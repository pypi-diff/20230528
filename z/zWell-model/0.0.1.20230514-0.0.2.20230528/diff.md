# Comparing `tmp/zWell_model-0.0.1.20230514.tar.gz` & `tmp/zWell_model-0.0.2.20230528.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zWell_model-0.0.1.20230514.tar", last modified: Sun May 14 08:03:44 2023, max compression
+gzip compressed data, was "zWell_model-0.0.2.20230528.tar", last modified: Sun May 28 10:07:36 2023, max compression
```

## Comparing `zWell_model-0.0.1.20230514.tar` & `zWell_model-0.0.2.20230528.tar`

### file list

```diff
@@ -1,24 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-05-14 08:03:44.238794 zWell_model-0.0.1.20230514/
--rw-rw-rw-   0        0        0     6635 2023-05-14 08:03:44.236800 zWell_model-0.0.1.20230514/PKG-INFO
--rw-rw-rw-   0        0        0     6044 2023-05-14 03:53:56.000000 zWell_model-0.0.1.20230514/README.md
--rw-rw-rw-   0        0        0      602 2023-05-14 08:03:19.000000 zWell_model-0.0.1.20230514/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-14 08:03:44.238794 zWell_model-0.0.1.20230514/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-14 08:03:44.231796 zWell_model-0.0.1.20230514/zWell_model/
--rw-rw-rw-   0        0        0      443 2023-05-14 07:53:46.000000 zWell_model-0.0.1.20230514/zWell_model/__init__.py
--rw-rw-rw-   0        0        0     1068 2023-05-14 07:12:33.000000 zWell_model-0.0.1.20230514/zWell_model/allModel.py
-drwxrwxrwx   0        0        0        0 2023-05-14 08:03:44.234796 zWell_model-0.0.1.20230514/zWell_model/convNet/
--rw-rw-rw-   0        0        0     3086 2023-05-14 07:20:32.000000 zWell_model-0.0.1.20230514/zWell_model/convNet/ConvNetV1.py
--rw-rw-rw-   0        0        0     2265 2023-05-14 07:18:31.000000 zWell_model-0.0.1.20230514/zWell_model/convNet/ConvNetV2.py
--rw-rw-rw-   0        0        0        0 2023-05-14 07:49:40.000000 zWell_model-0.0.1.20230514/zWell_model/convNet/__init__.py
--rw-rw-rw-   0        0        0     2641 2023-05-14 06:45:56.000000 zWell_model-0.0.1.20230514/zWell_model/convNet/convNetWork.py
-drwxrwxrwx   0        0        0        0 2023-05-14 08:03:44.236800 zWell_model-0.0.1.20230514/zWell_model/resNet/
--rw-rw-rw-   0        0        0     1719 2023-05-14 07:49:40.000000 zWell_model-0.0.1.20230514/zWell_model/resNet/ResNetV1.py
--rw-rw-rw-   0        0        0        0 2023-05-14 07:49:40.000000 zWell_model-0.0.1.20230514/zWell_model/resNet/__init__.py
--rw-rw-rw-   0        0        0     4518 2023-05-14 07:00:16.000000 zWell_model-0.0.1.20230514/zWell_model/resNet/resNetWork.py
--rw-rw-rw-   0        0        0     2728 2023-05-14 06:33:15.000000 zWell_model-0.0.1.20230514/zWell_model/resNet/utils.py
--rw-rw-rw-   0        0        0     2376 2023-05-14 07:34:26.000000 zWell_model-0.0.1.20230514/zWell_model/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-14 08:03:44.233795 zWell_model-0.0.1.20230514/zWell_model.egg-info/
--rw-rw-rw-   0        0        0     6635 2023-05-14 08:03:44.000000 zWell_model-0.0.1.20230514/zWell_model.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      489 2023-05-14 08:03:44.000000 zWell_model-0.0.1.20230514/zWell_model.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-14 08:03:44.000000 zWell_model-0.0.1.20230514/zWell_model.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-05-14 08:03:44.000000 zWell_model-0.0.1.20230514/zWell_model.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-28 10:07:36.592749 zWell_model-0.0.2.20230528/
+-rw-rw-rw-   0        0        0    11558 2022-11-12 10:49:35.000000 zWell_model-0.0.2.20230528/LICENSE
+-rw-rw-rw-   0        0        0    10996 2023-05-28 10:07:36.592387 zWell_model-0.0.2.20230528/PKG-INFO
+-rw-rw-rw-   0        0        0    10382 2023-05-28 09:49:34.000000 zWell_model-0.0.2.20230528/README.md
+-rw-rw-rw-   0        0        0      602 2023-05-28 09:52:09.000000 zWell_model-0.0.2.20230528/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-28 10:07:36.592749 zWell_model-0.0.2.20230528/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-28 10:07:36.584265 zWell_model-0.0.2.20230528/zWell_model/
+-rw-rw-rw-   0        0        0      775 2023-05-28 09:46:39.000000 zWell_model-0.0.2.20230528/zWell_model/__init__.py
+-rw-rw-rw-   0        0        0     1311 2023-05-28 09:37:02.000000 zWell_model-0.0.2.20230528/zWell_model/allModel.py
+drwxrwxrwx   0        0        0        0 2023-05-28 10:07:36.588014 zWell_model-0.0.2.20230528/zWell_model/convNet/
+-rw-rw-rw-   0        0        0     3185 2023-05-28 09:37:02.000000 zWell_model-0.0.2.20230528/zWell_model/convNet/ConvNetV1.py
+-rw-rw-rw-   0        0        0     2336 2023-05-28 09:37:02.000000 zWell_model-0.0.2.20230528/zWell_model/convNet/ConvNetV2.py
+-rw-rw-rw-   0        0        0        0 2023-05-14 07:49:40.000000 zWell_model-0.0.2.20230528/zWell_model/convNet/__init__.py
+-rw-rw-rw-   0        0        0     2404 2023-05-28 09:37:02.000000 zWell_model-0.0.2.20230528/zWell_model/convNet/convNetWork.py
+drwxrwxrwx   0        0        0        0 2023-05-28 10:07:36.589122 zWell_model-0.0.2.20230528/zWell_model/denseNet/
+-rw-rw-rw-   0        0        0     3224 2023-05-28 09:37:02.000000 zWell_model-0.0.2.20230528/zWell_model/denseNet/DenseNet.py
+-rw-rw-rw-   0        0        0     1680 2023-05-28 09:37:02.000000 zWell_model-0.0.2.20230528/zWell_model/denseNet/DenseNetV1.py
+-rw-rw-rw-   0        0        0      152 2023-05-28 09:37:02.000000 zWell_model-0.0.2.20230528/zWell_model/denseNet/__init__.py
+-rw-rw-rw-   0        0        0      716 2023-05-28 09:37:02.000000 zWell_model-0.0.2.20230528/zWell_model/denseNet/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-28 10:07:36.590784 zWell_model-0.0.2.20230528/zWell_model/resNet/
+-rw-rw-rw-   0        0        0     1927 2023-05-28 09:37:02.000000 zWell_model-0.0.2.20230528/zWell_model/resNet/ResNetV1.py
+-rw-rw-rw-   0        0        0        0 2023-05-14 07:49:40.000000 zWell_model-0.0.2.20230528/zWell_model/resNet/__init__.py
+-rw-rw-rw-   0        0        0     4257 2023-05-28 09:37:02.000000 zWell_model-0.0.2.20230528/zWell_model/resNet/resNetWork.py
+-rw-rw-rw-   0        0        0     2728 2023-05-14 06:33:15.000000 zWell_model-0.0.2.20230528/zWell_model/resNet/utils.py
+-rw-rw-rw-   0        0        0     2376 2023-05-14 07:34:26.000000 zWell_model-0.0.2.20230528/zWell_model/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-28 10:07:36.585831 zWell_model-0.0.2.20230528/zWell_model.egg-info/
+-rw-rw-rw-   0        0        0    10996 2023-05-28 10:07:36.000000 zWell_model-0.0.2.20230528/zWell_model.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      628 2023-05-28 10:07:36.000000 zWell_model-0.0.2.20230528/zWell_model.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-28 10:07:36.000000 zWell_model-0.0.2.20230528/zWell_model.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-05-28 10:07:36.000000 zWell_model-0.0.2.20230528/zWell_model.egg-info/top_level.txt
```

### Comparing `zWell_model-0.0.1.20230514/pyproject.toml` & `zWell_model-0.0.2.20230528/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "zWell_model"
-version = "0.0.1.20230514"
+version = "0.0.2.20230528"
 authors = [
   { name="BeardedManZhao", email="liming7887@qq.com" },
 ]
 description = "Deep learning model adapter, used to quickly create various deep learning models."
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
```

### Comparing `zWell_model-0.0.1.20230514/zWell_model/allModel.py` & `zWell_model-0.0.2.20230528/zWell_model/allModel.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,16 +4,17 @@
 # @Email : liming7887@qq.com
 # @File : allModel.py
 # @Project : Keras-model
 
 
 class AllModel:
 
-    def to_keras_model(self, **args):
+    def to_keras_model(self, add_fully_connected=True, **args):
         """
+        :param add_fully_connected 布尔数值 如果设置为true 代表要添加全连接神经网络部分，如果为False 代表不添加全连接，只添加最基本的架构，暑促部分由外部实现。
         :param args: 获取到模型需要使用的参数数值。
         :return: keras 中的模型对象
         """
         pass
 
     def __lshift__(self, other):
         """
```

### Comparing `zWell_model-0.0.1.20230514/zWell_model/convNet/ConvNetV1.py` & `zWell_model-0.0.2.20230528/zWell_model/convNet/ConvNetV1.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 
 class ConvNetV1(ConvNet):
     """
     第一种基本的卷积神经网络模型
     """
 
-    def to_keras_model(self, **args):
+    def to_keras_model(self, add_fully_connected=True, **args):
         from keras import Sequential
         from keras.layers import Convolution2D, Activation, MaxPooling2D, Flatten, Dense
         init_filters = self.init_k_len
         model = Sequential(name=args.get('name', 'ConvNetV1'))
         # 添加第一层神经元 这里第一层是卷积
         model.add(
             Convolution2D(
@@ -60,18 +60,19 @@
                 init_filters *= self.ckp
                 model.add(Convolution2D(filters=init_filters, kernel_size=2, padding='same', strides=self.stride[i]))
                 # 添加一层激活函数
                 model.add(Activation("relu"))
                 # 添加一层池化
                 model.add(MaxPooling2D(pool_size=2, padding='same'))
 
-        # 将矩阵扁平化准备全连接
-        model.add(Flatten())
-        # 正式进入全连接神经网络，添加全连接神经元(具有1024个神经元的层)
-        model.add(Dense(self.dense_len))
-        # 添加激活函数
-        model.add(Activation("relu"))
-        # 再一次添加一层 8 个神经元的网络层(每个神经元代表一个类别)
-        model.add(Dense(self.classes))
-        # 添加激活函数 softmax 用于计算概率得分
-        model.add(Activation("softmax"))
+        if add_fully_connected:
+            # 将矩阵扁平化准备全连接
+            model.add(Flatten())
+            # 正式进入全连接神经网络，添加全连接神经元(具有1024个神经元的层)
+            model.add(Dense(self.dense_len))
+            # 添加激活函数
+            model.add(Activation("relu"))
+            # 再一次添加一层 8 个神经元的网络层(每个神经元代表一个类别)
+            model.add(Dense(self.classes))
+            # 添加激活函数 softmax 用于计算概率得分
+            model.add(Activation("softmax"))
         return model
```

### Comparing `zWell_model-0.0.1.20230514/zWell_model/convNet/ConvNetV2.py` & `zWell_model-0.0.2.20230528/zWell_model/convNet/ConvNetV2.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # @File : ConvNetV2.py
 # @Project : ZWell-model
 from zWell_model.convNet.convNetWork import ConvNet
 
 
 class ConvNetV2(ConvNet):
 
-    def to_keras_model(self, **args):
+    def to_keras_model(self, add_fully_connected=True, **args):
         from keras import Sequential
         from keras.applications.densenet import layers
         init_filters = self.init_k_len
         model = Sequential(name=args.get('name', 'ConvNetV2'))
         # 卷积
         model.add(
             layers.Conv2D(init_filters, (3, 3), activation='relu', input_shape=self.input_shape)
@@ -51,13 +51,14 @@
         model.add(layers.BatchNormalization())
         # 随机失活
         model.add(layers.Dropout(0.25))
         # 池化 同时降维
         model.add(layers.GlobalAveragePooling2D())
 
         # 开始全连接
-        model.add(layers.Dense(self.dense_len))
-        model.add(layers.BatchNormalization())
-        model.add(layers.Dropout(0.5))
+        if add_fully_connected:
+            model.add(layers.Dense(self.dense_len))
+            model.add(layers.BatchNormalization())
+            model.add(layers.Dropout(0.5))
         # 输出类别
         model.add(layers.Dense(self.classes, activation='softmax'))
         return model
```

### Comparing `zWell_model-0.0.1.20230514/zWell_model/convNet/convNetWork.py` & `zWell_model-0.0.2.20230528/zWell_model/convNet/convNetWork.py`

 * *Files 9% similar despite different names*

```diff
@@ -32,22 +32,14 @@
         self.classes = classes
         self.stride = stride
         self.model_layers_num = model_layers_num
         self.ckp = ckp
         self.init_k_len = init_k_len
         self.dense_len = dense_len
 
-    def to_keras_model(self, **args):
-        """
-        将卷积神经网络转换成为Keras中能够支持的模型
-        :param args: 参数列表
-        :return: keras 中的神经网络模型
-        """
-        pass
-
     def __rshift__(self, other):
         other.stride = self.stride
         other.input_shape = self.input_shape
         other.classes = self.classes
         other.model_layers_num = self.model_layers_num
         other.ckp = self.ckp
         other.init_k_len = self.init_k_len
```

### Comparing `zWell_model-0.0.1.20230514/zWell_model/resNet/ResNetV1.py` & `zWell_model-0.0.2.20230528/zWell_model/resNet/ResNetV1.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # @File : ResNetV1.py
 # @Project : ZWell-model
 from zWell_model.resNet import utils as ru
 from zWell_model.resNet.resNetWork import ResNet
 
 
 class ResNetV1(ResNet):
-    def to_keras_model(self, **args):
+    def to_keras_model(self, add_fully_connected=True, **args):
         from keras import Input, Model
         from keras.layers import AveragePooling2D, Flatten, Dropout, Dense
         """定义残差网络"""
         inputs = Input(shape=self.input_shape)
         # 开始进行残差块之前进行一层卷积 然后开始进行残差块计算
         x = ru.res_module(inputs, k=self.init_k_len, stride=self.stride[0], chan_dim=self.chan_dim, red=self.red)
         # 准备进入其它残差块
@@ -27,17 +27,20 @@
         else:
             k_size *= self.ckp
             for index in range(1, self.model_layers_num):
                 x = ru.res_module(
                     x, k=k_size, stride=self.stride[index], chan_dim=self.chan_dim, red=self.red
                 )
         # 均值池化
-        x = AveragePooling2D()(x)
-        # 扁平化
-        x = Flatten()(x)
-        # 失活
-        x = Dropout(0.5)(x)
-        # 全连接
-        x = Dense(self.dense_len, activation='relu')(x)
-        outputs = Dense(self.classes, activation='softmax')(x)
-        model = Model(name=args.get('name', 'ResNetV1'), inputs=inputs, outputs=outputs)
+        if add_fully_connected:
+            output = AveragePooling2D()(x)
+            # 扁平化
+            x = Flatten()(output)
+            # 失活
+            x = Dropout(0.5)(x)
+            # 全连接
+            x = Dense(self.dense_len, activation='relu')(x)
+            outputs = Dense(self.classes, activation='softmax')(x)
+            model = Model(name=args.get('name', 'ResNetV1'), inputs=inputs, outputs=outputs)
+        else:
+            model = Model(name=args.get('name', 'ResNetV1'), inputs=inputs, outputs=x)
         return model
```

### Comparing `zWell_model-0.0.1.20230514/zWell_model/resNet/resNetWork.py` & `zWell_model-0.0.2.20230528/zWell_model/resNet/resNetWork.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,22 +54,14 @@
         self.bn_eps = bn_eps
         self.bn_mom = bn_mom
         self.model_layers_num = model_layers_num
         self.ckp = ckp
         self.init_k_len = init_k_len
         self.dense_len = dense_len
 
-    def to_keras_model(self, **args):
-        """
-        将当前神经网络模型对象转换成为 keras 中的模型对象
-        :param args: 需要使用到的参数
-        :return: 转换之后的 keras 模型对象
-        """
-        pass
-
     def __rshift__(self, other):
         """
         使用拷贝的方式将当亲残差网络模型中的所有属性拷贝到另一个残差网络模型对象中，常用于不同配置的网络之间的属性覆写操作。
         能够在不重新创建新神经网络对象的前提下复制神经网络对象
         :param other: 拷贝之后的新神经网络模型。
         :return: 拷贝之后的新神经网络模型。
         """
```

### Comparing `zWell_model-0.0.1.20230514/zWell_model/resNet/utils.py` & `zWell_model-0.0.2.20230528/zWell_model/resNet/utils.py`

 * *Files identical despite different names*

### Comparing `zWell_model-0.0.1.20230514/zWell_model/utils.py` & `zWell_model-0.0.2.20230528/zWell_model/utils.py`

 * *Files identical despite different names*

