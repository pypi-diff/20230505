# Comparing `tmp/valaw-0.0.5.tar.gz` & `tmp/valaw-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "valaw-0.0.5.tar", last modified: Thu Apr 20 20:05:12 2023, max compression
+gzip compressed data, was "valaw-0.0.6.tar", last modified: Fri May  5 01:52:33 2023, max compression
```

## Comparing `valaw-0.0.5.tar` & `valaw-0.0.6.tar`

### file list

```diff
@@ -1,16 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-04-20 20:05:12.618703 valaw-0.0.5/
--rw-rw-rw-   0        0        0     1090 2023-04-04 04:45:45.000000 valaw-0.0.5/LICENSE
--rw-rw-rw-   0        0        0     2306 2023-04-20 20:05:12.610672 valaw-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     1623 2023-04-20 18:57:49.000000 valaw-0.0.5/README.md
--rw-rw-rw-   0        0        0       42 2023-04-20 20:05:12.618703 valaw-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1143 2023-04-20 19:36:11.000000 valaw-0.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-20 20:05:12.472818 valaw-0.0.5/src/
-drwxrwxrwx   0        0        0        0 2023-04-20 20:05:12.521143 valaw-0.0.5/src/valaw/
--rw-rw-rw-   0        0        0       73 2023-04-04 05:08:42.000000 valaw-0.0.5/src/valaw/__init__.py
--rw-rw-rw-   0        0        0    13699 2023-04-20 19:46:04.000000 valaw-0.0.5/src/valaw/client.py
-drwxrwxrwx   0        0        0        0 2023-04-20 20:05:12.610672 valaw-0.0.5/src/valaw.egg-info/
--rw-rw-rw-   0        0        0     2306 2023-04-20 20:05:12.000000 valaw-0.0.5/src/valaw.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      232 2023-04-20 20:05:12.000000 valaw-0.0.5/src/valaw.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-20 20:05:12.000000 valaw-0.0.5/src/valaw.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2023-04-20 20:05:12.000000 valaw-0.0.5/src/valaw.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-04-20 20:05:12.000000 valaw-0.0.5/src/valaw.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-05 01:52:33.402411 valaw-0.0.6/
+-rw-rw-rw-   0        0        0     1091 2023-04-13 23:03:00.000000 valaw-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0     2306 2023-05-05 01:52:33.401901 valaw-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1623 2023-04-15 04:19:42.000000 valaw-0.0.6/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-05 01:52:33.402411 valaw-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1192 2023-04-25 02:46:12.000000 valaw-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-05 01:52:33.372742 valaw-0.0.6/src/
+drwxrwxrwx   0        0        0        0 2023-05-05 01:52:33.380945 valaw-0.0.6/src/valaw/
+-rw-rw-rw-   0        0        0       73 2023-04-13 23:03:00.000000 valaw-0.0.6/src/valaw/__init__.py
+-rw-rw-rw-   0        0        0    17479 2023-04-25 03:35:10.000000 valaw-0.0.6/src/valaw/client.py
+drwxrwxrwx   0        0        0        0 2023-05-05 01:52:33.400884 valaw-0.0.6/src/valaw/objects/
+-rw-rw-rw-   0        0        0      272 2023-04-25 02:57:23.000000 valaw-0.0.6/src/valaw/objects/account.py
+-rw-rw-rw-   0        0        0     1271 2023-04-25 03:07:41.000000 valaw-0.0.6/src/valaw/objects/content.py
+-rw-rw-rw-   0        0        0      159 2023-04-25 02:10:48.000000 valaw-0.0.6/src/valaw/objects/error.py
+-rw-rw-rw-   0        0        0     3269 2023-04-25 03:10:46.000000 valaw-0.0.6/src/valaw/objects/match.py
+-rw-rw-rw-   0        0        0      377 2023-04-25 02:01:45.000000 valaw-0.0.6/src/valaw/objects/ranked.py
+-rw-rw-rw-   0        0        0      719 2023-04-25 03:21:46.000000 valaw-0.0.6/src/valaw/objects/status.py
+drwxrwxrwx   0        0        0        0 2023-05-05 01:52:33.396297 valaw-0.0.6/src/valaw.egg-info/
+-rw-rw-rw-   0        0        0     2306 2023-05-05 01:52:33.000000 valaw-0.0.6/src/valaw.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      400 2023-05-05 01:52:33.000000 valaw-0.0.6/src/valaw.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 01:52:33.000000 valaw-0.0.6/src/valaw.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-05-05 01:52:33.000000 valaw-0.0.6/src/valaw.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-05 01:52:33.000000 valaw-0.0.6/src/valaw.egg-info/top_level.txt
```

### Comparing `valaw-0.0.5/LICENSE` & `valaw-0.0.6/LICENSE`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -14,8 +14,8 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+SOFTWARE.
```

### Comparing `valaw-0.0.5/PKG-INFO` & `valaw-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: valaw
-Version: 0.0.5
+Version: 0.0.6
 Summary: An asynchronous API wrapper for VALORANT's API
 Home-page: https://github.com/Jet612/valaw
 Author: Jet612
 Project-URL: Documentation, https://valaw.readthedocs.io
 Project-URL: Issue Tracker, https://github.com/Jet612/valaw/issues
 Project-URL: Chat/Support, https://discord.gg/mVXpvunBbF
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `valaw-0.0.5/README.md` & `valaw-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `valaw-0.0.5/setup.py` & `valaw-0.0.6/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_namespace_packages
 
 with open("README.md", "r") as readme:
     long_desc = readme.read()
 
 setup(
     name="valaw",
-    version="0.0.5",
+    version="0.0.6",
     author="Jet612",
     description="An asynchronous API wrapper for VALORANT's API",
     long_description=long_desc,
     long_description_content_type="text/markdown",
     url="https://github.com/Jet612/valaw",
     project_urls={
         "Documentation": "https://valaw.readthedocs.io",
@@ -25,10 +25,11 @@
     ],
     package_dir={"": "src"},
     packages=find_namespace_packages(where="src"),
     include_package_data=True,
     python_requires=">=3.8",
     install_requires=[
                     'aiohttp==3.8.3',
+                    'dataclass_wizard==0.22.2',
                     'setuptools==67.6.0'
                     ]
 )
```

### Comparing `valaw-0.0.5/src/valaw.egg-info/PKG-INFO` & `valaw-0.0.6/src/valaw.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: valaw
-Version: 0.0.5
+Version: 0.0.6
 Summary: An asynchronous API wrapper for VALORANT's API
 Home-page: https://github.com/Jet612/valaw
 Author: Jet612
 Project-URL: Documentation, https://valaw.readthedocs.io
 Project-URL: Issue Tracker, https://github.com/Jet612/valaw/issues
 Project-URL: Chat/Support, https://discord.gg/mVXpvunBbF
 Classifier: Programming Language :: Python :: 3.8
```

