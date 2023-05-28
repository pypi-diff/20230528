# Comparing `tmp/qclib-0.0.8.tar.gz` & `tmp/qclib-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qclib-0.0.8.tar", last modified: Wed Nov 10 17:54:15 2021, max compression
+gzip compressed data, was "qclib-0.0.9.tar", last modified: Sat Jan 22 13:04:07 2022, max compression
```

## Comparing `qclib-0.0.8.tar` & `qclib-0.0.9.tar`

### file list

```diff
@@ -1,48 +1,59 @@
-drwxrwxrwx   0        0        0        0 2021-11-10 17:54:15.443576 qclib-0.0.8/
--rw-rw-rw-   0        0        0    11558 2021-11-10 17:14:10.000000 qclib-0.0.8/LICENSE.md
--rw-rw-rw-   0        0        0      596 2021-11-10 17:54:15.444576 qclib-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      159 2021-11-10 17:14:10.000000 qclib-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2021-11-10 17:54:15.386582 qclib-0.0.8/qclib/
--rw-rw-rw-   0        0        0      144 2021-11-10 17:14:10.000000 qclib-0.0.8/qclib/__init__.py
--rw-rw-rw-   0        0        0    11666 2021-11-10 17:14:10.000000 qclib-0.0.8/qclib/isometry.py
-drwxrwxrwx   0        0        0        0 2021-11-10 17:54:15.421579 qclib-0.0.8/qclib/state_preparation/
--rw-rw-rw-   0        0        0        0 2021-11-10 17:14:10.000000 qclib-0.0.8/qclib/state_preparation/__init__.py
--rw-rw-rw-   0        0        0     3978 2021-11-10 17:14:10.000000 qclib-0.0.8/qclib/state_preparation/apqm.py
--rw-rw-rw-   0        0        0     1633 2021-11-10 17:14:10.000000 qclib-0.0.8/qclib/state_preparation/bdsp.py
--rw-rw-rw-   0        0        0     4780 2021-11-10 17:14:10.000000 qclib-0.0.8/qclib/state_preparation/cvoqram.py
--rw-rw-rw-   0        0        0     8460 2021-11-10 17:14:10.000000 qclib-0.0.8/qclib/state_preparation/dcsp.py
--rw-rw-rw-   0        0        0     1733 2021-11-10 17:14:10.000000 qclib-0.0.8/qclib/state_preparation/mottonen.py
--rw-rw-rw-   0        0        0     7989 2021-11-10 17:14:10.000000 qclib-0.0.8/qclib/state_preparation/pivot.py
--rw-rw-rw-   0        0        0     7365 2021-11-10 17:14:10.000000 qclib-0.0.8/qclib/state_preparation/schmidt.py
-drwxrwxrwx   0        0        0        0 2021-11-10 17:54:15.428579 qclib-0.0.8/qclib/state_preparation/util/
--rw-rw-rw-   0        0        0        0 2021-11-10 17:14:10.000000 qclib-0.0.8/qclib/state_preparation/util/__init__.py
--rw-rw-rw-   0        0        0     2005 2021-11-10 17:14:10.000000 qclib-0.0.8/qclib/state_preparation/util/angle_tree_preparation.py
--rw-rw-rw-   0        0        0     2470 2021-11-10 17:14:10.000000 qclib-0.0.8/qclib/state_preparation/util/state_tree_preparation.py
--rw-rw-rw-   0        0        0     2598 2021-11-10 17:14:10.000000 qclib-0.0.8/qclib/state_preparation/util/tree_register.py
--rw-rw-rw-   0        0        0     5558 2021-11-10 17:14:10.000000 qclib-0.0.8/qclib/state_preparation/util/tree_utils.py
--rw-rw-rw-   0        0        0     2994 2021-11-10 17:14:10.000000 qclib-0.0.8/qclib/state_preparation/util/tree_walk.py
--rw-rw-rw-   0        0        0     4908 2021-11-10 17:14:10.000000 qclib-0.0.8/qclib/state_preparation/ventura.py
--rw-rw-rw-   0        0        0     3833 2021-11-10 17:14:10.000000 qclib-0.0.8/qclib/unitary.py
--rw-rw-rw-   0        0        0     6337 2021-11-10 17:14:10.000000 qclib-0.0.8/qclib/util.py
-drwxrwxrwx   0        0        0        0 2021-11-10 17:54:15.410588 qclib-0.0.8/qclib.egg-info/
--rw-rw-rw-   0        0        0      596 2021-11-10 17:54:15.000000 qclib-0.0.8/qclib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1094 2021-11-10 17:54:15.000000 qclib-0.0.8/qclib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-11-10 17:54:15.000000 qclib-0.0.8/qclib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2021-11-10 17:54:15.000000 qclib-0.0.8/qclib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2021-11-10 17:54:15.000000 qclib-0.0.8/qclib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2021-11-10 17:54:15.449576 qclib-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      769 2021-11-10 17:53:53.000000 qclib-0.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2021-11-10 17:54:15.442577 qclib-0.0.8/test/
--rw-rw-rw-   0        0        0        0 2021-11-10 17:14:10.000000 qclib-0.0.8/test/__init__.py
--rw-rw-rw-   0        0        0     2336 2021-11-10 17:14:10.000000 qclib-0.0.8/test/test_bdsp.py
--rw-rw-rw-   0        0        0     1725 2021-11-10 17:14:10.000000 qclib-0.0.8/test/test_dcsp.py
--rw-rw-rw-   0        0        0     4318 2021-11-10 17:14:10.000000 qclib-0.0.8/test/test_isometry.py
--rw-rw-rw-   0        0        0     2873 2021-11-10 17:14:10.000000 qclib-0.0.8/test/test_majority.py
--rw-rw-rw-   0        0        0     4303 2021-11-10 17:14:10.000000 qclib-0.0.8/test/test_mc_gate.py
--rw-rw-rw-   0        0        0     2982 2021-11-10 17:14:10.000000 qclib-0.0.8/test/test_mottonen.py
--rw-rw-rw-   0        0        0     2707 2021-11-10 17:14:10.000000 qclib-0.0.8/test/test_pqm.py
--rw-rw-rw-   0        0        0     3756 2021-11-10 17:14:10.000000 qclib-0.0.8/test/test_schmidt.py
--rw-rw-rw-   0        0        0     4709 2021-11-10 17:14:10.000000 qclib-0.0.8/test/test_sparse_sp.py
--rw-rw-rw-   0        0        0     3338 2021-11-10 17:14:10.000000 qclib-0.0.8/test/test_unitary.py
--rw-rw-rw-   0        0        0     1997 2021-11-10 17:14:10.000000 qclib-0.0.8/test/test_ventura.py
--rw-rw-rw-   0        0        0      664 2021-11-10 17:14:10.000000 qclib-0.0.8/test/util.py
+drwxrwxrwx   0        0        0        0 2022-01-22 13:04:07.418770 qclib-0.0.9/
+-rw-rw-rw-   0        0        0    11558 2021-12-17 11:11:30.000000 qclib-0.0.9/LICENSE.md
+-rw-rw-rw-   0        0        0      596 2022-01-22 13:04:07.418770 qclib-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      159 2021-12-17 11:11:30.000000 qclib-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2022-01-22 13:04:07.354770 qclib-0.0.9/qclib/
+-rw-rw-rw-   0        0        0      144 2021-12-17 11:11:30.000000 qclib-0.0.9/qclib/__init__.py
+-rw-rw-rw-   0        0        0     5198 2022-01-20 13:11:43.000000 qclib-0.0.9/qclib/entanglement.py
+drwxrwxrwx   0        0        0        0 2022-01-22 13:04:07.378770 qclib-0.0.9/qclib/gates/
+-rw-rw-rw-   0        0        0        0 2022-01-22 12:53:28.000000 qclib-0.0.9/qclib/gates/__init__.py
+-rw-rw-rw-   0        0        0     1234 2022-01-22 12:53:28.000000 qclib-0.0.9/qclib/gates/majority.py
+-rw-rw-rw-   0        0        0     5490 2022-01-22 12:53:28.000000 qclib-0.0.9/qclib/gates/mc_gate.py
+-rw-rw-rw-   0        0        0    14982 2022-01-22 12:53:28.000000 qclib-0.0.9/qclib/isometry.py
+drwxrwxrwx   0        0        0        0 2022-01-22 13:04:07.391770 qclib-0.0.9/qclib/state_preparation/
+-rw-rw-rw-   0        0        0        0 2021-12-17 11:11:30.000000 qclib-0.0.9/qclib/state_preparation/__init__.py
+-rw-rw-rw-   0        0        0     3978 2021-12-17 11:11:30.000000 qclib-0.0.9/qclib/state_preparation/apqm.py
+-rw-rw-rw-   0        0        0     4353 2022-01-20 13:11:43.000000 qclib-0.0.9/qclib/state_preparation/baa_schmidt.py
+-rw-rw-rw-   0        0        0     1633 2021-12-17 11:11:30.000000 qclib-0.0.9/qclib/state_preparation/bdsp.py
+-rw-rw-rw-   0        0        0     4780 2022-01-22 12:53:28.000000 qclib-0.0.9/qclib/state_preparation/cvoqram.py
+-rw-rw-rw-   0        0        0     8460 2021-12-17 11:11:30.000000 qclib-0.0.9/qclib/state_preparation/dcsp.py
+-rw-rw-rw-   0        0        0    17174 2022-01-22 12:53:28.000000 qclib-0.0.9/qclib/state_preparation/gleining.py
+-rw-rw-rw-   0        0        0     1733 2021-12-17 11:11:30.000000 qclib-0.0.9/qclib/state_preparation/mottonen.py
+-rw-rw-rw-   0        0        0     7989 2022-01-22 12:53:28.000000 qclib-0.0.9/qclib/state_preparation/pivot.py
+-rw-rw-rw-   0        0        0    13121 2022-01-22 12:53:28.000000 qclib-0.0.9/qclib/state_preparation/schmidt.py
+drwxrwxrwx   0        0        0        0 2022-01-22 13:04:07.400770 qclib-0.0.9/qclib/state_preparation/util/
+-rw-rw-rw-   0        0        0        0 2021-12-17 11:11:30.000000 qclib-0.0.9/qclib/state_preparation/util/__init__.py
+-rw-rw-rw-   0        0        0     2122 2021-12-17 11:11:30.000000 qclib-0.0.9/qclib/state_preparation/util/angle_tree_preparation.py
+-rw-rw-rw-   0        0        0    17581 2022-01-22 12:51:43.000000 qclib-0.0.9/qclib/state_preparation/util/baa.py
+-rw-rw-rw-   0        0        0     2470 2021-12-17 11:11:30.000000 qclib-0.0.9/qclib/state_preparation/util/state_tree_preparation.py
+-rw-rw-rw-   0        0        0     2598 2021-12-17 11:11:30.000000 qclib-0.0.9/qclib/state_preparation/util/tree_register.py
+-rw-rw-rw-   0        0        0     5558 2021-12-17 11:11:30.000000 qclib-0.0.9/qclib/state_preparation/util/tree_utils.py
+-rw-rw-rw-   0        0        0     3008 2022-01-20 13:11:43.000000 qclib-0.0.9/qclib/state_preparation/util/tree_walk.py
+-rw-rw-rw-   0        0        0     4908 2021-12-17 11:11:30.000000 qclib-0.0.9/qclib/state_preparation/ventura.py
+-rw-rw-rw-   0        0        0     5614 2022-01-22 12:53:28.000000 qclib-0.0.9/qclib/unitary.py
+-rw-rw-rw-   0        0        0     6347 2022-01-20 13:11:43.000000 qclib-0.0.9/qclib/util.py
+drwxrwxrwx   0        0        0        0 2022-01-22 13:04:07.375770 qclib-0.0.9/qclib.egg-info/
+-rw-rw-rw-   0        0        0      596 2022-01-22 13:04:07.000000 qclib-0.0.9/qclib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1362 2022-01-22 13:04:07.000000 qclib-0.0.9/qclib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-01-22 13:04:07.000000 qclib-0.0.9/qclib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2022-01-22 13:04:07.000000 qclib-0.0.9/qclib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2022-01-22 13:04:07.000000 qclib-0.0.9/qclib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2022-01-22 13:04:07.419770 qclib-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      769 2022-01-22 13:03:49.000000 qclib-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2022-01-22 13:04:07.417770 qclib-0.0.9/test/
+-rw-rw-rw-   0        0        0        0 2021-12-17 11:11:30.000000 qclib-0.0.9/test/__init__.py
+-rw-rw-rw-   0        0        0    13829 2022-01-20 13:11:43.000000 qclib-0.0.9/test/test_baa.py
+-rw-rw-rw-   0        0        0     8540 2022-01-20 13:11:43.000000 qclib-0.0.9/test/test_baa_schmidt.py
+-rw-rw-rw-   0        0        0     2368 2021-12-17 11:11:30.000000 qclib-0.0.9/test/test_bdsp.py
+-rw-rw-rw-   0        0        0     1757 2021-12-17 11:11:30.000000 qclib-0.0.9/test/test_dcsp.py
+-rw-rw-rw-   0        0        0     2055 2022-01-20 13:11:43.000000 qclib-0.0.9/test/test_gleining.py
+-rw-rw-rw-   0        0        0     4318 2021-12-17 11:11:30.000000 qclib-0.0.9/test/test_isometry.py
+-rw-rw-rw-   0        0        0     2874 2022-01-22 12:54:05.000000 qclib-0.0.9/test/test_majority.py
+-rw-rw-rw-   0        0        0     4304 2022-01-22 12:54:05.000000 qclib-0.0.9/test/test_mc_gate.py
+-rw-rw-rw-   0        0        0     3014 2021-12-17 11:11:30.000000 qclib-0.0.9/test/test_mottonen.py
+-rw-rw-rw-   0        0        0     2707 2021-12-17 11:11:30.000000 qclib-0.0.9/test/test_pqm.py
+-rw-rw-rw-   0        0        0     5187 2022-01-20 13:11:43.000000 qclib-0.0.9/test/test_schmidt.py
+-rw-rw-rw-   0        0        0     4709 2021-12-17 11:11:30.000000 qclib-0.0.9/test/test_sparse_sp.py
+-rw-rw-rw-   0        0        0     3338 2022-01-22 12:53:28.000000 qclib-0.0.9/test/test_unitary.py
+-rw-rw-rw-   0        0        0     1997 2021-12-17 11:11:30.000000 qclib-0.0.9/test/test_ventura.py
+-rw-rw-rw-   0        0        0      664 2021-12-17 11:11:30.000000 qclib-0.0.9/test/util.py
```

### Comparing `qclib-0.0.8/LICENSE.md` & `qclib-0.0.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `qclib-0.0.8/PKG-INFO` & `qclib-0.0.9/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qclib
-Version: 0.0.8
+Version: 0.0.9
 Summary: A quantum computing library using qiskit
 Home-page: https://github.com/qclib/qclib
 Author: Adenilton Silva
 Author-email: ajsilva@cin.ufpe.br
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `qclib-0.0.8/qclib/isometry.py` & `qclib-0.0.9/qclib/isometry.py`

 * *Files 19% similar despite different names*

```diff
@@ -8,25 +8,24 @@
 
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-
 """
 Implements the decomposition of isometries using the methods
 defined at https://arxiv.org/abs/1501.06911.
 """
 
-
+from math import log2
 import numpy as np
 import scipy
 import qiskit.quantum_info as qi
-from qiskit import QuantumCircuit, QuantumRegister
+from qiskit import QuantumCircuit, QuantumRegister, transpile
 from qiskit.extensions.quantum_initializer.uc import UCGate
 
 # pylint: disable=maybe-no-member
 
 def decompose(isometry, scheme='ccd'):
     """
     Decompose an isometry from m to n qubits.
@@ -47,16 +46,16 @@
     iso = isometry.astype(complex)
     if len(iso.shape) == 1:
         iso = iso.reshape(iso.shape[0], 1) # change a row vector to a column
                                            # vector (in the case of state
                                            # preparation).
     lines = iso.shape[0]
     cols = iso.shape[1]
-    log_lines = np.log2(lines)
-    log_cols = np.log2(cols)
+    log_lines = log2(lines)
+    log_cols = log2(cols)
 
     _check_isometry(iso, log_lines, log_cols)
 
     log_lines = int(log_lines)
     log_cols = int(log_cols)
 
     if scheme == 'csd':
@@ -102,32 +101,15 @@
 
 def _knill(iso, log_lines, log_cols):
     if log_lines < 2:
         raise ValueError(
             "Knill decomposition does not work on a 1 qubit isometry (N=2)."
         )
 
-    if log_lines == log_cols:      # The isometry v is already unitary.
-        unitary = iso
-    else:                          # The isometry v is extended to a unitary maximizing
-                                   # the numbers of eigenvalues with complex argument equal
-                                   # to zero.
-        null_space = np.conj(scipy.linalg.null_space(iso.T)) # The complex conjugate of the null
-                                                             # space is the transformation that
-                                                             # generates the state |v> from |0>.
-                                                             # V=UI_{2^n,2^m} => U^-1 V=I_{2^n,2^m}
-                                                             # The transposition was removed
-                                                             # because it would be nullified in
-                                                             # U[:, M:] = W.T .
-        unitary = np.zeros((2**log_lines, 2**log_lines), dtype=complex)
-        unitary[:, :2**log_cols] = iso
-        unitary[:, 2**log_cols:] = null_space                # The transposition was removed
-                                                             # because it nullified the
-                                                             # transposition of the conjugate
-                                                             # complex above (which was removed).
+    unitary = _extend_to_unitary(iso, log_lines, log_cols)
 
     eigval, eigvec = np.linalg.eig(unitary)
     arg = np.angle(eigval)
 
     reg = QuantumRegister(log_lines)
     circuit = QuantumCircuit(reg)
 
@@ -140,18 +122,39 @@
 
             circuit.compose( schmidt(state).inverse(), reg, inplace=True )
 
             circuit.x(list(range(log_lines)))
             circuit.mcp(arg[i], list(range(log_lines-1)), log_lines-1)
             circuit.x(list(range(log_lines)))
 
-            circuit.compose( schmidt(state)          , reg, inplace=True )
+            circuit.compose( schmidt(state), reg, inplace=True )
 
     return circuit
 
+def _extend_to_unitary(iso, log_lines, log_cols):
+    if log_lines == log_cols:      # The isometry v is already unitary.
+        unitary = iso
+    else:                          # The isometry v is extended to a unitary maximizing
+                                   # the numbers of eigenvalues with complex argument equal
+                                   # to zero.
+        null_space = np.conj(scipy.linalg.null_space(iso.T)) # The complex conjugate of the null
+                                                             # space is the transformation that
+                                                             # generates the state |v> from |0>.
+                                                             # V=UI_{2^n,2^m} => U^-1 V=I_{2^n,2^m}
+                                                             # The transposition was removed
+                                                             # because it would be nullified in
+                                                             # U[:, M:] = W.T .
+        unitary = np.zeros((2**log_lines, 2**log_lines), dtype=complex)
+        unitary[:, :2**log_cols] = iso
+        unitary[:, 2**log_cols:] = null_space                # The transposition was removed
+                                                             # because it nullified the
+                                                             # transposition of the conjugate
+                                                             # complex above (which was removed).
+    return unitary
+
 
 
 #   Column-by-column
 
 
 
 def _ccd(iso, log_lines, log_cols):
@@ -273,16 +276,112 @@
         unitary = np.kron( iden[:,[basis]], psi_dagger ) + \
                     np.kron( iden[:,[-(basis+1)]], phi_dagger)
 
         return unitary
 
     return iden
 
-def _a(col_index, bit_index):
-    return col_index // 2**bit_index
-
-def _b(col_index, bit_index):
-    return col_index - (_a(col_index, bit_index) * 2**bit_index)
+def _a(col_index, bit_index):              # col_index >> bit_index.
+    return col_index // 2**bit_index       # Returns int representing n-bit_index most
+                                           # significant bits.
+def _b(col_index, bit_index):              # col_index ^ ((col_index >> bit_index) << bit_index)
+    return col_index - (_a(col_index, bit_index) * 2**bit_index) # Returns int representing
+                                                                 # bit_index less significant bits.
 
 def _k_s(col_index, bit_index):
     return int((col_index & 2**bit_index) / 2**bit_index) # Returns the bit value at bit_index
                                                           # of col_index (k in the paper).
+
+
+
+# CNOT count
+
+
+
+def cnot_count(isometry, scheme='ccd', method='estimate'):
+    """
+    Count the number of CNOTs to decompose the isometry.
+    """
+    if method == 'estimate':
+        return _cnot_count_estimate(isometry, scheme)
+
+    # Exact count
+    circuit = decompose(isometry, scheme)
+    transpiled_circuit = transpile(circuit, basis_gates=['u1','u2','u3','cx'],
+                                                            optimization_level=0)
+    count_ops = transpiled_circuit.count_ops()
+    if 'cx' in count_ops:
+        return count_ops['cx']
+
+    return 0
+
+def _cnot_count_estimate(isometry, scheme='ccd'):
+    """
+    Estimate the number of CNOTs to decompose the isometry.
+    """
+    iso = isometry.astype(complex)
+    if len(iso.shape) == 1:
+        iso = iso.reshape(iso.shape[0], 1)
+
+    log_lines = int(log2(iso.shape[0]))
+    log_cols = int(log2(iso.shape[1]))
+
+    if scheme == 'knill':
+        return _cnot_count_estimate_knill(isometry, log_lines, log_cols)
+
+    # CCD
+    return _cnot_count_estimate_ccd(log_lines, log_cols)
+
+def _cnot_count_estimate_knill(iso, log_lines, log_cols):
+    """
+    Estimate the number of CNOTs to decompose the isometry using Knill.
+    """
+    unitary = _extend_to_unitary(iso, log_lines, log_cols)
+
+    eigval, eigvec = np.linalg.eig(unitary)
+    arg = np.angle(eigval)
+
+    from qclib.state_preparation.schmidt import cnot_count as schmidt_cnot_count # pylint: disable=import-outside-toplevel
+
+    cnots = 0
+    for i in range(2**log_lines):
+        if np.abs(arg[i]) > 10**-15:
+            state = eigvec[:,i]
+
+            # Two times Schmidt state preparation
+            cnots += 2 * schmidt_cnot_count(state)
+
+            # MCP
+            if log_lines == 2:
+                cnots += 1
+            elif log_lines > 2:
+                cnots += 16*log_lines**2 - 60*log_lines + 42
+
+    return cnots
+
+def _cnot_count_estimate_ccd(log_lines, log_cols):
+    """
+    Estimate the number of CNOTs to decompose the isometry using CCD.
+    """
+    cnots = 0
+    for k in range(2**log_cols):
+        k_bin = '{:0{}b}'.format(k, log_lines)
+        # G_K
+        for i in range(log_lines):
+            target = log_lines - i - 1
+            control = list(range(target))
+            ancilla = list(range(target+1, log_lines))
+
+            if _k_s(k, i) == 0 and _b(k, i+1) != 0:
+                # MCG implemented as a UCG up to a diagonal
+                n_qubits = sum([k_bin[q] == '1' for q in control+ancilla]) + 1
+                cnots += 2**(n_qubits - 1) - 1
+
+            # UCG up to a diagonal
+            n_qubits = len(control) + 1
+            cnots += 2**(n_qubits - 1) - 1
+
+    # Diagonal
+    if log_cols > 0:
+        cnots += 2**log_cols - 2
+
+    return cnots
```

### Comparing `qclib-0.0.8/qclib/state_preparation/apqm.py` & `qclib-0.0.9/qclib/state_preparation/apqm.py`

 * *Files identical despite different names*

### Comparing `qclib-0.0.8/qclib/state_preparation/bdsp.py` & `qclib-0.0.9/qclib/state_preparation/bdsp.py`

 * *Files identical despite different names*

### Comparing `qclib-0.0.8/qclib/state_preparation/cvoqram.py` & `qclib-0.0.9/qclib/state_preparation/cvoqram.py`

 * *Files identical despite different names*

### Comparing `qclib-0.0.8/qclib/state_preparation/dcsp.py` & `qclib-0.0.9/qclib/state_preparation/dcsp.py`

 * *Files identical despite different names*

### Comparing `qclib-0.0.8/qclib/state_preparation/mottonen.py` & `qclib-0.0.9/qclib/state_preparation/mottonen.py`

 * *Files identical despite different names*

### Comparing `qclib-0.0.8/qclib/state_preparation/pivot.py` & `qclib-0.0.9/qclib/state_preparation/pivot.py`

 * *Files identical despite different names*

### Comparing `qclib-0.0.8/qclib/state_preparation/util/angle_tree_preparation.py` & `qclib-0.0.9/qclib/state_preparation/util/angle_tree_preparation.py`

 * *Files 10% similar despite different names*

```diff
@@ -42,21 +42,26 @@
 
 def create_angles_tree(state_tree):
     """
     :param state_tree: state_tree is an output of state_decomposition function
     :param tree: used in the recursive calls
     :return: tree with angles that will be used to perform the state preparation
     """
-    #angle_y = 0.0
-    #angle_z = 0.0
-    #if state_tree.right:
     amp = 0.0
     if state_tree.amplitude != 0.0:
         amp = state_tree.right.amplitude / state_tree.amplitude
-    angle_y = 2 * np.arcsin( np.abs(amp) )
+
+    # Avoid out-of-domain value due to numerical error.
+    if np.abs(amp) < -1.0:
+        angle_y = -np.pi
+    elif np.abs(amp) > 1.0:
+        angle_y = np.pi
+    else:
+        angle_y = 2 * np.arcsin( np.abs(amp) )
+
     angle_z = 2 * np.angle(amp)
 
     node = NodeAngleTree(state_tree.index, state_tree.level, angle_y, angle_z, None, None)
 
     if not is_leaf(state_tree.left):
         node.right = create_angles_tree(state_tree.right)
         node.left = create_angles_tree(state_tree.left)
```

### Comparing `qclib-0.0.8/qclib/state_preparation/util/state_tree_preparation.py` & `qclib-0.0.9/qclib/state_preparation/util/state_tree_preparation.py`

 * *Files identical despite different names*

### Comparing `qclib-0.0.8/qclib/state_preparation/util/tree_register.py` & `qclib-0.0.9/qclib/state_preparation/util/tree_register.py`

 * *Files identical despite different names*

### Comparing `qclib-0.0.8/qclib/state_preparation/util/tree_utils.py` & `qclib-0.0.9/qclib/state_preparation/util/tree_utils.py`

 * *Files identical despite different names*

### Comparing `qclib-0.0.8/qclib/state_preparation/util/tree_walk.py` & `qclib-0.0.9/qclib/state_preparation/util/tree_walk.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,16 +42,16 @@
         else:
             if target_nodes is None:
                 control_nodes = []                           # initialize the controls
                 target_nodes = [angle_tree]                  # start by the subtree root
             else:
                 target_nodes = children(target_nodes)        # all the nodes in the current level
 
-            angles_y = [node.angle_y for node in target_nodes]
-            angles_z = [node.angle_z for node in target_nodes]
+            angles_y = [float(node.angle_y) for node in target_nodes]
+            angles_z = [float(node.angle_z) for node in target_nodes]
             target_qubit = target_nodes[0].qubit
             control_qubits = [node.qubit for node in control_nodes]
             circuit.ucry(angles_y, control_qubits[::-1], target_qubit)     # qiskit reverse
             if any(angles_z) != 0.0:
                 circuit.ucrz(angles_z, control_qubits[::-1], target_qubit) # qiskit reverse
 
             control_nodes.append(angle_tree)                 # add current node to the controls list
```

### Comparing `qclib-0.0.8/qclib/state_preparation/ventura.py` & `qclib-0.0.9/qclib/state_preparation/ventura.py`

 * *Files identical despite different names*

### Comparing `qclib-0.0.8/qclib/util.py` & `qclib-0.0.9/qclib/util.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,15 +49,15 @@
     """
 
     backend = AerSimulator()
     tcirc = transpile(circ, backend)
     tcirc.save_statevector()
     state_vector = backend.run(tcirc).result().get_statevector()
 
-    return state_vector
+    return np.array(state_vector)
 
 
 def replace_all_values_with(new_value, dataset):
     """
         Given a list of tuples (v, b),where v is the value
         and b is the binary pattern associated to it.
         this procedure performs the task of replacing
```

### Comparing `qclib-0.0.8/qclib.egg-info/PKG-INFO` & `qclib-0.0.9/qclib.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qclib
-Version: 0.0.8
+Version: 0.0.9
 Summary: A quantum computing library using qiskit
 Home-page: https://github.com/qclib/qclib
 Author: Adenilton Silva
 Author-email: ajsilva@cin.ufpe.br
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `qclib-0.0.8/qclib.egg-info/SOURCES.txt` & `qclib-0.0.9/qclib.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,38 +1,48 @@
 LICENSE.md
 README.md
 setup.cfg
 setup.py
 qclib/__init__.py
+qclib/entanglement.py
 qclib/isometry.py
 qclib/unitary.py
 qclib/util.py
 qclib.egg-info/PKG-INFO
 qclib.egg-info/SOURCES.txt
 qclib.egg-info/dependency_links.txt
 qclib.egg-info/requires.txt
 qclib.egg-info/top_level.txt
+qclib/gates/__init__.py
+qclib/gates/majority.py
+qclib/gates/mc_gate.py
 qclib/state_preparation/__init__.py
 qclib/state_preparation/apqm.py
+qclib/state_preparation/baa_schmidt.py
 qclib/state_preparation/bdsp.py
 qclib/state_preparation/cvoqram.py
 qclib/state_preparation/dcsp.py
+qclib/state_preparation/gleining.py
 qclib/state_preparation/mottonen.py
 qclib/state_preparation/pivot.py
 qclib/state_preparation/schmidt.py
 qclib/state_preparation/ventura.py
 qclib/state_preparation/util/__init__.py
 qclib/state_preparation/util/angle_tree_preparation.py
+qclib/state_preparation/util/baa.py
 qclib/state_preparation/util/state_tree_preparation.py
 qclib/state_preparation/util/tree_register.py
 qclib/state_preparation/util/tree_utils.py
 qclib/state_preparation/util/tree_walk.py
 test/__init__.py
+test/test_baa.py
+test/test_baa_schmidt.py
 test/test_bdsp.py
 test/test_dcsp.py
+test/test_gleining.py
 test/test_isometry.py
 test/test_majority.py
 test/test_mc_gate.py
 test/test_mottonen.py
 test/test_pqm.py
 test/test_schmidt.py
 test/test_sparse_sp.py
```

### Comparing `qclib-0.0.8/setup.py` & `qclib-0.0.9/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="qclib",
-    version="0.0.8",
+    version="0.0.9",
     author="Adenilton Silva",
     author_email="ajsilva@cin.ufpe.br",
     description="A quantum computing library using qiskit",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/qclib/qclib",
     packages=setuptools.find_packages(),
```

### Comparing `qclib-0.0.8/test/test_bdsp.py` & `qclib-0.0.9/test/test_bdsp.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,19 +12,20 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """ Test bidirectional state preparation """
 
 from unittest import TestCase
 import numpy as np
-from qiskit import ClassicalRegister, Aer
+from qiskit import ClassicalRegister
+from qiskit.providers.aer.backends import AerSimulator
 from qclib.state_preparation.bdsp import initialize
 from .util import measurement
 
-backend = Aer.get_backend('qasm_simulator')
+backend = AerSimulator()
 SHOTS = 8192
 
 
 class TestBdsp(TestCase):
     """ Testing bdsp """
 
     @staticmethod
```

### Comparing `qclib-0.0.8/test/test_dcsp.py` & `qclib-0.0.9/test/test_dcsp.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,19 +12,20 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """ Test divide-and-conquer state preparation """
 
 from unittest import TestCase
 import numpy as np
-from qiskit import ClassicalRegister, Aer
+from qiskit import ClassicalRegister
+from qiskit.providers.aer.backends import AerSimulator
 from qclib.state_preparation.dcsp import initialize
 from .util import measurement
 
-backend = Aer.get_backend('qasm_simulator')
+backend = AerSimulator()
 SHOTS = 8192
 
 class TestInitialize(TestCase):
     """ Testing divide-and-conquer state preparation """
 
     @staticmethod
     def dcsp_experiment(state):
```

### Comparing `qclib-0.0.8/test/test_isometry.py` & `qclib-0.0.9/test/test_isometry.py`

 * *Files identical despite different names*

### Comparing `qclib-0.0.8/test/test_majority.py` & `qclib-0.0.9/test/test_majority.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """ Test majority gate """
 
 from unittest import TestCase
 from qiskit import ClassicalRegister, QuantumRegister, QuantumCircuit
-from qclib.gate.majority import operate as majority
+from qclib.gates.majority import operate as majority
 from qclib.util import get_counts
 
 class TestMajority(TestCase):
     """ Testing qclib.gate.majority """
     @staticmethod
     def _run_majority(bin_input):
         """ Run majority gate and return counts """
```

### Comparing `qclib-0.0.8/test/test_mc_gate.py` & `qclib-0.0.9/test/test_mc_gate.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 from unittest import TestCase
 
 import numpy as np
 from scipy.stats import unitary_group
 import qiskit
 import qclib.util
-from qclib.gate.mc_gate import mc_gate
+from qclib.gates.mc_gate import mc_gate
 
 
 class TestLinearToffoli(TestCase):
     """ Testing qclib.gate.toffoli """
 
     def test_controlled_gate(self):
         """ Testing multi controlled gate """
```

### Comparing `qclib-0.0.8/test/test_mottonen.py` & `qclib-0.0.9/test/test_mottonen.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,22 +14,23 @@
 
 """
 Tests for the mottonen.py module.
 """
 
 from unittest import TestCase
 import numpy as np
-from qiskit import ClassicalRegister, execute, Aer
+from qiskit import ClassicalRegister, execute
+from qiskit.providers.aer.backends import AerSimulator
 from qclib.state_preparation.mottonen import initialize
 from qclib.util import get_state
 
 # pylint: disable=missing-function-docstring
 # pylint: disable=missing-class-docstring
 
-backend = Aer.get_backend('qasm_simulator')
+backend = AerSimulator()
 SHOTS = 8192
 
 class TestMottonen(TestCase):
     @staticmethod
     def measurement(circuit, n_qubits, classical_reg):
         circuit.measure(list(range(n_qubits)), classical_reg)
```

### Comparing `qclib-0.0.8/test/test_pqm.py` & `qclib-0.0.9/test/test_pqm.py`

 * *Files identical despite different names*

### Comparing `qclib-0.0.8/test/test_schmidt.py` & `qclib-0.0.9/test/test_schmidt.py`

 * *Files 19% similar despite different names*

```diff
@@ -14,15 +14,17 @@
 
 """
 Tests for the schmidt.py module.
 """
 
 from unittest import TestCase
 import numpy as np
-from qiskit import ClassicalRegister, execute, Aer
+from itertools import combinations
+from qiskit import ClassicalRegister, execute, transpile
+from qiskit.providers.aer.backends import AerSimulator
 from qclib.state_preparation.schmidt import initialize
 from qclib.util import get_state
 
 # pylint: disable=missing-function-docstring
 # pylint: disable=missing-class-docstring
 
 class TestSchmidt(TestCase):
@@ -30,54 +32,76 @@
     def mae(state, ideal):
         """
         Mean Absolute Error
         """
         return np.sum(np.abs(state-ideal))/len(ideal)
 
     @staticmethod
+    def fidelity(state1, state2):
+        bra = np.conj(state1)
+        ket = state2
+
+        return np.abs(bra.dot(ket))**2
+
+    @staticmethod
     def get_counts(circuit):
         n_qubits = circuit.num_qubits
         classical_reg = ClassicalRegister(n_qubits)
         circuit.add_register(classical_reg)
         circuit.measure(list(range(n_qubits)), classical_reg)
 
-        backend = Aer.get_backend('qasm_simulator')
+        backend = AerSimulator()
         counts = execute(circuit, backend, shots=8192).result().get_counts()
 
         counts_with_zeros = {}
         for i in range(2**n_qubits):
             pattern = '{:0{}b}'.format(i, n_qubits)
             if pattern in counts:
                 counts_with_zeros[pattern] = counts[pattern]
             else:
                 counts_with_zeros[pattern] = 0.0
 
         sum_values = sum(counts.values())
         return [ value/sum_values for (key, value) in counts_with_zeros.items() ]
 
-    def _test_initialize_rank(self, rank, max_mae=10**-15):
+    def _test_initialize_mae(self, rank=0, max_mae=10**-15):
         state_vector = np.random.rand(32) + np.random.rand(32) * 1j
         state_vector = state_vector / np.linalg.norm(state_vector)
 
-        circuit = initialize(state_vector, low_rank=rank)
+        qubits = list(range(5))
+        partitions = combinations(qubits, 3)
+        for partition in partitions:
+            circuit = initialize(state_vector, low_rank=rank, partition=partition)
 
-        state = get_state(circuit)
+            state = get_state(circuit)
 
-        self.assertTrue(TestSchmidt.mae(state,state_vector) < max_mae)
+            self.assertTrue(TestSchmidt.mae(state, state_vector) < max_mae)
 
     def test_initialize_full_rank(self):
         state_vector = np.random.rand(32) + np.random.rand(32) * 1j
         state_vector = state_vector / np.linalg.norm(state_vector)
 
         circuit = initialize(state_vector)
 
         state = get_state(circuit)
 
         self.assertTrue(np.allclose(state_vector, state))
 
+    def test_initialize_ame(self):
+        """ Test initialization of a absolutely maximally entangled state"""
+        state_vector = [1, 1, 1, 1,1,-1,-1, 1, 1,-1,-1, 1, 1, 1,1,1,
+                        1, 1,-1,-1,1,-1, 1,-1,-1, 1,-1, 1,-1,-1,1,1]
+        state_vector = state_vector / np.linalg.norm(state_vector)
+
+        circuit = initialize(state_vector)
+
+        state = get_state(circuit)
+
+        self.assertTrue(np.allclose(state_vector, state))
+
     def test_measurement_full_rank(self):
         state_vector = np.random.rand(32) + np.random.rand(32) * 1j
         state_vector = state_vector / np.linalg.norm(state_vector)
 
         circuit = initialize(state_vector)
 
         state = TestSchmidt.get_counts(circuit)
@@ -92,17 +116,31 @@
         circuit = initialize(state_vector, low_rank=5)
 
         state = get_state(circuit)
 
         self.assertTrue(np.allclose(state_vector, state)) # same as unitary.
 
     def test_initialize_rank_4(self):
-        self._test_initialize_rank(4, max_mae=10**-14)
+        self._test_initialize_mae(4, max_mae=10**-14)
 
     def test_initialize_rank_3(self):
-        self._test_initialize_rank(3, max_mae=0.04)
+        self._test_initialize_mae(3, max_mae=0.04)
 
     def test_initialize_rank_2(self):
-        self._test_initialize_rank(2, max_mae=0.06)
+        self._test_initialize_mae(2, max_mae=0.06)
 
     def test_initialize_rank_1(self):
-        self._test_initialize_rank(1, max_mae=0.0825)
+        self._test_initialize_mae(1, max_mae=0.0875)
+
+    def test_cnot_count_rank_1(self):
+        # Builds a rank 1 state.
+        state_vector = [1]
+        for _ in range(5):
+            vec = np.random.rand(2) + np.random.rand(2) * 1j
+            vec = vec / np.linalg.norm(vec)
+            state_vector = np.kron(state_vector, vec)
+
+        circuit = initialize(state_vector)
+        transpiled_circuit = transpile(circuit, basis_gates=['u', 'cx'], optimization_level=3)
+
+        # The cnots count must be zero (i.e. not present in the dictionary).
+        self.assertTrue('cx' not in transpiled_circuit.count_ops())
```

### Comparing `qclib-0.0.8/test/test_sparse_sp.py` & `qclib-0.0.9/test/test_sparse_sp.py`

 * *Files identical despite different names*

### Comparing `qclib-0.0.8/test/test_unitary.py` & `qclib-0.0.9/test/test_unitary.py`

 * *Files identical despite different names*

### Comparing `qclib-0.0.8/test/test_ventura.py` & `qclib-0.0.9/test/test_ventura.py`

 * *Files identical despite different names*

### Comparing `qclib-0.0.8/test/util.py` & `qclib-0.0.9/test/util.py`

 * *Files identical despite different names*

