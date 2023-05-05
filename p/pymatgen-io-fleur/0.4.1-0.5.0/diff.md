# Comparing `tmp/pymatgen-io-fleur-0.4.1.tar.gz` & `tmp/pymatgen-io-fleur-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymatgen-io-fleur-0.4.1.tar", last modified: Wed Dec  7 11:25:25 2022, max compression
+gzip compressed data, was "pymatgen-io-fleur-0.5.0.tar", last modified: Fri May  5 12:24:56 2023, max compression
```

## Comparing `pymatgen-io-fleur-0.4.1.tar` & `pymatgen-io-fleur-0.5.0.tar`

### file list

```diff
@@ -1,19 +1,17 @@
--rw-r--r--   0        0        0      643 2022-12-07 11:25:20.605355 pymatgen-io-fleur-0.4.1/.github/workflows/linting.yml
--rw-r--r--   0        0        0     2342 2022-12-07 11:25:20.605355 pymatgen-io-fleur-0.4.1/.github/workflows/pypi_publish.yml
--rw-r--r--   0        0        0      971 2022-12-07 11:25:20.605355 pymatgen-io-fleur-0.4.1/.github/workflows/testing.yml
--rw-r--r--   0        0        0     1818 2022-12-07 11:25:20.605355 pymatgen-io-fleur-0.4.1/.gitignore
--rw-r--r--   0        0        0     1407 2022-12-07 11:25:20.605355 pymatgen-io-fleur-0.4.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1253 2022-12-07 11:25:20.605355 pymatgen-io-fleur-0.4.1/LICENSE
--rw-r--r--   0        0        0     2761 2022-12-07 11:25:20.605355 pymatgen-io-fleur-0.4.1/README.rst
--rw-r--r--   0        0        0      390 2022-12-07 11:25:20.605355 pymatgen-io-fleur-0.4.1/pymatgen/io/fleur/__init__.py
--rw-r--r--   0        0        0     7502 2022-12-07 11:25:20.605355 pymatgen-io-fleur-0.4.1/pymatgen/io/fleur/fleurinput.py
--rw-r--r--   0        0        0    14303 2022-12-07 11:25:20.605355 pymatgen-io-fleur-0.4.1/pymatgen/io/fleur/tests/test_fleurinput.py
--rw-r--r--   0        0        0     3399 2022-12-07 11:25:20.605355 pymatgen-io-fleur-0.4.1/pyproject.toml
--rw-r--r--   0        0        0       46 2022-12-07 11:25:20.609355 pymatgen-io-fleur-0.4.1/requirements-ci.txt
--rw-r--r--   0        0        0       19 2022-12-07 11:25:20.609355 pymatgen-io-fleur-0.4.1/requirements.txt
--rw-r--r--   0        0        0      154 2022-12-07 11:25:20.609355 pymatgen-io-fleur-0.4.1/setup.cfg
--rw-r--r--   0        0        0    11105 2022-12-07 11:25:20.609355 pymatgen-io-fleur-0.4.1/test-files/inp.xml
--rw-r--r--   0        0        0    44882 2022-12-07 11:25:20.609355 pymatgen-io-fleur-0.4.1/test-files/inp_film.xml
--rw-r--r--   0        0        0      623 2022-12-07 11:25:20.609355 pymatgen-io-fleur-0.4.1/test-files/inp_test
--rw-r--r--   0        0        0      586 2022-12-07 11:25:20.609355 pymatgen-io-fleur-0.4.1/test-files/inp_test_film
--rw-r--r--   0        0        0     4134 1970-01-01 00:00:00.000000 pymatgen-io-fleur-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0      658 2023-05-05 12:24:50.635488 pymatgen-io-fleur-0.5.0/.github/workflows/linting.yml
+-rw-r--r--   0        0        0     1032 2023-05-05 12:24:50.635488 pymatgen-io-fleur-0.5.0/.github/workflows/pypi_publish.yml
+-rw-r--r--   0        0        0      725 2023-05-05 12:24:50.635488 pymatgen-io-fleur-0.5.0/.github/workflows/testing.yml
+-rw-r--r--   0        0        0     1818 2023-05-05 12:24:50.635488 pymatgen-io-fleur-0.5.0/.gitignore
+-rw-r--r--   0        0        0     1409 2023-05-05 12:24:50.635488 pymatgen-io-fleur-0.5.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1253 2023-05-05 12:24:50.635488 pymatgen-io-fleur-0.5.0/LICENSE
+-rw-r--r--   0        0        0     2761 2023-05-05 12:24:50.635488 pymatgen-io-fleur-0.5.0/README.rst
+-rw-r--r--   0        0        0      390 2023-05-05 12:24:50.635488 pymatgen-io-fleur-0.5.0/pymatgen/io/fleur/__init__.py
+-rw-r--r--   0        0        0     7498 2023-05-05 12:24:50.635488 pymatgen-io-fleur-0.5.0/pymatgen/io/fleur/fleurinput.py
+-rw-r--r--   0        0        0    14303 2023-05-05 12:24:50.635488 pymatgen-io-fleur-0.5.0/pymatgen/io/fleur/tests/test_fleurinput.py
+-rw-r--r--   0        0        0     3440 2023-05-05 12:24:50.635488 pymatgen-io-fleur-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0      154 2023-05-05 12:24:50.635488 pymatgen-io-fleur-0.5.0/setup.cfg
+-rw-r--r--   0        0        0    11105 2023-05-05 12:24:50.635488 pymatgen-io-fleur-0.5.0/test-files/inp.xml
+-rw-r--r--   0        0        0    44882 2023-05-05 12:24:50.635488 pymatgen-io-fleur-0.5.0/test-files/inp_film.xml
+-rw-r--r--   0        0        0      623 2023-05-05 12:24:50.635488 pymatgen-io-fleur-0.5.0/test-files/inp_test
+-rw-r--r--   0        0        0      586 2023-05-05 12:24:50.635488 pymatgen-io-fleur-0.5.0/test-files/inp_test_film
+-rw-r--r--   0        0        0     4176 1970-01-01 00:00:00.000000 pymatgen-io-fleur-0.5.0/PKG-INFO
```

### Comparing `pymatgen-io-fleur-0.4.1/.github/workflows/linting.yml` & `pymatgen-io-fleur-0.5.0/.github/workflows/linting.yml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 name: Linting
 
-on: [push, pull_request]
+on: [push, pull_request, workflow_call]
 
 jobs:
   build:
     runs-on: ubuntu-latest
     strategy:
       max-parallel: 4
       matrix:
```

### Comparing `pymatgen-io-fleur-0.4.1/.github/workflows/testing.yml` & `pymatgen-io-fleur-0.5.0/.github/workflows/testing.yml`

 * *Files 17% similar despite different names*

```diff
@@ -1,39 +1,33 @@
 name: Testing
 
-on: [push, pull_request]
+on: [push, pull_request, workflow_call]
 
 jobs:
   build:
 
     strategy:
       max-parallel: 20
       matrix:
         os: [ubuntu-latest]
-        python-version: ["3.8","3.9","3.10"]
+        python-version: ["3.8","3.9","3.10","3.11"]
       fail-fast: false
 
     runs-on: ${{ matrix.os }}
 
     steps:
     - uses: actions/checkout@v2
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v2
       with:
         python-version: ${{ matrix.python-version }}
-    - name: Build pymatgen with compatible numpy
-      run: |
-        python -m pip install --upgrade pip
-        pip install numpy==1.21.4 wheel cython
-        pip install pymatgen==2022.7.8 --no-cache-dir --no-build-isolation
     - name: Install dependencies
       run: |
-        pip install --quiet -r requirements-ci.txt
-        pip install masci-tools
-        pip install --no-deps -e .
+        python -m pip install --upgrade pip
+        pip install -e .[testing]
     - name: pytest
       run: |
         pytest
     - name: Upload code coverage report
       run: |
         pip install codecov
         codecov
```

### Comparing `pymatgen-io-fleur-0.4.1/.gitignore` & `pymatgen-io-fleur-0.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pymatgen-io-fleur-0.4.1/.pre-commit-config.yaml` & `pymatgen-io-fleur-0.5.0/.pre-commit-config.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -11,45 +11,45 @@
       - id: trailing-whitespace
       - id: fix-encoding-pragma
       - id: mixed-line-ending
         types: [python]
       - id: flake8
         args: ["--max-line-length=120"]
   - repo: https://github.com/psf/black
-    rev: 22.10.0 # Replace by any tag/version: https://github.com/psf/black/tags
+    rev: 23.3.0 # Replace by any tag/version: https://github.com/psf/black/tags
     hooks:
     - id: black
       language_version: python3 # Should be a command that runs python3.6+
 
   - repo: https://github.com/ikamensh/flynt/
-    rev: '0.77'
+    rev: '0.78'
     hooks:
     -   id: flynt
         args: [
             '--line-length=120',
             '--fail-on-change',
-      ]
+        ]
   - repo: local
     hooks:
 
     - id: pylint
       name: pylint
       entry: pylint
       verbose: true
       types: [python]
       language: system
       exclude: '^(docs/)|(examples/)'
 
   - repo: https://github.com/pycqa/pydocstyle
-    rev: 6.1.1  # pick a git hash / tag to point to
+    rev: 6.3.0  # pick a git hash / tag to point to
     hooks:
     -   id: pydocstyle
-        additional_dependencies: ['toml']
+        additional_dependencies: ['tomli']
 
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: 'v0.991'  # Use the sha / tag you want to point at
+    rev: 'v1.2.0'  # Use the sha / tag you want to point at
     hooks:
     -   id: mypy
         args: [
           '--namespace-packages',
           '--explicit-package-bases'
         ]
```

### Comparing `pymatgen-io-fleur-0.4.1/LICENSE` & `pymatgen-io-fleur-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pymatgen-io-fleur-0.4.1/README.rst` & `pymatgen-io-fleur-0.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `pymatgen-io-fleur-0.4.1/pymatgen/io/fleur/fleurinput.py` & `pymatgen-io-fleur-0.5.0/pymatgen/io/fleur/fleurinput.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,23 +83,23 @@
         Kwargs are passed on to :py:func:`~masci_tools.io.fleur_xml.load_inpxml()` if the input
         is interpreted as a XML file
 
         returns: :py:class:`FleurInput` generated from the information read in from the data
         """
         from masci_tools.io.fleur_inpgen import read_inpgen_file
         from masci_tools.io.fleur_xml import load_inpxml
-        from masci_tools.util.xml.xml_getters import get_structure_data, get_parameter_data
+        from masci_tools.util.xml.xml_getters import get_structuredata, get_parameterdata
 
         if inpgen_input:
             cell, atoms, pbc, parameters = read_inpgen_file(data)
             title_in = parameters.pop("title", "")
         else:
             xmltree, schema_dict = load_inpxml(data, **kwargs)
-            atoms, cell, pbc = get_structure_data(xmltree, schema_dict)
-            parameters = get_parameter_data(xmltree, schema_dict)
+            atoms, cell, pbc = get_structuredata(xmltree, schema_dict)
+            parameters = get_parameterdata(xmltree, schema_dict)
             title_in = parameters.pop("title", "")
 
         positions, elements = zip(*[(site.position, site.symbol) for site in atoms])
         # create lattice and structure object
         lattice_in = Lattice(cell, pbc=pbc)
         structure_in = Structure(lattice_in, elements, positions, coords_are_cartesian=True)
```

### Comparing `pymatgen-io-fleur-0.4.1/pymatgen/io/fleur/tests/test_fleurinput.py` & `pymatgen-io-fleur-0.5.0/pymatgen/io/fleur/tests/test_fleurinput.py`

 * *Files identical despite different names*

### Comparing `pymatgen-io-fleur-0.4.1/pyproject.toml` & `pymatgen-io-fleur-0.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -10,28 +10,29 @@
 readme = "README.rst"
 license = {file = "LICENSE"}
 classifiers=[
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Development Status :: 4 - Beta",
         "Intended Audience :: Science/Research",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Topic :: Scientific/Engineering :: Information Analysis",
         "Topic :: Scientific/Engineering :: Physics",
         "Topic :: Scientific/Engineering :: Chemistry",
         "Topic :: Software Development :: Libraries :: Python Modules",
     ]
 keywords = ['pymatgen', 'fleur']
 requires-python = ">=3.8"
 dependencies = [
           "pymatgen>=2022.7.8",
-          "masci-tools>=0.11.3,~=0.11",
+          "masci-tools>=0.13",
         ]
 
 [project.optional-dependencies]
 testing = [
   "pytest~=6.0",
   "pytest-cov~=3.0",
 ]
```

### Comparing `pymatgen-io-fleur-0.4.1/test-files/inp.xml` & `pymatgen-io-fleur-0.5.0/test-files/inp.xml`

 * *Files identical despite different names*

### Comparing `pymatgen-io-fleur-0.4.1/test-files/inp_film.xml` & `pymatgen-io-fleur-0.5.0/test-files/inp_film.xml`

 * *Files identical despite different names*

### Comparing `pymatgen-io-fleur-0.4.1/test-files/inp_test` & `pymatgen-io-fleur-0.5.0/test-files/inp_test`

 * *Files identical despite different names*

### Comparing `pymatgen-io-fleur-0.4.1/test-files/inp_test_film` & `pymatgen-io-fleur-0.5.0/test-files/inp_test_film`

 * *Files identical despite different names*

### Comparing `pymatgen-io-fleur-0.4.1/PKG-INFO` & `pymatgen-io-fleur-0.5.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 Metadata-Version: 2.1
 Name: pymatgen-io-fleur
-Version: 0.4.1
+Version: 0.5.0
 Summary: A pymatgen add-on for IO for the fleur code.
 Keywords: pymatgen,fleur
 Author-email: The JuDFT team <he.janssen@fz-juelich.de>
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Scientific/Engineering :: Chemistry
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: pymatgen>=2022.7.8
-Requires-Dist: masci-tools>=0.11.3,~=0.11
+Requires-Dist: masci-tools>=0.13
 Requires-Dist: pre-commit>=2.6.0 ; extra == "pre-commit"
 Requires-Dist: pylint~=2.12.2 ; extra == "pre-commit"
 Requires-Dist: pytest~=6.0 ; extra == "testing"
 Requires-Dist: pytest-cov~=3.0 ; extra == "testing"
 Project-URL: Home, https://github.com/JuDFTteam/pymatgen-io-fleur
 Project-URL: Source, https://github.com/JuDFTteam/pymatgen-io-fleur
 Provides-Extra: pre-commit
```

