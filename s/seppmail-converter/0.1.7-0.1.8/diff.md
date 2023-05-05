# Comparing `tmp/seppmail_converter-0.1.7.tar.gz` & `tmp/seppmail_converter-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seppmail_converter-0.1.7.tar", max compression
+gzip compressed data, was "seppmail_converter-0.1.8.tar", max compression
```

## Comparing `seppmail_converter-0.1.7.tar` & `seppmail_converter-0.1.8.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      883 2023-04-13 20:56:58.210024 seppmail_converter-0.1.7/README.md
--rw-r--r--   0        0        0      543 2023-04-13 20:55:01.641998 seppmail_converter-0.1.7/pyproject.toml
--rw-r--r--   0        0        0       22 2023-04-13 20:55:01.643417 seppmail_converter-0.1.7/seppmail_converter/__init__.py
--rw-r--r--   0        0        0      133 2023-04-13 20:35:22.726388 seppmail_converter-0.1.7/seppmail_converter/exceptions.py
--rw-r--r--   0        0        0     4113 2023-04-13 20:56:23.716858 seppmail_converter-0.1.7/seppmail_converter/main.py
--rw-r--r--   0        0        0     1778 1970-01-01 00:00:00.000000 seppmail_converter-0.1.7/setup.py
--rw-r--r--   0        0        0     1540 1970-01-01 00:00:00.000000 seppmail_converter-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0      939 2023-05-05 11:44:24.721586 seppmail_converter-0.1.8/README.md
+-rw-r--r--   0        0        0      541 2023-05-05 11:30:27.127632 seppmail_converter-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-05-05 11:29:48.040535 seppmail_converter-0.1.8/seppmail_converter/__init__.py
+-rw-r--r--   0        0        0      133 2023-04-13 20:35:22.726388 seppmail_converter-0.1.8/seppmail_converter/exceptions.py
+-rw-r--r--   0        0        0     5072 2023-05-05 11:44:56.671543 seppmail_converter-0.1.8/seppmail_converter/main.py
+-rw-r--r--   0        0        0     1831 1970-01-01 00:00:00.000000 seppmail_converter-0.1.8/setup.py
+-rw-r--r--   0        0        0     1592 1970-01-01 00:00:00.000000 seppmail_converter-0.1.8/PKG-INFO
```

### Comparing `seppmail_converter-0.1.7/README.md` & `seppmail_converter-0.1.8/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -10,17 +10,18 @@
 Options:
   -u, --username TEXT
   -p, --password TEXT
   -o, --output PATH
   -f, --force          Skip SEPPMail input file validation
   -d, --delete         Delete input file after conversion
   -o, --overwrite      Overwrite output file if it exists
+  -e, --extract        Extract attachments from .eml file
   -q, --quiet          Suppress all output except final path
-  --help               Show this message and exit. 
- ```
+  --help               Show this message and exit.
+```
 
 Relevant environment variables:
 
 | Name | Description |
 | ---- | ----------- |
 | `SEPPMAIL_USERNAME` | Email supplied during login |
 | `SEPPMAIL_PASSWORD` | Password supplied during login|
```

### Comparing `seppmail_converter-0.1.7/seppmail_converter/main.py` & `seppmail_converter-0.1.8/seppmail_converter/main.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,9 +1,11 @@
+import email
 import pathlib
 import re
+from email import policy
 
 import click
 import requests
 from bs4 import BeautifulSoup
 
 from seppmail_converter.exceptions import AuthenticationError, ExportError
 
@@ -55,28 +57,37 @@
     "--overwrite",
     "-o",
     help="Overwrite output file if it exists",
     type=click.BOOL,
     is_flag=True,
 )
 @click.option(
+    "--extract",
+    "-e",
+    help="Extract attachments from .eml file",
+    type=click.BOOL,
+    is_flag=True,
+    default=False,
+)
+@click.option(
     "--quiet",
     "-q",
     help="Suppress all output except final path",
     type=click.BOOL,
     is_flag=True,
 )
 def cli(
     input_file: pathlib.Path,
     output: pathlib.Path,
     username: str,
     password: str,
     force: bool,
     delete: bool,
     overwrite: bool,
+    extract: bool,
     quiet: bool,
 ):
     # Extract key-value pairs from form
     if "secmail" not in input_file.read_text("utf-8") and not force:
         raise click.FileError(
             str(input_file.absolute()), "The input file provided seems to be invalid"
         )
@@ -142,22 +153,40 @@
         if output.exists() and overwrite:
             output.unlink()
 
     output.write_bytes(req.content)
 
     if delete:
         input_file.unlink()
-
     if quiet:
         click.echo(output.absolute())
     else:
         click.echo(
             f"Decoded {click.format_filename(input_file.absolute())} to {click.format_filename(output.absolute())}"
         )
 
+    if extract:
+        msg = email.message_from_bytes(output.read_bytes(), policy=policy.default)
+        msg.get_payload()
+        for attachment in msg.iter_attachments():
+            try:
+                attachment_filename = attachment.get_filename()
+            except AttributeError:
+                continue
+            if not attachment_filename:
+                continue
+            attachment_output = pathlib.Path(
+                pathlib.Path.joinpath(output.parent, attachment_filename)
+            )
+            attachment_output.write_bytes(attachment.get_payload(decode=True))
+            if not quiet:
+                click.echo(
+                    f"Extracted {click.format_filename(attachment_output.absolute())}"
+                )
+
 
 def entry():
     cli(auto_envvar_prefix="SEPPMAIL")
 
 
 if __name__ == "__main__":
     entry()
```

### Comparing `seppmail_converter-0.1.7/setup.py` & `seppmail_converter-0.1.8/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,27 +4,27 @@
 packages = \
 ['seppmail_converter']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['beautifulsoup4>=4.11.1,<5.0.0',
+['beautifulsoup4>=4.12.2,<5.0.0',
  'click>=8.1.3,<9.0.0',
- 'lxml>=4.9.1,<5.0.0',
- 'requests>=2.28.1,<3.0.0']
+ 'lxml>=4.9.2,<5.0.0',
+ 'requests>=2.30,<3.0']
 
 entry_points = \
 {'console_scripts': ['seppmail-converter = seppmail_converter.main:entry']}
 
 setup_kwargs = {
     'name': 'seppmail-converter',
-    'version': '0.1.7',
+    'version': '0.1.8',
     'description': 'Decode SEPPMail emails into EML files',
-    'long_description': '# SEPPMail Converter\n\nThis python tool allows you to convert [SEPPMail](https://www.seppmail.com/) encrypted email files (`html`) to `.eml` files.\n\n## Usage\n\n```\nUsage: seppmail-converter [OPTIONS] INPUT_FILE\n\nOptions:\n  -u, --username TEXT\n  -p, --password TEXT\n  -o, --output PATH\n  -f, --force          Skip SEPPMail input file validation\n  -d, --delete         Delete input file after conversion\n  -o, --overwrite      Overwrite output file if it exists\n  -q, --quiet          Suppress all output except final path\n  --help               Show this message and exit. \n ```\n\nRelevant environment variables:\n\n| Name | Description |\n| ---- | ----------- |\n| `SEPPMAIL_USERNAME` | Email supplied during login |\n| `SEPPMAIL_PASSWORD` | Password supplied during login|\n\nUnless specified, the script will place the output file next to the input file and name it after the original file.\n',
+    'long_description': '# SEPPMail Converter\n\nThis python tool allows you to convert [SEPPMail](https://www.seppmail.com/) encrypted email files (`html`) to `.eml` files.\n\n## Usage\n\n```\nUsage: seppmail-converter [OPTIONS] INPUT_FILE\n\nOptions:\n  -u, --username TEXT\n  -p, --password TEXT\n  -o, --output PATH\n  -f, --force          Skip SEPPMail input file validation\n  -d, --delete         Delete input file after conversion\n  -o, --overwrite      Overwrite output file if it exists\n  -e, --extract        Extract attachments from .eml file\n  -q, --quiet          Suppress all output except final path\n  --help               Show this message and exit.\n```\n\nRelevant environment variables:\n\n| Name | Description |\n| ---- | ----------- |\n| `SEPPMAIL_USERNAME` | Email supplied during login |\n| `SEPPMAIL_PASSWORD` | Password supplied during login|\n\nUnless specified, the script will place the output file next to the input file and name it after the original file.\n',
     'author': 'Daniel Malik',
     'author_email': 'daniel.malik@mhsp.solutions',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `seppmail_converter-0.1.7/PKG-INFO` & `seppmail_converter-0.1.8/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: seppmail-converter
-Version: 0.1.7
+Version: 0.1.8
 Summary: Decode SEPPMail emails into EML files
 License: MIT
 Author: Daniel Malik
 Author-email: daniel.malik@mhsp.solutions
 Requires-Python: >=3.10,<4.0
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: beautifulsoup4 (>=4.11.1,<5.0.0)
+Requires-Dist: beautifulsoup4 (>=4.12.2,<5.0.0)
 Requires-Dist: click (>=8.1.3,<9.0.0)
-Requires-Dist: lxml (>=4.9.1,<5.0.0)
-Requires-Dist: requests (>=2.28.1,<3.0.0)
+Requires-Dist: lxml (>=4.9.2,<5.0.0)
+Requires-Dist: requests (>=2.30,<3.0)
 Description-Content-Type: text/markdown
 
 # SEPPMail Converter
 
 This python tool allows you to convert [SEPPMail](https://www.seppmail.com/) encrypted email files (`html`) to `.eml` files.
 
 ## Usage
@@ -29,17 +29,18 @@
 Options:
   -u, --username TEXT
   -p, --password TEXT
   -o, --output PATH
   -f, --force          Skip SEPPMail input file validation
   -d, --delete         Delete input file after conversion
   -o, --overwrite      Overwrite output file if it exists
+  -e, --extract        Extract attachments from .eml file
   -q, --quiet          Suppress all output except final path
-  --help               Show this message and exit. 
- ```
+  --help               Show this message and exit.
+```
 
 Relevant environment variables:
 
 | Name | Description |
 | ---- | ----------- |
 | `SEPPMAIL_USERNAME` | Email supplied during login |
 | `SEPPMAIL_PASSWORD` | Password supplied during login|
```

