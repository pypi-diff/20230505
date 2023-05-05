# Comparing `tmp/python-barn-0.4.0.tar.gz` & `tmp/python-barn-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-barn-0.4.0.tar", last modified: Fri Apr 28 10:38:31 2023, max compression
+gzip compressed data, was "python-barn-0.5.0.tar", last modified: Fri May  5 21:19:51 2023, max compression
```

## Comparing `python-barn-0.4.0.tar` & `python-barn-0.5.0.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:38:31.974480 python-barn-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-04-28 10:38:31.974480 python-barn-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-28 10:38:19.000000 python-barn-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:38:31.970480 python-barn-0.4.0/python_barn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-04-28 10:38:31.000000 python-barn-0.4.0/python_barn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-28 10:38:31.000000 python-barn-0.4.0/python_barn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 10:38:31.000000 python-barn-0.4.0/python_barn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 10:38:31.000000 python-barn-0.4.0/python_barn.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-28 10:38:31.000000 python-barn-0.4.0/python_barn.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 10:38:31.974480 python-barn-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-04-28 10:38:19.000000 python-barn-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:38:31.970480 python-barn-0.4.0/src/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-28 10:38:19.000000 python-barn-0.4.0/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:38:31.974480 python-barn-0.4.0/src/actions/
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-28 10:38:19.000000 python-barn-0.4.0/src/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-04-28 10:38:19.000000 python-barn-0.4.0/src/actions/add.py
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-04-28 10:38:19.000000 python-barn-0.4.0/src/actions/execute_script.py
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-04-28 10:38:19.000000 python-barn-0.4.0/src/actions/init.py
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-04-28 10:38:19.000000 python-barn-0.4.0/src/actions/install.py
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-04-28 10:38:19.000000 python-barn-0.4.0/src/actions/remove.py
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-28 10:38:19.000000 python-barn-0.4.0/src/actions/show.py
--rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-04-28 10:38:19.000000 python-barn-0.4.0/src/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     7022 2023-04-28 10:38:19.000000 python-barn-0.4.0/src/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:19:51.099138 python-barn-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-05-05 21:19:51.099138 python-barn-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-05 21:19:39.000000 python-barn-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:19:51.099138 python-barn-0.5.0/python_barn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-05-05 21:19:51.000000 python-barn-0.5.0/python_barn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-05 21:19:51.000000 python-barn-0.5.0/python_barn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 21:19:51.000000 python-barn-0.5.0/python_barn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 21:19:51.000000 python-barn-0.5.0/python_barn.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-05 21:19:51.000000 python-barn-0.5.0/python_barn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-05 21:19:51.000000 python-barn-0.5.0/python_barn.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 21:19:51.099138 python-barn-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-05 21:19:39.000000 python-barn-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:19:51.099138 python-barn-0.5.0/src/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-05 21:19:39.000000 python-barn-0.5.0/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:19:51.099138 python-barn-0.5.0/src/actions/
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-05 21:19:39.000000 python-barn-0.5.0/src/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-05-05 21:19:39.000000 python-barn-0.5.0/src/actions/add.py
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-05 21:19:39.000000 python-barn-0.5.0/src/actions/execute_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-05-05 21:19:39.000000 python-barn-0.5.0/src/actions/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-05-05 21:19:39.000000 python-barn-0.5.0/src/actions/install.py
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-05 21:19:39.000000 python-barn-0.5.0/src/actions/remove.py
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-05 21:19:39.000000 python-barn-0.5.0/src/actions/show.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-05-05 21:19:39.000000 python-barn-0.5.0/src/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7077 2023-05-05 21:19:39.000000 python-barn-0.5.0/src/core.py
```

### Comparing `python-barn-0.4.0/PKG-INFO` & `python-barn-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-barn
-Version: 0.4.0
+Version: 0.5.0
 Summary: A wrapper for pip, to give better utils to python projects dependency management
 Home-page: https://github.com/JacopoMadaluni/barn
 Author: Jacopo Madaluni
 Author-email: jacopo.madaluni@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `python-barn-0.4.0/python_barn.egg-info/PKG-INFO` & `python-barn-0.5.0/python_barn.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-barn
-Version: 0.4.0
+Version: 0.5.0
 Summary: A wrapper for pip, to give better utils to python projects dependency management
 Home-page: https://github.com/JacopoMadaluni/barn
 Author: Jacopo Madaluni
 Author-email: jacopo.madaluni@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `python-barn-0.4.0/setup.py` & `python-barn-0.5.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 from setuptools import setup, find_packages
 
 setup(
     name="python-barn",
-    version="0.4.0",
+    version="0.5.0",
     packages=find_packages(),
     entry_points={
         "console_scripts": [
             "barn=src.cli:main",
         ],
     },
     package_data={
         "barn": ["src/templates/*"]
     },
     install_requires=[
         # Add your package dependencies here, e.g. 'numpy>=1.14.0'
+        "PyYAML==6.0"
     ],
     author="Jacopo Madaluni",
     author_email="jacopo.madaluni@gmail.com",
     description="A wrapper for pip, to give better utils to python projects dependency management",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/JacopoMadaluni/barn",
```

### Comparing `python-barn-0.4.0/src/actions/add.py` & `python-barn-0.5.0/src/actions/add.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,7 +26,9 @@
     if exit_code == 0:
         context.run_command_in_context("pip freeze > barn.lock")
         installed_version = context.get_installed_version(package_name)
         context.add_dependency_to_project_yaml(package_name, installed_version)
     else:
         print(f"Error installing {package_name}=={package_version}")
 
+    return stdout, exit_code
+
```

### Comparing `python-barn-0.4.0/src/actions/init.py` & `python-barn-0.5.0/src/actions/init.py`

 * *Files identical despite different names*

### Comparing `python-barn-0.4.0/src/cli.py` & `python-barn-0.5.0/src/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -44,37 +44,36 @@
 
     subparsers.add_parser('test')
 
     # Parse the arguments
  
     args, unknown_args = parser.parse_known_args()
 
+    exit_code = 0
     if len(unknown_args) > 0:
-        """
-        Script time
-        """
-        execute_script(unknown_args[0])
-
+        _, exit_code = execute_script(unknown_args[0])
     # If no command is given, print help and exit
     elif args.command is None:
-        install()
+        _, exit_code = install()
     elif args.command == 'show':
-        show(args.package_name, verbose=args.verbose, files=args.files)
+        _, exit_code = show(args.package_name, verbose=args.verbose, files=args.files)
     elif args.command == 'install':
-        install()
+        _, exit_code = install()
     elif args.command == 'remove':
-        remove(args.package_name)
+        _, exit_code = remove(args.package_name)
     elif args.command == 'add':
-        add(args.requirement)
+        _, exit_code = add(args.requirement)
     elif args.command == 'init':
         init()
     elif args.command == 'test':
         @barn_action
         def test_action(context: Context=None):
             # Do whatever here
             context.add_dependency_to_project_yaml("test", "1.0.0")
         test_action()
     else:
         print("Unknown command: " + args.command)
 
+    sys.exit(exit_code)
+
 # if __name__ == "__main__":
 #     main()
```

### Comparing `python-barn-0.4.0/src/core.py` & `python-barn-0.5.0/src/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,16 +107,17 @@
         stdout, exit_code = self.run_command_in_context(
             "pip freeze > ./barn.lock"
         )
 
     def install_from_project(self):
         requirements = self.get_dependencies_from_project_yaml()
         requirements_command = ' '.join(requirements)
-        self.run_command_in_context(f"pip install {requirements_command}")
+        stdout, exit_code = self.run_command_in_context(f"pip install {requirements_command}")
         self.freeze_lock()
+        return stdout, exit_code
 
     def get_project_config(self):
         # Load the YAML file
         with open(self.project_yaml_path, 'r') as yaml_file:
             yaml_content = yaml.safe_load(yaml_file)
 
         return yaml_content
@@ -196,24 +197,23 @@
 def find_project_yaml():
     current_dir = Path.cwd()
     while current_dir != Path(current_dir.root):
         if is_barn_project(current_dir):
             return current_dir / "project.yaml"
         current_dir = current_dir.parent
     
-    
     raise Exception("Barn could not find a project context to use. Are you in a project directory?")
 
 
 
 def barn_action(action):
     project_yaml = find_project_yaml()
     root_dir = project_yaml.parent
     is_initialized = is_env_initialized(root_dir)
     context = Context(
         root_dir=root_dir,
         is_initialized=is_initialized
     )
     def wrapper(*args, **kwargs):
-        action(*args, **kwargs, context=context)
+        return action(*args, **kwargs, context=context)
 
     return wrapper
```

