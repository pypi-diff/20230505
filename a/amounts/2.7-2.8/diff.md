# Comparing `tmp/amounts-2.7.tar.gz` & `tmp/amounts-2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amounts-2.7.tar", last modified: Fri May  5 17:02:07 2023, max compression
+gzip compressed data, was "amounts-2.8.tar", last modified: Fri May  5 17:07:00 2023, max compression
```

## Comparing `amounts-2.7.tar` & `amounts-2.8.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 17:02:07.566287 amounts-2.7/
--rwxrwx---   0 root         (0) root         (0)     1090 2023-04-28 13:47:58.000000 amounts-2.7/LICENSE
--rwxrwx---   0 root         (0) root         (0)       29 2023-05-05 16:34:14.000000 amounts-2.7/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     6086 2023-05-05 17:02:07.566287 amounts-2.7/PKG-INFO
--rwxrwx---   0 root         (0) root         (0)     5842 2023-05-05 17:01:40.000000 amounts-2.7/README.md
--rwxrwx---   0 root         (0) root         (0)      713 2023-05-05 17:01:57.000000 amounts-2.7/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-05 17:02:07.566287 amounts-2.7/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 17:02:07.562285 amounts-2.7/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 17:02:07.566287 amounts-2.7/src/amounts/
--rwxrwx---   0 root         (0) root         (0)        0 2023-04-28 13:13:40.000000 amounts-2.7/src/amounts/__init__.py
--rwxrwx---   0 root         (0) root         (0)    13830 2023-05-05 16:04:56.000000 amounts-2.7/src/amounts/amounts.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 17:02:07.566287 amounts-2.7/src/amounts.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6086 2023-05-05 17:02:07.000000 amounts-2.7/src/amounts.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      535 2023-05-05 17:02:07.000000 amounts-2.7/src/amounts.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-05 17:02:07.000000 amounts-2.7/src/amounts.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       49 2023-05-05 17:02:07.000000 amounts-2.7/src/amounts.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-05-05 17:02:07.000000 amounts-2.7/src/amounts.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 17:02:07.566287 amounts-2.7/src/wordlists/
--rwxrwx---   0 root         (0) root         (0)     5487 2023-04-28 13:47:58.000000 amounts-2.7/src/wordlists/all.txt
--rwxrwx---   0 root         (0) root         (0)     2202 2023-04-28 13:47:58.000000 amounts-2.7/src/wordlists/hundred.txt
--rwxrwx---   0 root         (0) root         (0)     2407 2023-04-28 13:47:58.000000 amounts-2.7/src/wordlists/hundred_thousand.txt
--rwxrwx---   0 root         (0) root         (0)     2471 2023-04-28 13:47:58.000000 amounts-2.7/src/wordlists/milion.txt
--rwxrwx---   0 root         (0) root         (0)     2069 2023-04-28 13:47:58.000000 amounts-2.7/src/wordlists/one.txt
--rwxrwx---   0 root         (0) root         (0)     2143 2023-04-28 13:47:58.000000 amounts-2.7/src/wordlists/ten.txt
--rwxrwx---   0 root         (0) root         (0)     2345 2023-04-28 13:47:58.000000 amounts-2.7/src/wordlists/ten_thousand.txt
--rwxrwx---   0 root         (0) root         (0)     2282 2023-04-28 13:47:58.000000 amounts-2.7/src/wordlists/thousand.txt
--rwxrwx---   0 root         (0) root         (0)     2055 2023-04-28 13:47:58.000000 amounts-2.7/src/wordlists/zero.txt
--rwxrwx---   0 root         (0) root         (0)     2225 2023-04-28 13:47:58.000000 amounts-2.7/src/wordlists/zero_point_one.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 17:07:00.360602 amounts-2.8/
+-rwxrwx---   0 root         (0) root         (0)     1090 2023-04-28 13:47:58.000000 amounts-2.8/LICENSE
+-rwxrwx---   0 root         (0) root         (0)       29 2023-05-05 16:34:14.000000 amounts-2.8/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     6098 2023-05-05 17:07:00.360602 amounts-2.8/PKG-INFO
+-rwxrwx---   0 root         (0) root         (0)     5854 2023-05-05 17:06:17.000000 amounts-2.8/README.md
+-rwxrwx---   0 root         (0) root         (0)      713 2023-05-05 17:06:54.000000 amounts-2.8/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-05 17:07:00.360602 amounts-2.8/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 17:07:00.356600 amounts-2.8/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 17:07:00.356600 amounts-2.8/src/amounts/
+-rwxrwx---   0 root         (0) root         (0)        0 2023-04-28 13:13:40.000000 amounts-2.8/src/amounts/__init__.py
+-rwxrwx---   0 root         (0) root         (0)    13830 2023-05-05 17:06:31.000000 amounts-2.8/src/amounts/amounts.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 17:07:00.360602 amounts-2.8/src/amounts.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6098 2023-05-05 17:07:00.000000 amounts-2.8/src/amounts.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      535 2023-05-05 17:07:00.000000 amounts-2.8/src/amounts.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-05 17:07:00.000000 amounts-2.8/src/amounts.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       49 2023-05-05 17:07:00.000000 amounts-2.8/src/amounts.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-05-05 17:07:00.000000 amounts-2.8/src/amounts.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 17:07:00.360602 amounts-2.8/src/wordlists/
+-rwxrwx---   0 root         (0) root         (0)     5487 2023-04-28 13:47:58.000000 amounts-2.8/src/wordlists/all.txt
+-rwxrwx---   0 root         (0) root         (0)     2202 2023-04-28 13:47:58.000000 amounts-2.8/src/wordlists/hundred.txt
+-rwxrwx---   0 root         (0) root         (0)     2407 2023-04-28 13:47:58.000000 amounts-2.8/src/wordlists/hundred_thousand.txt
+-rwxrwx---   0 root         (0) root         (0)     2471 2023-04-28 13:47:58.000000 amounts-2.8/src/wordlists/milion.txt
+-rwxrwx---   0 root         (0) root         (0)     2069 2023-04-28 13:47:58.000000 amounts-2.8/src/wordlists/one.txt
+-rwxrwx---   0 root         (0) root         (0)     2143 2023-04-28 13:47:58.000000 amounts-2.8/src/wordlists/ten.txt
+-rwxrwx---   0 root         (0) root         (0)     2345 2023-04-28 13:47:58.000000 amounts-2.8/src/wordlists/ten_thousand.txt
+-rwxrwx---   0 root         (0) root         (0)     2282 2023-04-28 13:47:58.000000 amounts-2.8/src/wordlists/thousand.txt
+-rwxrwx---   0 root         (0) root         (0)     2055 2023-04-28 13:47:58.000000 amounts-2.8/src/wordlists/zero.txt
+-rwxrwx---   0 root         (0) root         (0)     2225 2023-04-28 13:47:58.000000 amounts-2.8/src/wordlists/zero_point_one.txt
```

### Comparing `amounts-2.7/LICENSE` & `amounts-2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `amounts-2.7/PKG-INFO` & `amounts-2.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amounts
-Version: 2.7
+Version: 2.8
 Summary: Generate a wordlist to fuzz amounts or any other numerical values.
 Author: Ivan Sincek
 Project-URL: Homepage, https://github.com/ivan-sincek/amounts
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
@@ -65,24 +65,24 @@
 ```fundamental
 git clone https://github.com/ivan-sincek/amounts && cd amounts
 
 python3 -m pip install --upgrade build
 
 python3 -m build
 
-python3 -m pip install dist/amounts-2.7-py3-none-any.whl
+python3 -m pip install dist/amounts-2.8-py3-none-any.whl
 ```
 
 ## Generated Amounts
 
 ```fundamental
 amounts -min 1 -max 10000 -mid 2200 -o amounts.txt
 ```
 
-`amounts.txt` output:
+`amounts.txt` generated wordlist:
 
 ```fundamental
 1
 10000
 2200
 2 200
 2.200
@@ -168,15 +168,15 @@
 -999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999
 -99999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999
 ```
 
 ## Usage
 
 ```fundamental
-Amounts v2.7 ( github.com/ivan-sincek/amounts )
+Amounts v2.8 ( github.com/ivan-sincek/amounts )
 
 --- Generate a wordlist for a range of amounts ---
 Usage:   python3 amounts.py -min minimum -max maximum -mid middle -o out         [-q quotes]
 Example: python3 amounts.py -min 1       -max 1000    -mid 20     -o amounts.txt [-q double]
 
 --- Generate a wordlist for a single amount ---
 Usage:   python3 amounts.py -a amount -o out         [-q quotes]
```

### Comparing `amounts-2.7/README.md` & `amounts-2.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -52,24 +52,24 @@
 ```fundamental
 git clone https://github.com/ivan-sincek/amounts && cd amounts
 
 python3 -m pip install --upgrade build
 
 python3 -m build
 
-python3 -m pip install dist/amounts-2.7-py3-none-any.whl
+python3 -m pip install dist/amounts-2.8-py3-none-any.whl
 ```
 
 ## Generated Amounts
 
 ```fundamental
 amounts -min 1 -max 10000 -mid 2200 -o amounts.txt
 ```
 
-`amounts.txt` output:
+`amounts.txt` generated wordlist:
 
 ```fundamental
 1
 10000
 2200
 2 200
 2.200
@@ -155,15 +155,15 @@
 -999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999
 -99999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999
 ```
 
 ## Usage
 
 ```fundamental
-Amounts v2.7 ( github.com/ivan-sincek/amounts )
+Amounts v2.8 ( github.com/ivan-sincek/amounts )
 
 --- Generate a wordlist for a range of amounts ---
 Usage:   python3 amounts.py -min minimum -max maximum -mid middle -o out         [-q quotes]
 Example: python3 amounts.py -min 1       -max 1000    -mid 20     -o amounts.txt [-q double]
 
 --- Generate a wordlist for a single amount ---
 Usage:   python3 amounts.py -a amount -o out         [-q quotes]
```

### Comparing `amounts-2.7/pyproject.toml` & `amounts-2.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "amounts"
-version = "2.7"
+version = "2.8"
 authors = [{ name = "Ivan Sincek" }]
 description = "Generate a wordlist to fuzz amounts or any other numerical values."
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
 	"Programming Language :: Python :: 3",
 	"License :: OSI Approved :: MIT License",
```

### Comparing `amounts-2.7/src/amounts/amounts.py` & `amounts-2.8/src/amounts/amounts.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import struct
 
 # -------------------------- INFO --------------------------
 
 def basic():
 	global proceed
 	proceed = False
-	print("Amounts v2.7 ( github.com/ivan-sincek/amounts )")
+	print("Amounts v2.8 ( github.com/ivan-sincek/amounts )")
 	print("")
 	print("--- Generate a wordlist for a range of amounts ---")
 	print("Usage:   python3 amounts.py -min minimum -max maximum -mid middle -o out         [-q quotes]")
 	print("Example: python3 amounts.py -min 1       -max 1000    -mid 20     -o amounts.txt [-q double]")
 	print("")
 	print("--- Generate a wordlist for a single amount ---")
 	print("Usage:   python3 amounts.py -a amount -o out         [-q quotes]")
@@ -416,15 +416,15 @@
 			error("Missing a mandatory option (-a, -o) and/or optional (-q)", True)
 	else:
 		error("Incorrect usage", True)
 
 	if proceed:
 	print("##########################################################################")
 	print("#                                                                        #")
-	print("#                              Amounts v2.7                              #")
+	print("#                              Amounts v2.8                              #")
 	print("#                                 by Ivan Sincek                         #")
 	print("#                                                                        #")
 	print("# Generate a wordlist to fuzz amounts or any other numerical values.     #")
 	print("# GitHub repository at github.com/ivan-sincek/amounts.                   #")
 	print("# Feel free to donate ETH at 0xbc00e800f29524AD8b0968CEBEAD4cD5C5c1f105. #")
 	print("#                                                                        #")
 	print("##########################################################################")
```

### Comparing `amounts-2.7/src/amounts.egg-info/PKG-INFO` & `amounts-2.8/src/amounts.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amounts
-Version: 2.7
+Version: 2.8
 Summary: Generate a wordlist to fuzz amounts or any other numerical values.
 Author: Ivan Sincek
 Project-URL: Homepage, https://github.com/ivan-sincek/amounts
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
@@ -65,24 +65,24 @@
 ```fundamental
 git clone https://github.com/ivan-sincek/amounts && cd amounts
 
 python3 -m pip install --upgrade build
 
 python3 -m build
 
-python3 -m pip install dist/amounts-2.7-py3-none-any.whl
+python3 -m pip install dist/amounts-2.8-py3-none-any.whl
 ```
 
 ## Generated Amounts
 
 ```fundamental
 amounts -min 1 -max 10000 -mid 2200 -o amounts.txt
 ```
 
-`amounts.txt` output:
+`amounts.txt` generated wordlist:
 
 ```fundamental
 1
 10000
 2200
 2 200
 2.200
@@ -168,15 +168,15 @@
 -999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999
 -99999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999
 ```
 
 ## Usage
 
 ```fundamental
-Amounts v2.7 ( github.com/ivan-sincek/amounts )
+Amounts v2.8 ( github.com/ivan-sincek/amounts )
 
 --- Generate a wordlist for a range of amounts ---
 Usage:   python3 amounts.py -min minimum -max maximum -mid middle -o out         [-q quotes]
 Example: python3 amounts.py -min 1       -max 1000    -mid 20     -o amounts.txt [-q double]
 
 --- Generate a wordlist for a single amount ---
 Usage:   python3 amounts.py -a amount -o out         [-q quotes]
```

### Comparing `amounts-2.7/src/amounts.egg-info/SOURCES.txt` & `amounts-2.8/src/amounts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `amounts-2.7/src/wordlists/all.txt` & `amounts-2.8/src/wordlists/all.txt`

 * *Files identical despite different names*

### Comparing `amounts-2.7/src/wordlists/hundred.txt` & `amounts-2.8/src/wordlists/hundred.txt`

 * *Files identical despite different names*

### Comparing `amounts-2.7/src/wordlists/hundred_thousand.txt` & `amounts-2.8/src/wordlists/hundred_thousand.txt`

 * *Files identical despite different names*

### Comparing `amounts-2.7/src/wordlists/milion.txt` & `amounts-2.8/src/wordlists/milion.txt`

 * *Files identical despite different names*

### Comparing `amounts-2.7/src/wordlists/one.txt` & `amounts-2.8/src/wordlists/one.txt`

 * *Files identical despite different names*

### Comparing `amounts-2.7/src/wordlists/ten.txt` & `amounts-2.8/src/wordlists/ten.txt`

 * *Files identical despite different names*

### Comparing `amounts-2.7/src/wordlists/ten_thousand.txt` & `amounts-2.8/src/wordlists/ten_thousand.txt`

 * *Files identical despite different names*

### Comparing `amounts-2.7/src/wordlists/thousand.txt` & `amounts-2.8/src/wordlists/thousand.txt`

 * *Files identical despite different names*

### Comparing `amounts-2.7/src/wordlists/zero.txt` & `amounts-2.8/src/wordlists/zero.txt`

 * *Files identical despite different names*

### Comparing `amounts-2.7/src/wordlists/zero_point_one.txt` & `amounts-2.8/src/wordlists/zero_point_one.txt`

 * *Files identical despite different names*

