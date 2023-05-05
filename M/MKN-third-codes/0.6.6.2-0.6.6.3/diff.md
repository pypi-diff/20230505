# Comparing `tmp/MKN_third_codes-0.6.6.2.tar.gz` & `tmp/MKN_third_codes-0.6.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\MKN_third_codes-0.6.6.2.tar", last modified: Fri May  5 04:22:18 2023, max compression
+gzip compressed data, was "dist\MKN_third_codes-0.6.6.3.tar", last modified: Fri May  5 04:24:00 2023, max compression
```

## Comparing `MKN_third_codes-0.6.6.2.tar` & `MKN_third_codes-0.6.6.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 04:22:18.935904 MKN_third_codes-0.6.6.2/
--rw-rw-rw-   0        0        0     1073 2023-04-29 11:32:30.000000 MKN_third_codes-0.6.6.2/LICENSE.txt
--rw-rw-rw-   0        0        0       25 2023-04-29 11:33:13.000000 MKN_third_codes-0.6.6.2/MANIFEST.in
-drwxrwxrwx   0        0        0        0 2023-05-05 04:22:18.930918 MKN_third_codes-0.6.6.2/MKN_third_codes.egg-info/
--rw-rw-rw-   0        0        0     8110 2023-05-05 04:22:18.000000 MKN_third_codes-0.6.6.2/MKN_third_codes.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      271 2023-05-05 04:22:18.000000 MKN_third_codes-0.6.6.2/MKN_third_codes.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 04:22:18.000000 MKN_third_codes-0.6.6.2/MKN_third_codes.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-05-05 04:22:18.000000 MKN_third_codes-0.6.6.2/MKN_third_codes.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     8110 2023-05-05 04:22:18.935904 MKN_third_codes-0.6.6.2/PKG-INFO
--rw-rw-rw-   0        0        0     4375 2023-05-05 04:07:43.000000 MKN_third_codes-0.6.6.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-05 04:22:18.933910 MKN_third_codes-0.6.6.2/mfcn/
--rw-rw-rw-   0        0        0        0 2023-05-03 09:46:59.000000 MKN_third_codes-0.6.6.2/mfcn/__init__.py
--rw-rw-rw-   0        0        0     1389 2023-05-05 04:09:34.000000 MKN_third_codes-0.6.6.2/mfcn/mkn_globals.py
--rw-rw-rw-   0        0        0     9638 2023-05-03 12:36:38.000000 MKN_third_codes-0.6.6.2/mfcn/mkn_utils.py
--rw-rw-rw-   0        0        0    28001 2023-05-05 04:22:10.000000 MKN_third_codes-0.6.6.2/mfcn/solutions.py
--rw-rw-rw-   0        0        0       42 2023-05-05 04:22:18.935904 MKN_third_codes-0.6.6.2/setup.cfg
--rw-rw-rw-   0        0        0      478 2023-05-05 04:22:15.000000 MKN_third_codes-0.6.6.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-05 04:24:00.627223 MKN_third_codes-0.6.6.3/
+-rw-rw-rw-   0        0        0     1073 2023-04-29 11:32:30.000000 MKN_third_codes-0.6.6.3/LICENSE.txt
+-rw-rw-rw-   0        0        0       25 2023-04-29 11:33:13.000000 MKN_third_codes-0.6.6.3/MANIFEST.in
+drwxrwxrwx   0        0        0        0 2023-05-05 04:24:00.622221 MKN_third_codes-0.6.6.3/MKN_third_codes.egg-info/
+-rw-rw-rw-   0        0        0     8110 2023-05-05 04:24:00.000000 MKN_third_codes-0.6.6.3/MKN_third_codes.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      271 2023-05-05 04:24:00.000000 MKN_third_codes-0.6.6.3/MKN_third_codes.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 04:24:00.000000 MKN_third_codes-0.6.6.3/MKN_third_codes.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-05-05 04:24:00.000000 MKN_third_codes-0.6.6.3/MKN_third_codes.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     8110 2023-05-05 04:24:00.626227 MKN_third_codes-0.6.6.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4375 2023-05-05 04:07:43.000000 MKN_third_codes-0.6.6.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-05 04:24:00.625180 MKN_third_codes-0.6.6.3/mfcn/
+-rw-rw-rw-   0        0        0        0 2023-05-03 09:46:59.000000 MKN_third_codes-0.6.6.3/mfcn/__init__.py
+-rw-rw-rw-   0        0        0     1389 2023-05-05 04:09:34.000000 MKN_third_codes-0.6.6.3/mfcn/mkn_globals.py
+-rw-rw-rw-   0        0        0     9638 2023-05-03 12:36:38.000000 MKN_third_codes-0.6.6.3/mfcn/mkn_utils.py
+-rw-rw-rw-   0        0        0    28001 2023-05-05 04:22:10.000000 MKN_third_codes-0.6.6.3/mfcn/solutions.py
+-rw-rw-rw-   0        0        0       42 2023-05-05 04:24:00.627223 MKN_third_codes-0.6.6.3/setup.cfg
+-rw-rw-rw-   0        0        0      478 2023-05-05 04:23:51.000000 MKN_third_codes-0.6.6.3/setup.py
```

### Comparing `MKN_third_codes-0.6.6.2/LICENSE.txt` & `MKN_third_codes-0.6.6.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `MKN_third_codes-0.6.6.2/MKN_third_codes.egg-info/PKG-INFO` & `MKN_third_codes-0.6.6.3/MKN_third_codes.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MKN-third-codes
-Version: 0.6.6.2
+Version: 0.6.6.3
 Summary: Python library with standart solutions for probability tasks
 Author: Dolgun Ivan
 Author-email: vanadolgun@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
@@ -57,15 +57,15 @@
 [libaPage]: https://pypi.org/project/MKN-third-codes/
 [AlekseiBot]: https://t.me/mkn_solver_bot
 [LehaVK]: https://vk.com/miranchuk5959
 #
 ## Change Log
 ====================
 
-## 0.6.6 (03/05/2023)
+## 0.6.6 (05/05/2023)
 ```
 ------------------
 ┏ to_float_values функция
 ┗ починил принятие float для request функций
 ------------------
 ```
 ## 0.6.5.4 (03/05/2023)
```

### Comparing `MKN_third_codes-0.6.6.2/PKG-INFO` & `MKN_third_codes-0.6.6.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MKN_third_codes
-Version: 0.6.6.2
+Version: 0.6.6.3
 Summary: Python library with standart solutions for probability tasks
 Author: Dolgun Ivan
 Author-email: vanadolgun@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
@@ -57,15 +57,15 @@
 [libaPage]: https://pypi.org/project/MKN-third-codes/
 [AlekseiBot]: https://t.me/mkn_solver_bot
 [LehaVK]: https://vk.com/miranchuk5959
 #
 ## Change Log
 ====================
 
-## 0.6.6 (03/05/2023)
+## 0.6.6 (05/05/2023)
 ```
 ------------------
 ┏ to_float_values функция
 ┗ починил принятие float для request функций
 ------------------
 ```
 ## 0.6.5.4 (03/05/2023)
```

### Comparing `MKN_third_codes-0.6.6.2/README.md` & `MKN_third_codes-0.6.6.3/README.md`

 * *Files identical despite different names*

### Comparing `MKN_third_codes-0.6.6.2/mfcn/mkn_globals.py` & `MKN_third_codes-0.6.6.3/mfcn/mkn_globals.py`

 * *Files identical despite different names*

### Comparing `MKN_third_codes-0.6.6.2/mfcn/mkn_utils.py` & `MKN_third_codes-0.6.6.3/mfcn/mkn_utils.py`

 * *Files identical despite different names*

### Comparing `MKN_third_codes-0.6.6.2/mfcn/solutions.py` & `MKN_third_codes-0.6.6.3/mfcn/solutions.py`

 * *Files identical despite different names*

