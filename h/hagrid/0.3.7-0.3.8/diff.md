# Comparing `tmp/hagrid-0.3.7.tar.gz` & `tmp/hagrid-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hagrid-0.3.7.tar", last modified: Fri Apr 28 06:16:02 2023, max compression
+gzip compressed data, was "hagrid-0.3.8.tar", last modified: Fri May  5 03:25:15 2023, max compression
```

## Comparing `hagrid-0.3.7.tar` & `hagrid-0.3.8.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 06:16:02.879761 hagrid-0.3.7/
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-28 06:16:02.875761 hagrid-0.3.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7377 2023-04-28 06:13:50.000000 hagrid-0.3.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 06:16:02.875761 hagrid-0.3.7/hagrid/
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-04-28 06:13:50.000000 hagrid-0.3.7/hagrid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5882 2023-04-28 06:13:50.000000 hagrid-0.3.7/hagrid/art.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-28 06:13:50.000000 hagrid-0.3.7/hagrid/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-04-28 06:13:50.000000 hagrid-0.3.7/hagrid/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-04-28 06:13:50.000000 hagrid-0.3.7/hagrid/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)   134867 2023-04-28 06:13:50.000000 hagrid-0.3.7/hagrid/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    30059 2023-04-28 06:13:50.000000 hagrid-0.3.7/hagrid/deps.py
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-28 06:13:50.000000 hagrid-0.3.7/hagrid/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-28 06:13:50.000000 hagrid-0.3.7/hagrid/file.py
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-28 06:13:50.000000 hagrid-0.3.7/hagrid/git_check.py
--rw-r--r--   0 runner    (1001) docker     (123)    12046 2023-04-28 06:13:50.000000 hagrid-0.3.7/hagrid/grammar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-04-28 06:13:50.000000 hagrid-0.3.7/hagrid/land.py
--rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-04-28 06:13:50.000000 hagrid-0.3.7/hagrid/launch.py
--rw-r--r--   0 runner    (1001) docker     (123)    13852 2023-04-28 06:13:50.000000 hagrid-0.3.7/hagrid/lib.py
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-04-28 06:14:05.000000 hagrid-0.3.7/hagrid/manifest_template.yml
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-04-28 06:13:50.000000 hagrid-0.3.7/hagrid/mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-04-28 06:13:50.000000 hagrid-0.3.7/hagrid/names.py
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-28 06:13:50.000000 hagrid-0.3.7/hagrid/nb_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     8463 2023-04-28 06:13:50.000000 hagrid-0.3.7/hagrid/orchestra.py
--rw-r--r--   0 runner    (1001) docker     (123)     6043 2023-04-28 06:13:50.000000 hagrid-0.3.7/hagrid/parse_template.py
--rw-r--r--   0 runner    (1001) docker     (123)    10203 2023-04-28 06:13:50.000000 hagrid-0.3.7/hagrid/quickstart_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-04-28 06:13:50.000000 hagrid-0.3.7/hagrid/rand_sec.py
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-04-28 06:13:50.000000 hagrid-0.3.7/hagrid/style.py
--rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-04-28 06:13:50.000000 hagrid-0.3.7/hagrid/util.py
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-28 06:14:05.000000 hagrid-0.3.7/hagrid/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     7950 2023-04-28 06:13:50.000000 hagrid-0.3.7/hagrid/win_bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-04-28 06:13:50.000000 hagrid-0.3.7/hagrid/wizard_ui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 06:16:02.875761 hagrid-0.3.7/hagrid.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-28 06:16:02.000000 hagrid-0.3.7/hagrid.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-04-28 06:16:02.000000 hagrid-0.3.7/hagrid.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 06:16:02.000000 hagrid-0.3.7/hagrid.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-28 06:16:02.000000 hagrid-0.3.7/hagrid.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-28 06:16:02.000000 hagrid-0.3.7/hagrid.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-28 06:16:02.000000 hagrid-0.3.7/hagrid.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 06:16:02.879761 hagrid-0.3.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-04-28 06:14:05.000000 hagrid-0.3.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 06:16:02.875761 hagrid-0.3.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 06:13:50.000000 hagrid-0.3.7/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 06:16:02.875761 hagrid-0.3.7/tests/hagrid/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 06:13:50.000000 hagrid-0.3.7/tests/hagrid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6784 2023-04-28 06:13:50.000000 hagrid-0.3.7/tests/hagrid/cli_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 03:25:15.429014 hagrid-0.3.8/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-05 03:25:15.429014 hagrid-0.3.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7377 2023-05-05 03:22:19.000000 hagrid-0.3.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 03:25:15.429014 hagrid-0.3.8/hagrid/
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-05-05 03:22:19.000000 hagrid-0.3.8/hagrid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5882 2023-05-05 03:22:19.000000 hagrid-0.3.8/hagrid/art.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-05 03:22:19.000000 hagrid-0.3.8/hagrid/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-05-05 03:22:19.000000 hagrid-0.3.8/hagrid/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-05-05 03:22:19.000000 hagrid-0.3.8/hagrid/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)   134867 2023-05-05 03:22:19.000000 hagrid-0.3.8/hagrid/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30059 2023-05-05 03:22:19.000000 hagrid-0.3.8/hagrid/deps.py
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-05 03:22:19.000000 hagrid-0.3.8/hagrid/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-05 03:22:19.000000 hagrid-0.3.8/hagrid/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-05-05 03:22:19.000000 hagrid-0.3.8/hagrid/git_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12046 2023-05-05 03:22:19.000000 hagrid-0.3.8/hagrid/grammar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-05-05 03:22:19.000000 hagrid-0.3.8/hagrid/land.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-05-05 03:22:19.000000 hagrid-0.3.8/hagrid/launch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13852 2023-05-05 03:22:19.000000 hagrid-0.3.8/hagrid/lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-05-05 03:24:13.000000 hagrid-0.3.8/hagrid/manifest_template.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-05-05 03:22:19.000000 hagrid-0.3.8/hagrid/mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-05-05 03:22:19.000000 hagrid-0.3.8/hagrid/names.py
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-05 03:22:19.000000 hagrid-0.3.8/hagrid/nb_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8463 2023-05-05 03:22:19.000000 hagrid-0.3.8/hagrid/orchestra.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6043 2023-05-05 03:22:19.000000 hagrid-0.3.8/hagrid/parse_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10203 2023-05-05 03:22:19.000000 hagrid-0.3.8/hagrid/quickstart_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-05-05 03:22:19.000000 hagrid-0.3.8/hagrid/rand_sec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-05-05 03:22:19.000000 hagrid-0.3.8/hagrid/style.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-05-05 03:22:19.000000 hagrid-0.3.8/hagrid/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-05 03:22:38.000000 hagrid-0.3.8/hagrid/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7950 2023-05-05 03:22:19.000000 hagrid-0.3.8/hagrid/win_bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-05-05 03:22:19.000000 hagrid-0.3.8/hagrid/wizard_ui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 03:25:15.429014 hagrid-0.3.8/hagrid.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-05 03:25:15.000000 hagrid-0.3.8/hagrid.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-05-05 03:25:15.000000 hagrid-0.3.8/hagrid.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 03:25:15.000000 hagrid-0.3.8/hagrid.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-05 03:25:15.000000 hagrid-0.3.8/hagrid.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-05 03:25:15.000000 hagrid-0.3.8/hagrid.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-05 03:25:15.000000 hagrid-0.3.8/hagrid.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 03:25:15.429014 hagrid-0.3.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-05-05 03:22:38.000000 hagrid-0.3.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 03:25:15.429014 hagrid-0.3.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 03:22:19.000000 hagrid-0.3.8/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 03:25:15.429014 hagrid-0.3.8/tests/hagrid/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 03:22:19.000000 hagrid-0.3.8/tests/hagrid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6784 2023-05-05 03:22:19.000000 hagrid-0.3.8/tests/hagrid/cli_test.py
```

### Comparing `hagrid-0.3.7/README.md` & `hagrid-0.3.8/README.md`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.7/hagrid/__init__.py` & `hagrid-0.3.8/hagrid/__init__.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.7/hagrid/art.py` & `hagrid-0.3.8/hagrid/art.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.7/hagrid/auth.py` & `hagrid-0.3.8/hagrid/auth.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.7/hagrid/azure.py` & `hagrid-0.3.8/hagrid/azure.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.7/hagrid/cache.py` & `hagrid-0.3.8/hagrid/cache.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.7/hagrid/cli.py` & `hagrid-0.3.8/hagrid/cli.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.7/hagrid/deps.py` & `hagrid-0.3.8/hagrid/deps.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.7/hagrid/grammar.py` & `hagrid-0.3.8/hagrid/grammar.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.7/hagrid/land.py` & `hagrid-0.3.8/hagrid/land.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.7/hagrid/launch.py` & `hagrid-0.3.8/hagrid/launch.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.7/hagrid/lib.py` & `hagrid-0.3.8/hagrid/lib.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.7/hagrid/manifest_template.yml` & `hagrid-0.3.8/hagrid/manifest_template.yml`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 manifestVersion: 0.1
-hagrid_version: 0.3.7
-syft_version: 0.8.0
-dockerTag: 0.8.0
+hagrid_version: 0.3.8
+syft_version: 0.8.1-beta.0
+dockerTag: 0.8.1-beta.0
 baseUrl: https://raw.githubusercontent.com/OpenMined/PySyft/
-hash: 65a6ec9eb935fc0f190ff16ea04edecfbdba9e49
+hash: d80af183671ff8e27ed7b070f963c93039135fa8
 target_dir: ~/.hagrid/PySyft/
 files:
   grid:
     path: packages/grid/
     common:
-    - rabbitmq/rabbitmq.conf
-    - redis/redis.conf
-    - seaweedfs/filer.toml
-    - seaweedfs/s3config.json
-    - vpn/config.yaml
+      - rabbitmq/rabbitmq.conf
+      - redis/redis.conf
+      - seaweedfs/filer.toml
+      - seaweedfs/s3config.json
+      - vpn/config.yaml
     docker:
-    - .env
-    - docker-compose.build.yml
-    - docker-compose.dev.yml
-    - docker-compose.test.yml
-    - docker-compose.tls.yml
-    - docker-compose.yml
-    - traefik/docker/dynamic-tls.yml
-    - traefik/docker/dynamic.yml
-    - traefik/docker/traefik-tls.template.yml
-    - traefik/docker/traefik.yml
-    - vpn/headscale.dockerfile
-    - vpn/tailscale.dockerfile
+      - .env
+      - docker-compose.build.yml
+      - docker-compose.dev.yml
+      - docker-compose.test.yml
+      - docker-compose.tls.yml
+      - docker-compose.yml
+      - traefik/docker/dynamic-tls.yml
+      - traefik/docker/dynamic.yml
+      - traefik/docker/traefik-tls.template.yml
+      - traefik/docker/traefik.yml
+      - vpn/headscale.dockerfile
+      - vpn/tailscale.dockerfile
     k8s:
-    - devspace.yaml
-    - traefik/k8s/dynamic.yml
-    - traefik/k8s/traefik.yml
+      - devspace.yaml
+      - traefik/k8s/dynamic.yml
+      - traefik/k8s/traefik.yml
```

### Comparing `hagrid-0.3.7/hagrid/mode.py` & `hagrid-0.3.8/hagrid/mode.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.7/hagrid/names.py` & `hagrid-0.3.8/hagrid/names.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.7/hagrid/orchestra.py` & `hagrid-0.3.8/hagrid/orchestra.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.7/hagrid/parse_template.py` & `hagrid-0.3.8/hagrid/parse_template.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.7/hagrid/quickstart_ui.py` & `hagrid-0.3.8/hagrid/quickstart_ui.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.7/hagrid/rand_sec.py` & `hagrid-0.3.8/hagrid/rand_sec.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.7/hagrid/style.py` & `hagrid-0.3.8/hagrid/style.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.7/hagrid/util.py` & `hagrid-0.3.8/hagrid/util.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.7/hagrid/win_bootstrap.py` & `hagrid-0.3.8/hagrid/win_bootstrap.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.7/hagrid/wizard_ui.py` & `hagrid-0.3.8/hagrid/wizard_ui.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.7/hagrid.egg-info/SOURCES.txt` & `hagrid-0.3.8/hagrid.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.7/setup.py` & `hagrid-0.3.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # stdlib
 import platform
 
 # third party
 from setuptools import find_packages
 from setuptools import setup
 
-__version__ = "0.3.7"
+__version__ = "0.3.8"
 
 DATA_FILES = {"img": ["hagrid/img/*.png"], "hagrid": ["*.yml"]}
 
 packages = [
     "ascii_magic",
     "click>=7.1",
     "cryptography>=37.0.2",
```

### Comparing `hagrid-0.3.7/tests/hagrid/cli_test.py` & `hagrid-0.3.8/tests/hagrid/cli_test.py`

 * *Files identical despite different names*

