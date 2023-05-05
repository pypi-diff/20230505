# Comparing `tmp/MKN_third_codes-0.6.5.4.tar.gz` & `tmp/MKN_third_codes-0.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\MKN_third_codes-0.6.5.4.tar", last modified: Wed May  3 12:37:40 2023, max compression
+gzip compressed data, was "dist\MKN_third_codes-0.6.6.tar", last modified: Fri May  5 04:09:39 2023, max compression
```

## Comparing `MKN_third_codes-0.6.5.4.tar` & `MKN_third_codes-0.6.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 12:37:40.293656 MKN_third_codes-0.6.5.4/
--rw-rw-rw-   0        0        0     1073 2023-04-29 11:32:30.000000 MKN_third_codes-0.6.5.4/LICENSE.txt
--rw-rw-rw-   0        0        0       25 2023-04-29 11:33:13.000000 MKN_third_codes-0.6.5.4/MANIFEST.in
-drwxrwxrwx   0        0        0        0 2023-05-03 12:37:40.287670 MKN_third_codes-0.6.5.4/MKN_third_codes.egg-info/
--rw-rw-rw-   0        0        0     7818 2023-05-03 12:37:40.000000 MKN_third_codes-0.6.5.4/MKN_third_codes.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      271 2023-05-03 12:37:40.000000 MKN_third_codes-0.6.5.4/MKN_third_codes.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 12:37:40.000000 MKN_third_codes-0.6.5.4/MKN_third_codes.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-05-03 12:37:40.000000 MKN_third_codes-0.6.5.4/MKN_third_codes.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     7818 2023-05-03 12:37:40.292657 MKN_third_codes-0.6.5.4/PKG-INFO
--rw-rw-rw-   0        0        0     4265 2023-05-03 12:37:33.000000 MKN_third_codes-0.6.5.4/README.md
-drwxrwxrwx   0        0        0        0 2023-05-03 12:37:40.291660 MKN_third_codes-0.6.5.4/mfcn/
--rw-rw-rw-   0        0        0        0 2023-05-03 09:46:59.000000 MKN_third_codes-0.6.5.4/mfcn/__init__.py
--rw-rw-rw-   0        0        0      683 2023-05-03 07:35:48.000000 MKN_third_codes-0.6.5.4/mfcn/mkn_globals.py
--rw-rw-rw-   0        0        0     9638 2023-05-03 12:36:38.000000 MKN_third_codes-0.6.5.4/mfcn/mkn_utils.py
--rw-rw-rw-   0        0        0    27897 2023-05-03 12:36:23.000000 MKN_third_codes-0.6.5.4/mfcn/solutions.py
--rw-rw-rw-   0        0        0       42 2023-05-03 12:37:40.293656 MKN_third_codes-0.6.5.4/setup.cfg
--rw-rw-rw-   0        0        0      478 2023-05-03 12:36:48.000000 MKN_third_codes-0.6.5.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-05 04:09:39.682726 MKN_third_codes-0.6.6/
+-rw-rw-rw-   0        0        0     1073 2023-04-29 11:32:30.000000 MKN_third_codes-0.6.6/LICENSE.txt
+-rw-rw-rw-   0        0        0       25 2023-04-29 11:33:13.000000 MKN_third_codes-0.6.6/MANIFEST.in
+drwxrwxrwx   0        0        0        0 2023-05-05 04:09:39.638843 MKN_third_codes-0.6.6/MKN_third_codes.egg-info/
+-rw-rw-rw-   0        0        0     8108 2023-05-05 04:09:39.000000 MKN_third_codes-0.6.6/MKN_third_codes.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      271 2023-05-05 04:09:39.000000 MKN_third_codes-0.6.6/MKN_third_codes.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 04:09:39.000000 MKN_third_codes-0.6.6/MKN_third_codes.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-05-05 04:09:39.000000 MKN_third_codes-0.6.6/MKN_third_codes.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     8108 2023-05-05 04:09:39.681728 MKN_third_codes-0.6.6/PKG-INFO
+-rw-rw-rw-   0        0        0     4375 2023-05-05 04:07:43.000000 MKN_third_codes-0.6.6/README.md
+drwxrwxrwx   0        0        0        0 2023-05-05 04:09:39.679734 MKN_third_codes-0.6.6/mfcn/
+-rw-rw-rw-   0        0        0        0 2023-05-03 09:46:59.000000 MKN_third_codes-0.6.6/mfcn/__init__.py
+-rw-rw-rw-   0        0        0     1389 2023-05-05 04:09:34.000000 MKN_third_codes-0.6.6/mfcn/mkn_globals.py
+-rw-rw-rw-   0        0        0     9638 2023-05-03 12:36:38.000000 MKN_third_codes-0.6.6/mfcn/mkn_utils.py
+-rw-rw-rw-   0        0        0    27955 2023-05-05 04:07:02.000000 MKN_third_codes-0.6.6/mfcn/solutions.py
+-rw-rw-rw-   0        0        0       42 2023-05-05 04:09:39.682726 MKN_third_codes-0.6.6/setup.cfg
+-rw-rw-rw-   0        0        0      476 2023-05-05 04:05:26.000000 MKN_third_codes-0.6.6/setup.py
```

### Comparing `MKN_third_codes-0.6.5.4/LICENSE.txt` & `MKN_third_codes-0.6.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `MKN_third_codes-0.6.5.4/MKN_third_codes.egg-info/PKG-INFO` & `MKN_third_codes-0.6.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 Metadata-Version: 2.1
-Name: MKN-third-codes
-Version: 0.6.5.4
+Name: MKN_third_codes
+Version: 0.6.6
 Summary: Python library with standart solutions for probability tasks
 Author: Dolgun Ivan
 Author-email: vanadolgun@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 ### Здарова! Библиотека немного помогает с тервером по МКН 3
 
-# 📦 Версия: 0.6.5
+# 📦 Версия: 0.6.6
 
 - Функции `buckets_n_balls` => задачи про урны
 - Функции `things_complexity` => задачи про путаницу вещей
 - Функции `geometric_meeting` => задачи про встречи
 - Функции `find_math_prediction` => нахождение математического ожидания для таблицы СВ
 - Функции `find_disperion` => нахождение дисперсии для таблицы СВ
 - Функции `table_analysis` => нахождение МО и Дисперсии для таблицы СВ
 - Функция `combinations` => число сочетаний
+- Функция `to_float_values` => перевод найденных значений str(float) в float
 
 ### `подробно изменения расписаны в Change Log`
 
 # 🔩 Использование
 ## 📥 Импортирование
 ### `from mfcn import solutions`
 ## 📂 Структура
@@ -56,14 +57,21 @@
 [libaPage]: https://pypi.org/project/MKN-third-codes/
 [AlekseiBot]: https://t.me/mkn_solver_bot
 [LehaVK]: https://vk.com/miranchuk5959
 #
 ## Change Log
 ====================
 
+## 0.6.6 (03/05/2023)
+```
+------------------
+┏ to_float_values функция
+┗ починил принятие float для request функций
+------------------
+```
 ## 0.6.5.4 (03/05/2023)
 ```
 ------------------
 ━ вроде окончательно пофиксил import
 ------------------
 ```
 ## 0.6.5 (03/05/2023)
```

### Comparing `MKN_third_codes-0.6.5.4/PKG-INFO` & `MKN_third_codes-0.6.6/MKN_third_codes.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 Metadata-Version: 2.1
-Name: MKN_third_codes
-Version: 0.6.5.4
+Name: MKN-third-codes
+Version: 0.6.6
 Summary: Python library with standart solutions for probability tasks
 Author: Dolgun Ivan
 Author-email: vanadolgun@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 ### Здарова! Библиотека немного помогает с тервером по МКН 3
 
-# 📦 Версия: 0.6.5
+# 📦 Версия: 0.6.6
 
 - Функции `buckets_n_balls` => задачи про урны
 - Функции `things_complexity` => задачи про путаницу вещей
 - Функции `geometric_meeting` => задачи про встречи
 - Функции `find_math_prediction` => нахождение математического ожидания для таблицы СВ
 - Функции `find_disperion` => нахождение дисперсии для таблицы СВ
 - Функции `table_analysis` => нахождение МО и Дисперсии для таблицы СВ
 - Функция `combinations` => число сочетаний
+- Функция `to_float_values` => перевод найденных значений str(float) в float
 
 ### `подробно изменения расписаны в Change Log`
 
 # 🔩 Использование
 ## 📥 Импортирование
 ### `from mfcn import solutions`
 ## 📂 Структура
@@ -56,14 +57,21 @@
 [libaPage]: https://pypi.org/project/MKN-third-codes/
 [AlekseiBot]: https://t.me/mkn_solver_bot
 [LehaVK]: https://vk.com/miranchuk5959
 #
 ## Change Log
 ====================
 
+## 0.6.6 (03/05/2023)
+```
+------------------
+┏ to_float_values функция
+┗ починил принятие float для request функций
+------------------
+```
 ## 0.6.5.4 (03/05/2023)
 ```
 ------------------
 ━ вроде окончательно пофиксил import
 ------------------
 ```
 ## 0.6.5 (03/05/2023)
```

### Comparing `MKN_third_codes-0.6.5.4/README.md` & `MKN_third_codes-0.6.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 ### Здарова! Библиотека немного помогает с тервером по МКН 3
 
-# 📦 Версия: 0.6.5
+# 📦 Версия: 0.6.6
 
 - Функции `buckets_n_balls` => задачи про урны
 - Функции `things_complexity` => задачи про путаницу вещей
 - Функции `geometric_meeting` => задачи про встречи
 - Функции `find_math_prediction` => нахождение математического ожидания для таблицы СВ
 - Функции `find_disperion` => нахождение дисперсии для таблицы СВ
 - Функции `table_analysis` => нахождение МО и Дисперсии для таблицы СВ
 - Функция `combinations` => число сочетаний
+- Функция `to_float_values` => перевод найденных значений str(float) в float
 
 ### `подробно изменения расписаны в Change Log`
 
 # 🔩 Использование
 ## 📥 Импортирование
 ### `from mfcn import solutions`
 ## 📂 Структура
```

### Comparing `MKN_third_codes-0.6.5.4/mfcn/mkn_globals.py` & `MKN_third_codes-0.6.6/mfcn/mkn_globals.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import math
 
 regular_int = r'-?\d+'
-regular_float = r'-?\d+(?:[\.\,]\d+)?'
+regular_float = r'-?\d+(?:[\.\,\/]\d+)?'
 
 def combinations(k:float=0,n:float=0):
     """
     Функция, считающая число сочетаний из n по k
 
     Args:
         k (float): аргумент k - количество повторений
@@ -13,7 +13,28 @@
 
     Returns:
         float: результат применения формулы числа сочетаний
     """
     if k < 0 or n < 0:
         raise ValueError("ERROR: one or more argument's values are less than 0")
     return math.factorial(n)/(math.factorial(k)*math.factorial(n-k))
+
+def to_float_values(array: list):
+    """
+    Перевод каждой строки из входного массива в формат float
+
+    Args:
+        array (list(string)): массив строк, являющихся float-ами
+    
+    Returns:
+        list(float): массив float
+    """
+    for i in range(0, len(array)):
+        if "," in array[i]:
+            ind = array[i].index(",")
+            array[i] = float(array[i][:ind]+"."+array[i][ind+1:])
+        elif "/" in array[i]:
+            ind = array[i].index("/")
+            array[i] = int(array[i][:ind])/int(array[i][ind+1:])
+        else:
+            array[i] = float(array[i])
+    return array
```

### Comparing `MKN_third_codes-0.6.5.4/mfcn/mkn_utils.py` & `MKN_third_codes-0.6.6/mfcn/mkn_utils.py`

 * *Files identical despite different names*

### Comparing `MKN_third_codes-0.6.5.4/mfcn/solutions.py` & `MKN_third_codes-0.6.6/mfcn/solutions.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,15 +77,15 @@
         try:
             request = [int(parameter) for parameter in re.findall(glb.regular_int, text)]
 
             answer = []
 
             box_num = request[0]
 
-            boxes = [Box(request[1+2*i], request[2+2*i], request[1+box_num*2+i]) for i in range(box_num)]
+            boxes = [utl.Box(request[1+2*i], request[2+2*i], request[1+box_num*2+i]) for i in range(box_num)]
 
             result = buckets_n_balls_solution(boxes)
 
             answer.append("Обозначим событие A - достать Белый шар")
 
             txt = "P(B) = "
             for hypo in result[0]:
@@ -198,15 +198,15 @@
     Returns:
         list: массив строчек ответа
     """
     if text == None:
         return ["""Введите количество человек (число n)"""]
     else:
         try:
-            request = [int(parameter) for parameter in re.findall(regular_int, text)]
+            request = [int(parameter) for parameter in re.findall(glb.regular_int, text)]
             if len(request) == 1:
                 answer = []
 
                 humans_num = request[0]
 
                 result = things_complexity_solution(humans_num)
 
@@ -235,15 +235,15 @@
     Returns:
         list: массив строчек ответа
     """
     if text == None:
         return ["""Введите количество человек (число n)"""]
     else:
         try:
-            request = [int(parameter) for parameter in re.findall(regular_int, text)]
+            request = [int(parameter) for parameter in re.findall(glb.regular_int, text)]
             if len(request) == 1:
                 answer = []
 
                 humans_num = request[0]
                 if humans_num <= maximum_full:
                     result = things_complexity_solution(humans_num)
                 else:
@@ -264,19 +264,19 @@
             return ["""Возникла ошибка при обработке введённых данных. Проверьте правильность ввода."""]
 
 def geometric_meeting_terminal():
     """
     Общее решение задачи о встрече двух участников
     """
     ln = float(input("Введите отрезок меры: "))
-    fM = Meetiner(float(input("Введите начальный момент, когда может появиться участник первый (-1 для расширения на полный отрезок): ")), 
+    fM = utl.Meetiner(float(input("Введите начальный момент, когда может появиться участник первый (-1 для расширения на полный отрезок): ")), 
     float(input("Введите конечный момент, когда может появиться участник первый (-1 для расширения на полный отрезок): ")), 
     float(input("Введите, сколько времени будет ждать участник первый: ")))
 
-    sM = Meetiner(float(input("Введите начальный момент, когда может появиться участник второй (-1 для расширения на полный отрезок): ")), 
+    sM = utl.Meetiner(float(input("Введите начальный момент, когда может появиться участник второй (-1 для расширения на полный отрезок): ")), 
     float(input("Введите конечный момент, когда может появиться участник второй (-1 для расширения на полный отрезок): ")), 
     float(input("Введите, сколько времени будет ждать участник второй: ")))
 
     print("Обозначим за A - участники встретятся")
     print(f"P(A) = {geometric_meeting_solution(ln, fM, sM)}")
 
 def geometric_meeting_solution(length:float = 0, firstAim:utl.Meetiner=None, secondAim:utl.Meetiner=None):
@@ -311,21 +311,21 @@
         return ["""Введите отрезок меры
 Введите НАЧАЛЬНЫЙ и КОНЕЧНЫЙ моменты, когда может появиться участник ПЕРВЫЙ (-1 для расширения на полный отрезок)
 Введите, сколько времени будет ждать участник ПЕРВЫЙ
 Введите НАЧАЛЬНЫЙ и КОНЕЧНЫЙ моменты, когда может появиться участник ВТОРОЙ (-1 для расширения на полный отрезок)
 Введите, сколько времени будет ждать участник ВТОРОЙ"""]
     else:
         try:
-            request = [float(parameter) for parameter in re.findall(regular_float, text)]
+            request = [float(parameter) for parameter in re.findall(glb.regular_float, text)]
             if len(request) == 7:
                 answer = []
 
                 ln = request[0]
-                fM = Meetiner(request[1], request[2], request[3])
-                sM = Meetiner(request[4], request[5], request[6])
+                fM = utl.Meetiner(request[1], request[2], request[3])
+                sM = utl.Meetiner(request[4], request[5], request[6])
 
                 result = geometric_meeting_solution(ln, fM, sM)
 
                 answer.append("Обозначим за A - участники встретятся")
                 answer.append(f"P(A) = {result}")
 
                 return answer
@@ -357,18 +357,18 @@
         return str(matP)
 
 def find_math_prediction_terminal():
     """
     Нахождение МО по таблице значений случайных величин
     """
     n = int(input("Введите количество значений в таблице: "))
-    table = EttaTable()
+    table = utl.EttaTable()
     for i in range(0, n):
         v, p = map(float, input(f"введите пару чисел (значение, вероятность) для {i+1}-го значения").split())
-        table.cells.append(EttaTableCell(etta_value=v, probability=p))
+        table.cells.append(utl.EttaTableCell(etta_value=v, probability=p))
     result = find_math_prediction_solution(table)
     if "ошибка" not in result.lower():
         print(f"Mx = ⁱ⁼¹∑ⁿ(xi * pi) = {result}")
     else:
         print(result)
 
 def find_math_prediction_request(text: str = None):
@@ -379,24 +379,24 @@
         text (str): текст запроса, который может быть None или вводом пользователя
     
     Returns:
         list: массив строчек ответа
     """
     if text == None:
         return ["""Введите количество значений таблицы (число n)
-В следующих n строчках введите пары чисел: значение СВ, вероятность (любой разделитель, кроме точки)"""]
+В следующих n строчках введите пары чисел: значение СВ, вероятность (любой разделитель, кроме '.', ',', '/')"""]
     else:
         try:
-            request = [float(parameter) for parameter in re.findall(regular_float, text)]
+            request = glb.to_float_values(re.findall(glb.regular_float, text))
 
             n = int(request[0])
-            table = EttaTable()
+            table = utl.EttaTable()
 
             for i in range(0, n):
-                table.cells.append(EttaTableCell(etta_value=request[1+i*2], probability=request[2+i*2]))
+                table.cells.append(utl.EttaTableCell(etta_value=request[1+i*2], probability=request[2+i*2]))
 
             answer = []
 
             result = find_math_prediction_solution(table)
             if "ошибка" not in result.lower():
                 answer.append(f"Mx = ⁱ⁼¹∑ⁿ(xi * pi) = {find_math_prediction_solution(table)}")
             else:
@@ -427,18 +427,18 @@
             return "Ошибка при вычислении мат. ожидания. Проверьте коррекность введённых данных. (error code: 1)"
 
 def find_dispersion_terminal():
     """
     Функция, считающая дисперсию для таблицы СВ
     """
     n = int(input("Введите количество значений в таблице: "))
-    table = EttaTable()
+    table = utl.EttaTable()
     for i in range(0, n):
         v, p = map(float, input(f"введите пару чисел (значение, вероятность) для {i+1}-го значения").split())
-        table.cells.append(EttaTableCell(etta_value=v, probability=p))
+        table.cells.append(utl.EttaTableCell(etta_value=v, probability=p))
     result = find_dispersion_solution(table)
     if "ошибка" not in result.lower():
         print(f"Dx = ⁱ⁼¹∑ⁿ( (xi - M(X))² pi ) = {result}")
     else:
         print(result)
 
 def find_dispersion_request(text: str = None):
@@ -449,24 +449,24 @@
         text (str): текст запроса, который может быть None или вводом пользователя
     
     Returns:
         list: массив строчек ответа
     """
     if text == None:
         return ["""Введите количество значений таблицы (число n)
-В следующих n строчках введите пары чисел: значение СВ, вероятность (любой разделитель, кроме точки)"""]
+В следующих n строчках введите пары чисел: значение СВ, вероятность (любой разделитель, кроме  '.', ',', '/')"""]
     else:
         try:
-            request = [float(parameter) for parameter in re.findall(regular_float, text)]
+            request = glb.to_float_values(re.findall(glb.regular_float, text))
 
             n = int(request[0])
-            table = EttaTable()
+            table = utl.EttaTable()
 
             for i in range(0, n):
-                table.cells.append(EttaTableCell(etta_value=request[1+i*2], probability=request[2+i*2]))
+                table.cells.append(utl.EttaTableCell(etta_value=request[1+i*2], probability=request[2+i*2]))
 
             answer = []
 
             result = find_dispersion_solution(table)
             if "ошибка" not in result.lower():
                 answer.append(f"Dx = ⁱ⁼¹∑ⁿ( (xi - M(X))² pi ) = {result}")
             else:
@@ -492,18 +492,18 @@
     return [mat_prediction, dispersion]
 
 def table_analysis_terminal():
     """
     Функция, считающая дисперсию и математическое ожидание для таблицы СВ
     """
     n = int(input("Введите количество значений в таблице: "))
-    table = EttaTable()
+    table = utl.EttaTable()
     for i in range(0, n):
         v, p = map(float, input(f"введите пару чисел (значение, вероятность) для {i+1}-го значения: ").split())
-        table.cells.append(EttaTableCell(etta_value=v, probability=max(p,0)))
+        table.cells.append(utl.EttaTableCell(etta_value=v, probability=max(p,0)))
         
     result = table_analysis_solution(table)
 
     if "ошибка" not in result[0].lower() and "ошибка" not in result[1].lower():
         print(f"Mx = ⁱ⁼¹∑ⁿ(xi * pi) = {result[0]}\nDx = ⁱ⁼¹∑ⁿ( (xi - M(X))² pi ) = {result[1]}")
     else:
         print("Возникла ошибка при вычислении. Проверьте коррекность введённых данных.")
@@ -519,24 +519,24 @@
         text (str): текст запроса, который может быть None или вводом пользователя
     
     Returns:
         list: массив строчек ответа
     """
     if text == None:
         return ["""Введите количество значений таблицы (число n)
-В следующих n строчках введите пары чисел: значение СВ, вероятность (любой разделитель, кроме точки)"""]
+В следующих n строчках введите пары чисел: значение СВ, вероятность (любой разделитель, кроме  '.', ',', '/')"""]
     else:
         try:
-            request = [float(parameter) for parameter in re.findall(regular_float, text)]
+            request = glb.to_float_values(re.findall(glb.regular_float, text))
             print(request)
             n = int(request[0])
-            table = EttaTable()
+            table = utl.EttaTable()
 
             for i in range(0, n):
-                table.cells.append(EttaTableCell(etta_value=request[1+i*2], probability=max(request[2+i*2],0)))
+                table.cells.append(utl.EttaTableCell(etta_value=request[1+i*2], probability=max(request[2+i*2],0)))
                 print(table.cells[i].probability, table.cells[i].etta_value)
 
             answer = []
             result = table_analysis_solution(table)
             
             if "ошибка" not in result[0].lower() and "ошибка" not in result[1].lower():
                 answer.append(f"Mx = ⁱ⁼¹∑ⁿ(xi * pi) = {result[0]}")
```

