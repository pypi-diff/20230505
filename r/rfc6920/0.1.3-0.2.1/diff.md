# Comparing `tmp/rfc6920-0.1.3.tar.gz` & `tmp/rfc6920-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rfc6920-0.1.3.tar", last modified: Tue Nov 22 03:21:45 2022, max compression
+gzip compressed data, was "rfc6920-0.2.1.tar", last modified: Thu May  4 15:22:02 2023, max compression
```

## Comparing `rfc6920-0.1.3.tar` & `rfc6920-0.2.1.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 jmfernandez (10012) users      (100)        0 2022-11-22 03:21:45.233067 rfc6920-0.1.3/
--rw-r--r--   0 jmfernandez (10012) users      (100)    26530 2021-05-10 11:31:13.000000 rfc6920-0.1.3/LICENSE.txt
--rw-r--r--   0 jmfernandez (10012) users      (100)       63 2021-10-05 12:40:46.000000 rfc6920-0.1.3/MANIFEST.in
--rw-r--r--   0 jmfernandez (10012) users      (100)     1875 2022-11-22 03:21:45.232067 rfc6920-0.1.3/PKG-INFO
--rw-r--r--   0 jmfernandez (10012) users      (100)     1207 2022-11-22 03:13:20.000000 rfc6920-0.1.3/README.md
--rw-r--r--   0 jmfernandez (10012) users      (100)       98 2021-09-29 09:44:18.000000 rfc6920-0.1.3/pyproject.toml
--rw-r--r--   0 jmfernandez (10012) users      (100)       17 2021-10-05 12:40:25.000000 rfc6920-0.1.3/requirements.txt
-drwxr-xr-x   0 jmfernandez (10012) users      (100)        0 2022-11-22 03:21:45.231067 rfc6920-0.1.3/rfc6920/
--rw-r--r--   0 jmfernandez (10012) users      (100)     1146 2022-11-22 03:09:33.000000 rfc6920-0.1.3/rfc6920/__init__.py
--rw-r--r--   0 jmfernandez (10012) users      (100)     7152 2022-11-22 03:17:34.000000 rfc6920-0.1.3/rfc6920/methods.py
-drwxr-xr-x   0 jmfernandez (10012) users      (100)        0 2022-11-22 03:21:45.232067 rfc6920-0.1.3/rfc6920.egg-info/
--rw-r--r--   0 jmfernandez (10012) users      (100)     1875 2022-11-22 03:21:45.000000 rfc6920-0.1.3/rfc6920.egg-info/PKG-INFO
--rw-r--r--   0 jmfernandez (10012) users      (100)      267 2022-11-22 03:21:45.000000 rfc6920-0.1.3/rfc6920.egg-info/SOURCES.txt
--rw-r--r--   0 jmfernandez (10012) users      (100)        1 2022-11-22 03:21:45.000000 rfc6920-0.1.3/rfc6920.egg-info/dependency_links.txt
--rw-r--r--   0 jmfernandez (10012) users      (100)       15 2022-11-22 03:21:45.000000 rfc6920-0.1.3/rfc6920.egg-info/requires.txt
--rw-r--r--   0 jmfernandez (10012) users      (100)        8 2022-11-22 03:21:45.000000 rfc6920-0.1.3/rfc6920.egg-info/top_level.txt
--rw-r--r--   0 jmfernandez (10012) users      (100)       38 2022-11-22 03:21:45.233067 rfc6920-0.1.3/setup.cfg
--rw-r--r--   0 jmfernandez (10012) users      (100)     2635 2022-11-22 03:09:53.000000 rfc6920-0.1.3/setup.py
+drwxr-xr-x   0 jmfernandez (10012) users      (100)        0 2023-05-04 15:22:02.132994 rfc6920-0.2.1/
+-rw-r--r--   0 jmfernandez (10012) users      (100)    26530 2021-05-10 11:31:13.000000 rfc6920-0.2.1/LICENSE.txt
+-rw-r--r--   0 jmfernandez (10012) users      (100)       63 2021-10-05 12:40:46.000000 rfc6920-0.2.1/MANIFEST.in
+-rw-r--r--   0 jmfernandez (10012) users      (100)     1875 2023-05-04 15:22:02.132994 rfc6920-0.2.1/PKG-INFO
+-rw-r--r--   0 jmfernandez (10012) users      (100)     1207 2022-11-22 03:13:20.000000 rfc6920-0.2.1/README.md
+-rw-r--r--   0 jmfernandez (10012) users      (100)       98 2021-09-29 09:44:18.000000 rfc6920-0.2.1/pyproject.toml
+-rw-r--r--   0 jmfernandez (10012) users      (100)       17 2023-05-03 17:23:06.000000 rfc6920-0.2.1/requirements.txt
+drwxr-xr-x   0 jmfernandez (10012) users      (100)        0 2023-05-04 15:22:02.132994 rfc6920-0.2.1/rfc6920/
+-rw-r--r--   0 jmfernandez (10012) users      (100)     1151 2023-05-04 09:46:45.000000 rfc6920-0.2.1/rfc6920/__init__.py
+-rw-r--r--   0 jmfernandez (10012) users      (100)     7920 2023-05-04 09:36:52.000000 rfc6920-0.2.1/rfc6920/methods.py
+-rw-r--r--   0 jmfernandez (10012) users      (100)        0 2023-05-04 09:49:26.000000 rfc6920-0.2.1/rfc6920/py.typed
+drwxr-xr-x   0 jmfernandez (10012) users      (100)        0 2023-05-04 15:22:02.132994 rfc6920-0.2.1/rfc6920.egg-info/
+-rw-r--r--   0 jmfernandez (10012) users      (100)     1875 2023-05-04 15:22:02.000000 rfc6920-0.2.1/rfc6920.egg-info/PKG-INFO
+-rw-r--r--   0 jmfernandez (10012) users      (100)      284 2023-05-04 15:22:02.000000 rfc6920-0.2.1/rfc6920.egg-info/SOURCES.txt
+-rw-r--r--   0 jmfernandez (10012) users      (100)        1 2023-05-04 15:22:02.000000 rfc6920-0.2.1/rfc6920.egg-info/dependency_links.txt
+-rw-r--r--   0 jmfernandez (10012) users      (100)       15 2023-05-04 15:22:02.000000 rfc6920-0.2.1/rfc6920.egg-info/requires.txt
+-rw-r--r--   0 jmfernandez (10012) users      (100)        8 2023-05-04 15:22:02.000000 rfc6920-0.2.1/rfc6920.egg-info/top_level.txt
+-rw-r--r--   0 jmfernandez (10012) users      (100)       38 2023-05-04 15:22:02.132994 rfc6920-0.2.1/setup.cfg
+-rw-r--r--   0 jmfernandez (10012) users      (100)     2572 2023-05-04 09:49:19.000000 rfc6920-0.2.1/setup.py
```

### Comparing `rfc6920-0.1.3/LICENSE.txt` & `rfc6920-0.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rfc6920-0.1.3/PKG-INFO` & `rfc6920-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rfc6920
-Version: 0.1.3
+Version: 0.2.1
 Summary: A library to generate and validate RFC6920 URIs
 Home-page: https://github.com/inab/pyrfc6920
 Author: José M. Fernández <https://orcid.org/0000-0002-4806-5140>
 Author-email: jose.m.fernandez@bsc.es
 License: LGPL-2.1
 Project-URL: Bug Tracker, https://github.com/inab/pyrfc6920/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `rfc6920-0.1.3/README.md` & `rfc6920-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `rfc6920-0.1.3/rfc6920/__init__.py` & `rfc6920-0.2.1/rfc6920/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 # rfc6920, a library to generate and validate RFC6920 URIs
-# Copyright (C) 2022 Barcelona Supercomputinh Center, José M. Fernández
+# Copyright (C) 2022-2023 Barcelona Supercomputing Center, José M. Fernández
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License, or (at your option) any later version.
 #
 # This library is distributed in the hope that it will be useful,
@@ -14,13 +14,13 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU
 # Lesser General Public License for more details.
 #
 # You should have received a copy of the GNU Lesser General Public
 # License along with this library; if not, write to the Free Software
 # Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301  USA
 
-__author__ = 'José M. Fernández <https://orcid.org/0000-0002-4806-5140>'
-__copyright__ = '© 2022 Barcelona Supercomputing Center (BSC), ES'
-__license__ = 'LGPL-2.1'
+__author__ = "José M. Fernández <https://orcid.org/0000-0002-4806-5140>"
+__copyright__ = "© 2022 Barcelona Supercomputing Center (BSC), ES"
+__license__ = "LGPL-2.1"
 
 # https://www.python.org/dev/peps/pep-0396/
-__version__ = '0.1.3'
+__version__ = "0.2.1"
```

### Comparing `rfc6920-0.1.3/rfc6920/methods.py` & `rfc6920-0.2.1/rfc6920/methods.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 # rfc6920, a library to generate and validate RFC6920 URIs
-# Copyright (C) 2022 Barcelona Supercomputinh Center, José M. Fernández
+# Copyright (C) 2022-2023 Barcelona Supercomputing Center, José M. Fernández
 #
 # This library is free software; you can redistribute it and/or
 # modify it under the terms of the GNU Lesser General Public
 # License as published by the Free Software Foundation; either
 # version 2.1 of the License, or (at your option) any later version.
 #
 # This library is distributed in the hope that it will be useful,
@@ -18,220 +18,290 @@
 # License along with this library; if not, write to the Free Software
 # Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA  02110-1301  USA
 
 import genluhn
 
 import base64
 import hashlib
-import _hashlib
 import urllib.parse
 
-from typing import Union
-
-INDEXED_HASH_NAMES: "Sequence[None, Mapping[str, Union[str, int, None]]]" = [
-	None,	# Reserved
-	{
-		'name': 'sha-256',
-		'algo': 'sha256',
-		'trunc': None
-	},
-	{
-		'name': 'sha-256-128',
-		'algo': 'sha256',
-		'trunc': 128
-	},
-	{
-		'name': 'sha-256-120',
-		'algo': 'sha256',
-		'trunc': 120
-	},
-	{
-		'name': 'sha-256-96',
-		'algo': 'sha256',
-		'trunc': 96
-	},
-	{
-		'name': 'sha-256-64',
-		'algo': 'sha256',
-		'trunc': 64
-	},
-	{
-		'name': 'sha-256-32',
-		'algo': 'sha256',
-		'trunc': 32
-	},
+from typing import (
+	cast,
+	TYPE_CHECKING,
+)
+
+if TYPE_CHECKING:
+	from typing import (
+		Callable,
+		IO,
+		Iterable,
+		Mapping,
+		Optional,
+		Sequence,
+		Tuple,
+		Union,
+	)
+
+	from typing_extensions import (
+		Literal,
+		TypedDict,
+		NotRequired,
+	)
+
+	from genluhn import Digit
+
+	class IndexedHashName(TypedDict):
+		name: "str"
+		algo: "str"
+		trunc: "Optional[int]"
+		instance: "NotRequired[hashlib._Hash]"
+
+
+INDEXED_HASH_NAMES: "Sequence[Optional[IndexedHashName]]" = [
+	None,  # Reserved
+	{"name": "sha-256", "algo": "sha256", "trunc": None},
+	{"name": "sha-256-128", "algo": "sha256", "trunc": 128},
+	{"name": "sha-256-120", "algo": "sha256", "trunc": 120},
+	{"name": "sha-256-96", "algo": "sha256", "trunc": 96},
+	{"name": "sha-256-64", "algo": "sha256", "trunc": 64},
+	{"name": "sha-256-32", "algo": "sha256", "trunc": 32},
 ]
 
-NI_SCHEME = 'ni'
-NIH_SCHEME = 'nih'
-
-HASH_NAMES = { desc['name']: desc  for desc in filter(lambda desc: desc is not None, INDEXED_HASH_NAMES) }
+NI_SCHEME = "ni"
+NIH_SCHEME = "nih"
 
-STATIC_DEFAULT_BUFFER_SIZE=65536
-def compute_digest_from_filelike_and_callback(filelike: "IO[bytes]", h: "_hashlib.HASH", bufferSize: "int" = STATIC_DEFAULT_BUFFER_SIZE, cback=None) -> "bytes":
+HASH_NAMES = {
+	desc["name"]: desc
+	for desc in cast(
+		"Iterable[IndexedHashName]",
+		filter(lambda desc: desc is not None, INDEXED_HASH_NAMES),
+	)
+}
+
+STATIC_DEFAULT_BUFFER_SIZE = 65536
+
+
+def compute_digest_from_filelike_and_callback(
+	filelike: "IO[bytes]",
+	h: "hashlib._Hash",
+	bufferSize: "int" = STATIC_DEFAULT_BUFFER_SIZE,
+	cback: "Optional[Callable[[bytes], None]]" = None,
+) -> "bytes":
 	"""
 	Accessory method used to compute the digest of an input file-like object
 	"""
-	
+
 	buf = filelike.read(bufferSize)
 	while len(buf) > 0:
 		h.update(buf)
 		if cback:
 			cback(buf)
 		buf = filelike.read(bufferSize)
-		
+
 	return h.digest()
 
-def _generate_ni_pre(filename: "Union[str, bytes, bytearray]", algo: "Union[str, int, _hashlib.HASH]" = 'sha-256', trunc: "Optional[int]" = None) -> "Tuple[bytes, Mapping[str, Union[str, int, _hashlib.HASH]]":
+
+def _generate_ni_pre(
+	filename: "Union[str, IO[bytes], bytes, bytearray]",
+	algo: "Union[str, int, hashlib._Hash]" = "sha-256",
+	trunc: "Optional[int]" = None,
+) -> "Tuple[bytes, IndexedHashName]":
 	"""
 	The first parameter can be either the suite id (an integer)
 	or an algorithm
 	"""
+	desc: "IndexedHashName"
 	if isinstance(algo, str):
 		# First, try matching by name
-		desc = HASH_NAMES.get(algo)
-		
-		if desc is None:
+		gotdesc = HASH_NAMES.get(algo)
+
+		if gotdesc is None:
 			# Second, give a try later
 			name = algo
 			if trunc is not None:
-				name += '-' + str(trunc)
-			desc = {
-				'name': name,
-				'algo': algo,
-				'trunc': trunc
-			}
-		elif (trunc is not None) and (desc.get('trunc') is None):
+				name += "-" + str(trunc)
+			desc = {"name": name, "algo": algo, "trunc": trunc}
+		elif (trunc is not None) and (desc.get("trunc") is None):
 			# Overriding default value
-			desc = desc.copy()
-			desc['trunc'] = trunc
-			desc['name'] += '-{}'.format(trunc)
+			desc = gotdesc.copy()
+			desc["trunc"] = trunc
+			desc["name"] += "-{}".format(trunc)
 	elif isinstance(algo, int):
 		if algo < 1 or algo >= len(INDEXED_HASH_NAMES):
-			raise ValueError("Unrecognized or invalid RFC6920 suite id '{}'".format(algo))
-		
-		desc = INDEXED_HASH_NAMES[algo]
-		if (trunc is not None) and (desc.get('trunc') is None):
+			raise ValueError(
+				"Unrecognized or invalid RFC6920 suite id '{}'".format(algo)
+			)
+
+		gotdesc = INDEXED_HASH_NAMES[algo]
+		assert gotdesc is not None
+		desc = gotdesc
+		if (trunc is not None) and (desc.get("trunc") is None):
 			# Overriding default value
 			desc = desc.copy()
-			desc['trunc'] = trunc
-			desc['name'] += '-{}'.format(trunc)
-	elif isinstance(algo, _hashlib.HASH):
+			desc["trunc"] = trunc
+			desc["name"] += "-{}".format(trunc)
+	elif hasattr(algo, "digest_size"):
 		desc = {
-			'name': algo.name,
-			'algo': algo.name,
-			'trunc': algo.digest_size * 8,
-			'instance': algo
+			"name": algo.name,
+			"algo": algo.name,
+			"trunc": algo.digest_size * 8,
+			"instance": algo,
 		}
 	else:
 		raise ValueError("Unsupported algo type of {}".format(type(algo)))
-	
+
 	# Now, prepare the instance
-	instance = desc.get('instance')
+	instance = desc.get("instance")
 	if instance is None:
-		instance = hashlib.new(desc['algo'])
-	
-	# Time to open file
-	if isinstance(filename, (bytes,bytearray)):
+		instance = hashlib.new(desc["algo"])
+
+	if isinstance(filename, (bytes, bytearray)):
 		instance.update(filename)
 		digest = instance.digest()
+	elif hasattr(filename, "seek"):
+		# It is a file-like object
+		digest = compute_digest_from_filelike_and_callback(
+			cast("IO[bytes]", filename), instance
+		)
 	else:
-		with open(filename, mode='rb') as f:
+		# Time to open file
+		with open(filename, mode="rb") as f:
 			digest = compute_digest_from_filelike_and_callback(f, instance)
-	
+
 	return digest, desc
 
+
 def prettify_digest(digest: "Union[bytes, bytearray]") -> "str":
-	pretty_digest = ''
+	pretty_digest = ""
 	for ib, b in enumerate(digest):
-		pretty_digest += ('-{:02x}'  if ib > 0 and (ib & 1) == 0  else '{:02x}').format(b)
-	
+		pretty_digest += ("-{:02x}" if ib > 0 and (ib & 1) == 0 else "{:02x}").format(b)
+
 	return pretty_digest
 
-def generate_nih_from_digest(digest: "Union[bytes, bytearray]", algo: "str" = 'sha-256', trunc: "Optional[int]" = None) -> "str":
+
+def generate_nih_from_digest(
+	digest: "Union[bytes, bytearray]",
+	algo: "str" = "sha-256",
+	trunc: "Optional[int]" = None,
+) -> "str":
 	# First, let's truncate to the bytes limit
 	if trunc is not None:
 		truncbytes = trunc // 8
 		if len(digest) > truncbytes:
 			digest = digest[:truncbytes]
-	
+
 	checkdigit = genluhn.compute(digest, 16)
 	pretty_digest = prettify_digest(digest)
-	
-	return urllib.parse.urlunparse((NIH_SCHEME,'','{};{};{:x}'.format(algo,pretty_digest,checkdigit),'','',''))
 
-def generate_nih(filename: "Union[str, bytes, bytearray]", algo: "Union[str, int, _hashlib.HASH]" = 'sha-256', trunc: "Optional[int]" = None) -> "str":
+	return urllib.parse.urlunparse(
+		(
+			NIH_SCHEME,
+			"",
+			"{};{};{:x}".format(algo, pretty_digest, checkdigit),
+			"",
+			"",
+			"",
+		)
+	)
+
+
+def generate_nih(
+	filename: "Union[str, IO[bytes], bytes, bytearray]",
+	algo: "Union[str, int, hashlib._Hash]" = "sha-256",
+	trunc: "Optional[int]" = None,
+) -> "str":
 	digest, desc = _generate_ni_pre(filename, algo, trunc)
-	
-	return generate_nih_from_digest(digest, desc['name'], desc['trunc'])
 
-def generate_ni_from_digest(digest: "Union[bytes, bytearray]", algo: "str" = 'sha-256', trunc: "Optional[int]" = None, authority: "str" = '') -> "str":
+	return generate_nih_from_digest(digest, desc["name"], desc["trunc"])
+
+
+def generate_ni_from_digest(
+	digest: "Union[bytes, bytearray]",
+	algo: "str" = "sha-256",
+	trunc: "Optional[int]" = None,
+	authority: "str" = "",
+) -> "str":
 	# First, let's truncate to the bytes limit
 	if trunc is not None:
 		truncbytes = trunc // 8
 		if len(digest) > truncbytes:
 			digest = digest[:truncbytes]
-	
-	b64digest = base64.urlsafe_b64encode(digest).decode('utf-8')
-	
+
+	b64digest = base64.urlsafe_b64encode(digest).decode("utf-8")
+
 	if authority:
-		upat = '/{};{}'
+		upat = "/{};{}"
 	else:
-		upat = '///{};{}'
-	
-	return urllib.parse.urlunparse((NI_SCHEME,authority,upat.format(algo,b64digest),'','',''))
+		upat = "///{};{}"
+
+	return urllib.parse.urlunparse(
+		(NI_SCHEME, authority, upat.format(algo, b64digest), "", "", "")
+	)
+
 
-def generate_ni(filename: "Union[str, bytes, bytearray]", algo: "Union[str, int, _hashlib.HASH]" = 'sha-256', trunc: "Optional[int]" = None) -> "str":
+def generate_ni(
+	filename: "Union[str, IO[bytes], bytes, bytearray]",
+	algo: "Union[str, int, hashlib._Hash]" = "sha-256",
+	trunc: "Optional[int]" = None,
+) -> "str":
 	digest, desc = _generate_ni_pre(filename, algo, trunc)
-	
-	return generate_ni_from_digest(digest, desc['name'], desc['trunc'])
 
-def extract_digest(the_uri: "str") -> "Union[Tuple[None, None], Tuple[Union[Literal[False], bytes, bytearray], str]]":
+	return generate_ni_from_digest(digest, desc["name"], desc["trunc"])
+
+
+def extract_digest(
+	the_uri: "str",
+) -> "Union[Tuple[None, None], Tuple[Union[Literal[False], bytes, bytearray], str]]":
 	"""
 	It extracts both the digest and the hashing algorithm from
 	nih and ni URIs
 	"""
 	parsed = urllib.parse.urlparse(the_uri)
 	if parsed.scheme not in (NI_SCHEME, NIH_SCHEME):
 		return None, None
-	
-	lsemicolon = parsed.path.index(';')
+
+	lsemicolon = parsed.path.index(";")
 	algo = parsed.path[0:lsemicolon]
-	if algo[0] == '/':
+	if algo[0] == "/":
 		algo = algo[1:]
-	encoded_digest = parsed.path[lsemicolon+1:]
-	digest = None
+	encoded_digest = parsed.path[lsemicolon + 1 :]
+	digest: "Optional[bytes]" = None
 	# Obtaining the digest
 	if parsed.scheme == NIH_SCHEME:
 		checkdigit = None
-		rsemicolon = encoded_digest.rfind(';')
-		if ';' in encoded_digest:
-			checkdigit = int(encoded_digest[rsemicolon+1], 16)
+		rsemicolon = encoded_digest.rfind(";")
+		if ";" in encoded_digest:
+			checkdigit = cast("Digit", int(encoded_digest[rsemicolon + 1], 16))
 			hexdigest = encoded_digest[:rsemicolon]
-			
+
 			# Return false if the check digit validation fails
 			if not genluhn.validate(hexdigest, 16, checkdigit):
 				return False, algo
 		else:
 			hexdigest = encoded_digest
-		
-		digest = bytearray.fromhex(hexdigest.replace('-',''))
+
+		digest = bytearray.fromhex(hexdigest.replace("-", ""))
 	else:
 		digest = base64.urlsafe_b64decode(encoded_digest)
-	
+
 	return digest, algo
 
-def validate(the_uri: "str", filename: "Union[str, bytes, bytearray]") -> "bool":
+
+def validate(
+	the_uri: "str", filename: "Union[str, IO[bytes], bytes, bytearray]"
+) -> "bool":
 	digest, algo = extract_digest(the_uri)
-	
-	if not isinstance(digest, (bytes, bytearray)):
+
+	if digest is None or digest is False:
 		return False
-	
+
+	assert algo is not None
+
 	computed_digest, _ = _generate_ni_pre(filename, algo)
-	
+
 	# When the length of the computed digest is smaller, it is not
 	# going to end well....
 	if len(digest) > len(computed_digest):
 		return False
-	
+
 	# Last, compare the common part
-	return digest == computed_digest[:len(digest)]
+	return digest == computed_digest[: len(digest)]
```

### Comparing `rfc6920-0.1.3/rfc6920.egg-info/PKG-INFO` & `rfc6920-0.2.1/rfc6920.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rfc6920
-Version: 0.1.3
+Version: 0.2.1
 Summary: A library to generate and validate RFC6920 URIs
 Home-page: https://github.com/inab/pyrfc6920
 Author: José M. Fernández <https://orcid.org/0000-0002-4806-5140>
 Author-email: jose.m.fernandez@bsc.es
 License: LGPL-2.1
 Project-URL: Bug Tracker, https://github.com/inab/pyrfc6920/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `rfc6920-0.1.3/setup.py` & `rfc6920-0.2.1/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -32,42 +32,41 @@
 from rfc6920 import __version__ as rfc6920_version
 from rfc6920 import __author__ as rfc6920_author
 from rfc6920 import __license__ as rfc6920_license
 
 # Populating the long description
 readme_path = os.path.join(setupDir, "README.md")
 with open(readme_path, "r") as fh:
-    long_description = fh.read()
+	long_description = fh.read()
 
 # Populating the install requirements
 requirements = []
 requirements_path = os.path.join(setupDir, "requirements.txt")
 if os.path.exists(requirements_path):
-    with open(requirements_path) as f:
-        egg = re.compile(r"#[^#]*egg=([^=&]+)")
-        for line in f.read().splitlines():
-            m = egg.search(line)
-            requirements.append(line if m is None else m.group(1))
+	with open(requirements_path) as f:
+		egg = re.compile(r"#[^#]*egg=([^=&]+)")
+		for line in f.read().splitlines():
+			m = egg.search(line)
+			requirements.append(line if m is None else m.group(1))
 
 setuptools.setup(
-    name="rfc6920",
-    version=rfc6920_version,
-    author=rfc6920_author,
-    author_email="jose.m.fernandez@bsc.es",
-    license=rfc6920_license,
-    description="A library to generate and validate RFC6920 URIs",
-    long_description=long_description,
-    long_description_content_type="text/markdown",
-    url="https://github.com/inab/pyrfc6920",
-	project_urls={
-		"Bug Tracker": "https://github.com/inab/pyrfc6920/issues"
-	},
-    packages=setuptools.find_packages(),
-    install_requires=requirements,
-    classifiers=[
-        "Programming Language :: Python :: 3",
-        "Development Status :: 3 - Alpha",
-        "License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)",
-        "Operating System :: OS Independent",
-    ],
+	name="rfc6920",
+	version=rfc6920_version,
+	author=rfc6920_author,
+	author_email="jose.m.fernandez@bsc.es",
+	license=rfc6920_license,
+	description="A library to generate and validate RFC6920 URIs",
+	long_description=long_description,
+	long_description_content_type="text/markdown",
+	url="https://github.com/inab/pyrfc6920",
+	project_urls={"Bug Tracker": "https://github.com/inab/pyrfc6920/issues"},
+	packages=setuptools.find_packages(),
+	package_data={"rfc6920": ["py.typed"]},
+	install_requires=requirements,
+	classifiers=[
+		"Programming Language :: Python :: 3",
+		"Development Status :: 3 - Alpha",
+		"License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)",
+		"Operating System :: OS Independent",
+	],
 	python_requires=">=3.6",
 )
```

