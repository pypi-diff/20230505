# Comparing `tmp/tyro-0.4.2.tar.gz` & `tmp/tyro-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tyro-0.4.2.tar", max compression
+gzip compressed data, was "tyro-0.5.0.tar", max compression
```

## Comparing `tyro-0.4.2.tar` & `tyro-0.5.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     1065 2023-03-12 08:29:12.057639 tyro-0.4.2/LICENSE
--rw-r--r--   0        0        0     4445 2023-03-12 08:30:49.273280 tyro-0.4.2/README.md
--rw-r--r--   0        0        0     1866 2023-03-12 08:29:12.057639 tyro-0.4.2/pyproject.toml
--rw-r--r--   0        0        0      406 2023-03-12 08:29:12.061639 tyro-0.4.2/tyro/__init__.py
--rw-r--r--   0        0        0    17702 2023-03-12 08:29:12.061639 tyro-0.4.2/tyro/_argparse_formatter.py
--rw-r--r--   0        0        0    16635 2023-03-12 08:29:12.061639 tyro-0.4.2/tyro/_arguments.py
--rw-r--r--   0        0        0     8416 2023-03-12 08:29:12.061639 tyro-0.4.2/tyro/_calling.py
--rw-r--r--   0        0        0    15672 2023-03-12 08:29:12.061639 tyro-0.4.2/tyro/_cli.py
--rw-r--r--   0        0        0      101 2023-03-12 08:29:12.061639 tyro-0.4.2/tyro/_deprecated.py
--rw-r--r--   0        0        0    11733 2023-03-12 08:29:12.061639 tyro-0.4.2/tyro/_docstrings.py
--rw-r--r--   0        0        0    29870 2023-03-12 08:29:12.061639 tyro-0.4.2/tyro/_fields.py
--rw-r--r--   0        0        0    19936 2023-03-12 08:29:12.061639 tyro-0.4.2/tyro/_instantiators.py
--rw-r--r--   0        0        0    21122 2023-03-12 08:29:12.061639 tyro-0.4.2/tyro/_parsers.py
--rw-r--r--   0        0        0    11374 2023-03-12 08:29:12.061639 tyro-0.4.2/tyro/_resolver.py
--rw-r--r--   0        0        0      383 2023-03-12 08:29:12.061639 tyro-0.4.2/tyro/_singleton.py
--rw-r--r--   0        0        0     4949 2023-03-12 08:29:12.061639 tyro-0.4.2/tyro/_strings.py
--rw-r--r--   0        0        0     3793 2023-03-12 08:29:12.061639 tyro-0.4.2/tyro/_subcommand_matching.py
--rw-r--r--   0        0        0      764 2023-03-12 08:29:12.061639 tyro-0.4.2/tyro/_typing.py
--rw-r--r--   0        0        0     1206 2023-03-12 08:29:12.061639 tyro-0.4.2/tyro/_unsafe_cache.py
--rw-r--r--   0        0        0      877 2023-03-12 08:29:12.061639 tyro-0.4.2/tyro/conf/__init__.py
--rw-r--r--   0        0        0     1917 2023-03-12 08:29:12.061639 tyro-0.4.2/tyro/conf/_confstruct.py
--rw-r--r--   0        0        0     4926 2023-03-12 08:29:12.061639 tyro-0.4.2/tyro/conf/_markers.py
--rw-r--r--   0        0        0      579 2023-03-12 08:29:12.061639 tyro-0.4.2/tyro/extras/__init__.py
--rw-r--r--   0        0        0     2898 2023-03-12 08:29:12.061639 tyro-0.4.2/tyro/extras/_base_configs.py
--rw-r--r--   0        0        0     1512 2023-03-12 08:29:12.061639 tyro-0.4.2/tyro/extras/_choices_type.py
--rw-r--r--   0        0        0     8196 2023-03-12 08:29:12.061639 tyro-0.4.2/tyro/extras/_serialization.py
--rw-r--r--   0        0        0        0 2023-03-12 08:29:12.061639 tyro-0.4.2/tyro/py.typed
--rw-r--r--   0        0        0     5552 1970-01-01 00:00:00.000000 tyro-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-05-05 08:54:17.782618 tyro-0.5.0/LICENSE
+-rw-r--r--   0        0        0     4445 2023-05-05 08:57:01.487280 tyro-0.5.0/README.md
+-rw-r--r--   0        0        0     1866 2023-05-05 08:54:17.790618 tyro-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0      406 2023-05-05 08:54:17.790618 tyro-0.5.0/tyro/__init__.py
+-rw-r--r--   0        0        0    22530 2023-05-05 08:54:17.790618 tyro-0.5.0/tyro/_argparse_formatter.py
+-rw-r--r--   0        0        0    19546 2023-05-05 08:54:17.790618 tyro-0.5.0/tyro/_arguments.py
+-rw-r--r--   0        0        0     8697 2023-05-05 08:54:17.790618 tyro-0.5.0/tyro/_calling.py
+-rw-r--r--   0        0        0    15642 2023-05-05 08:54:17.790618 tyro-0.5.0/tyro/_cli.py
+-rw-r--r--   0        0        0      101 2023-05-05 08:54:17.790618 tyro-0.5.0/tyro/_deprecated.py
+-rw-r--r--   0        0        0    11749 2023-05-05 08:54:17.790618 tyro-0.5.0/tyro/_docstrings.py
+-rw-r--r--   0        0        0    30130 2023-05-05 08:54:17.790618 tyro-0.5.0/tyro/_fields.py
+-rw-r--r--   0        0        0    23100 2023-05-05 08:54:17.790618 tyro-0.5.0/tyro/_instantiators.py
+-rw-r--r--   0        0        0    21122 2023-05-05 08:54:17.790618 tyro-0.5.0/tyro/_parsers.py
+-rw-r--r--   0        0        0    11374 2023-05-05 08:54:17.790618 tyro-0.5.0/tyro/_resolver.py
+-rw-r--r--   0        0        0      383 2023-05-05 08:54:17.790618 tyro-0.5.0/tyro/_singleton.py
+-rw-r--r--   0        0        0     4949 2023-05-05 08:54:17.790618 tyro-0.5.0/tyro/_strings.py
+-rw-r--r--   0        0        0     3793 2023-05-05 08:54:17.790618 tyro-0.5.0/tyro/_subcommand_matching.py
+-rw-r--r--   0        0        0      764 2023-05-05 08:54:17.790618 tyro-0.5.0/tyro/_typing.py
+-rw-r--r--   0        0        0     1206 2023-05-05 08:54:17.790618 tyro-0.5.0/tyro/_unsafe_cache.py
+-rw-r--r--   0        0        0      921 2023-05-05 08:54:17.790618 tyro-0.5.0/tyro/conf/__init__.py
+-rw-r--r--   0        0        0     1998 2023-05-05 08:54:17.790618 tyro-0.5.0/tyro/conf/_confstruct.py
+-rw-r--r--   0        0        0     5478 2023-05-05 08:54:17.794618 tyro-0.5.0/tyro/conf/_markers.py
+-rw-r--r--   0        0        0      579 2023-05-05 08:54:17.794618 tyro-0.5.0/tyro/extras/__init__.py
+-rw-r--r--   0        0        0     2055 2023-05-05 08:54:17.794618 tyro-0.5.0/tyro/extras/_base_configs.py
+-rw-r--r--   0        0        0     1129 2023-05-05 08:54:17.794618 tyro-0.5.0/tyro/extras/_choices_type.py
+-rw-r--r--   0        0        0     8196 2023-05-05 08:54:17.794618 tyro-0.5.0/tyro/extras/_serialization.py
+-rw-r--r--   0        0        0        0 2023-05-05 08:54:17.794618 tyro-0.5.0/tyro/py.typed
+-rw-r--r--   0        0        0     5552 1970-01-01 00:00:00.000000 tyro-0.5.0/PKG-INFO
```

### Comparing `tyro-0.4.2/LICENSE` & `tyro-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tyro-0.4.2/README.md` & `tyro-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `tyro-0.4.2/pyproject.toml` & `tyro-0.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tyro"
-version = "0.4.2"
+version = "0.5.0"
 description = "Strongly typed, zero-effort CLI interfaces"
 authors = ["brentyi <brentyi@berkeley.edu>"]
 include = ["./tyro/**/*"]
 readme = "README.md"
 repository = "https://github.com/brentyi/tyro"
 homepage = "https://github.com/brentyi/tyro"
 documentation = "https://brentyi.github.io/tyro/"
```

### Comparing `tyro-0.4.2/tyro/_argparse_formatter.py` & `tyro-0.5.0/tyro/_argparse_formatter.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,19 +3,22 @@
     - Are more nicely formatted!
     - Support multiple columns when many fields are defined.
     - Use `rich` for formatting.
     - Can be themed with an accent color.
 
 This is largely built by fussing around in argparse implementation details, and is by
 far the hackiest part of `tyro`.
+
+TODO: we may want to just maintain our own fork of argparse.
 """
 import argparse
 import contextlib
 import dataclasses
 import itertools
+import re as _re
 import shutil
 from typing import Any, ContextManager, Generator, List, Optional
 
 from rich.columns import Columns
 from rich.console import Console, Group, RenderableType
 from rich.padding import Padding
 from rich.panel import Panel
@@ -454,7 +457,126 @@
             return Panel(
                 Group(*item_parts),
                 title=heading,
                 title_align="left",
                 border_style=THEME.border,
                 # padding=(1, 1, 0, 1),
             )
+
+    def _format_actions_usage(self, actions, groups):  #  pragma: no cover
+        """Backporting from Python 3.10, primarily to call format_usage() on actions."""
+
+        # find group indices and identify actions in groups
+        group_actions = set()
+        inserts = {}
+        for group in groups:
+            if not group._group_actions:
+                raise ValueError(f"empty group {group}")
+
+            try:
+                start = actions.index(group._group_actions[0])  # type: ignore
+            except ValueError:
+                continue
+            else:
+                group_action_count = len(group._group_actions)
+                end = start + group_action_count
+                if actions[start:end] == group._group_actions:  # type: ignore
+                    suppressed_actions_count = 0
+                    for action in group._group_actions:
+                        group_actions.add(action)
+                        if action.help is argparse.SUPPRESS:
+                            suppressed_actions_count += 1
+
+                    exposed_actions_count = (
+                        group_action_count - suppressed_actions_count
+                    )
+
+                    if not group.required:
+                        if start in inserts:
+                            inserts[start] += " ["
+                        else:
+                            inserts[start] = "["
+                        if end in inserts:
+                            inserts[end] += "]"
+                        else:
+                            inserts[end] = "]"
+                    elif exposed_actions_count > 1:
+                        if start in inserts:
+                            inserts[start] += " ("
+                        else:
+                            inserts[start] = "("
+                        if end in inserts:
+                            inserts[end] += ")"
+                        else:
+                            inserts[end] = ")"
+                    for i in range(start + 1, end):
+                        inserts[i] = "|"
+
+        # collect all actions format strings
+        parts = []
+        for i, action in enumerate(actions):
+            # suppressed arguments are marked with None
+            # remove | separators for suppressed arguments
+            if action.help is argparse.SUPPRESS:
+                parts.append(None)
+                if inserts.get(i) == "|":
+                    inserts.pop(i)
+                elif inserts.get(i + 1) == "|":
+                    inserts.pop(i + 1)
+
+            # produce all arg strings
+            elif not action.option_strings:
+                default = self._get_default_metavar_for_positional(action)
+                part = self._format_args(action, default)
+
+                # if it's in a group, strip the outer []
+                if action in group_actions:
+                    if part[0] == "[" and part[-1] == "]":
+                        part = part[1:-1]
+
+                # add the action string to the list
+                parts.append(part)
+
+            # produce the first way to invoke the option in brackets
+            else:
+                option_string = action.option_strings[0]
+
+                # if the Optional doesn't take a value, format is:
+                #    -s or --long
+                if action.nargs == 0:
+                    part = (
+                        action.format_usage()
+                        if hasattr(action, "format_usage")
+                        else "%s" % option_string
+                    )
+
+                # if the Optional takes a value, format is:
+                #    -s ARGS or --long ARGS
+                else:
+                    default = self._get_default_metavar_for_optional(action)
+                    args_string = self._format_args(action, default)
+                    part = "%s %s" % (option_string, args_string)
+
+                # make it look optional if it's not required or in a group
+                if not action.required and action not in group_actions:
+                    part = "[%s]" % part
+
+                # add the action string to the list
+                parts.append(part)
+
+        # insert things at the necessary indices
+        for i in sorted(inserts, reverse=True):
+            parts[i:i] = [inserts[i]]
+
+        # join all the action items with spaces
+        text = " ".join([item for item in parts if item is not None])
+
+        # clean up separators for mutually exclusive groups
+        open = r"[\[(]"
+        close = r"[\])]"
+        text = _re.sub(r"(%s) " % open, r"\1", text)
+        text = _re.sub(r" (%s)" % close, r"\1", text)
+        text = _re.sub(r"%s *%s" % (open, close), r"", text)
+        text = text.strip()
+
+        # return the text
+        return text
```

### Comparing `tyro-0.4.2/tyro/_arguments.py` & `tyro-0.5.0/tyro/_arguments.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,15 +4,27 @@
 
 import argparse
 import dataclasses
 import enum
 import functools
 import itertools
 import shlex
-from typing import Any, Dict, Mapping, Optional, Sequence, Set, Tuple, TypeVar, Union
+from typing import (
+    Any,
+    Callable,
+    Dict,
+    Iterable,
+    Mapping,
+    Optional,
+    Sequence,
+    Set,
+    Tuple,
+    TypeVar,
+    Union,
+)
 
 import rich.markup
 import shtab
 
 from . import _fields, _instantiators, _resolver, _strings
 from ._typing import TypeForm
 from .conf import _markers
@@ -21,14 +33,72 @@
     # Python >=3.8.
     from functools import cached_property
 except ImportError:
     # Python 3.7.
     from backports.cached_property import cached_property  # type: ignore
 
 
+_T = TypeVar("_T")
+
+
+# TODO: refactor!
+class BooleanOptionalAction(argparse.Action):
+    """Adapted from https://github.com/python/cpython/pull/27672"""
+
+    def __init__(
+        self,
+        option_strings: Sequence[str],
+        dest: str,
+        default: _T | str | None = None,
+        type: Callable[[str], _T] | argparse.FileType | None = None,
+        choices: Iterable[_T] | None = None,
+        required: bool = False,
+        help: str | None = None,
+        metavar: str | tuple[str, ...] | None = None,
+    ) -> None:
+        _option_strings = []
+        self._no_strings = set()
+        for option_string in option_strings:
+            _option_strings.append(option_string)
+
+            if option_string.startswith("--"):
+                if "." not in option_string:
+                    option_string = "--no-" + option_string[2:]
+                else:
+                    # Loose heuristic for where to add the no- prefix.
+                    left, _, right = option_string.rpartition(".")
+                    option_string = left + ".no-" + right
+                self._no_strings.add(option_string)
+
+                _option_strings.append(option_string)
+
+        super().__init__(
+            option_strings=_option_strings,
+            dest=dest,
+            nargs=0,
+            default=default,
+            type=type,
+            choices=choices,
+            required=required,
+            help=help,
+            metavar=metavar,
+        )
+
+    def __call__(self, parser, namespace, values, option_string=None):
+        if option_string in self.option_strings:
+            assert option_string is not None
+            print(self._no_strings)
+            setattr(namespace, self.dest, option_string not in self._no_strings)
+
+    # Typically only supported in Python 3.10, but we backport some functionality in
+    # _argparse_formatters.py
+    def format_usage(self):
+        return " | ".join(self.option_strings)
+
+
 @dataclasses.dataclass(frozen=True)
 class ArgumentDefinition:
     """Structure containing everything needed to define an argument."""
 
     dest_prefix: str  # True prefix. (eg for the argument's dest field)
     name_prefix: str  # User-facing prefix.
     subcommand_prefix: str  # Prefix for nesting.
@@ -37,34 +107,43 @@
 
     def add_argument(
         self, parser: Union[argparse.ArgumentParser, argparse._ArgumentGroup]
     ) -> None:
         """Add a defined argument to a parser."""
 
         # Get keyword arguments, with None values removed.
-        kwargs = dataclasses.asdict(self.lowered)
+        kwargs = dataclasses.asdict(self.lowered)  # type: ignore
         kwargs.pop("instantiator")
         kwargs = {k: v for k, v in kwargs.items() if v is not None}
         name_or_flag = kwargs.pop("name_or_flag")
         if len(name_or_flag) == 0:
             name_or_flag = _strings.dummy_field_name
 
         # We're actually going to skip the default field: if an argument is unset, the
         # MISSING value will be detected in _calling.py and the field default will
         # directly be used. This helps reduce the likelihood of issues with converting
         # the field default to a string format, then back to the desired type.
-        kwargs["default"] = _fields.MISSING_NONPROP
+        action = kwargs.get("action", None)
+        if action != "append":
+            kwargs["default"] = _fields.MISSING_NONPROP
+        elif action == BooleanOptionalAction:
+            pass
+        else:
+            kwargs["default"] = []
 
         # Apply overrides in our arg configuration object.
         # Note that the `name` field is applied when the field object is instantiated!
         if self.field.argconf.metavar is not None:
             kwargs["metavar"] = self.field.argconf.metavar
 
         # Add argument! Note that the name must be passed in as a position argument.
-        arg = parser.add_argument(name_or_flag, **kwargs)
+        try:
+            arg = parser.add_argument(name_or_flag, **kwargs)
+        except argparse.ArgumentError:
+            return
 
         # Do our best to tab complete paths.
         # There will be false positives here, but if choices is unset they should be
         # harmless.
         if "choices" not in kwargs:
             name_suggests_dir = (
                 # The conditions are intended to be conservative; if a directory path is
@@ -129,15 +208,15 @@
 
     # From here on out, all fields correspond 1:1 to inputs to argparse's
     # add_argument() method.
     name_or_flag: str = ""
     default: Optional[Any] = None
     dest: Optional[str] = None
     required: bool = False
-    action: Optional[str] = None
+    action: Optional[Any] = None
     nargs: Optional[Union[int, str]] = None
     choices: Optional[Set[Any]] = None
     # Note: unlike in vanilla argparse, our metavar is always a string. We handle
     # sequences, multiple arguments, etc, manually.
     metavar: Optional[str] = None
     help: Optional[str] = None
 
@@ -166,26 +245,19 @@
         arg.field.default in _fields.MISSING_SINGLETONS
         or arg.field.is_positional()
         or _markers.FlagConversionOff in arg.field.markers
         or _markers.Fixed in arg.field.markers
     ):
         # Treat bools as a normal parameter.
         return lowered
-    elif arg.field.default is False:
+    elif arg.field.default in (True, False):
         # Default `False` => --flag passed in flips to `True`.
         return dataclasses.replace(
             lowered,
-            action="store_true",
-            instantiator=lambda x: x,  # argparse will directly give us a bool!
-        )
-    elif arg.field.default is True:
-        # Default `True` => --no-flag passed in flips to `False`.
-        return dataclasses.replace(
-            lowered,
-            action="store_false",
+            action=BooleanOptionalAction,
             instantiator=lambda x: x,  # argparse will directly give us a bool!
         )
 
     assert False, (
         f"Expected a boolean as a default for {arg.field.name}, but got"
         f" {lowered.default}."
     )
@@ -211,16 +283,17 @@
             required=False,
             default=_fields.MISSING_PROP,
         )
     if lowered.instantiator is not None:
         return lowered
     try:
         instantiator, metadata = _instantiators.instantiator_from_type(
-            arg.field.typ,  # type: ignore
+            arg.field.typ,
             arg.type_from_typevar,
+            arg.field.markers,
         )
     except _instantiators.UnsupportedTypeAnnotationError as e:
         if arg.field.default in _fields.MISSING_SINGLETONS:
             raise _instantiators.UnsupportedTypeAnnotationError(
                 "Unsupported type annotation for the field"
                 f" {_strings.make_field_name([arg.name_prefix, arg.field.name])}. To"
                 " suppress this error, assign the field a default value."
@@ -231,21 +304,44 @@
             return dataclasses.replace(
                 lowered,
                 metavar="{fixed}",
                 required=False,
                 default=_fields.MISSING_PROP,
             )
 
-    return dataclasses.replace(
-        lowered,
-        instantiator=instantiator,
-        choices=metadata.choices,
-        nargs=metadata.nargs,
-        metavar=metadata.metavar,
-    )
+    if metadata.action == "append":
+
+        def append_instantiator(x: Any) -> Any:
+            out = instantiator(x)
+            if arg.field.default in _fields.MISSING_SINGLETONS:
+                return instantiator(x)
+
+            return type(out)(arg.field.default) + out
+
+            return out
+
+        return dataclasses.replace(
+            lowered,
+            instantiator=append_instantiator,
+            default=None,
+            choices=metadata.choices,
+            nargs=metadata.nargs,
+            metavar=metadata.metavar,
+            action=metadata.action,
+            required=False,
+        )
+    else:
+        return dataclasses.replace(
+            lowered,
+            instantiator=instantiator,
+            choices=metadata.choices,
+            nargs=metadata.nargs,
+            metavar=metadata.metavar,
+            action=metadata.action,
+        )
 
 
 def _rule_convert_defaults_to_strings(
     arg: ArgumentDefinition,
     lowered: LoweredArgumentDefinition,
 ) -> LoweredArgumentDefinition:
     """Sets all default values to strings, as required as input to our instantiator
@@ -308,32 +404,36 @@
     if primary_help is not None and primary_help != "":
         # Note that the percent symbol needs some extra handling in argparse.
         # https://stackoverflow.com/questions/21168120/python-argparse-errors-with-in-help-string
         primary_help = primary_help.replace("%", "%%")
         help_parts.append(_rich_tag_if_enabled(primary_help, "helptext"))
 
     default = lowered.default
-    if lowered.is_fixed():
-        # For fixed args, we'll be missing the lowered default. Use field default
-        # instead.
-        assert default in _fields.MISSING_SINGLETONS
+    if lowered.is_fixed() or lowered.action == "append":
+        # Cases where we'll be missing the lowered default. Use field default instead.
+        assert default in _fields.MISSING_SINGLETONS or default is None
         default = arg.field.default
 
     if not lowered.required:
         # Include default value in helptext. We intentionally don't use the % template
         # because the types of all arguments are set to strings, which will cause the
         # default to be casted to a string and introduce extra quotation marks.
         if lowered.instantiator is None:
             # Intentionally not quoted via shlex, since this can't actually be passed
             # in via the commandline.
             default_text = f"(fixed to: {str(arg.field.default)})"
-        elif lowered.action == "store_true":
-            default_text = f"(sets: {arg.field.name}=True)"
-        elif lowered.action == "store_false":
-            default_text = f"(sets: {arg.field.name}=False)"
+        elif lowered.action == "append" and (
+            arg.field.default in _fields.MISSING_SINGLETONS
+            or len(arg.field.default) == 0
+        ):
+            default_text = "(repeatable)"
+        elif lowered.action == "append" and len(arg.field.default) > 0:
+            assert default is not None  # Just for type checker.
+            default_parts = map(shlex.quote, map(str, default))
+            default_text = f"(repeatable, appends: {' '.join(default_parts)})"
         elif arg.field.default is _fields.EXCLUDE_FROM_CALL:
             default_text = "(unset by default)"
         elif lowered.nargs is not None and hasattr(default, "__iter__"):
             # For tuple types, we might have default as (0, 1, 2, 3).
             # For list types, we might have default as [0, 1, 2, 3].
             # For set types, we might have default as {0, 1, 2, 3}.
             #
@@ -351,40 +451,40 @@
     return dataclasses.replace(lowered, help=" ".join(help_parts))
 
 
 def _rule_set_name_or_flag_and_dest(
     arg: ArgumentDefinition,
     lowered: LoweredArgumentDefinition,
 ) -> LoweredArgumentDefinition:
-    # Positional arguments: no -- prefix.
-    if arg.field.is_positional():
-        name_or_flag = _strings.make_field_name([arg.name_prefix, arg.field.name])
-    # Negated booleans.
-    elif lowered.action == "store_false":
-        name_or_flag = "--" + _strings.make_field_name(
-            [arg.name_prefix, "no-" + arg.field.name]
-        )
+    name_or_flag = _strings.make_field_name(
+        [arg.name_prefix, arg.field.name]
+        if arg.field.argconf.prefix_name
+        else [arg.field.name]
+    )
+
     # Prefix keyword arguments with --.
-    else:
-        name_or_flag = "--" + _strings.make_field_name(
-            [arg.name_prefix, arg.field.name]
-        )
+    if not arg.field.is_positional():
+        name_or_flag = "--" + name_or_flag
 
     # Strip.
     if name_or_flag.startswith("--") and arg.subcommand_prefix != "":
         # This will run even when unused because we want the assert.
         strip_prefix = "--" + arg.subcommand_prefix + "."
         assert name_or_flag.startswith(strip_prefix)
         if _markers.OmitSubcommandPrefixes in arg.field.markers:
             name_or_flag = "--" + name_or_flag[len(strip_prefix) :]
 
     return dataclasses.replace(
         lowered,
         name_or_flag=name_or_flag,
-        dest=_strings.make_field_name([arg.dest_prefix, arg.field.name]),
+        dest=(
+            _strings.make_field_name([arg.dest_prefix, arg.field.name])
+            if arg.field.argconf.prefix_name
+            else arg.field.name
+        ),
     )
 
 
 def _rule_positional_special_handling(
     arg: ArgumentDefinition,
     lowered: LoweredArgumentDefinition,
 ) -> LoweredArgumentDefinition:
```

### Comparing `tyro-0.4.2/tyro/_calling.py` & `tyro-0.5.0/tyro/_calling.py`

 * *Files 5% similar despite different names*

```diff
@@ -38,15 +38,17 @@
     positional_args: List[Any] = []
     kwargs: Dict[str, Any] = {}
     consumed_keywords: Set[str] = set()
 
     def get_value_from_arg(prefixed_field_name: str) -> Any:
         """Helper for getting values from `value_from_arg` + doing some extra
         asserts."""
-        assert prefixed_field_name in value_from_prefixed_field_name
+        assert (
+            prefixed_field_name in value_from_prefixed_field_name
+        ), f"{prefixed_field_name} not in {value_from_prefixed_field_name}"
         return value_from_prefixed_field_name[prefixed_field_name]
 
     arg_from_prefixed_field_name: Dict[str, _arguments.ArgumentDefinition] = {}
     for arg in parser_definition.args:
         arg_from_prefixed_field_name[
             _strings.make_field_name([arg.dest_prefix, arg.field.name])
         ] = arg
@@ -59,17 +61,22 @@
         field_type = field.typ
 
         if prefixed_field_name in arg_from_prefixed_field_name:
             assert prefixed_field_name not in consumed_keywords
 
             # Standard arguments.
             arg = arg_from_prefixed_field_name[prefixed_field_name]
-            consumed_keywords.add(prefixed_field_name)
+            name_maybe_prefixed = (
+                prefixed_field_name
+                if field.argconf.prefix_name
+                else _strings.make_field_name([field.name])
+            )
+            consumed_keywords.add(name_maybe_prefixed)
             if not arg.lowered.is_fixed():
-                value = get_value_from_arg(prefixed_field_name)
+                value = get_value_from_arg(name_maybe_prefixed)
 
                 if value in _fields.MISSING_SINGLETONS:
                     value = arg.field.default
                 else:
                     if arg.lowered.nargs == "?":
                         # Special case for optional positional arguments: this is the
                         # only time that arguments don't come back as a list.
```

### Comparing `tyro-0.4.2/tyro/_cli.py` & `tyro-0.5.0/tyro/_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -251,18 +251,15 @@
     description: Optional[str],
     args: Optional[Sequence[str]],
     default: Optional[OutT],
     return_parser: bool,
     return_unknown_args: bool,
     **deprecated_kwargs,
 ) -> Union[OutT, argparse.ArgumentParser, Tuple[OutT, List[str]],]:
-    """Helper for stitching the `tyro` pipeline together.
-
-    Converts `f` into a
-    """
+    """Helper for stitching the `tyro` pipeline together."""
     if "default_instance" in deprecated_kwargs:
         warnings.warn(
             "`default_instance=` is deprecated! use `default=` instead.", stacklevel=2
         )
         default = deprecated_kwargs["default_instance"]
     if deprecated_kwargs.get("avoid_subparsers", False):
         f = conf.AvoidSubcommands[f]  # type: ignore
```

### Comparing `tyro-0.4.2/tyro/_docstrings.py` & `tyro-0.5.0/tyro/_docstrings.py`

 * *Files 0% similar despite different names*

```diff
@@ -304,15 +304,15 @@
         docstring = f.__init__.__doc__  # type: ignore
     if docstring is None:
         return ""
 
     docstring = _strings.dedent(docstring)
 
     if dataclasses.is_dataclass(f):
-        default_doc = f.__name__ + str(inspect.signature(f)).replace(" -> None", "")
+        default_doc = f.__name__ + str(inspect.signature(f)).replace(" -> None", "")  # type: ignore
         if docstring == default_doc:
             return ""
 
     parsed_docstring = docstring_parser.parse(docstring)
     return "\n".join(
         list(
             filter(
```

### Comparing `tyro-0.4.2/tyro/_fields.py` & `tyro-0.5.0/tyro/_fields.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import collections.abc
 import dataclasses
 import enum
 import functools
 import inspect
 import itertools
 import os
+import sys
 import typing
 import warnings
 from typing import (
     Any,
     Callable,
     Dict,
     FrozenSet,
@@ -75,15 +76,15 @@
         call_argname_override: Optional[Any] = None,
         *,
         markers: Tuple[_markers._Marker, ...] = (),
     ):
         # Try to extract argconf overrides from type.
         _, argconfs = _resolver.unwrap_annotated(typ, _confstruct._ArgConfiguration)
         if len(argconfs) == 0:
-            argconf = _confstruct._ArgConfiguration(None, None, None)
+            argconf = _confstruct._ArgConfiguration(None, None, None, True)
         else:
             assert len(argconfs) == 1
             (argconf,) = argconfs
             helptext = argconf.help
 
         typ, inferred_markers = _resolver.unwrap_annotated(typ, _markers._Marker)
         return FieldDefinition(
@@ -390,21 +391,26 @@
         )
     return field_list
 
 
 def _field_list_from_dataclass(
     cls: TypeForm[Any], default_instance: DefaultInstance
 ) -> Union[List[FieldDefinition], UnsupportedNestedTypeMessage]:
-    # Check if dataclass is a flax module.
     is_flax_module = False
     try:
-        import flax
+        # Check if dataclass is a flax module. This is only possible if flax is already
+        # loaded.
+        #
+        # We generally want to avoid importing flax, since it requires a lot of heavy
+        # imports.
+        if "flax.linen" in sys.modules.keys():
+            import flax.linen
 
-        if issubclass(cls, flax.linen.Module):
-            is_flax_module = True
+            if issubclass(cls, flax.linen.Module):
+                is_flax_module = True
     except ImportError:
         pass
 
     # Handle dataclasses.
     field_list = []
     for dc_field in filter(lambda field: field.init, _resolver.resolved_fields(cls)):
         # For flax modules, we ignore the built-in "name" and "parent" fields.
```

### Comparing `tyro-0.4.2/tyro/_instantiators.py` & `tyro-0.5.0/tyro/_instantiators.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 import os
 import pathlib
 from collections import deque
 from typing import (
     Any,
     Callable,
     Dict,
+    FrozenSet,
     Hashable,
     Iterable,
     List,
     Optional,
     Tuple,
     TypeVar,
     Union,
@@ -59,35 +60,38 @@
     get_args,
     get_origin,
     get_type_hints,
 )
 
 from . import _strings
 from ._typing import TypeForm
+from .conf import _markers
 
 _StandardInstantiator = Callable[[List[str]], Any]
+_AppendNargsInstantiator = Callable[[List[List[str]]], Any]
 # Special case: the only time that argparse doesn't give us a string is when the
 # argument action is set to `store_true` or `store_false`. In this case, we get
 # a bool directly, and the field action can be a no-op.
 _FlagInstantiator = Callable[[bool], bool]
 
-Instantiator = Union[_StandardInstantiator, _FlagInstantiator]
+Instantiator = Union[_StandardInstantiator, _AppendNargsInstantiator, _FlagInstantiator]
 
 NoneType = type(None)
 
 
 @dataclasses.dataclass
 class InstantiatorMetadata:
     # Unlike in vanilla argparse, we never set nargs to None. To make things simpler, we
     # instead use nargs=1.
-    nargs: Union[int, Literal["+"]]
+    nargs: Optional[Union[int, Literal["+"]]]
     # Unlike in vanilla argparse, our metavar is always a string. We handle
     # sequences, multiple arguments, etc, manually.
     metavar: str
     choices: Optional[Tuple[str, ...]]
+    action: Optional[Literal["append"]]
 
     def check_choices(self, strings: List[str]) -> None:
         if self.choices is not None and any(s not in self.choices for s in strings):
             raise ValueError(f"invalid choice: {strings} (choose from {self.choices}))")
 
 
 class UnsupportedTypeAnnotationError(Exception):
@@ -132,15 +136,17 @@
     # Raise an error if parameters look wrong.
     if not (param_count == 1 or (param_count == 0 and has_var_positional)):
         return False
     return True
 
 
 def instantiator_from_type(
-    typ: TypeForm, type_from_typevar: Dict[TypeVar, TypeForm[Any]]
+    typ: TypeForm,
+    type_from_typevar: Dict[TypeVar, TypeForm[Any]],
+    markers: FrozenSet[_markers.Marker],
 ) -> Tuple[Instantiator, InstantiatorMetadata]:
     """Recursive helper for parsing type annotations.
 
     Returns two things:
     - An instantiator function, for instantiating the type from a string or list of
       strings. The latter applies when argparse's `nargs` parameter is set.
     - A metadata structure, which specifies parameters for argparse.
@@ -159,25 +165,26 @@
             assert strings == ["None"]
             return None
 
         return instantiator, InstantiatorMetadata(
             nargs=1,
             metavar="{None}",
             choices=("None",),
+            action=None,
         )
 
     # Instantiate os.PathLike annotations using pathlib.Path.
     # Ideally this should be implemented in a more general way, eg using
     # https://github.com/brentyi/tyro/pull/30
     if typ is os.PathLike:
         typ = pathlib.Path
 
     # Address container types. If a matching container is found, this will recursively
     # call instantiator_from_type().
-    container_out = _instantiator_from_container_type(typ, type_from_typevar)
+    container_out = _instantiator_from_container_type(typ, type_from_typevar, markers)
     if container_out is not None:
         return container_out
 
     # Validate that typ is a `(arg: str) -> T` type converter, as expected by argparse.
     if typ in _builtin_set:
         pass
     elif not callable(typ):
@@ -229,78 +236,87 @@
         nargs=1,
         metavar=(
             typ.__name__.upper()
             if auto_choices is None
             else "{" + ",".join(map(str, auto_choices)) + "}"
         ),
         choices=auto_choices,
+        action=None,
     )
 
 
 @overload
 def _instantiator_from_type_inner(
     typ: TypeForm,
     type_from_typevar: Dict[TypeVar, TypeForm[Any]],
     allow_sequences: Literal["fixed_length"],
+    markers: FrozenSet[_markers.Marker],
 ) -> Tuple[Instantiator, InstantiatorMetadata]:
     ...
 
 
 @overload
 def _instantiator_from_type_inner(
     typ: TypeForm,
     type_from_typevar: Dict[TypeVar, TypeForm[Any]],
     allow_sequences: Literal[False],
+    markers: FrozenSet[_markers.Marker],
 ) -> Tuple[_StandardInstantiator, InstantiatorMetadata]:
     ...
 
 
 @overload
 def _instantiator_from_type_inner(
     typ: TypeForm,
     type_from_typevar: Dict[TypeVar, TypeForm[Any]],
     allow_sequences: Literal[True],
+    markers: FrozenSet[_markers.Marker],
 ) -> Tuple[Instantiator, InstantiatorMetadata]:
     ...
 
 
 def _instantiator_from_type_inner(
     typ: TypeForm,
     type_from_typevar: Dict[TypeVar, TypeForm[Any]],
     allow_sequences: Literal["fixed_length", True, False],
+    markers: FrozenSet[_markers.Marker],
 ) -> Tuple[Instantiator, InstantiatorMetadata]:
     """Thin wrapper over instantiator_from_type, with some extra asserts for catching
     errors."""
-    out = instantiator_from_type(typ, type_from_typevar)
-    if out[1].nargs is not None:
+    out = instantiator_from_type(typ, type_from_typevar, markers)
+    if out[1].nargs == "+":
         # We currently only use allow_sequences=False for options in Literal types,
         # which are evaluated using `type()`. It should not be possible to hit this
         # condition from polling a runtime type.
         assert allow_sequences
         if allow_sequences == "fixed_length" and not isinstance(out[1].nargs, int):
             raise UnsupportedTypeAnnotationError(
-                f"Found an unsupported (variable-length) nested sequence of type {typ}."
+                f"{typ} is a variable-length sequence, which is ambiguous when nested."
+                " For nesting variable-length sequences (example: List[List[int]]),"
+                " `tyro.conf.UseAppendAction` can help resolve ambiguities."
             )
     return out
 
 
 def _instantiator_from_container_type(
-    typ: TypeForm, type_from_typevar: Dict[TypeVar, TypeForm[Any]]
+    typ: TypeForm,
+    type_from_typevar: Dict[TypeVar, TypeForm[Any]],
+    markers: FrozenSet[_markers.Marker],
 ) -> Optional[Tuple[Instantiator, InstantiatorMetadata]]:
     """Attempt to create an instantiator from a container type. Returns `None` is no
     container type is found."""
 
     type_origin = get_origin(typ)
     if type_origin is None:
         return None
 
     # Unwrap Annotated and Final types.
     if type_origin in (Annotated, Final):
         contained_type = get_args(typ)[0]
-        return instantiator_from_type(contained_type, type_from_typevar)
+        return instantiator_from_type(contained_type, type_from_typevar, markers)
 
     for make, matched_origins in {
         _instantiator_from_sequence: (
             collections.abc.Sequence,
             frozenset,
             list,
             set,
@@ -308,43 +324,43 @@
         ),
         _instantiator_from_tuple: (tuple,),
         _instantiator_from_dict: (dict, collections.abc.Mapping),
         _instantiator_from_union: (Union,),
         _instantiator_from_literal: (Literal,),
     }.items():
         if type_origin in matched_origins:
-            return make(typ, type_from_typevar)
+            return make(typ, type_from_typevar, markers)
 
     raise UnsupportedTypeAnnotationError(  # pragma: no cover
         f"Unsupported type {typ} with origin {type_origin}"
     )
 
 
 def _instantiator_from_tuple(
-    typ: TypeForm, type_from_typevar: Dict[TypeVar, TypeForm[Any]]
+    typ: TypeForm,
+    type_from_typevar: Dict[TypeVar, TypeForm[Any]],
+    markers: FrozenSet[_markers.Marker],
 ) -> Tuple[Instantiator, InstantiatorMetadata]:
     types = get_args(typ)
     typeset = set(types)  # Note that sets are unordered.
     typeset_no_ellipsis = typeset - {Ellipsis}  # type: ignore
 
     if typeset_no_ellipsis != typeset:
         # Ellipsis: variable argument counts. When an ellipsis is used, tuples must
         # contain only one type.
         assert len(typeset_no_ellipsis) == 1
-        return _instantiator_from_sequence(typ, type_from_typevar)
+        return _instantiator_from_sequence(typ, type_from_typevar, markers)
 
     else:
         instantiators: List[_StandardInstantiator] = []
         metas: List[InstantiatorMetadata] = []
         nargs = 0
         for t in types:
             a, b = _instantiator_from_type_inner(
-                t,
-                type_from_typevar,
-                allow_sequences="fixed_length",
+                t, type_from_typevar, allow_sequences="fixed_length", markers=markers
             )
             instantiators.append(a)  # type: ignore
             metas.append(b)
             assert isinstance(b.nargs, int)
             nargs += b.nargs
 
         def fixed_length_tuple_instantiator(strings: List[str]) -> Any:
@@ -360,14 +376,15 @@
                 i += meta.nargs
             return tuple(out)
 
         return fixed_length_tuple_instantiator, InstantiatorMetadata(
             nargs=nargs,
             metavar=" ".join(m.metavar for m in metas),
             choices=None,
+            action=None,
         )
 
 
 def _join_union_metavars(metavars: Iterable[str]) -> str:
     """Metavar generation helper for unions. Could be revisited.
 
     Examples:
@@ -400,35 +417,35 @@
         if " " in m:
             merged_metavars[i] = "{" + m + "}"
 
     return "|".join(merged_metavars)
 
 
 def _instantiator_from_union(
-    typ: TypeForm, type_from_typevar: Dict[TypeVar, TypeForm[Any]]
+    typ: TypeForm,
+    type_from_typevar: Dict[TypeVar, TypeForm[Any]],
+    markers: FrozenSet[_markers.Marker],
 ) -> Tuple[Instantiator, InstantiatorMetadata]:
     options = list(get_args(typ))
     if NoneType in options:
         # Move `None` types to the beginning.
         # If we have `Optional[str]`, we want this to be parsed as
         # `Union[NoneType, str]`.
         options.remove(NoneType)
         options.insert(0, NoneType)
 
     # General unions, eg Union[int, bool]. We'll try to convert these from left to
     # right.
     instantiators = []
     metas = []
-    nargs: Union[int, Literal["+"]] = 1
+    nargs: Optional[Union[int, Literal["+"]]] = 1
     first = True
     for t in options:
         a, b = _instantiator_from_type_inner(
-            t,
-            type_from_typevar,
-            allow_sequences=True,
+            t, type_from_typevar, allow_sequences=True, markers=markers
         )
         instantiators.append(a)
         metas.append(b)
 
         if t is not NoneType:
             # Enforce that `nargs` is the same for all child types, except for
             # NoneType.
@@ -472,125 +489,182 @@
             f" {strings}.\n\nGot errors:  \n- " + "\n- ".join(errors)
         )
 
     return union_instantiator, InstantiatorMetadata(
         nargs=nargs,
         metavar=metavar,
         choices=None,
+        action=None,
     )
 
 
 def _instantiator_from_dict(
-    typ: TypeForm, type_from_typevar: Dict[TypeVar, TypeForm[Any]]
+    typ: TypeForm,
+    type_from_typevar: Dict[TypeVar, TypeForm[Any]],
+    markers: FrozenSet[_markers.Marker],
 ) -> Tuple[Instantiator, InstantiatorMetadata]:
     key_type, val_type = get_args(typ)
     key_instantiator, key_meta = _instantiator_from_type_inner(
-        key_type,
-        type_from_typevar,
-        allow_sequences="fixed_length",
-    )
-    val_instantiator, val_meta = _instantiator_from_type_inner(
-        val_type,
-        type_from_typevar,
-        allow_sequences="fixed_length",
+        key_type, type_from_typevar, allow_sequences="fixed_length", markers=markers
     )
 
-    key_nargs = cast(int, key_meta.nargs)  # Casts needed for mypy but not pyright!
-    val_nargs = cast(int, val_meta.nargs)
-    assert isinstance(key_nargs, int)
-    assert isinstance(val_nargs, int)
-    pair_nargs = key_nargs + val_nargs
-
-    def dict_instantiator(strings: List[str]) -> Any:
-        out = {}
-        if len(strings) % pair_nargs != 0:
-            raise ValueError("incomplete set of key value pairs!")
-
-        index = 0
-        for _ in range(len(strings) // pair_nargs):
-            k = strings[index : index + key_nargs]
-            index += key_nargs
-            v = strings[index : index + val_nargs]
-            index += val_nargs
-
-            if key_meta.choices is not None and any(
-                kj not in key_meta.choices for kj in k
-            ):
-                raise ValueError(
-                    f"invalid choice: {k} (choose from {key_meta.choices}))"
-                )
-            if val_meta.choices is not None and any(
-                vj not in val_meta.choices for vj in v
-            ):
-                raise ValueError(
-                    f"invalid choice: {v} (choose from {val_meta.choices}))"
-                )
-            out[key_instantiator(k)] = val_instantiator(v)  # type: ignore
-        return out
-
-    pair_metavar = f"{key_meta.metavar} {val_meta.metavar}"
-    return dict_instantiator, InstantiatorMetadata(
-        nargs="+",
-        metavar=_strings.multi_metavar_from_single(pair_metavar),
-        choices=None,
-    )
+    if _markers.UseAppendAction in markers:
+        val_instantiator, val_meta = _instantiator_from_type_inner(
+            val_type,
+            type_from_typevar,
+            allow_sequences=True,
+            markers=markers - {_markers.UseAppendAction},
+        )
+        pair_metavar = f"{key_meta.metavar} {val_meta.metavar}"
+        key_nargs = cast(int, key_meta.nargs)  # Casts needed for mypy but not pyright!
+        val_nargs = val_meta.nargs
+        assert isinstance(key_nargs, int)
+
+        def append_dict_instantiator(strings: List[List[str]]) -> Any:
+            out = {}
+            for s in strings:
+                out[key_instantiator(s[:key_nargs])] = val_instantiator(s[key_nargs:])  # type: ignore
+            return out
+
+        return append_dict_instantiator, InstantiatorMetadata(
+            nargs=key_nargs + val_nargs if isinstance(val_nargs, int) else "+",
+            metavar=pair_metavar,
+            choices=None,
+            action="append",
+        )
+    else:
+        val_instantiator, val_meta = _instantiator_from_type_inner(
+            val_type, type_from_typevar, allow_sequences="fixed_length", markers=markers
+        )
+        pair_metavar = f"{key_meta.metavar} {val_meta.metavar}"
+        key_nargs = cast(int, key_meta.nargs)  # Casts needed for mypy but not pyright!
+        val_nargs = cast(int, val_meta.nargs)
+        assert isinstance(key_nargs, int)
+        assert isinstance(val_nargs, int)
+        pair_nargs = key_nargs + val_nargs
+
+        def dict_instantiator(strings: List[str]) -> Any:
+            out = {}
+            if len(strings) % pair_nargs != 0:
+                raise ValueError("incomplete set of key value pairs!")
+
+            index = 0
+            for _ in range(len(strings) // pair_nargs):
+                assert isinstance(key_nargs, int)
+                assert isinstance(val_nargs, int)
+                k = strings[index : index + key_nargs]
+                index += key_nargs
+                v = strings[index : index + val_nargs]
+                index += val_nargs
+
+                if key_meta.choices is not None and any(
+                    kj not in key_meta.choices for kj in k
+                ):
+                    raise ValueError(
+                        f"invalid choice: {k} (choose from {key_meta.choices}))"
+                    )
+                if val_meta.choices is not None and any(
+                    vj not in val_meta.choices for vj in v
+                ):
+                    raise ValueError(
+                        f"invalid choice: {v} (choose from {val_meta.choices}))"
+                    )
+                out[key_instantiator(k)] = val_instantiator(v)  # type: ignore
+            return out
+
+        return dict_instantiator, InstantiatorMetadata(
+            nargs="+",
+            metavar=_strings.multi_metavar_from_single(pair_metavar),
+            choices=None,
+            action=None,
+        )
 
 
 def _instantiator_from_sequence(
-    typ: TypeForm, type_from_typevar: Dict[TypeVar, TypeForm[Any]]
+    typ: TypeForm,
+    type_from_typevar: Dict[TypeVar, TypeForm[Any]],
+    markers: FrozenSet[_markers.Marker],
 ) -> Tuple[Instantiator, InstantiatorMetadata]:
     """Instantiator for variable-length sequences: list, sets, Tuple[T, ...], etc."""
     container_type = get_origin(typ)
     if container_type is collections.abc.Sequence:
         container_type = list
 
     if container_type is tuple:
         (contained_type, ell) = get_args(typ)
         assert ell == Ellipsis
     else:
         (contained_type,) = get_args(typ)
 
-    make, inner_meta = _instantiator_from_type_inner(
-        contained_type,
-        type_from_typevar,
-        allow_sequences="fixed_length",
-    )
+    if _markers.UseAppendAction in markers:
+        make, inner_meta = _instantiator_from_type_inner(
+            contained_type,
+            type_from_typevar,
+            allow_sequences=True,
+            markers=markers - {_markers.UseAppendAction},
+        )
 
-    def sequence_instantiator(strings: List[str]) -> Any:
-        # Validate nargs.
-        assert type(inner_meta.nargs) in (int, NoneType)
-        if isinstance(inner_meta.nargs, int) and len(strings) % inner_meta.nargs != 0:
-            raise ValueError(
-                f"input {strings} is of length {len(strings)}, which is not divisible"
-                f" by {inner_meta.nargs}."
-            )
+        def append_sequence_instantiator(strings: Optional[List[List[str]]]) -> Any:
+            if strings is None:
+                assert container_type is not None
+                return container_type()
+            return container_type(make(s) for s in strings)  # type: ignore
+
+        return append_sequence_instantiator, InstantiatorMetadata(
+            nargs=inner_meta.nargs,
+            metavar=inner_meta.metavar,
+            choices=inner_meta.choices,
+            action="append",
+        )
+    else:
+        make, inner_meta = _instantiator_from_type_inner(
+            contained_type,
+            type_from_typevar,
+            allow_sequences="fixed_length",
+            markers=markers,
+        )
 
-        # Make tuple.
-        out = []
-        step = inner_meta.nargs if isinstance(inner_meta.nargs, int) else 1
-        for i in range(0, len(strings), step):
-            out.append(make(strings[i : i + inner_meta.nargs]))  # type: ignore
-        assert container_type is not None
-        return container_type(out)
-
-    return sequence_instantiator, InstantiatorMetadata(
-        nargs="+",
-        metavar=_strings.multi_metavar_from_single(inner_meta.metavar),
-        choices=inner_meta.choices,
-    )
+        def sequence_instantiator(strings: List[str]) -> Any:
+            # Validate nargs.
+            if (
+                isinstance(inner_meta.nargs, int)
+                and len(strings) % inner_meta.nargs != 0
+            ):
+                raise ValueError(
+                    f"input {strings} is of length {len(strings)}, which is not"
+                    f" divisible by {inner_meta.nargs}."
+                )
+
+            # Make tuple.
+            out = []
+            step = inner_meta.nargs if isinstance(inner_meta.nargs, int) else 1
+            for i in range(0, len(strings), step):
+                out.append(make(strings[i : i + inner_meta.nargs]))  # type: ignore
+            assert container_type is not None
+            return container_type(out)
+
+        return sequence_instantiator, InstantiatorMetadata(
+            nargs="+",
+            metavar=_strings.multi_metavar_from_single(inner_meta.metavar),
+            choices=inner_meta.choices,
+            action=None,
+        )
 
 
 def _instantiator_from_literal(
-    typ: TypeForm, type_from_typevar: Dict[TypeVar, TypeForm[Any]]
+    typ: TypeForm,
+    type_from_typevar: Dict[TypeVar, TypeForm[Any]],
+    markers: FrozenSet[_markers.Marker],
 ) -> Tuple[Instantiator, InstantiatorMetadata]:
     choices = get_args(typ)
     str_choices = tuple(x.name if isinstance(x, enum.Enum) else str(x) for x in choices)
     return (
         # Note that if string is not in str_choices, it will be caught from setting
         # `choices` below.
         lambda strings: choices[str_choices.index(strings[0])],
         InstantiatorMetadata(
             nargs=1,
             metavar="{" + ",".join(str_choices) + "}",
             choices=str_choices,
+            action=None,
         ),
     )
```

### Comparing `tyro-0.4.2/tyro/_parsers.py` & `tyro-0.5.0/tyro/_parsers.py`

 * *Files identical despite different names*

### Comparing `tyro-0.4.2/tyro/_resolver.py` & `tyro-0.5.0/tyro/_resolver.py`

 * *Files identical despite different names*

### Comparing `tyro-0.4.2/tyro/_strings.py` & `tyro-0.5.0/tyro/_strings.py`

 * *Files identical despite different names*

### Comparing `tyro-0.4.2/tyro/_subcommand_matching.py` & `tyro-0.5.0/tyro/_subcommand_matching.py`

 * *Files identical despite different names*

### Comparing `tyro-0.4.2/tyro/_typing.py` & `tyro-0.5.0/tyro/_typing.py`

 * *Files identical despite different names*

### Comparing `tyro-0.4.2/tyro/_unsafe_cache.py` & `tyro-0.5.0/tyro/_unsafe_cache.py`

 * *Files identical despite different names*

### Comparing `tyro-0.4.2/tyro/conf/__init__.py` & `tyro-0.5.0/tyro/conf/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,23 +14,25 @@
     ConsolidateSubcommandArgs,
     Fixed,
     FlagConversionOff,
     OmitSubcommandPrefixes,
     Positional,
     Suppress,
     SuppressFixed,
+    UseAppendAction,
     configure,
 )
 
 __all__ = [
     "arg",
     "subcommand",
     "AvoidSubcommands",
     "ConsolidateSubcommandArgs",
     "Fixed",
     "FlagConversionOff",
     "OmitSubcommandPrefixes",
     "Positional",
     "Suppress",
     "SuppressFixed",
+    "UseAppendAction",
     "configure",
 ]
```

### Comparing `tyro-0.4.2/tyro/conf/_confstruct.py` & `tyro-0.5.0/tyro/conf/_confstruct.py`

 * *Files 8% similar despite different names*

```diff
@@ -56,25 +56,31 @@
 
 
 @dataclasses.dataclass(frozen=True)
 class _ArgConfiguration:
     name: Optional[str]
     metavar: Optional[str]
     help: Optional[str]
-    # TODO - add prefix_name: bool
+    prefix_name: bool
 
 
 def arg(
     *,
     name: Optional[str] = None,
     metavar: Optional[str] = None,
     help: Optional[str] = None,
+    prefix_name: bool = True,
 ) -> Any:
     """Returns a metadata object for configuring arguments with `typing.Annotated`.
     Useful for aesthetics.
 
     Usage:
     ```python
     x: Annotated[int, tyro.conf.arg(...)]
     ```
     """
-    return _ArgConfiguration(name=name, metavar=metavar, help=help)
+    return _ArgConfiguration(
+        name=name,
+        metavar=metavar,
+        help=help,
+        prefix_name=prefix_name,
+    )
```

### Comparing `tyro-0.4.2/tyro/conf/_markers.py` & `tyro-0.5.0/tyro/conf/_markers.py`

 * *Files 5% similar despite different names*

```diff
@@ -84,14 +84,27 @@
 
     cmd: Union[NestedTypeA, NestedTypeB]
 
 By default, `--cmd.arg` may be generated as a flag for each dataclass in the union.
 If subcommand prefixes are omitted, we would instead simply have `--arg`.
 """
 
+UseAppendAction = Annotated[T, None]
+"""Use "append" actions for variable-length arguments.
+
+Given an annotation like `x: List[int]`, this means that `x = [0, 1, 2]` can be set via
+the CLI syntax `--x 0 --x 1 --x 2` instead of the default of `--x 0 1 2`.
+
+The resulting syntax may be more user-friendly; for `tyro`, it also enables support for
+otherwise ambiguous annotations like `List[List[int]]`.
+
+Can be applied to all variable-length sequences (`List[T]`, `Sequence[T]`,
+`Tuple[T, ...]`, etc), including dictionaries without default values.
+"""
+
 CallableType = TypeVar("CallableType", bound=Callable)
 
 # Dynamically generate marker singletons.
 # These can be used one of two ways:
 # - Marker[T]
 # - Annotated[T, Marker]
 
@@ -113,15 +126,15 @@
     ```python
     field: tyro.conf.FlagConversionOff[bool]
     ```
 
     This decorator makes markers applicable to general functions as well:
 
     ```python
-    # Recursively apply FlagConversionOff to all field in `main()`.
+    # Recursively apply FlagConversionOff to all fields in `main()`.
     @tyro.conf.configure(tyro.conf.FlagConversionOff)
     def main(field: bool) -> None:
         ...
     ```
     """
 
     def _inner(callable: CallableType) -> CallableType:
```

### Comparing `tyro-0.4.2/tyro/extras/__init__.py` & `tyro-0.5.0/tyro/extras/__init__.py`

 * *Files identical despite different names*

### Comparing `tyro-0.4.2/tyro/extras/_serialization.py` & `tyro-0.5.0/tyro/extras/_serialization.py`

 * *Files identical despite different names*

### Comparing `tyro-0.4.2/PKG-INFO` & `tyro-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tyro
-Version: 0.4.2
+Version: 0.5.0
 Summary: Strongly typed, zero-effort CLI interfaces
 Home-page: https://github.com/brentyi/tyro
 Author: brentyi
 Author-email: brentyi@berkeley.edu
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

