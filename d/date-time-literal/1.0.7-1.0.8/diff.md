# Comparing `tmp/date_time_literal-1.0.7.tar.gz` & `tmp/date_time_literal-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "date_time_literal-1.0.7.tar", last modified: Tue May 31 22:37:57 2022, max compression
+gzip compressed data, was "date_time_literal-1.0.8.tar", last modified: Fri May  5 11:10:02 2023, max compression
```

## Comparing `date_time_literal-1.0.7.tar` & `date_time_literal-1.0.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 kells     (1000) kells     (1000)        0 2022-05-31 22:37:57.650796 date_time_literal-1.0.7/
--rw-rw-r--   0 kells     (1000) kells     (1000)     1062 2022-05-31 22:12:21.000000 date_time_literal-1.0.7/LICENSE
--rw-rw-r--   0 kells     (1000) kells     (1000)     4940 2022-05-31 22:37:57.650796 date_time_literal-1.0.7/PKG-INFO
--rw-rw-r--   0 kells     (1000) kells     (1000)     4008 2022-05-31 22:12:21.000000 date_time_literal-1.0.7/README.md
-drwxrwxr-x   0 kells     (1000) kells     (1000)        0 2022-05-31 22:37:57.650796 date_time_literal-1.0.7/date_time_literal/
--rw-rw-r--   0 kells     (1000) kells     (1000)       49 2022-05-31 22:12:21.000000 date_time_literal-1.0.7/date_time_literal/__init__.py
--rw-rw-r--   0 kells     (1000) kells     (1000)     5930 2022-05-31 22:12:21.000000 date_time_literal-1.0.7/date_time_literal/difference.py
--rw-rw-r--   0 kells     (1000) kells     (1000)     6539 2022-05-31 22:12:21.000000 date_time_literal-1.0.7/date_time_literal/literal.py
--rw-rw-r--   0 kells     (1000) kells     (1000)      680 2022-05-31 22:12:21.000000 date_time_literal-1.0.7/date_time_literal/main.py
-drwxrwxr-x   0 kells     (1000) kells     (1000)        0 2022-05-31 22:37:57.650796 date_time_literal-1.0.7/date_time_literal.egg-info/
--rw-rw-r--   0 kells     (1000) kells     (1000)     4940 2022-05-31 22:37:57.000000 date_time_literal-1.0.7/date_time_literal.egg-info/PKG-INFO
--rw-rw-r--   0 kells     (1000) kells     (1000)      317 2022-05-31 22:37:57.000000 date_time_literal-1.0.7/date_time_literal.egg-info/SOURCES.txt
--rw-rw-r--   0 kells     (1000) kells     (1000)        1 2022-05-31 22:37:57.000000 date_time_literal-1.0.7/date_time_literal.egg-info/dependency_links.txt
--rw-rw-r--   0 kells     (1000) kells     (1000)       18 2022-05-31 22:37:57.000000 date_time_literal-1.0.7/date_time_literal.egg-info/top_level.txt
--rw-rw-r--   0 kells     (1000) kells     (1000)       79 2022-05-31 22:37:57.650796 date_time_literal-1.0.7/setup.cfg
--rw-rw-r--   0 kells     (1000) kells     (1000)     1405 2022-05-31 22:12:21.000000 date_time_literal-1.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-05 11:10:02.236485 date_time_literal-1.0.8/
+-rw-rw-rw-   0        0        0     1083 2022-05-31 19:43:31.000000 date_time_literal-1.0.8/LICENSE
+-rw-rw-rw-   0        0        0     5188 2023-05-05 11:10:02.237834 date_time_literal-1.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     4240 2023-05-05 11:03:01.000000 date_time_literal-1.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-05-05 11:10:02.188731 date_time_literal-1.0.8/date_time_literal/
+-rw-rw-rw-   0        0        0       51 2022-05-31 19:43:31.000000 date_time_literal-1.0.8/date_time_literal/__init__.py
+-rw-rw-rw-   0        0        0     3969 2023-05-05 10:58:57.000000 date_time_literal-1.0.8/date_time_literal/difference.py
+-rw-rw-rw-   0        0        0     6724 2022-05-31 20:04:31.000000 date_time_literal-1.0.8/date_time_literal/literal.py
+-rw-rw-rw-   0        0        0      706 2023-05-05 10:59:51.000000 date_time_literal-1.0.8/date_time_literal/main.py
+drwxrwxrwx   0        0        0        0 2023-05-05 11:10:02.233801 date_time_literal-1.0.8/date_time_literal.egg-info/
+-rw-rw-rw-   0        0        0     5188 2023-05-05 11:10:02.000000 date_time_literal-1.0.8/date_time_literal.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      317 2023-05-05 11:10:02.000000 date_time_literal-1.0.8/date_time_literal.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 11:10:02.000000 date_time_literal-1.0.8/date_time_literal.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-05-05 11:10:02.000000 date_time_literal-1.0.8/date_time_literal.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-05-05 11:10:02.239360 date_time_literal-1.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     1435 2023-05-05 11:03:01.000000 date_time_literal-1.0.8/setup.py
```

### Comparing `date_time_literal-1.0.7/PKG-INFO` & `date_time_literal-1.0.8/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,128 +1,113 @@
-Metadata-Version: 2.1
-Name: date_time_literal
-Version: 1.0.7
-Summary: date-time-literal is a python module that helps convert date-time or date to literal days, hours, seconds, or even minutes. Compare two DateTime or Date objects, by converting the objects to literal days, hours, minutes, or even seconds if you want to be precise. 
-Home-page: https://github.com/kells4real/date_literal
-Download-URL: https://github.com/kells4real/date_literal/archive/refs/tags/1.0.0.tar.gz
-Author: Kelvin Sajere
-Author-email: kells4real@gmail.com
-Keywords: date-time,date,literal,date converter,literal date,date-time converter,django,python,module,python package,date-time literal,convert time,convert date-time
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.5
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# date_literal
-A package/module for converting date or date-time formats to literal days, hours, minutes, or seconds for comparison or whatever. 
-For example, you can convert DateTime objects to know just how much of a difference there is between them, or you just want 
-to get the human-readable format of DateTime or Date objects.
-
-## Installation
-> pip install date_time_literal
-
-## Usage
-#### IMPORTANT
-DateTime or Date objects must be in the default 'Y-M-D Hr:Min:Sec' and 'Y-M-D' formats respectively.
-
-##### Converts Date Time Literal
-```python
-from django.utils import timezone
-time = timezone.now()
-from date_time_literal import ConvertTime
-convert_time = ConvertTime(time).slug_date_time
-```
-##### Converts Date Literal
-convert_time = ConvertTime(time).slug_date
-This returns the date or date-time in seconds. You can add an optional parameter to specify what you want.
-
-Note: You can use the slug_date class function on a DateTime object if you wish to use only the date part of the DateTime object, 
-but cannot use the slug_date_time class function on a Date object, only on DateTime objects.
-
-#### Specific conversion to days
-
-```python
-from django.utils import timezone
-from datetime import datetime
-from date_time_literal import ConvertTime
-
-time2 = datetime.now()
-time = timezone.now()
-
-convert_time = ConvertTime(time, 'd').slug_date_time
-convert_time2 = ConvertTime(time2, 'd').slug_date
-```
-
-#### Specific conversion to hours
-
-```python
-from date_time_literal import ConvertTime
-from datetime import datetime
-time = datetime.now()
-convert_time = ConvertTime(time, 'd').slug_date_time # Converts the DateTime object to days
-convert_time1 = ConvertTime(time, 'h').slug_date_time # Converts the DateTime object to hours
-convert_time2 = ConvertTime(time, 'm').slug_date_time # Converts the DateTime object to minutes
-
-# The default conversion if none is specified is to seconds
-```
-
-### CHECK DATE-TIME OR DATE DIFFERENCE BETWEEN TWO DATE-TIME OR DATE LITERALS
-
-```python
-from date_time_literal import ConvertTime
-from datetime import datetime
-from django.utils import timezone
-time = datetime.now()
-convert_time = ConvertTime(time, 'h').slug_date_time
-from date_time_literal import date_time_diff, date_diff
-convert_time2 = ConvertTime(time, 'm').slug_date_time
-date1 = '2021-05-31'
-date2 = '2021-03-21'
-date_time1 = timezone.now()
-date_time2 = '2021-03-21 23:16:45.735963'
-date_l = date_diff(date1, date2, 'd')
-date_time_l = date_time_diff(date_time1, date_time2, 'd')
-
-# date_time_l will return the difference in value between date_time1 and date_time2 in days. You can use the 
-# corresponding string literal to get for minutes, hours and seconds which is the default value.
-# date_time_diff returns the difference in two dateTimes to the second. This should be used when you need to get 
-# date time difference to the last second
-
-```
-
-## Convert between time and dates
-You can also use the convert_time function to convert between times
-
-```python
-from date_time_literal import convert_time
-
-# Converts between years, days, hours, minutes, and seconds
-print(convert_time(365, 'd', 'y')) # Converts 365 days to years
-print(convert_time(5, 'y', 'd')) # Converts 5 years to days
-print(convert_time(5, 'y', 'h')) # Converts 5 years to hours
-print(convert_time(5, 'd', 's')) # Converts 5 days to seconds
-# etc
-```
-
-### Some Basic use cases
-To get a rather comprehensive idea of how the package works, copy the code below and run it.
-
-```python
-from date_time_literal import ConvertTime, DateDiff, date_diff, convert_time
-from datetime import datetime
-
-t = ConvertTime('2021-05-31 23:16:55.321568', 'd')
-p = ConvertTime(datetime.now(), 'd')
-i = ConvertTime('2021-05-31 23:16:55+00:00', 'd')
-d = ConvertTime('2021-05-31', time_format='d')
-e = DateDiff('2021-05-31', '2021-04-31', 'd')
-print(t.slug_date_time)
-print(i.slug_date_time)
-print(d.slug_date)
-print(e.date_diff)
-print(date_diff('2021-08-31', '2021-05-30', 'D'))
-print(convert_time(1, "y", 'h'))
-print(convert_time(365, 'd', 'y'))
-
-```
+# date_literal
+A package/module for converting date or date-time formats to literal days, hours, minutes, or seconds for comparison or whatever. 
+For example, you can convert DateTime objects to know just how much of a difference there is between them, or you just want 
+to get the human-readable format of DateTime or Date objects.
+
+## Installation
+> pip install date_time_literal
+
+## Usage
+#### IMPORTANT
+DateTime or Date objects must be in the default 'Y-M-D Hr:Min:Sec' and 'Y-M-D' formats respectively.
+
+##### Converts Date Time Literal
+```python
+from django.utils import timezone
+time = timezone.now()
+from date_time_literal import ConvertTime
+convert_time = ConvertTime(time).slug_date_time
+```
+##### Converts Date Literal
+convert_time = ConvertTime(time).slug_date
+This returns the date or date-time in seconds. You can add an optional parameter to specify what you want.
+
+Note: You can use the slug_date class function on a DateTime object if you wish to use only the date part of the DateTime object, 
+but cannot use the slug_date_time class function on a Date object, only on DateTime objects.
+
+#### Specific conversion to days
+
+```python
+from django.utils import timezone
+from datetime import datetime
+from date_time_literal import ConvertTime
+
+time2 = datetime.now()
+time = timezone.now()
+
+convert_time = ConvertTime(time, 'd').slug_date_time
+convert_time2 = ConvertTime(time2, 'd').slug_date
+```
+
+#### Specific conversion to hours
+
+```python
+from date_time_literal import ConvertTime
+from datetime import datetime
+time = datetime.now()
+convert_time = ConvertTime(time, 'd').slug_date_time # Converts the DateTime object to days
+convert_time1 = ConvertTime(time, 'h').slug_date_time # Converts the DateTime object to hours
+convert_time2 = ConvertTime(time, 'm').slug_date_time # Converts the DateTime object to minutes
+
+# The default conversion if none is specified is to seconds
+```
+
+### CHECK DATE-TIME OR DATE DIFFERENCE BETWEEN TWO DATE-TIME OR DATE LITERALS
+
+```python
+from date_time_literal import ConvertTime
+from datetime import datetime
+from django.utils import timezone
+time = datetime.now()
+convert_time = ConvertTime(time, 'h').slug_date_time
+from date_time_literal import date_time_diff, date_diff
+convert_time2 = ConvertTime(time, 'm').slug_date_time
+date1 = '2021-05-31'
+date2 = '2021-03-21'
+date_time1 = timezone.now()
+date_time2 = '2021-03-21 23:16:45.735963'
+date_l = date_diff(date1, date2, 'd')
+date_time_l = date_time_diff(date_time1, date_time2, 'd')
+
+# date_time_l will return the difference in value between date_time1 and date_time2 in days. You can use the 
+# corresponding string literal to get for minutes, hours and seconds which is the default value.
+# date_time_diff returns the difference in two dateTimes to the second. This should be used when you need to get 
+# date time difference to the last second
+
+```
+
+## Convert between time and dates
+You can also use the convert_time function to convert between times
+
+```python
+from date_time_literal import convert_time
+
+# Converts between years, days, hours, minutes, and seconds
+print(convert_time(365, 'd', 'y')) # Converts 365 days to years
+print(convert_time(5, 'y', 'd')) # Converts 5 years to days
+print(convert_time(5, 'y', 'h')) # Converts 5 years to hours
+print(convert_time(5, 'd', 's')) # Converts 5 days to seconds
+# etc
+```
+
+### Some Basic use cases
+To get a rather comprehensive idea of how the package works, copy the code below and run it. The convert_time function
+was updated to be more efficient and now allows for week conversion as well in version 1.0.8
+
+```python
+from date_time_literal import ConvertTime, DateDiff, date_diff, convert_time
+from datetime import datetime
+
+t = ConvertTime('2021-05-31 23:16:55.321568', 'd')
+p = ConvertTime(datetime.now(), 'd')
+i = ConvertTime('2021-05-31 23:16:55+00:00', 'd')
+d = ConvertTime('2021-05-31', time_format='d')
+e = DateDiff('2021-05-31', '2021-04-31', 'd')
+print(t.slug_date_time)
+print(i.slug_date_time)
+print(d.slug_date)
+print(e.date_diff)
+print(date_diff('2021-08-31', '2021-05-30', 'D'))
+print(convert_time(1, "y", 'h'))
+print(convert_time(365, 'd', 'y'))
+
+```
```

### Comparing `date_time_literal-1.0.7/date_time_literal/literal.py` & `date_time_literal-1.0.8/date_time_literal/literal.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,409 +1,421 @@
-00000000: 0a63 6c61 7373 2043 6f6e 7665 7274 5469  .class ConvertTi
-00000010: 6d65 3a0a 2020 2020 6465 6620 5f5f 696e  me:.    def __in
-00000020: 6974 5f5f 2873 656c 662c 2074 696d 652c  it__(self, time,
-00000030: 2074 696d 655f 666f 726d 6174 3d27 7327   time_format='s'
-00000040: 293a 0a20 2020 2020 2020 2073 656c 662e  ):.        self.
-00000050: 7469 6d65 203d 2074 696d 650a 2020 2020  time = time.    
-00000060: 2020 2020 7365 6c66 2e74 696d 655f 3a20      self.time_: 
-00000070: 7374 7220 3d20 7469 6d65 5f66 6f72 6d61  str = time_forma
-00000080: 740a 0a20 2020 2040 7072 6f70 6572 7479  t..    @property
-00000090: 0a20 2020 2064 6566 2073 6c75 675f 6461  .    def slug_da
-000000a0: 7465 5f74 696d 6528 7365 6c66 293a 0a20  te_time(self):. 
-000000b0: 2020 2020 2020 2073 6c75 675f 7469 6d65         slug_time
-000000c0: 203d 2073 7472 2873 656c 662e 7469 6d65   = str(self.time
-000000d0: 290a 2020 2020 2020 2020 6669 7273 7420  ).        first 
-000000e0: 3d20 736c 7567 5f74 696d 652e 7370 6c69  = slug_time.spli
-000000f0: 7428 222d 2229 0a20 2020 2020 2020 2073  t("-").        s
-00000100: 6563 6f6e 6420 3d20 6669 7273 745b 303a  econd = first[0:
-00000110: 325d 0a20 2020 2020 2020 2074 6869 7264  2].        third
-00000120: 203d 2066 6972 7374 5b32 5d0a 2020 2020   = first[2].    
-00000130: 2020 2020 666f 7572 7468 203d 2074 6869      fourth = thi
-00000140: 7264 2e73 706c 6974 2822 2022 295b 315d  rd.split(" ")[1]
-00000150: 2e73 706c 6974 2822 3a22 290a 2020 2020  .split(":").    
-00000160: 2020 2020 6920 3d20 7365 636f 6e64 5b30      i = second[0
-00000170: 5d0a 2020 2020 2020 2020 6a20 3d20 7365  ].        j = se
-00000180: 636f 6e64 5b31 5d0a 2020 2020 2020 2020  cond[1].        
-00000190: 6b20 3d20 7468 6972 642e 7370 6c69 7428  k = third.split(
-000001a0: 2220 2229 5b30 5d0a 2020 2020 2020 2020  " ")[0].        
-000001b0: 6872 7320 3d20 696e 7428 666f 7572 7468  hrs = int(fourth
-000001c0: 5b30 5d29 0a20 2020 2020 2020 206d 696e  [0]).        min
-000001d0: 7320 3d20 696e 7428 666f 7572 7468 5b31  s = int(fourth[1
-000001e0: 5d29 0a20 2020 2020 2020 2073 6563 7320  ]).        secs 
-000001f0: 3d20 666f 7572 7468 5b32 5d2e 7370 6c69  = fourth[2].spli
-00000200: 7428 222e 2229 5b30 5d0a 2020 2020 2020  t(".")[0].      
-00000210: 2020 6966 2027 2b27 2069 6e20 7365 6373    if '+' in secs
-00000220: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-00000230: 6373 203d 2073 6563 732e 7370 6c69 7428  cs = secs.split(
-00000240: 272b 2729 5b30 5d0a 2020 2020 2020 2020  '+')[0].        
-00000250: 7365 6373 5f69 6e74 203d 2069 6e74 2873  secs_int = int(s
-00000260: 6563 7329 0a20 2020 2020 2020 2079 6561  ecs).        yea
-00000270: 725f 696e 5f64 6179 7320 3d20 696e 7428  r_in_days = int(
-00000280: 6929 202a 2033 3635 0a20 2020 2020 2020  i) * 365.       
-00000290: 2079 6561 7273 203d 2069 6e74 2879 6561   years = int(yea
-000002a0: 725f 696e 5f64 6179 7329 0a20 2020 2020  r_in_days).     
-000002b0: 2020 206d 6f6e 7468 7320 3d20 696e 7428     months = int(
-000002c0: 6a29 202a 2033 300a 2020 2020 2020 2020  j) * 30.        
-000002d0: 6461 7973 203d 2069 6e74 286b 290a 2020  days = int(k).  
-000002e0: 2020 2020 2020 6966 2073 656c 662e 7469        if self.ti
-000002f0: 6d65 5f20 3d3d 2027 6d27 3a0a 2020 2020  me_ == 'm':.    
-00000300: 2020 2020 2020 2020 6765 745f 6461 7973          get_days
-00000310: 5f6d 696e 7320 3d20 2868 7273 202a 2036  _mins = (hrs * 6
-00000320: 3029 202b 206d 696e 730a 2020 2020 2020  0) + mins.      
-00000330: 2020 2020 2020 6765 745f 7965 6172 735f        get_years_
-00000340: 6d69 6e73 203d 2028 7965 6172 7320 2b20  mins = (years + 
-00000350: 6d6f 6e74 6873 202b 2064 6179 7329 202a  months + days) *
-00000360: 2032 3420 2a20 3630 0a20 2020 2020 2020   24 * 60.       
-00000370: 2020 2020 2072 6574 7572 6e20 6765 745f       return get_
-00000380: 7965 6172 735f 6d69 6e73 202b 2067 6574  years_mins + get
-00000390: 5f64 6179 735f 6d69 6e73 0a20 2020 2020  _days_mins.     
-000003a0: 2020 2065 6c69 6620 7365 6c66 2e74 696d     elif self.tim
-000003b0: 655f 203d 3d20 2768 273a 0a20 2020 2020  e_ == 'h':.     
-000003c0: 2020 2020 2020 2067 6574 5f64 6179 735f         get_days_
-000003d0: 6d69 6e73 203d 2028 6872 7320 2a20 3630  mins = (hrs * 60
-000003e0: 2920 2b20 6d69 6e73 0a20 2020 2020 2020  ) + mins.       
-000003f0: 2020 2020 2067 6574 5f79 6561 7273 5f6d       get_years_m
-00000400: 696e 7320 3d20 2879 6561 7273 202b 206d  ins = (years + m
-00000410: 6f6e 7468 7320 2b20 6461 7973 2920 2a20  onths + days) * 
-00000420: 3234 202a 2036 300a 2020 2020 2020 2020  24 * 60.        
-00000430: 2020 2020 7265 7475 726e 2072 6f75 6e64      return round
-00000440: 2828 6765 745f 7965 6172 735f 6d69 6e73  ((get_years_mins
-00000450: 202b 2067 6574 5f64 6179 735f 6d69 6e73   + get_days_mins
-00000460: 2920 2f20 3630 2c20 3229 0a20 2020 2020  ) / 60, 2).     
-00000470: 2020 2065 6c69 6620 7365 6c66 2e74 696d     elif self.tim
-00000480: 655f 203d 3d20 2764 273a 0a20 2020 2020  e_ == 'd':.     
-00000490: 2020 2020 2020 2067 6574 5f79 6561 7273         get_years
-000004a0: 5f64 6179 7320 3d20 7965 6172 7320 2b20  _days = years + 
-000004b0: 6d6f 6e74 6873 202b 2064 6179 730a 2020  months + days.  
-000004c0: 2020 2020 2020 2020 2020 7265 7475 726e            return
-000004d0: 2067 6574 5f79 6561 7273 5f64 6179 730a   get_years_days.
-000004e0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-000004f0: 2020 2020 2020 2020 2020 6765 745f 6461            get_da
-00000500: 7973 5f73 6563 7320 3d20 2868 7273 202a  ys_secs = (hrs *
-00000510: 2036 3020 2a20 3630 2920 2b20 286d 696e   60 * 60) + (min
-00000520: 7320 2a20 3630 2920 2b20 7365 6373 5f69  s * 60) + secs_i
-00000530: 6e74 0a20 2020 2020 2020 2020 2020 2067  nt.            g
-00000540: 6574 5f79 6561 7273 5f73 6563 7320 3d20  et_years_secs = 
-00000550: 2879 6561 7273 202b 206d 6f6e 7468 7320  (years + months 
-00000560: 2b20 6461 7973 2920 2a20 3234 202a 2036  + days) * 24 * 6
-00000570: 3020 2a20 3630 0a20 2020 2020 2020 2020  0 * 60.         
-00000580: 2020 2072 6574 7572 6e20 6765 745f 7965     return get_ye
-00000590: 6172 735f 7365 6373 202b 2067 6574 5f64  ars_secs + get_d
-000005a0: 6179 735f 7365 6373 0a0a 2020 2020 4070  ays_secs..    @p
-000005b0: 726f 7065 7274 790a 2020 2020 6465 6620  roperty.    def 
-000005c0: 736c 7567 5f64 6174 6528 7365 6c66 293a  slug_date(self):
-000005d0: 0a20 2020 2020 2020 2073 6c75 675f 7469  .        slug_ti
-000005e0: 6d65 3a20 7374 7220 3d20 7374 7228 7365  me: str = str(se
-000005f0: 6c66 2e74 696d 6529 0a20 2020 2020 2020  lf.time).       
-00000600: 2066 6972 7374 203d 2073 6c75 675f 7469   first = slug_ti
-00000610: 6d65 2e73 706c 6974 2822 2d22 290a 2020  me.split("-").  
-00000620: 2020 2020 2020 7365 636f 6e64 203d 2066        second = f
-00000630: 6972 7374 5b30 3a32 5d0a 2020 2020 2020  irst[0:2].      
-00000640: 2020 7468 6972 6420 3d20 6669 7273 745b    third = first[
-00000650: 325d 0a20 2020 2020 2020 2069 203d 2073  2].        i = s
-00000660: 6563 6f6e 645b 305d 0a20 2020 2020 2020  econd[0].       
-00000670: 206a 203d 2073 6563 6f6e 645b 315d 0a20   j = second[1]. 
-00000680: 2020 2020 2020 206b 203d 2074 6869 7264         k = third
-00000690: 2e73 706c 6974 2822 2022 295b 305d 0a20  .split(" ")[0]. 
-000006a0: 2020 2020 2020 2079 6561 725f 696e 5f64         year_in_d
-000006b0: 6179 7320 3d20 696e 7428 6929 202a 2033  ays = int(i) * 3
-000006c0: 3635 0a20 2020 2020 2020 2079 6561 7273  65.        years
-000006d0: 203d 2069 6e74 2879 6561 725f 696e 5f64   = int(year_in_d
-000006e0: 6179 7329 0a20 2020 2020 2020 206d 6f6e  ays).        mon
-000006f0: 7468 7320 3d20 696e 7428 6a29 202a 2033  ths = int(j) * 3
-00000700: 300a 2020 2020 2020 2020 6461 7973 203d  0.        days =
-00000710: 2069 6e74 286b 290a 2020 2020 2020 2020   int(k).        
-00000720: 6966 2073 656c 662e 7469 6d65 5f20 3d3d  if self.time_ ==
-00000730: 2027 6d27 3a0a 2020 2020 2020 2020 2020   'm':.          
-00000740: 2020 6765 745f 6d69 6e73 203d 2028 7965    get_mins = (ye
-00000750: 6172 7320 2b20 6d6f 6e74 6873 202b 2064  ars + months + d
-00000760: 6179 7329 202a 2032 3420 2a20 3630 0a20  ays) * 24 * 60. 
-00000770: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00000780: 6e20 6765 745f 6d69 6e73 0a20 2020 2020  n get_mins.     
-00000790: 2020 2065 6c69 6620 7365 6c66 2e74 696d     elif self.tim
-000007a0: 655f 203d 3d20 2768 273a 0a20 2020 2020  e_ == 'h':.     
-000007b0: 2020 2020 2020 2067 6574 5f68 7273 203d         get_hrs =
-000007c0: 2072 6f75 6e64 2828 2879 6561 7273 202b   round(((years +
-000007d0: 206d 6f6e 7468 7320 2b20 6461 7973 2920   months + days) 
-000007e0: 2a20 3234 202a 2036 3029 202f 2036 302c  * 24 * 60) / 60,
-000007f0: 2032 290a 2020 2020 2020 2020 2020 2020   2).            
-00000800: 7265 7475 726e 2067 6574 5f68 7273 0a20  return get_hrs. 
-00000810: 2020 2020 2020 2065 6c69 6620 7365 6c66         elif self
-00000820: 2e74 696d 655f 203d 3d20 2764 273a 0a20  .time_ == 'd':. 
-00000830: 2020 2020 2020 2020 2020 2067 6574 5f64             get_d
-00000840: 6179 7320 3d20 7965 6172 7320 2b20 6d6f  ays = years + mo
-00000850: 6e74 6873 202b 2064 6179 730a 2020 2020  nths + days.    
-00000860: 2020 2020 2020 2020 7265 7475 726e 2067          return g
-00000870: 6574 5f64 6179 730a 2020 2020 2020 2020  et_days.        
-00000880: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-00000890: 2020 6765 745f 7365 6373 203d 2028 7965    get_secs = (ye
-000008a0: 6172 7320 2b20 6d6f 6e74 6873 202b 2064  ars + months + d
-000008b0: 6179 7329 202a 2032 3420 2a20 3630 202a  ays) * 24 * 60 *
-000008c0: 2036 300a 2020 2020 2020 2020 2020 2020   60.            
-000008d0: 7265 7475 726e 2067 6574 5f73 6563 730a  return get_secs.
-000008e0: 0a0a 636c 6173 7320 4461 7465 4469 6666  ..class DateDiff
-000008f0: 3a0a 2020 2020 6465 6620 5f5f 696e 6974  :.    def __init
-00000900: 5f5f 2873 656c 662c 2074 696d 6531 2c20  __(self, time1, 
-00000910: 7469 6d65 322c 2074 696d 655f 666f 726d  time2, time_form
-00000920: 6174 3d27 7327 293a 0a20 2020 2020 2020  at='s'):.       
-00000930: 2073 656c 662e 7469 6d65 3120 3d20 7469   self.time1 = ti
-00000940: 6d65 310a 2020 2020 2020 2020 7365 6c66  me1.        self
-00000950: 2e74 696d 6532 203d 2074 696d 6532 0a20  .time2 = time2. 
-00000960: 2020 2020 2020 2073 656c 662e 7469 6d65         self.time
-00000970: 5f3a 2073 7472 203d 2074 696d 655f 666f  _: str = time_fo
-00000980: 726d 6174 0a0a 2020 2020 4070 726f 7065  rmat..    @prope
-00000990: 7274 790a 2020 2020 6465 6620 6461 7465  rty.    def date
-000009a0: 5f74 696d 655f 6469 6666 2873 656c 6629  _time_diff(self)
-000009b0: 3a0a 2020 2020 2020 2020 2320 7469 6d65  :.        # time
-000009c0: 2031 0a20 2020 2020 2020 2073 6c75 675f   1.        slug_
-000009d0: 7469 6d65 3120 3d20 7374 7228 7365 6c66  time1 = str(self
-000009e0: 2e74 696d 6531 290a 2020 2020 2020 2020  .time1).        
-000009f0: 6669 7273 7420 3d20 736c 7567 5f74 696d  first = slug_tim
-00000a00: 6531 2e73 706c 6974 2822 2d22 290a 2020  e1.split("-").  
-00000a10: 2020 2020 2020 7365 636f 6e64 203d 2066        second = f
-00000a20: 6972 7374 5b30 3a32 5d0a 2020 2020 2020  irst[0:2].      
-00000a30: 2020 7468 6972 6420 3d20 6669 7273 745b    third = first[
-00000a40: 325d 0a20 2020 2020 2020 2066 6f75 7274  2].        fourt
-00000a50: 6820 3d20 7468 6972 642e 7370 6c69 7428  h = third.split(
-00000a60: 2220 2229 5b31 5d2e 7370 6c69 7428 223a  " ")[1].split(":
-00000a70: 2229 0a20 2020 2020 2020 2069 203d 2073  ").        i = s
-00000a80: 6563 6f6e 645b 305d 0a20 2020 2020 2020  econd[0].       
-00000a90: 206a 203d 2073 6563 6f6e 645b 315d 0a20   j = second[1]. 
-00000aa0: 2020 2020 2020 206b 203d 2074 6869 7264         k = third
-00000ab0: 2e73 706c 6974 2822 2022 295b 305d 0a20  .split(" ")[0]. 
-00000ac0: 2020 2020 2020 2068 7273 203d 2069 6e74         hrs = int
-00000ad0: 2866 6f75 7274 685b 305d 290a 2020 2020  (fourth[0]).    
-00000ae0: 2020 2020 6d69 6e73 203d 2069 6e74 2866      mins = int(f
-00000af0: 6f75 7274 685b 315d 290a 2020 2020 2020  ourth[1]).      
-00000b00: 2020 7365 6373 203d 2066 6f75 7274 685b    secs = fourth[
-00000b10: 325d 2e73 706c 6974 2822 2e22 295b 305d  2].split(".")[0]
-00000b20: 0a20 2020 2020 2020 2069 6620 272b 2720  .        if '+' 
-00000b30: 696e 2073 6563 733a 0a20 2020 2020 2020  in secs:.       
-00000b40: 2020 2020 2073 6563 7320 3d20 7365 6373       secs = secs
-00000b50: 2e73 706c 6974 2827 2b27 295b 305d 0a20  .split('+')[0]. 
-00000b60: 2020 2020 2020 2073 6563 735f 696e 7420         secs_int 
-00000b70: 3d20 696e 7428 7365 6373 290a 2020 2020  = int(secs).    
-00000b80: 2020 2020 7965 6172 5f69 6e5f 6461 7973      year_in_days
-00000b90: 203d 2069 6e74 2869 2920 2a20 3336 350a   = int(i) * 365.
-00000ba0: 2020 2020 2020 2020 7965 6172 7320 3d20          years = 
-00000bb0: 696e 7428 7965 6172 5f69 6e5f 6461 7973  int(year_in_days
-00000bc0: 290a 2020 2020 2020 2020 6d6f 6e74 6873  ).        months
-00000bd0: 203d 2069 6e74 286a 2920 2a20 3330 0a20   = int(j) * 30. 
-00000be0: 2020 2020 2020 2064 6179 7320 3d20 696e         days = in
-00000bf0: 7428 6b29 0a0a 2020 2020 2020 2020 2320  t(k)..        # 
-00000c00: 7469 6d65 320a 2020 2020 2020 2020 736c  time2.        sl
-00000c10: 7567 5f74 696d 6532 203d 2073 7472 2873  ug_time2 = str(s
-00000c20: 656c 662e 7469 6d65 3229 0a20 2020 2020  elf.time2).     
-00000c30: 2020 2066 6972 7374 3220 3d20 736c 7567     first2 = slug
-00000c40: 5f74 696d 6532 2e73 706c 6974 2822 2d22  _time2.split("-"
-00000c50: 290a 2020 2020 2020 2020 7365 636f 6e64  ).        second
-00000c60: 3220 3d20 6669 7273 7432 5b30 3a32 5d0a  2 = first2[0:2].
-00000c70: 2020 2020 2020 2020 7468 6972 6432 203d          third2 =
-00000c80: 2066 6972 7374 325b 325d 0a20 2020 2020   first2[2].     
-00000c90: 2020 2066 6f75 7274 6832 203d 2074 6869     fourth2 = thi
-00000ca0: 7264 322e 7370 6c69 7428 2220 2229 5b31  rd2.split(" ")[1
-00000cb0: 5d2e 7370 6c69 7428 223a 2229 0a20 2020  ].split(":").   
-00000cc0: 2020 2020 2069 3220 3d20 7365 636f 6e64       i2 = second
-00000cd0: 325b 305d 0a20 2020 2020 2020 206a 3220  2[0].        j2 
-00000ce0: 3d20 7365 636f 6e64 325b 315d 0a20 2020  = second2[1].   
-00000cf0: 2020 2020 206b 3220 3d20 7468 6972 6432       k2 = third2
-00000d00: 2e73 706c 6974 2822 2022 295b 305d 0a20  .split(" ")[0]. 
-00000d10: 2020 2020 2020 2068 7273 3220 3d20 696e         hrs2 = in
-00000d20: 7428 666f 7572 7468 325b 305d 290a 2020  t(fourth2[0]).  
-00000d30: 2020 2020 2020 6d69 6e73 3220 3d20 696e        mins2 = in
-00000d40: 7428 666f 7572 7468 325b 315d 290a 2020  t(fourth2[1]).  
-00000d50: 2020 2020 2020 7365 6373 3220 3d20 666f        secs2 = fo
-00000d60: 7572 7468 325b 325d 2e73 706c 6974 2822  urth2[2].split("
-00000d70: 2e22 295b 305d 0a20 2020 2020 2020 2069  .")[0].        i
-00000d80: 6620 272b 2720 696e 2073 6563 7332 3a0a  f '+' in secs2:.
-00000d90: 2020 2020 2020 2020 2020 2020 7365 6373              secs
-00000da0: 3220 3d20 7365 6373 322e 7370 6c69 7428  2 = secs2.split(
-00000db0: 272b 2729 5b30 5d0a 2020 2020 2020 2020  '+')[0].        
-00000dc0: 7365 6373 5f69 6e74 3220 3d20 696e 7428  secs_int2 = int(
-00000dd0: 7365 6373 3229 0a20 2020 2020 2020 2079  secs2).        y
-00000de0: 6561 725f 696e 5f64 6179 7332 203d 2069  ear_in_days2 = i
-00000df0: 6e74 2869 3229 202a 2033 3635 0a20 2020  nt(i2) * 365.   
-00000e00: 2020 2020 2079 6561 7273 3220 3d20 696e       years2 = in
-00000e10: 7428 7965 6172 5f69 6e5f 6461 7973 3229  t(year_in_days2)
-00000e20: 0a20 2020 2020 2020 206d 6f6e 7468 7332  .        months2
-00000e30: 203d 2069 6e74 286a 3229 202a 2033 300a   = int(j2) * 30.
-00000e40: 2020 2020 2020 2020 6461 7973 3220 3d20          days2 = 
-00000e50: 696e 7428 6b32 290a 0a20 2020 2020 2020  int(k2)..       
-00000e60: 2069 6620 7365 6c66 2e74 696d 655f 203d   if self.time_ =
-00000e70: 3d20 276d 2720 6f72 2073 656c 662e 7469  = 'm' or self.ti
-00000e80: 6d65 5f20 3d3d 2027 4d27 3a0a 2020 2020  me_ == 'M':.    
-00000e90: 2020 2020 2020 2020 6765 745f 6461 7973          get_days
-00000ea0: 5f6d 696e 7320 3d20 2868 7273 202a 2036  _mins = (hrs * 6
-00000eb0: 3029 202b 206d 696e 730a 2020 2020 2020  0) + mins.      
-00000ec0: 2020 2020 2020 6765 745f 7965 6172 735f        get_years_
-00000ed0: 6d69 6e73 203d 2028 7965 6172 7320 2b20  mins = (years + 
-00000ee0: 6d6f 6e74 6873 202b 2064 6179 7329 202a  months + days) *
-00000ef0: 2032 3420 2a20 3630 0a20 2020 2020 2020   24 * 60.       
-00000f00: 2020 2020 2067 6574 5f64 6179 735f 6d69       get_days_mi
-00000f10: 6e73 3220 3d20 2868 7273 3220 2a20 3630  ns2 = (hrs2 * 60
-00000f20: 2920 2b20 6d69 6e73 320a 2020 2020 2020  ) + mins2.      
-00000f30: 2020 2020 2020 6765 745f 7965 6172 735f        get_years_
-00000f40: 6d69 6e73 3220 3d20 2879 6561 7273 3220  mins2 = (years2 
-00000f50: 2b20 6d6f 6e74 6873 3220 2b20 6461 7973  + months2 + days
-00000f60: 3229 202a 2032 3420 2a20 3630 0a20 2020  2) * 24 * 60.   
-00000f70: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00000f80: 2867 6574 5f79 6561 7273 5f6d 696e 7320  (get_years_mins 
-00000f90: 2b20 6765 745f 6461 7973 5f6d 696e 7329  + get_days_mins)
-00000fa0: 202d 2028 6765 745f 7965 6172 735f 6d69   - (get_years_mi
-00000fb0: 6e73 3220 2b20 6765 745f 6461 7973 5f6d  ns2 + get_days_m
-00000fc0: 696e 7332 290a 2020 2020 2020 2020 656c  ins2).        el
-00000fd0: 6966 2073 656c 662e 7469 6d65 5f20 3d3d  if self.time_ ==
-00000fe0: 2027 6827 206f 7220 7365 6c66 2e74 696d   'h' or self.tim
-00000ff0: 655f 203d 3d20 2748 273a 0a20 2020 2020  e_ == 'H':.     
-00001000: 2020 2020 2020 2067 6574 5f64 6179 735f         get_days_
-00001010: 6d69 6e73 203d 2028 6872 7320 2a20 3630  mins = (hrs * 60
-00001020: 2920 2b20 6d69 6e73 0a20 2020 2020 2020  ) + mins.       
-00001030: 2020 2020 2067 6574 5f79 6561 7273 5f6d       get_years_m
-00001040: 696e 7320 3d20 2879 6561 7273 202b 206d  ins = (years + m
-00001050: 6f6e 7468 7320 2b20 6461 7973 2920 2a20  onths + days) * 
-00001060: 3234 202a 2036 300a 2020 2020 2020 2020  24 * 60.        
-00001070: 2020 2020 6765 745f 6461 7973 5f6d 696e      get_days_min
-00001080: 7332 203d 2028 6872 7332 202a 2036 3029  s2 = (hrs2 * 60)
-00001090: 202b 206d 696e 7332 0a20 2020 2020 2020   + mins2.       
-000010a0: 2020 2020 2067 6574 5f79 6561 7273 5f6d       get_years_m
-000010b0: 696e 7332 203d 2028 7965 6172 7332 202b  ins2 = (years2 +
-000010c0: 206d 6f6e 7468 7332 202b 2064 6179 7332   months2 + days2
-000010d0: 2920 2a20 3234 202a 2036 300a 2020 2020  ) * 24 * 60.    
-000010e0: 2020 2020 2020 2020 7265 7475 726e 2072          return r
-000010f0: 6f75 6e64 2828 6765 745f 7965 6172 735f  ound((get_years_
-00001100: 6d69 6e73 202b 2067 6574 5f64 6179 735f  mins + get_days_
-00001110: 6d69 6e73 2920 2d20 2867 6574 5f79 6561  mins) - (get_yea
-00001120: 7273 5f6d 696e 7332 202b 2067 6574 5f64  rs_mins2 + get_d
-00001130: 6179 735f 6d69 6e73 3229 202f 2036 302c  ays_mins2) / 60,
-00001140: 2032 290a 2020 2020 2020 2020 656c 6966   2).        elif
-00001150: 2073 656c 662e 7469 6d65 5f20 3d3d 2027   self.time_ == '
-00001160: 6427 206f 7220 7365 6c66 2e74 696d 655f  d' or self.time_
-00001170: 203d 3d20 2744 273a 0a20 2020 2020 2020   == 'D':.       
-00001180: 2020 2020 2067 6574 5f64 6179 7320 3d20       get_days = 
-00001190: 7965 6172 7320 2b20 6d6f 6e74 6873 202b  years + months +
-000011a0: 2064 6179 730a 2020 2020 2020 2020 2020   days.          
-000011b0: 2020 6765 745f 6461 7973 3220 3d20 7965    get_days2 = ye
-000011c0: 6172 7332 202b 206d 6f6e 7468 7332 202b  ars2 + months2 +
-000011d0: 2064 6179 7332 0a20 2020 2020 2020 2020   days2.         
-000011e0: 2020 2072 6574 7572 6e20 6765 745f 6461     return get_da
-000011f0: 7973 202d 2067 6574 5f64 6179 7332 0a20  ys - get_days2. 
-00001200: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-00001210: 2020 2020 2020 2020 2067 6574 5f64 6179           get_day
-00001220: 735f 7365 6373 203d 2028 6872 7320 2a20  s_secs = (hrs * 
-00001230: 3630 202a 2036 3029 202b 2028 6d69 6e73  60 * 60) + (mins
-00001240: 202a 2036 3029 202b 2073 6563 735f 696e   * 60) + secs_in
-00001250: 740a 2020 2020 2020 2020 2020 2020 6765  t.            ge
-00001260: 745f 7965 6172 735f 7365 6373 203d 2028  t_years_secs = (
-00001270: 7965 6172 7320 2b20 6d6f 6e74 6873 202b  years + months +
-00001280: 2064 6179 7329 202a 2032 3420 2a20 3630   days) * 24 * 60
-00001290: 202a 2036 300a 2020 2020 2020 2020 2020   * 60.          
-000012a0: 2020 6765 745f 6461 7973 5f73 6563 7332    get_days_secs2
-000012b0: 203d 2028 6872 7332 202a 2036 3020 2a20   = (hrs2 * 60 * 
-000012c0: 3630 2920 2b20 286d 696e 7332 202a 2036  60) + (mins2 * 6
-000012d0: 3029 202b 2073 6563 735f 696e 7432 0a20  0) + secs_int2. 
-000012e0: 2020 2020 2020 2020 2020 2067 6574 5f79             get_y
-000012f0: 6561 7273 5f73 6563 7332 203d 2028 7965  ears_secs2 = (ye
-00001300: 6172 7332 202b 206d 6f6e 7468 7332 202b  ars2 + months2 +
-00001310: 2064 6179 7332 2920 2a20 3234 202a 2036   days2) * 24 * 6
-00001320: 3020 2a20 3630 0a20 2020 2020 2020 2020  0 * 60.         
-00001330: 2020 2072 6574 7572 6e20 2867 6574 5f79     return (get_y
-00001340: 6561 7273 5f73 6563 7320 2b20 6765 745f  ears_secs + get_
-00001350: 6461 7973 5f73 6563 7329 202d 2028 6765  days_secs) - (ge
-00001360: 745f 6461 7973 5f73 6563 7332 202b 2067  t_days_secs2 + g
-00001370: 6574 5f79 6561 7273 5f73 6563 7332 290a  et_years_secs2).
-00001380: 0a20 2020 2040 7072 6f70 6572 7479 0a20  .    @property. 
-00001390: 2020 2064 6566 2064 6174 655f 6469 6666     def date_diff
-000013a0: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-000013b0: 2320 7469 6d65 2031 0a20 2020 2020 2020  # time 1.       
-000013c0: 2073 6c75 675f 7469 6d65 203d 2073 7472   slug_time = str
-000013d0: 2873 656c 662e 7469 6d65 3129 0a20 2020  (self.time1).   
-000013e0: 2020 2020 2066 6972 7374 203d 2073 6c75       first = slu
-000013f0: 675f 7469 6d65 2e73 706c 6974 2822 2d22  g_time.split("-"
-00001400: 290a 2020 2020 2020 2020 7365 636f 6e64  ).        second
-00001410: 203d 2066 6972 7374 5b30 3a32 5d0a 2020   = first[0:2].  
-00001420: 2020 2020 2020 7468 6972 6420 3d20 6669        third = fi
-00001430: 7273 745b 325d 0a20 2020 2020 2020 2069  rst[2].        i
-00001440: 203d 2073 6563 6f6e 645b 305d 0a20 2020   = second[0].   
-00001450: 2020 2020 206a 203d 2073 6563 6f6e 645b       j = second[
-00001460: 315d 0a20 2020 2020 2020 206b 203d 2074  1].        k = t
-00001470: 6869 7264 2e73 706c 6974 2822 2022 295b  hird.split(" ")[
-00001480: 305d 0a20 2020 2020 2020 2079 6561 725f  0].        year_
-00001490: 696e 5f64 6179 7320 3d20 696e 7428 6929  in_days = int(i)
-000014a0: 202a 2033 3635 0a20 2020 2020 2020 2079   * 365.        y
-000014b0: 6561 7273 203d 2069 6e74 2879 6561 725f  ears = int(year_
-000014c0: 696e 5f64 6179 7329 0a20 2020 2020 2020  in_days).       
-000014d0: 206d 6f6e 7468 7320 3d20 696e 7428 6a29   months = int(j)
-000014e0: 202a 2033 300a 2020 2020 2020 2020 6461   * 30.        da
-000014f0: 7973 203d 2069 6e74 286b 290a 0a20 2020  ys = int(k)..   
-00001500: 2020 2020 2023 2074 696d 6520 320a 2020       # time 2.  
-00001510: 2020 2020 2020 736c 7567 5f74 696d 6520        slug_time 
-00001520: 3d20 7374 7228 7365 6c66 2e74 696d 6532  = str(self.time2
-00001530: 290a 2020 2020 2020 2020 6669 7273 7432  ).        first2
-00001540: 203d 2073 6c75 675f 7469 6d65 2e73 706c   = slug_time.spl
-00001550: 6974 2822 2d22 290a 2020 2020 2020 2020  it("-").        
-00001560: 7365 636f 6e64 3220 3d20 6669 7273 7432  second2 = first2
-00001570: 5b30 3a32 5d0a 2020 2020 2020 2020 7468  [0:2].        th
-00001580: 6972 6432 203d 2066 6972 7374 325b 325d  ird2 = first2[2]
-00001590: 0a20 2020 2020 2020 2069 3220 3d20 7365  .        i2 = se
-000015a0: 636f 6e64 325b 305d 0a20 2020 2020 2020  cond2[0].       
-000015b0: 206a 3220 3d20 7365 636f 6e64 325b 315d   j2 = second2[1]
-000015c0: 0a20 2020 2020 2020 206b 3220 3d20 7468  .        k2 = th
-000015d0: 6972 6432 2e73 706c 6974 2822 2022 295b  ird2.split(" ")[
-000015e0: 305d 0a20 2020 2020 2020 2079 6561 725f  0].        year_
-000015f0: 696e 5f64 6179 7332 203d 2069 6e74 2869  in_days2 = int(i
-00001600: 3229 202a 2033 3635 0a20 2020 2020 2020  2) * 365.       
-00001610: 2079 6561 7273 3220 3d20 696e 7428 7965   years2 = int(ye
-00001620: 6172 5f69 6e5f 6461 7973 290a 2020 2020  ar_in_days).    
-00001630: 2020 2020 6d6f 6e74 6873 3220 3d20 696e      months2 = in
-00001640: 7428 6a32 2920 2a20 3330 0a20 2020 2020  t(j2) * 30.     
-00001650: 2020 2064 6179 7332 203d 2069 6e74 286b     days2 = int(k
-00001660: 3229 0a0a 2020 2020 2020 2020 6966 2073  2)..        if s
-00001670: 656c 662e 7469 6d65 5f20 3d3d 2027 6d27  elf.time_ == 'm'
-00001680: 206f 7220 7365 6c66 2e74 696d 655f 203d   or self.time_ =
-00001690: 3d20 276d 273a 0a20 2020 2020 2020 2020  = 'm':.         
-000016a0: 2020 2067 6574 5f6d 696e 7320 3d20 2879     get_mins = (y
-000016b0: 6561 7273 202b 206d 6f6e 7468 7320 2b20  ears + months + 
-000016c0: 6461 7973 2920 2a20 3234 202a 2036 300a  days) * 24 * 60.
-000016d0: 2020 2020 2020 2020 2020 2020 6765 745f              get_
-000016e0: 6d69 6e73 3220 3d20 2879 6561 7273 3220  mins2 = (years2 
-000016f0: 2b20 6d6f 6e74 6873 3220 2b20 6461 7973  + months2 + days
-00001700: 3229 202a 2032 3420 2a20 3630 0a20 2020  2) * 24 * 60.   
-00001710: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00001720: 6765 745f 6d69 6e73 202d 2067 6574 5f6d  get_mins - get_m
-00001730: 696e 7332 0a20 2020 2020 2020 2065 6c69  ins2.        eli
-00001740: 6620 7365 6c66 2e74 696d 655f 203d 3d20  f self.time_ == 
-00001750: 2768 2720 6f72 2073 656c 662e 7469 6d65  'h' or self.time
-00001760: 5f20 3d3d 2027 4827 3a0a 2020 2020 2020  _ == 'H':.      
-00001770: 2020 2020 2020 6765 745f 6d69 6e73 203d        get_mins =
-00001780: 2028 7965 6172 7320 2b20 6d6f 6e74 6873   (years + months
-00001790: 202b 2064 6179 7329 202a 2032 3420 2a20   + days) * 24 * 
-000017a0: 3630 0a20 2020 2020 2020 2020 2020 2067  60.            g
-000017b0: 6574 5f6d 696e 7332 203d 2028 7965 6172  et_mins2 = (year
-000017c0: 7332 202b 206d 6f6e 7468 7332 202b 2064  s2 + months2 + d
-000017d0: 6179 7332 2920 2a20 3234 202a 2036 300a  ays2) * 24 * 60.
-000017e0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-000017f0: 726e 2072 6f75 6e64 2828 6765 745f 6d69  rn round((get_mi
-00001800: 6e73 202d 2067 6574 5f6d 696e 7332 2920  ns - get_mins2) 
-00001810: 2f20 3630 2c20 3229 0a20 2020 2020 2020  / 60, 2).       
-00001820: 2065 6c69 6620 7365 6c66 2e74 696d 655f   elif self.time_
-00001830: 203d 3d20 2764 2720 6f72 2073 656c 662e   == 'd' or self.
-00001840: 7469 6d65 5f20 3d3d 2027 4427 3a0a 2020  time_ == 'D':.  
-00001850: 2020 2020 2020 2020 2020 6765 745f 6461            get_da
-00001860: 7973 203d 2079 6561 7273 202b 206d 6f6e  ys = years + mon
-00001870: 7468 7320 2b20 6461 7973 0a20 2020 2020  ths + days.     
-00001880: 2020 2020 2020 2067 6574 5f64 6179 7332         get_days2
-00001890: 203d 2079 6561 7273 3220 2b20 6d6f 6e74   = years2 + mont
-000018a0: 6873 3220 2b20 6461 7973 320a 2020 2020  hs2 + days2.    
-000018b0: 2020 2020 2020 2020 7265 7475 726e 2067          return g
-000018c0: 6574 5f64 6179 7320 2d20 6765 745f 6461  et_days - get_da
-000018d0: 7973 320a 2020 2020 2020 2020 656c 7365  ys2.        else
-000018e0: 3a0a 2020 2020 2020 2020 2020 2020 6765  :.            ge
-000018f0: 745f 7365 6373 203d 2028 7965 6172 7320  t_secs = (years 
-00001900: 2b20 6d6f 6e74 6873 202b 2064 6179 7329  + months + days)
-00001910: 202a 2032 3420 2a20 3630 202a 2036 300a   * 24 * 60 * 60.
-00001920: 2020 2020 2020 2020 2020 2020 6765 745f              get_
-00001930: 7365 6373 3220 3d20 2879 6561 7273 3220  secs2 = (years2 
-00001940: 2b20 6d6f 6e74 6873 3220 2b20 6461 7973  + months2 + days
-00001950: 3229 202a 2032 3420 2a20 3630 202a 2036  2) * 24 * 60 * 6
-00001960: 300a 2020 2020 2020 2020 2020 2020 7265  0.            re
-00001970: 7475 726e 2067 6574 5f73 6563 7320 2d20  turn get_secs - 
-00001980: 6765 745f 7365 6373 320a 0a              get_secs2..
+00000000: 0d0a 636c 6173 7320 436f 6e76 6572 7454  ..class ConvertT
+00000010: 696d 653a 0d0a 2020 2020 6465 6620 5f5f  ime:..    def __
+00000020: 696e 6974 5f5f 2873 656c 662c 2074 696d  init__(self, tim
+00000030: 652c 2074 696d 655f 666f 726d 6174 3d27  e, time_format='
+00000040: 7327 293a 0d0a 2020 2020 2020 2020 7365  s'):..        se
+00000050: 6c66 2e74 696d 6520 3d20 7469 6d65 0d0a  lf.time = time..
+00000060: 2020 2020 2020 2020 7365 6c66 2e74 696d          self.tim
+00000070: 655f 3a20 7374 7220 3d20 7469 6d65 5f66  e_: str = time_f
+00000080: 6f72 6d61 740d 0a0d 0a20 2020 2040 7072  ormat....    @pr
+00000090: 6f70 6572 7479 0d0a 2020 2020 6465 6620  operty..    def 
+000000a0: 736c 7567 5f64 6174 655f 7469 6d65 2873  slug_date_time(s
+000000b0: 656c 6629 3a0d 0a20 2020 2020 2020 2073  elf):..        s
+000000c0: 6c75 675f 7469 6d65 203d 2073 7472 2873  lug_time = str(s
+000000d0: 656c 662e 7469 6d65 290d 0a20 2020 2020  elf.time)..     
+000000e0: 2020 2066 6972 7374 203d 2073 6c75 675f     first = slug_
+000000f0: 7469 6d65 2e73 706c 6974 2822 2d22 290d  time.split("-").
+00000100: 0a20 2020 2020 2020 2073 6563 6f6e 6420  .        second 
+00000110: 3d20 6669 7273 745b 303a 325d 0d0a 2020  = first[0:2]..  
+00000120: 2020 2020 2020 7468 6972 6420 3d20 6669        third = fi
+00000130: 7273 745b 325d 0d0a 2020 2020 2020 2020  rst[2]..        
+00000140: 666f 7572 7468 203d 2074 6869 7264 2e73  fourth = third.s
+00000150: 706c 6974 2822 2022 295b 315d 2e73 706c  plit(" ")[1].spl
+00000160: 6974 2822 3a22 290d 0a20 2020 2020 2020  it(":")..       
+00000170: 2069 203d 2073 6563 6f6e 645b 305d 0d0a   i = second[0]..
+00000180: 2020 2020 2020 2020 6a20 3d20 7365 636f          j = seco
+00000190: 6e64 5b31 5d0d 0a20 2020 2020 2020 206b  nd[1]..        k
+000001a0: 203d 2074 6869 7264 2e73 706c 6974 2822   = third.split("
+000001b0: 2022 295b 305d 0d0a 2020 2020 2020 2020   ")[0]..        
+000001c0: 6872 7320 3d20 696e 7428 666f 7572 7468  hrs = int(fourth
+000001d0: 5b30 5d29 0d0a 2020 2020 2020 2020 6d69  [0])..        mi
+000001e0: 6e73 203d 2069 6e74 2866 6f75 7274 685b  ns = int(fourth[
+000001f0: 315d 290d 0a20 2020 2020 2020 2073 6563  1])..        sec
+00000200: 7320 3d20 666f 7572 7468 5b32 5d2e 7370  s = fourth[2].sp
+00000210: 6c69 7428 222e 2229 5b30 5d0d 0a20 2020  lit(".")[0]..   
+00000220: 2020 2020 2069 6620 272b 2720 696e 2073       if '+' in s
+00000230: 6563 733a 0d0a 2020 2020 2020 2020 2020  ecs:..          
+00000240: 2020 7365 6373 203d 2073 6563 732e 7370    secs = secs.sp
+00000250: 6c69 7428 272b 2729 5b30 5d0d 0a20 2020  lit('+')[0]..   
+00000260: 2020 2020 2073 6563 735f 696e 7420 3d20       secs_int = 
+00000270: 696e 7428 7365 6373 290d 0a20 2020 2020  int(secs)..     
+00000280: 2020 2079 6561 725f 696e 5f64 6179 7320     year_in_days 
+00000290: 3d20 696e 7428 6929 202a 2033 3635 0d0a  = int(i) * 365..
+000002a0: 2020 2020 2020 2020 7965 6172 7320 3d20          years = 
+000002b0: 696e 7428 7965 6172 5f69 6e5f 6461 7973  int(year_in_days
+000002c0: 290d 0a20 2020 2020 2020 206d 6f6e 7468  )..        month
+000002d0: 7320 3d20 696e 7428 6a29 202a 2033 300d  s = int(j) * 30.
+000002e0: 0a20 2020 2020 2020 2064 6179 7320 3d20  .        days = 
+000002f0: 696e 7428 6b29 0d0a 2020 2020 2020 2020  int(k)..        
+00000300: 6966 2073 656c 662e 7469 6d65 5f20 3d3d  if self.time_ ==
+00000310: 2027 6d27 3a0d 0a20 2020 2020 2020 2020   'm':..         
+00000320: 2020 2067 6574 5f64 6179 735f 6d69 6e73     get_days_mins
+00000330: 203d 2028 6872 7320 2a20 3630 2920 2b20   = (hrs * 60) + 
+00000340: 6d69 6e73 0d0a 2020 2020 2020 2020 2020  mins..          
+00000350: 2020 6765 745f 7965 6172 735f 6d69 6e73    get_years_mins
+00000360: 203d 2028 7965 6172 7320 2b20 6d6f 6e74   = (years + mont
+00000370: 6873 202b 2064 6179 7329 202a 2032 3420  hs + days) * 24 
+00000380: 2a20 3630 0d0a 2020 2020 2020 2020 2020  * 60..          
+00000390: 2020 7265 7475 726e 2067 6574 5f79 6561    return get_yea
+000003a0: 7273 5f6d 696e 7320 2b20 6765 745f 6461  rs_mins + get_da
+000003b0: 7973 5f6d 696e 730d 0a20 2020 2020 2020  ys_mins..       
+000003c0: 2065 6c69 6620 7365 6c66 2e74 696d 655f   elif self.time_
+000003d0: 203d 3d20 2768 273a 0d0a 2020 2020 2020   == 'h':..      
+000003e0: 2020 2020 2020 6765 745f 6461 7973 5f6d        get_days_m
+000003f0: 696e 7320 3d20 2868 7273 202a 2036 3029  ins = (hrs * 60)
+00000400: 202b 206d 696e 730d 0a20 2020 2020 2020   + mins..       
+00000410: 2020 2020 2067 6574 5f79 6561 7273 5f6d       get_years_m
+00000420: 696e 7320 3d20 2879 6561 7273 202b 206d  ins = (years + m
+00000430: 6f6e 7468 7320 2b20 6461 7973 2920 2a20  onths + days) * 
+00000440: 3234 202a 2036 300d 0a20 2020 2020 2020  24 * 60..       
+00000450: 2020 2020 2072 6574 7572 6e20 726f 756e       return roun
+00000460: 6428 2867 6574 5f79 6561 7273 5f6d 696e  d((get_years_min
+00000470: 7320 2b20 6765 745f 6461 7973 5f6d 696e  s + get_days_min
+00000480: 7329 202f 2036 302c 2032 290d 0a20 2020  s) / 60, 2)..   
+00000490: 2020 2020 2065 6c69 6620 7365 6c66 2e74       elif self.t
+000004a0: 696d 655f 203d 3d20 2764 273a 0d0a 2020  ime_ == 'd':..  
+000004b0: 2020 2020 2020 2020 2020 6765 745f 7965            get_ye
+000004c0: 6172 735f 6461 7973 203d 2079 6561 7273  ars_days = years
+000004d0: 202b 206d 6f6e 7468 7320 2b20 6461 7973   + months + days
+000004e0: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
+000004f0: 7475 726e 2067 6574 5f79 6561 7273 5f64  turn get_years_d
+00000500: 6179 730d 0a20 2020 2020 2020 2065 6c73  ays..        els
+00000510: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+00000520: 6765 745f 6461 7973 5f73 6563 7320 3d20  get_days_secs = 
+00000530: 2868 7273 202a 2036 3020 2a20 3630 2920  (hrs * 60 * 60) 
+00000540: 2b20 286d 696e 7320 2a20 3630 2920 2b20  + (mins * 60) + 
+00000550: 7365 6373 5f69 6e74 0d0a 2020 2020 2020  secs_int..      
+00000560: 2020 2020 2020 6765 745f 7965 6172 735f        get_years_
+00000570: 7365 6373 203d 2028 7965 6172 7320 2b20  secs = (years + 
+00000580: 6d6f 6e74 6873 202b 2064 6179 7329 202a  months + days) *
+00000590: 2032 3420 2a20 3630 202a 2036 300d 0a20   24 * 60 * 60.. 
+000005a0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+000005b0: 6e20 6765 745f 7965 6172 735f 7365 6373  n get_years_secs
+000005c0: 202b 2067 6574 5f64 6179 735f 7365 6373   + get_days_secs
+000005d0: 0d0a 0d0a 2020 2020 4070 726f 7065 7274  ....    @propert
+000005e0: 790d 0a20 2020 2064 6566 2073 6c75 675f  y..    def slug_
+000005f0: 6461 7465 2873 656c 6629 3a0d 0a20 2020  date(self):..   
+00000600: 2020 2020 2073 6c75 675f 7469 6d65 3a20       slug_time: 
+00000610: 7374 7220 3d20 7374 7228 7365 6c66 2e74  str = str(self.t
+00000620: 696d 6529 0d0a 2020 2020 2020 2020 6669  ime)..        fi
+00000630: 7273 7420 3d20 736c 7567 5f74 696d 652e  rst = slug_time.
+00000640: 7370 6c69 7428 222d 2229 0d0a 2020 2020  split("-")..    
+00000650: 2020 2020 7365 636f 6e64 203d 2066 6972      second = fir
+00000660: 7374 5b30 3a32 5d0d 0a20 2020 2020 2020  st[0:2]..       
+00000670: 2074 6869 7264 203d 2066 6972 7374 5b32   third = first[2
+00000680: 5d0d 0a20 2020 2020 2020 2069 203d 2073  ]..        i = s
+00000690: 6563 6f6e 645b 305d 0d0a 2020 2020 2020  econd[0]..      
+000006a0: 2020 6a20 3d20 7365 636f 6e64 5b31 5d0d    j = second[1].
+000006b0: 0a20 2020 2020 2020 206b 203d 2074 6869  .        k = thi
+000006c0: 7264 2e73 706c 6974 2822 2022 295b 305d  rd.split(" ")[0]
+000006d0: 0d0a 2020 2020 2020 2020 7965 6172 5f69  ..        year_i
+000006e0: 6e5f 6461 7973 203d 2069 6e74 2869 2920  n_days = int(i) 
+000006f0: 2a20 3336 350d 0a20 2020 2020 2020 2079  * 365..        y
+00000700: 6561 7273 203d 2069 6e74 2879 6561 725f  ears = int(year_
+00000710: 696e 5f64 6179 7329 0d0a 2020 2020 2020  in_days)..      
+00000720: 2020 6d6f 6e74 6873 203d 2069 6e74 286a    months = int(j
+00000730: 2920 2a20 3330 0d0a 2020 2020 2020 2020  ) * 30..        
+00000740: 6461 7973 203d 2069 6e74 286b 290d 0a20  days = int(k).. 
+00000750: 2020 2020 2020 2069 6620 7365 6c66 2e74         if self.t
+00000760: 696d 655f 203d 3d20 276d 273a 0d0a 2020  ime_ == 'm':..  
+00000770: 2020 2020 2020 2020 2020 6765 745f 6d69            get_mi
+00000780: 6e73 203d 2028 7965 6172 7320 2b20 6d6f  ns = (years + mo
+00000790: 6e74 6873 202b 2064 6179 7329 202a 2032  nths + days) * 2
+000007a0: 3420 2a20 3630 0d0a 2020 2020 2020 2020  4 * 60..        
+000007b0: 2020 2020 7265 7475 726e 2067 6574 5f6d      return get_m
+000007c0: 696e 730d 0a20 2020 2020 2020 2065 6c69  ins..        eli
+000007d0: 6620 7365 6c66 2e74 696d 655f 203d 3d20  f self.time_ == 
+000007e0: 2768 273a 0d0a 2020 2020 2020 2020 2020  'h':..          
+000007f0: 2020 6765 745f 6872 7320 3d20 726f 756e    get_hrs = roun
+00000800: 6428 2828 7965 6172 7320 2b20 6d6f 6e74  d(((years + mont
+00000810: 6873 202b 2064 6179 7329 202a 2032 3420  hs + days) * 24 
+00000820: 2a20 3630 2920 2f20 3630 2c20 3229 0d0a  * 60) / 60, 2)..
+00000830: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00000840: 726e 2067 6574 5f68 7273 0d0a 2020 2020  rn get_hrs..    
+00000850: 2020 2020 656c 6966 2073 656c 662e 7469      elif self.ti
+00000860: 6d65 5f20 3d3d 2027 6427 3a0d 0a20 2020  me_ == 'd':..   
+00000870: 2020 2020 2020 2020 2067 6574 5f64 6179           get_day
+00000880: 7320 3d20 7965 6172 7320 2b20 6d6f 6e74  s = years + mont
+00000890: 6873 202b 2064 6179 730d 0a20 2020 2020  hs + days..     
+000008a0: 2020 2020 2020 2072 6574 7572 6e20 6765         return ge
+000008b0: 745f 6461 7973 0d0a 2020 2020 2020 2020  t_days..        
+000008c0: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
+000008d0: 2020 2067 6574 5f73 6563 7320 3d20 2879     get_secs = (y
+000008e0: 6561 7273 202b 206d 6f6e 7468 7320 2b20  ears + months + 
+000008f0: 6461 7973 2920 2a20 3234 202a 2036 3020  days) * 24 * 60 
+00000900: 2a20 3630 0d0a 2020 2020 2020 2020 2020  * 60..          
+00000910: 2020 7265 7475 726e 2067 6574 5f73 6563    return get_sec
+00000920: 730d 0a0d 0a0d 0a63 6c61 7373 2044 6174  s......class Dat
+00000930: 6544 6966 663a 0d0a 2020 2020 6465 6620  eDiff:..    def 
+00000940: 5f5f 696e 6974 5f5f 2873 656c 662c 2074  __init__(self, t
+00000950: 696d 6531 2c20 7469 6d65 322c 2074 696d  ime1, time2, tim
+00000960: 655f 666f 726d 6174 3d27 7327 293a 0d0a  e_format='s'):..
+00000970: 2020 2020 2020 2020 7365 6c66 2e74 696d          self.tim
+00000980: 6531 203d 2074 696d 6531 0d0a 2020 2020  e1 = time1..    
+00000990: 2020 2020 7365 6c66 2e74 696d 6532 203d      self.time2 =
+000009a0: 2074 696d 6532 0d0a 2020 2020 2020 2020   time2..        
+000009b0: 7365 6c66 2e74 696d 655f 3a20 7374 7220  self.time_: str 
+000009c0: 3d20 7469 6d65 5f66 6f72 6d61 740d 0a0d  = time_format...
+000009d0: 0a20 2020 2040 7072 6f70 6572 7479 0d0a  .    @property..
+000009e0: 2020 2020 6465 6620 6461 7465 5f74 696d      def date_tim
+000009f0: 655f 6469 6666 2873 656c 6629 3a0d 0a20  e_diff(self):.. 
+00000a00: 2020 2020 2020 2023 2074 696d 6520 310d         # time 1.
+00000a10: 0a20 2020 2020 2020 2073 6c75 675f 7469  .        slug_ti
+00000a20: 6d65 3120 3d20 7374 7228 7365 6c66 2e74  me1 = str(self.t
+00000a30: 696d 6531 290d 0a20 2020 2020 2020 2066  ime1)..        f
+00000a40: 6972 7374 203d 2073 6c75 675f 7469 6d65  irst = slug_time
+00000a50: 312e 7370 6c69 7428 222d 2229 0d0a 2020  1.split("-")..  
+00000a60: 2020 2020 2020 7365 636f 6e64 203d 2066        second = f
+00000a70: 6972 7374 5b30 3a32 5d0d 0a20 2020 2020  irst[0:2]..     
+00000a80: 2020 2074 6869 7264 203d 2066 6972 7374     third = first
+00000a90: 5b32 5d0d 0a20 2020 2020 2020 2066 6f75  [2]..        fou
+00000aa0: 7274 6820 3d20 7468 6972 642e 7370 6c69  rth = third.spli
+00000ab0: 7428 2220 2229 5b31 5d2e 7370 6c69 7428  t(" ")[1].split(
+00000ac0: 223a 2229 0d0a 2020 2020 2020 2020 6920  ":")..        i 
+00000ad0: 3d20 7365 636f 6e64 5b30 5d0d 0a20 2020  = second[0]..   
+00000ae0: 2020 2020 206a 203d 2073 6563 6f6e 645b       j = second[
+00000af0: 315d 0d0a 2020 2020 2020 2020 6b20 3d20  1]..        k = 
+00000b00: 7468 6972 642e 7370 6c69 7428 2220 2229  third.split(" ")
+00000b10: 5b30 5d0d 0a20 2020 2020 2020 2068 7273  [0]..        hrs
+00000b20: 203d 2069 6e74 2866 6f75 7274 685b 305d   = int(fourth[0]
+00000b30: 290d 0a20 2020 2020 2020 206d 696e 7320  )..        mins 
+00000b40: 3d20 696e 7428 666f 7572 7468 5b31 5d29  = int(fourth[1])
+00000b50: 0d0a 2020 2020 2020 2020 7365 6373 203d  ..        secs =
+00000b60: 2066 6f75 7274 685b 325d 2e73 706c 6974   fourth[2].split
+00000b70: 2822 2e22 295b 305d 0d0a 2020 2020 2020  (".")[0]..      
+00000b80: 2020 6966 2027 2b27 2069 6e20 7365 6373    if '+' in secs
+00000b90: 3a0d 0a20 2020 2020 2020 2020 2020 2073  :..            s
+00000ba0: 6563 7320 3d20 7365 6373 2e73 706c 6974  ecs = secs.split
+00000bb0: 2827 2b27 295b 305d 0d0a 2020 2020 2020  ('+')[0]..      
+00000bc0: 2020 7365 6373 5f69 6e74 203d 2069 6e74    secs_int = int
+00000bd0: 2873 6563 7329 0d0a 2020 2020 2020 2020  (secs)..        
+00000be0: 7965 6172 5f69 6e5f 6461 7973 203d 2069  year_in_days = i
+00000bf0: 6e74 2869 2920 2a20 3336 350d 0a20 2020  nt(i) * 365..   
+00000c00: 2020 2020 2079 6561 7273 203d 2069 6e74       years = int
+00000c10: 2879 6561 725f 696e 5f64 6179 7329 0d0a  (year_in_days)..
+00000c20: 2020 2020 2020 2020 6d6f 6e74 6873 203d          months =
+00000c30: 2069 6e74 286a 2920 2a20 3330 0d0a 2020   int(j) * 30..  
+00000c40: 2020 2020 2020 6461 7973 203d 2069 6e74        days = int
+00000c50: 286b 290d 0a0d 0a20 2020 2020 2020 2023  (k)....        #
+00000c60: 2074 696d 6532 0d0a 2020 2020 2020 2020   time2..        
+00000c70: 736c 7567 5f74 696d 6532 203d 2073 7472  slug_time2 = str
+00000c80: 2873 656c 662e 7469 6d65 3229 0d0a 2020  (self.time2)..  
+00000c90: 2020 2020 2020 6669 7273 7432 203d 2073        first2 = s
+00000ca0: 6c75 675f 7469 6d65 322e 7370 6c69 7428  lug_time2.split(
+00000cb0: 222d 2229 0d0a 2020 2020 2020 2020 7365  "-")..        se
+00000cc0: 636f 6e64 3220 3d20 6669 7273 7432 5b30  cond2 = first2[0
+00000cd0: 3a32 5d0d 0a20 2020 2020 2020 2074 6869  :2]..        thi
+00000ce0: 7264 3220 3d20 6669 7273 7432 5b32 5d0d  rd2 = first2[2].
+00000cf0: 0a20 2020 2020 2020 2066 6f75 7274 6832  .        fourth2
+00000d00: 203d 2074 6869 7264 322e 7370 6c69 7428   = third2.split(
+00000d10: 2220 2229 5b31 5d2e 7370 6c69 7428 223a  " ")[1].split(":
+00000d20: 2229 0d0a 2020 2020 2020 2020 6932 203d  ")..        i2 =
+00000d30: 2073 6563 6f6e 6432 5b30 5d0d 0a20 2020   second2[0]..   
+00000d40: 2020 2020 206a 3220 3d20 7365 636f 6e64       j2 = second
+00000d50: 325b 315d 0d0a 2020 2020 2020 2020 6b32  2[1]..        k2
+00000d60: 203d 2074 6869 7264 322e 7370 6c69 7428   = third2.split(
+00000d70: 2220 2229 5b30 5d0d 0a20 2020 2020 2020  " ")[0]..       
+00000d80: 2068 7273 3220 3d20 696e 7428 666f 7572   hrs2 = int(four
+00000d90: 7468 325b 305d 290d 0a20 2020 2020 2020  th2[0])..       
+00000da0: 206d 696e 7332 203d 2069 6e74 2866 6f75   mins2 = int(fou
+00000db0: 7274 6832 5b31 5d29 0d0a 2020 2020 2020  rth2[1])..      
+00000dc0: 2020 7365 6373 3220 3d20 666f 7572 7468    secs2 = fourth
+00000dd0: 325b 325d 2e73 706c 6974 2822 2e22 295b  2[2].split(".")[
+00000de0: 305d 0d0a 2020 2020 2020 2020 6966 2027  0]..        if '
+00000df0: 2b27 2069 6e20 7365 6373 323a 0d0a 2020  +' in secs2:..  
+00000e00: 2020 2020 2020 2020 2020 7365 6373 3220            secs2 
+00000e10: 3d20 7365 6373 322e 7370 6c69 7428 272b  = secs2.split('+
+00000e20: 2729 5b30 5d0d 0a20 2020 2020 2020 2073  ')[0]..        s
+00000e30: 6563 735f 696e 7432 203d 2069 6e74 2873  ecs_int2 = int(s
+00000e40: 6563 7332 290d 0a20 2020 2020 2020 2079  ecs2)..        y
+00000e50: 6561 725f 696e 5f64 6179 7332 203d 2069  ear_in_days2 = i
+00000e60: 6e74 2869 3229 202a 2033 3635 0d0a 2020  nt(i2) * 365..  
+00000e70: 2020 2020 2020 7965 6172 7332 203d 2069        years2 = i
+00000e80: 6e74 2879 6561 725f 696e 5f64 6179 7332  nt(year_in_days2
+00000e90: 290d 0a20 2020 2020 2020 206d 6f6e 7468  )..        month
+00000ea0: 7332 203d 2069 6e74 286a 3229 202a 2033  s2 = int(j2) * 3
+00000eb0: 300d 0a20 2020 2020 2020 2064 6179 7332  0..        days2
+00000ec0: 203d 2069 6e74 286b 3229 0d0a 0d0a 2020   = int(k2)....  
+00000ed0: 2020 2020 2020 6966 2073 656c 662e 7469        if self.ti
+00000ee0: 6d65 5f20 3d3d 2027 6d27 206f 7220 7365  me_ == 'm' or se
+00000ef0: 6c66 2e74 696d 655f 203d 3d20 274d 273a  lf.time_ == 'M':
+00000f00: 0d0a 2020 2020 2020 2020 2020 2020 6765  ..            ge
+00000f10: 745f 6461 7973 5f6d 696e 7320 3d20 2868  t_days_mins = (h
+00000f20: 7273 202a 2036 3029 202b 206d 696e 730d  rs * 60) + mins.
+00000f30: 0a20 2020 2020 2020 2020 2020 2067 6574  .            get
+00000f40: 5f79 6561 7273 5f6d 696e 7320 3d20 2879  _years_mins = (y
+00000f50: 6561 7273 202b 206d 6f6e 7468 7320 2b20  ears + months + 
+00000f60: 6461 7973 2920 2a20 3234 202a 2036 300d  days) * 24 * 60.
+00000f70: 0a20 2020 2020 2020 2020 2020 2067 6574  .            get
+00000f80: 5f64 6179 735f 6d69 6e73 3220 3d20 2868  _days_mins2 = (h
+00000f90: 7273 3220 2a20 3630 2920 2b20 6d69 6e73  rs2 * 60) + mins
+00000fa0: 320d 0a20 2020 2020 2020 2020 2020 2067  2..            g
+00000fb0: 6574 5f79 6561 7273 5f6d 696e 7332 203d  et_years_mins2 =
+00000fc0: 2028 7965 6172 7332 202b 206d 6f6e 7468   (years2 + month
+00000fd0: 7332 202b 2064 6179 7332 2920 2a20 3234  s2 + days2) * 24
+00000fe0: 202a 2036 300d 0a20 2020 2020 2020 2020   * 60..         
+00000ff0: 2020 2072 6574 7572 6e20 2867 6574 5f79     return (get_y
+00001000: 6561 7273 5f6d 696e 7320 2b20 6765 745f  ears_mins + get_
+00001010: 6461 7973 5f6d 696e 7329 202d 2028 6765  days_mins) - (ge
+00001020: 745f 7965 6172 735f 6d69 6e73 3220 2b20  t_years_mins2 + 
+00001030: 6765 745f 6461 7973 5f6d 696e 7332 290d  get_days_mins2).
+00001040: 0a20 2020 2020 2020 2065 6c69 6620 7365  .        elif se
+00001050: 6c66 2e74 696d 655f 203d 3d20 2768 2720  lf.time_ == 'h' 
+00001060: 6f72 2073 656c 662e 7469 6d65 5f20 3d3d  or self.time_ ==
+00001070: 2027 4827 3a0d 0a20 2020 2020 2020 2020   'H':..         
+00001080: 2020 2067 6574 5f64 6179 735f 6d69 6e73     get_days_mins
+00001090: 203d 2028 6872 7320 2a20 3630 2920 2b20   = (hrs * 60) + 
+000010a0: 6d69 6e73 0d0a 2020 2020 2020 2020 2020  mins..          
+000010b0: 2020 6765 745f 7965 6172 735f 6d69 6e73    get_years_mins
+000010c0: 203d 2028 7965 6172 7320 2b20 6d6f 6e74   = (years + mont
+000010d0: 6873 202b 2064 6179 7329 202a 2032 3420  hs + days) * 24 
+000010e0: 2a20 3630 0d0a 2020 2020 2020 2020 2020  * 60..          
+000010f0: 2020 6765 745f 6461 7973 5f6d 696e 7332    get_days_mins2
+00001100: 203d 2028 6872 7332 202a 2036 3029 202b   = (hrs2 * 60) +
+00001110: 206d 696e 7332 0d0a 2020 2020 2020 2020   mins2..        
+00001120: 2020 2020 6765 745f 7965 6172 735f 6d69      get_years_mi
+00001130: 6e73 3220 3d20 2879 6561 7273 3220 2b20  ns2 = (years2 + 
+00001140: 6d6f 6e74 6873 3220 2b20 6461 7973 3229  months2 + days2)
+00001150: 202a 2032 3420 2a20 3630 0d0a 2020 2020   * 24 * 60..    
+00001160: 2020 2020 2020 2020 7265 7475 726e 2072          return r
+00001170: 6f75 6e64 2828 6765 745f 7965 6172 735f  ound((get_years_
+00001180: 6d69 6e73 202b 2067 6574 5f64 6179 735f  mins + get_days_
+00001190: 6d69 6e73 2920 2d20 2867 6574 5f79 6561  mins) - (get_yea
+000011a0: 7273 5f6d 696e 7332 202b 2067 6574 5f64  rs_mins2 + get_d
+000011b0: 6179 735f 6d69 6e73 3229 202f 2036 302c  ays_mins2) / 60,
+000011c0: 2032 290d 0a20 2020 2020 2020 2065 6c69   2)..        eli
+000011d0: 6620 7365 6c66 2e74 696d 655f 203d 3d20  f self.time_ == 
+000011e0: 2764 2720 6f72 2073 656c 662e 7469 6d65  'd' or self.time
+000011f0: 5f20 3d3d 2027 4427 3a0d 0a20 2020 2020  _ == 'D':..     
+00001200: 2020 2020 2020 2067 6574 5f64 6179 7320         get_days 
+00001210: 3d20 7965 6172 7320 2b20 6d6f 6e74 6873  = years + months
+00001220: 202b 2064 6179 730d 0a20 2020 2020 2020   + days..       
+00001230: 2020 2020 2067 6574 5f64 6179 7332 203d       get_days2 =
+00001240: 2079 6561 7273 3220 2b20 6d6f 6e74 6873   years2 + months
+00001250: 3220 2b20 6461 7973 320d 0a20 2020 2020  2 + days2..     
+00001260: 2020 2020 2020 2072 6574 7572 6e20 6765         return ge
+00001270: 745f 6461 7973 202d 2067 6574 5f64 6179  t_days - get_day
+00001280: 7332 0d0a 2020 2020 2020 2020 656c 7365  s2..        else
+00001290: 3a0d 0a20 2020 2020 2020 2020 2020 2067  :..            g
+000012a0: 6574 5f64 6179 735f 7365 6373 203d 2028  et_days_secs = (
+000012b0: 6872 7320 2a20 3630 202a 2036 3029 202b  hrs * 60 * 60) +
+000012c0: 2028 6d69 6e73 202a 2036 3029 202b 2073   (mins * 60) + s
+000012d0: 6563 735f 696e 740d 0a20 2020 2020 2020  ecs_int..       
+000012e0: 2020 2020 2067 6574 5f79 6561 7273 5f73       get_years_s
+000012f0: 6563 7320 3d20 2879 6561 7273 202b 206d  ecs = (years + m
+00001300: 6f6e 7468 7320 2b20 6461 7973 2920 2a20  onths + days) * 
+00001310: 3234 202a 2036 3020 2a20 3630 0d0a 2020  24 * 60 * 60..  
+00001320: 2020 2020 2020 2020 2020 6765 745f 6461            get_da
+00001330: 7973 5f73 6563 7332 203d 2028 6872 7332  ys_secs2 = (hrs2
+00001340: 202a 2036 3020 2a20 3630 2920 2b20 286d   * 60 * 60) + (m
+00001350: 696e 7332 202a 2036 3029 202b 2073 6563  ins2 * 60) + sec
+00001360: 735f 696e 7432 0d0a 2020 2020 2020 2020  s_int2..        
+00001370: 2020 2020 6765 745f 7965 6172 735f 7365      get_years_se
+00001380: 6373 3220 3d20 2879 6561 7273 3220 2b20  cs2 = (years2 + 
+00001390: 6d6f 6e74 6873 3220 2b20 6461 7973 3229  months2 + days2)
+000013a0: 202a 2032 3420 2a20 3630 202a 2036 300d   * 24 * 60 * 60.
+000013b0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+000013c0: 7572 6e20 2867 6574 5f79 6561 7273 5f73  urn (get_years_s
+000013d0: 6563 7320 2b20 6765 745f 6461 7973 5f73  ecs + get_days_s
+000013e0: 6563 7329 202d 2028 6765 745f 6461 7973  ecs) - (get_days
+000013f0: 5f73 6563 7332 202b 2067 6574 5f79 6561  _secs2 + get_yea
+00001400: 7273 5f73 6563 7332 290d 0a0d 0a20 2020  rs_secs2)....   
+00001410: 2040 7072 6f70 6572 7479 0d0a 2020 2020   @property..    
+00001420: 6465 6620 6461 7465 5f64 6966 6628 7365  def date_diff(se
+00001430: 6c66 293a 0d0a 2020 2020 2020 2020 2320  lf):..        # 
+00001440: 7469 6d65 2031 0d0a 2020 2020 2020 2020  time 1..        
+00001450: 736c 7567 5f74 696d 6520 3d20 7374 7228  slug_time = str(
+00001460: 7365 6c66 2e74 696d 6531 290d 0a20 2020  self.time1)..   
+00001470: 2020 2020 2066 6972 7374 203d 2073 6c75       first = slu
+00001480: 675f 7469 6d65 2e73 706c 6974 2822 2d22  g_time.split("-"
+00001490: 290d 0a20 2020 2020 2020 2073 6563 6f6e  )..        secon
+000014a0: 6420 3d20 6669 7273 745b 303a 325d 0d0a  d = first[0:2]..
+000014b0: 2020 2020 2020 2020 7468 6972 6420 3d20          third = 
+000014c0: 6669 7273 745b 325d 0d0a 2020 2020 2020  first[2]..      
+000014d0: 2020 6920 3d20 7365 636f 6e64 5b30 5d0d    i = second[0].
+000014e0: 0a20 2020 2020 2020 206a 203d 2073 6563  .        j = sec
+000014f0: 6f6e 645b 315d 0d0a 2020 2020 2020 2020  ond[1]..        
+00001500: 6b20 3d20 7468 6972 642e 7370 6c69 7428  k = third.split(
+00001510: 2220 2229 5b30 5d0d 0a20 2020 2020 2020  " ")[0]..       
+00001520: 2079 6561 725f 696e 5f64 6179 7320 3d20   year_in_days = 
+00001530: 696e 7428 6929 202a 2033 3635 0d0a 2020  int(i) * 365..  
+00001540: 2020 2020 2020 7965 6172 7320 3d20 696e        years = in
+00001550: 7428 7965 6172 5f69 6e5f 6461 7973 290d  t(year_in_days).
+00001560: 0a20 2020 2020 2020 206d 6f6e 7468 7320  .        months 
+00001570: 3d20 696e 7428 6a29 202a 2033 300d 0a20  = int(j) * 30.. 
+00001580: 2020 2020 2020 2064 6179 7320 3d20 696e         days = in
+00001590: 7428 6b29 0d0a 0d0a 2020 2020 2020 2020  t(k)....        
+000015a0: 2320 7469 6d65 2032 0d0a 2020 2020 2020  # time 2..      
+000015b0: 2020 736c 7567 5f74 696d 6520 3d20 7374    slug_time = st
+000015c0: 7228 7365 6c66 2e74 696d 6532 290d 0a20  r(self.time2).. 
+000015d0: 2020 2020 2020 2066 6972 7374 3220 3d20         first2 = 
+000015e0: 736c 7567 5f74 696d 652e 7370 6c69 7428  slug_time.split(
+000015f0: 222d 2229 0d0a 2020 2020 2020 2020 7365  "-")..        se
+00001600: 636f 6e64 3220 3d20 6669 7273 7432 5b30  cond2 = first2[0
+00001610: 3a32 5d0d 0a20 2020 2020 2020 2074 6869  :2]..        thi
+00001620: 7264 3220 3d20 6669 7273 7432 5b32 5d0d  rd2 = first2[2].
+00001630: 0a20 2020 2020 2020 2069 3220 3d20 7365  .        i2 = se
+00001640: 636f 6e64 325b 305d 0d0a 2020 2020 2020  cond2[0]..      
+00001650: 2020 6a32 203d 2073 6563 6f6e 6432 5b31    j2 = second2[1
+00001660: 5d0d 0a20 2020 2020 2020 206b 3220 3d20  ]..        k2 = 
+00001670: 7468 6972 6432 2e73 706c 6974 2822 2022  third2.split(" "
+00001680: 295b 305d 0d0a 2020 2020 2020 2020 7965  )[0]..        ye
+00001690: 6172 5f69 6e5f 6461 7973 3220 3d20 696e  ar_in_days2 = in
+000016a0: 7428 6932 2920 2a20 3336 350d 0a20 2020  t(i2) * 365..   
+000016b0: 2020 2020 2079 6561 7273 3220 3d20 696e       years2 = in
+000016c0: 7428 7965 6172 5f69 6e5f 6461 7973 290d  t(year_in_days).
+000016d0: 0a20 2020 2020 2020 206d 6f6e 7468 7332  .        months2
+000016e0: 203d 2069 6e74 286a 3229 202a 2033 300d   = int(j2) * 30.
+000016f0: 0a20 2020 2020 2020 2064 6179 7332 203d  .        days2 =
+00001700: 2069 6e74 286b 3229 0d0a 0d0a 2020 2020   int(k2)....    
+00001710: 2020 2020 6966 2073 656c 662e 7469 6d65      if self.time
+00001720: 5f20 3d3d 2027 6d27 206f 7220 7365 6c66  _ == 'm' or self
+00001730: 2e74 696d 655f 203d 3d20 276d 273a 0d0a  .time_ == 'm':..
+00001740: 2020 2020 2020 2020 2020 2020 6765 745f              get_
+00001750: 6d69 6e73 203d 2028 7965 6172 7320 2b20  mins = (years + 
+00001760: 6d6f 6e74 6873 202b 2064 6179 7329 202a  months + days) *
+00001770: 2032 3420 2a20 3630 0d0a 2020 2020 2020   24 * 60..      
+00001780: 2020 2020 2020 6765 745f 6d69 6e73 3220        get_mins2 
+00001790: 3d20 2879 6561 7273 3220 2b20 6d6f 6e74  = (years2 + mont
+000017a0: 6873 3220 2b20 6461 7973 3229 202a 2032  hs2 + days2) * 2
+000017b0: 3420 2a20 3630 0d0a 2020 2020 2020 2020  4 * 60..        
+000017c0: 2020 2020 7265 7475 726e 2067 6574 5f6d      return get_m
+000017d0: 696e 7320 2d20 6765 745f 6d69 6e73 320d  ins - get_mins2.
+000017e0: 0a20 2020 2020 2020 2065 6c69 6620 7365  .        elif se
+000017f0: 6c66 2e74 696d 655f 203d 3d20 2768 2720  lf.time_ == 'h' 
+00001800: 6f72 2073 656c 662e 7469 6d65 5f20 3d3d  or self.time_ ==
+00001810: 2027 4827 3a0d 0a20 2020 2020 2020 2020   'H':..         
+00001820: 2020 2067 6574 5f6d 696e 7320 3d20 2879     get_mins = (y
+00001830: 6561 7273 202b 206d 6f6e 7468 7320 2b20  ears + months + 
+00001840: 6461 7973 2920 2a20 3234 202a 2036 300d  days) * 24 * 60.
+00001850: 0a20 2020 2020 2020 2020 2020 2067 6574  .            get
+00001860: 5f6d 696e 7332 203d 2028 7965 6172 7332  _mins2 = (years2
+00001870: 202b 206d 6f6e 7468 7332 202b 2064 6179   + months2 + day
+00001880: 7332 2920 2a20 3234 202a 2036 300d 0a20  s2) * 24 * 60.. 
+00001890: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+000018a0: 6e20 726f 756e 6428 2867 6574 5f6d 696e  n round((get_min
+000018b0: 7320 2d20 6765 745f 6d69 6e73 3229 202f  s - get_mins2) /
+000018c0: 2036 302c 2032 290d 0a20 2020 2020 2020   60, 2)..       
+000018d0: 2065 6c69 6620 7365 6c66 2e74 696d 655f   elif self.time_
+000018e0: 203d 3d20 2764 2720 6f72 2073 656c 662e   == 'd' or self.
+000018f0: 7469 6d65 5f20 3d3d 2027 4427 3a0d 0a20  time_ == 'D':.. 
+00001900: 2020 2020 2020 2020 2020 2067 6574 5f64             get_d
+00001910: 6179 7320 3d20 7965 6172 7320 2b20 6d6f  ays = years + mo
+00001920: 6e74 6873 202b 2064 6179 730d 0a20 2020  nths + days..   
+00001930: 2020 2020 2020 2020 2067 6574 5f64 6179           get_day
+00001940: 7332 203d 2079 6561 7273 3220 2b20 6d6f  s2 = years2 + mo
+00001950: 6e74 6873 3220 2b20 6461 7973 320d 0a20  nths2 + days2.. 
+00001960: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00001970: 6e20 6765 745f 6461 7973 202d 2067 6574  n get_days - get
+00001980: 5f64 6179 7332 0d0a 2020 2020 2020 2020  _days2..        
+00001990: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
+000019a0: 2020 2067 6574 5f73 6563 7320 3d20 2879     get_secs = (y
+000019b0: 6561 7273 202b 206d 6f6e 7468 7320 2b20  ears + months + 
+000019c0: 6461 7973 2920 2a20 3234 202a 2036 3020  days) * 24 * 60 
+000019d0: 2a20 3630 0d0a 2020 2020 2020 2020 2020  * 60..          
+000019e0: 2020 6765 745f 7365 6373 3220 3d20 2879    get_secs2 = (y
+000019f0: 6561 7273 3220 2b20 6d6f 6e74 6873 3220  ears2 + months2 
+00001a00: 2b20 6461 7973 3229 202a 2032 3420 2a20  + days2) * 24 * 
+00001a10: 3630 202a 2036 300d 0a20 2020 2020 2020  60 * 60..       
+00001a20: 2020 2020 2072 6574 7572 6e20 6765 745f       return get_
+00001a30: 7365 6373 202d 2067 6574 5f73 6563 7332  secs - get_secs2
+00001a40: 0d0a 0d0a                                ....
```

### Comparing `date_time_literal-1.0.7/date_time_literal.egg-info/PKG-INFO` & `date_time_literal-1.0.8/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,128 +1,129 @@
-Metadata-Version: 2.1
-Name: date-time-literal
-Version: 1.0.7
-Summary: date-time-literal is a python module that helps convert date-time or date to literal days, hours, seconds, or even minutes. Compare two DateTime or Date objects, by converting the objects to literal days, hours, minutes, or even seconds if you want to be precise. 
-Home-page: https://github.com/kells4real/date_literal
-Download-URL: https://github.com/kells4real/date_literal/archive/refs/tags/1.0.0.tar.gz
-Author: Kelvin Sajere
-Author-email: kells4real@gmail.com
-Keywords: date-time,date,literal,date converter,literal date,date-time converter,django,python,module,python package,date-time literal,convert time,convert date-time
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.5
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# date_literal
-A package/module for converting date or date-time formats to literal days, hours, minutes, or seconds for comparison or whatever. 
-For example, you can convert DateTime objects to know just how much of a difference there is between them, or you just want 
-to get the human-readable format of DateTime or Date objects.
-
-## Installation
-> pip install date_time_literal
-
-## Usage
-#### IMPORTANT
-DateTime or Date objects must be in the default 'Y-M-D Hr:Min:Sec' and 'Y-M-D' formats respectively.
-
-##### Converts Date Time Literal
-```python
-from django.utils import timezone
-time = timezone.now()
-from date_time_literal import ConvertTime
-convert_time = ConvertTime(time).slug_date_time
-```
-##### Converts Date Literal
-convert_time = ConvertTime(time).slug_date
-This returns the date or date-time in seconds. You can add an optional parameter to specify what you want.
-
-Note: You can use the slug_date class function on a DateTime object if you wish to use only the date part of the DateTime object, 
-but cannot use the slug_date_time class function on a Date object, only on DateTime objects.
-
-#### Specific conversion to days
-
-```python
-from django.utils import timezone
-from datetime import datetime
-from date_time_literal import ConvertTime
-
-time2 = datetime.now()
-time = timezone.now()
-
-convert_time = ConvertTime(time, 'd').slug_date_time
-convert_time2 = ConvertTime(time2, 'd').slug_date
-```
-
-#### Specific conversion to hours
-
-```python
-from date_time_literal import ConvertTime
-from datetime import datetime
-time = datetime.now()
-convert_time = ConvertTime(time, 'd').slug_date_time # Converts the DateTime object to days
-convert_time1 = ConvertTime(time, 'h').slug_date_time # Converts the DateTime object to hours
-convert_time2 = ConvertTime(time, 'm').slug_date_time # Converts the DateTime object to minutes
-
-# The default conversion if none is specified is to seconds
-```
-
-### CHECK DATE-TIME OR DATE DIFFERENCE BETWEEN TWO DATE-TIME OR DATE LITERALS
-
-```python
-from date_time_literal import ConvertTime
-from datetime import datetime
-from django.utils import timezone
-time = datetime.now()
-convert_time = ConvertTime(time, 'h').slug_date_time
-from date_time_literal import date_time_diff, date_diff
-convert_time2 = ConvertTime(time, 'm').slug_date_time
-date1 = '2021-05-31'
-date2 = '2021-03-21'
-date_time1 = timezone.now()
-date_time2 = '2021-03-21 23:16:45.735963'
-date_l = date_diff(date1, date2, 'd')
-date_time_l = date_time_diff(date_time1, date_time2, 'd')
-
-# date_time_l will return the difference in value between date_time1 and date_time2 in days. You can use the 
-# corresponding string literal to get for minutes, hours and seconds which is the default value.
-# date_time_diff returns the difference in two dateTimes to the second. This should be used when you need to get 
-# date time difference to the last second
-
-```
-
-## Convert between time and dates
-You can also use the convert_time function to convert between times
-
-```python
-from date_time_literal import convert_time
-
-# Converts between years, days, hours, minutes, and seconds
-print(convert_time(365, 'd', 'y')) # Converts 365 days to years
-print(convert_time(5, 'y', 'd')) # Converts 5 years to days
-print(convert_time(5, 'y', 'h')) # Converts 5 years to hours
-print(convert_time(5, 'd', 's')) # Converts 5 days to seconds
-# etc
-```
-
-### Some Basic use cases
-To get a rather comprehensive idea of how the package works, copy the code below and run it.
-
-```python
-from date_time_literal import ConvertTime, DateDiff, date_diff, convert_time
-from datetime import datetime
-
-t = ConvertTime('2021-05-31 23:16:55.321568', 'd')
-p = ConvertTime(datetime.now(), 'd')
-i = ConvertTime('2021-05-31 23:16:55+00:00', 'd')
-d = ConvertTime('2021-05-31', time_format='d')
-e = DateDiff('2021-05-31', '2021-04-31', 'd')
-print(t.slug_date_time)
-print(i.slug_date_time)
-print(d.slug_date)
-print(e.date_diff)
-print(date_diff('2021-08-31', '2021-05-30', 'D'))
-print(convert_time(1, "y", 'h'))
-print(convert_time(365, 'd', 'y'))
-
-```
+Metadata-Version: 2.1
+Name: date_time_literal
+Version: 1.0.8
+Summary: date-time-literal is a python module that helps convert date-time or date to literal days, hours, seconds, or even minutes. Compare two DateTime or Date objects, by converting the objects to literal days, hours, minutes, or even seconds if you want to be precise. 
+Home-page: https://github.com/kells4real/date_literal
+Download-URL: https://github.com/kells4real/date_literal/archive/refs/tags/1.0.0.tar.gz
+Author: Kelvin Sajere
+Author-email: kells4real@gmail.com
+Keywords: date-time,date,literal,date converter,literal date,date-time converter,django,python,module,python package,date-time literal,convert time,convert date-time
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.5
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# date_literal
+A package/module for converting date or date-time formats to literal days, hours, minutes, or seconds for comparison or whatever. 
+For example, you can convert DateTime objects to know just how much of a difference there is between them, or you just want 
+to get the human-readable format of DateTime or Date objects.
+
+## Installation
+> pip install date_time_literal
+
+## Usage
+#### IMPORTANT
+DateTime or Date objects must be in the default 'Y-M-D Hr:Min:Sec' and 'Y-M-D' formats respectively.
+
+##### Converts Date Time Literal
+```python
+from django.utils import timezone
+time = timezone.now()
+from date_time_literal import ConvertTime
+convert_time = ConvertTime(time).slug_date_time
+```
+##### Converts Date Literal
+convert_time = ConvertTime(time).slug_date
+This returns the date or date-time in seconds. You can add an optional parameter to specify what you want.
+
+Note: You can use the slug_date class function on a DateTime object if you wish to use only the date part of the DateTime object, 
+but cannot use the slug_date_time class function on a Date object, only on DateTime objects.
+
+#### Specific conversion to days
+
+```python
+from django.utils import timezone
+from datetime import datetime
+from date_time_literal import ConvertTime
+
+time2 = datetime.now()
+time = timezone.now()
+
+convert_time = ConvertTime(time, 'd').slug_date_time
+convert_time2 = ConvertTime(time2, 'd').slug_date
+```
+
+#### Specific conversion to hours
+
+```python
+from date_time_literal import ConvertTime
+from datetime import datetime
+time = datetime.now()
+convert_time = ConvertTime(time, 'd').slug_date_time # Converts the DateTime object to days
+convert_time1 = ConvertTime(time, 'h').slug_date_time # Converts the DateTime object to hours
+convert_time2 = ConvertTime(time, 'm').slug_date_time # Converts the DateTime object to minutes
+
+# The default conversion if none is specified is to seconds
+```
+
+### CHECK DATE-TIME OR DATE DIFFERENCE BETWEEN TWO DATE-TIME OR DATE LITERALS
+
+```python
+from date_time_literal import ConvertTime
+from datetime import datetime
+from django.utils import timezone
+time = datetime.now()
+convert_time = ConvertTime(time, 'h').slug_date_time
+from date_time_literal import date_time_diff, date_diff
+convert_time2 = ConvertTime(time, 'm').slug_date_time
+date1 = '2021-05-31'
+date2 = '2021-03-21'
+date_time1 = timezone.now()
+date_time2 = '2021-03-21 23:16:45.735963'
+date_l = date_diff(date1, date2, 'd')
+date_time_l = date_time_diff(date_time1, date_time2, 'd')
+
+# date_time_l will return the difference in value between date_time1 and date_time2 in days. You can use the 
+# corresponding string literal to get for minutes, hours and seconds which is the default value.
+# date_time_diff returns the difference in two dateTimes to the second. This should be used when you need to get 
+# date time difference to the last second
+
+```
+
+## Convert between time and dates
+You can also use the convert_time function to convert between times
+
+```python
+from date_time_literal import convert_time
+
+# Converts between years, days, hours, minutes, and seconds
+print(convert_time(365, 'd', 'y')) # Converts 365 days to years
+print(convert_time(5, 'y', 'd')) # Converts 5 years to days
+print(convert_time(5, 'y', 'h')) # Converts 5 years to hours
+print(convert_time(5, 'd', 's')) # Converts 5 days to seconds
+# etc
+```
+
+### Some Basic use cases
+To get a rather comprehensive idea of how the package works, copy the code below and run it. The convert_time function
+was updated to be more efficient and now allows for week conversion as well in version 1.0.8
+
+```python
+from date_time_literal import ConvertTime, DateDiff, date_diff, convert_time
+from datetime import datetime
+
+t = ConvertTime('2021-05-31 23:16:55.321568', 'd')
+p = ConvertTime(datetime.now(), 'd')
+i = ConvertTime('2021-05-31 23:16:55+00:00', 'd')
+d = ConvertTime('2021-05-31', time_format='d')
+e = DateDiff('2021-05-31', '2021-04-31', 'd')
+print(t.slug_date_time)
+print(i.slug_date_time)
+print(d.slug_date)
+print(e.date_diff)
+print(date_diff('2021-08-31', '2021-05-30', 'D'))
+print(convert_time(1, "y", 'h'))
+print(convert_time(365, 'd', 'y'))
+
+```
```

### Comparing `date_time_literal-1.0.7/setup.py` & `date_time_literal-1.0.8/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-from setuptools import setup
-from os import path
-this_directory = path.abspath(path.dirname(__file__))
-with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
-    long_description = f.read()
-
-setup(
-    setup_requires=['wheel'],
-    name='date_time_literal',
-    packages=['date_time_literal'],
-    version='1.0.7',
-    long_description=long_description,
-    long_description_content_type='text/markdown',
-    description='date-time-literal is '
-                'a python module that helps convert date-time or'
-                ' date to literal days, hours, seconds, or even minutes. Compare two DateTime or Date objects, by'
-                ' converting the objects to literal days, hours, minutes, or even seconds if you want to be precise. ',
-    author='Kelvin Sajere',
-    author_email='kells4real@gmail.com',
-    url='https://github.com/kells4real/date_literal',
-    download_url='https://github.com/kells4real/date_literal/archive/refs/tags/1.0.0.tar.gz',
-    keywords=['date-time', 'date', 'literal', 'date converter', 'literal date', 'date-time converter',
-              'django', 'python', 'module', 'python package', 'date-time literal', 'convert time', 'convert date-time'],
-    classifiers=[
-        "Programming Language :: Python :: 3",
-        "License :: OSI Approved :: MIT License",
-        "Operating System :: OS Independent",
-    ],
-    python_requires='>=3.5',
-)
+from setuptools import setup
+from os import path
+this_directory = path.abspath(path.dirname(__file__))
+with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
+    long_description = f.read()
+
+setup(
+    setup_requires=['wheel'],
+    name='date_time_literal',
+    packages=['date_time_literal'],
+    version='1.0.8',
+    long_description=long_description,
+    long_description_content_type='text/markdown',
+    description='date-time-literal is '
+                'a python module that helps convert date-time or'
+                ' date to literal days, hours, seconds, or even minutes. Compare two DateTime or Date objects, by'
+                ' converting the objects to literal days, hours, minutes, or even seconds if you want to be precise. ',
+    author='Kelvin Sajere',
+    author_email='kells4real@gmail.com',
+    url='https://github.com/kells4real/date_literal',
+    download_url='https://github.com/kells4real/date_literal/archive/refs/tags/1.0.0.tar.gz',
+    keywords=['date-time', 'date', 'literal', 'date converter', 'literal date', 'date-time converter',
+              'django', 'python', 'module', 'python package', 'date-time literal', 'convert time', 'convert date-time'],
+    classifiers=[
+        "Programming Language :: Python :: 3",
+        "License :: OSI Approved :: MIT License",
+        "Operating System :: OS Independent",
+    ],
+    python_requires='>=3.5',
+)
```

