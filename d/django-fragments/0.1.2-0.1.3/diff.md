# Comparing `tmp/django_fragments-0.1.2.tar.gz` & `tmp/django_fragments-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_fragments-0.1.2.tar", max compression
+gzip compressed data, was "django_fragments-0.1.3.tar", max compression
```

## Comparing `django_fragments-0.1.2.tar` & `django_fragments-0.1.3.tar`

### file list

```diff
@@ -1,18 +1,21 @@
--rw-r--r--   0        0        0     1491 2023-05-09 09:45:58.288456 django_fragments-0.1.2/LICENSE
--rw-r--r--   0        0        0      690 2023-05-09 09:47:26.935180 django_fragments-0.1.2/README.md
--rw-r--r--   0        0        0       27 2023-05-10 21:50:52.993055 django_fragments-0.1.2/django_fragments/__init__.py
--rw-r--r--   0        0        0      163 2023-05-08 11:11:49.135944 django_fragments-0.1.2/django_fragments/apps.py
--rw-r--r--   0        0        0      258 2023-05-10 22:57:17.273819 django_fragments-0.1.2/django_fragments/forms.py
--rw-r--r--   0        0        0      292 2023-05-07 15:19:00.977243 django_fragments-0.1.2/django_fragments/templates/svg/heroicons_x_mark_mini.html
--rw-r--r--   0        0        0      132 2023-05-10 23:33:49.851109 django_fragments-0.1.2/django_fragments/templates/test_snippet.html
--rw-r--r--   0        0        0        0 2023-05-07 23:31:34.843055 django_fragments-0.1.2/django_fragments/templatetags/__init__.py
--rw-r--r--   0        0        0     5104 2023-05-10 23:39:18.905343 django_fragments-0.1.2/django_fragments/templatetags/fragments.py
--rw-r--r--   0        0        0     2039 2023-05-09 09:39:46.557198 django_fragments-0.1.2/django_fragments/templatetags/helpers.py
--rw-r--r--   0        0        0     1649 2023-05-09 09:40:55.305731 django_fragments-0.1.2/django_fragments/templatetags/og.py
--rw-r--r--   0        0        0       70 2023-05-08 02:09:45.909742 django_fragments-0.1.2/django_fragments/templatetags/utils/__init__.py
--rw-r--r--   0        0        0     2157 2023-05-08 02:17:55.382358 django_fragments-0.1.2/django_fragments/templatetags/utils/filter_attrs.py
--rw-r--r--   0        0        0     4146 2023-05-08 08:19:35.581999 django_fragments-0.1.2/django_fragments/templatetags/utils/wrap_svg.py
--rw-r--r--   0        0        0     4978 2023-05-10 23:39:48.860675 django_fragments-0.1.2/django_fragments/tests.py
--rw-r--r--   0        0        0      424 2023-05-10 23:01:29.088719 django_fragments-0.1.2/django_fragments/utils.py
--rw-r--r--   0        0        0     1406 2023-05-10 23:40:08.516052 django_fragments-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1482 1970-01-01 00:00:00.000000 django_fragments-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1491 2023-05-09 09:45:58.288456 django_fragments-0.1.3/LICENSE
+-rw-r--r--   0        0        0      690 2023-05-09 09:47:26.935180 django_fragments-0.1.3/README.md
+-rw-r--r--   0        0        0       27 2023-05-10 21:50:52.993055 django_fragments-0.1.3/django_fragments/__init__.py
+-rw-r--r--   0        0        0      163 2023-05-08 11:11:49.135944 django_fragments-0.1.3/django_fragments/apps.py
+-rw-r--r--   0        0        0      258 2023-05-10 22:57:17.273819 django_fragments-0.1.3/django_fragments/forms.py
+-rw-r--r--   0        0        0      473 2023-05-11 03:15:53.052499 django_fragments-0.1.3/django_fragments/templates/_test_base.html
+-rw-r--r--   0        0        0      413 2023-05-11 03:15:53.052885 django_fragments-0.1.3/django_fragments/templates/home.html
+-rw-r--r--   0        0        0      292 2023-05-07 15:19:00.977243 django_fragments-0.1.3/django_fragments/templates/svg/heroicons_x_mark_mini.html
+-rw-r--r--   0        0        0      131 2023-05-11 03:15:53.053123 django_fragments-0.1.3/django_fragments/templates/test_snippet.html
+-rw-r--r--   0        0        0        0 2023-05-07 23:31:34.843055 django_fragments-0.1.3/django_fragments/templatetags/__init__.py
+-rw-r--r--   0        0        0     6023 2023-05-11 03:15:53.053369 django_fragments-0.1.3/django_fragments/templatetags/fragments.py
+-rw-r--r--   0        0        0     3435 2023-05-11 03:15:53.053593 django_fragments-0.1.3/django_fragments/templatetags/helpers.py
+-rw-r--r--   0        0        0     1649 2023-05-09 09:40:55.305731 django_fragments-0.1.3/django_fragments/templatetags/og.py
+-rw-r--r--   0        0        0       70 2023-05-08 02:09:45.909742 django_fragments-0.1.3/django_fragments/templatetags/utils/__init__.py
+-rw-r--r--   0        0        0     2157 2023-05-08 02:17:55.382358 django_fragments-0.1.3/django_fragments/templatetags/utils/filter_attrs.py
+-rw-r--r--   0        0        0     4146 2023-05-08 08:19:35.581999 django_fragments-0.1.3/django_fragments/templatetags/utils/wrap_svg.py
+-rw-r--r--   0        0        0     5491 2023-05-11 03:15:53.053834 django_fragments-0.1.3/django_fragments/tests.py
+-rw-r--r--   0        0        0      754 2023-05-11 03:15:53.054065 django_fragments-0.1.3/django_fragments/urls.py
+-rw-r--r--   0        0        0      424 2023-05-11 03:15:18.733152 django_fragments-0.1.3/django_fragments/utils.py
+-rw-r--r--   0        0        0     1406 2023-05-11 03:15:53.055440 django_fragments-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1482 1970-01-01 00:00:00.000000 django_fragments-0.1.3/PKG-INFO
```

### Comparing `django_fragments-0.1.2/LICENSE` & `django_fragments-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `django_fragments-0.1.2/README.md` & `django_fragments-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `django_fragments-0.1.2/django_fragments/templatetags/fragments.py` & `django_fragments-0.1.3/django_fragments/templatetags/fragments.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from pathlib import Path
 
 from django import template
 from django.conf import settings
-from django.forms import Field
+from django.forms import BoundField
 from django.http.request import HttpRequest
 from django.template import Context, Template
 from django.template.loader import render_to_string
 from django.urls import reverse
 from django.utils.html import format_html
 from django.utils.safestring import SafeText, mark_safe
 from markdown import markdown
@@ -92,39 +92,60 @@
     path = folder / f"{prefix}_{name}.html"
     html = render_to_string(str(path))
     svg_with_kwargs = wrap_svg(html_markup=html, css=css, **kwargs)
     return mark_safe(str(svg_with_kwargs).strip())
 
 
 @register.simple_tag
-def input(bound: Field, kls: str, label_kls: str | None = None) -> SafeText:
-    """Can likely replace this with prospective Django 5.0's
-    `django.forms.BoundField.as_field_group`"""
+def hput(
+    bound: BoundField,
+    kls: str | None = "h",
+    label_kls: str | None = None,
+    validate: str | None = None,
+) -> SafeText:
+    """An encapsulation of an idiomatic BoundField with an optional ability for htmx inline
+    field validation if a url is passed as `validate` argument.
+
+    Args:
+        bound (BoundField): The field to render
+        kls (str | None, optional): If supplied will supply the containing div's class attribute. Defaults to "h".
+        label_kls (str | None, optional): If supplied will supply the containing div's class attribute. Defaults to None.
+        validate (str | None, optional): A url that should be the form's submit url for inline field validation using htmx. Defaults to None.
+
+    Returns:
+        SafeText: The html fragment consisting of a wrapped field
+    """  # noqa: E501
+    from .helpers import hx_enable_inline_validation
+
+    attrs = hx_enable_inline_validation(bound, validate) if validate else ""
     return mark_safe(
         Template("""
             {% load fragments %}
             {% whitespaceless %}
-            <div class="{{ kls }}
-                data-hidden="{{ bound.is_hidden}}"
+            <div {{attrs}}
+                {% if bound.is_hidden %}hidden{% endif %}
+                {% if bound.errors %}data-invalid=true{% endif %}
+                class="{{ kls }}"
                 data-widget="{{ bound.widget_type }}"
             >
                 <label for="{{ bound.id_for_label }}"
                     {% if label_kls %}class="{{ label_kls }}"{% endif %}>
                     {{bound.label}}
                 </label>
                 {{ bound }}
-                <p class="help">{{ bound.help_text }}</p>
+                <small>{{ bound.help_text }}</small>
                 {{ bound.errors }}
             </div>
             {% endwhitespaceless %}
             """)  # noqa: E501
         .render(
             context=Context(
                 {
                     "bound": bound,
-                    "kls": kls,
                     "label_kls": label_kls,
+                    "kls": kls,
+                    "attrs": attrs,
                 },
             )
         )
         .strip()
     )
```

### Comparing `django_fragments-0.1.2/django_fragments/templatetags/og.py` & `django_fragments-0.1.3/django_fragments/templatetags/og.py`

 * *Files identical despite different names*

### Comparing `django_fragments-0.1.2/django_fragments/templatetags/utils/filter_attrs.py` & `django_fragments-0.1.3/django_fragments/templatetags/utils/filter_attrs.py`

 * *Files identical despite different names*

### Comparing `django_fragments-0.1.2/django_fragments/templatetags/utils/wrap_svg.py` & `django_fragments-0.1.3/django_fragments/templatetags/utils/wrap_svg.py`

 * *Files identical despite different names*

### Comparing `django_fragments-0.1.2/django_fragments/tests.py` & `django_fragments-0.1.3/django_fragments/tests.py`

 * *Files 25% similar despite different names*

```diff
@@ -76,48 +76,59 @@
 
 @pytest.mark.parametrize(
     "data, html",
     [
         (  # unbound form, no values
             None,
             (
-                '<div class="fieldWrapper data-hidden="False"'
-                ' data-widget="email"><label for="id_email">Email</label><input'
-                ' type="email" name="email" required id="id_email"><p'
-                ' class="help">Testable form</p></div><div class="fieldWrapper'
-                ' data-hidden="False" data-widget="textarea"><label'
+                '<div class="fieldWrapper" data-widget="email"><label'
+                ' for="id_email">Email</label><input type="email" name="email" required'
+                ' id="id_email"><small>Testable form</small></div><div'
+                ' class="fieldWrapper" data-widget="textarea"><label'
                 ' for="id_message">Message</label><textarea name="message" cols="40"'
-                ' rows="3" required id="id_message"></textarea><p'
-                ' class="help"></p></div>'
+                ' rows="3" required id="id_message"></textarea><small></small></div>'
             ),
         ),
         (  # bound valid form, no error message list
             {"message": "Hi there", "email": "foo@example.com"},
             (
-                '<div class="fieldWrapper data-hidden="False"'
-                ' data-widget="email"><label for="id_email">Email</label><input'
-                ' type="email" name="email" value="foo@example.com" required'
-                ' id="id_email"><p class="help">Testable form</p></div><div'
-                ' class="fieldWrapper data-hidden="False" data-widget="textarea"><label'
+                '<div class="fieldWrapper" data-widget="email"><label'
+                ' for="id_email">Email</label><input type="email" name="email"'
+                ' value="foo@example.com" required id="id_email"><small>Testable'
+                ' form</small></div><div class="fieldWrapper"'
+                ' data-widget="textarea"><label'
                 ' for="id_message">Message</label><textarea name="message" cols="40"'
-                ' rows="3" required id="id_message">Hi there</textarea><p'
-                ' class="help"></p></div>'
+                ' rows="3" required id="id_message">Hi'
+                " there</textarea><small></small></div>"
             ),
         ),
         (  # bound invalid form, with error message list
             {"message": "Hi there", "email": "foo"},
             (
-                '<div class="fieldWrapper data-hidden="False"'
-                ' data-widget="email"><label for="id_email">Email</label><input'
-                ' type="email" name="email" value="foo" required id="id_email"><p'
-                ' class="help">Testable form</p><ul class="errorlist"><li>Enter a valid'
-                ' email address.</li></ul></div><div class="fieldWrapper'
-                ' data-hidden="False" data-widget="textarea"><label'
+                '<div data-invalid=true class="fieldWrapper" data-widget="email"><label'
+                ' for="id_email">Email</label><input type="email" name="email"'
+                ' value="foo" required id="id_email"><small>Testable form</small><ul'
+                ' class="errorlist"><li>Enter a valid email'
+                ' address.</li></ul></div><div class="fieldWrapper"'
+                ' data-widget="textarea"><label'
                 ' for="id_message">Message</label><textarea name="message" cols="40"'
-                ' rows="3" required id="id_message">Hi there</textarea><p'
-                ' class="help"></p></div>'
+                ' rows="3" required id="id_message">Hi'
+                " there</textarea><small></small></div>"
             ),
         ),
     ],
 )
 def test_contact_form(data, html):
     assert ContactForm(data).render() == html  # type: ignore
+
+
+def test_boundfield_with_inline_validation():
+    template = """{% load fragments %}{% spaceless %}{% hput form.email validate="/this-is-an-endpoint" %}{% endspaceless %}"""
+    context = Context({"form": ContactForm()})
+    html = (
+        '<div id="hput_id_email" hx-select="#hput_id_email"'
+        ' hx-post="/this-is-an-endpoint" hx-trigger="blur from:find input"'
+        ' hx-target="#hput_id_email" hx-swap="outerHTML" class="h"'
+        ' data-widget="email"><label for="id_email">Email</label><input type="email"'
+        ' name="email" required id="id_email"><small>Testable form</small></div>'
+    )
+    assert Template(template).render(context=context) == html
```

### Comparing `django_fragments-0.1.2/pyproject.toml` & `django_fragments-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "django-fragments"
 description = "Custom template tags for common html idioms in Django."
-version = "0.1.2"
+version = "0.1.3"
 authors = ["Marcelino G. Veloso III <mars@veloso.one>"]
 readme = "README.md"
 homepage = "https://mv3.dev"
 repository = "https://github.com/justmars/django-fragments"
 documentation = "https://mv3.dev/django-fragments"
 classifiers = [
   "Programming Language :: Python :: 3.11",
```

### Comparing `django_fragments-0.1.2/PKG-INFO` & `django_fragments-0.1.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-fragments
-Version: 0.1.2
+Version: 0.1.3
 Summary: Custom template tags for common html idioms in Django.
 Home-page: https://mv3.dev
 Author: Marcelino G. Veloso III
 Author-email: mars@veloso.one
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Pytest
```

