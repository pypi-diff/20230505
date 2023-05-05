# Comparing `tmp/morse-transcript-0.0.2.tar.gz` & `tmp/morse-transcript-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "morse-transcript-0.0.2.tar", last modified: Fri May  5 12:47:00 2023, max compression
+gzip compressed data, was "morse-transcript-0.0.3.tar", last modified: Fri May  5 15:13:56 2023, max compression
```

## Comparing `morse-transcript-0.0.2.tar` & `morse-transcript-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 12:47:00.842143 morse-transcript-0.0.2/
--rw-rw-rw-   0        0        0     1091 2023-05-05 11:15:04.000000 morse-transcript-0.0.2/LICENSE.md
--rw-rw-rw-   0        0        0     2679 2023-05-05 12:47:00.842143 morse-transcript-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1122 2023-05-05 12:45:05.000000 morse-transcript-0.0.2/README.md
--rw-rw-rw-   0        0        0       88 2023-05-05 12:14:05.000000 morse-transcript-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0      151 2023-05-05 12:47:00.843137 morse-transcript-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      637 2023-05-05 12:46:50.000000 morse-transcript-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-05 12:47:00.831089 morse-transcript-0.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-05-05 12:47:00.839146 morse-transcript-0.0.2/src/morse_transcript.egg-info/
--rw-rw-rw-   0        0        0     2679 2023-05-05 12:47:00.000000 morse-transcript-0.0.2/src/morse_transcript.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      319 2023-05-05 12:47:00.000000 morse-transcript-0.0.2/src/morse_transcript.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 12:47:00.000000 morse-transcript-0.0.2/src/morse_transcript.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-05-05 12:47:00.000000 morse-transcript-0.0.2/src/morse_transcript.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-05 12:47:00.841138 morse-transcript-0.0.2/src/morsecodetranslator/
--rw-rw-rw-   0        0        0        0 2023-05-05 11:15:04.000000 morse-transcript-0.0.2/src/morsecodetranslator/__init__.py
--rw-rw-rw-   0        0        0     3342 2023-05-05 11:49:52.000000 morse-transcript-0.0.2/src/morsecodetranslator/morse.py
-drwxrwxrwx   0        0        0        0 2023-05-05 12:47:00.842143 morse-transcript-0.0.2/tests/
--rw-rw-rw-   0        0        0      535 2023-05-05 11:49:52.000000 morse-transcript-0.0.2/tests/test_morse.py
+drwxr-xr-x   0 gugu       (501) staff       (20)        0 2023-05-05 15:13:56.688654 morse-transcript-0.0.3/
+-rw-r--r--   0 gugu       (501) staff       (20)     1070 2023-05-05 13:19:26.000000 morse-transcript-0.0.3/LICENSE.md
+-rw-r--r--   0 gugu       (501) staff       (20)     2608 2023-05-05 15:13:56.688717 morse-transcript-0.0.3/PKG-INFO
+-rw-r--r--   0 gugu       (501) staff       (20)     1088 2023-05-05 13:19:26.000000 morse-transcript-0.0.3/README.md
+-rw-r--r--   0 gugu       (501) staff       (20)       85 2023-05-05 13:19:26.000000 morse-transcript-0.0.3/pyproject.toml
+-rw-r--r--   0 gugu       (501) staff       (20)      143 2023-05-05 15:13:56.688993 morse-transcript-0.0.3/setup.cfg
+-rw-r--r--   0 gugu       (501) staff       (20)      717 2023-05-05 15:13:47.000000 morse-transcript-0.0.3/setup.py
+drwxr-xr-x   0 gugu       (501) staff       (20)        0 2023-05-05 15:13:56.686154 morse-transcript-0.0.3/src/
+drwxr-xr-x   0 gugu       (501) staff       (20)        0 2023-05-05 15:13:56.687257 morse-transcript-0.0.3/src/cli/
+-rw-r--r--   0 gugu       (501) staff       (20)        0 2023-05-05 14:20:24.000000 morse-transcript-0.0.3/src/cli/__init__.py
+-rw-r--r--   0 gugu       (501) staff       (20)     1283 2023-05-05 15:07:11.000000 morse-transcript-0.0.3/src/cli/morse.py
+drwxr-xr-x   0 gugu       (501) staff       (20)        0 2023-05-05 15:13:56.688063 morse-transcript-0.0.3/src/morse_transcript.egg-info/
+-rw-r--r--   0 gugu       (501) staff       (20)     2608 2023-05-05 15:13:56.000000 morse-transcript-0.0.3/src/morse_transcript.egg-info/PKG-INFO
+-rw-r--r--   0 gugu       (501) staff       (20)      403 2023-05-05 15:13:56.000000 morse-transcript-0.0.3/src/morse_transcript.egg-info/SOURCES.txt
+-rw-r--r--   0 gugu       (501) staff       (20)        1 2023-05-05 15:13:56.000000 morse-transcript-0.0.3/src/morse_transcript.egg-info/dependency_links.txt
+-rw-r--r--   0 gugu       (501) staff       (20)       41 2023-05-05 15:13:56.000000 morse-transcript-0.0.3/src/morse_transcript.egg-info/entry_points.txt
+-rw-r--r--   0 gugu       (501) staff       (20)       24 2023-05-05 15:13:56.000000 morse-transcript-0.0.3/src/morse_transcript.egg-info/top_level.txt
+drwxr-xr-x   0 gugu       (501) staff       (20)        0 2023-05-05 15:13:56.688363 morse-transcript-0.0.3/src/morsecodetranslator/
+-rw-r--r--   0 gugu       (501) staff       (20)        0 2023-05-05 13:19:26.000000 morse-transcript-0.0.3/src/morsecodetranslator/__init__.py
+-rw-r--r--   0 gugu       (501) staff       (20)     3543 2023-05-05 15:00:39.000000 morse-transcript-0.0.3/src/morsecodetranslator/morse.py
+drwxr-xr-x   0 gugu       (501) staff       (20)        0 2023-05-05 15:13:56.688525 morse-transcript-0.0.3/tests/
+-rw-r--r--   0 gugu       (501) staff       (20)      516 2023-05-05 13:19:26.000000 morse-transcript-0.0.3/tests/test_morse.py
```

### Comparing `morse-transcript-0.0.2/PKG-INFO` & `morse-transcript-0.0.3/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,71 +1,71 @@
-Metadata-Version: 2.1
-Name: morse-transcript
-Version: 0.0.2
-Summary: Convert text to Morse Code and vise-versa.
-Home-page: https://github.com/gugupy/morsecodetranslator
-Author: Gughanathan M
-Author-email: gugu.ap900@gmail.com
-License: MIT
-Keywords: MorseCode,Morse
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-
-# Morse Code Translator
-
-[![dot-dash](dotdash.png)](https://en.wikipedia.org/wiki/Morse_code)
-
-[![codecov](https://codecov.io/gh/gugupy/morsecodetranslator/branch/master/graph/badge.svg?token=TG5AR36QNI)](https://codecov.io/gh/gugupy/morsecodetranslator)
-
-Its converts plain text to morse code and vice versa and follows below rules for the conversion as per the morse-code algorithm,  
-1. Single space for same char repeats  
-2. Three spaces for different char  
-3. Seven spaces to differentiate the word  
-
-## Installation
-
-### Method 1:
-To install the MorseCodeTranslator just run the command `pip install -U morse-transcript`
-
-### Method 2:
-1. Clone the repository `git clone https://github.com/gugupy/morsecodetranslator.git`
-2. Run the command `pip install -e .`
-
-
-## Sample code
-```python
-from morsecodetranslator.morse import MorseCodeTranslator
-
-mct = MorseCodeTranslator()
-print(mct.encrypt('MORSE CODE'))
-print(mct.decrypt('--   ---   .-.   ...   .       -.-.   ---   -..   .'))
-```
-### output
-``` textmate
---   ---   .-.   -.-.   .       -.-.   ---   -..   .  
-MORSE CODE
-```
-
-MIT License
-
-Copyright (c) 2022 Gughanathan M
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+Metadata-Version: 2.1
+Name: morse-transcript
+Version: 0.0.3
+Summary: Convert text to Morse Code and vise-versa.
+Home-page: https://github.com/gugupy/morsecodetranslator
+Author: Gughanathan M
+Author-email: gugu.ap900@gmail.com
+License: MIT
+Keywords: MorseCode,Morse
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE.md
+
+# Morse Code Translator
+
+[![dot-dash](dotdash.png)](https://en.wikipedia.org/wiki/Morse_code)
+
+[![codecov](https://codecov.io/gh/gugupy/morsecodetranslator/branch/master/graph/badge.svg?token=TG5AR36QNI)](https://codecov.io/gh/gugupy/morsecodetranslator)
+
+Its converts plain text to morse code and vice versa and follows below rules for the conversion as per the morse-code algorithm,  
+1. Single space for same char repeats  
+2. Three spaces for different char  
+3. Seven spaces to differentiate the word  
+
+## Installation
+
+### Method 1:
+To install the MorseCodeTranslator just run the command `pip install -U morse-transcript`
+
+### Method 2:
+1. Clone the repository `git clone https://github.com/gugupy/morsecodetranslator.git`
+2. Run the command `pip install -e .`
+
+
+## Sample code
+```python
+from morsecodetranslator.morse import MorseCodeTranslator
+
+mct = MorseCodeTranslator()
+print(mct.encrypt('MORSE CODE'))
+print(mct.decrypt('--   ---   .-.   ...   .       -.-.   ---   -..   .'))
+```
+### output
+``` textmate
+--   ---   .-.   -.-.   .       -.-.   ---   -..   .  
+MORSE CODE
+```
+
+MIT License
+
+Copyright (c) 2022 Gughanathan M
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `morse-transcript-0.0.2/README.md` & `morse-transcript-0.0.3/README.md`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-# Morse Code Translator
-
-[![dot-dash](dotdash.png)](https://en.wikipedia.org/wiki/Morse_code)
-
-[![codecov](https://codecov.io/gh/gugupy/morsecodetranslator/branch/master/graph/badge.svg?token=TG5AR36QNI)](https://codecov.io/gh/gugupy/morsecodetranslator)
-
-Its converts plain text to morse code and vice versa and follows below rules for the conversion as per the morse-code algorithm,  
-1. Single space for same char repeats  
-2. Three spaces for different char  
-3. Seven spaces to differentiate the word  
-
-## Installation
-
-### Method 1:
-To install the MorseCodeTranslator just run the command `pip install -U morse-transcript`
-
-### Method 2:
-1. Clone the repository `git clone https://github.com/gugupy/morsecodetranslator.git`
-2. Run the command `pip install -e .`
-
-
-## Sample code
-```python
-from morsecodetranslator.morse import MorseCodeTranslator
-
-mct = MorseCodeTranslator()
-print(mct.encrypt('MORSE CODE'))
-print(mct.decrypt('--   ---   .-.   ...   .       -.-.   ---   -..   .'))
-```
-### output
-``` textmate
---   ---   .-.   -.-.   .       -.-.   ---   -..   .  
-MORSE CODE
-```
+# Morse Code Translator
+
+[![dot-dash](dotdash.png)](https://en.wikipedia.org/wiki/Morse_code)
+
+[![codecov](https://codecov.io/gh/gugupy/morsecodetranslator/branch/master/graph/badge.svg?token=TG5AR36QNI)](https://codecov.io/gh/gugupy/morsecodetranslator)
+
+Its converts plain text to morse code and vice versa and follows below rules for the conversion as per the morse-code algorithm,  
+1. Single space for same char repeats  
+2. Three spaces for different char  
+3. Seven spaces to differentiate the word  
+
+## Installation
+
+### Method 1:
+To install the MorseCodeTranslator just run the command `pip install -U morse-transcript`
+
+### Method 2:
+1. Clone the repository `git clone https://github.com/gugupy/morsecodetranslator.git`
+2. Run the command `pip install -e .`
+
+
+## Sample code
+```python
+from morsecodetranslator.morse import MorseCodeTranslator
+
+mct = MorseCodeTranslator()
+print(mct.encrypt('MORSE CODE'))
+print(mct.decrypt('--   ---   .-.   ...   .       -.-.   ---   -..   .'))
+```
+### output
+``` textmate
+--   ---   .-.   -.-.   .       -.-.   ---   -..   .  
+MORSE CODE
+```
```

### Comparing `morse-transcript-0.0.2/src/morse_transcript.egg-info/PKG-INFO` & `morse-transcript-0.0.3/src/morse_transcript.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,71 +1,71 @@
-Metadata-Version: 2.1
-Name: morse-transcript
-Version: 0.0.2
-Summary: Convert text to Morse Code and vise-versa.
-Home-page: https://github.com/gugupy/morsecodetranslator
-Author: Gughanathan M
-Author-email: gugu.ap900@gmail.com
-License: MIT
-Keywords: MorseCode,Morse
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-
-# Morse Code Translator
-
-[![dot-dash](dotdash.png)](https://en.wikipedia.org/wiki/Morse_code)
-
-[![codecov](https://codecov.io/gh/gugupy/morsecodetranslator/branch/master/graph/badge.svg?token=TG5AR36QNI)](https://codecov.io/gh/gugupy/morsecodetranslator)
-
-Its converts plain text to morse code and vice versa and follows below rules for the conversion as per the morse-code algorithm,  
-1. Single space for same char repeats  
-2. Three spaces for different char  
-3. Seven spaces to differentiate the word  
-
-## Installation
-
-### Method 1:
-To install the MorseCodeTranslator just run the command `pip install -U morse-transcript`
-
-### Method 2:
-1. Clone the repository `git clone https://github.com/gugupy/morsecodetranslator.git`
-2. Run the command `pip install -e .`
-
-
-## Sample code
-```python
-from morsecodetranslator.morse import MorseCodeTranslator
-
-mct = MorseCodeTranslator()
-print(mct.encrypt('MORSE CODE'))
-print(mct.decrypt('--   ---   .-.   ...   .       -.-.   ---   -..   .'))
-```
-### output
-``` textmate
---   ---   .-.   -.-.   .       -.-.   ---   -..   .  
-MORSE CODE
-```
-
-MIT License
-
-Copyright (c) 2022 Gughanathan M
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+Metadata-Version: 2.1
+Name: morse-transcript
+Version: 0.0.3
+Summary: Convert text to Morse Code and vise-versa.
+Home-page: https://github.com/gugupy/morsecodetranslator
+Author: Gughanathan M
+Author-email: gugu.ap900@gmail.com
+License: MIT
+Keywords: MorseCode,Morse
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE.md
+
+# Morse Code Translator
+
+[![dot-dash](dotdash.png)](https://en.wikipedia.org/wiki/Morse_code)
+
+[![codecov](https://codecov.io/gh/gugupy/morsecodetranslator/branch/master/graph/badge.svg?token=TG5AR36QNI)](https://codecov.io/gh/gugupy/morsecodetranslator)
+
+Its converts plain text to morse code and vice versa and follows below rules for the conversion as per the morse-code algorithm,  
+1. Single space for same char repeats  
+2. Three spaces for different char  
+3. Seven spaces to differentiate the word  
+
+## Installation
+
+### Method 1:
+To install the MorseCodeTranslator just run the command `pip install -U morse-transcript`
+
+### Method 2:
+1. Clone the repository `git clone https://github.com/gugupy/morsecodetranslator.git`
+2. Run the command `pip install -e .`
+
+
+## Sample code
+```python
+from morsecodetranslator.morse import MorseCodeTranslator
+
+mct = MorseCodeTranslator()
+print(mct.encrypt('MORSE CODE'))
+print(mct.decrypt('--   ---   .-.   ...   .       -.-.   ---   -..   .'))
+```
+### output
+``` textmate
+--   ---   .-.   -.-.   .       -.-.   ---   -..   .  
+MORSE CODE
+```
+
+MIT License
+
+Copyright (c) 2022 Gughanathan M
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `morse-transcript-0.0.2/src/morsecodetranslator/morse.py` & `morse-transcript-0.0.3/src/morsecodetranslator/morse.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,111 +1,123 @@
-import re
-
-__all__ = 'MorseCodeTranslator'
-
-
-class MorseCodeTranslator:
-    """
-    Morce code translator convert text to morce code and vice versa.
-    Its follow below algorithm for the conversion as per the morce-code,
-        1. Single space for same char follows
-        2. Three spaces for different char
-        3. Seven spaces to differentiate the word
-    """
-    def __init__(self):
-        self.__MORSE_CODE = {
-            'A': '.-',
-            'B': '-...',
-            'C': '-.-.',
-            'D': '-..',
-            'E': '.',
-            'F': '..-.',
-            'G': '--.',
-            'H': '....',
-            'I': '..',
-            'J': '.---',
-            'K': '-.-',
-            'L': '.-..',
-            'M': '--',
-            'N': '-.',
-            'O': '---',
-            'P': '.--.',
-            'Q': '--.-',
-            'R': '.-.',
-            'S': '...',
-            'T': '-',
-            'U': '..-',
-            'V': '...-',
-            'W': '.--',
-            'X': '-..-',
-            'Y': '-.--',
-            'Z': '--..',
-            '1': '.----',
-            '2': '..---',
-            '3': '...--',
-            '4': '....-',
-            '5': '.....',
-            '6': '-....',
-            '7': '--...',
-            '8': '---..',
-            '9': '----.',
-            '0': '-----'
-        }
-
-    def encrypt(self, message) -> str:
-        """
-        Encrypt text to morce code
-
-        :param message: message for convert to morce code
-        :return: morce code
-        """
-
-        morce_code = ''
-        _pre_char = None
-
-        for char in str(message).upper():
-            # Evaluating space to separate the word
-            if char == ' ':
-                morce_code += '       '
-                # reset the previous char to None
-                # To avoid append space to the morce code 
-                # on the next word cycle
-                _pre_char = None
-                continue
-            # Checking previous char is current char
-            # To add spaces based on the morce algorithm
-            if _pre_char:
-                if str(_pre_char).__eq__(char):
-                    morce_code += ' '
-                else:
-                    morce_code += '   '
-            morce_code += self.__MORSE_CODE.get(char)
-            _pre_char = char
-        return morce_code
-
-    def decrypt(self, morce_code) -> str:
-        """
-        Decrypting the morce code to text
-
-        :param morce_code: morce code for convert to text
-        :return: Plain text of equivalent morce code
-        """
-        message = ''
-
-        # Splitting the morce based more than 4 spaces
-        # So its exactly split the words
-        mc_li = re.split(r'\s\s\s\s+', morce_code)
-        for mc in mc_li:
-            if mc == '':
-                continue
-            codes = re.split(r'\s+', mc)
-            for code in codes:
-                idx = list(self.__MORSE_CODE.values()).index(code)
-                message += list(self.__MORSE_CODE.keys())[idx]
-            message += ' '
-        return message.removesuffix(' ')
-
-
-if __name__ == '__main__':
-    mct = MorseCodeTranslator()
-    print(mct.encrypt('MORSE CODE'))
-    print(mct.decrypt('--   ---   .-.   ...   .       -.-.   ---   -..   .'))
+import re
+
+__all__ = 'MorseCodeTranslator'
+
+
+class MorseCodeTranslator:
+    """
+    morse code translator convert text to morse code and vice versa.
+    Its follow below algorithm for the conversion as per the morse-code,
+        1. Single space for same char follows
+        2. Three spaces for different char
+        3. Seven spaces to differentiate the word
+    """
+    def __init__(self):
+        self.__MORSE_CODE = {
+            'A': '.-',
+            'B': '-...',
+            'C': '-.-.',
+            'D': '-..',
+            'E': '.',
+            'F': '..-.',
+            'G': '--.',
+            'H': '....',
+            'I': '..',
+            'J': '.---',
+            'K': '-.-',
+            'L': '.-..',
+            'M': '--',
+            'N': '-.',
+            'O': '---',
+            'P': '.--.',
+            'Q': '--.-',
+            'R': '.-.',
+            'S': '...',
+            'T': '-',
+            'U': '..-',
+            'V': '...-',
+            'W': '.--',
+            'X': '-..-',
+            'Y': '-.--',
+            'Z': '--..',
+            '1': '.----',
+            '2': '..---',
+            '3': '...--',
+            '4': '....-',
+            '5': '.....',
+            '6': '-....',
+            '7': '--...',
+            '8': '---..',
+            '9': '----.',
+            '0': '-----'
+        }
+
+    def encrypt(self, message) -> str:
+        """
+        Encrypt text to morse code
+
+        :param message: message for convert to morse code
+        :return: morse code
+        """
+
+        morse_code = ''
+        _pre_char = None
+
+        for char in str(message).upper():
+            # Evaluating space to separate the word
+            if char == ' ':
+                morse_code += '       '
+                # reset the previous char to None
+                # To avoid append space to the morse code 
+                # on the next word cycle
+                _pre_char = None
+                continue
+            # Checking previous char is current char
+            # To add spaces based on the morse algorithm
+            if _pre_char:
+                if str(_pre_char).__eq__(char):
+                    morse_code += ' '
+                else:
+                    morse_code += '   '
+
+            try:
+                morse_code += self.__MORSE_CODE.get(char)
+            except TypeError:
+                print(f'"{char}" is not a valid text to get Morse Code!')
+                exit(1)
+
+            _pre_char = char
+        return morse_code
+
+    def decrypt(self, morse_code) -> str:
+        """
+        Decrypting the morse code to text
+
+        :param morse_code: morse code for convert to text
+        :return: Plain text of equivalent morse code
+        """
+        message = ''
+
+        # Splitting the morse based more than 4 spaces
+        # So its exactly split the words
+        mc_li = re.split(r'\s\s\s\s+', morse_code)
+        for mc in mc_li:
+            if mc == '':
+                continue
+            codes = re.split(r'\s+', mc)
+            for code in codes:
+
+                try:
+                    idx = list(self.__MORSE_CODE.values()).index(code)
+                    message += list(self.__MORSE_CODE.keys())[idx]
+                except ValueError:
+                    print(f'"{code}" is not a valid Morse Code! ')
+                    exit(1)
+
+            message += ' '
+        return message.removesuffix(' ')
+
+
+if __name__ == '__main__':
+    mct = MorseCodeTranslator()
+    print(mct.encrypt('MORSE CODE'))
+    print(mct.decrypt('--   ---   .-.   ...   .       -.-.   ---   -..   .'))
```

