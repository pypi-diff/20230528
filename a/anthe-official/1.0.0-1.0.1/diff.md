# Comparing `tmp/anthe_official-1.0.0.tar.gz` & `tmp/anthe_official-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anthe_official-1.0.0.tar", last modified: Thu May 25 11:53:01 2023, max compression
+gzip compressed data, was "anthe_official-1.0.1.tar", last modified: Sun May 28 17:15:30 2023, max compression
```

## Comparing `anthe_official-1.0.0.tar` & `anthe_official-1.0.1.tar`

### file list

```diff
@@ -1,17 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-05-25 11:53:01.207143 anthe_official-1.0.0/
--rw-rw-rw-   0        0        0     2888 2023-05-25 11:53:01.206147 anthe_official-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     2341 2023-05-25 11:50:21.000000 anthe_official-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-25 11:53:01.175151 anthe_official-1.0.0/anthe_official.egg-info/
--rw-rw-rw-   0        0        0     2888 2023-05-25 11:53:01.000000 anthe_official-1.0.0/anthe_official.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      356 2023-05-25 11:53:01.000000 anthe_official-1.0.0/anthe_official.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-25 11:53:01.000000 anthe_official-1.0.0/anthe_official.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      133 2023-05-25 11:53:01.000000 anthe_official-1.0.0/anthe_official.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-05-25 11:53:01.000000 anthe_official-1.0.0/anthe_official.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-25 11:53:01.203148 anthe_official-1.0.0/neural_models/
--rw-rw-rw-   0        0        0      433 2023-05-25 08:40:52.000000 anthe_official-1.0.0/neural_models/__init__.py
--rw-rw-rw-   0        0        0     4871 2023-05-25 11:12:08.000000 anthe_official-1.0.0/neural_models/attentions.py
--rw-rw-rw-   0        0        0      329 2023-05-20 17:11:12.000000 anthe_official-1.0.0/neural_models/helper_layers.py
--rw-rw-rw-   0        0        0     8334 2023-05-25 11:12:08.000000 anthe_official-1.0.0/neural_models/special_embedding.py
--rw-rw-rw-   0        0        0    11827 2023-05-25 11:12:07.000000 anthe_official-1.0.0/neural_models/transformer.py
--rw-rw-rw-   0        0        0       42 2023-05-25 11:53:01.208146 anthe_official-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1039 2023-05-25 11:52:29.000000 anthe_official-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-28 17:15:30.443143 anthe_official-1.0.1/
+-rw-rw-rw-   0        0        0     2922 2023-05-28 17:15:30.442143 anthe_official-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2375 2023-05-28 17:11:58.000000 anthe_official-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-28 17:15:30.421140 anthe_official-1.0.1/anthe_official.egg-info/
+-rw-rw-rw-   0        0        0     2922 2023-05-28 17:15:30.000000 anthe_official-1.0.1/anthe_official.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      535 2023-05-28 17:15:30.000000 anthe_official-1.0.1/anthe_official.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-28 17:15:30.000000 anthe_official-1.0.1/anthe_official.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      133 2023-05-28 17:15:30.000000 anthe_official-1.0.1/anthe_official.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       34 2023-05-28 17:15:30.000000 anthe_official-1.0.1/anthe_official.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-28 17:15:30.431138 anthe_official-1.0.1/neural_models_pt/
+-rw-rw-rw-   0        0        0      454 2023-05-28 16:53:00.000000 anthe_official-1.0.1/neural_models_pt/__init__.py
+-rw-rw-rw-   0        0        0     4075 2023-05-28 16:39:48.000000 anthe_official-1.0.1/neural_models_pt/attentions.py
+-rw-rw-rw-   0        0        0      327 2023-05-28 16:42:41.000000 anthe_official-1.0.1/neural_models_pt/helper_layers.py
+-rw-rw-rw-   0        0        0     5357 2023-05-28 16:53:00.000000 anthe_official-1.0.1/neural_models_pt/special_embedding.py
+-rw-rw-rw-   0        0        0    11265 2023-05-28 17:06:11.000000 anthe_official-1.0.1/neural_models_pt/transformer.py
+drwxrwxrwx   0        0        0        0 2023-05-28 17:15:30.441151 anthe_official-1.0.1/neural_models_tf/
+-rw-rw-rw-   0        0        0      454 2023-05-28 16:34:00.000000 anthe_official-1.0.1/neural_models_tf/__init__.py
+-rw-rw-rw-   0        0        0     4864 2023-05-28 16:33:52.000000 anthe_official-1.0.1/neural_models_tf/attentions.py
+-rw-rw-rw-   0        0        0      329 2023-05-20 17:11:12.000000 anthe_official-1.0.1/neural_models_tf/helper_layers.py
+-rw-rw-rw-   0        0        0     8963 2023-05-28 16:50:18.000000 anthe_official-1.0.1/neural_models_tf/special_embedding.py
+-rw-rw-rw-   0        0        0    11707 2023-05-28 17:03:21.000000 anthe_official-1.0.1/neural_models_tf/transformer.py
+-rw-rw-rw-   0        0        0       42 2023-05-28 17:15:30.444142 anthe_official-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1039 2023-05-28 17:14:29.000000 anthe_official-1.0.1/setup.py
```

### Comparing `anthe_official-1.0.0/PKG-INFO` & `anthe_official-1.0.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anthe_official
-Version: 1.0.0
+Version: 1.0.1
 Summary: Anthe improves performance of Transformers with less parameters.
 Author: Luca Herranz-Celotti, Ermal Rrapaj
 Author-email: luca.herrtti@gmail.com
 License: Apache License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: MIT License
@@ -20,23 +20,23 @@
 To run the experiments run the ```train.py``` file. If you want to activate the Transformer architecture, pass the
 argument ```--comments=sameemb_projectoutput```. If you want to activate the Anthe architecture, pass the argument
 ```--comments=geglu_gateattention_hsoftpos:2_tcffn:.005_tcpreatt:.07_tclength:2```. By default it will use
 the WMT14 dataset. If you want to use the WMT17 add the following text to the comments argument:
 ```--comments=..._lpair:cs-en```, where the available
 language pairs are cs-en, de-en, fi-en, lv-en, ru-en, tr-en, zh-en.
 
-You can install it as a package with ```pip install anthe_official```.
+You can install it as a package with ```pip install anthe-official```.
 
 ## Layers Available
 
 The following layers are available for the Anthe architecture, only in TensorFlow 2.10.0 for now. 
 You can access the Anthe architecture, the AntheEncoderBlock and the AntheDecoderBlock, like so:
 
 ```python
-from anthe_official import Anthe, AntheEncoderBlock, AntheDecoderBlock
+from anthe_official.neural_models_tf import Anthe, AntheEncoderBlock, AntheDecoderBlock
 
 model = Anthe(
     inputs_vocab_size, target_vocab_size, encoder_count, decoder_count, attention_head_count,
     d_model, d_point_wise_ff, dropout_prob
 )
 
 encoder_block = AntheEncoderBlock(
@@ -50,15 +50,15 @@
 
 In the article we develop other layers that are part of the Anthe architecture, but might be of interest
 on their own.
 The TC versions of the Dense, Conv1D and Embedding,
 and the SoftPOS and the HSoftPOS, can be accessed like so:
 
 ```python
-from anthe_official import *
+from anthe_official.neural_models_tf import *
 
 tc_dense = TCDense(d_model, length=3, ratio=.2)
 tc_conv1d = TCConv1D(filters, kernel_size, tc_length=3, ratio=.2)
 tc_embedding = TCEmbedding(input_dim, output_dim, tc_length=3, ratio=.2)
 
 soft_pos = SoftPOS(add_units, n_subpos=add_units, repeat_subpos=1)
 hsoft_pos = HSoftPOS(vocab_size, embed_dim)
```

### Comparing `anthe_official-1.0.0/README.md` & `anthe_official-1.0.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -7,23 +7,23 @@
 To run the experiments run the ```train.py``` file. If you want to activate the Transformer architecture, pass the
 argument ```--comments=sameemb_projectoutput```. If you want to activate the Anthe architecture, pass the argument
 ```--comments=geglu_gateattention_hsoftpos:2_tcffn:.005_tcpreatt:.07_tclength:2```. By default it will use
 the WMT14 dataset. If you want to use the WMT17 add the following text to the comments argument:
 ```--comments=..._lpair:cs-en```, where the available
 language pairs are cs-en, de-en, fi-en, lv-en, ru-en, tr-en, zh-en.
 
-You can install it as a package with ```pip install anthe_official```.
+You can install it as a package with ```pip install anthe-official```.
 
 ## Layers Available
 
 The following layers are available for the Anthe architecture, only in TensorFlow 2.10.0 for now. 
 You can access the Anthe architecture, the AntheEncoderBlock and the AntheDecoderBlock, like so:
 
 ```python
-from anthe_official import Anthe, AntheEncoderBlock, AntheDecoderBlock
+from anthe_official.neural_models_tf import Anthe, AntheEncoderBlock, AntheDecoderBlock
 
 model = Anthe(
     inputs_vocab_size, target_vocab_size, encoder_count, decoder_count, attention_head_count,
     d_model, d_point_wise_ff, dropout_prob
 )
 
 encoder_block = AntheEncoderBlock(
@@ -37,15 +37,15 @@
 
 In the article we develop other layers that are part of the Anthe architecture, but might be of interest
 on their own.
 The TC versions of the Dense, Conv1D and Embedding,
 and the SoftPOS and the HSoftPOS, can be accessed like so:
 
 ```python
-from anthe_official import *
+from anthe_official.neural_models_tf import *
 
 tc_dense = TCDense(d_model, length=3, ratio=.2)
 tc_conv1d = TCConv1D(filters, kernel_size, tc_length=3, ratio=.2)
 tc_embedding = TCEmbedding(input_dim, output_dim, tc_length=3, ratio=.2)
 
 soft_pos = SoftPOS(add_units, n_subpos=add_units, repeat_subpos=1)
 hsoft_pos = HSoftPOS(vocab_size, embed_dim)
```

### Comparing `anthe_official-1.0.0/anthe_official.egg-info/PKG-INFO` & `anthe_official-1.0.1/anthe_official.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anthe-official
-Version: 1.0.0
+Version: 1.0.1
 Summary: Anthe improves performance of Transformers with less parameters.
 Author: Luca Herranz-Celotti, Ermal Rrapaj
 Author-email: luca.herrtti@gmail.com
 License: Apache License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: MIT License
@@ -20,23 +20,23 @@
 To run the experiments run the ```train.py``` file. If you want to activate the Transformer architecture, pass the
 argument ```--comments=sameemb_projectoutput```. If you want to activate the Anthe architecture, pass the argument
 ```--comments=geglu_gateattention_hsoftpos:2_tcffn:.005_tcpreatt:.07_tclength:2```. By default it will use
 the WMT14 dataset. If you want to use the WMT17 add the following text to the comments argument:
 ```--comments=..._lpair:cs-en```, where the available
 language pairs are cs-en, de-en, fi-en, lv-en, ru-en, tr-en, zh-en.
 
-You can install it as a package with ```pip install anthe_official```.
+You can install it as a package with ```pip install anthe-official```.
 
 ## Layers Available
 
 The following layers are available for the Anthe architecture, only in TensorFlow 2.10.0 for now. 
 You can access the Anthe architecture, the AntheEncoderBlock and the AntheDecoderBlock, like so:
 
 ```python
-from anthe_official import Anthe, AntheEncoderBlock, AntheDecoderBlock
+from anthe_official.neural_models_tf import Anthe, AntheEncoderBlock, AntheDecoderBlock
 
 model = Anthe(
     inputs_vocab_size, target_vocab_size, encoder_count, decoder_count, attention_head_count,
     d_model, d_point_wise_ff, dropout_prob
 )
 
 encoder_block = AntheEncoderBlock(
@@ -50,15 +50,15 @@
 
 In the article we develop other layers that are part of the Anthe architecture, but might be of interest
 on their own.
 The TC versions of the Dense, Conv1D and Embedding,
 and the SoftPOS and the HSoftPOS, can be accessed like so:
 
 ```python
-from anthe_official import *
+from anthe_official.neural_models_tf import *
 
 tc_dense = TCDense(d_model, length=3, ratio=.2)
 tc_conv1d = TCConv1D(filters, kernel_size, tc_length=3, ratio=.2)
 tc_embedding = TCEmbedding(input_dim, output_dim, tc_length=3, ratio=.2)
 
 soft_pos = SoftPOS(add_units, n_subpos=add_units, repeat_subpos=1)
 hsoft_pos = HSoftPOS(vocab_size, embed_dim)
```

### Comparing `anthe_official-1.0.0/neural_models/attentions.py` & `anthe_official-1.0.1/neural_models_tf/attentions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 import numpy as np
 import tensorflow as tf
 
 from pyaromatics.stay_organized.utils import str2val
-from anthe_official.neural_models.tensor_chain.dense import TCDense
+from anthe_official.neural_models_tf.tensor_chain.dense import TCDense
 
 
 class ScaledDotProductAttention(tf.keras.layers.Layer):
     def __init__(self, d_h):
         super().__init__()
         self.d_h = d_h
         self.softmax = tf.nn.softmax
@@ -72,15 +72,15 @@
             w_key = tf.keras.layers.Dense(d_model)
             w_value = tf.keras.layers.Dense(d_model)
 
         self.w_query = w_query
         self.w_key = w_key
         self.w_value = w_value
 
-        self.scaled_dot_product = ScaledDotProductAttention(self.d_h, comments)
+        self.scaled_dot_product = ScaledDotProductAttention(self.d_h)
         self.ff = tf.keras.layers.Dense(d_model)
 
         self.d_model = d_model
 
         qkv_order = str2val(comments, 'gateattention', str, default='kqv')
         assert all([k in qkv_order for k in 'qkv'])
```

### Comparing `anthe_official-1.0.0/neural_models/special_embedding.py` & `anthe_official-1.0.1/neural_models_tf/special_embedding.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import tensorflow as tf
 from pyaromatics.stay_organized.utils import str2val
-from anthe_official.neural_models.tensor_chain.convolutions import TCConv1D
+from anthe_official.neural_models_tf.tensor_chain.convolutions import TCConv1D
 
-from anthe_official.neural_models.tensor_chain.embedding import TCEmbedding
+from anthe_official.neural_models_tf.tensor_chain.embedding import TCEmbedding
 
 
 def positional_encoding(max_len, d_model):
     depth = d_model / 2
 
     positions = tf.expand_dims(tf.range(max_len), 1)  # (seq, 1)
     depths = tf.expand_dims(tf.range(depth) / depth, 0)  # (1, depth)
@@ -23,15 +23,15 @@
 
 
 def angle(pos, index, d_model):
     pos = tf.cast(pos, tf.float32)
     return pos / tf.pow(10000., tf.cast((index - index % 2) / d_model, tf.float32))
 
 
-class Embeddinglayer(tf.keras.layers.Layer):
+class EmbeddingLayer(tf.keras.layers.Layer):
     def __init__(self, vocab_size, d_model, **kwargs):
         # model hyper parameter variables
         super().__init__(**kwargs)
         self.vocab_size = vocab_size
         self.d_model = d_model
 
         self.embedding = tf.keras.layers.Embedding(vocab_size, d_model)
@@ -44,37 +44,29 @@
         pos = positional_encoding(max_sequence_len, self.d_model)
 
         output = output + pos
 
         return output
 
 
-def positional_emb(emb, max_sequence_len, d_model):
-    # max_sequence_len = sequences.shape[1]
-    output = emb * tf.sqrt(tf.cast(d_model, dtype=tf.float32))
-    output += positional_encoding(max_sequence_len, d_model)
-
-    return output
-
-
 class SoftPOS(tf.keras.layers.Layer):
     def __init__(self, add_units, n_subpos=3, repeat_subpos=2, initializer='orthogonal', **kwargs):
         super().__init__(**kwargs)
 
         self.add_units = add_units
         self.n_subpos = n_subpos
         self.repeat_subpos = repeat_subpos
         self.initializer = initializer
 
     def build(self, input_shape):
         if self.n_subpos > 0:
             self.spos = []
             for i in range(self.repeat_subpos):
                 spos = self.add_weight(
-                    f"spos_{i}", shape=[self.n_subpos, self.units], dtype="float32",
+                    f"spos_{i}", shape=[self.n_subpos, self.add_units], dtype="float32",
                     initializer=self.initializer
                 )
                 self.spos.append(spos)
 
     def call(self, inputs):
         x = inputs
         emb = x
@@ -93,37 +85,39 @@
         }
 
         base_config = super().get_config()
         return dict(list(base_config.items()) + list(config.items()))
 
 
 class HSoftPOS(tf.keras.layers.Layer):
-    def __init__(self, vocab_size, embed_dim, n_layers=2, tcemb=False, tcconv=False, tcr=.2, tclength=2, **kwargs):
+    def __init__(self, vocab_size, embed_dim, n_layers=2, tcembr=None, tcconvr=None, tclength=2, **kwargs):
         super().__init__(**kwargs)
 
+        assert tcembr is None or isinstance(tcembr, float)
+        assert tcconvr is None or isinstance(tcconvr, float)
+
         self.vocab_size = vocab_size
         self.embed_dim = embed_dim
         self.n_layers = n_layers
-        self.tcemb = tcemb
-        self.tcconv = tcconv
-        self.tcr = tcr
+        self.tcembr = tcembr
+        self.tcconvr = tcconvr
         self.tclength = tclength
 
         local_d = int(embed_dim / 2 / n_layers)
         embd_d = embed_dim - local_d * (2 * n_layers - 1)
 
-        if not tcemb:
-            self.emb = Embeddinglayer(vocab_size, embd_d)
+        if tcembr is None:
+            self.emb = EmbeddingLayer(vocab_size, embd_d)
         else:
-            self.emb = TCEmbedding(vocab_size, embd_d, ratio=tcr, tc_length=tclength)
+            self.emb = TCEmbedding(vocab_size, embd_d, ratio=tcembr, tc_length=tclength)
 
-        if tcconv:
-            conv1d = lambda *args, **kwargs: TCConv1D(*args, **kwargs, ratio=tcr, tc_length=tclength)
-        else:
+        if tcconvr is None:
             conv1d = tf.keras.layers.Conv1D
+        else:
+            conv1d = lambda *args, **kwargs: TCConv1D(*args, **kwargs, ratio=tcconvr, tc_length=tclength)
 
         self.spos, self.convs = [], []
         for i in range(n_layers):
             self.spos.append(SoftPOS(local_d, n_subpos=local_d, repeat_subpos=1))
             if i < n_layers - 1: self.convs.append(conv1d(local_d, 3, padding='causal', dilation_rate=2 ** i))
 
     def call(self, inputs):
@@ -131,55 +125,54 @@
         x = self.emb(inputs)
         xs = [x]
         for conv in self.convs:
             x = conv(x)
             xs.append(x)
 
         ys = []
-        for x, spos in zip(xs, self.sposs):
+        for x, spos in zip(xs, self.spos):
             y = spos(x)
             ys.append(y)
 
         x = tf.concat(ys, axis=-1)
 
         return x
 
     def get_config(self):
 
         config = {
             'vocab_size': self.vocab_size,
             'embed_dim': self.embed_dim,
             'n_layers': self.n_layers,
-            'tcemb': self.tcemb,
-            'tcconv': self.tcconv,
-            'tcr': self.tcr,
+            'tcembr': self.tcembr,
+            'tcconvr': self.tcconvr,
             'tclength': self.tclength,
         }
 
         base_config = super().get_config()
         return dict(list(base_config.items()) + list(config.items()))
 
 
 def select_embedding_type(self, comments, inputs_vocab_size, target_vocab_size, d_model):
     if not 'tcemb' in comments:
-        emb = lambda vocab, embd: Embeddinglayer(vocab, embd)
+        emb = lambda vocab, embd: EmbeddingLayer(vocab, embd)
     else:
         tclength = str2val(comments, 'tclength', int, default=3)
         tcr = str2val(comments, 'tcemb', float, default=.2)
         emb = lambda vocab, embd: TCEmbedding(vocab, embd, ratio=tcr, tc_length=tclength)
 
     if 'hsoftpos' in comments:
         n = str2val(comments, 'hsoftpos', output_type=int, default=3)
 
         local_d = int(d_model / 2 / n)
         embd_d = d_model - local_d * (2 * n - 1)
 
         if not 'tcemb' in comments:
-            eemb = Embeddinglayer(inputs_vocab_size, embd_d)
-            demb = Embeddinglayer(target_vocab_size, embd_d)
+            eemb = EmbeddingLayer(inputs_vocab_size, embd_d)
+            demb = EmbeddingLayer(target_vocab_size, embd_d)
         else:
             tcr = str2val(comments, 'tcemb', float, default=.2)
 
             tclength = str2val(comments, 'tclength', int, default=3)
             eemb = TCEmbedding(inputs_vocab_size, embd_d, ratio=tcr, tc_length=tclength)
             demb = TCEmbedding(target_vocab_size, embd_d, ratio=tcr, tc_length=tclength)
 
@@ -223,10 +216,29 @@
                 input = projector(input)
                 x = emb(input, mode='projection')
 
             return x
 
         self.encoder_embedding_layer = lambda x, mode='embedding': code(x, eemb, econvs, espos, mode)
         self.decoder_embedding_layer = lambda x, mode='embedding': code(x, demb, dconvs, dspos, mode)
+
+    elif 'layerhspos' in comments:
+        print('nice!')
+        n = str2val(comments, 'layerhspos', output_type=int, default=3)
+
+        tclength = str2val(comments, 'tclength', int, default=2)
+        tcembr, tcconvr = None, None
+        if 'tcemb' in comments:
+            tcembr = str2val(comments, 'tcemb', float, default=.2)
+
+        if 'tcconv' in comments:
+            tcconvr = str2val(comments, 'tcconv', float, default=.2)
+
+        self.encoder_embedding_layer = HSoftPOS(
+            inputs_vocab_size, d_model, n_layers=n, tcembr=tcembr, tcconvr=tcconvr, tclength=tclength
+        )
+        self.decoder_embedding_layer = HSoftPOS(
+            target_vocab_size, d_model, n_layers=n, tcembr=tcembr, tcconvr=tcconvr, tclength=tclength
+        )
     else:
         self.encoder_embedding_layer = emb(inputs_vocab_size, d_model)
         self.decoder_embedding_layer = emb(inputs_vocab_size, d_model)
```

### Comparing `anthe_official-1.0.0/neural_models/transformer.py` & `anthe_official-1.0.1/neural_models_tf/transformer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import os
 
 import tensorflow as tf
 
 from pyaromatics.stay_organized.utils import str2val
-from anthe_official.neural_models.attentions import MultiHeadAttention
-from anthe_official.neural_models.helper_layers import ProjectionLayer
-from anthe_official.neural_models.tensor_chain.dense import TCDense
-from anthe_official.neural_models.special_embedding import select_embedding_type
+from anthe_official.neural_models_tf.attentions import MultiHeadAttention
+from anthe_official.neural_models_tf.helper_layers import ProjectionLayer
+from anthe_official.neural_models_tf.tensor_chain.dense import TCDense
+from anthe_official.neural_models_tf.special_embedding import select_embedding_type
 
 os.environ['TF_CPP_MIN_LOG_LEVEL'] = '3'
 
 
 class Transformer:
     def __init__(self,
                  inputs_vocab_size,
@@ -165,30 +165,27 @@
         else:
             self.position_wise_feed_forward_layer = PositionWiseFeedForwardLayer(
                 d_point_wise_ff, d_model, comments
             )
         self.dropout_3 = tf.keras.layers.Dropout(dropout_prob)
         self.layer_norm_3 = tf.keras.layers.LayerNormalization(epsilon=1e-6)
 
-        self.last_op = lambda x, y: x + y if 'skipwithin' in comments else x
 
     def call(self, decoder_inputs, encoder_output, look_ahead_mask, padding_mask):
         output, attention_1 = self.attention([decoder_inputs, decoder_inputs, decoder_inputs, look_ahead_mask])
         output = self.dropout_1(output)
         query = self.layer_norm_1(tf.add(decoder_inputs, output))  # residual network
         output, attention_2 = self.conditioned_attention([query, encoder_output, encoder_output, padding_mask])
         output = self.dropout_2(output)
         encoder_decoder_attention_output = self.layer_norm_2(tf.add(output, query))
 
         output = self.position_wise_feed_forward_layer(encoder_decoder_attention_output)
         output = self.dropout_3(output)
         output = self.layer_norm_3(tf.add(encoder_decoder_attention_output, output))  # residual network
 
-        output = self.last_op(output, decoder_inputs)
-
         return output, attention_1, attention_2
 
 
 AntheDecoderBlock = lambda attention_head_count, d_model, d_point_wise_ff, dropout_prob: \
     EncoderLayer(
         attention_head_count, d_model, d_point_wise_ff, dropout_prob,
         comments='geglu_gateattention_hsoftpos:2_tcffn:.005_tcpreatt:.07_tclength:2'
```

### Comparing `anthe_official-1.0.0/setup.py` & `anthe_official-1.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     'pandas>=1.4.0',
     'scikit_learn>=1.1.3',
     'sentencepiece>=0.1.97',
     'tensorflow>=2.10.0',
     'tqdm>=4.64.0',
     'pyaromatics==0.0.2',
 ]
-__version__ = '1.0.0'
+__version__ = '1.0.1'
 
 setup(
     name='anthe_official',
     version=__version__,
     license='Apache License',
     author='Luca Herranz-Celotti, Ermal Rrapaj',
     author_email='luca.herrtti@gmail.com',
```

