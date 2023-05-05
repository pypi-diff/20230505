# Comparing `tmp/repairwheel-0.2.3.tar.gz` & `tmp/repairwheel-0.2.4.tar.gz`

## Comparing `repairwheel-0.2.3.tar` & `repairwheel-0.2.4.tar`

### file list

```diff
@@ -1,114 +1,114 @@
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 repairwheel-0.2.3/CHANGELOG.rst
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 repairwheel-0.2.3/codecov.yml
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/__init__.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/__main__.py
--rw-r--r--   0        0        0     2088 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/compat.py
--rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/fileutil.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/py.typed
--rw-r--r--   0        0        0     3433 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/repair.py
--rw-r--r--   0        0        0     5059 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/wheel.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/_vendor/__init__.py
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/_vendor/auditwheel.pyi
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/_vendor/vendor.txt
--rw-r--r--   0        0        0     4774 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/_vendor/auditwheel/LICENSE
--rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/_vendor/auditwheel/LICENSE.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/_vendor/auditwheel/__init__.py
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/_vendor/auditwheel/__main__.py
--rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/_vendor/auditwheel/condatools.py
--rw-r--r--   0        0        0     4958 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/_vendor/auditwheel/elfutils.py
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/_vendor/auditwheel/error.py
--rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/_vendor/auditwheel/genericpkgctx.py
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/_vendor/auditwheel/hashfile.py
--rw-r--r--   0        0        0    14346 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/_vendor/auditwheel/lddtree.py
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/_vendor/auditwheel/libc.py
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/_vendor/auditwheel/main.py
--rw-r--r--   0        0        0     2051 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/_vendor/auditwheel/main_addtag.py
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/_vendor/auditwheel/main_lddtree.py
--rw-r--r--   0        0        0     5919 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/_vendor/auditwheel/main_repair.py
--rw-r--r--   0        0        0     4414 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/_vendor/auditwheel/main_show.py
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/_vendor/auditwheel/musllinux.py
--rw-r--r--   0        0        0     2357 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/_vendor/auditwheel/patcher.py
--rw-r--r--   0        0        0     8009 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/_vendor/auditwheel/repair.py
--rw-r--r--   0        0        0     3000 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/_vendor/auditwheel/tmpdirs.py
--rw-r--r--   0        0        0     4512 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/_vendor/auditwheel/tools.py
--rw-r--r--   0        0        0    10995 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/_vendor/auditwheel/wheel_abi.py
--rw-r--r--   0        0        0     9516 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/_vendor/auditwheel/wheeltools.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/_vendor/auditwheel/_vendor/__init__.py
--rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/_vendor/auditwheel/_vendor/wheel/LICENSE.txt
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/_vendor/auditwheel/_vendor/wheel/__init__.py
--rw-r--r--   0        0        0     1257 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/_vendor/auditwheel/_vendor/wheel/pkginfo.py
--rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/_vendor/auditwheel/_vendor/wheel/util.py
--rw-r--r--   0        0        0     7326 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/_vendor/auditwheel/_vendor/wheel/wheelfile.py
--rw-r--r--   0        0        0     2572 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/_vendor/auditwheel/_vendor/wheel/cli/__init__.py
--rw-r--r--   0        0        0     9498 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/_vendor/auditwheel/_vendor/wheel/cli/convert.py
--rw-r--r--   0        0        0     3196 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/_vendor/auditwheel/_vendor/wheel/cli/pack.py
--rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/_vendor/auditwheel/_vendor/wheel/cli/unpack.py
--rw-r--r--   0        0        0     6348 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/_vendor/auditwheel/policy/__init__.py
--rw-r--r--   0        0        0     3147 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/_vendor/auditwheel/policy/external_references.py
--rw-r--r--   0        0        0    53261 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/_vendor/auditwheel/policy/manylinux-policy.json
--rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/_vendor/auditwheel/policy/musllinux-policy.json
--rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/_vendor/auditwheel/policy/policy-schema.json
--rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/_vendor/auditwheel/policy/versioned_symbols.py
--rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/_vendor/delocate/LICENSE
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/_vendor/delocate/__init__.py
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/_vendor/delocate/_version.py
--rw-r--r--   0        0        0    33312 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/_vendor/delocate/delocating.py
--rw-r--r--   0        0        0     3819 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/_vendor/delocate/fuse.py
--rw-r--r--   0        0        0    27193 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/_vendor/delocate/libsana.py
--rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/_vendor/delocate/pkginfo.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/_vendor/delocate/py.typed
--rw-r--r--   0        0        0     3961 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/_vendor/delocate/tmpdirs.py
--rw-r--r--   0        0        0    30694 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/_vendor/delocate/tools.py
--rw-r--r--   0        0        0     8296 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/_vendor/delocate/wheeltools.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/_vendor/delocate/cmd/__init__.py
--rw-r--r--   0        0        0     4790 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/_vendor/delocate/cmd/delocate_addplat.py
--rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/_vendor/delocate/cmd/delocate_fuse.py
--rw-r--r--   0        0        0     2069 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/_vendor/delocate/cmd/delocate_listdeps.py
--rw-r--r--   0        0        0     1685 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/_vendor/delocate/cmd/delocate_patch.py
--rw-r--r--   0        0        0     2196 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/_vendor/delocate/cmd/delocate_path.py
--rw-r--r--   0        0        0     4544 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/_vendor/delocate/cmd/delocate_wheel.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/linux/__init__.py
--rw-r--r--   0        0        0    39046 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/linux/elffile.py
--rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/linux/monkeypatch.py
--rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/linux/patcher.py
--rw-r--r--   0        0        0     2070 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/linux/repair.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/macos/__init__.py
--rw-r--r--   0        0        0    18881 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/macos/machosign.py
--rw-r--r--   0        0        0    11633 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/macos/machotools.py
--rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/macos/repair.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/windows/__init__.py
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 repairwheel-0.2.3/src/repairwheel/windows/repair.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 repairwheel-0.2.3/tests/__init__.py
--rw-r--r--   0        0        0     3084 2020-02-02 00:00:00.000000 repairwheel-0.2.3/tests/conftest.py
--rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 repairwheel-0.2.3/tests/test_common.py
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 repairwheel-0.2.3/tests/test_windows.py
--rw-r--r--   0        0        0     2931 2020-02-02 00:00:00.000000 repairwheel-0.2.3/tests/util.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 repairwheel-0.2.3/tests/gen_check/__init__.py
--rw-r--r--   0        0        0     1406 2020-02-02 00:00:00.000000 repairwheel-0.2.3/tests/gen_check/test_check.py
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 repairwheel-0.2.3/tests/gen_check/test_generate.py
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 repairwheel-0.2.3/tests/testwheel/build-native/README.md
--rwxr-xr-x   0        0        0     7756 2020-02-02 00:00:00.000000 repairwheel-0.2.3/tests/testwheel/build-native/build.py
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 repairwheel-0.2.3/tests/testwheel/build-native/testwheel.c
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 repairwheel-0.2.3/tests/testwheel/build-native/testdep/testdep.c
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 repairwheel-0.2.3/tests/testwheel/build-native/testdep/testdep.h
--rwxr-xr-x   0        0        0       97 2020-02-02 00:00:00.000000 repairwheel-0.2.3/tests/testwheel/build-python/build.sh
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 repairwheel-0.2.3/tests/testwheel/build-python/pyproject.toml
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 repairwheel-0.2.3/tests/testwheel/build-python/testwheel/__init__.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 repairwheel-0.2.3/tests/testwheel/build-python/testwheel/testwheel.py
--rw-r--r--   0        0        0     5902 2020-02-02 00:00:00.000000 repairwheel-0.2.3/tests/testwheel/cp36-abi3-linux_x86_64/testwheel-0.0.1-cp36-abi3-linux_x86_64.whl
--rw-r--r--   0        0        0     2992 2020-02-02 00:00:00.000000 repairwheel-0.2.3/tests/testwheel/cp36-abi3-linux_x86_64/lib/libtestdep.so
--rw-r--r--   0        0        0     2578 2020-02-02 00:00:00.000000 repairwheel-0.2.3/tests/testwheel/cp36-abi3-macosx_10_11_arm64/testwheel-0.0.1-cp36-abi3-macosx_10_11_arm64.whl
--rw-r--r--   0        0        0    16944 2020-02-02 00:00:00.000000 repairwheel-0.2.3/tests/testwheel/cp36-abi3-macosx_10_11_arm64/lib/libtestdep.dylib
--rw-r--r--   0        0        0     2265 2020-02-02 00:00:00.000000 repairwheel-0.2.3/tests/testwheel/cp36-abi3-macosx_10_11_x86_64/testwheel-0.0.1-cp36-abi3-macosx_10_11_x86_64.whl
--rw-r--r--   0        0        0     4454 2020-02-02 00:00:00.000000 repairwheel-0.2.3/tests/testwheel/cp36-abi3-macosx_10_11_x86_64/lib/libtestdep.dylib
--rw-r--r--   0        0        0    64683 2020-02-02 00:00:00.000000 repairwheel-0.2.3/tests/testwheel/cp36-abi3-win_amd64/testwheel-0.0.1-cp36-abi3-win_amd64.whl
--rw-r--r--   0        0        0   135168 2020-02-02 00:00:00.000000 repairwheel-0.2.3/tests/testwheel/cp36-abi3-win_amd64/lib/testdep.dll
--rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 repairwheel-0.2.3/tests/testwheel/py3-none-any/testwheel-0.0.1-py3-none-any.whl
--rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 repairwheel-0.2.3/tools/vendoring/patches/auditwheel.patch
--rw-r--r--   0        0        0      929 2020-02-02 00:00:00.000000 repairwheel-0.2.3/tools/vendoring/patches/delocate.chmod.patch
--rw-r--r--   0        0        0     7453 2020-02-02 00:00:00.000000 repairwheel-0.2.3/tools/vendoring/patches/delocate.patch
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 repairwheel-0.2.3/.gitignore
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 repairwheel-0.2.3/LICENSE
--rw-r--r--   0        0        0     2144 2020-02-02 00:00:00.000000 repairwheel-0.2.3/README.md
--rw-r--r--   0        0        0     2474 2020-02-02 00:00:00.000000 repairwheel-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     4398 2020-02-02 00:00:00.000000 repairwheel-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 repairwheel-0.2.4/CHANGELOG.rst
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 repairwheel-0.2.4/codecov.yml
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 repairwheel-0.2.4/src/repairwheel/__init__.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 repairwheel-0.2.4/src/repairwheel/__main__.py
+-rw-r--r--   0        0        0     2088 2020-02-02 00:00:00.000000 repairwheel-0.2.4/src/repairwheel/compat.py
+-rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 repairwheel-0.2.4/src/repairwheel/fileutil.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 repairwheel-0.2.4/src/repairwheel/py.typed
+-rw-r--r--   0        0        0     3433 2020-02-02 00:00:00.000000 repairwheel-0.2.4/src/repairwheel/repair.py
+-rw-r--r--   0        0        0     5059 2020-02-02 00:00:00.000000 repairwheel-0.2.4/src/repairwheel/wheel.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 repairwheel-0.2.4/src/repairwheel/_vendor/__init__.py
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 repairwheel-0.2.4/src/repairwheel/_vendor/auditwheel.pyi
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 repairwheel-0.2.4/src/repairwheel/_vendor/vendor.txt
+-rw-r--r--   0        0        0     4774 2020-02-02 00:00:00.000000 repairwheel-0.2.4/src/repairwheel/_vendor/auditwheel/LICENSE
+-rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 repairwheel-0.2.4/src/repairwheel/_vendor/auditwheel/LICENSE.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 repairwheel-0.2.4/src/repairwheel/_vendor/auditwheel/__init__.py
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 repairwheel-0.2.4/src/repairwheel/_vendor/auditwheel/__main__.py
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 repairwheel-0.2.4/src/repairwheel/_vendor/auditwheel/condatools.py
+-rw-r--r--   0        0        0     4947 2020-02-02 00:00:00.000000 repairwheel-0.2.4/src/repairwheel/_vendor/auditwheel/elfutils.py
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 repairwheel-0.2.4/src/repairwheel/_vendor/auditwheel/error.py
+-rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 repairwheel-0.2.4/src/repairwheel/_vendor/auditwheel/genericpkgctx.py
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 repairwheel-0.2.4/src/repairwheel/_vendor/auditwheel/hashfile.py
+-rw-r--r--   0        0        0    14266 2020-02-02 00:00:00.000000 repairwheel-0.2.4/src/repairwheel/_vendor/auditwheel/lddtree.py
+-rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 repairwheel-0.2.4/src/repairwheel/_vendor/auditwheel/libc.py
+-rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 repairwheel-0.2.4/src/repairwheel/_vendor/auditwheel/main.py
+-rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 repairwheel-0.2.4/src/repairwheel/_vendor/auditwheel/main_addtag.py
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 repairwheel-0.2.4/src/repairwheel/_vendor/auditwheel/main_lddtree.py
+-rw-r--r--   0        0        0     5955 2020-02-02 00:00:00.000000 repairwheel-0.2.4/src/repairwheel/_vendor/auditwheel/main_repair.py
+-rw-r--r--   0        0        0     4450 2020-02-02 00:00:00.000000 repairwheel-0.2.4/src/repairwheel/_vendor/auditwheel/main_show.py
+-rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 repairwheel-0.2.4/src/repairwheel/_vendor/auditwheel/musllinux.py
+-rw-r--r--   0        0        0     2366 2020-02-02 00:00:00.000000 repairwheel-0.2.4/src/repairwheel/_vendor/auditwheel/patcher.py
+-rw-r--r--   0        0        0     7987 2020-02-02 00:00:00.000000 repairwheel-0.2.4/src/repairwheel/_vendor/auditwheel/repair.py
+-rw-r--r--   0        0        0     2981 2020-02-02 00:00:00.000000 repairwheel-0.2.4/src/repairwheel/_vendor/auditwheel/tmpdirs.py
+-rw-r--r--   0        0        0     4529 2020-02-02 00:00:00.000000 repairwheel-0.2.4/src/repairwheel/_vendor/auditwheel/tools.py
+-rw-r--r--   0        0        0    10994 2020-02-02 00:00:00.000000 repairwheel-0.2.4/src/repairwheel/_vendor/auditwheel/wheel_abi.py
+-rw-r--r--   0        0        0     9515 2020-02-02 00:00:00.000000 repairwheel-0.2.4/src/repairwheel/_vendor/auditwheel/wheeltools.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 repairwheel-0.2.4/src/repairwheel/_vendor/auditwheel/_vendor/__init__.py
+-rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 repairwheel-0.2.4/src/repairwheel/_vendor/auditwheel/_vendor/wheel/LICENSE.txt
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 repairwheel-0.2.4/src/repairwheel/_vendor/auditwheel/_vendor/wheel/__init__.py
+-rw-r--r--   0        0        0     1257 2020-02-02 00:00:00.000000 repairwheel-0.2.4/src/repairwheel/_vendor/auditwheel/_vendor/wheel/pkginfo.py
+-rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 repairwheel-0.2.4/src/repairwheel/_vendor/auditwheel/_vendor/wheel/util.py
+-rw-r--r--   0        0        0     7326 2020-02-02 00:00:00.000000 repairwheel-0.2.4/src/repairwheel/_vendor/auditwheel/_vendor/wheel/wheelfile.py
+-rw-r--r--   0        0        0     2572 2020-02-02 00:00:00.000000 repairwheel-0.2.4/src/repairwheel/_vendor/auditwheel/_vendor/wheel/cli/__init__.py
+-rw-r--r--   0        0        0     9498 2020-02-02 00:00:00.000000 repairwheel-0.2.4/src/repairwheel/_vendor/auditwheel/_vendor/wheel/cli/convert.py
+-rw-r--r--   0        0        0     3196 2020-02-02 00:00:00.000000 repairwheel-0.2.4/src/repairwheel/_vendor/auditwheel/_vendor/wheel/cli/pack.py
+-rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 repairwheel-0.2.4/src/repairwheel/_vendor/auditwheel/_vendor/wheel/cli/unpack.py
+-rw-r--r--   0        0        0     6559 2020-02-02 00:00:00.000000 repairwheel-0.2.4/src/repairwheel/_vendor/auditwheel/policy/__init__.py
+-rw-r--r--   0        0        0     3158 2020-02-02 00:00:00.000000 repairwheel-0.2.4/src/repairwheel/_vendor/auditwheel/policy/external_references.py
+-rw-r--r--   0        0        0    53261 2020-02-02 00:00:00.000000 repairwheel-0.2.4/src/repairwheel/_vendor/auditwheel/policy/manylinux-policy.json
+-rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 repairwheel-0.2.4/src/repairwheel/_vendor/auditwheel/policy/musllinux-policy.json
+-rw-r--r--   0        0        0     1706 2020-02-02 00:00:00.000000 repairwheel-0.2.4/src/repairwheel/_vendor/auditwheel/policy/policy-schema.json
+-rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 repairwheel-0.2.4/src/repairwheel/_vendor/auditwheel/policy/versioned_symbols.py
+-rw-r--r--   0        0        0     1306 2020-02-02 00:00:00.000000 repairwheel-0.2.4/src/repairwheel/_vendor/delocate/LICENSE
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 repairwheel-0.2.4/src/repairwheel/_vendor/delocate/__init__.py
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 repairwheel-0.2.4/src/repairwheel/_vendor/delocate/_version.py
+-rw-r--r--   0        0        0    33312 2020-02-02 00:00:00.000000 repairwheel-0.2.4/src/repairwheel/_vendor/delocate/delocating.py
+-rw-r--r--   0        0        0     3819 2020-02-02 00:00:00.000000 repairwheel-0.2.4/src/repairwheel/_vendor/delocate/fuse.py
+-rw-r--r--   0        0        0    27193 2020-02-02 00:00:00.000000 repairwheel-0.2.4/src/repairwheel/_vendor/delocate/libsana.py
+-rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 repairwheel-0.2.4/src/repairwheel/_vendor/delocate/pkginfo.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 repairwheel-0.2.4/src/repairwheel/_vendor/delocate/py.typed
+-rw-r--r--   0        0        0     3961 2020-02-02 00:00:00.000000 repairwheel-0.2.4/src/repairwheel/_vendor/delocate/tmpdirs.py
+-rw-r--r--   0        0        0    30694 2020-02-02 00:00:00.000000 repairwheel-0.2.4/src/repairwheel/_vendor/delocate/tools.py
+-rw-r--r--   0        0        0     8296 2020-02-02 00:00:00.000000 repairwheel-0.2.4/src/repairwheel/_vendor/delocate/wheeltools.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 repairwheel-0.2.4/src/repairwheel/_vendor/delocate/cmd/__init__.py
+-rw-r--r--   0        0        0     4790 2020-02-02 00:00:00.000000 repairwheel-0.2.4/src/repairwheel/_vendor/delocate/cmd/delocate_addplat.py
+-rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 repairwheel-0.2.4/src/repairwheel/_vendor/delocate/cmd/delocate_fuse.py
+-rw-r--r--   0        0        0     2069 2020-02-02 00:00:00.000000 repairwheel-0.2.4/src/repairwheel/_vendor/delocate/cmd/delocate_listdeps.py
+-rw-r--r--   0        0        0     1685 2020-02-02 00:00:00.000000 repairwheel-0.2.4/src/repairwheel/_vendor/delocate/cmd/delocate_patch.py
+-rw-r--r--   0        0        0     2196 2020-02-02 00:00:00.000000 repairwheel-0.2.4/src/repairwheel/_vendor/delocate/cmd/delocate_path.py
+-rw-r--r--   0        0        0     4544 2020-02-02 00:00:00.000000 repairwheel-0.2.4/src/repairwheel/_vendor/delocate/cmd/delocate_wheel.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 repairwheel-0.2.4/src/repairwheel/linux/__init__.py
+-rw-r--r--   0        0        0    39046 2020-02-02 00:00:00.000000 repairwheel-0.2.4/src/repairwheel/linux/elffile.py
+-rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 repairwheel-0.2.4/src/repairwheel/linux/monkeypatch.py
+-rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 repairwheel-0.2.4/src/repairwheel/linux/patcher.py
+-rw-r--r--   0        0        0     2070 2020-02-02 00:00:00.000000 repairwheel-0.2.4/src/repairwheel/linux/repair.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 repairwheel-0.2.4/src/repairwheel/macos/__init__.py
+-rw-r--r--   0        0        0    18881 2020-02-02 00:00:00.000000 repairwheel-0.2.4/src/repairwheel/macos/machosign.py
+-rw-r--r--   0        0        0    11633 2020-02-02 00:00:00.000000 repairwheel-0.2.4/src/repairwheel/macos/machotools.py
+-rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 repairwheel-0.2.4/src/repairwheel/macos/repair.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 repairwheel-0.2.4/src/repairwheel/windows/__init__.py
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 repairwheel-0.2.4/src/repairwheel/windows/repair.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 repairwheel-0.2.4/tests/__init__.py
+-rw-r--r--   0        0        0     3084 2020-02-02 00:00:00.000000 repairwheel-0.2.4/tests/conftest.py
+-rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 repairwheel-0.2.4/tests/test_common.py
+-rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 repairwheel-0.2.4/tests/test_windows.py
+-rw-r--r--   0        0        0     2931 2020-02-02 00:00:00.000000 repairwheel-0.2.4/tests/util.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 repairwheel-0.2.4/tests/gen_check/__init__.py
+-rw-r--r--   0        0        0     1406 2020-02-02 00:00:00.000000 repairwheel-0.2.4/tests/gen_check/test_check.py
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 repairwheel-0.2.4/tests/gen_check/test_generate.py
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 repairwheel-0.2.4/tests/testwheel/build-native/README.md
+-rwxr-xr-x   0        0        0     7756 2020-02-02 00:00:00.000000 repairwheel-0.2.4/tests/testwheel/build-native/build.py
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 repairwheel-0.2.4/tests/testwheel/build-native/testwheel.c
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 repairwheel-0.2.4/tests/testwheel/build-native/testdep/testdep.c
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 repairwheel-0.2.4/tests/testwheel/build-native/testdep/testdep.h
+-rwxr-xr-x   0        0        0       97 2020-02-02 00:00:00.000000 repairwheel-0.2.4/tests/testwheel/build-python/build.sh
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 repairwheel-0.2.4/tests/testwheel/build-python/pyproject.toml
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 repairwheel-0.2.4/tests/testwheel/build-python/testwheel/__init__.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 repairwheel-0.2.4/tests/testwheel/build-python/testwheel/testwheel.py
+-rw-r--r--   0        0        0     5902 2020-02-02 00:00:00.000000 repairwheel-0.2.4/tests/testwheel/cp36-abi3-linux_x86_64/testwheel-0.0.1-cp36-abi3-linux_x86_64.whl
+-rw-r--r--   0        0        0     2992 2020-02-02 00:00:00.000000 repairwheel-0.2.4/tests/testwheel/cp36-abi3-linux_x86_64/lib/libtestdep.so
+-rw-r--r--   0        0        0     2578 2020-02-02 00:00:00.000000 repairwheel-0.2.4/tests/testwheel/cp36-abi3-macosx_10_11_arm64/testwheel-0.0.1-cp36-abi3-macosx_10_11_arm64.whl
+-rw-r--r--   0        0        0    16944 2020-02-02 00:00:00.000000 repairwheel-0.2.4/tests/testwheel/cp36-abi3-macosx_10_11_arm64/lib/libtestdep.dylib
+-rw-r--r--   0        0        0     2265 2020-02-02 00:00:00.000000 repairwheel-0.2.4/tests/testwheel/cp36-abi3-macosx_10_11_x86_64/testwheel-0.0.1-cp36-abi3-macosx_10_11_x86_64.whl
+-rw-r--r--   0        0        0     4454 2020-02-02 00:00:00.000000 repairwheel-0.2.4/tests/testwheel/cp36-abi3-macosx_10_11_x86_64/lib/libtestdep.dylib
+-rw-r--r--   0        0        0    64683 2020-02-02 00:00:00.000000 repairwheel-0.2.4/tests/testwheel/cp36-abi3-win_amd64/testwheel-0.0.1-cp36-abi3-win_amd64.whl
+-rw-r--r--   0        0        0   135168 2020-02-02 00:00:00.000000 repairwheel-0.2.4/tests/testwheel/cp36-abi3-win_amd64/lib/testdep.dll
+-rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 repairwheel-0.2.4/tests/testwheel/py3-none-any/testwheel-0.0.1-py3-none-any.whl
+-rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 repairwheel-0.2.4/tools/vendoring/patches/auditwheel.patch
+-rw-r--r--   0        0        0      929 2020-02-02 00:00:00.000000 repairwheel-0.2.4/tools/vendoring/patches/delocate.chmod.patch
+-rw-r--r--   0        0        0     7453 2020-02-02 00:00:00.000000 repairwheel-0.2.4/tools/vendoring/patches/delocate.patch
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 repairwheel-0.2.4/.gitignore
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 repairwheel-0.2.4/LICENSE
+-rw-r--r--   0        0        0     2144 2020-02-02 00:00:00.000000 repairwheel-0.2.4/README.md
+-rw-r--r--   0        0        0     2474 2020-02-02 00:00:00.000000 repairwheel-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0     4398 2020-02-02 00:00:00.000000 repairwheel-0.2.4/PKG-INFO
```

### Comparing `repairwheel-0.2.3/src/repairwheel/compat.py` & `repairwheel-0.2.4/src/repairwheel/compat.py`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.3/src/repairwheel/fileutil.py` & `repairwheel-0.2.4/src/repairwheel/fileutil.py`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.3/src/repairwheel/repair.py` & `repairwheel-0.2.4/src/repairwheel/repair.py`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.3/src/repairwheel/wheel.py` & `repairwheel-0.2.4/src/repairwheel/wheel.py`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.3/src/repairwheel/_vendor/auditwheel/LICENSE` & `repairwheel-0.2.4/src/repairwheel/_vendor/auditwheel/LICENSE`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.3/src/repairwheel/_vendor/auditwheel/LICENSE.txt` & `repairwheel-0.2.4/src/repairwheel/_vendor/auditwheel/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.3/src/repairwheel/_vendor/auditwheel/condatools.py` & `repairwheel-0.2.4/src/repairwheel/_vendor/auditwheel/condatools.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Context managers like those in wheeltools.py for unpacking
 conda packages.
 """
+from __future__ import annotations
+
 import os
-from typing import List, Optional
 
 from .tmpdirs import InTemporaryDirectory
 from .tools import tarbz2todir
 
 
 class InCondaPkg(InTemporaryDirectory):
     def __init__(self, in_conda_pkg: str) -> None:
@@ -18,19 +19,19 @@
         tarbz2todir(self.in_conda_pkg, self.name)
         return super().__enter__()
 
 
 class InCondaPkgCtx(InCondaPkg):
     def __init__(self, in_conda_pkg: str) -> None:
         super().__init__(in_conda_pkg)
-        self.path: Optional[str] = None
+        self.path: str | None = None
 
     def __enter__(self):
         self.path = super().__enter__()
         return self
 
-    def iter_files(self) -> List[str]:
+    def iter_files(self) -> list[str]:
         if self.path is None:
             raise ValueError("This function should be called from context manager")
         files = os.path.join(self.path, "info", "files")
         with open(files) as f:
             return [line.strip() for line in f.readlines()]
```

### Comparing `repairwheel-0.2.3/src/repairwheel/_vendor/auditwheel/elfutils.py` & `repairwheel-0.2.4/src/repairwheel/_vendor/auditwheel/elfutils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,35 @@
+from __future__ import annotations
+
 from os.path import basename
 from pathlib import Path
-from typing import Dict, Iterator, List, Optional, Set, Tuple
+from typing import Iterator
 
 from elftools.common.exceptions import ELFError
 from elftools.elf.elffile import ELFFile
 
 from .lddtree import parse_ld_paths
 
 
-def elf_read_dt_needed(fn: str) -> List[str]:
+def elf_read_dt_needed(fn: str) -> list[str]:
     needed = []
     with open(fn, "rb") as f:
         elf = ELFFile(f)
         section = elf.get_section_by_name(".dynamic")
         if section is None:
             raise ValueError("Could not find soname in %s" % fn)
 
         for t in section.iter_tags():
             if t.entry.d_tag == "DT_NEEDED":
                 needed.append(t.needed)
 
     return needed
 
 
-def elf_file_filter(paths: Iterator[str]) -> Iterator[Tuple[str, ELFFile]]:
+def elf_file_filter(paths: Iterator[str]) -> Iterator[tuple[str, ELFFile]]:
     """Filter through an iterator of filenames and load up only ELF
     files
     """
 
     for path in paths:
         if path.endswith(".py"):
             continue
@@ -37,15 +39,15 @@
                     candidate = ELFFile(f)
                     yield path, candidate
             except ELFError:
                 # not an elf file
                 continue
 
 
-def elf_find_versioned_symbols(elf: ELFFile) -> Iterator[Tuple[str, str]]:
+def elf_find_versioned_symbols(elf: ELFFile) -> Iterator[tuple[str, str]]:
     section = elf.get_section_by_name(".gnu.version_r")
 
     if section is not None:
         for verneed, verneed_iter in section.iter_versions():
             if verneed.name.startswith("ld-linux") or verneed.name in [
                 "ld64.so.2",
                 "ld64.so.1",
@@ -61,15 +63,14 @@
         # look for UCS2 symbols that are externally referenced
         for sym in section.iter_symbols():
             if (
                 "PyUnicodeUCS2_" in sym.name
                 and sym["st_shndx"] == "SHN_UNDEF"
                 and sym["st_info"]["type"] == "STT_FUNC"
             ):
-
                 yield sym.name
 
 
 def elf_references_PyFPE_jbuf(elf: ELFFile) -> bool:
     offending_symbol_names = ("PyFPE_jbuf", "PyFPE_dummy", "PyFPE_counter")
     section = elf.get_section_by_name(".dynsym")
     if section is not None:
@@ -80,15 +81,15 @@
                 and sym["st_shndx"] == "SHN_UNDEF"
                 and sym["st_info"]["type"] in ("STT_FUNC", "STT_NOTYPE")
             ):
                 return True
     return False
 
 
-def elf_is_python_extension(fn: str, elf: ELFFile) -> Tuple[bool, Optional[int]]:
+def elf_is_python_extension(fn: str, elf: ELFFile) -> tuple[bool, int | None]:
     modname = basename(fn).split(".", 1)[0]
     module_init_f = {
         "init" + modname: 2,
         "PyInit_" + modname: 3,
         "_cffi_pypyinit_" + modname: 2,
     }
 
@@ -98,22 +99,21 @@
 
     for sym in sect.iter_symbols():
         if (
             sym.name in module_init_f
             and sym["st_shndx"] != "SHN_UNDEF"
             and sym["st_info"]["type"] == "STT_FUNC"
         ):
-
             return True, module_init_f[sym.name]
 
     return False, None
 
 
-def elf_read_rpaths(fn: str) -> Dict[str, List[str]]:
-    result = {"rpaths": [], "runpaths": []}  # type: Dict[str, List[str]]
+def elf_read_rpaths(fn: str) -> dict[str, list[str]]:
+    result: dict[str, list[str]] = {"rpaths": [], "runpaths": []}
 
     with open(fn, "rb") as f:
         elf = ELFFile(f)
         section = elf.get_section_by_name(".dynamic")
         if section is None:
             return result
 
@@ -135,30 +135,30 @@
 
     if directory not in path.parents:
         return False
 
     return True
 
 
-def get_undefined_symbols(path: str) -> Set[str]:
+def get_undefined_symbols(path: str) -> set[str]:
     undef_symbols = set()
     with open(path, "rb") as f:
         elf = ELFFile(f)
         section = elf.get_section_by_name(".dynsym")
         if section is not None:
             # look for all undef symbols
             for sym in section.iter_symbols():
                 if sym["st_shndx"] == "SHN_UNDEF":
                     undef_symbols.add(sym.name)
     return undef_symbols
 
 
 def filter_undefined_symbols(
-    path: str, symbols: Dict[str, List[str]]
-) -> Dict[str, List[str]]:
+    path: str, symbols: dict[str, list[str]]
+) -> dict[str, list[str]]:
     if not symbols:
         return {}
     undef_symbols = set("*") | get_undefined_symbols(path)
     result = {}
     for lib, sym_list in symbols.items():
         intersection = set(sym_list) & undef_symbols
         if intersection:
```

### Comparing `repairwheel-0.2.3/src/repairwheel/_vendor/auditwheel/genericpkgctx.py` & `repairwheel-0.2.4/src/repairwheel/_vendor/auditwheel/genericpkgctx.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-from typing import Optional, Union
+from __future__ import annotations
 
 from .condatools import InCondaPkgCtx
 from .wheeltools import InWheelCtx
 
 
 def InGenericPkgCtx(
-    in_path: str, out_path: Optional[str] = None
-) -> Union[InWheelCtx, InCondaPkgCtx]:
+    in_path: str, out_path: str | None = None
+) -> InWheelCtx | InCondaPkgCtx:
     """Factory that returns a InWheelCtx or InCondaPkgCtx
     context manager depending on the file extension
     """
     if in_path.endswith(".whl"):
         return InWheelCtx(in_path, out_path)
     if in_path.endswith(".tar.bz2"):
         if out_path is not None:
```

### Comparing `repairwheel-0.2.3/src/repairwheel/_vendor/auditwheel/lddtree.py` & `repairwheel-0.2.4/src/repairwheel/_vendor/auditwheel/lddtree.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,21 +8,23 @@
 """Read the ELF dependency tree
 
 This does not work like `ldd` in that we do not execute/load code (only read
 files on disk), and we parse the dependency structure as a tree rather than
  a flat list.
 """
 
+from __future__ import annotations
+
 import errno
 import functools
 import glob
 import logging
 import os
 from pathlib import Path
-from typing import Any, Dict, List, Optional, Tuple
+from typing import Any
 
 from elftools.elf.elffile import ELFFile
 
 from .libc import Libc, get_libc
 
 log = logging.getLogger(__name__)
 __all__ = ["lddtree"]
@@ -68,21 +70,21 @@
 
     while os.path.islink(root + path):
         path = os.path.join(os.path.dirname(path), os.readlink(root + path))
 
     return normpath((root + path) if prefixed else path)
 
 
-def dedupe(items: List[str]) -> List[str]:
+def dedupe(items: list[str]) -> list[str]:
     """Remove all duplicates from ``items`` (keeping order)"""
-    seen = {}  # type: Dict[str, str]
+    seen: dict[str, str] = {}
     return [seen.setdefault(x, x) for x in items if x not in seen]
 
 
-def parse_ld_paths(str_ldpaths: str, path: str, root: str = "") -> List[str]:
+def parse_ld_paths(str_ldpaths: str, path: str, root: str = "") -> list[str]:
     """Parse the colon-delimited list of paths and apply ldso rules to each
 
     Note the special handling as dictated by the ldso:
     - Empty paths are equivalent to $PWD
     - $ORIGIN is expanded to the path of the given file
     - (TODO) $LIB and friends
 
@@ -95,29 +97,29 @@
     path
         The object actively being parsed (used for $ORIGIN)
 
     Returns
     -------
         list of processed paths
     """
-    ldpaths = []  # type: List[str]
+    ldpaths: list[str] = []
     for ldpath in str_ldpaths.split(":"):
         if ldpath == "":
             # The ldso treats "" paths as $PWD.
             ldpath = os.getcwd()
         elif "$ORIGIN" in ldpath:
             ldpath = ldpath.replace("$ORIGIN", os.path.dirname(os.path.abspath(path)))
         else:
             ldpath = root + ldpath
         ldpaths.append(normpath(ldpath))
     return [p for p in dedupe(ldpaths) if os.path.isdir(p)]
 
 
 @functools.lru_cache()
-def parse_ld_so_conf(ldso_conf: str, root: str = "/", _first: bool = True) -> List[str]:
+def parse_ld_so_conf(ldso_conf: str, root: str = "/", _first: bool = True) -> list[str]:
     """Load all the paths from a given ldso config file
 
     This should handle comments, whitespace, and "include" statements.
 
     Parameters
     ----------
     ldso_conf
@@ -127,15 +129,15 @@
     _first
         Recursive use only; is this the first ELF?
 
     Returns
     -------
     list of paths found
     """
-    paths = []  # type: List[str]
+    paths: list[str] = []
 
     dbg_pfx = "" if _first else "  "
     try:
         log.debug("%sparse_ld_so_conf(%s)", dbg_pfx, ldso_conf)
         with open(ldso_conf) as f:
             for line in f.readlines():
                 line = line.split("#", 1)[0].strip()
@@ -161,15 +163,15 @@
         # Remove duplicate entries to speed things up.
         paths = [p for p in dedupe(paths) if os.path.isdir(p)]
 
     return paths
 
 
 @functools.lru_cache()
-def load_ld_paths(root: str = "/", prefix: str = "") -> Dict[str, List[str]]:
+def load_ld_paths(root: str = "/", prefix: str = "") -> dict[str, list[str]]:
     """Load linker paths from common locations
 
     This parses the ld.so.conf and LD_LIBRARY_PATH env var.
 
     Parameters
     ----------
     root
@@ -177,15 +179,15 @@
     prefix
         The path under ``root`` to search
 
     Returns
     -------
     dict containing library paths to search
     """
-    ldpaths = {"conf": [], "env": [], "interp": []}  # type: Dict
+    ldpaths: dict = {"conf": [], "env": [], "interp": []}
 
     # Load up $LD_LIBRARY_PATH.
     env_ldpath = os.environ.get("LD_LIBRARY_PATH")
     if env_ldpath is not None:
         if root != "/":
             log.warning("ignoring LD_LIBRARY_PATH due to ROOT usage")
         else:
@@ -254,26 +256,26 @@
         and elf1.elfclass == elf2.elfclass
         and elf1.little_endian == elf2.little_endian
         and elf1.header["e_machine"] == elf2.header["e_machine"]
     )
 
 
 def find_lib(
-    elf: ELFFile, lib: str, ldpaths: List[str], root: str = "/"
-) -> Tuple[Optional[str], Optional[str]]:
+    elf: ELFFile, lib: str, ldpaths: list[str], root: str = "/"
+) -> tuple[str | None, str | None]:
     """Try to locate a ``lib`` that is compatible to ``elf`` in the given
     ``ldpaths``
 
     Parameters
     ----------
     elf : ELFFile
         The elf which the library should be compatible with (ELF wise)
     lib : str
         The library (basename) to search for
-    ldpaths : List[str]
+    ldpaths : list[str]
         A list of paths to search
     root : str
        The root path to resolve symlinks
 
     Returns
     -------
     Tuple of the full path to the desired library and the real path to it
@@ -292,19 +294,19 @@
     return (None, None)
 
 
 def lddtree(
     path: str,
     root: str = "/",
     prefix: str = "",
-    ldpaths: Optional[Dict[str, List[str]]] = None,
-    display: Optional[str] = None,
+    ldpaths: dict[str, list[str]] | None = None,
+    display: str | None = None,
     _first: bool = True,
-    _all_libs: Dict = {},
-) -> Dict:
+    _all_libs: dict = {},
+) -> dict:
     """Parse the ELF dependency tree of the specified file
 
     Parameters
     ----------
     path
         The ELF to scan
     root
@@ -343,23 +345,23 @@
     """
     if not ldpaths:
         ldpaths = load_ld_paths().copy()
 
     if _first:
         _all_libs = {}
 
-    ret = {
+    ret: dict[str, Any] = {
         "interp": None,
         "path": path if display is None else display,
         "realpath": path,
         "needed": [],
         "rpath": [],
         "runpath": [],
         "libs": _all_libs,
-    }  # type: Dict[str, Any]
+    }
 
     log.debug("lddtree(%s)" % path)
 
     with open(path, "rb") as f:
         elf = ELFFile(f)
 
         # If this is the first ELF, extract the interpreter.
@@ -383,17 +385,17 @@
                         root + prefix + "/usr" + os.path.dirname(interp).lstrip(prefix)
                     ),
                 ]
                 log.debug("  ldpaths[interp]  = %s", ldpaths["interp"])
                 break
 
         # Parse the ELF's dynamic tags.
-        libs = []  # type: List[str]
-        rpaths = []  # type: List[str]
-        runpaths = []  # type: List[str]
+        libs: list[str] = []
+        rpaths: list[str] = []
+        runpaths: list[str] = []
         for segment in elf.iter_segments():
             if segment.header.p_type != "PT_DYNAMIC":
                 continue
 
             for t in segment.iter_tags():
                 if t.entry.d_tag == "DT_RPATH":
                     rpaths = parse_ld_paths(t.rpath, path=path, root=root)
@@ -416,15 +418,15 @@
             log.debug("  ldpaths[rpath]   = %s", rpaths)
             log.debug("  ldpaths[runpath] = %s", runpaths)
         ret["rpath"] = rpaths
         ret["runpath"] = runpaths
         ret["needed"] = libs
 
         # Search for the libs this ELF uses.
-        all_ldpaths = None  # type: Optional[List[str]]
+        all_ldpaths: list[str] | None = None
         for lib in libs:
             if lib in _all_libs:
                 continue
             if all_ldpaths is None:
                 all_ldpaths = (
                     ldpaths["rpath"]
                     + rpaths
```

### Comparing `repairwheel-0.2.3/src/repairwheel/_vendor/auditwheel/main.py` & `repairwheel-0.2.4/src/repairwheel/_vendor/auditwheel/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,26 @@
+from __future__ import annotations
+
 import argparse
 import logging
 import os
 import pathlib
 import sys
 
 if sys.version_info[:2] >= (3, 8):
     from importlib import metadata
 else:
     import importlib_metadata as metadata
 
-from typing import Optional
-
 from repairwheel._vendor import auditwheel
 
 from . import main_addtag, main_lddtree, main_repair, main_show
 
 
-def main() -> Optional[int]:
+def main() -> int | None:
     if sys.platform != "linux":
         print("Error: This tool only supports Linux")
         return 1
 
     location = pathlib.Path(auditwheel.__file__).parent.resolve()
     version = "auditwheel {} installed at {} (python {}.{})".format(
         metadata.version("auditwheel"), location, *sys.version_info
```

### Comparing `repairwheel-0.2.3/src/repairwheel/_vendor/auditwheel/main_addtag.py` & `repairwheel-0.2.4/src/repairwheel/_vendor/auditwheel/main_addtag.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import logging
 from os.path import abspath, basename, exists, join
 
 logger = logging.getLogger(__name__)
 
 
 def configure_parser(sub_parsers):
```

### Comparing `repairwheel-0.2.3/src/repairwheel/_vendor/auditwheel/main_repair.py` & `repairwheel-0.2.4/src/repairwheel/_vendor/auditwheel/main_repair.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import argparse
 import logging
 from os.path import abspath, basename, exists, isfile
 
 from repairwheel._vendor.auditwheel.patcher import Patchelf
 
 from .policy import (
```

### Comparing `repairwheel-0.2.3/src/repairwheel/_vendor/auditwheel/main_show.py` & `repairwheel-0.2.4/src/repairwheel/_vendor/auditwheel/main_show.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import logging
 from collections import OrderedDict
 
 logger = logging.getLogger(__name__)
 
 
 def configure_parser(sub_parsers):
```

### Comparing `repairwheel-0.2.3/src/repairwheel/_vendor/auditwheel/musllinux.py` & `repairwheel-0.2.4/src/repairwheel/_vendor/auditwheel/musllinux.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import logging
 import pathlib
 import re
 import subprocess
 from typing import NamedTuple
 
 from repairwheel._vendor.auditwheel.error import InvalidLibc
```

### Comparing `repairwheel-0.2.3/src/repairwheel/_vendor/auditwheel/patcher.py` & `repairwheel-0.2.4/src/repairwheel/_vendor/auditwheel/patcher.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,17 @@
+from __future__ import annotations
+
 import re
 from distutils.spawn import find_executable
 from itertools import chain
 from subprocess import CalledProcessError, check_call, check_output
-from typing import Tuple
 
 
 class ElfPatcher:
-    def replace_needed(self, file_name: str, *old_new_pairs: Tuple[str, str]) -> None:
+    def replace_needed(self, file_name: str, *old_new_pairs: tuple[str, str]) -> None:
         raise NotImplementedError
 
     def set_soname(self, file_name: str, new_so_name: str) -> None:
         raise NotImplementedError
 
     def set_rpath(self, file_name: str, rpath: str) -> None:
         raise NotImplementedError
@@ -39,33 +40,31 @@
     )
 
 
 class Patchelf(ElfPatcher):
     def __init__(self) -> None:
         _verify_patchelf()
 
-    def replace_needed(self, file_name: str, *old_new_pairs: Tuple[str, str]) -> None:
+    def replace_needed(self, file_name: str, *old_new_pairs: tuple[str, str]) -> None:
         check_call(
             [
                 "patchelf",
                 *chain.from_iterable(
                     ("--replace-needed", *pair) for pair in old_new_pairs
                 ),
                 file_name,
             ]
         )
 
     def set_soname(self, file_name: str, new_so_name: str) -> None:
         check_call(["patchelf", "--set-soname", new_so_name, file_name])
 
     def set_rpath(self, file_name: str, rpath: str) -> None:
-
         check_call(["patchelf", "--remove-rpath", file_name])
         check_call(["patchelf", "--force-rpath", "--set-rpath", rpath, file_name])
 
     def get_rpath(self, file_name: str) -> str:
-
         return (
             check_output(["patchelf", "--print-rpath", file_name])
             .decode("utf-8")
             .strip()
         )
```

### Comparing `repairwheel-0.2.3/src/repairwheel/_vendor/auditwheel/repair.py` & `repairwheel-0.2.4/src/repairwheel/_vendor/auditwheel/repair.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,21 @@
+from __future__ import annotations
+
 import itertools
 import logging
 import os
 import platform
 import re
 import shutil
 import stat
 from collections import OrderedDict
 from os.path import abspath, basename, dirname, exists, isabs
 from os.path import join as pjoin
 from subprocess import check_call
-from typing import Dict, Iterable, List, Optional, Tuple
+from typing import Iterable
 
 from repairwheel._vendor.auditwheel.patcher import ElfPatcher
 
 from .elfutils import elf_read_dt_needed, elf_read_rpaths, is_subdir
 from .hashfile import hashfile
 from .policy import get_replace_platforms
 from .wheel_abi import get_wheel_elfdata
@@ -28,30 +30,29 @@
      -(?P<pyver>[a-z].+?)-(?P<abi>.+?)-(?P<plat>.+?)(\.whl|\.dist-info)$""",
     re.VERBOSE,
 ).match
 
 
 def repair_wheel(
     wheel_path: str,
-    abis: List[str],
+    abis: list[str],
     lib_sdir: str,
     out_dir: str,
     update_tags: bool,
     patcher: ElfPatcher,
-    exclude: List[str],
+    exclude: list[str],
     strip: bool = False,
-) -> Optional[str]:
-
+) -> str | None:
     external_refs_by_fn = get_wheel_elfdata(wheel_path)[1]
 
     # Do not repair a pure wheel, i.e. has no external refs
     if not external_refs_by_fn:
         return None
 
-    soname_map = {}  # type: Dict[str, Tuple[str, str]]
+    soname_map: dict[str, tuple[str, str]] = {}
     if not isabs(out_dir):
         out_dir = abspath(out_dir)
 
     wheel_fname = basename(wheel_path)
 
     with InWheelCtx(wheel_path) as ctx:
         ctx.out_wheel = pjoin(out_dir, wheel_fname)
@@ -64,18 +65,17 @@
 
         if not exists(dest_dir):
             os.mkdir(dest_dir)
 
         # here, fn is a path to a python extension library in
         # the wheel, and v['libs'] contains its required libs
         for fn, v in external_refs_by_fn.items():
-            ext_libs = v[abis[0]]["libs"]  # type: Dict[str, str]
-            replacements = []  # type: List[Tuple[str, str]]
+            ext_libs: dict[str, str] = v[abis[0]]["libs"]
+            replacements: list[tuple[str, str]] = []
             for soname, src_path in ext_libs.items():
-
                 if soname in exclude:
                     logger.info(f"Excluding {soname}")
                     continue
 
                 if src_path is None:
                     raise ValueError(
                         (
@@ -122,15 +122,15 @@
 
 def strip_symbols(libraries: Iterable[str]) -> None:
     for lib in libraries:
         logger.info("Stripping symbols from %s", lib)
         check_call(["strip", "-s", lib])
 
 
-def copylib(src_path: str, dest_dir: str, patcher: ElfPatcher) -> Tuple[str, str]:
+def copylib(src_path: str, dest_dir: str, patcher: ElfPatcher) -> tuple[str, str]:
     """Graft a shared library from the system into the wheel and update the
     relevant links.
 
     1) Copy the file from src_path to dest_dir/
     2) Rename the shared object from soname to soname.<unique>
     3) If the library has a RUNPATH/RPATH, clear it and set RPATH to point to
     its new location.
```

### Comparing `repairwheel-0.2.3/src/repairwheel/_vendor/auditwheel/tmpdirs.py` & `repairwheel-0.2.4/src/repairwheel/_vendor/auditwheel/tmpdirs.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """ Contexts for *with* statement providing temporary directories
 """
+from __future__ import annotations
+
 import os
 from tempfile import TemporaryDirectory
 from types import TracebackType
-from typing import Optional, Type
 
 
 class InTemporaryDirectory:
     """Create, return, and change directory to a temporary directory
 
     Examples
     --------
@@ -33,17 +34,17 @@
     def __enter__(self) -> str:
         self._pwd = os.getcwd()
         os.chdir(self._tmpdir.name)
         return self._tmpdir.__enter__()
 
     def __exit__(
         self,
-        exc: Optional[Type[BaseException]],
-        value: Optional[BaseException],
-        tb: Optional[TracebackType],
+        exc: type[BaseException] | None,
+        value: BaseException | None,
+        tb: TracebackType | None,
     ) -> None:
         os.chdir(self._pwd)
         return self._tmpdir.__exit__(exc, value, tb)
 
 
 class InGivenDirectory:
     """Change directory to given directory for duration of ``with`` block
@@ -65,15 +66,15 @@
     ...     pass
 
     You can then look at the temporary file outputs to debug what is happening,
     fix, and finally replace ``InGivenDirectory`` with ``InTemporaryDirectory``
     again.
     """
 
-    def __init__(self, path: Optional[str] = None) -> None:
+    def __init__(self, path: str | None = None) -> None:
         """Initialize directory context manager
 
         Parameters
         ----------
         path : None or str, optional
             path to change directory to, for duration of ``with`` block.
             Defaults to ``os.getcwd()`` if None
@@ -87,12 +88,12 @@
         if not os.path.isdir(self.name):
             os.mkdir(self.name)
         os.chdir(self.name)
         return self.name
 
     def __exit__(
         self,
-        exc: Optional[Type[BaseException]],
-        value: Optional[BaseException],
-        tb: Optional[TracebackType],
+        exc: type[BaseException] | None,
+        value: BaseException | None,
+        tb: TracebackType | None,
     ) -> None:
         os.chdir(self._pwd)
```

### Comparing `repairwheel-0.2.3/src/repairwheel/_vendor/auditwheel/tools.py` & `repairwheel-0.2.4/src/repairwheel/_vendor/auditwheel/tools.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,18 @@
+from __future__ import annotations
+
 import argparse
 import os
 import subprocess
 import zipfile
 from datetime import datetime, timezone
-from typing import Any, Iterable, List, Optional
+from typing import Any, Iterable
 
 
-def unique_by_index(sequence: Iterable[Any]) -> List[Any]:
+def unique_by_index(sequence: Iterable[Any]) -> list[Any]:
     """unique elements in `sequence` in the order in which they occur
 
     Parameters
     ----------
     sequence : iterable
 
     Returns
@@ -46,15 +48,15 @@
                 os.chmod(extracted_path, 0o755)
             elif attr != 0:
                 attr &= 511  # only keep permission bits
                 attr |= 6 << 6  # at least read/write for current user
                 os.chmod(extracted_path, attr)
 
 
-def dir2zip(in_dir: str, zip_fname: str, date_time: Optional[datetime] = None) -> None:
+def dir2zip(in_dir: str, zip_fname: str, date_time: datetime | None = None) -> None:
     """Make a zip file `zip_fname` with contents of directory `in_dir`
 
     The recorded filenames are relative to `in_dir`, so doing a standard zip
     unpack of the resulting `zip_fname` in an empty directory will result in
     the original directory contents.
 
     Parameters
```

### Comparing `repairwheel-0.2.3/src/repairwheel/_vendor/auditwheel/wheel_abi.py` & `repairwheel-0.2.4/src/repairwheel/_vendor/auditwheel/wheel_abi.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
+from __future__ import annotations
+
 import functools
 import itertools
 import json
 import logging
 import os
 from collections import defaultdict, namedtuple
 from collections.abc import Mapping
 from copy import deepcopy
 from os.path import basename
-from typing import Dict, Set
 
 from .elfutils import (
     elf_file_filter,
     elf_find_ucs2_symbols,
     elf_find_versioned_symbols,
     elf_is_python_extension,
     elf_references_PyFPE_jbuf,
@@ -58,15 +59,15 @@
 
 
 @functools.lru_cache()
 def get_wheel_elfdata(wheel_fn: str):
     full_elftree = {}
     nonpy_elftree = {}
     full_external_refs = {}
-    versioned_symbols = defaultdict(lambda: set())  # type: Dict[str, Set[str]]
+    versioned_symbols: dict[str, set[str]] = defaultdict(lambda: set())
     uses_ucs2_symbols = False
     uses_PyFPE_jbuf = False
 
     with InGenericPkgCtx(wheel_fn) as ctx:
         shared_libraries_in_purelib = []
 
         platform_wheel = False
@@ -161,22 +162,22 @@
         full_external_refs,
         versioned_symbols,
         uses_ucs2_symbols,
         uses_PyFPE_jbuf,
     )
 
 
-def get_external_libs(external_refs) -> Dict[str, str]:
+def get_external_libs(external_refs) -> dict[str, str]:
     """Get external library dependencies for all policies excluding the default
     linux policy
     :param external_refs: external references for all policies
     :return: {realpath: soname} e.g.
     {'/path/to/external_ref.so.1.2.3': 'external_ref.so.1'}
     """
-    result: Dict[str, str] = {}
+    result: dict[str, str] = {}
     for policy in external_refs.values():
         # linux tag (priority 0) has no white-list, do not analyze it
         if policy["priority"] == 0:
             continue
         # go through all libs, retrieving their soname and realpath
         for libname, realpath in policy["libs"].items():
             if realpath and realpath not in result.keys():
```

### Comparing `repairwheel-0.2.3/src/repairwheel/_vendor/auditwheel/wheeltools.py` & `repairwheel-0.2.4/src/repairwheel/_vendor/auditwheel/wheeltools.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 """ General tools for working with wheels
 
 Tools that aren't specific to delocation
 """
 
+from __future__ import annotations
+
 import csv
 import glob
 import hashlib
 import logging
 import os
 from base64 import urlsafe_b64encode
 from datetime import datetime, timezone
 from itertools import product
 from os.path import abspath, basename, dirname, exists
 from os.path import join as pjoin
 from os.path import relpath
 from os.path import sep as psep
 from os.path import splitext
 from types import TracebackType
-from typing import Generator, Iterable, List, Optional, Type
+from typing import Generator, Iterable
 
 from ._vendor.wheel.pkginfo import read_pkg_info, write_pkg_info
 from ._vendor.wheel.wheelfile import WHEEL_INFO_RE
 from .tmpdirs import InTemporaryDirectory
 from .tools import dir2zip, unique_by_index, zip2dir
 
 logger = logging.getLogger(__name__)
@@ -97,15 +99,15 @@
     """Context manager for doing things inside wheels
 
     On entering, you'll find yourself in the root tree of the wheel.  If you've
     asked for an output wheel, then on exit we'll rewrite the wheel record and
     pack stuff up for you.
     """
 
-    def __init__(self, in_wheel: str, out_wheel: Optional[str] = None) -> None:
+    def __init__(self, in_wheel: str, out_wheel: str | None = None) -> None:
         """Initialize in-wheel context manager
 
         Parameters
         ----------
         in_wheel : str
             filename of wheel to unpack and work inside
         out_wheel : None or str:
@@ -118,17 +120,17 @@
 
     def __enter__(self) -> str:
         zip2dir(self.in_wheel, self.name)
         return super().__enter__()
 
     def __exit__(
         self,
-        exc: Optional[Type[BaseException]],
-        value: Optional[BaseException],
-        tb: Optional[TracebackType],
+        exc: type[BaseException] | None,
+        value: BaseException | None,
+        tb: TracebackType | None,
     ) -> None:
         if self.out_wheel is not None:
             rewrite_record(self.name)
             date_time = None
             timestamp = os.environ.get("SOURCE_DATE_EPOCH")
             if timestamp:
                 date_time = datetime.fromtimestamp(int(timestamp), tz=timezone.utc)
@@ -148,15 +150,15 @@
     will dicate what the output wheel name is, or whether you want to save at
     all.
 
     The current path of the wheel contents is set in the attribute
     ``wheel_path``.
     """
 
-    def __init__(self, in_wheel: str, out_wheel: Optional[str] = None) -> None:
+    def __init__(self, in_wheel: str, out_wheel: str | None = None) -> None:
         """Init in-wheel context manager returning self from enter
 
         Parameters
         ----------
         in_wheel : str
             filename of wheel to unpack and work inside
         out_wheel : None or str:
@@ -182,15 +184,15 @@
         reader = csv.reader(r for r in record.splitlines())
         for row in reader:
             filename = row[0]
             yield filename
 
 
 def add_platforms(
-    wheel_ctx: InWheelCtx, platforms: List[str], remove_platforms: Iterable[str] = ()
+    wheel_ctx: InWheelCtx, platforms: list[str], remove_platforms: Iterable[str] = ()
 ) -> str:
     """Add platform tags `platforms` to a wheel
 
     Add any platform tags in `platforms` that are missing
     to wheel_ctx's filename and ``WHEEL`` file.
 
     Parameters
```

### Comparing `repairwheel-0.2.3/src/repairwheel/_vendor/auditwheel/_vendor/wheel/LICENSE.txt` & `repairwheel-0.2.4/src/repairwheel/_vendor/auditwheel/_vendor/wheel/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.3/src/repairwheel/_vendor/auditwheel/_vendor/wheel/pkginfo.py` & `repairwheel-0.2.4/src/repairwheel/_vendor/auditwheel/_vendor/wheel/pkginfo.py`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.3/src/repairwheel/_vendor/auditwheel/_vendor/wheel/util.py` & `repairwheel-0.2.4/src/repairwheel/_vendor/auditwheel/_vendor/wheel/util.py`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.3/src/repairwheel/_vendor/auditwheel/_vendor/wheel/wheelfile.py` & `repairwheel-0.2.4/src/repairwheel/_vendor/auditwheel/_vendor/wheel/wheelfile.py`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.3/src/repairwheel/_vendor/auditwheel/_vendor/wheel/cli/__init__.py` & `repairwheel-0.2.4/src/repairwheel/_vendor/auditwheel/_vendor/wheel/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.3/src/repairwheel/_vendor/auditwheel/_vendor/wheel/cli/convert.py` & `repairwheel-0.2.4/src/repairwheel/_vendor/auditwheel/_vendor/wheel/cli/convert.py`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.3/src/repairwheel/_vendor/auditwheel/_vendor/wheel/cli/pack.py` & `repairwheel-0.2.4/src/repairwheel/_vendor/auditwheel/_vendor/wheel/cli/pack.py`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.3/src/repairwheel/_vendor/auditwheel/_vendor/wheel/cli/unpack.py` & `repairwheel-0.2.4/src/repairwheel/_vendor/auditwheel/_vendor/wheel/cli/unpack.py`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.3/src/repairwheel/_vendor/auditwheel/policy/__init__.py` & `repairwheel-0.2.4/src/repairwheel/_vendor/auditwheel/policy/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,42 +1,47 @@
+from __future__ import annotations
+
 import json
 import logging
 import platform as _platform_module
 import sys
 from collections import defaultdict
 from os.path import abspath, dirname, join
 from pathlib import Path
-from typing import Dict, List, Optional, Set
 
 from ..libc import Libc, get_libc
 from ..musllinux import find_musl_libc, get_musl_version
 
 _HERE = Path(__file__).parent
 
 logger = logging.getLogger(__name__)
 
 # https://docs.python.org/3/library/platform.html#platform.architecture
 bits = 8 * (8 if sys.maxsize > 2**32 else 4)
 
 
 def get_arch_name() -> str:
     machine = _platform_module.machine()
-    if machine not in {"x86_64", "i686"}:
-        return machine
-    else:
+    if sys.platform == "darwin" and machine == "arm64":
+        return "aarch64"
+    if machine in {"x86_64", "i686"}:
         return {64: "x86_64", 32: "i686"}[bits]
+    if machine in {"aarch64", "armv8l"}:
+        # use armv7l policy for 64-bit arm kernel in 32-bit mode (armv8l)
+        return {64: "aarch64", 32: "armv7l"}[bits]
+    return machine
 
 
 _ARCH_NAME = get_arch_name()
 _LIBC = get_libc()
 
 
 def _validate_pep600_compliance(policies) -> None:
-    symbol_versions: Dict[str, Dict[str, Set[str]]] = {}
-    lib_whitelist: Set[str] = set()
+    symbol_versions: dict[str, dict[str, set[str]]] = {}
+    lib_whitelist: set[str] = set()
     for policy in sorted(policies, key=lambda x: x["priority"], reverse=True):
         if policy["name"] == "linux":
             continue
         if not lib_whitelist.issubset(set(policy["lib_whitelist"])):
             diff = lib_whitelist - set(policy["lib_whitelist"])
             raise ValueError(
                 'Invalid "policy.json" file. Missing whitelist libraries in '
@@ -127,38 +132,38 @@
 
 def _load_policy_schema():
     with open(join(dirname(abspath(__file__)), "policy-schema.json")) as f_:
         schema = json.load(f_)
     return schema
 
 
-def get_policy_by_name(name: str) -> Optional[Dict]:
+def get_policy_by_name(name: str) -> dict | None:
     matches = [p for p in _POLICIES if p["name"] == name or name in p["aliases"]]
     if len(matches) == 0:
         return None
     if len(matches) > 1:
         raise RuntimeError("Internal error. Policies should be unique")
     return matches[0]
 
 
-def get_policy_name(priority: int) -> Optional[str]:
+def get_policy_name(priority: int) -> str | None:
     matches = [p["name"] for p in _POLICIES if p["priority"] == priority]
     if len(matches) == 0:
         return None
     if len(matches) > 1:
         raise RuntimeError("Internal error. priorities should be unique")
     return matches[0]
 
 
-def get_priority_by_name(name: str) -> Optional[int]:
+def get_priority_by_name(name: str) -> int | None:
     policy = get_policy_by_name(name)
     return None if policy is None else policy["priority"]
 
 
-def get_replace_platforms(name: str) -> List[str]:
+def get_replace_platforms(name: str) -> list[str]:
     """Extract platform tag replacement rules from policy
 
     >>> get_replace_platforms('linux_x86_64')
     []
     >>> get_replace_platforms('linux_i686')
     []
     >>> get_replace_platforms('manylinux1_x86_64')
```

### Comparing `repairwheel-0.2.3/src/repairwheel/_vendor/auditwheel/policy/external_references.py` & `repairwheel-0.2.4/src/repairwheel/_vendor/auditwheel/policy/external_references.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,26 @@
+from __future__ import annotations
+
 import logging
 import re
-from typing import Any, Dict, Generator, Set
+from typing import Any, Generator
 
 from ..elfutils import filter_undefined_symbols, is_subdir
 from . import load_policies
 
 log = logging.getLogger(__name__)
-LIBPYTHON_RE = re.compile(r"^libpython\d\.\dm?.so(.\d)*$")
+LIBPYTHON_RE = re.compile(r"^libpython\d+\.\d+m?.so(.\d)*$")
 
 
-def lddtree_external_references(lddtree: Dict, wheel_path: str) -> Dict:
+def lddtree_external_references(lddtree: dict, wheel_path: str) -> dict:
     # XXX: Document the lddtree structure, or put it in something
     # more stable than a big nested dict
     policies = load_policies()
 
-    def filter_libs(libs: Set[str], whitelist: Set[str]) -> Generator[str, None, None]:
+    def filter_libs(libs: set[str], whitelist: set[str]) -> Generator[str, None, None]:
         for lib in libs:
             if "ld-linux" in lib or lib in ["ld64.so.2", "ld64.so.1"]:
                 # always exclude ELF dynamic linker/loader
                 # 'ld64.so.2' on s390x
                 # 'ld64.so.1' on ppc64le
                 # 'ld-linux*' on other platforms
                 continue
@@ -26,29 +28,29 @@
                 # always exclude libpythonXY
                 continue
             if lib in whitelist:
                 # exclude any libs in the whitelist
                 continue
             yield lib
 
-    def get_req_external(libs: Set[str], whitelist: Set[str]) -> Set[str]:
+    def get_req_external(libs: set[str], whitelist: set[str]) -> set[str]:
         # get all the required external libraries
         libs = libs.copy()
         reqs = set()
         while libs:
             lib = libs.pop()
             reqs.add(lib)
             for dep in filter_libs(lddtree["libs"][lib]["needed"], whitelist):
                 if dep not in reqs:
                     libs.add(dep)
         return reqs
 
-    ret = {}  # type: Dict[str, Dict[str, Any]]
+    ret: dict[str, dict[str, Any]] = {}
     for p in policies:
-        needed_external_libs = set()  # type: Set[str]
+        needed_external_libs: set[str] = set()
         blacklist = {}
 
         if not (p["name"] == "linux" and p["priority"] == 0):
             # special-case the generic linux platform here, because it
             # doesn't have a whitelist. or, you could say its
             # whitelist is the complete set of all libraries. so nothing
             # is considered "external" that needs to be copied in.
```

### Comparing `repairwheel-0.2.3/src/repairwheel/_vendor/auditwheel/policy/manylinux-policy.json` & `repairwheel-0.2.4/src/repairwheel/_vendor/auditwheel/policy/manylinux-policy.json`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.3/src/repairwheel/_vendor/auditwheel/policy/musllinux-policy.json` & `repairwheel-0.2.4/src/repairwheel/_vendor/auditwheel/policy/musllinux-policy.json`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.3/src/repairwheel/_vendor/auditwheel/policy/policy-schema.json` & `repairwheel-0.2.4/src/repairwheel/_vendor/auditwheel/policy/policy-schema.json`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.3/src/repairwheel/_vendor/auditwheel/policy/versioned_symbols.py` & `repairwheel-0.2.4/src/repairwheel/_vendor/auditwheel/policy/versioned_symbols.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,19 @@
+from __future__ import annotations
+
 import logging
-from typing import Dict, List, Set
 
 from . import load_policies
 
 log = logging.getLogger(__name__)
 
 
-def versioned_symbols_policy(versioned_symbols: Dict[str, Set[str]]) -> int:
+def versioned_symbols_policy(versioned_symbols: dict[str, set[str]]) -> int:
     def policy_is_satisfied(
-        policy_name: str, policy_sym_vers: Dict[str, Set[str]]
+        policy_name: str, policy_sym_vers: dict[str, set[str]]
     ) -> bool:
         policy_satisfied = True
         for name in set(required_vers) & set(policy_sym_vers):
             if not required_vers[name].issubset(policy_sym_vers[name]):
                 for symbol in required_vers[name] - policy_sym_vers[name]:
                     log.debug(
                         "Package requires %s, incompatible with "
@@ -20,20 +21,20 @@
                         symbol,
                         policy_name,
                         policy_sym_vers[name],
                     )
                 policy_satisfied = False
         return policy_satisfied
 
-    required_vers = {}  # type: Dict[str, Set[str]]
+    required_vers: dict[str, set[str]] = {}
     for symbols in versioned_symbols.values():
         for symbol in symbols:
             sym_name, _, _ = symbol.partition("_")
             required_vers.setdefault(sym_name, set()).add(symbol)
-    matching_policies = []  # type: List[int]
+    matching_policies: list[int] = []
     for p in load_policies():
         policy_sym_vers = {
             sym_name: {sym_name + "_" + version for version in versions}
             for sym_name, versions in p["symbol_versions"].items()
         }
         if policy_is_satisfied(p["name"], policy_sym_vers):
             matching_policies.append(p["priority"])
```

### Comparing `repairwheel-0.2.3/src/repairwheel/_vendor/delocate/LICENSE` & `repairwheel-0.2.4/src/repairwheel/_vendor/delocate/LICENSE`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.3/src/repairwheel/_vendor/delocate/delocating.py` & `repairwheel-0.2.4/src/repairwheel/_vendor/delocate/delocating.py`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.3/src/repairwheel/_vendor/delocate/fuse.py` & `repairwheel-0.2.4/src/repairwheel/_vendor/delocate/fuse.py`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.3/src/repairwheel/_vendor/delocate/libsana.py` & `repairwheel-0.2.4/src/repairwheel/_vendor/delocate/libsana.py`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.3/src/repairwheel/_vendor/delocate/pkginfo.py` & `repairwheel-0.2.4/src/repairwheel/_vendor/delocate/pkginfo.py`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.3/src/repairwheel/_vendor/delocate/tmpdirs.py` & `repairwheel-0.2.4/src/repairwheel/_vendor/delocate/tmpdirs.py`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.3/src/repairwheel/_vendor/delocate/tools.py` & `repairwheel-0.2.4/src/repairwheel/_vendor/delocate/tools.py`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.3/src/repairwheel/_vendor/delocate/wheeltools.py` & `repairwheel-0.2.4/src/repairwheel/_vendor/delocate/wheeltools.py`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.3/src/repairwheel/_vendor/delocate/cmd/delocate_addplat.py` & `repairwheel-0.2.4/src/repairwheel/_vendor/delocate/cmd/delocate_addplat.py`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.3/src/repairwheel/_vendor/delocate/cmd/delocate_fuse.py` & `repairwheel-0.2.4/src/repairwheel/_vendor/delocate/cmd/delocate_fuse.py`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.3/src/repairwheel/_vendor/delocate/cmd/delocate_listdeps.py` & `repairwheel-0.2.4/src/repairwheel/_vendor/delocate/cmd/delocate_listdeps.py`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.3/src/repairwheel/_vendor/delocate/cmd/delocate_patch.py` & `repairwheel-0.2.4/src/repairwheel/_vendor/delocate/cmd/delocate_patch.py`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.3/src/repairwheel/_vendor/delocate/cmd/delocate_path.py` & `repairwheel-0.2.4/src/repairwheel/_vendor/delocate/cmd/delocate_path.py`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.3/src/repairwheel/_vendor/delocate/cmd/delocate_wheel.py` & `repairwheel-0.2.4/src/repairwheel/_vendor/delocate/cmd/delocate_wheel.py`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.3/src/repairwheel/linux/elffile.py` & `repairwheel-0.2.4/src/repairwheel/linux/elffile.py`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.3/src/repairwheel/linux/monkeypatch.py` & `repairwheel-0.2.4/src/repairwheel/linux/monkeypatch.py`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.3/src/repairwheel/linux/patcher.py` & `repairwheel-0.2.4/src/repairwheel/linux/patcher.py`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.3/src/repairwheel/linux/repair.py` & `repairwheel-0.2.4/src/repairwheel/linux/repair.py`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.3/src/repairwheel/macos/machosign.py` & `repairwheel-0.2.4/src/repairwheel/macos/machosign.py`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.3/src/repairwheel/macos/machotools.py` & `repairwheel-0.2.4/src/repairwheel/macos/machotools.py`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.3/src/repairwheel/macos/repair.py` & `repairwheel-0.2.4/src/repairwheel/macos/repair.py`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.3/src/repairwheel/windows/repair.py` & `repairwheel-0.2.4/src/repairwheel/windows/repair.py`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.3/tests/conftest.py` & `repairwheel-0.2.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.3/tests/test_common.py` & `repairwheel-0.2.4/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.3/tests/test_windows.py` & `repairwheel-0.2.4/tests/test_windows.py`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.3/tests/util.py` & `repairwheel-0.2.4/tests/util.py`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.3/tests/gen_check/test_check.py` & `repairwheel-0.2.4/tests/gen_check/test_check.py`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.3/tests/testwheel/build-native/build.py` & `repairwheel-0.2.4/tests/testwheel/build-native/build.py`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.3/tests/testwheel/build-native/testwheel.c` & `repairwheel-0.2.4/tests/testwheel/build-native/testwheel.c`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.3/tests/testwheel/cp36-abi3-linux_x86_64/testwheel-0.0.1-cp36-abi3-linux_x86_64.whl` & `repairwheel-0.2.4/tests/testwheel/cp36-abi3-linux_x86_64/testwheel-0.0.1-cp36-abi3-linux_x86_64.whl`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.3/tests/testwheel/cp36-abi3-linux_x86_64/lib/libtestdep.so` & `repairwheel-0.2.4/tests/testwheel/cp36-abi3-linux_x86_64/lib/libtestdep.so`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.3/tests/testwheel/cp36-abi3-macosx_10_11_arm64/testwheel-0.0.1-cp36-abi3-macosx_10_11_arm64.whl` & `repairwheel-0.2.4/tests/testwheel/cp36-abi3-macosx_10_11_arm64/testwheel-0.0.1-cp36-abi3-macosx_10_11_arm64.whl`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.3/tests/testwheel/cp36-abi3-macosx_10_11_arm64/lib/libtestdep.dylib` & `repairwheel-0.2.4/tests/testwheel/cp36-abi3-macosx_10_11_arm64/lib/libtestdep.dylib`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.3/tests/testwheel/cp36-abi3-macosx_10_11_x86_64/testwheel-0.0.1-cp36-abi3-macosx_10_11_x86_64.whl` & `repairwheel-0.2.4/tests/testwheel/cp36-abi3-macosx_10_11_x86_64/testwheel-0.0.1-cp36-abi3-macosx_10_11_x86_64.whl`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.3/tests/testwheel/cp36-abi3-macosx_10_11_x86_64/lib/libtestdep.dylib` & `repairwheel-0.2.4/tests/testwheel/cp36-abi3-macosx_10_11_x86_64/lib/libtestdep.dylib`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.3/tests/testwheel/cp36-abi3-win_amd64/testwheel-0.0.1-cp36-abi3-win_amd64.whl` & `repairwheel-0.2.4/tests/testwheel/cp36-abi3-win_amd64/testwheel-0.0.1-cp36-abi3-win_amd64.whl`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.3/tests/testwheel/cp36-abi3-win_amd64/lib/testdep.dll` & `repairwheel-0.2.4/tests/testwheel/cp36-abi3-win_amd64/lib/testdep.dll`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.3/tests/testwheel/py3-none-any/testwheel-0.0.1-py3-none-any.whl` & `repairwheel-0.2.4/tests/testwheel/py3-none-any/testwheel-0.0.1-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.3/tools/vendoring/patches/auditwheel.patch` & `repairwheel-0.2.4/tools/vendoring/patches/auditwheel.patch`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 diff --git a/src/repairwheel/_vendor/auditwheel/elfutils.py b/src/repairwheel/_vendor/auditwheel/elfutils.py
 index 33527c9..a319350 100644
 --- a/src/repairwheel/_vendor/auditwheel/elfutils.py
 +++ b/src/repairwheel/_vendor/auditwheel/elfutils.py
-@@ -1,5 +1,5 @@
+@@ -3,5 +3,5 @@
 -import os
 -from os.path import basename, realpath, relpath
 +from os.path import basename
 +from pathlib import Path
- from typing import Dict, Iterator, List, Optional, Set, Tuple
+ from typing import Iterator
  
  from elftools.common.exceptions import ELFError
-@@ -130,12 +130,12 @@ def is_subdir(path: str, directory: str) -> bool:
+@@ -131,12 +131,12 @@ def is_subdir(path: str, directory: str) -> bool:
      if path is None:
          return False
  
 -    path = realpath(path)
 -    directory = realpath(directory)
 +    path = Path(path).resolve()
 +    directory = Path(directory).resolve()
```

### Comparing `repairwheel-0.2.3/tools/vendoring/patches/delocate.chmod.patch` & `repairwheel-0.2.4/tools/vendoring/patches/delocate.chmod.patch`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.3/tools/vendoring/patches/delocate.patch` & `repairwheel-0.2.4/tools/vendoring/patches/delocate.patch`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.3/LICENSE` & `repairwheel-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.3/README.md` & `repairwheel-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `repairwheel-0.2.3/pyproject.toml` & `repairwheel-0.2.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "repairwheel"
-version = "0.2.3"
+version = "0.2.4"
 description = "Repair any wheel, anywhere"
 readme = "README.md"
 requires-python = ">= 3.7"
 license.file = "LICENSE"
 classifiers = [
   "License :: OSI Approved :: MIT License",
   "Programming Language :: Python :: 3",
```

### Comparing `repairwheel-0.2.3/PKG-INFO` & `repairwheel-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: repairwheel
-Version: 0.2.3
+Version: 0.2.4
 Summary: Repair any wheel, anywhere
 Project-URL: homepage, https://github.com/jvolkman/repairwheel
 License: Copyright © 2023 Jeremy Volkman
         
         Permission is hereby granted, free of charge, to any person obtaining a
         copy of this software and associated documentation files (the "Software"),
         to deal in the Software without restriction, including without limitation
```

