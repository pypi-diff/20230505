# Comparing `tmp/AutoGenerateMKD-0.0.4.tar.gz` & `tmp/AutoGenerateMKD-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AutoGenerateMKD-0.0.4.tar", last modified: Fri May  5 14:53:26 2023, max compression
+gzip compressed data, was "AutoGenerateMKD-0.0.5.tar", last modified: Fri May  5 16:25:24 2023, max compression
```

## Comparing `AutoGenerateMKD-0.0.4.tar` & `AutoGenerateMKD-0.0.5.tar`

### file list

```diff
@@ -1,21 +1,24 @@
-drwxr-xr-x   0 coseto     (501) staff       (20)        0 2023-05-05 14:53:26.765801 AutoGenerateMKD-0.0.4/
-drwxr-xr-x   0 coseto     (501) staff       (20)        0 2023-05-05 14:53:26.759724 AutoGenerateMKD-0.0.4/AutoGenerateMKD/
--rw-r--r--   0 coseto     (501) staff       (20)        1 2023-05-05 14:51:10.000000 AutoGenerateMKD-0.0.4/AutoGenerateMKD/__init__.py
--rw-r--r--   0 coseto     (501) staff       (20)     1954 2023-05-05 14:52:11.000000 AutoGenerateMKD-0.0.4/AutoGenerateMKD/main.py
-drwxr-xr-x   0 coseto     (501) staff       (20)        0 2023-05-05 14:53:26.763218 AutoGenerateMKD-0.0.4/AutoGenerateMKD.egg-info/
--rw-r--r--   0 coseto     (501) staff       (20)      302 2023-05-05 14:53:26.000000 AutoGenerateMKD-0.0.4/AutoGenerateMKD.egg-info/PKG-INFO
--rw-r--r--   0 coseto     (501) staff       (20)      419 2023-05-05 14:53:26.000000 AutoGenerateMKD-0.0.4/AutoGenerateMKD.egg-info/SOURCES.txt
--rw-r--r--   0 coseto     (501) staff       (20)        1 2023-05-05 14:53:26.000000 AutoGenerateMKD-0.0.4/AutoGenerateMKD.egg-info/dependency_links.txt
--rw-r--r--   0 coseto     (501) staff       (20)      146 2023-05-05 14:53:26.000000 AutoGenerateMKD-0.0.4/AutoGenerateMKD.egg-info/entry_points.txt
--rw-r--r--   0 coseto     (501) staff       (20)      349 2023-05-05 14:53:26.000000 AutoGenerateMKD-0.0.4/AutoGenerateMKD.egg-info/requires.txt
--rw-r--r--   0 coseto     (501) staff       (20)       41 2023-05-05 14:53:26.000000 AutoGenerateMKD-0.0.4/AutoGenerateMKD.egg-info/top_level.txt
--rw-r--r--   0 coseto     (501) staff       (20)     1054 2023-05-04 15:54:56.000000 AutoGenerateMKD-0.0.4/LICENSE
--rw-r--r--   0 coseto     (501) staff       (20)      302 2023-05-05 14:53:26.765289 AutoGenerateMKD-0.0.4/PKG-INFO
--rw-r--r--   0 coseto     (501) staff       (20)      314 2023-05-04 17:27:35.000000 AutoGenerateMKD-0.0.4/SUMMARY.md
-drwxr-xr-x   0 coseto     (501) staff       (20)        0 2023-05-05 14:53:26.764600 AutoGenerateMKD-0.0.4/mkdocs_pagenav_generator/
--rw-r--r--   0 coseto     (501) staff       (20)        1 2023-05-04 16:28:20.000000 AutoGenerateMKD-0.0.4/mkdocs_pagenav_generator/__init__.py
--rw-r--r--   0 coseto     (501) staff       (20)      993 2023-05-04 16:28:20.000000 AutoGenerateMKD-0.0.4/mkdocs_pagenav_generator/plugin.py
--rw-r--r--   0 coseto     (501) staff       (20)     1371 2023-05-04 15:36:15.000000 AutoGenerateMKD-0.0.4/pyproject.toml
--rw-r--r--   0 coseto     (501) staff       (20)      225 2023-05-04 15:24:17.000000 AutoGenerateMKD-0.0.4/requirements.txt
--rw-r--r--   0 coseto     (501) staff       (20)       38 2023-05-05 14:53:26.765958 AutoGenerateMKD-0.0.4/setup.cfg
--rw-r--r--   0 coseto     (501) staff       (20)     1156 2023-05-05 14:53:22.000000 AutoGenerateMKD-0.0.4/setup.py
+drwxr-xr-x   0 coseto     (501) staff       (20)        0 2023-05-05 16:25:24.957503 AutoGenerateMKD-0.0.5/
+-rw-r--r--   0 coseto     (501) staff       (20)       52 2023-05-05 14:55:45.000000 AutoGenerateMKD-0.0.5/.gitignore
+drwxr-xr-x   0 coseto     (501) staff       (20)        0 2023-05-05 16:25:24.949313 AutoGenerateMKD-0.0.5/AutoGenerateMKD/
+-rw-r--r--   0 coseto     (501) staff       (20)        1 2023-05-05 14:51:10.000000 AutoGenerateMKD-0.0.5/AutoGenerateMKD/__init__.py
+-rw-r--r--   0 coseto     (501) staff       (20)     2369 2023-05-05 16:22:41.000000 AutoGenerateMKD-0.0.5/AutoGenerateMKD/main.py
+-rw-r--r--   0 coseto     (501) staff       (20)     1239 2023-05-04 17:27:12.000000 AutoGenerateMKD-0.0.5/AutoGenerateMKD/mkdocs.yml
+drwxr-xr-x   0 coseto     (501) staff       (20)        0 2023-05-05 16:25:24.954429 AutoGenerateMKD-0.0.5/AutoGenerateMKD.egg-info/
+-rw-r--r--   0 coseto     (501) staff       (20)      302 2023-05-05 16:25:24.000000 AutoGenerateMKD-0.0.5/AutoGenerateMKD.egg-info/PKG-INFO
+-rw-r--r--   0 coseto     (501) staff       (20)      467 2023-05-05 16:25:24.000000 AutoGenerateMKD-0.0.5/AutoGenerateMKD.egg-info/SOURCES.txt
+-rw-r--r--   0 coseto     (501) staff       (20)        1 2023-05-05 16:25:24.000000 AutoGenerateMKD-0.0.5/AutoGenerateMKD.egg-info/dependency_links.txt
+-rw-r--r--   0 coseto     (501) staff       (20)      146 2023-05-05 16:25:24.000000 AutoGenerateMKD-0.0.5/AutoGenerateMKD.egg-info/entry_points.txt
+-rw-r--r--   0 coseto     (501) staff       (20)      349 2023-05-05 16:25:24.000000 AutoGenerateMKD-0.0.5/AutoGenerateMKD.egg-info/requires.txt
+-rw-r--r--   0 coseto     (501) staff       (20)       41 2023-05-05 16:25:24.000000 AutoGenerateMKD-0.0.5/AutoGenerateMKD.egg-info/top_level.txt
+-rw-r--r--   0 coseto     (501) staff       (20)     1054 2023-05-04 15:54:56.000000 AutoGenerateMKD-0.0.5/LICENSE
+-rw-r--r--   0 coseto     (501) staff       (20)      302 2023-05-05 16:25:24.956812 AutoGenerateMKD-0.0.5/PKG-INFO
+-rw-r--r--   0 coseto     (501) staff       (20)       52 2023-05-04 15:56:36.000000 AutoGenerateMKD-0.0.5/Readme.md
+-rw-r--r--   0 coseto     (501) staff       (20)      314 2023-05-05 16:20:54.000000 AutoGenerateMKD-0.0.5/SUMMARY.md
+drwxr-xr-x   0 coseto     (501) staff       (20)        0 2023-05-05 16:25:24.955914 AutoGenerateMKD-0.0.5/mkdocs_pagenav_generator/
+-rw-r--r--   0 coseto     (501) staff       (20)        1 2023-05-04 16:28:20.000000 AutoGenerateMKD-0.0.5/mkdocs_pagenav_generator/__init__.py
+-rw-r--r--   0 coseto     (501) staff       (20)      993 2023-05-04 16:28:20.000000 AutoGenerateMKD-0.0.5/mkdocs_pagenav_generator/plugin.py
+-rw-r--r--   0 coseto     (501) staff       (20)     1371 2023-05-04 15:36:15.000000 AutoGenerateMKD-0.0.5/pyproject.toml
+-rw-r--r--   0 coseto     (501) staff       (20)      225 2023-05-04 15:24:17.000000 AutoGenerateMKD-0.0.5/requirements.txt
+-rw-r--r--   0 coseto     (501) staff       (20)       38 2023-05-05 16:25:24.957684 AutoGenerateMKD-0.0.5/setup.cfg
+-rw-r--r--   0 coseto     (501) staff       (20)     1158 2023-05-05 16:24:52.000000 AutoGenerateMKD-0.0.5/setup.py
```

### Comparing `AutoGenerateMKD-0.0.4/AutoGenerateMKD/main.py` & `AutoGenerateMKD-0.0.5/AutoGenerateMKD/main.py`

 * *Files 19% similar despite different names*

```diff
@@ -12,43 +12,55 @@
     with target_path.open("w") as f1:
         with mkdocs_yml.open("r") as f2:
             content = f2.read().replace("SITE NAME HERE", project_name)
         f1.write(content)
 
 
 def auto_gen_markdown(path: str):
-    path_obj = Path(path)
-    if not path_obj.exists():
+    root_dir = Path(path)
+    project_dir = root_dir
+    project_name = project_dir.name
+    if not root_dir.exists():
         raise FileNotFoundError(f"Path {path} not found")
-
-    copy_mkdocs(path_obj.parent, path_obj.name)
-
-    root_dir = Path(__file__).parent.resolve()
-    rep_files_dir = root_dir / path_obj
-    doc_files_dir = root_dir / "docs"
-    summary_path = root_dir / "SUMMARY.md"
+        
+    copy_mkdocs(root_dir.parent, project_name)
+    doc_files_dir = root_dir.joinpath("docs")
+    summary_path = root_dir.parent.joinpath("SUMMARY.md")
     doc_files_dir.mkdir(parents=True, exist_ok=True)
+    
+
 
     with summary_path.open("w", encoding="utf8") as f2:
-        for file_path in rep_files_dir.rglob("*.py"):
-            module_path = file_path.relative_to(rep_files_dir).with_suffix("").as_posix().replace("/", ".")
-            md_file_path = doc_files_dir / file_path.relative_to(rep_files_dir).with_suffix(".md")
+        for file_path in project_dir.rglob("*.py"):
+            module_path = file_path.with_suffix("").as_posix().replace("/", ".")
+            md_file_path = Path(str(doc_files_dir / file_path.with_suffix(".md")).replace(f"{project_name}/",""))
             md_file_path.parent.mkdir(parents=True, exist_ok=True)
             with md_file_path.open("w", encoding="utf8") as f:
-                f.write(f"::: {path}.{module_path}")
+                f.write(f"::: {module_path}")
                 file_name = md_file_path.name.rstrip(".md")
                 f2.write(f"* [{file_name}]({md_file_path.name})\n")
-    print("done")
+    md_content = f"""
+    # {project_dir.name}
+
+    Welcome to My Project -- {project_dir.name}!
+        
+    more style:
+        Material for MkDocs: https://squidfunk.github.io/mkdocs-material/reference/admonitions/
+    """
+    index_md = Path(str(doc_files_dir / "index.md").replace(f"{project_name}/",""))
+    with index_md.open("w", encoding="utf8") as f:
+        f.write(md_content)
+    print("done.")
 
 
 def main():
     parser = ArgumentParser(description="Process a project_path.")
     parser.add_argument("-p", "--project_path", dest="project_path", required=True, help="path of the project")
     args = parser.parse_args()
 
     project_path = args.project_path
-
     print(f"project_path: {project_path}")
+    auto_gen_markdown(project_path)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `AutoGenerateMKD-0.0.4/LICENSE` & `AutoGenerateMKD-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `AutoGenerateMKD-0.0.4/mkdocs_pagenav_generator/plugin.py` & `AutoGenerateMKD-0.0.5/mkdocs_pagenav_generator/plugin.py`

 * *Files identical despite different names*

### Comparing `AutoGenerateMKD-0.0.4/pyproject.toml` & `AutoGenerateMKD-0.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `AutoGenerateMKD-0.0.4/setup.py` & `AutoGenerateMKD-0.0.5/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,14 @@
+
 from setuptools import find_packages, setup
 
+
 setup(
     name="AutoGenerateMKD",
-    version="0.0.4",
+    version="0.0.5",
     author="E-NoR,Teng",
     description="Auto generate markdown api docs, base on dosc.",
     packages=find_packages(),
     install_requires=[
         "mkdocs>=1",
         "wcmatch>=7",
         "mkdocs-awesome-pages-plugin>=2.5.0",
```

