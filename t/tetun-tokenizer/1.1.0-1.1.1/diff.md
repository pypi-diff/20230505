# Comparing `tmp/tetun_tokenizer-1.1.0.tar.gz` & `tmp/tetun_tokenizer-1.1.1.tar.gz`

## Comparing `tetun_tokenizer-1.1.0.tar` & `tetun_tokenizer-1.1.1.tar`

### file list

```diff
@@ -1,13 +1,12 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 tetun_tokenizer-1.1.0/.DS_Store
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 tetun_tokenizer-1.1.0/Pipfile
--rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 tetun_tokenizer-1.1.0/Pipfile.lock
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 tetun_tokenizer-1.1.0/_token
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 tetun_tokenizer-1.1.0/.vscode/settings.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tetun_tokenizer-1.1.0/tetuntokenizer/__init__.py
--rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 tetun_tokenizer-1.1.0/tetuntokenizer/tokenizer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tetun_tokenizer-1.1.0/tetuntokenizer/config/__init__.py
--rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 tetun_tokenizer-1.1.0/tetuntokenizer/config/tetun_patterns.py
--rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 tetun_tokenizer-1.1.0/LICENSE
--rw-r--r--   0        0        0     5078 2020-02-02 00:00:00.000000 tetun_tokenizer-1.1.0/README.md
--rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 tetun_tokenizer-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     5456 2020-02-02 00:00:00.000000 tetun_tokenizer-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 tetun_tokenizer-1.1.1/.DS_Store
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 tetun_tokenizer-1.1.1/Pipfile
+-rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 tetun_tokenizer-1.1.1/Pipfile.lock
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 tetun_tokenizer-1.1.1/_token
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 tetun_tokenizer-1.1.1/.vscode/settings.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tetun_tokenizer-1.1.1/tetuntokenizer/__init__.py
+-rw-r--r--   0        0        0      957 2020-02-02 00:00:00.000000 tetun_tokenizer-1.1.1/tetuntokenizer/tetun_patterns.py
+-rw-r--r--   0        0        0     3233 2020-02-02 00:00:00.000000 tetun_tokenizer-1.1.1/tetuntokenizer/tokenizer.py
+-rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 tetun_tokenizer-1.1.1/LICENSE
+-rw-r--r--   0        0        0     5078 2020-02-02 00:00:00.000000 tetun_tokenizer-1.1.1/README.md
+-rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 tetun_tokenizer-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     5456 2020-02-02 00:00:00.000000 tetun_tokenizer-1.1.1/PKG-INFO
```

### Comparing `tetun_tokenizer-1.1.0/.DS_Store` & `tetun_tokenizer-1.1.1/.DS_Store`

 * *Files identical despite different names*

### Comparing `tetun_tokenizer-1.1.0/Pipfile.lock` & `tetun_tokenizer-1.1.1/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `tetun_tokenizer-1.1.0/tetuntokenizer/tokenizer.py` & `tetun_tokenizer-1.1.1/tetuntokenizer/tokenizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 * tokenize the input string by extracting only string and number and ignore punctuations and special characters.
 * tokenize the input string by extracting only string and ignore numbers, punctuations, and special characters.
 
 Note: please cite tetun-tokenizer if you use it for scientific publication purposes or contribute to a community.
 """
 import re
 from typing import List
-from config import tetun_patterns
+from . import tetun_patterns
 
 
 class TetunRegexTokenizer:
     """Tokenizes text using regular expressions."""
 
     def __init__(self, patterns: str, split: bool = False) -> None:
         """
```

### Comparing `tetun_tokenizer-1.1.0/tetuntokenizer/config/tetun_patterns.py` & `tetun_tokenizer-1.1.1/tetuntokenizer/tetun_patterns.py`

 * *Files identical despite different names*

### Comparing `tetun_tokenizer-1.1.0/LICENSE` & `tetun_tokenizer-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tetun_tokenizer-1.1.0/README.md` & `tetun_tokenizer-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `tetun_tokenizer-1.1.0/PKG-INFO` & `tetun_tokenizer-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tetun_tokenizer
-Version: 1.1.0
+Version: 1.1.1
 Summary: Tetun tokenizer
 Author-email: Gabriel de Jesus <gabriel.dejesus@timornews.tl>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

