# Comparing `tmp/pytest_yaml_sanmu-0.2.1.dev1-py3-none-any.whl.zip` & `tmp/pytest_yaml_sanmu-0.2.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 7765 bytes, number of entries: 11
--rw-rw-rw-  2.0 fat        0 b- defN 16-Jan-01 00:00 pytest_yaml/__init__.py
--rw-rw-rw-  2.0 fat     1810 b- defN 16-Jan-01 00:00 pytest_yaml/_plugin.py
--rw-rw-rw-  2.0 fat     7288 b- defN 16-Jan-01 00:00 pytest_yaml/file.py
--rw-rw-rw-  2.0 fat      661 b- defN 16-Jan-01 00:00 pytest_yaml/hooks.py
--rw-rw-rw-  2.0 fat      886 b- defN 16-Jan-01 00:00 pytest_yaml/models.py
--rw-rw-rw-  2.0 fat     1110 b- defN 16-Jan-01 00:00 pytest_yaml/plugin.py
--rw-rw-rw-  2.0 fat     2435 b- defN 16-Jan-01 00:00 pytest_yaml/templates.py
-?rw-------  2.0 fat       36 b- defN 16-Jan-01 00:00 pytest_yaml_sanmu-0.2.1.dev1.dist-info/entry_points.txt
-?rw-------  2.0 fat       87 b- defN 16-Jan-01 00:00 pytest_yaml_sanmu-0.2.1.dev1.dist-info/WHEEL
-?rw-------  2.0 fat      551 b- defN 16-Jan-01 00:00 pytest_yaml_sanmu-0.2.1.dev1.dist-info/METADATA
-?rw-------  2.0 fat      904 b- defN 16-Jan-01 00:00 pytest_yaml_sanmu-0.2.1.dev1.dist-info/RECORD
-11 files, 15768 bytes uncompressed, 6225 bytes compressed:  60.5%
+Zip file size: 8192 bytes, number of entries: 11
+-rw-r--r--  2.0 unx        0 b- defN 16-Jan-01 00:00 pytest_yaml/__init__.py
+-rw-r--r--  2.0 unx     1810 b- defN 16-Jan-01 00:00 pytest_yaml/_plugin.py
+-rw-r--r--  2.0 unx     7039 b- defN 16-Jan-01 00:00 pytest_yaml/file.py
+-rw-r--r--  2.0 unx      661 b- defN 16-Jan-01 00:00 pytest_yaml/hooks.py
+-rw-r--r--  2.0 unx      868 b- defN 16-Jan-01 00:00 pytest_yaml/models.py
+-rw-r--r--  2.0 unx     1425 b- defN 16-Jan-01 00:00 pytest_yaml/plugin.py
+-rw-r--r--  2.0 unx     2350 b- defN 16-Jan-01 00:00 pytest_yaml/templates.py
+?rw-------  2.0 unx       36 b- defN 16-Jan-01 00:00 pytest_yaml_sanmu-0.2.2.dist-info/entry_points.txt
+?rw-------  2.0 unx       87 b- defN 16-Jan-01 00:00 pytest_yaml_sanmu-0.2.2.dist-info/WHEEL
+?rw-------  2.0 unx     1859 b- defN 16-Jan-01 00:00 pytest_yaml_sanmu-0.2.2.dist-info/METADATA
+?rw-------  2.0 unx      885 b- defN 16-Jan-01 00:00 pytest_yaml_sanmu-0.2.2.dist-info/RECORD
+11 files, 17020 bytes uncompressed, 6692 bytes compressed:  60.7%
```

## zipnote {}

```diff
@@ -15,20 +15,20 @@
 
 Filename: pytest_yaml/plugin.py
 Comment: 
 
 Filename: pytest_yaml/templates.py
 Comment: 
 
-Filename: pytest_yaml_sanmu-0.2.1.dev1.dist-info/entry_points.txt
+Filename: pytest_yaml_sanmu-0.2.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: pytest_yaml_sanmu-0.2.1.dev1.dist-info/WHEEL
+Filename: pytest_yaml_sanmu-0.2.2.dist-info/WHEEL
 Comment: 
 
-Filename: pytest_yaml_sanmu-0.2.1.dev1.dist-info/METADATA
+Filename: pytest_yaml_sanmu-0.2.2.dist-info/METADATA
 Comment: 
 
-Filename: pytest_yaml_sanmu-0.2.1.dev1.dist-info/RECORD
+Filename: pytest_yaml_sanmu-0.2.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pytest_yaml/file.py

 * *Ordering differences only*

```diff
@@ -1,249 +1,249 @@
-import itertools
-import logging
-from typing import Any, Iterable, Union
-
-import pytest
-import yaml
-
-from .models import Case
-from .templates import Template
-
-logger = logging.getLogger(__name__)
-
-
-class YamlFile(pytest.File):
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-
-        class FakeObj(object):
-            __doc__ = self.path
-
-        self.obj = FakeObj
-
-    def collect(self):
-        # 加载文件内容
-
-        for case_dict in yaml.safe_load_all(self.path.open(encoding="utf-8")):
-            case = Case.from_case_dict(case_dict)
-            yield from _case_to_yaml_item(case, self)
-
-
-class YamlItem(pytest.Function):
-    yaml_data: Case  # yaml数据内容
-    max_step_no: int  # 最大步骤数
-    current_step_no: int  # 当前步骤书
-    current_step: dict  # 当前步骤内容
-    usefixtures: dict  # fixtures
-
-    def __init__(self, *args, own_markers=None, **kwargs):
-        if own_markers and hasattr(self, "own_markers"):
-            self.own_markers.extend(own_markers)
-        super().__init__(*args, **kwargs)
-        self.usefixtures = dict()
-
-    @property
-    def cls(self):
-        return self.__class__
-
-    @property
-    def is_first_step(self):
-        if self.current_step_no == 0:
-            return True
-
-        return False
-
-    @property
-    def is_last_step(self):
-        if self.current_step_no >= self.max_step_no:
-            return True
-
-        return False
-
-    @property
-    def location(self):
-        location = self.reportinfo()
-        relfspath = self.session._node_location_to_relpath(self.path)
-
-        assert type(location[2]) is str
-        return relfspath, location[1], location[2]
-
-    @classmethod
-    def from_parent(cls, parent, name, case, marks, **kw):
-        own_markers = []
-
-        obj: YamlItem = super().from_parent(
-            parent,
-            name=name,
-            callobj=cls._call_obj,
-            own_markers=own_markers,
-            **kw,
-        )
-        obj.yaml_data = case
-        obj.max_step_no = len(case.steps) - 1
-
-        for mark in marks:
-            if isinstance(mark, str):
-                mark_name = mark
-                mark_args = []
-            elif isinstance(mark, dict):
-                mark_name = list(mark.keys())[0]
-                mark_args = list(mark.values())
-
-            if mark_name == "usefixtures":
-                fixture_name_list = mark[mark_name]
-                for fixture_name in fixture_name_list:
-                    obj.usefixtures.setdefault(fixture_name, "no set")
-            else:
-                mark_func = getattr(pytest.mark, mark_name)
-                mark_obj = mark_func(*mark_args)
-                own_markers.append(mark_obj)  # ???
-                obj.add_marker(mark_obj)
-        logger.debug(f"Generate new test: nodeid={obj.nodeid}, marks={marks} ")
-        return obj
-
-    @classmethod
-    def from_parent_parametrize(
-        cls, parent, name, case: Case, marks, parametrize_marks
-    ):
-        # logger.warning(f"{marks=}")
-        # logger.warning(f"{parametrize_marks=}")
-
-        arg_names = []
-        for i in parametrize_marks:
-            arg_names.extend(str_or_list(i["parametrize"]["keys"]))
-
-        arg_vals = []
-        for i in parametrize_marks:
-            vals = i["parametrize"]["vals"]
-            arg_vals.append(vals)
-
-        template_case: Case = case.copy()
-        template_case.mark = [m for m in case.mark if not is_parametrize(m)]
-        case_str = template_case.to_yaml()
-        # logger.warning(f"{case_str=}")
-
-        for vals in itertools.product(*arg_vals):
-            vals = list(get_value_by_sequence(*vals))
-            case_yaml = Template(case_str).safe_substitute(dict(zip(arg_names, vals)))
-            logger.debug(f"nwe case by parametrize :{case_yaml}")
-            new_case = Case.from_yaml(case_yaml)
-            new_case.test_name += str(list(vals))
-
-            yield YamlItem.from_parent(
-                parent,
-                case=new_case,
-                name=new_case.test_name,
-                marks=new_case.mark,
-            )
-
-    def _call_obj(self, request: pytest.FixtureRequest):
-        logger.debug(f"runrtest: {self.nodeid}")
-        for fixture_name in self.usefixtures:
-            logger.debug(f"request fixture: {fixture_name}")
-            fixture_value = request.getfixturevalue(fixture_name)
-            logger.debug(f"fixture value is: {fixture_value}")
-            self.usefixtures[fixture_name] = fixture_value
-
-        for i, step in enumerate(self.yaml_data.steps):
-            self.current_step_no = i
-            self.current_step = step
-            request.config.hook.pytest_yaml_run_step(
-                item=self,
-                request=request,
-            )
-
-    def runtest(self) -> None:
-        funcargs = self.funcargs
-        testargs = {arg: funcargs[arg] for arg in self._fixtureinfo.argnames}
-
-        self._call_obj(**testargs)
-
-    def repr_failure(self, excinfo):
-        style = self.config.getoption("tbstyle", "auto")
-        if style == "auto":
-            style = "value"
-
-        tb_info = excinfo.traceback[-1]
-        file_info = f"{tb_info.path}:{tb_info.lineno}: {excinfo.typename}"
-        err_info = f"{self._repr_failure_py(excinfo, style=style)}"
-
-        str_l = [
-            "",
-            file_info,
-            err_info,
-        ]
-        if getattr(self, "current_step_no", -1) >= 0:  # 步骤已经开始执行
-            str_l[0] = "Yaml Content: \n" + self.yaml_data.to_yaml()
-
-        # logger.warning(str_l[0])
-        return "\n".join(str_l)
-
-
-def _case_to_yaml_item(
-    case: Case, parent: YamlFile
-) -> Iterable[Union[pytest.Item, pytest.Collector]]:
-
-    parametrize_marks = []
-    other_marks = []
-
-    for mark in case.mark:
-        if is_parametrize(mark):
-            parametrize_marks.append(mark)
-        else:
-            other_marks.append(mark)
-
-    if parametrize_marks:
-        yield from YamlItem.from_parent_parametrize(
-            parent,
-            case=case,
-            name=case.test_name,
-            marks=other_marks,
-            parametrize_marks=parametrize_marks,
-        )
-    else:
-        yield YamlItem.from_parent(
-            parent,
-            case=case,
-            name=case.test_name,
-            marks=case.mark,
-        )
-
-
-def is_parametrize(mark):
-
-    if isinstance(mark, dict) and "parametrize" in mark:
-        return True
-    else:
-        return False
-
-
-def str_or_list(x: Union[str, list]) -> list:
-    if isinstance(x, list):
-        return x
-    else:
-        return [x]
-
-
-def list_or_nestlist(x: Union[list[Any], list[list]]) -> list[list]:
-
-    try:
-        _ = x[0][0]
-        return x
-    except TypeError:
-        return [x]
-
-
-def get_value_by_sequence(*args):
-    """
-
-    [["username, id"], "password"] ->  ["username, id", "password"]
-    [[1,9],[2,99],[3,999]]    -> [1,9,2,99,3,999]
-
-    :param args:
-    :return:
-    """
-    for arg in args:
-        if type(arg) in [list, tuple]:
-            yield from arg
-        else:
-            yield arg
+import itertools
+import logging
+from typing import Any, Iterable, Union
+
+import pytest
+import yaml
+
+from .models import Case
+from .templates import Template
+
+logger = logging.getLogger(__name__)
+
+
+class YamlFile(pytest.File):
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+
+        class FakeObj(object):
+            __doc__ = self.path
+
+        self.obj = FakeObj
+
+    def collect(self):
+        # 加载文件内容
+
+        for case_dict in yaml.safe_load_all(self.path.open(encoding="utf-8")):
+            case = Case.from_case_dict(case_dict)
+            yield from _case_to_yaml_item(case, self)
+
+
+class YamlItem(pytest.Function):
+    yaml_data: Case  # yaml数据内容
+    max_step_no: int  # 最大步骤数
+    current_step_no: int  # 当前步骤书
+    current_step: dict  # 当前步骤内容
+    usefixtures: dict  # fixtures
+
+    def __init__(self, *args, own_markers=None, **kwargs):
+        if own_markers and hasattr(self, "own_markers"):
+            self.own_markers.extend(own_markers)
+        super().__init__(*args, **kwargs)
+        self.usefixtures = dict()
+
+    @property
+    def cls(self):
+        return self.__class__
+
+    @property
+    def is_first_step(self):
+        if self.current_step_no == 0:
+            return True
+
+        return False
+
+    @property
+    def is_last_step(self):
+        if self.current_step_no >= self.max_step_no:
+            return True
+
+        return False
+
+    @property
+    def location(self):
+        location = self.reportinfo()
+        relfspath = self.session._node_location_to_relpath(self.path)
+
+        assert type(location[2]) is str
+        return relfspath, location[1], location[2]
+
+    @classmethod
+    def from_parent(cls, parent, name, case, marks, **kw):
+        own_markers = []
+
+        obj: YamlItem = super().from_parent(
+            parent,
+            name=name,
+            callobj=cls._call_obj,
+            own_markers=own_markers,
+            **kw,
+        )
+        obj.yaml_data = case
+        obj.max_step_no = len(case.steps) - 1
+
+        for mark in marks:
+            if isinstance(mark, str):
+                mark_name = mark
+                mark_args = []
+            elif isinstance(mark, dict):
+                mark_name = list(mark.keys())[0]
+                mark_args = list(mark.values())
+
+            if mark_name == "usefixtures":
+                fixture_name_list = mark[mark_name]
+                for fixture_name in fixture_name_list:
+                    obj.usefixtures.setdefault(fixture_name, "no set")
+            else:
+                mark_func = getattr(pytest.mark, mark_name)
+                mark_obj = mark_func(*mark_args)
+                own_markers.append(mark_obj)  # ???
+                obj.add_marker(mark_obj)
+        logger.debug(f"Generate new test: nodeid={obj.nodeid}, marks={marks} ")
+        return obj
+
+    @classmethod
+    def from_parent_parametrize(
+        cls, parent, name, case: Case, marks, parametrize_marks
+    ):
+        # logger.warning(f"{marks=}")
+        # logger.warning(f"{parametrize_marks=}")
+
+        arg_names = []
+        for i in parametrize_marks:
+            arg_names.extend(str_or_list(i["parametrize"]["keys"]))
+
+        arg_vals = []
+        for i in parametrize_marks:
+            vals = i["parametrize"]["vals"]
+            arg_vals.append(vals)
+
+        template_case: Case = case.copy()
+        template_case.mark = [m for m in case.mark if not is_parametrize(m)]
+        case_str = template_case.to_yaml()
+        # logger.warning(f"{case_str=}")
+
+        for vals in itertools.product(*arg_vals):
+            vals = list(get_value_by_sequence(*vals))
+            case_yaml = Template(case_str).safe_substitute(dict(zip(arg_names, vals)))
+            logger.debug(f"nwe case by parametrize :{case_yaml}")
+            new_case = Case.from_yaml(case_yaml)
+            new_case.test_name += str(list(vals))
+
+            yield YamlItem.from_parent(
+                parent,
+                case=new_case,
+                name=new_case.test_name,
+                marks=new_case.mark,
+            )
+
+    def _call_obj(self, request: pytest.FixtureRequest):
+        logger.debug(f"runrtest: {self.nodeid}")
+        for fixture_name in self.usefixtures:
+            logger.debug(f"request fixture: {fixture_name}")
+            fixture_value = request.getfixturevalue(fixture_name)
+            logger.debug(f"fixture value is: {fixture_value}")
+            self.usefixtures[fixture_name] = fixture_value
+
+        for i, step in enumerate(self.yaml_data.steps):
+            self.current_step_no = i
+            self.current_step = step
+            request.config.hook.pytest_yaml_run_step(
+                item=self,
+                request=request,
+            )
+
+    def runtest(self) -> None:
+        funcargs = self.funcargs
+        testargs = {arg: funcargs[arg] for arg in self._fixtureinfo.argnames}
+
+        self._call_obj(**testargs)
+
+    def repr_failure(self, excinfo):
+        style = self.config.getoption("tbstyle", "auto")
+        if style == "auto":
+            style = "value"
+
+        tb_info = excinfo.traceback[-1]
+        file_info = f"{tb_info.path}:{tb_info.lineno}: {excinfo.typename}"
+        err_info = f"{self._repr_failure_py(excinfo, style=style)}"
+
+        str_l = [
+            "",
+            file_info,
+            err_info,
+        ]
+        if getattr(self, "current_step_no", -1) >= 0:  # 步骤已经开始执行
+            str_l[0] = "Yaml Content: \n" + self.yaml_data.to_yaml()
+
+        # logger.warning(str_l[0])
+        return "\n".join(str_l)
+
+
+def _case_to_yaml_item(
+    case: Case, parent: YamlFile
+) -> Iterable[Union[pytest.Item, pytest.Collector]]:
+
+    parametrize_marks = []
+    other_marks = []
+
+    for mark in case.mark:
+        if is_parametrize(mark):
+            parametrize_marks.append(mark)
+        else:
+            other_marks.append(mark)
+
+    if parametrize_marks:
+        yield from YamlItem.from_parent_parametrize(
+            parent,
+            case=case,
+            name=case.test_name,
+            marks=other_marks,
+            parametrize_marks=parametrize_marks,
+        )
+    else:
+        yield YamlItem.from_parent(
+            parent,
+            case=case,
+            name=case.test_name,
+            marks=case.mark,
+        )
+
+
+def is_parametrize(mark):
+
+    if isinstance(mark, dict) and "parametrize" in mark:
+        return True
+    else:
+        return False
+
+
+def str_or_list(x: Union[str, list]) -> list:
+    if isinstance(x, list):
+        return x
+    else:
+        return [x]
+
+
+def list_or_nestlist(x: Union[list[Any], list[list]]) -> list[list]:
+
+    try:
+        _ = x[0][0]
+        return x
+    except TypeError:
+        return [x]
+
+
+def get_value_by_sequence(*args):
+    """
+
+    [["username, id"], "password"] ->  ["username, id", "password"]
+    [[1,9],[2,99],[3,999]]    -> [1,9,2,99,3,999]
+
+    :param args:
+    :return:
+    """
+    for arg in args:
+        if type(arg) in [list, tuple]:
+            yield from arg
+        else:
+            yield arg
```

## pytest_yaml/models.py

```diff
@@ -1,35 +1,35 @@
-from typing import List, Union
-
-import yaml
-from pydantic import BaseModel
-
-
-class Case(BaseModel):
-    test_name: str
-    steps: List[dict]
-    mark: List[Union[str, dict]] = []
-
-    @classmethod
-    def from_case_dict(cls, case_dict: dict):
-        """
-
-        :param case_dict: {'test_name': 'test a add b',
-                            'steps': [
-                                        {'a': 1, 'b': 2, 'assert': 3},
-                                        {'a': 2, 'b': 3, 'assert': 4}
-                                    ]
-                            }
-
-        :return:
-        """
-        # print(case_dict)
-
-        return cls(**case_dict)
-
-    def to_yaml(self):
-        return yaml.dump(self.dict(), allow_unicode=True)
-
-    @classmethod
-    def from_yaml(cls, yaml_str):
-        data = yaml.safe_load(yaml_str)
-        return cls(**data)
+from typing import List, Union
+
+import yaml
+from pydantic import BaseModel
+
+
+class Case(BaseModel):
+    test_name: str
+    steps: List[dict]
+    mark: List[Union[str, dict]] = []
+
+    @classmethod
+    def from_case_dict(cls, case_dict: dict):
+        """
+
+        :param case_dict: {'test_name': 'test a add b',
+                            'steps': [
+                                        {'a': 1, 'b': 2, 'assert': 3},
+                                        {'a': 2, 'b': 3, 'assert': 4}
+                                    ]
+                            }
+
+        :return:
+        """
+        # print(case_dict)
+
+        return cls(**case_dict)
+
+    def to_yaml(self):
+        return yaml.dump(self.dict(), allow_unicode=True, sort_keys=False)
+
+    @classmethod
+    def from_yaml(cls, yaml_str):
+        data = yaml.safe_load(yaml_str)
+        return cls(**data)
```

## pytest_yaml/plugin.py

```diff
@@ -1,39 +1,58 @@
-import inspect
-import logging
-from pathlib import Path
-
-import pytest
-
-from . import _plugin
-from .file import YamlFile
-
-# from pytest_yml.settings import settings
-
-logger = logging.getLogger(__name__)
-
-
-def pytest_addhooks(pluginmanager):
-    from . import hooks
-
-    pluginmanager.add_hookspecs(hooks)
-
-
-def pytest_configure(config: pytest.Config):
-    for plug, dist in config.pluginmanager.list_plugin_distinfo():
-        if plug.__name__ == "pytest_yaml.plugin":
-            dist.metadata = dist.metadata.json
-            dist.metadata["name"] = "pytest-yaml"
-
-    for klass_name, klass in inspect.getmembers(
-        _plugin,
-        lambda x: isinstance(x, type)
-        and issubclass(x, _plugin.YamlPlugin)
-        and x is not _plugin.YamlPlugin,
-    ):
-        config.pluginmanager.register(klass(config))
-
-
-def pytest_collect_file(parent, file_path: Path):
-    if file_path.suffix in [".yaml", ".yml"] and file_path.name.startswith("test"):
-        logger.debug(f"YamlFile: {file_path.absolute()}")
-        return YamlFile.from_parent(parent, path=file_path)
+import inspect
+import logging
+from pathlib import Path
+
+import pytest
+
+from . import _plugin
+from .file import YamlFile
+
+# from pytest_yml.settings import settings
+
+logger = logging.getLogger(__name__)
+enable_plugin = False
+
+
+def pytest_addhooks(pluginmanager):
+    from . import hooks
+
+    pluginmanager.add_hookspecs(hooks)
+
+
+def pytest_addoption(parser):
+    parser.addini(
+        "run_yaml_case",
+        type="bool",
+        default=False,
+        help="是否执行yaml测试用例",
+    )
+
+
+def pytest_configure(config: pytest.Config):
+    global enable_plugin
+    enable_plugin = config.getini("run_yaml_case")
+
+    if not enable_plugin:
+        return
+
+    for plug, dist in config.pluginmanager.list_plugin_distinfo():
+        if plug.__name__ == "pytest_yaml.plugin":
+            dist.metadata = dist.metadata.json
+            dist.metadata["name"] = "pytest-yaml"
+
+    for klass_name, klass in inspect.getmembers(
+        _plugin,
+        lambda x: isinstance(x, type)
+        and issubclass(x, _plugin.YamlPlugin)
+        and x is not _plugin.YamlPlugin,
+    ):
+        config.pluginmanager.register(klass(config))
+
+
+def pytest_collect_file(parent, file_path: Path):
+    if not enable_plugin:
+        return
+
+    if file_path.suffix in [".yaml", ".yml"] and file_path.name.startswith("test"):
+        logger.debug(f"YamlFile: {file_path.absolute()}")
+        return YamlFile.from_parent(parent, path=file_path)
```

### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

## pytest_yaml/templates.py

 * *Ordering differences only*

```diff
@@ -1,85 +1,85 @@
-"""
-@Filename:   commons/template
-@Author:      sanmu
-@Time:        2023/2/1 20:23
-@Describe:    ...
-"""
-import copy
-import logging
-import re
-import string
-
-logger = logging.getLogger(__name__)
-
-
-def _str(s) -> str:
-    return f"'{s}'"
-
-
-class Template(string.Template):
-    """
-    1. 支持函数调用
-    2. 参数也可以是变量
-    """
-
-    func_mapping = {
-        "str": _str,
-        "float": float,
-        "bool": bool,
-        "int": int,
-    }
-
-    call_pattern = re.compile(r"\${(?P<func_name>.*?)\((?P<func_args>.*?)\)}")
-
-    def render(self, mapping: dict) -> str:
-        s = self.safe_substitute(mapping)  # 原有方法替换变量
-        s = self.safe_substitute_funcs(s, mapping)  # 新方法替换函数结果
-
-        return s
-
-    def safe_substitute_funcs(self, template, mapping) -> str:
-        """
-        解析字符串中的函数名和参数，并将函数调用结果进行替换
-        :param template: 字符串
-        :param mapping: 上下文，提供要使用的函数和变量
-        :return: 替换后的结果
-        """
-
-        mapping = copy.deepcopy(mapping)
-        mapping.update(self.func_mapping)  # 合并两个mapping
-
-        def convert(mo):
-            func_name = mo.group("func_name")
-            func_args = mo.group("func_args").split(",")
-
-            func = mapping.get(func_name)  # 读取指定函数
-            func_args_value = [mapping.get(arg, arg) for arg in func_args]
-
-            if func_args_value == [""]:
-                func_args_value = []
-
-            if not callable(func):
-                return mo.group()  # 如果是不可调用的假函数,不进行替换
-            else:
-                return str(func(*func_args_value))  # 否则用函数结果进行替换
-
-        return self.call_pattern.sub(convert, template)
-
-
-def hot_load():
-    try:
-        import yaml_funcs
-
-        logger.info("load funcs by yaml_funcs")
-        for func_name in dir(yaml_funcs):  # 遍历模块中的所有函数
-            if func_name.startswith("_"):
-                continue
-
-            func_code = getattr(yaml_funcs, func_name)  # 取到了函数对象
-            if callable(func_code):  # 如果是一个可以调用的函数
-                Template.func_mapping[func_name] = func_code  # 函数放到Template中
-    except ImportError:
-        ...
-
-
-hot_load()
+"""
+@Filename:   commons/template
+@Author:      sanmu
+@Time:        2023/2/1 20:23
+@Describe:    ...
+"""
+import copy
+import logging
+import re
+import string
+
+logger = logging.getLogger(__name__)
+
+
+def _str(s) -> str:
+    return f"'{s}'"
+
+
+class Template(string.Template):
+    """
+    1. 支持函数调用
+    2. 参数也可以是变量
+    """
+
+    func_mapping = {
+        "str": _str,
+        "float": float,
+        "bool": bool,
+        "int": int,
+    }
+
+    call_pattern = re.compile(r"\${(?P<func_name>.*?)\((?P<func_args>.*?)\)}")
+
+    def render(self, mapping: dict) -> str:
+        s = self.safe_substitute(mapping)  # 原有方法替换变量
+        s = self.safe_substitute_funcs(s, mapping)  # 新方法替换函数结果
+
+        return s
+
+    def safe_substitute_funcs(self, template, mapping) -> str:
+        """
+        解析字符串中的函数名和参数，并将函数调用结果进行替换
+        :param template: 字符串
+        :param mapping: 上下文，提供要使用的函数和变量
+        :return: 替换后的结果
+        """
+
+        mapping = copy.deepcopy(mapping)
+        mapping.update(self.func_mapping)  # 合并两个mapping
+
+        def convert(mo):
+            func_name = mo.group("func_name")
+            func_args = mo.group("func_args").split(",")
+
+            func = mapping.get(func_name)  # 读取指定函数
+            func_args_value = [mapping.get(arg, arg) for arg in func_args]
+
+            if func_args_value == [""]:
+                func_args_value = []
+
+            if not callable(func):
+                return mo.group()  # 如果是不可调用的假函数,不进行替换
+            else:
+                return str(func(*func_args_value))  # 否则用函数结果进行替换
+
+        return self.call_pattern.sub(convert, template)
+
+
+def hot_load():
+    try:
+        import yaml_funcs
+
+        logger.info("load funcs by yaml_funcs")
+        for func_name in dir(yaml_funcs):  # 遍历模块中的所有函数
+            if func_name.startswith("_"):
+                continue
+
+            func_code = getattr(yaml_funcs, func_name)  # 取到了函数对象
+            if callable(func_code):  # 如果是一个可以调用的函数
+                Template.func_mapping[func_name] = func_code  # 函数放到Template中
+    except ImportError:
+        ...
+
+
+hot_load()
```

## Comparing `pytest_yaml_sanmu-0.2.1.dev1.dist-info/RECORD` & `pytest_yaml_sanmu-0.2.2.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 pytest_yaml/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 pytest_yaml/_plugin.py,sha256=QSTtELd_duC7uw0cKt8pfM67jonbzIlUMgYrdCD1_dE,1810
-pytest_yaml/file.py,sha256=n3oSq5qRoDIbzn9MeNz3ImPLsul1atcZa3E2RWmOfAA,7288
+pytest_yaml/file.py,sha256=YCm2hjOrcLhRUpnx7gIoiFJ-IPQM8ufMO2avf02m3EA,7039
 pytest_yaml/hooks.py,sha256=cclZKDIxTpWoRFZHqXzukmSwPjpmx8aH1iSWhs0Io8o,661
-pytest_yaml/models.py,sha256=WZcPE6l2LnJ-YfXZBiTCqhLL8ZccasNlh_lNXfj79mo,886
-pytest_yaml/plugin.py,sha256=qPo40NB7meaWQEXEvN6BBoDnGpk40Z9FrvRwsNl8ZdY,1110
-pytest_yaml/templates.py,sha256=HCDMLS82h-6hAw-w5zlEkeAqg8WatYPFdG1AvTt-TCk,2435
-pytest_yaml_sanmu-0.2.1.dev1.dist-info/entry_points.txt,sha256=pEQ-BthnhQfWoRegIMd3s8W8oR9tMHZz_soP_RAGXTs,36
-pytest_yaml_sanmu-0.2.1.dev1.dist-info/WHEEL,sha256=JtIceljpZF_3FlF7JEESqvYUELdenaIGNR7wSL2mRl0,87
-pytest_yaml_sanmu-0.2.1.dev1.dist-info/METADATA,sha256=eI_7dLZvo9XdLDjAc1B7D1GOPoxQ9j5cGTQiPqX1TIU,551
-pytest_yaml_sanmu-0.2.1.dev1.dist-info/RECORD,,
+pytest_yaml/models.py,sha256=2hBsq9K2XUYVjmJcykv8CvezdeXiMbLcGNIYl7OGanM,868
+pytest_yaml/plugin.py,sha256=Z69brEVc5wZVvFYMUfqd1iAUt_RmaBtHN8C1kLYzmwM,1425
+pytest_yaml/templates.py,sha256=eMxiigvnqC2p88S4cbzqodddXWKLgdmdTdvrJE2YUrs,2350
+pytest_yaml_sanmu-0.2.2.dist-info/entry_points.txt,sha256=pEQ-BthnhQfWoRegIMd3s8W8oR9tMHZz_soP_RAGXTs,36
+pytest_yaml_sanmu-0.2.2.dist-info/WHEEL,sha256=B19PGBCYhWaz2p_UjAoRVh767nYQfk14Sn4TpIZ-nfU,87
+pytest_yaml_sanmu-0.2.2.dist-info/METADATA,sha256=O5UdjneUix99VIQHVHn7-VRIVA0nTqPGkte-ZQ_uMd0,1859
+pytest_yaml_sanmu-0.2.2.dist-info/RECORD,,
```

