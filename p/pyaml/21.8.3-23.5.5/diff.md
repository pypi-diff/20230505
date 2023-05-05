# Comparing `tmp/pyaml-21.8.3.tar.gz` & `tmp/pyaml-23.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyaml-21.8.3.tar", last modified: Sun Aug  8 13:12:20 2021, max compression
+gzip compressed data, was "pyaml-23.5.5.tar", last modified: Fri May  5 00:42:12 2023, max compression
```

## Comparing `pyaml-21.8.3.tar` & `pyaml-23.5.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 fraggod   (1000) fraggod   (1000)        0 2021-08-08 13:12:20.963774 pyaml-21.8.3/
--rw-r--r--   0 fraggod   (1000) fraggod   (1000)      491 2016-11-02 04:21:03.000000 pyaml-21.8.3/COPYING
--rw-r--r--   0 fraggod   (1000) fraggod   (1000)       27 2015-05-19 18:45:16.000000 pyaml-21.8.3/MANIFEST.in
--rw-r--r--   0 fraggod   (1000) fraggod   (1000)    10296 2021-08-08 13:12:20.966774 pyaml-21.8.3/PKG-INFO
--rw-r--r--   0 fraggod   (1000) fraggod   (1000)     9580 2020-03-09 20:21:14.000000 pyaml-21.8.3/README
--rw-r--r--   0 fraggod   (1000) fraggod   (1000)     9580 2020-03-09 20:21:14.000000 pyaml-21.8.3/README.rst
-drwxr-xr-x   0 fraggod   (1000) fraggod   (1000)        0 2021-08-08 13:12:20.962774 pyaml-21.8.3/pyaml/
--rw-r--r--   0 fraggod   (1000) fraggod   (1000)     8088 2020-04-02 09:58:50.000000 pyaml-21.8.3/pyaml/__init__.py
--rw-r--r--   0 fraggod   (1000) fraggod   (1000)     1647 2019-12-07 04:16:01.000000 pyaml-21.8.3/pyaml/__main__.py
-drwxr-xr-x   0 fraggod   (1000) fraggod   (1000)        0 2021-08-08 13:12:20.963774 pyaml-21.8.3/pyaml/tests/
--rw-r--r--   0 fraggod   (1000) fraggod   (1000)        0 2019-04-10 20:23:02.000000 pyaml-21.8.3/pyaml/tests/__init__.py
--rw-r--r--   0 fraggod   (1000) fraggod   (1000)    17498 2021-08-08 13:09:28.000000 pyaml-21.8.3/pyaml/tests/dump.py
-drwxr-xr-x   0 fraggod   (1000) fraggod   (1000)        0 2021-08-08 13:12:20.963774 pyaml-21.8.3/pyaml.egg-info/
--rw-r--r--   0 fraggod   (1000) fraggod   (1000)    10296 2021-08-08 13:12:20.000000 pyaml-21.8.3/pyaml.egg-info/PKG-INFO
--rw-r--r--   0 fraggod   (1000) fraggod   (1000)      280 2021-08-08 13:12:20.000000 pyaml-21.8.3/pyaml.egg-info/SOURCES.txt
--rw-r--r--   0 fraggod   (1000) fraggod   (1000)        1 2021-08-08 13:12:20.000000 pyaml-21.8.3/pyaml.egg-info/dependency_links.txt
--rw-r--r--   0 fraggod   (1000) fraggod   (1000)        7 2021-08-08 13:12:20.000000 pyaml-21.8.3/pyaml.egg-info/requires.txt
--rw-r--r--   0 fraggod   (1000) fraggod   (1000)        6 2021-08-08 13:12:20.000000 pyaml-21.8.3/pyaml.egg-info/top_level.txt
--rw-r--r--   0 fraggod   (1000) fraggod   (1000)       67 2021-08-08 13:12:20.966774 pyaml-21.8.3/setup.cfg
--rw-------   0 fraggod   (1000) fraggod   (1000)     1155 2021-08-08 13:11:46.000000 pyaml-21.8.3/setup.py
+drwxr-xr-x   0 fraggod   (1000) fraggod   (1000)        0 2023-05-05 00:42:12.326240 pyaml-23.5.5/
+-rw-r--r--   0 fraggod   (1000) fraggod   (1000)      491 2016-11-02 04:21:03.000000 pyaml-23.5.5/COPYING
+-rw-r--r--   0 fraggod   (1000) fraggod   (1000)       27 2015-05-19 18:45:16.000000 pyaml-23.5.5/MANIFEST.in
+-rw-r--r--   0 fraggod   (1000) fraggod   (1000)     9618 2023-05-05 00:42:12.326240 pyaml-23.5.5/PKG-INFO
+-rw-r--r--   0 fraggod   (1000) fraggod   (1000)     8914 2023-05-05 00:40:31.000000 pyaml-23.5.5/README.rst
+drwxr-xr-x   0 fraggod   (1000) fraggod   (1000)        0 2023-05-05 00:42:12.326240 pyaml-23.5.5/pyaml/
+-rw-r--r--   0 fraggod   (1000) fraggod   (1000)     7428 2023-05-05 00:29:16.000000 pyaml-23.5.5/pyaml/__init__.py
+-rw-r--r--   0 fraggod   (1000) fraggod   (1000)     2120 2023-05-04 23:33:19.000000 pyaml-23.5.5/pyaml/__main__.py
+drwxr-xr-x   0 fraggod   (1000) fraggod   (1000)        0 2023-05-05 00:42:12.326240 pyaml-23.5.5/pyaml/tests/
+-rw-r--r--   0 fraggod   (1000) fraggod   (1000)        0 2019-04-10 20:23:02.000000 pyaml-23.5.5/pyaml/tests/__init__.py
+-rw-r--r--   0 fraggod   (1000) fraggod   (1000)    16678 2023-05-04 23:58:10.000000 pyaml-23.5.5/pyaml/tests/test_dump.py
+drwxr-xr-x   0 fraggod   (1000) fraggod   (1000)        0 2023-05-05 00:42:12.326240 pyaml-23.5.5/pyaml.egg-info/
+-rw-r--r--   0 fraggod   (1000) fraggod   (1000)     9618 2023-05-05 00:42:12.000000 pyaml-23.5.5/pyaml.egg-info/PKG-INFO
+-rw-r--r--   0 fraggod   (1000) fraggod   (1000)      283 2023-05-05 00:42:12.000000 pyaml-23.5.5/pyaml.egg-info/SOURCES.txt
+-rw-r--r--   0 fraggod   (1000) fraggod   (1000)        1 2023-05-05 00:42:12.000000 pyaml-23.5.5/pyaml.egg-info/dependency_links.txt
+-rw-r--r--   0 fraggod   (1000) fraggod   (1000)       28 2023-05-05 00:42:12.000000 pyaml-23.5.5/pyaml.egg-info/requires.txt
+-rw-r--r--   0 fraggod   (1000) fraggod   (1000)        6 2023-05-05 00:42:12.000000 pyaml-23.5.5/pyaml.egg-info/top_level.txt
+-rw-r--r--   0 fraggod   (1000) fraggod   (1000)      805 2023-05-05 00:41:09.000000 pyaml-23.5.5/pyproject.toml
+-rw-r--r--   0 fraggod   (1000) fraggod   (1000)       38 2023-05-05 00:42:12.326240 pyaml-23.5.5/setup.cfg
+-rw-r--r--   0 fraggod   (1000) fraggod   (1000)       96 2023-05-05 00:23:33.000000 pyaml-23.5.5/setup.py
```

### Comparing `pyaml-21.8.3/PKG-INFO` & `pyaml-23.5.5/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,65 +1,73 @@
 Metadata-Version: 2.1
 Name: pyaml
-Version: 21.8.3
-Summary: PyYAML-based module to produce pretty and readable YAML-serialized data
-Home-page: https://github.com/mk-fg/pretty-yaml
-Author: Mike Kazantsev
-Author-email: mk.fraggod@gmail.com
+Version: 23.5.5
+Summary: PyYAML-based module to produce a bit more pretty and readable YAML-serialized data
+Author-email: Mike Kazantsev <mk.fraggod@gmail.com>
 License: WTFPL
-Keywords: yaml serialization pretty print format human readable readability
-Platform: UNKNOWN
+Keywords: yaml,serialization,pretty-print,formatter,human,readability
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
+Classifier: License :: Public Domain
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-License-File: COPYING
+Classifier: Topic :: Utilities
+Description-Content-Type: text/x-rst
+Provides-Extra: anchors
 
 pretty-yaml (or pyaml)
 ======================
 
-PyYAML-based python module to produce pretty and readable YAML-serialized data.
+PyYAML_-based python module to produce a bit more pretty and human-readable YAML-serialized data.
 
 This module is for serialization only, see `ruamel.yaml`_ module for literate
 YAML parsing (keeping track of comments, spacing, line/column numbers of values, etc).
 
-[note: to dump stuff parsed by ruamel.yaml with this module, use only ``YAML(typ='safe')`` there]
+[side-note: to dump stuff parsed by ruamel.yaml with this module, use only ``YAML(typ='safe')``]
+
+.. _PyYAML: http://pyyaml.org/
+.. _ruamel.yaml: https://bitbucket.org/ruamel/yaml/
 
 .. contents::
   :backlinks: none
 
+Repository URLs:
+
+- https://github.com/mk-fg/pretty-yaml
+- https://codeberg.org/mk-fg/pretty-yaml
+- https://fraggod.net/code/git/pretty-yaml
+
 
 Warning
 -------
 
 Prime goal of this module is to produce human-readable output that can be easily
 manipulated and re-used, but maybe with some occasional caveats.
 
-One good example of such "caveat" is that e.g. ``{'foo': '123'}`` will serialize
+One good example of such "caveat" is that e.g. ``{'foo': '123'}`` might serialize
 to ``foo: 123``, which for PyYAML would be a bug, as 123 will then be read back
 as an integer from that, but here it's a feature.
 
 So please do not rely on the thing to produce output that can always be
-deserialized exactly to what was exported, at least - use PyYAML (e.g. with
-options from the next section) for that.
+deserialized exactly to what was exported, at least - use PyYAML directly
+for that (but maybe with options from the next section).
 
 
 What this module does and why
 -----------------------------
 
 YAML is generally nice and easy format to read *if* it was written by humans.
 
 PyYAML can a do fairly decent job of making stuff readable, and the best
 combination of parameters for such output that I've seen so far is probably this one::
 
-  >>> m = [123, 45.67, {1: None, 2: False}, u'some text']
-  >>> data = dict(a=u'asldnsa\nasldpáknsa\n', b=u'whatever text', ma=m, mb=m)
+  >>> m = [123, 45.67, {1: None, 2: False}, 'some text']
+  >>> data = dict(a='asldnsa\nasldpáknsa\n', b='whatever text', ma=m, mb=m)
   >>> yaml.safe_dump(data, sys.stdout, allow_unicode=True, default_flow_style=False)
   a: 'asldnsa
 
     asldpáknsa
 
     '
   b: whatever text
@@ -67,36 +75,29 @@
   - 123
   - 45.67
   - 1: null
     2: false
   - some text
   mb: *id001
 
-pyaml tries to improve on that a bit, with the following tweaks:
+pyaml (this module) tries to improve on that a bit, with the following tweaks:
 
-* Most human-friendly representation options in PyYAML (that I know of) get
-  picked as defaults.
+* Most human-friendly representation options in PyYAML (that I know of)
+  are used as defaults.
 
-* Does not dump "null" values, if possible, replacing these with just empty
-  strings, which have the same meaning but reduce visual clutter and are easier
-  to edit.
+* Dump "null" values as empty values, if possible, which have the same meaning
+  but reduce visual clutter and are easier to edit.
 
-* Dicts, sets, OrderedDicts, defaultdicts, namedtuples, etc are representable
-  and get sorted on output (OrderedDicts and namedtuples keep their ordering),
-  so that output would be as diff-friendly as possible, and not arbitrarily
-  depend on python internals.
+* Use shorter and simplier yes/no for booleans.
 
-  It appears that at least recent PyYAML versions also do such sorting for
-  python dicts.
+* Dicts, sets, OrderedDicts, defaultdicts, namedtuples, etc are representable
+  and key-sorted by default, for more diff-friendly output.
 
 * List items get indented, as they should be.
 
-* bytestrings that can't be auto-converted to unicode raise error, as yaml has
-  no "binary bytes" (i.e. unix strings) type.
-
 * Attempt is made to pick more readable string representation styles, depending
   on the value, e.g.::
 
     >>> yaml.safe_dump(cert, sys.stdout)
     cert: '-----BEGIN CERTIFICATE-----
 
       MIIH3jCCBcagAwIBAgIJAJi7AjQ4Z87OMA0GCSqGSIb3DQEBCwUAMIHBMRcwFQYD
@@ -107,95 +108,92 @@
     >>> pyaml.p(cert):
     cert: |
       -----BEGIN CERTIFICATE-----
       MIIH3jCCBcagAwIBAgIJAJi7AjQ4Z87OMA0GCSqGSIb3DQEBCwUAMIHBMRcwFQYD
       VQQKFA52YWxlcm9uLm5vX2lzcDEeMBwGA1UECxMVQ2VydGlmaWNhdGUgQXV0aG9y
     ...
 
-* "force_embed" option to avoid having &id stuff scattered all over the output
-  (which might be beneficial in some cases, hence the option).
+* "force_embed" option (default=yes) to avoid having &id stuff scattered all
+  over the output. Might be more useful to disable it in some specific cases though.
 
 * "&id" anchors, if used, get labels from the keys they get attached to,
-  not just use meaningless enumerators.
+  not just meaningless enumerators.
 
 * "string_val_style" option to only apply to strings that are values, not keys,
   i.e::
 
     >>> pyaml.p(data, string_val_style='"')
     key: "value\nasldpáknsa\n"
     >>> yaml.safe_dump(data, sys.stdout, allow_unicode=True, default_style='"')
     "key": "value\nasldpáknsa\n"
 
-* "sort_dicts=False" option to leave dict item ordering to python, and not
-  force-sort them in yaml output, which can be important for python 3.6+ where
-  they retain ordering info.
+* Add vertical spacing (empty lines) between keys on different depths,
+  to separate long YAML sections in the output visually, make it more seekable.
 
-* Has an option to add vertical spacing (empty lines) between keys on different
-  depths, to make output much more seekable.
+Result for the (rather meaningless) example above::
 
-Result for the (rather meaningless) example above (without any additional
-tweaks)::
+  >>> pyaml.p(data, force_embed=False, vspacing=dict(split_lines=10))
 
-  >>> pyaml.p(data)
   a: |
     asldnsa
     asldpáknsa
-  b: 'whatever text'
+
+  b: whatever text
+
   ma: &ma
     - 123
     - 45.67
     - 1:
-      2: false
-    - 'some text'
+      2: no
+    - some text
+
   mb: *ma
 
+(force_embed enabled deduplication with ``&ma`` anchor,
+vspacing is adjusted to split even this tiny output)
+
 ----------
 
 Extended example::
 
-  >>> pyaml.dump(conf, sys.stdout, vspacing=[2, 1]):
+  >>> pyaml.dump(data, vspacing=dict(split_lines=10))
+
   destination:
 
     encoding:
       xz:
-        enabled: true
+        enabled: yes
         min_size: 5120
         options:
         path_filter:
           - \.(gz|bz2|t[gb]z2?|xz|lzma|7z|zip|rar)$
           - \.(rpm|deb|iso)$
           - \.(jpe?g|gif|png|mov|avi|ogg|mkv|webm|mp[34g]|flv|flac|ape|pdf|djvu)$
           - \.(sqlite3?|fossil|fsl)$
           - \.git/objects/[0-9a-f]+/[0-9a-f]+$
 
     result:
       append_to_file:
       append_to_lafs_dir:
-      print_to_stdout: true
+      print_to_stdout: yes
 
     url: http://localhost:3456/uri
 
-
   filter:
     - /(CVS|RCS|SCCS|_darcs|\{arch\})/$
     - /\.(git|hg|bzr|svn|cvs)(/|ignore|attributes|tags)?$
     - /=(RELEASE-ID|meta-update|update)$
 
-
   http:
-
     ca_certs_files: /etc/ssl/certs/ca-certificates.crt
-
-    debug_requests: false
-
+    debug_requests: no
     request_pool_options:
       cachedConnectionTimeout: 600
       maxPersistentPerHost: 10
-      retryAutomatically: true
-
+      retryAutomatically: yes
 
   logging:
 
     formatters:
       basic:
         datefmt: '%Y-%m-%d %H:%M:%S'
         format: '%(asctime)s :: %(name)s :: %(levelname)s: %(message)s'
@@ -232,24 +230,22 @@
     % python -m pyaml /path/to/some/file.yaml
     % curl -s https://www.githubstatus.com/api/v2/summary.json | python -m pyaml
 
 * Process and replace json/yaml file in-place::
 
     % python -m pyaml -r file-with-json.data
 
-* Easier "debug printf" for more complex data (all funcs below are aliases to
-  same thing)::
+* Easier "debug printf" for more complex data (all funcs below are aliases to same thing)::
 
     pyaml.p(stuff)
     pyaml.pprint(my_data)
     pyaml.pprint('----- HOW DOES THAT BREAKS!?!?', input_data, some_var, more_stuff)
     pyaml.print(data, file=sys.stderr) # needs "from __future__ import print_function"
 
-* Force all string values to a certain style (see info on these in
-  `PyYAML docs`_)::
+* Force all string values to a certain style (see info on these in `PyYAML docs`_)::
 
     pyaml.dump(many_weird_strings, string_val_style='|')
     pyaml.dump(multiline_words, string_val_style='>')
     pyaml.dump(no_want_quotes, string_val_style='plain')
 
   Using ``pyaml.add_representer()`` (note \*p\*yaml) as suggested in
   `this SO thread`_ (or `github-issue-7`_) should also work.
@@ -269,69 +265,45 @@
 .. _this SO thread: http://stackoverflow.com/a/7445560
 .. _github-issue-7: https://github.com/mk-fg/pretty-yaml/issues/7
 
 
 Installation
 ------------
 
-It's a regular package for Python (3.x or 2.x).
-
-Module uses PyYAML_ for processing of the actual YAML files and should pull it
-in as a dependency.
-
-Dependency on unidecode_ module is optional and should only be necessary if
-same-id objects or recursion is used within serialized data.
-
-Be sure to use python3/python2, pip3/pip2, easy_install-... binaries below,
-based on which python version you want to install the module for, if you have
-several on the system (as is norm these days for py2-py3 transition).
-
-Using pip_ is the best way::
+It's a regular python module/package, published on PyPI (as pyaml_).
 
-  % pip install pyaml
-
-(add --user option to install into $HOME for current user only)
-
-Or, if you don't have "pip" command::
+Module uses PyYAML_ for processing of the actual YAML files
+and should pull it in as a dependency.
 
-  % python -m ensurepip
-  % python -m pip install --upgrade pip
-  % python -m pip install pyaml
+Dependency on unidecode_ module is optional and should only be necessary
+with force_embed=False keyword, and same-id objects or recursion is used
+within serialized data.
 
-(same suggestion wrt "install --user" as above)
+Using pip_ is how you generally install it, usually coupled with venv_ usage
+(which will also provide "pip" tool itself)::
 
-On a very old systems, one of these might work::
-
-  % curl https://bootstrap.pypa.io/get-pip.py | python
   % pip install pyaml
 
-  % easy_install pyaml
-
-  % git clone --depth=1 https://github.com/mk-fg/pretty-yaml
-  % cd pretty-yaml
-  % python setup.py install
-
-(all of install-commands here also have --user option,
-see also `pip docs "installing" section`_)
-
 Current-git version can be installed like this::
 
-  % pip install 'git+https://github.com/mk-fg/pretty-yaml#egg=pyaml'
-
-Note that to install stuff to system-wide PATH and site-packages (without
---user), elevated privileges (i.e. root and su/sudo) are often required.
-
-Use "...install --user", `~/.pydistutils.cfg`_ or virtualenv_ to do unprivileged
-installs into custom paths.
-
-More info on python packaging can be found at `packaging.python.org`_.
+  % pip install 'git+https://github.com/mk-fg/pretty-yaml'
 
-.. _ruamel.yaml: https://bitbucket.org/ruamel/yaml/
-.. _PyYAML: http://pyyaml.org/
-.. _unidecode: http://pypi.python.org/pypi/Unidecode
-.. _pip: http://pip-installer.org/
-.. _pip docs "installing" section: http://www.pip-installer.org/en/latest/installing.html
-.. _~/.pydistutils.cfg: http://docs.python.org/install/index.html#distutils-configuration-files
-.. _virtualenv: http://pypi.python.org/pypi/virtualenv
+pip will default to installing into currently-active venv, then user's home
+directory (under ``~/.local/lib/python...``), and maybe system-wide when running
+as root (only useful in specialized environments like docker containers).
+
+There are many other python packaging tools - pipenv_, poetry_, pdm_, etc -
+use whatever is most suitable for specific project/environment.
+
+More general info on python packaging can be found at `packaging.python.org`_.
+
+When changing code, unit tests can be run with ``python -m unittest discover``
+from the local repository checkout.
+
+.. _pyaml: https://pypi.org/project/pyaml/
+.. _unidecode: https://pypi.python.org/pypi/Unidecode
+.. _pip: https://pip.pypa.io/en/stable/
+.. _venv: https://docs.python.org/3/library/venv.html
+.. _poetry: https://python-poetry.org/
+.. _pipenv: https://pipenv.pypa.io/
+.. _pdm: https://pdm.fming.dev/
 .. _packaging.python.org: https://packaging.python.org/installing/
-
-
```

### Comparing `pyaml-21.8.3/README` & `pyaml-23.5.5/README.rst`

 * *Files 9% similar despite different names*

```diff
@@ -1,46 +1,55 @@
 pretty-yaml (or pyaml)
 ======================
 
-PyYAML-based python module to produce pretty and readable YAML-serialized data.
+PyYAML_-based python module to produce a bit more pretty and human-readable YAML-serialized data.
 
 This module is for serialization only, see `ruamel.yaml`_ module for literate
 YAML parsing (keeping track of comments, spacing, line/column numbers of values, etc).
 
-[note: to dump stuff parsed by ruamel.yaml with this module, use only ``YAML(typ='safe')`` there]
+[side-note: to dump stuff parsed by ruamel.yaml with this module, use only ``YAML(typ='safe')``]
+
+.. _PyYAML: http://pyyaml.org/
+.. _ruamel.yaml: https://bitbucket.org/ruamel/yaml/
 
 .. contents::
   :backlinks: none
 
+Repository URLs:
+
+- https://github.com/mk-fg/pretty-yaml
+- https://codeberg.org/mk-fg/pretty-yaml
+- https://fraggod.net/code/git/pretty-yaml
+
 
 Warning
 -------
 
 Prime goal of this module is to produce human-readable output that can be easily
 manipulated and re-used, but maybe with some occasional caveats.
 
-One good example of such "caveat" is that e.g. ``{'foo': '123'}`` will serialize
+One good example of such "caveat" is that e.g. ``{'foo': '123'}`` might serialize
 to ``foo: 123``, which for PyYAML would be a bug, as 123 will then be read back
 as an integer from that, but here it's a feature.
 
 So please do not rely on the thing to produce output that can always be
-deserialized exactly to what was exported, at least - use PyYAML (e.g. with
-options from the next section) for that.
+deserialized exactly to what was exported, at least - use PyYAML directly
+for that (but maybe with options from the next section).
 
 
 What this module does and why
 -----------------------------
 
 YAML is generally nice and easy format to read *if* it was written by humans.
 
 PyYAML can a do fairly decent job of making stuff readable, and the best
 combination of parameters for such output that I've seen so far is probably this one::
 
-  >>> m = [123, 45.67, {1: None, 2: False}, u'some text']
-  >>> data = dict(a=u'asldnsa\nasldpáknsa\n', b=u'whatever text', ma=m, mb=m)
+  >>> m = [123, 45.67, {1: None, 2: False}, 'some text']
+  >>> data = dict(a='asldnsa\nasldpáknsa\n', b='whatever text', ma=m, mb=m)
   >>> yaml.safe_dump(data, sys.stdout, allow_unicode=True, default_flow_style=False)
   a: 'asldnsa
 
     asldpáknsa
 
     '
   b: whatever text
@@ -48,36 +57,29 @@
   - 123
   - 45.67
   - 1: null
     2: false
   - some text
   mb: *id001
 
-pyaml tries to improve on that a bit, with the following tweaks:
+pyaml (this module) tries to improve on that a bit, with the following tweaks:
 
-* Most human-friendly representation options in PyYAML (that I know of) get
-  picked as defaults.
+* Most human-friendly representation options in PyYAML (that I know of)
+  are used as defaults.
 
-* Does not dump "null" values, if possible, replacing these with just empty
-  strings, which have the same meaning but reduce visual clutter and are easier
-  to edit.
+* Dump "null" values as empty values, if possible, which have the same meaning
+  but reduce visual clutter and are easier to edit.
 
-* Dicts, sets, OrderedDicts, defaultdicts, namedtuples, etc are representable
-  and get sorted on output (OrderedDicts and namedtuples keep their ordering),
-  so that output would be as diff-friendly as possible, and not arbitrarily
-  depend on python internals.
+* Use shorter and simplier yes/no for booleans.
 
-  It appears that at least recent PyYAML versions also do such sorting for
-  python dicts.
+* Dicts, sets, OrderedDicts, defaultdicts, namedtuples, etc are representable
+  and key-sorted by default, for more diff-friendly output.
 
 * List items get indented, as they should be.
 
-* bytestrings that can't be auto-converted to unicode raise error, as yaml has
-  no "binary bytes" (i.e. unix strings) type.
-
 * Attempt is made to pick more readable string representation styles, depending
   on the value, e.g.::
 
     >>> yaml.safe_dump(cert, sys.stdout)
     cert: '-----BEGIN CERTIFICATE-----
 
       MIIH3jCCBcagAwIBAgIJAJi7AjQ4Z87OMA0GCSqGSIb3DQEBCwUAMIHBMRcwFQYD
@@ -88,95 +90,92 @@
     >>> pyaml.p(cert):
     cert: |
       -----BEGIN CERTIFICATE-----
       MIIH3jCCBcagAwIBAgIJAJi7AjQ4Z87OMA0GCSqGSIb3DQEBCwUAMIHBMRcwFQYD
       VQQKFA52YWxlcm9uLm5vX2lzcDEeMBwGA1UECxMVQ2VydGlmaWNhdGUgQXV0aG9y
     ...
 
-* "force_embed" option to avoid having &id stuff scattered all over the output
-  (which might be beneficial in some cases, hence the option).
+* "force_embed" option (default=yes) to avoid having &id stuff scattered all
+  over the output. Might be more useful to disable it in some specific cases though.
 
 * "&id" anchors, if used, get labels from the keys they get attached to,
-  not just use meaningless enumerators.
+  not just meaningless enumerators.
 
 * "string_val_style" option to only apply to strings that are values, not keys,
   i.e::
 
     >>> pyaml.p(data, string_val_style='"')
     key: "value\nasldpáknsa\n"
     >>> yaml.safe_dump(data, sys.stdout, allow_unicode=True, default_style='"')
     "key": "value\nasldpáknsa\n"
 
-* "sort_dicts=False" option to leave dict item ordering to python, and not
-  force-sort them in yaml output, which can be important for python 3.6+ where
-  they retain ordering info.
+* Add vertical spacing (empty lines) between keys on different depths,
+  to separate long YAML sections in the output visually, make it more seekable.
 
-* Has an option to add vertical spacing (empty lines) between keys on different
-  depths, to make output much more seekable.
+Result for the (rather meaningless) example above::
 
-Result for the (rather meaningless) example above (without any additional
-tweaks)::
+  >>> pyaml.p(data, force_embed=False, vspacing=dict(split_lines=10))
 
-  >>> pyaml.p(data)
   a: |
     asldnsa
     asldpáknsa
-  b: 'whatever text'
+
+  b: whatever text
+
   ma: &ma
     - 123
     - 45.67
     - 1:
-      2: false
-    - 'some text'
+      2: no
+    - some text
+
   mb: *ma
 
+(force_embed enabled deduplication with ``&ma`` anchor,
+vspacing is adjusted to split even this tiny output)
+
 ----------
 
 Extended example::
 
-  >>> pyaml.dump(conf, sys.stdout, vspacing=[2, 1]):
+  >>> pyaml.dump(data, vspacing=dict(split_lines=10))
+
   destination:
 
     encoding:
       xz:
-        enabled: true
+        enabled: yes
         min_size: 5120
         options:
         path_filter:
           - \.(gz|bz2|t[gb]z2?|xz|lzma|7z|zip|rar)$
           - \.(rpm|deb|iso)$
           - \.(jpe?g|gif|png|mov|avi|ogg|mkv|webm|mp[34g]|flv|flac|ape|pdf|djvu)$
           - \.(sqlite3?|fossil|fsl)$
           - \.git/objects/[0-9a-f]+/[0-9a-f]+$
 
     result:
       append_to_file:
       append_to_lafs_dir:
-      print_to_stdout: true
+      print_to_stdout: yes
 
     url: http://localhost:3456/uri
 
-
   filter:
     - /(CVS|RCS|SCCS|_darcs|\{arch\})/$
     - /\.(git|hg|bzr|svn|cvs)(/|ignore|attributes|tags)?$
     - /=(RELEASE-ID|meta-update|update)$
 
-
   http:
-
     ca_certs_files: /etc/ssl/certs/ca-certificates.crt
-
-    debug_requests: false
-
+    debug_requests: no
     request_pool_options:
       cachedConnectionTimeout: 600
       maxPersistentPerHost: 10
-      retryAutomatically: true
-
+      retryAutomatically: yes
 
   logging:
 
     formatters:
       basic:
         datefmt: '%Y-%m-%d %H:%M:%S'
         format: '%(asctime)s :: %(name)s :: %(levelname)s: %(message)s'
@@ -213,24 +212,22 @@
     % python -m pyaml /path/to/some/file.yaml
     % curl -s https://www.githubstatus.com/api/v2/summary.json | python -m pyaml
 
 * Process and replace json/yaml file in-place::
 
     % python -m pyaml -r file-with-json.data
 
-* Easier "debug printf" for more complex data (all funcs below are aliases to
-  same thing)::
+* Easier "debug printf" for more complex data (all funcs below are aliases to same thing)::
 
     pyaml.p(stuff)
     pyaml.pprint(my_data)
     pyaml.pprint('----- HOW DOES THAT BREAKS!?!?', input_data, some_var, more_stuff)
     pyaml.print(data, file=sys.stderr) # needs "from __future__ import print_function"
 
-* Force all string values to a certain style (see info on these in
-  `PyYAML docs`_)::
+* Force all string values to a certain style (see info on these in `PyYAML docs`_)::
 
     pyaml.dump(many_weird_strings, string_val_style='|')
     pyaml.dump(multiline_words, string_val_style='>')
     pyaml.dump(no_want_quotes, string_val_style='plain')
 
   Using ``pyaml.add_representer()`` (note \*p\*yaml) as suggested in
   `this SO thread`_ (or `github-issue-7`_) should also work.
@@ -250,67 +247,45 @@
 .. _this SO thread: http://stackoverflow.com/a/7445560
 .. _github-issue-7: https://github.com/mk-fg/pretty-yaml/issues/7
 
 
 Installation
 ------------
 
-It's a regular package for Python (3.x or 2.x).
-
-Module uses PyYAML_ for processing of the actual YAML files and should pull it
-in as a dependency.
-
-Dependency on unidecode_ module is optional and should only be necessary if
-same-id objects or recursion is used within serialized data.
-
-Be sure to use python3/python2, pip3/pip2, easy_install-... binaries below,
-based on which python version you want to install the module for, if you have
-several on the system (as is norm these days for py2-py3 transition).
-
-Using pip_ is the best way::
-
-  % pip install pyaml
-
-(add --user option to install into $HOME for current user only)
+It's a regular python module/package, published on PyPI (as pyaml_).
 
-Or, if you don't have "pip" command::
+Module uses PyYAML_ for processing of the actual YAML files
+and should pull it in as a dependency.
 
-  % python -m ensurepip
-  % python -m pip install --upgrade pip
-  % python -m pip install pyaml
+Dependency on unidecode_ module is optional and should only be necessary
+with force_embed=False keyword, and same-id objects or recursion is used
+within serialized data.
 
-(same suggestion wrt "install --user" as above)
+Using pip_ is how you generally install it, usually coupled with venv_ usage
+(which will also provide "pip" tool itself)::
 
-On a very old systems, one of these might work::
-
-  % curl https://bootstrap.pypa.io/get-pip.py | python
   % pip install pyaml
 
-  % easy_install pyaml
-
-  % git clone --depth=1 https://github.com/mk-fg/pretty-yaml
-  % cd pretty-yaml
-  % python setup.py install
-
-(all of install-commands here also have --user option,
-see also `pip docs "installing" section`_)
-
 Current-git version can be installed like this::
 
-  % pip install 'git+https://github.com/mk-fg/pretty-yaml#egg=pyaml'
-
-Note that to install stuff to system-wide PATH and site-packages (without
---user), elevated privileges (i.e. root and su/sudo) are often required.
+  % pip install 'git+https://github.com/mk-fg/pretty-yaml'
 
-Use "...install --user", `~/.pydistutils.cfg`_ or virtualenv_ to do unprivileged
-installs into custom paths.
-
-More info on python packaging can be found at `packaging.python.org`_.
-
-.. _ruamel.yaml: https://bitbucket.org/ruamel/yaml/
-.. _PyYAML: http://pyyaml.org/
-.. _unidecode: http://pypi.python.org/pypi/Unidecode
-.. _pip: http://pip-installer.org/
-.. _pip docs "installing" section: http://www.pip-installer.org/en/latest/installing.html
-.. _~/.pydistutils.cfg: http://docs.python.org/install/index.html#distutils-configuration-files
-.. _virtualenv: http://pypi.python.org/pypi/virtualenv
+pip will default to installing into currently-active venv, then user's home
+directory (under ``~/.local/lib/python...``), and maybe system-wide when running
+as root (only useful in specialized environments like docker containers).
+
+There are many other python packaging tools - pipenv_, poetry_, pdm_, etc -
+use whatever is most suitable for specific project/environment.
+
+More general info on python packaging can be found at `packaging.python.org`_.
+
+When changing code, unit tests can be run with ``python -m unittest discover``
+from the local repository checkout.
+
+.. _pyaml: https://pypi.org/project/pyaml/
+.. _unidecode: https://pypi.python.org/pypi/Unidecode
+.. _pip: https://pip.pypa.io/en/stable/
+.. _venv: https://docs.python.org/3/library/venv.html
+.. _poetry: https://python-poetry.org/
+.. _pipenv: https://pipenv.pypa.io/
+.. _pdm: https://pdm.fming.dev/
 .. _packaging.python.org: https://packaging.python.org/installing/
```

### Comparing `pyaml-21.8.3/README.rst` & `pyaml-23.5.5/pyaml.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,46 +1,73 @@
+Metadata-Version: 2.1
+Name: pyaml
+Version: 23.5.5
+Summary: PyYAML-based module to produce a bit more pretty and readable YAML-serialized data
+Author-email: Mike Kazantsev <mk.fraggod@gmail.com>
+License: WTFPL
+Keywords: yaml,serialization,pretty-print,formatter,human,readability
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: License :: Public Domain
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Topic :: Software Development
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Utilities
+Description-Content-Type: text/x-rst
+Provides-Extra: anchors
+
 pretty-yaml (or pyaml)
 ======================
 
-PyYAML-based python module to produce pretty and readable YAML-serialized data.
+PyYAML_-based python module to produce a bit more pretty and human-readable YAML-serialized data.
 
 This module is for serialization only, see `ruamel.yaml`_ module for literate
 YAML parsing (keeping track of comments, spacing, line/column numbers of values, etc).
 
-[note: to dump stuff parsed by ruamel.yaml with this module, use only ``YAML(typ='safe')`` there]
+[side-note: to dump stuff parsed by ruamel.yaml with this module, use only ``YAML(typ='safe')``]
+
+.. _PyYAML: http://pyyaml.org/
+.. _ruamel.yaml: https://bitbucket.org/ruamel/yaml/
 
 .. contents::
   :backlinks: none
 
+Repository URLs:
+
+- https://github.com/mk-fg/pretty-yaml
+- https://codeberg.org/mk-fg/pretty-yaml
+- https://fraggod.net/code/git/pretty-yaml
+
 
 Warning
 -------
 
 Prime goal of this module is to produce human-readable output that can be easily
 manipulated and re-used, but maybe with some occasional caveats.
 
-One good example of such "caveat" is that e.g. ``{'foo': '123'}`` will serialize
+One good example of such "caveat" is that e.g. ``{'foo': '123'}`` might serialize
 to ``foo: 123``, which for PyYAML would be a bug, as 123 will then be read back
 as an integer from that, but here it's a feature.
 
 So please do not rely on the thing to produce output that can always be
-deserialized exactly to what was exported, at least - use PyYAML (e.g. with
-options from the next section) for that.
+deserialized exactly to what was exported, at least - use PyYAML directly
+for that (but maybe with options from the next section).
 
 
 What this module does and why
 -----------------------------
 
 YAML is generally nice and easy format to read *if* it was written by humans.
 
 PyYAML can a do fairly decent job of making stuff readable, and the best
 combination of parameters for such output that I've seen so far is probably this one::
 
-  >>> m = [123, 45.67, {1: None, 2: False}, u'some text']
-  >>> data = dict(a=u'asldnsa\nasldpáknsa\n', b=u'whatever text', ma=m, mb=m)
+  >>> m = [123, 45.67, {1: None, 2: False}, 'some text']
+  >>> data = dict(a='asldnsa\nasldpáknsa\n', b='whatever text', ma=m, mb=m)
   >>> yaml.safe_dump(data, sys.stdout, allow_unicode=True, default_flow_style=False)
   a: 'asldnsa
 
     asldpáknsa
 
     '
   b: whatever text
@@ -48,36 +75,29 @@
   - 123
   - 45.67
   - 1: null
     2: false
   - some text
   mb: *id001
 
-pyaml tries to improve on that a bit, with the following tweaks:
+pyaml (this module) tries to improve on that a bit, with the following tweaks:
 
-* Most human-friendly representation options in PyYAML (that I know of) get
-  picked as defaults.
+* Most human-friendly representation options in PyYAML (that I know of)
+  are used as defaults.
 
-* Does not dump "null" values, if possible, replacing these with just empty
-  strings, which have the same meaning but reduce visual clutter and are easier
-  to edit.
+* Dump "null" values as empty values, if possible, which have the same meaning
+  but reduce visual clutter and are easier to edit.
 
-* Dicts, sets, OrderedDicts, defaultdicts, namedtuples, etc are representable
-  and get sorted on output (OrderedDicts and namedtuples keep their ordering),
-  so that output would be as diff-friendly as possible, and not arbitrarily
-  depend on python internals.
+* Use shorter and simplier yes/no for booleans.
 
-  It appears that at least recent PyYAML versions also do such sorting for
-  python dicts.
+* Dicts, sets, OrderedDicts, defaultdicts, namedtuples, etc are representable
+  and key-sorted by default, for more diff-friendly output.
 
 * List items get indented, as they should be.
 
-* bytestrings that can't be auto-converted to unicode raise error, as yaml has
-  no "binary bytes" (i.e. unix strings) type.
-
 * Attempt is made to pick more readable string representation styles, depending
   on the value, e.g.::
 
     >>> yaml.safe_dump(cert, sys.stdout)
     cert: '-----BEGIN CERTIFICATE-----
 
       MIIH3jCCBcagAwIBAgIJAJi7AjQ4Z87OMA0GCSqGSIb3DQEBCwUAMIHBMRcwFQYD
@@ -88,95 +108,92 @@
     >>> pyaml.p(cert):
     cert: |
       -----BEGIN CERTIFICATE-----
       MIIH3jCCBcagAwIBAgIJAJi7AjQ4Z87OMA0GCSqGSIb3DQEBCwUAMIHBMRcwFQYD
       VQQKFA52YWxlcm9uLm5vX2lzcDEeMBwGA1UECxMVQ2VydGlmaWNhdGUgQXV0aG9y
     ...
 
-* "force_embed" option to avoid having &id stuff scattered all over the output
-  (which might be beneficial in some cases, hence the option).
+* "force_embed" option (default=yes) to avoid having &id stuff scattered all
+  over the output. Might be more useful to disable it in some specific cases though.
 
 * "&id" anchors, if used, get labels from the keys they get attached to,
-  not just use meaningless enumerators.
+  not just meaningless enumerators.
 
 * "string_val_style" option to only apply to strings that are values, not keys,
   i.e::
 
     >>> pyaml.p(data, string_val_style='"')
     key: "value\nasldpáknsa\n"
     >>> yaml.safe_dump(data, sys.stdout, allow_unicode=True, default_style='"')
     "key": "value\nasldpáknsa\n"
 
-* "sort_dicts=False" option to leave dict item ordering to python, and not
-  force-sort them in yaml output, which can be important for python 3.6+ where
-  they retain ordering info.
+* Add vertical spacing (empty lines) between keys on different depths,
+  to separate long YAML sections in the output visually, make it more seekable.
 
-* Has an option to add vertical spacing (empty lines) between keys on different
-  depths, to make output much more seekable.
+Result for the (rather meaningless) example above::
 
-Result for the (rather meaningless) example above (without any additional
-tweaks)::
+  >>> pyaml.p(data, force_embed=False, vspacing=dict(split_lines=10))
 
-  >>> pyaml.p(data)
   a: |
     asldnsa
     asldpáknsa
-  b: 'whatever text'
+
+  b: whatever text
+
   ma: &ma
     - 123
     - 45.67
     - 1:
-      2: false
-    - 'some text'
+      2: no
+    - some text
+
   mb: *ma
 
+(force_embed enabled deduplication with ``&ma`` anchor,
+vspacing is adjusted to split even this tiny output)
+
 ----------
 
 Extended example::
 
-  >>> pyaml.dump(conf, sys.stdout, vspacing=[2, 1]):
+  >>> pyaml.dump(data, vspacing=dict(split_lines=10))
+
   destination:
 
     encoding:
       xz:
-        enabled: true
+        enabled: yes
         min_size: 5120
         options:
         path_filter:
           - \.(gz|bz2|t[gb]z2?|xz|lzma|7z|zip|rar)$
           - \.(rpm|deb|iso)$
           - \.(jpe?g|gif|png|mov|avi|ogg|mkv|webm|mp[34g]|flv|flac|ape|pdf|djvu)$
           - \.(sqlite3?|fossil|fsl)$
           - \.git/objects/[0-9a-f]+/[0-9a-f]+$
 
     result:
       append_to_file:
       append_to_lafs_dir:
-      print_to_stdout: true
+      print_to_stdout: yes
 
     url: http://localhost:3456/uri
 
-
   filter:
     - /(CVS|RCS|SCCS|_darcs|\{arch\})/$
     - /\.(git|hg|bzr|svn|cvs)(/|ignore|attributes|tags)?$
     - /=(RELEASE-ID|meta-update|update)$
 
-
   http:
-
     ca_certs_files: /etc/ssl/certs/ca-certificates.crt
-
-    debug_requests: false
-
+    debug_requests: no
     request_pool_options:
       cachedConnectionTimeout: 600
       maxPersistentPerHost: 10
-      retryAutomatically: true
-
+      retryAutomatically: yes
 
   logging:
 
     formatters:
       basic:
         datefmt: '%Y-%m-%d %H:%M:%S'
         format: '%(asctime)s :: %(name)s :: %(levelname)s: %(message)s'
@@ -213,24 +230,22 @@
     % python -m pyaml /path/to/some/file.yaml
     % curl -s https://www.githubstatus.com/api/v2/summary.json | python -m pyaml
 
 * Process and replace json/yaml file in-place::
 
     % python -m pyaml -r file-with-json.data
 
-* Easier "debug printf" for more complex data (all funcs below are aliases to
-  same thing)::
+* Easier "debug printf" for more complex data (all funcs below are aliases to same thing)::
 
     pyaml.p(stuff)
     pyaml.pprint(my_data)
     pyaml.pprint('----- HOW DOES THAT BREAKS!?!?', input_data, some_var, more_stuff)
     pyaml.print(data, file=sys.stderr) # needs "from __future__ import print_function"
 
-* Force all string values to a certain style (see info on these in
-  `PyYAML docs`_)::
+* Force all string values to a certain style (see info on these in `PyYAML docs`_)::
 
     pyaml.dump(many_weird_strings, string_val_style='|')
     pyaml.dump(multiline_words, string_val_style='>')
     pyaml.dump(no_want_quotes, string_val_style='plain')
 
   Using ``pyaml.add_representer()`` (note \*p\*yaml) as suggested in
   `this SO thread`_ (or `github-issue-7`_) should also work.
@@ -250,67 +265,45 @@
 .. _this SO thread: http://stackoverflow.com/a/7445560
 .. _github-issue-7: https://github.com/mk-fg/pretty-yaml/issues/7
 
 
 Installation
 ------------
 
-It's a regular package for Python (3.x or 2.x).
-
-Module uses PyYAML_ for processing of the actual YAML files and should pull it
-in as a dependency.
-
-Dependency on unidecode_ module is optional and should only be necessary if
-same-id objects or recursion is used within serialized data.
-
-Be sure to use python3/python2, pip3/pip2, easy_install-... binaries below,
-based on which python version you want to install the module for, if you have
-several on the system (as is norm these days for py2-py3 transition).
-
-Using pip_ is the best way::
-
-  % pip install pyaml
-
-(add --user option to install into $HOME for current user only)
+It's a regular python module/package, published on PyPI (as pyaml_).
 
-Or, if you don't have "pip" command::
+Module uses PyYAML_ for processing of the actual YAML files
+and should pull it in as a dependency.
 
-  % python -m ensurepip
-  % python -m pip install --upgrade pip
-  % python -m pip install pyaml
+Dependency on unidecode_ module is optional and should only be necessary
+with force_embed=False keyword, and same-id objects or recursion is used
+within serialized data.
 
-(same suggestion wrt "install --user" as above)
+Using pip_ is how you generally install it, usually coupled with venv_ usage
+(which will also provide "pip" tool itself)::
 
-On a very old systems, one of these might work::
-
-  % curl https://bootstrap.pypa.io/get-pip.py | python
   % pip install pyaml
 
-  % easy_install pyaml
-
-  % git clone --depth=1 https://github.com/mk-fg/pretty-yaml
-  % cd pretty-yaml
-  % python setup.py install
-
-(all of install-commands here also have --user option,
-see also `pip docs "installing" section`_)
-
 Current-git version can be installed like this::
 
-  % pip install 'git+https://github.com/mk-fg/pretty-yaml#egg=pyaml'
-
-Note that to install stuff to system-wide PATH and site-packages (without
---user), elevated privileges (i.e. root and su/sudo) are often required.
+  % pip install 'git+https://github.com/mk-fg/pretty-yaml'
 
-Use "...install --user", `~/.pydistutils.cfg`_ or virtualenv_ to do unprivileged
-installs into custom paths.
-
-More info on python packaging can be found at `packaging.python.org`_.
-
-.. _ruamel.yaml: https://bitbucket.org/ruamel/yaml/
-.. _PyYAML: http://pyyaml.org/
-.. _unidecode: http://pypi.python.org/pypi/Unidecode
-.. _pip: http://pip-installer.org/
-.. _pip docs "installing" section: http://www.pip-installer.org/en/latest/installing.html
-.. _~/.pydistutils.cfg: http://docs.python.org/install/index.html#distutils-configuration-files
-.. _virtualenv: http://pypi.python.org/pypi/virtualenv
+pip will default to installing into currently-active venv, then user's home
+directory (under ``~/.local/lib/python...``), and maybe system-wide when running
+as root (only useful in specialized environments like docker containers).
+
+There are many other python packaging tools - pipenv_, poetry_, pdm_, etc -
+use whatever is most suitable for specific project/environment.
+
+More general info on python packaging can be found at `packaging.python.org`_.
+
+When changing code, unit tests can be run with ``python -m unittest discover``
+from the local repository checkout.
+
+.. _pyaml: https://pypi.org/project/pyaml/
+.. _unidecode: https://pypi.python.org/pypi/Unidecode
+.. _pip: https://pip.pypa.io/en/stable/
+.. _venv: https://docs.python.org/3/library/venv.html
+.. _poetry: https://python-poetry.org/
+.. _pipenv: https://pipenv.pypa.io/
+.. _pdm: https://pdm.fming.dev/
 .. _packaging.python.org: https://packaging.python.org/installing/
```

### Comparing `pyaml-21.8.3/pyaml/__init__.py` & `pyaml-23.5.5/pyaml/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,99 +1,50 @@
-# -*- coding: utf-8 -*-
-from __future__ import unicode_literals, print_function
-
-import itertools as it, operator as op, functools as ft
-from collections import defaultdict, OrderedDict, namedtuple
-import os, sys, io, re
+import os, sys, io, re, string, warnings, pathlib, collections as cs
 
 import yaml
 
-if sys.version_info.major > 2: unicode = str
 
+class PYAMLDumper(yaml.dumper.SafeDumper):
 
-class PrettyYAMLDumper(yaml.dumper.SafeDumper):
+	pyaml_anchor_decode = None # imported from unidecode module when needed
 
 	def __init__(self, *args, **kws):
-		self.pyaml_force_embed = kws.pop('force_embed', False)
+		self.pyaml_force_embed = kws.pop('force_embed', True)
 		self.pyaml_string_val_style = kws.pop('string_val_style', None)
-		self.pyaml_sort_dicts = kws.pop('sort_dicts', True)
-		return super(PrettyYAMLDumper, self).__init__(*args, **kws)
-
-	def represent_odict(dumper, data):
-		value = list()
-		node = yaml.nodes.MappingNode(
-			'tag:yaml.org,2002:map', value, flow_style=None )
-		if dumper.alias_key is not None:
-			dumper.represented_objects[dumper.alias_key] = node
-		for item_key, item_value in data.items():
-			node_key = dumper.represent_data(item_key)
-			node_value = dumper.represent_data(item_value)
-			value.append((node_key, node_value))
-		node.flow_style = False
-		return node
-
-	def represent_undefined(dumper, data):
-		if isinstance(data, tuple) and hasattr(data, '_make') and hasattr(data, '_asdict'):
-			return dumper.represent_odict(data._asdict()) # assuming namedtuple
-		elif isinstance(data, OrderedDict): return dumper.represent_odict(data)
-		elif isinstance(data, dict): return dumper.represent_dict(data)
-		elif callable(getattr(data, 'tolist', None)): return dumper.represent_data(data.tolist())
-		return super(PrettyYAMLDumper, dumper).represent_undefined(data)
-
-	def represent_dict(dumper, data):
-		if not dumper.pyaml_sort_dicts: return dumper.represent_odict(data)
-		return super(PrettyYAMLDumper, dumper).represent_dict(data)
-
-	def serialize_node(self, node, parent, index):
-		if self.pyaml_force_embed: self.serialized_nodes.clear()
-		return super(PrettyYAMLDumper, self).serialize_node(node, parent, index)
+		if (sort_keys := kws.pop('sort_dicts', None)) is not None:
+			self.sort_keys = sort_keys # for compatibility with <23.x module options
+		return super().__init__(*args, **kws)
 
 	@staticmethod
-	def pyaml_transliterate(string):
-		if not all(ord(c) < 128 for c in string):
-			from unidecode import unidecode
-			string = unidecode(string)
-		string_new = ''
-		for ch in string:
-			if '0' <= ch <= '9' or 'A' <= ch <= 'Z' or 'a' <= ch <= 'z' or ch in '-_': string_new += ch
-			else: string_new += '_'
-		return string_new.lower()
+	def pyaml_transliterate(s):
+		if not all(ord(c) < 128 for c in s):
+			if not (unidecode := PYAMLDumper.pyaml_anchor_decode):
+				from unidecode import unidecode
+				PYAMLDumper.pyaml_anchor_decode = unidecode
+			s = unidecode(s)
+		return re.sub(r'[^-_a-z0-9]+', '_', s.lower())
 
-	def anchor_node(self, node, hint=list()):
+	def anchor_node(self, node, hints=list()):
 		if node in self.anchors:
 			if self.anchors[node] is None and not self.pyaml_force_embed:
-				self.anchors[node] = self.generate_anchor(node)\
-					if not hint else '{}'.format(
-						self.pyaml_transliterate(
-							'_-_'.join(map(op.attrgetter('value'), hint)) ) )
+				self.anchors[node] = (
+					self.generate_anchor(node) if not hints else
+					self.pyaml_transliterate('_-_'.join(h.value for h in hints)) )
 		else:
 			self.anchors[node] = None
 			if isinstance(node, yaml.nodes.SequenceNode):
-				for item in node.value:
-					self.anchor_node(item)
+				for item in node.value: self.anchor_node(item)
 			elif isinstance(node, yaml.nodes.MappingNode):
 				for key, value in node.value:
 					self.anchor_node(key)
-					self.anchor_node(value, hint=hint+[key])
+					self.anchor_node(value, hints=hints+[key])
 
-PrettyYAMLDumper.add_representer(dict, PrettyYAMLDumper.represent_dict)
-PrettyYAMLDumper.add_representer(defaultdict, PrettyYAMLDumper.represent_dict)
-PrettyYAMLDumper.add_representer(OrderedDict, PrettyYAMLDumper.represent_odict)
-PrettyYAMLDumper.add_representer(set, PrettyYAMLDumper.represent_list)
-PrettyYAMLDumper.add_representer(None, PrettyYAMLDumper.represent_undefined)
-
-if sys.version_info.major >= 3:
-	try: import pathlib
-	except ImportError: pass
-	else:
-		PrettyYAMLDumper.add_representer(
-			type(pathlib.Path('')), lambda cls,o: cls.represent_data(str(o)) )
-
-
-class UnsafePrettyYAMLDumper(PrettyYAMLDumper):
+	def serialize_node(self, node, parent, index):
+		if self.pyaml_force_embed: self.anchors[node] = self.serialized_nodes.clear()
+		return super().serialize_node(node, parent, index)
 
 	def expect_block_sequence(self):
 		self.increase_indent(flow=False, indentless=False)
 		self.state = self.expect_first_block_sequence_item
 
 	def expect_block_sequence_item(self, first=False):
 		if not first and isinstance(self.event, yaml.events.SequenceEndEvent):
@@ -101,110 +52,136 @@
 			self.state = self.states.pop()
 		else:
 			self.write_indent()
 			self.write_indicator('-', True, indention=True)
 			self.states.append(self.expect_block_sequence_item)
 			self.expect_node(sequence=True)
 
-	def choose_scalar_style(self):
-		is_dict_key = self.states[-1] == self.expect_block_mapping_simple_value
-		if is_dict_key:
-			# Don't mess-up (replace) styles for dict keys, if possible
+	def check_simple_key(self):
+		res = super().check_simple_key()
+		self.analysis.allow_flow_plain = False
+		return res
+
+	def choose_scalar_style(self, _re1=re.compile(r':(\s|$)')):
+		if self.states[-1] == self.expect_block_mapping_simple_value:
+			# Don't override string style for dict keys
 			if self.pyaml_string_val_style: self.event.style = 'plain'
-		else:
-			# Make sure we don't create "key: null" mapping accidentally
-			if self.event.value.endswith(':'): self.event.style = "'"
-		return super(UnsafePrettyYAMLDumper, self).choose_scalar_style()\
-			if self.event.style != 'plain' else ("'" if ' ' in self.event.value else None)
-
-	def represent_stringish(dumper, data):
-		# Will crash on bytestrings with weird chars in them,
-		#  because we can't tell if it's supposed to be e.g. utf-8 readable string
-		#  or an arbitrary binary buffer, and former one *must* be pretty-printed
-		# PyYAML's Representer.represent_str does the guesswork and !!binary or !!python/str
-		# Explicit crash on any bytes object might be more sane, but also annoying
-		# Use something like base64 to encode such buffer values instead
-		# Having such binary stuff pretty much everywhere on unix (e.g. paths) kinda sucks
-		data = unicode(data) # read the comment above
-
-		# Try to use '|' style for multiline data,
-		#  quoting it with 'literal' if lines are too long anyway,
-		#  not sure if Emitter.analyze_scalar can also provide useful info here
-		style = dumper.pyaml_string_val_style
-		if not style:
-			style = 'plain'
-			if '\n' in data or not data or data == '-' or data[0] in '!&*[' or '#' in data:
+		# Do default thing for complicated stuff
+		if self.event.style != 'plain': return super().choose_scalar_style()
+		# Make sure style isn't overidden for strings like list/mapping items
+		if (s := self.event.value).startswith('- ') or _re1.search(s): return "'"
+
+	def represent_str(self, data):
+		if not (style := self.pyaml_string_val_style):
+			if '\n' in data[:-1]:
 				style = 'literal'
-				if '\n' in data[:-1]:
-					for line in data.splitlines():
-						if len(line) > dumper.best_width: break
-					else: style = '|'
-
+				for line in data.splitlines():
+					if len(line) > self.best_width: break
+				else: style = '|'
 		return yaml.representer.ScalarNode('tag:yaml.org,2002:str', data, style=style)
 
-for str_type in {bytes, unicode}:
-	UnsafePrettyYAMLDumper.add_representer(
-		str_type, UnsafePrettyYAMLDumper.represent_stringish )
-
-UnsafePrettyYAMLDumper.add_representer(
-	type(None), lambda s,o: s.represent_scalar('tag:yaml.org,2002:null', '') )
-
-def add_representer(*args, **kws):
-	PrettyYAMLDumper.add_representer(*args, **kws)
-	UnsafePrettyYAMLDumper.add_representer(*args, **kws)
-
-
-def dump_add_vspacing(buff, vspacing):
-	'Post-processing to add some nice-ish spacing for deeper map/list levels.'
-	if isinstance(vspacing, int):
-		vspacing = ['\n']*(vspacing+1)
-	buff.seek(0)
-	result = list()
-	for line in buff:
-		level = 0
-		line = line.decode('utf-8')
-		result.append(line)
-		if ':' in line or re.search(r'---(\s*$|\s)', line):
-			while line.startswith('  '):
-				level, line = level + 1, line[2:]
-			if len(vspacing) > level and len(result) != 1:
-				vspace = vspacing[level]
-				result.insert( -1, vspace
-					if not isinstance(vspace, int) else '\n'*vspace )
-	buff.seek(0), buff.truncate()
-	buff.write(''.join(result).encode('utf-8'))
-
-
-def dump_all(data, *dump_args, **dump_kws):
-	return dump(data, *dump_args, multiple_docs=True, **dump_kws)
+	def represent_undefined(self, data):
+		if isinstance(data, tuple) and hasattr(data, '_make') and hasattr(data, '_asdict'):
+			return self.represent_dict(data._asdict()) # assuming namedtuple
+		elif isinstance(data, dict): return self.represent_dict(data) # some kind of dict
+		elif callable(getattr(data, 'tolist', None)):
+			return self.represent_data(data.tolist()) # numpy arrays
+		return super().represent_undefined(data)
+
+
+# Unsafe was a separate class in <23.x versions, left here for compatibility
+UnsafePYAMLDumper = PYAMLDumper
+
+add_representer = PYAMLDumper.add_representer
+
+add_representer( bool,
+	lambda s,o: s.represent_scalar('tag:yaml.org,2002:bool', ['no', 'yes'][o]) )
+add_representer( type(None),
+	lambda s,o: s.represent_scalar('tag:yaml.org,2002:null', '') )
+add_representer(str, PYAMLDumper.represent_str)
+
+add_representer(cs.defaultdict, PYAMLDumper.represent_dict)
+add_representer(cs.OrderedDict, PYAMLDumper.represent_dict)
+add_representer(set, PYAMLDumper.represent_list)
+add_representer(
+	type(pathlib.Path('')), lambda cls,o: cls.represent_data(str(o)) )
+add_representer(None, PYAMLDumper.represent_undefined)
+
+
+def dump_add_vspacing(yaml_str, split_lines=40, split_count=2):
+	'''Add some newlines to separate overly long YAML lists/mappings.
+		"long" means both >split_lines in length and has >split_count items.'''
+	def _add_vspacing(lines):
+		a = ind_re = ind_item = None
+		blocks, item_lines = list(), list()
+		for n, line in enumerate(lines):
+			if ind_item is None and (m := re.match('( *)[^# ]', line)):
+				ind_item = m.group(1)
+				lines.append(f'{ind_item}.') # to run add_vspacing on last block
+			if ind_re:
+				if ind_re.match(line): continue
+				if n - a > split_lines: blocks.append((a, n, _add_vspacing(lines[a:n])))
+				ind_re = None
+			if re.match(fr'{ind_item}\S', line): item_lines.append(n)
+			if m := re.match(r'( *)\S.*:\s*$', line):
+				a, ind_re = n+1, re.compile(m.group(1) + r' ')
+		if split_items := len(lines) > split_lines and len(item_lines) > split_count:
+			for n in item_lines: lines[n] = f'\n{lines[n]}'
+		for a, b, block in reversed(blocks): lines[a:b] = block
+		if ind_item is not None: lines.pop()
+		if split_items: lines.append('')
+		return lines
+	yaml_str = '\n'.join(_add_vspacing(yaml_str.splitlines()))
+	return re.sub(r'\n\n+', '\n\n', yaml_str.strip() + '\n')
+
+
+def dump( data, dst=str, safe=None, force_embed=True, vspacing=True,
+		string_val_style=None, sort_dicts=None, multiple_docs=False, **pyyaml_kws ):
+	'Serialize data as pretty-YAML to either specified dst file-like object, or str/bytes'
+	if safe is not None:
+		warnings.warn( 'pyaml module "safe" arg/keyword'
+			' is ignored as implicit safe=True, as of pyaml >= 23.x' )
+	if sort_dicts is not None:
+		warnings.warn( 'pyaml module "sort_dicts" arg/keyword'
+			' is ignored as of pyaml >= 23.x - translated to sort_keys pyaml keyword' )
 
-def dump( data, dst=unicode, safe=False, force_embed=False, vspacing=None,
-		string_val_style=None, sort_dicts=True, multiple_docs=False, **pyyaml_kws ):
-	buff = io.BytesIO()
-	Dumper = PrettyYAMLDumper if safe else UnsafePrettyYAMLDumper
-	Dumper = ft.partial( Dumper,
+	buff = io.StringIO()
+	Dumper = lambda *a,**kw: PYAMLDumper( *a, **kw,
 		force_embed=force_embed, string_val_style=string_val_style, sort_dicts=sort_dicts )
 	if not multiple_docs: data = [data]
 	else: pyyaml_kws.setdefault('explicit_start', True)
 	yaml.dump_all( data, buff, Dumper=Dumper,
-		default_flow_style=False, allow_unicode=True, encoding='utf-8', **pyyaml_kws )
+		default_flow_style=False, allow_unicode=True, **pyyaml_kws )
+	buff = buff.getvalue()
 
-	if vspacing is not None:
-		dump_add_vspacing(buff, vspacing)
+	if vspacing not in [None, False]:
+		if vspacing is True: vspacing = dict()
+		elif not isinstance(vspacing, dict):
+			warnings.warn(
+				'Unsupported pyaml "vspacing" parameter type:'
+					f' [{vspacing.__class__.__name__}] {vspacing}\n'
+				'As of pyaml >= 23.x it should be either True or keywords-dict'
+				' for pyaml_add_vspacing, and any other values are ignored,'
+				' enabling default vspacing behavior.', DeprecationWarning, stacklevel=2 )
+			vspacing = dict()
+		buff = dump_add_vspacing(buff, **vspacing)
 
-	buff = buff.getvalue()
-	if dst is bytes: return buff
-	elif dst is unicode: return buff.decode('utf-8')
+	if dst is bytes: return buff.encode()
+	elif dst is str: return buff
 	else:
-		try: dst.write(b'') # tests if dst is unicode- or bytestream
-		except: dst.write(buff.decode('utf-8'))
-		else: dst.write(buff)
+		try: dst.write(b'') # tests if dst is str- or bytestream
+		except: dst.write(buff)
+		else: dst.write(buff.encode())
+
+
+def dump_all(data, *dump_args, **dump_kws):
+	return dump(data, *dump_args, multiple_docs=True, **dump_kws)
 
 def dumps(data, **dump_kws):
-	return dump(data, dst=bytes, **dump_kws)
+	return dump(data, **dump_kws)
 
 def pprint(*data, **dump_kws):
 	dst = dump_kws.pop('file', dump_kws.pop('dst', sys.stdout))
 	if len(data) == 1: data, = data
 	dump(data, dst=dst, **dump_kws)
 
 p, _p = pprint, print
```

### Comparing `pyaml-21.8.3/pyaml/__main__.py` & `pyaml-23.5.5/pyaml/__main__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,28 +1,37 @@
-# -*- coding: utf-8 -*-
-
-import os, sys, stat, tempfile, contextlib, yaml, pyaml
+import os, sys, stat, tempfile, contextlib
+import yaml, pyaml
 
 
 @contextlib.contextmanager
-def safe_replacement(path, *open_args, **open_kws):
-	path = str(path)
-	try: mode = stat.S_IMODE(os.stat(path).st_mode)
-	except (OSError, IOError): mode = None
+def safe_replacement(path, *open_args, mode=None, xattrs=None, **open_kws):
+	'Context to atomically create/replace file-path in-place unless errors are raised'
+	path, xattrs = str(path), None
+	if mode is None:
+		try: mode = stat.S_IMODE(os.lstat(path).st_mode)
+		except FileNotFoundError: pass
+	if xattrs is None and getattr(os, 'getxattr', None): # MacOS
+		try: xattrs = dict((k, os.getxattr(path, k)) for k in os.listxattr(path))
+		except FileNotFoundError: pass
 	open_kws.update( delete=False,
 		dir=os.path.dirname(path), prefix=os.path.basename(path)+'.' )
+	if not open_args: open_kws.setdefault('mode', 'w')
 	with tempfile.NamedTemporaryFile(*open_args, **open_kws) as tmp:
 		try:
 			if mode is not None: os.fchmod(tmp.fileno(), mode)
+			if xattrs:
+				for k, v in xattrs.items(): os.setxattr(path, k, v)
 			yield tmp
 			if not tmp.closed: tmp.flush()
+			try: os.fdatasync(tmp)
+			except AttributeError: pass # MacOS
 			os.rename(tmp.name, path)
 		finally:
 			try: os.unlink(tmp.name)
-			except (OSError, IOError): pass
+			except FileNotFoundError: pass
 
 
 def main(argv=None):
 	import argparse
 	parser = argparse.ArgumentParser(
 		description='Process and dump prettified YAML to stdout.')
 	parser.add_argument('path', nargs='?', metavar='path',
```

### Comparing `pyaml-21.8.3/pyaml/tests/dump.py` & `pyaml-23.5.5/pyaml/tests/test_dump.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,18 @@
-# -*- coding: utf-8 -*-
-from __future__ import unicode_literals, print_function
+import os, sys, io, unittest, json, collections as cs
 
-import itertools as it, operator as op, functools as ft
-import os, sys, io, yaml, unittest
-
-if sys.version_info.major > 2:
-	from collections import OrderedDict, namedtuple
-	from collections.abc import Mapping
-	unicode = str
-else: from collections import Mapping, OrderedDict, namedtuple
+import yaml
 
 try: import pyaml
 except ImportError:
 	sys.path.insert(1, os.path.join(__file__, *['..']*3))
 	import pyaml
 
 
-large_yaml = b'''
+large_yaml = br'''
 ### Default (baseline) configuration parameters.
 ### DO NOT ever change this config, use -c commandline option instead!
 
 # Note that this file is YAML, so YAML types can be used here, see http://yaml.org/type/
 # For instance, large number can be specified as "10_000_000" or "!!float 10e6".
 
 source:
@@ -158,26 +150,26 @@
   root:
     level: custom
     handlers: [console]
 '''
 
 data = dict(
 	path='/some/path',
-	query_dump=OrderedDict([
+	query_dump=cs.OrderedDict([
 		('key1', 'тест1'),
 		('key2', 'тест2'),
 		('key3', 'тест3'),
 		('последний', None) ]),
-	ids=OrderedDict(),
+	ids=cs.OrderedDict(),
 	a=[1,None,'asd', 'не-ascii'], b=3.5, c=None,
-	asd=OrderedDict([('b', 1), ('a', 2)]) )
+	asd=cs.OrderedDict([('b', 1), ('a', 2)]) )
 data['query_dump_clone'] = data['query_dump']
 data['ids']['id в уникоде'] = [4, 5, 6]
 data['ids']['id2 в уникоде'] = data['ids']['id в уникоде']
-# data["'asd'\n!\0\1"] =OrderedDict([('b', 1), ('a', 2)]) <-- fails in many ways
+# data["'asd'\n!\0\1"] =cs.OrderedDict([('b', 1), ('a', 2)]) <-- fails in many ways
 
 data_str_multiline = dict(cert=(
 	'-----BEGIN CERTIFICATE-----\n'
 	'MIIDUjCCAjoCCQD0/aLLkLY/QDANBgkqhkiG9w0BAQUFADBqMRAwDgYDVQQKFAdm\n'
 	'Z19jb3JlMRYwFAYDVQQHEw1ZZWthdGVyaW5idXJnMR0wGwYDVQQIExRTdmVyZGxv\n'
 	'dnNrYXlhIG9ibGFzdDELMAkGA1UEBhMCUlUxEjAQBgNVBAMTCWxvY2FsaG9zdDAg\n'
 	'Fw0xMzA0MjQwODUxMTRaGA8yMDUzMDQxNDA4NTExNFowajEQMA4GA1UEChQHZmdf\n'
@@ -214,118 +206,90 @@
 	'uN59JWnpa/6RBJbykiZh8AMwdTonu02g95+13g44kjlUnK3WG5vGeUTrGv+6cnAf'
 	'4B4XwnWTHADQxbdRLja/YXqTkZrXkd7W3Ipxdi0bDCOSi/BXSmiblyWdbNU4cHF/'
 	'Ex4dTWeGFiTWY2upX8sa+1PuZjk/Ry+RPMLzuamvzP20mVXmKtEIfQTzz4b8+Pom'
 	'T1gqPkNEbe2j1DciRNUOH1iuY+cL/b7JqZvvdQK34w3t9Cz7GtMWKo+g+ZRdh3+q'
 	'2sn5m3EkrUb1hSKQbMWTbnaG4C/F3i4KVkH+8AZmR9OvOmZ+7Lo=' ))
 
 
-# Restore Python2-like heterogeneous list sorting functionality in Python3
-# Based on https://gist.github.com/pR0Ps/1e1a1e892aad5b691448
-def compare(x, y):
-	if x == y: return 0
-	try:
-		if x < y: return -1
-		else: return 1
-
-	except TypeError as e:
-		# The case where both are None is taken care of by the equality test
-		if x is None: return -1
-		elif y is None: return 1
-
-		if type(x) != type(y):
-			return compare(*map(lambda t: type(t).__name__, [x, y]))
-
-		# Types are the same but a native compare didn't work.
-		# x and y might be indexable, recursively compare elements
-		for a, b in zip(x, y):
-			c = compare(a, b)
-			if c != 0: return c
-
-		return compare(len(x), len(y))
-
-
 class DumpTests(unittest.TestCase):
 
 	def flatten(self, data, path=tuple()):
 		dst = list()
 		if isinstance(data, (tuple, list)):
-			for v in data:
-				dst.extend(self.flatten(v, path + (list,)))
-		elif isinstance(data, Mapping):
-			for k,v in data.items():
-				dst.extend(self.flatten(v, path + (k,)))
+			for v in data: dst.extend(self.flatten(v, path + ('!!list',)))
+		elif isinstance(data, dict):
+			for k,v in data.items(): dst.extend(self.flatten(v, path + (k,)))
 		else: dst.append((path, data))
-		return tuple(sorted(dst, key=ft.cmp_to_key(compare)))
+		return tuple(sorted(dst, key=lambda v: json.dumps(v, sort_keys=True)))
 
 	def test_dst(self):
 		buff = io.BytesIO()
 		self.assertIs(pyaml.dump(data, buff), None)
 		self.assertIsInstance(pyaml.dump(data, str), str)
-		self.assertIsInstance(pyaml.dump(data, unicode), unicode)
+		self.assertIsInstance(pyaml.dump(data, bytes), bytes)
 
 	def test_simple(self):
 		a = self.flatten(data)
-		b = pyaml.dump(data, unicode)
+		b = pyaml.dump(data)
 		self.assertEqual(a, self.flatten(yaml.safe_load(b)))
 
 	def test_vspacing(self):
 		data = yaml.safe_load(large_yaml)
 		a = self.flatten(data)
-		b = pyaml.dump(data, unicode, vspacing=[2, 1])
+		b = pyaml.dump(data, vspacing=dict(split_lines=10, split_count=2))
 		self.assertEqual(a, self.flatten(yaml.safe_load(b)))
 		pos, pos_list = 0, list()
 		while True:
 			pos = b.find(u'\n', pos+1)
 			if pos < 0: break
 			pos_list.append(pos)
 		self.assertEqual( pos_list,
-			[ 12, 13, 25, 33, 53, 74, 89, 108, 158, 185, 265, 300, 345, 346, 356, 376, 400, 426, 427,
-				460, 461, 462, 470, 508, 564, 603, 604, 605, 611, 612, 665, 666, 690, 691, 715, 748,
-				777, 806, 807, 808, 817, 818, 832, 843, 878, 948, 949, 961, 974, 1009, 1032, 1052,
-				1083, 1102, 1123, 1173, 1195, 1234, 1257, 1276, 1300, 1301, 1312, 1325, 1341, 1359,
-				1374, 1375, 1383, 1397, 1413, 1431, 1432, 1453, 1454, 1467, 1468, 1485, 1486, 1487,
-				1498, 1499, 1530, 1531, 1551, 1552, 1566, 1577, 1590, 1591, 1612, 1613, 1614, 1622,
-				1623, 1638, 1648, 1649, 1657, 1658, 1688, 1689, 1698, 1720, 1730 ] )
-		b = pyaml.dump(data, unicode)
+			[12, 13, 25, 33, 52, 73, 88, 107, 157, 184, 264, 299, 344, 345, 355, 375, 399,
+			424, 425, 458, 459, 467, 505, 561, 600, 601, 607, 660, 681, 705, 738, 767, 795,
+			796, 805, 806, 820, 831, 866, 936, 937, 949, 950, 963, 998, 1021, 1041, 1072,
+			1073, 1092, 1113, 1163, 1185, 1224, 1247, 1266, 1290, 1291, 1302, 1315, 1331,
+			1349, 1364, 1365, 1373, 1387, 1403, 1421, 1422, 1440, 1441, 1454, 1455, 1471,
+			1472, 1483, 1511, 1528, 1542, 1553, 1566, 1584, 1585, 1593, 1608, 1618, 1626,
+			1656, 1665, 1686, 1696] )
+		b = pyaml.dump(data, vspacing=False)
 		self.assertNotIn('\n\n', b)
 
 	def test_ids(self):
-		b = pyaml.dump(data, unicode)
+		b = pyaml.dump(data, force_embed=False)
 		self.assertNotIn('&id00', b)
 		self.assertIn('query_dump_clone: *query_dump_clone', b)
-		self.assertIn("'id в уникоде': &ids_-_id2_v_unikode", b) # kinda bug - should be just "id"
+		self.assertIn("id в уникоде: &ids_-_id2_v_unikode", b) # kinda bug - should be just "id"
 
 	def test_force_embed(self):
-		b = pyaml.dump(data, unicode, force_embed=True)
-		c = pyaml.dump(data, unicode, safe=True, force_embed=True)
-		for char, dump in it.product('*&', [b, c]):
-			self.assertNotIn(char, dump)
+		for check, fe in (self.assertNotIn, True), (self.assertIn, False):
+			dump = pyaml.dump(data, force_embed=fe)
+			for c in '*&': check(c, dump)
 
 	def test_encoding(self):
-		b = pyaml.dump(data, unicode, force_embed=True)
-		b_lines = list(map(unicode.strip, b.splitlines()))
+		b = pyaml.dump(data, force_embed=True)
+		b_lines = list(map(str.strip, b.splitlines()))
 		chk = ['query_dump:', 'key1: тест1', 'key2: тест2', 'key3: тест3', 'последний:']
 		pos = b_lines.index('query_dump:')
 		self.assertEqual(b_lines[pos:pos + len(chk)], chk)
 
 	def test_str_long(self):
-		b = pyaml.dump(data_str_long, unicode)
+		b = pyaml.dump(data_str_long)
 		self.assertNotIn('"', b)
 		self.assertNotIn("'", b)
 		self.assertEqual(len(b.splitlines()), 1)
 
 	def test_str_multiline(self):
-		b = pyaml.dump(data_str_multiline, unicode)
+		b = pyaml.dump(data_str_multiline)
 		b_lines = b.splitlines()
 		self.assertGreater(len(b_lines), len(data_str_multiline['cert'].splitlines()))
 		for line in b_lines: self.assertLess(len(line), 100)
 
 	def test_dumps(self):
 		b = pyaml.dumps(data_str_multiline)
-		self.assertIsInstance(b, bytes)
+		self.assertIsInstance(b, str)
 
 	def test_print(self):
 		self.assertIs(pyaml.print, pyaml.pprint)
 		self.assertIs(pyaml.print, pyaml.p)
 		buff = io.BytesIO()
 		b = pyaml.dump(data_str_multiline, dst=bytes)
 		pyaml.print(data_str_multiline, file=buff)
@@ -353,14 +317,21 @@
 		val2 = yaml.safe_load(val1_str)
 		val2_str = pyaml.dump(val2)
 		val3 = yaml.safe_load(val2_str)
 		self.assertEqual(val1, val2)
 		self.assertEqual(val1_str, val2_str)
 		self.assertEqual(val2, val3)
 
+	def test_unqouted_spaces(self):
+		val1 = {'key': 'word1 word2 word3', 'key key': 'asd', 'k3': 'word: stuff'}
+		val1_str = pyaml.dump(val1)
+		val2 = yaml.safe_load(val1_str)
+		self.assertEqual(val1, val2)
+		self.assertIn('key: word1 word2 word3', val1_str)
+
 	def test_empty_strings(self):
 		val1 = {'key': ['', 'stuff', '', 'more'], '': 'value', 'k3': ''}
 		val1_str = pyaml.dump(val1)
 		val2 = yaml.safe_load(val1_str)
 		val2_str = pyaml.dump(val2)
 		val3 = yaml.safe_load(val2_str)
 		self.assertEqual(val1, val2)
@@ -384,40 +355,42 @@
 		val1 = {'key': '-'}
 		val1_str = pyaml.dump(val1)
 		val2 = yaml.safe_load(val1_str)
 		val2_str = pyaml.dump(val2)
 		val3 = yaml.safe_load(val2_str)
 
 	def test_namedtuple(self):
-		TestTuple = namedtuple('TestTuple', 'y x z')
+		TestTuple = cs.namedtuple('TestTuple', 'y x z')
 		val = TestTuple(1, 2, 3)
-		val_str = pyaml.dump(val)
+		val_str = pyaml.dump(val, sort_keys=False)
 		self.assertEqual(val_str, u'y: 1\nx: 2\nz: 3\n') # namedtuple order was preserved
 
 	def test_ordereddict(self):
-		d = OrderedDict((i, '') for i in reversed(range(10)))
-		lines = pyaml.dump(d).splitlines()
+		d = cs.OrderedDict((i, '') for i in reversed(range(10)))
+		lines = pyaml.dump(d, sort_keys=False).splitlines()
 		self.assertEqual(lines, list(reversed(sorted(lines))))
 
 	def test_pyyaml_params(self):
 		d = {'foo': 'lorem ipsum ' * 30} # 300+ chars
 		for w in 40, 80, 200:
 			lines = pyaml.dump(d, width=w, indent=10).splitlines()
 			for n, line in enumerate(lines, 1):
 				self.assertLess(len(line), w*1.2)
 				if n != len(lines): self.assertGreater(len(line), w*0.8)
 
 	def test_multiple_docs(self):
 		docs = [yaml.safe_load(large_yaml), dict(a=1, b=2, c=3)]
-		docs_str = pyaml.dump_all(docs, vspacing=[3, 2])
+		docs_str = pyaml.dump_all(docs, vspacing=True)
 		self.assertTrue(docs_str.startswith('---'))
-		self.assertIn('---\n\n\n\na: 1\n\n\n\nb: 2\n\n\n\nc: 3\n', docs_str)
-		docs_str2 = pyaml.dump(docs, vspacing=[3, 2], multiple_docs=True)
+		self.assertIn('---\n\na: 1\n\nb: 2\n\nc: 3\n', docs_str)
+
+
+		docs_str2 = pyaml.dump(docs, vspacing=True, multiple_docs=True)
 		self.assertEqual(docs_str, docs_str2)
-		docs_str2 = pyaml.dump(docs, vspacing=[3, 2])
+		docs_str2 = pyaml.dump(docs, vspacing=True)
 		self.assertNotEqual(docs_str, docs_str2)
 		docs_str2 = pyaml.dump_all(docs, explicit_start=False)
 		self.assertFalse(docs_str2.startswith('---'))
 		self.assertNotEqual(docs_str, docs_str2)
 		docs_str = pyaml.dump(docs, multiple_docs=True, explicit_start=False)
 		self.assertEqual(docs_str, docs_str2)
```

