# Comparing `tmp/pyopp-0.0.7.tar.gz` & `tmp/pyopp-0.0.9.tar.gz`

## Comparing `pyopp-0.0.7.tar` & `pyopp-0.0.9.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 pyopp-0.0.7/src/pyopp/__init__.py
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 pyopp-0.0.7/src/pyopp/cli.py
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 pyopp-0.0.7/src/pyopp/enums.py
--rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 pyopp-0.0.7/src/pyopp/main.py
--rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 pyopp-0.0.7/src/pyopp/utils.py
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 pyopp-0.0.7/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 pyopp-0.0.7/LICENSE
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 pyopp-0.0.7/README.md
--rw-r--r--   0        0        0     1225 2020-02-02 00:00:00.000000 pyopp-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 pyopp-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 pyopp-0.0.9/src/pyopp/__init__.py
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 pyopp-0.0.9/src/pyopp/cli.py
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 pyopp-0.0.9/src/pyopp/enums.py
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 pyopp-0.0.9/src/pyopp/highlighter.py
+-rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 pyopp-0.0.9/src/pyopp/main.py
+-rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 pyopp-0.0.9/src/pyopp/utils.py
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 pyopp-0.0.9/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 pyopp-0.0.9/LICENSE
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 pyopp-0.0.9/README.md
+-rw-r--r--   0        0        0     1216 2020-02-02 00:00:00.000000 pyopp-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     1443 2020-02-02 00:00:00.000000 pyopp-0.0.9/PKG-INFO
```

### Comparing `pyopp-0.0.7/src/pyopp/utils.py` & `pyopp-0.0.9/src/pyopp/utils.py`

 * *Files identical despite different names*

### Comparing `pyopp-0.0.7/LICENSE` & `pyopp-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyopp-0.0.7/pyproject.toml` & `pyopp-0.0.9/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pyopp"
-version = "0.0.7"
-description = "Over-powered print(er) for Python."
+version = "0.0.9"
+description = "P(Y)thon Over(P)owered Print"
 readme = "README.md"
 requires-python = ">=3.10.4"
 license = { text = 'MIT' }
 authors = [{ name = "Wayde Gilliam", email = "waydegilliam@gmail.com" }]
 keywords = ["python", "console", "pprint"]
 classifiers = [
   "Development Status :: 3 - Alpha",
@@ -24,15 +24,15 @@
   "Operating System :: MacOS",
   "Programming Language :: Python :: 3 :: Only",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Topic :: Software Development :: Libraries :: Python Modules",
   "Topic :: Internet",
 ]
-dependencies = ["pygments~=2.0.0"]
+dependencies = ["rich~=13.3.5"]
 
 [project.urls]
 Homepage = "https://github.com/waydegg/pyopp"
 Source = "https://github.com/waydegg/pyopp"
 
 [project.scripts]
 pyopp = "pyopp.cli:main"
```

