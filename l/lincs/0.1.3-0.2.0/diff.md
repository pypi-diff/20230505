# Comparing `tmp/lincs-0.1.3.tar.gz` & `tmp/lincs-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lincs-0.1.3.tar", last modified: Thu May  4 12:22:14 2023, max compression
+gzip compressed data, was "lincs-0.2.0.tar", last modified: Fri May  5 13:57:19 2023, max compression
```

## Comparing `lincs-0.1.3.tar` & `lincs-0.2.0.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-05-04 12:22:14.811602 lincs-0.1.3/
--rw-r--r--   0 user      (1002) user      (1002)       58 2023-05-04 08:59:02.000000 lincs-0.1.3/MANIFEST.in
--rw-r--r--   0 user      (1002) user      (1002)      828 2023-05-04 12:22:14.811602 lincs-0.1.3/PKG-INFO
--rw-r--r--   0 user      (1002) user      (1002)      211 2023-05-04 09:18:36.000000 lincs-0.1.3/README.md
-drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-05-04 12:22:14.811602 lincs-0.1.3/lincs/
--rw-rw-r--   0 user      (1002) user      (1002)      241 2023-05-04 08:59:02.000000 lincs-0.1.3/lincs/__init__.py
--rw-r--r--   0 user      (1002) user      (1002)      136 2023-05-04 08:59:02.000000 lincs-0.1.3/lincs/__main__.py
--rw-rw-r--   0 user      (1002) user      (1002)    16100 2023-05-04 09:30:03.000000 lincs-0.1.3/lincs/command_line_interface.py
-drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-05-04 12:22:14.811602 lincs-0.1.3/lincs/liblincs/
--rw-rw-r--   0 user      (1002) user      (1002)     6579 2023-05-04 08:59:02.000000 lincs-0.1.3/lincs/liblincs/liblincs_module.cpp
--rw-rw-r--   0 user      (1002) user      (1002)     5489 2023-05-04 08:59:02.000000 lincs-0.1.3/lincs/liblincs/lincs.cpp
--rw-rw-r--   0 user      (1002) user      (1002)     3647 2023-05-04 08:59:02.000000 lincs-0.1.3/lincs/liblincs/lincs.hpp
-drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-05-04 12:22:14.811602 lincs-0.1.3/lincs.egg-info/
--rw-r--r--   0 user      (1002) user      (1002)      828 2023-05-04 12:22:14.000000 lincs-0.1.3/lincs.egg-info/PKG-INFO
--rw-r--r--   0 user      (1002) user      (1002)      376 2023-05-04 12:22:14.000000 lincs-0.1.3/lincs.egg-info/SOURCES.txt
--rw-r--r--   0 user      (1002) user      (1002)        1 2023-05-04 12:22:14.000000 lincs-0.1.3/lincs.egg-info/dependency_links.txt
--rw-r--r--   0 user      (1002) user      (1002)       60 2023-05-04 12:22:14.000000 lincs-0.1.3/lincs.egg-info/entry_points.txt
--rw-r--r--   0 user      (1002) user      (1002)       11 2023-05-04 12:22:14.000000 lincs-0.1.3/lincs.egg-info/requires.txt
--rw-r--r--   0 user      (1002) user      (1002)       15 2023-05-04 12:22:14.000000 lincs-0.1.3/lincs.egg-info/top_level.txt
--rw-r--r--   0 user      (1002) user      (1002)       11 2023-05-04 08:59:02.000000 lincs-0.1.3/requirements.txt
--rw-r--r--   0 user      (1002) user      (1002)       38 2023-05-04 12:22:14.811602 lincs-0.1.3/setup.cfg
--rw-rw-r--   0 user      (1002) user      (1002)     1551 2023-05-04 12:22:02.000000 lincs-0.1.3/setup.py
+drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-05-05 13:57:19.840721 lincs-0.2.0/
+-rw-r--r--   0 user      (1002) user      (1002)       58 2023-05-04 08:59:02.000000 lincs-0.2.0/MANIFEST.in
+-rw-r--r--   0 user      (1002) user      (1002)    10332 2023-05-05 13:57:19.840721 lincs-0.2.0/PKG-INFO
+-rw-r--r--   0 user      (1002) user      (1002)     9715 2023-05-05 13:53:52.000000 lincs-0.2.0/README.md
+drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-05-05 13:57:19.840721 lincs-0.2.0/lincs/
+-rw-rw-r--   0 user      (1002) user      (1002)      343 2023-05-05 13:09:35.000000 lincs-0.2.0/lincs/__init__.py
+-rw-r--r--   0 user      (1002) user      (1002)      136 2023-05-04 08:59:02.000000 lincs-0.2.0/lincs/__main__.py
+-rw-rw-r--   0 user      (1002) user      (1002)    18889 2023-05-05 13:44:47.000000 lincs-0.2.0/lincs/command_line_interface.py
+drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-05-05 13:57:19.840721 lincs-0.2.0/lincs/liblincs/
+-rw-rw-r--   0 user      (1002) user      (1002)     9114 2023-05-05 13:34:11.000000 lincs-0.2.0/lincs/liblincs/liblincs_module.cpp
+-rw-rw-r--   0 user      (1002) user      (1002)    12319 2023-05-05 12:56:20.000000 lincs-0.2.0/lincs/liblincs/lincs.cpp
+-rw-rw-r--   0 user      (1002) user      (1002)     4460 2023-05-05 13:32:55.000000 lincs-0.2.0/lincs/liblincs/lincs.hpp
+-rw-rw-r--   0 user      (1002) user      (1002)      718 2023-05-05 13:51:37.000000 lincs-0.2.0/lincs/visualization.py
+drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-05-05 13:57:19.840721 lincs-0.2.0/lincs.egg-info/
+-rw-r--r--   0 user      (1002) user      (1002)    10332 2023-05-05 13:57:19.000000 lincs-0.2.0/lincs.egg-info/PKG-INFO
+-rw-r--r--   0 user      (1002) user      (1002)      399 2023-05-05 13:57:19.000000 lincs-0.2.0/lincs.egg-info/SOURCES.txt
+-rw-r--r--   0 user      (1002) user      (1002)        1 2023-05-05 13:57:19.000000 lincs-0.2.0/lincs.egg-info/dependency_links.txt
+-rw-r--r--   0 user      (1002) user      (1002)       60 2023-05-05 13:57:19.000000 lincs-0.2.0/lincs.egg-info/entry_points.txt
+-rw-r--r--   0 user      (1002) user      (1002)       27 2023-05-05 13:57:19.000000 lincs-0.2.0/lincs.egg-info/requires.txt
+-rw-r--r--   0 user      (1002) user      (1002)       15 2023-05-05 13:57:19.000000 lincs-0.2.0/lincs.egg-info/top_level.txt
+-rw-r--r--   0 user      (1002) user      (1002)       27 2023-05-05 13:01:57.000000 lincs-0.2.0/requirements.txt
+-rw-r--r--   0 user      (1002) user      (1002)       38 2023-05-05 13:57:19.840721 lincs-0.2.0/setup.cfg
+-rw-rw-r--   0 user      (1002) user      (1002)     1551 2023-05-05 13:55:12.000000 lincs-0.2.0/setup.py
```

### Comparing `lincs-0.1.3/lincs/command_line_interface.py` & `lincs-0.2.0/lincs/command_line_interface.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 from __future__ import annotations
+import random
 import subprocess
+import sys
 
 import click
 
 import lincs
+import lincs.visualization
 
 
 def options_tree(name, kwds, dependents):
     """
     Ad-hoc decorator for a tree dependent of click.options.
     Options down the tree are only valid if the options up the tree are set to specific values.
     Think of them as sub-options of the previous ones.
@@ -88,85 +91,120 @@
 
         if isinstance(command, click.Group):
             for name, command in command.commands.items():
                 walk(prefix + [name], command)
 
     walk([], main)
 
+    for obj_name in sorted(dir(lincs)):
+        if obj_name.startswith("_"):
+            continue
+
+        obj = getattr(lincs, obj_name)
+        print(f"lincs.{obj_name}")
+        print("=" * len(f"lincs.{obj_name}"))
+        print()
+        if obj.__doc__:
+            print(obj.__doc__)
+            print()
+        if isinstance(obj, type):
+            for attr_name in sorted(dir(obj)):
+                if attr_name.startswith("_"):
+                    continue
+                if (
+                    obj_name in {"CategoryCorrelation", "SufficientCoalitionsKind", "ValueType"}
+                    and
+                    attr_name in {"as_integer_ratio", "bit_count", "bit_length", "conjugate", "denominator", "from_bytes", "imag", "numerator", "to_bytes", "attr_name", "name", "names", "values"}
+                ):
+                    continue
+                if (
+                    obj_name in {"CategoryCorrelation", "SufficientCoalitionsKind"}
+                    and
+                    attr_name in {"real"}
+                ):
+                    continue
+                print(f"{attr_name}")
+                print("-" * len(attr_name))
+                print()
+                doc = getattr(obj, attr_name).__doc__
+                if doc:
+                    print(doc)
+                    print()
+
 
 @main.group(
     help="Generate synthetic data.",
 )
 def generate():
     pass
 
 
 @generate.command(
     help="""
         Generate a synthetic classification domain.
 
         The generated domain has CRITERIA_COUNT criteria and CATEGORIES_COUNT categories.
-
-        The generated *classification domain* file is written to OUTPUT_DOMAIN, which defaults to - to write to the standard output.
     """,
 )
 @click.argument(
     "criteria-count",
     type=click.IntRange(min=1),
 )
 @click.argument(
     "categories-count",
     type=click.IntRange(min=1),
 )
-@click.argument(
-    "output-domain",
+@click.option(
+    "--output-domain",
     type=click.File(mode="w"),
     default="-",
+    help="Write generated domain to this file instead of standard output.",
 )
 @click.option(
     "--random-seed",
     help="The random seed to use.",
     type=click.IntRange(min=0),
+    default=random.randrange(2**30),
 )
 def classification_domain(
     criteria_count,
     categories_count,
     output_domain,
     random_seed
 ):
-    domain = lincs.Domain(
-        [lincs.Criterion(f"Criterion n°{i}", lincs.ValueType.real, lincs.CategoryCorrelation.growing) for i in range(criteria_count)],
-        [lincs.Category(f"Category n°{i}") for i in range(categories_count)],
+    domain = lincs.generate_domain(
+        criteria_count,
+        categories_count,
+        random_seed=random_seed,
     )
     domain.dump(output_domain)
-    output_domain.write("\n")
 
 
 @generate.command(
     help="""
         Generate a synthetic classification model.
 
         DOMAIN is a *classification domain* file describing the domain to generate a model for.
-
-        The generated *classification model* file is written to OUTPUT_MODEL, which defaults to - to write to the standard output.
     """,
 )
 @click.argument(
     "domain",
     type=click.File(mode="r"),
 )
-@click.argument(
-    "output-model",
+@click.option(
+    "--output-model",
     type=click.File(mode="w"),
     default="-",
+    help="Write generated model to this file instead of standard output.",
 )
 @click.option(
     "--random-seed",
     help="The random seed to use.",
     type=click.IntRange(min=0),
+    default=random.randrange(2**30),
 )
 @options_tree(
     "model-type",
     dict(
         help="The type of classification model to generate.",
         type=click.Choice(["mrsort"]),
         default="mrsort",
@@ -191,68 +229,120 @@
     domain,
     output_model,
     random_seed,
     model_type,
     mrsort__fixed_threshold,
 ):
     domain = lincs.load_domain(domain)
+    assert model_type == "mrsort"
+    model = lincs.generate_mrsort_model(
+        domain,
+        # fixed_threshold=mrsort__fixed_threshold,
+        random_seed=random_seed,
+    )
+    model.dump(output_model)
 
 
 @generate.command(
     help="""
         Generate synthetic classified alternatives.
 
         DOMAIN is a *classification domain* file describing the domain to generate alternatives for.
         MODEL is a *classification model* file for that domain describing the model to use to classify the generated alternatives.
-
-        The generated *classified alternatives* file is written to OUTPUT_CLASSIFIED_ALTERNATIVES, which defaults to - to write to the standard output.
     """,
 )
 @click.argument(
     "domain",
     type=click.File(mode="r"),
 )
 @click.argument(
     "model",
     type=click.File(mode="r"),
 )
 @click.argument(
     "alternatives-count",
     type=click.IntRange(min=1),
 )
-@click.argument(
-    "output-classified-alternatives",
+@click.option(
+    "--output-classified-alternatives",
     type=click.File(mode="w"),
     default="-",
+    help="Write generated classified alternatives to this file instead of standard output.",
 )
 @click.option(
     "--max-imbalance",
     help="@todo Define.",
     type=click.FloatRange(min=0.0, max=1.0),
     default=None,
     show_default=True,
 )
 @click.option(
     "--random-seed",
     help="The random seed to use.",
     type=click.IntRange(min=0),
+    default=random.randrange(2**30),
 )
 def classified_alternatives(
     domain,
     model,
     alternatives_count,
     max_imbalance,
     output_classified_alternatives,
     random_seed,
 ):
     domain = lincs.load_domain(domain)
+    model = lincs.load_model(domain, model)
+    alternatives = lincs.generate_alternatives(
+        domain,
+        model,
+        alternatives_count,
+        # max_imbalance=max_imbalance,
+        random_seed=random_seed,
+    )
+    alternatives.dump(output_classified_alternatives)
+
+
+@main.group()
+def visualize():
+    pass
+
+
+@visualize.command()
+@click.argument(
+    "domain",
+    type=click.File(mode="r"),
+)
+@click.argument(
+    "model",
+    type=click.File(mode="r"),
+)
+@click.option(
+    "--alternatives",
+    type=click.File(mode="r"),
+)
+@click.argument(
+    "output",
+    type=click.File(mode="wb"),
+)
+def model(
+    domain,
+    model,
+    alternatives,
+    output,
+):
+    domain = lincs.load_domain(domain)
+    model = lincs.load_model(domain, model)
+    if alternatives is not None:
+        alternatives = lincs.load_alternatives(domain, alternatives)
+    lincs.visualization.visualize_model(domain, model, alternatives, output)
 
 
 @main.group(
     help="Learn a model.",
+    hidden=True,
 )
 def learn():
     pass
 
 
 @learn.command(
     help="""
@@ -452,42 +542,45 @@
 @main.command(
     help="""
         Classify alternatives.
 
         DOMAIN is a *classification domain* file.
         MODEL is a *classification model* file for that domain.
         ALTERNATIVES is an *unclassified alternatives* file for that domain.
-
-        The *classified alternatives* file is written to OUTPUT_CLASSIFIED_ALTERNATIVES, which defaults to - to write to standard output.
     """,
 )
 @click.argument(
     "domain",
     type=click.File(mode="r"),
 )
 @click.argument(
     "model",
     type=click.File(mode="r"),
 )
 @click.argument(
     "alternatives",
     type=click.File(mode="r"),
 )
-@click.argument(
-    "output-classified-alternatives",
+@click.option(
+    "--output-classified-alternatives",
     type=click.File(mode="w"),
     default="-",
+    help="Write classified alternatives to this file instead of standard output.",
 )
 def classify(
     domain,
     model,
     alternatives,
     output_classified_alternatives,
 ):
-    pass
+    domain = lincs.load_domain(domain)
+    model = lincs.load_model(domain, model)
+    alternatives = lincs.load_alternatives(domain, alternatives)
+    lincs.classify_alternatives(domain, model, alternatives)
+    alternatives.dump(output_classified_alternatives)
 
 
 @main.command(
     help="""
         Compute a classification accuracy.
 
         DOMAIN is a *classification domain* file.
@@ -510,8 +603,12 @@
     type=click.File(mode="r"),
 )
 def classification_accuracy(
     domain,
     model,
     testing_set,
 ):
-    pass
+    domain = lincs.load_domain(domain)
+    model = lincs.load_model(domain, model)
+    testing_set = lincs.load_alternatives(domain, testing_set)
+    result = lincs.classify_alternatives(domain, model, testing_set)
+    print(f"{result.unchanged}/{result.changed + result.unchanged}")
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `lincs-0.1.3/lincs/liblincs/liblincs_module.cpp` & `lincs-0.2.0/lincs/liblincs/liblincs_module.cpp`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 #include "lincs.hpp"
 
 #include <iostream>
 
-#include <Python.h>
-
 #include <boost/python.hpp>
 #include <boost/python/suite/indexing/vector_indexing_suite.hpp>
 #include <boost/iostreams/concepts.hpp>
 #include <boost/iostreams/stream.hpp>
 #include <magic_enum.hpp>
 
 
@@ -35,15 +33,15 @@
 }
 
 void dump_model(const lincs::Model& model, bp::object& out_file) {
   boost::iostreams::stream<PythonOutputDevice> out_stream(out_file);
   model.dump(out_stream);
 }
 
-void dump_alternatives(const lincs::AlternativesSet& alternatives, bp::object& out_file) {
+void dump_alternatives(const lincs::Alternatives& alternatives, bp::object& out_file) {
   boost::iostreams::stream<PythonOutputDevice> out_stream(out_file);
   alternatives.dump(out_stream);
 }
 
 class PythonInputDevice : public boost::iostreams::source {
   public:
 
@@ -60,22 +58,22 @@
 };
 
 lincs::Domain load_domain(bp::object& in_file) {
   boost::iostreams::stream<PythonInputDevice> in_stream(in_file);
   return lincs::Domain::load(in_stream);
 }
 
-lincs::Model load_model(lincs::Domain* domain, bp::object& in_file) {
+lincs::Model load_model(const lincs::Domain& domain, bp::object& in_file) {
   boost::iostreams::stream<PythonInputDevice> in_stream(in_file);
   return lincs::Model::load(domain, in_stream);
 }
 
-lincs::AlternativesSet load_alternatives(lincs::Domain* domain, bp::object& in_file) {
+lincs::Alternatives load_alternatives(const lincs::Domain& domain, bp::object& in_file) {
   boost::iostreams::stream<PythonInputDevice> in_stream(in_file);
-  return lincs::AlternativesSet::load(domain, in_stream);
+  return lincs::Alternatives::load(domain, in_stream);
 }
 
 // https://stackoverflow.com/a/15940413/905845
 struct iterable_converter {
   template <typename Container>
   iterable_converter& from_python() {
     bp::converter::registry::push_back(
@@ -147,39 +145,106 @@
   ;
   bp::class_<std::vector<lincs::Domain::Criterion>>("criteria_vector")
     .def(bp::vector_indexing_suite<std::vector<lincs::Domain::Criterion>>())
   ;
   bp::class_<lincs::Domain>("Domain", bp::init<std::vector<lincs::Domain::Criterion>, std::vector<lincs::Domain::Category>>())
     .def_readwrite("criteria", &lincs::Domain::criteria)
     .def_readwrite("categories", &lincs::Domain::categories)
-    .def("dump", &dump_domain)
-  ;
-  bp::def("load_domain", &load_domain);
+    .def(
+      "dump",
+      &dump_domain,
+      (bp::arg("self"), "out"),
+      "Dump the domain to the provided `.write()`-supporting file-like object, in YAML format."
+    )
+  ;
+  // @todo Make these 'staticmethod's of Alternatives. Same for other load and generate functions.
+  bp::def(
+    "load_domain",
+    &load_domain,
+    (bp::arg("in")),
+    "Load a domain from the provided `.read()`-supporting file-like object, in YAML format."
+  );
+  bp::def(
+    "generate_domain",
+    &lincs::Domain::generate,
+    (bp::arg("criteria_count"), "categories_count", "random_seed"),
+    "Generate a domain with `criteria_count` criteria and `categories_count` categories."
+  );
 
   bp::class_<lincs::Model::SufficientCoalitions>("SufficientCoalitions", bp::init<lincs::Model::SufficientCoalitions::Kind, std::vector<float>>())
     .def_readwrite("kind", &lincs::Model::SufficientCoalitions::kind)
     .def_readwrite("criterion_weights", &lincs::Model::SufficientCoalitions::criterion_weights)
   ;
 
+  bp::class_<std::vector<float>>("floats_vector")
+    .def(bp::vector_indexing_suite<std::vector<float>>())
+  ;
   bp::class_<lincs::Model::Boundary>("Boundary", bp::init<std::vector<float>, lincs::Model::SufficientCoalitions>())
     .def_readwrite("profile", &lincs::Model::Boundary::profile)
     .def_readwrite("sufficient_coalitions", &lincs::Model::Boundary::sufficient_coalitions)
   ;
-
-  bp::class_<lincs::Model>("Model", bp::init<lincs::Domain*, const std::vector<lincs::Model::Boundary>&>())
-    .def_readwrite("boundaries", &lincs::Model::boundaries)
-    .def("dump", &dump_model)
+  bp::class_<std::vector<lincs::Model::Boundary>>("boundaries_vector")
+    .def(bp::vector_indexing_suite<std::vector<lincs::Model::Boundary>>())
   ;
-  bp::def("load_model", &load_model);
+  bp::class_<lincs::Model>("Model", bp::init<const lincs::Domain&, const std::vector<lincs::Model::Boundary>&>())
+    .def_readwrite("boundaries", &lincs::Model::boundaries)
+    .def(
+      "dump",
+      &dump_model,
+      (bp::arg("self"), "out"),
+      "Dump the model to the provided `.write()`-supporting file-like object, in YAML format."
+    )
+  ;
+  bp::def(
+    "load_model",
+    &load_model,
+    (bp::arg("domain"), "in"),
+    "Load a model for the provided `domain`, from the provided `.read()`-supporting file-like object, in YAML format."
+  );
+  bp::def(
+    "generate_mrsort_model",
+    &lincs::Model::generate_mrsort,
+    (bp::arg("domain"), "random_seed"),
+    "Generate an MR-Sort model for the provided `domain`."
+  );
 
   bp::class_<lincs::Alternative>("Alternative", bp::init<std::string, std::vector<float>, std::string>())
     .def_readwrite("name", &lincs::Alternative::name)
     .def_readwrite("profile", &lincs::Alternative::profile)
     .def_readwrite("category", &lincs::Alternative::category)
   ;
-
-  bp::class_<lincs::AlternativesSet>("AlternativesSet", bp::init<lincs::Domain*, const std::vector<lincs::Alternative>&>())
-    .def_readwrite("alternatives", &lincs::AlternativesSet::alternatives)
-    .def("dump", &dump_alternatives)
+  bp::class_<std::vector<lincs::Alternative>>("alternatives_vector")
+    .def(bp::vector_indexing_suite<std::vector<lincs::Alternative>>())
   ;
-  bp::def("load_alternatives", &load_alternatives);
+  bp::class_<lincs::Alternatives>("Alternatives", bp::init<const lincs::Domain&, const std::vector<lincs::Alternative>&>())
+    .def_readwrite("alternatives", &lincs::Alternatives::alternatives)
+    .def(
+      "dump",
+      &dump_alternatives,
+      (bp::arg("self"), "out"),
+      "Dump the set of alternatives to the provided `.write()`-supporting file-like object, in CSV format."
+    )
+  ;
+  bp::def(
+    "load_alternatives",
+    &load_alternatives,
+    (bp::arg("domain"), "in"),
+    "Load a set of alternatives (classified or not) from the provided `.read()`-supporting file-like object, in CSV format."
+  );
+  bp::def(
+    "generate_alternatives",
+    &lincs::Alternatives::generate,
+    (bp::arg("domain"), "model", "alternatives_count", "random_seed"),
+    "Generate a set of `alternatives_count` pseudo-random alternatives for the provided `domain`, classified according to the provided `model`."
+  );
+
+  bp::class_<lincs::ClassificationResult>("ClassificationResult", bp::no_init)
+    .def_readonly("changed", &lincs::ClassificationResult::changed)
+    .def_readonly("unchanged", &lincs::ClassificationResult::unchanged)
+  ;
+  bp::def(
+    "classify_alternatives",
+    &lincs::classify_alternatives,
+    (bp::arg("domain"), "model", "alternatives"),
+    "Classify the provided `alternatives` according to the provided `model`."
+  );
 }
```

### Comparing `lincs-0.1.3/lincs/liblincs/lincs.hpp` & `lincs-0.2.0/lincs/liblincs/lincs.hpp`

 * *Files 22% similar despite different names*

```diff
@@ -20,49 +20,51 @@
       growing,
       // @todo Add decreasing
       // @todo Add single-peaked
       // @todo Add single-valleyed
       // @todo Add unknown
     } category_correlation;
 
-    // @todo Remove these constructors:
+    // @todo Remove these constructors
     // The struct is usable without them in C++, and they were added only to allow using bp::init in the Python module
+    // (Do it for other structs as well)
     Criterion() {}
     Criterion(const std::string& name_, ValueType value_type_, CategoryCorrelation category_correlation_): name(name_), value_type(value_type_), category_correlation(category_correlation_) {}
 
-    // @todo Remove this operator:
+    // @todo Remove this operator
     // The struct is usable without it in C++, and it was added only to allow using bp::vector_indexing_suite in the Python module
+    // (Do it for other structs as well)
     bool operator==(const Criterion& other) const {
       return name == other.name && value_type == other.value_type && category_correlation == other.category_correlation;
     }
   };
 
   std::vector<Criterion> criteria;
 
   struct Category {
     std::string name;
 
-    // @todo Remove these constructors (see Criterion)
     Category() {}
     Category(const std::string& name_): name(name_) {}
 
-    // @todo Remove this operator (see Criterion)
     bool operator==(const Category& other) const { return name == other.name; }
   };
 
   std::vector<Category> categories;
 
   Domain(const std::vector<Criterion>& criteria_, const std::vector<Category>& categories_): criteria(criteria_), categories(categories_) {}
 
   void dump(std::ostream&) const;
   static Domain load(std::istream&);
+
+  static Domain generate(unsigned criteria_count, unsigned categories_count, unsigned random_seed);
 };
 
 struct Model {
-  Domain* domain;
+  const Domain& domain;
 
   struct SufficientCoalitions {
     // Sufficient coalitions form an https://en.wikipedia.org/wiki/Upper_set in the set of parts of the set of criteria.
     // This upset can be defined:
     enum class Kind {
       weights,  // by the weights of the criteria
       // @todo Add upset_roots,  // explicitly by its roots
@@ -76,38 +78,52 @@
 
   struct Boundary {
     std::vector<float> profile;
     SufficientCoalitions sufficient_coalitions;
 
     Boundary() {};
     Boundary(const std::vector<float>& profile_, const SufficientCoalitions& sufficient_coalitions_): profile(profile_), sufficient_coalitions(sufficient_coalitions_) {}
+
+    bool operator==(const Boundary& other) const { return profile == other.profile && sufficient_coalitions.kind == other.sufficient_coalitions.kind && sufficient_coalitions.criterion_weights == other.sufficient_coalitions.criterion_weights; }
   };
 
   std::vector<Boundary> boundaries;  // boundary_index 0 is between category_index 0 and category_index 1
 
-  Model(Domain* domain_, const std::vector<Boundary>& boundaries_) : domain(domain_), boundaries(boundaries_) {}
+  Model(const Domain& domain_, const std::vector<Boundary>& boundaries_) : domain(domain_), boundaries(boundaries_) {}
 
   void dump(std::ostream&) const;
-  static Model load(Domain*, std::istream&);
+  static Model load(const Domain&, std::istream&);
+
+  static Model generate_mrsort(const Domain&, unsigned random_seed);
 };
 
 struct Alternative {
   std::string name;
   std::vector<float> profile;
   std::optional<std::string> category;
 
   Alternative() {}
   Alternative(const std::string& name_, const std::vector<float>& profile_, const std::optional<std::string>& category_): name(name_), profile(profile_), category(category_) {}
+
+  bool operator==(const Alternative& other) const { return name == other.name && profile == other.profile && category == other.category; }
 };
 
-struct AlternativesSet {
-  Domain* domain;
+struct Alternatives {
+  const Domain& domain;
   std::vector<Alternative> alternatives;
 
+  Alternatives(const Domain& domain_, const std::vector<Alternative>& alternatives_): domain(domain_), alternatives(alternatives_) {}
+
   void dump(std::ostream&) const;
-  static AlternativesSet load(Domain*, std::istream&);
+  static Alternatives load(const Domain&, std::istream&);
+
+  static Alternatives generate(const Domain&, const Model&, unsigned alternatives_count, unsigned random_seed);
+};
 
-  AlternativesSet() {}
-  AlternativesSet(Domain* domain_, const std::vector<Alternative>& alternatives_): domain(domain_), alternatives(alternatives_) {}
+struct ClassificationResult {
+  unsigned unchanged;
+  unsigned changed;
 };
 
+ClassificationResult classify_alternatives(const Domain&, const Model&, Alternatives*);
+
 }  // namespace lincs
```

### Comparing `lincs-0.1.3/setup.py` & `lincs-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import setuptools
 
 
-version = "0.1.3"
+version = "0.2.0"
 
 with open("README.md") as f:
     long_description = f.read()
 
 with open("requirements.txt") as f:
     install_requires = f.readlines()
```

