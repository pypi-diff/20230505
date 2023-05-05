# Comparing `tmp/asc2mb-0.6.2.tar.gz` & `tmp/asc2mb-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asc2mb-0.6.2.tar", max compression
+gzip compressed data, was "asc2mb-0.7.0.tar", max compression
```

## Comparing `asc2mb-0.6.2.tar` & `asc2mb-0.7.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     2327 2021-12-20 03:30:53.502175 asc2mb-0.6.2/README.md
--rw-r--r--   0        0        0        0 2021-12-08 10:10:14.401686 asc2mb-0.6.2/asc2mb/__init__.py
--rw-r--r--   0        0        0    15150 2022-07-18 14:23:02.921145 asc2mb-0.6.2/asc2mb/asc2mb.py
--rw-r--r--   0        0        0      567 2022-07-19 06:57:35.181868 asc2mb-0.6.2/pyproject.toml
--rw-r--r--   0        0        0     3208 2022-07-19 06:57:40.680069 asc2mb-0.6.2/setup.py
--rw-r--r--   0        0        0     3095 2022-07-19 06:57:40.680223 asc2mb-0.6.2/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-01-04 05:44:08.623819 asc2mb-0.7.0/LICENSE
+-rw-r--r--   0        0        0     2327 2021-12-20 03:30:53.502175 asc2mb-0.7.0/README.md
+-rw-r--r--   0        0        0        0 2021-12-08 10:10:14.401686 asc2mb-0.7.0/asc2mb/__init__.py
+-rw-r--r--   0        0        0    16196 2023-05-05 03:38:11.938609 asc2mb-0.7.0/asc2mb/asc2mb.py
+-rw-r--r--   0        0        0      606 2023-05-05 03:44:02.698247 asc2mb-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     3178 1970-01-01 00:00:00.000000 asc2mb-0.7.0/PKG-INFO
```

### Comparing `asc2mb-0.6.2/README.md` & `asc2mb-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `asc2mb-0.6.2/asc2mb/asc2mb.py` & `asc2mb-0.7.0/asc2mb/asc2mb.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,17 @@
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 ˇ
 """
 
 import re
-import click
+from rich.console import Console
+console = Console()
+import rich_click as click
 import csv
 from lxml import etree
 
 from collections import UserDict, defaultdict
 
 
 class Json(UserDict):
@@ -68,15 +70,16 @@
         teacher = self
         pattern = "f'" + (self.default or '') + "'"
         return eval(pattern)
 
 # eval used 
 class_id_patterns = [
     {"p": "{class_.short}_{division.name}", "n":'default'},
-    {"p":"{class_.short} {division.divisiontag if division.divisiontag!='0' else ''}{subject.short}", "n": "dar_al_marefa"}
+    {"p":"{class_.short} {division.divisiontag if division.divisiontag!='0' else ''}{subject.short}", "n": "dar_al_marefa"},
+    {'p': '{class_.name}', 'n':'name_only'}
 ]
 pattern_choices = [pattern.get('n') for pattern in class_id_patterns]
 
 section_patterns = [
     {"p": "{int(division.divisiontag)+1}", "n": "default"},
 #    {"p": "{teacher.name.split(' ')[0][0] + teacher.name.split(' ')[1][0] if len(teacher.name.split(' '))>1 else ''}", "n": 'teacher_intiails'},
     {"p": "{class_.short if division.divisiontag == '0' else f'{class_.short}({division.divisiontag})'}", 'n': 'dar_al_marefa'}
@@ -215,33 +218,39 @@
             if smart_combine and len(teachers) == 1 and largest > 1:
                 combine = True
 
             uniqs = []
             for index in range(largest):
                 group_id = groups[index]
                 class_id = classes[index]
+                if not classes[index] and len(classes) == 1:
+                    console.print(r"[yellow]Warning:[/] Lesson definition with multiple divisions but only one class. Using the first class as the default", f'{lesson=}')
+                    class_id = classes[0]
 
                 division = Json(lookup.get('groups').get(group_id)) if group_id is not None else Json()
                 class_ = Json(lookup.get('classes').get(class_id)) if class_id is not None else Json()
 
+                if not class_:
+                    console.print(f'[yellow]Warning: [/] No class information available that cooresponds to division. Number of divisions: {len(groups)}, number of classes: {len(classes)}', f'{lesson=}')
+
                 pattern = get_pattern(class_id_patterns, class_id_pattern)
                 uniq = eval(pattern)
                 uniqs.append(uniq)
 
                 # all of the card placements
                 cards = lookup.get('cards').get(lesson_id)
                 staging[uniq] = cards
 
                 section = eval(get_pattern(section_patterns, section_pattern))
-                match = re.match(r'^[\d]+', class_.short)
-                if match is None:
-                    print(f"Warning: Grade {class_.short} given for {uniq}? Using 0 instead", class_)
-                    year = 0
-                else:
-                    year = match.group()
+
+                ## Get the year which we'll put in the classes output
+                year = ''.join(filter(str.isdigit, class_.short))
+                if not year:
+                    console.print(f"[yellow]Warning[/yellow]: Expecting digits in 'short' as the Grade `class_.sort`. Using itself instead, or '<>' if none provided", f'{class_=}')
+                    year = class_.short or '<>'
 
                 if cards is None:
                     continue
                 process_info['num_cards'] += len(cards)
                 for card in cards:
                     classrooms = map(lambda x: lookup.get('classrooms').get(x), card.get('classroomids').split(','))
                     if card.get('day'):
@@ -258,20 +267,25 @@
                                 matrix = []
                                 for row in range(len(uniqs)):
                                     matrix.append([ s for s in uniqs[row] ])
                                 combined_uniq = []
                                 for col in range(max([len(m) for m in matrix])):
                                     cells = []
                                     for row in range(len(matrix)):
-                                        cells.append(matrix[row][col])
+                                        try: 
+                                            cells.append(matrix[row][col])
+                                        except IndexError:
+                                            cells.append('')
                                     if len(set([c for c in cells])) == 1:
                                         # they are all the same
                                         combined_uniq.append(matrix[0][col])
                                     else:
                                         combined_uniq.append(''.join(sorted(set(cells))))
+
+                                # get the uniq:
                                 uniq = ''.join(combined_uniq)
                                 if combine_uniq_post:
                                     # special request 
                                     f, s = uniq.split(' ')
                                     g = re.match(r'(\d+\w+?)(\d+)', f)
                                     h = re.match(r'(\d+)(.*)', s)
                                     i = min(h.groups()[0])
@@ -281,19 +295,19 @@
                                 classes_file.append([uniq, f"Grade {year}", division.name, subject.short, '', teacher_emails, section])
 
                         else:
                             timetable_output.append([uniq, day, period, classroom_output])
                             classes_file.append([uniq, f"Grade {year}", division.name, subject.short, '', teacher_emails, section])
 
     elif grouptype == 2:
-        print('grouptype == 2 not implemented yet')
+        console.print('[red bold]Critical error[/]: grouptype == 2 not implemented yet')
         exit(0)
 
     else:
-        print("uknown group type")
+        console.print("[red bold]Critical error[/] uknown group type")
         exit(0)
 
     # remove dups
     classes_file = sorted(list(dict.fromkeys([tuple(i) for i in classes_file])))
     timetable_output = sorted(timetable_output)
     with open(timetable_csv, 'w', newline='') as csvfile:
         writer = csv.writer(csvfile)
@@ -303,11 +317,11 @@
 
     with open(classes_csv, 'w', newline='') as csvfile:
         writer = csv.writer(csvfile)
         writer.writerow(['Class ID', 'Year', 'Group', 'Subject', 'Name', 'Teacher Email', 'Section'])
         for row in classes_file:
             writer.writerow(row)
 
-    print('\nProcess completed.')
-    print(f"Lessons processed: {process_info['num_lessons']}\nCards processed: {process_info['num_cards']}")
+    console.print('\n[green]Process completed.')
+    console.print(f"Lessons processed: {process_info['num_lessons']}\nCards processed: {process_info['num_cards']}")
```

### Comparing `asc2mb-0.6.2/pyproject.toml` & `asc2mb-0.7.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 [tool.poetry]
 name = "asc2mb"
-version = "0.6.2"
+version = "0.7.0"
 description = "Manage your timetable by pasing the XML export from asc and format into two files suitable for upload into ManageBac"
 authors = ["Adam Morris <adam.morris@fariaedu.com>"]
 license = "MIT"
 readme = "README.md"
 keywords = ["ManageBac", "aSc", "timetable"]
 
 [tool.poetry.dependencies]
-python = "^3.6"
+python = "^3.7"
 click = "8.0"
 lxml = "^4.9.1"
+rich-click = "^1.6.1"
+rich = "^13.3.5"
 
 [tool.poetry.dev-dependencies]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `asc2mb-0.6.2/setup.py` & `asc2mb-0.7.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,34 +1,83 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: asc2mb
+Version: 0.7.0
+Summary: Manage your timetable by pasing the XML export from asc and format into two files suitable for upload into ManageBac
+License: MIT
+Keywords: ManageBac,aSc,timetable
+Author: Adam Morris
+Author-email: adam.morris@fariaedu.com
+Requires-Python: >=3.7,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: click (==8.0)
+Requires-Dist: lxml (>=4.9.1,<5.0.0)
+Requires-Dist: rich (>=13.3.5,<14.0.0)
+Requires-Dist: rich-click (>=1.6.1,<2.0.0)
+Description-Content-Type: text/markdown
+
+# aSc to ManageBac
+
+## Getting started
+
+Requires Python 3.6 or above. For Windows, install Python via the Microsoft Store. For Mac, install Python at [python.org](https://www.python.org). Installing Python also installs a package manager (called `pip`) that can install the command `asc2mb` into your command line environment.
+
+After installing Python, open the terminal or command line or PowerShell, and peform the following:
+
+```sh
+pip install asc2mb
+```
+
+If for some reason the `pip` command doesn't work, you can manually install it by following [the relevant instructions](https://pip.pypa.io/en/stable/installing/) for your system.
+
+### Upgrade
+
+Should you need to update to the latest version, you can do:
+
+```
+pip install --upgrade asc2mb
+```
+
+## Use
+
+After `pip install` worked, it is now installed on your path, and the command `asc2mb` should be available:
+
+```
+asc2mb ~/path/to/xml.xml ~/path/to/save/timetable.csv ~/path/to/save/classes.csv
+```
+
+It takes only a second to run. It reports how many records it processed.
+
+## Algorithm
+
+This script uses input from more than one international school to generate the expected output. The key to success is using aSc Divisions to match the `uniq_id`s found in ManageBac classes.
+
+## Help
+
+For built-in help, and list of options and their functionality:
+
+```
+asc2mb --help
+```
+
+## Miscellaneous
+
+The command takes three required arguments, and there are additional options as well. The three required arguments tell the program where the xml file is located, and where to save the two csv files. 
+
+The options depend on your school's needs. For example, the class id is how ManageBac knows which class you are referring to, so that program helps you derive the class ID based on information contains in the xml file. It's up to you to ensure there are classes that have those IDs in ManageBac, but the program does produce a csv so that they can be uploaded in bulk.
+
+By default, class id uses the pattern `{class_.short}_{division.name}`, which means "the short name of the class" plus an underscore, plus the name of the division." At the time of publication, having a different pattern is only possible by contacting the author (or, if you're a keen developer, add a pull request).
+
+If you run the program without any options, it'll prompt you to enter them.
+
+
+
 
-packages = \
-['asc2mb']
 
-package_data = \
-{'': ['*']}
 
-install_requires = \
-['click==8.0', 'lxml>=4.9.1,<5.0.0']
-
-entry_points = \
-{'console_scripts': ['asc2mb = asc2mb.asc2mb:main']}
-
-setup_kwargs = {
-    'name': 'asc2mb',
-    'version': '0.6.2',
-    'description': 'Manage your timetable by pasing the XML export from asc and format into two files suitable for upload into ManageBac',
-    'long_description': '# aSc to ManageBac\n\n## Getting started\n\nRequires Python 3.6 or above. For Windows, install Python via the Microsoft Store. For Mac, install Python at [python.org](https://www.python.org). Installing Python also installs a package manager (called `pip`) that can install the command `asc2mb` into your command line environment.\n\nAfter installing Python, open the terminal or command line or PowerShell, and peform the following:\n\n```sh\npip install asc2mb\n```\n\nIf for some reason the `pip` command doesn\'t work, you can manually install it by following [the relevant instructions](https://pip.pypa.io/en/stable/installing/) for your system.\n\n### Upgrade\n\nShould you need to update to the latest version, you can do:\n\n```\npip install --upgrade asc2mb\n```\n\n## Use\n\nAfter `pip install` worked, it is now installed on your path, and the command `asc2mb` should be available:\n\n```\nasc2mb ~/path/to/xml.xml ~/path/to/save/timetable.csv ~/path/to/save/classes.csv\n```\n\nIt takes only a second to run. It reports how many records it processed.\n\n## Algorithm\n\nThis script uses input from more than one international school to generate the expected output. The key to success is using aSc Divisions to match the `uniq_id`s found in ManageBac classes.\n\n## Help\n\nFor built-in help, and list of options and their functionality:\n\n```\nasc2mb --help\n```\n\n## Miscellaneous\n\nThe command takes three required arguments, and there are additional options as well. The three required arguments tell the program where the xml file is located, and where to save the two csv files. \n\nThe options depend on your school\'s needs. For example, the class id is how ManageBac knows which class you are referring to, so that program helps you derive the class ID based on information contains in the xml file. It\'s up to you to ensure there are classes that have those IDs in ManageBac, but the program does produce a csv so that they can be uploaded in bulk.\n\nBy default, class id uses the pattern `{class_.short}_{division.name}`, which means "the short name of the class" plus an underscore, plus the name of the division." At the time of publication, having a different pattern is only possible by contacting the author (or, if you\'re a keen developer, add a pull request).\n\nIf you run the program without any options, it\'ll prompt you to enter them.\n\n\n\n\n\n\n\n',
-    'author': 'Adam Morris',
-    'author_email': 'adam.morris@fariaedu.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': None,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.6,<4.0',
-}
 
 
-setup(**setup_kwargs)
```

