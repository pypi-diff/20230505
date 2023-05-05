# Comparing `tmp/google_benchmark-1.7.1.tar.gz` & `tmp/google_benchmark-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google_benchmark-1.7.1.tar", last modified: Fri Nov 11 14:02:56 2022, max compression
+gzip compressed data, was "google_benchmark-1.8.0.tar", last modified: Fri May  5 10:27:36 2023, max compression
```

## Comparing `google_benchmark-1.7.1.tar` & `google_benchmark-1.8.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 14:02:56.405317 google_benchmark-1.7.1/
--rw-r--r--   0 runner    (1001) docker     (121)     2488 2022-11-11 14:02:55.000000 google_benchmark-1.7.1/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (121)    11358 2022-11-11 14:02:55.000000 google_benchmark-1.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     8413 2022-11-11 14:02:56.405317 google_benchmark-1.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     7515 2022-11-11 14:02:55.000000 google_benchmark-1.7.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 14:02:56.401317 google_benchmark-1.7.1/bindings/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 14:02:56.401317 google_benchmark-1.7.1/bindings/python/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 14:02:56.405317 google_benchmark-1.7.1/bindings/python/google_benchmark/
--rw-r--r--   0 runner    (1001) docker     (121)     4462 2022-11-11 14:02:55.000000 google_benchmark-1.7.1/bindings/python/google_benchmark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3857 2022-11-11 14:02:55.000000 google_benchmark-1.7.1/bindings/python/google_benchmark/example.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-11 14:02:56.405317 google_benchmark-1.7.1/bindings/python/google_benchmark.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     8413 2022-11-11 14:02:56.000000 google_benchmark-1.7.1/bindings/python/google_benchmark.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      457 2022-11-11 14:02:56.000000 google_benchmark-1.7.1/bindings/python/google_benchmark.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-11 14:02:56.000000 google_benchmark-1.7.1/bindings/python/google_benchmark.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-11 14:02:56.000000 google_benchmark-1.7.1/bindings/python/google_benchmark.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-11-11 14:02:56.000000 google_benchmark-1.7.1/bindings/python/google_benchmark.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-11-11 14:02:56.000000 google_benchmark-1.7.1/bindings/python/google_benchmark.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-11 14:02:56.405317 google_benchmark-1.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     5297 2022-11-11 14:02:55.000000 google_benchmark-1.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:27:36.643857 google_benchmark-1.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-05-05 10:27:35.000000 google_benchmark-1.8.0/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-05 10:27:35.000000 google_benchmark-1.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8637 2023-05-05 10:27:36.643857 google_benchmark-1.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7809 2023-05-05 10:27:35.000000 google_benchmark-1.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:27:36.639857 google_benchmark-1.8.0/bindings/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:27:36.639857 google_benchmark-1.8.0/bindings/python/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:27:36.639857 google_benchmark-1.8.0/bindings/python/google_benchmark/
+-rw-r--r--   0 runner    (1001) docker     (123)     4463 2023-05-05 10:27:35.000000 google_benchmark-1.8.0/bindings/python/google_benchmark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3858 2023-05-05 10:27:35.000000 google_benchmark-1.8.0/bindings/python/google_benchmark/example.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:27:36.643857 google_benchmark-1.8.0/bindings/python/google_benchmark.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8637 2023-05-05 10:27:36.000000 google_benchmark-1.8.0/bindings/python/google_benchmark.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-05-05 10:27:36.000000 google_benchmark-1.8.0/bindings/python/google_benchmark.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 10:27:36.000000 google_benchmark-1.8.0/bindings/python/google_benchmark.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 10:27:36.000000 google_benchmark-1.8.0/bindings/python/google_benchmark.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-05 10:27:36.000000 google_benchmark-1.8.0/bindings/python/google_benchmark.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-05 10:27:36.000000 google_benchmark-1.8.0/bindings/python/google_benchmark.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 10:27:36.643857 google_benchmark-1.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5661 2023-05-05 10:27:35.000000 google_benchmark-1.8.0/setup.py
```

### Comparing `google_benchmark-1.7.1/AUTHORS` & `google_benchmark-1.8.0/AUTHORS`

 * *Files 6% similar despite different names*

```diff
@@ -28,26 +28,29 @@
 Eric Fiselier <eric@efcs.ca>
 Eugene Zhuk <eugene.zhuk@gmail.com>
 Evgeny Safronov <division494@gmail.com>
 Federico Ficarelli <federico.ficarelli@gmail.com>
 Felix Homann <linuxaudio@showlabor.de>
 Gergő Szitár <szitar.gergo@gmail.com>
 Google Inc.
+Henrique Bucher <hbucher@gmail.com>
 International Business Machines Corporation
 Ismael Jimenez Martinez <ismael.jimenez.martinez@gmail.com>
 Jern-Kuan Leong <jernkuan@gmail.com>
 JianXiong Zhou <zhoujianxiong2@gmail.com>
 Joao Paulo Magalhaes <joaoppmagalhaes@gmail.com>
 Jordan Williams <jwillikers@protonmail.com>
 Jussi Knuuttila <jussi.knuuttila@gmail.com>
 Kaito Udagawa <umireon@gmail.com>
 Kishan Kumar <kumar.kishan@outlook.com>
 Lei Xu <eddyxu@gmail.com>
+Marcel Jacobse <mjacobse@uni-bremen.de>
 Matt Clarkson <mattyclarkson@gmail.com>
 Maxim Vafin <maxvafin@gmail.com>
+Mike Apodaca <gatorfax@gmail.com>
 MongoDB Inc.
 Nick Hutchinson <nshutchinson@gmail.com>
 Norman Heino <norman.heino@gmail.com>
 Oleksandr Sochka <sasha.sochka@gmail.com>
 Ori Livneh <ori.livneh@gmail.com>
 Paul Redmond <paul.redmond@gmail.com>
 Raghu Raja <raghu@enfabrica.net>
```

### Comparing `google_benchmark-1.7.1/LICENSE` & `google_benchmark-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `google_benchmark-1.7.1/PKG-INFO` & `google_benchmark-1.8.0/bindings/python/google_benchmark.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 Metadata-Version: 2.1
-Name: google_benchmark
-Version: 1.7.1
+Name: google-benchmark
+Version: 1.8.0
 Summary: A library to benchmark code snippets.
 Home-page: https://github.com/google/benchmark
 Author: Google
 Author-email: benchmark-py@google.com
 License: Apache 2.0
 Keywords: benchmark
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: System :: Benchmark
 Description-Content-Type: text/markdown
@@ -26,15 +24,15 @@
 # Benchmark
 
 [![build-and-test](https://github.com/google/benchmark/workflows/build-and-test/badge.svg)](https://github.com/google/benchmark/actions?query=workflow%3Abuild-and-test)
 [![bazel](https://github.com/google/benchmark/actions/workflows/bazel.yml/badge.svg)](https://github.com/google/benchmark/actions/workflows/bazel.yml)
 [![pylint](https://github.com/google/benchmark/workflows/pylint/badge.svg)](https://github.com/google/benchmark/actions?query=workflow%3Apylint)
 [![test-bindings](https://github.com/google/benchmark/workflows/test-bindings/badge.svg)](https://github.com/google/benchmark/actions?query=workflow%3Atest-bindings)
 
-[![Build Status](https://travis-ci.org/google/benchmark.svg?branch=master)](https://travis-ci.org/google/benchmark)
+[![Build Status](https://travis-ci.org/google/benchmark.svg?branch=main)](https://travis-ci.org/google/benchmark)
 [![Coverage Status](https://coveralls.io/repos/google/benchmark/badge.svg)](https://coveralls.io/r/google/benchmark)
 
 
 A library to benchmark code snippets, similar to unit tests. Example:
 
 ```c++
 #include <benchmark/benchmark.h>
@@ -54,15 +52,15 @@
 
 ## Getting Started
 
 To get started, see [Requirements](#requirements) and
 [Installation](#installation). See [Usage](#usage) for a full example and the
 [User Guide](docs/user_guide.md) for a more comprehensive feature overview.
 
-It may also help to read the [Google Test documentation](https://github.com/google/googletest/blob/master/docs/primer.md)
+It may also help to read the [Google Test documentation](https://github.com/google/googletest/blob/main/docs/primer.md)
 as some of the structural aspects of the APIs are similar.
 
 ## Resources
 
 [Discussion group](https://groups.google.com/d/forum/benchmark-discuss)
 
 IRC channels:
@@ -160,14 +158,20 @@
 
 If you are using gcc, you might need to set `GCC_AR` and `GCC_RANLIB` cmake
 cache variables, if autodetection fails.
 
 If you are using clang, you may need to set `LLVMAR_EXECUTABLE`,
 `LLVMNM_EXECUTABLE` and `LLVMRANLIB_EXECUTABLE` cmake cache variables.
 
+To enable sanitizer checks (eg., `asan` and `tsan`), add:
+```
+ -DCMAKE_C_FLAGS="-g -O2 -fno-omit-frame-pointer -fsanitize=address -fsanitize=thread -fno-sanitize-recover=all"
+ -DCMAKE_CXX_FLAGS="-g -O2 -fno-omit-frame-pointer -fsanitize=address -fsanitize=thread -fno-sanitize-recover=all "  
+```
+
 ### Stable and Experimental Library Versions
 
 The main branch contains the latest stable version of the benchmarking library;
 the API of which can be considered largely stable, with source breaking changes
 being made only upon the release of a new major version.
 
 Newer, experimental, features are implemented and tested on the
@@ -237,9 +241,7 @@
 ```cmake
 add_subdirectory(benchmark)
 ```
 Either way, link to the library as follows.
 ```cmake
 target_link_libraries(MyTarget benchmark::benchmark)
 ```
-
-
```

### Comparing `google_benchmark-1.7.1/README.md` & `google_benchmark-1.8.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,38 @@
+Metadata-Version: 2.1
+Name: google_benchmark
+Version: 1.8.0
+Summary: A library to benchmark code snippets.
+Home-page: https://github.com/google/benchmark
+Author: Google
+Author-email: benchmark-py@google.com
+License: Apache 2.0
+Keywords: benchmark
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Testing
+Classifier: Topic :: System :: Benchmark
+Description-Content-Type: text/markdown
+License-File: LICENSE
+License-File: AUTHORS
+
 # Benchmark
 
 [![build-and-test](https://github.com/google/benchmark/workflows/build-and-test/badge.svg)](https://github.com/google/benchmark/actions?query=workflow%3Abuild-and-test)
 [![bazel](https://github.com/google/benchmark/actions/workflows/bazel.yml/badge.svg)](https://github.com/google/benchmark/actions/workflows/bazel.yml)
 [![pylint](https://github.com/google/benchmark/workflows/pylint/badge.svg)](https://github.com/google/benchmark/actions?query=workflow%3Apylint)
 [![test-bindings](https://github.com/google/benchmark/workflows/test-bindings/badge.svg)](https://github.com/google/benchmark/actions?query=workflow%3Atest-bindings)
 
-[![Build Status](https://travis-ci.org/google/benchmark.svg?branch=master)](https://travis-ci.org/google/benchmark)
+[![Build Status](https://travis-ci.org/google/benchmark.svg?branch=main)](https://travis-ci.org/google/benchmark)
 [![Coverage Status](https://coveralls.io/repos/google/benchmark/badge.svg)](https://coveralls.io/r/google/benchmark)
 
 
 A library to benchmark code snippets, similar to unit tests. Example:
 
 ```c++
 #include <benchmark/benchmark.h>
@@ -29,15 +52,15 @@
 
 ## Getting Started
 
 To get started, see [Requirements](#requirements) and
 [Installation](#installation). See [Usage](#usage) for a full example and the
 [User Guide](docs/user_guide.md) for a more comprehensive feature overview.
 
-It may also help to read the [Google Test documentation](https://github.com/google/googletest/blob/master/docs/primer.md)
+It may also help to read the [Google Test documentation](https://github.com/google/googletest/blob/main/docs/primer.md)
 as some of the structural aspects of the APIs are similar.
 
 ## Resources
 
 [Discussion group](https://groups.google.com/d/forum/benchmark-discuss)
 
 IRC channels:
@@ -135,14 +158,20 @@
 
 If you are using gcc, you might need to set `GCC_AR` and `GCC_RANLIB` cmake
 cache variables, if autodetection fails.
 
 If you are using clang, you may need to set `LLVMAR_EXECUTABLE`,
 `LLVMNM_EXECUTABLE` and `LLVMRANLIB_EXECUTABLE` cmake cache variables.
 
+To enable sanitizer checks (eg., `asan` and `tsan`), add:
+```
+ -DCMAKE_C_FLAGS="-g -O2 -fno-omit-frame-pointer -fsanitize=address -fsanitize=thread -fno-sanitize-recover=all"
+ -DCMAKE_CXX_FLAGS="-g -O2 -fno-omit-frame-pointer -fsanitize=address -fsanitize=thread -fno-sanitize-recover=all "  
+```
+
 ### Stable and Experimental Library Versions
 
 The main branch contains the latest stable version of the benchmarking library;
 the API of which can be considered largely stable, with source breaking changes
 being made only upon the release of a new major version.
 
 Newer, experimental, features are implemented and tested on the
```

### Comparing `google_benchmark-1.7.1/bindings/python/google_benchmark/__init__.py` & `google_benchmark-1.8.0/bindings/python/google_benchmark/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,15 +65,15 @@
     "oLogN",
     "oNLogN",
     "oAuto",
     "oLambda",
     "State",
 ]
 
-__version__ = "1.7.1"
+__version__ = "1.8.0"
 
 
 class __OptionMaker:
     """A stateless class to collect benchmark options.
 
     Collect all decorator calls like @option.range(start=0, limit=1<<5).
     """
@@ -100,15 +100,15 @@
 
             # The decorator that get called, either with the benchmared function
             # or the previous Options
             def __decorator(func_or_options):
                 options = self.make(func_or_options)
                 options.builder_calls.append((builder_name, args, kwargs))
                 # The decorator returns Options so it is not technically a decorator
-                # and needs a final call to @regiser
+                # and needs a final call to @register
                 return options
 
             return __decorator
 
         return __builder_method
```

### Comparing `google_benchmark-1.7.1/bindings/python/google_benchmark/example.py` & `google_benchmark-1.8.0/bindings/python/google_benchmark/example.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,15 +68,15 @@
         time.sleep(0.01)
         end = time.perf_counter()
         state.set_iteration_time(end - start)
 
 
 @benchmark.register
 def custom_counters(state):
-    """Collect cutom metric using benchmark.Counter."""
+    """Collect custom metric using benchmark.Counter."""
     num_foo = 0.0
     while state:
         # Benchmark some code here
         pass
         # Collect some custom metric named foo
         num_foo += 0.13
```

### Comparing `google_benchmark-1.7.1/bindings/python/google_benchmark.egg-info/PKG-INFO` & `google_benchmark-1.8.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,40 +1,15 @@
-Metadata-Version: 2.1
-Name: google-benchmark
-Version: 1.7.1
-Summary: A library to benchmark code snippets.
-Home-page: https://github.com/google/benchmark
-Author: Google
-Author-email: benchmark-py@google.com
-License: Apache 2.0
-Keywords: benchmark
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Software Development :: Testing
-Classifier: Topic :: System :: Benchmark
-Description-Content-Type: text/markdown
-License-File: LICENSE
-License-File: AUTHORS
-
 # Benchmark
 
 [![build-and-test](https://github.com/google/benchmark/workflows/build-and-test/badge.svg)](https://github.com/google/benchmark/actions?query=workflow%3Abuild-and-test)
 [![bazel](https://github.com/google/benchmark/actions/workflows/bazel.yml/badge.svg)](https://github.com/google/benchmark/actions/workflows/bazel.yml)
 [![pylint](https://github.com/google/benchmark/workflows/pylint/badge.svg)](https://github.com/google/benchmark/actions?query=workflow%3Apylint)
 [![test-bindings](https://github.com/google/benchmark/workflows/test-bindings/badge.svg)](https://github.com/google/benchmark/actions?query=workflow%3Atest-bindings)
 
-[![Build Status](https://travis-ci.org/google/benchmark.svg?branch=master)](https://travis-ci.org/google/benchmark)
+[![Build Status](https://travis-ci.org/google/benchmark.svg?branch=main)](https://travis-ci.org/google/benchmark)
 [![Coverage Status](https://coveralls.io/repos/google/benchmark/badge.svg)](https://coveralls.io/r/google/benchmark)
 
 
 A library to benchmark code snippets, similar to unit tests. Example:
 
 ```c++
 #include <benchmark/benchmark.h>
@@ -54,15 +29,15 @@
 
 ## Getting Started
 
 To get started, see [Requirements](#requirements) and
 [Installation](#installation). See [Usage](#usage) for a full example and the
 [User Guide](docs/user_guide.md) for a more comprehensive feature overview.
 
-It may also help to read the [Google Test documentation](https://github.com/google/googletest/blob/master/docs/primer.md)
+It may also help to read the [Google Test documentation](https://github.com/google/googletest/blob/main/docs/primer.md)
 as some of the structural aspects of the APIs are similar.
 
 ## Resources
 
 [Discussion group](https://groups.google.com/d/forum/benchmark-discuss)
 
 IRC channels:
@@ -160,14 +135,20 @@
 
 If you are using gcc, you might need to set `GCC_AR` and `GCC_RANLIB` cmake
 cache variables, if autodetection fails.
 
 If you are using clang, you may need to set `LLVMAR_EXECUTABLE`,
 `LLVMNM_EXECUTABLE` and `LLVMRANLIB_EXECUTABLE` cmake cache variables.
 
+To enable sanitizer checks (eg., `asan` and `tsan`), add:
+```
+ -DCMAKE_C_FLAGS="-g -O2 -fno-omit-frame-pointer -fsanitize=address -fsanitize=thread -fno-sanitize-recover=all"
+ -DCMAKE_CXX_FLAGS="-g -O2 -fno-omit-frame-pointer -fsanitize=address -fsanitize=thread -fno-sanitize-recover=all "  
+```
+
 ### Stable and Experimental Library Versions
 
 The main branch contains the latest stable version of the benchmarking library;
 the API of which can be considered largely stable, with source breaking changes
 being made only upon the release of a new major version.
 
 Newer, experimental, features are implemented and tested on the
@@ -237,9 +218,7 @@
 ```cmake
 add_subdirectory(benchmark)
 ```
 Either way, link to the library as follows.
 ```cmake
 target_link_libraries(MyTarget benchmark::benchmark)
 ```
-
-
```

### Comparing `google_benchmark-1.7.1/setup.py` & `google_benchmark-1.8.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,135 +1,142 @@
+import contextlib
 import os
-import posixpath
 import platform
-import re
 import shutil
-import sys
+import sysconfig
+from pathlib import Path
+from typing import List
 
-from distutils import sysconfig
 import setuptools
 from setuptools.command import build_ext
 
 
-HERE = os.path.dirname(os.path.abspath(__file__))
+PYTHON_INCLUDE_PATH_PLACEHOLDER = "<PYTHON_INCLUDE_PATH>"
 
+IS_WINDOWS = platform.system() == "Windows"
+IS_MAC = platform.system() == "Darwin"
 
-IS_WINDOWS = sys.platform.startswith("win")
 
+def _get_long_description(fp: str) -> str:
+    with open(fp, "r", encoding="utf-8") as f:
+        return f.read()
 
-with open("README.md", "r", encoding="utf-8") as fp:
-    long_description = fp.read()
 
+def _get_version(fp: str) -> str:
+    """Parse a version string from a file."""
+    with open(fp, "r") as f:
+        for line in f:
+            if "__version__" in line:
+                delim = '"'
+                return line.split(delim)[1]
+    raise RuntimeError(f"could not find a version string in file {fp!r}.")
 
-def _get_version():
-    """Parse the version string from __init__.py."""
-    with open(
-        os.path.join(HERE, "bindings", "python", "google_benchmark", "__init__.py")
-    ) as init_file:
-        try:
-            version_line = next(
-                line for line in init_file if line.startswith("__version__")
-            )
-        except StopIteration:
-            raise ValueError("__version__ not defined in __init__.py")
-        else:
-            namespace = {}
-            exec(version_line, namespace)  # pylint: disable=exec-used
-            return namespace["__version__"]
 
-
-def _parse_requirements(path):
-    with open(os.path.join(HERE, path)) as requirements:
+def _parse_requirements(fp: str) -> List[str]:
+    with open(fp) as requirements:
         return [
             line.rstrip()
             for line in requirements
             if not (line.isspace() or line.startswith("#"))
         ]
 
 
+@contextlib.contextmanager
+def temp_fill_include_path(fp: str):
+    """Temporarily set the Python include path in a file."""
+    with open(fp, "r+") as f:
+        try:
+            content = f.read()
+            replaced = content.replace(
+                PYTHON_INCLUDE_PATH_PLACEHOLDER,
+                Path(sysconfig.get_paths()['include']).as_posix(),
+            )
+            f.seek(0)
+            f.write(replaced)
+            f.truncate()
+            yield
+        finally:
+            # revert to the original content after exit
+            f.seek(0)
+            f.write(content)
+            f.truncate()
+
+
 class BazelExtension(setuptools.Extension):
     """A C/C++ extension that is defined as a Bazel BUILD target."""
 
-    def __init__(self, name, bazel_target):
+    def __init__(self, name: str, bazel_target: str):
+        super().__init__(name=name, sources=[])
+
         self.bazel_target = bazel_target
-        self.relpath, self.target_name = posixpath.relpath(bazel_target, "//").split(
-            ":"
-        )
-        setuptools.Extension.__init__(self, name, sources=[])
+        stripped_target = bazel_target.split("//")[-1]
+        self.relpath, self.target_name = stripped_target.split(":")
 
 
 class BuildBazelExtension(build_ext.build_ext):
     """A command that runs Bazel to build a C/C++ extension."""
 
     def run(self):
         for ext in self.extensions:
             self.bazel_build(ext)
         build_ext.build_ext.run(self)
 
-    def bazel_build(self, ext):
+    def bazel_build(self, ext: BazelExtension):
         """Runs the bazel build to create the package."""
-        with open("WORKSPACE", "r") as workspace:
-            workspace_contents = workspace.read()
-
-        with open("WORKSPACE", "w") as workspace:
-            workspace.write(
-                re.sub(
-                    r'(?<=path = ").*(?=",  # May be overwritten by setup\.py\.)',
-                    sysconfig.get_python_inc().replace(os.path.sep, posixpath.sep),
-                    workspace_contents,
-                )
-            )
-
-        if not os.path.exists(self.build_temp):
-            os.makedirs(self.build_temp)
+        with temp_fill_include_path("WORKSPACE"):
+            temp_path = Path(self.build_temp)
 
-        bazel_argv = [
-            "bazel",
-            "build",
-            ext.bazel_target,
-            "--symlink_prefix=" + os.path.join(self.build_temp, "bazel-"),
-            "--compilation_mode=" + ("dbg" if self.debug else "opt"),
-        ]
+            bazel_argv = [
+                "bazel",
+                "build",
+                ext.bazel_target,
+                f"--symlink_prefix={temp_path / 'bazel-'}",
+                f"--compilation_mode={'dbg' if self.debug else 'opt'}",
+                # C++17 is required by nanobind
+                f"--cxxopt={'/std:c++17' if IS_WINDOWS else '-std=c++17'}",
+            ]
+
+            if IS_WINDOWS:
+                # Link with python*.lib.
+                for library_dir in self.library_dirs:
+                    bazel_argv.append("--linkopt=/LIBPATH:" + library_dir)
+            elif IS_MAC:
+                if platform.machine() == "x86_64":
+                    # C++17 needs macOS 10.14 at minimum
+                    bazel_argv.append("--macos_minimum_os=10.14")
+
+                    # cross-compilation for Mac ARM64 on GitHub Mac x86 runners.
+                    # ARCHFLAGS is set by cibuildwheel before macOS wheel builds.
+                    archflags = os.getenv("ARCHFLAGS", "")
+                    if "arm64" in archflags:
+                        bazel_argv.append("--cpu=darwin_arm64")
+                        bazel_argv.append("--macos_cpus=arm64")
+
+                elif platform.machine() == "arm64":
+                    bazel_argv.append("--macos_minimum_os=11.0")
+
+            self.spawn(bazel_argv)
+
+            shared_lib_suffix = '.dll' if IS_WINDOWS else '.so'
+            ext_name = ext.target_name + shared_lib_suffix
+            ext_bazel_bin_path = temp_path / 'bazel-bin' / ext.relpath / ext_name
 
-        if IS_WINDOWS:
-            # Link with python*.lib.
-            for library_dir in self.library_dirs:
-                bazel_argv.append("--linkopt=/LIBPATH:" + library_dir)
-        elif sys.platform == "darwin" and platform.machine() == "x86_64":
-            bazel_argv.append("--macos_minimum_os=10.9")
-
-            # ARCHFLAGS is always set by cibuildwheel before macOS wheel builds.
-            archflags = os.getenv("ARCHFLAGS", "")
-            if "arm64" in archflags:
-                bazel_argv.append("--cpu=darwin_arm64")
-                bazel_argv.append("--macos_cpus=arm64")
-
-        self.spawn(bazel_argv)
-
-        shared_lib_suffix = '.dll' if IS_WINDOWS else '.so'
-        ext_bazel_bin_path = os.path.join(
-            self.build_temp, 'bazel-bin',
-            ext.relpath, ext.target_name + shared_lib_suffix)
-
-        ext_dest_path = self.get_ext_fullpath(ext.name)
-        ext_dest_dir = os.path.dirname(ext_dest_path)
-        if not os.path.exists(ext_dest_dir):
-            os.makedirs(ext_dest_dir)
-        shutil.copyfile(ext_bazel_bin_path, ext_dest_path)
+            ext_dest_path = Path(self.get_ext_fullpath(ext.name))
+            shutil.copyfile(ext_bazel_bin_path, ext_dest_path)
 
-        # explicitly call `bazel shutdown` for graceful exit
-        self.spawn(["bazel", "shutdown"])
+            # explicitly call `bazel shutdown` for graceful exit
+            self.spawn(["bazel", "shutdown"])
 
 
 setuptools.setup(
     name="google_benchmark",
-    version=_get_version(),
+    version=_get_version("bindings/python/google_benchmark/__init__.py"),
     url="https://github.com/google/benchmark",
     description="A library to benchmark code snippets.",
-    long_description=long_description,
+    long_description=_get_long_description("README.md"),
     long_description_content_type="text/markdown",
     author="Google",
     author_email="benchmark-py@google.com",
     # Contained modules and scripts.
     package_dir={"": "bindings/python"},
     packages=setuptools.find_packages("bindings/python"),
     install_requires=_parse_requirements("bindings/python/requirements.txt"),
@@ -143,15 +150,14 @@
     zip_safe=False,
     # PyPI package information.
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "Intended Audience :: Science/Research",
         "License :: OSI Approved :: Apache Software License",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Topic :: Software Development :: Testing",
         "Topic :: System :: Benchmark",
     ],
```

