# Comparing `tmp/vision6D-0.1.0.tar.gz` & `tmp/vision6D-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\vision6D-0.1.0.tar", last modified: Sun May 28 00:07:30 2023, max compression
+gzip compressed data, was "dist\vision6D-0.1.1.tar", last modified: Sun May 28 21:44:45 2023, max compression
```

## Comparing `vision6D-0.1.0.tar` & `vision6D-0.1.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-05-28 00:07:30.505332 vision6D-0.1.0/
--rw-rw-rw-   0        0        0     1086 2023-01-03 15:55:06.000000 vision6D-0.1.0/LICENSE
--rw-rw-rw-   0        0        0       33 2023-05-27 00:07:11.000000 vision6D-0.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0     1603 2023-05-28 00:07:30.505332 vision6D-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      918 2023-05-28 00:06:16.000000 vision6D-0.1.0/README.md
--rw-rw-rw-   0        0        0      413 2023-01-03 15:55:07.000000 vision6D-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0     1927 2023-05-28 00:07:30.511335 vision6D-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      165 2023-05-28 00:06:16.000000 vision6D-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-28 00:07:30.262457 vision6D-0.1.0/test/
--rw-rw-rw-   0        0        0    21974 2023-05-17 18:41:02.000000 vision6D-0.1.0/test/test_create_dataset.py
--rw-rw-rw-   0        0        0     3630 2023-05-14 22:36:01.000000 vision6D-0.1.0/test/test_projection.py
-drwxrwxrwx   0        0        0        0 2023-05-28 00:07:30.360335 vision6D-0.1.0/vision6D/
--rw-rw-rw-   0        0        0    48021 2023-05-28 00:06:16.000000 vision6D-0.1.0/vision6D/GUI.py
--rw-rw-rw-   0        0        0      939 2023-05-28 00:06:17.000000 vision6D-0.1.0/vision6D/__init__.py
--rw-rw-rw-   0        0        0    19331 2023-05-14 22:36:01.000000 vision6D-0.1.0/vision6D/app.py
--rw-rw-rw-   0        0        0    12369 2023-05-28 00:06:17.000000 vision6D-0.1.0/vision6D/config.py
-drwxrwxrwx   0        0        0        0 2023-05-28 00:07:30.499332 vision6D-0.1.0/vision6D/data/
--rw-rw-rw-   0        0        0   445902 2023-05-14 22:36:01.000000 vision6D-0.1.0/vision6D/data/ossiclesCoordinateMapping.json
--rw-rw-rw-   0        0        0   335336 2023-05-14 22:36:02.000000 vision6D-0.1.0/vision6D/data/ossiclesCoordinateMappingv1.json
--rw-rw-rw-   0        0        0    12109 2023-05-15 22:13:50.000000 vision6D-0.1.0/vision6D/data/style.qss
--rw-rw-rw-   0        0        0    22897 2023-05-14 22:36:02.000000 vision6D-0.1.0/vision6D/interface.py
--rw-rw-rw-   0        0        0    27532 2023-05-28 00:06:17.000000 vision6D-0.1.0/vision6D/interface_gui.py
--rw-rw-rw-   0        0        0    33713 2023-05-14 22:36:02.000000 vision6D-0.1.0/vision6D/mainwindow.py
--rw-rw-rw-   0        0        0    14068 2023-05-15 23:19:36.000000 vision6D-0.1.0/vision6D/run_gui.py
--rw-rw-rw-   0        0        0      197 2023-05-14 22:53:44.000000 vision6D-0.1.0/vision6D/run_interface.py
--rw-rw-rw-   0        0        0    14911 2023-05-14 22:36:02.000000 vision6D-0.1.0/vision6D/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-28 00:07:30.443333 vision6D-0.1.0/vision6D.egg-info/
--rw-rw-rw-   0        0        0     1603 2023-05-28 00:07:29.000000 vision6D-0.1.0/vision6D.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      597 2023-05-28 00:07:29.000000 vision6D-0.1.0/vision6D.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-28 00:07:29.000000 vision6D-0.1.0/vision6D.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      164 2023-05-28 00:07:29.000000 vision6D-0.1.0/vision6D.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-28 00:07:29.000000 vision6D-0.1.0/vision6D.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-28 21:44:45.160272 vision6D-0.1.1/
+-rw-rw-rw-   0        0        0     1086 2023-01-03 15:55:06.000000 vision6D-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0       33 2023-05-27 00:07:11.000000 vision6D-0.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     1603 2023-05-28 21:44:45.161273 vision6D-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      918 2023-05-28 01:21:42.000000 vision6D-0.1.1/README.md
+-rw-rw-rw-   0        0        0      413 2023-01-03 15:55:07.000000 vision6D-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0     1927 2023-05-28 21:44:45.168279 vision6D-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      165 2023-05-28 01:21:42.000000 vision6D-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-28 21:44:44.897270 vision6D-0.1.1/test/
+-rw-rw-rw-   0        0        0    21974 2023-05-17 18:41:02.000000 vision6D-0.1.1/test/test_create_dataset.py
+-rw-rw-rw-   0        0        0     3630 2023-05-14 22:36:01.000000 vision6D-0.1.1/test/test_projection.py
+drwxrwxrwx   0        0        0        0 2023-05-28 21:44:45.034308 vision6D-0.1.1/vision6D/
+-rw-rw-rw-   0        0        0    50430 2023-05-28 21:28:42.000000 vision6D-0.1.1/vision6D/GUI.py
+-rw-rw-rw-   0        0        0      939 2023-05-28 01:21:42.000000 vision6D-0.1.1/vision6D/__init__.py
+-rw-rw-rw-   0        0        0    19331 2023-05-14 22:36:01.000000 vision6D-0.1.1/vision6D/app.py
+-rw-rw-rw-   0        0        0    12369 2023-05-28 01:21:42.000000 vision6D-0.1.1/vision6D/config.py
+drwxrwxrwx   0        0        0        0 2023-05-28 21:44:45.156274 vision6D-0.1.1/vision6D/data/
+-rw-rw-rw-   0        0        0   445902 2023-05-14 22:36:01.000000 vision6D-0.1.1/vision6D/data/ossiclesCoordinateMapping.json
+-rw-rw-rw-   0        0        0   335336 2023-05-14 22:36:02.000000 vision6D-0.1.1/vision6D/data/ossiclesCoordinateMappingv1.json
+-rw-rw-rw-   0        0        0    12109 2023-05-15 22:13:50.000000 vision6D-0.1.1/vision6D/data/style.qss
+-rw-rw-rw-   0        0        0    22897 2023-05-14 22:36:02.000000 vision6D-0.1.1/vision6D/interface.py
+-rw-rw-rw-   0        0        0    26131 2023-05-28 21:42:04.000000 vision6D-0.1.1/vision6D/interface_gui.py
+-rw-rw-rw-   0        0        0    33713 2023-05-14 22:36:02.000000 vision6D-0.1.1/vision6D/mainwindow.py
+-rw-rw-rw-   0        0        0    14068 2023-05-15 23:19:36.000000 vision6D-0.1.1/vision6D/run_gui.py
+-rw-rw-rw-   0        0        0      197 2023-05-14 22:53:44.000000 vision6D-0.1.1/vision6D/run_interface.py
+-rw-rw-rw-   0        0        0    14911 2023-05-14 22:36:02.000000 vision6D-0.1.1/vision6D/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-28 21:44:45.106272 vision6D-0.1.1/vision6D.egg-info/
+-rw-rw-rw-   0        0        0     1603 2023-05-28 21:44:44.000000 vision6D-0.1.1/vision6D.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      597 2023-05-28 21:44:44.000000 vision6D-0.1.1/vision6D.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-28 21:44:44.000000 vision6D-0.1.1/vision6D.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      164 2023-05-28 21:44:44.000000 vision6D-0.1.1/vision6D.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-28 21:44:44.000000 vision6D-0.1.1/vision6D.egg-info/top_level.txt
```

### Comparing `vision6D-0.1.0/LICENSE` & `vision6D-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vision6D-0.1.0/PKG-INFO` & `vision6D-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vision6D
-Version: 0.1.0
+Version: 0.1.1
 Summary: vision6D: A tool for 6D pose estimation annotation
 Home-page: https://github.com/ykzzky/vision6D
 License: GNU GENERAL Public License
 Project-URL: Bug Tracker, https://github.com/ykzzky/vision6D/issues
 Keywords: multimodal,data,analysis,real-time,distributed
 Platform: any
 Classifier: Programming Language :: Python :: 3
```

### Comparing `vision6D-0.1.0/README.md` & `vision6D-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `vision6D-0.1.0/setup.cfg` & `vision6D-0.1.1/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2076 6973 696f 6e36 440d 0a76 6572   = vision6D..ver
-00000020: 7369 6f6e 203d 2030 2e31 2e30 0d0a 7572  sion = 0.1.0..ur
+00000020: 7369 6f6e 203d 2030 2e31 2e31 0d0a 7572  sion = 0.1.1..ur
 00000030: 6c20 3d20 6874 7470 733a 2f2f 6769 7468  l = https://gith
 00000040: 7562 2e63 6f6d 2f79 6b7a 7a6b 792f 7669  ub.com/ykzzky/vi
 00000050: 7369 6f6e 3644 0d0a 6465 7363 7269 7074  sion6D..descript
 00000060: 696f 6e20 3d20 7669 7369 6f6e 3644 3a20  ion = vision6D: 
 00000070: 4120 746f 6f6c 2066 6f72 2036 4420 706f  A tool for 6D po
 00000080: 7365 2065 7374 696d 6174 696f 6e20 616e  se estimation an
 00000090: 6e6f 7461 7469 6f6e 0d0a 6c6f 6e67 5f64  notation..long_d
```

### Comparing `vision6D-0.1.0/test/test_create_dataset.py` & `vision6D-0.1.1/test/test_create_dataset.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.1.0/test/test_projection.py` & `vision6D-0.1.1/test/test_projection.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.1.0/vision6D/GUI.py` & `vision6D-0.1.1/vision6D/GUI.py`

 * *Files 5% similar despite different names*

```diff
@@ -217,15 +217,15 @@
                         self.mask_path = file_path
                         self.add_mask_file(prompt=False)
                     elif button_clicked == QtWidgets.QMessageBox.No:
                         self.image_path = file_path
                         self.add_image_file(prompt=False)
             elif file_path.endswith('.npy'):
                 self.pose_path = file_path
-                self.add_pose_file(prompt=False)
+                self.add_pose_file()
             else:
                 QtWidgets.QMessageBox.warning(self, 'vision6D', "File format is not supported!", QtWidgets.QMessageBox.Ok, QtWidgets.QMessageBox.Ok)
                 return 0
 
     def resizeEvent(self, e):
         x = (self.plotter.size().width() - self.hintLabel.width()) // 2
         y = (self.plotter.size().height() - self.hintLabel.height()) // 2
@@ -249,28 +249,26 @@
             
         # allow to add files
         fileMenu = mainMenu.addMenu('File')
         fileMenu.addAction('Add Workspace', self.add_workspace)
         fileMenu.addAction('Add Image', self.add_image_file)
         fileMenu.addAction('Add Mask', self.add_mask_file)
         fileMenu.addAction('Add Mesh', self.add_mesh_file)
-        fileMenu.addAction('Add Pose', self.add_pose_file)
         fileMenu.addAction('Clear', self.clear_plot)
 
         # allow to export files
         exportMenu = mainMenu.addMenu('Export')
         exportMenu.addAction('Image Render', self.export_image_plot)
         exportMenu.addAction('Mask Render', self.export_mask_plot)
         exportMenu.addAction('Mesh Render', self.export_mesh_plot)
         exportMenu.addAction('SegMesh Render', self.export_segmesh_plot)
         exportMenu.addAction('Pose', self.export_pose)
                 
         # Add camera related actions
         CameraMenu = mainMenu.addMenu('Camera')
-        CameraMenu.addAction('Set Camera', self.set_camera)
         CameraMenu.addAction('Reset Camera (c)', self.reset_camera)
         CameraMenu.addAction('Zoom In (x)', self.zoom_in)
         CameraMenu.addAction('Zoom Out (z)', self.zoom_out)
 
         # add mirror actors related actions
         mirrorMenu = mainMenu.addMenu('Mirror')
         mirror_x = functools.partial(self.mirror_actors, direction='x')
@@ -338,14 +336,39 @@
                 try:
                     self.fx, self.fy, self.cx, self.cy, self.cam_viewup, self.cam_position = ast.literal_eval(fx), ast.literal_eval(fy), ast.literal_eval(cx), ast.literal_eval(cy), ast.literal_eval(cam_viewup), ast.literal_eval(cam_position)
                     self.set_camera_props()
                 except:
                     self.fx, self.fy, self.cx, self.cy, self.cam_viewup, self.cam_position = pre_fx, pre_fy, pre_cx, pre_cy, pre_cam_viewup, pre_cam_position
                     QtWidgets.QMessageBox.warning(self, 'vision6D', "Error occured, check the format of the input values", QtWidgets.QMessageBox.Ok, QtWidgets.QMessageBox.Ok)
 
+    def set_pose(self):
+        # get the gt pose
+        res = self.get_text_dialog.exec_()
+
+        if res == QtWidgets.QDialog.Accepted:
+            try:
+                gt_pose = ast.literal_eval(self.get_text_dialog.user_text)
+                gt_pose = np.array(gt_pose)
+                if gt_pose.shape != (4, 4): 
+                    QtWidgets.QMessageBox.warning(self, 'vision6D', "It needs to be a 4 by 4 matrix", QtWidgets.QMessageBox.Ok, QtWidgets.QMessageBox.Ok) 
+                    return None
+                else:
+                    self.hintLabel.hide()
+                    transformation_matrix = gt_pose
+                    self.transformation_matrix = transformation_matrix
+                    if self.mirror_x: transformation_matrix = np.array([[-1, 0, 0, 0], [0, 1, 0, 0], [0, 0, 1, 0], [0, 0, 0, 1]]) @ transformation_matrix
+                    if self.mirror_y: transformation_matrix = np.array([[1, 0, 0, 0], [0, -1, 0, 0], [0, 0, 1, 0], [0, 0, 0, 1]]) @ transformation_matrix
+                    self.add_pose(matrix=transformation_matrix)
+                    return 0
+            except: 
+                QtWidgets.QMessageBox.warning(self, 'vision6D', "Format is not correct", QtWidgets.QMessageBox.Ok, QtWidgets.QMessageBox.Ok)
+                return None
+        else: 
+            return None
+
     def set_spacing(self):
         checked_button = self.button_group_actors_names.checkedButton()
         if checked_button is not None:
             if checked_button.text() == 'image':
                 spacing, ok = self.input_dialog.getText(self, 'Input', "Set Spacing", text=str(self.image_spacing))
                 if ok:
                     try: self.image_spacing = ast.literal_eval(spacing)
@@ -377,74 +400,68 @@
             self.image_path = workspace['image_path']
             self.mask_path = workspace['mask_path']
             self.pose_path = workspace['pose_path']
             mesh_paths = workspace['mesh_path']
 
             self.add_image_file(prompt=False)
             self.add_mask_file(prompt=False)
-            self.add_pose_file(prompt=False)
+            self.add_pose_file()
 
             for item in mesh_paths.items():
                 mesh_name, self.mesh_path = item
                 self.add_mesh_file(mesh_name=mesh_name, prompt=False)
 
     def add_image_file(self, prompt=True):
         if prompt:
             if self.image_path == None or self.image_path == '':
                 self.image_path, _ = self.file_dialog.getOpenFileName(None, "Open file", "", "Files (*.png *.jpg)")
             else:
                 self.image_path, _ = self.file_dialog.getOpenFileName(None, "Open file", str(pathlib.Path(self.image_path).parent), "Files (*.png *.jpg)")
 
-        if self.image_path != '':
+        if self.image_path != '' and self.image_path is not None:
             self.hintLabel.hide()
             image_source = np.array(PIL.Image.open(self.image_path), dtype='uint8')
             if len(image_source.shape) == 2: image_source = image_source[..., None]
             self.add_image(image_source)
             
     def add_mask_file(self, prompt=True):
         if prompt:
             if self.mask_path == None or self.mask_path == '':
                 self.mask_path, _ = self.file_dialog.getOpenFileName(None, "Open file", "", "Files (*.png *.jpg)")
             else:
                 self.mask_path, _ = self.file_dialog.getOpenFileName(None, "Open file", str(pathlib.Path(self.mask_path).parent), "Files (*.png *.jpg)")
         
-        if self.mask_path != '':
+        if self.mask_path != '' and self.mask_path is not None:
             self.hintLabel.hide()
             mask_source = np.array(PIL.Image.open(self.mask_path), dtype='uint8')
             if len(mask_source.shape) == 2: mask_source = mask_source[..., None]
             self.add_mask(mask_source)
 
     def add_mesh_file(self, mesh_name=None, prompt=True):
         if prompt:
             if self.mesh_path == None or self.mesh_path == '':
                 self.mesh_path, _ = self.file_dialog.getOpenFileName(None, "Open file", "", "Files (*.mesh *.ply *.stl *.obj *.off *.dae *.fbx *.3ds *.x3d)")
             else:
                 self.mesh_path, _ = self.file_dialog.getOpenFileName(None, "Open file", str(pathlib.Path(self.mesh_path).parent), "Files (*.mesh *.ply)")
         
-        if self.mesh_path != '':
+        if self.mesh_path != '' and self.mesh_path is not None:
             self.hintLabel.hide()
             if mesh_name is None:
                 mesh_name, ok = self.input_dialog.getText(self, 'Input', 'Specify the object Class name')#, text='ossicles')
                 if not ok: return 0
 
             self.meshdict[mesh_name] = self.mesh_path
             self.mesh_opacity[mesh_name] = self.surface_opacity
             transformation_matrix = self.transformation_matrix
             if self.mirror_x: transformation_matrix = np.array([[-1, 0, 0, 0], [0, 1, 0, 0], [0, 0, 1, 0], [0, 0, 0, 1]]) @ transformation_matrix
             if self.mirror_y: transformation_matrix = np.array([[1, 0, 0, 0], [0, -1, 0, 0], [0, 0, 1, 0], [0, 0, 0, 1]]) @ transformation_matrix                   
             self.add_mesh(mesh_name, self.mesh_path, transformation_matrix)
                       
-    def add_pose_file(self, prompt=True):
-        if prompt:
-            if self.pose_path == None or self.pose_path == '':
-                self.pose_path, _ = self.file_dialog.getOpenFileName(None, "Open file", "", "Files (*.npy)")
-            else:
-                self.pose_path, _ = self.file_dialog.getOpenFileName(None, "Open file", str(pathlib.Path(self.pose_path).parent), "Files (*.npy)")
-        
-        if self.pose_path != '':
+    def add_pose_file(self):
+        if self.pose_path != '' and self.pose_path is not None:
             self.hintLabel.hide()
             transformation_matrix = np.load(self.pose_path)
             self.transformation_matrix = transformation_matrix
             if self.mirror_x: transformation_matrix = np.array([[-1, 0, 0, 0], [0, 1, 0, 0], [0, 0, 1, 0], [0, 0, 0, 1]]) @ transformation_matrix
             if self.mirror_y: transformation_matrix = np.array([[1, 0, 0, 0], [0, -1, 0, 0], [0, 0, 1, 0], [0, 0, 0, 1]]) @ transformation_matrix
             self.add_pose(matrix=transformation_matrix)
     
@@ -468,15 +485,18 @@
         #^ mirror the mesh actors
         if len(self.mesh_actors) != 0:
             for actor_name, _ in self.mesh_actors.items():
                 transformation_matrix = self.transformation_matrix
                 if self.mirror_x: transformation_matrix = np.array([[-1, 0, 0, 0], [0, 1, 0, 0], [0, 0, 1, 0], [0, 0, 0, 1]]) @ transformation_matrix
                 if self.mirror_y: transformation_matrix = np.array([[1, 0, 0, 0], [0, -1, 0, 0], [0, 0, 1, 0], [0, 0, 0, 1]]) @ transformation_matrix
                 self.add_mesh(actor_name, self.meshdict[actor_name], transformation_matrix)
-                
+            
+            # Output the mirrored transformation matrix
+            self.output_text.append(f"-> Mirrored transformation matrix is: \n{transformation_matrix}")
+             
     def remove_actor(self, button):
         name = button.text()
         if name == 'image': 
             actor = self.image_actor
             self.image_actor = None
             self.image_path = None
         elif name == 'mask':
@@ -491,15 +511,15 @@
             del self.meshdict[name]
             self.reference = None
             self.color_button.setText("Color")
             self.mesh_spacing = [1, 1, 1]
 
         self.plotter.remove_actor(actor)
         self.track_actors_names.remove(name)
-        self.output_text.clear(); self.output_text.append(f"Remove actor: <span style='background-color:yellow; color:black;'>{name}</span>")
+        self.output_text.append(f"-> Remove actor: <span style='background-color:yellow; color:black;'>{name}</span>")
         # remove the button from the button group
         self.button_group_actors_names.removeButton(button)
         # remove the button from the self.button_layout widget
         self.button_layout.removeWidget(button)
         # offically delete the button
         button.deleteLater()
 
@@ -552,15 +572,14 @@
         self.undo_poses = {}
         self.track_actors_names = []
 
         self.colors = ["cyan", "magenta", "yellow", "lime", "deepskyblue", "salmon", "silver", "aquamarine", "plum", "blueviolet"]
         self.used_colors = []
         self.color_button.setText("Color")
 
-        self.output_text.clear()
         self.ignore_slider_value_change = True
         self.opacity_slider.setValue(100)
         self.ignore_slider_value_change = False
 
     def export_image_plot(self):
 
         if self.image_actor is None:
@@ -581,16 +600,15 @@
 
         # obtain the rendered image
         image = self.render.last_image
         output_path, _ = QtWidgets.QFileDialog.getSaveFileName(self, "Save File", "", "Image Files (*.png)")
         if output_path: 
             rendered_image = PIL.Image.fromarray(image)
             rendered_image.save(output_path)
-            self.output_text.clear()
-            self.output_text.append(f"Export image render to:\n {str(output_path)}")
+            self.output_text.append(f"-> Export image render to:\n {str(output_path)}")
 
     def export_mask_plot(self):
         if self.mask_actor is None:
             QtWidgets.QMessageBox.warning(self, 'vision6D', "Need to load a mask first!", QtWidgets.QMessageBox.Ok, QtWidgets.QMessageBox.Ok)
             return 0
         
         reply = QtWidgets.QMessageBox.question(self,"vision6D", "Reset Camera?", QtWidgets.QMessageBox.Yes, QtWidgets.QMessageBox.No)
@@ -607,16 +625,15 @@
 
         # obtain the rendered image
         image = self.render.last_image
         output_path, _ = QtWidgets.QFileDialog.getSaveFileName(self, "Save File", "", "Mask Files (*.png)")
         if output_path:
             rendered_image = PIL.Image.fromarray(image)
             rendered_image.save(output_path)
-            self.output_text.clear()
-            self.output_text.append(f"Export mask render to:\n {str(output_path)}")
+            self.output_text.append(f"-> Export mask render to:\n {str(output_path)}")
 
     def export_mesh_plot(self, reply_reset_camera=None, reply_render_mesh=None, reply_export_surface=None, save_render=True):
 
         if self.reference is None:
             QtWidgets.QMessageBox.warning(self, 'vision6D', "Need to set a reference or load a mesh first", QtWidgets.QMessageBox.Ok, QtWidgets.QMessageBox.Ok)
             return 0
 
@@ -655,16 +672,15 @@
         image = self.render.last_image
 
         if save_render:
             output_path, _ = QtWidgets.QFileDialog.getSaveFileName(self, "Save File", "", "Mesh Files (*.png)")
             if output_path:
                 rendered_image = PIL.Image.fromarray(image)
                 rendered_image.save(output_path)
-                self.output_text.clear()
-                self.output_text.append(f"Export reference mesh render to:\n {str(output_path)}")
+                self.output_text.append(f"-> Export reference mesh render to:\n {str(output_path)}")
 
         return image
 
     def export_segmesh_plot(self):
 
         if self.reference is None:
             QtWidgets.QMessageBox.warning(self, 'vision6D', "Need to set a reference or load a mesh first", QtWidgets.QMessageBox.Ok, QtWidgets.QMessageBox.Ok)
@@ -712,29 +728,31 @@
         # obtain the rendered image
         image = self.render.last_image
         image = (image * segmask).astype(np.uint8)
         output_path, _ = QtWidgets.QFileDialog.getSaveFileName(self, "Save File", "", "SegMesh Files (*.png)")
         if output_path:
             rendered_image = PIL.Image.fromarray(image)
             rendered_image.save(output_path)
-            self.output_text.clear()
-            self.output_text.append(f"Export segmask render:\n to {str(output_path)}")
-            
-        # return image
-
+            self.output_text.append(f"-> Export segmask render:\n to {str(output_path)}")
+        
     def export_pose(self):
         if self.reference is None: 
             QtWidgets.QMessageBox.warning(self, 'vision6D', "Need to set a reference or load a mesh first", QtWidgets.QMessageBox.Ok, QtWidgets.QMessageBox.Ok)
             return 0
         self.update_gt_pose()
         output_path, _ = QtWidgets.QFileDialog.getSaveFileName(self, "Save File", "", "Pose Files (*.npy)")
         if output_path:
             np.save(output_path, self.transformation_matrix)
-            self.output_text.clear()
-            self.output_text.append(f"\nSaved:\n{self.transformation_matrix}\nExport to:\n {str(output_path)}")
+            self.output_text.append(f"-> Saved:\n{self.transformation_matrix}\nExport to:\n {str(output_path)}")
+
+    def copy_output_text(self):
+        self.clipboard.setText(self.output_text.toPlainText())
+        
+    def clear_output_text(self):
+        self.output_text.clear()
 
     # ^Panel
     def set_panel_bar(self):
         # Create a left panel layout
         self.panel_widget = QtWidgets.QWidget()
         self.panel_layout = QtWidgets.QVBoxLayout(self.panel_widget)
 
@@ -812,45 +830,45 @@
         else: self.remove_actor(checked_button)
 
     def opacity_value_change(self, value):
         if self.ignore_slider_value_change: return 0
         checked_button = self.button_group_actors_names.checkedButton()
         if checked_button is not None:
             actor_name = checked_button.text()
-            if actor_name == 'image': self.set_image_opacity(value / 100)
-            elif actor_name == 'mask': self.set_mask_opacity(value / 100)
+            if actor_name == 'image': 
+                self.store_image_opacity = copy.deepcopy(self.image_opacity)
+                self.set_image_opacity(value / 100)
+            elif actor_name == 'mask': 
+                self.store_mask_opacity = copy.deepcopy(self.mask_opacity)
+                self.set_mask_opacity(value / 100)
             else: 
+                self.store_mesh_opacity[actor_name] = copy.deepcopy(self.mesh_opacity[actor_name])
                 self.mesh_opacity[actor_name] = value / 100
                 self.set_mesh_opacity(actor_name, self.mesh_opacity[actor_name])
-            self.output_text.clear()
-            self.output_text.append(f"Current actor <span style='background-color:yellow; color:black;'>{actor_name}</span>'s opacity is {value / 100}")
         else:
             self.ignore_slider_value_change = True
             self.opacity_slider.setValue(value)
             self.ignore_slider_value_change = False
             return 0
         
     def toggle_hide_actors_button(self):
         self.toggle_hide_actors_flag = not self.toggle_hide_actors_flag
         
         if self.toggle_hide_actors_flag:
             for button in self.button_group_actors_names.buttons():
                 button.setChecked(True)
                 actor_name = button.text()
-                if actor_name == 'image': self.store_image_opacity = copy.deepcopy(self.image_opacity)
-                elif actor_name == 'mask': self.store_mask_opacity = copy.deepcopy(self.mask_opacity)
-                else: self.store_mesh_opacity[actor_name] = copy.deepcopy(self.mesh_opacity[actor_name])
                 self.opacity_value_change(0)
-
-            self.ignore_slider_value_change = True
-            self.opacity_slider.setValue(0)
-            self.ignore_slider_value_change = False
-                
+    
             checked_button = self.button_group_actors_names.checkedButton()
-            if checked_button is None: QtWidgets.QMessageBox.warning(self, 'vision6D', "Need to select an actor first", QtWidgets.QMessageBox.Ok, QtWidgets.QMessageBox.Ok)
+            if checked_button is not None: 
+                self.ignore_slider_value_change = True
+                self.opacity_slider.setValue(0)
+                self.ignore_slider_value_change = False
+            else: QtWidgets.QMessageBox.warning(self, 'vision6D', "Need to select an actor first", QtWidgets.QMessageBox.Ok, QtWidgets.QMessageBox.Ok)
         
         else:
             for button in self.button_group_actors_names.buttons():
                 button.setChecked(True)
                 actor_name = button.text()
                 if actor_name == 'image': self.opacity_value_change(self.store_image_opacity * 100)
                 elif actor_name == 'mask': self.opacity_value_change(self.store_mask_opacity * 100)
@@ -860,56 +878,71 @@
             if checked_button is not None:
                 actor_name = checked_button.text()
                 self.ignore_slider_value_change = True
                 if actor_name == 'image': self.opacity_slider.setValue(self.image_opacity * 100)
                 elif actor_name == 'mask': self.opacity_slider.setValue(self.mask_opacity * 100)
                 else: self.opacity_slider.setValue(self.mesh_opacity[actor_name] * 100)
                 self.ignore_slider_value_change = False
-            else:
-                QtWidgets.QMessageBox.warning(self, 'vision6D', "Need to select an actor first", QtWidgets.QMessageBox.Ok, QtWidgets.QMessageBox.Ok)
+            else: QtWidgets.QMessageBox.warning(self, 'vision6D', "Need to select an actor first", QtWidgets.QMessageBox.Ok, QtWidgets.QMessageBox.Ok)
 
     def panel_display(self):
         self.display = QtWidgets.QGroupBox("Console")
         display_layout = QtWidgets.QVBoxLayout()
         display_layout.setContentsMargins(10, 20, 10, 10)
 
         #* Create the top widgets (layout)
         top_layout = QtWidgets.QHBoxLayout()
-        top_layout.setContentsMargins(0, 10, 0, 10)
+        top_layout.setContentsMargins(0, 0, 0, 0)
+
+        # Create Grid layout for function buttons
+        grid_layout = QtWidgets.QGridLayout()
+
+        # Create the set camera button
+        set_camera_button = QtWidgets.QPushButton("Set Camera")
+        set_camera_button.clicked.connect(self.set_camera)
+        grid_layout.addWidget(set_camera_button, 0, 0)
+
+        # Create the actor pose button
+        actor_pose_button = QtWidgets.QPushButton("Set Pose")
+        actor_pose_button.clicked.connect(self.set_pose)
+        grid_layout.addWidget(actor_pose_button, 0, 1)
+
+        # Create the hide button
+        hide_button = QtWidgets.QPushButton("toggle hide")
+        hide_button.clicked.connect(self.toggle_hide_actors_button)
+        grid_layout.addWidget(hide_button, 0, 2)
+
+        # Create the remove button
+        remove_button = QtWidgets.QPushButton("Remove Actor")
+        remove_button.clicked.connect(self.remove_actors_button)
+        grid_layout.addWidget(remove_button, 0, 3)
 
         # Create the color dropdown menu (comboBox)
         self.color_button = QtWidgets.QPushButton("Color")
         self.color_button.clicked.connect(self.show_color_popup)
-        top_layout.addWidget(self.color_button, 1) # 1 is for the stretch factor
-
-        # Create the color dropdown menu (comboBox)
+        grid_layout.addWidget(self.color_button, 1, 0)
+        
+        # Create the spacing button (comboBox)
         self.spacing_button = QtWidgets.QPushButton("Spacing")
         self.spacing_button.clicked.connect(self.set_spacing)
-        top_layout.addWidget(self.spacing_button, 1) # 1 is for the stretch factor
+        grid_layout.addWidget(self.spacing_button, 1, 1)
 
-        # Create the opacity slider
         self.opacity_slider = QtWidgets.QSlider(Qt.Horizontal)
         self.opacity_slider.setMinimum(0)
         self.opacity_slider.setMaximum(100)
         self.opacity_slider.setValue(100)
         self.opacity_slider.setTickPosition(QtWidgets.QSlider.TicksBelow)
         self.opacity_slider.setSingleStep(1)
         self.ignore_slider_value_change = False 
         self.opacity_slider.valueChanged.connect(self.opacity_value_change)
-        top_layout.addWidget(self.opacity_slider, 1.5)
+        grid_layout.addWidget(self.opacity_slider, 1, 2, 1, 2)
 
-        # Create the hide button
-        hide_button = QtWidgets.QPushButton("toggle hide")
-        hide_button.clicked.connect(self.toggle_hide_actors_button)
-        top_layout.addWidget(hide_button, 1)
-
-        # Create the remove button
-        remove_button = QtWidgets.QPushButton("Remove")
-        remove_button.clicked.connect(self.remove_actors_button)
-        top_layout.addWidget(remove_button, 1)
+        grid_widget = QtWidgets.QWidget()
+        grid_widget.setLayout(grid_layout)
+        top_layout.addWidget(grid_widget)
 
         display_layout.addLayout(top_layout)
 
         #* Create the bottom widgets
         actor_widget = QtWidgets.QLabel("Actors")
         display_layout.addWidget(actor_widget)
 
@@ -934,16 +967,40 @@
 
     def panel_output(self):
         # Add a spacer to the top of the main layout
         self.output = QtWidgets.QGroupBox("Output")
         output_layout = QtWidgets.QVBoxLayout()
         output_layout.setContentsMargins(10, 20, 10, 10)
 
+        #* Create the top widgets (layout)
+        top_layout = QtWidgets.QHBoxLayout()
+        top_layout.setContentsMargins(0, 0, 0, 0)
+
+        # Create Grid layout for function buttons
+        grid_layout = QtWidgets.QGridLayout()
+
+        # Create the set camera button
+        copy_text_button = QtWidgets.QPushButton("Copy")
+        copy_text_button.clicked.connect(self.copy_output_text)
+        grid_layout.addWidget(copy_text_button, 0, 2, 1, 1)
+
+        # Create the actor pose button
+        clear_text_button = QtWidgets.QPushButton("Clear")
+        clear_text_button.clicked.connect(self.clear_output_text)
+        grid_layout.addWidget(clear_text_button, 0, 3, 1, 1)
+
+        grid_widget = QtWidgets.QWidget()
+        grid_widget.setLayout(grid_layout)
+        top_layout.addWidget(grid_widget)
+        output_layout.addLayout(top_layout)
+
         self.output_text = QtWidgets.QTextEdit()
-        self.output_text.setReadOnly(True)
+        self.output_text.setReadOnly(False)
+        # Access to the system clipboard
+        self.clipboard = QtGui.QGuiApplication.clipboard()
         output_layout.addWidget(self.output_text)
         self.output.setLayout(output_layout)
         self.panel_layout.addWidget(self.output)
 
     #^ Show plot
     def create_plotter(self):
         self.frame = QtWidgets.QFrame()
@@ -975,8 +1032,8 @@
         self.plotter.add_camera_orientation_widget()
 
         self.plotter.show()
         self.show()
 
     def showMaximized(self):
         super(MyMainWindow, self).showMaximized()
-        self.splitter.setSizes([int(self.width() * 0.2), int(self.width() * 0.8)])
+        self.splitter.setSizes([int(self.width() * 0.05), int(self.width() * 0.95)])
```

### Comparing `vision6D-0.1.0/vision6D/__init__.py` & `vision6D-0.1.1/vision6D/__init__.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.1.0/vision6D/app.py` & `vision6D-0.1.1/vision6D/app.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.1.0/vision6D/config.py` & `vision6D-0.1.1/vision6D/config.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.1.0/vision6D/data/ossiclesCoordinateMapping.json` & `vision6D-0.1.1/vision6D/data/ossiclesCoordinateMapping.json`

 * *Files identical despite different names*

### Comparing `vision6D-0.1.0/vision6D/data/ossiclesCoordinateMappingv1.json` & `vision6D-0.1.1/vision6D/data/ossiclesCoordinateMappingv1.json`

 * *Files identical despite different names*

### Comparing `vision6D-0.1.0/vision6D/data/style.qss` & `vision6D-0.1.1/vision6D/data/style.qss`

 * *Files identical despite different names*

### Comparing `vision6D-0.1.0/vision6D/interface.py` & `vision6D-0.1.1/vision6D/interface.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.1.0/vision6D/interface_gui.py` & `vision6D-0.1.1/vision6D/interface_gui.py`

 * *Files 4% similar despite different names*

```diff
@@ -58,25 +58,24 @@
         if text in self.mesh_actors:
             # set the current mesh color
             self.color_button.setText(self.mesh_colors[text])
             # set mesh reference
             self.reference = text
             curr_opacity = self.mesh_actors[self.reference].GetProperty().opacity
             self.opacity_slider.setValue(curr_opacity * 100)
-            self.output_text.clear()
-            self.output_text.append(f"Current reference mesh actor is <span style='background-color:yellow; color:black;'>{self.reference}</span>, and opacity is {curr_opacity}")
         else:
             self.color_button.setText("Color")
             if text == 'image': curr_opacity = self.image_opacity
             elif text == 'mask': curr_opacity = self.mask_opacity
             self.opacity_slider.setValue(curr_opacity * 100)
-            self.output_text.clear()
-            self.output_text.append(f"Current selected actor is <span style='background-color:yellow; color:black;'>{text}</span>, and opacity is {curr_opacity}")
             self.reference = None
-                                                                
+        
+        output = f"-> Actor {text}, and its opacity is {curr_opacity}"
+        if output not in self.output_text.toPlainText(): self.output_text.append(output)
+                                            
     def set_image_opacity(self, image_opacity: float):
         assert image_opacity>=0 and image_opacity<=1, "image opacity should range from 0 to 1!"
         self.image_opacity = image_opacity
         self.image_actor.GetProperty().opacity = image_opacity
         self.plotter.add_actor(self.image_actor, pickable=False, name='image')
 
     def set_mask_opacity(self, mask_opacity: float):
@@ -264,35 +263,34 @@
                 if actor_name not in self.undo_poses: self.undo_poses[actor_name] = []
                 self.undo_poses[actor_name].append(self.mesh_actors[actor_name].user_matrix)
                 if len(self.undo_poses[actor_name]) > 20: self.undo_poses[actor_name].pop(0)
                 # check the picked button
                 self.check_button(actor_name)
 
     def reset_gt_pose(self, *args):
-        self.output_text.clear(); self.output_text.append(f"\nReset the GT pose to: \n{self.initial_pose}\n")
+        self.output_text.append(f"-> Reset the GT pose to: \n{self.initial_pose}")
         for actor_name, actor in self.mesh_actors.items():
             actor.user_matrix = self.initial_pose
             self.plotter.add_actor(actor, pickable=True, name=actor_name)
 
     def update_gt_pose(self, *args):
         if self.reference is not None:
-            self.output_text.clear(); self.output_text.append(f"Current reference mesh is: <span style='background-color:yellow; color:black;'>{self.reference}</span>")
             self.transformation_matrix = self.mesh_actors[self.reference].user_matrix
             self.initial_pose = self.transformation_matrix
-            self.output_text.append(f"\nUpdate the GT pose to: \n{self.initial_pose}\n")
+            self.output_text.append(f"-> Current reference mesh is: <span style='background-color:yellow; color:black;'>{self.reference}</span>")
+            self.output_text.append(f"Update the GT pose to: \n{self.initial_pose}")
             for actor_name, actor in self.mesh_actors.items():
                 actor.user_matrix = self.initial_pose
                 self.plotter.add_actor(actor, pickable=True, name=actor_name)
 
     def current_pose(self, *args):
         if self.reference is not None:
             transformation_matrix = self.mesh_actors[self.reference].user_matrix
-            self.output_text.clear(); 
-            self.output_text.append(f"Current reference mesh is: <span style='background-color:yellow; color:black;'>{self.reference}</span>")
-            self.output_text.append(f"\nCurrent pose is: \n{transformation_matrix}\n")
+            self.output_text.append(f"-> Current reference mesh is: <span style='background-color:yellow; color:black;'>{self.reference}</span>")
+            self.output_text.append(f"Current pose is: \n{transformation_matrix}")
             for actor_name, actor in self.mesh_actors.items():
                 actor.user_matrix = transformation_matrix
                 self.plotter.add_actor(actor, pickable=True, name=actor_name)
 
     def undo_pose(self, *args):
         if self.button_group_actors_names.checkedButton() is not None:
             actor_name = self.button_group_actors_names.checkedButton().text()
@@ -301,17 +299,16 @@
             return 0
         if len(self.undo_poses[actor_name]) != 0: 
             transformation_matrix = self.undo_poses[actor_name].pop()
             if (transformation_matrix == self.mesh_actors[actor_name].user_matrix).all():
                 if len(self.undo_poses[actor_name]) != 0: 
                     transformation_matrix = self.undo_poses[actor_name].pop()
 
-            self.output_text.clear(); 
-            self.output_text.append(f"Current reference mesh is: <span style='background-color:yellow; color:black;'>{actor_name}</span>")
-            self.output_text.append(f"\nUndo pose to: \n{transformation_matrix}\n")
+            self.output_text.append(f"-> Current reference mesh is: <span style='background-color:yellow; color:black;'>{actor_name}</span>")
+            self.output_text.append(f"Undo pose to: \n{transformation_matrix}")
                 
             self.mesh_actors[actor_name].user_matrix = transformation_matrix
             self.plotter.add_actor(self.mesh_actors[actor_name], pickable=True, name=actor_name)
 
     def set_scalar(self, nocs, actor_name):
         vertices, faces = vis.utils.get_mesh_actor_vertices_faces(self.mesh_actors[actor_name])
         vertices_color = vertices
@@ -403,17 +400,16 @@
             if self.mesh_colors[self.reference] == 'nocs':
                 vertices, faces = vis.utils.get_mesh_actor_vertices_faces(self.mesh_actors[self.reference])
                 mesh = trimesh.Trimesh(vertices, faces, process=False)
                 predicted_pose = self.nocs_epnp(color_mask, mesh)
                 if self.mirror_x: predicted_pose = np.array([[-1, 0, 0, 0], [0, 1, 0, 0], [0, 0, 1, 0], [0, 0, 0, 1]]) @ predicted_pose @ np.array([[-1, 0, 0, 0], [0, 1, 0, 0], [0, 0, 1, 0], [0, 0, 0, 1]])
                 if self.mirror_y: predicted_pose = np.array([[1, 0, 0, 0], [0, -1, 0, 0], [0, 0, 1, 0], [0, 0, 0, 1]]) @ predicted_pose @ np.array([[1, 0, 0, 0], [0, -1, 0, 0], [0, 0, 1, 0], [0, 0, 0, 1]])
                 error = np.sum(np.abs(predicted_pose - gt_pose))
-                self.output_text.clear()
-                self.output_text.append(f"PREDICTED POSE WITH <span style='background-color:yellow; color:black;'>NOCS COLOR</span>: ")
-                self.output_text.append(f"\n{predicted_pose}\n\nGT POSE: \n\n{gt_pose}\n\nERROR: \n\n{error}")
+                self.output_text.append(f"-> PREDICTED POSE WITH <span style='background-color:yellow; color:black;'>NOCS COLOR</span>: ")
+                self.output_text.append(f"{predicted_pose}\nGT POSE: \n{gt_pose}\nERROR: \n{error}")
 
             else:
                 QtWidgets.QMessageBox.warning(self, 'vision6D', "Only works using EPnP with latlon mask", QtWidgets.QMessageBox.Ok, QtWidgets.QMessageBox.Ok)
 
         else:
             QtWidgets.QMessageBox.warning(self, 'vision6D', "A mesh need to be loaded/mesh reference need to be set", QtWidgets.QMessageBox.Ok, QtWidgets.QMessageBox.Ok)
             return 0
@@ -446,43 +442,29 @@
                 color_mask = mask_data
                 if np.sum(color_mask) != 0:
                     unique, counts = np.unique(color_mask, return_counts=True)
                     digit_counts = dict(zip(unique, counts))
                     if digit_counts[0] == np.max(counts): 
                         nocs_color = False if np.sum(color_mask[..., 2]) == 0 else True
 
-                        # get the gt pose
-                        res = self.get_text_dialog.exec_()
-
-                        if res == QtWidgets.QDialog.Accepted:
-                            try:
-                                gt_pose = ast.literal_eval(self.get_text_dialog.user_text)
-                                gt_pose = np.array(gt_pose)
-                                if gt_pose.shape != (4, 4): 
-                                    QtWidgets.QMessageBox.warning(self, 'vision6D', "It needs to be a 4 by 4 matrix", QtWidgets.QMessageBox.Ok, QtWidgets.QMessageBox.Ok) 
-                                    return 0
-                            except: 
-                                QtWidgets.QMessageBox.warning(self, 'vision6D', "Format is not correct", QtWidgets.QMessageBox.Ok, QtWidgets.QMessageBox.Ok)
-                                return 0
-                        else: 
-                            return 0
-
-                        self.output_text.clear()
-                        self.output_text.append(f"The input ground truth pose is:\n[{gt_pose[0]}, \n{gt_pose[1]}, \n{gt_pose[2]}, \n{gt_pose[3]}]")
-                        QtWidgets.QMessageBox.information(self, "Information", "Please load the corresponding mesh")
-
+                        # Set the pose information if the format is correct
+                        res = self.set_pose()
+                        if res is None: return 0
+                        
+                        gt_pose = self.transformation_matrix
+                                                
                         # add the mesh object file
-                        self.transformation_matrix = gt_pose
+                        QtWidgets.QMessageBox.information(self, "Information", "Please load the corresponding mesh")
+                        
                         self.add_mesh_file(prompt=True)
                         if self.mesh_path != '':
                             checked_button = self.button_group_actors_names.checkedButton()
                             vertices, faces = vis.utils.get_mesh_actor_vertices_faces(self.mesh_actors[checked_button.text()])
                             mesh = trimesh.Trimesh(vertices, faces, process=False)
-                        else:
-                            return 0
+                        else: return 0
                     else:
                         QtWidgets.QMessageBox.warning(self, 'vision6D', "A color mask need to be loaded", QtWidgets.QMessageBox.Ok, QtWidgets.QMessageBox.Ok)
                         return 0
         
             if np.sum(color_mask) == 0:
                 QtWidgets.QMessageBox.warning(self, 'vision6D', "The color mask is blank (maybe set the reference mesh wrong)", QtWidgets.QMessageBox.Ok, QtWidgets.QMessageBox.Ok)
                 return 0
@@ -495,14 +477,13 @@
                     color_theme = 'NOCS'
                 else: 
                     if self.mirror_x: color_mask = color_mask[:, ::-1, :]
                     if self.mirror_y: color_mask = color_mask[::-1, :, :]
                     predicted_pose = self.latlon_epnp(color_mask, mesh)
                     color_theme = 'LATLON'
                 error = np.sum(np.abs(predicted_pose - gt_pose))
-                self.output_text.clear()
-                self.output_text.append(f"PREDICTED POSE WITH <span style='background-color:yellow; color:black;'>{color_theme} COLOR (MASKED)</span>: ")
-                self.output_text.append(f"\n{predicted_pose}\n\nGT POSE: \n\n{gt_pose}\n\nERROR: \n\n{error}")
+                self.output_text.append(f"-> PREDICTED POSE WITH <span style='background-color:yellow; color:black;'>{color_theme} COLOR (MASKED)</span>: ")
+                self.output_text.append(f"{predicted_pose}\nGT POSE: \n{gt_pose}\nERROR: \n{error}")
             else:
                 QtWidgets.QMessageBox.warning(self,"vision6D", "Clicked the wrong method")
         else:
             QtWidgets.QMessageBox.warning(self,"vision6D", "please load a mask first")
```

### Comparing `vision6D-0.1.0/vision6D/mainwindow.py` & `vision6D-0.1.1/vision6D/mainwindow.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.1.0/vision6D/run_gui.py` & `vision6D-0.1.1/vision6D/run_gui.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.1.0/vision6D/utils.py` & `vision6D-0.1.1/vision6D/utils.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.1.0/vision6D.egg-info/PKG-INFO` & `vision6D-0.1.1/vision6D.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vision6D
-Version: 0.1.0
+Version: 0.1.1
 Summary: vision6D: A tool for 6D pose estimation annotation
 Home-page: https://github.com/ykzzky/vision6D
 License: GNU GENERAL Public License
 Project-URL: Bug Tracker, https://github.com/ykzzky/vision6D/issues
 Keywords: multimodal,data,analysis,real-time,distributed
 Platform: any
 Classifier: Programming Language :: Python :: 3
```

### Comparing `vision6D-0.1.0/vision6D.egg-info/SOURCES.txt` & `vision6D-0.1.1/vision6D.egg-info/SOURCES.txt`

 * *Files identical despite different names*

