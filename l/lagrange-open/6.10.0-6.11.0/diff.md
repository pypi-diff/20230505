# Comparing `tmp/lagrange_open-6.10.0-cp39-cp39-win_amd64.whl.zip` & `tmp/lagrange_open-6.11.0-cp39-cp39-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,18 @@
-Zip file size: 973012 bytes, number of entries: 10
--rw-rw-rw-  2.0 fat      674 b- defN 23-Apr-06 14:01 lagrange/__init__.py
--rw-rw-rw-  2.0 fat  2622976 b- defN 23-Apr-06 14:01 lagrange/lagrange.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat   310784 b- defN 23-Apr-06 13:47 lagrange/tbb12.dll
--rw-rw-rw-  2.0 fat    44060 b- defN 23-Apr-06 13:47 lagrange/tbb12.lib
--rw-rw-rw-  2.0 fat    11536 b- defN 23-Apr-06 14:01 lagrange_open-6.10.0.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     1973 b- defN 23-Apr-06 14:01 lagrange_open-6.10.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat    11144 b- defN 23-Apr-06 14:01 lagrange_open-6.10.0.dist-info/NOTICE.txt
--rw-rw-rw-  2.0 fat       94 b- defN 23-Apr-06 14:01 lagrange_open-6.10.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 23-Apr-06 14:01 lagrange_open-6.10.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      845 b- defN 23-Apr-06 14:01 lagrange_open-6.10.0.dist-info/RECORD
-10 files, 3004095 bytes uncompressed, 971576 bytes compressed:  67.7%
+Zip file size: 2534283 bytes, number of entries: 16
+-rw-rw-rw-  2.0 fat      730 b- defN 23-May-05 01:52 lagrange/__init__.py
+-rw-rw-rw-  2.0 fat     1865 b- defN 23-May-05 01:52 lagrange/_logging.py
+-rw-rw-rw-  2.0 fat  6211584 b- defN 23-May-05 01:52 lagrange/lagrange.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat        0 b- defN 23-May-05 01:52 lagrange/py.typed
+-rw-rw-rw-  2.0 fat   310784 b- defN 23-May-05 01:30 lagrange/tbb12.dll
+-rw-rw-rw-  2.0 fat    44060 b- defN 23-May-05 01:30 lagrange/tbb12.lib
+-rw-rw-rw-  2.0 fat      151 b- defN 23-May-05 01:52 lagrange/lagrange/__init__.pyi
+-rw-rw-rw-  2.0 fat    36142 b- defN 23-May-05 01:52 lagrange/lagrange/core.pyi
+-rw-rw-rw-  2.0 fat     3517 b- defN 23-May-05 01:52 lagrange/lagrange/io.pyi
+-rw-rw-rw-  2.0 fat     2393 b- defN 23-May-05 01:52 lagrange/lagrange/scene.pyi
+-rw-rw-rw-  2.0 fat    11536 b- defN 23-May-05 01:52 lagrange_open-6.11.0.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     2008 b- defN 23-May-05 01:52 lagrange_open-6.11.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat    11144 b- defN 23-May-05 01:52 lagrange_open-6.11.0.dist-info/NOTICE.txt
+-rw-rw-rw-  2.0 fat       94 b- defN 23-May-05 01:52 lagrange_open-6.11.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        9 b- defN 23-May-05 01:52 lagrange_open-6.11.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1328 b- defN 23-May-05 01:52 lagrange_open-6.11.0.dist-info/RECORD
+16 files, 6637345 bytes uncompressed, 2532103 bytes compressed:  61.9%
```

## zipnote {}

```diff
@@ -1,31 +1,49 @@
 Filename: lagrange/__init__.py
 Comment: 
 
+Filename: lagrange/_logging.py
+Comment: 
+
 Filename: lagrange/lagrange.cp39-win_amd64.pyd
 Comment: 
 
+Filename: lagrange/py.typed
+Comment: 
+
 Filename: lagrange/tbb12.dll
 Comment: 
 
 Filename: lagrange/tbb12.lib
 Comment: 
 
-Filename: lagrange_open-6.10.0.dist-info/LICENSE
+Filename: lagrange/lagrange/__init__.pyi
+Comment: 
+
+Filename: lagrange/lagrange/core.pyi
+Comment: 
+
+Filename: lagrange/lagrange/io.pyi
+Comment: 
+
+Filename: lagrange/lagrange/scene.pyi
+Comment: 
+
+Filename: lagrange_open-6.11.0.dist-info/LICENSE
 Comment: 
 
-Filename: lagrange_open-6.10.0.dist-info/METADATA
+Filename: lagrange_open-6.11.0.dist-info/METADATA
 Comment: 
 
-Filename: lagrange_open-6.10.0.dist-info/NOTICE.txt
+Filename: lagrange_open-6.11.0.dist-info/NOTICE.txt
 Comment: 
 
-Filename: lagrange_open-6.10.0.dist-info/WHEEL
+Filename: lagrange_open-6.11.0.dist-info/WHEEL
 Comment: 
 
-Filename: lagrange_open-6.10.0.dist-info/top_level.txt
+Filename: lagrange_open-6.11.0.dist-info/top_level.txt
 Comment: 
 
-Filename: lagrange_open-6.10.0.dist-info/RECORD
+Filename: lagrange_open-6.11.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## lagrange/__init__.py

```diff
@@ -7,7 +7,10 @@
 # Unless required by applicable law or agreed to in writing, software distributed under
 # the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR REPRESENTATIONS
 # OF ANY KIND, either express or implied. See the License for the specific language
 # governing permissions and limitations under the License.
 #
 from .lagrange import *
 from .lagrange.core import *
+from ._logging import logger
+
+del _logging, lagrange
```

## lagrange/tbb12.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x000000018001b27c
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Thu Apr  6 13:47:37 2023
+Time/Date		Fri May  5 01:30:08 2023
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	35
 SizeOfCode		000000000001b200
 SizeOfInitializedData	0000000000030800
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	000000000001b27c
@@ -25,15 +25,15 @@
 MajorImageVersion	12
 MinorImageVersion	8
 MajorSubsystemVersion	6
 MinorSubsystemVersion	0
 Win32Version		00000000
 SizeOfImage		00052000
 SizeOfHeaders		00000400
-CheckSum		00054be5
+CheckSum		0004f96e
 Subsystem		00000002	(Windows GUI)
 DllCharacteristics	00000160
 					HIGH_ENTROPY_VA
 					DYNAMIC_BASE
 					NX_COMPAT
 SizeOfStackReserve	0000000000100000
 SizeOfStackCommit	0000000000001000
@@ -50291,16 +50291,18 @@
    1800200aa:	add    %eax,0x1(%rax)
    1800200b0:	loopne 0x180020085
    1800200b2:	add    %eax,0x1(%rax)
    1800200b8:	call   0x181820290
    1800200bd:	add    %al,(%rax)
    1800200bf:	add    %al,(%rax)
    1800200c1:	add    %al,(%rax)
-   1800200c3:	add    %bh,-0x33(%rcx)
-   1800200c6:	cs add %al,%fs:(%rax)
+   1800200c3:	add    %ah,(%rax)
+   1800200c5:	pop    %rsp
+   1800200c6:	push   %rsp
+   1800200c7:	add    %al,%fs:(%rax)
    1800200ca:	add    %al,(%rax)
    1800200cc:	or     $0x64000000,%eax
    1800200d1:	add    (%rax),%eax
    1800200d3:	add    %bh,(%rsp,%rsi,1)
    1800200d6:	add    (%rax),%al
    1800200d8:	cmp    $0x1a,%al
    1800200da:	add    (%rax),%al
```

## lagrange/tbb12.lib

### nm -s {}

```diff
@@ -195,25 +195,25 @@
 __imp_TBB_runtime_version in tbb12.dll
 
 tbb12.dll:
 0000000000000000 i .idata$2
 0000000000000000 i .idata$4
 0000000000000000 i .idata$5
 0000000000000000 i .idata$6
-0000000001017dd8 a @comp.id
+0000000001017dd9 a @comp.id
 0000000000000000 I __IMPORT_DESCRIPTOR_tbb12
                  U __NULL_IMPORT_DESCRIPTOR
                  U tbb12_NULL_THUNK_DATA
 
 tbb12.dll:
-0000000001017dd8 a @comp.id
+0000000001017dd9 a @comp.id
 0000000000000000 I __NULL_IMPORT_DESCRIPTOR
 
 tbb12.dll:
-0000000001017dd8 a @comp.id
+0000000001017dd9 a @comp.id
 0000000000000000 I tbb12_NULL_THUNK_DATA
 
 tbb12.dll:
 0000000000000000 I .idata$4
 0000000000000000 I .idata$5
 0000000000000000 I .idata$6
 0000000000000000 T .text
```

## Comparing `lagrange_open-6.10.0.dist-info/LICENSE` & `lagrange_open-6.11.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `lagrange_open-6.10.0.dist-info/METADATA` & `lagrange_open-6.11.0.dist-info/METADATA`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: lagrange-open
-Version: 6.10.0
+Version: 6.11.0
 Summary: A robust geometry processing engine
 Maintainer-email: Lagrange Core Team <lagrange-core@adobe.com>
 Project-URL: repo, https://github.com/adobe/lagrange
 Project-URL: doc, https://opensource.adobe.com/lagrange-docs
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: NOTICE.txt
 Requires-Dist: numpy (>=1.23)
+Requires-Dist: colorama (>=0.4.5)
 
 # About Project Lagrange
 
 Project Lagrange is an initiative to bring the power of robust geometry processing to Adobe products. It bridges cutting edge research works with cutting edge products. Project Lagrange is built on the following design principles:
 
 ### Modular design
```

## Comparing `lagrange_open-6.10.0.dist-info/NOTICE.txt` & `lagrange_open-6.11.0.dist-info/NOTICE.txt`

 * *Files identical despite different names*

