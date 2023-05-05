# Comparing `tmp/datoso-0.2.2.tar.gz` & `tmp/datoso-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datoso-0.2.2.tar", last modified: Sun Apr 30 19:19:56 2023, max compression
+gzip compressed data, was "datoso-0.2.3.tar", last modified: Fri May  5 03:28:37 2023, max compression
```

## Comparing `datoso-0.2.2.tar` & `datoso-0.2.3.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 19:19:56.410938 datoso-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-30 19:19:38.000000 datoso-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-30 19:19:38.000000 datoso-0.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5584 2023-04-30 19:19:56.410938 datoso-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4768 2023-04-30 19:19:38.000000 datoso-0.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-04-30 19:19:38.000000 datoso-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-30 19:19:56.410938 datoso-0.2.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 19:19:56.402938 datoso-0.2.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 19:19:56.406938 datoso-0.2.2/src/datoso/
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-30 19:19:38.000000 datoso-0.2.2/src/datoso/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18019 2023-04-30 19:19:38.000000 datoso-0.2.2/src/datoso/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 19:19:56.406938 datoso-0.2.2/src/datoso/actions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 19:19:38.000000 datoso-0.2.2/src/datoso/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5316 2023-04-30 19:19:38.000000 datoso-0.2.2/src/datoso/actions/processor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 19:19:56.406938 datoso-0.2.2/src/datoso/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 19:19:38.000000 datoso-0.2.2/src/datoso/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-04-30 19:19:38.000000 datoso-0.2.2/src/datoso/commands/doctor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-04-30 19:19:38.000000 datoso-0.2.2/src/datoso/commands/seed.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 19:19:56.406938 datoso-0.2.2/src/datoso/configuration/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-30 19:19:38.000000 datoso-0.2.2/src/datoso/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-04-30 19:19:38.000000 datoso-0.2.2/src/datoso/configuration/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-04-30 19:19:38.000000 datoso-0.2.2/src/datoso/configuration/folder_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-04-30 19:19:38.000000 datoso-0.2.2/src/datoso/configuration/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 19:19:56.406938 datoso-0.2.2/src/datoso/database/
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-04-30 19:19:38.000000 datoso-0.2.2/src/datoso/database/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 19:19:56.410938 datoso-0.2.2/src/datoso/database/models/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-04-30 19:19:38.000000 datoso-0.2.2/src/datoso/database/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-04-30 19:19:38.000000 datoso-0.2.2/src/datoso/database/models/datfile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 19:19:56.410938 datoso-0.2.2/src/datoso/database/seeds/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 19:19:38.000000 datoso-0.2.2/src/datoso/database/seeds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-04-30 19:19:38.000000 datoso-0.2.2/src/datoso/database/seeds/dat_repos.py
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-04-30 19:19:38.000000 datoso-0.2.2/src/datoso/database/seeds/dat_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-04-30 19:19:38.000000 datoso-0.2.2/src/datoso/datoso.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 19:19:56.410938 datoso-0.2.2/src/datoso/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)     3347 2023-04-30 19:19:38.000000 datoso-0.2.2/src/datoso/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-04-30 19:19:38.000000 datoso-0.2.2/src/datoso/helpers/executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-04-30 19:19:38.000000 datoso-0.2.2/src/datoso/helpers/plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 19:19:56.410938 datoso-0.2.2/src/datoso/repositories/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 19:19:38.000000 datoso-0.2.2/src/datoso/repositories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13001 2023-04-30 19:19:38.000000 datoso-0.2.2/src/datoso/repositories/dat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-04-30 19:19:38.000000 datoso-0.2.2/src/datoso/repositories/dedupe.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 19:19:56.410938 datoso-0.2.2/src/datoso/seeds/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 19:19:38.000000 datoso-0.2.2/src/datoso/seeds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-04-30 19:19:38.000000 datoso-0.2.2/src/datoso/seeds/rules.py
--rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-04-30 19:19:38.000000 datoso-0.2.2/src/datoso/seeds/unknown_seed.py
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-04-30 19:19:38.000000 datoso-0.2.2/src/datoso/seeds.txt
--rw-r--r--   0 runner    (1001) docker     (123)    42016 2023-04-30 19:19:38.000000 datoso-0.2.2/src/datoso/systems.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 19:19:56.406938 datoso-0.2.2/src/datoso.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5584 2023-04-30 19:19:56.000000 datoso-0.2.2/src/datoso.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-04-30 19:19:56.000000 datoso-0.2.2/src/datoso.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 19:19:56.000000 datoso-0.2.2/src/datoso.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-30 19:19:56.000000 datoso-0.2.2/src/datoso.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-30 19:19:56.000000 datoso-0.2.2/src/datoso.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-30 19:19:56.000000 datoso-0.2.2/src/datoso.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 03:28:37.368187 datoso-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-05 03:28:21.000000 datoso-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-05 03:28:21.000000 datoso-0.2.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5600 2023-05-05 03:28:37.368187 datoso-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4665 2023-05-05 03:28:21.000000 datoso-0.2.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-05-05 03:28:21.000000 datoso-0.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-05 03:28:37.368187 datoso-0.2.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 03:28:37.364187 datoso-0.2.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 03:28:37.364187 datoso-0.2.3/src/datoso/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-05 03:28:21.000000 datoso-0.2.3/src/datoso/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18019 2023-05-05 03:28:21.000000 datoso-0.2.3/src/datoso/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 03:28:37.364187 datoso-0.2.3/src/datoso/actions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 03:28:21.000000 datoso-0.2.3/src/datoso/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5316 2023-05-05 03:28:21.000000 datoso-0.2.3/src/datoso/actions/processor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 03:28:37.368187 datoso-0.2.3/src/datoso/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 03:28:21.000000 datoso-0.2.3/src/datoso/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-05-05 03:28:21.000000 datoso-0.2.3/src/datoso/commands/doctor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3848 2023-05-05 03:28:21.000000 datoso-0.2.3/src/datoso/commands/seed.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 03:28:37.368187 datoso-0.2.3/src/datoso/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-05 03:28:21.000000 datoso-0.2.3/src/datoso/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-05 03:28:21.000000 datoso-0.2.3/src/datoso/configuration/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-05-05 03:28:21.000000 datoso-0.2.3/src/datoso/configuration/folder_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-05-05 03:28:21.000000 datoso-0.2.3/src/datoso/configuration/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 03:28:37.368187 datoso-0.2.3/src/datoso/database/
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-05-05 03:28:21.000000 datoso-0.2.3/src/datoso/database/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 03:28:37.368187 datoso-0.2.3/src/datoso/database/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-05 03:28:21.000000 datoso-0.2.3/src/datoso/database/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-05-05 03:28:21.000000 datoso-0.2.3/src/datoso/database/models/datfile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 03:28:37.368187 datoso-0.2.3/src/datoso/database/seeds/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 03:28:21.000000 datoso-0.2.3/src/datoso/database/seeds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-05-05 03:28:21.000000 datoso-0.2.3/src/datoso/database/seeds/dat_repos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-05-05 03:28:21.000000 datoso-0.2.3/src/datoso/database/seeds/dat_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-05-05 03:28:21.000000 datoso-0.2.3/src/datoso/datoso.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 03:28:37.368187 datoso-0.2.3/src/datoso/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)     3347 2023-05-05 03:28:21.000000 datoso-0.2.3/src/datoso/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-05-05 03:28:21.000000 datoso-0.2.3/src/datoso/helpers/executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-05-05 03:28:21.000000 datoso-0.2.3/src/datoso/helpers/plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 03:28:37.368187 datoso-0.2.3/src/datoso/repositories/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 03:28:21.000000 datoso-0.2.3/src/datoso/repositories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13001 2023-05-05 03:28:21.000000 datoso-0.2.3/src/datoso/repositories/dat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-05-05 03:28:21.000000 datoso-0.2.3/src/datoso/repositories/dedupe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 03:28:37.368187 datoso-0.2.3/src/datoso/seeds/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 03:28:21.000000 datoso-0.2.3/src/datoso/seeds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-05-05 03:28:21.000000 datoso-0.2.3/src/datoso/seeds/rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-05-05 03:28:21.000000 datoso-0.2.3/src/datoso/seeds/unknown_seed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-05-05 03:28:21.000000 datoso-0.2.3/src/datoso/seeds.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    42230 2023-05-05 03:28:21.000000 datoso-0.2.3/src/datoso/systems.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 03:28:37.364187 datoso-0.2.3/src/datoso.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5600 2023-05-05 03:28:37.000000 datoso-0.2.3/src/datoso.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-05-05 03:28:37.000000 datoso-0.2.3/src/datoso.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 03:28:37.000000 datoso-0.2.3/src/datoso.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-05 03:28:37.000000 datoso-0.2.3/src/datoso.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-05-05 03:28:37.000000 datoso-0.2.3/src/datoso.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-05 03:28:37.000000 datoso-0.2.3/src/datoso.egg-info/top_level.txt
```

### Comparing `datoso-0.2.2/LICENSE` & `datoso-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `datoso-0.2.2/PKG-INFO` & `datoso-0.2.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datoso
-Version: 0.2.2
+Version: 0.2.3
 Summary: Python command line tool to download and organize your Rom Dat files.
 Author-email: Lacides Miranda <laromicas@hotmail.com>
 License: MIT License
 Project-URL: Source Code, https://github.com/laromicas/datoso
 Keywords: emulators,roms
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
@@ -12,17 +12,21 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: System :: Emulators
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: all
 Provides-Extra: fbneo
+Provides-Extra: md_enhanced
 Provides-Extra: nointro
 Provides-Extra: pleasuredome
 Provides-Extra: redump
+Provides-Extra: sfc_enhancedcolors
+Provides-Extra: sfc_msu1
+Provides-Extra: sfc_speedhacks
 Provides-Extra: translatedenglish
 Provides-Extra: dev
 License-File: LICENSE
 
 ![Datoso](/bearlogo.png)
 
 # Datoso
@@ -121,60 +125,56 @@
 
 Be careful when updating dats from datomatic, sometimes they put a
 captcha, and you may be banned if the captcha fails, captcha support is
 OTW.
 
 ## TODO (without priority)
 
--   Datoso Initialization
 -   Change logo
 -   Change pydantic to dataclasses
 -   Better rules update process
     -   Make update rules write to database only when finished
 -   Tests
 -   More dat repositories
 -   Mega.nz download support (<https://pypi.org/project/mega.py/>)
 -   Zippyshare download support (<https://pypi.org/project/zippyshare-downloader/>)
 -   Zippyshare download support (<https://pypi.org/project/pyOneFichierClient/>)
 -   Configurable folder structure (instead of emulator-focused structure use dat-repositories or viceversa)
     -   Maybe with a builder, to avoid the need to change the code anytime
--   Modular design for repositories (done for seeds, repositores missing)
 
 
-*(*) Done but to be improved*
-*(**) Did it Yay!!!*
-
 ## USEFUL DEVELOPMENT COMMANDS
 
 ```bash
 # Find folders with more than one dat file:
 $ find . -type f -iname '*.dat' -printf '%h\n'|sort|uniq -cd
 
 # Find and delete empty folders:
 $ find . -type d -empty -print -delete
 
 # Pylint
 $ pylint src --errors-only
 $ pylint src --disable=all --enable=missing-function-docstring
+
+# Find duplicate names different case
+$ find . | sort -f | uniq -i -d
 ```
 
 ## WISHLIST (without priority)
 
 -   Dat structure for ClrMamePro or another dat manager.
 -   Web interface
 -   Download from central repositories (an S3 or something like that to prevent overload main sites)
     -   Lambda to download dats and upload to S3
     -   Downloading from S3
 -   Auto-Import MIA Lists (for redump)
     -   Add \[MIA\] to dat roms
 -   Remove MIA from dats
 -   .cue Generator
 
-*(**) Did it Yay!!!*
-
 ## Contributing
 
 Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
 Please make sure to update tests as appropriate.
 
 ## License
```

### Comparing `datoso-0.2.2/README.md` & `datoso-0.2.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -96,60 +96,56 @@
 
 Be careful when updating dats from datomatic, sometimes they put a
 captcha, and you may be banned if the captcha fails, captcha support is
 OTW.
 
 ## TODO (without priority)
 
--   Datoso Initialization
 -   Change logo
 -   Change pydantic to dataclasses
 -   Better rules update process
     -   Make update rules write to database only when finished
 -   Tests
 -   More dat repositories
 -   Mega.nz download support (<https://pypi.org/project/mega.py/>)
 -   Zippyshare download support (<https://pypi.org/project/zippyshare-downloader/>)
 -   Zippyshare download support (<https://pypi.org/project/pyOneFichierClient/>)
 -   Configurable folder structure (instead of emulator-focused structure use dat-repositories or viceversa)
     -   Maybe with a builder, to avoid the need to change the code anytime
--   Modular design for repositories (done for seeds, repositores missing)
 
 
-*(*) Done but to be improved*
-*(**) Did it Yay!!!*
-
 ## USEFUL DEVELOPMENT COMMANDS
 
 ```bash
 # Find folders with more than one dat file:
 $ find . -type f -iname '*.dat' -printf '%h\n'|sort|uniq -cd
 
 # Find and delete empty folders:
 $ find . -type d -empty -print -delete
 
 # Pylint
 $ pylint src --errors-only
 $ pylint src --disable=all --enable=missing-function-docstring
+
+# Find duplicate names different case
+$ find . | sort -f | uniq -i -d
 ```
 
 ## WISHLIST (without priority)
 
 -   Dat structure for ClrMamePro or another dat manager.
 -   Web interface
 -   Download from central repositories (an S3 or something like that to prevent overload main sites)
     -   Lambda to download dats and upload to S3
     -   Downloading from S3
 -   Auto-Import MIA Lists (for redump)
     -   Add \[MIA\] to dat roms
 -   Remove MIA from dats
 -   .cue Generator
 
-*(**) Did it Yay!!!*
-
 ## Contributing
 
 Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
 Please make sure to update tests as appropriate.
 
 ## License
```

### Comparing `datoso-0.2.2/src/datoso/__main__.py` & `datoso-0.2.3/src/datoso/__main__.py`

 * *Files identical despite different names*

### Comparing `datoso-0.2.2/src/datoso/actions/processor.py` & `datoso-0.2.3/src/datoso/actions/processor.py`

 * *Files identical despite different names*

### Comparing `datoso-0.2.2/src/datoso/commands/doctor.py` & `datoso-0.2.3/src/datoso/commands/doctor.py`

 * *Files identical despite different names*

### Comparing `datoso-0.2.2/src/datoso/commands/seed.py` & `datoso-0.2.3/src/datoso/commands/seed.py`

 * *Files 5% similar despite different names*

```diff
@@ -40,15 +40,18 @@
     def process_dats(self, fltr=None):
         """ Process dats."""
         def delete_line(line):
             # pylint: disable=expression-not-assigned
             [print('\b \b', end='') for x in range(0, len(line))]
             print(' ' * (len(line)), end='')
             print('\r', end='')
-        dat_origin = os.path.join(FileUtils.parse_folder(config['PATHS'].get('DownloadPath', 'tmp')), self.name, 'dats')
+        def get_preffix(name):
+            seed = get_seed(name)
+            return seed.__preffix__ if seed else name
+        dat_origin = os.path.join(FileUtils.parse_folder(config['PATHS'].get('DownloadPath', 'tmp')), get_preffix(self.name), 'dats')
         line = ''
         for path, actions in self.actions.items():
             new_path = path.format(dat_origin=dat_origin)
             actions = self.format_actions(actions, data={'dat_destination': config['PATHS'].get('DatPath', 'DatRoot')})
             for file in os.listdir(new_path) if os.path.isdir(new_path) else []:
                 if config['PROCESS'].get('DatIgnoreRegEx'):
                     ignore_regex = re.compile(config['PROCESS']['DatIgnoreRegEx'])
```

### Comparing `datoso-0.2.2/src/datoso/configuration/folder_helper.py` & `datoso-0.2.3/src/datoso/configuration/folder_helper.py`

 * *Files identical despite different names*

### Comparing `datoso-0.2.2/src/datoso/configuration/logger.py` & `datoso-0.2.3/src/datoso/configuration/logger.py`

 * *Files identical despite different names*

### Comparing `datoso-0.2.2/src/datoso/database/__init__.py` & `datoso-0.2.3/src/datoso/database/__init__.py`

 * *Files identical despite different names*

### Comparing `datoso-0.2.2/src/datoso/database/models/datfile.py` & `datoso-0.2.3/src/datoso/database/models/datfile.py`

 * *Files identical despite different names*

### Comparing `datoso-0.2.2/src/datoso/database/seeds/dat_repos.py` & `datoso-0.2.3/src/datoso/database/seeds/dat_repos.py`

 * *Files identical despite different names*

### Comparing `datoso-0.2.2/src/datoso/database/seeds/dat_rules.py` & `datoso-0.2.3/src/datoso/database/seeds/dat_rules.py`

 * *Files identical despite different names*

### Comparing `datoso-0.2.2/src/datoso/datoso.ini` & `datoso-0.2.3/src/datoso/datoso.ini`

 * *Files identical despite different names*

### Comparing `datoso-0.2.2/src/datoso/helpers/__init__.py` & `datoso-0.2.3/src/datoso/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `datoso-0.2.2/src/datoso/helpers/executor.py` & `datoso-0.2.3/src/datoso/helpers/executor.py`

 * *Files identical despite different names*

### Comparing `datoso-0.2.2/src/datoso/repositories/dat.py` & `datoso-0.2.3/src/datoso/repositories/dat.py`

 * *Files identical despite different names*

### Comparing `datoso-0.2.2/src/datoso/repositories/dedupe.py` & `datoso-0.2.3/src/datoso/repositories/dedupe.py`

 * *Files identical despite different names*

### Comparing `datoso-0.2.2/src/datoso/seeds/unknown_seed.py` & `datoso-0.2.3/src/datoso/seeds/unknown_seed.py`

 * *Files identical despite different names*

### Comparing `datoso-0.2.2/src/datoso/seeds.txt` & `datoso-0.2.3/src/datoso/seeds.txt`

 * *Files identical despite different names*

### Comparing `datoso-0.2.2/src/datoso/systems.json` & `datoso-0.2.3/src/datoso/systems.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9962121212121212%*

 * *Differences: {'insert': "[(179, OrderedDict([('company', 'Sega'), ('system', 'Mega CD Hacks'), ('override', "*

 * *           "OrderedDict([('system', 'Mega CD & Sega CD'), ('suffix', 'Hacks')])), ('system_type', "*

 * *           "'Console')]))]"}*

```diff
@@ -1295,14 +1295,23 @@
             }
         },
         "system": "Saturn",
         "system_type": "Console"
     },
     {
         "company": "Sega",
+        "override": {
+            "suffix": "Hacks",
+            "system": "Mega CD & Sega CD"
+        },
+        "system": "Mega CD Hacks",
+        "system_type": "Console"
+    },
+    {
+        "company": "Sega",
         "extra_configs": {
             "empty_suffix": {
                 "redump": "Discs"
             }
         },
         "override": {
             "system": "Mega CD & Sega CD"
```

### Comparing `datoso-0.2.2/src/datoso.egg-info/PKG-INFO` & `datoso-0.2.3/src/datoso.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datoso
-Version: 0.2.2
+Version: 0.2.3
 Summary: Python command line tool to download and organize your Rom Dat files.
 Author-email: Lacides Miranda <laromicas@hotmail.com>
 License: MIT License
 Project-URL: Source Code, https://github.com/laromicas/datoso
 Keywords: emulators,roms
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
@@ -12,17 +12,21 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: System :: Emulators
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: all
 Provides-Extra: fbneo
+Provides-Extra: md_enhanced
 Provides-Extra: nointro
 Provides-Extra: pleasuredome
 Provides-Extra: redump
+Provides-Extra: sfc_enhancedcolors
+Provides-Extra: sfc_msu1
+Provides-Extra: sfc_speedhacks
 Provides-Extra: translatedenglish
 Provides-Extra: dev
 License-File: LICENSE
 
 ![Datoso](/bearlogo.png)
 
 # Datoso
@@ -121,60 +125,56 @@
 
 Be careful when updating dats from datomatic, sometimes they put a
 captcha, and you may be banned if the captcha fails, captcha support is
 OTW.
 
 ## TODO (without priority)
 
--   Datoso Initialization
 -   Change logo
 -   Change pydantic to dataclasses
 -   Better rules update process
     -   Make update rules write to database only when finished
 -   Tests
 -   More dat repositories
 -   Mega.nz download support (<https://pypi.org/project/mega.py/>)
 -   Zippyshare download support (<https://pypi.org/project/zippyshare-downloader/>)
 -   Zippyshare download support (<https://pypi.org/project/pyOneFichierClient/>)
 -   Configurable folder structure (instead of emulator-focused structure use dat-repositories or viceversa)
     -   Maybe with a builder, to avoid the need to change the code anytime
--   Modular design for repositories (done for seeds, repositores missing)
 
 
-*(*) Done but to be improved*
-*(**) Did it Yay!!!*
-
 ## USEFUL DEVELOPMENT COMMANDS
 
 ```bash
 # Find folders with more than one dat file:
 $ find . -type f -iname '*.dat' -printf '%h\n'|sort|uniq -cd
 
 # Find and delete empty folders:
 $ find . -type d -empty -print -delete
 
 # Pylint
 $ pylint src --errors-only
 $ pylint src --disable=all --enable=missing-function-docstring
+
+# Find duplicate names different case
+$ find . | sort -f | uniq -i -d
 ```
 
 ## WISHLIST (without priority)
 
 -   Dat structure for ClrMamePro or another dat manager.
 -   Web interface
 -   Download from central repositories (an S3 or something like that to prevent overload main sites)
     -   Lambda to download dats and upload to S3
     -   Downloading from S3
 -   Auto-Import MIA Lists (for redump)
     -   Add \[MIA\] to dat roms
 -   Remove MIA from dats
 -   .cue Generator
 
-*(**) Did it Yay!!!*
-
 ## Contributing
 
 Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
 Please make sure to update tests as appropriate.
 
 ## License
```

### Comparing `datoso-0.2.2/src/datoso.egg-info/SOURCES.txt` & `datoso-0.2.3/src/datoso.egg-info/SOURCES.txt`

 * *Files identical despite different names*

