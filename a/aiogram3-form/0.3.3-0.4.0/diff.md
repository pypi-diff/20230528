# Comparing `tmp/aiogram3_form-0.3.3.tar.gz` & `tmp/aiogram3_form-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiogram3_form-0.3.3.tar", max compression
+gzip compressed data, was "aiogram3_form-0.4.0.tar", max compression
```

## Comparing `aiogram3_form-0.3.3.tar` & `aiogram3_form-0.4.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      294 2023-01-24 13:28:23.727234 aiogram3_form-0.3.3/aiogram3_form/__init__.py
--rw-r--r--   0        0        0     1383 2023-04-13 18:33:34.599104 aiogram3_form-0.3.3/aiogram3_form/field.py
--rw-r--r--   0        0        0      843 2023-01-24 00:46:35.276915 aiogram3_form-0.3.3/aiogram3_form/filters.py
--rw-r--r--   0        0        0     8478 2023-05-12 16:54:10.262129 aiogram3_form-0.3.3/aiogram3_form/form.py
--rw-r--r--   0        0        0      120 2023-01-24 00:23:37.244911 aiogram3_form-0.3.3/aiogram3_form/state.py
--rw-r--r--   0        0        0     1092 2023-01-24 00:20:12.265098 aiogram3_form-0.3.3/LICENSE
--rw-r--r--   0        0        0      520 2023-05-12 16:53:32.939025 aiogram3_form-0.3.3/pyproject.toml
--rw-r--r--   0        0        0     1479 2023-01-24 00:20:12.265098 aiogram3_form-0.3.3/README.md
--rw-r--r--   0        0        0     2025 1970-01-01 00:00:00.000000 aiogram3_form-0.3.3/setup.py
--rw-r--r--   0        0        0     1973 1970-01-01 00:00:00.000000 aiogram3_form-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0      294 2023-01-24 13:28:23.727234 aiogram3_form-0.4.0/aiogram3_form/__init__.py
+-rw-r--r--   0        0        0     1383 2023-04-13 18:33:34.599104 aiogram3_form-0.4.0/aiogram3_form/field.py
+-rw-r--r--   0        0        0      843 2023-01-24 00:46:35.276915 aiogram3_form-0.4.0/aiogram3_form/filters.py
+-rw-r--r--   0        0        0     8589 2023-05-28 18:45:46.654147 aiogram3_form-0.4.0/aiogram3_form/form.py
+-rw-r--r--   0        0        0      120 2023-01-24 00:23:37.244911 aiogram3_form-0.4.0/aiogram3_form/state.py
+-rw-r--r--   0        0        0     1092 2023-01-24 00:20:12.265098 aiogram3_form-0.4.0/LICENSE
+-rw-r--r--   0        0        0      520 2023-05-28 19:04:54.931946 aiogram3_form-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     1479 2023-01-24 00:20:12.265098 aiogram3_form-0.4.0/README.md
+-rw-r--r--   0        0        0     2025 1970-01-01 00:00:00.000000 aiogram3_form-0.4.0/setup.py
+-rw-r--r--   0        0        0     1973 1970-01-01 00:00:00.000000 aiogram3_form-0.4.0/PKG-INFO
```

### Comparing `aiogram3_form-0.3.3/aiogram3_form/field.py` & `aiogram3_form-0.4.0/aiogram3_form/field.py`

 * *Files identical despite different names*

### Comparing `aiogram3_form-0.3.3/aiogram3_form/filters.py` & `aiogram3_form-0.4.0/aiogram3_form/filters.py`

 * *Files identical despite different names*

### Comparing `aiogram3_form-0.3.3/aiogram3_form/form.py` & `aiogram3_form-0.4.0/aiogram3_form/form.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import functools
 import inspect
 from abc import ABC, ABCMeta
-from typing import Any, Callable, ClassVar, Optional, Set, Type, Union
+from typing import Any, Callable, ClassVar, Dict, Optional, Set, Type, Union
 
 from aiogram import Bot, types
 from aiogram.dispatcher.router import Router
 from aiogram.fsm.context import FSMContext
 from aiogram.utils.magic_filter import MagicFilter
 
 from . import filters
@@ -15,60 +15,59 @@
 SubmitCallback = Callable[..., Any]
 Markup = Union[types.ReplyKeyboardMarkup, types.InlineKeyboardMarkup]
 
 REMOVE_MARKUP = types.ReplyKeyboardRemove(remove_keyboard=True)
 
 
 class FormMeta(ABCMeta):
-    bot: ClassVar[Bot]
     router: ClassVar[Router]
     clear_state_on_submit: ClassVar[bool] = True
 
     __form_cls_names: Set[str] = set()
 
     def __new__(
         cls,
         cls_name: str,
         parents: tuple,
         cls_dict: dict,
         *,
         router: Router,
-        bot: Bot,
         clear_state_on_submit: bool = True,
     ):
         if cls_name in cls.__form_cls_names:
             raise NameError("Form with the same name does exist")
 
         cls.__form_cls_names.add(cls_name)
 
         cls_dict["clear_state_on_submit"] = clear_state_on_submit
         cls_dict["router"] = router
-        cls_dict["bot"] = bot
 
         return super().__new__(cls, cls_name, parents, cls_dict)
 
 
-class Form(ABC, metaclass=FormMeta, router=None, bot=None):  # type: ignore
-    __registered_forms: Set[Type["Form"]] = set()
+class Form(ABC, metaclass=FormMeta, router=None):  # type: ignore
+    __registered_forms: Set[str] = set()
     __submit_callback: Optional[SubmitCallback] = None
 
-    def __init__(self, state: FSMContext):
-        self.state = state
+    def __init__(self, bot: Bot, chat_id: int):
+        self.bot = bot
+        self.chat_id = chat_id
 
     @classmethod
     def submit(cls):
         def decorator(submit_callback: SubmitCallback):
             cls.__submit_callback = submit_callback
 
         return decorator
 
     @classmethod
-    async def __from_state(cls, state: FSMContext):
-        state_data = await state.get_data()
-        form_object = cls(state)
+    async def __create_object(
+        cls, handler_data: dict[str, Any], state_data: Dict[str, Any]
+    ):
+        form_object = cls(handler_data["event_chat"].id, handler_data["bot"])
         form_object.__dict__.update(state_data["__form_values"])
         return form_object
 
     @classmethod
     def __get_filter_from_type(cls, field_type: Type):
         field_filter = filters.DEFAULT_FORM_FILTERS.get(field_type)
 
@@ -118,17 +117,16 @@
 
         try:
             next_field_name = field_names[current_field_index + 1]
             return cls.__get_field_data_by_name(next_field_name)
         except IndexError:
             return None
 
-    # TODO: method to send enter message
     @classmethod
-    async def start(cls, state_ctx: FSMContext):
+    async def start(cls, bot: Bot, state_ctx: FSMContext):
         first_field = cls.__get_next_field(None)
 
         if first_field is None:
             raise TypeError("First field couldn't be None")
 
         await state_ctx.set_state(FormState.waiting_field_value)
 
@@ -139,30 +137,30 @@
         )
 
         if first_field.info.enter_callback:
             await first_field.info.enter_callback(
                 state_ctx.key.chat_id, state_ctx.key.user_id, {}
             )
         else:
-            await cls.bot.send_message(
+            await bot.send_message(
                 state_ctx.key.chat_id,
                 first_field.info.enter_message_text,  # type: ignore
                 reply_markup=first_field.info.reply_markup or REMOVE_MARKUP,  # type: ignore
             )
 
         if cls in Form.__registered_forms:
             return
 
         cls.router.message.register(
             cls.__resolve_callback,
             FormState.waiting_field_value,
             cls.__current_field_filter,
         )
 
-        Form.__registered_forms.add(cls)
+        Form.__registered_forms.add(cls.__name__)
 
     @classmethod
     async def __resolve_callback(
         cls, message: types.Message, state: FSMContext, value: Any, **data
     ):
         state_data = await state.get_data()
         current_field_name: str = state_data["__current_field_name"]
@@ -186,15 +184,15 @@
             )
 
         if not cls.__submit_callback:
             raise TypeError(
                 f"{cls.__name__} submit callback is {cls.__submit_callback}"
             )
 
-        form_object = await cls.__from_state(state)
+        form_object = await cls.__create_object(data, state_data)
         data["state"] = state
 
         prepared_submit_callback = cls.__prepare_submit_callback(form_object, **data)
 
         try:
             await prepared_submit_callback()
         finally:
@@ -252,11 +250,15 @@
         reply_markup: Union[
             types.InlineKeyboardMarkup,
             types.ReplyKeyboardMarkup,
             types.ReplyKeyboardRemove,
             types.ForceReply,
             None,
         ] = None,
+        reply_to_message_id: Optional[int] = None,
     ):
-        await self.__class__.bot.send_message(
-            self.state.key.chat_id, text=text, reply_markup=reply_markup
+        return await self.bot.send_message(
+            self.chat_id,
+            text=text,
+            reply_markup=reply_markup,
+            reply_to_message_id=reply_to_message_id,
         )
```

### Comparing `aiogram3_form-0.3.3/LICENSE` & `aiogram3_form-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aiogram3_form-0.3.3/pyproject.toml` & `aiogram3_form-0.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aiogram3-form"
-version = "0.3.3"
+version = "0.4.0"
 description = "A library to create forms in aiogram3"
 authors = ["TrixiS <oficialmorozov@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "aiogram3_form"}]
 
 [tool.poetry.dependencies]
```

### Comparing `aiogram3_form-0.3.3/README.md` & `aiogram3_form-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `aiogram3_form-0.3.3/setup.py` & `aiogram3_form-0.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['aiogram3_form']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'aiogram3-form',
-    'version': '0.3.3',
+    'version': '0.4.0',
     'description': 'A library to create forms in aiogram3',
     'long_description': '# aiogram3-form\nA library to create forms in aiogram3\n\n# Example\n```Python\n# suppose you import here your router and bot objects\nfrom aiogram import F, types\n\nfrom aiogram3_form import Form, FormField\n\n\nclass NameForm(Form, router=your_router):\n    first_name: str = FormField(enter_message_text="Enter your first name please")\n    second_name: str = FormField(enter_message_text="Enter your second name please", filter=F.text.len() > 10)\n    age: int = FormField(enter_message_text="Enter age as integer", error_message_text="Age should be numeric!")\n\n\n@NameForm.submit()\nasync def name_form_submit_handler(form: NameForm, event_chat: types.Chat):\n    # handle form data\n    # also supports aiogram standart DI (e. g. middlewares, filters, etc)\n    await bot.send_message(\n        event_chat.id, f"Your full name is {form.first_name} {form.second_name}!"\n    )\n    \n    \n@router.message(F.text == "/form")\nasync def form_handler(message: types.Message, state: FSMContext):\n    await NameForm.start(state)  # start your form\n```\n\nAfter submit callback call the state would be automatically cleared.\n\nYou can control this state using the following metaclass kwarg\n\n```Python\n...\n\n\nclass NameForm(Form, clear_state_on_submit=False):  # True by default\n    ...\n\n\n@NameForm.submit()\nasync def name_form_submit_handler(form: NameForm, state: FSMContext):\n    # so you can set your exit state manually\n    await state.set_state(...)\n```\n',
     'author': 'TrixiS',
     'author_email': 'oficialmorozov@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `aiogram3_form-0.3.3/PKG-INFO` & `aiogram3_form-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiogram3-form
-Version: 0.3.3
+Version: 0.4.0
 Summary: A library to create forms in aiogram3
 License: MIT
 Author: TrixiS
 Author-email: oficialmorozov@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

