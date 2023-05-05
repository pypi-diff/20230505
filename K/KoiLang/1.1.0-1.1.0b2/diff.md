# Comparing `tmp/KoiLang-1.1.0.tar.gz` & `tmp/KoiLang-1.1.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "KoiLang-1.1.0.tar", last modified: Fri May  5 14:47:19 2023, max compression
+gzip compressed data, was "KoiLang-1.1.0b2.tar", last modified: Wed Apr  5 12:08:00 2023, max compression
```

## Comparing `KoiLang-1.1.0.tar` & `KoiLang-1.1.0b2.tar`

### file list

```diff
@@ -1,49 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:47:19.005287 KoiLang-1.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:47:19.001287 KoiLang-1.1.0/KoiLang.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14570 2023-05-05 14:47:18.000000 KoiLang-1.1.0/KoiLang.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-05-05 14:47:18.000000 KoiLang-1.1.0/KoiLang.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 14:47:18.000000 KoiLang-1.1.0/KoiLang.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-05 14:47:18.000000 KoiLang-1.1.0/KoiLang.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-05 14:47:18.000000 KoiLang-1.1.0/KoiLang.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-05 14:47:07.000000 KoiLang-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14570 2023-05-05 14:47:19.005287 KoiLang-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11027 2023-05-05 14:47:07.000000 KoiLang-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:47:19.005287 KoiLang-1.1.0/kola/
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-05-05 14:47:07.000000 KoiLang-1.1.0/kola/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-05-05 14:47:07.000000 KoiLang-1.1.0/kola/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6748 2023-05-05 14:47:07.000000 KoiLang-1.1.0/kola/_cutil.h
--rw-r--r--   0 runner    (1001) docker     (123)     3126 2023-05-05 14:47:07.000000 KoiLang-1.1.0/kola/_cutil.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-05-05 14:47:07.000000 KoiLang-1.1.0/kola/_yylex.pxd
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-05-05 14:47:07.000000 KoiLang-1.1.0/kola/exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:47:19.005287 KoiLang-1.1.0/kola/klvm/
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-05-05 14:47:07.000000 KoiLang-1.1.0/kola/klvm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-05-05 14:47:07.000000 KoiLang-1.1.0/kola/klvm/command.py
--rw-r--r--   0 runner    (1001) docker     (123)     4797 2023-05-05 14:47:07.000000 KoiLang-1.1.0/kola/klvm/commandset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-05-05 14:47:07.000000 KoiLang-1.1.0/kola/klvm/commandset.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-05-05 14:47:07.000000 KoiLang-1.1.0/kola/klvm/decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-05-05 14:47:07.000000 KoiLang-1.1.0/kola/klvm/decorator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8123 2023-05-05 14:47:07.000000 KoiLang-1.1.0/kola/klvm/environment.py
--rw-r--r--   0 runner    (1001) docker     (123)    11633 2023-05-05 14:47:07.000000 KoiLang-1.1.0/kola/klvm/koilang.py
--rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-05-05 14:47:07.000000 KoiLang-1.1.0/kola/klvm/writer.py
--rw-r--r--   0 runner    (1001) docker     (123)   680498 2023-05-05 14:47:07.000000 KoiLang-1.1.0/kola/lexer.c
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-05-05 14:47:07.000000 KoiLang-1.1.0/kola/lexer.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     2931 2023-05-05 14:47:07.000000 KoiLang-1.1.0/kola/lexer.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:47:19.005287 KoiLang-1.1.0/kola/lib/
--rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-05-05 14:47:07.000000 KoiLang-1.1.0/kola/lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:47:19.005287 KoiLang-1.1.0/kola/lib/debugger/
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-05-05 14:47:07.000000 KoiLang-1.1.0/kola/lib/debugger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-05-05 14:47:07.000000 KoiLang-1.1.0/kola/lib/debugger/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-05-05 14:47:07.000000 KoiLang-1.1.0/kola/lib/debugger/command_debugger.py
--rw-r--r--   0 runner    (1001) docker     (123)     6188 2023-05-05 14:47:07.000000 KoiLang-1.1.0/kola/lib/debugger/default_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-05-05 14:47:07.000000 KoiLang-1.1.0/kola/lib/fast_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-05-05 14:47:07.000000 KoiLang-1.1.0/kola/lib/recorder.py
--rw-r--r--   0 runner    (1001) docker     (123)   577664 2023-05-05 14:47:07.000000 KoiLang-1.1.0/kola/parser.c
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-05-05 14:47:07.000000 KoiLang-1.1.0/kola/parser.pxd
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-05 14:47:07.000000 KoiLang-1.1.0/kola/parser.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-05-05 14:47:07.000000 KoiLang-1.1.0/kola/unicode_handler.c
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-05 14:47:07.000000 KoiLang-1.1.0/kola/version.py
--rw-r--r--   0 runner    (1001) docker     (123)  1137811 2023-05-05 14:47:07.000000 KoiLang-1.1.0/kola/writer.c
--rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-05-05 14:47:07.000000 KoiLang-1.1.0/kola/writer.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-05-05 14:47:07.000000 KoiLang-1.1.0/kola/writer.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 14:47:19.005287 KoiLang-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-05-05 14:47:07.000000 KoiLang-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 12:08:00.664754 KoiLang-1.1.0b2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 12:08:00.652753 KoiLang-1.1.0b2/KoiLang.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14572 2023-04-05 12:08:00.000000 KoiLang-1.1.0b2/KoiLang.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-04-05 12:08:00.000000 KoiLang-1.1.0b2/KoiLang.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 12:08:00.000000 KoiLang-1.1.0b2/KoiLang.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-05 12:08:00.000000 KoiLang-1.1.0b2/KoiLang.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-05 12:08:00.000000 KoiLang-1.1.0b2/KoiLang.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-05 12:07:46.000000 KoiLang-1.1.0b2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14572 2023-04-05 12:08:00.664754 KoiLang-1.1.0b2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11027 2023-04-05 12:07:46.000000 KoiLang-1.1.0b2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 12:08:00.660754 KoiLang-1.1.0b2/kola/
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-04-05 12:07:46.000000 KoiLang-1.1.0b2/kola/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-04-05 12:07:46.000000 KoiLang-1.1.0b2/kola/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6663 2023-04-05 12:07:46.000000 KoiLang-1.1.0b2/kola/_cutil.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3126 2023-04-05 12:07:46.000000 KoiLang-1.1.0b2/kola/_cutil.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-04-05 12:07:46.000000 KoiLang-1.1.0b2/kola/_yylex.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-04-05 12:07:46.000000 KoiLang-1.1.0b2/kola/exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 12:08:00.660754 KoiLang-1.1.0b2/kola/klvm/
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-04-05 12:07:46.000000 KoiLang-1.1.0b2/kola/klvm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-04-05 12:07:46.000000 KoiLang-1.1.0b2/kola/klvm/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-04-05 12:07:46.000000 KoiLang-1.1.0b2/kola/klvm/commandset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-04-05 12:07:46.000000 KoiLang-1.1.0b2/kola/klvm/commandset.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-04-05 12:07:46.000000 KoiLang-1.1.0b2/kola/klvm/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2952 2023-04-05 12:07:46.000000 KoiLang-1.1.0b2/kola/klvm/decorator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7256 2023-04-05 12:07:46.000000 KoiLang-1.1.0b2/kola/klvm/environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11395 2023-04-05 12:07:46.000000 KoiLang-1.1.0b2/kola/klvm/koilang.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3234 2023-04-05 12:07:46.000000 KoiLang-1.1.0b2/kola/klvm/writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)   676158 2023-04-05 12:07:46.000000 KoiLang-1.1.0b2/kola/lexer.c
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-04-05 12:07:46.000000 KoiLang-1.1.0b2/kola/lexer.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-04-05 12:07:46.000000 KoiLang-1.1.0b2/kola/lexer.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 12:08:00.664754 KoiLang-1.1.0b2/kola/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-04-05 12:07:46.000000 KoiLang-1.1.0b2/kola/lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 12:08:00.664754 KoiLang-1.1.0b2/kola/lib/debugger/
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-04-05 12:07:46.000000 KoiLang-1.1.0b2/kola/lib/debugger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-04-05 12:07:46.000000 KoiLang-1.1.0b2/kola/lib/debugger/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-04-05 12:07:46.000000 KoiLang-1.1.0b2/kola/lib/debugger/command_debugger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6180 2023-04-05 12:07:46.000000 KoiLang-1.1.0b2/kola/lib/debugger/default_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-04-05 12:07:46.000000 KoiLang-1.1.0b2/kola/lib/fast_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)   577659 2023-04-05 12:07:46.000000 KoiLang-1.1.0b2/kola/parser.c
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-04-05 12:07:46.000000 KoiLang-1.1.0b2/kola/parser.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-04-05 12:07:46.000000 KoiLang-1.1.0b2/kola/parser.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-04-05 12:07:46.000000 KoiLang-1.1.0b2/kola/unicode_handler.c
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-05 12:07:46.000000 KoiLang-1.1.0b2/kola/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1137811 2023-04-05 12:07:46.000000 KoiLang-1.1.0b2/kola/writer.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-04-05 12:07:46.000000 KoiLang-1.1.0b2/kola/writer.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-04-05 12:07:46.000000 KoiLang-1.1.0b2/kola/writer.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-05 12:08:00.664754 KoiLang-1.1.0b2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-04-05 12:07:46.000000 KoiLang-1.1.0b2/setup.py
```

### Comparing `KoiLang-1.1.0/KoiLang.egg-info/PKG-INFO` & `KoiLang-1.1.0b2/KoiLang.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KoiLang
-Version: 1.1.0
+Version: 1.1.0b2
 Summary: simple python module for KoiLang parsing
 Home-page: https://github.com/Ovizro/Kola
 Author: Ovizro
 Author-email: Ovizro@hypercol.com
 Maintainer: Ovizro
 Maintainer-email: Ovizro@hypercol.com
 License: Apache 2.0
```

### Comparing `KoiLang-1.1.0/KoiLang.egg-info/SOURCES.txt` & `KoiLang-1.1.0b2/KoiLang.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -30,12 +30,11 @@
 kola/klvm/decorator.py
 kola/klvm/decorator.pyi
 kola/klvm/environment.py
 kola/klvm/koilang.py
 kola/klvm/writer.py
 kola/lib/__init__.py
 kola/lib/fast_file.py
-kola/lib/recorder.py
 kola/lib/debugger/__init__.py
 kola/lib/debugger/base.py
 kola/lib/debugger/command_debugger.py
 kola/lib/debugger/default_runner.py
```

### Comparing `KoiLang-1.1.0/LICENSE` & `KoiLang-1.1.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `KoiLang-1.1.0/PKG-INFO` & `KoiLang-1.1.0b2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: KoiLang
-Version: 1.1.0
+Version: 1.1.0b2
 Summary: simple python module for KoiLang parsing
 Home-page: https://github.com/Ovizro/Kola
 Author: Ovizro
 Author-email: Ovizro@hypercol.com
 Maintainer: Ovizro
 Maintainer-email: Ovizro@hypercol.com
 License: Apache 2.0
```

### Comparing `KoiLang-1.1.0/README.md` & `KoiLang-1.1.0b2/README.md`

 * *Files identical despite different names*

### Comparing `KoiLang-1.1.0/kola/__init__.py` & `KoiLang-1.1.0b2/kola/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,7 @@
-"""
-simple python module for KoiLang parsing
-"""
-
 from .lexer import BaseLexer, FileLexer, StringLexer
 from .parser import Parser
 from .writer import BaseWriter, FileWriter, StringWriter, BaseWriterItem, FormatItem, ComplexArg, WriterItemLike
 from .klvm import KoiLang, Environment, kola_command, kola_text, kola_number, kola_annotation, kola_env_enter, kola_env_exit, kola_env_class
 from .version import __version__, version_info
 from .exception import KoiLangError, KoiLangSyntaxError, KoiLangCommandError
```

### Comparing `KoiLang-1.1.0/kola/__main__.py` & `KoiLang-1.1.0b2/kola/__main__.py`

 * *Files identical despite different names*

### Comparing `KoiLang-1.1.0/kola/_cutil.h` & `KoiLang-1.1.0b2/kola/_cutil.h`

 * *Files 2% similar despite different names*

```diff
@@ -216,21 +216,18 @@
     name = PyBytes_AS_STRING(stringobj);
 
     Py_BEGIN_ALLOW_THREADS
     fp = fopen(name, mode);
     Py_END_ALLOW_THREADS
 #endif
     if (fp == NULL) {
-        PyErr_SetFromErrno(PyExc_OSError);
-        // PyErr_Format(PyExc_OSError, "fail to open '%S'", raw_path);
+        PyErr_Format(PyExc_OSError, "fail to open '%S'", raw_path);
     }
     if (out)
         *out = stringobj;
-    else
-        Py_DECREF(stringobj);
     return fp;
 }
 
 static __inline const char* unicode2string(PyObject* __s, Py_ssize_t* s_len) {
     Py_ssize_t _s_len;
     const char* s = PyUnicode_AsUTF8AndSize(__s, &_s_len);
     if (s == NULL)
```

### Comparing `KoiLang-1.1.0/kola/_cutil.pxd` & `KoiLang-1.1.0b2/kola/_cutil.pxd`

 * *Files identical despite different names*

### Comparing `KoiLang-1.1.0/kola/_yylex.pxd` & `KoiLang-1.1.0b2/kola/_yylex.pxd`

 * *Files identical despite different names*

### Comparing `KoiLang-1.1.0/kola/klvm/__init__.py` & `KoiLang-1.1.0b2/kola/klvm/__init__.py`

 * *Files identical despite different names*

### Comparing `KoiLang-1.1.0/kola/klvm/command.py` & `KoiLang-1.1.0b2/kola/klvm/command.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from functools import partialmethod
 from types import MethodType
 from typing import Any, Callable, Dict, Generator, Iterable, Tuple, Union, overload
 from typing_extensions import Self, Protocol, runtime_checkable
 
 
 class CommandCaller(Protocol):
     def __call__(self, __command: Any, __args: tuple, __kwargs: Dict[str, Any], **kwds: Any) -> Any: ...
@@ -10,31 +9,29 @@
 
 @runtime_checkable
 class CommandLike(Protocol):
     def __kola_command__(self) -> Generator[Tuple[str, Callable], None, None]: ...
 
 
 class Command(object):
-    __slots__ = ["__name__", "__func__", "suppression", "virtual", "alias", "extra_data"]
+    __slots__ = ["__name__", "__func__", "suppression", "alias", "extra_data"]
 
     def __init__(
         self,
         __name: str,
         func: Callable,
         *,
         alias: Union[Iterable[str], str] = tuple(),
         suppression: bool = False,
-        virtual: bool = False,
         **kwds: Any
     ) -> None:
         self.__name__ = __name
         self.__func__ = func
         self.alias = (alias,) if isinstance(alias, str) else tuple(alias)
         self.suppression = suppression
-        self.virtual = virtual
         self.extra_data = kwds
     
     @overload
     def set_data(self, __name: str, value: Any) -> Self: ...
     @overload
     def set_data(self, __name: str) -> Callable[[Any], Self]: ...
 
@@ -44,46 +41,46 @@
             return self
         
         def wrapper(val: Any) -> Self:
             self.extra_data[__name] = val
             return self
         return wrapper
 
-    writer = partialmethod(set_data, "writer_func")
+    def writer(self, func: Callable) -> Self:
+        self.extra_data["writer_func"] = func
+        return self
     
     @classmethod
     def from_command(cls, command: "Command", **kwds: Any) -> Self:
         data = command.extra_data.copy()
         data.update(kwds)
         return cls(
             command.__name__,
             command.__func__,
             alias=command.alias,
             **data
         )
     
     @property
-    def __wrapped__(self) -> Callable:  # pragma: no cover
+    def __wrapped__(self) -> Callable:
         return self.__func__
     
     def __kola_command__(self, force: bool = False) -> Generator[Tuple[str, Self], None, None]:
         if not self.suppression or force:
             bound_func = self
             yield self.__name__, bound_func
             for i in self.alias:
                 yield i, bound_func
 
     def __get__(self, ins: Any, owner: type) -> Any:
         if ins is None:
             return self
-        elif self.virtual and (not hasattr(owner, "check_virtual") or ins.check_virtual(self)):
-            return ins[self.__name__]
         return MethodType(self, ins)
 
     def __call__(self, vmobj: Any, *args: Any, **kwds: Any) -> Any:
         caller = getattr(vmobj, "__kola_caller__", None)
-        if caller is None:  # pragma: no cover
+        if caller is None:
             return self.__func__(vmobj, *args, **kwds)
         return caller(self, args, kwds, **self.extra_data)
 
     def __repr__(self) -> str:
         return f"<kola command {self.__name__} with {self.__func__}>"
```

### Comparing `KoiLang-1.1.0/kola/klvm/commandset.py` & `KoiLang-1.1.0b2/kola/klvm/commandset.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,33 +7,20 @@
 
 
 class CommandSetMeta(ABCMeta):
     """
     metaclass for all command sets
     """
     __command_field__: Set[CommandLike]
-    __virtual_table__: Dict[str, str]
 
-    def __new__(cls, name: str, bases: Tuple[Type, ...], attr: Dict[str, Any], **kwds: Any) -> Self:
-        command_field = set()
-        virtual_table = attr.get("__virtual_table__", {})
-        for i in bases:
-            if isinstance(i, CommandSetMeta):
-                virtual_table.update(i.__virtual_table__)
-        for k, v in attr.items():
-            if isinstance(v, Command):
-                if v.virtual:
-                    virtual_table[k] = v.__name__
-            elif k in virtual_table:
-                v = Command(virtual_table[k], v, virtual=True)
-            elif not isinstance(v, CommandLike):
-                continue
-            command_field.add(v)
+    def __new__(cls, name: str, bases: Tuple[type, ...], attr: Dict[str, Any], **kwds: Any) -> Self:
+        command_field = {
+            i for i in attr.values() if isinstance(i, (Command, CommandLike))
+        }
         attr["__command_field__"] = command_field
-        attr["__virtual_table__"] = virtual_table
         return super().__new__(cls, name, bases, attr, **kwds)
 
     def generate_raw_commands(self) -> Dict[str, Any]:
         cmd_set = {}
         for cls in reversed(self.__mro__):
             cls: Type
             if not isinstance(cls, CommandSetMeta):
@@ -99,17 +86,14 @@
             return raw_cmd
         
         assert raw_cmd
         bound_cmd = MethodType(raw_cmd, self)
         self._bound_command_cache[__key] = bound_cmd
         return bound_cmd
 
-    def check_virtual(self, command: Command) -> bool:
-        return command is self.raw_command_set[command.__name__]
-
     def __kola_caller__(self, command: Command, args: tuple, kwargs: Dict[str, Any], **kwds: Any) -> Any:
         """hook function used to change the calling behavior of the `Command` class
 
         :param command: the `Command` object being invoked
         :type command: Command
         :param args: call positional arguments
         :type args: Tuple[Any]
```

### Comparing `KoiLang-1.1.0/kola/klvm/commandset.pyi` & `KoiLang-1.1.0b2/kola/klvm/commandset.pyi`

 * *Files 11% similar despite different names*

```diff
@@ -5,45 +5,44 @@
 from typing_extensions import Self
 
 from .command import Command, CommandLike
 
 
 class CommandSetMeta(ABCMeta):
     __command_field__: Set[CommandLike]
-    __virtual_table__: Dict[str, str]
 
     def __new__(cls, name: str, bases: Tuple[type, ...], attr: Dict[str, Any], **kwds: Any) -> Self: ...
     def generate_raw_commands(self) -> Dict[str, Any]: ...
     @overload
     def register_command(
         self, __func: Callable[..., Any], **kwds) -> Command: ...
     @overload
     def register_command(
-        self, __name: Optional[str] = ..., *, alias: Union[Iterable[str], str] = ..., virtual: bool = False, **kwds: Any
+        self, __name: Optional[str] = ..., *, alias: Union[Iterable[str], str] = ..., **kwds: Any
     ) -> Callable[[Callable[..., Any]], Command]: ...
     @overload
     def register_text(
         self, __func: Callable[..., Any], **kwds) -> Command: ...
     @overload
     def register_text(
-        self, *, alias: Union[Iterable[str], str] = ..., virtual: bool = False, **kwds: Any
+        self, *, alias: Union[Iterable[str], str] = ..., **kwds: Any
     ) -> Callable[[Callable[..., Any]], Command]: ...
     @overload
     def register_number(
         self, __func: Callable[..., Any], **kwds) -> Command: ...
     @overload
     def register_number(
-        self, *, alias: Union[Iterable[str], str] = ..., virtual: bool = False, **kwds: Any
+        self, *, alias: Union[Iterable[str], str] = ..., **kwds: Any
     ) -> Callable[[Callable[..., Any]], Command]: ...
     @overload
     def register_annotation(
         self, __func: Callable[..., Any], **kwds) -> Command: ...
     @overload
     def register_annotation(
-        self, *, alias: Union[Iterable[str], str] = ..., virtual: bool = False, **kwds: Any
+        self, *, alias: Union[Iterable[str], str] = ..., **kwds: Any
     ) -> Callable[[Callable[..., Any]], Command]: ...
     
 
 class CommandSet(metaclass=CommandSetMeta):
     raw_command_set: Dict[str, Callable]
     _bound_command_set: Dict[str, Callable]
```

### Comparing `KoiLang-1.1.0/kola/klvm/decorator.py` & `KoiLang-1.1.0b2/kola/klvm/decorator.py`

 * *Files identical despite different names*

### Comparing `KoiLang-1.1.0/kola/klvm/decorator.pyi` & `KoiLang-1.1.0b2/kola/klvm/decorator.pyi`

 * *Files 17% similar despite different names*

```diff
@@ -1,76 +1,76 @@
 from typing import Any, Callable, Iterable, Optional, Type, overload, Union
+from typing_extensions import Literal
 
-from .command import Command
-from .commandset import CommandSet
+from .commandset import Command, CommandSet
 from .environment import Environment, EnvironmentEntry, EnvironmentExit
 from .koilang import KoiLang
 
 
 @overload
 def kola_command(func: Callable[..., Any], **kwds: Any) -> Command: ...
 @overload
 def kola_command(
     func: Optional[str] = None,
     *,
+    method: Literal["static", "class", "default"] = ...,
     envs: Union[Iterable[str], str] = ...,
     alias: Union[Iterable[str], str] = ...,
-    virtual: bool = False,
     **kwds: Any
 ) -> Callable[[Callable[..., Any]], Command]: ...
 @overload
 def kola_text(func: Callable[..., Any], **kwds: Any) -> Command: ...
 @overload
 def kola_text(
     *,
+    method: Literal["static", "class", "default"] = ...,
     envs: Union[Iterable[str], str] = ...,
     alias: Union[Iterable[str], str] = ...,
-    virtual: bool = False,
     **kwds: Any
 ) -> Callable[[Callable[..., Any]], Command]: ...
 @overload
 def kola_number(func: Callable[..., Any], **kwds: Any) -> Command: ...
 @overload
 def kola_number(
     *,
+    method: Literal["static", "class", "default"] = ...,
     envs: Union[Iterable[str], str] = ...,
     alias: Union[Iterable[str], str] = ...,
-    virtual: bool = False,
     **kwds: Any
 ) -> Callable[[Callable[..., Any]], Command]: ...
 @overload
 def kola_annotation(func: Callable[..., Any], **kwds: Any) -> Command: ...
 @overload
 def kola_annotation(
     *,
+    method: Literal["static", "class", "default"] = ...,
     envs: Union[Iterable[str], str] = ...,
     alias: Union[Iterable[str], str] = ...,
-    virtual: bool = False,
     **kwds: Any
 ) -> Callable[[Callable[..., Any]], Command]: ...
 @overload
 def kola_env_enter(func: Callable[..., Any], **kwds: Any) -> EnvironmentEntry: ...
 @overload
 def kola_env_enter(
     func: Optional[str] = None,
     *,
+    method: Literal["static", "class", "default"] = ...,
     envs: Union[Iterable[str], str] = ...,
     alias: Union[Iterable[str], str] = ...,
-    virtual: bool = False,
     **kwds: Any
 ) -> Callable[[Callable[..., Any]], EnvironmentEntry]: ...
 @overload
 def kola_env_exit(func: Callable[..., Any], **kwds: Any) -> EnvironmentExit: ...
 @overload
 def kola_env_exit(
     func: Optional[str] = None,
     *,
+    method: Literal["static", "class", "default"] = ...,
     envs: Union[Iterable[str], str] = ...,
     alias: Union[Iterable[str], str] = ...,
-    virtual: bool = False,
     **kwds: Any
 ) -> Callable[[Callable[..., Any]], EnvironmentExit]: ...
 @overload
 def kola_command_set(kola_cls: Type, **kwds: Any) -> Type[CommandSet]: ...
 @overload
 def kola_command_set(kola_cls: Optional[str] = None, **kwds: Any) -> Callable[[Type], Type[CommandSet]]: ...
 @overload
```

### Comparing `KoiLang-1.1.0/kola/klvm/environment.py` & `KoiLang-1.1.0b2/kola/klvm/environment.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,10 @@
-from functools import partial
-from types import TracebackType
 from typing import Any, Callable, Dict, Generator, Iterable, Optional, Set, Tuple, Type, TypeVar, Union, overload
 from typing_extensions import Self
 
-from ..exception import KoiLangError
-
 from .command import Command
 from .commandset import CommandSet, CommandSetMeta
 
 
 T = TypeVar("T")
 
 
@@ -46,55 +42,56 @@
         if isinstance(ins, self.env_class) and self.env_class.__env_autopop__:
             return EnvironmentAutopop.from_command(self).__get__(ins, owner)
         return super().__get__(ins, owner)
 
     def __call__(self, vmobj: Union["Environment", "KoiLang"], *args: Any, **kwds: Any) -> Any:
         assert self.env_class
         home = vmobj.home
-        env = home.push_prepare(self.env_class)
+        env = home.push_start(self.env_class)
         ret = super().__call__(env, *args, **kwds)
-        home.push_apply(env)
+        home.push_end(env)
         return ret
 
 
 class EnvironmentExit(EnvironmentCommand):
     __slots__ = []
 
-    def __call__(self, vmobj: "Environment", *args: Any, **kwds: Any) -> Any:
+    def __call__(self, vmobj: Union["Environment", "KoiLang"], *args: Any, **kwds: Any) -> Any:
         home = vmobj.home
-        pop_env = home.pop_prepare(self.env_class)
+        pop_env = home.pop_start(self.env_class)
         ret = super().__call__(vmobj, *args, **kwds)
-        home.pop_apply(pop_env)
+        home.pop_end(pop_env)
         return ret
 
 
 class EnvironmentAutopop(EnvironmentCommand):
     __slots__ = []
 
-    def __call__(self, vmobj: "Environment", *args: Any, **kwds: Any) -> Any:
+    def __call__(self, vmobj: Union["Environment", "KoiLang"], *args: Any, **kwds: Any) -> Any:
         assert self.env_class
         home = vmobj.home
 
-        vmobj.on_autopop()
-        cache = home.push_prepare(self.env_class)
+        cache = home.pop_start(self.env_class)
+        home.pop_end(cache)
+        cache = home.push_start(self.env_class)
         ret = super().__call__(cache, *args, **kwds)
-        home.push_apply(cache)
+        home.push_end(cache)
         return ret
 
 
 class EnvironmentMeta(CommandSetMeta):
     __env_entry__: Set[EnvironmentCommand]
     __env_exit__: Set[EnvironmentCommand]
 
     def __new__(cls, name: str, bases: Tuple[type, ...], attr: Dict[str, Any], **kwds: Any) -> Self:
         entry = set()
         exit = set()
         
-        # Usually, there are not many entry points and exit points.
-        # Therefore, unlike the attribute `__command_fields__`, they are computed here
+        # usually, there are not many entry points and exit points.
+        # so, no like attr `__command_field__`, I calculate these here.
         for i in bases:
             if not isinstance(i, EnvironmentMeta):
                 continue
             entry.update(i.__env_entry__)
             exit.update(i.__env_exit__)
 
         attr["__env_entry__"] = entry
@@ -140,30 +137,30 @@
                 # raise ValueError(f"cannot find env '{self.__name__}' in the {home}")
         return self
     
     class EntryPointInterface:
         """
         interface for entry points in Python level
         """
-        __slots__ = ["__env_class", "__bound_ins"]
+        __slots__ = ["env_class", "bound_ins"]
 
         def __init__(self, env_class: "EnvironmentMeta", bound_ins: CommandSet) -> None:
-            self.__env_class = env_class
-            self.__bound_ins = bound_ins
+            self.env_class = env_class
+            self.bound_ins = bound_ins
         
         def __getattr__(self, __name: str) -> Any:
-            attr = getattr(self.__env_class, __name)
+            attr = getattr(self.env_class, __name)
             if isinstance(attr, EnvironmentEntry):
-                return attr.__get__(self.__bound_ins, self.__bound_ins.__class__)
+                return attr.__get__(self.bound_ins, self.bound_ins.__class__)
             elif isinstance(attr, Command):
                 raise AttributeError(f"cannot fetch command '{__name}' before the environment initialization")
             raise AttributeError("only entry commands can be accessed through the interface")
         
-        def __repr__(self) -> str:  # pragma: no cover
-            return f"<kola environment '{self.__env_class.__name__}' entry point command interface>"
+        def __repr__(self) -> str:
+            return f"<kola environment '{self.env_class.__name__}' entry point command interface>"
 
 
 class Environment(CommandSet, metaclass=EnvironmentMeta):
     __slots__ = ["back"]
 
     def __init__(self, back: CommandSet) -> None:
         if not self.__class__.__env_entry__:
@@ -197,34 +194,15 @@
     def home(self) -> "KoiLang":
         cmd_set = self
         while isinstance(cmd_set, Environment):
             cmd_set = cmd_set.back
         assert isinstance(cmd_set, KoiLang)
         return cmd_set
     
-    def set_up(self, cur_top: CommandSet) -> None:
-        """called before the environment added to the env stack top"""
-
-    def tear_down(self, cur_top: CommandSet) -> None:
-        """called after the environment removed from the env stack top"""
-
-    def on_autopop(self) -> None:
-        home = self.home
-        home.pop_apply(home.pop_prepare(self.__class__))
-
-    @partial(Command, "@end")
-    def at_end(self) -> None:
-        """
-        ensure autopop environments properly popped at the end of parsing
-        """
-        if not self.__class__.__env_autopop__:
-            return
-        home = self.home
-        home.pop_apply(home.pop_prepare(self.__class__))
-        home.at_end()
-    
-    @partial(Command, "@exception", virtual=True, suppression=True)
-    def on_exception(self, exc_type: Type[KoiLangError], exc_ins: Optional[KoiLangError], traceback: TracebackType) -> Any:
-        return self.back["@exception"]
+    def at_initialize(self, cur_top: CommandSet) -> None:
+        pass
 
+    def at_finalize(self, cur_top: CommandSet) -> None:
+        pass
+    
 
 from .koilang import KoiLang
```

### Comparing `KoiLang-1.1.0/kola/klvm/koilang.py` & `KoiLang-1.1.0b2/kola/klvm/koilang.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,13 @@
-from functools import partial
+from contextlib import contextmanager
 import os
 import sys
 from threading import Lock
 from types import TracebackType, new_class
-from contextlib import contextmanager, suppress
-from typing import Any, Callable, Dict, Generator, List, Optional, Tuple, Type, TypeVar, Union, overload
+from typing import Any, Callable, ClassVar, Dict, Generator, Optional, Tuple, Type, TypeVar, Union, overload
 from typing_extensions import Literal, Self
 
 from ..lexer import BaseLexer, FileLexer, StringLexer
 from ..parser import Parser
 from ..exception import KoiLangError
 from .command import Command
 from .commandset import CommandSetMeta, CommandSet
@@ -21,78 +20,63 @@
 class KoiLangMeta(CommandSetMeta):
     """
     metaclass for KoiLang class
 
     Provide encoding and command threshold support.
     """
     __text_encoding__: str
-    __text_lstrip__: bool
     __command_threshold__: int
 
-    def __new__(
-        cls,
-        name: str,
-        bases: Tuple[type, ...],
-        attr: Dict[str, Any],
-        command_threshold: int = 0,
-        encoding: Optional[str] = None,
-        lstrip_text: Optional[bool] = None,
-        **kwds: Any
-    ) -> Self:
+    builtin_mapping: ClassVar[Dict[str, str]] = {
+        "at_start": "@start", "at_end": "@end", "on_exception": "@exception"
+    }
+
+    def __new__(cls, name: str, bases: Tuple[type, ...], attr: Dict[str, Any],
+                command_threshold: int = 0, encoding: Optional[str] = None, **kwds: Any):
         """
         create a top-level language class
 
         :param name: class name
         :type name: str
         :param bases: class bases
         :type bases: Tuple[type, ...]
         :param attr: class namespace
         :type attr: Dict[str, Any]
         :param command_threshold: the `#` prefix length of commands, defaults to 0
         :type command_threshold: int, optional
         :param encoding: encoding for file parsing, defaults to None
         :type encoding: Optional[str], optional
-        :param lstrip_text: whether to remove text indentation, defaults to True
-        :type lstrip_text: bool, optional
         :return: new class
         :rtype: KoiLangMeta
         """
-        # if not base KoiLang class, set a default value
-        if not any(isinstance(i, cls) for i in bases):
-            command_threshold = command_threshold or 1
-            encoding = encoding or "utf-8"
-            lstrip_text = lstrip_text if lstrip_text is not None else True
-        
-        if command_threshold:
+        has_base = any(isinstance(i, cls) for i in bases)
+        if command_threshold or not has_base:
             assert command_threshold >= 0
-            attr["__command_threshold__"] = command_threshold
-        if lstrip_text is not None:
-            attr["__text_lstrip__"] = lstrip_text
-        if encoding:
-            attr["__text_encoding__"] = encoding
+            attr["__command_threshold__"] = command_threshold or 1
+        if encoding or not has_base:
+            attr["__text_encoding__"] = encoding or "utf-8"
+        for k, n in cls.builtin_mapping.items():
+            if k not in attr:
+                continue
+            cmd = attr[k]
+            if not isinstance(cmd, Command):
+                attr[k] = Command(n, cmd)
         return super().__new__(cls, name, bases, attr, **kwds)
 
     def register_environment(self, env_class: _T_EnvCls) -> _T_EnvCls:
         self.__command_field__.add(env_class)
         return env_class
     
     @property
     def writer(self) -> Type:
-        """writer class for KoiLang file building
-
-        :return: the writer class, which is a subclass of KoiLangWriter and current KoiLang class
-        :rtype: Type[KoiLang, Self]
-        """
-        cache = None
-        with suppress(AttributeError):
-            cache = self.__writer_class
+        cache = getattr(self, "__writer_class__", None)
         if cache is not None:
             return cache
         cache = new_class(f"{self.__qualname__}.writer", (KoiLangWriter, self))
-        self.__writer_class = cache
+        self.__writer_class__ = cache
         return cache
 
 
 class KoiLang(CommandSet, metaclass=KoiLangMeta):
     """
     main class for KoiLang virtual machine
 
@@ -103,46 +87,46 @@
 
     def __init__(self) -> None:
         super().__init__()
         self._lock = Lock()
         self.__top = self
         self.__exec_level = 0
     
-    def push_prepare(self, __env_type: Type[Environment]) -> Environment:
+    def push_start(self, __env_type: Type[Environment]) -> Environment:
         env = __env_type(self.__top)
-        env.set_up(self.__top)
+        env.at_initialize(self.__top)
         return env
 
-    def push_apply(self, __env_cache: Environment) -> None:
+    def push_end(self, __env_cache: Environment) -> None:
         assert __env_cache.back is self.__top
         with self._lock:
             self.__top = __env_cache
     
-    def pop_prepare(self, __env_type: Optional[Type[Environment]] = None) -> Environment:
+    def pop_start(self, __env_type: Optional[Type[Environment]] = None) -> Environment:
         top = self.__top
-        if top is self:  # pragma: no cover
+        if top is self:
             raise ValueError('cannot pop the inital environment')
         if __env_type is None:
             assert isinstance(top, Environment)
         else:
             while isinstance(top, Environment) and top.__class__.__env_autopop__:
                 if isinstance(top, __env_type):
                     break
                 top = top.back
             else:
-                if not isinstance(top, __env_type):  # pragma: no cover
+                if not isinstance(top, __env_type):
                     raise ValueError("unmatched environment")
         return top
 
-    def pop_apply(self, __env_cache: Environment) -> None:
+    def pop_end(self, __env_cache: Environment) -> None:
         with self._lock:
             top = self.__top
             self.__top = __env_cache.back
         while isinstance(top, Environment):
-            top.tear_down(self.__top)
+            top.at_finalize(self.__top)
             if top is __env_cache:
                 break
             top = top.back
         else:
             raise ValueError('cannot pop the inital environment')
     
     def ensure_env(self, names: Tuple[str, ...]) -> None:
@@ -166,18 +150,18 @@
         else:
             # the base KoiLang object name is '__init__'
             reachable.append("__init__")
 
         if ((not ng or all(not self._ensure_env(reachable, i) for i in ng)) and
                 (not pt or any(self._ensure_env(reachable, i) for i in pt))):
             return
-        raise ValueError(f"unmatched environment name {reachable[0]}")  # pragma: no cover
+        raise ValueError(f"unmatched environment name {reachable[0]}")
     
     @staticmethod
-    def _ensure_env(reachable: List[str], name: str) -> bool:
+    def _ensure_env(reachable: list, name: str) -> bool:
         if name.startswith('+'):
             strict = True
             name = name[1:]
         else:
             strict = False
         if name.startswith('!'):
             inverse = True
@@ -187,24 +171,50 @@
 
         if strict:
             is_in = reachable[0] == name
         else:
             is_in = name in reachable
         return not is_in if inverse else is_in
 
+        # for n in names:
+        #     if n.startswith('+!'):
+        #         while n[2:] in reachable:
+        #             if len(reachable) < 2:
+        #                 break
+        #             cache = self.pop_start()
+        #             self.pop_end(cache)
+        #             reachable.popleft()
+        #         else:
+        #             continue
+        #     elif n.startswith('!'):
+        #         if any(i != n[1:] for i in reachable):
+        #             continue
+        #     elif n.startswith('+'):
+        #         while reachable[0] != n[1:]:
+        #             if len(reachable) < 2:
+        #                 break
+        #             cache = self.pop_start()
+        #             self.pop_end(cache)
+        #             reachable.popleft()
+        #         else:
+        #             continue
+        #     elif n in reachable:
+        #         continue
+        #     raise ValueError(f"unmatched environment name {n}")
+    
     def __parse(self, __lexer: BaseLexer, *, close_lexer: bool = True) -> None:
         parser = Parser(__lexer, self)
         try:
             with self.exec_block():
                 while True:
                     try:
                         # Parser.exec() is a fast C level loop
                         parser.exec()
                     except KoiLangError:
-                        if not self.on_exception(*sys.exc_info()):
+                        if not self["@exception"](*sys.exc_info()):
                             raise
                     else:
                         break
         finally:
             if close_lexer:
                 __lexer.close()
     
@@ -212,15 +222,15 @@
         parser = Parser(__lexer, self)
         try:
             with self.exec_block():
                 while True:
                     try:
                         yield from parser
                     except KoiLangError:
-                        if not self.on_exception(*sys.exc_info()):
+                        if not self["@exception"](*sys.exc_info()):
 
                             raise
                     else:
                         break
         finally:
             if close_lexer:
                 __lexer.close()
@@ -233,112 +243,99 @@
         lexer: Union[BaseLexer, str],
         *,
         with_ret: Literal[True],
         close_lexer: bool = True
     ) -> Generator[Any, None, None]: ...
     
     def parse(self, lexer: Union[BaseLexer, str], *, with_ret: bool = False, close_lexer: bool = True) -> Any:
-        """parse kola text
-
-        :param lexer: Lexer object or legal KoiLang string
-        :type lexer: Union[BaseLexer, str]
-        :param with_ret: if true, return a gererater where command returns would be yielded, defaults to False
-        :type with_ret: bool, optional
-        :param close_lexer: whether or not to close the lexer, defaults to True
-        :type close_lexer: bool, optional
-        :raises ValueError: when a KoiLang string given without trying to close it
-        :return: return a generator if `with_ret` set
-        :rtype: Generator[Any, None, None] or None
+        """
+        Parse kola text or lexer from other method.
         """
         if isinstance(lexer, str):
-            if not close_lexer:  # pragma: no cover
+            if not close_lexer:
                 raise ValueError("inner string lexer must be closed at the end of parsing")
             lexer = StringLexer(
                 lexer,
                 encoding=self.__class__.__text_encoding__,
-                command_threshold=self.__class__.__command_threshold__,
-                no_lstrip=not self.__class__.__text_lstrip__
+                command_threshold=self.__class__.__command_threshold__
             )
         if with_ret:
             return self.__parse_and_ret(lexer, close_lexer=close_lexer)
         else:
             self.__parse(lexer, close_lexer=close_lexer)
         
     def parse_file(self, path: Union[str, bytes, os.PathLike], *, encoding: Optional[str] = None, **kwds: Any) -> Any:
         """
-        parse a kola file.
+        Parse a kola file.
         """
         return self.parse(
             FileLexer(
                 path, encoding=encoding or self.__class__.__text_encoding__,
-                command_threshold=self.__class__.__command_threshold__,
-                no_lstrip=not self.__class__.__text_lstrip__
+                command_threshold=self.__class__.__command_threshold__
             ), **kwds
         )
     
     @contextmanager
     def exec_block(self) -> Generator[Self, None, None]:
         if not self.__exec_level:
-            self.at_start()
+            self["@start"]()
         self.__exec_level += 1
         try:
             yield self
         finally:
             self.__exec_level -= 1
             if not self.__exec_level:
-                self.at_end()
+                self["@end"]()
 
     def __getitem__(self, __key: str) -> Callable:
         if self.__top is self:
             return super().__getitem__(__key)
         return self.__top[__key]
 
     def __kola_caller__(
         self,
         command: Command,
         args: tuple,
         kwargs: Dict[str, Any],
         *,
         bound_instance: Optional[CommandSet] = None,
         envs: Tuple[str, ...] = (),
-        skip: bool = False,
         **kwds: Any
     ) -> Any:
         if envs:
             self.ensure_env(envs)
-        if not skip:
-            return command.__func__(bound_instance or self, *args, **kwargs)
+        return command.__func__(bound_instance or self, *args, **kwargs)
 
     @property
     def top(self) -> CommandSet:
         return self.__top
     
     @property
     def home(self) -> Self:
         return self
 
-    @partial(Command, "@start", virtual=True)
     def at_start(self) -> None:
         """
         parser initalize command
         
         It is called before parsing start.
         """
 
-    @partial(Command, "@end", virtual=True)
     def at_end(self) -> None:
         """
         parser finalize command
         
         It is called after parsing end. And the return value
         will be that of 'parse' method.
         """
+        while isinstance(self.__top, Environment) and self.__top.__class__.__env_autopop__:
+            cache = self.pop_start()
+            self.pop_end(cache)
     
-    @partial(Command, "@exception", virtual=True)
-    def on_exception(self, exc_type: Type[KoiLangError], exc_ins: Optional[KoiLangError], traceback: TracebackType) -> None:
+    def on_exception(self, exc_type: Type[BaseException], exc_ins: BaseException, traceback: TracebackType) -> None:
         """
         exception handling command
 
         It is called when a KoiLang error occurs.
         If the command wishes to suppress the exception, it should a true value.
         """
```

### Comparing `KoiLang-1.1.0/kola/klvm/writer.py` & `KoiLang-1.1.0b2/kola/klvm/writer.py`

 * *Files 11% similar despite different names*

```diff
@@ -45,21 +45,21 @@
         else:
             self._writer = FileWriter(
                 ___writer,
                 command_threshold=self.__class__.__command_threshold__,
                 encoding=self.__class__.__text_encoding__
             )
     
-    def push_apply(self, __push_cache: Environment) -> None:
+    def push_end(self, __push_cache: Environment) -> None:
         self._writer.inc_indent()
-        return super().push_apply(__push_cache)
+        return super().push_end(__push_cache)
     
-    def pop_prepare(self, __env_type: Optional[Type[Environment]] = None) -> Environment:
+    def pop_start(self, __env_type: Optional[Type[Environment]] = None) -> Environment:
         self._writer.dec_indent()
-        return super().pop_prepare(__env_type)
+        return super().pop_start(__env_type)
     
     def __kola_caller__(
         self,
         command: Command,
         args: tuple,
         kwargs: Dict[str, Any],
         *,
@@ -70,28 +70,28 @@
         # if isinstance(command.__wrapped__, Command):
         #     return super().__kola_caller__(
         #         command, args, kwargs, envs=envs, writer_func=writer_func, **kwds
         #     )
         if envs:
             self.ensure_env(envs)
         
-        if command.__name__ in ["@start", "@end"]:  # pragma: no cover
+        if command.__name__ in ["@start", "@end"]:
             # writer do not need to initalize
             return
         if not writer_func:
             writer_func = _default_writer_factory(
                 command.__name__, signature(command.__func__)
             )
         writer_func(self._writer, *args, **kwargs)
     
     def newline(self) -> None:
         self._writer.newline()
     
     def getvalue(self) -> str:
-        if not isinstance(self._writer, StringWriter):  # pragma: no cover
+        if not isinstance(self._writer, StringWriter):
             raise TypeError("only `StringWriter` object can use 'getvalue' method")
         return self._writer.getvalue()
 
     def __enter__(self) -> Self:
         self._writer.__enter__()
         return self
```

### Comparing `KoiLang-1.1.0/kola/lexer.c` & `KoiLang-1.1.0b2/kola/lexer.c`

 * *Files 2% similar despite different names*

```diff
@@ -1255,28 +1255,28 @@
 struct __pyx_opt_args_7cpython_11contextvars_get_value_no_default {
   int __pyx_n;
   PyObject *default_value;
 };
 struct __pyx_ctuple_int__and_char__space_const__ptr__and_Py_ssize_t;
 typedef struct __pyx_ctuple_int__and_char__space_const__ptr__and_Py_ssize_t __pyx_ctuple_int__and_char__space_const__ptr__and_Py_ssize_t;
 
-/* "kola/lexer.pxd":39
+/* "kola/lexer.pxd":35
  *     cpdef void close(self)
  *     cdef void set_error(self, const char* text) except *
  *     cdef (int, const char*, Py_ssize_t) next_syn(self) nogil             # <<<<<<<<<<<<<<
  *     cdef Token next_token(self)
  * 
  */
 struct __pyx_ctuple_int__and_char__space_const__ptr__and_Py_ssize_t {
   int f0;
   char const *f1;
   Py_ssize_t f2;
 };
 
-/* "kola/lexer.pxd":12
+/* "kola/lexer.pxd":8
  * 
  * 
  * cdef class Token:             # <<<<<<<<<<<<<<
  *     cdef:
  *         Token next     # used in grammar parser
  */
 struct __pyx_obj_4kola_5lexer_Token {
@@ -1286,29 +1286,29 @@
   enum TokenSyn syn;
   PyObject *val;
   PyObject *raw_val;
   int lineno;
 };
 
 
-/* "kola/lexer.pxd":24
+/* "kola/lexer.pxd":20
  * 
  * 
  * cdef class LexerConfig:             # <<<<<<<<<<<<<<
  *     cdef LexerData* lexer_data
  *     cdef readonly BaseLexer lexer
  */
 struct __pyx_obj_4kola_5lexer_LexerConfig {
   PyObject_HEAD
   LexerData *lexer_data;
   struct __pyx_obj_4kola_5lexer_BaseLexer *lexer;
 };
 
 
-/* "kola/lexer.pxd":30
+/* "kola/lexer.pxd":26
  * 
  * @cython.no_gc
  * cdef class BaseLexer:             # <<<<<<<<<<<<<<
  *     cdef:
  *         yyscan_t scanner
  */
 struct __pyx_obj_4kola_5lexer_BaseLexer {
@@ -1316,58 +1316,58 @@
   struct __pyx_vtabstruct_4kola_5lexer_BaseLexer *__pyx_vtab;
   yyscan_t scanner;
   LexerData lexer_data;
   PyObject *encoding;
 };
 
 
-/* "kola/lexer.pxd":43
+/* "kola/lexer.pxd":39
  * 
  * 
  * cdef class FileLexer(BaseLexer):             # <<<<<<<<<<<<<<
  *     cdef:
  *         object _filenameo
  */
 struct __pyx_obj_4kola_5lexer_FileLexer {
   struct __pyx_obj_4kola_5lexer_BaseLexer __pyx_base;
   PyObject *_filenameo;
   PyObject *_filenameb;
   FILE *fp;
 };
 
 
-/* "kola/lexer.pxd":53
+/* "kola/lexer.pxd":49
  * 
  * @cython.no_gc
  * cdef class StringLexer(BaseLexer):             # <<<<<<<<<<<<<<
  *     cdef readonly bytes content
  */
 struct __pyx_obj_4kola_5lexer_StringLexer {
   struct __pyx_obj_4kola_5lexer_BaseLexer __pyx_base;
   PyObject *content;
 };
 
 
 
-/* "kola/lexer.pyx":37
+/* "kola/lexer.pyx":34
  * 
  * @cython.final
  * cdef class Token:             # <<<<<<<<<<<<<<
  *     """
  *     Token used in lexer
  */
 
 struct __pyx_vtabstruct_4kola_5lexer_Token {
   int (*get_flag)(struct __pyx_obj_4kola_5lexer_Token *, int __pyx_skip_dispatch);
 };
 static struct __pyx_vtabstruct_4kola_5lexer_Token *__pyx_vtabptr_4kola_5lexer_Token;
 static int __pyx_f_4kola_5lexer_5Token_get_flag(struct __pyx_obj_4kola_5lexer_Token *, int __pyx_skip_dispatch);
 
 
-/* "kola/lexer.pyx":161
+/* "kola/lexer.pyx":148
  * 
  * 
  * cdef class BaseLexer(object):             # <<<<<<<<<<<<<<
  *     """
  *     KoiLang lexer reading from stdin
  */
 
@@ -1376,29 +1376,29 @@
   void (*set_error)(struct __pyx_obj_4kola_5lexer_BaseLexer *, char const *);
   __pyx_ctuple_int__and_char__space_const__ptr__and_Py_ssize_t (*next_syn)(struct __pyx_obj_4kola_5lexer_BaseLexer *);
   struct __pyx_obj_4kola_5lexer_Token *(*next_token)(struct __pyx_obj_4kola_5lexer_BaseLexer *);
 };
 static struct __pyx_vtabstruct_4kola_5lexer_BaseLexer *__pyx_vtabptr_4kola_5lexer_BaseLexer;
 
 
-/* "kola/lexer.pyx":296
+/* "kola/lexer.pyx":280
  * 
  * 
  * cdef class FileLexer(BaseLexer):             # <<<<<<<<<<<<<<
  *     """
  *     KoiLang lexer reading from file
  */
 
 struct __pyx_vtabstruct_4kola_5lexer_FileLexer {
   struct __pyx_vtabstruct_4kola_5lexer_BaseLexer __pyx_base;
 };
 static struct __pyx_vtabstruct_4kola_5lexer_FileLexer *__pyx_vtabptr_4kola_5lexer_FileLexer;
 
 
-/* "kola/lexer.pyx":327
+/* "kola/lexer.pyx":311
  * 
  * 
  * cdef class StringLexer(BaseLexer):             # <<<<<<<<<<<<<<
  *     """
  *     KoiLang lexer reading from string provided
  */
 
@@ -1645,27 +1645,60 @@
 
 /* KeywordStringCheck.proto */
 static int __Pyx_CheckKeywordStrings(PyObject *kw, const char* function_name, int kw_allowed);
 
 /* RaiseException.proto */
 static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb, PyObject *cause);
 
-/* IterFinish.proto */
-static CYTHON_INLINE int __Pyx_IterFinish(void);
+/* RaiseUnexpectedTypeError.proto */
+static int __Pyx_RaiseUnexpectedTypeError(const char *expected, PyObject *obj);
+
+/* decode_c_string_utf16.proto */
+static CYTHON_INLINE PyObject *__Pyx_PyUnicode_DecodeUTF16(const char *s, Py_ssize_t size, const char *errors) {
+    int byteorder = 0;
+    return PyUnicode_DecodeUTF16(s, size, errors, &byteorder);
+}
+static CYTHON_INLINE PyObject *__Pyx_PyUnicode_DecodeUTF16LE(const char *s, Py_ssize_t size, const char *errors) {
+    int byteorder = -1;
+    return PyUnicode_DecodeUTF16(s, size, errors, &byteorder);
+}
+static CYTHON_INLINE PyObject *__Pyx_PyUnicode_DecodeUTF16BE(const char *s, Py_ssize_t size, const char *errors) {
+    int byteorder = 1;
+    return PyUnicode_DecodeUTF16(s, size, errors, &byteorder);
+}
 
-/* set_iter.proto */
-static CYTHON_INLINE PyObject* __Pyx_set_iterator(PyObject* iterable, int is_set,
-                                                  Py_ssize_t* p_orig_length, int* p_source_is_set);
-static CYTHON_INLINE int __Pyx_set_iter_next(
-        PyObject* iter_obj, Py_ssize_t orig_length,
-        Py_ssize_t* ppos, PyObject **value,
-        int source_is_set);
+/* decode_c_bytes.proto */
+static CYTHON_INLINE PyObject* __Pyx_decode_c_bytes(
+         const char* cstring, Py_ssize_t length, Py_ssize_t start, Py_ssize_t stop,
+         const char* encoding, const char* errors,
+         PyObject* (*decode_func)(const char *s, Py_ssize_t size, const char *errors));
 
-/* GetAttr.proto */
-static CYTHON_INLINE PyObject *__Pyx_GetAttr(PyObject *, PyObject *);
+/* decode_bytes.proto */
+static CYTHON_INLINE PyObject* __Pyx_decode_bytes(
+         PyObject* string, Py_ssize_t start, Py_ssize_t stop,
+         const char* encoding, const char* errors,
+         PyObject* (*decode_func)(const char *s, Py_ssize_t size, const char *errors)) {
+    return __Pyx_decode_c_bytes(
+        PyBytes_AS_STRING(string), PyBytes_GET_SIZE(string),
+        start, stop, encoding, errors, decode_func);
+}
+
+/* DictGetItem.proto */
+#if PY_MAJOR_VERSION >= 3 && !CYTHON_COMPILING_IN_PYPY
+static PyObject *__Pyx_PyDict_GetItem(PyObject *d, PyObject* key);
+#define __Pyx_PyObject_Dict_GetItem(obj, name)\
+    (likely(PyDict_CheckExact(obj)) ?\
+     __Pyx_PyDict_GetItem(obj, name) : PyObject_GetItem(obj, name))
+#else
+#define __Pyx_PyDict_GetItem(d, key) PyObject_GetItem(d, key)
+#define __Pyx_PyObject_Dict_GetItem(obj, name)  PyObject_GetItem(obj, name)
+#endif
+
+/* IterFinish.proto */
+static CYTHON_INLINE int __Pyx_IterFinish(void);
 
 /* PyObjectCallNoArg.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyObject_CallNoArg(PyObject *func);
 
 /* PyObjectGetMethod.proto */
 static int __Pyx_PyObject_GetMethod(PyObject *obj, PyObject *name, PyObject **method);
 
@@ -1701,34 +1734,14 @@
 
 /* dict_iter.proto */
 static CYTHON_INLINE PyObject* __Pyx_dict_iterator(PyObject* dict, int is_dict, PyObject* method_name,
                                                    Py_ssize_t* p_orig_length, int* p_is_dict);
 static CYTHON_INLINE int __Pyx_dict_iter_next(PyObject* dict_or_iter, Py_ssize_t orig_length, Py_ssize_t* ppos,
                                               PyObject** pkey, PyObject** pvalue, PyObject** pitem, int is_dict);
 
-/* pyfrozenset_new.proto */
-static CYTHON_INLINE PyObject* __Pyx_PyFrozenSet_New(PyObject* it);
-
-/* PySetContains.proto */
-static CYTHON_INLINE int __Pyx_PySet_ContainsTF(PyObject* key, PyObject* set, int eq);
-
-/* decode_c_string_utf16.proto */
-static CYTHON_INLINE PyObject *__Pyx_PyUnicode_DecodeUTF16(const char *s, Py_ssize_t size, const char *errors) {
-    int byteorder = 0;
-    return PyUnicode_DecodeUTF16(s, size, errors, &byteorder);
-}
-static CYTHON_INLINE PyObject *__Pyx_PyUnicode_DecodeUTF16LE(const char *s, Py_ssize_t size, const char *errors) {
-    int byteorder = -1;
-    return PyUnicode_DecodeUTF16(s, size, errors, &byteorder);
-}
-static CYTHON_INLINE PyObject *__Pyx_PyUnicode_DecodeUTF16BE(const char *s, Py_ssize_t size, const char *errors) {
-    int byteorder = 1;
-    return PyUnicode_DecodeUTF16(s, size, errors, &byteorder);
-}
-
 /* decode_c_string.proto */
 static CYTHON_INLINE PyObject* __Pyx_decode_c_string(
          const char* cstring, Py_ssize_t start, Py_ssize_t stop,
          const char* encoding, const char* errors,
          PyObject* (*decode_func)(const char *s, Py_ssize_t size, const char *errors));
 
 /* PyDictVersioning.proto */
@@ -1779,17 +1792,14 @@
 static PyObject *__Pyx__GetModuleGlobalName(PyObject *name, PY_UINT64_T *dict_version, PyObject **dict_cached_value);
 #else
 #define __Pyx_GetModuleGlobalName(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 #define __Pyx_GetModuleGlobalNameUncached(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 static CYTHON_INLINE PyObject *__Pyx__GetModuleGlobalName(PyObject *name);
 #endif
 
-/* RaiseUnexpectedTypeError.proto */
-static int __Pyx_RaiseUnexpectedTypeError(const char *expected, PyObject *obj);
-
 /* GetTopmostException.proto */
 #if CYTHON_USE_EXC_INFO_STACK
 static _PyErr_StackItem * __Pyx_PyErr_GetTopmostException(PyThreadState *tstate);
 #endif
 
 /* SaveResetException.proto */
 #if CYTHON_FAST_THREAD_STATE
@@ -2001,18 +2011,14 @@
 /* CythonFunction.proto */
 static PyObject *__Pyx_CyFunction_New(PyMethodDef *ml,
                                       int flags, PyObject* qualname,
                                       PyObject *closure,
                                       PyObject *module, PyObject *globals,
                                       PyObject* code);
 
-/* unicode_tailmatch.proto */
-static int __Pyx_PyUnicode_Tailmatch(
-    PyObject* s, PyObject* substr, Py_ssize_t start, Py_ssize_t end, int direction);
-
 /* CLineInTraceback.proto */
 #ifdef CYTHON_CLINE_IN_TRACEBACK
 #define __Pyx_CLineForTraceback(tstate, c_line)  (((CYTHON_CLINE_IN_TRACEBACK)) ? c_line : 0)
 #else
 static int __Pyx_CLineForTraceback(PyThreadState *tstate, int c_line);
 #endif
 
@@ -2038,14 +2044,15 @@
                                int py_line, const char *filename);
 
 /* GCCDiagnostics.proto */
 #if defined(__GNUC__) && (__GNUC__ > 4 || (__GNUC__ == 4 && __GNUC_MINOR__ >= 6))
 #define __Pyx_HAS_GCC_DIAGNOSTIC
 #endif
 
+static PyObject* __pyx_convert__to_py_LexerData(LexerData s);
 /* CIntToPy.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyInt_From_enum__TokenSyn(enum TokenSyn value);
 
 /* CIntToPy.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int(int value);
 
 /* CIntFromPy.proto */
@@ -2307,45 +2314,43 @@
 #if !CYTHON_USE_MODULE_STATE
 static PyTypeObject *__pyx_ptype_4kola_5lexer_Token = 0;
 static PyTypeObject *__pyx_ptype_4kola_5lexer_LexerConfig = 0;
 static PyTypeObject *__pyx_ptype_4kola_5lexer_BaseLexer = 0;
 static PyTypeObject *__pyx_ptype_4kola_5lexer_FileLexer = 0;
 static PyTypeObject *__pyx_ptype_4kola_5lexer_StringLexer = 0;
 #endif
-static PyObject *__pyx_v_4kola_5lexer__lexer_data_names = 0;
-static PyObject *__pyx_7genexpr__pyx_v_4kola_5lexer_i;
 /* #### Code section: typeinfo ### */
 /* #### Code section: before_global_var ### */
 #define __Pyx_MODULE_NAME "kola.lexer"
 extern int __pyx_module_is_main_kola__lexer;
 int __pyx_module_is_main_kola__lexer = 0;
 
 /* Implementation of "kola.lexer" */
 /* #### Code section: global_var ### */
 static PyObject *__pyx_builtin_TypeError;
 static PyObject *__pyx_builtin_AttributeError;
 static PyObject *__pyx_builtin_RuntimeError;
 static PyObject *__pyx_builtin_OSError;
 static PyObject *__pyx_builtin_StopIteration;
 /* #### Code section: string_decls ### */
-static const char __pyx_k_i[] = "i";
+static const char __pyx_k_[] = "__";
 static const char __pyx_k_k[] = "k";
 static const char __pyx_k_v[] = "v";
-static const char __pyx_k__2[] = ".";
+static const char __pyx_k__3[] = ".";
 static const char __pyx_k_gc[] = "gc";
-static const char __pyx_k__14[] = "__";
 static const char __pyx_k__26[] = "?";
 static const char __pyx_k_set[] = "set";
 static const char __pyx_k_syn[] = "syn";
 static const char __pyx_k_val[] = "val";
 static const char __pyx_k_None[] = "None";
 static const char __pyx_k_args[] = "args";
 static const char __pyx_k_data[] = "data";
 static const char __pyx_k_dict[] = "dict";
 static const char __pyx_k_exit[] = "__exit__";
+static const char __pyx_k_flag[] = "flag";
 static const char __pyx_k_kwds[] = "kwds";
 static const char __pyx_k_main[] = "__main__";
 static const char __pyx_k_name[] = "__name__";
 static const char __pyx_k_self[] = "self";
 static const char __pyx_k_test[] = "__test__";
 static const char __pyx_k_S_CLN[] = "S_CLN";
 static const char __pyx_k_S_CMA[] = "S_CMA";
@@ -2370,29 +2375,32 @@
 static const char __pyx_k_S_NUM_B[] = "S_NUM_B";
 static const char __pyx_k_S_NUM_F[] = "S_NUM_F";
 static const char __pyx_k_S_NUM_H[] = "S_NUM_H";
 static const char __pyx_k_content[] = "content";
 static const char __pyx_k_disable[] = "disable";
 static const char __pyx_k_raw_val[] = "raw_val";
 static const char __pyx_k_S_STRING[] = "S_STRING";
+static const char __pyx_k_encoding[] = "encoding";
+static const char __pyx_k_endswith[] = "endswith";
+static const char __pyx_k_filename[] = "filename";
 static const char __pyx_k_get_flag[] = "get_flag";
 static const char __pyx_k_getstate[] = "__getstate__";
 static const char __pyx_k_setstate[] = "__setstate__";
 static const char __pyx_k_BaseLexer[] = "BaseLexer";
 static const char __pyx_k_FileLexer[] = "FileLexer";
 static const char __pyx_k_S_LITERAL[] = "S_LITERAL";
 static const char __pyx_k_TypeError[] = "TypeError";
 static const char __pyx_k_exception[] = "exception";
 static const char __pyx_k_isenabled[] = "isenabled";
 static const char __pyx_k_pyx_state[] = "__pyx_state";
 static const char __pyx_k_reduce_ex[] = "__reduce_ex__";
 static const char __pyx_k_F_DISABLED[] = "F_DISABLED";
-static const char __pyx_k_data_names[] = "data_names";
 static const char __pyx_k_kola_lexer[] = "kola.lexer";
 static const char __pyx_k_pyx_vtable[] = "__pyx_vtable__";
+static const char __pyx_k_startswith[] = "startswith";
 static const char __pyx_k_LexerConfig[] = "LexerConfig";
 static const char __pyx_k_StringLexer[] = "StringLexer";
 static const char __pyx_k_RuntimeError[] = "RuntimeError";
 static const char __pyx_k_S_ANNOTATION[] = "S_ANNOTATION";
 static const char __pyx_k_is_coroutine[] = "_is_coroutine";
 static const char __pyx_k_stringsource[] = "<stringsource>";
 static const char __pyx_k_F_LSTRIP_TEXT[] = "F_LSTRIP_TEXT";
@@ -2405,14 +2413,15 @@
 static const char __pyx_k_FileLexer__path[] = "_FileLexer__path";
 static const char __pyx_k_FileLexer_close[] = "FileLexer.close";
 static const char __pyx_k_LexerConfig_set[] = "LexerConfig.set";
 static const char __pyx_k_setstate_cython[] = "__setstate_cython__";
 static const char __pyx_k_BaseLexer___exit[] = "BaseLexer.__exit__";
 static const char __pyx_k_LexerConfig_dict[] = "LexerConfig.dict";
 static const char __pyx_k_BaseLexer___enter[] = "BaseLexer.__enter__";
+static const char __pyx_k_command_threshold[] = "command_threshold";
 static const char __pyx_k_KoiLangSyntaxError[] = "KoiLangSyntaxError";
 static const char __pyx_k_asyncio_coroutines[] = "asyncio.coroutines";
 static const char __pyx_k_cline_in_traceback[] = "cline_in_traceback";
 static const char __pyx_k_Token___reduce_cython[] = "Token.__reduce_cython__";
 static const char __pyx_k_Token___setstate_cython[] = "Token.__setstate_cython__";
 static const char __pyx_k_BaseLexer___reduce_cython[] = "BaseLexer.__reduce_cython__";
 static const char __pyx_k_FileLexer___reduce_cython[] = "FileLexer.__reduce_cython__";
@@ -2422,14 +2431,15 @@
 static const char __pyx_k_LexerConfig___reduce_cython[] = "LexerConfig.__reduce_cython__";
 static const char __pyx_k_StringLexer___reduce_cython[] = "StringLexer.__reduce_cython__";
 static const char __pyx_k_LexerConfig___setstate_cython[] = "LexerConfig.__setstate_cython__";
 static const char __pyx_k_StringLexer___setstate_cython[] = "StringLexer.__setstate_cython__";
 static const char __pyx_k_no_default___reduce___due_to_non[] = "no default __reduce__ due to non-trivial __cinit__";
 static const char __pyx_k_self_lexer_data_cannot_be_conver[] = "self.lexer_data cannot be converted to a Python object for pickling";
 #if !CYTHON_USE_MODULE_STATE
+static PyObject *__pyx_n_u_;
 static PyObject *__pyx_n_s_AttributeError;
 static PyObject *__pyx_n_s_BaseLexer;
 static PyObject *__pyx_n_s_BaseLexer___enter;
 static PyObject *__pyx_n_s_BaseLexer___exit;
 static PyObject *__pyx_n_s_BaseLexer___reduce_cython;
 static PyObject *__pyx_n_s_BaseLexer___setstate_cython;
 static PyObject *__pyx_n_s_BaseLexer_close;
@@ -2468,34 +2478,37 @@
 static PyObject *__pyx_n_s_StringLexer___reduce_cython;
 static PyObject *__pyx_n_s_StringLexer___setstate_cython;
 static PyObject *__pyx_n_s_Token;
 static PyObject *__pyx_n_s_Token___reduce_cython;
 static PyObject *__pyx_n_s_Token___setstate_cython;
 static PyObject *__pyx_n_s_Token_get_flag;
 static PyObject *__pyx_n_s_TypeError;
-static PyObject *__pyx_n_u__14;
-static PyObject *__pyx_kp_u__2;
 static PyObject *__pyx_n_s__26;
+static PyObject *__pyx_kp_u__3;
 static PyObject *__pyx_n_s_args;
 static PyObject *__pyx_n_s_asyncio_coroutines;
 static PyObject *__pyx_n_s_cline_in_traceback;
 static PyObject *__pyx_n_s_close;
+static PyObject *__pyx_n_s_command_threshold;
 static PyObject *__pyx_n_s_content;
 static PyObject *__pyx_n_s_data;
-static PyObject *__pyx_n_u_data_names;
 static PyObject *__pyx_n_s_dict;
 static PyObject *__pyx_kp_u_disable;
 static PyObject *__pyx_kp_u_enable;
+static PyObject *__pyx_n_u_encoding;
+static PyObject *__pyx_n_s_endswith;
 static PyObject *__pyx_n_s_enter;
 static PyObject *__pyx_n_s_exception;
 static PyObject *__pyx_n_s_exit;
+static PyObject *__pyx_n_s_filename;
+static PyObject *__pyx_n_u_filename;
+static PyObject *__pyx_n_s_flag;
 static PyObject *__pyx_kp_u_gc;
 static PyObject *__pyx_n_s_get_flag;
 static PyObject *__pyx_n_s_getstate;
-static PyObject *__pyx_n_s_i;
 static PyObject *__pyx_n_s_import;
 static PyObject *__pyx_n_s_is_coroutine;
 static PyObject *__pyx_kp_u_isenabled;
 static PyObject *__pyx_n_s_items;
 static PyObject *__pyx_n_s_k;
 static PyObject *__pyx_n_s_kola_lexer;
 static PyObject *__pyx_kp_s_kola_lexer_pyx;
@@ -2514,14 +2527,15 @@
 static PyObject *__pyx_n_s_reduce_ex;
 static PyObject *__pyx_n_s_return;
 static PyObject *__pyx_n_s_self;
 static PyObject *__pyx_kp_s_self_lexer_data_cannot_be_conver;
 static PyObject *__pyx_n_s_set;
 static PyObject *__pyx_n_s_setstate;
 static PyObject *__pyx_n_s_setstate_cython;
+static PyObject *__pyx_n_s_startswith;
 static PyObject *__pyx_kp_s_stringsource;
 static PyObject *__pyx_n_s_syn;
 static PyObject *__pyx_n_s_test;
 static PyObject *__pyx_kp_u_utf_8;
 static PyObject *__pyx_n_s_v;
 static PyObject *__pyx_n_s_val;
 #endif
@@ -2583,27 +2597,27 @@
 static PyObject *__pyx_tp_new_4kola_5lexer_LexerConfig(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_4kola_5lexer_BaseLexer(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_4kola_5lexer_FileLexer(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_4kola_5lexer_StringLexer(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 #if !CYTHON_USE_MODULE_STATE
 #endif
 #if !CYTHON_USE_MODULE_STATE
-static PyObject *__pyx_tuple_;
-static PyObject *__pyx_tuple__3;
-static PyObject *__pyx_tuple__6;
-static PyObject *__pyx_tuple__8;
-static PyObject *__pyx_tuple__10;
+static PyObject *__pyx_tuple__2;
+static PyObject *__pyx_tuple__4;
+static PyObject *__pyx_tuple__7;
+static PyObject *__pyx_tuple__9;
+static PyObject *__pyx_tuple__11;
 static PyObject *__pyx_tuple__17;
-static PyObject *__pyx_codeobj__4;
 static PyObject *__pyx_codeobj__5;
-static PyObject *__pyx_codeobj__7;
-static PyObject *__pyx_codeobj__9;
-static PyObject *__pyx_codeobj__11;
+static PyObject *__pyx_codeobj__6;
+static PyObject *__pyx_codeobj__8;
+static PyObject *__pyx_codeobj__10;
 static PyObject *__pyx_codeobj__12;
 static PyObject *__pyx_codeobj__13;
+static PyObject *__pyx_codeobj__14;
 static PyObject *__pyx_codeobj__15;
 static PyObject *__pyx_codeobj__16;
 static PyObject *__pyx_codeobj__18;
 static PyObject *__pyx_codeobj__19;
 static PyObject *__pyx_codeobj__20;
 static PyObject *__pyx_codeobj__21;
 static PyObject *__pyx_codeobj__22;
@@ -2636,14 +2650,15 @@
   PyObject *__pyx_type_4kola_5lexer_LexerConfig;
   PyTypeObject *__pyx_ptype_4kola_5lexer_BaseLexer;
   PyObject *__pyx_type_4kola_5lexer_BaseLexer;
   PyTypeObject *__pyx_ptype_4kola_5lexer_FileLexer;
   PyObject *__pyx_type_4kola_5lexer_FileLexer;
   PyTypeObject *__pyx_ptype_4kola_5lexer_StringLexer;
   PyObject *__pyx_type_4kola_5lexer_StringLexer;
+  PyObject *__pyx_n_u_;
   PyObject *__pyx_n_s_AttributeError;
   PyObject *__pyx_n_s_BaseLexer;
   PyObject *__pyx_n_s_BaseLexer___enter;
   PyObject *__pyx_n_s_BaseLexer___exit;
   PyObject *__pyx_n_s_BaseLexer___reduce_cython;
   PyObject *__pyx_n_s_BaseLexer___setstate_cython;
   PyObject *__pyx_n_s_BaseLexer_close;
@@ -2682,34 +2697,37 @@
   PyObject *__pyx_n_s_StringLexer___reduce_cython;
   PyObject *__pyx_n_s_StringLexer___setstate_cython;
   PyObject *__pyx_n_s_Token;
   PyObject *__pyx_n_s_Token___reduce_cython;
   PyObject *__pyx_n_s_Token___setstate_cython;
   PyObject *__pyx_n_s_Token_get_flag;
   PyObject *__pyx_n_s_TypeError;
-  PyObject *__pyx_n_u__14;
-  PyObject *__pyx_kp_u__2;
   PyObject *__pyx_n_s__26;
+  PyObject *__pyx_kp_u__3;
   PyObject *__pyx_n_s_args;
   PyObject *__pyx_n_s_asyncio_coroutines;
   PyObject *__pyx_n_s_cline_in_traceback;
   PyObject *__pyx_n_s_close;
+  PyObject *__pyx_n_s_command_threshold;
   PyObject *__pyx_n_s_content;
   PyObject *__pyx_n_s_data;
-  PyObject *__pyx_n_u_data_names;
   PyObject *__pyx_n_s_dict;
   PyObject *__pyx_kp_u_disable;
   PyObject *__pyx_kp_u_enable;
+  PyObject *__pyx_n_u_encoding;
+  PyObject *__pyx_n_s_endswith;
   PyObject *__pyx_n_s_enter;
   PyObject *__pyx_n_s_exception;
   PyObject *__pyx_n_s_exit;
+  PyObject *__pyx_n_s_filename;
+  PyObject *__pyx_n_u_filename;
+  PyObject *__pyx_n_s_flag;
   PyObject *__pyx_kp_u_gc;
   PyObject *__pyx_n_s_get_flag;
   PyObject *__pyx_n_s_getstate;
-  PyObject *__pyx_n_s_i;
   PyObject *__pyx_n_s_import;
   PyObject *__pyx_n_s_is_coroutine;
   PyObject *__pyx_kp_u_isenabled;
   PyObject *__pyx_n_s_items;
   PyObject *__pyx_n_s_k;
   PyObject *__pyx_n_s_kola_lexer;
   PyObject *__pyx_kp_s_kola_lexer_pyx;
@@ -2728,33 +2746,34 @@
   PyObject *__pyx_n_s_reduce_ex;
   PyObject *__pyx_n_s_return;
   PyObject *__pyx_n_s_self;
   PyObject *__pyx_kp_s_self_lexer_data_cannot_be_conver;
   PyObject *__pyx_n_s_set;
   PyObject *__pyx_n_s_setstate;
   PyObject *__pyx_n_s_setstate_cython;
+  PyObject *__pyx_n_s_startswith;
   PyObject *__pyx_kp_s_stringsource;
   PyObject *__pyx_n_s_syn;
   PyObject *__pyx_n_s_test;
   PyObject *__pyx_kp_u_utf_8;
   PyObject *__pyx_n_s_v;
   PyObject *__pyx_n_s_val;
-  PyObject *__pyx_tuple_;
-  PyObject *__pyx_tuple__3;
-  PyObject *__pyx_tuple__6;
-  PyObject *__pyx_tuple__8;
-  PyObject *__pyx_tuple__10;
+  PyObject *__pyx_tuple__2;
+  PyObject *__pyx_tuple__4;
+  PyObject *__pyx_tuple__7;
+  PyObject *__pyx_tuple__9;
+  PyObject *__pyx_tuple__11;
   PyObject *__pyx_tuple__17;
-  PyObject *__pyx_codeobj__4;
   PyObject *__pyx_codeobj__5;
-  PyObject *__pyx_codeobj__7;
-  PyObject *__pyx_codeobj__9;
-  PyObject *__pyx_codeobj__11;
+  PyObject *__pyx_codeobj__6;
+  PyObject *__pyx_codeobj__8;
+  PyObject *__pyx_codeobj__10;
   PyObject *__pyx_codeobj__12;
   PyObject *__pyx_codeobj__13;
+  PyObject *__pyx_codeobj__14;
   PyObject *__pyx_codeobj__15;
   PyObject *__pyx_codeobj__16;
   PyObject *__pyx_codeobj__18;
   PyObject *__pyx_codeobj__19;
   PyObject *__pyx_codeobj__20;
   PyObject *__pyx_codeobj__21;
   PyObject *__pyx_codeobj__22;
@@ -2803,14 +2822,15 @@
   Py_CLEAR(clear_module_state->__pyx_type_4kola_5lexer_LexerConfig);
   Py_CLEAR(clear_module_state->__pyx_ptype_4kola_5lexer_BaseLexer);
   Py_CLEAR(clear_module_state->__pyx_type_4kola_5lexer_BaseLexer);
   Py_CLEAR(clear_module_state->__pyx_ptype_4kola_5lexer_FileLexer);
   Py_CLEAR(clear_module_state->__pyx_type_4kola_5lexer_FileLexer);
   Py_CLEAR(clear_module_state->__pyx_ptype_4kola_5lexer_StringLexer);
   Py_CLEAR(clear_module_state->__pyx_type_4kola_5lexer_StringLexer);
+  Py_CLEAR(clear_module_state->__pyx_n_u_);
   Py_CLEAR(clear_module_state->__pyx_n_s_AttributeError);
   Py_CLEAR(clear_module_state->__pyx_n_s_BaseLexer);
   Py_CLEAR(clear_module_state->__pyx_n_s_BaseLexer___enter);
   Py_CLEAR(clear_module_state->__pyx_n_s_BaseLexer___exit);
   Py_CLEAR(clear_module_state->__pyx_n_s_BaseLexer___reduce_cython);
   Py_CLEAR(clear_module_state->__pyx_n_s_BaseLexer___setstate_cython);
   Py_CLEAR(clear_module_state->__pyx_n_s_BaseLexer_close);
@@ -2849,34 +2869,37 @@
   Py_CLEAR(clear_module_state->__pyx_n_s_StringLexer___reduce_cython);
   Py_CLEAR(clear_module_state->__pyx_n_s_StringLexer___setstate_cython);
   Py_CLEAR(clear_module_state->__pyx_n_s_Token);
   Py_CLEAR(clear_module_state->__pyx_n_s_Token___reduce_cython);
   Py_CLEAR(clear_module_state->__pyx_n_s_Token___setstate_cython);
   Py_CLEAR(clear_module_state->__pyx_n_s_Token_get_flag);
   Py_CLEAR(clear_module_state->__pyx_n_s_TypeError);
-  Py_CLEAR(clear_module_state->__pyx_n_u__14);
-  Py_CLEAR(clear_module_state->__pyx_kp_u__2);
   Py_CLEAR(clear_module_state->__pyx_n_s__26);
+  Py_CLEAR(clear_module_state->__pyx_kp_u__3);
   Py_CLEAR(clear_module_state->__pyx_n_s_args);
   Py_CLEAR(clear_module_state->__pyx_n_s_asyncio_coroutines);
   Py_CLEAR(clear_module_state->__pyx_n_s_cline_in_traceback);
   Py_CLEAR(clear_module_state->__pyx_n_s_close);
+  Py_CLEAR(clear_module_state->__pyx_n_s_command_threshold);
   Py_CLEAR(clear_module_state->__pyx_n_s_content);
   Py_CLEAR(clear_module_state->__pyx_n_s_data);
-  Py_CLEAR(clear_module_state->__pyx_n_u_data_names);
   Py_CLEAR(clear_module_state->__pyx_n_s_dict);
   Py_CLEAR(clear_module_state->__pyx_kp_u_disable);
   Py_CLEAR(clear_module_state->__pyx_kp_u_enable);
+  Py_CLEAR(clear_module_state->__pyx_n_u_encoding);
+  Py_CLEAR(clear_module_state->__pyx_n_s_endswith);
   Py_CLEAR(clear_module_state->__pyx_n_s_enter);
   Py_CLEAR(clear_module_state->__pyx_n_s_exception);
   Py_CLEAR(clear_module_state->__pyx_n_s_exit);
+  Py_CLEAR(clear_module_state->__pyx_n_s_filename);
+  Py_CLEAR(clear_module_state->__pyx_n_u_filename);
+  Py_CLEAR(clear_module_state->__pyx_n_s_flag);
   Py_CLEAR(clear_module_state->__pyx_kp_u_gc);
   Py_CLEAR(clear_module_state->__pyx_n_s_get_flag);
   Py_CLEAR(clear_module_state->__pyx_n_s_getstate);
-  Py_CLEAR(clear_module_state->__pyx_n_s_i);
   Py_CLEAR(clear_module_state->__pyx_n_s_import);
   Py_CLEAR(clear_module_state->__pyx_n_s_is_coroutine);
   Py_CLEAR(clear_module_state->__pyx_kp_u_isenabled);
   Py_CLEAR(clear_module_state->__pyx_n_s_items);
   Py_CLEAR(clear_module_state->__pyx_n_s_k);
   Py_CLEAR(clear_module_state->__pyx_n_s_kola_lexer);
   Py_CLEAR(clear_module_state->__pyx_kp_s_kola_lexer_pyx);
@@ -2895,33 +2918,34 @@
   Py_CLEAR(clear_module_state->__pyx_n_s_reduce_ex);
   Py_CLEAR(clear_module_state->__pyx_n_s_return);
   Py_CLEAR(clear_module_state->__pyx_n_s_self);
   Py_CLEAR(clear_module_state->__pyx_kp_s_self_lexer_data_cannot_be_conver);
   Py_CLEAR(clear_module_state->__pyx_n_s_set);
   Py_CLEAR(clear_module_state->__pyx_n_s_setstate);
   Py_CLEAR(clear_module_state->__pyx_n_s_setstate_cython);
+  Py_CLEAR(clear_module_state->__pyx_n_s_startswith);
   Py_CLEAR(clear_module_state->__pyx_kp_s_stringsource);
   Py_CLEAR(clear_module_state->__pyx_n_s_syn);
   Py_CLEAR(clear_module_state->__pyx_n_s_test);
   Py_CLEAR(clear_module_state->__pyx_kp_u_utf_8);
   Py_CLEAR(clear_module_state->__pyx_n_s_v);
   Py_CLEAR(clear_module_state->__pyx_n_s_val);
-  Py_CLEAR(clear_module_state->__pyx_tuple_);
-  Py_CLEAR(clear_module_state->__pyx_tuple__3);
-  Py_CLEAR(clear_module_state->__pyx_tuple__6);
-  Py_CLEAR(clear_module_state->__pyx_tuple__8);
-  Py_CLEAR(clear_module_state->__pyx_tuple__10);
+  Py_CLEAR(clear_module_state->__pyx_tuple__2);
+  Py_CLEAR(clear_module_state->__pyx_tuple__4);
+  Py_CLEAR(clear_module_state->__pyx_tuple__7);
+  Py_CLEAR(clear_module_state->__pyx_tuple__9);
+  Py_CLEAR(clear_module_state->__pyx_tuple__11);
   Py_CLEAR(clear_module_state->__pyx_tuple__17);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__4);
   Py_CLEAR(clear_module_state->__pyx_codeobj__5);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__7);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__9);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__11);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__6);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__8);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__10);
   Py_CLEAR(clear_module_state->__pyx_codeobj__12);
   Py_CLEAR(clear_module_state->__pyx_codeobj__13);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__14);
   Py_CLEAR(clear_module_state->__pyx_codeobj__15);
   Py_CLEAR(clear_module_state->__pyx_codeobj__16);
   Py_CLEAR(clear_module_state->__pyx_codeobj__18);
   Py_CLEAR(clear_module_state->__pyx_codeobj__19);
   Py_CLEAR(clear_module_state->__pyx_codeobj__20);
   Py_CLEAR(clear_module_state->__pyx_codeobj__21);
   Py_CLEAR(clear_module_state->__pyx_codeobj__22);
@@ -2957,14 +2981,15 @@
   Py_VISIT(traverse_module_state->__pyx_type_4kola_5lexer_LexerConfig);
   Py_VISIT(traverse_module_state->__pyx_ptype_4kola_5lexer_BaseLexer);
   Py_VISIT(traverse_module_state->__pyx_type_4kola_5lexer_BaseLexer);
   Py_VISIT(traverse_module_state->__pyx_ptype_4kola_5lexer_FileLexer);
   Py_VISIT(traverse_module_state->__pyx_type_4kola_5lexer_FileLexer);
   Py_VISIT(traverse_module_state->__pyx_ptype_4kola_5lexer_StringLexer);
   Py_VISIT(traverse_module_state->__pyx_type_4kola_5lexer_StringLexer);
+  Py_VISIT(traverse_module_state->__pyx_n_u_);
   Py_VISIT(traverse_module_state->__pyx_n_s_AttributeError);
   Py_VISIT(traverse_module_state->__pyx_n_s_BaseLexer);
   Py_VISIT(traverse_module_state->__pyx_n_s_BaseLexer___enter);
   Py_VISIT(traverse_module_state->__pyx_n_s_BaseLexer___exit);
   Py_VISIT(traverse_module_state->__pyx_n_s_BaseLexer___reduce_cython);
   Py_VISIT(traverse_module_state->__pyx_n_s_BaseLexer___setstate_cython);
   Py_VISIT(traverse_module_state->__pyx_n_s_BaseLexer_close);
@@ -3003,34 +3028,37 @@
   Py_VISIT(traverse_module_state->__pyx_n_s_StringLexer___reduce_cython);
   Py_VISIT(traverse_module_state->__pyx_n_s_StringLexer___setstate_cython);
   Py_VISIT(traverse_module_state->__pyx_n_s_Token);
   Py_VISIT(traverse_module_state->__pyx_n_s_Token___reduce_cython);
   Py_VISIT(traverse_module_state->__pyx_n_s_Token___setstate_cython);
   Py_VISIT(traverse_module_state->__pyx_n_s_Token_get_flag);
   Py_VISIT(traverse_module_state->__pyx_n_s_TypeError);
-  Py_VISIT(traverse_module_state->__pyx_n_u__14);
-  Py_VISIT(traverse_module_state->__pyx_kp_u__2);
   Py_VISIT(traverse_module_state->__pyx_n_s__26);
+  Py_VISIT(traverse_module_state->__pyx_kp_u__3);
   Py_VISIT(traverse_module_state->__pyx_n_s_args);
   Py_VISIT(traverse_module_state->__pyx_n_s_asyncio_coroutines);
   Py_VISIT(traverse_module_state->__pyx_n_s_cline_in_traceback);
   Py_VISIT(traverse_module_state->__pyx_n_s_close);
+  Py_VISIT(traverse_module_state->__pyx_n_s_command_threshold);
   Py_VISIT(traverse_module_state->__pyx_n_s_content);
   Py_VISIT(traverse_module_state->__pyx_n_s_data);
-  Py_VISIT(traverse_module_state->__pyx_n_u_data_names);
   Py_VISIT(traverse_module_state->__pyx_n_s_dict);
   Py_VISIT(traverse_module_state->__pyx_kp_u_disable);
   Py_VISIT(traverse_module_state->__pyx_kp_u_enable);
+  Py_VISIT(traverse_module_state->__pyx_n_u_encoding);
+  Py_VISIT(traverse_module_state->__pyx_n_s_endswith);
   Py_VISIT(traverse_module_state->__pyx_n_s_enter);
   Py_VISIT(traverse_module_state->__pyx_n_s_exception);
   Py_VISIT(traverse_module_state->__pyx_n_s_exit);
+  Py_VISIT(traverse_module_state->__pyx_n_s_filename);
+  Py_VISIT(traverse_module_state->__pyx_n_u_filename);
+  Py_VISIT(traverse_module_state->__pyx_n_s_flag);
   Py_VISIT(traverse_module_state->__pyx_kp_u_gc);
   Py_VISIT(traverse_module_state->__pyx_n_s_get_flag);
   Py_VISIT(traverse_module_state->__pyx_n_s_getstate);
-  Py_VISIT(traverse_module_state->__pyx_n_s_i);
   Py_VISIT(traverse_module_state->__pyx_n_s_import);
   Py_VISIT(traverse_module_state->__pyx_n_s_is_coroutine);
   Py_VISIT(traverse_module_state->__pyx_kp_u_isenabled);
   Py_VISIT(traverse_module_state->__pyx_n_s_items);
   Py_VISIT(traverse_module_state->__pyx_n_s_k);
   Py_VISIT(traverse_module_state->__pyx_n_s_kola_lexer);
   Py_VISIT(traverse_module_state->__pyx_kp_s_kola_lexer_pyx);
@@ -3049,33 +3077,34 @@
   Py_VISIT(traverse_module_state->__pyx_n_s_reduce_ex);
   Py_VISIT(traverse_module_state->__pyx_n_s_return);
   Py_VISIT(traverse_module_state->__pyx_n_s_self);
   Py_VISIT(traverse_module_state->__pyx_kp_s_self_lexer_data_cannot_be_conver);
   Py_VISIT(traverse_module_state->__pyx_n_s_set);
   Py_VISIT(traverse_module_state->__pyx_n_s_setstate);
   Py_VISIT(traverse_module_state->__pyx_n_s_setstate_cython);
+  Py_VISIT(traverse_module_state->__pyx_n_s_startswith);
   Py_VISIT(traverse_module_state->__pyx_kp_s_stringsource);
   Py_VISIT(traverse_module_state->__pyx_n_s_syn);
   Py_VISIT(traverse_module_state->__pyx_n_s_test);
   Py_VISIT(traverse_module_state->__pyx_kp_u_utf_8);
   Py_VISIT(traverse_module_state->__pyx_n_s_v);
   Py_VISIT(traverse_module_state->__pyx_n_s_val);
-  Py_VISIT(traverse_module_state->__pyx_tuple_);
-  Py_VISIT(traverse_module_state->__pyx_tuple__3);
-  Py_VISIT(traverse_module_state->__pyx_tuple__6);
-  Py_VISIT(traverse_module_state->__pyx_tuple__8);
-  Py_VISIT(traverse_module_state->__pyx_tuple__10);
+  Py_VISIT(traverse_module_state->__pyx_tuple__2);
+  Py_VISIT(traverse_module_state->__pyx_tuple__4);
+  Py_VISIT(traverse_module_state->__pyx_tuple__7);
+  Py_VISIT(traverse_module_state->__pyx_tuple__9);
+  Py_VISIT(traverse_module_state->__pyx_tuple__11);
   Py_VISIT(traverse_module_state->__pyx_tuple__17);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__4);
   Py_VISIT(traverse_module_state->__pyx_codeobj__5);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__7);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__9);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__11);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__6);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__8);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__10);
   Py_VISIT(traverse_module_state->__pyx_codeobj__12);
   Py_VISIT(traverse_module_state->__pyx_codeobj__13);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__14);
   Py_VISIT(traverse_module_state->__pyx_codeobj__15);
   Py_VISIT(traverse_module_state->__pyx_codeobj__16);
   Py_VISIT(traverse_module_state->__pyx_codeobj__18);
   Py_VISIT(traverse_module_state->__pyx_codeobj__19);
   Py_VISIT(traverse_module_state->__pyx_codeobj__20);
   Py_VISIT(traverse_module_state->__pyx_codeobj__21);
   Py_VISIT(traverse_module_state->__pyx_codeobj__22);
@@ -3108,14 +3137,15 @@
 #define __pyx_type_4kola_5lexer_LexerConfig __pyx_mstate_global->__pyx_type_4kola_5lexer_LexerConfig
 #define __pyx_ptype_4kola_5lexer_BaseLexer __pyx_mstate_global->__pyx_ptype_4kola_5lexer_BaseLexer
 #define __pyx_type_4kola_5lexer_BaseLexer __pyx_mstate_global->__pyx_type_4kola_5lexer_BaseLexer
 #define __pyx_ptype_4kola_5lexer_FileLexer __pyx_mstate_global->__pyx_ptype_4kola_5lexer_FileLexer
 #define __pyx_type_4kola_5lexer_FileLexer __pyx_mstate_global->__pyx_type_4kola_5lexer_FileLexer
 #define __pyx_ptype_4kola_5lexer_StringLexer __pyx_mstate_global->__pyx_ptype_4kola_5lexer_StringLexer
 #define __pyx_type_4kola_5lexer_StringLexer __pyx_mstate_global->__pyx_type_4kola_5lexer_StringLexer
+#define __pyx_n_u_ __pyx_mstate_global->__pyx_n_u_
 #define __pyx_n_s_AttributeError __pyx_mstate_global->__pyx_n_s_AttributeError
 #define __pyx_n_s_BaseLexer __pyx_mstate_global->__pyx_n_s_BaseLexer
 #define __pyx_n_s_BaseLexer___enter __pyx_mstate_global->__pyx_n_s_BaseLexer___enter
 #define __pyx_n_s_BaseLexer___exit __pyx_mstate_global->__pyx_n_s_BaseLexer___exit
 #define __pyx_n_s_BaseLexer___reduce_cython __pyx_mstate_global->__pyx_n_s_BaseLexer___reduce_cython
 #define __pyx_n_s_BaseLexer___setstate_cython __pyx_mstate_global->__pyx_n_s_BaseLexer___setstate_cython
 #define __pyx_n_s_BaseLexer_close __pyx_mstate_global->__pyx_n_s_BaseLexer_close
@@ -3154,34 +3184,37 @@
 #define __pyx_n_s_StringLexer___reduce_cython __pyx_mstate_global->__pyx_n_s_StringLexer___reduce_cython
 #define __pyx_n_s_StringLexer___setstate_cython __pyx_mstate_global->__pyx_n_s_StringLexer___setstate_cython
 #define __pyx_n_s_Token __pyx_mstate_global->__pyx_n_s_Token
 #define __pyx_n_s_Token___reduce_cython __pyx_mstate_global->__pyx_n_s_Token___reduce_cython
 #define __pyx_n_s_Token___setstate_cython __pyx_mstate_global->__pyx_n_s_Token___setstate_cython
 #define __pyx_n_s_Token_get_flag __pyx_mstate_global->__pyx_n_s_Token_get_flag
 #define __pyx_n_s_TypeError __pyx_mstate_global->__pyx_n_s_TypeError
-#define __pyx_n_u__14 __pyx_mstate_global->__pyx_n_u__14
-#define __pyx_kp_u__2 __pyx_mstate_global->__pyx_kp_u__2
 #define __pyx_n_s__26 __pyx_mstate_global->__pyx_n_s__26
+#define __pyx_kp_u__3 __pyx_mstate_global->__pyx_kp_u__3
 #define __pyx_n_s_args __pyx_mstate_global->__pyx_n_s_args
 #define __pyx_n_s_asyncio_coroutines __pyx_mstate_global->__pyx_n_s_asyncio_coroutines
 #define __pyx_n_s_cline_in_traceback __pyx_mstate_global->__pyx_n_s_cline_in_traceback
 #define __pyx_n_s_close __pyx_mstate_global->__pyx_n_s_close
+#define __pyx_n_s_command_threshold __pyx_mstate_global->__pyx_n_s_command_threshold
 #define __pyx_n_s_content __pyx_mstate_global->__pyx_n_s_content
 #define __pyx_n_s_data __pyx_mstate_global->__pyx_n_s_data
-#define __pyx_n_u_data_names __pyx_mstate_global->__pyx_n_u_data_names
 #define __pyx_n_s_dict __pyx_mstate_global->__pyx_n_s_dict
 #define __pyx_kp_u_disable __pyx_mstate_global->__pyx_kp_u_disable
 #define __pyx_kp_u_enable __pyx_mstate_global->__pyx_kp_u_enable
+#define __pyx_n_u_encoding __pyx_mstate_global->__pyx_n_u_encoding
+#define __pyx_n_s_endswith __pyx_mstate_global->__pyx_n_s_endswith
 #define __pyx_n_s_enter __pyx_mstate_global->__pyx_n_s_enter
 #define __pyx_n_s_exception __pyx_mstate_global->__pyx_n_s_exception
 #define __pyx_n_s_exit __pyx_mstate_global->__pyx_n_s_exit
+#define __pyx_n_s_filename __pyx_mstate_global->__pyx_n_s_filename
+#define __pyx_n_u_filename __pyx_mstate_global->__pyx_n_u_filename
+#define __pyx_n_s_flag __pyx_mstate_global->__pyx_n_s_flag
 #define __pyx_kp_u_gc __pyx_mstate_global->__pyx_kp_u_gc
 #define __pyx_n_s_get_flag __pyx_mstate_global->__pyx_n_s_get_flag
 #define __pyx_n_s_getstate __pyx_mstate_global->__pyx_n_s_getstate
-#define __pyx_n_s_i __pyx_mstate_global->__pyx_n_s_i
 #define __pyx_n_s_import __pyx_mstate_global->__pyx_n_s_import
 #define __pyx_n_s_is_coroutine __pyx_mstate_global->__pyx_n_s_is_coroutine
 #define __pyx_kp_u_isenabled __pyx_mstate_global->__pyx_kp_u_isenabled
 #define __pyx_n_s_items __pyx_mstate_global->__pyx_n_s_items
 #define __pyx_n_s_k __pyx_mstate_global->__pyx_n_s_k
 #define __pyx_n_s_kola_lexer __pyx_mstate_global->__pyx_n_s_kola_lexer
 #define __pyx_kp_s_kola_lexer_pyx __pyx_mstate_global->__pyx_kp_s_kola_lexer_pyx
@@ -3200,47 +3233,48 @@
 #define __pyx_n_s_reduce_ex __pyx_mstate_global->__pyx_n_s_reduce_ex
 #define __pyx_n_s_return __pyx_mstate_global->__pyx_n_s_return
 #define __pyx_n_s_self __pyx_mstate_global->__pyx_n_s_self
 #define __pyx_kp_s_self_lexer_data_cannot_be_conver __pyx_mstate_global->__pyx_kp_s_self_lexer_data_cannot_be_conver
 #define __pyx_n_s_set __pyx_mstate_global->__pyx_n_s_set
 #define __pyx_n_s_setstate __pyx_mstate_global->__pyx_n_s_setstate
 #define __pyx_n_s_setstate_cython __pyx_mstate_global->__pyx_n_s_setstate_cython
+#define __pyx_n_s_startswith __pyx_mstate_global->__pyx_n_s_startswith
 #define __pyx_kp_s_stringsource __pyx_mstate_global->__pyx_kp_s_stringsource
 #define __pyx_n_s_syn __pyx_mstate_global->__pyx_n_s_syn
 #define __pyx_n_s_test __pyx_mstate_global->__pyx_n_s_test
 #define __pyx_kp_u_utf_8 __pyx_mstate_global->__pyx_kp_u_utf_8
 #define __pyx_n_s_v __pyx_mstate_global->__pyx_n_s_v
 #define __pyx_n_s_val __pyx_mstate_global->__pyx_n_s_val
-#define __pyx_tuple_ __pyx_mstate_global->__pyx_tuple_
-#define __pyx_tuple__3 __pyx_mstate_global->__pyx_tuple__3
-#define __pyx_tuple__6 __pyx_mstate_global->__pyx_tuple__6
-#define __pyx_tuple__8 __pyx_mstate_global->__pyx_tuple__8
-#define __pyx_tuple__10 __pyx_mstate_global->__pyx_tuple__10
+#define __pyx_tuple__2 __pyx_mstate_global->__pyx_tuple__2
+#define __pyx_tuple__4 __pyx_mstate_global->__pyx_tuple__4
+#define __pyx_tuple__7 __pyx_mstate_global->__pyx_tuple__7
+#define __pyx_tuple__9 __pyx_mstate_global->__pyx_tuple__9
+#define __pyx_tuple__11 __pyx_mstate_global->__pyx_tuple__11
 #define __pyx_tuple__17 __pyx_mstate_global->__pyx_tuple__17
-#define __pyx_codeobj__4 __pyx_mstate_global->__pyx_codeobj__4
 #define __pyx_codeobj__5 __pyx_mstate_global->__pyx_codeobj__5
-#define __pyx_codeobj__7 __pyx_mstate_global->__pyx_codeobj__7
-#define __pyx_codeobj__9 __pyx_mstate_global->__pyx_codeobj__9
-#define __pyx_codeobj__11 __pyx_mstate_global->__pyx_codeobj__11
+#define __pyx_codeobj__6 __pyx_mstate_global->__pyx_codeobj__6
+#define __pyx_codeobj__8 __pyx_mstate_global->__pyx_codeobj__8
+#define __pyx_codeobj__10 __pyx_mstate_global->__pyx_codeobj__10
 #define __pyx_codeobj__12 __pyx_mstate_global->__pyx_codeobj__12
 #define __pyx_codeobj__13 __pyx_mstate_global->__pyx_codeobj__13
+#define __pyx_codeobj__14 __pyx_mstate_global->__pyx_codeobj__14
 #define __pyx_codeobj__15 __pyx_mstate_global->__pyx_codeobj__15
 #define __pyx_codeobj__16 __pyx_mstate_global->__pyx_codeobj__16
 #define __pyx_codeobj__18 __pyx_mstate_global->__pyx_codeobj__18
 #define __pyx_codeobj__19 __pyx_mstate_global->__pyx_codeobj__19
 #define __pyx_codeobj__20 __pyx_mstate_global->__pyx_codeobj__20
 #define __pyx_codeobj__21 __pyx_mstate_global->__pyx_codeobj__21
 #define __pyx_codeobj__22 __pyx_mstate_global->__pyx_codeobj__22
 #define __pyx_codeobj__23 __pyx_mstate_global->__pyx_codeobj__23
 #define __pyx_codeobj__24 __pyx_mstate_global->__pyx_codeobj__24
 #define __pyx_codeobj__25 __pyx_mstate_global->__pyx_codeobj__25
 #endif
 /* #### Code section: module_code ### */
 
-/* "kola/lexer.pyx":45
+/* "kola/lexer.pyx":42
  *     """
  * 
  *     def __cinit__(             # <<<<<<<<<<<<<<
  *         self,
  *         TokenSyn syn,
  */
 
@@ -3263,24 +3297,24 @@
     #if CYTHON_USE_MODULE_STATE
     PyObject **__pyx_pyargnames[] = {&__pyx_n_s_syn,&__pyx_n_s_val,&__pyx_n_s_lineno,&__pyx_n_s_raw_val,0};
     #else
     static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_syn,&__pyx_n_s_val,&__pyx_n_s_lineno,&__pyx_n_s_raw_val,0};
     #endif
     PyObject* values[4] = {0,0,0,0};
 
-    /* "kola/lexer.pyx":48
+    /* "kola/lexer.pyx":45
  *         self,
  *         TokenSyn syn,
  *         val = None,             # <<<<<<<<<<<<<<
  *         *,
  *         int lineno = 0,
  */
     values[1] = ((PyObject *)Py_None);
 
-    /* "kola/lexer.pyx":51
+    /* "kola/lexer.pyx":48
  *         *,
  *         int lineno = 0,
  *         bytes raw_val = None             # <<<<<<<<<<<<<<
  *     ):
  *         self.syn = syn
  */
     values[3] = ((PyObject*)Py_None);
@@ -3294,66 +3328,66 @@
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
       kw_args = __Pyx_NumKwargs_VARARGS(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_VARARGS(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_syn)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 45, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 42, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (kw_args > 0) {
           PyObject* value = __Pyx_GetKwValue_VARARGS(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_val);
           if (value) { values[1] = value; kw_args--; }
-          else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 45, __pyx_L3_error)
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 42, __pyx_L3_error)
         }
       }
       if (kw_args > 0 && likely(kw_args <= 2)) {
         Py_ssize_t index;
         for (index = 2; index < 4 && kw_args > 0; index++) {
           PyObject* value = __Pyx_GetKwValue_VARARGS(__pyx_kwds, __pyx_kwvalues, *__pyx_pyargnames[index]);
           if (value) { values[index] = value; kw_args--; }
-          else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 45, __pyx_L3_error)
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 42, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "__cinit__") < 0)) __PYX_ERR(1, 45, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "__cinit__") < 0)) __PYX_ERR(1, 42, __pyx_L3_error)
       }
     } else {
       switch (__pyx_nargs) {
         case  2: values[1] = __Pyx_Arg_VARARGS(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
         case  1: values[0] = __Pyx_Arg_VARARGS(__pyx_args, 0);
         break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
-    __pyx_v_syn = ((enum TokenSyn)__Pyx_PyInt_As_enum__TokenSyn(values[0])); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 47, __pyx_L3_error)
+    __pyx_v_syn = ((enum TokenSyn)__Pyx_PyInt_As_enum__TokenSyn(values[0])); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 44, __pyx_L3_error)
     __pyx_v_val = values[1];
     if (values[2]) {
-      __pyx_v_lineno = __Pyx_PyInt_As_int(values[2]); if (unlikely((__pyx_v_lineno == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 50, __pyx_L3_error)
+      __pyx_v_lineno = __Pyx_PyInt_As_int(values[2]); if (unlikely((__pyx_v_lineno == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 47, __pyx_L3_error)
     } else {
       __pyx_v_lineno = ((int)0);
     }
     __pyx_v_raw_val = ((PyObject*)values[3]);
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__cinit__", 0, 1, 2, __pyx_nargs); __PYX_ERR(1, 45, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__cinit__", 0, 1, 2, __pyx_nargs); __PYX_ERR(1, 42, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("kola.lexer.Token.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_raw_val), (&PyBytes_Type), 1, "raw_val", 1))) __PYX_ERR(1, 51, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_raw_val), (&PyBytes_Type), 1, "raw_val", 1))) __PYX_ERR(1, 48, __pyx_L1_error)
   __pyx_r = __pyx_pf_4kola_5lexer_5Token___cinit__(((struct __pyx_obj_4kola_5lexer_Token *)__pyx_v_self), __pyx_v_syn, __pyx_v_val, __pyx_v_lineno, __pyx_v_raw_val);
 
-  /* "kola/lexer.pyx":45
+  /* "kola/lexer.pyx":42
  *     """
  * 
  *     def __cinit__(             # <<<<<<<<<<<<<<
  *         self,
  *         TokenSyn syn,
  */
 
@@ -3373,69 +3407,69 @@
   int __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__cinit__", 0);
 
-  /* "kola/lexer.pyx":53
+  /* "kola/lexer.pyx":50
  *         bytes raw_val = None
  *     ):
  *         self.syn = syn             # <<<<<<<<<<<<<<
  *         self.val = val
  * 
  */
   __pyx_v_self->syn = __pyx_v_syn;
 
-  /* "kola/lexer.pyx":54
+  /* "kola/lexer.pyx":51
  *     ):
  *         self.syn = syn
  *         self.val = val             # <<<<<<<<<<<<<<
  * 
  *         self.lineno = lineno
  */
   __Pyx_INCREF(__pyx_v_val);
   __Pyx_GIVEREF(__pyx_v_val);
   __Pyx_GOTREF(__pyx_v_self->val);
   __Pyx_DECREF(__pyx_v_self->val);
   __pyx_v_self->val = __pyx_v_val;
 
-  /* "kola/lexer.pyx":56
+  /* "kola/lexer.pyx":53
  *         self.val = val
  * 
  *         self.lineno = lineno             # <<<<<<<<<<<<<<
  *         self.raw_val = bytes(val) if raw_val is None else raw_val
  * 
  */
   __pyx_v_self->lineno = __pyx_v_lineno;
 
-  /* "kola/lexer.pyx":57
+  /* "kola/lexer.pyx":54
  * 
  *         self.lineno = lineno
  *         self.raw_val = bytes(val) if raw_val is None else raw_val             # <<<<<<<<<<<<<<
  * 
  *     def __eq__(self, other) -> bool:
  */
   __pyx_t_2 = (__pyx_v_raw_val == ((PyObject*)Py_None));
   if ((__pyx_t_2 != 0)) {
-    __pyx_t_3 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyBytes_Type)), __pyx_v_val); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 57, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_CallOneArg(((PyObject *)(&PyBytes_Type)), __pyx_v_val); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 54, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_1 = __pyx_t_3;
     __pyx_t_3 = 0;
   } else {
     __Pyx_INCREF(__pyx_v_raw_val);
     __pyx_t_1 = __pyx_v_raw_val;
   }
   __Pyx_GIVEREF(__pyx_t_1);
   __Pyx_GOTREF(__pyx_v_self->raw_val);
   __Pyx_DECREF(__pyx_v_self->raw_val);
   __pyx_v_self->raw_val = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "kola/lexer.pyx":45
+  /* "kola/lexer.pyx":42
  *     """
  * 
  *     def __cinit__(             # <<<<<<<<<<<<<<
  *         self,
  *         TokenSyn syn,
  */
 
@@ -3448,15 +3482,15 @@
   __Pyx_AddTraceback("kola.lexer.Token.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "kola/lexer.pyx":59
+/* "kola/lexer.pyx":56
  *         self.raw_val = bytes(val) if raw_val is None else raw_val
  * 
  *     def __eq__(self, other) -> bool:             # <<<<<<<<<<<<<<
  *         return self is other or self.syn == other
  * 
  */
 
@@ -3482,44 +3516,44 @@
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__eq__", 0);
 
-  /* "kola/lexer.pyx":60
+  /* "kola/lexer.pyx":57
  * 
  *     def __eq__(self, other) -> bool:
  *         return self is other or self.syn == other             # <<<<<<<<<<<<<<
  * 
  *     cpdef int get_flag(self):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_2 = (((PyObject *)__pyx_v_self) == __pyx_v_other);
   if (!__pyx_t_2) {
   } else {
-    __pyx_t_3 = __Pyx_PyBool_FromLong(__pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 60, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyBool_FromLong(__pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 57, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_1 = __pyx_t_3;
     __pyx_t_3 = 0;
     goto __pyx_L3_bool_binop_done;
   }
-  __pyx_t_3 = __Pyx_PyInt_From_enum__TokenSyn(__pyx_v_self->syn); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 60, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_enum__TokenSyn(__pyx_v_self->syn); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 57, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = PyObject_RichCompare(__pyx_t_3, __pyx_v_other, Py_EQ); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 60, __pyx_L1_error)
+  __pyx_t_4 = PyObject_RichCompare(__pyx_t_3, __pyx_v_other, Py_EQ); __Pyx_XGOTREF(__pyx_t_4); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 57, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_INCREF(__pyx_t_4);
   __pyx_t_1 = __pyx_t_4;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_L3_bool_binop_done:;
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "kola/lexer.pyx":59
+  /* "kola/lexer.pyx":56
  *         self.raw_val = bytes(val) if raw_val is None else raw_val
  * 
  *     def __eq__(self, other) -> bool:             # <<<<<<<<<<<<<<
  *         return self is other or self.syn == other
  * 
  */
 
@@ -3532,15 +3566,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "kola/lexer.pyx":62
+/* "kola/lexer.pyx":59
  *         return self is other or self.syn == other
  * 
  *     cpdef int get_flag(self):             # <<<<<<<<<<<<<<
  *         if self.syn <= TEXT or self.syn == ANNOTATION:
  *             return 0
  */
 
@@ -3554,15 +3588,15 @@
 static int __pyx_f_4kola_5lexer_5Token_get_flag(struct __pyx_obj_4kola_5lexer_Token *__pyx_v_self, CYTHON_UNUSED int __pyx_skip_dispatch) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_t_2;
   __Pyx_RefNannySetupContext("get_flag", 0);
 
-  /* "kola/lexer.pyx":63
+  /* "kola/lexer.pyx":60
  * 
  *     cpdef int get_flag(self):
  *         if self.syn <= TEXT or self.syn == ANNOTATION:             # <<<<<<<<<<<<<<
  *             return 0
  *         elif self.syn == LITERAL:
  */
   __pyx_t_2 = ((__pyx_v_self->syn <= TEXT) != 0);
@@ -3572,104 +3606,104 @@
     goto __pyx_L4_bool_binop_done;
   }
   __pyx_t_2 = ((__pyx_v_self->syn == ANNOTATION) != 0);
   __pyx_t_1 = __pyx_t_2;
   __pyx_L4_bool_binop_done:;
   if (__pyx_t_1) {
 
-    /* "kola/lexer.pyx":64
+    /* "kola/lexer.pyx":61
  *     cpdef int get_flag(self):
  *         if self.syn <= TEXT or self.syn == ANNOTATION:
  *             return 0             # <<<<<<<<<<<<<<
  *         elif self.syn == LITERAL:
  *             return 1
  */
     __pyx_r = 0;
     goto __pyx_L0;
 
-    /* "kola/lexer.pyx":63
+    /* "kola/lexer.pyx":60
  * 
  *     cpdef int get_flag(self):
  *         if self.syn <= TEXT or self.syn == ANNOTATION:             # <<<<<<<<<<<<<<
  *             return 0
  *         elif self.syn == LITERAL:
  */
   }
 
-  /* "kola/lexer.pyx":65
+  /* "kola/lexer.pyx":62
  *         if self.syn <= TEXT or self.syn == ANNOTATION:
  *             return 0
  *         elif self.syn == LITERAL:             # <<<<<<<<<<<<<<
  *             return 1
  *         elif self.syn <= NUM_F:
  */
   __pyx_t_1 = ((__pyx_v_self->syn == LITERAL) != 0);
   if (__pyx_t_1) {
 
-    /* "kola/lexer.pyx":66
+    /* "kola/lexer.pyx":63
  *             return 0
  *         elif self.syn == LITERAL:
  *             return 1             # <<<<<<<<<<<<<<
  *         elif self.syn <= NUM_F:
  *             return 2
  */
     __pyx_r = 1;
     goto __pyx_L0;
 
-    /* "kola/lexer.pyx":65
+    /* "kola/lexer.pyx":62
  *         if self.syn <= TEXT or self.syn == ANNOTATION:
  *             return 0
  *         elif self.syn == LITERAL:             # <<<<<<<<<<<<<<
  *             return 1
  *         elif self.syn <= NUM_F:
  */
   }
 
-  /* "kola/lexer.pyx":67
+  /* "kola/lexer.pyx":64
  *         elif self.syn == LITERAL:
  *             return 1
  *         elif self.syn <= NUM_F:             # <<<<<<<<<<<<<<
  *             return 2
  *         else:
  */
   __pyx_t_1 = ((__pyx_v_self->syn <= NUM_F) != 0);
   if (__pyx_t_1) {
 
-    /* "kola/lexer.pyx":68
+    /* "kola/lexer.pyx":65
  *             return 1
  *         elif self.syn <= NUM_F:
  *             return 2             # <<<<<<<<<<<<<<
  *         else:
  *             return self.syn - CLN + 3
  */
     __pyx_r = 2;
     goto __pyx_L0;
 
-    /* "kola/lexer.pyx":67
+    /* "kola/lexer.pyx":64
  *         elif self.syn == LITERAL:
  *             return 1
  *         elif self.syn <= NUM_F:             # <<<<<<<<<<<<<<
  *             return 2
  *         else:
  */
   }
 
-  /* "kola/lexer.pyx":70
+  /* "kola/lexer.pyx":67
  *             return 2
  *         else:
  *             return self.syn - CLN + 3             # <<<<<<<<<<<<<<
  * 
  *     def __repr__(self):
  */
   /*else*/ {
     __pyx_r = ((__pyx_v_self->syn - CLN) + 3);
     goto __pyx_L0;
   }
 
-  /* "kola/lexer.pyx":62
+  /* "kola/lexer.pyx":59
  *         return self is other or self.syn == other
  * 
  *     cpdef int get_flag(self):             # <<<<<<<<<<<<<<
  *         if self.syn <= TEXT or self.syn == ANNOTATION:
  *             return 0
  */
 
@@ -3717,15 +3751,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("get_flag", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_f_4kola_5lexer_5Token_get_flag(__pyx_v_self, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 62, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_f_4kola_5lexer_5Token_get_flag(__pyx_v_self, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 59, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -3734,15 +3768,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "kola/lexer.pyx":72
+/* "kola/lexer.pyx":69
  *             return self.syn - CLN + 3
  * 
  *     def __repr__(self):             # <<<<<<<<<<<<<<
  *         if self.val is None:
  *             return PyUnicode_FromFormat("<token %d>", self.syn)
  */
 
@@ -3767,65 +3801,65 @@
   int __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__repr__", 0);
 
-  /* "kola/lexer.pyx":73
+  /* "kola/lexer.pyx":70
  * 
  *     def __repr__(self):
  *         if self.val is None:             # <<<<<<<<<<<<<<
  *             return PyUnicode_FromFormat("<token %d>", self.syn)
  *         else:
  */
   __pyx_t_1 = (__pyx_v_self->val == Py_None);
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "kola/lexer.pyx":74
+    /* "kola/lexer.pyx":71
  *     def __repr__(self):
  *         if self.val is None:
  *             return PyUnicode_FromFormat("<token %d>", self.syn)             # <<<<<<<<<<<<<<
  *         else:
  *             return PyUnicode_FromFormat("<token %d: %R>", self.syn, <void*>self.val)
  */
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_3 = PyUnicode_FromFormat(((char const *)"<token %d>"), __pyx_v_self->syn); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 74, __pyx_L1_error)
+    __pyx_t_3 = PyUnicode_FromFormat(((char const *)"<token %d>"), __pyx_v_self->syn); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 71, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_r = __pyx_t_3;
     __pyx_t_3 = 0;
     goto __pyx_L0;
 
-    /* "kola/lexer.pyx":73
+    /* "kola/lexer.pyx":70
  * 
  *     def __repr__(self):
  *         if self.val is None:             # <<<<<<<<<<<<<<
  *             return PyUnicode_FromFormat("<token %d>", self.syn)
  *         else:
  */
   }
 
-  /* "kola/lexer.pyx":76
+  /* "kola/lexer.pyx":73
  *             return PyUnicode_FromFormat("<token %d>", self.syn)
  *         else:
  *             return PyUnicode_FromFormat("<token %d: %R>", self.syn, <void*>self.val)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
-    __pyx_t_3 = PyUnicode_FromFormat(((char const *)"<token %d: %R>"), __pyx_v_self->syn, ((void *)__pyx_v_self->val)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 76, __pyx_L1_error)
+    __pyx_t_3 = PyUnicode_FromFormat(((char const *)"<token %d: %R>"), __pyx_v_self->syn, ((void *)__pyx_v_self->val)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 73, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_r = __pyx_t_3;
     __pyx_t_3 = 0;
     goto __pyx_L0;
   }
 
-  /* "kola/lexer.pyx":72
+  /* "kola/lexer.pyx":69
  *             return self.syn - CLN + 3
  * 
  *     def __repr__(self):             # <<<<<<<<<<<<<<
  *         if self.val is None:
  *             return PyUnicode_FromFormat("<token %d>", self.syn)
  */
 
@@ -3836,15 +3870,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "kola/lexer.pxd":16
+/* "kola/lexer.pxd":12
  *         Token next     # used in grammar parser
  *     cdef readonly:
  *         TokenSyn syn             # <<<<<<<<<<<<<<
  *         object val
  *         bytes raw_val
  */
 
@@ -3867,15 +3901,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_enum__TokenSyn(__pyx_v_self->syn); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 16, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_enum__TokenSyn(__pyx_v_self->syn); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 12, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -3884,15 +3918,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "kola/lexer.pxd":17
+/* "kola/lexer.pxd":13
  *     cdef readonly:
  *         TokenSyn syn
  *         object val             # <<<<<<<<<<<<<<
  *         bytes raw_val
  *         int lineno
  */
 
@@ -3922,15 +3956,15 @@
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "kola/lexer.pxd":18
+/* "kola/lexer.pxd":14
  *         TokenSyn syn
  *         object val
  *         bytes raw_val             # <<<<<<<<<<<<<<
  *         int lineno
  * 
  */
 
@@ -3960,15 +3994,15 @@
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "kola/lexer.pxd":19
+/* "kola/lexer.pxd":15
  *         object val
  *         bytes raw_val
  *         int lineno             # <<<<<<<<<<<<<<
  * 
  *     cpdef int get_flag(self)
  */
 
@@ -3991,15 +4025,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->lineno); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 19, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_self->lineno); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 15, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -4193,15 +4227,15 @@
   __Pyx_AddTraceback("kola.lexer.Token.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "kola/lexer.pyx":84
+/* "kola/lexer.pyx":81
  *     """
  * 
  *     def __init__(self, BaseLexer lexer not None):             # <<<<<<<<<<<<<<
  *         self.lexer = lexer
  *         self.lexer_data = &lexer.lexer_data
  */
 
@@ -4232,37 +4266,37 @@
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
       kw_args = __Pyx_NumKwargs_VARARGS(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_VARARGS(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_lexer)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 84, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 81, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "__init__") < 0)) __PYX_ERR(1, 84, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "__init__") < 0)) __PYX_ERR(1, 81, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_VARARGS(__pyx_args, 0);
     }
     __pyx_v_lexer = ((struct __pyx_obj_4kola_5lexer_BaseLexer *)values[0]);
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__init__", 1, 1, 1, __pyx_nargs); __PYX_ERR(1, 84, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__init__", 1, 1, 1, __pyx_nargs); __PYX_ERR(1, 81, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("kola.lexer.LexerConfig.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_lexer), __pyx_ptype_4kola_5lexer_BaseLexer, 0, "lexer", 0))) __PYX_ERR(1, 84, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_lexer), __pyx_ptype_4kola_5lexer_BaseLexer, 0, "lexer", 0))) __PYX_ERR(1, 81, __pyx_L1_error)
   __pyx_r = __pyx_pf_4kola_5lexer_11LexerConfig___init__(((struct __pyx_obj_4kola_5lexer_LexerConfig *)__pyx_v_self), __pyx_v_lexer);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = -1;
   __pyx_L0:;
@@ -4271,56 +4305,56 @@
 }
 
 static int __pyx_pf_4kola_5lexer_11LexerConfig___init__(struct __pyx_obj_4kola_5lexer_LexerConfig *__pyx_v_self, struct __pyx_obj_4kola_5lexer_BaseLexer *__pyx_v_lexer) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__init__", 0);
 
-  /* "kola/lexer.pyx":85
+  /* "kola/lexer.pyx":82
  * 
  *     def __init__(self, BaseLexer lexer not None):
  *         self.lexer = lexer             # <<<<<<<<<<<<<<
  *         self.lexer_data = &lexer.lexer_data
  * 
  */
   __Pyx_INCREF((PyObject *)__pyx_v_lexer);
   __Pyx_GIVEREF((PyObject *)__pyx_v_lexer);
   __Pyx_GOTREF((PyObject *)__pyx_v_self->lexer);
   __Pyx_DECREF((PyObject *)__pyx_v_self->lexer);
   __pyx_v_self->lexer = __pyx_v_lexer;
 
-  /* "kola/lexer.pyx":86
+  /* "kola/lexer.pyx":83
  *     def __init__(self, BaseLexer lexer not None):
  *         self.lexer = lexer
  *         self.lexer_data = &lexer.lexer_data             # <<<<<<<<<<<<<<
  * 
  *     def dict(self) -> dict:
  */
   __pyx_v_self->lexer_data = (&__pyx_v_lexer->lexer_data);
 
-  /* "kola/lexer.pyx":84
+  /* "kola/lexer.pyx":81
  *     """
  * 
  *     def __init__(self, BaseLexer lexer not None):             # <<<<<<<<<<<<<<
  *         self.lexer = lexer
  *         self.lexer_data = &lexer.lexer_data
  */
 
   /* function exit code */
   __pyx_r = 0;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "kola/lexer.pyx":88
+/* "kola/lexer.pyx":85
  *         self.lexer_data = &lexer.lexer_data
  * 
  *     def dict(self) -> dict:             # <<<<<<<<<<<<<<
- *         cdef dict data = {}
- *         for i in _lexer_data_names:
+ *         cdef dict data = <dict>self.lexer_data[0]
+ *         data["filename"] = (<bytes>data["filename"]).decode()
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_4kola_5lexer_11LexerConfig_3dict(PyObject *__pyx_v_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
@@ -4350,115 +4384,121 @@
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 static PyObject *__pyx_pf_4kola_5lexer_11LexerConfig_2dict(struct __pyx_obj_4kola_5lexer_LexerConfig *__pyx_v_self) {
   PyObject *__pyx_v_data = 0;
-  PyObject *__pyx_v_i = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
-  Py_ssize_t __pyx_t_2;
-  Py_ssize_t __pyx_t_3;
-  int __pyx_t_4;
-  PyObject *__pyx_t_5 = NULL;
-  int __pyx_t_6;
+  PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("dict", 0);
 
-  /* "kola/lexer.pyx":89
+  /* "kola/lexer.pyx":86
  * 
  *     def dict(self) -> dict:
- *         cdef dict data = {}             # <<<<<<<<<<<<<<
- *         for i in _lexer_data_names:
- *             data[i] = getattr(self, <str>i)
+ *         cdef dict data = <dict>self.lexer_data[0]             # <<<<<<<<<<<<<<
+ *         data["filename"] = (<bytes>data["filename"]).decode()
+ *         data["encoding"] = self.lexer.encoding
  */
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 89, __pyx_L1_error)
+  __pyx_t_1 = __pyx_convert__to_py_LexerData((__pyx_v_self->lexer_data[0])); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 86, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_v_data = ((PyObject*)__pyx_t_1);
-  __pyx_t_1 = 0;
+  if (!(likely(PyDict_CheckExact(__pyx_t_1)) || __Pyx_RaiseUnexpectedTypeError("dict", __pyx_t_1))) __PYX_ERR(1, 86, __pyx_L1_error)
+  __pyx_t_2 = __pyx_t_1;
+  __Pyx_INCREF(__pyx_t_2);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_v_data = ((PyObject*)__pyx_t_2);
+  __pyx_t_2 = 0;
 
-  /* "kola/lexer.pyx":90
+  /* "kola/lexer.pyx":87
  *     def dict(self) -> dict:
- *         cdef dict data = {}
- *         for i in _lexer_data_names:             # <<<<<<<<<<<<<<
- *             data[i] = getattr(self, <str>i)
+ *         cdef dict data = <dict>self.lexer_data[0]
+ *         data["filename"] = (<bytes>data["filename"]).decode()             # <<<<<<<<<<<<<<
+ *         data["encoding"] = self.lexer.encoding
  *         return data
  */
-  __pyx_t_2 = 0;
-  __pyx_t_5 = __Pyx_set_iterator(__pyx_v_4kola_5lexer__lexer_data_names, 1, (&__pyx_t_3), (&__pyx_t_4)); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 90, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_5);
-  __Pyx_XDECREF(__pyx_t_1);
-  __pyx_t_1 = __pyx_t_5;
-  __pyx_t_5 = 0;
-  while (1) {
-    __pyx_t_6 = __Pyx_set_iter_next(__pyx_t_1, __pyx_t_3, &__pyx_t_2, &__pyx_t_5, __pyx_t_4);
-    if (unlikely(__pyx_t_6 == 0)) break;
-    if (unlikely(__pyx_t_6 == -1)) __PYX_ERR(1, 90, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_5);
-    __Pyx_XDECREF_SET(__pyx_v_i, __pyx_t_5);
-    __pyx_t_5 = 0;
+  if (unlikely(__pyx_v_data == Py_None)) {
+    PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
+    __PYX_ERR(1, 87, __pyx_L1_error)
+  }
+  __pyx_t_2 = __Pyx_PyDict_GetItem(__pyx_v_data, __pyx_n_u_filename); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 87, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (unlikely(__pyx_t_2 == Py_None)) {
+    PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "decode");
+    __PYX_ERR(1, 87, __pyx_L1_error)
+  }
+  __pyx_t_1 = __Pyx_decode_bytes(((PyObject*)__pyx_t_2), 0, PY_SSIZE_T_MAX, NULL, NULL, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 87, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  if (unlikely(__pyx_v_data == Py_None)) {
+    PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
+    __PYX_ERR(1, 87, __pyx_L1_error)
+  }
+  if (unlikely((PyDict_SetItem(__pyx_v_data, __pyx_n_u_filename, __pyx_t_1) < 0))) __PYX_ERR(1, 87, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-    /* "kola/lexer.pyx":91
- *         cdef dict data = {}
- *         for i in _lexer_data_names:
- *             data[i] = getattr(self, <str>i)             # <<<<<<<<<<<<<<
+  /* "kola/lexer.pyx":88
+ *         cdef dict data = <dict>self.lexer_data[0]
+ *         data["filename"] = (<bytes>data["filename"]).decode()
+ *         data["encoding"] = self.lexer.encoding             # <<<<<<<<<<<<<<
  *         return data
  * 
  */
-    __pyx_t_5 = __Pyx_GetAttr(((PyObject *)__pyx_v_self), __pyx_v_i); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 91, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_5);
-    if (unlikely((PyDict_SetItem(__pyx_v_data, __pyx_v_i, __pyx_t_5) < 0))) __PYX_ERR(1, 91, __pyx_L1_error)
-    __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+  __pyx_t_1 = __pyx_v_self->lexer->encoding;
+  __Pyx_INCREF(__pyx_t_1);
+  if (unlikely(__pyx_v_data == Py_None)) {
+    PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
+    __PYX_ERR(1, 88, __pyx_L1_error)
   }
+  if (unlikely((PyDict_SetItem(__pyx_v_data, __pyx_n_u_encoding, __pyx_t_1) < 0))) __PYX_ERR(1, 88, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "kola/lexer.pyx":92
- *         for i in _lexer_data_names:
- *             data[i] = getattr(self, <str>i)
+  /* "kola/lexer.pyx":89
+ *         data["filename"] = (<bytes>data["filename"]).decode()
+ *         data["encoding"] = self.lexer.encoding
  *         return data             # <<<<<<<<<<<<<<
  * 
  *     def set(self, **kwds) -> None:
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_data);
   __pyx_r = __pyx_v_data;
   goto __pyx_L0;
 
-  /* "kola/lexer.pyx":88
+  /* "kola/lexer.pyx":85
  *         self.lexer_data = &lexer.lexer_data
  * 
  *     def dict(self) -> dict:             # <<<<<<<<<<<<<<
- *         cdef dict data = {}
- *         for i in _lexer_data_names:
+ *         cdef dict data = <dict>self.lexer_data[0]
+ *         data["filename"] = (<bytes>data["filename"]).decode()
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_XDECREF(__pyx_t_2);
   __Pyx_AddTraceback("kola.lexer.LexerConfig.dict", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_data);
-  __Pyx_XDECREF(__pyx_v_i);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "kola/lexer.pyx":94
+/* "kola/lexer.pyx":91
  *         return data
  * 
  *     def set(self, **kwds) -> None:             # <<<<<<<<<<<<<<
  *         for k, v in kwds.items():
- *             if not k in _lexer_data_names:
+ *             if k.startswith('__') and k.endswith('__'):
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_4kola_5lexer_11LexerConfig_5set(PyObject *__pyx_v_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
@@ -4510,116 +4550,167 @@
   Py_ssize_t __pyx_t_2;
   Py_ssize_t __pyx_t_3;
   int __pyx_t_4;
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   int __pyx_t_7;
   int __pyx_t_8;
-  int __pyx_t_9;
-  PyObject *__pyx_t_10;
-  int __pyx_t_11;
+  PyObject *__pyx_t_9 = NULL;
+  int __pyx_t_10;
+  PyObject *__pyx_t_11;
+  int __pyx_t_12;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("set", 0);
 
-  /* "kola/lexer.pyx":95
+  /* "kola/lexer.pyx":92
  * 
  *     def set(self, **kwds) -> None:
  *         for k, v in kwds.items():             # <<<<<<<<<<<<<<
- *             if not k in _lexer_data_names:
+ *             if k.startswith('__') and k.endswith('__'):
  *                 PyErr_Format(AttributeError, "invalid config item '%U'", <void*>k)
  */
   __pyx_t_2 = 0;
-  __pyx_t_5 = __Pyx_dict_iterator(__pyx_v_kwds, 1, __pyx_n_s_items, (&__pyx_t_3), (&__pyx_t_4)); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 95, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_dict_iterator(__pyx_v_kwds, 1, __pyx_n_s_items, (&__pyx_t_3), (&__pyx_t_4)); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 92, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_XDECREF(__pyx_t_1);
   __pyx_t_1 = __pyx_t_5;
   __pyx_t_5 = 0;
   while (1) {
     __pyx_t_7 = __Pyx_dict_iter_next(__pyx_t_1, __pyx_t_3, &__pyx_t_2, &__pyx_t_5, &__pyx_t_6, NULL, __pyx_t_4);
     if (unlikely(__pyx_t_7 == 0)) break;
-    if (unlikely(__pyx_t_7 == -1)) __PYX_ERR(1, 95, __pyx_L1_error)
+    if (unlikely(__pyx_t_7 == -1)) __PYX_ERR(1, 92, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_5);
     __Pyx_GOTREF(__pyx_t_6);
     __Pyx_XDECREF_SET(__pyx_v_k, __pyx_t_5);
     __pyx_t_5 = 0;
     __Pyx_XDECREF_SET(__pyx_v_v, __pyx_t_6);
     __pyx_t_6 = 0;
 
-    /* "kola/lexer.pyx":96
+    /* "kola/lexer.pyx":93
  *     def set(self, **kwds) -> None:
  *         for k, v in kwds.items():
- *             if not k in _lexer_data_names:             # <<<<<<<<<<<<<<
+ *             if k.startswith('__') and k.endswith('__'):             # <<<<<<<<<<<<<<
  *                 PyErr_Format(AttributeError, "invalid config item '%U'", <void*>k)
  *             setattr(self, k, v)
  */
-    if (unlikely(__pyx_v_4kola_5lexer__lexer_data_names == Py_None)) {
-      PyErr_SetString(PyExc_TypeError, "'NoneType' object is not iterable");
-      __PYX_ERR(1, 96, __pyx_L1_error)
-    }
-    __pyx_t_8 = (__Pyx_PySet_ContainsTF(__pyx_v_k, __pyx_v_4kola_5lexer__lexer_data_names, Py_NE)); if (unlikely((__pyx_t_8 < 0))) __PYX_ERR(1, 96, __pyx_L1_error)
-    __pyx_t_9 = (__pyx_t_8 != 0);
-    if (__pyx_t_9) {
+    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_k, __pyx_n_s_startswith); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 93, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __pyx_t_9 = NULL;
+    __pyx_t_7 = 0;
+    if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_5))) {
+      __pyx_t_9 = PyMethod_GET_SELF(__pyx_t_5);
+      if (likely(__pyx_t_9)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
+        __Pyx_INCREF(__pyx_t_9);
+        __Pyx_INCREF(function);
+        __Pyx_DECREF_SET(__pyx_t_5, function);
+        __pyx_t_7 = 1;
+      }
+    }
+    {
+      PyObject *__pyx_callargs[2] = {__pyx_t_9, __pyx_n_u_};
+      __pyx_t_6 = __Pyx_PyObject_FastCall(__pyx_t_5, __pyx_callargs+1-__pyx_t_7, 1+__pyx_t_7);
+      __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
+      if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 93, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_6);
+      __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    }
+    __pyx_t_10 = __Pyx_PyObject_IsTrue(__pyx_t_6); if (unlikely((__pyx_t_10 < 0))) __PYX_ERR(1, 93, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+    if (__pyx_t_10) {
+    } else {
+      __pyx_t_8 = __pyx_t_10;
+      goto __pyx_L6_bool_binop_done;
+    }
+    __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_v_k, __pyx_n_s_endswith); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 93, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
+    __pyx_t_9 = NULL;
+    __pyx_t_7 = 0;
+    if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_5))) {
+      __pyx_t_9 = PyMethod_GET_SELF(__pyx_t_5);
+      if (likely(__pyx_t_9)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_5);
+        __Pyx_INCREF(__pyx_t_9);
+        __Pyx_INCREF(function);
+        __Pyx_DECREF_SET(__pyx_t_5, function);
+        __pyx_t_7 = 1;
+      }
+    }
+    {
+      PyObject *__pyx_callargs[2] = {__pyx_t_9, __pyx_n_u_};
+      __pyx_t_6 = __Pyx_PyObject_FastCall(__pyx_t_5, __pyx_callargs+1-__pyx_t_7, 1+__pyx_t_7);
+      __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
+      if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 93, __pyx_L1_error)
+      __Pyx_GOTREF(__pyx_t_6);
+      __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
+    }
+    __pyx_t_10 = __Pyx_PyObject_IsTrue(__pyx_t_6); if (unlikely((__pyx_t_10 < 0))) __PYX_ERR(1, 93, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __pyx_t_8 = __pyx_t_10;
+    __pyx_L6_bool_binop_done:;
+    if (__pyx_t_8) {
 
-      /* "kola/lexer.pyx":97
+      /* "kola/lexer.pyx":94
  *         for k, v in kwds.items():
- *             if not k in _lexer_data_names:
+ *             if k.startswith('__') and k.endswith('__'):
  *                 PyErr_Format(AttributeError, "invalid config item '%U'", <void*>k)             # <<<<<<<<<<<<<<
  *             setattr(self, k, v)
  * 
  */
-      __pyx_t_10 = PyErr_Format(__pyx_builtin_AttributeError, ((char *)"invalid config item '%U'"), ((void *)__pyx_v_k)); if (unlikely(__pyx_t_10 == ((PyObject *)NULL))) __PYX_ERR(1, 97, __pyx_L1_error)
+      __pyx_t_11 = PyErr_Format(__pyx_builtin_AttributeError, ((char *)"invalid config item '%U'"), ((void *)__pyx_v_k)); if (unlikely(__pyx_t_11 == ((PyObject *)NULL))) __PYX_ERR(1, 94, __pyx_L1_error)
 
-      /* "kola/lexer.pyx":96
+      /* "kola/lexer.pyx":93
  *     def set(self, **kwds) -> None:
  *         for k, v in kwds.items():
- *             if not k in _lexer_data_names:             # <<<<<<<<<<<<<<
+ *             if k.startswith('__') and k.endswith('__'):             # <<<<<<<<<<<<<<
  *                 PyErr_Format(AttributeError, "invalid config item '%U'", <void*>k)
  *             setattr(self, k, v)
  */
     }
 
-    /* "kola/lexer.pyx":98
- *             if not k in _lexer_data_names:
+    /* "kola/lexer.pyx":95
+ *             if k.startswith('__') and k.endswith('__'):
  *                 PyErr_Format(AttributeError, "invalid config item '%U'", <void*>k)
  *             setattr(self, k, v)             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
-    __pyx_t_11 = PyObject_SetAttr(((PyObject *)__pyx_v_self), __pyx_v_k, __pyx_v_v); if (unlikely(__pyx_t_11 == ((int)-1))) __PYX_ERR(1, 98, __pyx_L1_error)
+    __pyx_t_12 = PyObject_SetAttr(((PyObject *)__pyx_v_self), __pyx_v_k, __pyx_v_v); if (unlikely(__pyx_t_12 == ((int)-1))) __PYX_ERR(1, 95, __pyx_L1_error)
   }
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "kola/lexer.pyx":94
+  /* "kola/lexer.pyx":91
  *         return data
  * 
  *     def set(self, **kwds) -> None:             # <<<<<<<<<<<<<<
  *         for k, v in kwds.items():
- *             if not k in _lexer_data_names:
+ *             if k.startswith('__') and k.endswith('__'):
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_5);
   __Pyx_XDECREF(__pyx_t_6);
+  __Pyx_XDECREF(__pyx_t_9);
   __Pyx_AddTraceback("kola.lexer.LexerConfig.set", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_k);
   __Pyx_XDECREF(__pyx_v_v);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "kola/lexer.pyx":100
+/* "kola/lexer.pyx":97
  *             setattr(self, k, v)
  * 
  *     @property             # <<<<<<<<<<<<<<
  *     def filename(self) -> str:
  *         return self.lexer_data.filename.decode()
  */
 
@@ -4643,31 +4734,31 @@
   char const *__pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "kola/lexer.pyx":102
+  /* "kola/lexer.pyx":99
  *     @property
  *     def filename(self) -> str:
  *         return self.lexer_data.filename.decode()             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = __pyx_v_self->lexer_data->filename;
-  __pyx_t_2 = __Pyx_decode_c_string(__pyx_t_1, 0, strlen(__pyx_t_1), NULL, NULL, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 102, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_decode_c_string(__pyx_t_1, 0, strlen(__pyx_t_1), NULL, NULL, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 99, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_INCREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "kola/lexer.pyx":100
+  /* "kola/lexer.pyx":97
  *             setattr(self, k, v)
  * 
  *     @property             # <<<<<<<<<<<<<<
  *     def filename(self) -> str:
  *         return self.lexer_data.filename.decode()
  */
 
@@ -4678,15 +4769,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "kola/lexer.pyx":104
+/* "kola/lexer.pyx":101
  *         return self.lexer_data.filename.decode()
  * 
  *     @property             # <<<<<<<<<<<<<<
  *     def encoding(self) -> str:
  *         return self.lexer.encoding
  */
 
@@ -4705,42 +4796,42 @@
 }
 
 static PyObject *__pyx_pf_4kola_5lexer_11LexerConfig_8encoding___get__(struct __pyx_obj_4kola_5lexer_LexerConfig *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "kola/lexer.pyx":106
+  /* "kola/lexer.pyx":103
  *     @property
  *     def encoding(self) -> str:
  *         return self.lexer.encoding             # <<<<<<<<<<<<<<
  * 
  *     @encoding.setter
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_self->lexer->encoding);
   __pyx_r = __pyx_v_self->lexer->encoding;
   goto __pyx_L0;
 
-  /* "kola/lexer.pyx":104
+  /* "kola/lexer.pyx":101
  *         return self.lexer_data.filename.decode()
  * 
  *     @property             # <<<<<<<<<<<<<<
  *     def encoding(self) -> str:
  *         return self.lexer.encoding
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "kola/lexer.pyx":108
+/* "kola/lexer.pyx":105
  *         return self.lexer.encoding
  * 
  *     @encoding.setter             # <<<<<<<<<<<<<<
  *     def encoding(self, val: str) -> None:
  *         self.lexer.encoding = val
  */
 
@@ -4750,15 +4841,15 @@
   CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__set__ (wrapper)", 0);
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_val), (&PyUnicode_Type), 1, "val", 1))) __PYX_ERR(1, 109, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_val), (&PyUnicode_Type), 1, "val", 1))) __PYX_ERR(1, 106, __pyx_L1_error)
   __pyx_r = __pyx_pf_4kola_5lexer_11LexerConfig_8encoding_2__set__(((struct __pyx_obj_4kola_5lexer_LexerConfig *)__pyx_v_self), ((PyObject*)__pyx_v_val));
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = -1;
   __pyx_L0:;
@@ -4767,42 +4858,42 @@
 }
 
 static int __pyx_pf_4kola_5lexer_11LexerConfig_8encoding_2__set__(struct __pyx_obj_4kola_5lexer_LexerConfig *__pyx_v_self, PyObject *__pyx_v_val) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__set__", 0);
 
-  /* "kola/lexer.pyx":110
+  /* "kola/lexer.pyx":107
  *     @encoding.setter
  *     def encoding(self, val: str) -> None:
  *         self.lexer.encoding = val             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
   __Pyx_INCREF(__pyx_v_val);
   __Pyx_GIVEREF(__pyx_v_val);
   __Pyx_GOTREF(__pyx_v_self->lexer->encoding);
   __Pyx_DECREF(__pyx_v_self->lexer->encoding);
   __pyx_v_self->lexer->encoding = __pyx_v_val;
 
-  /* "kola/lexer.pyx":108
+  /* "kola/lexer.pyx":105
  *         return self.lexer.encoding
  * 
  *     @encoding.setter             # <<<<<<<<<<<<<<
  *     def encoding(self, val: str) -> None:
  *         self.lexer.encoding = val
  */
 
   /* function exit code */
   __pyx_r = 0;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "kola/lexer.pyx":112
+/* "kola/lexer.pyx":109
  *         self.lexer.encoding = val
  * 
  *     @property             # <<<<<<<<<<<<<<
  *     def command_threshold(self) -> int:
  *         return self.lexer_data.command_threshold
  */
 
@@ -4825,29 +4916,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "kola/lexer.pyx":114
+  /* "kola/lexer.pyx":111
  *     @property
  *     def command_threshold(self) -> int:
  *         return self.lexer_data.command_threshold             # <<<<<<<<<<<<<<
  * 
  *     @command_threshold.setter
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_uint8_t(__pyx_v_self->lexer_data->command_threshold); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 114, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_uint8_t(__pyx_v_self->lexer_data->command_threshold); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 111, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "kola/lexer.pyx":112
+  /* "kola/lexer.pyx":109
  *         self.lexer.encoding = val
  * 
  *     @property             # <<<<<<<<<<<<<<
  *     def command_threshold(self) -> int:
  *         return self.lexer_data.command_threshold
  */
 
@@ -4858,15 +4949,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "kola/lexer.pyx":116
+/* "kola/lexer.pyx":113
  *         return self.lexer_data.command_threshold
  * 
  *     @command_threshold.setter             # <<<<<<<<<<<<<<
  *     def command_threshold(self, uint8_t cmd_threshold) -> None:
  *         self.lexer_data.command_threshold = cmd_threshold
  */
 
@@ -4878,15 +4969,15 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__set__ (wrapper)", 0);
   assert(__pyx_arg_cmd_threshold); {
-    __pyx_v_cmd_threshold = __Pyx_PyInt_As_uint8_t(__pyx_arg_cmd_threshold); if (unlikely((__pyx_v_cmd_threshold == ((uint8_t)-1)) && PyErr_Occurred())) __PYX_ERR(1, 117, __pyx_L3_error)
+    __pyx_v_cmd_threshold = __Pyx_PyInt_As_uint8_t(__pyx_arg_cmd_threshold); if (unlikely((__pyx_v_cmd_threshold == ((uint8_t)-1)) && PyErr_Occurred())) __PYX_ERR(1, 114, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   __Pyx_AddTraceback("kola.lexer.LexerConfig.command_threshold.__set__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
@@ -4898,38 +4989,38 @@
 }
 
 static int __pyx_pf_4kola_5lexer_11LexerConfig_17command_threshold_2__set__(struct __pyx_obj_4kola_5lexer_LexerConfig *__pyx_v_self, uint8_t __pyx_v_cmd_threshold) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__set__", 0);
 
-  /* "kola/lexer.pyx":118
+  /* "kola/lexer.pyx":115
  *     @command_threshold.setter
  *     def command_threshold(self, uint8_t cmd_threshold) -> None:
  *         self.lexer_data.command_threshold = cmd_threshold             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
   __pyx_v_self->lexer_data->command_threshold = __pyx_v_cmd_threshold;
 
-  /* "kola/lexer.pyx":116
+  /* "kola/lexer.pyx":113
  *         return self.lexer_data.command_threshold
  * 
  *     @command_threshold.setter             # <<<<<<<<<<<<<<
  *     def command_threshold(self, uint8_t cmd_threshold) -> None:
  *         self.lexer_data.command_threshold = cmd_threshold
  */
 
   /* function exit code */
   __pyx_r = 0;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "kola/lexer.pyx":120
+/* "kola/lexer.pyx":117
  *         self.lexer_data.command_threshold = cmd_threshold
  * 
  *     @property             # <<<<<<<<<<<<<<
  *     def flag(self) -> int:
  *         return self.lexer_data.flag
  */
 
@@ -4952,29 +5043,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "kola/lexer.pyx":122
+  /* "kola/lexer.pyx":119
  *     @property
  *     def flag(self) -> int:
  *         return self.lexer_data.flag             # <<<<<<<<<<<<<<
  * 
  *     @flag.setter
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_uint8_t(__pyx_v_self->lexer_data->flag); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 122, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_uint8_t(__pyx_v_self->lexer_data->flag); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 119, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "kola/lexer.pyx":120
+  /* "kola/lexer.pyx":117
  *         self.lexer_data.command_threshold = cmd_threshold
  * 
  *     @property             # <<<<<<<<<<<<<<
  *     def flag(self) -> int:
  *         return self.lexer_data.flag
  */
 
@@ -4985,15 +5076,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "kola/lexer.pyx":124
+/* "kola/lexer.pyx":121
  *         return self.lexer_data.flag
  * 
  *     @flag.setter             # <<<<<<<<<<<<<<
  *     def flag(self, uint8_t val) -> None:
  *         self.lexer_data.flag = val
  */
 
@@ -5005,15 +5096,15 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__set__ (wrapper)", 0);
   assert(__pyx_arg_val); {
-    __pyx_v_val = __Pyx_PyInt_As_uint8_t(__pyx_arg_val); if (unlikely((__pyx_v_val == ((uint8_t)-1)) && PyErr_Occurred())) __PYX_ERR(1, 125, __pyx_L3_error)
+    __pyx_v_val = __Pyx_PyInt_As_uint8_t(__pyx_arg_val); if (unlikely((__pyx_v_val == ((uint8_t)-1)) && PyErr_Occurred())) __PYX_ERR(1, 122, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L3_error:;
   __Pyx_AddTraceback("kola.lexer.LexerConfig.flag.__set__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
@@ -5025,38 +5116,38 @@
 }
 
 static int __pyx_pf_4kola_5lexer_11LexerConfig_4flag_2__set__(struct __pyx_obj_4kola_5lexer_LexerConfig *__pyx_v_self, uint8_t __pyx_v_val) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__set__", 0);
 
-  /* "kola/lexer.pyx":126
+  /* "kola/lexer.pyx":123
  *     @flag.setter
  *     def flag(self, uint8_t val) -> None:
  *         self.lexer_data.flag = val             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
   __pyx_v_self->lexer_data->flag = __pyx_v_val;
 
-  /* "kola/lexer.pyx":124
+  /* "kola/lexer.pyx":121
  *         return self.lexer_data.flag
  * 
  *     @flag.setter             # <<<<<<<<<<<<<<
  *     def flag(self, uint8_t val) -> None:
  *         self.lexer_data.flag = val
  */
 
   /* function exit code */
   __pyx_r = 0;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "kola/lexer.pyx":128
+/* "kola/lexer.pyx":125
  *         self.lexer_data.flag = val
  * 
  *     @property             # <<<<<<<<<<<<<<
  *     def disabled(self) -> bool:
  *         return True if self.lexer_data.flag & LFLAG_DISABLED else False
  */
 
@@ -5076,15 +5167,15 @@
 
 static PyObject *__pyx_pf_4kola_5lexer_11LexerConfig_8disabled___get__(struct __pyx_obj_4kola_5lexer_LexerConfig *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "kola/lexer.pyx":130
+  /* "kola/lexer.pyx":127
  *     @property
  *     def disabled(self) -> bool:
  *         return True if self.lexer_data.flag & LFLAG_DISABLED else False             # <<<<<<<<<<<<<<
  * 
  *     @disabled.setter
  */
   __Pyx_XDECREF(__pyx_r);
@@ -5095,30 +5186,30 @@
     __Pyx_INCREF(Py_False);
     __pyx_t_1 = Py_False;
   }
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "kola/lexer.pyx":128
+  /* "kola/lexer.pyx":125
  *         self.lexer_data.flag = val
  * 
  *     @property             # <<<<<<<<<<<<<<
  *     def disabled(self) -> bool:
  *         return True if self.lexer_data.flag & LFLAG_DISABLED else False
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "kola/lexer.pyx":132
+/* "kola/lexer.pyx":129
  *         return True if self.lexer_data.flag & LFLAG_DISABLED else False
  * 
  *     @disabled.setter             # <<<<<<<<<<<<<<
  *     def disabled(self, val: bool) -> None:
  *         if val:
  */
 
@@ -5141,56 +5232,56 @@
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__set__", 0);
 
-  /* "kola/lexer.pyx":134
+  /* "kola/lexer.pyx":131
  *     @disabled.setter
  *     def disabled(self, val: bool) -> None:
  *         if val:             # <<<<<<<<<<<<<<
  *             self.lexer_data.flag |= LFLAG_DISABLED
  *         else:
  */
-  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_val); if (unlikely((__pyx_t_1 < 0))) __PYX_ERR(1, 134, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_val); if (unlikely((__pyx_t_1 < 0))) __PYX_ERR(1, 131, __pyx_L1_error)
   if (__pyx_t_1) {
 
-    /* "kola/lexer.pyx":135
+    /* "kola/lexer.pyx":132
  *     def disabled(self, val: bool) -> None:
  *         if val:
  *             self.lexer_data.flag |= LFLAG_DISABLED             # <<<<<<<<<<<<<<
  *         else:
  *             self.lexer_data.flag &= ~LFLAG_DISABLED
  */
     __pyx_v_self->lexer_data->flag = (__pyx_v_self->lexer_data->flag | LFLAG_DISABLED);
 
-    /* "kola/lexer.pyx":134
+    /* "kola/lexer.pyx":131
  *     @disabled.setter
  *     def disabled(self, val: bool) -> None:
  *         if val:             # <<<<<<<<<<<<<<
  *             self.lexer_data.flag |= LFLAG_DISABLED
  *         else:
  */
     goto __pyx_L3;
   }
 
-  /* "kola/lexer.pyx":137
+  /* "kola/lexer.pyx":134
  *             self.lexer_data.flag |= LFLAG_DISABLED
  *         else:
  *             self.lexer_data.flag &= ~LFLAG_DISABLED             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
   /*else*/ {
     __pyx_v_self->lexer_data->flag = (__pyx_v_self->lexer_data->flag & (~LFLAG_DISABLED));
   }
   __pyx_L3:;
 
-  /* "kola/lexer.pyx":132
+  /* "kola/lexer.pyx":129
  *         return True if self.lexer_data.flag & LFLAG_DISABLED else False
  * 
  *     @disabled.setter             # <<<<<<<<<<<<<<
  *     def disabled(self, val: bool) -> None:
  *         if val:
  */
 
@@ -5201,15 +5292,15 @@
   __Pyx_AddTraceback("kola.lexer.LexerConfig.disabled.__set__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "kola/lexer.pyx":139
+/* "kola/lexer.pyx":136
  *             self.lexer_data.flag &= ~LFLAG_DISABLED
  * 
  *     @property             # <<<<<<<<<<<<<<
  *     def no_lstrip(self) -> bool:
  *         return True if self.lexer_data.flag & LFLAG_NOLSTRIP else False
  */
 
@@ -5229,15 +5320,15 @@
 
 static PyObject *__pyx_pf_4kola_5lexer_11LexerConfig_9no_lstrip___get__(struct __pyx_obj_4kola_5lexer_LexerConfig *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "kola/lexer.pyx":141
+  /* "kola/lexer.pyx":138
  *     @property
  *     def no_lstrip(self) -> bool:
  *         return True if self.lexer_data.flag & LFLAG_NOLSTRIP else False             # <<<<<<<<<<<<<<
  * 
  *     @no_lstrip.setter
  */
   __Pyx_XDECREF(__pyx_r);
@@ -5248,30 +5339,30 @@
     __Pyx_INCREF(Py_False);
     __pyx_t_1 = Py_False;
   }
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "kola/lexer.pyx":139
+  /* "kola/lexer.pyx":136
  *             self.lexer_data.flag &= ~LFLAG_DISABLED
  * 
  *     @property             # <<<<<<<<<<<<<<
  *     def no_lstrip(self) -> bool:
  *         return True if self.lexer_data.flag & LFLAG_NOLSTRIP else False
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "kola/lexer.pyx":143
+/* "kola/lexer.pyx":140
  *         return True if self.lexer_data.flag & LFLAG_NOLSTRIP else False
  * 
  *     @no_lstrip.setter             # <<<<<<<<<<<<<<
  *     def no_lstrip(self, val: bool) -> None:
  *         if val:
  */
 
@@ -5294,56 +5385,56 @@
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__set__", 0);
 
-  /* "kola/lexer.pyx":145
+  /* "kola/lexer.pyx":142
  *     @no_lstrip.setter
  *     def no_lstrip(self, val: bool) -> None:
  *         if val:             # <<<<<<<<<<<<<<
  *             self.lexer_data.flag |= LFLAG_NOLSTRIP
  *         else:
  */
-  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_val); if (unlikely((__pyx_t_1 < 0))) __PYX_ERR(1, 145, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_val); if (unlikely((__pyx_t_1 < 0))) __PYX_ERR(1, 142, __pyx_L1_error)
   if (__pyx_t_1) {
 
-    /* "kola/lexer.pyx":146
+    /* "kola/lexer.pyx":143
  *     def no_lstrip(self, val: bool) -> None:
  *         if val:
  *             self.lexer_data.flag |= LFLAG_NOLSTRIP             # <<<<<<<<<<<<<<
  *         else:
  *             self.lexer_data.flag &= ~LFLAG_NOLSTRIP
  */
     __pyx_v_self->lexer_data->flag = (__pyx_v_self->lexer_data->flag | LFLAG_NOLSTRIP);
 
-    /* "kola/lexer.pyx":145
+    /* "kola/lexer.pyx":142
  *     @no_lstrip.setter
  *     def no_lstrip(self, val: bool) -> None:
  *         if val:             # <<<<<<<<<<<<<<
  *             self.lexer_data.flag |= LFLAG_NOLSTRIP
  *         else:
  */
     goto __pyx_L3;
   }
 
-  /* "kola/lexer.pyx":148
+  /* "kola/lexer.pyx":145
  *             self.lexer_data.flag |= LFLAG_NOLSTRIP
  *         else:
  *             self.lexer_data.flag &= ~LFLAG_NOLSTRIP             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __pyx_v_self->lexer_data->flag = (__pyx_v_self->lexer_data->flag & (~LFLAG_NOLSTRIP));
   }
   __pyx_L3:;
 
-  /* "kola/lexer.pyx":143
+  /* "kola/lexer.pyx":140
  *         return True if self.lexer_data.flag & LFLAG_NOLSTRIP else False
  * 
  *     @no_lstrip.setter             # <<<<<<<<<<<<<<
  *     def no_lstrip(self, val: bool) -> None:
  *         if val:
  */
 
@@ -5354,15 +5445,15 @@
   __Pyx_AddTraceback("kola.lexer.LexerConfig.no_lstrip.__set__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "kola/lexer.pxd":26
+/* "kola/lexer.pxd":22
  * cdef class LexerConfig:
  *     cdef LexerData* lexer_data
  *     cdef readonly BaseLexer lexer             # <<<<<<<<<<<<<<
  * 
  * 
  */
 
@@ -5577,15 +5668,15 @@
   __Pyx_AddTraceback("kola.lexer.LexerConfig.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "kola/lexer.pyx":166
+/* "kola/lexer.pyx":153
  *     """
  * 
  *     def __cinit__(self, *args, **kwds):             # <<<<<<<<<<<<<<
  *         self.encoding = "utf-8"
  *         self.lexer_data.filename = "<unknown>"
  */
 
@@ -5617,74 +5708,74 @@
   int __pyx_t_1;
   PyObject *__pyx_t_2;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__cinit__", 0);
 
-  /* "kola/lexer.pyx":167
+  /* "kola/lexer.pyx":154
  * 
  *     def __cinit__(self, *args, **kwds):
  *         self.encoding = "utf-8"             # <<<<<<<<<<<<<<
  *         self.lexer_data.filename = "<unknown>"
  *         self.lexer_data.command_threshold = 1
  */
   __Pyx_INCREF(__pyx_kp_u_utf_8);
   __Pyx_GIVEREF(__pyx_kp_u_utf_8);
   __Pyx_GOTREF(__pyx_v_self->encoding);
   __Pyx_DECREF(__pyx_v_self->encoding);
   __pyx_v_self->encoding = __pyx_kp_u_utf_8;
 
-  /* "kola/lexer.pyx":168
+  /* "kola/lexer.pyx":155
  *     def __cinit__(self, *args, **kwds):
  *         self.encoding = "utf-8"
  *         self.lexer_data.filename = "<unknown>"             # <<<<<<<<<<<<<<
  *         self.lexer_data.command_threshold = 1
  *         if yylex_init_extra(&self.lexer_data, &self.scanner):
  */
   __pyx_v_self->lexer_data.filename = ((char const *)"<unknown>");
 
-  /* "kola/lexer.pyx":169
+  /* "kola/lexer.pyx":156
  *         self.encoding = "utf-8"
  *         self.lexer_data.filename = "<unknown>"
  *         self.lexer_data.command_threshold = 1             # <<<<<<<<<<<<<<
  *         if yylex_init_extra(&self.lexer_data, &self.scanner):
  *             PyErr_SetFromErrno(RuntimeError)
  */
   __pyx_v_self->lexer_data.command_threshold = 1;
 
-  /* "kola/lexer.pyx":170
+  /* "kola/lexer.pyx":157
  *         self.lexer_data.filename = "<unknown>"
  *         self.lexer_data.command_threshold = 1
  *         if yylex_init_extra(&self.lexer_data, &self.scanner):             # <<<<<<<<<<<<<<
  *             PyErr_SetFromErrno(RuntimeError)
  * 
  */
   __pyx_t_1 = (yylex_init_extra((&__pyx_v_self->lexer_data), (&__pyx_v_self->scanner)) != 0);
   if (__pyx_t_1) {
 
-    /* "kola/lexer.pyx":171
+    /* "kola/lexer.pyx":158
  *         self.lexer_data.command_threshold = 1
  *         if yylex_init_extra(&self.lexer_data, &self.scanner):
  *             PyErr_SetFromErrno(RuntimeError)             # <<<<<<<<<<<<<<
  * 
  *     def __init__(self, **kwds):
  */
-    __pyx_t_2 = PyErr_SetFromErrno(__pyx_builtin_RuntimeError); if (unlikely(__pyx_t_2 == ((PyObject *)NULL))) __PYX_ERR(1, 171, __pyx_L1_error)
+    __pyx_t_2 = PyErr_SetFromErrno(__pyx_builtin_RuntimeError); if (unlikely(__pyx_t_2 == ((PyObject *)NULL))) __PYX_ERR(1, 158, __pyx_L1_error)
 
-    /* "kola/lexer.pyx":170
+    /* "kola/lexer.pyx":157
  *         self.lexer_data.filename = "<unknown>"
  *         self.lexer_data.command_threshold = 1
  *         if yylex_init_extra(&self.lexer_data, &self.scanner):             # <<<<<<<<<<<<<<
  *             PyErr_SetFromErrno(RuntimeError)
  * 
  */
   }
 
-  /* "kola/lexer.pyx":166
+  /* "kola/lexer.pyx":153
  *     """
  * 
  *     def __cinit__(self, *args, **kwds):             # <<<<<<<<<<<<<<
  *         self.encoding = "utf-8"
  *         self.lexer_data.filename = "<unknown>"
  */
 
@@ -5695,15 +5786,15 @@
   __Pyx_AddTraceback("kola.lexer.BaseLexer.__cinit__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "kola/lexer.pyx":173
+/* "kola/lexer.pyx":160
  *             PyErr_SetFromErrno(RuntimeError)
  * 
  *     def __init__(self, **kwds):             # <<<<<<<<<<<<<<
  *         yyrestart(stdin, self.scanner)
  *         self.lexer_data.filename = "<stdin>"
  */
 
@@ -5743,53 +5834,53 @@
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__init__", 0);
 
-  /* "kola/lexer.pyx":174
+  /* "kola/lexer.pyx":161
  * 
  *     def __init__(self, **kwds):
  *         yyrestart(stdin, self.scanner)             # <<<<<<<<<<<<<<
  *         self.lexer_data.filename = "<stdin>"
  *         LexerConfig(self).set(**kwds)
  */
   yyrestart(stdin, __pyx_v_self->scanner);
 
-  /* "kola/lexer.pyx":175
+  /* "kola/lexer.pyx":162
  *     def __init__(self, **kwds):
  *         yyrestart(stdin, self.scanner)
  *         self.lexer_data.filename = "<stdin>"             # <<<<<<<<<<<<<<
  *         LexerConfig(self).set(**kwds)
  * 
  */
   __pyx_v_self->lexer_data.filename = ((char const *)"<stdin>");
 
-  /* "kola/lexer.pyx":176
+  /* "kola/lexer.pyx":163
  *         yyrestart(stdin, self.scanner)
  *         self.lexer_data.filename = "<stdin>"
  *         LexerConfig(self).set(**kwds)             # <<<<<<<<<<<<<<
  * 
  *     def __dealloc__(self):
  */
-  __pyx_t_1 = __Pyx_PyObject_CallOneArg(((PyObject *)__pyx_ptype_4kola_5lexer_LexerConfig), ((PyObject *)__pyx_v_self)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 176, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_CallOneArg(((PyObject *)__pyx_ptype_4kola_5lexer_LexerConfig), ((PyObject *)__pyx_v_self)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 163, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_set); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 176, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_set); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 163, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyDict_Copy(__pyx_v_kwds); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 176, __pyx_L1_error)
+  __pyx_t_1 = PyDict_Copy(__pyx_v_kwds); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 163, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_empty_tuple, __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 176, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_empty_tuple, __pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 163, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "kola/lexer.pyx":173
+  /* "kola/lexer.pyx":160
  *             PyErr_SetFromErrno(RuntimeError)
  * 
  *     def __init__(self, **kwds):             # <<<<<<<<<<<<<<
  *         yyrestart(stdin, self.scanner)
  *         self.lexer_data.filename = "<stdin>"
  */
 
@@ -5803,15 +5894,15 @@
   __Pyx_AddTraceback("kola.lexer.BaseLexer.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "kola/lexer.pyx":178
+/* "kola/lexer.pyx":165
  *         LexerConfig(self).set(**kwds)
  * 
  *     def __dealloc__(self):             # <<<<<<<<<<<<<<
  *         self.close()
  *         if self.scanner:
  */
 
@@ -5828,64 +5919,64 @@
 }
 
 static void __pyx_pf_4kola_5lexer_9BaseLexer_4__dealloc__(struct __pyx_obj_4kola_5lexer_BaseLexer *__pyx_v_self) {
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("__dealloc__", 0);
 
-  /* "kola/lexer.pyx":179
+  /* "kola/lexer.pyx":166
  * 
  *     def __dealloc__(self):
  *         self.close()             # <<<<<<<<<<<<<<
  *         if self.scanner:
  *             yylex_destroy(self.scanner)
  */
   ((struct __pyx_vtabstruct_4kola_5lexer_BaseLexer *)__pyx_v_self->__pyx_vtab)->close(__pyx_v_self, 0);
 
-  /* "kola/lexer.pyx":180
+  /* "kola/lexer.pyx":167
  *     def __dealloc__(self):
  *         self.close()
  *         if self.scanner:             # <<<<<<<<<<<<<<
  *             yylex_destroy(self.scanner)
  * 
  */
   __pyx_t_1 = (__pyx_v_self->scanner != 0);
   if (__pyx_t_1) {
 
-    /* "kola/lexer.pyx":181
+    /* "kola/lexer.pyx":168
  *         self.close()
  *         if self.scanner:
  *             yylex_destroy(self.scanner)             # <<<<<<<<<<<<<<
  * 
  *     cpdef void close(self):
  */
     (void)(yylex_destroy(__pyx_v_self->scanner));
 
-    /* "kola/lexer.pyx":180
+    /* "kola/lexer.pyx":167
  *     def __dealloc__(self):
  *         self.close()
  *         if self.scanner:             # <<<<<<<<<<<<<<
  *             yylex_destroy(self.scanner)
  * 
  */
   }
 
-  /* "kola/lexer.pyx":178
+  /* "kola/lexer.pyx":165
  *         LexerConfig(self).set(**kwds)
  * 
  *     def __dealloc__(self):             # <<<<<<<<<<<<<<
  *         self.close()
  *         if self.scanner:
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "kola/lexer.pyx":183
+/* "kola/lexer.pyx":170
  *             yylex_destroy(self.scanner)
  * 
  *     cpdef void close(self):             # <<<<<<<<<<<<<<
  *         yypop_buffer_state(self.scanner)
  * 
  */
 
@@ -5912,15 +6003,15 @@
   /* Check if overridden in Python */
   else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || __Pyx_PyType_HasFeature(Py_TYPE(((PyObject *)__pyx_v_self)), (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
     if (unlikely(!__Pyx_object_dict_version_matches(((PyObject *)__pyx_v_self), __pyx_tp_dict_version, __pyx_obj_dict_version))) {
       PY_UINT64_T __pyx_typedict_guard = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
       #endif
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_close); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 183, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_close); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 170, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       #ifdef __Pyx_CyFunction_USED
       if (!__Pyx_IsCyOrPyCFunction(__pyx_t_1)
       #else
       if (!PyCFunction_Check(__pyx_t_1)
       #endif
               || (PyCFunction_GET_FUNCTION(__pyx_t_1) != (PyCFunction)(void*)__pyx_pw_4kola_5lexer_9BaseLexer_7close)) {
@@ -5937,15 +6028,15 @@
             __pyx_t_5 = 1;
           }
         }
         {
           PyObject *__pyx_callargs[1] = {__pyx_t_4, };
           __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_5, 0+__pyx_t_5);
           __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-          if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 183, __pyx_L1_error)
+          if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 170, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
         }
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         goto __pyx_L0;
       }
@@ -5958,24 +6049,24 @@
       #endif
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     }
     #endif
   }
 
-  /* "kola/lexer.pyx":184
+  /* "kola/lexer.pyx":171
  * 
  *     cpdef void close(self):
  *         yypop_buffer_state(self.scanner)             # <<<<<<<<<<<<<<
  * 
  *     cdef void set_error(self, const char* text) except *:
  */
   yypop_buffer_state(__pyx_v_self->scanner);
 
-  /* "kola/lexer.pyx":183
+  /* "kola/lexer.pyx":170
  *             yylex_destroy(self.scanner)
  * 
  *     cpdef void close(self):             # <<<<<<<<<<<<<<
  *         yypop_buffer_state(self.scanner)
  * 
  */
 
@@ -6029,15 +6120,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("close", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_void_to_None(__pyx_f_4kola_5lexer_9BaseLexer_close(__pyx_v_self, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 183, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_void_to_None(__pyx_f_4kola_5lexer_9BaseLexer_close(__pyx_v_self, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 170, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -6046,15 +6137,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "kola/lexer.pyx":186
+/* "kola/lexer.pyx":173
  *         yypop_buffer_state(self.scanner)
  * 
  *     cdef void set_error(self, const char* text) except *:             # <<<<<<<<<<<<<<
  *         cdef int errno = 1
  * 
  */
 
@@ -6067,42 +6158,42 @@
   int __pyx_t_2;
   PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("set_error", 0);
 
-  /* "kola/lexer.pyx":187
+  /* "kola/lexer.pyx":174
  * 
  *     cdef void set_error(self, const char* text) except *:
  *         cdef int errno = 1             # <<<<<<<<<<<<<<
  * 
  *         # correct lineno and set error
  */
   __pyx_v_errno = 1;
 
-  /* "kola/lexer.pyx":190
+  /* "kola/lexer.pyx":177
  * 
  *         # correct lineno and set error
  *         cdef bint c = strchr(text, ord('\n')) != NULL             # <<<<<<<<<<<<<<
  *         cdef int lineno = yyget_lineno(self.scanner)
  *         if c or text[0] == 0:
  */
   __pyx_v_c = (strchr(__pyx_v_text, 10) != NULL);
 
-  /* "kola/lexer.pyx":191
+  /* "kola/lexer.pyx":178
  *         # correct lineno and set error
  *         cdef bint c = strchr(text, ord('\n')) != NULL
  *         cdef int lineno = yyget_lineno(self.scanner)             # <<<<<<<<<<<<<<
  *         if c or text[0] == 0:
  *             lineno -= c
  */
   __pyx_v_lineno = yyget_lineno(__pyx_v_self->scanner);
 
-  /* "kola/lexer.pyx":192
+  /* "kola/lexer.pyx":179
  *         cdef bint c = strchr(text, ord('\n')) != NULL
  *         cdef int lineno = yyget_lineno(self.scanner)
  *         if c or text[0] == 0:             # <<<<<<<<<<<<<<
  *             lineno -= c
  *             errno = 10
  */
   __pyx_t_2 = (__pyx_v_c != 0);
@@ -6112,54 +6203,54 @@
     goto __pyx_L4_bool_binop_done;
   }
   __pyx_t_2 = (((__pyx_v_text[0]) == 0) != 0);
   __pyx_t_1 = __pyx_t_2;
   __pyx_L4_bool_binop_done:;
   if (__pyx_t_1) {
 
-    /* "kola/lexer.pyx":193
+    /* "kola/lexer.pyx":180
  *         cdef int lineno = yyget_lineno(self.scanner)
  *         if c or text[0] == 0:
  *             lineno -= c             # <<<<<<<<<<<<<<
  *             errno = 10
  *         kola_set_error(KoiLangSyntaxError, errno, self.lexer_data.filename, lineno, text)
  */
     __pyx_v_lineno = (__pyx_v_lineno - __pyx_v_c);
 
-    /* "kola/lexer.pyx":194
+    /* "kola/lexer.pyx":181
  *         if c or text[0] == 0:
  *             lineno -= c
  *             errno = 10             # <<<<<<<<<<<<<<
  *         kola_set_error(KoiLangSyntaxError, errno, self.lexer_data.filename, lineno, text)
  * 
  */
     __pyx_v_errno = 10;
 
-    /* "kola/lexer.pyx":192
+    /* "kola/lexer.pyx":179
  *         cdef bint c = strchr(text, ord('\n')) != NULL
  *         cdef int lineno = yyget_lineno(self.scanner)
  *         if c or text[0] == 0:             # <<<<<<<<<<<<<<
  *             lineno -= c
  *             errno = 10
  */
   }
 
-  /* "kola/lexer.pyx":195
+  /* "kola/lexer.pyx":182
  *             lineno -= c
  *             errno = 10
  *         kola_set_error(KoiLangSyntaxError, errno, self.lexer_data.filename, lineno, text)             # <<<<<<<<<<<<<<
  * 
  *     cdef (int, const char*, Py_ssize_t) next_syn(self) nogil:
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_KoiLangSyntaxError); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 195, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_KoiLangSyntaxError); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 182, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  kola_set_error(__pyx_t_3, __pyx_v_errno, __pyx_v_self->lexer_data.filename, __pyx_v_lineno, __pyx_v_text); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 195, __pyx_L1_error)
+  kola_set_error(__pyx_t_3, __pyx_v_errno, __pyx_v_self->lexer_data.filename, __pyx_v_lineno, __pyx_v_text); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 182, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "kola/lexer.pyx":186
+  /* "kola/lexer.pyx":173
  *         yypop_buffer_state(self.scanner)
  * 
  *     cdef void set_error(self, const char* text) except *:             # <<<<<<<<<<<<<<
  *         cdef int errno = 1
  * 
  */
 
@@ -6168,63 +6259,63 @@
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_AddTraceback("kola.lexer.BaseLexer.set_error", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
 }
 
-/* "kola/lexer.pyx":197
+/* "kola/lexer.pyx":184
  *         kola_set_error(KoiLangSyntaxError, errno, self.lexer_data.filename, lineno, text)
  * 
  *     cdef (int, const char*, Py_ssize_t) next_syn(self) nogil:             # <<<<<<<<<<<<<<
  *         cdef int syn = yylex(self.scanner)
  *         return syn, yyget_text(self.scanner), yyget_leng(self.scanner)
  */
 
 static __pyx_ctuple_int__and_char__space_const__ptr__and_Py_ssize_t __pyx_f_4kola_5lexer_9BaseLexer_next_syn(struct __pyx_obj_4kola_5lexer_BaseLexer *__pyx_v_self) {
   int __pyx_v_syn;
   __pyx_ctuple_int__and_char__space_const__ptr__and_Py_ssize_t __pyx_r;
   __pyx_ctuple_int__and_char__space_const__ptr__and_Py_ssize_t __pyx_t_1;
 
-  /* "kola/lexer.pyx":198
+  /* "kola/lexer.pyx":185
  * 
  *     cdef (int, const char*, Py_ssize_t) next_syn(self) nogil:
  *         cdef int syn = yylex(self.scanner)             # <<<<<<<<<<<<<<
  *         return syn, yyget_text(self.scanner), yyget_leng(self.scanner)
  * 
  */
   __pyx_v_syn = yylex(__pyx_v_self->scanner);
 
-  /* "kola/lexer.pyx":199
+  /* "kola/lexer.pyx":186
  *     cdef (int, const char*, Py_ssize_t) next_syn(self) nogil:
  *         cdef int syn = yylex(self.scanner)
  *         return syn, yyget_text(self.scanner), yyget_leng(self.scanner)             # <<<<<<<<<<<<<<
  * 
  *     cdef Token next_token(self):
  */
   __pyx_t_1.f0 = __pyx_v_syn;
   __pyx_t_1.f1 = yyget_text(__pyx_v_self->scanner);
   __pyx_t_1.f2 = yyget_leng(__pyx_v_self->scanner);
   __pyx_r = __pyx_t_1;
   goto __pyx_L0;
 
-  /* "kola/lexer.pyx":197
+  /* "kola/lexer.pyx":184
  *         kola_set_error(KoiLangSyntaxError, errno, self.lexer_data.filename, lineno, text)
  * 
  *     cdef (int, const char*, Py_ssize_t) next_syn(self) nogil:             # <<<<<<<<<<<<<<
  *         cdef int syn = yylex(self.scanner)
  *         return syn, yyget_text(self.scanner), yyget_leng(self.scanner)
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "kola/lexer.pyx":201
+/* "kola/lexer.pyx":188
  *         return syn, yyget_text(self.scanner), yyget_leng(self.scanner)
  * 
  *     cdef Token next_token(self):             # <<<<<<<<<<<<<<
  *         if not yylex_check(self.scanner):
  *             raise OSError("operation on closed lexer")
  */
 
@@ -6261,47 +6352,47 @@
   PyObject *__pyx_t_21 = NULL;
   PyObject *__pyx_t_22 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("next_token", 0);
 
-  /* "kola/lexer.pyx":202
+  /* "kola/lexer.pyx":189
  * 
  *     cdef Token next_token(self):
  *         if not yylex_check(self.scanner):             # <<<<<<<<<<<<<<
  *             raise OSError("operation on closed lexer")
  * 
  */
   __pyx_t_1 = ((!(yylex_check(__pyx_v_self->scanner) != 0)) != 0);
   if (unlikely(__pyx_t_1)) {
 
-    /* "kola/lexer.pyx":203
+    /* "kola/lexer.pyx":190
  *     cdef Token next_token(self):
  *         if not yylex_check(self.scanner):
  *             raise OSError("operation on closed lexer")             # <<<<<<<<<<<<<<
  * 
  *         cdef:
  */
-    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_OSError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 203, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_OSError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 190, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    __PYX_ERR(1, 203, __pyx_L1_error)
+    __PYX_ERR(1, 190, __pyx_L1_error)
 
-    /* "kola/lexer.pyx":202
+    /* "kola/lexer.pyx":189
  * 
  *     cdef Token next_token(self):
  *         if not yylex_check(self.scanner):             # <<<<<<<<<<<<<<
  *             raise OSError("operation on closed lexer")
  * 
  */
   }
 
-  /* "kola/lexer.pyx":210
+  /* "kola/lexer.pyx":197
  *             Py_ssize_t text_len
  *             const char* encoding
  *         with nogil:             # <<<<<<<<<<<<<<
  *             syn, text, text_len = self.next_syn()
  * 
  */
   {
@@ -6309,15 +6400,15 @@
       PyThreadState *_save;
       _save = NULL;
       Py_UNBLOCK_THREADS
       __Pyx_FastGIL_Remember();
       #endif
       /*try:*/ {
 
-        /* "kola/lexer.pyx":211
+        /* "kola/lexer.pyx":198
  *             const char* encoding
  *         with nogil:
  *             syn, text, text_len = self.next_syn()             # <<<<<<<<<<<<<<
  * 
  *         val = None
  */
         __pyx_t_3 = ((struct __pyx_vtabstruct_4kola_5lexer_BaseLexer *)__pyx_v_self->__pyx_vtab)->next_syn(__pyx_v_self);
@@ -6325,15 +6416,15 @@
         __pyx_t_5 = __pyx_t_3.f1;
         __pyx_t_6 = __pyx_t_3.f2;
         __pyx_v_syn = __pyx_t_4;
         __pyx_v_text = __pyx_t_5;
         __pyx_v_text_len = __pyx_t_6;
       }
 
-      /* "kola/lexer.pyx":210
+      /* "kola/lexer.pyx":197
  *             Py_ssize_t text_len
  *             const char* encoding
  *         with nogil:             # <<<<<<<<<<<<<<
  *             syn, text, text_len = self.next_syn()
  * 
  */
       /*finally:*/ {
@@ -6344,271 +6435,271 @@
           #endif
           goto __pyx_L6;
         }
         __pyx_L6:;
       }
   }
 
-  /* "kola/lexer.pyx":213
+  /* "kola/lexer.pyx":200
  *             syn, text, text_len = self.next_syn()
  * 
  *         val = None             # <<<<<<<<<<<<<<
  *         if syn == NUM or syn == CMD_N:
  *             val = PyLong_FromString(text, NULL, 10)
  */
   __Pyx_INCREF(Py_None);
   __pyx_v_val = Py_None;
 
-  /* "kola/lexer.pyx":214
+  /* "kola/lexer.pyx":201
  * 
  *         val = None
  *         if syn == NUM or syn == CMD_N:             # <<<<<<<<<<<<<<
  *             val = PyLong_FromString(text, NULL, 10)
  *         elif syn == NUM_H:
  */
   switch (__pyx_v_syn) {
     case NUM:
     case CMD_N:
 
-    /* "kola/lexer.pyx":215
+    /* "kola/lexer.pyx":202
  *         val = None
  *         if syn == NUM or syn == CMD_N:
  *             val = PyLong_FromString(text, NULL, 10)             # <<<<<<<<<<<<<<
  *         elif syn == NUM_H:
  *             val = PyLong_FromString(text, NULL, 16)
  */
-    __pyx_t_2 = PyLong_FromString(__pyx_v_text, NULL, 10); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 215, __pyx_L1_error)
+    __pyx_t_2 = PyLong_FromString(__pyx_v_text, NULL, 10); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 202, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF_SET(__pyx_v_val, __pyx_t_2);
     __pyx_t_2 = 0;
 
-    /* "kola/lexer.pyx":214
+    /* "kola/lexer.pyx":201
  * 
  *         val = None
  *         if syn == NUM or syn == CMD_N:             # <<<<<<<<<<<<<<
  *             val = PyLong_FromString(text, NULL, 10)
  *         elif syn == NUM_H:
  */
     break;
     case NUM_H:
 
-    /* "kola/lexer.pyx":217
+    /* "kola/lexer.pyx":204
  *             val = PyLong_FromString(text, NULL, 10)
  *         elif syn == NUM_H:
  *             val = PyLong_FromString(text, NULL, 16)             # <<<<<<<<<<<<<<
  *         elif syn == NUM_B:
  *             val = PyLong_FromString(text, NULL, 2)
  */
-    __pyx_t_2 = PyLong_FromString(__pyx_v_text, NULL, 16); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 217, __pyx_L1_error)
+    __pyx_t_2 = PyLong_FromString(__pyx_v_text, NULL, 16); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 204, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF_SET(__pyx_v_val, __pyx_t_2);
     __pyx_t_2 = 0;
 
-    /* "kola/lexer.pyx":216
+    /* "kola/lexer.pyx":203
  *         if syn == NUM or syn == CMD_N:
  *             val = PyLong_FromString(text, NULL, 10)
  *         elif syn == NUM_H:             # <<<<<<<<<<<<<<
  *             val = PyLong_FromString(text, NULL, 16)
  *         elif syn == NUM_B:
  */
     break;
     case NUM_B:
 
-    /* "kola/lexer.pyx":219
+    /* "kola/lexer.pyx":206
  *             val = PyLong_FromString(text, NULL, 16)
  *         elif syn == NUM_B:
  *             val = PyLong_FromString(text, NULL, 2)             # <<<<<<<<<<<<<<
  *         elif syn == NUM_F:
  *             val = PyFloat_FromString(text)
  */
-    __pyx_t_2 = PyLong_FromString(__pyx_v_text, NULL, 2); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 219, __pyx_L1_error)
+    __pyx_t_2 = PyLong_FromString(__pyx_v_text, NULL, 2); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 206, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_DECREF_SET(__pyx_v_val, __pyx_t_2);
     __pyx_t_2 = 0;
 
-    /* "kola/lexer.pyx":218
+    /* "kola/lexer.pyx":205
  *         elif syn == NUM_H:
  *             val = PyLong_FromString(text, NULL, 16)
  *         elif syn == NUM_B:             # <<<<<<<<<<<<<<
  *             val = PyLong_FromString(text, NULL, 2)
  *         elif syn == NUM_F:
  */
     break;
     case NUM_F:
 
-    /* "kola/lexer.pyx":221
+    /* "kola/lexer.pyx":208
  *             val = PyLong_FromString(text, NULL, 2)
  *         elif syn == NUM_F:
  *             val = PyFloat_FromString(text)             # <<<<<<<<<<<<<<
  *         elif syn == CMD or syn == LITERAL:
  *             val = PyUnicode_FromStringAndSize(text, text_len)
  */
-    __pyx_t_2 = __Pyx_PyBytes_FromString(__pyx_v_text); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 221, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyBytes_FromString(__pyx_v_text); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 208, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_7 = __Pyx_PyFloat_FromString(__pyx_t_2); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 221, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyFloat_FromString(__pyx_t_2); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 208, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_DECREF_SET(__pyx_v_val, __pyx_t_7);
     __pyx_t_7 = 0;
 
-    /* "kola/lexer.pyx":220
+    /* "kola/lexer.pyx":207
  *         elif syn == NUM_B:
  *             val = PyLong_FromString(text, NULL, 2)
  *         elif syn == NUM_F:             # <<<<<<<<<<<<<<
  *             val = PyFloat_FromString(text)
  *         elif syn == CMD or syn == LITERAL:
  */
     break;
     case CMD:
 
-    /* "kola/lexer.pyx":222
+    /* "kola/lexer.pyx":209
  *         elif syn == NUM_F:
  *             val = PyFloat_FromString(text)
  *         elif syn == CMD or syn == LITERAL:             # <<<<<<<<<<<<<<
  *             val = PyUnicode_FromStringAndSize(text, text_len)
  *         elif syn == TEXT or syn == ANNOTATION:
  */
     case LITERAL:
 
-    /* "kola/lexer.pyx":223
+    /* "kola/lexer.pyx":210
  *             val = PyFloat_FromString(text)
  *         elif syn == CMD or syn == LITERAL:
  *             val = PyUnicode_FromStringAndSize(text, text_len)             # <<<<<<<<<<<<<<
  *         elif syn == TEXT or syn == ANNOTATION:
  *             encoding = unicode2string(self.encoding, NULL)
  */
-    __pyx_t_7 = PyUnicode_FromStringAndSize(__pyx_v_text, __pyx_v_text_len); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 223, __pyx_L1_error)
+    __pyx_t_7 = PyUnicode_FromStringAndSize(__pyx_v_text, __pyx_v_text_len); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 210, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __Pyx_DECREF_SET(__pyx_v_val, __pyx_t_7);
     __pyx_t_7 = 0;
 
-    /* "kola/lexer.pyx":222
+    /* "kola/lexer.pyx":209
  *         elif syn == NUM_F:
  *             val = PyFloat_FromString(text)
  *         elif syn == CMD or syn == LITERAL:             # <<<<<<<<<<<<<<
  *             val = PyUnicode_FromStringAndSize(text, text_len)
  *         elif syn == TEXT or syn == ANNOTATION:
  */
     break;
     case TEXT:
 
-    /* "kola/lexer.pyx":224
+    /* "kola/lexer.pyx":211
  *         elif syn == CMD or syn == LITERAL:
  *             val = PyUnicode_FromStringAndSize(text, text_len)
  *         elif syn == TEXT or syn == ANNOTATION:             # <<<<<<<<<<<<<<
  *             encoding = unicode2string(self.encoding, NULL)
  *             s = PyUnicode_Decode(text, text_len, encoding, NULL)
  */
     case ANNOTATION:
 
-    /* "kola/lexer.pyx":225
+    /* "kola/lexer.pyx":212
  *             val = PyUnicode_FromStringAndSize(text, text_len)
  *         elif syn == TEXT or syn == ANNOTATION:
  *             encoding = unicode2string(self.encoding, NULL)             # <<<<<<<<<<<<<<
  *             s = PyUnicode_Decode(text, text_len, encoding, NULL)
  *             val = <str>filter_text(s)
  */
     __pyx_t_7 = __pyx_v_self->encoding;
     __Pyx_INCREF(__pyx_t_7);
-    __pyx_t_8 = unicode2string(((PyObject*)__pyx_t_7), NULL); if (unlikely(__pyx_t_8 == ((char const *)NULL))) __PYX_ERR(1, 225, __pyx_L1_error)
+    __pyx_t_8 = unicode2string(((PyObject*)__pyx_t_7), NULL); if (unlikely(__pyx_t_8 == ((char const *)NULL))) __PYX_ERR(1, 212, __pyx_L1_error)
     __pyx_v_encoding = __pyx_t_8;
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-    /* "kola/lexer.pyx":226
+    /* "kola/lexer.pyx":213
  *         elif syn == TEXT or syn == ANNOTATION:
  *             encoding = unicode2string(self.encoding, NULL)
  *             s = PyUnicode_Decode(text, text_len, encoding, NULL)             # <<<<<<<<<<<<<<
  *             val = <str>filter_text(s)
  *         elif syn == STRING:
  */
-    __pyx_t_7 = PyUnicode_Decode(__pyx_v_text, __pyx_v_text_len, __pyx_v_encoding, NULL); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 226, __pyx_L1_error)
+    __pyx_t_7 = PyUnicode_Decode(__pyx_v_text, __pyx_v_text_len, __pyx_v_encoding, NULL); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 213, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
     __pyx_v_s = __pyx_t_7;
     __pyx_t_7 = 0;
 
-    /* "kola/lexer.pyx":227
+    /* "kola/lexer.pyx":214
  *             encoding = unicode2string(self.encoding, NULL)
  *             s = PyUnicode_Decode(text, text_len, encoding, NULL)
  *             val = <str>filter_text(s)             # <<<<<<<<<<<<<<
  *         elif syn == STRING:
  *             encoding = unicode2string(self.encoding, NULL)
  */
-    if (!(likely(PyUnicode_CheckExact(__pyx_v_s))||((__pyx_v_s) == Py_None) || __Pyx_RaiseUnexpectedTypeError("unicode", __pyx_v_s))) __PYX_ERR(1, 227, __pyx_L1_error)
-    __pyx_t_9 = filter_text(((PyObject*)__pyx_v_s)); if (unlikely(__pyx_t_9 == ((PyObject *)NULL))) __PYX_ERR(1, 227, __pyx_L1_error)
+    if (!(likely(PyUnicode_CheckExact(__pyx_v_s))||((__pyx_v_s) == Py_None) || __Pyx_RaiseUnexpectedTypeError("unicode", __pyx_v_s))) __PYX_ERR(1, 214, __pyx_L1_error)
+    __pyx_t_9 = filter_text(((PyObject*)__pyx_v_s)); if (unlikely(__pyx_t_9 == ((PyObject *)NULL))) __PYX_ERR(1, 214, __pyx_L1_error)
     __pyx_t_7 = ((PyObject *)__pyx_t_9);
     __Pyx_INCREF(__pyx_t_7);
     __Pyx_DECREF_SET(__pyx_v_val, __pyx_t_7);
     __pyx_t_7 = 0;
 
-    /* "kola/lexer.pyx":224
+    /* "kola/lexer.pyx":211
  *         elif syn == CMD or syn == LITERAL:
  *             val = PyUnicode_FromStringAndSize(text, text_len)
  *         elif syn == TEXT or syn == ANNOTATION:             # <<<<<<<<<<<<<<
  *             encoding = unicode2string(self.encoding, NULL)
  *             s = PyUnicode_Decode(text, text_len, encoding, NULL)
  */
     break;
     case STRING:
 
-    /* "kola/lexer.pyx":229
+    /* "kola/lexer.pyx":216
  *             val = <str>filter_text(s)
  *         elif syn == STRING:
  *             encoding = unicode2string(self.encoding, NULL)             # <<<<<<<<<<<<<<
  *             if strcmp(encoding, "utf-8") != 0:
  *                 s = PyUnicode_Decode(text, text_len, encoding, NULL)
  */
     __pyx_t_7 = __pyx_v_self->encoding;
     __Pyx_INCREF(__pyx_t_7);
-    __pyx_t_8 = unicode2string(((PyObject*)__pyx_t_7), NULL); if (unlikely(__pyx_t_8 == ((char const *)NULL))) __PYX_ERR(1, 229, __pyx_L1_error)
+    __pyx_t_8 = unicode2string(((PyObject*)__pyx_t_7), NULL); if (unlikely(__pyx_t_8 == ((char const *)NULL))) __PYX_ERR(1, 216, __pyx_L1_error)
     __pyx_v_encoding = __pyx_t_8;
     __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-    /* "kola/lexer.pyx":230
+    /* "kola/lexer.pyx":217
  *         elif syn == STRING:
  *             encoding = unicode2string(self.encoding, NULL)
  *             if strcmp(encoding, "utf-8") != 0:             # <<<<<<<<<<<<<<
  *                 s = PyUnicode_Decode(text, text_len, encoding, NULL)
  *                 text = unicode2string(s, &text_len)
  */
     __pyx_t_1 = ((strcmp(__pyx_v_encoding, ((char const *)"utf-8")) != 0) != 0);
     if (__pyx_t_1) {
 
-      /* "kola/lexer.pyx":231
+      /* "kola/lexer.pyx":218
  *             encoding = unicode2string(self.encoding, NULL)
  *             if strcmp(encoding, "utf-8") != 0:
  *                 s = PyUnicode_Decode(text, text_len, encoding, NULL)             # <<<<<<<<<<<<<<
  *                 text = unicode2string(s, &text_len)
  *             try:
  */
-      __pyx_t_7 = PyUnicode_Decode(__pyx_v_text, __pyx_v_text_len, __pyx_v_encoding, NULL); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 231, __pyx_L1_error)
+      __pyx_t_7 = PyUnicode_Decode(__pyx_v_text, __pyx_v_text_len, __pyx_v_encoding, NULL); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 218, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_7);
       __pyx_v_s = __pyx_t_7;
       __pyx_t_7 = 0;
 
-      /* "kola/lexer.pyx":232
+      /* "kola/lexer.pyx":219
  *             if strcmp(encoding, "utf-8") != 0:
  *                 s = PyUnicode_Decode(text, text_len, encoding, NULL)
  *                 text = unicode2string(s, &text_len)             # <<<<<<<<<<<<<<
  *             try:
  *                 val = decode_escapes(text + 1, text_len - 2)
  */
-      if (!(likely(PyUnicode_CheckExact(__pyx_v_s))||((__pyx_v_s) == Py_None) || __Pyx_RaiseUnexpectedTypeError("unicode", __pyx_v_s))) __PYX_ERR(1, 232, __pyx_L1_error)
-      __pyx_t_8 = unicode2string(((PyObject*)__pyx_v_s), (&__pyx_v_text_len)); if (unlikely(__pyx_t_8 == ((char const *)NULL))) __PYX_ERR(1, 232, __pyx_L1_error)
+      if (!(likely(PyUnicode_CheckExact(__pyx_v_s))||((__pyx_v_s) == Py_None) || __Pyx_RaiseUnexpectedTypeError("unicode", __pyx_v_s))) __PYX_ERR(1, 219, __pyx_L1_error)
+      __pyx_t_8 = unicode2string(((PyObject*)__pyx_v_s), (&__pyx_v_text_len)); if (unlikely(__pyx_t_8 == ((char const *)NULL))) __PYX_ERR(1, 219, __pyx_L1_error)
       __pyx_v_text = __pyx_t_8;
 
-      /* "kola/lexer.pyx":230
+      /* "kola/lexer.pyx":217
  *         elif syn == STRING:
  *             encoding = unicode2string(self.encoding, NULL)
  *             if strcmp(encoding, "utf-8") != 0:             # <<<<<<<<<<<<<<
  *                 s = PyUnicode_Decode(text, text_len, encoding, NULL)
  *                 text = unicode2string(s, &text_len)
  */
     }
 
-    /* "kola/lexer.pyx":233
+    /* "kola/lexer.pyx":220
  *                 s = PyUnicode_Decode(text, text_len, encoding, NULL)
  *                 text = unicode2string(s, &text_len)
  *             try:             # <<<<<<<<<<<<<<
  *                 val = decode_escapes(text + 1, text_len - 2)
  *             except Exception as e:
  */
     {
@@ -6616,27 +6707,27 @@
       __Pyx_PyThreadState_assign
       __Pyx_ExceptionSave(&__pyx_t_10, &__pyx_t_11, &__pyx_t_12);
       __Pyx_XGOTREF(__pyx_t_10);
       __Pyx_XGOTREF(__pyx_t_11);
       __Pyx_XGOTREF(__pyx_t_12);
       /*try:*/ {
 
-        /* "kola/lexer.pyx":234
+        /* "kola/lexer.pyx":221
  *                 text = unicode2string(s, &text_len)
  *             try:
  *                 val = decode_escapes(text + 1, text_len - 2)             # <<<<<<<<<<<<<<
  *             except Exception as e:
  *                 kola_set_errcause(KoiLangSyntaxError, 5, self.lexer_data.filename, yyget_lineno(self.scanner), text, e)
  */
-        __pyx_t_7 = decode_escapes((__pyx_v_text + 1), (__pyx_v_text_len - 2)); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 234, __pyx_L8_error)
+        __pyx_t_7 = decode_escapes((__pyx_v_text + 1), (__pyx_v_text_len - 2)); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 221, __pyx_L8_error)
         __Pyx_GOTREF(__pyx_t_7);
         __Pyx_DECREF_SET(__pyx_v_val, __pyx_t_7);
         __pyx_t_7 = 0;
 
-        /* "kola/lexer.pyx":233
+        /* "kola/lexer.pyx":220
  *                 s = PyUnicode_Decode(text, text_len, encoding, NULL)
  *                 text = unicode2string(s, &text_len)
  *             try:             # <<<<<<<<<<<<<<
  *                 val = decode_escapes(text + 1, text_len - 2)
  *             except Exception as e:
  */
       }
@@ -6644,46 +6735,46 @@
       __Pyx_XDECREF(__pyx_t_11); __pyx_t_11 = 0;
       __Pyx_XDECREF(__pyx_t_12); __pyx_t_12 = 0;
       goto __pyx_L13_try_end;
       __pyx_L8_error:;
       __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
       __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-      /* "kola/lexer.pyx":235
+      /* "kola/lexer.pyx":222
  *             try:
  *                 val = decode_escapes(text + 1, text_len - 2)
  *             except Exception as e:             # <<<<<<<<<<<<<<
  *                 kola_set_errcause(KoiLangSyntaxError, 5, self.lexer_data.filename, yyget_lineno(self.scanner), text, e)
  *         elif syn == 0:
  */
       __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
       if (__pyx_t_4) {
         __Pyx_AddTraceback("kola.lexer.BaseLexer.next_token", __pyx_clineno, __pyx_lineno, __pyx_filename);
-        if (__Pyx_GetException(&__pyx_t_7, &__pyx_t_2, &__pyx_t_13) < 0) __PYX_ERR(1, 235, __pyx_L10_except_error)
+        if (__Pyx_GetException(&__pyx_t_7, &__pyx_t_2, &__pyx_t_13) < 0) __PYX_ERR(1, 222, __pyx_L10_except_error)
         __Pyx_GOTREF(__pyx_t_7);
         __Pyx_GOTREF(__pyx_t_2);
         __Pyx_GOTREF(__pyx_t_13);
         __Pyx_INCREF(__pyx_t_2);
         __pyx_v_e = __pyx_t_2;
         /*try:*/ {
 
-          /* "kola/lexer.pyx":236
+          /* "kola/lexer.pyx":223
  *                 val = decode_escapes(text + 1, text_len - 2)
  *             except Exception as e:
  *                 kola_set_errcause(KoiLangSyntaxError, 5, self.lexer_data.filename, yyget_lineno(self.scanner), text, e)             # <<<<<<<<<<<<<<
  *         elif syn == 0:
  *             self.set_error(text)
  */
-          __Pyx_GetModuleGlobalName(__pyx_t_14, __pyx_n_s_KoiLangSyntaxError); if (unlikely(!__pyx_t_14)) __PYX_ERR(1, 236, __pyx_L19_error)
+          __Pyx_GetModuleGlobalName(__pyx_t_14, __pyx_n_s_KoiLangSyntaxError); if (unlikely(!__pyx_t_14)) __PYX_ERR(1, 223, __pyx_L19_error)
           __Pyx_GOTREF(__pyx_t_14);
-          kola_set_errcause(__pyx_t_14, 5, __pyx_v_self->lexer_data.filename, yyget_lineno(__pyx_v_self->scanner), __pyx_v_text, __pyx_v_e); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 236, __pyx_L19_error)
+          kola_set_errcause(__pyx_t_14, 5, __pyx_v_self->lexer_data.filename, yyget_lineno(__pyx_v_self->scanner), __pyx_v_text, __pyx_v_e); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 223, __pyx_L19_error)
           __Pyx_DECREF(__pyx_t_14); __pyx_t_14 = 0;
         }
 
-        /* "kola/lexer.pyx":235
+        /* "kola/lexer.pyx":222
  *             try:
  *                 val = decode_escapes(text + 1, text_len - 2)
  *             except Exception as e:             # <<<<<<<<<<<<<<
  *                 kola_set_errcause(KoiLangSyntaxError, 5, self.lexer_data.filename, yyget_lineno(self.scanner), text, e)
  *         elif syn == 0:
  */
         /*finally:*/ {
@@ -6729,15 +6820,15 @@
         __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
         __Pyx_XDECREF(__pyx_t_13); __pyx_t_13 = 0;
         goto __pyx_L9_exception_handled;
       }
       goto __pyx_L10_except_error;
       __pyx_L10_except_error:;
 
-      /* "kola/lexer.pyx":233
+      /* "kola/lexer.pyx":220
  *                 s = PyUnicode_Decode(text, text_len, encoding, NULL)
  *                 text = unicode2string(s, &text_len)
  *             try:             # <<<<<<<<<<<<<<
  *                 val = decode_escapes(text + 1, text_len - 2)
  *             except Exception as e:
  */
       __Pyx_XGIVEREF(__pyx_t_10);
@@ -6749,142 +6840,142 @@
       __Pyx_XGIVEREF(__pyx_t_10);
       __Pyx_XGIVEREF(__pyx_t_11);
       __Pyx_XGIVEREF(__pyx_t_12);
       __Pyx_ExceptionReset(__pyx_t_10, __pyx_t_11, __pyx_t_12);
       __pyx_L13_try_end:;
     }
 
-    /* "kola/lexer.pyx":228
+    /* "kola/lexer.pyx":215
  *             s = PyUnicode_Decode(text, text_len, encoding, NULL)
  *             val = <str>filter_text(s)
  *         elif syn == STRING:             # <<<<<<<<<<<<<<
  *             encoding = unicode2string(self.encoding, NULL)
  *             if strcmp(encoding, "utf-8") != 0:
  */
     break;
     case 0:
 
-    /* "kola/lexer.pyx":238
+    /* "kola/lexer.pyx":225
  *                 kola_set_errcause(KoiLangSyntaxError, 5, self.lexer_data.filename, yyget_lineno(self.scanner), text, e)
  *         elif syn == 0:
  *             self.set_error(text)             # <<<<<<<<<<<<<<
  *         elif syn == EOF:
  *             return None
  */
-    ((struct __pyx_vtabstruct_4kola_5lexer_BaseLexer *)__pyx_v_self->__pyx_vtab)->set_error(__pyx_v_self, __pyx_v_text); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 238, __pyx_L1_error)
+    ((struct __pyx_vtabstruct_4kola_5lexer_BaseLexer *)__pyx_v_self->__pyx_vtab)->set_error(__pyx_v_self, __pyx_v_text); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 225, __pyx_L1_error)
 
-    /* "kola/lexer.pyx":237
+    /* "kola/lexer.pyx":224
  *             except Exception as e:
  *                 kola_set_errcause(KoiLangSyntaxError, 5, self.lexer_data.filename, yyget_lineno(self.scanner), text, e)
  *         elif syn == 0:             # <<<<<<<<<<<<<<
  *             self.set_error(text)
  *         elif syn == EOF:
  */
     break;
     case EOF:
 
-    /* "kola/lexer.pyx":240
+    /* "kola/lexer.pyx":227
  *             self.set_error(text)
  *         elif syn == EOF:
  *             return None             # <<<<<<<<<<<<<<
  *         return Token(
  *             syn, val,
  */
     __Pyx_XDECREF((PyObject *)__pyx_r);
     __pyx_r = ((struct __pyx_obj_4kola_5lexer_Token *)Py_None); __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "kola/lexer.pyx":239
+    /* "kola/lexer.pyx":226
  *         elif syn == 0:
  *             self.set_error(text)
  *         elif syn == EOF:             # <<<<<<<<<<<<<<
  *             return None
  *         return Token(
  */
     break;
     default: break;
   }
 
-  /* "kola/lexer.pyx":241
+  /* "kola/lexer.pyx":228
  *         elif syn == EOF:
  *             return None
  *         return Token(             # <<<<<<<<<<<<<<
  *             syn, val,
  *             lineno=yyget_lineno(self.scanner),
  */
   __Pyx_XDECREF((PyObject *)__pyx_r);
 
-  /* "kola/lexer.pyx":242
+  /* "kola/lexer.pyx":229
  *             return None
  *         return Token(
  *             syn, val,             # <<<<<<<<<<<<<<
  *             lineno=yyget_lineno(self.scanner),
  *             raw_val=PyBytes_FromStringAndSize(text, text_len)
  */
-  __pyx_t_13 = __Pyx_PyInt_From_int(__pyx_v_syn); if (unlikely(!__pyx_t_13)) __PYX_ERR(1, 242, __pyx_L1_error)
+  __pyx_t_13 = __Pyx_PyInt_From_int(__pyx_v_syn); if (unlikely(!__pyx_t_13)) __PYX_ERR(1, 229, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_13);
 
-  /* "kola/lexer.pyx":241
+  /* "kola/lexer.pyx":228
  *         elif syn == EOF:
  *             return None
  *         return Token(             # <<<<<<<<<<<<<<
  *             syn, val,
  *             lineno=yyget_lineno(self.scanner),
  */
-  __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 241, __pyx_L1_error)
+  __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 228, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_13);
   PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_t_13);
   __Pyx_INCREF(__pyx_v_val);
   __Pyx_GIVEREF(__pyx_v_val);
   PyTuple_SET_ITEM(__pyx_t_2, 1, __pyx_v_val);
   __pyx_t_13 = 0;
 
-  /* "kola/lexer.pyx":243
+  /* "kola/lexer.pyx":230
  *         return Token(
  *             syn, val,
  *             lineno=yyget_lineno(self.scanner),             # <<<<<<<<<<<<<<
  *             raw_val=PyBytes_FromStringAndSize(text, text_len)
  *         )
  */
-  __pyx_t_13 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_13)) __PYX_ERR(1, 243, __pyx_L1_error)
+  __pyx_t_13 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_13)) __PYX_ERR(1, 230, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_13);
-  __pyx_t_7 = __Pyx_PyInt_From_int(yyget_lineno(__pyx_v_self->scanner)); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 243, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyInt_From_int(yyget_lineno(__pyx_v_self->scanner)); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 230, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  if (PyDict_SetItem(__pyx_t_13, __pyx_n_s_lineno, __pyx_t_7) < 0) __PYX_ERR(1, 243, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_13, __pyx_n_s_lineno, __pyx_t_7) < 0) __PYX_ERR(1, 230, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-  /* "kola/lexer.pyx":244
+  /* "kola/lexer.pyx":231
  *             syn, val,
  *             lineno=yyget_lineno(self.scanner),
  *             raw_val=PyBytes_FromStringAndSize(text, text_len)             # <<<<<<<<<<<<<<
  *         )
  * 
  */
-  __pyx_t_7 = PyBytes_FromStringAndSize(__pyx_v_text, __pyx_v_text_len); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 244, __pyx_L1_error)
+  __pyx_t_7 = PyBytes_FromStringAndSize(__pyx_v_text, __pyx_v_text_len); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 231, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  if (PyDict_SetItem(__pyx_t_13, __pyx_n_s_raw_val, __pyx_t_7) < 0) __PYX_ERR(1, 243, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_13, __pyx_n_s_raw_val, __pyx_t_7) < 0) __PYX_ERR(1, 230, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-  /* "kola/lexer.pyx":241
+  /* "kola/lexer.pyx":228
  *         elif syn == EOF:
  *             return None
  *         return Token(             # <<<<<<<<<<<<<<
  *             syn, val,
  *             lineno=yyget_lineno(self.scanner),
  */
-  __pyx_t_7 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_4kola_5lexer_Token), __pyx_t_2, __pyx_t_13); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 241, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_Call(((PyObject *)__pyx_ptype_4kola_5lexer_Token), __pyx_t_2, __pyx_t_13); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 228, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_13); __pyx_t_13 = 0;
   __pyx_r = ((struct __pyx_obj_4kola_5lexer_Token *)__pyx_t_7);
   __pyx_t_7 = 0;
   goto __pyx_L0;
 
-  /* "kola/lexer.pyx":201
+  /* "kola/lexer.pyx":188
  *         return syn, yyget_text(self.scanner), yyget_leng(self.scanner)
  * 
  *     cdef Token next_token(self):             # <<<<<<<<<<<<<<
  *         if not yylex_check(self.scanner):
  *             raise OSError("operation on closed lexer")
  */
 
@@ -6901,15 +6992,15 @@
   __Pyx_XDECREF(__pyx_v_s);
   __Pyx_XDECREF(__pyx_v_e);
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "kola/lexer.pyx":247
+/* "kola/lexer.pyx":234
  *         )
  * 
  *     @property             # <<<<<<<<<<<<<<
  *     def filename(self):
  *         return self.lexer_data.filename.decode()
  */
 
@@ -6933,31 +7024,31 @@
   char const *__pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "kola/lexer.pyx":249
+  /* "kola/lexer.pyx":236
  *     @property
  *     def filename(self):
  *         return self.lexer_data.filename.decode()             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = __pyx_v_self->lexer_data.filename;
-  __pyx_t_2 = __Pyx_decode_c_string(__pyx_t_1, 0, strlen(__pyx_t_1), NULL, NULL, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 249, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_decode_c_string(__pyx_t_1, 0, strlen(__pyx_t_1), NULL, NULL, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 236, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_INCREF(__pyx_t_2);
   __pyx_r = __pyx_t_2;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "kola/lexer.pyx":247
+  /* "kola/lexer.pyx":234
  *         )
  * 
  *     @property             # <<<<<<<<<<<<<<
  *     def filename(self):
  *         return self.lexer_data.filename.decode()
  */
 
@@ -6968,15 +7059,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "kola/lexer.pyx":251
+/* "kola/lexer.pyx":238
  *         return self.lexer_data.filename.decode()
  * 
  *     @property             # <<<<<<<<<<<<<<
  *     def lineno(self):
  *         return yyget_lineno(self.scanner)
  */
 
@@ -6999,29 +7090,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "kola/lexer.pyx":253
+  /* "kola/lexer.pyx":240
  *     @property
  *     def lineno(self):
  *         return yyget_lineno(self.scanner)             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_int(yyget_lineno(__pyx_v_self->scanner)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 253, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(yyget_lineno(__pyx_v_self->scanner)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 240, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "kola/lexer.pyx":251
+  /* "kola/lexer.pyx":238
  *         return self.lexer_data.filename.decode()
  * 
  *     @property             # <<<<<<<<<<<<<<
  *     def lineno(self):
  *         return yyget_lineno(self.scanner)
  */
 
@@ -7032,15 +7123,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "kola/lexer.pyx":255
+/* "kola/lexer.pyx":242
  *         return yyget_lineno(self.scanner)
  * 
  *     @property             # <<<<<<<<<<<<<<
  *     def column(self):
  *         return yyget_column(self.scanner)
  */
 
@@ -7063,29 +7154,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "kola/lexer.pyx":257
+  /* "kola/lexer.pyx":244
  *     @property
  *     def column(self):
  *         return yyget_column(self.scanner)             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_int(yyget_column(__pyx_v_self->scanner)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 257, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(yyget_column(__pyx_v_self->scanner)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 244, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "kola/lexer.pyx":255
+  /* "kola/lexer.pyx":242
  *         return yyget_lineno(self.scanner)
  * 
  *     @property             # <<<<<<<<<<<<<<
  *     def column(self):
  *         return yyget_column(self.scanner)
  */
 
@@ -7096,15 +7187,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "kola/lexer.pyx":259
+/* "kola/lexer.pyx":246
  *         return yyget_column(self.scanner)
  * 
  *     @property             # <<<<<<<<<<<<<<
  *     def config(self) -> LexerConfig:
  *         return LexerConfig(self)
  */
 
@@ -7127,29 +7218,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "kola/lexer.pyx":261
+  /* "kola/lexer.pyx":248
  *     @property
  *     def config(self) -> LexerConfig:
  *         return LexerConfig(self)             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyObject_CallOneArg(((PyObject *)__pyx_ptype_4kola_5lexer_LexerConfig), ((PyObject *)__pyx_v_self)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 261, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_CallOneArg(((PyObject *)__pyx_ptype_4kola_5lexer_LexerConfig), ((PyObject *)__pyx_v_self)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 248, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "kola/lexer.pyx":259
+  /* "kola/lexer.pyx":246
  *         return yyget_column(self.scanner)
  * 
  *     @property             # <<<<<<<<<<<<<<
  *     def config(self) -> LexerConfig:
  *         return LexerConfig(self)
  */
 
@@ -7160,15 +7251,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "kola/lexer.pyx":263
+/* "kola/lexer.pyx":250
  *         return LexerConfig(self)
  * 
  *     @property             # <<<<<<<<<<<<<<
  *     def closed(self) -> bool:
  *         return not yylex_check(self.scanner)
  */
 
@@ -7191,29 +7282,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "kola/lexer.pyx":265
+  /* "kola/lexer.pyx":252
  *     @property
  *     def closed(self) -> bool:
  *         return not yylex_check(self.scanner)             # <<<<<<<<<<<<<<
  * 
  *     def __iter__(self):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyBool_FromLong((!(yylex_check(__pyx_v_self->scanner) != 0))); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 265, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyBool_FromLong((!(yylex_check(__pyx_v_self->scanner) != 0))); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 252, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "kola/lexer.pyx":263
+  /* "kola/lexer.pyx":250
  *         return LexerConfig(self)
  * 
  *     @property             # <<<<<<<<<<<<<<
  *     def closed(self) -> bool:
  *         return not yylex_check(self.scanner)
  */
 
@@ -7224,15 +7315,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "kola/lexer.pyx":267
+/* "kola/lexer.pyx":254
  *         return not yylex_check(self.scanner)
  * 
  *     def __iter__(self):             # <<<<<<<<<<<<<<
  *         return self
  * 
  */
 
@@ -7251,42 +7342,42 @@
 }
 
 static PyObject *__pyx_pf_4kola_5lexer_9BaseLexer_8__iter__(struct __pyx_obj_4kola_5lexer_BaseLexer *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__iter__", 0);
 
-  /* "kola/lexer.pyx":268
+  /* "kola/lexer.pyx":255
  * 
  *     def __iter__(self):
  *         return self             # <<<<<<<<<<<<<<
  * 
  *     def __next__(self):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF((PyObject *)__pyx_v_self);
   __pyx_r = ((PyObject *)__pyx_v_self);
   goto __pyx_L0;
 
-  /* "kola/lexer.pyx":267
+  /* "kola/lexer.pyx":254
  *         return not yylex_check(self.scanner)
  * 
  *     def __iter__(self):             # <<<<<<<<<<<<<<
  *         return self
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "kola/lexer.pyx":270
+/* "kola/lexer.pyx":257
  *         return self
  * 
  *     def __next__(self):             # <<<<<<<<<<<<<<
  *         token = self.next_token()
  *         if token is None:
  */
 
@@ -7312,69 +7403,69 @@
   int __pyx_t_2;
   int __pyx_t_3;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__next__", 0);
 
-  /* "kola/lexer.pyx":271
+  /* "kola/lexer.pyx":258
  * 
  *     def __next__(self):
  *         token = self.next_token()             # <<<<<<<<<<<<<<
  *         if token is None:
  *             raise StopIteration
  */
-  __pyx_t_1 = ((PyObject *)((struct __pyx_vtabstruct_4kola_5lexer_BaseLexer *)__pyx_v_self->__pyx_vtab)->next_token(__pyx_v_self)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 271, __pyx_L1_error)
+  __pyx_t_1 = ((PyObject *)((struct __pyx_vtabstruct_4kola_5lexer_BaseLexer *)__pyx_v_self->__pyx_vtab)->next_token(__pyx_v_self)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 258, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_token = ((struct __pyx_obj_4kola_5lexer_Token *)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "kola/lexer.pyx":272
+  /* "kola/lexer.pyx":259
  *     def __next__(self):
  *         token = self.next_token()
  *         if token is None:             # <<<<<<<<<<<<<<
  *             raise StopIteration
  *         return token
  */
   __pyx_t_2 = (((PyObject *)__pyx_v_token) == Py_None);
   __pyx_t_3 = (__pyx_t_2 != 0);
   if (unlikely(__pyx_t_3)) {
 
-    /* "kola/lexer.pyx":273
+    /* "kola/lexer.pyx":260
  *         token = self.next_token()
  *         if token is None:
  *             raise StopIteration             # <<<<<<<<<<<<<<
  *         return token
  * 
  */
     __Pyx_Raise(__pyx_builtin_StopIteration, 0, 0, 0);
-    __PYX_ERR(1, 273, __pyx_L1_error)
+    __PYX_ERR(1, 260, __pyx_L1_error)
 
-    /* "kola/lexer.pyx":272
+    /* "kola/lexer.pyx":259
  *     def __next__(self):
  *         token = self.next_token()
  *         if token is None:             # <<<<<<<<<<<<<<
  *             raise StopIteration
  *         return token
  */
   }
 
-  /* "kola/lexer.pyx":274
+  /* "kola/lexer.pyx":261
  *         if token is None:
  *             raise StopIteration
  *         return token             # <<<<<<<<<<<<<<
  * 
  *     def __enter__(self):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF((PyObject *)__pyx_v_token);
   __pyx_r = ((PyObject *)__pyx_v_token);
   goto __pyx_L0;
 
-  /* "kola/lexer.pyx":270
+  /* "kola/lexer.pyx":257
  *         return self
  * 
  *     def __next__(self):             # <<<<<<<<<<<<<<
  *         token = self.next_token()
  *         if token is None:
  */
 
@@ -7386,15 +7477,15 @@
   __pyx_L0:;
   __Pyx_XDECREF((PyObject *)__pyx_v_token);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "kola/lexer.pyx":276
+/* "kola/lexer.pyx":263
  *         return token
  * 
  *     def __enter__(self):             # <<<<<<<<<<<<<<
  *         return self
  * 
  */
 
@@ -7432,42 +7523,42 @@
 }
 
 static PyObject *__pyx_pf_4kola_5lexer_9BaseLexer_12__enter__(struct __pyx_obj_4kola_5lexer_BaseLexer *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__enter__", 0);
 
-  /* "kola/lexer.pyx":277
+  /* "kola/lexer.pyx":264
  * 
  *     def __enter__(self):
  *         return self             # <<<<<<<<<<<<<<
  * 
  *     def __exit__(self, *args):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF((PyObject *)__pyx_v_self);
   __pyx_r = ((PyObject *)__pyx_v_self);
   goto __pyx_L0;
 
-  /* "kola/lexer.pyx":276
+  /* "kola/lexer.pyx":263
  *         return token
  * 
  *     def __enter__(self):             # <<<<<<<<<<<<<<
  *         return self
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "kola/lexer.pyx":279
+/* "kola/lexer.pyx":266
  *         return self
  * 
  *     def __exit__(self, *args):             # <<<<<<<<<<<<<<
  *         self.close()
  * 
  */
 
@@ -7493,44 +7584,44 @@
 }
 
 static PyObject *__pyx_pf_4kola_5lexer_9BaseLexer_14__exit__(struct __pyx_obj_4kola_5lexer_BaseLexer *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v_args) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__exit__", 0);
 
-  /* "kola/lexer.pyx":280
+  /* "kola/lexer.pyx":267
  * 
  *     def __exit__(self, *args):
  *         self.close()             # <<<<<<<<<<<<<<
  * 
  *     def __repr__(self):
  */
   ((struct __pyx_vtabstruct_4kola_5lexer_BaseLexer *)__pyx_v_self->__pyx_vtab)->close(__pyx_v_self, 0);
 
-  /* "kola/lexer.pyx":279
+  /* "kola/lexer.pyx":266
  *         return self
  * 
  *     def __exit__(self, *args):             # <<<<<<<<<<<<<<
  *         self.close()
  * 
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "kola/lexer.pyx":282
+/* "kola/lexer.pyx":269
  *         self.close()
  * 
  *     def __repr__(self):             # <<<<<<<<<<<<<<
  *         if not yylex_check(self.scanner):
- *             return PyUnicode_FromFormat(
+ *             return PyUnicode_FromFormat("<kola lexer in file \"%s\" closed>")
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_4kola_5lexer_9BaseLexer_17__repr__(PyObject *__pyx_v_self); /*proto*/
 static PyObject *__pyx_pw_4kola_5lexer_9BaseLexer_17__repr__(PyObject *__pyx_v_self) {
   CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
   PyObject *__pyx_r = 0;
@@ -7549,99 +7640,91 @@
   int __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__repr__", 0);
 
-  /* "kola/lexer.pyx":283
+  /* "kola/lexer.pyx":270
  * 
  *     def __repr__(self):
  *         if not yylex_check(self.scanner):             # <<<<<<<<<<<<<<
- *             return PyUnicode_FromFormat(
- *                 "<kola lexer in file \"%s\" closed>",
+ *             return PyUnicode_FromFormat("<kola lexer in file \"%s\" closed>")
+ *         else:
  */
   __pyx_t_1 = ((!(yylex_check(__pyx_v_self->scanner) != 0)) != 0);
   if (__pyx_t_1) {
 
-    /* "kola/lexer.pyx":284
+    /* "kola/lexer.pyx":271
  *     def __repr__(self):
  *         if not yylex_check(self.scanner):
- *             return PyUnicode_FromFormat(             # <<<<<<<<<<<<<<
- *                 "<kola lexer in file \"%s\" closed>",
- *                 self.lexer_data.filename
- */
-    __Pyx_XDECREF(__pyx_r);
-
-    /* "kola/lexer.pyx":286
- *             return PyUnicode_FromFormat(
- *                 "<kola lexer in file \"%s\" closed>",
- *                 self.lexer_data.filename             # <<<<<<<<<<<<<<
- *             )
+ *             return PyUnicode_FromFormat("<kola lexer in file \"%s\" closed>")             # <<<<<<<<<<<<<<
  *         else:
+ *             return PyUnicode_FromFormat(
  */
-    __pyx_t_2 = PyUnicode_FromFormat(((char const *)"<kola lexer in file \"%s\" closed>"), __pyx_v_self->lexer_data.filename); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 284, __pyx_L1_error)
+    __Pyx_XDECREF(__pyx_r);
+    __pyx_t_2 = PyUnicode_FromFormat(((char const *)"<kola lexer in file \"%s\" closed>")); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 271, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_r = __pyx_t_2;
     __pyx_t_2 = 0;
     goto __pyx_L0;
 
-    /* "kola/lexer.pyx":283
+    /* "kola/lexer.pyx":270
  * 
  *     def __repr__(self):
  *         if not yylex_check(self.scanner):             # <<<<<<<<<<<<<<
- *             return PyUnicode_FromFormat(
- *                 "<kola lexer in file \"%s\" closed>",
+ *             return PyUnicode_FromFormat("<kola lexer in file \"%s\" closed>")
+ *         else:
  */
   }
 
-  /* "kola/lexer.pyx":289
- *             )
+  /* "kola/lexer.pyx":273
+ *             return PyUnicode_FromFormat("<kola lexer in file \"%s\" closed>")
  *         else:
  *             return PyUnicode_FromFormat(             # <<<<<<<<<<<<<<
  *                 "<kola lexer in file \"%s\" line %d>",
  *                 self.lexer_data.filename,
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
 
-    /* "kola/lexer.pyx":292
+    /* "kola/lexer.pyx":276
  *                 "<kola lexer in file \"%s\" line %d>",
  *                 self.lexer_data.filename,
  *                 yyget_lineno(self.scanner)             # <<<<<<<<<<<<<<
  *             )
  * 
  */
-    __pyx_t_2 = PyUnicode_FromFormat(((char const *)"<kola lexer in file \"%s\" line %d>"), __pyx_v_self->lexer_data.filename, yyget_lineno(__pyx_v_self->scanner)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 289, __pyx_L1_error)
+    __pyx_t_2 = PyUnicode_FromFormat(((char const *)"<kola lexer in file \"%s\" line %d>"), __pyx_v_self->lexer_data.filename, yyget_lineno(__pyx_v_self->scanner)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 273, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __pyx_r = __pyx_t_2;
     __pyx_t_2 = 0;
     goto __pyx_L0;
   }
 
-  /* "kola/lexer.pyx":282
+  /* "kola/lexer.pyx":269
  *         self.close()
  * 
  *     def __repr__(self):             # <<<<<<<<<<<<<<
  *         if not yylex_check(self.scanner):
- *             return PyUnicode_FromFormat(
+ *             return PyUnicode_FromFormat("<kola lexer in file \"%s\" closed>")
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_AddTraceback("kola.lexer.BaseLexer.__repr__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "kola/lexer.pxd":35
+/* "kola/lexer.pxd":31
  *         LexerData lexer_data
  *     cdef readonly:
  *         str encoding             # <<<<<<<<<<<<<<
  * 
  *     cpdef void close(self)
  */
 
@@ -7856,15 +7939,15 @@
   __Pyx_AddTraceback("kola.lexer.BaseLexer.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "kola/lexer.pyx":301
+/* "kola/lexer.pyx":285
  *     """
  * 
  *     def __init__(self, __path not None, **kwds):             # <<<<<<<<<<<<<<
  *         if self.fp:
  *             fclose(self.fp)
  */
 
@@ -7898,39 +7981,39 @@
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
       kw_args = __Pyx_NumKwargs_VARARGS(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_VARARGS(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_FileLexer__path)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 301, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 285, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, __pyx_v_kwds, values + 0, kwd_pos_args, "__init__") < 0)) __PYX_ERR(1, 301, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, __pyx_v_kwds, values + 0, kwd_pos_args, "__init__") < 0)) __PYX_ERR(1, 285, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_VARARGS(__pyx_args, 0);
     }
     __pyx_v__FileLexer__path = values[0];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__init__", 1, 1, 1, __pyx_nargs); __PYX_ERR(1, 301, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__init__", 1, 1, 1, __pyx_nargs); __PYX_ERR(1, 285, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_DECREF(__pyx_v_kwds); __pyx_v_kwds = 0;
   __Pyx_AddTraceback("kola.lexer.FileLexer.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
   if (unlikely(((PyObject *)__pyx_v__FileLexer__path) == Py_None)) {
-    PyErr_Format(PyExc_TypeError, "Argument '%.200s' must not be None", "__path"); __PYX_ERR(1, 301, __pyx_L1_error)
+    PyErr_Format(PyExc_TypeError, "Argument '%.200s' must not be None", "__path"); __PYX_ERR(1, 285, __pyx_L1_error)
   }
   __pyx_r = __pyx_pf_4kola_5lexer_9FileLexer___init__(((struct __pyx_obj_4kola_5lexer_FileLexer *)__pyx_v_self), __pyx_v__FileLexer__path, __pyx_v_kwds);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = -1;
@@ -7952,157 +8035,157 @@
   char const *__pyx_t_5;
   PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__init__", 0);
 
-  /* "kola/lexer.pyx":302
+  /* "kola/lexer.pyx":286
  * 
  *     def __init__(self, __path not None, **kwds):
  *         if self.fp:             # <<<<<<<<<<<<<<
  *             fclose(self.fp)
  * 
  */
   __pyx_t_1 = (__pyx_v_self->fp != 0);
   if (__pyx_t_1) {
 
-    /* "kola/lexer.pyx":303
+    /* "kola/lexer.pyx":287
  *     def __init__(self, __path not None, **kwds):
  *         if self.fp:
  *             fclose(self.fp)             # <<<<<<<<<<<<<<
  * 
  *         self._filenameo = __path
  */
     (void)(fclose(__pyx_v_self->fp));
 
-    /* "kola/lexer.pyx":302
+    /* "kola/lexer.pyx":286
  * 
  *     def __init__(self, __path not None, **kwds):
  *         if self.fp:             # <<<<<<<<<<<<<<
  *             fclose(self.fp)
  * 
  */
   }
 
-  /* "kola/lexer.pyx":305
+  /* "kola/lexer.pyx":289
  *             fclose(self.fp)
  * 
  *         self._filenameo = __path             # <<<<<<<<<<<<<<
  *         cdef PyObject* p_addr
  *         self.fp = kola_open(__path, &p_addr, 'r')
  */
   __Pyx_INCREF(__pyx_v__FileLexer__path);
   __Pyx_GIVEREF(__pyx_v__FileLexer__path);
   __Pyx_GOTREF(__pyx_v_self->_filenameo);
   __Pyx_DECREF(__pyx_v_self->_filenameo);
   __pyx_v_self->_filenameo = __pyx_v__FileLexer__path;
 
-  /* "kola/lexer.pyx":307
+  /* "kola/lexer.pyx":291
  *         self._filenameo = __path
  *         cdef PyObject* p_addr
  *         self.fp = kola_open(__path, &p_addr, 'r')             # <<<<<<<<<<<<<<
  *         p = <object>p_addr
  *         self._filenameb = <bytes>p if isinstance(p, bytes) else (<str>p).encode()
  */
-  __pyx_t_2 = kola_open(__pyx_v__FileLexer__path, (&__pyx_v_p_addr), ((char const *)"r")); if (unlikely(__pyx_t_2 == ((FILE *)NULL))) __PYX_ERR(1, 307, __pyx_L1_error)
+  __pyx_t_2 = kola_open(__pyx_v__FileLexer__path, (&__pyx_v_p_addr), ((char const *)"r")); if (unlikely(__pyx_t_2 == ((FILE *)NULL))) __PYX_ERR(1, 291, __pyx_L1_error)
   __pyx_v_self->fp = __pyx_t_2;
 
-  /* "kola/lexer.pyx":308
+  /* "kola/lexer.pyx":292
  *         cdef PyObject* p_addr
  *         self.fp = kola_open(__path, &p_addr, 'r')
  *         p = <object>p_addr             # <<<<<<<<<<<<<<
  *         self._filenameb = <bytes>p if isinstance(p, bytes) else (<str>p).encode()
  *         Py_DECREF(p)
  */
   __pyx_t_3 = ((PyObject *)__pyx_v_p_addr);
   __Pyx_INCREF(__pyx_t_3);
   __pyx_v_p = __pyx_t_3;
   __pyx_t_3 = 0;
 
-  /* "kola/lexer.pyx":309
+  /* "kola/lexer.pyx":293
  *         self.fp = kola_open(__path, &p_addr, 'r')
  *         p = <object>p_addr
  *         self._filenameb = <bytes>p if isinstance(p, bytes) else (<str>p).encode()             # <<<<<<<<<<<<<<
  *         Py_DECREF(p)
  * 
  */
   __pyx_t_1 = PyBytes_Check(__pyx_v_p); 
   if ((__pyx_t_1 != 0)) {
     __Pyx_INCREF(((PyObject*)__pyx_v_p));
     __pyx_t_3 = __pyx_v_p;
   } else {
     if (unlikely(__pyx_v_p == Py_None)) {
       PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "encode");
-      __PYX_ERR(1, 309, __pyx_L1_error)
+      __PYX_ERR(1, 293, __pyx_L1_error)
     }
-    __pyx_t_4 = PyUnicode_AsEncodedString(((PyObject*)__pyx_v_p), NULL, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 309, __pyx_L1_error)
+    __pyx_t_4 = PyUnicode_AsEncodedString(((PyObject*)__pyx_v_p), NULL, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 293, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __pyx_t_3 = __pyx_t_4;
     __pyx_t_4 = 0;
   }
   __Pyx_GIVEREF(__pyx_t_3);
   __Pyx_GOTREF(__pyx_v_self->_filenameb);
   __Pyx_DECREF(__pyx_v_self->_filenameb);
   __pyx_v_self->_filenameb = ((PyObject*)__pyx_t_3);
   __pyx_t_3 = 0;
 
-  /* "kola/lexer.pyx":310
+  /* "kola/lexer.pyx":294
  *         p = <object>p_addr
  *         self._filenameb = <bytes>p if isinstance(p, bytes) else (<str>p).encode()
  *         Py_DECREF(p)             # <<<<<<<<<<<<<<
  * 
  *         yyrestart(self.fp, self.scanner)
  */
   Py_DECREF(__pyx_v_p);
 
-  /* "kola/lexer.pyx":312
+  /* "kola/lexer.pyx":296
  *         Py_DECREF(p)
  * 
  *         yyrestart(self.fp, self.scanner)             # <<<<<<<<<<<<<<
  *         self.lexer_data.filename = self._filenameb
  *         LexerConfig(self).set(**kwds)
  */
   yyrestart(__pyx_v_self->fp, __pyx_v_self->__pyx_base.scanner);
 
-  /* "kola/lexer.pyx":313
+  /* "kola/lexer.pyx":297
  * 
  *         yyrestart(self.fp, self.scanner)
  *         self.lexer_data.filename = self._filenameb             # <<<<<<<<<<<<<<
  *         LexerConfig(self).set(**kwds)
  * 
  */
   if (unlikely(__pyx_v_self->_filenameb == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "expected bytes, NoneType found");
-    __PYX_ERR(1, 313, __pyx_L1_error)
+    __PYX_ERR(1, 297, __pyx_L1_error)
   }
-  __pyx_t_5 = __Pyx_PyBytes_AsString(__pyx_v_self->_filenameb); if (unlikely((!__pyx_t_5) && PyErr_Occurred())) __PYX_ERR(1, 313, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyBytes_AsString(__pyx_v_self->_filenameb); if (unlikely((!__pyx_t_5) && PyErr_Occurred())) __PYX_ERR(1, 297, __pyx_L1_error)
   __pyx_v_self->__pyx_base.lexer_data.filename = __pyx_t_5;
 
-  /* "kola/lexer.pyx":314
+  /* "kola/lexer.pyx":298
  *         yyrestart(self.fp, self.scanner)
  *         self.lexer_data.filename = self._filenameb
  *         LexerConfig(self).set(**kwds)             # <<<<<<<<<<<<<<
  * 
  *     cpdef void close(self):
  */
-  __pyx_t_3 = __Pyx_PyObject_CallOneArg(((PyObject *)__pyx_ptype_4kola_5lexer_LexerConfig), ((PyObject *)__pyx_v_self)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 314, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_CallOneArg(((PyObject *)__pyx_ptype_4kola_5lexer_LexerConfig), ((PyObject *)__pyx_v_self)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 298, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_set); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 314, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_set); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 298, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = PyDict_Copy(__pyx_v_kwds); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 314, __pyx_L1_error)
+  __pyx_t_3 = PyDict_Copy(__pyx_v_kwds); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 298, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_empty_tuple, __pyx_t_3); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 314, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_empty_tuple, __pyx_t_3); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 298, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
 
-  /* "kola/lexer.pyx":301
+  /* "kola/lexer.pyx":285
  *     """
  * 
  *     def __init__(self, __path not None, **kwds):             # <<<<<<<<<<<<<<
  *         if self.fp:
  *             fclose(self.fp)
  */
 
@@ -8117,15 +8200,15 @@
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_p);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "kola/lexer.pyx":316
+/* "kola/lexer.pyx":300
  *         LexerConfig(self).set(**kwds)
  * 
  *     cpdef void close(self):             # <<<<<<<<<<<<<<
  *         BaseLexer.close(self)
  *         if self.fp:
  */
 
@@ -8153,15 +8236,15 @@
   /* Check if overridden in Python */
   else if (unlikely((Py_TYPE(((PyObject *)__pyx_v_self))->tp_dictoffset != 0) || __Pyx_PyType_HasFeature(Py_TYPE(((PyObject *)__pyx_v_self)), (Py_TPFLAGS_IS_ABSTRACT | Py_TPFLAGS_HEAPTYPE)))) {
     #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     static PY_UINT64_T __pyx_tp_dict_version = __PYX_DICT_VERSION_INIT, __pyx_obj_dict_version = __PYX_DICT_VERSION_INIT;
     if (unlikely(!__Pyx_object_dict_version_matches(((PyObject *)__pyx_v_self), __pyx_tp_dict_version, __pyx_obj_dict_version))) {
       PY_UINT64_T __pyx_typedict_guard = __Pyx_get_tp_dict_version(((PyObject *)__pyx_v_self));
       #endif
-      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_close); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 316, __pyx_L1_error)
+      __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_self), __pyx_n_s_close); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 300, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_1);
       #ifdef __Pyx_CyFunction_USED
       if (!__Pyx_IsCyOrPyCFunction(__pyx_t_1)
       #else
       if (!PyCFunction_Check(__pyx_t_1)
       #endif
               || (PyCFunction_GET_FUNCTION(__pyx_t_1) != (PyCFunction)(void*)__pyx_pw_4kola_5lexer_9FileLexer_3close)) {
@@ -8178,15 +8261,15 @@
             __pyx_t_5 = 1;
           }
         }
         {
           PyObject *__pyx_callargs[1] = {__pyx_t_4, };
           __pyx_t_2 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_5, 0+__pyx_t_5);
           __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-          if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 316, __pyx_L1_error)
+          if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 300, __pyx_L1_error)
           __Pyx_GOTREF(__pyx_t_2);
           __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
         }
         __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
         __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
         goto __pyx_L0;
       }
@@ -8199,61 +8282,61 @@
       #endif
       __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
       #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_PYTYPE_LOOKUP && CYTHON_USE_TYPE_SLOTS
     }
     #endif
   }
 
-  /* "kola/lexer.pyx":317
+  /* "kola/lexer.pyx":301
  * 
  *     cpdef void close(self):
  *         BaseLexer.close(self)             # <<<<<<<<<<<<<<
  *         if self.fp:
  *             fclose(self.fp)
  */
   __pyx_f_4kola_5lexer_9BaseLexer_close(((struct __pyx_obj_4kola_5lexer_BaseLexer *)__pyx_v_self), 1);
 
-  /* "kola/lexer.pyx":318
+  /* "kola/lexer.pyx":302
  *     cpdef void close(self):
  *         BaseLexer.close(self)
  *         if self.fp:             # <<<<<<<<<<<<<<
  *             fclose(self.fp)
  *             self.fp = NULL
  */
   __pyx_t_6 = (__pyx_v_self->fp != 0);
   if (__pyx_t_6) {
 
-    /* "kola/lexer.pyx":319
+    /* "kola/lexer.pyx":303
  *         BaseLexer.close(self)
  *         if self.fp:
  *             fclose(self.fp)             # <<<<<<<<<<<<<<
  *             self.fp = NULL
  * 
  */
     (void)(fclose(__pyx_v_self->fp));
 
-    /* "kola/lexer.pyx":320
+    /* "kola/lexer.pyx":304
  *         if self.fp:
  *             fclose(self.fp)
  *             self.fp = NULL             # <<<<<<<<<<<<<<
  * 
  *     @property
  */
     __pyx_v_self->fp = NULL;
 
-    /* "kola/lexer.pyx":318
+    /* "kola/lexer.pyx":302
  *     cpdef void close(self):
  *         BaseLexer.close(self)
  *         if self.fp:             # <<<<<<<<<<<<<<
  *             fclose(self.fp)
  *             self.fp = NULL
  */
   }
 
-  /* "kola/lexer.pyx":316
+  /* "kola/lexer.pyx":300
  *         LexerConfig(self).set(**kwds)
  * 
  *     cpdef void close(self):             # <<<<<<<<<<<<<<
  *         BaseLexer.close(self)
  *         if self.fp:
  */
 
@@ -8307,15 +8390,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("close", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_void_to_None(__pyx_f_4kola_5lexer_9FileLexer_close(__pyx_v_self, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 316, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_void_to_None(__pyx_f_4kola_5lexer_9FileLexer_close(__pyx_v_self, 1)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 300, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -8324,15 +8407,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "kola/lexer.pyx":322
+/* "kola/lexer.pyx":306
  *             self.fp = NULL
  * 
  *     @property             # <<<<<<<<<<<<<<
  *     def filename(self):
  *         return self._filenameo
  */
 
@@ -8351,27 +8434,27 @@
 }
 
 static PyObject *__pyx_pf_4kola_5lexer_9FileLexer_8filename___get__(struct __pyx_obj_4kola_5lexer_FileLexer *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__get__", 0);
 
-  /* "kola/lexer.pyx":324
+  /* "kola/lexer.pyx":308
  *     @property
  *     def filename(self):
  *         return self._filenameo             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_self->_filenameo);
   __pyx_r = __pyx_v_self->_filenameo;
   goto __pyx_L0;
 
-  /* "kola/lexer.pyx":322
+  /* "kola/lexer.pyx":306
  *             self.fp = NULL
  * 
  *     @property             # <<<<<<<<<<<<<<
  *     def filename(self):
  *         return self._filenameo
  */
 
@@ -8563,15 +8646,15 @@
   __Pyx_AddTraceback("kola.lexer.FileLexer.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "kola/lexer.pyx":332
+/* "kola/lexer.pyx":316
  *     """
  * 
  *     def __init__(self, content: Union[str, bytes], **kwds):             # <<<<<<<<<<<<<<
  *         if not self.content is None:
  *             yypop_buffer_state(self.scanner)
  */
 
@@ -8605,31 +8688,31 @@
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
       kw_args = __Pyx_NumKwargs_VARARGS(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_VARARGS(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_content)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 332, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 316, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, __pyx_v_kwds, values + 0, kwd_pos_args, "__init__") < 0)) __PYX_ERR(1, 332, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, __pyx_v_kwds, values + 0, kwd_pos_args, "__init__") < 0)) __PYX_ERR(1, 316, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 1)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_VARARGS(__pyx_args, 0);
     }
     __pyx_v_content = values[0];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__init__", 1, 1, 1, __pyx_nargs); __PYX_ERR(1, 332, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__init__", 1, 1, 1, __pyx_nargs); __PYX_ERR(1, 316, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_DECREF(__pyx_v_kwds); __pyx_v_kwds = 0;
   __Pyx_AddTraceback("kola.lexer.StringLexer.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
   __pyx_r = __pyx_pf_4kola_5lexer_11StringLexer___init__(((struct __pyx_obj_4kola_5lexer_StringLexer *)__pyx_v_self), __pyx_v_content, __pyx_v_kwds);
@@ -8651,151 +8734,151 @@
   PyObject *__pyx_t_6 = NULL;
   PyObject *__pyx_t_7 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__init__", 0);
 
-  /* "kola/lexer.pyx":333
+  /* "kola/lexer.pyx":317
  * 
  *     def __init__(self, content: Union[str, bytes], **kwds):
  *         if not self.content is None:             # <<<<<<<<<<<<<<
  *             yypop_buffer_state(self.scanner)
  * 
  */
   __pyx_t_1 = (__pyx_v_self->content != ((PyObject*)Py_None));
   __pyx_t_2 = (__pyx_t_1 != 0);
   if (__pyx_t_2) {
 
-    /* "kola/lexer.pyx":334
+    /* "kola/lexer.pyx":318
  *     def __init__(self, content: Union[str, bytes], **kwds):
  *         if not self.content is None:
  *             yypop_buffer_state(self.scanner)             # <<<<<<<<<<<<<<
  * 
  *         if isinstance(content, str):
  */
     yypop_buffer_state(__pyx_v_self->__pyx_base.scanner);
 
-    /* "kola/lexer.pyx":333
+    /* "kola/lexer.pyx":317
  * 
  *     def __init__(self, content: Union[str, bytes], **kwds):
  *         if not self.content is None:             # <<<<<<<<<<<<<<
  *             yypop_buffer_state(self.scanner)
  * 
  */
   }
 
-  /* "kola/lexer.pyx":336
+  /* "kola/lexer.pyx":320
  *             yypop_buffer_state(self.scanner)
  * 
  *         if isinstance(content, str):             # <<<<<<<<<<<<<<
  *             self.content = (<str>content).encode()
  *         else:
  */
   __pyx_t_2 = PyUnicode_Check(__pyx_v_content); 
   __pyx_t_1 = (__pyx_t_2 != 0);
   if (__pyx_t_1) {
 
-    /* "kola/lexer.pyx":337
+    /* "kola/lexer.pyx":321
  * 
  *         if isinstance(content, str):
  *             self.content = (<str>content).encode()             # <<<<<<<<<<<<<<
  *         else:
  *             self.content = content
  */
     if (unlikely(__pyx_v_content == Py_None)) {
       PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "encode");
-      __PYX_ERR(1, 337, __pyx_L1_error)
+      __PYX_ERR(1, 321, __pyx_L1_error)
     }
-    __pyx_t_3 = PyUnicode_AsEncodedString(((PyObject*)__pyx_v_content), NULL, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 337, __pyx_L1_error)
+    __pyx_t_3 = PyUnicode_AsEncodedString(((PyObject*)__pyx_v_content), NULL, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 321, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_GIVEREF(__pyx_t_3);
     __Pyx_GOTREF(__pyx_v_self->content);
     __Pyx_DECREF(__pyx_v_self->content);
     __pyx_v_self->content = ((PyObject*)__pyx_t_3);
     __pyx_t_3 = 0;
 
-    /* "kola/lexer.pyx":336
+    /* "kola/lexer.pyx":320
  *             yypop_buffer_state(self.scanner)
  * 
  *         if isinstance(content, str):             # <<<<<<<<<<<<<<
  *             self.content = (<str>content).encode()
  *         else:
  */
     goto __pyx_L4;
   }
 
-  /* "kola/lexer.pyx":339
+  /* "kola/lexer.pyx":323
  *             self.content = (<str>content).encode()
  *         else:
  *             self.content = content             # <<<<<<<<<<<<<<
  * 
  *         yy_scan_bytes(self.content, len(self.content), self.scanner)
  */
   /*else*/ {
-    if (!(likely(PyBytes_CheckExact(__pyx_v_content))||((__pyx_v_content) == Py_None) || __Pyx_RaiseUnexpectedTypeError("bytes", __pyx_v_content))) __PYX_ERR(1, 339, __pyx_L1_error)
+    if (!(likely(PyBytes_CheckExact(__pyx_v_content))||((__pyx_v_content) == Py_None) || __Pyx_RaiseUnexpectedTypeError("bytes", __pyx_v_content))) __PYX_ERR(1, 323, __pyx_L1_error)
     __pyx_t_3 = __pyx_v_content;
     __Pyx_INCREF(__pyx_t_3);
     __Pyx_GIVEREF(__pyx_t_3);
     __Pyx_GOTREF(__pyx_v_self->content);
     __Pyx_DECREF(__pyx_v_self->content);
     __pyx_v_self->content = ((PyObject*)__pyx_t_3);
     __pyx_t_3 = 0;
   }
   __pyx_L4:;
 
-  /* "kola/lexer.pyx":341
+  /* "kola/lexer.pyx":325
  *             self.content = content
  * 
  *         yy_scan_bytes(self.content, len(self.content), self.scanner)             # <<<<<<<<<<<<<<
  *         self.lexer_data.filename = "<string>"
  *         LexerConfig(self).set(**kwds)
  */
   if (unlikely(__pyx_v_self->content == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "expected bytes, NoneType found");
-    __PYX_ERR(1, 341, __pyx_L1_error)
+    __PYX_ERR(1, 325, __pyx_L1_error)
   }
-  __pyx_t_4 = __Pyx_PyBytes_AsString(__pyx_v_self->content); if (unlikely((!__pyx_t_4) && PyErr_Occurred())) __PYX_ERR(1, 341, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyBytes_AsString(__pyx_v_self->content); if (unlikely((!__pyx_t_4) && PyErr_Occurred())) __PYX_ERR(1, 325, __pyx_L1_error)
   __pyx_t_3 = __pyx_v_self->content;
   __Pyx_INCREF(__pyx_t_3);
   if (unlikely(__pyx_t_3 == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len()");
-    __PYX_ERR(1, 341, __pyx_L1_error)
+    __PYX_ERR(1, 325, __pyx_L1_error)
   }
-  __pyx_t_5 = PyBytes_GET_SIZE(__pyx_t_3); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1))) __PYX_ERR(1, 341, __pyx_L1_error)
+  __pyx_t_5 = PyBytes_GET_SIZE(__pyx_t_3); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1))) __PYX_ERR(1, 325, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   (void)(yy_scan_bytes(__pyx_t_4, __pyx_t_5, __pyx_v_self->__pyx_base.scanner));
 
-  /* "kola/lexer.pyx":342
+  /* "kola/lexer.pyx":326
  * 
  *         yy_scan_bytes(self.content, len(self.content), self.scanner)
  *         self.lexer_data.filename = "<string>"             # <<<<<<<<<<<<<<
  *         LexerConfig(self).set(**kwds)
  */
   __pyx_v_self->__pyx_base.lexer_data.filename = ((char const *)"<string>");
 
-  /* "kola/lexer.pyx":343
+  /* "kola/lexer.pyx":327
  *         yy_scan_bytes(self.content, len(self.content), self.scanner)
  *         self.lexer_data.filename = "<string>"
  *         LexerConfig(self).set(**kwds)             # <<<<<<<<<<<<<<
  */
-  __pyx_t_3 = __Pyx_PyObject_CallOneArg(((PyObject *)__pyx_ptype_4kola_5lexer_LexerConfig), ((PyObject *)__pyx_v_self)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 343, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_CallOneArg(((PyObject *)__pyx_ptype_4kola_5lexer_LexerConfig), ((PyObject *)__pyx_v_self)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 327, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_set); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 343, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_set); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 327, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  __pyx_t_3 = PyDict_Copy(__pyx_v_kwds); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 343, __pyx_L1_error)
+  __pyx_t_3 = PyDict_Copy(__pyx_v_kwds); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 327, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_7 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_empty_tuple, __pyx_t_3); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 343, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyObject_Call(__pyx_t_6, __pyx_empty_tuple, __pyx_t_3); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 327, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-  /* "kola/lexer.pyx":332
+  /* "kola/lexer.pyx":316
  *     """
  * 
  *     def __init__(self, content: Union[str, bytes], **kwds):             # <<<<<<<<<<<<<<
  *         if not self.content is None:
  *             yypop_buffer_state(self.scanner)
  */
 
@@ -8809,15 +8892,15 @@
   __Pyx_AddTraceback("kola.lexer.StringLexer.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "kola/lexer.pxd":54
+/* "kola/lexer.pxd":50
  * @cython.no_gc
  * cdef class StringLexer(BaseLexer):
  *     cdef readonly bytes content             # <<<<<<<<<<<<<<
  */
 
 /* Python wrapper */
 static PyObject *__pyx_pw_4kola_5lexer_11StringLexer_7content_1__get__(PyObject *__pyx_v_self); /*proto*/
@@ -10317,14 +10400,15 @@
     #define CYTHON_SMALL_CODE
 #endif
 #endif
 /* #### Code section: pystring_table ### */
 
 static __Pyx_StringTabEntry __pyx_string_tab[] = {
   #if CYTHON_USE_MODULE_STATE
+  {0, __pyx_k_, sizeof(__pyx_k_), 0, 1, 0, 1},
   {0, __pyx_k_AttributeError, sizeof(__pyx_k_AttributeError), 0, 0, 1, 1},
   {0, __pyx_k_BaseLexer, sizeof(__pyx_k_BaseLexer), 0, 0, 1, 1},
   {0, __pyx_k_BaseLexer___enter, sizeof(__pyx_k_BaseLexer___enter), 0, 0, 1, 1},
   {0, __pyx_k_BaseLexer___exit, sizeof(__pyx_k_BaseLexer___exit), 0, 0, 1, 1},
   {0, __pyx_k_BaseLexer___reduce_cython, sizeof(__pyx_k_BaseLexer___reduce_cython), 0, 0, 1, 1},
   {0, __pyx_k_BaseLexer___setstate_cython, sizeof(__pyx_k_BaseLexer___setstate_cython), 0, 0, 1, 1},
   {0, __pyx_k_BaseLexer_close, sizeof(__pyx_k_BaseLexer_close), 0, 0, 1, 1},
@@ -10363,34 +10447,37 @@
   {0, __pyx_k_StringLexer___reduce_cython, sizeof(__pyx_k_StringLexer___reduce_cython), 0, 0, 1, 1},
   {0, __pyx_k_StringLexer___setstate_cython, sizeof(__pyx_k_StringLexer___setstate_cython), 0, 0, 1, 1},
   {0, __pyx_k_Token, sizeof(__pyx_k_Token), 0, 0, 1, 1},
   {0, __pyx_k_Token___reduce_cython, sizeof(__pyx_k_Token___reduce_cython), 0, 0, 1, 1},
   {0, __pyx_k_Token___setstate_cython, sizeof(__pyx_k_Token___setstate_cython), 0, 0, 1, 1},
   {0, __pyx_k_Token_get_flag, sizeof(__pyx_k_Token_get_flag), 0, 0, 1, 1},
   {0, __pyx_k_TypeError, sizeof(__pyx_k_TypeError), 0, 0, 1, 1},
-  {0, __pyx_k__14, sizeof(__pyx_k__14), 0, 1, 0, 1},
-  {0, __pyx_k__2, sizeof(__pyx_k__2), 0, 1, 0, 0},
   {0, __pyx_k__26, sizeof(__pyx_k__26), 0, 0, 1, 1},
+  {0, __pyx_k__3, sizeof(__pyx_k__3), 0, 1, 0, 0},
   {0, __pyx_k_args, sizeof(__pyx_k_args), 0, 0, 1, 1},
   {0, __pyx_k_asyncio_coroutines, sizeof(__pyx_k_asyncio_coroutines), 0, 0, 1, 1},
   {0, __pyx_k_cline_in_traceback, sizeof(__pyx_k_cline_in_traceback), 0, 0, 1, 1},
   {0, __pyx_k_close, sizeof(__pyx_k_close), 0, 0, 1, 1},
+  {0, __pyx_k_command_threshold, sizeof(__pyx_k_command_threshold), 0, 0, 1, 1},
   {0, __pyx_k_content, sizeof(__pyx_k_content), 0, 0, 1, 1},
   {0, __pyx_k_data, sizeof(__pyx_k_data), 0, 0, 1, 1},
-  {0, __pyx_k_data_names, sizeof(__pyx_k_data_names), 0, 1, 0, 1},
   {0, __pyx_k_dict, sizeof(__pyx_k_dict), 0, 0, 1, 1},
   {0, __pyx_k_disable, sizeof(__pyx_k_disable), 0, 1, 0, 0},
   {0, __pyx_k_enable, sizeof(__pyx_k_enable), 0, 1, 0, 0},
+  {0, __pyx_k_encoding, sizeof(__pyx_k_encoding), 0, 1, 0, 1},
+  {0, __pyx_k_endswith, sizeof(__pyx_k_endswith), 0, 0, 1, 1},
   {0, __pyx_k_enter, sizeof(__pyx_k_enter), 0, 0, 1, 1},
   {0, __pyx_k_exception, sizeof(__pyx_k_exception), 0, 0, 1, 1},
   {0, __pyx_k_exit, sizeof(__pyx_k_exit), 0, 0, 1, 1},
+  {0, __pyx_k_filename, sizeof(__pyx_k_filename), 0, 0, 1, 1},
+  {0, __pyx_k_filename, sizeof(__pyx_k_filename), 0, 1, 0, 1},
+  {0, __pyx_k_flag, sizeof(__pyx_k_flag), 0, 0, 1, 1},
   {0, __pyx_k_gc, sizeof(__pyx_k_gc), 0, 1, 0, 0},
   {0, __pyx_k_get_flag, sizeof(__pyx_k_get_flag), 0, 0, 1, 1},
   {0, __pyx_k_getstate, sizeof(__pyx_k_getstate), 0, 0, 1, 1},
-  {0, __pyx_k_i, sizeof(__pyx_k_i), 0, 0, 1, 1},
   {0, __pyx_k_import, sizeof(__pyx_k_import), 0, 0, 1, 1},
   {0, __pyx_k_is_coroutine, sizeof(__pyx_k_is_coroutine), 0, 0, 1, 1},
   {0, __pyx_k_isenabled, sizeof(__pyx_k_isenabled), 0, 1, 0, 0},
   {0, __pyx_k_items, sizeof(__pyx_k_items), 0, 0, 1, 1},
   {0, __pyx_k_k, sizeof(__pyx_k_k), 0, 0, 1, 1},
   {0, __pyx_k_kola_lexer, sizeof(__pyx_k_kola_lexer), 0, 0, 1, 1},
   {0, __pyx_k_kola_lexer_pyx, sizeof(__pyx_k_kola_lexer_pyx), 0, 0, 1, 0},
@@ -10409,21 +10496,23 @@
   {0, __pyx_k_reduce_ex, sizeof(__pyx_k_reduce_ex), 0, 0, 1, 1},
   {0, __pyx_k_return, sizeof(__pyx_k_return), 0, 0, 1, 1},
   {0, __pyx_k_self, sizeof(__pyx_k_self), 0, 0, 1, 1},
   {0, __pyx_k_self_lexer_data_cannot_be_conver, sizeof(__pyx_k_self_lexer_data_cannot_be_conver), 0, 0, 1, 0},
   {0, __pyx_k_set, sizeof(__pyx_k_set), 0, 0, 1, 1},
   {0, __pyx_k_setstate, sizeof(__pyx_k_setstate), 0, 0, 1, 1},
   {0, __pyx_k_setstate_cython, sizeof(__pyx_k_setstate_cython), 0, 0, 1, 1},
+  {0, __pyx_k_startswith, sizeof(__pyx_k_startswith), 0, 0, 1, 1},
   {0, __pyx_k_stringsource, sizeof(__pyx_k_stringsource), 0, 0, 1, 0},
   {0, __pyx_k_syn, sizeof(__pyx_k_syn), 0, 0, 1, 1},
   {0, __pyx_k_test, sizeof(__pyx_k_test), 0, 0, 1, 1},
   {0, __pyx_k_utf_8, sizeof(__pyx_k_utf_8), 0, 1, 0, 0},
   {0, __pyx_k_v, sizeof(__pyx_k_v), 0, 0, 1, 1},
   {0, __pyx_k_val, sizeof(__pyx_k_val), 0, 0, 1, 1},
   #else
+  {&__pyx_n_u_, __pyx_k_, sizeof(__pyx_k_), 0, 1, 0, 1},
   {&__pyx_n_s_AttributeError, __pyx_k_AttributeError, sizeof(__pyx_k_AttributeError), 0, 0, 1, 1},
   {&__pyx_n_s_BaseLexer, __pyx_k_BaseLexer, sizeof(__pyx_k_BaseLexer), 0, 0, 1, 1},
   {&__pyx_n_s_BaseLexer___enter, __pyx_k_BaseLexer___enter, sizeof(__pyx_k_BaseLexer___enter), 0, 0, 1, 1},
   {&__pyx_n_s_BaseLexer___exit, __pyx_k_BaseLexer___exit, sizeof(__pyx_k_BaseLexer___exit), 0, 0, 1, 1},
   {&__pyx_n_s_BaseLexer___reduce_cython, __pyx_k_BaseLexer___reduce_cython, sizeof(__pyx_k_BaseLexer___reduce_cython), 0, 0, 1, 1},
   {&__pyx_n_s_BaseLexer___setstate_cython, __pyx_k_BaseLexer___setstate_cython, sizeof(__pyx_k_BaseLexer___setstate_cython), 0, 0, 1, 1},
   {&__pyx_n_s_BaseLexer_close, __pyx_k_BaseLexer_close, sizeof(__pyx_k_BaseLexer_close), 0, 0, 1, 1},
@@ -10462,34 +10551,37 @@
   {&__pyx_n_s_StringLexer___reduce_cython, __pyx_k_StringLexer___reduce_cython, sizeof(__pyx_k_StringLexer___reduce_cython), 0, 0, 1, 1},
   {&__pyx_n_s_StringLexer___setstate_cython, __pyx_k_StringLexer___setstate_cython, sizeof(__pyx_k_StringLexer___setstate_cython), 0, 0, 1, 1},
   {&__pyx_n_s_Token, __pyx_k_Token, sizeof(__pyx_k_Token), 0, 0, 1, 1},
   {&__pyx_n_s_Token___reduce_cython, __pyx_k_Token___reduce_cython, sizeof(__pyx_k_Token___reduce_cython), 0, 0, 1, 1},
   {&__pyx_n_s_Token___setstate_cython, __pyx_k_Token___setstate_cython, sizeof(__pyx_k_Token___setstate_cython), 0, 0, 1, 1},
   {&__pyx_n_s_Token_get_flag, __pyx_k_Token_get_flag, sizeof(__pyx_k_Token_get_flag), 0, 0, 1, 1},
   {&__pyx_n_s_TypeError, __pyx_k_TypeError, sizeof(__pyx_k_TypeError), 0, 0, 1, 1},
-  {&__pyx_n_u__14, __pyx_k__14, sizeof(__pyx_k__14), 0, 1, 0, 1},
-  {&__pyx_kp_u__2, __pyx_k__2, sizeof(__pyx_k__2), 0, 1, 0, 0},
   {&__pyx_n_s__26, __pyx_k__26, sizeof(__pyx_k__26), 0, 0, 1, 1},
+  {&__pyx_kp_u__3, __pyx_k__3, sizeof(__pyx_k__3), 0, 1, 0, 0},
   {&__pyx_n_s_args, __pyx_k_args, sizeof(__pyx_k_args), 0, 0, 1, 1},
   {&__pyx_n_s_asyncio_coroutines, __pyx_k_asyncio_coroutines, sizeof(__pyx_k_asyncio_coroutines), 0, 0, 1, 1},
   {&__pyx_n_s_cline_in_traceback, __pyx_k_cline_in_traceback, sizeof(__pyx_k_cline_in_traceback), 0, 0, 1, 1},
   {&__pyx_n_s_close, __pyx_k_close, sizeof(__pyx_k_close), 0, 0, 1, 1},
+  {&__pyx_n_s_command_threshold, __pyx_k_command_threshold, sizeof(__pyx_k_command_threshold), 0, 0, 1, 1},
   {&__pyx_n_s_content, __pyx_k_content, sizeof(__pyx_k_content), 0, 0, 1, 1},
   {&__pyx_n_s_data, __pyx_k_data, sizeof(__pyx_k_data), 0, 0, 1, 1},
-  {&__pyx_n_u_data_names, __pyx_k_data_names, sizeof(__pyx_k_data_names), 0, 1, 0, 1},
   {&__pyx_n_s_dict, __pyx_k_dict, sizeof(__pyx_k_dict), 0, 0, 1, 1},
   {&__pyx_kp_u_disable, __pyx_k_disable, sizeof(__pyx_k_disable), 0, 1, 0, 0},
   {&__pyx_kp_u_enable, __pyx_k_enable, sizeof(__pyx_k_enable), 0, 1, 0, 0},
+  {&__pyx_n_u_encoding, __pyx_k_encoding, sizeof(__pyx_k_encoding), 0, 1, 0, 1},
+  {&__pyx_n_s_endswith, __pyx_k_endswith, sizeof(__pyx_k_endswith), 0, 0, 1, 1},
   {&__pyx_n_s_enter, __pyx_k_enter, sizeof(__pyx_k_enter), 0, 0, 1, 1},
   {&__pyx_n_s_exception, __pyx_k_exception, sizeof(__pyx_k_exception), 0, 0, 1, 1},
   {&__pyx_n_s_exit, __pyx_k_exit, sizeof(__pyx_k_exit), 0, 0, 1, 1},
+  {&__pyx_n_s_filename, __pyx_k_filename, sizeof(__pyx_k_filename), 0, 0, 1, 1},
+  {&__pyx_n_u_filename, __pyx_k_filename, sizeof(__pyx_k_filename), 0, 1, 0, 1},
+  {&__pyx_n_s_flag, __pyx_k_flag, sizeof(__pyx_k_flag), 0, 0, 1, 1},
   {&__pyx_kp_u_gc, __pyx_k_gc, sizeof(__pyx_k_gc), 0, 1, 0, 0},
   {&__pyx_n_s_get_flag, __pyx_k_get_flag, sizeof(__pyx_k_get_flag), 0, 0, 1, 1},
   {&__pyx_n_s_getstate, __pyx_k_getstate, sizeof(__pyx_k_getstate), 0, 0, 1, 1},
-  {&__pyx_n_s_i, __pyx_k_i, sizeof(__pyx_k_i), 0, 0, 1, 1},
   {&__pyx_n_s_import, __pyx_k_import, sizeof(__pyx_k_import), 0, 0, 1, 1},
   {&__pyx_n_s_is_coroutine, __pyx_k_is_coroutine, sizeof(__pyx_k_is_coroutine), 0, 0, 1, 1},
   {&__pyx_kp_u_isenabled, __pyx_k_isenabled, sizeof(__pyx_k_isenabled), 0, 1, 0, 0},
   {&__pyx_n_s_items, __pyx_k_items, sizeof(__pyx_k_items), 0, 0, 1, 1},
   {&__pyx_n_s_k, __pyx_k_k, sizeof(__pyx_k_k), 0, 0, 1, 1},
   {&__pyx_n_s_kola_lexer, __pyx_k_kola_lexer, sizeof(__pyx_k_kola_lexer), 0, 0, 1, 1},
   {&__pyx_kp_s_kola_lexer_pyx, __pyx_k_kola_lexer_pyx, sizeof(__pyx_k_kola_lexer_pyx), 0, 0, 1, 0},
@@ -10508,311 +10600,317 @@
   {&__pyx_n_s_reduce_ex, __pyx_k_reduce_ex, sizeof(__pyx_k_reduce_ex), 0, 0, 1, 1},
   {&__pyx_n_s_return, __pyx_k_return, sizeof(__pyx_k_return), 0, 0, 1, 1},
   {&__pyx_n_s_self, __pyx_k_self, sizeof(__pyx_k_self), 0, 0, 1, 1},
   {&__pyx_kp_s_self_lexer_data_cannot_be_conver, __pyx_k_self_lexer_data_cannot_be_conver, sizeof(__pyx_k_self_lexer_data_cannot_be_conver), 0, 0, 1, 0},
   {&__pyx_n_s_set, __pyx_k_set, sizeof(__pyx_k_set), 0, 0, 1, 1},
   {&__pyx_n_s_setstate, __pyx_k_setstate, sizeof(__pyx_k_setstate), 0, 0, 1, 1},
   {&__pyx_n_s_setstate_cython, __pyx_k_setstate_cython, sizeof(__pyx_k_setstate_cython), 0, 0, 1, 1},
+  {&__pyx_n_s_startswith, __pyx_k_startswith, sizeof(__pyx_k_startswith), 0, 0, 1, 1},
   {&__pyx_kp_s_stringsource, __pyx_k_stringsource, sizeof(__pyx_k_stringsource), 0, 0, 1, 0},
   {&__pyx_n_s_syn, __pyx_k_syn, sizeof(__pyx_k_syn), 0, 0, 1, 1},
   {&__pyx_n_s_test, __pyx_k_test, sizeof(__pyx_k_test), 0, 0, 1, 1},
   {&__pyx_kp_u_utf_8, __pyx_k_utf_8, sizeof(__pyx_k_utf_8), 0, 1, 0, 0},
   {&__pyx_n_s_v, __pyx_k_v, sizeof(__pyx_k_v), 0, 0, 1, 1},
   {&__pyx_n_s_val, __pyx_k_val, sizeof(__pyx_k_val), 0, 0, 1, 1},
   #endif
   {0, 0, 0, 0, 0, 0, 0}
 };
 /* #### Code section: cached_builtins ### */
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
   __pyx_builtin_TypeError = __Pyx_GetBuiltinName(__pyx_n_s_TypeError); if (!__pyx_builtin_TypeError) __PYX_ERR(0, 2, __pyx_L1_error)
-  __pyx_builtin_AttributeError = __Pyx_GetBuiltinName(__pyx_n_s_AttributeError); if (!__pyx_builtin_AttributeError) __PYX_ERR(1, 97, __pyx_L1_error)
-  __pyx_builtin_RuntimeError = __Pyx_GetBuiltinName(__pyx_n_s_RuntimeError); if (!__pyx_builtin_RuntimeError) __PYX_ERR(1, 171, __pyx_L1_error)
-  __pyx_builtin_OSError = __Pyx_GetBuiltinName(__pyx_n_s_OSError); if (!__pyx_builtin_OSError) __PYX_ERR(1, 203, __pyx_L1_error)
-  __pyx_builtin_StopIteration = __Pyx_GetBuiltinName(__pyx_n_s_StopIteration); if (!__pyx_builtin_StopIteration) __PYX_ERR(1, 273, __pyx_L1_error)
+  __pyx_builtin_AttributeError = __Pyx_GetBuiltinName(__pyx_n_s_AttributeError); if (!__pyx_builtin_AttributeError) __PYX_ERR(1, 94, __pyx_L1_error)
+  __pyx_builtin_RuntimeError = __Pyx_GetBuiltinName(__pyx_n_s_RuntimeError); if (!__pyx_builtin_RuntimeError) __PYX_ERR(1, 158, __pyx_L1_error)
+  __pyx_builtin_OSError = __Pyx_GetBuiltinName(__pyx_n_s_OSError); if (!__pyx_builtin_OSError) __PYX_ERR(1, 190, __pyx_L1_error)
+  __pyx_builtin_StopIteration = __Pyx_GetBuiltinName(__pyx_n_s_StopIteration); if (!__pyx_builtin_StopIteration) __PYX_ERR(1, 260, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
 /* #### Code section: cached_constants ### */
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "kola/lexer.pyx":203
+  /* "kola/lexer.pyx":190
  *     cdef Token next_token(self):
  *         if not yylex_check(self.scanner):
  *             raise OSError("operation on closed lexer")             # <<<<<<<<<<<<<<
  * 
  *         cdef:
  */
-  __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_u_operation_on_closed_lexer); if (unlikely(!__pyx_tuple_)) __PYX_ERR(1, 203, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple_);
-  __Pyx_GIVEREF(__pyx_tuple_);
+  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_u_operation_on_closed_lexer); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(1, 190, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__2);
+  __Pyx_GIVEREF(__pyx_tuple__2);
 
-  /* "kola/lexer.pyx":62
+  /* "kola/lexer.pyx":59
  *         return self is other or self.syn == other
  * 
  *     cpdef int get_flag(self):             # <<<<<<<<<<<<<<
  *         if self.syn <= TEXT or self.syn == ANNOTATION:
  *             return 0
  */
-  __pyx_tuple__3 = PyTuple_Pack(1, __pyx_n_s_self); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(1, 62, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__3);
-  __Pyx_GIVEREF(__pyx_tuple__3);
-  __pyx_codeobj__4 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__3, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_kola_lexer_pyx, __pyx_n_s_get_flag, 62, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__4)) __PYX_ERR(1, 62, __pyx_L1_error)
+  __pyx_tuple__4 = PyTuple_Pack(1, __pyx_n_s_self); if (unlikely(!__pyx_tuple__4)) __PYX_ERR(1, 59, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__4);
+  __Pyx_GIVEREF(__pyx_tuple__4);
+  __pyx_codeobj__5 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__4, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_kola_lexer_pyx, __pyx_n_s_get_flag, 59, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__5)) __PYX_ERR(1, 59, __pyx_L1_error)
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  * def __setstate_cython__(self, __pyx_state):
  */
-  __pyx_codeobj__5 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__3, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_reduce_cython, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__5)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_codeobj__6 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__4, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_reduce_cython, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__6)) __PYX_ERR(0, 1, __pyx_L1_error)
 
   /* "(tree fragment)":3
  * def __reduce_cython__(self):
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  */
-  __pyx_tuple__6 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_pyx_state); if (unlikely(!__pyx_tuple__6)) __PYX_ERR(0, 3, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__6);
-  __Pyx_GIVEREF(__pyx_tuple__6);
-  __pyx_codeobj__7 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__6, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_setstate_cython, 3, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__7)) __PYX_ERR(0, 3, __pyx_L1_error)
+  __pyx_tuple__7 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_pyx_state); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(0, 3, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__7);
+  __Pyx_GIVEREF(__pyx_tuple__7);
+  __pyx_codeobj__8 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__7, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_setstate_cython, 3, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__8)) __PYX_ERR(0, 3, __pyx_L1_error)
 
-  /* "kola/lexer.pyx":88
+  /* "kola/lexer.pyx":85
  *         self.lexer_data = &lexer.lexer_data
  * 
  *     def dict(self) -> dict:             # <<<<<<<<<<<<<<
- *         cdef dict data = {}
- *         for i in _lexer_data_names:
+ *         cdef dict data = <dict>self.lexer_data[0]
+ *         data["filename"] = (<bytes>data["filename"]).decode()
  */
-  __pyx_tuple__8 = PyTuple_Pack(3, __pyx_n_s_self, __pyx_n_s_data, __pyx_n_s_i); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(1, 88, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__8);
-  __Pyx_GIVEREF(__pyx_tuple__8);
-  __pyx_codeobj__9 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__8, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_kola_lexer_pyx, __pyx_n_s_dict, 88, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__9)) __PYX_ERR(1, 88, __pyx_L1_error)
+  __pyx_tuple__9 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_data); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(1, 85, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__9);
+  __Pyx_GIVEREF(__pyx_tuple__9);
+  __pyx_codeobj__10 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__9, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_kola_lexer_pyx, __pyx_n_s_dict, 85, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__10)) __PYX_ERR(1, 85, __pyx_L1_error)
 
-  /* "kola/lexer.pyx":94
+  /* "kola/lexer.pyx":91
  *         return data
  * 
  *     def set(self, **kwds) -> None:             # <<<<<<<<<<<<<<
  *         for k, v in kwds.items():
- *             if not k in _lexer_data_names:
+ *             if k.startswith('__') and k.endswith('__'):
  */
-  __pyx_tuple__10 = PyTuple_Pack(4, __pyx_n_s_self, __pyx_n_s_kwds, __pyx_n_s_k, __pyx_n_s_v); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(1, 94, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__10);
-  __Pyx_GIVEREF(__pyx_tuple__10);
-  __pyx_codeobj__11 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS|CO_VARKEYWORDS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__10, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_kola_lexer_pyx, __pyx_n_s_set, 94, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__11)) __PYX_ERR(1, 94, __pyx_L1_error)
+  __pyx_tuple__11 = PyTuple_Pack(4, __pyx_n_s_self, __pyx_n_s_kwds, __pyx_n_s_k, __pyx_n_s_v); if (unlikely(!__pyx_tuple__11)) __PYX_ERR(1, 91, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__11);
+  __Pyx_GIVEREF(__pyx_tuple__11);
+  __pyx_codeobj__12 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS|CO_VARKEYWORDS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__11, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_kola_lexer_pyx, __pyx_n_s_set, 91, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__12)) __PYX_ERR(1, 91, __pyx_L1_error)
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     raise TypeError, "self.lexer_data cannot be converted to a Python object for pickling"
  * def __setstate_cython__(self, __pyx_state):
  */
-  __pyx_codeobj__12 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__3, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_reduce_cython, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__12)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_codeobj__13 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__4, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_reduce_cython, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__13)) __PYX_ERR(0, 1, __pyx_L1_error)
 
   /* "(tree fragment)":3
  * def __reduce_cython__(self):
  *     raise TypeError, "self.lexer_data cannot be converted to a Python object for pickling"
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     raise TypeError, "self.lexer_data cannot be converted to a Python object for pickling"
  */
-  __pyx_codeobj__13 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__6, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_setstate_cython, 3, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__13)) __PYX_ERR(0, 3, __pyx_L1_error)
+  __pyx_codeobj__14 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__7, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_setstate_cython, 3, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__14)) __PYX_ERR(0, 3, __pyx_L1_error)
 
-  /* "kola/lexer.pyx":183
+  /* "kola/lexer.pyx":170
  *             yylex_destroy(self.scanner)
  * 
  *     cpdef void close(self):             # <<<<<<<<<<<<<<
  *         yypop_buffer_state(self.scanner)
  * 
  */
-  __pyx_codeobj__15 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__3, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_kola_lexer_pyx, __pyx_n_s_close, 183, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__15)) __PYX_ERR(1, 183, __pyx_L1_error)
+  __pyx_codeobj__15 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__4, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_kola_lexer_pyx, __pyx_n_s_close, 170, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__15)) __PYX_ERR(1, 170, __pyx_L1_error)
 
-  /* "kola/lexer.pyx":276
+  /* "kola/lexer.pyx":263
  *         return token
  * 
  *     def __enter__(self):             # <<<<<<<<<<<<<<
  *         return self
  * 
  */
-  __pyx_codeobj__16 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__3, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_kola_lexer_pyx, __pyx_n_s_enter, 276, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__16)) __PYX_ERR(1, 276, __pyx_L1_error)
+  __pyx_codeobj__16 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__4, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_kola_lexer_pyx, __pyx_n_s_enter, 263, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__16)) __PYX_ERR(1, 263, __pyx_L1_error)
 
-  /* "kola/lexer.pyx":279
+  /* "kola/lexer.pyx":266
  *         return self
  * 
  *     def __exit__(self, *args):             # <<<<<<<<<<<<<<
  *         self.close()
  * 
  */
-  __pyx_tuple__17 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_args); if (unlikely(!__pyx_tuple__17)) __PYX_ERR(1, 279, __pyx_L1_error)
+  __pyx_tuple__17 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_args); if (unlikely(!__pyx_tuple__17)) __PYX_ERR(1, 266, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__17);
   __Pyx_GIVEREF(__pyx_tuple__17);
-  __pyx_codeobj__18 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS|CO_VARARGS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__17, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_kola_lexer_pyx, __pyx_n_s_exit, 279, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__18)) __PYX_ERR(1, 279, __pyx_L1_error)
+  __pyx_codeobj__18 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS|CO_VARARGS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__17, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_kola_lexer_pyx, __pyx_n_s_exit, 266, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__18)) __PYX_ERR(1, 266, __pyx_L1_error)
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  * def __setstate_cython__(self, __pyx_state):
  */
-  __pyx_codeobj__19 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__3, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_reduce_cython, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__19)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_codeobj__19 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__4, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_reduce_cython, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__19)) __PYX_ERR(0, 1, __pyx_L1_error)
 
   /* "(tree fragment)":3
  * def __reduce_cython__(self):
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  */
-  __pyx_codeobj__20 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__6, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_setstate_cython, 3, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__20)) __PYX_ERR(0, 3, __pyx_L1_error)
+  __pyx_codeobj__20 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__7, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_setstate_cython, 3, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__20)) __PYX_ERR(0, 3, __pyx_L1_error)
 
-  /* "kola/lexer.pyx":316
+  /* "kola/lexer.pyx":300
  *         LexerConfig(self).set(**kwds)
  * 
  *     cpdef void close(self):             # <<<<<<<<<<<<<<
  *         BaseLexer.close(self)
  *         if self.fp:
  */
-  __pyx_codeobj__21 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__3, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_kola_lexer_pyx, __pyx_n_s_close, 316, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__21)) __PYX_ERR(1, 316, __pyx_L1_error)
+  __pyx_codeobj__21 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__4, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_kola_lexer_pyx, __pyx_n_s_close, 300, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__21)) __PYX_ERR(1, 300, __pyx_L1_error)
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  * def __setstate_cython__(self, __pyx_state):
  */
-  __pyx_codeobj__22 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__3, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_reduce_cython, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__22)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_codeobj__22 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__4, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_reduce_cython, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__22)) __PYX_ERR(0, 1, __pyx_L1_error)
 
   /* "(tree fragment)":3
  * def __reduce_cython__(self):
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  */
-  __pyx_codeobj__23 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__6, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_setstate_cython, 3, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__23)) __PYX_ERR(0, 3, __pyx_L1_error)
+  __pyx_codeobj__23 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__7, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_setstate_cython, 3, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__23)) __PYX_ERR(0, 3, __pyx_L1_error)
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  * def __setstate_cython__(self, __pyx_state):
  */
-  __pyx_codeobj__24 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__3, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_reduce_cython, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__24)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_codeobj__24 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 1, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__4, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_reduce_cython, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__24)) __PYX_ERR(0, 1, __pyx_L1_error)
 
   /* "(tree fragment)":3
  * def __reduce_cython__(self):
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  */
-  __pyx_codeobj__25 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__6, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_setstate_cython, 3, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__25)) __PYX_ERR(0, 3, __pyx_L1_error)
+  __pyx_codeobj__25 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__7, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_setstate_cython, 3, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__25)) __PYX_ERR(0, 3, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 /* #### Code section: init_constants ### */
 
 static CYTHON_SMALL_CODE int __Pyx_InitConstants(void) {
   #if CYTHON_USE_MODULE_STATE
-  if (__Pyx_InitString(__pyx_string_tab[0], &__pyx_n_s_AttributeError) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[1], &__pyx_n_s_BaseLexer) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[2], &__pyx_n_s_BaseLexer___enter) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[3], &__pyx_n_s_BaseLexer___exit) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[4], &__pyx_n_s_BaseLexer___reduce_cython) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[5], &__pyx_n_s_BaseLexer___setstate_cython) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[6], &__pyx_n_s_BaseLexer_close) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[7], &__pyx_n_s_F_DISABLED) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[8], &__pyx_n_s_F_LSTRIP_TEXT) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[9], &__pyx_n_s_FileLexer) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[10], &__pyx_n_s_FileLexer___reduce_cython) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[11], &__pyx_n_s_FileLexer___setstate_cython) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[12], &__pyx_n_s_FileLexer__path) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[13], &__pyx_n_s_FileLexer_close) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[14], &__pyx_n_s_KoiLangSyntaxError) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[15], &__pyx_n_s_LexerConfig) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[16], &__pyx_n_s_LexerConfig___reduce_cython) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[17], &__pyx_n_s_LexerConfig___setstate_cython) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[18], &__pyx_n_s_LexerConfig_dict) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[19], &__pyx_n_s_LexerConfig_set) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[20], &__pyx_n_s_None) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[21], &__pyx_n_s_OSError) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[22], &__pyx_n_s_RuntimeError) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[23], &__pyx_n_s_S_ANNOTATION) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[24], &__pyx_n_s_S_CLN) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[25], &__pyx_n_s_S_CMA) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[26], &__pyx_n_s_S_CMD) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[27], &__pyx_n_s_S_CMD_N) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[28], &__pyx_n_s_S_LITERAL) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[29], &__pyx_n_s_S_NUM) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[30], &__pyx_n_s_S_NUM_B) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[31], &__pyx_n_s_S_NUM_F) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[32], &__pyx_n_s_S_NUM_H) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[33], &__pyx_n_s_S_SLP) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[34], &__pyx_n_s_S_SRP) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[35], &__pyx_n_s_S_STRING) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[36], &__pyx_n_s_S_TEXT) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[37], &__pyx_n_s_StopIteration) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[38], &__pyx_n_s_StringLexer) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[39], &__pyx_n_s_StringLexer___reduce_cython) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[40], &__pyx_n_s_StringLexer___setstate_cython) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[41], &__pyx_n_s_Token) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[42], &__pyx_n_s_Token___reduce_cython) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[43], &__pyx_n_s_Token___setstate_cython) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[44], &__pyx_n_s_Token_get_flag) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[45], &__pyx_n_s_TypeError) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[46], &__pyx_n_u__14) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[47], &__pyx_kp_u__2) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[48], &__pyx_n_s__26) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[0], &__pyx_n_u_) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[1], &__pyx_n_s_AttributeError) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[2], &__pyx_n_s_BaseLexer) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[3], &__pyx_n_s_BaseLexer___enter) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[4], &__pyx_n_s_BaseLexer___exit) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[5], &__pyx_n_s_BaseLexer___reduce_cython) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[6], &__pyx_n_s_BaseLexer___setstate_cython) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[7], &__pyx_n_s_BaseLexer_close) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[8], &__pyx_n_s_F_DISABLED) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[9], &__pyx_n_s_F_LSTRIP_TEXT) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[10], &__pyx_n_s_FileLexer) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[11], &__pyx_n_s_FileLexer___reduce_cython) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[12], &__pyx_n_s_FileLexer___setstate_cython) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[13], &__pyx_n_s_FileLexer__path) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[14], &__pyx_n_s_FileLexer_close) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[15], &__pyx_n_s_KoiLangSyntaxError) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[16], &__pyx_n_s_LexerConfig) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[17], &__pyx_n_s_LexerConfig___reduce_cython) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[18], &__pyx_n_s_LexerConfig___setstate_cython) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[19], &__pyx_n_s_LexerConfig_dict) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[20], &__pyx_n_s_LexerConfig_set) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[21], &__pyx_n_s_None) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[22], &__pyx_n_s_OSError) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[23], &__pyx_n_s_RuntimeError) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[24], &__pyx_n_s_S_ANNOTATION) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[25], &__pyx_n_s_S_CLN) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[26], &__pyx_n_s_S_CMA) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[27], &__pyx_n_s_S_CMD) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[28], &__pyx_n_s_S_CMD_N) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[29], &__pyx_n_s_S_LITERAL) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[30], &__pyx_n_s_S_NUM) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[31], &__pyx_n_s_S_NUM_B) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[32], &__pyx_n_s_S_NUM_F) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[33], &__pyx_n_s_S_NUM_H) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[34], &__pyx_n_s_S_SLP) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[35], &__pyx_n_s_S_SRP) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[36], &__pyx_n_s_S_STRING) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[37], &__pyx_n_s_S_TEXT) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[38], &__pyx_n_s_StopIteration) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[39], &__pyx_n_s_StringLexer) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[40], &__pyx_n_s_StringLexer___reduce_cython) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[41], &__pyx_n_s_StringLexer___setstate_cython) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[42], &__pyx_n_s_Token) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[43], &__pyx_n_s_Token___reduce_cython) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[44], &__pyx_n_s_Token___setstate_cython) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[45], &__pyx_n_s_Token_get_flag) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[46], &__pyx_n_s_TypeError) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[47], &__pyx_n_s__26) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[48], &__pyx_kp_u__3) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
   if (__Pyx_InitString(__pyx_string_tab[49], &__pyx_n_s_args) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
   if (__Pyx_InitString(__pyx_string_tab[50], &__pyx_n_s_asyncio_coroutines) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
   if (__Pyx_InitString(__pyx_string_tab[51], &__pyx_n_s_cline_in_traceback) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
   if (__Pyx_InitString(__pyx_string_tab[52], &__pyx_n_s_close) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[53], &__pyx_n_s_content) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[54], &__pyx_n_s_data) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[55], &__pyx_n_u_data_names) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[53], &__pyx_n_s_command_threshold) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[54], &__pyx_n_s_content) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[55], &__pyx_n_s_data) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
   if (__Pyx_InitString(__pyx_string_tab[56], &__pyx_n_s_dict) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
   if (__Pyx_InitString(__pyx_string_tab[57], &__pyx_kp_u_disable) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
   if (__Pyx_InitString(__pyx_string_tab[58], &__pyx_kp_u_enable) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[59], &__pyx_n_s_enter) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[60], &__pyx_n_s_exception) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[61], &__pyx_n_s_exit) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[62], &__pyx_kp_u_gc) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[63], &__pyx_n_s_get_flag) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[64], &__pyx_n_s_getstate) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[65], &__pyx_n_s_i) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[66], &__pyx_n_s_import) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[67], &__pyx_n_s_is_coroutine) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[68], &__pyx_kp_u_isenabled) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[69], &__pyx_n_s_items) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[70], &__pyx_n_s_k) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[71], &__pyx_n_s_kola_lexer) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[72], &__pyx_kp_s_kola_lexer_pyx) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[73], &__pyx_n_s_kwds) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[74], &__pyx_n_s_lexer) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[75], &__pyx_n_s_lineno) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[76], &__pyx_n_s_main) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[77], &__pyx_n_s_name) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[78], &__pyx_kp_s_no_default___reduce___due_to_non) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[79], &__pyx_kp_u_operation_on_closed_lexer) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[80], &__pyx_n_s_pyx_state) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[81], &__pyx_n_s_pyx_vtable) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[82], &__pyx_n_s_raw_val) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[83], &__pyx_n_s_reduce) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[84], &__pyx_n_s_reduce_cython) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[85], &__pyx_n_s_reduce_ex) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[86], &__pyx_n_s_return) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[87], &__pyx_n_s_self) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[88], &__pyx_kp_s_self_lexer_data_cannot_be_conver) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[89], &__pyx_n_s_set) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[90], &__pyx_n_s_setstate) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[91], &__pyx_n_s_setstate_cython) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[92], &__pyx_kp_s_stringsource) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[93], &__pyx_n_s_syn) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[94], &__pyx_n_s_test) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[95], &__pyx_kp_u_utf_8) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[96], &__pyx_n_s_v) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
-  if (__Pyx_InitString(__pyx_string_tab[97], &__pyx_n_s_val) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[59], &__pyx_n_u_encoding) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[60], &__pyx_n_s_endswith) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[61], &__pyx_n_s_enter) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[62], &__pyx_n_s_exception) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[63], &__pyx_n_s_exit) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[64], &__pyx_n_s_filename) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[65], &__pyx_n_u_filename) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[66], &__pyx_n_s_flag) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[67], &__pyx_kp_u_gc) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[68], &__pyx_n_s_get_flag) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[69], &__pyx_n_s_getstate) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[70], &__pyx_n_s_import) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[71], &__pyx_n_s_is_coroutine) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[72], &__pyx_kp_u_isenabled) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[73], &__pyx_n_s_items) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[74], &__pyx_n_s_k) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[75], &__pyx_n_s_kola_lexer) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[76], &__pyx_kp_s_kola_lexer_pyx) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[77], &__pyx_n_s_kwds) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[78], &__pyx_n_s_lexer) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[79], &__pyx_n_s_lineno) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[80], &__pyx_n_s_main) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[81], &__pyx_n_s_name) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[82], &__pyx_kp_s_no_default___reduce___due_to_non) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[83], &__pyx_kp_u_operation_on_closed_lexer) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[84], &__pyx_n_s_pyx_state) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[85], &__pyx_n_s_pyx_vtable) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[86], &__pyx_n_s_raw_val) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[87], &__pyx_n_s_reduce) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[88], &__pyx_n_s_reduce_cython) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[89], &__pyx_n_s_reduce_ex) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[90], &__pyx_n_s_return) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[91], &__pyx_n_s_self) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[92], &__pyx_kp_s_self_lexer_data_cannot_be_conver) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[93], &__pyx_n_s_set) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[94], &__pyx_n_s_setstate) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[95], &__pyx_n_s_setstate_cython) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[96], &__pyx_n_s_startswith) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[97], &__pyx_kp_s_stringsource) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[98], &__pyx_n_s_syn) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[99], &__pyx_n_s_test) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[100], &__pyx_kp_u_utf_8) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[101], &__pyx_n_s_v) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
+  if (__Pyx_InitString(__pyx_string_tab[102], &__pyx_n_s_val) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
   #endif
   #if !CYTHON_USE_MODULE_STATE
   if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(1, 1, __pyx_L1_error);
   #endif
   return 0;
   __pyx_L1_error:;
   return -1;
@@ -10832,16 +10930,14 @@
 static CYTHON_SMALL_CODE int __Pyx_modinit_variable_import_code(void); /*proto*/
 static CYTHON_SMALL_CODE int __Pyx_modinit_function_import_code(void); /*proto*/
 
 static int __Pyx_modinit_global_init_code(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_modinit_global_init_code", 0);
   /*--- Global init code ---*/
-  __pyx_v_4kola_5lexer__lexer_data_names = ((PyObject*)Py_None); Py_INCREF(Py_None);
-  __pyx_7genexpr__pyx_v_4kola_5lexer_i = Py_None; Py_INCREF(Py_None);
   __Pyx_RefNannyFinishContext();
   return 0;
 }
 
 static int __Pyx_modinit_variable_export_code(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_modinit_variable_export_code", 0);
@@ -10865,163 +10961,163 @@
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_init_code", 0);
   /*--- Type init code ---*/
   __pyx_vtabptr_4kola_5lexer_Token = &__pyx_vtable_4kola_5lexer_Token;
   __pyx_vtable_4kola_5lexer_Token.get_flag = (int (*)(struct __pyx_obj_4kola_5lexer_Token *, int __pyx_skip_dispatch))__pyx_f_4kola_5lexer_5Token_get_flag;
   #if CYTHON_USE_TYPE_SPECS
-  __pyx_ptype_4kola_5lexer_Token = (PyTypeObject *) __Pyx_PyType_FromModuleAndSpec(__pyx_m, &__pyx_type_4kola_5lexer_Token_spec, NULL); if (unlikely(!__pyx_ptype_4kola_5lexer_Token)) __PYX_ERR(1, 37, __pyx_L1_error)
-  if (__Pyx_fix_up_extension_type_from_spec(&__pyx_type_4kola_5lexer_Token_spec, __pyx_ptype_4kola_5lexer_Token) < 0) __PYX_ERR(1, 37, __pyx_L1_error)
+  __pyx_ptype_4kola_5lexer_Token = (PyTypeObject *) __Pyx_PyType_FromModuleAndSpec(__pyx_m, &__pyx_type_4kola_5lexer_Token_spec, NULL); if (unlikely(!__pyx_ptype_4kola_5lexer_Token)) __PYX_ERR(1, 34, __pyx_L1_error)
+  if (__Pyx_fix_up_extension_type_from_spec(&__pyx_type_4kola_5lexer_Token_spec, __pyx_ptype_4kola_5lexer_Token) < 0) __PYX_ERR(1, 34, __pyx_L1_error)
   #else
   __pyx_ptype_4kola_5lexer_Token = &__pyx_type_4kola_5lexer_Token;
   #endif
   #if !CYTHON_COMPILING_IN_LIMITED_API
   #endif
   #if !CYTHON_USE_TYPE_SPECS
-  if (__Pyx_PyType_Ready(__pyx_ptype_4kola_5lexer_Token) < 0) __PYX_ERR(1, 37, __pyx_L1_error)
+  if (__Pyx_PyType_Ready(__pyx_ptype_4kola_5lexer_Token) < 0) __PYX_ERR(1, 34, __pyx_L1_error)
   #endif
   #if PY_MAJOR_VERSION < 3
   __pyx_ptype_4kola_5lexer_Token->tp_print = 0;
   #endif
   #if !CYTHON_COMPILING_IN_LIMITED_API
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_ptype_4kola_5lexer_Token->tp_dictoffset && __pyx_ptype_4kola_5lexer_Token->tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_ptype_4kola_5lexer_Token->tp_getattro = __Pyx_PyObject_GenericGetAttrNoDict;
   }
   #endif
-  if (__Pyx_SetVtable(__pyx_ptype_4kola_5lexer_Token, __pyx_vtabptr_4kola_5lexer_Token) < 0) __PYX_ERR(1, 37, __pyx_L1_error)
+  if (__Pyx_SetVtable(__pyx_ptype_4kola_5lexer_Token, __pyx_vtabptr_4kola_5lexer_Token) < 0) __PYX_ERR(1, 34, __pyx_L1_error)
   #if !CYTHON_COMPILING_IN_LIMITED_API
-  if (__Pyx_MergeVtables(__pyx_ptype_4kola_5lexer_Token) < 0) __PYX_ERR(1, 37, __pyx_L1_error)
+  if (__Pyx_MergeVtables(__pyx_ptype_4kola_5lexer_Token) < 0) __PYX_ERR(1, 34, __pyx_L1_error)
   #endif
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_Token, (PyObject *) __pyx_ptype_4kola_5lexer_Token) < 0) __PYX_ERR(1, 37, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_Token, (PyObject *) __pyx_ptype_4kola_5lexer_Token) < 0) __PYX_ERR(1, 34, __pyx_L1_error)
   #if !CYTHON_COMPILING_IN_LIMITED_API
-  if (__Pyx_setup_reduce((PyObject *) __pyx_ptype_4kola_5lexer_Token) < 0) __PYX_ERR(1, 37, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject *) __pyx_ptype_4kola_5lexer_Token) < 0) __PYX_ERR(1, 34, __pyx_L1_error)
   #endif
   #if CYTHON_USE_TYPE_SPECS
-  __pyx_ptype_4kola_5lexer_LexerConfig = (PyTypeObject *) __Pyx_PyType_FromModuleAndSpec(__pyx_m, &__pyx_type_4kola_5lexer_LexerConfig_spec, NULL); if (unlikely(!__pyx_ptype_4kola_5lexer_LexerConfig)) __PYX_ERR(1, 79, __pyx_L1_error)
-  if (__Pyx_fix_up_extension_type_from_spec(&__pyx_type_4kola_5lexer_LexerConfig_spec, __pyx_ptype_4kola_5lexer_LexerConfig) < 0) __PYX_ERR(1, 79, __pyx_L1_error)
+  __pyx_ptype_4kola_5lexer_LexerConfig = (PyTypeObject *) __Pyx_PyType_FromModuleAndSpec(__pyx_m, &__pyx_type_4kola_5lexer_LexerConfig_spec, NULL); if (unlikely(!__pyx_ptype_4kola_5lexer_LexerConfig)) __PYX_ERR(1, 76, __pyx_L1_error)
+  if (__Pyx_fix_up_extension_type_from_spec(&__pyx_type_4kola_5lexer_LexerConfig_spec, __pyx_ptype_4kola_5lexer_LexerConfig) < 0) __PYX_ERR(1, 76, __pyx_L1_error)
   #else
   __pyx_ptype_4kola_5lexer_LexerConfig = &__pyx_type_4kola_5lexer_LexerConfig;
   #endif
   #if !CYTHON_COMPILING_IN_LIMITED_API
   #endif
   #if !CYTHON_USE_TYPE_SPECS
-  if (__Pyx_PyType_Ready(__pyx_ptype_4kola_5lexer_LexerConfig) < 0) __PYX_ERR(1, 79, __pyx_L1_error)
+  if (__Pyx_PyType_Ready(__pyx_ptype_4kola_5lexer_LexerConfig) < 0) __PYX_ERR(1, 76, __pyx_L1_error)
   #endif
   #if PY_MAJOR_VERSION < 3
   __pyx_ptype_4kola_5lexer_LexerConfig->tp_print = 0;
   #endif
   #if !CYTHON_COMPILING_IN_LIMITED_API
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_ptype_4kola_5lexer_LexerConfig->tp_dictoffset && __pyx_ptype_4kola_5lexer_LexerConfig->tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_ptype_4kola_5lexer_LexerConfig->tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
   #endif
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_LexerConfig, (PyObject *) __pyx_ptype_4kola_5lexer_LexerConfig) < 0) __PYX_ERR(1, 79, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_LexerConfig, (PyObject *) __pyx_ptype_4kola_5lexer_LexerConfig) < 0) __PYX_ERR(1, 76, __pyx_L1_error)
   #if !CYTHON_COMPILING_IN_LIMITED_API
-  if (__Pyx_setup_reduce((PyObject *) __pyx_ptype_4kola_5lexer_LexerConfig) < 0) __PYX_ERR(1, 79, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject *) __pyx_ptype_4kola_5lexer_LexerConfig) < 0) __PYX_ERR(1, 76, __pyx_L1_error)
   #endif
   __pyx_vtabptr_4kola_5lexer_BaseLexer = &__pyx_vtable_4kola_5lexer_BaseLexer;
   __pyx_vtable_4kola_5lexer_BaseLexer.close = (void (*)(struct __pyx_obj_4kola_5lexer_BaseLexer *, int __pyx_skip_dispatch))__pyx_f_4kola_5lexer_9BaseLexer_close;
   __pyx_vtable_4kola_5lexer_BaseLexer.set_error = (void (*)(struct __pyx_obj_4kola_5lexer_BaseLexer *, char const *))__pyx_f_4kola_5lexer_9BaseLexer_set_error;
   __pyx_vtable_4kola_5lexer_BaseLexer.next_syn = (__pyx_ctuple_int__and_char__space_const__ptr__and_Py_ssize_t (*)(struct __pyx_obj_4kola_5lexer_BaseLexer *))__pyx_f_4kola_5lexer_9BaseLexer_next_syn;
   __pyx_vtable_4kola_5lexer_BaseLexer.next_token = (struct __pyx_obj_4kola_5lexer_Token *(*)(struct __pyx_obj_4kola_5lexer_BaseLexer *))__pyx_f_4kola_5lexer_9BaseLexer_next_token;
   #if CYTHON_USE_TYPE_SPECS
-  __pyx_ptype_4kola_5lexer_BaseLexer = (PyTypeObject *) __Pyx_PyType_FromModuleAndSpec(__pyx_m, &__pyx_type_4kola_5lexer_BaseLexer_spec, NULL); if (unlikely(!__pyx_ptype_4kola_5lexer_BaseLexer)) __PYX_ERR(1, 161, __pyx_L1_error)
-  if (__Pyx_fix_up_extension_type_from_spec(&__pyx_type_4kola_5lexer_BaseLexer_spec, __pyx_ptype_4kola_5lexer_BaseLexer) < 0) __PYX_ERR(1, 161, __pyx_L1_error)
+  __pyx_ptype_4kola_5lexer_BaseLexer = (PyTypeObject *) __Pyx_PyType_FromModuleAndSpec(__pyx_m, &__pyx_type_4kola_5lexer_BaseLexer_spec, NULL); if (unlikely(!__pyx_ptype_4kola_5lexer_BaseLexer)) __PYX_ERR(1, 148, __pyx_L1_error)
+  if (__Pyx_fix_up_extension_type_from_spec(&__pyx_type_4kola_5lexer_BaseLexer_spec, __pyx_ptype_4kola_5lexer_BaseLexer) < 0) __PYX_ERR(1, 148, __pyx_L1_error)
   #else
   __pyx_ptype_4kola_5lexer_BaseLexer = &__pyx_type_4kola_5lexer_BaseLexer;
   #endif
   #if !CYTHON_COMPILING_IN_LIMITED_API
   #endif
   #if !CYTHON_USE_TYPE_SPECS
-  if (__Pyx_PyType_Ready(__pyx_ptype_4kola_5lexer_BaseLexer) < 0) __PYX_ERR(1, 161, __pyx_L1_error)
+  if (__Pyx_PyType_Ready(__pyx_ptype_4kola_5lexer_BaseLexer) < 0) __PYX_ERR(1, 148, __pyx_L1_error)
   #endif
   #if PY_MAJOR_VERSION < 3
   __pyx_ptype_4kola_5lexer_BaseLexer->tp_print = 0;
   #endif
   #if !CYTHON_COMPILING_IN_LIMITED_API
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_ptype_4kola_5lexer_BaseLexer->tp_dictoffset && __pyx_ptype_4kola_5lexer_BaseLexer->tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_ptype_4kola_5lexer_BaseLexer->tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
   #endif
-  if (__Pyx_SetVtable(__pyx_ptype_4kola_5lexer_BaseLexer, __pyx_vtabptr_4kola_5lexer_BaseLexer) < 0) __PYX_ERR(1, 161, __pyx_L1_error)
+  if (__Pyx_SetVtable(__pyx_ptype_4kola_5lexer_BaseLexer, __pyx_vtabptr_4kola_5lexer_BaseLexer) < 0) __PYX_ERR(1, 148, __pyx_L1_error)
   #if !CYTHON_COMPILING_IN_LIMITED_API
-  if (__Pyx_MergeVtables(__pyx_ptype_4kola_5lexer_BaseLexer) < 0) __PYX_ERR(1, 161, __pyx_L1_error)
+  if (__Pyx_MergeVtables(__pyx_ptype_4kola_5lexer_BaseLexer) < 0) __PYX_ERR(1, 148, __pyx_L1_error)
   #endif
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_BaseLexer, (PyObject *) __pyx_ptype_4kola_5lexer_BaseLexer) < 0) __PYX_ERR(1, 161, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_BaseLexer, (PyObject *) __pyx_ptype_4kola_5lexer_BaseLexer) < 0) __PYX_ERR(1, 148, __pyx_L1_error)
   #if !CYTHON_COMPILING_IN_LIMITED_API
-  if (__Pyx_setup_reduce((PyObject *) __pyx_ptype_4kola_5lexer_BaseLexer) < 0) __PYX_ERR(1, 161, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject *) __pyx_ptype_4kola_5lexer_BaseLexer) < 0) __PYX_ERR(1, 148, __pyx_L1_error)
   #endif
   __pyx_vtabptr_4kola_5lexer_FileLexer = &__pyx_vtable_4kola_5lexer_FileLexer;
   __pyx_vtable_4kola_5lexer_FileLexer.__pyx_base = *__pyx_vtabptr_4kola_5lexer_BaseLexer;
   __pyx_vtable_4kola_5lexer_FileLexer.__pyx_base.close = (void (*)(struct __pyx_obj_4kola_5lexer_BaseLexer *, int __pyx_skip_dispatch))__pyx_f_4kola_5lexer_9FileLexer_close;
   #if CYTHON_USE_TYPE_SPECS
-  __pyx_t_1 = PyTuple_Pack(1, (PyObject *)__pyx_ptype_4kola_5lexer_BaseLexer); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 296, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_Pack(1, (PyObject *)__pyx_ptype_4kola_5lexer_BaseLexer); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 280, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_4kola_5lexer_FileLexer = (PyTypeObject *) __Pyx_PyType_FromModuleAndSpec(__pyx_m, &__pyx_type_4kola_5lexer_FileLexer_spec, __pyx_t_1);
   __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (unlikely(!__pyx_ptype_4kola_5lexer_FileLexer)) __PYX_ERR(1, 296, __pyx_L1_error)
-  if (__Pyx_fix_up_extension_type_from_spec(&__pyx_type_4kola_5lexer_FileLexer_spec, __pyx_ptype_4kola_5lexer_FileLexer) < 0) __PYX_ERR(1, 296, __pyx_L1_error)
+  if (unlikely(!__pyx_ptype_4kola_5lexer_FileLexer)) __PYX_ERR(1, 280, __pyx_L1_error)
+  if (__Pyx_fix_up_extension_type_from_spec(&__pyx_type_4kola_5lexer_FileLexer_spec, __pyx_ptype_4kola_5lexer_FileLexer) < 0) __PYX_ERR(1, 280, __pyx_L1_error)
   #else
   __pyx_ptype_4kola_5lexer_FileLexer = &__pyx_type_4kola_5lexer_FileLexer;
   #endif
   #if !CYTHON_COMPILING_IN_LIMITED_API
   __pyx_ptype_4kola_5lexer_FileLexer->tp_base = __pyx_ptype_4kola_5lexer_BaseLexer;
   #endif
   #if !CYTHON_USE_TYPE_SPECS
-  if (__Pyx_PyType_Ready(__pyx_ptype_4kola_5lexer_FileLexer) < 0) __PYX_ERR(1, 296, __pyx_L1_error)
+  if (__Pyx_PyType_Ready(__pyx_ptype_4kola_5lexer_FileLexer) < 0) __PYX_ERR(1, 280, __pyx_L1_error)
   #endif
   #if PY_MAJOR_VERSION < 3
   __pyx_ptype_4kola_5lexer_FileLexer->tp_print = 0;
   #endif
   #if !CYTHON_COMPILING_IN_LIMITED_API
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_ptype_4kola_5lexer_FileLexer->tp_dictoffset && __pyx_ptype_4kola_5lexer_FileLexer->tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_ptype_4kola_5lexer_FileLexer->tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
   #endif
-  if (__Pyx_SetVtable(__pyx_ptype_4kola_5lexer_FileLexer, __pyx_vtabptr_4kola_5lexer_FileLexer) < 0) __PYX_ERR(1, 296, __pyx_L1_error)
+  if (__Pyx_SetVtable(__pyx_ptype_4kola_5lexer_FileLexer, __pyx_vtabptr_4kola_5lexer_FileLexer) < 0) __PYX_ERR(1, 280, __pyx_L1_error)
   #if !CYTHON_COMPILING_IN_LIMITED_API
-  if (__Pyx_MergeVtables(__pyx_ptype_4kola_5lexer_FileLexer) < 0) __PYX_ERR(1, 296, __pyx_L1_error)
+  if (__Pyx_MergeVtables(__pyx_ptype_4kola_5lexer_FileLexer) < 0) __PYX_ERR(1, 280, __pyx_L1_error)
   #endif
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_FileLexer, (PyObject *) __pyx_ptype_4kola_5lexer_FileLexer) < 0) __PYX_ERR(1, 296, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_FileLexer, (PyObject *) __pyx_ptype_4kola_5lexer_FileLexer) < 0) __PYX_ERR(1, 280, __pyx_L1_error)
   #if !CYTHON_COMPILING_IN_LIMITED_API
-  if (__Pyx_setup_reduce((PyObject *) __pyx_ptype_4kola_5lexer_FileLexer) < 0) __PYX_ERR(1, 296, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject *) __pyx_ptype_4kola_5lexer_FileLexer) < 0) __PYX_ERR(1, 280, __pyx_L1_error)
   #endif
   __pyx_vtabptr_4kola_5lexer_StringLexer = &__pyx_vtable_4kola_5lexer_StringLexer;
   __pyx_vtable_4kola_5lexer_StringLexer.__pyx_base = *__pyx_vtabptr_4kola_5lexer_BaseLexer;
   #if CYTHON_USE_TYPE_SPECS
-  __pyx_t_1 = PyTuple_Pack(1, (PyObject *)__pyx_ptype_4kola_5lexer_BaseLexer); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 327, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_Pack(1, (PyObject *)__pyx_ptype_4kola_5lexer_BaseLexer); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 311, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_4kola_5lexer_StringLexer = (PyTypeObject *) __Pyx_PyType_FromModuleAndSpec(__pyx_m, &__pyx_type_4kola_5lexer_StringLexer_spec, __pyx_t_1);
   __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (unlikely(!__pyx_ptype_4kola_5lexer_StringLexer)) __PYX_ERR(1, 327, __pyx_L1_error)
-  if (__Pyx_fix_up_extension_type_from_spec(&__pyx_type_4kola_5lexer_StringLexer_spec, __pyx_ptype_4kola_5lexer_StringLexer) < 0) __PYX_ERR(1, 327, __pyx_L1_error)
+  if (unlikely(!__pyx_ptype_4kola_5lexer_StringLexer)) __PYX_ERR(1, 311, __pyx_L1_error)
+  if (__Pyx_fix_up_extension_type_from_spec(&__pyx_type_4kola_5lexer_StringLexer_spec, __pyx_ptype_4kola_5lexer_StringLexer) < 0) __PYX_ERR(1, 311, __pyx_L1_error)
   #else
   __pyx_ptype_4kola_5lexer_StringLexer = &__pyx_type_4kola_5lexer_StringLexer;
   #endif
   #if !CYTHON_COMPILING_IN_LIMITED_API
   __pyx_ptype_4kola_5lexer_StringLexer->tp_base = __pyx_ptype_4kola_5lexer_BaseLexer;
   #endif
   #if !CYTHON_USE_TYPE_SPECS
-  if (__Pyx_PyType_Ready(__pyx_ptype_4kola_5lexer_StringLexer) < 0) __PYX_ERR(1, 327, __pyx_L1_error)
+  if (__Pyx_PyType_Ready(__pyx_ptype_4kola_5lexer_StringLexer) < 0) __PYX_ERR(1, 311, __pyx_L1_error)
   #endif
   #if PY_MAJOR_VERSION < 3
   __pyx_ptype_4kola_5lexer_StringLexer->tp_print = 0;
   #endif
   #if !CYTHON_COMPILING_IN_LIMITED_API
   if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_ptype_4kola_5lexer_StringLexer->tp_dictoffset && __pyx_ptype_4kola_5lexer_StringLexer->tp_getattro == PyObject_GenericGetAttr)) {
     __pyx_ptype_4kola_5lexer_StringLexer->tp_getattro = __Pyx_PyObject_GenericGetAttr;
   }
   #endif
-  if (__Pyx_SetVtable(__pyx_ptype_4kola_5lexer_StringLexer, __pyx_vtabptr_4kola_5lexer_StringLexer) < 0) __PYX_ERR(1, 327, __pyx_L1_error)
+  if (__Pyx_SetVtable(__pyx_ptype_4kola_5lexer_StringLexer, __pyx_vtabptr_4kola_5lexer_StringLexer) < 0) __PYX_ERR(1, 311, __pyx_L1_error)
   #if !CYTHON_COMPILING_IN_LIMITED_API
-  if (__Pyx_MergeVtables(__pyx_ptype_4kola_5lexer_StringLexer) < 0) __PYX_ERR(1, 327, __pyx_L1_error)
+  if (__Pyx_MergeVtables(__pyx_ptype_4kola_5lexer_StringLexer) < 0) __PYX_ERR(1, 311, __pyx_L1_error)
   #endif
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_StringLexer, (PyObject *) __pyx_ptype_4kola_5lexer_StringLexer) < 0) __PYX_ERR(1, 327, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_StringLexer, (PyObject *) __pyx_ptype_4kola_5lexer_StringLexer) < 0) __PYX_ERR(1, 311, __pyx_L1_error)
   #if !CYTHON_COMPILING_IN_LIMITED_API
-  if (__Pyx_setup_reduce((PyObject *) __pyx_ptype_4kola_5lexer_StringLexer) < 0) __PYX_ERR(1, 327, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject *) __pyx_ptype_4kola_5lexer_StringLexer) < 0) __PYX_ERR(1, 311, __pyx_L1_error)
   #endif
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -11239,21 +11335,14 @@
 #endif
 #endif
 {
   int stringtab_initialized = 0;
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
-  PyObject *__pyx_t_4 = NULL;
-  Py_ssize_t __pyx_t_5;
-  PyObject *(*__pyx_t_6)(PyObject *);
-  int __pyx_t_7;
-  int __pyx_t_8;
-  int __pyx_t_9;
-  PyObject *__pyx_t_10 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannyDeclarations
   #if CYTHON_PEP489_MULTI_PHASE_INIT
   if (__pyx_m) {
     if (__pyx_m == __pyx_pyinit_module) return 0;
@@ -11362,525 +11451,354 @@
   (void)__Pyx_modinit_variable_import_code();
   (void)__Pyx_modinit_function_import_code();
   /*--- Execution code ---*/
   #if defined(__Pyx_Generator_USED) || defined(__Pyx_Coroutine_USED)
   if (__Pyx_patch_abc() < 0) __PYX_ERR(1, 1, __pyx_L1_error)
   #endif
 
-  /* "kola/lexer.pyx":12
+  /* "kola/lexer.pyx":9
  * from ._yylex cimport *
  * 
  * from .exception import KoiLangSyntaxError             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_2 = PyList_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 12, __pyx_L1_error)
+  __pyx_t_2 = PyList_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_INCREF(__pyx_n_s_KoiLangSyntaxError);
   __Pyx_GIVEREF(__pyx_n_s_KoiLangSyntaxError);
   PyList_SET_ITEM(__pyx_t_2, 0, __pyx_n_s_KoiLangSyntaxError);
-  __pyx_t_3 = __Pyx_Import(__pyx_n_s_exception, __pyx_t_2, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 12, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_Import(__pyx_n_s_exception, __pyx_t_2, 1); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_3, __pyx_n_s_KoiLangSyntaxError); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 12, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_3, __pyx_n_s_KoiLangSyntaxError); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_KoiLangSyntaxError, __pyx_t_2) < 0) __PYX_ERR(1, 12, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_KoiLangSyntaxError, __pyx_t_2) < 0) __PYX_ERR(1, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "kola/lexer.pyx":18
+  /* "kola/lexer.pyx":15
  * 
  * # token syn
  * S_CMD = CMD             # <<<<<<<<<<<<<<
  * S_CMD_N = CMD_N
  * S_TEXT = TEXT
  */
-  __pyx_t_3 = __Pyx_PyInt_From_enum__TokenSyn(CMD); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 18, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_enum__TokenSyn(CMD); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 15, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_S_CMD, __pyx_t_3) < 0) __PYX_ERR(1, 18, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_S_CMD, __pyx_t_3) < 0) __PYX_ERR(1, 15, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "kola/lexer.pyx":19
+  /* "kola/lexer.pyx":16
  * # token syn
  * S_CMD = CMD
  * S_CMD_N = CMD_N             # <<<<<<<<<<<<<<
  * S_TEXT = TEXT
  * S_LITERAL = LITERAL
  */
-  __pyx_t_3 = __Pyx_PyInt_From_enum__TokenSyn(CMD_N); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 19, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_enum__TokenSyn(CMD_N); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 16, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_S_CMD_N, __pyx_t_3) < 0) __PYX_ERR(1, 19, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_S_CMD_N, __pyx_t_3) < 0) __PYX_ERR(1, 16, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "kola/lexer.pyx":20
+  /* "kola/lexer.pyx":17
  * S_CMD = CMD
  * S_CMD_N = CMD_N
  * S_TEXT = TEXT             # <<<<<<<<<<<<<<
  * S_LITERAL = LITERAL
  * S_STRING = STRING
  */
-  __pyx_t_3 = __Pyx_PyInt_From_enum__TokenSyn(TEXT); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 20, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_enum__TokenSyn(TEXT); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 17, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_S_TEXT, __pyx_t_3) < 0) __PYX_ERR(1, 20, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_S_TEXT, __pyx_t_3) < 0) __PYX_ERR(1, 17, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "kola/lexer.pyx":21
+  /* "kola/lexer.pyx":18
  * S_CMD_N = CMD_N
  * S_TEXT = TEXT
  * S_LITERAL = LITERAL             # <<<<<<<<<<<<<<
  * S_STRING = STRING
  * S_NUM = NUM
  */
-  __pyx_t_3 = __Pyx_PyInt_From_enum__TokenSyn(LITERAL); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 21, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_enum__TokenSyn(LITERAL); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 18, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_S_LITERAL, __pyx_t_3) < 0) __PYX_ERR(1, 21, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_S_LITERAL, __pyx_t_3) < 0) __PYX_ERR(1, 18, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "kola/lexer.pyx":22
+  /* "kola/lexer.pyx":19
  * S_TEXT = TEXT
  * S_LITERAL = LITERAL
  * S_STRING = STRING             # <<<<<<<<<<<<<<
  * S_NUM = NUM
  * S_NUM_H = NUM_H
  */
-  __pyx_t_3 = __Pyx_PyInt_From_enum__TokenSyn(STRING); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 22, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_enum__TokenSyn(STRING); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 19, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_S_STRING, __pyx_t_3) < 0) __PYX_ERR(1, 22, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_S_STRING, __pyx_t_3) < 0) __PYX_ERR(1, 19, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "kola/lexer.pyx":23
+  /* "kola/lexer.pyx":20
  * S_LITERAL = LITERAL
  * S_STRING = STRING
  * S_NUM = NUM             # <<<<<<<<<<<<<<
  * S_NUM_H = NUM_H
  * S_NUM_B = NUM_B
  */
-  __pyx_t_3 = __Pyx_PyInt_From_enum__TokenSyn(NUM); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 23, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_enum__TokenSyn(NUM); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 20, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_S_NUM, __pyx_t_3) < 0) __PYX_ERR(1, 23, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_S_NUM, __pyx_t_3) < 0) __PYX_ERR(1, 20, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "kola/lexer.pyx":24
+  /* "kola/lexer.pyx":21
  * S_STRING = STRING
  * S_NUM = NUM
  * S_NUM_H = NUM_H             # <<<<<<<<<<<<<<
  * S_NUM_B = NUM_B
  * S_NUM_F = NUM_F
  */
-  __pyx_t_3 = __Pyx_PyInt_From_enum__TokenSyn(NUM_H); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 24, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_enum__TokenSyn(NUM_H); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 21, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_S_NUM_H, __pyx_t_3) < 0) __PYX_ERR(1, 24, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_S_NUM_H, __pyx_t_3) < 0) __PYX_ERR(1, 21, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "kola/lexer.pyx":25
+  /* "kola/lexer.pyx":22
  * S_NUM = NUM
  * S_NUM_H = NUM_H
  * S_NUM_B = NUM_B             # <<<<<<<<<<<<<<
  * S_NUM_F = NUM_F
  * S_CLN = CLN
  */
-  __pyx_t_3 = __Pyx_PyInt_From_enum__TokenSyn(NUM_B); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 25, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_enum__TokenSyn(NUM_B); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 22, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_S_NUM_B, __pyx_t_3) < 0) __PYX_ERR(1, 25, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_S_NUM_B, __pyx_t_3) < 0) __PYX_ERR(1, 22, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "kola/lexer.pyx":26
+  /* "kola/lexer.pyx":23
  * S_NUM_H = NUM_H
  * S_NUM_B = NUM_B
  * S_NUM_F = NUM_F             # <<<<<<<<<<<<<<
  * S_CLN = CLN
  * S_CMA = CMA
  */
-  __pyx_t_3 = __Pyx_PyInt_From_enum__TokenSyn(NUM_F); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 26, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_enum__TokenSyn(NUM_F); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 23, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_S_NUM_F, __pyx_t_3) < 0) __PYX_ERR(1, 26, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_S_NUM_F, __pyx_t_3) < 0) __PYX_ERR(1, 23, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "kola/lexer.pyx":27
+  /* "kola/lexer.pyx":24
  * S_NUM_B = NUM_B
  * S_NUM_F = NUM_F
  * S_CLN = CLN             # <<<<<<<<<<<<<<
  * S_CMA = CMA
  * S_SLP = SLP
  */
-  __pyx_t_3 = __Pyx_PyInt_From_enum__TokenSyn(CLN); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 27, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_enum__TokenSyn(CLN); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 24, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_S_CLN, __pyx_t_3) < 0) __PYX_ERR(1, 27, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_S_CLN, __pyx_t_3) < 0) __PYX_ERR(1, 24, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "kola/lexer.pyx":28
+  /* "kola/lexer.pyx":25
  * S_NUM_F = NUM_F
  * S_CLN = CLN
  * S_CMA = CMA             # <<<<<<<<<<<<<<
  * S_SLP = SLP
  * S_SRP = SRP
  */
-  __pyx_t_3 = __Pyx_PyInt_From_enum__TokenSyn(CMA); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 28, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_enum__TokenSyn(CMA); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 25, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_S_CMA, __pyx_t_3) < 0) __PYX_ERR(1, 28, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_S_CMA, __pyx_t_3) < 0) __PYX_ERR(1, 25, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "kola/lexer.pyx":29
+  /* "kola/lexer.pyx":26
  * S_CLN = CLN
  * S_CMA = CMA
  * S_SLP = SLP             # <<<<<<<<<<<<<<
  * S_SRP = SRP
  * S_ANNOTATION = ANNOTATION
  */
-  __pyx_t_3 = __Pyx_PyInt_From_enum__TokenSyn(SLP); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 29, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_enum__TokenSyn(SLP); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 26, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_S_SLP, __pyx_t_3) < 0) __PYX_ERR(1, 29, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_S_SLP, __pyx_t_3) < 0) __PYX_ERR(1, 26, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "kola/lexer.pyx":30
+  /* "kola/lexer.pyx":27
  * S_CMA = CMA
  * S_SLP = SLP
  * S_SRP = SRP             # <<<<<<<<<<<<<<
  * S_ANNOTATION = ANNOTATION
  * F_DISABLED = LFLAG_DISABLED
  */
-  __pyx_t_3 = __Pyx_PyInt_From_enum__TokenSyn(SRP); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 30, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_enum__TokenSyn(SRP); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 27, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_S_SRP, __pyx_t_3) < 0) __PYX_ERR(1, 30, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_S_SRP, __pyx_t_3) < 0) __PYX_ERR(1, 27, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "kola/lexer.pyx":31
+  /* "kola/lexer.pyx":28
  * S_SLP = SLP
  * S_SRP = SRP
  * S_ANNOTATION = ANNOTATION             # <<<<<<<<<<<<<<
  * F_DISABLED = LFLAG_DISABLED
  * F_LSTRIP_TEXT = LFLAG_NOLSTRIP
  */
-  __pyx_t_3 = __Pyx_PyInt_From_enum__TokenSyn(ANNOTATION); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 31, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_enum__TokenSyn(ANNOTATION); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 28, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_S_ANNOTATION, __pyx_t_3) < 0) __PYX_ERR(1, 31, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_S_ANNOTATION, __pyx_t_3) < 0) __PYX_ERR(1, 28, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "kola/lexer.pyx":32
+  /* "kola/lexer.pyx":29
  * S_SRP = SRP
  * S_ANNOTATION = ANNOTATION
  * F_DISABLED = LFLAG_DISABLED             # <<<<<<<<<<<<<<
  * F_LSTRIP_TEXT = LFLAG_NOLSTRIP
  * 
  */
-  __pyx_t_3 = __Pyx_PyInt_From_int(LFLAG_DISABLED); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 32, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_int(LFLAG_DISABLED); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 29, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_F_DISABLED, __pyx_t_3) < 0) __PYX_ERR(1, 32, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_F_DISABLED, __pyx_t_3) < 0) __PYX_ERR(1, 29, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "kola/lexer.pyx":33
+  /* "kola/lexer.pyx":30
  * S_ANNOTATION = ANNOTATION
  * F_DISABLED = LFLAG_DISABLED
  * F_LSTRIP_TEXT = LFLAG_NOLSTRIP             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_3 = __Pyx_PyInt_From_int(LFLAG_NOLSTRIP); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 33, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyInt_From_int(LFLAG_NOLSTRIP); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 30, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_F_LSTRIP_TEXT, __pyx_t_3) < 0) __PYX_ERR(1, 33, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_F_LSTRIP_TEXT, __pyx_t_3) < 0) __PYX_ERR(1, 30, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "kola/lexer.pyx":62
+  /* "kola/lexer.pyx":59
  *         return self is other or self.syn == other
  * 
  *     cpdef int get_flag(self):             # <<<<<<<<<<<<<<
  *         if self.syn <= TEXT or self.syn == ANNOTATION:
  *             return 0
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_4kola_5lexer_5Token_5get_flag, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Token_get_flag, NULL, __pyx_n_s_kola_lexer, __pyx_d, ((PyObject *)__pyx_codeobj__4)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 62, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_4kola_5lexer_5Token_5get_flag, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Token_get_flag, NULL, __pyx_n_s_kola_lexer, __pyx_d, ((PyObject *)__pyx_codeobj__5)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 59, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_4kola_5lexer_Token->tp_dict, __pyx_n_s_get_flag, __pyx_t_3) < 0) __PYX_ERR(1, 62, __pyx_L1_error)
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_4kola_5lexer_Token->tp_dict, __pyx_n_s_get_flag, __pyx_t_3) < 0) __PYX_ERR(1, 59, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   PyType_Modified(__pyx_ptype_4kola_5lexer_Token);
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  * def __setstate_cython__(self, __pyx_state):
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_4kola_5lexer_5Token_9__reduce_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Token___reduce_cython, NULL, __pyx_n_s_kola_lexer, __pyx_d, ((PyObject *)__pyx_codeobj__5)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_4kola_5lexer_5Token_9__reduce_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Token___reduce_cython, NULL, __pyx_n_s_kola_lexer, __pyx_d, ((PyObject *)__pyx_codeobj__6)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_reduce_cython, __pyx_t_3) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
   /* "(tree fragment)":3
  * def __reduce_cython__(self):
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_4kola_5lexer_5Token_11__setstate_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Token___setstate_cython, NULL, __pyx_n_s_kola_lexer, __pyx_d, ((PyObject *)__pyx_codeobj__7)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 3, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_4kola_5lexer_5Token_11__setstate_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_Token___setstate_cython, NULL, __pyx_n_s_kola_lexer, __pyx_d, ((PyObject *)__pyx_codeobj__8)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 3, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_setstate_cython, __pyx_t_3) < 0) __PYX_ERR(0, 3, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "kola/lexer.pyx":88
+  /* "kola/lexer.pyx":85
  *         self.lexer_data = &lexer.lexer_data
  * 
  *     def dict(self) -> dict:             # <<<<<<<<<<<<<<
- *         cdef dict data = {}
- *         for i in _lexer_data_names:
+ *         cdef dict data = <dict>self.lexer_data[0]
+ *         data["filename"] = (<bytes>data["filename"]).decode()
  */
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 88, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 85, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_return, __pyx_n_s_dict) < 0) __PYX_ERR(1, 88, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_4kola_5lexer_11LexerConfig_3dict, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_LexerConfig_dict, NULL, __pyx_n_s_kola_lexer, __pyx_d, ((PyObject *)__pyx_codeobj__9)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 88, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_return, __pyx_n_s_dict) < 0) __PYX_ERR(1, 85, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_CyFunction_New(&__pyx_mdef_4kola_5lexer_11LexerConfig_3dict, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_LexerConfig_dict, NULL, __pyx_n_s_kola_lexer, __pyx_d, ((PyObject *)__pyx_codeobj__10)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 85, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_2, __pyx_t_3);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_4kola_5lexer_LexerConfig->tp_dict, __pyx_n_s_dict, __pyx_t_2) < 0) __PYX_ERR(1, 88, __pyx_L1_error)
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_4kola_5lexer_LexerConfig->tp_dict, __pyx_n_s_dict, __pyx_t_2) < 0) __PYX_ERR(1, 85, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   PyType_Modified(__pyx_ptype_4kola_5lexer_LexerConfig);
 
-  /* "kola/lexer.pyx":94
+  /* "kola/lexer.pyx":91
  *         return data
  * 
  *     def set(self, **kwds) -> None:             # <<<<<<<<<<<<<<
  *         for k, v in kwds.items():
- *             if not k in _lexer_data_names:
+ *             if k.startswith('__') and k.endswith('__'):
  */
-  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 94, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 91, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_return, __pyx_n_s_None) < 0) __PYX_ERR(1, 94, __pyx_L1_error)
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_4kola_5lexer_11LexerConfig_5set, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_LexerConfig_set, NULL, __pyx_n_s_kola_lexer, __pyx_d, ((PyObject *)__pyx_codeobj__11)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 94, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_return, __pyx_n_s_None) < 0) __PYX_ERR(1, 91, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_4kola_5lexer_11LexerConfig_5set, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_LexerConfig_set, NULL, __pyx_n_s_kola_lexer, __pyx_d, ((PyObject *)__pyx_codeobj__12)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 91, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_CyFunction_SetAnnotationsDict(__pyx_t_3, __pyx_t_2);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_4kola_5lexer_LexerConfig->tp_dict, __pyx_n_s_set, __pyx_t_3) < 0) __PYX_ERR(1, 94, __pyx_L1_error)
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_4kola_5lexer_LexerConfig->tp_dict, __pyx_n_s_set, __pyx_t_3) < 0) __PYX_ERR(1, 91, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   PyType_Modified(__pyx_ptype_4kola_5lexer_LexerConfig);
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     raise TypeError, "self.lexer_data cannot be converted to a Python object for pickling"
  * def __setstate_cython__(self, __pyx_state):
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_4kola_5lexer_11LexerConfig_7__reduce_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_LexerConfig___reduce_cython, NULL, __pyx_n_s_kola_lexer, __pyx_d, ((PyObject *)__pyx_codeobj__12)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_4kola_5lexer_11LexerConfig_7__reduce_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_LexerConfig___reduce_cython, NULL, __pyx_n_s_kola_lexer, __pyx_d, ((PyObject *)__pyx_codeobj__13)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_reduce_cython, __pyx_t_3) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
   /* "(tree fragment)":3
  * def __reduce_cython__(self):
  *     raise TypeError, "self.lexer_data cannot be converted to a Python object for pickling"
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     raise TypeError, "self.lexer_data cannot be converted to a Python object for pickling"
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_4kola_5lexer_11LexerConfig_9__setstate_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_LexerConfig___setstate_cython, NULL, __pyx_n_s_kola_lexer, __pyx_d, ((PyObject *)__pyx_codeobj__13)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 3, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_4kola_5lexer_11LexerConfig_9__setstate_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_LexerConfig___setstate_cython, NULL, __pyx_n_s_kola_lexer, __pyx_d, ((PyObject *)__pyx_codeobj__14)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 3, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_setstate_cython, __pyx_t_3) < 0) __PYX_ERR(0, 3, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "kola/lexer.pyx":151
- * 
- * 
- * cdef set _lexer_data_names = {             # <<<<<<<<<<<<<<
- *     i for i in dir(LexerConfig)
- *     if not (<str>i).startswith('__') and not (<str>i).endswith('__') and PyDescr_IsData(getattr(LexerConfig, (<str>i)))
- */
-  { /* enter inner scope */
-    __pyx_t_3 = PySet_New(NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 151, __pyx_L4_error)
-    __Pyx_GOTREF(__pyx_t_3);
-
-    /* "kola/lexer.pyx":152
- * 
- * cdef set _lexer_data_names = {
- *     i for i in dir(LexerConfig)             # <<<<<<<<<<<<<<
- *     if not (<str>i).startswith('__') and not (<str>i).endswith('__') and PyDescr_IsData(getattr(LexerConfig, (<str>i)))
- * }
- */
-    __pyx_t_2 = PyObject_Dir(((PyObject *)__pyx_ptype_4kola_5lexer_LexerConfig)); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 152, __pyx_L4_error)
-    __Pyx_GOTREF(__pyx_t_2);
-    if (likely(PyList_CheckExact(__pyx_t_2)) || PyTuple_CheckExact(__pyx_t_2)) {
-      __pyx_t_4 = __pyx_t_2; __Pyx_INCREF(__pyx_t_4); __pyx_t_5 = 0;
-      __pyx_t_6 = NULL;
-    } else {
-      __pyx_t_5 = -1; __pyx_t_4 = PyObject_GetIter(__pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 152, __pyx_L4_error)
-      __Pyx_GOTREF(__pyx_t_4);
-      __pyx_t_6 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_4); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 152, __pyx_L4_error)
-    }
-    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-    for (;;) {
-      if (likely(!__pyx_t_6)) {
-        if (likely(PyList_CheckExact(__pyx_t_4))) {
-          if (__pyx_t_5 >= PyList_GET_SIZE(__pyx_t_4)) break;
-          #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_2 = PyList_GET_ITEM(__pyx_t_4, __pyx_t_5); __Pyx_INCREF(__pyx_t_2); __pyx_t_5++; if (unlikely((0 < 0))) __PYX_ERR(1, 152, __pyx_L4_error)
-          #else
-          __pyx_t_2 = PySequence_ITEM(__pyx_t_4, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 152, __pyx_L4_error)
-          __Pyx_GOTREF(__pyx_t_2);
-          #endif
-        } else {
-          if (__pyx_t_5 >= PyTuple_GET_SIZE(__pyx_t_4)) break;
-          #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_2 = PyTuple_GET_ITEM(__pyx_t_4, __pyx_t_5); __Pyx_INCREF(__pyx_t_2); __pyx_t_5++; if (unlikely((0 < 0))) __PYX_ERR(1, 152, __pyx_L4_error)
-          #else
-          __pyx_t_2 = PySequence_ITEM(__pyx_t_4, __pyx_t_5); __pyx_t_5++; if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 152, __pyx_L4_error)
-          __Pyx_GOTREF(__pyx_t_2);
-          #endif
-        }
-      } else {
-        __pyx_t_2 = __pyx_t_6(__pyx_t_4);
-        if (unlikely(!__pyx_t_2)) {
-          PyObject* exc_type = PyErr_Occurred();
-          if (exc_type) {
-            if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-            else __PYX_ERR(1, 152, __pyx_L4_error)
-          }
-          break;
-        }
-        __Pyx_GOTREF(__pyx_t_2);
-      }
-      __Pyx_XGOTREF(__pyx_7genexpr__pyx_v_4kola_5lexer_i);
-      __Pyx_DECREF_SET(__pyx_7genexpr__pyx_v_4kola_5lexer_i, __pyx_t_2);
-      __Pyx_GIVEREF(__pyx_t_2);
-      __pyx_t_2 = 0;
-
-      /* "kola/lexer.pyx":153
- * cdef set _lexer_data_names = {
- *     i for i in dir(LexerConfig)
- *     if not (<str>i).startswith('__') and not (<str>i).endswith('__') and PyDescr_IsData(getattr(LexerConfig, (<str>i)))             # <<<<<<<<<<<<<<
- * }
- * 
- */
-      if (unlikely(__pyx_7genexpr__pyx_v_4kola_5lexer_i == Py_None)) {
-        PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "startswith");
-        __PYX_ERR(1, 153, __pyx_L4_error)
-      }
-      __pyx_t_8 = __Pyx_PyUnicode_Tailmatch(((PyObject*)__pyx_7genexpr__pyx_v_4kola_5lexer_i), __pyx_n_u__14, 0, PY_SSIZE_T_MAX, -1); if (unlikely(__pyx_t_8 == ((int)-1))) __PYX_ERR(1, 153, __pyx_L4_error)
-      __pyx_t_9 = ((!(__pyx_t_8 != 0)) != 0);
-      if (__pyx_t_9) {
-      } else {
-        __pyx_t_7 = __pyx_t_9;
-        goto __pyx_L8_bool_binop_done;
-      }
-      if (unlikely(__pyx_7genexpr__pyx_v_4kola_5lexer_i == Py_None)) {
-        PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "endswith");
-        __PYX_ERR(1, 153, __pyx_L4_error)
-      }
-      __pyx_t_9 = __Pyx_PyUnicode_Tailmatch(((PyObject*)__pyx_7genexpr__pyx_v_4kola_5lexer_i), __pyx_n_u__14, 0, PY_SSIZE_T_MAX, 1); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(1, 153, __pyx_L4_error)
-      __pyx_t_8 = ((!(__pyx_t_9 != 0)) != 0);
-      if (__pyx_t_8) {
-      } else {
-        __pyx_t_7 = __pyx_t_8;
-        goto __pyx_L8_bool_binop_done;
-      }
-      __pyx_t_2 = __pyx_7genexpr__pyx_v_4kola_5lexer_i;
-      __Pyx_INCREF(__pyx_t_2);
-      __pyx_t_10 = __Pyx_GetAttr(((PyObject *)__pyx_ptype_4kola_5lexer_LexerConfig), __pyx_t_2); if (unlikely(!__pyx_t_10)) __PYX_ERR(1, 153, __pyx_L4_error)
-      __Pyx_GOTREF(__pyx_t_10);
-      __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-      __pyx_t_8 = (PyDescr_IsData(__pyx_t_10) != 0);
-      __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
-      __pyx_t_7 = __pyx_t_8;
-      __pyx_L8_bool_binop_done:;
-      if (__pyx_t_7) {
-
-        /* "kola/lexer.pyx":152
- * 
- * cdef set _lexer_data_names = {
- *     i for i in dir(LexerConfig)             # <<<<<<<<<<<<<<
- *     if not (<str>i).startswith('__') and not (<str>i).endswith('__') and PyDescr_IsData(getattr(LexerConfig, (<str>i)))
- * }
- */
-        if (unlikely(PySet_Add(__pyx_t_3, (PyObject*)__pyx_7genexpr__pyx_v_4kola_5lexer_i))) __PYX_ERR(1, 152, __pyx_L4_error)
-
-        /* "kola/lexer.pyx":153
- * cdef set _lexer_data_names = {
- *     i for i in dir(LexerConfig)
- *     if not (<str>i).startswith('__') and not (<str>i).endswith('__') and PyDescr_IsData(getattr(LexerConfig, (<str>i)))             # <<<<<<<<<<<<<<
- * }
- * 
- */
-      }
-
-      /* "kola/lexer.pyx":152
- * 
- * cdef set _lexer_data_names = {
- *     i for i in dir(LexerConfig)             # <<<<<<<<<<<<<<
- *     if not (<str>i).startswith('__') and not (<str>i).endswith('__') and PyDescr_IsData(getattr(LexerConfig, (<str>i)))
- * }
- */
-    }
-    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-    __Pyx_GOTREF(__pyx_7genexpr__pyx_v_4kola_5lexer_i);
-    __Pyx_DECREF_SET(__pyx_7genexpr__pyx_v_4kola_5lexer_i, Py_None);
-    goto __pyx_L11_exit_scope;
-    __pyx_L4_error:;
-    __Pyx_GOTREF(__pyx_7genexpr__pyx_v_4kola_5lexer_i);
-    __Pyx_DECREF_SET(__pyx_7genexpr__pyx_v_4kola_5lexer_i, Py_None);
-    goto __pyx_L1_error;
-    __pyx_L11_exit_scope:;
-  } /* exit inner scope */
-  __Pyx_XGOTREF(__pyx_v_4kola_5lexer__lexer_data_names);
-  __Pyx_DECREF_SET(__pyx_v_4kola_5lexer__lexer_data_names, ((PyObject*)__pyx_t_3));
-  __Pyx_GIVEREF(__pyx_t_3);
-  __pyx_t_3 = 0;
-
-  /* "kola/lexer.pyx":157
- * 
- * # update LexerConfig.attr_names
- * (<dict>(<PyTypeObject*>LexerConfig).tp_dict)["data_names"] = frozenset(_lexer_data_names)             # <<<<<<<<<<<<<<
- * PyType_Modified(LexerConfig)
- * 
- */
-  __pyx_t_3 = __Pyx_PyFrozenSet_New(__pyx_v_4kola_5lexer__lexer_data_names); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 157, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  if (unlikely(((PyObject *)((PyTypeObject *)__pyx_ptype_4kola_5lexer_LexerConfig)->tp_dict) == Py_None)) {
-    PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
-    __PYX_ERR(1, 157, __pyx_L1_error)
-  }
-  if (unlikely((PyDict_SetItem(((PyObject*)((PyTypeObject *)__pyx_ptype_4kola_5lexer_LexerConfig)->tp_dict), __pyx_n_u_data_names, __pyx_t_3) < 0))) __PYX_ERR(1, 157, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-
-  /* "kola/lexer.pyx":158
- * # update LexerConfig.attr_names
- * (<dict>(<PyTypeObject*>LexerConfig).tp_dict)["data_names"] = frozenset(_lexer_data_names)
- * PyType_Modified(LexerConfig)             # <<<<<<<<<<<<<<
- * 
- * 
- */
-  PyType_Modified(((PyTypeObject *)__pyx_ptype_4kola_5lexer_LexerConfig));
-
-  /* "kola/lexer.pyx":183
+  /* "kola/lexer.pyx":170
  *             yylex_destroy(self.scanner)
  * 
  *     cpdef void close(self):             # <<<<<<<<<<<<<<
  *         yypop_buffer_state(self.scanner)
  * 
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_4kola_5lexer_9BaseLexer_7close, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_BaseLexer_close, NULL, __pyx_n_s_kola_lexer, __pyx_d, ((PyObject *)__pyx_codeobj__15)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 183, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_4kola_5lexer_9BaseLexer_7close, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_BaseLexer_close, NULL, __pyx_n_s_kola_lexer, __pyx_d, ((PyObject *)__pyx_codeobj__15)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 170, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_4kola_5lexer_BaseLexer->tp_dict, __pyx_n_s_close, __pyx_t_3) < 0) __PYX_ERR(1, 183, __pyx_L1_error)
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_4kola_5lexer_BaseLexer->tp_dict, __pyx_n_s_close, __pyx_t_3) < 0) __PYX_ERR(1, 170, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   PyType_Modified(__pyx_ptype_4kola_5lexer_BaseLexer);
 
-  /* "kola/lexer.pyx":276
+  /* "kola/lexer.pyx":263
  *         return token
  * 
  *     def __enter__(self):             # <<<<<<<<<<<<<<
  *         return self
  * 
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_4kola_5lexer_9BaseLexer_13__enter__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_BaseLexer___enter, NULL, __pyx_n_s_kola_lexer, __pyx_d, ((PyObject *)__pyx_codeobj__16)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 276, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_4kola_5lexer_9BaseLexer_13__enter__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_BaseLexer___enter, NULL, __pyx_n_s_kola_lexer, __pyx_d, ((PyObject *)__pyx_codeobj__16)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 263, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_4kola_5lexer_BaseLexer->tp_dict, __pyx_n_s_enter, __pyx_t_3) < 0) __PYX_ERR(1, 276, __pyx_L1_error)
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_4kola_5lexer_BaseLexer->tp_dict, __pyx_n_s_enter, __pyx_t_3) < 0) __PYX_ERR(1, 263, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   PyType_Modified(__pyx_ptype_4kola_5lexer_BaseLexer);
 
-  /* "kola/lexer.pyx":279
+  /* "kola/lexer.pyx":266
  *         return self
  * 
  *     def __exit__(self, *args):             # <<<<<<<<<<<<<<
  *         self.close()
  * 
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_4kola_5lexer_9BaseLexer_15__exit__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_BaseLexer___exit, NULL, __pyx_n_s_kola_lexer, __pyx_d, ((PyObject *)__pyx_codeobj__18)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 279, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_4kola_5lexer_9BaseLexer_15__exit__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_BaseLexer___exit, NULL, __pyx_n_s_kola_lexer, __pyx_d, ((PyObject *)__pyx_codeobj__18)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 266, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_4kola_5lexer_BaseLexer->tp_dict, __pyx_n_s_exit, __pyx_t_3) < 0) __PYX_ERR(1, 279, __pyx_L1_error)
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_4kola_5lexer_BaseLexer->tp_dict, __pyx_n_s_exit, __pyx_t_3) < 0) __PYX_ERR(1, 266, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   PyType_Modified(__pyx_ptype_4kola_5lexer_BaseLexer);
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  * def __setstate_cython__(self, __pyx_state):
@@ -11897,24 +11815,24 @@
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  */
   __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_4kola_5lexer_9BaseLexer_21__setstate_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_BaseLexer___setstate_cython, NULL, __pyx_n_s_kola_lexer, __pyx_d, ((PyObject *)__pyx_codeobj__20)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 3, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_setstate_cython, __pyx_t_3) < 0) __PYX_ERR(0, 3, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "kola/lexer.pyx":316
+  /* "kola/lexer.pyx":300
  *         LexerConfig(self).set(**kwds)
  * 
  *     cpdef void close(self):             # <<<<<<<<<<<<<<
  *         BaseLexer.close(self)
  *         if self.fp:
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_4kola_5lexer_9FileLexer_3close, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_FileLexer_close, NULL, __pyx_n_s_kola_lexer, __pyx_d, ((PyObject *)__pyx_codeobj__21)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 316, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_4kola_5lexer_9FileLexer_3close, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_FileLexer_close, NULL, __pyx_n_s_kola_lexer, __pyx_d, ((PyObject *)__pyx_codeobj__21)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 300, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_4kola_5lexer_FileLexer->tp_dict, __pyx_n_s_close, __pyx_t_3) < 0) __PYX_ERR(1, 316, __pyx_L1_error)
+  if (PyDict_SetItem((PyObject *)__pyx_ptype_4kola_5lexer_FileLexer->tp_dict, __pyx_n_s_close, __pyx_t_3) < 0) __PYX_ERR(1, 300, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   PyType_Modified(__pyx_ptype_4kola_5lexer_FileLexer);
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     raise TypeError, "no default __reduce__ due to non-trivial __cinit__"
  * def __setstate_cython__(self, __pyx_state):
@@ -11976,16 +11894,14 @@
 
   /*--- Wrapped vars code ---*/
 
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
-  __Pyx_XDECREF(__pyx_t_4);
-  __Pyx_XDECREF(__pyx_t_10);
   if (__pyx_m) {
     if (__pyx_d && stringtab_initialized) {
       __Pyx_AddTraceback("init kola.lexer", __pyx_clineno, __pyx_lineno, __pyx_filename);
     }
     #if !CYTHON_USE_MODULE_STATE
     Py_CLEAR(__pyx_m);
     #endif
@@ -12978,14 +12894,76 @@
     }
 bad:
     Py_XDECREF(owned_instance);
     return;
 }
 #endif
 
+/* RaiseUnexpectedTypeError */
+static int
+__Pyx_RaiseUnexpectedTypeError(const char *expected, PyObject *obj)
+{
+    __Pyx_TypeName obj_type_name = __Pyx_PyType_GetName(Py_TYPE(obj));
+    PyErr_Format(PyExc_TypeError, "Expected %s, got " __Pyx_FMT_TYPENAME,
+                 expected, obj_type_name);
+    __Pyx_DECREF_TypeName(obj_type_name);
+    return 0;
+}
+
+/* decode_c_bytes */
+static CYTHON_INLINE PyObject* __Pyx_decode_c_bytes(
+         const char* cstring, Py_ssize_t length, Py_ssize_t start, Py_ssize_t stop,
+         const char* encoding, const char* errors,
+         PyObject* (*decode_func)(const char *s, Py_ssize_t size, const char *errors)) {
+    if (unlikely((start < 0) | (stop < 0))) {
+        if (start < 0) {
+            start += length;
+            if (start < 0)
+                start = 0;
+        }
+        if (stop < 0)
+            stop += length;
+    }
+    if (stop > length)
+        stop = length;
+    if (unlikely(stop <= start))
+        return __Pyx_NewRef(__pyx_empty_unicode);
+    length = stop - start;
+    cstring += start;
+    if (decode_func) {
+        return decode_func(cstring, length, errors);
+    } else {
+        return PyUnicode_Decode(cstring, length, encoding, errors);
+    }
+}
+
+/* DictGetItem */
+#if PY_MAJOR_VERSION >= 3 && !CYTHON_COMPILING_IN_PYPY
+static PyObject *__Pyx_PyDict_GetItem(PyObject *d, PyObject* key) {
+    PyObject *value;
+    value = PyDict_GetItemWithError(d, key);
+    if (unlikely(!value)) {
+        if (!PyErr_Occurred()) {
+            if (unlikely(PyTuple_Check(key))) {
+                PyObject* args = PyTuple_Pack(1, key);
+                if (likely(args)) {
+                    PyErr_SetObject(PyExc_KeyError, args);
+                    Py_DECREF(args);
+                }
+            } else {
+                PyErr_SetObject(PyExc_KeyError, key);
+            }
+        }
+        return NULL;
+    }
+    Py_INCREF(value);
+    return value;
+}
+#endif
+
 /* IterFinish */
 static CYTHON_INLINE int __Pyx_IterFinish(void) {
 #if CYTHON_FAST_THREAD_STATE
     PyThreadState *tstate = __Pyx_PyThreadState_Current;
     PyObject* exc_type = tstate->curexc_type;
     if (unlikely(exc_type)) {
         if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) {
@@ -13013,78 +12991,14 @@
             return -1;
         }
     }
     return 0;
 #endif
 }
 
-/* set_iter */
-static CYTHON_INLINE PyObject* __Pyx_set_iterator(PyObject* iterable, int is_set,
-                                                  Py_ssize_t* p_orig_length, int* p_source_is_set) {
-#if CYTHON_COMPILING_IN_CPYTHON
-    is_set = is_set || likely(PySet_CheckExact(iterable) || PyFrozenSet_CheckExact(iterable));
-    *p_source_is_set = is_set;
-    if (likely(is_set)) {
-        *p_orig_length = PySet_Size(iterable);
-        Py_INCREF(iterable);
-        return iterable;
-    }
-#else
-    (void)is_set;
-    *p_source_is_set = 0;
-#endif
-    *p_orig_length = 0;
-    return PyObject_GetIter(iterable);
-}
-static CYTHON_INLINE int __Pyx_set_iter_next(
-        PyObject* iter_obj, Py_ssize_t orig_length,
-        Py_ssize_t* ppos, PyObject **value,
-        int source_is_set) {
-    if (!CYTHON_COMPILING_IN_CPYTHON || unlikely(!source_is_set)) {
-        *value = PyIter_Next(iter_obj);
-        if (unlikely(!*value)) {
-            return __Pyx_IterFinish();
-        }
-        (void)orig_length;
-        (void)ppos;
-        return 1;
-    }
-#if CYTHON_COMPILING_IN_CPYTHON
-    if (unlikely(PySet_GET_SIZE(iter_obj) != orig_length)) {
-        PyErr_SetString(
-            PyExc_RuntimeError,
-            "set changed size during iteration");
-        return -1;
-    }
-    {
-        Py_hash_t hash;
-        int ret = _PySet_NextEntry(iter_obj, ppos, value, &hash);
-        assert (ret != -1);
-        if (likely(ret)) {
-            Py_INCREF(*value);
-            return 1;
-        }
-    }
-#endif
-    return 0;
-}
-
-/* GetAttr */
-static CYTHON_INLINE PyObject *__Pyx_GetAttr(PyObject *o, PyObject *n) {
-#if CYTHON_USE_TYPE_SLOTS
-#if PY_MAJOR_VERSION >= 3
-    if (likely(PyUnicode_Check(n)))
-#else
-    if (likely(PyString_Check(n)))
-#endif
-        return __Pyx_PyObject_GetAttrStr(o, n);
-#endif
-    return PyObject_GetAttr(o, n);
-}
-
 /* PyObjectCallNoArg */
 static CYTHON_INLINE PyObject* __Pyx_PyObject_CallNoArg(PyObject *func) {
     PyObject *arg = NULL;
     return __Pyx_PyObject_FastCall(func, (&arg)+1, 0 | __Pyx_PY_VECTORCALL_ARGUMENTS_OFFSET);
 }
 
 /* PyObjectGetMethod */
@@ -13404,68 +13318,14 @@
         *pkey = next_item;
     } else {
         *pvalue = next_item;
     }
     return 1;
 }
 
-/* pyfrozenset_new */
-static CYTHON_INLINE PyObject* __Pyx_PyFrozenSet_New(PyObject* it) {
-    if (it) {
-        PyObject* result;
-#if CYTHON_COMPILING_IN_PYPY
-        PyObject* args;
-        args = PyTuple_Pack(1, it);
-        if (unlikely(!args))
-            return NULL;
-        result = PyObject_Call((PyObject*)&PyFrozenSet_Type, args, NULL);
-        Py_DECREF(args);
-        return result;
-#else
-        if (PyFrozenSet_CheckExact(it)) {
-            Py_INCREF(it);
-            return it;
-        }
-        result = PyFrozenSet_New(it);
-        if (unlikely(!result))
-            return NULL;
-        if ((PY_VERSION_HEX >= 0x031000A1) || likely(PySet_GET_SIZE(result)))
-            return result;
-        Py_DECREF(result);
-#endif
-    }
-#if CYTHON_USE_TYPE_SLOTS
-    return PyFrozenSet_Type.tp_new(&PyFrozenSet_Type, __pyx_empty_tuple, NULL);
-#else
-    return PyObject_Call((PyObject*)&PyFrozenSet_Type, __pyx_empty_tuple, NULL);
-#endif
-}
-
-/* PySetContains */
-static int __Pyx_PySet_ContainsUnhashable(PyObject *set, PyObject *key) {
-    int result = -1;
-    if (PySet_Check(key) && PyErr_ExceptionMatches(PyExc_TypeError)) {
-        PyObject *tmpkey;
-        PyErr_Clear();
-        tmpkey = __Pyx_PyFrozenSet_New(key);
-        if (tmpkey != NULL) {
-            result = PySet_Contains(set, tmpkey);
-            Py_DECREF(tmpkey);
-        }
-    }
-    return result;
-}
-static CYTHON_INLINE int __Pyx_PySet_ContainsTF(PyObject* key, PyObject* set, int eq) {
-    int result = PySet_Contains(set, key);
-    if (unlikely(result < 0)) {
-        result = __Pyx_PySet_ContainsUnhashable(set, key);
-    }
-    return unlikely(result < 0) ? result : (result == (eq == Py_EQ));
-}
-
 /* decode_c_string */
 static CYTHON_INLINE PyObject* __Pyx_decode_c_string(
          const char* cstring, Py_ssize_t start, Py_ssize_t stop,
          const char* encoding, const char* errors,
          PyObject* (*decode_func)(const char *s, Py_ssize_t size, const char *errors)) {
     Py_ssize_t length;
     if (unlikely((start < 0) | (stop < 0))) {
@@ -13606,25 +13466,14 @@
         return __Pyx_NewRef(result);
     }
     PyErr_Clear();
 #endif
     return __Pyx_GetBuiltinName(name);
 }
 
-/* RaiseUnexpectedTypeError */
-static int
-__Pyx_RaiseUnexpectedTypeError(const char *expected, PyObject *obj)
-{
-    __Pyx_TypeName obj_type_name = __Pyx_PyType_GetName(Py_TYPE(obj));
-    PyErr_Format(PyExc_TypeError, "Expected %s, got " __Pyx_FMT_TYPENAME,
-                 expected, obj_type_name);
-    __Pyx_DECREF_TypeName(obj_type_name);
-    return 0;
-}
-
 /* GetTopmostException */
 #if CYTHON_USE_EXC_INFO_STACK
 static _PyErr_StackItem *
 __Pyx_PyErr_GetTopmostException(PyThreadState *tstate)
 {
     _PyErr_StackItem *exc_info = tstate->exc_info;
     while ((exc_info->exc_type == NULL || exc_info->exc_type == Py_None) &&
@@ -14377,15 +14226,15 @@
         PyObject* module_dot = 0;
         PyObject* full_name = 0;
         PyErr_Clear();
         module_name_str = PyModule_GetName(module);
         if (unlikely(!module_name_str)) { goto modbad; }
         module_name = PyUnicode_FromString(module_name_str);
         if (unlikely(!module_name)) { goto modbad; }
-        module_dot = PyUnicode_Concat(module_name, __pyx_kp_u__2);
+        module_dot = PyUnicode_Concat(module_name, __pyx_kp_u__3);
         if (unlikely(!module_dot)) { goto modbad; }
         full_name = PyUnicode_Concat(module_dot, name);
         if (unlikely(!full_name)) { goto modbad; }
         #if PY_VERSION_HEX < 0x030700A1 || (CYTHON_COMPILING_IN_PYPY && PYPY_VERSION_NUM  < 0x07030400)
         {
             PyObject *modules = PyImport_GetModuleDict();
             if (unlikely(!modules))
@@ -15443,43 +15292,14 @@
     );
     if (likely(op)) {
         PyObject_GC_Track(op);
     }
     return op;
 }
 
-/* unicode_tailmatch */
-static int __Pyx_PyUnicode_TailmatchTuple(PyObject* s, PyObject* substrings,
-                                          Py_ssize_t start, Py_ssize_t end, int direction) {
-    Py_ssize_t i, count = PyTuple_GET_SIZE(substrings);
-    for (i = 0; i < count; i++) {
-        Py_ssize_t result;
-#if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        result = PyUnicode_Tailmatch(s, PyTuple_GET_ITEM(substrings, i),
-                                     start, end, direction);
-#else
-        PyObject* sub = PySequence_ITEM(substrings, i);
-        if (unlikely(!sub)) return -1;
-        result = PyUnicode_Tailmatch(s, sub, start, end, direction);
-        Py_DECREF(sub);
-#endif
-        if (result) {
-            return (int) result;
-        }
-    }
-    return 0;
-}
-static int __Pyx_PyUnicode_Tailmatch(PyObject* s, PyObject* substr,
-                                     Py_ssize_t start, Py_ssize_t end, int direction) {
-    if (unlikely(PyTuple_Check(substr))) {
-        return __Pyx_PyUnicode_TailmatchTuple(s, substr, start, end, direction);
-    }
-    return (int) PyUnicode_Tailmatch(s, substr, start, end, direction);
-}
-
 /* CLineInTraceback */
 #ifndef CYTHON_CLINE_IN_TRACEBACK
 static int __Pyx_CLineForTraceback(CYTHON_NCP_UNUSED PyThreadState *tstate, int c_line) {
     PyObject *use_cline;
     PyObject *ptype, *pvalue, *ptraceback;
 #if CYTHON_COMPILING_IN_CPYTHON
     PyObject **cython_runtime_dict;
@@ -15721,14 +15541,33 @@
                 else\
                     goto raise_overflow;\
             }\
         }\
         return (target_type) value;\
     }
 
+static PyObject* __pyx_convert__to_py_LexerData(LexerData s) {
+  PyObject* res;
+  PyObject* member;
+  res = __Pyx_PyDict_NewPresized(3); if (unlikely(!res)) return NULL;
+  member = __Pyx_PyObject_FromString(s.filename); if (unlikely(!member)) goto bad;
+  if (unlikely(PyDict_SetItem(res, __pyx_n_s_filename, member) < 0)) goto bad;
+  Py_DECREF(member);
+  member = __Pyx_PyInt_From_uint8_t(s.command_threshold); if (unlikely(!member)) goto bad;
+  if (unlikely(PyDict_SetItem(res, __pyx_n_s_command_threshold, member) < 0)) goto bad;
+  Py_DECREF(member);
+  member = __Pyx_PyInt_From_uint8_t(s.flag); if (unlikely(!member)) goto bad;
+  if (unlikely(PyDict_SetItem(res, __pyx_n_s_flag, member) < 0)) goto bad;
+  Py_DECREF(member);
+  return res;
+  bad:
+  Py_XDECREF(member);
+  Py_DECREF(res);
+  return NULL;
+}
 /* CIntToPy */
 static CYTHON_INLINE PyObject* __Pyx_PyInt_From_enum__TokenSyn(enum TokenSyn value) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const enum TokenSyn neg_one = (enum TokenSyn) -1, const_zero = (enum TokenSyn) 0;
```

### Comparing `KoiLang-1.1.0/kola/lexer.pxd` & `KoiLang-1.1.0b2/kola/lexer.pxd`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,14 @@
 cimport cython
 from libc.stdio cimport stdin, FILE, fopen, fclose, EOF
 from cpython cimport PyObject
 
 from ._cutil cimport *
 
 
-cdef extern from *:
-    bint PyDescr_IsData(object desc)
-
-
 cdef class Token:
     cdef:
         Token next     # used in grammar parser
     cdef readonly:
         TokenSyn syn
         object val
         bytes raw_val
```

### Comparing `KoiLang-1.1.0/kola/lexer.pyi` & `KoiLang-1.1.0b2/kola/lexer.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import os
-from typing import Any, ClassVar, Final, FrozenSet, Union, final, TypedDict
+from typing import Any, Final, Union, final, TypedDict
 from typing_extensions import Self
 
 
 S_CMD: int
 S_CMD_N: int
 S_TEXT: int
 S_LITERAL: int
@@ -44,16 +44,14 @@
     def get_flag(self) -> int: ...
 
 
 class LexerConfig:
     """
     Python-level interface to access extra lexer data
     """
-    data_names: ClassVar[FrozenSet[str]]
-
     def __init__(self, lexer: BaseLexer) -> None: ...
     def dict(self) -> _LexerData: ...
     def set(
         self,
         *,
         encoding: str = ...,
         command_threshold: int = ...,
```

### Comparing `KoiLang-1.1.0/kola/lib/__init__.py` & `KoiLang-1.1.0b2/kola/lib/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,105 +1,74 @@
-"""
-Kola sub libraries support modules
-
-Include some useful builtin kola sub module.
-And modules imported from `load_library()` will be mounted as a sub module.
-"""
-
 import inspect
 import os
 import re
 import sys
 from glob import glob
 from importlib.util import spec_from_file_location
 from importlib._bootstrap import _load
 from types import ModuleType
 from typing import List, NamedTuple, Optional, Type
 
 from ..klvm import CommandSetMeta, KoiLang
 
 
-if "KOLA_LIB_PATH" in os.environ:  # pragma: no cover
+if "KOLA_LIB_PATH" in os.environ:
     KOLA_LIB_PATH = os.environ["KOLA_LIB_PATH"].split(os.pathsep)
 else:
     KOLA_LIB_PATH = ['.', './kola_lib', os.path.dirname(__file__)]
 
 
 _module_pattern = re.compile(r"^[A-Za-z_]\w*(?:\.[A-Za-z_]\w*)*$", re.A)
 
 
 class KolaSpec(NamedTuple):
-    """
-    Kola module spec
-    
-    Usage:
-        __kola_spec__ = KolaSpec(
-            __name__,
-            collect_all()
-        )
-    """
     name: str
     command_set_classes: List[CommandSetMeta]
     
     doc: Optional[str] = None
     main_class: Optional[Type[KoiLang]] = None
 
 
 def collect_all() -> List[CommandSetMeta]:
-    """get all CommandSet class defined in the module
-
-    :return: a list of CommandSet class found
-    :rtype: List[CommandSetMeta]
-    """
     frame = inspect.currentframe()
-    if not frame or not frame.f_back:  # pragma: no cover
-        raise ValueError("cannot read variables from the frame")
+    assert frame and frame.f_back
     return [
         i for i in frame.f_back.f_locals.values()
         if isinstance(i, CommandSetMeta)
     ]
 
 
-def load_library(name: str, paths: List[str] = KOLA_LIB_PATH) -> ModuleType:
-    """load a Phython script or package as a Kola module
-
-    :param name: module name like 'mymodule.sub'
-    :type name: str
-    :param paths: base path to load the module, defaults to KOLA_LIB_PATH
-    :type paths: List[str], optional
-    :raises ValueError: illegal module name
-    :raises ImportError: fail to load the module
-    :return: the Kola module
-    :rtype: ModuleType
-    """
-    if not _module_pattern.match(name):  # pragma: no cover
+def load_library(name: str, bases: List[str] = KOLA_LIB_PATH) -> ModuleType:
+    if not _module_pattern.match(name):
         raise ValueError(f"illegal module name '{name}'")
     module_name = "kola.lib." + name
     if module_name in sys.modules:
         return sys.modules[module_name]
 
-    for b in paths:
+    for b in bases:
         spec = None
         b = os.path.abspath(b)
         full_path = os.path.join(b, name)
-        if os.path.isdir(full_path):
+        if os.path.isfile(full_path):
+            spec = spec_from_file_location(module_name, full_path)
+        elif os.path.isdir(full_path):
             spec = spec_from_file_location(
                 module_name, os.path.join(full_path, "__init__.py"),
                 submodule_search_locations=[full_path]
             )
         else:
             for i in glob(full_path + '.*'):
                 spec = spec_from_file_location(module_name, i)
                 if spec:
                     full_path = i
                     break
         if spec:
             spec.name = module_name
             return _load(spec)
-    raise ImportError(f"cannot load script {name}", name=name)  # pragma: no cover
+    raise ImportError(f"cannot load script {name}", name=name)
 
 
 def main_class_from_module(module: ModuleType) -> Type[KoiLang]:
     spec = getattr(module, "__kola_spec__", None)
     if spec:
         if not isinstance(spec, KolaSpec):
             spec = KolaSpec(*spec)
@@ -108,10 +77,10 @@
         for i in spec.command_set_classes:
             if issubclass(i, KoiLang):
                 return i
     else:
         for i in module.__dict__.values():
             if isinstance(i, type) and issubclass(i, KoiLang) and i is not KoiLang:
                 return i
-    raise ValueError(  # pragma: no cover
+    raise ValueError(
         f"no available main class for kola module '{spec.name if spec else module.__name__}'"
     )
```

### Comparing `KoiLang-1.1.0/kola/lib/debugger/base.py` & `KoiLang-1.1.0b2/kola/lib/debugger/base.py`

 * *Files identical despite different names*

### Comparing `KoiLang-1.1.0/kola/lib/debugger/default_runner.py` & `KoiLang-1.1.0b2/kola/lib/debugger/default_runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -168,23 +168,23 @@
             command,
             tuple(self.format_text(i) for i in args),
             self.format_text(kwargs),
             bound_instance=bound_instance,
             **kwds
         )
     
-    def push_apply(self, __push_cache: Environment) -> None:
+    def push_end(self, __push_cache: Environment) -> None:
         if self.flag & FLAG_DEBUG:
             print(f"## [DEBUG] Push env: {__push_cache}")
-        return super().push_apply(__push_cache)
+        return super().push_end(__push_cache)
     
-    def pop_apply(self, __env_cache: Environment) -> None:
+    def pop_end(self, __env_cache: Environment) -> None:
         if self.flag & FLAG_DEBUG:
             print(f"## [DEBUG] Pop env: {__env_cache}")
-        return super().pop_apply(__env_cache)
+        return super().pop_end(__env_cache)
 
 
 __kola_spec__ = KolaSpec(
     "Kola Runner",
     collect_all(),
     main_class=KoiLangRunner
 )
```

### Comparing `KoiLang-1.1.0/kola/lib/fast_file.py` & `KoiLang-1.1.0b2/kola/lib/fast_file.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,17 +26,17 @@
                 raise ValueError(f"invalid seek whence {__whence}")
             self.fp.seek(__cookie, __whence)
         
         @kola_text
         def text(self, text: str) -> None:
             self.fp.write(text)
 
-        def tear_down(self, cur_top: CommandSet) -> None:
+        def at_finalize(self, cur_top: CommandSet) -> None:
             self.fp.close()
-            return super().tear_down(cur_top)
+            return super().at_finalize(cur_top)
     
     class space(Environment):
         @kola_env_enter("space", envs="!file")
         def enter(self, name: Optional[str] = None, path: Optional[Union[str, bytes, os.PathLike]] = None) -> None:
             self.pwd = os.getcwd()
             if not path:
                 assert name
@@ -47,15 +47,15 @@
                 os.makedirs(path)
             os.chdir(path)
         
         @kola_env_exit("endspace")
         def exit(self) -> None:
             os.chdir(self.pwd)
         
-        def set_up(self, cur_top: CommandSet) -> None:
+        def at_initialize(self, cur_top: CommandSet) -> None:
             if isinstance(cur_top, FastFile.file):
                 home = self.home
-                cache = home.pop_prepare()
-                home.pop_apply(cache)
+                cache = home.pop_start()
+                home.pop_end(cache)
                 # update self.back
                 self.back = home.top
-            return super().set_up(cur_top)
+            return super().at_initialize(cur_top)
```

### Comparing `KoiLang-1.1.0/kola/parser.c` & `KoiLang-1.1.0b2/kola/parser.c`

 * *Files 0% similar despite different names*

```diff
@@ -1241,15 +1241,15 @@
 struct __pyx_opt_args_7cpython_11contextvars_get_value_no_default {
   int __pyx_n;
   PyObject *default_value;
 };
 struct __pyx_ctuple_int__and_char__space_const__ptr__and_Py_ssize_t;
 typedef struct __pyx_ctuple_int__and_char__space_const__ptr__and_Py_ssize_t __pyx_ctuple_int__and_char__space_const__ptr__and_Py_ssize_t;
 
-/* "lexer.pxd":39
+/* "lexer.pxd":35
  *     cpdef void close(self)
  *     cdef void set_error(self, const char* text) except *
  *     cdef (int, const char*, Py_ssize_t) next_syn(self) nogil             # <<<<<<<<<<<<<<
  *     cdef Token next_token(self)
  * 
  */
 struct __pyx_ctuple_int__and_char__space_const__ptr__and_Py_ssize_t {
@@ -1268,15 +1268,15 @@
  */
 struct __pyx_opt_args_4kola_6parser_6Parser_set_error {
   int __pyx_n;
   int errorno;
   int recovery;
 };
 
-/* "lexer.pxd":12
+/* "lexer.pxd":8
  * 
  * 
  * cdef class Token:             # <<<<<<<<<<<<<<
  *     cdef:
  *         Token next     # used in grammar parser
  */
 struct __pyx_obj_4kola_5lexer_Token {
@@ -1286,29 +1286,29 @@
   enum TokenSyn syn;
   PyObject *val;
   PyObject *raw_val;
   int lineno;
 };
 
 
-/* "lexer.pxd":24
+/* "lexer.pxd":20
  * 
  * 
  * cdef class LexerConfig:             # <<<<<<<<<<<<<<
  *     cdef LexerData* lexer_data
  *     cdef readonly BaseLexer lexer
  */
 struct __pyx_obj_4kola_5lexer_LexerConfig {
   PyObject_HEAD
   LexerData *lexer_data;
   struct __pyx_obj_4kola_5lexer_BaseLexer *lexer;
 };
 
 
-/* "lexer.pxd":30
+/* "lexer.pxd":26
  * 
  * @cython.no_gc
  * cdef class BaseLexer:             # <<<<<<<<<<<<<<
  *     cdef:
  *         yyscan_t scanner
  */
 struct __pyx_obj_4kola_5lexer_BaseLexer {
@@ -1316,30 +1316,30 @@
   struct __pyx_vtabstruct_4kola_5lexer_BaseLexer *__pyx_vtab;
   yyscan_t scanner;
   LexerData lexer_data;
   PyObject *encoding;
 };
 
 
-/* "lexer.pxd":43
+/* "lexer.pxd":39
  * 
  * 
  * cdef class FileLexer(BaseLexer):             # <<<<<<<<<<<<<<
  *     cdef:
  *         object _filenameo
  */
 struct __pyx_obj_4kola_5lexer_FileLexer {
   struct __pyx_obj_4kola_5lexer_BaseLexer __pyx_base;
   PyObject *_filenameo;
   PyObject *_filenameb;
   FILE *fp;
 };
 
 
-/* "lexer.pxd":53
+/* "lexer.pxd":49
  * 
  * @cython.no_gc
  * cdef class StringLexer(BaseLexer):             # <<<<<<<<<<<<<<
  *     cdef readonly bytes content
  */
 struct __pyx_obj_4kola_5lexer_StringLexer {
   struct __pyx_obj_4kola_5lexer_BaseLexer __pyx_base;
@@ -1362,29 +1362,29 @@
   uint8_t stat;
   struct __pyx_obj_4kola_5lexer_BaseLexer *lexer;
   PyObject *command_set;
 };
 
 
 
-/* "lexer.pxd":12
+/* "lexer.pxd":8
  * 
  * 
  * cdef class Token:             # <<<<<<<<<<<<<<
  *     cdef:
  *         Token next     # used in grammar parser
  */
 
 struct __pyx_vtabstruct_4kola_5lexer_Token {
   int (*get_flag)(struct __pyx_obj_4kola_5lexer_Token *, int __pyx_skip_dispatch);
 };
 static struct __pyx_vtabstruct_4kola_5lexer_Token *__pyx_vtabptr_4kola_5lexer_Token;
 
 
-/* "lexer.pxd":30
+/* "lexer.pxd":26
  * 
  * @cython.no_gc
  * cdef class BaseLexer:             # <<<<<<<<<<<<<<
  *     cdef:
  *         yyscan_t scanner
  */
 
@@ -1393,29 +1393,29 @@
   void (*set_error)(struct __pyx_obj_4kola_5lexer_BaseLexer *, char const *);
   __pyx_ctuple_int__and_char__space_const__ptr__and_Py_ssize_t (*next_syn)(struct __pyx_obj_4kola_5lexer_BaseLexer *);
   struct __pyx_obj_4kola_5lexer_Token *(*next_token)(struct __pyx_obj_4kola_5lexer_BaseLexer *);
 };
 static struct __pyx_vtabstruct_4kola_5lexer_BaseLexer *__pyx_vtabptr_4kola_5lexer_BaseLexer;
 
 
-/* "lexer.pxd":43
+/* "lexer.pxd":39
  * 
  * 
  * cdef class FileLexer(BaseLexer):             # <<<<<<<<<<<<<<
  *     cdef:
  *         object _filenameo
  */
 
 struct __pyx_vtabstruct_4kola_5lexer_FileLexer {
   struct __pyx_vtabstruct_4kola_5lexer_BaseLexer __pyx_base;
 };
 static struct __pyx_vtabstruct_4kola_5lexer_FileLexer *__pyx_vtabptr_4kola_5lexer_FileLexer;
 
 
-/* "lexer.pxd":53
+/* "lexer.pxd":49
  * 
  * @cython.no_gc
  * cdef class StringLexer(BaseLexer):             # <<<<<<<<<<<<<<
  *     cdef readonly bytes content
  */
 
 struct __pyx_vtabstruct_4kola_5lexer_StringLexer {
@@ -8837,30 +8837,30 @@
    if (!__pyx_ptype_7cpython_4bool_bool) __PYX_ERR(4, 8, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(5, 15, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_7cpython_7complex_complex = __Pyx_ImportType(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "complex", sizeof(PyComplexObject), __Pyx_ImportType_CheckSize_Warn);
    if (!__pyx_ptype_7cpython_7complex_complex) __PYX_ERR(5, 15, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = PyImport_ImportModule("kola.lexer"); if (unlikely(!__pyx_t_1)) __PYX_ERR(6, 12, __pyx_L1_error)
+  __pyx_t_1 = PyImport_ImportModule("kola.lexer"); if (unlikely(!__pyx_t_1)) __PYX_ERR(6, 8, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_4kola_5lexer_Token = __Pyx_ImportType(__pyx_t_1, "kola.lexer", "Token", sizeof(struct __pyx_obj_4kola_5lexer_Token), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_4kola_5lexer_Token) __PYX_ERR(6, 12, __pyx_L1_error)
-  __pyx_vtabptr_4kola_5lexer_Token = (struct __pyx_vtabstruct_4kola_5lexer_Token*)__Pyx_GetVtable(__pyx_ptype_4kola_5lexer_Token); if (unlikely(!__pyx_vtabptr_4kola_5lexer_Token)) __PYX_ERR(6, 12, __pyx_L1_error)
+   if (!__pyx_ptype_4kola_5lexer_Token) __PYX_ERR(6, 8, __pyx_L1_error)
+  __pyx_vtabptr_4kola_5lexer_Token = (struct __pyx_vtabstruct_4kola_5lexer_Token*)__Pyx_GetVtable(__pyx_ptype_4kola_5lexer_Token); if (unlikely(!__pyx_vtabptr_4kola_5lexer_Token)) __PYX_ERR(6, 8, __pyx_L1_error)
   __pyx_ptype_4kola_5lexer_LexerConfig = __Pyx_ImportType(__pyx_t_1, "kola.lexer", "LexerConfig", sizeof(struct __pyx_obj_4kola_5lexer_LexerConfig), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_4kola_5lexer_LexerConfig) __PYX_ERR(6, 24, __pyx_L1_error)
+   if (!__pyx_ptype_4kola_5lexer_LexerConfig) __PYX_ERR(6, 20, __pyx_L1_error)
   __pyx_ptype_4kola_5lexer_BaseLexer = __Pyx_ImportType(__pyx_t_1, "kola.lexer", "BaseLexer", sizeof(struct __pyx_obj_4kola_5lexer_BaseLexer), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_4kola_5lexer_BaseLexer) __PYX_ERR(6, 30, __pyx_L1_error)
-  __pyx_vtabptr_4kola_5lexer_BaseLexer = (struct __pyx_vtabstruct_4kola_5lexer_BaseLexer*)__Pyx_GetVtable(__pyx_ptype_4kola_5lexer_BaseLexer); if (unlikely(!__pyx_vtabptr_4kola_5lexer_BaseLexer)) __PYX_ERR(6, 30, __pyx_L1_error)
+   if (!__pyx_ptype_4kola_5lexer_BaseLexer) __PYX_ERR(6, 26, __pyx_L1_error)
+  __pyx_vtabptr_4kola_5lexer_BaseLexer = (struct __pyx_vtabstruct_4kola_5lexer_BaseLexer*)__Pyx_GetVtable(__pyx_ptype_4kola_5lexer_BaseLexer); if (unlikely(!__pyx_vtabptr_4kola_5lexer_BaseLexer)) __PYX_ERR(6, 26, __pyx_L1_error)
   __pyx_ptype_4kola_5lexer_FileLexer = __Pyx_ImportType(__pyx_t_1, "kola.lexer", "FileLexer", sizeof(struct __pyx_obj_4kola_5lexer_FileLexer), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_4kola_5lexer_FileLexer) __PYX_ERR(6, 43, __pyx_L1_error)
-  __pyx_vtabptr_4kola_5lexer_FileLexer = (struct __pyx_vtabstruct_4kola_5lexer_FileLexer*)__Pyx_GetVtable(__pyx_ptype_4kola_5lexer_FileLexer); if (unlikely(!__pyx_vtabptr_4kola_5lexer_FileLexer)) __PYX_ERR(6, 43, __pyx_L1_error)
+   if (!__pyx_ptype_4kola_5lexer_FileLexer) __PYX_ERR(6, 39, __pyx_L1_error)
+  __pyx_vtabptr_4kola_5lexer_FileLexer = (struct __pyx_vtabstruct_4kola_5lexer_FileLexer*)__Pyx_GetVtable(__pyx_ptype_4kola_5lexer_FileLexer); if (unlikely(!__pyx_vtabptr_4kola_5lexer_FileLexer)) __PYX_ERR(6, 39, __pyx_L1_error)
   __pyx_ptype_4kola_5lexer_StringLexer = __Pyx_ImportType(__pyx_t_1, "kola.lexer", "StringLexer", sizeof(struct __pyx_obj_4kola_5lexer_StringLexer), __Pyx_ImportType_CheckSize_Warn);
-   if (!__pyx_ptype_4kola_5lexer_StringLexer) __PYX_ERR(6, 53, __pyx_L1_error)
-  __pyx_vtabptr_4kola_5lexer_StringLexer = (struct __pyx_vtabstruct_4kola_5lexer_StringLexer*)__Pyx_GetVtable(__pyx_ptype_4kola_5lexer_StringLexer); if (unlikely(!__pyx_vtabptr_4kola_5lexer_StringLexer)) __PYX_ERR(6, 53, __pyx_L1_error)
+   if (!__pyx_ptype_4kola_5lexer_StringLexer) __PYX_ERR(6, 49, __pyx_L1_error)
+  __pyx_vtabptr_4kola_5lexer_StringLexer = (struct __pyx_vtabstruct_4kola_5lexer_StringLexer*)__Pyx_GetVtable(__pyx_ptype_4kola_5lexer_StringLexer); if (unlikely(!__pyx_vtabptr_4kola_5lexer_StringLexer)) __PYX_ERR(6, 49, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
```

### Comparing `KoiLang-1.1.0/kola/parser.pxd` & `KoiLang-1.1.0b2/kola/parser.pxd`

 * *Files identical despite different names*

### Comparing `KoiLang-1.1.0/kola/parser.pyi` & `KoiLang-1.1.0b2/kola/parser.pyi`

 * *Files identical despite different names*

### Comparing `KoiLang-1.1.0/kola/unicode_handler.c` & `KoiLang-1.1.0b2/kola/unicode_handler.c`

 * *Files identical despite different names*

### Comparing `KoiLang-1.1.0/kola/writer.c` & `KoiLang-1.1.0b2/kola/writer.c`

 * *Files identical despite different names*

### Comparing `KoiLang-1.1.0/kola/writer.pxd` & `KoiLang-1.1.0b2/kola/writer.pxd`

 * *Files identical despite different names*

### Comparing `KoiLang-1.1.0/kola/writer.pyi` & `KoiLang-1.1.0b2/kola/writer.pyi`

 * *Files identical despite different names*

### Comparing `KoiLang-1.1.0/setup.py` & `KoiLang-1.1.0b2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Copyright 2023 Ovizro
+Copyright 2022 Ovizro
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

