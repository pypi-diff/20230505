# Comparing `tmp/depfinder-2.9.1.tar.gz` & `tmp/depfinder-2.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "depfinder-2.9.1.tar", last modified: Wed Jan  4 20:06:48 2023, max compression
+gzip compressed data, was "depfinder-2.9.2.tar", last modified: Mon Mar  6 01:43:38 2023, max compression
```

## Comparing `depfinder-2.9.1.tar` & `depfinder-2.9.2.tar`

### file list

```diff
@@ -1,54 +1,55 @@
-drwxrwxr-x   0 filipe    (1000) filipe    (1000)        0 2023-01-04 20:06:48.842275 depfinder-2.9.1/
--rw-r--r--   0 filipe    (1000) filipe    (1000)     1010 2022-06-23 17:57:22.000000 depfinder-2.9.1/.authors.yml
--rw-rw-r--   0 filipe    (1000) filipe    (1000)      222 2022-08-05 14:25:07.000000 depfinder-2.9.1/.coveragerc
--rw-rw-r--   0 filipe    (1000) filipe    (1000)       35 2022-09-05 18:33:20.000000 depfinder-2.9.1/.gitattributes
-drwxrwxr-x   0 filipe    (1000) filipe    (1000)        0 2023-01-04 20:06:48.834275 depfinder-2.9.1/.github/
-drwxrwxr-x   0 filipe    (1000) filipe    (1000)        0 2023-01-04 20:06:48.838275 depfinder-2.9.1/.github/workflows/
--rw-rw-r--   0 filipe    (1000) filipe    (1000)     1165 2022-09-05 18:36:38.000000 depfinder-2.9.1/.github/workflows/deploy-docs.yml
--rw-rw-r--   0 filipe    (1000) filipe    (1000)     1153 2022-09-05 18:36:38.000000 depfinder-2.9.1/.github/workflows/tests.yml
--rw-rw-r--   0 filipe    (1000) filipe    (1000)      861 2022-09-05 18:33:20.000000 depfinder-2.9.1/.gitignore
--rw-rw-r--   0 filipe    (1000) filipe    (1000)     1052 2022-09-05 18:32:27.000000 depfinder-2.9.1/.mailmap
--rw-r--r--   0 filipe    (1000) filipe    (1000)      217 2022-06-23 17:57:22.000000 depfinder-2.9.1/AUTHORS
--rw-r--r--   0 filipe    (1000) filipe    (1000)     1208 2022-06-23 17:57:22.000000 depfinder-2.9.1/CHANGELOG.rst
--rw-r--r--   0 filipe    (1000) filipe    (1000)     1539 2018-10-19 12:09:30.000000 depfinder-2.9.1/LICENSE
--rw-r--r--   0 filipe    (1000) filipe    (1000)       93 2018-10-19 12:09:30.000000 depfinder-2.9.1/MANIFEST.in
--rw-rw-r--   0 filipe    (1000) filipe    (1000)      334 2023-01-04 20:06:48.842275 depfinder-2.9.1/PKG-INFO
-drwxrwxr-x   0 filipe    (1000) filipe    (1000)        0 2023-01-04 20:06:48.846274 depfinder-2.9.1/depfinder/
--rw-rw-r--   0 filipe    (1000) filipe    (1000)     1797 2022-09-05 18:32:27.000000 depfinder-2.9.1/depfinder/__init__.py
--rw-rw-r--   0 filipe    (1000) filipe    (1000)      471 2023-01-04 20:06:48.846274 depfinder-2.9.1/depfinder/_version.py
--rw-rw-r--   0 filipe    (1000) filipe    (1000)     9226 2022-09-05 18:36:38.000000 depfinder-2.9.1/depfinder/cli.py
--rw-rw-r--   0 filipe    (1000) filipe    (1000)    13225 2022-09-05 18:36:38.000000 depfinder-2.9.1/depfinder/inspection.py
--rw-rw-r--   0 filipe    (1000) filipe    (1000)    11730 2022-07-21 23:48:31.000000 depfinder-2.9.1/depfinder/main.py
-drwxrwxr-x   0 filipe    (1000) filipe    (1000)        0 2023-01-04 20:06:48.842275 depfinder-2.9.1/depfinder/pkg_data/
--rw-r--r--   0 filipe    (1000) filipe    (1000)   485132 2022-06-23 17:57:22.000000 depfinder-2.9.1/depfinder/pkg_data/name_mapping.yml
--rw-r--r--   0 filipe    (1000) filipe    (1000)      579 2019-11-27 17:33:59.000000 depfinder-2.9.1/depfinder/pkg_data/pkg_data.yml
--rw-rw-r--   0 filipe    (1000) filipe    (1000)     6887 2022-09-05 18:36:38.000000 depfinder-2.9.1/depfinder/reports.py
--rw-rw-r--   0 filipe    (1000) filipe    (1000)      524 2023-01-04 20:03:31.000000 depfinder-2.9.1/depfinder/stdliblist.py
--rw-rw-r--   0 filipe    (1000) filipe    (1000)     1706 2022-09-05 18:36:38.000000 depfinder-2.9.1/depfinder/utils.py
-drwxrwxr-x   0 filipe    (1000) filipe    (1000)        0 2023-01-04 20:06:48.842275 depfinder-2.9.1/depfinder.egg-info/
--rw-rw-r--   0 filipe    (1000) filipe    (1000)      334 2023-01-04 20:06:48.000000 depfinder-2.9.1/depfinder.egg-info/PKG-INFO
--rw-rw-r--   0 filipe    (1000) filipe    (1000)      839 2023-01-04 20:06:48.000000 depfinder-2.9.1/depfinder.egg-info/SOURCES.txt
--rw-rw-r--   0 filipe    (1000) filipe    (1000)        1 2023-01-04 20:06:48.000000 depfinder-2.9.1/depfinder.egg-info/dependency_links.txt
--rw-rw-r--   0 filipe    (1000) filipe    (1000)       48 2023-01-04 20:06:48.000000 depfinder-2.9.1/depfinder.egg-info/entry_points.txt
--rw-rw-r--   0 filipe    (1000) filipe    (1000)       56 2023-01-04 20:06:48.000000 depfinder-2.9.1/depfinder.egg-info/requires.txt
--rw-rw-r--   0 filipe    (1000) filipe    (1000)       10 2023-01-04 20:06:48.000000 depfinder-2.9.1/depfinder.egg-info/top_level.txt
--rw-r--r--   0 filipe    (1000) filipe    (1000)     3840 2018-10-19 12:09:30.000000 depfinder-2.9.1/depfinder_usage.ipynb
-drwxrwxr-x   0 filipe    (1000) filipe    (1000)        0 2023-01-04 20:06:48.842275 depfinder-2.9.1/doc/
--rw-r--r--   0 filipe    (1000) filipe    (1000)     7421 2018-10-19 12:09:30.000000 depfinder-2.9.1/doc/Makefile
-drwxrwxr-x   0 filipe    (1000) filipe    (1000)        0 2023-01-04 20:06:48.842275 depfinder-2.9.1/doc/_templates/
--rw-rw-r--   0 filipe    (1000) filipe    (1000)      332 2022-09-05 18:36:38.000000 depfinder-2.9.1/doc/_templates/layout.html
--rw-rw-r--   0 filipe    (1000) filipe    (1000)     9601 2022-09-05 18:36:38.000000 depfinder-2.9.1/doc/conf.py
--rw-rw-r--   0 filipe    (1000) filipe    (1000)       28 2022-09-05 18:36:38.000000 depfinder-2.9.1/doc/index.rst
--rw-r--r--   0 filipe    (1000) filipe    (1000)     6987 2018-10-19 12:09:30.000000 depfinder-2.9.1/doc/make.bat
-drwxrwxr-x   0 filipe    (1000) filipe    (1000)        0 2023-01-04 20:06:48.842275 depfinder-2.9.1/news/
--rw-r--r--   0 filipe    (1000) filipe    (1000)      173 2022-06-23 17:57:22.000000 depfinder-2.9.1/news/TEMPLATE
--rw-rw-r--   0 filipe    (1000) filipe    (1000)      244 2022-07-21 23:48:31.000000 depfinder-2.9.1/news/imp.rst
--rw-rw-r--   0 filipe    (1000) filipe    (1000)     5737 2022-09-05 18:36:38.000000 depfinder-2.9.1/readme.rst
--rw-rw-r--   0 filipe    (1000) filipe    (1000)       63 2022-09-05 18:36:38.000000 depfinder-2.9.1/requirements-dev.txt
--rw-rw-r--   0 filipe    (1000) filipe    (1000)       52 2022-09-05 18:36:38.000000 depfinder-2.9.1/requirements.txt
--rw-rw-r--   0 filipe    (1000) filipe    (1000)      477 2022-09-05 18:32:27.000000 depfinder-2.9.1/rever.xsh
--rwxrwxr-x   0 filipe    (1000) filipe    (1000)      425 2023-01-04 20:06:17.000000 depfinder-2.9.1/run_tests.py
--rw-rw-r--   0 filipe    (1000) filipe    (1000)      251 2023-01-04 20:06:48.842275 depfinder-2.9.1/setup.cfg
--rw-rw-r--   0 filipe    (1000) filipe    (1000)      673 2022-09-05 18:33:20.000000 depfinder-2.9.1/setup.py
--rw-rw-r--   0 filipe    (1000) filipe    (1000)    15513 2022-09-05 18:36:38.000000 depfinder-2.9.1/test.py
--rw-rw-r--   0 filipe    (1000) filipe    (1000)    65709 2022-09-05 18:36:38.000000 depfinder-2.9.1/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 01:43:38.538149 depfinder-2.9.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-03-06 01:43:21.000000 depfinder-2.9.2/.authors.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-03-06 01:43:21.000000 depfinder-2.9.2/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 01:43:38.534149 depfinder-2.9.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-03-06 01:43:21.000000 depfinder-2.9.2/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 01:43:38.534149 depfinder-2.9.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-03-06 01:43:21.000000 depfinder-2.9.2/.github/workflows/deploy-docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-03-06 01:43:21.000000 depfinder-2.9.2/.github/workflows/pypi.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-03-06 01:43:21.000000 depfinder-2.9.2/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-03-06 01:43:21.000000 depfinder-2.9.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-03-06 01:43:21.000000 depfinder-2.9.2/.mailmap
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-03-06 01:43:21.000000 depfinder-2.9.2/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-03-06 01:43:21.000000 depfinder-2.9.2/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-03-06 01:43:21.000000 depfinder-2.9.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-03-06 01:43:21.000000 depfinder-2.9.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6170 2023-03-06 01:43:38.538149 depfinder-2.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5663 2023-03-06 01:43:21.000000 depfinder-2.9.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 01:43:38.534149 depfinder-2.9.2/depfinder/
+-rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-03-06 01:43:21.000000 depfinder-2.9.2/depfinder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-06 01:43:38.000000 depfinder-2.9.2/depfinder/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9226 2023-03-06 01:43:21.000000 depfinder-2.9.2/depfinder/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13225 2023-03-06 01:43:21.000000 depfinder-2.9.2/depfinder/inspection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11730 2023-03-06 01:43:21.000000 depfinder-2.9.2/depfinder/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 01:43:38.538149 depfinder-2.9.2/depfinder/pkg_data/
+-rw-r--r--   0 runner    (1001) docker     (123)   485132 2023-03-06 01:43:21.000000 depfinder-2.9.2/depfinder/pkg_data/name_mapping.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-03-06 01:43:21.000000 depfinder-2.9.2/depfinder/pkg_data/pkg_data.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     6887 2023-03-06 01:43:21.000000 depfinder-2.9.2/depfinder/reports.py
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-03-06 01:43:21.000000 depfinder-2.9.2/depfinder/stdliblist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-03-06 01:43:21.000000 depfinder-2.9.2/depfinder/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 01:43:38.538149 depfinder-2.9.2/depfinder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6170 2023-03-06 01:43:38.000000 depfinder-2.9.2/depfinder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-03-06 01:43:38.000000 depfinder-2.9.2/depfinder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-06 01:43:38.000000 depfinder-2.9.2/depfinder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-03-06 01:43:38.000000 depfinder-2.9.2/depfinder.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-03-06 01:43:38.000000 depfinder-2.9.2/depfinder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-06 01:43:38.000000 depfinder-2.9.2/depfinder.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-06 01:43:38.000000 depfinder-2.9.2/depfinder.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-03-06 01:43:21.000000 depfinder-2.9.2/depfinder_usage.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 01:43:38.538149 depfinder-2.9.2/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)     7421 2023-03-06 01:43:21.000000 depfinder-2.9.2/doc/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 01:43:38.538149 depfinder-2.9.2/doc/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-03-06 01:43:21.000000 depfinder-2.9.2/doc/_templates/layout.html
+-rw-r--r--   0 runner    (1001) docker     (123)     9548 2023-03-06 01:43:21.000000 depfinder-2.9.2/doc/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-03-06 01:43:21.000000 depfinder-2.9.2/doc/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6987 2023-03-06 01:43:21.000000 depfinder-2.9.2/doc/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 01:43:38.538149 depfinder-2.9.2/news/
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-03-06 01:43:21.000000 depfinder-2.9.2/news/TEMPLATE
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-03-06 01:43:21.000000 depfinder-2.9.2/news/imp.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-03-06 01:43:21.000000 depfinder-2.9.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-03-06 01:43:21.000000 depfinder-2.9.2/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-03-06 01:43:21.000000 depfinder-2.9.2/requirements.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      425 2023-03-06 01:43:21.000000 depfinder-2.9.2/run_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-03-06 01:43:38.538149 depfinder-2.9.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-03-06 01:43:21.000000 depfinder-2.9.2/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16649 2023-03-06 01:43:21.000000 depfinder-2.9.2/test.py
```

### Comparing `depfinder-2.9.1/.authors.yml` & `depfinder-2.9.2/.authors.yml`

 * *Files identical despite different names*

### Comparing `depfinder-2.9.1/.github/workflows/tests.yml` & `depfinder-2.9.2/.github/workflows/tests.yml`

 * *Files 13% similar despite different names*

```diff
@@ -1,45 +1,46 @@
 name: Tests
 
 on:
   pull_request:
   push:
-    branches: [master]
+    branches: [main]
 
 defaults:
   run:
     shell: bash -l {0}
 
 jobs:
   run:
     runs-on: ${{ matrix.os }}
     strategy:
       matrix:
-        python-version: ["3.6", "3.7", "3.8", "3.9", "3.10"]
+        python-version: ["3.6", "3.7", "3.8", "3.9", "3.10", "3.11"]
         os: [windows-latest, ubuntu-latest, macos-latest]
       fail-fast: false
 
     steps:
       - name: cancel previous runs
-        uses: styfle/cancel-workflow-action@0.10.0
+        uses: styfle/cancel-workflow-action@0.11.0
         with:
           access_token: ${{ github.token }}
 
       - uses: actions/checkout@v3
 
       - name: Setup Micromamba
-        uses: mamba-org/provision-with-micromamba@main
+        uses: mamba-org/provision-with-micromamba@v15
         with:
          environment-file: false
  
       - name: Python ${{ matrix.python-version }}
         run: |
           micromamba create --name TEST python=${{ matrix.python-version }} pip --file requirements-dev.txt --channel conda-forge
           micromamba activate TEST
-          python -m pip install -e .
+          pip install -e . --force-reinstall
+
       - name: test
         run: |
           micromamba activate TEST
           coverage run -m pytest -vrsx test.py
 
       - name: coverage
         run: |
```

### Comparing `depfinder-2.9.1/.gitignore` & `depfinder-2.9.2/.gitignore`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 parts/
 sdist/
 var/
 *.egg-info/
 .installed.cfg
 *.egg
 doc/_build
+_version.py
 
 # Installer logs
 pip-log.txt
 pip-delete-this-directory.txt
 
 # Unit test / coverage reports
 htmlcov/
```

### Comparing `depfinder-2.9.1/.mailmap` & `depfinder-2.9.2/.mailmap`

 * *Files identical despite different names*

### Comparing `depfinder-2.9.1/CHANGELOG.rst` & `depfinder-2.9.2/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `depfinder-2.9.1/LICENSE` & `depfinder-2.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `depfinder-2.9.1/depfinder/__init__.py` & `depfinder-2.9.2/depfinder/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,17 +23,19 @@
 # CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
 # SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
 # INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
 # CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
 # ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
 # POSSIBILITY OF SUCH DAMAGE.
 
-from ._version import get_versions
-__version__ = get_versions()['version']
-del get_versions
+try:
+    from ._version import __version__
+except ImportError:
+    __version__ = "unknown"
+
 
 from .inspection import parse_file
 
 from .main import (iterate_over_library, notebook_path_to_dependencies)
 
 import logging
 logger = logging.getLogger('depfinder')
```

### Comparing `depfinder-2.9.1/depfinder/cli.py` & `depfinder-2.9.2/depfinder/cli.py`

 * *Files identical despite different names*

### Comparing `depfinder-2.9.1/depfinder/inspection.py` & `depfinder-2.9.2/depfinder/inspection.py`

 * *Files identical despite different names*

### Comparing `depfinder-2.9.1/depfinder/main.py` & `depfinder-2.9.2/depfinder/main.py`

 * *Files identical despite different names*

### Comparing `depfinder-2.9.1/depfinder/pkg_data/name_mapping.yml` & `depfinder-2.9.2/depfinder/pkg_data/name_mapping.yml`

 * *Files identical despite different names*

### Comparing `depfinder-2.9.1/depfinder/pkg_data/pkg_data.yml` & `depfinder-2.9.2/depfinder/pkg_data/pkg_data.yml`

 * *Files identical despite different names*

### Comparing `depfinder-2.9.1/depfinder/reports.py` & `depfinder-2.9.2/depfinder/reports.py`

 * *Files identical despite different names*

### Comparing `depfinder-2.9.1/depfinder/stdliblist.py` & `depfinder-2.9.2/depfinder/stdliblist.py`

 * *Files identical despite different names*

### Comparing `depfinder-2.9.1/depfinder/utils.py` & `depfinder-2.9.2/depfinder/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -18,23 +18,46 @@
     SKETCHY_TYPES_TABLE[ast.Try] = 'try'
 except AttributeError:
     # python 2.7
     AST_TRY = [ast.TryExcept, ast.TryFinally]
     SKETCHY_TYPES_TABLE[ast.TryExcept] = 'try'
     SKETCHY_TYPES_TABLE[ast.TryFinally] = 'try'
 
+
+try:
+    # python 3.10+
+    AST_MATCH = [ast.match_case]
+    SKETCHY_TYPES_TABLE[ast.match_case] = 'match'
+except AttributeError:
+    # match/case does not exist before 3.10
+    AST_MATCH = []
+
+
 # this AST_QUESTIONABLE list comprises the various ways an import can be weird
 # 1. inside a try/except block
-# 2. inside a function
-# 3. inside a class
-AST_QUESTIONABLE = tuple(AST_TRY + [ast.FunctionDef, ast.ClassDef, ast.If])
+# 2. inside a function (async or otherwise)
+# 3. part of an if/elif/else
+# 4. inside a loop
+# 5. (for Python 3.10+) inside a match/case
+AST_QUESTIONABLE = tuple(AST_TRY + AST_MATCH + [
+    ast.FunctionDef,
+    ast.AsyncFunctionDef,
+    ast.If,
+    ast.While,
+    ast.For,
+    ast.AsyncFor,
+])
 SKETCHY_TYPES_TABLE[ast.FunctionDef] = 'function'
-SKETCHY_TYPES_TABLE[ast.ClassDef] = 'class'
+SKETCHY_TYPES_TABLE[ast.AsyncFunctionDef] = 'async-function'
 SKETCHY_TYPES_TABLE[ast.If] = 'if'
+SKETCHY_TYPES_TABLE[ast.While] = 'while'
+SKETCHY_TYPES_TABLE[ast.For] = 'for'
+SKETCHY_TYPES_TABLE[ast.AsyncFor] = 'async-for'
 del AST_TRY
+del AST_MATCH
 
 try:
     # Try and use the C extensions because they're faster
     yaml_loader = yaml.CSafeLoader
 except ImportError:
     # Fall back to the slower python implementation of the extensions because
     # that is what is available from the PyYAML pip package
```

### Comparing `depfinder-2.9.1/depfinder.egg-info/SOURCES.txt` & `depfinder-2.9.2/depfinder.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 .authors.yml
 .coveragerc
-.gitattributes
 .gitignore
 .mailmap
 AUTHORS
 CHANGELOG.rst
 LICENSE
 MANIFEST.in
+README.md
 depfinder_usage.ipynb
-readme.rst
+pyproject.toml
 requirements-dev.txt
 requirements.txt
-rever.xsh
 run_tests.py
 setup.cfg
 setup.py
 test.py
-versioneer.py
+.github/dependabot.yml
 .github/workflows/deploy-docs.yml
+.github/workflows/pypi.yaml
 .github/workflows/tests.yml
 depfinder/__init__.py
 depfinder/_version.py
 depfinder/cli.py
 depfinder/inspection.py
 depfinder/main.py
 depfinder/reports.py
@@ -29,14 +29,15 @@
 depfinder/utils.py
 depfinder.egg-info/PKG-INFO
 depfinder.egg-info/SOURCES.txt
 depfinder.egg-info/dependency_links.txt
 depfinder.egg-info/entry_points.txt
 depfinder.egg-info/requires.txt
 depfinder.egg-info/top_level.txt
+depfinder.egg-info/zip-safe
 depfinder/pkg_data/name_mapping.yml
 depfinder/pkg_data/pkg_data.yml
 doc/Makefile
 doc/conf.py
 doc/index.rst
 doc/make.bat
 doc/_templates/layout.html
```

### Comparing `depfinder-2.9.1/depfinder_usage.ipynb` & `depfinder-2.9.2/depfinder_usage.ipynb`

 * *Files identical despite different names*

### Comparing `depfinder-2.9.1/doc/Makefile` & `depfinder-2.9.2/doc/Makefile`

 * *Files identical despite different names*

### Comparing `depfinder-2.9.1/doc/conf.py` & `depfinder-2.9.2/doc/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,33 +27,35 @@
 # If your documentation needs a minimal Sphinx version, state it here.
 #needs_sphinx = '1.0'
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = [
+    'myst_parser',
     'sphinx.ext.autosummary',
     'sphinx.ext.autodoc',
     'sphinx.ext.viewcode',
     'sphinx.ext.todo',
     'numpydoc',
     'sphinx.ext.extlinks',
     'sphinx.ext.intersphinx',
     'sphinx.ext.napoleon',
 ]
+
+
 # map to the standard library
 intersphinx_mapping = {'python': ('https://docs.python.org/3.4', None)}
 numpydoc_show_class_members = False
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ['_templates']
 
 # The suffix(es) of source filenames.
 # You can specify multiple suffix as a list of string:
-# source_suffix = ['.rst', '.md']
-source_suffix = '.rst'
+source_suffix = [".rst", ".md"]
 
 # The encoding of source files.
 #source_encoding = 'utf-8-sig'
 
 # The master toctree document.
 master_doc = 'index'
 
@@ -62,18 +64,17 @@
 copyright = '2015, Eric Dill'
 author = 'Eric Dill'
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
-# The short X.Y version.
-version = 'v1.0'
-# The full version, including alpha/beta/rc tags.
-release = 'v1.0'
+import depfinder
+
+version = release = depfinder.__version__
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
 language = "en"
```

### Comparing `depfinder-2.9.1/doc/make.bat` & `depfinder-2.9.2/doc/make.bat`

 * *Files identical despite different names*

### Comparing `depfinder-2.9.1/readme.rst` & `depfinder-2.9.2/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,170 +1,177 @@
+# depfinder
 
+[![image](https://github.com/ericdill/depfinder/actions/workflows/tests.yml/badge.svg)](https://github.com/ericdill/depfinder/actions/workflows/tests.yml)
 
+[![image](http://codecov.io/github/ericdill/depfinder/coverage.svg?branch=main)](https://app.codecov.io/github/ericdill/depfinder?branch=main)
 
-.. depfinder documentation master file, created by
-   sphinx-quickstart on Wed Oct  7 22:23:01 2015.
-   You can adapt this file completely to your liking, but it should at least
-   contain the root `toctree` directive.
+-   [docs](https://ericdill.github.io/depfinder)
+-   [github repo](https://github.com/ericdill/depfinder)
 
-depfinder
-=========
-
-.. image:: https://github.com/ericdill/depfinder/actions/workflows/tests.yml/badge.svg
-   :target: https://github.com/ericdill/depfinder/actions/workflows/tests.yml
-.. image:: http://codecov.io/github/ericdill/depfinder/coverage.svg?branch=master
-   :target: http://codecov.io/github/ericdill/depfinder?branch=master
-
-- `docs <https://ericdill.github.io/depfinder>`_
-- `github repo <https://github.com/ericdill/depfinder>`_
-
-Installation
-------------
-
-``depfinder`` is on pypi. It is tested against Python 2.7 and 3.6-3.8.
-
-    pip install depfinder
-
-It is available via conda. ::
-
-    conda install -c conda-forge depfinder
-
-It is also via github. ::
-
-    git clone git@github.com:ericdill/depfinder
-    cd depfinder
-    python setup.py install
-
-or ::
-
-    pip install https://github.com/ericdill/depfinder/zipball/master#egg=depfinder
-
-
-
-Using depfinder
----------------
-
-::
-
-    $ depfinder -h
-    usage: depfinder [-h] [-y] [-V] [--no-remap] [-v] [-q] [-k KEY] [--conda]
-                 [--pdb]
-                 file_or_directory
-
-    Tool for inspecting the dependencies of your python project.
-
-    positional arguments:
-      file_or_directory  Valid options are a single python file, a single jupyter
-                         (ipython) notebook or a directory of files that include
-                         python files
-
-    optional arguments:
-      -h, --help         show this help message and exit
-      -y, --yaml         Output in syntactically valid yaml when true. Defaults to
-                         False
-      -V, --version      Print out the version of depfinder and exit
-      --no-remap         Do not remap the names of the imported libraries to their
-                         proper conda name
-      -v, --verbose      Enable debug level logging info from depfinder
-      -q, --quiet        Turn off all logging from depfinder
-      -k KEY, --key KEY  Select some or all of the output keys. Valid options are
-                         'required', 'optional', 'builtin', 'relative', 'all'.
-                         Defaults to 'all'
-      --conda            Format output so it can be passed as an argument to conda
-                         install or conda create
-      --pdb              Enable PDB debugging on exception
-
-Ok, great. That's the help output.  Not super helpful.  What does the output of
-depfinder look like when we run it on the source code for depfinder?
-
-::
-
-    $ depfinder depfinder
-    {'builtin': ['__future__',
-                 'argparse',
-                 'ast',
-                 'collections',
-                 'copy',
-                 'errno',
-                 'json',
-                 'logging',
-                 'os',
-                 'pprint',
-                 're',
-                 'subprocess',
-                 'sys'],
-     'relative': ['_version', 'main'],
-     'required': ['pyyaml', 'stdlib-list']}
-
-So, what do these things mean?  Well `builtin` are modules that are built in to
-the standard library.  `required` are modules that are not from the standard
-library or from within the `depfinder` package and `relative` are modules that
-are imported from one module to another within the `depfinder` source code.
-
-`Also see this notebook <https://github.com/ericdill/depfinder/blob/master/depfinder_usage.ipynb>`_
-
-
-Description
------------
-
-Find all the unique imports in your library, automatically, because who likes
-do it by hand?  `depfinder <https://github.com/ericdill/depfinder>`_ uses the `ast
-<https://docs.python.org/2/library/ast.html>`_ (Abstract Syntax Tree) module
-(and `more ast docs <https://greentreesnakes.readthedocs.io/en/latest/>`_) to find
-all :py:class:`ast.Try` and :py:class:`ast.ImportFrom` nodes.  These
-:py:class:`ast.Import` and :py:class:`ast.ImportFrom` nodes are then grouped
-according to the following categories, in order of decreasing precedence:
-
-* **relative**
-    The import is a relative import from within the same library
-
-* **builtin**
-    The import is built into the standard library, as determined by scraping the
-    official python docs for the builtins with `stdlib-list
-    <https://github.com/jackmaney/python-stdlib-list>`_
-
-* **questionable**
-    The import occurs inside any combination of
-
-    - :py:class:`ast.Try` (:py:class:`ast.TryExcept` on py27)
-    - :py:class:`ast.FunctionDef`
-    - :py:class:`ast.ClassDef`
+## Installation
+
+`depfinder` is on pypi. It is tested against Python 2.7 and 3.6-3.8.
+
+```
+pip install depfinder
+```
+
+It is available via conda.
+```
+conda install -c conda-forge depfinder
+```
+
+It is also via github.
+```
+git clone git@github.com:ericdill/depfinder
+cd depfinder
+python setup.py install
+```
+
+## Using depfinder
+
+```
+$ depfinder -h
+usage: depfinder [-h] [-y] [-V] [--no-remap] [-v] [-q] [-k KEY] [--conda]
+                [--pdb]
+                file_or_directory
+
+Tool for inspecting the dependencies of your python project.
+
+positional arguments:
+    file_or_directory  Valid options are a single python file, a single jupyter
+                        (ipython) notebook or a directory of files that include
+                        python files
+
+optional arguments:
+    -h, --help         show this help message and exit
+    -y, --yaml         Output in syntactically valid yaml when true. Defaults to
+                        False
+    -V, --version      Print out the version of depfinder and exit
+    --no-remap         Do not remap the names of the imported libraries to their
+                        proper conda name
+    -v, --verbose      Enable debug level logging info from depfinder
+    -q, --quiet        Turn off all logging from depfinder
+    -k KEY, --key KEY  Select some or all of the output keys. Valid options are
+                        'required', 'optional', 'builtin', 'relative', 'all'.
+                        Defaults to 'all'
+    --conda            Format output so it can be passed as an argument to conda
+                        install or conda create
+    --pdb              Enable PDB debugging on exception
+```
+
+Ok, great. That's the help output. Not super helpful. What does the
+output of depfinder look like when we run it on the source code for
+depfinder?
+```
+$ depfinder depfinder
+{'builtin': ['__future__',
+                'argparse',
+                'ast',
+                'collections',
+                'copy',
+                'errno',
+                'json',
+                'logging',
+                'os',
+                'pprint',
+                're',
+                'subprocess',
+                'sys'],
+    'relative': ['_version', 'main'],
+    'required': ['pyyaml', 'stdlib-list']}
+```
+So, what do these things mean? Well `builtin` are modules
+that are built in to the standard library. `required` are
+modules that are not from the standard library or from within the
+`depfinder` package and `relative` are modules
+that are imported from one module to another within the
+`depfinder` source code.
+
+Also see [this
+notebook](https://github.com/ericdill/depfinder/blob/master/depfinder_usage.ipynb)
+
+## Description
+
+Find all the unique imports in your library, automatically, because who
+likes do it by hand? [depfinder](https://github.com/ericdill/depfinder)
+uses the [ast](https://docs.python.org/2/library/ast.html) (Abstract
+Syntax Tree) module (and [more ast
+docs](https://greentreesnakes.readthedocs.io/en/latest/)) to find all
+:py`ast.Try`{.interpreted-text role="class"} and
+:py`ast.ImportFrom`{.interpreted-text role="class"} nodes. These
+:py`ast.Import`{.interpreted-text role="class"} and
+:py`ast.ImportFrom`{.interpreted-text role="class"} nodes are then
+grouped according to the following categories, in order of decreasing
+precedence:
+
+- **relative**
+  : The import is a relative import from within the same library
+- **builtin**
+  : The import is built into the standard library, as determined by scraping the
+    official python docs for the builtins with [stdlib-list](https://github.com/jackmaney/python-stdlib-list)
+- **questionable**
+  : The import occurs inside any combination of
+
+    - {py:class}`ast.Try` ({py:class}`ast.TryExcept` on py27)
+    - {py:class}`ast.FunctionDef`
+    - {py:class}`ast.ClassDef`
 
     The module may be importable without these imports, but the it will likely
     not have full functionality.
-
-* **required**
-    The import occurs at the top level of the module and will get executed
+- **required**
+  : The import occurs at the top level of the module and will get executed
     when the module is imported. These imports must be accounted for in an
     environment, or the module will not be importable.
 
-Testing
--------
+## Testing
 
-It has dependencies on, `stdlib-list
-<https://github.com/jackmaney/python-stdlib-list>`_ and `pyyaml
-<https://pyyaml.org/wiki/PyYAML>`_. I use ``stdlib-list`` to get the list of
-libraries built in to the standard library. These requirements can be installed
-via pip ::
+It has dependencies on,
+[stdlib-list](https://github.com/jackmaney/python-stdlib-list) and
+[pyyaml](https://pyyaml.org/wiki/PyYAML). I use `stdlib-list` to get the
+list of libraries built in to the standard library. These requirements
+can be installed via pip :
 
     pip install -r requirements.txt
 
-Also install the test-requiements ::
+Also install the test-requiements :
 
     pip install -r test-requirements.txt
 
-Then you can run the tests from the root of the git repository ::
+Then you can run the tests from the root of the git repository :
 
     coverage run run_tests.py
 
-API
-====
+## Releasing
+
+manual:
+1. create an annotated tag and push it to github. `git tag -a TAG and then `git push --tags`
+1. `git checkout TAG`
+1. `python -m build --sdist --wheel . --outdir dist`
+1. `twine check dist/*`
+1. `twine upload dist/* --verbose`
+
+# API
+
+```{eval-rst}
 .. currentmodule:: depfinder.main
+```
+
+```{eval-rst}
 .. autofunction:: get_imported_libs
+```
+
+```{eval-rst}
 .. autofunction:: iterate_over_library
+```
+
+```{eval-rst}
 .. autofunction:: simple_import_search
+```
+
+# IPython/Jupyter Notebook support
 
-IPython/Jupyter Notebook support
-================================
-``depfinder`` has support for v4 Jupyter notebooks.
+`depfinder` has support for v4 Jupyter notebooks.
 
+```{eval-rst}
 .. autofunction:: notebook_path_to_dependencies
+```
```

### Comparing `depfinder-2.9.1/test.py` & `depfinder-2.9.2/test.py`

 * *Files 6% similar despite different names*

```diff
@@ -46,27 +46,45 @@
     {'targets': {'required': ['foo'], 'builtin': ['os']},
      'code': """
 import foo
 try:
     import os
 except ImportError:
     # why would you put this in a try block??
-    pass"""},
-    {'targets': {'required': ['toplevel', 'toplevelfrom'],
-                 'questionable': ['function_inside_class',
-                                  'function_inside_class_from',
-                                  'inside_class',
-                                  'inside_class_from',
-                                  'inside_function',
-                                  'inside_function_from'],
-                 'relative': ['relative_function',
-                              'relative_function_inside_class',
-                              'relative_inside_class'],
-                 'builtin': ['os', 'pprint']},
-     'code': """
+        pass""",
+    },
+    {
+        "targets": {
+            "required": [
+                "toplevel",
+                "toplevelfrom",
+                "inside_class",
+                "inside_class_from",
+            ],
+            "questionable": [
+                "function_inside_class",
+                "function_inside_class_from",
+                "inside_for",
+                "inside_for_else",
+                "inside_function",
+                "inside_function_from",
+                "inside_async_function",
+                "inside_if",
+                "inside_else",
+                "inside_while",
+                "inside_nested_class",
+            ],
+            "relative": [
+                "relative_function",
+                "relative_function_inside_class",
+                "relative_inside_class",
+            ],
+            "builtin": ["os", "pprint"],
+        },
+        "code": """
 from toplevelfrom import some_function
 import toplevel
 def function():
     import inside_function
     from inside_function_from import another_function
     from .relative_function import random_function
 class Class:
@@ -75,19 +93,44 @@
     from .relative_inside_class import a_third_function
     import os
     def __init__(self):
         import function_inside_class
         from function_inside_class_from import some_function
         from .relative_function_inside_class import a_third_function
         import pprint
-"""},
 
-    {'targets':
-         {'questionable': ['chico', 'groucho', 'harpo']},
-     'code': """
+# Handle nesting properly. import in a class def should be treated as "required to import",
+# unless its inside any of the nodes that would render it questionable. This import _should_
+# land in the questionable section, so we want to make sure it does.
+if True:
+    class NestedClass:
+        import inside_nested_class
+# weird edge cases that we want to make sure end up sorted properly. This hits the "ast.While"
+for i in []:
+    import inside_for
+else:
+    import inside_for_else
+# import inside an async function. This hits the "ast.AsyncFunctionDef"
+async def async_function():
+    import inside_async_function
+# import inside an if block. This hits the "ast.If"
+foo = 'cat'
+if foo == 'cat':
+    import inside_if
+else:
+    import inside_else
+# import inside an if block. This hits the "ast.While"
+while True:
+    import inside_while
+    break
+""",
+    },
+    {
+        "targets": {"questionable": ["chico", "groucho", "harpo"]},
+        "code": """
 if this:
     import groucho
 elif that:
     import harpo
 else:
     import chico"""
      },
@@ -201,19 +244,19 @@
 def tester(import_list_dict, capsys):
     # http://nbviewer.ipython.org/gist/fperez/9716279
     for import_dict in import_list_dict:
         cell_code = [import_dict['code']]
         target = import_dict['targets']
         with write_notebook(cell_code) as fname:
             # parse the notebook!
-            assert target == main.notebook_path_to_dependencies(fname)
+            assert set(target) == set(main.notebook_path_to_dependencies(fname))
             # check the notebook cli
             _run_cli(path_to_check=fname)
             stdout, stderr = capsys.readouterr()
-            assert target == eval(stdout)
+            assert set(target) == set(eval(stdout))
 
 
 def test_multiple_code_cells(capsys):
     targets = defaultdict(set)
     import_list_dict = complex_imports + relative_imports + simple_imports
     # http://nbviewer.ipython.org/gist/fperez/9716279
     code_for_cells = []
```

