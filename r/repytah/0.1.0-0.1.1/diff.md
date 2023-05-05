# Comparing `tmp/repytah-0.1.0.tar.gz` & `tmp/repytah-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "repytah-0.1.0.tar", last modified: Thu Feb 16 14:27:03 2023, max compression
+gzip compressed data, was "repytah-0.1.1.tar", last modified: Fri May  5 09:26:54 2023, max compression
```

## Comparing `repytah-0.1.0.tar` & `repytah-0.1.1.tar`

### file list

```diff
@@ -1,136 +1,137 @@
-drwxr-xr-x   0 katiek     (501) staff       (20)        0 2023-02-16 14:27:03.829963 repytah-0.1.0/
--rw-r--r--   0 katiek     (501) staff       (20)      669 2023-02-16 14:19:23.000000 repytah-0.1.0/AUTHORS.md
--rw-r--r--   0 katiek     (501) staff       (20)     3430 2021-07-29 17:37:15.000000 repytah-0.1.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 katiek     (501) staff       (20)      792 2023-02-16 14:19:23.000000 repytah-0.1.0/LICENSE.md
--rw-r--r--   0 katiek     (501) staff       (20)      156 2021-07-29 17:37:15.000000 repytah-0.1.0/MANIFEST.in
--rw-r--r--   0 katiek     (501) staff       (20)     5734 2023-02-16 14:27:03.829781 repytah-0.1.0/PKG-INFO
--rw-r--r--   0 katiek     (501) staff       (20)     4737 2023-02-16 14:19:23.000000 repytah-0.1.0/README.md
-drwxr-xr-x   0 katiek     (501) staff       (20)        0 2023-02-16 14:27:03.813001 repytah-0.1.0/docs/
-drwxr-xr-x   0 katiek     (501) staff       (20)        0 2023-02-16 14:27:03.813187 repytah-0.1.0/docs/.ipynb_checkpoints/
--rw-r--r--   0 katiek     (501) staff       (20)   316363 2021-07-30 02:08:42.000000 repytah-0.1.0/docs/.ipynb_checkpoints/example_vignette-checkpoint.ipynb
--rw-r--r--   0 katiek     (501) staff       (20)      634 2021-07-06 19:40:28.000000 repytah-0.1.0/docs/Makefile
-drwxr-xr-x   0 katiek     (501) staff       (20)        0 2023-02-16 14:27:03.804649 repytah-0.1.0/docs/_build/
-drwxr-xr-x   0 katiek     (501) staff       (20)        0 2023-02-16 14:27:03.814353 repytah-0.1.0/docs/_build/doctrees/
--rw-r--r--   0 katiek     (501) staff       (20)    25279 2021-07-29 17:37:15.000000 repytah-0.1.0/docs/_build/doctrees/assemble.doctree
--rw-r--r--   0 katiek     (501) staff       (20)    67237 2021-07-29 17:37:15.000000 repytah-0.1.0/docs/_build/doctrees/environment.pickle
--rw-r--r--   0 katiek     (501) staff       (20)     5445 2021-07-29 17:37:15.000000 repytah-0.1.0/docs/_build/doctrees/index.doctree
--rw-r--r--   0 katiek     (501) staff       (20)    18207 2021-07-29 17:37:15.000000 repytah-0.1.0/docs/_build/doctrees/search_doc.doctree
--rw-r--r--   0 katiek     (501) staff       (20)    13646 2021-07-29 17:37:15.000000 repytah-0.1.0/docs/_build/doctrees/transform.doctree
--rw-r--r--   0 katiek     (501) staff       (20)    43724 2021-07-29 17:37:15.000000 repytah-0.1.0/docs/_build/doctrees/utilities.doctree
-drwxr-xr-x   0 katiek     (501) staff       (20)        0 2023-02-16 14:27:03.816029 repytah-0.1.0/docs/_build/html/
--rw-r--r--   0 katiek     (501) staff       (20)      230 2021-07-29 17:37:15.000000 repytah-0.1.0/docs/_build/html/.buildinfo
-drwxr-xr-x   0 katiek     (501) staff       (20)        0 2023-02-16 14:27:03.816179 repytah-0.1.0/docs/_build/html/_sources/
--rw-r--r--   0 katiek     (501) staff       (20)      811 2021-07-29 17:37:15.000000 repytah-0.1.0/docs/_build/html/_sources/index.rst.txt
-drwxr-xr-x   0 katiek     (501) staff       (20)        0 2023-02-16 14:27:03.819880 repytah-0.1.0/docs/_build/html/_static/
--rw-r--r--   0 katiek     (501) staff       (20)    14652 2021-07-06 19:40:28.000000 repytah-0.1.0/docs/_build/html/_static/basic.css
--rw-r--r--   0 katiek     (501) staff       (20)      224 2021-07-29 17:37:15.000000 repytah-0.1.0/docs/_build/html/_static/custom.css
--rw-r--r--   0 katiek     (501) staff       (20)     9592 2021-07-06 19:40:28.000000 repytah-0.1.0/docs/_build/html/_static/doctools.js
--rw-r--r--   0 katiek     (501) staff       (20)      350 2021-07-06 19:40:28.000000 repytah-0.1.0/docs/_build/html/_static/documentation_options.js
--rw-r--r--   0 katiek     (501) staff       (20)      286 2021-07-06 19:40:28.000000 repytah-0.1.0/docs/_build/html/_static/file.png
--rw-r--r--   0 katiek     (501) staff       (20)   268039 2021-07-06 19:40:28.000000 repytah-0.1.0/docs/_build/html/_static/jquery-3.2.1.js
--rw-r--r--   0 katiek     (501) staff       (20)   287630 2021-07-06 19:40:28.000000 repytah-0.1.0/docs/_build/html/_static/jquery-3.5.1.js
--rw-r--r--   0 katiek     (501) staff       (20)    89476 2021-07-06 19:40:28.000000 repytah-0.1.0/docs/_build/html/_static/jquery.js
--rw-r--r--   0 katiek     (501) staff       (20)    10854 2021-07-06 19:40:28.000000 repytah-0.1.0/docs/_build/html/_static/language_data.js
--rw-r--r--   0 katiek     (501) staff       (20)       90 2021-07-06 19:40:28.000000 repytah-0.1.0/docs/_build/html/_static/minus.png
--rw-r--r--   0 katiek     (501) staff       (20)       90 2021-07-06 19:40:28.000000 repytah-0.1.0/docs/_build/html/_static/plus.png
--rw-r--r--   0 katiek     (501) staff       (20)     5249 2021-07-06 19:40:28.000000 repytah-0.1.0/docs/_build/html/_static/pygments.css
--rw-r--r--   0 katiek     (501) staff       (20)    16578 2021-07-06 19:40:28.000000 repytah-0.1.0/docs/_build/html/_static/searchtools.js
--rw-r--r--   0 katiek     (501) staff       (20)    67692 2021-07-06 19:40:28.000000 repytah-0.1.0/docs/_build/html/_static/underscore-1.12.0.js
--rw-r--r--   0 katiek     (501) staff       (20)    35168 2021-07-06 19:40:28.000000 repytah-0.1.0/docs/_build/html/_static/underscore-1.3.1.js
--rw-r--r--   0 katiek     (501) staff       (20)    19358 2021-07-06 19:40:28.000000 repytah-0.1.0/docs/_build/html/_static/underscore.js
--rw-r--r--   0 katiek     (501) staff       (20)    13249 2021-07-29 17:37:15.000000 repytah-0.1.0/docs/_build/html/assemble.html
--rw-r--r--   0 katiek     (501) staff       (20)    16094 2021-07-29 17:37:15.000000 repytah-0.1.0/docs/_build/html/genindex.html
--rw-r--r--   0 katiek     (501) staff       (20)     9037 2021-07-29 17:37:15.000000 repytah-0.1.0/docs/_build/html/index.html
--rw-r--r--   0 katiek     (501) staff       (20)     2535 2021-07-29 17:37:15.000000 repytah-0.1.0/docs/_build/html/objects.inv
--rw-r--r--   0 katiek     (501) staff       (20)     7045 2021-07-29 17:37:15.000000 repytah-0.1.0/docs/_build/html/py-modindex.html
--rw-r--r--   0 katiek     (501) staff       (20)     6150 2021-07-29 17:37:15.000000 repytah-0.1.0/docs/_build/html/search.html
--rw-r--r--   0 katiek     (501) staff       (20)    11653 2021-07-29 17:37:15.000000 repytah-0.1.0/docs/_build/html/search_doc.html
--rw-r--r--   0 katiek     (501) staff       (20)    16557 2021-07-29 17:37:15.000000 repytah-0.1.0/docs/_build/html/searchindex.js
--rw-r--r--   0 katiek     (501) staff       (20)     9841 2021-07-29 17:37:15.000000 repytah-0.1.0/docs/_build/html/transform.html
--rw-r--r--   0 katiek     (501) staff       (20)    18990 2021-07-29 17:37:15.000000 repytah-0.1.0/docs/_build/html/utilities.html
-drwxr-xr-x   0 katiek     (501) staff       (20)        0 2023-02-16 14:27:03.822787 repytah-0.1.0/docs/_static/
--rw-r--r--   0 katiek     (501) staff       (20)    14652 2021-07-29 17:37:15.000000 repytah-0.1.0/docs/_static/basic.css
--rw-r--r--   0 katiek     (501) staff       (20)      224 2021-07-29 17:37:15.000000 repytah-0.1.0/docs/_static/custom.css
--rw-r--r--   0 katiek     (501) staff       (20)     9592 2021-07-29 17:37:15.000000 repytah-0.1.0/docs/_static/doctools.js
--rw-r--r--   0 katiek     (501) staff       (20)      350 2021-07-29 17:37:15.000000 repytah-0.1.0/docs/_static/documentation_options.js
--rw-r--r--   0 katiek     (501) staff       (20)      286 2021-07-29 17:37:15.000000 repytah-0.1.0/docs/_static/file.png
--rw-r--r--   0 katiek     (501) staff       (20)   268039 2021-07-29 17:37:15.000000 repytah-0.1.0/docs/_static/jquery-3.2.1.js
--rw-r--r--   0 katiek     (501) staff       (20)   287630 2021-07-29 17:37:15.000000 repytah-0.1.0/docs/_static/jquery-3.5.1.js
--rw-r--r--   0 katiek     (501) staff       (20)    89476 2021-07-29 17:37:15.000000 repytah-0.1.0/docs/_static/jquery.js
--rw-r--r--   0 katiek     (501) staff       (20)    10854 2021-07-29 17:37:15.000000 repytah-0.1.0/docs/_static/language_data.js
--rw-r--r--   0 katiek     (501) staff       (20)       90 2021-07-29 17:37:15.000000 repytah-0.1.0/docs/_static/minus.png
--rw-r--r--   0 katiek     (501) staff       (20)       90 2021-07-29 17:37:15.000000 repytah-0.1.0/docs/_static/plus.png
--rw-r--r--   0 katiek     (501) staff       (20)     5249 2021-07-29 17:37:15.000000 repytah-0.1.0/docs/_static/pygments.css
--rw-r--r--   0 katiek     (501) staff       (20)    16578 2021-07-29 17:37:15.000000 repytah-0.1.0/docs/_static/searchtools.js
--rw-r--r--   0 katiek     (501) staff       (20)    67692 2021-07-29 17:37:15.000000 repytah-0.1.0/docs/_static/underscore-1.12.0.js
--rw-r--r--   0 katiek     (501) staff       (20)    35168 2021-07-29 17:37:15.000000 repytah-0.1.0/docs/_static/underscore-1.3.1.js
--rw-r--r--   0 katiek     (501) staff       (20)    19358 2021-07-29 17:37:15.000000 repytah-0.1.0/docs/_static/underscore.js
--rw-r--r--   0 katiek     (501) staff       (20)     1518 2021-07-29 17:37:15.000000 repytah-0.1.0/docs/about.rst
--rw-r--r--   0 katiek     (501) staff       (20)     3549 2021-07-29 17:37:15.000000 repytah-0.1.0/docs/assemble.rst
--rw-r--r--   0 katiek     (501) staff       (20)      247 2023-01-30 13:28:27.000000 repytah-0.1.0/docs/assemble_import.rst
--rw-r--r--   0 katiek     (501) staff       (20)    66529 2023-01-30 13:28:27.000000 repytah-0.1.0/docs/assemble_vignette.ipynb
--rw-r--r--   0 katiek     (501) staff       (20)       76 2021-07-29 17:37:15.000000 repytah-0.1.0/docs/changelog.rst
--rw-r--r--   0 katiek     (501) staff       (20)     3445 2023-01-30 13:28:27.000000 repytah-0.1.0/docs/conf.py
--rw-r--r--   0 katiek     (501) staff       (20)  1255075 2023-01-30 13:28:27.000000 repytah-0.1.0/docs/example_vignette.ipynb
--rw-r--r--   0 katiek     (501) staff       (20)      837 2021-07-29 17:37:15.000000 repytah-0.1.0/docs/function_pipeline.rst
--rw-r--r--   0 katiek     (501) staff       (20)      791 2023-01-30 13:28:27.000000 repytah-0.1.0/docs/general_installation.rst
--rw-r--r--   0 katiek     (501) staff       (20)       29 2021-07-29 17:37:15.000000 repytah-0.1.0/docs/genindex.rst
--rw-r--r--   0 katiek     (501) staff       (20)      929 2023-02-13 16:27:33.000000 repytah-0.1.0/docs/index.rst
--rw-r--r--   0 katiek     (501) staff       (20)      760 2021-07-06 19:40:28.000000 repytah-0.1.0/docs/make.bat
-drwxr-xr-x   0 katiek     (501) staff       (20)        0 2023-02-16 14:27:03.825890 repytah-0.1.0/docs/pictures/
--rw-r--r--   0 katiek     (501) staff       (20)     4732 2021-07-06 19:40:28.000000 repytah-0.1.0/docs/pictures/Purple4.PNG
--rw-r--r--   0 katiek     (501) staff       (20)    14672 2021-07-06 19:40:28.000000 repytah-0.1.0/docs/pictures/Red1Blue1Purple1.PNG
--rw-r--r--   0 katiek     (501) staff       (20)    13959 2021-07-06 19:40:28.000000 repytah-0.1.0/docs/pictures/Red2Blue2Purple2.PNG
--rw-r--r--   0 katiek     (501) staff       (20)    13799 2021-07-06 19:40:28.000000 repytah-0.1.0/docs/pictures/Red2Blue2Purple4.PNG
--rw-r--r--   0 katiek     (501) staff       (20)    13622 2021-07-06 19:40:28.000000 repytah-0.1.0/docs/pictures/Red3Blue3Purple3.PNG
--rw-r--r--   0 katiek     (501) staff       (20)     8746 2021-07-06 19:40:28.000000 repytah-0.1.0/docs/pictures/find_all_repeats1.png
--rw-r--r--   0 katiek     (501) staff       (20)     9027 2021-07-06 19:40:28.000000 repytah-0.1.0/docs/pictures/find_all_repeats2.png
--rw-r--r--   0 katiek     (501) staff       (20)    12368 2021-07-06 19:40:28.000000 repytah-0.1.0/docs/pictures/find_all_repeats3.png
--rw-r--r--   0 katiek     (501) staff       (20)    44856 2022-01-26 19:47:49.000000 repytah-0.1.0/docs/pictures/find_complete_list_visualization.png
--rw-r--r--   0 katiek     (501) staff       (20)    26133 2021-07-06 19:40:28.000000 repytah-0.1.0/docs/pictures/find_initial_repeats.png
--rw-r--r--   0 katiek     (501) staff       (20)    58028 2021-07-29 17:37:15.000000 repytah-0.1.0/docs/pictures/function_flow_step.png
--rw-r--r--   0 katiek     (501) staff       (20)    31228 2021-07-06 19:40:28.000000 repytah-0.1.0/docs/pictures/function_flow_steps.PNG
--rw-r--r--   0 katiek     (501) staff       (20)    42222 2021-07-29 17:37:15.000000 repytah-0.1.0/docs/pictures/function_pipeline.jpg
--rw-r--r--   0 katiek     (501) staff       (20)    55141 2021-07-06 19:40:28.000000 repytah-0.1.0/docs/pictures/num_of_parts.png
--rw-r--r--   0 katiek     (501) staff       (20)   134848 2023-01-30 13:28:27.000000 repytah-0.1.0/docs/pictures/score.jpg
--rw-r--r--   0 katiek     (501) staff       (20)   409360 2023-01-30 13:28:27.000000 repytah-0.1.0/docs/pictures/score1.jpg
--rw-r--r--   0 katiek     (501) staff       (20)   421399 2023-01-30 13:28:27.000000 repytah-0.1.0/docs/pictures/score2.jpg
--rw-r--r--   0 katiek     (501) staff       (20)   958111 2023-01-30 13:28:27.000000 repytah-0.1.0/docs/quick_start.ipynb
--rw-r--r--   0 katiek     (501) staff       (20)      565 2023-01-30 13:28:27.000000 repytah-0.1.0/docs/recommended_installation.rst
--rw-r--r--   0 katiek     (501) staff       (20)      201 2023-01-30 13:28:27.000000 repytah-0.1.0/docs/requirements.txt
--rw-r--r--   0 katiek     (501) staff       (20)     2491 2022-01-26 19:47:49.000000 repytah-0.1.0/docs/search_doc.rst
--rw-r--r--   0 katiek     (501) staff       (20)      165 2023-01-30 13:28:27.000000 repytah-0.1.0/docs/search_import.rst
--rw-r--r--   0 katiek     (501) staff       (20)    12955 2022-01-26 19:47:49.000000 repytah-0.1.0/docs/search_vignette.ipynb
--rw-r--r--   0 katiek     (501) staff       (20)     2105 2021-07-29 17:37:15.000000 repytah-0.1.0/docs/transform.rst
--rw-r--r--   0 katiek     (501) staff       (20)      162 2023-01-30 13:28:27.000000 repytah-0.1.0/docs/transform_import.rst
--rw-r--r--   0 katiek     (501) staff       (20)     5882 2023-01-30 13:28:27.000000 repytah-0.1.0/docs/transform_vignette.ipynb
--rw-r--r--   0 katiek     (501) staff       (20)     5821 2021-07-29 17:37:15.000000 repytah-0.1.0/docs/utilities.rst
--rw-r--r--   0 katiek     (501) staff       (20)      244 2023-01-30 13:28:27.000000 repytah-0.1.0/docs/utilities_import.rst
--rw-r--r--   0 katiek     (501) staff       (20)    29683 2021-07-29 17:37:15.000000 repytah-0.1.0/docs/utilities_vignette.ipynb
--rw-r--r--   0 katiek     (501) staff       (20)       86 2023-02-16 14:19:23.000000 repytah-0.1.0/pyproject.toml
-drwxr-xr-x   0 katiek     (501) staff       (20)        0 2023-02-16 14:27:03.827335 repytah-0.1.0/repytah/
--rw-r--r--   0 katiek     (501) staff       (20)      260 2023-02-16 13:08:16.000000 repytah-0.1.0/repytah/__init__.py
--rw-r--r--   0 katiek     (501) staff       (20)    42108 2023-02-16 13:08:16.000000 repytah-0.1.0/repytah/assemble.py
-drwxr-xr-x   0 katiek     (501) staff       (20)        0 2023-02-16 14:27:03.828803 repytah-0.1.0/repytah/data/
--rw-r--r--   0 katiek     (501) staff       (20)   100800 2023-02-16 13:08:16.000000 repytah-0.1.0/repytah/data/input.csv
--rw-r--r--   0 katiek     (501) staff       (20)    47700 2023-02-16 13:08:16.000000 repytah-0.1.0/repytah/data/mazurka30-1.csv
--rw-r--r--   0 katiek     (501) staff       (20)    99300 2023-02-16 13:08:16.000000 repytah-0.1.0/repytah/data/mazurka30-3.csv
--rw-r--r--   0 katiek     (501) staff       (20)     6899 2023-02-16 13:08:16.000000 repytah-0.1.0/repytah/example.py
--rw-r--r--   0 katiek     (501) staff       (20)    22743 2023-02-16 13:08:16.000000 repytah-0.1.0/repytah/search.py
--rw-r--r--   0 katiek     (501) staff       (20)    16025 2023-02-16 13:08:16.000000 repytah-0.1.0/repytah/transform.py
--rw-r--r--   0 katiek     (501) staff       (20)    23840 2023-02-16 13:08:16.000000 repytah-0.1.0/repytah/utilities.py
--rw-r--r--   0 katiek     (501) staff       (20)     1225 2023-02-16 13:08:16.000000 repytah-0.1.0/repytah/version.py
-drwxr-xr-x   0 katiek     (501) staff       (20)        0 2023-02-16 14:27:03.828303 repytah-0.1.0/repytah.egg-info/
--rw-r--r--   0 katiek     (501) staff       (20)     5734 2023-02-16 14:27:03.000000 repytah-0.1.0/repytah.egg-info/PKG-INFO
--rw-r--r--   0 katiek     (501) staff       (20)     3444 2023-02-16 14:27:03.000000 repytah-0.1.0/repytah.egg-info/SOURCES.txt
--rw-r--r--   0 katiek     (501) staff       (20)        1 2023-02-16 14:27:03.000000 repytah-0.1.0/repytah.egg-info/dependency_links.txt
--rw-r--r--   0 katiek     (501) staff       (20)      260 2023-02-16 14:27:03.000000 repytah-0.1.0/repytah.egg-info/requires.txt
--rw-r--r--   0 katiek     (501) staff       (20)        8 2023-02-16 14:27:03.000000 repytah-0.1.0/repytah.egg-info/top_level.txt
--rw-r--r--   0 katiek     (501) staff       (20)       38 2023-02-16 14:27:03.830013 repytah-0.1.0/setup.cfg
--rw-r--r--   0 katiek     (501) staff       (20)     1800 2023-02-16 14:19:23.000000 repytah-0.1.0/setup.py
-drwxr-xr-x   0 katiek     (501) staff       (20)        0 2023-02-16 14:27:03.829576 repytah-0.1.0/test/
--rw-r--r--   0 katiek     (501) staff       (20)    10155 2023-02-16 12:47:40.000000 repytah-0.1.0/test/test_assemble.py
--rw-r--r--   0 katiek     (501) staff       (20)     1806 2023-01-30 13:28:27.000000 repytah-0.1.0/test/test_example.py
--rwxr-xr-x   0 katiek     (501) staff       (20)    11606 2023-01-30 13:28:27.000000 repytah-0.1.0/test/test_search.py
--rw-r--r--   0 katiek     (501) staff       (20)    33835 2023-01-30 13:28:27.000000 repytah-0.1.0/test/test_transform.py
--rw-r--r--   0 katiek     (501) staff       (20)    16125 2023-01-30 13:28:27.000000 repytah-0.1.0/test/test_utilities.py
+drwxr-xr-x   0 katiek     (501) staff       (20)        0 2023-05-05 09:26:54.178023 repytah-0.1.1/
+-rw-r--r--   0 katiek     (501) staff       (20)      669 2023-02-16 14:19:23.000000 repytah-0.1.1/AUTHORS.md
+-rw-r--r--   0 katiek     (501) staff       (20)     3430 2021-07-29 17:37:15.000000 repytah-0.1.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 katiek     (501) staff       (20)      792 2023-02-16 14:19:23.000000 repytah-0.1.1/LICENSE.md
+-rw-r--r--   0 katiek     (501) staff       (20)      156 2021-07-29 17:37:15.000000 repytah-0.1.1/MANIFEST.in
+-rw-r--r--   0 katiek     (501) staff       (20)     7220 2023-05-05 09:26:54.177819 repytah-0.1.1/PKG-INFO
+-rw-r--r--   0 katiek     (501) staff       (20)     6223 2023-05-05 09:24:05.000000 repytah-0.1.1/README.md
+drwxr-xr-x   0 katiek     (501) staff       (20)        0 2023-05-05 09:26:54.150838 repytah-0.1.1/docs/
+drwxr-xr-x   0 katiek     (501) staff       (20)        0 2023-05-05 09:26:54.151059 repytah-0.1.1/docs/.ipynb_checkpoints/
+-rw-r--r--   0 katiek     (501) staff       (20)   316363 2021-07-30 02:08:42.000000 repytah-0.1.1/docs/.ipynb_checkpoints/example_vignette-checkpoint.ipynb
+-rw-r--r--   0 katiek     (501) staff       (20)      634 2021-07-06 19:40:28.000000 repytah-0.1.1/docs/Makefile
+drwxr-xr-x   0 katiek     (501) staff       (20)        0 2023-05-05 09:26:54.139487 repytah-0.1.1/docs/_build/
+drwxr-xr-x   0 katiek     (501) staff       (20)        0 2023-05-05 09:26:54.153294 repytah-0.1.1/docs/_build/doctrees/
+-rw-r--r--   0 katiek     (501) staff       (20)    25279 2021-07-29 17:37:15.000000 repytah-0.1.1/docs/_build/doctrees/assemble.doctree
+-rw-r--r--   0 katiek     (501) staff       (20)    67237 2021-07-29 17:37:15.000000 repytah-0.1.1/docs/_build/doctrees/environment.pickle
+-rw-r--r--   0 katiek     (501) staff       (20)     5445 2021-07-29 17:37:15.000000 repytah-0.1.1/docs/_build/doctrees/index.doctree
+-rw-r--r--   0 katiek     (501) staff       (20)    18207 2021-07-29 17:37:15.000000 repytah-0.1.1/docs/_build/doctrees/search_doc.doctree
+-rw-r--r--   0 katiek     (501) staff       (20)    13646 2021-07-29 17:37:15.000000 repytah-0.1.1/docs/_build/doctrees/transform.doctree
+-rw-r--r--   0 katiek     (501) staff       (20)    43724 2021-07-29 17:37:15.000000 repytah-0.1.1/docs/_build/doctrees/utilities.doctree
+drwxr-xr-x   0 katiek     (501) staff       (20)        0 2023-05-05 09:26:54.155578 repytah-0.1.1/docs/_build/html/
+-rw-r--r--   0 katiek     (501) staff       (20)      230 2021-07-29 17:37:15.000000 repytah-0.1.1/docs/_build/html/.buildinfo
+drwxr-xr-x   0 katiek     (501) staff       (20)        0 2023-05-05 09:26:54.155776 repytah-0.1.1/docs/_build/html/_sources/
+-rw-r--r--   0 katiek     (501) staff       (20)      811 2021-07-29 17:37:15.000000 repytah-0.1.1/docs/_build/html/_sources/index.rst.txt
+drwxr-xr-x   0 katiek     (501) staff       (20)        0 2023-05-05 09:26:54.160602 repytah-0.1.1/docs/_build/html/_static/
+-rw-r--r--   0 katiek     (501) staff       (20)    14652 2021-07-06 19:40:28.000000 repytah-0.1.1/docs/_build/html/_static/basic.css
+-rw-r--r--   0 katiek     (501) staff       (20)      224 2021-07-29 17:37:15.000000 repytah-0.1.1/docs/_build/html/_static/custom.css
+-rw-r--r--   0 katiek     (501) staff       (20)     9592 2021-07-06 19:40:28.000000 repytah-0.1.1/docs/_build/html/_static/doctools.js
+-rw-r--r--   0 katiek     (501) staff       (20)      350 2021-07-06 19:40:28.000000 repytah-0.1.1/docs/_build/html/_static/documentation_options.js
+-rw-r--r--   0 katiek     (501) staff       (20)      286 2021-07-06 19:40:28.000000 repytah-0.1.1/docs/_build/html/_static/file.png
+-rw-r--r--   0 katiek     (501) staff       (20)   268039 2021-07-06 19:40:28.000000 repytah-0.1.1/docs/_build/html/_static/jquery-3.2.1.js
+-rw-r--r--   0 katiek     (501) staff       (20)   287630 2021-07-06 19:40:28.000000 repytah-0.1.1/docs/_build/html/_static/jquery-3.5.1.js
+-rw-r--r--   0 katiek     (501) staff       (20)    89476 2021-07-06 19:40:28.000000 repytah-0.1.1/docs/_build/html/_static/jquery.js
+-rw-r--r--   0 katiek     (501) staff       (20)    10854 2021-07-06 19:40:28.000000 repytah-0.1.1/docs/_build/html/_static/language_data.js
+-rw-r--r--   0 katiek     (501) staff       (20)       90 2021-07-06 19:40:28.000000 repytah-0.1.1/docs/_build/html/_static/minus.png
+-rw-r--r--   0 katiek     (501) staff       (20)       90 2021-07-06 19:40:28.000000 repytah-0.1.1/docs/_build/html/_static/plus.png
+-rw-r--r--   0 katiek     (501) staff       (20)     5249 2021-07-06 19:40:28.000000 repytah-0.1.1/docs/_build/html/_static/pygments.css
+-rw-r--r--   0 katiek     (501) staff       (20)    16578 2021-07-06 19:40:28.000000 repytah-0.1.1/docs/_build/html/_static/searchtools.js
+-rw-r--r--   0 katiek     (501) staff       (20)    67692 2021-07-06 19:40:28.000000 repytah-0.1.1/docs/_build/html/_static/underscore-1.12.0.js
+-rw-r--r--   0 katiek     (501) staff       (20)    35168 2021-07-06 19:40:28.000000 repytah-0.1.1/docs/_build/html/_static/underscore-1.3.1.js
+-rw-r--r--   0 katiek     (501) staff       (20)    19358 2021-07-06 19:40:28.000000 repytah-0.1.1/docs/_build/html/_static/underscore.js
+-rw-r--r--   0 katiek     (501) staff       (20)    13249 2021-07-29 17:37:15.000000 repytah-0.1.1/docs/_build/html/assemble.html
+-rw-r--r--   0 katiek     (501) staff       (20)    16094 2021-07-29 17:37:15.000000 repytah-0.1.1/docs/_build/html/genindex.html
+-rw-r--r--   0 katiek     (501) staff       (20)     9037 2021-07-29 17:37:15.000000 repytah-0.1.1/docs/_build/html/index.html
+-rw-r--r--   0 katiek     (501) staff       (20)     2535 2021-07-29 17:37:15.000000 repytah-0.1.1/docs/_build/html/objects.inv
+-rw-r--r--   0 katiek     (501) staff       (20)     7045 2021-07-29 17:37:15.000000 repytah-0.1.1/docs/_build/html/py-modindex.html
+-rw-r--r--   0 katiek     (501) staff       (20)     6150 2021-07-29 17:37:15.000000 repytah-0.1.1/docs/_build/html/search.html
+-rw-r--r--   0 katiek     (501) staff       (20)    11653 2021-07-29 17:37:15.000000 repytah-0.1.1/docs/_build/html/search_doc.html
+-rw-r--r--   0 katiek     (501) staff       (20)    16557 2021-07-29 17:37:15.000000 repytah-0.1.1/docs/_build/html/searchindex.js
+-rw-r--r--   0 katiek     (501) staff       (20)     9841 2021-07-29 17:37:15.000000 repytah-0.1.1/docs/_build/html/transform.html
+-rw-r--r--   0 katiek     (501) staff       (20)    18990 2021-07-29 17:37:15.000000 repytah-0.1.1/docs/_build/html/utilities.html
+drwxr-xr-x   0 katiek     (501) staff       (20)        0 2023-05-05 09:26:54.165669 repytah-0.1.1/docs/_static/
+-rw-r--r--   0 katiek     (501) staff       (20)    14652 2021-07-29 17:37:15.000000 repytah-0.1.1/docs/_static/basic.css
+-rw-r--r--   0 katiek     (501) staff       (20)      224 2021-07-29 17:37:15.000000 repytah-0.1.1/docs/_static/custom.css
+-rw-r--r--   0 katiek     (501) staff       (20)     9592 2021-07-29 17:37:15.000000 repytah-0.1.1/docs/_static/doctools.js
+-rw-r--r--   0 katiek     (501) staff       (20)      350 2021-07-29 17:37:15.000000 repytah-0.1.1/docs/_static/documentation_options.js
+-rw-r--r--   0 katiek     (501) staff       (20)      286 2021-07-29 17:37:15.000000 repytah-0.1.1/docs/_static/file.png
+-rw-r--r--   0 katiek     (501) staff       (20)   268039 2021-07-29 17:37:15.000000 repytah-0.1.1/docs/_static/jquery-3.2.1.js
+-rw-r--r--   0 katiek     (501) staff       (20)   287630 2021-07-29 17:37:15.000000 repytah-0.1.1/docs/_static/jquery-3.5.1.js
+-rw-r--r--   0 katiek     (501) staff       (20)    89476 2021-07-29 17:37:15.000000 repytah-0.1.1/docs/_static/jquery.js
+-rw-r--r--   0 katiek     (501) staff       (20)    10854 2021-07-29 17:37:15.000000 repytah-0.1.1/docs/_static/language_data.js
+-rw-r--r--   0 katiek     (501) staff       (20)       90 2021-07-29 17:37:15.000000 repytah-0.1.1/docs/_static/minus.png
+-rw-r--r--   0 katiek     (501) staff       (20)       90 2021-07-29 17:37:15.000000 repytah-0.1.1/docs/_static/plus.png
+-rw-r--r--   0 katiek     (501) staff       (20)     5249 2021-07-29 17:37:15.000000 repytah-0.1.1/docs/_static/pygments.css
+-rw-r--r--   0 katiek     (501) staff       (20)    16578 2021-07-29 17:37:15.000000 repytah-0.1.1/docs/_static/searchtools.js
+-rw-r--r--   0 katiek     (501) staff       (20)    67692 2021-07-29 17:37:15.000000 repytah-0.1.1/docs/_static/underscore-1.12.0.js
+-rw-r--r--   0 katiek     (501) staff       (20)    35168 2021-07-29 17:37:15.000000 repytah-0.1.1/docs/_static/underscore-1.3.1.js
+-rw-r--r--   0 katiek     (501) staff       (20)    19358 2021-07-29 17:37:15.000000 repytah-0.1.1/docs/_static/underscore.js
+-rw-r--r--   0 katiek     (501) staff       (20)     1518 2021-07-29 17:37:15.000000 repytah-0.1.1/docs/about.rst
+-rw-r--r--   0 katiek     (501) staff       (20)     3549 2021-07-29 17:37:15.000000 repytah-0.1.1/docs/assemble.rst
+-rw-r--r--   0 katiek     (501) staff       (20)      247 2023-01-30 13:28:27.000000 repytah-0.1.1/docs/assemble_import.rst
+-rw-r--r--   0 katiek     (501) staff       (20)    66529 2023-01-30 13:28:27.000000 repytah-0.1.1/docs/assemble_vignette.ipynb
+-rw-r--r--   0 katiek     (501) staff       (20)       76 2021-07-29 17:37:15.000000 repytah-0.1.1/docs/changelog.rst
+-rw-r--r--   0 katiek     (501) staff       (20)     3445 2023-01-30 13:28:27.000000 repytah-0.1.1/docs/conf.py
+-rw-r--r--   0 katiek     (501) staff       (20)  1255075 2023-01-30 13:28:27.000000 repytah-0.1.1/docs/example_vignette.ipynb
+-rw-r--r--   0 katiek     (501) staff       (20)      837 2021-07-29 17:37:15.000000 repytah-0.1.1/docs/function_pipeline.rst
+-rw-r--r--   0 katiek     (501) staff       (20)      914 2023-05-05 09:24:05.000000 repytah-0.1.1/docs/general_installation.rst
+-rw-r--r--   0 katiek     (501) staff       (20)       29 2021-07-29 17:37:15.000000 repytah-0.1.1/docs/genindex.rst
+-rw-r--r--   0 katiek     (501) staff       (20)      929 2023-02-13 16:27:33.000000 repytah-0.1.1/docs/index.rst
+-rw-r--r--   0 katiek     (501) staff       (20)      760 2021-07-06 19:40:28.000000 repytah-0.1.1/docs/make.bat
+drwxr-xr-x   0 katiek     (501) staff       (20)        0 2023-05-05 09:26:54.171515 repytah-0.1.1/docs/pictures/
+-rw-r--r--   0 katiek     (501) staff       (20)     4732 2021-07-06 19:40:28.000000 repytah-0.1.1/docs/pictures/Purple4.PNG
+-rw-r--r--   0 katiek     (501) staff       (20)    14672 2021-07-06 19:40:28.000000 repytah-0.1.1/docs/pictures/Red1Blue1Purple1.PNG
+-rw-r--r--   0 katiek     (501) staff       (20)    13959 2021-07-06 19:40:28.000000 repytah-0.1.1/docs/pictures/Red2Blue2Purple2.PNG
+-rw-r--r--   0 katiek     (501) staff       (20)    13799 2021-07-06 19:40:28.000000 repytah-0.1.1/docs/pictures/Red2Blue2Purple4.PNG
+-rw-r--r--   0 katiek     (501) staff       (20)    13622 2021-07-06 19:40:28.000000 repytah-0.1.1/docs/pictures/Red3Blue3Purple3.PNG
+-rw-r--r--   0 katiek     (501) staff       (20)     8746 2021-07-06 19:40:28.000000 repytah-0.1.1/docs/pictures/find_all_repeats1.png
+-rw-r--r--   0 katiek     (501) staff       (20)     9027 2021-07-06 19:40:28.000000 repytah-0.1.1/docs/pictures/find_all_repeats2.png
+-rw-r--r--   0 katiek     (501) staff       (20)    12368 2021-07-06 19:40:28.000000 repytah-0.1.1/docs/pictures/find_all_repeats3.png
+-rw-r--r--   0 katiek     (501) staff       (20)    44856 2022-01-26 19:47:49.000000 repytah-0.1.1/docs/pictures/find_complete_list_visualization.png
+-rw-r--r--   0 katiek     (501) staff       (20)    26133 2021-07-06 19:40:28.000000 repytah-0.1.1/docs/pictures/find_initial_repeats.png
+-rw-r--r--   0 katiek     (501) staff       (20)    58028 2021-07-29 17:37:15.000000 repytah-0.1.1/docs/pictures/function_flow_step.png
+-rw-r--r--   0 katiek     (501) staff       (20)    31228 2021-07-06 19:40:28.000000 repytah-0.1.1/docs/pictures/function_flow_steps.PNG
+-rw-r--r--   0 katiek     (501) staff       (20)    42222 2021-07-29 17:37:15.000000 repytah-0.1.1/docs/pictures/function_pipeline.jpg
+-rw-r--r--   0 katiek     (501) staff       (20)    55141 2021-07-06 19:40:28.000000 repytah-0.1.1/docs/pictures/num_of_parts.png
+-rw-r--r--   0 katiek     (501) staff       (20)   134848 2023-01-30 13:28:27.000000 repytah-0.1.1/docs/pictures/score.jpg
+-rw-r--r--   0 katiek     (501) staff       (20)   409360 2023-01-30 13:28:27.000000 repytah-0.1.1/docs/pictures/score1.jpg
+-rw-r--r--   0 katiek     (501) staff       (20)   421399 2023-01-30 13:28:27.000000 repytah-0.1.1/docs/pictures/score2.jpg
+-rw-r--r--   0 katiek     (501) staff       (20)   958111 2023-01-30 13:28:27.000000 repytah-0.1.1/docs/quick_start.ipynb
+-rw-r--r--   0 katiek     (501) staff       (20)      594 2023-05-05 09:24:05.000000 repytah-0.1.1/docs/recommended_installation.rst
+-rw-r--r--   0 katiek     (501) staff       (20)      201 2023-01-30 13:28:27.000000 repytah-0.1.1/docs/requirements.txt
+-rw-r--r--   0 katiek     (501) staff       (20)     2491 2022-01-26 19:47:49.000000 repytah-0.1.1/docs/search_doc.rst
+-rw-r--r--   0 katiek     (501) staff       (20)      165 2023-01-30 13:28:27.000000 repytah-0.1.1/docs/search_import.rst
+-rw-r--r--   0 katiek     (501) staff       (20)    12955 2022-01-26 19:47:49.000000 repytah-0.1.1/docs/search_vignette.ipynb
+-rw-r--r--   0 katiek     (501) staff       (20)     2105 2021-07-29 17:37:15.000000 repytah-0.1.1/docs/transform.rst
+-rw-r--r--   0 katiek     (501) staff       (20)      162 2023-01-30 13:28:27.000000 repytah-0.1.1/docs/transform_import.rst
+-rw-r--r--   0 katiek     (501) staff       (20)     5882 2023-01-30 13:28:27.000000 repytah-0.1.1/docs/transform_vignette.ipynb
+-rw-r--r--   0 katiek     (501) staff       (20)     5821 2021-07-29 17:37:15.000000 repytah-0.1.1/docs/utilities.rst
+-rw-r--r--   0 katiek     (501) staff       (20)      244 2023-01-30 13:28:27.000000 repytah-0.1.1/docs/utilities_import.rst
+-rw-r--r--   0 katiek     (501) staff       (20)    29683 2021-07-29 17:37:15.000000 repytah-0.1.1/docs/utilities_vignette.ipynb
+-rw-r--r--   0 katiek     (501) staff       (20)       86 2023-02-16 14:19:23.000000 repytah-0.1.1/pyproject.toml
+drwxr-xr-x   0 katiek     (501) staff       (20)        0 2023-05-05 09:26:54.174376 repytah-0.1.1/repytah/
+-rw-r--r--   0 katiek     (501) staff       (20)      260 2023-02-16 13:08:16.000000 repytah-0.1.1/repytah/__init__.py
+-rw-r--r--   0 katiek     (501) staff       (20)    42108 2023-02-16 13:08:16.000000 repytah-0.1.1/repytah/assemble.py
+drwxr-xr-x   0 katiek     (501) staff       (20)        0 2023-05-05 09:26:54.176180 repytah-0.1.1/repytah/data/
+-rw-r--r--   0 katiek     (501) staff       (20)     2308 2023-05-05 09:24:05.000000 repytah-0.1.1/repytah/data/README.md
+-rw-r--r--   0 katiek     (501) staff       (20)   100800 2023-02-16 13:08:16.000000 repytah-0.1.1/repytah/data/input.csv
+-rw-r--r--   0 katiek     (501) staff       (20)    47700 2023-02-16 13:08:16.000000 repytah-0.1.1/repytah/data/mazurka30-1.csv
+-rw-r--r--   0 katiek     (501) staff       (20)    99300 2023-02-16 13:08:16.000000 repytah-0.1.1/repytah/data/mazurka30-3.csv
+-rw-r--r--   0 katiek     (501) staff       (20)     6899 2023-02-16 13:08:16.000000 repytah-0.1.1/repytah/example.py
+-rw-r--r--   0 katiek     (501) staff       (20)    22743 2023-02-16 13:08:16.000000 repytah-0.1.1/repytah/search.py
+-rw-r--r--   0 katiek     (501) staff       (20)    16025 2023-02-16 13:08:16.000000 repytah-0.1.1/repytah/transform.py
+-rw-r--r--   0 katiek     (501) staff       (20)    23840 2023-02-16 13:08:16.000000 repytah-0.1.1/repytah/utilities.py
+-rw-r--r--   0 katiek     (501) staff       (20)     1225 2023-02-16 13:08:16.000000 repytah-0.1.1/repytah/version.py
+drwxr-xr-x   0 katiek     (501) staff       (20)        0 2023-05-05 09:26:54.175100 repytah-0.1.1/repytah.egg-info/
+-rw-r--r--   0 katiek     (501) staff       (20)     7220 2023-05-05 09:26:54.000000 repytah-0.1.1/repytah.egg-info/PKG-INFO
+-rw-r--r--   0 katiek     (501) staff       (20)     3467 2023-05-05 09:26:54.000000 repytah-0.1.1/repytah.egg-info/SOURCES.txt
+-rw-r--r--   0 katiek     (501) staff       (20)        1 2023-05-05 09:26:54.000000 repytah-0.1.1/repytah.egg-info/dependency_links.txt
+-rw-r--r--   0 katiek     (501) staff       (20)      260 2023-05-05 09:26:54.000000 repytah-0.1.1/repytah.egg-info/requires.txt
+-rw-r--r--   0 katiek     (501) staff       (20)        8 2023-05-05 09:26:54.000000 repytah-0.1.1/repytah.egg-info/top_level.txt
+-rw-r--r--   0 katiek     (501) staff       (20)       38 2023-05-05 09:26:54.178071 repytah-0.1.1/setup.cfg
+-rw-r--r--   0 katiek     (501) staff       (20)     1800 2023-05-05 09:25:01.000000 repytah-0.1.1/setup.py
+drwxr-xr-x   0 katiek     (501) staff       (20)        0 2023-05-05 09:26:54.177539 repytah-0.1.1/test/
+-rw-r--r--   0 katiek     (501) staff       (20)    10155 2023-02-16 12:47:40.000000 repytah-0.1.1/test/test_assemble.py
+-rw-r--r--   0 katiek     (501) staff       (20)     1806 2023-01-30 13:28:27.000000 repytah-0.1.1/test/test_example.py
+-rwxr-xr-x   0 katiek     (501) staff       (20)    11606 2023-01-30 13:28:27.000000 repytah-0.1.1/test/test_search.py
+-rw-r--r--   0 katiek     (501) staff       (20)    33835 2023-01-30 13:28:27.000000 repytah-0.1.1/test/test_transform.py
+-rw-r--r--   0 katiek     (501) staff       (20)    16125 2023-01-30 13:28:27.000000 repytah-0.1.1/test/test_utilities.py
```

### Comparing `repytah-0.1.0/AUTHORS.md` & `repytah-0.1.1/AUTHORS.md`

 * *Files identical despite different names*

### Comparing `repytah-0.1.0/CODE_OF_CONDUCT.md` & `repytah-0.1.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `repytah-0.1.0/LICENSE.md` & `repytah-0.1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `repytah-0.1.0/PKG-INFO` & `repytah-0.1.1/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,32 +1,7 @@
-Metadata-Version: 2.1
-Name: repytah
-Version: 0.1.0
-Summary: Python package for building Aligned Hierarchies for sequential data streams
-Home-page: https://github.com/smith-tinkerlab/repytah
-Author: Smith Tinker Lab, Katherine M. Kinnaird (PI)
-Author-email: tinkerlab@smith.edu
-License: ISC
-Project-URL: Bug Reports, https://github.com/smith-tinkerlab/repytah/issues
-Project-URL: Source, https://github.com/smith-tinkerlab/repytah
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: ISC License (ISCL)
-Classifier: Topic :: Multimedia :: Sound/Audio :: Analysis
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.7, <4
-Description-Content-Type: text/markdown
-Provides-Extra: docs
-Provides-Extra: tests
-License-File: LICENSE.md
-License-File: AUTHORS.md
-
 # <img alt="repytah" src="branding/repytah_logo.png" height="100">
 
 A Python package that builds aligned hierarchies for sequential data streams.
 
 [![PyPI](https://img.shields.io/pypi/v/repytah.svg)](https://pypi.python.org/pypi/repytah)
 [![Anaconda-Server Badge](https://anaconda.org/conda-forge/repytah/badges/version.svg)](https://anaconda.org/conda-forge/repytah)
 
@@ -37,15 +12,19 @@
 
 ## Documentation
 
 See our [website](https://repytah.readthedocs.io/en/latest/index.html) for a complete reference manual and introductory tutorials.
 
 This [example](https://repytah.readthedocs.io/en/latest/example_vignette.html) tutorial will show you a usage of the package from start to finish.
 
-## Statement of Need
+## Summary
+
+We introduce `repytah`, a Python package that constructs the aligned hierarchies representation that contains all possible structure-based hierarchical decompositions for a finite length piece of sequential data aligned on a common time axis. In particular, this representation--introduced by Kinnaird [@Kinnaird_ah] with music-based data (like musical recordings or scores) as the primary motivation--is intended for sequential data where repetitions have particular meaning (such as a verse, chorus, motif, or theme). Although the original motivation for the aligned hierarchies representation was finding structure for music-based data streams, there is nothing inherent in the construction of these representations that limits `repytah` to only being used on sequential data that is music-based. 
+
+The `repytah` package builds these aligned hierarchies by first extracting repeated structures (of all meaningful lengths) from the self-dissimilarity matrix (SDM) for a piece of sequential data. Intentionally `repytah` uses the SDM as the starting point for constructing the aligned hierarchies, as an SDM cannot be reversed-engineered back to the original signal and allows for researchers to collaborate with signals that are protected either by copyright or under privacy considerations. This package is a Python translation of the original MATLAB code by Kinnaird [-@Kinnaird_code] with additional documentation, and the code has been updated to leverage efficiencies in Python. 
 
 ### Problems Addressed
 
 Sequential data streams often have repeated elements that build on each other, creating hierarchies. Therefore, the goal of `repytah` is to extract these repetitions and their relationships to each other in order to form aligned hierarchies.
 
 To learn more about aligned hierarchies, see this [paper](https://s18798.pcdn.co/ismir2016/wp-content/uploads/sites/2294/2016/07/020_Paper.pdf) by Kinnaird (ISMIR 2016) which introduces aligned hierarchies in the context of music-based data streams.
 
@@ -72,15 +51,15 @@
 To build repytah from source, say `python setup.py build`.
 Then, to install repytah, say `python setup.py install`.
 
 Alternatively, you can download or clone the repository and use `pip` to handle dependencies:
 
 ```bash
 unzip repytah.zip
-pip install -e repytah
+pip install -e repytah-main
 ```
 
 or
 
 ```bash
 git clone https://github.com/smith-tinkerlab/repytah.git
 pip install -e repytah
@@ -91,27 +70,27 @@
 ```bash
 repytah (0.x.x, /path/to/repytah)
 ```
 
 ## Current and Future Work - Elements of the Package
 
 * Aligned Hierarchies - This is the fundamental output of the package, of which derivatives can be built. The aligned hierarchies for a given sequential data stream is the collection of all possible **hierarchical** structure decompositions, **aligned** on a common time axis. To this end, we offer all possible structure decompositions in one cohesive object.
-  * Includes walk through file example.py using supplied input.csv
+  * Includes walk through file `example.py` using supplied `input.csv`
 * _Forthcoming_ Aligned sub-Hierarchies - (AsH) - These are derivatives of the aligned hierarchies and are described in [Aligned sub-Hierarchies: a structure-based approach to the cover song task](http://ismir2018.ircam.fr/doc/pdfs/81_Paper.pdf)
 * _Forthcoming_ Start-End and S_NL diagrams
 * _Forthcoming_ SuPP and MaPP representations
 
 ### MATLAB code
 
 The original code to this project was written in MATLAB by Katherine M. Kinnaird. It can be found [here](https://github.com/kmkinnaird/ThesisCode).
 
 ### Acknowledgements
 
-This code was developed as part of Smith College's Summer Undergraduate Research Fellowship (SURF) from 2019 to 2022, and has been partially funded by Smith College's CFCD funding mechanism. Additionally, as Kinnaird is the Clare Boothe Luce Assistant Professor of Computer Science and Statistical & Data Sciences at Smith College, this work has also been partially supported by Henry Luce Foundation's Clare Boothe Luce Program.
+This code was developed as part of Smith College's Summer Undergraduate Research Fellowship (SURF) from 2019 to 2022 and has been partially funded by Smith College's CFCD funding mechanism. Additionally, as Kinnaird is the Clare Boothe Luce Assistant Professor of Computer Science and Statistical & Data Sciences at Smith College, this work has also been partially supported by Henry Luce Foundation's Clare Boothe Luce Program.
 
 Additionally, we would like to acknowledge and give thanks to Brian McFee and the [librosa](https://github.com/librosa) team. We significantly referenced the Python package [librosa](https://github.com/librosa/librosa) in our development process.
 
 ### Citing
 
 Please cite `repytah` using the following:
 
-C. Jia et al., repytah: A Python package that builds aligned hierarchies for sequential data streams. Python package version 0.1.0, 2023. [Online]. Available: [https://github.com/smith-tinkerlab/repytah](https://github.com/smith-tinkerlab/repytah).
+C. Jia et al., repytah: A Python package that builds aligned hierarchies for sequential data streams. Python package version 0.1.1, 2023. [Online]. Available: [https://github.com/smith-tinkerlab/repytah](https://github.com/smith-tinkerlab/repytah).
```

### Comparing `repytah-0.1.0/README.md` & `repytah-0.1.1/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,32 @@
+Metadata-Version: 2.1
+Name: repytah
+Version: 0.1.1
+Summary: Python package for building Aligned Hierarchies for sequential data streams
+Home-page: https://github.com/smith-tinkerlab/repytah
+Author: Smith Tinker Lab, Katherine M. Kinnaird (PI)
+Author-email: tinkerlab@smith.edu
+License: ISC
+Project-URL: Bug Reports, https://github.com/smith-tinkerlab/repytah/issues
+Project-URL: Source, https://github.com/smith-tinkerlab/repytah
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: ISC License (ISCL)
+Classifier: Topic :: Multimedia :: Sound/Audio :: Analysis
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >=3.7, <4
+Description-Content-Type: text/markdown
+Provides-Extra: docs
+Provides-Extra: tests
+License-File: LICENSE.md
+License-File: AUTHORS.md
+
 # <img alt="repytah" src="branding/repytah_logo.png" height="100">
 
 A Python package that builds aligned hierarchies for sequential data streams.
 
 [![PyPI](https://img.shields.io/pypi/v/repytah.svg)](https://pypi.python.org/pypi/repytah)
 [![Anaconda-Server Badge](https://anaconda.org/conda-forge/repytah/badges/version.svg)](https://anaconda.org/conda-forge/repytah)
 
@@ -12,15 +37,19 @@
 
 ## Documentation
 
 See our [website](https://repytah.readthedocs.io/en/latest/index.html) for a complete reference manual and introductory tutorials.
 
 This [example](https://repytah.readthedocs.io/en/latest/example_vignette.html) tutorial will show you a usage of the package from start to finish.
 
-## Statement of Need
+## Summary
+
+We introduce `repytah`, a Python package that constructs the aligned hierarchies representation that contains all possible structure-based hierarchical decompositions for a finite length piece of sequential data aligned on a common time axis. In particular, this representation--introduced by Kinnaird [@Kinnaird_ah] with music-based data (like musical recordings or scores) as the primary motivation--is intended for sequential data where repetitions have particular meaning (such as a verse, chorus, motif, or theme). Although the original motivation for the aligned hierarchies representation was finding structure for music-based data streams, there is nothing inherent in the construction of these representations that limits `repytah` to only being used on sequential data that is music-based. 
+
+The `repytah` package builds these aligned hierarchies by first extracting repeated structures (of all meaningful lengths) from the self-dissimilarity matrix (SDM) for a piece of sequential data. Intentionally `repytah` uses the SDM as the starting point for constructing the aligned hierarchies, as an SDM cannot be reversed-engineered back to the original signal and allows for researchers to collaborate with signals that are protected either by copyright or under privacy considerations. This package is a Python translation of the original MATLAB code by Kinnaird [-@Kinnaird_code] with additional documentation, and the code has been updated to leverage efficiencies in Python. 
 
 ### Problems Addressed
 
 Sequential data streams often have repeated elements that build on each other, creating hierarchies. Therefore, the goal of `repytah` is to extract these repetitions and their relationships to each other in order to form aligned hierarchies.
 
 To learn more about aligned hierarchies, see this [paper](https://s18798.pcdn.co/ismir2016/wp-content/uploads/sites/2294/2016/07/020_Paper.pdf) by Kinnaird (ISMIR 2016) which introduces aligned hierarchies in the context of music-based data streams.
 
@@ -47,15 +76,15 @@
 To build repytah from source, say `python setup.py build`.
 Then, to install repytah, say `python setup.py install`.
 
 Alternatively, you can download or clone the repository and use `pip` to handle dependencies:
 
 ```bash
 unzip repytah.zip
-pip install -e repytah
+pip install -e repytah-main
 ```
 
 or
 
 ```bash
 git clone https://github.com/smith-tinkerlab/repytah.git
 pip install -e repytah
@@ -66,27 +95,27 @@
 ```bash
 repytah (0.x.x, /path/to/repytah)
 ```
 
 ## Current and Future Work - Elements of the Package
 
 * Aligned Hierarchies - This is the fundamental output of the package, of which derivatives can be built. The aligned hierarchies for a given sequential data stream is the collection of all possible **hierarchical** structure decompositions, **aligned** on a common time axis. To this end, we offer all possible structure decompositions in one cohesive object.
-  * Includes walk through file example.py using supplied input.csv
+  * Includes walk through file `example.py` using supplied `input.csv`
 * _Forthcoming_ Aligned sub-Hierarchies - (AsH) - These are derivatives of the aligned hierarchies and are described in [Aligned sub-Hierarchies: a structure-based approach to the cover song task](http://ismir2018.ircam.fr/doc/pdfs/81_Paper.pdf)
 * _Forthcoming_ Start-End and S_NL diagrams
 * _Forthcoming_ SuPP and MaPP representations
 
 ### MATLAB code
 
 The original code to this project was written in MATLAB by Katherine M. Kinnaird. It can be found [here](https://github.com/kmkinnaird/ThesisCode).
 
 ### Acknowledgements
 
-This code was developed as part of Smith College's Summer Undergraduate Research Fellowship (SURF) from 2019 to 2022, and has been partially funded by Smith College's CFCD funding mechanism. Additionally, as Kinnaird is the Clare Boothe Luce Assistant Professor of Computer Science and Statistical & Data Sciences at Smith College, this work has also been partially supported by Henry Luce Foundation's Clare Boothe Luce Program.
+This code was developed as part of Smith College's Summer Undergraduate Research Fellowship (SURF) from 2019 to 2022 and has been partially funded by Smith College's CFCD funding mechanism. Additionally, as Kinnaird is the Clare Boothe Luce Assistant Professor of Computer Science and Statistical & Data Sciences at Smith College, this work has also been partially supported by Henry Luce Foundation's Clare Boothe Luce Program.
 
 Additionally, we would like to acknowledge and give thanks to Brian McFee and the [librosa](https://github.com/librosa) team. We significantly referenced the Python package [librosa](https://github.com/librosa/librosa) in our development process.
 
 ### Citing
 
 Please cite `repytah` using the following:
 
-C. Jia et al., repytah: A Python package that builds aligned hierarchies for sequential data streams. Python package version 0.1.0, 2023. [Online]. Available: [https://github.com/smith-tinkerlab/repytah](https://github.com/smith-tinkerlab/repytah).
+C. Jia et al., repytah: A Python package that builds aligned hierarchies for sequential data streams. Python package version 0.1.1, 2023. [Online]. Available: [https://github.com/smith-tinkerlab/repytah](https://github.com/smith-tinkerlab/repytah).
```

### Comparing `repytah-0.1.0/docs/.ipynb_checkpoints/example_vignette-checkpoint.ipynb` & `repytah-0.1.1/docs/.ipynb_checkpoints/example_vignette-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `repytah-0.1.0/docs/Makefile` & `repytah-0.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `repytah-0.1.0/docs/_build/doctrees/assemble.doctree` & `repytah-0.1.1/docs/_build/doctrees/assemble.doctree`

 * *Files identical despite different names*

### Comparing `repytah-0.1.0/docs/_build/doctrees/environment.pickle` & `repytah-0.1.1/docs/_build/doctrees/environment.pickle`

 * *Files identical despite different names*

### Comparing `repytah-0.1.0/docs/_build/doctrees/index.doctree` & `repytah-0.1.1/docs/_build/doctrees/index.doctree`

 * *Files identical despite different names*

### Comparing `repytah-0.1.0/docs/_build/doctrees/search_doc.doctree` & `repytah-0.1.1/docs/_build/doctrees/search_doc.doctree`

 * *Files identical despite different names*

### Comparing `repytah-0.1.0/docs/_build/doctrees/transform.doctree` & `repytah-0.1.1/docs/_build/doctrees/transform.doctree`

 * *Files identical despite different names*

### Comparing `repytah-0.1.0/docs/_build/doctrees/utilities.doctree` & `repytah-0.1.1/docs/_build/doctrees/utilities.doctree`

 * *Files identical despite different names*

### Comparing `repytah-0.1.0/docs/_build/html/_sources/index.rst.txt` & `repytah-0.1.1/docs/_build/html/_sources/index.rst.txt`

 * *Files identical despite different names*

### Comparing `repytah-0.1.0/docs/_build/html/_static/basic.css` & `repytah-0.1.1/docs/_build/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `repytah-0.1.0/docs/_build/html/_static/doctools.js` & `repytah-0.1.1/docs/_build/html/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `repytah-0.1.0/docs/_build/html/_static/jquery-3.2.1.js` & `repytah-0.1.1/docs/_build/html/_static/jquery-3.2.1.js`

 * *Files identical despite different names*

### Comparing `repytah-0.1.0/docs/_build/html/_static/jquery-3.5.1.js` & `repytah-0.1.1/docs/_build/html/_static/jquery-3.5.1.js`

 * *Files identical despite different names*

### Comparing `repytah-0.1.0/docs/_build/html/_static/jquery.js` & `repytah-0.1.1/docs/_build/html/_static/jquery.js`

 * *Files identical despite different names*

### Comparing `repytah-0.1.0/docs/_build/html/_static/language_data.js` & `repytah-0.1.1/docs/_build/html/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `repytah-0.1.0/docs/_build/html/_static/pygments.css` & `repytah-0.1.1/docs/_build/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `repytah-0.1.0/docs/_build/html/_static/searchtools.js` & `repytah-0.1.1/docs/_build/html/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `repytah-0.1.0/docs/_build/html/_static/underscore-1.12.0.js` & `repytah-0.1.1/docs/_build/html/_static/underscore-1.12.0.js`

 * *Files identical despite different names*

### Comparing `repytah-0.1.0/docs/_build/html/_static/underscore-1.3.1.js` & `repytah-0.1.1/docs/_build/html/_static/underscore-1.3.1.js`

 * *Files identical despite different names*

### Comparing `repytah-0.1.0/docs/_build/html/_static/underscore.js` & `repytah-0.1.1/docs/_build/html/_static/underscore.js`

 * *Files identical despite different names*

### Comparing `repytah-0.1.0/docs/_build/html/assemble.html` & `repytah-0.1.1/docs/_build/html/assemble.html`

 * *Files identical despite different names*

### Comparing `repytah-0.1.0/docs/_build/html/genindex.html` & `repytah-0.1.1/docs/_build/html/genindex.html`

 * *Files identical despite different names*

### Comparing `repytah-0.1.0/docs/_build/html/index.html` & `repytah-0.1.1/docs/_build/html/index.html`

 * *Files identical despite different names*

### Comparing `repytah-0.1.0/docs/_build/html/objects.inv` & `repytah-0.1.1/docs/_build/html/objects.inv`

 * *Files identical despite different names*

### Comparing `repytah-0.1.0/docs/_build/html/py-modindex.html` & `repytah-0.1.1/docs/_build/html/py-modindex.html`

 * *Files identical despite different names*

### Comparing `repytah-0.1.0/docs/_build/html/search.html` & `repytah-0.1.1/docs/_build/html/search.html`

 * *Files identical despite different names*

### Comparing `repytah-0.1.0/docs/_build/html/search_doc.html` & `repytah-0.1.1/docs/_build/html/search_doc.html`

 * *Files identical despite different names*

### Comparing `repytah-0.1.0/docs/_build/html/searchindex.js` & `repytah-0.1.1/docs/_build/html/searchindex.js`

 * *Files identical despite different names*

### Comparing `repytah-0.1.0/docs/_build/html/transform.html` & `repytah-0.1.1/docs/_build/html/transform.html`

 * *Files identical despite different names*

### Comparing `repytah-0.1.0/docs/_build/html/utilities.html` & `repytah-0.1.1/docs/_build/html/utilities.html`

 * *Files identical despite different names*

### Comparing `repytah-0.1.0/docs/_static/basic.css` & `repytah-0.1.1/docs/_static/basic.css`

 * *Files identical despite different names*

### Comparing `repytah-0.1.0/docs/_static/doctools.js` & `repytah-0.1.1/docs/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `repytah-0.1.0/docs/_static/jquery-3.2.1.js` & `repytah-0.1.1/docs/_static/jquery-3.2.1.js`

 * *Files identical despite different names*

### Comparing `repytah-0.1.0/docs/_static/jquery-3.5.1.js` & `repytah-0.1.1/docs/_static/jquery-3.5.1.js`

 * *Files identical despite different names*

### Comparing `repytah-0.1.0/docs/_static/jquery.js` & `repytah-0.1.1/docs/_static/jquery.js`

 * *Files identical despite different names*

### Comparing `repytah-0.1.0/docs/_static/language_data.js` & `repytah-0.1.1/docs/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `repytah-0.1.0/docs/_static/pygments.css` & `repytah-0.1.1/docs/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `repytah-0.1.0/docs/_static/searchtools.js` & `repytah-0.1.1/docs/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `repytah-0.1.0/docs/_static/underscore-1.12.0.js` & `repytah-0.1.1/docs/_static/underscore-1.12.0.js`

 * *Files identical despite different names*

### Comparing `repytah-0.1.0/docs/_static/underscore-1.3.1.js` & `repytah-0.1.1/docs/_static/underscore-1.3.1.js`

 * *Files identical despite different names*

### Comparing `repytah-0.1.0/docs/_static/underscore.js` & `repytah-0.1.1/docs/_static/underscore.js`

 * *Files identical despite different names*

### Comparing `repytah-0.1.0/docs/about.rst` & `repytah-0.1.1/docs/about.rst`

 * *Files identical despite different names*

### Comparing `repytah-0.1.0/docs/assemble.rst` & `repytah-0.1.1/docs/assemble.rst`

 * *Files identical despite different names*

### Comparing `repytah-0.1.0/docs/assemble_vignette.ipynb` & `repytah-0.1.1/docs/assemble_vignette.ipynb`

 * *Files identical despite different names*

### Comparing `repytah-0.1.0/docs/conf.py` & `repytah-0.1.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `repytah-0.1.0/docs/example_vignette.ipynb` & `repytah-0.1.1/docs/example_vignette.ipynb`

 * *Files identical despite different names*

### Comparing `repytah-0.1.0/docs/function_pipeline.rst` & `repytah-0.1.1/docs/function_pipeline.rst`

 * *Files identical despite different names*

### Comparing `repytah-0.1.0/docs/general_installation.rst` & `repytah-0.1.1/docs/general_installation.rst`

 * *Files 23% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-General Installation
+Install from `pip` or `conda`
 ============
 
 PyPI
 ~~~~
 
 The latest stable release is available on PyPI, and you can install it by running::
 
@@ -14,23 +14,23 @@
 If you use Anaconda, you can install the package using ``conda-forge``::
 
     conda install -c conda-forge repytah
 
 Source
 ~~~~~~
 
-To build repytah from source, say ``python setup.py build``. Then, to install repytah, say ``python setup.py install``.
+To build repytah from source, you need to first clone the repo using ``git clone git@github.com:smith-tinkerlab/repytah.git``. Then build with ``python setup.py build``. Then, to install repytah, say ``python setup.py install``.
 
 Alternatively, you can download or clone the repository and use ``pip`` to handle dependencies::
 
     unzip repytah.zip
     pip install -e repytah
 
 or::
 
     git clone https://github.com/smith-tinkerlab/repytah.git
-    pip install -e repytah
+    pip install -e repytah-main
 
 By calling ``pip list`` you should see ``repytah`` now as an installed package::
 
     repytah (0.x.x, /path/to/repytah)
```

### Comparing `repytah-0.1.0/docs/index.rst` & `repytah-0.1.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `repytah-0.1.0/docs/make.bat` & `repytah-0.1.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `repytah-0.1.0/docs/pictures/Purple4.PNG` & `repytah-0.1.1/docs/pictures/Purple4.PNG`

 * *Files identical despite different names*

### Comparing `repytah-0.1.0/docs/pictures/Red1Blue1Purple1.PNG` & `repytah-0.1.1/docs/pictures/Red1Blue1Purple1.PNG`

 * *Files identical despite different names*

### Comparing `repytah-0.1.0/docs/pictures/Red2Blue2Purple2.PNG` & `repytah-0.1.1/docs/pictures/Red2Blue2Purple2.PNG`

 * *Files identical despite different names*

### Comparing `repytah-0.1.0/docs/pictures/Red2Blue2Purple4.PNG` & `repytah-0.1.1/docs/pictures/Red2Blue2Purple4.PNG`

 * *Files identical despite different names*

### Comparing `repytah-0.1.0/docs/pictures/Red3Blue3Purple3.PNG` & `repytah-0.1.1/docs/pictures/Red3Blue3Purple3.PNG`

 * *Files identical despite different names*

### Comparing `repytah-0.1.0/docs/pictures/find_all_repeats1.png` & `repytah-0.1.1/docs/pictures/find_all_repeats1.png`

 * *Files identical despite different names*

### Comparing `repytah-0.1.0/docs/pictures/find_all_repeats2.png` & `repytah-0.1.1/docs/pictures/find_all_repeats2.png`

 * *Files identical despite different names*

### Comparing `repytah-0.1.0/docs/pictures/find_all_repeats3.png` & `repytah-0.1.1/docs/pictures/find_all_repeats3.png`

 * *Files identical despite different names*

### Comparing `repytah-0.1.0/docs/pictures/find_complete_list_visualization.png` & `repytah-0.1.1/docs/pictures/find_complete_list_visualization.png`

 * *Files identical despite different names*

### Comparing `repytah-0.1.0/docs/pictures/find_initial_repeats.png` & `repytah-0.1.1/docs/pictures/find_initial_repeats.png`

 * *Files identical despite different names*

### Comparing `repytah-0.1.0/docs/pictures/function_flow_step.png` & `repytah-0.1.1/docs/pictures/function_flow_step.png`

 * *Files identical despite different names*

### Comparing `repytah-0.1.0/docs/pictures/function_flow_steps.PNG` & `repytah-0.1.1/docs/pictures/function_flow_steps.PNG`

 * *Files identical despite different names*

### Comparing `repytah-0.1.0/docs/pictures/function_pipeline.jpg` & `repytah-0.1.1/docs/pictures/function_pipeline.jpg`

 * *Files identical despite different names*

### Comparing `repytah-0.1.0/docs/pictures/num_of_parts.png` & `repytah-0.1.1/docs/pictures/num_of_parts.png`

 * *Files identical despite different names*

### Comparing `repytah-0.1.0/docs/pictures/score.jpg` & `repytah-0.1.1/docs/pictures/score.jpg`

 * *Files identical despite different names*

### Comparing `repytah-0.1.0/docs/pictures/score1.jpg` & `repytah-0.1.1/docs/pictures/score1.jpg`

 * *Files identical despite different names*

### Comparing `repytah-0.1.0/docs/pictures/score2.jpg` & `repytah-0.1.1/docs/pictures/score2.jpg`

 * *Files identical despite different names*

### Comparing `repytah-0.1.0/docs/quick_start.ipynb` & `repytah-0.1.1/docs/quick_start.ipynb`

 * *Files identical despite different names*

### Comparing `repytah-0.1.0/docs/recommended_installation.rst` & `repytah-0.1.1/docs/recommended_installation.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Recommended Installation
+Installing from `conda` package-manager or from `pip`
 ============
 
 Anaconda
 ~~~~~~~~
 
 The safest way to install repytah is through ``conda``.
 In terminal, navigate to the directory that contains environment.yml and execute::
```

### Comparing `repytah-0.1.0/docs/search_doc.rst` & `repytah-0.1.1/docs/search_doc.rst`

 * *Files identical despite different names*

### Comparing `repytah-0.1.0/docs/search_vignette.ipynb` & `repytah-0.1.1/docs/search_vignette.ipynb`

 * *Files identical despite different names*

### Comparing `repytah-0.1.0/docs/transform.rst` & `repytah-0.1.1/docs/transform.rst`

 * *Files identical despite different names*

### Comparing `repytah-0.1.0/docs/transform_vignette.ipynb` & `repytah-0.1.1/docs/transform_vignette.ipynb`

 * *Files identical despite different names*

### Comparing `repytah-0.1.0/docs/utilities.rst` & `repytah-0.1.1/docs/utilities.rst`

 * *Files identical despite different names*

### Comparing `repytah-0.1.0/docs/utilities_vignette.ipynb` & `repytah-0.1.1/docs/utilities_vignette.ipynb`

 * *Files identical despite different names*

### Comparing `repytah-0.1.0/repytah/assemble.py` & `repytah-0.1.1/repytah/assemble.py`

 * *Files identical despite different names*

### Comparing `repytah-0.1.0/repytah/data/input.csv` & `repytah-0.1.1/repytah/data/input.csv`

 * *Files identical despite different names*

### Comparing `repytah-0.1.0/repytah/data/mazurka30-1.csv` & `repytah-0.1.1/repytah/data/mazurka30-1.csv`

 * *Files identical despite different names*

### Comparing `repytah-0.1.0/repytah/data/mazurka30-3.csv` & `repytah-0.1.1/repytah/data/mazurka30-3.csv`

 * *Files identical despite different names*

### Comparing `repytah-0.1.0/repytah/example.py` & `repytah-0.1.1/repytah/example.py`

 * *Files identical despite different names*

### Comparing `repytah-0.1.0/repytah/search.py` & `repytah-0.1.1/repytah/search.py`

 * *Files identical despite different names*

### Comparing `repytah-0.1.0/repytah/transform.py` & `repytah-0.1.1/repytah/transform.py`

 * *Files identical despite different names*

### Comparing `repytah-0.1.0/repytah/utilities.py` & `repytah-0.1.1/repytah/utilities.py`

 * *Files identical despite different names*

### Comparing `repytah-0.1.0/repytah/version.py` & `repytah-0.1.1/repytah/version.py`

 * *Files identical despite different names*

### Comparing `repytah-0.1.0/repytah.egg-info/SOURCES.txt` & `repytah-0.1.1/repytah.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -106,14 +106,15 @@
 repytah/utilities.py
 repytah/version.py
 repytah.egg-info/PKG-INFO
 repytah.egg-info/SOURCES.txt
 repytah.egg-info/dependency_links.txt
 repytah.egg-info/requires.txt
 repytah.egg-info/top_level.txt
+repytah/data/README.md
 repytah/data/input.csv
 repytah/data/mazurka30-1.csv
 repytah/data/mazurka30-3.csv
 test/test_assemble.py
 test/test_example.py
 test/test_search.py
 test/test_transform.py
```

### Comparing `repytah-0.1.0/setup.py` & `repytah-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='repytah',
-    version='0.1.0',
+    version='0.1.1',
     description='Python package for building Aligned Hierarchies for sequential data streams',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/smith-tinkerlab/repytah',
     author='Smith Tinker Lab, Katherine M. Kinnaird (PI)',
     author_email='tinkerlab@smith.edu',
     packages=find_packages(),
```

### Comparing `repytah-0.1.0/test/test_assemble.py` & `repytah-0.1.1/test/test_assemble.py`

 * *Files identical despite different names*

### Comparing `repytah-0.1.0/test/test_example.py` & `repytah-0.1.1/test/test_example.py`

 * *Files identical despite different names*

### Comparing `repytah-0.1.0/test/test_search.py` & `repytah-0.1.1/test/test_search.py`

 * *Files identical despite different names*

### Comparing `repytah-0.1.0/test/test_transform.py` & `repytah-0.1.1/test/test_transform.py`

 * *Files identical despite different names*

### Comparing `repytah-0.1.0/test/test_utilities.py` & `repytah-0.1.1/test/test_utilities.py`

 * *Files identical despite different names*

