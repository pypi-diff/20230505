# Comparing `tmp/ou_container_builder-2.3.0.tar.gz` & `tmp/ou_container_builder-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ou_container_builder-2.3.0.tar", max compression
+gzip compressed data, was "ou_container_builder-2.4.0.tar", max compression
```

## Comparing `ou_container_builder-2.3.0.tar` & `ou_container_builder-2.4.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0       32 2023-05-02 13:54:37.775985 ou_container_builder-2.3.0/ou_container_builder/__init__.py
--rw-r--r--   0        0        0     1454 2023-05-02 13:54:37.775985 ou_container_builder-2.3.0/ou_container_builder/__main__.py
--rw-r--r--   0        0        0     6189 2023-05-02 13:54:37.775985 ou_container_builder-2.3.0/ou_container_builder/builder.py
--rw-r--r--   0        0        0      158 2023-05-02 13:54:37.775985 ou_container_builder-2.3.0/ou_container_builder/core/__init__.py
--rw-r--r--   0        0        0     1035 2023-05-02 13:54:37.775985 ou_container_builder-2.3.0/ou_container_builder/core/base.py
--rw-r--r--   0        0        0     2435 2023-05-02 13:54:37.775985 ou_container_builder-2.3.0/ou_container_builder/core/content.py
--rw-r--r--   0        0        0      815 2023-05-02 13:54:37.775985 ou_container_builder-2.3.0/ou_container_builder/core/env.py
--rw-r--r--   0        0        0     1137 2023-05-02 13:54:37.775985 ou_container_builder-2.3.0/ou_container_builder/core/hacks.py
--rw-r--r--   0        0        0     3096 2023-05-02 13:54:37.776985 ou_container_builder-2.3.0/ou_container_builder/core/jupyter_server.py
--rw-r--r--   0        0        0     1172 2023-05-02 13:54:37.776985 ou_container_builder-2.3.0/ou_container_builder/core/packages.py
--rw-r--r--   0        0        0     4219 2023-05-02 13:54:37.776985 ou_container_builder-2.3.0/ou_container_builder/core/scripts.py
--rw-r--r--   0        0        0     1522 2023-05-02 13:54:37.776985 ou_container_builder-2.3.0/ou_container_builder/core/services.py
--rw-r--r--   0        0        0     2216 2023-05-02 13:54:37.776985 ou_container_builder-2.3.0/ou_container_builder/core/startup.py
--rw-r--r--   0        0        0     2613 2023-05-02 13:54:37.776985 ou_container_builder-2.3.0/ou_container_builder/core/web_apps.py
--rw-r--r--   0        0        0      152 2023-05-02 13:54:37.776985 ou_container_builder-2.3.0/ou_container_builder/packs/__init__.py
--rw-r--r--   0        0        0     4579 2023-05-02 13:54:37.776985 ou_container_builder-2.3.0/ou_container_builder/packs/code_server.py
--rw-r--r--   0        0        0     1558 2023-05-02 13:54:37.776985 ou_container_builder-2.3.0/ou_container_builder/packs/jupyterlab.py
--rw-r--r--   0        0        0     2895 2023-05-02 13:54:37.776985 ou_container_builder-2.3.0/ou_container_builder/packs/mariadb.py
--rw-r--r--   0        0        0     1853 2023-05-02 13:54:37.777985 ou_container_builder-2.3.0/ou_container_builder/packs/nbclassic.py
--rw-r--r--   0        0        0     2733 2023-05-02 13:54:37.777985 ou_container_builder-2.3.0/ou_container_builder/packs/tutorial_server.py
--rw-r--r--   0        0        0     3599 2023-05-02 13:54:37.777985 ou_container_builder-2.3.0/ou_container_builder/templates/Dockerfile.jinja2
--rw-r--r--   0        0        0      990 2023-05-02 13:54:37.777985 ou_container_builder-2.3.0/ou_container_builder/templates/core/content/content_config.yaml
--rw-r--r--   0        0        0      190 2023-05-02 13:54:37.777985 ou_container_builder-2.3.0/ou_container_builder/templates/core/services/sudoers
--rw-r--r--   0        0        0      140 2023-05-02 13:54:37.777985 ou_container_builder-2.3.0/ou_container_builder/templates/core/startup/home-dir.sudoers
--rw-r--r--   0        0        0      486 2023-05-02 13:54:37.777985 ou_container_builder-2.3.0/ou_container_builder/templates/core/startup/start.sh
--rw-r--r--   0        0        0     4451 2023-05-02 13:54:37.777985 ou_container_builder-2.3.0/ou_container_builder/templates/packs/code_server/vscode.svg
--rw-r--r--   0        0        0      615 2023-05-02 13:54:37.778985 ou_container_builder-2.3.0/ou_container_builder/templates/packs/mariadb/setup.sh
--rw-r--r--   0        0        0      942 2023-05-02 13:54:37.778985 ou_container_builder-2.3.0/ou_container_builder/templates/packs/tutorial-server/production.ini
--rw-r--r--   0        0        0     2142 2023-05-02 13:54:37.778985 ou_container_builder-2.3.0/ou_container_builder/utils.py
--rw-r--r--   0        0        0    12432 2023-05-02 13:54:37.778985 ou_container_builder-2.3.0/ou_container_builder/validator.py
--rw-r--r--   0        0        0      629 2023-05-02 13:54:37.778985 ou_container_builder-2.3.0/pyproject.toml
--rw-r--r--   0        0        0      612 1970-01-01 00:00:00.000000 ou_container_builder-2.3.0/PKG-INFO
+-rw-r--r--   0        0        0       32 2023-05-05 10:53:41.164722 ou_container_builder-2.4.0/ou_container_builder/__init__.py
+-rw-r--r--   0        0        0     1454 2023-05-05 10:53:41.164722 ou_container_builder-2.4.0/ou_container_builder/__main__.py
+-rw-r--r--   0        0        0     6189 2023-05-05 10:53:41.165722 ou_container_builder-2.4.0/ou_container_builder/builder.py
+-rw-r--r--   0        0        0      158 2023-05-05 10:53:41.165722 ou_container_builder-2.4.0/ou_container_builder/core/__init__.py
+-rw-r--r--   0        0        0     1098 2023-05-05 10:53:41.165722 ou_container_builder-2.4.0/ou_container_builder/core/base.py
+-rw-r--r--   0        0        0     2435 2023-05-05 10:53:41.165722 ou_container_builder-2.4.0/ou_container_builder/core/content.py
+-rw-r--r--   0        0        0      815 2023-05-05 10:53:41.165722 ou_container_builder-2.4.0/ou_container_builder/core/env.py
+-rw-r--r--   0        0        0     1137 2023-05-05 10:53:41.165722 ou_container_builder-2.4.0/ou_container_builder/core/hacks.py
+-rw-r--r--   0        0        0     3096 2023-05-05 10:53:41.165722 ou_container_builder-2.4.0/ou_container_builder/core/jupyter_server.py
+-rw-r--r--   0        0        0     1172 2023-05-05 10:53:41.165722 ou_container_builder-2.4.0/ou_container_builder/core/packages.py
+-rw-r--r--   0        0        0     4219 2023-05-05 10:53:41.166722 ou_container_builder-2.4.0/ou_container_builder/core/scripts.py
+-rw-r--r--   0        0        0     1522 2023-05-05 10:53:41.166722 ou_container_builder-2.4.0/ou_container_builder/core/services.py
+-rw-r--r--   0        0        0     2216 2023-05-05 10:53:41.166722 ou_container_builder-2.4.0/ou_container_builder/core/startup.py
+-rw-r--r--   0        0        0     2613 2023-05-05 10:53:41.166722 ou_container_builder-2.4.0/ou_container_builder/core/web_apps.py
+-rw-r--r--   0        0        0      152 2023-05-05 10:53:41.166722 ou_container_builder-2.4.0/ou_container_builder/packs/__init__.py
+-rw-r--r--   0        0        0     4616 2023-05-05 10:53:41.166722 ou_container_builder-2.4.0/ou_container_builder/packs/code_server.py
+-rw-r--r--   0        0        0     1558 2023-05-05 10:53:41.166722 ou_container_builder-2.4.0/ou_container_builder/packs/jupyterlab.py
+-rw-r--r--   0        0        0     2895 2023-05-05 10:53:41.166722 ou_container_builder-2.4.0/ou_container_builder/packs/mariadb.py
+-rw-r--r--   0        0        0     1853 2023-05-05 10:53:41.166722 ou_container_builder-2.4.0/ou_container_builder/packs/nbclassic.py
+-rw-r--r--   0        0        0     2733 2023-05-05 10:53:41.166722 ou_container_builder-2.4.0/ou_container_builder/packs/tutorial_server.py
+-rw-r--r--   0        0        0     3766 2023-05-05 10:53:41.167723 ou_container_builder-2.4.0/ou_container_builder/templates/Dockerfile.jinja2
+-rw-r--r--   0        0        0      990 2023-05-05 10:53:41.167723 ou_container_builder-2.4.0/ou_container_builder/templates/core/content/content_config.yaml
+-rw-r--r--   0        0        0      190 2023-05-05 10:53:41.167723 ou_container_builder-2.4.0/ou_container_builder/templates/core/services/sudoers
+-rw-r--r--   0        0        0      140 2023-05-05 10:53:41.167723 ou_container_builder-2.4.0/ou_container_builder/templates/core/startup/home-dir.sudoers
+-rw-r--r--   0        0        0      486 2023-05-05 10:53:41.167723 ou_container_builder-2.4.0/ou_container_builder/templates/core/startup/start.sh
+-rw-r--r--   0        0        0     4451 2023-05-05 10:53:41.168722 ou_container_builder-2.4.0/ou_container_builder/templates/packs/code_server/vscode.svg
+-rw-r--r--   0        0        0      615 2023-05-05 10:53:41.168722 ou_container_builder-2.4.0/ou_container_builder/templates/packs/mariadb/setup.sh
+-rw-r--r--   0        0        0      942 2023-05-05 10:53:41.168722 ou_container_builder-2.4.0/ou_container_builder/templates/packs/tutorial-server/production.ini
+-rw-r--r--   0        0        0     2142 2023-05-05 10:53:41.168722 ou_container_builder-2.4.0/ou_container_builder/utils.py
+-rw-r--r--   0        0        0    12634 2023-05-05 10:53:41.168722 ou_container_builder-2.4.0/ou_container_builder/validator.py
+-rw-r--r--   0        0        0      629 2023-05-05 10:53:41.169722 ou_container_builder-2.4.0/pyproject.toml
+-rw-r--r--   0        0        0      612 1970-01-01 00:00:00.000000 ou_container_builder-2.4.0/PKG-INFO
```

### Comparing `ou_container_builder-2.3.0/ou_container_builder/__main__.py` & `ou_container_builder-2.4.0/ou_container_builder/__main__.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.3.0/ou_container_builder/builder.py` & `ou_container_builder-2.4.0/ou_container_builder/builder.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.3.0/ou_container_builder/core/base.py` & `ou_container_builder-2.4.0/ou_container_builder/core/base.py`

 * *Files 13% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     :param settings: The settings parsed from the configuration file
     :type settings: dict
     :return: The updated settings
     :rtype: dict
     """
     settings = merge_settings({
         'packages': {
-            'apt': ['libcurl3-gnutls'],
+            'apt': ['libcurl3-gnutls', 'libcurl3-gnutls-dev', 'gnutls-dev', 'gcc', 'build-essential'],
             'pip': ['pycurl'],
         }
     }, settings)
     return settings
 
 
 def generate_files(context: str, env: Environment, settings: dict) -> None:
```

### Comparing `ou_container_builder-2.3.0/ou_container_builder/core/content.py` & `ou_container_builder-2.4.0/ou_container_builder/core/content.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
             }
         })
     if 'flags' in settings and settings['flags']:
         if 'ou_container_content' in settings['flags'] and settings['flags']['ou_container_content']:
             settings = merge_settings(settings, {
                 'packages': {
                     'pip': [
-                        'ou-container-content>=1.1.2'
+                        'ou-container-content>=1.1.3'
                     ]
                 },
                 'scripts': {
                     'build': [
                         {
                             'commands': [
                                 'ou-container-content prepare'
```

### Comparing `ou_container_builder-2.3.0/ou_container_builder/core/env.py` & `ou_container_builder-2.4.0/ou_container_builder/core/env.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.3.0/ou_container_builder/core/hacks.py` & `ou_container_builder-2.4.0/ou_container_builder/core/hacks.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.3.0/ou_container_builder/core/jupyter_server.py` & `ou_container_builder-2.4.0/ou_container_builder/core/jupyter_server.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.3.0/ou_container_builder/core/packages.py` & `ou_container_builder-2.4.0/ou_container_builder/core/packages.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.3.0/ou_container_builder/core/scripts.py` & `ou_container_builder-2.4.0/ou_container_builder/core/scripts.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.3.0/ou_container_builder/core/services.py` & `ou_container_builder-2.4.0/ou_container_builder/core/services.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.3.0/ou_container_builder/core/startup.py` & `ou_container_builder-2.4.0/ou_container_builder/core/startup.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.3.0/ou_container_builder/core/web_apps.py` & `ou_container_builder-2.4.0/ou_container_builder/core/web_apps.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.3.0/ou_container_builder/packs/code_server.py` & `ou_container_builder-2.4.0/ou_container_builder/packs/code_server.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,14 +26,15 @@
     warn('Automatically setting the code_server as the default web-app is deprecated in 2.2.0 and will be removed in 3.0.0. Instead set server.default_path explicitly.', FutureWarning)  # noqa: E501
     settings = merge_settings(settings, {
         'sources': {
             'apt': [
                 {
                     'name': 'nodesource',
                     'key_url': 'https://deb.nodesource.com/gpgkey/nodesource.gpg.key',
+                    'dearmor': True,
                     'deb': {
                         'url': 'https://deb.nodesource.com/node_18.x',
                         'distribution': 'bullseye',
                         'component': 'main'
                     }
                 }
             ],
```

### Comparing `ou_container_builder-2.3.0/ou_container_builder/packs/jupyterlab.py` & `ou_container_builder-2.4.0/ou_container_builder/packs/jupyterlab.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.3.0/ou_container_builder/packs/mariadb.py` & `ou_container_builder-2.4.0/ou_container_builder/packs/mariadb.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.3.0/ou_container_builder/packs/nbclassic.py` & `ou_container_builder-2.4.0/ou_container_builder/packs/nbclassic.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.3.0/ou_container_builder/packs/tutorial_server.py` & `ou_container_builder-2.4.0/ou_container_builder/packs/tutorial_server.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.3.0/ou_container_builder/templates/Dockerfile.jinja2` & `ou_container_builder-2.4.0/ou_container_builder/templates/Dockerfile.jinja2`

 * *Files 12% similar despite different names*

```diff
@@ -38,17 +38,22 @@
 RUN mkdir -p /usr/share/man/man1
     {% endif %}
   {% endif %}
 {% endblock %}
 
 {% block apt_sources %}
   {% if sources and sources.apt %}
+RUN apt-get install -y gnupg
     {% for source in sources.apt %}
-RUN curl -fsSL "{{ source.key_url }}" | apt-key --keyring "/etc/apt/trusted.gpg.d/{{ source.name }}.gpg" add - && \
-    echo "deb [signed-by=/etc/apt/trusted.gpg.d/{{ source.name }}.gpg] {{ source.deb.url }} {{ source.deb.distribution }} {{ source.deb.component }}" > "/etc/apt/sources.list.d/{{ source.name }}.list"
+      {% if source.dearmor %}
+RUN curl -fsSL "{{ source.key_url }}" | gpg --dearmor -o "/usr/share/keyrings/{{ source.name }}.gpg"
+      {% else %}
+RUN curl -fsSL "{{ source.key_url }}" --output "/usr/share/keyrings/{{ source.name }}.gpg"
+      {% endif %}
+RUN echo "deb [signed-by=/usr/share/keyrings/{{ source.name }}.gpg] {{ source.deb.url }} {{ source.deb.distribution }} {{ source.deb.component }}" > "/etc/apt/sources.list.d/{{ source.name }}.list"
     {% endfor %}
 RUN DEBIAN_FRONTEND=noninteractive apt-get update -y && \
     DEBIAN_FRONTEND=noninteractive apt-get dist-upgrade -y
   {% endif %}
 {% endblock %}
 
 {% block apt %}
```

### Comparing `ou_container_builder-2.3.0/ou_container_builder/templates/core/content/content_config.yaml` & `ou_container_builder-2.4.0/ou_container_builder/templates/core/content/content_config.yaml`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.3.0/ou_container_builder/templates/packs/code_server/vscode.svg` & `ou_container_builder-2.4.0/ou_container_builder/templates/packs/code_server/vscode.svg`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.3.0/ou_container_builder/templates/packs/mariadb/setup.sh` & `ou_container_builder-2.4.0/ou_container_builder/templates/packs/mariadb/setup.sh`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.3.0/ou_container_builder/templates/packs/tutorial-server/production.ini` & `ou_container_builder-2.4.0/ou_container_builder/templates/packs/tutorial-server/production.ini`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.3.0/ou_container_builder/utils.py` & `ou_container_builder-2.4.0/ou_container_builder/utils.py`

 * *Files identical despite different names*

### Comparing `ou_container_builder-2.3.0/ou_container_builder/validator.py` & `ou_container_builder-2.4.0/ou_container_builder/validator.py`

 * *Files 1% similar despite different names*

```diff
@@ -149,14 +149,19 @@
                             'empty': False
                         },
                         'key_url': {
                             'type': 'string',
                             'required': True,
                             'empty': False,
                         },
+                        'dearmor': {
+                            'type': 'boolean',
+                            'required': False,
+                            'default': True
+                        },
                         'deb': {
                             'type': 'dict',
                             'required': True,
                             'schema': {
                                 'url': {
                                     'type': 'string',
                                     'required': True,
```

### Comparing `ou_container_builder-2.3.0/pyproject.toml` & `ou_container_builder-2.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ou-container-builder"
-version = "2.3.0"
+version = "2.4.0"
 description = ""
 authors = ["Mark Hall <mark.hall@open.ac.uk>"]
 
 [tool.poetry.dependencies]
 python = "^3.7"
 pyyaml = "^5.4.1"
 jinja2 = "^3.0.0"
```

### Comparing `ou_container_builder-2.3.0/PKG-INFO` & `ou_container_builder-2.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ou-container-builder
-Version: 2.3.0
+Version: 2.4.0
 Summary: 
 Author: Mark Hall
 Author-email: mark.hall@open.ac.uk
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

