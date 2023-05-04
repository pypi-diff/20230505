# Comparing `tmp/divfusion-0.1.0a0.tar.gz` & `tmp/divfusion-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "divfusion-0.1.0a0.tar", last modified: Sun Apr 30 21:19:04 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `divfusion-0.1.0a0.tar` & `divfusion-0.3.4.tar`

### file list

```diff
@@ -1,29 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 21:19:04.326147 divfusion-0.1.0a0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 21:19:04.322147 divfusion-0.1.0a0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 21:19:04.326147 divfusion-0.1.0a0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-04-30 21:18:46.000000 divfusion-0.1.0a0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-30 21:18:46.000000 divfusion-0.1.0a0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     9648 2023-04-30 21:18:46.000000 divfusion-0.1.0a0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     3170 2023-04-30 21:19:04.326147 divfusion-0.1.0a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-04-30 21:18:46.000000 divfusion-0.1.0a0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-30 21:18:46.000000 divfusion-0.1.0a0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 21:19:04.326147 divfusion-0.1.0a0/resources_test/
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-04-30 21:18:46.000000 divfusion-0.1.0a0/resources_test/COMPLEX_TEST.html
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-30 21:18:46.000000 divfusion-0.1.0a0/resources_test/MINIMAL_TEST.html
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-04-30 21:18:46.000000 divfusion-0.1.0a0/resources_test/MULTIROW_TEST.html
--rw-r--r--   0 runner    (1001) docker     (123)     8366 2023-04-30 21:18:46.000000 divfusion-0.1.0a0/resources_test/PLOTLY_TEST.html
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-04-30 21:19:04.326147 divfusion-0.1.0a0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 21:19:04.322147 divfusion-0.1.0a0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 21:19:04.326147 divfusion-0.1.0a0/src/divfusion/
--rw-r--r--   0 runner    (1001) docker     (123)     5504 2023-04-30 21:18:46.000000 divfusion-0.1.0a0/src/divfusion/Report.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-04-30 21:18:46.000000 divfusion-0.1.0a0/src/divfusion/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 21:19:04.326147 divfusion-0.1.0a0/src/divfusion.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3170 2023-04-30 21:19:04.000000 divfusion-0.1.0a0/src/divfusion.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-04-30 21:19:04.000000 divfusion-0.1.0a0/src/divfusion.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 21:19:04.000000 divfusion-0.1.0a0/src/divfusion.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 21:19:04.000000 divfusion-0.1.0a0/src/divfusion.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-30 21:19:04.000000 divfusion-0.1.0a0/src/divfusion.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-30 21:19:04.000000 divfusion-0.1.0a0/src/divfusion.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 21:19:04.326147 divfusion-0.1.0a0/test/
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-04-30 21:18:46.000000 divfusion-0.1.0a0/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4897 2023-04-30 21:18:46.000000 divfusion-0.1.0a0/test/test_Report.py
+-rw-r--r--   0        0        0     2921 2020-02-02 00:00:00.000000 divfusion-0.3.4/.github/workflows/divfusion_pr_main.yml
+-rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 divfusion-0.3.4/.github/workflows/divfusion_publish_main.yml
+-rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 divfusion-0.3.4/resources_test/COMPLEX_TEST.html
+-rw-r--r--   0        0        0     9550 2020-02-02 00:00:00.000000 divfusion-0.3.4/resources_test/DIFFERENT_TYPES_TEST.html
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 divfusion-0.3.4/resources_test/MINIMAL_TEST.html
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 divfusion-0.3.4/resources_test/MULTIROW_TEST.html
+-rw-r--r--   0        0        0     8366 2020-02-02 00:00:00.000000 divfusion-0.3.4/resources_test/PLOTLY_TEST.html
+-rw-r--r--   0        0        0     8183 2020-02-02 00:00:00.000000 divfusion-0.3.4/src/divfusion/Report.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 divfusion-0.3.4/src/divfusion/__about__.py
+-rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 divfusion-0.3.4/src/divfusion/__init__.py
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 divfusion-0.3.4/test/__init__.py
+-rw-r--r--   0        0        0     5286 2020-02-02 00:00:00.000000 divfusion-0.3.4/test/test_Report.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 divfusion-0.3.4/.gitignore
+-rw-r--r--   0        0        0     9648 2020-02-02 00:00:00.000000 divfusion-0.3.4/LICENSE.md
+-rw-r--r--   0        0        0     2728 2020-02-02 00:00:00.000000 divfusion-0.3.4/README.md
+-rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 divfusion-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0    15400 2020-02-02 00:00:00.000000 divfusion-0.3.4/PKG-INFO
```

### Comparing `divfusion-0.1.0a0/LICENSE.md` & `divfusion-0.3.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `divfusion-0.1.0a0/PKG-INFO` & `divfusion-0.3.4/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,18 @@
-Metadata-Version: 2.1
-Name: divfusion
-Version: 0.1.0a0
-Summary: divfusion takes multiple html elements and generates a stand-alone HTML-Report while managing styling and layout.
-Home-page: https://github.com/p-koenig/divfusion.git
-Author: Paul Koenig
-Author-email: 45401982+p-koenig@users.noreply.github.com
-License: Apache License 2.0
-Keywords: html,static,export
-Requires-Python: <4,>=3.10
-Description-Content-Type: text/markdown
-Provides-Extra: test
-Provides-Extra: setup
-License-File: LICENSE.md
-
 # divfusion
 
-`divfusion` is a Python class that generates an HTML-Report from a set of HTML divs. In practise, these divs would
-originate from other Python modules, especially those that generate plots (e.g. `matplotlib`, `seaborn`, `plotly`).
+`divfusion` takes multiple HTML elements and generates a stand-alone HTML-Report while managing styling and layout.
+In practise, these elements ('divs') would originate from other Python modules, especially those that generate plots
+and provide a html export (e.g. `plotly`).
 
 If used with plotly, this closes between a single-figure plotly export and a full-fledged plotly-dash server, which
 needs to be hosted somewhere. Using this Library, all interactivity of plotly is preserved (hovering, zooming, buttons,
 dropdowns, etc.). In addition to that, you can add html-exports of your pd.DataFrames, images or any other HTML content.
 `divfusion` brings all of this together and manges the layout and style of the report for you (bring your own css is
-possible).
+possible in a future version).
 
 The resulting html file is completely self-contained and can be opened in any browser on any device.
 
 ## Installation
 
 You can install `divfusion` via pip:
 
@@ -41,56 +27,49 @@
 ```python
 from divfusion import Report
 ```
 
 Next, create a new instance of `Report` by passing the following parameters:
 
 * `title` - The title of the report (string)
-* `divs` - A list of HTML divs, can be nested (list)
+* `div_like` - A list of div_like elements. Can be
+    * strings
+    * plotly figures
+    * pandas dataframes
+    * pandas series
+    * All nested combinations of the above (first dimension is columns, second dimension is rows)
 * `css_files` (optional) - The CSS files to include (list)
 * `js_files` (optional) - The JS files to include (list)
 * `js_libs` (optional) - A list of JS libraries to include (list)
 
 ```python
 report = Report(title="My Report",
-                divs=[["<h1>Heading 1</h1>", "<p>Paragraph 1</p>"], ["<h2>Heading 2</h2>", "<p>Paragraph 2</p>"]])
+                div_like=[[px.scatter(x=[1, 2, 3], y=[1, 2, 3]), "<div>some text</div>"],
+                          ["<div>Some Info Text</div>", "<div>HTML Table</div>"],
+                          [pd.DataFrame([[1, 2, 3], [4, 5, 6]]), pd.Series([1, 2, 3])]
+                          ])
 ```
+The Elements will be placed as the nested list of divs suggests: Columns horizontally, Rows vertically.
+Optionally you can add custom css files, js files or js script tags.
 
 To generate the HTML report, call the `write` method and pass the file path where you want to save the report:
 
 ```python
 report.write("path/to/report.html")
 ```
 
-## Example
-
-Here's an example of how to use `divfusion.Report`:
-
-```python
-from divfusion import Report
-
-report = Report(title="My Report",
-                divs=[["<h1>Heading 1</h1>", "<p>Paragraph 1</p>"],
-                      ["<h2>Heading 2</h2>", "<p>Paragraph 2</p>"]])
-report.write("path/to/report.html")
-```
-
-This will generate an HTML report with the title "My Report" and two rows of HTML divs. The first row contains a heading
-and a paragraph, and the second row contains a subheading and another paragraph. The report will be saved to the file
-path specified.
-
 ## Dependencies
 
-Currently `divfusion` does not require any dependencies.
+Currently `divfusion` requires pandas>=1.4.0 and plotly>=5.0.0. Python >= 3.10 is required.
 
 ## Future Work
 
 - Add support for custom css
 - Provide easy-to-use wrapper functions for adding plotly-figures, pandas-dataframes, etc.
 
 ## Contribution
 
-I welcome any and all contributions, no matter what size. Please feel free to open an issue or pull request.
+I welcome any and all contributions, no matter what size. Please feel free to open an issue or pull request against dev.
 
 ## License
 
 Apache License 2.0
```

### Comparing `divfusion-0.1.0a0/resources_test/COMPLEX_TEST.html` & `divfusion-0.3.4/resources_test/COMPLEX_TEST.html`

 * *Files identical despite different names*

### Comparing `divfusion-0.1.0a0/resources_test/MINIMAL_TEST.html` & `divfusion-0.3.4/resources_test/MINIMAL_TEST.html`

 * *Files identical despite different names*

### Comparing `divfusion-0.1.0a0/resources_test/MULTIROW_TEST.html` & `divfusion-0.3.4/resources_test/MULTIROW_TEST.html`

 * *Files identical despite different names*

### Comparing `divfusion-0.1.0a0/resources_test/PLOTLY_TEST.html` & `divfusion-0.3.4/resources_test/PLOTLY_TEST.html`

 * *Files identical despite different names*

### Comparing `divfusion-0.1.0a0/src/divfusion/__init__.py` & `divfusion-0.3.4/test/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,17 +7,8 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
-#  ==============================================================================
-
-from pkg_resources import get_distribution, DistributionNotFound
-
-from .Report import Report
-
-try:
-    __version__ = get_distribution(__name__).version
-except DistributionNotFound:
-    raise DistributionNotFound("Could not find the package version. Did you install it?")
+#  ==============================================================================
```

### Comparing `divfusion-0.1.0a0/test/__init__.py` & `divfusion-0.3.4/src/divfusion/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,8 +7,10 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
-#  ==============================================================================
+#  ==============================================================================
+
+from .Report import Report
```

### Comparing `divfusion-0.1.0a0/test/test_Report.py` & `divfusion-0.3.4/test/test_Report.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,25 +8,25 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #  ==============================================================================
-
 import re
 
+import pandas as pd
 import plotly.express as px
 import pytest
 from pyfakefs.fake_filesystem_unittest import Patcher
 
 from divfusion import Report
 
 
-@pytest.fixture(params=["MINIMAL_TEST", "PLOTLY_TEST", "MULTIROW_TEST", "COMPLEX_TEST"])
+@pytest.fixture(params=["MINIMAL_TEST", "PLOTLY_TEST", "MULTIROW_TEST", "COMPLEX_TEST", "DIFFERENT_TYPES_TEST"])
 def report_type(request):
     return request.param
 
 
 @pytest.fixture
 def report(report_type):
     """
@@ -69,14 +69,21 @@
                          ["<div>Row 3, Third Width left</div>",
                           "<div>Row 3, Third Width middle</div>",
                           "<div>Row 3, Third Width right</div>"]
                      ]
                      ]
                     ]
             report = Report(title, divs)
+        case "DIFFERENT_TYPES_TEST":
+            divs = ["This is a test String",
+                    px.scatter(x=[1, 2, 3], y=[1, 2, 3]),
+                    "<div>Test Content</div>",
+                    pd.DataFrame({"A": [1, 2, 3], "B": [4, 5, 6]}),
+                    pd.Series([1, 2, 3, 4, 5, 6])]
+            report = Report(title, divs)
         case _:
             raise ValueError(f"Unknown test case: {report_type}")
 
     return report
 
 
 @pytest.fixture
@@ -91,15 +98,15 @@
     Returns
     -------
     out : str
         expected HTML string
 
     """
     try:
-        with open(f"../resources_test/{report_type}.html") as f:
+        with open(f"./resources_test/{report_type}.html") as f:
             return f.read()
     except FileNotFoundError:
         raise ValueError(f"Could not find expected HTML file for test case: {report_type}")
 
 
 def compare_html(html1, html2):
     """
```

