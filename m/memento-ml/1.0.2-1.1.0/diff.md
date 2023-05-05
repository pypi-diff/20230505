# Comparing `tmp/memento-ml-1.0.2.tar.gz` & `tmp/memento-ml-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/xcha011/workspace/memento-wickerlab/dist/.tmp-32fnfzjt/memento-ml-1.0.2.tar", last modified: Wed Mar  1 22:15:01 2023, max compression
+gzip compressed data, was "memento-ml-1.1.0.tar", last modified: Thu May  4 22:47:59 2023, max compression
```

## Comparing `memento-ml-1.0.2.tar` & `memento-ml-1.1.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 xcha011  (375365)  1375365        0 2023-03-01 22:15:01.000000 memento-ml-1.0.2/
--rw-r--r--   0 xcha011  (375365)  1375365     1496 2023-03-01 21:32:27.000000 memento-ml-1.0.2/LICENSE
--rw-r--r--   0 xcha011  (375365)  1375365     7365 2023-03-01 22:15:01.000000 memento-ml-1.0.2/PKG-INFO
--rw-r--r--   0 xcha011  (375365)  1375365     5176 2023-03-01 21:32:27.000000 memento-ml-1.0.2/README.md
-drwxr-xr-x   0 xcha011  (375365)  1375365        0 2023-03-01 22:15:01.000000 memento-ml-1.0.2/memento/
--rw-r--r--   0 xcha011  (375365)  1375365     1594 2023-03-01 22:14:06.000000 memento-ml-1.0.2/memento/__init__.py
--rw-r--r--   0 xcha011  (375365)  1375365     9082 2023-03-01 21:32:27.000000 memento-ml-1.0.2/memento/caching.py
--rw-r--r--   0 xcha011  (375365)  1375365     3451 2023-03-01 21:32:27.000000 memento-ml-1.0.2/memento/configurations.py
--rw-r--r--   0 xcha011  (375365)  1375365     1099 2023-03-01 21:32:27.000000 memento-ml-1.0.2/memento/exceptions.py
--rw-r--r--   0 xcha011  (375365)  1375365     8022 2023-03-01 21:32:27.000000 memento-ml-1.0.2/memento/memento.py
--rw-r--r--   0 xcha011  (375365)  1375365     6438 2023-03-01 21:32:27.000000 memento-ml-1.0.2/memento/notifications.py
--rw-r--r--   0 xcha011  (375365)  1375365     6593 2023-03-01 21:32:27.000000 memento-ml-1.0.2/memento/parallel.py
--rw-r--r--   0 xcha011  (375365)  1375365     9894 2023-03-01 21:32:27.000000 memento-ml-1.0.2/memento/task_interface.py
-drwxr-xr-x   0 xcha011  (375365)  1375365        0 2023-03-01 22:15:01.000000 memento-ml-1.0.2/memento_ml.egg-info/
--rw-r--r--   0 xcha011  (375365)  1375365     7365 2023-03-01 22:15:01.000000 memento-ml-1.0.2/memento_ml.egg-info/PKG-INFO
--rw-r--r--   0 xcha011  (375365)  1375365      540 2023-03-01 22:15:01.000000 memento-ml-1.0.2/memento_ml.egg-info/SOURCES.txt
--rw-r--r--   0 xcha011  (375365)  1375365        1 2023-03-01 22:15:01.000000 memento-ml-1.0.2/memento_ml.egg-info/dependency_links.txt
--rw-r--r--   0 xcha011  (375365)  1375365      156 2023-03-01 22:15:01.000000 memento-ml-1.0.2/memento_ml.egg-info/requires.txt
--rw-r--r--   0 xcha011  (375365)  1375365        8 2023-03-01 22:15:01.000000 memento-ml-1.0.2/memento_ml.egg-info/top_level.txt
--rw-r--r--   0 xcha011  (375365)  1375365     1747 2023-03-01 22:14:06.000000 memento-ml-1.0.2/pyproject.toml
--rw-r--r--   0 xcha011  (375365)  1375365       38 2023-03-01 22:15:01.000000 memento-ml-1.0.2/setup.cfg
--rw-r--r--   0 xcha011  (375365)  1375365       38 2023-03-01 21:32:27.000000 memento-ml-1.0.2/setup.py
-drwxr-xr-x   0 xcha011  (375365)  1375365        0 2023-03-01 22:15:01.000000 memento-ml-1.0.2/tests/
--rw-r--r--   0 xcha011  (375365)  1375365     8683 2023-03-01 21:32:27.000000 memento-ml-1.0.2/tests/test_caching.py
--rw-r--r--   0 xcha011  (375365)  1375365     2660 2023-03-01 21:32:27.000000 memento-ml-1.0.2/tests/test_configurations.py
--rw-r--r--   0 xcha011  (375365)  1375365     5949 2023-03-01 21:32:27.000000 memento-ml-1.0.2/tests/test_memento.py
--rw-r--r--   0 xcha011  (375365)  1375365     5942 2023-03-01 21:32:27.000000 memento-ml-1.0.2/tests/test_notifications.py
--rw-r--r--   0 xcha011  (375365)  1375365     3578 2023-03-01 21:32:27.000000 memento-ml-1.0.2/tests/test_parallel.py
--rw-r--r--   0 xcha011  (375365)  1375365     5676 2023-03-01 21:32:27.000000 memento-ml-1.0.2/tests/test_task_interface.py
+drwxrwxrwx   0        0        0        0 2023-05-04 22:47:59.029466 memento-ml-1.1.0/
+-rw-rw-rw-   0        0        0     1524 2023-05-02 21:21:49.000000 memento-ml-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0     7847 2023-05-04 22:47:59.029466 memento-ml-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     5360 2023-05-02 21:21:49.000000 memento-ml-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-04 22:47:59.022463 memento-ml-1.1.0/memento/
+-rw-rw-rw-   0        0        0     1657 2023-05-02 21:21:49.000000 memento-ml-1.1.0/memento/__init__.py
+-rw-rw-rw-   0        0        0     9892 2023-05-03 04:24:04.000000 memento-ml-1.1.0/memento/caching.py
+-rw-rw-rw-   0        0        0     4055 2023-05-04 22:44:14.000000 memento-ml-1.1.0/memento/configurations.py
+-rw-rw-rw-   0        0        0     1099 2023-05-02 21:21:49.000000 memento-ml-1.1.0/memento/exceptions.py
+-rw-rw-rw-   0        0        0     8277 2023-05-02 22:58:43.000000 memento-ml-1.1.0/memento/memento.py
+-rw-rw-rw-   0        0        0     6657 2023-05-02 21:21:49.000000 memento-ml-1.1.0/memento/notifications.py
+-rw-rw-rw-   0        0        0     6817 2023-05-02 21:21:49.000000 memento-ml-1.1.0/memento/parallel.py
+-rw-rw-rw-   0        0        0    10207 2023-05-02 21:21:49.000000 memento-ml-1.1.0/memento/task_interface.py
+drwxrwxrwx   0        0        0        0 2023-05-04 22:47:59.025463 memento-ml-1.1.0/memento_ml.egg-info/
+-rw-rw-rw-   0        0        0     7847 2023-05-04 22:47:59.000000 memento-ml-1.1.0/memento_ml.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      540 2023-05-04 22:47:59.000000 memento-ml-1.1.0/memento_ml.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-04 22:47:59.000000 memento-ml-1.1.0/memento_ml.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      145 2023-05-04 22:47:59.000000 memento-ml-1.1.0/memento_ml.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-04 22:47:59.000000 memento-ml-1.1.0/memento_ml.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1849 2023-05-02 23:53:40.000000 memento-ml-1.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-04 22:47:59.029466 memento-ml-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0       41 2023-05-02 21:21:49.000000 memento-ml-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-04 22:47:59.028461 memento-ml-1.1.0/tests/
+-rw-rw-rw-   0        0        0     9494 2023-05-02 21:21:49.000000 memento-ml-1.1.0/tests/test_caching.py
+-rw-rw-rw-   0        0        0     2749 2023-05-02 21:21:49.000000 memento-ml-1.1.0/tests/test_configurations.py
+-rw-rw-rw-   0        0        0     6022 2023-05-02 23:09:06.000000 memento-ml-1.1.0/tests/test_memento.py
+-rw-rw-rw-   0        0        0     6135 2023-05-02 21:21:49.000000 memento-ml-1.1.0/tests/test_notifications.py
+-rw-rw-rw-   0        0        0     3719 2023-05-02 23:26:33.000000 memento-ml-1.1.0/tests/test_parallel.py
+-rw-rw-rw-   0        0        0     5846 2023-05-02 23:48:57.000000 memento-ml-1.1.0/tests/test_task_interface.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `memento-ml-1.0.2/LICENSE` & `memento-ml-1.1.0/LICENSE`

 * *Ordering differences only*

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-BSD 3-Clause License
-
-Copyright (c) 2023, wickerlab
-
-Redistribution and use in source and binary forms, with or without
-modification, are permitted provided that the following conditions are met:
-
-1. Redistributions of source code must retain the above copyright notice, this
-   list of conditions and the following disclaimer.
-
-2. Redistributions in binary form must reproduce the above copyright notice,
-   this list of conditions and the following disclaimer in the documentation
-   and/or other materials provided with the distribution.
-
-3. Neither the name of the copyright holder nor the names of its
-   contributors may be used to endorse or promote products derived from
-   this software without specific prior written permission.
-
-THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
-AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
-IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
-DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
-FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
-DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
-SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
-CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
-OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
-OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+BSD 3-Clause License
+
+Copyright (c) 2023, wickerlab
+
+Redistribution and use in source and binary forms, with or without
+modification, are permitted provided that the following conditions are met:
+
+1. Redistributions of source code must retain the above copyright notice, this
+   list of conditions and the following disclaimer.
+
+2. Redistributions in binary form must reproduce the above copyright notice,
+   this list of conditions and the following disclaimer in the documentation
+   and/or other materials provided with the distribution.
+
+3. Neither the name of the copyright holder nor the names of its
+   contributors may be used to endorse or promote products derived from
+   this software without specific prior written permission.
+
+THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
+FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
+DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
+SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
+CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
+OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
+OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```

### Comparing `memento-ml-1.0.2/PKG-INFO` & `memento-ml-1.1.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,251 +1,202 @@
-Metadata-Version: 2.1
-Name: memento-ml
-Version: 1.0.2
-Summary: A Python library for running computationally expensive experiments
-Author-email: Wickerlab dev team <luke.x.chang@gmail.com>
-License: BSD 3-Clause License
-        
-        Copyright (c) 2023, wickerlab
-        
-        Redistribution and use in source and binary forms, with or without
-        modification, are permitted provided that the following conditions are met:
-        
-        1. Redistributions of source code must retain the above copyright notice, this
-           list of conditions and the following disclaimer.
-        
-        2. Redistributions in binary form must reproduce the above copyright notice,
-           this list of conditions and the following disclaimer in the documentation
-           and/or other materials provided with the distribution.
-        
-        3. Neither the name of the copyright holder nor the names of its
-           contributors may be used to endorse or promote products derived from
-           this software without specific prior written permission.
-        
-        THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
-        AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
-        IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
-        DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
-        FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
-        DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
-        SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
-        CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
-        OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
-        OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
-        
-Project-URL: Homepage, https://github.com/wickerlab/memento
-Keywords: experiment,parallel,sklearn,machine learning
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Requires-Python: <3.10,>=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
-[![PyPI](https://img.shields.io/pypi/v/memento-ml)](https://pypi.org/project/memento-ml/)
-![Python versions](https://img.shields.io/pypi/pyversions/memento-ml)
-
-# Memento
-
-Memento is a Python library for running computationally expensive experiments.
-
-If you need to run a large number of time-consuming experiments Memento can help:
-
-- Structure your configuration
-- Parallelize experiments across CPUs
-- Save and restore results
-- Checkpoint in-progress experiments
-- Send notifications when experiments fail or finish
-
-## Getting Started
-
-### Install
-
-```bash
-pip install memento-ml
-```
-
-### The Configuration Matrix
-
-The core of Memento is a configuration `matrix` that describes the list of experiments you
-want Memento to run. This must contain a key `parameters` which is itself a dict, this describes
-each paramter you want to vary for your experiments and their values.
-
-As an example let's say you wanted to test a few simple linear classifiers on a number of
-image recognition datasets. You might write something like this:
-
-> Don't worry if you're not working on machine learning, this is just an example.
-
-```python
-matrix = {
-  "parameters": {
-    "model": [
-      sklearn.svm.SVC,
-      sklearn.linear_model.Perceptron,
-      sklearn.linear_model.LogisticRegression
-    ],
-    "dataset": ["imagenet", "mnist", "cifar10", "quickdraw"]
-  }
-}
-```
-
-Memento would then generate 12 configurations by taking the _cartesian product_ of the
-parameters.
-
-Frequently you might also want to set some global configuration values, such as a regularization
-parameter or potentially even change your preprocessing pipeline. In this case Memento also
-accepts a "settings" key. These settings apply to all experiments and can be accessed from the
-configuration list as well as individual configurations.
-
-```python
-matrix = {
-  "parameters": ...,
-  "settings": {
-    "regularization": 1e-1,
-    "preprocessing": make_preprocessing_pipeline()
-  }
-}
-```
-
-You can also exclude specific parameter configurations. Returning to our machine learning
-example, if you know SVCs perform poorly on cifar10 you might decide to skip that
-experiment entirely. This is done with the "exclude" key:
-
-```python
-matrix = {
-  "parameters": ...,
-  "exclude": [
-    {"model": sklearn.svm.SVC, "dataset": "cifar10"}
-  ]
-}
-```
-
-### Running an experiment
-
-Along with a configuration matrix you need some code to run your experiments. This can be any
-`Callable` such as a function, lambda, class, or class method.
-
-```python
-from memento import Memento, Config, Context
-
-def experiment(context: Context, config: Config):
-  classifier = config.model()
-  dataset = fetch_dataset(config.dataset)
-
-  classifier.fit(*dataset)
-
-  return classifier
-
-Memento(experiment).run(matrix)
-```
-
-You can also perform a dry run to check you've gotten the matrix correct.
-
-```python
-Memento(experiment).run(matrix, dry_run=True)
-```
-
-```python
-Running configurations:
-  {'model': sklearn.svm.SVC, 'dataset': 'imagenet'}
-  {'model': sklearn.svm.SVC, 'dataset': 'mnist'}
-  {'model': sklearn.svm.SVC, 'dataset': 'cifar10'}
-  {'model': sklearn.svm.SVC, 'dataset': 'quickdraw'}
-  {'model': sklearn.linear_model.Perceptron, 'dataset': 'imagenet'}
-  ...
-Exiting due to dry run
-```
-
-## Code demo
-
-- Code demo can be found [here](demo).
-- `Memento` does not depend on `scikit-learn`. The `scikit-learn` and `jupyterlab` packages are required to run the demo (`./demo/*`).
-
-```bash
-pip install scikit-learn jupyterlab
-```
-
-## Developing
-
-### Install as local package in Editable mode
-
-```bash
-pip install -e .
-
-```
-
-### Install development dependencies
-
-```bash
-pip install memento-ml[dev]
-```
-
-### Tests
-
-```bash
-pytest
-```
-
-Alternatively to only run a subset of tests that haven't been marked as time consuming/slow you can use:
-
-```bash
-pytest -m "not slow"
-```
-
-### Linters
-
-```bash
-pylint memento
-```
-
-### Format code
-
-```bash
-black .
-```
-
-### Build Documentation
-
-```bash
-sphinx-apidoc -o docs memento -f
-sphinx-build -W -b html docs docs/_build
-```
-
-### Bump up version
-
-```bash
-# The `--dry` flag is for testing only. Remove `--dry` to update the version number.
-# Use `minor` instead of `patch` for feature updates.
-bumpver update --patch --dry
-```
-
-### Run CI locally
-
-Install [act](https://github.com/nektos/act), then:
-
-```bash
-act
-```
-
-## Roadmap
-
-- Finish HPC support
-- Improve result serialisation
-- Production testing & fleshed-out integration test suite
-
-## Contributors
-
-- [Zac Pullar-Strecker](https://github.com/zacps)
-- [Feras Albaroudi](https://github.com/NeedsSoySauce)
-- [Liam Scott-Russell](https://github.com/Liam-Scott-Russell)
-- [Joshua de Wet](https://github.com/Dewera)
-- [Nipun Jasti](https://github.com/watefeenex)
-- [James Lamberton](https://github.com/JamesLamberton)
-- [Joerg Wicker](https://github.com/joergwicker)
-- [Xinglong (Luke) Chang](https://github.com/changx03)
-
-## License
-
-Memento is licensed under the [3-Clause BSD License](https://opensource.org/licenses/BSD-3-Clause) license.
+Metadata-Version: 2.1
+Name: memento-ml
+Version: 1.1.0
+Summary: A Python library for running computationally expensive experiments
+Author-email: Wickerlab dev team <luke.x.chang@gmail.com>
+License: BSD 3-Clause License
+        
+        Copyright (c) 2023, wickerlab
+        
+        Redistribution and use in source and binary forms, with or without
+        modification, are permitted provided that the following conditions are met:
+        
+        1. Redistributions of source code must retain the above copyright notice, this
+           list of conditions and the following disclaimer.
+        
+        2. Redistributions in binary form must reproduce the above copyright notice,
+           this list of conditions and the following disclaimer in the documentation
+           and/or other materials provided with the distribution.
+        
+        3. Neither the name of the copyright holder nor the names of its
+           contributors may be used to endorse or promote products derived from
+           this software without specific prior written permission.
+        
+        THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+        AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+        IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+        DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
+        FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
+        DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
+        SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
+        CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
+        OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
+        OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+        
+Project-URL: Homepage, https://github.com/wickerlab/memento
+Keywords: experiment,parallel,sklearn,machine learning
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+License-File: LICENSE
+
+[![PyPI](https://img.shields.io/pypi/v/memento-ml)](https://pypi.org/project/memento-ml/)
+![Python versions](https://img.shields.io/pypi/pyversions/memento-ml)
+
+# MEMENTO
+
+`MEMENTO` is a Python library for running computationally expensive experiments.
+
+Running complex sets of machine learning experiments is challenging and time-consuming due to the lack of a unified framework.
+This leaves researchers forced to spend time implementing necessary features such as parallelization, caching, and checkpointing themselves instead of focussing on their project.
+To simplify the process, we introduce `MEMENTO`, a Python package that is designed to aid researchers and data scientists in the efficient management and execution of computationally intensive experiments.
+`MEMENTO` has the capacity to streamline any experimental pipeline by providing a straightforward configuration matrix and the ability to concurrently run experiments across multiple threads.
+
+If you need to run a large number of time-consuming experiments `MEMENTO` can help:
+
+- Structure your configuration
+- Parallelize experiments across CPUs
+- Save and restore results
+- Checkpoint in-progress experiments
+- Send notifications when experiments fail or finish
+
+[![Demo video](https://img.youtube.com/vi/GEtdCl1ZUWc/0.jpg)](http://www.youtube.com/watch?v=GEtdCl1ZUWc)
+
+## Getting Started
+
+`MEMENTO` is officially available on PyPl. To install the package:
+
+### Install
+
+```bash
+pip install memento-ml
+```
+
+### The Configuration Matrix
+
+The core of `MEMENTO` is a configuration `matrix` that describes the list of experiments you
+want `MEMENTO` to run. This must contain a key `parameters` which is itself a dict, this describes
+each paramter you want to vary for your experiments and their values.
+
+As an example let's say you wanted to test a few simple linear classifiers on a number of
+image recognition datasets. You might write something like this:
+
+> Don't worry if you're not working on machine learning, this is just an example.
+
+```python
+matrix = {
+  "parameters": {
+    "model": [
+      sklearn.svm.SVC,
+      sklearn.linear_model.Perceptron,
+      sklearn.linear_model.LogisticRegression
+    ],
+    "dataset": ["imagenet", "mnist", "cifar10", "quickdraw"]
+  }
+}
+```
+
+`MEMENTO` would then generate 12 configurations by taking the _cartesian product_ of the
+parameters.
+
+Frequently you might also want to set some global configuration values, such as a regularization
+parameter or potentially even change your preprocessing pipeline. In this case `MEMENTO` also
+accepts a "settings" key. These settings apply to all experiments and can be accessed from the
+configuration list as well as individual configurations.
+
+```python
+matrix = {
+  "parameters": ...,
+  "settings": {
+    "regularization": 1e-1,
+    "preprocessing": make_preprocessing_pipeline()
+  }
+}
+```
+
+You can also exclude specific parameter configurations. Returning to our machine learning
+example, if you know SVCs perform poorly on cifar10 you might decide to skip that
+experiment entirely. This is done with the "exclude" key:
+
+```python
+matrix = {
+  "parameters": ...,
+  "exclude": [
+    {"model": sklearn.svm.SVC, "dataset": "cifar10"}
+  ]
+}
+```
+
+### Running an experiment
+
+Along with a configuration matrix you need some code to run your experiments. This can be any
+`Callable` such as a function, lambda, class, or class method.
+
+```python
+from memento import Memento, Config, Context
+
+def experiment(context: Context, config: Config):
+  classifier = config.model()
+  dataset = fetch_dataset(config.dataset)
+
+  classifier.fit(*dataset)
+
+  return classifier
+
+Memento(experiment).run(matrix)
+```
+
+You can also perform a dry run to check you've gotten the matrix correct.
+
+```python
+Memento(experiment).run(matrix, dry_run=True)
+```
+
+```python
+Running configurations:
+  {'model': sklearn.svm.SVC, 'dataset': 'imagenet'}
+  {'model': sklearn.svm.SVC, 'dataset': 'mnist'}
+  {'model': sklearn.svm.SVC, 'dataset': 'cifar10'}
+  {'model': sklearn.svm.SVC, 'dataset': 'quickdraw'}
+  {'model': sklearn.linear_model.Perceptron, 'dataset': 'imagenet'}
+  ...
+Exiting due to dry run
+```
+
+## Code demo
+
+- Code demo can be found [here](demo).
+- `MEMENTO` does not depend on any ML packages, e.g., `scikit-learn`. The `scikit-learn` and `jupyterlab` packages are required to run the demo (`./demo/*`).
+
+```bash
+pip install memento-ml scikit-learn jupyterlab
+```
+
+## Roadmap
+
+- Finish HPC support
+- Improve result serialisation
+- Improve customization for notification
+
+## Contributors
+
+- [Zac Pullar-Strecker](https://github.com/zacps)
+- [Feras Albaroudi](https://github.com/NeedsSoySauce)
+- [Liam Scott-Russell](https://github.com/Liam-Scott-Russell)
+- [Joshua de Wet](https://github.com/Dewera)
+- [Nipun Jasti](https://github.com/watefeenex)
+- [James Lamberton](https://github.com/JamesLamberton)
+- [Xinglong (Luke) Chang](https://github.com/changx03)
+- [Liam Brydon](https://github.com/MyCreativityOutlet)
+- [Ioannis Ziogas](izio995@aucklanduni.ac.nz)
+- [Katharina Dost](katharina.dost@auckland.ac.nz)
+- [Joerg Wicker](https://github.com/joergwicker)
+
+## License
+
+MEMENTO is licensed under the [3-Clause BSD License](https://opensource.org/licenses/BSD-3-Clause) license.
```

### Comparing `memento-ml-1.0.2/README.md` & `memento-ml-1.1.0/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -4,321 +4,332 @@
 00000030: 6c29 5d28 6874 7470 733a 2f2f 7079 7069  l)](https://pypi
 00000040: 2e6f 7267 2f70 726f 6a65 6374 2f6d 656d  .org/project/mem
 00000050: 656e 746f 2d6d 6c2f 290d 0a21 5b50 7974  ento-ml/)..![Pyt
 00000060: 686f 6e20 7665 7273 696f 6e73 5d28 6874  hon versions](ht
 00000070: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
 00000080: 732e 696f 2f70 7970 692f 7079 7665 7273  s.io/pypi/pyvers
 00000090: 696f 6e73 2f6d 656d 656e 746f 2d6d 6c29  ions/memento-ml)
-000000a0: 0d0a 0d0a 2320 4d65 6d65 6e74 6f0d 0a0d  ....# Memento...
-000000b0: 0a4d 656d 656e 746f 2069 7320 6120 5079  .Memento is a Py
-000000c0: 7468 6f6e 206c 6962 7261 7279 2066 6f72  thon library for
-000000d0: 2072 756e 6e69 6e67 2063 6f6d 7075 7461   running computa
-000000e0: 7469 6f6e 616c 6c79 2065 7870 656e 7369  tionally expensi
-000000f0: 7665 2065 7870 6572 696d 656e 7473 2e0d  ve experiments..
-00000100: 0a0d 0a49 6620 796f 7520 6e65 6564 2074  ...If you need t
-00000110: 6f20 7275 6e20 6120 6c61 7267 6520 6e75  o run a large nu
-00000120: 6d62 6572 206f 6620 7469 6d65 2d63 6f6e  mber of time-con
-00000130: 7375 6d69 6e67 2065 7870 6572 696d 656e  suming experimen
-00000140: 7473 204d 656d 656e 746f 2063 616e 2068  ts Memento can h
-00000150: 656c 703a 0d0a 0d0a 2d20 5374 7275 6374  elp:....- Struct
-00000160: 7572 6520 796f 7572 2063 6f6e 6669 6775  ure your configu
-00000170: 7261 7469 6f6e 0d0a 2d20 5061 7261 6c6c  ration..- Parall
-00000180: 656c 697a 6520 6578 7065 7269 6d65 6e74  elize experiment
-00000190: 7320 6163 726f 7373 2043 5055 730d 0a2d  s across CPUs..-
-000001a0: 2053 6176 6520 616e 6420 7265 7374 6f72   Save and restor
-000001b0: 6520 7265 7375 6c74 730d 0a2d 2043 6865  e results..- Che
-000001c0: 636b 706f 696e 7420 696e 2d70 726f 6772  ckpoint in-progr
-000001d0: 6573 7320 6578 7065 7269 6d65 6e74 730d  ess experiments.
-000001e0: 0a2d 2053 656e 6420 6e6f 7469 6669 6361  .- Send notifica
-000001f0: 7469 6f6e 7320 7768 656e 2065 7870 6572  tions when exper
-00000200: 696d 656e 7473 2066 6169 6c20 6f72 2066  iments fail or f
-00000210: 696e 6973 680d 0a0d 0a23 2320 4765 7474  inish....## Gett
-00000220: 696e 6720 5374 6172 7465 640d 0a0d 0a23  ing Started....#
-00000230: 2323 2049 6e73 7461 6c6c 0d0a 0d0a 6060  ## Install....``
-00000240: 6062 6173 680d 0a70 6970 2069 6e73 7461  `bash..pip insta
-00000250: 6c6c 206d 656d 656e 746f 2d6d 6c0d 0a60  ll memento-ml..`
-00000260: 6060 0d0a 0d0a 2323 2320 5468 6520 436f  ``....### The Co
-00000270: 6e66 6967 7572 6174 696f 6e20 4d61 7472  nfiguration Matr
-00000280: 6978 0d0a 0d0a 5468 6520 636f 7265 206f  ix....The core o
-00000290: 6620 4d65 6d65 6e74 6f20 6973 2061 2063  f Memento is a c
-000002a0: 6f6e 6669 6775 7261 7469 6f6e 2060 6d61  onfiguration `ma
-000002b0: 7472 6978 6020 7468 6174 2064 6573 6372  trix` that descr
-000002c0: 6962 6573 2074 6865 206c 6973 7420 6f66  ibes the list of
-000002d0: 2065 7870 6572 696d 656e 7473 2079 6f75   experiments you
-000002e0: 0d0a 7761 6e74 204d 656d 656e 746f 2074  ..want Memento t
-000002f0: 6f20 7275 6e2e 2054 6869 7320 6d75 7374  o run. This must
-00000300: 2063 6f6e 7461 696e 2061 206b 6579 2060   contain a key `
-00000310: 7061 7261 6d65 7465 7273 6020 7768 6963  parameters` whic
-00000320: 6820 6973 2069 7473 656c 6620 6120 6469  h is itself a di
-00000330: 6374 2c20 7468 6973 2064 6573 6372 6962  ct, this describ
-00000340: 6573 0d0a 6561 6368 2070 6172 616d 7465  es..each paramte
-00000350: 7220 796f 7520 7761 6e74 2074 6f20 7661  r you want to va
-00000360: 7279 2066 6f72 2079 6f75 7220 6578 7065  ry for your expe
-00000370: 7269 6d65 6e74 7320 616e 6420 7468 6569  riments and thei
-00000380: 7220 7661 6c75 6573 2e0d 0a0d 0a41 7320  r values.....As 
-00000390: 616e 2065 7861 6d70 6c65 206c 6574 2773  an example let's
-000003a0: 2073 6179 2079 6f75 2077 616e 7465 6420   say you wanted 
-000003b0: 746f 2074 6573 7420 6120 6665 7720 7369  to test a few si
-000003c0: 6d70 6c65 206c 696e 6561 7220 636c 6173  mple linear clas
-000003d0: 7369 6669 6572 7320 6f6e 2061 206e 756d  sifiers on a num
-000003e0: 6265 7220 6f66 0d0a 696d 6167 6520 7265  ber of..image re
-000003f0: 636f 676e 6974 696f 6e20 6461 7461 7365  cognition datase
-00000400: 7473 2e20 596f 7520 6d69 6768 7420 7772  ts. You might wr
-00000410: 6974 6520 736f 6d65 7468 696e 6720 6c69  ite something li
-00000420: 6b65 2074 6869 733a 0d0a 0d0a 3e20 446f  ke this:....> Do
-00000430: 6e27 7420 776f 7272 7920 6966 2079 6f75  n't worry if you
-00000440: 2772 6520 6e6f 7420 776f 726b 696e 6720  're not working 
-00000450: 6f6e 206d 6163 6869 6e65 206c 6561 726e  on machine learn
-00000460: 696e 672c 2074 6869 7320 6973 206a 7573  ing, this is jus
-00000470: 7420 616e 2065 7861 6d70 6c65 2e0d 0a0d  t an example....
-00000480: 0a60 6060 7079 7468 6f6e 0d0a 6d61 7472  .```python..matr
-00000490: 6978 203d 207b 0d0a 2020 2270 6172 616d  ix = {..  "param
-000004a0: 6574 6572 7322 3a20 7b0d 0a20 2020 2022  eters": {..    "
-000004b0: 6d6f 6465 6c22 3a20 5b0d 0a20 2020 2020  model": [..     
-000004c0: 2073 6b6c 6561 726e 2e73 766d 2e53 5643   sklearn.svm.SVC
-000004d0: 2c0d 0a20 2020 2020 2073 6b6c 6561 726e  ,..      sklearn
-000004e0: 2e6c 696e 6561 725f 6d6f 6465 6c2e 5065  .linear_model.Pe
-000004f0: 7263 6570 7472 6f6e 2c0d 0a20 2020 2020  rceptron,..     
-00000500: 2073 6b6c 6561 726e 2e6c 696e 6561 725f   sklearn.linear_
-00000510: 6d6f 6465 6c2e 4c6f 6769 7374 6963 5265  model.LogisticRe
-00000520: 6772 6573 7369 6f6e 0d0a 2020 2020 5d2c  gression..    ],
-00000530: 0d0a 2020 2020 2264 6174 6173 6574 223a  ..    "dataset":
-00000540: 205b 2269 6d61 6765 6e65 7422 2c20 226d   ["imagenet", "m
-00000550: 6e69 7374 222c 2022 6369 6661 7231 3022  nist", "cifar10"
-00000560: 2c20 2271 7569 636b 6472 6177 225d 0d0a  , "quickdraw"]..
-00000570: 2020 7d0d 0a7d 0d0a 6060 600d 0a0d 0a4d    }..}..```....M
-00000580: 656d 656e 746f 2077 6f75 6c64 2074 6865  emento would the
-00000590: 6e20 6765 6e65 7261 7465 2031 3220 636f  n generate 12 co
-000005a0: 6e66 6967 7572 6174 696f 6e73 2062 7920  nfigurations by 
-000005b0: 7461 6b69 6e67 2074 6865 205f 6361 7274  taking the _cart
-000005c0: 6573 6961 6e20 7072 6f64 7563 745f 206f  esian product_ o
-000005d0: 6620 7468 650d 0a70 6172 616d 6574 6572  f the..parameter
-000005e0: 732e 0d0a 0d0a 4672 6571 7565 6e74 6c79  s.....Frequently
-000005f0: 2079 6f75 206d 6967 6874 2061 6c73 6f20   you might also 
-00000600: 7761 6e74 2074 6f20 7365 7420 736f 6d65  want to set some
-00000610: 2067 6c6f 6261 6c20 636f 6e66 6967 7572   global configur
-00000620: 6174 696f 6e20 7661 6c75 6573 2c20 7375  ation values, su
-00000630: 6368 2061 7320 6120 7265 6775 6c61 7269  ch as a regulari
-00000640: 7a61 7469 6f6e 0d0a 7061 7261 6d65 7465  zation..paramete
-00000650: 7220 6f72 2070 6f74 656e 7469 616c 6c79  r or potentially
-00000660: 2065 7665 6e20 6368 616e 6765 2079 6f75   even change you
-00000670: 7220 7072 6570 726f 6365 7373 696e 6720  r preprocessing 
-00000680: 7069 7065 6c69 6e65 2e20 496e 2074 6869  pipeline. In thi
-00000690: 7320 6361 7365 204d 656d 656e 746f 2061  s case Memento a
-000006a0: 6c73 6f0d 0a61 6363 6570 7473 2061 2022  lso..accepts a "
-000006b0: 7365 7474 696e 6773 2220 6b65 792e 2054  settings" key. T
-000006c0: 6865 7365 2073 6574 7469 6e67 7320 6170  hese settings ap
-000006d0: 706c 7920 746f 2061 6c6c 2065 7870 6572  ply to all exper
-000006e0: 696d 656e 7473 2061 6e64 2063 616e 2062  iments and can b
-000006f0: 6520 6163 6365 7373 6564 2066 726f 6d20  e accessed from 
-00000700: 7468 650d 0a63 6f6e 6669 6775 7261 7469  the..configurati
-00000710: 6f6e 206c 6973 7420 6173 2077 656c 6c20  on list as well 
-00000720: 6173 2069 6e64 6976 6964 7561 6c20 636f  as individual co
-00000730: 6e66 6967 7572 6174 696f 6e73 2e0d 0a0d  nfigurations....
-00000740: 0a60 6060 7079 7468 6f6e 0d0a 6d61 7472  .```python..matr
-00000750: 6978 203d 207b 0d0a 2020 2270 6172 616d  ix = {..  "param
-00000760: 6574 6572 7322 3a20 2e2e 2e2c 0d0a 2020  eters": ...,..  
-00000770: 2273 6574 7469 6e67 7322 3a20 7b0d 0a20  "settings": {.. 
-00000780: 2020 2022 7265 6775 6c61 7269 7a61 7469     "regularizati
-00000790: 6f6e 223a 2031 652d 312c 0d0a 2020 2020  on": 1e-1,..    
-000007a0: 2270 7265 7072 6f63 6573 7369 6e67 223a  "preprocessing":
-000007b0: 206d 616b 655f 7072 6570 726f 6365 7373   make_preprocess
-000007c0: 696e 675f 7069 7065 6c69 6e65 2829 0d0a  ing_pipeline()..
-000007d0: 2020 7d0d 0a7d 0d0a 6060 600d 0a0d 0a59    }..}..```....Y
-000007e0: 6f75 2063 616e 2061 6c73 6f20 6578 636c  ou can also excl
-000007f0: 7564 6520 7370 6563 6966 6963 2070 6172  ude specific par
-00000800: 616d 6574 6572 2063 6f6e 6669 6775 7261  ameter configura
-00000810: 7469 6f6e 732e 2052 6574 7572 6e69 6e67  tions. Returning
-00000820: 2074 6f20 6f75 7220 6d61 6368 696e 6520   to our machine 
-00000830: 6c65 6172 6e69 6e67 0d0a 6578 616d 706c  learning..exampl
-00000840: 652c 2069 6620 796f 7520 6b6e 6f77 2053  e, if you know S
-00000850: 5643 7320 7065 7266 6f72 6d20 706f 6f72  VCs perform poor
-00000860: 6c79 206f 6e20 6369 6661 7231 3020 796f  ly on cifar10 yo
-00000870: 7520 6d69 6768 7420 6465 6369 6465 2074  u might decide t
-00000880: 6f20 736b 6970 2074 6861 740d 0a65 7870  o skip that..exp
-00000890: 6572 696d 656e 7420 656e 7469 7265 6c79  eriment entirely
-000008a0: 2e20 5468 6973 2069 7320 646f 6e65 2077  . This is done w
-000008b0: 6974 6820 7468 6520 2265 7863 6c75 6465  ith the "exclude
-000008c0: 2220 6b65 793a 0d0a 0d0a 6060 6070 7974  " key:....```pyt
-000008d0: 686f 6e0d 0a6d 6174 7269 7820 3d20 7b0d  hon..matrix = {.
-000008e0: 0a20 2022 7061 7261 6d65 7465 7273 223a  .  "parameters":
-000008f0: 202e 2e2e 2c0d 0a20 2022 6578 636c 7564   ...,..  "exclud
-00000900: 6522 3a20 5b0d 0a20 2020 207b 226d 6f64  e": [..    {"mod
-00000910: 656c 223a 2073 6b6c 6561 726e 2e73 766d  el": sklearn.svm
-00000920: 2e53 5643 2c20 2264 6174 6173 6574 223a  .SVC, "dataset":
-00000930: 2022 6369 6661 7231 3022 7d0d 0a20 205d   "cifar10"}..  ]
-00000940: 0d0a 7d0d 0a60 6060 0d0a 0d0a 2323 2320  ..}..```....### 
-00000950: 5275 6e6e 696e 6720 616e 2065 7870 6572  Running an exper
-00000960: 696d 656e 740d 0a0d 0a41 6c6f 6e67 2077  iment....Along w
-00000970: 6974 6820 6120 636f 6e66 6967 7572 6174  ith a configurat
-00000980: 696f 6e20 6d61 7472 6978 2079 6f75 206e  ion matrix you n
-00000990: 6565 6420 736f 6d65 2063 6f64 6520 746f  eed some code to
-000009a0: 2072 756e 2079 6f75 7220 6578 7065 7269   run your experi
-000009b0: 6d65 6e74 732e 2054 6869 7320 6361 6e20  ments. This can 
-000009c0: 6265 2061 6e79 0d0a 6043 616c 6c61 626c  be any..`Callabl
-000009d0: 6560 2073 7563 6820 6173 2061 2066 756e  e` such as a fun
-000009e0: 6374 696f 6e2c 206c 616d 6264 612c 2063  ction, lambda, c
-000009f0: 6c61 7373 2c20 6f72 2063 6c61 7373 206d  lass, or class m
-00000a00: 6574 686f 642e 0d0a 0d0a 6060 6070 7974  ethod.....```pyt
-00000a10: 686f 6e0d 0a66 726f 6d20 6d65 6d65 6e74  hon..from mement
-00000a20: 6f20 696d 706f 7274 204d 656d 656e 746f  o import Memento
-00000a30: 2c20 436f 6e66 6967 2c20 436f 6e74 6578  , Config, Contex
-00000a40: 740d 0a0d 0a64 6566 2065 7870 6572 696d  t....def experim
-00000a50: 656e 7428 636f 6e74 6578 743a 2043 6f6e  ent(context: Con
-00000a60: 7465 7874 2c20 636f 6e66 6967 3a20 436f  text, config: Co
-00000a70: 6e66 6967 293a 0d0a 2020 636c 6173 7369  nfig):..  classi
-00000a80: 6669 6572 203d 2063 6f6e 6669 672e 6d6f  fier = config.mo
-00000a90: 6465 6c28 290d 0a20 2064 6174 6173 6574  del()..  dataset
-00000aa0: 203d 2066 6574 6368 5f64 6174 6173 6574   = fetch_dataset
-00000ab0: 2863 6f6e 6669 672e 6461 7461 7365 7429  (config.dataset)
-00000ac0: 0d0a 0d0a 2020 636c 6173 7369 6669 6572  ....  classifier
-00000ad0: 2e66 6974 282a 6461 7461 7365 7429 0d0a  .fit(*dataset)..
-00000ae0: 0d0a 2020 7265 7475 726e 2063 6c61 7373  ..  return class
-00000af0: 6966 6965 720d 0a0d 0a4d 656d 656e 746f  ifier....Memento
-00000b00: 2865 7870 6572 696d 656e 7429 2e72 756e  (experiment).run
-00000b10: 286d 6174 7269 7829 0d0a 6060 600d 0a0d  (matrix)..```...
-00000b20: 0a59 6f75 2063 616e 2061 6c73 6f20 7065  .You can also pe
-00000b30: 7266 6f72 6d20 6120 6472 7920 7275 6e20  rform a dry run 
-00000b40: 746f 2063 6865 636b 2079 6f75 2776 6520  to check you've 
-00000b50: 676f 7474 656e 2074 6865 206d 6174 7269  gotten the matri
-00000b60: 7820 636f 7272 6563 742e 0d0a 0d0a 6060  x correct.....``
-00000b70: 6070 7974 686f 6e0d 0a4d 656d 656e 746f  `python..Memento
-00000b80: 2865 7870 6572 696d 656e 7429 2e72 756e  (experiment).run
-00000b90: 286d 6174 7269 782c 2064 7279 5f72 756e  (matrix, dry_run
-00000ba0: 3d54 7275 6529 0d0a 6060 600d 0a0d 0a60  =True)..```....`
-00000bb0: 6060 7079 7468 6f6e 0d0a 5275 6e6e 696e  ``python..Runnin
-00000bc0: 6720 636f 6e66 6967 7572 6174 696f 6e73  g configurations
-00000bd0: 3a0d 0a20 207b 276d 6f64 656c 273a 2073  :..  {'model': s
-00000be0: 6b6c 6561 726e 2e73 766d 2e53 5643 2c20  klearn.svm.SVC, 
-00000bf0: 2764 6174 6173 6574 273a 2027 696d 6167  'dataset': 'imag
-00000c00: 656e 6574 277d 0d0a 2020 7b27 6d6f 6465  enet'}..  {'mode
-00000c10: 6c27 3a20 736b 6c65 6172 6e2e 7376 6d2e  l': sklearn.svm.
-00000c20: 5356 432c 2027 6461 7461 7365 7427 3a20  SVC, 'dataset': 
-00000c30: 276d 6e69 7374 277d 0d0a 2020 7b27 6d6f  'mnist'}..  {'mo
-00000c40: 6465 6c27 3a20 736b 6c65 6172 6e2e 7376  del': sklearn.sv
-00000c50: 6d2e 5356 432c 2027 6461 7461 7365 7427  m.SVC, 'dataset'
-00000c60: 3a20 2763 6966 6172 3130 277d 0d0a 2020  : 'cifar10'}..  
-00000c70: 7b27 6d6f 6465 6c27 3a20 736b 6c65 6172  {'model': sklear
-00000c80: 6e2e 7376 6d2e 5356 432c 2027 6461 7461  n.svm.SVC, 'data
-00000c90: 7365 7427 3a20 2771 7569 636b 6472 6177  set': 'quickdraw
-00000ca0: 277d 0d0a 2020 7b27 6d6f 6465 6c27 3a20  '}..  {'model': 
-00000cb0: 736b 6c65 6172 6e2e 6c69 6e65 6172 5f6d  sklearn.linear_m
-00000cc0: 6f64 656c 2e50 6572 6365 7074 726f 6e2c  odel.Perceptron,
-00000cd0: 2027 6461 7461 7365 7427 3a20 2769 6d61   'dataset': 'ima
-00000ce0: 6765 6e65 7427 7d0d 0a20 202e 2e2e 0d0a  genet'}..  .....
-00000cf0: 4578 6974 696e 6720 6475 6520 746f 2064  Exiting due to d
-00000d00: 7279 2072 756e 0d0a 6060 600d 0a0d 0a23  ry run..```....#
-00000d10: 2320 436f 6465 2064 656d 6f0d 0a0d 0a2d  # Code demo....-
-00000d20: 2043 6f64 6520 6465 6d6f 2063 616e 2062   Code demo can b
-00000d30: 6520 666f 756e 6420 5b68 6572 655d 2864  e found [here](d
-00000d40: 656d 6f29 2e0d 0a2d 2060 4d65 6d65 6e74  emo)...- `Mement
-00000d50: 6f60 2064 6f65 7320 6e6f 7420 6465 7065  o` does not depe
-00000d60: 6e64 206f 6e20 6073 6369 6b69 742d 6c65  nd on `scikit-le
-00000d70: 6172 6e60 2e20 5468 6520 6073 6369 6b69  arn`. The `sciki
-00000d80: 742d 6c65 6172 6e60 2061 6e64 2060 6a75  t-learn` and `ju
-00000d90: 7079 7465 726c 6162 6020 7061 636b 6167  pyterlab` packag
-00000da0: 6573 2061 7265 2072 6571 7569 7265 6420  es are required 
-00000db0: 746f 2072 756e 2074 6865 2064 656d 6f20  to run the demo 
-00000dc0: 2860 2e2f 6465 6d6f 2f2a 6029 2e0d 0a0d  (`./demo/*`)....
-00000dd0: 0a60 6060 6261 7368 0d0a 7069 7020 696e  .```bash..pip in
-00000de0: 7374 616c 6c20 7363 696b 6974 2d6c 6561  stall scikit-lea
-00000df0: 726e 206a 7570 7974 6572 6c61 620d 0a60  rn jupyterlab..`
-00000e00: 6060 0d0a 0d0a 2323 2044 6576 656c 6f70  ``....## Develop
-00000e10: 696e 670d 0a0d 0a23 2323 2049 6e73 7461  ing....### Insta
-00000e20: 6c6c 2061 7320 6c6f 6361 6c20 7061 636b  ll as local pack
-00000e30: 6167 6520 696e 2045 6469 7461 626c 6520  age in Editable 
-00000e40: 6d6f 6465 0d0a 0d0a 6060 6062 6173 680d  mode....```bash.
-00000e50: 0a70 6970 2069 6e73 7461 6c6c 202d 6520  .pip install -e 
-00000e60: 2e0d 0a0d 0a60 6060 0d0a 0d0a 2323 2320  .....```....### 
-00000e70: 496e 7374 616c 6c20 6465 7665 6c6f 706d  Install developm
-00000e80: 656e 7420 6465 7065 6e64 656e 6369 6573  ent dependencies
-00000e90: 0d0a 0d0a 6060 6062 6173 680d 0a70 6970  ....```bash..pip
-00000ea0: 2069 6e73 7461 6c6c 206d 656d 656e 746f   install memento
-00000eb0: 2d6d 6c5b 6465 765d 0d0a 6060 600d 0a0d  -ml[dev]..```...
-00000ec0: 0a23 2323 2054 6573 7473 0d0a 0d0a 6060  .### Tests....``
-00000ed0: 6062 6173 680d 0a70 7974 6573 740d 0a60  `bash..pytest..`
-00000ee0: 6060 0d0a 0d0a 416c 7465 726e 6174 6976  ``....Alternativ
-00000ef0: 656c 7920 746f 206f 6e6c 7920 7275 6e20  ely to only run 
-00000f00: 6120 7375 6273 6574 206f 6620 7465 7374  a subset of test
-00000f10: 7320 7468 6174 2068 6176 656e 2774 2062  s that haven't b
-00000f20: 6565 6e20 6d61 726b 6564 2061 7320 7469  een marked as ti
-00000f30: 6d65 2063 6f6e 7375 6d69 6e67 2f73 6c6f  me consuming/slo
-00000f40: 7720 796f 7520 6361 6e20 7573 653a 0d0a  w you can use:..
-00000f50: 0d0a 6060 6062 6173 680d 0a70 7974 6573  ..```bash..pytes
-00000f60: 7420 2d6d 2022 6e6f 7420 736c 6f77 220d  t -m "not slow".
-00000f70: 0a60 6060 0d0a 0d0a 2323 2320 4c69 6e74  .```....### Lint
-00000f80: 6572 730d 0a0d 0a60 6060 6261 7368 0d0a  ers....```bash..
-00000f90: 7079 6c69 6e74 206d 656d 656e 746f 0d0a  pylint memento..
-00000fa0: 6060 600d 0a0d 0a23 2323 2046 6f72 6d61  ```....### Forma
-00000fb0: 7420 636f 6465 0d0a 0d0a 6060 6062 6173  t code....```bas
-00000fc0: 680d 0a62 6c61 636b 202e 0d0a 6060 600d  h..black ...```.
-00000fd0: 0a0d 0a23 2323 2042 7569 6c64 2044 6f63  ...### Build Doc
-00000fe0: 756d 656e 7461 7469 6f6e 0d0a 0d0a 6060  umentation....``
-00000ff0: 6062 6173 680d 0a73 7068 696e 782d 6170  `bash..sphinx-ap
-00001000: 6964 6f63 202d 6f20 646f 6373 206d 656d  idoc -o docs mem
-00001010: 656e 746f 202d 660d 0a73 7068 696e 782d  ento -f..sphinx-
-00001020: 6275 696c 6420 2d57 202d 6220 6874 6d6c  build -W -b html
-00001030: 2064 6f63 7320 646f 6373 2f5f 6275 696c   docs docs/_buil
-00001040: 640d 0a60 6060 0d0a 0d0a 2323 2320 4275  d..```....### Bu
-00001050: 6d70 2075 7020 7665 7273 696f 6e0d 0a0d  mp up version...
-00001060: 0a60 6060 6261 7368 0d0a 2320 5468 6520  .```bash..# The 
-00001070: 602d 2d64 7279 6020 666c 6167 2069 7320  `--dry` flag is 
-00001080: 666f 7220 7465 7374 696e 6720 6f6e 6c79  for testing only
-00001090: 2e20 5265 6d6f 7665 2060 2d2d 6472 7960  . Remove `--dry`
-000010a0: 2074 6f20 7570 6461 7465 2074 6865 2076   to update the v
-000010b0: 6572 7369 6f6e 206e 756d 6265 722e 0d0a  ersion number...
-000010c0: 2320 5573 6520 606d 696e 6f72 6020 696e  # Use `minor` in
-000010d0: 7374 6561 6420 6f66 2060 7061 7463 6860  stead of `patch`
-000010e0: 2066 6f72 2066 6561 7475 7265 2075 7064   for feature upd
-000010f0: 6174 6573 2e0d 0a62 756d 7076 6572 2075  ates...bumpver u
-00001100: 7064 6174 6520 2d2d 7061 7463 6820 2d2d  pdate --patch --
-00001110: 6472 790d 0a60 6060 0d0a 0d0a 2323 2320  dry..```....### 
-00001120: 5275 6e20 4349 206c 6f63 616c 6c79 0d0a  Run CI locally..
-00001130: 0d0a 496e 7374 616c 6c20 5b61 6374 5d28  ..Install [act](
-00001140: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00001150: 6f6d 2f6e 656b 746f 732f 6163 7429 2c20  om/nektos/act), 
-00001160: 7468 656e 3a0d 0a0d 0a60 6060 6261 7368  then:....```bash
-00001170: 0d0a 6163 740d 0a60 6060 0d0a 0d0a 2323  ..act..```....##
-00001180: 2052 6f61 646d 6170 0d0a 0d0a 2d20 4669   Roadmap....- Fi
-00001190: 6e69 7368 2048 5043 2073 7570 706f 7274  nish HPC support
-000011a0: 0d0a 2d20 496d 7072 6f76 6520 7265 7375  ..- Improve resu
-000011b0: 6c74 2073 6572 6961 6c69 7361 7469 6f6e  lt serialisation
-000011c0: 0d0a 2d20 5072 6f64 7563 7469 6f6e 2074  ..- Production t
-000011d0: 6573 7469 6e67 2026 2066 6c65 7368 6564  esting & fleshed
-000011e0: 2d6f 7574 2069 6e74 6567 7261 7469 6f6e  -out integration
-000011f0: 2074 6573 7420 7375 6974 650d 0a0d 0a23   test suite....#
-00001200: 2320 436f 6e74 7269 6275 746f 7273 0d0a  # Contributors..
-00001210: 0d0a 2d20 5b5a 6163 2050 756c 6c61 722d  ..- [Zac Pullar-
-00001220: 5374 7265 636b 6572 5d28 6874 7470 733a  Strecker](https:
-00001230: 2f2f 6769 7468 7562 2e63 6f6d 2f7a 6163  //github.com/zac
-00001240: 7073 290d 0a2d 205b 4665 7261 7320 416c  ps)..- [Feras Al
-00001250: 6261 726f 7564 695d 2868 7474 7073 3a2f  baroudi](https:/
-00001260: 2f67 6974 6875 622e 636f 6d2f 4e65 6564  /github.com/Need
-00001270: 7353 6f79 5361 7563 6529 0d0a 2d20 5b4c  sSoySauce)..- [L
-00001280: 6961 6d20 5363 6f74 742d 5275 7373 656c  iam Scott-Russel
-00001290: 6c5d 2868 7474 7073 3a2f 2f67 6974 6875  l](https://githu
-000012a0: 622e 636f 6d2f 4c69 616d 2d53 636f 7474  b.com/Liam-Scott
-000012b0: 2d52 7573 7365 6c6c 290d 0a2d 205b 4a6f  -Russell)..- [Jo
-000012c0: 7368 7561 2064 6520 5765 745d 2868 7474  shua de Wet](htt
-000012d0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-000012e0: 4465 7765 7261 290d 0a2d 205b 4e69 7075  Dewera)..- [Nipu
-000012f0: 6e20 4a61 7374 695d 2868 7474 7073 3a2f  n Jasti](https:/
-00001300: 2f67 6974 6875 622e 636f 6d2f 7761 7465  /github.com/wate
-00001310: 6665 656e 6578 290d 0a2d 205b 4a61 6d65  feenex)..- [Jame
-00001320: 7320 4c61 6d62 6572 746f 6e5d 2868 7474  s Lamberton](htt
-00001330: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-00001340: 4a61 6d65 734c 616d 6265 7274 6f6e 290d  JamesLamberton).
-00001350: 0a2d 205b 4a6f 6572 6720 5769 636b 6572  .- [Joerg Wicker
-00001360: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
-00001370: 2e63 6f6d 2f6a 6f65 7267 7769 636b 6572  .com/joergwicker
-00001380: 290d 0a2d 205b 5869 6e67 6c6f 6e67 2028  )..- [Xinglong (
-00001390: 4c75 6b65 2920 4368 616e 675d 2868 7474  Luke) Chang](htt
-000013a0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-000013b0: 6368 616e 6778 3033 290d 0a0d 0a23 2320  changx03)....## 
-000013c0: 4c69 6365 6e73 650d 0a0d 0a4d 656d 656e  License....Memen
-000013d0: 746f 2069 7320 6c69 6365 6e73 6564 2075  to is licensed u
-000013e0: 6e64 6572 2074 6865 205b 332d 436c 6175  nder the [3-Clau
-000013f0: 7365 2042 5344 204c 6963 656e 7365 5d28  se BSD License](
-00001400: 6874 7470 733a 2f2f 6f70 656e 736f 7572  https://opensour
-00001410: 6365 2e6f 7267 2f6c 6963 656e 7365 732f  ce.org/licenses/
-00001420: 4253 442d 332d 436c 6175 7365 2920 6c69  BSD-3-Clause) li
-00001430: 6365 6e73 652e 0d0a                      cense...
+000000a0: 0d0a 0d0a 2320 4d45 4d45 4e54 4f0d 0a0d  ....# MEMENTO...
+000000b0: 0a60 4d45 4d45 4e54 4f60 2069 7320 6120  .`MEMENTO` is a 
+000000c0: 5079 7468 6f6e 206c 6962 7261 7279 2066  Python library f
+000000d0: 6f72 2072 756e 6e69 6e67 2063 6f6d 7075  or running compu
+000000e0: 7461 7469 6f6e 616c 6c79 2065 7870 656e  tationally expen
+000000f0: 7369 7665 2065 7870 6572 696d 656e 7473  sive experiments
+00000100: 2e0d 0a0d 0a52 756e 6e69 6e67 2063 6f6d  .....Running com
+00000110: 706c 6578 2073 6574 7320 6f66 206d 6163  plex sets of mac
+00000120: 6869 6e65 206c 6561 726e 696e 6720 6578  hine learning ex
+00000130: 7065 7269 6d65 6e74 7320 6973 2063 6861  periments is cha
+00000140: 6c6c 656e 6769 6e67 2061 6e64 2074 696d  llenging and tim
+00000150: 652d 636f 6e73 756d 696e 6720 6475 6520  e-consuming due 
+00000160: 746f 2074 6865 206c 6163 6b20 6f66 2061  to the lack of a
+00000170: 2075 6e69 6669 6564 2066 7261 6d65 776f   unified framewo
+00000180: 726b 2e0d 0a54 6869 7320 6c65 6176 6573  rk...This leaves
+00000190: 2072 6573 6561 7263 6865 7273 2066 6f72   researchers for
+000001a0: 6365 6420 746f 2073 7065 6e64 2074 696d  ced to spend tim
+000001b0: 6520 696d 706c 656d 656e 7469 6e67 206e  e implementing n
+000001c0: 6563 6573 7361 7279 2066 6561 7475 7265  ecessary feature
+000001d0: 7320 7375 6368 2061 7320 7061 7261 6c6c  s such as parall
+000001e0: 656c 697a 6174 696f 6e2c 2063 6163 6869  elization, cachi
+000001f0: 6e67 2c20 616e 6420 6368 6563 6b70 6f69  ng, and checkpoi
+00000200: 6e74 696e 6720 7468 656d 7365 6c76 6573  nting themselves
+00000210: 2069 6e73 7465 6164 206f 6620 666f 6375   instead of focu
+00000220: 7373 696e 6720 6f6e 2074 6865 6972 2070  ssing on their p
+00000230: 726f 6a65 6374 2e0d 0a54 6f20 7369 6d70  roject...To simp
+00000240: 6c69 6679 2074 6865 2070 726f 6365 7373  lify the process
+00000250: 2c20 7765 2069 6e74 726f 6475 6365 2060  , we introduce `
+00000260: 4d45 4d45 4e54 4f60 2c20 6120 5079 7468  MEMENTO`, a Pyth
+00000270: 6f6e 2070 6163 6b61 6765 2074 6861 7420  on package that 
+00000280: 6973 2064 6573 6967 6e65 6420 746f 2061  is designed to a
+00000290: 6964 2072 6573 6561 7263 6865 7273 2061  id researchers a
+000002a0: 6e64 2064 6174 6120 7363 6965 6e74 6973  nd data scientis
+000002b0: 7473 2069 6e20 7468 6520 6566 6669 6369  ts in the effici
+000002c0: 656e 7420 6d61 6e61 6765 6d65 6e74 2061  ent management a
+000002d0: 6e64 2065 7865 6375 7469 6f6e 206f 6620  nd execution of 
+000002e0: 636f 6d70 7574 6174 696f 6e61 6c6c 7920  computationally 
+000002f0: 696e 7465 6e73 6976 6520 6578 7065 7269  intensive experi
+00000300: 6d65 6e74 732e 0d0a 604d 454d 454e 544f  ments...`MEMENTO
+00000310: 6020 6861 7320 7468 6520 6361 7061 6369  ` has the capaci
+00000320: 7479 2074 6f20 7374 7265 616d 6c69 6e65  ty to streamline
+00000330: 2061 6e79 2065 7870 6572 696d 656e 7461   any experimenta
+00000340: 6c20 7069 7065 6c69 6e65 2062 7920 7072  l pipeline by pr
+00000350: 6f76 6964 696e 6720 6120 7374 7261 6967  oviding a straig
+00000360: 6874 666f 7277 6172 6420 636f 6e66 6967  htforward config
+00000370: 7572 6174 696f 6e20 6d61 7472 6978 2061  uration matrix a
+00000380: 6e64 2074 6865 2061 6269 6c69 7479 2074  nd the ability t
+00000390: 6f20 636f 6e63 7572 7265 6e74 6c79 2072  o concurrently r
+000003a0: 756e 2065 7870 6572 696d 656e 7473 2061  un experiments a
+000003b0: 6372 6f73 7320 6d75 6c74 6970 6c65 2074  cross multiple t
+000003c0: 6872 6561 6473 2e0d 0a0d 0a49 6620 796f  hreads.....If yo
+000003d0: 7520 6e65 6564 2074 6f20 7275 6e20 6120  u need to run a 
+000003e0: 6c61 7267 6520 6e75 6d62 6572 206f 6620  large number of 
+000003f0: 7469 6d65 2d63 6f6e 7375 6d69 6e67 2065  time-consuming e
+00000400: 7870 6572 696d 656e 7473 2060 4d45 4d45  xperiments `MEME
+00000410: 4e54 4f60 2063 616e 2068 656c 703a 0d0a  NTO` can help:..
+00000420: 0d0a 2d20 5374 7275 6374 7572 6520 796f  ..- Structure yo
+00000430: 7572 2063 6f6e 6669 6775 7261 7469 6f6e  ur configuration
+00000440: 0d0a 2d20 5061 7261 6c6c 656c 697a 6520  ..- Parallelize 
+00000450: 6578 7065 7269 6d65 6e74 7320 6163 726f  experiments acro
+00000460: 7373 2043 5055 730d 0a2d 2053 6176 6520  ss CPUs..- Save 
+00000470: 616e 6420 7265 7374 6f72 6520 7265 7375  and restore resu
+00000480: 6c74 730d 0a2d 2043 6865 636b 706f 696e  lts..- Checkpoin
+00000490: 7420 696e 2d70 726f 6772 6573 7320 6578  t in-progress ex
+000004a0: 7065 7269 6d65 6e74 730d 0a2d 2053 656e  periments..- Sen
+000004b0: 6420 6e6f 7469 6669 6361 7469 6f6e 7320  d notifications 
+000004c0: 7768 656e 2065 7870 6572 696d 656e 7473  when experiments
+000004d0: 2066 6169 6c20 6f72 2066 696e 6973 680d   fail or finish.
+000004e0: 0a0d 0a5b 215b 4465 6d6f 2076 6964 656f  ...[![Demo video
+000004f0: 5d28 6874 7470 733a 2f2f 696d 672e 796f  ](https://img.yo
+00000500: 7574 7562 652e 636f 6d2f 7669 2f47 4574  utube.com/vi/GEt
+00000510: 6443 6c31 5a55 5763 2f30 2e6a 7067 295d  dCl1ZUWc/0.jpg)]
+00000520: 2868 7474 703a 2f2f 7777 772e 796f 7574  (http://www.yout
+00000530: 7562 652e 636f 6d2f 7761 7463 683f 763d  ube.com/watch?v=
+00000540: 4745 7464 436c 315a 5557 6329 0d0a 0d0a  GEtdCl1ZUWc)....
+00000550: 2323 2047 6574 7469 6e67 2053 7461 7274  ## Getting Start
+00000560: 6564 0d0a 0d0a 604d 454d 454e 544f 6020  ed....`MEMENTO` 
+00000570: 6973 206f 6666 6963 6961 6c6c 7920 6176  is officially av
+00000580: 6169 6c61 626c 6520 6f6e 2050 7950 6c2e  ailable on PyPl.
+00000590: 2054 6f20 696e 7374 616c 6c20 7468 6520   To install the 
+000005a0: 7061 636b 6167 653a 0d0a 0d0a 2323 2320  package:....### 
+000005b0: 496e 7374 616c 6c0d 0a0d 0a60 6060 6261  Install....```ba
+000005c0: 7368 0d0a 7069 7020 696e 7374 616c 6c20  sh..pip install 
+000005d0: 6d65 6d65 6e74 6f2d 6d6c 0d0a 6060 600d  memento-ml..```.
+000005e0: 0a0d 0a23 2323 2054 6865 2043 6f6e 6669  ...### The Confi
+000005f0: 6775 7261 7469 6f6e 204d 6174 7269 780d  guration Matrix.
+00000600: 0a0d 0a54 6865 2063 6f72 6520 6f66 2060  ...The core of `
+00000610: 4d45 4d45 4e54 4f60 2069 7320 6120 636f  MEMENTO` is a co
+00000620: 6e66 6967 7572 6174 696f 6e20 606d 6174  nfiguration `mat
+00000630: 7269 7860 2074 6861 7420 6465 7363 7269  rix` that descri
+00000640: 6265 7320 7468 6520 6c69 7374 206f 6620  bes the list of 
+00000650: 6578 7065 7269 6d65 6e74 7320 796f 750d  experiments you.
+00000660: 0a77 616e 7420 604d 454d 454e 544f 6020  .want `MEMENTO` 
+00000670: 746f 2072 756e 2e20 5468 6973 206d 7573  to run. This mus
+00000680: 7420 636f 6e74 6169 6e20 6120 6b65 7920  t contain a key 
+00000690: 6070 6172 616d 6574 6572 7360 2077 6869  `parameters` whi
+000006a0: 6368 2069 7320 6974 7365 6c66 2061 2064  ch is itself a d
+000006b0: 6963 742c 2074 6869 7320 6465 7363 7269  ict, this descri
+000006c0: 6265 730d 0a65 6163 6820 7061 7261 6d74  bes..each paramt
+000006d0: 6572 2079 6f75 2077 616e 7420 746f 2076  er you want to v
+000006e0: 6172 7920 666f 7220 796f 7572 2065 7870  ary for your exp
+000006f0: 6572 696d 656e 7473 2061 6e64 2074 6865  eriments and the
+00000700: 6972 2076 616c 7565 732e 0d0a 0d0a 4173  ir values.....As
+00000710: 2061 6e20 6578 616d 706c 6520 6c65 7427   an example let'
+00000720: 7320 7361 7920 796f 7520 7761 6e74 6564  s say you wanted
+00000730: 2074 6f20 7465 7374 2061 2066 6577 2073   to test a few s
+00000740: 696d 706c 6520 6c69 6e65 6172 2063 6c61  imple linear cla
+00000750: 7373 6966 6965 7273 206f 6e20 6120 6e75  ssifiers on a nu
+00000760: 6d62 6572 206f 660d 0a69 6d61 6765 2072  mber of..image r
+00000770: 6563 6f67 6e69 7469 6f6e 2064 6174 6173  ecognition datas
+00000780: 6574 732e 2059 6f75 206d 6967 6874 2077  ets. You might w
+00000790: 7269 7465 2073 6f6d 6574 6869 6e67 206c  rite something l
+000007a0: 696b 6520 7468 6973 3a0d 0a0d 0a3e 2044  ike this:....> D
+000007b0: 6f6e 2774 2077 6f72 7279 2069 6620 796f  on't worry if yo
+000007c0: 7527 7265 206e 6f74 2077 6f72 6b69 6e67  u're not working
+000007d0: 206f 6e20 6d61 6368 696e 6520 6c65 6172   on machine lear
+000007e0: 6e69 6e67 2c20 7468 6973 2069 7320 6a75  ning, this is ju
+000007f0: 7374 2061 6e20 6578 616d 706c 652e 0d0a  st an example...
+00000800: 0d0a 6060 6070 7974 686f 6e0d 0a6d 6174  ..```python..mat
+00000810: 7269 7820 3d20 7b0d 0a20 2022 7061 7261  rix = {..  "para
+00000820: 6d65 7465 7273 223a 207b 0d0a 2020 2020  meters": {..    
+00000830: 226d 6f64 656c 223a 205b 0d0a 2020 2020  "model": [..    
+00000840: 2020 736b 6c65 6172 6e2e 7376 6d2e 5356    sklearn.svm.SV
+00000850: 432c 0d0a 2020 2020 2020 736b 6c65 6172  C,..      sklear
+00000860: 6e2e 6c69 6e65 6172 5f6d 6f64 656c 2e50  n.linear_model.P
+00000870: 6572 6365 7074 726f 6e2c 0d0a 2020 2020  erceptron,..    
+00000880: 2020 736b 6c65 6172 6e2e 6c69 6e65 6172    sklearn.linear
+00000890: 5f6d 6f64 656c 2e4c 6f67 6973 7469 6352  _model.LogisticR
+000008a0: 6567 7265 7373 696f 6e0d 0a20 2020 205d  egression..    ]
+000008b0: 2c0d 0a20 2020 2022 6461 7461 7365 7422  ,..    "dataset"
+000008c0: 3a20 5b22 696d 6167 656e 6574 222c 2022  : ["imagenet", "
+000008d0: 6d6e 6973 7422 2c20 2263 6966 6172 3130  mnist", "cifar10
+000008e0: 222c 2022 7175 6963 6b64 7261 7722 5d0d  ", "quickdraw"].
+000008f0: 0a20 207d 0d0a 7d0d 0a60 6060 0d0a 0d0a  .  }..}..```....
+00000900: 604d 454d 454e 544f 6020 776f 756c 6420  `MEMENTO` would 
+00000910: 7468 656e 2067 656e 6572 6174 6520 3132  then generate 12
+00000920: 2063 6f6e 6669 6775 7261 7469 6f6e 7320   configurations 
+00000930: 6279 2074 616b 696e 6720 7468 6520 5f63  by taking the _c
+00000940: 6172 7465 7369 616e 2070 726f 6475 6374  artesian product
+00000950: 5f20 6f66 2074 6865 0d0a 7061 7261 6d65  _ of the..parame
+00000960: 7465 7273 2e0d 0a0d 0a46 7265 7175 656e  ters.....Frequen
+00000970: 746c 7920 796f 7520 6d69 6768 7420 616c  tly you might al
+00000980: 736f 2077 616e 7420 746f 2073 6574 2073  so want to set s
+00000990: 6f6d 6520 676c 6f62 616c 2063 6f6e 6669  ome global confi
+000009a0: 6775 7261 7469 6f6e 2076 616c 7565 732c  guration values,
+000009b0: 2073 7563 6820 6173 2061 2072 6567 756c   such as a regul
+000009c0: 6172 697a 6174 696f 6e0d 0a70 6172 616d  arization..param
+000009d0: 6574 6572 206f 7220 706f 7465 6e74 6961  eter or potentia
+000009e0: 6c6c 7920 6576 656e 2063 6861 6e67 6520  lly even change 
+000009f0: 796f 7572 2070 7265 7072 6f63 6573 7369  your preprocessi
+00000a00: 6e67 2070 6970 656c 696e 652e 2049 6e20  ng pipeline. In 
+00000a10: 7468 6973 2063 6173 6520 604d 454d 454e  this case `MEMEN
+00000a20: 544f 6020 616c 736f 0d0a 6163 6365 7074  TO` also..accept
+00000a30: 7320 6120 2273 6574 7469 6e67 7322 206b  s a "settings" k
+00000a40: 6579 2e20 5468 6573 6520 7365 7474 696e  ey. These settin
+00000a50: 6773 2061 7070 6c79 2074 6f20 616c 6c20  gs apply to all 
+00000a60: 6578 7065 7269 6d65 6e74 7320 616e 6420  experiments and 
+00000a70: 6361 6e20 6265 2061 6363 6573 7365 6420  can be accessed 
+00000a80: 6672 6f6d 2074 6865 0d0a 636f 6e66 6967  from the..config
+00000a90: 7572 6174 696f 6e20 6c69 7374 2061 7320  uration list as 
+00000aa0: 7765 6c6c 2061 7320 696e 6469 7669 6475  well as individu
+00000ab0: 616c 2063 6f6e 6669 6775 7261 7469 6f6e  al configuration
+00000ac0: 732e 0d0a 0d0a 6060 6070 7974 686f 6e0d  s.....```python.
+00000ad0: 0a6d 6174 7269 7820 3d20 7b0d 0a20 2022  .matrix = {..  "
+00000ae0: 7061 7261 6d65 7465 7273 223a 202e 2e2e  parameters": ...
+00000af0: 2c0d 0a20 2022 7365 7474 696e 6773 223a  ,..  "settings":
+00000b00: 207b 0d0a 2020 2020 2272 6567 756c 6172   {..    "regular
+00000b10: 697a 6174 696f 6e22 3a20 3165 2d31 2c0d  ization": 1e-1,.
+00000b20: 0a20 2020 2022 7072 6570 726f 6365 7373  .    "preprocess
+00000b30: 696e 6722 3a20 6d61 6b65 5f70 7265 7072  ing": make_prepr
+00000b40: 6f63 6573 7369 6e67 5f70 6970 656c 696e  ocessing_pipelin
+00000b50: 6528 290d 0a20 207d 0d0a 7d0d 0a60 6060  e()..  }..}..```
+00000b60: 0d0a 0d0a 596f 7520 6361 6e20 616c 736f  ....You can also
+00000b70: 2065 7863 6c75 6465 2073 7065 6369 6669   exclude specifi
+00000b80: 6320 7061 7261 6d65 7465 7220 636f 6e66  c parameter conf
+00000b90: 6967 7572 6174 696f 6e73 2e20 5265 7475  igurations. Retu
+00000ba0: 726e 696e 6720 746f 206f 7572 206d 6163  rning to our mac
+00000bb0: 6869 6e65 206c 6561 726e 696e 670d 0a65  hine learning..e
+00000bc0: 7861 6d70 6c65 2c20 6966 2079 6f75 206b  xample, if you k
+00000bd0: 6e6f 7720 5356 4373 2070 6572 666f 726d  now SVCs perform
+00000be0: 2070 6f6f 726c 7920 6f6e 2063 6966 6172   poorly on cifar
+00000bf0: 3130 2079 6f75 206d 6967 6874 2064 6563  10 you might dec
+00000c00: 6964 6520 746f 2073 6b69 7020 7468 6174  ide to skip that
+00000c10: 0d0a 6578 7065 7269 6d65 6e74 2065 6e74  ..experiment ent
+00000c20: 6972 656c 792e 2054 6869 7320 6973 2064  irely. This is d
+00000c30: 6f6e 6520 7769 7468 2074 6865 2022 6578  one with the "ex
+00000c40: 636c 7564 6522 206b 6579 3a0d 0a0d 0a60  clude" key:....`
+00000c50: 6060 7079 7468 6f6e 0d0a 6d61 7472 6978  ``python..matrix
+00000c60: 203d 207b 0d0a 2020 2270 6172 616d 6574   = {..  "paramet
+00000c70: 6572 7322 3a20 2e2e 2e2c 0d0a 2020 2265  ers": ...,..  "e
+00000c80: 7863 6c75 6465 223a 205b 0d0a 2020 2020  xclude": [..    
+00000c90: 7b22 6d6f 6465 6c22 3a20 736b 6c65 6172  {"model": sklear
+00000ca0: 6e2e 7376 6d2e 5356 432c 2022 6461 7461  n.svm.SVC, "data
+00000cb0: 7365 7422 3a20 2263 6966 6172 3130 227d  set": "cifar10"}
+00000cc0: 0d0a 2020 5d0d 0a7d 0d0a 6060 600d 0a0d  ..  ]..}..```...
+00000cd0: 0a23 2323 2052 756e 6e69 6e67 2061 6e20  .### Running an 
+00000ce0: 6578 7065 7269 6d65 6e74 0d0a 0d0a 416c  experiment....Al
+00000cf0: 6f6e 6720 7769 7468 2061 2063 6f6e 6669  ong with a confi
+00000d00: 6775 7261 7469 6f6e 206d 6174 7269 7820  guration matrix 
+00000d10: 796f 7520 6e65 6564 2073 6f6d 6520 636f  you need some co
+00000d20: 6465 2074 6f20 7275 6e20 796f 7572 2065  de to run your e
+00000d30: 7870 6572 696d 656e 7473 2e20 5468 6973  xperiments. This
+00000d40: 2063 616e 2062 6520 616e 790d 0a60 4361   can be any..`Ca
+00000d50: 6c6c 6162 6c65 6020 7375 6368 2061 7320  llable` such as 
+00000d60: 6120 6675 6e63 7469 6f6e 2c20 6c61 6d62  a function, lamb
+00000d70: 6461 2c20 636c 6173 732c 206f 7220 636c  da, class, or cl
+00000d80: 6173 7320 6d65 7468 6f64 2e0d 0a0d 0a60  ass method.....`
+00000d90: 6060 7079 7468 6f6e 0d0a 6672 6f6d 206d  ``python..from m
+00000da0: 656d 656e 746f 2069 6d70 6f72 7420 4d65  emento import Me
+00000db0: 6d65 6e74 6f2c 2043 6f6e 6669 672c 2043  mento, Config, C
+00000dc0: 6f6e 7465 7874 0d0a 0d0a 6465 6620 6578  ontext....def ex
+00000dd0: 7065 7269 6d65 6e74 2863 6f6e 7465 7874  periment(context
+00000de0: 3a20 436f 6e74 6578 742c 2063 6f6e 6669  : Context, confi
+00000df0: 673a 2043 6f6e 6669 6729 3a0d 0a20 2063  g: Config):..  c
+00000e00: 6c61 7373 6966 6965 7220 3d20 636f 6e66  lassifier = conf
+00000e10: 6967 2e6d 6f64 656c 2829 0d0a 2020 6461  ig.model()..  da
+00000e20: 7461 7365 7420 3d20 6665 7463 685f 6461  taset = fetch_da
+00000e30: 7461 7365 7428 636f 6e66 6967 2e64 6174  taset(config.dat
+00000e40: 6173 6574 290d 0a0d 0a20 2063 6c61 7373  aset)....  class
+00000e50: 6966 6965 722e 6669 7428 2a64 6174 6173  ifier.fit(*datas
+00000e60: 6574 290d 0a0d 0a20 2072 6574 7572 6e20  et)....  return 
+00000e70: 636c 6173 7369 6669 6572 0d0a 0d0a 4d65  classifier....Me
+00000e80: 6d65 6e74 6f28 6578 7065 7269 6d65 6e74  mento(experiment
+00000e90: 292e 7275 6e28 6d61 7472 6978 290d 0a60  ).run(matrix)..`
+00000ea0: 6060 0d0a 0d0a 596f 7520 6361 6e20 616c  ``....You can al
+00000eb0: 736f 2070 6572 666f 726d 2061 2064 7279  so perform a dry
+00000ec0: 2072 756e 2074 6f20 6368 6563 6b20 796f   run to check yo
+00000ed0: 7527 7665 2067 6f74 7465 6e20 7468 6520  u've gotten the 
+00000ee0: 6d61 7472 6978 2063 6f72 7265 6374 2e0d  matrix correct..
+00000ef0: 0a0d 0a60 6060 7079 7468 6f6e 0d0a 4d65  ...```python..Me
+00000f00: 6d65 6e74 6f28 6578 7065 7269 6d65 6e74  mento(experiment
+00000f10: 292e 7275 6e28 6d61 7472 6978 2c20 6472  ).run(matrix, dr
+00000f20: 795f 7275 6e3d 5472 7565 290d 0a60 6060  y_run=True)..```
+00000f30: 0d0a 0d0a 6060 6070 7974 686f 6e0d 0a52  ....```python..R
+00000f40: 756e 6e69 6e67 2063 6f6e 6669 6775 7261  unning configura
+00000f50: 7469 6f6e 733a 0d0a 2020 7b27 6d6f 6465  tions:..  {'mode
+00000f60: 6c27 3a20 736b 6c65 6172 6e2e 7376 6d2e  l': sklearn.svm.
+00000f70: 5356 432c 2027 6461 7461 7365 7427 3a20  SVC, 'dataset': 
+00000f80: 2769 6d61 6765 6e65 7427 7d0d 0a20 207b  'imagenet'}..  {
+00000f90: 276d 6f64 656c 273a 2073 6b6c 6561 726e  'model': sklearn
+00000fa0: 2e73 766d 2e53 5643 2c20 2764 6174 6173  .svm.SVC, 'datas
+00000fb0: 6574 273a 2027 6d6e 6973 7427 7d0d 0a20  et': 'mnist'}.. 
+00000fc0: 207b 276d 6f64 656c 273a 2073 6b6c 6561   {'model': sklea
+00000fd0: 726e 2e73 766d 2e53 5643 2c20 2764 6174  rn.svm.SVC, 'dat
+00000fe0: 6173 6574 273a 2027 6369 6661 7231 3027  aset': 'cifar10'
+00000ff0: 7d0d 0a20 207b 276d 6f64 656c 273a 2073  }..  {'model': s
+00001000: 6b6c 6561 726e 2e73 766d 2e53 5643 2c20  klearn.svm.SVC, 
+00001010: 2764 6174 6173 6574 273a 2027 7175 6963  'dataset': 'quic
+00001020: 6b64 7261 7727 7d0d 0a20 207b 276d 6f64  kdraw'}..  {'mod
+00001030: 656c 273a 2073 6b6c 6561 726e 2e6c 696e  el': sklearn.lin
+00001040: 6561 725f 6d6f 6465 6c2e 5065 7263 6570  ear_model.Percep
+00001050: 7472 6f6e 2c20 2764 6174 6173 6574 273a  tron, 'dataset':
+00001060: 2027 696d 6167 656e 6574 277d 0d0a 2020   'imagenet'}..  
+00001070: 2e2e 2e0d 0a45 7869 7469 6e67 2064 7565  .....Exiting due
+00001080: 2074 6f20 6472 7920 7275 6e0d 0a60 6060   to dry run..```
+00001090: 0d0a 0d0a 2323 2043 6f64 6520 6465 6d6f  ....## Code demo
+000010a0: 0d0a 0d0a 2d20 436f 6465 2064 656d 6f20  ....- Code demo 
+000010b0: 6361 6e20 6265 2066 6f75 6e64 205b 6865  can be found [he
+000010c0: 7265 5d28 6465 6d6f 292e 0d0a 2d20 604d  re](demo)...- `M
+000010d0: 454d 454e 544f 6020 646f 6573 206e 6f74  EMENTO` does not
+000010e0: 2064 6570 656e 6420 6f6e 2061 6e79 204d   depend on any M
+000010f0: 4c20 7061 636b 6167 6573 2c20 652e 672e  L packages, e.g.
+00001100: 2c20 6073 6369 6b69 742d 6c65 6172 6e60  , `scikit-learn`
+00001110: 2e20 5468 6520 6073 6369 6b69 742d 6c65  . The `scikit-le
+00001120: 6172 6e60 2061 6e64 2060 6a75 7079 7465  arn` and `jupyte
+00001130: 726c 6162 6020 7061 636b 6167 6573 2061  rlab` packages a
+00001140: 7265 2072 6571 7569 7265 6420 746f 2072  re required to r
+00001150: 756e 2074 6865 2064 656d 6f20 2860 2e2f  un the demo (`./
+00001160: 6465 6d6f 2f2a 6029 2e0d 0a0d 0a60 6060  demo/*`).....```
+00001170: 6261 7368 0d0a 7069 7020 696e 7374 616c  bash..pip instal
+00001180: 6c20 6d65 6d65 6e74 6f2d 6d6c 2073 6369  l memento-ml sci
+00001190: 6b69 742d 6c65 6172 6e20 6a75 7079 7465  kit-learn jupyte
+000011a0: 726c 6162 0d0a 6060 600d 0a0d 0a23 2320  rlab..```....## 
+000011b0: 526f 6164 6d61 700d 0a0d 0a2d 2046 696e  Roadmap....- Fin
+000011c0: 6973 6820 4850 4320 7375 7070 6f72 740d  ish HPC support.
+000011d0: 0a2d 2049 6d70 726f 7665 2072 6573 756c  .- Improve resul
+000011e0: 7420 7365 7269 616c 6973 6174 696f 6e0d  t serialisation.
+000011f0: 0a2d 2049 6d70 726f 7665 2063 7573 746f  .- Improve custo
+00001200: 6d69 7a61 7469 6f6e 2066 6f72 206e 6f74  mization for not
+00001210: 6966 6963 6174 696f 6e0d 0a0d 0a23 2320  ification....## 
+00001220: 436f 6e74 7269 6275 746f 7273 0d0a 0d0a  Contributors....
+00001230: 2d20 5b5a 6163 2050 756c 6c61 722d 5374  - [Zac Pullar-St
+00001240: 7265 636b 6572 5d28 6874 7470 733a 2f2f  recker](https://
+00001250: 6769 7468 7562 2e63 6f6d 2f7a 6163 7073  github.com/zacps
+00001260: 290d 0a2d 205b 4665 7261 7320 416c 6261  )..- [Feras Alba
+00001270: 726f 7564 695d 2868 7474 7073 3a2f 2f67  roudi](https://g
+00001280: 6974 6875 622e 636f 6d2f 4e65 6564 7353  ithub.com/NeedsS
+00001290: 6f79 5361 7563 6529 0d0a 2d20 5b4c 6961  oySauce)..- [Lia
+000012a0: 6d20 5363 6f74 742d 5275 7373 656c 6c5d  m Scott-Russell]
+000012b0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+000012c0: 636f 6d2f 4c69 616d 2d53 636f 7474 2d52  com/Liam-Scott-R
+000012d0: 7573 7365 6c6c 290d 0a2d 205b 4a6f 7368  ussell)..- [Josh
+000012e0: 7561 2064 6520 5765 745d 2868 7474 7073  ua de Wet](https
+000012f0: 3a2f 2f67 6974 6875 622e 636f 6d2f 4465  ://github.com/De
+00001300: 7765 7261 290d 0a2d 205b 4e69 7075 6e20  wera)..- [Nipun 
+00001310: 4a61 7374 695d 2868 7474 7073 3a2f 2f67  Jasti](https://g
+00001320: 6974 6875 622e 636f 6d2f 7761 7465 6665  ithub.com/watefe
+00001330: 656e 6578 290d 0a2d 205b 4a61 6d65 7320  enex)..- [James 
+00001340: 4c61 6d62 6572 746f 6e5d 2868 7474 7073  Lamberton](https
+00001350: 3a2f 2f67 6974 6875 622e 636f 6d2f 4a61  ://github.com/Ja
+00001360: 6d65 734c 616d 6265 7274 6f6e 290d 0a2d  mesLamberton)..-
+00001370: 205b 5869 6e67 6c6f 6e67 2028 4c75 6b65   [Xinglong (Luke
+00001380: 2920 4368 616e 675d 2868 7474 7073 3a2f  ) Chang](https:/
+00001390: 2f67 6974 6875 622e 636f 6d2f 6368 616e  /github.com/chan
+000013a0: 6778 3033 290d 0a2d 205b 4c69 616d 2042  gx03)..- [Liam B
+000013b0: 7279 646f 6e5d 2868 7474 7073 3a2f 2f67  rydon](https://g
+000013c0: 6974 6875 622e 636f 6d2f 4d79 4372 6561  ithub.com/MyCrea
+000013d0: 7469 7669 7479 4f75 746c 6574 290d 0a2d  tivityOutlet)..-
+000013e0: 205b 496f 616e 6e69 7320 5a69 6f67 6173   [Ioannis Ziogas
+000013f0: 5d28 697a 696f 3939 3540 6175 636b 6c61  ](izio995@auckla
+00001400: 6e64 756e 692e 6163 2e6e 7a29 0d0a 2d20  nduni.ac.nz)..- 
+00001410: 5b4b 6174 6861 7269 6e61 2044 6f73 745d  [Katharina Dost]
+00001420: 286b 6174 6861 7269 6e61 2e64 6f73 7440  (katharina.dost@
+00001430: 6175 636b 6c61 6e64 2e61 632e 6e7a 290d  auckland.ac.nz).
+00001440: 0a2d 205b 4a6f 6572 6720 5769 636b 6572  .- [Joerg Wicker
+00001450: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+00001460: 2e63 6f6d 2f6a 6f65 7267 7769 636b 6572  .com/joergwicker
+00001470: 290d 0a0d 0a23 2320 4c69 6365 6e73 650d  )....## License.
+00001480: 0a0d 0a4d 454d 454e 544f 2069 7320 6c69  ...MEMENTO is li
+00001490: 6365 6e73 6564 2075 6e64 6572 2074 6865  censed under the
+000014a0: 205b 332d 436c 6175 7365 2042 5344 204c   [3-Clause BSD L
+000014b0: 6963 656e 7365 5d28 6874 7470 733a 2f2f  icense](https://
+000014c0: 6f70 656e 736f 7572 6365 2e6f 7267 2f6c  opensource.org/l
+000014d0: 6963 656e 7365 732f 4253 442d 332d 436c  icenses/BSD-3-Cl
+000014e0: 6175 7365 2920 6c69 6365 6e73 652e 0d0a  ause) license...
```

### Comparing `memento-ml-1.0.2/memento/__init__.py` & `memento-ml-1.1.0/memento/__init__.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,63 +1,63 @@
-"""
-MEMENTO is a Python library for running computationally expensive experiments.
-"""
-
-from memento.configurations import Config, Configurations, generate_configurations
-from memento.memento import Memento
-from memento.task_interface import FileSystemCheckpointing, Context, MemoryUsage, Result
-from memento.notifications import (
-    NotificationProvider,
-    DefaultNotificationProvider,
-    ConsoleNotificationProvider,
-    FileSystemNotificationProvider,
-    EmailNotificationProvider,
-    SmtpConfiguration,
-)
-from memento.caching import (
-    CacheProvider,
-    MemoryCacheProvider,
-    FileSystemCacheProvider,
-    Cache,
-    default_key_provider,
-)
-from memento.parallel import (
-    TaskManager,
-    delayed,
-    TASK_PRIORITY_LOW,
-    TASK_PRIORITY_MEDIUM,
-    TASK_PRIORITY_HIGH,
-)
-from memento.exceptions import AggregateException, CacheMiss, CyclicDependency
-
-__all__ = [
-    "Memento",
-    "Config",
-    "Configurations",
-    "generate_configurations",
-    "FileSystemCheckpointing",
-    "Context",
-    "MemoryUsage",
-    "Result",
-    "default_key_provider",
-    "NotificationProvider",
-    "DefaultNotificationProvider",
-    "ConsoleNotificationProvider",
-    "FileSystemNotificationProvider",
-    "EmailNotificationProvider",
-    "SmtpConfiguration",
-    "CacheProvider",
-    "MemoryCacheProvider",
-    "FileSystemCacheProvider",
-    "Cache",
-    "default_key_provider",
-    "TaskManager",
-    "delayed",
-    "TASK_PRIORITY_LOW",
-    "TASK_PRIORITY_MEDIUM",
-    "TASK_PRIORITY_HIGH",
-    "AggregateException",
-    "CacheMiss",
-    "CyclicDependency",
-]
-
-__version__ = "1.0.2"
+"""
+MEMENTO is a Python library for running computationally expensive experiments.
+"""
+
+from memento.configurations import Config, Configurations, generate_configurations
+from memento.memento import Memento
+from memento.task_interface import FileSystemCheckpointing, Context, MemoryUsage, Result
+from memento.notifications import (
+    NotificationProvider,
+    DefaultNotificationProvider,
+    ConsoleNotificationProvider,
+    FileSystemNotificationProvider,
+    EmailNotificationProvider,
+    SmtpConfiguration,
+)
+from memento.caching import (
+    CacheProvider,
+    MemoryCacheProvider,
+    FileSystemCacheProvider,
+    Cache,
+    default_key_provider,
+)
+from memento.parallel import (
+    TaskManager,
+    delayed,
+    TASK_PRIORITY_LOW,
+    TASK_PRIORITY_MEDIUM,
+    TASK_PRIORITY_HIGH,
+)
+from memento.exceptions import AggregateException, CacheMiss, CyclicDependency
+
+__all__ = [
+    "Memento",
+    "Config",
+    "Configurations",
+    "generate_configurations",
+    "FileSystemCheckpointing",
+    "Context",
+    "MemoryUsage",
+    "Result",
+    "default_key_provider",
+    "NotificationProvider",
+    "DefaultNotificationProvider",
+    "ConsoleNotificationProvider",
+    "FileSystemNotificationProvider",
+    "EmailNotificationProvider",
+    "SmtpConfiguration",
+    "CacheProvider",
+    "MemoryCacheProvider",
+    "FileSystemCacheProvider",
+    "Cache",
+    "default_key_provider",
+    "TaskManager",
+    "delayed",
+    "TASK_PRIORITY_LOW",
+    "TASK_PRIORITY_MEDIUM",
+    "TASK_PRIORITY_HIGH",
+    "AggregateException",
+    "CacheMiss",
+    "CyclicDependency",
+]
+
+__version__ = "1.0.2"
```

### Comparing `memento-ml-1.0.2/memento/caching.py` & `memento-ml-1.1.0/memento/caching.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,289 +1,303 @@
-"""
-Contains classes for implementing caching of functions.
-"""
-import os
-import sqlite3
-import tempfile
-from abc import ABC, abstractmethod
-from typing import Callable
-import cloudpickle
-
-
-class CacheProvider(ABC):
-    """
-    Abstract base class for implementing a cache provider, allowing different forms of caching.
-
-    Provides the interface that all cache providers must adhere to.
-
-    Must be used as the parent class of a cache provider class.
-
-    ..
-        class CustomCacheProvider(CacheProvider):
-    """
-
-    def __getitem__(self, key: str):
-        return self.get(key)
-
-    def __setitem__(self, key: str, item):
-        return self.set(key, item)
-
-    def __contains__(self, key: str):
-        return self.contains(key)
-
-    @abstractmethod
-    def __str__(self) -> str:
-        """
-        Creates a human-readable string of the cache.
-
-        :return: A string representing the cache.
-        """
-
-    @abstractmethod
-    def get(self, key: str):
-        """
-        Gets the item in the cache specified by the key.
-
-        :param key: Used to get the item from the cache.
-        :returns: The item in the cache, if it exists.
-        :raise KeyError: When the key is not in the cache.
-        """
-
-    @abstractmethod
-    def set(self, key: str, item) -> None:
-        """
-        Puts the item in the cache, at the specified key.
-
-        :param key: The location for the item in the cache.
-        :param item: The item to be cached.
-        :returns: Nothing.
-        """
-
-    @abstractmethod
-    def contains(self, key: str) -> bool:
-        """
-        Checks whether a key is already in the cache.
-
-        :param key: The key to check.
-        :returns: True if it exists, False otherwise.
-        """
-
-    @abstractmethod
-    def make_key(self, func: Callable, *args, **kwargs) -> str:
-        """
-        Generates a key to be used in caching.
-
-        :param func: The function to be cached.
-        :param args: Arguments to the function to be cached.
-        :param kwargs: Keyword arguments to the function to be cached.
-        :returns: True if it exists, False otherwise.
-        """
-
-
-class MemoryCacheProvider(CacheProvider):
-    """
-    An in-memory cache provider. Uses a dictionary for underlying storage.
-    """
-
-    def __init__(self, initial_cache: dict = None, key_provider: Callable = None):
-        """
-        Creates a cache provider that uses memory for caching.
-
-        :param initial_cache: Optional initial cache, defaults to an empty dictionary.
-        """
-        self._cache = initial_cache or {}
-
-        self._key_provider = key_provider or default_key_provider
-
-    def __str__(self):
-        return str(self._cache)
-
-    def get(self, key: str):
-        return self._cache[key]
-
-    def set(self, key: str, item) -> None:
-        self._cache[key] = item
-
-    def contains(self, key: str) -> bool:
-        return self._cache.get(key, False) is not False
-
-    def make_key(self, func: Callable, *args, **kwargs) -> str:
-        return self._key_provider(func, *args, **kwargs)
-
-
-class FileSystemCacheProvider(CacheProvider):
-    """
-    A filesystem caching provider. Uses SQLITE3 to write to a database file on disk.
-    """
-
-    def __init__(
-        self,
-        connection: sqlite3.Connection = None,
-        filepath: str = None,
-        key_provider: Callable = None,
-        table_name: str = None,
-    ):
-        """
-        Creates a FileSystemCacheProvider, optionally using a DB connection or filepath.
-        :param connection: A sqlite3 DB connection to use. Supplying this breaks parallelization.
-        :param filepath: A filepath to use for the database file (relative or absolute).
-        """
-        self._connection = connection  # if none is handled elsewhere
-        # use a temporary file (in appropriate tmp dir) if no file provided
-        self._filepath = os.path.abspath(
-            filepath or tempfile.NamedTemporaryFile(suffix="_memento.cache").name
-        )
-        self._table_name = table_name or "cache"
-
-        self._sqlite_timestamp = "(julianday('now') - 2440587.5)*86400.0"
-        self._sql_select = f"SELECT value FROM {self._table_name} WHERE key = ?"
-        self._sql_insert = (
-            f"INSERT OR REPLACE INTO {self._table_name}(key,value) VALUES(?,?)"
-        )
-
-        self._key_provider = key_provider or default_key_provider
-
-        self._setup_database()
-
-    def _setup_database(self) -> None:
-        """
-        Sets up the database, creating a "cache" table, with a key, value, and timestamp column.
-        :return: Nothing.
-        """
-        with self as database:
-            database.execute(
-                f"""
-                CREATE TABLE IF NOT EXISTS {self._table_name} (
-                    key BINARY PRIMARY KEY,
-                    ts REAL NOT NULL DEFAULT ({self._sqlite_timestamp}),
-                    value BLOB NOT NULL
-                ) WITHOUT ROWID
-            """
-            )
-
-    def __enter__(self) -> sqlite3.Connection:
-        """
-        Used to connect to the underlying database safely, handling setup and teardown.
-
-        Runs at the beginning of a `with _ as _` block
-        ...
-            with file_system_caching_object as database:
-                database.execute("some SQL")
-
-        :return: A sqlite3 Connection object, representing a database connection.
-        """
-        return self._connection or sqlite3.Connection(
-            self._filepath, isolation_level="DEFERRED"
-        )
-
-    def __exit__(self, exc_type, exc_val, exc_tb) -> None:
-        """
-        Run at the end of the `with _ as _` block
-        ...
-            with file_system_caching_object as database:
-                database.execute("some SQL")
-
-        :return: Nothing.
-        """
-
-    def __str__(self) -> str:
-        return f"Filesystem cache, using {self._connection or self._filepath}"
-
-    def get(self, key: str):
-        with self as database:
-            rows = database.execute(self._sql_select, (key,)).fetchall()
-            if rows:
-                return cloudpickle.loads(rows[0][0])
-
-            raise KeyError(f"Key '{key}' not in cache")
-
-    def set(self, key: str, item) -> None:
-        with self as database:
-            database.execute(self._sql_insert, (key, cloudpickle.dumps(item)))
-            database.commit()
-
-    def contains(self, key: str) -> bool:
-        try:
-            self.get(key)
-            return True
-        except KeyError:
-            return False
-
-    def make_key(self, func: Callable, *args, **kwargs) -> str:
-        return self._key_provider(func, *args, **kwargs)
-
-
-class Cache:
-    """
-    A higher order function that caches another, underlying function.
-    """
-
-    def __init__(self, func: Callable, cache_provider: CacheProvider = None):
-        """
-        Create the Cache object.
-
-        Usage can be one of the following:
-
-        ..
-            @Cache
-            def underlying_function():
-                pass
-
-            cached_function = Cache(underlying_function)
-
-        :param func: The function to be cached.
-        :param cache_provider: The cache provider, defaults to FileSystemCacheProvider
-        """
-        self._func = func
-        if cache_provider is None:
-            cache_provider = FileSystemCacheProvider()
-        self._cache_provider = cache_provider
-
-    def __call__(
-        self, *args, force_cache: bool = False, force_run: bool = False, **kwargs
-    ):
-        """
-        Method called when the cached function is called.
-
-        ..
-            @Cache
-            def underlying_func():
-                pass
-            cached_func = Cache(underlying_func)
-
-            underlying_func()
-            cached_func()
-
-        :param args: Arguments to the underlying function.
-        :param force_cache: Attempt to retrieve cached results, raising
-        ``KeyError`` if they do not exist
-        :param force_run: Run the function, ignoring any cached values
-        :param kwargs: Keyword arguments to the underlying function.
-        :return: The (cached) result of the underlying function.
-        """
-        key = self._cache_provider.make_key(self._func, *args, **kwargs)
-
-        try:
-            if force_run:
-                raise KeyError("cache ignored due to force_run")
-            return self._cache_provider.get(key)
-        except KeyError as ex:
-            if force_cache:
-                raise ex
-            value = self._func(*args, **kwargs)  # execute the function, with arguments
-            self._cache_provider.set(key, value)
-            return value
-
-    def __str__(self):
-        """
-        Creates a human-readable string of the cache and cached function.
-
-        :return: A string representing the cached function.
-        """
-        return f"Cached function object: func: {self._func}, cache: {str(self._cache_provider)}"
-
-
-def default_key_provider(func: Callable, *args, **kwargs) -> str:
-    """
-    Default cache key function. This uses cloudpickle to hash the function and all arguments.
-    """
-    return cloudpickle.dumps({"function": func, "args": args, "kwargs": kwargs})
+"""
+Contains classes for implementing caching of functions.
+"""
+import os
+import sqlite3
+import hashlib
+import tempfile
+from abc import ABC, abstractmethod
+from typing import Callable
+import cloudpickle
+
+
+class CacheProvider(ABC):
+    """
+    Abstract base class for implementing a cache provider, allowing different forms of caching.
+
+    Provides the interface that all cache providers must adhere to.
+
+    Must be used as the parent class of a cache provider class.
+
+    ..
+        class CustomCacheProvider(CacheProvider):
+    """
+
+    def __getitem__(self, key: str):
+        return self.get(key)
+
+    def __setitem__(self, key: str, item):
+        return self.set(key, item)
+
+    def __contains__(self, key: str):
+        return self.contains(key)
+
+    @abstractmethod
+    def __str__(self) -> str:
+        """
+        Creates a human-readable string of the cache.
+
+        :return: A string representing the cache.
+        """
+
+    @abstractmethod
+    def get(self, key: str):
+        """
+        Gets the item in the cache specified by the key.
+
+        :param key: Used to get the item from the cache.
+        :returns: The item in the cache, if it exists.
+        :raise KeyError: When the key is not in the cache.
+        """
+
+    @abstractmethod
+    def set(self, key: str, item) -> None:
+        """
+        Puts the item in the cache, at the specified key.
+
+        :param key: The location for the item in the cache.
+        :param item: The item to be cached.
+        :returns: Nothing.
+        """
+
+    @abstractmethod
+    def contains(self, key: str) -> bool:
+        """
+        Checks whether a key is already in the cache.
+
+        :param key: The key to check.
+        :returns: True if it exists, False otherwise.
+        """
+
+    @abstractmethod
+    def make_key(self, func: Callable, *args, **kwargs) -> str:
+        """
+        Generates a key to be used in caching.
+
+        :param func: The function to be cached.
+        :param args: Arguments to the function to be cached.
+        :param kwargs: Keyword arguments to the function to be cached.
+        :returns: True if it exists, False otherwise.
+        """
+
+
+class MemoryCacheProvider(CacheProvider):
+    """
+    An in-memory cache provider. Uses a dictionary for underlying storage.
+    """
+
+    def __init__(self, initial_cache: dict = None, key_provider: Callable = None):
+        """
+        Creates a cache provider that uses memory for caching.
+
+        :param initial_cache: Optional initial cache, defaults to an empty dictionary.
+        """
+        self._cache = initial_cache or {}
+
+        self._key_provider = key_provider or default_key_provider
+
+    def __str__(self):
+        return str(self._cache)
+
+    def get(self, key: str):
+        return self._cache[key]
+
+    def set(self, key: str, item) -> None:
+        self._cache[key] = item
+
+    def contains(self, key: str) -> bool:
+        return self._cache.get(key, False) is not False
+
+    def make_key(self, func: Callable, *args, **kwargs) -> str:
+        return self._key_provider(func, *args, **kwargs)
+
+
+class FileSystemCacheProvider(CacheProvider):
+    """
+    A filesystem caching provider. Uses SQLITE3 to write to a database file on disk.
+    """
+
+    def __init__(
+        self,
+        connection: sqlite3.Connection = None,
+        filepath: str = None,
+        key_provider: Callable = None,
+        table_name: str = None,
+    ):
+        """
+        Creates a FileSystemCacheProvider, optionally using a DB connection or filepath.
+        :param connection: A sqlite3 DB connection to use. Supplying this breaks parallelization.
+        :param filepath: A filepath to use for the database file (relative or absolute).
+        """
+        self._connection = connection  # if none is handled elsewhere
+        # use a temporary file (in appropriate tmp dir) if no file provided
+        self._filepath = os.path.abspath(
+            filepath or tempfile.NamedTemporaryFile(suffix="_memento.cache").name
+        )
+        self._table_name = table_name or "cache"
+
+        self._sqlite_timestamp = "(julianday('now') - 2440587.5)*86400.0"
+        self._sql_select = f"SELECT value FROM {self._table_name} WHERE key = ?"
+        self._sql_insert = (
+            f"INSERT OR REPLACE INTO {self._table_name}(key,value) VALUES(?,?)"
+        )
+        self._cache_files_folder = "memento_cache"
+
+        self._key_provider = key_provider or default_key_provider
+
+        self._setup_database()
+
+    def _setup_database(self) -> None:
+        """
+        Sets up the database, creating a "cache" table, with a key, value, and timestamp column.
+        :return: Nothing.
+        """
+        try:
+            os.mkdir(self._cache_files_folder)
+        except FileExistsError:
+            pass
+        with self as database:
+            database.execute(
+                f"""
+                CREATE TABLE IF NOT EXISTS {self._table_name} (
+                    key BINARY PRIMARY KEY,
+                    ts REAL NOT NULL DEFAULT ({self._sqlite_timestamp}),
+                    value BLOB NOT NULL
+                ) WITHOUT ROWID
+            """
+            )
+
+    def __enter__(self) -> sqlite3.Connection:
+        """
+        Used to connect to the underlying database safely, handling setup and teardown.
+
+        Runs at the beginning of a `with _ as _` block
+        ...
+            with file_system_caching_object as database:
+                database.execute("some SQL")
+
+        :return: A sqlite3 Connection object, representing a database connection.
+        """
+        return self._connection or sqlite3.Connection(
+            self._filepath, isolation_level="DEFERRED", timeout=10
+        )
+
+    def __exit__(self, exc_type, exc_val, exc_tb) -> None:
+        """
+        Run at the end of the `with _ as _` block
+        ...
+            with file_system_caching_object as database:
+                database.execute("some SQL")
+
+        :return: Nothing.
+        """
+
+    def __str__(self) -> str:
+        return f"Filesystem cache, using {self._connection or self._filepath}"
+
+    def get(self, key: str):
+        with self as database:
+            rows = database.execute(self._sql_select, (key,)).fetchall()
+            if rows:
+                with open(rows[0][0], "rb") as pkl_file:
+                    data = cloudpickle.load(pkl_file)
+                return data
+
+            raise KeyError(f"Key '{key}' not in cache")
+
+    def set(self, key: str, item) -> None:
+        bytes_key = str(key)
+        file_name = hashlib.sha256(bytes(bytes_key, "utf-8")).hexdigest()
+
+        path = f"{self._cache_files_folder}/{file_name}.pkl"
+        with open(path, "wb") as pkl_file:
+            cloudpickle.dump(item, pkl_file)
+        with self as database:
+            database.execute(self._sql_insert, (key, path))
+            database.commit()
+
+    def contains(self, key: str) -> bool:
+        try:
+            self.get(key)
+            return True
+        except KeyError:
+            return False
+
+    def make_key(self, func: Callable, *args, **kwargs) -> str:
+        return self._key_provider(func, *args, **kwargs)
+
+
+class Cache:
+    """
+    A higher order function that caches another, underlying function.
+    """
+
+    def __init__(self, func: Callable, cache_provider: CacheProvider = None):
+        """
+        Create the Cache object.
+
+        Usage can be one of the following:
+
+        ..
+            @Cache
+            def underlying_function():
+                pass
+
+            cached_function = Cache(underlying_function)
+
+        :param func: The function to be cached.
+        :param cache_provider: The cache provider, defaults to FileSystemCacheProvider
+        """
+        self._func = func
+        if cache_provider is None:
+            cache_provider = FileSystemCacheProvider()
+        self._cache_provider = cache_provider
+
+    def __call__(
+        self, *args, force_cache: bool = False, force_run: bool = False, **kwargs
+    ):
+        """
+        Method called when the cached function is called.
+
+        ..
+            @Cache
+            def underlying_func():
+                pass
+            cached_func = Cache(underlying_func)
+
+            underlying_func()
+            cached_func()
+
+        :param args: Arguments to the underlying function.
+        :param force_cache: Attempt to retrieve cached results, raising
+        ``KeyError`` if they do not exist
+        :param force_run: Run the function, ignoring any cached values
+        :param kwargs: Keyword arguments to the underlying function.
+        :return: The (cached) result of the underlying function.
+        """
+        key = self._cache_provider.make_key(self._func, *args, **kwargs)
+
+        try:
+            if force_run:
+                raise KeyError("cache ignored due to force_run")
+            return self._cache_provider.get(key)
+        except KeyError as ex:
+            if force_cache:
+                raise ex
+            value = self._func(*args, **kwargs)  # execute the function, with arguments
+            self._cache_provider.set(key, value)
+            return value
+
+    def __str__(self):
+        """
+        Creates a human-readable string of the cache and cached function.
+
+        :return: A string representing the cached function.
+        """
+        return f"Cached function object: func: {self._func}, cache: {str(self._cache_provider)}"
+
+
+def default_key_provider(func: Callable, *args, **kwargs) -> str:
+    """
+    Default cache key function. This uses cloudpickle to hash the function and all arguments.
+    """
+    return cloudpickle.dumps({"function": func, "args": args, "kwargs": kwargs})
```

### Comparing `memento-ml-1.0.2/memento/exceptions.py` & `memento-ml-1.1.0/memento/exceptions.py`

 * *Files identical despite different names*

### Comparing `memento-ml-1.0.2/memento/memento.py` & `memento-ml-1.1.0/memento/memento.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,246 +1,246 @@
-"""
-Contains `Memento`, the main entry point of MEMENTO.
-"""
-
-import functools
-import logging
-import os
-from datetime import datetime
-from typing import Callable, List, Optional, Dict, Any, cast
-from networkx import DiGraph, is_directed_acyclic_graph, topological_sort  # type: ignore
-
-import cloudpickle
-
-from memento.notifications import NotificationProvider, DefaultNotificationProvider
-from memento.parallel import TaskManager, delayed
-from memento.caching import FileSystemCacheProvider, CacheProvider
-from memento.configurations import generate_configurations, Config
-from memento.task_interface import Context, Result, FileSystemCheckpointing
-from memento.exceptions import CacheMiss, CyclicDependency
-
-logger = logging.getLogger(__name__)
-
-
-class Memento:
-    """
-    The main class of MEMENTO. This is the 'front end' of MEMENTO with which you can run a
-    configuration matrix and retrieve results from your experiments.
-    """
-
-    def __init__(
-        self, func: Callable, notification_provider: NotificationProvider = None
-    ):
-        """
-        :param func: Your experiment code. This will be called with an experiment configuration.
-        :param notification_provider: Notification provider to use. If not specified, no
-            notifications will be emitted.
-        """
-        self.func = func
-        self._notification_provider = (
-            notification_provider or DefaultNotificationProvider()
-        )
-        self._matrices: List[dict] = []
-
-    def add_matrix(self, matrix: dict):
-        """
-        Adds a configuration matrix.
-
-        :param matrix: A configuration matrix
-        """
-        self._matrices.append(matrix)
-
-    def _get_execution_order(self):
-        # Construct graph representation of matrices
-
-        graph_edges = []
-
-        for matrix in self._matrices:
-            for dependency in matrix["dependencies"]:
-                graph_edges.append(tuple([matrix["id"], dependency]))
-
-        graph = DiGraph()
-        graph.add_edges_from(graph_edges)
-        graph.add_nodes_from(matrix["id"] for matrix in self._matrices)
-
-        # Validate graph
-
-        if not is_directed_acyclic_graph(graph):
-            raise CyclicDependency()
-
-        # Get execution order via a topological sort
-        id_matrix_map = {matrix["id"]: matrix for matrix in self._matrices}
-        matrices = [id_matrix_map[id_] for id_ in list(topological_sort(graph))[::-1]]
-        return matrices
-
-    def run_all(self, **kwargs) -> Optional[Dict[Any, Optional[List[Result]]]]:
-        """
-        Runs this object's configuration matrices and returns their results.
-
-        :param kwargs: keyword arguments to Memento.run
-        """
-        matrices = self._get_execution_order()
-
-        n_matrices = len(matrices)
-
-        results: Dict[Any, Optional[List[Result]]] = {
-            matrix["id"]: None for matrix in matrices
-        }
-
-        # Run each matrix
-        for i in range(n_matrices):
-            matrix = matrices[i]
-
-            if kwargs.get("dry_run"):
-                configs = generate_configurations(matrix)
-
-                logger.info("Running configurations for matrix '%s':", matrix["id"])
-                for config in configs:
-                    logger.info("  %s", config)
-
-                if i == n_matrices - 1:
-                    logger.info("Exiting due to dry run")
-                    return None
-
-                inners = list(configs)
-            else:
-                results[matrix["id"]] = self.run(
-                    matrix, **kwargs, notify_on_complete=False
-                )
-
-                if i == n_matrices - 1:
-                    break
-
-                inners = [result.inner for result in cast(List, results[matrix["id"]])]
-
-            # Update all matrices that depend on the matrix that was just run
-            for mat in matrices[i + 1 :]:
-                if matrix["id"] in mat["dependencies"]:
-                    mat["parameters"][str(matrix["id"])] = inners
-
-        self._notification_provider.all_tasks_completed()
-
-        return results
-
-    def run(  # pylint: disable=too-many-arguments, too-many-locals
-        self,
-        matrix: dict,
-        dry_run: bool = False,
-        force_run: bool = False,
-        force_cache: bool = False,
-        cache_path: str = None,
-        notify_on_complete: bool = True,
-    ) -> Optional[List[Result]]:
-        """
-        Run a configuration matrix and return it's results.
-
-        :param matrix: A configuration matrix
-        :param dry_run: Do not actually run experiments, just log what would be run
-        :param force_run: Ignore the cache and re-run all experiments
-        :param force_cache: Raise ``exceptions.CacheMiss`` if an experiment is not found in the
-            cache
-        :param cache_path: Path to save results. This defaults to the current working directory and
-            can also be specified using ``MEMENTO_CACHE_PATH``.
-        :param notify_on_complete: If true, a notification will be triggered when all tasks have
-            been run.
-        :returns: A list of results from your experiments.
-        """
-
-        configs = generate_configurations(matrix)
-
-        logger.info("Running configurations:")
-        for config in configs:
-            logger.info("  %s", config)
-
-        if dry_run:
-            logger.info("Exiting due to dry run")
-            return None
-
-        cache_provider = FileSystemCacheProvider(
-            filepath=(
-                cache_path
-                or os.environ.get("MEMENTO_CACHE_PATH", None)
-                or "memento.sqlite"
-            ),
-            key_provider=_key_provider,
-        )
-
-        checkpoint_provider = FileSystemCheckpointing(
-            filepath=(cache_path or "memento.sqlite"),
-            key=_key_provider,
-        )
-        manager = TaskManager(
-            notification_provider=self._notification_provider,
-            notify_on_complete=notify_on_complete,
-        )
-
-        # Run tasks for which we have no cached result
-        ran = []
-        for config in configs:
-            key = _key_provider(self.func, config)
-            if not cache_provider.contains(key) or force_run:
-                if force_cache:
-                    raise CacheMiss(config)
-                context = Context(key, checkpoint_provider)
-                manager.add_task(
-                    delayed(_wrapper(self.func))(context, config, cache_provider)
-                )
-                ran.append(config)
-
-        manager.run()
-
-        results = [
-            cache_provider.get(_key_provider(self.func, config)) for config in configs
-        ]
-
-        for config in configs:
-            checkpoint_provider.remove(_key_provider(self.func, config))
-
-        for result in results:
-            if result.config in ran:
-                result.was_cached = False
-
-        logger.info(
-            "%s/%s results retrieved from cache",
-            len(configs) - len(ran),
-            len(configs),
-        )
-
-        return results
-
-
-def _wrapper(func: Callable) -> Callable:
-    """
-    Wrapper which runs in the task thread. This is responsible for collecting performance metrics
-    and writing to the cache.
-    """
-
-    @functools.wraps(func)
-    def inner(
-        context: Context, config: Config, cache_provider: CacheProvider
-    ) -> Result:
-        start_time = datetime.now()
-
-        inner = func(context, config)
-
-        runtime = datetime.now() - start_time
-
-        result = Result(
-            config,
-            inner,
-            metrics=context.collect_metrics(),
-            start_time=start_time,
-            runtime=runtime,
-            cpu_time=None,
-            memory=None,
-            was_cached=True,
-        )
-        cache_provider.set(context.key, result)
-        context.checkpoint(result)
-        return result
-
-    return inner
-
-
-def _key_provider(func: Callable, config: Config):
-    # The default behaviour caches on all arguments, including the config object.
-    return cloudpickle.dumps({"function": func, "args": [config]})
+"""
+Contains `Memento`, the main entry point of MEMENTO.
+"""
+
+import functools
+import logging
+import os
+from datetime import datetime
+from typing import Callable, List, Optional, Dict, Any, cast
+from networkx import DiGraph, is_directed_acyclic_graph, topological_sort  # type: ignore
+
+import cloudpickle
+
+from memento.notifications import NotificationProvider, DefaultNotificationProvider
+from memento.parallel import TaskManager, delayed
+from memento.caching import FileSystemCacheProvider, CacheProvider
+from memento.configurations import generate_configurations, Config
+from memento.task_interface import Context, Result, FileSystemCheckpointing
+from memento.exceptions import CacheMiss, CyclicDependency
+
+logger = logging.getLogger(__name__)
+
+
+class Memento:
+    """
+    The main class of MEMENTO. This is the 'front end' of MEMENTO with which you can run a
+    configuration matrix and retrieve results from your experiments.
+    """
+
+    def __init__(
+        self, func: Callable, notification_provider: NotificationProvider = None
+    ):
+        """
+        :param func: Your experiment code. This will be called with an experiment configuration.
+        :param notification_provider: Notification provider to use. If not specified, no
+            notifications will be emitted.
+        """
+        self.func = func
+        self._notification_provider = (
+            notification_provider or DefaultNotificationProvider()
+        )
+        self._matrices: List[dict] = []
+
+    def add_matrix(self, matrix: dict):
+        """
+        Adds a configuration matrix.
+
+        :param matrix: A configuration matrix
+        """
+        self._matrices.append(matrix)
+
+    def _get_execution_order(self):
+        # Construct graph representation of matrices
+
+        graph_edges = []
+
+        for matrix in self._matrices:
+            for dependency in matrix["dependencies"]:
+                graph_edges.append(tuple([matrix["id"], dependency]))
+
+        graph = DiGraph()
+        graph.add_edges_from(graph_edges)
+        graph.add_nodes_from(matrix["id"] for matrix in self._matrices)
+
+        # Validate graph
+
+        if not is_directed_acyclic_graph(graph):
+            raise CyclicDependency()
+
+        # Get execution order via a topological sort
+        id_matrix_map = {matrix["id"]: matrix for matrix in self._matrices}
+        matrices = [id_matrix_map[id_] for id_ in list(topological_sort(graph))[::-1]]
+        return matrices
+
+    def run_all(self, **kwargs) -> Optional[Dict[Any, Optional[List[Result]]]]:
+        """
+        Runs this object's configuration matrices and returns their results.
+
+        :param kwargs: keyword arguments to Memento.run
+        """
+        matrices = self._get_execution_order()
+
+        n_matrices = len(matrices)
+
+        results: Dict[Any, Optional[List[Result]]] = {
+            matrix["id"]: None for matrix in matrices
+        }
+
+        # Run each matrix
+        for i in range(n_matrices):
+            matrix = matrices[i]
+
+            if kwargs.get("dry_run"):
+                configs = generate_configurations(matrix)
+
+                logger.info("Running configurations for matrix '%s':", matrix["id"])
+                for config in configs:
+                    logger.info("  %s", config)
+
+                if i == n_matrices - 1:
+                    logger.info("Exiting due to dry run")
+                    return None
+
+                inners = list(configs)
+            else:
+                results[matrix["id"]] = self.run(
+                    matrix, **kwargs, notify_on_complete=False
+                )
+
+                if i == n_matrices - 1:
+                    break
+
+                inners = [result.inner for result in cast(List, results[matrix["id"]])]
+
+            # Update all matrices that depend on the matrix that was just run
+            for mat in matrices[i + 1 :]:
+                if matrix["id"] in mat["dependencies"]:
+                    mat["parameters"][str(matrix["id"])] = inners
+
+        self._notification_provider.all_tasks_completed()
+
+        return results
+
+    def run(  # pylint: disable=too-many-arguments, too-many-locals
+        self,
+        matrix: dict,
+        dry_run: bool = False,
+        force_run: bool = False,
+        force_cache: bool = False,
+        cache_path: str = None,
+        notify_on_complete: bool = True,
+    ) -> Optional[List[Result]]:
+        """
+        Run a configuration matrix and return it's results.
+
+        :param matrix: A configuration matrix
+        :param dry_run: Do not actually run experiments, just log what would be run
+        :param force_run: Ignore the cache and re-run all experiments
+        :param force_cache: Raise ``exceptions.CacheMiss`` if an experiment is not found in the
+            cache
+        :param cache_path: Path to save results. This defaults to the current working directory and
+            can also be specified using ``MEMENTO_CACHE_PATH``.
+        :param notify_on_complete: If true, a notification will be triggered when all tasks have
+            been run.
+        :returns: A list of results from your experiments.
+        """
+
+        configs = generate_configurations(matrix)
+
+        logger.info("Running configurations:")
+        for config in configs:
+            logger.info("  %s", config)
+
+        if dry_run:
+            logger.info("Exiting due to dry run")
+            return None
+
+        cache_provider = FileSystemCacheProvider(
+            filepath=(
+                cache_path
+                or os.environ.get("MEMENTO_CACHE_PATH", None)
+                or "memento.sqlite"
+            ),
+            key_provider=_key_provider,
+        )
+
+        checkpoint_provider = FileSystemCheckpointing(
+            filepath=(cache_path or "memento.sqlite"),
+            key=_key_provider,
+        )
+        manager = TaskManager(
+            notification_provider=self._notification_provider,
+            notify_on_complete=notify_on_complete,
+        )
+
+        # Run tasks for which we have no cached result
+        ran = []
+        for config in configs:
+            key = _key_provider(self.func, config)
+            if not cache_provider.contains(key) or force_run:
+                if force_cache:
+                    raise CacheMiss(config)
+                context = Context(key, checkpoint_provider)
+                manager.add_task(
+                    delayed(_wrapper(self.func))(context, config, cache_provider)
+                )
+                ran.append(config)
+
+        manager.run()
+
+        results = [
+            cache_provider.get(_key_provider(self.func, config)) for config in configs
+        ]
+
+        for config in configs:
+            checkpoint_provider.remove(_key_provider(self.func, config))
+
+        for result in results:
+            if result.config in ran:
+                result.was_cached = False
+
+        logger.info(
+            "%s/%s results retrieved from cache",
+            len(configs) - len(ran),
+            len(configs),
+        )
+
+        return results
+
+
+def _wrapper(func: Callable) -> Callable:
+    """
+    Wrapper which runs in the task thread. This is responsible for collecting performance metrics
+    and writing to the cache.
+    """
+
+    @functools.wraps(func)
+    def inner(
+        context: Context, config: Config, cache_provider: CacheProvider
+    ) -> Result:
+        start_time = datetime.now()
+
+        inner = func(context, config)
+
+        runtime = datetime.now() - start_time
+
+        result = Result(
+            config,
+            inner,
+            metrics=context.collect_metrics(),
+            start_time=start_time,
+            runtime=runtime,
+            cpu_time=None,
+            memory=None,
+            was_cached=True,
+        )
+        cache_provider.set(context.key, result)
+        context.checkpoint(result)
+        return result
+
+    return inner
+
+
+def _key_provider(func: Callable, config: Config):
+    # The default behaviour caches on all arguments, including the config object.
+    return cloudpickle.dumps({"function": func.__name__, "args": [config]})
```

### Comparing `memento-ml-1.0.2/memento/notifications.py` & `memento-ml-1.1.0/memento/notifications.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,219 +1,219 @@
-"""
-Contains classes for progress reporting.
-"""
-import email
-from email.utils import formataddr
-import smtplib
-from abc import ABC, abstractmethod
-from typing import Union, TextIO, Iterable, NamedTuple, Optional
-
-
-class NotificationProvider(ABC):
-    """
-    Abstract base class for implementing a notification provider, allowing notifications to be
-    raised to different locations. Generally, you should inherit from
-    :class:`DefaultNotificationProvider` to avoid having to implement every method.
-    """
-
-    @abstractmethod
-    def task_completed(self):
-        """
-        Executed when a task completes.
-        """
-
-    @abstractmethod
-    def all_tasks_completed(self):
-        """
-        Executed when all tasks complete.
-        """
-
-    @abstractmethod
-    def task_failure(self):
-        """
-        Executed when a task fails to execute.
-        """
-
-
-class DefaultNotificationProvider(NotificationProvider):
-    """
-    Default :class:`NotificationProvider` implementation that takes no actions when an event
-    occurs. This is the class you should extend if you want to create your own custom
-    notification provider.
-    """
-
-    def task_completed(self):
-        pass
-
-    def all_tasks_completed(self):
-        pass
-
-    def task_failure(self):
-        pass
-
-
-class ConsoleNotificationProvider(DefaultNotificationProvider):
-    """
-    Writes notification to the console (stdout).
-    """
-
-    def task_completed(self):
-        print("Task completed")
-
-    def all_tasks_completed(self):
-        print("All tasks completed")
-
-    def task_failure(self):
-        print("Task failed")
-
-
-class FileSystemNotificationProvider(DefaultNotificationProvider):
-    """
-    Writes notifications to a file.
-    """
-
-    def __init__(self, filepath: Union[TextIO, str] = None):
-        """
-        Creates a FileSystemNotificationProvider.
-
-        :param filepath: the filepath to write notifications to, opened in append mode,
-        or a file-like object. Defaults to 'logs.txt'.
-        """
-        self._filepath = filepath if isinstance(filepath, str) else "logs.txt"
-        self._file = filepath if not isinstance(filepath, str) else None
-
-    def _write(self, message: str):
-        str_ = f"{message}\n"
-        if self._file:
-            self._file.write(str_)
-        else:
-            with open(self._filepath, "a") as file:
-                file.write(str_)
-
-    def task_completed(self):
-        self._write("Task completed")
-
-    def all_tasks_completed(self):
-        self._write("All tasks completed")
-
-    def task_failure(self):
-        self._write("Task failed")
-
-
-class SmtpConfiguration(NamedTuple):
-    """SMTP server configuration options used by :class:`EmailNotificationProvider`."""
-
-    host: str
-    """ SMTP server host. """
-
-    port: int
-    """ SMTP server port. """
-
-    username: Optional[str] = None
-    """ Username to authenticate with. """
-
-    password: Optional[str] = None
-    """ Password to authenticate with. """
-
-    require_tls: Optional[bool] = True
-    """ Whether to require a TLS connection. Defaults to True. """
-
-
-class EmailNotificationProvider(DefaultNotificationProvider):
-    """
-    Sends notifications via email. Requires an SMTP server to connect to.
-
-    For example, to send notifications using a Gmail account::
-
-        smtp_config = SmtpConfiguration(
-            'smtp.gmail.com',
-            587,
-            username='sender@gmail.com',
-            password='password'
-        )
-
-        provider = EmailNotificationProvider(
-            smtp_config,
-            "sender@gmail.com",
-            ["recipient@gmail.com"]
-        )
-    """
-
-    def __init__(
-        self,
-        smtp: Union[SmtpConfiguration, smtplib.SMTP],
-        from_addr: str,
-        to_addrs: Iterable[str],
-    ):
-        """
-        Creates an EmailNotificationProvider.
-
-        :param smtp: SMTP configuration or a smtplib.SMTP object
-        :param from_addr: email address emails will be sent from
-        :param to_addrs: email addresses emails will be sent to
-        """
-        self._smpt_config = (
-            smtp
-            if isinstance(smtp, SmtpConfiguration)
-            else SmtpConfiguration("localhost", 0)
-        )
-        self._client = smtp if isinstance(smtp, smtplib.SMTP) else None
-        self._from_addr = from_addr
-        self._to_addrs = to_addrs
-
-    @property
-    def smpt(self):
-        """This provider's SmtpConfiguration."""
-        return self._smpt_config
-
-    @property
-    def from_addr(self):
-        """Email address emails will be sent from."""
-        return self._from_addr
-
-    @property
-    def to_addrs(self):
-        """Email addresses emails will be sent to."""
-        return self._to_addrs
-
-    def _send_email(self, message: email.message.Message):
-        if self._client:
-            self._client.send_message(message)
-        else:
-            with smtplib.SMTP(self._smpt_config.host, self._smpt_config.port) as smtp:
-                try:
-                    smtp.starttls()
-                except smtplib.SMTPNotSupportedError as error:
-                    if self._smpt_config.require_tls:
-                        raise error
-
-                if (
-                    self._smpt_config.username is not None
-                    and self._smpt_config.password is not None
-                ):
-                    smtp.login(self._smpt_config.username, self._smpt_config.password)
-                smtp.send_message(message)
-
-    def create_message(self, subject: str, content: str) -> email.message.Message:
-        """Creates an :class:`email.message.Message` with the given subject and content."""
-        message = email.message.EmailMessage()
-        message["From"] = formataddr(("Memento", self._from_addr))
-        message["To"] = ",".join(self._to_addrs)
-        message["Subject"] = subject
-        message.set_content(
-            content
-        )  # TODO: Maybe support HTML messages with a plain text fallback
-        return message
-
-    def task_completed(self):
-        message = self.create_message("[Memento] Task completed", "Task completed")
-        self._send_email(message)
-
-    def all_tasks_completed(self):
-        message = self.create_message(
-            "[Memento] All tasks completed", "All tasks completed"
-        )
-        self._send_email(message)
-
-    def task_failure(self):
-        message = self.create_message("[Memento] Task failed", "Task failed")
-        self._send_email(message)
+"""
+Contains classes for progress reporting.
+"""
+import email
+from email.utils import formataddr
+import smtplib
+from abc import ABC, abstractmethod
+from typing import Union, TextIO, Iterable, NamedTuple, Optional
+
+
+class NotificationProvider(ABC):
+    """
+    Abstract base class for implementing a notification provider, allowing notifications to be
+    raised to different locations. Generally, you should inherit from
+    :class:`DefaultNotificationProvider` to avoid having to implement every method.
+    """
+
+    @abstractmethod
+    def task_completed(self):
+        """
+        Executed when a task completes.
+        """
+
+    @abstractmethod
+    def all_tasks_completed(self):
+        """
+        Executed when all tasks complete.
+        """
+
+    @abstractmethod
+    def task_failure(self):
+        """
+        Executed when a task fails to execute.
+        """
+
+
+class DefaultNotificationProvider(NotificationProvider):
+    """
+    Default :class:`NotificationProvider` implementation that takes no actions when an event
+    occurs. This is the class you should extend if you want to create your own custom
+    notification provider.
+    """
+
+    def task_completed(self):
+        pass
+
+    def all_tasks_completed(self):
+        pass
+
+    def task_failure(self):
+        pass
+
+
+class ConsoleNotificationProvider(DefaultNotificationProvider):
+    """
+    Writes notification to the console (stdout).
+    """
+
+    def task_completed(self):
+        print("Task completed")
+
+    def all_tasks_completed(self):
+        print("All tasks completed")
+
+    def task_failure(self):
+        print("Task failed")
+
+
+class FileSystemNotificationProvider(DefaultNotificationProvider):
+    """
+    Writes notifications to a file.
+    """
+
+    def __init__(self, filepath: Union[TextIO, str] = None):
+        """
+        Creates a FileSystemNotificationProvider.
+
+        :param filepath: the filepath to write notifications to, opened in append mode,
+        or a file-like object. Defaults to 'logs.txt'.
+        """
+        self._filepath = filepath if isinstance(filepath, str) else "logs.txt"
+        self._file = filepath if not isinstance(filepath, str) else None
+
+    def _write(self, message: str):
+        str_ = f"{message}\n"
+        if self._file:
+            self._file.write(str_)
+        else:
+            with open(self._filepath, "a") as file:
+                file.write(str_)
+
+    def task_completed(self):
+        self._write("Task completed")
+
+    def all_tasks_completed(self):
+        self._write("All tasks completed")
+
+    def task_failure(self):
+        self._write("Task failed")
+
+
+class SmtpConfiguration(NamedTuple):
+    """SMTP server configuration options used by :class:`EmailNotificationProvider`."""
+
+    host: str
+    """ SMTP server host. """
+
+    port: int
+    """ SMTP server port. """
+
+    username: Optional[str] = None
+    """ Username to authenticate with. """
+
+    password: Optional[str] = None
+    """ Password to authenticate with. """
+
+    require_tls: Optional[bool] = True
+    """ Whether to require a TLS connection. Defaults to True. """
+
+
+class EmailNotificationProvider(DefaultNotificationProvider):
+    """
+    Sends notifications via email. Requires an SMTP server to connect to.
+
+    For example, to send notifications using a Gmail account::
+
+        smtp_config = SmtpConfiguration(
+            'smtp.gmail.com',
+            587,
+            username='sender@gmail.com',
+            password='password'
+        )
+
+        provider = EmailNotificationProvider(
+            smtp_config,
+            "sender@gmail.com",
+            ["recipient@gmail.com"]
+        )
+    """
+
+    def __init__(
+        self,
+        smtp: Union[SmtpConfiguration, smtplib.SMTP],
+        from_addr: str,
+        to_addrs: Iterable[str],
+    ):
+        """
+        Creates an EmailNotificationProvider.
+
+        :param smtp: SMTP configuration or a smtplib.SMTP object
+        :param from_addr: email address emails will be sent from
+        :param to_addrs: email addresses emails will be sent to
+        """
+        self._smpt_config = (
+            smtp
+            if isinstance(smtp, SmtpConfiguration)
+            else SmtpConfiguration("localhost", 0)
+        )
+        self._client = smtp if isinstance(smtp, smtplib.SMTP) else None
+        self._from_addr = from_addr
+        self._to_addrs = to_addrs
+
+    @property
+    def smpt(self):
+        """This provider's SmtpConfiguration."""
+        return self._smpt_config
+
+    @property
+    def from_addr(self):
+        """Email address emails will be sent from."""
+        return self._from_addr
+
+    @property
+    def to_addrs(self):
+        """Email addresses emails will be sent to."""
+        return self._to_addrs
+
+    def _send_email(self, message: email.message.Message):
+        if self._client:
+            self._client.send_message(message)
+        else:
+            with smtplib.SMTP(self._smpt_config.host, self._smpt_config.port) as smtp:
+                try:
+                    smtp.starttls()
+                except smtplib.SMTPNotSupportedError as error:
+                    if self._smpt_config.require_tls:
+                        raise error
+
+                if (
+                    self._smpt_config.username is not None
+                    and self._smpt_config.password is not None
+                ):
+                    smtp.login(self._smpt_config.username, self._smpt_config.password)
+                smtp.send_message(message)
+
+    def create_message(self, subject: str, content: str) -> email.message.Message:
+        """Creates an :class:`email.message.Message` with the given subject and content."""
+        message = email.message.EmailMessage()
+        message["From"] = formataddr(("Memento", self._from_addr))
+        message["To"] = ",".join(self._to_addrs)
+        message["Subject"] = subject
+        message.set_content(
+            content
+        )  # TODO: Maybe support HTML messages with a plain text fallback
+        return message
+
+    def task_completed(self):
+        message = self.create_message("[Memento] Task completed", "Task completed")
+        self._send_email(message)
+
+    def all_tasks_completed(self):
+        message = self.create_message(
+            "[Memento] All tasks completed", "All tasks completed"
+        )
+        self._send_email(message)
+
+    def task_failure(self):
+        message = self.create_message("[Memento] Task failed", "Task failed")
+        self._send_email(message)
```

### Comparing `memento-ml-1.0.2/memento/task_interface.py` & `memento-ml-1.1.0/memento/task_interface.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,313 +1,313 @@
-"""
-Contains MEMENTO's task interface, once the configurations are
-generated and dispatched to tasks, we need some way to interact
-with the user code
-"""
-import datetime
-import os
-import sqlite3
-import tempfile
-import time
-from collections import namedtuple
-from typing import Any, Optional, Union, Tuple, Dict, List, cast
-from typing import Callable
-
-import cloudpickle
-import pandas as pd
-from pandas import DataFrame
-
-from memento.configurations import Config
-from memento.caching import default_key_provider
-
-Metric = namedtuple("Metric", "x y")
-
-
-class FileSystemCheckpointing:
-    """
-    A filesystem checkpoint. Uses SQLITE3 to write to a database file on disk.
-    """
-
-    def __init__(
-        self,
-        filepath: str = None,
-        key: Callable = None,
-        connection: sqlite3.Connection = None,
-    ):
-        """
-        Creates a FileSystemCheckpointing, optionally using a DB connection or filepath.
-        :param filepath: A filepath to use for the database file.
-        :param connection: A sqlite3 DB connection to use. Supplying this breaks parallelization.
-        """
-        self._filepath = os.path.abspath(
-            filepath or tempfile.NamedTemporaryFile(suffix="_memento.checkpoint").name
-        )
-        self._table_name = "checkpoint_table"
-        self.key = key or default_key_provider
-        self._connection = connection
-
-        self._setup_database()
-
-    def _setup_database(self) -> None:
-        """
-        :return: Nothing.
-        """
-        with self as databases:
-            databases.execute(
-                f"""
-                CREATE TABLE IF NOT EXISTS {self._table_name} (
-                    key BINARY PRIMARY KEY,
-                    ts REAL NOT NULL DEFAULT ((julianday('now') - 2440587.5)*86400.0),
-                    value BLOB NOT NULL
-                ) WITHOUT ROWID
-            """
-            )
-
-    def __enter__(self) -> sqlite3.Connection:
-        """
-        Used to connect to the underlying database safely, handling setup and teardown.
-
-        Runs at the beginning of a `with _ as _` block
-        ...
-            with File_System_Checkpointing_Object as database:
-                database.execute("some SQL")
-
-        :return: A sqlite3 Connection object, representing a database connection.
-        """
-        return self._connection or sqlite3.Connection(
-            self._filepath, isolation_level="DEFERRED"
-        )
-
-    def __exit__(self, exc_type, exc_val, exc_tb) -> None:
-        """
-        Run at the end of the `with _ as _` block
-        ...
-            with File_System_Checkpointing_Object as database:
-                database.execute("some SQL")
-
-        :return: Nothing.
-        """
-
-    def __str__(self) -> str:
-        """
-        Creates a human-readable string of the checkpoint.
-        :return: A string representing the checkpoint.
-        """
-        return f"Filesystem checkpoint, using {self._connection or self._filepath}"
-
-    def get(self, key: str):
-        """
-        Gets the item in the checkpoint specified by the key.
-        :param key: Used to get the item from the cache.
-        :returns: The item in the checkpoint, if it exists.
-        :raise KeyError: When the key has not been checkpoint.
-        """
-        with self as database:
-            rows = database.execute(
-                f"SELECT value FROM {self._table_name} WHERE key = ?", (key,)
-            ).fetchall()
-            if rows:
-                return cloudpickle.loads(rows[0][0])[0]
-
-            raise KeyError(f"Key '{key}' not in checkpoint")
-
-    def set(self, key: str, item) -> None:
-        """
-        Checkpoint the item with a specified key.
-        :param key: The location for the item in checkpoint.
-        :param item: The item to be checkpoint.
-        :returns: Nothing.
-        """
-        with self as database:
-            database.execute(
-                f"INSERT OR REPLACE INTO {self._table_name}(key,value) VALUES(?,?)",
-                (key, cloudpickle.dumps(item)),
-            )
-            database.commit()
-
-    def remove(self, key: str):
-        """
-        Remove checkpoint by using key
-        :param key: Key of the checkpoint
-        :returns: None
-        """
-        with self as database:
-            database.execute(f"DELETE FROM {self._table_name} WHERE key = ?", (key,))
-            database.commit()
-
-    def contains(self, key: str) -> bool:
-        """
-        Checks whether a key has been checkpoint.
-        :param key: The key to check.
-        :returns: True if it exists, False otherwise.
-        """
-        try:
-            self.get(key)
-            return True
-        except KeyError:
-            return False
-
-    def make_key(self, *args, **kwargs) -> str:
-        """
-        Generates a key to be used in checkpointing.
-        :param args: Arguments to the function to be checkpoint.
-        :param kwargs: Keyword arguments to the function to be checkpoint.
-        :returns: True if it exists, False otherwise.
-        """
-        return self.key(*args, **kwargs)
-
-
-class Context:
-    """
-    The ``Context`` makes MEMENTO's utilities like checkpointing, metrics,
-    progress reporting, and more available to tasks.
-    """
-
-    _metrics: Dict[str, List[Metric]]
-
-    def __init__(self, key: str, checkpoint_provider: FileSystemCheckpointing):
-        """
-        Each context is associated with exactly one task.
-
-        :param key: This is the key provided by memento for each task.
-        :param checkpoint_provider: The checkpoint provider, defaults to FileSystemCheckpointing
-        """
-        self.key = key
-        self._metrics = {}
-        self._checkpoint_provider = checkpoint_provider
-        self.checkpoint_key = None
-
-    def collect_metrics(self) -> Dict[str, pd.DataFrame]:
-        """
-        Collects all of the metrics as dataframes.
-        :return: A dictionary of metric names that map to Pandas Dataframes.
-        """
-        metrics: Dict[str, DataFrame] = {}
-        for name in self._metrics:
-            metrics[name] = pd.DataFrame(self._metrics[name])
-
-        return metrics
-
-    def record(self, value_dict: Dict[str, Union[float, Tuple[float, float]]]) -> None:
-        """
-        Records a floating point metric in one of the following formats.
-        Default x value is a timestamp.
-        Metrics are available as part of the results object.
-
-        ..
-            context.record({"metric_name": value})
-            context.record({"metric_name": (x,y)})
-
-            # Record with the same timestamp
-            context.record({"metric_1": value1, "metric_2": value2})
-
-        :return: None.
-        :param value_dict:
-        """
-        x_value = time.time()
-
-        for name in value_dict:
-            y_value = value_dict[name]
-
-            # Handles the case of a tuple
-            if isinstance(y_value, tuple):
-                y_value = cast(Tuple[float, float], y_value)
-                x_value = y_value[0]
-                y_value = y_value[1]
-
-            # Type guards that shouldn't be triggered.
-            assert isinstance(x_value, float)
-            assert isinstance(y_value, float)
-
-            metric = Metric(x_value, y_value)
-            if self._metrics.get(name, False):
-                self._metrics[name].append(metric)
-            else:
-                self._metrics[name] = [metric]
-
-    def progress(self, delta, total=None):  # pylint: disable=no-self-use
-        """
-        Update the progress estimate, changing the current progress by ``delta``.
-        The first call to this should (if possible) estimate the total amount of work.
-        This can later be refined by passing a different value of ``total``.
-        """
-        raise NotADirectoryError("feature: progress")
-
-    def checkpoint(self, *func) -> None:
-        """
-        Save the current state of the task.
-        :param func: The function to be checkpoint.
-        """
-        # self.checkpoint_key = self._checkpoint_provider.make_key(self.key, func)
-        self._checkpoint_provider.set(self.key, func)
-
-    def restore(self):
-        """
-        Save the current state of the task.
-        :return: The function saved to the key
-        """
-        return self._checkpoint_provider.get(self.key)
-
-    def checkpoint_exist(self):
-        """
-        Checks if checkpoint already exists
-        """
-        return self._checkpoint_provider.contains(self.key)
-
-
-class MemoryUsage:
-    """
-    Memory usage statistics recorded from a task.
-    """
-
-    virtual_peak: int
-    hardware_peak: int
-
-    def __init__(self, virtual_peak: int, hardware_peak: int):
-        self.virtual_peak = virtual_peak
-        self.hardware_peak = hardware_peak
-
-
-class Result:
-    """
-    The result from a single task. This contains the value returned from the experiment, ``inner``,
-    and metadata about the task run.
-    """
-
-    config: Config
-
-    inner: Any
-
-    metrics: Dict[str, pd.DataFrame]
-
-    "The start time of the task."
-    start_time: datetime.datetime
-
-    "The task's runtime, measured on the wall clock."
-    runtime: datetime.timedelta
-    "The task's runtime, measured by the CPU"
-    cpu_time: Optional[datetime.timedelta]
-    "Memory usage statistics"
-    memory: Optional[MemoryUsage]
-
-    "Whether or not this result was retrieved from cache."
-    was_cached: bool
-
-    def __init__(  # pylint: disable=too-many-arguments
-        self,
-        config,
-        inner,
-        metrics: Dict[str, pd.DataFrame],
-        start_time: datetime.datetime,
-        runtime: datetime.timedelta,
-        cpu_time: Optional[datetime.timedelta],
-        memory: Optional[MemoryUsage],
-        was_cached: bool,
-    ):
-        self.config = config
-        self.inner = inner
-        self.metrics = metrics
-        self.start_time = start_time
-        self.runtime = runtime
-        self.cpu_time = cpu_time
-        self.memory = memory
-        self.was_cached = was_cached
+"""
+Contains MEMENTO's task interface, once the configurations are
+generated and dispatched to tasks, we need some way to interact
+with the user code
+"""
+import datetime
+import os
+import sqlite3
+import tempfile
+import time
+from collections import namedtuple
+from typing import Any, Optional, Union, Tuple, Dict, List, cast
+from typing import Callable
+
+import cloudpickle
+import pandas as pd
+from pandas import DataFrame
+
+from memento.configurations import Config
+from memento.caching import default_key_provider
+
+Metric = namedtuple("Metric", "x y")
+
+
+class FileSystemCheckpointing:
+    """
+    A filesystem checkpoint. Uses SQLITE3 to write to a database file on disk.
+    """
+
+    def __init__(
+        self,
+        filepath: str = None,
+        key: Callable = None,
+        connection: sqlite3.Connection = None,
+    ):
+        """
+        Creates a FileSystemCheckpointing, optionally using a DB connection or filepath.
+        :param filepath: A filepath to use for the database file.
+        :param connection: A sqlite3 DB connection to use. Supplying this breaks parallelization.
+        """
+        self._filepath = os.path.abspath(
+            filepath or tempfile.NamedTemporaryFile(suffix="_memento.checkpoint").name
+        )
+        self._table_name = "checkpoint_table"
+        self.key = key or default_key_provider
+        self._connection = connection
+
+        self._setup_database()
+
+    def _setup_database(self) -> None:
+        """
+        :return: Nothing.
+        """
+        with self as databases:
+            databases.execute(
+                f"""
+                CREATE TABLE IF NOT EXISTS {self._table_name} (
+                    key BINARY PRIMARY KEY,
+                    ts REAL NOT NULL DEFAULT ((julianday('now') - 2440587.5)*86400.0),
+                    value BLOB NOT NULL
+                ) WITHOUT ROWID
+            """
+            )
+
+    def __enter__(self) -> sqlite3.Connection:
+        """
+        Used to connect to the underlying database safely, handling setup and teardown.
+
+        Runs at the beginning of a `with _ as _` block
+        ...
+            with File_System_Checkpointing_Object as database:
+                database.execute("some SQL")
+
+        :return: A sqlite3 Connection object, representing a database connection.
+        """
+        return self._connection or sqlite3.Connection(
+            self._filepath, isolation_level="DEFERRED"
+        )
+
+    def __exit__(self, exc_type, exc_val, exc_tb) -> None:
+        """
+        Run at the end of the `with _ as _` block
+        ...
+            with File_System_Checkpointing_Object as database:
+                database.execute("some SQL")
+
+        :return: Nothing.
+        """
+
+    def __str__(self) -> str:
+        """
+        Creates a human-readable string of the checkpoint.
+        :return: A string representing the checkpoint.
+        """
+        return f"Filesystem checkpoint, using {self._connection or self._filepath}"
+
+    def get(self, key: str):
+        """
+        Gets the item in the checkpoint specified by the key.
+        :param key: Used to get the item from the cache.
+        :returns: The item in the checkpoint, if it exists.
+        :raise KeyError: When the key has not been checkpoint.
+        """
+        with self as database:
+            rows = database.execute(
+                f"SELECT value FROM {self._table_name} WHERE key = ?", (key,)
+            ).fetchall()
+            if rows:
+                return cloudpickle.loads(rows[0][0])[0]
+
+            raise KeyError(f"Key '{key}' not in checkpoint")
+
+    def set(self, key: str, item) -> None:
+        """
+        Checkpoint the item with a specified key.
+        :param key: The location for the item in checkpoint.
+        :param item: The item to be checkpoint.
+        :returns: Nothing.
+        """
+        with self as database:
+            database.execute(
+                f"INSERT OR REPLACE INTO {self._table_name}(key,value) VALUES(?,?)",
+                (key, cloudpickle.dumps(item)),
+            )
+            database.commit()
+
+    def remove(self, key: str):
+        """
+        Remove checkpoint by using key
+        :param key: Key of the checkpoint
+        :returns: None
+        """
+        with self as database:
+            database.execute(f"DELETE FROM {self._table_name} WHERE key = ?", (key,))
+            database.commit()
+
+    def contains(self, key: str) -> bool:
+        """
+        Checks whether a key has been checkpoint.
+        :param key: The key to check.
+        :returns: True if it exists, False otherwise.
+        """
+        try:
+            self.get(key)
+            return True
+        except KeyError:
+            return False
+
+    def make_key(self, *args, **kwargs) -> str:
+        """
+        Generates a key to be used in checkpointing.
+        :param args: Arguments to the function to be checkpoint.
+        :param kwargs: Keyword arguments to the function to be checkpoint.
+        :returns: True if it exists, False otherwise.
+        """
+        return self.key(*args, **kwargs)
+
+
+class Context:
+    """
+    The ``Context`` makes MEMENTO's utilities like checkpointing, metrics,
+    progress reporting, and more available to tasks.
+    """
+
+    _metrics: Dict[str, List[Metric]]
+
+    def __init__(self, key: str, checkpoint_provider: FileSystemCheckpointing):
+        """
+        Each context is associated with exactly one task.
+
+        :param key: This is the key provided by memento for each task.
+        :param checkpoint_provider: The checkpoint provider, defaults to FileSystemCheckpointing
+        """
+        self.key = key
+        self._metrics = {}
+        self._checkpoint_provider = checkpoint_provider
+        self.checkpoint_key = None
+
+    def collect_metrics(self) -> Dict[str, pd.DataFrame]:
+        """
+        Collects all of the metrics as dataframes.
+        :return: A dictionary of metric names that map to Pandas Dataframes.
+        """
+        metrics: Dict[str, DataFrame] = {}
+        for name in self._metrics:
+            metrics[name] = pd.DataFrame(self._metrics[name])
+
+        return metrics
+
+    def record(self, value_dict: Dict[str, Union[float, Tuple[float, float]]]) -> None:
+        """
+        Records a floating point metric in one of the following formats.
+        Default x value is a timestamp.
+        Metrics are available as part of the results object.
+
+        ..
+            context.record({"metric_name": value})
+            context.record({"metric_name": (x,y)})
+
+            # Record with the same timestamp
+            context.record({"metric_1": value1, "metric_2": value2})
+
+        :return: None.
+        :param value_dict:
+        """
+        x_value = time.time()
+
+        for name in value_dict:
+            y_value = value_dict[name]
+
+            # Handles the case of a tuple
+            if isinstance(y_value, tuple):
+                y_value = cast(Tuple[float, float], y_value)
+                x_value = y_value[0]
+                y_value = y_value[1]
+
+            # Type guards that shouldn't be triggered.
+            assert isinstance(x_value, float)
+            assert isinstance(y_value, float)
+
+            metric = Metric(x_value, y_value)
+            if self._metrics.get(name, False):
+                self._metrics[name].append(metric)
+            else:
+                self._metrics[name] = [metric]
+
+    def progress(self, delta, total=None):  # pylint: disable=no-self-use
+        """
+        Update the progress estimate, changing the current progress by ``delta``.
+        The first call to this should (if possible) estimate the total amount of work.
+        This can later be refined by passing a different value of ``total``.
+        """
+        raise NotADirectoryError("feature: progress")
+
+    def checkpoint(self, *func) -> None:
+        """
+        Save the current state of the task.
+        :param func: The function to be checkpoint.
+        """
+        # self.checkpoint_key = self._checkpoint_provider.make_key(self.key, func)
+        self._checkpoint_provider.set(self.key, func)
+
+    def restore(self):
+        """
+        Save the current state of the task.
+        :return: The function saved to the key
+        """
+        return self._checkpoint_provider.get(self.key)
+
+    def checkpoint_exist(self):
+        """
+        Checks if checkpoint already exists
+        """
+        return self._checkpoint_provider.contains(self.key)
+
+
+class MemoryUsage:
+    """
+    Memory usage statistics recorded from a task.
+    """
+
+    virtual_peak: int
+    hardware_peak: int
+
+    def __init__(self, virtual_peak: int, hardware_peak: int):
+        self.virtual_peak = virtual_peak
+        self.hardware_peak = hardware_peak
+
+
+class Result:
+    """
+    The result from a single task. This contains the value returned from the experiment, ``inner``,
+    and metadata about the task run.
+    """
+
+    config: Config
+
+    inner: Any
+
+    metrics: Dict[str, pd.DataFrame]
+
+    "The start time of the task."
+    start_time: datetime.datetime
+
+    "The task's runtime, measured on the wall clock."
+    runtime: datetime.timedelta
+    "The task's runtime, measured by the CPU"
+    cpu_time: Optional[datetime.timedelta]
+    "Memory usage statistics"
+    memory: Optional[MemoryUsage]
+
+    "Whether or not this result was retrieved from cache."
+    was_cached: bool
+
+    def __init__(  # pylint: disable=too-many-arguments
+        self,
+        config,
+        inner,
+        metrics: Dict[str, pd.DataFrame],
+        start_time: datetime.datetime,
+        runtime: datetime.timedelta,
+        cpu_time: Optional[datetime.timedelta],
+        memory: Optional[MemoryUsage],
+        was_cached: bool,
+    ):
+        self.config = config
+        self.inner = inner
+        self.metrics = metrics
+        self.start_time = start_time
+        self.runtime = runtime
+        self.cpu_time = cpu_time
+        self.memory = memory
+        self.was_cached = was_cached
```

### Comparing `memento-ml-1.0.2/memento_ml.egg-info/PKG-INFO` & `memento-ml-1.1.0/memento_ml.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,251 +1,202 @@
-Metadata-Version: 2.1
-Name: memento-ml
-Version: 1.0.2
-Summary: A Python library for running computationally expensive experiments
-Author-email: Wickerlab dev team <luke.x.chang@gmail.com>
-License: BSD 3-Clause License
-        
-        Copyright (c) 2023, wickerlab
-        
-        Redistribution and use in source and binary forms, with or without
-        modification, are permitted provided that the following conditions are met:
-        
-        1. Redistributions of source code must retain the above copyright notice, this
-           list of conditions and the following disclaimer.
-        
-        2. Redistributions in binary form must reproduce the above copyright notice,
-           this list of conditions and the following disclaimer in the documentation
-           and/or other materials provided with the distribution.
-        
-        3. Neither the name of the copyright holder nor the names of its
-           contributors may be used to endorse or promote products derived from
-           this software without specific prior written permission.
-        
-        THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
-        AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
-        IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
-        DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
-        FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
-        DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
-        SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
-        CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
-        OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
-        OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
-        
-Project-URL: Homepage, https://github.com/wickerlab/memento
-Keywords: experiment,parallel,sklearn,machine learning
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Requires-Python: <3.10,>=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
-[![PyPI](https://img.shields.io/pypi/v/memento-ml)](https://pypi.org/project/memento-ml/)
-![Python versions](https://img.shields.io/pypi/pyversions/memento-ml)
-
-# Memento
-
-Memento is a Python library for running computationally expensive experiments.
-
-If you need to run a large number of time-consuming experiments Memento can help:
-
-- Structure your configuration
-- Parallelize experiments across CPUs
-- Save and restore results
-- Checkpoint in-progress experiments
-- Send notifications when experiments fail or finish
-
-## Getting Started
-
-### Install
-
-```bash
-pip install memento-ml
-```
-
-### The Configuration Matrix
-
-The core of Memento is a configuration `matrix` that describes the list of experiments you
-want Memento to run. This must contain a key `parameters` which is itself a dict, this describes
-each paramter you want to vary for your experiments and their values.
-
-As an example let's say you wanted to test a few simple linear classifiers on a number of
-image recognition datasets. You might write something like this:
-
-> Don't worry if you're not working on machine learning, this is just an example.
-
-```python
-matrix = {
-  "parameters": {
-    "model": [
-      sklearn.svm.SVC,
-      sklearn.linear_model.Perceptron,
-      sklearn.linear_model.LogisticRegression
-    ],
-    "dataset": ["imagenet", "mnist", "cifar10", "quickdraw"]
-  }
-}
-```
-
-Memento would then generate 12 configurations by taking the _cartesian product_ of the
-parameters.
-
-Frequently you might also want to set some global configuration values, such as a regularization
-parameter or potentially even change your preprocessing pipeline. In this case Memento also
-accepts a "settings" key. These settings apply to all experiments and can be accessed from the
-configuration list as well as individual configurations.
-
-```python
-matrix = {
-  "parameters": ...,
-  "settings": {
-    "regularization": 1e-1,
-    "preprocessing": make_preprocessing_pipeline()
-  }
-}
-```
-
-You can also exclude specific parameter configurations. Returning to our machine learning
-example, if you know SVCs perform poorly on cifar10 you might decide to skip that
-experiment entirely. This is done with the "exclude" key:
-
-```python
-matrix = {
-  "parameters": ...,
-  "exclude": [
-    {"model": sklearn.svm.SVC, "dataset": "cifar10"}
-  ]
-}
-```
-
-### Running an experiment
-
-Along with a configuration matrix you need some code to run your experiments. This can be any
-`Callable` such as a function, lambda, class, or class method.
-
-```python
-from memento import Memento, Config, Context
-
-def experiment(context: Context, config: Config):
-  classifier = config.model()
-  dataset = fetch_dataset(config.dataset)
-
-  classifier.fit(*dataset)
-
-  return classifier
-
-Memento(experiment).run(matrix)
-```
-
-You can also perform a dry run to check you've gotten the matrix correct.
-
-```python
-Memento(experiment).run(matrix, dry_run=True)
-```
-
-```python
-Running configurations:
-  {'model': sklearn.svm.SVC, 'dataset': 'imagenet'}
-  {'model': sklearn.svm.SVC, 'dataset': 'mnist'}
-  {'model': sklearn.svm.SVC, 'dataset': 'cifar10'}
-  {'model': sklearn.svm.SVC, 'dataset': 'quickdraw'}
-  {'model': sklearn.linear_model.Perceptron, 'dataset': 'imagenet'}
-  ...
-Exiting due to dry run
-```
-
-## Code demo
-
-- Code demo can be found [here](demo).
-- `Memento` does not depend on `scikit-learn`. The `scikit-learn` and `jupyterlab` packages are required to run the demo (`./demo/*`).
-
-```bash
-pip install scikit-learn jupyterlab
-```
-
-## Developing
-
-### Install as local package in Editable mode
-
-```bash
-pip install -e .
-
-```
-
-### Install development dependencies
-
-```bash
-pip install memento-ml[dev]
-```
-
-### Tests
-
-```bash
-pytest
-```
-
-Alternatively to only run a subset of tests that haven't been marked as time consuming/slow you can use:
-
-```bash
-pytest -m "not slow"
-```
-
-### Linters
-
-```bash
-pylint memento
-```
-
-### Format code
-
-```bash
-black .
-```
-
-### Build Documentation
-
-```bash
-sphinx-apidoc -o docs memento -f
-sphinx-build -W -b html docs docs/_build
-```
-
-### Bump up version
-
-```bash
-# The `--dry` flag is for testing only. Remove `--dry` to update the version number.
-# Use `minor` instead of `patch` for feature updates.
-bumpver update --patch --dry
-```
-
-### Run CI locally
-
-Install [act](https://github.com/nektos/act), then:
-
-```bash
-act
-```
-
-## Roadmap
-
-- Finish HPC support
-- Improve result serialisation
-- Production testing & fleshed-out integration test suite
-
-## Contributors
-
-- [Zac Pullar-Strecker](https://github.com/zacps)
-- [Feras Albaroudi](https://github.com/NeedsSoySauce)
-- [Liam Scott-Russell](https://github.com/Liam-Scott-Russell)
-- [Joshua de Wet](https://github.com/Dewera)
-- [Nipun Jasti](https://github.com/watefeenex)
-- [James Lamberton](https://github.com/JamesLamberton)
-- [Joerg Wicker](https://github.com/joergwicker)
-- [Xinglong (Luke) Chang](https://github.com/changx03)
-
-## License
-
-Memento is licensed under the [3-Clause BSD License](https://opensource.org/licenses/BSD-3-Clause) license.
+Metadata-Version: 2.1
+Name: memento-ml
+Version: 1.1.0
+Summary: A Python library for running computationally expensive experiments
+Author-email: Wickerlab dev team <luke.x.chang@gmail.com>
+License: BSD 3-Clause License
+        
+        Copyright (c) 2023, wickerlab
+        
+        Redistribution and use in source and binary forms, with or without
+        modification, are permitted provided that the following conditions are met:
+        
+        1. Redistributions of source code must retain the above copyright notice, this
+           list of conditions and the following disclaimer.
+        
+        2. Redistributions in binary form must reproduce the above copyright notice,
+           this list of conditions and the following disclaimer in the documentation
+           and/or other materials provided with the distribution.
+        
+        3. Neither the name of the copyright holder nor the names of its
+           contributors may be used to endorse or promote products derived from
+           this software without specific prior written permission.
+        
+        THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+        AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+        IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+        DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
+        FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
+        DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
+        SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
+        CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
+        OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
+        OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+        
+Project-URL: Homepage, https://github.com/wickerlab/memento
+Keywords: experiment,parallel,sklearn,machine learning
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Provides-Extra: dev
+License-File: LICENSE
+
+[![PyPI](https://img.shields.io/pypi/v/memento-ml)](https://pypi.org/project/memento-ml/)
+![Python versions](https://img.shields.io/pypi/pyversions/memento-ml)
+
+# MEMENTO
+
+`MEMENTO` is a Python library for running computationally expensive experiments.
+
+Running complex sets of machine learning experiments is challenging and time-consuming due to the lack of a unified framework.
+This leaves researchers forced to spend time implementing necessary features such as parallelization, caching, and checkpointing themselves instead of focussing on their project.
+To simplify the process, we introduce `MEMENTO`, a Python package that is designed to aid researchers and data scientists in the efficient management and execution of computationally intensive experiments.
+`MEMENTO` has the capacity to streamline any experimental pipeline by providing a straightforward configuration matrix and the ability to concurrently run experiments across multiple threads.
+
+If you need to run a large number of time-consuming experiments `MEMENTO` can help:
+
+- Structure your configuration
+- Parallelize experiments across CPUs
+- Save and restore results
+- Checkpoint in-progress experiments
+- Send notifications when experiments fail or finish
+
+[![Demo video](https://img.youtube.com/vi/GEtdCl1ZUWc/0.jpg)](http://www.youtube.com/watch?v=GEtdCl1ZUWc)
+
+## Getting Started
+
+`MEMENTO` is officially available on PyPl. To install the package:
+
+### Install
+
+```bash
+pip install memento-ml
+```
+
+### The Configuration Matrix
+
+The core of `MEMENTO` is a configuration `matrix` that describes the list of experiments you
+want `MEMENTO` to run. This must contain a key `parameters` which is itself a dict, this describes
+each paramter you want to vary for your experiments and their values.
+
+As an example let's say you wanted to test a few simple linear classifiers on a number of
+image recognition datasets. You might write something like this:
+
+> Don't worry if you're not working on machine learning, this is just an example.
+
+```python
+matrix = {
+  "parameters": {
+    "model": [
+      sklearn.svm.SVC,
+      sklearn.linear_model.Perceptron,
+      sklearn.linear_model.LogisticRegression
+    ],
+    "dataset": ["imagenet", "mnist", "cifar10", "quickdraw"]
+  }
+}
+```
+
+`MEMENTO` would then generate 12 configurations by taking the _cartesian product_ of the
+parameters.
+
+Frequently you might also want to set some global configuration values, such as a regularization
+parameter or potentially even change your preprocessing pipeline. In this case `MEMENTO` also
+accepts a "settings" key. These settings apply to all experiments and can be accessed from the
+configuration list as well as individual configurations.
+
+```python
+matrix = {
+  "parameters": ...,
+  "settings": {
+    "regularization": 1e-1,
+    "preprocessing": make_preprocessing_pipeline()
+  }
+}
+```
+
+You can also exclude specific parameter configurations. Returning to our machine learning
+example, if you know SVCs perform poorly on cifar10 you might decide to skip that
+experiment entirely. This is done with the "exclude" key:
+
+```python
+matrix = {
+  "parameters": ...,
+  "exclude": [
+    {"model": sklearn.svm.SVC, "dataset": "cifar10"}
+  ]
+}
+```
+
+### Running an experiment
+
+Along with a configuration matrix you need some code to run your experiments. This can be any
+`Callable` such as a function, lambda, class, or class method.
+
+```python
+from memento import Memento, Config, Context
+
+def experiment(context: Context, config: Config):
+  classifier = config.model()
+  dataset = fetch_dataset(config.dataset)
+
+  classifier.fit(*dataset)
+
+  return classifier
+
+Memento(experiment).run(matrix)
+```
+
+You can also perform a dry run to check you've gotten the matrix correct.
+
+```python
+Memento(experiment).run(matrix, dry_run=True)
+```
+
+```python
+Running configurations:
+  {'model': sklearn.svm.SVC, 'dataset': 'imagenet'}
+  {'model': sklearn.svm.SVC, 'dataset': 'mnist'}
+  {'model': sklearn.svm.SVC, 'dataset': 'cifar10'}
+  {'model': sklearn.svm.SVC, 'dataset': 'quickdraw'}
+  {'model': sklearn.linear_model.Perceptron, 'dataset': 'imagenet'}
+  ...
+Exiting due to dry run
+```
+
+## Code demo
+
+- Code demo can be found [here](demo).
+- `MEMENTO` does not depend on any ML packages, e.g., `scikit-learn`. The `scikit-learn` and `jupyterlab` packages are required to run the demo (`./demo/*`).
+
+```bash
+pip install memento-ml scikit-learn jupyterlab
+```
+
+## Roadmap
+
+- Finish HPC support
+- Improve result serialisation
+- Improve customization for notification
+
+## Contributors
+
+- [Zac Pullar-Strecker](https://github.com/zacps)
+- [Feras Albaroudi](https://github.com/NeedsSoySauce)
+- [Liam Scott-Russell](https://github.com/Liam-Scott-Russell)
+- [Joshua de Wet](https://github.com/Dewera)
+- [Nipun Jasti](https://github.com/watefeenex)
+- [James Lamberton](https://github.com/JamesLamberton)
+- [Xinglong (Luke) Chang](https://github.com/changx03)
+- [Liam Brydon](https://github.com/MyCreativityOutlet)
+- [Ioannis Ziogas](izio995@aucklanduni.ac.nz)
+- [Katharina Dost](katharina.dost@auckland.ac.nz)
+- [Joerg Wicker](https://github.com/joergwicker)
+
+## License
+
+MEMENTO is licensed under the [3-Clause BSD License](https://opensource.org/licenses/BSD-3-Clause) license.
```

### Comparing `memento-ml-1.0.2/memento_ml.egg-info/SOURCES.txt` & `memento-ml-1.1.0/memento_ml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `memento-ml-1.0.2/pyproject.toml` & `memento-ml-1.1.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,79 +1,80 @@
-# pyproject.toml
-
-[build-system]
-requires = ["setuptools>=67.4.0", "wheel"]
-build-backend = "setuptools.build_meta"
-
-[project]
-name = "memento-ml"
-version = "1.0.2"
-description = "A Python library for running computationally expensive experiments"
-readme = "README.md"
-authors = [
-    { name = "Wickerlab dev team", email = "luke.x.chang@gmail.com" },
-]
-license = { file = "LICENSE" }
-classifiers = [
-    "License :: OSI Approved :: BSD License",
-    "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.7",
-    "Programming Language :: Python :: 3.8",
-    "Programming Language :: Python :: 3.9",
-
-]
-keywords = ["experiment", "parallel", "sklearn", "machine learning"]
-requires-python = ">=3.7, <3.10"
-dependencies = [
-    "cloudpickle >= 1.6.0, < 2",
-    "networkx >= 2.5.1, < 3",
-    "pandas >= 1.3.5, < 2",
-    "pandas-stubs",
-]
-
-[project.optional-dependencies]
-dev = [
-    "black", 
-    "pylint",
-    "bumpver", 
-    "isort", 
-    "pip-tools", 
-    "pytest",
-    "Sphinx",
-    "mypy",
-    "aiosmtpd",
-    "scikit-learn",
-]
-
-[project.urls]
-Homepage = "https://github.com/wickerlab/memento"
-
-[tool.setuptools]
-packages = ["memento"]
-py-modules = ["memento"]
-
-[tool.pylint.miscellaneous]
-# Allow TODO notes
-notes = "FIXME,XXX"
-disable = ["too-many-instance-attributes", "too-few-public-methods"]
-
-[tool.pytest.ini_options]
-markers = [
-    "slow"
-]
-log_cli=true
-log_level="NOTSET"
-
-[tool.bumpver]
-current_version = "1.0.2"
-version_pattern = "MAJOR.MINOR.PATCH"
-commit_message = "bump version {old_version} -> {new_version}"
-commit = true
-tag = true
-push = false
-
-[tool.bumpver.file_patterns]
-"pyproject.toml" = [
-    'current_version = "{version}"',
-    'version = "{version}"',
-]
-"memento/__init__.py" = ["{version}"]
+# pyproject.toml
+
+[build-system]
+requires = ["setuptools>=67.4.0", "wheel"]
+build-backend = "setuptools.build_meta"
+
+[project]
+name = "memento-ml"
+version = "1.1.0"
+description = "A Python library for running computationally expensive experiments"
+readme = "README.md"
+authors = [
+    { name = "Wickerlab dev team", email = "luke.x.chang@gmail.com" },
+]
+license = { file = "LICENSE" }
+classifiers = [
+    "License :: OSI Approved :: BSD License",
+    "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11"
+
+]
+keywords = ["experiment", "parallel", "sklearn", "machine learning"]
+requires-python = ">=3.8"
+dependencies = [
+    "cloudpickle ~= 2.2.1",
+    "networkx ~= 3.1",
+    "pandas ~= 2.0.1",
+    "pandas-stubs",
+]
+
+[project.optional-dependencies]
+dev = [
+    "black", 
+    "pylint",
+    "bumpver", 
+    "isort", 
+    "pip-tools", 
+    "pytest",
+    "Sphinx",
+    "mypy",
+    "aiosmtpd",
+    "scikit-learn",
+]
+
+[project.urls]
+Homepage = "https://github.com/wickerlab/memento"
+
+[tool.setuptools]
+packages = ["memento"]
+py-modules = ["memento"]
+
+[tool.pylint.miscellaneous]
+# Allow TODO notes
+notes = "FIXME,XXX"
+disable = ["too-many-instance-attributes", "too-few-public-methods"]
+
+[tool.pytest.ini_options]
+markers = [
+    "slow"
+]
+log_cli=true
+log_level="NOTSET"
+
+[tool.bumpver]
+current_version = "1.1.0"
+version_pattern = "MAJOR.MINOR.PATCH"
+commit_message = "bump version {old_version} -> {new_version}"
+commit = true
+tag = true
+push = false
+
+[tool.bumpver.file_patterns]
+"pyproject.toml" = [
+    'current_version = "{version}"',
+    'version = "{version}"',
+]
+"memento/__init__.py" = ["{version}"]
```

### Comparing `memento-ml-1.0.2/tests/test_caching.py` & `memento-ml-1.1.0/tests/test_caching.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,252 +1,265 @@
-import time
-import os
-import tempfile
-
-from sqlite3 import Connection
-from unittest.mock import Mock
-import pytest
-import cloudpickle
-from memento.caching import (
-    Cache,
-    MemoryCacheProvider,
-    CacheProvider,
-    FileSystemCacheProvider,
-)
-from memento.parallel import TaskManager, delayed
-
-
-class TestCache:
-    def test_cache_calls_underlying_function_when_not_in_cache(self):
-        underlying_func = Mock()
-        cache_provider = Mock(spec_set=CacheProvider)
-        cache_provider.get.side_effect = KeyError()
-
-        cached = Cache(underlying_func, cache_provider)
-        cached({"key1": "value1"})
-        underlying_func.assert_called_with({"key1": "value1"})
-
-    def test_cache_does_not_execute_already_cached_function(self):
-        underlying_func = Mock()
-        cache_provider = Mock(spec_set=CacheProvider)
-        cache_provider.contains.return_value = True
-        cached_function = Cache(underlying_func, cache_provider=cache_provider)
-
-        cached_function()
-
-        underlying_func.assert_not_called()
-
-    def test_cache_saves_function_result_if_not_in_cache(self):
-        result = "result"
-        cache_key = "not_in_cache"
-        underlying_func = Mock(return_value=result)
-        cache_provider = Mock(spec_set=CacheProvider)
-        cache_provider.make_key.return_value = cache_key
-        cache_provider.get.side_effect = KeyError()
-
-        cached_function = Cache(underlying_func, cache_provider=cache_provider)
-
-        cached_function()
-
-        cache_provider.set.assert_called_once_with(cache_key, result)
-
-    def test_cache_creates_file_system_cache_provider_by_default(self):
-        cache = Cache(lambda x: x + 1)
-        assert isinstance(cache._cache_provider, FileSystemCacheProvider)
-
-    def test_cache_force_cache(self):
-        underlying_func = Mock()
-        cache_provider = Mock(spec_set=CacheProvider)
-        cache_provider.get.side_effect = KeyError()
-
-        cached = Cache(underlying_func, cache_provider)
-        with pytest.raises(KeyError):
-            cached({"key1": "value1"}, force_cache=True)
-        underlying_func.assert_not_called()
-
-    def test_cache_force_run(self):
-        def func():
-            return time.monotonic()
-
-        cached_function = Cache(func, cache_provider=MemoryCacheProvider())
-
-        first = cached_function()
-        time.sleep(0.1)
-        second = cached_function()
-        time.sleep(0.1)
-        third = cached_function(force_run=True)
-
-        assert first == second and second != third
-
-
-class TestMemoryCacheProvider:
-    def test_memory_cache_provider_get_works_when_data_in_cache(self):
-        provider = MemoryCacheProvider({"key": "value"})
-        value = provider.get("key")
-        assert value == "value"
-
-    def test_memory_cache_provider_set_works(self):
-        provider = MemoryCacheProvider()
-        provider.set("key", "value")
-        assert provider._cache.get("key") == "value"
-
-    def test_memory_cache_provider_contains_works(self):
-        provider = MemoryCacheProvider({"key": "value"})
-        assert provider.contains("key") is True
-        assert provider.contains("not_in_cache") is False
-
-    def test_memory_cache_provider_creates_initial_empty_cache(self):
-        provider = MemoryCacheProvider()
-        assert provider._cache == {}
-
-    def test_memory_cache_provider_creates_initial_cache_when_provided(self):
-        initial_cache = {"key1": "value1", "key2": 123}
-        provider = MemoryCacheProvider(initial_cache)
-        assert provider._cache == initial_cache
-
-    def test_memory_cache_provider_creates_correct_keys(self):
-        def function(*args):
-            return args
-
-        arguments = ("test1", "test2", 123, True)
-        keyword_arguments = {
-            "key1": "value1",
-            "key2": "value2",
-            "key3": 321,
-            "key4": False,
-        }
-        expected = cloudpickle.dumps(
-            {
-                "function": function,
-                "args": arguments,
-                "kwargs": keyword_arguments,
-            }
-        )
-
-        provider = MemoryCacheProvider()
-        actual = provider.make_key(function, *arguments, **keyword_arguments)
-
-        assert expected == actual
-
-    def test_memory_cache_provider_raises_key_error_when_key_not_in_cache(self):
-        provider = MemoryCacheProvider()
-        with pytest.raises(KeyError) as error_info:
-            provider.get("not_in_cache")
-
-
-class TestFileSystemCacheProvider:
-    def setup_method(self, method):
-        # This is ugly, but sqlite3 doesn't seem to accept a file handle directly, so we need to
-        # create a temporary file, close it (to not run afoul of locking on windows), then manually
-        # remove it after we're done.
-        file = tempfile.NamedTemporaryFile(suffix="_memento.cache", delete=False)
-        self._filepath = os.path.abspath(file.name)
-        file.close()
-
-    def teardown_method(self, method):
-        os.unlink(self._filepath)
-
-    def test_file_system_cache_provider_get_works_when_data_in_cache(self):
-        connection = Mock(spec_set=Connection)
-        connection.execute().fetchall.return_value = [[cloudpickle.dumps("value")]]
-        provider = FileSystemCacheProvider(connection=connection)
-
-        value = provider.get("key")
-
-        assert value == "value"
-
-    def test_file_system_cache_provider_set_works(self):
-        connection = Mock(spec_set=Connection)
-        provider = FileSystemCacheProvider(connection=connection)
-
-        provider.set("key", "value")
-
-        assert connection.execute.called_once_with(
-            "INSERT OR REPLACE INTO cache (key, value) VALUES (?, ?)", "key", "value"
-        )
-
-    def test_file_system_cache_provider_contains_works_when_key_in_file(self):
-        connection = Mock(spec_set=Connection)
-        connection.execute().fetchall.return_value = [[cloudpickle.dumps("value")]]
-        provider = FileSystemCacheProvider(connection=connection)
-
-        assert provider.contains("key") is True
-
-    def test_file_system_cache_provider_contains_works_when_key_not_in_file(self):
-        connection = Mock(spec_set=Connection)
-        connection.execute().fetchall.return_value = None
-        provider = FileSystemCacheProvider(connection=connection)
-
-        assert provider.contains("not_in_cache") is False
-
-    def test_file_system_cache_provider_creates_correct_keys(self):
-        def function(*args):
-            return args
-
-        arguments = ("test1", "test2", 123, True)
-        keyword_arguments = {
-            "key1": "value1",
-            "key2": "value2",
-            "key3": 321,
-            "key4": False,
-        }
-        expected = cloudpickle.dumps(
-            {
-                "function": function,
-                "args": arguments,
-                "kwargs": keyword_arguments,
-            }
-        )
-
-        connection = Mock(spec_set=Connection)
-        provider = FileSystemCacheProvider(connection)
-        actual = provider.make_key(function, *arguments, **keyword_arguments)
-
-        assert expected == actual
-
-    def test_file_system_cache_provider_get_raises_key_error_when_key_not_in_cache(
-        self,
-    ):
-        connection = Mock(spec_set=Connection)
-        connection.execute().fetchall.return_value = None
-        provider = FileSystemCacheProvider(connection=connection)
-        with pytest.raises(KeyError) as error_info:
-            provider.get("not_in_cache")
-
-    def test_file_system_cache_provider_sets_then_gets_to_file(self):
-        provider = FileSystemCacheProvider()
-        provider.set("test_key1", "test_value1")
-        provider.set("test_key2", "test_value2")
-        provider.set("test_key1", "test_value3")
-
-        assert provider.get("test_key1") == "test_value3"
-        assert provider.get("test_key2") == "test_value2"
-
-    def test_file_system_cache_provider_does_not_close_supplied_connection(self):
-        connection = Mock(spec_set=Connection)
-        connection.execute().fetchall.return_value = [[cloudpickle.dumps("value")]]
-        provider = FileSystemCacheProvider(connection=connection)
-
-        provider.set("key", "value")
-        provider.get("key")
-        provider.make_key(lambda x: x + 1, 1)
-
-        del provider
-
-        connection.close.assert_not_called()
-
-    @pytest.mark.slow
-    def test_file_system_cache_provider_works_in_parallel(self):
-        provider = FileSystemCacheProvider()
-
-        def underlying_func(a, b):
-            return a + b
-
-        cached_func = Cache(underlying_func, cache_provider=provider)
-
-        manager = TaskManager()
-        for x in range(10):
-            manager.add_task(delayed(cached_func)(1, 1))
-
-        res = manager.run()
-
-        assert res == [2] * 10
+import time
+import os
+import tempfile
+import hashlib
+from sqlite3 import Connection
+from unittest.mock import Mock
+import pytest
+import cloudpickle
+from memento.caching import (
+    Cache,
+    MemoryCacheProvider,
+    CacheProvider,
+    FileSystemCacheProvider,
+)
+from memento.parallel import TaskManager, delayed
+
+
+class TestCache:
+    def test_cache_calls_underlying_function_when_not_in_cache(self):
+        underlying_func = Mock()
+        cache_provider = Mock(spec_set=CacheProvider)
+        cache_provider.get.side_effect = KeyError()
+
+        cached = Cache(underlying_func, cache_provider)
+        cached({"key1": "value1"})
+        underlying_func.assert_called_with({"key1": "value1"})
+
+    def test_cache_does_not_execute_already_cached_function(self):
+        underlying_func = Mock()
+        cache_provider = Mock(spec_set=CacheProvider)
+        cache_provider.contains.return_value = True
+        cached_function = Cache(underlying_func, cache_provider=cache_provider)
+
+        cached_function()
+
+        underlying_func.assert_not_called()
+
+    def test_cache_saves_function_result_if_not_in_cache(self):
+        result = "result"
+        cache_key = "not_in_cache"
+        underlying_func = Mock(return_value=result)
+        cache_provider = Mock(spec_set=CacheProvider)
+        cache_provider.make_key.return_value = cache_key
+        cache_provider.get.side_effect = KeyError()
+
+        cached_function = Cache(underlying_func, cache_provider=cache_provider)
+
+        cached_function()
+
+        cache_provider.set.assert_called_once_with(cache_key, result)
+
+    def test_cache_creates_file_system_cache_provider_by_default(self):
+        cache = Cache(lambda x: x + 1)
+        assert isinstance(cache._cache_provider, FileSystemCacheProvider)
+
+    def test_cache_force_cache(self):
+        underlying_func = Mock()
+        cache_provider = Mock(spec_set=CacheProvider)
+        cache_provider.get.side_effect = KeyError()
+
+        cached = Cache(underlying_func, cache_provider)
+        with pytest.raises(KeyError):
+            cached({"key1": "value1"}, force_cache=True)
+        underlying_func.assert_not_called()
+
+    def test_cache_force_run(self):
+        def func():
+            return time.monotonic()
+
+        cached_function = Cache(func, cache_provider=MemoryCacheProvider())
+
+        first = cached_function()
+        time.sleep(0.1)
+        second = cached_function()
+        time.sleep(0.1)
+        third = cached_function(force_run=True)
+
+        assert first == second and second != third
+
+
+class TestMemoryCacheProvider:
+    def test_memory_cache_provider_get_works_when_data_in_cache(self):
+        provider = MemoryCacheProvider({"key": "value"})
+        value = provider.get("key")
+        assert value == "value"
+
+    def test_memory_cache_provider_set_works(self):
+        provider = MemoryCacheProvider()
+        provider.set("key", "value")
+        assert provider._cache.get("key") == "value"
+
+    def test_memory_cache_provider_contains_works(self):
+        provider = MemoryCacheProvider({"key": "value"})
+        assert provider.contains("key") is True
+        assert provider.contains("not_in_cache") is False
+
+    def test_memory_cache_provider_creates_initial_empty_cache(self):
+        provider = MemoryCacheProvider()
+        assert provider._cache == {}
+
+    def test_memory_cache_provider_creates_initial_cache_when_provided(self):
+        initial_cache = {"key1": "value1", "key2": 123}
+        provider = MemoryCacheProvider(initial_cache)
+        assert provider._cache == initial_cache
+
+    def test_memory_cache_provider_creates_correct_keys(self):
+        def function(*args):
+            return args
+
+        arguments = ("test1", "test2", 123, True)
+        keyword_arguments = {
+            "key1": "value1",
+            "key2": "value2",
+            "key3": 321,
+            "key4": False,
+        }
+        expected = cloudpickle.dumps(
+            {
+                "function": function,
+                "args": arguments,
+                "kwargs": keyword_arguments,
+            }
+        )
+
+        provider = MemoryCacheProvider()
+        actual = provider.make_key(function, *arguments, **keyword_arguments)
+
+        assert expected == actual
+
+    def test_memory_cache_provider_raises_key_error_when_key_not_in_cache(self):
+        provider = MemoryCacheProvider()
+        with pytest.raises(KeyError) as error_info:
+            provider.get("not_in_cache")
+
+
+class TestFileSystemCacheProvider:
+    def setup_method(self, method):
+        # This is ugly, but sqlite3 doesn't seem to accept a file handle directly, so we need to
+        # create a temporary file, close it (to not run afoul of locking on windows), then manually
+        # remove it after we're done.
+        file = tempfile.NamedTemporaryFile(suffix="_memento.cache", delete=False)
+        self._filepath = os.path.abspath(file.name)
+        file.close()
+
+    def teardown_method(self, method):
+        os.unlink(self._filepath)
+
+    def test_file_system_cache_provider_get_works_when_data_in_cache(self):
+        connection = Mock(spec_set=Connection)
+        try:
+            os.mkdir("memento_cache")
+        except FileExistsError:
+            pass
+        path = f"memento_cache/{hashlib.sha256(b'key').hexdigest()}.pkl"
+        with open(path, "wb") as test_file:
+            cloudpickle.dump("value", test_file)
+        connection.execute().fetchall.return_value = [[path]]
+        provider = FileSystemCacheProvider(connection=connection)
+
+        value = provider.get("key")
+
+        assert value == "value"
+
+    def test_file_system_cache_provider_set_works(self):
+        connection = Mock(spec_set=Connection)
+        provider = FileSystemCacheProvider(connection=connection)
+
+        provider.set("key", "value")
+
+        assert connection.execute.called_once_with(
+            "INSERT OR REPLACE INTO cache (key, value) VALUES (?, ?)", "key", "value"
+        )
+
+    def test_file_system_cache_provider_contains_works_when_key_in_file(self):
+        connection = Mock(spec_set=Connection)
+        path = f"memento_cache/{hashlib.sha256(b'key').hexdigest()}.pkl"
+        with open(path, "wb") as test_file:
+            cloudpickle.dump("value", test_file)
+        connection.execute().fetchall.return_value = [[path]]
+        provider = FileSystemCacheProvider(connection=connection)
+
+        assert provider.contains("key") is True
+
+    def test_file_system_cache_provider_contains_works_when_key_not_in_file(self):
+        connection = Mock(spec_set=Connection)
+        connection.execute().fetchall.return_value = None
+        provider = FileSystemCacheProvider(connection=connection)
+
+        assert provider.contains("not_in_cache") is False
+
+    def test_file_system_cache_provider_creates_correct_keys(self):
+        def function(*args):
+            return args
+
+        arguments = ("test1", "test2", 123, True)
+        keyword_arguments = {
+            "key1": "value1",
+            "key2": "value2",
+            "key3": 321,
+            "key4": False,
+        }
+        expected = cloudpickle.dumps(
+            {
+                "function": function,
+                "args": arguments,
+                "kwargs": keyword_arguments,
+            }
+        )
+
+        connection = Mock(spec_set=Connection)
+        provider = FileSystemCacheProvider(connection)
+        actual = provider.make_key(function, *arguments, **keyword_arguments)
+
+        assert expected == actual
+
+    def test_file_system_cache_provider_get_raises_key_error_when_key_not_in_cache(
+        self,
+    ):
+        connection = Mock(spec_set=Connection)
+        connection.execute().fetchall.return_value = None
+        provider = FileSystemCacheProvider(connection=connection)
+        with pytest.raises(KeyError) as error_info:
+            provider.get("not_in_cache")
+
+    def test_file_system_cache_provider_sets_then_gets_to_file(self):
+        provider = FileSystemCacheProvider()
+        provider.set("test_key1", "test_value1")
+        provider.set("test_key2", "test_value2")
+        provider.set("test_key1", "test_value3")
+
+        assert provider.get("test_key1") == "test_value3"
+        assert provider.get("test_key2") == "test_value2"
+
+    def test_file_system_cache_provider_does_not_close_supplied_connection(self):
+        connection = Mock(spec_set=Connection)
+        path = f"memento_cache/{hashlib.sha256(b'key').hexdigest()}.pkl"
+        with open(path, "wb") as test_file:
+            cloudpickle.dump("value", test_file)
+        connection.execute().fetchall.return_value = [[path]]
+        provider = FileSystemCacheProvider(connection=connection)
+
+        provider.set("key", "value")
+        provider.get("key")
+        provider.make_key(lambda x: x + 1, 1)
+
+        del provider
+
+        connection.close.assert_not_called()
+
+    @pytest.mark.slow
+    def test_file_system_cache_provider_works_in_parallel(self):
+        provider = FileSystemCacheProvider()
+
+        def underlying_func(a, b):
+            return a + b
+
+        cached_func = Cache(underlying_func, cache_provider=provider)
+
+        manager = TaskManager()
+        for x in range(10):
+            manager.add_task(delayed(cached_func)(1, 1))
+
+        res = manager.run()
+
+        assert res == [2] * 10
```

### Comparing `memento-ml-1.0.2/tests/test_configurations.py` & `memento-ml-1.1.0/tests/test_configurations.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,89 +1,89 @@
-from memento.configurations import generate_configurations
-
-
-def test_configurations_no_exclude():
-    matrix = {
-        "parameters": {"param1": [1, 2], "param2": [3, 4]},
-    }
-
-    configs = generate_configurations(matrix)
-    expected = [
-        {"param1": 1, "param2": 3},
-        {"param1": 1, "param2": 4},
-        {"param1": 2, "param2": 3},
-        {"param1": 2, "param2": 4},
-    ]
-
-    assert len(configs) == len(expected)
-
-    for config, expected in zip(configs, expected):
-        assert config.asdict() == expected
-
-
-def test_configurations():
-    matrix = {
-        "parameters": {"param1": [1, 2, 3], "param2": [4, 5, 6]},
-        "exclude": [{"param1": 3, "param2": 6}],
-    }
-
-    configs = generate_configurations(matrix)
-    expected = [
-        {"param1": 1, "param2": 4},
-        {"param1": 1, "param2": 5},
-        {"param1": 1, "param2": 6},
-        {"param1": 2, "param2": 4},
-        {"param1": 2, "param2": 5},
-        {"param1": 2, "param2": 6},
-        {"param1": 3, "param2": 4},
-        {"param1": 3, "param2": 5},
-        # Excluded
-        # {"param1": 3, "param2": 6},
-    ]
-
-    assert len(configs) == len(expected)
-
-    for config, expected in zip(configs, expected):
-        assert config.asdict() == expected
-
-
-def test_configurations_multi_steps():
-    matrix = {
-        "parameters": {
-            "param1": [1, 2, 3],
-            "param2": [4, 5, 6],
-            "param3": [7, 8],
-        },
-        "exclude": [{"param1": 3, "param2": 5}],
-    }
-
-    configs = generate_configurations(matrix)
-    expected = [
-        {"param1": 1, "param2": 4, "param3": 7},
-        {"param1": 1, "param2": 4, "param3": 8},
-        {"param1": 1, "param2": 5, "param3": 7},
-        {"param1": 1, "param2": 5, "param3": 8},
-        {"param1": 1, "param2": 6, "param3": 7},
-        {"param1": 1, "param2": 6, "param3": 8},
-        {"param1": 2, "param2": 4, "param3": 7},
-        {"param1": 2, "param2": 4, "param3": 8},
-        {"param1": 2, "param2": 5, "param3": 7},
-        {"param1": 2, "param2": 5, "param3": 8},
-        {"param1": 2, "param2": 6, "param3": 7},
-        {"param1": 2, "param2": 6, "param3": 8},
-        {"param1": 3, "param2": 4, "param3": 7},
-        {"param1": 3, "param2": 4, "param3": 8},
-        {"param1": 3, "param2": 6, "param3": 7},
-        {"param1": 3, "param2": 6, "param3": 8},
-        # Excluded
-        # {"param1": 3, "param2": 5, "param3": 7},
-        # {"param1": 3, "param2": 5, "param3": 8},
-    ]
-
-    assert len(configs) == len(expected)
-
-    for config, expected in zip(configs, expected):
-        assert config.asdict() == expected
-
-
-if __name__ == "__main__":
-    test_configurations()
+from memento.configurations import generate_configurations
+
+
+def test_configurations_no_exclude():
+    matrix = {
+        "parameters": {"param1": [1, 2], "param2": [3, 4]},
+    }
+
+    configs = generate_configurations(matrix)
+    expected = [
+        {"param1": 1, "param2": 3},
+        {"param1": 1, "param2": 4},
+        {"param1": 2, "param2": 3},
+        {"param1": 2, "param2": 4},
+    ]
+
+    assert len(configs) == len(expected)
+
+    for config, expected in zip(configs, expected):
+        assert config.asdict() == expected
+
+
+def test_configurations():
+    matrix = {
+        "parameters": {"param1": [1, 2, 3], "param2": [4, 5, 6]},
+        "exclude": [{"param1": 3, "param2": 6}],
+    }
+
+    configs = generate_configurations(matrix)
+    expected = [
+        {"param1": 1, "param2": 4},
+        {"param1": 1, "param2": 5},
+        {"param1": 1, "param2": 6},
+        {"param1": 2, "param2": 4},
+        {"param1": 2, "param2": 5},
+        {"param1": 2, "param2": 6},
+        {"param1": 3, "param2": 4},
+        {"param1": 3, "param2": 5},
+        # Excluded
+        # {"param1": 3, "param2": 6},
+    ]
+
+    assert len(configs) == len(expected)
+
+    for config, expected in zip(configs, expected):
+        assert config.asdict() == expected
+
+
+def test_configurations_multi_steps():
+    matrix = {
+        "parameters": {
+            "param1": [1, 2, 3],
+            "param2": [4, 5, 6],
+            "param3": [7, 8],
+        },
+        "exclude": [{"param1": 3, "param2": 5}],
+    }
+
+    configs = generate_configurations(matrix)
+    expected = [
+        {"param1": 1, "param2": 4, "param3": 7},
+        {"param1": 1, "param2": 4, "param3": 8},
+        {"param1": 1, "param2": 5, "param3": 7},
+        {"param1": 1, "param2": 5, "param3": 8},
+        {"param1": 1, "param2": 6, "param3": 7},
+        {"param1": 1, "param2": 6, "param3": 8},
+        {"param1": 2, "param2": 4, "param3": 7},
+        {"param1": 2, "param2": 4, "param3": 8},
+        {"param1": 2, "param2": 5, "param3": 7},
+        {"param1": 2, "param2": 5, "param3": 8},
+        {"param1": 2, "param2": 6, "param3": 7},
+        {"param1": 2, "param2": 6, "param3": 8},
+        {"param1": 3, "param2": 4, "param3": 7},
+        {"param1": 3, "param2": 4, "param3": 8},
+        {"param1": 3, "param2": 6, "param3": 7},
+        {"param1": 3, "param2": 6, "param3": 8},
+        # Excluded
+        # {"param1": 3, "param2": 5, "param3": 7},
+        # {"param1": 3, "param2": 5, "param3": 8},
+    ]
+
+    assert len(configs) == len(expected)
+
+    for config, expected in zip(configs, expected):
+        assert config.asdict() == expected
+
+
+if __name__ == "__main__":
+    test_configurations()
```

### Comparing `memento-ml-1.0.2/tests/test_memento.py` & `memento-ml-1.1.0/tests/test_memento.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,16 +26,19 @@
         # This is ugly, but sqlite3 doesn't seem to accept a file handle directly, so we need to
         # create a temporary file, close it (to not run afoul of locking on windows), then manually
         # remove it after we're done.
         self._cache_filepath = _create_file("_memento.cache")
         self._notification_filepath = _create_file("_memento.notifications")
 
     def teardown_method(self, method):
-        os.unlink(self._cache_filepath)
-        os.unlink(self._notification_filepath)
+        try:
+            os.unlink(self._cache_filepath)
+            os.unlink(self._notification_filepath)
+        except PermissionError:
+            pass
 
     @pytest.mark.slow
     def test_memento(self):
         def func(context, config):
             return config.k1
 
         memento = Memento(func)
```

### Comparing `memento-ml-1.0.2/tests/test_notifications.py` & `memento-ml-1.1.0/tests/test_notifications.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,193 +1,193 @@
-import email
-import smtplib
-from email.utils import parseaddr
-from io import StringIO
-from typing import List
-from unittest.mock import Mock
-
-import pytest
-from aiosmtpd import controller, handlers
-
-from memento.notifications import (
-    FileSystemNotificationProvider,
-    EmailNotificationProvider,
-    SmtpConfiguration,
-)
-from memento.parallel import TaskManager, delayed
-
-
-class TestFileSystemNotificationProvider:
-    def setup_method(self):
-        self.file = StringIO()
-        self.provider = FileSystemNotificationProvider(filepath=self.file)
-
-    def test_writes_to_file_on_job_completed(self):
-        self.provider.task_completed()
-        assert self.file.getvalue() == "Task completed\n"
-
-    def test_writes_to_file_on_all_tasks_completed(self):
-        self.provider.all_tasks_completed()
-        assert self.file.getvalue() == "All tasks completed\n"
-
-    def test_writes_to_file_on_task_failure(self):
-        self.provider.task_failure()
-        assert self.file.getvalue() == "Task failed\n"
-
-
-class Handler(handlers.Message):
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        self._messages: List[email.message.Message] = []
-
-    def handle_message(self, message):
-        self._messages.append(message)
-        print("<<< START MESSAGE >>>")
-        print(message)
-        print("<<< END MESSAGE >>>")
-
-    @property
-    def messages(self):
-        """Returns the messages processed by this handler."""
-        return self._messages
-
-
-class DummySmtpServer:
-    """Dummy SMTP server that saves emails to a list. Primarily for testing/debugging."""
-
-    def __init__(self):
-        self._messages = []
-        self._handler = Handler()
-        self._controller = controller.Controller(self._handler)
-
-    def __enter__(self):
-        self._controller.start()
-
-    def __exit__(self, exc_type, exc_val, exc_tb):
-        self._controller.stop()
-
-    @property
-    def messages(self):
-        """List of messages in the order they were received by this server."""
-        return self._handler.messages
-
-    @property
-    def host(self):
-        """
-        This server's hostname.
-        """
-        return self._controller.hostname
-
-    @property
-    def port(self):
-        """
-        Port this server is accessible from.
-        """
-        return self._controller.port
-
-    def start(self):
-        """Starts this server."""
-        self._controller.start()
-
-    def stop(self):
-        """Stops this server."""
-        self._controller.stop()
-
-
-@pytest.mark.parametrize(
-    "to_addrs",
-    [
-        ["receiver@test.com"],
-        ["receiver1@test.com", "receiver2@test.com"],
-    ],
-)
-class TestEmailNotificationProvider:
-    def setup_provider(self, to_addrs: List[str]):
-        self.messages: List[email.message.Message] = []
-        self.client = Mock(spec_set=smtplib.SMTP)
-        self.client.send_message.side_effect = self.messages.append
-        self.from_addr = "sender@text.com"
-        self.to_addrs = to_addrs
-        self.provider = EmailNotificationProvider(
-            self.client, self.from_addr, self.to_addrs
-        )
-
-    def _check_message(
-        self, message: email.message.Message, subject: str, payload: str
-    ):
-        """
-        Checks a message is being sent from and delivered to the right person as well as that it
-        contains the correct information.
-        """
-        assert parseaddr(message["from"])[1] == self.from_addr
-        assert message["to"] == ", ".join(self.to_addrs)
-        assert message["subject"] == subject
-        assert message.get_payload().strip() == payload
-
-    def _check_messages(self, subject, payload):
-        messages = self.messages
-        assert len(messages) == 1
-        self._check_message(messages[0], subject, payload)
-
-    def test_sends_email_on_task_completed(self, to_addrs):
-        self.setup_provider(to_addrs)
-        self.provider.task_completed()
-        subject = "[Memento] Task completed"
-        payload = "Task completed"
-        self._check_messages(subject, payload)
-
-    def test_sends_email_on_all_tasks_completed(self, to_addrs):
-        self.setup_provider(to_addrs)
-        self.provider.all_tasks_completed()
-        subject = "[Memento] All tasks completed"
-        payload = "All tasks completed"
-        self._check_messages(subject, payload)
-
-    def test_sends_email_on_task_failure(self, to_addrs):
-        self.setup_provider(to_addrs)
-        self.provider.task_failure()
-        subject = "[Memento] Task failed"
-        payload = "Task failed"
-        self._check_messages(subject, payload)
-
-
-@pytest.mark.slow
-class TestEmailNotificationProviderWithServer:
-    """Tests to verify that emails are delivered to the SMTP server."""
-
-    def setup_method(self):
-        self.server = DummySmtpServer()
-        self.server.start()
-
-        self.from_addr = "sender@text.com"
-        self.to_addrs = ["receiver@test.com"]
-
-        smtp_config = SmtpConfiguration(
-            self.server.host, self.server.port, require_tls=False
-        )
-
-        self.provider = EmailNotificationProvider(
-            smtp_config, self.from_addr, self.to_addrs
-        )
-
-    def teardown_method(self):
-        self.server.stop()
-
-    def test_sends_email_to_server_on_task_completed(self):
-        self.provider.task_completed()
-        assert len(self.server.messages) == 1
-
-    def test_sends_email_to_server_on_all_tasks_completed(self):
-        self.provider.all_tasks_completed()
-        assert len(self.server.messages) == 1
-
-    def test_sends_email_to_server_on_task_failure(self):
-        self.provider.task_failure()
-        assert len(self.server.messages) == 1
-
-    def test_sends_emails_in_parallel(self):
-        manager = TaskManager(
-            notification_provider=self.provider, notify_on_complete=True
-        )
-        manager.add_task(delayed(lambda x: print(x))("Hello World!"))
-        manager.run()
-        assert len(self.server.messages) == 2
+import email
+import smtplib
+from email.utils import parseaddr
+from io import StringIO
+from typing import List
+from unittest.mock import Mock
+
+import pytest
+from aiosmtpd import controller, handlers
+
+from memento.notifications import (
+    FileSystemNotificationProvider,
+    EmailNotificationProvider,
+    SmtpConfiguration,
+)
+from memento.parallel import TaskManager, delayed
+
+
+class TestFileSystemNotificationProvider:
+    def setup_method(self):
+        self.file = StringIO()
+        self.provider = FileSystemNotificationProvider(filepath=self.file)
+
+    def test_writes_to_file_on_job_completed(self):
+        self.provider.task_completed()
+        assert self.file.getvalue() == "Task completed\n"
+
+    def test_writes_to_file_on_all_tasks_completed(self):
+        self.provider.all_tasks_completed()
+        assert self.file.getvalue() == "All tasks completed\n"
+
+    def test_writes_to_file_on_task_failure(self):
+        self.provider.task_failure()
+        assert self.file.getvalue() == "Task failed\n"
+
+
+class Handler(handlers.Message):
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self._messages: List[email.message.Message] = []
+
+    def handle_message(self, message):
+        self._messages.append(message)
+        print("<<< START MESSAGE >>>")
+        print(message)
+        print("<<< END MESSAGE >>>")
+
+    @property
+    def messages(self):
+        """Returns the messages processed by this handler."""
+        return self._messages
+
+
+class DummySmtpServer:
+    """Dummy SMTP server that saves emails to a list. Primarily for testing/debugging."""
+
+    def __init__(self):
+        self._messages = []
+        self._handler = Handler()
+        self._controller = controller.Controller(self._handler)
+
+    def __enter__(self):
+        self._controller.start()
+
+    def __exit__(self, exc_type, exc_val, exc_tb):
+        self._controller.stop()
+
+    @property
+    def messages(self):
+        """List of messages in the order they were received by this server."""
+        return self._handler.messages
+
+    @property
+    def host(self):
+        """
+        This server's hostname.
+        """
+        return self._controller.hostname
+
+    @property
+    def port(self):
+        """
+        Port this server is accessible from.
+        """
+        return self._controller.port
+
+    def start(self):
+        """Starts this server."""
+        self._controller.start()
+
+    def stop(self):
+        """Stops this server."""
+        self._controller.stop()
+
+
+@pytest.mark.parametrize(
+    "to_addrs",
+    [
+        ["receiver@test.com"],
+        ["receiver1@test.com", "receiver2@test.com"],
+    ],
+)
+class TestEmailNotificationProvider:
+    def setup_provider(self, to_addrs: List[str]):
+        self.messages: List[email.message.Message] = []
+        self.client = Mock(spec_set=smtplib.SMTP)
+        self.client.send_message.side_effect = self.messages.append
+        self.from_addr = "sender@text.com"
+        self.to_addrs = to_addrs
+        self.provider = EmailNotificationProvider(
+            self.client, self.from_addr, self.to_addrs
+        )
+
+    def _check_message(
+        self, message: email.message.Message, subject: str, payload: str
+    ):
+        """
+        Checks a message is being sent from and delivered to the right person as well as that it
+        contains the correct information.
+        """
+        assert parseaddr(message["from"])[1] == self.from_addr
+        assert message["to"] == ", ".join(self.to_addrs)
+        assert message["subject"] == subject
+        assert message.get_payload().strip() == payload
+
+    def _check_messages(self, subject, payload):
+        messages = self.messages
+        assert len(messages) == 1
+        self._check_message(messages[0], subject, payload)
+
+    def test_sends_email_on_task_completed(self, to_addrs):
+        self.setup_provider(to_addrs)
+        self.provider.task_completed()
+        subject = "[Memento] Task completed"
+        payload = "Task completed"
+        self._check_messages(subject, payload)
+
+    def test_sends_email_on_all_tasks_completed(self, to_addrs):
+        self.setup_provider(to_addrs)
+        self.provider.all_tasks_completed()
+        subject = "[Memento] All tasks completed"
+        payload = "All tasks completed"
+        self._check_messages(subject, payload)
+
+    def test_sends_email_on_task_failure(self, to_addrs):
+        self.setup_provider(to_addrs)
+        self.provider.task_failure()
+        subject = "[Memento] Task failed"
+        payload = "Task failed"
+        self._check_messages(subject, payload)
+
+
+@pytest.mark.slow
+class TestEmailNotificationProviderWithServer:
+    """Tests to verify that emails are delivered to the SMTP server."""
+
+    def setup_method(self):
+        self.server = DummySmtpServer()
+        self.server.start()
+
+        self.from_addr = "sender@text.com"
+        self.to_addrs = ["receiver@test.com"]
+
+        smtp_config = SmtpConfiguration(
+            self.server.host, self.server.port, require_tls=False
+        )
+
+        self.provider = EmailNotificationProvider(
+            smtp_config, self.from_addr, self.to_addrs
+        )
+
+    def teardown_method(self):
+        self.server.stop()
+
+    def test_sends_email_to_server_on_task_completed(self):
+        self.provider.task_completed()
+        assert len(self.server.messages) == 1
+
+    def test_sends_email_to_server_on_all_tasks_completed(self):
+        self.provider.all_tasks_completed()
+        assert len(self.server.messages) == 1
+
+    def test_sends_email_to_server_on_task_failure(self):
+        self.provider.task_failure()
+        assert len(self.server.messages) == 1
+
+    def test_sends_emails_in_parallel(self):
+        manager = TaskManager(
+            notification_provider=self.provider, notify_on_complete=True
+        )
+        manager.add_task(delayed(lambda x: print(x))("Hello World!"))
+        manager.run()
+        assert len(self.server.messages) == 2
```

### Comparing `memento-ml-1.0.2/tests/test_parallel.py` & `memento-ml-1.1.0/tests/test_parallel.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,128 +1,128 @@
-"""
-Contains tests for parallel.py.
-"""
-
-import functools
-import multiprocessing
-import os
-import time
-from typing import List, Callable, TextIO
-
-import pytest
-
-from memento.parallel import TaskManager, delayed
-
-BASE_PATH = os.path.abspath(os.path.dirname(__file__))
-INPUT_PATH = os.path.join(BASE_PATH, "data", "hello_world.txt")
-
-
-def get_process_id():
-    return id(multiprocessing.current_process())
-
-
-class DummyClass:
-    def __init__(self, x: int, y: int):
-        self._result = x + y
-
-    def calculate(self):
-        return self._result
-
-    def __eq__(self, other):
-        return isinstance(other, DummyClass) and self._result == other._result
-
-
-class CallableDummyClass:
-    def __call__(self, x: int, y: int):
-        return x + y
-
-
-def recursive_function(x: int):
-    if x <= 0:
-        return 0
-    return 1 + recursive_function(x - 1)
-
-
-def function_with_dependencies(x: int, y: int):
-    time.sleep(0)
-    return x + y
-
-
-def function_referencing_locals(x: int, y: int):
-    return function_with_dependencies(x, y)
-
-
-def function_with_local_import(x: int, y: int):
-    import math
-
-    return math.floor(x + y)
-
-
-def read_file(file: TextIO):
-    return file.readlines()
-
-
-@pytest.mark.slow
-class TestParallel:
-    def test_parallel_uses_multiple_processes(self):
-        """Multiple processes are used when running tasks."""
-        manager = TaskManager(max_tasks_per_worker=1)
-        manager.add_tasks((delayed(get_process_id)() for _ in range(10)))
-        results = manager.run()
-
-        assert len(set(results)) > 0
-
-    # The current method used to spawn processes doesn't give precise control over how many are
-    # spawned so this test has been skipped (for now)
-    @pytest.mark.skip
-    def test_parallel_uses_correct_number_of_processes(self):
-        """Multiple processes are used up to the specified limit when possible."""
-        manager = TaskManager(max_tasks_per_worker=2, workers=5)
-        manager.add_tasks((delayed(get_process_id)() for _ in range(10)))
-        results = manager.run()
-
-        assert len(set(results)) <= 5
-
-    @pytest.mark.parametrize(
-        "task,expected",
-        [
-            (delayed(sum)([1, 2]), [3]),
-            (delayed(lambda x: sum(x))([2, 2]), [4]),
-            (delayed(functools.partial(lambda x, y: sum([x, y]), 2))(3), [5]),
-            (delayed(DummyClass)(3, 3), [DummyClass(3, 3)]),
-            (delayed(DummyClass(3, 3).calculate)(), [6]),
-            (delayed(CallableDummyClass())(3, 4), [7]),
-            (delayed(recursive_function)(8), [8]),
-            (delayed(function_with_dependencies)(4, 5), [9]),
-            (delayed(function_referencing_locals)(5, 5), [10]),
-            (delayed(function_with_local_import)(5, 6), [11]),
-            (delayed(list)(range(5)), [[0, 1, 2, 3, 4]]),
-        ],
-    )
-    def test_parallel_returns_correct_result(self, task: Callable, expected: List):
-        """The correct result is returned when tasks are run."""
-        manager = TaskManager()
-        manager.add_task(task)
-        results = manager.run()
-
-        assert results == expected
-
-    def test_parallel_order(self):
-        manager = TaskManager()
-
-        def identity(x):
-            return x
-
-        manager.add_tasks(delayed(identity)(x) for x in range(10))
-
-        results = manager.run()
-
-        assert results == list(range(10))
-
-    def test_parallel_with_file(self):
-        manager = TaskManager()
-
-        with open(INPUT_PATH) as f:
-            manager.add_task(delayed(read_file)(f))
-
-        results = manager.run()
-        assert results == [["Hello World!\n"]]
+"""
+Contains tests for parallel.py.
+"""
+
+import functools
+import multiprocessing
+import os
+import time
+from typing import List, Callable, TextIO
+
+import pytest
+
+from memento.parallel import TaskManager, delayed
+
+BASE_PATH = os.path.abspath(os.path.dirname(__file__))
+INPUT_PATH = os.path.join(BASE_PATH, "data", "hello_world.txt")
+
+
+def get_process_id():
+    return id(multiprocessing.current_process())
+
+
+class DummyClass:
+    def __init__(self, x: int, y: int):
+        self._result = x + y
+
+    def calculate(self):
+        return self._result
+
+    def __eq__(self, other):
+        return isinstance(other, DummyClass) and self._result == other._result
+
+
+class CallableDummyClass:
+    def __call__(self, x: int, y: int):
+        return x + y
+
+
+def recursive_function(x: int):
+    if x <= 0:
+        return 0
+    return 1 + recursive_function(x - 1)
+
+
+def function_with_dependencies(x: int, y: int):
+    time.sleep(0)
+    return x + y
+
+
+def function_referencing_locals(x: int, y: int):
+    return function_with_dependencies(x, y)
+
+
+def function_with_local_import(x: int, y: int):
+    import math
+
+    return math.floor(x + y)
+
+
+def read_file(file: TextIO):
+    return file.readlines()
+
+
+@pytest.mark.slow
+class TestParallel:
+    def test_parallel_uses_multiple_processes(self):
+        """Multiple processes are used when running tasks."""
+        manager = TaskManager(max_tasks_per_worker=1)
+        manager.add_tasks((delayed(get_process_id)() for _ in range(10)))
+        results = manager.run()
+
+        assert len(set(results)) > 0
+
+    # The current method used to spawn processes doesn't give precise control over how many are
+    # spawned so this test has been skipped (for now)
+    @pytest.mark.skip
+    def test_parallel_uses_correct_number_of_processes(self):
+        """Multiple processes are used up to the specified limit when possible."""
+        manager = TaskManager(max_tasks_per_worker=2, workers=5)
+        manager.add_tasks((delayed(get_process_id)() for _ in range(10)))
+        results = manager.run()
+
+        assert len(set(results)) <= 5
+
+    @pytest.mark.parametrize(
+        "task,expected",
+        [
+            (delayed(sum)([1, 2]), [3]),
+            (delayed(lambda x: sum(x))([2, 2]), [4]),
+            (delayed(functools.partial(lambda x, y: sum([x, y]), 2))(3), [5]),
+            (delayed(DummyClass)(3, 3), [DummyClass(3, 3)]),
+            (delayed(DummyClass(3, 3).calculate)(), [6]),
+            (delayed(CallableDummyClass())(3, 4), [7]),
+            (delayed(recursive_function)(8), [8]),
+            (delayed(function_with_dependencies)(4, 5), [9]),
+            (delayed(function_referencing_locals)(5, 5), [10]),
+            (delayed(function_with_local_import)(5, 6), [11]),
+            (delayed(lambda x: list(x))(range(5)), [[0, 1, 2, 3, 4]]),
+        ],
+    )
+    def test_parallel_returns_correct_result(self, task: Callable, expected: List):
+        """The correct result is returned when tasks are run."""
+        manager = TaskManager()
+        manager.add_task(task)
+        results = manager.run()
+
+        assert results == expected
+
+    def test_parallel_order(self):
+        manager = TaskManager()
+
+        def identity(x):
+            return x
+
+        manager.add_tasks(delayed(identity)(x) for x in range(10))
+
+        results = manager.run()
+
+        assert results == list(range(10))
+
+    def test_parallel_with_file(self):
+        manager = TaskManager()
+
+        with open(INPUT_PATH) as f:
+            manager.add_task(delayed(read_file)(f))
+
+        results = manager.run()
+        assert results == [["Hello World!\n"]]
```

### Comparing `memento-ml-1.0.2/tests/test_task_interface.py` & `memento-ml-1.1.0/tests/test_task_interface.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,166 +1,168 @@
-import time
-from sqlite3 import Connection
-from unittest.mock import Mock
-import pytest
-from memento.task_interface import Context, FileSystemCheckpointing
-import os
-import tempfile
-import cloudpickle
-
-
-def constant_key_provider(
-    *args, **kwargs
-):  # Necessary to ensure that mocks are not pickled
-    return "key"
-
-
-def arbitrary_expensive_thing(x):
-    return x
-
-
-def arbitrary_expensive_thing2(x):
-    return x + 1
-
-
-class TestContext:
-    class TestRecord:
-        def test_record_records_single_value(self):
-            context = Context("key", FileSystemCheckpointing())
-            context.record({"name": 1.0})
-            context.record({"name": 2.0})
-
-            metrics = context.collect_metrics()
-
-            assert metrics.__contains__("name")
-
-            expected_y_values = [1.0, 2.0]
-            actual_y_values = list(metrics["name"]["y"])
-
-            assert expected_y_values == actual_y_values
-
-        def test_record_records_multiple_values_at_same_timestamp(self):
-            context = Context("key", FileSystemCheckpointing())
-            context.record(value_dict={"name1": 1.0, "name2": 2.0})
-
-            metrics = context.collect_metrics()
-
-            assert metrics.__contains__("name1")
-            assert metrics.__contains__("name2")
-
-            expected_y_values_1 = [1.0]
-            actual_y_values_1 = list(metrics["name1"]["y"])
-            expected_y_values_2 = [2.0]
-            actual_y_values_2 = list(metrics["name2"]["y"])
-            x_values_1 = list(metrics["name1"]["x"])
-            x_values_2 = list(metrics["name2"]["x"])
-
-            assert expected_y_values_1 == actual_y_values_1
-            assert expected_y_values_2 == actual_y_values_2
-            assert x_values_1 == x_values_2
-
-        def test_record_records_multiple_values_at_different_timestamps(self):
-            context = Context("key", FileSystemCheckpointing())
-            context.record({"name1": 1.0})
-            time.sleep(0.001)
-            context.record({"name2": 2.0})
-
-            metrics = context.collect_metrics()
-
-            assert metrics.__contains__("name1")
-            assert metrics.__contains__("name2")
-
-            expected_y_values_1 = [1.0]
-            actual_y_values_1 = list(metrics["name1"]["y"])
-            expected_y_values_2 = [2.0]
-            actual_y_values_2 = list(metrics["name2"]["y"])
-            x_values_1 = list(metrics["name1"]["x"])
-            x_values_2 = list(metrics["name2"]["x"])
-
-            assert expected_y_values_1 == actual_y_values_1
-            assert expected_y_values_2 == actual_y_values_2
-            assert x_values_1 != x_values_2
-
-        def test_record_records_x_and_y_when_given_a_tuple(self):
-            context = Context("key", FileSystemCheckpointing())
-            context.record({"name1": (1.0, 2.0)})
-
-            metrics = context.collect_metrics()
-
-            assert metrics.__contains__("name1")
-
-            expected_y_values = [2.0]
-            actual_y_values = list(metrics["name1"]["y"])
-            expected_x_values = [1.0]
-            actual_x_values = list(metrics["name1"]["x"])
-
-            assert expected_y_values == actual_y_values
-            assert expected_x_values == actual_x_values
-
-    class TestCheckpoint:
-        def setup_method(self, method):
-            file = tempfile.NamedTemporaryFile(
-                suffix="_memento.checkpoint", delete=False
-            )
-            self._filepath = os.path.abspath(file.name)
-            file.close()
-
-        def teardown_method(self, method):
-            os.unlink(self._filepath)
-
-        def test_file_system_checkpoint_provider_checkpoint_works(self):
-            checkpoint_provider = FileSystemCheckpointing()
-            intermediate = arbitrary_expensive_thing(1)
-            context = Context("key", checkpoint_provider)
-
-            context.checkpoint(intermediate)
-
-            assert checkpoint_provider.contains("key")
-
-        def test_file_system_checkpoint_provider_restore_works(self):
-            checkpoint_provider = FileSystemCheckpointing()
-            intermediate = arbitrary_expensive_thing(1)
-            context = Context("key", checkpoint_provider)
-
-            context.checkpoint(intermediate)
-            value = context.restore()
-
-            assert value == 1
-
-        def test_file_system_checkpoint_provider_creates_correct_keys(self):
-            def function(*args):
-                return args
-
-            context_key = "key"
-            arguments = ("test1", "test2", 123, True)
-            keyword_arguments = {
-                "key1": "value1",
-                "key2": "value2",
-                "key3": 321,
-                "key4": False,
-                "context_key": context_key,
-            }
-            expected = cloudpickle.dumps(
-                {
-                    "function": function,
-                    "args": arguments,
-                    "kwargs": keyword_arguments,
-                }
-            )
-
-            connection = Mock(spec_set=Connection)
-            checkpoint_provider = FileSystemCheckpointing(connection=connection)
-            actual = checkpoint_provider.make_key(
-                function, *arguments, **keyword_arguments
-            )
-
-            assert expected == actual
-
-        def test_file_system_checkpoint_provider_get_raises_key_error_when_key_not_in_database(
-            self,
-        ):
-            connection = Mock(spec_set=Connection)
-            connection.execute().fetchall.return_value = None
-            checkpoint_provider = FileSystemCheckpointing(connection=connection)
-
-            with pytest.raises(KeyError) as error_info:
-                checkpoint_provider.get("not_in_checkpoint")
+import time
+from sqlite3 import Connection
+from unittest.mock import Mock
+import pytest
+import os
+import tempfile
+import cloudpickle
+from memento.task_interface import Context, FileSystemCheckpointing
+
+
+
+
+def constant_key_provider(
+    *args, **kwargs
+):  # Necessary to ensure that mocks are not pickled
+    return "key"
+
+
+def arbitrary_expensive_thing(x):
+    return x
+
+
+def arbitrary_expensive_thing2(x):
+    return x + 1
+
+
+class TestContext:
+    class TestRecord:
+        def test_record_records_single_value(self):
+            context = Context("key", FileSystemCheckpointing())
+            context.record({"name": 1.0})
+            context.record({"name": 2.0})
+
+            metrics = context.collect_metrics()
+
+            assert metrics.__contains__("name")
+
+            expected_y_values = [1.0, 2.0]
+            actual_y_values = list(metrics["name"]["y"])
+
+            assert expected_y_values == actual_y_values
+
+        def test_record_records_multiple_values_at_same_timestamp(self):
+            context = Context("key", FileSystemCheckpointing())
+            context.record(value_dict={"name1": 1.0, "name2": 2.0})
+
+            metrics = context.collect_metrics()
+
+            assert metrics.__contains__("name1")
+            assert metrics.__contains__("name2")
+
+            expected_y_values_1 = [1.0]
+            actual_y_values_1 = list(metrics["name1"]["y"])
+            expected_y_values_2 = [2.0]
+            actual_y_values_2 = list(metrics["name2"]["y"])
+            x_values_1 = list(metrics["name1"]["x"])
+            x_values_2 = list(metrics["name2"]["x"])
+
+            assert expected_y_values_1 == actual_y_values_1
+            assert expected_y_values_2 == actual_y_values_2
+            assert x_values_1 == x_values_2
+
+        def test_record_records_multiple_values_at_different_timestamps(self):
+            context = Context("key", FileSystemCheckpointing())
+            context.record({"name1": 1.0})
+            time.sleep(0.001)
+            context.record({"name2": 2.0})
+
+            metrics = context.collect_metrics()
+
+            assert metrics.__contains__("name1")
+            assert metrics.__contains__("name2")
+
+            expected_y_values_1 = [1.0]
+            actual_y_values_1 = list(metrics["name1"]["y"])
+            expected_y_values_2 = [2.0]
+            actual_y_values_2 = list(metrics["name2"]["y"])
+            x_values_1 = list(metrics["name1"]["x"])
+            x_values_2 = list(metrics["name2"]["x"])
+
+            assert expected_y_values_1 == actual_y_values_1
+            assert expected_y_values_2 == actual_y_values_2
+            assert x_values_1 != x_values_2
+
+        def test_record_records_x_and_y_when_given_a_tuple(self):
+            context = Context("key", FileSystemCheckpointing())
+            context.record({"name1": (1.0, 2.0)})
+
+            metrics = context.collect_metrics()
+
+            assert metrics.__contains__("name1")
+
+            expected_y_values = [2.0]
+            actual_y_values = list(metrics["name1"]["y"])
+            expected_x_values = [1.0]
+            actual_x_values = list(metrics["name1"]["x"])
+
+            assert expected_y_values == actual_y_values
+            assert expected_x_values == actual_x_values
+
+    class TestCheckpoint:
+        def setup_method(self, method):
+            file = tempfile.NamedTemporaryFile(
+                suffix="_memento.checkpoint", delete=False
+            )
+            self._filepath = os.path.abspath(file.name)
+            file.close()
+
+        def teardown_method(self, method):
+            os.unlink(self._filepath)
+
+        def test_file_system_checkpoint_provider_checkpoint_works(self):
+            checkpoint_provider = FileSystemCheckpointing()
+            intermediate = arbitrary_expensive_thing(1)
+            context = Context("key", checkpoint_provider)
+
+            context.checkpoint(intermediate)
+
+            assert checkpoint_provider.contains("key")
+
+        def test_file_system_checkpoint_provider_restore_works(self):
+            checkpoint_provider = FileSystemCheckpointing()
+            intermediate = arbitrary_expensive_thing(1)
+            context = Context("key", checkpoint_provider)
+
+            context.checkpoint(intermediate)
+            value = context.restore()
+
+            assert value == 1
+
+        def test_file_system_checkpoint_provider_creates_correct_keys(self):
+            def function(*args):
+                return args
+
+            context_key = "key"
+            arguments = ("test1", "test2", 123, True)
+            keyword_arguments = {
+                "key1": "value1",
+                "key2": "value2",
+                "key3": 321,
+                "key4": False,
+                "context_key": context_key,
+            }
+            expected = cloudpickle.dumps(
+                {
+                    "function": function,
+                    "args": arguments,
+                    "kwargs": keyword_arguments,
+                }
+            )
+
+            connection = Mock(spec_set=Connection)
+            checkpoint_provider = FileSystemCheckpointing(connection=connection)
+            actual = checkpoint_provider.make_key(
+                function, *arguments, **keyword_arguments
+            )
+
+            assert expected == actual
+
+        def test_file_system_checkpoint_provider_get_raises_key_error_when_key_not_in_database(
+            self,
+        ):
+            connection = Mock(spec_set=Connection)
+            connection.execute().fetchall.return_value = None
+            checkpoint_provider = FileSystemCheckpointing(connection=connection)
+
+            with pytest.raises(KeyError) as error_info:
+                checkpoint_provider.get("not_in_checkpoint")
```

