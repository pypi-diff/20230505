# Comparing `tmp/cartman-0.3.0.tar.gz` & `tmp/cartman-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cartman-0.3.0.tar", last modified: Sat Mar 14 20:46:39 2020, max compression
+gzip compressed data, was "cartman-0.3.1.tar", last modified: Fri May  5 17:09:08 2023, max compression
```

## Comparing `cartman-0.3.0.tar` & `cartman-0.3.1.tar`

### file list

```diff
@@ -1,20 +1,27 @@
-drwxr-xr-x   0 tamentis   (501) staff       (20)        0 2020-03-14 20:46:39.000000 cartman-0.3.0/
--rw-r--r--   0 tamentis   (501) staff       (20)    12628 2020-03-14 20:46:39.000000 cartman-0.3.0/PKG-INFO
-drwxr-xr-x   0 tamentis   (501) staff       (20)        0 2020-03-14 20:46:39.000000 cartman-0.3.0/cartman.egg-info/
--rw-r--r--   0 tamentis   (501) staff       (20)    12628 2020-03-14 20:46:39.000000 cartman-0.3.0/cartman.egg-info/PKG-INFO
--rw-r--r--   0 tamentis   (501) staff       (20)      299 2020-03-14 20:46:39.000000 cartman-0.3.0/cartman.egg-info/SOURCES.txt
--rw-r--r--   0 tamentis   (501) staff       (20)       16 2020-03-14 20:46:39.000000 cartman-0.3.0/cartman.egg-info/requires.txt
--rw-r--r--   0 tamentis   (501) staff       (20)        8 2020-03-14 20:46:39.000000 cartman-0.3.0/cartman.egg-info/top_level.txt
--rw-r--r--   0 tamentis   (501) staff       (20)        1 2020-03-14 20:46:39.000000 cartman-0.3.0/cartman.egg-info/dependency_links.txt
-drwxr-xr-x   0 tamentis   (501) staff       (20)        0 2020-03-14 20:46:39.000000 cartman-0.3.0/cartman/
--rw-r--r--   0 tamentis   (501) staff       (20)     2597 2020-03-14 20:32:57.000000 cartman-0.3.0/cartman/ticket.py
--rw-r--r--   0 tamentis   (501) staff       (20)      860 2020-03-14 20:32:57.000000 cartman-0.3.0/cartman/compat.py
--rw-r--r--   0 tamentis   (501) staff       (20)     1287 2020-03-14 20:32:57.000000 cartman-0.3.0/cartman/ui.py
--rw-r--r--   0 tamentis   (501) staff       (20)      798 2020-03-14 20:34:07.000000 cartman-0.3.0/cartman/__init__.py
--rw-r--r--   0 tamentis   (501) staff       (20)     6556 2020-03-14 20:32:57.000000 cartman-0.3.0/cartman/text.py
--rw-r--r--   0 tamentis   (501) staff       (20)    31190 2020-03-14 20:32:57.000000 cartman-0.3.0/cartman/app.py
--rw-r--r--   0 tamentis   (501) staff       (20)     1501 2020-03-14 20:32:57.000000 cartman-0.3.0/cartman/exceptions.py
--rwxr-xr-x   0 tamentis   (501) staff       (20)     1425 2020-03-14 20:32:57.000000 cartman-0.3.0/setup.py
--rw-r--r--   0 tamentis   (501) staff       (20)       38 2020-03-14 20:46:39.000000 cartman-0.3.0/setup.cfg
--rwxr-xr-x   0 tamentis   (501) staff       (20)     2871 2020-03-14 20:32:57.000000 cartman-0.3.0/cm
--rw-r--r--   0 tamentis   (501) staff       (20)     6983 2020-03-14 20:32:57.000000 cartman-0.3.0/README.rst
+drwxr-xr-x   0 bertrand   (501) staff       (20)        0 2023-05-05 17:09:08.947233 cartman-0.3.1/
+-rw-r--r--   0 bertrand   (501) staff       (20)      746 2020-03-14 20:32:57.000000 cartman-0.3.1/LICENSE
+-rw-r--r--   0 bertrand   (501) staff       (20)     8033 2023-05-05 17:09:08.947100 cartman-0.3.1/PKG-INFO
+-rw-r--r--   0 bertrand   (501) staff       (20)     7003 2023-05-05 16:56:50.000000 cartman-0.3.1/README.rst
+drwxr-xr-x   0 bertrand   (501) staff       (20)        0 2023-05-05 17:09:08.945663 cartman-0.3.1/cartman/
+-rw-r--r--   0 bertrand   (501) staff       (20)      798 2023-05-05 16:53:11.000000 cartman-0.3.1/cartman/__init__.py
+-rw-r--r--   0 bertrand   (501) staff       (20)    31190 2020-03-14 20:32:57.000000 cartman-0.3.1/cartman/app.py
+-rw-r--r--   0 bertrand   (501) staff       (20)      860 2020-03-14 20:32:57.000000 cartman-0.3.1/cartman/compat.py
+-rw-r--r--   0 bertrand   (501) staff       (20)     1501 2020-03-14 20:32:57.000000 cartman-0.3.1/cartman/exceptions.py
+-rw-r--r--   0 bertrand   (501) staff       (20)     6558 2023-05-05 16:52:49.000000 cartman-0.3.1/cartman/text.py
+-rw-r--r--   0 bertrand   (501) staff       (20)     2597 2020-03-14 20:32:57.000000 cartman-0.3.1/cartman/ticket.py
+-rw-r--r--   0 bertrand   (501) staff       (20)     1287 2020-03-14 20:32:57.000000 cartman-0.3.1/cartman/ui.py
+drwxr-xr-x   0 bertrand   (501) staff       (20)        0 2023-05-05 17:09:08.946224 cartman-0.3.1/cartman.egg-info/
+-rw-r--r--   0 bertrand   (501) staff       (20)     8033 2023-05-05 17:09:08.000000 cartman-0.3.1/cartman.egg-info/PKG-INFO
+-rw-r--r--   0 bertrand   (501) staff       (20)      397 2023-05-05 17:09:08.000000 cartman-0.3.1/cartman.egg-info/SOURCES.txt
+-rw-r--r--   0 bertrand   (501) staff       (20)        1 2023-05-05 17:09:08.000000 cartman-0.3.1/cartman.egg-info/dependency_links.txt
+-rw-r--r--   0 bertrand   (501) staff       (20)       16 2023-05-05 17:09:08.000000 cartman-0.3.1/cartman.egg-info/requires.txt
+-rw-r--r--   0 bertrand   (501) staff       (20)        8 2023-05-05 17:09:08.000000 cartman-0.3.1/cartman.egg-info/top_level.txt
+-rwxr-xr-x   0 bertrand   (501) staff       (20)     2871 2020-03-14 20:32:57.000000 cartman-0.3.1/cm
+-rw-r--r--   0 bertrand   (501) staff       (20)      831 2023-05-05 17:07:07.000000 cartman-0.3.1/pyproject.toml
+-rw-r--r--   0 bertrand   (501) staff       (20)       38 2023-05-05 17:09:08.947266 cartman-0.3.1/setup.cfg
+-rwxr-xr-x   0 bertrand   (501) staff       (20)     1425 2020-03-14 20:32:57.000000 cartman-0.3.1/setup.py
+drwxr-xr-x   0 bertrand   (501) staff       (20)        0 2023-05-05 17:09:08.946942 cartman-0.3.1/tests/
+-rw-r--r--   0 bertrand   (501) staff       (20)     8504 2020-03-14 20:32:57.000000 cartman-0.3.1/tests/test_app.py
+-rw-r--r--   0 bertrand   (501) staff       (20)     4156 2020-03-14 20:32:57.000000 cartman-0.3.1/tests/test_text.py
+-rw-r--r--   0 bertrand   (501) staff       (20)     1125 2020-03-14 20:32:57.000000 cartman-0.3.1/tests/test_ticket.py
+-rw-r--r--   0 bertrand   (501) staff       (20)      605 2020-03-14 20:32:57.000000 cartman-0.3.1/tests/test_ui.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `cartman-0.3.0/PKG-INFO` & `cartman-0.3.1/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,336 +1,278 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: cartman
-Version: 0.3.0
+Version: 0.3.1
 Summary: trac command-line tools
 Home-page: http://tamentis.com/projects/cartman/
 Author: Bertrand Janin
-Author-email: b@janin.com
+Author-email: Bertrand Janin <bertrand@janin.com>
 License: ISC License (ISCL, BSD/MIT compatible)
-Description: cartman
-        =======
-        
-        .. image:: https://travis-ci.org/tamentis/cartman.png
-        
-        *cartman* allows you to create and manage your Trac_ tickets from the
-        command-line, without the need to setup physical access to the Trac_
-        installation/database or even the need to install a plugin on Trac_.  All you
-        need is a Trac_ account.
-        
-        Examples
-        --------
-        Create a new ticket, that will open your $EDITOR::
-        
-            $ cm new
-        
-        View the content of a ticket::
-        
-            $ cm view 1514
-        
-        Configuration
-        -------------
-        At a minimum you need to create a ``~/.cartman/config`` file with the
-        following::
-        
-            [trac]
-            base_url = http://your.trac.install/
-            username = tamentis
-            password = sitnemat
-        
-        The password can also be specified through a `TRAC_PASSWORD`
-        environment variable, which overrides the above `password` field.
-        
-        Configuration Options
-        ^^^^^^^^^^^^^^^^^^^^^
-        Each section represent a site which can be selected using the ``-s``
-        command-line argument.  Within each section, the following settings are
-        available:
-        
-        - ``base_url`` - required, defines the URL of your Trac system
-        - ``auth_type`` - forces an authentication type, currently available: ``basic``
-          (default), ``digest``, ``acctmgr`` or ``none``.
-        - ``username`` - required if ``auth_type`` is not ``none``
-        - ``password`` - required if ``auth_type`` is not ``none``
-        - ``verify_ssl_cert`` - ignore self-signed or invalid SSL certificates if set
-          to false.
-        - ``editor`` - override the editor defined the ``$EDITOR`` environment
-          variable.
-        
-        
-        Command walk through
-        --------------------
-        
-        Report Listing and Search
-        ^^^^^^^^^^^^^^^^^^^^^^^^^
-        Dump a list of tickets on screen, without details::
-        
-            $ cm report 1
-            #142. fix world hunger (bjanin@)
-            #159. ignore unpaid rent (bjanin@)
-        
-        Another way to find ticket is using the search command::
-        
-            $ cm search dead mouse
-            #154. mickey
-        
-        Ticket View
-        ^^^^^^^^^^^
-        Show all the properties of a ticket::
-        
-            $ cm view 1
-        
-        List of Reports
-        ^^^^^^^^^^^^^^^
-        Get a list of all the available reports with::
-        
-            $ cm reports
-        
-        System Properties
-        ^^^^^^^^^^^^^^^^^
-        This will dump on screen all the Milestones, Components, Versions::
-        
-            $ cm properties
-        
-        Creating a ticket
-        ^^^^^^^^^^^^^^^^^
-        Creating a ticket will work similarly to writing a new email in mutt_, it loads
-        your current ``$EDITOR`` and lets you edit the details of the ticket. Assuming
-        all the parameters are correct, it will create the ticket as soon as you save
-        and exit and return the ticket number. If your ticket does not appear valid
-        (missing required field, inexistent Milestone, etc.) *cartman* will stop and
-        lists each error and let you return to your editor::
-        
-            $ cm new
-            -- opens your editor --
-        
-            Found the following errors:
-             - Invalid 'Subject': cannot be blank
-             - Invalid 'Milestone': expected: Bug Bucket, Release 2, Release 3
-        
-            -- Hit Enter to return to editor, ^C to abort --
-        
-        The first parameter to ``cm`` is the owner of the ticket, it populates the
-        ``To`` field by default::
-        
-            $ cm new jcarmack
-        
-        If your Trac has custom fields, you can use their identifier in the headers,
-        e.g.::
-        
-            story_id: 5123
-            iteration: 15
-        
-        If you specify a template with -t, cartman will look for a matching file in the
-        ``~/.cartman/templates`` folder and will use it as a base for your ticket::
-        
-            $ cm new -t sysadmin
-        
-        You can define a ``default`` template in this same directory in order to set
-        the template used by default (without ``-t``).
-        
-        Commenting on a ticket
-        ^^^^^^^^^^^^^^^^^^^^^^
-        Just like creating a ticket, adding a comment is just like mutt_, your current
-        ``$EDITOR`` will be loaded on a blank file for you to edit. Upon save and exit,
-        *cartman* will commit this new comment and return silently, unless an error
-        occurs::
-        
-            $ cm comment 1
-        
-        If the comment is short enough to fit on the command line, you may use the
-        ``-m`` flag as such::
-        
-            $ cm comment 1 -m "you forgot to call twiddle()"
-        
-        View/Set the status of a ticket
-        ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
-        View the current status of a ticket, and the available statuses::
-        
-            $ cm status 1
-        
-        Set a ticket as accepted::
-        
-            $ cm status 1 accept
-        
-        If you need to add a comment with this status change, you can use the ``-c``
-        flag, it will open your default editor::
-        
-            $ cm status 1 reopen -c
-        
-        You may also use the ``-m`` flag to define the comment in-line, without the use
-        of an editor::
-        
-            $ cm status 1 reopen -m "does not work with x = y"
-        
-        Advanced configuration
-        ----------------------
-        If you are using vim_ as your default editor, you also might want to add
-        email-like syntax highlighting to match the ``.cm.ticket`` extension::
-        
-            autocmd BufNewFile *.cm.ticket setf mail
-        
-        If you use multiple Trac sites, you can have multiple configurations in the
-        same file using the section to separate the sites, here is an example::
-        
-            [other]
-            base_url = http://other.trac.site/
-            username = tamentis
-            password = sitnemat
-            verify_ssl_cert = False
-        
-        
-        You would pass the ``-s`` parameter to ``cm`` to define which site to access::
-        
-            cm -s other report 1
-        
-        You may define all common configuration settings in the ``[DEFAULT]`` section.
-        
-        Using cartman without editor
-        ----------------------------
-        You may need to integrate cartman with other software where opening an editor
-        does not make sense.  In that case you can automatically create tickets from
-        a file using the ``--message-file`` option::
-        
-            cm new --message-file=secerror.txt
-        
-        This file would need to contain a complete ticket, if anything is missing,
-        cartman will exit with an error message.
-        
-        Installation
-        ------------
-        Quick and dirty if you are not familiar with Python packaging::
-        
-            sudo python setup.py install
-        
-        Requirements
-        ------------
-        - Python 2.7+, 3.3+ (not 3.2, not 2.6)
-        - python-requests 1.2 and above
-        
-        
-        Compatibility
-        -------------
-        - Tested on Trac 0.12.5 and 1.2.x
-        - Probably still works on 0.11, but untested.
-        
-        
-        Hacking
-        -------
-        - The following command will create one virtualenv and sandbox for each latest
-          0.12, 1.0 and 1.2 releases of Trac::
-        
-            $ ./tools/mkenv.sh
-        
-        - You can then serve one or the other using, the default admin user/pass is
-          sandbox/sandbox::
-        
-            $ ./tools/serve-0.12.sh
-            $ ./tools/serve-1.0.sh
-            $ ./tools/serve-1.2.sh
-        
-        - Follow PEP-8, existing style then the following notes.
-        - For dictionaries, lists: keep commas after each items, closing bracket
-          should close on the same column as the first letter of the statement with the
-          opening bracket.
-        - Use double-quotes for strings unless it makes it easier on certain strings
-          (avoids escaped double-quotes).
-        - If an error is exceptional, let the exception rise.
-        
-        
-        Distribute
-        ----------
-        - Change the version in cartman/__init__.py
-        - Commit
-        - Create a tag::
-        
-            git tag -a vX.Y.Z -m 'Releasing vX.Y.Z'
-            git push --tags
-        
-        - Download the file from github (release section),
-        - Sign it::
-        
-            gpg --armor --detach-sig cartman-X.Y.Z.tar.gz
-        
-        - Distribute on Pypi::
-        
-            python setup.py sdist upload
-        
-        
-        .. _Trac: http://trac.edgewall.org/
-        .. _vim: http://www.vim.org/
-        .. _mutt: http://www.mutt.org/
-        
-        
-        Changelog
-        =========
-        
-        0.3.0 (2020-03-14)
-        ------------------
-        - add new auth_type: acctmgr
-        - add new auth_type: none (for sites accepting anonymous tickets/comments)
-        - bump compatibility to 1.2.x
-        - remove warnings if you decided not to verify your SSL cert.
-        - use SafeConfigParser to allow variables interpolation (thanks to Sandro Santilli @strk)
-        - allow password to be provided by environment (thanks to Antoine Beaupré @anarcat)
-        
-        0.2.3 (2015-12-27)
-        ------------------
-        - add a configuration item to define the editor (by Nicolas Schodet <nico@ni.fr.eu.org>).
-        - fix the parsing of properties when one of them contains a semi-colon (thanks
-          to Josh Strange <josh@joshstrange.com>).
-        - fix property lookup (including option groups for milestone lookup on 1.0).
-        - add timeline command (thanks to Sandro Santilli @strk)
-        - allow to pass a fully formed message from the command line with --message-file
-        
-        0.2.2 (2013-09-01)
-        ------------------
-        - added ``search`` command.
-        - crash properly and early when trac return error 500.
-        - crash with a descriptive message when you lack permission to create a
-          ticket.
-        - don't die if the ``base_url`` has a trailing slash.
-        - test the existence of base_url instead of stack tracing.
-        - create the ~/.cartman/ directory by default.
-        - die with an error message if you don't have an $EDITOR env var.
-        - fix fetching current ticket status on v1.0+
-        
-        0.2.1 (2013-05-23)
-        ------------------
-        - added the ``default`` template,
-        - allow an owner to be specified, even with a template,
-        - added v1.0 compatibility,
-        - show Priority in ``cm properties``,
-        - fixed a bug lower-casing the properties after tokenized fuzzy match.
-        - fixed bug in ``view`` if the ticket contains unicode.
-        
-        0.2.0 (2013-05-03)
-        ------------------
-        - cm help now prints a list of commands (by goodwillcoding@webhippo.net),
-        - add auth_type to the config  (by goodwillcoding@webhippo.net),
-        - basic debianization (by Ryan P. Kelly <rpkelly@cpan.org>),
-        - added template support (in ~/.cartman/templates),
-        - document how to hack on this thing,
-        - move the configuration in a sub-directory,
-        - added option to skip SSL cert validation,
-        - added support for Trac 0.12,
-        - match single tokens during fuzzy find,
-        - python 3.3 support,
-        - transmit ticket body with CRLF end of lines.
-        
-        0.1.0 (2011-09-11)
-        ------------------
-        Initial release.
-        
-        
-Platform: UNKNOWN
+Project-URL: Homepage, https://tamentis.com/projects/cartman/
+Project-URL: Bug Tracker, https://github.com/tamentis/cartman/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: ISC License (ISCL)
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.3
+Classifier: Programming Language :: Python :: 3
 Classifier: Framework :: Trac
 Classifier: Topic :: Software Development :: Bug Tracking
+Requires-Python: >2.7,>=3.3
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+
+cartman
+=======
+
+.. image:: https://travis-ci.org/tamentis/cartman.png
+
+*cartman* allows you to create and manage your Trac_ tickets from the
+command-line, without the need to setup physical access to the Trac_
+installation/database or even the need to install a plugin on Trac_.  All you
+need is a Trac_ account.
+
+Examples
+--------
+Create a new ticket, that will open your $EDITOR::
+
+    $ cm new
+
+View the content of a ticket::
+
+    $ cm view 1514
+
+Configuration
+-------------
+At a minimum you need to create a ``~/.cartman/config`` file with the
+following::
+
+    [trac]
+    base_url = http://your.trac.install/
+    username = tamentis
+    password = sitnemat
+
+The password can also be specified through a `TRAC_PASSWORD`
+environment variable, which overrides the above `password` field.
+
+Configuration Options
+^^^^^^^^^^^^^^^^^^^^^
+Each section represent a site which can be selected using the ``-s``
+command-line argument.  Within each section, the following settings are
+available:
+
+- ``base_url`` - required, defines the URL of your Trac system
+- ``auth_type`` - forces an authentication type, currently available: ``basic``
+  (default), ``digest``, ``acctmgr`` or ``none``.
+- ``username`` - required if ``auth_type`` is not ``none``
+- ``password`` - required if ``auth_type`` is not ``none``
+- ``verify_ssl_cert`` - ignore self-signed or invalid SSL certificates if set
+  to false.
+- ``editor`` - override the editor defined the ``$EDITOR`` environment
+  variable.
+
+
+Command walk through
+--------------------
+
+Report Listing and Search
+^^^^^^^^^^^^^^^^^^^^^^^^^
+Dump a list of tickets on screen, without details::
+
+    $ cm report 1
+    #142. fix world hunger (bjanin@)
+    #159. ignore unpaid rent (bjanin@)
+
+Another way to find ticket is using the search command::
+
+    $ cm search dead mouse
+    #154. mickey
+
+Ticket View
+^^^^^^^^^^^
+Show all the properties of a ticket::
+
+    $ cm view 1
+
+List of Reports
+^^^^^^^^^^^^^^^
+Get a list of all the available reports with::
+
+    $ cm reports
+
+System Properties
+^^^^^^^^^^^^^^^^^
+This will dump on screen all the Milestones, Components, Versions::
+
+    $ cm properties
+
+Creating a ticket
+^^^^^^^^^^^^^^^^^
+Creating a ticket will work similarly to writing a new email in mutt_, it loads
+your current ``$EDITOR`` and lets you edit the details of the ticket. Assuming
+all the parameters are correct, it will create the ticket as soon as you save
+and exit and return the ticket number. If your ticket does not appear valid
+(missing required field, inexistent Milestone, etc.) *cartman* will stop and
+lists each error and let you return to your editor::
+
+    $ cm new
+    -- opens your editor --
+
+    Found the following errors:
+     - Invalid 'Subject': cannot be blank
+     - Invalid 'Milestone': expected: Bug Bucket, Release 2, Release 3
+
+    -- Hit Enter to return to editor, ^C to abort --
+
+The first parameter to ``cm`` is the owner of the ticket, it populates the
+``To`` field by default::
+
+    $ cm new jcarmack
+
+If your Trac has custom fields, you can use their identifier in the headers,
+e.g.::
+
+    story_id: 5123
+    iteration: 15
+
+If you specify a template with -t, cartman will look for a matching file in the
+``~/.cartman/templates`` folder and will use it as a base for your ticket::
+
+    $ cm new -t sysadmin
+
+You can define a ``default`` template in this same directory in order to set
+the template used by default (without ``-t``).
+
+Commenting on a ticket
+^^^^^^^^^^^^^^^^^^^^^^
+Just like creating a ticket, adding a comment is just like mutt_, your current
+``$EDITOR`` will be loaded on a blank file for you to edit. Upon save and exit,
+*cartman* will commit this new comment and return silently, unless an error
+occurs::
+
+    $ cm comment 1
+
+If the comment is short enough to fit on the command line, you may use the
+``-m`` flag as such::
+
+    $ cm comment 1 -m "you forgot to call twiddle()"
+
+View/Set the status of a ticket
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+View the current status of a ticket, and the available statuses::
+
+    $ cm status 1
+
+Set a ticket as accepted::
+
+    $ cm status 1 accept
+
+If you need to add a comment with this status change, you can use the ``-c``
+flag, it will open your default editor::
+
+    $ cm status 1 reopen -c
+
+You may also use the ``-m`` flag to define the comment in-line, without the use
+of an editor::
+
+    $ cm status 1 reopen -m "does not work with x = y"
+
+Advanced configuration
+----------------------
+If you are using vim_ as your default editor, you also might want to add
+email-like syntax highlighting to match the ``.cm.ticket`` extension::
+
+    autocmd BufNewFile *.cm.ticket setf mail
+
+If you use multiple Trac sites, you can have multiple configurations in the
+same file using the section to separate the sites, here is an example::
+
+    [other]
+    base_url = http://other.trac.site/
+    username = tamentis
+    password = sitnemat
+    verify_ssl_cert = False
+
+
+You would pass the ``-s`` parameter to ``cm`` to define which site to access::
+
+    cm -s other report 1
+
+You may define all common configuration settings in the ``[DEFAULT]`` section.
+
+Using cartman without editor
+----------------------------
+You may need to integrate cartman with other software where opening an editor
+does not make sense.  In that case you can automatically create tickets from
+a file using the ``--message-file`` option::
+
+    cm new --message-file=secerror.txt
+
+This file would need to contain a complete ticket, if anything is missing,
+cartman will exit with an error message.
+
+Installation
+------------
+Quick and dirty if you are not familiar with Python packaging::
+
+    sudo python setup.py install
+
+Requirements
+------------
+- Python 2.7+, 3.3+ (not 3.2, not 2.6)
+- python-requests 1.2 and above
+
+
+Compatibility
+-------------
+- Tested on Trac 0.12.5 and 1.2.x
+- Probably still works on 0.11, but untested.
+
+
+Hacking
+-------
+- The following command will create one virtualenv and sandbox for each latest
+  0.12, 1.0 and 1.2 releases of Trac::
+
+    $ ./tools/mkenv.sh
+
+- You can then serve one or the other using, the default admin user/pass is
+  sandbox/sandbox::
+
+    $ ./tools/serve-0.12.sh
+    $ ./tools/serve-1.0.sh
+    $ ./tools/serve-1.2.sh
+
+- Follow PEP-8, existing style then the following notes.
+- For dictionaries, lists: keep commas after each items, closing bracket
+  should close on the same column as the first letter of the statement with the
+  opening bracket.
+- Use double-quotes for strings unless it makes it easier on certain strings
+  (avoids escaped double-quotes).
+- If an error is exceptional, let the exception rise.
+
+
+Distribute
+----------
+- Change the version in cartman/__init__.py, update CHANGES.txt
+- Commit
+- Create a tag::
+
+    git tag -a vX.Y.Z -m 'Releasing vX.Y.Z'
+    git push --tags
+
+- Download the file from github (release section),
+- Sign it::
+
+    gpg --armor --detach-sig cartman-X.Y.Z.tar.gz
+
+- Distribute on Pypi::
+
+    python setup.py sdist upload
+
+
+.. _Trac: http://trac.edgewall.org/
+.. _vim: http://www.vim.org/
+.. _mutt: http://www.mutt.org/
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `cartman-0.3.0/cartman.egg-info/PKG-INFO` & `cartman-0.3.1/cartman.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,336 +1,278 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: cartman
-Version: 0.3.0
+Version: 0.3.1
 Summary: trac command-line tools
 Home-page: http://tamentis.com/projects/cartman/
 Author: Bertrand Janin
-Author-email: b@janin.com
+Author-email: Bertrand Janin <bertrand@janin.com>
 License: ISC License (ISCL, BSD/MIT compatible)
-Description: cartman
-        =======
-        
-        .. image:: https://travis-ci.org/tamentis/cartman.png
-        
-        *cartman* allows you to create and manage your Trac_ tickets from the
-        command-line, without the need to setup physical access to the Trac_
-        installation/database or even the need to install a plugin on Trac_.  All you
-        need is a Trac_ account.
-        
-        Examples
-        --------
-        Create a new ticket, that will open your $EDITOR::
-        
-            $ cm new
-        
-        View the content of a ticket::
-        
-            $ cm view 1514
-        
-        Configuration
-        -------------
-        At a minimum you need to create a ``~/.cartman/config`` file with the
-        following::
-        
-            [trac]
-            base_url = http://your.trac.install/
-            username = tamentis
-            password = sitnemat
-        
-        The password can also be specified through a `TRAC_PASSWORD`
-        environment variable, which overrides the above `password` field.
-        
-        Configuration Options
-        ^^^^^^^^^^^^^^^^^^^^^
-        Each section represent a site which can be selected using the ``-s``
-        command-line argument.  Within each section, the following settings are
-        available:
-        
-        - ``base_url`` - required, defines the URL of your Trac system
-        - ``auth_type`` - forces an authentication type, currently available: ``basic``
-          (default), ``digest``, ``acctmgr`` or ``none``.
-        - ``username`` - required if ``auth_type`` is not ``none``
-        - ``password`` - required if ``auth_type`` is not ``none``
-        - ``verify_ssl_cert`` - ignore self-signed or invalid SSL certificates if set
-          to false.
-        - ``editor`` - override the editor defined the ``$EDITOR`` environment
-          variable.
-        
-        
-        Command walk through
-        --------------------
-        
-        Report Listing and Search
-        ^^^^^^^^^^^^^^^^^^^^^^^^^
-        Dump a list of tickets on screen, without details::
-        
-            $ cm report 1
-            #142. fix world hunger (bjanin@)
-            #159. ignore unpaid rent (bjanin@)
-        
-        Another way to find ticket is using the search command::
-        
-            $ cm search dead mouse
-            #154. mickey
-        
-        Ticket View
-        ^^^^^^^^^^^
-        Show all the properties of a ticket::
-        
-            $ cm view 1
-        
-        List of Reports
-        ^^^^^^^^^^^^^^^
-        Get a list of all the available reports with::
-        
-            $ cm reports
-        
-        System Properties
-        ^^^^^^^^^^^^^^^^^
-        This will dump on screen all the Milestones, Components, Versions::
-        
-            $ cm properties
-        
-        Creating a ticket
-        ^^^^^^^^^^^^^^^^^
-        Creating a ticket will work similarly to writing a new email in mutt_, it loads
-        your current ``$EDITOR`` and lets you edit the details of the ticket. Assuming
-        all the parameters are correct, it will create the ticket as soon as you save
-        and exit and return the ticket number. If your ticket does not appear valid
-        (missing required field, inexistent Milestone, etc.) *cartman* will stop and
-        lists each error and let you return to your editor::
-        
-            $ cm new
-            -- opens your editor --
-        
-            Found the following errors:
-             - Invalid 'Subject': cannot be blank
-             - Invalid 'Milestone': expected: Bug Bucket, Release 2, Release 3
-        
-            -- Hit Enter to return to editor, ^C to abort --
-        
-        The first parameter to ``cm`` is the owner of the ticket, it populates the
-        ``To`` field by default::
-        
-            $ cm new jcarmack
-        
-        If your Trac has custom fields, you can use their identifier in the headers,
-        e.g.::
-        
-            story_id: 5123
-            iteration: 15
-        
-        If you specify a template with -t, cartman will look for a matching file in the
-        ``~/.cartman/templates`` folder and will use it as a base for your ticket::
-        
-            $ cm new -t sysadmin
-        
-        You can define a ``default`` template in this same directory in order to set
-        the template used by default (without ``-t``).
-        
-        Commenting on a ticket
-        ^^^^^^^^^^^^^^^^^^^^^^
-        Just like creating a ticket, adding a comment is just like mutt_, your current
-        ``$EDITOR`` will be loaded on a blank file for you to edit. Upon save and exit,
-        *cartman* will commit this new comment and return silently, unless an error
-        occurs::
-        
-            $ cm comment 1
-        
-        If the comment is short enough to fit on the command line, you may use the
-        ``-m`` flag as such::
-        
-            $ cm comment 1 -m "you forgot to call twiddle()"
-        
-        View/Set the status of a ticket
-        ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
-        View the current status of a ticket, and the available statuses::
-        
-            $ cm status 1
-        
-        Set a ticket as accepted::
-        
-            $ cm status 1 accept
-        
-        If you need to add a comment with this status change, you can use the ``-c``
-        flag, it will open your default editor::
-        
-            $ cm status 1 reopen -c
-        
-        You may also use the ``-m`` flag to define the comment in-line, without the use
-        of an editor::
-        
-            $ cm status 1 reopen -m "does not work with x = y"
-        
-        Advanced configuration
-        ----------------------
-        If you are using vim_ as your default editor, you also might want to add
-        email-like syntax highlighting to match the ``.cm.ticket`` extension::
-        
-            autocmd BufNewFile *.cm.ticket setf mail
-        
-        If you use multiple Trac sites, you can have multiple configurations in the
-        same file using the section to separate the sites, here is an example::
-        
-            [other]
-            base_url = http://other.trac.site/
-            username = tamentis
-            password = sitnemat
-            verify_ssl_cert = False
-        
-        
-        You would pass the ``-s`` parameter to ``cm`` to define which site to access::
-        
-            cm -s other report 1
-        
-        You may define all common configuration settings in the ``[DEFAULT]`` section.
-        
-        Using cartman without editor
-        ----------------------------
-        You may need to integrate cartman with other software where opening an editor
-        does not make sense.  In that case you can automatically create tickets from
-        a file using the ``--message-file`` option::
-        
-            cm new --message-file=secerror.txt
-        
-        This file would need to contain a complete ticket, if anything is missing,
-        cartman will exit with an error message.
-        
-        Installation
-        ------------
-        Quick and dirty if you are not familiar with Python packaging::
-        
-            sudo python setup.py install
-        
-        Requirements
-        ------------
-        - Python 2.7+, 3.3+ (not 3.2, not 2.6)
-        - python-requests 1.2 and above
-        
-        
-        Compatibility
-        -------------
-        - Tested on Trac 0.12.5 and 1.2.x
-        - Probably still works on 0.11, but untested.
-        
-        
-        Hacking
-        -------
-        - The following command will create one virtualenv and sandbox for each latest
-          0.12, 1.0 and 1.2 releases of Trac::
-        
-            $ ./tools/mkenv.sh
-        
-        - You can then serve one or the other using, the default admin user/pass is
-          sandbox/sandbox::
-        
-            $ ./tools/serve-0.12.sh
-            $ ./tools/serve-1.0.sh
-            $ ./tools/serve-1.2.sh
-        
-        - Follow PEP-8, existing style then the following notes.
-        - For dictionaries, lists: keep commas after each items, closing bracket
-          should close on the same column as the first letter of the statement with the
-          opening bracket.
-        - Use double-quotes for strings unless it makes it easier on certain strings
-          (avoids escaped double-quotes).
-        - If an error is exceptional, let the exception rise.
-        
-        
-        Distribute
-        ----------
-        - Change the version in cartman/__init__.py
-        - Commit
-        - Create a tag::
-        
-            git tag -a vX.Y.Z -m 'Releasing vX.Y.Z'
-            git push --tags
-        
-        - Download the file from github (release section),
-        - Sign it::
-        
-            gpg --armor --detach-sig cartman-X.Y.Z.tar.gz
-        
-        - Distribute on Pypi::
-        
-            python setup.py sdist upload
-        
-        
-        .. _Trac: http://trac.edgewall.org/
-        .. _vim: http://www.vim.org/
-        .. _mutt: http://www.mutt.org/
-        
-        
-        Changelog
-        =========
-        
-        0.3.0 (2020-03-14)
-        ------------------
-        - add new auth_type: acctmgr
-        - add new auth_type: none (for sites accepting anonymous tickets/comments)
-        - bump compatibility to 1.2.x
-        - remove warnings if you decided not to verify your SSL cert.
-        - use SafeConfigParser to allow variables interpolation (thanks to Sandro Santilli @strk)
-        - allow password to be provided by environment (thanks to Antoine Beaupré @anarcat)
-        
-        0.2.3 (2015-12-27)
-        ------------------
-        - add a configuration item to define the editor (by Nicolas Schodet <nico@ni.fr.eu.org>).
-        - fix the parsing of properties when one of them contains a semi-colon (thanks
-          to Josh Strange <josh@joshstrange.com>).
-        - fix property lookup (including option groups for milestone lookup on 1.0).
-        - add timeline command (thanks to Sandro Santilli @strk)
-        - allow to pass a fully formed message from the command line with --message-file
-        
-        0.2.2 (2013-09-01)
-        ------------------
-        - added ``search`` command.
-        - crash properly and early when trac return error 500.
-        - crash with a descriptive message when you lack permission to create a
-          ticket.
-        - don't die if the ``base_url`` has a trailing slash.
-        - test the existence of base_url instead of stack tracing.
-        - create the ~/.cartman/ directory by default.
-        - die with an error message if you don't have an $EDITOR env var.
-        - fix fetching current ticket status on v1.0+
-        
-        0.2.1 (2013-05-23)
-        ------------------
-        - added the ``default`` template,
-        - allow an owner to be specified, even with a template,
-        - added v1.0 compatibility,
-        - show Priority in ``cm properties``,
-        - fixed a bug lower-casing the properties after tokenized fuzzy match.
-        - fixed bug in ``view`` if the ticket contains unicode.
-        
-        0.2.0 (2013-05-03)
-        ------------------
-        - cm help now prints a list of commands (by goodwillcoding@webhippo.net),
-        - add auth_type to the config  (by goodwillcoding@webhippo.net),
-        - basic debianization (by Ryan P. Kelly <rpkelly@cpan.org>),
-        - added template support (in ~/.cartman/templates),
-        - document how to hack on this thing,
-        - move the configuration in a sub-directory,
-        - added option to skip SSL cert validation,
-        - added support for Trac 0.12,
-        - match single tokens during fuzzy find,
-        - python 3.3 support,
-        - transmit ticket body with CRLF end of lines.
-        
-        0.1.0 (2011-09-11)
-        ------------------
-        Initial release.
-        
-        
-Platform: UNKNOWN
+Project-URL: Homepage, https://tamentis.com/projects/cartman/
+Project-URL: Bug Tracker, https://github.com/tamentis/cartman/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: ISC License (ISCL)
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.3
+Classifier: Programming Language :: Python :: 3
 Classifier: Framework :: Trac
 Classifier: Topic :: Software Development :: Bug Tracking
+Requires-Python: >2.7,>=3.3
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+
+cartman
+=======
+
+.. image:: https://travis-ci.org/tamentis/cartman.png
+
+*cartman* allows you to create and manage your Trac_ tickets from the
+command-line, without the need to setup physical access to the Trac_
+installation/database or even the need to install a plugin on Trac_.  All you
+need is a Trac_ account.
+
+Examples
+--------
+Create a new ticket, that will open your $EDITOR::
+
+    $ cm new
+
+View the content of a ticket::
+
+    $ cm view 1514
+
+Configuration
+-------------
+At a minimum you need to create a ``~/.cartman/config`` file with the
+following::
+
+    [trac]
+    base_url = http://your.trac.install/
+    username = tamentis
+    password = sitnemat
+
+The password can also be specified through a `TRAC_PASSWORD`
+environment variable, which overrides the above `password` field.
+
+Configuration Options
+^^^^^^^^^^^^^^^^^^^^^
+Each section represent a site which can be selected using the ``-s``
+command-line argument.  Within each section, the following settings are
+available:
+
+- ``base_url`` - required, defines the URL of your Trac system
+- ``auth_type`` - forces an authentication type, currently available: ``basic``
+  (default), ``digest``, ``acctmgr`` or ``none``.
+- ``username`` - required if ``auth_type`` is not ``none``
+- ``password`` - required if ``auth_type`` is not ``none``
+- ``verify_ssl_cert`` - ignore self-signed or invalid SSL certificates if set
+  to false.
+- ``editor`` - override the editor defined the ``$EDITOR`` environment
+  variable.
+
+
+Command walk through
+--------------------
+
+Report Listing and Search
+^^^^^^^^^^^^^^^^^^^^^^^^^
+Dump a list of tickets on screen, without details::
+
+    $ cm report 1
+    #142. fix world hunger (bjanin@)
+    #159. ignore unpaid rent (bjanin@)
+
+Another way to find ticket is using the search command::
+
+    $ cm search dead mouse
+    #154. mickey
+
+Ticket View
+^^^^^^^^^^^
+Show all the properties of a ticket::
+
+    $ cm view 1
+
+List of Reports
+^^^^^^^^^^^^^^^
+Get a list of all the available reports with::
+
+    $ cm reports
+
+System Properties
+^^^^^^^^^^^^^^^^^
+This will dump on screen all the Milestones, Components, Versions::
+
+    $ cm properties
+
+Creating a ticket
+^^^^^^^^^^^^^^^^^
+Creating a ticket will work similarly to writing a new email in mutt_, it loads
+your current ``$EDITOR`` and lets you edit the details of the ticket. Assuming
+all the parameters are correct, it will create the ticket as soon as you save
+and exit and return the ticket number. If your ticket does not appear valid
+(missing required field, inexistent Milestone, etc.) *cartman* will stop and
+lists each error and let you return to your editor::
+
+    $ cm new
+    -- opens your editor --
+
+    Found the following errors:
+     - Invalid 'Subject': cannot be blank
+     - Invalid 'Milestone': expected: Bug Bucket, Release 2, Release 3
+
+    -- Hit Enter to return to editor, ^C to abort --
+
+The first parameter to ``cm`` is the owner of the ticket, it populates the
+``To`` field by default::
+
+    $ cm new jcarmack
+
+If your Trac has custom fields, you can use their identifier in the headers,
+e.g.::
+
+    story_id: 5123
+    iteration: 15
+
+If you specify a template with -t, cartman will look for a matching file in the
+``~/.cartman/templates`` folder and will use it as a base for your ticket::
+
+    $ cm new -t sysadmin
+
+You can define a ``default`` template in this same directory in order to set
+the template used by default (without ``-t``).
+
+Commenting on a ticket
+^^^^^^^^^^^^^^^^^^^^^^
+Just like creating a ticket, adding a comment is just like mutt_, your current
+``$EDITOR`` will be loaded on a blank file for you to edit. Upon save and exit,
+*cartman* will commit this new comment and return silently, unless an error
+occurs::
+
+    $ cm comment 1
+
+If the comment is short enough to fit on the command line, you may use the
+``-m`` flag as such::
+
+    $ cm comment 1 -m "you forgot to call twiddle()"
+
+View/Set the status of a ticket
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+View the current status of a ticket, and the available statuses::
+
+    $ cm status 1
+
+Set a ticket as accepted::
+
+    $ cm status 1 accept
+
+If you need to add a comment with this status change, you can use the ``-c``
+flag, it will open your default editor::
+
+    $ cm status 1 reopen -c
+
+You may also use the ``-m`` flag to define the comment in-line, without the use
+of an editor::
+
+    $ cm status 1 reopen -m "does not work with x = y"
+
+Advanced configuration
+----------------------
+If you are using vim_ as your default editor, you also might want to add
+email-like syntax highlighting to match the ``.cm.ticket`` extension::
+
+    autocmd BufNewFile *.cm.ticket setf mail
+
+If you use multiple Trac sites, you can have multiple configurations in the
+same file using the section to separate the sites, here is an example::
+
+    [other]
+    base_url = http://other.trac.site/
+    username = tamentis
+    password = sitnemat
+    verify_ssl_cert = False
+
+
+You would pass the ``-s`` parameter to ``cm`` to define which site to access::
+
+    cm -s other report 1
+
+You may define all common configuration settings in the ``[DEFAULT]`` section.
+
+Using cartman without editor
+----------------------------
+You may need to integrate cartman with other software where opening an editor
+does not make sense.  In that case you can automatically create tickets from
+a file using the ``--message-file`` option::
+
+    cm new --message-file=secerror.txt
+
+This file would need to contain a complete ticket, if anything is missing,
+cartman will exit with an error message.
+
+Installation
+------------
+Quick and dirty if you are not familiar with Python packaging::
+
+    sudo python setup.py install
+
+Requirements
+------------
+- Python 2.7+, 3.3+ (not 3.2, not 2.6)
+- python-requests 1.2 and above
+
+
+Compatibility
+-------------
+- Tested on Trac 0.12.5 and 1.2.x
+- Probably still works on 0.11, but untested.
+
+
+Hacking
+-------
+- The following command will create one virtualenv and sandbox for each latest
+  0.12, 1.0 and 1.2 releases of Trac::
+
+    $ ./tools/mkenv.sh
+
+- You can then serve one or the other using, the default admin user/pass is
+  sandbox/sandbox::
+
+    $ ./tools/serve-0.12.sh
+    $ ./tools/serve-1.0.sh
+    $ ./tools/serve-1.2.sh
+
+- Follow PEP-8, existing style then the following notes.
+- For dictionaries, lists: keep commas after each items, closing bracket
+  should close on the same column as the first letter of the statement with the
+  opening bracket.
+- Use double-quotes for strings unless it makes it easier on certain strings
+  (avoids escaped double-quotes).
+- If an error is exceptional, let the exception rise.
+
+
+Distribute
+----------
+- Change the version in cartman/__init__.py, update CHANGES.txt
+- Commit
+- Create a tag::
+
+    git tag -a vX.Y.Z -m 'Releasing vX.Y.Z'
+    git push --tags
+
+- Download the file from github (release section),
+- Sign it::
+
+    gpg --armor --detach-sig cartman-X.Y.Z.tar.gz
+
+- Distribute on Pypi::
+
+    python setup.py sdist upload
+
+
+.. _Trac: http://trac.edgewall.org/
+.. _vim: http://www.vim.org/
+.. _mutt: http://www.mutt.org/
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `cartman-0.3.0/cartman/ticket.py` & `cartman-0.3.1/cartman/ticket.py`

 * *Files identical despite different names*

### Comparing `cartman-0.3.0/cartman/compat.py` & `cartman-0.3.1/cartman/compat.py`

 * *Files identical despite different names*

### Comparing `cartman-0.3.0/cartman/ui.py` & `cartman-0.3.1/cartman/ui.py`

 * *Files identical despite different names*

### Comparing `cartman-0.3.0/cartman/__init__.py` & `cartman-0.3.1/cartman/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-# Copyright (c) 2011-2020 Bertrand Janin <b@janin.com>
+# Copyright (c) 2011-2023 Bertrand Janin <b@janin.com>
 #
 # Permission to use, copy, modify, and/or distribute this software for any
 # purpose with or without fee is hereby granted, provided that the above
 # copyright notice and this permission notice appear in all copies.
 #
 # THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES
 # WITH REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF
 # MERCHANTABILITY AND FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR
 # ANY SPECIAL, DIRECT, INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES
 # WHATSOEVER RESULTING FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN
 # ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT OF
 # OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
 
-__version__ = "0.3.0"
+__version__ = "0.3.1"
```

### Comparing `cartman-0.3.0/cartman/text.py` & `cartman-0.3.1/cartman/text.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,15 +93,15 @@
 def extract_timestamps_common(token, raw_html):
     """Given a dump of HTML data, extract the timestamp and return it as a
     string value.
 
     :param raw_html: Dump from the ticket page.
 
     """
-    regex = r"""name="{}" value="([^"]+)""".format(token)
+    regex = r"""name="{}"\s*value="([^"]+)""".format(token)
 
     m = re.search(regex, raw_html, re.MULTILINE)
 
     if m:
         timestamp = m.group(1)
     else:
         raise exceptions.FatalError("unable to fetch timestamp")
```

### Comparing `cartman-0.3.0/cartman/app.py` & `cartman-0.3.1/cartman/app.py`

 * *Files identical despite different names*

### Comparing `cartman-0.3.0/cartman/exceptions.py` & `cartman-0.3.1/cartman/exceptions.py`

 * *Files identical despite different names*

### Comparing `cartman-0.3.0/setup.py` & `cartman-0.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `cartman-0.3.0/cm` & `cartman-0.3.1/cm`

 * *Files identical despite different names*

### Comparing `cartman-0.3.0/README.rst` & `cartman-0.3.1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -226,15 +226,15 @@
 - Use double-quotes for strings unless it makes it easier on certain strings
   (avoids escaped double-quotes).
 - If an error is exceptional, let the exception rise.
 
 
 Distribute
 ----------
-- Change the version in cartman/__init__.py
+- Change the version in cartman/__init__.py, update CHANGES.txt
 - Commit
 - Create a tag::
 
     git tag -a vX.Y.Z -m 'Releasing vX.Y.Z'
     git push --tags
 
 - Download the file from github (release section),
```

