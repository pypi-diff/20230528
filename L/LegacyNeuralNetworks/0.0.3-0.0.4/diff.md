# Comparing `tmp/LegacyNeuralNetworks-0.0.3.tar.gz` & `tmp/LegacyNeuralNetworks-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LegacyNeuralNetworks-0.0.3.tar", last modified: Sat May 27 14:41:47 2023, max compression
+gzip compressed data, was "LegacyNeuralNetworks-0.0.4.tar", last modified: Sun May 28 18:36:29 2023, max compression
```

## Comparing `LegacyNeuralNetworks-0.0.3.tar` & `LegacyNeuralNetworks-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-27 14:41:47.673488 LegacyNeuralNetworks-0.0.3/
-drwxrwxrwx   0        0        0        0 2023-05-27 14:41:47.663516 LegacyNeuralNetworks-0.0.3/LegacyNeuralNetworks/
--rw-rw-rw-   0        0        0    31698 2023-05-27 10:22:37.000000 LegacyNeuralNetworks-0.0.3/LegacyNeuralNetworks/Fill.py
--rw-rw-rw-   0        0        0    19189 2023-05-27 08:44:43.000000 LegacyNeuralNetworks-0.0.3/LegacyNeuralNetworks/LegacyNeuralNetworks.py
--rw-rw-rw-   0        0        0      151 2023-05-27 14:39:50.000000 LegacyNeuralNetworks-0.0.3/LegacyNeuralNetworks/__init__.py
--rw-rw-rw-   0        0        0    14578 2023-05-27 14:39:19.000000 LegacyNeuralNetworks-0.0.3/LegacyNeuralNetworks/ann_fill.py
-drwxrwxrwx   0        0        0        0 2023-05-27 14:41:47.669041 LegacyNeuralNetworks-0.0.3/LegacyNeuralNetworks.egg-info/
--rw-rw-rw-   0        0        0     1628 2023-05-27 14:41:47.000000 LegacyNeuralNetworks-0.0.3/LegacyNeuralNetworks.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      377 2023-05-27 14:41:47.000000 LegacyNeuralNetworks-0.0.3/LegacyNeuralNetworks.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-27 14:41:47.000000 LegacyNeuralNetworks-0.0.3/LegacyNeuralNetworks.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2023-05-27 14:41:47.000000 LegacyNeuralNetworks-0.0.3/LegacyNeuralNetworks.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-05-27 14:41:47.000000 LegacyNeuralNetworks-0.0.3/LegacyNeuralNetworks.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1628 2023-05-27 14:41:47.670048 LegacyNeuralNetworks-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      722 2023-05-27 10:52:46.000000 LegacyNeuralNetworks-0.0.3/README.md
--rw-rw-rw-   0        0        0       42 2023-05-27 14:41:47.673488 LegacyNeuralNetworks-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      907 2023-05-27 14:41:12.000000 LegacyNeuralNetworks-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-28 18:36:29.857357 LegacyNeuralNetworks-0.0.4/
+drwxrwxrwx   0        0        0        0 2023-05-28 18:36:29.829495 LegacyNeuralNetworks-0.0.4/LegacyNeuralNetworks/
+-rw-rw-rw-   0        0        0    29928 2023-05-28 18:33:46.000000 LegacyNeuralNetworks-0.0.4/LegacyNeuralNetworks/Fill.py
+-rw-rw-rw-   0        0        0    19189 2023-05-27 08:44:43.000000 LegacyNeuralNetworks-0.0.4/LegacyNeuralNetworks/LegacyNeuralNetworks.py
+-rw-rw-rw-   0        0        0      151 2023-05-27 14:39:50.000000 LegacyNeuralNetworks-0.0.4/LegacyNeuralNetworks/__init__.py
+-rw-rw-rw-   0        0        0    14578 2023-05-27 14:39:19.000000 LegacyNeuralNetworks-0.0.4/LegacyNeuralNetworks/ann_fill.py
+drwxrwxrwx   0        0        0        0 2023-05-28 18:36:29.855358 LegacyNeuralNetworks-0.0.4/LegacyNeuralNetworks.egg-info/
+-rw-rw-rw-   0        0        0     4398 2023-05-28 18:36:29.000000 LegacyNeuralNetworks-0.0.4/LegacyNeuralNetworks.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      377 2023-05-28 18:36:29.000000 LegacyNeuralNetworks-0.0.4/LegacyNeuralNetworks.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-28 18:36:29.000000 LegacyNeuralNetworks-0.0.4/LegacyNeuralNetworks.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2023-05-28 18:36:29.000000 LegacyNeuralNetworks-0.0.4/LegacyNeuralNetworks.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-05-28 18:36:29.000000 LegacyNeuralNetworks-0.0.4/LegacyNeuralNetworks.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4398 2023-05-28 18:36:29.856354 LegacyNeuralNetworks-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     3284 2023-05-27 14:44:31.000000 LegacyNeuralNetworks-0.0.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-28 18:36:29.857357 LegacyNeuralNetworks-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      907 2023-05-28 18:36:05.000000 LegacyNeuralNetworks-0.0.4/setup.py
```

### Comparing `LegacyNeuralNetworks-0.0.3/LegacyNeuralNetworks/Fill.py` & `LegacyNeuralNetworks-0.0.4/LegacyNeuralNetworks/Fill.py`

 * *Files 8% similar despite different names*

```diff
@@ -108,14 +108,15 @@
         inputs = np.array([x1, x2])
         return self.activate(inputs, weights) 
 
 neuron = McCullochPittsNeuron()
 weights = [1, 4]
 x1 = 0; x2 = 0
 output = neuron.andnot(x1, x2, weights)
+print(output)
 """
 
 ascii_perceptron = """ 
 import numpy as np
 import tensorflow as tf
 import matplotlib.pyplot as plt
 from sklearn.linear_model import Perceptron
@@ -617,108 +618,34 @@
 recalled_vector = hopfield.recall(noisy_vector, steps=5)
 
 print(f"Noisy input:    {noisy_vector}")
 print(f"Recalled output: {recalled_vector.tolist()}")
 """
 
 cnn_object_detection = """ 
-import numpy as np
 import tensorflow as tf
-import matplotlib.pyplot as plt
-from sklearn.linear_model import Perceptron
-from sklearn.datasets import make_classification
-from sklearn.neural_network import MLPClassifier
-
-class CNNObjectDetection:
-    def __init__(self, num_classes=10, filters=32, kernel=(3, 3), dense_nodes=64):
-        self.filters = filters
-        self.kernel = kernel
-        self.dense_nodes = dense_nodes
-        self.num_classes = num_classes
-        self.model = self.create_model()
-
-    def create_model(self):
-        model = tf.keras.Sequential([
-            tf.keras.layers.Conv2D(self.filters, self.kernel, activation='relu', input_shape=(32, 32, 3)),
-            tf.keras.layers.MaxPooling2D((2, 2)),
-            tf.keras.layers.Flatten(),
-            tf.keras.layers.Dense(self.dense_nodes, activation='relu'),
-            tf.keras.layers.Dense(self.num_classes, activation='softmax')
-        ])
-        return model
-
-    def train_model(self, X_train, y_train, X_val, y_val, epochs, batch_size):
-        # Compile the model
-        self.model.compile(optimizer='adam', loss='sparse_categorical_crossentropy', metrics=['accuracy'])
-
-        # Train the model
-        history = self.model.fit(X_train, y_train, validation_data=(X_val, y_val), epochs=epochs, batch_size=batch_size)
-
-        return history
-
-    def plot_accuracy(self, history):
-        # Plot accuracy graph
-        plt.plot(history.history['accuracy'])
-        plt.plot(history.history['val_accuracy'])
-        plt.title('Model Accuracy')
-        plt.ylabel('Accuracy')
-        plt.xlabel('Epoch')
-        plt.legend(['Train', 'Validation'], loc='upper left')
-        plt.show()
-
-    def plot_loss(self, history):
-        # Plot loss graph
-        plt.plot(history.history['loss'])
-        plt.plot(history.history['val_loss'])
-        plt.title('Model Loss')
-        plt.ylabel('Loss')
-        plt.xlabel('Epoch')
-        plt.legend(['Train', 'Validation'], loc='upper right')
-        plt.show()
-
-    def evaluate_model(self, X_test, y_test):
-        loss, accuracy = self.model.evaluate(X_test, y_test)
-        print("Test Loss:", loss)
-        print("Test Accuracy:", accuracy)
-
-    def run(self, X_train, y_train, X_val, y_val, X_test, y_test, epochs=10, batch_size=32, plot=False):
-        history = self.train_model(X_train, y_train, X_val, y_val, epochs, batch_size)
-
-        if plot: self.plot_accuracy(history)
-        if plot: self.plot_loss(history)
-
-        self.evaluate_model(X_test, y_test)
-
-        
-(X_train, y_train), (X_test, y_test) = tf.keras.datasets.cifar10.load_data()
-
-# Split the data into training and validation sets
-X_train, X_val, y_train, y_val = train_test_split(X_train, y_train, 
-                                                  test_size=0.2, random_state=42)
-
-# Normalize pixel values
-X_train = X_train / 255.0
-X_val = X_val / 255.0
-X_test = X_test / 255.0
-
-# Create and train the model
-cnn = ConvNetImageClassification(num_classes=10)
-cnn.run(X_train, y_train, 
-        X_val, y_val, 
-        X_test, y_test, 
-        epochs=20, batch_size=128)
+model = tf.keras.applications.MobileNetV2(weights='imagenet')
+# Load image and preprocess it
+image = tf.keras.preprocessing.image.load_img('download.jpeg', target_size=(224, 224))
+image = tf.keras.preprocessing.image.img_to_array(image)
+image = tf.keras.applications.mobilenet_v2.preprocess_input(image)
+image = tf.expand_dims(image, axis=0)
+# Run object detection
+predictions = model.predict(image)
+decoded_predictions = tf.keras.applications.mobilenet_v2.decode_predictions(predictions)
+# Print top predicted objects
+for _, label, confidence in decoded_predictions[0]:
+    print(f"{label}: {confidence * 100}%")
 """
 
 cnn_image_classification = """ 
 import numpy as np
 import tensorflow as tf
 import matplotlib.pyplot as plt
-from sklearn.linear_model import Perceptron
-from sklearn.datasets import make_classification
-from sklearn.neural_network import MLPClassifier
+from sklearn.model_selection import train_test_split
 
 class CNNObjectDetection:
     def __init__(self, num_classes=10, filters=32, kernel=(3, 3), dense_nodes=64):
         self.filters = filters
         self.kernel = kernel
         self.dense_nodes = dense_nodes
         self.num_classes = num_classes
@@ -785,15 +712,15 @@
 
 # Normalize pixel values
 X_train = X_train / 255.0
 X_val = X_val / 255.0
 X_test = X_test / 255.0
 
 # Create and train the model
-cnn = ConvNetImageClassification(num_classes=10, filters=32, kernel=(3, 3), dense_nodes=64)
+cnn = CNNObjectDetection(num_classes=10, filters=32, kernel=(3, 3), dense_nodes=64)
 cnn.run(X_train, y_train, 
         X_val, y_val, 
         X_test, y_test, 
         epochs=20, batch_size=128,
         plot=True)
 """
 
@@ -904,29 +831,51 @@
 # Evaluate the model
 mnist_classifier.evaluate(X_test, y_test)
 
 # To visualize the data
 mnist_classifier.visualize_data( X_test, y_test, num_samples=5)
 """
 
+bam = """ 
+import numpy as np
+def bam(input_patterns,output_patterns):
+    input_patterns=np.array(input_patterns)
+    output_patterns= np.array(output_patterns)
+    weight_matrix = np.dot(output_patterns.T,input_patterns)
+    def activation(input_pattern):
+        output_pattern = np.dot(weight_matrix,input_pattern)
+        output_pattern[output_pattern>=0]=1
+        output_pattern[output_pattern<0]=-1
+        return output_pattern    
+    print("input patterns | output patterns")
+    for i in range(input_patterns.shape[0]):
+        input_pattern = input_patterns[i]
+        output_pattern = activation(input_pattern)
+        print(f"{input_pattern} | {output_pattern}")
+input_patterns=[[1,-1,1,-1],[1,1,-1,-1]]
+output_patterns=[[1,1],[-1,-1]]
+bam(input_patterns,output_patterns)
+"""
+
 
 masterDict = {
     'activation_function' : activation_function,
     'mcculloh_pitt': mcculloh_pitt,
     'ascii_perceptron': ascii_perceptron,
     'descision_region_perceptron': descision_region_perceptron,
     'recognize_5x3_matrix': recognize_5x3_matrix,
     'ann_forward_backward': ann_forward_backward,
     'xor_backprop': xor_backprop,
     'art_network': art_network,
     'hopfield_network':hopfield_network,
     'cnn_object_detection': cnn_object_detection,
     'cnn_image_classification': cnn_image_classification,
     'cnn_tf_implementation': cnn_tf_implementation,
-    'mnist_detection': mnist_detection   
+    'mnist_detection': mnist_detection,
+    'bam': bam
 }
 
 class Writer:
     def __init__(self, filename):
         self.filename = os.path.join(os.getcwd(), filename)
         self.masterDict = masterDict
         self.questions = list(masterDict.keys())
```

### Comparing `LegacyNeuralNetworks-0.0.3/LegacyNeuralNetworks/LegacyNeuralNetworks.py` & `LegacyNeuralNetworks-0.0.4/LegacyNeuralNetworks/LegacyNeuralNetworks.py`

 * *Files identical despite different names*

### Comparing `LegacyNeuralNetworks-0.0.3/LegacyNeuralNetworks/ann_fill.py` & `LegacyNeuralNetworks-0.0.4/LegacyNeuralNetworks/ann_fill.py`

 * *Files identical despite different names*

### Comparing `LegacyNeuralNetworks-0.0.3/setup.py` & `LegacyNeuralNetworks-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.3'
+VERSION = '0.0.4'
 DESCRIPTION = 'Legacy Neural Networks'
  
 # Setting up
 setup(
     name="LegacyNeuralNetworks",
     version=VERSION,
     author="Hrushikesh Kachgunde",
```

