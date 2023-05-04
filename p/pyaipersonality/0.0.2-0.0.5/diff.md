# Comparing `tmp/pyaipersonality-0.0.2.tar.gz` & `tmp/pyaipersonality-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyaipersonality-0.0.2.tar", last modified: Sat Apr 29 08:59:21 2023, max compression
+gzip compressed data, was "pyaipersonality-0.0.5.tar", last modified: Thu May  4 22:57:43 2023, max compression
```

## Comparing `pyaipersonality-0.0.2.tar` & `pyaipersonality-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-29 08:59:21.847112 pyaipersonality-0.0.2/
--rw-rw-rw-   0        0        0    11558 2023-04-29 07:11:51.000000 pyaipersonality-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     1667 2023-04-29 08:59:21.846116 pyaipersonality-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1174 2023-04-29 08:19:53.000000 pyaipersonality-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-29 08:59:21.838113 pyaipersonality-0.0.2/pyaipersonality/
--rw-rw-rw-   0        0        0     5340 2023-04-29 08:54:25.000000 pyaipersonality-0.0.2/pyaipersonality/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-29 08:59:21.845112 pyaipersonality-0.0.2/pyaipersonality.egg-info/
--rw-rw-rw-   0        0        0     1667 2023-04-29 08:59:21.000000 pyaipersonality-0.0.2/pyaipersonality.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      248 2023-04-29 08:59:21.000000 pyaipersonality-0.0.2/pyaipersonality.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-29 08:59:21.000000 pyaipersonality-0.0.2/pyaipersonality.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2023-04-29 08:59:21.000000 pyaipersonality-0.0.2/pyaipersonality.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-04-29 08:59:21.000000 pyaipersonality-0.0.2/pyaipersonality.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-29 08:59:21.847112 pyaipersonality-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1075 2023-04-29 08:59:11.000000 pyaipersonality-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-04 22:57:43.917258 pyaipersonality-0.0.5/
+-rw-rw-rw-   0        0        0    11558 2023-04-29 07:11:51.000000 pyaipersonality-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0     8362 2023-05-04 22:57:43.917258 pyaipersonality-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     7869 2023-05-04 22:49:56.000000 pyaipersonality-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-05-04 22:57:43.899259 pyaipersonality-0.0.5/pyaipersonality/
+-rw-rw-rw-   0        0        0     8393 2023-05-04 22:36:59.000000 pyaipersonality-0.0.5/pyaipersonality/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-04 22:57:43.915263 pyaipersonality-0.0.5/pyaipersonality.egg-info/
+-rw-rw-rw-   0        0        0     8362 2023-05-04 22:57:43.000000 pyaipersonality-0.0.5/pyaipersonality.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      248 2023-05-04 22:57:43.000000 pyaipersonality-0.0.5/pyaipersonality.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-04 22:57:43.000000 pyaipersonality-0.0.5/pyaipersonality.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2023-05-04 22:57:43.000000 pyaipersonality-0.0.5/pyaipersonality.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-05-04 22:57:43.000000 pyaipersonality-0.0.5/pyaipersonality.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-04 22:57:43.917258 pyaipersonality-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1075 2023-05-04 21:34:14.000000 pyaipersonality-0.0.5/setup.py
```

### Comparing `pyaipersonality-0.0.2/LICENSE` & `pyaipersonality-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyaipersonality-0.0.2/setup.py` & `pyaipersonality-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 
 requirements = read_requirements("requirements.txt")
 requirements_dev = read_requirements("requirements_dev.txt")
 
 setuptools.setup(
     name="pyaipersonality",
-    version="0.0.2",
+    version="0.0.5",
     author="Saifeddine ALOUI",
     author_email="aloui.saifeddine@gmail.com",
     description="A python library for AI personality definition",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ParisNeo/PyAIPersonality",
     packages=setuptools.find_packages(),
```

