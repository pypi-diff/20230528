# Comparing `tmp/dash-cytoscape-elements-0.0.2.tar.gz` & `tmp/dash-cytoscape-elements-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dash-cytoscape-elements-0.0.2.tar", max compression
+gzip compressed data, was "dash-cytoscape-elements-0.0.3.tar", max compression
```

## Comparing `dash-cytoscape-elements-0.0.2.tar` & `dash-cytoscape-elements-0.0.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1065 2023-01-09 07:08:52.909508 dash-cytoscape-elements-0.0.2/LICENSE
--rw-r--r--   0        0        0     4754 2023-01-26 07:40:08.793126 dash-cytoscape-elements-0.0.2/README.md
--rw-r--r--   0        0        0      221 2023-01-26 07:57:19.665712 dash-cytoscape-elements-0.0.2/dash_cytoscape_elements/__init__.py
--rw-r--r--   0        0        0     4659 2023-01-26 07:55:38.206865 dash-cytoscape-elements-0.0.2/dash_cytoscape_elements/element.py
--rw-r--r--   0        0        0    10570 2023-01-26 07:55:38.207305 dash-cytoscape-elements-0.0.2/dash_cytoscape_elements/elements.py
--rw-r--r--   0        0        0      665 2023-01-26 07:57:35.174474 dash-cytoscape-elements-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     5636 2023-01-26 08:01:48.403030 dash-cytoscape-elements-0.0.2/setup.py
--rw-r--r--   0        0        0     5487 2023-01-26 08:01:48.403479 dash-cytoscape-elements-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-05-02 15:51:58.105390 dash-cytoscape-elements-0.0.3/LICENSE
+-rw-r--r--   0        0        0     4754 2023-05-02 15:51:58.105768 dash-cytoscape-elements-0.0.3/README.md
+-rw-r--r--   0        0        0      221 2023-05-28 16:52:24.311252 dash-cytoscape-elements-0.0.3/dash_cytoscape_elements/__init__.py
+-rw-r--r--   0        0        0     4973 2023-05-28 16:33:47.805861 dash-cytoscape-elements-0.0.3/dash_cytoscape_elements/element.py
+-rw-r--r--   0        0        0    10692 2023-05-08 15:59:42.716960 dash-cytoscape-elements-0.0.3/dash_cytoscape_elements/elements.py
+-rw-r--r--   0        0        0      665 2023-05-28 16:52:45.826138 dash-cytoscape-elements-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     5636 2023-05-28 16:56:05.860914 dash-cytoscape-elements-0.0.3/setup.py
+-rw-r--r--   0        0        0     5487 2023-05-28 16:56:05.861328 dash-cytoscape-elements-0.0.3/PKG-INFO
```

### Comparing `dash-cytoscape-elements-0.0.2/LICENSE` & `dash-cytoscape-elements-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dash-cytoscape-elements-0.0.2/README.md` & `dash-cytoscape-elements-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `dash-cytoscape-elements-0.0.2/dash_cytoscape_elements/element.py` & `dash-cytoscape-elements-0.0.3/dash_cytoscape_elements/element.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,16 +8,26 @@
 
 class BaseElement(BaseModel):
     class Config:
         validate_assignment: bool = True
         allow_population_by_field_name: bool = True
         extra: str = "forbid"
 
+    def __getattr__(self, value: str) -> Any:
+        for k, v in vars(self).items():
+            if isinstance(v, BaseElement):
+                result = v.__getattribute__(value)
+                if result:
+                    return result
+            elif k == value:
+                return v
+        return None
+
     def is_match_attribute(self, key: str, value: Any) -> bool:
-        if hasattr(self, key):
+        if key in vars(self):
             if isinstance(getattr(self, key), List):
                 if isinstance(value, List):
                     return set(getattr(self, key)) >= set(value)
                 else:
                     return value in getattr(self, key)
             elif isinstance(getattr(self, key), Set):
                 if isinstance(value, Set):
@@ -34,15 +44,15 @@
         else:
             for v in self.__dict__.values():
                 if isinstance(v, BaseElement):
                     return v.is_match_attribute(key, value)
             return False
 
     def add_attribute(self, key: str, value: Any):
-        if hasattr(self, key):
+        if key in vars(self):
             if isinstance(getattr(self, key), List):
                 if isinstance(value, List):
                     for v in value:
                         if not (v in getattr(self, key)):
                             getattr(self, key).append(v)
                 else:
                     if not (value in getattr(self, key)):
```

### Comparing `dash-cytoscape-elements-0.0.2/dash_cytoscape_elements/elements.py` & `dash-cytoscape-elements-0.0.3/dash_cytoscape_elements/elements.py`

 * *Files 16% similar despite different names*

```diff
@@ -163,20 +163,18 @@
                 elements._append(e)
         return elements
 
     def get(self, **kwargs: Any) -> Union[NodeT, EdgeT, None]:
         """Get the Element(`element.Node`/`element.Edge`) object
          in the `GenericElements` matching the `kwargs`.
 
-        Must specify the values that uniquely identify the Element in the `kwargs`.
-        The others parameters are ignored.
+        Get first element if matching multiple elements.
 
         Args:
-            **kwargs (Any): the values of `GenericElements.node_keys`
-             or `GenericElements.edge_keys`
+            **kwargs (Any): each class variables in the Element(`element.Node`/`element.Edge`)
 
         Returns:
             Union[element.Node, element.Edge, None]: no comment
 
         Examples:
             >>> e = Elements()
             >>> e.add(id="node1")
@@ -191,36 +189,26 @@
             >>>
             >>> print(e.get(source="node1", target="node2"))
             Edge(id="edge1")
             >>>
             >>> print(e.get(id="node3"))
             None
         """
-        if kwargs.keys() >= self.node_keys:
-            key_dict = {k: kwargs[k] for k in self.node_keys}
-            for e in self.filter(group="nodes"):
-                if e.is_match(**key_dict):
-                    return e
-
-        if kwargs.keys() >= self.edge_keys:
-            key_dict = {k: kwargs[k] for k in self.edge_keys}
-            for e in self.filter(group="edges"):
-                if e.is_match(**key_dict):
-                    return e
-
+        for e in self.filter(**kwargs):
+            return e
         return None
 
     def add(self, **kwargs: Any) -> None:
         """Add the Element(`element.Node`/`element.Edge`) object to the `GenericElements`.
 
         If exist `source` and `target` in `kwargs`, add the `element.Edge`.
         Otherwise add the `element.Node`.
 
         Args:
-            **kwargs (Any): each class variables in `element`
+            **kwargs (Any): each class variables in the Element(`element.Node`/`element.Edge`)
 
         Returns:
             None: no comment
 
         Examples:
             >>> e = Elements()
             >>> e.add(id="node1", classes="test", label="node1_label")
@@ -251,15 +239,21 @@
 
         Note:
             * UUID is assigned if not exist `id` in the `kwargs`.
             * If already exist Element, update the Element(`element.Node`/`element.Edge`) parameters.
                 * List/Dict/Set and `classes`: append value
                 * The others Type: replace value
         """
-        element = self.get(**kwargs)
+        element = None
+        if kwargs.keys() >= self.edge_keys:
+            key_dict = {k: kwargs[k] for k in self.edge_keys}
+            element = self.get(**key_dict)
+        elif kwargs.keys() >= self.node_keys:
+            key_dict = {k: kwargs[k] for k in self.node_keys}
+            element = self.get(**key_dict)
 
         if element:
             if "id" in kwargs:
                 for e in self.filter(id=kwargs["id"]):
                     if e != element:
                         return
             element.add(**kwargs)
@@ -305,13 +299,20 @@
             >>> print(e)
             [Node(id="node2"), Edge(id="edge1"), Edge(id="edge2")]
             >>>
             >>> e.remove(id="node3")
             >>> print(e)
             [Node(id="node2"), Edge(id="edge1"), Edge(id="edge2")]
         """
-        element = self.get(**kwargs)
+        element = None
+        if kwargs.keys() >= self.edge_keys:
+            key_dict = {k: kwargs[k] for k in self.edge_keys}
+            element = self.get(**key_dict)
+        elif kwargs.keys() >= self.node_keys:
+            key_dict = {k: kwargs[k] for k in self.node_keys}
+            element = self.get(**key_dict)
+
         if element:
             self._remove(element)
 
 
 Elements: TypeAlias = GenericElements[Node, Edge]
```

### Comparing `dash-cytoscape-elements-0.0.2/pyproject.toml` & `dash-cytoscape-elements-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dash-cytoscape-elements"
-version = "0.0.2"
+version = "0.0.3"
 description = "Python object for dash-cytoscape elements"
 authors = ["minefuto <minefuto@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/minefuto/dash-cytoscape-elements"
 
 [tool.poetry.dependencies]
```

### Comparing `dash-cytoscape-elements-0.0.2/setup.py` & `dash-cytoscape-elements-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['pydantic>=1.10.4,<2.0.0']
 
 setup_kwargs = {
     'name': 'dash-cytoscape-elements',
-    'version': '0.0.2',
+    'version': '0.0.3',
     'description': 'Python object for dash-cytoscape elements',
     'long_description': '# dash-cytoscape-elements\n[![test](https://github.com/minefuto/dash-cytoscape-elements/actions/workflows/test.yml/badge.svg)](https://github.com/minefuto/dash-cytoscape-elements/actions/workflows/test.yml)\n![PyPI - Python Version](https://img.shields.io/pypi/pyversions/dash-cytoscape-elements)\n![PyPI](https://img.shields.io/pypi/v/dash-cytoscape-elements)\n![GitHub](https://img.shields.io/github/license/minefuto/dash-cytoscape-elements)\n\nThis is a Python object for [Dash Cytoscape](https://github.com/plotly/dash-cytoscape) Elements.\n\n## Features\n- Add/Remove/Get/Filter Element(Node/Edge) on Python object.\n- Convert Python object from/to Dash Cytoscape format \n- Convert Python object from/to json(Cytoscape.js format)\n\n## Install\n```\npip install dash-cytoscape-elements\n```\n\n## Usage\n### Example1\nCreate Elements object & using on Dash Cytoscape  \n```python\nimport dash\nimport dash_cytoscape as cyto\nfrom dash import html\nfrom dash_cytoscape_elements import Elements\n\ne = Elements()\ne.add(id="one", label="Node 1", x=50, y=50)\ne.add(id="two", label="Node 2", x=200, y=200)\ne.add(source="one", target="two", label="Node 1 to 2")\n\napp = dash.Dash(__name__)\napp.layout = html.Div([\n    cyto.Cytoscape(\n        id=\'cytoscape\',\n        elements=e.to_dash(),\n        layout={\'name\': \'preset\'}\n    )\n])\n\nif __name__ == \'__main__\':\n    app.run_server(debug=True)\n```\n### Example2\nEdit json file of Elements.\n```python\nfrom dash_cytoscape_elements import Elements\n\ne = Elements.from_file("elements.json")\ne.remove(id="node2")\ne.remove(source="node1", target="node2")\n\nwith open("elements.json", mode=\'w\') as f:\n    f.write(e.to_json())\n```\n### Supported Parameters\nThis package supports the following parameters of [Dash Cytoscape](https://github.com/plotly/dash-cytoscape) Element.  \n\n| Parameter | Type | Element |\n| --------- | ---- | ------- |\n| id |  str | Node, Edge |\n| parent | str | Node |\n| source | str | Edge |\n| target | str | Edge |\n| label | str | Node, Edge |\n| source_label | str | Edge |\n| target_label | str | Edge |\n| x | float | Node |\n| y | float | Node |\n| classes | str | Node, Edge |\n| selected | str | Node, Edge |\n| selectable | str | Node, Edge |\n| locked | str | Node, Edge |\n| grabbable | str | Node, Edge |\n| pannable | str | Node, Edge |\n| scratch | dict | Node, Edge |\n\nexample output:\n```python\n>>> e = Elements()\n>>> e.add(id="node1", parent="parent1", label="node_label1", x=1, y=1, classes="class1")\n>>> e.add(source="node1", target="node2", label="edge_label1", source_label="source_label1", target_label="target_label1", classes="class1")\n>>> print(e.to_json())\n[\n    {\n        "group": "nodes",\n        "classes": "class1",\n        "data": {\n            "id": "node1",\n            "parent": "parent1",\n            "label": "node_label1"\n        },\n        "position": {\n            "x": 1.0,\n            "y": 1.0\n        }\n    },\n    {\n        "group": "edges",\n        "classes": "class1",\n        "data": {\n            "id": "49082bcd-dcbb-4db7-b369-29e3bf8f74e2",\n            "source": "node1",\n            "target": "node2",\n            "label": "edge_label1",\n            "source-label": "source_label1",\n            "target-label": "target_label1"\n        }\n    }\n]\n```\nHow to add your own parameters:\n```python\nfrom typing import List, Set\nfrom dash_cytoscape_elements import GenericElements\nfrom dash_cytoscape_elements.element import Edge, EdgeData, Node, NodeData\n\n\nclass CustomNodeData(NodeData):\n    custom_str1: str = ""\n\nclass CustomNode(Node):\n    data: CustomNodeData = CustomNodeData()\n    custom_str2: str = ""\n    custom_list: List[str] = []\n\nclass CustomEdgeData(EdgeData):\n    custom_str1: str = ""\n\nclass CustomEdge(Edge):\n    data: CustomEdgeData = CustomEdgeData()\n    custom_str2: str = ""\n    custom_set: Set[str] = set()\n\ne = GenericElements[CustomNode, CustomEdge]()\ne.add(id="node1", custom_str1="str1", custom_str2="str2", custom_list=["list1", "list2"])\ne.add(id="edge1", source="node1", target="node2", custom_str1="str1", custom_str2="str2", custom_set={"set1", "set2"})\n\nprint(e.to_json())\n# [\n#     {\n#         "group": "nodes",\n#         "data": {\n#             "id": "node1",\n#             "custom_str1": "str1"\n#         },\n#         "custom_str2": "str2",\n#         "custom_list": [\n#             "list1",\n#             "list2"\n#         ]\n#     },\n#     {\n#         "group": "edges",\n#         "data": {\n#             "id": "edge1",\n#             "source": "node1",\n#             "target": "node2",\n#             "custom_str1": "str1"\n#         },\n#         "custom_str2": "str2",\n#         "custom_set": [\n#             "set1",\n#             "set2"\n#         ]\n#     }\n# ]\n```\n\nPlease see the [Documentation](https://minefuto.github.io/dash-cytoscape-elements/) for details.\n',
     'author': 'minefuto',
     'author_email': 'minefuto@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/minefuto/dash-cytoscape-elements',
```

### Comparing `dash-cytoscape-elements-0.0.2/PKG-INFO` & `dash-cytoscape-elements-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dash-cytoscape-elements
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python object for dash-cytoscape elements
 Home-page: https://github.com/minefuto/dash-cytoscape-elements
 License: MIT
 Author: minefuto
 Author-email: minefuto@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

