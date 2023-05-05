# Comparing `tmp/appeal-0.5.8.tar.gz` & `tmp/appeal-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "appeal-0.5.8.tar", last modified: Thu May  4 07:00:10 2023, max compression
+gzip compressed data, was "appeal-0.5.9.tar", last modified: Fri May  5 07:28:01 2023, max compression
```

## Comparing `appeal-0.5.8.tar` & `appeal-0.5.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0       19 2022-01-26 11:06:53.000000 appeal-0.5.8/.gitignore
--rw-r--r--   0        0        0     1090 2023-05-02 08:25:22.598769 appeal-0.5.8/LICENSE
--rw-r--r--   0        0        0    68258 2023-05-04 06:59:09.308913 appeal-0.5.8/README.md
--rw-r--r--   0        0        0   174135 2023-05-04 06:53:52.222431 appeal-0.5.8/appeal/__init__.py
--rw-r--r--   0        0        0    23346 2023-05-02 08:25:22.602769 appeal-0.5.8/appeal/argument_grouping.py
--rw-r--r--   0        0        0     4637 2022-02-12 23:26:33.980913 appeal-0.5.8/appeal/cpp.py
--rw-r--r--   0        0        0    19692 2023-05-02 08:26:43.265271 appeal-0.5.8/appeal/text.py
--rw-r--r--   0        0        0      537 2023-05-02 08:26:43.265271 appeal-0.5.8/pyproject.toml
--rw-r--r--   0        0        0    50634 2022-01-26 11:06:53.000000 appeal-0.5.8/resources/images/appeal.logo.png
--rw-r--r--   0        0        0    18772 2022-01-26 11:06:53.000000 appeal-0.5.8/resources/images/give.your.program.appeal.png
--rw-r--r--   0        0        0      125 2022-01-26 11:06:53.000000 appeal-0.5.8/resources/links.txt
--rw-r--r--   0        0        0    67934 2023-05-04 06:53:04.228844 appeal-0.5.8/tests/run_tests.py
--rw-r--r--   0        0        0    68752 1970-01-01 00:00:00.000000 appeal-0.5.8/PKG-INFO
+-rw-r--r--   0        0        0       19 2022-01-26 11:06:53.000000 appeal-0.5.9/.gitignore
+-rw-r--r--   0        0        0     1090 2023-05-02 08:25:22.598769 appeal-0.5.9/LICENSE
+-rw-r--r--   0        0        0    69688 2023-05-05 07:27:29.162568 appeal-0.5.9/README.md
+-rw-r--r--   0        0        0   168554 2023-05-05 07:15:41.683718 appeal-0.5.9/appeal/__init__.py
+-rw-r--r--   0        0        0    23888 2023-05-05 07:12:51.458204 appeal-0.5.9/appeal/argument_grouping.py
+-rw-r--r--   0        0        0     4637 2022-02-12 23:26:33.980913 appeal-0.5.9/appeal/cpp.py
+-rw-r--r--   0        0        0    19692 2023-05-02 08:26:43.265271 appeal-0.5.9/appeal/text.py
+-rw-r--r--   0        0        0      537 2023-05-02 08:26:43.265271 appeal-0.5.9/pyproject.toml
+-rw-r--r--   0        0        0    50634 2022-01-26 11:06:53.000000 appeal-0.5.9/resources/images/appeal.logo.png
+-rw-r--r--   0        0        0    18772 2022-01-26 11:06:53.000000 appeal-0.5.9/resources/images/give.your.program.appeal.png
+-rw-r--r--   0        0        0      125 2022-01-26 11:06:53.000000 appeal-0.5.9/resources/links.txt
+-rw-r--r--   0        0        0    67934 2023-05-05 04:50:34.315935 appeal-0.5.9/tests/run_tests.py
+-rw-r--r--   0        0        0    70182 1970-01-01 00:00:00.000000 appeal-0.5.9/PKG-INFO
```

### Comparing `appeal-0.5.8/LICENSE` & `appeal-0.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `appeal-0.5.8/README.md` & `appeal-0.5.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-![## Appeal](/resources/images/appeal.logo.png)
+![## Appeal](https://raw.githubusercontent.com/larryhastings/appeal/master/resources/images/appeal.logo.png)
 
-![## Give your program Appeal!](/resources/images/give.your.program.appeal.png)
+![## Give your program Appeal!](https://raw.githubusercontent.com/larryhastings/appeal/master/resources/images/give.your.program.appeal.png)
 
 ##### Copyright 2021-2023 by Larry Hastings
 
 
 ## Quickstart
 
 ```Python
@@ -1965,14 +1965,39 @@
   for any keyword-only parameter to a converter or command function.
 * The converter for a *var_positional* (`*args`) parameter
   *must* require at least one positional argument.
 
 
 ## Changelog
 
+**0.5.9**
+
+* Improved the error message generated when you have a
+  required parameter after a `VAR_POSITIONAL` parameter.
+  (This command-line can never succeed, because the
+  `VAR_POSITIONAL` consumes all remaining arguments on
+  the command-line, which means the subsequent required
+  parameter can never be satisfied.)  Fixes #6.
+* Changed README to use absolute instead of relative links
+  for images, which means images should now render properly
+  on the Appeal page at PyPI.  Thanks for the PR, Hugo!
+* Switched a bunch of internal classes to use Python "slots".
+  Hopefully a tiny memory and speed optimization.
+* Remove unused / unneeded stuff:
+    * unused `partial_replace*` functions
+    * unused Charm bytecode instructions `jump_relative` and `load_o_option`
+    * unneeded CharmInterpreter register `option` (only used in one error
+      message, obviated by instead using the program name directly)
+* Now that Appeal depends on [**big**](https://github.com/larryhastings/big)
+  anyway, switch to
+  [**big**'s `PushbackIterator`.](https://github.com/larryhastings/big#pushbackiteratoriterablenone).
+* Add peephole optimizer step for jump-to-jump optimization.
+  Honestly this was probably unnecessary, as I don't think Appeal's
+  compiler can even *generate* code with jumps-to-jumps (yet).
+
 **0.5.8**
 
 * Fixed up the "name" of the program for options.  We used to take
   the name of the command, add all the option strings, and join it
   together with commas, as in `'command, -o, --option'`.  Now it
   looks like `'command -o | --option'`.
 * Fixed presentation bug: if you didn't have enough positional
```

### Comparing `appeal-0.5.8/appeal/__init__.py` & `appeal-0.5.9/appeal/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python3
 
 "A powerful & Pythonic command-line parsing library.  Give your program Appeal!"
-__version__ = "0.5.8"
+__version__ = "0.5.9"
 
 
 # please leave this copyright notice in binary distributions.
 license = """
 appeal/__init__.py
 part of the Appeal software package
 Copyright 2021-2023 by Larry Hastings
@@ -32,14 +32,15 @@
 
 want_prints = 1
 want_prints = 0
 
 
 from abc import abstractmethod, ABCMeta
 import big.all as big
+from big.itertools import PushbackIterator
 import builtins
 import collections
 import enum
 import functools
 import inspect
 import itertools
 import math
@@ -105,109 +106,14 @@
     """
     functools.update_wrapper(wrapped, wrapper)
     if hasattr(wrapped, '__wrapped__'):
         delattr(wrapped, '__wrapped__')
     return wrapped
 
 
-# copied and pasted in from "big"
-# because I'm too lazy to make appeal depend on big
-# (for now)
-class PushbackIterator:
-    """
-    Wraps any iterator, allowing you to push items back on the iterator.
-    This allows you to "peek" at the next item (or items); you can get the
-    next item, examine it, and then push it back.  If any objects have
-    been pushed onto the iterator, they are yielded first, before attempting
-    to yield from the wrapped iterator.
-
-    Pass in any iterable to the constructor.  Passing in an iterable of None
-    means the PushbackIterator is created in an exhausted state.
-
-    When the wrapped iterable is exhausted (or if you passed in None to
-    the constructor) you can still call push to add new items, at which
-    point the PushBackIterator can be iterated over again.
-    """
-    def __init__(self, iterable=None):
-        if (iterable != None) and (not hasattr(iterable, '__next__')):
-            iterable = iter(iterable)
-        self.i = iterable
-        self.stack = []
-
-    def __iter__(self):
-        return self
-
-    def push(self, o):
-        """
-        Pushes a value into the iterator's internal stack.
-        When a PushbackIterator is iterated over, and there are
-        any pushed values, the top value on the stack will be popped
-        and yielded.  PushbackIterator only yields from the
-        iterator it wraps when this internal stack is empty.
-        """
-        self.stack.append(o)
-
-    def __next__(self):
-        if self.stack:
-            return self.stack.pop()
-        if self.i:
-            return next(self.i)
-        raise StopIteration
-
-    def next(self, default=None):
-        """
-        Equivalent to next(PushbackIterator),
-        but won't raise StopIteration.
-        If the iterator is exhausted, returns
-        the "default" argument.
-        """
-        if self.stack:
-            return self.stack.pop()
-        if not self.i:
-            return default
-        try:
-            return next(self.i)
-        except StopIteration:
-            self.i = None
-            return default
-
-    def __bool__(self):
-        if self.stack:
-            return True
-        if not self.i:
-            return False
-        try:
-            o = next(self.i)
-            self.push(o)
-            return True
-        except StopIteration:
-            return False
-
-    # this is used for debugging,
-    # it doesn't have to be performant
-    @property
-    def values(self):
-        if self.i:
-            values = list(self.i)
-            values.reverse()
-            values.extend(self.stack)
-            # keep the same arrya object for stack
-            # just in case someone naughty has a reference
-            self.stack.clear()
-            self.stack.extend(values)
-            self.i = False
-        values = self.stack.copy()
-        values.reverse()
-        return tuple(values)
-
-    def __repr__(self):
-        return f"<{self.__class__.__name__} i={self.i} stack={self.stack}>"
-
-
-
 
 class DictGetattrProxy:
     def __init__(self, d, repr_string):
         self.__d__ = d
         self.__repr_string__ = repr_string
 
     def __repr__(self):
@@ -289,14 +195,16 @@
 #
 # is wrong, the user must call appeal.split:
 #
 #    @app.command()
 #    def my_command(a:appeal.split()):
 #        ...
 #
+# this just adds a field we can check for, and if we find
+# it we throw a helpful exception so the user can fix it.
 def must_be_instance(callable):
     callable.__appeal_must_be_instance__ = True
     return callable
 
 
 def is_legal_annotation(annotation):
     if getattr(annotation, "__appeal_must_be_instance__", False):
@@ -385,92 +293,14 @@
     If all those statements are true, this function:
         * extracts the callable from the partial,
         * uses getattr(self, callable.__name__) to
           bind callable to self.
     """
     return _partial_rebind(partial, placeholder, instance, False)
 
-def partial_replace_map(partial, map):
-    """
-    Replaces curried values in a functools.partial()
-    object.  The map should be of the form
-        {old: new}
-    where "old" is a curried value in partial,
-    which will be replaced with "new".
-
-    Returns a new partial object with:
-        * all positional values matching "old"
-          replaced with "new", and
-        * all keyword-only values whose value
-          matches "old" replaced with "new".
-
-    "old" values that don't appear as a curried
-    value in partial are ignored and harmless.
-    """
-    func = partial.func
-    if isinstance(func, functools.partial):
-        func = partial_replace_map(func, map)
-    new_args = []
-    for value in partial.args:
-        new_args.append(map.get(value, value))
-    new_kwargs = {}
-    for key, value in partial.keywords.items():
-        new_kwargs[key] = map.get(value, value)
-    func2 = functools.partial(func, *new_args, **new_kwargs)
-    update_wrapper(func2, func)
-    return func2
-
-
-def partial_replace(partial, **kwargs):
-    """
-    Keyword-argument convience wrapper function
-    for partial_replace_map().
-    """
-    return partial_replace_map(partial, kwargs)
-
-def partial_replace_map_self(partial, map):
-    """
-    Does the same thing as partial_replace_map(),
-    with one exception: the first positional value
-    curried by the partial object is treated like
-    a "self" object, and the curried function is
-    assumed to be an unbound method.  For maximum
-    compatibility, and *only* in this case,
-    partial_replace_map_self will call
-    getattr() on this "self" object to create a
-    bound method version of fn by looking it up
-    *by name*.
-    """
-    func = partial.func
-    args = partial.args
-    kwargs = partial.keywords
-    if isinstance(func, functools.partial):
-        func = partial_replace_map_self(func, map)
-    elif args:
-        args = list(args)
-        self = args.pop(0)
-        self = map.get(self, self)
-        # print(f"Handled a self {self!r}")
-        name = func.__name__
-        assert hasattr(self, name)
-        func = getattr(self, name)
-        if not (args or kwargs):
-            return func
-    new_args = []
-    for value in args:
-        new_args.append(map.get(value, value))
-    new_kwargs = {}
-    for key, value in kwargs.items():
-        new_kwargs[key] = map.get(value, value)
-    func2 = functools.partial(func, *new_args, **new_kwargs)
-    update_wrapper(func2, func)
-    return func2
-
-def no_op_prepare(fn):
-    return fn
 
 ##
 ## charm
 ##
 ## Charm is a simple "bytecode" language.
 ## Appeal uses Charm to represent mapping
 ## an Appeal "command" function to the command-line.
@@ -584,21 +414,19 @@
         i += 1
 
 print('class opcode(enum.Enum):')
 
 print_enum('''
     invalid
     jump
-    jump_relative
     branch_on_o
     call
     create_converter
     load_converter
     load_o
-    load_o_option
     append_args
     store_kwargs
     map_option
     consume_argument
     flush_multioption
     set_group
     push_context
@@ -633,31 +461,28 @@
 # Modify the code in the quotes above and run
 #         % python3 cpp.py __init__.py
 # to regenerate.
 
 class opcode(enum.Enum):
     invalid = 0
     jump = 1
-    jump_relative = 2
-    branch_on_o = 3
-    call = 4
-    create_converter = 5
-    load_converter = 6
-    load_o = 7
-    load_o_context = 8
-    load_o_option = 9
-    append_args = 10
-    store_kwargs = 11
-    map_option = 12
-    consume_argument = 13
-    flush_multioption = 14
-    set_group = 15
-    push_context = 16
-    pop_context = 17
-    end = 18
+    branch_on_o = 2
+    call = 3
+    create_converter = 4
+    load_converter = 5
+    load_o = 6
+    append_args = 7
+    store_kwargs = 8
+    map_option = 9
+    consume_argument = 10
+    flush_multioption = 11
+    set_group = 12
+    push_context = 13
+    pop_context = 14
+    end = 15
 
     # these are removed by the peephole optimizer.
     # the interpreter never sees them.
     # (well... unless you leave in comments during debugging.)
 
     no_op = 100
     comment = 101
@@ -665,99 +490,80 @@
     jump_to_label = 103
     branch_on_o_to_label = 104
 
 # cpp
 
 
 class CharmInstruction:
-    op = opcode.invalid
+    __slots__ = ['op']
 
     def copy(self):
         kwargs = {attr: getattr(self, attr) for attr in dir(self) if not (attr.startswith("_") or (attr in ("copy", "op"))) }
         return self.__class__(**kwargs)
 
-class CharmInstructionNoArgBase(CharmInstruction):
-    # __slots__ = []
-    def __repr__(self):
-        return f"<{str(self.op).partition('.')[2]}>"
-
-class CharmInstructionAddressBase(CharmInstruction):
-    # __slots__ = ['address']
 
-    def __init__(self, address):
-        self.address = address
-
-    def __repr__(self):
-        return f"<{str(self.op).partition('.')[2]} address={self.address}>"
-
-class CharmInstructionKeyBase(CharmInstruction):
-    # __slots__ = ['key']
-
-    def __init__(self, key):
-        self.key = key
-
-    def __repr__(self):
-        return f"<{str(self.op).partition('.')[2]} key={self.key}>"
-
-class CharmInstructionLabelBase(CharmInstruction):
-    # __slots__ = ['label']
-
-    def __init__(self, label):
-        self.label = label
-
-    def __repr__(self):
-        return f"<{str(self.op).partition('.')[2]} label={self.label!r}>"
 
 class CharmInstructionComment(CharmInstruction):
-    # __slots__ = ['comment']
-    op = opcode.comment
+    __slots__ = ['comment']
 
     def __init__(self, comment):
+        self.op = opcode.comment
         self.comment = comment
 
     def __repr__(self):
         return f"<comment {self.comment!r}>"
 
-class CharmInstructionNoOp(CharmInstructionNoArgBase):
-    op = opcode.no_op
-
-class CharmInstructionJumpRelative(CharmInstruction):
-    """
-    jump_relative <offset>
 
-    Adds <offset> to the 'ip' register.
-    <offset> is an integer, and may be negative.
-    """
-    op = opcode.jump_relative
-    # __slots__ = ['offset']
+class CharmInstructionNoOp(CharmInstruction): # CharmInstructionNoArgBase
 
-    def __init__(self, offset):
-        self.offset = offset
+    def __init__(self):
+        self.op = opcode.no_op
 
     def __repr__(self):
-        return f"<jump_relative offset={self.offset}>"
+        return f"<no-op>"
 
-class CharmInstructionJump(CharmInstructionAddressBase):
+
+class CharmInstructionJump(CharmInstruction): # CharmInstructionAddressBase
     """
     jump <address>
 
     Sets the 'ip' register to <address>.
     <address> is an integer.
     """
-    op = opcode.jump
 
-class CharmInstructionBranchOnO(CharmInstructionAddressBase):
+    __slots__ = ['address']
+
+    def __init__(self, address):
+        self.op = opcode.jump
+        self.address = address
+
+    def __repr__(self):
+        return f"<jump address={self.address}>"
+
+
+class CharmInstructionBranchOnO(CharmInstruction): # CharmInstructionAddressBase
     """
     branch_on_o <address>
 
     If the 'o' register is a true value,
     sets the 'ip' register to <address>.
     <address> is an integer.
     """
-    op = opcode.branch_on_o
+
+    __slots__ = ['address']
+
+    def __init__(self, address):
+        self.op = opcode.branch_on_o
+        self.address = address
+
+    def __repr__(self):
+        return f"<branch_on_o address={self.address}>"
+
+
+label_id_counter = 0
 
 class CharmInstructionLabel(CharmInstruction):
     """
     label <name>
 
     Sets a destination in the program that can be
     jumped to by the jump_to_label instruction.
@@ -765,126 +571,149 @@
     <name> may be nearly any Python value; the value
     must support basic mathematical properties:
     reflexive, symmetric, transitive, substitution, etc.
 
     label and *_to_label are both pseudo-instructions.
     They're removed by a pass in the peephole optimizer.
     """
-    op = opcode.label
-    # __slots__ = ['id', 'name']
-
-    label_id_counter = 0
+    __slots__ = ['id', 'label']
 
-    def __init__(self, name=''):
-        CharmInstructionLabel.label_id_counter += 1
-        self.id = CharmInstructionLabel.label_id_counter
-        self.name = name
+    def __init__(self, label):
+        global label_id_counter
+        self.op = opcode.label
+        label_id_counter += 1
+        self.id = label_id_counter
+        self.label = label
 
     def __repr__(self):
-        print_name = f" name={self.name!r}" if self.name else ""
-        return f"<label id={self.id}{print_name}>"
+        opcode = str(self.op).rpartition('.')[2]
+        label = f" label={self.label!r}" if self.label else ""
+        return f"<{opcode} id={self.id}{label}>"
 
     def __hash__(self):
         return id(CharmInstructionLabel) ^ self.id
 
-class CharmInstructionJumpToLabel(CharmInstructionLabelBase):
+class CharmInstructionJumpToLabel(CharmInstruction): # CharmInstructionLabelBase
     """
     jump_to_label <label>
 
     Sets the 'ip' register to point to the instruction
     after the instance of the <label> instruction in the
     current program.
 
     label and *_to_label are both pseudo-instructions.
     They're removed by a pass in the peephole optimizer.
     """
-    op = opcode.jump_to_label
 
-class CharmInstructionBranchOnOToLabel(CharmInstructionLabelBase):
+    __slots__ = ['label']
+
+    def __init__(self, label):
+        self.op = opcode.jump_to_label
+        self.label = label
+
+    def __repr__(self):
+        label = f" label={self.label!r}" if self.label else ""
+        return f"<jump-to-label {label}>"
+
+
+class CharmInstructionBranchOnOToLabel(CharmInstruction):
     """
     branch_on_o_to_label <label>
 
     If the 'o' register is a true value,
     sets the 'ip' register to point to the instruction
     after the instance of the <label> instruction in the
     current program.
 
     label and *_to_label are both pseudo-instructions.
     They're removed by a pass in the peephole optimizer.
     """
-    op = opcode.branch_on_o_to_label
+
+    __slots__ = ['label']
+
+    def __init__(self, label):
+        self.op = opcode.branch_on_o_to_label
+        self.label = label
+
+    def __repr__(self):
+        label = f" label={self.label!r}" if self.label else ""
+        return f"<branch-on-o-to-label {label}>"
+
 
 class CharmInstructionCreateConverter(CharmInstruction):
     """
     create_converter <parameter> <key>
 
     Creates a Converter object using <parameter>,
     an inspect.Parameter object.
 
     Stores the resulting converter object
     in 'converters[key]' and in the 'o' register.
     """
-    op = opcode.create_converter
-    # __slots__ = ['parameter', 'key']
+    __slots__ = ['parameter', 'key']
 
     def __init__(self, parameter, key):
+        self.op = opcode.create_converter
         self.parameter = parameter
         self.key = key
 
     def __repr__(self):
         return f"<create_converter parameter={parameter!r} key={self.key}>"
 
-class CharmInstructionLoadConverter(CharmInstructionKeyBase):
+class CharmInstructionLoadConverter(CharmInstruction): # CharmInstructionKeyBase
     """
     load_converter <key>
 
     Loads a Converter object from 'converters[key]' and
     stores a reference in the 'converter' register.
     """
-    op = opcode.load_converter
 
-class CharmInstructionLoadO(CharmInstructionKeyBase):
-    """
-    load_o <key>
+    __slots__ = ['key']
 
-    Loads a Converter object from 'converters[key]' and
-    stores a reference in the 'o' register.
-    """
-    op = opcode.load_o
+    def __init__(self, key):
+        self.op = opcode.load_converter
+        self.key = key
+
+    def __repr__(self):
+        return f"<load_converter key={self.key}>"
 
-class CharmInstructionLoadOOption(CharmInstruction):
+
+class CharmInstructionLoadO(CharmInstruction): # CharmInstructionKeyBase
     """
     load_o <key>
 
     Loads a Converter object from 'converters[key]' and
     stores a reference in the 'o' register.
     """
-    op = opcode.load_o_option
+    __slots__ = ['key']
 
-    def __init__(self, option):
-        self.option = option
+    def __init__(self, key):
+        self.op = opcode.load_o
+        self.key = key
 
     def __repr__(self):
-        return f"<load_o_option option={self.option}>"
+        return f"<load_converter key={self.key}>"
 
 class CharmInstructionAppendArgs(CharmInstruction):
     """
     append_args <parameter> <usage>
 
     Takes a reference to the value in the 'o' register
     and appends it to 'converter.args'.
 
     <callable> is a callable object.
     <parameter> and <usage> are strings identifying
     the name of the parameter.  These are all used in
     generating usage information and documentation.
     """
-    op = opcode.append_args
+
+    __slots__ = ['callable', 'parameter', 'usage', 'usage_callable', 'usage_parameter']
 
     def __init__(self, callable, parameter, usage, usage_callable, usage_parameter):
+        self.op = opcode.append_args
         self.callable = callable
         self.parameter = parameter
         self.usage = usage
         self.usage_callable = usage_callable
         self.usage_parameter = usage_parameter
 
     def __repr__(self):
@@ -896,62 +725,71 @@
 
     Takes a reference to the object currently in
     the 'o' register and stores it in 'converter.kwargs[<name>]'.
     (Here 'converter' is the 'converter' register.)
 
     <name> is a string.
     """
-    op = opcode.store_kwargs
-    # __slots__ = ['name']
+
+    __slots__ = ['name']
 
     def __init__(self, name):
+        self.op = opcode.store_kwargs
         self.name = name
 
     def __repr__(self):
         return f"<store_kwargs name={self.name}>"
 
-class CharmInstructionPushContext(CharmInstructionNoArgBase):
+class CharmInstructionPushContext(CharmInstruction): # CharmInstructionNoArgBase
     """
     push_context
 
-    Pushes the current 'converter', 'total', 'option', and 'group'
-    registers on the stack.
+    Pushes the current 'converter', 'group', 'o', 'option',
+    and 'total' registers on the stack.
     """
-    op = opcode.push_context
+    def __init__(self):
+        self.op = opcode.push_context
+
+    def __repr__(self):
+        return f"<push_context>"
 
-class CharmInstructionPopContext(CharmInstructionNoArgBase):
+class CharmInstructionPopContext(CharmInstruction): # CharmInstructionNoArgBase
     """
     pop_context
 
     Pops the top value from the stack, restoring
-    the previous values of the 'converter', 'total',
-    and 'group' registers.
+    the previous values of the 'converter', 'group',
+    'o', 'option', and 'total' registers.
     """
-    op = opcode.pop_context
+    def __init__(self):
+        self.op = opcode.pop_context
+
+    def __repr__(self):
+        return f"<pop_context>"
 
 class CharmInstructionMapOption(CharmInstruction):
     """
-    map_option <option> <program>
+    map_option <option> <program> <callable> <parameter> <key>
 
     Maps the option <option> to the program <program>.
 
     <program> is self-contained; if the option is invoked
     on the command-line, you may simply 'push' the new
     program on your current CharmInterpreter.
 
     <key> and <parameter> are used in generating
     usage information.  <key> is the converter key
     for the converter, and <parameter> is the
     parameter on that converter, that this option
     maps to.
     """
-    op = opcode.map_option
-    # __slots__ = ['option', 'program']
+    __slots__ = ['option', 'program', 'callable', 'parameter', 'key']
 
     def __init__(self, option, program, callable, parameter, key):
+        self.op = opcode.map_option
         self.option = option
         self.program = program
         self.callable = callable
         self.parameter = parameter
         self.key = key
 
     def __repr__(self):
@@ -974,49 +812,54 @@
           command-line positional argument.  You should process
           command-line arguments normally, including
           processing options.  Continue processing until
           you find a command-line argument that isn't
           an option, nor is consumed by any options that
           you might have encountered while processing,
           and then consume that argument to satisfy this
-          instruction.  (Also, is_oparg being False has some
-          effect on the "option stack".)
+          instruction.
     """
-    op = opcode.consume_argument
-    # __slots__ = ['is_oparg']
+    __slots__ = ['is_oparg']
 
     def __init__(self, is_oparg):
+        self.op = opcode.consume_argument
         self.is_oparg = is_oparg
 
     def __repr__(self):
         return f"<consume_argument is_oparg={self.is_oparg}>"
 
-class CharmInstructionFlushMultioption(CharmInstructionNoArgBase):
+class CharmInstructionFlushMultioption(CharmInstruction): # CharmInstructionNoArgBase
     """
     flush_multioption
 
     Calls the flush() method on the object stored in
     the 'o' register.
     """
-    op = opcode.flush_multioption
+
+    def __init__(self):
+        self.op = opcode.flush_multioption
+
+    def __repr__(self):
+        return f"<flush_multioption>"
 
 
 class CharmInstructionSetGroup(CharmInstruction):
     """
-    set_group <minimum> <maximum>
+    set_group <minimum> <maximum> <optional> <repeating>
 
     Indicates that the program has entered a new argument
     group, and specifies the minimum and maximum arguments
     accepted by that group.  These numbers are stored as
     an ArgumentCount object in the 'group' register.
     """
-    op = opcode.set_group
-    # __slots__ = ['group', 'optional', 'repeating']
+
+    __slots__ = ['group', 'optional', 'repeating']
 
     def __init__(self, minimum, maximum, optional, repeating):
+        self.op = opcode.set_group
         self.group = ArgumentCounter(minimum, maximum, optional)
         self.optional = optional
         self.repeating = repeating
 
     def __repr__(self):
         return f"<set_group group={self.group.summary()} optional={self.optional} repeating={self.repeating}>"
 
@@ -1024,22 +867,24 @@
     """
     end
 
     Marks the end of a program.  A no-op, exists only
     to provide some context when reading the trace from
     a running interpreter.
     """
-    op = opcode.end
+
+    __slots__ = ['id', 'name']
 
     def __init__(self, id, name):
+        self.op = opcode.end
         self.id = id
         self.name = name
 
     def __repr__(self):
-        return f"<{str(self.op).partition('.')[2]} id={self.id} name={self.name!r}>"
+        return f"<end id={self.id} name={self.name!r}>"
 
 
 class CharmAssembler:
     def __init__(self, compiler):
         self.compiler = compiler
         self.opcodes = []
 
@@ -1087,20 +932,14 @@
 
     def load_o(self, key):
         op = CharmInstructionLoadO(
             key=key,
             )
         return self.append(op)
 
-    def load_o_option(self, key):
-        op = CharmInstructionLoadOOption(
-            option=option,
-            )
-        return self.append(op)
-
     def append_args(self, callable, parameter, usage, usage_callable, usage_parameter):
         op = CharmInstructionAppendArgs(
             callable = callable,
             parameter = parameter,
             usage = usage,
             usage_callable = usage_callable,
             usage_parameter = usage_parameter,
@@ -1238,21 +1077,14 @@
             self.assemblers.append(self.waiting_argument_group_options)
             self.waiting_argument_group_options = None
 
     def after_consume_argument(self):
         self.flush_argument_group_options()
         self.new_consume_argument_assemblers()
 
-    # def ensure_callables_have_unique_names(self, callable):
-    #     assert hasattr(callable, '__name__'), "{callable} has no __name__ attribute, how do we track it?"
-    #     name = callable.__name__
-    #     existing = self.name_to_callable.get(name)
-    #     if existing and (existing != callable):
-    #         raise AppealConfigurationError("multiple annotation functions with the same name {name!r}: {callable} and {existing}")
-
     def compile_options(self, parent_callable, key, parameter, options, depth):
         if want_prints:
             indent = "  " * depth
             print(f"[cc] {indent}compile_options options={options} key={key} parameter={parameter} parameter.kind={parameter.kind}")
 
         cls = self.appeal.root.map_to_converter(parameter)
 
@@ -1545,15 +1377,15 @@
                 continue
             break
 
         # in Python 3.11, inspect.Parameter won't allow you to use
         # 'lambda' (or '<lambda>') as a parameter name.  And we aren't
         # doing that, not really.  It's not a *real* Parameter, we
         # just use one of those because of the way _compile recurses.
-        # But if we're compiling a lambda  function, we create a
+        # But if we're compiling a lambda function, we create a
         # Parameter out of the function's name, which is '<lambda>',
         # and, well... we gotta use *something*.  (hope this works!)
         fix_lambda = parameter_name == 'lambda'
         if fix_lambda:
             parameter_name = '_____lambda______'
 
         def signature(p):
@@ -1585,16 +1417,16 @@
     def finalize(self):
         """
         Performs a finalization pass on program:
 
         * Computes total and group min/max values.
         * Convert label/jump_to_label pseudo-ops into
           absolute jump ops.
-        * Simple peephole optimizer to remove redundant
-          load_* ops.
+        * Simple peephole optimizations to remove redundant
+          load_* ops and jump-to-jumps.
         """
 
         program = self.program.opcodes
         for a in self.assemblers:
             opcodes = a.opcodes
             if not opcodes:
                 continue
@@ -1672,35 +1504,48 @@
                     continue
                 o = op.key
             if op.op == opcode.create_converter:
                 o = op.key
             if op.op == opcode.consume_argument:
                 o = '(string value)'
             if op.op == opcode.push_context:
-                stack.append((converter, o, option, total, group))
+                stack.append(CharmContextStackEntry(converter, group, o, total))
             if op.op == opcode.pop_context:
-                converter, o, option, total, group = stack.pop()
+                context = stack.pop()
+                converter = context.converter
+                group = context.group
+                o = context.o
+                total = context.total
 
             i += 1
 
         # now process jump fixups:
         # replace *_to_label ops with absolute jump ops
         opcode_map = {
             opcode.jump_to_label: CharmInstructionJump,
             opcode.branch_on_o_to_label: CharmInstructionBranchOnO,
         }
         for i in jump_fixups:
             op = p[i]
-            new_instruction_cls = opcode_map.get(op.op)
-            assert new_instruction_cls
+            new_instruction_cls = opcode_map[op.op]
             address = labels.get(op.label)
             if address is None:
                 raise AppealConfigurationError(f"unknown label {op.label}")
             p[i] = new_instruction_cls(address)
 
+        # and *now* do a jump-to-jump peephole optimization
+        # (I don't know if Appeal can actually generate jump-to-jumps)
+        for i in jump_fixups:
+            op = p[i]
+            while True:
+                op2 = p[op.address]
+                if op2.op != opcode.jump:
+                    break
+                op.address = op2.address
+
         return p
 
 
 def charm_compile(appeal, callable, default=empty, name=None, *, is_option=False):
     if name is None:
         name = callable.__name__
     cc = CharmCompiler(appeal, name=name)
@@ -1749,14 +1594,16 @@
                     value = repr(value)
                 print(f"{indent2}{slot}={value}")
     print()
 
 
 
 class CharmProgramIterator:
+    __slots__ = ['program', 'opcodes', 'length', 'ip']
+
     def __init__(self, program):
         self.program = program
         self.opcodes = program.opcodes
         self.length = len(program)
         self.ip = 0
 
     def __next__(self):
@@ -1776,47 +1623,49 @@
 
     def jump_relative(self, delta):
         self.ip += delta
 
 
 
 class CharmStackEntry:
+    __slots__ = ['i', 'program', 'context_count']
+
     def __init__(self, i, program, context_count=0):
         self.i = i
         self.program = program
         self.context_count = context_count
 
     def __repr__(self):
         return f"<CharmStackEntry i={self.i} program={self.program.name!r} context_count={self.context_count}>"
 
 
 class CharmContextStackEntry:
-    def __init__(self, converter, group, o, option, total):
+    __slots__ = ['converter', 'group', 'o', 'total']
+
+    def __init__(self, converter, group, o, total):
         self.converter = converter
         self.group = group
         self.o = o
-        self.option = option
         self.total = total
 
     def __repr__(self):
-        return f"<CharmContextStackEntry converter={self.converter} group={self.group} o={self.o} option={self.option} total={self.total}>"
+        return f"<CharmContextStackEntry converter={self.converter} group={self.group} o={self.o} total={self.total}>"
 
 
 class CharmInterpreter:
     def __init__(self, program, *, name=''):
         self.name = name
         self.stack = []
         self.context_stack = []
 
         assert program
 
         # registers
         self.converter = None
         self.o = None
-        self.option = None
         self.total = None
         self.group = None
         self.converters = {}
         self.program = program
 
         self.op = None
 
@@ -1872,25 +1721,24 @@
 
     def call(self, program):
         self.stack.append(CharmStackEntry(self.i, self.program))
         self.program = program
         self.i = CharmProgramIterator(program)
 
     def push_context(self):
-        context = CharmContextStackEntry(self.converter, self.group, self.o, self.option, self.total)
+        context = CharmContextStackEntry(self.converter, self.group, self.o, self.total)
         self.context_stack.append(context)
         if self.stack:
             self.stack[-1].context_count += 1
 
     def _pop_context(self):
         context = self.context_stack.pop()
         self.converter = context.converter
         self.group = context.group
         self.o = context.o
-        self.option = context.option
         self.total = context.total
 
     def pop_context(self):
         self._pop_context()
         if self.stack:
             self.stack[-1].context_count -= 1
 
@@ -2214,20 +2062,14 @@
             if op.op == opcode.load_o:
                 ci.o = ci.converters.get(op.key, None)
                 if want_prints:
                     o = ci.repr_converter(ci.o)
                     print(f"## {ip_spacer} load_o op.key={op.key} o={o!s}")
                 continue
 
-            if op.op == opcode.load_o_option:
-                ci.option = op.option
-                if want_prints:
-                    print(f"## {ip_spacer} load_o_option op.option={op.option} o={o!s}")
-                continue
-
             if op.op == opcode.map_option:
                 options_bucket[op.option] = op.program
                 if want_prints:
                     print(f"## {ip_spacer} map_option op.option={op.option} op.program={op.program} token {options_token}")
                 continue
 
             if op.op == opcode.append_args:
@@ -2239,16 +2081,15 @@
                 continue
 
             if op.op == opcode.store_kwargs:
                 converter = ci.o
                 if op.name in ci.converter.kwargs_converters:
                     existing = ci.converter.kwargs_converters[op.name]
                     if not ((existing == converter) and isinstance(existing, MultiOption)):
-                        # TODO: this is terrible UI, must fix.
-                        raise AppealUsageError(f"{ci.option} specified more than once.")
+                        raise AppealUsageError(f"{program.name} specified more than once.")
                     # we're setting the kwarg to the value it's already set to,
                     # and it's a multioption, so this is fine.
                     continue
                 ci.converter.kwargs_converters[op.name] = ci.o
                 if want_prints:
                     o = ci.repr_converter(ci.o)
                     print(f"## {ip_spacer} store_kwargs name={op.name} o={o}")
@@ -2294,20 +2135,14 @@
 
             if op.op == opcode.jump:
                 if want_prints:
                     print(f"## {ip_spacer} jump op.address={op.address}")
                 ci.i.jump(op.address)
                 continue
 
-            if op.op == opcode.jump_relative:
-                if want_prints:
-                    print(f"## {ip_spacer} jump_relative op.delta={op.delta}")
-                ci.i.jump_relative(op.delta)
-                continue
-
             if op.op == opcode.branch_on_o:
                 if want_prints:
                     print(f"## {ip_spacer} branch_on_o o={ci.o} op.address={op.address}")
                 if ci.o:
                     ci.i.jump(op.address)
                 continue
 
@@ -2418,14 +2253,19 @@
             #  -o=X
             #  -oX
             # it's set to X if the user specifies an X, otherwise it's None.
             split_value = None
 
             if a.startswith("--"):
                 if a == "--":
+                    # we shouldn't be able to reach this twice.
+                    # if the user specifies -- twice on the command-line,
+                    # the first time turns of option processing, which means
+                    # it should be impossible to get here.
+                    assert not appeal.root.force_positional
                     appeal.root.force_positional = True
                     if want_prints:
                         print(f"#[]  '--', force_positional=True")
                     continue
 
                 option, equals, _split_value = a.partition("=")
                 if equals:
@@ -2502,15 +2342,14 @@
                             raise AppealUsageError(f"{error_option} doesn't take an argument")
                         if maximum_arguments >= 2:
                             raise AppealUsageError(f"{error_option} given a single argument but it requires multiple arguments, you must separate the arguments with spaces")
                     argi.push(split_value)
                     if want_prints:
                         print(f"#[]  pushing split value {split_value!r} on argi")
 
-                ci.option = error_option
                 ci.call(program)
             break
 
     undo_converters()
     satisfied = True
     if ci.total and not ci.total.satisfied():
         satisfied = False
@@ -4781,19 +4620,14 @@
         if appeal.appeal_preparer:
             # print(f"bind appeal.appeal_preparer to self.appeal={self.appeal}")
             self.preparer(appeal.appeal_preparer.bind(self.appeal))
         if appeal.processor_preparer:
             # print(f"bind appeal.processor_preparer to self={self}")
             self.preparer(appeal.processor_preparer.bind(self))
 
-        # print()
-        # for p in self.preparers:
-        #     print("[[]] preparer", p)
-        # print()
-
         appeal.analyze(self)
         appeal.parse(self)
         appeal.convert(self)
         result = self.result = appeal.execute(self)
         self.log_event("process complete")
         if want_prints:
             self.print_log()
```

### Comparing `appeal-0.5.8/appeal/argument_grouping.py` & `appeal-0.5.9/appeal/argument_grouping.py`

 * *Files 3% similar despite different names*

```diff
@@ -216,50 +216,61 @@
                 # fn is the actual Python callable this is a parameter of
                 # i is the (0-based!) index of the parameter in the function's parameter list
                 #
                 # e.g. for
                 #   def foo(a, b, c, d)
                 # if we were returning 'c', we'd return the tuple
                 #     (breadcrumb, Parameter("c", inspect.Parameter(...)), foo, 2)
-                yield (breadcrumb, p, fn, i)
+                if breadcrumb:
+                    child_breadcrumb = f"{breadcrumb}, "
+                else:
+                    child_breadcrumb = ""
+                if p.var_positional:
+                    star = "*"
+                else:
+                    star = ""
+                child_breadcrumb = child_breadcrumb + f"argument {star}{name}"
+
+                yield (child_breadcrumb, p, fn, i)
+
                 # if p.converter and (not p.var_positional):
                 if p.converter:
-                    child_breadcrumb = f"{breadcrumb}.{name}" if breadcrumb else name
+                    name = getattr(p.converter.fn, '__name__', str(p.converter.fn))
+                    child_breadcrumb = child_breadcrumb + f", converter {name}()"
                     yield from argument_generator(p.converter, child_breadcrumb)
 
         groups = []
         group = []
         def finish():
             nonlocal group
             if group:
                 # print(f"  pinching off group={group}")
                 groups.append(group)
                 # print(f"  groups is now groups={groups}")
                 group = []
 
         last_tuple = None
-        found_var_positional = None
+        var_positional_breadcrumb = None
         under_var_positional = {}
 
-        for b_p_fn_i in argument_generator(self, self.fn.__name__):
+        for b_p_fn_i in argument_generator(self, f'{self.fn.__name__}()'):
             breadcrumb, p, fn, i = b_p_fn_i
-            if found_var_positional:
-                current_breadcrumb = f"{breadcrumb}.{p}"
-                if p.required and (not current_breadcrumb.startswith(found_var_positional)):
-                    raise ValueError(f'Required parameter "{breadcrumb}.{p}" found after VAR_POSITIONAL parameter "{found_var_positional}"')
+            if var_positional_breadcrumb:
+                if p.required and (not breadcrumb.startswith(var_positional_breadcrumb)):
+                    raise ValueError(f'This command-line can never be satisfied.  "{breadcrumb}" is a required parameter, but it can never get an argument, because it comes after VAR_POSITIONAL parameter "{var_positional_breadcrumb}" which already consumed all remaining command-line arguments.')
             # t = (p.optionality, p.required)
             t = p.optionality
             if (last_tuple != t) or (not p.required):
                 # print(f"finishing because {p}, group={group}")
                 finish()
                 last_tuple = t
             group.append((p, fn, i))
             # once we hit the first var_positional parameter, we are donezo!
             if p.var_positional:
-                found_var_positional = f"{breadcrumb}.{p.name}."
+                var_positional_breadcrumb = breadcrumb
 
         finish()
         required = None
         if groups:
             assert groups[0]
             first_option = groups[0][0][0]
             if first_option.required and first_option.optionality == 0:
```

### Comparing `appeal-0.5.8/appeal/cpp.py` & `appeal-0.5.9/appeal/cpp.py`

 * *Files identical despite different names*

### Comparing `appeal-0.5.8/appeal/text.py` & `appeal-0.5.9/appeal/text.py`

 * *Files identical despite different names*

### Comparing `appeal-0.5.8/pyproject.toml` & `appeal-0.5.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `appeal-0.5.8/resources/images/appeal.logo.png` & `appeal-0.5.9/resources/images/appeal.logo.png`

 * *Files identical despite different names*

### Comparing `appeal-0.5.8/resources/images/give.your.program.appeal.png` & `appeal-0.5.9/resources/images/give.your.program.appeal.png`

 * *Files identical despite different names*

### Comparing `appeal-0.5.8/tests/run_tests.py` & `appeal-0.5.9/tests/run_tests.py`

 * *Files identical despite different names*

### Comparing `appeal-0.5.8/PKG-INFO` & `appeal-0.5.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: appeal
-Version: 0.5.8
+Version: 0.5.9
 Summary: A powerful & Pythonic command-line parsing library.  Give your program Appeal!
 Author-email: Larry Hastings <larry@hastings.org>
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Dist: big >= 0.7.1
 Project-URL: Source, https://github.com/larryhastings/appeal/
 
-![## Appeal](/resources/images/appeal.logo.png)
+![## Appeal](https://raw.githubusercontent.com/larryhastings/appeal/master/resources/images/appeal.logo.png)
 
-![## Give your program Appeal!](/resources/images/give.your.program.appeal.png)
+![## Give your program Appeal!](https://raw.githubusercontent.com/larryhastings/appeal/master/resources/images/give.your.program.appeal.png)
 
 ##### Copyright 2021-2023 by Larry Hastings
 
 
 ## Quickstart
 
 ```Python
@@ -1978,14 +1978,39 @@
   for any keyword-only parameter to a converter or command function.
 * The converter for a *var_positional* (`*args`) parameter
   *must* require at least one positional argument.
 
 
 ## Changelog
 
+**0.5.9**
+
+* Improved the error message generated when you have a
+  required parameter after a `VAR_POSITIONAL` parameter.
+  (This command-line can never succeed, because the
+  `VAR_POSITIONAL` consumes all remaining arguments on
+  the command-line, which means the subsequent required
+  parameter can never be satisfied.)  Fixes #6.
+* Changed README to use absolute instead of relative links
+  for images, which means images should now render properly
+  on the Appeal page at PyPI.  Thanks for the PR, Hugo!
+* Switched a bunch of internal classes to use Python "slots".
+  Hopefully a tiny memory and speed optimization.
+* Remove unused / unneeded stuff:
+    * unused `partial_replace*` functions
+    * unused Charm bytecode instructions `jump_relative` and `load_o_option`
+    * unneeded CharmInterpreter register `option` (only used in one error
+      message, obviated by instead using the program name directly)
+* Now that Appeal depends on [**big**](https://github.com/larryhastings/big)
+  anyway, switch to
+  [**big**'s `PushbackIterator`.](https://github.com/larryhastings/big#pushbackiteratoriterablenone).
+* Add peephole optimizer step for jump-to-jump optimization.
+  Honestly this was probably unnecessary, as I don't think Appeal's
+  compiler can even *generate* code with jumps-to-jumps (yet).
+
 **0.5.8**
 
 * Fixed up the "name" of the program for options.  We used to take
   the name of the command, add all the option strings, and join it
   together with commas, as in `'command, -o, --option'`.  Now it
   looks like `'command -o | --option'`.
 * Fixed presentation bug: if you didn't have enough positional
```

