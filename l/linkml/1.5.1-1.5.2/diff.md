# Comparing `tmp/linkml-1.5.1.tar.gz` & `tmp/linkml-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linkml-1.5.1.tar", max compression
+gzip compressed data, was "linkml-1.5.2.tar", max compression
```

## Comparing `linkml-1.5.1.tar` & `linkml-1.5.2.tar`

### file list

```diff
@@ -1,108 +1,108 @@
--rw-r--r--   0        0        0     6555 2023-04-25 21:29:56.109279 linkml-1.5.1/LICENSE
--rw-r--r--   0        0        0     1369 2023-04-25 21:29:56.109279 linkml-1.5.1/README.md
--rw-r--r--   0        0        0     3227 2023-04-25 21:29:56.133279 linkml-1.5.1/linkml/__init__.py
--rw-r--r--   0        0        0      326 2023-04-25 21:29:56.133279 linkml-1.5.1/linkml/_version.py
--rw-r--r--   0        0        0    51005 2023-04-25 21:29:56.133279 linkml-1.5.1/linkml/generators/PythonGenNotes.md
--rw-r--r--   0        0        0     3926 2023-04-25 21:29:56.133279 linkml-1.5.1/linkml/generators/README.md
--rw-r--r--   0        0        0      616 2023-04-25 21:29:56.133279 linkml-1.5.1/linkml/generators/__init__.py
--rw-r--r--   0        0        0        0 2023-04-25 21:29:56.133279 linkml-1.5.1/linkml/generators/common/__init__.py
--rw-r--r--   0        0        0     2040 2023-04-25 21:29:56.133279 linkml-1.5.1/linkml/generators/common/type_designators.py
--rw-r--r--   0        0        0     3118 2023-04-25 21:29:56.133279 linkml-1.5.1/linkml/generators/csvgen.py
--rw-r--r--   0        0        0     2873 2023-04-25 21:29:56.133279 linkml-1.5.1/linkml/generators/docgen/class.md.jinja2
--rw-r--r--   0        0        0     2682 2023-04-25 21:29:56.133279 linkml-1.5.1/linkml/generators/docgen/class_diagram.md.jinja2
--rw-r--r--   0        0        0     1321 2023-04-25 21:29:56.133279 linkml-1.5.1/linkml/generators/docgen/common_metadata.md.jinja2
--rw-r--r--   0        0        0     1018 2023-04-25 21:29:56.133279 linkml-1.5.1/linkml/generators/docgen/enum.md.jinja2
--rw-r--r--   0        0        0     1190 2023-04-25 21:29:56.133279 linkml-1.5.1/linkml/generators/docgen/index.md.jinja2
--rw-r--r--   0        0        0      501 2023-04-25 21:29:56.133279 linkml-1.5.1/linkml/generators/docgen/index.tex.jinja2
--rw-r--r--   0        0        0       70 2023-04-25 21:29:56.133279 linkml-1.5.1/linkml/generators/docgen/schema.md.jinja2
--rw-r--r--   0        0        0     2557 2023-04-25 21:29:56.133279 linkml-1.5.1/linkml/generators/docgen/slot.md.jinja2
--rw-r--r--   0        0        0     1704 2023-04-25 21:29:56.133279 linkml-1.5.1/linkml/generators/docgen/subset.md.jinja2
--rw-r--r--   0        0        0      635 2023-04-25 21:29:56.133279 linkml-1.5.1/linkml/generators/docgen/type.md.jinja2
--rw-r--r--   0        0        0    32663 2023-04-25 21:29:56.133279 linkml-1.5.1/linkml/generators/docgen.py
--rw-r--r--   0        0        0     5112 2023-04-25 21:29:56.133279 linkml-1.5.1/linkml/generators/dotgen.py
--rw-r--r--   0        0        0    10863 2023-04-25 21:29:56.133279 linkml-1.5.1/linkml/generators/erdiagramgen.py
--rw-r--r--   0        0        0     6894 2023-04-25 21:29:56.133279 linkml-1.5.1/linkml/generators/excelgen.py
--rw-r--r--   0        0        0     3575 2023-04-25 21:29:56.133279 linkml-1.5.1/linkml/generators/golrgen.py
--rw-r--r--   0        0        0     2347 2023-04-25 21:29:56.133279 linkml-1.5.1/linkml/generators/graphqlgen.py
--rw-r--r--   0        0        0      444 2023-04-25 21:29:56.133279 linkml-1.5.1/linkml/generators/javagen/example_template.java.jinja2
--rw-r--r--   0        0        0     1737 2023-04-25 21:29:56.133279 linkml-1.5.1/linkml/generators/javagen/java_record_template.jinja2
--rw-r--r--   0        0        0     5499 2023-04-25 21:29:56.133279 linkml-1.5.1/linkml/generators/javagen.py
--rw-r--r--   0        0        0     8821 2023-04-25 21:29:56.133279 linkml-1.5.1/linkml/generators/jsonldcontextgen.py
--rw-r--r--   0        0        0     7952 2023-04-25 21:29:56.133279 linkml-1.5.1/linkml/generators/jsonldgen.py
--rw-r--r--   0        0        0    19361 2023-04-25 21:29:56.137279 linkml-1.5.1/linkml/generators/jsonschemagen.py
--rw-r--r--   0        0        0     3555 2023-04-25 21:29:56.137279 linkml-1.5.1/linkml/generators/linkmlgen.py
--rw-r--r--   0        0        0    34422 2023-04-25 21:29:56.137279 linkml-1.5.1/linkml/generators/markdowngen.py
--rw-r--r--   0        0        0     6532 2023-04-25 21:29:56.137279 linkml-1.5.1/linkml/generators/namespacegen.py
--rw-r--r--   0        0        0     6695 2023-04-25 21:29:56.137279 linkml-1.5.1/linkml/generators/oocodegen.py
--rw-r--r--   0        0        0    27365 2023-04-25 21:29:56.137279 linkml-1.5.1/linkml/generators/owlgen.py
--rw-r--r--   0        0        0     4911 2023-04-25 21:29:56.137279 linkml-1.5.1/linkml/generators/prefixmapgen.py
--rw-r--r--   0        0        0     9811 2023-04-25 21:29:56.137279 linkml-1.5.1/linkml/generators/projectgen.py
--rw-r--r--   0        0        0     2443 2023-04-25 21:29:56.137279 linkml-1.5.1/linkml/generators/protogen.py
--rw-r--r--   0        0        0    20322 2023-04-25 21:29:56.137279 linkml-1.5.1/linkml/generators/pydanticgen.py
--rw-r--r--   0        0        0    49083 2023-04-25 21:29:56.137279 linkml-1.5.1/linkml/generators/pythongen.py
--rw-r--r--   0        0        0     2825 2023-04-25 21:29:56.137279 linkml-1.5.1/linkml/generators/rdfgen.py
--rw-r--r--   0        0        0     5621 2023-04-25 21:29:56.137279 linkml-1.5.1/linkml/generators/shaclgen.py
--rw-r--r--   0        0        0     9547 2023-04-25 21:29:56.137279 linkml-1.5.1/linkml/generators/shexgen.py
--rw-r--r--   0        0        0     6632 2023-04-25 21:29:56.137279 linkml-1.5.1/linkml/generators/sparqlgen.py
--rw-r--r--   0        0        0      166 2023-04-25 21:29:56.137279 linkml-1.5.1/linkml/generators/sqlalchemy/__init__.py
--rw-r--r--   0        0        0     2575 2023-04-25 21:29:56.137279 linkml-1.5.1/linkml/generators/sqlalchemy/sqlalchemy_declarative_template.py
--rw-r--r--   0        0        0     1625 2023-04-25 21:29:56.137279 linkml-1.5.1/linkml/generators/sqlalchemy/sqlalchemy_imperative_template.py
--rw-r--r--   0        0        0     9334 2023-04-25 21:29:56.137279 linkml-1.5.1/linkml/generators/sqlalchemygen.py
--rw-r--r--   0        0        0    18626 2023-04-25 21:29:56.137279 linkml-1.5.1/linkml/generators/sqlddlgen.py
--rw-r--r--   0        0        0    11387 2023-04-25 21:29:56.137279 linkml-1.5.1/linkml/generators/sqltablegen.py
--rw-r--r--   0        0        0     7177 2023-04-25 21:29:56.137279 linkml-1.5.1/linkml/generators/sssomgen.py
--rw-r--r--   0        0        0     1788 2023-04-25 21:29:56.137279 linkml-1.5.1/linkml/generators/string_template.md
--rw-r--r--   0        0        0     3020 2023-04-25 21:29:56.137279 linkml-1.5.1/linkml/generators/summarygen.py
--rw-r--r--   0        0        0     4760 2023-04-25 21:29:56.137279 linkml-1.5.1/linkml/generators/terminusdbgen.py
--rw-r--r--   0        0        0     5555 2023-04-25 21:29:56.137279 linkml-1.5.1/linkml/generators/typescriptgen.py
--rw-r--r--   0        0        0     1746 2023-04-25 21:29:56.137279 linkml-1.5.1/linkml/generators/yamlgen.py
--rw-r--r--   0        0        0    13311 2023-04-25 21:29:56.137279 linkml-1.5.1/linkml/generators/yumlgen.py
--rw-r--r--   0        0        0        0 2023-04-25 21:29:56.137279 linkml-1.5.1/linkml/linter/__init__.py
--rw-r--r--   0        0        0     3868 2023-04-25 21:29:56.137279 linkml-1.5.1/linkml/linter/cli.py
--rw-r--r--   0        0        0      292 2023-04-25 21:29:56.137279 linkml-1.5.1/linkml/linter/config/datamodel/.linkmllint.yaml
--rw-r--r--   0        0        0        0 2023-04-25 21:29:56.137279 linkml-1.5.1/linkml/linter/config/datamodel/__init__.py
--rw-r--r--   0        0        0    17711 2023-04-25 21:29:56.137279 linkml-1.5.1/linkml/linter/config/datamodel/config.py
--rw-r--r--   0        0        0     6980 2023-04-25 21:29:56.137279 linkml-1.5.1/linkml/linter/config/datamodel/config.yaml
--rw-r--r--   0        0        0      540 2023-04-25 21:29:56.137279 linkml-1.5.1/linkml/linter/config/default.yaml
--rw-r--r--   0        0        0      198 2023-04-25 21:29:56.137279 linkml-1.5.1/linkml/linter/config/recommended.yaml
--rw-r--r--   0        0        0      269 2023-04-25 21:29:56.137279 linkml-1.5.1/linkml/linter/formatters/__init__.py
--rw-r--r--   0        0        0      518 2023-04-25 21:29:56.137279 linkml-1.5.1/linkml/linter/formatters/formatter.py
--rw-r--r--   0        0        0      767 2023-04-25 21:29:56.137279 linkml-1.5.1/linkml/linter/formatters/json_formatter.py
--rw-r--r--   0        0        0     2605 2023-04-25 21:29:56.137279 linkml-1.5.1/linkml/linter/formatters/markdown_formatter.py
--rw-r--r--   0        0        0     1990 2023-04-25 21:29:56.137279 linkml-1.5.1/linkml/linter/formatters/terminal_formatter.py
--rw-r--r--   0        0        0      871 2023-04-25 21:29:56.137279 linkml-1.5.1/linkml/linter/formatters/tsv_formatter.py
--rw-r--r--   0        0        0     3230 2023-04-25 21:29:56.137279 linkml-1.5.1/linkml/linter/linter.py
--rw-r--r--   0        0        0    11658 2023-04-25 21:29:56.137279 linkml-1.5.1/linkml/linter/rules.py
--rw-r--r--   0        0        0       55 2023-04-25 21:29:56.137279 linkml-1.5.1/linkml/reporting/__init__.py
--rw-r--r--   0        0        0     9189 2023-04-25 21:29:56.137279 linkml-1.5.1/linkml/reporting/model.py
--rw-r--r--   0        0        0        0 2023-04-25 21:29:56.137279 linkml-1.5.1/linkml/transformers/__init__.py
--rw-r--r--   0        0        0    18594 2023-04-25 21:29:56.137279 linkml-1.5.1/linkml/transformers/relmodel_transformer.py
--rw-r--r--   0        0        0     5455 2023-04-25 21:29:56.137279 linkml-1.5.1/linkml/transformers/schema_renamer.py
--rw-r--r--   0        0        0        0 2023-04-25 21:29:56.137279 linkml-1.5.1/linkml/utils/__init__.py
--rw-r--r--   0        0        0     6463 2023-04-25 21:29:56.137279 linkml-1.5.1/linkml/utils/converter.py
--rw-r--r--   0        0        0     4384 2023-04-25 21:29:56.137279 linkml-1.5.1/linkml/utils/datautils.py
--rw-r--r--   0        0        0      490 2023-04-25 21:29:56.137279 linkml-1.5.1/linkml/utils/datavalidator.py
--rw-r--r--   0        0        0     6999 2023-04-25 21:29:56.137279 linkml-1.5.1/linkml/utils/execute_tutorial.py
--rw-r--r--   0        0        0    39740 2023-04-25 21:29:56.141280 linkml-1.5.1/linkml/utils/generator.py
--rw-r--r--   0        0        0      445 2023-04-25 21:29:56.141280 linkml-1.5.1/linkml/utils/helpers.py
--rw-r--r--   0        0        0     5773 2023-04-25 21:29:56.141280 linkml-1.5.1/linkml/utils/ifabsent_functions.py
--rw-r--r--   0        0        0     9498 2023-04-25 21:29:56.141280 linkml-1.5.1/linkml/utils/mergeutils.py
--rw-r--r--   0        0        0     4560 2023-04-25 21:29:56.141280 linkml-1.5.1/linkml/utils/rawloader.py
--rw-r--r--   0        0        0     9065 2023-04-25 21:29:56.141280 linkml-1.5.1/linkml/utils/schema_builder.py
--rw-r--r--   0        0        0    13464 2023-04-25 21:29:56.141280 linkml-1.5.1/linkml/utils/schema_fixer.py
--rw-r--r--   0        0        0    48537 2023-04-25 21:29:56.141280 linkml-1.5.1/linkml/utils/schemaloader.py
--rw-r--r--   0        0        0    19733 2023-04-25 21:29:56.141280 linkml-1.5.1/linkml/utils/schemasynopsis.py
--rw-r--r--   0        0        0    16297 2023-04-25 21:29:56.141280 linkml-1.5.1/linkml/utils/sqlutils.py
--rw-r--r--   0        0        0     2395 2023-04-25 21:29:56.141280 linkml-1.5.1/linkml/utils/typereferences.py
--rw-r--r--   0        0        0     1514 2023-04-25 21:29:56.141280 linkml-1.5.1/linkml/utils/validation.py
--rw-r--r--   0        0        0      140 2023-04-25 21:29:56.141280 linkml-1.5.1/linkml/validators/__init__.py
--rw-r--r--   0        0        0     6165 2023-04-25 21:29:56.141280 linkml-1.5.1/linkml/validators/jsonschemavalidator.py
--rw-r--r--   0        0        0     4873 2023-04-25 21:29:56.141280 linkml-1.5.1/linkml/validators/sparqlvalidator.py
--rw-r--r--   0        0        0        0 2023-04-25 21:29:56.141280 linkml-1.5.1/linkml/workspaces/__init__.py
--rw-r--r--   0        0        0        0 2023-04-25 21:29:56.141280 linkml-1.5.1/linkml/workspaces/datamodel/__init__.py
--rw-r--r--   0        0        0    15641 2023-04-25 21:29:56.141280 linkml-1.5.1/linkml/workspaces/datamodel/workspaces.py
--rw-r--r--   0        0        0     4233 2023-04-25 21:29:56.141280 linkml-1.5.1/linkml/workspaces/datamodel/workspaces.yaml
--rw-r--r--   0        0        0    11759 2023-04-25 21:29:56.141280 linkml-1.5.1/linkml/workspaces/example_runner.py
--rw-r--r--   0        0        0     4868 2023-04-25 21:30:31.461436 linkml-1.5.1/pyproject.toml
--rw-r--r--   0        0        0     6564 1970-01-01 00:00:00.000000 linkml-1.5.1/setup.py
--rw-r--r--   0        0        0     3770 1970-01-01 00:00:00.000000 linkml-1.5.1/PKG-INFO
+-rw-r--r--   0        0        0     6555 2023-05-05 00:39:55.714937 linkml-1.5.2/LICENSE
+-rw-r--r--   0        0        0     1369 2023-05-05 00:39:55.714937 linkml-1.5.2/README.md
+-rw-r--r--   0        0        0     3227 2023-05-05 00:39:55.734937 linkml-1.5.2/linkml/__init__.py
+-rw-r--r--   0        0        0      326 2023-05-05 00:39:55.738937 linkml-1.5.2/linkml/_version.py
+-rw-r--r--   0        0        0    51005 2023-05-05 00:39:55.738937 linkml-1.5.2/linkml/generators/PythonGenNotes.md
+-rw-r--r--   0        0        0     3926 2023-05-05 00:39:55.738937 linkml-1.5.2/linkml/generators/README.md
+-rw-r--r--   0        0        0      616 2023-05-05 00:39:55.738937 linkml-1.5.2/linkml/generators/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-05 00:39:55.738937 linkml-1.5.2/linkml/generators/common/__init__.py
+-rw-r--r--   0        0        0     2040 2023-05-05 00:39:55.738937 linkml-1.5.2/linkml/generators/common/type_designators.py
+-rw-r--r--   0        0        0     3118 2023-05-05 00:39:55.738937 linkml-1.5.2/linkml/generators/csvgen.py
+-rw-r--r--   0        0        0     2873 2023-05-05 00:39:55.738937 linkml-1.5.2/linkml/generators/docgen/class.md.jinja2
+-rw-r--r--   0        0        0     2682 2023-05-05 00:39:55.738937 linkml-1.5.2/linkml/generators/docgen/class_diagram.md.jinja2
+-rw-r--r--   0        0        0     1321 2023-05-05 00:39:55.738937 linkml-1.5.2/linkml/generators/docgen/common_metadata.md.jinja2
+-rw-r--r--   0        0        0     1018 2023-05-05 00:39:55.738937 linkml-1.5.2/linkml/generators/docgen/enum.md.jinja2
+-rw-r--r--   0        0        0     1190 2023-05-05 00:39:55.738937 linkml-1.5.2/linkml/generators/docgen/index.md.jinja2
+-rw-r--r--   0        0        0      501 2023-05-05 00:39:55.738937 linkml-1.5.2/linkml/generators/docgen/index.tex.jinja2
+-rw-r--r--   0        0        0       70 2023-05-05 00:39:55.738937 linkml-1.5.2/linkml/generators/docgen/schema.md.jinja2
+-rw-r--r--   0        0        0     2557 2023-05-05 00:39:55.738937 linkml-1.5.2/linkml/generators/docgen/slot.md.jinja2
+-rw-r--r--   0        0        0     1704 2023-05-05 00:39:55.738937 linkml-1.5.2/linkml/generators/docgen/subset.md.jinja2
+-rw-r--r--   0        0        0      635 2023-05-05 00:39:55.738937 linkml-1.5.2/linkml/generators/docgen/type.md.jinja2
+-rw-r--r--   0        0        0    32663 2023-05-05 00:39:55.738937 linkml-1.5.2/linkml/generators/docgen.py
+-rw-r--r--   0        0        0     5112 2023-05-05 00:39:55.738937 linkml-1.5.2/linkml/generators/dotgen.py
+-rw-r--r--   0        0        0    10863 2023-05-05 00:39:55.738937 linkml-1.5.2/linkml/generators/erdiagramgen.py
+-rw-r--r--   0        0        0     6894 2023-05-05 00:39:55.738937 linkml-1.5.2/linkml/generators/excelgen.py
+-rw-r--r--   0        0        0     3575 2023-05-05 00:39:55.738937 linkml-1.5.2/linkml/generators/golrgen.py
+-rw-r--r--   0        0        0     2347 2023-05-05 00:39:55.738937 linkml-1.5.2/linkml/generators/graphqlgen.py
+-rw-r--r--   0        0        0      444 2023-05-05 00:39:55.738937 linkml-1.5.2/linkml/generators/javagen/example_template.java.jinja2
+-rw-r--r--   0        0        0     1737 2023-05-05 00:39:55.738937 linkml-1.5.2/linkml/generators/javagen/java_record_template.jinja2
+-rw-r--r--   0        0        0     5499 2023-05-05 00:39:55.738937 linkml-1.5.2/linkml/generators/javagen.py
+-rw-r--r--   0        0        0     8821 2023-05-05 00:39:55.738937 linkml-1.5.2/linkml/generators/jsonldcontextgen.py
+-rw-r--r--   0        0        0     7952 2023-05-05 00:39:55.738937 linkml-1.5.2/linkml/generators/jsonldgen.py
+-rw-r--r--   0        0        0    22730 2023-05-05 00:39:55.738937 linkml-1.5.2/linkml/generators/jsonschemagen.py
+-rw-r--r--   0        0        0     3555 2023-05-05 00:39:55.738937 linkml-1.5.2/linkml/generators/linkmlgen.py
+-rw-r--r--   0        0        0    34422 2023-05-05 00:39:55.738937 linkml-1.5.2/linkml/generators/markdowngen.py
+-rw-r--r--   0        0        0     6532 2023-05-05 00:39:55.738937 linkml-1.5.2/linkml/generators/namespacegen.py
+-rw-r--r--   0        0        0     6695 2023-05-05 00:39:55.738937 linkml-1.5.2/linkml/generators/oocodegen.py
+-rw-r--r--   0        0        0    27365 2023-05-05 00:39:55.738937 linkml-1.5.2/linkml/generators/owlgen.py
+-rw-r--r--   0        0        0     4911 2023-05-05 00:39:55.738937 linkml-1.5.2/linkml/generators/prefixmapgen.py
+-rw-r--r--   0        0        0     9811 2023-05-05 00:39:55.738937 linkml-1.5.2/linkml/generators/projectgen.py
+-rw-r--r--   0        0        0     2443 2023-05-05 00:39:55.738937 linkml-1.5.2/linkml/generators/protogen.py
+-rw-r--r--   0        0        0    21783 2023-05-05 00:39:55.738937 linkml-1.5.2/linkml/generators/pydanticgen.py
+-rw-r--r--   0        0        0    50389 2023-05-05 00:39:55.738937 linkml-1.5.2/linkml/generators/pythongen.py
+-rw-r--r--   0        0        0     2825 2023-05-05 00:39:55.738937 linkml-1.5.2/linkml/generators/rdfgen.py
+-rw-r--r--   0        0        0     5621 2023-05-05 00:39:55.738937 linkml-1.5.2/linkml/generators/shaclgen.py
+-rw-r--r--   0        0        0     9547 2023-05-05 00:39:55.738937 linkml-1.5.2/linkml/generators/shexgen.py
+-rw-r--r--   0        0        0     6632 2023-05-05 00:39:55.738937 linkml-1.5.2/linkml/generators/sparqlgen.py
+-rw-r--r--   0        0        0      166 2023-05-05 00:39:55.738937 linkml-1.5.2/linkml/generators/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     2575 2023-05-05 00:39:55.738937 linkml-1.5.2/linkml/generators/sqlalchemy/sqlalchemy_declarative_template.py
+-rw-r--r--   0        0        0     1625 2023-05-05 00:39:55.738937 linkml-1.5.2/linkml/generators/sqlalchemy/sqlalchemy_imperative_template.py
+-rw-r--r--   0        0        0     9334 2023-05-05 00:39:55.738937 linkml-1.5.2/linkml/generators/sqlalchemygen.py
+-rw-r--r--   0        0        0    18626 2023-05-05 00:39:55.738937 linkml-1.5.2/linkml/generators/sqlddlgen.py
+-rw-r--r--   0        0        0    11387 2023-05-05 00:39:55.738937 linkml-1.5.2/linkml/generators/sqltablegen.py
+-rw-r--r--   0        0        0     7177 2023-05-05 00:39:55.742937 linkml-1.5.2/linkml/generators/sssomgen.py
+-rw-r--r--   0        0        0     1788 2023-05-05 00:39:55.742937 linkml-1.5.2/linkml/generators/string_template.md
+-rw-r--r--   0        0        0     3020 2023-05-05 00:39:55.742937 linkml-1.5.2/linkml/generators/summarygen.py
+-rw-r--r--   0        0        0     4760 2023-05-05 00:39:55.742937 linkml-1.5.2/linkml/generators/terminusdbgen.py
+-rw-r--r--   0        0        0     5555 2023-05-05 00:39:55.742937 linkml-1.5.2/linkml/generators/typescriptgen.py
+-rw-r--r--   0        0        0     1746 2023-05-05 00:39:55.742937 linkml-1.5.2/linkml/generators/yamlgen.py
+-rw-r--r--   0        0        0    13311 2023-05-05 00:39:55.742937 linkml-1.5.2/linkml/generators/yumlgen.py
+-rw-r--r--   0        0        0        0 2023-05-05 00:39:55.742937 linkml-1.5.2/linkml/linter/__init__.py
+-rw-r--r--   0        0        0     4323 2023-05-05 00:39:55.742937 linkml-1.5.2/linkml/linter/cli.py
+-rw-r--r--   0        0        0      292 2023-05-05 00:39:55.742937 linkml-1.5.2/linkml/linter/config/datamodel/.linkmllint.yaml
+-rw-r--r--   0        0        0        0 2023-05-05 00:39:55.742937 linkml-1.5.2/linkml/linter/config/datamodel/__init__.py
+-rw-r--r--   0        0        0    17711 2023-05-05 00:39:55.742937 linkml-1.5.2/linkml/linter/config/datamodel/config.py
+-rw-r--r--   0        0        0     6980 2023-05-05 00:39:55.742937 linkml-1.5.2/linkml/linter/config/datamodel/config.yaml
+-rw-r--r--   0        0        0      540 2023-05-05 00:39:55.742937 linkml-1.5.2/linkml/linter/config/default.yaml
+-rw-r--r--   0        0        0      198 2023-05-05 00:39:55.742937 linkml-1.5.2/linkml/linter/config/recommended.yaml
+-rw-r--r--   0        0        0      269 2023-05-05 00:39:55.742937 linkml-1.5.2/linkml/linter/formatters/__init__.py
+-rw-r--r--   0        0        0      518 2023-05-05 00:39:55.742937 linkml-1.5.2/linkml/linter/formatters/formatter.py
+-rw-r--r--   0        0        0      767 2023-05-05 00:39:55.742937 linkml-1.5.2/linkml/linter/formatters/json_formatter.py
+-rw-r--r--   0        0        0     2605 2023-05-05 00:39:55.742937 linkml-1.5.2/linkml/linter/formatters/markdown_formatter.py
+-rw-r--r--   0        0        0     2085 2023-05-05 00:39:55.742937 linkml-1.5.2/linkml/linter/formatters/terminal_formatter.py
+-rw-r--r--   0        0        0      871 2023-05-05 00:39:55.742937 linkml-1.5.2/linkml/linter/formatters/tsv_formatter.py
+-rw-r--r--   0        0        0     5004 2023-05-05 00:39:55.742937 linkml-1.5.2/linkml/linter/linter.py
+-rw-r--r--   0        0        0    11649 2023-05-05 00:39:55.742937 linkml-1.5.2/linkml/linter/rules.py
+-rw-r--r--   0        0        0       55 2023-05-05 00:39:55.742937 linkml-1.5.2/linkml/reporting/__init__.py
+-rw-r--r--   0        0        0     9189 2023-05-05 00:39:55.742937 linkml-1.5.2/linkml/reporting/model.py
+-rw-r--r--   0        0        0        0 2023-05-05 00:39:55.742937 linkml-1.5.2/linkml/transformers/__init__.py
+-rw-r--r--   0        0        0    18594 2023-05-05 00:39:55.742937 linkml-1.5.2/linkml/transformers/relmodel_transformer.py
+-rw-r--r--   0        0        0     5455 2023-05-05 00:39:55.742937 linkml-1.5.2/linkml/transformers/schema_renamer.py
+-rw-r--r--   0        0        0        0 2023-05-05 00:39:55.742937 linkml-1.5.2/linkml/utils/__init__.py
+-rw-r--r--   0        0        0     6463 2023-05-05 00:39:55.742937 linkml-1.5.2/linkml/utils/converter.py
+-rw-r--r--   0        0        0     4384 2023-05-05 00:39:55.742937 linkml-1.5.2/linkml/utils/datautils.py
+-rw-r--r--   0        0        0      490 2023-05-05 00:39:55.742937 linkml-1.5.2/linkml/utils/datavalidator.py
+-rw-r--r--   0        0        0     6999 2023-05-05 00:39:55.742937 linkml-1.5.2/linkml/utils/execute_tutorial.py
+-rw-r--r--   0        0        0    39740 2023-05-05 00:39:55.742937 linkml-1.5.2/linkml/utils/generator.py
+-rw-r--r--   0        0        0      445 2023-05-05 00:39:55.742937 linkml-1.5.2/linkml/utils/helpers.py
+-rw-r--r--   0        0        0     5773 2023-05-05 00:39:55.742937 linkml-1.5.2/linkml/utils/ifabsent_functions.py
+-rw-r--r--   0        0        0     9498 2023-05-05 00:39:55.742937 linkml-1.5.2/linkml/utils/mergeutils.py
+-rw-r--r--   0        0        0     4560 2023-05-05 00:39:55.742937 linkml-1.5.2/linkml/utils/rawloader.py
+-rw-r--r--   0        0        0     9065 2023-05-05 00:39:55.742937 linkml-1.5.2/linkml/utils/schema_builder.py
+-rw-r--r--   0        0        0    13464 2023-05-05 00:39:55.742937 linkml-1.5.2/linkml/utils/schema_fixer.py
+-rw-r--r--   0        0        0    48537 2023-05-05 00:39:55.742937 linkml-1.5.2/linkml/utils/schemaloader.py
+-rw-r--r--   0        0        0    19733 2023-05-05 00:39:55.742937 linkml-1.5.2/linkml/utils/schemasynopsis.py
+-rw-r--r--   0        0        0    16297 2023-05-05 00:39:55.742937 linkml-1.5.2/linkml/utils/sqlutils.py
+-rw-r--r--   0        0        0     2395 2023-05-05 00:39:55.742937 linkml-1.5.2/linkml/utils/typereferences.py
+-rw-r--r--   0        0        0     1514 2023-05-05 00:39:55.742937 linkml-1.5.2/linkml/utils/validation.py
+-rw-r--r--   0        0        0      140 2023-05-05 00:39:55.742937 linkml-1.5.2/linkml/validators/__init__.py
+-rw-r--r--   0        0        0     6255 2023-05-05 00:39:55.742937 linkml-1.5.2/linkml/validators/jsonschemavalidator.py
+-rw-r--r--   0        0        0     4873 2023-05-05 00:39:55.742937 linkml-1.5.2/linkml/validators/sparqlvalidator.py
+-rw-r--r--   0        0        0        0 2023-05-05 00:39:55.742937 linkml-1.5.2/linkml/workspaces/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-05 00:39:55.742937 linkml-1.5.2/linkml/workspaces/datamodel/__init__.py
+-rw-r--r--   0        0        0    15641 2023-05-05 00:39:55.742937 linkml-1.5.2/linkml/workspaces/datamodel/workspaces.py
+-rw-r--r--   0        0        0     4233 2023-05-05 00:39:55.742937 linkml-1.5.2/linkml/workspaces/datamodel/workspaces.yaml
+-rw-r--r--   0        0        0    11759 2023-05-05 00:39:55.742937 linkml-1.5.2/linkml/workspaces/example_runner.py
+-rw-r--r--   0        0        0     4868 2023-05-05 00:40:31.907169 linkml-1.5.2/pyproject.toml
+-rw-r--r--   0        0        0     6564 1970-01-01 00:00:00.000000 linkml-1.5.2/setup.py
+-rw-r--r--   0        0        0     3770 1970-01-01 00:00:00.000000 linkml-1.5.2/PKG-INFO
```

### Comparing `linkml-1.5.1/LICENSE` & `linkml-1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `linkml-1.5.1/README.md` & `linkml-1.5.2/README.md`

 * *Files identical despite different names*

### Comparing `linkml-1.5.1/linkml/__init__.py` & `linkml-1.5.2/linkml/__init__.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.1/linkml/generators/PythonGenNotes.md` & `linkml-1.5.2/linkml/generators/PythonGenNotes.md`

 * *Files identical despite different names*

### Comparing `linkml-1.5.1/linkml/generators/README.md` & `linkml-1.5.2/linkml/generators/README.md`

 * *Files identical despite different names*

### Comparing `linkml-1.5.1/linkml/generators/__init__.py` & `linkml-1.5.2/linkml/generators/__init__.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.1/linkml/generators/common/type_designators.py` & `linkml-1.5.2/linkml/generators/common/type_designators.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.1/linkml/generators/csvgen.py` & `linkml-1.5.2/linkml/generators/csvgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.1/linkml/generators/docgen/class.md.jinja2` & `linkml-1.5.2/linkml/generators/docgen/class.md.jinja2`

 * *Files identical despite different names*

### Comparing `linkml-1.5.1/linkml/generators/docgen/class_diagram.md.jinja2` & `linkml-1.5.2/linkml/generators/docgen/class_diagram.md.jinja2`

 * *Files identical despite different names*

### Comparing `linkml-1.5.1/linkml/generators/docgen/common_metadata.md.jinja2` & `linkml-1.5.2/linkml/generators/docgen/common_metadata.md.jinja2`

 * *Files identical despite different names*

### Comparing `linkml-1.5.1/linkml/generators/docgen/enum.md.jinja2` & `linkml-1.5.2/linkml/generators/docgen/enum.md.jinja2`

 * *Files identical despite different names*

### Comparing `linkml-1.5.1/linkml/generators/docgen/index.md.jinja2` & `linkml-1.5.2/linkml/generators/docgen/index.md.jinja2`

 * *Files identical despite different names*

### Comparing `linkml-1.5.1/linkml/generators/docgen/slot.md.jinja2` & `linkml-1.5.2/linkml/generators/docgen/slot.md.jinja2`

 * *Files identical despite different names*

### Comparing `linkml-1.5.1/linkml/generators/docgen/subset.md.jinja2` & `linkml-1.5.2/linkml/generators/docgen/subset.md.jinja2`

 * *Files identical despite different names*

### Comparing `linkml-1.5.1/linkml/generators/docgen/type.md.jinja2` & `linkml-1.5.2/linkml/generators/docgen/type.md.jinja2`

 * *Files identical despite different names*

### Comparing `linkml-1.5.1/linkml/generators/docgen.py` & `linkml-1.5.2/linkml/generators/docgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.1/linkml/generators/dotgen.py` & `linkml-1.5.2/linkml/generators/dotgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.1/linkml/generators/erdiagramgen.py` & `linkml-1.5.2/linkml/generators/erdiagramgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.1/linkml/generators/excelgen.py` & `linkml-1.5.2/linkml/generators/excelgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.1/linkml/generators/golrgen.py` & `linkml-1.5.2/linkml/generators/golrgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.1/linkml/generators/graphqlgen.py` & `linkml-1.5.2/linkml/generators/graphqlgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.1/linkml/generators/javagen/java_record_template.jinja2` & `linkml-1.5.2/linkml/generators/javagen/java_record_template.jinja2`

 * *Files identical despite different names*

### Comparing `linkml-1.5.1/linkml/generators/javagen.py` & `linkml-1.5.2/linkml/generators/javagen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.1/linkml/generators/jsonldcontextgen.py` & `linkml-1.5.2/linkml/generators/jsonldcontextgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.1/linkml/generators/jsonldgen.py` & `linkml-1.5.2/linkml/generators/jsonldgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.1/linkml/generators/jsonschemagen.py` & `linkml-1.5.2/linkml/generators/jsonschemagen.py`

 * *Files 6% similar despite different names*

```diff
@@ -83,22 +83,19 @@
 
         if required:
             if 'required' not in self:
                 self['required'] = []
             
             self['required'].append(canonical_name)
 
-    def add_keyword(self, keyword: str, value: Any, applies_to_all_array_elements: bool = False):
+    def add_keyword(self, keyword: str, value: Any):
         if value is None:
             return
         
-        if applies_to_all_array_elements and self.is_array:
-            self['items'][keyword] = value
-        else:
-            self[keyword] = value
+        self[keyword] = value
 
     @property
     def is_array(self):
         return self.get('type') == 'array'
 
     @property
     def is_object(self):
@@ -237,20 +234,31 @@
                 
                 if if_subschema:
                     inverse_subschema["then"] = if_subschema
 
                 rule_subschemas.append(inverse_subschema)
 
         if len(rule_subschemas) == 1:
-            self.top_level_schema.update(rule_subschemas[0])
+            class_subschema.update(rule_subschemas[0])
         elif len(rule_subschemas) > 1:
-            self.top_level_schema["allOf"] = rule_subschemas
+            if "allOf" not in class_subschema:
+                class_subschema["allOf"] = []
+            class_subschema["allOf"].extend(rule_subschemas)
 
         self.top_level_schema.add_def(cls.name, class_subschema)
 
+        if (
+            self.top_class is not None and camelcase(self.top_class) == camelcase(cls.name)
+        ) or (self.top_class is None and cls.tree_root):
+            for key, value in class_subschema.items():
+                # check this first to ensure we don't overwrite things like additionalProperties
+                # or description on the root. But we do want to copy over properties, required, 
+                # if, then, etc.
+                if key not in self.top_level_schema:
+                    self.top_level_schema[key] = value
 
     def get_subschema_for_anonymous_class(self, cls: AnonymousClassExpression, properties_required: bool = False) -> Union[None, JsonSchema]:
         if not cls:
             return None
 
         subschema = JsonSchema()
         for slot in cls.slot_conditions.values():
@@ -316,14 +324,26 @@
                 reference = descendants
             else:
                 reference = slot.range
         else:
             typ = "string"
 
         return (typ, fmt, reference)
+    
+    def get_value_constraints_for_slot(self, slot: Union[AnonymousSlotExpression, None]) -> JsonSchema:
+        if slot is None:
+            return JsonSchema()
+        
+        constraints = JsonSchema()
+        constraints.add_keyword('pattern', slot.pattern)
+        constraints.add_keyword('minimum', slot.minimum_value)
+        constraints.add_keyword('maximum', slot.maximum_value)
+        constraints.add_keyword('const', slot.equals_string)
+        constraints.add_keyword('const', slot.equals_number)
+        return constraints
 
     def get_subschema_for_slot(self, slot: SlotDefinition, omit_type: bool = False) -> JsonSchema:
         slot_has_range_union = slot.any_of is not None and len(slot.any_of) > 0 and all(s.range is not None for s in slot.any_of)
         if omit_type:
             prop = JsonSchema()
         else:
             slot_is_inlined = self.schemaview.is_inlined(slot)
@@ -347,19 +367,42 @@
                 else:
                     prop = subschema
             else:
                 typ, fmt, reference = self.get_type_info_for_slot_subschema(slot, slot_is_inlined)
                 if slot_is_inlined:
                     # If inline we have to include redefined slots
                     if slot.multivalued:
-                        range_id_slot = self.schemaview.get_identifier_slot(slot.range, use_key=True)
+                        range_id_slot, range_simple_dict_value_slot, range_required_slots = self._get_range_associated_slots(slot)
+                        # if the range class has an ID and the slot is not inlined as a list, then we need to consider
+                        # various inlined as dict formats
                         if range_id_slot is not None and not slot.inlined_as_list:
+                            # At a minimum, the inlined dict can have keys (additionalProps) that are IDs
+                            # and the values are the range class but possibly omitting the ID.
+                            additionalProps = [JsonSchema.ref_for(reference, identifier_optional=True)]
+
+                            # If the range can be collected as a simple dict, then we can also accept the value
+                            # of that simple dict directly.
+                            if range_simple_dict_value_slot is not None:
+                                additionalProps.append(self.get_subschema_for_slot(range_simple_dict_value_slot))
+
+                            # If the range has no required slots, then null is acceptable
+                            if len(range_required_slots) == 0:
+                                additionalProps.append(JsonSchema({"type": "null"}))
+
+                            # If through the above logic we identified multiple acceptable forms, then wrap them
+                            # in an "anyOf", otherwise just take the only acceptable form
+                            if len(additionalProps) == 1:
+                                additionalProps = additionalProps[0]
+                            else:
+                                additionalProps = JsonSchema({
+                                    "anyOf": additionalProps
+                                })
                             prop = JsonSchema({
                                 "type": "object",
-                                "additionalProperties": JsonSchema.ref_for(reference, identifier_optional=True)
+                                "additionalProperties": additionalProps
                             })
                             self.top_level_schema.add_lax_def(reference, self.aliased_slot_name(range_id_slot))
                         else:
                             prop = JsonSchema.array_of(JsonSchema.ref_for(reference))
                     else:
                         prop = JsonSchema.ref_for(reference)
                 else:
@@ -376,23 +419,27 @@
                         elif fmt is None:
                             prop = JsonSchema({"type": typ})
                         else:
                             prop = JsonSchema({"type": typ, "format": fmt})
 
         prop.add_keyword('description', slot.description)
 
-        prop.add_keyword('pattern', slot.pattern, applies_to_all_array_elements=True)
-        prop.add_keyword('minimum', slot.minimum_value, applies_to_all_array_elements=True)
-        prop.add_keyword('maximum', slot.maximum_value, applies_to_all_array_elements=True)
-        prop.add_keyword('const', slot.equals_string, applies_to_all_array_elements=True)
-        prop.add_keyword('const', slot.equals_number, applies_to_all_array_elements=True)
+        own_constraints = self.get_value_constraints_for_slot(slot)
 
         if prop.is_array:
+            all_element_constraints = self.get_value_constraints_for_slot(slot.all_members)
+            any_element_constraints = self.get_value_constraints_for_slot(slot.has_member)
             prop.add_keyword('minItems', slot.minimum_cardinality)
             prop.add_keyword('maxItems', slot.maximum_cardinality)
+            prop["items"].update(own_constraints)
+            prop["items"].update(all_element_constraints)
+            if any_element_constraints:
+                prop["contains"] = any_element_constraints
+        else:
+            prop.update(own_constraints)
 
         if prop.is_object:
             prop.add_keyword('minProperties', slot.minimum_cardinality)
             prop.add_keyword('maxProperties', slot.maximum_cardinality)
 
         if slot.any_of is not None and len(slot.any_of) > 0:
             if not slot_has_range_union:
@@ -416,28 +463,43 @@
         class_id_slot = self.schemaview.get_identifier_slot(cls.name, use_key=True)
         slot_is_required = slot.required or slot == class_id_slot
 
         aliased_slot_name = self.aliased_slot_name(slot)
         prop = self.get_subschema_for_slot(slot)
         subschema.add_property(aliased_slot_name, prop, slot_is_required)
 
-        if (
-            self.top_class is not None and camelcase(self.top_class) == camelcase(cls.name)
-        ) or (self.top_class is None and cls.tree_root):
-            self.top_level_schema.add_property(aliased_slot_name, prop, slot_is_required)
-
     def serialize(self, **kwargs) -> str:
         self.start_schema()
         for enum_definition in self.schemaview.all_enums().values():
             self.handle_enum(enum_definition)
 
         for class_definition in self.schemaview.all_classes().values():
             self.handle_class(class_definition)
 
         return self.top_level_schema.to_json(sort_keys=True, indent=self.indent if self.indent > 0 else None)
+    
+    def _get_range_associated_slots(self, slot: SlotDefinition) -> Tuple[Union[SlotDefinition, None], Union[SlotDefinition, None], Union[List[SlotDefinition], None]]:
+        range_class = self.schemaview.get_class(slot.range)
+        if range_class is None:
+            return None, None, None
+        
+        range_class_id_slot = self.schemaview.get_identifier_slot(range_class.name, use_key=True)
+        if range_class_id_slot is None:
+            return None, None, None
+        
+        non_id_slots = [
+            s for s in self.schemaview.class_induced_slots(range_class.name) if s.name != range_class_id_slot.name
+        ]
+        non_id_required_slots = [s for s in non_id_slots if s.required]
+
+        range_simple_dict_value_slot = None
+        if len(non_id_slots) == 1:
+            range_simple_dict_value_slot = non_id_slots[0]
+        
+        return range_class_id_slot, range_simple_dict_value_slot, non_id_required_slots
 
 
 @shared_arguments(JsonSchemaGenerator)
 @click.command()
 @click.option(
     "-i",
     "--inline",
```

### Comparing `linkml-1.5.1/linkml/generators/linkmlgen.py` & `linkml-1.5.2/linkml/generators/linkmlgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.1/linkml/generators/markdowngen.py` & `linkml-1.5.2/linkml/generators/markdowngen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.1/linkml/generators/namespacegen.py` & `linkml-1.5.2/linkml/generators/namespacegen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.1/linkml/generators/oocodegen.py` & `linkml-1.5.2/linkml/generators/oocodegen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.1/linkml/generators/owlgen.py` & `linkml-1.5.2/linkml/generators/owlgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.1/linkml/generators/prefixmapgen.py` & `linkml-1.5.2/linkml/generators/prefixmapgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.1/linkml/generators/projectgen.py` & `linkml-1.5.2/linkml/generators/projectgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.1/linkml/generators/protogen.py` & `linkml-1.5.2/linkml/generators/protogen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.1/linkml/generators/pydanticgen.py` & `linkml-1.5.2/linkml/generators/pydanticgen.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 import os
+import logging
 from collections import defaultdict
 from copy import deepcopy
-from dataclasses import field, dataclass
-from typing import Dict, List, TextIO, Union, Optional, Set
-from linkml.utils.ifabsent_functions import ifabsent_value_declaration
+from dataclasses import dataclass, field
+from typing import Dict, List, Optional, Set, TextIO, Union
 
 import click
 from jinja2 import Template
 # from linkml.generators import pydantic_GEN_VERSION
-from linkml_runtime.linkml_model.meta import (Annotation, ClassDefinition,
-                                              EnumDefinition,
+from linkml_runtime.linkml_model.meta import (Annotation,
+                                              AnonymousSlotExpression,
+                                              ClassDefinition, EnumDefinition,
                                               EnumDefinitionName,
-                                              SchemaDefinition, TypeDefinition, AnonymousSlotExpression, SlotDefinition)
+                                              SchemaDefinition, SlotDefinition,
+                                              TypeDefinition)
 from linkml_runtime.utils.formatutils import camelcase, underscore
 from linkml_runtime.utils.schemaview import SchemaView
 
-from linkml.generators.common.type_designators import get_type_designator_value, get_accepted_type_designator_values
 from linkml._version import __version__
+from linkml.generators.common.type_designators import (
+    get_accepted_type_designator_values, get_type_designator_value)
 from linkml.generators.oocodegen import OOCodeGenerator
 from linkml.utils.generator import shared_arguments
+from linkml.utils.ifabsent_functions import ifabsent_value_declaration
 
 default_template = """
 {#-
 
   Jinja2 Template for a pydantic classes
 -#}
 from __future__ import annotations
@@ -33,22 +37,23 @@
 from linkml_runtime.linkml_model import Decimal
 
 metamodel_version = "{{metamodel_version}}"
 version = "{{version if version else None}}"
 
 class WeakRefShimBaseModel(BaseModel):
    __slots__ = '__weakref__'
-    
+
 class ConfiguredBaseModel(WeakRefShimBaseModel,
-                validate_assignment = True, 
-                validate_all = True, 
-                underscore_attrs_are_private = True, 
-                extra = {% if allow_extra %}'allow'{% else %}'forbid'{% endif %}, 
-                arbitrary_types_allowed = True):
-    pass                    
+                validate_assignment = True,
+                validate_all = True,
+                underscore_attrs_are_private = True,
+                extra = {% if allow_extra %}'allow'{% else %}'forbid'{% endif %},
+                arbitrary_types_allowed = True,
+                use_enum_values = True):
+    pass
 
 {% for e in enums.values() %}
 class {{ e.name }}(str, Enum):
     {% if e.description -%}
     \"\"\"
     {{ e.description }}
     \"\"\"
@@ -58,47 +63,47 @@
     {% endfor %}
     {% if not e['values'] -%}
     dummy = "dummy"
     {% endif %}
 {% endfor %}
 
 {%- for c in schema.classes.values() %}
-class {{ c.name }} 
+class {{ c.name }}
     {%- if class_isa_plus_mixins[c.name] -%}
         ({{class_isa_plus_mixins[c.name]|join(', ')}})
     {%- else -%}
         (ConfiguredBaseModel)
-    {%- endif -%}                   
+    {%- endif -%}
                   :
-    {% if c.description -%}    
+    {% if c.description -%}
     \"\"\"
     {{ c.description }}
     \"\"\"
     {%- endif %}
     {% for attr in c.attributes.values() if c.attributes -%}
     {{attr.name}}: {{ attr.annotations['python_range'].value }} = Field(
-    {%- if predefined_slot_values[c.name][attr.name] -%} 
+    {%- if predefined_slot_values[c.name][attr.name] -%}
         {{ predefined_slot_values[c.name][attr.name] }}
     {%- else -%}
         None
-    {%- endif -%}    
+    {%- endif -%}
     {%- if attr.title != None %}, title="{{attr.title}}"{% endif -%}
     {%- if attr.description %}, description=\"\"\"{{attr.description}}\"\"\"{% endif -%}
     {%- if attr.minimum_value != None %}, ge={{attr.minimum_value}}{% endif -%}
     {%- if attr.maximum_value != None %}, le={{attr.maximum_value}}{% endif -%}
     )
     {% else -%}
     None
     {% endfor %}
 
 {% endfor %}
 
 # Update forward refs
 # see https://pydantic-docs.helpmanual.io/usage/postponed_annotations/
-{% for c in schema.classes.values() -%} 
+{% for c in schema.classes.values() -%}
 {{ c.name }}.update_forward_refs()
 {% endfor %}
 """
 
 
 def _get_pyrange(t: TypeDefinition, sv: SchemaView) -> str:
     pyrange = t.repr if t is not None else None
@@ -135,26 +140,25 @@
 
     # ObjectVars (identical to pythongen)
     gen_classvars: bool = field(default_factory=lambda: True)
     gen_slots: bool = field(default_factory=lambda: True)
     genmeta: bool = field(default_factory=lambda: False)
     emit_metadata: bool = field(default_factory=lambda: True)
 
-
     def generate_enums(
         self, all_enums: Dict[EnumDefinitionName, EnumDefinition]
     ) -> Dict[str, dict]:
         # TODO: make an explicit class to represent how an enum is passed to the template
         enums = {}
-        for enum_name, enum_orignal in all_enums.items():
+        for enum_name, enum_original in all_enums.items():
             enum = {"name": camelcase(enum_name), "values": {}}
 
-            for pv in enum_orignal.permissible_values.values():
+            for pv in enum_original.permissible_values.values():
                 label = self.generate_enum_label(pv.text)
-                enum["values"][label] = pv.text
+                enum["values"][label] = pv.text.replace('"', '\\"')
 
             enums[enum_name] = enum
 
         return enums
 
     def sort_classes(self, clist: List[ClassDefinition]) -> List[ClassDefinition]:
         """
@@ -191,47 +195,55 @@
         return slist
 
     def get_predefined_slot_values(self) -> Dict[str, Dict[str, str]]:
         """
         :return: Dictionary of dictionaries with predefined slot values for each class
         """
         sv = self.schemaview
-        default_prefix = sv.schema.default_prefix
         slot_values = defaultdict(dict)
         for class_def in sv.all_classes().values():
-
             for slot_name in sv.class_slots(class_def.name):
                 slot = sv.induced_slot(slot_name, class_def.name)
                 if slot.designates_type:
                     target_value = get_type_designator_value(sv, slot, class_def)
                     slot_values[camelcase(class_def.name)][
                         slot.name
                     ] = f'"{target_value}"'
                     if slot.multivalued:
                         slot_values[camelcase(class_def.name)][slot.name] = (
                             "["
                             + slot_values[camelcase(class_def.name)][slot.name]
                             + "]"
                         )
-                    slot_values[camelcase(class_def.name)][slot.name] = slot_values[camelcase(class_def.name)][slot.name]
+                    slot_values[camelcase(class_def.name)][slot.name] = slot_values[
+                        camelcase(class_def.name)
+                    ][slot.name]
                 elif slot.ifabsent is not None:
-                    value = ifabsent_value_declaration(slot.ifabsent, sv, class_def, slot)
+                    value = ifabsent_value_declaration(
+                        slot.ifabsent, sv, class_def, slot
+                    )
                     slot_values[camelcase(class_def.name)][slot.name] = value
                 # Multivalued slots that are either not inlined (just an identifier) or are
                 # inlined as lists should get default_factory list, if they're inlined but
                 # not as a list, that means a dictionary
                 elif slot.multivalued:
                     has_identifier_slot = self.range_class_has_identifier_slot(slot)
 
-                    if slot.inlined and not slot.inlined_as_list and has_identifier_slot:
-                        slot_values[camelcase(class_def.name)][slot.name] = "default_factory=dict"
+                    if (
+                        slot.inlined
+                        and not slot.inlined_as_list
+                        and has_identifier_slot
+                    ):
+                        slot_values[camelcase(class_def.name)][
+                            slot.name
+                        ] = "default_factory=dict"
                     else:
-                        slot_values[camelcase(class_def.name)][slot.name] = "default_factory=list"
-
-
+                        slot_values[camelcase(class_def.name)][
+                            slot.name
+                        ] = "default_factory=list"
 
         return slot_values
 
     def range_class_has_identifier_slot(self, slot):
         """
         Check if the range class of a slot has an identifier slot, via both slot.any_of and slot.range
         Should return False if the range is not a class, and also if the range is a class but has no
@@ -241,17 +253,23 @@
         :return: bool
         """
         sv = self.schemaview
         has_identifier_slot = False
         if slot.any_of:
             for slot_range in slot.any_of:
                 any_of_range = slot_range.range
-                if any_of_range in sv.all_classes() and sv.get_identifier_slot(any_of_range) is not None:
+                if (
+                    any_of_range in sv.all_classes()
+                    and sv.get_identifier_slot(any_of_range, use_key=True) is not None
+                ):
                     has_identifier_slot = True
-        if slot.range in sv.all_classes() and sv.get_identifier_slot(slot.range) is not None:
+        if (
+            slot.range in sv.all_classes()
+            and sv.get_identifier_slot(slot.range, use_key=True) is not None
+        ):
             has_identifier_slot = True
         return has_identifier_slot
 
     def get_class_isa_plus_mixins(self) -> Dict[str, List[str]]:
         """
         Generate the inheritance list for each class from is_a plus mixins
         :return:
@@ -283,30 +301,46 @@
         if len(id_ranges) == 0:
             return None
         elif len(id_ranges) == 1:
             return id_ranges[0]
         else:
             return f"Union[{'.'.join(id_ranges)}]"
 
-    def get_class_slot_range(self, slot_range: str, inlined: bool, inlined_as_list: bool) -> str:
+    def get_class_slot_range(
+        self, slot_range: str, inlined: bool, inlined_as_list: bool
+    ) -> str:
         sv = self.schemaview
         range_cls = sv.get_class(slot_range)
 
         # Hardcoded handling for Any
         if range_cls.class_uri == "linkml:Any":
             return "Any"
 
         # Inline the class itself only if the class is defined as inline, or if the class has no
         # identifier slot and also isn't a mixin.
-        if inlined or inlined_as_list or (
-            sv.get_identifier_slot(range_cls.name) is None
-            and not sv.is_mixin(range_cls.name)
+        if (
+            inlined
+            or inlined_as_list
+            or (
+                sv.get_identifier_slot(range_cls.name, use_key=True) is None
+                and not sv.is_mixin(range_cls.name)
+            )
         ):
-            if len([x for x in sv.class_induced_slots(slot_range) if x.designates_type]) > 0 and len(sv.class_descendants(slot_range)) > 1:
-                return f"Union[" + ",".join([camelcase(c) for c in sv.class_descendants(slot_range)]) + "]"
+            if (
+                len(
+                    [x for x in sv.class_induced_slots(slot_range) if x.designates_type]
+                )
+                > 0
+                and len(sv.class_descendants(slot_range)) > 1
+            ):
+                return (
+                    f"Union["
+                    + ",".join([camelcase(c) for c in sv.class_descendants(slot_range)])
+                    + "]"
+                )
             else:
                 return f"{camelcase(slot_range)}"
 
         # For the more difficult cases, set string as the default and attempt to improve it
         range_cls_identifier_slot_range = "str"
 
         # For mixins, try to use the identifier slot of descendant classes
@@ -324,65 +358,92 @@
         ):
             range_cls_identifier_slot_range = _get_pyrange(
                 sv.get_type(sv.get_identifier_slot(range_cls.name).range), sv
             )
 
         return range_cls_identifier_slot_range
 
-    def generate_python_range(self, slot_range, slot_def:SlotDefinition, class_def:ClassDefinition) -> str:
+    def generate_python_range(
+        self, slot_range, slot_def: SlotDefinition, class_def: ClassDefinition
+    ) -> str:
         """
         Generate the python range for a slot range value
         """
         sv = self.schemaview
 
         if slot_def.designates_type:
-            pyrange = "Literal[" + ",".join(
-                ["\"" + x + "\"" for x in get_accepted_type_designator_values(sv, slot_def, class_def)]) + "]"
+            pyrange = (
+                "Literal["
+                + ",".join(
+                    [
+                        '"' + x + '"'
+                        for x in get_accepted_type_designator_values(
+                            sv, slot_def, class_def
+                        )
+                    ]
+                )
+                + "]"
+            )
         elif slot_range in sv.all_classes():
-            pyrange = self.get_class_slot_range(slot_range, inlined=slot_def.inlined, inlined_as_list=slot_def.inlined_as_list)
+            pyrange = self.get_class_slot_range(
+                slot_range,
+                inlined=slot_def.inlined,
+                inlined_as_list=slot_def.inlined_as_list,
+            )
         elif slot_range in sv.all_enums():
             pyrange = f"{camelcase(slot_range)}"
         elif slot_range in sv.all_types():
             t = sv.get_type(slot_range)
             pyrange = _get_pyrange(t, sv)
         elif slot_range is None:
             pyrange = "str"
         else:
             # TODO: default ranges in schemagen
             # pyrange = 'str'
             # logging.error(f'range: {s.range} is unknown')
             raise Exception(f"range: {slot_range}")
         return pyrange
 
-    def generate_collection_key(self, slot_ranges: List[str], slot_def: SlotDefinition, class_def: ClassDefinition) -> Optional[str]:
+    def generate_collection_key(
+        self,
+        slot_ranges: List[str],
+        slot_def: SlotDefinition,
+        class_def: ClassDefinition,
+    ) -> Optional[str]:
         """
         Find the python range value (str, int, etc) for the identifier slot
         of a class used as a slot range.
 
         If a pyrange value matches a class name, the range of the identifier slot
         will be returned. If more than one match is found and they don't match,
         an exception will be raised.
 
         :param slot_ranges: list of python range values
         """
 
-        collection_keys:Set[str] = set()
+        collection_keys: Set[str] = set()
 
         if slot_ranges is None:
             return None
 
         for slot_range in slot_ranges:
             if slot_range is None or slot_range not in self.schemaview.all_classes():
-                continue # ignore non-class ranges
+                continue  # ignore non-class ranges
 
-            identifier_slot = self.schemaview.get_identifier_slot(slot_range)
+            identifier_slot = self.schemaview.get_identifier_slot(slot_range, use_key=True)
             if identifier_slot is not None:
-                collection_keys.add(self.generate_python_range(identifier_slot.range, slot_def, class_def))
+                collection_keys.add(
+                    self.generate_python_range(
+                        identifier_slot.range, slot_def, class_def
+                    )
+                )
         if len(collection_keys) > 1:
-            raise Exception(f"Slot with any_of range has multiple identifier slot range types: {collection_keys}")
+            raise Exception(
+                f"Slot with any_of range has multiple identifier slot range types: {collection_keys}"
+            )
         if len(collection_keys) == 1:
             return list(collection_keys)[0]
         return None
 
     def serialize(self) -> str:
         sv = self.schemaview
 
@@ -394,15 +455,17 @@
 
         sv: SchemaView
         sv = self.schemaview
         schema = sv.schema
         pyschema = SchemaDefinition(
             id=schema.id,
             name=schema.name,
-            description=schema.description.replace('"', '\\"') if schema.description else None,
+            description=schema.description.replace('"', '\\"')
+            if schema.description
+            else None,
         )
         enums = self.generate_enums(sv.all_enums())
 
         sorted_classes = self.sort_classes(list(sv.all_classes().values()))
         self.sorted_class_names = [camelcase(c.name) for c in sorted_classes]
 
         # Don't want to generate classes when class_uri is linkml:Any, will
@@ -427,44 +490,54 @@
                 s = deepcopy(sv.induced_slot(sn, class_name))
                 # logging.error(f'Induced slot {class_name}.{sn} == {s.name} {s.range}')
                 s.name = underscore(s.name)
                 if s.description:
                     s.description = s.description.replace('"', '\\"')
                 class_def.attributes[s.name] = s
 
-                slot_ranges:List[str] = []
+                slot_ranges: List[str] = []
 
                 if len(s.any_of) > 0 and s.range is not None:
                     raise ValueError("Slot cannot have both range and any_of defined")
 
                 if s.any_of is not None and len(s.any_of) > 0:
                     # list comprehension here is pulling ranges from within AnonymousSlotExpression
                     slot_ranges.extend([r.range for r in s.any_of])
                 else:
                     slot_ranges.append(s.range)
 
-                pyranges = [self.generate_python_range(slot_range, s, class_def)
-                            for slot_range in slot_ranges]
+                pyranges = [
+                    self.generate_python_range(slot_range, s, class_def)
+                    for slot_range in slot_ranges
+                ]
 
-                pyranges = list(set(pyranges)) # remove duplicates
+                pyranges = list(set(pyranges))  # remove duplicates
                 pyranges.sort()
 
                 if len(pyranges) == 1:
                     pyrange = pyranges[0]
                 elif len(pyranges) > 1:
                     pyrange = f"Union[{', '.join(pyranges)}]"
                 else:
-                    raise Exception(f"Could not generate python range for {class_name}.{s.name}")
+                    raise Exception(
+                        f"Could not generate python range for {class_name}.{s.name}"
+                    )
 
                 if s.multivalued:
                     if s.inlined or s.inlined_as_list:
-                        collection_key = self.generate_collection_key(slot_ranges, s, class_def)
+                        collection_key = self.generate_collection_key(
+                            slot_ranges, s, class_def
+                        )
                     else:
                         collection_key = None
-                    if s.inlined == False or collection_key is None or s.inlined_as_list == True:
+                    if (
+                        s.inlined == False
+                        or collection_key is None
+                        or s.inlined_as_list == True
+                    ):
                         pyrange = f"List[{pyrange}]"
                     else:
                         pyrange = f"Dict[{collection_key}, {pyrange}]"
                 if not s.required and not s.designates_type:
                     pyrange = f"Optional[{pyrange}]"
                 ann = Annotation("python_range", pyrange)
                 s.annotations[ann.tag] = ann
@@ -477,15 +550,15 @@
             metamodel_version=self.schema.metamodel_version,
             version=self.schema.version,
             class_isa_plus_mixins=self.get_class_isa_plus_mixins(),
         )
         return code
 
     def default_value_for_type(self, typ: str) -> str:
-        return 'None'
+        return "None"
 
 
 @shared_arguments(PydanticGenerator)
 @click.option(
     "--template_file", help="Optional jinja2 template to use for class generation"
 )
 @click.version_option(__version__, "-V", "--version")
```

### Comparing `linkml-1.5.1/linkml/generators/pythongen.py` & `linkml-1.5.2/linkml/generators/pythongen.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 import keyword
 import logging
 import os
 import re
 from dataclasses import dataclass, field
 from types import ModuleType
-from typing import (Callable, Dict, Iterator, List, Optional, Set, TextIO,
-                    Tuple, Union)
+from typing import Callable, Dict, Iterator, List, Optional, Set, Tuple, Union
 
 import click
 from linkml_runtime.linkml_model import linkml_files
 from linkml_runtime.linkml_model.meta import (ClassDefinition,
-                                              ClassDefinitionName, Definition,
+                                              ClassDefinitionName,
                                               DefinitionName, Element,
                                               EnumDefinition, PermissibleValue,
-                                              SchemaDefinition, SlotDefinition,
+                                              SlotDefinition,
                                               SlotDefinitionName,
                                               TypeDefinition)
 from linkml_runtime.utils.compile_python import compile_python
-from linkml_runtime.utils.formatutils import (be, camelcase, sfx, split_line,
+from linkml_runtime.utils.formatutils import (be, camelcase, sfx, split_col,
                                               underscore, wrapped_annotation)
 from linkml_runtime.utils.metamodelcore import builtinnames
 from rdflib import URIRef
 
 import linkml
 from linkml._version import __version__
 from linkml.generators import PYTHON_GEN_VERSION
@@ -55,15 +54,15 @@
     def __post_init__(self) -> None:
         self.sourcefile = self.schema
         super().__post_init__()
         if self.format is None:
             self.format = self.valid_formats[0]
         if self.schema.default_prefix == "linkml" and not self.genmeta:
             logging.error(
-                f"Generating metamodel without --genmeta is highly inadvised!"
+                f"Generating metamodel without --genmeta is highly inadvisable!"
             )
         if (
             not self.schema.source_file
             and isinstance(self.sourcefile, str)
             and "\n" not in self.sourcefile
         ):
             self.schema.source_file = os.path.basename(self.sourcefile)
@@ -123,33 +122,34 @@
             ""
             if self.genmeta
             else "from linkml_runtime.linkml_model.meta import EnumDefinition, PermissibleValue, PvFormulaOptions\n"
         )
         handlerimport = (
             "from linkml_runtime.utils.enumerations import EnumDefinitionImpl"
         )
-        split_descripton = "\n#              ".join(
-            split_line(be(self.schema.description), split_len=100)
-        )
+        split_description = ""
+        if self.schema.description:
+            split_description = "\n#   ".join(
+                d for d in self.schema.description.split("\n") if d is not None
+            )
         head = (
             f"""# Auto generated from {self.schema.source_file} by {self.generatorname} version: {self.generatorversion}
 # Generation date: {self.schema.generation_date}
 # Schema: {self.schema.name}
 #"""
             if self.emit_metadata and self.schema.generation_date
             else ""
         )
 
         return f"""{head}
 # id: {self.schema.id}
-# description: {split_descripton}
+# description: {split_description}
 # license: {be(self.schema.license)}
 
 import dataclasses
-import sys
 import re
 from jsonasobj2 import JsonObj, as_dict
 from typing import Optional, List, Union, Dict, ClassVar, Any
 from dataclasses import dataclass
 {enumimports}
 from linkml_runtime.utils.slot import Slot
 from linkml_runtime.utils.metamodelcore import empty_list, empty_dict, bnode
@@ -297,16 +297,14 @@
                         if self.class_identifier(parent):
                             rval.add_entry(
                                 parent.imported_from,
                                 self.class_identifier_path(parent, False)[-1],
                             )
                 for slotname in cls.slots:
                     add_slot_range(self.schema.slots[slotname])
-                # for slotname in cls.slot_usage:
-                #     add_slot_range(self.schema.slots[slotname])
 
         return rval.values()
 
     def gen_namespaces(self) -> str:
         dflt_prefix = default_curie_or_uri(self)
         dflt = (
             f"CurieNamespace('', '{sfx(dflt_prefix)}')"
@@ -358,44 +356,54 @@
                         rval.append(f"class {classname}({parent_cls}):\n\tpass")
                         break  # We only do the first primary key
         return "\n\n\n".join(rval)
 
     def gen_typedefs(self) -> str:
         """Generate python type declarations for all defined types"""
         rval = []
-        defs_to_generate = [x for x in self.schema.types.values() if not x.imported_from]
+        defs_to_generate = [
+            x for x in self.schema.types.values() if not x.imported_from
+        ]
         emitted_types = []
         ## all imported_from types are already considered generated
-        emitted_types.extend([x.name for x in self.schema.types.values() if x.imported_from])
+        emitted_types.extend(
+            [x.name for x in self.schema.types.values() if x.imported_from]
+        )
         for typ in [x for x in defs_to_generate if not x.typeof]:
-            typname = camelcase(typ.name)
-            desc = f'\n\t""" {typ.description} """' if typ.description else ""
-            base_base = typ.base.rsplit(".")[-1]
-            rval.append(
-                f"class {typname}({base_base}):{desc}\n\t{self.gen_type_meta(typ)}\n\n"
-            )
-            emitted_types.append(typ.name)
+            self._gen_typedef(typ, typ.base.rsplit(".")[-1], rval, emitted_types)
 
         while True:
-            defs_to_generate_typeof = [x for x in defs_to_generate if x.typeof and not x.name in emitted_types]
+            defs_to_generate_typeof = [
+                x for x in defs_to_generate if x.typeof and not x.name in emitted_types
+            ]
             if len(defs_to_generate_typeof) == 0:
                 break
-            defs_can_generate = [x for x in defs_to_generate_typeof if x.typeof in emitted_types ]
+            defs_can_generate = [
+                x for x in defs_to_generate_typeof if x.typeof in emitted_types
+            ]
             if len(defs_can_generate) == 0:
-                raise ValueError(f"Can not generate type definition for {[f'{x.name} of {x.typeof}' for x in defs_to_generate_typeof]}. Forgot a link in the type hierarchy chain ?")
-            for typ in defs_can_generate:
-                typname = camelcase(typ.name)
-                desc = f'\n\t""" {typ.description} """' if typ.description else ""
-                parent_typename = camelcase(typ.typeof)
-                rval.append(
-                    f"class {typname}({parent_typename}):{desc}\n\t{self.gen_type_meta(typ)}\n\n"
+                raise ValueError(
+                    f"Cannot generate type definition for {[f'{x.name} of {x.typeof}' for x in defs_to_generate_typeof]}. Forgot a link in the type hierarchy chain?"
                 )
-                emitted_types.append(typ.name)
+            for typ in defs_can_generate:
+                self._gen_typedef(typ, camelcase(typ.typeof), rval, emitted_types)
+
         return "\n".join(rval)
 
+    def _gen_typedef(self, typ, superclass, rval, emitted_types):
+        typname = camelcase(typ.name)
+        desc = ""
+        if typ.description:
+            description = typ.description.replace('"""', "---")
+            desc = f'\n\t""" {description} """'
+        rval.append(
+            f"class {typname}({superclass}):{desc}\n\t{self.gen_type_meta(typ)}\n\n"
+        )
+        emitted_types.append(typ.name)
+
     def gen_classdefs(self) -> str:
         """Create class definitions for all non-mixin classes in the model
         Note that apply_to classes are transformed to mixins
         """
         clist = self._sort_classes(self.schema.classes.values())
         return "\n".join([self.gen_classdef(v) for v in clist if not v.imported_from])
 
@@ -493,21 +501,21 @@
         )
         if ":/" in type_model_uri:
             type_model_uri = f'URIRef("{type_model_uri}")'
         else:
             ns, ln = type_model_uri.split(":", 1)
             ln_suffix = f".{ln}" if ln.isidentifier() else f'["{ln}"]'
             type_model_uri = f"{ns.upper()}{ln_suffix}"
-        vars = [
+        type_meta = [
             f"type_class_uri = {type_class_uri}",
             f"type_class_curie = {type_class_curie}",
             f'type_name = "{typ.name}"',
             f"type_model_uri = {type_model_uri}",
         ]
-        return "\n\t".join(vars)
+        return "\n\t".join(type_meta)
 
     def gen_class_variables(self, cls: ClassDefinition) -> str:
         """
         Generate the variable declarations for a dataclass.
 
         :param cls: class containing variables to be rendered in inheritence hierarchy
         :return: variable declarations for target class and its ancestors
@@ -935,32 +943,38 @@
         if len(cidpath) < 2:
             return cidpath[0]
         else:
             return f"Union[{cidpath[0]}, {cidpath[-1]}]"
 
     def forward_reference(self, slot_range: str, owning_class: str) -> bool:
         """Determine whether slot_range is a forward reference"""
-        #logging.info(f"CHECKING: {slot_range} {owning_class}")
+        # logging.info(f"CHECKING: {slot_range} {owning_class}")
         if (
             slot_range in self.schema.classes
             and self.schema.classes[slot_range].imported_from
         ) or (
             slot_range in self.schema.enums
             and self.schema.enums[slot_range].imported_from
         ):
-            logging.info(f"FALSE: FORWARD: {slot_range} {owning_class} // IMP={self.schema.classes[slot_range].imported_from}")
+            logging.info(
+                f"FALSE: FORWARD: {slot_range} {owning_class} // IMP={self.schema.classes[slot_range].imported_from}"
+            )
             return False
         if slot_range in self.schema.enums:
             return True
         for cname in self.schema.classes:
             if cname == owning_class:
-                logging.info(f"TRUE: OCCURS SAME: {cname} == {slot_range} owning: {owning_class}")
+                logging.info(
+                    f"TRUE: OCCURS SAME: {cname} == {slot_range} owning: {owning_class}"
+                )
                 return True  # Occurs on or after
             elif cname == slot_range:
-                logging.info(f"FALSE: OCCURS BEFORE: {cname} == {slot_range} owning: {owning_class}")
+                logging.info(
+                    f"FALSE: OCCURS BEFORE: {cname} == {slot_range} owning: {owning_class}"
+                )
                 return False  # Occurs before
         return True
 
     def python_uri_for(
         self, uriorcurie: Union[str, URIRef]
     ) -> Tuple[str, Optional[str]]:
         """Return the python form of uriorcurie
@@ -1037,58 +1051,47 @@
                 self.gen_enum(enum)
                 for enum in self.schema.enums.values()
                 if not enum.imported_from
             ]
         )
 
     def gen_enum(self, enum: EnumDefinition) -> str:
+        """
+        Generate an enum class
+        @param enum: EnumDefinition object to be converted into code
+        @return: python code string
+        """
         enum_name = camelcase(enum.name)
         return f"""
 class {enum_name}(EnumDefinitionImpl):
     {self.gen_enum_comment(enum)}
     {self.gen_enum_description(enum, enum_name)}
 """.strip()
 
     def gen_enum_comment(self, enum: EnumDefinition) -> str:
-        return (
-            f'"""\n\t{wrapped_annotation(be(enum.description))}\n\t"""'
-            if be(enum.description)
-            else ""
-        )
+        if not be(enum.description):
+            return ""
+        desc_text = enum.description.replace('"""', "---")
+        return f'"""\n\t{wrapped_annotation(be(desc_text))}\n\t"""'
 
     def gen_enum_description(self, enum: EnumDefinition, enum_name: str) -> str:
         return f"""
     {self.gen_pvs(enum)}
 
     {self.gen_enum_definition(enum, enum_name)}
-    {self.gen_pvs2(enum)}
+    {self.gen_pvs_as_setattrs(enum)}
 """.strip()
 
-    def gen_pvs(self, enum: EnumDefinition) -> str:
-        """
-        Generate the python compliant permissible value initializers as a set of class variables
-        @param enum:
-        @return:
-        """
-        init_list = []
-        for pv in enum.permissible_values.values():
-            if str.isidentifier(pv.text) and not keyword.iskeyword(pv.text):
-                l1 = f"{pv.text} = "
-                l1len = len(l1)
-                l2ton = "\n" + l1len * " "
-                init_list.append(l1 + (l2ton.join(self.gen_pv_constructor(pv, l1len))))
-        return "\n\t".join(init_list).strip()
-
     def gen_enum_definition(self, enum: EnumDefinition, enum_name: str) -> str:
         enum_desc = (
-            enum.description.replace('"', '\\"').replace(r"\n", r"\\n")
+            self.process_multiline_string(enum.description, "\t\tdescription=")
             if enum.description
             else None
         )
-        desc = f'\t\tdescription="{enum_desc}",\n' if enum.description else ""
+        desc = f"{enum_desc},\n" if enum.description else ""
         cs = (
             f"\t\tcode_set={self.namespaces.curie_for(self.namespaces.uri_for(enum.code_set), default_ok=False, pythonform=True)},\n"
             if enum.code_set
             else ""
         )
         tag = f'\t\tcode_set_tag="{enum.code_set_tag}",\n' if enum.code_set_tag else ""
         ver = (
@@ -1100,65 +1103,115 @@
             f"\t\tpv_formula=PvFormulaOptions.{enum.pv_formula.code.text},\n"
             if enum.pv_formula
             else ""
         )
 
         return f"""_defn = EnumDefinition(\n\t\tname="{enum_name}",\n{desc}{cs}{tag}{ver}{vf}\t)"""
 
-    def gen_pvs2(self, enum: EnumDefinition) -> str:
+    def gen_pvs(self, enum: EnumDefinition) -> str:
+        """
+        Generate the python compliant permissible value initializers as a set of class variables
+        @param enum: EnumDefinition object to be converted into class variables
+        @return: string containing the enum declaration
+        """
+        init_list = []
+        for pv in enum.permissible_values.values():
+            if str.isidentifier(pv.text) and not keyword.iskeyword(pv.text):
+                init_list.append(f"{pv.text} = " + self.gen_pv_constructor(pv, 4))
+
+        return "\n\t".join(init_list).strip()
+
+    def gen_pvs_as_setattrs(self, enum: EnumDefinition) -> str:
         """
         Generate the non-python compliant permissible value initializers as a set of setattr instructions
-        @param enum:
-        @return:
+        in the form
+
+        @classmethod
+        def _addvals(cls):
+            setattr(cls, "NAME",
+                PermissibleValue(
+                    text="NAME",
+                    description="description here"))
+
+        @param enum: EnumDefinition object to be converted into code
+        @return: string containing the enum declaration
         """
         if any(
             not str.isidentifier(pv.text) or keyword.iskeyword(pv.text)
             for pv in enum.permissible_values.values()
         ):
+            init_list = []
+            for pv in enum.permissible_values.values():
+                if not str.isidentifier(pv.text) or keyword.iskeyword(pv.text):
+                    # first line is "        setattr("
+                    indent = 12
+                    indent_str = indent * " "
+                    pv_text = pv.text.replace('"', '\\"').replace(r"\n", r"\\n")
+                    pv_parts = self.gen_pv_constructor(pv, indent)
+                    init_list.append(
+                        f'        setattr(cls, "{pv_text}",\n{indent_str}{pv_parts})'
+                    )
+
+            add_vals_text = "\n".join(init_list).rstrip()
+
             return f"""
     @classmethod
     def _addvals(cls):
-        {self.gen_pvs2_initializers(enum)}"""
-        else:
-            return ""
+{add_vals_text}
+"""
 
-    def gen_pvs2_initializers(self, enum: EnumDefinition) -> str:
-        init_list = []
-        for pv in enum.permissible_values.values():
-            if not str.isidentifier(pv.text) or keyword.iskeyword(pv.text):
-                l1 = "        setattr("
-                l2ton = len(l1) * " "
-                pv_cons = "\n".join(self.gen_pv_constructor(pv, len(l1)))
-                pv_text = pv.text.replace('"', '\\"').replace(r"\n", r"\\n")
-                init_list.append(f'{l1}cls, "{pv_text}",\n{l2ton}{pv_cons} )')
-        return "\n".join(init_list).strip()
+        return ""
 
-    def gen_pv_constructor(self, pv: PermissibleValue, indent: int) -> List[str]:
+    def gen_pv_constructor(self, pv: PermissibleValue, indent: int) -> str:
         """
-        Generate a permissible value constructor
+        Generate a permissible value constructor in the form
+
+        PermissibleValue(text="NAME_ONLY")
+        PermissibleValue(
+            text="CODE",
+            description="...",
+            meaning="...")
+
         @param pv: Value to be constructed
         @param indent: number of additional spaces to add on successive lines
         @return: Permissible value constructor
         """
-        # PermissibleValue(text="CODE",
-        #                  description="...",
-        #                  meaning="...")
-        constructor = "PermissibleValue("
-        indent = (len(constructor) + indent) * " "
-        c1 = "," if pv.description or pv.meaning else ")"
-        rval = [f'{constructor}text="{pv.text}"{c1}']
+        constructor = "PermissibleValue"
+        pv_text = pv.text.replace('"', '\\"')
+
+        if not pv.description and not pv.meaning:
+            return f'{constructor}(text="{pv_text}")'
+
+        indent_str = (4 + indent) * " "
+        pv_attrs = [f'{indent_str}text="{pv_text}"']
         if pv.description:
-            c2 = "," if pv.meaning else ")"
-            rval.append(f'{indent}description="{pv.description}"{c2}')
+            pv_attrs.append(
+                f'{self.process_multiline_string(pv.description, f"{indent_str}description=")}'
+            )
         if pv.meaning:
             pv_meaning = self.namespaces.curie_for(
                 self.namespaces.uri_for(pv.meaning), default_ok=False, pythonform=True
             )
-            rval.append(f"{indent}meaning={pv_meaning})")
-        return rval
+            pv_attrs.append(f"{indent_str}meaning={pv_meaning}")
+
+        return "PermissibleValue(\n" + ",\n".join(pv_attrs) + ")"
+
+    def process_multiline_string(self, input: str, prefix_string: str) -> str:
+        """
+        Process a (potentially multi-line) string, preserving existing formatting
+
+        @param input: input string to be formatted
+        @param prefix_string: the text to prefix the first line of the output
+        @return: formatted string
+        """
+        string = input.rstrip().replace('"', '\\"')
+        if len(prefix_string + string) < split_col and input.find("\n") == -1:
+            return f'{prefix_string}"{string}"'
+
+        return f'{prefix_string}"""{string}"""'
 
 
 @shared_arguments(PythonGenerator)
 @click.command()
 @click.option(
     "--head/--no-head", default=True, show_default=True, help="Emit metadata heading"
 )
@@ -1183,27 +1236,33 @@
 @click.option(
     "--validate/--no-validate",
     default=False,
     show_default=True,
     help="Validate generated code by compiling it",
 )
 @click.version_option(__version__, "-V", "--version")
-def cli(yamlfile, head=True, genmeta=False, classvars=True, slots=True, validate=False, **args):
+def cli(
+    yamlfile,
+    head=True,
+    genmeta=False,
+    classvars=True,
+    slots=True,
+    validate=False,
+    **args,
+):
     """Generate python classes to represent a LinkML model"""
     gen = PythonGenerator(
-            yamlfile,
-            emit_metadata=head,
-            genmeta=genmeta,
-            gen_classvars=classvars,
-            gen_slots=slots,
-            **args,
-        )
+        yamlfile,
+        emit_metadata=head,
+        genmeta=genmeta,
+        gen_classvars=classvars,
+        gen_slots=slots,
+        **args,
+    )
     if validate:
         mod = gen.compile_module()
         logging.info(f"Module {mod} compiled successfully")
-    print(
-        gen.serialize(emit_metadata=head, **args)
-    )
+    print(gen.serialize(emit_metadata=head, **args))
 
 
 if __name__ == "__main__":
     cli()
```

### Comparing `linkml-1.5.1/linkml/generators/rdfgen.py` & `linkml-1.5.2/linkml/generators/rdfgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.1/linkml/generators/shaclgen.py` & `linkml-1.5.2/linkml/generators/shaclgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.1/linkml/generators/shexgen.py` & `linkml-1.5.2/linkml/generators/shexgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.1/linkml/generators/sparqlgen.py` & `linkml-1.5.2/linkml/generators/sparqlgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.1/linkml/generators/sqlalchemy/sqlalchemy_declarative_template.py` & `linkml-1.5.2/linkml/generators/sqlalchemy/sqlalchemy_declarative_template.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.1/linkml/generators/sqlalchemy/sqlalchemy_imperative_template.py` & `linkml-1.5.2/linkml/generators/sqlalchemy/sqlalchemy_imperative_template.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.1/linkml/generators/sqlalchemygen.py` & `linkml-1.5.2/linkml/generators/sqlalchemygen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.1/linkml/generators/sqlddlgen.py` & `linkml-1.5.2/linkml/generators/sqlddlgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.1/linkml/generators/sqltablegen.py` & `linkml-1.5.2/linkml/generators/sqltablegen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.1/linkml/generators/sssomgen.py` & `linkml-1.5.2/linkml/generators/sssomgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.1/linkml/generators/string_template.md` & `linkml-1.5.2/linkml/generators/string_template.md`

 * *Files identical despite different names*

### Comparing `linkml-1.5.1/linkml/generators/summarygen.py` & `linkml-1.5.2/linkml/generators/summarygen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.1/linkml/generators/terminusdbgen.py` & `linkml-1.5.2/linkml/generators/terminusdbgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.1/linkml/generators/typescriptgen.py` & `linkml-1.5.2/linkml/generators/typescriptgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.1/linkml/generators/yamlgen.py` & `linkml-1.5.2/linkml/generators/yamlgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.1/linkml/generators/yumlgen.py` & `linkml-1.5.2/linkml/generators/yumlgen.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.1/linkml/linter/cli.py` & `linkml-1.5.2/linkml/linter/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -49,14 +49,26 @@
     "-f",
     "--format",
     type=click.Choice(["terminal", "markdown", "json", "tsv"]),
     default="terminal",
     help="Report format.",
     show_default=True,
 )
+@click.option(
+    "--validate",
+    is_flag=True,
+    default=False,
+    help="Validate the schema against the LinkML Metamodel before linting.",
+)
+@click.option(
+    "--validate-only",
+    is_flag=True,
+    default=False,
+    help="Validate the schema against the LinkML Metamodel and then exit without checking linter rules.",
+)
 @click.option("-v", "--verbose", is_flag=True)
 @click.option(
     "-o", "--output", type=click.File("w"), default="-", help="Report file name."
 )
 @click.option(
     "--ignore-warnings",
     is_flag=True,
@@ -73,18 +85,20 @@
 @click.option("--fix/--no-fix", default=False)
 @click.version_option(__version__, "-V", "--version")
 def main(
     schema: Path,
     fix: bool,
     config: str,
     format: str,
+    validate: bool,
+    validate_only: bool,
     output,
     ignore_warnings: bool,
     max_warnings: int,
-    verbose: bool
+    verbose: bool,
 ):
     """Run linter on SCHEMA.
 
     SCHEMA can be a single LinkML YAML file or a directory. If it is a directory
     every YAML file found in the directory (recursively) will be linted."""
     config_file = None
     if config:
@@ -113,15 +127,17 @@
         formatter = TsvFormatter(output)
 
     error_count = 0
     warning_count = 0
     formatter.start_report()
     for path in get_yaml_files(schema):
         formatter.start_schema(path)
-        report = linter.lint(path, fix=fix)
+        report = linter.lint(
+            path, fix=fix, validate_schema=validate, validate_only=validate_only
+        )
         for problem in report:
             if str(problem.level) is RuleLevel.error.text:
                 error_count += 1
             elif str(problem.level) is RuleLevel.warning.text:
                 warning_count += 1
             formatter.handle_problem(problem)
         formatter.end_schema()
```

### Comparing `linkml-1.5.1/linkml/linter/config/datamodel/config.py` & `linkml-1.5.2/linkml/linter/config/datamodel/config.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.1/linkml/linter/config/datamodel/config.yaml` & `linkml-1.5.2/linkml/linter/config/datamodel/config.yaml`

 * *Files identical despite different names*

### Comparing `linkml-1.5.1/linkml/linter/config/default.yaml` & `linkml-1.5.2/linkml/linter/config/default.yaml`

 * *Files identical despite different names*

### Comparing `linkml-1.5.1/linkml/linter/formatters/formatter.py` & `linkml-1.5.2/linkml/linter/formatters/formatter.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.1/linkml/linter/formatters/json_formatter.py` & `linkml-1.5.2/linkml/linter/formatters/json_formatter.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.1/linkml/linter/formatters/markdown_formatter.py` & `linkml-1.5.2/linkml/linter/formatters/markdown_formatter.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.1/linkml/linter/formatters/terminal_formatter.py` & `linkml-1.5.2/linkml/linter/formatters/terminal_formatter.py`

 * *Files 6% similar despite different names*

```diff
@@ -56,7 +56,9 @@
                 + " "
                 + plural("problem", total_problems)
                 + " in "
                 + str(problem_schemas)
                 + " "
                 + plural("schema", problem_schemas)
             )
+        else:
+            self.write(click.style("\u2713", fg="green") + " No problems found")
```

### Comparing `linkml-1.5.1/linkml/linter/formatters/tsv_formatter.py` & `linkml-1.5.2/linkml/linter/formatters/tsv_formatter.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.1/linkml/linter/rules.py` & `linkml-1.5.2/linkml/linter/rules.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,14 @@
                                       RecommendedRuleConfig, RuleConfig,
                                       StandardNamingConfig,
                                       TreeRootClassRuleConfig)
 from .linter import LinterProblem
 
 
 class LinterRule(ABC):
-
     PATTERNS = {
         "snake": re.compile(r"[a-z][_a-z0-9]+"),
         "uppersnake": re.compile(r"[A-Z][_A-Z0-9]+"),
         "camel": re.compile(r"[a-z][a-zA-Z0-9]+"),
         "uppercamel": re.compile(r"[A-Z][a-zA-Z0-9]+"),
         "kebab": re.compile(r"[a-z][\-a-z0-9]+"),
         "_uncamel": re.compile(r"(?<!^)(?=[A-Z])"),
@@ -48,15 +47,14 @@
     @staticmethod
     def format_element(element: Element):
         class_name = element.__class__.__name__.replace("Definition", "")
         return f"{class_name} '{element.name}'"
 
 
 class NoEmptyTitleRule(LinterRule):
-
     id = "no_empty_title"
 
     def check(
         self, schema_view: SchemaView, fix: bool = False
     ) -> Iterable[LinterProblem]:
         for e in schema_view.all_elements(imports=False).values():
             if fix and e.title is None:
@@ -67,30 +65,28 @@
                 problem = LinterProblem(
                     message=f"{self.format_element(e)} has no title"
                 )
                 yield problem
 
 
 class NoXsdIntTypeRule(LinterRule):
-
     id = "no_xsd_int_type"
 
     def check(self, schema_view: SchemaView, fix: bool = False):
         for type_definition in schema_view.all_types(imports=False).values():
             if type_definition.uri == "xsd:int":
                 if fix:
                     type_definition.uri = "xsd:integer"
                 else:
                     yield LinterProblem(
                         f"{self.format_element(type_definition)} has uri xsd:int"
                     )
 
 
 class PermissibleValuesFormatRule(LinterRule):
-
     id = "permissible_values_format"
 
     def check(
         self, schema_view: SchemaView, fix: bool = False
     ) -> Iterable[LinterProblem]:
         pattern = self.PATTERNS.get(self.config.format, re.compile(self.config.format))
         for enum_def in schema_view.all_enums(imports=False).values():
@@ -110,15 +106,14 @@
         for slot in class_slots:
             if slot.recommended:
                 recommended_meta_slots.append(f"{class_name}__{slot.name}")
     return recommended_meta_slots
 
 
 class RecommendedRule(LinterRule):
-
     id = "recommended"
 
     def __init__(self, config: RecommendedRuleConfig) -> None:
         self.config = config
 
     def check(self, schema_view: SchemaView, fix: bool = False):
         recommended_meta_slots = _get_recommended_metamodel_slots()
@@ -134,15 +129,14 @@
                 if key in recommended_meta_slots and not meta_slot_value:
                     yield LinterProblem(
                         f"{self.format_element(element_definition)} does not have recommended slot '{meta_slot_name}'"
                     )
 
 
 class TreeRootClassRule(LinterRule):
-
     id = "tree_root_class"
 
     def __init__(self, config: TreeRootClassRuleConfig) -> None:
         super().__init__(config)
 
     def check(
         self, schema_view: SchemaView, fix: bool = False
@@ -220,15 +214,14 @@
             index_slots.append(index_slot)
             schema_view.add_slot(index_slot)
             container.slots.append(index_slot.name)
         return index_slots
 
 
 class NoInvalidSlotUsageRule(LinterRule):
-
     id = "no_invalid_slot_usage"
 
     def check(
         self, schema_view: SchemaView, fix: bool = False
     ) -> Iterable[LinterProblem]:
         for class_name, class_definition in schema_view.all_classes(
             imports=False
@@ -241,15 +234,14 @@
                 if slot_usage_name not in class_slots:
                     yield LinterProblem(
                         f"Slot '{slot_usage_name}' not found on class '{class_name}'"
                     )
 
 
 class StandardNamingRule(LinterRule):
-
     id = "standard_naming"
 
     def __init__(self, config: StandardNamingConfig) -> None:
         self.config = config
 
     def check(
         self, schema_view: SchemaView, fix: bool = False
@@ -279,15 +271,14 @@
                 if permissible_value_pattern.fullmatch(permissible_value_name) is None:
                     yield LinterProblem(
                         f"Permissible value of {self.format_element(enum_definition)} has name '{permissible_value_name}'"
                     )
 
 
 class CanonicalPrefixesRule(LinterRule):
-
     id = "canonical_prefixes"
 
     def __init__(self, config: CanonicalPrefixesConfig) -> None:
         self.config = config
 
     def check(
         self, schema_view: SchemaView, fix: bool = False
```

### Comparing `linkml-1.5.1/linkml/reporting/model.py` & `linkml-1.5.2/linkml/reporting/model.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.1/linkml/transformers/relmodel_transformer.py` & `linkml-1.5.2/linkml/transformers/relmodel_transformer.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.1/linkml/transformers/schema_renamer.py` & `linkml-1.5.2/linkml/transformers/schema_renamer.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.1/linkml/utils/converter.py` & `linkml-1.5.2/linkml/utils/converter.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.1/linkml/utils/datautils.py` & `linkml-1.5.2/linkml/utils/datautils.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.1/linkml/utils/execute_tutorial.py` & `linkml-1.5.2/linkml/utils/execute_tutorial.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.1/linkml/utils/generator.py` & `linkml-1.5.2/linkml/utils/generator.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.1/linkml/utils/ifabsent_functions.py` & `linkml-1.5.2/linkml/utils/ifabsent_functions.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.1/linkml/utils/mergeutils.py` & `linkml-1.5.2/linkml/utils/mergeutils.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.1/linkml/utils/rawloader.py` & `linkml-1.5.2/linkml/utils/rawloader.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.1/linkml/utils/schema_builder.py` & `linkml-1.5.2/linkml/utils/schema_builder.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.1/linkml/utils/schema_fixer.py` & `linkml-1.5.2/linkml/utils/schema_fixer.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.1/linkml/utils/schemaloader.py` & `linkml-1.5.2/linkml/utils/schemaloader.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.1/linkml/utils/schemasynopsis.py` & `linkml-1.5.2/linkml/utils/schemasynopsis.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.1/linkml/utils/sqlutils.py` & `linkml-1.5.2/linkml/utils/sqlutils.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.1/linkml/utils/typereferences.py` & `linkml-1.5.2/linkml/utils/typereferences.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.1/linkml/utils/validation.py` & `linkml-1.5.2/linkml/utils/validation.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.1/linkml/validators/jsonschemavalidator.py` & `linkml-1.5.2/linkml/validators/jsonschemavalidator.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,26 +48,27 @@
         inst_dict = as_simple_dict(data)
         not_closed = not closed
         if self.schema is None:
             raise ValueError(f"schema object must be set")
         if self.jsonschema_objs is None:
             self.jsonschema_objs = {}
         schema_id = self.schema.id if isinstance(self.schema, SchemaDefinition) else self.schema
-        if schema_id not in self.jsonschema_objs:
+        cache_params = frozenset([schema_id, target_class.class_name])
+        if cache_params not in self.jsonschema_objs:
             jsonschemastr = JsonSchemaGenerator(
                 self.schema,
                 mergeimports=True,
                 top_class=target_class.class_name,
                 not_closed=not_closed,
             ).serialize(not_closed=not_closed)
             jsonschema_obj = json.loads(jsonschemastr)
-            self.jsonschema_objs[schema_id] = jsonschema_obj
+            self.jsonschema_objs[cache_params] = jsonschema_obj
         else:
             logging.info(f"Using cached jsonschema for {schema_id}")
-            jsonschema_obj = self.jsonschema_objs[schema_id]
+            jsonschema_obj = self.jsonschema_objs[cache_params]
         return jsonschema.validate(inst_dict, schema=jsonschema_obj, format_checker=jsonschema.Draft7Validator.FORMAT_CHECKER)
 
     def validate_dict(
         self, data: dict, target_class: ClassDefinitionName = None, closed: bool = True
     ) -> None:
         """
         validates instance data against a schema
@@ -144,15 +145,15 @@
     input_format = datautils._get_format(input, input_format)
     loader = datautils.get_loader(input_format)
 
     inargs = {}
     outargs = {}
     if datautils._is_xsv(input_format):
         if index_slot is None:
-            index_slot = infer_index_slot(sv, target_class)
+            index_slot = datautils.infer_index_slot(sv, target_class)
             if index_slot is None:
                 raise Exception("--index-slot is required for CSV input")
         inargs["index_slot"] = index_slot
         inargs["schema"] = schema
     if datautils._is_rdf_format(input_format):
         inargs["schemaview"] = sv
         inargs["fmt"] = input_format
```

### Comparing `linkml-1.5.1/linkml/validators/sparqlvalidator.py` & `linkml-1.5.2/linkml/validators/sparqlvalidator.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.1/linkml/workspaces/datamodel/workspaces.py` & `linkml-1.5.2/linkml/workspaces/datamodel/workspaces.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.1/linkml/workspaces/datamodel/workspaces.yaml` & `linkml-1.5.2/linkml/workspaces/datamodel/workspaces.yaml`

 * *Files identical despite different names*

### Comparing `linkml-1.5.1/linkml/workspaces/example_runner.py` & `linkml-1.5.2/linkml/workspaces/example_runner.py`

 * *Files identical despite different names*

### Comparing `linkml-1.5.1/pyproject.toml` & `linkml-1.5.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "linkml"
-version = "1.5.1"
+version = "1.5.2"
 description = "Linked Open Data Modeling Language"
 authors = [
     "Chris Mungall <cjmungall@lbl.gov>",
     "Harold Solbrig <solbrig@jhu.edu>",
     "Sujay Patil <spatil@lbl.gov>",
     "Harshad Hegde <hhegde@lbl.gov>",
     "Sierra Moxon <smoxon@lbl.gov>",
```

### Comparing `linkml-1.5.1/setup.py` & `linkml-1.5.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -106,15 +106,15 @@
                      'linkml-sqldb = linkml.utils.sqlutils:main',
                      'linkml-validate = '
                      'linkml.validators.jsonschemavalidator:cli',
                      'run-tutorial = linkml.utils.execute_tutorial:cli']}
 
 setup_kwargs = {
     'name': 'linkml',
-    'version': '1.5.1',
+    'version': '1.5.2',
     'description': 'Linked Open Data Modeling Language',
     'long_description': '[![Pyversions](https://img.shields.io/pypi/pyversions/linkml.svg)](https://pypi.python.org/pypi/linkml)\n![](https://github.com/linkml/linkml/workflows/Build/badge.svg)\n[![PyPi](https://img.shields.io/pypi/v/linkml.svg)](https://pypi.python.org/pypi/linkml)\n[![badge](https://img.shields.io/badge/launch-binder-579ACA.svg)](https://mybinder.org/v2/gh/linkml/linkml/main?filepath=notebooks)\n[![DOI](https://zenodo.org/badge/13996/linkml/linkml.svg)](https://zenodo.org/badge/latestdoi/13996/linkml/linkml)\n[![PyPIDownloadsTotal](https://pepy.tech/badge/linkml)](https://pepy.tech/project/linkml)\n[![PyPIDownloadsMonth](https://img.shields.io/pypi/dm/linkml?logo=PyPI&color=blue)](https://pypi.org/project/linkml)\n[![codecov](https://codecov.io/gh/linkml/linkml/branch/main/graph/badge.svg?token=WNQNG986UN)](https://codecov.io/gh/linkml/linkml)\n\n\n# LinkML - Linked Data Modeling Language\n\nLinkML is a linked data modeling language following object-oriented and ontological principles. LinkML models are typically authored in YAML, and can be converted to other schema representation formats such as JSON or RDF.\n\nThis repo holds the tools for generating and working with LinkML. For the LinkML schema (metamodel), please see https://github.com/linkml/linkml-model\n\nThe complete documentation for LinkML can be found here:\n\n - [linkml.io/linkml](https://linkml.io/linkml)\n',
     'author': 'Chris Mungall',
     'author_email': 'cjmungall@lbl.gov',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://linkml.io/linkml/',
```

### Comparing `linkml-1.5.1/PKG-INFO` & `linkml-1.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linkml
-Version: 1.5.1
+Version: 1.5.2
 Summary: Linked Open Data Modeling Language
 Home-page: https://linkml.io/linkml/
 Keywords: schema,linked data,data modeling,rdf,owl,biolink
 Author: Chris Mungall
 Author-email: cjmungall@lbl.gov
 Requires-Python: >=3.7.6,<4.0.0
 Classifier: Development Status :: 5 - Production/Stable
```

