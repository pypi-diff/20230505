# Comparing `tmp/afex-sso-0.0.41.tar.gz` & `tmp/afex-sso-0.0.42.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "afex-sso-0.0.41.tar", last modified: Mon Mar 27 13:17:10 2023, max compression
+gzip compressed data, was "afex-sso-0.0.42.tar", last modified: Fri May  5 12:15:58 2023, max compression
```

## Comparing `afex-sso-0.0.41.tar` & `afex-sso-0.0.42.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-03-27 13:17:10.047325 afex-sso-0.0.41/
--rw-r--r--   0 mac        (501) staff       (20)     1063 2023-03-04 00:13:16.000000 afex-sso-0.0.41/LICENSE
--rw-r--r--   0 mac        (501) staff       (20)     1353 2023-03-27 13:17:10.047402 afex-sso-0.0.41/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)      911 2023-03-27 13:13:14.000000 afex-sso-0.0.41/README.md
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-03-27 13:17:10.044682 afex-sso-0.0.41/app/
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-03-27 13:17:10.045847 afex-sso-0.0.41/app/AFEX_SSO/
--rw-r--r--   0 mac        (501) staff       (20)       33 2023-03-20 23:30:24.000000 afex-sso-0.0.41/app/AFEX_SSO/__init__.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-03-27 13:17:10.046529 afex-sso-0.0.41/app/AFEX_SSO/src/
--rw-r--r--   0 mac        (501) staff       (20)        0 2023-03-20 23:17:21.000000 afex-sso-0.0.41/app/AFEX_SSO/src/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)     1202 2023-03-23 15:01:53.000000 afex-sso-0.0.41/app/AFEX_SSO/src/sso.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-03-27 13:17:10.047194 afex-sso-0.0.41/app/afex_sso.egg-info/
--rw-r--r--   0 mac        (501) staff       (20)     1353 2023-03-27 13:17:09.000000 afex-sso-0.0.41/app/afex_sso.egg-info/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)      308 2023-03-27 13:17:09.000000 afex-sso-0.0.41/app/afex_sso.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (501) staff       (20)        1 2023-03-27 13:17:09.000000 afex-sso-0.0.41/app/afex_sso.egg-info/dependency_links.txt
--rw-r--r--   0 mac        (501) staff       (20)       61 2023-03-27 13:17:09.000000 afex-sso-0.0.41/app/afex_sso.egg-info/requires.txt
--rw-r--r--   0 mac        (501) staff       (20)        9 2023-03-27 13:17:09.000000 afex-sso-0.0.41/app/afex_sso.egg-info/top_level.txt
--rw-r--r--   0 mac        (501) staff       (20)      134 2023-03-15 21:51:52.000000 afex-sso-0.0.41/pyproject.toml
--rw-r--r--   0 mac        (501) staff       (20)      474 2023-03-27 13:17:10.047668 afex-sso-0.0.41/setup.cfg
--rw-r--r--   0 mac        (501) staff       (20)      799 2023-03-27 13:15:43.000000 afex-sso-0.0.41/setup.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-05-05 12:15:58.201666 afex-sso-0.0.42/
+-rw-r--r--   0 mac        (501) staff       (20)     1063 2023-03-04 00:13:16.000000 afex-sso-0.0.42/LICENSE
+-rw-r--r--   0 mac        (501) staff       (20)     1356 2023-05-05 12:15:58.201758 afex-sso-0.0.42/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)      911 2023-03-27 13:13:14.000000 afex-sso-0.0.42/README.md
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-05-05 12:15:58.199004 afex-sso-0.0.42/app/
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-05-05 12:15:58.200139 afex-sso-0.0.42/app/AFEX_SSO/
+-rw-r--r--   0 mac        (501) staff       (20)       33 2023-03-20 23:30:24.000000 afex-sso-0.0.42/app/AFEX_SSO/__init__.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-05-05 12:15:58.200633 afex-sso-0.0.42/app/AFEX_SSO/src/
+-rw-r--r--   0 mac        (501) staff       (20)        0 2023-03-20 23:17:21.000000 afex-sso-0.0.42/app/AFEX_SSO/src/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)     1184 2023-05-05 11:28:13.000000 afex-sso-0.0.42/app/AFEX_SSO/src/sso.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-05-05 12:15:58.201405 afex-sso-0.0.42/app/afex_sso.egg-info/
+-rw-r--r--   0 mac        (501) staff       (20)     1356 2023-05-05 12:15:58.000000 afex-sso-0.0.42/app/afex_sso.egg-info/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)      308 2023-05-05 12:15:58.000000 afex-sso-0.0.42/app/afex_sso.egg-info/SOURCES.txt
+-rw-r--r--   0 mac        (501) staff       (20)        1 2023-05-05 12:15:58.000000 afex-sso-0.0.42/app/afex_sso.egg-info/dependency_links.txt
+-rw-r--r--   0 mac        (501) staff       (20)       61 2023-05-05 12:15:58.000000 afex-sso-0.0.42/app/afex_sso.egg-info/requires.txt
+-rw-r--r--   0 mac        (501) staff       (20)        9 2023-05-05 12:15:58.000000 afex-sso-0.0.42/app/afex_sso.egg-info/top_level.txt
+-rw-r--r--   0 mac        (501) staff       (20)      134 2023-03-15 21:51:52.000000 afex-sso-0.0.42/pyproject.toml
+-rw-r--r--   0 mac        (501) staff       (20)      474 2023-05-05 12:15:58.202039 afex-sso-0.0.42/setup.cfg
+-rw-r--r--   0 mac        (501) staff       (20)      802 2023-05-05 12:15:04.000000 afex-sso-0.0.42/setup.py
```

### Comparing `afex-sso-0.0.41/LICENSE` & `afex-sso-0.0.42/LICENSE`

 * *Files identical despite different names*

### Comparing `afex-sso-0.0.41/PKG-INFO` & `afex-sso-0.0.42/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: afex-sso
-Version: 0.0.41
+Version: 0.0.42
 Summary: For integrating sso
 Home-page: UNKNOWN
 Author: AFEX NIGERIA
-Author-email: it@afexnigeria.com
+Author-email: it@africaexchange.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 
 # AFEX SSO (DJANGO)
```

### Comparing `afex-sso-0.0.41/README.md` & `afex-sso-0.0.42/README.md`

 * *Files identical despite different names*

### Comparing `afex-sso-0.0.41/app/AFEX_SSO/src/sso.py` & `afex-sso-0.0.42/app/AFEX_SSO/src/sso.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,9 +37,7 @@
             response = requests.get(
                 f"{URL}/v1/api/verify_sp/{session_key}", headers=headers)
             data = json.loads(response.text)
             return data
 
         except Exception as e:
             return f"Something went wrong, please confirm the credentials and try again: {e}"
-
-SSO("afex", "")()
```

### Comparing `afex-sso-0.0.41/app/afex_sso.egg-info/PKG-INFO` & `afex-sso-0.0.42/app/afex_sso.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: afex-sso
-Version: 0.0.41
+Version: 0.0.42
 Summary: For integrating sso
 Home-page: UNKNOWN
 Author: AFEX NIGERIA
-Author-email: it@afexnigeria.com
+Author-email: it@africaexchange.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 
 # AFEX SSO (DJANGO)
```

### Comparing `afex-sso-0.0.41/setup.py` & `afex-sso-0.0.42/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,28 +3,28 @@
 from setuptools import find_packages, setup
 
 with open("./README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="afex-sso",
-    version="0.0.41",
+    version="0.0.42",
     description="For integrating sso",
     package_dir={"": "app"},
     packages=find_packages(where="app"),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
     author="AFEX NIGERIA",
-    author_email="it@afexnigeria.com",
+    author_email="it@africaexchange.com",
     license="MIT",
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3.8",
         "Operating System :: OS Independent",
     ],
     install_requires=["requests >= 2.28.2", "django>=4.1"],
     extras_require={
         "dev": ["pytest>=7.0", "twine>=4.0.2"],
     },
-    python_requires=">=3.8",
+    python_requires=">=3.7",
 )
```

