# Comparing `tmp/folint-1.0.3.tar.gz` & `tmp/folint-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "folint-1.0.3.tar", last modified: Wed Sep 28 07:35:41 2022, max compression
+gzip compressed data, was "folint-1.0.4.tar", last modified: Fri May  5 05:34:37 2023, max compression
```

## Comparing `folint-1.0.3.tar` & `folint-1.0.4.tar`

### file list

```diff
@@ -1,26 +1,25 @@
-drwxr-xr-x   0 saltfactory  (1000) sudo      (1001)        0 2022-09-28 07:35:41.954496 folint-1.0.3/
--rw-r--r--   0 saltfactory  (1000) sudo      (1001)    35149 2022-09-28 07:33:49.000000 folint-1.0.3/LICENSE
--rw-r--r--   0 saltfactory  (1000) sudo      (1001)       50 2022-09-28 07:33:49.000000 folint-1.0.3/MANIFEST.in
--rw-r--r--   0 saltfactory  (1000) sudo      (1001)     1233 2022-09-28 07:35:41.954496 folint-1.0.3/PKG-INFO
--rw-r--r--   0 saltfactory  (1000) sudo      (1001)      646 2022-09-28 07:33:49.000000 folint-1.0.3/README.md
-drwxr-xr-x   0 saltfactory  (1000) sudo      (1001)        0 2022-09-28 07:35:41.952496 folint-1.0.3/folint/
--rw-r--r--   0 saltfactory  (1000) sudo      (1001)      988 2022-09-28 07:33:49.000000 folint-1.0.3/folint/ASTprint.py
--rw-r--r--   0 saltfactory  (1000) sudo      (1001)    10967 2022-09-28 07:33:52.000000 folint-1.0.3/folint/SCA.py
--rw-r--r--   0 saltfactory  (1000) sudo      (1001)       14 2022-09-28 07:33:49.000000 folint-1.0.3/folint/__init__.py
-drwxr-xr-x   0 saltfactory  (1000) sudo      (1001)        0 2022-09-28 07:35:41.954496 folint-1.0.3/folint/ast_engine/
--rw-r--r--   0 saltfactory  (1000) sudo      (1001)    28978 2022-09-28 07:33:49.000000 folint-1.0.3/folint/ast_engine/Annotate.py
--rw-r--r--   0 saltfactory  (1000) sudo      (1001)     9808 2022-09-28 07:33:49.000000 folint-1.0.3/folint/ast_engine/Assignments.py
--rw-r--r--   0 saltfactory  (1000) sudo      (1001)    62132 2022-09-28 07:33:52.000000 folint-1.0.3/folint/ast_engine/Expression.py
--rw-r--r--   0 saltfactory  (1000) sudo      (1001)    58784 2022-09-28 07:33:52.000000 folint-1.0.3/folint/ast_engine/Parse.py
--rw-r--r--   0 saltfactory  (1000) sudo      (1001)    17338 2022-09-28 07:33:49.000000 folint-1.0.3/folint/ast_engine/Simplify.py
--rw-r--r--   0 saltfactory  (1000) sudo      (1001)       82 2022-09-28 07:33:49.000000 folint-1.0.3/folint/ast_engine/__init__.py
--rw-r--r--   0 saltfactory  (1000) sudo      (1001)     4287 2022-09-28 07:33:49.000000 folint-1.0.3/folint/ast_engine/utils.py
-drwxr-xr-x   0 saltfactory  (1000) sudo      (1001)        0 2022-09-28 07:35:41.953496 folint-1.0.3/folint.egg-info/
--rw-r--r--   0 saltfactory  (1000) sudo      (1001)     1233 2022-09-28 07:35:41.000000 folint-1.0.3/folint.egg-info/PKG-INFO
--rw-r--r--   0 saltfactory  (1000) sudo      (1001)      481 2022-09-28 07:35:41.000000 folint-1.0.3/folint.egg-info/SOURCES.txt
--rw-r--r--   0 saltfactory  (1000) sudo      (1001)        1 2022-09-28 07:35:41.000000 folint-1.0.3/folint.egg-info/dependency_links.txt
--rw-r--r--   0 saltfactory  (1000) sudo      (1001)       44 2022-09-28 07:35:41.000000 folint-1.0.3/folint.egg-info/entry_points.txt
--rw-r--r--   0 saltfactory  (1000) sudo      (1001)       22 2022-09-28 07:35:41.000000 folint-1.0.3/folint.egg-info/requires.txt
--rw-r--r--   0 saltfactory  (1000) sudo      (1001)        7 2022-09-28 07:35:41.000000 folint-1.0.3/folint.egg-info/top_level.txt
--rw-r--r--   0 saltfactory  (1000) sudo      (1001)       38 2022-09-28 07:35:41.954496 folint-1.0.3/setup.cfg
--rw-r--r--   0 saltfactory  (1000) sudo      (1001)     1096 2022-09-28 07:35:35.000000 folint-1.0.3/setup.py
+drwxr-xr-x   0 sva       (1000) sva       (1001)        0 2023-05-05 05:34:37.443359 folint-1.0.4/
+-rw-r--r--   0 sva       (1000) sva       (1001)    35149 2022-12-23 19:15:30.000000 folint-1.0.4/LICENSE
+-rw-r--r--   0 sva       (1000) sva       (1001)       50 2022-12-23 19:15:30.000000 folint-1.0.4/MANIFEST.in
+-rw-r--r--   0 sva       (1000) sva       (1001)     2891 2023-05-05 05:34:37.443359 folint-1.0.4/PKG-INFO
+-rw-r--r--   0 sva       (1000) sva       (1001)     2341 2023-04-13 06:56:56.000000 folint-1.0.4/README.md
+drwxr-xr-x   0 sva       (1000) sva       (1001)        0 2023-05-05 05:34:37.443359 folint-1.0.4/folint/
+-rw-r--r--   0 sva       (1000) sva       (1001)    10309 2023-05-05 05:21:40.000000 folint-1.0.4/folint/SCA.py
+-rw-r--r--   0 sva       (1000) sva       (1001)       14 2022-12-23 19:15:30.000000 folint-1.0.4/folint/__init__.py
+drwxr-xr-x   0 sva       (1000) sva       (1001)        0 2023-05-05 05:34:37.443359 folint-1.0.4/folint/ast_engine/
+-rw-r--r--   0 sva       (1000) sva       (1001)       34 2022-12-23 19:15:30.000000 folint-1.0.4/folint/ast_engine/Annotate.py
+-rw-r--r--   0 sva       (1000) sva       (1001)       36 2022-12-23 19:15:30.000000 folint-1.0.4/folint/ast_engine/Assignments.py
+-rw-r--r--   0 sva       (1000) sva       (1001)    16941 2023-05-05 05:21:40.000000 folint-1.0.4/folint/ast_engine/Expression.py
+-rw-r--r--   0 sva       (1000) sva       (1001)    11004 2023-04-20 07:12:10.000000 folint-1.0.4/folint/ast_engine/Parse.py
+-rw-r--r--   0 sva       (1000) sva       (1001)       34 2022-12-23 19:15:30.000000 folint-1.0.4/folint/ast_engine/Simplify.py
+-rw-r--r--   0 sva       (1000) sva       (1001)       82 2022-12-23 19:15:30.000000 folint-1.0.4/folint/ast_engine/__init__.py
+-rw-r--r--   0 sva       (1000) sva       (1001)       30 2022-12-23 19:15:30.000000 folint-1.0.4/folint/ast_engine/utils.py
+drwxr-xr-x   0 sva       (1000) sva       (1001)        0 2023-05-05 05:34:37.443359 folint-1.0.4/folint.egg-info/
+-rw-r--r--   0 sva       (1000) sva       (1001)     2891 2023-05-05 05:34:37.000000 folint-1.0.4/folint.egg-info/PKG-INFO
+-rw-r--r--   0 sva       (1000) sva       (1001)      462 2023-05-05 05:34:37.000000 folint-1.0.4/folint.egg-info/SOURCES.txt
+-rw-r--r--   0 sva       (1000) sva       (1001)        1 2023-05-05 05:34:37.000000 folint-1.0.4/folint.egg-info/dependency_links.txt
+-rw-r--r--   0 sva       (1000) sva       (1001)       43 2023-05-05 05:34:37.000000 folint-1.0.4/folint.egg-info/entry_points.txt
+-rw-r--r--   0 sva       (1000) sva       (1001)       41 2023-05-05 05:34:37.000000 folint-1.0.4/folint.egg-info/requires.txt
+-rw-r--r--   0 sva       (1000) sva       (1001)        7 2023-05-05 05:34:37.000000 folint-1.0.4/folint.egg-info/top_level.txt
+-rw-r--r--   0 sva       (1000) sva       (1001)       38 2023-05-05 05:34:37.443359 folint-1.0.4/setup.cfg
+-rw-r--r--   0 sva       (1000) sva       (1001)     1041 2023-05-05 05:33:45.000000 folint-1.0.4/setup.py
```

### Comparing `folint-1.0.3/LICENSE` & `folint-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `folint-1.0.3/folint/SCA.py` & `folint-1.0.4/folint/SCA.py`

 * *Files 4% similar despite different names*

```diff
@@ -103,15 +103,15 @@
 def extra_check(file, detections):
     pattern2 = re.compile(r"\/\/")  # Comments
     consistence = ''
     consistence_help = False
     unicode_symbols = ['⨯', '→', '𝔹', 'ℤ', 'ℝ', '∀', '∃', '∈', '∉', '←', '∧',
                        '∨', '¬', '⇒', '⇔', '⇐', '≤', '≠', '≥']
     ascii_symbols = ['*', '->', ' Bool ', ' Int ', ' Real ', '!', '?', ' in ',
-                     '<-', '&', '|', '~', '=>', '<=>', '<=', '=<',
+                     '<-', '&', '~', '=>', '<=>', '<=', '=<',
                      '~=', '>=']
     cur_block = None
     for line_number, line in enumerate(file.split('\n'), start=1):
         # Set the current block.
         if 'ocabulary' in line:
             cur_block = 'voc'
         elif 'tructure' in line:
@@ -125,20 +125,14 @@
             # Don't perform style checks on the main.
             continue
 
         # Ignore annotations.
         if line.strip().startswith('['):
             continue
 
-        # Some symbols should not have a space in front.
-        for match in re.finditer(r'\s,\s?', line):
-            detections.append((line_number, match.span()[0], match.span()[1],
-                               "Style: no space in front of a comma",
-                               "Warning"))
-
         # Some symbols should have a space in front.
         for match in re.finditer(r'[\w\)\d][*⨯><→⇒⇔≤≠≥=∉∈∧∨&|]', line):
             symbol = match.group()[1]
             detections.append((line_number, match.span()[0], match.span()[1],
                                f"Style: space in front of '{symbol}'",
                                "Warning"))
 
@@ -146,28 +140,20 @@
         for match in re.finditer(r'[,*⨯><→⇒⇔≤≠≥=∉∈][\w\d]', line):
             symbol = match.group()[0]
             detections.append((line_number, match.span()[0], match.span()[1],
                                f"Style: space after '{symbol}'",
                                "Warning"))
 
         # Some symbols should not be followed by a space.
-        for match in re.finditer(r'[~¬]s', line):
+        for match in re.finditer(r'[~¬]\s', line):
             symbol = match.group()[0]
             detections.append((line_number, match.span()[0], match.span()[1],
                                f"Style: no space allowed after '{symbol}'",
                                "Warning"))
 
-        # Comments on separate lines
-        for match in re.finditer(pattern2, line):
-            if len(line[0:match.span()[0]].strip()) != 0:
-                detections.append((line_number, match.span()[0],
-                                   match.span()[1],
-                                   "Style: comment should be on separate line",
-                                   "Warning"))
-
         # Don't allow multiple rules on the same line.
         if line.count('. ') > 1:
             detections.append((line_number, 0, len(line),
                                "Style: use new line for new rule",
                                "Warning"))
 
         # Correct use of indentation
@@ -222,33 +208,32 @@
     """ Lint FO(.) """
     start_time = time.time()
     output_str = ''
     try:
         total = 0
         idp = IDP.from_str(idp_file)  # Parse IDP file to AST.
 
-        # Print AST if requested.
-        if print_ast:
-            idp.printAST(0)
-
         # Execute the SCA!
         total, output_str = sca(idp)
 
         # Apply non-AST checks.
         number, extra_str = extra(idp_file)
         total += number
         output_str += extra_str
 
         output_str += f"\n---------- Total number detections: {total} ----------\n"
 
     except IDPZ3Error as e1:
         res1 = e1.args[0].split(': ', 1)
         res = res1[0].split()
         output_str += "\n---------- Syntax Error ----------\n"
-        output_str += f"{res[0]}: line {res[3].strip(',')} - colStart {res[5].strip(':')} - colEnd {res[5].strip(':')} => {res1[1]}\n"
+        if res1[0].startswith("Error on line") and 6 <= len(res):
+            output_str += f"{res[0]}: line {res[3].strip(',')} - colStart {res[5].strip(':')} - colEnd {res[5].strip(':')} => {res1[1]}\n"
+        else:
+            output_str += e1.args[0]
 
     except KeyError as e2:  # In case of KeyError
         output_str += f"Error: line {0} - colStart {0} - colEnd {0} => Key Error {e2}\n"
 
     except Exception as e:
         output_str += str(e) + '\n'
         output_str += "\n---------- Syntax Error ----------\n"
```

### Comparing `folint-1.0.3/setup.py` & `folint-1.0.4/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -6,29 +6,27 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="folint",
-    version="1.0.3",
+    version="1.0.4",
     description="Linter for FO-dot, used in the IDP-Z3 system",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://gitlab.com/EAVISE/sva/folint",
     author="vadevesi",
     author_email="s.vandevelde@kuleuven.be",
     classifiers=[
         'Topic :: Scientific/Engineering',
         'Topic :: Software Development',
         'Topic :: Scientific/Engineering :: Artificial Intelligence',
         'Topic :: Scientific/Engineering :: Mathematics',
         'Topic :: Software Development :: Quality Assurance'
       ],
     packages=find_packages(),
-    include_package_data=True,
-    package_data={'': ['ast_engine/Idp.tx']},
-    install_requires=["textX", "z3-solver", "click"],
+    install_requires=["textX", "z3-solver", "click", "idp_engine==0.10.2"],
     entry_points={
       'console_scripts': ['folint=folint.SCA:main']
     }
 )
```

