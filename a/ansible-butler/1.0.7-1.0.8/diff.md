# Comparing `tmp/ansible-butler-1.0.7.tar.gz` & `tmp/ansible-butler-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansible-butler-1.0.7.tar", last modified: Fri May  5 16:10:47 2023, max compression
+gzip compressed data, was "ansible-butler-1.0.8.tar", last modified: Fri May  5 16:29:00 2023, max compression
```

## Comparing `ansible-butler-1.0.7.tar` & `ansible-butler-1.0.8.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-05-05 16:10:47.716140 ansible-butler-1.0.7/
--rw-r--r--   0 zach       (501) staff       (20)      387 2023-02-16 18:57:23.000000 ansible-butler-1.0.7/.ansible-butler.yml
--rw-r--r--   0 zach       (501) staff       (20)     1908 2023-02-16 18:58:06.000000 ansible-butler-1.0.7/.gitignore
--rw-r--r--   0 zach       (501) staff       (20)    35149 2023-02-02 23:05:59.000000 ansible-butler-1.0.7/LICENSE
--rw-r--r--   0 zach       (501) staff       (20)       43 2023-02-02 23:05:59.000000 ansible-butler-1.0.7/MANIFEST.in
--rw-r--r--   0 zach       (501) staff       (20)     3091 2023-05-05 16:10:47.716312 ansible-butler-1.0.7/PKG-INFO
--rw-r--r--   0 zach       (501) staff       (20)     2525 2023-02-16 18:54:36.000000 ansible-butler-1.0.7/README.md
--rw-r--r--   0 zach       (501) staff       (20)      392 2023-02-16 18:58:41.000000 ansible-butler-1.0.7/ansible-butler.yml
-drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-05-05 16:10:47.711713 ansible-butler-1.0.7/ansible_butler.egg-info/
--rw-r--r--   0 zach       (501) staff       (20)     3091 2023-05-05 16:10:47.000000 ansible-butler-1.0.7/ansible_butler.egg-info/PKG-INFO
--rw-r--r--   0 zach       (501) staff       (20)      837 2023-05-05 16:10:47.000000 ansible-butler-1.0.7/ansible_butler.egg-info/SOURCES.txt
--rw-r--r--   0 zach       (501) staff       (20)        1 2023-05-05 16:10:47.000000 ansible-butler-1.0.7/ansible_butler.egg-info/dependency_links.txt
--rw-r--r--   0 zach       (501) staff       (20)       54 2023-05-05 16:10:47.000000 ansible-butler-1.0.7/ansible_butler.egg-info/entry_points.txt
--rw-r--r--   0 zach       (501) staff       (20)       42 2023-05-05 16:10:47.000000 ansible-butler-1.0.7/ansible_butler.egg-info/requires.txt
--rw-r--r--   0 zach       (501) staff       (20)       14 2023-05-05 16:10:47.000000 ansible-butler-1.0.7/ansible_butler.egg-info/top_level.txt
-drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-05-05 16:10:47.712272 ansible-butler-1.0.7/ansiblebutler/
--rw-r--r--   0 zach       (501) staff       (20)     1062 2023-02-16 18:46:37.000000 ansible-butler-1.0.7/ansiblebutler/__init__.py
--rw-r--r--   0 zach       (501) staff       (20)       68 2023-02-02 23:05:59.000000 ansible-butler-1.0.7/ansiblebutler/__main__.py
-drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-05-05 16:10:47.712937 ansible-butler-1.0.7/ansiblebutler/common/
--rw-r--r--   0 zach       (501) staff       (20)      403 2023-02-16 18:19:30.000000 ansible-butler-1.0.7/ansiblebutler/common/.ansible-butler.yml
--rw-r--r--   0 zach       (501) staff       (20)     2177 2023-05-05 02:05:35.000000 ansible-butler-1.0.7/ansiblebutler/common/__init__.py
-drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-05-05 16:10:47.713719 ansible-butler-1.0.7/ansiblebutler/directory/
--rw-r--r--   0 zach       (501) staff       (20)      355 2023-02-16 18:19:44.000000 ansible-butler-1.0.7/ansiblebutler/directory/__init__.py
--rw-r--r--   0 zach       (501) staff       (20)      857 2023-02-02 23:05:59.000000 ansible-butler-1.0.7/ansiblebutler/directory/_clean.py
--rw-r--r--   0 zach       (501) staff       (20)      975 2023-02-16 18:19:42.000000 ansible-butler-1.0.7/ansiblebutler/directory/_initialize.py
-drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-05-05 16:10:47.714057 ansible-butler-1.0.7/ansiblebutler/directory/templates/
--rw-r--r--   0 zach       (501) staff       (20)      213 2023-02-02 23:05:59.000000 ansible-butler-1.0.7/ansiblebutler/directory/templates/playbook.yml.j2
-drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-05-05 16:10:47.715029 ansible-butler-1.0.7/ansiblebutler/roles/
--rw-r--r--   0 zach       (501) staff       (20)      525 2023-02-12 15:35:55.000000 ansible-butler-1.0.7/ansiblebutler/roles/__init__.py
--rw-r--r--   0 zach       (501) staff       (20)      279 2023-02-02 23:05:59.000000 ansible-butler-1.0.7/ansiblebutler/roles/_clean.py
--rw-r--r--   0 zach       (501) staff       (20)       71 2023-02-02 23:05:59.000000 ansible-butler-1.0.7/ansiblebutler/roles/_list.py
--rw-r--r--   0 zach       (501) staff       (20)     1406 2023-05-05 02:06:24.000000 ansible-butler-1.0.7/ansiblebutler/roles/_mkreadme.py
-drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-05-05 16:10:47.715451 ansible-butler-1.0.7/ansiblebutler/roles/templates/
--rw-r--r--   0 zach       (501) staff       (20)     2921 2023-05-05 02:06:53.000000 ansible-butler-1.0.7/ansiblebutler/roles/templates/README.md.j2
-drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-05-05 16:10:47.707891 ansible-butler-1.0.7/docs/
-drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-05-05 16:10:47.715812 ansible-butler-1.0.7/docs/config/
--rw-r--r--   0 zach       (501) staff       (20)      486 2023-02-16 18:28:54.000000 ansible-butler-1.0.7/docs/config/.ansible-butler.example.yml
--rwxr-xr-x   0 zach       (501) staff       (20)      161 2023-02-02 23:36:43.000000 ansible-butler-1.0.7/package.sh
--rw-r--r--   0 zach       (501) staff       (20)      147 2023-02-02 23:05:59.000000 ansible-butler-1.0.7/pyproject.toml
--rw-r--r--   0 zach       (501) staff       (20)      828 2023-05-05 16:10:47.716685 ansible-butler-1.0.7/setup.cfg
+drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-05-05 16:29:00.947415 ansible-butler-1.0.8/
+-rw-r--r--   0 zach       (501) staff       (20)      387 2023-02-16 18:57:23.000000 ansible-butler-1.0.8/.ansible-butler.yml
+-rw-r--r--   0 zach       (501) staff       (20)     1908 2023-02-16 18:58:06.000000 ansible-butler-1.0.8/.gitignore
+-rw-r--r--   0 zach       (501) staff       (20)    35149 2023-02-02 23:05:59.000000 ansible-butler-1.0.8/LICENSE
+-rw-r--r--   0 zach       (501) staff       (20)       43 2023-02-02 23:05:59.000000 ansible-butler-1.0.8/MANIFEST.in
+-rw-r--r--   0 zach       (501) staff       (20)     3091 2023-05-05 16:29:00.947551 ansible-butler-1.0.8/PKG-INFO
+-rw-r--r--   0 zach       (501) staff       (20)     2525 2023-02-16 18:54:36.000000 ansible-butler-1.0.8/README.md
+-rw-r--r--   0 zach       (501) staff       (20)      392 2023-02-16 18:58:41.000000 ansible-butler-1.0.8/ansible-butler.yml
+drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-05-05 16:29:00.942934 ansible-butler-1.0.8/ansible_butler.egg-info/
+-rw-r--r--   0 zach       (501) staff       (20)     3091 2023-05-05 16:29:00.000000 ansible-butler-1.0.8/ansible_butler.egg-info/PKG-INFO
+-rw-r--r--   0 zach       (501) staff       (20)      837 2023-05-05 16:29:00.000000 ansible-butler-1.0.8/ansible_butler.egg-info/SOURCES.txt
+-rw-r--r--   0 zach       (501) staff       (20)        1 2023-05-05 16:29:00.000000 ansible-butler-1.0.8/ansible_butler.egg-info/dependency_links.txt
+-rw-r--r--   0 zach       (501) staff       (20)       54 2023-05-05 16:29:00.000000 ansible-butler-1.0.8/ansible_butler.egg-info/entry_points.txt
+-rw-r--r--   0 zach       (501) staff       (20)       42 2023-05-05 16:29:00.000000 ansible-butler-1.0.8/ansible_butler.egg-info/requires.txt
+-rw-r--r--   0 zach       (501) staff       (20)       14 2023-05-05 16:29:00.000000 ansible-butler-1.0.8/ansible_butler.egg-info/top_level.txt
+drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-05-05 16:29:00.943529 ansible-butler-1.0.8/ansiblebutler/
+-rw-r--r--   0 zach       (501) staff       (20)     1062 2023-02-16 18:46:37.000000 ansible-butler-1.0.8/ansiblebutler/__init__.py
+-rw-r--r--   0 zach       (501) staff       (20)       68 2023-02-02 23:05:59.000000 ansible-butler-1.0.8/ansiblebutler/__main__.py
+drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-05-05 16:29:00.944022 ansible-butler-1.0.8/ansiblebutler/common/
+-rw-r--r--   0 zach       (501) staff       (20)      403 2023-02-16 18:19:30.000000 ansible-butler-1.0.8/ansiblebutler/common/.ansible-butler.yml
+-rw-r--r--   0 zach       (501) staff       (20)     2177 2023-05-05 02:05:35.000000 ansible-butler-1.0.8/ansiblebutler/common/__init__.py
+drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-05-05 16:29:00.945037 ansible-butler-1.0.8/ansiblebutler/directory/
+-rw-r--r--   0 zach       (501) staff       (20)      355 2023-02-16 18:19:44.000000 ansible-butler-1.0.8/ansiblebutler/directory/__init__.py
+-rw-r--r--   0 zach       (501) staff       (20)      857 2023-02-02 23:05:59.000000 ansible-butler-1.0.8/ansiblebutler/directory/_clean.py
+-rw-r--r--   0 zach       (501) staff       (20)      975 2023-02-16 18:19:42.000000 ansible-butler-1.0.8/ansiblebutler/directory/_initialize.py
+drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-05-05 16:29:00.945370 ansible-butler-1.0.8/ansiblebutler/directory/templates/
+-rw-r--r--   0 zach       (501) staff       (20)      213 2023-02-02 23:05:59.000000 ansible-butler-1.0.8/ansiblebutler/directory/templates/playbook.yml.j2
+drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-05-05 16:29:00.946712 ansible-butler-1.0.8/ansiblebutler/roles/
+-rw-r--r--   0 zach       (501) staff       (20)      525 2023-02-12 15:35:55.000000 ansible-butler-1.0.8/ansiblebutler/roles/__init__.py
+-rw-r--r--   0 zach       (501) staff       (20)      279 2023-02-02 23:05:59.000000 ansible-butler-1.0.8/ansiblebutler/roles/_clean.py
+-rw-r--r--   0 zach       (501) staff       (20)       71 2023-02-02 23:05:59.000000 ansible-butler-1.0.8/ansiblebutler/roles/_list.py
+-rw-r--r--   0 zach       (501) staff       (20)     1242 2023-05-05 16:27:29.000000 ansible-butler-1.0.8/ansiblebutler/roles/_mkreadme.py
+drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-05-05 16:29:00.946898 ansible-butler-1.0.8/ansiblebutler/roles/templates/
+-rw-r--r--   0 zach       (501) staff       (20)     2980 2023-05-05 16:20:23.000000 ansible-butler-1.0.8/ansiblebutler/roles/templates/README.md.j2
+drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-05-05 16:29:00.938758 ansible-butler-1.0.8/docs/
+drwxr-xr-x   0 zach       (501) staff       (20)        0 2023-05-05 16:29:00.947075 ansible-butler-1.0.8/docs/config/
+-rw-r--r--   0 zach       (501) staff       (20)      486 2023-02-16 18:28:54.000000 ansible-butler-1.0.8/docs/config/.ansible-butler.example.yml
+-rwxr-xr-x   0 zach       (501) staff       (20)      161 2023-02-02 23:36:43.000000 ansible-butler-1.0.8/package.sh
+-rw-r--r--   0 zach       (501) staff       (20)      147 2023-02-02 23:05:59.000000 ansible-butler-1.0.8/pyproject.toml
+-rw-r--r--   0 zach       (501) staff       (20)      828 2023-05-05 16:29:00.947909 ansible-butler-1.0.8/setup.cfg
```

### Comparing `ansible-butler-1.0.7/.gitignore` & `ansible-butler-1.0.8/.gitignore`

 * *Files identical despite different names*

### Comparing `ansible-butler-1.0.7/LICENSE` & `ansible-butler-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ansible-butler-1.0.7/PKG-INFO` & `ansible-butler-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansible-butler
-Version: 1.0.7
+Version: 1.0.8
 Summary: A butler CLI for assistance in managing Ansible projects
 Home-page: https://github.com/zjleblanc/ansible-butler
 Author: Zach LeBlanc
 Author-email: zjleblanc3@gmail.com
 Project-URL: Bug Tracker, https://github.com/zjleblanc/ansible-butler/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
```

### Comparing `ansible-butler-1.0.7/README.md` & `ansible-butler-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `ansible-butler-1.0.7/ansible_butler.egg-info/PKG-INFO` & `ansible-butler-1.0.8/ansible_butler.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansible-butler
-Version: 1.0.7
+Version: 1.0.8
 Summary: A butler CLI for assistance in managing Ansible projects
 Home-page: https://github.com/zjleblanc/ansible-butler
 Author: Zach LeBlanc
 Author-email: zjleblanc3@gmail.com
 Project-URL: Bug Tracker, https://github.com/zjleblanc/ansible-butler/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
```

### Comparing `ansible-butler-1.0.7/ansible_butler.egg-info/SOURCES.txt` & `ansible-butler-1.0.8/ansible_butler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ansible-butler-1.0.7/ansiblebutler/__init__.py` & `ansible-butler-1.0.8/ansiblebutler/__init__.py`

 * *Files identical despite different names*

### Comparing `ansible-butler-1.0.7/ansiblebutler/common/__init__.py` & `ansible-butler-1.0.8/ansiblebutler/common/__init__.py`

 * *Files identical despite different names*

### Comparing `ansible-butler-1.0.7/ansiblebutler/directory/_clean.py` & `ansible-butler-1.0.8/ansiblebutler/directory/_clean.py`

 * *Files identical despite different names*

### Comparing `ansible-butler-1.0.7/ansiblebutler/directory/_initialize.py` & `ansible-butler-1.0.8/ansiblebutler/directory/_initialize.py`

 * *Files identical despite different names*

### Comparing `ansible-butler-1.0.7/ansiblebutler/roles/__init__.py` & `ansible-butler-1.0.8/ansiblebutler/roles/__init__.py`

 * *Files identical despite different names*

### Comparing `ansible-butler-1.0.7/ansiblebutler/roles/_mkreadme.py` & `ansible-butler-1.0.8/ansiblebutler/roles/_mkreadme.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,43 +5,33 @@
 
 def mk_readme(role: str):
   role_name = os.path.basename(role)
   template_vars = {
     "role_name": role_name,
     "meta": {
       "galaxy_info": {}
-    },
-    "defaults": {}
+    }
   }
   template_vars.update(get_yaml_dict(role + '/meta/main.yml', 'meta'))
-  template_vars.update(get_defaults(role + '/defaults/main.yml'))
-  template_vars.update(get_required_vars(role + '/defaults/main.yml', 'required_vars'))
+  template_vars.update(get_yaml_dict(role + '/defaults/main.yml', 'defaults'))
   template_vars.update(get_yaml_dict(role + '/vars/main.yml', 'vars'))
   template_vars.update(get_yaml_dict(role + '/handlers/main.yml', 'handlers'))
+  template_vars.update(get_required_vars(role + '/defaults/main.yml', 'required_vars'))
   
   template = get_template('README.md.j2', TEMPLATE_DIR)
   template.stream(template_vars).dump(role + '/README-butler.md')
 
-def get_defaults(yml):
-  defaults = get_yaml_dict(yml)
-  comments = parse_comment_line_endings(yml)
-  return { "defaults": defaults, "default_comments": comments }
-
-def get_yaml_dict(yml, key=None) -> dict:
+def get_yaml_dict(yml, key) -> dict:
   if os.path.isfile(yml):
     parsed = parse_yml(yml) or {}
+    comments = parse_comment_line_endings(yml)
   else:
-    return {}
+    parsed = {}
+    comments = {}
 
-  if key:
-    return { key: parsed }
-  return parsed or {}
+  return { key: parsed, key + "_comments": comments }
 
-def get_required_vars(yml, key=None) -> dict:
+def get_required_vars(yml, key) -> dict:
   if os.path.isfile(yml):
-    parsed = parse_comment_lines(yml) or {}
+    return { key: parse_comment_lines(yml) or {} }
   else:
-    return {}
-
-  if key:
-    return { key: parsed }
-  return parsed or {}
+    return { key: {} }
```

### Comparing `ansible-butler-1.0.7/ansiblebutler/roles/templates/README.md.j2` & `ansible-butler-1.0.8/ansiblebutler/roles/templates/README.md.j2`

 * *Files 8% similar despite different names*

```diff
@@ -55,18 +55,18 @@
 
 Role Variables
 --------------
 
 | Variable | Type | Value or Expression | Description |
 | -------- | ------- | ------------------- | --------- |
 {% for key in defaults %}
-| {{ key }} | default | {{ defaults[key] | string | truncate(length=50,end=' ...') }} | {{ default_comments[key] if key in default_comments else '' }} |
+| {{ key }} | default | {{ defaults[key] | string | truncate(length=50,end=' ...') }} | {{ defaults_comments[key] if key in defaults_comments else '' }} |
 {% endfor %}
 {% for key in vars %}
-| {{ key }} | var | {{ vars[key] | string | truncate(length=50,end=' ...') }} | |
+| {{ key }} | var | {{ vars[key] | string | truncate(length=50,end=' ...') }} | {{ vars_comments[key] if key in vars_comments else '' }} |
 {% endfor %}
 {% endif %}
 {% if handlers|length > 0 %}
 
 Handlers
 --------------
```

### Comparing `ansible-butler-1.0.7/setup.cfg` & `ansible-butler-1.0.8/setup.cfg`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ansible-butler
-version = 1.0.7
+version = 1.0.8
 author = Zach LeBlanc
 author_email = zjleblanc3@gmail.com
 description = A butler CLI for assistance in managing Ansible projects
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/zjleblanc/ansible-butler
 project_urls =
```

