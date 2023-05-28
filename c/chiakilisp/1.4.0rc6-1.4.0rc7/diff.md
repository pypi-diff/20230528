# Comparing `tmp/chiakilisp-1.4.0rc6-py3-none-any.whl.zip` & `tmp/chiakilisp-1.4.0rc7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,21 +1,21 @@
-Zip file size: 27302 bytes, number of entries: 19
+Zip file size: 27319 bytes, number of entries: 19
 -rw-r--r--  2.0 unx        0 b- defN 22-May-22 18:38 chiakilisp/__init__.py
--rw-r--r--  2.0 unx    14401 b- defN 23-May-27 23:49 chiakilisp/lexer.py
+-rw-r--r--  2.0 unx    14553 b- defN 23-May-28 20:46 chiakilisp/lexer.py
 -rw-r--r--  2.0 unx     5943 b- defN 23-May-18 21:24 chiakilisp/parser.py
 -rw-r--r--  2.0 unx     1378 b- defN 23-May-19 18:48 chiakilisp/runtime.py
 -rw-r--r--  2.0 unx    11225 b- defN 23-May-18 22:30 chiakilisp/spec.py
 -rw-r--r--  2.0 unx     3311 b- defN 23-May-27 10:34 chiakilisp/utils.py
--rw-r--r--  2.0 unx     7391 b- defN 23-May-27 22:54 chiakilisp/corelib/core.cl
+-rw-r--r--  2.0 unx     7391 b- defN 23-May-28 13:22 chiakilisp/corelib/core.cl
 -rw-r--r--  2.0 unx        0 b- defN 22-Jun-13 11:18 chiakilisp/models/__init__.py
 -rw-r--r--  2.0 unx    31150 b- defN 23-May-27 22:02 chiakilisp/models/expression.py
 -rw-r--r--  2.0 unx      790 b- defN 23-May-15 20:31 chiakilisp/models/forward.py
--rw-r--r--  2.0 unx     4001 b- defN 23-May-27 22:34 chiakilisp/models/literal.py
+-rw-r--r--  2.0 unx     4001 b- defN 23-May-28 20:48 chiakilisp/models/literal.py
 -rw-r--r--  2.0 unx     2123 b- defN 23-May-27 22:28 chiakilisp/models/token.py
 -rw-r--r--  2.0 unx        0 b- defN 23-May-15 20:31 chiakilisp/proxies/__init__.py
 -rw-r--r--  2.0 unx      205 b- defN 23-May-15 20:31 chiakilisp/proxies/keyword.py
--rwxr-xr-x  2.0 unx    13359 b- defN 23-May-27 23:55 chiakilisp-1.4.0rc6.data/scripts/chiakilang
--rw-r--r--  2.0 unx     1408 b- defN 23-May-27 23:55 chiakilisp-1.4.0rc6.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-27 23:55 chiakilisp-1.4.0rc6.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-May-27 23:55 chiakilisp-1.4.0rc6.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1559 b- defN 23-May-27 23:55 chiakilisp-1.4.0rc6.dist-info/RECORD
-19 files, 98347 bytes uncompressed, 24754 bytes compressed:  74.8%
+-rwxr-xr-x  2.0 unx    13359 b- defN 23-May-28 21:12 chiakilisp-1.4.0rc7.data/scripts/chiakilang
+-rw-r--r--  2.0 unx     1408 b- defN 23-May-28 21:12 chiakilisp-1.4.0rc7.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-28 21:12 chiakilisp-1.4.0rc7.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-May-28 21:12 chiakilisp-1.4.0rc7.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1559 b- defN 23-May-28 21:12 chiakilisp-1.4.0rc7.dist-info/RECORD
+19 files, 98499 bytes uncompressed, 24771 bytes compressed:  74.9%
```

## zipnote {}

```diff
@@ -36,23 +36,23 @@
 
 Filename: chiakilisp/proxies/__init__.py
 Comment: 
 
 Filename: chiakilisp/proxies/keyword.py
 Comment: 
 
-Filename: chiakilisp-1.4.0rc6.data/scripts/chiakilang
+Filename: chiakilisp-1.4.0rc7.data/scripts/chiakilang
 Comment: 
 
-Filename: chiakilisp-1.4.0rc6.dist-info/METADATA
+Filename: chiakilisp-1.4.0rc7.dist-info/METADATA
 Comment: 
 
-Filename: chiakilisp-1.4.0rc6.dist-info/WHEEL
+Filename: chiakilisp-1.4.0rc7.dist-info/WHEEL
 Comment: 
 
-Filename: chiakilisp-1.4.0rc6.dist-info/top_level.txt
+Filename: chiakilisp-1.4.0rc7.dist-info/top_level.txt
 Comment: 
 
-Filename: chiakilisp-1.4.0rc6.dist-info/RECORD
+Filename: chiakilisp-1.4.0rc7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## chiakilisp/lexer.py

```diff
@@ -61,315 +61,318 @@
 
         return tuple((self._source_code_file_name, self._line_num, self._char_num))
 
     def lex(self) -> None:  # pylint: disable=R0912, disable=R0915  # maybe refactor
 
         """Process the given source code, thus produces a list of Token instances"""
 
-        while self._has_next_symbol():
+        while self._can_be_advanced():
 
-            if self._current_symbol_is_semicolon() or \
-                    (self._current_symbol_is_hash() and
-                        self._next_symbol_is_exclamation_mark()):
+            if self._current_char_is_semicolon() or \
+                    (self._current_char_is_hash() and
+                        self._next_char_is_exclamation_mark()):
                 self._advance()
-                while self._has_next_symbol():
-                    if self._current_symbol_is_nl():
+                while self._can_be_advanced():
+                    if self._current_char_is_nl():
                         break
                     self._advance()
                 self._advance()
                 self._increment_line_number_with_char_number_reset()
 
-            elif (self._current_symbol_is_hash()
-                    and self._next_symbol_is_opening_paren()):
+            elif (self._current_char_is_hash()
+                  and self._next_char_is_opening_paren()):
                 self._advance()
                 self._increment_char_number()
                 self._tokens.append(Token(Token.InlineFunMarker,  '#{', self.pos()))
 
-            elif (self._current_symbol_is_hash()
-                    and self._next_symbol_is_underscore()):
+            elif (self._current_char_is_hash()
+                  and self._next_char_is_underscore()):
                 self._advance()
                 self._advance()
                 self._increment_char_number()
                 self._increment_char_number()
                 self._tokens.append(Token(Token.CommentedMarker,  '#_', self.pos()))
 
-            elif (self._current_symbol_is_hash()
-                    and self._next_symbol_is_cr_opening_paren()):
+            elif (self._current_char_is_hash()
+                  and self._next_char_is_cr_opening_paren()):
                 self._advance()
                 self._increment_char_number()  # <-- increment character num as well
                 self._tokens.append(Token(Token.OpeningParen,      '(', self.pos()))
                 self._tokens.append(Token(Token.Identifier,    'setty', self.pos()))
                 self._advance()
                 self._increment_char_number()  # <-- increment character num as well
 
-            elif (self._current_symbol_is_hash()
-                  and self._next_symbol_is_sq_opening_paren()):
+            elif (self._current_char_is_hash()
+                  and self._next_char_is_sq_opening_paren()):
                 self._advance()
                 self._increment_char_number()  # <-- increment character num as well
                 self._tokens.append(Token(Token.OpeningParen,     '(', self.pos()))
                 self._tokens.append(Token(Token.Identifier,   'tuply', self.pos()))
                 self._advance()
                 self._increment_char_number()  # <-- increment character num as well
 
-            elif self._current_symbol_is_number() \
-                    or (self._current_symbol_is_sign()
-                        and self._next_symbol_is_number()):
-                value = self._current_symbol()
+            elif self._current_char_is_number() \
+                    or (self._current_char_is_sign()
+                        and self._next_char_is_number()):
+                value = self._current_char()
                 self._advance()
                 self._increment_char_number()
-                while self._has_next_symbol():
-                    if self._current_symbol_is_number() \
-                            or self._current_symbol_is_dot():
-                        value += self._current_symbol()
+                while self._can_be_advanced():
+                    if self._current_char_is_number() \
+                            or self._current_char_is_dot():
+                        value += self._current_char()
                         self._advance()
                         self._increment_char_number()
                     else:
                         break
                 if re.match(r'^\d+?\.{2}(\d+)?$', value):
                     self._tokens.append(Token(Token.Slice, value, self.pos()))
                 elif re.match(r'^(-)?\d+(\.\d+)?$', value):
                     self._tokens.append(Token(Token.Number, value, self.pos()))
                 else:
                     self._raise_syntax_error(f'Invalid float syntax: {value}.')
 
-            elif self._current_symbol_is_letter() \
-                    or self._current_symbol_is_colon():
-                value = self._current_symbol()
+            elif self._current_char_is_letter() \
+                    or self._current_char_is_colon():
+                value = self._current_char()
                 self._advance()
                 self._increment_char_number()
-                while self._has_next_symbol():
-                    if self._current_symbol_is_letter() or \
-                            self._current_symbol_is_number():
-                        value += self._current_symbol()
+                while self._can_be_advanced():
+                    if self._current_char_is_letter() or \
+                            self._current_char_is_number():
+                        value += self._current_char()
                         self._advance()
                         self._increment_char_number()
                     else:
                         break
                 if re.match(r'^\.\d+$', value):
                     value = '0' + value  # make it possible to define 0.2 as .2
                     self._tokens.append(Token(Token.Number, value, self.pos()))
+                elif re.match(r'^-\.\d+$', value):
+                    value = '-0' + value[1:]  # make it possible to prepend '-'
+                    self._tokens.append(Token(Token.Number, value, self.pos()))
                 elif value.startswith(':'):
                     self._tokens.append(Token(Token.Keyword, value, self.pos()))
                 elif value == 'nil':
                     self._tokens.append(Token(Token.Nil, value, self.pos()))
                 elif value in ['true', 'false']:
                     self._tokens.append(Token(Token.Boolean, value, self.pos()))
                 elif re.match(r'^\.{2}\d+$', value):  # make it equivalent for 0..2
                     self._tokens.append(Token(Token.Slice, value, self.pos()))
                 else:
                     self._tokens.append(Token(Token.Identifier, value, self.pos()))
 
-            elif self._current_symbol_is_double_quote():
+            elif self._current_char_is_double_quote():
                 value = ''
-                while self._has_next_symbol():
+                while self._can_be_advanced():
                     self._advance()
                     self._increment_char_number()
-                    if self._current_symbol() == '\\':
+                    if self._current_char() == '\\':
                         self._advance()
                         self._increment_char_number()
-                        if self._current_symbol() == 'n':
+                        if self._current_char() == 'n':
                             value += '\n'
-                        if self._current_symbol() == 't':
+                        if self._current_char() == 't':
                             value += '\t'
-                        if self._current_symbol_is_double_quote():
+                        if self._current_char_is_double_quote():
                             value += '"'
                         continue
-                    if not self._current_symbol_is_double_quote():
-                        value += self._current_symbol()
+                    if not self._current_char_is_double_quote():
+                        value += self._current_char()
                     else:
                         self._tokens.append(Token(Token.String, value,  self.pos()))
                         break
                 self._advance()  # <--- call _advance() to skip the leading '"' char
                 self._increment_char_number()  # <-- increment character num as well
 
-            elif self._current_symbol_is_opening_paren():
+            elif self._current_char_is_opening_paren():
                 self._tokens.append(Token(Token.OpeningParen,      '(', self.pos()))
                 self._advance()
                 self._increment_char_number()  # <-- increment character num as well
 
-            elif self._current_symbol_is_closing_paren():
+            elif self._current_char_is_closing_paren():
                 self._tokens.append(Token(Token.ClosingParen,      ')', self.pos()))
                 self._advance()
                 self._increment_char_number()  # <-- increment character num as well
 
-            elif self._current_symbol_is_cr_opening_paren():
+            elif self._current_char_is_cr_opening_paren():
                 self._tokens.append(Token(Token.OpeningParen,      '(', self.pos()))
                 self._tokens.append(Token(Token.Identifier,    'dicty', self.pos()))
                 self._advance()
                 self._increment_char_number()  # <-- increment character num as well
 
-            elif self._current_symbol_is_cr_closing_paren():
+            elif self._current_char_is_cr_closing_paren():
                 self._tokens.append(Token(Token.ClosingParen,      ')', self.pos()))
                 self._advance()
                 self._increment_char_number()  # <-- increment character num as well
 
-            elif self._current_symbol_is_sq_opening_paren():
+            elif self._current_char_is_sq_opening_paren():
                 self._tokens.append(Token(Token.OpeningParen,      '(', self.pos()))
                 self._tokens.append(Token(Token.Identifier,    'listy', self.pos()))
                 self._advance()
                 self._increment_char_number()  # <-- increment character num as well
 
-            elif self._current_symbol_is_sq_closing_paren():
+            elif self._current_char_is_sq_closing_paren():
                 self._tokens.append(Token(Token.ClosingParen,      ')', self.pos()))
                 self._advance()
                 self._increment_char_number()  # <-- increment character num as well
 
-            elif self._current_symbol_is_nl():
+            elif self._current_char_is_nl():
                 self._advance()
                 self._increment_line_number_with_char_number_reset()  # go a newline
 
             else:
                 self._advance()  # call _advance() to skip over the extra characters
                 self._increment_char_number()  # <-- increment character num as well
 
     def _advance(self) -> None:
 
-        """Advance the pointer"""
+        """Advances char pointer"""
 
         self._pointer += 1
 
-    def _current_symbol(self) -> str:
+    def _current_char(self) -> str:
 
-        """Returns the current symbol"""
+        """Returns a current character"""
 
         return self._source_code[self._pointer]
 
-    def _next_symbol(self) -> str:
+    def _next_char(self) -> str:
 
-        """Returns the next symbol (if possible, otherwise '')"""
+        """Returns a next character if possible, otherwise ''"""
 
         if (len(self._source_code) == 1 and not self._pointer) \
-                or not self._has_next_symbol():
+                or not self._can_be_advanced():
             return ''
         return self._source_code[self._pointer + 1]
 
-    def _has_next_symbol(self) -> bool:
+    def _can_be_advanced(self) -> bool:
 
-        """Returns whether source has next symbol"""
+        """Whether source has a next character"""
 
         return self._pointer < len(self._source_code)
 
-    def _current_symbol_is_nl(self) -> bool:
+    def _current_char_is_nl(self) -> bool:
 
-        """Returns whether current symbol is a newline symbol"""
+        """Returns whether current character is a newline character"""
 
-        return self._current_symbol() == '\n'
+        return self._current_char() == '\n'
 
-    def _current_symbol_is_sign(self) -> bool:
+    def _current_char_is_sign(self) -> bool:
 
-        """Returns whether current symbol is a number sign"""
+        """Returns whether current character is a number sign: +, -"""
 
-        return self._current_symbol() in ['+', '-']
+        return self._current_char() in ['+', '-']
 
-    def _current_symbol_is_hash(self) -> bool:
+    def _current_char_is_hash(self) -> bool:
 
-        """Returns whether current symbol is a hashtag symbol"""
+        """Returns whether current character is a hashtag character"""
 
-        return self._current_symbol() == '#'
+        return self._current_char() == '#'
 
-    def _current_symbol_is_dot(self) -> bool:
+    def _current_char_is_dot(self) -> bool:
 
-        """Returns whether current symbol is a dot symbol"""
+        """Returns whether current character is a dot character"""
 
-        return self._current_symbol() == '.'
+        return self._current_char() == '.'
 
-    def _current_symbol_is_colon(self) -> bool:
+    def _current_char_is_colon(self) -> bool:
 
-        """Returns whether current symbol is a colon symbol"""
+        """Returns whether current character is a colon character"""
 
-        return self._current_symbol() == ':'
+        return self._current_char() == ':'
 
-    def _current_symbol_is_semicolon(self) -> bool:
+    def _current_char_is_semicolon(self) -> bool:
 
-        """Returns whether current symbol is a semicolon symbol"""
+        """Returns whether current character is a semicolon character"""
 
-        return self._current_symbol() == ';'
+        return self._current_char() == ';'
 
-    def _current_symbol_is_double_quote(self) -> bool:
+    def _current_char_is_double_quote(self) -> bool:
 
-        """Returns whether current symbol is a double-quote symbol"""
+        """Returns whether current character is a double-quote character"""
 
-        return self._current_symbol() == '"'
+        return self._current_char() == '"'
 
-    def _current_symbol_is_opening_paren(self) -> bool:
+    def _current_char_is_opening_paren(self) -> bool:
 
-        """Returns whether current symbol is an opening paren symbol"""
+        """Returns whether current character is an opening paren character"""
 
-        return self._current_symbol() == '('
+        return self._current_char() == '('
 
-    def _current_symbol_is_closing_paren(self) -> bool:
+    def _current_char_is_closing_paren(self) -> bool:
 
-        """Returns whether current symbol is a closing paren symbol"""
+        """Returns whether current character is a closing paren character"""
 
-        return self._current_symbol() == ')'
+        return self._current_char() == ')'
 
-    def _current_symbol_is_cr_opening_paren(self) -> bool:
+    def _current_char_is_cr_opening_paren(self) -> bool:
 
-        """Returns whether current symbol is a curly-opening paren symbol"""
+        """Returns whether current character is a curly-opening paren character"""
 
-        return self._current_symbol() == '{'
+        return self._current_char() == '{'
 
-    def _current_symbol_is_cr_closing_paren(self) -> bool:
+    def _current_char_is_cr_closing_paren(self) -> bool:
 
-        """Returns whether current symbol is a curly-closing paren symbol"""
+        """Returns whether current character is a curly-closing paren character"""
 
-        return self._current_symbol() == '}'
+        return self._current_char() == '}'
 
-    def _current_symbol_is_sq_opening_paren(self) -> bool:
+    def _current_char_is_sq_opening_paren(self) -> bool:
 
-        """Returns whether current symbol is a square-opening paren symbol"""
+        """Returns whether current character is a square-opening paren character"""
 
-        return self._current_symbol() == '['
+        return self._current_char() == '['
 
-    def _current_symbol_is_sq_closing_paren(self) -> bool:
+    def _current_char_is_sq_closing_paren(self) -> bool:
 
-        """Returns whether current symbol is a square-closing paren symbol"""
+        """Returns whether current character is a square-closing paren character"""
 
-        return self._current_symbol() == ']'
+        return self._current_char() == ']'
 
-    def _next_symbol_is_number(self) -> bool:
+    def _next_char_is_number(self) -> bool:
 
-        """Returns whether next symbol is a number, valid number is from 0 to 9"""
+        """Returns whether next symbol is a character, valid number is from 0 to 9"""
 
-        return re.match(r'\d', self._next_symbol()) is not None
+        return re.match(r'\d', self._next_char()) is not None
 
-    def _next_symbol_is_exclamation_mark(self) -> bool:
+    def _next_char_is_exclamation_mark(self) -> bool:
 
-        """Returns whether next symbol is an exclamation mark symbol"""
+        """Returns whether next character is an exclamation mark character"""
 
-        return self._next_symbol() == '!'
+        return self._next_char() == '!'
 
-    def _next_symbol_is_opening_paren(self) -> bool:
+    def _next_char_is_opening_paren(self) -> bool:
 
-        """Returns whether next symbol is an opening paren symbol"""
+        """Returns whether next character is an opening paren character"""
 
-        return self._next_symbol() == '('
+        return self._next_char() == '('
 
-    def _next_symbol_is_underscore(self) -> bool:
+    def _next_char_is_underscore(self) -> bool:
 
-        """Returns whether next symbol is an underscore symbol"""
+        """Returns whether next character is an underscore character"""
 
-        return self._next_symbol() == '_'
+        return self._next_char() == '_'
 
-    def _next_symbol_is_cr_opening_paren(self) -> bool:
+    def _next_char_is_cr_opening_paren(self) -> bool:
 
-        """Returns whether next symbol is a curly-opening paren symbol"""
+        """Returns whether next character is a curly-opening paren character"""
 
-        return self._next_symbol() == '{'
+        return self._next_char() == '{'
 
-    def _next_symbol_is_sq_opening_paren(self) -> bool:
+    def _next_char_is_sq_opening_paren(self) -> bool:
 
-        """Returns whether next symbol is a square-opening paren symbol"""
+        """Returns whether next character is a square-opening paren character"""
 
-        return self._next_symbol() == '['
+        return self._next_char() == '['
 
-    def _current_symbol_is_number(self) -> bool:
+    def _current_char_is_number(self) -> bool:
 
-        """Returns whether current symbol is a number, valid number is from 0 to 9"""
+        """Returns whether current character is a number, valid number is from 0 to 9"""
 
-        return re.match(r'\d', self._current_symbol()) is not None
+        return re.match(r'\d', self._current_char()) is not None
 
-    def _current_symbol_is_letter(self) -> bool:
+    def _current_char_is_letter(self) -> bool:
 
-        """Returns whether current symbol is a letter: valid letter is from a-zA-Z or from the alphabet"""
+        """Returns whether current character is a letter: valid letter is from a-zA-Z or from ALPHABET"""
 
-        return re.match(r'[a-zA-Z]', self._current_symbol()) is not None or self._current_symbol() in ALPHABET
+        return re.match(r'[a-zA-Z]', self._current_char()) is not None or self._current_char() in ALPHABET
```

## chiakilisp/corelib/core.cl

```diff
@@ -116,15 +116,15 @@
   (get coll 2)))
 (defn last (coll)                 ;; Returns the last collection item
  (when (or (list? coll) (tuple? coll) (str? coll))
   (get coll -1))))
 
 (defn rest (coll)                 ;; Returns the rest of a collection
  (when (and coll (or (str? coll) (list? coll) (tuple? coll)))
-  (get coll (slice 1..))))        ;; this one is equivalent for: [1:]
+  (get coll 1..)))                ;; this one is equivalent for: [1:]
 
 (defn get-in (& args)        ;; Goes through full path to get an item
  (when args
   (let ((coll path default) args)
         (cond (>= (count args) 2)
               (functools/reduce (fn (acc n)
                                   (get acc n default)) path coll)))))
```

## Comparing `chiakilisp-1.4.0rc6.data/scripts/chiakilang` & `chiakilisp-1.4.0rc7.data/scripts/chiakilang`

 * *Files identical despite different names*

## Comparing `chiakilisp-1.4.0rc6.dist-info/METADATA` & `chiakilisp-1.4.0rc7.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chiakilisp
-Version: 1.4.0rc6
+Version: 1.4.0rc7
 Summary: ChiakiLisp - Yet another LISP
 Home-page: https://chiakilisp.jedi2light.moe
 Author: @jedi2light
 Author-email: jedi2light@jedi2light.moe
 Maintainer: @jedi2light
 Maintainer-email: jedi2light@jedi2light.moe
 License: WTFPL
```

## Comparing `chiakilisp-1.4.0rc6.dist-info/RECORD` & `chiakilisp-1.4.0rc7.dist-info/RECORD`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 chiakilisp/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-chiakilisp/lexer.py,sha256=6zSmOLVskcHKqGFGImXKYdLjthT-OxBXKqE0kU0FuhQ,14401
+chiakilisp/lexer.py,sha256=7f7q6iWpjkh8NIogYnRa4Ea2YVJsVZwl7WyjP_cWIQs,14553
 chiakilisp/parser.py,sha256=aPAa3U8D28DO15NzwUliLTOZeCaQEu5giOpzCnPBSs8,5943
 chiakilisp/runtime.py,sha256=J69abrFy4RdcA6oU9z2Pv4ok4A7h5X8lR9VM1l28kk4,1378
 chiakilisp/spec.py,sha256=4_hvO1HYm3RGnky1q85q72we1L3wpjufDgoVU_kcTwk,11225
 chiakilisp/utils.py,sha256=lYwdSJY_y5QEBAM9rEd02Z9ra9ZADJ_yO8JIfsS2WAM,3311
-chiakilisp/corelib/core.cl,sha256=YaxdnBJt0U7ebyXvIK2gE4KR5TGOAiPksy6PYhqatBg,7391
+chiakilisp/corelib/core.cl,sha256=dzLuHsn9URABl8Sj-XHLweHsj-tntjuPl8O2m2Emoy8,7391
 chiakilisp/models/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 chiakilisp/models/expression.py,sha256=T2R6S3pMAJxmcrjbmxueyDfzAUE8aOzbTutNV-451y4,31150
 chiakilisp/models/forward.py,sha256=ykZjLoXxONjvoCZ3h2itUieAFteh5TUiAuk4f8NoiZs,790
 chiakilisp/models/literal.py,sha256=Dg5tqdDWzuaW0NvxtZpHP9CQAvTDDjB4eJGMFuxWImc,4001
 chiakilisp/models/token.py,sha256=1ks0qk_t-V-EaLu_LhjEeHx2hrPa_bbyIsqHxdFeAeU,2123
 chiakilisp/proxies/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 chiakilisp/proxies/keyword.py,sha256=fMVWpRxk_Sk_6CXE08IFnFTtMbvhadUSe2IYgin_h60,205
-chiakilisp-1.4.0rc6.data/scripts/chiakilang,sha256=-vbv8w6RFangekz5zoX-FBDYFabYX_Ad4VvvPD8Hvro,13359
-chiakilisp-1.4.0rc6.dist-info/METADATA,sha256=Mj9euCLkCwew08v61lxVPCKZqdLUSsJOtRIVcOXzBgw,1408
-chiakilisp-1.4.0rc6.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-chiakilisp-1.4.0rc6.dist-info/top_level.txt,sha256=uV87HteR3vUsfEm7HlxKG0Fh7zkoke2RetMtgLu97Bc,11
-chiakilisp-1.4.0rc6.dist-info/RECORD,,
+chiakilisp-1.4.0rc7.data/scripts/chiakilang,sha256=-vbv8w6RFangekz5zoX-FBDYFabYX_Ad4VvvPD8Hvro,13359
+chiakilisp-1.4.0rc7.dist-info/METADATA,sha256=qhhwNsZeOFcXAZnK5d736xYmTcPskYWjvW1H4nXfZVc,1408
+chiakilisp-1.4.0rc7.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+chiakilisp-1.4.0rc7.dist-info/top_level.txt,sha256=uV87HteR3vUsfEm7HlxKG0Fh7zkoke2RetMtgLu97Bc,11
+chiakilisp-1.4.0rc7.dist-info/RECORD,,
```

