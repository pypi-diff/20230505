# Comparing `tmp/ontodev_valve-0.2.0-cp39-none-win_amd64.whl.zip` & `tmp/ontodev_valve-0.2.1-cp39-cp39-manylinux_2_31_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 3048164 bytes, number of entries: 6
--rw-r--r--  4.6 unx     2966 b- defN 23-Jan-10 16:22 ontodev_valve-0.2.0.dist-info/METADATA
--rw-r--r--  4.6 unx       95 b- defN 23-Jan-10 16:22 ontodev_valve-0.2.0.dist-info/WHEEL
--rw-r--r--  4.6 unx     1544 b- defN 23-Jan-10 16:22 ontodev_valve-0.2.0.dist-info/license_files/LICENSE
--rw-r--r--  4.6 unx      135 b- defN 23-Jan-10 16:22 ontodev_valve/__init__.py
--rwxr-xr-x  4.6 unx  7088640 b- defN 23-Jan-10 16:22 ontodev_valve/ontodev_valve.cp39-win_amd64.pyd
--rw-r--r--  4.6 unx      519 b- defN 23-Jan-10 16:22 ontodev_valve-0.2.0.dist-info/RECORD
-6 files, 7093899 bytes uncompressed, 3047224 bytes compressed:  57.1%
+Zip file size: 4937380 bytes, number of entries: 6
+-rw-r--r--  4.6 unx     3454 b- defN 23-May-05 17:49 ontodev_valve-0.2.1.dist-info/METADATA
+-rw-r--r--  4.6 unx      108 b- defN 23-May-05 17:49 ontodev_valve-0.2.1.dist-info/WHEEL
+-rw-r--r--  4.6 unx     1515 b- defN 23-May-05 17:49 ontodev_valve-0.2.1.dist-info/license_files/LICENSE
+-rw-r--r--  4.6 unx      135 b- defN 23-May-05 17:49 ontodev_valve/__init__.py
+-rwxr-xr-x  4.6 unx 14545728 b- defN 23-May-05 17:49 ontodev_valve/ontodev_valve.cpython-39-x86_64-linux-gnu.so
+-rw-r--r--  4.6 unx      533 b- defN 23-May-05 17:49 ontodev_valve-0.2.1.dist-info/RECORD
+6 files, 14551473 bytes uncompressed, 4936416 bytes compressed:  66.1%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
-Filename: ontodev_valve-0.2.0.dist-info/METADATA
+Filename: ontodev_valve-0.2.1.dist-info/METADATA
 Comment: 
 
-Filename: ontodev_valve-0.2.0.dist-info/WHEEL
+Filename: ontodev_valve-0.2.1.dist-info/WHEEL
 Comment: 
 
-Filename: ontodev_valve-0.2.0.dist-info/license_files/LICENSE
+Filename: ontodev_valve-0.2.1.dist-info/license_files/LICENSE
 Comment: 
 
 Filename: ontodev_valve/__init__.py
 Comment: 
 
-Filename: ontodev_valve/ontodev_valve.cp39-win_amd64.pyd
+Filename: ontodev_valve/ontodev_valve.cpython-39-x86_64-linux-gnu.so
 Comment: 
 
-Filename: ontodev_valve-0.2.0.dist-info/RECORD
+Filename: ontodev_valve-0.2.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `ontodev_valve-0.2.0.dist-info/METADATA` & `ontodev_valve-0.2.1.dist-info/METADATA`

 * *Files 10% similar despite different names*

```diff
@@ -1,65 +1,85 @@
 Metadata-Version: 2.1
 Name: ontodev_valve
-Version: 0.2.0
+Version: 0.2.1
 License-File: LICENSE
 Summary: VALVE bindings for Python
 Author: Knocean Inc.
 License: BSD-3-Clause
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Project-URL: Homepage, https://github.com/ontodev/valve.py
 
-# valve.py
-VALVE bindings for Python
-
-## Install/setup from source
-
-1. Retrieve valve.py from GitHub:
-
-	    git clone git@github.com:ontodev/valve.py.git
-	    cd valve.py
-	    make test
-
-2. Activate the virtual environment:
-
-        source valve.rs/.venv/bin/activate
-
-3. Add the statement
-
-        import ontodev_valve
-
-    to the top of your python script.
-
-## Usage examples
-
-See the file `test/main.py` for usage examples.
-
-## API reference
-
-### `configure_and_or_load(table_table, db_path, load, verbose)`
-
-Given a path to a table table file (table.tsv), a directory in which to find/create a database: configure the database using the configuration which can be looked up using the table table, and optionally load it if the `load` flag is set to true. If the `verbose` flag is also set to true, output progress messages while loading.
-
-
-Returns the configuration map back as a JSON string.
-
-### `get_matching_values(config, db_path, table_name, column_name, matching_string)`
-
-Given a config map represented as a JSON string, a directory containing the database, the table name and column name from which to retrieve matching values, return a JSON array (represented as a string) of possible valid values for the given column which contain the matching string (optional) as a substring (or all of them if no matching string is given). The JSON array returned is formatted for Typeahead, i.e., it takes the form: `[{"id": id, "label": label, "order": order}, ...]`.
-
-### `validate_row(config, db_path, table_name, row, existing_row, row_number)`
-
-Given a config map represented as a JSON string, a directory in which to find the database, a table name, a row, and if the row already exists in the database, its associated row number (optional), perform both intra- and inter-row validation and return the validated row as a JSON string.
-
-### `update_row(config, db_path, table_name, row, row_number)`
-
-Given a config map represented as a JSON string, a directory in which the database is located, a table name, a row represented as a JSON string, and its associated row number, update the row in the database.
-
-### `insert_new_row(config, db_path, table_name, row)`
-
-Given a config map represented as a JSON string, a directory in which the database is located, a table name, and a row represented as a JSON string, insert the new row to the database.
-
-## Before creating a new release
-
-Edit the file `VALVE.VERSION` and adjust the version of valve.py (and, if necessary, valve.rs). After pushing your commit, create a new release in GitHub with the new version number as the release name and tag.
+# valve.py
+VALVE bindings for Python
+
+## Install/setup from source
+
+1. Retrieve valve.py from GitHub:
+
+	    git clone git@github.com:ontodev/valve.py.git
+	    cd valve.py
+	    make test
+
+2. Activate the virtual environment:
+
+        source valve.rs/.venv/bin/activate
+
+3. Add the statement
+
+        import ontodev_valve
+
+    to the top of your python script.
+
+## Usage examples
+
+See the file `test/main.py` for usage examples.
+
+## API reference
+
+### `valve(table_table, db_path, command, verbose, config_table="table")`
+
+Given a path to a configuration table (either a table.tsv file or a database containing a
+table named "table"), and a directory in which to find/create a database: configure the
+database using the configuration which can be looked up using the table table, and
+optionally create and/or load it according to the value of `command`
+(see [Valve Command](#ValveCommand)). If the `verbose` flag is set to true, output status
+messages while loading. If `config_table` (which defaults to "table") is given and
+`table_table` indicates a database, query the table called `config_table` for the
+table table information. Returns the configuration map as a String.
+
+### `get_matching_values(config, db_path, table_name, column_name, matching_string)`
+
+Given a config map represented as a JSON string, a directory containing the database, the table name and column name from which to retrieve matching values, return a JSON array (represented as a string) of possible valid values for the given column which contain the matching string (optional) as a substring (or all of them if no matching string is given). The JSON array returned is formatted for Typeahead, i.e., it takes the form: `[{"id": id, "label": label, "order": order}, ...]`.
+
+### `validate_row(config, db_path, table_name, row, existing_row, row_number)`
+
+Given a config map represented as a JSON string, a directory in which to find the database, a table name, a row, and if the row already exists in the database, its associated row number (optional), perform both intra- and inter-row validation and return the validated row as a JSON string.
+
+### `update_row(config, db_path, table_name, row, row_number)`
+
+Given a config map represented as a JSON string, a directory in which the database is located, a table name, a row represented as a JSON string, and its associated row number, update the row in the database.
+
+### `insert_new_row(config, db_path, table_name, row)`
+
+Given a config map represented as a JSON string, a directory in which the database is located, a table name, and a row represented as a JSON string, insert the new row to the database.
+
+### ValveCommand
+
+The following commands may be used with the valve() function.
+
+#### ValveCommand.Config
+
+Configure but do not create or load.
+
+#### ValveCommand.Create
+
+Configure and create but do not load.
+
+#### ValveCommand.Load
+
+Configure, create, and load.
+
+## Before creating a new release
+
+Edit the file `VALVE.VERSION` and adjust the version of valve.py (and, if necessary, valve.rs). After pushing your commit, create a new release in GitHub with the new version number as the release name and tag.
```

## Comparing `ontodev_valve-0.2.0.dist-info/license_files/LICENSE` & `ontodev_valve-0.2.1.dist-info/license_files/LICENSE`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-BSD 3-Clause License
-
-Copyright (c) 2020, OntoDev
-All rights reserved.
-
-Redistribution and use in source and binary forms, with or without
-modification, are permitted provided that the following conditions are met:
-
-1. Redistributions of source code must retain the above copyright notice, this
-   list of conditions and the following disclaimer.
-
-2. Redistributions in binary form must reproduce the above copyright notice,
-   this list of conditions and the following disclaimer in the documentation
-   and/or other materials provided with the distribution.
-
-3. Neither the name of the copyright holder nor the names of its
-   contributors may be used to endorse or promote products derived from
-   this software without specific prior written permission.
-
-THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
-AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
-IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
-DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
-FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
-DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
-SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
-CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
-OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
-OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+BSD 3-Clause License
+
+Copyright (c) 2020, OntoDev
+All rights reserved.
+
+Redistribution and use in source and binary forms, with or without
+modification, are permitted provided that the following conditions are met:
+
+1. Redistributions of source code must retain the above copyright notice, this
+   list of conditions and the following disclaimer.
+
+2. Redistributions in binary form must reproduce the above copyright notice,
+   this list of conditions and the following disclaimer in the documentation
+   and/or other materials provided with the distribution.
+
+3. Neither the name of the copyright holder nor the names of its
+   contributors may be used to endorse or promote products derived from
+   this software without specific prior written permission.
+
+THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
+FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
+DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
+SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
+CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
+OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
+OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
```

