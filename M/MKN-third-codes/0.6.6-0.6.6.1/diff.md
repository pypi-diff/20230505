# Comparing `tmp/MKN_third_codes-0.6.6.tar.gz` & `tmp/MKN_third_codes-0.6.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\MKN_third_codes-0.6.6.tar", last modified: Fri May  5 04:09:39 2023, max compression
+gzip compressed data, was "dist\MKN_third_codes-0.6.6.1.tar", last modified: Fri May  5 04:16:15 2023, max compression
```

## Comparing `MKN_third_codes-0.6.6.tar` & `MKN_third_codes-0.6.6.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 04:09:39.682726 MKN_third_codes-0.6.6/
--rw-rw-rw-   0        0        0     1073 2023-04-29 11:32:30.000000 MKN_third_codes-0.6.6/LICENSE.txt
--rw-rw-rw-   0        0        0       25 2023-04-29 11:33:13.000000 MKN_third_codes-0.6.6/MANIFEST.in
-drwxrwxrwx   0        0        0        0 2023-05-05 04:09:39.638843 MKN_third_codes-0.6.6/MKN_third_codes.egg-info/
--rw-rw-rw-   0        0        0     8108 2023-05-05 04:09:39.000000 MKN_third_codes-0.6.6/MKN_third_codes.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      271 2023-05-05 04:09:39.000000 MKN_third_codes-0.6.6/MKN_third_codes.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 04:09:39.000000 MKN_third_codes-0.6.6/MKN_third_codes.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-05-05 04:09:39.000000 MKN_third_codes-0.6.6/MKN_third_codes.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     8108 2023-05-05 04:09:39.681728 MKN_third_codes-0.6.6/PKG-INFO
--rw-rw-rw-   0        0        0     4375 2023-05-05 04:07:43.000000 MKN_third_codes-0.6.6/README.md
-drwxrwxrwx   0        0        0        0 2023-05-05 04:09:39.679734 MKN_third_codes-0.6.6/mfcn/
--rw-rw-rw-   0        0        0        0 2023-05-03 09:46:59.000000 MKN_third_codes-0.6.6/mfcn/__init__.py
--rw-rw-rw-   0        0        0     1389 2023-05-05 04:09:34.000000 MKN_third_codes-0.6.6/mfcn/mkn_globals.py
--rw-rw-rw-   0        0        0     9638 2023-05-03 12:36:38.000000 MKN_third_codes-0.6.6/mfcn/mkn_utils.py
--rw-rw-rw-   0        0        0    27955 2023-05-05 04:07:02.000000 MKN_third_codes-0.6.6/mfcn/solutions.py
--rw-rw-rw-   0        0        0       42 2023-05-05 04:09:39.682726 MKN_third_codes-0.6.6/setup.cfg
--rw-rw-rw-   0        0        0      476 2023-05-05 04:05:26.000000 MKN_third_codes-0.6.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-05 04:16:15.622308 MKN_third_codes-0.6.6.1/
+-rw-rw-rw-   0        0        0     1073 2023-04-29 11:32:30.000000 MKN_third_codes-0.6.6.1/LICENSE.txt
+-rw-rw-rw-   0        0        0       25 2023-04-29 11:33:13.000000 MKN_third_codes-0.6.6.1/MANIFEST.in
+drwxrwxrwx   0        0        0        0 2023-05-05 04:16:15.617321 MKN_third_codes-0.6.6.1/MKN_third_codes.egg-info/
+-rw-rw-rw-   0        0        0     8110 2023-05-05 04:16:15.000000 MKN_third_codes-0.6.6.1/MKN_third_codes.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      271 2023-05-05 04:16:15.000000 MKN_third_codes-0.6.6.1/MKN_third_codes.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 04:16:15.000000 MKN_third_codes-0.6.6.1/MKN_third_codes.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-05-05 04:16:15.000000 MKN_third_codes-0.6.6.1/MKN_third_codes.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     8110 2023-05-05 04:16:15.622308 MKN_third_codes-0.6.6.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4375 2023-05-05 04:07:43.000000 MKN_third_codes-0.6.6.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-05 04:16:15.620313 MKN_third_codes-0.6.6.1/mfcn/
+-rw-rw-rw-   0        0        0        0 2023-05-03 09:46:59.000000 MKN_third_codes-0.6.6.1/mfcn/__init__.py
+-rw-rw-rw-   0        0        0     1389 2023-05-05 04:09:34.000000 MKN_third_codes-0.6.6.1/mfcn/mkn_globals.py
+-rw-rw-rw-   0        0        0     9638 2023-05-03 12:36:38.000000 MKN_third_codes-0.6.6.1/mfcn/mkn_utils.py
+-rw-rw-rw-   0        0        0    27849 2023-05-05 04:16:03.000000 MKN_third_codes-0.6.6.1/mfcn/solutions.py
+-rw-rw-rw-   0        0        0       42 2023-05-05 04:16:15.622308 MKN_third_codes-0.6.6.1/setup.cfg
+-rw-rw-rw-   0        0        0      478 2023-05-05 04:16:10.000000 MKN_third_codes-0.6.6.1/setup.py
```

### Comparing `MKN_third_codes-0.6.6/LICENSE.txt` & `MKN_third_codes-0.6.6.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `MKN_third_codes-0.6.6/MKN_third_codes.egg-info/PKG-INFO` & `MKN_third_codes-0.6.6.1/MKN_third_codes.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MKN-third-codes
-Version: 0.6.6
+Version: 0.6.6.1
 Summary: Python library with standart solutions for probability tasks
 Author: Dolgun Ivan
 Author-email: vanadolgun@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `MKN_third_codes-0.6.6/PKG-INFO` & `MKN_third_codes-0.6.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MKN_third_codes
-Version: 0.6.6
+Version: 0.6.6.1
 Summary: Python library with standart solutions for probability tasks
 Author: Dolgun Ivan
 Author-email: vanadolgun@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `MKN_third_codes-0.6.6/README.md` & `MKN_third_codes-0.6.6.1/README.md`

 * *Files identical despite different names*

### Comparing `MKN_third_codes-0.6.6/mfcn/mkn_globals.py` & `MKN_third_codes-0.6.6.1/mfcn/mkn_globals.py`

 * *Files identical despite different names*

### Comparing `MKN_third_codes-0.6.6/mfcn/mkn_utils.py` & `MKN_third_codes-0.6.6.1/mfcn/mkn_utils.py`

 * *Files identical despite different names*

### Comparing `MKN_third_codes-0.6.6/mfcn/solutions.py` & `MKN_third_codes-0.6.6.1/mfcn/solutions.py`

 * *Files 0% similar despite different names*

```diff
@@ -523,21 +523,19 @@
     """
     if text == None:
         return ["""Введите количество значений таблицы (число n)
 В следующих n строчках введите пары чисел: значение СВ, вероятность (любой разделитель, кроме  '.', ',', '/')"""]
     else:
         try:
             request = glb.to_float_values(re.findall(glb.regular_float, text))
-            print(request)
             n = int(request[0])
             table = utl.EttaTable()
 
             for i in range(0, n):
                 table.cells.append(utl.EttaTableCell(etta_value=request[1+i*2], probability=max(request[2+i*2],0)))
-                print(table.cells[i].probability, table.cells[i].etta_value)
 
             answer = []
             result = table_analysis_solution(table)
             
             if "ошибка" not in result[0].lower() and "ошибка" not in result[1].lower():
                 answer.append(f"Mx = ⁱ⁼¹∑ⁿ(xi * pi) = {result[0]}")
                 answer.append(f"Dx = ⁱ⁼¹∑ⁿ( (xi - M(X))² pi ) = {result[1]}")
```

