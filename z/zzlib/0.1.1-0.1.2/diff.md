# Comparing `tmp/zzlib-0.1.1.tar.gz` & `tmp/zzlib-0.1.2.tar.gz`

## Comparing `zzlib-0.1.1.tar` & `zzlib-0.1.2.tar`

### file list

```diff
@@ -1,53 +1,53 @@
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 zzlib-0.1.1/.gitattributes
--rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 zzlib-0.1.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 zzlib-0.1.1/MANIFEST.in
--rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 zzlib-0.1.1/Makefile
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 zzlib-0.1.1/requirements_dev.txt
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 zzlib-0.1.1/tox.ini
--rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 zzlib-0.1.1/.github/workflows/ci.yaml
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 zzlib-0.1.1/.github/workflows/lint.yaml
--rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 zzlib-0.1.1/.github/workflows/pypi.yaml
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 zzlib-0.1.1/.vscode/launch.json
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 zzlib-0.1.1/.vscode/settings.json
--rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 zzlib-0.1.1/tests/test_common.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 zzlib-0.1.1/zzlib/__init__.py
--rw-r--r--   0        0        0     7553 2020-02-02 00:00:00.000000 zzlib-0.1.1/zzlib/cls.py
--rw-r--r--   0        0        0     6970 2020-02-02 00:00:00.000000 zzlib-0.1.1/zzlib/func.py
--rw-r--r--   0        0        0     2331 2020-02-02 00:00:00.000000 zzlib-0.1.1/zzlib/mixin.py
--rw-r--r--   0        0        0    17334 2020-02-02 00:00:00.000000 zzlib-0.1.1/zzlib/utils.py
--rw-r--r--   0        0        0      880 2020-02-02 00:00:00.000000 zzlib-0.1.1/zzlib/bio/seq.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 zzlib-0.1.1/zzlib/cli/__init__.py
--rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 zzlib-0.1.1/zzlib/cli/progress.py
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 zzlib-0.1.1/zzlib/cli/click/__init__.py
--rw-r--r--   0        0        0     1209 2020-02-02 00:00:00.000000 zzlib-0.1.1/zzlib/cli/click/_common.py
--rw-r--r--   0        0        0     3382 2020-02-02 00:00:00.000000 zzlib-0.1.1/zzlib/cli/click/_shared_option.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 zzlib-0.1.1/zzlib/cli/typer/__init__.py
--rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 zzlib-0.1.1/zzlib/cli/typer/_async.py
--rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 zzlib-0.1.1/zzlib/cli/typer/_optional_value.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zzlib-0.1.1/zzlib/data/__init__.py
--rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 zzlib-0.1.1/zzlib/data/pandas.py
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 zzlib-0.1.1/zzlib/data/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zzlib-0.1.1/zzlib/dl/__init__.py
--rw-r--r--   0        0        0     1485 2020-02-02 00:00:00.000000 zzlib-0.1.1/zzlib/dl/device.py
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 zzlib-0.1.1/zzlib/log/__init__.py
--rw-r--r--   0        0        0     3604 2020-02-02 00:00:00.000000 zzlib-0.1.1/zzlib/log/chameleon.py
--rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 zzlib-0.1.1/zzlib/log/common.py
--rw-r--r--   0        0        0     5610 2020-02-02 00:00:00.000000 zzlib-0.1.1/zzlib/log/logging.py
--rw-r--r--   0        0        0     4680 2020-02-02 00:00:00.000000 zzlib-0.1.1/zzlib/log/loguru.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zzlib-0.1.1/zzlib/sch/__init__.py
--rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 zzlib-0.1.1/zzlib/sch/files.py
--rw-r--r--   0        0        0    13696 2020-02-02 00:00:00.000000 zzlib-0.1.1/zzlib/sch/structure.py
--rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 zzlib-0.1.1/zzlib/sch/utils.py
--rw-r--r--   0        0        0     2346 2020-02-02 00:00:00.000000 zzlib-0.1.1/zzlib/sch/workflow.py
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 zzlib-0.1.1/zzlib/shell/__init__.py
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 zzlib-0.1.1/zzlib/shell/env.py
--rw-r--r--   0        0        0     6019 2020-02-02 00:00:00.000000 zzlib-0.1.1/zzlib/shell/envmgr.py
--rw-r--r--   0        0        0     2554 2020-02-02 00:00:00.000000 zzlib-0.1.1/zzlib/shell/pathutils.py
--rw-r--r--   0        0        0     5706 2020-02-02 00:00:00.000000 zzlib-0.1.1/zzlib/shell/sandbox.py
--rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 zzlib-0.1.1/zzlib/shell/shell.py
--rw-r--r--   0        0        0    24137 2020-02-02 00:00:00.000000 zzlib-0.1.1/zzlib/shell/slurm.py
--rw-r--r--   0        0        0    11015 2020-02-02 00:00:00.000000 zzlib-0.1.1/zzlib/shell/subprocess.py
--rw-r--r--   0        0        0     3495 2020-02-02 00:00:00.000000 zzlib-0.1.1/.gitignore
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 zzlib-0.1.1/README.md
--rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 zzlib-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 zzlib-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 zzlib-0.1.2/.gitattributes
+-rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 zzlib-0.1.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 zzlib-0.1.2/MANIFEST.in
+-rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 zzlib-0.1.2/Makefile
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 zzlib-0.1.2/requirements_dev.txt
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 zzlib-0.1.2/tox.ini
+-rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 zzlib-0.1.2/.github/workflows/ci.yaml
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 zzlib-0.1.2/.github/workflows/lint.yaml
+-rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 zzlib-0.1.2/.github/workflows/pypi.yaml
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 zzlib-0.1.2/.vscode/launch.json
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 zzlib-0.1.2/.vscode/settings.json
+-rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 zzlib-0.1.2/tests/test_common.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 zzlib-0.1.2/zzlib/__init__.py
+-rw-r--r--   0        0        0     7553 2020-02-02 00:00:00.000000 zzlib-0.1.2/zzlib/cls.py
+-rw-r--r--   0        0        0     6970 2020-02-02 00:00:00.000000 zzlib-0.1.2/zzlib/func.py
+-rw-r--r--   0        0        0     2331 2020-02-02 00:00:00.000000 zzlib-0.1.2/zzlib/mixin.py
+-rw-r--r--   0        0        0    17334 2020-02-02 00:00:00.000000 zzlib-0.1.2/zzlib/utils.py
+-rw-r--r--   0        0        0      880 2020-02-02 00:00:00.000000 zzlib-0.1.2/zzlib/bio/seq.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 zzlib-0.1.2/zzlib/cli/__init__.py
+-rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 zzlib-0.1.2/zzlib/cli/progress.py
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 zzlib-0.1.2/zzlib/cli/click/__init__.py
+-rw-r--r--   0        0        0     1209 2020-02-02 00:00:00.000000 zzlib-0.1.2/zzlib/cli/click/_common.py
+-rw-r--r--   0        0        0     3382 2020-02-02 00:00:00.000000 zzlib-0.1.2/zzlib/cli/click/_shared_option.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 zzlib-0.1.2/zzlib/cli/typer/__init__.py
+-rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 zzlib-0.1.2/zzlib/cli/typer/_async.py
+-rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 zzlib-0.1.2/zzlib/cli/typer/_optional_value.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zzlib-0.1.2/zzlib/data/__init__.py
+-rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 zzlib-0.1.2/zzlib/data/pandas.py
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 zzlib-0.1.2/zzlib/data/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zzlib-0.1.2/zzlib/dl/__init__.py
+-rw-r--r--   0        0        0     1485 2020-02-02 00:00:00.000000 zzlib-0.1.2/zzlib/dl/device.py
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 zzlib-0.1.2/zzlib/log/__init__.py
+-rw-r--r--   0        0        0     3604 2020-02-02 00:00:00.000000 zzlib-0.1.2/zzlib/log/chameleon.py
+-rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 zzlib-0.1.2/zzlib/log/common.py
+-rw-r--r--   0        0        0     5610 2020-02-02 00:00:00.000000 zzlib-0.1.2/zzlib/log/logging.py
+-rw-r--r--   0        0        0     4680 2020-02-02 00:00:00.000000 zzlib-0.1.2/zzlib/log/loguru.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zzlib-0.1.2/zzlib/sch/__init__.py
+-rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 zzlib-0.1.2/zzlib/sch/files.py
+-rw-r--r--   0        0        0    13696 2020-02-02 00:00:00.000000 zzlib-0.1.2/zzlib/sch/structure.py
+-rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 zzlib-0.1.2/zzlib/sch/utils.py
+-rw-r--r--   0        0        0     2346 2020-02-02 00:00:00.000000 zzlib-0.1.2/zzlib/sch/workflow.py
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 zzlib-0.1.2/zzlib/shell/__init__.py
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 zzlib-0.1.2/zzlib/shell/env.py
+-rw-r--r--   0        0        0     6031 2020-02-02 00:00:00.000000 zzlib-0.1.2/zzlib/shell/envmgr.py
+-rw-r--r--   0        0        0     2554 2020-02-02 00:00:00.000000 zzlib-0.1.2/zzlib/shell/pathutils.py
+-rw-r--r--   0        0        0     5706 2020-02-02 00:00:00.000000 zzlib-0.1.2/zzlib/shell/sandbox.py
+-rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 zzlib-0.1.2/zzlib/shell/shell.py
+-rw-r--r--   0        0        0    24137 2020-02-02 00:00:00.000000 zzlib-0.1.2/zzlib/shell/slurm.py
+-rw-r--r--   0        0        0    11015 2020-02-02 00:00:00.000000 zzlib-0.1.2/zzlib/shell/subprocess.py
+-rw-r--r--   0        0        0     3495 2020-02-02 00:00:00.000000 zzlib-0.1.2/.gitignore
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 zzlib-0.1.2/README.md
+-rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 zzlib-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 zzlib-0.1.2/PKG-INFO
```

### Comparing `zzlib-0.1.1/.pre-commit-config.yaml` & `zzlib-0.1.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `zzlib-0.1.1/Makefile` & `zzlib-0.1.2/Makefile`

 * *Files identical despite different names*

### Comparing `zzlib-0.1.1/.github/workflows/ci.yaml` & `zzlib-0.1.2/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `zzlib-0.1.1/.github/workflows/pypi.yaml` & `zzlib-0.1.2/.github/workflows/pypi.yaml`

 * *Files identical despite different names*

### Comparing `zzlib-0.1.1/zzlib/cls.py` & `zzlib-0.1.2/zzlib/cls.py`

 * *Files identical despite different names*

### Comparing `zzlib-0.1.1/zzlib/func.py` & `zzlib-0.1.2/zzlib/func.py`

 * *Files identical despite different names*

### Comparing `zzlib-0.1.1/zzlib/mixin.py` & `zzlib-0.1.2/zzlib/mixin.py`

 * *Files identical despite different names*

### Comparing `zzlib-0.1.1/zzlib/utils.py` & `zzlib-0.1.2/zzlib/utils.py`

 * *Files identical despite different names*

### Comparing `zzlib-0.1.1/zzlib/bio/seq.py` & `zzlib-0.1.2/zzlib/bio/seq.py`

 * *Files identical despite different names*

### Comparing `zzlib-0.1.1/zzlib/cli/progress.py` & `zzlib-0.1.2/zzlib/cli/progress.py`

 * *Files identical despite different names*

### Comparing `zzlib-0.1.1/zzlib/cli/click/_common.py` & `zzlib-0.1.2/zzlib/cli/click/_common.py`

 * *Files identical despite different names*

### Comparing `zzlib-0.1.1/zzlib/cli/click/_shared_option.py` & `zzlib-0.1.2/zzlib/cli/click/_shared_option.py`

 * *Files identical despite different names*

### Comparing `zzlib-0.1.1/zzlib/cli/typer/_async.py` & `zzlib-0.1.2/zzlib/cli/typer/_async.py`

 * *Files identical despite different names*

### Comparing `zzlib-0.1.1/zzlib/cli/typer/_optional_value.py` & `zzlib-0.1.2/zzlib/cli/typer/_optional_value.py`

 * *Files identical despite different names*

### Comparing `zzlib-0.1.1/zzlib/data/pandas.py` & `zzlib-0.1.2/zzlib/data/pandas.py`

 * *Files identical despite different names*

### Comparing `zzlib-0.1.1/zzlib/dl/device.py` & `zzlib-0.1.2/zzlib/dl/device.py`

 * *Files identical despite different names*

### Comparing `zzlib-0.1.1/zzlib/log/chameleon.py` & `zzlib-0.1.2/zzlib/log/chameleon.py`

 * *Files identical despite different names*

### Comparing `zzlib-0.1.1/zzlib/log/common.py` & `zzlib-0.1.2/zzlib/log/common.py`

 * *Files identical despite different names*

### Comparing `zzlib-0.1.1/zzlib/log/logging.py` & `zzlib-0.1.2/zzlib/log/logging.py`

 * *Files identical despite different names*

### Comparing `zzlib-0.1.1/zzlib/log/loguru.py` & `zzlib-0.1.2/zzlib/log/loguru.py`

 * *Files identical despite different names*

### Comparing `zzlib-0.1.1/zzlib/sch/files.py` & `zzlib-0.1.2/zzlib/sch/files.py`

 * *Files identical despite different names*

### Comparing `zzlib-0.1.1/zzlib/sch/structure.py` & `zzlib-0.1.2/zzlib/sch/structure.py`

 * *Files identical despite different names*

### Comparing `zzlib-0.1.1/zzlib/sch/utils.py` & `zzlib-0.1.2/zzlib/sch/utils.py`

 * *Files identical despite different names*

### Comparing `zzlib-0.1.1/zzlib/sch/workflow.py` & `zzlib-0.1.2/zzlib/sch/workflow.py`

 * *Files identical despite different names*

### Comparing `zzlib-0.1.1/zzlib/shell/env.py` & `zzlib-0.1.2/zzlib/shell/env.py`

 * *Files identical despite different names*

### Comparing `zzlib-0.1.1/zzlib/shell/envmgr.py` & `zzlib-0.1.2/zzlib/shell/envmgr.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,15 +84,15 @@
     Args:
         env_sh: Init shell script to be sourced for loading environment.
     """
 
     load_cmd = None
 
     def __init__(self, env_sh: str = None, env: Dict[str, str] = None, inherit=False, **kw):
-        super().__init__(inherit, env, **kw)
+        super().__init__(env=env, inherit=inherit, **kw)
         env_sh = self.get_env_sh(env_sh)
         self.update(
             f"source {shlex.quote(str(env_sh))} >/dev/null",
             clean=True,
             fail=f"failed to load {self.name} init shell script",
         )
```

### Comparing `zzlib-0.1.1/zzlib/shell/pathutils.py` & `zzlib-0.1.2/zzlib/shell/pathutils.py`

 * *Files identical despite different names*

### Comparing `zzlib-0.1.1/zzlib/shell/sandbox.py` & `zzlib-0.1.2/zzlib/shell/sandbox.py`

 * *Files identical despite different names*

### Comparing `zzlib-0.1.1/zzlib/shell/shell.py` & `zzlib-0.1.2/zzlib/shell/shell.py`

 * *Files identical despite different names*

### Comparing `zzlib-0.1.1/zzlib/shell/slurm.py` & `zzlib-0.1.2/zzlib/shell/slurm.py`

 * *Files identical despite different names*

### Comparing `zzlib-0.1.1/zzlib/shell/subprocess.py` & `zzlib-0.1.2/zzlib/shell/subprocess.py`

 * *Files identical despite different names*

### Comparing `zzlib-0.1.1/.gitignore` & `zzlib-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `zzlib-0.1.1/pyproject.toml` & `zzlib-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `zzlib-0.1.1/PKG-INFO` & `zzlib-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zzlib
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python utils for structure-based computer-aided drug design
 Project-URL: Homepage, https://github.com/jackzzs-lab/zzlib
 Author-email: Zhesheng Zhou <zhouzzs@zju.edu.cn>
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Natural Language :: English
```

