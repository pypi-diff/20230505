# Comparing `tmp/david-test-datadog-sma-0.1.1.tar.gz` & `tmp/david-test-datadog-sma-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "david-test-datadog-sma-0.1.1.tar", last modified: Thu May  4 21:49:14 2023, max compression
+gzip compressed data, was "david-test-datadog-sma-0.1.2.tar", last modified: Fri May  5 00:16:08 2023, max compression
```

## Comparing `david-test-datadog-sma-0.1.1.tar` & `david-test-datadog-sma-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:49:14.909523 david-test-datadog-sma-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-04 21:49:14.909523 david-test-datadog-sma-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-04 21:49:04.000000 david-test-datadog-sma-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 21:49:14.909523 david-test-datadog-sma-0.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:49:14.905523 david-test-datadog-sma-0.1.1/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 21:48:57.000000 david-test-datadog-sma-0.1.1/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:49:14.905523 david-test-datadog-sma-0.1.1/src/datadog-serverless-agent-linux-amd64/
--rwxr-xr-x   0 runner    (1001) docker     (123)   980596 2023-05-04 21:49:04.000000 david-test-datadog-sma-0.1.1/src/datadog-serverless-agent-linux-amd64/datadog-serverless-trace-mini-agent
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:49:14.905523 david-test-datadog-sma-0.1.1/src/datadog-serverless-agent-windows-amd64/
--rwxr-xr-x   0 runner    (1001) docker     (123)   947200 2023-05-04 21:49:04.000000 david-test-datadog-sma-0.1.1/src/datadog-serverless-agent-windows-amd64/datadog-serverless-trace-mini-agent.exe
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:49:14.909523 david-test-datadog-sma-0.1.1/src/david_test_datadog_sma.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-04 21:49:14.000000 david-test-datadog-sma-0.1.1/src/david_test_datadog_sma.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-04 21:49:14.000000 david-test-datadog-sma-0.1.1/src/david_test_datadog_sma.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 21:49:14.000000 david-test-datadog-sma-0.1.1/src/david_test_datadog_sma.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-04 21:49:14.000000 david-test-datadog-sma-0.1.1/src/david_test_datadog_sma.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 00:16:08.398542 david-test-datadog-sma-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-05 00:16:08.398542 david-test-datadog-sma-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-05 00:16:00.000000 david-test-datadog-sma-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 00:16:08.398542 david-test-datadog-sma-0.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 00:16:08.394542 david-test-datadog-sma-0.1.2/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 00:15:56.000000 david-test-datadog-sma-0.1.2/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 00:16:08.394542 david-test-datadog-sma-0.1.2/src/datadog-serverless-agent-linux-amd64/
+-rwxr-xr-x   0 runner    (1001) docker     (123)   968564 2023-05-05 00:16:00.000000 david-test-datadog-sma-0.1.2/src/datadog-serverless-agent-linux-amd64/datadog-serverless-trace-mini-agent
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 00:16:08.398542 david-test-datadog-sma-0.1.2/src/datadog-serverless-agent-windows-amd64/
+-rwxr-xr-x   0 runner    (1001) docker     (123)   947200 2023-05-05 00:16:00.000000 david-test-datadog-sma-0.1.2/src/datadog-serverless-agent-windows-amd64/datadog-serverless-trace-mini-agent.exe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 00:16:08.398542 david-test-datadog-sma-0.1.2/src/david_test_datadog_sma.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-05 00:16:08.000000 david-test-datadog-sma-0.1.2/src/david_test_datadog_sma.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-05 00:16:08.000000 david-test-datadog-sma-0.1.2/src/david_test_datadog_sma.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 00:16:08.000000 david-test-datadog-sma-0.1.2/src/david_test_datadog_sma.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-05 00:16:08.000000 david-test-datadog-sma-0.1.2/src/david_test_datadog_sma.egg-info/top_level.txt
```

### Comparing `david-test-datadog-sma-0.1.1/src/datadog-serverless-agent-linux-amd64/datadog-serverless-trace-mini-agent` & `david-test-datadog-sma-0.1.2/src/datadog-serverless-agent-linux-amd64/datadog-serverless-trace-mini-agent`

 * *Files 9% similar despite different names*

#### readelf --wide --file-header {}

```diff
@@ -4,17 +4,17 @@
   Data:                              2's complement, little endian
   Version:                           1 (current)
   OS/ABI:                            UNIX - System V
   ABI Version:                       0
   Type:                              DYN (Shared object file)
   Machine:                           Advanced Micro Devices X86-64
   Version:                           0x1
-  Entry point address:               0xee088
+  Entry point address:               0x351028
   Start of program headers:          64 (bytes into file)
   Start of section headers:          0 (bytes into file)
   Flags:                             0x0
   Size of this header:               64 (bytes)
   Size of program headers:           56 (bytes)
   Number of program headers:         3
-  Size of section headers:           64 (bytes)
+  Size of section headers:           0 (bytes)
   Number of section headers:         0
   Section header string table index: 0
```

#### readelf --wide --program-header {}

```diff
@@ -1,10 +1,10 @@
 
 Elf file type is DYN (Shared object file)
-Entry point 0xee088
+Entry point 0x351028
 There are 3 program headers, starting at offset 64
 
 Program Headers:
   Type           Offset   VirtAddr           PhysAddr           FileSiz  MemSiz   Flg Align
-  LOAD           0x000000 0x0000000000000000 0x0000000000000000 0x0ef33e 0x0ef33e R E 0x1000
-  LOAD           0x000000 0x00000000000f0000 0x00000000000f0000 0x000000 0x175230 RW  0x1000
+  LOAD           0x000000 0x0000000000000000 0x0000000000000000 0x001000 0x265230 RW  0x1000
+  LOAD           0x000000 0x0000000000266000 0x0000000000266000 0x0ec43d 0x0ec43d R E 0x1000
   GNU_STACK      0x000000 0x0000000000000000 0x0000000000000000 0x000000 0x000000 RW  0x10
```

#### strings --all --bytes=8 {}

```diff
@@ -1,22 +1,10 @@
-nux-x86-
-pITM_deregist
-GetLanguageSpecificDa^
-6tcv8osix
-xxb_impl
-o?prot`%lph~+
-rsd_xpg1O
-6KrarTWkey
-wI_phH#s.
-m	6cGLIBC_H
-qrrHNP}wX
-Fvv:M/@G
-ldAOw/hw
- 8P@xX!g`
-?HCrvdG@
+B/K!aN_ 
+t-;MD%Jru&f9
+gGWWw;p#
 ?LfQCU-&
 WJ`X$\k01A
 3^l{[$P1e
 FnN=u~nXl
 ftwc( |\
 ht> eyz!
  Sac!llm
@@ -214,9 +202,9 @@
 Z/q.M0'$J
 Mg[tO	_l
 BmKqb}%o
 ]PE!R6cU
 []A\A]A^A_H
 PROT_EXEC|PROT_WRITE failed.
 $Info: This file is packed with the UPX executable packer http://upx.sf.net $
-$Id: UPX 3.96 Copyright (C) 1996-2020 the UPX Team. All Rights Reserved. $
+$Id: UPX 4.02 Copyright (C) 1996-2023 the UPX Team. All Rights Reserved. $
 /proc/self/exe
```

### Comparing `david-test-datadog-sma-0.1.1/src/datadog-serverless-agent-windows-amd64/datadog-serverless-trace-mini-agent.exe` & `david-test-datadog-sma-0.1.2/src/datadog-serverless-agent-windows-amd64/datadog-serverless-trace-mini-agent.exe`

 * *Files 1% similar despite different names*

#### objdump

 * *error from `objdump --all-headers --disassemble-all --line-numbers --no-show-raw-insn {}`:*

 * *objdump: error: /tmp/diffoscope_153yn74f_/tmpxow4vfdj_TarContainer/0/9.exe(UPX0) is too large (0x1a8000 bytes)*

 * *objdump: Reading section UPX0 failed because: file truncated*

```diff
@@ -3,15 +3,15 @@
 HAS_RELOC, EXEC_P, HAS_LINENO, HAS_DEBUG, HAS_LOCALS, D_PAGED
 start address 0x000000014028e9a0
 
 Characteristics 0x22
 	executable
 	large address aware
 
-Time/Date		Thu May  4 16:44:03 2023
+Time/Date		Thu May  4 23:46:28 2023
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	35
 SizeOfCode		00000000000e7000
 SizeOfInitializedData	0000000000001000
 SizeOfUninitializedData	00000000001a8000
 AddressOfEntryPoint	000000000028e9a0
@@ -23,15 +23,15 @@
 MinorOSystemVersion	0
 MajorImageVersion	0
 MinorImageVersion	0
 MajorSubsystemVersion	6
 MinorSubsystemVersion	0
 Win32Version		00000000
 SizeOfImage		00291000
-SizeOfHeaders		00001000
+SizeOfHeaders		00000400
 CheckSum		00000000
 Subsystem		00000003	(Windows CUI)
 DllCharacteristics	00008160
 					HIGH_ENTROPY_VA
 					DYNAMIC_BASE
 					NX_COMPAT
 					TERMINAL_SERVICE_AWARE
@@ -48,16 +48,16 @@
 Entry 2 0000000000000000 00000000 Resource Directory [.rsrc]
 Entry 3 0000000000273000 000152c4 Exception Directory [.pdata]
 Entry 4 0000000000000000 00000000 Security Directory
 Entry 5 00000000002903f4 00000024 Base Relocation Directory [.reloc]
 Entry 6 0000000000000000 00000000 Debug Directory
 Entry 7 0000000000000000 00000000 Description Directory
 Entry 8 0000000000000000 00000000 Special Directory
-Entry 9 000000000028f5c8 00000028 Thread Storage Directory [.tls]
-Entry a 000000000028f790 00000140 Load Configuration Directory
+Entry 9 000000000028f5d8 00000028 Thread Storage Directory [.tls]
+Entry a 000000000028f7a0 00000140 Load Configuration Directory
 Entry b 0000000000000000 00000000 Bound Import Directory
 Entry c 0000000000000000 00000000 Import Address Table Directory
 Entry d 0000000000000000 00000000 Delay Import Directory
 Entry e 0000000000000000 00000000 CLR Runtime Header
 Entry f 0000000000000000 00000000 Reserved
 
 There is an import table in UPX2 at 0x140290000
@@ -359193,82 +359193,95 @@
    14028e8bd:	xchg   %eax,%edx
    14028e8be:	(bad)
    14028e8bf:	fildll 0x35187b70(%rcx)
    14028e8c5:	xchg   %bl,0x4e7fdb62(%rsi)
    14028e8cb:	or     $0x8642a967,%eax
    14028e8d0:	(bad)
    14028e8d1:	enter  $0xe218,$0x1b
-   14028e8d5:	sbb    %ecx,0x0(%rdx)
-   14028e8d8:	(bad)
-   14028e8d9:	add    %ch,(%rsi,%rsi,8)
-   14028e8dc:	(bad)
-   14028e8dd:	cs rex.XB pop %r14
-   14028e8e0:	adc    $0xe1953b0f,%eax
-   14028e8e5:	(bad)
-   14028e8e6:	sub    %eax,-0xcc1cae4(%rsi)
-   14028e8ec:	rcrb   $0xbe,0x75(%rcx)
-   14028e8f0:	cld
-   14028e8f1:	(bad)
-   14028e8f2:	rex.RX int $0x6e
-   14028e8f5:	test   $0x40,%al
-   14028e8f7:	jae    0x14028e893
-   14028e8f9:	lock outsl %ds:(%rsi),(%dx)
-   14028e8fb:	xchg   %eax,%ebp
-   14028e8fc:	cltd
-   14028e8fd:	push   $0xffffffffffffffe7
-   14028e8ff:	movsxd (%rdi),%edi
-   14028e901:	sub    $0x2e29ad44,%eax
-   14028e906:	adc    $0xba,%al
-   14028e908:	sbb    0x3aadb08a(%rbp),%dh
-   14028e90e:	movsb  %ds:(%rsi),%es:(%rdi)
-   14028e90f:	in     $0x75,%eax
-   14028e911:	rcrl   $0x5a,(%rcx)
-   14028e914:	shr    %bl
-   14028e916:	pop    %rcx
-   14028e917:	mov    $0xb1a2658d,%eax
-   14028e91c:	pop    %rsp
-   14028e91d:	mov    $0xe8,%bl
-   14028e91f:	jb     0x114e618f1
-   14028e925:	call   0x14562881e
-   14028e92a:	lock cmp 0x19(%rax),%esp
-   14028e92e:	xchg   %eax,%ebp
-   14028e92f:	rex.WB jbe 0x14028e93f
-   14028e932:	(bad)
-   14028e933:	and    $0xbca28bec,%eax
-   14028e938:	adc    $0xb3e2d774,%eax
-   14028e93d:	shll   $0x25,0x4deddbf7(%rbx)
-   14028e944:	lret   $0xa8a
-   14028e947:	cmp    0x11(%rdx),%ah
-   14028e94a:	ret    $0x1442
-   14028e94d:	xor    $0x8c0bef9e,%eax
-   14028e952:	jae    0x14028e93e
-   14028e954:	fisttpll -0x64(%rdx)
-   14028e957:	sarb   $0xa9,-0xf(%rbp,%rbp,2)
-   14028e95c:	insb   (%dx),%es:(%rdi)
-   14028e95d:	and    $0x719c66d6,%eax
-   14028e962:	imul   $0xffffffe6,-0x64(%rcx),%ebp
-   14028e966:	adc    $0xd366b28d,%eax
-   14028e96b:	rex.WRB mov $0xc3,%r15b
-   14028e96e:	cld
-   14028e96f:	and    %ecx,-0x2e634323(%rbp)
-   14028e975:	rcrb   $0x57,0x725444dd(%rdi)
-   14028e97c:	(bad)
-   14028e97d:	and    %ch,%dh
-   14028e97f:	(bad)
-   14028e983:	xchg   %eax,%edx
-   14028e984:	ret    $0x38ee
-   14028e987:	push   %rdi
-   14028e988:	(bad)
-   14028e989:	repz iret
-   14028e98b:	sbb    %si,%si
-   14028e98e:	or     $0xf9b6f333,%eax
-   14028e993:	jne    0x14028e92c
-   14028e995:	jno    0x14028e9e7
-	...
-   14028e99f:	add    %dl,0x56(%rbx)
+   14028e8d5:	sbb    %bh,-0x4d(%rcx,%rcx,4)
+   14028e8d9:	fwait
+   14028e8da:	imul   $0xffffffd5,(%rsi),%ebp
+   14028e8dd:	jrcxz  0x14028e871
+   14028e8df:	push   %rdx
+   14028e8e0:	int3
+   14028e8e1:	xor    $0x24be12d7,%eax
+   14028e8e6:	clc
+   14028e8e7:	insl   (%dx),%es:(%rdi)
+   14028e8e8:	sub    (%rcx,%rsi,1),%ah
+   14028e8eb:	xor    $0x8c83e58f,%eax
+   14028e8f0:	xchg   %eax,%esp
+   14028e8f1:	ds pop %rsi
+   14028e8f3:	jl     0x14028e96e
+   14028e8f5:	mov    $0x2c,%al
+   14028e8f7:	mov    (%rsi,%rdx,2),%cl
+   14028e8fa:	cmp    $0x4a,%al
+   14028e8fc:	out    %eax,(%dx)
+   14028e8fd:	and    -0x105210d3(%rcx),%esi
+   14028e903:	xorl   $0xd66db7e6,-0x19(%rdx)
+   14028e90a:	push   %rsi
+   14028e90b:	xchg   %eax,%ecx
+   14028e90c:	sub    $0x94fb93c9,%eax
+   14028e911:	rex.WR out %al,(%dx)
+   14028e913:	in     $0xb6,%eax
+   14028e915:	jrcxz  0x14028e93e
+   14028e917:	divl   (%rsi,%rdx,8)
+   14028e91a:	fistpll (%ebx,%ebp,1)
+   14028e91e:	sub    %esp,%ebx
+   14028e920:	pop    %rdx
+   14028e921:	js     0x14028e8f3
+   14028e923:	(bad)
+   14028e927:	movabs 0xa21dbfc67c60b591,%al
+   14028e930:	(bad)
+   14028e931:	rex.R jg 0x14028e8ff
+   14028e934:	movabs 0x66fd0271d37ac1f4,%al
+   14028e93d:	xor    0x7d05cdaf(%rdi),%dl
+   14028e943:	movsl  %ds:(%rsi),%es:(%rdi)
+   14028e944:	cli
+   14028e945:	pop    %rbp
+   14028e946:	mov    %dh,%cl
+   14028e948:	adc    %dl,-0x71(%rbx)
+   14028e94b:	rex.W test $0x4,%al
+   14028e94e:	xor    $0xdfeec39b,%eax
+   14028e953:	(bad)
+   14028e954:	(bad)
+   14028e955:	hlt
+   14028e956:	rex.RXB (bad)
+   14028e958:	fistpl -0x5b(%rax)
+   14028e95b:	movabs %eax,0x1c24e3450b4c9e95
+   14028e964:	mov    (%rdi),%ah
+   14028e966:	rex.W (bad)
+   14028e968:	std
+   14028e969:	rcrb   $0x61,(%rbx)
+   14028e96c:	cmovo  0x49(%rbx),%edx
+   14028e970:	xchg   %eax,%edx
+   14028e971:	rex.WRX
+   14028e972:	rex.WB (bad)
+   14028e974:	sbb    %edi,%edi
+   14028e976:	int1
+   14028e977:	fs (bad)
+   14028e979:	and    $0x54,%al
+   14028e97b:	jg     0x14028e98b
+   14028e97d:	out    %al,$0x73
+   14028e97f:	jg     0x14028e969
+   14028e981:	cmp    %esp,%edx
+   14028e983:	sub    $0x2d,%al
+   14028e985:	rex.RB push %r14
+   14028e987:	imul   $0x5d,%edi,%esi
+   14028e98a:	(bad)
+   14028e98b:	out    %al,$0xe3
+   14028e98d:	mov    $0xfc,%al
+   14028e98f:	xchg   %eax,%edx
+   14028e990:	mul    %ecx
+   14028e992:	rex.B xlat %ds:(%rbx)
+   14028e994:	sub    %dl,0xfc(%rcx)
+   14028e99a:	add    %al,(%rax)
+   14028e99c:	add    %al,(%rax)
+   14028e99e:	add    %al,(%rax)
+   14028e9a0:	push   %rbx
+   14028e9a1:	push   %rsi
    14028e9a2:	push   %rdi
    14028e9a3:	push   %rbp
    14028e9a4:	lea    -0xe59ab(%rip),%rsi        # 0x1401a9000
    14028e9ab:	lea    -0x1a8000(%rsi),%rdi
    14028e9b2:	lea    0x271330(%rdi),%rax
    14028e9b9:	push   (%rax)
    14028e9bb:	movl   $0x8321ba67,(%rax)
@@ -359318,914 +359331,919 @@
    14028ea3a:	push   %r14
    14028ea3c:	mov    $0x1,%r14d
    14028ea42:	push   %r13
    14028ea44:	xor    %r13d,%r13d
    14028ea47:	push   %r12
    14028ea49:	push   %rbp
    14028ea4a:	push   %rbx
-   14028ea4b:	mov    %rcx,-0x10(%rsp)
-   14028ea50:	mov    %rax,-0x28(%rsp)
-   14028ea55:	mov    $0x1,%eax
-   14028ea5a:	mov    %rsi,-0x8(%rsp)
-   14028ea5f:	mov    %r8,-0x18(%rsp)
-   14028ea64:	mov    %eax,%ebx
-   14028ea66:	mov    %r9d,-0x1c(%rsp)
-   14028ea6b:	movzbl 0x2(%rdi),%ecx
-   14028ea6f:	shl    %cl,%ebx
-   14028ea71:	mov    %ebx,%ecx
-   14028ea73:	mov    0x38(%rsp),%rbx
-   14028ea78:	dec    %ecx
-   14028ea7a:	mov    %ecx,-0x2c(%rsp)
-   14028ea7e:	movzbl 0x1(%rdi),%ecx
-   14028ea82:	shl    %cl,%eax
-   14028ea84:	mov    -0x10(%rsp),%rcx
-   14028ea89:	dec    %eax
-   14028ea8b:	mov    %eax,-0x30(%rsp)
-   14028ea8f:	movzbl (%rdi),%eax
-   14028ea92:	movl   $0x0,(%rcx)
-   14028ea98:	movl   $0x0,-0x38(%rsp)
-   14028eaa0:	movl   $0x1,-0x3c(%rsp)
-   14028eaa8:	movl   $0x1,-0x40(%rsp)
-   14028eab0:	movl   $0x1,-0x44(%rsp)
-   14028eab8:	movl   $0x0,(%rbx)
-   14028eabe:	mov    %eax,-0x34(%rsp)
-   14028eac2:	movzbl 0x1(%rdi),%ecx
-   14028eac6:	add    %eax,%ecx
-   14028eac8:	mov    $0x300,%eax
-   14028eacd:	shl    %cl,%eax
-   14028eacf:	xor    %ecx,%ecx
-   14028ead1:	lea    0x736(%rax),%edi
-   14028ead7:	cmp    %edi,%r15d
-   14028eada:	jae    0x14028eaef
-   14028eadc:	mov    -0x28(%rsp),%rbx
-   14028eae1:	mov    %ecx,%eax
-   14028eae3:	inc    %ecx
-   14028eae5:	cmp    %edi,%ecx
-   14028eae7:	movw   $0x400,(%rbx,%rax,2)
-   14028eaed:	jmp    0x14028eada
-   14028eaef:	mov    -0x8(%rsp),%rdi
-   14028eaf4:	mov    %edx,%eax
-   14028eaf6:	xor    %r10d,%r10d
-   14028eaf9:	or     $0xffffffff,%r11d
-   14028eafd:	xor    %edx,%edx
-   14028eaff:	mov    %rdi,%r12
-   14028eb02:	add    %rax,%r12
-   14028eb05:	cmp    %r12,%rdi
-   14028eb08:	je     0x14028f3fd
-   14028eb0e:	movzbl (%rdi),%eax
-   14028eb11:	shl    $0x8,%r10d
-   14028eb15:	inc    %edx
-   14028eb17:	inc    %rdi
-   14028eb1a:	or     %eax,%r10d
-   14028eb1d:	cmp    $0x4,%edx
-   14028eb20:	jle    0x14028eb05
-   14028eb22:	cmp    -0x1c(%rsp),%r15d
-   14028eb27:	jae    0x14028f407
-   14028eb2d:	mov    -0x2c(%rsp),%eax
-   14028eb31:	movslq -0x38(%rsp),%rbx
-   14028eb36:	mov    -0x28(%rsp),%rdx
-   14028eb3b:	and    %r15d,%eax
-   14028eb3e:	mov    %eax,-0x48(%rsp)
-   14028eb42:	movslq -0x48(%rsp),%rbp
-   14028eb47:	mov    %rbx,%rax
-   14028eb4a:	shl    $0x4,%rax
-   14028eb4e:	add    %rbp,%rax
-   14028eb51:	cmp    $0xffffff,%r11d
-   14028eb58:	lea    (%rdx,%rax,2),%r9
-   14028eb5c:	ja     0x14028eb78
-   14028eb5e:	cmp    %r12,%rdi
-   14028eb61:	je     0x14028f3fd
-   14028eb67:	movzbl (%rdi),%eax
-   14028eb6a:	shl    $0x8,%r10d
-   14028eb6e:	shl    $0x8,%r11d
-   14028eb72:	inc    %rdi
-   14028eb75:	or     %eax,%r10d
-   14028eb78:	movzwl (%r9),%edx
-   14028eb7c:	mov    %r11d,%eax
-   14028eb7f:	shr    $0xb,%eax
-   14028eb82:	movzwl %dx,%ecx
-   14028eb85:	imul   %ecx,%eax
-   14028eb88:	cmp    %eax,%r10d
-   14028eb8b:	jae    0x14028ed56
-   14028eb91:	mov    %eax,%r11d
-   14028eb94:	mov    $0x800,%eax
-   14028eb99:	mov    -0x28(%rsp),%rbx
-   14028eb9e:	sub    %ecx,%eax
-   14028eba0:	movzbl -0x34(%rsp),%ecx
-   14028eba5:	mov    $0x1,%esi
-   14028ebaa:	sar    $0x5,%eax
-   14028ebad:	lea    (%rdx,%rax,1),%eax
-   14028ebb0:	movzbl %r13b,%edx
-   14028ebb4:	mov    %ax,(%r9)
-   14028ebb8:	mov    -0x30(%rsp),%eax
-   14028ebbc:	and    %r15d,%eax
-   14028ebbf:	shl    %cl,%eax
-   14028ebc1:	mov    $0x8,%ecx
-   14028ebc6:	sub    -0x34(%rsp),%ecx
-   14028ebca:	sar    %cl,%edx
-   14028ebcc:	add    %edx,%eax
-   14028ebce:	imul   $0x300,%eax,%eax
-   14028ebd4:	cmpl   $0x6,-0x38(%rsp)
-   14028ebd9:	mov    %eax,%eax
-   14028ebdb:	lea    0xe6c(%rbx,%rax,2),%r9
-   14028ebe3:	jle    0x14028eca1
-   14028ebe9:	mov    -0x18(%rsp),%rdx
-   14028ebee:	mov    %r15d,%eax
-   14028ebf1:	sub    %r14d,%eax
-   14028ebf4:	movzbl (%rdx,%rax,1),%ebp
-   14028ebf8:	add    %ebp,%ebp
-   14028ebfa:	movslq %esi,%rdx
-   14028ebfd:	mov    %ebp,%ebx
-   14028ebff:	and    $0x100,%ebx
-   14028ec05:	cmp    $0xffffff,%r11d
-   14028ec0c:	movslq %ebx,%rax
-   14028ec0f:	lea    (%r9,%rax,2),%rax
-   14028ec13:	lea    (%rax,%rdx,2),%r8
-   14028ec17:	ja     0x14028ec33
-   14028ec19:	cmp    %r12,%rdi
-   14028ec1c:	je     0x14028f3fd
-   14028ec22:	movzbl (%rdi),%eax
-   14028ec25:	shl    $0x8,%r10d
-   14028ec29:	shl    $0x8,%r11d
-   14028ec2d:	inc    %rdi
-   14028ec30:	or     %eax,%r10d
-   14028ec33:	movzwl 0x200(%r8),%edx
-   14028ec3b:	mov    %r11d,%eax
-   14028ec3e:	shr    $0xb,%eax
-   14028ec41:	movzwl %dx,%ecx
-   14028ec44:	imul   %ecx,%eax
-   14028ec47:	cmp    %eax,%r10d
-   14028ec4a:	jae    0x14028ec6c
-   14028ec4c:	mov    %eax,%r11d
-   14028ec4f:	mov    $0x800,%eax
-   14028ec54:	add    %esi,%esi
-   14028ec56:	sub    %ecx,%eax
-   14028ec58:	sar    $0x5,%eax
-   14028ec5b:	test   %ebx,%ebx
-   14028ec5d:	lea    (%rdx,%rax,1),%eax
-   14028ec60:	mov    %ax,0x200(%r8)
-   14028ec68:	je     0x14028ec8b
-   14028ec6a:	jmp    0x14028ec99
-   14028ec6c:	sub    %eax,%r11d
-   14028ec6f:	sub    %eax,%r10d
-   14028ec72:	mov    %edx,%eax
-   14028ec74:	shr    $0x5,%ax
-   14028ec78:	lea    0x1(%rsi,%rsi,1),%esi
-   14028ec7c:	sub    %ax,%dx
-   14028ec7f:	test   %ebx,%ebx
-   14028ec81:	mov    %dx,0x200(%r8)
-   14028ec89:	je     0x14028ec99
-   14028ec8b:	cmp    $0xff,%esi
-   14028ec91:	jle    0x14028ebf8
-   14028ec97:	jmp    0x14028ed11
-   14028ec99:	cmp    $0xff,%esi
-   14028ec9f:	jg     0x14028ed11
-   14028eca1:	movslq %esi,%rax
-   14028eca4:	cmp    $0xffffff,%r11d
-   14028ecab:	lea    (%r9,%rax,2),%r8
-   14028ecaf:	ja     0x14028eccb
-   14028ecb1:	cmp    %r12,%rdi
-   14028ecb4:	je     0x14028f3fd
-   14028ecba:	movzbl (%rdi),%eax
-   14028ecbd:	shl    $0x8,%r10d
-   14028ecc1:	shl    $0x8,%r11d
-   14028ecc5:	inc    %rdi
-   14028ecc8:	or     %eax,%r10d
-   14028eccb:	movzwl (%r8),%edx
-   14028eccf:	mov    %r11d,%eax
-   14028ecd2:	shr    $0xb,%eax
-   14028ecd5:	movzwl %dx,%ecx
-   14028ecd8:	imul   %ecx,%eax
-   14028ecdb:	cmp    %eax,%r10d
-   14028ecde:	jae    0x14028ecf8
-   14028ece0:	mov    %eax,%r11d
-   14028ece3:	mov    $0x800,%eax
-   14028ece8:	add    %esi,%esi
-   14028ecea:	sub    %ecx,%eax
-   14028ecec:	sar    $0x5,%eax
-   14028ecef:	lea    (%rdx,%rax,1),%eax
-   14028ecf2:	mov    %ax,(%r8)
-   14028ecf6:	jmp    0x14028ec99
-   14028ecf8:	sub    %eax,%r11d
-   14028ecfb:	sub    %eax,%r10d
-   14028ecfe:	mov    %edx,%eax
-   14028ed00:	shr    $0x5,%ax
-   14028ed04:	lea    0x1(%rsi,%rsi,1),%esi
-   14028ed08:	sub    %ax,%dx
-   14028ed0b:	mov    %dx,(%r8)
-   14028ed0f:	jmp    0x14028ec99
-   14028ed11:	mov    -0x18(%rsp),%rcx
-   14028ed16:	mov    %r15d,%eax
-   14028ed19:	inc    %r15d
-   14028ed1c:	mov    %esi,%r13d
-   14028ed1f:	mov    %sil,(%rcx,%rax,1)
-   14028ed23:	cmpl   $0x3,-0x38(%rsp)
-   14028ed28:	jg     0x14028ed37
-   14028ed2a:	movl   $0x0,-0x38(%rsp)
-   14028ed32:	jmp    0x14028f3dd
-   14028ed37:	mov    -0x38(%rsp),%edx
-   14028ed3b:	mov    -0x38(%rsp),%eax
-   14028ed3f:	sub    $0x3,%edx
-   14028ed42:	sub    $0x6,%eax
-   14028ed45:	cmpl   $0x9,-0x38(%rsp)
-   14028ed4a:	cmovg  %eax,%edx
-   14028ed4d:	mov    %edx,-0x38(%rsp)
-   14028ed51:	jmp    0x14028f3dd
-   14028ed56:	sub    %eax,%r11d
-   14028ed59:	sub    %eax,%r10d
-   14028ed5c:	mov    %edx,%eax
-   14028ed5e:	shr    $0x5,%ax
-   14028ed62:	sub    %ax,%dx
-   14028ed65:	mov    -0x28(%rsp),%rax
-   14028ed6a:	cmp    $0xffffff,%r11d
-   14028ed71:	mov    %dx,(%r9)
-   14028ed75:	lea    (%rax,%rbx,2),%rsi
-   14028ed79:	ja     0x14028ed95
-   14028ed7b:	cmp    %r12,%rdi
-   14028ed7e:	je     0x14028f3fd
-   14028ed84:	movzbl (%rdi),%eax
-   14028ed87:	shl    $0x8,%r10d
-   14028ed8b:	shl    $0x8,%r11d
-   14028ed8f:	inc    %rdi
-   14028ed92:	or     %eax,%r10d
-   14028ed95:	movzwl 0x180(%rsi),%edx
-   14028ed9c:	mov    %r11d,%eax
-   14028ed9f:	shr    $0xb,%eax
-   14028eda2:	movzwl %dx,%ecx
-   14028eda5:	imul   %ecx,%eax
-   14028eda8:	cmp    %eax,%r10d
-   14028edab:	jae    0x14028edfb
-   14028edad:	mov    %eax,%r11d
-   14028edb0:	mov    $0x800,%eax
-   14028edb5:	mov    -0x28(%rsp),%r9
-   14028edba:	sub    %ecx,%eax
-   14028edbc:	mov    -0x3c(%rsp),%ecx
-   14028edc0:	mov    %r14d,-0x3c(%rsp)
-   14028edc5:	sar    $0x5,%eax
-   14028edc8:	lea    (%rdx,%rax,1),%eax
-   14028edcb:	mov    -0x40(%rsp),%edx
-   14028edcf:	mov    %ecx,-0x40(%rsp)
-   14028edd3:	mov    %ax,0x180(%rsi)
-   14028edda:	xor    %eax,%eax
-   14028eddc:	cmpl   $0x6,-0x38(%rsp)
-   14028ede1:	mov    %edx,-0x44(%rsp)
-   14028ede5:	setg   %al
-   14028ede8:	add    $0x664,%r9
-   14028edef:	lea    (%rax,%rax,2),%eax
-   14028edf2:	mov    %eax,-0x38(%rsp)
-   14028edf6:	jmp    0x14028f04f
-   14028edfb:	sub    %eax,%r11d
-   14028edfe:	sub    %eax,%r10d
-   14028ee01:	mov    %edx,%eax
-   14028ee03:	shr    $0x5,%ax
-   14028ee07:	sub    %ax,%dx
-   14028ee0a:	cmp    $0xffffff,%r11d
-   14028ee11:	mov    %dx,0x180(%rsi)
-   14028ee18:	ja     0x14028ee34
-   14028ee1a:	cmp    %r12,%rdi
-   14028ee1d:	je     0x14028f3fd
-   14028ee23:	movzbl (%rdi),%eax
-   14028ee26:	shl    $0x8,%r10d
-   14028ee2a:	shl    $0x8,%r11d
-   14028ee2e:	inc    %rdi
-   14028ee31:	or     %eax,%r10d
-   14028ee34:	movzwl 0x198(%rsi),%edx
-   14028ee3b:	mov    %r11d,%eax
-   14028ee3e:	shr    $0xb,%eax
-   14028ee41:	movzwl %dx,%ecx
-   14028ee44:	imul   %ecx,%eax
-   14028ee47:	cmp    %eax,%r10d
-   14028ee4a:	jae    0x14028ef20
-   14028ee50:	mov    $0x800,%r8d
-   14028ee56:	mov    %eax,%r11d
-   14028ee59:	shl    $0x5,%rbx
-   14028ee5d:	mov    %r8d,%eax
-   14028ee60:	sub    %ecx,%eax
-   14028ee62:	sar    $0x5,%eax
-   14028ee65:	lea    (%rdx,%rax,1),%eax
-   14028ee68:	mov    %ax,0x198(%rsi)
-   14028ee6f:	mov    -0x28(%rsp),%rax
-   14028ee74:	add    %rbx,%rax
-   14028ee77:	cmp    $0xffffff,%r11d
-   14028ee7e:	lea    (%rax,%rbp,2),%rsi
-   14028ee82:	ja     0x14028ee9e
-   14028ee84:	cmp    %r12,%rdi
-   14028ee87:	je     0x14028f3fd
-   14028ee8d:	movzbl (%rdi),%eax
-   14028ee90:	shl    $0x8,%r10d
-   14028ee94:	shl    $0x8,%r11d
-   14028ee98:	inc    %rdi
-   14028ee9b:	or     %eax,%r10d
-   14028ee9e:	movzwl 0x1e0(%rsi),%edx
-   14028eea5:	mov    %r11d,%eax
-   14028eea8:	shr    $0xb,%eax
-   14028eeab:	movzwl %dx,%ecx
-   14028eeae:	imul   %ecx,%eax
-   14028eeb1:	cmp    %eax,%r10d
-   14028eeb4:	jae    0x14028ef05
-   14028eeb6:	sub    %ecx,%r8d
-   14028eeb9:	mov    %eax,%r11d
-   14028eebc:	sar    $0x5,%r8d
-   14028eec0:	test   %r15d,%r15d
-   14028eec3:	lea    (%rdx,%r8,1),%eax
-   14028eec7:	mov    %ax,0x1e0(%rsi)
-   14028eece:	je     0x14028f3fd
-   14028eed4:	xor    %eax,%eax
-   14028eed6:	cmpl   $0x6,-0x38(%rsp)
-   14028eedb:	mov    -0x18(%rsp),%rbx
-   14028eee0:	setg   %al
-   14028eee3:	lea    0x9(%rax,%rax,1),%eax
-   14028eee7:	mov    %eax,-0x38(%rsp)
-   14028eeeb:	mov    %r15d,%eax
-   14028eeee:	sub    %r14d,%eax
-   14028eef1:	movzbl (%rbx,%rax,1),%r13d
-   14028eef6:	mov    %r15d,%eax
-   14028eef9:	inc    %r15d
-   14028eefc:	mov    %r13b,(%rbx,%rax,1)
-   14028ef00:	jmp    0x14028f3dd
-   14028ef05:	sub    %eax,%r11d
-   14028ef08:	sub    %eax,%r10d
-   14028ef0b:	mov    %edx,%eax
-   14028ef0d:	shr    $0x5,%ax
-   14028ef11:	sub    %ax,%dx
-   14028ef14:	mov    %dx,0x1e0(%rsi)
-   14028ef1b:	jmp    0x14028f031
-   14028ef20:	sub    %eax,%r11d
-   14028ef23:	sub    %eax,%r10d
-   14028ef26:	mov    %edx,%eax
-   14028ef28:	shr    $0x5,%ax
-   14028ef2c:	sub    %ax,%dx
-   14028ef2f:	cmp    $0xffffff,%r11d
-   14028ef36:	mov    %dx,0x198(%rsi)
-   14028ef3d:	ja     0x14028ef59
-   14028ef3f:	cmp    %r12,%rdi
-   14028ef42:	je     0x14028f3fd
-   14028ef48:	movzbl (%rdi),%eax
-   14028ef4b:	shl    $0x8,%r10d
-   14028ef4f:	shl    $0x8,%r11d
-   14028ef53:	inc    %rdi
-   14028ef56:	or     %eax,%r10d
-   14028ef59:	movzwl 0x1b0(%rsi),%edx
-   14028ef60:	mov    %r11d,%eax
-   14028ef63:	shr    $0xb,%eax
-   14028ef66:	movzwl %dx,%ecx
-   14028ef69:	imul   %ecx,%eax
-   14028ef6c:	cmp    %eax,%r10d
-   14028ef6f:	jae    0x14028ef91
-   14028ef71:	mov    %eax,%r11d
-   14028ef74:	mov    $0x800,%eax
-   14028ef79:	sub    %ecx,%eax
-   14028ef7b:	sar    $0x5,%eax
-   14028ef7e:	lea    (%rdx,%rax,1),%eax
-   14028ef81:	mov    %ax,0x1b0(%rsi)
-   14028ef88:	mov    -0x3c(%rsp),%eax
-   14028ef8c:	jmp    0x14028f029
-   14028ef91:	sub    %eax,%r11d
-   14028ef94:	sub    %eax,%r10d
-   14028ef97:	mov    %edx,%eax
-   14028ef99:	shr    $0x5,%ax
-   14028ef9d:	sub    %ax,%dx
-   14028efa0:	cmp    $0xffffff,%r11d
-   14028efa7:	mov    %dx,0x1b0(%rsi)
-   14028efae:	ja     0x14028efca
-   14028efb0:	cmp    %r12,%rdi
-   14028efb3:	je     0x14028f3fd
-   14028efb9:	movzbl (%rdi),%eax
-   14028efbc:	shl    $0x8,%r10d
-   14028efc0:	shl    $0x8,%r11d
-   14028efc4:	inc    %rdi
-   14028efc7:	or     %eax,%r10d
-   14028efca:	movzwl 0x1c8(%rsi),%edx
-   14028efd1:	mov    %r11d,%eax
-   14028efd4:	shr    $0xb,%eax
-   14028efd7:	movzwl %dx,%ecx
-   14028efda:	imul   %ecx,%eax
-   14028efdd:	cmp    %eax,%r10d
-   14028efe0:	jae    0x14028efff
-   14028efe2:	mov    %eax,%r11d
-   14028efe5:	mov    $0x800,%eax
-   14028efea:	sub    %ecx,%eax
-   14028efec:	sar    $0x5,%eax
-   14028efef:	lea    (%rdx,%rax,1),%eax
-   14028eff2:	mov    %ax,0x1c8(%rsi)
-   14028eff9:	mov    -0x40(%rsp),%eax
-   14028effd:	jmp    0x14028f021
-   14028efff:	sub    %eax,%r11d
-   14028f002:	sub    %eax,%r10d
-   14028f005:	mov    %edx,%eax
-   14028f007:	shr    $0x5,%ax
-   14028f00b:	sub    %ax,%dx
-   14028f00e:	mov    -0x44(%rsp),%eax
-   14028f012:	mov    %dx,0x1c8(%rsi)
-   14028f019:	mov    -0x40(%rsp),%edx
-   14028f01d:	mov    %edx,-0x44(%rsp)
-   14028f021:	mov    -0x3c(%rsp),%ecx
-   14028f025:	mov    %ecx,-0x40(%rsp)
-   14028f029:	mov    %r14d,-0x3c(%rsp)
-   14028f02e:	mov    %eax,%r14d
-   14028f031:	xor    %eax,%eax
-   14028f033:	cmpl   $0x6,-0x38(%rsp)
-   14028f038:	mov    -0x28(%rsp),%r9
-   14028f03d:	setg   %al
-   14028f040:	add    $0xa68,%r9
-   14028f047:	lea    0x8(%rax,%rax,2),%eax
-   14028f04b:	mov    %eax,-0x38(%rsp)
-   14028f04f:	cmp    $0xffffff,%r11d
-   14028f056:	ja     0x14028f072
-   14028f058:	cmp    %r12,%rdi
-   14028f05b:	je     0x14028f3fd
-   14028f061:	movzbl (%rdi),%eax
-   14028f064:	shl    $0x8,%r10d
-   14028f068:	shl    $0x8,%r11d
-   14028f06c:	inc    %rdi
-   14028f06f:	or     %eax,%r10d
-   14028f072:	movzwl (%r9),%edx
-   14028f076:	mov    %r11d,%eax
-   14028f079:	shr    $0xb,%eax
-   14028f07c:	movzwl %dx,%ecx
-   14028f07f:	imul   %ecx,%eax
-   14028f082:	cmp    %eax,%r10d
-   14028f085:	jae    0x14028f0ae
-   14028f087:	mov    %eax,%r11d
-   14028f08a:	mov    $0x800,%eax
-   14028f08f:	xor    %r13d,%r13d
-   14028f092:	sub    %ecx,%eax
-   14028f094:	sar    $0x5,%eax
-   14028f097:	lea    (%rdx,%rax,1),%eax
-   14028f09a:	mov    %ax,(%r9)
-   14028f09e:	movslq -0x48(%rsp),%rax
-   14028f0a3:	shl    $0x4,%rax
-   14028f0a7:	lea    0x4(%r9,%rax,1),%r8
-   14028f0ac:	jmp    0x14028f126
-   14028f0ae:	sub    %eax,%r11d
-   14028f0b1:	sub    %eax,%r10d
-   14028f0b4:	mov    %edx,%eax
-   14028f0b6:	shr    $0x5,%ax
-   14028f0ba:	sub    %ax,%dx
-   14028f0bd:	cmp    $0xffffff,%r11d
-   14028f0c4:	mov    %dx,(%r9)
-   14028f0c8:	ja     0x14028f0e4
-   14028f0ca:	cmp    %r12,%rdi
-   14028f0cd:	je     0x14028f3fd
-   14028f0d3:	movzbl (%rdi),%eax
-   14028f0d6:	shl    $0x8,%r10d
-   14028f0da:	shl    $0x8,%r11d
-   14028f0de:	inc    %rdi
-   14028f0e1:	or     %eax,%r10d
-   14028f0e4:	movzwl 0x2(%r9),%edx
-   14028f0e9:	mov    %r11d,%eax
-   14028f0ec:	shr    $0xb,%eax
-   14028f0ef:	movzwl %dx,%ecx
-   14028f0f2:	imul   %ecx,%eax
-   14028f0f5:	cmp    %eax,%r10d
-   14028f0f8:	jae    0x14028f12e
-   14028f0fa:	mov    %eax,%r11d
-   14028f0fd:	mov    $0x800,%eax
-   14028f102:	mov    $0x8,%r13d
-   14028f108:	sub    %ecx,%eax
-   14028f10a:	sar    $0x5,%eax
-   14028f10d:	lea    (%rdx,%rax,1),%eax
-   14028f110:	mov    %ax,0x2(%r9)
-   14028f115:	movslq -0x48(%rsp),%rax
-   14028f11a:	shl    $0x4,%rax
-   14028f11e:	lea    0x104(%r9,%rax,1),%r8
-   14028f126:	mov    $0x3,%r9d
-   14028f12c:	jmp    0x14028f155
-   14028f12e:	sub    %eax,%r11d
-   14028f131:	sub    %eax,%r10d
-   14028f134:	mov    %edx,%eax
-   14028f136:	shr    $0x5,%ax
-   14028f13a:	lea    0x204(%r9),%r8
-   14028f141:	mov    $0x10,%r13d
-   14028f147:	sub    %ax,%dx
-   14028f14a:	mov    %dx,0x2(%r9)
-   14028f14f:	mov    $0x8,%r9d
-   14028f155:	mov    %r9d,%ebx
-   14028f158:	mov    $0x1,%ebp
-   14028f15d:	movslq %ebp,%rax
-   14028f160:	cmp    $0xffffff,%r11d
-   14028f167:	lea    (%r8,%rax,2),%rsi
-   14028f16b:	ja     0x14028f187
-   14028f16d:	cmp    %r12,%rdi
-   14028f170:	je     0x14028f3fd
-   14028f176:	movzbl (%rdi),%eax
-   14028f179:	shl    $0x8,%r10d
-   14028f17d:	shl    $0x8,%r11d
-   14028f181:	inc    %rdi
-   14028f184:	or     %eax,%r10d
-   14028f187:	movzwl (%rsi),%ecx
-   14028f18a:	mov    %r11d,%eax
-   14028f18d:	shr    $0xb,%eax
-   14028f190:	movzwl %cx,%edx
-   14028f193:	imul   %edx,%eax
-   14028f196:	cmp    %eax,%r10d
-   14028f199:	jae    0x14028f1b2
-   14028f19b:	mov    %eax,%r11d
-   14028f19e:	mov    $0x800,%eax
-   14028f1a3:	add    %ebp,%ebp
-   14028f1a5:	sub    %edx,%eax
-   14028f1a7:	sar    $0x5,%eax
-   14028f1aa:	lea    (%rcx,%rax,1),%eax
-   14028f1ad:	mov    %ax,(%rsi)
-   14028f1b0:	jmp    0x14028f1c8
-   14028f1b2:	sub    %eax,%r11d
-   14028f1b5:	sub    %eax,%r10d
-   14028f1b8:	mov    %ecx,%eax
-   14028f1ba:	shr    $0x5,%ax
-   14028f1be:	lea    0x1(%rbp,%rbp,1),%ebp
-   14028f1c2:	sub    %ax,%cx
-   14028f1c5:	mov    %cx,(%rsi)
-   14028f1c8:	dec    %ebx
-   14028f1ca:	jne    0x14028f15d
-   14028f1cc:	mov    $0x1,%eax
-   14028f1d1:	mov    %r9d,%ecx
-   14028f1d4:	shl    %cl,%eax
-   14028f1d6:	sub    %eax,%ebp
-   14028f1d8:	add    %r13d,%ebp
-   14028f1db:	cmpl   $0x3,-0x38(%rsp)
-   14028f1e0:	jg     0x14028f3a8
-   14028f1e6:	addl   $0x7,-0x38(%rsp)
-   14028f1eb:	mov    $0x3,%eax
-   14028f1f0:	cmp    $0x4,%ebp
-   14028f1f3:	cmovl  %ebp,%eax
-   14028f1f6:	mov    -0x28(%rsp),%rbx
-   14028f1fb:	mov    $0x1,%r8d
-   14028f201:	cltq
-   14028f203:	shl    $0x7,%rax
-   14028f207:	lea    0x360(%rbx,%rax,1),%r9
-   14028f20f:	mov    $0x6,%ebx
-   14028f214:	movslq %r8d,%rax
-   14028f217:	cmp    $0xffffff,%r11d
-   14028f21e:	lea    (%r9,%rax,2),%rsi
-   14028f222:	ja     0x14028f23e
-   14028f224:	cmp    %r12,%rdi
-   14028f227:	je     0x14028f3fd
-   14028f22d:	movzbl (%rdi),%eax
-   14028f230:	shl    $0x8,%r10d
-   14028f234:	shl    $0x8,%r11d
-   14028f238:	inc    %rdi
-   14028f23b:	or     %eax,%r10d
-   14028f23e:	movzwl (%rsi),%edx
-   14028f241:	mov    %r11d,%eax
-   14028f244:	shr    $0xb,%eax
-   14028f247:	movzwl %dx,%ecx
-   14028f24a:	imul   %ecx,%eax
-   14028f24d:	cmp    %eax,%r10d
-   14028f250:	jae    0x14028f26a
-   14028f252:	mov    %eax,%r11d
-   14028f255:	mov    $0x800,%eax
-   14028f25a:	add    %r8d,%r8d
-   14028f25d:	sub    %ecx,%eax
-   14028f25f:	sar    $0x5,%eax
-   14028f262:	lea    (%rdx,%rax,1),%eax
-   14028f265:	mov    %ax,(%rsi)
-   14028f268:	jmp    0x14028f281
-   14028f26a:	sub    %eax,%r11d
-   14028f26d:	sub    %eax,%r10d
-   14028f270:	mov    %edx,%eax
-   14028f272:	shr    $0x5,%ax
-   14028f276:	lea    0x1(%r8,%r8,1),%r8d
-   14028f27b:	sub    %ax,%dx
-   14028f27e:	mov    %dx,(%rsi)
-   14028f281:	dec    %ebx
-   14028f283:	jne    0x14028f214
-   14028f285:	sub    $0x40,%r8d
-   14028f289:	cmp    $0x3,%r8d
-   14028f28d:	mov    %r8d,%r14d
-   14028f290:	jle    0x14028f3a3
-   14028f296:	and    $0x1,%r14d
-   14028f29a:	mov    %r8d,%eax
-   14028f29d:	sar    %eax
-   14028f29f:	or     $0x2,%r14d
-   14028f2a3:	cmp    $0xd,%r8d
-   14028f2a7:	lea    -0x1(%rax),%esi
-   14028f2aa:	jg     0x14028f2cf
-   14028f2ac:	mov    %esi,%ecx
-   14028f2ae:	mov    -0x28(%rsp),%rbx
-   14028f2b3:	movslq %r8d,%rax
-   14028f2b6:	shl    %cl,%r14d
-   14028f2b9:	add    %rax,%rax
-   14028f2bc:	mov    %r14d,%edx
-   14028f2bf:	lea    (%rbx,%rdx,2),%rdx
-   14028f2c3:	sub    %rax,%rdx
-   14028f2c6:	lea    0x55e(%rdx),%r9
-   14028f2cd:	jmp    0x14028f320
-   14028f2cf:	lea    -0x5(%rax),%esi
-   14028f2d2:	cmp    $0xffffff,%r11d
-   14028f2d9:	ja     0x14028f2f5
-   14028f2db:	cmp    %r12,%rdi
-   14028f2de:	je     0x14028f3fd
-   14028f2e4:	movzbl (%rdi),%eax
-   14028f2e7:	shl    $0x8,%r10d
-   14028f2eb:	shl    $0x8,%r11d
-   14028f2ef:	inc    %rdi
-   14028f2f2:	or     %eax,%r10d
-   14028f2f5:	shr    %r11d
-   14028f2f8:	add    %r14d,%r14d
-   14028f2fb:	cmp    %r11d,%r10d
-   14028f2fe:	jb     0x14028f307
-   14028f300:	sub    %r11d,%r10d
-   14028f303:	or     $0x1,%r14d
-   14028f307:	dec    %esi
-   14028f309:	jne    0x14028f2d2
-   14028f30b:	mov    -0x28(%rsp),%r9
-   14028f310:	shl    $0x4,%r14d
-   14028f314:	mov    $0x4,%esi
-   14028f319:	add    $0x644,%r9
-   14028f320:	mov    $0x1,%r13d
-   14028f326:	mov    $0x1,%ebx
-   14028f32b:	movslq %ebx,%rax
-   14028f32e:	cmp    $0xffffff,%r11d
-   14028f335:	lea    (%r9,%rax,2),%r8
-   14028f339:	ja     0x14028f355
-   14028f33b:	cmp    %r12,%rdi
-   14028f33e:	je     0x14028f3fd
-   14028f344:	movzbl (%rdi),%eax
-   14028f347:	shl    $0x8,%r10d
-   14028f34b:	shl    $0x8,%r11d
-   14028f34f:	inc    %rdi
-   14028f352:	or     %eax,%r10d
-   14028f355:	movzwl (%r8),%edx
-   14028f359:	mov    %r11d,%eax
-   14028f35c:	shr    $0xb,%eax
-   14028f35f:	movzwl %dx,%ecx
-   14028f362:	imul   %ecx,%eax
-   14028f365:	cmp    %eax,%r10d
-   14028f368:	jae    0x14028f382
-   14028f36a:	mov    %eax,%r11d
-   14028f36d:	mov    $0x800,%eax
-   14028f372:	add    %ebx,%ebx
-   14028f374:	sub    %ecx,%eax
-   14028f376:	sar    $0x5,%eax
-   14028f379:	lea    (%rdx,%rax,1),%eax
-   14028f37c:	mov    %ax,(%r8)
-   14028f380:	jmp    0x14028f39c
-   14028f382:	sub    %eax,%r11d
-   14028f385:	sub    %eax,%r10d
-   14028f388:	mov    %edx,%eax
-   14028f38a:	shr    $0x5,%ax
-   14028f38e:	lea    0x1(%rbx,%rbx,1),%ebx
-   14028f392:	or     %r13d,%r14d
-   14028f395:	sub    %ax,%dx
-   14028f398:	mov    %dx,(%r8)
-   14028f39c:	add    %r13d,%r13d
-   14028f39f:	dec    %esi
-   14028f3a1:	jne    0x14028f32b
-   14028f3a3:	inc    %r14d
-   14028f3a6:	je     0x14028f3e8
-   14028f3a8:	add    $0x2,%ebp
-   14028f3ab:	cmp    %r15d,%r14d
-   14028f3ae:	ja     0x14028f3fd
-   14028f3b0:	mov    -0x18(%rsp),%rdx
-   14028f3b5:	mov    %r15d,%eax
-   14028f3b8:	sub    %r14d,%eax
-   14028f3bb:	movzbl (%rdx,%rax,1),%r13d
-   14028f3c0:	mov    %r15d,%eax
-   14028f3c3:	inc    %r15d
-   14028f3c6:	dec    %ebp
-   14028f3c8:	mov    %r13b,(%rdx,%rax,1)
-   14028f3cc:	setne  %dl
-   14028f3cf:	xor    %eax,%eax
-   14028f3d1:	cmp    -0x1c(%rsp),%r15d
-   14028f3d6:	setb   %al
-   14028f3d9:	test   %eax,%edx
-   14028f3db:	jne    0x14028f3b0
-   14028f3dd:	cmp    -0x1c(%rsp),%r15d
-   14028f3e2:	jb     0x14028eb2d
-   14028f3e8:	cmp    $0xffffff,%r11d
-   14028f3ef:	ja     0x14028f407
-   14028f3f1:	cmp    %r12,%rdi
-   14028f3f4:	mov    $0x1,%eax
-   14028f3f9:	je     0x14028f41e
-   14028f3fb:	jmp    0x14028f404
-   14028f3fd:	mov    $0x1,%eax
-   14028f402:	jmp    0x14028f41e
-   14028f404:	inc    %rdi
-   14028f407:	mov    %edi,%eax
-   14028f409:	sub    -0x8(%rsp),%eax
-   14028f40d:	mov    -0x10(%rsp),%rcx
-   14028f412:	mov    0x38(%rsp),%rbx
-   14028f417:	mov    %eax,(%rcx)
-   14028f419:	mov    %r15d,(%rbx)
-   14028f41c:	xor    %eax,%eax
-   14028f41e:	pop    %rbx
-   14028f41f:	pop    %rbp
-   14028f420:	pop    %r12
-   14028f422:	pop    %r13
-   14028f424:	pop    %r14
-   14028f426:	pop    %r15
-   14028f428:	leave
-   14028f429:	pop    %rax
-   14028f42a:	pop    %rsi
-   14028f42b:	pop    %rdi
-   14028f42c:	pop    %rax
-   14028f42d:	mov    %eax,(%rdi)
-   14028f42f:	mov    %rsi,%rdi
-   14028f432:	push   %rsi
-   14028f433:	mov    %rsi,%rdi
-   14028f436:	mov    $0x1c2800,%rsi
-   14028f43d:	mov    $0x1d,%dl
-   14028f43f:	push   %rbx
-   14028f440:	push   %rdi
-   14028f441:	lea    -0x3(%rdi,%rsi,1),%rcx
-   14028f446:	pop    %rsi
-   14028f447:	push   %rsi
-   14028f448:	pop    %rbx
-   14028f449:	jmp    0x14028f47a
-   14028f44b:	cmp    %rcx,%rsi
-   14028f44e:	jae    0x14028f482
-   14028f450:	push   %rsi
-   14028f451:	pop    %rsi
-   14028f452:	lods   %ds:(%rsi),%al
-   14028f453:	cmp    $0x80,%al
-   14028f455:	jb     0x14028f461
-   14028f457:	cmp    $0x8f,%al
-   14028f459:	ja     0x14028f461
-   14028f45b:	cmpb   $0xf,-0x2(%rsi)
-   14028f45f:	je     0x14028f467
-   14028f461:	sub    $0xe8,%al
-   14028f463:	cmp    $0x1,%al
-   14028f465:	ja     0x14028f44b
-   14028f467:	cmp    %rcx,%rsi
-   14028f46a:	jae    0x14028f482
-   14028f46c:	push   %rsi
-   14028f46d:	lods   %ds:(%rsi),%eax
-   14028f46e:	sub    %dl,%al
-   14028f470:	jne    0x14028f451
-   14028f472:	pop    %rdi
-   14028f473:	bswap  %eax
-   14028f475:	sub    %edi,%eax
-   14028f477:	add    %ebx,%eax
-   14028f479:	stos   %eax,%es:(%rdi)
-   14028f47a:	cmp    %rcx,%rsi
-   14028f47d:	jae    0x14028f482
-   14028f47f:	lods   %ds:(%rsi),%al
-   14028f480:	jmp    0x14028f461
-   14028f482:	pop    %rbx
-   14028f483:	pop    %rsi
-   14028f484:	sub    $0x28,%rsp
-   14028f488:	lea    0x28b000(%rsi),%rdi
-   14028f48f:	mov    (%rdi),%eax
-   14028f491:	or     %eax,%eax
-   14028f493:	je     0x14028f4df
-   14028f495:	mov    0x4(%rdi),%ebx
-   14028f498:	lea    0x28f000(%rax,%rsi,1),%rcx
-   14028f4a0:	add    %rsi,%rbx
-   14028f4a3:	add    $0x8,%rdi
-   14028f4a7:	call   *0xcfb(%rip)        # 0x1402901a8
-   14028f4ad:	xchg   %rax,%rbp
-   14028f4af:	mov    (%rdi),%al
-   14028f4b1:	inc    %rdi
-   14028f4b4:	or     %al,%al
-   14028f4b6:	je     0x14028f48f
-   14028f4b8:	mov    %rdi,%rcx
-   14028f4bb:	mov    %rdi,%rdx
-   14028f4be:	dec    %eax
-   14028f4c0:	repnz scas %es:(%rdi),%al
-   14028f4c2:	mov    %rbp,%rcx
-   14028f4c5:	call   *0xced(%rip)        # 0x1402901b8
-   14028f4cb:	or     %rax,%rax
-   14028f4ce:	je     0x14028f4d9
-   14028f4d0:	mov    %rax,(%rbx)
-   14028f4d3:	add    $0x8,%rbx
-   14028f4d7:	jmp    0x14028f4af
-   14028f4d9:	jmp    *0xcd1(%rip)        # 0x1402901b0
-   14028f4df:	add    $0x28,%rsp
-   14028f4e3:	add    $0x4,%rdi
-   14028f4e7:	lea    -0x4(%rsi),%rbx
-   14028f4eb:	xor    %eax,%eax
-   14028f4ed:	mov    (%rdi),%al
-   14028f4ef:	inc    %rdi
-   14028f4f2:	or     %eax,%eax
-   14028f4f4:	je     0x14028f523
-   14028f4f6:	cmp    $0xef,%al
-   14028f4f8:	ja     0x14028f50b
-   14028f4fa:	add    %rax,%rbx
-   14028f4fd:	mov    (%rbx),%rax
-   14028f500:	bswap  %rax
-   14028f503:	add    %rsi,%rax
-   14028f506:	mov    %rax,(%rbx)
-   14028f509:	jmp    0x14028f4eb
-   14028f50b:	and    $0xf,%al
-   14028f50d:	shl    $0x10,%eax
-   14028f510:	mov    (%rdi),%ax
-   14028f513:	add    $0x2,%rdi
-   14028f517:	or     %eax,%eax
-   14028f519:	jne    0x14028f4fa
-   14028f51b:	mov    (%rdi),%eax
-   14028f51d:	add    $0x4,%rdi
-   14028f521:	jmp    0x14028f4fa
-   14028f523:	mov    0xc96(%rip),%rbp        # 0x1402901c0
-   14028f52a:	lea    -0x1000(%rsi),%rdi
-   14028f531:	mov    $0x1000,%ebx
-   14028f536:	push   %rax
-   14028f537:	mov    %rsp,%r9
-   14028f53a:	mov    $0x4,%r8d
-   14028f540:	mov    %rbx,%rdx
-   14028f543:	mov    %rdi,%rcx
-   14028f546:	sub    $0x20,%rsp
-   14028f54a:	call   *%rbp
-   14028f54c:	lea    0x237(%rdi),%rax
-   14028f553:	andb   $0x7f,(%rax)
-   14028f556:	andb   $0x7f,0x28(%rax)
-   14028f55a:	lea    0x20(%rsp),%r9
-   14028f55f:	mov    (%r9),%r8
-   14028f562:	mov    %rbx,%rdx
-   14028f565:	mov    %rdi,%rcx
-   14028f568:	call   *%rbp
-   14028f56a:	add    $0x28,%rsp
-   14028f56e:	movb   $0xfc,0x2d(%rip)        # 0x14028f5a2
-   14028f575:	lea    -0x1000(%rsi),%rcx
-   14028f57c:	push   $0x1
-   14028f57e:	pop    %rdx
-   14028f57f:	xor    %r8,%r8
-   14028f582:	push   %rax
-   14028f583:	call   0x14028f5a2
-   14028f588:	pop    %rax
-   14028f589:	pop    %rbp
-   14028f58a:	pop    %rdi
-   14028f58b:	pop    %rsi
-   14028f58c:	pop    %rbx
-   14028f58d:	lea    -0x80(%rsp),%rax
-   14028f592:	push   $0x0
-   14028f594:	cmp    %rax,%rsp
-   14028f597:	jne    0x14028f592
-   14028f599:	sub    $0xffffffffffffff80,%rsp
-   14028f59d:	jmp    0x1401b974c
-   14028f5a2:	ret
-   14028f5a3:	push   %rsi
-   14028f5a4:	lea    -0xcb0a3(%rip),%rsi        # 0x1401c4508
-   14028f5ab:	lods   %ds:(%rsi),%rax
-   14028f5ad:	test   %rax,%rax
-   14028f5b0:	je     0x14028f5c6
-   14028f5b2:	push   %rcx
-   14028f5b3:	push   %rdx
-   14028f5b4:	push   %r8
-   14028f5b6:	sub    $0x28,%rsp
-   14028f5ba:	call   *%rax
-   14028f5bc:	add    $0x28,%rsp
-   14028f5c0:	pop    %r8
-   14028f5c2:	pop    %rdx
-   14028f5c3:	pop    %rcx
-   14028f5c4:	jmp    0x14028f5ab
-   14028f5c6:	pop    %rsi
-   14028f5c7:	ret
-   14028f5c8:	lock cmc
-   14028f5ca:	sub    %al,0x1(%rax)
-   14028f5cd:	add    %al,(%rax)
-   14028f5cf:	add    %al,0x14028f7(%rax)
-   14028f5d5:	add    %al,(%rax)
-   14028f5d7:	add    %dh,(%rax)
-   14028f5d9:	and    (%rdi),%esp
-   14028f5db:	rex add %eax,(%rax)
-   14028f5de:	add    %al,(%rax)
-   14028f5e0:	xor    $0x28,%bh
-   14028f5e3:	rex add %eax,(%rax)
-	...
-   14028f5ee:	rex add %al,(%rax)
+   14028ea4b:	sub    $0x48,%rsp
+   14028ea4f:	mov    %rcx,0x38(%rsp)
+   14028ea54:	mov    %rax,0x20(%rsp)
+   14028ea59:	mov    $0x1,%eax
+   14028ea5e:	mov    %rsi,0x40(%rsp)
+   14028ea63:	mov    %r8,0x30(%rsp)
+   14028ea68:	mov    %eax,%ebx
+   14028ea6a:	mov    %r9d,0x2c(%rsp)
+   14028ea6f:	movzbl 0x2(%rdi),%ecx
+   14028ea73:	shl    %cl,%ebx
+   14028ea75:	mov    %ebx,%ecx
+   14028ea77:	mov    0x80(%rsp),%rbx
+   14028ea7f:	dec    %ecx
+   14028ea81:	mov    %ecx,0x1c(%rsp)
+   14028ea85:	movzbl 0x1(%rdi),%ecx
+   14028ea89:	shl    %cl,%eax
+   14028ea8b:	mov    0x38(%rsp),%rcx
+   14028ea90:	dec    %eax
+   14028ea92:	mov    %eax,0x18(%rsp)
+   14028ea96:	movzbl (%rdi),%eax
+   14028ea99:	movl   $0x0,(%rcx)
+   14028ea9f:	movl   $0x0,0x10(%rsp)
+   14028eaa7:	movl   $0x1,0xc(%rsp)
+   14028eaaf:	movl   $0x1,0x8(%rsp)
+   14028eab7:	movl   $0x1,0x4(%rsp)
+   14028eabf:	movl   $0x0,(%rbx)
+   14028eac5:	mov    %eax,0x14(%rsp)
+   14028eac9:	movzbl 0x1(%rdi),%ecx
+   14028eacd:	add    %eax,%ecx
+   14028eacf:	mov    $0x300,%eax
+   14028ead4:	shl    %cl,%eax
+   14028ead6:	xor    %ecx,%ecx
+   14028ead8:	lea    0x736(%rax),%edi
+   14028eade:	cmp    %edi,%r15d
+   14028eae1:	jae    0x14028eaf6
+   14028eae3:	mov    0x20(%rsp),%rbx
+   14028eae8:	mov    %ecx,%eax
+   14028eaea:	inc    %ecx
+   14028eaec:	cmp    %edi,%ecx
+   14028eaee:	movw   $0x400,(%rbx,%rax,2)
+   14028eaf4:	jmp    0x14028eae1
+   14028eaf6:	mov    0x40(%rsp),%rdi
+   14028eafb:	mov    %edx,%eax
+   14028eafd:	xor    %r10d,%r10d
+   14028eb00:	or     $0xffffffff,%r11d
+   14028eb04:	xor    %edx,%edx
+   14028eb06:	mov    %rdi,%r12
+   14028eb09:	add    %rax,%r12
+   14028eb0c:	cmp    %r12,%rdi
+   14028eb0f:	je     0x14028f400
+   14028eb15:	movzbl (%rdi),%eax
+   14028eb18:	shl    $0x8,%r10d
+   14028eb1c:	inc    %edx
+   14028eb1e:	inc    %rdi
+   14028eb21:	or     %eax,%r10d
+   14028eb24:	cmp    $0x4,%edx
+   14028eb27:	jle    0x14028eb0c
+   14028eb29:	cmp    0x2c(%rsp),%r15d
+   14028eb2e:	jae    0x14028f40a
+   14028eb34:	mov    0x1c(%rsp),%eax
+   14028eb38:	movslq 0x10(%rsp),%rbx
+   14028eb3d:	mov    0x20(%rsp),%rdx
+   14028eb42:	and    %r15d,%eax
+   14028eb45:	mov    %eax,(%rsp)
+   14028eb48:	movslq (%rsp),%rbp
+   14028eb4c:	mov    %rbx,%rax
+   14028eb4f:	shl    $0x4,%rax
+   14028eb53:	add    %rbp,%rax
+   14028eb56:	cmp    $0xffffff,%r11d
+   14028eb5d:	lea    (%rdx,%rax,2),%r9
+   14028eb61:	ja     0x14028eb7d
+   14028eb63:	cmp    %r12,%rdi
+   14028eb66:	je     0x14028f400
+   14028eb6c:	movzbl (%rdi),%eax
+   14028eb6f:	shl    $0x8,%r10d
+   14028eb73:	shl    $0x8,%r11d
+   14028eb77:	inc    %rdi
+   14028eb7a:	or     %eax,%r10d
+   14028eb7d:	movzwl (%r9),%edx
+   14028eb81:	mov    %r11d,%eax
+   14028eb84:	shr    $0xb,%eax
+   14028eb87:	movzwl %dx,%ecx
+   14028eb8a:	imul   %ecx,%eax
+   14028eb8d:	cmp    %eax,%r10d
+   14028eb90:	jae    0x14028ed5b
+   14028eb96:	mov    %eax,%r11d
+   14028eb99:	mov    $0x800,%eax
+   14028eb9e:	mov    0x20(%rsp),%rbx
+   14028eba3:	sub    %ecx,%eax
+   14028eba5:	movzbl 0x14(%rsp),%ecx
+   14028ebaa:	mov    $0x1,%esi
+   14028ebaf:	sar    $0x5,%eax
+   14028ebb2:	lea    (%rdx,%rax,1),%eax
+   14028ebb5:	movzbl %r13b,%edx
+   14028ebb9:	mov    %ax,(%r9)
+   14028ebbd:	mov    0x18(%rsp),%eax
+   14028ebc1:	and    %r15d,%eax
+   14028ebc4:	shl    %cl,%eax
+   14028ebc6:	mov    $0x8,%ecx
+   14028ebcb:	sub    0x14(%rsp),%ecx
+   14028ebcf:	sar    %cl,%edx
+   14028ebd1:	add    %edx,%eax
+   14028ebd3:	imul   $0x300,%eax,%eax
+   14028ebd9:	cmpl   $0x6,0x10(%rsp)
+   14028ebde:	mov    %eax,%eax
+   14028ebe0:	lea    0xe6c(%rbx,%rax,2),%r9
+   14028ebe8:	jle    0x14028eca6
+   14028ebee:	mov    0x30(%rsp),%rdx
+   14028ebf3:	mov    %r15d,%eax
+   14028ebf6:	sub    %r14d,%eax
+   14028ebf9:	movzbl (%rdx,%rax,1),%ebp
+   14028ebfd:	add    %ebp,%ebp
+   14028ebff:	movslq %esi,%rdx
+   14028ec02:	mov    %ebp,%ebx
+   14028ec04:	and    $0x100,%ebx
+   14028ec0a:	cmp    $0xffffff,%r11d
+   14028ec11:	movslq %ebx,%rax
+   14028ec14:	lea    (%r9,%rax,2),%rax
+   14028ec18:	lea    (%rax,%rdx,2),%r8
+   14028ec1c:	ja     0x14028ec38
+   14028ec1e:	cmp    %r12,%rdi
+   14028ec21:	je     0x14028f400
+   14028ec27:	movzbl (%rdi),%eax
+   14028ec2a:	shl    $0x8,%r10d
+   14028ec2e:	shl    $0x8,%r11d
+   14028ec32:	inc    %rdi
+   14028ec35:	or     %eax,%r10d
+   14028ec38:	movzwl 0x200(%r8),%edx
+   14028ec40:	mov    %r11d,%eax
+   14028ec43:	shr    $0xb,%eax
+   14028ec46:	movzwl %dx,%ecx
+   14028ec49:	imul   %ecx,%eax
+   14028ec4c:	cmp    %eax,%r10d
+   14028ec4f:	jae    0x14028ec71
+   14028ec51:	mov    %eax,%r11d
+   14028ec54:	mov    $0x800,%eax
+   14028ec59:	add    %esi,%esi
+   14028ec5b:	sub    %ecx,%eax
+   14028ec5d:	sar    $0x5,%eax
+   14028ec60:	test   %ebx,%ebx
+   14028ec62:	lea    (%rdx,%rax,1),%eax
+   14028ec65:	mov    %ax,0x200(%r8)
+   14028ec6d:	je     0x14028ec90
+   14028ec6f:	jmp    0x14028ec9e
+   14028ec71:	sub    %eax,%r11d
+   14028ec74:	sub    %eax,%r10d
+   14028ec77:	mov    %edx,%eax
+   14028ec79:	shr    $0x5,%ax
+   14028ec7d:	lea    0x1(%rsi,%rsi,1),%esi
+   14028ec81:	sub    %ax,%dx
+   14028ec84:	test   %ebx,%ebx
+   14028ec86:	mov    %dx,0x200(%r8)
+   14028ec8e:	je     0x14028ec9e
+   14028ec90:	cmp    $0xff,%esi
+   14028ec96:	jle    0x14028ebfd
+   14028ec9c:	jmp    0x14028ed16
+   14028ec9e:	cmp    $0xff,%esi
+   14028eca4:	jg     0x14028ed16
+   14028eca6:	movslq %esi,%rax
+   14028eca9:	cmp    $0xffffff,%r11d
+   14028ecb0:	lea    (%r9,%rax,2),%r8
+   14028ecb4:	ja     0x14028ecd0
+   14028ecb6:	cmp    %r12,%rdi
+   14028ecb9:	je     0x14028f400
+   14028ecbf:	movzbl (%rdi),%eax
+   14028ecc2:	shl    $0x8,%r10d
+   14028ecc6:	shl    $0x8,%r11d
+   14028ecca:	inc    %rdi
+   14028eccd:	or     %eax,%r10d
+   14028ecd0:	movzwl (%r8),%edx
+   14028ecd4:	mov    %r11d,%eax
+   14028ecd7:	shr    $0xb,%eax
+   14028ecda:	movzwl %dx,%ecx
+   14028ecdd:	imul   %ecx,%eax
+   14028ece0:	cmp    %eax,%r10d
+   14028ece3:	jae    0x14028ecfd
+   14028ece5:	mov    %eax,%r11d
+   14028ece8:	mov    $0x800,%eax
+   14028eced:	add    %esi,%esi
+   14028ecef:	sub    %ecx,%eax
+   14028ecf1:	sar    $0x5,%eax
+   14028ecf4:	lea    (%rdx,%rax,1),%eax
+   14028ecf7:	mov    %ax,(%r8)
+   14028ecfb:	jmp    0x14028ec9e
+   14028ecfd:	sub    %eax,%r11d
+   14028ed00:	sub    %eax,%r10d
+   14028ed03:	mov    %edx,%eax
+   14028ed05:	shr    $0x5,%ax
+   14028ed09:	lea    0x1(%rsi,%rsi,1),%esi
+   14028ed0d:	sub    %ax,%dx
+   14028ed10:	mov    %dx,(%r8)
+   14028ed14:	jmp    0x14028ec9e
+   14028ed16:	mov    0x30(%rsp),%rcx
+   14028ed1b:	mov    %r15d,%eax
+   14028ed1e:	inc    %r15d
+   14028ed21:	mov    %esi,%r13d
+   14028ed24:	mov    %sil,(%rcx,%rax,1)
+   14028ed28:	cmpl   $0x3,0x10(%rsp)
+   14028ed2d:	jg     0x14028ed3c
+   14028ed2f:	movl   $0x0,0x10(%rsp)
+   14028ed37:	jmp    0x14028f3e0
+   14028ed3c:	mov    0x10(%rsp),%edx
+   14028ed40:	mov    0x10(%rsp),%eax
+   14028ed44:	sub    $0x3,%edx
+   14028ed47:	sub    $0x6,%eax
+   14028ed4a:	cmpl   $0x9,0x10(%rsp)
+   14028ed4f:	cmovg  %eax,%edx
+   14028ed52:	mov    %edx,0x10(%rsp)
+   14028ed56:	jmp    0x14028f3e0
+   14028ed5b:	sub    %eax,%r11d
+   14028ed5e:	sub    %eax,%r10d
+   14028ed61:	mov    %edx,%eax
+   14028ed63:	shr    $0x5,%ax
+   14028ed67:	sub    %ax,%dx
+   14028ed6a:	mov    0x20(%rsp),%rax
+   14028ed6f:	cmp    $0xffffff,%r11d
+   14028ed76:	mov    %dx,(%r9)
+   14028ed7a:	lea    (%rax,%rbx,2),%rsi
+   14028ed7e:	ja     0x14028ed9a
+   14028ed80:	cmp    %r12,%rdi
+   14028ed83:	je     0x14028f400
+   14028ed89:	movzbl (%rdi),%eax
+   14028ed8c:	shl    $0x8,%r10d
+   14028ed90:	shl    $0x8,%r11d
+   14028ed94:	inc    %rdi
+   14028ed97:	or     %eax,%r10d
+   14028ed9a:	movzwl 0x180(%rsi),%edx
+   14028eda1:	mov    %r11d,%eax
+   14028eda4:	shr    $0xb,%eax
+   14028eda7:	movzwl %dx,%ecx
+   14028edaa:	imul   %ecx,%eax
+   14028edad:	cmp    %eax,%r10d
+   14028edb0:	jae    0x14028ee00
+   14028edb2:	mov    %eax,%r11d
+   14028edb5:	mov    $0x800,%eax
+   14028edba:	mov    0x20(%rsp),%r9
+   14028edbf:	sub    %ecx,%eax
+   14028edc1:	mov    0xc(%rsp),%ecx
+   14028edc5:	mov    %r14d,0xc(%rsp)
+   14028edca:	sar    $0x5,%eax
+   14028edcd:	lea    (%rdx,%rax,1),%eax
+   14028edd0:	mov    0x8(%rsp),%edx
+   14028edd4:	mov    %ecx,0x8(%rsp)
+   14028edd8:	mov    %ax,0x180(%rsi)
+   14028eddf:	xor    %eax,%eax
+   14028ede1:	cmpl   $0x6,0x10(%rsp)
+   14028ede6:	mov    %edx,0x4(%rsp)
+   14028edea:	setg   %al
+   14028eded:	add    $0x664,%r9
+   14028edf4:	lea    (%rax,%rax,2),%eax
+   14028edf7:	mov    %eax,0x10(%rsp)
+   14028edfb:	jmp    0x14028f054
+   14028ee00:	sub    %eax,%r11d
+   14028ee03:	sub    %eax,%r10d
+   14028ee06:	mov    %edx,%eax
+   14028ee08:	shr    $0x5,%ax
+   14028ee0c:	sub    %ax,%dx
+   14028ee0f:	cmp    $0xffffff,%r11d
+   14028ee16:	mov    %dx,0x180(%rsi)
+   14028ee1d:	ja     0x14028ee39
+   14028ee1f:	cmp    %r12,%rdi
+   14028ee22:	je     0x14028f400
+   14028ee28:	movzbl (%rdi),%eax
+   14028ee2b:	shl    $0x8,%r10d
+   14028ee2f:	shl    $0x8,%r11d
+   14028ee33:	inc    %rdi
+   14028ee36:	or     %eax,%r10d
+   14028ee39:	movzwl 0x198(%rsi),%edx
+   14028ee40:	mov    %r11d,%eax
+   14028ee43:	shr    $0xb,%eax
+   14028ee46:	movzwl %dx,%ecx
+   14028ee49:	imul   %ecx,%eax
+   14028ee4c:	cmp    %eax,%r10d
+   14028ee4f:	jae    0x14028ef25
+   14028ee55:	mov    $0x800,%r8d
+   14028ee5b:	mov    %eax,%r11d
+   14028ee5e:	shl    $0x5,%rbx
+   14028ee62:	mov    %r8d,%eax
+   14028ee65:	sub    %ecx,%eax
+   14028ee67:	sar    $0x5,%eax
+   14028ee6a:	lea    (%rdx,%rax,1),%eax
+   14028ee6d:	mov    %ax,0x198(%rsi)
+   14028ee74:	mov    0x20(%rsp),%rax
+   14028ee79:	add    %rbx,%rax
+   14028ee7c:	cmp    $0xffffff,%r11d
+   14028ee83:	lea    (%rax,%rbp,2),%rsi
+   14028ee87:	ja     0x14028eea3
+   14028ee89:	cmp    %r12,%rdi
+   14028ee8c:	je     0x14028f400
+   14028ee92:	movzbl (%rdi),%eax
+   14028ee95:	shl    $0x8,%r10d
+   14028ee99:	shl    $0x8,%r11d
+   14028ee9d:	inc    %rdi
+   14028eea0:	or     %eax,%r10d
+   14028eea3:	movzwl 0x1e0(%rsi),%edx
+   14028eeaa:	mov    %r11d,%eax
+   14028eead:	shr    $0xb,%eax
+   14028eeb0:	movzwl %dx,%ecx
+   14028eeb3:	imul   %ecx,%eax
+   14028eeb6:	cmp    %eax,%r10d
+   14028eeb9:	jae    0x14028ef0a
+   14028eebb:	sub    %ecx,%r8d
+   14028eebe:	mov    %eax,%r11d
+   14028eec1:	sar    $0x5,%r8d
+   14028eec5:	test   %r15d,%r15d
+   14028eec8:	lea    (%rdx,%r8,1),%eax
+   14028eecc:	mov    %ax,0x1e0(%rsi)
+   14028eed3:	je     0x14028f400
+   14028eed9:	xor    %eax,%eax
+   14028eedb:	cmpl   $0x6,0x10(%rsp)
+   14028eee0:	mov    0x30(%rsp),%rbx
+   14028eee5:	setg   %al
+   14028eee8:	lea    0x9(%rax,%rax,1),%eax
+   14028eeec:	mov    %eax,0x10(%rsp)
+   14028eef0:	mov    %r15d,%eax
+   14028eef3:	sub    %r14d,%eax
+   14028eef6:	movzbl (%rbx,%rax,1),%r13d
+   14028eefb:	mov    %r15d,%eax
+   14028eefe:	inc    %r15d
+   14028ef01:	mov    %r13b,(%rbx,%rax,1)
+   14028ef05:	jmp    0x14028f3e0
+   14028ef0a:	sub    %eax,%r11d
+   14028ef0d:	sub    %eax,%r10d
+   14028ef10:	mov    %edx,%eax
+   14028ef12:	shr    $0x5,%ax
+   14028ef16:	sub    %ax,%dx
+   14028ef19:	mov    %dx,0x1e0(%rsi)
+   14028ef20:	jmp    0x14028f036
+   14028ef25:	sub    %eax,%r11d
+   14028ef28:	sub    %eax,%r10d
+   14028ef2b:	mov    %edx,%eax
+   14028ef2d:	shr    $0x5,%ax
+   14028ef31:	sub    %ax,%dx
+   14028ef34:	cmp    $0xffffff,%r11d
+   14028ef3b:	mov    %dx,0x198(%rsi)
+   14028ef42:	ja     0x14028ef5e
+   14028ef44:	cmp    %r12,%rdi
+   14028ef47:	je     0x14028f400
+   14028ef4d:	movzbl (%rdi),%eax
+   14028ef50:	shl    $0x8,%r10d
+   14028ef54:	shl    $0x8,%r11d
+   14028ef58:	inc    %rdi
+   14028ef5b:	or     %eax,%r10d
+   14028ef5e:	movzwl 0x1b0(%rsi),%edx
+   14028ef65:	mov    %r11d,%eax
+   14028ef68:	shr    $0xb,%eax
+   14028ef6b:	movzwl %dx,%ecx
+   14028ef6e:	imul   %ecx,%eax
+   14028ef71:	cmp    %eax,%r10d
+   14028ef74:	jae    0x14028ef96
+   14028ef76:	mov    %eax,%r11d
+   14028ef79:	mov    $0x800,%eax
+   14028ef7e:	sub    %ecx,%eax
+   14028ef80:	sar    $0x5,%eax
+   14028ef83:	lea    (%rdx,%rax,1),%eax
+   14028ef86:	mov    %ax,0x1b0(%rsi)
+   14028ef8d:	mov    0xc(%rsp),%eax
+   14028ef91:	jmp    0x14028f02e
+   14028ef96:	sub    %eax,%r11d
+   14028ef99:	sub    %eax,%r10d
+   14028ef9c:	mov    %edx,%eax
+   14028ef9e:	shr    $0x5,%ax
+   14028efa2:	sub    %ax,%dx
+   14028efa5:	cmp    $0xffffff,%r11d
+   14028efac:	mov    %dx,0x1b0(%rsi)
+   14028efb3:	ja     0x14028efcf
+   14028efb5:	cmp    %r12,%rdi
+   14028efb8:	je     0x14028f400
+   14028efbe:	movzbl (%rdi),%eax
+   14028efc1:	shl    $0x8,%r10d
+   14028efc5:	shl    $0x8,%r11d
+   14028efc9:	inc    %rdi
+   14028efcc:	or     %eax,%r10d
+   14028efcf:	movzwl 0x1c8(%rsi),%edx
+   14028efd6:	mov    %r11d,%eax
+   14028efd9:	shr    $0xb,%eax
+   14028efdc:	movzwl %dx,%ecx
+   14028efdf:	imul   %ecx,%eax
+   14028efe2:	cmp    %eax,%r10d
+   14028efe5:	jae    0x14028f004
+   14028efe7:	mov    %eax,%r11d
+   14028efea:	mov    $0x800,%eax
+   14028efef:	sub    %ecx,%eax
+   14028eff1:	sar    $0x5,%eax
+   14028eff4:	lea    (%rdx,%rax,1),%eax
+   14028eff7:	mov    %ax,0x1c8(%rsi)
+   14028effe:	mov    0x8(%rsp),%eax
+   14028f002:	jmp    0x14028f026
+   14028f004:	sub    %eax,%r11d
+   14028f007:	sub    %eax,%r10d
+   14028f00a:	mov    %edx,%eax
+   14028f00c:	shr    $0x5,%ax
+   14028f010:	sub    %ax,%dx
+   14028f013:	mov    0x4(%rsp),%eax
+   14028f017:	mov    %dx,0x1c8(%rsi)
+   14028f01e:	mov    0x8(%rsp),%edx
+   14028f022:	mov    %edx,0x4(%rsp)
+   14028f026:	mov    0xc(%rsp),%ecx
+   14028f02a:	mov    %ecx,0x8(%rsp)
+   14028f02e:	mov    %r14d,0xc(%rsp)
+   14028f033:	mov    %eax,%r14d
+   14028f036:	xor    %eax,%eax
+   14028f038:	cmpl   $0x6,0x10(%rsp)
+   14028f03d:	mov    0x20(%rsp),%r9
+   14028f042:	setg   %al
+   14028f045:	add    $0xa68,%r9
+   14028f04c:	lea    0x8(%rax,%rax,2),%eax
+   14028f050:	mov    %eax,0x10(%rsp)
+   14028f054:	cmp    $0xffffff,%r11d
+   14028f05b:	ja     0x14028f077
+   14028f05d:	cmp    %r12,%rdi
+   14028f060:	je     0x14028f400
+   14028f066:	movzbl (%rdi),%eax
+   14028f069:	shl    $0x8,%r10d
+   14028f06d:	shl    $0x8,%r11d
+   14028f071:	inc    %rdi
+   14028f074:	or     %eax,%r10d
+   14028f077:	movzwl (%r9),%edx
+   14028f07b:	mov    %r11d,%eax
+   14028f07e:	shr    $0xb,%eax
+   14028f081:	movzwl %dx,%ecx
+   14028f084:	imul   %ecx,%eax
+   14028f087:	cmp    %eax,%r10d
+   14028f08a:	jae    0x14028f0b2
+   14028f08c:	mov    %eax,%r11d
+   14028f08f:	mov    $0x800,%eax
+   14028f094:	xor    %r13d,%r13d
+   14028f097:	sub    %ecx,%eax
+   14028f099:	sar    $0x5,%eax
+   14028f09c:	lea    (%rdx,%rax,1),%eax
+   14028f09f:	mov    %ax,(%r9)
+   14028f0a3:	movslq (%rsp),%rax
+   14028f0a7:	shl    $0x4,%rax
+   14028f0ab:	lea    0x4(%r9,%rax,1),%r8
+   14028f0b0:	jmp    0x14028f129
+   14028f0b2:	sub    %eax,%r11d
+   14028f0b5:	sub    %eax,%r10d
+   14028f0b8:	mov    %edx,%eax
+   14028f0ba:	shr    $0x5,%ax
+   14028f0be:	sub    %ax,%dx
+   14028f0c1:	cmp    $0xffffff,%r11d
+   14028f0c8:	mov    %dx,(%r9)
+   14028f0cc:	ja     0x14028f0e8
+   14028f0ce:	cmp    %r12,%rdi
+   14028f0d1:	je     0x14028f400
+   14028f0d7:	movzbl (%rdi),%eax
+   14028f0da:	shl    $0x8,%r10d
+   14028f0de:	shl    $0x8,%r11d
+   14028f0e2:	inc    %rdi
+   14028f0e5:	or     %eax,%r10d
+   14028f0e8:	movzwl 0x2(%r9),%edx
+   14028f0ed:	mov    %r11d,%eax
+   14028f0f0:	shr    $0xb,%eax
+   14028f0f3:	movzwl %dx,%ecx
+   14028f0f6:	imul   %ecx,%eax
+   14028f0f9:	cmp    %eax,%r10d
+   14028f0fc:	jae    0x14028f131
+   14028f0fe:	mov    %eax,%r11d
+   14028f101:	mov    $0x800,%eax
+   14028f106:	mov    $0x8,%r13d
+   14028f10c:	sub    %ecx,%eax
+   14028f10e:	sar    $0x5,%eax
+   14028f111:	lea    (%rdx,%rax,1),%eax
+   14028f114:	mov    %ax,0x2(%r9)
+   14028f119:	movslq (%rsp),%rax
+   14028f11d:	shl    $0x4,%rax
+   14028f121:	lea    0x104(%r9,%rax,1),%r8
+   14028f129:	mov    $0x3,%r9d
+   14028f12f:	jmp    0x14028f158
+   14028f131:	sub    %eax,%r11d
+   14028f134:	sub    %eax,%r10d
+   14028f137:	mov    %edx,%eax
+   14028f139:	shr    $0x5,%ax
+   14028f13d:	lea    0x204(%r9),%r8
+   14028f144:	mov    $0x10,%r13d
+   14028f14a:	sub    %ax,%dx
+   14028f14d:	mov    %dx,0x2(%r9)
+   14028f152:	mov    $0x8,%r9d
+   14028f158:	mov    %r9d,%ebx
+   14028f15b:	mov    $0x1,%ebp
+   14028f160:	movslq %ebp,%rax
+   14028f163:	cmp    $0xffffff,%r11d
+   14028f16a:	lea    (%r8,%rax,2),%rsi
+   14028f16e:	ja     0x14028f18a
+   14028f170:	cmp    %r12,%rdi
+   14028f173:	je     0x14028f400
+   14028f179:	movzbl (%rdi),%eax
+   14028f17c:	shl    $0x8,%r10d
+   14028f180:	shl    $0x8,%r11d
+   14028f184:	inc    %rdi
+   14028f187:	or     %eax,%r10d
+   14028f18a:	movzwl (%rsi),%ecx
+   14028f18d:	mov    %r11d,%eax
+   14028f190:	shr    $0xb,%eax
+   14028f193:	movzwl %cx,%edx
+   14028f196:	imul   %edx,%eax
+   14028f199:	cmp    %eax,%r10d
+   14028f19c:	jae    0x14028f1b5
+   14028f19e:	mov    %eax,%r11d
+   14028f1a1:	mov    $0x800,%eax
+   14028f1a6:	add    %ebp,%ebp
+   14028f1a8:	sub    %edx,%eax
+   14028f1aa:	sar    $0x5,%eax
+   14028f1ad:	lea    (%rcx,%rax,1),%eax
+   14028f1b0:	mov    %ax,(%rsi)
+   14028f1b3:	jmp    0x14028f1cb
+   14028f1b5:	sub    %eax,%r11d
+   14028f1b8:	sub    %eax,%r10d
+   14028f1bb:	mov    %ecx,%eax
+   14028f1bd:	shr    $0x5,%ax
+   14028f1c1:	lea    0x1(%rbp,%rbp,1),%ebp
+   14028f1c5:	sub    %ax,%cx
+   14028f1c8:	mov    %cx,(%rsi)
+   14028f1cb:	dec    %ebx
+   14028f1cd:	jne    0x14028f160
+   14028f1cf:	mov    $0x1,%eax
+   14028f1d4:	mov    %r9d,%ecx
+   14028f1d7:	shl    %cl,%eax
+   14028f1d9:	sub    %eax,%ebp
+   14028f1db:	add    %r13d,%ebp
+   14028f1de:	cmpl   $0x3,0x10(%rsp)
+   14028f1e3:	jg     0x14028f3ab
+   14028f1e9:	addl   $0x7,0x10(%rsp)
+   14028f1ee:	mov    $0x3,%eax
+   14028f1f3:	cmp    $0x4,%ebp
+   14028f1f6:	cmovl  %ebp,%eax
+   14028f1f9:	mov    0x20(%rsp),%rbx
+   14028f1fe:	mov    $0x1,%r8d
+   14028f204:	cltq
+   14028f206:	shl    $0x7,%rax
+   14028f20a:	lea    0x360(%rbx,%rax,1),%r9
+   14028f212:	mov    $0x6,%ebx
+   14028f217:	movslq %r8d,%rax
+   14028f21a:	cmp    $0xffffff,%r11d
+   14028f221:	lea    (%r9,%rax,2),%rsi
+   14028f225:	ja     0x14028f241
+   14028f227:	cmp    %r12,%rdi
+   14028f22a:	je     0x14028f400
+   14028f230:	movzbl (%rdi),%eax
+   14028f233:	shl    $0x8,%r10d
+   14028f237:	shl    $0x8,%r11d
+   14028f23b:	inc    %rdi
+   14028f23e:	or     %eax,%r10d
+   14028f241:	movzwl (%rsi),%edx
+   14028f244:	mov    %r11d,%eax
+   14028f247:	shr    $0xb,%eax
+   14028f24a:	movzwl %dx,%ecx
+   14028f24d:	imul   %ecx,%eax
+   14028f250:	cmp    %eax,%r10d
+   14028f253:	jae    0x14028f26d
+   14028f255:	mov    %eax,%r11d
+   14028f258:	mov    $0x800,%eax
+   14028f25d:	add    %r8d,%r8d
+   14028f260:	sub    %ecx,%eax
+   14028f262:	sar    $0x5,%eax
+   14028f265:	lea    (%rdx,%rax,1),%eax
+   14028f268:	mov    %ax,(%rsi)
+   14028f26b:	jmp    0x14028f284
+   14028f26d:	sub    %eax,%r11d
+   14028f270:	sub    %eax,%r10d
+   14028f273:	mov    %edx,%eax
+   14028f275:	shr    $0x5,%ax
+   14028f279:	lea    0x1(%r8,%r8,1),%r8d
+   14028f27e:	sub    %ax,%dx
+   14028f281:	mov    %dx,(%rsi)
+   14028f284:	dec    %ebx
+   14028f286:	jne    0x14028f217
+   14028f288:	sub    $0x40,%r8d
+   14028f28c:	cmp    $0x3,%r8d
+   14028f290:	mov    %r8d,%r14d
+   14028f293:	jle    0x14028f3a6
+   14028f299:	and    $0x1,%r14d
+   14028f29d:	mov    %r8d,%eax
+   14028f2a0:	sar    %eax
+   14028f2a2:	or     $0x2,%r14d
+   14028f2a6:	cmp    $0xd,%r8d
+   14028f2aa:	lea    -0x1(%rax),%esi
+   14028f2ad:	jg     0x14028f2d2
+   14028f2af:	mov    %esi,%ecx
+   14028f2b1:	mov    0x20(%rsp),%rbx
+   14028f2b6:	movslq %r8d,%rax
+   14028f2b9:	shl    %cl,%r14d
+   14028f2bc:	add    %rax,%rax
+   14028f2bf:	mov    %r14d,%edx
+   14028f2c2:	lea    (%rbx,%rdx,2),%rdx
+   14028f2c6:	sub    %rax,%rdx
+   14028f2c9:	lea    0x55e(%rdx),%r9
+   14028f2d0:	jmp    0x14028f323
+   14028f2d2:	lea    -0x5(%rax),%esi
+   14028f2d5:	cmp    $0xffffff,%r11d
+   14028f2dc:	ja     0x14028f2f8
+   14028f2de:	cmp    %r12,%rdi
+   14028f2e1:	je     0x14028f400
+   14028f2e7:	movzbl (%rdi),%eax
+   14028f2ea:	shl    $0x8,%r10d
+   14028f2ee:	shl    $0x8,%r11d
+   14028f2f2:	inc    %rdi
+   14028f2f5:	or     %eax,%r10d
+   14028f2f8:	shr    %r11d
+   14028f2fb:	add    %r14d,%r14d
+   14028f2fe:	cmp    %r11d,%r10d
+   14028f301:	jb     0x14028f30a
+   14028f303:	sub    %r11d,%r10d
+   14028f306:	or     $0x1,%r14d
+   14028f30a:	dec    %esi
+   14028f30c:	jne    0x14028f2d5
+   14028f30e:	mov    0x20(%rsp),%r9
+   14028f313:	shl    $0x4,%r14d
+   14028f317:	mov    $0x4,%esi
+   14028f31c:	add    $0x644,%r9
+   14028f323:	mov    $0x1,%r13d
+   14028f329:	mov    $0x1,%ebx
+   14028f32e:	movslq %ebx,%rax
+   14028f331:	cmp    $0xffffff,%r11d
+   14028f338:	lea    (%r9,%rax,2),%r8
+   14028f33c:	ja     0x14028f358
+   14028f33e:	cmp    %r12,%rdi
+   14028f341:	je     0x14028f400
+   14028f347:	movzbl (%rdi),%eax
+   14028f34a:	shl    $0x8,%r10d
+   14028f34e:	shl    $0x8,%r11d
+   14028f352:	inc    %rdi
+   14028f355:	or     %eax,%r10d
+   14028f358:	movzwl (%r8),%edx
+   14028f35c:	mov    %r11d,%eax
+   14028f35f:	shr    $0xb,%eax
+   14028f362:	movzwl %dx,%ecx
+   14028f365:	imul   %ecx,%eax
+   14028f368:	cmp    %eax,%r10d
+   14028f36b:	jae    0x14028f385
+   14028f36d:	mov    %eax,%r11d
+   14028f370:	mov    $0x800,%eax
+   14028f375:	add    %ebx,%ebx
+   14028f377:	sub    %ecx,%eax
+   14028f379:	sar    $0x5,%eax
+   14028f37c:	lea    (%rdx,%rax,1),%eax
+   14028f37f:	mov    %ax,(%r8)
+   14028f383:	jmp    0x14028f39f
+   14028f385:	sub    %eax,%r11d
+   14028f388:	sub    %eax,%r10d
+   14028f38b:	mov    %edx,%eax
+   14028f38d:	shr    $0x5,%ax
+   14028f391:	lea    0x1(%rbx,%rbx,1),%ebx
+   14028f395:	or     %r13d,%r14d
+   14028f398:	sub    %ax,%dx
+   14028f39b:	mov    %dx,(%r8)
+   14028f39f:	add    %r13d,%r13d
+   14028f3a2:	dec    %esi
+   14028f3a4:	jne    0x14028f32e
+   14028f3a6:	inc    %r14d
+   14028f3a9:	je     0x14028f3eb
+   14028f3ab:	add    $0x2,%ebp
+   14028f3ae:	cmp    %r15d,%r14d
+   14028f3b1:	ja     0x14028f400
+   14028f3b3:	mov    0x30(%rsp),%rdx
+   14028f3b8:	mov    %r15d,%eax
+   14028f3bb:	sub    %r14d,%eax
+   14028f3be:	movzbl (%rdx,%rax,1),%r13d
+   14028f3c3:	mov    %r15d,%eax
+   14028f3c6:	inc    %r15d
+   14028f3c9:	dec    %ebp
+   14028f3cb:	mov    %r13b,(%rdx,%rax,1)
+   14028f3cf:	setne  %dl
+   14028f3d2:	xor    %eax,%eax
+   14028f3d4:	cmp    0x2c(%rsp),%r15d
+   14028f3d9:	setb   %al
+   14028f3dc:	test   %eax,%edx
+   14028f3de:	jne    0x14028f3b3
+   14028f3e0:	cmp    0x2c(%rsp),%r15d
+   14028f3e5:	jb     0x14028eb34
+   14028f3eb:	cmp    $0xffffff,%r11d
+   14028f3f2:	ja     0x14028f40a
+   14028f3f4:	cmp    %r12,%rdi
+   14028f3f7:	mov    $0x1,%eax
+   14028f3fc:	je     0x14028f424
+   14028f3fe:	jmp    0x14028f407
+   14028f400:	mov    $0x1,%eax
+   14028f405:	jmp    0x14028f424
+   14028f407:	inc    %rdi
+   14028f40a:	mov    %edi,%eax
+   14028f40c:	sub    0x40(%rsp),%eax
+   14028f410:	mov    0x38(%rsp),%rcx
+   14028f415:	mov    0x80(%rsp),%rbx
+   14028f41d:	mov    %eax,(%rcx)
+   14028f41f:	mov    %r15d,(%rbx)
+   14028f422:	xor    %eax,%eax
+   14028f424:	add    $0x48,%rsp
+   14028f428:	pop    %rbx
+   14028f429:	pop    %rbp
+   14028f42a:	pop    %r12
+   14028f42c:	pop    %r13
+   14028f42e:	pop    %r14
+   14028f430:	pop    %r15
+   14028f432:	leave
+   14028f433:	pop    %rax
+   14028f434:	pop    %rsi
+   14028f435:	pop    %rdi
+   14028f436:	pop    %rax
+   14028f437:	mov    %eax,(%rdi)
+   14028f439:	mov    %rsi,%rdi
+   14028f43c:	push   %rsi
+   14028f43d:	mov    %rsi,%rdi
+   14028f440:	mov    $0x1c2800,%rsi
+   14028f447:	mov    $0x1d,%dl
+   14028f449:	push   %rbx
+   14028f44a:	push   %rdi
+   14028f44b:	lea    -0x3(%rdi,%rsi,1),%rcx
+   14028f450:	pop    %rsi
+   14028f451:	push   %rsi
+   14028f452:	pop    %rbx
+   14028f453:	jmp    0x14028f484
+   14028f455:	cmp    %rcx,%rsi
+   14028f458:	jae    0x14028f48c
+   14028f45a:	push   %rsi
+   14028f45b:	pop    %rsi
+   14028f45c:	lods   %ds:(%rsi),%al
+   14028f45d:	cmp    $0x80,%al
+   14028f45f:	jb     0x14028f46b
+   14028f461:	cmp    $0x8f,%al
+   14028f463:	ja     0x14028f46b
+   14028f465:	cmpb   $0xf,-0x2(%rsi)
+   14028f469:	je     0x14028f471
+   14028f46b:	sub    $0xe8,%al
+   14028f46d:	cmp    $0x1,%al
+   14028f46f:	ja     0x14028f455
+   14028f471:	cmp    %rcx,%rsi
+   14028f474:	jae    0x14028f48c
+   14028f476:	push   %rsi
+   14028f477:	lods   %ds:(%rsi),%eax
+   14028f478:	sub    %dl,%al
+   14028f47a:	jne    0x14028f45b
+   14028f47c:	pop    %rdi
+   14028f47d:	bswap  %eax
+   14028f47f:	sub    %edi,%eax
+   14028f481:	add    %ebx,%eax
+   14028f483:	stos   %eax,%es:(%rdi)
+   14028f484:	cmp    %rcx,%rsi
+   14028f487:	jae    0x14028f48c
+   14028f489:	lods   %ds:(%rsi),%al
+   14028f48a:	jmp    0x14028f46b
+   14028f48c:	pop    %rbx
+   14028f48d:	pop    %rsi
+   14028f48e:	sub    $0x28,%rsp
+   14028f492:	lea    0x28b000(%rsi),%rdi
+   14028f499:	mov    (%rdi),%eax
+   14028f49b:	or     %eax,%eax
+   14028f49d:	je     0x14028f4e9
+   14028f49f:	mov    0x4(%rdi),%ebx
+   14028f4a2:	lea    0x28f000(%rax,%rsi,1),%rcx
+   14028f4aa:	add    %rsi,%rbx
+   14028f4ad:	add    $0x8,%rdi
+   14028f4b1:	call   *0xcf1(%rip)        # 0x1402901a8
+   14028f4b7:	xchg   %rax,%rbp
+   14028f4b9:	mov    (%rdi),%al
+   14028f4bb:	inc    %rdi
+   14028f4be:	or     %al,%al
+   14028f4c0:	je     0x14028f499
+   14028f4c2:	mov    %rdi,%rcx
+   14028f4c5:	mov    %rdi,%rdx
+   14028f4c8:	dec    %eax
+   14028f4ca:	repnz scas %es:(%rdi),%al
+   14028f4cc:	mov    %rbp,%rcx
+   14028f4cf:	call   *0xce3(%rip)        # 0x1402901b8
+   14028f4d5:	or     %rax,%rax
+   14028f4d8:	je     0x14028f4e3
+   14028f4da:	mov    %rax,(%rbx)
+   14028f4dd:	add    $0x8,%rbx
+   14028f4e1:	jmp    0x14028f4b9
+   14028f4e3:	jmp    *0xcc7(%rip)        # 0x1402901b0
+   14028f4e9:	add    $0x28,%rsp
+   14028f4ed:	add    $0x4,%rdi
+   14028f4f1:	lea    -0x4(%rsi),%rbx
+   14028f4f5:	xor    %eax,%eax
+   14028f4f7:	mov    (%rdi),%al
+   14028f4f9:	inc    %rdi
+   14028f4fc:	or     %eax,%eax
+   14028f4fe:	je     0x14028f52d
+   14028f500:	cmp    $0xef,%al
+   14028f502:	ja     0x14028f515
+   14028f504:	add    %rax,%rbx
+   14028f507:	mov    (%rbx),%rax
+   14028f50a:	bswap  %rax
+   14028f50d:	add    %rsi,%rax
+   14028f510:	mov    %rax,(%rbx)
+   14028f513:	jmp    0x14028f4f5
+   14028f515:	and    $0xf,%al
+   14028f517:	shl    $0x10,%eax
+   14028f51a:	mov    (%rdi),%ax
+   14028f51d:	add    $0x2,%rdi
+   14028f521:	or     %eax,%eax
+   14028f523:	jne    0x14028f504
+   14028f525:	mov    (%rdi),%eax
+   14028f527:	add    $0x4,%rdi
+   14028f52b:	jmp    0x14028f504
+   14028f52d:	mov    0xc8c(%rip),%rbp        # 0x1402901c0
+   14028f534:	lea    -0x1000(%rsi),%rdi
+   14028f53b:	mov    $0x1000,%ebx
+   14028f540:	push   %rax
+   14028f541:	mov    %rsp,%r9
+   14028f544:	mov    $0x4,%r8d
+   14028f54a:	mov    %rbx,%rdx
+   14028f54d:	mov    %rdi,%rcx
+   14028f550:	sub    $0x20,%rsp
+   14028f554:	call   *%rbp
+   14028f556:	lea    0x237(%rdi),%rax
+   14028f55d:	andb   $0x7f,(%rax)
+   14028f560:	andb   $0x7f,0x28(%rax)
+   14028f564:	lea    0x20(%rsp),%r9
+   14028f569:	mov    (%r9),%r8
+   14028f56c:	mov    %rbx,%rdx
+   14028f56f:	mov    %rdi,%rcx
+   14028f572:	call   *%rbp
+   14028f574:	add    $0x28,%rsp
+   14028f578:	movb   $0xfc,0x2d(%rip)        # 0x14028f5ac
+   14028f57f:	lea    -0x1000(%rsi),%rcx
+   14028f586:	push   $0x1
+   14028f588:	pop    %rdx
+   14028f589:	xor    %r8,%r8
+   14028f58c:	push   %rax
+   14028f58d:	call   0x14028f5ac
+   14028f592:	pop    %rax
+   14028f593:	pop    %rbp
+   14028f594:	pop    %rdi
+   14028f595:	pop    %rsi
+   14028f596:	pop    %rbx
+   14028f597:	lea    -0x80(%rsp),%rax
+   14028f59c:	push   $0x0
+   14028f59e:	cmp    %rax,%rsp
+   14028f5a1:	jne    0x14028f59c
+   14028f5a3:	sub    $0xffffffffffffff80,%rsp
+   14028f5a7:	jmp    0x1401b974c
+   14028f5ac:	ret
+   14028f5ad:	push   %rsi
+   14028f5ae:	lea    -0xcb0ad(%rip),%rsi        # 0x1401c4508
+   14028f5b5:	lods   %ds:(%rsi),%rax
+   14028f5b7:	test   %rax,%rax
+   14028f5ba:	je     0x14028f5d0
+   14028f5bc:	push   %rcx
+   14028f5bd:	push   %rdx
+   14028f5be:	push   %r8
+   14028f5c0:	sub    $0x28,%rsp
+   14028f5c4:	call   *%rax
+   14028f5c6:	add    $0x28,%rsp
+   14028f5ca:	pop    %r8
+   14028f5cc:	pop    %rdx
+   14028f5cd:	pop    %rcx
+   14028f5ce:	jmp    0x14028f5b5
+   14028f5d0:	pop    %rsi
+   14028f5d1:	ret
+   14028f5d2:	add    %al,(%rax)
+   14028f5d4:	add    %al,(%rax)
+   14028f5d6:	add    %al,(%rax)
+   14028f5d8:	add    %dh,%dh
+   14028f5da:	sub    %al,0x1(%rax)
+   14028f5dd:	add    %al,(%rax)
+   14028f5df:	add    %dl,0x14028f7(%rax)
+   14028f5e5:	add    %al,(%rax)
+   14028f5e7:	add    %dh,(%rax)
+   14028f5e9:	and    (%rdi),%esp
+   14028f5eb:	rex add %eax,(%rax)
+   14028f5ee:	add    %al,(%rax)
+   14028f5f0:	nop
+   14028f5f1:	imull  (%rax)
+   14028f5f3:	rex add %eax,(%rax)
 	...
-   14028f6bd:	add    %al,(%rax)
-   14028f6bf:	add    %cl,(%rax)
+   14028f5fe:	rex add %al,(%rax)
 	...
-   14028f77d:	add    %al,(%rax)
-   14028f77f:	add    %ah,0x14028f5(%rdx)
+   14028f6cd:	add    %al,(%rax)
+   14028f6cf:	add    %cl,(%rax)
 	...
    14028f78d:	add    %al,(%rax)
-   14028f78f:	add    %al,0x1(%rax)
+   14028f78f:	add    %ch,0x14028(%rbp,%rsi,8)
+	...
+   14028f79e:	add    %al,(%rax)
+   14028f7a0:	rex add %eax,(%rax)
 	...
-   14028f7e6:	add    %al,(%rax)
-   14028f7e8:	sbb    %ah,(%rcx)
-   14028f7ea:	(bad)
-   14028f7eb:	rex add %eax,(%rax)
+   14028f7f7:	add    %bl,(%rax)
+   14028f7f9:	and    %esp,(%rdi)
+   14028f7fb:	rex add %eax,(%rax)
 	...
-   14028f7fe:	add    %al,(%rax)
-   14028f800:	mov    %al,0x40(%rsp,%rbx,1)
-   14028f804:	add    %eax,(%rax)
-   14028f806:	add    %al,(%rax)
-   14028f808:	cwtl
-   14028f809:	rex.R sbb $0x40,%al
-   14028f80c:	add    %eax,(%rax)
+   14028f80e:	add    %al,(%rax)
+   14028f810:	mov    %al,0x40(%rsp,%rbx,1)
+   14028f814:	add    %eax,(%rax)
+   14028f816:	add    %al,(%rax)
+   14028f818:	cwtl
+   14028f819:	rex.R sbb $0x40,%al
+   14028f81c:	add    %eax,(%rax)
 	...
-   14028f81e:	add    %al,(%rax)
-   14028f820:	add    %al,(%rcx)
+   14028f82e:	add    %al,(%rax)
+   14028f830:	add    %al,(%rcx)
 	...
-   14028f88e:	add    %al,(%rax)
-   14028f890:	sbb    $0x93,%al
-   14028f892:	and    0x1(%rax),%al
+   14028f89e:	add    %al,(%rax)
+   14028f8a0:	sbb    $0x93,%al
+   14028f8a2:	and    0x1(%rax),%al
 	...
-   14028f8a5:	add    %al,(%rax)
-   14028f8a7:	add    %dl,0x1401c44(%rax)
-   14028f8ad:	add    %al,(%rax)
-   14028f8af:	add    %ah,0x1401c44(%rax)
    14028f8b5:	add    %al,(%rax)
-   14028f8b7:	add    %ch,0x1401c44(%rax)
+   14028f8b7:	add    %dl,0x1401c44(%rax)
    14028f8bd:	add    %al,(%rax)
-   14028f8bf:	add    %dh,0x1401c44(%rax)
+   14028f8bf:	add    %ah,0x1401c44(%rax)
    14028f8c5:	add    %al,(%rax)
-   14028f8c7:	add    %bh,0x1401c44(%rax)
+   14028f8c7:	add    %ch,0x1401c44(%rax)
+   14028f8cd:	add    %al,(%rax)
+   14028f8cf:	add    %dh,0x1401c44(%rax)
+   14028f8d5:	add    %al,(%rax)
+   14028f8d7:	add    %bh,0x1401c44(%rax)
 	...
 
 Disassembly of section UPX2:
 
 0000000140290000 <UPX2>:
 	...
    14029000c:	add    %al,(%rdx)
@@ -360513,31 +360531,19 @@
    1402903ec:	jb     0x140290453
    1402903ee:	movsxd 0x0(%rsi),%esi
    1402903f1:	add    %al,(%rax)
    1402903f3:	add    %al,(%rax)
    1402903f5:	lock sub %al,(%rax)
    1402903f8:	and    $0x0,%al
    1402903fa:	add    %al,(%rax)
-   1402903fc:	enter  $0xd0a5,$0xa5
-   140290400:	fsubs  -0x587f5a20(%rbp)
-   140290406:	call   0x148d104b2
-   14029040b:	test   $0x90,%al
-   14029040d:	test   $0xa8,%al
-   14029040f:	test   $0xb0,%al
-   140290411:	test   $0xb8,%al
-   140290413:	test   $0xc0,%al
-   140290415:	test   $0xc8,%al
+   1402903fc:	fsubs  -0x5a175a20(%rbp)
+   140290402:	lock movsl %ds:(%rsi),%es:(%rdi)
+   140290404:	nop
+   140290405:	cmpsl  %es:(%rdi),%ds:(%rsi)
+   140290406:	clc
+   140290407:	cmpsl  %es:(%rdi),%ds:(%rsi)
+   140290408:	adc    %ch,-0x575f57e8(%rax)
+   14029040e:	mov    $0xc8a8c0a8,%eax
+   140290413:	test   $0xd0,%al
+   140290415:	test   $0xd8,%al
    140290417:	test   $0x0,%al
-   140290419:	lock sub %al,(%rax)
-   14029041c:	and    $0x0,%al
-   14029041e:	add    %al,(%rax)
-   140290420:	enter  $0xd0a5,$0xa5
-   140290424:	fsubs  -0x587f5a20(%rbp)
-   14029042a:	call   0x148d104d6
-   14029042f:	test   $0x90,%al
-   140290431:	test   $0xa8,%al
-   140290433:	test   $0xb0,%al
-   140290435:	test   $0xb8,%al
-   140290437:	test   $0xc0,%al
-   140290439:	test   $0xc8,%al
-   14029043b:	test   $0x0,%al
 	...
```

