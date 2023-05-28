# Comparing `tmp/kodexa-6.1.4.tar.gz` & `tmp/kodexa-6.2.25104807008.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kodexa-6.1.4.tar", max compression
+gzip compressed data, was "kodexa-6.2.25104807008.tar", max compression
```

## Comparing `kodexa-6.1.4.tar` & `kodexa-6.2.25104807008.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0    11357 2023-04-03 12:23:08.183390 kodexa-6.1.4/LICENSE
--rw-r--r--   0        0        0     2256 2023-04-03 12:23:08.183390 kodexa-6.1.4/README.md
--rw-r--r--   0        0        0      847 2023-04-03 12:23:08.187390 kodexa-6.1.4/kodexa/__init__.py
--rw-r--r--   0        0        0      171 2023-04-03 12:23:08.187390 kodexa-6.1.4/kodexa/assistant/__init__.py
--rw-r--r--   0        0        0     7952 2023-04-03 12:23:08.187390 kodexa-6.1.4/kodexa/assistant/assistant.py
--rw-r--r--   0        0        0      297 2023-04-03 12:23:08.187390 kodexa-6.1.4/kodexa/connectors/__init__.py
--rw-r--r--   0        0        0     7722 2023-04-03 12:23:08.187390 kodexa-6.1.4/kodexa/connectors/connectors.py
--rw-r--r--   0        0        0      720 2023-04-03 12:23:08.187390 kodexa-6.1.4/kodexa/model/__init__.py
--rw-r--r--   0        0        0      753 2023-04-03 12:23:08.187390 kodexa-6.1.4/kodexa/model/base.py
--rw-r--r--   0        0        0    88889 2023-04-03 12:23:08.187390 kodexa-6.1.4/kodexa/model/model.py
--rw-r--r--   0        0        0   116415 2023-04-03 12:23:08.191390 kodexa-6.1.4/kodexa/model/objects.py
--rw-r--r--   0        0        0    37847 2023-04-03 12:23:08.191390 kodexa-6.1.4/kodexa/model/persistence.py
--rw-r--r--   0        0        0      236 2023-04-03 12:23:08.191390 kodexa-6.1.4/kodexa/pipeline/__init__.py
--rw-r--r--   0        0        0    19763 2023-04-03 12:23:08.191390 kodexa-6.1.4/kodexa/pipeline/pipeline.py
--rw-r--r--   0        0        0      216 2023-04-03 12:23:08.191390 kodexa-6.1.4/kodexa/platform/__init__.py
--rw-r--r--   0        0        0   109544 2023-04-03 12:23:08.191390 kodexa-6.1.4/kodexa/platform/client.py
--rw-r--r--   0        0        0    27604 2023-04-03 12:23:08.191390 kodexa-6.1.4/kodexa/platform/kodexa.py
--rw-r--r--   0        0        0      100 2023-04-03 12:23:08.191390 kodexa-6.1.4/kodexa/selectors/__init__.py
--rw-r--r--   0        0        0    13499 2023-04-03 12:23:08.191390 kodexa-6.1.4/kodexa/selectors/ast.py
--rw-r--r--   0        0        0     3698 2023-04-03 12:23:08.191390 kodexa-6.1.4/kodexa/selectors/core.py
--rw-r--r--   0        0        0     3735 2023-04-03 12:23:08.191390 kodexa-6.1.4/kodexa/selectors/lexrules.py
--rw-r--r--   0        0        0     2354 2023-04-03 12:23:08.191390 kodexa-6.1.4/kodexa/selectors/lextab.py
--rw-r--r--   0        0        0       60 2023-04-03 12:23:08.191390 kodexa-6.1.4/kodexa/selectors/lextab.pyi
--rw-r--r--   0        0        0     7054 2023-04-03 12:23:08.191390 kodexa-6.1.4/kodexa/selectors/parserules.py
--rw-r--r--   0        0        0       60 2023-04-03 12:23:08.191390 kodexa-6.1.4/kodexa/selectors/parserules.pyi
--rw-r--r--   0        0        0    21267 2023-04-03 12:23:08.191390 kodexa-6.1.4/kodexa/selectors/parsetab.py
--rw-r--r--   0        0        0       60 2023-04-03 12:23:08.191390 kodexa-6.1.4/kodexa/selectors/parsetab.pyi
--rw-r--r--   0        0        0        0 2023-04-03 12:23:08.191390 kodexa-6.1.4/kodexa/spatial/__init__.py
--rw-r--r--   0        0        0    18991 2023-04-03 12:23:08.191390 kodexa-6.1.4/kodexa/spatial/azure_models.py
--rw-r--r--   0        0        0     2738 2023-04-03 12:23:08.191390 kodexa-6.1.4/kodexa/spatial/bbox_common.py
--rw-r--r--   0        0        0    34222 2023-04-03 12:23:08.191390 kodexa-6.1.4/kodexa/spatial/table_form_common.py
--rw-r--r--   0        0        0      160 2023-04-03 12:23:08.191390 kodexa-6.1.4/kodexa/steps/__init__.py
--rw-r--r--   0        0        0     9587 2023-04-03 12:23:08.191390 kodexa-6.1.4/kodexa/steps/common.py
--rw-r--r--   0        0        0      159 2023-04-03 12:23:08.191390 kodexa-6.1.4/kodexa/testing/__init__.py
--rw-r--r--   0        0        0      932 2023-04-03 12:23:08.191390 kodexa-6.1.4/kodexa/testing/test_components.py
--rw-r--r--   0        0        0    13596 2023-04-03 12:23:08.191390 kodexa-6.1.4/kodexa/testing/test_utils.py
--rw-r--r--   0        0        0       52 2023-04-03 12:23:08.191390 kodexa-6.1.4/kodexa/training/__init__.py
--rw-r--r--   0        0        0        0 2023-04-03 12:23:08.191390 kodexa-6.1.4/kodexa/training/train_utils.py
--rw-r--r--   0        0        0     1291 2023-04-03 12:23:23.515580 kodexa-6.1.4/pyproject.toml
--rw-r--r--   0        0        0     3536 1970-01-01 00:00:00.000000 kodexa-6.1.4/setup.py
--rw-r--r--   0        0        0     3600 1970-01-01 00:00:00.000000 kodexa-6.1.4/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-28 14:14:34.600176 kodexa-6.2.25104807008/LICENSE
+-rw-r--r--   0        0        0     2804 2023-05-28 14:14:34.600176 kodexa-6.2.25104807008/README.md
+-rw-r--r--   0        0        0      847 2023-05-28 14:14:34.608176 kodexa-6.2.25104807008/kodexa/__init__.py
+-rw-r--r--   0        0        0      171 2023-05-28 14:14:34.608176 kodexa-6.2.25104807008/kodexa/assistant/__init__.py
+-rw-r--r--   0        0        0    12530 2023-05-28 14:14:34.608176 kodexa-6.2.25104807008/kodexa/assistant/assistant.py
+-rw-r--r--   0        0        0      297 2023-05-28 14:14:34.608176 kodexa-6.2.25104807008/kodexa/connectors/__init__.py
+-rw-r--r--   0        0        0     7722 2023-05-28 14:14:34.608176 kodexa-6.2.25104807008/kodexa/connectors/connectors.py
+-rw-r--r--   0        0        0      720 2023-05-28 14:14:34.608176 kodexa-6.2.25104807008/kodexa/model/__init__.py
+-rw-r--r--   0        0        0      753 2023-05-28 14:14:34.608176 kodexa-6.2.25104807008/kodexa/model/base.py
+-rw-r--r--   0        0        0    96183 2023-05-28 14:14:34.608176 kodexa-6.2.25104807008/kodexa/model/model.py
+-rw-r--r--   0        0        0   116484 2023-05-28 14:14:34.608176 kodexa-6.2.25104807008/kodexa/model/objects.py
+-rw-r--r--   0        0        0    38334 2023-05-28 14:14:34.608176 kodexa-6.2.25104807008/kodexa/model/persistence.py
+-rw-r--r--   0        0        0      236 2023-05-28 14:14:34.608176 kodexa-6.2.25104807008/kodexa/pipeline/__init__.py
+-rw-r--r--   0        0        0    19763 2023-05-28 14:14:34.608176 kodexa-6.2.25104807008/kodexa/pipeline/pipeline.py
+-rw-r--r--   0        0        0      216 2023-05-28 14:14:34.608176 kodexa-6.2.25104807008/kodexa/platform/__init__.py
+-rw-r--r--   0        0        0   110049 2023-05-28 14:14:34.608176 kodexa-6.2.25104807008/kodexa/platform/client.py
+-rw-r--r--   0        0        0    28246 2023-05-28 14:14:34.608176 kodexa-6.2.25104807008/kodexa/platform/kodexa.py
+-rw-r--r--   0        0        0      100 2023-05-28 14:14:34.608176 kodexa-6.2.25104807008/kodexa/selectors/__init__.py
+-rw-r--r--   0        0        0    13499 2023-05-28 14:14:34.608176 kodexa-6.2.25104807008/kodexa/selectors/ast.py
+-rw-r--r--   0        0        0     3698 2023-05-28 14:14:34.608176 kodexa-6.2.25104807008/kodexa/selectors/core.py
+-rw-r--r--   0        0        0     3735 2023-05-28 14:14:34.608176 kodexa-6.2.25104807008/kodexa/selectors/lexrules.py
+-rw-r--r--   0        0        0     2354 2023-05-28 14:14:34.608176 kodexa-6.2.25104807008/kodexa/selectors/lextab.py
+-rw-r--r--   0        0        0       60 2023-05-28 14:14:34.612176 kodexa-6.2.25104807008/kodexa/selectors/lextab.pyi
+-rw-r--r--   0        0        0     7054 2023-05-28 14:14:34.612176 kodexa-6.2.25104807008/kodexa/selectors/parserules.py
+-rw-r--r--   0        0        0       60 2023-05-28 14:14:34.612176 kodexa-6.2.25104807008/kodexa/selectors/parserules.pyi
+-rw-r--r--   0        0        0    21267 2023-05-28 14:14:34.612176 kodexa-6.2.25104807008/kodexa/selectors/parsetab.py
+-rw-r--r--   0        0        0       60 2023-05-28 14:14:34.612176 kodexa-6.2.25104807008/kodexa/selectors/parsetab.pyi
+-rw-r--r--   0        0        0        0 2023-05-28 14:14:34.612176 kodexa-6.2.25104807008/kodexa/spatial/__init__.py
+-rw-r--r--   0        0        0    18991 2023-05-28 14:14:34.612176 kodexa-6.2.25104807008/kodexa/spatial/azure_models.py
+-rw-r--r--   0        0        0     2738 2023-05-28 14:14:34.612176 kodexa-6.2.25104807008/kodexa/spatial/bbox_common.py
+-rw-r--r--   0        0        0    34222 2023-05-28 14:14:34.612176 kodexa-6.2.25104807008/kodexa/spatial/table_form_common.py
+-rw-r--r--   0        0        0      160 2023-05-28 14:14:34.612176 kodexa-6.2.25104807008/kodexa/steps/__init__.py
+-rw-r--r--   0        0        0     9587 2023-05-28 14:14:34.612176 kodexa-6.2.25104807008/kodexa/steps/common.py
+-rw-r--r--   0        0        0      159 2023-05-28 14:14:34.612176 kodexa-6.2.25104807008/kodexa/testing/__init__.py
+-rw-r--r--   0        0        0      932 2023-05-28 14:14:34.612176 kodexa-6.2.25104807008/kodexa/testing/test_components.py
+-rw-r--r--   0        0        0    13596 2023-05-28 14:14:34.612176 kodexa-6.2.25104807008/kodexa/testing/test_utils.py
+-rw-r--r--   0        0        0       52 2023-05-28 14:14:34.612176 kodexa-6.2.25104807008/kodexa/training/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-28 14:14:34.612176 kodexa-6.2.25104807008/kodexa/training/train_utils.py
+-rw-r--r--   0        0        0     1301 2023-05-28 14:15:05.039914 kodexa-6.2.25104807008/pyproject.toml
+-rw-r--r--   0        0        0     4103 1970-01-01 00:00:00.000000 kodexa-6.2.25104807008/setup.py
+-rw-r--r--   0        0        0     4158 1970-01-01 00:00:00.000000 kodexa-6.2.25104807008/PKG-INFO
```

### Comparing `kodexa-6.1.4/LICENSE` & `kodexa-6.2.25104807008/LICENSE`

 * *Files identical despite different names*

### Comparing `kodexa-6.1.4/README.md` & `kodexa-6.2.25104807008/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -32,15 +32,23 @@
 
 ## Documentation & Examples
 
 Documentation is available at the [Kodexa Documentation Portal](https://docs.kodexa.com)
 
 ## Current Development
 
-The main branch is 6.0 which is a production release.
+[//]: # (Replace it with the diagrams and descriptions for build releases)
+**BUILD VERSION FLOW**
+![build-version-flow.png](docs%2Fbuild-version-flow.png)
+Build version will differ based on the branches that are published to pypi.
+
+**GITHUB PROCESS**
+![github-process.png](docs%2Fgithub-process.png)
+Changes that contain bugs, features, and fixes should first be pushed to the test branch. 
+Once these changes are thoroughly tested, they can be submitted as a pull request to the main branch. The pull request should be reviewed and approved by an appropriate person before the changes can be merged.
 
 ## Set-up
 
 We use poetry to manage our dependencies, so you can install them with:
 
     poetry install
 
@@ -51,7 +59,8 @@
 # Contributing
 
 We welcome contributions to the Kodexa platform. Please see our [contributing guide](CONTRIBUTING.md) for more details.
 
 # License
 
 Apache 2.0
+
```

### Comparing `kodexa-6.1.4/kodexa/__init__.py` & `kodexa-6.2.25104807008/kodexa/__init__.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.1.4/kodexa/connectors/connectors.py` & `kodexa-6.2.25104807008/kodexa/connectors/connectors.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.1.4/kodexa/model/__init__.py` & `kodexa-6.2.25104807008/kodexa/model/__init__.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.1.4/kodexa/model/base.py` & `kodexa-6.2.25104807008/kodexa/model/base.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.1.4/kodexa/model/model.py` & `kodexa-6.2.25104807008/kodexa/model/model.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,16 @@
 from enum import Enum
 from typing import Any, List, Optional
 
 import msgpack
 from addict import Dict
 
 from kodexa.model.base import KodexaBaseModel
-from kodexa.model.objects import ContentObject
+from kodexa.model.objects import ContentObject, FeatureSet
+import deepdiff
 
 
 class Ref:
 
     def __init__(self, ref: str):
         self.ref: str = ref
         first_part = ref
@@ -46,24 +47,26 @@
 
 
 class ContentException(Dict):
     """A content exception represents an issue identified during labeling or validation at the document level"""
 
     def __init__(self, exception_type: str, message: str, severity: str = 'ERROR', tag: Optional[str] = None,
                  group_uuid: Optional[str] = None, tag_uuid: Optional[str] = None,
-                 exception_details: Optional[str] = None, node_uuid: Optional[str] = None, *args, **kwargs):
+                 exception_details: Optional[str] = None, node_uuid: Optional[str] = None, value: Optional[str] = None,
+                 *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.tag = tag
         self.message = message
         self.exception_details = exception_details
         self.group_uuid = group_uuid
         self.tag_uuid = tag_uuid
         self.exception_type = exception_type
         self.node_uuid = node_uuid
         self.severity = severity
+        self.value = value
 
 
 class Tag(Dict):
     """A tag represents the metadata for a label that is applies as a feature on a content node"""
 
     def __init__(self, start: Optional[int] = None, end: Optional[int] = None, value: Optional[str] = None,
                  uuid: Optional[str] = None, data: Any = None, *args, confidence: Optional[float] = None,
@@ -75,15 +78,15 @@
         """The start position (zero indexed) of the content within the node, if None then label is applied to the whole node"""
         self.end: Optional[int] = end
         """The end position (zero indexed) of the content within the node, if None then label is applied to the whole node"""
         self.value: Optional[str] = value
         """A string representing the value that was labelled in the node"""
         self.data: Optional[Any] = data
         """Any data object (JSON serializable) that you wish to associate with the label"""
-        self.uuid: Optional[str] = uuid
+        self.uuid: Optional[str] = uuid or str(uuid.uuid4())
         """The UUID for this tag instance, this allows tags that are on different content nodes to be related through the same UUID"""
         self.confidence: Optional[float] = confidence
         """The confidence of the tag in a range of 0-1"""
         self.index: Optional[int] = index
         """The tag index, this is used to allow us to order tags, and understand the ordering of parent child tag relationships"""
         self.bbox: Optional[List[int]] = bbox
         """The optional bounding box that can be used if the label is spatial (based on the node as the container)"""
@@ -1532,20 +1535,22 @@
 
         while True:
             node = self.get_parent().get_node_at_index(search_index) if self.get_parent() else None
 
             if not node:
                 if (traverse == traverse.ALL or traverse == traverse.PARENT) and self.get_parent().get_parent():
                     try:
-                        potential_next_node = self.get_parent().get_parent().get_children()[self.get_parent().index + 1].get_children()[0]
+                        potential_next_node = \
+                            self.get_parent().get_parent().get_children()[self.get_parent().index + 1].get_children()[0]
                         if potential_next_node:
                             return potential_next_node
                     except:
                         # traverse additional layer
-                        potential_next_node = self.get_parent().get_parent().get_parent().get_children()[self.get_parent().get_parent().index + 1].get_children()[0].get_children()[0]
+                        potential_next_node = self.get_parent().get_parent().get_parent().get_children()[
+                            self.get_parent().get_parent().index + 1].get_children()[0].get_children()[0]
                         if potential_next_node:
                             return potential_next_node
                 return node
 
             if compiled_node_type_re.match(node.node_type) and (not skip_virtual or not node.virtual):
                 if (not has_no_content and node.content) or has_no_content:
                     return node
@@ -1703,14 +1708,140 @@
 
     @classmethod
     def from_dict(cls, dict_val):
         return ContentClassification(label=dict_val['label'], taxonomy=dict_val.get('taxonomy'),
                                      selector=dict_val.get('selector'), confidence=dict_val.get('confidence'))
 
 
+class FeatureSetDiff:
+    """
+    A utility class that can be used to diff two feature sets
+    """
+
+    def __init__(self, first_feature_set: FeatureSet, second_feature_set: FeatureSet):
+        self.first_feature_map = self.parse_feature_set(first_feature_set)
+        self.second_feature_map = self.parse_feature_set(second_feature_set)
+        self._differences = deepdiff.DeepDiff(self.first_feature_map, self.second_feature_map,
+                                              exclude_obj_callback=self.exclude_callback).to_dict()
+        self._changed_nodes = self.get_changed_nodes()
+
+    def get_differences(self):
+        """
+        :return: Data dictionaries that contains the differences of two feature sets
+        """
+        if 'type_changes' in self._differences:
+            self._differences.pop('type_changes')
+
+        return self._differences
+
+    def get_changed_nodes(self):
+        """
+        :return: Data dictionary of added and removed nodes
+        """
+        return self._changed_nodes
+
+    def get_exclude_paths(self):
+        """
+        :return: List of paths to exclude
+        """
+        return ['shape', 'group_uuid', 'uuid', 'parent_group_uuid', 'single']
+
+    def exclude_callback(self, path, key):
+        """
+        Checks if the key is to be exluceded from the diff
+        :param path: contains the values of that key
+        :param key: The key of the data dictionary to compare
+        :return: boolean
+        """
+        if any(re.search(exclude_key, key) for exclude_key in self.get_exclude_paths()):
+            return True
+        else:
+            return False
+
+    def parse_feature_set(self, feature_set: FeatureSet):
+        """
+        :param feature_set: The feature set to be parsed
+        :return: Dictionary of feature with the key as the nodeUuid
+        """
+        return {feature.get('nodeUuid'): feature for feature in feature_set.node_features}
+
+    def parsed_values_changed(self):
+        for key, value in self._differences.get('values_changed').items():
+            # Check if the old_value is stil in the second_feature_map. If it is remove the key
+            if key in self.second_feature_map.node_features:
+                self._differences.get('values_changed').remove(key)
+
+    def is_equal(self) -> bool:
+        """
+        Checks if the two feature set is equal to each other
+        :return: This returns a bool
+        """
+        return self._differences == {}
+
+    def get_changed_nodes(self):
+        """
+        :return: A list of nodes that were changed
+        """
+        if self.is_equal():
+            return []
+
+        # Check for new nodes added in the second_feature_map
+        new_added_nodes = []
+
+        # Checked for removed nodes in the first_feature_map
+        removed_nodes = []
+
+        # Checked for modified nodes
+        modified_nodes = []
+        for key, value in self._differences.get('values_changed').items():
+            modified_nodes.append(self.parsed_node_uuid(key))
+
+        # Merge unique nodeUuid of first_feature_map and second_feature_map
+        merged_node_uuids = set(self.first_feature_map.keys()).union(set(self.second_feature_map.keys()))
+        for node_uuid in merged_node_uuids:
+            if node_uuid not in self.first_feature_map:
+                new_added_nodes.append(node_uuid)
+            elif node_uuid not in self.second_feature_map:
+                removed_nodes.append(node_uuid)
+
+        return {
+            'new_added_nodes': new_added_nodes,
+            'removed_nodes': removed_nodes,
+            'existing_modified_nodes': modified_nodes
+        }
+
+    def get_difference_count(self):
+        """
+        :return: The total number of differences between the feature sets
+        """
+        return len(self._differences().keys())
+
+    def parsed_item_added(self):
+        item_added: Dict = self._differences.get('iterable_item_added')
+        if item_added:
+            return {}
+
+        for key, value in item_added.items():
+            node = self.parsed_node_uuid(key)
+            if node in self._changed_nodes['new_added_nodes']:
+                self._differences['iterable_item_added'][key]['details'] = f'Node: {node} was added'
+                continue
+
+            # if node in
+        return self.get_difference_count()
+
+    def parsed_node_uuid(self, key):
+        """
+        :param key: Key of data dictionary
+        :return: node uuid from the key
+        """
+        node = key.split("['")[1].split("']")[0]
+        return node
+
+
 class Document(object):
     """A Document is a collection of metadata and a set of content nodes."""
 
     PREVIOUS_VERSION: str = "1.0.0"
     CURRENT_VERSION: str = "4.0.2"
 
     def __str__(self):
@@ -1758,22 +1889,55 @@
         self.source: SourceMetadata = source
         """Source metadata for this document"""
         self.labels: List[str] = []
         """A list of the document level labels for the document"""
         self.classes: List[ContentClassification] = []
         """A list of the content classifications associated at the document level"""
 
+        self.tag_instances: List[TagInstance] = []
+        """A list of tag instances that contains a set of tag that has a set of nodes"""
+
         # Start persistence layer
         from kodexa.model import PersistenceManager
 
         self._persistence_layer: Optional[PersistenceManager] = PersistenceManager(document=self,
                                                                                    filename=kddb_path,
                                                                                    delete_on_close=delete_on_close)
         self._persistence_layer.initialize()
 
+    def add_tag_instance(self, tag_to_apply, node_list: List[ContentNode]):
+        """
+            This will create a group of a tag with indexes
+        :param tag: name of the tag
+        :param node_indices: contains the list of index of a node
+        :return:
+        """
+        # For each node in the list create/update a feature
+        tag = Tag()
+        for node in node_list:
+            node.add_feature('tag', tag_to_apply, Tag)
+        # Tag Object
+        tag_instance = TagInstance(tag, node_list)
+        self.tag_instances.append(tag_instance)
+
+    def update_tag_instance(self, tag_uuid):
+        for tag_instance in self.tag_instances:
+            if tag_instance.tag.uuid == tag_uuid:
+                # Update attributes of a Tag
+                for node in tag_instance.nodes:
+                    node.get_tag(tag_instance.tag.value, tag_uuid=tag_instance.tag.uuid)
+
+    def get_tag_instance(self, tag):
+        """
+            Get the tag instance based on the tag itself
+        :param tag: name of the tag
+        :return: a list of tag instance
+        """
+        return [tag_instance for tag_instance in self.tag_instances if tag_instance.tag == tag]
+
     def get_persistence(self):
         return self._persistence_layer
 
     def get_all_tags(self):
         return self._persistence_layer.get_all_tags()
 
     def add_model_insight(self, model_insight: ModelInsight):
@@ -2274,14 +2438,57 @@
 
         Returns:
           List[str]: list of associated labels
 
         """
         return self.labels
 
+    def get_feature_set(self) -> FeatureSet:
+        """
+        Build a feature set of all the tagged nodes
+
+        :return:
+        """
+        feature_set = FeatureSet()
+        feature_set.node_features = []
+        for tagged_node in self.get_all_tagged_nodes():
+            node_feature = {
+                'nodeUuid': str(tagged_node.uuid),
+                'features': []
+            }
+
+            feature_set.node_features.append(node_feature)
+
+            # TODO this needs to be cleaned up
+            for feature in tagged_node.get_features():
+                if feature.feature_type == 'tag':
+                    feature_dict = feature.to_dict()
+                    feature_dict['featureType'] = feature.feature_type
+                    feature_dict['name'] = feature.name
+                    node_feature['features'].append(feature_dict)
+
+        return feature_set
+
+    def get_all_tagged_nodes(self) -> List[ContentNode]:
+        """
+        Get all the tagged nodes in the document
+
+        :return:
+        """
+        return self._persistence_layer.get_all_tagged_nodes()
+
+
+class TagInstance:
+    def __init__(self, tag: Tag, nodes):
+        self.tag = tag
+        self.nodes = nodes
+
+    def add_node(self, nodes: List[ContentNode]):
+        self.nodes.extend(nodes)
+
 
 class ContentObjectReference:
     """ """
 
     def __init__(self, content_object: ContentObject, store, document: Document,
                  document_family):
         self.content_object = content_object
```

### Comparing `kodexa-6.1.4/kodexa/model/objects.py` & `kodexa-6.2.25104807008/kodexa/model/objects.py`

 * *Files 0% similar despite different names*

```diff
@@ -1346,14 +1346,15 @@
     list_description: Optional[str] = Field(None, alias='listDescription')
     feature_flag: Optional[str] = Field(None, alias='featureFlag')
     default: Optional[Any] = None
     description: Optional[str] = None
     support_article: Optional[str] = Field(None, alias='supportArticle')
     overview_markdown: Optional[str] = Field(None, alias='overviewMarkdown')
     show_if: Optional[str] = Field(None, alias='showIf')
+    show_on_popup: Optional[bool] = Field(None, alias='showOnPopup')
     possible_values: Optional[List[PossibleValue]] = Field(None, alias='possibleValues')
     properties: Optional[Dict[str, Any]] = None
 
 
 class Overlay(KodexaBaseModel):
     """
     Overlays provide the ability to apply validation, normalization and enrichment
```

### Comparing `kodexa-6.1.4/kodexa/model/persistence.py` & `kodexa-6.2.25104807008/kodexa/model/persistence.py`

 * *Files 1% similar despite different names*

```diff
@@ -577,14 +577,24 @@
         self.cursor.execute("delete from content_exceptions")
         for exception in exceptions:
             self.add_exception(exception)
 
     def clear_model_insights(self):
         self.cursor.execute("delete from model_insights")
 
+    def get_all_tagged_nodes(self):
+        content_nodes = []
+        query = f"select cn_id from ft where f_type in (select id from f_type where name like 'tag:%')"
+        for content_node_ids in self.cursor.execute(
+                query).fetchall():
+            content_nodes.append(self.get_node(content_node_ids[0]))
+
+        return content_nodes
+
+
 
 class SimpleObjectCache(object):
     """
     A simple cache based on ID'd objects, where we will build ID's for new
     objects, store them and also a dirty flag so that it is easy to pull all
     dirty objects and store them as needed
     """
@@ -665,14 +675,18 @@
     def get_all_tags(self):
         return self._underlying_persistence.get_all_tags()
 
     def get_tagged_nodes(self, tag, tag_uuid=None):
         self.flush_cache()
         return self._underlying_persistence.get_tagged_nodes(tag, tag_uuid)
 
+    def get_all_tagged_nodes(self):
+        self.flush_cache()
+        return self._underlying_persistence.get_all_tagged_nodes()
+
     def initialize(self):
         self._underlying_persistence.initialize()
 
         self.node_cache.next_id = self._underlying_persistence.get_next_node_id()
 
     def get_parent(self, node):
         if node.uuid in self.node_parent_cache:
```

### Comparing `kodexa-6.1.4/kodexa/pipeline/pipeline.py` & `kodexa-6.2.25104807008/kodexa/pipeline/pipeline.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.1.4/kodexa/platform/client.py` & `kodexa-6.2.25104807008/kodexa/platform/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -188,14 +188,36 @@
         import pandas as pd
         df = pd.DataFrame(seq(self.list(query, page, page_size, sort, filters)).map(lambda x: x.dict()).to_list())
 
         if 'client' in df:
             df.drop(columns='client', axis=1)
         return df
 
+    def stream_list(self, query="*", sort=None, filters: List[str] = None):
+        """
+            Stream the list of resources
+        :param query:
+        :param sort:
+        :param filters:
+        :return:
+        """
+        page_size = 5
+        page = 1
+
+        if not sort:
+            sort = "id"
+
+        while True:
+            page_response = self.list(query=query, page=page, page_size=page_size, sort=sort, filters=filters)
+            if not page_response.content:
+                break
+            for resource in page_response.content:
+                yield resource
+            page += 1
+
     def list(self, query="*", page=1, page_size=10, sort=None, filters: List[str] = None):
 
         url = f"/api/projects/{self.project.id}/{self.get_type()}"
 
         params = {"query": requests.utils.quote(query),
                   "page": page,
                   "pageSize": page_size}
@@ -385,14 +407,35 @@
         raise NotImplementedError()
 
     def __init__(self, client: "KodexaClient", organization: "OrganizationEndpoint" = None):
         """Initialize the entities endpoint by client and organization"""
         self.client: "KodexaClient" = client
         self.organization: Optional["OrganizationEndpoint"] = organization
 
+    def stream_list(self, query="*", sort=None, filters: List[str] = None):
+        """
+            Stream the list of resources
+        :param query:
+        :param sort:
+        :param filters:
+        :return:
+        """
+        page_size = 5
+        page = 1
+        if not sort:
+            sort = "id"
+
+        while True:
+            page_response = self.list(query=query, page=page, page_size=page_size, sort=sort, filters=filters)
+            if not page_response.content:
+                break
+            for resource in page_response.content:
+                yield resource
+            page += 1
+
     def list(self, query="*", page=1, page_size=10, sort=None, filters: List[str] = None):
         url = f"/api/{self.get_type()}"
 
         params = {"query": query,
                   "page": page,
                   "pageSize": page_size}
 
@@ -1601,15 +1644,15 @@
         start = time.time()
         while time.time() - start < timeout:
             url = f"/api/stores/{self.store_ref.replace(':', '/')}/families/{self.id}"
             updated_document_family = DocumentFamilyEndpoint.parse_obj(self.client.get(url).json()).set_client(
                 self.client)
             if mixin and mixin in updated_document_family.mixins:
                 return updated_document_family
-            if label and label in updated_document_family.labels:
+            if label and any(l.name == label for l in updated_document_family.labels):
                 return updated_document_family
 
             time.sleep(5)
 
         raise Exception(f"Not available on document family {self.id}")
 
     def delete(self):
@@ -1673,36 +1716,18 @@
         """Export the document family as bytes"""
         url = f"/api/stores/{self.store_ref.replace(':', '/')}/families/{self.id}/export"
         get_response = self.client.get(url)
         return get_response.content
 
     def replace_tags(self, document: Document, content_object: Optional[ContentObject] = None):
         """Replace the tags of the document family"""
-        feature_set = FeatureSet()
         if content_object is None:
             content_object = self.content_objects[-1]
-        feature_set.node_features = []
-        for tagged_node in document.select('//*[hasTag()]'):
-            node_feature = {
-                'nodeUuid': str(tagged_node.uuid),
-                'features': []
-            }
-
-            feature_set.node_features.append(node_feature)
-
-            # TODO this needs to be cleaned up
-            for feature in tagged_node.get_features():
-                if feature.feature_type == 'tag':
-                    feature_dict = feature.to_dict()
-                    feature_dict['featureType'] = feature.feature_type
-                    feature_dict['name'] = feature.name
-                    node_feature['features'].append(feature_dict)
-
         url = f"/api/stores/{self.store_ref.replace(':', '/')}/families/{self.id}/objects/{content_object.id}/_replaceTags"
-        self.client.put(url, body=feature_set.dict(by_alias=True))
+        self.client.put(url, body=document.get_feature_set().dict(by_alias=True))
 
 
 class StoreEndpoint(ComponentInstanceEndpoint, Store):
     """Represents a store endpoint"""
 
     def get_type(self) -> str:
         """Get the type of the endpoint"""
@@ -2162,15 +2187,15 @@
             params['sort'] = sort
 
         get_response = self.client.get(f"api/stores/{self.ref.replace(':', '/')}/families",
                                        params=params)
 
         return PageDocumentFamilyEndpoint.parse_obj(get_response.json()).set_client(self.client)
 
-    def stream_filter(self, filter_string: str = "", sort=None):
+    def stream_filter(self, filter_string: str = "", sort=None, limit=None):
         """
             Stream the filter for the document family
         :param query: the query to run
         :param sort: sorting order of the query
         :return:
             A generator of the document families
         """
@@ -2581,18 +2606,18 @@
                                     data={'taxonomyJson': taxonomy.json(exclude={'client'})},
                                     files={'document': document.to_kddb()})
         return response.text
 
 
 class KodexaClient:
 
-    def __init__(self, url=None, access_token=None):
+    def __init__(self, url=None, access_token=None, profile=None):
         from kodexa import KodexaPlatform
-        self.base_url = url if url is not None else KodexaPlatform.get_url()
-        self.access_token = access_token if access_token is not None else KodexaPlatform.get_access_token()
+        self.base_url = url if url is not None else KodexaPlatform.get_url(profile)
+        self.access_token = access_token if access_token is not None else KodexaPlatform.get_access_token(profile)
         self.organizations = OrganizationsEndpoint(self)
         self.projects = ProjectsEndpoint(self)
         self.workspaces = WorkspacesEndpoint(self)
         self.users = UsersEndpoint(self)
         self.memberships = MembershipsEndpoint(self)
         self.executions = ExecutionsEndpoint(self)
 
@@ -2661,24 +2686,24 @@
                                                                            "content-type": "application/json"})
         return process_response(response)
 
     def post(self, url, body=None, data=None, files=None, params=None) -> requests.Response:
         headers = {"x-access-token": self.access_token}
         if files is None:
             headers["content-type"] = "application/json"
+
         response = requests.post(self.get_url(url), json=body, data=data, files=files, params=params,
                                  headers=headers)
         return process_response(response)
 
     def put(self, url, body=None, data=None, files=None, params=None) -> requests.Response:
         headers = {"x-access-token": self.access_token}
         if files is None:
             headers["content-type"] = "application/json"
-        else:
-            headers["content-type"] = "multipart/form-data"
+
         response = requests.put(self.get_url(url), json=body, data=data, files=files, params=params,
                                 headers=headers)
         return process_response(response)
 
     def delete(self, url, params=None) -> requests.Response:
         response = requests.delete(self.get_url(url), params=params, headers={"x-access-token": self.access_token})
         return process_response(response)
```

### Comparing `kodexa-6.1.4/kodexa/platform/kodexa.py` & `kodexa-6.2.25104807008/kodexa/platform/kodexa.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,30 +30,33 @@
 from kodexa.platform.client import DocumentStoreEndpoint, KodexaClient
 
 logger = logging.getLogger()
 
 dirs = AppDirs("Kodexa", "Kodexa")
 
 
-def get_config():
+def get_config(profile=None):
     """Get the kodexa config object we use when you want to store your PAT locally
 
     :return: the config as a dict
 
     Args:
 
     Returns:
 
     """
     path = os.path.join(dirs.user_config_dir, '.kodexa.json')
     if os.path.exists(path):
         with open(path, 'r') as outfile:
-            return json.load(outfile)
+            kodexa_config = json.load(outfile)
+            if profile and profile not in kodexa_config:
+                kodexa_config[profile] = {'url': None, 'access_token': None}
+            return kodexa_config
     else:
-        return {'url': None, 'access_token': None}
+        return {'url': None, 'access_token': None} if not profile else {profile: {'url': None, 'access_token': None}}
 
 
 def save_config(config_obj):
     """Saves the configuration dictionary for the user
 
     Args:
       config_obj: return:
@@ -240,42 +243,43 @@
 
     @staticmethod
     def get_client():
         from kodexa import KodexaClient
         return KodexaClient(KodexaPlatform.get_url(), KodexaPlatform.get_access_token())
 
     @staticmethod
-    def get_access_token() -> str:
+    def get_access_token(profile=None) -> str:
         """
         Returns the access token
 
         >>> access_token = KodexaPlatform.get_access_token()
 
         Returns: The access token if it is defined in the user config store, or as an environment variable
 
         """
-        kodexa_config = get_config()
+        kodexa_config = get_config(profile)
         access_token = os.getenv('KODEXA_ACCESS_TOKEN')
-        return access_token if access_token is not None else kodexa_config['access_token']
+        return access_token if access_token is not None else \
+            kodexa_config[profile]['access_token'] if profile else kodexa_config['access_token']
 
     @staticmethod
-    def get_url() -> str:
+    def get_url(profile=None) -> str:
         """
         Returns the URL to use to access a Kodexa Platform
 
         The URL should be in the form https://my-company.kodexa.ai
 
         >>> access_token = KodexaPlatform.get_url()
 
         Returns: The URL if it is defined in the user config store, or as an environment variable
 
         """
-        kodexa_config = get_config()
+        kodexa_config = get_config(profile)
         env_url = os.getenv('KODEXA_URL', None)
-        return env_url if env_url is not None else kodexa_config['url']
+        return env_url if env_url is not None else kodexa_config[profile]['url'] if profile else kodexa_config['url']
 
     @staticmethod
     def set_access_token(access_token: str):
         """
         Set to override the access token to use, not that this does not impact your user config stored
         value
 
@@ -332,23 +336,27 @@
 
         if len(ref.split('/')[1].split(":")) == 2:
             version = ref.split('/')[1].split(":")[1]
 
         return [org_slug, slug, version]
 
     @classmethod
-    def login(cls, kodexa_url, username, password):
+    def login(cls, kodexa_url, username, password, profile=None):
         from requests.auth import HTTPBasicAuth
         obj_response = requests.get(f"{kodexa_url}/api/account/me/token",
                                     auth=HTTPBasicAuth(username, password),
                                     headers={"content-type": "application/json"})
         if obj_response.status_code == 200:
-            kodexa_config = get_config()
-            kodexa_config['url'] = kodexa_url
-            kodexa_config['access_token'] = obj_response.text
+            kodexa_config = get_config(profile)
+            if profile and profile in kodexa_config:
+                kodexa_config[profile]['url'] = kodexa_url
+                kodexa_config[profile]['access_token'] = obj_response.text
+            else:
+                kodexa_config['url'] = kodexa_url
+                kodexa_config['access_token'] = obj_response.text
             save_config(kodexa_config)
             print("Logged in")
         else:
             print(f"Check your URL and password [{obj_response.status_code}]")
 
     @classmethod
     def get_server_info(cls):
```

### Comparing `kodexa-6.1.4/kodexa/selectors/ast.py` & `kodexa-6.2.25104807008/kodexa/selectors/ast.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.1.4/kodexa/selectors/core.py` & `kodexa-6.2.25104807008/kodexa/selectors/core.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.1.4/kodexa/selectors/lexrules.py` & `kodexa-6.2.25104807008/kodexa/selectors/lexrules.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.1.4/kodexa/selectors/lextab.py` & `kodexa-6.2.25104807008/kodexa/selectors/lextab.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.1.4/kodexa/selectors/parserules.py` & `kodexa-6.2.25104807008/kodexa/selectors/parserules.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.1.4/kodexa/selectors/parsetab.py` & `kodexa-6.2.25104807008/kodexa/selectors/parsetab.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.1.4/kodexa/spatial/azure_models.py` & `kodexa-6.2.25104807008/kodexa/spatial/azure_models.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.1.4/kodexa/spatial/bbox_common.py` & `kodexa-6.2.25104807008/kodexa/spatial/bbox_common.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.1.4/kodexa/spatial/table_form_common.py` & `kodexa-6.2.25104807008/kodexa/spatial/table_form_common.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.1.4/kodexa/steps/common.py` & `kodexa-6.2.25104807008/kodexa/steps/common.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.1.4/kodexa/testing/test_components.py` & `kodexa-6.2.25104807008/kodexa/testing/test_components.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.1.4/kodexa/testing/test_utils.py` & `kodexa-6.2.25104807008/kodexa/testing/test_utils.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.1.4/pyproject.toml` & `kodexa-6.2.25104807008/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kodexa"
-version = "6.1.4"
+version = "6.2.25104807008"
 description = "Python SDK for the Kodexa Platform"
 authors = ["Austin Redenbaugh <austin@kodexa.com>", "Philip Dodds <philip@kodexa.com>", "Romar Cablao <rcablao@kodexa.com>", "Amadea Paula Dodds <amadeapaula@kodexa.com>"]
 readme = "README.md"
 
 packages = [
     { include = "kodexa" }
 ]
```

### Comparing `kodexa-6.1.4/setup.py` & `kodexa-6.2.25104807008/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -33,17 +33,17 @@
  'pyyaml>=6.0,<7.0',
  'requests>=2.28.1,<3.0.0',
  'simpleeval==0.9.12',
  'urllib3>=1.26.14,<2.0.0']
 
 setup_kwargs = {
     'name': 'kodexa',
-    'version': '6.1.4',
+    'version': '6.2.25104807008',
     'description': 'Python SDK for the Kodexa Platform',
-    'long_description': '# Kodexa\n\n[![Build and Package with Poetry](https://github.com/kodexa-ai/kodexa/actions/workflows/main.yml/badge.svg?branch=main)](https://github.com/kodexa-ai/kodexa/actions/workflows/main.yml)\n\n![img.png](https://docs.kodexa.com/img.png)\n\nKodexa is a platform for building intelligent document processing pipelines. It is a set of tools and services that\nallow you to build a pipeline that can take a document, extract the content, and then process it to extract the\ninformation you need.\n\nIt is built on a set of core principles:\n\n* **Document Centric** - Kodexa is built around the idea of a document. A document is a collection of content\n  nodes that are connected together. This is a powerful model that allows you to build pipelines that can\n  extract content from a wide range of sources.\n\n* **Pipeline Oriented** - Kodexa is built around the idea of a pipeline. A pipeline is a series of steps that\n  can be executed on a document. This allows you to build a pipeline that can extract content from a wide range\n  of sources.\n\n* **Extensible** - Kodexa is built around the idea of a pipeline. A pipeline is a series of steps that can be executed\n  on a document. This allows you to build a pipeline that can extract content from a wide range of sources.\n\n* **Label Driven** - Kodexa focuses on the idea of labels. Labels are a way to identify content within a document\n  and then use that content to drive the processing of the document.\n\n# Python SDK\n\nThis repository contains the Python SDK for Kodexa. The SDK is the primary way to interact with Kodexa. It allows you to\ndefine actions, models, and pipelines that can be executed on Kodexa. It also includes a complete SDK client for\nworking with a Kodexa platform instance.\n\n## Documentation & Examples\n\nDocumentation is available at the [Kodexa Documentation Portal](https://docs.kodexa.com)\n\n## Current Development\n\nThe main branch is 6.0 which is a production release.\n\n## Set-up\n\nWe use poetry to manage our dependencies, so you can install them with:\n\n    poetry install\n\nYou can then run the tests with:\n\n    poetry run pytest\n\n# Contributing\n\nWe welcome contributions to the Kodexa platform. Please see our [contributing guide](CONTRIBUTING.md) for more details.\n\n# License\n\nApache 2.0\n',
+    'long_description': '# Kodexa\n\n[![Build and Package with Poetry](https://github.com/kodexa-ai/kodexa/actions/workflows/main.yml/badge.svg?branch=main)](https://github.com/kodexa-ai/kodexa/actions/workflows/main.yml)\n\n![img.png](https://docs.kodexa.com/img.png)\n\nKodexa is a platform for building intelligent document processing pipelines. It is a set of tools and services that\nallow you to build a pipeline that can take a document, extract the content, and then process it to extract the\ninformation you need.\n\nIt is built on a set of core principles:\n\n* **Document Centric** - Kodexa is built around the idea of a document. A document is a collection of content\n  nodes that are connected together. This is a powerful model that allows you to build pipelines that can\n  extract content from a wide range of sources.\n\n* **Pipeline Oriented** - Kodexa is built around the idea of a pipeline. A pipeline is a series of steps that\n  can be executed on a document. This allows you to build a pipeline that can extract content from a wide range\n  of sources.\n\n* **Extensible** - Kodexa is built around the idea of a pipeline. A pipeline is a series of steps that can be executed\n  on a document. This allows you to build a pipeline that can extract content from a wide range of sources.\n\n* **Label Driven** - Kodexa focuses on the idea of labels. Labels are a way to identify content within a document\n  and then use that content to drive the processing of the document.\n\n# Python SDK\n\nThis repository contains the Python SDK for Kodexa. The SDK is the primary way to interact with Kodexa. It allows you to\ndefine actions, models, and pipelines that can be executed on Kodexa. It also includes a complete SDK client for\nworking with a Kodexa platform instance.\n\n## Documentation & Examples\n\nDocumentation is available at the [Kodexa Documentation Portal](https://docs.kodexa.com)\n\n## Current Development\n\n[//]: # (Replace it with the diagrams and descriptions for build releases)\n**BUILD VERSION FLOW**\n![build-version-flow.png](docs%2Fbuild-version-flow.png)\nBuild version will differ based on the branches that are published to pypi.\n\n**GITHUB PROCESS**\n![github-process.png](docs%2Fgithub-process.png)\nChanges that contain bugs, features, and fixes should first be pushed to the test branch. \nOnce these changes are thoroughly tested, they can be submitted as a pull request to the main branch. The pull request should be reviewed and approved by an appropriate person before the changes can be merged.\n\n## Set-up\n\nWe use poetry to manage our dependencies, so you can install them with:\n\n    poetry install\n\nYou can then run the tests with:\n\n    poetry run pytest\n\n# Contributing\n\nWe welcome contributions to the Kodexa platform. Please see our [contributing guide](CONTRIBUTING.md) for more details.\n\n# License\n\nApache 2.0\n\n',
     'author': 'Austin Redenbaugh',
     'author_email': 'austin@kodexa.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `kodexa-6.1.4/PKG-INFO` & `kodexa-6.2.25104807008/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kodexa
-Version: 6.1.4
+Version: 6.2.25104807008
 Summary: Python SDK for the Kodexa Platform
 Author: Austin Redenbaugh
 Author-email: austin@kodexa.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
@@ -66,15 +66,23 @@
 
 ## Documentation & Examples
 
 Documentation is available at the [Kodexa Documentation Portal](https://docs.kodexa.com)
 
 ## Current Development
 
-The main branch is 6.0 which is a production release.
+[//]: # (Replace it with the diagrams and descriptions for build releases)
+**BUILD VERSION FLOW**
+![build-version-flow.png](docs%2Fbuild-version-flow.png)
+Build version will differ based on the branches that are published to pypi.
+
+**GITHUB PROCESS**
+![github-process.png](docs%2Fgithub-process.png)
+Changes that contain bugs, features, and fixes should first be pushed to the test branch. 
+Once these changes are thoroughly tested, they can be submitted as a pull request to the main branch. The pull request should be reviewed and approved by an appropriate person before the changes can be merged.
 
 ## Set-up
 
 We use poetry to manage our dependencies, so you can install them with:
 
     poetry install
 
@@ -86,7 +94,8 @@
 
 We welcome contributions to the Kodexa platform. Please see our [contributing guide](CONTRIBUTING.md) for more details.
 
 # License
 
 Apache 2.0
 
+
```

