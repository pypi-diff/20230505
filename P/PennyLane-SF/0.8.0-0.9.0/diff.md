# Comparing `tmp/PennyLane-SF-0.8.0.tar.gz` & `tmp/PennyLane-SF-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/PennyLane-SF-0.8.0.tar", last modified: Fri Jan 31 21:31:07 2020, max compression
+gzip compressed data, was "dist/PennyLane-SF-0.9.0.tar", last modified: Fri May 15 03:49:49 2020, max compression
```

## Comparing `PennyLane-SF-0.8.0.tar` & `PennyLane-SF-0.9.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 antal     (1000) antal     (1000)        0 2020-01-31 21:31:07.000000 PennyLane-SF-0.8.0/
--rw-r--r--   0 antal     (1000) antal     (1000)     6525 2020-01-31 21:31:07.000000 PennyLane-SF-0.8.0/PKG-INFO
-drwxr-xr-x   0 antal     (1000) antal     (1000)        0 2020-01-31 21:31:07.000000 PennyLane-SF-0.8.0/PennyLane_SF.egg-info/
--rw-r--r--   0 antal     (1000) antal     (1000)     6525 2020-01-31 21:31:07.000000 PennyLane-SF-0.8.0/PennyLane_SF.egg-info/PKG-INFO
--rw-r--r--   0 antal     (1000) antal     (1000)      388 2020-01-31 21:31:07.000000 PennyLane-SF-0.8.0/PennyLane_SF.egg-info/SOURCES.txt
--rw-r--r--   0 antal     (1000) antal     (1000)        1 2020-01-31 21:31:07.000000 PennyLane-SF-0.8.0/PennyLane_SF.egg-info/dependency_links.txt
--rw-r--r--   0 antal     (1000) antal     (1000)      145 2020-01-31 21:31:07.000000 PennyLane-SF-0.8.0/PennyLane_SF.egg-info/entry_points.txt
--rw-r--r--   0 antal     (1000) antal     (1000)       38 2020-01-31 21:31:07.000000 PennyLane-SF-0.8.0/PennyLane_SF.egg-info/requires.txt
--rw-r--r--   0 antal     (1000) antal     (1000)       13 2020-01-31 21:31:07.000000 PennyLane-SF-0.8.0/PennyLane_SF.egg-info/top_level.txt
--rw-r--r--   0 antal     (1000) antal     (1000)     4586 2020-01-31 21:25:59.000000 PennyLane-SF-0.8.0/README.rst
-drwxr-xr-x   0 antal     (1000) antal     (1000)        0 2020-01-31 21:31:07.000000 PennyLane-SF-0.8.0/pennylane_sf/
--rw-r--r--   0 antal     (1000) antal     (1000)      753 2020-01-31 21:25:59.000000 PennyLane-SF-0.8.0/pennylane_sf/__init__.py
--rw-r--r--   0 antal     (1000) antal     (1000)      691 2020-01-31 21:25:59.000000 PennyLane-SF-0.8.0/pennylane_sf/_version.py
--rw-r--r--   0 antal     (1000) antal     (1000)     6833 2020-01-31 21:25:59.000000 PennyLane-SF-0.8.0/pennylane_sf/expectations.py
--rw-r--r--   0 antal     (1000) antal     (1000)     3746 2020-01-31 21:25:59.000000 PennyLane-SF-0.8.0/pennylane_sf/fock.py
--rw-r--r--   0 antal     (1000) antal     (1000)     3245 2020-01-31 21:25:59.000000 PennyLane-SF-0.8.0/pennylane_sf/gaussian.py
--rw-r--r--   0 antal     (1000) antal     (1000)     5762 2020-01-31 21:25:59.000000 PennyLane-SF-0.8.0/pennylane_sf/simulator.py
--rw-r--r--   0 antal     (1000) antal     (1000)       38 2020-01-31 21:31:07.000000 PennyLane-SF-0.8.0/setup.cfg
--rw-r--r--   0 antal     (1000) antal     (1000)     2551 2020-01-31 21:25:59.000000 PennyLane-SF-0.8.0/setup.py
+drwxr-xr-x   0 antal     (1000) antal     (1000)        0 2020-05-15 03:49:49.000000 PennyLane-SF-0.9.0/
+-rw-r--r--   0 antal     (1000) antal     (1000)     7992 2020-05-15 03:49:49.000000 PennyLane-SF-0.9.0/PKG-INFO
+drwxr-xr-x   0 antal     (1000) antal     (1000)        0 2020-05-15 03:49:49.000000 PennyLane-SF-0.9.0/PennyLane_SF.egg-info/
+-rw-r--r--   0 antal     (1000) antal     (1000)     7992 2020-05-15 03:49:49.000000 PennyLane-SF-0.9.0/PennyLane_SF.egg-info/PKG-INFO
+-rw-r--r--   0 antal     (1000) antal     (1000)      388 2020-05-15 03:49:49.000000 PennyLane-SF-0.9.0/PennyLane_SF.egg-info/SOURCES.txt
+-rw-r--r--   0 antal     (1000) antal     (1000)        1 2020-05-15 03:49:49.000000 PennyLane-SF-0.9.0/PennyLane_SF.egg-info/dependency_links.txt
+-rw-r--r--   0 antal     (1000) antal     (1000)      145 2020-05-15 03:49:49.000000 PennyLane-SF-0.9.0/PennyLane_SF.egg-info/entry_points.txt
+-rw-r--r--   0 antal     (1000) antal     (1000)       40 2020-05-15 03:49:49.000000 PennyLane-SF-0.9.0/PennyLane_SF.egg-info/requires.txt
+-rw-r--r--   0 antal     (1000) antal     (1000)       13 2020-05-15 03:49:49.000000 PennyLane-SF-0.9.0/PennyLane_SF.egg-info/top_level.txt
+-rw-r--r--   0 antal     (1000) antal     (1000)     5619 2020-05-15 03:44:35.000000 PennyLane-SF-0.9.0/README.rst
+drwxr-xr-x   0 antal     (1000) antal     (1000)        0 2020-05-15 03:49:49.000000 PennyLane-SF-0.9.0/pennylane_sf/
+-rw-r--r--   0 antal     (1000) antal     (1000)      757 2020-05-12 14:30:43.000000 PennyLane-SF-0.9.0/pennylane_sf/__init__.py
+-rw-r--r--   0 antal     (1000) antal     (1000)      696 2020-05-14 16:04:41.000000 PennyLane-SF-0.9.0/pennylane_sf/_version.py
+-rw-r--r--   0 antal     (1000) antal     (1000)     6838 2020-05-12 14:30:43.000000 PennyLane-SF-0.9.0/pennylane_sf/expectations.py
+-rw-r--r--   0 antal     (1000) antal     (1000)     3751 2020-05-12 14:30:43.000000 PennyLane-SF-0.9.0/pennylane_sf/fock.py
+-rw-r--r--   0 antal     (1000) antal     (1000)     3250 2020-05-12 14:30:43.000000 PennyLane-SF-0.9.0/pennylane_sf/gaussian.py
+-rw-r--r--   0 antal     (1000) antal     (1000)     5767 2020-05-12 14:30:43.000000 PennyLane-SF-0.9.0/pennylane_sf/simulator.py
+-rw-r--r--   0 antal     (1000) antal     (1000)       38 2020-05-15 03:49:49.000000 PennyLane-SF-0.9.0/setup.cfg
+-rw-r--r--   0 antal     (1000) antal     (1000)     2604 2020-05-15 03:14:50.000000 PennyLane-SF-0.9.0/setup.py
```

### Comparing `PennyLane-SF-0.8.0/PKG-INFO` & `PennyLane-SF-0.9.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: PennyLane-SF
-Version: 0.8.0
+Version: 0.9.0
 Summary: Open source library for continuous-variable quantum computation
 Home-page: https://github.com/XanaduAI/pennylane-sf
 Maintainer: Xanadu Inc.
 Maintainer-email: nathan@xanadu.ai
 License: Apache License 2.0
 Description: PennyLane Strawberry Fields Plugin
         ##################################
@@ -29,110 +29,159 @@
             :alt: PyPI
             :target: https://pypi.org/project/PennyLane-SF
         
         .. image:: https://img.shields.io/pypi/pyversions/PennyLane-SF.svg?style=for-the-badge
             :alt: PyPI - Python Version
             :target: https://pypi.org/project/PennyLane-SF
         
+        .. header-start-inclusion-marker-do-not-remove
         
-        This PennyLane plugin allows the Strawberry Fields simulators to be used as PennyLane devices.
         
-        `Strawberry Fields <https://strawberryfields.readthedocs.io>`_ is a full-stack Python library for designing, simulating, and optimizing continuous variable (CV) quantum optical circuits.
+        The PennyLane-SF plugin integrates the StrawberryFields photonic quantum computing framework with PennyLane's
+        quantum machine learning capabilities.
         
-        `PennyLane <https://pennylane.readthedocs.io>`_ is a machine learning library for optimization and automatic differentiation of hybrid quantum-classical computations.
+        `PennyLane <https://pennylane.readthedocs.io>`__ is a machine learning library for optimization and
+        automatic differentiation of hybrid quantum-classical computations.
+        
+        `Strawberry Fields <https://strawberryfields.readthedocs.io>`__ is a full-stack Python library
+        for designing, simulating, and optimizing photonic quantum circuits.
+        
+        .. header-end-inclusion-marker-do-not-remove
+        
+        The plugin documentation can be found here: `PennyLane-Strawberry Fields <https://pennylane-sf.readthedocs.io/en/latest/>`__.
         
         
         Features
         ========
         
         * Provides two devices to be used with PennyLane: ``strawberryfields.fock`` and ``strawberryfields.gaussian``. These provide access to the Strawberry Fields Fock and Gaussian backends respectively.
         
         * Supports all core PennyLane operations and observables across the two devices.
         
         * Combine Strawberry Fields optimized simulator suite with PennyLane's automatic differentiation and optimization.
         
+        .. installation-start-inclusion-marker-do-not-remove
         
         Installation
         ============
         
-        PennyLane-SF requires both PennyLane and Strawberry Fields. It can be installed via ``pip``:
+        Installation of PennyLane-SF, as well as all required Python packages, can be installed via ``pip``:
+        ::
+        
+           	$ python -m pip install pennylane-sf
+        
+        
+        Make sure you are using the Python 3 version of pip.
+        
+        Alternatively, you can install PennyLane-SF from the source code by navigating to the top directory and running
+        ::
+        
+        	$ python setup.py install
         
-        .. code-block:: bash
+        Dependencies
+        ~~~~~~~~~~~~
         
-            $ python -m pip install pennylane-sf
+        PennyLane-SF requires the following libraries be installed:
         
+        * `Python <http://python.org/>`__ >=3.6
         
-        Getting started
-        ===============
+        as well as the following Python packages:
         
-        Once the PennyLane-SF plugin is installed, the two provided Strawberry Fields devices can be accessed straight away in PennyLane.
+        * `PennyLane <http://pennylane.readthedocs.io/>`__ >=0.7
+        * `StrawberryFields <https://strawberryfields.readthedocs.io/>`__ >=0.11.2
         
-        You can instantiate these devices for PennyLane as follows:
         
-        .. code-block:: python
+        If you currently do not have Python 3 installed,
+        we recommend `Anaconda for Python 3 <https://www.anaconda.com/download/>`__, a distributed
+        version of Python packaged for scientific computation.
         
-            import pennylane as qml
-            dev_fock = qml.device('strawberryfields.fock', wires=2, cutoff_dim=10)
-            dev_gaussian = qml.device('strawberryfields.gaussian', wires=2)
+        Software tests
+        ~~~~~~~~~~~~~~
         
-        These devices can then be used just like other devices for the definition and evaluation of QNodes within PennyLane. For more details, see the `plugin usage guide <https://pennylane-sf.readthedocs.io/en/latest/usage.html>`_ and refer to the PennyLane documentation.
+        To ensure that PennyLane-SF is working correctly after installation, the test suite can be
+        run by navigating to the source code folder and running
+        ::
         
+        	$ make test
+        
+        
+        Documentation
+        ~~~~~~~~~~~~~
+        
+        To build the HTML documentation, go to the top-level directory and run
+        ::
+        
+            $ make docs
+        
+        The documentation can then be found in the ``doc/_build/html/`` directory.
+        
+        .. installation-end-inclusion-marker-do-not-remove
         
         Contributing
         ============
         
         We welcome contributions - simply fork the PennyLane-SF repository, and then make a
-        `pull request <https://help.github.com/articles/about-pull-requests/>`_ containing your contribution.  All contributers to PennyLane-SF will be listed as authors on the releases.
+        `pull request <https://help.github.com/articles/about-pull-requests/>`__ containing your contribution.
+        All contributers to PennyLane-SF will be listed as authors on the releases.
         
-        We also encourage bug reports, suggestions for new features and enhancements, and even links to cool projects or applications built on PennyLane and Strawberry Fields.
+        We also encourage bug reports, suggestions for new features and enhancements, and even links
+        to cool projects or applications built on PennyLane and Strawberry Fields.
         
         
         Authors
         =======
         
         Josh Izaac, Ville Bergholm, Maria Schuld, Nathan Killoran and Christian Gogolin
         
         If you are doing research using PennyLane and StrawberryFields, please cite our papers:
         
             Ville Bergholm, Josh Izaac, Maria Schuld, Christian Gogolin, and Nathan Killoran.
             *PennyLane: Automatic differentiation of hybrid quantum-classical computations.* 2018.
-            `arXiv:1811.04968 <https://arxiv.org/abs/1811.04968>`_
+            `arXiv:1811.04968 <https://arxiv.org/abs/1811.04968>`__
         
             Nathan Killoran, Josh Izaac, Nicolás Quesada, Ville Bergholm, Matthew Amy, and Christian Weedbrook.
             *Strawberry Fields: A Software Platform for Photonic Quantum Computing.* 2018.
-            `arXiv:1804.03159  <https://arxiv.org/abs/1804.03159>`_
+            `arXiv:1804.03159 <https://arxiv.org/abs/1804.03159>`__
         
+        .. support-start-inclusion-marker-do-not-remove
         
         Support
         =======
         
         - **Source Code:** https://github.com/XanaduAI/pennylane-sf
         - **Issue Tracker:** https://github.com/XanaduAI/pennylane-sf/issues
+        - **PennyLane Forum:** https://discuss.pennylane.ai
         
-        If you are having issues, please let us know by posting the issue on our Github issue tracker.
+        If you are having issues, please let us know by posting the issue on our Github issue tracker, or
+        by asking a question in the forum.
         
-        We also have a `Strawberry Fields Slack channel <https://u.strawberryfields.ai/slack>`_ -
+        We also have a `Strawberry Fields Slack channel <https://u.strawberryfields.ai/slack>`__ -
         come join the discussion and chat with our Strawberry Fields team.
         
+        .. support-end-inclusion-marker-do-not-remove
+        .. license-start-inclusion-marker-do-not-remove
         
         License
         =======
         
         PennyLane-SF is **free** and **open source**, released under the Apache License, Version 2.0.
         
+        .. license-end-inclusion-marker-do-not-remove
+        
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Scientific/Engineering :: Physics
 Provides: pennylane_sf
```

### Comparing `PennyLane-SF-0.8.0/PennyLane_SF.egg-info/PKG-INFO` & `PennyLane-SF-0.9.0/PennyLane_SF.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: PennyLane-SF
-Version: 0.8.0
+Version: 0.9.0
 Summary: Open source library for continuous-variable quantum computation
 Home-page: https://github.com/XanaduAI/pennylane-sf
 Maintainer: Xanadu Inc.
 Maintainer-email: nathan@xanadu.ai
 License: Apache License 2.0
 Description: PennyLane Strawberry Fields Plugin
         ##################################
@@ -29,110 +29,159 @@
             :alt: PyPI
             :target: https://pypi.org/project/PennyLane-SF
         
         .. image:: https://img.shields.io/pypi/pyversions/PennyLane-SF.svg?style=for-the-badge
             :alt: PyPI - Python Version
             :target: https://pypi.org/project/PennyLane-SF
         
+        .. header-start-inclusion-marker-do-not-remove
         
-        This PennyLane plugin allows the Strawberry Fields simulators to be used as PennyLane devices.
         
-        `Strawberry Fields <https://strawberryfields.readthedocs.io>`_ is a full-stack Python library for designing, simulating, and optimizing continuous variable (CV) quantum optical circuits.
+        The PennyLane-SF plugin integrates the StrawberryFields photonic quantum computing framework with PennyLane's
+        quantum machine learning capabilities.
         
-        `PennyLane <https://pennylane.readthedocs.io>`_ is a machine learning library for optimization and automatic differentiation of hybrid quantum-classical computations.
+        `PennyLane <https://pennylane.readthedocs.io>`__ is a machine learning library for optimization and
+        automatic differentiation of hybrid quantum-classical computations.
+        
+        `Strawberry Fields <https://strawberryfields.readthedocs.io>`__ is a full-stack Python library
+        for designing, simulating, and optimizing photonic quantum circuits.
+        
+        .. header-end-inclusion-marker-do-not-remove
+        
+        The plugin documentation can be found here: `PennyLane-Strawberry Fields <https://pennylane-sf.readthedocs.io/en/latest/>`__.
         
         
         Features
         ========
         
         * Provides two devices to be used with PennyLane: ``strawberryfields.fock`` and ``strawberryfields.gaussian``. These provide access to the Strawberry Fields Fock and Gaussian backends respectively.
         
         * Supports all core PennyLane operations and observables across the two devices.
         
         * Combine Strawberry Fields optimized simulator suite with PennyLane's automatic differentiation and optimization.
         
+        .. installation-start-inclusion-marker-do-not-remove
         
         Installation
         ============
         
-        PennyLane-SF requires both PennyLane and Strawberry Fields. It can be installed via ``pip``:
+        Installation of PennyLane-SF, as well as all required Python packages, can be installed via ``pip``:
+        ::
+        
+           	$ python -m pip install pennylane-sf
+        
+        
+        Make sure you are using the Python 3 version of pip.
+        
+        Alternatively, you can install PennyLane-SF from the source code by navigating to the top directory and running
+        ::
+        
+        	$ python setup.py install
         
-        .. code-block:: bash
+        Dependencies
+        ~~~~~~~~~~~~
         
-            $ python -m pip install pennylane-sf
+        PennyLane-SF requires the following libraries be installed:
         
+        * `Python <http://python.org/>`__ >=3.6
         
-        Getting started
-        ===============
+        as well as the following Python packages:
         
-        Once the PennyLane-SF plugin is installed, the two provided Strawberry Fields devices can be accessed straight away in PennyLane.
+        * `PennyLane <http://pennylane.readthedocs.io/>`__ >=0.7
+        * `StrawberryFields <https://strawberryfields.readthedocs.io/>`__ >=0.11.2
         
-        You can instantiate these devices for PennyLane as follows:
         
-        .. code-block:: python
+        If you currently do not have Python 3 installed,
+        we recommend `Anaconda for Python 3 <https://www.anaconda.com/download/>`__, a distributed
+        version of Python packaged for scientific computation.
         
-            import pennylane as qml
-            dev_fock = qml.device('strawberryfields.fock', wires=2, cutoff_dim=10)
-            dev_gaussian = qml.device('strawberryfields.gaussian', wires=2)
+        Software tests
+        ~~~~~~~~~~~~~~
         
-        These devices can then be used just like other devices for the definition and evaluation of QNodes within PennyLane. For more details, see the `plugin usage guide <https://pennylane-sf.readthedocs.io/en/latest/usage.html>`_ and refer to the PennyLane documentation.
+        To ensure that PennyLane-SF is working correctly after installation, the test suite can be
+        run by navigating to the source code folder and running
+        ::
         
+        	$ make test
+        
+        
+        Documentation
+        ~~~~~~~~~~~~~
+        
+        To build the HTML documentation, go to the top-level directory and run
+        ::
+        
+            $ make docs
+        
+        The documentation can then be found in the ``doc/_build/html/`` directory.
+        
+        .. installation-end-inclusion-marker-do-not-remove
         
         Contributing
         ============
         
         We welcome contributions - simply fork the PennyLane-SF repository, and then make a
-        `pull request <https://help.github.com/articles/about-pull-requests/>`_ containing your contribution.  All contributers to PennyLane-SF will be listed as authors on the releases.
+        `pull request <https://help.github.com/articles/about-pull-requests/>`__ containing your contribution.
+        All contributers to PennyLane-SF will be listed as authors on the releases.
         
-        We also encourage bug reports, suggestions for new features and enhancements, and even links to cool projects or applications built on PennyLane and Strawberry Fields.
+        We also encourage bug reports, suggestions for new features and enhancements, and even links
+        to cool projects or applications built on PennyLane and Strawberry Fields.
         
         
         Authors
         =======
         
         Josh Izaac, Ville Bergholm, Maria Schuld, Nathan Killoran and Christian Gogolin
         
         If you are doing research using PennyLane and StrawberryFields, please cite our papers:
         
             Ville Bergholm, Josh Izaac, Maria Schuld, Christian Gogolin, and Nathan Killoran.
             *PennyLane: Automatic differentiation of hybrid quantum-classical computations.* 2018.
-            `arXiv:1811.04968 <https://arxiv.org/abs/1811.04968>`_
+            `arXiv:1811.04968 <https://arxiv.org/abs/1811.04968>`__
         
             Nathan Killoran, Josh Izaac, Nicolás Quesada, Ville Bergholm, Matthew Amy, and Christian Weedbrook.
             *Strawberry Fields: A Software Platform for Photonic Quantum Computing.* 2018.
-            `arXiv:1804.03159  <https://arxiv.org/abs/1804.03159>`_
+            `arXiv:1804.03159 <https://arxiv.org/abs/1804.03159>`__
         
+        .. support-start-inclusion-marker-do-not-remove
         
         Support
         =======
         
         - **Source Code:** https://github.com/XanaduAI/pennylane-sf
         - **Issue Tracker:** https://github.com/XanaduAI/pennylane-sf/issues
+        - **PennyLane Forum:** https://discuss.pennylane.ai
         
-        If you are having issues, please let us know by posting the issue on our Github issue tracker.
+        If you are having issues, please let us know by posting the issue on our Github issue tracker, or
+        by asking a question in the forum.
         
-        We also have a `Strawberry Fields Slack channel <https://u.strawberryfields.ai/slack>`_ -
+        We also have a `Strawberry Fields Slack channel <https://u.strawberryfields.ai/slack>`__ -
         come join the discussion and chat with our Strawberry Fields team.
         
+        .. support-end-inclusion-marker-do-not-remove
+        .. license-start-inclusion-marker-do-not-remove
         
         License
         =======
         
         PennyLane-SF is **free** and **open source**, released under the Apache License, Version 2.0.
         
+        .. license-end-inclusion-marker-do-not-remove
+        
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Scientific/Engineering :: Physics
 Provides: pennylane_sf
```

### Comparing `PennyLane-SF-0.8.0/pennylane_sf/_version.py` & `PennyLane-SF-0.9.0/pennylane_sf/_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2018 Xanadu Quantum Technologies Inc.
+# Copyright 2018-2020 Xanadu Quantum Technologies Inc.
 
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 
 #     http://www.apache.org/licenses/LICENSE-2.0
 
@@ -12,8 +12,8 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """Version information.
    Version number (major.minor.patch[-label])
 """
 
-__version__ = '0.8.0'
+__version__ = '0.9.0'
```

### Comparing `PennyLane-SF-0.8.0/pennylane_sf/expectations.py` & `PennyLane-SF-0.9.0/pennylane_sf/expectations.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2018 Xanadu Quantum Technologies Inc.
+# Copyright 2018-2020 Xanadu Quantum Technologies Inc.
 
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PennyLane-SF-0.8.0/pennylane_sf/fock.py` & `PennyLane-SF-0.9.0/pennylane_sf/fock.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2018 Xanadu Quantum Technologies Inc.
+# Copyright 2018-2020 Xanadu Quantum Technologies Inc.
 
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PennyLane-SF-0.8.0/pennylane_sf/gaussian.py` & `PennyLane-SF-0.9.0/pennylane_sf/gaussian.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2018 Xanadu Quantum Technologies Inc.
+# Copyright 2018-2020 Xanadu Quantum Technologies Inc.
 
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 
 #     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `PennyLane-SF-0.8.0/pennylane_sf/simulator.py` & `PennyLane-SF-0.9.0/pennylane_sf/simulator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2018 Xanadu Quantum Technologies Inc.
+# Copyright 2018-2020 Xanadu Quantum Technologies Inc.
 
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 
 #     http://www.apache.org/licenses/LICENSE-2.0
 
@@ -55,15 +55,15 @@
         shots (int): Number of circuit evaluations/random samples used
             to estimate expectation values of observables. If ``analytic=True``,
             this setting is ignored.
         hbar (float): the convention chosen in the canonical commutation
             relation :math:`[x, p] = i \hbar`
     """
     name = 'Strawberry Fields Simulator PennyLane plugin'
-    pennylane_requires = '>=0.6.0'
+    pennylane_requires = '>=0.7.0'
     version = __version__
     author = 'Josh Izaac'
 
     short_name = 'strawberryfields'
     _operation_map = {}
     _observable_map = {}
     _capabilities = {"model": "cv"}
```

### Comparing `PennyLane-SF-0.8.0/setup.py` & `PennyLane-SF-0.9.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2018 Xanadu Quantum Technologies Inc.
+# Copyright 2018-2020 Xanadu Quantum Technologies Inc.
 
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 
 #     http://www.apache.org/licenses/LICENSE-2.0
 
@@ -18,16 +18,16 @@
 from setuptools import setup
 
 with open("pennylane_sf/_version.py") as f:
 	version = f.readlines()[-1].split()[-1].strip("\"'")
 
 
 requirements = [
-    "strawberryfields>=0.11",
-    "pennylane>=0.6"
+    "strawberryfields>=0.11.2",
+    "pennylane>=0.7"
 ]
 
 info = {
     'name': 'PennyLane-SF',
     'version': version,
     'maintainer': 'Xanadu Inc.',
     'maintainer_email': 'nathan@xanadu.ai',
@@ -61,14 +61,15 @@
     "Natural Language :: English",
     "Operating System :: POSIX",
     "Operating System :: MacOS :: MacOS X",
     "Operating System :: POSIX :: Linux",
     "Operating System :: Microsoft :: Windows",
     "Programming Language :: Python",
     'Programming Language :: Python :: 3',
-    'Programming Language :: Python :: 3.5',
     'Programming Language :: Python :: 3.6',
+    'Programming Language :: Python :: 3.7',
+    'Programming Language :: Python :: 3.8',
     'Programming Language :: Python :: 3 :: Only',
     "Topic :: Scientific/Engineering :: Physics"
 ]
 
 setup(classifiers=classifiers, **(info))
```

