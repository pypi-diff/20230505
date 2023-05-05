# Comparing `tmp/date_time_literal-1.0.8.tar.gz` & `tmp/date_time_literal-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "date_time_literal-1.0.8.tar", last modified: Fri May  5 11:10:02 2023, max compression
+gzip compressed data, was "date_time_literal-1.1.0.tar", last modified: Fri May  5 14:51:32 2023, max compression
```

## Comparing `date_time_literal-1.0.8.tar` & `date_time_literal-1.1.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 11:10:02.236485 date_time_literal-1.0.8/
--rw-rw-rw-   0        0        0     1083 2022-05-31 19:43:31.000000 date_time_literal-1.0.8/LICENSE
--rw-rw-rw-   0        0        0     5188 2023-05-05 11:10:02.237834 date_time_literal-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     4240 2023-05-05 11:03:01.000000 date_time_literal-1.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-05-05 11:10:02.188731 date_time_literal-1.0.8/date_time_literal/
--rw-rw-rw-   0        0        0       51 2022-05-31 19:43:31.000000 date_time_literal-1.0.8/date_time_literal/__init__.py
--rw-rw-rw-   0        0        0     3969 2023-05-05 10:58:57.000000 date_time_literal-1.0.8/date_time_literal/difference.py
--rw-rw-rw-   0        0        0     6724 2022-05-31 20:04:31.000000 date_time_literal-1.0.8/date_time_literal/literal.py
--rw-rw-rw-   0        0        0      706 2023-05-05 10:59:51.000000 date_time_literal-1.0.8/date_time_literal/main.py
-drwxrwxrwx   0        0        0        0 2023-05-05 11:10:02.233801 date_time_literal-1.0.8/date_time_literal.egg-info/
--rw-rw-rw-   0        0        0     5188 2023-05-05 11:10:02.000000 date_time_literal-1.0.8/date_time_literal.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      317 2023-05-05 11:10:02.000000 date_time_literal-1.0.8/date_time_literal.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 11:10:02.000000 date_time_literal-1.0.8/date_time_literal.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-05-05 11:10:02.000000 date_time_literal-1.0.8/date_time_literal.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-05-05 11:10:02.239360 date_time_literal-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1435 2023-05-05 11:03:01.000000 date_time_literal-1.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-05 14:51:32.122289 date_time_literal-1.1.0/
+-rw-rw-rw-   0        0        0     1083 2022-05-31 19:43:31.000000 date_time_literal-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0     5268 2023-05-05 14:51:32.123513 date_time_literal-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4320 2023-05-05 14:46:35.000000 date_time_literal-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-05 14:51:32.081039 date_time_literal-1.1.0/date_time_literal/
+-rw-rw-rw-   0        0        0       51 2022-05-31 19:43:31.000000 date_time_literal-1.1.0/date_time_literal/__init__.py
+-rw-rw-rw-   0        0        0     1921 2023-05-05 14:11:22.000000 date_time_literal-1.1.0/date_time_literal/difference.py
+-rw-rw-rw-   0        0        0     4887 2023-05-05 14:36:08.000000 date_time_literal-1.1.0/date_time_literal/literal.py
+-rw-rw-rw-   0        0        0      799 2023-05-05 14:37:00.000000 date_time_literal-1.1.0/date_time_literal/main.py
+drwxrwxrwx   0        0        0        0 2023-05-05 14:51:32.119723 date_time_literal-1.1.0/date_time_literal.egg-info/
+-rw-rw-rw-   0        0        0     5268 2023-05-05 14:51:32.000000 date_time_literal-1.1.0/date_time_literal.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      317 2023-05-05 14:51:32.000000 date_time_literal-1.1.0/date_time_literal.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 14:51:32.000000 date_time_literal-1.1.0/date_time_literal.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-05-05 14:51:32.000000 date_time_literal-1.1.0/date_time_literal.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-05-05 14:51:32.133080 date_time_literal-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1435 2023-05-05 14:46:35.000000 date_time_literal-1.1.0/setup.py
```

### Comparing `date_time_literal-1.0.8/LICENSE` & `date_time_literal-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `date_time_literal-1.0.8/PKG-INFO` & `date_time_literal-1.1.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: date_time_literal
-Version: 1.0.8
+Version: 1.1.0
 Summary: date-time-literal is a python module that helps convert date-time or date to literal days, hours, seconds, or even minutes. Compare two DateTime or Date objects, by converting the objects to literal days, hours, minutes, or even seconds if you want to be precise. 
 Home-page: https://github.com/kells4real/date_literal
 Download-URL: https://github.com/kells4real/date_literal/archive/refs/tags/1.0.0.tar.gz
 Author: Kelvin Sajere
 Author-email: kells4real@gmail.com
 Keywords: date-time,date,literal,date converter,literal date,date-time converter,django,python,module,python package,date-time literal,convert time,convert date-time
 Classifier: Programming Language :: Python :: 3
@@ -27,75 +27,75 @@
 DateTime or Date objects must be in the default 'Y-M-D Hr:Min:Sec' and 'Y-M-D' formats respectively.
 
 ##### Converts Date Time Literal
 ```python
 from django.utils import timezone
 time = timezone.now()
 from date_time_literal import ConvertTime
-convert_time = ConvertTime(time).slug_date_time
+convert_time = ConvertTime(time).convert_time
 ```
 ##### Converts Date Literal
-convert_time = ConvertTime(time).slug_date
-This returns the date or date-time in seconds. You can add an optional parameter to specify what you want.
+convert_time = ConvertTime(time).convert
+This returns the date or date_time in seconds. You can add an optional parameter to specify what you want.
 
-Note: You can use the slug_date class function on a DateTime object if you wish to use only the date part of the DateTime object, 
-but cannot use the slug_date_time class function on a Date object, only on DateTime objects.
+Note: You can use the convert class function on a DateTime object if you wish to use only the date part of the DateTime object, 
+but cannot use the convert_time class function on a Date object, only on DateTime objects.
 
 #### Specific conversion to days
 
 ```python
 from django.utils import timezone
 from datetime import datetime
 from date_time_literal import ConvertTime
 
 time2 = datetime.now()
 time = timezone.now()
 
-convert_time = ConvertTime(time, 'd').slug_date_time
-convert_time2 = ConvertTime(time2, 'd').slug_date
+convert_time = ConvertTime(time, 'd').convert_time
+convert_time2 = ConvertTime(time2, 'd').convert
 ```
 
 #### Specific conversion to hours
 
 ```python
 from date_time_literal import ConvertTime
 from datetime import datetime
 time = datetime.now()
-convert_time = ConvertTime(time, 'd').slug_date_time # Converts the DateTime object to days
-convert_time1 = ConvertTime(time, 'h').slug_date_time # Converts the DateTime object to hours
-convert_time2 = ConvertTime(time, 'm').slug_date_time # Converts the DateTime object to minutes
+convert_time = ConvertTime(time, 'd').convert_time # Converts the DateTime object to days
+convert_time1 = ConvertTime(time, 'h').convert_time # Converts the DateTime object to hours
+convert_time2 = ConvertTime(time, 'm').convert_time # Converts the DateTime object to minutes
 
 # The default conversion if none is specified is to seconds
 ```
 
-### CHECK DATE-TIME OR DATE DIFFERENCE BETWEEN TWO DATE-TIME OR DATE LITERALS
+### CHECK DATE-TIME OR DATE DIFFERENCE BETWEEN TWO DATE-TIME OR DATE OBJECTS
 
 ```python
 from date_time_literal import ConvertTime
 from datetime import datetime
 from django.utils import timezone
 time = datetime.now()
-convert_time = ConvertTime(time, 'h').slug_date_time
+convert_time = ConvertTime(time, 'h').convert_time
 from date_time_literal import date_time_diff, date_diff
-convert_time2 = ConvertTime(time, 'm').slug_date_time
+convert_time2 = ConvertTime(time, 'm').convert_time
 date1 = '2021-05-31'
 date2 = '2021-03-21'
 date_time1 = timezone.now()
 date_time2 = '2021-03-21 23:16:45.735963'
 date_l = date_diff(date1, date2, 'd')
 date_time_l = date_time_diff(date_time1, date_time2, 'd')
 
 # date_time_l will return the difference in value between date_time1 and date_time2 in days. You can use the 
 # corresponding string literal to get for minutes, hours and seconds which is the default value.
 # date_time_diff returns the difference in two dateTimes to the second. This should be used when you need to get 
 # date time difference to the last second
 
 ```
 
-## Convert between time and dates
+## Convert between time and date objects
 You can also use the convert_time function to convert between times
 
 ```python
 from date_time_literal import convert_time
 
 # Converts between years, days, hours, minutes, and seconds
 print(convert_time(365, 'd', 'y')) # Converts 365 days to years
@@ -106,24 +106,25 @@
 ```
 
 ### Some Basic use cases
 To get a rather comprehensive idea of how the package works, copy the code below and run it. The convert_time function
 was updated to be more efficient and now allows for week conversion as well in version 1.0.8
 
 ```python
-from date_time_literal import ConvertTime, DateDiff, date_diff, convert_time
+from date_time_literal import ConvertTime, DateDiff, date_diff, convert_time, date_time_diff
 from datetime import datetime
 
 t = ConvertTime('2021-05-31 23:16:55.321568', 'd')
 p = ConvertTime(datetime.now(), 'd')
 i = ConvertTime('2021-05-31 23:16:55+00:00', 'd')
 d = ConvertTime('2021-05-31', time_format='d')
 e = DateDiff('2021-05-31', '2021-04-31', 'd')
-print(t.slug_date_time)
-print(i.slug_date_time)
-print(d.slug_date)
+print(t.convert_time)
+print(i.convert_time)
+print(d.convert)
 print(e.date_diff)
 print(date_diff('2021-08-31', '2021-05-30', 'D'))
+print(date_time_diff('2021-04-30 21:58:50+00:00', '2021-04-30 10:58:55+00:00', 'H'))
 print(convert_time(1, "y", 'h'))
 print(convert_time(365, 'd', 'y'))
 
 ```
```

### Comparing `date_time_literal-1.0.8/README.md` & `date_time_literal-1.1.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -11,75 +11,75 @@
 DateTime or Date objects must be in the default 'Y-M-D Hr:Min:Sec' and 'Y-M-D' formats respectively.
 
 ##### Converts Date Time Literal
 ```python
 from django.utils import timezone
 time = timezone.now()
 from date_time_literal import ConvertTime
-convert_time = ConvertTime(time).slug_date_time
+convert_time = ConvertTime(time).convert_time
 ```
 ##### Converts Date Literal
-convert_time = ConvertTime(time).slug_date
-This returns the date or date-time in seconds. You can add an optional parameter to specify what you want.
+convert_time = ConvertTime(time).convert
+This returns the date or date_time in seconds. You can add an optional parameter to specify what you want.
 
-Note: You can use the slug_date class function on a DateTime object if you wish to use only the date part of the DateTime object, 
-but cannot use the slug_date_time class function on a Date object, only on DateTime objects.
+Note: You can use the convert class function on a DateTime object if you wish to use only the date part of the DateTime object, 
+but cannot use the convert_time class function on a Date object, only on DateTime objects.
 
 #### Specific conversion to days
 
 ```python
 from django.utils import timezone
 from datetime import datetime
 from date_time_literal import ConvertTime
 
 time2 = datetime.now()
 time = timezone.now()
 
-convert_time = ConvertTime(time, 'd').slug_date_time
-convert_time2 = ConvertTime(time2, 'd').slug_date
+convert_time = ConvertTime(time, 'd').convert_time
+convert_time2 = ConvertTime(time2, 'd').convert
 ```
 
 #### Specific conversion to hours
 
 ```python
 from date_time_literal import ConvertTime
 from datetime import datetime
 time = datetime.now()
-convert_time = ConvertTime(time, 'd').slug_date_time # Converts the DateTime object to days
-convert_time1 = ConvertTime(time, 'h').slug_date_time # Converts the DateTime object to hours
-convert_time2 = ConvertTime(time, 'm').slug_date_time # Converts the DateTime object to minutes
+convert_time = ConvertTime(time, 'd').convert_time # Converts the DateTime object to days
+convert_time1 = ConvertTime(time, 'h').convert_time # Converts the DateTime object to hours
+convert_time2 = ConvertTime(time, 'm').convert_time # Converts the DateTime object to minutes
 
 # The default conversion if none is specified is to seconds
 ```
 
-### CHECK DATE-TIME OR DATE DIFFERENCE BETWEEN TWO DATE-TIME OR DATE LITERALS
+### CHECK DATE-TIME OR DATE DIFFERENCE BETWEEN TWO DATE-TIME OR DATE OBJECTS
 
 ```python
 from date_time_literal import ConvertTime
 from datetime import datetime
 from django.utils import timezone
 time = datetime.now()
-convert_time = ConvertTime(time, 'h').slug_date_time
+convert_time = ConvertTime(time, 'h').convert_time
 from date_time_literal import date_time_diff, date_diff
-convert_time2 = ConvertTime(time, 'm').slug_date_time
+convert_time2 = ConvertTime(time, 'm').convert_time
 date1 = '2021-05-31'
 date2 = '2021-03-21'
 date_time1 = timezone.now()
 date_time2 = '2021-03-21 23:16:45.735963'
 date_l = date_diff(date1, date2, 'd')
 date_time_l = date_time_diff(date_time1, date_time2, 'd')
 
 # date_time_l will return the difference in value between date_time1 and date_time2 in days. You can use the 
 # corresponding string literal to get for minutes, hours and seconds which is the default value.
 # date_time_diff returns the difference in two dateTimes to the second. This should be used when you need to get 
 # date time difference to the last second
 
 ```
 
-## Convert between time and dates
+## Convert between time and date objects
 You can also use the convert_time function to convert between times
 
 ```python
 from date_time_literal import convert_time
 
 # Converts between years, days, hours, minutes, and seconds
 print(convert_time(365, 'd', 'y')) # Converts 365 days to years
@@ -90,24 +90,25 @@
 ```
 
 ### Some Basic use cases
 To get a rather comprehensive idea of how the package works, copy the code below and run it. The convert_time function
 was updated to be more efficient and now allows for week conversion as well in version 1.0.8
 
 ```python
-from date_time_literal import ConvertTime, DateDiff, date_diff, convert_time
+from date_time_literal import ConvertTime, DateDiff, date_diff, convert_time, date_time_diff
 from datetime import datetime
 
 t = ConvertTime('2021-05-31 23:16:55.321568', 'd')
 p = ConvertTime(datetime.now(), 'd')
 i = ConvertTime('2021-05-31 23:16:55+00:00', 'd')
 d = ConvertTime('2021-05-31', time_format='d')
 e = DateDiff('2021-05-31', '2021-04-31', 'd')
-print(t.slug_date_time)
-print(i.slug_date_time)
-print(d.slug_date)
+print(t.convert_time)
+print(i.convert_time)
+print(d.convert)
 print(e.date_diff)
 print(date_diff('2021-08-31', '2021-05-30', 'D'))
+print(date_time_diff('2021-04-30 21:58:50+00:00', '2021-04-30 10:58:55+00:00', 'H'))
 print(convert_time(1, "y", 'h'))
 print(convert_time(365, 'd', 'y'))
 
 ```
```

### Comparing `date_time_literal-1.0.8/date_time_literal/literal.py` & `date_time_literal-1.1.0/date_time_literal/literal.py`

 * *Files 21% similar despite different names*

```diff
@@ -4,418 +4,303 @@
 00000030: 652c 2074 696d 655f 666f 726d 6174 3d27  e, time_format='
 00000040: 7327 293a 0d0a 2020 2020 2020 2020 7365  s'):..        se
 00000050: 6c66 2e74 696d 6520 3d20 7469 6d65 0d0a  lf.time = time..
 00000060: 2020 2020 2020 2020 7365 6c66 2e74 696d          self.tim
 00000070: 655f 3a20 7374 7220 3d20 7469 6d65 5f66  e_: str = time_f
 00000080: 6f72 6d61 740d 0a0d 0a20 2020 2040 7072  ormat....    @pr
 00000090: 6f70 6572 7479 0d0a 2020 2020 6465 6620  operty..    def 
-000000a0: 736c 7567 5f64 6174 655f 7469 6d65 2873  slug_date_time(s
-000000b0: 656c 6629 3a0d 0a20 2020 2020 2020 2073  elf):..        s
-000000c0: 6c75 675f 7469 6d65 203d 2073 7472 2873  lug_time = str(s
-000000d0: 656c 662e 7469 6d65 290d 0a20 2020 2020  elf.time)..     
-000000e0: 2020 2066 6972 7374 203d 2073 6c75 675f     first = slug_
-000000f0: 7469 6d65 2e73 706c 6974 2822 2d22 290d  time.split("-").
-00000100: 0a20 2020 2020 2020 2073 6563 6f6e 6420  .        second 
-00000110: 3d20 6669 7273 745b 303a 325d 0d0a 2020  = first[0:2]..  
-00000120: 2020 2020 2020 7468 6972 6420 3d20 6669        third = fi
-00000130: 7273 745b 325d 0d0a 2020 2020 2020 2020  rst[2]..        
-00000140: 666f 7572 7468 203d 2074 6869 7264 2e73  fourth = third.s
-00000150: 706c 6974 2822 2022 295b 315d 2e73 706c  plit(" ")[1].spl
-00000160: 6974 2822 3a22 290d 0a20 2020 2020 2020  it(":")..       
-00000170: 2069 203d 2073 6563 6f6e 645b 305d 0d0a   i = second[0]..
-00000180: 2020 2020 2020 2020 6a20 3d20 7365 636f          j = seco
-00000190: 6e64 5b31 5d0d 0a20 2020 2020 2020 206b  nd[1]..        k
-000001a0: 203d 2074 6869 7264 2e73 706c 6974 2822   = third.split("
-000001b0: 2022 295b 305d 0d0a 2020 2020 2020 2020   ")[0]..        
-000001c0: 6872 7320 3d20 696e 7428 666f 7572 7468  hrs = int(fourth
-000001d0: 5b30 5d29 0d0a 2020 2020 2020 2020 6d69  [0])..        mi
-000001e0: 6e73 203d 2069 6e74 2866 6f75 7274 685b  ns = int(fourth[
-000001f0: 315d 290d 0a20 2020 2020 2020 2073 6563  1])..        sec
-00000200: 7320 3d20 666f 7572 7468 5b32 5d2e 7370  s = fourth[2].sp
-00000210: 6c69 7428 222e 2229 5b30 5d0d 0a20 2020  lit(".")[0]..   
-00000220: 2020 2020 2069 6620 272b 2720 696e 2073       if '+' in s
-00000230: 6563 733a 0d0a 2020 2020 2020 2020 2020  ecs:..          
-00000240: 2020 7365 6373 203d 2073 6563 732e 7370    secs = secs.sp
-00000250: 6c69 7428 272b 2729 5b30 5d0d 0a20 2020  lit('+')[0]..   
-00000260: 2020 2020 2073 6563 735f 696e 7420 3d20       secs_int = 
-00000270: 696e 7428 7365 6373 290d 0a20 2020 2020  int(secs)..     
-00000280: 2020 2079 6561 725f 696e 5f64 6179 7320     year_in_days 
-00000290: 3d20 696e 7428 6929 202a 2033 3635 0d0a  = int(i) * 365..
-000002a0: 2020 2020 2020 2020 7965 6172 7320 3d20          years = 
-000002b0: 696e 7428 7965 6172 5f69 6e5f 6461 7973  int(year_in_days
-000002c0: 290d 0a20 2020 2020 2020 206d 6f6e 7468  )..        month
-000002d0: 7320 3d20 696e 7428 6a29 202a 2033 300d  s = int(j) * 30.
-000002e0: 0a20 2020 2020 2020 2064 6179 7320 3d20  .        days = 
-000002f0: 696e 7428 6b29 0d0a 2020 2020 2020 2020  int(k)..        
-00000300: 6966 2073 656c 662e 7469 6d65 5f20 3d3d  if self.time_ ==
-00000310: 2027 6d27 3a0d 0a20 2020 2020 2020 2020   'm':..         
-00000320: 2020 2067 6574 5f64 6179 735f 6d69 6e73     get_days_mins
-00000330: 203d 2028 6872 7320 2a20 3630 2920 2b20   = (hrs * 60) + 
-00000340: 6d69 6e73 0d0a 2020 2020 2020 2020 2020  mins..          
-00000350: 2020 6765 745f 7965 6172 735f 6d69 6e73    get_years_mins
-00000360: 203d 2028 7965 6172 7320 2b20 6d6f 6e74   = (years + mont
-00000370: 6873 202b 2064 6179 7329 202a 2032 3420  hs + days) * 24 
-00000380: 2a20 3630 0d0a 2020 2020 2020 2020 2020  * 60..          
-00000390: 2020 7265 7475 726e 2067 6574 5f79 6561    return get_yea
-000003a0: 7273 5f6d 696e 7320 2b20 6765 745f 6461  rs_mins + get_da
-000003b0: 7973 5f6d 696e 730d 0a20 2020 2020 2020  ys_mins..       
-000003c0: 2065 6c69 6620 7365 6c66 2e74 696d 655f   elif self.time_
-000003d0: 203d 3d20 2768 273a 0d0a 2020 2020 2020   == 'h':..      
-000003e0: 2020 2020 2020 6765 745f 6461 7973 5f6d        get_days_m
-000003f0: 696e 7320 3d20 2868 7273 202a 2036 3029  ins = (hrs * 60)
-00000400: 202b 206d 696e 730d 0a20 2020 2020 2020   + mins..       
-00000410: 2020 2020 2067 6574 5f79 6561 7273 5f6d       get_years_m
-00000420: 696e 7320 3d20 2879 6561 7273 202b 206d  ins = (years + m
-00000430: 6f6e 7468 7320 2b20 6461 7973 2920 2a20  onths + days) * 
-00000440: 3234 202a 2036 300d 0a20 2020 2020 2020  24 * 60..       
-00000450: 2020 2020 2072 6574 7572 6e20 726f 756e       return roun
-00000460: 6428 2867 6574 5f79 6561 7273 5f6d 696e  d((get_years_min
-00000470: 7320 2b20 6765 745f 6461 7973 5f6d 696e  s + get_days_min
-00000480: 7329 202f 2036 302c 2032 290d 0a20 2020  s) / 60, 2)..   
-00000490: 2020 2020 2065 6c69 6620 7365 6c66 2e74       elif self.t
-000004a0: 696d 655f 203d 3d20 2764 273a 0d0a 2020  ime_ == 'd':..  
-000004b0: 2020 2020 2020 2020 2020 6765 745f 7965            get_ye
-000004c0: 6172 735f 6461 7973 203d 2079 6561 7273  ars_days = years
-000004d0: 202b 206d 6f6e 7468 7320 2b20 6461 7973   + months + days
-000004e0: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
-000004f0: 7475 726e 2067 6574 5f79 6561 7273 5f64  turn get_years_d
-00000500: 6179 730d 0a20 2020 2020 2020 2065 6c73  ays..        els
-00000510: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-00000520: 6765 745f 6461 7973 5f73 6563 7320 3d20  get_days_secs = 
-00000530: 2868 7273 202a 2036 3020 2a20 3630 2920  (hrs * 60 * 60) 
-00000540: 2b20 286d 696e 7320 2a20 3630 2920 2b20  + (mins * 60) + 
-00000550: 7365 6373 5f69 6e74 0d0a 2020 2020 2020  secs_int..      
-00000560: 2020 2020 2020 6765 745f 7965 6172 735f        get_years_
-00000570: 7365 6373 203d 2028 7965 6172 7320 2b20  secs = (years + 
-00000580: 6d6f 6e74 6873 202b 2064 6179 7329 202a  months + days) *
-00000590: 2032 3420 2a20 3630 202a 2036 300d 0a20   24 * 60 * 60.. 
-000005a0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-000005b0: 6e20 6765 745f 7965 6172 735f 7365 6373  n get_years_secs
-000005c0: 202b 2067 6574 5f64 6179 735f 7365 6373   + get_days_secs
-000005d0: 0d0a 0d0a 2020 2020 4070 726f 7065 7274  ....    @propert
-000005e0: 790d 0a20 2020 2064 6566 2073 6c75 675f  y..    def slug_
-000005f0: 6461 7465 2873 656c 6629 3a0d 0a20 2020  date(self):..   
-00000600: 2020 2020 2073 6c75 675f 7469 6d65 3a20       slug_time: 
-00000610: 7374 7220 3d20 7374 7228 7365 6c66 2e74  str = str(self.t
-00000620: 696d 6529 0d0a 2020 2020 2020 2020 6669  ime)..        fi
-00000630: 7273 7420 3d20 736c 7567 5f74 696d 652e  rst = slug_time.
-00000640: 7370 6c69 7428 222d 2229 0d0a 2020 2020  split("-")..    
-00000650: 2020 2020 7365 636f 6e64 203d 2066 6972      second = fir
-00000660: 7374 5b30 3a32 5d0d 0a20 2020 2020 2020  st[0:2]..       
-00000670: 2074 6869 7264 203d 2066 6972 7374 5b32   third = first[2
-00000680: 5d0d 0a20 2020 2020 2020 2069 203d 2073  ]..        i = s
-00000690: 6563 6f6e 645b 305d 0d0a 2020 2020 2020  econd[0]..      
-000006a0: 2020 6a20 3d20 7365 636f 6e64 5b31 5d0d    j = second[1].
-000006b0: 0a20 2020 2020 2020 206b 203d 2074 6869  .        k = thi
-000006c0: 7264 2e73 706c 6974 2822 2022 295b 305d  rd.split(" ")[0]
-000006d0: 0d0a 2020 2020 2020 2020 7965 6172 5f69  ..        year_i
-000006e0: 6e5f 6461 7973 203d 2069 6e74 2869 2920  n_days = int(i) 
-000006f0: 2a20 3336 350d 0a20 2020 2020 2020 2079  * 365..        y
-00000700: 6561 7273 203d 2069 6e74 2879 6561 725f  ears = int(year_
-00000710: 696e 5f64 6179 7329 0d0a 2020 2020 2020  in_days)..      
-00000720: 2020 6d6f 6e74 6873 203d 2069 6e74 286a    months = int(j
-00000730: 2920 2a20 3330 0d0a 2020 2020 2020 2020  ) * 30..        
-00000740: 6461 7973 203d 2069 6e74 286b 290d 0a20  days = int(k).. 
-00000750: 2020 2020 2020 2069 6620 7365 6c66 2e74         if self.t
-00000760: 696d 655f 203d 3d20 276d 273a 0d0a 2020  ime_ == 'm':..  
-00000770: 2020 2020 2020 2020 2020 6765 745f 6d69            get_mi
-00000780: 6e73 203d 2028 7965 6172 7320 2b20 6d6f  ns = (years + mo
-00000790: 6e74 6873 202b 2064 6179 7329 202a 2032  nths + days) * 2
-000007a0: 3420 2a20 3630 0d0a 2020 2020 2020 2020  4 * 60..        
-000007b0: 2020 2020 7265 7475 726e 2067 6574 5f6d      return get_m
-000007c0: 696e 730d 0a20 2020 2020 2020 2065 6c69  ins..        eli
-000007d0: 6620 7365 6c66 2e74 696d 655f 203d 3d20  f self.time_ == 
-000007e0: 2768 273a 0d0a 2020 2020 2020 2020 2020  'h':..          
-000007f0: 2020 6765 745f 6872 7320 3d20 726f 756e    get_hrs = roun
-00000800: 6428 2828 7965 6172 7320 2b20 6d6f 6e74  d(((years + mont
-00000810: 6873 202b 2064 6179 7329 202a 2032 3420  hs + days) * 24 
-00000820: 2a20 3630 2920 2f20 3630 2c20 3229 0d0a  * 60) / 60, 2)..
-00000830: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00000840: 726e 2067 6574 5f68 7273 0d0a 2020 2020  rn get_hrs..    
-00000850: 2020 2020 656c 6966 2073 656c 662e 7469      elif self.ti
-00000860: 6d65 5f20 3d3d 2027 6427 3a0d 0a20 2020  me_ == 'd':..   
-00000870: 2020 2020 2020 2020 2067 6574 5f64 6179           get_day
-00000880: 7320 3d20 7965 6172 7320 2b20 6d6f 6e74  s = years + mont
-00000890: 6873 202b 2064 6179 730d 0a20 2020 2020  hs + days..     
-000008a0: 2020 2020 2020 2072 6574 7572 6e20 6765         return ge
-000008b0: 745f 6461 7973 0d0a 2020 2020 2020 2020  t_days..        
-000008c0: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
-000008d0: 2020 2067 6574 5f73 6563 7320 3d20 2879     get_secs = (y
-000008e0: 6561 7273 202b 206d 6f6e 7468 7320 2b20  ears + months + 
-000008f0: 6461 7973 2920 2a20 3234 202a 2036 3020  days) * 24 * 60 
-00000900: 2a20 3630 0d0a 2020 2020 2020 2020 2020  * 60..          
-00000910: 2020 7265 7475 726e 2067 6574 5f73 6563    return get_sec
-00000920: 730d 0a0d 0a0d 0a63 6c61 7373 2044 6174  s......class Dat
-00000930: 6544 6966 663a 0d0a 2020 2020 6465 6620  eDiff:..    def 
-00000940: 5f5f 696e 6974 5f5f 2873 656c 662c 2074  __init__(self, t
-00000950: 696d 6531 2c20 7469 6d65 322c 2074 696d  ime1, time2, tim
-00000960: 655f 666f 726d 6174 3d27 7327 293a 0d0a  e_format='s'):..
-00000970: 2020 2020 2020 2020 7365 6c66 2e74 696d          self.tim
-00000980: 6531 203d 2074 696d 6531 0d0a 2020 2020  e1 = time1..    
-00000990: 2020 2020 7365 6c66 2e74 696d 6532 203d      self.time2 =
-000009a0: 2074 696d 6532 0d0a 2020 2020 2020 2020   time2..        
-000009b0: 7365 6c66 2e74 696d 655f 3a20 7374 7220  self.time_: str 
-000009c0: 3d20 7469 6d65 5f66 6f72 6d61 740d 0a0d  = time_format...
-000009d0: 0a20 2020 2040 7072 6f70 6572 7479 0d0a  .    @property..
-000009e0: 2020 2020 6465 6620 6461 7465 5f74 696d      def date_tim
-000009f0: 655f 6469 6666 2873 656c 6629 3a0d 0a20  e_diff(self):.. 
-00000a00: 2020 2020 2020 2023 2074 696d 6520 310d         # time 1.
-00000a10: 0a20 2020 2020 2020 2073 6c75 675f 7469  .        slug_ti
-00000a20: 6d65 3120 3d20 7374 7228 7365 6c66 2e74  me1 = str(self.t
-00000a30: 696d 6531 290d 0a20 2020 2020 2020 2066  ime1)..        f
-00000a40: 6972 7374 203d 2073 6c75 675f 7469 6d65  irst = slug_time
-00000a50: 312e 7370 6c69 7428 222d 2229 0d0a 2020  1.split("-")..  
-00000a60: 2020 2020 2020 7365 636f 6e64 203d 2066        second = f
-00000a70: 6972 7374 5b30 3a32 5d0d 0a20 2020 2020  irst[0:2]..     
-00000a80: 2020 2074 6869 7264 203d 2066 6972 7374     third = first
-00000a90: 5b32 5d0d 0a20 2020 2020 2020 2066 6f75  [2]..        fou
-00000aa0: 7274 6820 3d20 7468 6972 642e 7370 6c69  rth = third.spli
-00000ab0: 7428 2220 2229 5b31 5d2e 7370 6c69 7428  t(" ")[1].split(
-00000ac0: 223a 2229 0d0a 2020 2020 2020 2020 6920  ":")..        i 
-00000ad0: 3d20 7365 636f 6e64 5b30 5d0d 0a20 2020  = second[0]..   
-00000ae0: 2020 2020 206a 203d 2073 6563 6f6e 645b       j = second[
-00000af0: 315d 0d0a 2020 2020 2020 2020 6b20 3d20  1]..        k = 
-00000b00: 7468 6972 642e 7370 6c69 7428 2220 2229  third.split(" ")
-00000b10: 5b30 5d0d 0a20 2020 2020 2020 2068 7273  [0]..        hrs
-00000b20: 203d 2069 6e74 2866 6f75 7274 685b 305d   = int(fourth[0]
-00000b30: 290d 0a20 2020 2020 2020 206d 696e 7320  )..        mins 
-00000b40: 3d20 696e 7428 666f 7572 7468 5b31 5d29  = int(fourth[1])
-00000b50: 0d0a 2020 2020 2020 2020 7365 6373 203d  ..        secs =
-00000b60: 2066 6f75 7274 685b 325d 2e73 706c 6974   fourth[2].split
-00000b70: 2822 2e22 295b 305d 0d0a 2020 2020 2020  (".")[0]..      
-00000b80: 2020 6966 2027 2b27 2069 6e20 7365 6373    if '+' in secs
-00000b90: 3a0d 0a20 2020 2020 2020 2020 2020 2073  :..            s
-00000ba0: 6563 7320 3d20 7365 6373 2e73 706c 6974  ecs = secs.split
-00000bb0: 2827 2b27 295b 305d 0d0a 2020 2020 2020  ('+')[0]..      
-00000bc0: 2020 7365 6373 5f69 6e74 203d 2069 6e74    secs_int = int
-00000bd0: 2873 6563 7329 0d0a 2020 2020 2020 2020  (secs)..        
-00000be0: 7965 6172 5f69 6e5f 6461 7973 203d 2069  year_in_days = i
-00000bf0: 6e74 2869 2920 2a20 3336 350d 0a20 2020  nt(i) * 365..   
-00000c00: 2020 2020 2079 6561 7273 203d 2069 6e74       years = int
-00000c10: 2879 6561 725f 696e 5f64 6179 7329 0d0a  (year_in_days)..
-00000c20: 2020 2020 2020 2020 6d6f 6e74 6873 203d          months =
-00000c30: 2069 6e74 286a 2920 2a20 3330 0d0a 2020   int(j) * 30..  
-00000c40: 2020 2020 2020 6461 7973 203d 2069 6e74        days = int
-00000c50: 286b 290d 0a0d 0a20 2020 2020 2020 2023  (k)....        #
-00000c60: 2074 696d 6532 0d0a 2020 2020 2020 2020   time2..        
-00000c70: 736c 7567 5f74 696d 6532 203d 2073 7472  slug_time2 = str
-00000c80: 2873 656c 662e 7469 6d65 3229 0d0a 2020  (self.time2)..  
-00000c90: 2020 2020 2020 6669 7273 7432 203d 2073        first2 = s
-00000ca0: 6c75 675f 7469 6d65 322e 7370 6c69 7428  lug_time2.split(
-00000cb0: 222d 2229 0d0a 2020 2020 2020 2020 7365  "-")..        se
-00000cc0: 636f 6e64 3220 3d20 6669 7273 7432 5b30  cond2 = first2[0
-00000cd0: 3a32 5d0d 0a20 2020 2020 2020 2074 6869  :2]..        thi
-00000ce0: 7264 3220 3d20 6669 7273 7432 5b32 5d0d  rd2 = first2[2].
-00000cf0: 0a20 2020 2020 2020 2066 6f75 7274 6832  .        fourth2
-00000d00: 203d 2074 6869 7264 322e 7370 6c69 7428   = third2.split(
-00000d10: 2220 2229 5b31 5d2e 7370 6c69 7428 223a  " ")[1].split(":
-00000d20: 2229 0d0a 2020 2020 2020 2020 6932 203d  ")..        i2 =
-00000d30: 2073 6563 6f6e 6432 5b30 5d0d 0a20 2020   second2[0]..   
-00000d40: 2020 2020 206a 3220 3d20 7365 636f 6e64       j2 = second
-00000d50: 325b 315d 0d0a 2020 2020 2020 2020 6b32  2[1]..        k2
-00000d60: 203d 2074 6869 7264 322e 7370 6c69 7428   = third2.split(
-00000d70: 2220 2229 5b30 5d0d 0a20 2020 2020 2020  " ")[0]..       
-00000d80: 2068 7273 3220 3d20 696e 7428 666f 7572   hrs2 = int(four
-00000d90: 7468 325b 305d 290d 0a20 2020 2020 2020  th2[0])..       
-00000da0: 206d 696e 7332 203d 2069 6e74 2866 6f75   mins2 = int(fou
-00000db0: 7274 6832 5b31 5d29 0d0a 2020 2020 2020  rth2[1])..      
-00000dc0: 2020 7365 6373 3220 3d20 666f 7572 7468    secs2 = fourth
-00000dd0: 325b 325d 2e73 706c 6974 2822 2e22 295b  2[2].split(".")[
-00000de0: 305d 0d0a 2020 2020 2020 2020 6966 2027  0]..        if '
-00000df0: 2b27 2069 6e20 7365 6373 323a 0d0a 2020  +' in secs2:..  
-00000e00: 2020 2020 2020 2020 2020 7365 6373 3220            secs2 
-00000e10: 3d20 7365 6373 322e 7370 6c69 7428 272b  = secs2.split('+
-00000e20: 2729 5b30 5d0d 0a20 2020 2020 2020 2073  ')[0]..        s
-00000e30: 6563 735f 696e 7432 203d 2069 6e74 2873  ecs_int2 = int(s
-00000e40: 6563 7332 290d 0a20 2020 2020 2020 2079  ecs2)..        y
-00000e50: 6561 725f 696e 5f64 6179 7332 203d 2069  ear_in_days2 = i
-00000e60: 6e74 2869 3229 202a 2033 3635 0d0a 2020  nt(i2) * 365..  
-00000e70: 2020 2020 2020 7965 6172 7332 203d 2069        years2 = i
-00000e80: 6e74 2879 6561 725f 696e 5f64 6179 7332  nt(year_in_days2
-00000e90: 290d 0a20 2020 2020 2020 206d 6f6e 7468  )..        month
-00000ea0: 7332 203d 2069 6e74 286a 3229 202a 2033  s2 = int(j2) * 3
-00000eb0: 300d 0a20 2020 2020 2020 2064 6179 7332  0..        days2
-00000ec0: 203d 2069 6e74 286b 3229 0d0a 0d0a 2020   = int(k2)....  
-00000ed0: 2020 2020 2020 6966 2073 656c 662e 7469        if self.ti
-00000ee0: 6d65 5f20 3d3d 2027 6d27 206f 7220 7365  me_ == 'm' or se
-00000ef0: 6c66 2e74 696d 655f 203d 3d20 274d 273a  lf.time_ == 'M':
-00000f00: 0d0a 2020 2020 2020 2020 2020 2020 6765  ..            ge
-00000f10: 745f 6461 7973 5f6d 696e 7320 3d20 2868  t_days_mins = (h
-00000f20: 7273 202a 2036 3029 202b 206d 696e 730d  rs * 60) + mins.
-00000f30: 0a20 2020 2020 2020 2020 2020 2067 6574  .            get
-00000f40: 5f79 6561 7273 5f6d 696e 7320 3d20 2879  _years_mins = (y
-00000f50: 6561 7273 202b 206d 6f6e 7468 7320 2b20  ears + months + 
-00000f60: 6461 7973 2920 2a20 3234 202a 2036 300d  days) * 24 * 60.
-00000f70: 0a20 2020 2020 2020 2020 2020 2067 6574  .            get
-00000f80: 5f64 6179 735f 6d69 6e73 3220 3d20 2868  _days_mins2 = (h
-00000f90: 7273 3220 2a20 3630 2920 2b20 6d69 6e73  rs2 * 60) + mins
-00000fa0: 320d 0a20 2020 2020 2020 2020 2020 2067  2..            g
-00000fb0: 6574 5f79 6561 7273 5f6d 696e 7332 203d  et_years_mins2 =
-00000fc0: 2028 7965 6172 7332 202b 206d 6f6e 7468   (years2 + month
-00000fd0: 7332 202b 2064 6179 7332 2920 2a20 3234  s2 + days2) * 24
-00000fe0: 202a 2036 300d 0a20 2020 2020 2020 2020   * 60..         
-00000ff0: 2020 2072 6574 7572 6e20 2867 6574 5f79     return (get_y
-00001000: 6561 7273 5f6d 696e 7320 2b20 6765 745f  ears_mins + get_
-00001010: 6461 7973 5f6d 696e 7329 202d 2028 6765  days_mins) - (ge
-00001020: 745f 7965 6172 735f 6d69 6e73 3220 2b20  t_years_mins2 + 
-00001030: 6765 745f 6461 7973 5f6d 696e 7332 290d  get_days_mins2).
-00001040: 0a20 2020 2020 2020 2065 6c69 6620 7365  .        elif se
-00001050: 6c66 2e74 696d 655f 203d 3d20 2768 2720  lf.time_ == 'h' 
-00001060: 6f72 2073 656c 662e 7469 6d65 5f20 3d3d  or self.time_ ==
-00001070: 2027 4827 3a0d 0a20 2020 2020 2020 2020   'H':..         
-00001080: 2020 2067 6574 5f64 6179 735f 6d69 6e73     get_days_mins
-00001090: 203d 2028 6872 7320 2a20 3630 2920 2b20   = (hrs * 60) + 
-000010a0: 6d69 6e73 0d0a 2020 2020 2020 2020 2020  mins..          
-000010b0: 2020 6765 745f 7965 6172 735f 6d69 6e73    get_years_mins
-000010c0: 203d 2028 7965 6172 7320 2b20 6d6f 6e74   = (years + mont
-000010d0: 6873 202b 2064 6179 7329 202a 2032 3420  hs + days) * 24 
-000010e0: 2a20 3630 0d0a 2020 2020 2020 2020 2020  * 60..          
-000010f0: 2020 6765 745f 6461 7973 5f6d 696e 7332    get_days_mins2
-00001100: 203d 2028 6872 7332 202a 2036 3029 202b   = (hrs2 * 60) +
-00001110: 206d 696e 7332 0d0a 2020 2020 2020 2020   mins2..        
-00001120: 2020 2020 6765 745f 7965 6172 735f 6d69      get_years_mi
-00001130: 6e73 3220 3d20 2879 6561 7273 3220 2b20  ns2 = (years2 + 
-00001140: 6d6f 6e74 6873 3220 2b20 6461 7973 3229  months2 + days2)
-00001150: 202a 2032 3420 2a20 3630 0d0a 2020 2020   * 24 * 60..    
-00001160: 2020 2020 2020 2020 7265 7475 726e 2072          return r
-00001170: 6f75 6e64 2828 6765 745f 7965 6172 735f  ound((get_years_
-00001180: 6d69 6e73 202b 2067 6574 5f64 6179 735f  mins + get_days_
-00001190: 6d69 6e73 2920 2d20 2867 6574 5f79 6561  mins) - (get_yea
-000011a0: 7273 5f6d 696e 7332 202b 2067 6574 5f64  rs_mins2 + get_d
-000011b0: 6179 735f 6d69 6e73 3229 202f 2036 302c  ays_mins2) / 60,
-000011c0: 2032 290d 0a20 2020 2020 2020 2065 6c69   2)..        eli
-000011d0: 6620 7365 6c66 2e74 696d 655f 203d 3d20  f self.time_ == 
-000011e0: 2764 2720 6f72 2073 656c 662e 7469 6d65  'd' or self.time
-000011f0: 5f20 3d3d 2027 4427 3a0d 0a20 2020 2020  _ == 'D':..     
-00001200: 2020 2020 2020 2067 6574 5f64 6179 7320         get_days 
-00001210: 3d20 7965 6172 7320 2b20 6d6f 6e74 6873  = years + months
-00001220: 202b 2064 6179 730d 0a20 2020 2020 2020   + days..       
-00001230: 2020 2020 2067 6574 5f64 6179 7332 203d       get_days2 =
-00001240: 2079 6561 7273 3220 2b20 6d6f 6e74 6873   years2 + months
-00001250: 3220 2b20 6461 7973 320d 0a20 2020 2020  2 + days2..     
-00001260: 2020 2020 2020 2072 6574 7572 6e20 6765         return ge
-00001270: 745f 6461 7973 202d 2067 6574 5f64 6179  t_days - get_day
-00001280: 7332 0d0a 2020 2020 2020 2020 656c 7365  s2..        else
-00001290: 3a0d 0a20 2020 2020 2020 2020 2020 2067  :..            g
-000012a0: 6574 5f64 6179 735f 7365 6373 203d 2028  et_days_secs = (
-000012b0: 6872 7320 2a20 3630 202a 2036 3029 202b  hrs * 60 * 60) +
-000012c0: 2028 6d69 6e73 202a 2036 3029 202b 2073   (mins * 60) + s
-000012d0: 6563 735f 696e 740d 0a20 2020 2020 2020  ecs_int..       
-000012e0: 2020 2020 2067 6574 5f79 6561 7273 5f73       get_years_s
-000012f0: 6563 7320 3d20 2879 6561 7273 202b 206d  ecs = (years + m
-00001300: 6f6e 7468 7320 2b20 6461 7973 2920 2a20  onths + days) * 
-00001310: 3234 202a 2036 3020 2a20 3630 0d0a 2020  24 * 60 * 60..  
-00001320: 2020 2020 2020 2020 2020 6765 745f 6461            get_da
-00001330: 7973 5f73 6563 7332 203d 2028 6872 7332  ys_secs2 = (hrs2
-00001340: 202a 2036 3020 2a20 3630 2920 2b20 286d   * 60 * 60) + (m
-00001350: 696e 7332 202a 2036 3029 202b 2073 6563  ins2 * 60) + sec
-00001360: 735f 696e 7432 0d0a 2020 2020 2020 2020  s_int2..        
-00001370: 2020 2020 6765 745f 7965 6172 735f 7365      get_years_se
-00001380: 6373 3220 3d20 2879 6561 7273 3220 2b20  cs2 = (years2 + 
-00001390: 6d6f 6e74 6873 3220 2b20 6461 7973 3229  months2 + days2)
-000013a0: 202a 2032 3420 2a20 3630 202a 2036 300d   * 24 * 60 * 60.
-000013b0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-000013c0: 7572 6e20 2867 6574 5f79 6561 7273 5f73  urn (get_years_s
-000013d0: 6563 7320 2b20 6765 745f 6461 7973 5f73  ecs + get_days_s
-000013e0: 6563 7329 202d 2028 6765 745f 6461 7973  ecs) - (get_days
-000013f0: 5f73 6563 7332 202b 2067 6574 5f79 6561  _secs2 + get_yea
-00001400: 7273 5f73 6563 7332 290d 0a0d 0a20 2020  rs_secs2)....   
-00001410: 2040 7072 6f70 6572 7479 0d0a 2020 2020   @property..    
-00001420: 6465 6620 6461 7465 5f64 6966 6628 7365  def date_diff(se
-00001430: 6c66 293a 0d0a 2020 2020 2020 2020 2320  lf):..        # 
-00001440: 7469 6d65 2031 0d0a 2020 2020 2020 2020  time 1..        
-00001450: 736c 7567 5f74 696d 6520 3d20 7374 7228  slug_time = str(
-00001460: 7365 6c66 2e74 696d 6531 290d 0a20 2020  self.time1)..   
-00001470: 2020 2020 2066 6972 7374 203d 2073 6c75       first = slu
-00001480: 675f 7469 6d65 2e73 706c 6974 2822 2d22  g_time.split("-"
-00001490: 290d 0a20 2020 2020 2020 2073 6563 6f6e  )..        secon
-000014a0: 6420 3d20 6669 7273 745b 303a 325d 0d0a  d = first[0:2]..
-000014b0: 2020 2020 2020 2020 7468 6972 6420 3d20          third = 
-000014c0: 6669 7273 745b 325d 0d0a 2020 2020 2020  first[2]..      
-000014d0: 2020 6920 3d20 7365 636f 6e64 5b30 5d0d    i = second[0].
-000014e0: 0a20 2020 2020 2020 206a 203d 2073 6563  .        j = sec
-000014f0: 6f6e 645b 315d 0d0a 2020 2020 2020 2020  ond[1]..        
-00001500: 6b20 3d20 7468 6972 642e 7370 6c69 7428  k = third.split(
-00001510: 2220 2229 5b30 5d0d 0a20 2020 2020 2020  " ")[0]..       
-00001520: 2079 6561 725f 696e 5f64 6179 7320 3d20   year_in_days = 
-00001530: 696e 7428 6929 202a 2033 3635 0d0a 2020  int(i) * 365..  
-00001540: 2020 2020 2020 7965 6172 7320 3d20 696e        years = in
-00001550: 7428 7965 6172 5f69 6e5f 6461 7973 290d  t(year_in_days).
-00001560: 0a20 2020 2020 2020 206d 6f6e 7468 7320  .        months 
-00001570: 3d20 696e 7428 6a29 202a 2033 300d 0a20  = int(j) * 30.. 
-00001580: 2020 2020 2020 2064 6179 7320 3d20 696e         days = in
-00001590: 7428 6b29 0d0a 0d0a 2020 2020 2020 2020  t(k)....        
-000015a0: 2320 7469 6d65 2032 0d0a 2020 2020 2020  # time 2..      
-000015b0: 2020 736c 7567 5f74 696d 6520 3d20 7374    slug_time = st
-000015c0: 7228 7365 6c66 2e74 696d 6532 290d 0a20  r(self.time2).. 
-000015d0: 2020 2020 2020 2066 6972 7374 3220 3d20         first2 = 
-000015e0: 736c 7567 5f74 696d 652e 7370 6c69 7428  slug_time.split(
-000015f0: 222d 2229 0d0a 2020 2020 2020 2020 7365  "-")..        se
-00001600: 636f 6e64 3220 3d20 6669 7273 7432 5b30  cond2 = first2[0
-00001610: 3a32 5d0d 0a20 2020 2020 2020 2074 6869  :2]..        thi
-00001620: 7264 3220 3d20 6669 7273 7432 5b32 5d0d  rd2 = first2[2].
-00001630: 0a20 2020 2020 2020 2069 3220 3d20 7365  .        i2 = se
-00001640: 636f 6e64 325b 305d 0d0a 2020 2020 2020  cond2[0]..      
-00001650: 2020 6a32 203d 2073 6563 6f6e 6432 5b31    j2 = second2[1
-00001660: 5d0d 0a20 2020 2020 2020 206b 3220 3d20  ]..        k2 = 
-00001670: 7468 6972 6432 2e73 706c 6974 2822 2022  third2.split(" "
-00001680: 295b 305d 0d0a 2020 2020 2020 2020 7965  )[0]..        ye
-00001690: 6172 5f69 6e5f 6461 7973 3220 3d20 696e  ar_in_days2 = in
-000016a0: 7428 6932 2920 2a20 3336 350d 0a20 2020  t(i2) * 365..   
-000016b0: 2020 2020 2079 6561 7273 3220 3d20 696e       years2 = in
-000016c0: 7428 7965 6172 5f69 6e5f 6461 7973 290d  t(year_in_days).
-000016d0: 0a20 2020 2020 2020 206d 6f6e 7468 7332  .        months2
-000016e0: 203d 2069 6e74 286a 3229 202a 2033 300d   = int(j2) * 30.
-000016f0: 0a20 2020 2020 2020 2064 6179 7332 203d  .        days2 =
-00001700: 2069 6e74 286b 3229 0d0a 0d0a 2020 2020   int(k2)....    
-00001710: 2020 2020 6966 2073 656c 662e 7469 6d65      if self.time
-00001720: 5f20 3d3d 2027 6d27 206f 7220 7365 6c66  _ == 'm' or self
-00001730: 2e74 696d 655f 203d 3d20 276d 273a 0d0a  .time_ == 'm':..
-00001740: 2020 2020 2020 2020 2020 2020 6765 745f              get_
-00001750: 6d69 6e73 203d 2028 7965 6172 7320 2b20  mins = (years + 
-00001760: 6d6f 6e74 6873 202b 2064 6179 7329 202a  months + days) *
-00001770: 2032 3420 2a20 3630 0d0a 2020 2020 2020   24 * 60..      
-00001780: 2020 2020 2020 6765 745f 6d69 6e73 3220        get_mins2 
-00001790: 3d20 2879 6561 7273 3220 2b20 6d6f 6e74  = (years2 + mont
-000017a0: 6873 3220 2b20 6461 7973 3229 202a 2032  hs2 + days2) * 2
-000017b0: 3420 2a20 3630 0d0a 2020 2020 2020 2020  4 * 60..        
-000017c0: 2020 2020 7265 7475 726e 2067 6574 5f6d      return get_m
-000017d0: 696e 7320 2d20 6765 745f 6d69 6e73 320d  ins - get_mins2.
-000017e0: 0a20 2020 2020 2020 2065 6c69 6620 7365  .        elif se
-000017f0: 6c66 2e74 696d 655f 203d 3d20 2768 2720  lf.time_ == 'h' 
-00001800: 6f72 2073 656c 662e 7469 6d65 5f20 3d3d  or self.time_ ==
-00001810: 2027 4827 3a0d 0a20 2020 2020 2020 2020   'H':..         
-00001820: 2020 2067 6574 5f6d 696e 7320 3d20 2879     get_mins = (y
-00001830: 6561 7273 202b 206d 6f6e 7468 7320 2b20  ears + months + 
-00001840: 6461 7973 2920 2a20 3234 202a 2036 300d  days) * 24 * 60.
-00001850: 0a20 2020 2020 2020 2020 2020 2067 6574  .            get
-00001860: 5f6d 696e 7332 203d 2028 7965 6172 7332  _mins2 = (years2
-00001870: 202b 206d 6f6e 7468 7332 202b 2064 6179   + months2 + day
-00001880: 7332 2920 2a20 3234 202a 2036 300d 0a20  s2) * 24 * 60.. 
-00001890: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-000018a0: 6e20 726f 756e 6428 2867 6574 5f6d 696e  n round((get_min
-000018b0: 7320 2d20 6765 745f 6d69 6e73 3229 202f  s - get_mins2) /
-000018c0: 2036 302c 2032 290d 0a20 2020 2020 2020   60, 2)..       
-000018d0: 2065 6c69 6620 7365 6c66 2e74 696d 655f   elif self.time_
-000018e0: 203d 3d20 2764 2720 6f72 2073 656c 662e   == 'd' or self.
-000018f0: 7469 6d65 5f20 3d3d 2027 4427 3a0d 0a20  time_ == 'D':.. 
-00001900: 2020 2020 2020 2020 2020 2067 6574 5f64             get_d
-00001910: 6179 7320 3d20 7965 6172 7320 2b20 6d6f  ays = years + mo
-00001920: 6e74 6873 202b 2064 6179 730d 0a20 2020  nths + days..   
-00001930: 2020 2020 2020 2020 2067 6574 5f64 6179           get_day
-00001940: 7332 203d 2079 6561 7273 3220 2b20 6d6f  s2 = years2 + mo
-00001950: 6e74 6873 3220 2b20 6461 7973 320d 0a20  nths2 + days2.. 
-00001960: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00001970: 6e20 6765 745f 6461 7973 202d 2067 6574  n get_days - get
-00001980: 5f64 6179 7332 0d0a 2020 2020 2020 2020  _days2..        
-00001990: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
-000019a0: 2020 2067 6574 5f73 6563 7320 3d20 2879     get_secs = (y
-000019b0: 6561 7273 202b 206d 6f6e 7468 7320 2b20  ears + months + 
-000019c0: 6461 7973 2920 2a20 3234 202a 2036 3020  days) * 24 * 60 
-000019d0: 2a20 3630 0d0a 2020 2020 2020 2020 2020  * 60..          
-000019e0: 2020 6765 745f 7365 6373 3220 3d20 2879    get_secs2 = (y
-000019f0: 6561 7273 3220 2b20 6d6f 6e74 6873 3220  ears2 + months2 
-00001a00: 2b20 6461 7973 3229 202a 2032 3420 2a20  + days2) * 24 * 
-00001a10: 3630 202a 2036 300d 0a20 2020 2020 2020  60 * 60..       
-00001a20: 2020 2020 2072 6574 7572 6e20 6765 745f       return get_
-00001a30: 7365 6373 202d 2067 6574 5f73 6563 7332  secs - get_secs2
-00001a40: 0d0a 0d0a                                ....
+000000a0: 636f 6e76 6572 745f 7469 6d65 2873 656c  convert_time(sel
+000000b0: 6629 3a0d 0a20 2020 2020 2020 2073 6c75  f):..        slu
+000000c0: 675f 7469 6d65 203d 2073 7472 2873 656c  g_time = str(sel
+000000d0: 662e 7469 6d65 290d 0a20 2020 2020 2020  f.time)..       
+000000e0: 2066 6972 7374 203d 2073 6c75 675f 7469   first = slug_ti
+000000f0: 6d65 2e73 706c 6974 2822 2d22 290d 0a20  me.split("-").. 
+00000100: 2020 2020 2020 2073 6563 6f6e 6420 3d20         second = 
+00000110: 6669 7273 745b 303a 325d 0d0a 2020 2020  first[0:2]..    
+00000120: 2020 2020 7468 6972 6420 3d20 6669 7273      third = firs
+00000130: 745b 325d 0d0a 2020 2020 2020 2020 666f  t[2]..        fo
+00000140: 7572 7468 203d 2074 6869 7264 2e73 706c  urth = third.spl
+00000150: 6974 2822 2022 295b 315d 2e73 706c 6974  it(" ")[1].split
+00000160: 2822 3a22 290d 0a20 2020 2020 2020 2069  (":")..        i
+00000170: 203d 2073 6563 6f6e 645b 305d 0d0a 2020   = second[0]..  
+00000180: 2020 2020 2020 6a20 3d20 7365 636f 6e64        j = second
+00000190: 5b31 5d0d 0a20 2020 2020 2020 206b 203d  [1]..        k =
+000001a0: 2074 6869 7264 2e73 706c 6974 2822 2022   third.split(" "
+000001b0: 295b 305d 0d0a 2020 2020 2020 2020 6872  )[0]..        hr
+000001c0: 7320 3d20 696e 7428 666f 7572 7468 5b30  s = int(fourth[0
+000001d0: 5d29 0d0a 2020 2020 2020 2020 6d69 6e73  ])..        mins
+000001e0: 203d 2069 6e74 2866 6f75 7274 685b 315d   = int(fourth[1]
+000001f0: 290d 0a20 2020 2020 2020 2073 6563 7320  )..        secs 
+00000200: 3d20 666f 7572 7468 5b32 5d2e 7370 6c69  = fourth[2].spli
+00000210: 7428 222e 2229 5b30 5d0d 0a20 2020 2020  t(".")[0]..     
+00000220: 2020 2069 6620 272b 2720 696e 2073 6563     if '+' in sec
+00000230: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
+00000240: 7365 6373 203d 2073 6563 732e 7370 6c69  secs = secs.spli
+00000250: 7428 272b 2729 5b30 5d0d 0a20 2020 2020  t('+')[0]..     
+00000260: 2020 2073 6563 735f 696e 7420 3d20 696e     secs_int = in
+00000270: 7428 7365 6373 290d 0a20 2020 2020 2020  t(secs)..       
+00000280: 2079 6561 725f 696e 5f64 6179 7320 3d20   year_in_days = 
+00000290: 696e 7428 6929 202a 2033 3635 0d0a 2020  int(i) * 365..  
+000002a0: 2020 2020 2020 7965 6172 7320 3d20 696e        years = in
+000002b0: 7428 7965 6172 5f69 6e5f 6461 7973 290d  t(year_in_days).
+000002c0: 0a20 2020 2020 2020 206d 6f6e 7468 7320  .        months 
+000002d0: 3d20 696e 7428 6a29 202a 2033 300d 0a20  = int(j) * 30.. 
+000002e0: 2020 2020 2020 2064 6179 7320 3d20 696e         days = in
+000002f0: 7428 6b29 0d0a 2020 2020 2020 2020 6966  t(k)..        if
+00000300: 2073 656c 662e 7469 6d65 5f20 3d3d 2027   self.time_ == '
+00000310: 6d27 3a0d 0a20 2020 2020 2020 2020 2020  m':..           
+00000320: 2067 6574 5f64 6179 735f 6d69 6e73 203d   get_days_mins =
+00000330: 2028 6872 7320 2a20 3630 2920 2b20 6d69   (hrs * 60) + mi
+00000340: 6e73 0d0a 2020 2020 2020 2020 2020 2020  ns..            
+00000350: 6765 745f 7965 6172 735f 6d69 6e73 203d  get_years_mins =
+00000360: 2028 7965 6172 7320 2b20 6d6f 6e74 6873   (years + months
+00000370: 202b 2064 6179 7329 202a 2032 3420 2a20   + days) * 24 * 
+00000380: 3630 0d0a 2020 2020 2020 2020 2020 2020  60..            
+00000390: 7265 7475 726e 2067 6574 5f79 6561 7273  return get_years
+000003a0: 5f6d 696e 7320 2b20 6765 745f 6461 7973  _mins + get_days
+000003b0: 5f6d 696e 730d 0a20 2020 2020 2020 2065  _mins..        e
+000003c0: 6c69 6620 7365 6c66 2e74 696d 655f 203d  lif self.time_ =
+000003d0: 3d20 2768 273a 0d0a 2020 2020 2020 2020  = 'h':..        
+000003e0: 2020 2020 6765 745f 6461 7973 5f6d 696e      get_days_min
+000003f0: 7320 3d20 2868 7273 202a 2036 3029 202b  s = (hrs * 60) +
+00000400: 206d 696e 730d 0a20 2020 2020 2020 2020   mins..         
+00000410: 2020 2067 6574 5f79 6561 7273 5f6d 696e     get_years_min
+00000420: 7320 3d20 2879 6561 7273 202b 206d 6f6e  s = (years + mon
+00000430: 7468 7320 2b20 6461 7973 2920 2a20 3234  ths + days) * 24
+00000440: 202a 2036 300d 0a20 2020 2020 2020 2020   * 60..         
+00000450: 2020 2072 6574 7572 6e20 726f 756e 6428     return round(
+00000460: 2867 6574 5f79 6561 7273 5f6d 696e 7320  (get_years_mins 
+00000470: 2b20 6765 745f 6461 7973 5f6d 696e 7329  + get_days_mins)
+00000480: 202f 2036 302c 2032 290d 0a20 2020 2020   / 60, 2)..     
+00000490: 2020 2065 6c69 6620 7365 6c66 2e74 696d     elif self.tim
+000004a0: 655f 203d 3d20 2764 273a 0d0a 2020 2020  e_ == 'd':..    
+000004b0: 2020 2020 2020 2020 6765 745f 7965 6172          get_year
+000004c0: 735f 6461 7973 203d 2079 6561 7273 202b  s_days = years +
+000004d0: 206d 6f6e 7468 7320 2b20 6461 7973 0d0a   months + days..
+000004e0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+000004f0: 726e 2067 6574 5f79 6561 7273 5f64 6179  rn get_years_day
+00000500: 730d 0a20 2020 2020 2020 2065 6c73 653a  s..        else:
+00000510: 0d0a 2020 2020 2020 2020 2020 2020 6765  ..            ge
+00000520: 745f 6461 7973 5f73 6563 7320 3d20 2868  t_days_secs = (h
+00000530: 7273 202a 2036 3020 2a20 3630 2920 2b20  rs * 60 * 60) + 
+00000540: 286d 696e 7320 2a20 3630 2920 2b20 7365  (mins * 60) + se
+00000550: 6373 5f69 6e74 0d0a 2020 2020 2020 2020  cs_int..        
+00000560: 2020 2020 6765 745f 7965 6172 735f 7365      get_years_se
+00000570: 6373 203d 2028 7965 6172 7320 2b20 6d6f  cs = (years + mo
+00000580: 6e74 6873 202b 2064 6179 7329 202a 2032  nths + days) * 2
+00000590: 3420 2a20 3630 202a 2036 300d 0a20 2020  4 * 60 * 60..   
+000005a0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+000005b0: 6765 745f 7965 6172 735f 7365 6373 202b  get_years_secs +
+000005c0: 2067 6574 5f64 6179 735f 7365 6373 0d0a   get_days_secs..
+000005d0: 0d0a 2020 2020 4070 726f 7065 7274 790d  ..    @property.
+000005e0: 0a20 2020 2064 6566 2063 6f6e 7665 7274  .    def convert
+000005f0: 2873 656c 6629 3a0d 0a20 2020 2020 2020  (self):..       
+00000600: 2073 6c75 675f 7469 6d65 3a20 7374 7220   slug_time: str 
+00000610: 3d20 7374 7228 7365 6c66 2e74 696d 6529  = str(self.time)
+00000620: 0d0a 2020 2020 2020 2020 6669 7273 7420  ..        first 
+00000630: 3d20 736c 7567 5f74 696d 652e 7370 6c69  = slug_time.spli
+00000640: 7428 222d 2229 0d0a 2020 2020 2020 2020  t("-")..        
+00000650: 7365 636f 6e64 203d 2066 6972 7374 5b30  second = first[0
+00000660: 3a32 5d0d 0a20 2020 2020 2020 2074 6869  :2]..        thi
+00000670: 7264 203d 2066 6972 7374 5b32 5d0d 0a20  rd = first[2].. 
+00000680: 2020 2020 2020 2069 203d 2073 6563 6f6e         i = secon
+00000690: 645b 305d 0d0a 2020 2020 2020 2020 6a20  d[0]..        j 
+000006a0: 3d20 7365 636f 6e64 5b31 5d0d 0a20 2020  = second[1]..   
+000006b0: 2020 2020 206b 203d 2074 6869 7264 2e73       k = third.s
+000006c0: 706c 6974 2822 2022 295b 305d 0d0a 2020  plit(" ")[0]..  
+000006d0: 2020 2020 2020 7965 6172 5f69 6e5f 6461        year_in_da
+000006e0: 7973 203d 2069 6e74 2869 2920 2a20 3336  ys = int(i) * 36
+000006f0: 350d 0a20 2020 2020 2020 2079 6561 7273  5..        years
+00000700: 203d 2069 6e74 2879 6561 725f 696e 5f64   = int(year_in_d
+00000710: 6179 7329 0d0a 2020 2020 2020 2020 6d6f  ays)..        mo
+00000720: 6e74 6873 203d 2069 6e74 286a 2920 2a20  nths = int(j) * 
+00000730: 3330 0d0a 2020 2020 2020 2020 6461 7973  30..        days
+00000740: 203d 2069 6e74 286b 290d 0a20 2020 2020   = int(k)..     
+00000750: 2020 2069 6620 7365 6c66 2e74 696d 655f     if self.time_
+00000760: 203d 3d20 276d 273a 0d0a 2020 2020 2020   == 'm':..      
+00000770: 2020 2020 2020 6765 745f 6d69 6e73 203d        get_mins =
+00000780: 2028 7965 6172 7320 2b20 6d6f 6e74 6873   (years + months
+00000790: 202b 2064 6179 7329 202a 2032 3420 2a20   + days) * 24 * 
+000007a0: 3630 0d0a 2020 2020 2020 2020 2020 2020  60..            
+000007b0: 7265 7475 726e 2067 6574 5f6d 696e 730d  return get_mins.
+000007c0: 0a20 2020 2020 2020 2065 6c69 6620 7365  .        elif se
+000007d0: 6c66 2e74 696d 655f 203d 3d20 2768 273a  lf.time_ == 'h':
+000007e0: 0d0a 2020 2020 2020 2020 2020 2020 6765  ..            ge
+000007f0: 745f 6872 7320 3d20 726f 756e 6428 2828  t_hrs = round(((
+00000800: 7965 6172 7320 2b20 6d6f 6e74 6873 202b  years + months +
+00000810: 2064 6179 7329 202a 2032 3420 2a20 3630   days) * 24 * 60
+00000820: 2920 2f20 3630 2c20 3229 0d0a 2020 2020  ) / 60, 2)..    
+00000830: 2020 2020 2020 2020 7265 7475 726e 2067          return g
+00000840: 6574 5f68 7273 0d0a 2020 2020 2020 2020  et_hrs..        
+00000850: 656c 6966 2073 656c 662e 7469 6d65 5f20  elif self.time_ 
+00000860: 3d3d 2027 6427 3a0d 0a20 2020 2020 2020  == 'd':..       
+00000870: 2020 2020 2067 6574 5f64 6179 7320 3d20       get_days = 
+00000880: 7965 6172 7320 2b20 6d6f 6e74 6873 202b  years + months +
+00000890: 2064 6179 730d 0a20 2020 2020 2020 2020   days..         
+000008a0: 2020 2072 6574 7572 6e20 6765 745f 6461     return get_da
+000008b0: 7973 0d0a 2020 2020 2020 2020 656c 7365  ys..        else
+000008c0: 3a0d 0a20 2020 2020 2020 2020 2020 2067  :..            g
+000008d0: 6574 5f73 6563 7320 3d20 2879 6561 7273  et_secs = (years
+000008e0: 202b 206d 6f6e 7468 7320 2b20 6461 7973   + months + days
+000008f0: 2920 2a20 3234 202a 2036 3020 2a20 3630  ) * 24 * 60 * 60
+00000900: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
+00000910: 7475 726e 2067 6574 5f73 6563 730d 0a0d  turn get_secs...
+00000920: 0a0d 0a63 6c61 7373 2044 6174 6544 6966  ...class DateDif
+00000930: 663a 0d0a 2020 2020 6465 6620 5f5f 696e  f:..    def __in
+00000940: 6974 5f5f 2873 656c 662c 2074 696d 6531  it__(self, time1
+00000950: 2c20 7469 6d65 322c 2074 696d 655f 666f  , time2, time_fo
+00000960: 726d 6174 3d27 7327 293a 0d0a 2020 2020  rmat='s'):..    
+00000970: 2020 2020 7365 6c66 2e74 696d 6531 203d      self.time1 =
+00000980: 2074 696d 6531 0d0a 2020 2020 2020 2020   time1..        
+00000990: 7365 6c66 2e74 696d 6532 203d 2074 696d  self.time2 = tim
+000009a0: 6532 0d0a 2020 2020 2020 2020 7365 6c66  e2..        self
+000009b0: 2e74 696d 655f 203d 2074 696d 655f 666f  .time_ = time_fo
+000009c0: 726d 6174 0d0a 0d0a 2020 2020 6465 6620  rmat....    def 
+000009d0: 5f67 6574 5f79 6561 725f 6d6f 6e74 685f  _get_year_month_
+000009e0: 6461 7928 7365 6c66 2c20 736c 7567 5f74  day(self, slug_t
+000009f0: 696d 6529 3a0d 0a20 2020 2020 2020 2066  ime):..        f
+00000a00: 6972 7374 203d 2073 6c75 675f 7469 6d65  irst = slug_time
+00000a10: 2e73 706c 6974 2822 2d22 290d 0a20 2020  .split("-")..   
+00000a20: 2020 2020 2073 6563 6f6e 6420 3d20 6669       second = fi
+00000a30: 7273 745b 303a 325d 0d0a 2020 2020 2020  rst[0:2]..      
+00000a40: 2020 7468 6972 6420 3d20 6669 7273 745b    third = first[
+00000a50: 325d 2e73 706c 6974 2822 2022 295b 305d  2].split(" ")[0]
+00000a60: 0d0a 2020 2020 2020 2020 7965 6172 5f69  ..        year_i
+00000a70: 6e5f 6461 7973 203d 2069 6e74 2873 6563  n_days = int(sec
+00000a80: 6f6e 645b 305d 2920 2a20 3336 350d 0a20  ond[0]) * 365.. 
+00000a90: 2020 2020 2020 2079 6561 7273 203d 2079         years = y
+00000aa0: 6561 725f 696e 5f64 6179 7320 2f2f 2033  ear_in_days // 3
+00000ab0: 3635 0d0a 2020 2020 2020 2020 6d6f 6e74  65..        mont
+00000ac0: 6873 203d 2069 6e74 2873 6563 6f6e 645b  hs = int(second[
+00000ad0: 315d 2920 2a20 3330 0d0a 2020 2020 2020  1]) * 30..      
+00000ae0: 2020 6461 7973 203d 2069 6e74 2874 6869    days = int(thi
+00000af0: 7264 290d 0a20 2020 2020 2020 2072 6574  rd)..        ret
+00000b00: 7572 6e20 7965 6172 732c 206d 6f6e 7468  urn years, month
+00000b10: 732c 2064 6179 730d 0a0d 0a20 2020 2064  s, days....    d
+00000b20: 6566 205f 6765 745f 686f 7572 735f 6d69  ef _get_hours_mi
+00000b30: 6e75 7465 735f 7365 636f 6e64 7328 7365  nutes_seconds(se
+00000b40: 6c66 2c20 736c 7567 5f74 696d 6529 3a0d  lf, slug_time):.
+00000b50: 0a20 2020 2020 2020 2066 6f75 7274 6820  .        fourth 
+00000b60: 3d20 736c 7567 5f74 696d 652e 7370 6c69  = slug_time.spli
+00000b70: 7428 2220 2229 5b31 5d2e 7370 6c69 7428  t(" ")[1].split(
+00000b80: 223a 2229 0d0a 2020 2020 2020 2020 6872  ":")..        hr
+00000b90: 7320 3d20 696e 7428 666f 7572 7468 5b30  s = int(fourth[0
+00000ba0: 5d29 0d0a 2020 2020 2020 2020 6d69 6e73  ])..        mins
+00000bb0: 203d 2069 6e74 2866 6f75 7274 685b 315d   = int(fourth[1]
+00000bc0: 290d 0a20 2020 2020 2020 2073 6563 7320  )..        secs 
+00000bd0: 3d20 666f 7572 7468 5b32 5d2e 7370 6c69  = fourth[2].spli
+00000be0: 7428 222e 2229 5b30 5d0d 0a20 2020 2020  t(".")[0]..     
+00000bf0: 2020 2069 6620 272b 2720 696e 2073 6563     if '+' in sec
+00000c00: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
+00000c10: 7365 6373 203d 2073 6563 732e 7370 6c69  secs = secs.spli
+00000c20: 7428 272b 2729 5b30 5d0d 0a20 2020 2020  t('+')[0]..     
+00000c30: 2020 2073 6563 735f 696e 7420 3d20 696e     secs_int = in
+00000c40: 7428 7365 6373 290d 0a20 2020 2020 2020  t(secs)..       
+00000c50: 2072 6574 7572 6e20 6872 732c 206d 696e   return hrs, min
+00000c60: 732c 2073 6563 735f 696e 740d 0a0d 0a20  s, secs_int.... 
+00000c70: 2020 2040 7072 6f70 6572 7479 0d0a 2020     @property..  
+00000c80: 2020 6465 6620 6461 7465 5f74 696d 655f    def date_time_
+00000c90: 6469 6666 2873 656c 6629 3a0d 0a20 2020  diff(self):..   
+00000ca0: 2020 2020 2023 2074 696d 6520 310d 0a20       # time 1.. 
+00000cb0: 2020 2020 2020 2079 6561 7273 2c20 6d6f         years, mo
+00000cc0: 6e74 6873 2c20 6461 7973 203d 2073 656c  nths, days = sel
+00000cd0: 662e 5f67 6574 5f79 6561 725f 6d6f 6e74  f._get_year_mont
+00000ce0: 685f 6461 7928 7374 7228 7365 6c66 2e74  h_day(str(self.t
+00000cf0: 696d 6531 2929 0d0a 2020 2020 2020 2020  ime1))..        
+00000d00: 6872 732c 206d 696e 732c 2073 6563 735f  hrs, mins, secs_
+00000d10: 696e 7420 3d20 7365 6c66 2e5f 6765 745f  int = self._get_
+00000d20: 686f 7572 735f 6d69 6e75 7465 735f 7365  hours_minutes_se
+00000d30: 636f 6e64 7328 7374 7228 7365 6c66 2e74  conds(str(self.t
+00000d40: 696d 6531 2929 0d0a 0d0a 2020 2020 2020  ime1))....      
+00000d50: 2020 2320 7469 6d65 2032 0d0a 2020 2020    # time 2..    
+00000d60: 2020 2020 7965 6172 7332 2c20 6d6f 6e74      years2, mont
+00000d70: 6873 322c 2064 6179 7332 203d 2073 656c  hs2, days2 = sel
+00000d80: 662e 5f67 6574 5f79 6561 725f 6d6f 6e74  f._get_year_mont
+00000d90: 685f 6461 7928 7374 7228 7365 6c66 2e74  h_day(str(self.t
+00000da0: 696d 6532 2929 0d0a 2020 2020 2020 2020  ime2))..        
+00000db0: 6872 7332 2c20 6d69 6e73 322c 2073 6563  hrs2, mins2, sec
+00000dc0: 735f 696e 7432 203d 2073 656c 662e 5f67  s_int2 = self._g
+00000dd0: 6574 5f68 6f75 7273 5f6d 696e 7574 6573  et_hours_minutes
+00000de0: 5f73 6563 6f6e 6473 2873 7472 2873 656c  _seconds(str(sel
+00000df0: 662e 7469 6d65 3229 290d 0a0d 0a20 2020  f.time2))....   
+00000e00: 2020 2020 2069 6620 7365 6c66 2e74 696d       if self.tim
+00000e10: 655f 203d 3d20 276d 2720 6f72 2073 656c  e_ == 'm' or sel
+00000e20: 662e 7469 6d65 5f20 3d3d 2027 4d27 3a0d  f.time_ == 'M':.
+00000e30: 0a20 2020 2020 2020 2020 2020 2067 6574  .            get
+00000e40: 5f64 6179 735f 6d69 6e73 203d 2028 6872  _days_mins = (hr
+00000e50: 7320 2a20 3630 2920 2b20 6d69 6e73 0d0a  s * 60) + mins..
+00000e60: 2020 2020 2020 2020 2020 2020 6765 745f              get_
+00000e70: 7965 6172 735f 6d69 6e73 203d 2028 7965  years_mins = (ye
+00000e80: 6172 7320 2b20 6d6f 6e74 6873 202b 2064  ars + months + d
+00000e90: 6179 7329 202a 2032 3420 2a20 3630 0d0a  ays) * 24 * 60..
+00000ea0: 2020 2020 2020 2020 2020 2020 6765 745f              get_
+00000eb0: 6461 7973 5f6d 696e 7332 203d 2028 6872  days_mins2 = (hr
+00000ec0: 7332 202a 2036 3029 202b 206d 696e 7332  s2 * 60) + mins2
+00000ed0: 0d0a 2020 2020 2020 2020 2020 2020 6765  ..            ge
+00000ee0: 745f 7965 6172 735f 6d69 6e73 3220 3d20  t_years_mins2 = 
+00000ef0: 2879 6561 7273 3220 2b20 6d6f 6e74 6873  (years2 + months
+00000f00: 3220 2b20 6461 7973 3229 202a 2032 3420  2 + days2) * 24 
+00000f10: 2a20 3630 0d0a 2020 2020 2020 2020 2020  * 60..          
+00000f20: 2020 7265 7475 726e 2028 6765 745f 7965    return (get_ye
+00000f30: 6172 735f 6d69 6e73 202b 2067 6574 5f64  ars_mins + get_d
+00000f40: 6179 735f 6d69 6e73 2920 2d20 2867 6574  ays_mins) - (get
+00000f50: 5f79 6561 7273 5f6d 696e 7332 202b 2067  _years_mins2 + g
+00000f60: 6574 5f64 6179 735f 6d69 6e73 3229 0d0a  et_days_mins2)..
+00000f70: 2020 2020 2020 2020 656c 6966 2073 656c          elif sel
+00000f80: 662e 7469 6d65 5f20 3d3d 2027 6827 206f  f.time_ == 'h' o
+00000f90: 7220 7365 6c66 2e74 696d 655f 203d 3d20  r self.time_ == 
+00000fa0: 2748 273a 0d0a 2020 2020 2020 2020 2020  'H':..          
+00000fb0: 2020 6765 745f 6461 7973 5f6d 696e 7320    get_days_mins 
+00000fc0: 3d20 2868 7273 202a 2036 3029 202b 206d  = (hrs * 60) + m
+00000fd0: 696e 730d 0a20 2020 2020 2020 2020 2020  ins..           
+00000fe0: 2067 6574 5f79 6561 7273 5f6d 696e 7320   get_years_mins 
+00000ff0: 3d20 2879 6561 7273 202b 206d 6f6e 7468  = (years + month
+00001000: 7320 2b20 6461 7973 2920 2a20 3234 202a  s + days) * 24 *
+00001010: 2036 300d 0a20 2020 2020 2020 2020 2020   60..           
+00001020: 2067 6574 5f64 6179 735f 6d69 6e73 3220   get_days_mins2 
+00001030: 3d20 2868 7273 3220 2a20 3630 2920 2b20  = (hrs2 * 60) + 
+00001040: 6d69 6e73 320d 0a20 2020 2020 2020 2020  mins2..         
+00001050: 2020 2067 6574 5f79 6561 7273 5f6d 696e     get_years_min
+00001060: 7332 203d 2028 7965 6172 7332 202b 206d  s2 = (years2 + m
+00001070: 6f6e 7468 7332 202b 2064 6179 7332 2920  onths2 + days2) 
+00001080: 2a20 3234 202a 2036 300d 0a20 2020 2020  * 24 * 60..     
+00001090: 2020 2020 2020 2072 6574 7572 6e20 726f         return ro
+000010a0: 756e 6428 2867 6574 5f79 6561 7273 5f6d  und((get_years_m
+000010b0: 696e 7320 2b20 6765 745f 6461 7973 5f6d  ins + get_days_m
+000010c0: 696e 7329 202d 2028 6765 745f 7965 6172  ins) - (get_year
+000010d0: 735f 6d69 6e73 3220 2b20 6765 745f 6461  s_mins2 + get_da
+000010e0: 7973 5f6d 696e 7332 2920 2f20 3630 2c20  ys_mins2) / 60, 
+000010f0: 3229 0d0a 2020 2020 2020 2020 656c 6966  2)..        elif
+00001100: 2073 656c 662e 7469 6d65 5f20 3d3d 2027   self.time_ == '
+00001110: 6427 206f 7220 7365 6c66 2e74 696d 655f  d' or self.time_
+00001120: 203d 3d20 2744 273a 0d0a 2020 2020 2020   == 'D':..      
+00001130: 2020 2020 2020 6765 745f 6461 7973 203d        get_days =
+00001140: 2079 6561 7273 202b 206d 6f6e 7468 7320   years + months 
+00001150: 2b20 6461 7973 0d0a 2020 2020 2020 2020  + days..        
+00001160: 2020 2020 6765 745f 6461 7973 3220 3d20      get_days2 = 
+00001170: 7965 6172 7332 202b 206d 6f6e 7468 7332  years2 + months2
+00001180: 202b 2064 6179 7332 0d0a 2020 2020 2020   + days2..      
+00001190: 2020 2020 2020 7265 7475 726e 2067 6574        return get
+000011a0: 5f64 6179 7320 2d20 6765 745f 6461 7973  _days - get_days
+000011b0: 320d 0a20 2020 2020 2020 2065 6c73 653a  2..        else:
+000011c0: 0d0a 2020 2020 2020 2020 2020 2020 6765  ..            ge
+000011d0: 745f 6461 7973 5f73 6563 7320 3d20 2868  t_days_secs = (h
+000011e0: 7273 202a 2036 3020 2a20 3630 2920 2b20  rs * 60 * 60) + 
+000011f0: 286d 696e 7320 2a20 3630 2920 2b20 7365  (mins * 60) + se
+00001200: 6373 5f69 6e74 0d0a 2020 2020 2020 2020  cs_int..        
+00001210: 2020 2020 6765 745f 7965 6172 735f 7365      get_years_se
+00001220: 6373 203d 2028 7965 6172 7320 2b20 6d6f  cs = (years + mo
+00001230: 6e74 6873 202b 2064 6179 7329 202a 2032  nths + days) * 2
+00001240: 3420 2a20 3630 202a 2036 300d 0a20 2020  4 * 60 * 60..   
+00001250: 2020 2020 2020 2020 2067 6574 5f64 6179           get_day
+00001260: 735f 7365 6373 3220 3d20 2868 7273 3220  s_secs2 = (hrs2 
+00001270: 2a20 3630 202a 2036 3029 202b 2028 6d69  * 60 * 60) + (mi
+00001280: 6e73 3220 2a20 3630 2920 2b20 7365 6373  ns2 * 60) + secs
+00001290: 5f69 6e74 320d 0a20 2020 2020 2020 2020  _int2..         
+000012a0: 2020 2067 6574 5f79 6561 7273 5f73 6563     get_years_sec
+000012b0: 7332 203d 2028 7965 6172 7332 202b 206d  s2 = (years2 + m
+000012c0: 6f6e 7468 7332 202b 2064 6179 7332 2920  onths2 + days2) 
+000012d0: 2a20 3234 202a 2036 3020 2a20 3630 0d0a  * 24 * 60 * 60..
+000012e0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+000012f0: 726e 2067 6574 5f79 6561 7273 5f73 6563  rn get_years_sec
+00001300: 7320 2b20 6765 745f 6461 7973 5f73 6563  s + get_days_sec
+00001310: 730d 0a0d 0a0d 0a                        s......
```

### Comparing `date_time_literal-1.0.8/date_time_literal/main.py` & `date_time_literal-1.1.0/date_time_literal/main.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,21 +3,24 @@
 from difference import date_diff, convert_time, date_time_diff
 
 if __name__ == "__main__":
     t = ConvertTime('2021-05-31 23:16:55.321568', 'd')
     p = ConvertTime(datetime.now(), 'd')
     i = ConvertTime('2021-05-31 23:16:55+00:00', 'd')
     d = ConvertTime('2021-05-31', time_format='d')
-    e = DateDiff('2021-05-31 23:16:55+00:00', '2021-04-30 23:16:55+00:00', 'h')
-    print(t.slug_date_time)
-    print(i.slug_date_time)
-    print(d.slug_date)
-    print(e.date_diff)
-    print(date_time_diff('2021-04-30 21:56:50+00:00', '2021-04-30 10:58:55+00:00', 'm'))
-    print(convert_time(1, "w", 'y'))
+    e = DateDiff('2021-05-31 23:16:55+00:00', '2021-04-30 23:16:55+00:00', 'D')
+    print(t.convert)
+    print(i.convert_time)
+    print(p.convert)
+    print(d.convert)
+    print(d.convert)
+    print(e.date_time_diff)
+    print(date_time_diff('2021-04-30 21:58:50+00:00', '2021-04-30 10:58:55+00:00', 'H'))
+    print(date_diff('2021-06-30', '2021-05-30', 'H'))
+    print(convert_time(1, "y", 'w'))
```

### Comparing `date_time_literal-1.0.8/date_time_literal.egg-info/PKG-INFO` & `date_time_literal-1.1.0/date_time_literal.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: date-time-literal
-Version: 1.0.8
+Version: 1.1.0
 Summary: date-time-literal is a python module that helps convert date-time or date to literal days, hours, seconds, or even minutes. Compare two DateTime or Date objects, by converting the objects to literal days, hours, minutes, or even seconds if you want to be precise. 
 Home-page: https://github.com/kells4real/date_literal
 Download-URL: https://github.com/kells4real/date_literal/archive/refs/tags/1.0.0.tar.gz
 Author: Kelvin Sajere
 Author-email: kells4real@gmail.com
 Keywords: date-time,date,literal,date converter,literal date,date-time converter,django,python,module,python package,date-time literal,convert time,convert date-time
 Classifier: Programming Language :: Python :: 3
@@ -27,75 +27,75 @@
 DateTime or Date objects must be in the default 'Y-M-D Hr:Min:Sec' and 'Y-M-D' formats respectively.
 
 ##### Converts Date Time Literal
 ```python
 from django.utils import timezone
 time = timezone.now()
 from date_time_literal import ConvertTime
-convert_time = ConvertTime(time).slug_date_time
+convert_time = ConvertTime(time).convert_time
 ```
 ##### Converts Date Literal
-convert_time = ConvertTime(time).slug_date
-This returns the date or date-time in seconds. You can add an optional parameter to specify what you want.
+convert_time = ConvertTime(time).convert
+This returns the date or date_time in seconds. You can add an optional parameter to specify what you want.
 
-Note: You can use the slug_date class function on a DateTime object if you wish to use only the date part of the DateTime object, 
-but cannot use the slug_date_time class function on a Date object, only on DateTime objects.
+Note: You can use the convert class function on a DateTime object if you wish to use only the date part of the DateTime object, 
+but cannot use the convert_time class function on a Date object, only on DateTime objects.
 
 #### Specific conversion to days
 
 ```python
 from django.utils import timezone
 from datetime import datetime
 from date_time_literal import ConvertTime
 
 time2 = datetime.now()
 time = timezone.now()
 
-convert_time = ConvertTime(time, 'd').slug_date_time
-convert_time2 = ConvertTime(time2, 'd').slug_date
+convert_time = ConvertTime(time, 'd').convert_time
+convert_time2 = ConvertTime(time2, 'd').convert
 ```
 
 #### Specific conversion to hours
 
 ```python
 from date_time_literal import ConvertTime
 from datetime import datetime
 time = datetime.now()
-convert_time = ConvertTime(time, 'd').slug_date_time # Converts the DateTime object to days
-convert_time1 = ConvertTime(time, 'h').slug_date_time # Converts the DateTime object to hours
-convert_time2 = ConvertTime(time, 'm').slug_date_time # Converts the DateTime object to minutes
+convert_time = ConvertTime(time, 'd').convert_time # Converts the DateTime object to days
+convert_time1 = ConvertTime(time, 'h').convert_time # Converts the DateTime object to hours
+convert_time2 = ConvertTime(time, 'm').convert_time # Converts the DateTime object to minutes
 
 # The default conversion if none is specified is to seconds
 ```
 
-### CHECK DATE-TIME OR DATE DIFFERENCE BETWEEN TWO DATE-TIME OR DATE LITERALS
+### CHECK DATE-TIME OR DATE DIFFERENCE BETWEEN TWO DATE-TIME OR DATE OBJECTS
 
 ```python
 from date_time_literal import ConvertTime
 from datetime import datetime
 from django.utils import timezone
 time = datetime.now()
-convert_time = ConvertTime(time, 'h').slug_date_time
+convert_time = ConvertTime(time, 'h').convert_time
 from date_time_literal import date_time_diff, date_diff
-convert_time2 = ConvertTime(time, 'm').slug_date_time
+convert_time2 = ConvertTime(time, 'm').convert_time
 date1 = '2021-05-31'
 date2 = '2021-03-21'
 date_time1 = timezone.now()
 date_time2 = '2021-03-21 23:16:45.735963'
 date_l = date_diff(date1, date2, 'd')
 date_time_l = date_time_diff(date_time1, date_time2, 'd')
 
 # date_time_l will return the difference in value between date_time1 and date_time2 in days. You can use the 
 # corresponding string literal to get for minutes, hours and seconds which is the default value.
 # date_time_diff returns the difference in two dateTimes to the second. This should be used when you need to get 
 # date time difference to the last second
 
 ```
 
-## Convert between time and dates
+## Convert between time and date objects
 You can also use the convert_time function to convert between times
 
 ```python
 from date_time_literal import convert_time
 
 # Converts between years, days, hours, minutes, and seconds
 print(convert_time(365, 'd', 'y')) # Converts 365 days to years
@@ -106,24 +106,25 @@
 ```
 
 ### Some Basic use cases
 To get a rather comprehensive idea of how the package works, copy the code below and run it. The convert_time function
 was updated to be more efficient and now allows for week conversion as well in version 1.0.8
 
 ```python
-from date_time_literal import ConvertTime, DateDiff, date_diff, convert_time
+from date_time_literal import ConvertTime, DateDiff, date_diff, convert_time, date_time_diff
 from datetime import datetime
 
 t = ConvertTime('2021-05-31 23:16:55.321568', 'd')
 p = ConvertTime(datetime.now(), 'd')
 i = ConvertTime('2021-05-31 23:16:55+00:00', 'd')
 d = ConvertTime('2021-05-31', time_format='d')
 e = DateDiff('2021-05-31', '2021-04-31', 'd')
-print(t.slug_date_time)
-print(i.slug_date_time)
-print(d.slug_date)
+print(t.convert_time)
+print(i.convert_time)
+print(d.convert)
 print(e.date_diff)
 print(date_diff('2021-08-31', '2021-05-30', 'D'))
+print(date_time_diff('2021-04-30 21:58:50+00:00', '2021-04-30 10:58:55+00:00', 'H'))
 print(convert_time(1, "y", 'h'))
 print(convert_time(365, 'd', 'y'))
 
 ```
```

### Comparing `date_time_literal-1.0.8/setup.py` & `date_time_literal-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     setup_requires=['wheel'],
     name='date_time_literal',
     packages=['date_time_literal'],
-    version='1.0.8',
+    version='1.1.0',
     long_description=long_description,
     long_description_content_type='text/markdown',
     description='date-time-literal is '
                 'a python module that helps convert date-time or'
                 ' date to literal days, hours, seconds, or even minutes. Compare two DateTime or Date objects, by'
                 ' converting the objects to literal days, hours, minutes, or even seconds if you want to be precise. ',
     author='Kelvin Sajere',
```

