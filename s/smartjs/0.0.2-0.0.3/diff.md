# Comparing `tmp/smartjs-0.0.2.tar.gz` & `tmp/smartjs-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smartjs-0.0.2.tar", max compression
+gzip compressed data, was "smartjs-0.0.3.tar", max compression
```

## Comparing `smartjs-0.0.2.tar` & `smartjs-0.0.3.tar`

### file list

```diff
@@ -1,6 +1,12 @@
--rw-r--r--   0        0        0      302 2023-05-02 19:31:14.497807 smartjs-0.0.2/pyproject.toml
--rw-r--r--   0        0        0       64 2023-05-02 19:31:14.507976 smartjs-0.0.2/smartjs/__init__.py
--rw-r--r--   0        0        0     5676 2023-05-02 19:16:04.673162 smartjs-0.0.2/smartjs/functions.py
--rw-r--r--   0        0        0    10416 2023-05-02 19:31:14.522993 smartjs-0.0.2/smartjs/javascript.py
--rw-r--r--   0        0        0      584 2023-05-02 21:19:16.640853 smartjs-0.0.2/setup.py
--rw-r--r--   0        0        0      333 2023-05-02 21:19:16.641089 smartjs-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      327 2023-05-05 03:50:25.692153 smartjs-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      208 2023-05-05 01:28:03.905694 smartjs-0.0.3/smartjs/__init__.py
+-rw-r--r--   0        0        0    13312 2023-05-05 03:48:44.377945 smartjs-0.0.3/smartjs/base.py
+-rw-r--r--   0        0        0     2224 2023-05-05 03:50:25.688280 smartjs-0.0.3/smartjs/constants.py
+-rw-r--r--   0        0        0     4479 2023-05-04 15:42:17.533986 smartjs-0.0.3/smartjs/elements.py
+-rw-r--r--   0        0        0     1094 2023-05-05 01:54:13.346118 smartjs-0.0.3/smartjs/env.py
+-rw-r--r--   0        0        0     5801 2023-05-04 01:36:29.647942 smartjs-0.0.3/smartjs/functions.py
+-rw-r--r--   0        0        0    13893 2023-05-05 00:52:12.308743 smartjs-0.0.3/smartjs/javascript.py
+-rw-r--r--   0        0        0      619 2023-05-05 02:05:47.881002 smartjs-0.0.3/smartjs/page.py
+-rw-r--r--   0        0        0     1598 2023-05-05 03:48:44.383638 smartjs-0.0.3/smartjs/style.py
+-rw-r--r--   0        0        0      615 2023-05-05 03:50:31.019594 smartjs-0.0.3/setup.py
+-rw-r--r--   0        0        0      379 2023-05-05 03:50:31.019816 smartjs-0.0.3/PKG-INFO
```

### Comparing `smartjs-0.0.2/smartjs/functions.py` & `smartjs-0.0.3/smartjs/functions.py`

 * *Files 11% similar despite different names*

```diff
@@ -26,43 +26,37 @@
         'get_string_list_of_digits',
         'only_decimals',
         'get_group_or_return_none',
         'get_group_or_return_value',
         'get_iso_datetimes',
         'get_iso_dates',
         'get_first_iso_datetime',
-        'get_first_iso_date'
+        'get_first_iso_date',
+        'underscore_to_hyphen',
+        'list_of_type',
+        'set_filtered'
 ]
 
 import calendar
 import re
 import datetime
-from typing import Sequence, Callable, Optional, Union
+from typing import Callable, Optional, Collection, Union
 from unidecode import unidecode
+from smartjs.constants import *
 
 
-Number = Union[int, float]
-
-
-YEAR_PATTERN = re.compile(r'\b(19|20)\d{2}\b')
-
-DAY_PATTERN = re.compile(r'\b([0-2]\d|3[0-1])\b')
-
-MONTH_PATTERN = re.compile(r'\b(0\d|1[0-2])\b')
-
-ISO_DATE_PATTERN = re.compile(r'(19|20)(\d{2})(-)(01|02|03|04|05|06|07|08|09|10|11|12)(-)([0-3]\d)')
-
-ISO_DATETIME_PATTERN = re.compile(r'(19|20)(\d{2})(-)(01|02|03|04|05|06|07|08|09|10|11|12)(-)([0-3]\d)(T)([0-1]\d|2[0-3])(:)([0-5]\d)(?::[0-5]\d)?')
+def underscore_to_hyphen(value: str) -> str:
+    return value.replace("_", "-")
 
 
 def normalize(string: str) -> str:
     return ' '.join(unidecode(string).split()).lower()
 
 
-def repr_dict(data: dict, sep=", ") -> str:
+def repr_dict(data: dict, sep=" ") -> str:
     return join([f'{k}="{v}"' for k, v in dict_filtered(data).items()], sep=sep)
 
 
 def remove_extra_whitespaces(value: str) -> str:
     return remove_whitespace_before_final_point(re.sub(r'\s+', ' ', value))
 
 
@@ -75,24 +69,32 @@
 
 
 def age(start: datetime.date, end: datetime.date = None) -> float:
     end = end or datetime.date.today()
     return (((end - start).days - calendar.leapdays(start.year, end.year)) / 365).__round__(2)
 
 
-def list_filtered(items: Sequence, func: Callable = lambda x: x not in [None, '']) -> list:
+def list_filtered(items: Collection, func: Callable = lambda x: x not in [None, '']) -> list:
     return list(filter(func, items))
 
 
-def list_of_strings(items: Sequence) -> list[str]:
+def set_filtered(items: Collection, func: Callable = lambda x: x not in [None, '']) -> set:
+    return set(list_filtered(items, func))
+
+
+def list_of_type(items: Collection, types: Union[type[GenericType], tuple[type[GenericType]]]) -> list[GenericType]:
+    return [item for item in items if isinstance(item, types)]
+
+
+def list_of_strings(items: Collection) -> list[str]:
     return [str(i) for i in list_filtered(items)]
 
 
-def join(items: Sequence, sep: str = ' ', end: str = '') -> str:
-    return sep.join(list_of_strings(items)) + end
+def join(items: Collection, sep: str = ' ', end: str = '') -> str:
+    return sep.join([str(item) for item in items if item not in [None, '']]) + end
 
 
 def dict_filtered(data: dict, function: Callable = lambda x: x not in [None, '', " "]) -> dict:
     new = dict()
     for key, value in data.items():
         if function(value):
             new[key] = value
@@ -197,12 +199,14 @@
 
 def get_iso_dates(value: str) -> list[Optional[str]]:
     result = ISO_DATE_PATTERN.findall(value)
     if result:
         return [join(i, sep='') for i in result]
     return []
 
+
 def get_iso_datetimes(value: str) -> list[Optional[str]]:
     result = ISO_DATETIME_PATTERN.findall(value)
     if result:
         return [join(i, sep='') for i in result]
     return []
+
```

### Comparing `smartjs-0.0.2/setup.py` & `smartjs-0.0.3/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 packages = \
 ['smartjs']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['Unidecode>=1.3.6,<2.0.0']
+['Unidecode>=1.3.6,<2.0.0', 'python-dotenv>=1.0.0,<2.0.0']
 
 setup_kwargs = {
     'name': 'smartjs',
-    'version': '0.0.2',
+    'version': '0.0.3',
     'description': '',
     'long_description': None,
     'author': 'Daniel Victor',
     'author_email': 'arantesdv@me.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

