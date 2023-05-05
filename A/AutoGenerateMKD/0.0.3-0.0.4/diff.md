# Comparing `tmp/AutoGenerateMKD-0.0.3.tar.gz` & `tmp/AutoGenerateMKD-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AutoGenerateMKD-0.0.3.tar", last modified: Thu May  4 17:15:43 2023, max compression
+gzip compressed data, was "AutoGenerateMKD-0.0.4.tar", last modified: Fri May  5 14:53:26 2023, max compression
```

## Comparing `AutoGenerateMKD-0.0.3.tar` & `AutoGenerateMKD-0.0.4.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 coseto     (501) staff       (20)        0 2023-05-04 17:15:43.772786 AutoGenerateMKD-0.0.3/
-drwxr-xr-x   0 coseto     (501) staff       (20)        0 2023-05-04 17:15:43.765979 AutoGenerateMKD-0.0.3/AutoGenerateMKD/
--rw-r--r--   0 coseto     (501) staff       (20)        0 2023-05-04 17:07:10.000000 AutoGenerateMKD-0.0.3/AutoGenerateMKD/__init__.py
--rw-r--r--   0 coseto     (501) staff       (20)     2007 2023-05-04 17:06:38.000000 AutoGenerateMKD-0.0.3/AutoGenerateMKD/main.py
-drwxr-xr-x   0 coseto     (501) staff       (20)        0 2023-05-04 17:15:43.769648 AutoGenerateMKD-0.0.3/AutoGenerateMKD.egg-info/
--rw-r--r--   0 coseto     (501) staff       (20)      302 2023-05-04 17:15:43.000000 AutoGenerateMKD-0.0.3/AutoGenerateMKD.egg-info/PKG-INFO
--rw-r--r--   0 coseto     (501) staff       (20)      408 2023-05-04 17:15:43.000000 AutoGenerateMKD-0.0.3/AutoGenerateMKD.egg-info/SOURCES.txt
--rw-r--r--   0 coseto     (501) staff       (20)        1 2023-05-04 17:15:43.000000 AutoGenerateMKD-0.0.3/AutoGenerateMKD.egg-info/dependency_links.txt
--rw-r--r--   0 coseto     (501) staff       (20)      153 2023-05-04 17:15:43.000000 AutoGenerateMKD-0.0.3/AutoGenerateMKD.egg-info/entry_points.txt
--rw-r--r--   0 coseto     (501) staff       (20)      349 2023-05-04 17:15:43.000000 AutoGenerateMKD-0.0.3/AutoGenerateMKD.egg-info/requires.txt
--rw-r--r--   0 coseto     (501) staff       (20)       41 2023-05-04 17:15:43.000000 AutoGenerateMKD-0.0.3/AutoGenerateMKD.egg-info/top_level.txt
--rw-r--r--   0 coseto     (501) staff       (20)     1054 2023-05-04 15:54:56.000000 AutoGenerateMKD-0.0.3/LICENSE
--rw-r--r--   0 coseto     (501) staff       (20)      302 2023-05-04 17:15:43.772297 AutoGenerateMKD-0.0.3/PKG-INFO
-drwxr-xr-x   0 coseto     (501) staff       (20)        0 2023-05-04 17:15:43.771150 AutoGenerateMKD-0.0.3/mkdocs_pagenav_generator/
--rw-r--r--   0 coseto     (501) staff       (20)        1 2023-05-04 16:28:20.000000 AutoGenerateMKD-0.0.3/mkdocs_pagenav_generator/__init__.py
--rw-r--r--   0 coseto     (501) staff       (20)      993 2023-05-04 16:28:20.000000 AutoGenerateMKD-0.0.3/mkdocs_pagenav_generator/plugin.py
--rw-r--r--   0 coseto     (501) staff       (20)     1371 2023-05-04 15:36:15.000000 AutoGenerateMKD-0.0.3/pyproject.toml
--rw-r--r--   0 coseto     (501) staff       (20)      225 2023-05-04 15:24:17.000000 AutoGenerateMKD-0.0.3/requirements.txt
--rw-r--r--   0 coseto     (501) staff       (20)       38 2023-05-04 17:15:43.772917 AutoGenerateMKD-0.0.3/setup.cfg
--rw-r--r--   0 coseto     (501) staff       (20)     1163 2023-05-04 17:15:24.000000 AutoGenerateMKD-0.0.3/setup.py
+drwxr-xr-x   0 coseto     (501) staff       (20)        0 2023-05-05 14:53:26.765801 AutoGenerateMKD-0.0.4/
+drwxr-xr-x   0 coseto     (501) staff       (20)        0 2023-05-05 14:53:26.759724 AutoGenerateMKD-0.0.4/AutoGenerateMKD/
+-rw-r--r--   0 coseto     (501) staff       (20)        1 2023-05-05 14:51:10.000000 AutoGenerateMKD-0.0.4/AutoGenerateMKD/__init__.py
+-rw-r--r--   0 coseto     (501) staff       (20)     1954 2023-05-05 14:52:11.000000 AutoGenerateMKD-0.0.4/AutoGenerateMKD/main.py
+drwxr-xr-x   0 coseto     (501) staff       (20)        0 2023-05-05 14:53:26.763218 AutoGenerateMKD-0.0.4/AutoGenerateMKD.egg-info/
+-rw-r--r--   0 coseto     (501) staff       (20)      302 2023-05-05 14:53:26.000000 AutoGenerateMKD-0.0.4/AutoGenerateMKD.egg-info/PKG-INFO
+-rw-r--r--   0 coseto     (501) staff       (20)      419 2023-05-05 14:53:26.000000 AutoGenerateMKD-0.0.4/AutoGenerateMKD.egg-info/SOURCES.txt
+-rw-r--r--   0 coseto     (501) staff       (20)        1 2023-05-05 14:53:26.000000 AutoGenerateMKD-0.0.4/AutoGenerateMKD.egg-info/dependency_links.txt
+-rw-r--r--   0 coseto     (501) staff       (20)      146 2023-05-05 14:53:26.000000 AutoGenerateMKD-0.0.4/AutoGenerateMKD.egg-info/entry_points.txt
+-rw-r--r--   0 coseto     (501) staff       (20)      349 2023-05-05 14:53:26.000000 AutoGenerateMKD-0.0.4/AutoGenerateMKD.egg-info/requires.txt
+-rw-r--r--   0 coseto     (501) staff       (20)       41 2023-05-05 14:53:26.000000 AutoGenerateMKD-0.0.4/AutoGenerateMKD.egg-info/top_level.txt
+-rw-r--r--   0 coseto     (501) staff       (20)     1054 2023-05-04 15:54:56.000000 AutoGenerateMKD-0.0.4/LICENSE
+-rw-r--r--   0 coseto     (501) staff       (20)      302 2023-05-05 14:53:26.765289 AutoGenerateMKD-0.0.4/PKG-INFO
+-rw-r--r--   0 coseto     (501) staff       (20)      314 2023-05-04 17:27:35.000000 AutoGenerateMKD-0.0.4/SUMMARY.md
+drwxr-xr-x   0 coseto     (501) staff       (20)        0 2023-05-05 14:53:26.764600 AutoGenerateMKD-0.0.4/mkdocs_pagenav_generator/
+-rw-r--r--   0 coseto     (501) staff       (20)        1 2023-05-04 16:28:20.000000 AutoGenerateMKD-0.0.4/mkdocs_pagenav_generator/__init__.py
+-rw-r--r--   0 coseto     (501) staff       (20)      993 2023-05-04 16:28:20.000000 AutoGenerateMKD-0.0.4/mkdocs_pagenav_generator/plugin.py
+-rw-r--r--   0 coseto     (501) staff       (20)     1371 2023-05-04 15:36:15.000000 AutoGenerateMKD-0.0.4/pyproject.toml
+-rw-r--r--   0 coseto     (501) staff       (20)      225 2023-05-04 15:24:17.000000 AutoGenerateMKD-0.0.4/requirements.txt
+-rw-r--r--   0 coseto     (501) staff       (20)       38 2023-05-05 14:53:26.765958 AutoGenerateMKD-0.0.4/setup.cfg
+-rw-r--r--   0 coseto     (501) staff       (20)     1156 2023-05-05 14:53:22.000000 AutoGenerateMKD-0.0.4/setup.py
```

### Comparing `AutoGenerateMKD-0.0.3/AutoGenerateMKD/main.py` & `AutoGenerateMKD-0.0.4/AutoGenerateMKD/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,54 +1,49 @@
 # @Author: E-NoR
 # @Date:   2022-11-30 02:05:53
 # @Last Modified by:   E-NoR
 # @Last Modified time: 2022-11-30 04:45:58
 from argparse import ArgumentParser
-from os import chdir
 from pathlib import Path
 
-import AutoGenerateMKD
 
-def copy_mkdocs(mkdocs_yml: Path, target_path: Path, project_name: str):
+def copy_mkdocs(target_path: Path, project_name: str):
+    mkdocs_yml = Path(__file__).resolve().parent.joinpath("mkdocs.yml")
     target_path = target_path.joinpath("mkdocs.yml")
     with target_path.open("w") as f1:
         with mkdocs_yml.open("r") as f2:
             content = f2.read().replace("SITE NAME HERE", project_name)
         f1.write(content)
 
 
 def auto_gen_markdown(path: str):
-    mkdocs_yml = Path("mkdocs.yml")
     path_obj = Path(path)
     if not path_obj.exists():
         raise FileNotFoundError(f"Path {path} not found")
 
-    chdir(path_obj.parent)
-    copy_mkdocs(mkdocs_yml, path_obj.parent, path_obj.name)
+    copy_mkdocs(path_obj.parent, path_obj.name)
 
     root_dir = Path(__file__).parent.resolve()
     rep_files_dir = root_dir / path_obj
     doc_files_dir = root_dir / "docs"
     summary_path = root_dir / "SUMMARY.md"
+    doc_files_dir.mkdir(parents=True, exist_ok=True)
 
     with summary_path.open("w", encoding="utf8") as f2:
         for file_path in rep_files_dir.rglob("*.py"):
             module_path = file_path.relative_to(rep_files_dir).with_suffix("").as_posix().replace("/", ".")
             md_file_path = doc_files_dir / file_path.relative_to(rep_files_dir).with_suffix(".md")
             md_file_path.parent.mkdir(parents=True, exist_ok=True)
             with md_file_path.open("w", encoding="utf8") as f:
                 f.write(f"::: {path}.{module_path}")
                 file_name = md_file_path.name.rstrip(".md")
                 f2.write(f"* [{file_name}]({md_file_path.name})\n")
     print("done")
 
 
-# auto_gen_markdown("fast_api_server")
-
-
 def main():
     parser = ArgumentParser(description="Process a project_path.")
     parser.add_argument("-p", "--project_path", dest="project_path", required=True, help="path of the project")
     args = parser.parse_args()
 
     project_path = args.project_path
```

### Comparing `AutoGenerateMKD-0.0.3/LICENSE` & `AutoGenerateMKD-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `AutoGenerateMKD-0.0.3/mkdocs_pagenav_generator/plugin.py` & `AutoGenerateMKD-0.0.4/mkdocs_pagenav_generator/plugin.py`

 * *Files identical despite different names*

### Comparing `AutoGenerateMKD-0.0.3/pyproject.toml` & `AutoGenerateMKD-0.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `AutoGenerateMKD-0.0.3/setup.py` & `AutoGenerateMKD-0.0.4/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name="AutoGenerateMKD",
-    version="0.0.3",
+    version="0.0.4",
     author="E-NoR,Teng",
     description="Auto generate markdown api docs, base on dosc.",
     packages=find_packages(),
     install_requires=[
         "mkdocs>=1",
         "wcmatch>=7",
         "mkdocs-awesome-pages-plugin>=2.5.0",
@@ -22,15 +22,15 @@
         "mkdocs>=1",
         "wcmatch>=7",
         "mkdocs-awesome-pages-plugin>=2.5.0",
     ],
     entry_points={
         "mkdocs.plugins": ["pagenav-generator = mkdocs_pagenav_generator.plugin:NavGeneratorPlugin"],
         "console_scripts": [
-            "auto-gen-markdown=AutoGenerateMKD.main:main",
+            "AutoGenMKD=AutoGenerateMKD.main:main",
         ],
     },
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
```

