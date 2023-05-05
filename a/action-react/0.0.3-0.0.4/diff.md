# Comparing `tmp/action-react-0.0.3.tar.gz` & `tmp/action-react-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/action-react-0.0.3.tar", last modified: Fri May  5 00:55:50 2023, max compression
+gzip compressed data, was "dist/action-react-0.0.4.tar", last modified: Fri May  5 02:42:33 2023, max compression
```

## Comparing `action-react-0.0.3.tar` & `action-react-0.0.4.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 wyu        (501) staff       (20)        0 2023-05-05 00:55:50.000000 action-react-0.0.3/
-drwxr-xr-x   0 wyu        (501) staff       (20)        0 2023-05-05 00:55:50.000000 action-react-0.0.3/.github/
-drwxr-xr-x   0 wyu        (501) staff       (20)        0 2023-05-05 00:55:50.000000 action-react-0.0.3/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 wyu        (501) staff       (20)      834 2023-03-26 23:10:55.000000 action-react-0.0.3/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 wyu        (501) staff       (20)      595 2023-03-26 23:10:55.000000 action-react-0.0.3/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 wyu        (501) staff       (20)      118 2023-03-26 23:10:55.000000 action-react-0.0.3/.github/dependabot.yml
-drwxr-xr-x   0 wyu        (501) staff       (20)        0 2023-05-05 00:55:50.000000 action-react-0.0.3/.github/workflows/
--rw-r--r--   0 wyu        (501) staff       (20)     1097 2023-03-26 23:10:55.000000 action-react-0.0.3/.github/workflows/build.yml
--rw-r--r--   0 wyu        (501) staff       (20)     1848 2023-04-05 01:58:18.000000 action-react-0.0.3/.gitignore
--rw-r--r--   0 wyu        (501) staff       (20)     1022 2023-03-26 23:30:54.000000 action-react-0.0.3/CONTRIBUTING.md
--rw-r--r--   0 wyu        (501) staff       (20)    11357 2023-03-26 23:10:55.000000 action-react-0.0.3/LICENSE
--rw-r--r--   0 wyu        (501) staff       (20)     2622 2023-04-05 14:52:29.000000 action-react-0.0.3/Makefile
--rw-r--r--   0 wyu        (501) staff       (20)    15688 2023-05-05 00:55:50.000000 action-react-0.0.3/PKG-INFO
--rw-r--r--   0 wyu        (501) staff       (20)     1921 2023-04-05 14:52:29.000000 action-react-0.0.3/README.md
-drwxr-xr-x   0 wyu        (501) staff       (20)        0 2023-05-05 00:55:50.000000 action-react-0.0.3/action_react/
--rw-r--r--   0 wyu        (501) staff       (20)     4217 2023-05-05 00:08:49.000000 action-react-0.0.3/action_react/main.py
--rw-r--r--   0 wyu        (501) staff       (20)     2426 2023-05-05 00:47:23.000000 action-react-0.0.3/action_react/react.py
-drwxr-xr-x   0 wyu        (501) staff       (20)        0 2023-05-05 00:55:50.000000 action-react-0.0.3/action_react/tests/
-drwxr-xr-x   0 wyu        (501) staff       (20)        0 2023-05-05 00:55:50.000000 action-react-0.0.3/action_react/tests/fixtures/
--rw-r--r--   0 wyu        (501) staff       (20)      159 2023-03-26 23:10:55.000000 action-react-0.0.3/action_react/tests/fixtures/config.ini
--rw-r--r--   0 wyu        (501) staff       (20)     2054 2023-03-26 23:10:55.000000 action-react-0.0.3/action_react/tests/test_all.py
-drwxr-xr-x   0 wyu        (501) staff       (20)        0 2023-05-05 00:55:50.000000 action-react-0.0.3/action_react.egg-info/
--rw-r--r--   0 wyu        (501) staff       (20)    15688 2023-05-05 00:55:50.000000 action-react-0.0.3/action_react.egg-info/PKG-INFO
--rw-r--r--   0 wyu        (501) staff       (20)      582 2023-05-05 00:55:50.000000 action-react-0.0.3/action_react.egg-info/SOURCES.txt
--rw-r--r--   0 wyu        (501) staff       (20)        1 2023-05-05 00:55:50.000000 action-react-0.0.3/action_react.egg-info/dependency_links.txt
--rw-r--r--   0 wyu        (501) staff       (20)      204 2023-05-05 00:55:50.000000 action-react-0.0.3/action_react.egg-info/requires.txt
--rw-r--r--   0 wyu        (501) staff       (20)       13 2023-05-05 00:55:50.000000 action-react-0.0.3/action_react.egg-info/top_level.txt
--rw-r--r--   0 wyu        (501) staff       (20)      198 2023-03-26 23:10:55.000000 action-react-0.0.3/config.ini
-drwxr-xr-x   0 wyu        (501) staff       (20)        0 2023-05-05 00:55:50.000000 action-react-0.0.3/docs/
--rw-r--r--   0 wyu        (501) staff       (20)      634 2023-04-05 01:53:42.000000 action-react-0.0.3/docs/Makefile
--rw-r--r--   0 wyu        (501) staff       (20)     2252 2023-04-05 15:48:54.000000 action-react-0.0.3/docs/conf.py
--rw-r--r--   0 wyu        (501) staff       (20)     2201 2023-04-05 14:52:29.000000 action-react-0.0.3/docs/index.md
--rw-r--r--   0 wyu        (501) staff       (20)      800 2023-04-05 01:53:42.000000 action-react-0.0.3/docs/make.bat
--rw-r--r--   0 wyu        (501) staff       (20)     2235 2023-05-05 00:11:22.000000 action-react-0.0.3/pyproject.toml
--rw-r--r--   0 wyu        (501) staff       (20)       48 2023-05-04 23:55:50.000000 action-react-0.0.3/requirements.txt
--rw-r--r--   0 wyu        (501) staff       (20)       38 2023-05-05 00:55:50.000000 action-react-0.0.3/setup.cfg
--rw-r--r--   0 wyu        (501) staff       (20)       39 2023-03-26 23:10:55.000000 action-react-0.0.3/setup.py
+drwxr-xr-x   0 wyu        (501) staff       (20)        0 2023-05-05 02:42:33.000000 action-react-0.0.4/
+drwxr-xr-x   0 wyu        (501) staff       (20)        0 2023-05-05 02:42:33.000000 action-react-0.0.4/.github/
+drwxr-xr-x   0 wyu        (501) staff       (20)        0 2023-05-05 02:42:33.000000 action-react-0.0.4/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 wyu        (501) staff       (20)      834 2023-03-26 23:10:55.000000 action-react-0.0.4/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 wyu        (501) staff       (20)      595 2023-03-26 23:10:55.000000 action-react-0.0.4/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 wyu        (501) staff       (20)      118 2023-03-26 23:10:55.000000 action-react-0.0.4/.github/dependabot.yml
+drwxr-xr-x   0 wyu        (501) staff       (20)        0 2023-05-05 02:42:33.000000 action-react-0.0.4/.github/workflows/
+-rw-r--r--   0 wyu        (501) staff       (20)     1097 2023-03-26 23:10:55.000000 action-react-0.0.4/.github/workflows/build.yml
+-rw-r--r--   0 wyu        (501) staff       (20)     1848 2023-04-05 01:58:18.000000 action-react-0.0.4/.gitignore
+-rw-r--r--   0 wyu        (501) staff       (20)     1022 2023-03-26 23:30:54.000000 action-react-0.0.4/CONTRIBUTING.md
+-rw-r--r--   0 wyu        (501) staff       (20)    11357 2023-03-26 23:10:55.000000 action-react-0.0.4/LICENSE
+-rw-r--r--   0 wyu        (501) staff       (20)     2622 2023-04-05 14:52:29.000000 action-react-0.0.4/Makefile
+-rw-r--r--   0 wyu        (501) staff       (20)    15688 2023-05-05 02:42:33.000000 action-react-0.0.4/PKG-INFO
+-rw-r--r--   0 wyu        (501) staff       (20)     1921 2023-04-05 14:52:29.000000 action-react-0.0.4/README.md
+drwxr-xr-x   0 wyu        (501) staff       (20)        0 2023-05-05 02:42:33.000000 action-react-0.0.4/action_react/
+-rw-r--r--   0 wyu        (501) staff       (20)     4217 2023-05-05 00:08:49.000000 action-react-0.0.4/action_react/main.py
+-rw-r--r--   0 wyu        (501) staff       (20)     2814 2023-05-05 02:41:58.000000 action-react-0.0.4/action_react/react.py
+drwxr-xr-x   0 wyu        (501) staff       (20)        0 2023-05-05 02:42:33.000000 action-react-0.0.4/action_react/tests/
+drwxr-xr-x   0 wyu        (501) staff       (20)        0 2023-05-05 02:42:33.000000 action-react-0.0.4/action_react/tests/fixtures/
+-rw-r--r--   0 wyu        (501) staff       (20)      159 2023-03-26 23:10:55.000000 action-react-0.0.4/action_react/tests/fixtures/config.ini
+-rw-r--r--   0 wyu        (501) staff       (20)     2054 2023-03-26 23:10:55.000000 action-react-0.0.4/action_react/tests/test_all.py
+drwxr-xr-x   0 wyu        (501) staff       (20)        0 2023-05-05 02:42:33.000000 action-react-0.0.4/action_react.egg-info/
+-rw-r--r--   0 wyu        (501) staff       (20)    15688 2023-05-05 02:42:33.000000 action-react-0.0.4/action_react.egg-info/PKG-INFO
+-rw-r--r--   0 wyu        (501) staff       (20)      582 2023-05-05 02:42:33.000000 action-react-0.0.4/action_react.egg-info/SOURCES.txt
+-rw-r--r--   0 wyu        (501) staff       (20)        1 2023-05-05 02:42:33.000000 action-react-0.0.4/action_react.egg-info/dependency_links.txt
+-rw-r--r--   0 wyu        (501) staff       (20)      204 2023-05-05 02:42:33.000000 action-react-0.0.4/action_react.egg-info/requires.txt
+-rw-r--r--   0 wyu        (501) staff       (20)       13 2023-05-05 02:42:33.000000 action-react-0.0.4/action_react.egg-info/top_level.txt
+-rw-r--r--   0 wyu        (501) staff       (20)      198 2023-03-26 23:10:55.000000 action-react-0.0.4/config.ini
+drwxr-xr-x   0 wyu        (501) staff       (20)        0 2023-05-05 02:42:33.000000 action-react-0.0.4/docs/
+-rw-r--r--   0 wyu        (501) staff       (20)      634 2023-04-05 01:53:42.000000 action-react-0.0.4/docs/Makefile
+-rw-r--r--   0 wyu        (501) staff       (20)     2252 2023-04-05 15:48:54.000000 action-react-0.0.4/docs/conf.py
+-rw-r--r--   0 wyu        (501) staff       (20)     2201 2023-05-05 02:15:02.000000 action-react-0.0.4/docs/index.md
+-rw-r--r--   0 wyu        (501) staff       (20)      800 2023-04-05 01:53:42.000000 action-react-0.0.4/docs/make.bat
+-rw-r--r--   0 wyu        (501) staff       (20)     2235 2023-05-05 02:41:58.000000 action-react-0.0.4/pyproject.toml
+-rw-r--r--   0 wyu        (501) staff       (20)       48 2023-05-04 23:55:50.000000 action-react-0.0.4/requirements.txt
+-rw-r--r--   0 wyu        (501) staff       (20)       38 2023-05-05 02:42:33.000000 action-react-0.0.4/setup.cfg
+-rw-r--r--   0 wyu        (501) staff       (20)       39 2023-03-26 23:10:55.000000 action-react-0.0.4/setup.py
```

### Comparing `action-react-0.0.3/.github/ISSUE_TEMPLATE/bug_report.md` & `action-react-0.0.4/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `action-react-0.0.3/.github/ISSUE_TEMPLATE/feature_request.md` & `action-react-0.0.4/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `action-react-0.0.3/.github/workflows/build.yml` & `action-react-0.0.4/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `action-react-0.0.3/.gitignore` & `action-react-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `action-react-0.0.3/CONTRIBUTING.md` & `action-react-0.0.4/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `action-react-0.0.3/LICENSE` & `action-react-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `action-react-0.0.3/Makefile` & `action-react-0.0.4/Makefile`

 * *Files identical despite different names*

### Comparing `action-react-0.0.3/PKG-INFO` & `action-react-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: action-react
-Version: 0.0.3
+Version: 0.0.4
 Summary: telegram listener tool
 Author-email: yd-wu <yw3960@columbia.edu>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `action-react-0.0.3/README.md` & `action-react-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `action-react-0.0.3/action_react/main.py` & `action-react-0.0.4/action_react/main.py`

 * *Files identical despite different names*

### Comparing `action-react-0.0.3/action_react/react.py` & `action-react-0.0.4/action_react/react.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,22 +15,44 @@
 SLEEP = 0.15
 
 chrome_options = Options()
 chrome_options.add_experimental_option("detach", True)
 
 
 def process_with_city_and_date(reaction, object, city, date):
+    """
+    Process string object with city and/or date
+
+    Parameters
+    ----------
+    reaction: json object, reaction
+    object: str, string to be updated
+    city: str, target city
+    date: date, target date
+
+    Returns
+    -------
+    object: updated object
+    """
     if "replace_city" in reaction and reaction["replace_city"] is True:
         object.replace("city", city)
     if "replace_date" in reaction and reaction["replace_date"] is True:
         object.replace("date", datetime.strptime(date, reaction["date_format"]))
     return object
 
 
 def react(date, city):
+    """
+    React
+
+    Parameters
+    ----------
+    city: str, target city
+    date: date, target date
+    """
     c_service = Service("/usr/bin/chromedriver")
     c_service.command_line_args()
     c_service.start()
     driver = webdriver.Chrome(chrome_options=chrome_options)
     with open(REACTIONS_FILE) as f:
         reactions = json.load(f)
         for reaction in reactions:
```

### Comparing `action-react-0.0.3/action_react/tests/test_all.py` & `action-react-0.0.4/action_react/tests/test_all.py`

 * *Files identical despite different names*

### Comparing `action-react-0.0.3/action_react.egg-info/PKG-INFO` & `action-react-0.0.4/action_react.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: action-react
-Version: 0.0.3
+Version: 0.0.4
 Summary: telegram listener tool
 Author-email: yd-wu <yw3960@columbia.edu>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `action-react-0.0.3/action_react.egg-info/SOURCES.txt` & `action-react-0.0.4/action_react.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `action-react-0.0.3/docs/Makefile` & `action-react-0.0.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `action-react-0.0.3/docs/conf.py` & `action-react-0.0.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `action-react-0.0.3/docs/index.md` & `action-react-0.0.4/docs/index.md`

 * *Files identical despite different names*

### Comparing `action-react-0.0.3/docs/make.bat` & `action-react-0.0.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `action-react-0.0.3/pyproject.toml` & `action-react-0.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 build-backend="setuptools.build_meta"
 
 [project]
 name = "action-react"
 authors = [{name = "yd-wu", email = "yw3960@columbia.edu"}]
 description="telegram listener tool"
 readme = "README.md"
-version = "0.0.3"
+version = "0.0.4"
 requires-python = ">=3.7"
 
 dynamic = ["dependencies"]
 
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "Programming Language :: Python :: Implementation :: CPython",
```

