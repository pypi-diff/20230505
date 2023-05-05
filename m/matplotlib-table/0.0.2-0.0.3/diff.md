# Comparing `tmp/matplotlib_table-0.0.2.tar.gz` & `tmp/matplotlib_table-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "matplotlib_table-0.0.2.tar", last modified: Fri May  5 00:54:02 2023, max compression
+gzip compressed data, was "matplotlib_table-0.0.3.tar", last modified: Fri May  5 01:14:07 2023, max compression
```

## Comparing `matplotlib_table-0.0.2.tar` & `matplotlib_table-0.0.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 00:54:02.723529 matplotlib_table-0.0.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 00:54:02.715529 matplotlib_table-0.0.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 00:54:02.719529 matplotlib_table-0.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-05 00:53:53.000000 matplotlib_table-0.0.2/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-05 00:53:53.000000 matplotlib_table-0.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-05-05 00:53:53.000000 matplotlib_table-0.0.2/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 00:54:02.719529 matplotlib_table-0.0.2/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-05-05 00:53:53.000000 matplotlib_table-0.0.2/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-05 00:53:53.000000 matplotlib_table-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5451 2023-05-05 00:54:02.723529 matplotlib_table-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4745 2023-05-05 00:53:53.000000 matplotlib_table-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 00:54:02.719529 matplotlib_table-0.0.2/matplotlib_table.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5451 2023-05-05 00:54:02.000000 matplotlib_table-0.0.2/matplotlib_table.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-05-05 00:54:02.000000 matplotlib_table-0.0.2/matplotlib_table.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 00:54:02.000000 matplotlib_table-0.0.2/matplotlib_table.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-05 00:54:02.000000 matplotlib_table-0.0.2/matplotlib_table.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-05 00:54:02.000000 matplotlib_table-0.0.2/matplotlib_table.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-05 00:53:53.000000 matplotlib_table-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-05 00:53:53.000000 matplotlib_table-0.0.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-05-05 00:54:02.723529 matplotlib_table-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-05-05 00:53:53.000000 matplotlib_table-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 00:54:02.719529 matplotlib_table-0.0.2/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 00:53:53.000000 matplotlib_table-0.0.2/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 00:54:02.723529 matplotlib_table-0.0.2/src/mpltable/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-05 00:53:53.000000 matplotlib_table-0.0.2/src/mpltable/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4854 2023-05-05 00:53:53.000000 matplotlib_table-0.0.2/src/mpltable/options.py
--rw-r--r--   0 runner    (1001) docker     (123)    15340 2023-05-05 00:53:53.000000 matplotlib_table-0.0.2/src/mpltable/table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 00:54:02.723529 matplotlib_table-0.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-05 00:53:53.000000 matplotlib_table-0.0.2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-05-05 00:53:53.000000 matplotlib_table-0.0.2/tests/test_options.py
--rw-r--r--   0 runner    (1001) docker     (123)    34884 2023-05-05 00:53:53.000000 matplotlib_table-0.0.2/tests/test_table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 01:14:07.765665 matplotlib_table-0.0.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 01:14:07.757665 matplotlib_table-0.0.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 01:14:07.761665 matplotlib_table-0.0.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-05 01:13:58.000000 matplotlib_table-0.0.3/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-05 01:13:58.000000 matplotlib_table-0.0.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-05-05 01:13:58.000000 matplotlib_table-0.0.3/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 01:14:07.761665 matplotlib_table-0.0.3/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-05-05 01:13:58.000000 matplotlib_table-0.0.3/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-05 01:13:58.000000 matplotlib_table-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5451 2023-05-05 01:14:07.765665 matplotlib_table-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4745 2023-05-05 01:13:58.000000 matplotlib_table-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-05 01:13:58.000000 matplotlib_table-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-05 01:13:58.000000 matplotlib_table-0.0.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-05-05 01:14:07.769665 matplotlib_table-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-05 01:13:58.000000 matplotlib_table-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 01:14:07.761665 matplotlib_table-0.0.3/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 01:13:58.000000 matplotlib_table-0.0.3/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 01:14:07.765665 matplotlib_table-0.0.3/src/matplotlib_table.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5451 2023-05-05 01:14:07.000000 matplotlib_table-0.0.3/src/matplotlib_table.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-05-05 01:14:07.000000 matplotlib_table-0.0.3/src/matplotlib_table.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 01:14:07.000000 matplotlib_table-0.0.3/src/matplotlib_table.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-05 01:14:07.000000 matplotlib_table-0.0.3/src/matplotlib_table.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-05 01:14:07.000000 matplotlib_table-0.0.3/src/matplotlib_table.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 01:14:07.765665 matplotlib_table-0.0.3/src/mpltable/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-05 01:13:58.000000 matplotlib_table-0.0.3/src/mpltable/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4854 2023-05-05 01:13:58.000000 matplotlib_table-0.0.3/src/mpltable/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15340 2023-05-05 01:13:58.000000 matplotlib_table-0.0.3/src/mpltable/table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 01:14:07.765665 matplotlib_table-0.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-05 01:13:58.000000 matplotlib_table-0.0.3/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-05-05 01:13:58.000000 matplotlib_table-0.0.3/tests/test_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34884 2023-05-05 01:13:58.000000 matplotlib_table-0.0.3/tests/test_table.py
```

### Comparing `matplotlib_table-0.0.2/.vscode/settings.json` & `matplotlib_table-0.0.3/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `matplotlib_table-0.0.2/LICENSE` & `matplotlib_table-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `matplotlib_table-0.0.2/PKG-INFO` & `matplotlib_table-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matplotlib_table
-Version: 0.0.2
+Version: 0.0.3
 Summary: Create prettier tables in matplotlib
 Home-page: https://github.com/dmoggles/matplotlib_table
 Author: Dmitry Mogilevsky
 Author-email: dmitry.mogilevsky@gmail.com
 License: MIT
 Classifier: 
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `matplotlib_table-0.0.2/README.md` & `matplotlib_table-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `matplotlib_table-0.0.2/matplotlib_table.egg-info/PKG-INFO` & `matplotlib_table-0.0.3/src/matplotlib_table.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matplotlib-table
-Version: 0.0.2
+Version: 0.0.3
 Summary: Create prettier tables in matplotlib
 Home-page: https://github.com/dmoggles/matplotlib_table
 Author: Dmitry Mogilevsky
 Author-email: dmitry.mogilevsky@gmail.com
 License: MIT
 Classifier: 
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `matplotlib_table-0.0.2/setup.cfg` & `matplotlib_table-0.0.3/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 [metadata]
 name = matplotlib_table
-version = 0.0.0
 author = Dmitry Mogilevsky
 author_email = dmitry.mogilevsky@gmail.com
 description = Create prettier tables in matplotlib
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/dmoggles/matplotlib_table
 license = MIT
```

### Comparing `matplotlib_table-0.0.2/setup.py` & `matplotlib_table-0.0.3/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,21 +5,21 @@
 config = configparser.ConfigParser()
 config.read("setup.cfg")
 metadata = config["metadata"]
 options = config["options"]
 # Define the setup() arguments
 setup(
     name=metadata["name"],
-    version=metadata["version"],
     author=metadata["author"],
     author_email=metadata["author_email"],
     description=metadata["description"],
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url=metadata["url"],
     license=metadata["license"],
-    packages=find_packages(),
+    packages=find_packages("src"),
+    package_dir={"": "src"},
     python_requires=">=3.6",
     install_requires=options["install_requires"],
     extras_require=config["options.extras_require"],
     classifiers=metadata["classifiers"].splitlines(),
 )
```

### Comparing `matplotlib_table-0.0.2/src/mpltable/options.py` & `matplotlib_table-0.0.3/src/mpltable/options.py`

 * *Files identical despite different names*

### Comparing `matplotlib_table-0.0.2/src/mpltable/table.py` & `matplotlib_table-0.0.3/src/mpltable/table.py`

 * *Files identical despite different names*

### Comparing `matplotlib_table-0.0.2/tests/test_options.py` & `matplotlib_table-0.0.3/tests/test_options.py`

 * *Files identical despite different names*

### Comparing `matplotlib_table-0.0.2/tests/test_table.py` & `matplotlib_table-0.0.3/tests/test_table.py`

 * *Files identical despite different names*

