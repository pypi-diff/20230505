# Comparing `tmp/cercis-0.1.1.tar.gz` & `tmp/cercis-0.1.2.tar.gz`

## Comparing `cercis-0.1.1.tar` & `cercis-0.1.2.tar`

### file list

```diff
@@ -1,291 +1,297 @@
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 cercis-0.1.1/.coveragerc
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 cercis-0.1.1/.flake8
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 cercis-0.1.1/.git_archival.txt
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 cercis-0.1.1/.gitattributes
--rw-r--r--   0        0        0     1276 2020-02-02 00:00:00.000000 cercis-0.1.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 cercis-0.1.1/.pre-commit-hooks.yaml
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 cercis-0.1.1/.prettierrc.yaml
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 cercis-0.1.1/.readthedocs.yaml
--rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 cercis-0.1.1/CHANGES.md
--rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 cercis-0.1.1/CONTRIBUTING.md
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 cercis-0.1.1/Dockerfile
--rw-r--r--   0        0        0     6688 2020-02-02 00:00:00.000000 cercis-0.1.1/README.md
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 cercis-0.1.1/SECURITY.md
--rw-r--r--   0        0        0     1540 2020-02-02 00:00:00.000000 cercis-0.1.1/action.yml
--rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 cercis-0.1.1/mypy.ini
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 cercis-0.1.1/test_requirements.txt
--rw-r--r--   0        0        0     2972 2020-02-02 00:00:00.000000 cercis-0.1.1/tox.ini
--rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 cercis-0.1.1/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 cercis-0.1.1/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 cercis-0.1.1/.github/dependabot.yml
--rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 cercis-0.1.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 cercis-0.1.1/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 cercis-0.1.1/.github/ISSUE_TEMPLATE/docs-issue.md
--rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 cercis-0.1.1/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 cercis-0.1.1/.github/ISSUE_TEMPLATE/style_issue.md
--rw-r--r--   0        0        0     1894 2020-02-02 00:00:00.000000 cercis-0.1.1/.github/workflows/docker.yml
--rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 cercis-0.1.1/.github/workflows/fuzz.yml
--rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 cercis-0.1.1/.github/workflows/lint.yml
--rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 cercis-0.1.1/.github/workflows/python-package.yml
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 cercis-0.1.1/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0     2998 2020-02-02 00:00:00.000000 cercis-0.1.1/.github/workflows/test.yml
--rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 cercis-0.1.1/.github/workflows/upload_binary.yml
--rw-r--r--   0        0        0     2245 2020-02-02 00:00:00.000000 cercis-0.1.1/action/main.py
--rw-r--r--   0        0        0     7597 2020-02-02 00:00:00.000000 cercis-0.1.1/autoload/black.vim
--rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 cercis-0.1.1/gallery/Dockerfile
--rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 cercis-0.1.1/gallery/README.md
--rwxr-xr-x   0        0        0     9123 2020-02-02 00:00:00.000000 cercis-0.1.1/gallery/gallery.py
--rw-r--r--   0        0        0     2176 2020-02-02 00:00:00.000000 cercis-0.1.1/plugin/black.vim
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.1/scripts/__init__.py
--rw-r--r--   0        0        0     8650 2020-02-02 00:00:00.000000 cercis-0.1.1/scripts/diff_shades_gha_helper.py
--rw-r--r--   0        0        0     3527 2020-02-02 00:00:00.000000 cercis-0.1.1/scripts/fuzz.py
--rw-r--r--   0        0        0     2458 2020-02-02 00:00:00.000000 cercis-0.1.1/scripts/make_width_table.py
--rwxr-xr-x   0        0        0     2993 2020-02-02 00:00:00.000000 cercis-0.1.1/scripts/migrate-black.py
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 cercis-0.1.1/src/_cercis_version.py
--rw-r--r--   0        0        0     8100 2020-02-02 00:00:00.000000 cercis-0.1.1/src/blackd/__init__.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cercis-0.1.1/src/blackd/__main__.py
--rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 cercis-0.1.1/src/blackd/middlewares.py
--rw-r--r--   0        0        0    11278 2020-02-02 00:00:00.000000 cercis-0.1.1/src/blib2to3/Grammar.txt
--rw-r--r--   0        0        0    12762 2020-02-02 00:00:00.000000 cercis-0.1.1/src/blib2to3/LICENSE
--rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 cercis-0.1.1/src/blib2to3/PatternGrammar.txt
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 cercis-0.1.1/src/blib2to3/README
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 cercis-0.1.1/src/blib2to3/__init__.py
--rw-r--r--   0        0        0     5732 2020-02-02 00:00:00.000000 cercis-0.1.1/src/blib2to3/pygram.py
--rw-r--r--   0        0        0    32612 2020-02-02 00:00:00.000000 cercis-0.1.1/src/blib2to3/pytree.py
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 cercis-0.1.1/src/blib2to3/pgen2/__init__.py
--rw-r--r--   0        0        0     9607 2020-02-02 00:00:00.000000 cercis-0.1.1/src/blib2to3/pgen2/conv.py
--rw-r--r--   0        0        0    10671 2020-02-02 00:00:00.000000 cercis-0.1.1/src/blib2to3/pgen2/driver.py
--rw-r--r--   0        0        0     6873 2020-02-02 00:00:00.000000 cercis-0.1.1/src/blib2to3/pgen2/grammar.py
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 cercis-0.1.1/src/blib2to3/pgen2/literals.py
--rw-r--r--   0        0        0    14859 2020-02-02 00:00:00.000000 cercis-0.1.1/src/blib2to3/pgen2/parse.py
--rw-r--r--   0        0        0    15491 2020-02-02 00:00:00.000000 cercis-0.1.1/src/blib2to3/pgen2/pgen.py
--rw-r--r--   0        0        0     1919 2020-02-02 00:00:00.000000 cercis-0.1.1/src/blib2to3/pgen2/token.py
--rw-r--r--   0        0        0    22847 2020-02-02 00:00:00.000000 cercis-0.1.1/src/blib2to3/pgen2/tokenize.py
--rw-r--r--   0        0        0    47673 2020-02-02 00:00:00.000000 cercis-0.1.1/src/cercis/__init__.py
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 cercis-0.1.1/src/cercis/__main__.py
--rw-r--r--   0        0        0    10871 2020-02-02 00:00:00.000000 cercis-0.1.1/src/cercis/_width_table.py
--rw-r--r--   0        0        0    12274 2020-02-02 00:00:00.000000 cercis-0.1.1/src/cercis/brackets.py
--rw-r--r--   0        0        0     2952 2020-02-02 00:00:00.000000 cercis-0.1.1/src/cercis/cache.py
--rw-r--r--   0        0        0    12797 2020-02-02 00:00:00.000000 cercis-0.1.1/src/cercis/comments.py
--rw-r--r--   0        0        0     6343 2020-02-02 00:00:00.000000 cercis-0.1.1/src/cercis/concurrency.py
--rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 cercis-0.1.1/src/cercis/const.py
--rw-r--r--   0        0        0     1597 2020-02-02 00:00:00.000000 cercis-0.1.1/src/cercis/debug.py
--rw-r--r--   0        0        0    13538 2020-02-02 00:00:00.000000 cercis-0.1.1/src/cercis/files.py
--rw-r--r--   0        0        0    13506 2020-02-02 00:00:00.000000 cercis-0.1.1/src/cercis/handle_ipynb_magics.py
--rw-r--r--   0        0        0    61129 2020-02-02 00:00:00.000000 cercis-0.1.1/src/cercis/linegen.py
--rw-r--r--   0        0        0    36582 2020-02-02 00:00:00.000000 cercis-0.1.1/src/cercis/lines.py
--rw-r--r--   0        0        0     7399 2020-02-02 00:00:00.000000 cercis-0.1.1/src/cercis/mode.py
--rw-r--r--   0        0        0    25731 2020-02-02 00:00:00.000000 cercis-0.1.1/src/cercis/nodes.py
--rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 cercis-0.1.1/src/cercis/numerics.py
--rw-r--r--   0        0        0     3486 2020-02-02 00:00:00.000000 cercis-0.1.1/src/cercis/output.py
--rw-r--r--   0        0        0    10164 2020-02-02 00:00:00.000000 cercis-0.1.1/src/cercis/parsing.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.1/src/cercis/py.typed
--rw-r--r--   0        0        0     3452 2020-02-02 00:00:00.000000 cercis-0.1.1/src/cercis/report.py
--rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 cercis-0.1.1/src/cercis/rusty.py
--rw-r--r--   0        0        0    14304 2020-02-02 00:00:00.000000 cercis-0.1.1/src/cercis/strings.py
--rw-r--r--   0        0        0    91688 2020-02-02 00:00:00.000000 cercis-0.1.1/src/cercis/trans.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/__init__.py
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/conftest.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/empty.toml
--rw-r--r--   0        0        0     4133 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/optional.py
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/test.toml
--rw-r--r--   0        0        0   100658 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/test_black.py
--rw-r--r--   0        0        0     9188 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/test_blackd.py
--rw-r--r--   0        0        0     8227 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/test_format.py
--rw-r--r--   0        0        0    16290 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/test_ipynb.py
--rw-r--r--   0        0        0     1292 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/test_no_ipynb.py
--rw-r--r--   0        0        0     2267 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/test_trans.py
--rw-r--r--   0        0        0     6959 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/util.py
--rw-r--r--   0        0        0     4160 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/conditional_expression.py
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/empty_pyproject.toml
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/configurable_cases/func_def_extra_indent.py
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/configurable_cases/func_def_no_extra_indent.py
--rw-r--r--   0        0        0     7702 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/configurable_cases/single_quote/docstring.py
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/configurable_cases/single_quote/docstring_no_extra_empty_line_before_eof.py
--rw-r--r--   0        0        0     3513 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/configurable_cases/single_quote/docstring_preview.py
--rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/configurable_cases/single_quote/more_quotes.py
--rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/configurable_cases/single_quote/string_prefixes.py
--rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/configurable_cases/single_quote/torture.py
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/fast/pep_572_do_not_remove_parens.py
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/gitignore_used_on_multiple_sources/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/gitignore_used_on_multiple_sources/dir1/a.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/gitignore_used_on_multiple_sources/dir1/b.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/gitignore_used_on_multiple_sources/dir2/a.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/gitignore_used_on_multiple_sources/dir2/b.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/ignore_subfolders_gitignore_tests/a.py
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/ignore_subfolders_gitignore_tests/subdir/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/ignore_subfolders_gitignore_tests/subdir/b.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/ignore_subfolders_gitignore_tests/subdir/subdir/c.py
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/include_exclude_tests/.gitignore
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/include_exclude_tests/pyproject.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/include_exclude_tests/b/.definitely_exclude/a.pie
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/include_exclude_tests/b/.definitely_exclude/a.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/include_exclude_tests/b/.definitely_exclude/a.pyi
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/include_exclude_tests/b/dont_exclude/a.pie
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/include_exclude_tests/b/dont_exclude/a.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/include_exclude_tests/b/dont_exclude/a.pyi
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/include_exclude_tests/b/exclude/a.pie
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/include_exclude_tests/b/exclude/a.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/include_exclude_tests/b/exclude/a.pyi
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/invalid_gitignore_tests/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/invalid_gitignore_tests/a.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/invalid_gitignore_tests/pyproject.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/invalid_nested_gitignore_tests/a.py
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/invalid_nested_gitignore_tests/pyproject.toml
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/invalid_nested_gitignore_tests/a/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/invalid_nested_gitignore_tests/a/a.py
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/jupyter/non_python_notebook.ipynb
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/jupyter/notebook_empty_metadata.ipynb
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/jupyter/notebook_no_trailing_newline.ipynb
--rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/jupyter/notebook_trailing_newline.ipynb
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/jupyter/notebook_which_cant_be_parsed.ipynb
--rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/jupyter/notebook_without_changes.ipynb
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/miscellaneous/async_as_identifier.py
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/miscellaneous/blackd_diff.diff
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/miscellaneous/blackd_diff.py
--rw-r--r--   0        0        0    15604 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/miscellaneous/debug_visitor.out
--rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/miscellaneous/debug_visitor.py
--rw-r--r--   0        0        0     1774 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/miscellaneous/decorators.py
--rw-r--r--   0        0        0     3601 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/miscellaneous/docstring_no_string_normalization.py
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/miscellaneous/docstring_preview_no_string_normalization.py
--rw-r--r--   0        0        0    15711 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/miscellaneous/expression_skip_magic_trailing_comma.diff
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/miscellaneous/force_py36.py
--rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/miscellaneous/force_pyi.py
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/miscellaneous/invalid_header.py
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/miscellaneous/linelength6.py
--rw-r--r--   0        0        0    11583 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/miscellaneous/long_strings_flag_disabled.py
--rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/miscellaneous/missing_final_newline.diff
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/miscellaneous/missing_final_newline.py
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/miscellaneous/nested_class_stub.pyi
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/miscellaneous/pattern_matching_invalid.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/miscellaneous/power_op_newline.py
--rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/miscellaneous/python2_detection.py
--rw-r--r--   0        0        0     2361 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/miscellaneous/string_quotes.py
--rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/miscellaneous/stub.pyi
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/nested_gitignore_tests/pyproject.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/nested_gitignore_tests/x.py
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/nested_gitignore_tests/root/.gitignore
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/nested_gitignore_tests/root/a.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/nested_gitignore_tests/root/b.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/nested_gitignore_tests/root/c.py
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/nested_gitignore_tests/root/child/.gitignore
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/nested_gitignore_tests/root/child/a.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/nested_gitignore_tests/root/child/b.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/nested_gitignore_tests/root/child/c.py
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/preview/async_stmts.py
--rw-r--r--   0        0        0     4107 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/preview/cantfit.py
--rw-r--r--   0        0        0     8294 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/preview/comments7.py
--rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/preview/format_unicode_escape_seq.py
--rw-r--r--   0        0        0     2784 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/preview/long_dict_values.py
--rw-r--r--   0        0        0    33216 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/preview/long_strings.py
--rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/preview/long_strings__east_asian_width.py
--rw-r--r--   0        0        0     6536 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/preview/long_strings__edge_case.py
--rw-r--r--   0        0        0    45897 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/preview/long_strings__regression.py
--rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/preview/long_strings__type_annotations.py
--rw-r--r--   0        0        0     7207 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/preview/multiline_strings.py
--rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/preview/percent_precedence.py
--rw-r--r--   0        0        0     2525 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/preview/prefer_rhs_split.py
--rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/preview/return_annotation_brackets_string.py
--rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/preview/trailing_comma.py
--rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/preview_context_managers/targeting_py38.py
--rw-r--r--   0        0        0     3361 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/preview_context_managers/targeting_py39.py
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/preview_context_managers/auto_detect/features_3_10.py
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/preview_context_managers/auto_detect/features_3_11.py
--rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/preview_context_managers/auto_detect/features_3_8.py
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/preview_context_managers/auto_detect/features_3_9.py
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/project_metadata/both_pyproject.toml
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/project_metadata/neither_pyproject.toml
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/project_metadata/only_black_pyproject.toml
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/project_metadata/only_metadata_pyproject.toml
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/py_310/parenthesized_context_managers.py
--rw-r--r--   0        0        0     2668 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/py_310/pattern_matching_complex.py
--rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/py_310/pattern_matching_extras.py
--rw-r--r--   0        0        0     3066 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/py_310/pattern_matching_generic.py
--rw-r--r--   0        0        0     2641 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/py_310/pattern_matching_simple.py
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/py_310/pattern_matching_style.py
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/py_310/pep_572_py310.py
--rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/py_310/remove_newline_after_match.py
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/py_310/starred_for_target.py
--rw-r--r--   0        0        0     2114 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/py_311/pep_646.py
--rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/py_311/pep_654.py
--rw-r--r--   0        0        0     2033 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/py_311/pep_654_style.py
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/py_36/numeric_literals.py
--rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/py_36/numeric_literals_skip_underscores.py
--rw-r--r--   0        0        0     1199 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/py_37/python37.py
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/py_38/pep_570.py
--rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/py_38/pep_572.py
--rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/py_38/pep_572_remove_parens.py
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/py_38/python38.py
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/py_39/pep_572_py39.py
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/py_39/python39.py
--rw-r--r--   0        0        0     2575 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/py_39/remove_with_brackets.py
--rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/simple_cases/attribute_access_on_number_literals.py
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/simple_cases/beginning_backslash.py
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/simple_cases/bracketmatch.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/simple_cases/class_blank_parentheses.py
--rw-r--r--   0        0        0     4318 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/simple_cases/class_methods_new_line.py
--rw-r--r--   0        0        0     3294 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/simple_cases/collections.py
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/simple_cases/comment_after_escaped_newline.py
--rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/simple_cases/comments.py
--rw-r--r--   0        0        0     7639 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/simple_cases/comments2.py
--rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/simple_cases/comments3.py
--rw-r--r--   0        0        0     3536 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/simple_cases/comments4.py
--rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/simple_cases/comments5.py
--rw-r--r--   0        0        0     2567 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/simple_cases/comments6.py
--rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/simple_cases/comments8.py
--rw-r--r--   0        0        0     5279 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/simple_cases/comments9.py
--rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/simple_cases/comments_non_breaking_space.py
--rw-r--r--   0        0        0     5597 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/simple_cases/composition.py
--rw-r--r--   0        0        0    11198 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/simple_cases/composition_no_trailing_comma.py
--rw-r--r--   0        0        0     7699 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/simple_cases/docstring.py
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/simple_cases/docstring_no_extra_empty_line_before_eof.py
--rw-r--r--   0        0        0     3513 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/simple_cases/docstring_preview.py
--rw-r--r--   0        0        0     4596 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/simple_cases/empty_lines.py
--rw-r--r--   0        0        0    15801 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/simple_cases/expression.diff
--rw-r--r--   0        0        0    18624 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/simple_cases/expression.py
--rw-r--r--   0        0        0     9681 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/simple_cases/fmtonoff.py
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/simple_cases/fmtonoff2.py
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/simple_cases/fmtonoff3.py
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/simple_cases/fmtonoff4.py
--rw-r--r--   0        0        0     3627 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/simple_cases/fmtonoff5.py
--rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/simple_cases/fmtpass_imports.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/simple_cases/fmtskip.py
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/simple_cases/fmtskip2.py
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/simple_cases/fmtskip3.py
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/simple_cases/fmtskip4.py
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/simple_cases/fmtskip5.py
--rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/simple_cases/fmtskip6.py
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/simple_cases/fmtskip7.py
--rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/simple_cases/fmtskip8.py
--rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/simple_cases/fstring.py
--rw-r--r--   0        0        0     6482 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/simple_cases/function.py
--rw-r--r--   0        0        0     2427 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/simple_cases/function2.py
--rw-r--r--   0        0        0     3657 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/simple_cases/function_trailing_comma.py
--rw-r--r--   0        0        0     2542 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/simple_cases/import_spacing.py
--rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/simple_cases/one_element_subscript.py
--rw-r--r--   0        0        0     3359 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/simple_cases/power_op_spacing.py
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/simple_cases/prefer_rhs_split_reformatted.py
--rw-r--r--   0        0        0     3205 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/simple_cases/remove_await_parens.py
--rw-r--r--   0        0        0     2025 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/simple_cases/remove_except_parens.py
--rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/simple_cases/remove_for_brackets.py
--rw-r--r--   0        0        0     3351 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/simple_cases/remove_newline_after_code_block_open.py
--rw-r--r--   0        0        0     3493 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/simple_cases/remove_parens.py
--rw-r--r--   0        0        0     5141 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/simple_cases/return_annotation_brackets.py
--rw-r--r--   0        0        0     1398 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/simple_cases/skip_magic_trailing_comma.py
--rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/simple_cases/slices.py
--rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/simple_cases/string_prefixes.py
--rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/simple_cases/torture.py
--rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/simple_cases/trailing_comma_optional_parens1.py
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/simple_cases/trailing_comma_optional_parens2.py
--rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/simple_cases/trailing_comma_optional_parens3.py
--rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/simple_cases/trailing_commas_in_leading_parts.py
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/simple_cases/tricky_unicode_symbols.py
--rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/simple_cases/tupleassign.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/simple_cases/whitespace.py
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 cercis-0.1.1/tests/data/type_comments/type_comment_syntax_error.py
--rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 cercis-0.1.1/.gitignore
--rw-r--r--   0        0        0     8043 2020-02-02 00:00:00.000000 cercis-0.1.1/AUTHORS.md
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 cercis-0.1.1/LICENSE
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 cercis-0.1.1/LICENSE_ORIGINAL
--rw-r--r--   0        0        0     6940 2020-02-02 00:00:00.000000 cercis-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     9414 2020-02-02 00:00:00.000000 cercis-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 cercis-0.1.2/.coveragerc
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 cercis-0.1.2/.flake8
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 cercis-0.1.2/.git_archival.txt
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 cercis-0.1.2/.gitattributes
+-rw-r--r--   0        0        0     1276 2020-02-02 00:00:00.000000 cercis-0.1.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 cercis-0.1.2/.pre-commit-hooks.yaml
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 cercis-0.1.2/.prettierrc.yaml
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 cercis-0.1.2/.readthedocs.yaml
+-rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 cercis-0.1.2/CHANGES.md
+-rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 cercis-0.1.2/CONTRIBUTING.md
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 cercis-0.1.2/Dockerfile
+-rw-r--r--   0        0        0     8193 2020-02-02 00:00:00.000000 cercis-0.1.2/README.md
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 cercis-0.1.2/SECURITY.md
+-rw-r--r--   0        0        0     1540 2020-02-02 00:00:00.000000 cercis-0.1.2/action.yml
+-rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 cercis-0.1.2/mypy.ini
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 cercis-0.1.2/test_requirements.txt
+-rw-r--r--   0        0        0     2972 2020-02-02 00:00:00.000000 cercis-0.1.2/tox.ini
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 cercis-0.1.2/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 cercis-0.1.2/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 cercis-0.1.2/.github/dependabot.yml
+-rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 cercis-0.1.2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 cercis-0.1.2/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 cercis-0.1.2/.github/ISSUE_TEMPLATE/docs-issue.md
+-rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 cercis-0.1.2/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      646 2020-02-02 00:00:00.000000 cercis-0.1.2/.github/ISSUE_TEMPLATE/style_issue.md
+-rw-r--r--   0        0        0     1894 2020-02-02 00:00:00.000000 cercis-0.1.2/.github/workflows/docker.yml
+-rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 cercis-0.1.2/.github/workflows/fuzz.yml
+-rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 cercis-0.1.2/.github/workflows/lint.yml
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 cercis-0.1.2/.github/workflows/python-package.yml
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 cercis-0.1.2/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0     2998 2020-02-02 00:00:00.000000 cercis-0.1.2/.github/workflows/test.yml
+-rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 cercis-0.1.2/.github/workflows/upload_binary.yml
+-rw-r--r--   0        0        0     2245 2020-02-02 00:00:00.000000 cercis-0.1.2/action/main.py
+-rw-r--r--   0        0        0     7597 2020-02-02 00:00:00.000000 cercis-0.1.2/autoload/black.vim
+-rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 cercis-0.1.2/gallery/Dockerfile
+-rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 cercis-0.1.2/gallery/README.md
+-rwxr-xr-x   0        0        0     9123 2020-02-02 00:00:00.000000 cercis-0.1.2/gallery/gallery.py
+-rw-r--r--   0        0        0     2176 2020-02-02 00:00:00.000000 cercis-0.1.2/plugin/black.vim
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.2/scripts/__init__.py
+-rw-r--r--   0        0        0     8650 2020-02-02 00:00:00.000000 cercis-0.1.2/scripts/diff_shades_gha_helper.py
+-rw-r--r--   0        0        0     3527 2020-02-02 00:00:00.000000 cercis-0.1.2/scripts/fuzz.py
+-rw-r--r--   0        0        0     2458 2020-02-02 00:00:00.000000 cercis-0.1.2/scripts/make_width_table.py
+-rwxr-xr-x   0        0        0     2993 2020-02-02 00:00:00.000000 cercis-0.1.2/scripts/migrate-black.py
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 cercis-0.1.2/src/_cercis_version.py
+-rw-r--r--   0        0        0     8100 2020-02-02 00:00:00.000000 cercis-0.1.2/src/blackd/__init__.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cercis-0.1.2/src/blackd/__main__.py
+-rw-r--r--   0        0        0     1585 2020-02-02 00:00:00.000000 cercis-0.1.2/src/blackd/middlewares.py
+-rw-r--r--   0        0        0    11278 2020-02-02 00:00:00.000000 cercis-0.1.2/src/blib2to3/Grammar.txt
+-rw-r--r--   0        0        0    12762 2020-02-02 00:00:00.000000 cercis-0.1.2/src/blib2to3/LICENSE
+-rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 cercis-0.1.2/src/blib2to3/PatternGrammar.txt
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 cercis-0.1.2/src/blib2to3/README
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 cercis-0.1.2/src/blib2to3/__init__.py
+-rw-r--r--   0        0        0     5732 2020-02-02 00:00:00.000000 cercis-0.1.2/src/blib2to3/pygram.py
+-rw-r--r--   0        0        0    32612 2020-02-02 00:00:00.000000 cercis-0.1.2/src/blib2to3/pytree.py
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 cercis-0.1.2/src/blib2to3/pgen2/__init__.py
+-rw-r--r--   0        0        0     9607 2020-02-02 00:00:00.000000 cercis-0.1.2/src/blib2to3/pgen2/conv.py
+-rw-r--r--   0        0        0    10671 2020-02-02 00:00:00.000000 cercis-0.1.2/src/blib2to3/pgen2/driver.py
+-rw-r--r--   0        0        0     6873 2020-02-02 00:00:00.000000 cercis-0.1.2/src/blib2to3/pgen2/grammar.py
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 cercis-0.1.2/src/blib2to3/pgen2/literals.py
+-rw-r--r--   0        0        0    14859 2020-02-02 00:00:00.000000 cercis-0.1.2/src/blib2to3/pgen2/parse.py
+-rw-r--r--   0        0        0    15491 2020-02-02 00:00:00.000000 cercis-0.1.2/src/blib2to3/pgen2/pgen.py
+-rw-r--r--   0        0        0     1919 2020-02-02 00:00:00.000000 cercis-0.1.2/src/blib2to3/pgen2/token.py
+-rw-r--r--   0        0        0    23120 2020-02-02 00:00:00.000000 cercis-0.1.2/src/blib2to3/pgen2/tokenize.py
+-rw-r--r--   0        0        0    48202 2020-02-02 00:00:00.000000 cercis-0.1.2/src/cercis/__init__.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 cercis-0.1.2/src/cercis/__main__.py
+-rw-r--r--   0        0        0    10871 2020-02-02 00:00:00.000000 cercis-0.1.2/src/cercis/_width_table.py
+-rw-r--r--   0        0        0    12274 2020-02-02 00:00:00.000000 cercis-0.1.2/src/cercis/brackets.py
+-rw-r--r--   0        0        0     2952 2020-02-02 00:00:00.000000 cercis-0.1.2/src/cercis/cache.py
+-rw-r--r--   0        0        0    12797 2020-02-02 00:00:00.000000 cercis-0.1.2/src/cercis/comments.py
+-rw-r--r--   0        0        0     6343 2020-02-02 00:00:00.000000 cercis-0.1.2/src/cercis/concurrency.py
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 cercis-0.1.2/src/cercis/const.py
+-rw-r--r--   0        0        0     1597 2020-02-02 00:00:00.000000 cercis-0.1.2/src/cercis/debug.py
+-rw-r--r--   0        0        0    13538 2020-02-02 00:00:00.000000 cercis-0.1.2/src/cercis/files.py
+-rw-r--r--   0        0        0    13506 2020-02-02 00:00:00.000000 cercis-0.1.2/src/cercis/handle_ipynb_magics.py
+-rw-r--r--   0        0        0    61366 2020-02-02 00:00:00.000000 cercis-0.1.2/src/cercis/linegen.py
+-rw-r--r--   0        0        0    36582 2020-02-02 00:00:00.000000 cercis-0.1.2/src/cercis/lines.py
+-rw-r--r--   0        0        0     7513 2020-02-02 00:00:00.000000 cercis-0.1.2/src/cercis/mode.py
+-rw-r--r--   0        0        0    25731 2020-02-02 00:00:00.000000 cercis-0.1.2/src/cercis/nodes.py
+-rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 cercis-0.1.2/src/cercis/numerics.py
+-rw-r--r--   0        0        0     3486 2020-02-02 00:00:00.000000 cercis-0.1.2/src/cercis/output.py
+-rw-r--r--   0        0        0    10164 2020-02-02 00:00:00.000000 cercis-0.1.2/src/cercis/parsing.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.2/src/cercis/py.typed
+-rw-r--r--   0        0        0     3452 2020-02-02 00:00:00.000000 cercis-0.1.2/src/cercis/report.py
+-rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 cercis-0.1.2/src/cercis/rusty.py
+-rw-r--r--   0        0        0    14304 2020-02-02 00:00:00.000000 cercis-0.1.2/src/cercis/strings.py
+-rw-r--r--   0        0        0    91688 2020-02-02 00:00:00.000000 cercis-0.1.2/src/cercis/trans.py
+-rw-r--r--   0        0        0     2327 2020-02-02 00:00:00.000000 cercis-0.1.2/src/cercis/utils_line_wrapping.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/__init__.py
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/conftest.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/empty.toml
+-rw-r--r--   0        0        0     4133 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/optional.py
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/test.toml
+-rw-r--r--   0        0        0   100658 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/test_black.py
+-rw-r--r--   0        0        0     9188 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/test_blackd.py
+-rw-r--r--   0        0        0     9000 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/test_format.py
+-rw-r--r--   0        0        0    16377 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/test_ipynb.py
+-rw-r--r--   0        0        0     1292 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/test_no_ipynb.py
+-rw-r--r--   0        0        0     2267 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/test_trans.py
+-rw-r--r--   0        0        0     2546 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/test_utils_line_wrapping.py
+-rw-r--r--   0        0        0     7023 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/util.py
+-rw-r--r--   0        0        0     4160 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/conditional_expression.py
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/empty_pyproject.toml
+-rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/configurable_cases/func_def_indent/func_def_extra_indent.py
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/configurable_cases/func_def_indent/func_def_no_extra_indent.py
+-rw-r--r--   0        0        0    11583 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/configurable_cases/line_with_long_string/long_strings_flag_disabled__Black_default.py
+-rw-r--r--   0        0        0    23081 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/configurable_cases/line_with_long_string/long_strings_flag_disabled__Cercis_default.py
+-rw-r--r--   0        0        0     6138 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/configurable_cases/line_with_long_string/test_cases__Black_default.py
+-rw-r--r--   0        0        0     6024 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/configurable_cases/line_with_long_string/test_cases__Cercis_default.py
+-rw-r--r--   0        0        0     7702 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/configurable_cases/single_quote/docstring.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/configurable_cases/single_quote/docstring_no_extra_empty_line_before_eof.py
+-rw-r--r--   0        0        0     3513 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/configurable_cases/single_quote/docstring_preview.py
+-rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/configurable_cases/single_quote/more_quotes.py
+-rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/configurable_cases/single_quote/string_prefixes.py
+-rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/configurable_cases/single_quote/torture.py
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/fast/pep_572_do_not_remove_parens.py
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/gitignore_used_on_multiple_sources/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/gitignore_used_on_multiple_sources/dir1/a.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/gitignore_used_on_multiple_sources/dir1/b.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/gitignore_used_on_multiple_sources/dir2/a.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/gitignore_used_on_multiple_sources/dir2/b.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/ignore_subfolders_gitignore_tests/a.py
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/ignore_subfolders_gitignore_tests/subdir/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/ignore_subfolders_gitignore_tests/subdir/b.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/ignore_subfolders_gitignore_tests/subdir/subdir/c.py
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/include_exclude_tests/.gitignore
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/include_exclude_tests/pyproject.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/include_exclude_tests/b/.definitely_exclude/a.pie
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/include_exclude_tests/b/.definitely_exclude/a.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/include_exclude_tests/b/.definitely_exclude/a.pyi
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/include_exclude_tests/b/dont_exclude/a.pie
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/include_exclude_tests/b/dont_exclude/a.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/include_exclude_tests/b/dont_exclude/a.pyi
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/include_exclude_tests/b/exclude/a.pie
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/include_exclude_tests/b/exclude/a.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/include_exclude_tests/b/exclude/a.pyi
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/invalid_gitignore_tests/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/invalid_gitignore_tests/a.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/invalid_gitignore_tests/pyproject.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/invalid_nested_gitignore_tests/a.py
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/invalid_nested_gitignore_tests/pyproject.toml
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/invalid_nested_gitignore_tests/a/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/invalid_nested_gitignore_tests/a/a.py
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/jupyter/non_python_notebook.ipynb
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/jupyter/notebook_empty_metadata.ipynb
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/jupyter/notebook_no_trailing_newline.ipynb
+-rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/jupyter/notebook_trailing_newline.ipynb
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/jupyter/notebook_which_cant_be_parsed.ipynb
+-rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/jupyter/notebook_without_changes.ipynb
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/miscellaneous/async_as_identifier.py
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/miscellaneous/blackd_diff.diff
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/miscellaneous/blackd_diff.py
+-rw-r--r--   0        0        0    15604 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/miscellaneous/debug_visitor.out
+-rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/miscellaneous/debug_visitor.py
+-rw-r--r--   0        0        0     1774 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/miscellaneous/decorators.py
+-rw-r--r--   0        0        0     3601 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/miscellaneous/docstring_no_string_normalization.py
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/miscellaneous/docstring_preview_no_string_normalization.py
+-rw-r--r--   0        0        0    15711 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/miscellaneous/expression_skip_magic_trailing_comma.diff
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/miscellaneous/force_py36.py
+-rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/miscellaneous/force_pyi.py
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/miscellaneous/invalid_header.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/miscellaneous/linelength6.py
+-rw-r--r--   0        0        0    11583 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/miscellaneous/long_strings_flag_disabled.py
+-rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/miscellaneous/missing_final_newline.diff
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/miscellaneous/missing_final_newline.py
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/miscellaneous/nested_class_stub.pyi
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/miscellaneous/pattern_matching_invalid.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/miscellaneous/power_op_newline.py
+-rw-r--r--   0        0        0      758 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/miscellaneous/python2_detection.py
+-rw-r--r--   0        0        0     2361 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/miscellaneous/string_quotes.py
+-rw-r--r--   0        0        0     2266 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/miscellaneous/stub.pyi
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/nested_gitignore_tests/pyproject.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/nested_gitignore_tests/x.py
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/nested_gitignore_tests/root/.gitignore
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/nested_gitignore_tests/root/a.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/nested_gitignore_tests/root/b.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/nested_gitignore_tests/root/c.py
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/nested_gitignore_tests/root/child/.gitignore
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/nested_gitignore_tests/root/child/a.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/nested_gitignore_tests/root/child/b.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/nested_gitignore_tests/root/child/c.py
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/preview/async_stmts.py
+-rw-r--r--   0        0        0     4107 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/preview/cantfit.py
+-rw-r--r--   0        0        0     8294 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/preview/comments7.py
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/preview/format_unicode_escape_seq.py
+-rw-r--r--   0        0        0     2784 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/preview/long_dict_values.py
+-rw-r--r--   0        0        0    33216 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/preview/long_strings.py
+-rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/preview/long_strings__east_asian_width.py
+-rw-r--r--   0        0        0     6536 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/preview/long_strings__edge_case.py
+-rw-r--r--   0        0        0    45897 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/preview/long_strings__regression.py
+-rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/preview/long_strings__type_annotations.py
+-rw-r--r--   0        0        0     7207 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/preview/multiline_strings.py
+-rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/preview/percent_precedence.py
+-rw-r--r--   0        0        0     2525 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/preview/prefer_rhs_split.py
+-rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/preview/return_annotation_brackets_string.py
+-rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/preview/trailing_comma.py
+-rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/preview_context_managers/targeting_py38.py
+-rw-r--r--   0        0        0     3361 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/preview_context_managers/targeting_py39.py
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/preview_context_managers/auto_detect/features_3_10.py
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/preview_context_managers/auto_detect/features_3_11.py
+-rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/preview_context_managers/auto_detect/features_3_8.py
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/preview_context_managers/auto_detect/features_3_9.py
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/project_metadata/both_pyproject.toml
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/project_metadata/neither_pyproject.toml
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/project_metadata/only_black_pyproject.toml
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/project_metadata/only_metadata_pyproject.toml
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/py_310/parenthesized_context_managers.py
+-rw-r--r--   0        0        0     2668 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/py_310/pattern_matching_complex.py
+-rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/py_310/pattern_matching_extras.py
+-rw-r--r--   0        0        0     3066 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/py_310/pattern_matching_generic.py
+-rw-r--r--   0        0        0     2641 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/py_310/pattern_matching_simple.py
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/py_310/pattern_matching_style.py
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/py_310/pep_572_py310.py
+-rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/py_310/remove_newline_after_match.py
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/py_310/starred_for_target.py
+-rw-r--r--   0        0        0     2114 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/py_311/pep_646.py
+-rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/py_311/pep_654.py
+-rw-r--r--   0        0        0     2033 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/py_311/pep_654_style.py
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/py_36/numeric_literals.py
+-rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/py_36/numeric_literals_skip_underscores.py
+-rw-r--r--   0        0        0     1199 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/py_37/python37.py
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/py_38/pep_570.py
+-rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/py_38/pep_572.py
+-rw-r--r--   0        0        0     1895 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/py_38/pep_572_remove_parens.py
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/py_38/python38.py
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/py_39/pep_572_py39.py
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/py_39/python39.py
+-rw-r--r--   0        0        0     2575 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/py_39/remove_with_brackets.py
+-rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/simple_cases/attribute_access_on_number_literals.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/simple_cases/beginning_backslash.py
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/simple_cases/bracketmatch.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/simple_cases/class_blank_parentheses.py
+-rw-r--r--   0        0        0     4318 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/simple_cases/class_methods_new_line.py
+-rw-r--r--   0        0        0     3294 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/simple_cases/collections.py
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/simple_cases/comment_after_escaped_newline.py
+-rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/simple_cases/comments.py
+-rw-r--r--   0        0        0     7639 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/simple_cases/comments2.py
+-rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/simple_cases/comments3.py
+-rw-r--r--   0        0        0     3536 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/simple_cases/comments4.py
+-rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/simple_cases/comments5.py
+-rw-r--r--   0        0        0     2567 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/simple_cases/comments6.py
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/simple_cases/comments8.py
+-rw-r--r--   0        0        0     5279 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/simple_cases/comments9.py
+-rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/simple_cases/comments_non_breaking_space.py
+-rw-r--r--   0        0        0     5597 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/simple_cases/composition.py
+-rw-r--r--   0        0        0    11198 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/simple_cases/composition_no_trailing_comma.py
+-rw-r--r--   0        0        0     7699 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/simple_cases/docstring.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/simple_cases/docstring_no_extra_empty_line_before_eof.py
+-rw-r--r--   0        0        0     3513 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/simple_cases/docstring_preview.py
+-rw-r--r--   0        0        0     4596 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/simple_cases/empty_lines.py
+-rw-r--r--   0        0        0    15801 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/simple_cases/expression.diff
+-rw-r--r--   0        0        0    18624 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/simple_cases/expression.py
+-rw-r--r--   0        0        0     9681 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/simple_cases/fmtonoff.py
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/simple_cases/fmtonoff2.py
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/simple_cases/fmtonoff3.py
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/simple_cases/fmtonoff4.py
+-rw-r--r--   0        0        0     3627 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/simple_cases/fmtonoff5.py
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/simple_cases/fmtpass_imports.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/simple_cases/fmtskip.py
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/simple_cases/fmtskip2.py
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/simple_cases/fmtskip3.py
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/simple_cases/fmtskip4.py
+-rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/simple_cases/fmtskip5.py
+-rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/simple_cases/fmtskip6.py
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/simple_cases/fmtskip7.py
+-rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/simple_cases/fmtskip8.py
+-rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/simple_cases/fstring.py
+-rw-r--r--   0        0        0     6482 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/simple_cases/function.py
+-rw-r--r--   0        0        0     2427 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/simple_cases/function2.py
+-rw-r--r--   0        0        0     3657 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/simple_cases/function_trailing_comma.py
+-rw-r--r--   0        0        0     2542 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/simple_cases/import_spacing.py
+-rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/simple_cases/one_element_subscript.py
+-rw-r--r--   0        0        0     3359 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/simple_cases/power_op_spacing.py
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/simple_cases/prefer_rhs_split_reformatted.py
+-rw-r--r--   0        0        0     3205 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/simple_cases/remove_await_parens.py
+-rw-r--r--   0        0        0     2025 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/simple_cases/remove_except_parens.py
+-rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/simple_cases/remove_for_brackets.py
+-rw-r--r--   0        0        0     3351 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/simple_cases/remove_newline_after_code_block_open.py
+-rw-r--r--   0        0        0     3493 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/simple_cases/remove_parens.py
+-rw-r--r--   0        0        0     5141 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/simple_cases/return_annotation_brackets.py
+-rw-r--r--   0        0        0     1398 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/simple_cases/skip_magic_trailing_comma.py
+-rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/simple_cases/slices.py
+-rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/simple_cases/string_prefixes.py
+-rw-r--r--   0        0        0     2279 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/simple_cases/torture.py
+-rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/simple_cases/trailing_comma_optional_parens1.py
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/simple_cases/trailing_comma_optional_parens2.py
+-rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/simple_cases/trailing_comma_optional_parens3.py
+-rw-r--r--   0        0        0     2123 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/simple_cases/trailing_commas_in_leading_parts.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/simple_cases/tricky_unicode_symbols.py
+-rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/simple_cases/tupleassign.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/simple_cases/whitespace.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 cercis-0.1.2/tests/data/type_comments/type_comment_syntax_error.py
+-rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 cercis-0.1.2/.gitignore
+-rw-r--r--   0        0        0     8043 2020-02-02 00:00:00.000000 cercis-0.1.2/AUTHORS.md
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 cercis-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 cercis-0.1.2/LICENSE_ORIGINAL
+-rw-r--r--   0        0        0     6940 2020-02-02 00:00:00.000000 cercis-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0    10925 2020-02-02 00:00:00.000000 cercis-0.1.2/PKG-INFO
```

### Comparing `cercis-0.1.1/.pre-commit-config.yaml` & `cercis-0.1.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/.pre-commit-hooks.yaml` & `cercis-0.1.2/.pre-commit-hooks.yaml`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/CHANGES.md` & `cercis-0.1.2/CHANGES.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,28 @@
 # Change Log
 
 ## [0.1.1] - 2023-05-03
 
 ### Added
+
 - A configurable option: `single-quote`, for formatting code into single quotes
+
 ### Full changelog
-- https://github.com/jsh9/cercis/compare/0.1.0...0.1.1
 
+- https://github.com/jsh9/cercis/compare/0.1.0...0.1.1
 
 ## [0.1.0] - 2023-04-30
 
 This is the initial version that branches away from Black (commit:
 [e712e4](https://github.com/psf/black/commit/e712e48e06420d9240ce95c81acfcf6f11d14c83))
+
 ### Changed
+
 - The default indentation within a function definition (when line wrap happens) is now 8
   spaces. (Black's default is 4, which is
   [not PEP8-compatible](https://github.com/psf/black/issues/1127))
 - Updated README, because `cercis` now branches away from Black
+
 ### Added
+
 - A configurable option (`function-definition-extra-indent`) is added instead of
   enforcing 8 spaces for everyone
```

### Comparing `cercis-0.1.1/Dockerfile` & `cercis-0.1.2/Dockerfile`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/README.md` & `cercis-0.1.2/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -80,14 +80,15 @@
 The main difference is that _Cercis_ provides several configurable options that Black
 doesn't. That's also our main motivation of creating _Cercis_.
 
 _Cercis_ offers the following configurable options:
 
 - [Extra indentation at function definition](#31-extra-indentation-at-function-definition)
 - [Single quote vs double quote](#32-single-quote-vs-double-quote)
+- ["Simple" lines with long strings](#33-simple-lines-with-long-strings)
 
 The next section ([How to configure _Cercis_](#4-how-to-configure-cercis)) contains
 detailed instructions of how to configure these options.
 
 ### 3.1. Extra indentation at function definition
 
 <table>
@@ -128,37 +129,89 @@
 We choose to indent an extra 4 spaces because it adds a clear visual separation between
 the function name and the argument list. Not adding extra indentation is also called out
 as wrong in the the official
 [PEP8 style guide](https://peps.python.org/pep-0008/#indentation).
 
 If you do not like this default, you can easily turn it off.
 
-| Details                |                                                                 |
+| Option                 |                                                                 |
 | ---------------------- | --------------------------------------------------------------- |
 | Name                   | `--function-definition-extra-indent`                            |
 | Abbreviation           | `-fdei`                                                         |
 | Default                | `True`                                                          |
 | Command line usage     | `cercis -fdei=False myScript.py`                                |
 | `pyproject.toml` usage | `function-definition-extra-indent = true` under `[tool.cercis]` |
 | `pre-commit` usage     | `args: [--function-definition-extra-indent=False]`              |
 
 ### 3.2. Single quote vs double quote
 
 Both _Cercis_ and Black default to using double quotes. But in _Cercis_ you can specify
 using single quotes as the default style.
 
-| Details                |                                             |
+| Option                 |                                             |
 | ---------------------- | ------------------------------------------- |
 | Name                   | `--single-quote`                            |
 | Abbreviation           | `-sq`                                       |
 | Default                | `False`                                     |
 | Command line usage     | `cercis -sq=True myScript.py`               |
 | `pyproject.toml` usage | `single-quote = true` under `[tool.cercis]` |
 | `pre-commit` usage     | `args: [--single-quote=False]`              |
 
+### 3.3. "Simple" lines with long strings
+
+By default, Black wraps lines that exceed length limit. But for very simple lines (such
+as assigning a long string to a variable), line wrapping is not necessary.
+
+Also, as seen below, Black's default style can be a bit hard to predict (`var2` vs
+`var3`).
+
+<table>
+  <tr>
+    <td>
+
+```python
+# Cercis's default style
+var1 = "not wrapped even if too long"
+
+var2 = "not wrapped even if too long"  # comment
+
+var3 = "not wrapped, if the line gets too long"
+```
+
+  </td>
+
+  <td>
+
+```python
+# Black's style (not configurable)
+var1 = (
+    "wrapped when too long"
+)
+
+var2 = (
+    "wrapped when too long"
+)  # comment
+
+var3 = "not wrapped, if the line gets too long"
+```
+
+  </td>
+
+  </tr>
+</table>
+
+| Option                 |                                                           |
+| ---------------------- | --------------------------------------------------------- |
+| Name                   | `--wrap-line-with-long-string`                            |
+| Abbreviation           | `-wl`                                                     |
+| Default                | `False`                                                   |
+| Command line usage     | `cercis -wl=True myScript.py`                             |
+| `pyproject.toml` usage | `wrap-line-with-long-string = true` under `[tool.cercis]` |
+| `pre-commit` usage     | `args: [--wrap-line-with-long-string=False]`              |
+
 ## 4. How to configure _Cercis_
 
 ### 4.1. Dynamically in the command line
 
 Here are some examples:
 
 - `cercis --single-quote=True myScript.py` to format files to single quotes
```

#### html2text {}

```diff
@@ -30,51 +30,67 @@
 arguments in pre-commit config. ## 3. The code style The code style in _Cercis_
 is largely consistent with the [style of of _Black_](https://
 black.readthedocs.io/en/stable/the_black_code_style/current_style.html). The
 main difference is that _Cercis_ provides several configurable options that
 Black doesn't. That's also our main motivation of creating _Cercis_. _Cercis_
 offers the following configurable options: - [Extra indentation at function
 definition](#31-extra-indentation-at-function-definition) - [Single quote vs
-double quote](#32-single-quote-vs-double-quote) The next section ([How to
+double quote](#32-single-quote-vs-double-quote) - ["Simple" lines with long
+strings](#33-simple-lines-with-long-strings) The next section ([How to
 configure _Cercis_](#4-how-to-configure-cercis)) contains detailed instructions
 of how to configure these options. ### 3.1. Extra indentation at function
 definition
 ```python # Cercis's default style def  ```python # Black's style (not
 some_function( arg1_with_long_name:     configurable) def some_function
 str, arg2_with_longer_name: int,        ( arg1_with_long_name: str,
 arg3_with_longer_name: float,           arg2_with_longer_name: int,
 arg4_with_longer_name: bool, ) -> None: arg3_with_longer_name: float,
 ... ```                                 arg4_with_longer_name: bool, ) -> None:
                                         ... ```
 We choose to indent an extra 4 spaces because it adds a clear visual separation
 between the function name and the argument list. Not adding extra indentation
 is also called out as wrong in the the official [PEP8 style guide](https://
 peps.python.org/pep-0008/#indentation). If you do not like this default, you
-can easily turn it off. | Details | | | ---------------------- | --------------
-------------------------------------------------- | | Name | `--function-
+can easily turn it off. | Option | | | ---------------------- | ---------------
+------------------------------------------------ | | Name | `--function-
 definition-extra-indent` | | Abbreviation | `-fdei` | | Default | `True` | |
 Command line usage | `cercis -fdei=False myScript.py` | | `pyproject.toml`
 usage | `function-definition-extra-indent = true` under `[tool.cercis]` | |
 `pre-commit` usage | `args: [--function-definition-extra-indent=False]` | ###
 3.2. Single quote vs double quote Both _Cercis_ and Black default to using
 double quotes. But in _Cercis_ you can specify using single quotes as the
-default style. | Details | | | ---------------------- | -----------------------
--------------------- | | Name | `--single-quote` | | Abbreviation | `-sq` | |
+default style. | Option | | | ---------------------- | ------------------------
+------------------- | | Name | `--single-quote` | | Abbreviation | `-sq` | |
 Default | `False` | | Command line usage | `cercis -sq=True myScript.py` | |
 `pyproject.toml` usage | `single-quote = true` under `[tool.cercis]` | | `pre-
-commit` usage | `args: [--single-quote=False]` | ## 4. How to configure
-_Cercis_ ### 4.1. Dynamically in the command line Here are some examples: -
-`cercis --single-quote=True myScript.py` to format files to single quotes -
-`cercis --function-definition-extra-indent=False myScript.py` to format files
-without extra indentation at function definition - `cercis --line-length=79
-myScript.py` to format files with a line length of 79 characters ### 4.2. In
-your project's `pyproject.toml` file You can specify the options under the `
-[tool.cercis]` section of the file: ```toml [tool.cercis] line-length = 88
-function-definition-extra-indent = true single-quote = false ``` ### 4.3. In
-your project's `.pre-commit-config.yaml` file You can specify the options under
-the `args` section of your `.pre-commit-config.yaml` file. For example: ```yaml
-repos: - repo: https://github.com/jsh9/cercis rev: 0.1.0 hooks: - id: cercis
-args: [--function-definition-extra-indent=False, --ling-length=79] - repo:
-https://github.com/jsh9/cercis rev: 0.1.0 hooks: - id: cercis-jupyter args: [--
-function-definition-extra-indent=False, --line-length=79] ``` ### 4.4. Specify
-options in `tox.ini` Currently, _Cercis_ does not support a config section in
-`tox.ini`. Instead, you can specify the options in `pyproject.toml`.
+commit` usage | `args: [--single-quote=False]` | ### 3.3. "Simple" lines with
+long strings By default, Black wraps lines that exceed length limit. But for
+very simple lines (such as assigning a long string to a variable), line
+wrapping is not necessary. Also, as seen below, Black's default style can be a
+bit hard to predict (`var2` vs `var3`).
+```python # Cercis's default style var1 ```python # Black's style (not
+= "not wrapped even if too long" var2 = configurable) var1 = ( "wrapped when
+"not wrapped even if too long" #        too long" ) var2 = ( "wrapped when too
+comment var3 = "not wrapped, if the     long" ) # comment var3 = "not wrapped,
+line gets too long" ```                 if the line gets too long" ```
+| Option | | | ---------------------- | ---------------------------------------
+------------------ | | Name | `--wrap-line-with-long-string` | | Abbreviation |
+`-wl` | | Default | `False` | | Command line usage | `cercis -wl=True
+myScript.py` | | `pyproject.toml` usage | `wrap-line-with-long-string = true`
+under `[tool.cercis]` | | `pre-commit` usage | `args: [--wrap-line-with-long-
+string=False]` | ## 4. How to configure _Cercis_ ### 4.1. Dynamically in the
+command line Here are some examples: - `cercis --single-quote=True myScript.py`
+to format files to single quotes - `cercis --function-definition-extra-
+indent=False myScript.py` to format files without extra indentation at function
+definition - `cercis --line-length=79 myScript.py` to format files with a line
+length of 79 characters ### 4.2. In your project's `pyproject.toml` file You
+can specify the options under the `[tool.cercis]` section of the file: ```toml
+[tool.cercis] line-length = 88 function-definition-extra-indent = true single-
+quote = false ``` ### 4.3. In your project's `.pre-commit-config.yaml` file You
+can specify the options under the `args` section of your `.pre-commit-
+config.yaml` file. For example: ```yaml repos: - repo: https://github.com/jsh9/
+cercis rev: 0.1.0 hooks: - id: cercis args: [--function-definition-extra-
+indent=False, --ling-length=79] - repo: https://github.com/jsh9/cercis rev:
+0.1.0 hooks: - id: cercis-jupyter args: [--function-definition-extra-
+indent=False, --line-length=79] ``` ### 4.4. Specify options in `tox.ini`
+Currently, _Cercis_ does not support a config section in `tox.ini`. Instead,
+you can specify the options in `pyproject.toml`.
```

### Comparing `cercis-0.1.1/action.yml` & `cercis-0.1.2/action.yml`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/mypy.ini` & `cercis-0.1.2/mypy.ini`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/tox.ini` & `cercis-0.1.2/tox.ini`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/.github/CODE_OF_CONDUCT.md` & `cercis-0.1.2/.github/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/.github/PULL_REQUEST_TEMPLATE.md` & `cercis-0.1.2/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/.github/dependabot.yml` & `cercis-0.1.2/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/.github/ISSUE_TEMPLATE/bug_report.md` & `cercis-0.1.2/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/.github/ISSUE_TEMPLATE/config.yml` & `cercis-0.1.2/.github/ISSUE_TEMPLATE/config.yml`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/.github/ISSUE_TEMPLATE/docs-issue.md` & `cercis-0.1.2/.github/ISSUE_TEMPLATE/docs-issue.md`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/.github/ISSUE_TEMPLATE/feature_request.md` & `cercis-0.1.2/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/.github/ISSUE_TEMPLATE/style_issue.md` & `cercis-0.1.2/.github/ISSUE_TEMPLATE/style_issue.md`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/.github/workflows/docker.yml` & `cercis-0.1.2/.github/workflows/docker.yml`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/.github/workflows/fuzz.yml` & `cercis-0.1.2/.github/workflows/fuzz.yml`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/.github/workflows/lint.yml` & `cercis-0.1.2/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/.github/workflows/python-package.yml` & `cercis-0.1.2/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/.github/workflows/python-publish.yml` & `cercis-0.1.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/.github/workflows/test.yml` & `cercis-0.1.2/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/.github/workflows/upload_binary.yml` & `cercis-0.1.2/.github/workflows/upload_binary.yml`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/action/main.py` & `cercis-0.1.2/action/main.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/autoload/black.vim` & `cercis-0.1.2/autoload/black.vim`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/gallery/README.md` & `cercis-0.1.2/gallery/README.md`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/gallery/gallery.py` & `cercis-0.1.2/gallery/gallery.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/plugin/black.vim` & `cercis-0.1.2/plugin/black.vim`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/scripts/diff_shades_gha_helper.py` & `cercis-0.1.2/scripts/diff_shades_gha_helper.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/scripts/fuzz.py` & `cercis-0.1.2/scripts/fuzz.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/scripts/make_width_table.py` & `cercis-0.1.2/scripts/make_width_table.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/scripts/migrate-black.py` & `cercis-0.1.2/scripts/migrate-black.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/src/blackd/__init__.py` & `cercis-0.1.2/src/blackd/__init__.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/src/blackd/middlewares.py` & `cercis-0.1.2/src/blackd/middlewares.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/src/blib2to3/Grammar.txt` & `cercis-0.1.2/src/blib2to3/Grammar.txt`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/src/blib2to3/LICENSE` & `cercis-0.1.2/src/blib2to3/LICENSE`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/src/blib2to3/PatternGrammar.txt` & `cercis-0.1.2/src/blib2to3/PatternGrammar.txt`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/src/blib2to3/README` & `cercis-0.1.2/src/blib2to3/README`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/src/blib2to3/pygram.py` & `cercis-0.1.2/src/blib2to3/pygram.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/src/blib2to3/pytree.py` & `cercis-0.1.2/src/blib2to3/pytree.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/src/blib2to3/pgen2/conv.py` & `cercis-0.1.2/src/blib2to3/pgen2/conv.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/src/blib2to3/pgen2/driver.py` & `cercis-0.1.2/src/blib2to3/pgen2/driver.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/src/blib2to3/pgen2/grammar.py` & `cercis-0.1.2/src/blib2to3/pgen2/grammar.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/src/blib2to3/pgen2/literals.py` & `cercis-0.1.2/src/blib2to3/pgen2/literals.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/src/blib2to3/pgen2/parse.py` & `cercis-0.1.2/src/blib2to3/pgen2/parse.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/src/blib2to3/pgen2/pgen.py` & `cercis-0.1.2/src/blib2to3/pgen2/pgen.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/src/blib2to3/pgen2/token.py` & `cercis-0.1.2/src/blib2to3/pgen2/token.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/src/blib2to3/pgen2/tokenize.py` & `cercis-0.1.2/src/blib2to3/pgen2/tokenize.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 import sys
 from typing import (
     Callable,
     Iterable,
     Iterator,
     List,
     Optional,
+    Set,
     Text,
     Tuple,
     Pattern,
     Union,
     cast,
 )
 
@@ -62,27 +63,27 @@
     "tokenize",
     "generate_tokens",
     "untokenize",
 ]
 del token
 
 
-def group(*choices):
+def group(*choices: str) -> str:
     return "(" + "|".join(choices) + ")"
 
 
-def any(*choices):
+def any(*choices: str) -> str:
     return group(*choices) + "*"
 
 
-def maybe(*choices):
+def maybe(*choices: str) -> str:
     return group(*choices) + "?"
 
 
-def _combinations(*l):
+def _combinations(*l: str) -> Set[str]:
     return set(x + y for x in l for y in l + ("",) if x.casefold() != y.casefold())
 
 
 Whitespace = r"[ \f\t]*"
 Comment = r"#[^\r\n]*"
 Ignore = Whitespace + any(r"\\\r?\n" + Whitespace) + maybe(Comment)
 Name = (  # this is invalid but it's fine because Name comes after Number in all groups
@@ -159,15 +160,14 @@
 endprogs: Final = {
     "'": re.compile(Single),
     '"': re.compile(Double),
     "'''": single3prog,
     '"""': double3prog,
     **{f"{prefix}'''": single3prog for prefix in _strprefixes},
     **{f'{prefix}"""': double3prog for prefix in _strprefixes},
-    **{prefix: None for prefix in _strprefixes},
 }
 
 triple_quoted: Final = (
     {"'''", '"""'}
     | {f"{prefix}'''" for prefix in _strprefixes}
     | {f'{prefix}"""' for prefix in _strprefixes}
 )
@@ -184,23 +184,27 @@
     pass
 
 
 class StopTokenizing(Exception):
     pass
 
 
-def printtoken(type, token, xxx_todo_changeme, xxx_todo_changeme1, line):  # for testing
-    (srow, scol) = xxx_todo_changeme
-    (erow, ecol) = xxx_todo_changeme1
+Coord = Tuple[int, int]
+
+
+def printtoken(
+    type: int, token: Text, srow_col: Coord, erow_col: Coord, line: Text
+) -> None:  # for testing
+    (srow, scol) = srow_col
+    (erow, ecol) = erow_col
     print(
         "%d,%d-%d,%d:\t%s\t%s" % (srow, scol, erow, ecol, tok_name[type], repr(token))
     )
 
 
-Coord = Tuple[int, int]
 TokenEater = Callable[[int, Text, Coord, Coord, Text], None]
 
 
 def tokenize(readline: Callable[[], Text], tokeneater: TokenEater = printtoken) -> None:
     """
     The tokenize() function accepts two parameters: one representing the
     input stream, and one providing an output mechanism for tokenize().
@@ -216,25 +220,24 @@
     try:
         tokenize_loop(readline, tokeneater)
     except StopTokenizing:
         pass
 
 
 # backwards compatible interface
-def tokenize_loop(readline, tokeneater):
+def tokenize_loop(readline: Callable[[], Text], tokeneater: TokenEater) -> None:
     for token_info in generate_tokens(readline):
         tokeneater(*token_info)
 
 
 GoodTokenInfo = Tuple[int, Text, Coord, Coord, Text]
 TokenInfo = Union[Tuple[int, str], GoodTokenInfo]
 
 
 class Untokenizer:
-
     tokens: List[Text]
     prev_row: int
     prev_col: int
 
     def __init__(self) -> None:
         self.tokens = []
         self.prev_row = 1
@@ -595,19 +598,23 @@
                 elif (
                     initial in single_quoted
                     or token[:2] in single_quoted
                     or token[:3] in single_quoted
                 ):
                     if token[-1] == "\n":  # continued string
                         strstart = (lnum, start)
-                        endprog = (
-                            endprogs[initial]
-                            or endprogs[token[1]]
-                            or endprogs[token[2]]
+                        maybe_endprog = (
+                            endprogs.get(initial)
+                            or endprogs.get(token[1])
+                            or endprogs.get(token[2])
                         )
+                        assert (
+                            maybe_endprog is not None
+                        ), f"endprog not found for {token}"
+                        endprog = maybe_endprog
                         contstr, needcont = line[start:], 1
                         contline = line
                         break
                     else:  # ordinary string
                         if stashed:
                             yield stashed
                             stashed = None
@@ -627,15 +634,14 @@
                     tok = (NAME, token, spos, epos, line)
                     if token == "async" and not stashed:
                         stashed = tok
                         continue
 
                     if token in ("def", "for"):
                         if stashed and stashed[0] == NAME and stashed[1] == "async":
-
                             if token == "def":
                                 async_def = True
                                 async_def_indent = indents[-1]
 
                             yield (
                                 ASYNC,
                                 stashed[1],
```

### Comparing `cercis-0.1.1/src/cercis/__init__.py` & `cercis-0.1.2/src/cercis/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,14 +40,15 @@
 from cercis.comments import normalize_fmt_off
 from cercis.const import (
     DEFAULT_EXCLUDES,
     DEFAULT_FUNCTION_DEFINITION_EXTRA_INDENT,
     DEFAULT_INCLUDES,
     DEFAULT_LINE_LENGTH,
     DEFAULT_SINGLE_QUOTE,
+    DEFAULT_WRAP_LINE_WITH_LONG_STRING,
     STDIN_PLACEHOLDER,
 )
 from cercis.files import (
     find_project_root,
     find_pyproject_toml,
     find_user_pyproject_toml,
     gen_python_files,
@@ -230,14 +231,26 @@
     "--single-quote",
     type=bool,
     show_default=True,
     default=DEFAULT_SINGLE_QUOTE,
     help="If True, format code using single quotes; otherwise use double quotes.",
 )
 @click.option(
+    "-wl",
+    "--wrap-line-with-long-string",
+    type=bool,
+    show_default=True,
+    default=DEFAULT_WRAP_LINE_WITH_LONG_STRING,
+    help=(
+        "If False, do not wrap lines with just a variable, an operator, and"
+        " a long string, even if it exceeds the line length limit. If True,"
+        " wrap that line with the string put in parentheses."
+    ),
+)
+@click.option(
     "-t",
     "--target-version",
     type=click.Choice([v.name.lower() for v in TargetVersion]),
     callback=target_version_option_callback,
     multiple=True,
     help=(
         "Python versions that should be supported by Cercis's output. By default,"
@@ -448,14 +461,15 @@
 @click.pass_context
 def main(  # noqa: C901
         ctx: click.Context,
         code: Optional[str],
         line_length: int,
         function_definition_extra_indent: bool,
         single_quote: bool,
+        wrap_line_with_long_string: bool,
         target_version: List[TargetVersion],
         check: bool,
         diff: bool,
         color: bool,
         fast: bool,
         pyi: bool,
         ipynb: bool,
@@ -572,14 +586,15 @@
         string_normalization=not skip_string_normalization,
         magic_trailing_comma=not skip_magic_trailing_comma,
         experimental_string_processing=experimental_string_processing,
         preview=preview,
         python_cell_magics=set(python_cell_magics),
         function_definition_extra_indent=function_definition_extra_indent,
         single_quote=single_quote,
+        wrap_line_with_long_string=wrap_line_with_long_string,
     )
 
     if code is not None:
         # Run in quiet mode by default with -c; the extra output isn't useful.
         # You can still pass -v to get verbose output.
         quiet = True
```

### Comparing `cercis-0.1.1/src/cercis/_width_table.py` & `cercis-0.1.2/src/cercis/_width_table.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/src/cercis/brackets.py` & `cercis-0.1.2/src/cercis/brackets.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/src/cercis/cache.py` & `cercis-0.1.2/src/cercis/cache.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/src/cercis/comments.py` & `cercis-0.1.2/src/cercis/comments.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/src/cercis/concurrency.py` & `cercis-0.1.2/src/cercis/concurrency.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/src/cercis/debug.py` & `cercis-0.1.2/src/cercis/debug.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/src/cercis/files.py` & `cercis-0.1.2/src/cercis/files.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/src/cercis/handle_ipynb_magics.py` & `cercis-0.1.2/src/cercis/handle_ipynb_magics.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/src/cercis/linegen.py` & `cercis-0.1.2/src/cercis/linegen.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,14 +70,15 @@
     StringMerger,
     StringParenStripper,
     StringParenWrapper,
     StringSplitter,
     Transformer,
     hug_power_op,
 )
+from cercis.utils_line_wrapping import check_eligibility_to_opt_out_of_line_wrapping
 
 # types
 LeafID = int
 LN = Union[Leaf, Node]
 
 
 class CannotSplit(CannotTransform):
@@ -519,14 +520,19 @@
     sq = mode.single_quote
 
     string_merge = StringMerger(ll, sn, sq)
     string_paren_strip = StringParenStripper(ll, sn)
     string_split = StringSplitter(ll, sn, sq)
     string_paren_wrap = StringParenWrapper(ll, sn)
 
+    eligible_to_opt_out = check_eligibility_to_opt_out_of_line_wrapping(
+        line,
+        mode.wrap_line_with_long_string,
+    )
+
     transformers: List[Transformer]
     if (
         not line.contains_uncollapsable_type_comments()
         and not line.should_split_rhs
         and not line.magic_trailing_comma
         and (
             is_line_short_enough(line, mode=mode, line_str=line_str)
@@ -579,29 +585,31 @@
                 transformers = [
                     string_merge,
                     string_paren_strip,
                     string_split,
                     delimiter_split,
                     standalone_comment_split,
                     string_paren_wrap,
-                    rhs,
                 ]
             else:
                 transformers = [
                     string_merge,
                     string_paren_strip,
                     string_split,
                     string_paren_wrap,
-                    rhs,
                 ]
         else:
             if line.inside_brackets:
-                transformers = [delimiter_split, standalone_comment_split, rhs]
+                transformers = [delimiter_split, standalone_comment_split]
             else:
-                transformers = [rhs]
+                transformers = []
+
+        if not eligible_to_opt_out:
+            transformers.append(rhs)
+
     # It's always safe to attempt hugging of power operations and pretty much every line
     # could match.
     transformers.append(hug_power_op)
 
     for transform in transformers:
         # We are accumulating lines in `result` because we might want to abort
         # mission and return the original line in the end, or attempt a different
```

### Comparing `cercis-0.1.1/src/cercis/lines.py` & `cercis-0.1.2/src/cercis/lines.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/src/cercis/mode.py` & `cercis-0.1.2/src/cercis/mode.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 else:
     from typing import Final
 
 from cercis.const import (
     DEFAULT_FUNCTION_DEFINITION_EXTRA_INDENT,
     DEFAULT_LINE_LENGTH,
     DEFAULT_SINGLE_QUOTE,
+    DEFAULT_WRAP_LINE_WITH_LONG_STRING,
 )
 
 
 class TargetVersion(Enum):
     PY33 = 3
     PY34 = 4
     PY35 = 5
@@ -186,14 +187,15 @@
     skip_source_first_line: bool = False
     magic_trailing_comma: bool = True
     experimental_string_processing: bool = False
     python_cell_magics: Set[str] = field(default_factory=set)
     preview: bool = False
     function_definition_extra_indent: bool = DEFAULT_FUNCTION_DEFINITION_EXTRA_INDENT
     single_quote: bool = DEFAULT_SINGLE_QUOTE
+    wrap_line_with_long_string: bool = DEFAULT_WRAP_LINE_WITH_LONG_STRING
 
     def __post_init__(self) -> None:
         if self.experimental_string_processing:
             warn(
                 "`experimental string processing` has been included in `preview`"
                 " and deprecated. Use `preview` instead.",
                 Deprecated,
```

### Comparing `cercis-0.1.1/src/cercis/nodes.py` & `cercis-0.1.2/src/cercis/nodes.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/src/cercis/numerics.py` & `cercis-0.1.2/src/cercis/numerics.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/src/cercis/output.py` & `cercis-0.1.2/src/cercis/output.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/src/cercis/parsing.py` & `cercis-0.1.2/src/cercis/parsing.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/src/cercis/report.py` & `cercis-0.1.2/src/cercis/report.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/src/cercis/rusty.py` & `cercis-0.1.2/src/cercis/rusty.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/src/cercis/strings.py` & `cercis-0.1.2/src/cercis/strings.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/src/cercis/trans.py` & `cercis-0.1.2/src/cercis/trans.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/tests/optional.py` & `cercis-0.1.2/tests/optional.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/tests/test_black.py` & `cercis-0.1.2/tests/test_black.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/tests/test_blackd.py` & `cercis-0.1.2/tests/test_blackd.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/tests/test_format.py` & `cercis-0.1.2/tests/test_format.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,22 +29,25 @@
     assert_format(source, expected, mode, fast=False)
 
 
 @pytest.mark.filterwarnings("ignore:invalid escape sequence.*:DeprecationWarning")
 @pytest.mark.parametrize("filename", all_data_cases("simple_cases"))
 def test_simple_format(filename: str) -> None:
     magic_trailing_comma = filename != "skip_magic_trailing_comma"
-    check_file(
-        "simple_cases", filename, cercis.Mode(magic_trailing_comma=magic_trailing_comma)
+    mode = cercis.Mode(
+        magic_trailing_comma=magic_trailing_comma,
+        wrap_line_with_long_string=True,
     )
+    check_file("simple_cases", filename, mode)
 
 
 @pytest.mark.parametrize("filename", all_data_cases("preview"))
 def test_preview_format(filename: str) -> None:
-    check_file("preview", filename, cercis.Mode(preview=True))
+    mode = cercis.Mode(preview=True, wrap_line_with_long_string=True)
+    check_file("preview", filename, mode)
 
 
 def test_preview_context_managers_targeting_py38() -> None:
     source, expected = read_data("preview_context_managers", "targeting_py38.py")
     mode = cercis.Mode(preview=True, target_versions={cercis.TargetVersion.PY38})
     assert_format(source, expected, mode, minimum_version=(3, 8))
 
@@ -172,15 +175,19 @@
     mode = replace(DEFAULT_MODE, string_normalization=False, preview=True)
     assert_format(source, expected, mode)
 
 
 def test_long_strings_flag_disabled() -> None:
     """Tests for turning off the string processing logic."""
     source, expected = read_data("miscellaneous", "long_strings_flag_disabled")
-    mode = replace(DEFAULT_MODE, experimental_string_processing=False)
+    mode = replace(
+        DEFAULT_MODE,
+        experimental_string_processing=False,
+        wrap_line_with_long_string=True,
+    )
     assert_format(source, expected, mode)
 
 
 def test_stub() -> None:
     mode = replace(DEFAULT_MODE, is_pyi=True)
     source, expected = read_data("miscellaneous", "stub.pyi")
     assert_format(source, expected, mode)
@@ -204,24 +211,38 @@
     assert_format(source, expected)
     cercis.assert_equivalent(source, expected)
 
 
 @pytest.mark.parametrize(
     "filename, extra_indent",
     [
-        ("func_def_extra_indent.py", True),
-        ("func_def_no_extra_indent.py", False),
+        ("func_def_extra_indent.py", True),  # Cercis's default
+        ("func_def_no_extra_indent.py", False),  # Black's default
     ],
 )
 def test_function_definition_extra_indent(filename: str, extra_indent: bool) -> None:
     mode = replace(DEFAULT_MODE, function_definition_extra_indent=extra_indent)
-    check_file("configurable_cases", filename, mode)
+    check_file("configurable_cases/func_def_indent", filename, mode)
 
 
 @pytest.mark.filterwarnings("ignore:invalid escape sequence.*:DeprecationWarning")
 @pytest.mark.parametrize(
     "filename",
     all_data_cases("configurable_cases/single_quote"),
 )
 def test_single_quote(filename: str) -> None:
-    mode = replace(DEFAULT_MODE, single_quote=True)
+    mode = replace(DEFAULT_MODE, single_quote=True, wrap_line_with_long_string=True)
     check_file("configurable_cases/single_quote", filename, mode)
+
+
+@pytest.mark.parametrize(
+    "filename, wrap_line",
+    [
+        ("test_cases__Cercis_default.py", False),
+        ("test_cases__Black_default.py", True),
+        ("long_strings_flag_disabled__Cercis_default.py", False),
+        ("long_strings_flag_disabled__Black_default.py", True),
+    ],
+)
+def test_opt_out_of_wrapping(filename: str, wrap_line: bool) -> None:
+    mode = replace(DEFAULT_MODE, wrap_line_with_long_string=wrap_line)
+    check_file("configurable_cases/line_with_long_string", filename, mode)
```

### Comparing `cercis-0.1.1/tests/test_ipynb.py` & `cercis-0.1.2/tests/test_ipynb.py`

 * *Files 1% similar despite different names*

```diff
@@ -251,14 +251,15 @@
     with pytest.raises(NothingChanged):
         format_cell(src, fast=True, mode=JUPYTER_MODE)
 
 
 def test_entire_notebook_empty_metadata() -> None:
     content = read_jupyter_notebook("jupyter", "notebook_empty_metadata")
     result = format_file_contents(content, fast=True, mode=JUPYTER_MODE)
+    # fmt: off
     expected = (
         "{\n"
         ' "cells": [\n'
         "  {\n"
         '   "cell_type": "code",\n'
         '   "execution_count": null,\n'
         '   "metadata": {\n'
@@ -280,20 +281,22 @@
         "  }\n"
         " ],\n"
         ' "metadata": {},\n'
         ' "nbformat": 4,\n'
         ' "nbformat_minor": 4\n'
         "}\n"
     )
+    # fmt: on
     assert result == expected
 
 
 def test_entire_notebook_trailing_newline() -> None:
     content = read_jupyter_notebook("jupyter", "notebook_trailing_newline")
     result = format_file_contents(content, fast=True, mode=JUPYTER_MODE)
+    # fmt: off
     expected = (
         "{\n"
         ' "cells": [\n'
         "  {\n"
         '   "cell_type": "code",\n'
         '   "execution_count": null,\n'
         '   "metadata": {\n'
@@ -327,20 +330,22 @@
         '   "version": ""\n'
         "  }\n"
         " },\n"
         ' "nbformat": 4,\n'
         ' "nbformat_minor": 4\n'
         "}\n"
     )
+    # fmt: on
     assert result == expected
 
 
 def test_entire_notebook_no_trailing_newline() -> None:
     content = read_jupyter_notebook("jupyter", "notebook_no_trailing_newline")
     result = format_file_contents(content, fast=True, mode=JUPYTER_MODE)
+    # fmt: off
     expected = (
         "{\n"
         ' "cells": [\n'
         "  {\n"
         '   "cell_type": "code",\n'
         '   "execution_count": null,\n'
         '   "metadata": {\n'
@@ -374,14 +379,15 @@
         '   "version": ""\n'
         "  }\n"
         " },\n"
         ' "nbformat": 4,\n'
         ' "nbformat_minor": 4\n'
         "}"
     )
+    # fmt: on
     assert result == expected
 
 
 def test_entire_notebook_without_changes() -> None:
     content = read_jupyter_notebook("jupyter", "notebook_without_changes")
     with pytest.raises(NothingChanged):
         format_file_contents(content, fast=True, mode=JUPYTER_MODE)
```

### Comparing `cercis-0.1.1/tests/test_no_ipynb.py` & `cercis-0.1.2/tests/test_no_ipynb.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/tests/test_trans.py` & `cercis-0.1.2/tests/test_trans.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/tests/util.py` & `cercis-0.1.2/tests/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import os
 import sys
+import traceback
 import unittest
 from contextlib import contextmanager
 from dataclasses import replace
 from functools import partial
 from pathlib import Path
 from typing import Any, Iterator, List, Optional, Tuple
 
@@ -87,16 +88,17 @@
             None,
             replace(mode, preview=not mode.preview),
             fast=fast,
             minimum_version=minimum_version,
         )
     except Exception as e:
         text = "non-preview" if mode.preview else "preview"
+        tb = traceback.format_exc()
         raise FormatFailure(
-            f"Black crashed formatting this case in {text} mode."
+            f"Black crashed formatting this case in {text} mode.\n{e}\n{tb}"
         ) from e
     # Similarly, setting line length to 1 is a good way to catch
     # stability bugs. But only in non-preview mode because preview mode
     # currently has a lot of line length 1 bugs.
     try:
         _assert_format_inner(
             source,
```

### Comparing `cercis-0.1.1/tests/data/conditional_expression.py` & `cercis-0.1.2/tests/data/conditional_expression.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/tests/data/configurable_cases/single_quote/docstring.py` & `cercis-0.1.2/tests/data/configurable_cases/single_quote/docstring.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/tests/data/configurable_cases/single_quote/docstring_preview.py` & `cercis-0.1.2/tests/data/configurable_cases/single_quote/docstring_preview.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/tests/data/configurable_cases/single_quote/more_quotes.py` & `cercis-0.1.2/tests/data/configurable_cases/single_quote/more_quotes.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/tests/data/configurable_cases/single_quote/string_prefixes.py` & `cercis-0.1.2/tests/data/configurable_cases/single_quote/string_prefixes.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/tests/data/configurable_cases/single_quote/torture.py` & `cercis-0.1.2/tests/data/configurable_cases/single_quote/torture.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/tests/data/jupyter/notebook_no_trailing_newline.ipynb` & `cercis-0.1.2/tests/data/jupyter/notebook_no_trailing_newline.ipynb`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/tests/data/jupyter/notebook_trailing_newline.ipynb` & `cercis-0.1.2/tests/data/jupyter/notebook_trailing_newline.ipynb`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/tests/data/jupyter/notebook_without_changes.ipynb` & `cercis-0.1.2/tests/data/jupyter/notebook_without_changes.ipynb`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/tests/data/miscellaneous/debug_visitor.out` & `cercis-0.1.2/tests/data/miscellaneous/debug_visitor.out`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/tests/data/miscellaneous/debug_visitor.py` & `cercis-0.1.2/tests/data/miscellaneous/debug_visitor.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/tests/data/miscellaneous/decorators.py` & `cercis-0.1.2/tests/data/miscellaneous/decorators.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/tests/data/miscellaneous/docstring_no_string_normalization.py` & `cercis-0.1.2/tests/data/miscellaneous/docstring_no_string_normalization.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/tests/data/miscellaneous/expression_skip_magic_trailing_comma.diff` & `cercis-0.1.2/tests/data/miscellaneous/expression_skip_magic_trailing_comma.diff`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/tests/data/miscellaneous/force_py36.py` & `cercis-0.1.2/tests/data/miscellaneous/force_py36.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/tests/data/miscellaneous/force_pyi.py` & `cercis-0.1.2/tests/data/miscellaneous/force_pyi.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/tests/data/miscellaneous/long_strings_flag_disabled.py` & `cercis-0.1.2/tests/data/configurable_cases/line_with_long_string/long_strings_flag_disabled__Black_default.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/tests/data/miscellaneous/python2_detection.py` & `cercis-0.1.2/tests/data/miscellaneous/python2_detection.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/tests/data/miscellaneous/string_quotes.py` & `cercis-0.1.2/tests/data/miscellaneous/string_quotes.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/tests/data/miscellaneous/stub.pyi` & `cercis-0.1.2/tests/data/miscellaneous/stub.pyi`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/tests/data/preview/cantfit.py` & `cercis-0.1.2/tests/data/preview/cantfit.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/tests/data/preview/comments7.py` & `cercis-0.1.2/tests/data/preview/comments7.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/tests/data/preview/format_unicode_escape_seq.py` & `cercis-0.1.2/tests/data/preview/format_unicode_escape_seq.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/tests/data/preview/long_dict_values.py` & `cercis-0.1.2/tests/data/preview/long_dict_values.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/tests/data/preview/long_strings.py` & `cercis-0.1.2/tests/data/preview/long_strings.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/tests/data/preview/long_strings__east_asian_width.py` & `cercis-0.1.2/tests/data/preview/long_strings__east_asian_width.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/tests/data/preview/long_strings__edge_case.py` & `cercis-0.1.2/tests/data/preview/long_strings__edge_case.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/tests/data/preview/long_strings__regression.py` & `cercis-0.1.2/tests/data/preview/long_strings__regression.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/tests/data/preview/long_strings__type_annotations.py` & `cercis-0.1.2/tests/data/preview/long_strings__type_annotations.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/tests/data/preview/multiline_strings.py` & `cercis-0.1.2/tests/data/preview/multiline_strings.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/tests/data/preview/prefer_rhs_split.py` & `cercis-0.1.2/tests/data/preview/prefer_rhs_split.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/tests/data/preview/trailing_comma.py` & `cercis-0.1.2/tests/data/preview/trailing_comma.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/tests/data/preview_context_managers/targeting_py38.py` & `cercis-0.1.2/tests/data/preview_context_managers/targeting_py38.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/tests/data/preview_context_managers/targeting_py39.py` & `cercis-0.1.2/tests/data/preview_context_managers/targeting_py39.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/tests/data/preview_context_managers/auto_detect/features_3_10.py` & `cercis-0.1.2/tests/data/preview_context_managers/auto_detect/features_3_10.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/tests/data/preview_context_managers/auto_detect/features_3_11.py` & `cercis-0.1.2/tests/data/preview_context_managers/auto_detect/features_3_11.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/tests/data/preview_context_managers/auto_detect/features_3_8.py` & `cercis-0.1.2/tests/data/preview_context_managers/auto_detect/features_3_8.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/tests/data/preview_context_managers/auto_detect/features_3_9.py` & `cercis-0.1.2/tests/data/preview_context_managers/auto_detect/features_3_9.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/tests/data/py_310/parenthesized_context_managers.py` & `cercis-0.1.2/tests/data/py_310/parenthesized_context_managers.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/tests/data/py_310/pattern_matching_complex.py` & `cercis-0.1.2/tests/data/py_310/pattern_matching_complex.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/tests/data/py_310/pattern_matching_extras.py` & `cercis-0.1.2/tests/data/py_310/pattern_matching_extras.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/tests/data/py_310/pattern_matching_generic.py` & `cercis-0.1.2/tests/data/py_310/pattern_matching_generic.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/tests/data/py_310/pattern_matching_simple.py` & `cercis-0.1.2/tests/data/py_310/pattern_matching_simple.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/tests/data/py_310/pattern_matching_style.py` & `cercis-0.1.2/tests/data/py_310/pattern_matching_style.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/tests/data/py_311/pep_646.py` & `cercis-0.1.2/tests/data/py_311/pep_646.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/tests/data/py_311/pep_654.py` & `cercis-0.1.2/tests/data/py_311/pep_654.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/tests/data/py_311/pep_654_style.py` & `cercis-0.1.2/tests/data/py_311/pep_654_style.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/tests/data/py_36/numeric_literals.py` & `cercis-0.1.2/tests/data/py_36/numeric_literals.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/tests/data/py_37/python37.py` & `cercis-0.1.2/tests/data/py_37/python37.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/tests/data/py_38/pep_570.py` & `cercis-0.1.2/tests/data/py_38/pep_570.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/tests/data/py_38/pep_572.py` & `cercis-0.1.2/tests/data/py_38/pep_572.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/tests/data/py_38/pep_572_remove_parens.py` & `cercis-0.1.2/tests/data/py_38/pep_572_remove_parens.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/tests/data/py_38/python38.py` & `cercis-0.1.2/tests/data/py_38/python38.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/tests/data/py_39/python39.py` & `cercis-0.1.2/tests/data/py_39/python39.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/tests/data/py_39/remove_with_brackets.py` & `cercis-0.1.2/tests/data/py_39/remove_with_brackets.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/tests/data/simple_cases/attribute_access_on_number_literals.py` & `cercis-0.1.2/tests/data/simple_cases/attribute_access_on_number_literals.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/tests/data/simple_cases/class_blank_parentheses.py` & `cercis-0.1.2/tests/data/simple_cases/class_blank_parentheses.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/tests/data/simple_cases/class_methods_new_line.py` & `cercis-0.1.2/tests/data/simple_cases/class_methods_new_line.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/tests/data/simple_cases/collections.py` & `cercis-0.1.2/tests/data/simple_cases/collections.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/tests/data/simple_cases/comments.py` & `cercis-0.1.2/tests/data/simple_cases/comments.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/tests/data/simple_cases/comments2.py` & `cercis-0.1.2/tests/data/simple_cases/comments2.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/tests/data/simple_cases/comments3.py` & `cercis-0.1.2/tests/data/simple_cases/comments3.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/tests/data/simple_cases/comments4.py` & `cercis-0.1.2/tests/data/simple_cases/comments4.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/tests/data/simple_cases/comments5.py` & `cercis-0.1.2/tests/data/simple_cases/comments5.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/tests/data/simple_cases/comments6.py` & `cercis-0.1.2/tests/data/simple_cases/comments6.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/tests/data/simple_cases/comments9.py` & `cercis-0.1.2/tests/data/simple_cases/comments9.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/tests/data/simple_cases/comments_non_breaking_space.py` & `cercis-0.1.2/tests/data/simple_cases/comments_non_breaking_space.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/tests/data/simple_cases/composition.py` & `cercis-0.1.2/tests/data/simple_cases/composition.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/tests/data/simple_cases/composition_no_trailing_comma.py` & `cercis-0.1.2/tests/data/simple_cases/composition_no_trailing_comma.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/tests/data/simple_cases/docstring.py` & `cercis-0.1.2/tests/data/simple_cases/docstring.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/tests/data/simple_cases/docstring_preview.py` & `cercis-0.1.2/tests/data/simple_cases/docstring_preview.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/tests/data/simple_cases/empty_lines.py` & `cercis-0.1.2/tests/data/simple_cases/empty_lines.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/tests/data/simple_cases/expression.diff` & `cercis-0.1.2/tests/data/simple_cases/expression.diff`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/tests/data/simple_cases/expression.py` & `cercis-0.1.2/tests/data/simple_cases/expression.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/tests/data/simple_cases/fmtonoff.py` & `cercis-0.1.2/tests/data/simple_cases/fmtonoff.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/tests/data/simple_cases/fmtonoff2.py` & `cercis-0.1.2/tests/data/simple_cases/fmtonoff2.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/tests/data/simple_cases/fmtonoff5.py` & `cercis-0.1.2/tests/data/simple_cases/fmtonoff5.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/tests/data/simple_cases/fmtskip2.py` & `cercis-0.1.2/tests/data/simple_cases/fmtskip2.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/tests/data/simple_cases/fmtskip8.py` & `cercis-0.1.2/tests/data/simple_cases/fmtskip8.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/tests/data/simple_cases/function.py` & `cercis-0.1.2/tests/data/simple_cases/function.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/tests/data/simple_cases/function2.py` & `cercis-0.1.2/tests/data/simple_cases/function2.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/tests/data/simple_cases/function_trailing_comma.py` & `cercis-0.1.2/tests/data/simple_cases/function_trailing_comma.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/tests/data/simple_cases/import_spacing.py` & `cercis-0.1.2/tests/data/simple_cases/import_spacing.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/tests/data/simple_cases/one_element_subscript.py` & `cercis-0.1.2/tests/data/simple_cases/one_element_subscript.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/tests/data/simple_cases/power_op_spacing.py` & `cercis-0.1.2/tests/data/simple_cases/power_op_spacing.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/tests/data/simple_cases/prefer_rhs_split_reformatted.py` & `cercis-0.1.2/tests/data/simple_cases/prefer_rhs_split_reformatted.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/tests/data/simple_cases/remove_await_parens.py` & `cercis-0.1.2/tests/data/simple_cases/remove_await_parens.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/tests/data/simple_cases/remove_except_parens.py` & `cercis-0.1.2/tests/data/simple_cases/remove_except_parens.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/tests/data/simple_cases/remove_for_brackets.py` & `cercis-0.1.2/tests/data/simple_cases/remove_for_brackets.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/tests/data/simple_cases/remove_newline_after_code_block_open.py` & `cercis-0.1.2/tests/data/simple_cases/remove_newline_after_code_block_open.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/tests/data/simple_cases/remove_parens.py` & `cercis-0.1.2/tests/data/simple_cases/remove_parens.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/tests/data/simple_cases/return_annotation_brackets.py` & `cercis-0.1.2/tests/data/simple_cases/return_annotation_brackets.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/tests/data/simple_cases/skip_magic_trailing_comma.py` & `cercis-0.1.2/tests/data/simple_cases/skip_magic_trailing_comma.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/tests/data/simple_cases/slices.py` & `cercis-0.1.2/tests/data/simple_cases/slices.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/tests/data/simple_cases/string_prefixes.py` & `cercis-0.1.2/tests/data/simple_cases/string_prefixes.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/tests/data/simple_cases/torture.py` & `cercis-0.1.2/tests/data/simple_cases/torture.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/tests/data/simple_cases/trailing_comma_optional_parens1.py` & `cercis-0.1.2/tests/data/simple_cases/trailing_comma_optional_parens1.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/tests/data/simple_cases/trailing_comma_optional_parens3.py` & `cercis-0.1.2/tests/data/simple_cases/trailing_comma_optional_parens3.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/tests/data/simple_cases/trailing_commas_in_leading_parts.py` & `cercis-0.1.2/tests/data/simple_cases/trailing_commas_in_leading_parts.py`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/AUTHORS.md` & `cercis-0.1.2/AUTHORS.md`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/LICENSE` & `cercis-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/LICENSE_ORIGINAL` & `cercis-0.1.2/LICENSE_ORIGINAL`

 * *Files identical despite different names*

### Comparing `cercis-0.1.1/pyproject.toml` & `cercis-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
 [build-system]
 requires = ["hatchling>=1.8.0", "hatch-vcs", "hatch-fancy-pypi-readme"]
 build-backend = "hatchling.build"
 
 [project]
 name = "cercis"
-version = "0.1.1"
+version = "0.1.2"
 description = "A more configurable Python code formatter"
 license = { text = "MIT" }
 requires-python = ">=3.7"
 authors = [
   { name = "Łukasz Langa", email = "lukasz@langa.pl" },
   { name = "jsh9", email = "" },
 ]
```

### Comparing `cercis-0.1.1/PKG-INFO` & `cercis-0.1.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cercis
-Version: 0.1.1
+Version: 0.1.2
 Summary: A more configurable Python code formatter
 Project-URL: Changelog, https://github.com/jsh9/cercis/blob/main/CHANGES.md
 Project-URL: Homepage, https://github.com/jsh9/cercis
 Author: jsh9
 Author-email: Łukasz Langa <lukasz@langa.pl>
 License: MIT
 License-File: AUTHORS.md
@@ -127,14 +127,15 @@
 The main difference is that _Cercis_ provides several configurable options that Black
 doesn't. That's also our main motivation of creating _Cercis_.
 
 _Cercis_ offers the following configurable options:
 
 - [Extra indentation at function definition](#31-extra-indentation-at-function-definition)
 - [Single quote vs double quote](#32-single-quote-vs-double-quote)
+- ["Simple" lines with long strings](#33-simple-lines-with-long-strings)
 
 The next section ([How to configure _Cercis_](#4-how-to-configure-cercis)) contains
 detailed instructions of how to configure these options.
 
 ### 3.1. Extra indentation at function definition
 
 <table>
@@ -175,37 +176,89 @@
 We choose to indent an extra 4 spaces because it adds a clear visual separation between
 the function name and the argument list. Not adding extra indentation is also called out
 as wrong in the the official
 [PEP8 style guide](https://peps.python.org/pep-0008/#indentation).
 
 If you do not like this default, you can easily turn it off.
 
-| Details                |                                                                 |
+| Option                 |                                                                 |
 | ---------------------- | --------------------------------------------------------------- |
 | Name                   | `--function-definition-extra-indent`                            |
 | Abbreviation           | `-fdei`                                                         |
 | Default                | `True`                                                          |
 | Command line usage     | `cercis -fdei=False myScript.py`                                |
 | `pyproject.toml` usage | `function-definition-extra-indent = true` under `[tool.cercis]` |
 | `pre-commit` usage     | `args: [--function-definition-extra-indent=False]`              |
 
 ### 3.2. Single quote vs double quote
 
 Both _Cercis_ and Black default to using double quotes. But in _Cercis_ you can specify
 using single quotes as the default style.
 
-| Details                |                                             |
+| Option                 |                                             |
 | ---------------------- | ------------------------------------------- |
 | Name                   | `--single-quote`                            |
 | Abbreviation           | `-sq`                                       |
 | Default                | `False`                                     |
 | Command line usage     | `cercis -sq=True myScript.py`               |
 | `pyproject.toml` usage | `single-quote = true` under `[tool.cercis]` |
 | `pre-commit` usage     | `args: [--single-quote=False]`              |
 
+### 3.3. "Simple" lines with long strings
+
+By default, Black wraps lines that exceed length limit. But for very simple lines (such
+as assigning a long string to a variable), line wrapping is not necessary.
+
+Also, as seen below, Black's default style can be a bit hard to predict (`var2` vs
+`var3`).
+
+<table>
+  <tr>
+    <td>
+
+```python
+# Cercis's default style
+var1 = "not wrapped even if too long"
+
+var2 = "not wrapped even if too long"  # comment
+
+var3 = "not wrapped, if the line gets too long"
+```
+
+  </td>
+
+  <td>
+
+```python
+# Black's style (not configurable)
+var1 = (
+    "wrapped when too long"
+)
+
+var2 = (
+    "wrapped when too long"
+)  # comment
+
+var3 = "not wrapped, if the line gets too long"
+```
+
+  </td>
+
+  </tr>
+</table>
+
+| Option                 |                                                           |
+| ---------------------- | --------------------------------------------------------- |
+| Name                   | `--wrap-line-with-long-string`                            |
+| Abbreviation           | `-wl`                                                     |
+| Default                | `False`                                                   |
+| Command line usage     | `cercis -wl=True myScript.py`                             |
+| `pyproject.toml` usage | `wrap-line-with-long-string = true` under `[tool.cercis]` |
+| `pre-commit` usage     | `args: [--wrap-line-with-long-string=False]`              |
+
 ## 4. How to configure _Cercis_
 
 ### 4.1. Dynamically in the command line
 
 Here are some examples:
 
 - `cercis --single-quote=True myScript.py` to format files to single quotes
@@ -251,24 +304,30 @@
 Currently, _Cercis_ does not support a config section in `tox.ini`. Instead, you can
 specify the options in `pyproject.toml`.
 # Change Log
 
 ## [0.1.1] - 2023-05-03
 
 ### Added
+
 - A configurable option: `single-quote`, for formatting code into single quotes
+
 ### Full changelog
-- https://github.com/jsh9/cercis/compare/0.1.0...0.1.1
 
+- https://github.com/jsh9/cercis/compare/0.1.0...0.1.1
 
 ## [0.1.0] - 2023-04-30
 
 This is the initial version that branches away from Black (commit:
 [e712e4](https://github.com/psf/black/commit/e712e48e06420d9240ce95c81acfcf6f11d14c83))
+
 ### Changed
+
 - The default indentation within a function definition (when line wrap happens) is now 8
   spaces. (Black's default is 4, which is
   [not PEP8-compatible](https://github.com/psf/black/issues/1127))
 - Updated README, because `cercis` now branches away from Black
+
 ### Added
+
 - A configurable option (`function-definition-extra-indent`) is added instead of
   enforcing 8 spaces for everyone
```

