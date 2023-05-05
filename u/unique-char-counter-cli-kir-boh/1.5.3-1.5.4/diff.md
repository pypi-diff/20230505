# Comparing `tmp/unique_char_counter_cli_kir_boh-1.5.3.tar.gz` & `tmp/unique_char_counter_cli_kir_boh-1.5.4.tar.gz`

## Comparing `unique_char_counter_cli_kir_boh-1.5.3.tar` & `unique_char_counter_cli_kir_boh-1.5.4.tar`

### file list

```diff
@@ -1,15 +1,21 @@
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.3/.idea/.gitignore
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.3/.idea/Task 5 Package.iml
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.3/.idea/misc.xml
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.3/.idea/modules.xml
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.3/.idea/vcs.xml
--rw-r--r--   0        0        0     3634 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.3/.idea/workspace.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.3/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.3/src/unique_char_counter_cli_kir_boh/__init__.py
--rw-r--r--   0        0        0     1827 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.3/src/unique_char_counter_cli_kir_boh/unique_char_counter_cli.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.3/src/unique_char_counter_cli_kir_boh/tests/__init__.py
--rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.3/src/unique_char_counter_cli_kir_boh/tests/tests_unique_char_counter_cli.py
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.3/LICENSE
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.3/README.md
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.3/pyproject.toml
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.3/PKG-INFO
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.4/.idea/.gitignore
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.4/.idea/Task 5 Package.iml
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.4/.idea/misc.xml
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.4/.idea/modules.xml
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.4/.idea/vcs.xml
+-rw-r--r--   0        0        0     4776 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.4/.idea/workspace.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.4/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.4/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.4/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.4/.pytest_cache/README.md
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.4/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.4/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.4/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.4/src/unique_char_counter_cli_kir_boh/__init__.py
+-rw-r--r--   0        0        0     1827 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.4/src/unique_char_counter_cli_kir_boh/unique_char_counter_cli.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.4/src/unique_char_counter_cli_kir_boh/tests/__init__.py
+-rw-r--r--   0        0        0     2008 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.4/src/unique_char_counter_cli_kir_boh/tests/tests_unique_char_counter_cli.py
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.4/LICENSE
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.4/README.md
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.4/pyproject.toml
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 unique_char_counter_cli_kir_boh-1.5.4/PKG-INFO
```

### Comparing `unique_char_counter_cli_kir_boh-1.5.3/.idea/workspace.xml` & `unique_char_counter_cli_kir_boh-1.5.4/.idea/workspace.xml`

 * *Files 23% similar despite different names*

#### Comparing `unique_char_counter_cli_kir_boh-1.5.3/.idea/workspace.xml` & `unique_char_counter_cli_kir_boh-1.5.4/.idea/workspace.xml`

```diff
@@ -40,15 +40,15 @@
   }
 }]]></component>
   <component name="RecentsManager">
     <key name="MoveFile.RECENT_KEYS">
       <recent name="C:\Users\Кирило\FoxEd\Task 5 Package\src\unique_char_counter_cli_kir_boh"/>
     </key>
   </component>
-  <component name="RunManager">
+  <component name="RunManager" selected="Python tests.Python tests in tests_unique_char_counter_cli.py">
     <configuration name="main" type="PythonConfigurationType" factoryName="Python" nameIsGenerated="true">
       <module name="Task 5 Package"/>
       <option name="INTERPRETER_OPTIONS" value=""/>
       <option name="PARENT_ENVS" value="true"/>
       <envs>
         <env name="PYTHONUNBUFFERED" value="1"/>
       </envs>
@@ -62,14 +62,33 @@
       <option name="SHOW_COMMAND_LINE" value="false"/>
       <option name="EMULATE_TERMINAL" value="false"/>
       <option name="MODULE_MODE" value="false"/>
       <option name="REDIRECT_INPUT" value="false"/>
       <option name="INPUT_FILE" value=""/>
       <method v="2"/>
     </configuration>
+    <configuration name="Python tests in tests_unique_char_counter_cli.py" type="tests" factoryName="Autodetect" temporary="true" nameIsGenerated="true">
+      <module name="Task 5 Package"/>
+      <option name="INTERPRETER_OPTIONS" value=""/>
+      <option name="PARENT_ENVS" value="true"/>
+      <option name="SDK_HOME" value=""/>
+      <option name="WORKING_DIRECTORY" value="$PROJECT_DIR$"/>
+      <option name="IS_MODULE_SDK" value="true"/>
+      <option name="ADD_CONTENT_ROOTS" value="true"/>
+      <option name="ADD_SOURCE_ROOTS" value="true"/>
+      <option name="_new_additionalArguments" value="&quot;&quot;"/>
+      <option name="_new_target" value="&quot;$PROJECT_DIR$/src/unique_char_counter_cli_kir_boh/tests/tests_unique_char_counter_cli.py&quot;"/>
+      <option name="_new_targetType" value="&quot;PATH&quot;"/>
+      <method v="2"/>
+    </configuration>
+    <recent_temporary>
+      <list>
+        <item itemvalue="Python tests.Python tests in tests_unique_char_counter_cli.py"/>
+      </list>
+    </recent_temporary>
   </component>
   <component name="SpellCheckerSettings" RuntimeDictionaries="0" Folders="0" CustomDictionaries="0" DefaultDictionary="application-level" UseSingleDictionary="true" transferred="true"/>
   <component name="TaskManager">
     <task active="true" id="Default" summary="Default task">
       <changelist id="4f5767a4-6088-4d9f-af6d-f4455ea21aad" name="Changes" comment=""/>
       <created>1683227041829</created>
       <option name="number" value="Default"/>
```

### Comparing `unique_char_counter_cli_kir_boh-1.5.3/src/unique_char_counter_cli_kir_boh/unique_char_counter_cli.py` & `unique_char_counter_cli_kir_boh-1.5.4/src/unique_char_counter_cli_kir_boh/unique_char_counter_cli.py`

 * *Files identical despite different names*

### Comparing `unique_char_counter_cli_kir_boh-1.5.3/src/unique_char_counter_cli_kir_boh/tests/tests_unique_char_counter_cli.py` & `unique_char_counter_cli_kir_boh-1.5.4/src/unique_char_counter_cli_kir_boh/tests/tests_unique_char_counter_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from argparse import Namespace
 import unittest
 from unittest.mock import patch, mock_open
-from ...unique_char_counter_cli_kir_boh import unique_char_counter_cli
+from unique_char_counter_cli_kir_boh import unique_char_counter_cli
 
 
 class TestUniqueCharCounterCli(unittest.TestCase):
     def test_return_amount_once_occured_items_with_string(self):
         self.assertEqual(unique_char_counter_cli.return_amount_once_occured_items('11adadfgfgfacehgj'), 4)
 
     def test_return_amount_once_occured_items_with_empty_string(self):
@@ -21,15 +21,15 @@
 
     @patch('unique_char_counter_cli.unique_char_counter_cli.get_obj_from_cli')
     @patch('builtins.open', new_callable=mock_open, read_data='dataff')
     def test_main_with_mock_file(self, mock_open, mock_get_obj_from_cli):
         mock_get_obj_from_cli.return_value = Namespace(string=False, file=True, hashable_obj='some file')
         self.assertEqual(unique_char_counter_cli.main(), 2)
 
-    @patch('unique_char_counter_cli.unique_char_counter_cli.get_obj_from_cli')
+    @patch('unique_char_counter_cli_kir_boh.unique_char_counter_cli.get_obj_from_cli')
     def test_main_with_mock_file(self, mock_get_obj_from_cli):
         mock_get_obj_from_cli.return_value = Namespace(string=True, file=False, hashable_obj='some file')
         self.assertEqual(unique_char_counter_cli.main(), 7)
 
 
     @patch('builtins.open', new_callable=mock_open, read_data='dat\nafff')
     def test_read_file_in_chunks(self, mock_open):
```

### Comparing `unique_char_counter_cli_kir_boh-1.5.3/LICENSE` & `unique_char_counter_cli_kir_boh-1.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `unique_char_counter_cli_kir_boh-1.5.3/pyproject.toml` & `unique_char_counter_cli_kir_boh-1.5.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 
 [project]
 name = "unique_char_counter_cli_kir_boh"
-version = "1.5.3"
+version = "1.5.4"
 authors = [
   { name="Example Author", email="kirillbogatu2005@gmail.com" },
 ]
 description = "Project gets hashable obj from cli an returns uniqe items amount"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

