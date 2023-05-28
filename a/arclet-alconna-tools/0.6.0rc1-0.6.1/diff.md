# Comparing `tmp/arclet-alconna-tools-0.6.0rc1.tar.gz` & `tmp/arclet-alconna-tools-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arclet-alconna-tools-0.6.0rc1.tar", last modified: Mon May  8 16:36:19 2023, max compression
+gzip compressed data, was "arclet-alconna-tools-0.6.1.tar", last modified: Sun May 28 14:06:35 2023, max compression
```

## Comparing `arclet-alconna-tools-0.6.0rc1.tar` & `arclet-alconna-tools-0.6.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1091 2022-01-24 11:14:57.524000 arclet-alconna-tools-0.6.0rc1/LICENSE
--rw-r--r--   0        0        0     1081 2023-05-08 16:35:08.337284 arclet-alconna-tools-0.6.0rc1/pyproject.toml
--rw-r--r--   0        0        0       53 2022-09-16 06:41:48.807371 arclet-alconna-tools-0.6.0rc1/README.md
--rw-r--r--   0        0        0      391 2023-05-08 11:53:03.576121 arclet-alconna-tools-0.6.0rc1/src/arclet/alconna/tools/__init__.py
--rw-r--r--   0        0        0     2355 2023-05-08 11:53:03.567259 arclet-alconna-tools-0.6.0rc1/src/arclet/alconna/tools/actions.py
--rw-r--r--   0        0        0      866 2023-05-07 05:15:13.324038 arclet-alconna-tools-0.6.0rc1/src/arclet/alconna/tools/checker.py
--rw-r--r--   0        0        0       96 2023-05-08 11:53:03.585160 arclet-alconna-tools-0.6.0rc1/src/arclet/alconna/tools/config.py
--rw-r--r--   0        0        0    27100 2023-05-08 15:07:41.119518 arclet-alconna-tools-0.6.0rc1/src/arclet/alconna/tools/construct.py
--rw-r--r--   0        0        0     3879 2023-05-07 05:15:13.335037 arclet-alconna-tools-0.6.0rc1/src/arclet/alconna/tools/debug.py
--rw-r--r--   0        0        0    17495 2023-05-08 16:19:03.896293 arclet-alconna-tools-0.6.0rc1/src/arclet/alconna/tools/formatter.py
--rw-r--r--   0        0        0       26 2023-05-08 11:44:10.335552 arclet-alconna-tools-0.6.0rc1/src/arclet/alconna/tools/i18n/.config.json
--rw-r--r--   0        0        0      692 2023-05-08 16:08:05.985424 arclet-alconna-tools-0.6.0rc1/src/arclet/alconna/tools/i18n/en-US.json
--rw-r--r--   0        0        0      661 2023-05-08 16:18:05.842731 arclet-alconna-tools-0.6.0rc1/src/arclet/alconna/tools/i18n/zh-CN.json
--rw-r--r--   0        0        0     4453 2023-05-07 05:35:56.817434 arclet-alconna-tools-0.6.0rc1/src/arclet/alconna/tools/pattern.py
--rw-r--r--   0        0        0      280 1970-01-01 00:00:00.000000 arclet-alconna-tools-0.6.0rc1/PKG-INFO
+-rw-r--r--   0        0        0     1091 2022-01-24 11:14:57.524000 arclet-alconna-tools-0.6.1/LICENSE
+-rw-r--r--   0        0        0     1075 2023-05-28 13:57:51.253672 arclet-alconna-tools-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0      749 2023-05-10 16:28:11.249182 arclet-alconna-tools-0.6.1/README.md
+-rw-r--r--   0        0        0      387 2023-05-10 14:13:40.054086 arclet-alconna-tools-0.6.1/src/arclet/alconna/tools/__init__.py
+-rw-r--r--   0        0        0     2355 2023-05-08 11:53:03.567259 arclet-alconna-tools-0.6.1/src/arclet/alconna/tools/actions.py
+-rw-r--r--   0        0        0      866 2023-05-07 05:15:13.324038 arclet-alconna-tools-0.6.1/src/arclet/alconna/tools/checker.py
+-rw-r--r--   0        0        0       96 2023-05-08 11:53:03.585160 arclet-alconna-tools-0.6.1/src/arclet/alconna/tools/config.py
+-rw-r--r--   0        0        0    30725 2023-05-28 13:55:54.267542 arclet-alconna-tools-0.6.1/src/arclet/alconna/tools/construct.py
+-rw-r--r--   0        0        0     3879 2023-05-07 05:15:13.335037 arclet-alconna-tools-0.6.1/src/arclet/alconna/tools/debug.py
+-rw-r--r--   0        0        0    17620 2023-05-10 14:36:13.901208 arclet-alconna-tools-0.6.1/src/arclet/alconna/tools/formatter.py
+-rw-r--r--   0        0        0       26 2023-05-08 11:44:10.335552 arclet-alconna-tools-0.6.1/src/arclet/alconna/tools/i18n/.config.json
+-rw-r--r--   0        0        0      692 2023-05-08 16:08:05.985424 arclet-alconna-tools-0.6.1/src/arclet/alconna/tools/i18n/en-US.json
+-rw-r--r--   0        0        0      661 2023-05-08 16:18:05.842731 arclet-alconna-tools-0.6.1/src/arclet/alconna/tools/i18n/zh-CN.json
+-rw-r--r--   0        0        0     4453 2023-05-07 05:35:56.817434 arclet-alconna-tools-0.6.1/src/arclet/alconna/tools/pattern.py
+-rw-r--r--   0        0        0      939 1970-01-01 00:00:00.000000 arclet-alconna-tools-0.6.1/PKG-INFO
```

### Comparing `arclet-alconna-tools-0.6.0rc1/LICENSE` & `arclet-alconna-tools-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `arclet-alconna-tools-0.6.0rc1/pyproject.toml` & `arclet-alconna-tools-0.6.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [project]
 name = "arclet-alconna-tools"
-version = "0.6.0rc1"
+version = "0.6.1"
 description = "Builtin Tools for Alconna"
 authors = [
     { name = "RF-Tar-Railt", email = "rf_tar_railt@qq.com" },
 ]
 dependencies = [
-    "nepattern<0.6.0, >=0.5.0",
-    "arclet-alconna>=1.7.0rc6",
+    "nepattern<0.6.0, >=0.5.8",
+    "arclet-alconna>=1.7.7",
 ]
 requires-python = ">=3.8"
 readme = "README.md"
 
 [project.license]
 text = "MIT"
```

### Comparing `arclet-alconna-tools-0.6.0rc1/src/arclet/alconna/tools/actions.py` & `arclet-alconna-tools-0.6.1/src/arclet/alconna/tools/actions.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-tools-0.6.0rc1/src/arclet/alconna/tools/checker.py` & `arclet-alconna-tools-0.6.1/src/arclet/alconna/tools/checker.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-tools-0.6.0rc1/src/arclet/alconna/tools/construct.py` & `arclet-alconna-tools-0.6.1/src/arclet/alconna/tools/construct.py`

 * *Files 4% similar despite different names*

```diff
@@ -425,14 +425,20 @@
         for p in re.findall(r"\[(.+?)]", _others):
             res = re.split("[:=]", p)
             res[0] = f"{res[0]};?"
             arg.append(res)
         return arg
 
     def __init__(self, command: str, help_text: Optional[str] = None):
+        """创建 AlconnaString
+
+        Args:
+            command (str): 命令字符串, 例如 `test <message:str:hello> #HELP_STRING`
+            help_text (Optional[str], optional): 选填的命令的帮助文本.
+        """
         self.buffer = {}
         self.options = []
         self.meta = CommandMeta(description=help_text, fuzzy_match=True)
         head, others = split_once(command, (" ",))
         if mat := re.match(r"^\[(.+?)]$", head):
             self.buffer["prefixes"] = mat[1].split("|")
         else:
@@ -440,14 +446,22 @@
         args = self.args_gen(others)
         if help_string := re.findall(r"(?: )#(.+)$", others):  # noqa
             self.meta.description = help_string[0]
         custom_types = getattr(inspect.getmodule(inspect.stack()[1][0]), "__dict__", {})
         self.buffer["main_args"] = args_from_list(args, custom_types.copy())
 
     def option(self, name: str, opt: Optional[str] = None, default: Any = None, action: Optional[Action] = None):
+        """添加一个选项
+
+        Args:
+            name (str): 选项的实际名称
+            opt (Optional[str], optional): 选项的字符串, 例如 `--foo -f <val:bool>`.
+            default (Any, optional): 选项的默认值.
+            action (Optional[Action], optional): 选项的动作.
+        """
         if opt is None:
             self.options.append(
                 Option(name, default=default, action=action)
             )
             return self
         parts = split(opt, (" ",))
         aliases = []
@@ -468,22 +482,25 @@
             opt = Option("|".join(aliases), _args, dest=name, default=default, action=action, help_text=help_text)
         else:
             opt = Option(name, _args, default=default, action=action, help_text=help_text)
         self.options.append(opt)
         return self
 
     def usage(self, content: str):
+        """设置命令的使用方法"""
         self.meta.usage = content
         return self
 
     def example(self, content: str):
+        """设置命令的使用示例"""
         self.meta.example = content
         return self
 
     def build(self):
+        """构造为 Alconna 对象"""
         return Alconna(*self.buffer.values(), *self.options, meta=self.meta)
 
 class MountConfig(TypedDict):
     prefixes: NotRequired[List[str]]
     raise_exception: NotRequired[bool]
     description: NotRequired[str]
     # get_subcommand: NotRequired[bool]
@@ -517,27 +534,89 @@
     elif config := inspect.getmembers(
         obj, lambda x: inspect.isclass(x) and x.__name__.endswith("Config")
     ):
         config = config[0][1]
         result = {k: getattr(config, k) for k in config_keys if k in dir(config)}
     return result
 
+
 @dataclass(unsafe_hash=True)
 class CallbackHandler(ArparmaBehavior):
     main_call: Optional[Callable] = field(default=None)
     options: Dict[str, Callable] = field(default_factory=dict, hash=False)
 
     def operate(self, interface: Arparma):
-        self.before_operate(interface)
         if call := self.main_call:
             call(**interface.main_args)
         for path, action in self.options.items():
-            if d := interface.query(path, None):
+            if (d := interface.query(path, None)) is not None:
                 action(**d)
 
+
+class SubClassMounter(Subcommand):
+
+    def _get_instance(self):
+        return self.instance
+
+    def _inject_instance(self, target: Callable):
+        @wraps(target)
+        def wrapper(*args, **kwargs):
+            return target(self._get_instance(), *args, **kwargs)
+
+        return wrapper
+
+    def __init__(self, mount_cls: Type, upper_handler: CallbackHandler, upper_path: str):
+        self.mount_cls = mount_cls
+        self.instance: mount_cls = None
+        config = visit_config(mount_cls)
+        members = inspect.getmembers(
+            mount_cls, lambda x: inspect.isfunction(x) or inspect.ismethod(x)
+        )
+
+        _options = []
+        main_help_text = (
+            mount_cls.__doc__ or mount_cls.__init__.__doc__ or mount_cls.__name__
+        )
+
+        main_args = Args.from_callable(mount_cls.__init__)[0]
+
+        def _main_func(**kwargs):
+            if self.instance is None:
+                self.instance = mount_cls(**kwargs)
+                for key, value in kwargs.items():
+                    self.args[key].field.default = value
+            else:
+                for k, v in kwargs.items():
+                    setattr(self.instance, k, v)
+        path = f"subcommands.{upper_path}.{mount_cls.__name__}" if upper_path else f"subcommands.{mount_cls.__name__}"
+        upper_handler.options[f"{path}.args"] = _main_func
+        for name, func in filter(lambda x: not x[0].startswith("_"), members):
+            help_text = func.__doc__ or name
+            _opt_args, method = Args.from_callable(func)
+            if method:
+                func = self._inject_instance(func)
+            _options.append(
+                Option(name, _opt_args, help_text=help_text)
+            )
+            upper_handler.options[f"{path}.options.{name}.args"] = func
+
+        _options.extend(
+            SubClassMounter(cls, upper_handler, path)
+            for name, cls in inspect.getmembers(mount_cls, inspect.isclass)
+            if not name.startswith("_") and not name.endswith("Config")
+        )
+
+        super().__init__(
+            config.get("command", mount_cls.__name__),
+            main_args,
+            *_options,
+            help_text=config.get("description", main_help_text),
+        )
+
+
 class FuncMounter(Alconna):
     def __init__(
         self, func: Union[FunctionType, MethodType], config: Optional[MountConfig] = None
     ):
         config = config or visit_config(func)
         func_name = func.__name__
         if func_name.startswith("_"):
@@ -577,14 +656,19 @@
                 func = partial(func, func.__self__)
             _options.append(
                 Option(
                     name, args=_opt_args, help_text=help_text
                 )
             )
             behavior.options[f"options.{name}.args"] = func
+        _options.extend(
+            SubClassMounter(cls, behavior, "")
+            for name, cls in inspect.getmembers(module, inspect.isclass)
+            if not name.startswith("_") and not name.endswith("Config")
+        )
         super().__init__(
             config.get("command", module.__name__),
             config.get("headers", []),
             *_options,
             namespace=config.get("namespace", None),
             meta=CommandMeta(
                 description=config.get(
@@ -639,14 +723,20 @@
             _opt_args, method = Args.from_callable(func)
             if method:
                 func = self._inject_instance(func)
             _options.append(
                 Option(name, _opt_args, help_text=help_text)
             )
             behavior.options[f"options.{name}.args"] = func
+
+        _options.extend(
+            SubClassMounter(cls, behavior, "")
+            for name, cls in inspect.getmembers(mount_cls, inspect.isclass)
+            if not name.startswith("_") and not name.endswith("Config")
+        )
         super().__init__(
             config.get("command", mount_cls.__name__),
             main_args,
             config.get("headers", []),
             *_options,
             namespace=config.get("namespace", None),
             meta=CommandMeta(
@@ -680,14 +770,20 @@
             _opt_args, _ = Args.from_callable(func)
             _options.append(
                 Option(
                     name, args=_opt_args, help_text=help_text
                 )
             )
             behavior.options[f"options.{name}.args"] = func
+
+        _options.extend(
+            SubClassMounter(cls, behavior, "")
+            for name, cls in inspect.getmembers(obj, inspect.isclass)
+            if not name.startswith("_")
+        )
         main_args = Args.from_callable(obj.__init__)[0]
         for arg in main_args.argument:
             if hasattr(self.instance, arg.name):
                 arg.field.default = getattr(self.instance, arg.name)
 
         super().__init__(
             config.get("command", obj_name),
```

### Comparing `arclet-alconna-tools-0.6.0rc1/src/arclet/alconna/tools/debug.py` & `arclet-alconna-tools-0.6.1/src/arclet/alconna/tools/debug.py`

 * *Files identical despite different names*

### Comparing `arclet-alconna-tools-0.6.0rc1/src/arclet/alconna/tools/formatter.py` & `arclet-alconna-tools-0.6.1/src/arclet/alconna/tools/formatter.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,42 +1,43 @@
 from typing import List, Dict, Any, Union, Tuple, Optional
-from nepattern import Empty, AllParam
+from nepattern import Empty, AllParam, AnyOne, AnyString
 from tarina import lang
 from arclet.alconna.args import Args, Arg
 from arclet.alconna.base import Subcommand, Option
 from arclet.alconna.formatter import TextFormatter, Trace
 
 
-class ArgParserTextFormatter(TextFormatter):
+class ShellTextFormatter(TextFormatter):
     """
-    argparser 风格的帮助文本格式化器
+    shell 风格的帮助文本格式化器
     """
 
     def format(self, trace: Trace) -> str:
         parts = trace.body  # type: ignore
         sub_names = [i.name for i in filter(lambda x: isinstance(x, Subcommand), parts)]
         opt_names = [min(i.aliases, key=len) for i in filter(lambda x: isinstance(x, Option), parts)]
         sub_names = f"{{{','.join(sub_names)}}}" if sub_names else ""
         opt_names = (" ".join(f"[{i}]" for i in opt_names)) if opt_names else ""
         topic = f"{lang.require('tools', 'format.ap.title')}: {trace.head['name']} {opt_names}\n {sub_names}"
         header = self.header(trace.head, trace.separators)
         param = self.parameters(trace.args)
         body = self.body(parts)
-        return f"{topic}\n{header % (param, body)}"
+        return header % (topic, param, body)
 
     def param(self, parameter: Arg) -> str:
         name = parameter.name
         if str(parameter.value).strip("'\"") == name:
             return f"[{name}]" if parameter.optional else name
         if parameter.hidden:
             return f"[{name.upper()}]" if parameter.optional else name.upper()
         if parameter.value is AllParam:
             return f"{name.upper()}..."
         arg = f"[{name.upper()}" if parameter.optional else name.upper()
-        arg += f":{parameter.value}"
+        if parameter.value not in (AnyOne, AnyString):
+            arg += f":{parameter.value}"
         if parameter.field.display is Empty:
             arg += "=None"
         elif parameter.field.display is not None:
             arg += f"={parameter.field.display}"
         return f"{arg}]" if parameter.optional else arg
 
     def parameters(self, args: Args) -> str:
@@ -46,30 +47,30 @@
                 continue
             if len(arg.separators) == 1:
                 sep = ' ' if arg.separators[0] == ' ' else f' {arg.separators[0]!r} '
             else:
                 sep = f"[{'|'.join(arg.separators)!r}]"
             res += self.param(arg) + sep
         notice = [(arg.name, arg.notice) for arg in args.argument if arg.notice]
-        return f"{res}\n  {lang.require('tools', 'format.ap.notice')}:\n  " + \
-            "\n  ".join(f"{v[0]}: {v[1]}" for v in notice) if notice else res
+        return f"{res}\n{lang.require('tools', 'format.ap.notice')}:\n  - " + \
+            "\n  - ".join(f"{v[0]}: {v[1]}" for v in notice) if notice else res
 
     def header(self, root: Dict[str, Any], separators: Tuple[str, ...]) -> str:
-        help_string = f"\n{lang.require('tools', 'format.ap.desc')}: {desc}\n" if (desc := root.get("description")) else ""
+        help_string = f"{desc}\n" if (desc := root.get("description")) else ""
         usage = f"\n{lang.require('tools', 'format.ap.usage')}: {usage}\n" if (usage := root.get("usage")) else ""
         example = f"\n{lang.require('tools', 'format.ap.example')}: {example}\n" if (example := root.get("example")) else ""
         header_text = (
             f"[{''.join(map(str, headers))}]"
             if (headers := root.get("header", [])) and headers != [""]
             else ""
         )
         cmd = f"{header_text}{root.get('name', '')}"
         sep = separators[0]
         command_string = (cmd or root["name"]) + sep
-        return f"\n{command_string}%s{help_string}{usage}\n%s{example}"
+        return f"{help_string}\n%s\n\n{command_string}%s{usage}\n%s{example}"
 
     def body(self, parts: List[Union[Option, Subcommand]]) -> str:
         options = []
         opt_description = []
         max_len = 1
         for opt in filter(
             lambda x: isinstance(x, Option) and (x.name not in self.ignore_names or not x.nargs), parts
@@ -150,15 +151,16 @@
         if str(parameter.value).strip("'\"") == name:
             return f"&#91;{name}&#93;" if parameter.optional else name
         if parameter.hidden:
             return f"&#91;{name}&#93;" if parameter.optional else f"&lt;{name}&gt;"
         if parameter.value is AllParam:
             return f"&lt;...{name}&gt;"
         arg = f"&#91;{name}" if parameter.optional else f"&lt;{name}"
-        arg += f": {parameter.value}"
+        if parameter.value not in (AnyOne, AnyString):
+            arg += f": {parameter.value}"
         if parameter.field.display is Empty:
             arg += " = None"
         elif parameter.field.display is not None:
             arg += f" = {parameter.field.display}"
         return f"{arg}&#93;" if parameter.optional else f"{arg}&gt;"
 
     def parameters(self, args: Args) -> Tuple[str, Optional[List[str]]]:
@@ -270,26 +272,27 @@
         sub_names = self._convert(f"{{{','.join(sub_names)}}}\n", "info") if sub_names else ""
         opt_names = self._convert((" ".join(f"[{i}]" for i in opt_names)), 'info') if opt_names else ""
         title = f"{lang.require('tools', 'format.ap.title')}:"
         topic = f"{self._convert(title, 'warn')} {self._convert(trace.head['name'], 'msg')} {opt_names}\n {sub_names}"
         header = self.header(trace.head, trace.separators)
         param = self._convert(self.parameters(trace.args), "success")
         body = self.body(parts)
-        return f"{topic}{header % (param, body)}"
+        return header % (topic, param, body)
 
     def param(self, parameter: Arg) -> str:
         name = parameter.name
         if str(parameter.value).strip("'\"") == name:
             return f"[{name}]" if parameter.optional else name
         if parameter.hidden:
             return f"[{name.upper()}]" if parameter.optional else name.upper()
         if parameter.value is AllParam:
             return f"{name.upper()}..."
         arg = f"[{name.upper()}" if parameter.optional else name.upper()
-        arg += f":{parameter.value}"
+        if parameter.value not in (AnyOne, AnyString):
+            arg += f":{parameter.value}"
         if parameter.field.display is Empty:
             arg += "=None"
         elif parameter.field.display is not None:
             arg += f"={parameter.field.display}"
         return f"{arg}]" if parameter.optional else arg
 
     def parameters(self, args: Args) -> str:
@@ -299,34 +302,34 @@
                 continue
             if len(arg.separators) == 1:
                 sep = ' ' if arg.separators[0] == ' ' else f' {arg.separators[0]!r} '
             else:
                 sep = f"[{'|'.join(arg.separators)!r}]"
             res += self.param(arg) + sep
         notice = [(arg.name, arg.notice) for arg in args.argument if arg.notice]
-        return f"{res}\n  {lang.require('tools', 'format.ap.notice')}:\n  " + \
-            "\n  ".join(f"{v[0]}: {v[1]}" for v in notice) if notice else res
+        _not = self._convert(f"{lang.require('tools', 'format.ap.notice')}:", 'warn')
+        return f"{res}\n{_not}\n  - " + \
+            "\n  - ".join(self._convert(f"{v[0]}: {v[1]}", "success") for v in notice) if notice else res
 
 
     def header(self, root: Dict[str, Any], separators: Tuple[str, ...]) -> str:
-        _desc = f"{lang.require('tools', 'format.ap.desc')}:"
         _usage = f"{lang.require('tools', 'format.ap.usage')}:"
         _example = f"{lang.require('tools', 'format.ap.example')}:"
-        help_string = f"\n{self._convert(_desc, 'warn')} {desc}\n" if (desc := root.get("description")) else ""
+        help_string = f"{desc}\n" if (desc := root.get("description")) else ""
         usage = f"\n{self._convert(_usage, 'warn')} {usage}\n" if (usage := root.get("usage")) else ""
         example = f"\n{self._convert(_example, 'warn')} {example}\n" if (example := root.get("example")) else ""
         header_text = (
             f"[{''.join(map(str, headers))}]"
             if (headers := root.get("header", [])) and headers != [""]
             else ""
         )
         cmd = f"{header_text}{root.get('name', '')}"
         sep = separators[0]
-        command_string = self._convert((cmd or root["name"]) + sep, "success")
-        return f"\n{command_string}%s{help_string}{usage}\n%s{example}"
+        command_string = self._convert((cmd or root["name"]) + sep, "msg")
+        return f"{help_string}\n%s\n\n{command_string}%s{usage}\n%s{example}"
 
     def body(self, parts: List[Union[Option, Subcommand]]) -> str:
         options = []
         opt_description = []
         max_len = 1
         for opt in filter(
             lambda x: isinstance(x, Option) and (x.name not in self.ignore_names or not x.nargs), parts
```

### Comparing `arclet-alconna-tools-0.6.0rc1/src/arclet/alconna/tools/i18n/en-US.json` & `arclet-alconna-tools-0.6.1/src/arclet/alconna/tools/i18n/en-US.json`

 * *Files identical despite different names*

### Comparing `arclet-alconna-tools-0.6.0rc1/src/arclet/alconna/tools/i18n/zh-CN.json` & `arclet-alconna-tools-0.6.1/src/arclet/alconna/tools/i18n/zh-CN.json`

 * *Files identical despite different names*

### Comparing `arclet-alconna-tools-0.6.0rc1/src/arclet/alconna/tools/pattern.py` & `arclet-alconna-tools-0.6.1/src/arclet/alconna/tools/pattern.py`

 * *Files identical despite different names*

