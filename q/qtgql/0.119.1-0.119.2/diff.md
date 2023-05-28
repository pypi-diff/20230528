# Comparing `tmp/qtgql-0.119.1.tar.gz` & `tmp/qtgql-0.119.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qtgql-0.119.1.tar", max compression
+gzip compressed data, was "qtgql-0.119.2.tar", max compression
```

## Comparing `qtgql-0.119.1.tar` & `qtgql-0.119.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1064 2023-05-24 15:09:49.035745 qtgql-0.119.1/LICENSE
--rw-r--r--   0        0        0     1805 2023-05-24 15:09:49.035745 qtgql-0.119.1/README.md
--rw-r--r--   0        0        0     4363 2023-05-24 15:10:06.287816 qtgql-0.119.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-24 15:09:49.051745 qtgql-0.119.1/qtgqlcodegen/__init__.py
--rw-r--r--   0        0        0     1866 2023-05-24 15:09:49.051745 qtgql-0.119.1/qtgqlcodegen/cli.py
--rw-r--r--   0        0        0        0 2023-05-24 15:09:49.051745 qtgql-0.119.1/qtgqlcodegen/compiler/__init__.py
--rw-r--r--   0        0        0     1761 2023-05-24 15:09:49.051745 qtgql-0.119.1/qtgqlcodegen/compiler/builtin_scalars.py
--rw-r--r--   0        0        0    11706 2023-05-24 15:09:49.051745 qtgql-0.119.1/qtgqlcodegen/compiler/operation.py
--rw-r--r--   0        0        0     3631 2023-05-24 15:09:49.051745 qtgql-0.119.1/qtgqlcodegen/compiler/template.py
--rw-r--r--   0        0        0     2065 2023-05-24 15:09:49.051745 qtgql-0.119.1/qtgqlcodegen/config.py
--rw-r--r--   0        0        0      413 2023-05-24 15:09:49.051745 qtgql-0.119.1/qtgqlcodegen/cppref.py
--rw-r--r--   0        0        0       41 2023-05-24 15:09:49.051745 qtgql-0.119.1/qtgqlcodegen/exceptions.py
--rw-r--r--   0        0        0     3187 2023-05-24 15:09:49.051745 qtgql-0.119.1/qtgqlcodegen/graphql_ref.py
--rw-r--r--   0        0        0    17696 2023-05-24 15:09:49.051745 qtgql-0.119.1/qtgqlcodegen/introspection.py
--rw-r--r--   0        0        0    10489 2023-05-24 15:09:49.051745 qtgql-0.119.1/qtgqlcodegen/objecttype.py
--rw-r--r--   0        0        0        0 2023-05-24 15:09:49.051745 qtgql-0.119.1/qtgqlcodegen/py.typed
--rw-r--r--   0        0        0        0 2023-05-24 15:09:49.051745 qtgql-0.119.1/qtgqlcodegen/runtime/__init__.py
--rw-r--r--   0        0        0     1566 2023-05-24 15:09:49.051745 qtgql-0.119.1/qtgqlcodegen/runtime/custom_scalars.py
--rw-r--r--   0        0        0      488 2023-05-24 15:09:49.051745 qtgql-0.119.1/qtgqlcodegen/templates/CMakeLists.jinja.cmake
--rw-r--r--   0        0        0      541 2023-05-24 15:09:49.051745 qtgql-0.119.1/qtgqlcodegen/templates/config.jinja.hpp
--rw-r--r--   0        0        0     2826 2023-05-24 15:09:49.051745 qtgql-0.119.1/qtgqlcodegen/templates/macros.jinja.hpp
--rw-r--r--   0        0        0     2869 2023-05-24 15:09:49.051745 qtgql-0.119.1/qtgqlcodegen/templates/operation.jinja.hpp
--rw-r--r--   0        0        0     2028 2023-05-24 15:09:49.051745 qtgql-0.119.1/qtgqlcodegen/templates/schema.jinja.hpp
--rw-r--r--   0        0        0     1028 2023-05-24 15:09:49.051745 qtgql-0.119.1/qtgqlcodegen/utils.py
--rw-r--r--   0        0        0     2800 1970-01-01 00:00:00.000000 qtgql-0.119.1/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-05-28 09:34:45.890799 qtgql-0.119.2/LICENSE
+-rw-r--r--   0        0        0     1805 2023-05-28 09:34:45.890799 qtgql-0.119.2/README.md
+-rw-r--r--   0        0        0     4363 2023-05-28 09:35:05.603632 qtgql-0.119.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-28 09:34:45.902799 qtgql-0.119.2/qtgqlcodegen/__init__.py
+-rw-r--r--   0        0        0     1866 2023-05-28 09:34:45.902799 qtgql-0.119.2/qtgqlcodegen/cli.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:34:45.902799 qtgql-0.119.2/qtgqlcodegen/compiler/__init__.py
+-rw-r--r--   0        0        0     1761 2023-05-28 09:34:45.902799 qtgql-0.119.2/qtgqlcodegen/compiler/builtin_scalars.py
+-rw-r--r--   0        0        0    11944 2023-05-28 09:34:45.902799 qtgql-0.119.2/qtgqlcodegen/compiler/operation.py
+-rw-r--r--   0        0        0     3631 2023-05-28 09:34:45.902799 qtgql-0.119.2/qtgqlcodegen/compiler/template.py
+-rw-r--r--   0        0        0     2065 2023-05-28 09:34:45.902799 qtgql-0.119.2/qtgqlcodegen/config.py
+-rw-r--r--   0        0        0      413 2023-05-28 09:34:45.902799 qtgql-0.119.2/qtgqlcodegen/cppref.py
+-rw-r--r--   0        0        0       41 2023-05-28 09:34:45.902799 qtgql-0.119.2/qtgqlcodegen/exceptions.py
+-rw-r--r--   0        0        0     3187 2023-05-28 09:34:45.902799 qtgql-0.119.2/qtgqlcodegen/graphql_ref.py
+-rw-r--r--   0        0        0    17696 2023-05-28 09:34:45.902799 qtgql-0.119.2/qtgqlcodegen/introspection.py
+-rw-r--r--   0        0        0    10492 2023-05-28 09:34:45.902799 qtgql-0.119.2/qtgqlcodegen/objecttype.py
+-rw-r--r--   0        0        0        0 2023-05-28 09:34:45.902799 qtgql-0.119.2/qtgqlcodegen/py.typed
+-rw-r--r--   0        0        0        0 2023-05-28 09:34:45.902799 qtgql-0.119.2/qtgqlcodegen/runtime/__init__.py
+-rw-r--r--   0        0        0     1566 2023-05-28 09:34:45.902799 qtgql-0.119.2/qtgqlcodegen/runtime/custom_scalars.py
+-rw-r--r--   0        0        0      488 2023-05-28 09:34:45.902799 qtgql-0.119.2/qtgqlcodegen/templates/CMakeLists.jinja.cmake
+-rw-r--r--   0        0        0      536 2023-05-28 09:34:45.902799 qtgql-0.119.2/qtgqlcodegen/templates/config.jinja.hpp
+-rw-r--r--   0        0        0     2855 2023-05-28 09:34:45.902799 qtgql-0.119.2/qtgqlcodegen/templates/macros.jinja.hpp
+-rw-r--r--   0        0        0     3257 2023-05-28 09:34:45.902799 qtgql-0.119.2/qtgqlcodegen/templates/operation.jinja.hpp
+-rw-r--r--   0        0        0     2034 2023-05-28 09:34:45.902799 qtgql-0.119.2/qtgqlcodegen/templates/schema.jinja.hpp
+-rw-r--r--   0        0        0     1028 2023-05-28 09:34:45.902799 qtgql-0.119.2/qtgqlcodegen/utils.py
+-rw-r--r--   0        0        0     2800 1970-01-01 00:00:00.000000 qtgql-0.119.2/PKG-INFO
```

### Comparing `qtgql-0.119.1/LICENSE` & `qtgql-0.119.2/LICENSE`

 * *Files identical despite different names*

### Comparing `qtgql-0.119.1/README.md` & `qtgql-0.119.2/README.md`

 * *Files identical despite different names*

### Comparing `qtgql-0.119.1/pyproject.toml` & `qtgql-0.119.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qtgql"
-version = "0.119.1"
+version = "0.119.2"
 packages = [{ include = "qtgqlcodegen" }]
 description = "Qt framework for building graphql driven QML applications"
 authors = ["Nir <88795475+nrbnlulu@users.noreply.github.com>"]
 maintainers = ["Nir.J Benlulu <nrbnlulu@gmail.com>"]
 license = "MIT"
 readme = "README.md"
```

### Comparing `qtgql-0.119.1/qtgqlcodegen/cli.py` & `qtgql-0.119.2/qtgqlcodegen/cli.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.119.1/qtgqlcodegen/compiler/builtin_scalars.py` & `qtgql-0.119.2/qtgqlcodegen/compiler/builtin_scalars.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.119.1/qtgqlcodegen/compiler/operation.py` & `qtgql-0.119.2/qtgqlcodegen/compiler/operation.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,14 +94,15 @@
     @classmethod
     def from_field(
         cls,
         field_definition: QtGqlFieldDefinition,
         selection_set: Optional[gql_lang.SelectionSetNode],
         operation: QtGqlOperationDefinition,
         parent_interface_field: Optional[QtGqlQueriedField] = UNSET,
+        is_root: bool = False,
     ) -> QtGqlQueriedField:
         """Main purpose here is to find inner selections of fields, this could
         be an object type, interface, union or a list.
 
         Any other fields should not have inner selections.
         """
         assert parent_interface_field is not UNSET
@@ -228,26 +229,31 @@
         )
 
 
 @define(slots=False)
 class QtGqlQueriedObjectType:
     definition: QtGqlObjectTypeDefinition = attrs.field(on_setattr=attrs.setters.frozen)
     fields: dict[str, QtGqlQueriedField] = attrs.Factory(dict)
+    is_root_field: bool = False
 
     @cached_property
     def name(self) -> str:
         return f"{self.definition.name}__{'$'.join(sorted(self.fields.keys()))}"
 
     @cached_property
     def doc_fields(self) -> str:
         return "{} {{\n  {}\n}}".format(
             self.definition.name,
             "\n   ".join(self.fields.keys()),
         )
 
+    @cached_property
+    def references(self) -> list[QtGqlQueriedField]:
+        return [f for f in self.fields.values() if f.type.is_object_type]
+
 
 @define(slots=False)
 class QtGqlOperationDefinition:
     operation_def: gql_def.OperationDefinitionNode
     evaluator: SchemaEvaluator
     directives: list[str] = attrs.Factory(list)
     fragments: list[str] = attrs.Factory(list)
@@ -285,14 +291,15 @@
     def root_field(self) -> QtGqlQueriedField:
         root_field_def: gql_lang.FieldNode = self.operation_def.selection_set.selections[0]  # type: ignore
         return QtGqlQueriedField.from_field(
             self._root_type.fields_dict[root_field_def.name.value],
             root_field_def.selection_set,
             self,
             parent_interface_field=None,
+            is_root=True,
         )
 
     @classmethod
     def from_definition(
         cls,
         operation_def: gql_def.OperationDefinitionNode,
         evaluator: SchemaEvaluator,
```

### Comparing `qtgql-0.119.1/qtgqlcodegen/compiler/template.py` & `qtgql-0.119.2/qtgqlcodegen/compiler/template.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.119.1/qtgqlcodegen/config.py` & `qtgql-0.119.2/qtgqlcodegen/config.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.119.1/qtgqlcodegen/graphql_ref.py` & `qtgql-0.119.2/qtgqlcodegen/graphql_ref.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.119.1/qtgqlcodegen/introspection.py` & `qtgql-0.119.2/qtgqlcodegen/introspection.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.119.1/qtgqlcodegen/objecttype.py` & `qtgql-0.119.2/qtgqlcodegen/objecttype.py`

 * *Files 4% similar despite different names*

```diff
@@ -92,15 +92,15 @@
 @define(slots=False)
 class QtGqlFieldDefinition(BaseQtGqlFieldDefinition):
     @cached_property
     def default_value(self):
         if builtin_scalar := self.type.is_builtin_scalar:
             return builtin_scalar.default_value
         if self.type.is_object_type:
-            raise NotImplementedError
+            return "{}"
 
         if self.type.is_model:
             # this would just generate the model without data.
             raise NotImplementedError
 
         if self.type.is_custom_scalar:
             return "{}"
@@ -321,15 +321,15 @@
         if scalar := t_self.is_custom_scalar:
             return scalar.type_name
         if gql_enum := t_self.is_enum:
             return gql_enum.name
         if model_of := t_self.is_model:
             return f"{QtGqlTypes.QGraphQLList.name}[{model_of.member_type}]"
         if object_def := t_self.is_object_type or t_self.is_interface:
-            return f"{object_def.name}"
+            return f"std::shared_ptr<{object_def.name}>"
         if q_object_def := t_self.is_queried_object_type:
             return f"{q_object_def.name}"
         if t_self.is_union:
             return "std::variant<" + ", ".join(th.member_type for th in t_self.of_type) + ">"
         if input_obj := t_self.is_input_object_type:
             return input_obj.name
```

### Comparing `qtgql-0.119.1/qtgqlcodegen/runtime/custom_scalars.py` & `qtgql-0.119.2/qtgqlcodegen/runtime/custom_scalars.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.119.1/qtgqlcodegen/templates/config.jinja.hpp` & `qtgql-0.119.2/qtgqlcodegen/templates/config.jinja.hpp`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 {% if context.selections or context.choices %}
-    {
+{
+{
         {% for name, selection in context.selections.items() %}
                 {"👉name👈", {%if selection %} 👉selection👈 {% else %} {} {% endif %}},{% endfor %}
-    },
+}
 {% if context.choices %}
-choices={
+.choices{
 {% for choice_name, selections in context.choices.items() %}
     "👉choice_name👈": {
                        {% for field_name, inner_template in selections.items() %} {"👉field_name👈", 👉inner_template👈}, {% endfor %}
 }
 {% endfor %}
 }
 {% endif %}
+}
 {% endif %}
```

### Comparing `qtgql-0.119.1/qtgqlcodegen/templates/macros.jinja.hpp` & `qtgql-0.119.2/qtgqlcodegen/templates/macros.jinja.hpp`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,13 @@
 {% macro deserialize_field(f, assign_to, include_selection_check = True) -%}
 
 if ({% if include_selection_check %}config.selections.contains("👉f.name👈") && {% endif %} !data.value("👉f.name👈").isNull()){
 {% if f.type.is_object_type -%}
 
-  👉 assign_to 👈 = 👉f.type.is_object_type.name👈.from_dict(
-  parent,
-  field_data,
-  inner_config,
-  metadata,
-
-);
+👉 assign_to 👈 = 👉f.type.is_object_type.name👈::from_json(data.value("👉f.name👈").toObject(), config.selections.value("person"), metadata);
 
 {% elif f.type.is_interface -%}
 if field_data:
         👉 assign_to 👈 = 👉f.type.is_interface.name👈.from_dict(
         parent,
         field_data,
         inner_config,
```

### Comparing `qtgql-0.119.1/qtgqlcodegen/templates/operation.jinja.hpp` & `qtgql-0.119.2/qtgqlcodegen/templates/operation.jinja.hpp`

 * *Files 12% similar despite different names*

```diff
@@ -4,38 +4,42 @@
 #include <qtgql/gqlwstransport/gqlwstransport.hpp>
 
 namespace 👉 context.config.env_name 👈{
 namespace 👉context.ns👈{
 
 inline const qtgql::bases::OperationMetadata OPERATION_METADATA = qtgql::bases::OperationMetadata{
         "👉 context.operation.name 👈",
-        {
-                👉 context.operation.root_field.as_conf_string() 👈
-        }
+        {👉 context.operation.root_field.as_conf_string() 👈}
 };
 
 
 {% for t in context.operation.narrowed_types %}
 class 👉 t.name 👈{
 /*
 👉 t.doc_fields 👈
  */
     Q_GADGET
 std::shared_ptr<👉context.schema_ns👈::👉 t.definition.name 👈> m_inst;
+{% for ref in t.references -%}
+std::unique_ptr<👉ref.narrowed_type.name👈> m_👉ref.name👈;
+{% endfor %}
 
 public:
-
-👉 t.name 👈(const QJsonObject& data,
-const qtgql::bases::SelectionsConfig& config){
-    m_inst = 👉context.schema_ns👈::👉 t.definition.name 👈::from_json(data, config, OPERATION_METADATA);
-
+👉 t.name 👈(const std::shared_ptr<👉 t.definition.name 👈> inst ): m_inst{inst}{
+{% for ref in t.references -%}
+m_👉ref.name👈 = std::make_unique<👉ref.narrowed_type.name👈>(m_inst->👉ref.definition.getter_name 👈());
+{% endfor %}
 }
 {%- for f in t.fields.values() %}
-inline const 👉 f.property_type 👈 & 👉 f.definition.getter_name 👈() const {
+[[nodiscard]] inline const 👉 f.property_type 👈 & 👉 f.definition.getter_name 👈() const {
+    {% if f.type.is_object_type %}
+    return *m_👉f.name👈;
+    {% else %}
     return m_inst->👉 f.definition.getter_name 👈();
+    {% endif %}
 };
 {% endfor -%}
 };
 {% endfor %}
 
 class 👉 context.operation.name 👈: public qtgql::gqlwstransport::OperationHandlerABC {
     Q_OBJECT
@@ -58,15 +62,18 @@
 }
 
 
 void on_next(const QJsonObject &message) override{
     if (!m_data && message.contains("data")){
         auto data = message.value("data").toObject();
         if (data.contains("👉 context.operation.root_field.name 👈")){
-            m_data = std::make_unique<👉 context.operation.root_field.property_type 👈>(data.value("👉 context.operation.root_field.name 👈").toObject(), OPERATION_METADATA.selections);
+            m_data = std::make_unique<👉 context.operation.root_field.property_type 👈>(
+👉context.schema_ns👈::👉 context.operation.root_field.definition.type.is_object_type.name 👈::from_json(
+        data.value("👉 context.operation.root_field.name 👈").toObject(), OPERATION_METADATA.selections, OPERATION_METADATA)
+);
         }
     }
 }
 inline const 👉 context.operation.root_field.property_type 👈* get_data(){
     return m_data.get();
 }
```

### Comparing `qtgql-0.119.1/qtgqlcodegen/templates/schema.jinja.hpp` & `qtgql-0.119.2/qtgqlcodegen/templates/schema.jinja.hpp`

 * *Files 8% similar despite different names*

```diff
@@ -20,42 +20,41 @@
     static qtgql::bases::ObjectStore<👉 type.name 👈> _store;
     return _store;
 }
 
 👉 macros.props(type) 👈
 public:
 inline static const QString TYPE_NAME = "👉 type.name 👈";
-👉 type.name 👈 (QObject* parent = nullptr)
+explicit 👉 type.name 👈 (QObject* parent = nullptr)
 : qtgql::bases::👉 base_class 👈::👉 base_class 👈(parent) {};
 
 
 static std::shared_ptr<👉 type.name 👈> from_json(const QJsonObject& data,
-                                 const qtgql::bases::SelectionsConfig& config,
+                                 const qtgql::bases::SelectionsConfig &config,
                                  const qtgql::bases::OperationMetadata& metadata){
 auto inst = std::make_shared<👉 type.name 👈>();
 {% for f in type.fields -%}
 {% set assign_to %} inst->👉 f.private_name 👈 {% endset %}
 👉macros.deserialize_field(f, assign_to)👈
 {% endfor %}
-
 {% if type.id_is_optional %}
 if (inst->id) {
   auto record = qtgql::bases::NodeRecord(node = inst, retainers = set())
                     .retain(metadata.operation_name)
                         cls.INST_STORE.add_record(record)
 }
 {% elif type.has_id_field and not type.id_is_optional %}
 auto record = std::make_shared<qtgql::bases::NodeRecord<👉 type.name 👈>>(inst);
 record->retain(metadata.operation_name);
 INST_STORE().add_record(record);
 {% endif %}
 return inst;
-  };
-{% endfor %}
+};
 
 void loose(const qtgql::bases::OperationMetadata &metadata){throw "not implemented";};
 void update(const QJsonObject &data,
             const qtgql::bases::SelectionsConfig &selections){throw "not implemented";};
 
 };
+{% endfor %}
 
 }
```

### Comparing `qtgql-0.119.1/qtgqlcodegen/utils.py` & `qtgql-0.119.2/qtgqlcodegen/utils.py`

 * *Files identical despite different names*

### Comparing `qtgql-0.119.1/PKG-INFO` & `qtgql-0.119.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qtgql
-Version: 0.119.1
+Version: 0.119.2
 Summary: Qt framework for building graphql driven QML applications
 License: MIT
 Author: Nir
 Author-email: 88795475+nrbnlulu@users.noreply.github.com
 Maintainer: Nir.J Benlulu
 Maintainer-email: nrbnlulu@gmail.com
 Requires-Python: >=3.9,<3.12
```

