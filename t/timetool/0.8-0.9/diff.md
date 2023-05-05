# Comparing `tmp/timetool-0.8.tar.gz` & `tmp/timetool-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "timetool-0.8.tar", last modified: Sat Dec 17 09:51:36 2022, max compression
+gzip compressed data, was "timetool-0.9.tar", last modified: Fri May  5 19:09:01 2023, max compression
```

## Comparing `timetool-0.8.tar` & `timetool-0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2022-12-17 09:51:36.396753 timetool-0.8/
--rw-rw-r--   0 john      (1000) john      (1000)     1051 2021-12-26 03:57:28.000000 timetool-0.8/LICENSE
--rw-rw-r--   0 john      (1000) john      (1000)     3602 2022-12-17 09:51:36.396753 timetool-0.8/PKG-INFO
--rw-rw-r--   0 john      (1000) john      (1000)     3050 2022-12-17 09:41:03.000000 timetool-0.8/README.md
--rw-rw-r--   0 john      (1000) john      (1000)       38 2022-12-17 09:51:36.396753 timetool-0.8/setup.cfg
--rw-rw-r--   0 john      (1000) john      (1000)     1181 2022-12-17 09:51:30.000000 timetool-0.8/setup.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2022-12-17 09:51:36.396753 timetool-0.8/timetool/
--rw-rw-r--   0 john      (1000) john      (1000)        0 2021-12-26 02:57:24.000000 timetool-0.8/timetool/__init__.py
--rwxr-xr-x   0 john      (1000) john      (1000)    25882 2022-12-17 09:46:56.000000 timetool-0.8/timetool/main.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2022-12-17 09:51:36.396753 timetool-0.8/timetool.egg-info/
--rw-rw-r--   0 john      (1000) john      (1000)     3602 2022-12-17 09:51:36.000000 timetool-0.8/timetool.egg-info/PKG-INFO
--rw-rw-r--   0 john      (1000) john      (1000)      258 2022-12-17 09:51:36.000000 timetool-0.8/timetool.egg-info/SOURCES.txt
--rw-rw-r--   0 john      (1000) john      (1000)        1 2022-12-17 09:51:36.000000 timetool-0.8/timetool.egg-info/dependency_links.txt
--rw-rw-r--   0 john      (1000) john      (1000)       49 2022-12-17 09:51:36.000000 timetool-0.8/timetool.egg-info/entry_points.txt
--rw-rw-r--   0 john      (1000) john      (1000)       34 2022-12-17 09:51:36.000000 timetool-0.8/timetool.egg-info/requires.txt
--rw-rw-r--   0 john      (1000) john      (1000)        9 2022-12-17 09:51:36.000000 timetool-0.8/timetool.egg-info/top_level.txt
+drwxr-xr-x   0 johnmiller   (502) staff       (20)        0 2023-05-05 19:09:01.511367 timetool-0.9/
+-rw-rw-r--   0 johnmiller   (502) staff       (20)     1051 2021-12-26 03:57:28.000000 timetool-0.9/LICENSE
+-rw-r--r--   0 johnmiller   (502) staff       (20)     3602 2023-05-05 19:09:01.511245 timetool-0.9/PKG-INFO
+-rw-rw-r--   0 johnmiller   (502) staff       (20)     3050 2022-12-17 09:41:03.000000 timetool-0.9/README.md
+-rw-r--r--   0 johnmiller   (502) staff       (20)       38 2023-05-05 19:09:01.511405 timetool-0.9/setup.cfg
+-rw-rw-r--   0 johnmiller   (502) staff       (20)     1181 2023-05-05 19:08:49.000000 timetool-0.9/setup.py
+drwxr-xr-x   0 johnmiller   (502) staff       (20)        0 2023-05-05 19:09:01.510424 timetool-0.9/timetool/
+-rw-rw-r--   0 johnmiller   (502) staff       (20)        0 2021-12-26 02:57:24.000000 timetool-0.9/timetool/__init__.py
+-rwxr-xr-x   0 johnmiller   (502) staff       (20)    26393 2023-04-28 01:09:09.000000 timetool-0.9/timetool/main.py
+drwxr-xr-x   0 johnmiller   (502) staff       (20)        0 2023-05-05 19:09:01.511080 timetool-0.9/timetool.egg-info/
+-rw-r--r--   0 johnmiller   (502) staff       (20)     3602 2023-05-05 19:09:01.000000 timetool-0.9/timetool.egg-info/PKG-INFO
+-rw-r--r--   0 johnmiller   (502) staff       (20)      258 2023-05-05 19:09:01.000000 timetool-0.9/timetool.egg-info/SOURCES.txt
+-rw-r--r--   0 johnmiller   (502) staff       (20)        1 2023-05-05 19:09:01.000000 timetool-0.9/timetool.egg-info/dependency_links.txt
+-rw-r--r--   0 johnmiller   (502) staff       (20)       49 2023-05-05 19:09:01.000000 timetool-0.9/timetool.egg-info/entry_points.txt
+-rw-r--r--   0 johnmiller   (502) staff       (20)       34 2023-05-05 19:09:01.000000 timetool-0.9/timetool.egg-info/requires.txt
+-rw-r--r--   0 johnmiller   (502) staff       (20)        9 2023-05-05 19:09:01.000000 timetool-0.9/timetool.egg-info/top_level.txt
```

### Comparing `timetool-0.8/LICENSE` & `timetool-0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `timetool-0.8/PKG-INFO` & `timetool-0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timetool
-Version: 0.8
+Version: 0.9
 Summary: Quick timezone and time format conversion CLI tool
 Home-page: https://github.com/personalcomputer/timetool
 Author: John Miller
 Author-email: john@johngm.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `timetool-0.8/README.md` & `timetool-0.9/README.md`

 * *Files identical despite different names*

### Comparing `timetool-0.8/setup.py` & `timetool-0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 here = os.path.abspath(os.path.dirname(__file__))
 with io.open(os.path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = '\n' + f.read()
 
 setup(
     name=NAME,
-    version='0.8',
+    version='0.9',
     description='Quick timezone and time format conversion CLI tool',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='John Miller',
     author_email='john@johngm.com',
     python_requires='>=3.7.0',
     url='https://github.com/personalcomputer/timetool',
```

### Comparing `timetool-0.8/timetool/main.py` & `timetool-0.9/timetool/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -262,31 +262,31 @@
         ret_time += relativedelta(weekday=DAYS_OF_WEEK.index(dow_match.group(2)))
         return ret_time, input_timezone_raw
 
     # Maybe it is unix time?
     # Warning: Without leading zeros, our logic only supports unix times after **1973-03-03** and up to **33658**
     if re.match(r"^\d{9,12}(?:\.\d+)?$", datetime_agg):
         log_format("unix")
-        return pytz.utc.localize(datetime.datetime.utcfromtimestamp(float(datetime_agg))), input_timezone_raw
+        return datetime.datetime.fromtimestamp(float(datetime_agg), tz=datetime.timezone.utc), input_timezone_raw
     # Or unixime with milliseconds?
     # Warning: Without leading zeros, our logic only supports unix times w/ ms after **2001-09-09** and up to **33658**
     if re.match(r"^\d{13,15}$", datetime_agg):
         log_format("unix milliseconds")
-        return pytz.utc.localize(datetime.datetime.utcfromtimestamp(int(datetime_agg) / 1000.0)), input_timezone_raw
+        return datetime.datetime.fromtimestamp(int(datetime_agg) / 1000.0, tz=datetime.timezone.utc), input_timezone_raw
     # Or unixtime with microseconds?
     # Warning: Without leading zeros, our logic only supports unix times w/ us after **1973-03-03** and up to **5138**
     if re.match(r"^\d{16,18}$", datetime_agg):
         log_format("unix microseconds")
-        return pytz.utc.localize(datetime.datetime.utcfromtimestamp(int(datetime_agg) / 10000000.0)), input_timezone_raw
+        return datetime.datetime.fromtimestamp(int(datetime_agg) / 10000000.0, tz=datetime.timezone.utc), input_timezone_raw
     # Or unixtime with nanoseconds?
     # Warning: Without leading zeros, our logic only supports unix times w/ ns after **2001-09-09** and up to **33658**
     if re.match(r"^\d{19,21}$", datetime_agg):
         log_format("unix nanoseconds")
         return (
-            pytz.utc.localize(datetime.datetime.utcfromtimestamp(int(datetime_agg) / 1000000000.0)),
+            datetime.datetime.fromtimestamp(int(datetime_agg) / 1000000000.0, tz=datetime.timezone.utc),
             input_timezone_raw,
         )
 
     # Try parsing with dateutil - this is the main mode
     try:
         # First convert specifications like GMT+6 or UTC+6 into just "+6" to avoid the extremely counter-intuitive and
         # unusual design behavior of dateutil/POSIX. POSIX specifies to interpret UTC+6 as meaning a timezone with UTC
@@ -490,15 +490,20 @@
         return f"{sign}{delta_str}{relative_term}"
     return delta_str
 
 
 def run(argv):
     USAGE = textwrap.dedent(
         """
-        Usage: {prog} [-h] [TIME] [in CONVERSION_TIMEZONE] [-o][-e]
+        Usage: {prog} [-h] [TIME] [in CONVERSION_TIMEZONE] [-o][-e][-i]
+
+        Flags:
+            -o  Show "one line" output format that includes all timezones in one line.
+            -e  Show extended delta time formats.
+            -i  Output JUST an ISO8601 UTC time. For repurposing timetool for use in scripts.
 
         Examples:
           {prog}
           {prog} 1621108906
           {prog} 1621108906000
           {prog} 1621108906.000
           {prog} May 15, 2021 01:01:46 PM PDT
@@ -512,34 +517,39 @@
           {prog} + 1mo
           {prog} + 01:30:00
 
         Help & support:
           https://github.com/personalcomputer/timetool/issues
     """
     ).strip()
-    if len(argv) > 1 and argv[1] in ("-h", "--help"):
+    if len(argv) > 1 and (set(argv) & set(["-h", "--help"])):
         print(USAGE.format(prog=argv[0]))
         return
 
-    datetime_agg = " ".join([arg.strip() for arg in argv[1:]])
-    if datetime_agg.endswith("--debug"):
-        datetime_agg = datetime_agg[: -len("--debug")].strip()
+    if "--debug" in argv:
+        argv.remove("--debug")
         debug = True
     else:
         debug = False
-    if datetime_agg.endswith("-e"):
-        datetime_agg = datetime_agg[: -len("-e")].strip()
+    if "-e" in argv:
+        argv.remove("-e")
         extra_output = True
     else:
         extra_output = False
-    if datetime_agg.endswith("-o"):
-        datetime_agg = datetime_agg[: -len("-o")].strip()
+    if "-o" in argv:
+        argv.remove("-o")
         oneline = True
     else:
         oneline = False
+    if "-i" in argv:
+        argv.remove("-i")
+        iso8601_only_mode = True
+    else:
+        iso8601_only_mode = False
+    datetime_agg = " ".join([arg.strip() for arg in argv[1:]])
 
     # Check if the time used 'X in <TIMEZONE>' pattern, and if so then ensure we display that timezone in the output
     match = re.search(r" (?:as|in) ((?:[a-zA-Z/_]{2,},? ?){1,})$", datetime_agg, re.IGNORECASE)
     if match:
         extra_display_timezones = [parse_timezone(item.strip()) for item in match.group(1).split(",")]
         datetime_agg = datetime_agg[: match.span()[0]]
     else:
@@ -567,21 +577,23 @@
             if not b_delta:
                 raise exc
             finding_delta = False
         if finding_delta:
             if operator == add:
                 print("Error: Cannot add two datetimes together")
                 sys.exit(1)
-            print(
-                f"{format_datetime_for_inferred_locale(a_dt)} {operator_char} {format_datetime_for_inferred_locale(b_dt)}"
-            )
+            if not iso8601_only_mode:
+                print(
+                    f"{format_datetime_for_inferred_locale(a_dt)} {operator_char} {format_datetime_for_inferred_locale(b_dt)}"
+                )
             handle_delta_display(a_dt, b_dt, extra_output=extra_output)
             return
         # finding absolute..
-        print(f"{format_datetime_for_inferred_locale(a_dt)} {operator_char} {b_str}")
+        if not iso8601_only_mode:
+            print(f"{format_datetime_for_inferred_locale(a_dt)} {operator_char} {b_str}")
         input_time = a_dt + b_delta
         display_prefix = "= "
     else:
         # Just a single time!
         try:
             input_time = parse_datetime(datetime_agg, log_input_format=extra_output)
         except ValueError as exc:
@@ -590,14 +602,15 @@
             print("Error: " + (" ".join(exc.args)))
             sys.exit(1)
 
     handle_time_display(
         input_time,
         display_prefix=display_prefix,
         oneline=oneline,
+        iso8601_only_mode=iso8601_only_mode,
         extra_output=extra_output,
         extra_display_timezones=extra_display_timezones,
     )
 
 
 def handle_delta_display(a_dt, b_dt, extra_output):
     output = [
@@ -611,17 +624,21 @@
                 "~" + humanize_time_difference(a_dt, b_dt, variant="multiterm"),
                 "~" + humanize_time_difference(a_dt, b_dt, variant="oneterm-alt"),
             ]
         )
     print(textwrap.indent("\n".join(output), "= "))
 
 
-def handle_time_display(input_time, display_prefix, oneline, extra_output, extra_display_timezones):
+def handle_time_display(input_time, display_prefix, oneline, iso8601_only_mode, extra_output, extra_display_timezones):
     utc_time = input_time.astimezone(pytz.utc)
 
+    if iso8601_only_mode:
+        print(utc_time.isoformat(timespec="milliseconds"))
+        return
+
     # Unix
     unix_time = input_time.timestamp()
     assert unix_time == (utc_time - pytz.utc.localize(datetime.datetime.utcfromtimestamp(0))).total_seconds()
     output = []
     BOLD_TERM_CODE = "\033[1m"  # TODO: Use tput (actually, curses - tigetstr('bold') & tigetstr('sgr0'))
     NOBOLD_TERM_CODE = "\033[0m"
     output.append(f"{BOLD_TERM_CODE}{unix_time:.0f}{NOBOLD_TERM_CODE}")
```

### Comparing `timetool-0.8/timetool.egg-info/PKG-INFO` & `timetool-0.9/timetool.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timetool
-Version: 0.8
+Version: 0.9
 Summary: Quick timezone and time format conversion CLI tool
 Home-page: https://github.com/personalcomputer/timetool
 Author: John Miller
 Author-email: john@johngm.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

