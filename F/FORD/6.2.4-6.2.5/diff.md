# Comparing `tmp/FORD-6.2.4.tar.gz` & `tmp/FORD-6.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FORD-6.2.4.tar", last modified: Wed Apr  5 13:18:27 2023, max compression
+gzip compressed data, was "FORD-6.2.5.tar", last modified: Fri May  5 17:00:12 2023, max compression
```

## Comparing `FORD-6.2.4.tar` & `FORD-6.2.5.tar`

### file list

```diff
@@ -1,182 +1,182 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 13:18:27.961084 FORD-6.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-05 13:18:16.000000 FORD-6.2.4/.git-blame-ignore-revs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 13:18:27.929084 FORD-6.2.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 13:18:27.945084 FORD-6.2.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-04-05 13:18:16.000000 FORD-6.2.4/.github/workflows/black.yml
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-04-05 13:18:16.000000 FORD-6.2.4/.github/workflows/corpus_regressions.yml
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-04-05 13:18:16.000000 FORD-6.2.4/.github/workflows/python_publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-04-05 13:18:16.000000 FORD-6.2.4/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-05 13:18:16.000000 FORD-6.2.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-05 13:18:16.000000 FORD-6.2.4/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)  4225846 2023-04-05 13:18:16.000000 FORD-6.2.4/2003standard.pdf
--rw-r--r--   0 runner    (1001) docker     (123)  8053119 2023-04-05 13:18:16.000000 FORD-6.2.4/2008standard.pdf
--rw-r--r--   0 runner    (1001) docker     (123)    30503 2023-04-05 13:18:16.000000 FORD-6.2.4/CHANGELOG.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 13:18:27.945084 FORD-6.2.4/FORD.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6183 2023-04-05 13:18:27.000000 FORD-6.2.4/FORD.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-04-05 13:18:27.000000 FORD-6.2.4/FORD.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 13:18:27.000000 FORD-6.2.4/FORD.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-05 13:18:27.000000 FORD-6.2.4/FORD.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-04-05 13:18:27.000000 FORD-6.2.4/FORD.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-05 13:18:27.000000 FORD-6.2.4/FORD.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    35120 2023-04-05 13:18:16.000000 FORD-6.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-05 13:18:16.000000 FORD-6.2.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6183 2023-04-05 13:18:27.961084 FORD-6.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4879 2023-04-05 13:18:16.000000 FORD-6.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 13:18:27.945084 FORD-6.2.4/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-04-05 13:18:16.000000 FORD-6.2.4/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 13:18:27.945084 FORD-6.2.4/docs/api/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-05 13:18:16.000000 FORD-6.2.4/docs/api/ford.fixed2free2.rst
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-05 13:18:16.000000 FORD-6.2.4/docs/api/ford.fortran_project.rst
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-05 13:18:16.000000 FORD-6.2.4/docs/api/ford.graphs.rst
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-05 13:18:16.000000 FORD-6.2.4/docs/api/ford.intrinsics.rst
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-05 13:18:16.000000 FORD-6.2.4/docs/api/ford.md_environ.rst
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-05 13:18:16.000000 FORD-6.2.4/docs/api/ford.md_striped_table.rst
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-05 13:18:16.000000 FORD-6.2.4/docs/api/ford.output.rst
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-05 13:18:16.000000 FORD-6.2.4/docs/api/ford.pagetree.rst
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-05 13:18:16.000000 FORD-6.2.4/docs/api/ford.reader.rst
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-05 13:18:16.000000 FORD-6.2.4/docs/api/ford.rst
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-05 13:18:16.000000 FORD-6.2.4/docs/api/ford.sourceform.rst
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-05 13:18:16.000000 FORD-6.2.4/docs/api/ford.tipue_search.rst
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-04-05 13:18:16.000000 FORD-6.2.4/docs/api/ford.utils.rst
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-05 13:18:16.000000 FORD-6.2.4/docs/api/modules.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-04-05 13:18:16.000000 FORD-6.2.4/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 13:18:27.945084 FORD-6.2.4/docs/developers_guide/
--rw-r--r--   0 runner    (1001) docker     (123)     3674 2023-04-05 13:18:16.000000 FORD-6.2.4/docs/developers_guide/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5875 2023-04-05 13:18:16.000000 FORD-6.2.4/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-04-05 13:18:16.000000 FORD-6.2.4/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 13:18:27.949084 FORD-6.2.4/docs/user_guide/
--rw-r--r--   0 runner    (1001) docker     (123)    11896 2023-04-05 13:18:16.000000 FORD-6.2.4/docs/user_guide/callgraph.png
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-05 13:18:16.000000 FORD-6.2.4/docs/user_guide/command_line_options.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-04-05 13:18:16.000000 FORD-6.2.4/docs/user_guide/documentation_meta_data.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-04-05 13:18:16.000000 FORD-6.2.4/docs/user_guide/getting_started.rst
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-05 13:18:16.000000 FORD-6.2.4/docs/user_guide/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-04-05 13:18:16.000000 FORD-6.2.4/docs/user_guide/limitation.rst
--rw-r--r--   0 runner    (1001) docker     (123)    72521 2023-04-05 13:18:16.000000 FORD-6.2.4/docs/user_guide/output-example.png
--rw-r--r--   0 runner    (1001) docker     (123)   132134 2023-04-05 13:18:16.000000 FORD-6.2.4/docs/user_guide/pages-example.png
--rw-r--r--   0 runner    (1001) docker     (123)    26471 2023-04-05 13:18:16.000000 FORD-6.2.4/docs/user_guide/project_file_options.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-04-05 13:18:16.000000 FORD-6.2.4/docs/user_guide/running_ford.rst
--rw-r--r--   0 runner    (1001) docker     (123)    40179 2023-04-05 13:18:16.000000 FORD-6.2.4/docs/user_guide/say_hello_example.png
--rw-r--r--   0 runner    (1001) docker     (123)    13335 2023-04-05 13:18:16.000000 FORD-6.2.4/docs/user_guide/writing_documentation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5639 2023-04-05 13:18:16.000000 FORD-6.2.4/docs/user_guide/writing_pages.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 13:18:27.949084 FORD-6.2.4/example/
--rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-04-05 13:18:16.000000 FORD-6.2.4/example/example-project-file.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 13:18:27.949084 FORD-6.2.4/example/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 13:18:27.949084 FORD-6.2.4/example/src/excluded_directory/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-05 13:18:16.000000 FORD-6.2.4/example/src/excluded_directory/this_file_will_not_be_included.f90
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-05 13:18:16.000000 FORD-6.2.4/example/src/excluded_file.f90
--rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-04-05 13:18:16.000000 FORD-6.2.4/example/src/ford_example_type.f90
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-04-05 13:18:16.000000 FORD-6.2.4/example/src/ford_f77_example.f
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-04-05 13:18:16.000000 FORD-6.2.4/example/src/ford_interfaces.f90
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-04-05 13:18:16.000000 FORD-6.2.4/example/src/ford_test_module.fpp
--rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-04-05 13:18:16.000000 FORD-6.2.4/example/src/ford_test_program.f90
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 13:18:27.953084 FORD-6.2.4/ford/
--rwxr-xr-x   0 runner    (1001) docker     (123)    21883 2023-04-05 13:18:16.000000 FORD-6.2.4/ford/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-05 13:18:16.000000 FORD-6.2.4/ford/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-05 13:18:27.000000 FORD-6.2.4/ford/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    17815 2023-04-05 13:18:16.000000 FORD-6.2.4/ford/config.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 13:18:27.953084 FORD-6.2.4/ford/css/
--rw-r--r--   0 runner    (1001) docker     (123)   126891 2023-04-05 13:18:16.000000 FORD-6.2.4/ford/css/bootstrap.css
--rw-r--r--   0 runner    (1001) docker     (123)   105249 2023-04-05 13:18:16.000000 FORD-6.2.4/ford/css/bootstrap.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    26651 2023-04-05 13:18:16.000000 FORD-6.2.4/ford/css/font-awesome.css
--rw-r--r--   0 runner    (1001) docker     (123)    21984 2023-04-05 13:18:16.000000 FORD-6.2.4/ford/css/font-awesome.min.css
--rw-r--r--   0 runner    (1001) docker     (123)     5232 2023-04-05 13:18:16.000000 FORD-6.2.4/ford/css/local.css
--rw-r--r--   0 runner    (1001) docker     (123)     3442 2023-04-05 13:18:16.000000 FORD-6.2.4/ford/css/pygments.css
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-04-05 13:18:16.000000 FORD-6.2.4/ford/favicon.png
--rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-04-05 13:18:16.000000 FORD-6.2.4/ford/fixed2free2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 13:18:27.953084 FORD-6.2.4/ford/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)    85908 2023-04-05 13:18:16.000000 FORD-6.2.4/ford/fonts/FontAwesome.otf
--rw-r--r--   0 runner    (1001) docker     (123)    56006 2023-04-05 13:18:16.000000 FORD-6.2.4/ford/fonts/fontawesome-webfont.eot
--rw-r--r--   0 runner    (1001) docker     (123)   287007 2023-04-05 13:18:16.000000 FORD-6.2.4/ford/fonts/fontawesome-webfont.svg
--rw-r--r--   0 runner    (1001) docker     (123)   112160 2023-04-05 13:18:16.000000 FORD-6.2.4/ford/fonts/fontawesome-webfont.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    65452 2023-04-05 13:18:16.000000 FORD-6.2.4/ford/fonts/fontawesome-webfont.woff
--rw-r--r--   0 runner    (1001) docker     (123)    20335 2023-04-05 13:18:16.000000 FORD-6.2.4/ford/fonts/glyphicons-halflings-regular.eot
--rw-r--r--   0 runner    (1001) docker     (123)    62926 2023-04-05 13:18:16.000000 FORD-6.2.4/ford/fonts/glyphicons-halflings-regular.svg
--rw-r--r--   0 runner    (1001) docker     (123)    41280 2023-04-05 13:18:16.000000 FORD-6.2.4/ford/fonts/glyphicons-halflings-regular.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    23320 2023-04-05 13:18:16.000000 FORD-6.2.4/ford/fonts/glyphicons-halflings-regular.woff
--rwxr-xr-x   0 runner    (1001) docker     (123)    15161 2023-04-05 13:18:16.000000 FORD-6.2.4/ford/fortran_project.py
--rw-r--r--   0 runner    (1001) docker     (123)    45836 2023-04-05 13:18:16.000000 FORD-6.2.4/ford/graphs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7191 2023-04-05 13:18:16.000000 FORD-6.2.4/ford/intrinsics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 13:18:27.957084 FORD-6.2.4/ford/js/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 13:18:27.957084 FORD-6.2.4/ford/js/MathJax-config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 13:18:16.000000 FORD-6.2.4/ford/js/MathJax-config/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    67155 2023-04-05 13:18:16.000000 FORD-6.2.4/ford/js/bootstrap.js
--rw-r--r--   0 runner    (1001) docker     (123)    35601 2023-04-05 13:18:16.000000 FORD-6.2.4/ford/js/bootstrap.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-04-05 13:18:16.000000 FORD-6.2.4/ford/js/ie10-viewport-bug-workaround.js
--rw-r--r--   0 runner    (1001) docker     (123)    84320 2023-04-05 13:18:16.000000 FORD-6.2.4/ford/js/jquery-2.1.3.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    28810 2023-04-05 13:18:16.000000 FORD-6.2.4/ford/js/svg-pan-zoom.min.js
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-04-05 13:18:16.000000 FORD-6.2.4/ford/md_environ.py
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-04-05 13:18:16.000000 FORD-6.2.4/ford/md_striped_table.py
--rw-r--r--   0 runner    (1001) docker     (123)    17032 2023-04-05 13:18:16.000000 FORD-6.2.4/ford/output.py
--rw-r--r--   0 runner    (1001) docker     (123)     6014 2023-04-05 13:18:16.000000 FORD-6.2.4/ford/pagetree.py
--rw-r--r--   0 runner    (1001) docker     (123)    16542 2023-04-05 13:18:16.000000 FORD-6.2.4/ford/reader.py
--rw-r--r--   0 runner    (1001) docker     (123)   112981 2023-04-05 13:18:16.000000 FORD-6.2.4/ford/sourceform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 13:18:27.957084 FORD-6.2.4/ford/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-04-05 13:18:16.000000 FORD-6.2.4/ford/templates/absint_list.html
--rw-r--r--   0 runner    (1001) docker     (123)    10765 2023-04-05 13:18:16.000000 FORD-6.2.4/ford/templates/base.html
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-04-05 13:18:16.000000 FORD-6.2.4/ford/templates/block_list.html
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-04-05 13:18:16.000000 FORD-6.2.4/ford/templates/block_page.html
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-04-05 13:18:16.000000 FORD-6.2.4/ford/templates/file_list.html
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-04-05 13:18:16.000000 FORD-6.2.4/ford/templates/file_page.html
--rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-04-05 13:18:16.000000 FORD-6.2.4/ford/templates/genint_page.html
--rw-r--r--   0 runner    (1001) docker     (123)     6468 2023-04-05 13:18:16.000000 FORD-6.2.4/ford/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-04-05 13:18:16.000000 FORD-6.2.4/ford/templates/info_page.html
--rw-r--r--   0 runner    (1001) docker     (123)    26582 2023-04-05 13:18:16.000000 FORD-6.2.4/ford/templates/macros.html
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-04-05 13:18:16.000000 FORD-6.2.4/ford/templates/mod_list.html
--rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-04-05 13:18:16.000000 FORD-6.2.4/ford/templates/mod_page.html
--rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-04-05 13:18:16.000000 FORD-6.2.4/ford/templates/nongenint_page.html
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-04-05 13:18:16.000000 FORD-6.2.4/ford/templates/proc_list.html
--rw-r--r--   0 runner    (1001) docker     (123)     4172 2023-04-05 13:18:16.000000 FORD-6.2.4/ford/templates/proc_page.html
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-04-05 13:18:16.000000 FORD-6.2.4/ford/templates/prog_list.html
--rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-04-05 13:18:16.000000 FORD-6.2.4/ford/templates/prog_page.html
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-04-05 13:18:16.000000 FORD-6.2.4/ford/templates/search.html
--rw-r--r--   0 runner    (1001) docker     (123)     3210 2023-04-05 13:18:16.000000 FORD-6.2.4/ford/templates/type_page.html
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-04-05 13:18:16.000000 FORD-6.2.4/ford/templates/types_list.html
--rw-r--r--   0 runner    (1001) docker     (123)     3454 2023-04-05 13:18:16.000000 FORD-6.2.4/ford/tipue_search.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 13:18:27.957084 FORD-6.2.4/ford/tipuesearch/
--rw-r--r--   0 runner    (1001) docker     (123)    12292 2023-04-05 13:18:16.000000 FORD-6.2.4/ford/tipuesearch/.DS_Store
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 13:18:27.961084 FORD-6.2.4/ford/tipuesearch/img/
--rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-04-05 13:18:16.000000 FORD-6.2.4/ford/tipuesearch/img/.DS_Store
--rw-r--r--   0 runner    (1001) docker     (123)     4178 2023-04-05 13:18:16.000000 FORD-6.2.4/ford/tipuesearch/img/loader.gif
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-04-05 13:18:16.000000 FORD-6.2.4/ford/tipuesearch/img/search.png
--rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-04-05 13:18:16.000000 FORD-6.2.4/ford/tipuesearch/tipuesearch.css
--rw-r--r--   0 runner    (1001) docker     (123)    22505 2023-04-05 13:18:16.000000 FORD-6.2.4/ford/tipuesearch/tipuesearch.js
--rw-r--r--   0 runner    (1001) docker     (123)     6784 2023-04-05 13:18:16.000000 FORD-6.2.4/ford/tipuesearch/tipuesearch.min.js
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-05 13:18:16.000000 FORD-6.2.4/ford/tipuesearch/tipuesearch_set.js
--rw-r--r--   0 runner    (1001) docker     (123)    18170 2023-04-05 13:18:16.000000 FORD-6.2.4/ford/utils.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      138 2023-04-05 13:18:16.000000 FORD-6.2.4/ford.py
--rw-r--r--   0 runner    (1001) docker     (123)    72521 2023-04-05 13:18:16.000000 FORD-6.2.4/output-example.png
--rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-04-05 13:18:16.000000 FORD-6.2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-05 13:18:16.000000 FORD-6.2.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-05 13:18:27.961084 FORD-6.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-05 13:18:16.000000 FORD-6.2.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 13:18:27.961084 FORD-6.2.4/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-04-05 13:18:16.000000 FORD-6.2.4/test/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4253 2023-04-05 13:18:16.000000 FORD-6.2.4/test/test_corpus.py
--rw-r--r--   0 runner    (1001) docker     (123)    14620 2023-04-05 13:18:16.000000 FORD-6.2.4/test/test_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     9493 2023-04-05 13:18:16.000000 FORD-6.2.4/test/test_graphs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5026 2023-04-05 13:18:16.000000 FORD-6.2.4/test/test_initialisation.py
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-04-05 13:18:16.000000 FORD-6.2.4/test/test_md_environ.py
--rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-04-05 13:18:16.000000 FORD-6.2.4/test/test_md_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-04-05 13:18:16.000000 FORD-6.2.4/test/test_md_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-04-05 13:18:16.000000 FORD-6.2.4/test/test_pagetree.py
--rw-r--r--   0 runner    (1001) docker     (123)    26751 2023-04-05 13:18:16.000000 FORD-6.2.4/test/test_project.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 13:18:27.961084 FORD-6.2.4/test/test_projects/
--rw-r--r--   0 runner    (1001) docker     (123)     5014 2023-04-05 13:18:16.000000 FORD-6.2.4/test/test_projects/test_external_project.py
--rw-r--r--   0 runner    (1001) docker     (123)     5832 2023-04-05 13:18:16.000000 FORD-6.2.4/test/test_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    43073 2023-04-05 13:18:16.000000 FORD-6.2.4/test/test_sourceform.py
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-04-05 13:18:16.000000 FORD-6.2.4/test/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 13:18:27.961084 FORD-6.2.4/test_data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 13:18:27.929084 FORD-6.2.4/test_data/external_project/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 13:18:27.961084 FORD-6.2.4/test_data/external_project/external_project/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-05 13:18:16.000000 FORD-6.2.4/test_data/external_project/external_project/doc.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 13:18:27.961084 FORD-6.2.4/test_data/external_project/external_project/src/
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-04-05 13:18:16.000000 FORD-6.2.4/test_data/external_project/external_project/src/external.f90
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 13:18:27.961084 FORD-6.2.4/test_data/external_project/top_level_project/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-04-05 13:18:16.000000 FORD-6.2.4/test_data/external_project/top_level_project/doc.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 13:18:27.961084 FORD-6.2.4/test_data/external_project/top_level_project/src/
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-04-05 13:18:16.000000 FORD-6.2.4/test_data/external_project/top_level_project/src/top_level.f90
--rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-04-05 13:18:16.000000 FORD-6.2.4/test_data/ford_issues_bad.f90
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-04-05 13:18:16.000000 FORD-6.2.4/test_data/ford_issues_ok.f90
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-04-05 13:18:16.000000 FORD-6.2.4/test_data/ford_issues_ok_expected.f90
--rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-04-05 13:18:16.000000 FORD-6.2.4/test_data/ford_test_program.f90
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-04-05 13:18:16.000000 FORD-6.2.4/test_data/ford_test_program_expected.f90
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:00:12.432575 FORD-6.2.5/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-05 16:59:55.000000 FORD-6.2.5/.git-blame-ignore-revs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:00:12.388575 FORD-6.2.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:00:12.408575 FORD-6.2.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-05-05 16:59:55.000000 FORD-6.2.5/.github/workflows/black.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-05-05 16:59:55.000000 FORD-6.2.5/.github/workflows/corpus_regressions.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-05-05 16:59:55.000000 FORD-6.2.5/.github/workflows/python_publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-05 16:59:55.000000 FORD-6.2.5/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-05 16:59:55.000000 FORD-6.2.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-05 16:59:55.000000 FORD-6.2.5/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)  4225846 2023-05-05 16:59:55.000000 FORD-6.2.5/2003standard.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)  8053119 2023-05-05 16:59:55.000000 FORD-6.2.5/2008standard.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)    30503 2023-05-05 16:59:55.000000 FORD-6.2.5/CHANGELOG.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:00:12.408575 FORD-6.2.5/FORD.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6183 2023-05-05 17:00:12.000000 FORD-6.2.5/FORD.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-05-05 17:00:12.000000 FORD-6.2.5/FORD.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 17:00:12.000000 FORD-6.2.5/FORD.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-05 17:00:12.000000 FORD-6.2.5/FORD.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-05-05 17:00:12.000000 FORD-6.2.5/FORD.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-05 17:00:12.000000 FORD-6.2.5/FORD.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35120 2023-05-05 16:59:55.000000 FORD-6.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-05 16:59:55.000000 FORD-6.2.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6183 2023-05-05 17:00:12.432575 FORD-6.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4879 2023-05-05 16:59:55.000000 FORD-6.2.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:00:12.408575 FORD-6.2.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-05 16:59:55.000000 FORD-6.2.5/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:00:12.408575 FORD-6.2.5/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-05 16:59:55.000000 FORD-6.2.5/docs/api/ford.fixed2free2.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-05 16:59:55.000000 FORD-6.2.5/docs/api/ford.fortran_project.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-05 16:59:55.000000 FORD-6.2.5/docs/api/ford.graphs.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-05 16:59:55.000000 FORD-6.2.5/docs/api/ford.intrinsics.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-05 16:59:55.000000 FORD-6.2.5/docs/api/ford.md_environ.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-05 16:59:55.000000 FORD-6.2.5/docs/api/ford.md_striped_table.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-05 16:59:55.000000 FORD-6.2.5/docs/api/ford.output.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-05 16:59:55.000000 FORD-6.2.5/docs/api/ford.pagetree.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-05 16:59:55.000000 FORD-6.2.5/docs/api/ford.reader.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-05-05 16:59:55.000000 FORD-6.2.5/docs/api/ford.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-05 16:59:55.000000 FORD-6.2.5/docs/api/ford.sourceform.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-05 16:59:55.000000 FORD-6.2.5/docs/api/ford.tipue_search.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-05 16:59:55.000000 FORD-6.2.5/docs/api/ford.utils.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-05 16:59:55.000000 FORD-6.2.5/docs/api/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-05-05 16:59:55.000000 FORD-6.2.5/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:00:12.408575 FORD-6.2.5/docs/developers_guide/
+-rw-r--r--   0 runner    (1001) docker     (123)     3674 2023-05-05 16:59:55.000000 FORD-6.2.5/docs/developers_guide/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5875 2023-05-05 16:59:55.000000 FORD-6.2.5/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-05-05 16:59:55.000000 FORD-6.2.5/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:00:12.412575 FORD-6.2.5/docs/user_guide/
+-rw-r--r--   0 runner    (1001) docker     (123)    11896 2023-05-05 16:59:55.000000 FORD-6.2.5/docs/user_guide/callgraph.png
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-05 16:59:55.000000 FORD-6.2.5/docs/user_guide/command_line_options.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-05-05 16:59:55.000000 FORD-6.2.5/docs/user_guide/documentation_meta_data.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-05-05 16:59:55.000000 FORD-6.2.5/docs/user_guide/getting_started.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-05 16:59:55.000000 FORD-6.2.5/docs/user_guide/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-05-05 16:59:55.000000 FORD-6.2.5/docs/user_guide/limitation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    72521 2023-05-05 16:59:55.000000 FORD-6.2.5/docs/user_guide/output-example.png
+-rw-r--r--   0 runner    (1001) docker     (123)   132134 2023-05-05 16:59:55.000000 FORD-6.2.5/docs/user_guide/pages-example.png
+-rw-r--r--   0 runner    (1001) docker     (123)    26471 2023-05-05 16:59:55.000000 FORD-6.2.5/docs/user_guide/project_file_options.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-05-05 16:59:55.000000 FORD-6.2.5/docs/user_guide/running_ford.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    40179 2023-05-05 16:59:55.000000 FORD-6.2.5/docs/user_guide/say_hello_example.png
+-rw-r--r--   0 runner    (1001) docker     (123)    13335 2023-05-05 16:59:55.000000 FORD-6.2.5/docs/user_guide/writing_documentation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5639 2023-05-05 16:59:55.000000 FORD-6.2.5/docs/user_guide/writing_pages.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:00:12.412575 FORD-6.2.5/example/
+-rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-05-05 16:59:55.000000 FORD-6.2.5/example/example-project-file.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:00:12.412575 FORD-6.2.5/example/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:00:12.412575 FORD-6.2.5/example/src/excluded_directory/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-05 16:59:55.000000 FORD-6.2.5/example/src/excluded_directory/this_file_will_not_be_included.f90
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-05 16:59:55.000000 FORD-6.2.5/example/src/excluded_file.f90
+-rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-05-05 16:59:55.000000 FORD-6.2.5/example/src/ford_example_type.f90
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-05-05 16:59:55.000000 FORD-6.2.5/example/src/ford_f77_example.f
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-05-05 16:59:55.000000 FORD-6.2.5/example/src/ford_interfaces.f90
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-05-05 16:59:55.000000 FORD-6.2.5/example/src/ford_test_module.fpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-05-05 16:59:55.000000 FORD-6.2.5/example/src/ford_test_program.f90
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:00:12.416575 FORD-6.2.5/ford/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    21883 2023-05-05 16:59:55.000000 FORD-6.2.5/ford/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-05 16:59:55.000000 FORD-6.2.5/ford/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-05 17:00:12.000000 FORD-6.2.5/ford/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17815 2023-05-05 16:59:55.000000 FORD-6.2.5/ford/config.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:00:12.416575 FORD-6.2.5/ford/css/
+-rw-r--r--   0 runner    (1001) docker     (123)   126891 2023-05-05 16:59:55.000000 FORD-6.2.5/ford/css/bootstrap.css
+-rw-r--r--   0 runner    (1001) docker     (123)   105249 2023-05-05 16:59:55.000000 FORD-6.2.5/ford/css/bootstrap.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    26651 2023-05-05 16:59:55.000000 FORD-6.2.5/ford/css/font-awesome.css
+-rw-r--r--   0 runner    (1001) docker     (123)    21984 2023-05-05 16:59:55.000000 FORD-6.2.5/ford/css/font-awesome.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)     5232 2023-05-05 16:59:55.000000 FORD-6.2.5/ford/css/local.css
+-rw-r--r--   0 runner    (1001) docker     (123)     3442 2023-05-05 16:59:55.000000 FORD-6.2.5/ford/css/pygments.css
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-05-05 16:59:55.000000 FORD-6.2.5/ford/favicon.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-05-05 16:59:55.000000 FORD-6.2.5/ford/fixed2free2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:00:12.420575 FORD-6.2.5/ford/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)    85908 2023-05-05 16:59:55.000000 FORD-6.2.5/ford/fonts/FontAwesome.otf
+-rw-r--r--   0 runner    (1001) docker     (123)    56006 2023-05-05 16:59:55.000000 FORD-6.2.5/ford/fonts/fontawesome-webfont.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   287007 2023-05-05 16:59:55.000000 FORD-6.2.5/ford/fonts/fontawesome-webfont.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   112160 2023-05-05 16:59:55.000000 FORD-6.2.5/ford/fonts/fontawesome-webfont.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    65452 2023-05-05 16:59:55.000000 FORD-6.2.5/ford/fonts/fontawesome-webfont.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    20335 2023-05-05 16:59:55.000000 FORD-6.2.5/ford/fonts/glyphicons-halflings-regular.eot
+-rw-r--r--   0 runner    (1001) docker     (123)    62926 2023-05-05 16:59:55.000000 FORD-6.2.5/ford/fonts/glyphicons-halflings-regular.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    41280 2023-05-05 16:59:55.000000 FORD-6.2.5/ford/fonts/glyphicons-halflings-regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    23320 2023-05-05 16:59:55.000000 FORD-6.2.5/ford/fonts/glyphicons-halflings-regular.woff
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15161 2023-05-05 16:59:55.000000 FORD-6.2.5/ford/fortran_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45931 2023-05-05 16:59:55.000000 FORD-6.2.5/ford/graphs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7191 2023-05-05 16:59:55.000000 FORD-6.2.5/ford/intrinsics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:00:12.420575 FORD-6.2.5/ford/js/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:00:12.420575 FORD-6.2.5/ford/js/MathJax-config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 16:59:55.000000 FORD-6.2.5/ford/js/MathJax-config/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    67155 2023-05-05 16:59:55.000000 FORD-6.2.5/ford/js/bootstrap.js
+-rw-r--r--   0 runner    (1001) docker     (123)    35601 2023-05-05 16:59:55.000000 FORD-6.2.5/ford/js/bootstrap.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-05-05 16:59:55.000000 FORD-6.2.5/ford/js/ie10-viewport-bug-workaround.js
+-rw-r--r--   0 runner    (1001) docker     (123)    84320 2023-05-05 16:59:55.000000 FORD-6.2.5/ford/js/jquery-2.1.3.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    28810 2023-05-05 16:59:55.000000 FORD-6.2.5/ford/js/svg-pan-zoom.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-05-05 16:59:55.000000 FORD-6.2.5/ford/md_environ.py
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-05-05 16:59:55.000000 FORD-6.2.5/ford/md_striped_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17032 2023-05-05 16:59:55.000000 FORD-6.2.5/ford/output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6014 2023-05-05 16:59:55.000000 FORD-6.2.5/ford/pagetree.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16542 2023-05-05 16:59:55.000000 FORD-6.2.5/ford/reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)   109424 2023-05-05 16:59:55.000000 FORD-6.2.5/ford/sourceform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:00:12.424575 FORD-6.2.5/ford/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-05-05 16:59:55.000000 FORD-6.2.5/ford/templates/absint_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)    10765 2023-05-05 16:59:55.000000 FORD-6.2.5/ford/templates/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-05-05 16:59:55.000000 FORD-6.2.5/ford/templates/block_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-05-05 16:59:55.000000 FORD-6.2.5/ford/templates/block_page.html
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-05-05 16:59:55.000000 FORD-6.2.5/ford/templates/file_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-05-05 16:59:55.000000 FORD-6.2.5/ford/templates/file_page.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-05-05 16:59:55.000000 FORD-6.2.5/ford/templates/genint_page.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6468 2023-05-05 16:59:55.000000 FORD-6.2.5/ford/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-05-05 16:59:55.000000 FORD-6.2.5/ford/templates/info_page.html
+-rw-r--r--   0 runner    (1001) docker     (123)    26582 2023-05-05 16:59:55.000000 FORD-6.2.5/ford/templates/macros.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-05-05 16:59:55.000000 FORD-6.2.5/ford/templates/mod_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-05-05 16:59:55.000000 FORD-6.2.5/ford/templates/mod_page.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-05-05 16:59:55.000000 FORD-6.2.5/ford/templates/nongenint_page.html
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-05 16:59:55.000000 FORD-6.2.5/ford/templates/proc_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-05-05 16:59:55.000000 FORD-6.2.5/ford/templates/proc_page.html
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-05-05 16:59:55.000000 FORD-6.2.5/ford/templates/prog_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-05-05 16:59:55.000000 FORD-6.2.5/ford/templates/prog_page.html
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-05 16:59:55.000000 FORD-6.2.5/ford/templates/search.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3210 2023-05-05 16:59:55.000000 FORD-6.2.5/ford/templates/type_page.html
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-05-05 16:59:55.000000 FORD-6.2.5/ford/templates/types_list.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3454 2023-05-05 16:59:55.000000 FORD-6.2.5/ford/tipue_search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:00:12.428575 FORD-6.2.5/ford/tipuesearch/
+-rw-r--r--   0 runner    (1001) docker     (123)    12292 2023-05-05 16:59:55.000000 FORD-6.2.5/ford/tipuesearch/.DS_Store
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:00:12.428575 FORD-6.2.5/ford/tipuesearch/img/
+-rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-05-05 16:59:55.000000 FORD-6.2.5/ford/tipuesearch/img/.DS_Store
+-rw-r--r--   0 runner    (1001) docker     (123)     4178 2023-05-05 16:59:55.000000 FORD-6.2.5/ford/tipuesearch/img/loader.gif
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-05-05 16:59:55.000000 FORD-6.2.5/ford/tipuesearch/img/search.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-05-05 16:59:55.000000 FORD-6.2.5/ford/tipuesearch/tipuesearch.css
+-rw-r--r--   0 runner    (1001) docker     (123)    22505 2023-05-05 16:59:55.000000 FORD-6.2.5/ford/tipuesearch/tipuesearch.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6784 2023-05-05 16:59:55.000000 FORD-6.2.5/ford/tipuesearch/tipuesearch.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-05 16:59:55.000000 FORD-6.2.5/ford/tipuesearch/tipuesearch_set.js
+-rw-r--r--   0 runner    (1001) docker     (123)    18196 2023-05-05 16:59:55.000000 FORD-6.2.5/ford/utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      138 2023-05-05 16:59:55.000000 FORD-6.2.5/ford.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72521 2023-05-05 16:59:55.000000 FORD-6.2.5/output-example.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-05-05 16:59:55.000000 FORD-6.2.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-05 16:59:55.000000 FORD-6.2.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 17:00:12.432575 FORD-6.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-05 16:59:55.000000 FORD-6.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:00:12.432575 FORD-6.2.5/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-05-05 16:59:55.000000 FORD-6.2.5/test/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4253 2023-05-05 16:59:55.000000 FORD-6.2.5/test/test_corpus.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14620 2023-05-05 16:59:55.000000 FORD-6.2.5/test/test_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10087 2023-05-05 16:59:55.000000 FORD-6.2.5/test/test_graphs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5026 2023-05-05 16:59:55.000000 FORD-6.2.5/test/test_initialisation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-05-05 16:59:55.000000 FORD-6.2.5/test/test_md_environ.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-05-05 16:59:55.000000 FORD-6.2.5/test/test_md_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-05-05 16:59:55.000000 FORD-6.2.5/test/test_md_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-05-05 16:59:55.000000 FORD-6.2.5/test/test_pagetree.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26751 2023-05-05 16:59:55.000000 FORD-6.2.5/test/test_project.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:00:12.432575 FORD-6.2.5/test/test_projects/
+-rw-r--r--   0 runner    (1001) docker     (123)     5014 2023-05-05 16:59:55.000000 FORD-6.2.5/test/test_projects/test_external_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5832 2023-05-05 16:59:55.000000 FORD-6.2.5/test/test_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44857 2023-05-05 16:59:55.000000 FORD-6.2.5/test/test_sourceform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-05-05 16:59:55.000000 FORD-6.2.5/test/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:00:12.432575 FORD-6.2.5/test_data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:00:12.388575 FORD-6.2.5/test_data/external_project/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:00:12.432575 FORD-6.2.5/test_data/external_project/external_project/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-05 16:59:55.000000 FORD-6.2.5/test_data/external_project/external_project/doc.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:00:12.432575 FORD-6.2.5/test_data/external_project/external_project/src/
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-05-05 16:59:55.000000 FORD-6.2.5/test_data/external_project/external_project/src/external.f90
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:00:12.432575 FORD-6.2.5/test_data/external_project/top_level_project/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-05 16:59:55.000000 FORD-6.2.5/test_data/external_project/top_level_project/doc.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:00:12.432575 FORD-6.2.5/test_data/external_project/top_level_project/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-05-05 16:59:55.000000 FORD-6.2.5/test_data/external_project/top_level_project/src/top_level.f90
+-rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-05-05 16:59:55.000000 FORD-6.2.5/test_data/ford_issues_bad.f90
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-05-05 16:59:55.000000 FORD-6.2.5/test_data/ford_issues_ok.f90
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-05-05 16:59:55.000000 FORD-6.2.5/test_data/ford_issues_ok_expected.f90
+-rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-05-05 16:59:55.000000 FORD-6.2.5/test_data/ford_test_program.f90
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-05-05 16:59:55.000000 FORD-6.2.5/test_data/ford_test_program_expected.f90
```

### Comparing `FORD-6.2.4/.github/workflows/black.yml` & `FORD-6.2.5/.github/workflows/black.yml`

 * *Files identical despite different names*

### Comparing `FORD-6.2.4/.github/workflows/corpus_regressions.yml` & `FORD-6.2.5/.github/workflows/corpus_regressions.yml`

 * *Files 27% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 name: "Corpus regressions"
-on:
-  push:
-    branches: "master"
+on: pull_request
 
 jobs:
   regression:
     runs-on: ubuntu-latest
     steps:
     - uses: actions/checkout@v3
     - name: Set up Python
```

### Comparing `FORD-6.2.4/.github/workflows/python_publish.yml` & `FORD-6.2.5/.github/workflows/python_publish.yml`

 * *Files identical despite different names*

### Comparing `FORD-6.2.4/.github/workflows/test.yml` & `FORD-6.2.5/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `FORD-6.2.4/.readthedocs.yaml` & `FORD-6.2.5/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `FORD-6.2.4/2003standard.pdf` & `FORD-6.2.5/2003standard.pdf`

 * *Files identical despite different names*

### Comparing `FORD-6.2.4/2008standard.pdf` & `FORD-6.2.5/2008standard.pdf`

 * *Files identical despite different names*

### Comparing `FORD-6.2.4/CHANGELOG.md` & `FORD-6.2.5/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `FORD-6.2.4/FORD.egg-info/PKG-INFO` & `FORD-6.2.5/FORD.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FORD
-Version: 6.2.4
+Version: 6.2.5
 Summary: FORD (FORtran Documenter) is an automatic documentation generator for modern Fortran programs.
 Author-email: Chris MacMackin <cmacmackin@gmail.com>, Peter Hill <peter.hill@york.ac.uk>
 License: GPLv3
 Project-URL: Source, https://github.com/Fortran-FOSS-Programmers/ford
 Project-URL: Tracker, https://github.com/Fortran-FOSS-Programmers/ford/issues
 Project-URL: Documentation, https://forddocs.readthedocs.io/en/latest/
 Keywords: Markdown,Fortran,documentation,comments
```

### Comparing `FORD-6.2.4/FORD.egg-info/SOURCES.txt` & `FORD-6.2.5/FORD.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `FORD-6.2.4/LICENSE` & `FORD-6.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `FORD-6.2.4/PKG-INFO` & `FORD-6.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FORD
-Version: 6.2.4
+Version: 6.2.5
 Summary: FORD (FORtran Documenter) is an automatic documentation generator for modern Fortran programs.
 Author-email: Chris MacMackin <cmacmackin@gmail.com>, Peter Hill <peter.hill@york.ac.uk>
 License: GPLv3
 Project-URL: Source, https://github.com/Fortran-FOSS-Programmers/ford
 Project-URL: Tracker, https://github.com/Fortran-FOSS-Programmers/ford/issues
 Project-URL: Documentation, https://forddocs.readthedocs.io/en/latest/
 Keywords: Markdown,Fortran,documentation,comments
```

### Comparing `FORD-6.2.4/README.md` & `FORD-6.2.5/README.md`

 * *Files identical despite different names*

### Comparing `FORD-6.2.4/docs/Makefile` & `FORD-6.2.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `FORD-6.2.4/docs/conf.py` & `FORD-6.2.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `FORD-6.2.4/docs/developers_guide/index.rst` & `FORD-6.2.5/docs/developers_guide/index.rst`

 * *Files identical despite different names*

### Comparing `FORD-6.2.4/docs/index.rst` & `FORD-6.2.5/docs/index.rst`

 * *Files identical despite different names*

### Comparing `FORD-6.2.4/docs/make.bat` & `FORD-6.2.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `FORD-6.2.4/docs/user_guide/callgraph.png` & `FORD-6.2.5/docs/user_guide/callgraph.png`

 * *Files identical despite different names*

### Comparing `FORD-6.2.4/docs/user_guide/documentation_meta_data.rst` & `FORD-6.2.5/docs/user_guide/documentation_meta_data.rst`

 * *Files identical despite different names*

### Comparing `FORD-6.2.4/docs/user_guide/getting_started.rst` & `FORD-6.2.5/docs/user_guide/getting_started.rst`

 * *Files identical despite different names*

### Comparing `FORD-6.2.4/docs/user_guide/limitation.rst` & `FORD-6.2.5/docs/user_guide/limitation.rst`

 * *Files identical despite different names*

### Comparing `FORD-6.2.4/docs/user_guide/output-example.png` & `FORD-6.2.5/docs/user_guide/output-example.png`

 * *Files identical despite different names*

### Comparing `FORD-6.2.4/docs/user_guide/pages-example.png` & `FORD-6.2.5/docs/user_guide/pages-example.png`

 * *Files identical despite different names*

### Comparing `FORD-6.2.4/docs/user_guide/project_file_options.rst` & `FORD-6.2.5/docs/user_guide/project_file_options.rst`

 * *Files identical despite different names*

### Comparing `FORD-6.2.4/docs/user_guide/running_ford.rst` & `FORD-6.2.5/docs/user_guide/running_ford.rst`

 * *Files identical despite different names*

### Comparing `FORD-6.2.4/docs/user_guide/say_hello_example.png` & `FORD-6.2.5/docs/user_guide/say_hello_example.png`

 * *Files identical despite different names*

### Comparing `FORD-6.2.4/docs/user_guide/writing_documentation.rst` & `FORD-6.2.5/docs/user_guide/writing_documentation.rst`

 * *Files identical despite different names*

### Comparing `FORD-6.2.4/docs/user_guide/writing_pages.rst` & `FORD-6.2.5/docs/user_guide/writing_pages.rst`

 * *Files identical despite different names*

### Comparing `FORD-6.2.4/example/example-project-file.md` & `FORD-6.2.5/example/example-project-file.md`

 * *Files identical despite different names*

### Comparing `FORD-6.2.4/example/src/ford_example_type.f90` & `FORD-6.2.5/example/src/ford_example_type.f90`

 * *Files identical despite different names*

### Comparing `FORD-6.2.4/example/src/ford_f77_example.f` & `FORD-6.2.5/example/src/ford_f77_example.f`

 * *Files identical despite different names*

### Comparing `FORD-6.2.4/example/src/ford_interfaces.f90` & `FORD-6.2.5/example/src/ford_interfaces.f90`

 * *Files identical despite different names*

### Comparing `FORD-6.2.4/example/src/ford_test_module.fpp` & `FORD-6.2.5/example/src/ford_test_module.fpp`

 * *Files identical despite different names*

### Comparing `FORD-6.2.4/example/src/ford_test_program.f90` & `FORD-6.2.5/example/src/ford_test_program.f90`

 * *Files identical despite different names*

### Comparing `FORD-6.2.4/ford/__init__.py` & `FORD-6.2.5/ford/__init__.py`

 * *Files identical despite different names*

### Comparing `FORD-6.2.4/ford/config.json` & `FORD-6.2.5/ford/config.json`

 * *Files identical despite different names*

### Comparing `FORD-6.2.4/ford/css/bootstrap.css` & `FORD-6.2.5/ford/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `FORD-6.2.4/ford/css/bootstrap.min.css` & `FORD-6.2.5/ford/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `FORD-6.2.4/ford/css/font-awesome.css` & `FORD-6.2.5/ford/css/font-awesome.css`

 * *Files identical despite different names*

### Comparing `FORD-6.2.4/ford/css/font-awesome.min.css` & `FORD-6.2.5/ford/css/font-awesome.min.css`

 * *Files identical despite different names*

### Comparing `FORD-6.2.4/ford/css/local.css` & `FORD-6.2.5/ford/css/local.css`

 * *Files identical despite different names*

### Comparing `FORD-6.2.4/ford/css/pygments.css` & `FORD-6.2.5/ford/css/pygments.css`

 * *Files identical despite different names*

### Comparing `FORD-6.2.4/ford/favicon.png` & `FORD-6.2.5/ford/favicon.png`

 * *Files identical despite different names*

### Comparing `FORD-6.2.4/ford/fixed2free2.py` & `FORD-6.2.5/ford/fixed2free2.py`

 * *Files identical despite different names*

### Comparing `FORD-6.2.4/ford/fonts/FontAwesome.otf` & `FORD-6.2.5/ford/fonts/FontAwesome.otf`

 * *Files identical despite different names*

### Comparing `FORD-6.2.4/ford/fonts/fontawesome-webfont.eot` & `FORD-6.2.5/ford/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `FORD-6.2.4/ford/fonts/fontawesome-webfont.svg` & `FORD-6.2.5/ford/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `FORD-6.2.4/ford/fonts/fontawesome-webfont.ttf` & `FORD-6.2.5/ford/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `FORD-6.2.4/ford/fonts/fontawesome-webfont.woff` & `FORD-6.2.5/ford/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `FORD-6.2.4/ford/fonts/glyphicons-halflings-regular.eot` & `FORD-6.2.5/ford/fonts/glyphicons-halflings-regular.eot`

 * *Files identical despite different names*

### Comparing `FORD-6.2.4/ford/fonts/glyphicons-halflings-regular.svg` & `FORD-6.2.5/ford/fonts/glyphicons-halflings-regular.svg`

 * *Files identical despite different names*

### Comparing `FORD-6.2.4/ford/fonts/glyphicons-halflings-regular.ttf` & `FORD-6.2.5/ford/fonts/glyphicons-halflings-regular.ttf`

 * *Files identical despite different names*

### Comparing `FORD-6.2.4/ford/fonts/glyphicons-halflings-regular.woff` & `FORD-6.2.5/ford/fonts/glyphicons-halflings-regular.woff`

 * *Files identical despite different names*

### Comparing `FORD-6.2.4/ford/fortran_project.py` & `FORD-6.2.5/ford/fortran_project.py`

 * *Files identical despite different names*

### Comparing `FORD-6.2.4/ford/graphs.py` & `FORD-6.2.5/ford/graphs.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,22 +45,21 @@
     ExternalProgram,
     ExternalSourceFile,
     ExternalSubmodule,
     ExternalSubroutine,
     ExternalType,
     FortranBlockData,
     FortranContainer,
-    FortranFunction,
     FortranInterface,
     FortranModule,
+    FortranProcedure,
     FortranProgram,
     FortranSourceFile,
     FortranSubmodule,
     FortranSubmoduleProcedure,
-    FortranSubroutine,
     FortranType,
 )
 
 try:
     graphviz_version()
     graphviz_installed = True
 except ExecutableNotFound:
@@ -92,20 +91,15 @@
 def is_type(obj):
     return isinstance(obj, FortranType)
 
 
 def is_proc(obj):
     return isinstance(
         obj,
-        (
-            FortranFunction,
-            FortranSubroutine,
-            FortranInterface,
-            FortranSubmoduleProcedure,
-        ),
+        (FortranProcedure, FortranInterface, FortranSubmoduleProcedure),
     )
 
 
 def is_program(obj):
     return isinstance(obj, FortranProgram)
 
 
@@ -226,15 +220,15 @@
         if isinstance(mod, str):
             # Most likely a third-party module
             mod = ExternalModule(mod)
         return cast(ModNode, self.get_node(mod))
 
     def get_procedure_node(
         self,
-        procedure: Union[FortranSubroutine, FortranFunction, str],
+        procedure: Union[FortranProcedure, str],
         hist: NodeCollection,
     ) -> ProcNode:
         if isinstance(procedure, str):
             # Most likely a third-party procedure
             procedure = ExternalSubroutine(procedure)
             procedure.proctype = "unknown"
 
@@ -418,17 +412,23 @@
         return ProcNode.COLOURS.get(self.proctype.lower(), super().colour)
 
     def __init__(self, obj, gd, hist=None):
         # ToDo: Figure out appropriate way to handle interfaces to routines in submodules.
         self.proctype = getattr(obj, "proctype", "")
         super().__init__(obj, gd)
 
-        if gd.show_proc_parent:
-            if parent := getattr(obj, "parent", None):
-                self.attribs["label"] = f"{parent.name}::{self.name}"
+        if parent := getattr(obj, "parent", None):
+            parent_label = f"{parent.name}::"
+        else:
+            parent_label = ""
+        if binding := getattr(obj, "binding", None):
+            binding_label = f"{binding.parent.name}%"
+        else:
+            binding_label = ""
+        self.attribs["label"] = f"{parent_label}{binding_label}{self.name}"
 
         self.uses = set()
         self.calls = set()
         self.called_by = set()
         self.interfaces = set()
         self.interfaced_by = set()
```

### Comparing `FORD-6.2.4/ford/intrinsics.py` & `FORD-6.2.5/ford/intrinsics.py`

 * *Files identical despite different names*

### Comparing `FORD-6.2.4/ford/js/bootstrap.js` & `FORD-6.2.5/ford/js/bootstrap.js`

 * *Files identical despite different names*

### Comparing `FORD-6.2.4/ford/js/bootstrap.min.js` & `FORD-6.2.5/ford/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `FORD-6.2.4/ford/js/ie10-viewport-bug-workaround.js` & `FORD-6.2.5/ford/js/ie10-viewport-bug-workaround.js`

 * *Files identical despite different names*

### Comparing `FORD-6.2.4/ford/js/jquery-2.1.3.min.js` & `FORD-6.2.5/ford/js/jquery-2.1.3.min.js`

 * *Files identical despite different names*

### Comparing `FORD-6.2.4/ford/js/svg-pan-zoom.min.js` & `FORD-6.2.5/ford/js/svg-pan-zoom.min.js`

 * *Files identical despite different names*

### Comparing `FORD-6.2.4/ford/md_environ.py` & `FORD-6.2.5/ford/md_environ.py`

 * *Files identical despite different names*

### Comparing `FORD-6.2.4/ford/md_striped_table.py` & `FORD-6.2.5/ford/md_striped_table.py`

 * *Files identical despite different names*

### Comparing `FORD-6.2.4/ford/output.py` & `FORD-6.2.5/ford/output.py`

 * *Files identical despite different names*

### Comparing `FORD-6.2.4/ford/pagetree.py` & `FORD-6.2.5/ford/pagetree.py`

 * *Files identical despite different names*

### Comparing `FORD-6.2.4/ford/reader.py` & `FORD-6.2.5/ford/reader.py`

 * *Files identical despite different names*

### Comparing `FORD-6.2.4/ford/sourceform.py` & `FORD-6.2.5/ford/sourceform.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 from collections import defaultdict
 from dataclasses import dataclass
 import sys
 import re
 import os.path
 import copy
 import textwrap
-from typing import List, Tuple, Optional, Union
+from typing import List, Tuple, Optional, Union, Sequence, Dict
 from itertools import chain
 
 # Python 2 or 3:
 if sys.version_info[0] > 2:
     from urllib.parse import quote
 else:
     from urllib import quote
@@ -66,15 +66,15 @@
 NBSP_RE = re.compile(r" (?= )|(?<= ) ")
 DIM_RE = re.compile(r"^\w+\s*(\(.*\))\s*$")
 
 
 base_url = ""
 
 
-class FortranBase(object):
+class FortranBase:
     """
     An object containing the data common to all of the classes used to represent
     Fortran data.
     """
 
     IS_SPOOF = False
 
@@ -130,68 +130,54 @@
         cur = self.parent
         while cur:
             self.hierarchy.append(cur)
             cur = cur.parent
         self.hierarchy.reverse()
 
     @property
-    def filename(self):
+    def filename(self) -> str:
         """Name of the file containing this entity"""
         # If `hierarchy` is empty, it's probably because it's a source
         # file, so we can use its name directly
         return self.hierarchy[0].name if self.hierarchy else self.name
 
-    def get_dir(self):
-        if (
-            type(self)
-            in [
-                FortranSubroutine,
-                ExternalSubroutine,
-                FortranFunction,
-                ExternalFunction,
-            ]
-            and type(self.parent) in [FortranInterface, ExternalInterface]
-            and not self.parent.generic
-        ):
-            return "interface"
-        elif type(self) is FortranSubmodule:
-            return "module"
-        elif type(self) in [
-            FortranSourceFile,
-            FortranProgram,
-            FortranModule,
-            GenericSource,
-            FortranBlockData,
-            ExternalModule,
-        ] or (
-            type(self)
-            in [
-                FortranType,
-                ExternalType,
-                FortranInterface,
-                ExternalInterface,
-                FortranFunction,
-                ExternalFunction,
-                FortranSubroutine,
-                ExternalSubroutine,
-                FortranSubmoduleProcedure,
-            ]
-            and type(self.parent)
-            in [
+    def get_dir(self) -> Optional[str]:
+        if isinstance(
+            self,
+            (
                 FortranSourceFile,
                 FortranProgram,
                 FortranModule,
-                FortranSubmodule,
+                GenericSource,
                 FortranBlockData,
-                ExternalModule,
-            ]
+            ),
+        ) or (
+            isinstance(
+                self,
+                (
+                    FortranType,
+                    FortranInterface,
+                    FortranProcedure,
+                    FortranSubmoduleProcedure,
+                ),
+            )
+            and isinstance(
+                self.parent,
+                (
+                    FortranSourceFile,
+                    FortranProgram,
+                    FortranModule,
+                    FortranSubmodule,
+                    FortranBlockData,
+                ),
+            )
         ):
             return self.obj
-        else:
-            return None
+
+        return None
 
     def get_url(self):
         if hasattr(self, "external_url"):
             return self.external_url
         outstr = "{0}/{1}/{2}.html"
         loc = self.get_dir()
         if loc:
@@ -229,20 +215,14 @@
                 )
             )
         return description
 
     @property
     def ident(self) -> str:
         """Return a unique identifier for this object"""
-        if (
-            isinstance(self, (FortranSubroutine, FortranFunction))
-            and isinstance(self.parent, FortranInterface)
-            and not self.parent.generic
-        ):
-            return namelist.get_name(self.parent)
         return namelist.get_name(self)
 
     @property
     def anchor(self) -> str:
         """Return a string suitable for an HTML anchor link"""
         return f"{self.obj}-{quote(self.ident)}"
 
@@ -519,14 +499,25 @@
                 "subroutines",
                 "types",
                 "variables",
             ),
             filter(None, (getattr(self, item, None) for item in non_list_children)),
         )
 
+    def _should_display(self, item) -> bool:
+        """Return True if item should be displayed"""
+        if self.settings["hide_undoc"] and not item.doc:
+            return False
+        return item.permission in self.display
+
+    def filter_display(self, collection: Sequence) -> List:
+        """Remove items from collection if they shouldn't be displayed"""
+
+        return [obj for obj in collection if self._should_display(obj)]
+
 
 class FortranContainer(FortranBase):
     """
     A class on which any classes requiring further parsing are based.
     """
 
     ATTRIB_RE = re.compile(
@@ -552,43 +543,56 @@
         (?::\s*(?P<parent_submod>\w+))?\s*\)  # Optional parent submodule
         \s*(?P<name>\w+)                      # This submodule's name
         $""",
         re.IGNORECASE | re.VERBOSE,
     )
     PROGRAM_RE = re.compile(r"^program(?:\s+(\w+))?$", re.IGNORECASE)
     SUBROUTINE_RE = re.compile(
-        r"^\s*(?:(.+?)\s+)?subroutine\s+(\w+)\s*(\([^()]*\))?(?:\s*bind\s*\(\s*(.*)\s*\))?$",
-        re.IGNORECASE,
+        r"""^\s*(?:(?P<attributes>.+?)\s+)?     # Optional attributes
+        subroutine\s+(?P<name>\w+)\s*           # Required subroutine name
+        (?P<arguments>\([^()]*\))?              # Optional arguments
+        (?:\s*bind\s*\(\s*(?P<bindC>.*)\s*\))?$ # Optional C-binding""",
+        re.IGNORECASE | re.VERBOSE,
     )
     FUNCTION_RE = re.compile(
-        r"^(?:(.+?)\s+)?function\s+(\w+)\s*(\([^()]*\))?(?=(?:.*result\s*\(\s*(\w+)\s*\))?)(?=(?:.*bind\s*\(\s*(.*)\s*\))?).*$",
-        re.IGNORECASE,
+        r"""^(?:(?P<attributes>.+?)\s+)?               # Optional attributes (including type)
+        function\s+(?P<name>\w+)\s*                    # Required function name
+        (?P<arguments>\([^()]*\))?                     # Required arguments
+        (?=(?:.*result\s*\(\s*(?P<result>\w+)\s*\))?)  # Optional result name
+        (?=(?:.*bind\s*\(\s*(?P<bindC>.*)\s*\))?).*$   # Optional C-binding""",
+        re.IGNORECASE | re.VERBOSE,
     )
     TYPE_RE = re.compile(
         r"^type(?:\s+|\s*(,.*)?::\s*)((?!(?:is\s*\())\w+)\s*(\([^()]*\))?\s*$",
         re.IGNORECASE,
     )
     INTERFACE_RE = re.compile(r"^(abstract\s+)?interface(?:\s+(.+))?$", re.IGNORECASE)
-    # ~ ABS_INTERFACE_RE = re.compile(r"^abstract\s+interface(?:\s+(\S.+))?$",re.IGNORECASE)
     BOUNDPROC_RE = re.compile(
-        r"^(generic|procedure)\s*(\([^()]*\))?\s*(.*)\s*::\s*(\w.*)", re.IGNORECASE
+        r"""^(?P<generic>generic|procedure)\s*  # Required keyword
+        (?P<prototype>\([^()]*\))?\s*           # Optional interface name
+        (?:,\s*(?P<attributes>\w[^:]*))?        # Optional list of attributes
+        (?:\s*::)?\s*                           # Optional double-colon
+        (?P<names>\w.*)$                        # Required name(s)
+        """,
+        re.IGNORECASE | re.VERBOSE,
     )
     COMMON_RE = re.compile(r"^common(?:\s*/\s*(\w+)\s*/\s*|\s+)(\w+.*)", re.IGNORECASE)
     COMMON_SPLIT_RE = re.compile(r"\s*(/\s*\w+\s*/)\s*", re.IGNORECASE)
     FINAL_RE = re.compile(r"^final\s*::\s*(\w.*)", re.IGNORECASE)
     USE_RE = re.compile(
         r"^use(?:\s*(?:,\s*(?:non_)?intrinsic\s*)?::\s*|\s+)(\w+)\s*($|,.*)",
         re.IGNORECASE,
     )
     ARITH_GOTO_RE = re.compile(r"go\s*to\s*\([0-9,\s]+\)", re.IGNORECASE)
     CALL_RE = re.compile(
-        r"(?:^|[^a-zA-Z0-9_% ]\s*)(\w+)(?=\s*\(\s*(?:.*?)\s*\))", re.IGNORECASE
+        r"(?:^|[^a-zA-Z0-9_% ]\s*(?:\w+%)?)(\w+)(?=\s*\(\s*(?:.*?)\s*\))", re.IGNORECASE
     )
     SUBCALL_RE = re.compile(
-        r"^(?:if\s*\(.*\)\s*)?call\s+(\w+)\s*(?:\(\s*(.*?)\s*\))?$", re.IGNORECASE
+        r"^(?:if\s*\(.*\)\s*)?call\s+(?:\w+%)?(\w+)\s*(?:\(\s*(.*?)\s*\))?$",
+        re.IGNORECASE,
     )
     FORMAT_RE = re.compile(r"^[0-9]+\s+format\s+\(.*\)", re.IGNORECASE)
 
     VARIABLE_STRING = (
         r"^(integer|real|double\s*precision|character|complex|double\s*complex|logical|type(?!\s+is)|class(?!\s+is|\s+default)|"
         r"procedure|enumerator{})\s*((?:\(|\s\w|[:,*]).*)$"
     )
@@ -649,15 +653,15 @@
             line_lower = line.lower()
 
             if self.settings["lower"]:
                 line = line_lower
 
             # Check the various possibilities for what is on this line
             if line_lower == "contains":
-                if not incontains and type(self) in _can_have_contains:
+                if not incontains and isinstance(self, _can_have_contains):
                     incontains = True
                     if isinstance(self, FortranType):
                         child_permission = "public"
                 elif incontains:
                     self.print_error(line, "Multiple CONTAINS statements present")
                 else:
                     self.print_error(line, "Unexpected CONTAINS statement")
@@ -835,34 +839,37 @@
                 if hasattr(self, "enums"):
                     self.enums.append(FortranEnum(source, match, self, self.permission))
                     self.num_lines += self.enums[-1].num_lines - 1
                 else:
                     self.print_error(line, "Unexpected ENUM")
 
             elif (match := self.BOUNDPROC_RE.match(line)) and incontains:
-                if hasattr(self, "boundprocs"):
-                    split = match.group(4).split(",")
-                    split.reverse()
-                    if match.group(1).lower() == "generic" or len(split) == 1:
-                        self.boundprocs.append(
-                            FortranBoundProcedure(source, match, self, child_permission)
-                        )
-                    else:
-                        for bind in split:
-                            pseudo_line = line[: match.start(4)] + bind
-                            self.boundprocs.append(
-                                FortranBoundProcedure(
-                                    source,
-                                    self.BOUNDPROC_RE.match(pseudo_line),
-                                    self,
-                                    child_permission,
-                                )
-                            )
-                else:
+                if not hasattr(self, "boundprocs"):
                     self.print_error(line, "Unexpected type-bound procedure")
+                    continue
+
+                names = match["names"].split(",")
+                # Generic procedures or single name
+                if match["generic"].lower() == "generic" or len(names) == 1:
+                    self.boundprocs.append(
+                        FortranBoundProcedure(source, match, self, child_permission)
+                    )
+                    continue
+
+                # For multiple procedures, parse each one as if it
+                # were on a line by itself
+                for bind in reversed(names):
+                    pseudo_line = self.BOUNDPROC_RE.match(
+                        line[: match.start("names")] + bind
+                    )
+                    self.boundprocs.append(
+                        FortranBoundProcedure(
+                            source, pseudo_line, self, child_permission
+                        )
+                    )
 
             elif match := self.COMMON_RE.match(line):
                 if hasattr(self, "common"):
                     split = self.COMMON_SPLIT_RE.split(line)
                     if len(split) > 1:
                         for i in range(len(split) // 2):
                             pseudo_line = (
@@ -1052,66 +1059,61 @@
         if hasattr(self, "calls"):
             tmplst = []
             for call in self.calls:
                 call_low = call.lower()
                 argname = False
                 for a in getattr(self, "args", []):
                     # Consider allowing procedures passed as arguments to be included in callgraphs
-                    argname = argname or call_low == a.name.lower()
+                    argname |= call_low == a.name.lower()
                 if hasattr(self, "retvar"):
-                    argname = argname or call_low == self.retvar.name.lower()
+                    argname |= call_low == self.retvar.name.lower()
                 if (
                     not argname
                     and call_low not in self.all_vars
                     and (call_low not in self.all_types or call_low in self.all_procs)
                 ):
                     tmplst.append(call)
             self.calls = tmplst
-            fileprocs = {}
-            if self.parobj == "sourcefile":
-                for proc in self.parent.subroutines + self.parent.functions:
-                    fileprocs[proc.name.lower()] = proc
-            for i in range(len(self.calls)):
-                if self.calls[i].lower() in self.all_procs:
-                    self.calls[i] = self.all_procs[self.calls[i].lower()]
-                elif self.calls[i].lower() in fileprocs:
-                    self.calls[i] = fileprocs[self.calls[i].lower()]
-                else:
-                    for proc in project.procedures:
-                        if self.calls[i] == proc.name.lower():
-                            self.calls[i] = proc
-                            break
+
+            procedures = (
+                {proc.name.lower(): proc for proc in self.parent.routines}
+                if self.parobj == "sourcefile"
+                else {}
+            )
+            procedures.update({proc.name.lower(): proc for proc in project.procedures})
+            procedures.update(self.all_procs)
+
+            for i, call in enumerate(self.calls):
+                try:
+                    self.calls[i] = procedures[call.lower()]
+                except KeyError:
+                    pass
 
         if self.obj == "submodule":
             self.ancestry = []
             item = self
             while item.parent_submodule:
                 item = item.parent_submodule
                 self.ancestry.insert(0, item)
             self.ancestry.insert(0, item.ancestor_module)
 
         # Recurse
         for dtype in typeorder:
             if dtype in self.types:
                 dtype.correlate(project)
-        for func in self.functions:
-            func.correlate(project)
-        for subrtn in self.subroutines:
-            subrtn.correlate(project)
-        for interface in self.interfaces:
-            interface.correlate(project)
-        for absint in self.absinterfaces:
-            absint.correlate(project)
-        for var in self.variables:
-            var.correlate(project)
-        for com in self.common:
-            com.correlate(project)
-        if hasattr(self, "modprocedures"):
-            for mp in self.modprocedures:
-                mp.correlate(project)
+        for entity in self.iterator(
+            "functions",
+            "subroutines",
+            "interfaces",
+            "absinterfaces",
+            "variables",
+            "common",
+            "modprocedures",
+        ):
+            entity.correlate(project)
         if hasattr(self, "args") and not getattr(self, "mp", False):
             for arg in self.args:
                 arg.correlate(project)
         if hasattr(self, "retvar") and not getattr(self, "mp", False):
             self.retvar.correlate(project)
 
         self.sort_components()
@@ -1190,67 +1192,50 @@
         del self.attr_dict
 
     def prune(self):
         """
         Remove anything which shouldn't be displayed.
         """
 
-        def to_include(obj):
-            inc = obj.permission in self.display
-            if self.settings["hide_undoc"] and not obj.doc:
-                inc = False
-            return inc
-
         if self.obj == "proc" and not self.meta["proc_internals"]:
             self.functions = []
             self.subroutines = []
             self.types = []
             self.interfaces = []
             self.absinterfaces = []
             self.variables = []
-        else:
-            self.functions = [obj for obj in self.functions if to_include(obj)]
-            self.subroutines = [obj for obj in self.subroutines if to_include(obj)]
-            self.types = [obj for obj in self.types if to_include(obj)]
-            self.interfaces = [obj for obj in self.interfaces if to_include(obj)]
-            self.absinterfaces = [obj for obj in self.absinterfaces if to_include(obj)]
-            self.variables = [obj for obj in self.variables if to_include(obj)]
-            if hasattr(self, "modprocedures"):
-                self.modprocedures = [
-                    obj for obj in self.modprocedures if to_include(obj)
-                ]
-            if hasattr(self, "modsubroutines"):
-                self.modsubroutines = [
-                    obj for obj in self.modsubroutines if to_include(obj)
-                ]
-            if hasattr(self, "modfunctions"):
-                self.modfunctions = [
-                    obj for obj in self.modfunctions if to_include(obj)
-                ]
+            return
+
+        self.functions = self.filter_display(self.functions)
+        self.subroutines = self.filter_display(self.subroutines)
+        self.types = self.filter_display(self.types)
+        self.interfaces = self.filter_display(self.interfaces)
+        self.absinterfaces = self.filter_display(self.absinterfaces)
+        self.variables = self.filter_display(self.variables)
+        if self.obj == "submodule":
+            self.modprocedures = self.filter_display(self.modprocedures)
+            self.modsubroutines = self.filter_display(self.modsubroutines)
+            self.modfunctions = self.filter_display(self.modfunctions)
+
         # Recurse
-        for obj in self.absinterfaces:
-            obj.visible = True
         for obj in self.iterator(
-            "functions",
-            "subroutines",
-            "types",
+            "absinterfaces",
             "interfaces",
-            "modprocedures",
-            "modfunctions",
-            "modsubroutines",
         ):
             obj.visible = True
+
         for obj in self.iterator(
             "functions",
             "subroutines",
             "types",
             "modprocedures",
             "modfunctions",
             "modsubroutines",
         ):
+            obj.visible = True
             obj.prune()
 
 
 class FortranSourceFile(FortranContainer):
     """
     An object representing individual files containing Fortran code. A project
     will consist of a list of these objects. In turn, SourceFile objects will
@@ -1288,29 +1273,22 @@
             settings["fixed_length_limit"],
             preprocessor,
             settings["macro"],
             settings["include"],
             settings["encoding"],
         )
 
-        FortranContainer.__init__(self, source, "")
+        super().__init__(source, "")
         with open(self.path, "r", encoding=settings["encoding"]) as readobj:
             self.raw_src = readobj.read()
-        if self.fixed:
-            self.src = highlight(
-                self.raw_src,
-                FortranFixedLexer(),
-                HtmlFormatter(lineanchors="ln", cssclass="hl"),
-            )
-        else:
-            self.src = highlight(
-                self.raw_src,
-                FortranLexer(),
-                HtmlFormatter(lineanchors="ln", cssclass="hl"),
-            )
+
+        lexer = FortranFixedLexer() if self.fixed else FortranLexer()
+        self.src = highlight(
+            self.raw_src, lexer, HtmlFormatter(lineanchors="ln", cssclass="hl")
+        )
 
 
 class FortranModule(FortranCodeUnit):
     """
     An object representing individual modules within your source code. These
     objects contains lists of all of the module's contents, as well as its
     dependencies.
@@ -1357,15 +1335,15 @@
             if interface.generic:
                 for proc in interface.iterator("subroutines", "functions"):
                     self.all_procs[proc.name.lower()] = proc
         self.process_attribs()
         self.variables = [v for v in self.variables if "external" not in v.attribs]
 
         def should_be_public(item: FortranBase) -> bool:
-            return item.permission == "public" or item.permission == "protected"
+            return item.permission in ["public", "protected"]
 
         def filter_public(collection: list) -> dict:
             return {
                 obj.name.lower(): obj for obj in collection if should_be_public(obj)
             }
 
         self.pub_procs = filter_public(self.all_procs.values())
@@ -1431,16 +1409,21 @@
         for interface in self.interfaces:
             if not interface.abstract:
                 self.all_procs[interface.name.lower()] = interface
             if interface.generic:
                 for proc in interface.iterator("subroutines", "functions"):
                     self.all_procs[proc.name.lower()] = proc
 
+    def get_dir(self):
+        return "module"
+
 
-def _list_of_procedure_attributes(attribute_string: str) -> Tuple[List[str], str]:
+def _list_of_procedure_attributes(
+    attribute_string: Optional[str],
+) -> Tuple[List[str], str]:
     """Convert a string of attributes into a list of attributes"""
     if not attribute_string:
         return [], ""
 
     attribute_list = []
     attribute_string = attribute_string.lower()
 
@@ -1457,222 +1440,213 @@
             attribute_string = re.sub(
                 attribute, "", attribute_string, flags=re.IGNORECASE
             )
 
     return attribute_list, attribute_string.replace(" ", "")
 
 
-class FortranSubroutine(FortranCodeUnit):
-    """
-    An object representing a Fortran subroutine and holding all of said
-    subroutine's contents.
-    """
+def implicit_type(name: str) -> str:
+    """Map names to implicit types"""
 
-    def _initialize(self, line):
-        self.proctype = "Subroutine"
-        self.name = line.group(2)
-        attribstr = line.group(1)
-        self.module = False
+    if name[0].lower() in "ijklmn":
+        return "integer"
+    return "real"
+
+
+class FortranProcedure(FortranCodeUnit):
+    """Base class for subroutines and functions for common functionality"""
+
+    def _procedure_initialize(
+        self,
+        name: str,
+        arguments: Optional[str],
+        attributes: Optional[str],
+        bindC: Optional[str],
+        **kwargs,
+    ) -> str:
+        self.name = name
+        self.attribs, attribstr = _list_of_procedure_attributes(attributes)
         self.mp = False
-        self.attribs, attribstr = _list_of_procedure_attributes(attribstr)
         self.module = "module" in self.attribs
 
         self.args = []
-        if line.group(3):
-            arguments = self.SPLIT_RE.split(line.group(3)[1:-1].strip())
+        if arguments:
             # Empty argument lists will contain the empty string, so we need to remove it
-            self.args = [arg for arg in arguments if arg]
+            self.args = [
+                arg for arg in self.SPLIT_RE.split(arguments[1:-1].strip()) if arg
+            ]
 
-        self.bindC = line.group(4)
-        self.variables = []
-        self.enums = []
+        self._parse_bind_C(bindC)
+        self.variables: List[FortranVariable] = []
+        self.enums: List[FortranEnum] = []
         self.uses = []
         self.calls = []
-        self.optional_list = []
-        self.subroutines = []
-        self.functions = []
-        self.interfaces = []
-        self.absinterfaces = []
-        self.types = []
-        self.common = []
-        self.attr_dict = defaultdict(list)
-        self.param_dict = dict()
+        self.subroutines: List[FortranSubroutine] = []
+        self.functions: List[FortranFunction] = []
+        self.interfaces: List[FortranInterface] = []
+        self.absinterfaces: List[FortranInterface] = []
+        self.types: List[FortranType] = []
+        self.common: List[FortranCommon] = []
+        self.attr_dict: Dict[str, List[str]] = defaultdict(list)
+        self.param_dict: Dict[str, str] = dict()
         self.associate_blocks = []
 
-    def set_permission(self, value):
-        self._permission = value
+        return attribstr
+
+    def _parse_bind_C(self, bind_C_text: Optional[str]):
+        """Parses a `bind(...)` attribute"""
 
-    def get_permission(self):
-        if type(self.parent) == FortranInterface and not self.parent.generic:
+        if bind_C_text is None:
+            self.bindC = None
+            return
+
+        # Shouldn't have parentheses in, but just to be safe, let's
+        # remove any
+        if "(" in bind_C_text or ")" in bind_C_text:
+            bind_C_text = ford.utils.get_parens(bind_C_text, -1)
+
+        self.bindC = bind_C_text
+
+        # Now we have to replace any quoted text that has previously
+        # been removed
+        search_from = 0
+        while quote := QUOTES_RE.search(self.bindC[search_from:]):
+            num = int(quote.group()[1:-1])
+            self.bindC = self.bindC[0:search_from] + QUOTES_RE.sub(
+                self.parent.strings[num], self.bindC[search_from:], count=1
+            )
+            if not (next_match := QUOTES_RE.search(self.bindC[search_from:])):
+                raise ValueError(
+                    f"Unexpected missing quotes in '{self.bindC[search_from:]}'"
+                )
+            search_from += next_match.end(0)
+
+    @property
+    def is_interface_procedure(self) -> bool:
+        """Is this procedure just an interface?"""
+        return isinstance(self.parent, FortranInterface) and not self.parent.generic
+
+    @property
+    def permission(self):
+        """Permission (public/private) of this procedure"""
+        if self.is_interface_procedure:
             return self.parent.permission
-        else:
-            return self._permission
 
-    permission = property(get_permission, set_permission)
+        return self._permission
+
+    @permission.setter
+    def permission(self, value):
+        self._permission = value
+
+    @property
+    def ident(self) -> str:
+        """Return a unique identifier for this object"""
+        if self.is_interface_procedure:
+            return namelist.get_name(self.parent)
+        return super().ident
+
+    def get_dir(self) -> Optional[str]:
+        if self.is_interface_procedure:
+            return "interface"
+
+        return super().get_dir()
 
     def _cleanup(self):
-        self.all_procs = {}
-        for p in self.routines:
-            self.all_procs[p.name.lower()] = p
+        """Convert all child entities to object instances"""
+
+        self.all_procs = {p.name.lower(): p for p in self.routines}
         for interface in self.interfaces:
             if not interface.abstract:
                 self.all_procs[interface.name.lower()] = interface
             if interface.generic:
-                for proc in interface.iterator("subroutines", "functions"):
+                for proc in interface.routines:
                     self.all_procs[proc.name.lower()] = proc
-        for i in range(len(self.args)):
+
+        for i, arg in enumerate(self.args):
+            # Is there a variable declaration for this argument?
             for var in self.variables:
-                if self.args[i].lower() == var.name.lower():
-                    self.args[i] = var
+                if arg.lower() == var.name.lower():
+                    arg = var
                     self.variables.remove(var)
                     break
-            if type(self.args[i]) == str:
+
+            # Otherwise, is it a procedure with an interface?
+            if isinstance(arg, str):
                 for intr in self.interfaces:
-                    if not (intr.abstract or intr.generic):
-                        proc = intr.procedure
-                        if proc.name.lower() == self.args[i].lower():
-                            self.args[i] = proc
-                            self.interfaces.remove(intr)
-                            self.args[i].parent = self
-                            break
-            if type(self.args[i]) == str:
-                if self.args[i][0].lower() in "ijklmn":
-                    vartype = "integer"
-                else:
-                    vartype = "real"
-                self.args[i] = FortranVariable(self.args[i], vartype, self)
-                self.args[i].doc = ""
+                    if intr.abstract or intr.generic:
+                        continue
+                    proc = intr.procedure
+                    if proc.name.lower() == arg.lower():
+                        arg = proc
+                        arg.parent = self
+                        self.interfaces.remove(intr)
+                        break
+
+            # If we've still not found it, it's an implicitly-type variable.
+            # FIXME: we pay no attention to `implicit none` or other
+            # `implicit` statements
+            if isinstance(arg, str):
+                arg = FortranVariable(arg, implicit_type(arg), self, doc="")
+
+            self.args[i] = arg
+
         self.process_attribs()
         self.variables = [v for v in self.variables if "external" not in v.attribs]
 
 
-class FortranFunction(FortranCodeUnit):
+class FortranSubroutine(FortranProcedure):
+    """
+    An object representing a Fortran subroutine and holding all of said
+    subroutine's contents.
+    """
+
+    def _initialize(self, line: re.Match):
+        self._procedure_initialize(**line.groupdict())
+        self.proctype = "Subroutine"
+
+
+class FortranFunction(FortranProcedure):
     """
     An object representing a Fortran function and holding all of said function's
     contents.
     """
 
-    def _initialize(self, line):
+    def _initialize(self, line: re.Match):
+        attribstr = self._procedure_initialize(**line.groupdict())
         self.proctype = "Function"
-        self.name = line.group(2)
-        attribstr = line.group(1)
-        self.module = False
-        self.mp = False
-
-        self.attribs, attribstr = _list_of_procedure_attributes(attribstr)
-        self.module = "module" in self.attribs
-
-        if line.group(4):
-            self.retvar = line.group(4)
-        else:
-            self.retvar = self.name
+        self.retvar = line["result"] or self.name
 
-        typestr = ""
-        for vtype in self.settings["extra_vartypes"]:
-            typestr = typestr + "|" + vtype
-        var_type_re = re.compile(VAR_TYPE_STRING + typestr, re.IGNORECASE)
-        if var_type_re.search(attribstr):
-            parsed_type = parse_type(attribstr, self.strings, self.settings)
+        try:
+            parsed_type = parse_type(
+                attribstr, self.strings, self.settings["extra_vartypes"]
+            )
             self.retvar = FortranVariable(
-                self.retvar,
-                parsed_type.vartype,
-                self,
+                name=self.retvar,
+                vartype=parsed_type.vartype,
+                parent=self,
                 kind=parsed_type.kind,
                 strlen=parsed_type.strlen,
                 proto=parsed_type.proto,
             )
-
-        arguments = self.SPLIT_RE.split(line.group(3)[1:-1].strip())
-        # Empty argument lists will contain the empty string, so we need to remove it
-        self.args = [arg for arg in arguments if arg]
-
-        try:
-            self.bindC = ford.utils.get_parens(line.group(5), -1)[0:-1]
-        except (RuntimeError, TypeError):
-            self.bindC = line.group(5)
-        if self.bindC:
-            search_from = 0
-            while quote := QUOTES_RE.search(self.bindC[search_from:]):
-                num = int(quote.group()[1:-1])
-                self.bindC = self.bindC[0:search_from] + QUOTES_RE.sub(
-                    self.parent.strings[num], self.bindC[search_from:], count=1
-                )
-                search_from += QUOTES_RE.search(self.bindC[search_from:]).end(0)
-        self.variables = []
-        self.enums = []
-        self.uses = []
-        self.calls = []
-        self.optional_list = []
-        self.subroutines = []
-        self.functions = []
-        self.interfaces = []
-        self.absinterfaces = []
-        self.types = []
-        self.common = []
-        self.attr_dict = defaultdict(list)
-        self.param_dict = dict()
-        self.associate_blocks = []
-
-    def set_permission(self, value):
-        self._permission = value
-
-    def get_permission(self):
-        if type(self.parent) == FortranInterface and not self.parent.generic:
-            return self.parent.permission
-        else:
-            return self._permission
-
-    permission = property(get_permission, set_permission)
+        except ValueError:
+            pass
 
     def _cleanup(self):
-        self.all_procs = {}
-        for p in self.routines:
-            self.all_procs[p.name.lower()] = p
-        for interface in self.interfaces:
-            if not interface.abstract:
-                self.all_procs[interface.name.lower()] = interface
-            if interface.generic:
-                for proc in interface.iterator("subroutines", "functions"):
-                    self.all_procs[proc.name.lower()] = proc
-        for i in range(len(self.args)):
-            for var in self.variables:
-                if self.args[i].lower() == var.name.lower():
-                    self.args[i] = var
-                    self.variables.remove(var)
-                    break
-            if type(self.args[i]) == str:
-                for intr in self.interfaces:
-                    if not (intr.abstract or intr.generic):
-                        proc = intr.procedure
-                        if proc.name.lower() == self.args[i].lower():
-                            self.args[i] = proc
-                            self.interfaces.remove(intr)
-                            self.args[i].parent = self
-                            break
-            if type(self.args[i]) == str:
-                if self.args[i][0].lower() in "ijklmn":
-                    vartype = "integer"
-                else:
-                    vartype = "real"
-                self.args[i] = FortranVariable(self.args[i], vartype, self)
-                self.args[i].doc = ""
-        if type(self.retvar) != FortranVariable:
+        if not isinstance(self.retvar, FortranVariable):
             for var in self.variables:
                 if var.name.lower() == self.retvar.lower():
                     self.retvar = var
                     self.variables.remove(var)
                     break
             else:
-                if self.retvar[0].lower() in "ijklmn":
-                    vartype = "integer"
-                else:
-                    vartype = "real"
-                self.retvar = FortranVariable(self.retvar, vartype, self)
-        self.process_attribs()
-        self.variables = [v for v in self.variables if "external" not in v.attribs]
+                self.retvar = FortranVariable(
+                    self.retvar, implicit_type(self.retvar), self
+                )
+
+        super()._cleanup()
 
 
 class FortranSubmoduleProcedure(FortranCodeUnit):
     """
     An object representing a the implementation of a Module Function or
     Module Subroutine in a submodule.
     """
@@ -1860,31 +1834,27 @@
         self.sort_components()
 
         # Get total num_lines, including implementations
         for proc in self.finalprocs:
             self.num_lines_all += proc.procedure.num_lines
         for proc in self.boundprocs:
             for bind in proc.bindings:
-                if isinstance(bind, (FortranFunction, FortranSubroutine)):
+                if isinstance(bind, FortranProcedure):
                     self.num_lines_all += bind.num_lines
                 elif isinstance(bind, FortranBoundProcedure):
                     for b in bind.bindings:
-                        if isinstance(b, (FortranFunction, FortranSubroutine)):
+                        if isinstance(b, FortranProcedure):
                             self.num_lines_all += b.num_lines
 
     def prune(self):
         """
         Remove anything which shouldn't be displayed.
         """
-        self.boundprocs = [
-            obj for obj in self.boundprocs if obj.permission in self.display
-        ]
-        self.variables = [
-            obj for obj in self.variables if obj.permission in self.display
-        ]
+        self.boundprocs = self.filter_display(self.boundprocs)
+        self.variables = self.filter_display(self.variables)
         for obj in self.boundprocs + self.variables:
             obj.visible = True
 
     def __repr__(self):
         return f"FortranType('{self.name}', variables={self.variables}, boundprocs={self.boundprocs})"
 
 
@@ -1943,17 +1913,15 @@
         self.subroutines = []
         self.functions = []
         self.modprocs = []
         self.variables = []
         self.generic = bool(self.name)
         self.abstract = bool(line.group(1))
         if self.generic and self.abstract:
-            raise Exception(
-                "Generic interface {} can not be abstract".format(self.name)
-            )
+            raise Exception(f"Generic interface '{self.name}' can not be abstract")
 
     def correlate(self, project):
         self.all_absinterfaces = self.parent.all_absinterfaces
         self.all_types = self.parent.all_types
         self.all_procs = self.parent.all_procs
         self.num_lines_all = self.num_lines
         if self.generic:
@@ -1984,42 +1952,30 @@
                 proc.correlate(project)
         else:
             self.procedure.correlate(project)
 
         self.sort_components()
 
     def _cleanup(self):
-        if self.abstract:
-            contents = []
-            for proc in self.routines:
-                proc.visible = False
-                item = copy.copy(self)
-                item.procedure = proc
-                item.procedure.parent = item
-                del item.functions
-                del item.modprocs
-                del item.subroutines
-                item.name = proc.name
-                item.permission = proc.permission
-                contents.append(item)
-            self.contents = contents
-        elif not self.generic:
-            contents = []
-            for proc in self.routines:
-                proc.visible = False
-                item = copy.copy(self)
-                item.procedure = proc
-                item.procedure.parent = item
-                del item.functions
-                del item.modprocs
-                del item.subroutines
-                item.name = proc.name
-                item.permission = proc.permission
-                contents.append(item)
-            self.contents = contents
+        if not self.abstract and self.generic:
+            return
+
+        contents = []
+        for proc in self.routines:
+            proc.visible = False
+            item = copy.copy(self)
+            item.procedure = proc
+            item.procedure.parent = item
+            del item.functions
+            del item.modprocs
+            del item.subroutines
+            item.name = proc.name
+            item.permission = proc.permission
+            contents.append(item)
+        self.contents = contents
 
 
 class FortranFinalProc(FortranBase):
     """
     An object representing a finalization procedure for a derived type
     within Fortran.
     """
@@ -2086,15 +2042,15 @@
         self.obj = type(self).__name__[7:].lower()
         self.attribs = copy.copy(attribs)
         self.intent = intent
         self.optional = optional
         self.kind = kind
         self.strlen = strlen
         self.proto = copy.copy(proto)
-        self.doc = copy.copy(doc) or []
+        self.doc = copy.copy(doc) if doc is not None else []
         self.permission = permission
         self.points = points
         self.parameter = parameter
         self.initial = initial
         self.dimension = ""
         self.meta = {}
         self.visible = False
@@ -2181,85 +2137,75 @@
 
 
 class FortranBoundProcedure(FortranBase):
     """
     An object representing a type-bound procedure, possibly overloaded.
     """
 
-    def _initialize(self, line):
-        attribstr = line.group(3)
+    def _initialize(self, line: re.Match):
         self.attribs = []
         self.deferred = False
-        if attribstr:
-            tmp_attribs = ford.utils.paren_split(",", attribstr[1:])
-            for i in range(len(tmp_attribs)):
-                tmp_attribs[i] = tmp_attribs[i].strip()
-                if tmp_attribs[i].lower() == "public":
-                    self.permission = "public"
-                elif tmp_attribs[i].lower() == "private":
-                    self.permission = "private"
-                elif tmp_attribs[i].lower() == "deferred":
-                    self.deferred = True
-                else:
-                    self.attribs.append(tmp_attribs[i])
-        rest = line.group(4)
-        split = self.POINTS_TO_RE.split(rest)
+
+        for attribute in ford.utils.paren_split(",", line["attributes"] or ""):
+            attribute = attribute.strip()
+            # Preserve original capitalisation -- TODO: needed?
+            attribute_lower = attribute.lower()
+            if attribute_lower in ["public", "private"]:
+                self.permission = attribute_lower
+            elif attribute_lower == "deferred":
+                self.deferred = True
+            else:
+                self.attribs.append(attribute)
+
+        split = self.POINTS_TO_RE.split(line["names"])
         self.name = split[0].strip()
-        self.generic = line.group(1).lower() == "generic"
-        self.proto = line.group(2)
+        self.generic = line["generic"].lower() == "generic"
+        self.proto = line["prototype"]
         if self.proto:
             self.proto = self.proto[1:-1].strip()
         self.bindings = []
         if len(split) > 1:
             binds = self.SPLIT_RE.split(split[1])
             for bind in binds:
                 self.bindings.append(bind.strip())
         else:
             self.bindings.append(self.name)
-        if line.group(2):
-            self.prototype = line.group(2)[1:-1]
-        else:
-            self.prototype = None
 
     def correlate(self, project):
         self.all_procs = self.parent.all_procs
         self.protomatch = False
         if self.proto:
-            if self.proto.lower() in self.all_procs:
-                self.proto = self.all_procs[self.proto.lower()]
+            proto_lower = self.proto.lower()
+            if proto_lower in self.all_procs:
+                self.proto = self.all_procs[proto_lower]
                 self.protomatch = True
-            elif self.proto.lower() in self.parent.all_absinterfaces:
-                self.proto = self.parent.all_absinterfaces[self.proto.lower()]
+            elif proto_lower in self.parent.all_absinterfaces:
+                self.proto = self.parent.all_absinterfaces[proto_lower]
                 self.protomatch = True
-            # else:
-            #    self.proto = FortranSpoof(self.proto, self, 'INTERFACE')
-            #    self.protomatch = True
+
         if self.generic:
-            for i in range(len(self.bindings)):
-                for proc in self.parent.boundprocs:
-                    if type(self.bindings[i]) is str:
-                        if proc.name and proc.name.lower() == self.bindings[i].lower():
-                            self.bindings[i] = proc
-                            break
-                    else:
-                        if (
-                            proc.name
-                            and proc.name.lower() == self.bindings[i].name.lower()
-                        ):
-                            self.bindings[i] = proc
-                            break
-                # else:
-                #    self.bindings[i] = FortranSpoof(self.bindings[i], self.parent, 'BOUNDPROC')
+            parent_boundprocs = {
+                proc.name.lower(): proc for proc in self.parent.boundprocs if proc
+            }
+
+            for i, binding in enumerate(self.bindings):
+                binding_name = getattr(binding, "name", binding).lower()
+
+                try:
+                    self.bindings[i] = parent_boundprocs[binding_name]
+                except KeyError:
+                    pass
+
         elif not self.deferred:
             for i in range(len(self.bindings)):
-                if self.bindings[i].lower() in self.all_procs:
+                try:
                     self.bindings[i] = self.all_procs[self.bindings[i].lower()]
+                    self.bindings[i].binding = self
+                except KeyError:
                     break
-            # else:
-            #    self.bindings[i] = FortranSpoof(self.bindings[i], self.parent, 'BOUNDPROC')
 
         self.sort_components()
 
     def __repr__(self):
         return f"FortranBoundProcedure('{self.name}', permission='{self.permission}')"
 
 
@@ -2352,21 +2298,18 @@
             var.correlate(project)
         for com in self.common:
             com.correlate(project)
 
         self.sort_components()
 
     def prune(self):
-        self.types = [obj for obj in self.types if obj.permission in self.display]
-        self.variables = [
-            obj for obj in self.variables if obj.permission in self.display
-        ]
+        self.types = self.filter_display(self.types)
+        self.variables = self.filter_display(self.variables)
         for dtype in self.types:
             dtype.visible = True
-        for dtype in self.types:
             dtype.prune()
 
     def _cleanup(self):
         self.process_attribs()
 
     def process_attribs(self):
         for item in self.types:
@@ -2418,20 +2361,17 @@
             if self.variables[i] in self.parent.all_vars:
                 self.variables[i] = self.parent.all_vars[self.variables[i]]
                 try:
                     self.parent.variables.remove(self.variables[i])
                 except ValueError:
                     pass
             else:
-                if self.variables[i][0].lower() in "ijklmn":
-                    vartype = "integer"
-                else:
-                    vartype = "real"
-                self.variables[i] = FortranVariable(self.variables[i], vartype, self)
-                self.variables[i].doc = ""
+                self.variables[i] = FortranVariable(
+                    self.variables[i], implicit_type(self.variables[i]), self, doc=""
+                )
 
         if self.name in project.common:
             self.other_uses = project.common[self.name]
             self.other_uses.append(self)
         else:
             lst = [self]
             project.common[self.name] = lst
@@ -2614,23 +2554,22 @@
                 prevdoc = False
             docalt = False
 
     def lines_description(self, total, total_all=0):
         return ""
 
 
-_can_have_contains = [
+_can_have_contains = (
     FortranModule,
     FortranProgram,
-    FortranFunction,
-    FortranSubroutine,
+    FortranProcedure,
     FortranType,
     FortranSubmodule,
     FortranSubmoduleProcedure,
-]
+)
 
 
 def remove_kind_suffix(literal, is_character: bool = False):
     """Return the literal without the kind suffix of a numerical literal,
     or the kind prefix of a character literal"""
 
     kind_re = CHAR_KIND_SUFFIX_RE if is_character else KIND_SUFFIX_RE
@@ -2641,15 +2580,15 @@
 
 
 def line_to_variables(source, line, inherit_permission, parent):
     """
     Returns a list of variables declared in the provided line of code. The
     line of code should be provided as a string.
     """
-    parsed_type = parse_type(line, parent.strings, parent.settings)
+    parsed_type = parse_type(line, parent.strings, parent.settings["extra_vartypes"])
     attribs = []
     intent = ""
     optional = False
     permission = inherit_permission
     parameter = False
 
     if attribmatch := ATTRIBSPLIT_RE.match(parsed_type.rest):
@@ -2731,35 +2670,44 @@
                 initial,
             )
         )
 
     return varlist
 
 
+_EXTRA_TYPES_RE_CACHE: Dict[Tuple[str, ...], re.Pattern] = {}
+
+
 @dataclass
 class ParsedType:
     vartype: str
     rest: str
     kind: Optional[str] = None
     strlen: Optional[str] = None
     proto: Union[None, str, List[str]] = None
 
 
-def parse_type(string: str, capture_strings: List[str], settings: dict) -> ParsedType:
+def parse_type(
+    string: str, capture_strings: List[str], extra_vartypes: Sequence[str]
+) -> ParsedType:
     """
     Gets variable type, kind, length, and/or derived-type attributes from a
     variable declaration.
     """
-    typestr = ""
-    for vtype in settings["extra_vartypes"]:
-        typestr = typestr + "|" + vtype
-    var_type_re = re.compile(VAR_TYPE_STRING + typestr, re.IGNORECASE)
-    match = var_type_re.match(string)
-    if not match:
-        raise Exception("Invalid variable declaration: {}".format(string))
+    extra_vartypes = tuple(extra_vartypes)
+    try:
+        var_type_re = _EXTRA_TYPES_RE_CACHE[extra_vartypes]
+    except KeyError:
+        var_type_re = re.compile(
+            "|".join((VAR_TYPE_STRING, *extra_vartypes)), re.IGNORECASE
+        )
+        _EXTRA_TYPES_RE_CACHE[extra_vartypes] = var_type_re
+
+    if not (match := var_type_re.match(string)):
+        raise ValueError("Invalid variable declaration: {}".format(string))
 
     vartype = match.group().lower()
     if DOUBLE_PREC_RE.match(vartype):
         vartype = "double precision"
     if DOUBLE_CMPLX_RE.match(vartype):
         vartype = "double complex"
     rest = string[match.end() :].strip()
```

### Comparing `FORD-6.2.4/ford/templates/absint_list.html` & `FORD-6.2.5/ford/templates/absint_list.html`

 * *Files identical despite different names*

### Comparing `FORD-6.2.4/ford/templates/base.html` & `FORD-6.2.5/ford/templates/base.html`

 * *Files identical despite different names*

### Comparing `FORD-6.2.4/ford/templates/block_list.html` & `FORD-6.2.5/ford/templates/block_list.html`

 * *Files identical despite different names*

### Comparing `FORD-6.2.4/ford/templates/block_page.html` & `FORD-6.2.5/ford/templates/block_page.html`

 * *Files identical despite different names*

### Comparing `FORD-6.2.4/ford/templates/file_list.html` & `FORD-6.2.5/ford/templates/file_list.html`

 * *Files identical despite different names*

### Comparing `FORD-6.2.4/ford/templates/file_page.html` & `FORD-6.2.5/ford/templates/file_page.html`

 * *Files identical despite different names*

### Comparing `FORD-6.2.4/ford/templates/genint_page.html` & `FORD-6.2.5/ford/templates/genint_page.html`

 * *Files identical despite different names*

### Comparing `FORD-6.2.4/ford/templates/index.html` & `FORD-6.2.5/ford/templates/index.html`

 * *Files identical despite different names*

### Comparing `FORD-6.2.4/ford/templates/info_page.html` & `FORD-6.2.5/ford/templates/info_page.html`

 * *Files identical despite different names*

### Comparing `FORD-6.2.4/ford/templates/macros.html` & `FORD-6.2.5/ford/templates/macros.html`

 * *Files identical despite different names*

### Comparing `FORD-6.2.4/ford/templates/mod_list.html` & `FORD-6.2.5/ford/templates/mod_list.html`

 * *Files identical despite different names*

### Comparing `FORD-6.2.4/ford/templates/mod_page.html` & `FORD-6.2.5/ford/templates/mod_page.html`

 * *Files identical despite different names*

### Comparing `FORD-6.2.4/ford/templates/nongenint_page.html` & `FORD-6.2.5/ford/templates/nongenint_page.html`

 * *Files identical despite different names*

### Comparing `FORD-6.2.4/ford/templates/proc_list.html` & `FORD-6.2.5/ford/templates/proc_list.html`

 * *Files identical despite different names*

### Comparing `FORD-6.2.4/ford/templates/proc_page.html` & `FORD-6.2.5/ford/templates/proc_page.html`

 * *Files 5% similar despite different names*

```diff
@@ -20,14 +20,19 @@
     <h2>{{ macros.proc_line(procedure,False) }}</h2>
     {{ macros.use_list(procedure) }}
 
     {% if procedure.doc %}
     {{ procedure.doc }}
     {% endif %}
 
+    {% if procedure.binding %}
+    <h3>Type Bound</h3>
+    <p>{{ procedure.binding.parent }}</p>
+    {% endif %}
+
     <h3>Arguments</h3>
     {% if procedure.args|length > 0 %}
       {{ macros.variable_list(procedure.args, intent=True) }}
     {% else %}
     <em>None</em>
     <br>
     {% endif %}
```

### Comparing `FORD-6.2.4/ford/templates/prog_list.html` & `FORD-6.2.5/ford/templates/prog_list.html`

 * *Files identical despite different names*

### Comparing `FORD-6.2.4/ford/templates/prog_page.html` & `FORD-6.2.5/ford/templates/prog_page.html`

 * *Files identical despite different names*

### Comparing `FORD-6.2.4/ford/templates/search.html` & `FORD-6.2.5/ford/templates/search.html`

 * *Files identical despite different names*

### Comparing `FORD-6.2.4/ford/templates/type_page.html` & `FORD-6.2.5/ford/templates/type_page.html`

 * *Files identical despite different names*

### Comparing `FORD-6.2.4/ford/templates/types_list.html` & `FORD-6.2.5/ford/templates/types_list.html`

 * *Files identical despite different names*

### Comparing `FORD-6.2.4/ford/tipue_search.py` & `FORD-6.2.5/ford/tipue_search.py`

 * *Files identical despite different names*

### Comparing `FORD-6.2.4/ford/tipuesearch/.DS_Store` & `FORD-6.2.5/ford/tipuesearch/.DS_Store`

 * *Files identical despite different names*

### Comparing `FORD-6.2.4/ford/tipuesearch/img/.DS_Store` & `FORD-6.2.5/ford/tipuesearch/img/.DS_Store`

 * *Files identical despite different names*

### Comparing `FORD-6.2.4/ford/tipuesearch/img/loader.gif` & `FORD-6.2.5/ford/tipuesearch/img/loader.gif`

 * *Files identical despite different names*

### Comparing `FORD-6.2.4/ford/tipuesearch/tipuesearch.css` & `FORD-6.2.5/ford/tipuesearch/tipuesearch.css`

 * *Files identical despite different names*

### Comparing `FORD-6.2.4/ford/tipuesearch/tipuesearch.js` & `FORD-6.2.5/ford/tipuesearch/tipuesearch.js`

 * *Files identical despite different names*

### Comparing `FORD-6.2.4/ford/tipuesearch/tipuesearch.min.js` & `FORD-6.2.5/ford/tipuesearch/tipuesearch.min.js`

 * *Files identical despite different names*

### Comparing `FORD-6.2.4/ford/tipuesearch/tipuesearch_set.js` & `FORD-6.2.5/ford/tipuesearch/tipuesearch_set.js`

 * *Files identical despite different names*

### Comparing `FORD-6.2.4/ford/utils.py` & `FORD-6.2.5/ford/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,15 +81,15 @@
         return ret
 
     for regex in NOTE_RE:
         docs = regex.sub(substitute, docs)
     return docs
 
 
-def get_parens(line, retlevel=0, retblevel=0):
+def get_parens(line: str, retlevel: int = 0, retblevel: int = 0) -> str:
     """
     By default akes a string starting with an open parenthesis and returns the portion
     of the string going to the corresponding close parenthesis. If retlevel != 0 then
     will return when that level (for parentheses) is reached. Same for retblevel.
     """
     if len(line) == 0:
         return line
```

### Comparing `FORD-6.2.4/output-example.png` & `FORD-6.2.5/output-example.png`

 * *Files identical despite different names*

### Comparing `FORD-6.2.4/pyproject.toml` & `FORD-6.2.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `FORD-6.2.4/test/conftest.py` & `FORD-6.2.5/test/conftest.py`

 * *Files identical despite different names*

### Comparing `FORD-6.2.4/test/test_corpus.py` & `FORD-6.2.5/test/test_corpus.py`

 * *Files identical despite different names*

### Comparing `FORD-6.2.4/test/test_example.py` & `FORD-6.2.5/test/test_example.py`

 * *Files identical despite different names*

### Comparing `FORD-6.2.4/test/test_graphs.py` & `FORD-6.2.5/test/test_graphs.py`

 * *Files 6% similar despite different names*

```diff
@@ -51,31 +51,47 @@
         type(external_type) :: component
       end type leaf
 
       type thing
         type(derived) :: part
       end type thing
 
+      type alpha
+      contains
+        procedure :: five
+        procedure :: six
+      end type alpha
+
     contains
       subroutine one
       end subroutine one
       subroutine two
         call one
       end subroutine two
+      subroutine five
+      end subroutine five
+      function six(this) result(res)
+        real :: res
+        res = 1
+      end function six
     end module c
 
     submodule (c) c_submod
     end submodule c_submod
 
     submodule (c:c_submod) c_subsubmod
     end submodule c_subsubmod
 
     program foo
       use c
       call three
+      real :: x
+      type(alpha) :: y
+      call y%five()
+      x = y%six()
     contains
       subroutine three
         use external_mod
         call one
         call two
         call two
         call other_sub
@@ -157,28 +173,39 @@
                 "proc~three->external_mod",
                 "program~foo->module~c",
             ],
             MOD_GRAPH_KEY,
         ),
         (
             ["callgraph"],
-            ["c::one", "foo::three", "c::two", "foo::four", "other_sub", "foo"],
+            [
+                "c::one",
+                "foo::three",
+                "c::two",
+                "foo::four",
+                "other_sub",
+                "foo",
+                "c::alpha%five",
+                "c::alpha%six",
+            ],
             [
                 "proc~three->proc~one",
                 "proc~three->proc~two",
                 "proc~two->proc~one",
                 "proc~three->other_sub",
                 "program~foo->proc~three",
                 "proc~four->proc~four",
+                "program~foo->proc~five",
+                "program~foo->proc~six",
             ],
             PROC_GRAPH_KEY,
         ),
         (
             ["typegraph"],
-            ["base", "derived", "leaf", "external_type", "thing"],
+            ["base", "derived", "leaf", "external_type", "thing", "alpha"],
             [
                 "type~leaf->type~derived",
                 "type~derived->type~base",
                 "type~leaf->external_type",
                 "type~thing->type~derived",
             ],
             TYPE_GRAPH_KEY,
```

### Comparing `FORD-6.2.4/test/test_initialisation.py` & `FORD-6.2.5/test/test_initialisation.py`

 * *Files identical despite different names*

### Comparing `FORD-6.2.4/test/test_md_inputs.py` & `FORD-6.2.5/test/test_md_inputs.py`

 * *Files identical despite different names*

### Comparing `FORD-6.2.4/test/test_md_table.py` & `FORD-6.2.5/test/test_md_table.py`

 * *Files identical despite different names*

### Comparing `FORD-6.2.4/test/test_pagetree.py` & `FORD-6.2.5/test/test_pagetree.py`

 * *Files identical despite different names*

### Comparing `FORD-6.2.4/test/test_project.py` & `FORD-6.2.5/test/test_project.py`

 * *Files identical despite different names*

### Comparing `FORD-6.2.4/test/test_projects/test_external_project.py` & `FORD-6.2.5/test/test_projects/test_external_project.py`

 * *Files identical despite different names*

### Comparing `FORD-6.2.4/test/test_reader.py` & `FORD-6.2.5/test/test_reader.py`

 * *Files identical despite different names*

### Comparing `FORD-6.2.4/test/test_sourceform.py` & `FORD-6.2.5/test/test_sourceform.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,19 @@
 from dataclasses import dataclass, field
 from typing import Union, List, Optional
 
 import markdown
 import pytest
 
 
+class FakeProject:
+    def __init__(self, procedures=None):
+        self.procedures = procedures or []
+
+
 @pytest.fixture
 def parse_fortran_file(copy_fortran_file):
     def parse_file(data, **kwargs):
         filename = copy_fortran_file(data)
         settings = deepcopy(DEFAULT_SETTINGS)
         settings.update(kwargs)
 
@@ -419,15 +424,15 @@
 
       integer function func_private()
       end function func_private
     end module default_access
     """
 
     fortran_file = parse_fortran_file(data)
-    fortran_file.modules[0].correlate(None)
+    fortran_file.modules[0].correlate(FakeProject())
 
     assert set(fortran_file.modules[0].all_procs.keys()) == {
         "sub_public",
         "func_public",
         "sub_private",
         "func_private",
     }
@@ -487,15 +492,15 @@
 
       integer function func_private()
       end function func_private
     end module public_access
     """
 
     fortran_file = parse_fortran_file(data)
-    fortran_file.modules[0].correlate(None)
+    fortran_file.modules[0].correlate(FakeProject())
 
     assert set(fortran_file.modules[0].all_procs.keys()) == {
         "sub_public",
         "func_public",
         "sub_private",
         "func_private",
     }
@@ -555,15 +560,15 @@
 
       integer function func_private()
       end function func_private
     end module private_access
     """
 
     fortran_file = parse_fortran_file(data)
-    fortran_file.modules[0].correlate(None)
+    fortran_file.modules[0].correlate(FakeProject())
 
     assert set(fortran_file.modules[0].all_procs.keys()) == {
         "sub_public",
         "func_public",
         "sub_private",
         "func_private",
     }
@@ -734,21 +739,23 @@
             "class(foo) :: thing",
             ParsedType("class", ":: thing", proto=["foo", ""]),
         ),
         (
             "procedure(bar) :: thing",
             ParsedType("procedure", ":: thing", proto=["bar", ""]),
         ),
+        ("Vec :: vector", ParsedType("vec", ":: vector")),
+        ("Mat :: matrix", ParsedType("mat", ":: matrix")),
     ],
 )
 def test_parse_type(variable_decl, expected):
     # Tokeniser will have previously replaced strings with index into
     # this list
     capture_strings = ['"a"']
-    result = parse_type(variable_decl, capture_strings, {"extra_vartypes": []})
+    result = parse_type(variable_decl, capture_strings, ["Vec", "Mat"])
     assert result.vartype == expected.vartype
     assert result.kind == expected.kind
     assert result.strlen == expected.strlen
     assert result.proto == expected.proto
     assert result.rest == expected.rest
 
 
@@ -1235,15 +1242,15 @@
 
       subroutine sub_private
       end subroutine sub_private
     end module default_access
     """
 
     fortran_file = parse_fortran_file(data)
-    fortran_file.modules[0].correlate(None)
+    fortran_file.modules[0].correlate(FakeProject())
 
     for ftype in fortran_file.modules[0].types:
         assert (
             ftype.variables[0].permission == "public"
         ), f"{ftype.name}::{ftype.variables[0].name}"
         assert (
             ftype.variables[1].permission == "private"
@@ -1266,15 +1273,15 @@
     contains
       type(bar) function quux()
       end function quux
     end module foo_m
     """
 
     fortran_file = parse_fortran_file(data)
-    fortran_file.modules[0].correlate(None)
+    fortran_file.modules[0].correlate(FakeProject())
     variable0 = fortran_file.modules[0].variables[0]
     variable1 = fortran_file.modules[0].variables[1]
 
     assert variable0.full_type == "character(kind=kind('a'), len=4)"
     assert (
         variable0.full_declaration
         == "character(kind=kind('a'), len=4), dimension(:, :), allocatable"
@@ -1389,15 +1396,15 @@
         print*, "implementation"
       end procedure
     end module foo_mod
     """
 
     fortran_file = parse_fortran_file(data)
     module = fortran_file.modules[0]
-    module.correlate(None)
+    module.correlate(FakeProject())
 
     interface = module.interfaces[0]
     assert interface.name == "quaxx"
     modproc = module.modprocedures[0]
 
     assert interface.procedure.module == modproc
     assert modproc.module == interface
@@ -1416,15 +1423,15 @@
         bar = .true.
       end procedure
     end module
     """
 
     fortran_file = parse_fortran_file(data)
     module = fortran_file.modules[0]
-    module.correlate(None)
+    module.correlate(FakeProject())
 
     interface = module.interfaces[0]
     assert interface.name == "foo"
 
     modproc = module.modprocedures[0]
     assert modproc.name == "foo"
 
@@ -1447,15 +1454,15 @@
         procedure unary_f
       end interface
     end module
     """
 
     fortran_file = parse_fortran_file(data)
     module = fortran_file.modules[0]
-    module.correlate(None)
+    module.correlate(FakeProject())
     assert len(module.interfaces[0].modprocs) == 0
     assert module.interfaces[0].variables[0].name == "unary_f"
 
 
 def test_block_data(parse_fortran_file):
     data = """\
     block data name
@@ -1523,7 +1530,62 @@
     end function foo
     """
 
     fortran_file = parse_fortran_file(data)
     function = fortran_file.functions[0]
     arg_names = [arg.name for arg in function.args]
     assert arg_names == ["a", "b", "c", "d"]
+
+
+def test_bind_name_subroutine(parse_fortran_file):
+    data = """\
+    subroutine init() bind(C, name="c_init")
+    end subroutine init
+    """
+
+    fortran_file = parse_fortran_file(data)
+    subroutine = fortran_file.subroutines[0]
+
+    assert subroutine.bindC == 'C, name="c_init"'
+
+
+def test_bind_name_function(parse_fortran_file):
+    data = """\
+    integer function foo() bind(C, name="c_foo")
+    end function foo
+    """
+
+    fortran_file = parse_fortran_file(data)
+    function = fortran_file.functions[0]
+
+    assert function.bindC == 'C, name="c_foo"'
+
+
+def test_generic_bound_procedure(parse_fortran_file):
+    data = """\
+    module subdomain_m
+      type subdomain_t
+      contains
+        procedure no_colon
+        procedure :: colon
+        generic :: operator(+) => no_colon, colon
+      end type
+      interface
+        module function no_colon(lhs, rhs)
+          class(subdomain_t), intent(in) :: lhs
+          integer, intent(in) :: rhs
+          type(subdomain_t) total
+        end function
+        module function colon(lhs, rhs)
+          class(subdomain_t), intent(in) :: lhs, rhs
+          type(subdomain_t) total
+        end function
+      end interface
+    end module
+    """
+
+    fortran_file = parse_fortran_file(data)
+    fortran_type = fortran_file.modules[0].types[0]
+
+    expected_names = sorted(["no_colon", "colon", "operator(+)"])
+    bound_proc_names = sorted([proc.name for proc in fortran_type.boundprocs])
+    assert bound_proc_names == expected_names
```

### Comparing `FORD-6.2.4/test/test_utils.py` & `FORD-6.2.5/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `FORD-6.2.4/test_data/external_project/external_project/src/external.f90` & `FORD-6.2.5/test_data/external_project/external_project/src/external.f90`

 * *Files identical despite different names*

### Comparing `FORD-6.2.4/test_data/external_project/top_level_project/src/top_level.f90` & `FORD-6.2.5/test_data/external_project/top_level_project/src/top_level.f90`

 * *Files identical despite different names*

### Comparing `FORD-6.2.4/test_data/ford_issues_bad.f90` & `FORD-6.2.5/test_data/ford_issues_bad.f90`

 * *Files identical despite different names*

### Comparing `FORD-6.2.4/test_data/ford_issues_ok.f90` & `FORD-6.2.5/test_data/ford_issues_ok.f90`

 * *Files identical despite different names*

### Comparing `FORD-6.2.4/test_data/ford_issues_ok_expected.f90` & `FORD-6.2.5/test_data/ford_issues_ok_expected.f90`

 * *Files identical despite different names*

### Comparing `FORD-6.2.4/test_data/ford_test_program.f90` & `FORD-6.2.5/test_data/ford_test_program.f90`

 * *Files identical despite different names*

### Comparing `FORD-6.2.4/test_data/ford_test_program_expected.f90` & `FORD-6.2.5/test_data/ford_test_program_expected.f90`

 * *Files identical despite different names*

