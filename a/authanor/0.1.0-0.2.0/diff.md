# Comparing `tmp/authanor-0.1.0.tar.gz` & `tmp/authanor-0.2.0.tar.gz`

## Comparing `authanor-0.1.0.tar` & `authanor-0.2.0.tar`

### file list

```diff
@@ -1,9 +1,11 @@
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 authanor-0.1.0/authanor/_version.py
--rw-r--r--   0        0        0    15543 2020-02-02 00:00:00.000000 authanor-0.1.0/authanor/handler.py
--rw-r--r--   0        0        0     3613 2020-02-02 00:00:00.000000 authanor-0.1.0/authanor/models.py
--rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 authanor-0.1.0/authanor/utils.py
--rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 authanor-0.1.0/.gitignore
--rw-r--r--   0        0        0    35150 2020-02-02 00:00:00.000000 authanor-0.1.0/COPYING
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 authanor-0.1.0/LICENSE
--rw-r--r--   0        0        0     1822 2020-02-02 00:00:00.000000 authanor-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3065 2020-02-02 00:00:00.000000 authanor-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 authanor-0.2.0/authanor/_version.py
+-rw-r--r--   0        0        0     3985 2020-02-02 00:00:00.000000 authanor-0.2.0/authanor/database/__init__.py
+-rw-r--r--   0        0        0    18062 2020-02-02 00:00:00.000000 authanor-0.2.0/authanor/database/handler.py
+-rw-r--r--   0        0        0     5545 2020-02-02 00:00:00.000000 authanor-0.2.0/authanor/database/models.py
+-rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 authanor-0.2.0/authanor/database/utils.py
+-rw-r--r--   0        0        0    10612 2020-02-02 00:00:00.000000 authanor-0.2.0/authanor/test/helpers.py
+-rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 authanor-0.2.0/.gitignore
+-rw-r--r--   0        0        0    35150 2020-02-02 00:00:00.000000 authanor-0.2.0/COPYING
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 authanor-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2166 2020-02-02 00:00:00.000000 authanor-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3146 2020-02-02 00:00:00.000000 authanor-0.2.0/PKG-INFO
```

### Comparing `authanor-0.1.0/authanor/handler.py` & `authanor-0.2.0/authanor/database/handler.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """
 A database handler for facilitating interactions with the SQLite database.
 """
+import functools
 from abc import ABCMeta
 from collections import UserList
 
 from flask import current_app, g
-from sqlalchemy import inspect, select
+from sqlalchemy import select
 from sqlalchemy.exc import ArgumentError, NoResultFound
 from werkzeug.exceptions import abort
 
 from .models import AuthorizedAccessMixin
 from .utils import validate_sort_order
 
 
@@ -42,15 +43,15 @@
 
     @property
     def model(cls):
         return cls._get_required_attribute_data_descriptor("model")
 
     @property
     def table(cls):
-        return cls.model.__tablename__
+        return cls.model.__table__
 
     def _get_required_attribute_data_descriptor(cls, name):
         # The named property/attribute is a data descriptor, so standard overrides are
         # not permitted; instead, the metaclass property must reference the true
         # class's dictionary of values to get the overridden attribute
         value = cls.__dict__.get(name)
         if value:
@@ -87,19 +88,19 @@
 
     @property
     def model(cls):
         return cls._model_view if cls._view_context else cls._model
 
     @property
     def table(cls):
-        return cls._model.__tablename__
+        return cls._model.__table__
 
     @property
     def table_view(cls):
-        return cls._model_view.__tablename__
+        return cls._model_view.__table__
 
 
 class QueryCriteria(UserList):
     """
     A helper object for constructing queries using a database handler.
     """
 
@@ -127,15 +128,15 @@
                 criterion = getattr(model, field).in_(values)
             except ArgumentError:
                 criterion = getattr(model, field) == values
             self.data.append(criterion)
             self.discriminators.append(model)
 
     def append(self, item):
-        raise NotImplementedError(
+        raise RuntimeError(
             "The `QueryCriteria` object can not be appended to directly. Use a helper "
             "method (e.g., `add_match_filter`) instead."
         )
 
 
 class DatabaseHandlerMixin:
     """
@@ -149,157 +150,213 @@
     handler to be shared by any objects that implement the database
     handler interface.
     """
 
     _initialize_criteria_list = QueryCriteria
 
     @classmethod
-    def _make_select_query(cls, model, **kwargs):
+    def _build_select_query(cls, **kwargs):
         # Query entries for the authorized user (or fall back to SQLAlchemy `select`)
         select_method = getattr(cls.model, "select_for_user", select)
         query = select_method(cls.model, **kwargs)
         return query
 
     @classmethod
-    def get_entries(cls, criteria=None, sort_order=None, **kwargs):
+    def _customize_entries_query(cls, query, criteria, column_orders):
         """
-        Retrieve a set of entries from the database.
-
-        Executes a simple query to select the table entries from
-        the database which match the given filters.
+        Customize a query to retrieve entries from the database.
 
         Parameters
         ----------
+        query : sqlalchemy.sql.expression.Select
+            The query to be customized.
         criteria : QueryCriteria
-            Criteria to use when applying filters to the query.
-            (A filter with a value of `None` will be ignored.)
-        sort_order : str
-            The order to use when sorting values returned by the
-            database query.
+            Additional criteria to use when applying filters to the
+            query. (Any filters with a value of `None` will be ignored.)
+        column_orders : dict
+            A mapping between columns and the sorting order to
+            apply to those columns (e.g., 'ASC' or 'DESC'). Columns will
+            be sorted first to last.
 
         Returns
         -------
-        entries : list of database.models.Model
-            Models containing matching entries from the database.
-        """
-        query = cls._make_select_query(cls.model, **kwargs)
-        query = cls._customize_entries_query(query, criteria, sort_order)
-        entries = cls._db.session.execute(query).scalars()
-        return entries
-
-    @classmethod
-    def find_entry(cls, criteria=None, sort_order=None, require_unique=True):
-        """
-        Find an entry using uniquely identifying characteristics.
-
-        Parameters
-        ----------
-        criteria : QueryCriteria
-            Criteria to use when applying filters to the query. (If all
-            criteria are `None`, the returned entry will be `None`.)
-        sort_order : str
-            The order to use when sorting values returned by the
-            database query.
-        require_unique : bool
-            A flag indicating whether a found entry must be the one and
-            only entry matching the criteria. The default is `True`, and
-            if an entry is not the only one matching the criteria, an
-            error is raised.
-
-        Returns
-        -------
-        entry : database.models.Model
-            A model containing a matching entry from the database.
-        """
-        if criteria:
-            # Query entries from the authorized user
-            query = cls._make_select_query(cls.model)
-            query = cls._customize_entries_query(query, criteria, sort_order)
-            results = cls._db.session.execute(query)
-            if require_unique:
-                entry = results.scalar_one_or_none()
-            else:
-                entry = results.scalar()
-            return entry
-        return None
-
-    @classmethod
-    def _customize_entries_query(cls, query, criteria, sort_order):
-        """
-        Customize a query to retrieve entries from the database.
+        query : sqlalchemy.sql.expression.Select
+            The customized (sorted, filtered, etc.) query.
 
         Note
         ----
         As an implementation detail, the query returned by this method
         defined in the lowest level subclass should always be the final
         query executed by the current `Session` object in the
         `get_entries` method.
         """
+        column_orders = column_orders if column_orders else {}
+        query = cls._sort_query(query, column_orders)
         return cls._filter_entries(query, criteria)
 
     @staticmethod
     def _filter_entries(query, criteria):
         """Apply filters to a query based on the given criteria."""
         if criteria:
             query = query.filter(*criteria)
         return query
 
     @classmethod
-    def _sort_query(cls, query, *column_orders):
+    def _execute_query(cls, query):
+        return cls._db.session.execute(query)
+
+    @classmethod
+    def _sort_query(cls, query, column_orders):
         """
         Sort a query on the given column(s).
 
         Parameters
         ----------
         query : sqlalchemy.sql.expression.Select
             The query to be sorted.
-        column_orders : tuple
-            Any number of pairs consisting of a table column and a
-            string giving the sorting order for that column.
+        column_orders :
+            A mapping of pairs consisting of a table column key and a
+            string value describing the sorting order ('ASC' or 'DESC')
+            for the column.
         """
-        for column, sort_order in column_orders:
+        for column, sort_order in column_orders.items():
             if sort_order:
                 validate_sort_order(sort_order)
                 if sort_order == "DESC":
                     order_column = column.desc()
-                else:
+                elif sort_order == "ASC":
                     order_column = column.asc()
                 query = query.order_by(order_column)
         return query
 
     @classmethod
+    def get_entries(cls, entry_ids=None, criteria=None, column_orders=None, **kwargs):
+        """
+        Retrieve a set of entries from the database.
+
+        Executes a simple query to select the table entries from
+        the database which match the given filters.
+
+        Parameters
+        ----------
+        entry_ids : list
+            A set of primary keys (IDs) to be found.
+        criteria : QueryCriteria
+            Additional criteria to use when applying filters to the
+            query. (Any filters with a value of `None` will be ignored.)
+        column_orders : dict
+            A mapping between column names and the sorting order to
+            apply to those columns (e.g., 'ASC' or 'DESC'). Columns will
+            be sorted first to last.
+        **kwargs :
+            Keyword arguments that may be defined for specific handler
+            subclasses.
+
+        Returns
+        -------
+        entries : list of database.models.Model
+            Models containing matching entries from the database.
+        """
+        # Prepare the criteria by merging IDs with other criteria
+        criteria = criteria if criteria else QueryCriteria()
+        criteria.add_match_filter(cls.model, "primary_key_field", entry_ids)
+        # Query the database
+        query = cls._build_select_query(**kwargs)
+        query = cls._customize_entries_query(query, criteria, column_orders)
+        entries = cls._execute_query(query).scalars()
+        return entries
+
+    @classmethod
+    def find_entry(cls, criteria=None, column_orders=None, require_unique=True):
+        """
+        Find an entry using uniquely identifying characteristics.
+
+        Parameters
+        ----------
+        criteria : QueryCriteria
+            Criteria to use when applying filters to the query. (If all
+            criteria are `None`, the returned entry will be `None`.)
+        column_orders : dict
+            A mapping between column names and the sorting order to
+            apply to those columns (e.g., 'ASC' or 'DESC'). Columns will
+            be sorted first to last.
+        require_unique : bool
+            A flag indicating whether a found entry must be the one and
+            only entry matching the criteria. The default is `True`, and
+            if an entry is not the only one matching the criteria, an
+            error is raised.
+
+        Returns
+        -------
+        entry : database.models.Model
+            A model containing a matching entry from the database.
+        """
+        if criteria:
+            # Query entries from the authorized user
+            query = cls._build_select_query()
+            query = cls._customize_entries_query(query, criteria, column_orders)
+            results = cls._execute_query(query)
+            entry = results.scalar_one_or_none() if require_unique else results.scalar()
+            return entry
+        return None
+
+    @classmethod
     def get_entry(cls, entry_id):
         """
         Retrieve a single entry from the database.
 
         Executes a simple query from the database to get a single entry
-        by ID.
+        by its primary key (most often its ID).
 
         Parameters
         ----------
         entry_id : int
-            The ID of the entry to be found.
+            The primary key (ID) of the entry to be found.
 
         Returns
         -------
         entry : database.models.Model
             A model containing a matching entry from the database.
         """
-        criteria = [cls.model.id == entry_id]
-        query = cls.model.select_for_user().where(*criteria)
+        criteria = QueryCriteria()
+        criteria.add_match_filter(cls.model, "primary_key_field", entry_id)
+        query = cls._build_select_query().where(*criteria)
         try:
-            entry = cls._db.session.execute(query).scalar_one()
+            entry = cls._execute_query(query).scalar_one()
         except NoResultFound:
             abort_msg = (
                 f"The entry with ID {entry_id} does not exist for the current user."
             )
             abort(404, abort_msg)
         return entry
 
+    def entry_saver(method):
+        """
+        A decorator to facilitate saving an entry safely.
+
+        This decorator wraps a function that saves an entry. The entry
+        must always be a normal entry (not a view) for the save
+        operation to succeed, and the saved entry should also be
+        validated to ensure that it belongs to an authorized user. This
+        method performs both functions: it takes the saved entry and
+        queries the database for the up-to-date version, using the
+        handler logic to choose either the entry or the corresponding
+        view; that process implicitly guarantees authorization.
+        """
+        @functools.wraps(method)
+        def wrapper(cls, *args, **kwargs):
+            entry = method(cls, *args, **kwargs)
+            # Return either the entry or its view (implicitly confirming authorizatio)
+            entry_id = getattr(entry, entry.primary_key_field.name)
+            entry = cls.get_entry(entry_id)
+            return entry
+        return wrapper
+
     @classmethod
+    @entry_saver
     def add_entry(cls, **field_values):
         """
         Create a new entry in the database given field values.
 
         Parameters
         ----------
         **field_values :
@@ -309,19 +366,18 @@
         -------
         entry : database.models.Model
             The saved entry.
         """
         entry = cls.model(**field_values)
         cls._db.session.add(entry)
         cls._db.session.flush()
-        # Confirm that this was an authorized entry by the user
-        entry = cls.get_entry(entry.id)
         return entry
 
     @classmethod
+    @entry_saver
     def update_entry(cls, entry_id, **field_values):
         """
         Update an entry in the database given field values.
 
         Accept a mapping relating given inputs to database fields. This
         mapping is used to update an existing entry in the database. All
         fields are sanitized prior to updating.
@@ -334,45 +390,43 @@
             Values for fields to update in the entry.
 
         Returns
         -------
         entry : database.models.Model
             The saved entry.
         """
-        cls._confirm_manipulation_authorization(entry_id)
+        cls._validate_authorization(entry_id)
         entry = cls._db.session.get(cls.model, entry_id)
-        entry_fields = [column.name for column in inspect(cls.model).columns]
+        entry_fields = [column.name for column in cls.model.fields]
         for field, value in field_values.items():
             if field not in entry_fields:
                 raise ValueError(
                     f"A value cannot be updated in the nonexistent field {field}."
                 )
             setattr(entry, field, value)
         cls._db.session.flush()
-        # Confirm that this was an authorized entry by the user
-        entry = cls.get_entry(entry.id)
         return entry
 
     @classmethod
     def delete_entry(cls, entry_id):
         """
         Delete an entry in the database given its ID.
 
         Parameters
         ----------
         entry_id : int
             The ID of the entry to be deleted.
         """
-        cls._confirm_manipulation_authorization(entry_id)
+        cls._validate_authorization(entry_id)
         entry = cls._db.session.get(cls.model, entry_id)
         cls._db.session.delete(entry)
         cls._db.session.flush()
 
     @classmethod
-    def _confirm_manipulation_authorization(cls, entry_id):
+    def _validate_authorization(cls, entry_id):
         # Confirm (via access) that the user may manipulate the entry
         return cls.get_entry(entry_id)
 
 
 class DatabaseViewHandlerMixin(DatabaseHandlerMixin):
     """
     A mixin providing the functionality of a database view handler.
@@ -386,35 +440,40 @@
     """
 
     _view_context = False
 
     def view_query(func):
         """Require that a function use a model view rather than the model."""
 
+        @functools.wraps(func)
         def wrapper(cls, *args, **kwargs):
             orig_view_context = cls._view_context
             cls._view_context = True
             try:
                 return_value = func(cls, *args, **kwargs)
             finally:
                 cls._view_context = orig_view_context
             return return_value
 
         return wrapper
 
     @classmethod
     @view_query
-    def get_entries(cls, criteria=None, sort_order=None):
-        return super().get_entries(criteria=criteria, sort_order=sort_order)
+    def get_entries(cls, entry_ids=None, criteria=None, column_orders=None):
+        return super().get_entries(
+            entry_ids=entry_ids, criteria=criteria, column_orders=column_orders
+        )
 
     @classmethod
     @view_query
-    def find_entry(cls, criteria=None, sort_order=None, require_unique=True):
+    def find_entry(cls, criteria=None, column_orders=None, require_unique=True):
         return super().find_entry(
-            criteria=criteria, sort_order=sort_order, require_unique=require_unique
+            criteria=criteria,
+            column_orders=column_orders,
+            require_unique=require_unique,
         )
 
     @classmethod
     @view_query
     def get_entry(cls, entry_id):
         return super().get_entry(entry_id)
```

### Comparing `authanor-0.1.0/.gitignore` & `authanor-0.2.0/.gitignore`

 * *Files 18% similar despite different names*

```diff
@@ -66,11 +66,11 @@
 # PyBuilder
 target/
 
 # Mac custom attributes file
 .DS_Store
 
 # Virtual environment
-auth-env/
+authanor-env/
 
 # Hatch-generated version file
 authanor/_version.py
```

### Comparing `authanor-0.1.0/COPYING` & `authanor-0.2.0/COPYING`

 * *Files identical despite different names*

### Comparing `authanor-0.1.0/pyproject.toml` & `authanor-0.2.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -9,33 +9,38 @@
 ]
 description = 'A Pythonic SQLALchemy interface to enforce authorization criteria.'
 license = { text = 'GNU GPLv3' }
 requires-python = '>=3.9,<3.11'
 dependencies = [
     'flask>=2.2.2',
     'sqlalchemy>=2.0.0',
+    'sqlalchemy-views>=0.3.2',
 ]
 keywords = [
 ]
 classifiers = [
   'Development Status :: 3 - Alpha',
   'Framework :: Flask',
+  'Framework :: Pytest',
   'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
   'Natural Language :: English',
   'Operating System :: OS Independent',
   'Programming Language :: Python',
 ]
 dynamic = ['readme', 'version']
 
 [project.urls]
 Download = 'https://pypi.org/project/authanor'
 Homepage = 'https://github.com/mitchnegus/authanor'
 Repository = 'https://github.com/mitchnegus/authanor'
 Changelog = 'https://github.com/mitchnegus/authanor/blob/main/CHANGELOG.md'
 
+[project.entry-points.pytest11]
+authanor = "authanor.test.helpers"
+
 [tool.hatch.version]
 source = 'vcs'
 
 [tool.hatch.build.targets.sdist]
 include = [
   '/authanor',
 ]
@@ -56,13 +61,29 @@
 pattern = 'src="((?!https?:\/\/)\S+?)"'
 replacement = 'src="https://raw.githubusercontent.com/mitchnegus/authanor/main/\1"'
 
 [[tool.hatch.metadata.hooks.fancy-pypi-readme.substitutions]]
 pattern = '\[(.+?)\]\(((?!https?://)\S+?)\)'
 replacement = '[\1](https://github.com/mitchnegus/authanor/blob/main/\g<2>)'
 
+[tool.pytest.ini_options]
+addopts = [
+  '--import-mode=importlib',
+]
+
+[tool.coverage.run]
+omit = [
+  'tests/*',
+  'authanor/test/helpers.py',
+]
+
+[tool.coverage.report]
+exclude_lines = [
+  'raise NotImplementedError',
+]
+
 [tool.black]
 force-exclude = 'authanor/_version.py'
 
 [tool.isort]
 profile = 'black'
 src_paths = ['authanor', 'test']
```

### Comparing `authanor-0.1.0/PKG-INFO` & `authanor-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 Metadata-Version: 2.1
 Name: authanor
-Version: 0.1.0
+Version: 0.2.0
 Summary: A Pythonic SQLALchemy interface to enforce authorization criteria.
 Project-URL: Download, https://pypi.org/project/authanor
 Project-URL: Homepage, https://github.com/mitchnegus/authanor
 Project-URL: Repository, https://github.com/mitchnegus/authanor
 Project-URL: Changelog, https://github.com/mitchnegus/authanor/blob/main/CHANGELOG.md
 Author-email: Mitch Negus <mitchnegus57@gmail.com>
 License: GNU GPLv3
 License-File: COPYING
 License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Flask
+Classifier: Framework :: Pytest
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Requires-Python: <3.11,>=3.9
 Requires-Dist: flask>=2.2.2
+Requires-Dist: sqlalchemy-views>=0.3.2
 Requires-Dist: sqlalchemy>=2.0.0
 Description-Content-Type: text/markdown
 
 # Authanor
 
 <img src="https://upload.wikimedia.org/wikipedia/commons/1/10/Athanor.jpg" alt="Athanor" />
 
-A tool providing a a Pythonic interface to SQLAlchemy while enforcing authorization criteria.
+A tool providing a a Pythonic interface to SQLAlchemy while enforcing authorization criteria for Flask.
 
 SQLAlchemy provides a phenomenal interface for querying a database.
 However, this package is designed to enable the construction of handler objects that perform a series of consistent actions on many similar ORM entities.
 For example, it is common to want to select all values in a given table using an ORM, or add an entry to the table based on a mapping.
 These are easy to do using SQLAlchemy, but my experience is that things get a bit more challenging when a query must be limited to a single authorized user (and several joins are required to filter that query).
 
 It's possible I'm missing a key functionality of SQLAlchemy that enables this behavior elegantly, but I haven't found a clean way to do it yet.
```

