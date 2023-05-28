# Comparing `tmp/vision6D-0.0.9.tar.gz` & `tmp/vision6D-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\vision6D-0.0.9.tar", last modified: Sat May 27 00:14:57 2023, max compression
+gzip compressed data, was "dist\vision6D-0.1.0.tar", last modified: Sun May 28 00:07:30 2023, max compression
```

## Comparing `vision6D-0.0.9.tar` & `vision6D-0.1.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-05-27 00:14:56.976513 vision6D-0.0.9/
--rw-rw-rw-   0        0        0     1086 2023-01-03 15:55:06.000000 vision6D-0.0.9/LICENSE
--rw-rw-rw-   0        0        0       33 2023-05-27 00:07:11.000000 vision6D-0.0.9/MANIFEST.in
--rw-rw-rw-   0        0        0     1603 2023-05-27 00:14:56.976513 vision6D-0.0.9/PKG-INFO
--rw-rw-rw-   0        0        0      918 2023-05-27 00:06:55.000000 vision6D-0.0.9/README.md
--rw-rw-rw-   0        0        0      413 2023-01-03 15:55:07.000000 vision6D-0.0.9/pyproject.toml
--rw-rw-rw-   0        0        0     1927 2023-05-27 00:14:56.981517 vision6D-0.0.9/setup.cfg
--rw-rw-rw-   0        0        0      165 2023-05-27 00:14:24.000000 vision6D-0.0.9/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-27 00:14:56.894510 vision6D-0.0.9/test/
--rw-rw-rw-   0        0        0    21974 2023-05-17 18:41:02.000000 vision6D-0.0.9/test/test_create_dataset.py
--rw-rw-rw-   0        0        0     3630 2023-05-14 22:36:01.000000 vision6D-0.0.9/test/test_projection.py
-drwxrwxrwx   0        0        0        0 2023-05-27 00:14:56.918515 vision6D-0.0.9/vision6D/
--rw-rw-rw-   0        0        0    45165 2023-05-27 00:06:55.000000 vision6D-0.0.9/vision6D/GUI.py
--rw-rw-rw-   0        0        0      939 2023-05-27 00:06:55.000000 vision6D-0.0.9/vision6D/__init__.py
--rw-rw-rw-   0        0        0    19331 2023-05-14 22:36:01.000000 vision6D-0.0.9/vision6D/app.py
--rw-rw-rw-   0        0        0    12369 2023-05-27 00:06:55.000000 vision6D-0.0.9/vision6D/config.py
-drwxrwxrwx   0        0        0        0 2023-05-27 00:14:56.973513 vision6D-0.0.9/vision6D/data/
--rw-rw-rw-   0        0        0   445902 2023-05-14 22:36:01.000000 vision6D-0.0.9/vision6D/data/ossiclesCoordinateMapping.json
--rw-rw-rw-   0        0        0   335336 2023-05-14 22:36:02.000000 vision6D-0.0.9/vision6D/data/ossiclesCoordinateMappingv1.json
--rw-rw-rw-   0        0        0    12109 2023-05-15 22:13:50.000000 vision6D-0.0.9/vision6D/data/style.qss
--rw-rw-rw-   0        0        0    22897 2023-05-14 22:36:02.000000 vision6D-0.0.9/vision6D/interface.py
--rw-rw-rw-   0        0        0    27855 2023-05-27 00:06:55.000000 vision6D-0.0.9/vision6D/interface_gui.py
--rw-rw-rw-   0        0        0    33713 2023-05-14 22:36:02.000000 vision6D-0.0.9/vision6D/mainwindow.py
--rw-rw-rw-   0        0        0    14068 2023-05-15 23:19:36.000000 vision6D-0.0.9/vision6D/run_gui.py
--rw-rw-rw-   0        0        0      197 2023-05-14 22:53:44.000000 vision6D-0.0.9/vision6D/run_interface.py
--rw-rw-rw-   0        0        0    14911 2023-05-14 22:36:02.000000 vision6D-0.0.9/vision6D/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-27 00:14:56.962515 vision6D-0.0.9/vision6D.egg-info/
--rw-rw-rw-   0        0        0     1603 2023-05-27 00:14:56.000000 vision6D-0.0.9/vision6D.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      597 2023-05-27 00:14:56.000000 vision6D-0.0.9/vision6D.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-27 00:14:56.000000 vision6D-0.0.9/vision6D.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      164 2023-05-27 00:14:56.000000 vision6D-0.0.9/vision6D.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-27 00:14:56.000000 vision6D-0.0.9/vision6D.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-28 00:07:30.505332 vision6D-0.1.0/
+-rw-rw-rw-   0        0        0     1086 2023-01-03 15:55:06.000000 vision6D-0.1.0/LICENSE
+-rw-rw-rw-   0        0        0       33 2023-05-27 00:07:11.000000 vision6D-0.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     1603 2023-05-28 00:07:30.505332 vision6D-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      918 2023-05-28 00:06:16.000000 vision6D-0.1.0/README.md
+-rw-rw-rw-   0        0        0      413 2023-01-03 15:55:07.000000 vision6D-0.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0     1927 2023-05-28 00:07:30.511335 vision6D-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      165 2023-05-28 00:06:16.000000 vision6D-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-28 00:07:30.262457 vision6D-0.1.0/test/
+-rw-rw-rw-   0        0        0    21974 2023-05-17 18:41:02.000000 vision6D-0.1.0/test/test_create_dataset.py
+-rw-rw-rw-   0        0        0     3630 2023-05-14 22:36:01.000000 vision6D-0.1.0/test/test_projection.py
+drwxrwxrwx   0        0        0        0 2023-05-28 00:07:30.360335 vision6D-0.1.0/vision6D/
+-rw-rw-rw-   0        0        0    48021 2023-05-28 00:06:16.000000 vision6D-0.1.0/vision6D/GUI.py
+-rw-rw-rw-   0        0        0      939 2023-05-28 00:06:17.000000 vision6D-0.1.0/vision6D/__init__.py
+-rw-rw-rw-   0        0        0    19331 2023-05-14 22:36:01.000000 vision6D-0.1.0/vision6D/app.py
+-rw-rw-rw-   0        0        0    12369 2023-05-28 00:06:17.000000 vision6D-0.1.0/vision6D/config.py
+drwxrwxrwx   0        0        0        0 2023-05-28 00:07:30.499332 vision6D-0.1.0/vision6D/data/
+-rw-rw-rw-   0        0        0   445902 2023-05-14 22:36:01.000000 vision6D-0.1.0/vision6D/data/ossiclesCoordinateMapping.json
+-rw-rw-rw-   0        0        0   335336 2023-05-14 22:36:02.000000 vision6D-0.1.0/vision6D/data/ossiclesCoordinateMappingv1.json
+-rw-rw-rw-   0        0        0    12109 2023-05-15 22:13:50.000000 vision6D-0.1.0/vision6D/data/style.qss
+-rw-rw-rw-   0        0        0    22897 2023-05-14 22:36:02.000000 vision6D-0.1.0/vision6D/interface.py
+-rw-rw-rw-   0        0        0    27532 2023-05-28 00:06:17.000000 vision6D-0.1.0/vision6D/interface_gui.py
+-rw-rw-rw-   0        0        0    33713 2023-05-14 22:36:02.000000 vision6D-0.1.0/vision6D/mainwindow.py
+-rw-rw-rw-   0        0        0    14068 2023-05-15 23:19:36.000000 vision6D-0.1.0/vision6D/run_gui.py
+-rw-rw-rw-   0        0        0      197 2023-05-14 22:53:44.000000 vision6D-0.1.0/vision6D/run_interface.py
+-rw-rw-rw-   0        0        0    14911 2023-05-14 22:36:02.000000 vision6D-0.1.0/vision6D/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-28 00:07:30.443333 vision6D-0.1.0/vision6D.egg-info/
+-rw-rw-rw-   0        0        0     1603 2023-05-28 00:07:29.000000 vision6D-0.1.0/vision6D.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      597 2023-05-28 00:07:29.000000 vision6D-0.1.0/vision6D.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-28 00:07:29.000000 vision6D-0.1.0/vision6D.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      164 2023-05-28 00:07:29.000000 vision6D-0.1.0/vision6D.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-28 00:07:29.000000 vision6D-0.1.0/vision6D.egg-info/top_level.txt
```

### Comparing `vision6D-0.0.9/LICENSE` & `vision6D-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vision6D-0.0.9/PKG-INFO` & `vision6D-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vision6D
-Version: 0.0.9
+Version: 0.1.0
 Summary: vision6D: A tool for 6D pose estimation annotation
 Home-page: https://github.com/ykzzky/vision6D
 License: GNU GENERAL Public License
 Project-URL: Bug Tracker, https://github.com/ykzzky/vision6D/issues
 Keywords: multimodal,data,analysis,real-time,distributed
 Platform: any
 Classifier: Programming Language :: Python :: 3
```

### Comparing `vision6D-0.0.9/README.md` & `vision6D-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `vision6D-0.0.9/setup.cfg` & `vision6D-0.1.0/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2076 6973 696f 6e36 440d 0a76 6572   = vision6D..ver
-00000020: 7369 6f6e 203d 2030 2e30 2e39 0d0a 7572  sion = 0.0.9..ur
+00000020: 7369 6f6e 203d 2030 2e31 2e30 0d0a 7572  sion = 0.1.0..ur
 00000030: 6c20 3d20 6874 7470 733a 2f2f 6769 7468  l = https://gith
 00000040: 7562 2e63 6f6d 2f79 6b7a 7a6b 792f 7669  ub.com/ykzzky/vi
 00000050: 7369 6f6e 3644 0d0a 6465 7363 7269 7074  sion6D..descript
 00000060: 696f 6e20 3d20 7669 7369 6f6e 3644 3a20  ion = vision6D: 
 00000070: 4120 746f 6f6c 2066 6f72 2036 4420 706f  A tool for 6D po
 00000080: 7365 2065 7374 696d 6174 696f 6e20 616e  se estimation an
 00000090: 6e6f 7461 7469 6f6e 0d0a 6c6f 6e67 5f64  notation..long_d
```

### Comparing `vision6D-0.0.9/test/test_create_dataset.py` & `vision6D-0.1.0/test/test_create_dataset.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.0.9/test/test_projection.py` & `vision6D-0.1.0/test/test_projection.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.0.9/vision6D/GUI.py` & `vision6D-0.1.0/vision6D/GUI.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import functools
 import trimesh
 import pathlib
 import PIL
 import ast
 import json
 import math
+import copy
 
 # Qt5 import
 from PyQt5 import QtWidgets, QtGui
 from pyvistaqt import QtInteractor, MainWindow
 from PyQt5.QtCore import Qt, QPoint
 
 # self defined package import
@@ -91,31 +92,52 @@
                 self.args4.text(),
                 self.args5.text(),
                 self.args6.text())
     
 class GetTextDialog(QtWidgets.QDialog):
     def __init__(self, parent=None):
         super(GetTextDialog, self).__init__(parent)
+
+        layout = QtWidgets.QVBoxLayout(self)
         
         self.setWindowTitle("Vision6D")
         self.introLabel = QtWidgets.QLabel("Input the Ground Truth Pose:")
+        self.btnloadfromfile = QtWidgets.QPushButton("Load from file", self)
+
+        hbox = QtWidgets.QHBoxLayout()
+        hbox.addWidget(self.introLabel)
+        hbox.addWidget(self.btnloadfromfile)
+        hbox.setContentsMargins(0, 0, 0, 0)
+        self.hboxWidget = QtWidgets.QWidget()
+        self.hboxWidget.setLayout(hbox)
+
+        self.btnloadfromfile.clicked.connect(self.load_from_file)
         self.textEdit = QtWidgets.QTextEdit(self)
         self.textEdit.setPlainText(f"[[1, 0, 0, 0], \n[0, 1, 0, 0], \n[0, 0, 1, 0], \n[0, 0, 0, 1]]")
         self.btnSubmit = QtWidgets.QPushButton("Submit", self)
         self.btnSubmit.clicked.connect(self.submit_text)
 
-        layout = QtWidgets.QVBoxLayout(self)
-        layout.addWidget(self.introLabel)
+        layout.addWidget(self.hboxWidget)
         layout.addWidget(self.textEdit)
         layout.addWidget(self.btnSubmit)
 
     def submit_text(self):
         self.user_text = self.textEdit.toPlainText()
         self.accept()
 
+    def load_from_file(self):
+        file_dialog = QtWidgets.QFileDialog()
+        pose_path, _ = file_dialog.getOpenFileName(None, "Open file", "", "Files (*.npy)")
+        if pose_path != '':
+            gt_pose = np.load(pose_path)
+            self.textEdit.setPlainText(f"[[{np.around(gt_pose[0, 0], 8)}, {np.around(gt_pose[0, 1], 8)}, {np.around(gt_pose[0, 2], 8)}, {np.around(gt_pose[0, 3], 8)}],\n"
+                                    f"[{np.around(gt_pose[1, 0], 8)}, {np.around(gt_pose[1, 1], 8)}, {np.around(gt_pose[1, 2], 8)}, {np.around(gt_pose[1, 3], 8)}],\n"
+                                    f"[{np.around(gt_pose[2, 0], 8)}, {np.around(gt_pose[2, 1], 8)}, {np.around(gt_pose[2, 2], 8)}, {np.around(gt_pose[2, 3], 8)}],\n"
+                                    f"[{np.around(gt_pose[3, 0], 8)}, {np.around(gt_pose[3, 1], 8)}, {np.around(gt_pose[3, 2], 8)}, {np.around(gt_pose[3, 3], 8)}]]")
+
     def get_text(self):
         return self.user_text
 
 class MyMainWindow(MainWindow):
     def __init__(self, parent=None):
         QtWidgets.QMainWindow.__init__(self, parent)
 
@@ -125,14 +147,16 @@
         self.main_widget = QtWidgets.QWidget()
         self.setCentralWidget(self.main_widget)
         self.setAcceptDrops(True)
 
         self.track_actors_names = []
         self.button_group_actors_names = QtWidgets.QButtonGroup(self)
 
+        self.toggle_hide_actors_flag = False
+
         # Set panel bar
         self.set_panel_bar()
         
         # Set menu bar
         self.set_menu_bars()
 
         # Create the plotter
@@ -422,43 +446,25 @@
             self.transformation_matrix = transformation_matrix
             if self.mirror_x: transformation_matrix = np.array([[-1, 0, 0, 0], [0, 1, 0, 0], [0, 0, 1, 0], [0, 0, 0, 1]]) @ transformation_matrix
             if self.mirror_y: transformation_matrix = np.array([[1, 0, 0, 0], [0, -1, 0, 0], [0, 0, 1, 0], [0, 0, 0, 1]]) @ transformation_matrix
             self.add_pose(matrix=transformation_matrix)
     
     def mirror_actors(self, direction):
 
-        if direction == 'x': mirror_x = True; mirror_y = False
-        elif direction == 'y': mirror_x = False; mirror_y = True
+        if direction == 'x': self.mirror_x = not self.mirror_x
+        elif direction == 'y': self.mirror_y = not self.mirror_y
 
         #^ mirror the image actor
         if self.image_actor is not None:
             original_image_data = np.array(PIL.Image.open(self.image_path), dtype='uint8')
             if len(original_image_data.shape) == 2: original_image_data = original_image_data[..., None]
-            curr_image_data = vis.utils.get_image_mask_actor_scalars(self.image_actor)
-            if mirror_x: curr_image_data = curr_image_data[:, ::-1, :]
-            if mirror_y: curr_image_data = curr_image_data[::-1, :, :]
-            if (curr_image_data == original_image_data).all(): 
-                self.mirror_x = False
-                self.mirror_y = False
-            elif (curr_image_data == original_image_data[:, ::-1, :]).all(): 
-                self.mirror_x = True
-                self.mirror_y = False
-            elif (curr_image_data == original_image_data[::-1, :, :]).all():
-                self.mirror_x = False
-                self.mirror_y = True
-            elif (curr_image_data == original_image_data[:, ::-1, :][::-1, :, :]).all():
-                self.mirror_x = True
-                self.mirror_y = True
             self.add_image(original_image_data)
-        else:
-            QtWidgets.QMessageBox.warning(self, 'vision6D', "Need to load an image first!", QtWidgets.QMessageBox.Ok, QtWidgets.QMessageBox.Ok)
-            return 0
 
+        #^ mirror the mask actor
         if self.mask_actor is not None:
-            #^ mirror the mask actor
             original_mask_data = np.array(PIL.Image.open(self.mask_path), dtype='uint8')
             if len(original_mask_data.shape) == 2: original_mask_data = original_mask_data[..., None]
             self.add_mask(original_mask_data)
 
         #^ mirror the mesh actors
         if len(self.mesh_actors) != 0:
             for actor_name, _ in self.mesh_actors.items():
@@ -521,15 +527,19 @@
         # Re-initial the dictionaries
         self.image_path = None
         self.mask_path = None
         self.mesh_path = None
         self.pose_path = None
         self.meshdict = {}
         self.mesh_colors = {}
+
+        # reset everything to original actor opacity
         self.mesh_opacity = {}
+        self.image_opacity = 0.99
+        self.mask_opacity = 0.5
 
         self.image_spacing = [0.01, 0.01, 1]
         self.mask_spacing = [0.01, 0.01, 1]
         self.mesh_spacing = [1, 1, 1]
 
         self.mirror_x = False
         self.mirror_y = False
@@ -811,53 +821,95 @@
             else: 
                 self.mesh_opacity[actor_name] = value / 100
                 self.set_mesh_opacity(actor_name, self.mesh_opacity[actor_name])
             self.output_text.clear()
             self.output_text.append(f"Current actor <span style='background-color:yellow; color:black;'>{actor_name}</span>'s opacity is {value / 100}")
         else:
             self.ignore_slider_value_change = True
-            self.opacity_slider.setValue(100)
+            self.opacity_slider.setValue(value)
             self.ignore_slider_value_change = False
-            QtWidgets.QMessageBox.warning(self, 'vision6D', "Need to select an actor first", QtWidgets.QMessageBox.Ok, QtWidgets.QMessageBox.Ok)
             return 0
         
+    def toggle_hide_actors_button(self):
+        self.toggle_hide_actors_flag = not self.toggle_hide_actors_flag
+        
+        if self.toggle_hide_actors_flag:
+            for button in self.button_group_actors_names.buttons():
+                button.setChecked(True)
+                actor_name = button.text()
+                if actor_name == 'image': self.store_image_opacity = copy.deepcopy(self.image_opacity)
+                elif actor_name == 'mask': self.store_mask_opacity = copy.deepcopy(self.mask_opacity)
+                else: self.store_mesh_opacity[actor_name] = copy.deepcopy(self.mesh_opacity[actor_name])
+                self.opacity_value_change(0)
+
+            self.ignore_slider_value_change = True
+            self.opacity_slider.setValue(0)
+            self.ignore_slider_value_change = False
+                
+            checked_button = self.button_group_actors_names.checkedButton()
+            if checked_button is None: QtWidgets.QMessageBox.warning(self, 'vision6D', "Need to select an actor first", QtWidgets.QMessageBox.Ok, QtWidgets.QMessageBox.Ok)
+        
+        else:
+            for button in self.button_group_actors_names.buttons():
+                button.setChecked(True)
+                actor_name = button.text()
+                if actor_name == 'image': self.opacity_value_change(self.store_image_opacity * 100)
+                elif actor_name == 'mask': self.opacity_value_change(self.store_mask_opacity * 100)
+                else: self.opacity_value_change(self.store_mesh_opacity[actor_name] * 100)
+
+            checked_button = self.button_group_actors_names.checkedButton()
+            if checked_button is not None:
+                actor_name = checked_button.text()
+                self.ignore_slider_value_change = True
+                if actor_name == 'image': self.opacity_slider.setValue(self.image_opacity * 100)
+                elif actor_name == 'mask': self.opacity_slider.setValue(self.mask_opacity * 100)
+                else: self.opacity_slider.setValue(self.mesh_opacity[actor_name] * 100)
+                self.ignore_slider_value_change = False
+            else:
+                QtWidgets.QMessageBox.warning(self, 'vision6D', "Need to select an actor first", QtWidgets.QMessageBox.Ok, QtWidgets.QMessageBox.Ok)
+
     def panel_display(self):
         self.display = QtWidgets.QGroupBox("Console")
         display_layout = QtWidgets.QVBoxLayout()
         display_layout.setContentsMargins(10, 20, 10, 10)
 
         #* Create the top widgets (layout)
         top_layout = QtWidgets.QHBoxLayout()
         top_layout.setContentsMargins(0, 10, 0, 10)
 
         # Create the color dropdown menu (comboBox)
         self.color_button = QtWidgets.QPushButton("Color")
         self.color_button.clicked.connect(self.show_color_popup)
-        top_layout.addWidget(self.color_button, 0.5) # 1 is for the stretch factor
+        top_layout.addWidget(self.color_button, 1) # 1 is for the stretch factor
 
         # Create the color dropdown menu (comboBox)
         self.spacing_button = QtWidgets.QPushButton("Spacing")
         self.spacing_button.clicked.connect(self.set_spacing)
-        top_layout.addWidget(self.spacing_button, 0.5) # 1 is for the stretch factor
+        top_layout.addWidget(self.spacing_button, 1) # 1 is for the stretch factor
 
         # Create the opacity slider
         self.opacity_slider = QtWidgets.QSlider(Qt.Horizontal)
         self.opacity_slider.setMinimum(0)
         self.opacity_slider.setMaximum(100)
         self.opacity_slider.setValue(100)
         self.opacity_slider.setTickPosition(QtWidgets.QSlider.TicksBelow)
         self.opacity_slider.setSingleStep(1)
         self.ignore_slider_value_change = False 
         self.opacity_slider.valueChanged.connect(self.opacity_value_change)
-        top_layout.addWidget(self.opacity_slider, 1)
+        top_layout.addWidget(self.opacity_slider, 1.5)
+
+        # Create the hide button
+        hide_button = QtWidgets.QPushButton("toggle hide")
+        hide_button.clicked.connect(self.toggle_hide_actors_button)
+        top_layout.addWidget(hide_button, 1)
 
-        # Create the second button
+        # Create the remove button
         remove_button = QtWidgets.QPushButton("Remove")
         remove_button.clicked.connect(self.remove_actors_button)
-        top_layout.addWidget(remove_button, 0.5)
+        top_layout.addWidget(remove_button, 1)
 
         display_layout.addLayout(top_layout)
 
         #* Create the bottom widgets
         actor_widget = QtWidgets.QLabel("Actors")
         display_layout.addWidget(actor_widget)
```

### Comparing `vision6D-0.0.9/vision6D/__init__.py` & `vision6D-0.1.0/vision6D/__init__.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.0.9/vision6D/app.py` & `vision6D-0.1.0/vision6D/app.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.0.9/vision6D/config.py` & `vision6D-0.1.0/vision6D/config.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.0.9/vision6D/data/ossiclesCoordinateMapping.json` & `vision6D-0.1.0/vision6D/data/ossiclesCoordinateMapping.json`

 * *Files identical despite different names*

### Comparing `vision6D-0.0.9/vision6D/data/ossiclesCoordinateMappingv1.json` & `vision6D-0.1.0/vision6D/data/ossiclesCoordinateMappingv1.json`

 * *Files identical despite different names*

### Comparing `vision6D-0.0.9/vision6D/data/style.qss` & `vision6D-0.1.0/vision6D/data/style.qss`

 * *Files identical despite different names*

### Comparing `vision6D-0.0.9/vision6D/interface.py` & `vision6D-0.1.0/vision6D/interface.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.0.9/vision6D/interface_gui.py` & `vision6D-0.1.0/vision6D/interface_gui.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,20 +39,21 @@
         
         self.undo_poses = {}
         self.latlon = vis.utils.load_latitude_longitude()
 
         self.colors = ["cyan", "magenta", "yellow", "lime", "deepskyblue", "salmon", "silver", "aquamarine", "plum", "blueviolet"]
         self.used_colors = []
         self.mesh_colors = {}
-        self.mesh_opacity = {}
 
-        # default opacity for image and surface
+        self.mesh_opacity = {}
+        self.store_mesh_opacity = {}
         self.image_opacity = 0.99
         self.mask_opacity = 0.5
         self.surface_opacity = 0.8
+        
         self.image_spacing = [0.01, 0.01, 1]
         self.mask_spacing = [0.01, 0.01, 1]
         self.mesh_spacing = [1, 1, 1]
         
     def button_actor_name_clicked(self, text):
         if text in self.mesh_actors:
             # set the current mesh color
@@ -426,15 +427,14 @@
             if np.all(np.logical_or(mask_data == 0, mask_data == 1)):
                 if self.reference is not None:
                     colors = vis.utils.get_mesh_actor_scalars(self.mesh_actors[self.reference])
                     if colors is None or (np.all(colors == colors[0])):
                         QtWidgets.QMessageBox.warning(self, 'vision6D', "The mesh need to be colored with nocs or latlon with gradient color", QtWidgets.QMessageBox.Ok, QtWidgets.QMessageBox.Ok)
                         return 0
                     color_mask = self.export_mesh_plot(QtWidgets.QMessageBox.Yes, QtWidgets.QMessageBox.Yes, QtWidgets.QMessageBox.Yes, save_render=False)
-                    # nocs_color = False if np.sum(color_mask[..., 2]) == 0 else True
                     nocs_color = (self.mesh_colors[self.reference] == 'nocs')
                     gt_pose = self.mesh_actors[self.reference].user_matrix
                     if self.mirror_x: gt_pose = np.array([[-1, 0, 0, 0], [0, 1, 0, 0], [0, 0, 1, 0], [0, 0, 0, 1]]) @ gt_pose
                     if self.mirror_y: gt_pose = np.array([[1, 0, 0, 0], [0, -1, 0, 0], [0, 0, 1, 0], [0, 0, 0, 1]]) @ gt_pose
                     vertices, faces = vis.utils.get_mesh_actor_vertices_faces(self.mesh_actors[self.reference])
                     mesh = trimesh.Trimesh(vertices, faces, process=False)
                 else: 
@@ -469,17 +469,20 @@
                         self.output_text.clear()
                         self.output_text.append(f"The input ground truth pose is:\n[{gt_pose[0]}, \n{gt_pose[1]}, \n{gt_pose[2]}, \n{gt_pose[3]}]")
                         QtWidgets.QMessageBox.information(self, "Information", "Please load the corresponding mesh")
 
                         # add the mesh object file
                         self.transformation_matrix = gt_pose
                         self.add_mesh_file(prompt=True)
-                        checked_button = self.button_group_actors_names.checkedButton()
-                        vertices, faces = vis.utils.get_mesh_actor_vertices_faces(self.mesh_actors[checked_button.text()])
-                        mesh = trimesh.Trimesh(vertices, faces, process=False)
+                        if self.mesh_path != '':
+                            checked_button = self.button_group_actors_names.checkedButton()
+                            vertices, faces = vis.utils.get_mesh_actor_vertices_faces(self.mesh_actors[checked_button.text()])
+                            mesh = trimesh.Trimesh(vertices, faces, process=False)
+                        else:
+                            return 0
                     else:
                         QtWidgets.QMessageBox.warning(self, 'vision6D', "A color mask need to be loaded", QtWidgets.QMessageBox.Ok, QtWidgets.QMessageBox.Ok)
                         return 0
         
             if np.sum(color_mask) == 0:
                 QtWidgets.QMessageBox.warning(self, 'vision6D', "The color mask is blank (maybe set the reference mesh wrong)", QtWidgets.QMessageBox.Ok, QtWidgets.QMessageBox.Ok)
                 return 0
@@ -487,24 +490,19 @@
             if nocs_method == nocs_color:
                 if nocs_method: 
                     predicted_pose = self.nocs_epnp(color_mask, mesh)
                     if self.mirror_x: predicted_pose = np.array([[-1, 0, 0, 0], [0, 1, 0, 0], [0, 0, 1, 0], [0, 0, 0, 1]]) @ predicted_pose @ np.array([[-1, 0, 0, 0], [0, 1, 0, 0], [0, 0, 1, 0], [0, 0, 0, 1]])
                     if self.mirror_y: predicted_pose = np.array([[1, 0, 0, 0], [0, -1, 0, 0], [0, 0, 1, 0], [0, 0, 0, 1]]) @ predicted_pose @ np.array([[1, 0, 0, 0], [0, -1, 0, 0], [0, 0, 1, 0], [0, 0, 0, 1]])
                     color_theme = 'NOCS'
                 else: 
+                    if self.mirror_x: color_mask = color_mask[:, ::-1, :]
+                    if self.mirror_y: color_mask = color_mask[::-1, :, :]
                     predicted_pose = self.latlon_epnp(color_mask, mesh)
-                    if self.mirror_x: 
-                        predicted_pose = np.array([[-1, 0, 0, 0], [0, 1, 0, 0], [0, 0, -1, 0], [0, 0, 0, 1]]) @ predicted_pose
-                        predicted_pose[2, 3] = -1 * predicted_pose[2, 3] #^ interesting
-                    if self.mirror_y: 
-                        predicted_pose = np.array([[1, 0, 0, 0], [0, -1, 0, 0], [0, 0, -1, 0], [0, 0, 0, 1]]) @ predicted_pose
-                        predicted_pose[2, 3] = -1 * predicted_pose[2, 3] #^ interesting
                     color_theme = 'LATLON'
                 error = np.sum(np.abs(predicted_pose - gt_pose))
                 self.output_text.clear()
                 self.output_text.append(f"PREDICTED POSE WITH <span style='background-color:yellow; color:black;'>{color_theme} COLOR (MASKED)</span>: ")
                 self.output_text.append(f"\n{predicted_pose}\n\nGT POSE: \n\n{gt_pose}\n\nERROR: \n\n{error}")
-
             else:
                 QtWidgets.QMessageBox.warning(self,"vision6D", "Clicked the wrong method")
         else:
             QtWidgets.QMessageBox.warning(self,"vision6D", "please load a mask first")
```

### Comparing `vision6D-0.0.9/vision6D/mainwindow.py` & `vision6D-0.1.0/vision6D/mainwindow.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.0.9/vision6D/run_gui.py` & `vision6D-0.1.0/vision6D/run_gui.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.0.9/vision6D/utils.py` & `vision6D-0.1.0/vision6D/utils.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.0.9/vision6D.egg-info/PKG-INFO` & `vision6D-0.1.0/vision6D.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vision6D
-Version: 0.0.9
+Version: 0.1.0
 Summary: vision6D: A tool for 6D pose estimation annotation
 Home-page: https://github.com/ykzzky/vision6D
 License: GNU GENERAL Public License
 Project-URL: Bug Tracker, https://github.com/ykzzky/vision6D/issues
 Keywords: multimodal,data,analysis,real-time,distributed
 Platform: any
 Classifier: Programming Language :: Python :: 3
```

### Comparing `vision6D-0.0.9/vision6D.egg-info/SOURCES.txt` & `vision6D-0.1.0/vision6D.egg-info/SOURCES.txt`

 * *Files identical despite different names*

