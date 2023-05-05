# Comparing `tmp/seppmail_converter-0.1.8.tar.gz` & `tmp/seppmail_converter-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seppmail_converter-0.1.8.tar", max compression
+gzip compressed data, was "seppmail_converter-0.1.9.tar", max compression
```

## Comparing `seppmail_converter-0.1.8.tar` & `seppmail_converter-0.1.9.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      939 2023-05-05 11:44:24.721586 seppmail_converter-0.1.8/README.md
--rw-r--r--   0        0        0      541 2023-05-05 11:30:27.127632 seppmail_converter-0.1.8/pyproject.toml
--rw-r--r--   0        0        0       22 2023-05-05 11:29:48.040535 seppmail_converter-0.1.8/seppmail_converter/__init__.py
--rw-r--r--   0        0        0      133 2023-04-13 20:35:22.726388 seppmail_converter-0.1.8/seppmail_converter/exceptions.py
--rw-r--r--   0        0        0     5072 2023-05-05 11:44:56.671543 seppmail_converter-0.1.8/seppmail_converter/main.py
--rw-r--r--   0        0        0     1831 1970-01-01 00:00:00.000000 seppmail_converter-0.1.8/setup.py
--rw-r--r--   0        0        0     1592 1970-01-01 00:00:00.000000 seppmail_converter-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-05-05 11:53:27.312906 seppmail_converter-0.1.9/README.md
+-rw-r--r--   0        0        0      541 2023-05-05 11:52:59.559390 seppmail_converter-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-05-05 11:52:53.240120 seppmail_converter-0.1.9/seppmail_converter/__init__.py
+-rw-r--r--   0        0        0      133 2023-04-13 20:35:22.726388 seppmail_converter-0.1.9/seppmail_converter/exceptions.py
+-rw-r--r--   0        0        0     5211 2023-05-05 11:52:30.262072 seppmail_converter-0.1.9/seppmail_converter/main.py
+-rw-r--r--   0        0        0     1954 1970-01-01 00:00:00.000000 seppmail_converter-0.1.9/setup.py
+-rw-r--r--   0        0        0     1714 1970-01-01 00:00:00.000000 seppmail_converter-0.1.9/PKG-INFO
```

### Comparing `seppmail_converter-0.1.8/README.md` & `seppmail_converter-0.1.9/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -12,18 +12,19 @@
   -p, --password TEXT
   -o, --output PATH
   -f, --force          Skip SEPPMail input file validation
   -d, --delete         Delete input file after conversion
   -o, --overwrite      Overwrite output file if it exists
   -e, --extract        Extract attachments from .eml file
   -q, --quiet          Suppress all output except final path
+  -v, --version        Show the version and exit.
   --help               Show this message and exit.
 ```
 
 Relevant environment variables:
 
-| Name | Description |
-| ---- | ----------- |
-| `SEPPMAIL_USERNAME` | Email supplied during login |
-| `SEPPMAIL_PASSWORD` | Password supplied during login|
+| Name                | Description                    |
+|---------------------|--------------------------------|
+| `SEPPMAIL_USERNAME` | Email supplied during login    |
+| `SEPPMAIL_PASSWORD` | Password supplied during login |
 
 Unless specified, the script will place the output file next to the input file and name it after the original file.
```

### Comparing `seppmail_converter-0.1.8/pyproject.toml` & `seppmail_converter-0.1.9/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "seppmail-converter"
-version = "0.1.8"
+version = "0.1.9"
 description = "Decode SEPPMail emails into EML files"
 license = "MIT"
 authors = ["Daniel Malik <daniel.malik@mhsp.solutions>"]
 readme = "README.md"
 classifiers = ["Environment :: Console"]
 
 [tool.poetry.dependencies]
```

### Comparing `seppmail_converter-0.1.8/seppmail_converter/main.py` & `seppmail_converter-0.1.9/seppmail_converter/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from email import policy
 
 import click
 import requests
 from bs4 import BeautifulSoup
 
 from seppmail_converter.exceptions import AuthenticationError, ExportError
+from seppmail_converter import __version__
 
 
 def get_valid_filename(name):
     s = str(name).strip().replace(" ", "_")
     s = re.sub(r"(?u)[^-\w.]", "", s)
     if s in {"", ".", ".."}:
         return None
@@ -71,24 +72,26 @@
 @click.option(
     "--quiet",
     "-q",
     help="Suppress all output except final path",
     type=click.BOOL,
     is_flag=True,
 )
+@click.version_option(__version__, "-v", "--version", message="%(version)s")
 def cli(
     input_file: pathlib.Path,
     output: pathlib.Path,
     username: str,
     password: str,
     force: bool,
     delete: bool,
     overwrite: bool,
     extract: bool,
     quiet: bool,
+    version: bool,
 ):
     # Extract key-value pairs from form
     if "secmail" not in input_file.read_text("utf-8") and not force:
         raise click.FileError(
             str(input_file.absolute()), "The input file provided seems to be invalid"
         )
```

### Comparing `seppmail_converter-0.1.8/setup.py` & `seppmail_converter-0.1.9/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,17 +14,17 @@
  'requests>=2.30,<3.0']
 
 entry_points = \
 {'console_scripts': ['seppmail-converter = seppmail_converter.main:entry']}
 
 setup_kwargs = {
     'name': 'seppmail-converter',
-    'version': '0.1.8',
+    'version': '0.1.9',
     'description': 'Decode SEPPMail emails into EML files',
-    'long_description': '# SEPPMail Converter\n\nThis python tool allows you to convert [SEPPMail](https://www.seppmail.com/) encrypted email files (`html`) to `.eml` files.\n\n## Usage\n\n```\nUsage: seppmail-converter [OPTIONS] INPUT_FILE\n\nOptions:\n  -u, --username TEXT\n  -p, --password TEXT\n  -o, --output PATH\n  -f, --force          Skip SEPPMail input file validation\n  -d, --delete         Delete input file after conversion\n  -o, --overwrite      Overwrite output file if it exists\n  -e, --extract        Extract attachments from .eml file\n  -q, --quiet          Suppress all output except final path\n  --help               Show this message and exit.\n```\n\nRelevant environment variables:\n\n| Name | Description |\n| ---- | ----------- |\n| `SEPPMAIL_USERNAME` | Email supplied during login |\n| `SEPPMAIL_PASSWORD` | Password supplied during login|\n\nUnless specified, the script will place the output file next to the input file and name it after the original file.\n',
+    'long_description': '# SEPPMail Converter\n\nThis python tool allows you to convert [SEPPMail](https://www.seppmail.com/) encrypted email files (`html`) to `.eml` files.\n\n## Usage\n\n```\nUsage: seppmail-converter [OPTIONS] INPUT_FILE\n\nOptions:\n  -u, --username TEXT\n  -p, --password TEXT\n  -o, --output PATH\n  -f, --force          Skip SEPPMail input file validation\n  -d, --delete         Delete input file after conversion\n  -o, --overwrite      Overwrite output file if it exists\n  -e, --extract        Extract attachments from .eml file\n  -q, --quiet          Suppress all output except final path\n  -v, --version        Show the version and exit.\n  --help               Show this message and exit.\n```\n\nRelevant environment variables:\n\n| Name                | Description                    |\n|---------------------|--------------------------------|\n| `SEPPMAIL_USERNAME` | Email supplied during login    |\n| `SEPPMAIL_PASSWORD` | Password supplied during login |\n\nUnless specified, the script will place the output file next to the input file and name it after the original file.\n',
     'author': 'Daniel Malik',
     'author_email': 'daniel.malik@mhsp.solutions',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `seppmail_converter-0.1.8/PKG-INFO` & `seppmail_converter-0.1.9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seppmail-converter
-Version: 0.1.8
+Version: 0.1.9
 Summary: Decode SEPPMail emails into EML files
 License: MIT
 Author: Daniel Malik
 Author-email: daniel.malik@mhsp.solutions
 Requires-Python: >=3.10,<4.0
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
@@ -31,19 +31,20 @@
   -p, --password TEXT
   -o, --output PATH
   -f, --force          Skip SEPPMail input file validation
   -d, --delete         Delete input file after conversion
   -o, --overwrite      Overwrite output file if it exists
   -e, --extract        Extract attachments from .eml file
   -q, --quiet          Suppress all output except final path
+  -v, --version        Show the version and exit.
   --help               Show this message and exit.
 ```
 
 Relevant environment variables:
 
-| Name | Description |
-| ---- | ----------- |
-| `SEPPMAIL_USERNAME` | Email supplied during login |
-| `SEPPMAIL_PASSWORD` | Password supplied during login|
+| Name                | Description                    |
+|---------------------|--------------------------------|
+| `SEPPMAIL_USERNAME` | Email supplied during login    |
+| `SEPPMAIL_PASSWORD` | Password supplied during login |
 
 Unless specified, the script will place the output file next to the input file and name it after the original file.
```

