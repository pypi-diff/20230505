# Comparing `tmp/ansible-butler-1.0.6.tar.gz` & `tmp/ansible-butler-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansible-butler-1.0.6.tar", last modified: Thu Feb  9 15:16:33 2023, max compression
+gzip compressed data, was "ansible-butler-1.0.7.tar", last modified: Fri May  5 16:10:47 2023, max compression
```

## Comparing `ansible-butler-1.0.6.tar` & `ansible-butler-1.0.7.tar`

### file list

```diff
@@ -1,35 +1,40 @@
-drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-02-09 15:16:33.998085 ansible-butler-1.0.6/
--rw-r--r--   0 zach       (501) staff       (20)     1886 2023-02-02 23:05:59.000000 ansible-butler-1.0.6/.gitignore
--rw-r--r--   0 zach       (501) staff       (20)    35149 2023-02-02 23:05:59.000000 ansible-butler-1.0.6/LICENSE
--rw-r--r--   0 zach       (501) staff       (20)       43 2023-02-02 23:05:59.000000 ansible-butler-1.0.6/MANIFEST.in
--rw-r--r--   0 zach       (501) staff       (20)     2315 2023-02-09 15:16:33.998197 ansible-butler-1.0.6/PKG-INFO
--rw-r--r--   0 zach       (501) staff       (20)     1749 2023-02-02 23:05:59.000000 ansible-butler-1.0.6/README.md
-drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-02-09 15:16:33.995582 ansible-butler-1.0.6/ansible_butler.egg-info/
--rw-r--r--   0 zach       (501) staff       (20)     2315 2023-02-09 15:16:33.000000 ansible-butler-1.0.6/ansible_butler.egg-info/PKG-INFO
--rw-r--r--   0 zach       (501) staff       (20)      765 2023-02-09 15:16:33.000000 ansible-butler-1.0.6/ansible_butler.egg-info/SOURCES.txt
--rw-r--r--   0 zach       (501) staff       (20)        1 2023-02-09 15:16:33.000000 ansible-butler-1.0.6/ansible_butler.egg-info/dependency_links.txt
--rw-r--r--   0 zach       (501) staff       (20)       54 2023-02-09 15:16:33.000000 ansible-butler-1.0.6/ansible_butler.egg-info/entry_points.txt
--rw-r--r--   0 zach       (501) staff       (20)       42 2023-02-09 15:16:33.000000 ansible-butler-1.0.6/ansible_butler.egg-info/requires.txt
--rw-r--r--   0 zach       (501) staff       (20)       14 2023-02-09 15:16:33.000000 ansible-butler-1.0.6/ansible_butler.egg-info/top_level.txt
-drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-02-09 15:16:33.995872 ansible-butler-1.0.6/ansiblebutler/
--rw-r--r--   0 zach       (501) staff       (20)      882 2023-02-02 23:05:59.000000 ansible-butler-1.0.6/ansiblebutler/__init__.py
--rw-r--r--   0 zach       (501) staff       (20)       68 2023-02-02 23:05:59.000000 ansible-butler-1.0.6/ansiblebutler/__main__.py
-drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-02-09 15:16:33.996017 ansible-butler-1.0.6/ansiblebutler/common/
--rw-r--r--   0 zach       (501) staff       (20)      575 2023-02-02 23:27:52.000000 ansible-butler-1.0.6/ansiblebutler/common/__init__.py
-drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-02-09 15:16:33.996484 ansible-butler-1.0.6/ansiblebutler/directory/
--rw-r--r--   0 zach       (501) staff       (20)      325 2023-02-02 23:05:59.000000 ansible-butler-1.0.6/ansiblebutler/directory/__init__.py
--rw-r--r--   0 zach       (501) staff       (20)      857 2023-02-02 23:05:59.000000 ansible-butler-1.0.6/ansiblebutler/directory/_clean.py
--rw-r--r--   0 zach       (501) staff       (20)     1069 2023-02-02 23:25:47.000000 ansible-butler-1.0.6/ansiblebutler/directory/_initialize.py
-drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-02-09 15:16:33.997027 ansible-butler-1.0.6/ansiblebutler/directory/templates/
--rw-r--r--   0 zach       (501) staff       (20)      213 2023-02-02 23:05:59.000000 ansible-butler-1.0.6/ansiblebutler/directory/templates/playbook.yml.j2
--rw-r--r--   0 zach       (501) staff       (20)      314 2023-02-02 23:05:59.000000 ansible-butler-1.0.6/ansiblebutler/directory/templates/structure.yml
-drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-02-09 15:16:33.997763 ansible-butler-1.0.6/ansiblebutler/roles/
--rw-r--r--   0 zach       (501) staff       (20)      511 2023-02-02 23:05:59.000000 ansible-butler-1.0.6/ansiblebutler/roles/__init__.py
--rw-r--r--   0 zach       (501) staff       (20)      279 2023-02-02 23:05:59.000000 ansible-butler-1.0.6/ansiblebutler/roles/_clean.py
--rw-r--r--   0 zach       (501) staff       (20)       71 2023-02-02 23:05:59.000000 ansible-butler-1.0.6/ansiblebutler/roles/_list.py
--rw-r--r--   0 zach       (501) staff       (20)      906 2023-02-02 23:45:27.000000 ansible-butler-1.0.6/ansiblebutler/roles/_mkreadme.py
-drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-02-09 15:16:33.997912 ansible-butler-1.0.6/ansiblebutler/roles/templates/
--rw-r--r--   0 zach       (501) staff       (20)     2272 2023-02-02 23:05:59.000000 ansible-butler-1.0.6/ansiblebutler/roles/templates/README.md.j2
--rwxr-xr-x   0 zach       (501) staff       (20)      161 2023-02-02 23:36:43.000000 ansible-butler-1.0.6/package.sh
--rw-r--r--   0 zach       (501) staff       (20)      147 2023-02-02 23:05:59.000000 ansible-butler-1.0.6/pyproject.toml
--rw-r--r--   0 zach       (501) staff       (20)      828 2023-02-09 15:16:33.998489 ansible-butler-1.0.6/setup.cfg
+drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-05-05 16:10:47.716140 ansible-butler-1.0.7/
+-rw-r--r--   0 zach       (501) staff       (20)      387 2023-02-16 18:57:23.000000 ansible-butler-1.0.7/.ansible-butler.yml
+-rw-r--r--   0 zach       (501) staff       (20)     1908 2023-02-16 18:58:06.000000 ansible-butler-1.0.7/.gitignore
+-rw-r--r--   0 zach       (501) staff       (20)    35149 2023-02-02 23:05:59.000000 ansible-butler-1.0.7/LICENSE
+-rw-r--r--   0 zach       (501) staff       (20)       43 2023-02-02 23:05:59.000000 ansible-butler-1.0.7/MANIFEST.in
+-rw-r--r--   0 zach       (501) staff       (20)     3091 2023-05-05 16:10:47.716312 ansible-butler-1.0.7/PKG-INFO
+-rw-r--r--   0 zach       (501) staff       (20)     2525 2023-02-16 18:54:36.000000 ansible-butler-1.0.7/README.md
+-rw-r--r--   0 zach       (501) staff       (20)      392 2023-02-16 18:58:41.000000 ansible-butler-1.0.7/ansible-butler.yml
+drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-05-05 16:10:47.711713 ansible-butler-1.0.7/ansible_butler.egg-info/
+-rw-r--r--   0 zach       (501) staff       (20)     3091 2023-05-05 16:10:47.000000 ansible-butler-1.0.7/ansible_butler.egg-info/PKG-INFO
+-rw-r--r--   0 zach       (501) staff       (20)      837 2023-05-05 16:10:47.000000 ansible-butler-1.0.7/ansible_butler.egg-info/SOURCES.txt
+-rw-r--r--   0 zach       (501) staff       (20)        1 2023-05-05 16:10:47.000000 ansible-butler-1.0.7/ansible_butler.egg-info/dependency_links.txt
+-rw-r--r--   0 zach       (501) staff       (20)       54 2023-05-05 16:10:47.000000 ansible-butler-1.0.7/ansible_butler.egg-info/entry_points.txt
+-rw-r--r--   0 zach       (501) staff       (20)       42 2023-05-05 16:10:47.000000 ansible-butler-1.0.7/ansible_butler.egg-info/requires.txt
+-rw-r--r--   0 zach       (501) staff       (20)       14 2023-05-05 16:10:47.000000 ansible-butler-1.0.7/ansible_butler.egg-info/top_level.txt
+drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-05-05 16:10:47.712272 ansible-butler-1.0.7/ansiblebutler/
+-rw-r--r--   0 zach       (501) staff       (20)     1062 2023-02-16 18:46:37.000000 ansible-butler-1.0.7/ansiblebutler/__init__.py
+-rw-r--r--   0 zach       (501) staff       (20)       68 2023-02-02 23:05:59.000000 ansible-butler-1.0.7/ansiblebutler/__main__.py
+drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-05-05 16:10:47.712937 ansible-butler-1.0.7/ansiblebutler/common/
+-rw-r--r--   0 zach       (501) staff       (20)      403 2023-02-16 18:19:30.000000 ansible-butler-1.0.7/ansiblebutler/common/.ansible-butler.yml
+-rw-r--r--   0 zach       (501) staff       (20)     2177 2023-05-05 02:05:35.000000 ansible-butler-1.0.7/ansiblebutler/common/__init__.py
+drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-05-05 16:10:47.713719 ansible-butler-1.0.7/ansiblebutler/directory/
+-rw-r--r--   0 zach       (501) staff       (20)      355 2023-02-16 18:19:44.000000 ansible-butler-1.0.7/ansiblebutler/directory/__init__.py
+-rw-r--r--   0 zach       (501) staff       (20)      857 2023-02-02 23:05:59.000000 ansible-butler-1.0.7/ansiblebutler/directory/_clean.py
+-rw-r--r--   0 zach       (501) staff       (20)      975 2023-02-16 18:19:42.000000 ansible-butler-1.0.7/ansiblebutler/directory/_initialize.py
+drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-05-05 16:10:47.714057 ansible-butler-1.0.7/ansiblebutler/directory/templates/
+-rw-r--r--   0 zach       (501) staff       (20)      213 2023-02-02 23:05:59.000000 ansible-butler-1.0.7/ansiblebutler/directory/templates/playbook.yml.j2
+drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-05-05 16:10:47.715029 ansible-butler-1.0.7/ansiblebutler/roles/
+-rw-r--r--   0 zach       (501) staff       (20)      525 2023-02-12 15:35:55.000000 ansible-butler-1.0.7/ansiblebutler/roles/__init__.py
+-rw-r--r--   0 zach       (501) staff       (20)      279 2023-02-02 23:05:59.000000 ansible-butler-1.0.7/ansiblebutler/roles/_clean.py
+-rw-r--r--   0 zach       (501) staff       (20)       71 2023-02-02 23:05:59.000000 ansible-butler-1.0.7/ansiblebutler/roles/_list.py
+-rw-r--r--   0 zach       (501) staff       (20)     1406 2023-05-05 02:06:24.000000 ansible-butler-1.0.7/ansiblebutler/roles/_mkreadme.py
+drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-05-05 16:10:47.715451 ansible-butler-1.0.7/ansiblebutler/roles/templates/
+-rw-r--r--   0 zach       (501) staff       (20)     2921 2023-05-05 02:06:53.000000 ansible-butler-1.0.7/ansiblebutler/roles/templates/README.md.j2
+drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-05-05 16:10:47.707891 ansible-butler-1.0.7/docs/
+drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-05-05 16:10:47.715812 ansible-butler-1.0.7/docs/config/
+-rw-r--r--   0 zach       (501) staff       (20)      486 2023-02-16 18:28:54.000000 ansible-butler-1.0.7/docs/config/.ansible-butler.example.yml
+-rwxr-xr-x   0 zach       (501) staff       (20)      161 2023-02-02 23:36:43.000000 ansible-butler-1.0.7/package.sh
+-rw-r--r--   0 zach       (501) staff       (20)      147 2023-02-02 23:05:59.000000 ansible-butler-1.0.7/pyproject.toml
+-rw-r--r--   0 zach       (501) staff       (20)      828 2023-05-05 16:10:47.716685 ansible-butler-1.0.7/setup.cfg
```

### Comparing `ansible-butler-1.0.6/.gitignore` & `ansible-butler-1.0.7/.gitignore`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+/*ansible-butler.yml
+
 .DS_Store
 roles/
 
 # Byte-compiled / optimized / DLL files
 __pycache__/
 *.py[cod]
 *$py.class
```

### Comparing `ansible-butler-1.0.6/LICENSE` & `ansible-butler-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ansible-butler-1.0.6/PKG-INFO` & `ansible-butler-1.0.7/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: ansible-butler
-Version: 1.0.6
-Summary: A butler CLI for assistance in managing Ansible projects
-Home-page: https://github.com/zjleblanc/ansible-butler
-Author: Zach LeBlanc
-Author-email: zjleblanc3@gmail.com
-Project-URL: Bug Tracker, https://github.com/zjleblanc/ansible-butler/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License (GPL)
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 ansible-butler
 =========
 
 Butler CLI for Ansible projects
 
 Functions
 ------------
@@ -30,45 +15,79 @@
 | role | mk-readme | auto generate readme based on role meta and basic yml info |
 
 Usage
 --------------
 
 ```
 Usage:
-  ansible-butler directory init [<dir>]
+  ansible-butler directory init [<dir>] [--config=PATH]
   ansible-butler directory clean [<dir>] [--skip-roles]
   ansible-butler role list [--roles-path=PATH] [<name>]
   ansible-butler role clean [--roles-path=PATH] [<name>]
   ansible-butler role mk-readme [--roles-path=PATH] [<name>]
 
 Arguments:
   name    name of role (accepts glob patterns)
   dir     path to directory [default: ./]
 
 Options:
-  -h --help                               Show this screen
+  -h --help           Show this screen
+  --config=PATH       Path to config file
   --roles-path=PATH   Path to roles directory [default: ./roles]
   --skip-roles        Flag to skip cleaning roles
 ```
 
 Examples
 ----------------
 
 - Initialize Ansible Directory
   - `ansible-butler directory init ./sandbox`
+  - `ansible-butler directory init ./sandbox --config=~/configs/ansible-butler.yml`
 - Clean an Ansible Directory
   - `ansible-butler directory clean ./sandbox`
   - `ansible-butler directory clean ./sandbox --skip-roles`
 - Clean Roles 
   - `ansible-butler role clean my-role-1`
   - `ansible-butler role clean my-role-*`
 - Generate README
   - `ansible-butler role mk-readme my-role-1`
   - `ansible-butler role mk-readme my-role-*`
 
+Configuration
+-------------
+
+Create an `.ansible-butler.yml` in one or more of the following locations:
+```
+/etc/ansible-butler/    ## least precedence
+~/
+./                      ## highest precedence
+```
+
+You can also specify a specific path at runtime via the `--config` option.
+
+```yaml
+# Configuration Schema
+
+role: {}
+directory:
+  init:
+    folders:
+      - name: plugins
+        folders:
+          ...
+        files:
+          - README.md
+    files:
+      - playbook.yml
+```
+
+[🔗](./ansiblebutler/common/.ansible-butler.yml) Default configuration file
+<br>
+[🔗](./docs/config/.ansible-butler.example.yml) Example adding test plugins directory
+
 Troubleshooting
 ----------------
 
 - `ansible-butler: command not found`
   - check the $PATH environment variable and ensure that `~/.local/bin` is included
 
 License
@@ -76,8 +95,8 @@
 
 GNU General Public License
 
 Author Information
 -------
 **Zach LeBlanc**
 
-Red Hat
+Red Hat
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `ansible-butler-1.0.6/ansible_butler.egg-info/PKG-INFO` & `ansible-butler-1.0.7/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansible-butler
-Version: 1.0.6
+Version: 1.0.7
 Summary: A butler CLI for assistance in managing Ansible projects
 Home-page: https://github.com/zjleblanc/ansible-butler
 Author: Zach LeBlanc
 Author-email: zjleblanc3@gmail.com
 Project-URL: Bug Tracker, https://github.com/zjleblanc/ansible-butler/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
@@ -30,45 +30,79 @@
 | role | mk-readme | auto generate readme based on role meta and basic yml info |
 
 Usage
 --------------
 
 ```
 Usage:
-  ansible-butler directory init [<dir>]
+  ansible-butler directory init [<dir>] [--config=PATH]
   ansible-butler directory clean [<dir>] [--skip-roles]
   ansible-butler role list [--roles-path=PATH] [<name>]
   ansible-butler role clean [--roles-path=PATH] [<name>]
   ansible-butler role mk-readme [--roles-path=PATH] [<name>]
 
 Arguments:
   name    name of role (accepts glob patterns)
   dir     path to directory [default: ./]
 
 Options:
-  -h --help                               Show this screen
+  -h --help           Show this screen
+  --config=PATH       Path to config file
   --roles-path=PATH   Path to roles directory [default: ./roles]
   --skip-roles        Flag to skip cleaning roles
 ```
 
 Examples
 ----------------
 
 - Initialize Ansible Directory
   - `ansible-butler directory init ./sandbox`
+  - `ansible-butler directory init ./sandbox --config=~/configs/ansible-butler.yml`
 - Clean an Ansible Directory
   - `ansible-butler directory clean ./sandbox`
   - `ansible-butler directory clean ./sandbox --skip-roles`
 - Clean Roles 
   - `ansible-butler role clean my-role-1`
   - `ansible-butler role clean my-role-*`
 - Generate README
   - `ansible-butler role mk-readme my-role-1`
   - `ansible-butler role mk-readme my-role-*`
 
+Configuration
+-------------
+
+Create an `.ansible-butler.yml` in one or more of the following locations:
+```
+/etc/ansible-butler/    ## least precedence
+~/
+./                      ## highest precedence
+```
+
+You can also specify a specific path at runtime via the `--config` option.
+
+```yaml
+# Configuration Schema
+
+role: {}
+directory:
+  init:
+    folders:
+      - name: plugins
+        folders:
+          ...
+        files:
+          - README.md
+    files:
+      - playbook.yml
+```
+
+[🔗](./ansiblebutler/common/.ansible-butler.yml) Default configuration file
+<br>
+[🔗](./docs/config/.ansible-butler.example.yml) Example adding test plugins directory
+
 Troubleshooting
 ----------------
 
 - `ansible-butler: command not found`
   - check the $PATH environment variable and ensure that `~/.local/bin` is included
 
 License
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `ansible-butler-1.0.6/ansible_butler.egg-info/SOURCES.txt` & `ansible-butler-1.0.7/ansible_butler.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,29 @@
+.ansible-butler.yml
 .gitignore
 LICENSE
 MANIFEST.in
 README.md
+ansible-butler.yml
 package.sh
 pyproject.toml
 setup.cfg
 ansible_butler.egg-info/PKG-INFO
 ansible_butler.egg-info/SOURCES.txt
 ansible_butler.egg-info/dependency_links.txt
 ansible_butler.egg-info/entry_points.txt
 ansible_butler.egg-info/requires.txt
 ansible_butler.egg-info/top_level.txt
 ansiblebutler/__init__.py
 ansiblebutler/__main__.py
+ansiblebutler/common/.ansible-butler.yml
 ansiblebutler/common/__init__.py
 ansiblebutler/directory/__init__.py
 ansiblebutler/directory/_clean.py
 ansiblebutler/directory/_initialize.py
 ansiblebutler/directory/templates/playbook.yml.j2
-ansiblebutler/directory/templates/structure.yml
 ansiblebutler/roles/__init__.py
 ansiblebutler/roles/_clean.py
 ansiblebutler/roles/_list.py
 ansiblebutler/roles/_mkreadme.py
-ansiblebutler/roles/templates/README.md.j2
+ansiblebutler/roles/templates/README.md.j2
+docs/config/.ansible-butler.example.yml
```

### Comparing `ansible-butler-1.0.6/ansiblebutler/__init__.py` & `ansible-butler-1.0.7/ansiblebutler/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,32 +1,36 @@
 """
 Usage:
-  ansible-butler directory init [<dir>]
+  ansible-butler directory init [<dir>] [--config=PATH]
   ansible-butler directory clean [<dir>] [--skip-roles]
   ansible-butler role list [--roles-path=PATH] [<name>]
   ansible-butler role clean [--roles-path=PATH] [<name>]
   ansible-butler role mk-readme [--roles-path=PATH] [<name>]
 
 Arguments:
   name    name of role (accepts glob patterns)
   dir     path to directory [default: ./]
 
 Options:
-  -h --help                               Show this screen
+  -h --help           Show this screen
+  --config=PATH       Path to config file
   --roles-path=PATH   Path to roles directory [default: ./roles]
   --skip-roles        Flag to skip cleaning roles
 """
 from docopt import docopt
 from ansiblebutler import roles
 from ansiblebutler import directory
+from ansiblebutler.common import process_config
 
 def main():
   args = docopt(__doc__)
+  config = process_config(args.get('--config'))
+
   if args.get('role'):
-    roles.do_roles_action(args)
+    roles.do_roles_action(args, config.get('role'))
   elif args.get('directory'):
-    directory.do_dir_action(args)
+    directory.do_dir_action(args, config.get('directory'))
   else:
     print(args)
 
 if __name__ == '__main__':
   main()
```

### Comparing `ansible-butler-1.0.6/ansiblebutler/directory/_clean.py` & `ansible-butler-1.0.7/ansiblebutler/directory/_clean.py`

 * *Files identical despite different names*

### Comparing `ansible-butler-1.0.6/ansiblebutler/directory/_initialize.py` & `ansible-butler-1.0.7/ansiblebutler/directory/_initialize.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,14 @@
 import os
-import yaml
 from ..common import get_template 
 from datetime import datetime
 
 DEFAULT_DIR = "./"
 TEMPLATE_DIR = os.path.dirname(os.path.abspath(__file__)) + '/templates'
 
-with open(TEMPLATE_DIR + '/structure.yml', 'r') as stream:
-    STRUCTURE = yaml.safe_load(stream)
-
 def create_file(parent, file: str):
     full_path = parent + '/' + file
     if file.endswith('.j2'):
         template = get_template(file, TEMPLATE_DIR)
         content = template.render({'date': datetime.now()})
         with open(full_path[:-3], 'w') as file:
             file.write(content)
@@ -25,13 +21,13 @@
         create_file(parent, file)
     
     for folder in folder.get('folders', []):
         path = parent + '/' + folder['name']
         os.makedirs(path, exist_ok=True)
         create_folder(path, folder)
 
-def init_dir(dir: str):
+def init_dir(dir: str, structure: dict):
     if dir != DEFAULT_DIR:
         os.makedirs(dir, exist_ok=True)
-    create_folder(dir, STRUCTURE)
+    create_folder(dir, structure)
```

### Comparing `ansible-butler-1.0.6/ansiblebutler/roles/_mkreadme.py` & `ansible-butler-1.0.7/ansiblebutler/roles/_mkreadme.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,31 +1,47 @@
 import os
-from ..common import parse_yml, get_template
+from ..common import parse_yml, parse_comment_lines, parse_comment_line_endings, get_template
 
 TEMPLATE_DIR = os.path.dirname(os.path.abspath(__file__)) + '/templates'
 
 def mk_readme(role: str):
   role_name = os.path.basename(role)
   template_vars = {
     "role_name": role_name,
     "meta": {
       "galaxy_info": {}
     },
     "defaults": {}
   }
   template_vars.update(get_yaml_dict(role + '/meta/main.yml', 'meta'))
-  template_vars.update(get_yaml_dict(role + '/defaults/main.yml', 'defaults'))
+  template_vars.update(get_defaults(role + '/defaults/main.yml'))
+  template_vars.update(get_required_vars(role + '/defaults/main.yml', 'required_vars'))
   template_vars.update(get_yaml_dict(role + '/vars/main.yml', 'vars'))
   template_vars.update(get_yaml_dict(role + '/handlers/main.yml', 'handlers'))
   
   template = get_template('README.md.j2', TEMPLATE_DIR)
   template.stream(template_vars).dump(role + '/README-butler.md')
 
+def get_defaults(yml):
+  defaults = get_yaml_dict(yml)
+  comments = parse_comment_line_endings(yml)
+  return { "defaults": defaults, "default_comments": comments }
+
 def get_yaml_dict(yml, key=None) -> dict:
   if os.path.isfile(yml):
-    parsed = parse_yml(yml)
+    parsed = parse_yml(yml) or {}
+  else:
+    return {}
+
+  if key:
+    return { key: parsed }
+  return parsed or {}
+
+def get_required_vars(yml, key=None) -> dict:
+  if os.path.isfile(yml):
+    parsed = parse_comment_lines(yml) or {}
   else:
     return {}
 
   if key:
     return { key: parsed }
-  return parsed
+  return parsed or {}
```

### Comparing `ansible-butler-1.0.6/ansiblebutler/roles/templates/README.md.j2` & `ansible-butler-1.0.7/ansiblebutler/roles/templates/README.md.j2`

 * *Files 8% similar despite different names*

```diff
@@ -35,26 +35,38 @@
 ------------
 
 {% for req in requirements %}
   - {{ req }}
 {% endfor %}
 
 {% endif %}
+{% if required_vars|length > 0 %}
+
+Required Variables
+------------------
+
+| Name | Example | Description |
+| -------- | ------- | ------------------- |
+{% for req in required_vars %}
+| {{ req.name }} | {{ req.value | default('') }} | {{ req.desc | default('') }} |
+{% endfor %}
+
+{% endif %}
 {% if defaults|length > 0 or vars|length > 0 %}
 
 Role Variables
 --------------
 
-| Variable | Default | Value or Expression |
-| -------- | ------- | ------------------- |
+| Variable | Type | Value or Expression | Description |
+| -------- | ------- | ------------------- | --------- |
 {% for key in defaults %}
-| {{ key }} | :heavy_check_mark: | {{ defaults[key] | string | truncate(length=50,end=' ...') }} |
+| {{ key }} | default | {{ defaults[key] | string | truncate(length=50,end=' ...') }} | {{ default_comments[key] if key in default_comments else '' }} |
 {% endfor %}
 {% for key in vars %}
-| {{ key }} | :x: | {{ vars[key] | string | truncate(length=50,end=' ...') }} |
+| {{ key }} | var | {{ vars[key] | string | truncate(length=50,end=' ...') }} | |
 {% endfor %}
 {% endif %}
 {% if handlers|length > 0 %}
 
 Handlers
 --------------
 
@@ -75,16 +87,24 @@
 Example Playbook
 ----------------
 
 Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:
 
   ```yaml
     - hosts: servers
-      roles:
-          - { role: username.rolename, x: 42 }
+      tasks:
+        - name: Execute {{ role_name }} role
+          ansible.builtin.include_role:
+            name: {{ role_name }}
+          {% if required_vars|length > 0 %}
+          vars:
+          {% for req in required_vars %}
+            {{ req.name }}: {{ req.value | default('...') }}
+          {% endfor %}
+          {% endif %}
   ```
 {% if meta.galaxy_info.license %}
 
 License
 -------
 
 {{ meta.galaxy_info.license }}
```

### Comparing `ansible-butler-1.0.6/setup.cfg` & `ansible-butler-1.0.7/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ansible-butler
-version = 1.0.6
+version = 1.0.7
 author = Zach LeBlanc
 author_email = zjleblanc3@gmail.com
 description = A butler CLI for assistance in managing Ansible projects
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/zjleblanc/ansible-butler
 project_urls =
```

