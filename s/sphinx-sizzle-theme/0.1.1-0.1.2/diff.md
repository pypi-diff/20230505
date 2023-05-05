# Comparing `tmp/sphinx_sizzle_theme-0.1.1.tar.gz` & `tmp/sphinx_sizzle_theme-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sphinx_sizzle_theme-0.1.1.tar", last modified: Tue May  3 15:20:46 2022, max compression
+gzip compressed data, was "/home/vinay/projects/sphinx_sizzle_theme/dist/tmp1d95_tg1/sphinx_sizzle_theme-0.1.2.tar", last modified: Fri May  5 10:29:51 2023, max compression
```

## Comparing `sphinx_sizzle_theme-0.1.1.tar` & `sphinx_sizzle_theme-0.1.2.tar`

### file list

```diff
@@ -1,35 +1,36 @@
-drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2022-05-03 15:20:46.000000 sphinx_sizzle_theme-0.1.1/
--rw-rw-r--   0 vinay     (1000) vinay     (1000)      206 2019-05-10 15:28:32.000000 sphinx_sizzle_theme-0.1.1/MANIFEST.in
-drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2022-05-03 15:20:46.000000 sphinx_sizzle_theme-0.1.1/sphinx_sizzle_theme/
--rw-rw-r--   0 vinay     (1000) vinay     (1000)    20555 2022-05-03 15:12:59.000000 sphinx_sizzle_theme-0.1.1/sphinx_sizzle_theme/__init__.py
--rw-rw-r--   0 vinay     (1000) vinay     (1000)     2095 2019-04-05 19:27:51.000000 sphinx_sizzle_theme-0.1.1/sphinx_sizzle_theme/genindex.html
--rw-rw-r--   0 vinay     (1000) vinay     (1000)      225 2019-05-13 14:19:52.000000 sphinx_sizzle_theme-0.1.1/sphinx_sizzle_theme/logo-text.html
--rw-r--r--   0 vinay     (1000) vinay     (1000)    24135 2022-04-29 14:53:47.000000 sphinx_sizzle_theme-0.1.1/sphinx_sizzle_theme/sizzle.scss
--rw-r--r--   0 vinay     (1000) vinay     (1000)       36 2022-05-03 15:20:17.000000 sphinx_sizzle_theme-0.1.1/sphinx_sizzle_theme/version.txt
-drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2022-05-03 15:20:46.000000 sphinx_sizzle_theme-0.1.1/sphinx_sizzle_theme/static/
-drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2022-05-03 15:20:46.000000 sphinx_sizzle_theme-0.1.1/sphinx_sizzle_theme/static/css/
--rw-r--r--   0 vinay     (1000) vinay     (1000)    24741 2022-04-29 14:53:48.000000 sphinx_sizzle_theme-0.1.1/sphinx_sizzle_theme/static/css/sizzle.css
--rw-rw-r--   0 vinay     (1000) vinay     (1000)     1558 2022-05-03 14:40:26.000000 sphinx_sizzle_theme-0.1.1/sphinx_sizzle_theme/search.html
--rw-rw-r--   0 vinay     (1000) vinay     (1000)    18722 2022-05-03 14:55:09.000000 sphinx_sizzle_theme-0.1.1/sphinx_sizzle_theme/layout.html
--rw-rw-r--   0 vinay     (1000) vinay     (1000)      574 2019-05-09 14:30:39.000000 sphinx_sizzle_theme-0.1.1/README.rst
--rw-rw-r--   0 vinay     (1000) vinay     (1000)       67 2022-05-03 15:20:46.000000 sphinx_sizzle_theme-0.1.1/setup.cfg
--rw-rw-r--   0 vinay     (1000) vinay     (1000)     2417 2019-04-07 18:45:31.000000 sphinx_sizzle_theme-0.1.1/LICENSE
-drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2022-05-03 15:20:46.000000 sphinx_sizzle_theme-0.1.1/docs/
--rw-r--r--   0 vinay     (1000) vinay     (1000)      810 2019-04-12 06:44:40.000000 sphinx_sizzle_theme-0.1.1/docs/make.bat
--rw-r--r--   0 vinay     (1000) vinay     (1000)       11 2019-05-09 06:33:17.000000 sphinx_sizzle_theme-0.1.1/docs/.dict-validwords
-drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2022-05-03 15:20:46.000000 sphinx_sizzle_theme-0.1.1/docs/_static/
-drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2022-05-03 15:20:46.000000 sphinx_sizzle_theme-0.1.1/docs/_static/img/
--rw-r--r--   0 vinay     (1000) vinay     (1000)     2696 2019-04-12 19:22:47.000000 sphinx_sizzle_theme-0.1.1/docs/_static/img/ff-open.png
--rw-r--r--   0 vinay     (1000) vinay     (1000)     2315 2019-04-12 19:22:56.000000 sphinx_sizzle_theme-0.1.1/docs/_static/img/chrome-closed.png
--rw-rw-r--   0 vinay     (1000) vinay     (1000)    36939 2019-05-10 15:06:59.000000 sphinx_sizzle_theme-0.1.1/docs/_static/img/mobile_1.png
--rw-r--r--   0 vinay     (1000) vinay     (1000)     3383 2019-04-12 19:22:56.000000 sphinx_sizzle_theme-0.1.1/docs/_static/img/chrome-open.png
--rw-rw-r--   0 vinay     (1000) vinay     (1000)    36013 2019-05-10 15:07:10.000000 sphinx_sizzle_theme-0.1.1/docs/_static/img/mobile_2.png
--rw-r--r--   0 vinay     (1000) vinay     (1000)     1969 2019-04-12 19:22:47.000000 sphinx_sizzle_theme-0.1.1/docs/_static/img/ff-closed.png
--rw-rw-r--   0 vinay     (1000) vinay     (1000)    27144 2022-05-03 14:56:27.000000 sphinx_sizzle_theme-0.1.1/docs/index.rst
--rw-r--r--   0 vinay     (1000) vinay     (1000)      603 2019-04-12 06:44:40.000000 sphinx_sizzle_theme-0.1.1/docs/Makefile
--rw-r--r--   0 vinay     (1000) vinay     (1000)     5881 2021-12-17 19:21:27.000000 sphinx_sizzle_theme-0.1.1/docs/conf.py
--rw-rw-r--   0 vinay     (1000) vinay     (1000)     1720 2022-05-02 08:06:13.000000 sphinx_sizzle_theme-0.1.1/setup.py
--rw-rw-r--   0 vinay     (1000) vinay     (1000)     1831 2022-05-03 15:20:46.000000 sphinx_sizzle_theme-0.1.1/PKG-INFO
-drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2022-05-03 15:20:46.000000 sphinx_sizzle_theme-0.1.1/sphinx_sizzle_theme.egg-info/
--rw-r--r--   0 vinay     (1000) vinay     (1000)      595 2022-05-03 15:20:46.000000 sphinx_sizzle_theme-0.1.1/sphinx_sizzle_theme.egg-info/SOURCES.txt
--rw-r--r--   0 vinay     (1000) vinay     (1000)      150 2019-04-09 12:21:53.000000 sphinx_sizzle_theme-0.1.1/Makefile
+drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-05-05 10:29:51.000000 sphinx_sizzle_theme-0.1.2/
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)      206 2019-05-10 15:28:32.000000 sphinx_sizzle_theme-0.1.2/MANIFEST.in
+drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-05-05 10:29:51.000000 sphinx_sizzle_theme-0.1.2/sphinx_sizzle_theme/
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)    22687 2023-05-05 10:25:00.000000 sphinx_sizzle_theme-0.1.2/sphinx_sizzle_theme/__init__.py
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)     2095 2019-04-05 19:27:51.000000 sphinx_sizzle_theme-0.1.2/sphinx_sizzle_theme/genindex.html
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)      225 2019-05-13 14:19:52.000000 sphinx_sizzle_theme-0.1.2/sphinx_sizzle_theme/logo-text.html
+-rw-r--r--   0 vinay     (1000) vinay     (1000)    24702 2022-11-12 14:35:23.000000 sphinx_sizzle_theme-0.1.2/sphinx_sizzle_theme/sizzle.scss
+-rw-r--r--   0 vinay     (1000) vinay     (1000)       36 2023-05-05 10:28:10.000000 sphinx_sizzle_theme-0.1.2/sphinx_sizzle_theme/version.txt
+drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-05-05 10:29:51.000000 sphinx_sizzle_theme-0.1.2/sphinx_sizzle_theme/static/
+drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-05-05 10:29:51.000000 sphinx_sizzle_theme-0.1.2/sphinx_sizzle_theme/static/css/
+-rw-r--r--   0 vinay     (1000) vinay     (1000)    25377 2022-11-12 14:35:31.000000 sphinx_sizzle_theme-0.1.2/sphinx_sizzle_theme/static/css/sizzle.css
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)     1558 2022-05-03 14:40:26.000000 sphinx_sizzle_theme-0.1.2/sphinx_sizzle_theme/search.html
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)    20281 2023-05-05 09:25:43.000000 sphinx_sizzle_theme-0.1.2/sphinx_sizzle_theme/layout.html
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)      665 2022-11-16 19:12:59.000000 sphinx_sizzle_theme-0.1.2/README.rst
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)     1694 2023-05-05 10:29:51.000000 sphinx_sizzle_theme-0.1.2/setup.cfg
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)     2422 2023-05-05 10:18:30.000000 sphinx_sizzle_theme-0.1.2/LICENSE
+drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-05-05 10:29:51.000000 sphinx_sizzle_theme-0.1.2/docs/
+-rw-r--r--   0 vinay     (1000) vinay     (1000)      810 2019-04-12 06:44:40.000000 sphinx_sizzle_theme-0.1.2/docs/make.bat
+-rw-r--r--   0 vinay     (1000) vinay     (1000)       11 2019-05-09 06:33:17.000000 sphinx_sizzle_theme-0.1.2/docs/.dict-validwords
+drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-05-05 10:29:51.000000 sphinx_sizzle_theme-0.1.2/docs/_static/
+drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-05-05 10:29:51.000000 sphinx_sizzle_theme-0.1.2/docs/_static/img/
+-rw-r--r--   0 vinay     (1000) vinay     (1000)     2696 2019-04-12 19:22:47.000000 sphinx_sizzle_theme-0.1.2/docs/_static/img/ff-open.png
+-rw-r--r--   0 vinay     (1000) vinay     (1000)     2315 2019-04-12 19:22:56.000000 sphinx_sizzle_theme-0.1.2/docs/_static/img/chrome-closed.png
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)    36939 2019-05-10 15:06:59.000000 sphinx_sizzle_theme-0.1.2/docs/_static/img/mobile_1.png
+-rw-r--r--   0 vinay     (1000) vinay     (1000)     3383 2019-04-12 19:22:56.000000 sphinx_sizzle_theme-0.1.2/docs/_static/img/chrome-open.png
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)    36013 2019-05-10 15:07:10.000000 sphinx_sizzle_theme-0.1.2/docs/_static/img/mobile_2.png
+-rw-r--r--   0 vinay     (1000) vinay     (1000)     1969 2019-04-12 19:22:47.000000 sphinx_sizzle_theme-0.1.2/docs/_static/img/ff-closed.png
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)    46752 2023-05-05 10:17:56.000000 sphinx_sizzle_theme-0.1.2/docs/index.rst
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)      196 2022-11-11 17:35:37.000000 sphinx_sizzle_theme-0.1.2/docs/spelling_wordlist.txt
+-rw-r--r--   0 vinay     (1000) vinay     (1000)      603 2019-04-12 06:44:40.000000 sphinx_sizzle_theme-0.1.2/docs/Makefile
+-rw-r--r--   0 vinay     (1000) vinay     (1000)     5882 2022-11-07 18:24:56.000000 sphinx_sizzle_theme-0.1.2/docs/conf.py
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)      117 2022-05-11 18:19:06.000000 sphinx_sizzle_theme-0.1.2/pyproject.toml
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)     2142 2023-05-05 10:29:51.000000 sphinx_sizzle_theme-0.1.2/PKG-INFO
+drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-05-05 10:29:51.000000 sphinx_sizzle_theme-0.1.2/sphinx_sizzle_theme.egg-info/
+-rw-r--r--   0 vinay     (1000) vinay     (1000)      628 2023-05-05 10:29:51.000000 sphinx_sizzle_theme-0.1.2/sphinx_sizzle_theme.egg-info/SOURCES.txt
+-rw-r--r--   0 vinay     (1000) vinay     (1000)      150 2019-04-09 12:21:53.000000 sphinx_sizzle_theme-0.1.2/Makefile
```

### Comparing `sphinx_sizzle_theme-0.1.1/sphinx_sizzle_theme/__init__.py` & `sphinx_sizzle_theme-0.1.2/sphinx_sizzle_theme/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 #
-# Copyright 2019-2022 by Vinay Sajip. All Rights Reserved.
+# Copyright 2019-2023 by Vinay Sajip. All Rights Reserved.
 #
 from __future__ import print_function
 import datetime
 import inspect
 import io
 import json
 import logging
@@ -21,29 +21,27 @@
     basestring = str
 except ImportError:
     from urlparse import urljoin
     from urllib import urlencode
     from urllib2 import urlopen, Request
 
 from docutils.nodes import (strong, emphasis, inline, Text, document,
-                            paragraph, reprunicode, raw)
+                            paragraph, reprunicode, raw, literal)
 
 from docutils.parsers.rst.roles import set_classes
 
 # from sphinx import version_info as sphinx_version
 from sphinx.addnodes import literal_strong
+from sphinx.domains.python import PythonDomain
 from sphinx.util.console import bold
 from sphinx.writers.html import logger, HTMLTranslator as BaseTranslator
 
 HERE = path.abspath(path.dirname(__file__))
 
-__version__ = '0.1.1'
-
-logger = logging.getLogger(__name__)
-logger.addHandler(logging.NullHandler())
+__version__ = '0.1.2'
 
 logging_enabled = False
 
 def font_awesome(role, rawtext, text, lineno, inliner,
                  options=None, content=None):
     if options is None:
         options = {}
@@ -112,14 +110,32 @@
         _ICON_DATA[text] = svg
     content = Text(svg)
     node = raw(format='html')
     node.append(content)
     # import pdb; pdb.set_trace()
     return [node], []
 
+base_resolve_xref = PythonDomain.resolve_xref
+
+def resolve_xref(self, env, fromdocname, builder,
+                 type, target, node, contnode):
+    modname = node['py:module']
+    ref = node['reftarget']
+    if modname:
+        prefix = '%s.' % modname
+        if not ref.startswith(prefix):
+            ref = '%s%s' % (prefix, ref)
+    if not isinstance(contnode, str):
+        contnode['classes'].append('hover')
+        contnode['data-hoverref'] = ref
+    result = base_resolve_xref(self, env, fromdocname, builder, type, target, node, contnode)
+    return result
+
+PythonDomain.resolve_xref = resolve_xref
+
 def create_sitemap(app):
     filename = app.outdir + '/sitemap.xml'
     logger.info(bold('creating sitemap... '), nonl=True)
 
     root = ET.Element('urlset')
     root.set('xmlns', 'http://www.sitemaps.org/schemas/sitemap/0.9')
 
@@ -137,21 +153,24 @@
   sizzle.app_data = JSON.parse('%s');
 })();
 '''
 
 def create_app_data(app):
     logger.info(bold('creating app data... '), nonl=True)
     filename = app.outdir + '/app-data.js'
+    # if not path.exists(app.outdir):
+        # makedirs(app.outdir)
     data = {
         'glossary': {
             'document': app.glossary_doc,
             'terms': app.glossary_info,
         },
         'custom_data': app.config.html_theme_options.get('custom_data', {})
     }
+    # import pdb; pdb.set_trace()
     s = json.dumps(data).replace('\\', '\\\\').replace('\'', '\\\'')
     s = _APP_JS_SNIPPET % s
     with io.open(filename, 'w', encoding='utf-8') as f:
         f.write(s)
     logger.info('done')
 
 def on_init(app):
@@ -184,14 +203,15 @@
     # remove unused files.
     outdir = app.builder.outdir
     unused = (
         ('_static', 'jquery.js'),
         ('_static', 'jquery-3.2.1.js'),
         ('_static', 'underscore.js'),
         ('_static', 'underscore-1.3.1.js'),
+        ('_static', 'underscore-1.13.1.js'),
         ('_static', 'ajax-loader.gif'),
         ('_static', 'comment.png'),
         ('_static', 'comment-bright.png'),
         ('_static', 'comment-close.png'),
         #('_static', 'file.png'),
         ('_static', 'up.png'),
         ('_static', 'up-pressed.png'),
@@ -483,14 +503,15 @@
         self.body.append('</%s>' % tagname)
 
     def visit_inline(self, node):
         kwargs = {}
         if node.attributes:
             kwargs = extract_keys(node.attributes, 'title')
         self.body.append(self.starttag(node, 'span', '', **kwargs))
+        node.html5tagname = 'span'  # needed for Sphinx 7
 
     # For issue #6. Too bad we have to do copy-paste-edit here :-(
     def visit_label(self, node):
         self.body.append(self.starttag(node, 'td', '%s[' % self.context.pop(),
                                        CLASS='footnote-label'))
 
     # For issue #6. Too bad we have to do copy-paste-edit here :-(
@@ -499,14 +520,48 @@
                                        CLASS='docutils footnote',
                                        frame="void", rules="none"))
         self.body.append('<colgroup><col class="footnote-label" /><col /></colgroup>\n'
                          '<tbody valign="top">\n'
                          '<tr>')
         self.footnote_backrefs(node)
 
+    def visit_literal(self, node):
+        #
+        # This code had to be copied from the parent class, as there's no
+        # useful way of extending the parent class behaviour
+        #
+        if 'kbd' in node['classes']:
+            self.body.append(self.starttag(node, 'kbd', '',
+                                           CLASS='docutils literal notranslate'))
+            return
+        lang = node.get("language", None)
+        if 'code' not in node['classes'] or not lang:
+            kwargs = {
+                'CLASS': 'docutils literal notranslate'
+            }
+            for k, v in node.attributes.items():
+                if k.startswith('data-'):
+                    kwargs[k] = v
+            self.body.append(self.starttag(node, 'code', '',
+                                           **kwargs))
+            self.protect_literal_text += 1
+            return
+
+        opts = self.config.highlight_options.get(lang, {})
+        highlighted = self.highlighter.highlight_block(
+            node.astext(), lang, opts=opts, location=node, nowrap=True)
+        starttag = self.starttag(
+            node,
+            "code",
+            suffix="",
+            CLASS="docutils literal highlight highlight-%s" % lang
+        )
+        self.body.append(starttag + highlighted.strip() + "</code>")
+        raise nodes.SkipNode
+
     # Glossary processing
 
     def visit_glossary(self, node):
         self.in_glossary = True
         b = self.builder
         if b.app.glossary_doc is None:
             b.app.glossary_doc = b.current_docname
```

### Comparing `sphinx_sizzle_theme-0.1.1/sphinx_sizzle_theme/genindex.html` & `sphinx_sizzle_theme-0.1.2/sphinx_sizzle_theme/genindex.html`

 * *Files identical despite different names*

### Comparing `sphinx_sizzle_theme-0.1.1/sphinx_sizzle_theme/sizzle.scss` & `sphinx_sizzle_theme-0.1.2/sphinx_sizzle_theme/sizzle.scss`

 * *Files 2% similar despite different names*

```diff
@@ -504,14 +504,18 @@
       }
       &.cap {
         margin-top: 10px;
         background-color: #f2f2f2;
       }
     }
   }
+  &.generic-table.hpad td, &.generic-table.hpad th {
+    padding-left: 2px;
+    padding-right: 2px;
+  }
 }
 
 img.toggler {
   margin-right: 3px;
   margin-top: 3px;
   cursor: pointer;
 }
@@ -1451,14 +1455,41 @@
   box-shadow: 3px 3px 2px 0 rgba(0,0,0,0.4);
 }
 
 .tc-infotip {
   cursor: help;
 }
 
+.hovertip {
+  color: black;
+  font-size: 100%;
+
+  .function, .class {
+    border-bottom: 1px solid black;
+    margin-bottom: 0.5em;
+    margin-top: 0.25em;
+    padding-bottom: 0.25em;
+    font-size: 105%;
+  }
+  blockquote {
+    padding: 0px 0px 0px 1em;
+    margin: 0px;
+    background-color: transparent;
+    font-size: 100%;
+  }
+  h6 {
+    font-size: 100%;
+    font-weight: bold;
+    font-family: $sans-font;
+  }
+  .pdoc-alert p {
+    padding-left: 1em;
+  }
+}
+
 /* Keyboard keys style */
 
 kbd
 {
   background-color:#f7f7f7;
   border:1px solid #ccc;
   border-radius:3px;
```

### Comparing `sphinx_sizzle_theme-0.1.1/sphinx_sizzle_theme/static/css/sizzle.css` & `sphinx_sizzle_theme-0.1.2/sphinx_sizzle_theme/static/css/sizzle.css`

 * *Files 1% similar despite different names*

```diff
@@ -507,14 +507,19 @@
 }
 
 table.indextable tr.cap {
   margin-top: 10px;
   background-color: #f2f2f2;
 }
 
+table.generic-table.hpad td, table.generic-table.hpad th {
+  padding-left: 2px;
+  padding-right: 2px;
+}
+
 img.toggler {
   margin-right: 3px;
   margin-top: 3px;
   cursor: pointer;
 }
 
 div.modindex-jumpbox, div.genindex-jumpbox {
@@ -1493,14 +1498,44 @@
   box-shadow: 3px 3px 2px 0 rgba(0, 0, 0, 0.4);
 }
 
 .tc-infotip {
   cursor: help;
 }
 
+.hovertip {
+  color: black;
+  font-size: 100%;
+}
+
+.hovertip .function, .hovertip .class {
+  border-bottom: 1px solid black;
+  margin-bottom: 0.5em;
+  margin-top: 0.25em;
+  padding-bottom: 0.25em;
+  font-size: 105%;
+}
+
+.hovertip blockquote {
+  padding: 0px 0px 0px 1em;
+  margin: 0px;
+  background-color: transparent;
+  font-size: 100%;
+}
+
+.hovertip h6 {
+  font-size: 100%;
+  font-weight: bold;
+  font-family: Roboto, "Open Sans", "Helvetica Neue", Helvetica, Arial, sans-serif;
+}
+
+.hovertip .pdoc-alert p {
+  padding-left: 1em;
+}
+
 /* Keyboard keys style */
 kbd {
   background-color: #f7f7f7;
   border: 1px solid #ccc;
   border-radius: 3px;
   color: #333;
   display: inline-block;
```

### Comparing `sphinx_sizzle_theme-0.1.1/sphinx_sizzle_theme/search.html` & `sphinx_sizzle_theme-0.1.2/sphinx_sizzle_theme/search.html`

 * *Files identical despite different names*

### Comparing `sphinx_sizzle_theme-0.1.1/sphinx_sizzle_theme/layout.html` & `sphinx_sizzle_theme-0.1.2/sphinx_sizzle_theme/layout.html`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 {%- macro css() %}
-    <link rel="stylesheet" href="{{ pathto('_static/pygments.css', 1) }}" type="text/css" />
-    <link rel="stylesheet" href="{{ pathto('_static/' + style, 1) }}" type="text/css" />
     {%- for cssfile in css_files %}
     <link rel="stylesheet" href="{{ pathto(cssfile, 1) }}" type="text/css" />
     {%- endfor %}
 {%- endmacro %}
 {%- macro script() %}
     <script>
       var DOCUMENTATION_OPTIONS = {
@@ -14,15 +12,15 @@
         FILE_SUFFIX: '{{ '' if no_search_suffix else file_suffix }}',
         LINK_SUFFIX: '{{ link_suffix }}',
         HAS_SOURCE:  false,
         SOURCELINK_SUFFIX: '{{ sourcelink_suffix }}'
       };
       $(document).data('sizzle', {on_load: []});
     </script>
-    {%- for scriptfile in script_files[2:] %}
+    {%- for scriptfile in script_files[3:] %}
     {%- if js_tag is defined %}
     {{ js_tag(scriptfile) }}
     {%- else %}
     {%- if scriptfile %}
     <script src="{{ pathto(scriptfile, 1) }}"></script>
     {%- endif %}
     {%- endif %}
@@ -111,19 +109,19 @@
 <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap@3.4.1/dist/css/bootstrap.min.css" integrity="sha256-bZLfwXAP04zRMK2BjiO8iu9pf4FbLqX6zitd+tIvLhE=" crossorigin="anonymous">
 <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap@3.4.1/dist/css/bootstrap-theme.min.css" integrity="sha256-8uHMIn1ru0GS5KO+zf7Zccf8Uw12IA5DrdEcmMuWLFM=" crossorigin="anonymous">
 <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/tooltipster@4.2.8/dist/css/tooltipster.bundle.min.css" integrity="sha256-Qc4lCfqZWYaHF5hgEOFrYzSIX9Rrxk0NPHRac+08QeQ=" crossorigin="anonymous">
 <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/tooltipster@4.2.8/dist/css/plugins/tooltipster/sideTip/themes/tooltipster-sideTip-light.min.css" integrity="sha256-Wa1I4jhSXeWd3N6RhfPlkqr1WlT+zS3Vh2YGCg0129E=" crossorigin="anonymous">
 <link href="https://fonts.googleapis.com/css?family=Open+Sans|Source+Code+Pro|Source+Sans+Pro|Source+Serif+Pro|Roboto|Roboto+Mono{{ theme_google_fonts }}" rel="stylesheet">
 <link href="https://fonts.red-dove.com/iosevka-ss09-regular/webfont.css" rel="stylesheet">
 {{ css() }}
-<script src="https://cdnjs.cloudflare.com/ajax/libs/jquery/3.6.0/jquery.min.js" integrity="sha512-894YE6QWD5I59HgZOGReFYm4dnWc1Qt5NtvYSaNcOP+u1T9qYdvdihz0PPSiiqn/+/3e7Jo4EaG7TubfWGUrMQ==" crossorigin="anonymous" referrerpolicy="no-referrer"></script>
-<script src="https://cdn.jsdelivr.net/npm/bootstrap@3.4.1/dist/js/bootstrap.min.js" integrity="sha256-nuL8/2cJ5NDSSwnKD8VqreErSWHtnEP9E7AySL+1ev4=" crossorigin="anonymous"></script>
-<script src="https://cdnjs.cloudflare.com/ajax/libs/underscore.js/1.9.1/underscore-min.js" integrity="sha256-G7A4JrJjJlFqP0yamznwPjAApIKPkadeHfyIwiaa9e0=" crossorigin="anonymous"></script>
-<script src="https://cdn.jsdelivr.net/npm/tooltipster@4.2.8/dist/js/tooltipster.bundle.min.js" integrity="sha256-v8akIv8SCqn5f3mbVB7vEWprIizxPh6oV0yhao/dbB4=" crossorigin="anonymous"></script>
-<script src="https://cdnjs.cloudflare.com/ajax/libs/clipboard.js/2.0.4/clipboard.min.js" integrity="sha256-FiZwavyI2V6+EXO1U+xzLG3IKldpiTFf3153ea9zikQ=" crossorigin="anonymous"></script>
+<script src="https://cdnjs.cloudflare.com/ajax/libs/jquery/3.6.1/jquery.min.js" integrity="sha512-aVKKRRi/Q/YV+4mjoKBsE4x3H+BkegoM/em46NNlCqNTmUYADjBbeNefNxYV7giUp0VxICtqdrbqU7iVaeZNXA==" crossorigin="anonymous" referrerpolicy="no-referrer"></script>
+<script src="https://cdn.jsdelivr.net/npm/bootstrap@3.4.1/dist/js/bootstrap.min.js" integrity="sha256-nuL8/2cJ5NDSSwnKD8VqreErSWHtnEP9E7AySL+1ev4=" crossorigin="anonymous" referrerpolicy="no-referrer"></script>
+<script src="https://cdnjs.cloudflare.com/ajax/libs/underscore.js/1.13.6/underscore-min.js" integrity="sha512-2V49R8ndaagCOnwmj8QnbT1Gz/rie17UouD9Re5WxbzRVUGoftCu5IuqqtAM9+UC3fwfHCSJR1hkzNQh/2wdtg==" crossorigin="anonymous" referrerpolicy="no-referrer"></script>
+<script src="https://cdn.jsdelivr.net/npm/tooltipster@4.2.8/dist/js/tooltipster.bundle.min.js" integrity="sha256-v8akIv8SCqn5f3mbVB7vEWprIizxPh6oV0yhao/dbB4=" crossorigin="anonymous" referrerpolicy="no-referrer"></script>
+<script src="https://cdnjs.cloudflare.com/ajax/libs/clipboard.js/2.0.4/clipboard.min.js" integrity="sha256-FiZwavyI2V6+EXO1U+xzLG3IKldpiTFf3153ea9zikQ=" crossorigin="anonymous" referrerpolicy="no-referrer"></script>
 {%- block scripts %}
 {{- script() }}
 {%- endblock %}
 {%- block linktags %}
 {%- if hasdoc('about') %}
 <link rel="author" title="{{ _('About these documents') }}" href="{{ pathto('about') }}" />
 {%- endif %}
@@ -506,35 +504,86 @@
 
   function add_custom_tooltips() {
     if (!sizzle.app_data) {
       return;
     }
 
     var info_tips = sizzle.app_data.custom_data['info-tips'] || {};
+    var hover_tips = sizzle.app_data.custom_data['hovers'] || {};
 
-    if ($.isEmptyObject(info_tips)) {
+    if ($.isEmptyObject(info_tips) && $.isEmptyObject(hover_tips)) {
       return;
     }
 
     var tt_options = $.extend({contentAsHTML: true}, default_tt_options);
 
-    $('.tc-info').each(function() {
-      var $elem = $(this).prev();
-      var classes = $elem.attr('class');
-      var m = /\btci-([\S]+)/.exec(classes);
-
-      if (m !== null) {
-        var key = m[1];
-
-        if (key in info_tips) {
-          var v = info_tips[key];
-          var tt = $elem.tooltipster(tt_options).tooltipster('content', v);
+    if (!$.isEmptyObject(info_tips)) {
+      $('.tc-info').each(function() {
+        var $elem = $(this).prev();
+        var classes = $elem.attr('class');
+        var m = /\btci-([\S]+)/.exec(classes);
+
+        if (m !== null) {
+          var key = m[1];
+
+          if (key in info_tips) {
+            var v = info_tips[key];
+            var tt = $elem.tooltipster(tt_options).tooltipster('content', v);
+          }
         }
-      }
-    });
+      });
+    }
+    if (!$.isEmptyObject(hover_tips)) {
+      var current_origin, current_instance;
+
+      var h_options = {
+        functionBefore: function(instance, helper) {
+          current_instance = instance;
+          current_origin = helper.origin;
+          //console.log('before', current_instance, current_origin);
+        },
+        functionAfter: function(instance, helper) {
+          current_instance = null;
+          current_origin = null;
+          //console.log('after', current_instance, current_origin);
+        }
+      };
+
+      var ht_options = $.extend(h_options, tt_options);
+      $('.hover').each(function() {
+        var $e = $(this);
+        var ref = $e.data('hoverref');
+
+        if (ref) {
+          var tip = hover_tips[ref];
+
+          if (tip) {
+            $e.tooltipster(ht_options).tooltipster('content', tip);
+            //if (/encrypt_and_sign/.test(ref)) { console.log(tip); }
+          }
+        }
+      });
+/*
+      $(document).on('click', '.hovertip a.hoverlink', function(e) {
+        if (!sizzle.app_data) {
+          return;
+        }
+        var $this = $(this);
+        var $content = $this.parent('.tooltipster-content');
+        var ref = $this.data('href');
+        var hover_tips = sizzle.app_data.custom_data['hovers'] || {};
+        var tip = hover_tips[ref];
+
+        if (tip && current_instance) {
+          current_instance.content(tip);
+        }
+
+      });
+ */
+    }
   }
 
   add_custom_tooltips();
 
   setTimeout(activate_tooltips, 1000);
 {% endif %}
```

### Comparing `sphinx_sizzle_theme-0.1.1/README.rst` & `sphinx_sizzle_theme-0.1.2/README.rst`

 * *Files 27% similar despite different names*

```diff
@@ -1,12 +1,13 @@
-Sizzle theme for Sphinx
-=======================
+The Sizzle theme for Sphinx
+===========================
 
 This repository contains the Sizzle theme for Sphinx_. Sizzle was inspired by,
-and used some of the styling of, the Guzzle_ theme for Sphinx.
+and used some of the styling of, the Guzzle_ theme for Sphinx. It has now diverged
+quite a lot, both in terms of styling and other functionality.
 
 .. _Sphinx: https://www.sphinx-doc.org/
 
 .. _Guzzle: https://github.com/guzzle/guzzle_sphinx_theme
 
 Installation
 ------------
```

### Comparing `sphinx_sizzle_theme-0.1.1/LICENSE` & `sphinx_sizzle_theme-0.1.2/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (C) 2019 Vinay Sajip <vinay_sajip@yahoo.co.uk>
+Copyright (C) 2019-2023 Vinay Sajip <vinay_sajip@yahoo.co.uk>
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `sphinx_sizzle_theme-0.1.1/docs/make.bat` & `sphinx_sizzle_theme-0.1.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `sphinx_sizzle_theme-0.1.1/docs/_static/img/ff-open.png` & `sphinx_sizzle_theme-0.1.2/docs/_static/img/ff-open.png`

 * *Files identical despite different names*

### Comparing `sphinx_sizzle_theme-0.1.1/docs/_static/img/chrome-closed.png` & `sphinx_sizzle_theme-0.1.2/docs/_static/img/chrome-closed.png`

 * *Files identical despite different names*

### Comparing `sphinx_sizzle_theme-0.1.1/docs/_static/img/mobile_1.png` & `sphinx_sizzle_theme-0.1.2/docs/_static/img/mobile_1.png`

 * *Files identical despite different names*

### Comparing `sphinx_sizzle_theme-0.1.1/docs/_static/img/chrome-open.png` & `sphinx_sizzle_theme-0.1.2/docs/_static/img/chrome-open.png`

 * *Files identical despite different names*

### Comparing `sphinx_sizzle_theme-0.1.1/docs/_static/img/mobile_2.png` & `sphinx_sizzle_theme-0.1.2/docs/_static/img/mobile_2.png`

 * *Files identical despite different names*

### Comparing `sphinx_sizzle_theme-0.1.1/docs/_static/img/ff-closed.png` & `sphinx_sizzle_theme-0.1.2/docs/_static/img/ff-closed.png`

 * *Files identical despite different names*

### Comparing `sphinx_sizzle_theme-0.1.1/docs/Makefile` & `sphinx_sizzle_theme-0.1.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `sphinx_sizzle_theme-0.1.1/docs/conf.py` & `sphinx_sizzle_theme-0.1.2/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,15 +66,15 @@
 version = '.'.join(release.split('.')[:2])
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
-language = None
+#language = None
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This patterns also effect to html_static_path and html_extra_path
 exclude_patterns = ['_build', 'Thumbs.db', '.DS_Store']
 
 # The name of the Pygments (syntax highlighting) style to use.
```

### Comparing `sphinx_sizzle_theme-0.1.1/setup.py` & `sphinx_sizzle_theme-0.1.2/setup.cfg`

 * *Files 27% similar despite different names*

```diff
@@ -1,56 +1,65 @@
-# -*- coding: utf-8 -*-
-#
-# Copyright 2019 by Vinay Sajip. All Rights Reserved.
-#
-
-from io import open
-from setuptools import setup
-from sphinx_sizzle_theme import __version__
-
-setup(
-    name='sphinx_sizzle_theme',
-    version=__version__,
-    url='https://bitbucket.org/vinay.sajip/sphinx_sizzle_theme/',
-    license='MIT',
-    author='Vinay Sajip',
-    author_email='vinay_sajip@yahoo.co.uk',
-    description='Sizzle theme for Sphinx',
-    long_description=open('README.rst', encoding='utf-8').read(),
-    zip_safe=False,
-    packages=['sphinx_sizzle_theme'],
-    package_data={'sphinx_sizzle_theme': [
-        'theme.conf',
-        '*.html',
-        'version.txt',
-        'static/css/*.css',
-        'static/js/*.js',
-        'static/fonts/*.*'
-    ]},
-    entry_points = {
-        'sphinx.html_themes': [
-            'sizzle = sphinx_sizzle_theme',
-        ]
-    },
-    install_requires=[
-       'sphinx'
-    ],
-    classifiers=[
-        'Framework :: Sphinx',
-        'Framework :: Sphinx :: Theme',
-        'Development Status :: 5 - Production/Stable',
-        'License :: OSI Approved :: MIT License',
-        'Environment :: Console',
-        'Environment :: Web Environment',
-        'Intended Audience :: Developers',
-        'Programming Language :: Python :: 2.7',
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
-        'Programming Language :: Python :: 3.10',
-        'Operating System :: OS Independent',
-        'Topic :: Documentation',
-        'Topic :: Software Development :: Documentation',
-    ],
-)
+[metadata]
+name = sphinx_sizzle_theme
+version = attr: sphinx_sizzle_theme.__version__
+description = The Sizzle theme for Sphinx.
+long_description = file: README.rst
+url = https://docs.red-dove.com/sphinx_sizzle_theme/
+author = Vinay Sajip
+author_email = vinay_sajip@yahoo.co.uk
+maintainer = Vinay Sajip
+maintainer_email = vinay_sajip@yahoo.co.uk
+license = MIT
+license_file = LICENSE
+classifiers = 
+	Framework :: Sphinx
+	Framework :: Sphinx :: Theme
+	Development Status :: 5 - Production/Stable
+	License :: OSI Approved :: MIT License
+	Environment :: Console
+	Environment :: Web Environment
+	Intended Audience :: Developers
+	Programming Language :: Python
+	Programming Language :: Python :: Implementation
+	Programming Language :: Python :: 2.7
+	Programming Language :: Python :: 3
+	Programming Language :: Python :: 3.6
+	Programming Language :: Python :: 3.7
+	Programming Language :: Python :: 3.8
+	Programming Language :: Python :: 3.9
+	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
+	Operating System :: OS Independent
+	Topic :: Documentation
+project_urls = 
+	Documentation = https://docs.red-dove.com/sphinx_sizzle_theme/
+	Source = https://github.com/vsajip/sphinx_sizzle_theme
+	Tracker = https://github.com/vsajip/sphinx_sizzle_theme/issues
+keywords = documentation,sphinx,theme
+platforms = any
+
+[options]
+packages = sphinx_sizzle_theme
+zip_safe = False
+install_requires = 
+	sphinx
+
+[options.entry_points]
+sphinx.html_themes = 
+	sizzle = sphinx_sizzle_theme
+
+[options.package_data]
+sphinx_sizzle_theme = 
+	theme.conf
+	*.html
+	version.txt
+	static/css/*.css
+	static/js/*.js
+	static/fonts/*.*
+
+[bdist_wheel]
+universal = 1
+
+[egg_info]
+tag_build = 
+tag_date = 0
+
```

### Comparing `sphinx_sizzle_theme-0.1.1/sphinx_sizzle_theme.egg-info/SOURCES.txt` & `sphinx_sizzle_theme-0.1.2/sphinx_sizzle_theme.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 LICENSE
 MANIFEST.in
 Makefile
 README.rst
+pyproject.toml
 setup.cfg
-setup.py
 docs/.dict-validwords
 docs/Makefile
 docs/conf.py
 docs/index.rst
 docs/make.bat
+docs/spelling_wordlist.txt
 docs/_static/img/chrome-closed.png
 docs/_static/img/chrome-open.png
 docs/_static/img/ff-closed.png
 docs/_static/img/ff-open.png
 docs/_static/img/mobile_1.png
 docs/_static/img/mobile_2.png
 sphinx_sizzle_theme/__init__.py
```

