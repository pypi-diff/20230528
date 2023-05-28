# Comparing `tmp/chiakilisp-1.4.0rc5-py3-none-any.whl.zip` & `tmp/chiakilisp-1.4.0rc6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,21 +1,21 @@
-Zip file size: 27299 bytes, number of entries: 19
+Zip file size: 27302 bytes, number of entries: 19
 -rw-r--r--  2.0 unx        0 b- defN 22-May-22 18:38 chiakilisp/__init__.py
--rw-r--r--  2.0 unx    14396 b- defN 23-May-27 22:56 chiakilisp/lexer.py
+-rw-r--r--  2.0 unx    14401 b- defN 23-May-27 23:49 chiakilisp/lexer.py
 -rw-r--r--  2.0 unx     5943 b- defN 23-May-18 21:24 chiakilisp/parser.py
 -rw-r--r--  2.0 unx     1378 b- defN 23-May-19 18:48 chiakilisp/runtime.py
 -rw-r--r--  2.0 unx    11225 b- defN 23-May-18 22:30 chiakilisp/spec.py
 -rw-r--r--  2.0 unx     3311 b- defN 23-May-27 10:34 chiakilisp/utils.py
 -rw-r--r--  2.0 unx     7391 b- defN 23-May-27 22:54 chiakilisp/corelib/core.cl
 -rw-r--r--  2.0 unx        0 b- defN 22-Jun-13 11:18 chiakilisp/models/__init__.py
 -rw-r--r--  2.0 unx    31150 b- defN 23-May-27 22:02 chiakilisp/models/expression.py
 -rw-r--r--  2.0 unx      790 b- defN 23-May-15 20:31 chiakilisp/models/forward.py
 -rw-r--r--  2.0 unx     4001 b- defN 23-May-27 22:34 chiakilisp/models/literal.py
 -rw-r--r--  2.0 unx     2123 b- defN 23-May-27 22:28 chiakilisp/models/token.py
 -rw-r--r--  2.0 unx        0 b- defN 23-May-15 20:31 chiakilisp/proxies/__init__.py
 -rw-r--r--  2.0 unx      205 b- defN 23-May-15 20:31 chiakilisp/proxies/keyword.py
--rwxr-xr-x  2.0 unx    13359 b- defN 23-May-27 23:14 chiakilisp-1.4.0rc5.data/scripts/chiakilang
--rw-r--r--  2.0 unx     1408 b- defN 23-May-27 23:14 chiakilisp-1.4.0rc5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-27 23:14 chiakilisp-1.4.0rc5.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-May-27 23:14 chiakilisp-1.4.0rc5.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1559 b- defN 23-May-27 23:14 chiakilisp-1.4.0rc5.dist-info/RECORD
-19 files, 98342 bytes uncompressed, 24751 bytes compressed:  74.8%
+-rwxr-xr-x  2.0 unx    13359 b- defN 23-May-27 23:55 chiakilisp-1.4.0rc6.data/scripts/chiakilang
+-rw-r--r--  2.0 unx     1408 b- defN 23-May-27 23:55 chiakilisp-1.4.0rc6.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-27 23:55 chiakilisp-1.4.0rc6.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-May-27 23:55 chiakilisp-1.4.0rc6.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1559 b- defN 23-May-27 23:55 chiakilisp-1.4.0rc6.dist-info/RECORD
+19 files, 98347 bytes uncompressed, 24754 bytes compressed:  74.8%
```

## zipnote {}

```diff
@@ -36,23 +36,23 @@
 
 Filename: chiakilisp/proxies/__init__.py
 Comment: 
 
 Filename: chiakilisp/proxies/keyword.py
 Comment: 
 
-Filename: chiakilisp-1.4.0rc5.data/scripts/chiakilang
+Filename: chiakilisp-1.4.0rc6.data/scripts/chiakilang
 Comment: 
 
-Filename: chiakilisp-1.4.0rc5.dist-info/METADATA
+Filename: chiakilisp-1.4.0rc6.dist-info/METADATA
 Comment: 
 
-Filename: chiakilisp-1.4.0rc5.dist-info/WHEEL
+Filename: chiakilisp-1.4.0rc6.dist-info/WHEEL
 Comment: 
 
-Filename: chiakilisp-1.4.0rc5.dist-info/top_level.txt
+Filename: chiakilisp-1.4.0rc6.dist-info/top_level.txt
 Comment: 
 
-Filename: chiakilisp-1.4.0rc5.dist-info/RECORD
+Filename: chiakilisp-1.4.0rc6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## chiakilisp/lexer.py

```diff
@@ -120,15 +120,15 @@
                     if self._current_symbol_is_number() \
                             or self._current_symbol_is_dot():
                         value += self._current_symbol()
                         self._advance()
                         self._increment_char_number()
                     else:
                         break
-                if re.match(r'^\d\.{2}\d?$', value):
+                if re.match(r'^\d+?\.{2}(\d+)?$', value):
                     self._tokens.append(Token(Token.Slice, value, self.pos()))
                 elif re.match(r'^(-)?\d+(\.\d+)?$', value):
                     self._tokens.append(Token(Token.Number, value, self.pos()))
                 else:
                     self._raise_syntax_error(f'Invalid float syntax: {value}.')
 
             elif self._current_symbol_is_letter() \
@@ -149,15 +149,15 @@
                     self._tokens.append(Token(Token.Number, value, self.pos()))
                 elif value.startswith(':'):
                     self._tokens.append(Token(Token.Keyword, value, self.pos()))
                 elif value == 'nil':
                     self._tokens.append(Token(Token.Nil, value, self.pos()))
                 elif value in ['true', 'false']:
                     self._tokens.append(Token(Token.Boolean, value, self.pos()))
-                elif re.match(r'^\.{2}\d$', value):  # make it equivalent for: 0..2
+                elif re.match(r'^\.{2}\d+$', value):  # make it equivalent for 0..2
                     self._tokens.append(Token(Token.Slice, value, self.pos()))
                 else:
                     self._tokens.append(Token(Token.Identifier, value, self.pos()))
 
             elif self._current_symbol_is_double_quote():
                 value = ''
                 while self._has_next_symbol():
```

## Comparing `chiakilisp-1.4.0rc5.data/scripts/chiakilang` & `chiakilisp-1.4.0rc6.data/scripts/chiakilang`

 * *Files identical despite different names*

## Comparing `chiakilisp-1.4.0rc5.dist-info/METADATA` & `chiakilisp-1.4.0rc6.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chiakilisp
-Version: 1.4.0rc5
+Version: 1.4.0rc6
 Summary: ChiakiLisp - Yet another LISP
 Home-page: https://chiakilisp.jedi2light.moe
 Author: @jedi2light
 Author-email: jedi2light@jedi2light.moe
 Maintainer: @jedi2light
 Maintainer-email: jedi2light@jedi2light.moe
 License: WTFPL
```

## Comparing `chiakilisp-1.4.0rc5.dist-info/RECORD` & `chiakilisp-1.4.0rc6.dist-info/RECORD`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 chiakilisp/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-chiakilisp/lexer.py,sha256=6CSBSHw3V-_UIBSvf-6qGwzDNXgJoxN49JrwDmIr63c,14396
+chiakilisp/lexer.py,sha256=6zSmOLVskcHKqGFGImXKYdLjthT-OxBXKqE0kU0FuhQ,14401
 chiakilisp/parser.py,sha256=aPAa3U8D28DO15NzwUliLTOZeCaQEu5giOpzCnPBSs8,5943
 chiakilisp/runtime.py,sha256=J69abrFy4RdcA6oU9z2Pv4ok4A7h5X8lR9VM1l28kk4,1378
 chiakilisp/spec.py,sha256=4_hvO1HYm3RGnky1q85q72we1L3wpjufDgoVU_kcTwk,11225
 chiakilisp/utils.py,sha256=lYwdSJY_y5QEBAM9rEd02Z9ra9ZADJ_yO8JIfsS2WAM,3311
 chiakilisp/corelib/core.cl,sha256=YaxdnBJt0U7ebyXvIK2gE4KR5TGOAiPksy6PYhqatBg,7391
 chiakilisp/models/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 chiakilisp/models/expression.py,sha256=T2R6S3pMAJxmcrjbmxueyDfzAUE8aOzbTutNV-451y4,31150
 chiakilisp/models/forward.py,sha256=ykZjLoXxONjvoCZ3h2itUieAFteh5TUiAuk4f8NoiZs,790
 chiakilisp/models/literal.py,sha256=Dg5tqdDWzuaW0NvxtZpHP9CQAvTDDjB4eJGMFuxWImc,4001
 chiakilisp/models/token.py,sha256=1ks0qk_t-V-EaLu_LhjEeHx2hrPa_bbyIsqHxdFeAeU,2123
 chiakilisp/proxies/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 chiakilisp/proxies/keyword.py,sha256=fMVWpRxk_Sk_6CXE08IFnFTtMbvhadUSe2IYgin_h60,205
-chiakilisp-1.4.0rc5.data/scripts/chiakilang,sha256=-vbv8w6RFangekz5zoX-FBDYFabYX_Ad4VvvPD8Hvro,13359
-chiakilisp-1.4.0rc5.dist-info/METADATA,sha256=QFgsViQU2H69SFkA8uXuTISKETgXSKJg8jscoNxMO-c,1408
-chiakilisp-1.4.0rc5.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-chiakilisp-1.4.0rc5.dist-info/top_level.txt,sha256=uV87HteR3vUsfEm7HlxKG0Fh7zkoke2RetMtgLu97Bc,11
-chiakilisp-1.4.0rc5.dist-info/RECORD,,
+chiakilisp-1.4.0rc6.data/scripts/chiakilang,sha256=-vbv8w6RFangekz5zoX-FBDYFabYX_Ad4VvvPD8Hvro,13359
+chiakilisp-1.4.0rc6.dist-info/METADATA,sha256=Mj9euCLkCwew08v61lxVPCKZqdLUSsJOtRIVcOXzBgw,1408
+chiakilisp-1.4.0rc6.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+chiakilisp-1.4.0rc6.dist-info/top_level.txt,sha256=uV87HteR3vUsfEm7HlxKG0Fh7zkoke2RetMtgLu97Bc,11
+chiakilisp-1.4.0rc6.dist-info/RECORD,,
```

