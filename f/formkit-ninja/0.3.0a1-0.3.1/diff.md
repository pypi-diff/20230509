# Comparing `tmp/formkit_ninja-0.3.0a1.tar.gz` & `tmp/formkit_ninja-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "formkit_ninja-0.3.0a1.tar", max compression
+gzip compressed data, was "formkit_ninja-0.3.1.tar", max compression
```

## Comparing `formkit_ninja-0.3.0a1.tar` & `formkit_ninja-0.3.1.tar`

### file list

```diff
@@ -1,19 +1,21 @@
--rw-r--r--   0        0        0      813 2023-04-06 13:15:44.220033 formkit_ninja-0.3.0a1/README.md
--rw-r--r--   0        0        0        0 2023-04-06 13:15:44.220033 formkit_ninja-0.3.0a1/formkit_ninja/__init__.py
--rw-r--r--   0        0        0       21 2023-04-06 13:15:44.224033 formkit_ninja-0.3.0a1/formkit_ninja/__main__.py
--rw-r--r--   0        0        0    14754 2023-04-26 06:27:35.615331 formkit_ninja-0.3.0a1/formkit_ninja/admin.py
--rw-r--r--   0        0        0     1714 2023-04-26 06:10:12.439548 formkit_ninja-0.3.0a1/formkit_ninja/api.py
--rw-r--r--   0        0        0     4333 2023-04-10 00:27:28.783846 formkit_ninja-0.3.0a1/formkit_ninja/fields.py
--rw-r--r--   0        0        0    13135 2023-04-13 06:01:40.565549 formkit_ninja-0.3.0a1/formkit_ninja/formkit_schema.py
--rw-r--r--   0        0        0        0 2023-04-23 01:43:59.588049 formkit_ninja-0.3.0a1/formkit_ninja/management/__init__.py
--rw-r--r--   0        0        0        0 2023-04-06 13:15:44.220033 formkit_ninja-0.3.0a1/formkit_ninja/management/commands/__init__.py
--rw-r--r--   0        0        0     3955 2023-04-26 06:10:12.528997 formkit_ninja-0.3.0a1/formkit_ninja/management/commands/common_nodes.py
--rw-r--r--   0        0        0    19101 2023-04-26 06:35:40.064339 formkit_ninja-0.3.0a1/formkit_ninja/management/commands/create_sf11_form.py
--rw-r--r--   0        0        0     3190 2023-04-26 06:36:11.021575 formkit_ninja-0.3.0a1/formkit_ninja/management/commands/create_sf12_form.py
--rw-r--r--   0        0        0     1360 2023-04-26 06:10:12.411087 formkit_ninja-0.3.0a1/formkit_ninja/management/commands/create_sf13_form.py
--rw-r--r--   0        0        0    15058 2023-04-26 08:00:47.228814 formkit_ninja-0.3.0a1/formkit_ninja/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2023-04-13 11:58:36.247052 formkit_ninja-0.3.0a1/formkit_ninja/migrations/__init__.py
--rw-r--r--   0        0        0    11459 2023-04-26 06:10:12.671301 formkit_ninja-0.3.0a1/formkit_ninja/models.py
--rw-r--r--   0        0        0      101 2023-04-06 13:15:44.224033 formkit_ninja-0.3.0a1/formkit_ninja/urls.py
--rw-r--r--   0        0        0     1201 2023-04-28 02:14:47.604734 formkit_ninja-0.3.0a1/pyproject.toml
--rw-r--r--   0        0        0     1574 1970-01-01 00:00:00.000000 formkit_ninja-0.3.0a1/PKG-INFO
+-rw-r--r--   0        0        0      813 2023-04-06 13:15:44.220033 formkit_ninja-0.3.1/README.md
+-rw-r--r--   0        0        0        0 2023-04-06 13:15:44.220033 formkit_ninja-0.3.1/formkit_ninja/__init__.py
+-rw-r--r--   0        0        0       21 2023-04-06 13:15:44.224033 formkit_ninja-0.3.1/formkit_ninja/__main__.py
+-rw-r--r--   0        0        0    14860 2023-05-09 05:40:10.838963 formkit_ninja-0.3.1/formkit_ninja/admin.py
+-rw-r--r--   0        0        0     2568 2023-05-09 05:38:40.651974 formkit_ninja-0.3.1/formkit_ninja/api.py
+-rw-r--r--   0        0        0     4333 2023-04-10 00:27:28.783846 formkit_ninja-0.3.1/formkit_ninja/fields.py
+-rw-r--r--   0        0        0    13509 2023-05-09 05:25:34.174674 formkit_ninja-0.3.1/formkit_ninja/formkit_schema.py
+-rw-r--r--   0        0        0        0 2023-04-23 01:43:59.588049 formkit_ninja-0.3.1/formkit_ninja/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-06 13:15:44.220033 formkit_ninja-0.3.1/formkit_ninja/management/commands/__init__.py
+-rw-r--r--   0        0        0     3807 2023-05-09 05:37:21.012799 formkit_ninja-0.3.1/formkit_ninja/management/commands/common_nodes.py
+-rw-r--r--   0        0        0    19033 2023-05-09 05:17:09.351553 formkit_ninja-0.3.1/formkit_ninja/management/commands/create_sf11_form.py
+-rw-r--r--   0        0        0     3190 2023-04-26 06:36:11.021575 formkit_ninja-0.3.1/formkit_ninja/management/commands/create_sf12_form.py
+-rw-r--r--   0        0        0     1360 2023-04-26 06:10:12.411087 formkit_ninja-0.3.1/formkit_ninja/management/commands/create_sf13_form.py
+-rw-r--r--   0        0        0    15059 2023-05-09 05:38:40.671974 formkit_ninja-0.3.1/formkit_ninja/migrations/0001_initial.py
+-rw-r--r--   0        0        0      605 2023-05-09 05:15:03.707613 formkit_ninja-0.3.1/formkit_ninja/migrations/0002_alter_formcomponents_label_alter_formkitschema_key.py
+-rw-r--r--   0        0        0      339 2023-05-09 05:37:27.484727 formkit_ninja-0.3.1/formkit_ninja/migrations/0003_delete_translatable.py
+-rw-r--r--   0        0        0        0 2023-04-13 11:58:36.247052 formkit_ninja-0.3.1/formkit_ninja/migrations/__init__.py
+-rw-r--r--   0        0        0     9588 2023-05-09 05:38:40.647974 formkit_ninja-0.3.1/formkit_ninja/models.py
+-rw-r--r--   0        0        0      101 2023-04-06 13:15:44.224033 formkit_ninja-0.3.1/formkit_ninja/urls.py
+-rw-r--r--   0        0        0     1199 2023-05-09 05:55:08.053571 formkit_ninja-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     1572 1970-01-01 00:00:00.000000 formkit_ninja-0.3.1/PKG-INFO
```

### Comparing `formkit_ninja-0.3.0a1/README.md` & `formkit_ninja-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `formkit_ninja-0.3.0a1/formkit_ninja/admin.py` & `formkit_ninja-0.3.1/formkit_ninja/admin.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
-from functools import reduce
 
 import logging
 import operator
 import warnings
-from typing import Any, Optional
+from functools import reduce
+from typing import Any, Literal, Optional
 
 from django import forms
 from django.contrib import admin
 from django.http import HttpRequest
 from ordered_model.admin import OrderedInlineModelAdminMixin, OrderedModelAdmin, OrderedTabularInline
 
 from formkit_ninja import models
@@ -103,19 +103,21 @@
     )
     ordering = ("order",)
     extra = 0
 
 
 class FormKitSchemaComponentInline(OrderedTabularInline):
     model = models.FormComponents
-    # form = FormComponentsForm
     readonly_fields = (
+        "node",
+        "created_by",
+        "updated_by",
+        "id",
         "order",
         "move_up_down_links",
-        "node",
     )
     ordering = ("order",)
     extra = 0
 
 
 class FormKitNodeGroupForm(JsonDecoratedFormBase):
     class Meta:
@@ -145,15 +147,16 @@
     This is the most common component type: the 'FormKit' schema node
     """
 
     class Meta:
         model = models.FormKitSchemaNode
         fields = ("label", "translation_context", "description", "additional_props")
 
-    # The `_json_fields["node"]` item affects the admin form, adding the fields included in the `FormKitSchemaProps.__fields__.items` dict
+    # The `_json_fields["node"]` item affects the admin form,
+    # adding the fields included in the `FormKitSchemaProps.__fields__.items` dict
     _json_fields = {
         "node": (
             "formkit",
             "description",
             "name",
             "key",
             "html_id",
@@ -407,15 +410,17 @@
                             "validationVisibility",
                             "validationMessages",
                             "validationRules",
                         )
                     },
                 )
             )
-            if obj.node.get("formkit") == "repeater":
+            # The "Repeater" has some specific fields
+            # See these specified in FormKitNodeRepeaterForm
+            if obj.node and obj.node.get("formkit", None) == "repeater":
                 fieldsets.append(
                     (
                         "Repeater field properties",
                         {"fields": ("addLabel", "upControl", "downControl", "itemsClass", "itemClass")},
                     )
                 )
 
@@ -428,47 +433,41 @@
     def get_form(
         self,
         request: Any,
         obj: models.FormKitSchemaNode | None,
         change: None = None,
         **kwargs,
     ):
+        # Handle different formkit node types
+        formkit_forms = {"group": FormKitNodeGroupForm, "repeater": FormKitNodeRepeaterForm}
+
+        # Handle different node types
+        forms = {
+            "condition": FormKitConditionForm,
+            "$formkit": FormKitNodeForm,
+            "$el": FormKitElementForm,
+            "text": FormKitTextNode,
+            "$cmp": FormKitComponentForm,
+        }
         if not obj:
             return NewFormKitForm
+        if node_type := getattr(obj, "node_type", None) is None:
+            return super().get_form(request, obj, change, **kwargs)
 
-        try:
-            node_type: FORMKIT_TYPE = obj.node_type
-        except (AttributeError, KeyError) as E:
-            warnings.warn("Expected a 'Node' with a 'NodeType' in the admin form")
-            warnings.warn(f"{E}")
-
-        if node_type == "condition":
-            return FormKitConditionForm
-
-        elif node_type == "$formkit":
-            formkit_node_type = (obj.node or {}).get("formkit", None)
-
+        if node_type == "$formkit":
+            formkit_node_type: Literal["group", "repeater", None] = (obj.node or {}).get("formkit", None)
             # Some special 'formkitnode' types have their own admin page
-            if formkit_node_type == "group":
-                return FormKitNodeGroupForm
-            elif formkit_node_type == "repeater":
-                return FormKitNodeRepeaterForm
-            return FormKitNodeForm
-
-        elif node_type == "$el":
-            return FormKitElementForm
-
-        elif node_type == "text":
-            return FormKitTextNode
+            if formkit_node_type in formkit_forms:
+                return formkit_forms.get(formkit_node_type)
 
-        elif node_type == "$cmp":
-            return FormKitComponentForm
+        if node_type in forms:
+            return forms[node_type]
 
-        else:
-            return super().get_form(request, obj, change, **kwargs)
+        warnings.warn(f"Expected: one of [{','.join(forms.keys())}]. Got {node_type}")
+        return super().get_form(request, obj, change, **kwargs)
 
 
 @admin.register(models.Option)
 class OptionAdmin(OrderedModelAdmin):
     form = OptionForm
     readonly_fields = ("id",)
     list_display = ("value", "label", "field", "move_up_down_links")
@@ -492,12 +491,7 @@
         FormKitSchemaComponentInline,
     ]
 
 
 @admin.register(models.FormComponents)
 class FormComponentsAdmin(OrderedModelAdmin):
     list_display = ("label", "schema", "node", "move_up_down_links")
-
-
-@admin.register(models.Translatable)
-class TranslatableAdmin(admin.ModelAdmin):
-    list_display = ("field", "language_code", "value", "context")
```

### Comparing `formkit_ninja-0.3.0a1/formkit_ninja/fields.py` & `formkit_ninja-0.3.1/formkit_ninja/fields.py`

 * *Files identical despite different names*

### Comparing `formkit_ninja-0.3.0a1/formkit_ninja/formkit_schema.py` & `formkit_ninja-0.3.1/formkit_ninja/formkit_schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -143,14 +143,20 @@
 
 class DateNode(FormKitSchemaProps):
     node_type: Literal["formkit"] = "formkit"
     formkit: Literal["date"] = "date"
     dollar_formkit: str = Field(default="date", alias="$formkit")
 
 
+class DatePickerNode(FormKitSchemaProps):
+    node_type: Literal["formkit"] = "formkit"
+    formkit: Literal["date"] = "datepicker"
+    dollar_formkit: str = Field(default="datepicker", alias="$formkit")
+
+
 class CheckBoxNode(FormKitSchemaProps):
     node_type: Literal["formkit"] = "formkit"
     formkit: Literal["checkbox"] = "checkbox"
     dollar_formkit: str = Field(default="checkbox", alias="$formkit")
 
 
 class NumberNode(FormKitSchemaProps):
@@ -225,14 +231,15 @@
         PasswordNode,
         SelectNode,
         EmailNode,
         NumberNode,
         RadioNode,
         GroupNode,
         DateNode,
+        DatePickerNode,
         DropDownNode,
         RepeaterNode,
     ],
     Field(discriminator="formkit"),
 ]
 
 
@@ -352,14 +359,15 @@
     "list",
     "password",
     "button",
     "select",
     "radio",
     "form",
     "date",
+    "datepicker",
     "dropdown",
     "repeater",
 ]
 
 
 class Discriminators(TypedDict, total=False):
     node_type: NODE_TYPE
@@ -406,14 +414,18 @@
 
 
 class FormKitNode(BaseModel):
     __root__: Node
 
     @classmethod
     def parse_obj(cls: Type["Model"], obj: Any) -> "Model":
+        """
+        This classmethod differentiates between the different "Node" types
+        when deserializing
+        """
         if "id" in obj:
             obj["html_id"] = obj.pop("id")
         try:
             return super().parse_obj({**get_node_type(obj), **obj})
         except KeyError as E:
             raise Exception(f"Unable to parse content {obj} to a {cls}") from E
```

### Comparing `formkit_ninja-0.3.0a1/formkit_ninja/management/commands/common_nodes.py` & `formkit_ninja-0.3.1/formkit_ninja/management/commands/common_nodes.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,16 +19,14 @@
                 formkit="select",
                 options="$getLocations()",
             ),
         ),
     )
     yield district, c
 
-    district.translatable_content()
-
     admin_post, c = models.FormKitSchemaNode.objects.get_or_create(
         label="admin_post",
         defaults=dict(
             node_type="$formkit",
             translation_context="admin_post",
             node=dict(
                 label="Administrative Post",
@@ -122,11 +120,7 @@
     yield models.FormComponents.objects.update_or_create(
         key="Aldeias for the Location Select schema",
         defaults=dict(
             schema=locations,
             node=aldeia,
         ),
     )
-
-    municipality.translatable_content()
-    admin_post.translatable_content()
-    suco.translatable_content()
```

### Comparing `formkit_ninja-0.3.0a1/formkit_ninja/management/commands/create_sf11_form.py` & `formkit_ninja-0.3.1/formkit_ninja/management/commands/create_sf11_form.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,100 +37,100 @@
     partisipants_group = {
         "children": [
             {
                 "key": "attendance_male",
                 "if": "$get(activity_type).value !== '----' && $get(activity_subtype).value !== '----' && $get(activity_subtype).value != 16 && $get(activity_subtype).value != 40 && $get(activity_subtype).value != 11",
                 "id": "attendance_male",
                 "name": "attendance_male",
-                "label": "$pgettext('partisipants', 'Total participants male')",
+                "label": "Total participants male",
                 "validation": "greaterThanOrEqualSum:kpa_male+community_member_male",
                 "validation-messages": {
-                    "greaterThanOrEqualSum": '$gettext("The total participants male should be greater than or equal to the sum of Participants Suku Management Team (SMT) - male and Number of community members - male")'
+                    "greaterThanOrEqualSum": "The total participants male should be greater than or equal to the sum of Participants Suku Management Team (SMT) - male and Number of community members - male"
                 },
                 "node_type": "formkit",
                 "formkit": "number",
                 "$formkit": "number",
                 "min": 0,
             },
             {
                 "key": "attendance_female",
                 "if": "$get(activity_type).value !== '----' && $get(activity_subtype).value !== '----' && $get(activity_subtype).value != 16 && $get(activity_subtype).value != 11",
                 "id": "attendance_female",
                 "name": "attendance_female",
-                "label": "$pgettext('partisipants', 'Total participants female')",
+                "label": "Total participants female",
                 "validation": "greaterThanOrEqualSum:kpa_female+community_member_female",
                 "validation-messages": {
-                    "greaterThanOrEqualSum": '$gettext("The total participants female should be greater than or equal to the sum of Participants Suku Management Team (SMT) - female and Number of community members - female")'
+                    "greaterThanOrEqualSum": "The total participants female should be greater than or equal to the sum of Participants Suku Management Team (SMT) - female and Number of community members - female"
                 },
                 "node_type": "formkit",
                 "formkit": "number",
                 "$formkit": "number",
                 "min": 0,
             },
             {
                 "key": "kpa_male",
                 "if": "$get(activity_type).value !== '----' && $get(activity_subtype).value !== '----' && $get(activity_subtype).value != 16 && $get(activity_subtype).value != 20 && $get(activity_subtype).value != 21 && $get(activity_subtype).value != 40 && $get(activity_subtype).value != 11",
                 "id": "kpa_male",
                 "name": "kpa_male",
-                "label": "$pgettext('partisipants', 'Participants Suku Management Team (SMT) - male')",
+                "label": "Participants Suku Management Team (SMT) - male",
                 "node_type": "formkit",
                 "formkit": "number",
                 "$formkit": "number",
                 "min": 0,
             },
             {
                 "key": "kpa_female",
                 "if": "$get(activity_type).value !== '----' && $get(activity_subtype).value !== '----' && $get(activity_subtype).value != 16 && $get(activity_subtype).value != 11 && $get(activity_subtype).value != 20 && $get(activity_subtype).value != 21",
                 "id": "kpa_female",
                 "name": "kpa_female",
-                "label": "$pgettext('partisipants', 'Participants Suku Management Team (SMT) - female')",
+                "label": "Participants Suku Management Team (SMT) - female",
                 "node_type": "formkit",
                 "formkit": "number",
                 "$formkit": "number",
                 "min": 0,
             },
             {
                 "key": "disable_male",
                 "if": "$get(activity_type).value !== '----' && $get(activity_subtype).value !== '----' && $get(activity_subtype).value != 16 && $get(activity_subtype).value != 40 && $get(activity_subtype).value != 11",
                 "id": "disable_male",
                 "name": "disable_male",
-                "label": "$pgettext('partisipants', 'Number of People with Disability - male')",
+                "label": "Number of People with Disability - male",
                 "node_type": "formkit",
                 "formkit": "number",
                 "$formkit": "number",
                 "min": 0,
             },
             {
                 "key": "disable_female",
                 "if": "$get(activity_type).value !== '----' && $get(activity_subtype).value !== '----' && $get(activity_subtype).value != 16 && $get(activity_subtype).value != 11",
                 "id": "disable_female",
                 "name": "disable_female",
-                "label": "$pgettext('partisipants', 'Number of People with Disability - female')",
+                "label": "Number of People with Disability - female",
                 "node_type": "formkit",
                 "formkit": "number",
                 "$formkit": "number",
                 "min": 0,
             },
             {
                 "key": "community_member_male",
                 "if": "$get(activity_type).value !== '----' && $get(activity_subtype).value !== '----' && $get(activity_subtype).value != 16 && $get(activity_subtype).value != 20 && $get(activity_subtype).value != 21 && $get(activity_subtype).value != 40 && $get(activity_subtype).value != 11",
                 "id": "community_member_male",
                 "name": "community_member_male",
-                "label": "$pgettext('partisipants', 'Number of community members - male')",
+                "label": "Number of community members - male",
                 "node_type": "formkit",
                 "formkit": "number",
                 "$formkit": "number",
                 "min": 0,
             },
             {
                 "key": "community_member_female",
                 "if": "$get(activity_type).value !== '----' && $get(activity_subtype).value !== '----' && $get(activity_subtype).value != 16 && $get(activity_subtype).value != 11 && $get(activity_subtype).value != 20 && $get(activity_subtype).value != 21",
                 "id": "community_member_female",
                 "name": "community_member_female",
-                "label": "$pgettext('partisipants', 'Number of community members - female')",
+                "label": "Number of community members - female",
                 "node_type": "formkit",
                 "formkit": "number",
                 "$formkit": "number",
                 "min": 0,
             },
         ],
         "name": "partisipants",
@@ -189,15 +189,15 @@
     )
 
     yield models.FormComponents.objects.update_or_create(
         defaults=dict(
             schema=meeting_information,
             node=activity_type,
         ),
-        label=f"SF 1.1 Meeting Information (activity type)",
+        label="SF 1.1 Meeting Information (activity type)",
     )
 
     # The JSON code for the Subtype nodes
 
     activity_subtype = FormKitNode.parse_obj(
         {
             "key": "activity_subtype",
@@ -413,18 +413,14 @@
         label="Aldeias for the for SF 1.1 Location Select schema",
         defaults=dict(
             schema=locations_sf11,
             node=sf11_aldeia,
         ),
     )
 
-    sf11_aldeia.translatable_content()
-    sf11_admin_post.translatable_content()
-    sf11_suco.translatable_content()
-
 
 class Command(BaseCommand):
     help = """
         Create the Partisipa 'SF11' form
         as a set of Django models / FormKit integration
     """
 
@@ -439,7 +435,12 @@
             if options["verbosity"] > 1:
                 self.stdout.write(self.style.SUCCESS(f"{'Created' if created else 'Updated'} {instance}"))
 
         self.stdout.write(self.style.SUCCESS("Writing Locations schema for SF 11"))
         for instance, created in create_sf11_locations():
             if options["verbosity"] > 1:
                 self.stdout.write(self.style.SUCCESS(f"{'Created' if created else 'Updated'} {instance}"))
+
+        # Update / Create translated content hooks for "labels" and "options"
+        for instance, created in models.FormKitSchemaNode.translatable_content():
+            if options["verbosity"] > 1:
+                self.stdout.write(self.style.SUCCESS(f"{'Created' if created else 'Updated'} {instance}"))
```

### Comparing `formkit_ninja-0.3.0a1/formkit_ninja/management/commands/create_sf12_form.py` & `formkit_ninja-0.3.1/formkit_ninja/management/commands/create_sf12_form.py`

 * *Files identical despite different names*

### Comparing `formkit_ninja-0.3.0a1/formkit_ninja/management/commands/create_sf13_form.py` & `formkit_ninja-0.3.1/formkit_ninja/management/commands/create_sf13_form.py`

 * *Files identical despite different names*

### Comparing `formkit_ninja-0.3.0a1/formkit_ninja/migrations/0001_initial.py` & `formkit_ninja-0.3.1/formkit_ninja/migrations/0001_initial.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Generated by Django 4.1.5 on 2023-04-26 08:00
 
+import uuid
+
+import django.db.models.deletion
 from django.conf import settings
 from django.db import migrations, models
-import django.db.models.deletion
-import uuid
 
 
 class Migration(migrations.Migration):
 
     initial = True
 
     dependencies = [
```

### Comparing `formkit_ninja-0.3.0a1/formkit_ninja/models.py` & `formkit_ninja-0.3.1/formkit_ninja/models.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 import itertools
 import json
 import logging
 import uuid
 from typing import Iterable, TypedDict, get_args
 
 from django.conf import settings
+from django.core.exceptions import ValidationError
 from django.db import models
 from django.utils.functional import cached_property
+from django.utils.text import slugify
 from ordered_model.models import OrderedModel
 
 from . import formkit_schema
 
 logger = logging.getLogger()
 
 
@@ -35,34 +37,14 @@
         settings.AUTH_USER_MODEL, on_delete=models.PROTECT, related_name="+", blank=True, null=True
     )
     updated_by = models.ForeignKey(
         settings.AUTH_USER_MODEL, on_delete=models.PROTECT, related_name="+", blank=True, null=True
     )
 
 
-class Translatable(UuidIdModel):
-    """
-    This is a holder for "translatable" content from different fields
-    """
-
-    object_id = models.UUIDField(editable=False, help_text="The UUID of the model which this translation relates to")
-    language_code = models.CharField(max_length=3, editable=False)
-
-    # These are translation values: "field", "value", "context" and "msgstr"
-    field = models.CharField(max_length=100, help_text="The field on the generic model to translate", editable=False)
-    value = models.CharField(max_length=5000, null=True, blank=True, editable=False)
-    context = models.CharField(max_length=1024, null=True, blank=True, editable=False)
-    msgstr = models.CharField(max_length=5000, help_text="The string")
-
-    # options_function = models.CharField(max_length=1024, null=True, blank=True, editable=False, help_text="If 'options' are provided client side enter the function string. ie `$getOptions(...)`")
-
-    def __str__(self):
-        return f"{self.value} ({self.language_code})"
-
-
 class OptionDict(TypedDict):
     value: str
     label: str
 
 
 class Option(OrderedModel, UuidIdModel):
     """
@@ -94,17 +76,15 @@
 class FormComponents(OrderedModel, UuidIdModel):
     """
     A model relating "nodes" of a schema to a schema with model ordering
     """
 
     schema = models.ForeignKey("FormKitSchema", on_delete=models.CASCADE)
     node = models.ForeignKey("FormKitSchemaNode", on_delete=models.CASCADE)
-    label = models.CharField(
-        max_length=1024, unique=True, help_text="Used as a human-readable label", default=uuid.uuid4
-    )
+    label = models.CharField(max_length=1024, help_text="Used as a human-readable label")
 
     order_with_respect_to = "schema"
 
     class Meta:
         ordering = ("schema", "order")
 
     def __str__(self):
@@ -192,48 +172,14 @@
     translation_context = models.CharField(
         max_length=1024,
         null=True,
         blank=True,
         help_text="The gettext context to use to translate Options, label, placeholder and help text",
     )
 
-    def translatable_content(self):
-        """
-        Returns UUID, context, and label for content which can be i18n marked
-        """
-        from django.conf import settings
-
-        translatable_fields = ("label", "placeholder")
-        language_codes = [lang[0] for lang in settings.LANGUAGES if lang[0] != "en"]
-
-        # Make a 'translatable' type object for each language/field
-        # specified in settings
-
-        for field, code in itertools.product(translatable_fields, language_codes):
-            if not self.node:
-                continue
-            value = self.node.get(field, None)
-            if not value:
-                continue
-            logger.info(f"adding translatable string: {value}")
-            Translatable.objects.get_or_create(
-                object_id=self.id, language_code=code, field=field, context=self.translation_context, value=value
-            )
-
-        # Also add translation hooks for the content of "options" if present
-        options: Iterable[Option] = self.option_set.all()
-        for option, code in itertools.product(options, language_codes):
-            Translatable.objects.get_or_create(
-                object_id=self.id,
-                language_code=code,
-                field="option",
-                value=option.label or option.value,
-                context=self.translation_context,
-            )
-
     def __str__(self):
         return self.label
 
     def save(self, *args, **kwargs):
         """
         On save validate the 'node' field matches the 'FormKitNode'
         """
@@ -243,38 +189,38 @@
     def node_options(self):
         """
         Because "options" are translated and
         separately stored, this step is necessary to
         reinstate them
         """
         options: Iterable[Option] = self.option_set.all()
-        return [{"value": option.value} for option in options]
+        return [{"value": option.value, "label": option.label} for option in options]
 
     def get_node_values(self) -> dict:
         """
         Reify a 'dict' instance suitable for creating
         a FormKit Schema node from
         """
+        if not self.node:
+            return {}
         values = {**self.node}
         if self.node_options:
             values["options"] = self.node_options
         return values
 
-    def get_node(self) -> formkit_schema.FormKitNode:
+    def get_node(self) -> formkit_schema.Node:
         """
         Return a "decorated" node instance
         with restored options and translated fields
         """
-        return formkit_schema.FormKitNode.parse_obj(self.get_node_values())
-
-    def get_node_type() -> str:
-        """
-        Return the "type" of a FormKit node
-        """
-        return
+        node_content = self.get_node_values()
+        formkit_node = formkit_schema.FormKitNode.parse_obj(node_content)
+        # 'FormKitNode' is really a container to store any kind
+        # of Node
+        return formkit_node.__root__
 
     @classmethod
     def from_pydantic(
         cls, input_models: Iterable[formkit_schema.FormKitNode]
     ) -> Iterable[tuple["FormKitSchemaNode", Iterable[Option]]]:
         for input_model in input_models:
             instance = cls()
@@ -298,15 +244,15 @@
 
 class FormKitSchema(UuidIdModel):
     """
     This represents a "FormKitSchema" which is an heterogenous
     collection of items.
     """
 
-    key = models.SlugField(max_length=1024, unique=True)
+    key = models.TextField(max_length=1024, unique=True)
     nodes = models.ManyToManyField(FormKitSchemaNode, through=FormComponents)
     objects = SchemaManager()
 
     def get_schema_values(self):
         """
         Return a list of "node" dicts
         """
@@ -316,14 +262,23 @@
     def to_pydantic(self):
         values = list(self.get_schema_values())
         return formkit_schema.FormKitSchema.parse_obj(values)
 
     def __str__(self):
         return self.key
 
+    def clean(self):
+        slugified = slugify(self.key)
+        for instance in self._meta.model.objects.exclude(pk=self.pk):
+            if slugified == slugify(instance.key):
+                raise ValidationError(
+                    f"The name '{self.key} clashed with {instance.key}. Please enter a different name."
+                )
+        return super().clean()
+
     @classmethod
     def from_pydantic(cls, input_model: formkit_schema.FormKitSchema) -> "FormKitSchema":
         """
         Converts a given Pydantic representation of a Schema
         to Django database fields
         """
         instance = cls.objects.create()
```

### Comparing `formkit_ninja-0.3.0a1/pyproject.toml` & `formkit_ninja-0.3.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "formkit-ninja"
-version = "0.3.0a1"
+version = "0.3.1"
 description = "A Django-Ninja backend to specify FormKit schemas"
 authors = ["Josh Brooks <josh@catalpa.io>"]
 license = "GPLv3"
 readme = "README.md"
 homepage = "https://github.com/catalpainternational/formkit-ninja"
 repository = "https://github.com/catalpainternational/formkit-ninja"
 packages = [{include = "formkit_ninja"}]
```

### Comparing `formkit_ninja-0.3.0a1/PKG-INFO` & `formkit_ninja-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: formkit-ninja
-Version: 0.3.0a1
+Version: 0.3.1
 Summary: A Django-Ninja backend to specify FormKit schemas
 Home-page: https://github.com/catalpainternational/formkit-ninja
 License: GPLv3
 Author: Josh Brooks
 Author-email: josh@catalpa.io
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
```

