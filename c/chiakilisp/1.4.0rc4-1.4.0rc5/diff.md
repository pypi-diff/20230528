# Comparing `tmp/chiakilisp-1.4.0rc4-py3-none-any.whl.zip` & `tmp/chiakilisp-1.4.0rc5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,21 +1,21 @@
-Zip file size: 27071 bytes, number of entries: 19
+Zip file size: 27299 bytes, number of entries: 19
 -rw-r--r--  2.0 unx        0 b- defN 22-May-22 18:38 chiakilisp/__init__.py
--rw-r--r--  2.0 unx    13791 b- defN 23-May-19 18:36 chiakilisp/lexer.py
+-rw-r--r--  2.0 unx    14396 b- defN 23-May-27 22:56 chiakilisp/lexer.py
 -rw-r--r--  2.0 unx     5943 b- defN 23-May-18 21:24 chiakilisp/parser.py
 -rw-r--r--  2.0 unx     1378 b- defN 23-May-19 18:48 chiakilisp/runtime.py
 -rw-r--r--  2.0 unx    11225 b- defN 23-May-18 22:30 chiakilisp/spec.py
 -rw-r--r--  2.0 unx     3311 b- defN 23-May-27 10:34 chiakilisp/utils.py
--rw-r--r--  2.0 unx     7443 b- defN 23-May-23 21:25 chiakilisp/corelib/core.cl
+-rw-r--r--  2.0 unx     7391 b- defN 23-May-27 22:54 chiakilisp/corelib/core.cl
 -rw-r--r--  2.0 unx        0 b- defN 22-Jun-13 11:18 chiakilisp/models/__init__.py
--rw-r--r--  2.0 unx    31381 b- defN 23-May-27 16:44 chiakilisp/models/expression.py
+-rw-r--r--  2.0 unx    31150 b- defN 23-May-27 22:02 chiakilisp/models/expression.py
 -rw-r--r--  2.0 unx      790 b- defN 23-May-15 20:31 chiakilisp/models/forward.py
--rw-r--r--  2.0 unx     3778 b- defN 23-May-15 20:32 chiakilisp/models/literal.py
--rw-r--r--  2.0 unx     1986 b- defN 23-May-15 20:31 chiakilisp/models/token.py
+-rw-r--r--  2.0 unx     4001 b- defN 23-May-27 22:34 chiakilisp/models/literal.py
+-rw-r--r--  2.0 unx     2123 b- defN 23-May-27 22:28 chiakilisp/models/token.py
 -rw-r--r--  2.0 unx        0 b- defN 23-May-15 20:31 chiakilisp/proxies/__init__.py
 -rw-r--r--  2.0 unx      205 b- defN 23-May-15 20:31 chiakilisp/proxies/keyword.py
--rwxr-xr-x  2.0 unx    13359 b- defN 23-May-27 16:47 chiakilisp-1.4.0rc4.data/scripts/chiakilang
--rw-r--r--  2.0 unx     1408 b- defN 23-May-27 16:47 chiakilisp-1.4.0rc4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-27 16:47 chiakilisp-1.4.0rc4.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-May-27 16:47 chiakilisp-1.4.0rc4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1559 b- defN 23-May-27 16:47 chiakilisp-1.4.0rc4.dist-info/RECORD
-19 files, 97660 bytes uncompressed, 24523 bytes compressed:  74.9%
+-rwxr-xr-x  2.0 unx    13359 b- defN 23-May-27 23:14 chiakilisp-1.4.0rc5.data/scripts/chiakilang
+-rw-r--r--  2.0 unx     1408 b- defN 23-May-27 23:14 chiakilisp-1.4.0rc5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-27 23:14 chiakilisp-1.4.0rc5.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-May-27 23:14 chiakilisp-1.4.0rc5.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1559 b- defN 23-May-27 23:14 chiakilisp-1.4.0rc5.dist-info/RECORD
+19 files, 98342 bytes uncompressed, 24751 bytes compressed:  74.8%
```

## zipnote {}

```diff
@@ -36,23 +36,23 @@
 
 Filename: chiakilisp/proxies/__init__.py
 Comment: 
 
 Filename: chiakilisp/proxies/keyword.py
 Comment: 
 
-Filename: chiakilisp-1.4.0rc4.data/scripts/chiakilang
+Filename: chiakilisp-1.4.0rc5.data/scripts/chiakilang
 Comment: 
 
-Filename: chiakilisp-1.4.0rc4.dist-info/METADATA
+Filename: chiakilisp-1.4.0rc5.dist-info/METADATA
 Comment: 
 
-Filename: chiakilisp-1.4.0rc4.dist-info/WHEEL
+Filename: chiakilisp-1.4.0rc5.dist-info/WHEEL
 Comment: 
 
-Filename: chiakilisp-1.4.0rc4.dist-info/top_level.txt
+Filename: chiakilisp-1.4.0rc5.dist-info/top_level.txt
 Comment: 
 
-Filename: chiakilisp-1.4.0rc4.dist-info/RECORD
+Filename: chiakilisp-1.4.0rc5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## chiakilisp/lexer.py

```diff
@@ -18,14 +18,20 @@
 
     _source_code: str  # <----------------------------------- source code context
     _source_code_file_name: str  # <----------------------- source code file name
     _pointer: int = 0  # <------------------------------ default pointer position
     _tokens: List[Token]  # <----------------------- list of the populated Tokens
     _line_num, _char_num = 1, 0  # <------------ initial pointer position in file
 
+    def _raise_syntax_error(self, message: str) -> None:
+
+        """A shortcut for future that helps to throw a SyntaxError"""
+
+        raise SyntaxError(f'{":".join(map(str, self.pos()))}: {message}')
+
     def __init__(self, source_code: str, source_code_file_name: str) -> None:
 
         """Initialize Lexer instance"""
 
         self._source_code = source_code
         self._source_code_file_name = source_code_file_name
         self._tokens = []
@@ -103,50 +109,56 @@
                 self._tokens.append(Token(Token.Identifier,   'tuply', self.pos()))
                 self._advance()
                 self._increment_char_number()  # <-- increment character num as well
 
             elif self._current_symbol_is_number() \
                     or (self._current_symbol_is_sign()
                         and self._next_symbol_is_number()):
-                has_already_encountered_dot_character = False
                 value = self._current_symbol()
                 self._advance()
                 self._increment_char_number()
                 while self._has_next_symbol():
-                    if self._current_symbol_is_number() or \
-                            (self._current_symbol_is_dot() and
-                             not has_already_encountered_dot_character):
-                        if self._current_symbol_is_dot():
-                            has_already_encountered_dot_character = True
+                    if self._current_symbol_is_number() \
+                            or self._current_symbol_is_dot():
                         value += self._current_symbol()
                         self._advance()
                         self._increment_char_number()
                     else:
                         break
-                self._tokens.append(Token(Token.Number, value, self.pos()))
+                if re.match(r'^\d\.{2}\d?$', value):
+                    self._tokens.append(Token(Token.Slice, value, self.pos()))
+                elif re.match(r'^(-)?\d+(\.\d+)?$', value):
+                    self._tokens.append(Token(Token.Number, value, self.pos()))
+                else:
+                    self._raise_syntax_error(f'Invalid float syntax: {value}.')
 
             elif self._current_symbol_is_letter() \
                     or self._current_symbol_is_colon():
                 value = self._current_symbol()
                 self._advance()
                 self._increment_char_number()
                 while self._has_next_symbol():
                     if self._current_symbol_is_letter() or \
                             self._current_symbol_is_number():
                         value += self._current_symbol()
                         self._advance()
                         self._increment_char_number()
                     else:
                         break
-                if value.startswith(':'):
+                if re.match(r'^\.\d+$', value):
+                    value = '0' + value  # make it possible to define 0.2 as .2
+                    self._tokens.append(Token(Token.Number, value, self.pos()))
+                elif value.startswith(':'):
                     self._tokens.append(Token(Token.Keyword, value, self.pos()))
                 elif value == 'nil':
                     self._tokens.append(Token(Token.Nil, value, self.pos()))
                 elif value in ['true', 'false']:
                     self._tokens.append(Token(Token.Boolean, value, self.pos()))
+                elif re.match(r'^\.{2}\d$', value):  # make it equivalent for: 0..2
+                    self._tokens.append(Token(Token.Slice, value, self.pos()))
                 else:
                     self._tokens.append(Token(Token.Identifier, value, self.pos()))
 
             elif self._current_symbol_is_double_quote():
                 value = ''
                 while self._has_next_symbol():
                     self._advance()
```

## chiakilisp/corelib/core.cl

```diff
@@ -55,14 +55,16 @@
   (isinstance x dict))
 (defn bool? (x)              ;; Returns true if 'x' is a boolean
   (isinstance x bool))
 (defn float? (x)             ;; Returns true if 'x' is a float number
   (isinstance x float))
 (defn tuple? (x)             ;; Returns true if 'x' is a tuple
   (isinstance x tuple))
+(defn slice? (x)             ;; Returns true if `x` is a slice
+  (isinstance x slice))
 (defn keyword? (x)           ;; Returns true if 'x' is a keyword
   (isinstance x keyword/Keyword))
 
 (defn not (x)                ;; Returns inverted boolean presentation
   (if x false true))
 
 (defn = (first second)       ;; Returns whether both items do equal
@@ -93,15 +95,15 @@
   (let (coll (.__getitem__ args 0)
         item (.__getitem__ args 1))
    (cond (= 2 (count args)) (get coll item nil)
          (= 3 (count args))
          (let (default   (.__getitem__ args 2))
           (cond (set? coll) (when (contains? coll item) item)
                 (and (or (str? coll) (list? coll) (tuple? coll))
-                     (int? item))
+                     (or (int? item) (slice? item)))
                 (try (.__getitem__ coll item)
                   (catch IndexError _ default))
                 (dict? coll) (try (.__getitem__ coll item)
                                    (catch KeyError __ default))))))))
 
 (defn first (coll)                 ;; Returns a first collection item
  (when (or (list? coll) (tuple? coll) (str? coll))
@@ -113,23 +115,16 @@
  (when (or (list? coll) (tuple? coll) (str? coll))
   (get coll 2)))
 (defn last (coll)                 ;; Returns the last collection item
  (when (or (list? coll) (tuple? coll) (str? coll))
   (get coll -1))))
 
 (defn rest (coll)                 ;; Returns the rest of a collection
- (when (and coll
-            (or (list? coll)
-                (tuple? coll)))
-  (let (cast (cond (list? coll) list
-                   (tuple? coll) tuple)   ;; preserve collection type
-        new  (list coll)
-        rev  (-> new reversed list))
-   (.pop rev)
-   (-> rev reversed cast))))
+ (when (and coll (or (str? coll) (list? coll) (tuple? coll)))
+  (get coll (slice 1..))))        ;; this one is equivalent for: [1:]
 
 (defn get-in (& args)        ;; Goes through full path to get an item
  (when args
   (let ((coll path default) args)
         (cond (>= (count args) 2)
               (functools/reduce (fn (acc n)
                                   (get acc n default)) path coll)))))
```

## chiakilisp/models/expression.py

```diff
@@ -199,15 +199,14 @@
             SE_ASSERT(where, len(tail) >= 1,  'Expression[execute]: keyword must be followed by at least one arg')
             SE_ASSERT(where, len(tail) <= 2,   'Expression[execute]: keyword can be followed by at most two args')
             collection, default = tail if len(tail) == 2 else (tail[0], Nil)  # <--- define collection and default
             return get(
                 collection.execute(environ, False), head.execute(environ, False), default.execute(environ, False))
 
         if self._is_inline_fn:  # <--- if this expression is actually an inline function: i.e.: #(prn "Hello," %1)
-
             RE_ASSERT(where, first,     'Expression[execute]: unable to use inline function without `core/first`')
 
             def handler(*args, **kwargs):   # <---------------------- then construct an anonymous function handler
 
                 ifn = {}  # <----------------------------------------- start with an empty computation environment
                 ifn.update(environ)  # <-------------------------------------------- update it with the global one
                 ifn.update({'%': first(args)})  # <-------------------------- make an alias for the first argument
@@ -383,24 +382,22 @@
 
             handle.x__custom_name__x = '<anonymous function>'  # set the function name to the <anonymous function>
             return handle  # <-------------------------------------------------- return the function handle object
 
         if head.token().value() == 'def':
             SE_ASSERT(where, top,   'Expression[execute]: def: can only use (def) form at the top of the program')
             TAIL_IS_VALID(tail, 'def', where,                                   'Expression[execute]: def: {why}')
-            name: Literal  # <--------------------------------------------------- assign name as a type of Literal
             name, value = tail  # <-------------------------------------------------- assign value as a CommonType
             computed = value.execute(environ, False)  # <-------------------------------- store the computed value
             environ.update({name.token().value(): computed})  # <------------------- assign it to its binding name
             return computed   # <----------------------------------------------------------- return computed value
 
         if head.token().value() == 'def?':
             SE_ASSERT(where, top, 'Expression[execute]: def?: can only use (def?) form at the top of the program')
             TAIL_IS_VALID(tail, 'def?', where,                                 'Expression[execute]: def?: {why}')
-            name: Literal  # <--------------------------------------------------- assign name as a type of Literal
             name, value = tail  # <-------------------------------------------------- assign value as a CommonType
             from_env = environ.get(name.token().value()) if (name.token().value() in environ.keys()) else NotFound
             computed = value.execute(environ, False) if from_env is NotFound else from_env  # try to find existing
             environ.update({name.token().value(): computed})  # assign existing/computed value to its binding name
             return computed   # <----------------------------------------------------------- return computed value
 
         if head.token().value() == 'defn':
```

## chiakilisp/models/literal.py

```diff
@@ -55,14 +55,19 @@
 
         """Execute, here, is to return Python value tied to the literal: number, string, boolean, etc ..."""
 
         if self.token().type() == Token.Nil:
 
             return None
 
+        if self.token().type() == Token.Slice:
+
+            start_point, end_pint = self.token().value().split('..')
+            return slice(int(start_point) if start_point else None, int(end_pint) if end_pint else None)
+
         if self.token().type() == Token.Number:
 
             return float(self.token().value()) if '.' in self.token().value() else int(self.token().value())
 
         if self.token().type() == Token.String:
 
             return self.token().value()
```

## chiakilisp/models/token.py

```diff
@@ -4,14 +4,15 @@
 class Token:
 
     """
     Token is the class that encapsulates a part of a source code: number, string or something else
     """
 
     Nil: str = 'Nil'
+    Slice: str = 'Slice'
     Number: str = 'Number'
     String: str = 'String'
     Keyword: str = 'Keyword'
     Boolean: str = 'Boolean'
     Identifier: str = 'Identifier'
     OpeningParen: str = 'OpeningParen'
     ClosingParen: str = 'ClosingParen'
@@ -50,14 +51,20 @@
 
     def is_nil(self) -> bool:
 
         """Just a handy shortcut"""
 
         return self._type == Token.Nil
 
+    def is_slice(self) -> bool:
+
+        """Just a handy shortcut"""
+
+        return self._type == Token.Slice
+
     def is_number(self) -> bool:
 
         """Just a handy shortcut"""
 
         return self._type == Token.Number
 
     def is_string(self) -> bool:
```

## Comparing `chiakilisp-1.4.0rc4.data/scripts/chiakilang` & `chiakilisp-1.4.0rc5.data/scripts/chiakilang`

 * *Files identical despite different names*

## Comparing `chiakilisp-1.4.0rc4.dist-info/METADATA` & `chiakilisp-1.4.0rc5.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chiakilisp
-Version: 1.4.0rc4
+Version: 1.4.0rc5
 Summary: ChiakiLisp - Yet another LISP
 Home-page: https://chiakilisp.jedi2light.moe
 Author: @jedi2light
 Author-email: jedi2light@jedi2light.moe
 Maintainer: @jedi2light
 Maintainer-email: jedi2light@jedi2light.moe
 License: WTFPL
```

## Comparing `chiakilisp-1.4.0rc4.dist-info/RECORD` & `chiakilisp-1.4.0rc5.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 chiakilisp/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-chiakilisp/lexer.py,sha256=FnLU7DPtpVRLP2rkMQ3h1INQ4KC-MLy_vAjSrvPG9vg,13791
+chiakilisp/lexer.py,sha256=6CSBSHw3V-_UIBSvf-6qGwzDNXgJoxN49JrwDmIr63c,14396
 chiakilisp/parser.py,sha256=aPAa3U8D28DO15NzwUliLTOZeCaQEu5giOpzCnPBSs8,5943
 chiakilisp/runtime.py,sha256=J69abrFy4RdcA6oU9z2Pv4ok4A7h5X8lR9VM1l28kk4,1378
 chiakilisp/spec.py,sha256=4_hvO1HYm3RGnky1q85q72we1L3wpjufDgoVU_kcTwk,11225
 chiakilisp/utils.py,sha256=lYwdSJY_y5QEBAM9rEd02Z9ra9ZADJ_yO8JIfsS2WAM,3311
-chiakilisp/corelib/core.cl,sha256=a-vhEjziW_vQy9kfWFF_SJbNPdL4O0sx23AwaUvAdR4,7443
+chiakilisp/corelib/core.cl,sha256=YaxdnBJt0U7ebyXvIK2gE4KR5TGOAiPksy6PYhqatBg,7391
 chiakilisp/models/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-chiakilisp/models/expression.py,sha256=yRBvimRfmTRUYiO4GeLSZdlY1GFnsZeAfsKTeeKfmMs,31381
+chiakilisp/models/expression.py,sha256=T2R6S3pMAJxmcrjbmxueyDfzAUE8aOzbTutNV-451y4,31150
 chiakilisp/models/forward.py,sha256=ykZjLoXxONjvoCZ3h2itUieAFteh5TUiAuk4f8NoiZs,790
-chiakilisp/models/literal.py,sha256=0m0FRZ9YLq23pH_DKjSSObey5gZIo73BUJP37F5svsA,3778
-chiakilisp/models/token.py,sha256=TYfdqCVn3_74aBCn6m5gPikjpwixUW65FeKrMLuvpvE,1986
+chiakilisp/models/literal.py,sha256=Dg5tqdDWzuaW0NvxtZpHP9CQAvTDDjB4eJGMFuxWImc,4001
+chiakilisp/models/token.py,sha256=1ks0qk_t-V-EaLu_LhjEeHx2hrPa_bbyIsqHxdFeAeU,2123
 chiakilisp/proxies/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 chiakilisp/proxies/keyword.py,sha256=fMVWpRxk_Sk_6CXE08IFnFTtMbvhadUSe2IYgin_h60,205
-chiakilisp-1.4.0rc4.data/scripts/chiakilang,sha256=-vbv8w6RFangekz5zoX-FBDYFabYX_Ad4VvvPD8Hvro,13359
-chiakilisp-1.4.0rc4.dist-info/METADATA,sha256=KYbur4Dz8kwHeDMLhQbsEHT5K_hmcTtWZ4XQFfX5A4g,1408
-chiakilisp-1.4.0rc4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-chiakilisp-1.4.0rc4.dist-info/top_level.txt,sha256=uV87HteR3vUsfEm7HlxKG0Fh7zkoke2RetMtgLu97Bc,11
-chiakilisp-1.4.0rc4.dist-info/RECORD,,
+chiakilisp-1.4.0rc5.data/scripts/chiakilang,sha256=-vbv8w6RFangekz5zoX-FBDYFabYX_Ad4VvvPD8Hvro,13359
+chiakilisp-1.4.0rc5.dist-info/METADATA,sha256=QFgsViQU2H69SFkA8uXuTISKETgXSKJg8jscoNxMO-c,1408
+chiakilisp-1.4.0rc5.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+chiakilisp-1.4.0rc5.dist-info/top_level.txt,sha256=uV87HteR3vUsfEm7HlxKG0Fh7zkoke2RetMtgLu97Bc,11
+chiakilisp-1.4.0rc5.dist-info/RECORD,,
```

