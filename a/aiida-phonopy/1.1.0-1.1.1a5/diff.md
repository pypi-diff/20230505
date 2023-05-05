# Comparing `tmp/aiida-phonopy-1.1.0.tar.gz` & `tmp/aiida-phonopy-1.1.1a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiida-phonopy-1.1.0.tar", last modified: Tue May  2 13:41:29 2023, max compression
+gzip compressed data, was "aiida-phonopy-1.1.1a5.tar", last modified: Fri May  5 10:22:11 2023, max compression
```

## Comparing `aiida-phonopy-1.1.0.tar` & `aiida-phonopy-1.1.1a5.tar`

### file list

```diff
@@ -1,46 +1,46 @@
--rw-r--r--   0        0        0     3718 2023-05-02 11:10:46.800256 aiida-phonopy-1.1.0/.github/workflows/cd.yml
--rw-r--r--   0        0        0     2397 2023-05-02 11:10:46.822256 aiida-phonopy-1.1.0/.github/workflows/ci.yml
--rw-r--r--   0        0        0     1512 2023-05-02 11:10:46.868255 aiida-phonopy-1.1.0/.github/workflows/validate_release_tag.py
--rw-r--r--   0        0        0      392 2022-10-25 11:13:01.498840 aiida-phonopy-1.1.0/.gitignore
--rw-r--r--   0        0        0      781 2023-05-02 11:30:11.383556 aiida-phonopy-1.1.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      239 2022-10-25 10:53:20.495745 aiida-phonopy-1.1.0/.readthedocs.yml
--rw-r--r--   0        0        0     4028 2023-05-02 11:42:38.288260 aiida-phonopy-1.1.0/CHANGELOG.md
--rw-r--r--   0        0        0     1085 2022-10-25 10:53:20.499745 aiida-phonopy-1.1.0/LICENSE.txt
--rw-r--r--   0        0        0     2003 2022-10-25 12:18:09.423923 aiida-phonopy-1.1.0/README.md
--rw-r--r--   0        0        0      155 2022-01-27 11:33:53.420852 aiida-phonopy-1.1.0/docker-compose.yml
--rw-r--r--   0        0        0    52380 2022-10-25 10:53:20.513744 aiida-phonopy-1.1.0/examples/BaTiO3/FORCE_SETS
--rw-r--r--   0        0        0    21945 2022-10-25 10:53:20.515744 aiida-phonopy-1.1.0/examples/BaTiO3/phonopy.yaml
--rw-r--r--   0        0        0    52380 2022-10-25 10:53:20.521744 aiida-phonopy-1.1.0/examples/BaTiO3/ref_out/FORCE_SETS
--rw-r--r--   0        0        0       41 2022-10-25 10:53:20.523744 aiida-phonopy-1.1.0/examples/BaTiO3/ref_out/aiida.in
--rw-r--r--   0        0        0     1538 2022-10-25 10:53:20.525744 aiida-phonopy-1.1.0/examples/BaTiO3/ref_out/aiida.out
--rw-r--r--   0        0        0    58620 2022-10-25 10:53:20.527744 aiida-phonopy-1.1.0/examples/BaTiO3/ref_out/band.hdf5
--rw-r--r--   0        0        0    43797 2022-10-25 10:53:20.530744 aiida-phonopy-1.1.0/examples/BaTiO3/ref_out/force_constants.hdf5
--rw-r--r--   0        0        0     2445 2022-10-25 10:53:20.532744 aiida-phonopy-1.1.0/examples/BaTiO3/ref_out/irreps.yaml
--rw-r--r--   0        0        0    39220 2022-10-25 10:53:20.534744 aiida-phonopy-1.1.0/examples/BaTiO3/ref_out/mesh.hdf5
--rw-r--r--   0        0        0    21837 2022-10-25 10:53:20.537744 aiida-phonopy-1.1.0/examples/BaTiO3/ref_out/phonopy.yaml
--rw-r--r--   0        0        0     2336 2022-10-25 10:53:20.539744 aiida-phonopy-1.1.0/examples/BaTiO3/ref_out/qpoints.hdf5
--rw-r--r--   0        0        0    33644 2022-10-25 10:53:20.542744 aiida-phonopy-1.1.0/examples/BaTiO3/ref_out/thermal_properties.yaml
--rw-r--r--   0        0        0     1254 2023-05-02 11:10:46.944255 aiida-phonopy-1.1.0/examples/BaTiO3/script.py
--rw-r--r--   0        0        0     3220 2023-05-02 11:21:44.224474 aiida-phonopy-1.1.0/pyproject.toml
--rw-r--r--   0        0        0       91 2023-05-02 11:13:04.579463 aiida-phonopy-1.1.0/src/aiida_phonopy/__init__.py
--rw-r--r--   0        0        0        0 2022-11-21 14:49:58.336931 aiida-phonopy-1.1.0/src/aiida_phonopy/calculations/__init__.py
--rw-r--r--   0        0        0       62 2022-11-21 14:49:58.187932 aiida-phonopy-1.1.0/src/aiida_phonopy/calculations/functions/__init__.py
--rw-r--r--   0        0        0    10382 2023-02-20 17:13:17.220510 aiida-phonopy-1.1.0/src/aiida_phonopy/calculations/functions/data_utils.py
--rw-r--r--   0        0        0     3591 2022-11-21 14:49:58.333931 aiida-phonopy-1.1.0/src/aiida_phonopy/calculations/functions/link_structures.py
--rw-r--r--   0        0        0    18063 2023-05-02 11:02:32.280097 aiida-phonopy-1.1.0/src/aiida_phonopy/calculations/phonopy.py
--rw-r--r--   0        0        0      271 2022-11-21 14:49:59.015927 aiida-phonopy-1.1.0/src/aiida_phonopy/data/__init__.py
--rw-r--r--   0        0        0     3026 2023-05-02 11:02:03.694261 aiida-phonopy-1.1.0/src/aiida_phonopy/data/force_constants.py
--rw-r--r--   0        0        0     9265 2023-05-02 10:59:59.422975 aiida-phonopy-1.1.0/src/aiida_phonopy/data/phonopy.py
--rw-r--r--   0        0        0    11504 2023-05-02 11:14:43.966892 aiida-phonopy-1.1.0/src/aiida_phonopy/data/preprocess.py
--rw-r--r--   0        0        0    19358 2023-05-02 11:10:47.202254 aiida-phonopy-1.1.0/src/aiida_phonopy/data/raw.py
--rw-r--r--   0        0        0       65 2022-11-21 14:49:58.597929 aiida-phonopy-1.1.0/src/aiida_phonopy/parsers/__init__.py
--rw-r--r--   0        0        0     2450 2022-11-21 14:49:58.615929 aiida-phonopy-1.1.0/src/aiida_phonopy/parsers/base.py
--rw-r--r--   0        0        0    18362 2023-05-02 11:10:47.175254 aiida-phonopy-1.1.0/src/aiida_phonopy/parsers/phonopy.py
--rw-r--r--   0        0        0        0 2022-11-21 14:49:58.576929 aiida-phonopy-1.1.0/src/aiida_phonopy/parsers/raw_parsers/__init__.py
--rw-r--r--   0        0        0     1080 2023-02-10 21:29:51.740132 aiida-phonopy-1.1.0/src/aiida_phonopy/parsers/raw_parsers/phonopy.py
--rw-r--r--   0        0        0        0 2022-11-21 14:49:58.975927 aiida-phonopy-1.1.0/src/aiida_phonopy/utils/__init__.py
--rw-r--r--   0        0        0     1879 2022-11-21 14:49:59.001927 aiida-phonopy-1.1.0/src/aiida_phonopy/utils/mapping.py
--rw-r--r--   0        0        0      688 2022-11-21 14:49:59.008927 aiida-phonopy-1.1.0/src/aiida_phonopy/utils/resources.py
--rw-r--r--   0        0        0        0 2022-11-21 14:49:58.848928 aiida-phonopy-1.1.0/src/aiida_phonopy/workflows/__init__.py
--rw-r--r--   0        0        0    15627 2023-05-02 11:05:35.530044 aiida-phonopy-1.1.0/src/aiida_phonopy/workflows/phonopy.py
--rw-r--r--   0        0        0     3585 1970-01-01 00:00:00.000000 aiida-phonopy-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     3763 2023-05-05 10:22:08.167641 aiida-phonopy-1.1.1a5/.github/workflows/cd.yml
+-rw-r--r--   0        0        0     2397 2023-05-05 10:22:08.167641 aiida-phonopy-1.1.1a5/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     1512 2023-05-05 10:22:08.167641 aiida-phonopy-1.1.1a5/.github/workflows/validate_release_tag.py
+-rw-r--r--   0        0        0      392 2023-05-05 10:22:08.167641 aiida-phonopy-1.1.1a5/.gitignore
+-rw-r--r--   0        0        0     1034 2023-05-05 10:22:08.167641 aiida-phonopy-1.1.1a5/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      239 2023-05-05 10:22:08.167641 aiida-phonopy-1.1.1a5/.readthedocs.yml
+-rw-r--r--   0        0        0     4028 2023-05-05 10:22:08.167641 aiida-phonopy-1.1.1a5/CHANGELOG.md
+-rw-r--r--   0        0        0     1085 2023-05-05 10:22:08.167641 aiida-phonopy-1.1.1a5/LICENSE.txt
+-rw-r--r--   0        0        0     1816 2023-05-05 10:22:08.167641 aiida-phonopy-1.1.1a5/README.md
+-rw-r--r--   0        0        0      155 2023-05-05 10:22:08.167641 aiida-phonopy-1.1.1a5/docker-compose.yml
+-rw-r--r--   0        0        0    52380 2023-05-05 10:22:08.175641 aiida-phonopy-1.1.1a5/examples/BaTiO3/FORCE_SETS
+-rw-r--r--   0        0        0    21945 2023-05-05 10:22:08.175641 aiida-phonopy-1.1.1a5/examples/BaTiO3/phonopy.yaml
+-rw-r--r--   0        0        0    52380 2023-05-05 10:22:08.175641 aiida-phonopy-1.1.1a5/examples/BaTiO3/ref_out/FORCE_SETS
+-rw-r--r--   0        0        0       41 2023-05-05 10:22:08.175641 aiida-phonopy-1.1.1a5/examples/BaTiO3/ref_out/aiida.in
+-rw-r--r--   0        0        0     1538 2023-05-05 10:22:08.175641 aiida-phonopy-1.1.1a5/examples/BaTiO3/ref_out/aiida.out
+-rw-r--r--   0        0        0    58620 2023-05-05 10:22:08.175641 aiida-phonopy-1.1.1a5/examples/BaTiO3/ref_out/band.hdf5
+-rw-r--r--   0        0        0    43797 2023-05-05 10:22:08.175641 aiida-phonopy-1.1.1a5/examples/BaTiO3/ref_out/force_constants.hdf5
+-rw-r--r--   0        0        0     2445 2023-05-05 10:22:08.175641 aiida-phonopy-1.1.1a5/examples/BaTiO3/ref_out/irreps.yaml
+-rw-r--r--   0        0        0    39220 2023-05-05 10:22:08.175641 aiida-phonopy-1.1.1a5/examples/BaTiO3/ref_out/mesh.hdf5
+-rw-r--r--   0        0        0    21837 2023-05-05 10:22:08.175641 aiida-phonopy-1.1.1a5/examples/BaTiO3/ref_out/phonopy.yaml
+-rw-r--r--   0        0        0     2336 2023-05-05 10:22:08.175641 aiida-phonopy-1.1.1a5/examples/BaTiO3/ref_out/qpoints.hdf5
+-rw-r--r--   0        0        0    33644 2023-05-05 10:22:08.175641 aiida-phonopy-1.1.1a5/examples/BaTiO3/ref_out/thermal_properties.yaml
+-rw-r--r--   0        0        0     1254 2023-05-05 10:22:08.175641 aiida-phonopy-1.1.1a5/examples/BaTiO3/script.py
+-rw-r--r--   0        0        0     3220 2023-05-05 10:22:08.175641 aiida-phonopy-1.1.1a5/pyproject.toml
+-rw-r--r--   0        0        0       93 2023-05-05 10:22:08.175641 aiida-phonopy-1.1.1a5/src/aiida_phonopy/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-05 10:22:08.175641 aiida-phonopy-1.1.1a5/src/aiida_phonopy/calculations/__init__.py
+-rw-r--r--   0        0        0       62 2023-05-05 10:22:08.175641 aiida-phonopy-1.1.1a5/src/aiida_phonopy/calculations/functions/__init__.py
+-rw-r--r--   0        0        0    10762 2023-05-05 10:22:08.175641 aiida-phonopy-1.1.1a5/src/aiida_phonopy/calculations/functions/data_utils.py
+-rw-r--r--   0        0        0     4037 2023-05-05 10:22:08.179641 aiida-phonopy-1.1.1a5/src/aiida_phonopy/calculations/functions/link_structures.py
+-rw-r--r--   0        0        0    18068 2023-05-05 10:22:08.179641 aiida-phonopy-1.1.1a5/src/aiida_phonopy/calculations/phonopy.py
+-rw-r--r--   0        0        0      271 2023-05-05 10:22:08.179641 aiida-phonopy-1.1.1a5/src/aiida_phonopy/data/__init__.py
+-rw-r--r--   0        0        0     4299 2023-05-05 10:22:08.179641 aiida-phonopy-1.1.1a5/src/aiida_phonopy/data/force_constants.py
+-rw-r--r--   0        0        0    10147 2023-05-05 10:22:08.179641 aiida-phonopy-1.1.1a5/src/aiida_phonopy/data/phonopy.py
+-rw-r--r--   0        0        0    13302 2023-05-05 10:22:08.179641 aiida-phonopy-1.1.1a5/src/aiida_phonopy/data/preprocess.py
+-rw-r--r--   0        0        0    21446 2023-05-05 10:22:08.179641 aiida-phonopy-1.1.1a5/src/aiida_phonopy/data/raw.py
+-rw-r--r--   0        0        0       65 2023-05-05 10:22:08.179641 aiida-phonopy-1.1.1a5/src/aiida_phonopy/parsers/__init__.py
+-rw-r--r--   0        0        0     2450 2023-05-05 10:22:08.179641 aiida-phonopy-1.1.1a5/src/aiida_phonopy/parsers/base.py
+-rw-r--r--   0        0        0    18608 2023-05-05 10:22:08.179641 aiida-phonopy-1.1.1a5/src/aiida_phonopy/parsers/phonopy.py
+-rw-r--r--   0        0        0        0 2023-05-05 10:22:08.179641 aiida-phonopy-1.1.1a5/src/aiida_phonopy/parsers/raw_parsers/__init__.py
+-rw-r--r--   0        0        0     1080 2023-05-05 10:22:08.179641 aiida-phonopy-1.1.1a5/src/aiida_phonopy/parsers/raw_parsers/phonopy.py
+-rw-r--r--   0        0        0        0 2023-05-05 10:22:08.179641 aiida-phonopy-1.1.1a5/src/aiida_phonopy/utils/__init__.py
+-rw-r--r--   0        0        0     2138 2023-05-05 10:22:08.179641 aiida-phonopy-1.1.1a5/src/aiida_phonopy/utils/mapping.py
+-rw-r--r--   0        0        0      688 2023-05-05 10:22:08.179641 aiida-phonopy-1.1.1a5/src/aiida_phonopy/utils/resources.py
+-rw-r--r--   0        0        0        0 2023-05-05 10:22:08.179641 aiida-phonopy-1.1.1a5/src/aiida_phonopy/workflows/__init__.py
+-rw-r--r--   0        0        0    15542 2023-05-05 10:22:08.179641 aiida-phonopy-1.1.1a5/src/aiida_phonopy/workflows/phonopy.py
+-rw-r--r--   0        0        0     3400 1970-01-01 00:00:00.000000 aiida-phonopy-1.1.1a5/PKG-INFO
```

### Comparing `aiida-phonopy-1.1.0/.github/workflows/cd.yml` & `aiida-phonopy-1.1.1a5/.github/workflows/cd.yml`

 * *Files 6% similar despite different names*

```diff
@@ -117,18 +117,18 @@
             uses: actions/setup-python@v2
             with:
                 python-version: '3.8'
 
         -   name: Install flit
             run: pip install flit~=3.4
 
-        -   name: Build and publish to TestPyPI
-            run: flit publish
-            env:
-                FLIT_USERNAME: __token__
-                FLIT_PASSWORD: ${{ secrets.TEST_PYPI_API_TOKEN }}
+        # -   name: Build and publish to TestPyPI
+        #     run: flit publish --repository https://test.pypi.org/legacy/
+        #     env:
+        #         FLIT_USERNAME: __token__
+        #         FLIT_PASSWORD: ${{ secrets.TEST_PYPI_API_TOKEN }}
 
-        -   name: Build and publish to PyPI
+        -   name: Build and publish
             run: flit publish
             env:
                 FLIT_USERNAME: __token__
                 FLIT_PASSWORD: ${{ secrets.PYPI_API_TOKEN }}
```

### Comparing `aiida-phonopy-1.1.0/.github/workflows/ci.yml` & `aiida-phonopy-1.1.1a5/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `aiida-phonopy-1.1.0/.github/workflows/validate_release_tag.py` & `aiida-phonopy-1.1.1a5/.github/workflows/validate_release_tag.py`

 * *Files identical despite different names*

### Comparing `aiida-phonopy-1.1.0/.pre-commit-config.yaml` & `aiida-phonopy-1.1.1a5/.pre-commit-config.yaml`

 * *Files 13% similar despite different names*

```diff
@@ -30,7 +30,18 @@
 -   repo: local
     hooks:
     -   id: pylint
         name: pylint
         entry: pylint
         types: [python]
         language: system
+
+-   repo: https://github.com/PyCQA/pydocstyle
+    rev: '6.1.1'
+    hooks:
+    -   id: pydocstyle
+        exclude: >
+            (?x)^(
+                docs/.*|
+                tests/.*(?<!\.py)$
+            )$
+        additional_dependencies: ['toml']
```

### Comparing `aiida-phonopy-1.1.0/CHANGELOG.md` & `aiida-phonopy-1.1.1a5/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `aiida-phonopy-1.1.0/LICENSE.txt` & `aiida-phonopy-1.1.1a5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aiida-phonopy-1.1.0/README.md` & `aiida-phonopy-1.1.1a5/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 # `aiida-phonopy`
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
 [![PyPI version](https://badge.fury.io/py/aiida-phonopy.svg)](https://badge.fury.io/py/aiida-phonopy)
-[![Build Status](https://github.com/aiida-phonopy/aiida-phonopy/workflows/aiida-phonopy/badge.svg?branch=develop&event=push)](https://github.com/aiida-phonopy/aiida-phonopy/actions)
 [![Docs status](https://readthedocs.org/projects/aiida-phonopy/badge)](http://aiida-phonopy.readthedocs.io/)
 
 This is the official AiiDA plugin for [Phonopy](https://phonopy.github.io/phonopy/index.html).
 
 ## Compatibility
 
 From `v0.7.0` this plugin does not support retro-compatibility with previous versions,
@@ -35,9 +34,9 @@
 
 ## Acknowlegements
 
 We acknowledge support from:
 * the [U Bremen Excellence Chairs](https://www.uni-bremen.de/u-bremen-excellence-chairs) program funded within the scope of the [Excellence Strategy of Germany’s federal and state governments](https://www.dfg.de/en/research_funding/excellence_strategy/index.html);
 * the [MAPEX](https://www.uni-bremen.de/en/mapex) Center for Materials and Processes.
 
-<img src="https://raw.githubusercontent.com/aiida-phonopy/aiida-phonopy/develop/docs/source/images/UBREMEN.png" width="300px" height="54px"/>
-<img src="https://raw.githubusercontent.com/aiida-phonopy/aiida-phonopy/develop/docs/source/images/MAPEX.jpg" width="300px" height="99px"/>
+<img src="https://raw.githubusercontent.com/aiida-phonopy/aiida-phonopy/main/docs/source/images/UBREMEN.png" width="300px" height="108px"/>
+<img src="https://raw.githubusercontent.com/aiida-phonopy/aiida-phonopy/main/docs/source/images/MAPEX.jpg" width="300px" height="99px"/>
```

### Comparing `aiida-phonopy-1.1.0/examples/BaTiO3/FORCE_SETS` & `aiida-phonopy-1.1.1a5/examples/BaTiO3/FORCE_SETS`

 * *Files identical despite different names*

### Comparing `aiida-phonopy-1.1.0/examples/BaTiO3/phonopy.yaml` & `aiida-phonopy-1.1.1a5/examples/BaTiO3/phonopy.yaml`

 * *Files identical despite different names*

### Comparing `aiida-phonopy-1.1.0/examples/BaTiO3/ref_out/FORCE_SETS` & `aiida-phonopy-1.1.1a5/examples/BaTiO3/ref_out/FORCE_SETS`

 * *Files identical despite different names*

### Comparing `aiida-phonopy-1.1.0/examples/BaTiO3/ref_out/aiida.out` & `aiida-phonopy-1.1.1a5/examples/BaTiO3/ref_out/aiida.out`

 * *Files identical despite different names*

### Comparing `aiida-phonopy-1.1.0/examples/BaTiO3/ref_out/band.hdf5` & `aiida-phonopy-1.1.1a5/examples/BaTiO3/ref_out/band.hdf5`

 * *Files identical despite different names*

### Comparing `aiida-phonopy-1.1.0/examples/BaTiO3/ref_out/force_constants.hdf5` & `aiida-phonopy-1.1.1a5/examples/BaTiO3/ref_out/force_constants.hdf5`

 * *Files identical despite different names*

### Comparing `aiida-phonopy-1.1.0/examples/BaTiO3/ref_out/irreps.yaml` & `aiida-phonopy-1.1.1a5/examples/BaTiO3/ref_out/irreps.yaml`

 * *Files identical despite different names*

### Comparing `aiida-phonopy-1.1.0/examples/BaTiO3/ref_out/mesh.hdf5` & `aiida-phonopy-1.1.1a5/examples/BaTiO3/ref_out/mesh.hdf5`

 * *Files identical despite different names*

### Comparing `aiida-phonopy-1.1.0/examples/BaTiO3/ref_out/phonopy.yaml` & `aiida-phonopy-1.1.1a5/examples/BaTiO3/ref_out/phonopy.yaml`

 * *Files identical despite different names*

### Comparing `aiida-phonopy-1.1.0/examples/BaTiO3/ref_out/qpoints.hdf5` & `aiida-phonopy-1.1.1a5/examples/BaTiO3/ref_out/qpoints.hdf5`

 * *Files identical despite different names*

### Comparing `aiida-phonopy-1.1.0/examples/BaTiO3/ref_out/thermal_properties.yaml` & `aiida-phonopy-1.1.1a5/examples/BaTiO3/ref_out/thermal_properties.yaml`

 * *Files identical despite different names*

### Comparing `aiida-phonopy-1.1.0/examples/BaTiO3/script.py` & `aiida-phonopy-1.1.1a5/examples/BaTiO3/script.py`

 * *Files identical despite different names*

### Comparing `aiida-phonopy-1.1.0/pyproject.toml` & `aiida-phonopy-1.1.1a5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aiida-phonopy-1.1.0/src/aiida_phonopy/calculations/functions/data_utils.py` & `aiida-phonopy-1.1.1a5/src/aiida_phonopy/calculations/functions/data_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,71 +1,71 @@
 # -*- coding: utf-8 -*-
 """Calcfunctions Utils for aiida-phonopy DataTypes."""
+from __future__ import annotations
+
 from aiida import orm
 from aiida.engine import calcfunction
-from aiida.plugins import DataFactory
 
-PreProcessData = DataFactory('phonopy.preprocess')
-PhonopyData = DataFactory('phonopy.phonopy')
+from aiida_phonopy.data import PhonopyData, PreProcessData
 
 __all__ = (
     'get_unitcell', 'get_primitive', 'get_supercell', 'get_supercells_with_displacements', 'get_displacements',
     'get_preprocess_with_new_displacements', 'generate_preprocess_data', 'generate_phonopy_data', 'CalcfunctionMixin'
 )
 
 
 @calcfunction
-def get_unitcell(preprocess_data: PreProcessData):
+def get_unitcell(preprocess_data: PreProcessData) -> orm.StructureData:
     """Get the unitcell of a PreProcessData as a StructureData."""
     structure_data = preprocess_data.get_unitcell()
     return structure_data
 
 
 @calcfunction
-def get_primitive(preprocess_data: PreProcessData):
+def get_primitive(preprocess_data: PreProcessData) -> orm.StructureData:
     """Get the primitive cell of a PreProcessData as a StructureData."""
     structure_data = preprocess_data.get_primitive_cell()
     return structure_data
 
 
 @calcfunction
-def get_supercell(preprocess_data: PreProcessData):
+def get_supercell(preprocess_data: PreProcessData) -> orm.StructureData:
     """Get the supercell (pristine) of a PreProcessData as a StructureData."""
     structure_data = preprocess_data.get_supercell()
     return structure_data
 
 
 @calcfunction
-def get_supercells_with_displacements(preprocess_data: PreProcessData):
+def get_supercells_with_displacements(preprocess_data: PreProcessData) -> dict[orm.StructureData]:
     """Get the supercells with displacements of a PreProcessData as a StructureData."""
     structures_data = preprocess_data.get_supercells_with_displacements()
     return structures_data
 
 
 @calcfunction
-def get_displacements(preprocess_data: PreProcessData):
+def get_displacements(preprocess_data: PreProcessData) -> orm.ArrayData:
     """Get the displacements of a PreProcessData as an ArrayData with array name `displacements`."""
     displacements = preprocess_data.get_displacements()
     the_displacements = orm.ArrayData()
     the_displacements.set_array('displacements', displacements)
 
     return the_displacements
 
 
 @calcfunction
 def generate_preprocess_data(
     structure: orm.StructureData,
-    displacement_generator=None,
-    supercell_matrix=None,
-    primitive_matrix=None,
-    symprec=None,
-    is_symmetry=None,
-    distinguish_kinds=None,
+    displacement_generator: orm.Dict | None = None,
+    supercell_matrix: orm.List | None = None,
+    primitive_matrix: orm.List | None = None,
+    symprec: orm.Float | None = None,
+    is_symmetry: orm.Float | None = None,
+    distinguish_kinds: orm.Bool | None = None,
 ):
-    """Returns a complete stored PreProcessData node.
+    """Return a complete stored PreProcessData node.
 
     :param structure: structure data node representing the unitcell
     :type structure: orm.StructureData
     :param displacement_generator: dictionary containing the info for generating the displacements
     :type displacement_generator: orm.Dict
     :param supercell_matrix: supercell matrix, defaults to diag(1,1,1)
     :type supercell_matrix: orm.List, optional
@@ -122,15 +122,17 @@
 
     preprocess.set_displacements(**displ_generator)
 
     return preprocess
 
 
 @calcfunction
-def get_preprocess_with_new_displacements(preprocess_data: PreProcessData, displacement_generator: orm.Dict):
+def get_preprocess_with_new_displacements(
+    preprocess_data: PreProcessData, displacement_generator: orm.Dict
+) -> PreProcessData:
     """Get a new PreProcessData from an old one from new displacement generator settings."""
     displacement_dataset = preprocess_data.generate_displacement_dataset(**displacement_generator.get_dict())
 
     preprocess = PreProcessData(
         structure=preprocess_data.get_unitcell(),
         supercell_matrix=preprocess_data.supercell_matrix,
         primitive_matrix=preprocess_data.primitive_matrix,
@@ -141,37 +143,41 @@
 
     preprocess.set_displacements_from_dataset(displacement_dataset)
 
     return preprocess
 
 
 @calcfunction
-def generate_phonopy_data(preprocess_data: PreProcessData, nac_parameters=None, forces_index=None, **forces_dict):
-    """Create a PhonopyData node from a PreProcess(Phonopy)Data node, storing forces and (optionally)
-        non-analytical constants.
-
-        `Forces` must be passed as **kwargs**, since we are calling a calcfunction with a variable
-        number of supercells forces.
-
-        :param nac_parameters: ArrayData containing 'dielectric' and 'born_charges' as arrays
-            with their correct shape
-        :param forces_index: Int if a TrajectoryData is given, in order to get the correct slice of the array.
-        :param forces_dict: dictionary of supercells forces as ArrayData stored as `forces`, each Data
-            labelled in the dictionary in the format `forces_{suffix}`.
-            The prefix is common and the suffix corresponds to the suffix number of the supercell with
-            displacement label given from the `get_supercells_with_displacements` method.
-
-            For example:
-                {'forces_1':ArrayData, 'forces_2':ArrayData}
-                <==>
-                {'supercell_1':StructureData, 'supercell_2':StructureData}
-                and forces in each ArrayData stored as 'forces',
-                i.e. ArrayData.get_array('forces') must not raise error
+def generate_phonopy_data(
+    preprocess_data: PreProcessData,
+    nac_parameters: orm.ArrayData | None = None,
+    forces_index: orm.Int | None = None,
+    **forces_dict
+) -> PhonopyData:
+    """Create a PhonopyData node from a PreProcess(Phonopy)Data node.
+
+    `Forces` must be passed as **kwargs**, since we are calling a calcfunction with a variable
+    number of supercells forces.
+
+    :param nac_parameters: ArrayData containing 'dielectric' and 'born_charges' as arrays
+        with their correct shape
+    :param forces_index: Int if a TrajectoryData is given, in order to get the correct slice of the array.
+    :param forces_dict: dictionary of supercells forces as ArrayData stored as `forces`, each Data
+        labelled in the dictionary in the format `forces_{suffix}`.
+        The prefix is common and the suffix corresponds to the suffix number of the supercell with
+        displacement label given from the `get_supercells_with_displacements` method.
+
+        For example:
+            {'forces_1':ArrayData, 'forces_2':ArrayData}
+            <==>
+            {'supercell_1':StructureData, 'supercell_2':StructureData}
+            and forces in each ArrayData stored as 'forces',
+            i.e. ArrayData.get_array('forces') must not raise error
 
-            .. note: if residual forces would be stored, label it with 0 as suffix.
+        .. note: if residual forces would be stored, label it with 0 as suffix.
     """
     prefix = 'forces'
 
     forces_0 = forces_dict.pop(f'{prefix}_0', None)
     # Setting the dictionary of forces
     dict_of_forces = {}
 
@@ -195,48 +201,54 @@
 
     return new_phonopy_data
 
 
 class CalcfunctionMixin:
     """Set of calcfunctions to be called from the aiida-phonopy DataTypes."""
 
-    def __init__(self, data_node):
+    def __init__(self, data_node: PreProcessData | PhonopyData):
+        """Instantiate the class."""
         self._data_node = data_node
 
-    def get_unitcell(self):
+    def get_unitcell(self) -> orm.StructureData:
         """Get the unitcell as a StructureData through a calfunction."""
         return get_unitcell(preprocess_data=self._data_node)
 
-    def get_primitive_cell(self):
+    def get_primitive_cell(self) -> orm.StructureData:
         """Get the primitive cell as a StructureData through a calfunction."""
         return get_primitive(preprocess_data=self._data_node)
 
-    def get_supercell(self):
+    def get_supercell(self) -> orm.StructureData:
         """Get the supercell (pristine) as a StructureData through a calfunction."""
         return get_supercell(preprocess_data=self._data_node)
 
-    def get_supercells_with_displacements(self):
+    def get_supercells_with_displacements(self) -> dict[orm.StructureData]:
         """Get the supercells with displacements as a StructureData through a calfunction."""
         return get_supercells_with_displacements(preprocess_data=self._data_node)
 
-    def get_displacements(self):
+    def get_displacements(self) -> orm.ArrayData:
         """Get the displacements as an ArrayData through a calfunction."""
         return get_displacements(preprocess_data=self._data_node)
 
-    def get_preprocess_with_new_displacements(self, displacement_generator: orm.Dict):
+    def get_preprocess_with_new_displacements(self, displacement_generator: orm.Dict) -> PreProcessData:
         """Create a PreProcessData node from a PreProcess/PhonopyData with a new set of displacements.
 
-        :param displacement_generator: a `storable` dictionary  """
+        :param displacement_generator: a `storable` dictionary
+        """
         return get_preprocess_with_new_displacements(
             preprocess_data=self._data_node, displacement_generator=displacement_generator
         )
 
-    def generate_phonopy_data(self, nac_parameters=None, forces_index=None, **forces_dict):
-        """Create a PhonopyData node from a PreProcess(Phonopy)Data node, storing forces and (optionally)
-        non-analytical constants.
+    def generate_phonopy_data(
+        self,
+        nac_parameters: orm.ArrayData | None = None,
+        forces_index: orm.Int | None = None,
+        **forces_dict
+    ) -> PhonopyData:
+        """Create a PhonopyData node from a PreProcess(Phonopy)Data node.
 
         `Forces` must be passed as **kwargs**, since we are calling a calcfunction with a variable
         number of supercells forces.
 
         :param nac_parameters: ArrayData containing 'dielectric' and 'born_charges' as arrays
             with their correct shape
         :param forces_index: Int if a TrajectoryData is given, in order to get the correct slice of the array.
```

### Comparing `aiida-phonopy-1.1.0/src/aiida_phonopy/calculations/functions/link_structures.py` & `aiida-phonopy-1.1.1a5/src/aiida_phonopy/calculations/functions/link_structures.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,28 @@
 # -*- coding: utf-8 -*-
 """Functions for linking PhonopyAtoms and StructureData."""
+from __future__ import annotations
+
+from aiida.orm import StructureData
+from phonopy.structure.cells import PhonopyAtoms
 
 __all__ = ('phonopy_atoms_to_structure', 'phonopy_atoms_from_structure', 'if_to_map')
 
 
-def phonopy_atoms_to_structure(cell, mapping=None):
+def phonopy_atoms_to_structure(
+    cell: PhonopyAtoms,
+    mapping: dict | None = None,
+    pbc: tuple[bool, bool, bool] = (True, True, True),
+) -> StructureData:
     """Return a StructureData from a PhonopyAtoms instance.
 
     :param cell: a PhonopyAtoms instance
     :param mapping: a number to kinds and symbols map, defaults to None
+    :param pbc: periodic boundary conditions in the three lattice directions
     """
-    from aiida import orm
-
     if mapping:
         numbers_to_kinds, numbers_to_symbols = mapping
         symbols = []
         positions = []
         names = []
         for number in cell.numbers:
             try:
@@ -27,29 +34,30 @@
     else:
         names = cell.symbols
         symbols = cell.symbols
 
     positions = cell.positions
     masses = cell.masses
 
-    structure = orm.StructureData(cell=cell.cell)
+    structure = StructureData(cell=cell.cell, pbc=pbc)
     for position, symbol, name, mass in zip(positions, symbols, names, masses):
         structure.append_atom(position=position, symbols=symbol, name=name, mass=mass)
 
     return structure
 
 
-def phonopy_atoms_from_structure(structure):
+def phonopy_atoms_from_structure(structure: StructureData) -> PhonopyAtoms:
     """Return a tuple containg the PhonopyAtoms and the mapping from a StructureData.
 
     :param structure: StructureData instance
-    :return: it returns a PhonopyAtoms istance and the mapping
+    :return: tuple with element:
+        * a :class:`~phonopy.structure.cells.PhonopyAtoms` istance
+        * mapping dictionary, with key:pair of the type int:str, string
+            referring to the custom atomic name
     """
-    from phonopy.structure.cells import PhonopyAtoms
-
     to_map = if_to_map(structure)
 
     if not to_map:  # when kind_names=symbols are used in the structure
         cell = PhonopyAtoms(
             symbols=[site.kind_name for site in structure.sites],
             positions=[site.position for site in structure.sites],
             cell=structure.cell,
@@ -89,15 +97,16 @@
 
     # Also here we start from 1.
     numbers_to_kinds = {i + 1: kind_names[i] for i in range(len(kind_names))}
 
     return (cell, [numbers_to_kinds, numbers_to_symbols])
 
 
-def if_to_map(structure):
+def if_to_map(structure: StructureData) -> bool:
     """Return a bool according whether kind names and symbols are the same.
 
     :param structure: StructureData instance
+
     :return: True if kind names different from symbols are used, False otherwise
     """
     check_kinds = [True for kind in structure.kinds if kind.name != kind.symbol]
     return bool(check_kinds)
```

### Comparing `aiida-phonopy-1.1.0/src/aiida_phonopy/calculations/phonopy.py` & `aiida-phonopy-1.1.1a5/src/aiida_phonopy/calculations/phonopy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 # -*- coding: utf-8 -*-
 """CalcJob for phonopy post-processing."""
-
 from aiida import orm
 from aiida.common import InputValidationError, datastructures
 from aiida.engine import CalcJob
 
 from aiida_phonopy.data import ForceConstantsData, PhonopyData
 from aiida_phonopy.utils.mapping import _lowercase_dict, _uppercase_dict
 
@@ -270,15 +269,15 @@
         """Prepare the calculation job for submission by transforming input nodes into input files.
 
         In addition to the input files being written to the sandbox folder, a `CalcInfo` instance will be returned that
         contains lists of files that need to be copied to the remote machine before job submission, as well as file
         lists that are to be retrieved after job completion.
 
         :param folder: a sandbox folder to temporarily write files on disk.
-        :return: :py:`~aiida.common.datastructures.CalcInfo` instance.
+        :return: :py:class:`~aiida.common.datastructures.CalcInfo` instance.
         """
         retrieve_list = []
         retrieve_temporary_list = []
         calculation_cmds = []
 
         if 'settings' in self.inputs:
             settings = _lowercase_dict(self.inputs.settings.get_dict(), dict_name='settings')
```

### Comparing `aiida-phonopy-1.1.0/src/aiida_phonopy/data/force_constants.py` & `aiida-phonopy-1.1.1a5/src/aiida_phonopy/data/force_constants.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,67 +1,88 @@
 # -*- coding: utf-8 -*-
-"""
-This module defines the class for force constants data.
-"""
+"""Module defining the class for force constants data."""
+from __future__ import annotations
+
+from aiida.orm import StructureData
 import numpy as np
+from phonopy.structure.cells import PhonopyAtoms
 
 from .raw import RawData
 
 
 class ForceConstantsData(RawData):  # pylint: disable=too-many-ancestors
-    """
-    This class provides the force constants data, along with the non-analytical constants
-    (optional) and the structure information (unitcell, supercell, ...).
+    """Self-contained class for force constants data and non-analytical constants.
+
+    It stores also the structure information (unitcell, supercell, ...), for a
+    complete transferable data type.
     """
 
     def __init__(
         self,
-        structure=None,
-        phonopy_atoms=None,
-        supercell_matrix=None,
-        primitive_matrix=None,
-        symprec=1e-05,
-        is_symmetry=True,
+        structure: StructureData | None = None,
+        phonopy_atoms: PhonopyAtoms | None = None,
+        supercell_matrix: list | None = None,
+        primitive_matrix: list | None = None,
+        symprec: float = 1e-05,
+        is_symmetry: bool = True,
+        distinguish_kinds: bool = True,
         **kwargs
     ):
+        """Instantiate the class.
+
+        The minimal input is to define either the `structure` or the `phonopy_atoms` input.
+        They cannot be specified at the same time.
+
+        :param structure: an :class:`~aiida.orm.StructureData` node
+        :param phononpy_atoms: a :class:`~phonopy.structure.cells.PhonopyAtoms` instance
+        :param supercell_matrix: a (3,3) shape array describing the supercell transformation
+        :param primitive_matrix: a (3,3) shape array describing the primite transformation
+        :param symprec: precision tollerance for symmetry analysis
+        :param is_symmetry: whether using symmetries
+        :distinguish_kinds: it stores a mapping between kinds and chemical symbols;
+            by default Phonopy does not support kind,
+            thus useful if in the input `structure` kinds are defined
+        :paramm kwargs: for internal use
+        """
         kwargs['structure'] = structure
         kwargs['phonopy_atoms'] = phonopy_atoms
         kwargs['supercell_matrix'] = supercell_matrix
         kwargs['primitive_matrix'] = primitive_matrix
         kwargs['symprec'] = symprec
         kwargs['is_symmetry'] = is_symmetry
+        kwargs['distinguish_kinds'] = distinguish_kinds
 
         super().__init__(**kwargs)
 
     def get_phonopy_instance(self, **kwargs):
-        """Return a `phonopy.Phonopy` object with force and nac parameters (if set).
+        """Return a :class:`~phonopy.Phonopy` object with force and nac parameters (if set).
 
         :param kwargs: see :func:`aiida_phonopy.data.preprocess.PreProcessData.get_phonopy_instance`
             * symmetrize_nac: whether or not to symmetrize the nac parameters
                 using point group symmetry; bool, defaults to self.is_symmetry
             * factor_nac: factor for non-analytical corrections;
                 float, defaults to Hartree*Bohr
         """
         ph_instance = super().get_phonopy_instance(**kwargs)
 
         if self.force_constants is not None:
-            ph_instance.set_force_constants(self.force_constants)
+            ph_instance.force_constants = self.force_constants
 
         return ph_instance
 
     @property
-    def force_constants(self):
+    def force_constants(self) -> np.ndarray:
         """Get force force constants matrix."""
         try:
             the_forces = self.get_array('force_constants')
         except KeyError:
             the_forces = None
         return the_forces
 
-    def set_force_constants(self, force_constants):
+    def set_force_constants(self, force_constants: list | np.ndarray):
         """Set force constants matrix.
 
         :param force_constants: array of force constants matrix in compact or full format
         :param type: (n_patom = atoms in primitive cell, n_satom =  atoms in supercell)
             * Compact format: (n_patom, n_satom, 3, 3)
             * Full format: (n_satom, n_satom, 3, 3)
```

### Comparing `aiida-phonopy-1.1.0/src/aiida_phonopy/data/phonopy.py` & `aiida-phonopy-1.1.1a5/src/aiida_phonopy/data/phonopy.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,56 +1,66 @@
 # -*- coding: utf-8 -*-
-"""
-This module defines the class which wraps the :func:`phonopy.Phonopy` main class.
-"""
+"""Module defining the class which wraps the :class:`phonopy.Phonopy` main class."""
+from __future__ import annotations
 
 import numpy as np
+from phonopy import Phonopy
 
 from .preprocess import PreProcessData
 
 
 class PhonopyData(PreProcessData):  # pylint: disable=too-many-ancestors
-    """
-    This class wraps the :class:`phonopy.Phonopy` class. It represents the final Data node status
-    of a frozen phonon calculaiton. It stores information regarding the pre-processing,
-    the displacements and forces dataset, and the (eventual) non-analytical constants.
+    """Class wrapping the :class:`phonopy.Phonopy` class.
+
+    It represents the final Data node status of a frozen phonon calculaiton.
+    It stores information regarding the pre-processing, the displacements and
+    forces dataset, and the (eventual) non-analytical constants.
 
     .. note: direct calculation of properties from this class is still not implemented.
         Use :class:`~aiida_phonopy.calculations.phonopy.PhonopyCalculation` for
         post-processing this data node, keeping the provenance and having the
         data produced in the correct data type.
     """
 
     def __init__(self, preprocess_data: PreProcessData, **kwargs):
+        """Instantiate the class.
 
-        if isinstance(preprocess_data, PreProcessData):
-            kwargs['structure'] = preprocess_data.get_unitcell()
-            kwargs['supercell_matrix'] = preprocess_data.supercell_matrix
-            kwargs['primitive_matrix'] = preprocess_data.primitive_matrix
-            kwargs['symprec'] = preprocess_data.symprec
-            kwargs['is_symmetry'] = preprocess_data.is_symmetry
-            kwargs['distinguish_kinds'] = preprocess_data.distinguish_kinds
-            super().__init__(**kwargs)
+        :param preprocess_data: a :class:`~aiida_phonopy.data.preprocess.PreProcessData` node
 
-            # super().set_displacements_from_dataset(preprocess_data.displacement_dataset)
-            dataset = preprocess_data.displacement_dataset
+        :raises TypeError: if the input is not of the correct type,
+        :raises ValueError: if the preprocess_data input does not contain displacement dataset
+        """
+        if not isinstance(preprocess_data, PreProcessData):
+            raise TypeError(f'incorrect type. Given type <{type(preprocess_data)}>, expected `PreProcessData')
 
-            if dataset is not None:
-                self.base.attributes.set('displacement_dataset', dataset)
-            else:
-                raise ValueError('cannot instantiate object without having displacement dataset set')
+        kwargs['structure'] = preprocess_data.get_unitcell()
+        kwargs['supercell_matrix'] = preprocess_data.supercell_matrix
+        kwargs['primitive_matrix'] = preprocess_data.primitive_matrix
+        kwargs['symprec'] = preprocess_data.symprec
+        kwargs['is_symmetry'] = preprocess_data.is_symmetry
+        kwargs['distinguish_kinds'] = preprocess_data.distinguish_kinds
+        super().__init__(**kwargs)
+
+        dataset = preprocess_data.displacement_dataset
+
+        if dataset is not None:
+            super().set_displacements_from_dataset(dataset)
+        else:
+            raise ValueError('cannot instantiate object without having displacement dataset set')
 
     def set_displacements(self):
+        """Set displacements cannot be accessed from PhonopyData."""
         raise RuntimeError('`displacements` cannot be changed for this Data')
 
     def set_displacements_from_dataset(self):
+        """Set displacements cannot be accessed from PhonopyData."""
         raise RuntimeError('`displacements` cannot be changed for this Data')
 
-    def get_phonopy_instance(self, subtract_residual_forces=None, **kwargs):
-        """Return a `phonopy.Phonopy` object with force and nac parameters (if set).
+    def get_phonopy_instance(self, subtract_residual_forces: bool | None = None, **kwargs) -> Phonopy:
+        """Return a :class:`~phonopy.Phonopy` object with forces and nac parameters (if set).
 
         :param subtract_residual_forces: whether or not subract residual forces (if set)
         :type subtract_residual_forces: bool, defaults to False
         :param kwargs: see :func:`aiida_phonopy.data.preprocess.PreProcessData.get_phonopy_instance`
             * symmetrize_nac: whether or not to symmetrize the nac parameters
                 using point group symmetry; bool, defaults to self.is_symmetry
             * factor_nac: factor for non-analytical corrections;
@@ -75,29 +85,29 @@
                 ph_instance.forces = the_forces
         except AttributeError:
             pass
 
         return ph_instance
 
     @property
-    def residual_forces(self):
+    def residual_forces(self) -> np.ndarray:
         """Get the residual forces calculated on the pristine (i.e. no displaced) supercell structure (if set).
 
         ..note: if you have specified the `forces_index` this will be used as well here.
         """
         try:
             if self.forces_index is not None:
                 the_forces = self.get_array('residual_forces')[self.forces_index]
             else:
                 the_forces = self.get_array('residual_forces')
         except KeyError:
             the_forces = None
         return the_forces
 
-    def set_residual_forces(self, forces):
+    def set_residual_forces(self, forces: list | np.ndarray):
         """Set the residual forces of the pristine supercell.
 
         :param forces: (atoms in supercell, 3) array shape
 
         :raises:
             * TypeError: if the format is not of the correct type
             * ValueError: if the format is not compatible
@@ -119,33 +129,45 @@
         else:
             if the_forces.shape == (natoms, 3):
                 self.set_array('residual_forces', the_forces)
             else:
                 raise ValueError('the array is not of the correct shape. Check also `forces_index`')
 
     @property
-    def forces(self):
+    def forces(self) -> np.ndarray:
         """Get forces for each supercell with displacements in the dataset as a unique array."""
         try:
             the_forces = self.get_array('forces')
+            return the_forces
         except (KeyError, AttributeError):
-            try:
-                nsupercells = len(self.displacements)
-                the_forces = np.zeros((nsupercells)).tolist()
-                for i in range(nsupercells):
-                    if self.forces_index is not None:
-                        the_forces[i] = self.get_array(f'forces_{i+1}')[self.forces_index]
-                    else:
-                        the_forces[i] = self.get_array(f'forces_{i+1}')
-                the_forces = np.array(the_forces)
-            except (KeyError, AttributeError):
-                the_forces = None
+            pass
+
+        if not 'forces_1' in self.get_arraynames():
+            return
+
+        try:
+            nsupercells = len(self.displacements)
+            the_forces = np.zeros((nsupercells)).tolist()
+            for i in range(nsupercells):
+                if self.forces_index is not None:
+                    the_forces[i] = self.get_array(f'forces_{i+1}')[self.forces_index]
+                else:
+                    the_forces[i] = self.get_array(f'forces_{i+1}')
+            the_forces = np.array(the_forces)
+        except (KeyError, AttributeError):
+            return
+
         return the_forces
 
-    def set_forces(self, sets_of_forces=None, dict_of_forces=None, forces_index=None):
+    def set_forces(
+        self,
+        sets_of_forces: list | np.ndarray | None = None,
+        dict_of_forces: dict | None = None,
+        forces_index: int | None = None
+    ):
         """Set forces per each supercell with displacement in the dataset.
 
         :param sets_of_forces: a set of atomic forces in displaced supercells. The order of
             displaced supercells has to match with that in displacement dataset.
         :param type: (supercells with displacements, atoms in supercell, 3) array shape
         :param dict_of_forces: dictionary of forces, in numpy.ndarray to store for each displacement.
             They keys for the dictionary must be passed as `forces_{num}`, where `num` corresponds to
@@ -191,21 +213,25 @@
         if forces_index is not None:
             if isinstance(forces_index, int):
                 self.base.attributes.set('forces_index', forces_index)
             else:
                 raise ValueError('index for forces must be an integer')
 
     @property
-    def forces_index(self):
+    def forces_index(self) -> int:
         """Return the index of the forces to use."""
         try:
             index = self.base.attributes.get('forces_index')
         except (KeyError, AttributeError):
             index = None
         return index
 
-    def set_forces_index(self, value):
-        """Set the `forces_index` attribute."""
+    def set_forces_index(self, value: int):
+        """Set the `forces_index` attribute.
+
+        This is used for tacking a particular array index of each single forces set.
+        This is useful to not duplicate data of e.g. trajectories.
+        """
         if isinstance(value, int):
             self.base.attributes.set('forces_index', value)
         else:
             raise ValueError('index for forces must be an integer')
```

### Comparing `aiida-phonopy-1.1.0/src/aiida_phonopy/data/preprocess.py` & `aiida-phonopy-1.1.1a5/src/aiida_phonopy/data/preprocess.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,57 +1,77 @@
 # -*- coding: utf-8 -*-
-"""
-This module defines the class for managing the frozen phonon structure.
-"""
+"""Module defining the class for managing the frozen phonon structure."""
+from __future__ import annotations
 
 import copy
 import json
 
 from aiida import orm
 import numpy as np
+from phonopy.structure.cells import PhonopyAtoms
 
 from aiida_phonopy.calculations.functions.link_structures import phonopy_atoms_to_structure
 
 from .raw import RawData
 
 
 class PreProcessData(RawData):  # pylint: disable=too-many-ancestors
-    """
+    """Class for pre-processing of frozen-phonon calculations.
+
     This class is designed for handling the pre-process information regarding
-    a frozen phonon calculation using `Phonopy`. These regard the unitcell structure,
+    a frozen phonon calculation using ``Phonopy``. These regard the unitcell structure,
     the supercell and primitive matrix, as well as other symmetry information.
     """
 
     def __init__(
         self,
-        structure=None,
-        phonopy_atoms=None,
-        supercell_matrix=None,
-        primitive_matrix=None,
-        symprec=1e-05,
-        is_symmetry=True,
-        distinguish_kinds=True,
+        structure: orm.StructureData | None = None,
+        phonopy_atoms: PhonopyAtoms | None = None,
+        supercell_matrix: list | None = None,
+        primitive_matrix: list | None = None,
+        symprec: float = 1e-05,
+        is_symmetry: bool = True,
+        distinguish_kinds: bool = True,
         **kwargs
     ):
+        """Instantiate the class.
+
+        The minimal input is to define either the `structure` or the `phonopy_atoms` input.
+        They cannot be specified at the same time.
+
+        :param structure: an :class:`~aiida.orm.StructureData` node
+        :param phononpy_atoms: a :class:`~phonopy.structure.cells.PhonopyAtoms` instance
+        :param supercell_matrix: a (3,3) shape array describing the supercell transformation
+        :param primitive_matrix: a (3,3) shape array describing the primite transformation
+        :param symprec: precision tollerance for symmetry analysis
+        :param is_symmetry: whether using symmetries
+        :distinguish_kinds: it stores a mapping between kinds and chemical symbols;
+            by default Phonopy does not support kind,
+            thus useful if in the input `structure` kinds are defined
+        :paramm kwargs: for internal use
+        """
         kwargs['structure'] = structure
         kwargs['phonopy_atoms'] = phonopy_atoms
         kwargs['supercell_matrix'] = supercell_matrix
         kwargs['primitive_matrix'] = primitive_matrix
         kwargs['symprec'] = symprec
         kwargs['is_symmetry'] = is_symmetry
         kwargs['distinguish_kinds'] = distinguish_kinds
 
         super().__init__(**kwargs)
 
         if self.__class__.__name__ == 'PreProcessData':
             self.set_displacements()
 
     @property
-    def displacement_dataset(self):
-        """Get the dispacement dataset in a readible format for phonopy."""
+    def displacement_dataset(self) -> dict | list | None:
+        """Get the dispacement dataset in a readible format for phonopy.
+
+        If not set, None is returned.
+        """
         message = '`displacement_dataset` stored in the database will be deprecated in v2.0.0'
         try:
             import warnings
             the_dataset = self.base.attributes.get('displacement_dataset')
             warnings.warn(message, DeprecationWarning)
             return the_dataset
         except AttributeError:
@@ -60,43 +80,43 @@
             if filename in self.base.repository.list_object_names():
                 with self.base.repository.open(filename, mode='rb') as handle:
                     return json.load(handle)
 
             return None
 
     @property
-    def displacements(self):
+    def displacements(self) -> list | dict:
         """Get the displacements to apply to the supercell.
 
         :returns: array with displacements; can be type-I or type-II (see :func:`phonopy.Phonopy.displacements`)
         """
         # For the time being, it is important to keep this implementation for the subclasses in the package,
         # otherwise a loop is generated (i.e. in the PhonopyData class, when setting the forces).
         ph = super().get_phonopy_instance()
         ph.dataset = self.displacement_dataset
-
         return ph.displacements
 
-    def get_displacements(self):
+    def get_displacements(self) -> list | dict:
         """Get the displacements to apply to the supercell."""
         return self.displacements
 
     def set_displacements(
         self,
-        distance=0.01,
-        is_plusminus='auto',
-        is_diagonal=True,
-        is_trigonal=False,
-        number_of_snapshots=None,
-        random_seed=None,
-        temperature=None,
-        cutoff_frequency=None,
+        distance: float = 0.01,
+        is_plusminus: str = 'auto',
+        is_diagonal: bool = True,
+        is_trigonal: bool = False,
+        number_of_snapshots: int | None = None,
+        random_seed: int | None = None,
+        temperature: float | None = None,
+        cutoff_frequency: float | None = None,
     ):
         """Set displacements for frozen phonon calculation.
-        (see `phonopy.Phonopy.generate_displacements` for a complete description of the inputs)
+
+        Refer to :py:func:`phonopy.Phonopy.generate_displacements` for a complete description of the inputs.
 
         .. note: temperature different from 0K can be given only when forces are set up.
         Thus, in the PreProcessData value different from zero will raise an error.
 
         :raises ValueError: if the inputs are not compatible with phonopy standards
         """
         self._if_can_modify()
@@ -114,25 +134,26 @@
                 cutoff_frequency=cutoff_frequency,
             )
         except ValueError as err:
             raise ValueError('one or more input types are not accepted') from err
 
         self._set_displacements(copy.deepcopy(ph.dataset))
 
-    def _set_displacements(self, value):
+    def _set_displacements(self, value: list | dict):
         """Put in the repository the displacement dataset in json format."""
         try:
             serialized = json.dumps(value)
         except TypeError:
             serialized = json.dumps(_serialize(value))
 
         self.base.repository.put_object_from_bytes(serialized.encode('utf-8'), 'displacement_dataset.json')
 
-    def set_displacements_from_dataset(self, dataset):
+    def set_displacements_from_dataset(self, dataset: dict | list):
         """Set displacements for frozen phonon calculation from a dataset.
+
         Useful if you want to set displacements from a previously random generated
         displacement dataset, or for setting dataset for self-consistent harmonic
         approximation.
 
         :param dataset: dictionary or array like (numpy or list), compatible with phonopy
 
         :raises ValueError: if the inputs are not compatible with phonopy standards
@@ -151,32 +172,35 @@
             except RuntimeError as err:
                 raise ValueError('non compatible format') from err
         else:
             raise ValueError('type not accepted')
 
         self._set_displacements(_serialize(copy.deepcopy(ph.dataset)))
 
-    def get_phonopy_instance(self, symmetrize_nac=None, factor_nac=None, **kwargs):
-        """Return a `phonopy.Phonopy` object with the current values.
+    def get_phonopy_instance(self, symmetrize_nac: bool = None, factor_nac: float | None = None, **kwargs):
+        """Return a :class:`~phonopy.Phonopy` object with the current values.
 
         :param symmetrize_nac: whether or not to symmetrize the nac parameters using point group symmetry.
         :type symmetrize_nac: bool, defaults to self.is_symmetry
         :param factor_nac: factor for non-analytical corrections
-        :type factor_nac: float,defaults to Hartree*Bohr
+        :type factor_nac: float, defaults to Hartree*Bohr
         :param kwargs: for internal use to set the primitive cell
         """
         ph = super().get_phonopy_instance(symmetrize_nac, factor_nac, **kwargs)
         if self.displacement_dataset is not None:
             ph.dataset = self.displacement_dataset
         return ph
 
-    def get_supercells_with_displacements(self):
+    def get_supercells_with_displacements(self) -> dict[orm.StructureData]:
         """Get the supercells with displacements for frozen phonon calculation.
 
-        :returns: dictionary with StructureData nodes (note: not stored), None if
+        .. note: this is not linking in the provenance the output structures.
+            Use the `self.calcfunctions.get_supercells_with_displacements` instead
+
+        :returns: dictionary with StructureData nodes, None if
             the displacement dataset has not been set
         """
         # Here we distinguish the kind, but only for mapping purposes.
         # This does not affect the number of displacements, since they
         # have been set with the correct flag of not distinguishing kinds.
         ph = self.get_phonopy_instance(**{'distinguish': True})
 
@@ -184,31 +208,32 @@
         mapping = self.kinds_map
         structures_dict = {}
 
         digits = len(str(len(supercells)))  # this will make the labels more nice to read
 
         for i, scell in enumerate(supercells):  # start from 1 - better choice for gathering forces
             label = f'supercell_{str(i + 1).zfill(digits)}'
-            structures_dict.update({label: phonopy_atoms_to_structure(scell, mapping)})
+            structures_dict.update({label: phonopy_atoms_to_structure(scell, mapping, self.pbc)})
 
         return structures_dict
 
     def generate_displacement_dataset(
         self,
-        distance=0.01,
-        is_plusminus='auto',
-        is_diagonal=True,
-        is_trigonal=False,
-        number_of_snapshots=None,
-        random_seed=None,
-        temperature=None,
-        cutoff_frequency=None,
+        distance: float = 0.01,
+        is_plusminus: str = 'auto',
+        is_diagonal: bool = True,
+        is_trigonal: bool = False,
+        number_of_snapshots: int | None = None,
+        random_seed: int | None = None,
+        temperature: float | None = None,
+        cutoff_frequency: float | None = None,
     ):
         """Return the displacement dataset for frozen phonon calculation.
-        (see `phonopy.Phonopy.generate_displacements` for a complete description of the inputs)
+
+        Refer to :py:func:`phonopy.Phonopy.generate_displacements` for a complete description of the inputs.
 
         :raises ValueError: if the inputs are not compatible with phonopy standards
         """
         ph = self.get_phonopy_instance()
 
         try:
             ph.generate_displacements(
@@ -232,22 +257,22 @@
         from aiida_phonopy.calculations.functions.data_utils import CalcfunctionMixin
 
         return CalcfunctionMixin(data_node=self)
 
     @staticmethod
     def generate_preprocess_data(
         structure: orm.StructureData,
-        displacement_generator=None,
-        supercell_matrix=None,
-        primitive_matrix=None,
-        symprec=None,
-        is_symmetry=None,
-        distinguish_kinds=None,
+        displacement_generator: dict | None = None,
+        supercell_matrix: list | None = None,
+        primitive_matrix: list | None = None,
+        symprec: float | None = None,
+        is_symmetry: bool | None = None,
+        distinguish_kinds: bool | None = None,
     ):
-        """Returns a complete stored PreProcessData node.
+        """Return a complete stored PreProcessData node.
 
         :param structure: structure data node representing the unitcell
         :type structure: orm.StructureData
         :param displacement_generator: dictionary containing the info for generating the displacements,
             defaults to phonopy default (see phonopy doc)
         :type displacement_generator: orm.Dict
         :param supercell_matrix: supercell matrix, defaults to diag(1,1,1)
@@ -256,14 +281,15 @@
         :type primitive_matrix: orm.List or orm.List, optional
         :param symprec: symmetry precision on atoms, defaults to 1e-5
         :type symprec: orm.Float, optional
         :param is_symmetry: if using space group symmetry, defaults to True
         :type is_symmetry: orm.Bool, optional
         :param distinguish_kinds: if distinguish names of same specie by symmetry, defaults to True
         :type distinguish_kinds: orm.Bool, optional
+
         :return: PreProcessData node
         """
         from aiida_phonopy.calculations.functions.data_utils import generate_preprocess_data
 
         kwargs = {}
 
         kwargs['structure'] = structure
@@ -285,15 +311,15 @@
 
         if distinguish_kinds is not None:
             kwargs['distinguish_kinds'] = distinguish_kinds
 
         return generate_preprocess_data(**kwargs)
 
 
-def _serialize(data):
+def _serialize(data: dict | list):
     """Serialize the data for displacement dataset, in case it contains numpy.ndarray."""
     serialized = copy.deepcopy(data)
 
     try:
         for key, value in data.items():
             serialized[key] = _serialize(value)
     except AttributeError:
```

### Comparing `aiida-phonopy-1.1.0/src/aiida_phonopy/data/raw.py` & `aiida-phonopy-1.1.1a5/src/aiida_phonopy/data/raw.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 # -*- coding: utf-8 -*-
-"""
-This module defines the base class for other Data types.
-"""
+"""Module defining the base class for other Data types."""
+from __future__ import annotations
 
 from copy import deepcopy
 
 from aiida import orm
 from aiida.orm.nodes.data import ArrayData
 import numpy as np
 from phonopy import Phonopy
@@ -13,15 +12,15 @@
 
 from aiida_phonopy.calculations.functions.link_structures import (
     phonopy_atoms_from_structure,
     phonopy_atoms_to_structure,
 )
 
 
-def _get_valid_matrix(matrix):
+def _get_valid_matrix(matrix: list | np.ndarray) -> np.ndarray:
     """Get and validate the `supercell_matrix` and `primitive_matrix` inputs.
 
     :param matrix: (3,1) or (3,3) shape array
     :type matrix: list, orm.List, numpy.ndarray
     :return: a (3,3) numpy.ndarray
     :raises:
         * TypeError: if it is not a valid array type and if the array does not contain only numbers
@@ -50,37 +49,52 @@
     valid_matrix = np.array(matrix)
     valid_matrix = np.diag(valid_matrix) if valid_matrix.shape == (3,) else valid_matrix
 
     return valid_matrix
 
 
 class RawData(ArrayData):  # pylint: disable=too-many-ancestors
-    """
-    This class contaings the base information for the other phonon and phonopy related data types,
-    i.e. the unitcell and its symmetry information, the supercell and primitive cell matrices.
-    """
+    """Base class containing the information for the other phonon related data types."""
 
     def __init__(
         self,
-        structure: orm.StructureData = None,
-        phonopy_atoms: PhonopyAtoms = None,
-        supercell_matrix: list = None,
-        primitive_matrix: list = None,
+        structure: orm.StructureData | None = None,
+        phonopy_atoms: PhonopyAtoms | None = None,
+        supercell_matrix: list | None = None,
+        primitive_matrix: list | None = None,
         symprec: float = 1e-05,
         is_symmetry: bool = True,
         distinguish_kinds: bool = True,
         **kwargs
     ):
+        """Instantiate the class.
+
+        The minimal input is to define either the `structure` or the `phonopy_atoms` input.
+        They cannot be specified at the same time.
+
+        :param structure: an :class:`~aiida.orm.StructureData` node
+        :param phononpy_atoms: a :class:`~phonopy.structure.cells.PhonopyAtoms` instance
+        :param supercell_matrix: a (3,3) shape array describing the supercell transformation
+        :param primitive_matrix: a (3,3) shape array describing the primite transformation
+        :param symprec: precision tollerance for symmetry analysis
+        :param is_symmetry: whether using symmetries
+        :distinguish_kinds: it stores a mapping between kinds and chemical symbols;
+            by default Phonopy does not support kind,
+            thus useful if in the input `structure` kinds are defined
+        :paramm kwargs: for internal use
+        """
         if structure and phonopy_atoms:
             raise ValueError('cannot pass `structure`and `phonopy_atoms` at the same time')
 
         if structure:
             phonopy_atoms_unitcell, mapping = phonopy_atoms_from_structure(structure)
+            pbc = structure.pbc
         elif phonopy_atoms:
             phonopy_atoms_unitcell, mapping = (phonopy_atoms, None)
+            pbc = [True, True, True]  # to be changed when Phonopy will support PBC
         else:
             raise ValueError('at least one between `structure` and `phonopy_atoms` must be specified')
 
         args = {
             'unitcell': phonopy_atoms_unitcell,
             'supercell_matrix': supercell_matrix,
             'primitive_matrix': primitive_matrix,
@@ -93,15 +107,15 @@
         except Exception as err:
             raise ValueError('one or more inputs are not consistent with the `phonopy.Phonopy` format') from err
 
         super().__init__(**kwargs)
 
         # Inizializing the class attributes.
         self._set_phonopy_version()
-        self._set_unitcell_attributes(phonopy_atoms=phonopy_atoms_unitcell)
+        self._set_unitcell_attributes(phonopy_atoms=phonopy_atoms_unitcell, pbc=pbc)
         self._set_kinds_map(mapping)
         self._set_distinguish_kinds(distinguish_kinds)  # crucial before setting symbols/names!
         self._set_symbols_and_names()
 
         if not supercell_matrix is None:
             self._set_supercell_matrix(supercell_matrix)
         else:
@@ -114,77 +128,92 @@
         # a phonopy instance is generated to get the primitive structure.
         if not primitive_matrix is None:
             self._set_primitive_matrix(primitive_matrix)
         else:
             self._set_primitive_matrix('auto')
 
     @property
-    def phonopy_version(self):
+    def phonopy_version(self) -> str:
         """Get the Phonopy version used."""
         return self.base.attributes.get('phonopy_version')
 
     def _set_phonopy_version(self):
         """Set the installed Phonopy version."""
         from phonopy.version import __version__ as the_phonopy_version
 
         self._if_can_modify()
         self.base.attributes.set('phonopy_version', the_phonopy_version)
 
     @property
-    def numbers(self):
-        """Get the `numbers` array of the atoms in the cell."""
+    def numbers(self) -> np.ndarray:
+        """Get the array corresponding to the atomic number in periodic table of the sturcture.
+
+        :return: (nat,) shaper array
+        """
         return self.base.attributes.get('numbers')
 
     @property
-    def masses(self):
-        """Get the `masses` array of the atoms in the cell."""
+    def masses(self) -> np.ndarray:
+        """Get the array of the atomic masses in the cell.
+
+        :return: (nat,) shape array
+        """
         return self.base.attributes.get('masses')
 
     @property
-    def positions(self):
-        """Get the `positions` array of the atoms in the cell."""
+    def positions(self) -> np.ndarray:
+        """Get the array of the atomic positions in the cell.
+
+        :return: (nat, 3) shape array
+        """
         return self.base.attributes.get('positions')
 
     @property
-    def cell(self):
-        """Get the `cell` of the structure."""
+    def cell(self) -> np.ndarray:
+        """Get the lattice matrix of the structure.
+
+        .. important: lattice vectors as rows of the matrix
+
+        :return: (3,3) shape array
+        """
         return self.base.attributes.get('cell')
 
     @property
-    def magnetic_moments(self):
+    def magnetic_moments(self) -> list[int]:
         """Get the `magnetic_moments` array of the atoms in the cell."""
         return self.base.attributes.get('magnetic_moments')
 
     @property
-    def symbols(self):
+    def symbols(self) -> list[str]:
         """Get the chemical `symbols` array of the atoms in the cell."""
         return self.base.attributes.get('symbols')
 
     @property
-    def pbc(self):
+    def pbc(self) -> tuple[int, int, int]:
         """Get the periodic boundary conditions."""
         return self.base.attributes.get('pbc')
 
     @property
-    def names(self):
+    def names(self) -> list[str]:
         """Get the custom `names` array of the atoms in the cell.
 
-        .. note: if no special names are specified, this will be equal to `symbols`."""
+        .. note: if no special names are specified, this will be equal to `symbols`.
+        """
         return self.base.attributes.get('names')
 
-    def _set_unitcell_attributes(self, phonopy_atoms: PhonopyAtoms):
+    def _set_unitcell_attributes(self, phonopy_atoms: PhonopyAtoms, pbc: tuple[bool, bool, bool]):
         """Set the attributes for full reproducibility of the `PhonopyAtoms` class."""
         self._if_can_modify()
         self.base.attributes.set_many({
             'numbers': phonopy_atoms.numbers,
             'masses': phonopy_atoms.masses,
             'positions': phonopy_atoms.positions,
             'cell': phonopy_atoms.cell,
             'magnetic_moments': phonopy_atoms.magnetic_moments,
-            'pbc': [True, True, True],  # to change when modifying Phonopy
+            'pbc': pbc,
         })
 
     def _set_symbols_and_names(self):
         """Set the `symbols` and `names`."""
         if self.kinds_map:
             numbers_to_names, numbers_to_symbols = self.kinds_map
             symbols = []
@@ -200,37 +229,44 @@
             self.base.attributes.set('names', names)
         else:
             phonopy_atoms = self._get_phonopy_atoms_unitcell(distinguish_kinds=True)
             self.base.attributes.set('symbols', deepcopy(phonopy_atoms.symbols))
             self.base.attributes.set('names', deepcopy(phonopy_atoms.symbols))
 
     @property
-    def supercell_matrix(self):
-        """Get the `supercell_matrix`."""
+    def supercell_matrix(self) -> list:
+        """Get the `supercell_matrix`.
+
+        :return: a (3,3) shape array
+        """
         return self.base.attributes.get('supercell_matrix')
 
-    def _set_supercell_matrix(self, value):
+    def _set_supercell_matrix(self, value: list | np.ndarray):
         """Set the Phonopy supercell matrix.
 
         :param value: (3,3) or (3,1) shape array
         :type value: list, orm.List, numpy.ndarray
+
         :raises ModificationNotAllowed: if object is already stored
         """
         self._if_can_modify()
         the_supercell_matrix = _get_valid_matrix(value)
 
         self.base.attributes.set('supercell_matrix', deepcopy(the_supercell_matrix))
 
     @property
-    def primitive_matrix(self):
-        """Get the `primitive_matrix`."""
+    def primitive_matrix(self) -> list:
+        """Get the `primitive_matrix`.
+
+        :return: a (3,3) shape array
+        """
         return self.base.attributes.get('primitive_matrix')
 
-    def _set_primitive_matrix(self, value):
-        """Set the Phonopy primitive matrix.
+    def _set_primitive_matrix(self, value: list | np.ndarray):
+        """Set the primitive matrix.
 
         :param value: (3,3) or (3,1) shape array, or str
         :type value: list, orm.List, numpy.ndarray, str
         :raises ModificationNotAllowed: if object is already stored
         """
         self._if_can_modify()
 
@@ -238,20 +274,20 @@
             the_primitive_matrix = self.get_phonopy_instance(**{'primitive': value}).primitive_matrix
         else:
             the_primitive_matrix = _get_valid_matrix(value)
 
         self.base.attributes.set('primitive_matrix', deepcopy(the_primitive_matrix))
 
     @property
-    def symprec(self):
-        """Get the Phonopy symmetry tolerance (`symprec`)."""
+    def symprec(self) -> float:
+        """Get the tolerance for symmetry analysis."""
         return self.base.attributes.get('symprec')
 
-    def _set_symprec(self, value):
-        """Set the Phonopy symmetry tolerance (`symprec`).
+    def _set_symprec(self, value: float):
+        """Set the symmetry tolerance.
 
         :param value: tolerance for symmetry analysis. Check that you get
         the right symmetry of your structure before starting any calculation. Default is 1e-05.
         :type value: float
         :raises:
             * ModificationNotAllowed: if object is already stored
             * TypeError: if the input is not of type `float`
@@ -259,58 +295,66 @@
         self._if_can_modify()
         if not isinstance(value, float):
             raise ValueError('only `float` type is accepted.')
 
         self.base.attributes.set('symprec', deepcopy(value))
 
     @property
-    def is_symmetry(self):
-        """Get `is_symmetry` value."""
+    def is_symmetry(self) -> bool:
+        """Get `is_symmetry` value.
+
+        It refers to whether Phonopy will use symmetries to reduce the number of
+        displacements for frozen phonons.
+        """
         return self.base.attributes.get('is_symmetry')
 
-    def _set_is_symmetry(self, value):
-        """Set whether to use the symmetries. Use with care and if you know what your are doing.
+    def _set_is_symmetry(self, value: bool):
+        """Set whether to use the symmetries.
+
+        Use with care and if you know what your are doing.
 
         :param value: whether to use or not the symmetries. Deafault is True.
         :type value: bool
+
         :raises:
             * ModificationNotAllowed: if object is already stored
             * TypeError: if the input is not of type `bool`
         """
         self._if_can_modify()
         if not isinstance(value, bool):
             raise ValueError('only `bool` type is accepted.')
 
         self.base.attributes.set('is_symmetry', deepcopy(value))
 
     @property
-    def kinds_map(self):
+    def kinds_map(self) -> dict | None:
         """Get the map bewtween of the `numbers` and the `symbols` and `names`."""
         try:
             the_map = self.base.attributes.get('kinds_map')
         except AttributeError:
             the_map = None
         return the_map
 
-    def _set_kinds_map(self, value):
-        """Set the kind names map between the PhonopyAtoms unitcell and a reference
-        structure. This is needed since PhonopyAtoms does not support kind names.
+    def _set_kinds_map(self, value: dict):
+        """Set the kind names map between the PhonopyAtoms unitcell and a reference structure.
+
+        This is needed since PhonopyAtoms does not support kind names.
         This attribute allows to get proper `StructureData` supercells with displacements.
 
         :param value: tuple with two dictionaries (numbers_to_names, numbers_to_symbols)
         """
         self._if_can_modify()
         self.base.attributes.set('kinds_map', value)
 
     @property
-    def distinguish_kinds(self):
+    def distinguish_kinds(self) -> bool:
         """Get whether or not kinds with same chemical symbol will be distinguished by symmetry."""
         return self.base.attributes.get('distinguish_kinds')
 
-    def _set_distinguish_kinds(self, value):
+    def _set_distinguish_kinds(self, value: bool):
         """Set whether or not to distinguish kinds."""
         self._if_can_modify()
         if not isinstance(value, bool):
             raise ValueError('only `bool` type is accepted.')
 
         self.base.attributes.set('distinguish_kinds', value)
 
@@ -325,16 +369,18 @@
         if distinguish_kinds:
             kwargs.update({'numbers': self.numbers})
         else:
             kwargs.update({'symbols': self.symbols})
 
         return PhonopyAtoms(**kwargs)
 
-    def get_phonopy_instance(self, symmetrize_nac=None, factor_nac=None, **kwargs) -> Phonopy:
-        """Return a `phonopy.Phonopy` object with the current values.
+    def get_phonopy_instance(
+        self, symmetrize_nac: bool | None = None, factor_nac: float | None = None, **kwargs
+    ) -> Phonopy:
+        """Return a :py:class:`phonopy.Phonopy` object with the current values.
 
         :param symmetrize_nac: whether or not to symmetrize the nac parameters using point group symmetry.
         :type symmetrize_nac: bool, defaults to self.is_symmetry
         :param factor_nac: factor for non-analytical corrections
         :type factor_nac: float, defaults to Hartree*Bohr
         :param kwargs: for internal use to set the primitive cell
         """
@@ -388,30 +434,35 @@
 
         return ph_instance
 
     def get_unitcell(self) -> orm.StructureData:
         """Get the `unitcell` as StructureData (not stored)."""
         kwargs = {'distinguish': True}
         phonopy_instance = self.get_phonopy_instance(**kwargs).unitcell
-        return phonopy_atoms_to_structure(phonopy_instance, self.kinds_map)
+        return phonopy_atoms_to_structure(phonopy_instance, self.kinds_map, self.pbc)
 
     def get_primitive_cell(self) -> orm.StructureData:
         """Get the `primitive cell` as StructureData (not stored)."""
         kwargs = {'distinguish': True}
         phonopy_instance = self.get_phonopy_instance(**kwargs).primitive
-        return phonopy_atoms_to_structure(phonopy_instance, self.kinds_map)
+        return phonopy_atoms_to_structure(phonopy_instance, self.kinds_map, self.pbc)
 
     def get_supercell(self) -> orm.StructureData:
         """Get the pristine `supercell` as StructureData (not stored)."""
         kwargs = {'distinguish': True}
         phonopy_instance = self.get_phonopy_instance(**kwargs).supercell
-        return phonopy_atoms_to_structure(phonopy_instance, self.kinds_map)
+        return phonopy_atoms_to_structure(phonopy_instance, self.kinds_map, self.pbc)
 
-    def get_cells_mappings(self):
-        """Return a dictionary containing the mappings among unit-, super- and primitive cell"""
+    def get_cells_mappings(self) -> dict[dict[list]]:
+        """Return a dictionary containing the mappings among unit-, super- and primitive cell.
+
+        :return: dictionary with the following key:pair structure:
+            * primitive: {p2p_map: list, p2s_map: list, s2p_map: list}
+            * supercell: {u2u_map: list, u2s_map: list, s2u_map: list}
+        """
         ph = self.get_phonopy_instance()
 
         cells_maps = {
             'primitive': {
                 'p2p_map': ph.primitive.p2p_map,
                 'p2s_map': ph.primitive.p2s_map,
                 's2p_map': ph.primitive.s2p_map,
@@ -422,27 +473,27 @@
                 's2u_map': ph.supercell.s2u_map,
             },
         }
 
         return cells_maps
 
     @property
-    def dielectric(self):
-        """Get the `infinity` dielectric tensor (i.e. in the static field limit) in Cartesian coordinates."""
+    def dielectric(self) -> np.ndarray | None:
+        """Get the high-frequency dielectric tensor in Cartesian coordinates."""
         try:
             value = self.base.attributes.get('dielectric')
             value = np.array(value)
         except (KeyError, AttributeError):
             value = None
         return value
 
-    def set_dielectric(self, dielectric):
-        """Set the `infinity` dielectric tensor in Cartesian coordinates.
+    def set_dielectric(self, dielectric: list | np.ndarray):
+        """Set the high-frequency dielectric tensor in Cartesian coordinates.
 
-        .. note: it is assumed that the reference system is the same (if not the) of the primitive cell.
+        .. note: it is assumed that the reference system is the same of the primitive cell.
 
         :param dielectric: (3, 3) array like
 
         :raises:
             * TypeError: if the format is not compatible or of the correct type
             * ValueError: if the format is not compatible or of the correct type
         """
@@ -455,15 +506,15 @@
 
         if the_dielectric.shape == (3, 3):
             self.base.attributes.set('dielectric', the_dielectric.tolist())
         else:
             raise ValueError('the array is not of the correct shape')
 
     @property
-    def born_charges(self):
+    def born_charges(self) -> np.ndarray:
         """Get the effective Born charges tensors in Cartesian coordinates.
 
         ..note:
             The indecis refers to:
                 1. Atomic index.
                 2. Polarization index.
                 3. Atomic displacement index.
@@ -472,24 +523,25 @@
         """
         try:
             value = self.get_array('born_charges')
         except (KeyError, AttributeError):
             value = None
         return value
 
-    def set_born_charges(self, born_charges):
+    def set_born_charges(self, born_charges: list | np.ndarray):
         """Set the Born effective charge tensors in Cartesian coordinates.
 
         ..note:
             The indecis refers to:
                 1. Atomic index.
                 2. Polarization index.
                 3. Atomic displacement index.
 
         :param born_charges: (number of atoms in the primitive cell, 3, 3) shape array like
+
         :raises:
             * TypeError: if the format is not compatible or of the correct type
             * ValueError: if the format is not compatible or of the correct type
         """
         self._if_can_modify()
 
         if not isinstance(born_charges, (list, np.ndarray)):
@@ -500,16 +552,16 @@
         nprimitive_atoms = len(self.get_primitive_cell().sites)
 
         if the_born_charges.shape == (nprimitive_atoms, 3, 3):
             self.set_array('born_charges', the_born_charges)
         else:
             raise ValueError('the array is not of the correct shape')
 
-    def has_nac_parameters(self):
-        """Returns wheter or not the Data has non-analytical constants."""
+    def has_nac_parameters(self) -> bool:
+        """Return wheter or not the Data has non-analytical constants."""
         return (self.dielectric is not None and self.born_charges is not None)
 
     def _if_can_modify(self):
         """Check if the object is stored and raise an error if so. To use in every setter."""
         from aiida.common.exceptions import ModificationNotAllowed
 
         if self.is_stored:
```

### Comparing `aiida-phonopy-1.1.0/src/aiida_phonopy/parsers/base.py` & `aiida-phonopy-1.1.1a5/src/aiida_phonopy/parsers/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 # -*- coding: utf-8 -*-
-"""Defines a `Parser` base class for `aiida-phonopy`.
-
-All `Parser` implementations in `aiida-phonopy` must use this base class, not `aiida.parsers.Parser`.
-"""
+"""Defines a `Parser` base class for `aiida-phonopy`."""
+# All `Parser` implementations in `aiida-phonopy` must use this base class, not `aiida.parsers.Parser`.
 from aiida.parsers import Parser as _BaseParser
 
 __all__ = ('Parser',)
 
 
 class Parser(_BaseParser):  # pylint: disable=abstract-method
     """Custom `Parser` class for `aiida-phonopy` parser implementations."""
```

### Comparing `aiida-phonopy-1.1.0/src/aiida_phonopy/parsers/phonopy.py` & `aiida-phonopy-1.1.1a5/src/aiida_phonopy/parsers/phonopy.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # -*- coding: utf-8 -*-
 """Parsers of `PhonopyCalculation` output files."""
+from __future__ import annotations
 
 import os
 import traceback
 
 from aiida import orm
 import h5py
 import numpy as np
@@ -11,16 +12,16 @@
 
 from aiida_phonopy.calculations.phonopy import PhonopyCalculation
 from aiida_phonopy.utils.mapping import _uppercase_dict, get_logging_container
 
 from .base import Parser
 
 
-def file_opener(folder_path, filename):
-    """Function to open sistematically each expected output format."""
+def file_opener(folder_path: str, filename: str):
+    """Return a function to open different expected output format."""
     filename_path = os.path.join(folder_path, filename)
 
     if filename.endswith('hdf5'):
         return h5py.File(filename_path, 'r')
 
     return open(filename_path, mode='r', encoding='utf-8')
 
@@ -123,15 +124,15 @@
         # !FIXME!
         # Still to work out better. Good chances are that is not necessary...
         #
         # If something is still present and it has not been parsed, we raise error.
         # if filenames:
         #     self.exit_codes.ERROR_NOT_IMPLEMENTED_PARSER
 
-    def parse_stdout(self):
+    def parse_stdout(self) -> tuple:
         """Parse the stdout output file.
 
         :param parameters: the input parameters dictionary
         :param parsed_phonopy: the collected parsed data from the yaml phonopy output
         :return: raw parsed data
         """
         from .raw_parsers.phonopy import parse_stdout as parse_stdout_
@@ -168,15 +169,15 @@
             parameters = _uppercase_dict(self.node.inputs.parameters.get_dict(), dict_name='parameters')
             if 'FORCE_CONSTANTS' in parameters:
                 if str.upper(parameters['FORCE_CONSTANTS']) != 'WRITE':
                     exit_code_stdout = self.exit_codes.ERROR_BAD_INPUTS
 
         return parsed_data, logs, exit_code_stdout
 
-    def get_expected_filenames_keys(self):
+    def get_expected_filenames_keys(self) -> set:
         """Return the retrieve file keys (that map to the filenames outputs) depending on the tags in `parameters`."""
         retrieved_set = set()
         parameters = _uppercase_dict(self.node.inputs.parameters.get_dict(), dict_name='parameters')
 
         maps = {
             'band': {'BAND', 'BAND_PATHS', 'BAND_POINTS', 'BAND_LABELS', 'BAND_CONNECTION', 'BAND_INDICES'},
             'mesh': {'MESH', 'MP', 'MESH_NUMBERS', 'MP_SHIFT', 'GAMMA_CENTER', 'WRITE_MESH'},
@@ -210,61 +211,61 @@
         # Double check on mesh. The writing tag must have priority.
         if 'WRITE_MESH' in parameters.keys():
             if not parameters['WRITE_MESH']:
                 retrieved_set.remove('mesh')
 
         return retrieved_set
 
-    def parse_force_constants(self, filepath):
+    def parse_force_constants(self, filepath: str) -> orm.ArrayData:
         """Parse the `force_constants.hdf5` output file."""
         from phonopy.file_IO import read_force_constants_hdf5
 
         p2s_map = self._get_p2s_map()
         force_constants = read_force_constants_hdf5(filename=filepath, p2s_map=p2s_map)
 
         fc_array = orm.ArrayData()
         fc_array.set_array('force_constants', force_constants)
         fc_array.label = 'force_constants'
 
         return fc_array
 
-    def load_with_numpy(self, file):
+    def load_with_numpy(self, file: str) -> np.ndarray:
         """Load a txt file using numpy."""
         try:
             data = np.loadtxt(file)
         except ValueError:
             self.exit(self.exit_codes.ERROR_OUTPUT_NUMPY_LOAD)
         return data
 
-    def load_with_yaml(self, file):
+    def load_with_yaml(self, file: str) -> dict:
         """Load a yaml file using."""
         try:
             data = yaml.safe_load(file)
         except yaml.YAMLError:
             self.exit(self.exit_codes.ERROR_OUTPUT_YAML_LOAD)
         return data
 
-    def parse_yaml(self, file):
+    def parse_yaml(self, file: str) -> orm.Dict:
         """Parse a `.yaml` file and return it as a Dict."""
         data = self.load_with_yaml(file=file)
         return orm.Dict(data)
 
-    def parse_total_dos(self, file):
+    def parse_total_dos(self, file: str) -> orm.XyData:
         """Parse `total_dos.dat` output file."""
         data = self.load_with_numpy(file=file)
 
         total_dos = {'frequency_points': data[:, 0], 'total_dos': data[:, 1]}
         dos = orm.XyData()
         dos.set_x(total_dos['frequency_points'], 'Frequency', 'THz')
         dos.set_y(total_dos['total_dos'], 'DOS', '1/THz')
         dos.label = 'Total DOS'
 
         return dos
 
-    def parse_projected_dos(self, file):
+    def parse_projected_dos(self, file: str) -> orm.XyData:
         """Parse `projected_dos.dat` output file."""
         data = self.load_with_numpy(file=file)
 
         projected_dos = {'frequency_points': data[:, 0], 'projected_dos': data[:, 1:].T}
         pdos = orm.XyData()
         pdos_list = list(projected_dos['projected_dos'])
         pdos.set_x(projected_dos['frequency_points'], 'Frequency', 'THz')
@@ -277,15 +278,15 @@
                 '1/THz',
             ] * len(pdos_list),
         )
         pdos.label = 'Projected DOS'
 
         return pdos
 
-    def parse_thermal_properties(self, file):
+    def parse_thermal_properties(self, file: str) -> orm.XyData:
         """Parse the `thermal_properties.yaml`` output file."""
         data = self.load_with_yaml(file=file)
 
         thermal_properties = {
             'temperatures': [],
             'free_energy': [],
             'entropy': [],
@@ -312,15 +313,15 @@
             ['Helmholtz free energy', 'Entropy', 'Cv'],
             ['kJ/mol', 'J/K/mol', 'J/K/mol'],
         )
         tprops.label = 'Thermal properties'
 
         return tprops
 
-    def parse_band_structure(self, file, freqs_units='THz'):
+    def parse_band_structure(self, file: str, freqs_units: str = 'THz') -> orm.BandsData:
         """Parse the `band.hdf5`` output file.
 
         Expected keys are:
             * **nqpoint**: array with total number of q-points in the band structure, array(1,)
             * **frequency**: array of frequencies at each q-point; array(npath, segment_nqpoint, nband)
             * **label**: array of labels, two per each path; array(npath, 2)
             * **path**: number of q-points per path; array(npath, segment_nqpoint, qpoint/qposition(3,))
@@ -385,15 +386,15 @@
         # Setting the final bands structure data.
         band_structure.set_kpoints(np.array(qpoints))
         band_structure.set_bands(np.array(frequencies), units=freqs_units)
         band_structure.labels = final_labels
 
         return band_structure
 
-    def parse_qpoints(self, file, freqs_units='THz'):
+    def parse_qpoints(self, file: str, freqs_units: str = 'THz') -> orm.BandsData:
         """Parse the `mesh.hdf5`` and `qpoints.hdf5`` output files.
 
         Expected keys are:
             * **frequency**: array of frequencies at each q-point; array(nqpoint, nband)
             * **mesh**: qpoint mesh; array(3,)
             * **qpoint**: qpoints; array(nqpoint, 3)
             * **weight**: weight of qpoints; array(nqpoint,)
```

### Comparing `aiida-phonopy-1.1.0/src/aiida_phonopy/parsers/raw_parsers/phonopy.py` & `aiida-phonopy-1.1.1a5/src/aiida_phonopy/parsers/raw_parsers/phonopy.py`

 * *Files identical despite different names*

### Comparing `aiida-phonopy-1.1.0/src/aiida_phonopy/utils/mapping.py` & `aiida-phonopy-1.1.1a5/src/aiida_phonopy/utils/mapping.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,15 +18,16 @@
         'info': [],
         'warning': [],
         'error': [],
         'critical': [],
     })
 
 
-def _case_transform_dict(dictionary, dict_name, func_name, transform):
+def _case_transform_dict(dictionary: dict, dict_name: str, func_name, transform):
+    """Transform a dictionary to have the first keys capitalized or decapitalized."""
     from collections import Counter
 
     from aiida.common import InputValidationError
 
     if not isinstance(dictionary, dict):
         raise TypeError(f'{func_name} accepts only dictionaries as argument, got {type(dictionary)}')
     new_dict = dict((transform(str(k)), v) for k, v in dictionary.items())
@@ -38,13 +39,15 @@
             f'are repeated more than once when compared case-insensitively: {double_keys}.'
             'This is not allowed.'
         )
         raise InputValidationError(message)
     return new_dict
 
 
-def _lowercase_dict(dictionary, dict_name):
+def _lowercase_dict(dictionary: dict, dict_name: str):
+    """Transform a dictionary to have the first keys decapitalized."""
     return _case_transform_dict(dictionary, dict_name, '_lowercase_dict', str.lower)
 
 
-def _uppercase_dict(dictionary, dict_name):
+def _uppercase_dict(dictionary: dict, dict_name: str):
+    """Transform a dictionary to have the first keys capitalized."""
     return _case_transform_dict(dictionary, dict_name, '_uppercase_dict', str.upper)
```

### Comparing `aiida-phonopy-1.1.0/src/aiida_phonopy/utils/resources.py` & `aiida-phonopy-1.1.1a5/src/aiida_phonopy/utils/resources.py`

 * *Files identical despite different names*

### Comparing `aiida-phonopy-1.1.0/src/aiida_phonopy/workflows/phonopy.py` & `aiida-phonopy-1.1.1a5/src/aiida_phonopy/workflows/phonopy.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 # -*- coding: utf-8 -*-
 """Abstract workflow for automatic frozen phonons calculations."""
-
 from abc import ABCMeta
 
 from aiida import orm
 from aiida.engine import WorkChain
 
 from aiida_phonopy.data import ForceConstantsData, PhonopyData, PreProcessData
 
@@ -66,18 +65,18 @@
         return 'a structure data is required'
 
     if not given_inputs and not 'preprocess_data' in inputs:
         return 'at least one between `preprocess_data` and `structure` must be provided in input'
 
 
 class PhonopyWorkChain(WorkChain, metaclass=ABCMeta):
-    """
-    Abstract Workflow to compute automatically the force sets and force constants
-    of a given structure using the frozen phonons approach. Phonopy is used to produce
-    structures with displacements, while the forces are calculated with a quantum engine of choice.
+    """Abstract workflow for automated frozen phonons.
+
+    Phonopy is used to produce structures with displacements,
+    while the forces are calculated with a quantum engine of choice.
 
     This workchain is meant to be used as a base for other specific force calculato plugin workchains,
     or as an example on how to set a possible workchain/workflow. For this reason, the outline of
     this class is not defined, while it provides the inputs and a `setup` method, which can be used
     in a specific workflow outline. Ideally, the workflow would look like:
 
     1. Setup the preprocess data.
@@ -163,15 +162,15 @@
         * Note: we require in the input for generating the full phonopy data, to give the nac in the primitive cell.
         The primitive cell of phonopy will just rotate the lattice vectors, thus mantaining the Cartasian coordinate
         system. It can happen, though, that the unitcell is not the primitive cell of the system, meaning that the
         primitive cell will contain less atoms. We expect in input the nac computed on this number of atoms. If you
         want, for some reason, compute the nac on the unitcell, you will need to get the reduced nac.
         To do so, you can consider using a built-in function in phonopy, namely:
 
-        ```phonopy.structure.symmetry.elaborate_borns_and_epsilon```
+        :py:func:`phonopy.structure.symmetry.elaborate_borns_and_epsilon`
 
     """
 
     _ENABLED_DISPLACEMENT_GENERATOR_FLAGS = {
         'distance': [float],
         'is_plusminus': ['auto', float],
         'is_diagonal': [bool],
@@ -343,15 +342,15 @@
                 for key in value_dict.keys()
                 if not (type(value_dict[key]) in enabled_dict[key] or value_dict[key] in enabled_dict[key])
             ]
             if invalid_values:
                 return f'Displacement options must be of the correct type; got invalid values {invalid_values}.'
 
     def setup(self):
-        """Setup the workflow generating the PreProcessData."""
+        """Set up the workflow generating the PreProcessData."""
         if 'preprocess_data' in self.inputs:
             preprocess = self.inputs.preprocess_data
             if 'displacement_generator' in self.inputs:
                 preprocess = preprocess.calcfunctions.get_preprocess_with_new_displacements(
                     self.inputs.displacement_generator
                 )
         else:
```

### Comparing `aiida-phonopy-1.1.0/PKG-INFO` & `aiida-phonopy-1.1.1a5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiida-phonopy
-Version: 1.1.0
+Version: 1.1.1a5
 Summary: The official AiiDA plugin for Phonopy
 Keywords: aiida,phonopy,workflows
 Author-email: Lorenzo Bastonero <bastonero.lorenzo@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: AiiDA
@@ -34,15 +34,14 @@
 Provides-Extra: docs
 Provides-Extra: pre-commit
 Provides-Extra: tests
 
 # `aiida-phonopy`
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
 [![PyPI version](https://badge.fury.io/py/aiida-phonopy.svg)](https://badge.fury.io/py/aiida-phonopy)
-[![Build Status](https://github.com/aiida-phonopy/aiida-phonopy/workflows/aiida-phonopy/badge.svg?branch=develop&event=push)](https://github.com/aiida-phonopy/aiida-phonopy/actions)
 [![Docs status](https://readthedocs.org/projects/aiida-phonopy/badge)](http://aiida-phonopy.readthedocs.io/)
 
 This is the official AiiDA plugin for [Phonopy](https://phonopy.github.io/phonopy/index.html).
 
 ## Compatibility
 
 From `v0.7.0` this plugin does not support retro-compatibility with previous versions,
@@ -72,10 +71,10 @@
 
 ## Acknowlegements
 
 We acknowledge support from:
 * the [U Bremen Excellence Chairs](https://www.uni-bremen.de/u-bremen-excellence-chairs) program funded within the scope of the [Excellence Strategy of Germany’s federal and state governments](https://www.dfg.de/en/research_funding/excellence_strategy/index.html);
 * the [MAPEX](https://www.uni-bremen.de/en/mapex) Center for Materials and Processes.
 
-<img src="https://raw.githubusercontent.com/aiida-phonopy/aiida-phonopy/develop/docs/source/images/UBREMEN.png" width="300px" height="54px"/>
-<img src="https://raw.githubusercontent.com/aiida-phonopy/aiida-phonopy/develop/docs/source/images/MAPEX.jpg" width="300px" height="99px"/>
+<img src="https://raw.githubusercontent.com/aiida-phonopy/aiida-phonopy/main/docs/source/images/UBREMEN.png" width="300px" height="108px"/>
+<img src="https://raw.githubusercontent.com/aiida-phonopy/aiida-phonopy/main/docs/source/images/MAPEX.jpg" width="300px" height="99px"/>
```

