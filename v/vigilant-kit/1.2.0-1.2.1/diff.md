# Comparing `tmp/vigilant_kit-1.2.0.tar.gz` & `tmp/vigilant_kit-1.2.1.tar.gz`

## Comparing `vigilant_kit-1.2.0.tar` & `vigilant_kit-1.2.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 vigilant_kit-1.2.0/.vigilant.env.example
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 vigilant_kit-1.2.0/docs/actions.md
--rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 vigilant_kit-1.2.0/docs/browser_options.md
--rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 vigilant_kit-1.2.0/docs/native_selenium.md
--rw-r--r--   0        0        0     2406 2020-02-02 00:00:00.000000 vigilant_kit-1.2.0/docs/selenium_install.md
--rw-r--r--   0        0        0    11059 2020-02-02 00:00:00.000000 vigilant_kit-1.2.0/docs/tutorial_pytest.md
--rw-r--r--   0        0        0     2579 2020-02-02 00:00:00.000000 vigilant_kit-1.2.0/docs/vigilant_pytest.md
--rw-r--r--   0        0        0     1779 2020-02-02 00:00:00.000000 vigilant_kit-1.2.0/docs/vigilant_unittest.md
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 vigilant_kit-1.2.0/src/vgl_cli/install_dev_kit_command.py
--rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 vigilant_kit-1.2.0/src/vgl_cli/install_standalone_command.py
--rw-r--r--   0        0        0     5058 2020-02-02 00:00:00.000000 vigilant_kit-1.2.0/src/vgl_cli/install_webdriver_command.py
--rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 vigilant_kit-1.2.0/src/vgl_cli/run_selenium_command.py
--rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 vigilant_kit-1.2.0/src/vgl_cli/vgl.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vigilant_kit-1.2.0/src/vigilant/__init__.py
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 vigilant_kit-1.2.0/src/vigilant/logger.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vigilant_kit-1.2.0/src/vigilant/actions/__init__.py
--rw-r--r--   0        0        0     4097 2020-02-02 00:00:00.000000 vigilant_kit-1.2.0/src/vigilant/actions/assertions.py
--rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 vigilant_kit-1.2.0/src/vigilant/actions/finder.py
--rw-r--r--   0        0        0     7286 2020-02-02 00:00:00.000000 vigilant_kit-1.2.0/src/vigilant/actions/vigilant_actions.py
--rw-r--r--   0        0        0     3298 2020-02-02 00:00:00.000000 vigilant_kit-1.2.0/src/vigilant/actions/waiter.py
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 vigilant_kit-1.2.0/src/vigilant/driver/__init__.py
--rw-r--r--   0        0        0     3398 2020-02-02 00:00:00.000000 vigilant_kit-1.2.0/src/vigilant/driver/vigilant_driver.py
--rw-r--r--   0        0        0     3076 2020-02-02 00:00:00.000000 vigilant_kit-1.2.0/.gitignore
--rw-r--r--   0        0        0    35125 2020-02-02 00:00:00.000000 vigilant_kit-1.2.0/LICENSE
--rw-r--r--   0        0        0     5636 2020-02-02 00:00:00.000000 vigilant_kit-1.2.0/README.md
--rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 vigilant_kit-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     6233 2020-02-02 00:00:00.000000 vigilant_kit-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 vigilant_kit-1.2.1/.vigilant.env.example
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 vigilant_kit-1.2.1/docs/actions.md
+-rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 vigilant_kit-1.2.1/docs/browser_options.md
+-rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 vigilant_kit-1.2.1/docs/native_selenium.md
+-rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 vigilant_kit-1.2.1/docs/selenium_install.md
+-rw-r--r--   0        0        0    11059 2020-02-02 00:00:00.000000 vigilant_kit-1.2.1/docs/tutorial_pytest.md
+-rw-r--r--   0        0        0     2579 2020-02-02 00:00:00.000000 vigilant_kit-1.2.1/docs/vigilant_pytest.md
+-rw-r--r--   0        0        0     3895 2020-02-02 00:00:00.000000 vigilant_kit-1.2.1/docs/vigilant_unittest.md
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 vigilant_kit-1.2.1/src/vgl_cli/install_dev_kit_command.py
+-rw-r--r--   0        0        0     1439 2020-02-02 00:00:00.000000 vigilant_kit-1.2.1/src/vgl_cli/install_standalone_command.py
+-rw-r--r--   0        0        0     5058 2020-02-02 00:00:00.000000 vigilant_kit-1.2.1/src/vgl_cli/install_webdriver_command.py
+-rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 vigilant_kit-1.2.1/src/vgl_cli/run_selenium_command.py
+-rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 vigilant_kit-1.2.1/src/vgl_cli/vgl.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vigilant_kit-1.2.1/src/vigilant/__init__.py
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 vigilant_kit-1.2.1/src/vigilant/logger.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 vigilant_kit-1.2.1/src/vigilant/actions/__init__.py
+-rw-r--r--   0        0        0     4097 2020-02-02 00:00:00.000000 vigilant_kit-1.2.1/src/vigilant/actions/assertions.py
+-rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 vigilant_kit-1.2.1/src/vigilant/actions/finder.py
+-rw-r--r--   0        0        0     7286 2020-02-02 00:00:00.000000 vigilant_kit-1.2.1/src/vigilant/actions/vigilant_actions.py
+-rw-r--r--   0        0        0     3298 2020-02-02 00:00:00.000000 vigilant_kit-1.2.1/src/vigilant/actions/waiter.py
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 vigilant_kit-1.2.1/src/vigilant/driver/__init__.py
+-rw-r--r--   0        0        0     3398 2020-02-02 00:00:00.000000 vigilant_kit-1.2.1/src/vigilant/driver/vigilant_driver.py
+-rw-r--r--   0        0        0     3076 2020-02-02 00:00:00.000000 vigilant_kit-1.2.1/.gitignore
+-rw-r--r--   0        0        0    35125 2020-02-02 00:00:00.000000 vigilant_kit-1.2.1/LICENSE
+-rw-r--r--   0        0        0     1969 2020-02-02 00:00:00.000000 vigilant_kit-1.2.1/README.md
+-rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 vigilant_kit-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0     2566 2020-02-02 00:00:00.000000 vigilant_kit-1.2.1/PKG-INFO
```

### Comparing `vigilant_kit-1.2.0/docs/browser_options.md` & `vigilant_kit-1.2.1/docs/browser_options.md`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.2.0/docs/native_selenium.md` & `vigilant_kit-1.2.1/docs/native_selenium.md`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.2.0/docs/tutorial_pytest.md` & `vigilant_kit-1.2.1/docs/tutorial_pytest.md`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.2.0/docs/vigilant_pytest.md` & `vigilant_kit-1.2.1/docs/vigilant_pytest.md`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.2.0/src/vgl_cli/install_dev_kit_command.py` & `vigilant_kit-1.2.1/src/vgl_cli/install_dev_kit_command.py`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.2.0/src/vgl_cli/install_standalone_command.py` & `vigilant_kit-1.2.1/src/vgl_cli/install_standalone_command.py`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.2.0/src/vgl_cli/install_webdriver_command.py` & `vigilant_kit-1.2.1/src/vgl_cli/install_webdriver_command.py`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.2.0/src/vgl_cli/run_selenium_command.py` & `vigilant_kit-1.2.1/src/vgl_cli/run_selenium_command.py`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.2.0/src/vgl_cli/vgl.py` & `vigilant_kit-1.2.1/src/vgl_cli/vgl.py`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.2.0/src/vigilant/actions/assertions.py` & `vigilant_kit-1.2.1/src/vigilant/actions/assertions.py`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.2.0/src/vigilant/actions/finder.py` & `vigilant_kit-1.2.1/src/vigilant/actions/finder.py`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.2.0/src/vigilant/actions/vigilant_actions.py` & `vigilant_kit-1.2.1/src/vigilant/actions/vigilant_actions.py`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.2.0/src/vigilant/actions/waiter.py` & `vigilant_kit-1.2.1/src/vigilant/actions/waiter.py`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.2.0/src/vigilant/driver/vigilant_driver.py` & `vigilant_kit-1.2.1/src/vigilant/driver/vigilant_driver.py`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.2.0/.gitignore` & `vigilant_kit-1.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.2.0/LICENSE` & `vigilant_kit-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vigilant_kit-1.2.0/README.md` & `vigilant_kit-1.2.1/docs/vigilant_unittest.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,54 +1,15 @@
-# Vigilant Kit
-Vigilant is a set of tools made to help writing and running robust functional tests using Selenium WebDriver.
-
-## Why Vigilant?
- - It allows you to start writing complex test cases in a minute.
- - Simple configuration process (just one `.vigilant.env` file to start)
- - Usage is not limited to a single testing framework, it can be used with `unittest`, `pytest` or anything else.
-It is up to you.
-
-**Vigilant** provide you with methods that help write functional tests fast, without spending your time on writing
-boilerplate code every time you start new project.
-
-Methods for **interacting** with WebBrowser (`click`, `scroll_to`,  etc.), **assertions** (`see`, `dont_see`, `see_text`
-, etc.) **waiting** (`wait_for_element_to_be_visible`, `wait_for_element_to_be_clickable`, etc.)
-It is already there, ready to use.
-
-List of all available [actions](docs/actions.md).
-
-### What if you need something that is not covered in this library?
-
-You still have access to all native `Selenium WebDriver` methods. Despite all functional that library provide - 
-you can create your own methods or use native `WebDriver` methods and share them on one browser session.
-
-## Docs
- - [How to install Selenium server & browser drivers](docs/selenium_install.md)
- - [Quick start example using `unittest` library](docs/vigilant_unittest.md) 
- - [Quick start example using `pytest`](docs/vigilant_pytest.md) 
- - [How to add custom browser options](docs/browser_options.md)
- - [Access native Selenium WebDriver methods](docs/native_selenium.md)
- - [List of actions](docs/actions.md).
-
-## Tutorials
- - [Testing ecommerce project using `vigilant-kit` and `pytest`](docs/tutorial_pytest.md)
- 
-## Install
-```shell
-pip install vigilant-kit
-```
-
 ## Quick start
 We will write our first test with `unittest` library. Also make sure that you installed
 `vigilant-kit` library.
 
 
 ### Configuration
 Configuration can be done through environment variables. Make sure that your Selenium Server is up and running, if not -
-[**Install Selenium server**](docs/selenium_install.md)
+[**Install Selenium server**](selenium_install.md)
 
 Create `.vigilant.env` file with next data:
 ```shell
 # Selenium host URL
 SELENIUM_HOST=http://127.0.0.1:4444/wd/hub 
 
 # Browser which will performing the tests
```

### Comparing `vigilant_kit-1.2.0/pyproject.toml` & `vigilant_kit-1.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "vigilant_kit"
-version = "1.2.0"
+version = "1.2.1"
 authors = [
   { name="Pelykh Ivan", email="ivan.pelykh@protonmail.com" },
 ]
 description = "Library that makes functional testing with Selenium WebDriver fast and easy. "
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
```

