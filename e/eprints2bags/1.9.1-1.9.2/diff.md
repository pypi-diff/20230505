# Comparing `tmp/eprints2bags-1.9.1.tar.gz` & `tmp/eprints2bags-1.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/eprints2bags-1.9.1.tar", last modified: Sat Nov  9 22:05:05 2019, max compression
+gzip compressed data, was "dist/eprints2bags-1.9.2.tar", last modified: Sat Jul  4 01:18:52 2020, max compression
```

## Comparing `eprints2bags-1.9.1.tar` & `eprints2bags-1.9.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 mhucka     (511) staff       (20)        0 2019-11-09 22:05:05.000000 eprints2bags-1.9.1/
--rw-r--r--   0 mhucka     (511) staff       (20)    29297 2019-11-09 22:05:05.000000 eprints2bags-1.9.1/PKG-INFO
--rw-r--r--   0 mhucka     (511) staff       (20)    25678 2019-11-09 22:02:53.000000 eprints2bags-1.9.1/README.md
-drwxr-xr-x   0 mhucka     (511) staff       (20)        0 2019-11-09 22:05:05.000000 eprints2bags-1.9.1/bin/
--rwxr-xr-x   0 mhucka     (511) staff       (20)      916 2018-12-13 18:27:19.000000 eprints2bags-1.9.1/bin/eprints2bags
-drwxr-xr-x   0 mhucka     (511) staff       (20)        0 2019-11-09 22:05:05.000000 eprints2bags-1.9.1/eprints2bags/
--rw-r--r--   0 mhucka     (511) staff       (20)     2970 2019-11-09 00:56:31.000000 eprints2bags-1.9.1/eprints2bags/__init__.py
--rwxr-xr-x   0 mhucka     (511) staff       (20)    31247 2019-11-09 00:56:31.000000 eprints2bags-1.9.1/eprints2bags/__main__.py
--rw-r--r--   0 mhucka     (511) staff       (20)      558 2019-01-20 19:49:26.000000 eprints2bags-1.9.1/eprints2bags/constants.py
--rw-r--r--   0 mhucka     (511) staff       (20)     1588 2019-11-09 00:56:31.000000 eprints2bags-1.9.1/eprints2bags/data_helpers.py
--rw-r--r--   0 mhucka     (511) staff       (20)     3556 2019-11-09 00:56:31.000000 eprints2bags-1.9.1/eprints2bags/debug.py
--rw-r--r--   0 mhucka     (511) staff       (20)     6143 2019-01-22 01:41:10.000000 eprints2bags-1.9.1/eprints2bags/eprints.py
--rw-r--r--   0 mhucka     (511) staff       (20)     1245 2019-01-20 19:49:24.000000 eprints2bags-1.9.1/eprints2bags/exceptions.py
--rw-r--r--   0 mhucka     (511) staff       (20)     4898 2019-11-08 21:25:08.000000 eprints2bags-1.9.1/eprints2bags/files.py
--rw-r--r--   0 mhucka     (511) staff       (20)     6146 2019-01-20 19:49:25.000000 eprints2bags-1.9.1/eprints2bags/messages.py
--rw-r--r--   0 mhucka     (511) staff       (20)    14638 2019-11-09 00:56:31.000000 eprints2bags-1.9.1/eprints2bags/network.py
--rw-r--r--   0 mhucka     (511) staff       (20)     3334 2019-01-20 19:49:25.000000 eprints2bags-1.9.1/eprints2bags/processes.py
-drwxr-xr-x   0 mhucka     (511) staff       (20)        0 2019-11-09 22:05:05.000000 eprints2bags-1.9.1/eprints2bags.egg-info/
--rw-r--r--   0 mhucka     (511) staff       (20)    29297 2019-11-09 22:05:05.000000 eprints2bags-1.9.1/eprints2bags.egg-info/PKG-INFO
--rw-r--r--   0 mhucka     (511) staff       (20)      534 2019-11-09 22:05:05.000000 eprints2bags-1.9.1/eprints2bags.egg-info/SOURCES.txt
--rw-r--r--   0 mhucka     (511) staff       (20)        1 2019-11-09 22:05:05.000000 eprints2bags-1.9.1/eprints2bags.egg-info/dependency_links.txt
--rw-r--r--   0 mhucka     (511) staff       (20)        1 2019-11-08 21:20:08.000000 eprints2bags-1.9.1/eprints2bags.egg-info/not-zip-safe
--rw-r--r--   0 mhucka     (511) staff       (20)      200 2019-11-09 22:05:05.000000 eprints2bags-1.9.1/eprints2bags.egg-info/requires.txt
--rw-r--r--   0 mhucka     (511) staff       (20)       13 2019-11-09 22:05:05.000000 eprints2bags-1.9.1/eprints2bags.egg-info/top_level.txt
--rw-r--r--   0 mhucka     (511) staff       (20)     1281 2019-11-09 22:05:05.000000 eprints2bags-1.9.1/setup.cfg
--rw-r--r--   0 mhucka     (511) staff       (20)      824 2019-11-09 22:00:26.000000 eprints2bags-1.9.1/setup.py
+drwxr-xr-x   0 mhucka     (511) staff       (20)        0 2020-07-04 01:18:52.000000 eprints2bags-1.9.2/
+-rw-r--r--   0 mhucka     (511) staff       (20)    29083 2020-07-04 01:18:52.000000 eprints2bags-1.9.2/PKG-INFO
+-rw-r--r--   0 mhucka     (511) staff       (20)    25479 2020-07-04 01:05:20.000000 eprints2bags-1.9.2/README.md
+drwxr-xr-x   0 mhucka     (511) staff       (20)        0 2020-07-04 01:18:52.000000 eprints2bags-1.9.2/bin/
+-rwxr-xr-x   0 mhucka     (511) staff       (20)      916 2018-12-13 18:27:19.000000 eprints2bags-1.9.2/bin/eprints2bags
+drwxr-xr-x   0 mhucka     (511) staff       (20)        0 2020-07-04 01:18:52.000000 eprints2bags-1.9.2/eprints2bags/
+-rw-r--r--   0 mhucka     (511) staff       (20)     2970 2019-11-09 00:56:31.000000 eprints2bags-1.9.2/eprints2bags/__init__.py
+-rwxr-xr-x   0 mhucka     (511) staff       (20)    31459 2020-07-03 22:52:24.000000 eprints2bags-1.9.2/eprints2bags/__main__.py
+-rw-r--r--   0 mhucka     (511) staff       (20)      558 2019-01-20 19:49:26.000000 eprints2bags-1.9.2/eprints2bags/constants.py
+-rw-r--r--   0 mhucka     (511) staff       (20)     1588 2019-11-09 00:56:31.000000 eprints2bags-1.9.2/eprints2bags/data_helpers.py
+-rw-r--r--   0 mhucka     (511) staff       (20)     3556 2019-11-09 00:56:31.000000 eprints2bags-1.9.2/eprints2bags/debug.py
+-rw-r--r--   0 mhucka     (511) staff       (20)     6143 2019-01-22 01:41:10.000000 eprints2bags-1.9.2/eprints2bags/eprints.py
+-rw-r--r--   0 mhucka     (511) staff       (20)     1245 2019-01-20 19:49:24.000000 eprints2bags-1.9.2/eprints2bags/exceptions.py
+-rw-r--r--   0 mhucka     (511) staff       (20)     4898 2019-11-08 21:25:08.000000 eprints2bags-1.9.2/eprints2bags/files.py
+-rw-r--r--   0 mhucka     (511) staff       (20)     6146 2019-01-20 19:49:25.000000 eprints2bags-1.9.2/eprints2bags/messages.py
+-rw-r--r--   0 mhucka     (511) staff       (20)    14819 2020-07-03 23:55:30.000000 eprints2bags-1.9.2/eprints2bags/network.py
+-rw-r--r--   0 mhucka     (511) staff       (20)     3334 2019-01-20 19:49:25.000000 eprints2bags-1.9.2/eprints2bags/processes.py
+drwxr-xr-x   0 mhucka     (511) staff       (20)        0 2020-07-04 01:18:52.000000 eprints2bags-1.9.2/eprints2bags.egg-info/
+-rw-r--r--   0 mhucka     (511) staff       (20)    29083 2020-07-04 01:18:52.000000 eprints2bags-1.9.2/eprints2bags.egg-info/PKG-INFO
+-rw-r--r--   0 mhucka     (511) staff       (20)      534 2020-07-04 01:18:52.000000 eprints2bags-1.9.2/eprints2bags.egg-info/SOURCES.txt
+-rw-r--r--   0 mhucka     (511) staff       (20)        1 2020-07-04 01:18:52.000000 eprints2bags-1.9.2/eprints2bags.egg-info/dependency_links.txt
+-rw-r--r--   0 mhucka     (511) staff       (20)        1 2020-07-04 01:10:57.000000 eprints2bags-1.9.2/eprints2bags.egg-info/not-zip-safe
+-rw-r--r--   0 mhucka     (511) staff       (20)      200 2020-07-04 01:18:52.000000 eprints2bags-1.9.2/eprints2bags.egg-info/requires.txt
+-rw-r--r--   0 mhucka     (511) staff       (20)       13 2020-07-04 01:18:52.000000 eprints2bags-1.9.2/eprints2bags.egg-info/top_level.txt
+-rw-r--r--   0 mhucka     (511) staff       (20)     1281 2020-07-04 01:18:52.000000 eprints2bags-1.9.2/setup.cfg
+-rw-r--r--   0 mhucka     (511) staff       (20)      824 2019-11-09 22:00:26.000000 eprints2bags-1.9.2/setup.py
```

### Comparing `eprints2bags-1.9.1/PKG-INFO` & `eprints2bags-1.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eprints2bags
-Version: 1.9.1
+Version: 1.9.2
 Summary: Download EPrints content and save it in BagIt-format bags.
 Home-page: https://github.com/caltechlibrary/eprints2bags
 Author: Michael Hucka
 Author-email: mhucka@caltech.edu
 License: BSD 3-clause
 Project-URL: Source Code, https://github.com/caltechlibrary/eprints2bags
 Project-URL: Bug Tracker, https://github.com/caltechlibrary/eprints2bags/issues
@@ -16,23 +16,21 @@
         *Authors*:      [Michael Hucka](http://github.com/mhucka), [Betsy Coles](https://github.com/betsycoles)<br>
         *Repository*:   [https://github.com/caltechlibrary/eprints2bags](https://github.com/caltechlibrary/eprints2bags)<br>
         *License*:      BSD/MIT derivative &ndash; see the [LICENSE](LICENSE) file for more information
         
         [![License](https://img.shields.io/badge/License-BSD%203--Clause-blue.svg?style=flat-square)](https://choosealicense.com/licenses/bsd-3-clause)
         [![Python](https://img.shields.io/badge/Python-3.5+-brightgreen.svg?style=flat-square)](http://shields.io)
         [![Latest release](https://img.shields.io/github/v/release/caltechlibrary/eprints2bags.svg?style=flat-square&color=b44e88)](https://github.com/caltechlibrary/eprints2bags/releases)
-        [![DOI](http://img.shields.io/badge/DOI-10.22002%20%2f%20D1.1310-blue.svg?style=flat-square)](https://data.caltech.edu/records/1310)
+        [![DOI](http://img.shields.io/badge/DOI-10.22002%20%2f%20D1.1450-blue.svg?style=flat-square)](https://data.caltech.edu/records/1450)
         [![PyPI](https://img.shields.io/pypi/v/eprints2bags.svg?style=flat-square&color=red)](https://pypi.org/project/eprints2bags/)
         
         🏁 Log of recent changes
         -----------------------
         
-        _Version 1.9.1_: This release updates the README file to explain how to install from PyPI, and fixes some internal files related to producing releases on PyPI.
-        
-        _Version 1.9.0_: This release fixes a couple of minor bugs.  It also changes the debug flag letter to be `-@` and changes the behavior of the flag; these changes are not backward-compatible.  Internally, it changes the setup process to use `setup.cfg` and uses a new way to get package metadata.  Finally, this version is being made available from [PyPI](https://pypi.org/project/eprints2bags).
+        _Version 1.9.2_: **Critical fix** &ndash; this version fixes a bug that caused `eprints2bags` to write zero-length data files when used with newer versions of Python.  **You should upgrade your copy of `eprints2bags` to this version**.  This version also reports skipped records separately from missing records (in the final summary at the end of a run).
         
         The file [CHANGES](CHANGES.md) contains a more complete change log that includes information about previous releases.
         
         
         Table of Contents
         -----------------
         
@@ -66,15 +64,15 @@
         Then, to install `eprints2bags` from the Python package repository, run the following command:
         ```
         python3 -m pip install eprints2bags --user --upgrade
         ```
         
         As an alternative to getting it from PyPI, you can instruct `pip` to install `eprints2bags` directly from the GitHub repository:
         ```sh
-        python3 -m pip install git+https@github.com:caltechlibrary/eprints2bags.git --user --upgrade
+        python3 -m pip install git+https://github.com/caltechlibrary/eprints2bags.git --user --upgrade
         ```
         
         On Linux and macOS systems, assuming that the installation proceeds normally, you should end up with a program called `eprints2bags` in a location normally searched by your terminal shell for commands.
         
         
         ▶︎ Using Eprints2bags
         ---------------------
@@ -221,20 +219,20 @@
         | `-p`_P_ | `--password`_U_   | Password for EPrints proxy login | |
         | `-t`_T_ | `--arch-type`_T_  | Use archive type _T_ | Uncompressed ZIP | ♢ |
         | `-y`_Y_ | `--delay`_Y_      | Pause _Y_ ms between getting records | 100 milliseconds | |
         | `-C`    | `--no-color`      | Don't color-code the output | Use colors in the terminal output | |
         | `-K`    | `--no-keyring`    | Don't use a keyring/keychain | Store login info in keyring | |
         | `-R`    | `--reset`         | Reset user login & password used | Reuse previous credentials |
         | `-V`    | `--version`       | Print program version info and exit | Do other actions instead | |
-        | `-@`_OUT_ | `--debug`_OUT_    | Debugging mode; write trace to _OUT_ | Normal mode | ♣ |
+        | `-@`_OUT_ | `--debug`_OUT_    | Debugging mode; write trace to _OUT_ | Normal mode | ⚐ |
         
          ⚑ &nbsp; Required argument.<br>
         ✦ &nbsp; Possible values: `none`, `bag`, `bag-and-archive`.<br>
         ♢ &nbsp; Possible values: `uncompressed-zip`, `compressed-zip`, `uncompressed-tar`, `compressed-tar`.<br>
-        ♣ &nbsp; To write to the console, use the character `-` as the value of _OUT_; otherwise, _OUT_ must be the name of a file where the output should be written.
+        ⚐ &nbsp; To write to the console, use the character `-` as the value of _OUT_; otherwise, _OUT_ must be the name of a file where the output should be written.
         
         ### Additional notes and considerations
         
         Beware that some file systems have limitations on the number of subdirectories that can be created, which directly impacts how many record subdirectories can be created by this program.  `eprints2bags` attempts to guess the type of file system where the output is being written and warn the user if the number of records exceeds known maximums (e.g., 31,998 subdirectories for the [ext2](https://en.wikipedia.org/wiki/Ext2) and [ext3](https://en.wikipedia.org/wiki/Ext3) file systems in Linux), but its internal table does not include all possible file systems and it may not be able to warn users in all cases.  If you encounter file system limitations on the number of subdirectories that can be created, a simple solution is to manually create an intermediate level of subdirectories under the destination given to `-o`, then run `eprints2bags` multiple times, each time indicating a different subrange of records to the `-i` option and a different subdirectory to `-o`, such that the number of records written to each destination is below the file system's limit on total number of directories.
         
         It is also noteworthy that hitting a server for tens of thousands of records and documents in rapid succession is likely to draw suspicion from server administrators.  By default, this program inserts a small delay between record fetches (adjustable using the `-y` command-line option), which may be too short in some cases.  Setting the value to 0 is also possible, but might get you blocked or banned from an institution's servers.
         
@@ -313,9 +311,9 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Topic :: System :: Archiving
 Classifier: Topic :: System :: Archiving :: Packaging
 Classifier: Topic :: Utilities
-Requires-Python: >=3.5
+Requires-Python: >= 3.5
 Description-Content-Type: text/markdown
```

### Comparing `eprints2bags-1.9.1/README.md` & `eprints2bags-1.9.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,21 @@
 *Authors*:      [Michael Hucka](http://github.com/mhucka), [Betsy Coles](https://github.com/betsycoles)<br>
 *Repository*:   [https://github.com/caltechlibrary/eprints2bags](https://github.com/caltechlibrary/eprints2bags)<br>
 *License*:      BSD/MIT derivative &ndash; see the [LICENSE](LICENSE) file for more information
 
 [![License](https://img.shields.io/badge/License-BSD%203--Clause-blue.svg?style=flat-square)](https://choosealicense.com/licenses/bsd-3-clause)
 [![Python](https://img.shields.io/badge/Python-3.5+-brightgreen.svg?style=flat-square)](http://shields.io)
 [![Latest release](https://img.shields.io/github/v/release/caltechlibrary/eprints2bags.svg?style=flat-square&color=b44e88)](https://github.com/caltechlibrary/eprints2bags/releases)
-[![DOI](http://img.shields.io/badge/DOI-10.22002%20%2f%20D1.1310-blue.svg?style=flat-square)](https://data.caltech.edu/records/1310)
+[![DOI](http://img.shields.io/badge/DOI-10.22002%20%2f%20D1.1450-blue.svg?style=flat-square)](https://data.caltech.edu/records/1450)
 [![PyPI](https://img.shields.io/pypi/v/eprints2bags.svg?style=flat-square&color=red)](https://pypi.org/project/eprints2bags/)
 
 🏁 Log of recent changes
 -----------------------
 
-_Version 1.9.1_: This release updates the README file to explain how to install from PyPI, and fixes some internal files related to producing releases on PyPI.
-
-_Version 1.9.0_: This release fixes a couple of minor bugs.  It also changes the debug flag letter to be `-@` and changes the behavior of the flag; these changes are not backward-compatible.  Internally, it changes the setup process to use `setup.cfg` and uses a new way to get package metadata.  Finally, this version is being made available from [PyPI](https://pypi.org/project/eprints2bags).
+_Version 1.9.2_: **Critical fix** &ndash; this version fixes a bug that caused `eprints2bags` to write zero-length data files when used with newer versions of Python.  **You should upgrade your copy of `eprints2bags` to this version**.  This version also reports skipped records separately from missing records (in the final summary at the end of a run).
 
 The file [CHANGES](CHANGES.md) contains a more complete change log that includes information about previous releases.
 
 
 Table of Contents
 -----------------
 
@@ -56,15 +54,15 @@
 Then, to install `eprints2bags` from the Python package repository, run the following command:
 ```
 python3 -m pip install eprints2bags --user --upgrade
 ```
 
 As an alternative to getting it from PyPI, you can instruct `pip` to install `eprints2bags` directly from the GitHub repository:
 ```sh
-python3 -m pip install git+https@github.com:caltechlibrary/eprints2bags.git --user --upgrade
+python3 -m pip install git+https://github.com/caltechlibrary/eprints2bags.git --user --upgrade
 ```
 
 On Linux and macOS systems, assuming that the installation proceeds normally, you should end up with a program called `eprints2bags` in a location normally searched by your terminal shell for commands.
 
 
 ▶︎ Using Eprints2bags
 ---------------------
@@ -211,20 +209,20 @@
 | `-p`_P_ | `--password`_U_   | Password for EPrints proxy login | |
 | `-t`_T_ | `--arch-type`_T_  | Use archive type _T_ | Uncompressed ZIP | ♢ |
 | `-y`_Y_ | `--delay`_Y_      | Pause _Y_ ms between getting records | 100 milliseconds | |
 | `-C`    | `--no-color`      | Don't color-code the output | Use colors in the terminal output | |
 | `-K`    | `--no-keyring`    | Don't use a keyring/keychain | Store login info in keyring | |
 | `-R`    | `--reset`         | Reset user login & password used | Reuse previous credentials |
 | `-V`    | `--version`       | Print program version info and exit | Do other actions instead | |
-| `-@`_OUT_ | `--debug`_OUT_    | Debugging mode; write trace to _OUT_ | Normal mode | ♣ |
+| `-@`_OUT_ | `--debug`_OUT_    | Debugging mode; write trace to _OUT_ | Normal mode | ⚐ |
 
  ⚑ &nbsp; Required argument.<br>
 ✦ &nbsp; Possible values: `none`, `bag`, `bag-and-archive`.<br>
 ♢ &nbsp; Possible values: `uncompressed-zip`, `compressed-zip`, `uncompressed-tar`, `compressed-tar`.<br>
-♣ &nbsp; To write to the console, use the character `-` as the value of _OUT_; otherwise, _OUT_ must be the name of a file where the output should be written.
+⚐ &nbsp; To write to the console, use the character `-` as the value of _OUT_; otherwise, _OUT_ must be the name of a file where the output should be written.
 
 ### Additional notes and considerations
 
 Beware that some file systems have limitations on the number of subdirectories that can be created, which directly impacts how many record subdirectories can be created by this program.  `eprints2bags` attempts to guess the type of file system where the output is being written and warn the user if the number of records exceeds known maximums (e.g., 31,998 subdirectories for the [ext2](https://en.wikipedia.org/wiki/Ext2) and [ext3](https://en.wikipedia.org/wiki/Ext3) file systems in Linux), but its internal table does not include all possible file systems and it may not be able to warn users in all cases.  If you encounter file system limitations on the number of subdirectories that can be created, a simple solution is to manually create an intermediate level of subdirectories under the destination given to `-o`, then run `eprints2bags` multiple times, each time indicating a different subrange of records to the `-i` option and a different subdirectory to `-o`, such that the number of records written to each destination is below the file system's limit on total number of directories.
 
 It is also noteworthy that hitting a server for tens of thousands of records and documents in rapid succession is likely to draw suspicion from server administrators.  By default, this program inserts a small delay between record fetches (adjustable using the `-y` command-line option), which may be too short in some cases.  Setting the value to 0 is also possible, but might get you blocked or banned from an institution's servers.
```

### Comparing `eprints2bags-1.9.1/bin/eprints2bags` & `eprints2bags-1.9.2/bin/eprints2bags`

 * *Files identical despite different names*

### Comparing `eprints2bags-1.9.1/eprints2bags/__init__.py` & `eprints2bags-1.9.2/eprints2bags/__init__.py`

 * *Files identical despite different names*

### Comparing `eprints2bags-1.9.1/eprints2bags/__main__.py` & `eprints2bags-1.9.2/eprints2bags/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -413,29 +413,33 @@
             say.info('Will only keep records {} status {}',
                      'without' if status_negation else 'with',
                      fmt_statuses(status, status_negation))
         say.info('Output will be written under directory "{}"', output_dir)
         make_dir(output_dir)
 
         say.msg('='*70, 'dark')
-        missing = wanted.copy()
+        missing = []
+        skipped = []
         for number in wanted:
             # Start by getting the full record in EP3 XML format.  A failure
             # here will either cause an exit or moving to the next record.
             say.msg('Getting record with id {}'.format(number), 'white')
             xml = eprints_xml(number, api_url, user, password, keep_going, say)
             if xml == None:
+                missing.append(number)
                 continue
             if lastmod and eprints_lastmod(xml) < lastmod:
                 say.info("{} hasn't been modified since {} -- skipping",
                          number, lastmod_str)
+                skipped.append(number)
                 continue
             if status and ((not status_negation and eprints_status(xml) not in status)
                            or (status_negation and eprints_status(xml) in status)):
                 say.info('{} has status "{}" -- skipping', number, eprints_status(xml))
+                skipped.append(number)
                 continue
 
             # Good so far.  Create the directory and write the XML out.
             record_dir = path.join(output_dir, prefix + str(number))
             say.info('Creating {}', record_dir)
             make_dir(record_dir)
             write_record(number, xml, prefix, record_dir)
@@ -443,22 +447,23 @@
             # Download any documents referenced in the XML record.
             docs = eprints_documents(xml)
             download_files(docs, user, password, record_dir, keep_going, say)
 
             # Bag it and archive it, depending on user choice.
             bag_and_archive(record_dir, bag_action, archive_fmt, procs, xml, api_url, say)
 
-            if wanted and number in wanted:
-                missing.remove(number)
+            # Be nice to the server.
             sleep(delay/1000)
 
         say.msg('='*70, 'dark')
-        count = len(wanted) - len(missing)
+        count = len(wanted) - len(missing) - len(skipped)
         say.info('Wrote {} EPrints record{} to {}/.', intcomma(count),
                  's' if count > 1 else '', output_dir)
+        if len(skipped) > 0:
+            say.info('The following records were skipped: '+ ', '.join(skipped) + '.')
         if len(missing) > 0:
             say.warn('The following records were not found: '+ ', '.join(missing) + '.')
 
         # Bag the whole result and archive it, depending on user choice.
         bag_and_archive(output_dir, end_action, archive_fmt, procs, None, api_url, say)
 
     except KeyboardInterrupt as ex:
```

### Comparing `eprints2bags-1.9.1/eprints2bags/constants.py` & `eprints2bags-1.9.2/eprints2bags/constants.py`

 * *Files identical despite different names*

### Comparing `eprints2bags-1.9.1/eprints2bags/data_helpers.py` & `eprints2bags-1.9.2/eprints2bags/data_helpers.py`

 * *Files identical despite different names*

### Comparing `eprints2bags-1.9.1/eprints2bags/debug.py` & `eprints2bags-1.9.2/eprints2bags/debug.py`

 * *Files identical despite different names*

### Comparing `eprints2bags-1.9.1/eprints2bags/eprints.py` & `eprints2bags-1.9.2/eprints2bags/eprints.py`

 * *Files identical despite different names*

### Comparing `eprints2bags-1.9.1/eprints2bags/exceptions.py` & `eprints2bags-1.9.2/eprints2bags/exceptions.py`

 * *Files identical despite different names*

### Comparing `eprints2bags-1.9.1/eprints2bags/files.py` & `eprints2bags-1.9.2/eprints2bags/files.py`

 * *Files identical despite different names*

### Comparing `eprints2bags-1.9.1/eprints2bags/messages.py` & `eprints2bags-1.9.2/eprints2bags/messages.py`

 * *Files identical despite different names*

### Comparing `eprints2bags-1.9.1/eprints2bags/network.py` & `eprints2bags-1.9.2/eprints2bags/network.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 Copyright (c) 2019 by the California Institute of Technology.  This code is
 open-source software released under a 3-clause BSD license.  Please see the
 file "LICENSE" for more information.
 '''
 
 import http.client
 from   http.client import responses as http_responses
-from   os import path
+from   os import path, stat
 import requests
 from   requests.packages.urllib3.exceptions import InsecureRequestWarning
 from   time import sleep
 import shutil
 import socket
 import ssl
 import urllib
@@ -103,15 +103,15 @@
                 warnings.simplefilter("ignore", InsecureRequestWarning)
                 if __debug__: log('doing http {} on {}', get_or_post, url)
                 if session:
                     method = getattr(session, get_or_post)
                 else:
                     method = requests.get if get_or_post == 'get' else requests.post
                 response = method(url, timeout = timeout, verify = False, **kwargs)
-                if __debug__: log('received {} bytes', len(response.content))
+                if __debug__: log('response received')
                 return response
         except Exception as ex:
             # Problem might be transient.  Don't quit right away.
             failures += 1
             if __debug__: log('exception (failure #{}): {}', failures, str(ex))
             # Record the first error we get, not the subsequent ones, because
             # in the case of network outages, the subsequent ones will be
@@ -200,22 +200,25 @@
 
     # Interpret the response.
     code = req.status_code
     if code == 202:
         # Code 202 = Accepted, "received but not yet acted upon."
         sleep(1)                        # Sleep a short time and try again.
         recursing += 1
-        if __debug__: log('Calling download() recursively for http code 202')
+        if __debug__: log('calling download() recursively for http code 202')
         download(url, user, password, local_destination, recursing)
     elif 200 <= code < 400:
         # The following originally started out as the code here:
         # https://stackoverflow.com/a/39217788/743730
         with open(local_destination, 'wb') as f:
+            if __debug__: log('writing data to {}', local_destination)
             shutil.copyfileobj(req.raw, f)
         req.close()
+        size = stat(local_destination).st_size
+        if __debug__: log('wrote {} bytes to file {}', size, local_destination)
     elif code in [401, 402, 403, 407, 451, 511]:
         raise AuthenticationFailure(addurl('Access is forbidden'))
     elif code in [404, 410]:
         raise NoContent(addurl('No content found'))
     elif code in [405, 406, 409, 411, 412, 414, 417, 428, 431, 505, 510]:
         raise InternalError(addurl('Server returned code {}'.format(code)))
     elif code in [415, 416]:
```

### Comparing `eprints2bags-1.9.1/eprints2bags/processes.py` & `eprints2bags-1.9.2/eprints2bags/processes.py`

 * *Files identical despite different names*

### Comparing `eprints2bags-1.9.1/eprints2bags.egg-info/PKG-INFO` & `eprints2bags-1.9.2/eprints2bags.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eprints2bags
-Version: 1.9.1
+Version: 1.9.2
 Summary: Download EPrints content and save it in BagIt-format bags.
 Home-page: https://github.com/caltechlibrary/eprints2bags
 Author: Michael Hucka
 Author-email: mhucka@caltech.edu
 License: BSD 3-clause
 Project-URL: Source Code, https://github.com/caltechlibrary/eprints2bags
 Project-URL: Bug Tracker, https://github.com/caltechlibrary/eprints2bags/issues
@@ -16,23 +16,21 @@
         *Authors*:      [Michael Hucka](http://github.com/mhucka), [Betsy Coles](https://github.com/betsycoles)<br>
         *Repository*:   [https://github.com/caltechlibrary/eprints2bags](https://github.com/caltechlibrary/eprints2bags)<br>
         *License*:      BSD/MIT derivative &ndash; see the [LICENSE](LICENSE) file for more information
         
         [![License](https://img.shields.io/badge/License-BSD%203--Clause-blue.svg?style=flat-square)](https://choosealicense.com/licenses/bsd-3-clause)
         [![Python](https://img.shields.io/badge/Python-3.5+-brightgreen.svg?style=flat-square)](http://shields.io)
         [![Latest release](https://img.shields.io/github/v/release/caltechlibrary/eprints2bags.svg?style=flat-square&color=b44e88)](https://github.com/caltechlibrary/eprints2bags/releases)
-        [![DOI](http://img.shields.io/badge/DOI-10.22002%20%2f%20D1.1310-blue.svg?style=flat-square)](https://data.caltech.edu/records/1310)
+        [![DOI](http://img.shields.io/badge/DOI-10.22002%20%2f%20D1.1450-blue.svg?style=flat-square)](https://data.caltech.edu/records/1450)
         [![PyPI](https://img.shields.io/pypi/v/eprints2bags.svg?style=flat-square&color=red)](https://pypi.org/project/eprints2bags/)
         
         🏁 Log of recent changes
         -----------------------
         
-        _Version 1.9.1_: This release updates the README file to explain how to install from PyPI, and fixes some internal files related to producing releases on PyPI.
-        
-        _Version 1.9.0_: This release fixes a couple of minor bugs.  It also changes the debug flag letter to be `-@` and changes the behavior of the flag; these changes are not backward-compatible.  Internally, it changes the setup process to use `setup.cfg` and uses a new way to get package metadata.  Finally, this version is being made available from [PyPI](https://pypi.org/project/eprints2bags).
+        _Version 1.9.2_: **Critical fix** &ndash; this version fixes a bug that caused `eprints2bags` to write zero-length data files when used with newer versions of Python.  **You should upgrade your copy of `eprints2bags` to this version**.  This version also reports skipped records separately from missing records (in the final summary at the end of a run).
         
         The file [CHANGES](CHANGES.md) contains a more complete change log that includes information about previous releases.
         
         
         Table of Contents
         -----------------
         
@@ -66,15 +64,15 @@
         Then, to install `eprints2bags` from the Python package repository, run the following command:
         ```
         python3 -m pip install eprints2bags --user --upgrade
         ```
         
         As an alternative to getting it from PyPI, you can instruct `pip` to install `eprints2bags` directly from the GitHub repository:
         ```sh
-        python3 -m pip install git+https@github.com:caltechlibrary/eprints2bags.git --user --upgrade
+        python3 -m pip install git+https://github.com/caltechlibrary/eprints2bags.git --user --upgrade
         ```
         
         On Linux and macOS systems, assuming that the installation proceeds normally, you should end up with a program called `eprints2bags` in a location normally searched by your terminal shell for commands.
         
         
         ▶︎ Using Eprints2bags
         ---------------------
@@ -221,20 +219,20 @@
         | `-p`_P_ | `--password`_U_   | Password for EPrints proxy login | |
         | `-t`_T_ | `--arch-type`_T_  | Use archive type _T_ | Uncompressed ZIP | ♢ |
         | `-y`_Y_ | `--delay`_Y_      | Pause _Y_ ms between getting records | 100 milliseconds | |
         | `-C`    | `--no-color`      | Don't color-code the output | Use colors in the terminal output | |
         | `-K`    | `--no-keyring`    | Don't use a keyring/keychain | Store login info in keyring | |
         | `-R`    | `--reset`         | Reset user login & password used | Reuse previous credentials |
         | `-V`    | `--version`       | Print program version info and exit | Do other actions instead | |
-        | `-@`_OUT_ | `--debug`_OUT_    | Debugging mode; write trace to _OUT_ | Normal mode | ♣ |
+        | `-@`_OUT_ | `--debug`_OUT_    | Debugging mode; write trace to _OUT_ | Normal mode | ⚐ |
         
          ⚑ &nbsp; Required argument.<br>
         ✦ &nbsp; Possible values: `none`, `bag`, `bag-and-archive`.<br>
         ♢ &nbsp; Possible values: `uncompressed-zip`, `compressed-zip`, `uncompressed-tar`, `compressed-tar`.<br>
-        ♣ &nbsp; To write to the console, use the character `-` as the value of _OUT_; otherwise, _OUT_ must be the name of a file where the output should be written.
+        ⚐ &nbsp; To write to the console, use the character `-` as the value of _OUT_; otherwise, _OUT_ must be the name of a file where the output should be written.
         
         ### Additional notes and considerations
         
         Beware that some file systems have limitations on the number of subdirectories that can be created, which directly impacts how many record subdirectories can be created by this program.  `eprints2bags` attempts to guess the type of file system where the output is being written and warn the user if the number of records exceeds known maximums (e.g., 31,998 subdirectories for the [ext2](https://en.wikipedia.org/wiki/Ext2) and [ext3](https://en.wikipedia.org/wiki/Ext3) file systems in Linux), but its internal table does not include all possible file systems and it may not be able to warn users in all cases.  If you encounter file system limitations on the number of subdirectories that can be created, a simple solution is to manually create an intermediate level of subdirectories under the destination given to `-o`, then run `eprints2bags` multiple times, each time indicating a different subrange of records to the `-i` option and a different subdirectory to `-o`, such that the number of records written to each destination is below the file system's limit on total number of directories.
         
         It is also noteworthy that hitting a server for tens of thousands of records and documents in rapid succession is likely to draw suspicion from server administrators.  By default, this program inserts a small delay between record fetches (adjustable using the `-y` command-line option), which may be too short in some cases.  Setting the value to 0 is also possible, but might get you blocked or banned from an institution's servers.
         
@@ -313,9 +311,9 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Topic :: System :: Archiving
 Classifier: Topic :: System :: Archiving :: Packaging
 Classifier: Topic :: Utilities
-Requires-Python: >=3.5
+Requires-Python: >= 3.5
 Description-Content-Type: text/markdown
```

### Comparing `eprints2bags-1.9.1/eprints2bags.egg-info/SOURCES.txt` & `eprints2bags-1.9.2/eprints2bags.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `eprints2bags-1.9.1/setup.cfg` & `eprints2bags-1.9.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = eprints2bags
-version = 1.9.1
+version = 1.9.2
 description = Download EPrints content and save it in BagIt-format bags.
 author = Michael Hucka
 author_email = mhucka@caltech.edu
 license = BSD 3-clause
 license_files = LICENSE
 url = https://github.com/caltechlibrary/eprints2bags
 project_urls =
```

### Comparing `eprints2bags-1.9.1/setup.py` & `eprints2bags-1.9.2/setup.py`

 * *Files identical despite different names*

