# Comparing `tmp/django_unfold-0.5.3.tar.gz` & `tmp/django_unfold-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_unfold-0.5.3.tar", max compression
+gzip compressed data, was "django_unfold-0.6.0.tar", max compression
```

## Comparing `django_unfold-0.5.3.tar` & `django_unfold-0.6.0.tar`

### file list

```diff
@@ -1,116 +1,133 @@
--rw-r--r--   0        0        0     1082 2023-01-13 08:15:39.294988 django_unfold-0.5.3/LICENSE
--rw-r--r--   0        0        0    24431 2023-04-16 18:09:25.250028 django_unfold-0.5.3/README.md
--rw-r--r--   0        0        0     1290 2023-04-25 16:51:27.159997 django_unfold-0.5.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-21 12:27:16.286605 django_unfold-0.5.3/src/unfold/__init__.py
--rw-r--r--   0        0        0    18412 2023-04-23 16:40:44.097338 django_unfold-0.5.3/src/unfold/admin.py
--rw-r--r--   0        0        0      307 2023-04-21 12:27:16.287919 django_unfold-0.5.3/src/unfold/apps.py
--rw-r--r--   0        0        0        0 2023-04-21 12:27:16.288025 django_unfold-0.5.3/src/unfold/contrib/__init__.py
--rw-r--r--   0        0        0        0 2023-04-21 12:27:16.288132 django_unfold-0.5.3/src/unfold/contrib/filters/__init__.py
--rw-r--r--   0        0        0    14454 2023-04-21 12:27:16.288308 django_unfold-0.5.3/src/unfold/contrib/filters/admin.py
--rw-r--r--   0        0        0      107 2023-04-21 12:27:16.288447 django_unfold-0.5.3/src/unfold/contrib/filters/apps.py
--rw-r--r--   0        0        0     4055 2023-04-21 12:27:16.288719 django_unfold-0.5.3/src/unfold/contrib/filters/forms.py
--rw-r--r--   0        0        0     4221 2023-04-21 12:27:16.288899 django_unfold-0.5.3/src/unfold/contrib/filters/static/unfold/filters/css/nouislider.min.css
--rw-r--r--   0        0        0    19332 2023-04-21 12:27:16.289101 django_unfold-0.5.3/src/unfold/contrib/filters/static/unfold/filters/js/DateTimeShortcuts.js
--rw-r--r--   0        0        0     1668 2023-04-21 12:27:16.289262 django_unfold-0.5.3/src/unfold/contrib/filters/static/unfold/filters/js/admin-numeric-filter.js
--rw-r--r--   0        0        0    26683 2023-04-21 12:27:16.289501 django_unfold-0.5.3/src/unfold/contrib/filters/static/unfold/filters/js/nouislider.min.js
--rw-r--r--   0        0        0     2236 2023-04-21 12:27:16.289662 django_unfold-0.5.3/src/unfold/contrib/filters/static/unfold/filters/js/wNumb.min.js
--rw-r--r--   0        0        0      470 2023-04-21 12:27:16.289830 django_unfold-0.5.3/src/unfold/contrib/filters/templates/unfold/filters/filters_date_range.html
--rw-r--r--   0        0        0      470 2023-04-21 12:27:16.289978 django_unfold-0.5.3/src/unfold/contrib/filters/templates/unfold/filters/filters_datetime_range.html
--rw-r--r--   0        0        0      338 2023-04-21 12:27:16.290268 django_unfold-0.5.3/src/unfold/contrib/filters/templates/unfold/filters/filters_numeric_range.html
--rw-r--r--   0        0        0      273 2023-04-21 12:27:16.290446 django_unfold-0.5.3/src/unfold/contrib/filters/templates/unfold/filters/filters_numeric_single.html
--rw-r--r--   0        0        0     1648 2023-04-21 12:27:16.290615 django_unfold-0.5.3/src/unfold/contrib/filters/templates/unfold/filters/filters_numeric_slider.html
--rw-r--r--   0        0        0        0 2023-04-21 12:27:16.290713 django_unfold-0.5.3/src/unfold/contrib/forms/__init__.py
--rw-r--r--   0        0        0      105 2023-04-21 12:27:16.290870 django_unfold-0.5.3/src/unfold/contrib/forms/apps.py
--rw-r--r--   0        0        0    20007 2023-04-21 12:27:16.291077 django_unfold-0.5.3/src/unfold/contrib/forms/static/unfold/forms/css/trix.css
--rw-r--r--   0        0        0      858 2023-04-21 12:27:16.291263 django_unfold-0.5.3/src/unfold/contrib/forms/static/unfold/forms/js/trix.config.js
--rw-r--r--   0        0        0   172634 2023-04-21 12:27:16.291864 django_unfold-0.5.3/src/unfold/contrib/forms/static/unfold/forms/js/trix.js
--rw-r--r--   0        0        0     9558 2023-04-21 12:27:16.292065 django_unfold-0.5.3/src/unfold/contrib/forms/templates/unfold/forms/helpers/toolbar.html
--rw-r--r--   0        0        0      351 2023-04-21 12:27:16.292215 django_unfold-0.5.3/src/unfold/contrib/forms/templates/unfold/forms/wysiwyg.html
--rw-r--r--   0        0        0      886 2023-04-21 12:27:16.292361 django_unfold-0.5.3/src/unfold/contrib/forms/widgets.py
--rw-r--r--   0        0        0     1487 2023-04-21 12:27:16.292502 django_unfold-0.5.3/src/unfold/decorators.py
--rw-r--r--   0        0        0       43 2023-04-21 12:27:16.292670 django_unfold-0.5.3/src/unfold/exceptions.py
--rw-r--r--   0        0        0     2920 2023-04-21 12:27:16.292849 django_unfold-0.5.3/src/unfold/forms.py
--rw-r--r--   0        0        0     1116 2023-04-21 12:27:16.293085 django_unfold-0.5.3/src/unfold/settings.py
--rw-r--r--   0        0        0     8345 2023-04-22 09:45:19.675394 django_unfold-0.5.3/src/unfold/sites.py
--rw-r--r--   0        0        0     3890 2023-04-21 12:27:16.293525 django_unfold-0.5.3/src/unfold/static/unfold/css/simplebar.css
--rw-r--r--   0        0        0    71322 2023-04-23 16:41:16.604253 django_unfold-0.5.3/src/unfold/static/unfold/css/styles.css
--rw-r--r--   0        0        0    39813 2023-04-21 12:27:16.294180 django_unfold-0.5.3/src/unfold/static/unfold/js/alpine.js
--rw-r--r--   0        0        0      511 2023-04-21 12:27:16.294353 django_unfold-0.5.3/src/unfold/static/unfold/js/alpine.persist.js
--rw-r--r--   0        0        0     1628 2023-04-21 12:27:16.294509 django_unfold-0.5.3/src/unfold/static/unfold/js/app.js
--rw-r--r--   0        0        0    39951 2023-04-21 12:27:16.294770 django_unfold-0.5.3/src/unfold/static/unfold/js/htmx.js
--rw-r--r--   0        0        0    65855 2023-04-21 12:27:16.295127 django_unfold-0.5.3/src/unfold/static/unfold/js/simplebar.js
--rw-r--r--   0        0        0     2519 2023-04-21 12:27:16.295294 django_unfold-0.5.3/src/unfold/templates/admin/actions.html
--rw-r--r--   0        0        0      802 2023-04-21 12:27:16.295436 django_unfold-0.5.3/src/unfold/templates/admin/app_index.html
--rw-r--r--   0        0        0     3594 2023-04-21 12:27:16.295583 django_unfold-0.5.3/src/unfold/templates/admin/app_list.html
--rw-r--r--   0        0        0      478 2023-04-21 12:27:16.295725 django_unfold-0.5.3/src/unfold/templates/admin/auth/user/add_form.html
--rw-r--r--   0        0        0     2829 2023-04-21 12:27:16.295871 django_unfold-0.5.3/src/unfold/templates/admin/auth/user/change_password.html
--rw-r--r--   0        0        0     3503 2023-04-21 12:27:16.296015 django_unfold-0.5.3/src/unfold/templates/admin/base.html
--rw-r--r--   0        0        0      361 2023-04-21 12:27:16.296151 django_unfold-0.5.3/src/unfold/templates/admin/base_site.html
--rw-r--r--   0        0        0     5001 2023-04-21 12:27:16.296296 django_unfold-0.5.3/src/unfold/templates/admin/change_form.html
--rw-r--r--   0        0        0      686 2023-04-21 12:27:16.296448 django_unfold-0.5.3/src/unfold/templates/admin/change_form_object_tools.html
--rw-r--r--   0        0        0     8376 2023-04-21 12:27:16.296647 django_unfold-0.5.3/src/unfold/templates/admin/change_list.html
--rw-r--r--   0        0        0      699 2023-04-21 12:27:16.297088 django_unfold-0.5.3/src/unfold/templates/admin/change_list_object_tools.html
--rw-r--r--   0        0        0     4082 2023-04-21 12:27:16.297356 django_unfold-0.5.3/src/unfold/templates/admin/change_list_results.html
--rw-r--r--   0        0        0     1306 2023-04-21 12:27:16.297588 django_unfold-0.5.3/src/unfold/templates/admin/date_hierarchy.html
--rw-r--r--   0        0        0     5158 2023-04-21 12:27:16.297821 django_unfold-0.5.3/src/unfold/templates/admin/delete_confirmation.html
--rw-r--r--   0        0        0     4941 2023-04-21 12:27:16.298062 django_unfold-0.5.3/src/unfold/templates/admin/delete_selected_confirmation.html
--rw-r--r--   0        0        0     4372 2023-04-21 12:27:16.298276 django_unfold-0.5.3/src/unfold/templates/admin/edit_inline/stacked.html
--rw-r--r--   0        0        0    12199 2023-04-21 12:27:16.298553 django_unfold-0.5.3/src/unfold/templates/admin/edit_inline/tabular.html
--rw-r--r--   0        0        0     1479 2023-04-21 12:27:16.298778 django_unfold-0.5.3/src/unfold/templates/admin/filter.html
--rw-r--r--   0        0        0     3047 2023-04-23 16:40:44.098304 django_unfold-0.5.3/src/unfold/templates/admin/includes/fieldset.html
--rw-r--r--   0        0        0      468 2023-04-21 12:27:16.299180 django_unfold-0.5.3/src/unfold/templates/admin/includes/object_delete_summary.html
--rw-r--r--   0        0        0      674 2023-04-22 09:45:19.676010 django_unfold-0.5.3/src/unfold/templates/admin/index.html
--rw-r--r--   0        0        0     3494 2023-04-22 09:45:19.676184 django_unfold-0.5.3/src/unfold/templates/admin/login.html
--rw-r--r--   0        0        0     1178 2023-04-21 12:27:16.299975 django_unfold-0.5.3/src/unfold/templates/admin/nav_sidebar.html
--rw-r--r--   0        0        0     3951 2023-04-21 12:27:16.300177 django_unfold-0.5.3/src/unfold/templates/admin/object_history.html
--rw-r--r--   0        0        0     1173 2023-04-21 12:27:16.300371 django_unfold-0.5.3/src/unfold/templates/admin/pagination.html
--rw-r--r--   0        0        0     1143 2023-04-23 16:02:42.848153 django_unfold-0.5.3/src/unfold/templates/admin/search_form.html
--rw-r--r--   0        0        0     4306 2023-04-21 12:27:16.300816 django_unfold-0.5.3/src/unfold/templates/admin/submit_line.html
--rw-r--r--   0        0        0     1751 2023-04-21 12:27:16.301001 django_unfold-0.5.3/src/unfold/templates/admin/widgets/clearable_file_input.html
--rw-r--r--   0        0        0     3888 2023-04-22 09:45:19.676369 django_unfold-0.5.3/src/unfold/templates/admin/widgets/related_widget_wrapper.html
--rw-r--r--   0        0        0      848 2023-04-21 12:27:16.301779 django_unfold-0.5.3/src/unfold/templates/admin/widgets/split_datetime.html
--rw-r--r--   0        0        0      785 2023-04-21 12:27:16.301978 django_unfold-0.5.3/src/unfold/templates/auth/widgets/read_only_password_hash.html
--rw-r--r--   0        0        0     1028 2023-04-21 12:27:16.302149 django_unfold-0.5.3/src/unfold/templates/registration/logged_out.html
--rw-r--r--   0        0        0     1062 2023-04-21 12:27:16.302314 django_unfold-0.5.3/src/unfold/templates/registration/password_change_done.html
--rw-r--r--   0        0        0     2225 2023-04-21 12:27:16.302475 django_unfold-0.5.3/src/unfold/templates/registration/password_change_form.html
--rw-r--r--   0        0        0     1083 2023-04-21 12:27:16.302643 django_unfold-0.5.3/src/unfold/templates/unfold/helpers/actions_row.html
--rw-r--r--   0        0        0     3908 2023-04-21 12:27:16.302826 django_unfold-0.5.3/src/unfold/templates/unfold/helpers/app_list.html
--rw-r--r--   0        0        0     3302 2023-04-23 15:58:58.488273 django_unfold-0.5.3/src/unfold/templates/unfold/helpers/app_list_default.html
--rw-r--r--   0        0        0      466 2023-04-21 12:27:16.303144 django_unfold-0.5.3/src/unfold/templates/unfold/helpers/boolean.html
--rw-r--r--   0        0        0      234 2023-04-21 12:27:16.303305 django_unfold-0.5.3/src/unfold/templates/unfold/helpers/breadcrumb_item.html
--rw-r--r--   0        0        0      248 2023-04-21 12:27:16.303469 django_unfold-0.5.3/src/unfold/templates/unfold/helpers/display_header.html
--rw-r--r--   0        0        0     2072 2023-04-21 12:27:16.303789 django_unfold-0.5.3/src/unfold/templates/unfold/helpers/display_label.html
--rw-r--r--   0        0        0      325 2023-04-21 12:27:16.303938 django_unfold-0.5.3/src/unfold/templates/unfold/helpers/field.html
--rw-r--r--   0        0        0      266 2023-04-21 12:27:16.304088 django_unfold-0.5.3/src/unfold/templates/unfold/helpers/form_errors.html
--rw-r--r--   0        0        0      151 2023-04-22 09:45:19.676520 django_unfold-0.5.3/src/unfold/templates/unfold/helpers/help_text.html
--rw-r--r--   0        0        0     1995 2023-04-22 09:45:19.676674 django_unfold-0.5.3/src/unfold/templates/unfold/helpers/history.html
--rw-r--r--   0        0        0      237 2023-04-21 12:27:16.304552 django_unfold-0.5.3/src/unfold/templates/unfold/helpers/label.html
--rw-r--r--   0        0        0      557 2023-04-21 12:27:16.304713 django_unfold-0.5.3/src/unfold/templates/unfold/helpers/messages/error.html
--rw-r--r--   0        0        0      404 2023-04-21 12:27:16.304988 django_unfold-0.5.3/src/unfold/templates/unfold/helpers/messages/errornote.html
--rw-r--r--   0        0        0      143 2023-04-21 12:27:16.305125 django_unfold-0.5.3/src/unfold/templates/unfold/helpers/messages/info.html
--rw-r--r--   0        0        0      595 2023-04-21 12:27:16.305264 django_unfold-0.5.3/src/unfold/templates/unfold/helpers/messages.html
--rw-r--r--   0        0        0     1101 2023-04-21 12:27:16.306215 django_unfold-0.5.3/src/unfold/templates/unfold/helpers/navigation.html
--rw-r--r--   0        0        0       69 2023-04-21 12:27:16.306487 django_unfold-0.5.3/src/unfold/templates/unfold/helpers/pagination_current_item.html
--rw-r--r--   0        0        0       56 2023-04-21 12:27:16.306644 django_unfold-0.5.3/src/unfold/templates/unfold/helpers/pagination_ellipsis.html
--rw-r--r--   0        0        0     1314 2023-04-21 12:27:16.306800 django_unfold-0.5.3/src/unfold/templates/unfold/helpers/search.html
--rw-r--r--   0        0        0      725 2023-04-21 12:27:16.306954 django_unfold-0.5.3/src/unfold/templates/unfold/helpers/search_results.html
--rw-r--r--   0        0        0      442 2023-04-21 12:27:16.307106 django_unfold-0.5.3/src/unfold/templates/unfold/helpers/site_icon.html
--rw-r--r--   0        0        0     1862 2023-04-21 12:27:16.307252 django_unfold-0.5.3/src/unfold/templates/unfold/helpers/tab_list.html
--rw-r--r--   0        0        0     4895 2023-04-21 12:27:16.307409 django_unfold-0.5.3/src/unfold/templates/unfold/helpers/userlinks.html
--rw-r--r--   0        0        0     1120 2023-04-21 12:27:16.307570 django_unfold-0.5.3/src/unfold/templates/unfold/helpers/welcomemsg.html
--rw-r--r--   0        0        0      859 2023-04-21 12:27:16.307737 django_unfold-0.5.3/src/unfold/templates/unfold/layouts/base_simple.html
--rw-r--r--   0        0        0     3056 2023-04-21 12:27:16.308375 django_unfold-0.5.3/src/unfold/templates/unfold/layouts/skeleton.html
--rw-r--r--   0        0        0     2211 2023-04-21 12:27:16.308571 django_unfold-0.5.3/src/unfold/templates/unfold/widgets/clearable_file_input_small.html
--rw-r--r--   0        0        0       88 2023-04-21 12:27:16.308719 django_unfold-0.5.3/src/unfold/templates/unfold/widgets/date.html
--rw-r--r--   0        0        0      262 2023-04-21 12:27:16.308860 django_unfold-0.5.3/src/unfold/templates/unfold/widgets/range.html
--rw-r--r--   0        0        0      881 2023-04-21 12:27:16.309020 django_unfold-0.5.3/src/unfold/templates/unfold/widgets/split_datetime_vertical.html
--rw-r--r--   0        0        0      459 2023-04-21 12:27:16.309174 django_unfold-0.5.3/src/unfold/templates/unfold/widgets/textarea.html
--rw-r--r--   0        0        0       88 2023-04-21 12:27:16.309319 django_unfold-0.5.3/src/unfold/templates/unfold/widgets/time.html
--rw-r--r--   0        0        0        0 2023-04-21 12:27:16.309421 django_unfold-0.5.3/src/unfold/templatetags/__init__.py
--rw-r--r--   0        0        0     3203 2023-04-21 12:27:16.309586 django_unfold-0.5.3/src/unfold/templatetags/unfold.py
--rw-r--r--   0        0        0     9163 2023-04-21 12:27:16.309747 django_unfold-0.5.3/src/unfold/templatetags/unfold_list.py
--rw-r--r--   0        0        0     3716 2023-04-21 12:27:16.309904 django_unfold-0.5.3/src/unfold/utils.py
--rw-r--r--   0        0        0      660 2023-04-21 12:27:16.310054 django_unfold-0.5.3/src/unfold/views.py
--rw-r--r--   0        0        0     7126 2023-04-21 12:27:16.310231 django_unfold-0.5.3/src/unfold/widgets.py
--rw-r--r--   0        0        0    26805 1970-01-01 00:00:00.000000 django_unfold-0.5.3/setup.py
--rw-r--r--   0        0        0    25479 1970-01-01 00:00:00.000000 django_unfold-0.5.3/PKG-INFO
+-rw-r--r--   0        0        0     1082 2023-01-13 08:15:39.294988 django_unfold-0.6.0/LICENSE
+-rw-r--r--   0        0        0    25346 2023-05-12 17:59:11.443851 django_unfold-0.6.0/README.md
+-rw-r--r--   0        0        0     1273 2023-05-12 18:08:32.293031 django_unfold-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-25 16:53:58.827841 django_unfold-0.6.0/src/unfold/__init__.py
+-rw-r--r--   0        0        0    22083 2023-04-29 14:53:25.025426 django_unfold-0.6.0/src/unfold/admin.py
+-rw-r--r--   0        0        0      307 2023-04-25 16:53:58.828269 django_unfold-0.6.0/src/unfold/apps.py
+-rw-r--r--   0        0        0     1835 2023-04-29 14:48:57.720570 django_unfold-0.6.0/src/unfold/checks.py
+-rw-r--r--   0        0        0        0 2023-04-25 16:53:58.828366 django_unfold-0.6.0/src/unfold/contrib/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-25 16:53:58.828468 django_unfold-0.6.0/src/unfold/contrib/filters/__init__.py
+-rw-r--r--   0        0        0    16034 2023-04-29 14:54:36.705530 django_unfold-0.6.0/src/unfold/contrib/filters/admin.py
+-rw-r--r--   0        0        0      107 2023-04-25 16:53:58.828782 django_unfold-0.6.0/src/unfold/contrib/filters/apps.py
+-rw-r--r--   0        0        0     4055 2023-04-25 16:53:58.828924 django_unfold-0.6.0/src/unfold/contrib/filters/forms.py
+-rw-r--r--   0        0        0     4221 2023-04-25 16:53:58.829091 django_unfold-0.6.0/src/unfold/contrib/filters/static/unfold/filters/css/nouislider.min.css
+-rw-r--r--   0        0        0    19332 2023-04-25 16:53:58.829291 django_unfold-0.6.0/src/unfold/contrib/filters/static/unfold/filters/js/DateTimeShortcuts.js
+-rw-r--r--   0        0        0     1668 2023-04-25 16:53:58.829456 django_unfold-0.6.0/src/unfold/contrib/filters/static/unfold/filters/js/admin-numeric-filter.js
+-rw-r--r--   0        0        0    26683 2023-04-25 16:53:58.829680 django_unfold-0.6.0/src/unfold/contrib/filters/static/unfold/filters/js/nouislider.min.js
+-rw-r--r--   0        0        0     2236 2023-04-25 16:53:58.829830 django_unfold-0.6.0/src/unfold/contrib/filters/static/unfold/filters/js/wNumb.min.js
+-rw-r--r--   0        0        0      470 2023-04-25 16:53:58.829970 django_unfold-0.6.0/src/unfold/contrib/filters/templates/unfold/filters/filters_date_range.html
+-rw-r--r--   0        0        0      470 2023-04-25 16:53:58.830145 django_unfold-0.6.0/src/unfold/contrib/filters/templates/unfold/filters/filters_datetime_range.html
+-rw-r--r--   0        0        0      338 2023-04-25 16:53:58.830286 django_unfold-0.6.0/src/unfold/contrib/filters/templates/unfold/filters/filters_numeric_range.html
+-rw-r--r--   0        0        0      273 2023-04-25 16:53:58.830426 django_unfold-0.6.0/src/unfold/contrib/filters/templates/unfold/filters/filters_numeric_single.html
+-rw-r--r--   0        0        0     1648 2023-04-25 16:53:58.830578 django_unfold-0.6.0/src/unfold/contrib/filters/templates/unfold/filters/filters_numeric_slider.html
+-rw-r--r--   0        0        0        0 2023-04-25 16:53:58.830668 django_unfold-0.6.0/src/unfold/contrib/forms/__init__.py
+-rw-r--r--   0        0        0      105 2023-04-25 16:53:58.830813 django_unfold-0.6.0/src/unfold/contrib/forms/apps.py
+-rw-r--r--   0        0        0    20007 2023-04-25 16:53:58.830992 django_unfold-0.6.0/src/unfold/contrib/forms/static/unfold/forms/css/trix.css
+-rw-r--r--   0        0        0      858 2023-04-25 16:53:58.831136 django_unfold-0.6.0/src/unfold/contrib/forms/static/unfold/forms/js/trix.config.js
+-rw-r--r--   0        0        0   172634 2023-04-25 16:53:58.831717 django_unfold-0.6.0/src/unfold/contrib/forms/static/unfold/forms/js/trix.js
+-rw-r--r--   0        0        0     9558 2023-04-25 16:53:58.831938 django_unfold-0.6.0/src/unfold/contrib/forms/templates/unfold/forms/helpers/toolbar.html
+-rw-r--r--   0        0        0      351 2023-04-25 16:53:58.832097 django_unfold-0.6.0/src/unfold/contrib/forms/templates/unfold/forms/wysiwyg.html
+-rw-r--r--   0        0        0      962 2023-04-29 14:41:34.283805 django_unfold-0.6.0/src/unfold/contrib/forms/widgets.py
+-rw-r--r--   0        0        0        0 2023-05-12 17:59:11.446021 django_unfold-0.6.0/src/unfold/contrib/import_export/__init__.py
+-rw-r--r--   0        0        0      142 2023-05-12 17:59:11.446213 django_unfold-0.6.0/src/unfold/contrib/import_export/apps.py
+-rw-r--r--   0        0        0      672 2023-05-12 17:59:11.446368 django_unfold-0.6.0/src/unfold/contrib/import_export/forms.py
+-rw-r--r--   0        0        0      357 2023-05-12 17:59:11.446801 django_unfold-0.6.0/src/unfold/contrib/import_export/templates/admin/import_export/base.html
+-rw-r--r--   0        0        0      412 2023-05-12 17:59:11.446954 django_unfold-0.6.0/src/unfold/contrib/import_export/templates/admin/import_export/change_list_export_item.html
+-rw-r--r--   0        0        0      229 2023-05-12 17:59:11.447087 django_unfold-0.6.0/src/unfold/contrib/import_export/templates/admin/import_export/change_list_import_export.html
+-rw-r--r--   0        0        0      387 2023-05-12 17:59:11.447460 django_unfold-0.6.0/src/unfold/contrib/import_export/templates/admin/import_export/change_list_import_item.html
+-rw-r--r--   0        0        0     1791 2023-05-12 17:59:11.447700 django_unfold-0.6.0/src/unfold/contrib/import_export/templates/admin/import_export/export.html
+-rw-r--r--   0        0        0     2075 2023-05-12 17:59:11.448059 django_unfold-0.6.0/src/unfold/contrib/import_export/templates/admin/import_export/import.html
+-rw-r--r--   0        0        0      867 2023-05-12 17:59:11.448210 django_unfold-0.6.0/src/unfold/contrib/import_export/templates/admin/import_export/import_confirm.html
+-rw-r--r--   0        0        0     1422 2023-05-12 17:59:11.448490 django_unfold-0.6.0/src/unfold/contrib/import_export/templates/admin/import_export/import_errors.html
+-rw-r--r--   0        0        0     1312 2023-05-12 17:59:11.448646 django_unfold-0.6.0/src/unfold/contrib/import_export/templates/admin/import_export/import_form.html
+-rw-r--r--   0        0        0     2413 2023-05-12 17:59:11.448800 django_unfold-0.6.0/src/unfold/contrib/import_export/templates/admin/import_export/import_preview.html
+-rw-r--r--   0        0        0     4880 2023-05-12 17:59:11.448961 django_unfold-0.6.0/src/unfold/contrib/import_export/templates/admin/import_export/import_validation.html
+-rw-r--r--   0        0        0      199 2023-04-29 14:24:13.252315 django_unfold-0.6.0/src/unfold/dataclasses.py
+-rw-r--r--   0        0        0     3277 2023-04-29 14:41:34.283979 django_unfold-0.6.0/src/unfold/decorators.py
+-rw-r--r--   0        0        0       43 2023-04-25 16:53:58.832547 django_unfold-0.6.0/src/unfold/exceptions.py
+-rw-r--r--   0        0        0     3281 2023-04-29 14:41:34.284117 django_unfold-0.6.0/src/unfold/forms.py
+-rw-r--r--   0        0        0     1116 2023-04-25 16:53:58.832819 django_unfold-0.6.0/src/unfold/settings.py
+-rw-r--r--   0        0        0     9000 2023-04-29 14:41:34.284275 django_unfold-0.6.0/src/unfold/sites.py
+-rw-r--r--   0        0        0     3890 2023-04-25 16:53:58.833130 django_unfold-0.6.0/src/unfold/static/unfold/css/simplebar.css
+-rw-r--r--   0        0        0    71987 2023-05-12 17:59:11.449470 django_unfold-0.6.0/src/unfold/static/unfold/css/styles.css
+-rw-r--r--   0        0        0    41071 2023-04-29 14:24:13.253109 django_unfold-0.6.0/src/unfold/static/unfold/js/alpine.js
+-rw-r--r--   0        0        0      626 2023-05-12 17:59:11.449806 django_unfold-0.6.0/src/unfold/static/unfold/js/alpine.persist.js
+-rw-r--r--   0        0        0     1628 2023-04-25 16:53:58.834027 django_unfold-0.6.0/src/unfold/static/unfold/js/app.js
+-rw-r--r--   0        0        0    42820 2023-04-29 14:24:13.253449 django_unfold-0.6.0/src/unfold/static/unfold/js/htmx.js
+-rw-r--r--   0        0        0    65855 2023-04-25 16:53:58.834621 django_unfold-0.6.0/src/unfold/static/unfold/js/simplebar.js
+-rw-r--r--   0        0        0     2519 2023-04-25 16:53:58.834775 django_unfold-0.6.0/src/unfold/templates/admin/actions.html
+-rw-r--r--   0        0        0      802 2023-04-25 16:53:58.834928 django_unfold-0.6.0/src/unfold/templates/admin/app_index.html
+-rw-r--r--   0        0        0     3594 2023-04-25 16:53:58.835073 django_unfold-0.6.0/src/unfold/templates/admin/app_list.html
+-rw-r--r--   0        0        0      478 2023-04-25 16:53:58.835211 django_unfold-0.6.0/src/unfold/templates/admin/auth/user/add_form.html
+-rw-r--r--   0        0        0     2892 2023-05-12 17:59:11.450055 django_unfold-0.6.0/src/unfold/templates/admin/auth/user/change_password.html
+-rw-r--r--   0        0        0     3503 2023-04-25 16:53:58.835525 django_unfold-0.6.0/src/unfold/templates/admin/base.html
+-rw-r--r--   0        0        0      361 2023-04-25 16:53:58.835682 django_unfold-0.6.0/src/unfold/templates/admin/base_site.html
+-rw-r--r--   0        0        0     5001 2023-04-25 16:53:58.835845 django_unfold-0.6.0/src/unfold/templates/admin/change_form.html
+-rw-r--r--   0        0        0      686 2023-04-25 16:53:58.835984 django_unfold-0.6.0/src/unfold/templates/admin/change_form_object_tools.html
+-rw-r--r--   0        0        0     8376 2023-04-25 16:53:58.836131 django_unfold-0.6.0/src/unfold/templates/admin/change_list.html
+-rw-r--r--   0        0        0      699 2023-04-25 16:53:58.836285 django_unfold-0.6.0/src/unfold/templates/admin/change_list_object_tools.html
+-rw-r--r--   0        0        0     4206 2023-04-29 14:24:13.253582 django_unfold-0.6.0/src/unfold/templates/admin/change_list_results.html
+-rw-r--r--   0        0        0     1306 2023-04-25 16:53:58.836586 django_unfold-0.6.0/src/unfold/templates/admin/date_hierarchy.html
+-rw-r--r--   0        0        0     5166 2023-05-12 17:59:11.450271 django_unfold-0.6.0/src/unfold/templates/admin/delete_confirmation.html
+-rw-r--r--   0        0        0     4941 2023-04-25 16:53:58.836907 django_unfold-0.6.0/src/unfold/templates/admin/delete_selected_confirmation.html
+-rw-r--r--   0        0        0     4372 2023-04-25 16:53:58.837062 django_unfold-0.6.0/src/unfold/templates/admin/edit_inline/stacked.html
+-rw-r--r--   0        0        0    12199 2023-04-25 16:53:58.837259 django_unfold-0.6.0/src/unfold/templates/admin/edit_inline/tabular.html
+-rw-r--r--   0        0        0     1479 2023-04-25 16:53:58.837505 django_unfold-0.6.0/src/unfold/templates/admin/filter.html
+-rw-r--r--   0        0        0     3047 2023-04-25 16:53:58.837678 django_unfold-0.6.0/src/unfold/templates/admin/includes/fieldset.html
+-rw-r--r--   0        0        0      468 2023-04-25 16:53:58.837840 django_unfold-0.6.0/src/unfold/templates/admin/includes/object_delete_summary.html
+-rw-r--r--   0        0        0      674 2023-04-25 16:53:58.837997 django_unfold-0.6.0/src/unfold/templates/admin/index.html
+-rw-r--r--   0        0        0     3494 2023-04-25 16:53:58.838180 django_unfold-0.6.0/src/unfold/templates/admin/login.html
+-rw-r--r--   0        0        0     1178 2023-04-25 16:53:58.838335 django_unfold-0.6.0/src/unfold/templates/admin/nav_sidebar.html
+-rw-r--r--   0        0        0     3951 2023-04-25 16:53:58.838481 django_unfold-0.6.0/src/unfold/templates/admin/object_history.html
+-rw-r--r--   0        0        0     1173 2023-04-25 16:53:58.838617 django_unfold-0.6.0/src/unfold/templates/admin/pagination.html
+-rw-r--r--   0        0        0     1143 2023-04-25 16:53:58.839211 django_unfold-0.6.0/src/unfold/templates/admin/search_form.html
+-rw-r--r--   0        0        0     4306 2023-04-25 16:53:58.839427 django_unfold-0.6.0/src/unfold/templates/admin/submit_line.html
+-rw-r--r--   0        0        0     1751 2023-04-25 16:53:58.839617 django_unfold-0.6.0/src/unfold/templates/admin/widgets/clearable_file_input.html
+-rw-r--r--   0        0        0     3888 2023-04-25 16:53:58.839816 django_unfold-0.6.0/src/unfold/templates/admin/widgets/related_widget_wrapper.html
+-rw-r--r--   0        0        0      848 2023-04-25 16:53:58.839974 django_unfold-0.6.0/src/unfold/templates/admin/widgets/split_datetime.html
+-rw-r--r--   0        0        0      785 2023-04-25 16:53:58.840124 django_unfold-0.6.0/src/unfold/templates/auth/widgets/read_only_password_hash.html
+-rw-r--r--   0        0        0     1028 2023-04-25 16:53:58.840286 django_unfold-0.6.0/src/unfold/templates/registration/logged_out.html
+-rw-r--r--   0        0        0     1062 2023-04-25 16:53:58.840449 django_unfold-0.6.0/src/unfold/templates/registration/password_change_done.html
+-rw-r--r--   0        0        0     2225 2023-04-25 16:53:58.840609 django_unfold-0.6.0/src/unfold/templates/registration/password_change_form.html
+-rw-r--r--   0        0        0     1461 2023-04-29 14:24:13.253731 django_unfold-0.6.0/src/unfold/templates/unfold/helpers/actions_row.html
+-rw-r--r--   0        0        0     3908 2023-04-25 16:53:58.840917 django_unfold-0.6.0/src/unfold/templates/unfold/helpers/app_list.html
+-rw-r--r--   0        0        0     3302 2023-04-25 16:53:58.841436 django_unfold-0.6.0/src/unfold/templates/unfold/helpers/app_list_default.html
+-rw-r--r--   0        0        0      466 2023-04-25 16:53:58.841593 django_unfold-0.6.0/src/unfold/templates/unfold/helpers/boolean.html
+-rw-r--r--   0        0        0      234 2023-04-25 16:53:58.841751 django_unfold-0.6.0/src/unfold/templates/unfold/helpers/breadcrumb_item.html
+-rw-r--r--   0        0        0      248 2023-04-25 16:53:58.841920 django_unfold-0.6.0/src/unfold/templates/unfold/helpers/display_header.html
+-rw-r--r--   0        0        0     2072 2023-04-25 16:53:58.842071 django_unfold-0.6.0/src/unfold/templates/unfold/helpers/display_label.html
+-rw-r--r--   0        0        0      335 2023-05-12 17:59:11.450462 django_unfold-0.6.0/src/unfold/templates/unfold/helpers/field.html
+-rw-r--r--   0        0        0      266 2023-04-25 16:53:58.842332 django_unfold-0.6.0/src/unfold/templates/unfold/helpers/form_errors.html
+-rw-r--r--   0        0        0      151 2023-04-25 16:53:58.842459 django_unfold-0.6.0/src/unfold/templates/unfold/helpers/help_text.html
+-rw-r--r--   0        0        0     1995 2023-04-25 16:53:58.842615 django_unfold-0.6.0/src/unfold/templates/unfold/helpers/history.html
+-rw-r--r--   0        0        0      237 2023-04-25 16:53:58.842754 django_unfold-0.6.0/src/unfold/templates/unfold/helpers/label.html
+-rw-r--r--   0        0        0      557 2023-04-25 16:53:58.842902 django_unfold-0.6.0/src/unfold/templates/unfold/helpers/messages/error.html
+-rw-r--r--   0        0        0      404 2023-04-25 16:53:58.843034 django_unfold-0.6.0/src/unfold/templates/unfold/helpers/messages/errornote.html
+-rw-r--r--   0        0        0      143 2023-04-25 16:53:58.843183 django_unfold-0.6.0/src/unfold/templates/unfold/helpers/messages/info.html
+-rw-r--r--   0        0        0      595 2023-04-25 16:53:58.843319 django_unfold-0.6.0/src/unfold/templates/unfold/helpers/messages.html
+-rw-r--r--   0        0        0     1101 2023-04-29 08:17:13.737125 django_unfold-0.6.0/src/unfold/templates/unfold/helpers/navigation.html
+-rw-r--r--   0        0        0       69 2023-04-25 16:53:58.843716 django_unfold-0.6.0/src/unfold/templates/unfold/helpers/pagination_current_item.html
+-rw-r--r--   0        0        0       56 2023-04-25 16:53:58.843850 django_unfold-0.6.0/src/unfold/templates/unfold/helpers/pagination_ellipsis.html
+-rw-r--r--   0        0        0     1314 2023-04-25 16:53:58.843984 django_unfold-0.6.0/src/unfold/templates/unfold/helpers/search.html
+-rw-r--r--   0        0        0      725 2023-04-25 16:53:58.844119 django_unfold-0.6.0/src/unfold/templates/unfold/helpers/search_results.html
+-rw-r--r--   0        0        0      442 2023-04-25 16:53:58.844252 django_unfold-0.6.0/src/unfold/templates/unfold/helpers/site_icon.html
+-rw-r--r--   0        0        0     2038 2023-05-12 17:59:11.450664 django_unfold-0.6.0/src/unfold/templates/unfold/helpers/tab_list.html
+-rw-r--r--   0        0        0     4895 2023-04-25 16:53:58.844537 django_unfold-0.6.0/src/unfold/templates/unfold/helpers/userlinks.html
+-rw-r--r--   0        0        0     1120 2023-04-25 16:53:58.844676 django_unfold-0.6.0/src/unfold/templates/unfold/helpers/welcomemsg.html
+-rw-r--r--   0        0        0      859 2023-04-25 16:53:58.844811 django_unfold-0.6.0/src/unfold/templates/unfold/layouts/base_simple.html
+-rw-r--r--   0        0        0     3149 2023-05-12 17:59:11.450883 django_unfold-0.6.0/src/unfold/templates/unfold/layouts/skeleton.html
+-rw-r--r--   0        0        0     2218 2023-05-12 17:59:11.451078 django_unfold-0.6.0/src/unfold/templates/unfold/widgets/clearable_file_input_small.html
+-rw-r--r--   0        0        0       88 2023-04-25 16:53:58.845218 django_unfold-0.6.0/src/unfold/templates/unfold/widgets/date.html
+-rw-r--r--   0        0        0      262 2023-04-25 16:53:58.845347 django_unfold-0.6.0/src/unfold/templates/unfold/widgets/range.html
+-rw-r--r--   0        0        0      881 2023-04-25 16:53:58.845482 django_unfold-0.6.0/src/unfold/templates/unfold/widgets/split_datetime_vertical.html
+-rw-r--r--   0        0        0      459 2023-04-25 16:53:58.845611 django_unfold-0.6.0/src/unfold/templates/unfold/widgets/textarea.html
+-rw-r--r--   0        0        0       88 2023-04-25 16:53:58.845754 django_unfold-0.6.0/src/unfold/templates/unfold/widgets/time.html
+-rw-r--r--   0        0        0        0 2023-04-25 16:53:58.845896 django_unfold-0.6.0/src/unfold/templatetags/__init__.py
+-rw-r--r--   0        0        0     3559 2023-05-12 17:59:11.451293 django_unfold-0.6.0/src/unfold/templatetags/unfold.py
+-rw-r--r--   0        0        0    10012 2023-04-29 14:41:34.284613 django_unfold-0.6.0/src/unfold/templatetags/unfold_list.py
+-rw-r--r--   0        0        0      576 2023-04-29 14:41:34.284745 django_unfold-0.6.0/src/unfold/typing.py
+-rw-r--r--   0        0        0     3878 2023-04-29 14:41:34.285023 django_unfold-0.6.0/src/unfold/utils.py
+-rw-r--r--   0        0        0      708 2023-04-29 14:41:34.285153 django_unfold-0.6.0/src/unfold/views.py
+-rw-r--r--   0        0        0     8150 2023-05-12 17:59:11.451628 django_unfold-0.6.0/src/unfold/widgets.py
+-rw-r--r--   0        0        0    27827 1970-01-01 00:00:00.000000 django_unfold-0.6.0/setup.py
+-rw-r--r--   0        0        0    26377 1970-01-01 00:00:00.000000 django_unfold-0.6.0/PKG-INFO
```

### Comparing `django_unfold-0.5.3/LICENSE` & `django_unfold-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_unfold-0.5.3/README.md` & `django_unfold-0.6.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -28,14 +28,16 @@
   - [Actions overview](#actions-overview)
   - [Custom unfold @action decorator](#custom-unfold-action-decorator)
   - [Action handler functions](#action-handler-functions)
     - [For submit row action](#for-submit-row-action)
     - [For global, row and detail action](#for-global-row-and-detail-action)
   - [Action examples](#action-examples)
 - [Filters](#filters)
+- [Third party packages](#third-party-packages)
+  - [django-import-export](#django-import-export)
 - [User Admin Form](#user-admin-form)
 - [Adding Custom Styles and Scripts](#adding-custom-styles-and-scripts)
 - [Project Level Tailwind Stylesheet](#project-level-tailwind-stylesheet)
 - [Custom Admin Dashboard](#custom-admin-dashboard)
 - [Unfold Development](#unfold-development)
   - [Pre-commit](#pre-commit)
   - [Poetry Configuration](#poetry-configuration)
@@ -48,14 +50,15 @@
 ```python
 # settings.py
 
 INSTALLED_APPS = [
     "unfold",  # before django.contrib.admin
     "unfold.contrib.filters",  # optional, if special filters are needed
     "unfold.contrib.forms",  # optional, if special form elements are needed
+    "unfold.contrib.import_export",  # optional, if django-import-export package is used
     "django.contrib.admin",  # required
 ]
 ```
 
 In case you need installation command below are the versions for `pip` and `poetry` which needs to be executed in shell.
 
 ```bash
@@ -481,14 +484,32 @@
     )
 
     def get_queryset(self, request):
         return super().get_queryset().annotate(items_count=Count("item", distinct=True))
 ```
 
 
+## Third party packages
+
+
+### django-import-export
+
+To get proper visual appearance for django-import-export, two things are needed
+
+1. Add `unfold.contrib.import_export` to `INSTALLED_APPS` at the begging of the file. This action will override all templates coming from the plugin.
+2. Change `import_form_class` and `export_form_class` in ModelAdmin which is inheriting from `ImportExportModelAdmin`. This chunk of code is responsible for adding proper styling to form elements.
+
+```python
+from unfold.admin import ModelAdmin
+from unfold.contrib.import_export.forms import ExportForm, ImportForm
+
+class ExampleAdmin(ModelAdmin, ImportExportModelAdmin):
+    import_form_class = ImportForm
+    export_form_class = ExportForm
+```
 
 ## User Admin Form
 
 User's admin in Django is specific as it contains several forms which are requiring custom styling. All of these forms has been inherited and accordingly adjusted. In user admin class it is needed to use these inherited form classes to enable custom styling matching rest of the website.
 
 ```python
 # models.py
```

### Comparing `django_unfold-0.5.3/pyproject.toml` & `django_unfold-0.6.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [tool.poetry]
 name = "django-unfold"
-version = "0.5.3"
+version = "0.6.0"
 description = "Clean & minimal Django admin theme based on Tailwind CSS"
 license = "MIT"
 readme = "README.md"
 authors = []
-homepage = "https://github.com/remastr/django-unfold"
+homepage = "https://unfoldadmin.com"
 repository = "https://github.com/remastr/django-unfold"
 packages = [
     { include = "unfold", from = "src" },
 ]
 keywords = [
     "django",
     "admin",
```

### Comparing `django_unfold-0.5.3/src/unfold/admin.py` & `django_unfold-0.6.0/src/unfold/admin.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,41 +1,55 @@
 import copy
 from functools import update_wrapper
+from typing import Any, Callable, Dict, List, Optional, Tuple
 
 from django import forms
 from django.contrib.admin import ModelAdmin as BaseModelAdmin
 from django.contrib.admin import StackedInline as BaseStackedInline
 from django.contrib.admin import TabularInline as BaseTabularInline
 from django.contrib.admin import display, helpers
 from django.contrib.admin.utils import lookup_field
 from django.core.exceptions import ObjectDoesNotExist
 from django.db import models
 from django.db.models import (
     BLANK_CHOICE_DASH,
     ForeignObjectRel,
     ManyToManyRel,
+    Model,
     OneToOneField,
 )
+from django.db.models.fields import Field
+from django.db.models.fields.related import ForeignKey, ManyToManyField
+from django.forms import Form
+from django.forms.fields import TypedChoiceField
+from django.forms.models import (
+    ModelChoiceField,
+    ModelMultipleChoiceField,
+)
 from django.forms.utils import flatatt
 from django.forms.widgets import SelectMultiple
-from django.http import HttpRequest
+from django.http import HttpRequest, HttpResponse
 from django.shortcuts import redirect
 from django.template.defaultfilters import linebreaksbr
-from django.template.loader import render_to_string
-from django.urls import path, reverse
+from django.template.response import TemplateResponse
+from django.urls import URLPattern, path, reverse
 from django.utils.html import conditional_escape, format_html
 from django.utils.module_loading import import_string
-from django.utils.safestring import mark_safe
+from django.utils.safestring import SafeText, mark_safe
 from django.utils.text import capfirst
 from django.utils.translation import gettext_lazy as _
+from django.views import View
 from unfold.utils import display_for_field
 
+from .checks import UnfoldModelAdminChecks
+from .dataclasses import UnfoldAction
 from .exceptions import UnfoldException
 from .forms import ActionForm
 from .settings import get_config
+from .typing import FieldsetsType
 from .widgets import (
     CHECKBOX_LABEL_CLASSES,
     INPUT_CLASSES,
     LABEL_CLASSES,
     SELECT_CLASSES,
     UnfoldAdminBigIntegerFieldWidget,
     UnfoldAdminDecimalFieldWidget,
@@ -100,15 +114,15 @@
     {
         models.ImageField: {"widget": UnfoldAdminImageSmallFieldWidget},
     }
 )
 
 
 class UnfoldAdminField(helpers.AdminField):
-    def label_tag(self):
+    def label_tag(self) -> SafeText:
         classes = []
 
         # TODO load config from current AdminSite (override Fieldline.__iter__ method)
         for lang, flag in get_config()["EXTENSIONS"]["modeltranslation"][
             "flags"
         ].items():
             if f"[{lang}]" in self.field.label:
@@ -135,15 +149,15 @@
         )
 
 
 helpers.AdminField = UnfoldAdminField
 
 
 class UnfoldAdminReadonlyField(helpers.AdminReadonlyField):
-    def label_tag(self):
+    def label_tag(self) -> SafeText:
         attrs = {
             "class": " ".join(LABEL_CLASSES + ["mb-2"]),
         }
 
         if not self.is_first:
             attrs["class"] = "inline"
 
@@ -152,22 +166,22 @@
         return format_html(
             "<label{}>{}{}</label>",
             flatatt(attrs),
             capfirst(label),
             self.form.label_suffix,
         )
 
-    def contents(self):
+    def contents(self) -> str:
         contents = self._get_contents()
 
         self._preprocess_field(contents)
 
         return contents
 
-    def _get_contents(self):
+    def _get_contents(self) -> str:
         from django.contrib.admin.templatetags.admin_list import _boolean_icon
 
         field, obj, model_admin = (
             self.field["field"],
             self.form.instance,
             self.model_admin,
         )
@@ -200,15 +214,15 @@
                     result_repr = self.get_admin_url(f.remote_field, value)
                 else:
                     result_repr = display_for_field(value, f, self.empty_value_display)
                     return conditional_escape(result_repr)
                 result_repr = linebreaksbr(result_repr)
         return conditional_escape(result_repr)
 
-    def _preprocess_field(self, contents):
+    def _preprocess_field(self, contents: str) -> str:
         if self.field["field"] in self.model_admin.readonly_preprocess_fields:
             func = self.model_admin.readonly_preprocess_fields[self.field["field"]]
 
             if isinstance(func, str):
                 contents = import_string(func)(contents)
             elif callable(func):
                 contents = func(contents)
@@ -226,25 +240,29 @@
         for k, v in self.formfield_overrides.items():
             overrides.setdefault(k, {}).update(v)
 
         self.formfield_overrides = overrides
 
         super().__init__(model, admin_site)
 
-    def formfield_for_choice_field(self, db_field, request: HttpRequest, **kwargs):
+    def formfield_for_choice_field(
+        self, db_field: Field, request: HttpRequest, **kwargs
+    ) -> TypedChoiceField:
         # Overrides widget for CharFields which have choices attribute
         if "widget" not in kwargs:
             kwargs["widget"] = forms.Select(attrs={"class": " ".join(SELECT_CLASSES)})
             kwargs["choices"] = db_field.get_choices(
                 include_blank=db_field.blank, blank_choice=[("", _("Select value"))]
             )
 
         return super().formfield_for_choice_field(db_field, request, **kwargs)
 
-    def formfield_for_foreignkey(self, db_field, request, **kwargs):
+    def formfield_for_foreignkey(
+        self, db_field: ForeignKey[Any], request: HttpRequest, **kwargs
+    ) -> Optional[ModelChoiceField]:
         # Overrides widgets for all related fields
         if "widget" not in kwargs:
             if db_field.name in self.raw_id_fields:
                 kwargs["widget"] = forms.TextInput(
                     attrs={"class": " ".join(INPUT_CLASSES)}
                 )
             elif (
@@ -254,15 +272,20 @@
                 kwargs["widget"] = forms.Select(
                     attrs={"class": " ".join(SELECT_CLASSES)}
                 )
                 kwargs["empty_label"] = _("Select value")
 
         return super().formfield_for_foreignkey(db_field, request, **kwargs)
 
-    def formfield_for_manytomany(self, db_field, request, **kwargs):
+    def formfield_for_manytomany(
+        self,
+        db_field: ManyToManyField,
+        request: HttpRequest,
+        **kwargs,
+    ) -> ModelMultipleChoiceField:
         if "widget" not in kwargs:
             if db_field.name in self.raw_id_fields:
                 kwargs["widget"] = forms.TextInput(
                     attrs={"class": " ".join(INPUT_CLASSES)}
                 )
 
         form_field = super().formfield_for_manytomany(db_field, request, **kwargs)
@@ -272,23 +295,27 @@
             return None
 
         if isinstance(form_field.widget, SelectMultiple):
             form_field.widget.attrs["class"] = " ".join(SELECT_CLASSES)
 
         return form_field
 
-    def formfield_for_nullboolean_field(self, db_field, request, **kwargs):
+    def formfield_for_nullboolean_field(
+        self, db_field: Field, request: HttpRequest, **kwargs
+    ) -> Optional[Field]:
         if "widget" not in kwargs:
             kwargs["widget"] = forms.NullBooleanSelect(
                 attrs={"class": " ".join(SELECT_CLASSES)}
             )
 
         return db_field.formfield(**kwargs)
 
-    def formfield_for_dbfield(self, db_field, request, **kwargs):
+    def formfield_for_dbfield(
+        self, db_field: Field, request: HttpRequest, **kwargs
+    ) -> Optional[Field]:
         if isinstance(db_field, models.BooleanField) and db_field.null is True:
             return self.formfield_for_nullboolean_field(db_field, request, **kwargs)
 
         return super().formfield_for_dbfield(db_field, request, **kwargs)
 
 
 class ModelAdmin(ModelAdminMixin, BaseModelAdmin):
@@ -297,14 +324,15 @@
     actions_row = ()
     actions_detail = ()
     actions_submit_line = ()
     custom_urls = ()
     add_fieldsets = ()
     list_filter_submit = False
     readonly_preprocess_fields = {}
+    checks_class = UnfoldModelAdminChecks
 
     @property
     def media(self):
         media = super().media
         additional_media = forms.Media()
 
         for filter in self.list_filter:
@@ -314,43 +342,92 @@
             if hasattr(filter[1], "form_class") and hasattr(
                 filter[1].form_class, "Media"
             ):
                 additional_media += forms.Media(filter[1].form_class.Media)
 
         return media + additional_media
 
-    def get_fieldsets(self, request, obj=None):
+    def get_fieldsets(self, request: HttpRequest, obj=None) -> FieldsetsType:
         if not obj and self.add_fieldsets:
             return self.add_fieldsets
         return super().get_fieldsets(request, obj)
 
-    def get_actions_list(self):
+    def _filter_unfold_actions_by_permissions(
+        self, request: HttpRequest, actions: List[UnfoldAction]
+    ) -> List[UnfoldAction]:
+        """Filter out any Unfold actions that the user doesn't have access to."""
+        filtered_actions = []
+        for action in actions:
+            if not hasattr(action.method, "allowed_permissions"):
+                filtered_actions.append(action)
+                continue
+            permission_checks = (
+                getattr(self, "has_%s_permission" % permission)
+                for permission in action.method.allowed_permissions
+            )
+            if any(has_permission(request) for has_permission in permission_checks):
+                filtered_actions.append(action)
+        return filtered_actions
+
+    def get_actions_list(self, request: HttpRequest) -> List[UnfoldAction]:
+        return self._filter_unfold_actions_by_permissions(
+            request, self._get_base_actions_list()
+        )
+
+    def _get_base_actions_list(self) -> List[UnfoldAction]:
+        """
+        Returns all available list global actions, prior to any filtering
+        """
         return [self.get_unfold_action(action) for action in self.actions_list or []]
 
-    def get_actions_detail(self):
+    def get_actions_detail(self, request: HttpRequest) -> List[UnfoldAction]:
+        return self._filter_unfold_actions_by_permissions(
+            request, self._get_base_actions_detail()
+        )
+
+    def _get_base_actions_detail(self) -> List[UnfoldAction]:
+        """
+        Returns all available detail actions, prior to any filtering
+        """
         return [self.get_unfold_action(action) for action in self.actions_detail or []]
 
-    def get_actions_row(self):
+    def get_actions_row(self, request: HttpRequest) -> List[UnfoldAction]:
+        return self._filter_unfold_actions_by_permissions(
+            request, self._get_base_actions_row()
+        )
+
+    def _get_base_actions_row(self) -> List[UnfoldAction]:
+        """
+        Returns all available row actions, prior to any filtering
+        """
         return [self.get_unfold_action(action) for action in self.actions_row or []]
 
-    def get_actions_submit_line(self):
+    def get_actions_submit_line(self, request: HttpRequest) -> List[UnfoldAction]:
+        return self._filter_unfold_actions_by_permissions(
+            request, self._get_base_actions_submit_line()
+        )
+
+    def _get_base_actions_submit_line(self) -> List[UnfoldAction]:
+        """
+        Returns all available submit row actions, prior to any filtering
+        """
         return [
             self.get_unfold_action(action) for action in self.actions_submit_line or []
         ]
 
-    def get_custom_urls(self):
+    def get_custom_urls(self) -> Tuple[Tuple[str, str, View], ...]:
         """
         Method to get custom views for ModelAdmin with their urls
 
         Format of custom_urls item:
             ("path_to_view", "name_of_view", view_itself)
         """
         return () if self.custom_urls is None else self.custom_urls
 
-    def get_urls(self):
+    def get_urls(self) -> List[URLPattern]:
         urls = super().get_urls()
 
         def wrap(view):
             def wrapper(*args, **kwargs):
                 return self.admin_site.admin_view(view)(*args, **kwargs)
 
             wrapper.model_admin = self
@@ -359,173 +436,191 @@
         custom_urls = [
             self._path_from_custom_url(custom_url)
             for custom_url in self.get_custom_urls()
         ]
 
         actions_list_urls = [
             path(
-                action["path"],
-                wrap(action["method"]),
-                name=action["action_name"],
+                action.path,
+                wrap(action.method),
+                name=action.action_name,
             )
-            for action in self.get_actions_list()
+            for action in self._get_base_actions_list()
         ]
 
         action_detail_urls = [
             path(
-                f"<path:object_id>/{action['path']}/",
-                wrap(action["method"]),
-                name=action["action_name"],
+                f"<path:object_id>/{action.path}/",
+                wrap(action.method),
+                name=action.action_name,
             )
-            for action in self.get_actions_detail()
+            for action in self._get_base_actions_detail()
         ]
 
         action_row_urls = [
             path(
-                f"<path:object_id>/{action['path']}",
-                wrap(action["method"]),
-                name=action["action_name"],
+                f"<path:object_id>/{action.path}",
+                wrap(action.method),
+                name=action.action_name,
             )
-            for action in self.get_actions_row()
+            for action in self._get_base_actions_row()
         ]
 
         return (
             custom_urls
             + action_row_urls
             + actions_list_urls
             + action_detail_urls
             + urls
         )
 
-    def _path_from_custom_url(self, custom_url):
+    def _path_from_custom_url(self, custom_url) -> URLPattern:
         # TODO: wrap()
         return path(
             custom_url[0],
             self.admin_site.admin_view(custom_url[2]),
             {"model_admin": self},
             name=custom_url[1],
         )
 
-    @display(description="")
-    def actions_holder(self, instance):
-        actions = [
-            {
-                "title": action["description"],
-                "attrs": action["method"].attrs,
-                "path": reverse(f"admin:{action['action_name']}", args=(instance.pk,)),
-            }
-            for action in self.get_actions_row()
-        ]
-        return render_to_string(
-            "unfold/helpers/actions_row.html",
-            context={
-                "instance": instance,
-                "actions": actions,
-            },
-        )
-
-    def get_list_display(self, request):
-        if len(self.get_actions_row()) > 0:
-            return [*super().get_list_display(request), "actions_holder"]
-        return super().get_list_display(request)
-
-    def changeform_view(self, request, object_id=None, form_url="", extra_context=None):
+    def changeform_view(
+        self,
+        request: HttpRequest,
+        object_id: Optional[str] = None,
+        form_url: str = "",
+        extra_context: Optional[Dict[str, bool]] = None,
+    ) -> Any:
         if extra_context is None:
             extra_context = {}
 
         actions = []
         if object_id:
-            for action in self.get_actions_detail():
+            for action in self.get_actions_detail(request):
                 actions.append(
                     {
-                        "title": action["description"],
-                        "attrs": action["method"].attrs,
+                        "title": action.description,
+                        "attrs": action.method.attrs,
                         "path": reverse(
-                            f"admin:{action['action_name']}", args=(object_id,)
+                            f"admin:{action.action_name}", args=(object_id,)
                         ),
                     }
                 )
 
         extra_context.update(
             {
-                "actions_submit_line": self.get_actions_submit_line(),
+                "actions_submit_line": self.get_actions_submit_line(request),
                 "actions_detail": actions,
             }
         )
 
         return super().changeform_view(request, object_id, form_url, extra_context)
 
-    def changelist_view(self, request, extra_context=None):
+    def changelist_view(
+        self, request: HttpRequest, extra_context: Optional[Dict[str, str]] = None
+    ) -> TemplateResponse:
         if extra_context is None:
             extra_context = {}
 
         actions = [
             {
-                "title": action["description"],
-                "attrs": action["method"].attrs,
-                "path": reverse(f"admin:{action['action_name']}"),
+                "title": action.description,
+                "attrs": action.method.attrs,
+                "path": reverse(f"admin:{action.action_name}"),
             }
-            for action in self.get_actions_list()
+            for action in self.get_actions_list(request)
         ]
 
-        extra_context.update({"actions_list": actions})
+        actions_row = [
+            {
+                "title": action.description,
+                "attrs": action.method.attrs,
+                "raw_path": f"admin:{action.action_name}",
+            }
+            for action in self.get_actions_row(request)
+        ]
+
+        extra_context.update({"actions_list": actions, "actions_row": actions_row})
 
         return super().changelist_view(request, extra_context)
 
-    def get_unfold_action(self, action):
+    def get_unfold_action(self, action: str) -> UnfoldAction:
+        """
+        Converts action name to UnfoldAction
+        :param action:
+        :return:
+        """
         method = self._get_instance_method(action)
 
-        return {
-            "action_name": f"{self.model._meta.app_label}_{self.model._meta.model_name}_{action}",
-            "method": method,
-            "description": self._get_action_description(method, action),
-            "path": self._get_action_url(method, action),
-        }
+        return UnfoldAction(
+            action_name=f"{self.model._meta.app_label}_{self.model._meta.model_name}_{action}",
+            method=method,
+            description=self._get_action_description(method, action),
+            path=self._get_action_url(method, action),
+        )
 
     @staticmethod
-    def _get_action_url(func, name):
+    def _get_action_url(func: Callable, name: str) -> str:
+        """
+        Returns action URL if it was specified in @action decorator.
+        If it was not, name of the action is returned.
+        :param func:
+        :param name:
+        :return:
+        """
         return getattr(func, "url_path", name)
 
-    def save_model(self, request, obj, form, change):
+    def save_model(
+        self, request: HttpRequest, obj: Model, form: Form, change: Any
+    ) -> None:
         super().save_model(request, obj, form, change)
 
-        for action_attrs in self.get_actions_submit_line():
-            if action_attrs["action_name"] not in request.POST:
+        for action in self.get_actions_submit_line(request):
+            if action.action_name not in request.POST:
                 continue
 
-            action_attrs["method"](request, obj)
+            action.method(request, obj)
 
-    def _get_instance_method(self, method_name):
+    def _get_instance_method(self, method_name: str) -> Callable:
+        """
+        Searches for method on self instance based on method_name and returns it if it exists.
+        If it does not exist or is not callable, it raises UnfoldException
+        :param method_name: Name of the method to search for
+        :return: method from self instance
+        """
         try:
             method = getattr(self, method_name)
         except AttributeError as e:
             raise UnfoldException(
                 f"Method {method_name} specified does not exist on current object"
             ) from e
 
         if not callable(method):
             raise UnfoldException(f"{method_name} is not callable")
 
         return method
 
-    def get_action_choices(self, request, default_choices=BLANK_CHOICE_DASH):
+    def get_action_choices(
+        self, request: HttpRequest, default_choices=BLANK_CHOICE_DASH
+    ):
         default_choices = [("", _("Select action"))]
         return super().get_action_choices(request, default_choices)
 
     @display(description=mark_safe('<input type="checkbox" id="action-toggle">'))
-    def action_checkbox(self, obj):
+    def action_checkbox(self, obj: Model):
         return checkbox.render(helpers.ACTION_CHECKBOX_NAME, str(obj.pk))
 
-    def response_change(self, request, obj):
+    def response_change(self, request: HttpRequest, obj: Model) -> HttpResponse:
         res = super().response_change(request, obj)
         if "next" in request.GET:
             return redirect(request.GET["next"])
         return res
 
-    def response_add(self, request, obj, post_url_continue=None):
+    def response_add(
+        self, request: HttpRequest, obj: Model, post_url_continue: Optional[str] = None
+    ) -> HttpResponse:
         res = super().response_add(request, obj, post_url_continue)
         if "next" in request.GET:
             return redirect(request.GET["next"])
         return res
 
 
 class TabularInline(ModelAdminMixin, BaseTabularInline):
```

### Comparing `django_unfold-0.5.3/src/unfold/contrib/filters/admin.py` & `django_unfold-0.6.0/src/unfold/contrib/filters/admin.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,24 @@
+from typing import Any, Dict, List, Optional, Tuple, Type
+
 from django.contrib import admin
+from django.contrib.admin.options import ModelAdmin
+from django.contrib.admin.views.main import ChangeList
 from django.core.validators import EMPTY_VALUES
-from django.db.models import Max, Min
+from django.db.models import Max, Min, Model, QuerySet
 from django.db.models.fields import (
     AutoField,
     DateField,
     DateTimeField,
     DecimalField,
+    Field,
     FloatField,
     IntegerField,
 )
+from django.http import HttpRequest
 from django.utils.dateparse import parse_datetime
 
 from .forms import (
     RangeDateForm,
     RangeDateTimeForm,
     RangeNumericForm,
     SingleNumericForm,
@@ -21,15 +27,23 @@
 
 
 class SingleNumericFilter(admin.FieldListFilter):
     request = None
     parameter_name = None
     template = "unfold/filters/filters_numeric_single.html"
 
-    def __init__(self, field, request, params, model, model_admin, field_path):
+    def __init__(
+        self,
+        field: Field,
+        request: HttpRequest,
+        params: Dict[str, str],
+        model: Type[Model],
+        model_admin: ModelAdmin,
+        field_path: str,
+    ) -> None:
         super().__init__(field, request, params, model, model_admin, field_path)
 
         if not isinstance(field, (DecimalField, IntegerField, FloatField, AutoField)):
             raise TypeError(
                 "Class {} is not supported for {}.".format(
                     type(self.field), self.__class__.__name__
                 )
@@ -40,25 +54,27 @@
         if self.parameter_name is None:
             self.parameter_name = self.field_path
 
         if self.parameter_name in params:
             value = params.pop(self.parameter_name)
             self.used_parameters[self.parameter_name] = value
 
-    def queryset(self, request, queryset):
+    def queryset(
+        self, request: HttpRequest, queryset: QuerySet[Any]
+    ) -> Optional[QuerySet]:
         if self.value():
             return queryset.filter(**{self.parameter_name: self.value()})
 
-    def value(self):
+    def value(self) -> Any:
         return self.used_parameters.get(self.parameter_name, None)
 
-    def expected_parameters(self):
+    def expected_parameters(self) -> List[Optional[str]]:
         return [self.parameter_name]
 
-    def choices(self, changelist):
+    def choices(self, changelist: ChangeList) -> Tuple[Dict[str, Any], ...]:
         return (
             {
                 "request": self.request,
                 "parameter_name": self.parameter_name,
                 "form": SingleNumericForm(
                     name=self.parameter_name, data={self.parameter_name: self.value()}
                 ),
@@ -67,24 +83,24 @@
 
 
 class RangeNumericMixin:
     request = None
     parameter_name = None
     template = "unfold/filters/filters_numeric_range.html"
 
-    def init_used_parameters(self, params):
+    def init_used_parameters(self, params: Dict[str, Any]) -> None:
         if self.parameter_name + "_from" in params:
             value = params.pop(self.parameter_name + "_from")
             self.used_parameters[self.parameter_name + "_from"] = value
 
         if self.parameter_name + "_to" in params:
             value = params.pop(self.parameter_name + "_to")
             self.used_parameters[self.parameter_name + "_to"] = value
 
-    def queryset(self, request, queryset):
+    def queryset(self, request: HttpRequest, queryset: QuerySet) -> QuerySet:
         filters = {}
 
         value_from = self.used_parameters.get(self.parameter_name + "_from", None)
         if value_from is not None and value_from != "":
             filters.update(
                 {
                     self.parameter_name
@@ -103,21 +119,21 @@
                         self.parameter_name + "_to", None
                     ),
                 }
             )
 
         return queryset.filter(**filters)
 
-    def expected_parameters(self):
+    def expected_parameters(self) -> List[str]:
         return [
             f"{self.parameter_name}_from",
             f"{self.parameter_name}_to",
         ]
 
-    def choices(self, changelist):
+    def choices(self, changelist: ChangeList) -> Tuple[Dict[str, Any], ...]:
         return (
             {
                 "request": self.request,
                 "parameter_name": self.parameter_name,
                 "form": RangeNumericForm(
                     name=self.parameter_name,
                     data={
@@ -132,28 +148,44 @@
                     },
                 ),
             },
         )
 
 
 class RangeNumericListFilter(RangeNumericMixin, admin.SimpleListFilter):
-    def __init__(self, request, params, model, model_admin):
+    def __init__(
+        self,
+        request: HttpRequest,
+        params: Dict[str, str],
+        model: Type[Model],
+        model_admin: ModelAdmin,
+    ) -> None:
         super().__init__(request, params, model, model_admin)
         if not self.parameter_name:
             raise ValueError("Parameter name cannot be None")
 
         self.request = request
         self.init_used_parameters(params)
 
-    def lookups(self, request, model_admin):
+    def lookups(
+        self, request: HttpRequest, model_admin: ModelAdmin
+    ) -> Tuple[Tuple[str, str], ...]:
         return (("dummy", "dummy"),)
 
 
 class RangeNumericFilter(RangeNumericMixin, admin.FieldListFilter):
-    def __init__(self, field, request, params, model, model_admin, field_path):
+    def __init__(
+        self,
+        field: Field,
+        request: HttpRequest,
+        params: Dict[str, str],
+        model: Type[Model],
+        model_admin: ModelAdmin,
+        field_path: str,
+    ) -> None:
         super().__init__(field, request, params, model, model_admin, field_path)
         if not isinstance(field, (DecimalField, IntegerField, FloatField, AutoField)):
             raise TypeError(
                 "Class {} is not supported for {}.".format(
                     type(self.field), self.__class__.__name__
                 )
             )
@@ -169,21 +201,29 @@
     MAX_DECIMALS = 7
     STEP = None
 
     template = "unfold/filters/filters_numeric_slider.html"
     field = None
     form_class = SliderNumericForm
 
-    def __init__(self, field, request, params, model, model_admin, field_path):
+    def __init__(
+        self,
+        field: Field,
+        request: HttpRequest,
+        params: Dict[str, str],
+        model: Type[Model],
+        model_admin: ModelAdmin,
+        field_path: str,
+    ) -> None:
         super().__init__(field, request, params, model, model_admin, field_path)
 
         self.field = field
         self.q = model_admin.get_queryset(request)
 
-    def choices(self, changelist):
+    def choices(self, changelist: ChangeList) -> Tuple[Dict[str, Any], ...]:
         total = self.q.all().count()
         min_value = self.q.all().aggregate(min=Min(self.parameter_name)).get("min", 0)
 
         if total > 1:
             max_value = (
                 self.q.all().aggregate(max=Max(self.parameter_name)).get("max", 0)
             )
@@ -223,26 +263,34 @@
                             self.parameter_name + "_to", max_value
                         ),
                     },
                 ),
             },
         )
 
-    def _get_min_step(self, precision):
+    def _get_min_step(self, precision: int) -> float:
         result_format = f"{{:.{precision - 1}f}}"
         return float(result_format.format(0) + "1")
 
 
 class RangeDateFilter(admin.FieldListFilter):
     request = None
     parameter_name = None
     form_class = RangeDateForm
     template = "unfold/filters/filters_date_range.html"
 
-    def __init__(self, field, request, params, model, model_admin, field_path):
+    def __init__(
+        self,
+        field: Field,
+        request: HttpRequest,
+        params: Dict[str, str],
+        model: Type[Model],
+        model_admin: ModelAdmin,
+        field_path: str,
+    ) -> None:
         super().__init__(field, request, params, model, model_admin, field_path)
         if not isinstance(field, DateField):
             raise TypeError(
                 "Class {} is not supported for {}.".format(
                     type(self.field), self.__class__.__name__
                 )
             )
@@ -255,15 +303,15 @@
             value = params.pop(self.field_path + "_from")
             self.used_parameters[self.field_path + "_from"] = value
 
         if self.parameter_name + "_to" in params:
             value = params.pop(self.field_path + "_to")
             self.used_parameters[self.field_path + "_to"] = value
 
-    def queryset(self, request, queryset):
+    def queryset(self, request: HttpRequest, queryset: QuerySet) -> QuerySet:
         filters = {}
 
         value_from = self.used_parameters.get(self.parameter_name + "_from", None)
         if value_from not in EMPTY_VALUES:
             filters.update(
                 {
                     self.parameter_name
@@ -282,21 +330,21 @@
                         self.parameter_name + "_to", None
                     ),
                 }
             )
 
         return queryset.filter(**filters)
 
-    def expected_parameters(self):
+    def expected_parameters(self) -> List[str]:
         return [
             f"{self.parameter_name}_from",
             f"{self.parameter_name}_to",
         ]
 
-    def choices(self, changelist):
+    def choices(self, changelist: ChangeList) -> Tuple[Dict[str, Any], ...]:
         return (
             {
                 "request": self.request,
                 "parameter_name": self.parameter_name,
                 "form": self.form_class(
                     name=self.parameter_name,
                     data={
@@ -316,15 +364,23 @@
 
 class RangeDateTimeFilter(admin.FieldListFilter):
     request = None
     parameter_name = None
     template = "unfold/filters/filters_datetime_range.html"
     form_class = RangeDateTimeForm
 
-    def __init__(self, field, request, params, model, model_admin, field_path):
+    def __init__(
+        self,
+        field: Field,
+        request: HttpRequest,
+        params: Dict[str, str],
+        model: Type[Model],
+        model_admin: ModelAdmin,
+        field_path: str,
+    ) -> None:
         super().__init__(field, request, params, model, model_admin, field_path)
         if not isinstance(field, DateTimeField):
             raise TypeError(
                 "Class {} is not supported for {}.".format(
                     type(self.field), self.__class__.__name__
                 )
             )
@@ -345,23 +401,23 @@
             value = params.pop(self.field_path + "_to_0")
             self.used_parameters[self.field_path + "_to_0"] = value
 
         if self.parameter_name + "_to_1" in params:
             value = params.pop(self.field_path + "_to_1")
             self.used_parameters[self.field_path + "_to_1"] = value
 
-    def expected_parameters(self):
+    def expected_parameters(self) -> List[str]:
         return [
             f"{self.parameter_name}_from_0",
             f"{self.parameter_name}_from_1",
             f"{self.parameter_name}_to_0",
             f"{self.parameter_name}_to_1",
         ]
 
-    def queryset(self, request, queryset):
+    def queryset(self, request: HttpRequest, queryset: QuerySet) -> QuerySet:
         filters = {}
 
         date_value_from = self.used_parameters.get(
             self.parameter_name + "_from_0", None
         )
         time_value_from = self.used_parameters.get(
             self.parameter_name + "_from_1", None
@@ -385,15 +441,15 @@
                         f"{date_value_to}T{time_value_to}"
                     ),
                 }
             )
 
         return queryset.filter(**filters)
 
-    def choices(self, changelist):
+    def choices(self, changelist: ChangeList) -> Tuple[Dict[str, Any], ...]:
         return (
             {
                 "request": self.request,
                 "parameter_name": self.parameter_name,
                 "form": self.form_class(
                     name=self.parameter_name,
                     data={
```

### Comparing `django_unfold-0.5.3/src/unfold/contrib/filters/forms.py` & `django_unfold-0.6.0/src/unfold/contrib/filters/forms.py`

 * *Files identical despite different names*

### Comparing `django_unfold-0.5.3/src/unfold/contrib/filters/static/unfold/filters/css/nouislider.min.css` & `django_unfold-0.6.0/src/unfold/contrib/filters/static/unfold/filters/css/nouislider.min.css`

 * *Files identical despite different names*

### Comparing `django_unfold-0.5.3/src/unfold/contrib/filters/static/unfold/filters/js/DateTimeShortcuts.js` & `django_unfold-0.6.0/src/unfold/contrib/filters/static/unfold/filters/js/DateTimeShortcuts.js`

 * *Files identical despite different names*

### Comparing `django_unfold-0.5.3/src/unfold/contrib/filters/static/unfold/filters/js/admin-numeric-filter.js` & `django_unfold-0.6.0/src/unfold/contrib/filters/static/unfold/filters/js/admin-numeric-filter.js`

 * *Files identical despite different names*

### Comparing `django_unfold-0.5.3/src/unfold/contrib/filters/static/unfold/filters/js/nouislider.min.js` & `django_unfold-0.6.0/src/unfold/contrib/filters/static/unfold/filters/js/nouislider.min.js`

 * *Files identical despite different names*

### Comparing `django_unfold-0.5.3/src/unfold/contrib/filters/static/unfold/filters/js/wNumb.min.js` & `django_unfold-0.6.0/src/unfold/contrib/filters/static/unfold/filters/js/wNumb.min.js`

 * *Files identical despite different names*

### Comparing `django_unfold-0.5.3/src/unfold/contrib/filters/templates/unfold/filters/filters_numeric_slider.html` & `django_unfold-0.6.0/src/unfold/contrib/filters/templates/unfold/filters/filters_numeric_slider.html`

 * *Files identical despite different names*

### Comparing `django_unfold-0.5.3/src/unfold/contrib/forms/static/unfold/forms/css/trix.css` & `django_unfold-0.6.0/src/unfold/contrib/forms/static/unfold/forms/css/trix.css`

 * *Files identical despite different names*

### Comparing `django_unfold-0.5.3/src/unfold/contrib/forms/static/unfold/forms/js/trix.config.js` & `django_unfold-0.6.0/src/unfold/contrib/forms/static/unfold/forms/js/trix.config.js`

 * *Files identical despite different names*

### Comparing `django_unfold-0.5.3/src/unfold/contrib/forms/static/unfold/forms/js/trix.js` & `django_unfold-0.6.0/src/unfold/contrib/forms/static/unfold/forms/js/trix.js`

 * *Files identical despite different names*

### Comparing `django_unfold-0.5.3/src/unfold/contrib/forms/templates/unfold/forms/helpers/toolbar.html` & `django_unfold-0.6.0/src/unfold/contrib/forms/templates/unfold/forms/helpers/toolbar.html`

 * *Files identical despite different names*

### Comparing `django_unfold-0.5.3/src/unfold/settings.py` & `django_unfold-0.6.0/src/unfold/settings.py`

 * *Files identical despite different names*

### Comparing `django_unfold-0.5.3/src/unfold/sites.py` & `django_unfold-0.6.0/src/unfold/sites.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 from http import HTTPStatus
+from typing import Any, Callable, Dict, List, Optional, Union
 
 from django.contrib.admin import AdminSite
 from django.contrib.auth import REDIRECT_FIELD_NAME
 from django.core.validators import EMPTY_VALUES
-from django.http import HttpResponse
+from django.http import HttpRequest, HttpResponse
 from django.template.response import TemplateResponse
-from django.urls import path, reverse, reverse_lazy
+from django.urls import URLPattern, path, reverse, reverse_lazy
 from django.utils.module_loading import import_string
 
 from .settings import get_config
 
 
 class UnfoldAdminSite(AdminSite):
     default_site = "unfold.admin.UnfoldAdminSite"
     settings_name = "UNFOLD"
 
-    def __init__(self, name="admin"):
+    def __init__(self, name: str = "admin") -> None:
         from .forms import AuthenticationForm
 
         super().__init__(name)
 
         if self.login_form is None:
             self.login_form = AuthenticationForm
 
@@ -28,27 +29,27 @@
 
         if get_config(self.settings_name)["SITE_HEADER"]:
             self.site_header = get_config(self.settings_name)["SITE_HEADER"]
 
         if get_config(self.settings_name)["SITE_URL"]:
             self.site_url = get_config(self.settings_name)["SITE_URL"]
 
-    def get_urls(self):
+    def get_urls(self) -> List[URLPattern]:
         urlpatterns = [
             path("search/", self.admin_view(self.search), name="search"),
             path(
                 "toggle-sidebar/",
                 self.admin_view(self.toggle_sidebar),
                 name="toggle_sidebar",
             ),
         ] + super().get_urls()
 
         return urlpatterns
 
-    def each_context(self, request):
+    def each_context(self, request: HttpRequest) -> Dict[str, Any]:
         context = super().each_context(request)
 
         context.update(
             {
                 "logo": self._get_value(
                     get_config(self.settings_name)["SIDEBAR"].get("logo"), request
                 ),
@@ -78,15 +79,17 @@
                 if self.has_permission(request)
                 else [],
             }
         )
 
         return context
 
-    def index(self, request, extra_context=None):
+    def index(
+        self, request: HttpRequest, extra_context: Optional[Dict[str, Any]] = None
+    ) -> TemplateResponse:
         app_list = self.get_app_list(request)
 
         context = {
             **self.each_context(request),
             "title": self.index_title,
             "subtitle": None,
             "app_list": app_list,
@@ -101,23 +104,27 @@
 
         request.current_app = self.name
 
         return TemplateResponse(
             request, self.index_template or "admin/index.html", context
         )
 
-    def toggle_sidebar(self, request, extra_context=None):
+    def toggle_sidebar(
+        self, request: HttpRequest, extra_context: Optional[Dict[str, Any]] = None
+    ) -> HttpResponse:
         if "toggle_sidebar" not in request.session:
             request.session["toggle_sidebar"] = True
         else:
             request.session["toggle_sidebar"] = not request.session["toggle_sidebar"]
 
         return HttpResponse(status=HTTPStatus.OK)
 
-    def search(self, request, extra_context=None):
+    def search(
+        self, request: HttpRequest, extra_context: Optional[Dict[str, Any]] = None
+    ) -> TemplateResponse:
         query = request.GET.get("s").lower()
         app_list = super().get_app_list(request)
         results = []
 
         if query in EMPTY_VALUES:
             return HttpResponse()
 
@@ -140,15 +147,17 @@
             request,
             template="unfold/helpers/search_results.html",
             context={
                 "results": results,
             },
         )
 
-    def login(self, request, extra_context=None):
+    def login(
+        self, request: HttpRequest, extra_context: Optional[Dict[str, Any]] = None
+    ) -> HttpResponse:
         extra_context = {} if extra_context is None else extra_context
         image = self._get_value(
             get_config(self.settings_name)["LOGIN"].get("image"), request
         )
 
         redirect_field_name = self._get_value(
             get_config(self.settings_name)["LOGIN"].get("redirect_after"), request
@@ -162,15 +171,17 @@
             )
 
         if redirect_field_name not in EMPTY_VALUES:
             extra_context.update({REDIRECT_FIELD_NAME: redirect_field_name})
 
         return super().login(request, extra_context)
 
-    def password_change(self, request, extra_context=None):
+    def password_change(
+        self, request: HttpRequest, extra_context: Optional[Dict[str, Any]] = None
+    ) -> HttpResponse:
         from django.contrib.auth.views import PasswordChangeView
 
         from .forms import AdminOwnPasswordChangeForm
 
         url = reverse("admin:password_change_done", current_app=self.name)
         defaults = {
             "form_class": AdminOwnPasswordChangeForm,
@@ -178,19 +189,19 @@
             "extra_context": {**self.each_context(request), **(extra_context or {})},
         }
         if self.password_change_template is not None:
             defaults["template_name"] = self.password_change_template
         request.current_app = self.name
         return PasswordChangeView.as_view(**defaults)(request)
 
-    def get_sidebar_list(self, request):
+    def get_sidebar_list(self, request: HttpRequest) -> List[Dict[str, Any]]:
         navigation = get_config(self.settings_name)["SIDEBAR"].get("navigation", [])
         results = []
 
-        def _get_is_active(link):
+        def _get_is_active(link: str) -> bool:
             if not isinstance(link, str):
                 link = str(link)
 
             if link in request.path and link != reverse_lazy("admin:index"):
                 return True
             elif link == request.path == reverse_lazy("admin:index"):
                 return True
@@ -225,24 +236,26 @@
                     except ImportError:
                         pass
 
             results.append(group)
 
         return results
 
-    def _get_value(self, instance, *args):
+    def _get_value(
+        self, instance: Union[str, Callable, None], *args: Any
+    ) -> Optional[str]:
         if instance is None:
             return None
 
         if isinstance(instance, str):
             return instance
 
         return instance(*args)
 
-    def _replace_values(self, target, source, request):
+    def _replace_values(self, target: Dict, source: Dict, request: HttpRequest):
         for key in source.keys():
             if source[key] is not None and callable(source[key]):
                 target[key] = source[key](request)
             else:
                 target[key] = source[key]
 
         return target
```

### Comparing `django_unfold-0.5.3/src/unfold/static/unfold/css/simplebar.css` & `django_unfold-0.6.0/src/unfold/static/unfold/css/simplebar.css`

 * *Files identical despite different names*

### Comparing `django_unfold-0.5.3/src/unfold/static/unfold/css/styles.css` & `django_unfold-0.6.0/src/unfold/static/unfold/css/styles.css`

 * *Files 0% similar despite different names*

```diff
@@ -1 +1 @@
-/*! tailwindcss v3.3.1 | MIT License | https://tailwindcss.com*/*,:after,:before{box-sizing:border-box;border:0 solid #e5e7eb}:after,:before{--tw-content:""}html{line-height:1.5;-webkit-text-size-adjust:100%;-moz-tab-size:4;-o-tab-size:4;tab-size:4;font-family:Inter,sans-serif;font-feature-settings:normal;font-variation-settings:normal}body{margin:0;line-height:inherit}hr{height:0;color:inherit;border-top-width:1px}abbr:where([title]){-webkit-text-decoration:underline dotted;text-decoration:underline dotted}h1,h2,h3,h4,h5,h6{font-size:inherit;font-weight:inherit}a{color:inherit;text-decoration:inherit}b,strong{font-weight:bolder}code,kbd,pre,samp{font-family:ui-monospace,SFMono-Regular,Menlo,Monaco,Consolas,Liberation Mono,Courier New,monospace;font-size:1em}small{font-size:80%}sub,sup{font-size:75%;line-height:0;position:relative;vertical-align:initial}sub{bottom:-.25em}sup{top:-.5em}table{text-indent:0;border-color:inherit;border-collapse:collapse}button,input,optgroup,select,textarea{font-family:inherit;font-size:100%;font-weight:inherit;line-height:inherit;color:inherit;margin:0;padding:0}button,select{text-transform:none}[type=button],[type=reset],[type=submit],button{-webkit-appearance:button;background-color:initial;background-image:none}:-moz-focusring{outline:auto}:-moz-ui-invalid{box-shadow:none}progress{vertical-align:initial}::-webkit-inner-spin-button,::-webkit-outer-spin-button{height:auto}[type=search]{-webkit-appearance:textfield;outline-offset:-2px}::-webkit-search-decoration{-webkit-appearance:none}::-webkit-file-upload-button{-webkit-appearance:button;font:inherit}summary{display:list-item}blockquote,dd,dl,figure,h1,h2,h3,h4,h5,h6,hr,p,pre{margin:0}fieldset{margin:0}fieldset,legend{padding:0}menu,ol,ul{list-style:none;margin:0;padding:0}textarea{resize:vertical}input::-moz-placeholder,textarea::-moz-placeholder{opacity:1;color:#9ca3af}input:-ms-input-placeholder,textarea:-ms-input-placeholder{opacity:1;color:#9ca3af}input::placeholder,textarea::placeholder{opacity:1;color:#9ca3af}[role=button],button{cursor:pointer}:disabled{cursor:default}audio,canvas,embed,iframe,img,object,svg,video{display:block;vertical-align:middle}img,video{max-width:100%;height:auto}[hidden]{display:none}*,:after,:before{--tw-border-spacing-x:0;--tw-border-spacing-y:0;--tw-translate-x:0;--tw-translate-y:0;--tw-rotate:0;--tw-skew-x:0;--tw-skew-y:0;--tw-scale-x:1;--tw-scale-y:1;--tw-pan-x: ;--tw-pan-y: ;--tw-pinch-zoom: ;--tw-scroll-snap-strictness:proximity;--tw-ordinal: ;--tw-slashed-zero: ;--tw-numeric-figure: ;--tw-numeric-spacing: ;--tw-numeric-fraction: ;--tw-ring-inset: ;--tw-ring-offset-width:0px;--tw-ring-offset-color:#fff;--tw-ring-color:#3b82f680;--tw-ring-offset-shadow:0 0 #0000;--tw-ring-shadow:0 0 #0000;--tw-shadow:0 0 #0000;--tw-shadow-colored:0 0 #0000;--tw-blur: ;--tw-brightness: ;--tw-contrast: ;--tw-grayscale: ;--tw-hue-rotate: ;--tw-invert: ;--tw-saturate: ;--tw-sepia: ;--tw-drop-shadow: ;--tw-backdrop-blur: ;--tw-backdrop-brightness: ;--tw-backdrop-contrast: ;--tw-backdrop-grayscale: ;--tw-backdrop-hue-rotate: ;--tw-backdrop-invert: ;--tw-backdrop-opacity: ;--tw-backdrop-saturate: ;--tw-backdrop-sepia: }::-webkit-backdrop{--tw-border-spacing-x:0;--tw-border-spacing-y:0;--tw-translate-x:0;--tw-translate-y:0;--tw-rotate:0;--tw-skew-x:0;--tw-skew-y:0;--tw-scale-x:1;--tw-scale-y:1;--tw-pan-x: ;--tw-pan-y: ;--tw-pinch-zoom: ;--tw-scroll-snap-strictness:proximity;--tw-ordinal: ;--tw-slashed-zero: ;--tw-numeric-figure: ;--tw-numeric-spacing: ;--tw-numeric-fraction: ;--tw-ring-inset: ;--tw-ring-offset-width:0px;--tw-ring-offset-color:#fff;--tw-ring-color:#3b82f680;--tw-ring-offset-shadow:0 0 #0000;--tw-ring-shadow:0 0 #0000;--tw-shadow:0 0 #0000;--tw-shadow-colored:0 0 #0000;--tw-blur: ;--tw-brightness: ;--tw-contrast: ;--tw-grayscale: ;--tw-hue-rotate: ;--tw-invert: ;--tw-saturate: ;--tw-sepia: ;--tw-drop-shadow: ;--tw-backdrop-blur: ;--tw-backdrop-brightness: ;--tw-backdrop-contrast: ;--tw-backdrop-grayscale: ;--tw-backdrop-hue-rotate: ;--tw-backdrop-invert: ;--tw-backdrop-opacity: ;--tw-backdrop-saturate: ;--tw-backdrop-sepia: }::backdrop{--tw-border-spacing-x:0;--tw-border-spacing-y:0;--tw-translate-x:0;--tw-translate-y:0;--tw-rotate:0;--tw-skew-x:0;--tw-skew-y:0;--tw-scale-x:1;--tw-scale-y:1;--tw-pan-x: ;--tw-pan-y: ;--tw-pinch-zoom: ;--tw-scroll-snap-strictness:proximity;--tw-ordinal: ;--tw-slashed-zero: ;--tw-numeric-figure: ;--tw-numeric-spacing: ;--tw-numeric-fraction: ;--tw-ring-inset: ;--tw-ring-offset-width:0px;--tw-ring-offset-color:#fff;--tw-ring-color:#3b82f680;--tw-ring-offset-shadow:0 0 #0000;--tw-ring-shadow:0 0 #0000;--tw-shadow:0 0 #0000;--tw-shadow-colored:0 0 #0000;--tw-blur: ;--tw-brightness: ;--tw-contrast: ;--tw-grayscale: ;--tw-hue-rotate: ;--tw-invert: ;--tw-saturate: ;--tw-sepia: ;--tw-drop-shadow: ;--tw-backdrop-blur: ;--tw-backdrop-brightness: ;--tw-backdrop-contrast: ;--tw-backdrop-grayscale: ;--tw-backdrop-hue-rotate: ;--tw-backdrop-invert: ;--tw-backdrop-opacity: ;--tw-backdrop-saturate: ;--tw-backdrop-sepia: }.container{width:100%}@media (min-width:640px){.container{max-width:640px}}@media (min-width:768px){.container{max-width:768px}}@media (min-width:1024px){.container{max-width:1024px}}@media (min-width:1280px){.container{max-width:1280px}}@media (min-width:1536px){.container{max-width:1536px}}.prose-sm{font-size:.875rem;line-height:1.7142857}.prose-sm :where(p):not(:where([class~=not-prose] *)){margin-top:1.1428571em;margin-bottom:1.1428571em}.prose-sm :where([class~=lead]):not(:where([class~=not-prose] *)){font-size:1.2857143em;line-height:1.5555556;margin-top:.8888889em;margin-bottom:.8888889em}.prose-sm :where(blockquote):not(:where([class~=not-prose] *)){margin-top:1.3333333em;margin-bottom:1.3333333em;padding-left:1.1111111em}.prose-sm :where(h1):not(:where([class~=not-prose] *)){font-size:2.1428571em;margin-top:0;margin-bottom:.8em;line-height:1.2}.prose-sm :where(h2):not(:where([class~=not-prose] *)){font-size:1.4285714em;margin-top:1.6em;margin-bottom:.8em;line-height:1.4}.prose-sm :where(h3):not(:where([class~=not-prose] *)){font-size:1.2857143em;margin-top:1.5555556em;margin-bottom:.4444444em;line-height:1.5555556}.prose-sm :where(h4):not(:where([class~=not-prose] *)){margin-top:1.4285714em;margin-bottom:.5714286em;line-height:1.4285714}.prose-sm :where(img):not(:where([class~=not-prose] *)){margin-top:1.7142857em;margin-bottom:1.7142857em}.prose-sm :where(video):not(:where([class~=not-prose] *)){margin-top:1.7142857em;margin-bottom:1.7142857em}.prose-sm :where(figure):not(:where([class~=not-prose] *)){margin-top:1.7142857em;margin-bottom:1.7142857em}.prose-sm :where(figure>*):not(:where([class~=not-prose] *)){margin-top:0;margin-bottom:0}.prose-sm :where(figcaption):not(:where([class~=not-prose] *)){font-size:.8571429em;line-height:1.3333333;margin-top:.6666667em}.prose-sm :where(code):not(:where([class~=not-prose] *)){font-size:.8571429em}.prose-sm :where(h2 code):not(:where([class~=not-prose] *)){font-size:.9em}.prose-sm :where(h3 code):not(:where([class~=not-prose] *)){font-size:.8888889em}.prose-sm :where(pre):not(:where([class~=not-prose] *)){font-size:.8571429em;line-height:1.6666667;margin-top:1.6666667em;margin-bottom:1.6666667em;border-radius:.25rem;padding:.6666667em 1em}.prose-sm :where(ol):not(:where([class~=not-prose] *)){margin-top:1.1428571em;margin-bottom:1.1428571em;padding-left:1.5714286em}.prose-sm :where(ul):not(:where([class~=not-prose] *)){margin-top:1.1428571em;margin-bottom:1.1428571em;padding-left:1.5714286em}.prose-sm :where(li):not(:where([class~=not-prose] *)){margin-top:.2857143em;margin-bottom:.2857143em}.prose-sm :where(ol>li):not(:where([class~=not-prose] *)){padding-left:.4285714em}.prose-sm :where(ul>li):not(:where([class~=not-prose] *)){padding-left:.4285714em}.prose-sm :where(.prose-sm>ul>li p):not(:where([class~=not-prose] *)){margin-top:.5714286em;margin-bottom:.5714286em}.prose-sm :where(.prose-sm>ul>li>:first-child):not(:where([class~=not-prose] *)){margin-top:1.1428571em}.prose-sm :where(.prose-sm>ul>li>:last-child):not(:where([class~=not-prose] *)){margin-bottom:1.1428571em}.prose-sm :where(.prose-sm>ol>li>:first-child):not(:where([class~=not-prose] *)){margin-top:1.1428571em}.prose-sm :where(.prose-sm>ol>li>:last-child):not(:where([class~=not-prose] *)){margin-bottom:1.1428571em}.prose-sm :where(ul ul,ul ol,ol ul,ol ol):not(:where([class~=not-prose] *)){margin-top:.5714286em;margin-bottom:.5714286em}.prose-sm :where(hr):not(:where([class~=not-prose] *)){margin-top:2.8571429em;margin-bottom:2.8571429em}.prose-sm :where(hr+*):not(:where([class~=not-prose] *)){margin-top:0}.prose-sm :where(h2+*):not(:where([class~=not-prose] *)){margin-top:0}.prose-sm :where(h3+*):not(:where([class~=not-prose] *)){margin-top:0}.prose-sm :where(h4+*):not(:where([class~=not-prose] *)){margin-top:0}.prose-sm :where(table):not(:where([class~=not-prose] *)){font-size:.8571429em;line-height:1.5}.prose-sm :where(thead th):not(:where([class~=not-prose] *)){padding-right:1em;padding-bottom:.6666667em;padding-left:1em}.prose-sm :where(thead th:first-child):not(:where([class~=not-prose] *)){padding-left:0}.prose-sm :where(thead th:last-child):not(:where([class~=not-prose] *)){padding-right:0}.prose-sm :where(tbody td,tfoot td):not(:where([class~=not-prose] *)){padding:.6666667em 1em}.prose-sm :where(tbody td:first-child,tfoot td:first-child):not(:where([class~=not-prose] *)){padding-left:0}.prose-sm :where(tbody td:last-child,tfoot td:last-child):not(:where([class~=not-prose] *)){padding-right:0}.prose-sm :where(.prose-sm>:first-child):not(:where([class~=not-prose] *)){margin-top:0}.prose-sm :where(.prose-sm>:last-child):not(:where([class~=not-prose] *)){margin-bottom:0}.visible{visibility:visible}.invisible{visibility:hidden}.collapse{visibility:collapse}.static{position:static}.fixed{position:fixed}.absolute{position:absolute}.relative{position:relative}.sticky{position:sticky}.-bottom-px{bottom:-1px}.-right-2{right:-.5rem}.bottom-0{bottom:0}.bottom-4{bottom:1rem}.left-0{left:0}.left-72{left:18rem}.right-0{right:0}.right-2{right:.5rem}.right-4{right:1rem}.top-0{top:0}.top-2{top:.5rem}.top-5{top:1.25rem}.top-7{top:1.75rem}.z-10{z-index:10}.z-20{z-index:20}.z-30{z-index:30}.z-50{z-index:50}.-mx-2{margin-left:-.5rem;margin-right:-.5rem}.-mx-3{margin-left:-.75rem;margin-right:-.75rem}.-mx-4{margin-left:-1rem;margin-right:-1rem}.-my-1{margin-top:-.25rem;margin-bottom:-.25rem}.-my-3{margin-top:-.75rem;margin-bottom:-.75rem}.mx-1{margin-left:.25rem;margin-right:.25rem}.mx-2{margin-left:.5rem;margin-right:.5rem}.mx-3{margin-left:.75rem;margin-right:.75rem}.mx-6{margin-left:1.5rem;margin-right:1.5rem}.mx-auto{margin-left:auto;margin-right:auto}.my-2{margin-top:.5rem;margin-bottom:.5rem}.my-3{margin-top:.75rem;margin-bottom:.75rem}.my-4{margin-top:1rem;margin-bottom:1rem}.-mb-5{margin-bottom:-1.25rem}.-mb-px{margin-bottom:-1px}.-mr-1{margin-right:-.25rem}.mb-1{margin-bottom:.25rem}.mb-10{margin-bottom:2.5rem}.mb-12{margin-bottom:3rem}.mb-2{margin-bottom:.5rem}.mb-3{margin-bottom:.75rem}.mb-4{margin-bottom:1rem}.mb-5{margin-bottom:1.25rem}.mb-6{margin-bottom:1.5rem}.mb-8{margin-bottom:2rem}.ml-1{margin-left:.25rem}.ml-2{margin-left:.5rem}.ml-3{margin-left:.75rem}.ml-4{margin-left:1rem}.ml-6{margin-left:1.5rem}.ml-72{margin-left:18rem}.ml-auto{margin-left:auto}.mr-1{margin-right:.25rem}.mr-2{margin-right:.5rem}.mr-3{margin-right:.75rem}.mr-4{margin-right:1rem}.mr-auto{margin-right:auto}.mt-0{margin-top:0}.mt-0\.5{margin-top:.125rem}.mt-1{margin-top:.25rem}.mt-12{margin-top:3rem}.mt-2{margin-top:.5rem}.mt-20{margin-top:5rem}.mt-3{margin-top:.75rem}.mt-4{margin-top:1rem}.mt-auto{margin-top:auto}.block{display:block}.inline-block{display:inline-block}.inline{display:inline}.flex{display:flex}.table{display:table}.contents{display:contents}.hidden{display:none}.h-1{height:.25rem}.h-10{height:2.5rem}.h-11{height:2.75rem}.h-16{height:4rem}.h-4{height:1rem}.h-5{height:1.25rem}.h-6{height:1.5rem}.h-8{height:2rem}.h-9{height:2.25rem}.h-9\.5{height:2.375rem}.h-full{height:100%}.max-h-screen{max-height:100vh}.min-h-screen{min-height:100vh}.w-1{width:.25rem}.w-10{width:2.5rem}.w-36{width:9rem}.w-4\/12{width:33.333333%}.w-40{width:10rem}.w-48{width:12rem}.w-52{width:13rem}.w-6{width:1.5rem}.w-72{width:18rem}.w-8{width:2rem}.w-80{width:20rem}.w-9{width:2.25rem}.w-9\.5{width:2.375rem}.w-96{width:24rem}.w-full{width:100%}.w-px{width:1px}.w-screen{width:100vw}.w-sidebar{width:18rem}.min-w-0{min-width:0}.min-w-sidebar{min-width:18rem}.max-w-2xl{max-width:42rem}.max-w-3xl{max-width:48rem}.max-w-4xl{max-width:56rem}.max-w-none{max-width:none}.flex-none{flex:none}.flex-shrink-0,.shrink-0{flex-shrink:0}.flex-grow{flex-grow:1}.basis-1\/2{flex-basis:50%}.table-fixed{table-layout:fixed}.border-separate{border-collapse:initial}.-translate-x-1\/2{--tw-translate-x:-50%}.-translate-x-1\/2,.translate-y-full{transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.translate-y-full{--tw-translate-y:100%}.rotate-180{--tw-rotate:180deg}.rotate-180,.transform{transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}@-webkit-keyframes spin{to{transform:rotate(1turn)}}.animate-spin{-webkit-animation:spin 1s linear infinite;animation:spin 1s linear infinite}.cursor-not-allowed{cursor:not-allowed}.cursor-pointer{cursor:pointer}.resize-none{resize:none}.resize{resize:both}.appearance-none{-webkit-appearance:none;-moz-appearance:none;appearance:none}.flex-row{flex-direction:row}.flex-col{flex-direction:column}.flex-col-reverse{flex-direction:column-reverse}.flex-wrap{flex-wrap:wrap}.items-start{align-items:flex-start}.items-center{align-items:center}.justify-start{justify-content:flex-start}.justify-end{justify-content:flex-end}.justify-center{justify-content:center}.gap-x-8{-moz-column-gap:2rem;column-gap:2rem}.space-x-4>:not([hidden])~:not([hidden]){--tw-space-x-reverse:0;margin-right:calc(1rem*var(--tw-space-x-reverse));margin-left:calc(1rem*(1 - var(--tw-space-x-reverse)))}.space-y-4>:not([hidden])~:not([hidden]){--tw-space-y-reverse:0;margin-top:calc(1rem*(1 - var(--tw-space-y-reverse)));margin-bottom:calc(1rem*var(--tw-space-y-reverse))}.self-end{align-self:flex-end}.self-center{align-self:center}.self-stretch{align-self:stretch}.overflow-auto{overflow:auto}.overflow-hidden{overflow:hidden}.overflow-y-auto{overflow-y:auto}.overflow-x-hidden{overflow-x:hidden}.truncate{overflow:hidden;white-space:nowrap}.text-ellipsis,.truncate{text-overflow:ellipsis}.whitespace-nowrap{white-space:nowrap}.break-words{overflow-wrap:break-word}.rounded{border-radius:.25rem}.rounded-full{border-radius:9999px}.rounded-md{border-radius:.375rem}.rounded-sm{border-radius:.125rem}.rounded-b{border-bottom-right-radius:.25rem;border-bottom-left-radius:.25rem}.rounded-b-md{border-bottom-right-radius:.375rem;border-bottom-left-radius:.375rem}.rounded-t-md{border-top-left-radius:.375rem;border-top-right-radius:.375rem}.rounded-t-none{border-top-left-radius:0;border-top-right-radius:0}.border{border-width:1px}.border-0{border-width:0}.border-b{border-bottom-width:1px}.border-l-4{border-left-width:4px}.border-r{border-right-width:1px}.border-t{border-top-width:1px}.border-t-0{border-top-width:0}.border-blue-200{--tw-border-opacity:1;border-color:rgb(191 219 254/var(--tw-border-opacity))}.border-gray-100{--tw-border-opacity:1;border-color:rgb(243 244 246/var(--tw-border-opacity))}.border-gray-200{--tw-border-opacity:1;border-color:rgb(229 231 235/var(--tw-border-opacity))}.border-green-200{--tw-border-opacity:1;border-color:rgb(187 247 208/var(--tw-border-opacity))}.border-orange-200{--tw-border-opacity:1;border-color:rgb(254 215 170/var(--tw-border-opacity))}.border-primary-600{--tw-border-opacity:1;border-color:rgb(var(--color-primary-600)/var(--tw-border-opacity))}.border-red-200{--tw-border-opacity:1;border-color:rgb(254 202 202/var(--tw-border-opacity))}.border-red-500{--tw-border-opacity:1;border-color:rgb(239 68 68/var(--tw-border-opacity))}.border-transparent{border-color:#0000}.bg-amber-100{--tw-bg-opacity:1;background-color:rgb(254 243 199/var(--tw-bg-opacity))}.bg-blue-50{--tw-bg-opacity:1;background-color:rgb(239 246 255/var(--tw-bg-opacity))}.bg-gray-100{--tw-bg-opacity:1;background-color:rgb(243 244 246/var(--tw-bg-opacity))}.bg-gray-200{--tw-bg-opacity:1;background-color:rgb(229 231 235/var(--tw-bg-opacity))}.bg-gray-50{--tw-bg-opacity:1;background-color:rgb(249 250 251/var(--tw-bg-opacity))}.bg-gray-500{--tw-bg-opacity:1;background-color:rgb(107 114 128/var(--tw-bg-opacity))}.bg-gray-700{--tw-bg-opacity:1;background-color:rgb(55 65 81/var(--tw-bg-opacity))}.bg-gray-900{--tw-bg-opacity:1;background-color:rgb(17 24 39/var(--tw-bg-opacity))}.bg-green-100{--tw-bg-opacity:1;background-color:rgb(220 252 231/var(--tw-bg-opacity))}.bg-green-50{--tw-bg-opacity:1;background-color:rgb(240 253 244/var(--tw-bg-opacity))}.bg-green-500{--tw-bg-opacity:1;background-color:rgb(34 197 94/var(--tw-bg-opacity))}.bg-orange-50{--tw-bg-opacity:1;background-color:rgb(255 247 237/var(--tw-bg-opacity))}.bg-primary-100{--tw-bg-opacity:1;background-color:rgb(var(--color-primary-100)/var(--tw-bg-opacity))}.bg-primary-600{--tw-bg-opacity:1;background-color:rgb(var(--color-primary-600)/var(--tw-bg-opacity))}.bg-red-100{--tw-bg-opacity:1;background-color:rgb(254 226 226/var(--tw-bg-opacity))}.bg-red-50{--tw-bg-opacity:1;background-color:rgb(254 242 242/var(--tw-bg-opacity))}.bg-red-500{--tw-bg-opacity:1;background-color:rgb(239 68 68/var(--tw-bg-opacity))}.bg-red-600{--tw-bg-opacity:1;background-color:rgb(220 38 38/var(--tw-bg-opacity))}.bg-white{--tw-bg-opacity:1;background-color:rgb(255 255 255/var(--tw-bg-opacity))}.bg-opacity-80{--tw-bg-opacity:0.8}.bg-none{background-image:none}.bg-cover{background-size:cover}.bg-center{background-position:50%}.bg-no-repeat{background-repeat:no-repeat}.p-1{padding:.25rem}.p-3{padding:.75rem}.p-4{padding:1rem}.px-1{padding-left:.25rem;padding-right:.25rem}.px-12{padding-left:3rem;padding-right:3rem}.px-2{padding-left:.5rem;padding-right:.5rem}.px-3{padding-left:.75rem;padding-right:.75rem}.px-4{padding-left:1rem;padding-right:1rem}.px-6{padding-left:1.5rem;padding-right:1.5rem}.px-8{padding-left:2rem;padding-right:2rem}.py-1{padding-top:.25rem;padding-bottom:.25rem}.py-1\.5{padding-top:.375rem;padding-bottom:.375rem}.py-2{padding-top:.5rem;padding-bottom:.5rem}.py-3{padding-top:.75rem;padding-bottom:.75rem}.py-4{padding-top:1rem;padding-bottom:1rem}.py-5{padding-top:1.25rem;padding-bottom:1.25rem}.pb-1{padding-bottom:.25rem}.pb-12{padding-bottom:3rem}.pb-16{padding-bottom:4rem}.pl-2{padding-left:.5rem}.pl-3{padding-left:.75rem}.pl-4{padding-left:1rem}.pr-2{padding-right:.5rem}.pr-3{padding-right:.75rem}.pr-4{padding-right:1rem}.pr-8{padding-right:2rem}.pt-1{padding-top:.25rem}.pt-3{padding-top:.75rem}.text-left{text-align:left}.text-center{text-align:center}.text-right{text-align:right}.align-top{vertical-align:top}.align-middle{vertical-align:middle}.align-text-top{vertical-align:text-top}.font-sans{font-family:Inter,sans-serif}.text-lg{font-size:1.125rem;line-height:1.75rem}.text-sm{font-size:.875rem;line-height:1.25rem}.text-xl{font-size:1.25rem;line-height:1.75rem}.text-xs{font-size:.75rem;line-height:1rem}.text-xxs{font-size:11px;line-height:14px}.font-medium{font-weight:500}.font-normal{font-weight:400}.font-semibold{font-weight:600}.uppercase{text-transform:uppercase}.italic{font-style:italic}.leading-none{line-height:1}.leading-relaxed{line-height:1.625}.text-amber-600{--tw-text-opacity:1;color:rgb(217 119 6/var(--tw-text-opacity))}.text-blue-500{--tw-text-opacity:1;color:rgb(59 130 246/var(--tw-text-opacity))}.text-gray-200{--tw-text-opacity:1;color:rgb(229 231 235/var(--tw-text-opacity))}.text-gray-300{--tw-text-opacity:1;color:rgb(209 213 219/var(--tw-text-opacity))}.text-gray-400{--tw-text-opacity:1;color:rgb(156 163 175/var(--tw-text-opacity))}.text-gray-500{--tw-text-opacity:1;color:rgb(107 114 128/var(--tw-text-opacity))}.text-gray-700{--tw-text-opacity:1;color:rgb(55 65 81/var(--tw-text-opacity))}.text-gray-900{--tw-text-opacity:1;color:rgb(17 24 39/var(--tw-text-opacity))}.text-green-500{--tw-text-opacity:1;color:rgb(34 197 94/var(--tw-text-opacity))}.text-green-600{--tw-text-opacity:1;color:rgb(22 163 74/var(--tw-text-opacity))}.text-orange-500{--tw-text-opacity:1;color:rgb(249 115 22/var(--tw-text-opacity))}.text-primary-500{--tw-text-opacity:1;color:rgb(var(--color-primary-500)/var(--tw-text-opacity))}.text-primary-600{--tw-text-opacity:1;color:rgb(var(--color-primary-600)/var(--tw-text-opacity))}.text-red-500{--tw-text-opacity:1;color:rgb(239 68 68/var(--tw-text-opacity))}.text-red-600{--tw-text-opacity:1;color:rgb(220 38 38/var(--tw-text-opacity))}.text-white{--tw-text-opacity:1;color:rgb(255 255 255/var(--tw-text-opacity))}.underline{-webkit-text-decoration-line:underline;text-decoration-line:underline}.antialiased{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale}.opacity-0{opacity:0}.shadow{--tw-shadow:0 1px 3px 0 #0000001a,0 1px 2px -1px #0000001a;--tw-shadow-colored:0 1px 3px 0 var(--tw-shadow-color),0 1px 2px -1px var(--tw-shadow-color)}.shadow,.shadow-lg{box-shadow:var(--tw-ring-offset-shadow,0 0 #0000),var(--tw-ring-shadow,0 0 #0000),var(--tw-shadow)}.shadow-lg{--tw-shadow:0 10px 15px -3px #0000001a,0 4px 6px -4px #0000001a;--tw-shadow-colored:0 10px 15px -3px var(--tw-shadow-color),0 4px 6px -4px var(--tw-shadow-color)}.shadow-sm{--tw-shadow:0 1px 2px 0 #0000000d;--tw-shadow-colored:0 1px 2px 0 var(--tw-shadow-color);box-shadow:var(--tw-ring-offset-shadow,0 0 #0000),var(--tw-ring-shadow,0 0 #0000),var(--tw-shadow)}.blur{--tw-blur:blur(8px)}.blur,.filter{filter:var(--tw-blur) var(--tw-brightness) var(--tw-contrast) var(--tw-grayscale) var(--tw-hue-rotate) var(--tw-invert) var(--tw-saturate) var(--tw-sepia) var(--tw-drop-shadow)}.backdrop-blur-sm{--tw-backdrop-blur:blur(4px);-webkit-backdrop-filter:var(--tw-backdrop-blur) var(--tw-backdrop-brightness) var(--tw-backdrop-contrast) var(--tw-backdrop-grayscale) var(--tw-backdrop-hue-rotate) var(--tw-backdrop-invert) var(--tw-backdrop-opacity) var(--tw-backdrop-saturate) var(--tw-backdrop-sepia);backdrop-filter:var(--tw-backdrop-blur) var(--tw-backdrop-brightness) var(--tw-backdrop-contrast) var(--tw-backdrop-grayscale) var(--tw-backdrop-hue-rotate) var(--tw-backdrop-invert) var(--tw-backdrop-opacity) var(--tw-backdrop-saturate) var(--tw-backdrop-sepia)}.transition{transition-property:color,background-color,border-color,fill,stroke,opacity,box-shadow,transform,filter,-webkit-text-decoration-color,-webkit-backdrop-filter;transition-property:color,background-color,border-color,text-decoration-color,fill,stroke,opacity,box-shadow,transform,filter,backdrop-filter;transition-property:color,background-color,border-color,text-decoration-color,fill,stroke,opacity,box-shadow,transform,filter,backdrop-filter,-webkit-text-decoration-color,-webkit-backdrop-filter;transition-timing-function:cubic-bezier(.4,0,.2,1);transition-duration:.15s}.transition-all{transition-property:all;transition-timing-function:cubic-bezier(.4,0,.2,1);transition-duration:.15s}.transition-colors{transition-property:color,background-color,border-color,fill,stroke,-webkit-text-decoration-color;transition-property:color,background-color,border-color,text-decoration-color,fill,stroke;transition-property:color,background-color,border-color,text-decoration-color,fill,stroke,-webkit-text-decoration-color;transition-timing-function:cubic-bezier(.4,0,.2,1);transition-duration:.15s}.transition-height{transition-property:height;transition-timing-function:cubic-bezier(.4,0,.2,1);transition-duration:.15s}.transition-width{transition-property:width;transition-timing-function:cubic-bezier(.4,0,.2,1);transition-duration:.15s}.duration-75{transition-duration:75ms}.ease-in-out{transition-timing-function:cubic-bezier(.4,0,.2,1)}.border-spacing-none{border-spacing:0}.material-symbols-outlined{font-family:Material Symbols Outlined;font-weight:400;font-style:normal;font-size:18px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-moz-font-feature-settings:"liga";-moz-osx-font-smoothing:grayscale}.scrollable-top:after{position:absolute;left:0;right:0;top:-1rem;height:1rem;background-image:linear-gradient(to top,var(--tw-gradient-stops));--tw-gradient-from:#f3f4f6 var(--tw-gradient-from-position);--tw-gradient-from-position: ;--tw-gradient-to:#f3f4f600 var(--tw-gradient-from-position);--tw-gradient-to-position: ;--tw-gradient-stops:var(--tw-gradient-from),var(--tw-gradient-to)}:is(.dark .scrollable-top):after{background-image:none}.scrollable-top:after{content:""}html{--color-primary-100:#f3e8ff;--color-primary-200:#e9d5ff;--color-primary-300:#d8b4fe;--color-primary-400:#c084fc;--color-primary-500:#a855f7;--color-primary-600:#9333ea;--color-primary-700:#7e22ce;--color-primary-800:#6b21a8;--color-primary-900:#581c87}.column-fill-auto{-moz-column-fill:auto;column-fill:auto}[x-cloak]{display:none!important}.asteriskField{--tw-text-opacity:1;color:rgb(220 38 38/var(--tw-text-opacity))}.md-16{font-size:16px}.md-18{font-size:18px}select:not([class*=bg-none]):not([multiple]){background-image:url("data:image/svg+xml;charset=utf-8,%3Csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 48 48'%3E%3Cpath fill='%236B7280' d='M24 31.4 11.3 18.7l2.85-2.8L24 25.8l9.85-9.85 2.85 2.8Z'/%3E%3C/svg%3E");background-position:right .7rem center;background-repeat:no-repeat;background-size:1.125rem 1.125rem}select:after{content:"";display:block}#page input[type=checkbox]{position:relative;display:block;height:1rem;width:1rem;cursor:pointer;-webkit-appearance:none;-moz-appearance:none;appearance:none;border-radius:.25rem;border-width:1px;border-color:rgb(209 213 219/var(--tw-border-opacity));background-color:rgb(255 255 255/var(--tw-bg-opacity))}#page input[type=checkbox],:is(.dark #page input[type=checkbox]){--tw-border-opacity:1;--tw-bg-opacity:1}:is(.dark #page input[type=checkbox]){border-color:rgb(107 114 128/var(--tw-border-opacity));background-color:rgb(55 65 81/var(--tw-bg-opacity))}#page input[type=checkbox]:hover{--tw-border-opacity:1;border-color:rgb(156 163 175/var(--tw-border-opacity))}#page input[type=checkbox]:after{position:absolute;margin-left:-1px;margin-top:-1px;display:flex;height:1rem;width:1rem;align-items:center;justify-content:center;font-size:.875rem;line-height:1.25rem;line-height:1;--tw-text-opacity:1;color:rgb(255 255 255/var(--tw-text-opacity));transition-property:all;transition-timing-function:cubic-bezier(.4,0,.2,1);transition-duration:.15s}:is(.dark #page input[type=checkbox]):after{--tw-text-opacity:1;color:rgb(55 65 81/var(--tw-text-opacity))}#page input[type=checkbox]:after{content:"done";font-family:Material Symbols Outlined}#page input[type=checkbox]:checked{--tw-border-opacity:1;border-color:rgb(var(--color-primary-600)/var(--tw-border-opacity));--tw-bg-opacity:1;background-color:rgb(var(--color-primary-600)/var(--tw-bg-opacity));transition-property:all;transition-timing-function:cubic-bezier(.4,0,.2,1);transition-duration:.15s}#page input[type=checkbox]:checked:after{--tw-text-opacity:1;color:rgb(255 255 255/var(--tw-text-opacity))}#page input[type=checkbox].hidden{display:none}table select{display:block;cursor:pointer;-webkit-appearance:none;-moz-appearance:none;appearance:none;border-radius:.375rem;border-width:1px;background-repeat:no-repeat;padding:.5rem 1.25rem .5rem .75rem;font-weight:500;--tw-text-opacity:1;color:rgb(107 114 128/var(--tw-text-opacity));--tw-shadow:0 1px 2px 0 #0000000d;--tw-shadow-colored:0 1px 2px 0 var(--tw-shadow-color);box-shadow:var(--tw-ring-offset-shadow,0 0 #0000),var(--tw-ring-shadow,0 0 #0000),var(--tw-shadow);background-image:url('data:image/svg+xml;utf8,<svg xmlns="http://www.w3.org/2000/svg" height="24px" viewBox="0 0 24 24" width="24px" fill="rgb(156, 163, 175)"><path d="M0 0h24v24H0V0z" fill="none"/><path d="M7 10l5 5 5-5H7z"/></svg>');background-size:1.125rem 1.125rem;background-position:right .5rem center}table select:focus{--tw-border-opacity:1;border-color:rgb(var(--color-primary-600)/var(--tw-border-opacity))}table tr.selected{--tw-bg-opacity:1;background-color:rgb(254 252 232/var(--tw-bg-opacity))}:is(.dark table tr.selected){background-color:#ffffff0f}.datetimeshortcuts{display:flex;flex-direction:row-reverse;align-items:center;font-size:0;line-height:1}.datetimeshortcuts a{font-size:0;line-height:1;--tw-text-opacity:1;color:rgb(156 163 175/var(--tw-text-opacity));transition-property:color,background-color,border-color,fill,stroke,opacity,box-shadow,transform,filter,-webkit-text-decoration-color,-webkit-backdrop-filter;transition-property:color,background-color,border-color,text-decoration-color,fill,stroke,opacity,box-shadow,transform,filter,backdrop-filter;transition-property:color,background-color,border-color,text-decoration-color,fill,stroke,opacity,box-shadow,transform,filter,backdrop-filter,-webkit-text-decoration-color,-webkit-backdrop-filter;transition-timing-function:cubic-bezier(.4,0,.2,1);transition-duration:.15s}.datetimeshortcuts a:hover{--tw-text-opacity:1;color:rgb(55 65 81/var(--tw-text-opacity))}.datetimeshortcuts a:first-child{margin-left:.5rem}.datetimeshortcuts a:first-child:hover{--tw-text-opacity:1;color:rgb(55 65 81/var(--tw-text-opacity))}:is(.dark .datetimeshortcuts a:first-child){--tw-text-opacity:1;color:rgb(107 114 128/var(--tw-text-opacity))}:is(.dark .datetimeshortcuts a:first-child:hover){--tw-text-opacity:1;color:rgb(229 231 235/var(--tw-text-opacity))}.datetimeshortcuts a:first-child:after{display:flex;height:2.375rem;width:2.375rem;align-items:center;justify-content:center;border-radius:.25rem;border-width:1px;--tw-bg-opacity:1;background-color:rgb(255 255 255/var(--tw-bg-opacity));padding-top:.5rem;padding-bottom:.5rem;text-align:center;font-size:1rem;line-height:1.5rem;--tw-shadow:0 1px 2px 0 #0000000d;--tw-shadow-colored:0 1px 2px 0 var(--tw-shadow-color);box-shadow:var(--tw-ring-offset-shadow,0 0 #0000),var(--tw-ring-shadow,0 0 #0000),var(--tw-shadow);font-family:Material Symbols Outlined;font-weight:400;font-style:normal;font-size:18px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-moz-font-feature-settings:"liga";-moz-osx-font-smoothing:grayscale}.datetimeshortcuts a:first-child:hover:after{--tw-text-opacity:1;color:rgb(55 65 81/var(--tw-text-opacity))}:is(.dark .datetimeshortcuts a:first-child):after{--tw-border-opacity:1;border-color:rgb(55 65 81/var(--tw-border-opacity));--tw-bg-opacity:1;background-color:rgb(17 24 39/var(--tw-bg-opacity))}:is(.dark .datetimeshortcuts a:first-child:hover):after{--tw-text-opacity:1;color:rgb(255 255 255/var(--tw-text-opacity))}.datetimeshortcuts a:first-child:after{content:"timer";display:flex}.date-icon{margin-left:.5rem;display:block;height:2.375rem;width:2.375rem;--tw-text-opacity:1;color:rgb(156 163 175/var(--tw-text-opacity));transition-property:all;transition-timing-function:cubic-bezier(.4,0,.2,1);transition-duration:.15s}.date-icon:hover{--tw-text-opacity:1;color:rgb(55 65 81/var(--tw-text-opacity))}:is(.dark .date-icon){--tw-text-opacity:1;color:rgb(107 114 128/var(--tw-text-opacity))}:is(.dark .date-icon:hover){--tw-text-opacity:1;color:rgb(255 255 255/var(--tw-text-opacity))}.date-icon:after{height:2.375rem;width:2.375rem;align-items:center;justify-content:center;border-radius:.25rem;border-width:1px;--tw-bg-opacity:1;background-color:rgb(255 255 255/var(--tw-bg-opacity));padding-top:.5rem;padding-bottom:.5rem;text-align:center;font-size:1rem;line-height:1.5rem;--tw-shadow:0 1px 2px 0 #0000000d;--tw-shadow-colored:0 1px 2px 0 var(--tw-shadow-color);box-shadow:var(--tw-ring-offset-shadow,0 0 #0000),var(--tw-ring-shadow,0 0 #0000),var(--tw-shadow);font-family:Material Symbols Outlined;font-weight:400;font-style:normal;font-size:18px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-moz-font-feature-settings:"liga";-moz-osx-font-smoothing:grayscale}.date-icon:hover:after{--tw-text-opacity:1;color:rgb(55 65 81/var(--tw-text-opacity))}:is(.dark .date-icon):after{--tw-border-opacity:1;border-color:rgb(55 65 81/var(--tw-border-opacity));--tw-bg-opacity:1;background-color:rgb(17 24 39/var(--tw-bg-opacity))}.date-icon:after{content:"edit";display:flex}:is(.dark .date-icon:hover):after{--tw-text-opacity:1;color:rgb(255 255 255/var(--tw-text-opacity))}.clock-icon{margin-left:.5rem;display:block;height:2.375rem;width:2.375rem}.clock-icon:hover{--tw-text-opacity:1;color:rgb(55 65 81/var(--tw-text-opacity))}:is(.dark .clock-icon){--tw-text-opacity:1;color:rgb(107 114 128/var(--tw-text-opacity))}:is(.dark .clock-icon:hover){--tw-text-opacity:1;color:rgb(229 231 235/var(--tw-text-opacity))}.clock-icon:after{height:2.375rem;width:2.375rem;align-items:center;justify-content:center;border-radius:.25rem;border-width:1px;--tw-bg-opacity:1;background-color:rgb(255 255 255/var(--tw-bg-opacity));padding-top:.5rem;padding-bottom:.5rem;text-align:center;font-size:1rem;line-height:1.5rem;--tw-shadow:0 1px 2px 0 #0000000d;--tw-shadow-colored:0 1px 2px 0 var(--tw-shadow-color);box-shadow:var(--tw-ring-offset-shadow,0 0 #0000),var(--tw-ring-shadow,0 0 #0000),var(--tw-shadow);font-family:Material Symbols Outlined;font-weight:400;font-style:normal;font-size:18px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-moz-font-feature-settings:"liga";-moz-osx-font-smoothing:grayscale}.clock-icon:hover:after{--tw-text-opacity:1;color:rgb(55 65 81/var(--tw-text-opacity))}:is(.dark .clock-icon):after{--tw-border-opacity:1;border-color:rgb(55 65 81/var(--tw-border-opacity));--tw-bg-opacity:1;background-color:rgb(17 24 39/var(--tw-bg-opacity))}:is(.dark .clock-icon:hover):after{--tw-text-opacity:1;color:rgb(255 255 255/var(--tw-text-opacity))}.clock-icon:after{content:"edit";display:flex}.timezonewarning{margin-top:.5rem;width:100%;font-size:.75rem;line-height:1rem;--tw-text-opacity:1;color:rgb(107 114 128/var(--tw-text-opacity))}.selector{display:flex;flex-direction:column;align-items:center}@media (min-width:768px){.selector{flex-direction:row}}.selector select{width:100%;flex-grow:1;background-image:none}:is(.dark .selector select){--tw-bg-opacity:1;background-color:rgb(17 24 39/var(--tw-bg-opacity))}.selector option{overflow:hidden;text-overflow:ellipsis;white-space:nowrap;padding-left:.75rem;padding-right:.75rem;font-size:.875rem;line-height:1.25rem;--tw-text-opacity:1;color:rgb(107 114 128/var(--tw-text-opacity))}:is(.dark .selector option){--tw-text-opacity:1;color:rgb(156 163 175/var(--tw-text-opacity))}.selector .list-footer-display{border-top-width:1px;padding-top:.5rem;padding-bottom:.5rem;text-align:center;font-size:.875rem;line-height:1.25rem}:is(.dark .selector .list-footer-display){--tw-border-opacity:1;border-color:rgb(55 65 81/var(--tw-border-opacity))}.selector-available,.selector-chosen{display:flex;flex-grow:1;flex-direction:column;align-self:stretch;border-radius:.375rem;border-width:1px;--tw-shadow:0 1px 2px 0 #0000000d;--tw-shadow-colored:0 1px 2px 0 var(--tw-shadow-color);box-shadow:var(--tw-ring-offset-shadow,0 0 #0000),var(--tw-ring-shadow,0 0 #0000),var(--tw-shadow)}:is(.dark .selector-available),:is(.dark .selector-chosen){--tw-border-opacity:1;border-color:rgb(55 65 81/var(--tw-border-opacity))}@media (min-width:768px){.selector-available,.selector-chosen{width:18rem}}@media (min-width:1024px){.selector-available,.selector-chosen{width:24rem}}.selector-available h2,.selector-chosen h2{margin-bottom:.75rem;border-bottom-width:1px;padding:.5rem .75rem;font-size:.875rem;line-height:1.25rem;--tw-text-opacity:1;color:rgb(107 114 128/var(--tw-text-opacity))}:is(.dark .selector-available h2),:is(.dark .selector-chosen h2){--tw-border-opacity:1;border-color:rgb(55 65 81/var(--tw-border-opacity));--tw-text-opacity:1;color:rgb(229 231 235/var(--tw-text-opacity))}.selector-filter{display:flex}.selector-filter input{margin-left:.75rem;margin-right:.75rem;margin-bottom:.75rem;display:block;flex-grow:1;border-radius:.375rem;--tw-bg-opacity:1;background-color:rgb(243 244 246/var(--tw-bg-opacity));padding:.5rem .75rem;font-size:.875rem;line-height:1.25rem;font-weight:500;--tw-text-opacity:1;color:rgb(107 114 128/var(--tw-text-opacity))}.selector-filter input:focus{outline:2px solid #0000;outline-offset:2px}:is(.dark .selector-filter input){--tw-bg-opacity:1;background-color:rgb(31 41 55/var(--tw-bg-opacity));--tw-text-opacity:1;color:rgb(156 163 175/var(--tw-text-opacity))}.selector-chooseall,.selector-clearall{display:block;border-top-width:1px;padding-top:.5rem;padding-bottom:.5rem;text-align:center;font-size:.875rem;line-height:1.25rem;--tw-text-opacity:1;color:rgb(var(--color-primary-500)/var(--tw-text-opacity));-webkit-text-decoration-line:underline;text-decoration-line:underline}:is(.dark .selector-chooseall),:is(.dark .selector-clearall){--tw-border-opacity:1;border-color:rgb(55 65 81/var(--tw-border-opacity))}.selector-clearall{--tw-text-opacity:1;color:rgb(220 38 38/var(--tw-text-opacity))}:is(.dark .selector-clearall){--tw-text-opacity:1;color:rgb(239 68 68/var(--tw-text-opacity))}.selector-chooser{margin-top:1rem;margin-bottom:1rem;display:flex;width:3.5rem;flex-direction:column;font-size:0;line-height:1}.selector-chooser li{padding-top:.25rem;padding-bottom:.25rem;text-align:center}.selector-add:after,.selector-remove:after{width:1.25rem;--tw-text-opacity:1;color:rgb(156 163 175/var(--tw-text-opacity));font-family:Material Symbols Outlined;font-weight:400;font-style:normal;font-size:18px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-moz-font-feature-settings:"liga";-moz-osx-font-smoothing:grayscale}.selector-add:after{content:"arrow_forward"}.selector-remove:after{content:"arrow_back"}#page input[type=checkbox].empty-form,.empty-form{display:none}.add-row{--tw-bg-opacity:1;background-color:rgb(249 250 251/var(--tw-bg-opacity));padding:1.25rem .75rem;text-align:left;text-align:right;vertical-align:middle;font-size:.875rem;line-height:1.25rem;font-weight:400}:is(.dark .add-row){--tw-bg-opacity:1;background-color:rgb(17 24 39/var(--tw-bg-opacity))}[data-inline-type=stacked] .add-row{overflow:hidden;border-top-width:1px;--tw-border-opacity:1;border-color:rgb(229 231 235/var(--tw-border-opacity))}:is(.dark [data-inline-type=stacked] .add-row){--tw-border-opacity:1;border-color:rgb(31 41 55/var(--tw-border-opacity))}.add-row td{padding:1rem .75rem}.add-row a{display:block;border-radius:.375rem;border-width:1px;--tw-bg-opacity:1;background-color:rgb(255 255 255/var(--tw-bg-opacity));padding:.5rem .75rem;text-align:center;font-size:.875rem;line-height:1.25rem;font-weight:500;--tw-text-opacity:1;color:rgb(107 114 128/var(--tw-text-opacity));transition-property:all;transition-timing-function:cubic-bezier(.4,0,.2,1);transition-duration:.15s}:is(.dark .add-row a){--tw-border-opacity:1;border-color:rgb(55 65 81/var(--tw-border-opacity));--tw-bg-opacity:1;background-color:rgb(17 24 39/var(--tw-bg-opacity));--tw-text-opacity:1;color:rgb(156 163 175/var(--tw-text-opacity))}:is(.dark .add-row a:hover){--tw-text-opacity:1;color:rgb(229 231 235/var(--tw-text-opacity))}@media (min-width:1024px){.add-row a{float:right}}h3 .delete label{--tw-text-opacity:1;color:rgb(107 114 128/var(--tw-text-opacity))}.inline-deletelink{display:block;font-size:.875rem;line-height:1.25rem;line-height:1;--tw-text-opacity:1;color:rgb(220 38 38/var(--tw-text-opacity));-webkit-text-decoration-line:underline;text-decoration-line:underline}:is(.dark .inline-deletelink){--tw-text-opacity:1;color:rgb(239 68 68/var(--tw-text-opacity))}td .inline-deletelink{display:block}@media (min-width:1024px){td .inline-deletelink{margin-top:.625rem}}h3 span:nth-child(3){margin-left:auto}.select2.select2-container{width:100%;max-width:42rem;border-radius:.375rem;border-width:1px;--tw-shadow:0 1px 2px 0 #0000000d;--tw-shadow-colored:0 1px 2px 0 var(--tw-shadow-color);box-shadow:var(--tw-ring-offset-shadow,0 0 #0000),var(--tw-ring-shadow,0 0 #0000),var(--tw-shadow)}:is(.dark .select2.select2-container){--tw-border-opacity:1;border-color:rgb(55 65 81/var(--tw-border-opacity))}.select2.select2-container{width:100%!important}.errors .select2.select2-container{--tw-border-opacity:1;border-color:rgb(220 38 38/var(--tw-border-opacity))}.select2-container.select2-container--admin-autocomplete .select2-selection--single{height:auto}.select2-container.select2-container--admin-autocomplete .select2-selection--single .select2-selection__rendered{height:2.25rem;padding:.5rem .75rem;font-size:.875rem;line-height:1.25rem;font-weight:500;--tw-text-opacity:1;color:rgb(107 114 128/var(--tw-text-opacity))}:is(.dark .select2-container.select2-container--admin-autocomplete .select2-selection--single .select2-selection__rendered){--tw-text-opacity:1;color:rgb(156 163 175/var(--tw-text-opacity))}.select2-container.select2-container--admin-autocomplete .select2-selection--single .select2-selection__clear{margin-right:1.25rem;margin-top:-.5rem;display:flex;height:2.25rem;align-items:center;font-size:0;line-height:1}.select2-container.select2-container--admin-autocomplete .select2-selection--single .select2-selection__clear:after{--tw-text-opacity:1;color:rgb(107 114 128/var(--tw-text-opacity));font-family:Material Symbols Outlined;font-weight:400;font-style:normal;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-moz-font-feature-settings:"liga";-moz-osx-font-smoothing:grayscale;content:"close";font-size:14px}.select2-container.select2-container--admin-autocomplete .select2-selection--single .select2-selection__arrow{margin-right:.5rem;margin-top:-1px;display:flex;height:2.25rem;align-items:center}.select2-container.select2-container--admin-autocomplete .select2-selection--single .select2-selection__arrow:after{left:0;margin:0;font-size:1.125rem;line-height:1.75rem;--tw-text-opacity:1;color:rgb(107 114 128/var(--tw-text-opacity));font-family:Material Symbols Outlined;font-weight:400;font-style:normal;font-size:18px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-moz-font-feature-settings:"liga";-moz-osx-font-smoothing:grayscale;content:"expand_more"}#page input[type=checkbox].select2-container.select2-container--admin-autocomplete .select2-selection--single .select2-selection__arrow b,.select2-container.select2-container--admin-autocomplete .select2-selection--single .select2-selection__arrow b{display:none}.select2-container.select2-container--admin-autocomplete .select2-search--dropdown{display:flex;padding:.5rem .75rem}.select2-container.select2-container--admin-autocomplete .select2-search--dropdown .select2-search__field{margin-left:0;margin-right:0;width:auto;flex-grow:1;border-radius:.375rem;border-width:1px;border-style:solid;--tw-border-opacity:1;border-color:rgb(229 231 235/var(--tw-border-opacity));--tw-bg-opacity:1;background-color:rgb(249 250 251/var(--tw-bg-opacity));padding:.5rem .75rem;font-size:.875rem;line-height:1.25rem;font-weight:500;--tw-text-opacity:1;color:rgb(107 114 128/var(--tw-text-opacity));--tw-shadow:0 1px 2px 0 #0000000d;--tw-shadow-colored:0 1px 2px 0 var(--tw-shadow-color);box-shadow:var(--tw-ring-offset-shadow,0 0 #0000),var(--tw-ring-shadow,0 0 #0000),var(--tw-shadow);outline:2px solid #0000;outline-offset:2px}:is(.dark .select2-container.select2-container--admin-autocomplete .select2-search--dropdown .select2-search__field){--tw-border-opacity:1;border-color:rgb(31 41 55/var(--tw-border-opacity));--tw-bg-opacity:1;background-color:rgb(31 41 55/var(--tw-bg-opacity));--tw-text-opacity:1;color:rgb(156 163 175/var(--tw-text-opacity))}.select2-container.select2-container--admin-autocomplete.select2-container--open.select2-container--above{border-top-left-radius:0;border-top-right-radius:0}.select2-container.select2-container--admin-autocomplete.select2-container--open.select2-container--below{border-bottom-right-radius:0;border-bottom-left-radius:0}.select2-container.select2-container--open .select2-dropdown{border-width:1px;--tw-border-opacity:1;border-color:rgb(229 231 235/var(--tw-border-opacity));padding-bottom:.5rem;--tw-shadow:0 1px 2px 0 #0000000d;--tw-shadow-colored:0 1px 2px 0 var(--tw-shadow-color);box-shadow:var(--tw-ring-offset-shadow,0 0 #0000),var(--tw-ring-shadow,0 0 #0000),var(--tw-shadow)}:is(.dark .select2-container.select2-container--open .select2-dropdown){--tw-border-opacity:1;border-color:rgb(55 65 81/var(--tw-border-opacity));--tw-bg-opacity:1;background-color:rgb(17 24 39/var(--tw-bg-opacity))}.select2-container.select2-container--open .select2-dropdown--below{border-top-left-radius:0;border-top-right-radius:0;border-bottom-right-radius:.375rem;border-bottom-left-radius:.375rem}.select2-container.select2-container--open .select2-dropdown--above{border-bottom-right-radius:0;border-bottom-left-radius:0;border-top-left-radius:.375rem;border-top-right-radius:.375rem}.select2-container.select2-container--admin-autocomplete .select2-results__option{display:block;padding:.5rem .75rem;font-size:.875rem;line-height:1.25rem;--tw-text-opacity:1;color:rgb(107 114 128/var(--tw-text-opacity));transition-property:all;transition-timing-function:cubic-bezier(.4,0,.2,1);transition-duration:.15s}:is(.dark .select2-container.select2-container--admin-autocomplete .select2-results__option){--tw-text-opacity:1;color:rgb(156 163 175/var(--tw-text-opacity))}.select2-container.select2-container--admin-autocomplete .select2-results__option--highlighted[aria-selected]{--tw-text-opacity:1;color:rgb(var(--color-primary-500)/var(--tw-text-opacity))}.select2-container--admin-autocomplete .select2-selection--multiple li.select2-selection__choice{display:flex;height:1.75rem;align-items:center;--tw-bg-opacity:1;background-color:rgb(243 244 246/var(--tw-bg-opacity));padding-left:.5rem;padding-right:.5rem;font-size:.875rem;line-height:1.25rem;font-weight:500;--tw-text-opacity:1;color:rgb(107 114 128/var(--tw-text-opacity));transition-property:all;transition-timing-function:cubic-bezier(.4,0,.2,1);transition-duration:.15s}:is(.dark .select2-container--admin-autocomplete .select2-selection--multiple li.select2-selection__choice){--tw-bg-opacity:1;background-color:rgb(31 41 55/var(--tw-bg-opacity));--tw-text-opacity:1;color:rgb(156 163 175/var(--tw-text-opacity))}:is(.dark .select2-container--admin-autocomplete .select2-selection--multiple li.select2-selection__choice:hover){--tw-text-opacity:1;color:rgb(229 231 235/var(--tw-text-opacity))}.select2-container--admin-autocomplete .select2-selection--multiple li.select2-selection__choice .select2-selection__choice__remove{font-size:0;line-height:1}.select2-container--admin-autocomplete .select2-selection--multiple li.select2-selection__choice .select2-selection__choice__remove:hover{--tw-text-opacity:1;color:rgb(75 85 99/var(--tw-text-opacity))}:is(.dark .select2-container--admin-autocomplete .select2-selection--multiple li.select2-selection__choice .select2-selection__choice__remove:hover){--tw-text-opacity:1;color:rgb(229 231 235/var(--tw-text-opacity))}.select2-container--admin-autocomplete .select2-selection--multiple li.select2-selection__choice .select2-selection__choice__remove:after{font-family:Material Symbols Outlined;font-weight:400;font-style:normal;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-moz-font-feature-settings:"liga";-moz-osx-font-smoothing:grayscale;content:"close";font-size:14px}.select2-container--admin-autocomplete .select2-selection--multiple li.select2-search--inline .select2-search__field{height:1.75rem;font-size:.875rem;line-height:1.25rem;--tw-text-opacity:1;color:rgb(107 114 128/var(--tw-text-opacity))}fieldset.collapsed>div{display:none}fieldset.collapse{visibility:visible}fieldset.collapsed,fieldset.collapsed h2{display:block}fieldset.collapsed .collapse-toggle{display:inline}.calendarbox{z-index:50;width:20rem;border-radius:.375rem;border-width:1px;--tw-bg-opacity:1;background-color:rgb(255 255 255/var(--tw-bg-opacity));font-size:.875rem;line-height:1.25rem;--tw-text-opacity:1;color:rgb(107 114 128/var(--tw-text-opacity));--tw-shadow:0 1px 2px 0 #0000000d;--tw-shadow-colored:0 1px 2px 0 var(--tw-shadow-color);box-shadow:var(--tw-ring-offset-shadow,0 0 #0000),var(--tw-ring-shadow,0 0 #0000),var(--tw-shadow)}:is(.dark .calendarbox){--tw-border-opacity:1;border-color:rgb(55 65 81/var(--tw-border-opacity));--tw-bg-opacity:1;background-color:rgb(31 41 55/var(--tw-bg-opacity))}.calendar caption{margin-bottom:.75rem;padding-top:.75rem;padding-bottom:.75rem;font-weight:500;--tw-text-opacity:1;color:rgb(55 65 81/var(--tw-text-opacity))}:is(.dark .calendar caption){--tw-text-opacity:1;color:rgb(229 231 235/var(--tw-text-opacity))}.calendar table{margin-bottom:.75rem;width:100%}.calendar table th{text-align:center;font-size:.75rem;line-height:1rem;font-weight:500;--tw-text-opacity:1;color:rgb(55 65 81/var(--tw-text-opacity))}:is(.dark .calendar table th){--tw-text-opacity:1;color:rgb(229 231 235/var(--tw-text-opacity))}.calendar table td{height:2.5rem;width:2.5rem;padding:.25rem;text-align:center}.calendar table td a{display:block;display:flex;height:2rem;width:2rem;align-items:center;justify-content:center;border-radius:9999px;transition-property:all;transition-timing-function:cubic-bezier(.4,0,.2,1);transition-duration:.15s}:is(.dark .calendar table td a){--tw-text-opacity:1;color:rgb(156 163 175/var(--tw-text-opacity))}.calendar table td a:hover{--tw-bg-opacity:1;background-color:rgb(243 244 246/var(--tw-bg-opacity));--tw-text-opacity:1;color:rgb(55 65 81/var(--tw-text-opacity))}.calendar table td.today a{--tw-bg-opacity:1;background-color:rgb(var(--color-primary-600)/var(--tw-bg-opacity));font-weight:500;--tw-text-opacity:1;color:rgb(255 255 255/var(--tw-text-opacity))}.calendar-shortcuts{margin-bottom:.75rem;display:flex;flex-direction:row;justify-content:center;border-bottom-right-radius:.375rem;border-bottom-left-radius:.375rem;padding-left:.25rem;padding-right:.25rem;font-size:0;line-height:1}.calendar-shortcuts a{margin-left:.25rem;margin-right:.25rem;width:33.333333%;border-radius:.375rem;border-width:1px;padding:.5rem;text-align:center;font-size:.75rem;line-height:1rem;font-weight:500;line-height:1;--tw-text-opacity:1;color:rgb(107 114 128/var(--tw-text-opacity));--tw-shadow:0 1px 2px 0 #0000000d;--tw-shadow-colored:0 1px 2px 0 var(--tw-shadow-color);box-shadow:var(--tw-ring-offset-shadow,0 0 #0000),var(--tw-ring-shadow,0 0 #0000),var(--tw-shadow);transition-property:all;transition-timing-function:cubic-bezier(.4,0,.2,1);transition-duration:.15s}:is(.dark .calendar-shortcuts a){--tw-border-opacity:1;border-color:rgb(55 65 81/var(--tw-border-opacity));--tw-text-opacity:1;color:rgb(156 163 175/var(--tw-text-opacity))}:is(.dark .calendar-shortcuts a:hover){--tw-border-opacity:1;border-color:rgb(75 85 99/var(--tw-border-opacity));--tw-text-opacity:1;color:rgb(229 231 235/var(--tw-text-opacity))}.calendar-cancel{display:block;border-top-width:1px;padding-top:.5rem;padding-bottom:.5rem;text-align:center;font-size:.75rem;line-height:1rem;--tw-text-opacity:1;color:rgb(220 38 38/var(--tw-text-opacity));-webkit-text-decoration-line:underline;text-decoration-line:underline}:is(.dark .calendar-cancel){--tw-border-opacity:1;border-color:rgb(55 65 81/var(--tw-border-opacity));--tw-text-opacity:1;color:rgb(239 68 68/var(--tw-text-opacity))}.calendarnav-previous{position:absolute;left:0;top:0;margin-left:.5rem;margin-top:.5rem;display:block;font-size:0;line-height:1}.calendarnav-next:after,.calendarnav-previous:after{display:flex;height:1.75rem;width:1.75rem;align-items:center;justify-content:center;border-radius:9999px;border-width:1px;--tw-text-opacity:1;color:rgb(156 163 175/var(--tw-text-opacity));transition-property:all;transition-timing-function:cubic-bezier(.4,0,.2,1);transition-duration:.15s;font-family:Material Symbols Outlined;font-weight:400;font-style:normal;font-size:18px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-moz-font-feature-settings:"liga";-moz-osx-font-smoothing:grayscale}.calendarnav-next:hover:after,.calendarnav-previous:hover:after{--tw-border-opacity:1;border-color:rgb(var(--color-primary-600)/var(--tw-border-opacity));--tw-text-opacity:1;color:rgb(var(--color-primary-500)/var(--tw-text-opacity))}:is(.dark .calendarnav-next):after,:is(.dark .calendarnav-previous):after{--tw-border-opacity:1;border-color:rgb(55 65 81/var(--tw-border-opacity));--tw-bg-opacity:1;background-color:rgb(31 41 55/var(--tw-bg-opacity))}:is(.dark .calendarnav-next:hover):after,:is(.dark .calendarnav-previous:hover):after{border-color:rgb(31 41 55/var(--tw-border-opacity))}.calendarnav-next:after,.calendarnav-previous:after{content:"navigate_before";display:flex}:is(.dark .calendarnav-next:hover):after,:is(.dark .calendarnav-previous:hover):after{--tw-border-opacity:1;border-color:rgb(75 85 99/var(--tw-border-opacity));--tw-text-opacity:1;color:rgb(229 231 235/var(--tw-text-opacity))}.calendarnav-next{position:absolute;right:0;top:0;margin-right:.5rem;margin-top:.5rem;display:block;font-size:0;line-height:1}.calendarnav-next:after{content:"navigate_next";display:flex}.clockbox{z-index:50;border-radius:.375rem;border-width:1px;--tw-bg-opacity:1;background-color:rgb(255 255 255/var(--tw-bg-opacity));font-size:.875rem;line-height:1.25rem;--tw-shadow:0 1px 2px 0 #0000000d;--tw-shadow-colored:0 1px 2px 0 var(--tw-shadow-color);box-shadow:var(--tw-ring-offset-shadow,0 0 #0000),var(--tw-ring-shadow,0 0 #0000),var(--tw-shadow)}:is(.dark .clockbox){--tw-border-opacity:1;border-color:rgb(55 65 81/var(--tw-border-opacity));--tw-bg-opacity:1;background-color:rgb(31 41 55/var(--tw-bg-opacity))}.clockbox h2{padding:.5rem .75rem;font-weight:500;--tw-text-opacity:1;color:rgb(55 65 81/var(--tw-text-opacity))}:is(.dark .clockbox h2){--tw-text-opacity:1;color:rgb(229 231 235/var(--tw-text-opacity))}.clockbox .timelist{padding-left:.75rem;padding-right:.75rem;padding-bottom:.5rem;--tw-text-opacity:1;color:rgb(107 114 128/var(--tw-text-opacity))}:is(.dark .clockbox .timelist){--tw-text-opacity:1;color:rgb(156 163 175/var(--tw-text-opacity))}.clockbox .timelist li{display:block;padding-bottom:.25rem;transition-property:all;transition-timing-function:cubic-bezier(.4,0,.2,1);transition-duration:.15s}.clockbox .timelist li:hover{--tw-text-opacity:1;color:rgb(var(--color-primary-500)/var(--tw-text-opacity))}.field-actions_holder{width:0}.htmx-swapping:before{bottom:0;left:0;right:0;top:0;--tw-bg-opacity:1;background-color:rgb(255 255 255/var(--tw-bg-opacity));opacity:.8;transition-property:all;transition-timing-function:cubic-bezier(.4,0,.2,1);transition-duration:.15s;content:""}.htmx-swapping:after,.htmx-swapping:before{position:absolute}.htmx-swapping:after{inset:50%;height:1rem;width:1rem}@keyframes spin{to{transform:rotate(1turn)}}.htmx-swapping:after{-webkit-animation:spin 1s linear infinite;animation:spin 1s linear infinite;--tw-text-opacity:1;color:rgb(156 163 175/var(--tw-text-opacity));font-family:Material Symbols Outlined;font-weight:400;font-style:normal;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-moz-font-feature-settings:"liga";-moz-osx-font-smoothing:grayscale;font-size:16px;content:"sync"}#changelist-filter .admin-numeric-filter-slider .noUi-handle{right:-1rem;height:1rem;width:1rem;cursor:pointer;border-radius:9999px;border-width:1px;--tw-border-opacity:1;border-color:rgb(229 231 235/var(--tw-border-opacity));--tw-bg-opacity:1;background-color:rgb(255 255 255/var(--tw-bg-opacity));--tw-shadow:0 1px 2px 0 #0000000d;--tw-shadow-colored:0 1px 2px 0 var(--tw-shadow-color);box-shadow:var(--tw-ring-offset-shadow,0 0 #0000),var(--tw-ring-shadow,0 0 #0000),var(--tw-shadow)}:is(.dark #changelist-filter .admin-numeric-filter-slider .noUi-handle){--tw-border-opacity:1;border-color:rgb(229 231 235/var(--tw-border-opacity));--tw-bg-opacity:1;background-color:rgb(229 231 235/var(--tw-bg-opacity))}#changelist-filter .admin-numeric-filter-slider .noUi-handle-upper{right:0}#changelist-filter .admin-numeric-filter-slider .noUi-handle:after,#changelist-filter .admin-numeric-filter-slider .noUi-handle:before{content:none}#changelist-filter .admin-numeric-filter-slider.noUi-target{height:.25rem;border-width:0;--tw-bg-opacity:1;background-color:rgb(229 231 235/var(--tw-bg-opacity));--tw-shadow:0 0 #0000;--tw-shadow-colored:0 0 #0000;box-shadow:var(--tw-ring-offset-shadow,0 0 #0000),var(--tw-ring-shadow,0 0 #0000),var(--tw-shadow)}:is(.dark #changelist-filter .admin-numeric-filter-slider.noUi-target){--tw-bg-opacity:1;background-color:rgb(75 85 99/var(--tw-bg-opacity))}#changelist-filter .admin-numeric-filter-slider .noUi-connect{height:.25rem;border-width:0;--tw-bg-opacity:1;background-color:rgb(var(--color-primary-600)/var(--tw-bg-opacity))}#changelist-filter .admin-numeric-filter-slider-tooltips{margin-bottom:1.25rem;display:flex;flex-direction:row}#changelist-filter .admin-numeric-filter-slider-tooltips>:not([hidden])~:not([hidden]){--tw-space-x-reverse:0;margin-right:calc(1rem*var(--tw-space-x-reverse));margin-left:calc(1rem*(1 - var(--tw-space-x-reverse)))}#changelist-filter .admin-numeric-filter-slider-tooltips{font-size:.875rem;line-height:1.25rem;font-weight:500;--tw-text-opacity:1;color:rgb(107 114 128/var(--tw-text-opacity))}trix-toolbar[id^=trix-toolbar-]{position:sticky;top:0}:is(.dark trix-toolbar[id^=trix-toolbar-]){--tw-bg-opacity:1;background-color:rgb(17 24 39/var(--tw-bg-opacity))}.trix-active{--tw-text-opacity:1;color:rgb(var(--color-primary-600)/var(--tw-text-opacity))}.before\:mr-auto:before{content:var(--tw-content);margin-right:auto}.before\:block:before{content:var(--tw-content);display:block}.before\:w-72:before{content:var(--tw-content);width:18rem}.before\:capitalize:before{content:var(--tw-content);text-transform:capitalize}.before\:text-gray-500:before{content:var(--tw-content);--tw-text-opacity:1;color:rgb(107 114 128/var(--tw-text-opacity))}.before\:content-\[attr\(data-label\)\]:before{--tw-content:attr(data-label);content:var(--tw-content)}.first\:mt-0:first-child{margin-top:0}.last\:mb-0:last-child{margin-bottom:0}.last\:mb-8:last-child{margin-bottom:2rem}.last\:mr-0:last-child{margin-right:0}.last\:border-0:last-child{border-width:0}.last\:border-b-0:last-child{border-bottom-width:0}.focus-within\:border-primary-600:focus-within{--tw-border-opacity:1;border-color:rgb(var(--color-primary-600)/var(--tw-border-opacity))}.focus-within\:ring:focus-within{--tw-ring-offset-shadow:var(--tw-ring-inset) 0 0 0 var(--tw-ring-offset-width) var(--tw-ring-offset-color);--tw-ring-shadow:var(--tw-ring-inset) 0 0 0 calc(3px + var(--tw-ring-offset-width)) var(--tw-ring-color);box-shadow:var(--tw-ring-offset-shadow),var(--tw-ring-shadow),var(--tw-shadow,0 0 #0000)}.focus-within\:ring-primary-300:focus-within{--tw-ring-opacity:1;--tw-ring-color:rgb(var(--color-primary-300)/var(--tw-ring-opacity))}.hover\:bg-gray-100:hover{--tw-bg-opacity:1;background-color:rgb(243 244 246/var(--tw-bg-opacity))}.hover\:bg-gray-50:hover{--tw-bg-opacity:1;background-color:rgb(249 250 251/var(--tw-bg-opacity))}.hover\:bg-red-100:hover{--tw-bg-opacity:1;background-color:rgb(254 226 226/var(--tw-bg-opacity))}.hover\:\!text-primary-600:hover{--tw-text-opacity:1!important;color:rgb(var(--color-primary-600)/var(--tw-text-opacity))!important}.hover\:text-gray-700:hover{--tw-text-opacity:1;color:rgb(55 65 81/var(--tw-text-opacity))}.hover\:text-primary-600:hover{--tw-text-opacity:1;color:rgb(var(--color-primary-600)/var(--tw-text-opacity))}.hover\:text-red-700:hover{--tw-text-opacity:1;color:rgb(185 28 28/var(--tw-text-opacity))}.focus\:border-primary-600:focus{--tw-border-opacity:1;border-color:rgb(var(--color-primary-600)/var(--tw-border-opacity))}.focus\:outline-none:focus{outline:2px solid #0000;outline-offset:2px}.focus\:ring:focus{--tw-ring-offset-shadow:var(--tw-ring-inset) 0 0 0 var(--tw-ring-offset-width) var(--tw-ring-offset-color);--tw-ring-shadow:var(--tw-ring-inset) 0 0 0 calc(3px + var(--tw-ring-offset-width)) var(--tw-ring-color);box-shadow:var(--tw-ring-offset-shadow),var(--tw-ring-shadow),var(--tw-shadow,0 0 #0000)}.focus\:ring-primary-300:focus{--tw-ring-opacity:1;--tw-ring-color:rgb(var(--color-primary-300)/var(--tw-ring-opacity))}.group:hover .group-hover\:-right-1{right:-.25rem}.group:hover .group-hover\:text-gray-400{--tw-text-opacity:1;color:rgb(156 163 175/var(--tw-text-opacity))}.group:hover .group-hover\:text-gray-700{--tw-text-opacity:1;color:rgb(55 65 81/var(--tw-text-opacity))}.group:hover .group-hover\:text-primary-600{--tw-text-opacity:1;color:rgb(var(--color-primary-600)/var(--tw-text-opacity))}.group.inline-stacked .group-\[\.inline-stacked\]\:mx-3,.group.inline-tabular .group-\[\.inline-tabular\]\:mx-3{margin-left:.75rem;margin-right:.75rem}.group.inline-stacked .group-\[\.inline-stacked\]\:mb-3{margin-bottom:.75rem}.group.inline-stacked .group-\[\.inline-stacked\]\:mt-3{margin-top:.75rem}.group.inline-tabular .group-\[\.inline-tabular\]\:mb-0{margin-bottom:0}.group.inline-tabular .group-\[\.inline-tabular\]\:mt-3{margin-top:.75rem}.group.errors .group-\[\.errors\]\:border-red-600{--tw-border-opacity:1;border-color:rgb(220 38 38/var(--tw-border-opacity))}.group.errors .group-\[\.errors\]\:border-x-red-600{--tw-border-opacity:1;border-left-color:rgb(220 38 38/var(--tw-border-opacity));border-right-color:rgb(220 38 38/var(--tw-border-opacity))}.group.errors .group-\[\.errors\]\:border-t-red-600{--tw-border-opacity:1;border-top-color:rgb(220 38 38/var(--tw-border-opacity))}.group.errors .group-\[\.errors\]\:focus\:ring-red-200:focus{--tw-ring-opacity:1;--tw-ring-color:rgb(254 202 202/var(--tw-ring-opacity))}.peer:checked~.peer-checked\:block{display:block}.peer:checked~.peer-checked\:flex{display:flex}.prose-headings\:font-medium :is(:where(h1,h2,h3,h4,h5,h6,th):not(:where([class~=not-prose] *))){font-weight:500}.prose-headings\:text-gray-700 :is(:where(h1,h2,h3,h4,h5,h6,th):not(:where([class~=not-prose] *))){--tw-text-opacity:1;color:rgb(55 65 81/var(--tw-text-opacity))}.prose-a\:text-primary-600 :is(:where(a):not(:where([class~=not-prose] *))){--tw-text-opacity:1;color:rgb(var(--color-primary-600)/var(--tw-text-opacity))}.prose-a\:underline :is(:where(a):not(:where([class~=not-prose] *))){-webkit-text-decoration-line:underline;text-decoration-line:underline}.prose-blockquote\:not-italic :is(:where(blockquote):not(:where([class~=not-prose] *))){font-style:normal}.prose-strong\:text-gray-700 :is(:where(strong):not(:where([class~=not-prose] *))){--tw-text-opacity:1;color:rgb(55 65 81/var(--tw-text-opacity))}.prose-ol\:list-decimal :is(:where(ol):not(:where([class~=not-prose] *))){list-style-type:decimal}.prose-ul\:list-disc :is(:where(ul):not(:where([class~=not-prose] *))){list-style-type:disc}:is(.dark .dark\:border){border-width:1px}:is(.dark .dark\:border-r){border-right-width:1px}:is(.dark .dark\:border-amber-600\/10){border-color:#d977061a}:is(.dark .dark\:border-blue-500\/10){border-color:#3b82f61a}:is(.dark .dark\:border-gray-600){--tw-border-opacity:1;border-color:rgb(75 85 99/var(--tw-border-opacity))}:is(.dark .dark\:border-gray-700){--tw-border-opacity:1;border-color:rgb(55 65 81/var(--tw-border-opacity))}:is(.dark .dark\:border-gray-800){--tw-border-opacity:1;border-color:rgb(31 41 55/var(--tw-border-opacity))}:is(.dark .dark\:border-green-500\/10){border-color:#22c55e1a}:is(.dark .dark\:border-orange-500\/10){border-color:#f973161a}:is(.dark .dark\:border-red-500\/10){border-color:#ef44441a}:is(.dark .dark\:border-red-500\/20){border-color:#ef444433}:is(.dark .dark\:border-transparent){border-color:#0000}:is(.dark .dark\:bg-amber-600\/20){background-color:#d9770633}:is(.dark .dark\:bg-blue-500\/20){background-color:#3b82f633}:is(.dark .dark\:bg-gray-700){--tw-bg-opacity:1;background-color:rgb(55 65 81/var(--tw-bg-opacity))}:is(.dark .dark\:bg-gray-800){--tw-bg-opacity:1;background-color:rgb(31 41 55/var(--tw-bg-opacity))}:is(.dark .dark\:bg-gray-900){--tw-bg-opacity:1;background-color:rgb(17 24 39/var(--tw-bg-opacity))}:is(.dark .dark\:bg-green-500\/20){background-color:#22c55e33}:is(.dark .dark\:bg-orange-500\/20){background-color:#f9731633}:is(.dark .dark\:bg-red-500\/20){background-color:#ef444433}:is(.dark .dark\:bg-white\/\[\.02\]){background-color:#ffffff05}:is(.dark .dark\:bg-white\/\[\.04\]){background-color:#ffffff0a}:is(.dark .dark\:text-gray-200){--tw-text-opacity:1;color:rgb(229 231 235/var(--tw-text-opacity))}:is(.dark .dark\:text-gray-300){--tw-text-opacity:1;color:rgb(209 213 219/var(--tw-text-opacity))}:is(.dark .dark\:text-gray-400){--tw-text-opacity:1;color:rgb(156 163 175/var(--tw-text-opacity))}:is(.dark .dark\:text-gray-500){--tw-text-opacity:1;color:rgb(107 114 128/var(--tw-text-opacity))}:is(.dark .dark\:text-gray-600){--tw-text-opacity:1;color:rgb(75 85 99/var(--tw-text-opacity))}:is(.dark .dark\:text-primary-500){--tw-text-opacity:1;color:rgb(var(--color-primary-500)/var(--tw-text-opacity))}:is(.dark .dark\:text-red-500){--tw-text-opacity:1;color:rgb(239 68 68/var(--tw-text-opacity))}:is(.dark .dark\:before\:text-gray-400):before{content:var(--tw-content);--tw-text-opacity:1;color:rgb(156 163 175/var(--tw-text-opacity))}:is(.dark .dark\:focus-within\:ring-primary-600\/30:focus-within),:is(.dark .focus-within\:dark\:ring-primary-600\/30):focus-within{--tw-ring-color:rgb(var(--color-primary-600)/0.3)}:is(.dark .dark\:hover\:bg-gray-700:hover){--tw-bg-opacity:1;background-color:rgb(55 65 81/var(--tw-bg-opacity))}:is(.dark .dark\:hover\:bg-gray-900:hover){--tw-bg-opacity:1;background-color:rgb(17 24 39/var(--tw-bg-opacity))}:is(.dark .dark\:hover\:bg-red-500\/20:hover){background-color:#ef444433}:is(.dark .dark\:hover\:text-gray-200:hover){--tw-text-opacity:1;color:rgb(229 231 235/var(--tw-text-opacity))}:is(.dark .dark\:hover\:text-red-500:hover){--tw-text-opacity:1;color:rgb(239 68 68/var(--tw-text-opacity))}:is(.dark .hover\:dark\:text-gray-200):hover{--tw-text-opacity:1;color:rgb(229 231 235/var(--tw-text-opacity))}:is(.dark .dark\:focus\:ring-primary-600\/30:focus){--tw-ring-color:rgb(var(--color-primary-600)/0.3)}:is(.dark .group:hover .dark\:group-hover\:text-gray-200){--tw-text-opacity:1;color:rgb(229 231 235/var(--tw-text-opacity))}:is(.dark .group.errors .dark\:group-\[\.errors\]\:border-red-500){--tw-border-opacity:1;border-color:rgb(239 68 68/var(--tw-border-opacity))}:is(.dark .group.errors .dark\:group-\[\.errors\]\:border-x-red-500){--tw-border-opacity:1;border-left-color:rgb(239 68 68/var(--tw-border-opacity));border-right-color:rgb(239 68 68/var(--tw-border-opacity))}:is(.dark .group.errors .dark\:group-\[\.errors\]\:border-t-red-500){--tw-border-opacity:1;border-top-color:rgb(239 68 68/var(--tw-border-opacity))}:is(.dark .group.errors .dark\:group-\[\.errors\]\:focus\:ring-red-600\/40:focus){--tw-ring-color:#dc262666}:is(.dark .dark\:prose-headings\:text-gray-200 :is(:where(h1,h2,h3,h4,h5,h6,th):not(:where([class~=not-prose] *)))){--tw-text-opacity:1;color:rgb(229 231 235/var(--tw-text-opacity))}:is(.dark .dark\:prose-blockquote\:border-gray-700 :is(:where(blockquote):not(:where([class~=not-prose] *)))){--tw-border-opacity:1;border-color:rgb(55 65 81/var(--tw-border-opacity))}:is(.dark .dark\:prose-blockquote\:text-gray-200 :is(:where(blockquote):not(:where([class~=not-prose] *)))){--tw-text-opacity:1;color:rgb(229 231 235/var(--tw-text-opacity))}:is(.dark .dark\:prose-strong\:text-gray-200 :is(:where(strong):not(:where([class~=not-prose] *)))){--tw-text-opacity:1;color:rgb(229 231 235/var(--tw-text-opacity))}@media not all and (min-width:1280px){.max-xl\:fixed{position:fixed}}@media not all and (min-width:768px){.max-md\:w-full{width:100%}}@media (min-width:640px){.sm\:w-96{width:24rem}}@media (min-width:768px){.md\:mb-0{margin-bottom:0}.md\:mb-2{margin-bottom:.5rem}.md\:ml-auto{margin-left:auto}.md\:mr-4{margin-right:1rem}.md\:mr-8{margin-right:2rem}.md\:mt-0{margin-top:0}.md\:block{display:block}.md\:flex-row{flex-direction:row}.md\:items-center{align-items:center}.md\:justify-end{justify-content:flex-end}.md\:border-b{border-bottom-width:1px}.md\:border-b-0{border-bottom-width:0}.md\:border-l-0{border-left-width:0}.md\:border-r-0{border-right-width:0}.md\:border-t-0{border-top-width:0}.md\:border-primary-600{--tw-border-opacity:1;border-color:rgb(var(--color-primary-600)/var(--tw-border-opacity))}.md\:px-0{padding-left:0;padding-right:0}.md\:py-4{padding-top:1rem;padding-bottom:1rem}:is(.dark .dark\:md\:border-gray-800){--tw-border-opacity:1;border-color:rgb(31 41 55/var(--tw-border-opacity))}:is(.dark .dark\:md\:border-primary-600){--tw-border-opacity:1;border-color:rgb(var(--color-primary-600)/var(--tw-border-opacity))}}@media (min-width:1024px){.lg\:-mx-4{margin-left:-1rem;margin-right:-1rem}.lg\:mb-0{margin-bottom:0}.lg\:mb-12{margin-bottom:3rem}.lg\:ml-auto{margin-left:auto}.lg\:mr-3{margin-right:.75rem}.lg\:mt-0{margin-top:0}.lg\:mt-3{margin-top:.75rem}.lg\:mt-8{margin-top:2rem}.lg\:block{display:block}.lg\:table-cell{display:table-cell}.lg\:table-header-group{display:table-header-group}.lg\:table-row{display:table-row}.lg\:w-60{width:15rem}.lg\:w-72{width:18rem}.lg\:w-auto{width:auto}.lg\:w-px{width:1px}.lg\:max-w-xs{max-width:20rem}.lg\:flex-row{flex-direction:row}.lg\:flex-row-reverse{flex-direction:row-reverse}.lg\:rounded-md{border-radius:.375rem}.lg\:border{border-width:1px}.lg\:border-0{border-width:0}.lg\:border-b-0{border-bottom-width:0}.lg\:border-t{border-top-width:1px}.lg\:border-none{border-style:none}.lg\:border-gray-200{--tw-border-opacity:1;border-color:rgb(229 231 235/var(--tw-border-opacity))}.lg\:p-12{padding:3rem}.lg\:px-12{padding-left:3rem;padding-right:3rem}.lg\:py-3{padding-top:.75rem;padding-bottom:.75rem}.lg\:align-top{vertical-align:top}.lg\:underline{-webkit-text-decoration-line:underline;text-decoration-line:underline}.lg\:shadow-none{--tw-shadow:0 0 #0000;--tw-shadow-colored:0 0 #0000}.lg\:shadow-none,.lg\:shadow-sm{box-shadow:var(--tw-ring-offset-shadow,0 0 #0000),var(--tw-ring-shadow,0 0 #0000),var(--tw-shadow)}.lg\:shadow-sm{--tw-shadow:0 1px 2px 0 #0000000d;--tw-shadow-colored:0 1px 2px 0 var(--tw-shadow-color)}.lg\:before\:hidden:before{content:var(--tw-content);display:none}:is(.dark .dark\:lg\:border-gray-800),:is(.dark .lg\:dark\:border-gray-800){--tw-border-opacity:1;border-color:rgb(31 41 55/var(--tw-border-opacity))}}@media (min-width:1280px){.xl\:left-0{left:0}.xl\:left-72{left:18rem}.xl\:block{display:block}.xl\:flex{display:flex}.xl\:hidden{display:none}.xl\:max-w-4xl{max-width:56rem}.xl\:text-base{font-size:1rem;line-height:1.5rem}}
+/*! tailwindcss v3.3.1 | MIT License | https://tailwindcss.com*/*,:after,:before{box-sizing:border-box;border:0 solid #e5e7eb}:after,:before{--tw-content:""}html{line-height:1.5;-webkit-text-size-adjust:100%;-moz-tab-size:4;-o-tab-size:4;tab-size:4;font-family:Inter,sans-serif;font-feature-settings:normal;font-variation-settings:normal}body{margin:0;line-height:inherit}hr{height:0;color:inherit;border-top-width:1px}abbr:where([title]){-webkit-text-decoration:underline dotted;text-decoration:underline dotted}h1,h2,h3,h4,h5,h6{font-size:inherit;font-weight:inherit}a{color:inherit;text-decoration:inherit}b,strong{font-weight:bolder}code,kbd,pre,samp{font-family:ui-monospace,SFMono-Regular,Menlo,Monaco,Consolas,Liberation Mono,Courier New,monospace;font-size:1em}small{font-size:80%}sub,sup{font-size:75%;line-height:0;position:relative;vertical-align:initial}sub{bottom:-.25em}sup{top:-.5em}table{text-indent:0;border-color:inherit;border-collapse:collapse}button,input,optgroup,select,textarea{font-family:inherit;font-size:100%;font-weight:inherit;line-height:inherit;color:inherit;margin:0;padding:0}button,select{text-transform:none}[type=button],[type=reset],[type=submit],button{-webkit-appearance:button;background-color:initial;background-image:none}:-moz-focusring{outline:auto}:-moz-ui-invalid{box-shadow:none}progress{vertical-align:initial}::-webkit-inner-spin-button,::-webkit-outer-spin-button{height:auto}[type=search]{-webkit-appearance:textfield;outline-offset:-2px}::-webkit-search-decoration{-webkit-appearance:none}::-webkit-file-upload-button{-webkit-appearance:button;font:inherit}summary{display:list-item}blockquote,dd,dl,figure,h1,h2,h3,h4,h5,h6,hr,p,pre{margin:0}fieldset{margin:0}fieldset,legend{padding:0}menu,ol,ul{list-style:none;margin:0;padding:0}textarea{resize:vertical}input::-moz-placeholder,textarea::-moz-placeholder{opacity:1;color:#9ca3af}input:-ms-input-placeholder,textarea:-ms-input-placeholder{opacity:1;color:#9ca3af}input::placeholder,textarea::placeholder{opacity:1;color:#9ca3af}[role=button],button{cursor:pointer}:disabled{cursor:default}audio,canvas,embed,iframe,img,object,svg,video{display:block;vertical-align:middle}img,video{max-width:100%;height:auto}[hidden]{display:none}*,:after,:before{--tw-border-spacing-x:0;--tw-border-spacing-y:0;--tw-translate-x:0;--tw-translate-y:0;--tw-rotate:0;--tw-skew-x:0;--tw-skew-y:0;--tw-scale-x:1;--tw-scale-y:1;--tw-pan-x: ;--tw-pan-y: ;--tw-pinch-zoom: ;--tw-scroll-snap-strictness:proximity;--tw-ordinal: ;--tw-slashed-zero: ;--tw-numeric-figure: ;--tw-numeric-spacing: ;--tw-numeric-fraction: ;--tw-ring-inset: ;--tw-ring-offset-width:0px;--tw-ring-offset-color:#fff;--tw-ring-color:#3b82f680;--tw-ring-offset-shadow:0 0 #0000;--tw-ring-shadow:0 0 #0000;--tw-shadow:0 0 #0000;--tw-shadow-colored:0 0 #0000;--tw-blur: ;--tw-brightness: ;--tw-contrast: ;--tw-grayscale: ;--tw-hue-rotate: ;--tw-invert: ;--tw-saturate: ;--tw-sepia: ;--tw-drop-shadow: ;--tw-backdrop-blur: ;--tw-backdrop-brightness: ;--tw-backdrop-contrast: ;--tw-backdrop-grayscale: ;--tw-backdrop-hue-rotate: ;--tw-backdrop-invert: ;--tw-backdrop-opacity: ;--tw-backdrop-saturate: ;--tw-backdrop-sepia: }::-webkit-backdrop{--tw-border-spacing-x:0;--tw-border-spacing-y:0;--tw-translate-x:0;--tw-translate-y:0;--tw-rotate:0;--tw-skew-x:0;--tw-skew-y:0;--tw-scale-x:1;--tw-scale-y:1;--tw-pan-x: ;--tw-pan-y: ;--tw-pinch-zoom: ;--tw-scroll-snap-strictness:proximity;--tw-ordinal: ;--tw-slashed-zero: ;--tw-numeric-figure: ;--tw-numeric-spacing: ;--tw-numeric-fraction: ;--tw-ring-inset: ;--tw-ring-offset-width:0px;--tw-ring-offset-color:#fff;--tw-ring-color:#3b82f680;--tw-ring-offset-shadow:0 0 #0000;--tw-ring-shadow:0 0 #0000;--tw-shadow:0 0 #0000;--tw-shadow-colored:0 0 #0000;--tw-blur: ;--tw-brightness: ;--tw-contrast: ;--tw-grayscale: ;--tw-hue-rotate: ;--tw-invert: ;--tw-saturate: ;--tw-sepia: ;--tw-drop-shadow: ;--tw-backdrop-blur: ;--tw-backdrop-brightness: ;--tw-backdrop-contrast: ;--tw-backdrop-grayscale: ;--tw-backdrop-hue-rotate: ;--tw-backdrop-invert: ;--tw-backdrop-opacity: ;--tw-backdrop-saturate: ;--tw-backdrop-sepia: }::backdrop{--tw-border-spacing-x:0;--tw-border-spacing-y:0;--tw-translate-x:0;--tw-translate-y:0;--tw-rotate:0;--tw-skew-x:0;--tw-skew-y:0;--tw-scale-x:1;--tw-scale-y:1;--tw-pan-x: ;--tw-pan-y: ;--tw-pinch-zoom: ;--tw-scroll-snap-strictness:proximity;--tw-ordinal: ;--tw-slashed-zero: ;--tw-numeric-figure: ;--tw-numeric-spacing: ;--tw-numeric-fraction: ;--tw-ring-inset: ;--tw-ring-offset-width:0px;--tw-ring-offset-color:#fff;--tw-ring-color:#3b82f680;--tw-ring-offset-shadow:0 0 #0000;--tw-ring-shadow:0 0 #0000;--tw-shadow:0 0 #0000;--tw-shadow-colored:0 0 #0000;--tw-blur: ;--tw-brightness: ;--tw-contrast: ;--tw-grayscale: ;--tw-hue-rotate: ;--tw-invert: ;--tw-saturate: ;--tw-sepia: ;--tw-drop-shadow: ;--tw-backdrop-blur: ;--tw-backdrop-brightness: ;--tw-backdrop-contrast: ;--tw-backdrop-grayscale: ;--tw-backdrop-hue-rotate: ;--tw-backdrop-invert: ;--tw-backdrop-opacity: ;--tw-backdrop-saturate: ;--tw-backdrop-sepia: }.container{width:100%}@media (min-width:640px){.container{max-width:640px}}@media (min-width:768px){.container{max-width:768px}}@media (min-width:1024px){.container{max-width:1024px}}@media (min-width:1280px){.container{max-width:1280px}}@media (min-width:1536px){.container{max-width:1536px}}.prose-sm{font-size:.875rem;line-height:1.7142857}.prose-sm :where(p):not(:where([class~=not-prose] *)){margin-top:1.1428571em;margin-bottom:1.1428571em}.prose-sm :where([class~=lead]):not(:where([class~=not-prose] *)){font-size:1.2857143em;line-height:1.5555556;margin-top:.8888889em;margin-bottom:.8888889em}.prose-sm :where(blockquote):not(:where([class~=not-prose] *)){margin-top:1.3333333em;margin-bottom:1.3333333em;padding-left:1.1111111em}.prose-sm :where(h1):not(:where([class~=not-prose] *)){font-size:2.1428571em;margin-top:0;margin-bottom:.8em;line-height:1.2}.prose-sm :where(h2):not(:where([class~=not-prose] *)){font-size:1.4285714em;margin-top:1.6em;margin-bottom:.8em;line-height:1.4}.prose-sm :where(h3):not(:where([class~=not-prose] *)){font-size:1.2857143em;margin-top:1.5555556em;margin-bottom:.4444444em;line-height:1.5555556}.prose-sm :where(h4):not(:where([class~=not-prose] *)){margin-top:1.4285714em;margin-bottom:.5714286em;line-height:1.4285714}.prose-sm :where(img):not(:where([class~=not-prose] *)){margin-top:1.7142857em;margin-bottom:1.7142857em}.prose-sm :where(video):not(:where([class~=not-prose] *)){margin-top:1.7142857em;margin-bottom:1.7142857em}.prose-sm :where(figure):not(:where([class~=not-prose] *)){margin-top:1.7142857em;margin-bottom:1.7142857em}.prose-sm :where(figure>*):not(:where([class~=not-prose] *)){margin-top:0;margin-bottom:0}.prose-sm :where(figcaption):not(:where([class~=not-prose] *)){font-size:.8571429em;line-height:1.3333333;margin-top:.6666667em}.prose-sm :where(code):not(:where([class~=not-prose] *)){font-size:.8571429em}.prose-sm :where(h2 code):not(:where([class~=not-prose] *)){font-size:.9em}.prose-sm :where(h3 code):not(:where([class~=not-prose] *)){font-size:.8888889em}.prose-sm :where(pre):not(:where([class~=not-prose] *)){font-size:.8571429em;line-height:1.6666667;margin-top:1.6666667em;margin-bottom:1.6666667em;border-radius:.25rem;padding:.6666667em 1em}.prose-sm :where(ol):not(:where([class~=not-prose] *)){margin-top:1.1428571em;margin-bottom:1.1428571em;padding-left:1.5714286em}.prose-sm :where(ul):not(:where([class~=not-prose] *)){margin-top:1.1428571em;margin-bottom:1.1428571em;padding-left:1.5714286em}.prose-sm :where(li):not(:where([class~=not-prose] *)){margin-top:.2857143em;margin-bottom:.2857143em}.prose-sm :where(ol>li):not(:where([class~=not-prose] *)){padding-left:.4285714em}.prose-sm :where(ul>li):not(:where([class~=not-prose] *)){padding-left:.4285714em}.prose-sm :where(.prose-sm>ul>li p):not(:where([class~=not-prose] *)){margin-top:.5714286em;margin-bottom:.5714286em}.prose-sm :where(.prose-sm>ul>li>:first-child):not(:where([class~=not-prose] *)){margin-top:1.1428571em}.prose-sm :where(.prose-sm>ul>li>:last-child):not(:where([class~=not-prose] *)){margin-bottom:1.1428571em}.prose-sm :where(.prose-sm>ol>li>:first-child):not(:where([class~=not-prose] *)){margin-top:1.1428571em}.prose-sm :where(.prose-sm>ol>li>:last-child):not(:where([class~=not-prose] *)){margin-bottom:1.1428571em}.prose-sm :where(ul ul,ul ol,ol ul,ol ol):not(:where([class~=not-prose] *)){margin-top:.5714286em;margin-bottom:.5714286em}.prose-sm :where(hr):not(:where([class~=not-prose] *)){margin-top:2.8571429em;margin-bottom:2.8571429em}.prose-sm :where(hr+*):not(:where([class~=not-prose] *)){margin-top:0}.prose-sm :where(h2+*):not(:where([class~=not-prose] *)){margin-top:0}.prose-sm :where(h3+*):not(:where([class~=not-prose] *)){margin-top:0}.prose-sm :where(h4+*):not(:where([class~=not-prose] *)){margin-top:0}.prose-sm :where(table):not(:where([class~=not-prose] *)){font-size:.8571429em;line-height:1.5}.prose-sm :where(thead th):not(:where([class~=not-prose] *)){padding-right:1em;padding-bottom:.6666667em;padding-left:1em}.prose-sm :where(thead th:first-child):not(:where([class~=not-prose] *)){padding-left:0}.prose-sm :where(thead th:last-child):not(:where([class~=not-prose] *)){padding-right:0}.prose-sm :where(tbody td,tfoot td):not(:where([class~=not-prose] *)){padding:.6666667em 1em}.prose-sm :where(tbody td:first-child,tfoot td:first-child):not(:where([class~=not-prose] *)){padding-left:0}.prose-sm :where(tbody td:last-child,tfoot td:last-child):not(:where([class~=not-prose] *)){padding-right:0}.prose-sm :where(.prose-sm>:first-child):not(:where([class~=not-prose] *)){margin-top:0}.prose-sm :where(.prose-sm>:last-child):not(:where([class~=not-prose] *)){margin-bottom:0}.visible{visibility:visible}.invisible{visibility:hidden}.collapse{visibility:collapse}.static{position:static}.fixed{position:fixed}.absolute{position:absolute}.relative{position:relative}.sticky{position:sticky}.-bottom-px{bottom:-1px}.-right-2{right:-.5rem}.bottom-0{bottom:0}.bottom-4{bottom:1rem}.left-0{left:0}.left-72{left:18rem}.right-0{right:0}.right-2{right:.5rem}.right-4{right:1rem}.top-0{top:0}.top-2{top:.5rem}.top-5{top:1.25rem}.top-7{top:1.75rem}.z-10{z-index:10}.z-20{z-index:20}.z-30{z-index:30}.z-50{z-index:50}.-mx-2{margin-left:-.5rem;margin-right:-.5rem}.-mx-3{margin-left:-.75rem;margin-right:-.75rem}.-mx-4{margin-left:-1rem;margin-right:-1rem}.-my-1{margin-top:-.25rem;margin-bottom:-.25rem}.-my-3{margin-top:-.75rem;margin-bottom:-.75rem}.mx-1{margin-left:.25rem;margin-right:.25rem}.mx-2{margin-left:.5rem;margin-right:.5rem}.mx-3{margin-left:.75rem;margin-right:.75rem}.mx-6{margin-left:1.5rem;margin-right:1.5rem}.mx-auto{margin-left:auto;margin-right:auto}.my-2{margin-top:.5rem;margin-bottom:.5rem}.my-3{margin-top:.75rem;margin-bottom:.75rem}.my-4{margin-top:1rem;margin-bottom:1rem}.my-6{margin-top:1.5rem;margin-bottom:1.5rem}.my-12{margin-top:3rem;margin-bottom:3rem}.my-8{margin-top:2rem;margin-bottom:2rem}.-mb-5{margin-bottom:-1.25rem}.-mb-px{margin-bottom:-1px}.-mr-1{margin-right:-.25rem}.mb-1{margin-bottom:.25rem}.mb-10{margin-bottom:2.5rem}.mb-12{margin-bottom:3rem}.mb-2{margin-bottom:.5rem}.mb-3{margin-bottom:.75rem}.mb-4{margin-bottom:1rem}.mb-5{margin-bottom:1.25rem}.mb-6{margin-bottom:1.5rem}.mb-8{margin-bottom:2rem}.ml-1{margin-left:.25rem}.ml-2{margin-left:.5rem}.ml-3{margin-left:.75rem}.ml-4{margin-left:1rem}.ml-6{margin-left:1.5rem}.ml-72{margin-left:18rem}.ml-auto{margin-left:auto}.mr-1{margin-right:.25rem}.mr-2{margin-right:.5rem}.mr-3{margin-right:.75rem}.mr-4{margin-right:1rem}.mr-auto{margin-right:auto}.mt-0{margin-top:0}.mt-0\.5{margin-top:.125rem}.mt-1{margin-top:.25rem}.mt-12{margin-top:3rem}.mt-2{margin-top:.5rem}.mt-20{margin-top:5rem}.mt-3{margin-top:.75rem}.mt-4{margin-top:1rem}.mt-auto{margin-top:auto}.mt-8{margin-top:2rem}.block{display:block}.inline-block{display:inline-block}.inline{display:inline}.flex{display:flex}.table{display:table}.contents{display:contents}.hidden{display:none}.h-1{height:.25rem}.h-10{height:2.5rem}.h-11{height:2.75rem}.h-16{height:4rem}.h-4{height:1rem}.h-5{height:1.25rem}.h-6{height:1.5rem}.h-8{height:2rem}.h-9{height:2.25rem}.h-9\.5{height:2.375rem}.h-full{height:100%}.max-h-screen{max-height:100vh}.min-h-screen{min-height:100vh}.w-1{width:.25rem}.w-10{width:2.5rem}.w-36{width:9rem}.w-4\/12{width:33.333333%}.w-40{width:10rem}.w-48{width:12rem}.w-52{width:13rem}.w-6{width:1.5rem}.w-72{width:18rem}.w-8{width:2rem}.w-80{width:20rem}.w-9{width:2.25rem}.w-9\.5{width:2.375rem}.w-96{width:24rem}.w-full{width:100%}.w-px{width:1px}.w-screen{width:100vw}.w-sidebar{width:18rem}.w-12{width:3rem}.min-w-0{min-width:0}.min-w-sidebar{min-width:18rem}.max-w-2xl{max-width:42rem}.max-w-3xl{max-width:48rem}.max-w-4xl{max-width:56rem}.max-w-none{max-width:none}.flex-none{flex:none}.flex-shrink-0,.shrink-0{flex-shrink:0}.flex-grow{flex-grow:1}.grow-0{flex-grow:0}.basis-1\/2{flex-basis:50%}.table-fixed{table-layout:fixed}.border-separate{border-collapse:initial}.-translate-x-1\/2{--tw-translate-x:-50%}.-translate-x-1\/2,.translate-y-full{transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}.translate-y-full{--tw-translate-y:100%}.rotate-180{--tw-rotate:180deg}.rotate-180,.transform{transform:translate(var(--tw-translate-x),var(--tw-translate-y)) rotate(var(--tw-rotate)) skewX(var(--tw-skew-x)) skewY(var(--tw-skew-y)) scaleX(var(--tw-scale-x)) scaleY(var(--tw-scale-y))}@-webkit-keyframes spin{to{transform:rotate(1turn)}}.animate-spin{-webkit-animation:spin 1s linear infinite;animation:spin 1s linear infinite}.cursor-not-allowed{cursor:not-allowed}.cursor-pointer{cursor:pointer}.resize-none{resize:none}.resize{resize:both}.appearance-none{-webkit-appearance:none;-moz-appearance:none;appearance:none}.flex-row{flex-direction:row}.flex-col{flex-direction:column}.flex-col-reverse{flex-direction:column-reverse}.flex-wrap{flex-wrap:wrap}.items-start{align-items:flex-start}.items-center{align-items:center}.justify-start{justify-content:flex-start}.justify-end{justify-content:flex-end}.justify-center{justify-content:center}.gap-x-8{-moz-column-gap:2rem;column-gap:2rem}.space-x-4>:not([hidden])~:not([hidden]){--tw-space-x-reverse:0;margin-right:calc(1rem*var(--tw-space-x-reverse));margin-left:calc(1rem*(1 - var(--tw-space-x-reverse)))}.space-y-4>:not([hidden])~:not([hidden]){--tw-space-y-reverse:0;margin-top:calc(1rem*(1 - var(--tw-space-y-reverse)));margin-bottom:calc(1rem*var(--tw-space-y-reverse))}.self-end{align-self:flex-end}.self-center{align-self:center}.self-stretch{align-self:stretch}.overflow-auto{overflow:auto}.overflow-hidden{overflow:hidden}.overflow-y-auto{overflow-y:auto}.overflow-x-hidden{overflow-x:hidden}.truncate{overflow:hidden;white-space:nowrap}.text-ellipsis,.truncate{text-overflow:ellipsis}.whitespace-nowrap{white-space:nowrap}.break-words{overflow-wrap:break-word}.rounded{border-radius:.25rem}.rounded-full{border-radius:9999px}.rounded-md{border-radius:.375rem}.rounded-sm{border-radius:.125rem}.rounded-b{border-bottom-right-radius:.25rem;border-bottom-left-radius:.25rem}.rounded-b-md{border-bottom-right-radius:.375rem;border-bottom-left-radius:.375rem}.rounded-t-md{border-top-left-radius:.375rem;border-top-right-radius:.375rem}.rounded-t-none{border-top-left-radius:0;border-top-right-radius:0}.border{border-width:1px}.border-0{border-width:0}.border-b{border-bottom-width:1px}.border-l-4{border-left-width:4px}.border-r{border-right-width:1px}.border-t{border-top-width:1px}.border-t-0{border-top-width:0}.border-blue-200{--tw-border-opacity:1;border-color:rgb(191 219 254/var(--tw-border-opacity))}.border-gray-100{--tw-border-opacity:1;border-color:rgb(243 244 246/var(--tw-border-opacity))}.border-gray-200{--tw-border-opacity:1;border-color:rgb(229 231 235/var(--tw-border-opacity))}.border-green-200{--tw-border-opacity:1;border-color:rgb(187 247 208/var(--tw-border-opacity))}.border-orange-200{--tw-border-opacity:1;border-color:rgb(254 215 170/var(--tw-border-opacity))}.border-primary-600{--tw-border-opacity:1;border-color:rgb(var(--color-primary-600)/var(--tw-border-opacity))}.border-red-200{--tw-border-opacity:1;border-color:rgb(254 202 202/var(--tw-border-opacity))}.border-red-500{--tw-border-opacity:1;border-color:rgb(239 68 68/var(--tw-border-opacity))}.border-transparent{border-color:#0000}.border-red-600{--tw-border-opacity:1;border-color:rgb(220 38 38/var(--tw-border-opacity))}.bg-amber-100{--tw-bg-opacity:1;background-color:rgb(254 243 199/var(--tw-bg-opacity))}.bg-blue-50{--tw-bg-opacity:1;background-color:rgb(239 246 255/var(--tw-bg-opacity))}.bg-gray-100{--tw-bg-opacity:1;background-color:rgb(243 244 246/var(--tw-bg-opacity))}.bg-gray-200{--tw-bg-opacity:1;background-color:rgb(229 231 235/var(--tw-bg-opacity))}.bg-gray-50{--tw-bg-opacity:1;background-color:rgb(249 250 251/var(--tw-bg-opacity))}.bg-gray-500{--tw-bg-opacity:1;background-color:rgb(107 114 128/var(--tw-bg-opacity))}.bg-gray-700{--tw-bg-opacity:1;background-color:rgb(55 65 81/var(--tw-bg-opacity))}.bg-gray-900{--tw-bg-opacity:1;background-color:rgb(17 24 39/var(--tw-bg-opacity))}.bg-green-100{--tw-bg-opacity:1;background-color:rgb(220 252 231/var(--tw-bg-opacity))}.bg-green-50{--tw-bg-opacity:1;background-color:rgb(240 253 244/var(--tw-bg-opacity))}.bg-green-500{--tw-bg-opacity:1;background-color:rgb(34 197 94/var(--tw-bg-opacity))}.bg-orange-50{--tw-bg-opacity:1;background-color:rgb(255 247 237/var(--tw-bg-opacity))}.bg-primary-100{--tw-bg-opacity:1;background-color:rgb(var(--color-primary-100)/var(--tw-bg-opacity))}.bg-primary-600{--tw-bg-opacity:1;background-color:rgb(var(--color-primary-600)/var(--tw-bg-opacity))}.bg-red-100{--tw-bg-opacity:1;background-color:rgb(254 226 226/var(--tw-bg-opacity))}.bg-red-50{--tw-bg-opacity:1;background-color:rgb(254 242 242/var(--tw-bg-opacity))}.bg-red-500{--tw-bg-opacity:1;background-color:rgb(239 68 68/var(--tw-bg-opacity))}.bg-red-600{--tw-bg-opacity:1;background-color:rgb(220 38 38/var(--tw-bg-opacity))}.bg-white{--tw-bg-opacity:1;background-color:rgb(255 255 255/var(--tw-bg-opacity))}.bg-red-200{--tw-bg-opacity:1;background-color:rgb(254 202 202/var(--tw-bg-opacity))}.bg-opacity-80{--tw-bg-opacity:0.8}.bg-none{background-image:none}.bg-cover{background-size:cover}.bg-center{background-position:50%}.bg-no-repeat{background-repeat:no-repeat}.p-1{padding:.25rem}.p-3{padding:.75rem}.p-4{padding:1rem}.px-1{padding-left:.25rem;padding-right:.25rem}.px-12{padding-left:3rem;padding-right:3rem}.px-2{padding-left:.5rem;padding-right:.5rem}.px-3{padding-left:.75rem;padding-right:.75rem}.px-4{padding-left:1rem;padding-right:1rem}.px-6{padding-left:1.5rem;padding-right:1.5rem}.px-8{padding-left:2rem;padding-right:2rem}.py-1{padding-top:.25rem;padding-bottom:.25rem}.py-1\.5{padding-top:.375rem;padding-bottom:.375rem}.py-2{padding-top:.5rem;padding-bottom:.5rem}.py-3{padding-top:.75rem;padding-bottom:.75rem}.py-4{padding-top:1rem;padding-bottom:1rem}.py-5{padding-top:1.25rem;padding-bottom:1.25rem}.pb-1{padding-bottom:.25rem}.pb-12{padding-bottom:3rem}.pb-16{padding-bottom:4rem}.pl-2{padding-left:.5rem}.pl-3{padding-left:.75rem}.pl-4{padding-left:1rem}.pr-2{padding-right:.5rem}.pr-3{padding-right:.75rem}.pr-4{padding-right:1rem}.pr-8{padding-right:2rem}.pt-1{padding-top:.25rem}.pt-3{padding-top:.75rem}.text-left{text-align:left}.text-center{text-align:center}.text-right{text-align:right}.align-top{vertical-align:top}.align-middle{vertical-align:middle}.align-text-top{vertical-align:text-top}.font-sans{font-family:Inter,sans-serif}.text-lg{font-size:1.125rem;line-height:1.75rem}.text-sm{font-size:.875rem;line-height:1.25rem}.text-xl{font-size:1.25rem;line-height:1.75rem}.text-xs{font-size:.75rem;line-height:1rem}.text-xxs{font-size:11px;line-height:14px}.font-medium{font-weight:500}.font-normal{font-weight:400}.font-semibold{font-weight:600}.uppercase{text-transform:uppercase}.capitalize{text-transform:capitalize}.italic{font-style:italic}.leading-none{line-height:1}.leading-relaxed{line-height:1.625}.text-amber-600{--tw-text-opacity:1;color:rgb(217 119 6/var(--tw-text-opacity))}.text-blue-500{--tw-text-opacity:1;color:rgb(59 130 246/var(--tw-text-opacity))}.text-blue-700{--tw-text-opacity:1;color:rgb(29 78 216/var(--tw-text-opacity))}.text-gray-200{--tw-text-opacity:1;color:rgb(229 231 235/var(--tw-text-opacity))}.text-gray-300{--tw-text-opacity:1;color:rgb(209 213 219/var(--tw-text-opacity))}.text-gray-400{--tw-text-opacity:1;color:rgb(156 163 175/var(--tw-text-opacity))}.text-gray-500{--tw-text-opacity:1;color:rgb(107 114 128/var(--tw-text-opacity))}.text-gray-700{--tw-text-opacity:1;color:rgb(55 65 81/var(--tw-text-opacity))}.text-gray-900{--tw-text-opacity:1;color:rgb(17 24 39/var(--tw-text-opacity))}.text-green-500{--tw-text-opacity:1;color:rgb(34 197 94/var(--tw-text-opacity))}.text-green-600{--tw-text-opacity:1;color:rgb(22 163 74/var(--tw-text-opacity))}.text-orange-500{--tw-text-opacity:1;color:rgb(249 115 22/var(--tw-text-opacity))}.text-primary-500{--tw-text-opacity:1;color:rgb(var(--color-primary-500)/var(--tw-text-opacity))}.text-primary-600{--tw-text-opacity:1;color:rgb(var(--color-primary-600)/var(--tw-text-opacity))}.text-red-500{--tw-text-opacity:1;color:rgb(239 68 68/var(--tw-text-opacity))}.text-red-600{--tw-text-opacity:1;color:rgb(220 38 38/var(--tw-text-opacity))}.text-white{--tw-text-opacity:1;color:rgb(255 255 255/var(--tw-text-opacity))}.underline{-webkit-text-decoration-line:underline;text-decoration-line:underline}.antialiased{-webkit-font-smoothing:antialiased;-moz-osx-font-smoothing:grayscale}.opacity-0{opacity:0}.shadow{--tw-shadow:0 1px 3px 0 #0000001a,0 1px 2px -1px #0000001a;--tw-shadow-colored:0 1px 3px 0 var(--tw-shadow-color),0 1px 2px -1px var(--tw-shadow-color)}.shadow,.shadow-lg{box-shadow:var(--tw-ring-offset-shadow,0 0 #0000),var(--tw-ring-shadow,0 0 #0000),var(--tw-shadow)}.shadow-lg{--tw-shadow:0 10px 15px -3px #0000001a,0 4px 6px -4px #0000001a;--tw-shadow-colored:0 10px 15px -3px var(--tw-shadow-color),0 4px 6px -4px var(--tw-shadow-color)}.shadow-sm{--tw-shadow:0 1px 2px 0 #0000000d;--tw-shadow-colored:0 1px 2px 0 var(--tw-shadow-color);box-shadow:var(--tw-ring-offset-shadow,0 0 #0000),var(--tw-ring-shadow,0 0 #0000),var(--tw-shadow)}.blur{--tw-blur:blur(8px)}.blur,.filter{filter:var(--tw-blur) var(--tw-brightness) var(--tw-contrast) var(--tw-grayscale) var(--tw-hue-rotate) var(--tw-invert) var(--tw-saturate) var(--tw-sepia) var(--tw-drop-shadow)}.backdrop-blur-sm{--tw-backdrop-blur:blur(4px);-webkit-backdrop-filter:var(--tw-backdrop-blur) var(--tw-backdrop-brightness) var(--tw-backdrop-contrast) var(--tw-backdrop-grayscale) var(--tw-backdrop-hue-rotate) var(--tw-backdrop-invert) var(--tw-backdrop-opacity) var(--tw-backdrop-saturate) var(--tw-backdrop-sepia);backdrop-filter:var(--tw-backdrop-blur) var(--tw-backdrop-brightness) var(--tw-backdrop-contrast) var(--tw-backdrop-grayscale) var(--tw-backdrop-hue-rotate) var(--tw-backdrop-invert) var(--tw-backdrop-opacity) var(--tw-backdrop-saturate) var(--tw-backdrop-sepia)}.transition{transition-property:color,background-color,border-color,fill,stroke,opacity,box-shadow,transform,filter,-webkit-text-decoration-color,-webkit-backdrop-filter;transition-property:color,background-color,border-color,text-decoration-color,fill,stroke,opacity,box-shadow,transform,filter,backdrop-filter;transition-property:color,background-color,border-color,text-decoration-color,fill,stroke,opacity,box-shadow,transform,filter,backdrop-filter,-webkit-text-decoration-color,-webkit-backdrop-filter;transition-timing-function:cubic-bezier(.4,0,.2,1);transition-duration:.15s}.transition-all{transition-property:all;transition-timing-function:cubic-bezier(.4,0,.2,1);transition-duration:.15s}.transition-colors{transition-property:color,background-color,border-color,fill,stroke,-webkit-text-decoration-color;transition-property:color,background-color,border-color,text-decoration-color,fill,stroke;transition-property:color,background-color,border-color,text-decoration-color,fill,stroke,-webkit-text-decoration-color;transition-timing-function:cubic-bezier(.4,0,.2,1);transition-duration:.15s}.transition-height{transition-property:height;transition-timing-function:cubic-bezier(.4,0,.2,1);transition-duration:.15s}.transition-width{transition-property:width;transition-timing-function:cubic-bezier(.4,0,.2,1);transition-duration:.15s}.duration-75{transition-duration:75ms}.ease-in-out{transition-timing-function:cubic-bezier(.4,0,.2,1)}.border-spacing-none{border-spacing:0}.material-symbols-outlined{font-family:Material Symbols Outlined;font-weight:400;font-style:normal;font-size:18px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-moz-font-feature-settings:"liga";-moz-osx-font-smoothing:grayscale}.scrollable-top:after{position:absolute;left:0;right:0;top:-1rem;height:1rem;background-image:linear-gradient(to top,var(--tw-gradient-stops));--tw-gradient-from:#f3f4f6 var(--tw-gradient-from-position);--tw-gradient-from-position: ;--tw-gradient-to:#f3f4f600 var(--tw-gradient-from-position);--tw-gradient-to-position: ;--tw-gradient-stops:var(--tw-gradient-from),var(--tw-gradient-to)}:is(.dark .scrollable-top):after{background-image:none}.scrollable-top:after{content:""}.\[a-zA-Z\:\\-\]{a-z-a--z:\-}html{--color-primary-100:#f3e8ff;--color-primary-200:#e9d5ff;--color-primary-300:#d8b4fe;--color-primary-400:#c084fc;--color-primary-500:#a855f7;--color-primary-600:#9333ea;--color-primary-700:#7e22ce;--color-primary-800:#6b21a8;--color-primary-900:#581c87}.column-fill-auto{-moz-column-fill:auto;column-fill:auto}[x-cloak]{display:none!important}.asteriskField{--tw-text-opacity:1;color:rgb(220 38 38/var(--tw-text-opacity))}.md-16{font-size:16px}.md-18{font-size:18px}select:not([class*=bg-none]):not([multiple]){background-image:url("data:image/svg+xml;charset=utf-8,%3Csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 48 48'%3E%3Cpath fill='%236B7280' d='M24 31.4 11.3 18.7l2.85-2.8L24 25.8l9.85-9.85 2.85 2.8Z'/%3E%3C/svg%3E");background-position:right .7rem center;background-repeat:no-repeat;background-size:1.125rem 1.125rem}select:after{content:"";display:block}#page input[type=checkbox]{position:relative;display:block;height:1rem;width:1rem;cursor:pointer;-webkit-appearance:none;-moz-appearance:none;appearance:none;border-radius:.25rem;border-width:1px;border-color:rgb(209 213 219/var(--tw-border-opacity));background-color:rgb(255 255 255/var(--tw-bg-opacity))}#page input[type=checkbox],:is(.dark #page input[type=checkbox]){--tw-border-opacity:1;--tw-bg-opacity:1}:is(.dark #page input[type=checkbox]){border-color:rgb(107 114 128/var(--tw-border-opacity));background-color:rgb(55 65 81/var(--tw-bg-opacity))}#page input[type=checkbox]:hover{--tw-border-opacity:1;border-color:rgb(156 163 175/var(--tw-border-opacity))}#page input[type=checkbox]:after{position:absolute;margin-left:-1px;margin-top:-1px;display:flex;height:1rem;width:1rem;align-items:center;justify-content:center;font-size:.875rem;line-height:1.25rem;line-height:1;--tw-text-opacity:1;color:rgb(255 255 255/var(--tw-text-opacity));transition-property:all;transition-timing-function:cubic-bezier(.4,0,.2,1);transition-duration:.15s}:is(.dark #page input[type=checkbox]):after{--tw-text-opacity:1;color:rgb(55 65 81/var(--tw-text-opacity))}#page input[type=checkbox]:after{content:"done";font-family:Material Symbols Outlined}#page input[type=checkbox]:checked{--tw-border-opacity:1;border-color:rgb(var(--color-primary-600)/var(--tw-border-opacity));--tw-bg-opacity:1;background-color:rgb(var(--color-primary-600)/var(--tw-bg-opacity));transition-property:all;transition-timing-function:cubic-bezier(.4,0,.2,1);transition-duration:.15s}#page input[type=checkbox]:checked:after{--tw-text-opacity:1;color:rgb(255 255 255/var(--tw-text-opacity))}#page input[type=checkbox].hidden{display:none}table select{display:block;cursor:pointer;-webkit-appearance:none;-moz-appearance:none;appearance:none;border-radius:.375rem;border-width:1px;background-repeat:no-repeat;padding:.5rem 1.25rem .5rem .75rem;font-weight:500;--tw-text-opacity:1;color:rgb(107 114 128/var(--tw-text-opacity));--tw-shadow:0 1px 2px 0 #0000000d;--tw-shadow-colored:0 1px 2px 0 var(--tw-shadow-color);box-shadow:var(--tw-ring-offset-shadow,0 0 #0000),var(--tw-ring-shadow,0 0 #0000),var(--tw-shadow);background-image:url('data:image/svg+xml;utf8,<svg xmlns="http://www.w3.org/2000/svg" height="24px" viewBox="0 0 24 24" width="24px" fill="rgb(156, 163, 175)"><path d="M0 0h24v24H0V0z" fill="none"/><path d="M7 10l5 5 5-5H7z"/></svg>');background-size:1.125rem 1.125rem;background-position:right .5rem center}table select:focus{--tw-border-opacity:1;border-color:rgb(var(--color-primary-600)/var(--tw-border-opacity))}table tr.selected{--tw-bg-opacity:1;background-color:rgb(254 252 232/var(--tw-bg-opacity))}:is(.dark table tr.selected){background-color:#ffffff0f}.datetimeshortcuts{display:flex;flex-direction:row-reverse;align-items:center;font-size:0;line-height:1}.datetimeshortcuts a{font-size:0;line-height:1;--tw-text-opacity:1;color:rgb(156 163 175/var(--tw-text-opacity));transition-property:color,background-color,border-color,fill,stroke,opacity,box-shadow,transform,filter,-webkit-text-decoration-color,-webkit-backdrop-filter;transition-property:color,background-color,border-color,text-decoration-color,fill,stroke,opacity,box-shadow,transform,filter,backdrop-filter;transition-property:color,background-color,border-color,text-decoration-color,fill,stroke,opacity,box-shadow,transform,filter,backdrop-filter,-webkit-text-decoration-color,-webkit-backdrop-filter;transition-timing-function:cubic-bezier(.4,0,.2,1);transition-duration:.15s}.datetimeshortcuts a:hover{--tw-text-opacity:1;color:rgb(55 65 81/var(--tw-text-opacity))}.datetimeshortcuts a:first-child{margin-left:.5rem}.datetimeshortcuts a:first-child:hover{--tw-text-opacity:1;color:rgb(55 65 81/var(--tw-text-opacity))}:is(.dark .datetimeshortcuts a:first-child){--tw-text-opacity:1;color:rgb(107 114 128/var(--tw-text-opacity))}:is(.dark .datetimeshortcuts a:first-child:hover){--tw-text-opacity:1;color:rgb(229 231 235/var(--tw-text-opacity))}.datetimeshortcuts a:first-child:after{display:flex;height:2.375rem;width:2.375rem;align-items:center;justify-content:center;border-radius:.25rem;border-width:1px;--tw-bg-opacity:1;background-color:rgb(255 255 255/var(--tw-bg-opacity));padding-top:.5rem;padding-bottom:.5rem;text-align:center;font-size:1rem;line-height:1.5rem;--tw-shadow:0 1px 2px 0 #0000000d;--tw-shadow-colored:0 1px 2px 0 var(--tw-shadow-color);box-shadow:var(--tw-ring-offset-shadow,0 0 #0000),var(--tw-ring-shadow,0 0 #0000),var(--tw-shadow);font-family:Material Symbols Outlined;font-weight:400;font-style:normal;font-size:18px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-moz-font-feature-settings:"liga";-moz-osx-font-smoothing:grayscale}.datetimeshortcuts a:first-child:hover:after{--tw-text-opacity:1;color:rgb(55 65 81/var(--tw-text-opacity))}:is(.dark .datetimeshortcuts a:first-child):after{--tw-border-opacity:1;border-color:rgb(55 65 81/var(--tw-border-opacity));--tw-bg-opacity:1;background-color:rgb(17 24 39/var(--tw-bg-opacity))}:is(.dark .datetimeshortcuts a:first-child:hover):after{--tw-text-opacity:1;color:rgb(255 255 255/var(--tw-text-opacity))}.datetimeshortcuts a:first-child:after{content:"timer";display:flex}.date-icon{margin-left:.5rem;display:block;height:2.375rem;width:2.375rem;--tw-text-opacity:1;color:rgb(156 163 175/var(--tw-text-opacity));transition-property:all;transition-timing-function:cubic-bezier(.4,0,.2,1);transition-duration:.15s}.date-icon:hover{--tw-text-opacity:1;color:rgb(55 65 81/var(--tw-text-opacity))}:is(.dark .date-icon){--tw-text-opacity:1;color:rgb(107 114 128/var(--tw-text-opacity))}:is(.dark .date-icon:hover){--tw-text-opacity:1;color:rgb(255 255 255/var(--tw-text-opacity))}.date-icon:after{height:2.375rem;width:2.375rem;align-items:center;justify-content:center;border-radius:.25rem;border-width:1px;--tw-bg-opacity:1;background-color:rgb(255 255 255/var(--tw-bg-opacity));padding-top:.5rem;padding-bottom:.5rem;text-align:center;font-size:1rem;line-height:1.5rem;--tw-shadow:0 1px 2px 0 #0000000d;--tw-shadow-colored:0 1px 2px 0 var(--tw-shadow-color);box-shadow:var(--tw-ring-offset-shadow,0 0 #0000),var(--tw-ring-shadow,0 0 #0000),var(--tw-shadow);font-family:Material Symbols Outlined;font-weight:400;font-style:normal;font-size:18px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-moz-font-feature-settings:"liga";-moz-osx-font-smoothing:grayscale}.date-icon:hover:after{--tw-text-opacity:1;color:rgb(55 65 81/var(--tw-text-opacity))}:is(.dark .date-icon):after{--tw-border-opacity:1;border-color:rgb(55 65 81/var(--tw-border-opacity));--tw-bg-opacity:1;background-color:rgb(17 24 39/var(--tw-bg-opacity))}.date-icon:after{content:"edit";display:flex}:is(.dark .date-icon:hover):after{--tw-text-opacity:1;color:rgb(255 255 255/var(--tw-text-opacity))}.clock-icon{margin-left:.5rem;display:block;height:2.375rem;width:2.375rem}.clock-icon:hover{--tw-text-opacity:1;color:rgb(55 65 81/var(--tw-text-opacity))}:is(.dark .clock-icon){--tw-text-opacity:1;color:rgb(107 114 128/var(--tw-text-opacity))}:is(.dark .clock-icon:hover){--tw-text-opacity:1;color:rgb(229 231 235/var(--tw-text-opacity))}.clock-icon:after{height:2.375rem;width:2.375rem;align-items:center;justify-content:center;border-radius:.25rem;border-width:1px;--tw-bg-opacity:1;background-color:rgb(255 255 255/var(--tw-bg-opacity));padding-top:.5rem;padding-bottom:.5rem;text-align:center;font-size:1rem;line-height:1.5rem;--tw-shadow:0 1px 2px 0 #0000000d;--tw-shadow-colored:0 1px 2px 0 var(--tw-shadow-color);box-shadow:var(--tw-ring-offset-shadow,0 0 #0000),var(--tw-ring-shadow,0 0 #0000),var(--tw-shadow);font-family:Material Symbols Outlined;font-weight:400;font-style:normal;font-size:18px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-moz-font-feature-settings:"liga";-moz-osx-font-smoothing:grayscale}.clock-icon:hover:after{--tw-text-opacity:1;color:rgb(55 65 81/var(--tw-text-opacity))}:is(.dark .clock-icon):after{--tw-border-opacity:1;border-color:rgb(55 65 81/var(--tw-border-opacity));--tw-bg-opacity:1;background-color:rgb(17 24 39/var(--tw-bg-opacity))}:is(.dark .clock-icon:hover):after{--tw-text-opacity:1;color:rgb(255 255 255/var(--tw-text-opacity))}.clock-icon:after{content:"edit";display:flex}.timezonewarning{margin-top:.5rem;width:100%;font-size:.75rem;line-height:1rem;--tw-text-opacity:1;color:rgb(107 114 128/var(--tw-text-opacity))}.selector{display:flex;flex-direction:column;align-items:center}@media (min-width:768px){.selector{flex-direction:row}}.selector select{width:100%;flex-grow:1;background-image:none}:is(.dark .selector select){--tw-bg-opacity:1;background-color:rgb(17 24 39/var(--tw-bg-opacity))}.selector option{overflow:hidden;text-overflow:ellipsis;white-space:nowrap;padding-left:.75rem;padding-right:.75rem;font-size:.875rem;line-height:1.25rem;--tw-text-opacity:1;color:rgb(107 114 128/var(--tw-text-opacity))}:is(.dark .selector option){--tw-text-opacity:1;color:rgb(156 163 175/var(--tw-text-opacity))}.selector .list-footer-display{border-top-width:1px;padding-top:.5rem;padding-bottom:.5rem;text-align:center;font-size:.875rem;line-height:1.25rem}:is(.dark .selector .list-footer-display){--tw-border-opacity:1;border-color:rgb(55 65 81/var(--tw-border-opacity))}.selector-available,.selector-chosen{display:flex;flex-grow:1;flex-direction:column;align-self:stretch;border-radius:.375rem;border-width:1px;--tw-shadow:0 1px 2px 0 #0000000d;--tw-shadow-colored:0 1px 2px 0 var(--tw-shadow-color);box-shadow:var(--tw-ring-offset-shadow,0 0 #0000),var(--tw-ring-shadow,0 0 #0000),var(--tw-shadow)}:is(.dark .selector-available),:is(.dark .selector-chosen){--tw-border-opacity:1;border-color:rgb(55 65 81/var(--tw-border-opacity))}@media (min-width:768px){.selector-available,.selector-chosen{width:18rem}}@media (min-width:1024px){.selector-available,.selector-chosen{width:24rem}}.selector-available h2,.selector-chosen h2{margin-bottom:.75rem;border-bottom-width:1px;padding:.5rem .75rem;font-size:.875rem;line-height:1.25rem;--tw-text-opacity:1;color:rgb(107 114 128/var(--tw-text-opacity))}:is(.dark .selector-available h2),:is(.dark .selector-chosen h2){--tw-border-opacity:1;border-color:rgb(55 65 81/var(--tw-border-opacity));--tw-text-opacity:1;color:rgb(229 231 235/var(--tw-text-opacity))}.selector-filter{display:flex}.selector-filter input{margin-left:.75rem;margin-right:.75rem;margin-bottom:.75rem;display:block;flex-grow:1;border-radius:.375rem;--tw-bg-opacity:1;background-color:rgb(243 244 246/var(--tw-bg-opacity));padding:.5rem .75rem;font-size:.875rem;line-height:1.25rem;font-weight:500;--tw-text-opacity:1;color:rgb(107 114 128/var(--tw-text-opacity))}.selector-filter input:focus{outline:2px solid #0000;outline-offset:2px}:is(.dark .selector-filter input){--tw-bg-opacity:1;background-color:rgb(31 41 55/var(--tw-bg-opacity));--tw-text-opacity:1;color:rgb(156 163 175/var(--tw-text-opacity))}.selector-chooseall,.selector-clearall{display:block;border-top-width:1px;padding-top:.5rem;padding-bottom:.5rem;text-align:center;font-size:.875rem;line-height:1.25rem;--tw-text-opacity:1;color:rgb(var(--color-primary-500)/var(--tw-text-opacity));-webkit-text-decoration-line:underline;text-decoration-line:underline}:is(.dark .selector-chooseall),:is(.dark .selector-clearall){--tw-border-opacity:1;border-color:rgb(55 65 81/var(--tw-border-opacity))}.selector-clearall{--tw-text-opacity:1;color:rgb(220 38 38/var(--tw-text-opacity))}:is(.dark .selector-clearall){--tw-text-opacity:1;color:rgb(239 68 68/var(--tw-text-opacity))}.selector-chooser{margin-top:1rem;margin-bottom:1rem;display:flex;width:3.5rem;flex-direction:column;font-size:0;line-height:1}.selector-chooser li{padding-top:.25rem;padding-bottom:.25rem;text-align:center}.selector-add:after,.selector-remove:after{width:1.25rem;--tw-text-opacity:1;color:rgb(156 163 175/var(--tw-text-opacity));font-family:Material Symbols Outlined;font-weight:400;font-style:normal;font-size:18px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-moz-font-feature-settings:"liga";-moz-osx-font-smoothing:grayscale}.selector-add:after{content:"arrow_forward"}.selector-remove:after{content:"arrow_back"}#page input[type=checkbox].empty-form,.empty-form{display:none}.add-row{--tw-bg-opacity:1;background-color:rgb(249 250 251/var(--tw-bg-opacity));padding:1.25rem .75rem;text-align:left;text-align:right;vertical-align:middle;font-size:.875rem;line-height:1.25rem;font-weight:400}:is(.dark .add-row){--tw-bg-opacity:1;background-color:rgb(17 24 39/var(--tw-bg-opacity))}[data-inline-type=stacked] .add-row{overflow:hidden;border-top-width:1px;--tw-border-opacity:1;border-color:rgb(229 231 235/var(--tw-border-opacity))}:is(.dark [data-inline-type=stacked] .add-row){--tw-border-opacity:1;border-color:rgb(31 41 55/var(--tw-border-opacity))}.add-row td{padding:1rem .75rem}.add-row a{display:block;border-radius:.375rem;border-width:1px;--tw-bg-opacity:1;background-color:rgb(255 255 255/var(--tw-bg-opacity));padding:.5rem .75rem;text-align:center;font-size:.875rem;line-height:1.25rem;font-weight:500;--tw-text-opacity:1;color:rgb(107 114 128/var(--tw-text-opacity));transition-property:all;transition-timing-function:cubic-bezier(.4,0,.2,1);transition-duration:.15s}:is(.dark .add-row a){--tw-border-opacity:1;border-color:rgb(55 65 81/var(--tw-border-opacity));--tw-bg-opacity:1;background-color:rgb(17 24 39/var(--tw-bg-opacity));--tw-text-opacity:1;color:rgb(156 163 175/var(--tw-text-opacity))}:is(.dark .add-row a:hover){--tw-text-opacity:1;color:rgb(229 231 235/var(--tw-text-opacity))}@media (min-width:1024px){.add-row a{float:right}}h3 .delete label{--tw-text-opacity:1;color:rgb(107 114 128/var(--tw-text-opacity))}.inline-deletelink{display:block;font-size:.875rem;line-height:1.25rem;line-height:1;--tw-text-opacity:1;color:rgb(220 38 38/var(--tw-text-opacity));-webkit-text-decoration-line:underline;text-decoration-line:underline}:is(.dark .inline-deletelink){--tw-text-opacity:1;color:rgb(239 68 68/var(--tw-text-opacity))}td .inline-deletelink{display:block}@media (min-width:1024px){td .inline-deletelink{margin-top:.625rem}}h3 span:nth-child(3){margin-left:auto}.select2.select2-container{width:100%;max-width:42rem;border-radius:.375rem;border-width:1px;--tw-shadow:0 1px 2px 0 #0000000d;--tw-shadow-colored:0 1px 2px 0 var(--tw-shadow-color);box-shadow:var(--tw-ring-offset-shadow,0 0 #0000),var(--tw-ring-shadow,0 0 #0000),var(--tw-shadow)}:is(.dark .select2.select2-container){--tw-border-opacity:1;border-color:rgb(55 65 81/var(--tw-border-opacity))}.select2.select2-container{width:100%!important}.errors .select2.select2-container{--tw-border-opacity:1;border-color:rgb(220 38 38/var(--tw-border-opacity))}.select2-container.select2-container--admin-autocomplete .select2-selection--single{height:auto}.select2-container.select2-container--admin-autocomplete .select2-selection--single .select2-selection__rendered{height:2.25rem;padding:.5rem .75rem;font-size:.875rem;line-height:1.25rem;font-weight:500;--tw-text-opacity:1;color:rgb(107 114 128/var(--tw-text-opacity))}:is(.dark .select2-container.select2-container--admin-autocomplete .select2-selection--single .select2-selection__rendered){--tw-text-opacity:1;color:rgb(156 163 175/var(--tw-text-opacity))}.select2-container.select2-container--admin-autocomplete .select2-selection--single .select2-selection__clear{margin-right:1.25rem;margin-top:-.5rem;display:flex;height:2.25rem;align-items:center;font-size:0;line-height:1}.select2-container.select2-container--admin-autocomplete .select2-selection--single .select2-selection__clear:after{--tw-text-opacity:1;color:rgb(107 114 128/var(--tw-text-opacity));font-family:Material Symbols Outlined;font-weight:400;font-style:normal;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-moz-font-feature-settings:"liga";-moz-osx-font-smoothing:grayscale;content:"close";font-size:14px}.select2-container.select2-container--admin-autocomplete .select2-selection--single .select2-selection__arrow{margin-right:.5rem;margin-top:-1px;display:flex;height:2.25rem;align-items:center}.select2-container.select2-container--admin-autocomplete .select2-selection--single .select2-selection__arrow:after{left:0;margin:0;font-size:1.125rem;line-height:1.75rem;--tw-text-opacity:1;color:rgb(107 114 128/var(--tw-text-opacity));font-family:Material Symbols Outlined;font-weight:400;font-style:normal;font-size:18px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-moz-font-feature-settings:"liga";-moz-osx-font-smoothing:grayscale;content:"expand_more"}#page input[type=checkbox].select2-container.select2-container--admin-autocomplete .select2-selection--single .select2-selection__arrow b,.select2-container.select2-container--admin-autocomplete .select2-selection--single .select2-selection__arrow b{display:none}.select2-container.select2-container--admin-autocomplete .select2-search--dropdown{display:flex;padding:.5rem .75rem}.select2-container.select2-container--admin-autocomplete .select2-search--dropdown .select2-search__field{margin-left:0;margin-right:0;width:auto;flex-grow:1;border-radius:.375rem;border-width:1px;border-style:solid;--tw-border-opacity:1;border-color:rgb(229 231 235/var(--tw-border-opacity));--tw-bg-opacity:1;background-color:rgb(249 250 251/var(--tw-bg-opacity));padding:.5rem .75rem;font-size:.875rem;line-height:1.25rem;font-weight:500;--tw-text-opacity:1;color:rgb(107 114 128/var(--tw-text-opacity));--tw-shadow:0 1px 2px 0 #0000000d;--tw-shadow-colored:0 1px 2px 0 var(--tw-shadow-color);box-shadow:var(--tw-ring-offset-shadow,0 0 #0000),var(--tw-ring-shadow,0 0 #0000),var(--tw-shadow);outline:2px solid #0000;outline-offset:2px}:is(.dark .select2-container.select2-container--admin-autocomplete .select2-search--dropdown .select2-search__field){--tw-border-opacity:1;border-color:rgb(31 41 55/var(--tw-border-opacity));--tw-bg-opacity:1;background-color:rgb(31 41 55/var(--tw-bg-opacity));--tw-text-opacity:1;color:rgb(156 163 175/var(--tw-text-opacity))}.select2-container.select2-container--admin-autocomplete.select2-container--open.select2-container--above{border-top-left-radius:0;border-top-right-radius:0}.select2-container.select2-container--admin-autocomplete.select2-container--open.select2-container--below{border-bottom-right-radius:0;border-bottom-left-radius:0}.select2-container.select2-container--open .select2-dropdown{border-width:1px;--tw-border-opacity:1;border-color:rgb(229 231 235/var(--tw-border-opacity));padding-bottom:.5rem;--tw-shadow:0 1px 2px 0 #0000000d;--tw-shadow-colored:0 1px 2px 0 var(--tw-shadow-color);box-shadow:var(--tw-ring-offset-shadow,0 0 #0000),var(--tw-ring-shadow,0 0 #0000),var(--tw-shadow)}:is(.dark .select2-container.select2-container--open .select2-dropdown){--tw-border-opacity:1;border-color:rgb(55 65 81/var(--tw-border-opacity));--tw-bg-opacity:1;background-color:rgb(17 24 39/var(--tw-bg-opacity))}.select2-container.select2-container--open .select2-dropdown--below{border-top-left-radius:0;border-top-right-radius:0;border-bottom-right-radius:.375rem;border-bottom-left-radius:.375rem}.select2-container.select2-container--open .select2-dropdown--above{border-bottom-right-radius:0;border-bottom-left-radius:0;border-top-left-radius:.375rem;border-top-right-radius:.375rem}.select2-container.select2-container--admin-autocomplete .select2-results__option{display:block;padding:.5rem .75rem;font-size:.875rem;line-height:1.25rem;--tw-text-opacity:1;color:rgb(107 114 128/var(--tw-text-opacity));transition-property:all;transition-timing-function:cubic-bezier(.4,0,.2,1);transition-duration:.15s}:is(.dark .select2-container.select2-container--admin-autocomplete .select2-results__option){--tw-text-opacity:1;color:rgb(156 163 175/var(--tw-text-opacity))}.select2-container.select2-container--admin-autocomplete .select2-results__option--highlighted[aria-selected]{--tw-text-opacity:1;color:rgb(var(--color-primary-500)/var(--tw-text-opacity))}.select2-container--admin-autocomplete .select2-selection--multiple li.select2-selection__choice{display:flex;height:1.75rem;align-items:center;--tw-bg-opacity:1;background-color:rgb(243 244 246/var(--tw-bg-opacity));padding-left:.5rem;padding-right:.5rem;font-size:.875rem;line-height:1.25rem;font-weight:500;--tw-text-opacity:1;color:rgb(107 114 128/var(--tw-text-opacity));transition-property:all;transition-timing-function:cubic-bezier(.4,0,.2,1);transition-duration:.15s}:is(.dark .select2-container--admin-autocomplete .select2-selection--multiple li.select2-selection__choice){--tw-bg-opacity:1;background-color:rgb(31 41 55/var(--tw-bg-opacity));--tw-text-opacity:1;color:rgb(156 163 175/var(--tw-text-opacity))}:is(.dark .select2-container--admin-autocomplete .select2-selection--multiple li.select2-selection__choice:hover){--tw-text-opacity:1;color:rgb(229 231 235/var(--tw-text-opacity))}.select2-container--admin-autocomplete .select2-selection--multiple li.select2-selection__choice .select2-selection__choice__remove{font-size:0;line-height:1}.select2-container--admin-autocomplete .select2-selection--multiple li.select2-selection__choice .select2-selection__choice__remove:hover{--tw-text-opacity:1;color:rgb(75 85 99/var(--tw-text-opacity))}:is(.dark .select2-container--admin-autocomplete .select2-selection--multiple li.select2-selection__choice .select2-selection__choice__remove:hover){--tw-text-opacity:1;color:rgb(229 231 235/var(--tw-text-opacity))}.select2-container--admin-autocomplete .select2-selection--multiple li.select2-selection__choice .select2-selection__choice__remove:after{font-family:Material Symbols Outlined;font-weight:400;font-style:normal;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-moz-font-feature-settings:"liga";-moz-osx-font-smoothing:grayscale;content:"close";font-size:14px}.select2-container--admin-autocomplete .select2-selection--multiple li.select2-search--inline .select2-search__field{height:1.75rem;font-size:.875rem;line-height:1.25rem;--tw-text-opacity:1;color:rgb(107 114 128/var(--tw-text-opacity))}fieldset.collapsed>div{display:none}fieldset.collapse{visibility:visible}fieldset.collapsed,fieldset.collapsed h2{display:block}fieldset.collapsed .collapse-toggle{display:inline}.calendarbox{z-index:50;width:20rem;border-radius:.375rem;border-width:1px;--tw-bg-opacity:1;background-color:rgb(255 255 255/var(--tw-bg-opacity));font-size:.875rem;line-height:1.25rem;--tw-text-opacity:1;color:rgb(107 114 128/var(--tw-text-opacity));--tw-shadow:0 1px 2px 0 #0000000d;--tw-shadow-colored:0 1px 2px 0 var(--tw-shadow-color);box-shadow:var(--tw-ring-offset-shadow,0 0 #0000),var(--tw-ring-shadow,0 0 #0000),var(--tw-shadow)}:is(.dark .calendarbox){--tw-border-opacity:1;border-color:rgb(55 65 81/var(--tw-border-opacity));--tw-bg-opacity:1;background-color:rgb(31 41 55/var(--tw-bg-opacity))}.calendar caption{margin-bottom:.75rem;padding-top:.75rem;padding-bottom:.75rem;font-weight:500;--tw-text-opacity:1;color:rgb(55 65 81/var(--tw-text-opacity))}:is(.dark .calendar caption){--tw-text-opacity:1;color:rgb(229 231 235/var(--tw-text-opacity))}.calendar table{margin-bottom:.75rem;width:100%}.calendar table th{text-align:center;font-size:.75rem;line-height:1rem;font-weight:500;--tw-text-opacity:1;color:rgb(55 65 81/var(--tw-text-opacity))}:is(.dark .calendar table th){--tw-text-opacity:1;color:rgb(229 231 235/var(--tw-text-opacity))}.calendar table td{height:2.5rem;width:2.5rem;padding:.25rem;text-align:center}.calendar table td a{display:block;display:flex;height:2rem;width:2rem;align-items:center;justify-content:center;border-radius:9999px;transition-property:all;transition-timing-function:cubic-bezier(.4,0,.2,1);transition-duration:.15s}:is(.dark .calendar table td a){--tw-text-opacity:1;color:rgb(156 163 175/var(--tw-text-opacity))}.calendar table td a:hover{--tw-bg-opacity:1;background-color:rgb(243 244 246/var(--tw-bg-opacity));--tw-text-opacity:1;color:rgb(55 65 81/var(--tw-text-opacity))}.calendar table td.today a{--tw-bg-opacity:1;background-color:rgb(var(--color-primary-600)/var(--tw-bg-opacity));font-weight:500;--tw-text-opacity:1;color:rgb(255 255 255/var(--tw-text-opacity))}.calendar-shortcuts{margin-bottom:.75rem;display:flex;flex-direction:row;justify-content:center;border-bottom-right-radius:.375rem;border-bottom-left-radius:.375rem;padding-left:.25rem;padding-right:.25rem;font-size:0;line-height:1}.calendar-shortcuts a{margin-left:.25rem;margin-right:.25rem;width:33.333333%;border-radius:.375rem;border-width:1px;padding:.5rem;text-align:center;font-size:.75rem;line-height:1rem;font-weight:500;line-height:1;--tw-text-opacity:1;color:rgb(107 114 128/var(--tw-text-opacity));--tw-shadow:0 1px 2px 0 #0000000d;--tw-shadow-colored:0 1px 2px 0 var(--tw-shadow-color);box-shadow:var(--tw-ring-offset-shadow,0 0 #0000),var(--tw-ring-shadow,0 0 #0000),var(--tw-shadow);transition-property:all;transition-timing-function:cubic-bezier(.4,0,.2,1);transition-duration:.15s}:is(.dark .calendar-shortcuts a){--tw-border-opacity:1;border-color:rgb(55 65 81/var(--tw-border-opacity));--tw-text-opacity:1;color:rgb(156 163 175/var(--tw-text-opacity))}:is(.dark .calendar-shortcuts a:hover){--tw-border-opacity:1;border-color:rgb(75 85 99/var(--tw-border-opacity));--tw-text-opacity:1;color:rgb(229 231 235/var(--tw-text-opacity))}.calendar-cancel{display:block;border-top-width:1px;padding-top:.5rem;padding-bottom:.5rem;text-align:center;font-size:.75rem;line-height:1rem;--tw-text-opacity:1;color:rgb(220 38 38/var(--tw-text-opacity));-webkit-text-decoration-line:underline;text-decoration-line:underline}:is(.dark .calendar-cancel){--tw-border-opacity:1;border-color:rgb(55 65 81/var(--tw-border-opacity));--tw-text-opacity:1;color:rgb(239 68 68/var(--tw-text-opacity))}.calendarnav-previous{position:absolute;left:0;top:0;margin-left:.5rem;margin-top:.5rem;display:block;font-size:0;line-height:1}.calendarnav-next:after,.calendarnav-previous:after{display:flex;height:1.75rem;width:1.75rem;align-items:center;justify-content:center;border-radius:9999px;border-width:1px;--tw-text-opacity:1;color:rgb(156 163 175/var(--tw-text-opacity));transition-property:all;transition-timing-function:cubic-bezier(.4,0,.2,1);transition-duration:.15s;font-family:Material Symbols Outlined;font-weight:400;font-style:normal;font-size:18px;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-moz-font-feature-settings:"liga";-moz-osx-font-smoothing:grayscale}.calendarnav-next:hover:after,.calendarnav-previous:hover:after{--tw-border-opacity:1;border-color:rgb(var(--color-primary-600)/var(--tw-border-opacity));--tw-text-opacity:1;color:rgb(var(--color-primary-500)/var(--tw-text-opacity))}:is(.dark .calendarnav-next):after,:is(.dark .calendarnav-previous):after{--tw-border-opacity:1;border-color:rgb(55 65 81/var(--tw-border-opacity));--tw-bg-opacity:1;background-color:rgb(31 41 55/var(--tw-bg-opacity))}:is(.dark .calendarnav-next:hover):after,:is(.dark .calendarnav-previous:hover):after{border-color:rgb(31 41 55/var(--tw-border-opacity))}.calendarnav-next:after,.calendarnav-previous:after{content:"navigate_before";display:flex}:is(.dark .calendarnav-next:hover):after,:is(.dark .calendarnav-previous:hover):after{--tw-border-opacity:1;border-color:rgb(75 85 99/var(--tw-border-opacity));--tw-text-opacity:1;color:rgb(229 231 235/var(--tw-text-opacity))}.calendarnav-next{position:absolute;right:0;top:0;margin-right:.5rem;margin-top:.5rem;display:block;font-size:0;line-height:1}.calendarnav-next:after{content:"navigate_next";display:flex}.clockbox{z-index:50;border-radius:.375rem;border-width:1px;--tw-bg-opacity:1;background-color:rgb(255 255 255/var(--tw-bg-opacity));font-size:.875rem;line-height:1.25rem;--tw-shadow:0 1px 2px 0 #0000000d;--tw-shadow-colored:0 1px 2px 0 var(--tw-shadow-color);box-shadow:var(--tw-ring-offset-shadow,0 0 #0000),var(--tw-ring-shadow,0 0 #0000),var(--tw-shadow)}:is(.dark .clockbox){--tw-border-opacity:1;border-color:rgb(55 65 81/var(--tw-border-opacity));--tw-bg-opacity:1;background-color:rgb(31 41 55/var(--tw-bg-opacity))}.clockbox h2{padding:.5rem .75rem;font-weight:500;--tw-text-opacity:1;color:rgb(55 65 81/var(--tw-text-opacity))}:is(.dark .clockbox h2){--tw-text-opacity:1;color:rgb(229 231 235/var(--tw-text-opacity))}.clockbox .timelist{padding-left:.75rem;padding-right:.75rem;padding-bottom:.5rem;--tw-text-opacity:1;color:rgb(107 114 128/var(--tw-text-opacity))}:is(.dark .clockbox .timelist){--tw-text-opacity:1;color:rgb(156 163 175/var(--tw-text-opacity))}.clockbox .timelist li{display:block;padding-bottom:.25rem;transition-property:all;transition-timing-function:cubic-bezier(.4,0,.2,1);transition-duration:.15s}.clockbox .timelist li:hover{--tw-text-opacity:1;color:rgb(var(--color-primary-500)/var(--tw-text-opacity))}.field-actions_holder{width:0}.htmx-swapping:before{bottom:0;left:0;right:0;top:0;--tw-bg-opacity:1;background-color:rgb(255 255 255/var(--tw-bg-opacity));opacity:.8;transition-property:all;transition-timing-function:cubic-bezier(.4,0,.2,1);transition-duration:.15s;content:""}.htmx-swapping:after,.htmx-swapping:before{position:absolute}.htmx-swapping:after{inset:50%;height:1rem;width:1rem}@keyframes spin{to{transform:rotate(1turn)}}.htmx-swapping:after{-webkit-animation:spin 1s linear infinite;animation:spin 1s linear infinite;--tw-text-opacity:1;color:rgb(156 163 175/var(--tw-text-opacity));font-family:Material Symbols Outlined;font-weight:400;font-style:normal;line-height:1;letter-spacing:normal;text-transform:none;display:inline-block;white-space:nowrap;word-wrap:normal;direction:ltr;-moz-font-feature-settings:"liga";-moz-osx-font-smoothing:grayscale;font-size:16px;content:"sync"}#changelist-filter .admin-numeric-filter-slider .noUi-handle{right:-1rem;height:1rem;width:1rem;cursor:pointer;border-radius:9999px;border-width:1px;--tw-border-opacity:1;border-color:rgb(229 231 235/var(--tw-border-opacity));--tw-bg-opacity:1;background-color:rgb(255 255 255/var(--tw-bg-opacity));--tw-shadow:0 1px 2px 0 #0000000d;--tw-shadow-colored:0 1px 2px 0 var(--tw-shadow-color);box-shadow:var(--tw-ring-offset-shadow,0 0 #0000),var(--tw-ring-shadow,0 0 #0000),var(--tw-shadow)}:is(.dark #changelist-filter .admin-numeric-filter-slider .noUi-handle){--tw-border-opacity:1;border-color:rgb(229 231 235/var(--tw-border-opacity));--tw-bg-opacity:1;background-color:rgb(229 231 235/var(--tw-bg-opacity))}#changelist-filter .admin-numeric-filter-slider .noUi-handle-upper{right:0}#changelist-filter .admin-numeric-filter-slider .noUi-handle:after,#changelist-filter .admin-numeric-filter-slider .noUi-handle:before{content:none}#changelist-filter .admin-numeric-filter-slider.noUi-target{height:.25rem;border-width:0;--tw-bg-opacity:1;background-color:rgb(229 231 235/var(--tw-bg-opacity));--tw-shadow:0 0 #0000;--tw-shadow-colored:0 0 #0000;box-shadow:var(--tw-ring-offset-shadow,0 0 #0000),var(--tw-ring-shadow,0 0 #0000),var(--tw-shadow)}:is(.dark #changelist-filter .admin-numeric-filter-slider.noUi-target){--tw-bg-opacity:1;background-color:rgb(75 85 99/var(--tw-bg-opacity))}#changelist-filter .admin-numeric-filter-slider .noUi-connect{height:.25rem;border-width:0;--tw-bg-opacity:1;background-color:rgb(var(--color-primary-600)/var(--tw-bg-opacity))}#changelist-filter .admin-numeric-filter-slider-tooltips{margin-bottom:1.25rem;display:flex;flex-direction:row}#changelist-filter .admin-numeric-filter-slider-tooltips>:not([hidden])~:not([hidden]){--tw-space-x-reverse:0;margin-right:calc(1rem*var(--tw-space-x-reverse));margin-left:calc(1rem*(1 - var(--tw-space-x-reverse)))}#changelist-filter .admin-numeric-filter-slider-tooltips{font-size:.875rem;line-height:1.25rem;font-weight:500;--tw-text-opacity:1;color:rgb(107 114 128/var(--tw-text-opacity))}trix-toolbar[id^=trix-toolbar-]{position:sticky;top:0}:is(.dark trix-toolbar[id^=trix-toolbar-]){--tw-bg-opacity:1;background-color:rgb(17 24 39/var(--tw-bg-opacity))}.trix-active{--tw-text-opacity:1;color:rgb(var(--color-primary-600)/var(--tw-text-opacity))}.before\:mr-auto:before{content:var(--tw-content);margin-right:auto}.before\:block:before{content:var(--tw-content);display:block}.before\:w-72:before{content:var(--tw-content);width:18rem}.before\:capitalize:before{content:var(--tw-content);text-transform:capitalize}.before\:text-gray-500:before{content:var(--tw-content);--tw-text-opacity:1;color:rgb(107 114 128/var(--tw-text-opacity))}.before\:content-\[attr\(data-label\)\]:before{--tw-content:attr(data-label);content:var(--tw-content)}.first\:mt-0:first-child{margin-top:0}.last\:mb-0:last-child{margin-bottom:0}.last\:mb-8:last-child{margin-bottom:2rem}.last\:mr-0:last-child{margin-right:0}.last\:mb-4:last-child{margin-bottom:1rem}.last\:border-0:last-child{border-width:0}.last\:border-b-0:last-child{border-bottom-width:0}.focus-within\:border-primary-600:focus-within{--tw-border-opacity:1;border-color:rgb(var(--color-primary-600)/var(--tw-border-opacity))}.focus-within\:ring:focus-within{--tw-ring-offset-shadow:var(--tw-ring-inset) 0 0 0 var(--tw-ring-offset-width) var(--tw-ring-offset-color);--tw-ring-shadow:var(--tw-ring-inset) 0 0 0 calc(3px + var(--tw-ring-offset-width)) var(--tw-ring-color);box-shadow:var(--tw-ring-offset-shadow),var(--tw-ring-shadow),var(--tw-shadow,0 0 #0000)}.focus-within\:ring-primary-300:focus-within{--tw-ring-opacity:1;--tw-ring-color:rgb(var(--color-primary-300)/var(--tw-ring-opacity))}.hover\:bg-gray-100:hover{--tw-bg-opacity:1;background-color:rgb(243 244 246/var(--tw-bg-opacity))}.hover\:bg-gray-50:hover{--tw-bg-opacity:1;background-color:rgb(249 250 251/var(--tw-bg-opacity))}.hover\:bg-red-100:hover{--tw-bg-opacity:1;background-color:rgb(254 226 226/var(--tw-bg-opacity))}.hover\:\!text-primary-600:hover{--tw-text-opacity:1!important;color:rgb(var(--color-primary-600)/var(--tw-text-opacity))!important}.hover\:text-gray-700:hover{--tw-text-opacity:1;color:rgb(55 65 81/var(--tw-text-opacity))}.hover\:text-primary-600:hover{--tw-text-opacity:1;color:rgb(var(--color-primary-600)/var(--tw-text-opacity))}.hover\:text-red-700:hover{--tw-text-opacity:1;color:rgb(185 28 28/var(--tw-text-opacity))}.focus\:border-primary-600:focus{--tw-border-opacity:1;border-color:rgb(var(--color-primary-600)/var(--tw-border-opacity))}.focus\:outline-none:focus{outline:2px solid #0000;outline-offset:2px}.focus\:ring:focus{--tw-ring-offset-shadow:var(--tw-ring-inset) 0 0 0 var(--tw-ring-offset-width) var(--tw-ring-offset-color);--tw-ring-shadow:var(--tw-ring-inset) 0 0 0 calc(3px + var(--tw-ring-offset-width)) var(--tw-ring-color);box-shadow:var(--tw-ring-offset-shadow),var(--tw-ring-shadow),var(--tw-shadow,0 0 #0000)}.focus\:ring-primary-300:focus{--tw-ring-opacity:1;--tw-ring-color:rgb(var(--color-primary-300)/var(--tw-ring-opacity))}.group:hover .group-hover\:-right-1{right:-.25rem}.group:hover .group-hover\:text-gray-400{--tw-text-opacity:1;color:rgb(156 163 175/var(--tw-text-opacity))}.group:hover .group-hover\:text-gray-700{--tw-text-opacity:1;color:rgb(55 65 81/var(--tw-text-opacity))}.group:hover .group-hover\:text-primary-600{--tw-text-opacity:1;color:rgb(var(--color-primary-600)/var(--tw-text-opacity))}.group.inline-stacked .group-\[\.inline-stacked\]\:mx-3,.group.inline-tabular .group-\[\.inline-tabular\]\:mx-3{margin-left:.75rem;margin-right:.75rem}.group.inline-stacked .group-\[\.inline-stacked\]\:mb-3{margin-bottom:.75rem}.group.inline-stacked .group-\[\.inline-stacked\]\:mt-3{margin-top:.75rem}.group.inline-tabular .group-\[\.inline-tabular\]\:mb-0{margin-bottom:0}.group.inline-tabular .group-\[\.inline-tabular\]\:mt-3{margin-top:.75rem}.group.errors .group-\[\.errors\]\:border-red-600{--tw-border-opacity:1;border-color:rgb(220 38 38/var(--tw-border-opacity))}.group.errors .group-\[\.errors\]\:border-x-red-600{--tw-border-opacity:1;border-left-color:rgb(220 38 38/var(--tw-border-opacity));border-right-color:rgb(220 38 38/var(--tw-border-opacity))}.group.errors .group-\[\.errors\]\:border-t-red-600{--tw-border-opacity:1;border-top-color:rgb(220 38 38/var(--tw-border-opacity))}.group.errors .group-\[\.errors\]\:focus\:ring-red-200:focus{--tw-ring-opacity:1;--tw-ring-color:rgb(254 202 202/var(--tw-ring-opacity))}.peer:checked~.peer-checked\:block{display:block}.peer:checked~.peer-checked\:flex{display:flex}.prose-headings\:font-medium :is(:where(h1,h2,h3,h4,h5,h6,th):not(:where([class~=not-prose] *))){font-weight:500}.prose-headings\:text-gray-700 :is(:where(h1,h2,h3,h4,h5,h6,th):not(:where([class~=not-prose] *))){--tw-text-opacity:1;color:rgb(55 65 81/var(--tw-text-opacity))}.prose-a\:text-primary-600 :is(:where(a):not(:where([class~=not-prose] *))){--tw-text-opacity:1;color:rgb(var(--color-primary-600)/var(--tw-text-opacity))}.prose-a\:underline :is(:where(a):not(:where([class~=not-prose] *))){-webkit-text-decoration-line:underline;text-decoration-line:underline}.prose-blockquote\:not-italic :is(:where(blockquote):not(:where([class~=not-prose] *))){font-style:normal}.prose-strong\:text-gray-700 :is(:where(strong):not(:where([class~=not-prose] *))){--tw-text-opacity:1;color:rgb(55 65 81/var(--tw-text-opacity))}.prose-ol\:list-decimal :is(:where(ol):not(:where([class~=not-prose] *))){list-style-type:decimal}.prose-ul\:list-disc :is(:where(ul):not(:where([class~=not-prose] *))){list-style-type:disc}:is(.dark .dark\:border){border-width:1px}:is(.dark .dark\:border-r){border-right-width:1px}:is(.dark .dark\:border-amber-600\/10){border-color:#d977061a}:is(.dark .dark\:border-blue-500\/10){border-color:#3b82f61a}:is(.dark .dark\:border-gray-600){--tw-border-opacity:1;border-color:rgb(75 85 99/var(--tw-border-opacity))}:is(.dark .dark\:border-gray-700){--tw-border-opacity:1;border-color:rgb(55 65 81/var(--tw-border-opacity))}:is(.dark .dark\:border-gray-800){--tw-border-opacity:1;border-color:rgb(31 41 55/var(--tw-border-opacity))}:is(.dark .dark\:border-green-500\/10){border-color:#22c55e1a}:is(.dark .dark\:border-orange-500\/10){border-color:#f973161a}:is(.dark .dark\:border-red-500\/10){border-color:#ef44441a}:is(.dark .dark\:border-red-500\/20){border-color:#ef444433}:is(.dark .dark\:border-transparent){border-color:#0000}:is(.dark .dark\:bg-amber-600\/20){background-color:#d9770633}:is(.dark .dark\:bg-blue-500\/20){background-color:#3b82f633}:is(.dark .dark\:bg-gray-700){--tw-bg-opacity:1;background-color:rgb(55 65 81/var(--tw-bg-opacity))}:is(.dark .dark\:bg-gray-800){--tw-bg-opacity:1;background-color:rgb(31 41 55/var(--tw-bg-opacity))}:is(.dark .dark\:bg-gray-900){--tw-bg-opacity:1;background-color:rgb(17 24 39/var(--tw-bg-opacity))}:is(.dark .dark\:bg-green-500\/20){background-color:#22c55e33}:is(.dark .dark\:bg-orange-500\/20){background-color:#f9731633}:is(.dark .dark\:bg-red-500\/20){background-color:#ef444433}:is(.dark .dark\:bg-white\/\[\.02\]){background-color:#ffffff05}:is(.dark .dark\:bg-white\/\[\.04\]){background-color:#ffffff0a}:is(.dark .dark\:text-gray-200){--tw-text-opacity:1;color:rgb(229 231 235/var(--tw-text-opacity))}:is(.dark .dark\:text-gray-300){--tw-text-opacity:1;color:rgb(209 213 219/var(--tw-text-opacity))}:is(.dark .dark\:text-gray-400){--tw-text-opacity:1;color:rgb(156 163 175/var(--tw-text-opacity))}:is(.dark .dark\:text-gray-500){--tw-text-opacity:1;color:rgb(107 114 128/var(--tw-text-opacity))}:is(.dark .dark\:text-gray-600){--tw-text-opacity:1;color:rgb(75 85 99/var(--tw-text-opacity))}:is(.dark .dark\:text-primary-500){--tw-text-opacity:1;color:rgb(var(--color-primary-500)/var(--tw-text-opacity))}:is(.dark .dark\:text-red-500){--tw-text-opacity:1;color:rgb(239 68 68/var(--tw-text-opacity))}:is(.dark .dark\:before\:text-gray-400):before{content:var(--tw-content);--tw-text-opacity:1;color:rgb(156 163 175/var(--tw-text-opacity))}:is(.dark .dark\:focus-within\:ring-primary-600\/30:focus-within),:is(.dark .focus-within\:dark\:ring-primary-600\/30):focus-within{--tw-ring-color:rgb(var(--color-primary-600)/0.3)}:is(.dark .dark\:hover\:bg-gray-700:hover){--tw-bg-opacity:1;background-color:rgb(55 65 81/var(--tw-bg-opacity))}:is(.dark .dark\:hover\:bg-gray-900:hover){--tw-bg-opacity:1;background-color:rgb(17 24 39/var(--tw-bg-opacity))}:is(.dark .dark\:hover\:bg-red-500\/20:hover){background-color:#ef444433}:is(.dark .dark\:hover\:text-gray-200:hover){--tw-text-opacity:1;color:rgb(229 231 235/var(--tw-text-opacity))}:is(.dark .dark\:hover\:text-red-500:hover){--tw-text-opacity:1;color:rgb(239 68 68/var(--tw-text-opacity))}:is(.dark .hover\:dark\:text-gray-200):hover{--tw-text-opacity:1;color:rgb(229 231 235/var(--tw-text-opacity))}:is(.dark .dark\:focus\:ring-primary-600\/30:focus){--tw-ring-color:rgb(var(--color-primary-600)/0.3)}:is(.dark .group:hover .dark\:group-hover\:text-gray-200){--tw-text-opacity:1;color:rgb(229 231 235/var(--tw-text-opacity))}:is(.dark .group.errors .dark\:group-\[\.errors\]\:border-red-500){--tw-border-opacity:1;border-color:rgb(239 68 68/var(--tw-border-opacity))}:is(.dark .group.errors .dark\:group-\[\.errors\]\:border-x-red-500){--tw-border-opacity:1;border-left-color:rgb(239 68 68/var(--tw-border-opacity));border-right-color:rgb(239 68 68/var(--tw-border-opacity))}:is(.dark .group.errors .dark\:group-\[\.errors\]\:border-t-red-500){--tw-border-opacity:1;border-top-color:rgb(239 68 68/var(--tw-border-opacity))}:is(.dark .group.errors .dark\:group-\[\.errors\]\:focus\:ring-red-600\/40:focus){--tw-ring-color:#dc262666}:is(.dark .dark\:prose-headings\:text-gray-200 :is(:where(h1,h2,h3,h4,h5,h6,th):not(:where([class~=not-prose] *)))){--tw-text-opacity:1;color:rgb(229 231 235/var(--tw-text-opacity))}:is(.dark .dark\:prose-blockquote\:border-gray-700 :is(:where(blockquote):not(:where([class~=not-prose] *)))){--tw-border-opacity:1;border-color:rgb(55 65 81/var(--tw-border-opacity))}:is(.dark .dark\:prose-blockquote\:text-gray-200 :is(:where(blockquote):not(:where([class~=not-prose] *)))){--tw-text-opacity:1;color:rgb(229 231 235/var(--tw-text-opacity))}:is(.dark .dark\:prose-strong\:text-gray-200 :is(:where(strong):not(:where([class~=not-prose] *)))){--tw-text-opacity:1;color:rgb(229 231 235/var(--tw-text-opacity))}@media not all and (min-width:1280px){.max-xl\:fixed{position:fixed}}@media not all and (min-width:768px){.max-md\:w-full{width:100%}}@media (min-width:640px){.sm\:w-96{width:24rem}}@media (min-width:768px){.md\:mb-0{margin-bottom:0}.md\:mb-2{margin-bottom:.5rem}.md\:ml-auto{margin-left:auto}.md\:mr-4{margin-right:1rem}.md\:mr-8{margin-right:2rem}.md\:mt-0{margin-top:0}.md\:block{display:block}.md\:flex-row{flex-direction:row}.md\:items-center{align-items:center}.md\:justify-end{justify-content:flex-end}.md\:border-b{border-bottom-width:1px}.md\:border-b-0{border-bottom-width:0}.md\:border-l-0{border-left-width:0}.md\:border-r-0{border-right-width:0}.md\:border-t-0{border-top-width:0}.md\:border-primary-600{--tw-border-opacity:1;border-color:rgb(var(--color-primary-600)/var(--tw-border-opacity))}.md\:border-primary-500{--tw-border-opacity:1;border-color:rgb(var(--color-primary-500)/var(--tw-border-opacity))}.md\:px-0{padding-left:0;padding-right:0}.md\:py-4{padding-top:1rem;padding-bottom:1rem}:is(.dark .dark\:md\:border-gray-800){--tw-border-opacity:1;border-color:rgb(31 41 55/var(--tw-border-opacity))}:is(.dark .dark\:md\:border-primary-600){--tw-border-opacity:1;border-color:rgb(var(--color-primary-600)/var(--tw-border-opacity))}}@media (min-width:1024px){.lg\:-mx-4{margin-left:-1rem;margin-right:-1rem}.lg\:mb-0{margin-bottom:0}.lg\:mb-12{margin-bottom:3rem}.lg\:ml-auto{margin-left:auto}.lg\:mr-3{margin-right:.75rem}.lg\:mt-0{margin-top:0}.lg\:mt-3{margin-top:.75rem}.lg\:mt-8{margin-top:2rem}.lg\:block{display:block}.lg\:table-cell{display:table-cell}.lg\:table-header-group{display:table-header-group}.lg\:table-row{display:table-row}.lg\:w-60{width:15rem}.lg\:w-72{width:18rem}.lg\:w-auto{width:auto}.lg\:w-px{width:1px}.lg\:max-w-xs{max-width:20rem}.lg\:flex-row{flex-direction:row}.lg\:flex-row-reverse{flex-direction:row-reverse}.lg\:rounded-md{border-radius:.375rem}.lg\:border{border-width:1px}.lg\:border-0{border-width:0}.lg\:border-b-0{border-bottom-width:0}.lg\:border-t{border-top-width:1px}.lg\:border-none{border-style:none}.lg\:border-gray-200{--tw-border-opacity:1;border-color:rgb(229 231 235/var(--tw-border-opacity))}.lg\:p-12{padding:3rem}.lg\:px-12{padding-left:3rem;padding-right:3rem}.lg\:py-3{padding-top:.75rem;padding-bottom:.75rem}.lg\:align-top{vertical-align:top}.lg\:underline{-webkit-text-decoration-line:underline;text-decoration-line:underline}.lg\:shadow-none{--tw-shadow:0 0 #0000;--tw-shadow-colored:0 0 #0000}.lg\:shadow-none,.lg\:shadow-sm{box-shadow:var(--tw-ring-offset-shadow,0 0 #0000),var(--tw-ring-shadow,0 0 #0000),var(--tw-shadow)}.lg\:shadow-sm{--tw-shadow:0 1px 2px 0 #0000000d;--tw-shadow-colored:0 1px 2px 0 var(--tw-shadow-color)}.lg\:before\:hidden:before{content:var(--tw-content);display:none}:is(.dark .dark\:lg\:border-gray-800),:is(.dark .lg\:dark\:border-gray-800){--tw-border-opacity:1;border-color:rgb(31 41 55/var(--tw-border-opacity))}}@media (min-width:1280px){.xl\:left-0{left:0}.xl\:left-72{left:18rem}.xl\:block{display:block}.xl\:flex{display:flex}.xl\:hidden{display:none}.xl\:max-w-4xl{max-width:56rem}.xl\:text-base{font-size:1rem;line-height:1.5rem}}
```

### Comparing `django_unfold-0.5.3/src/unfold/static/unfold/js/alpine.js` & `django_unfold-0.6.0/src/unfold/static/unfold/js/alpine.js`

 * *Files 4% similar despite different names*

#### js-beautify {}

```diff
@@ -1,138 +1,139 @@
 (() => {
-    var We = !1,
-        Ge = !1,
-        B = [];
+    var Ye = !1,
+        Ze = !1,
+        V = [],
+        Qe = -1;
 
-    function $t(e) {
-        an(e)
+    function Bt(e) {
+        hn(e)
     }
 
-    function an(e) {
-        B.includes(e) || B.push(e), cn()
+    function hn(e) {
+        V.includes(e) || V.push(e), _n()
     }
 
-    function he(e) {
-        let t = B.indexOf(e);
-        t !== -1 && B.splice(t, 1)
+    function ye(e) {
+        let t = V.indexOf(e);
+        t !== -1 && t > Qe && V.splice(t, 1)
     }
 
-    function cn() {
-        !Ge && !We && (We = !0, queueMicrotask(ln))
+    function _n() {
+        !Ze && !Ye && (Ye = !0, queueMicrotask(gn))
     }
 
-    function ln() {
-        We = !1, Ge = !0;
-        for (let e = 0; e < B.length; e++) B[e]();
-        B.length = 0, Ge = !1
+    function gn() {
+        Ye = !1, Ze = !0;
+        for (let e = 0; e < V.length; e++) V[e](), Qe = e;
+        V.length = 0, Qe = -1, Ze = !1
     }
-    var A, K, Y, Ye, Je = !0;
+    var C, P, L, et, Xe = !0;
 
-    function Lt(e) {
-        Je = !1, e(), Je = !0
+    function Kt(e) {
+        Xe = !1, e(), Xe = !0
     }
 
-    function jt(e) {
-        A = e.reactive, Y = e.release, K = t => e.effect(t, {
+    function zt(e) {
+        C = e.reactive, L = e.release, P = t => e.effect(t, {
             scheduler: r => {
-                Je ? $t(r) : r()
+                Xe ? Bt(r) : r()
             }
-        }), Ye = e.raw
+        }), et = e.raw
     }
 
-    function Ze(e) {
-        K = e
+    function tt(e) {
+        P = e
     }
 
-    function Ft(e) {
+    function Vt(e) {
         let t = () => {};
         return [n => {
-            let i = K(n);
+            let i = P(n);
             return e._x_effects || (e._x_effects = new Set, e._x_runEffects = () => {
                 e._x_effects.forEach(o => o())
             }), e._x_effects.add(i), t = () => {
-                i !== void 0 && (e._x_effects.delete(i), Y(i))
+                i !== void 0 && (e._x_effects.delete(i), L(i))
             }, i
         }, () => {
             t()
         }]
     }
-    var Bt = [],
-        Kt = [],
-        zt = [];
+    var Ht = [],
+        qt = [],
+        Ut = [];
 
-    function Vt(e) {
-        zt.push(e)
+    function Wt(e) {
+        Ut.push(e)
     }
 
-    function _e(e, t) {
-        typeof t == "function" ? (e._x_cleanups || (e._x_cleanups = []), e._x_cleanups.push(t)) : (t = e, Kt.push(t))
+    function we(e, t) {
+        typeof t == "function" ? (e._x_cleanups || (e._x_cleanups = []), e._x_cleanups.push(t)) : (t = e, qt.push(t))
     }
 
-    function Ht(e) {
-        Bt.push(e)
+    function Gt(e) {
+        Ht.push(e)
     }
 
-    function qt(e, t, r) {
+    function Jt(e, t, r) {
         e._x_attributeCleanups || (e._x_attributeCleanups = {}), e._x_attributeCleanups[t] || (e._x_attributeCleanups[t] = []), e._x_attributeCleanups[t].push(r)
     }
 
-    function Qe(e, t) {
-        !e._x_attributeCleanups || Object.entries(e._x_attributeCleanups).forEach(([r, n]) => {
+    function nt(e, t) {
+        e._x_attributeCleanups && Object.entries(e._x_attributeCleanups).forEach(([r, n]) => {
             (t === void 0 || t.includes(r)) && (n.forEach(i => i()), delete e._x_attributeCleanups[r])
         })
     }
-    var et = new MutationObserver(Xe),
-        tt = !1;
+    var it = new MutationObserver(ct),
+        ot = !1;
 
-    function rt() {
-        et.observe(document, {
+    function se() {
+        it.observe(document, {
             subtree: !0,
             childList: !0,
             attributes: !0,
             attributeOldValue: !0
-        }), tt = !0
+        }), ot = !0
     }
 
-    function fn() {
-        un(), et.disconnect(), tt = !1
+    function st() {
+        xn(), it.disconnect(), ot = !1
     }
-    var te = [],
-        nt = !1;
+    var oe = [],
+        rt = !1;
 
-    function un() {
-        te = te.concat(et.takeRecords()), te.length && !nt && (nt = !0, queueMicrotask(() => {
-            dn(), nt = !1
+    function xn() {
+        oe = oe.concat(it.takeRecords()), oe.length && !rt && (rt = !0, queueMicrotask(() => {
+            yn(), rt = !1
         }))
     }
 
-    function dn() {
-        Xe(te), te.length = 0
+    function yn() {
+        ct(oe), oe.length = 0
     }
 
-    function m(e) {
-        if (!tt) return e();
-        fn();
+    function h(e) {
+        if (!ot) return e();
+        st();
         let t = e();
-        return rt(), t
+        return se(), t
     }
-    var it = !1,
-        ge = [];
+    var at = !1,
+        be = [];
 
-    function Ut() {
-        it = !0
+    function Yt() {
+        at = !0
     }
 
-    function Wt() {
-        it = !1, Xe(ge), ge = []
+    function Zt() {
+        at = !1, ct(be), be = []
     }
 
-    function Xe(e) {
-        if (it) {
-            ge = ge.concat(e);
+    function ct(e) {
+        if (at) {
+            be = be.concat(e);
             return
         }
         let t = [],
             r = [],
             n = new Map,
             i = new Map;
         for (let o = 0; o < e.length; o++)
@@ -147,52 +148,52 @@
                         })
                     },
                     u = () => {
                         i.has(s) || i.set(s, []), i.get(s).push(a)
                     };
                 s.hasAttribute(a) && c === null ? l() : s.hasAttribute(a) ? (u(), l()) : u()
             } i.forEach((o, s) => {
-            Qe(s, o)
+            nt(s, o)
         }), n.forEach((o, s) => {
-            Bt.forEach(a => a(s, o))
+            Ht.forEach(a => a(s, o))
         });
         for (let o of r)
-            if (!t.includes(o) && (Kt.forEach(s => s(o)), o._x_cleanups))
+            if (!t.includes(o) && (qt.forEach(s => s(o)), o._x_cleanups))
                 for (; o._x_cleanups.length;) o._x_cleanups.pop()();
         t.forEach(o => {
             o._x_ignoreSelf = !0, o._x_ignore = !0
         });
-        for (let o of t) r.includes(o) || !o.isConnected || (delete o._x_ignoreSelf, delete o._x_ignore, zt.forEach(s => s(o)), o._x_ignore = !0, o._x_ignoreSelf = !0);
+        for (let o of t) r.includes(o) || o.isConnected && (delete o._x_ignoreSelf, delete o._x_ignore, Ut.forEach(s => s(o)), o._x_ignore = !0, o._x_ignoreSelf = !0);
         t.forEach(o => {
             delete o._x_ignoreSelf, delete o._x_ignore
         }), t = null, r = null, n = null, i = null
     }
 
-    function xe(e) {
-        return D(k(e))
+    function Ee(e) {
+        return j($(e))
     }
 
-    function C(e, t, r) {
-        return e._x_dataStack = [t, ...k(r || e)], () => {
+    function R(e, t, r) {
+        return e._x_dataStack = [t, ...$(r || e)], () => {
             e._x_dataStack = e._x_dataStack.filter(n => n !== t)
         }
     }
 
-    function ot(e, t) {
+    function lt(e, t) {
         let r = e._x_dataStack[0];
         Object.entries(t).forEach(([n, i]) => {
             r[n] = i
         })
     }
 
-    function k(e) {
-        return e._x_dataStack ? e._x_dataStack : typeof ShadowRoot == "function" && e instanceof ShadowRoot ? k(e.host) : e.parentNode ? k(e.parentNode) : []
+    function $(e) {
+        return e._x_dataStack ? e._x_dataStack : typeof ShadowRoot == "function" && e instanceof ShadowRoot ? $(e.host) : e.parentNode ? $(e.parentNode) : []
     }
 
-    function D(e) {
+    function j(e) {
         let t = new Proxy({}, {
             ownKeys: () => Array.from(new Set(e.flatMap(r => Object.keys(r)))),
             has: (r, n) => e.some(i => i.hasOwnProperty(n)),
             get: (r, n) => (e.find(i => {
                 if (i.hasOwnProperty(n)) {
                     let o = Object.getOwnPropertyDescriptor(i, n);
                     if (o.get && o.get._x_alreadyBound || o.set && o.set._x_alreadyBound) return !0;
@@ -214,496 +215,509 @@
                 let o = e.find(s => s.hasOwnProperty(n));
                 return o ? o[n] = i : e[e.length - 1][n] = i, !0
             }
         });
         return t
     }
 
-    function ye(e) {
+    function ve(e) {
         let t = n => typeof n == "object" && !Array.isArray(n) && n !== null,
             r = (n, i = "") => {
                 Object.entries(Object.getOwnPropertyDescriptors(n)).forEach(([o, {
                     value: s,
                     enumerable: a
                 }]) => {
                     if (a === !1 || s === void 0) return;
                     let c = i === "" ? o : `${i}.${o}`;
                     typeof s == "object" && s !== null && s._x_interceptor ? n[o] = s.initialize(e, c, o) : t(s) && s !== n && !(s instanceof Element) && r(s, c)
                 })
             };
         return r(e)
     }
 
-    function be(e, t = () => {}) {
+    function Se(e, t = () => {}) {
         let r = {
             initialValue: void 0,
             _x_interceptor: !0,
             initialize(n, i, o) {
-                return e(this.initialValue, () => pn(n, i), s => st(n, i, s), i, o)
+                return e(this.initialValue, () => bn(n, i), s => ut(n, i, s), i, o)
             }
         };
         return t(r), n => {
             if (typeof n == "object" && n !== null && n._x_interceptor) {
                 let i = r.initialize.bind(r);
                 r.initialize = (o, s, a) => {
                     let c = n.initialize(o, s, a);
                     return r.initialValue = c, i(o, s, a)
                 }
             } else r.initialValue = n;
             return r
         }
     }
 
-    function pn(e, t) {
+    function bn(e, t) {
         return t.split(".").reduce((r, n) => r[n], e)
     }
 
-    function st(e, t, r) {
+    function ut(e, t, r) {
         if (typeof t == "string" && (t = t.split(".")), t.length === 1) e[t[0]] = r;
         else {
             if (t.length === 0) throw error;
-            return e[t[0]] || (e[t[0]] = {}), st(e[t[0]], t.slice(1), r)
+            return e[t[0]] || (e[t[0]] = {}), ut(e[t[0]], t.slice(1), r)
         }
     }
-    var Gt = {};
+    var Qt = {};
 
-    function x(e, t) {
-        Gt[e] = t
+    function y(e, t) {
+        Qt[e] = t
     }
 
-    function re(e, t) {
-        return Object.entries(Gt).forEach(([r, n]) => {
+    function ae(e, t) {
+        return Object.entries(Qt).forEach(([r, n]) => {
             Object.defineProperty(e, `$${r}`, {
                 get() {
-                    let [i, o] = at(t);
+                    let [i, o] = ft(t);
                     return i = {
-                        interceptor: be,
+                        interceptor: Se,
                         ...i
-                    }, _e(t, o), n(t, i)
+                    }, we(t, o), n(t, i)
                 },
                 enumerable: !1
             })
         }), e
     }
 
-    function Yt(e, t, r, ...n) {
+    function Xt(e, t, r, ...n) {
         try {
             return r(...n)
         } catch (i) {
-            J(i, e, t)
+            Z(i, e, t)
         }
     }
 
-    function J(e, t, r = void 0) {
+    function Z(e, t, r = void 0) {
         Object.assign(e, {
             el: t,
             expression: r
         }), console.warn(`Alpine Expression Error: ${e.message}
 
 ${r?'Expression: "'+r+`"
 
 `:""}`, t), setTimeout(() => {
             throw e
         }, 0)
     }
-    var ve = !0;
+    var Ae = !0;
 
-    function Jt(e) {
-        let t = ve;
-        ve = !1, e(), ve = t
+    function er(e) {
+        let t = Ae;
+        Ae = !1, e(), Ae = t
     }
 
-    function P(e, t, r = {}) {
+    function I(e, t, r = {}) {
         let n;
-        return g(e, t)(i => n = i, r), n
+        return x(e, t)(i => n = i, r), n
     }
 
-    function g(...e) {
-        return Zt(...e)
+    function x(...e) {
+        return tr(...e)
     }
-    var Zt = ct;
+    var tr = pt;
 
-    function Qt(e) {
-        Zt = e
+    function rr(e) {
+        tr = e
     }
 
-    function ct(e, t) {
+    function pt(e, t) {
         let r = {};
-        re(r, e);
-        let n = [r, ...k(e)];
-        if (typeof t == "function") return mn(n, t);
-        let i = hn(n, t, e);
-        return Yt.bind(null, e, t, i)
+        ae(r, e);
+        let n = [r, ...$(e)],
+            i = typeof t == "function" ? wn(n, t) : vn(n, t, e);
+        return Xt.bind(null, e, t, i)
     }
 
-    function mn(e, t) {
+    function wn(e, t) {
         return (r = () => {}, {
             scope: n = {},
             params: i = []
         } = {}) => {
-            let o = t.apply(D([n, ...e]), i);
-            we(r, o)
+            let o = t.apply(j([n, ...e]), i);
+            Oe(r, o)
         }
     }
-    var lt = {};
+    var dt = {};
 
-    function _n(e, t) {
-        if (lt[e]) return lt[e];
+    function En(e, t) {
+        if (dt[e]) return dt[e];
         let r = Object.getPrototypeOf(async function() {}).constructor,
-            n = /^[\n\s]*if.*\(.*\)/.test(e) || /^(let|const)\s/.test(e) ? `(() => { ${e} })()` : e,
+            n = /^[\n\s]*if.*\(.*\)/.test(e) || /^(let|const)\s/.test(e) ? `(async()=>{ ${e} })()` : e,
             o = (() => {
                 try {
                     return new r(["__self", "scope"], `with (scope) { __self.result = ${n} }; __self.finished = true; return __self.result;`)
                 } catch (s) {
-                    return J(s, t, e), Promise.resolve()
+                    return Z(s, t, e), Promise.resolve()
                 }
             })();
-        return lt[e] = o, o
+        return dt[e] = o, o
     }
 
-    function hn(e, t, r) {
-        let n = _n(t, r);
+    function vn(e, t, r) {
+        let n = En(t, r);
         return (i = () => {}, {
             scope: o = {},
             params: s = []
         } = {}) => {
             n.result = void 0, n.finished = !1;
-            let a = D([o, ...e]);
+            let a = j([o, ...e]);
             if (typeof n == "function") {
-                let c = n(n, a).catch(l => J(l, r, t));
-                n.finished ? (we(i, n.result, a, s, r), n.result = void 0) : c.then(l => {
-                    we(i, l, a, s, r)
-                }).catch(l => J(l, r, t)).finally(() => n.result = void 0)
+                let c = n(n, a).catch(l => Z(l, r, t));
+                n.finished ? (Oe(i, n.result, a, s, r), n.result = void 0) : c.then(l => {
+                    Oe(i, l, a, s, r)
+                }).catch(l => Z(l, r, t)).finally(() => n.result = void 0)
             }
         }
     }
 
-    function we(e, t, r, n, i) {
-        if (ve && typeof t == "function") {
+    function Oe(e, t, r, n, i) {
+        if (Ae && typeof t == "function") {
             let o = t.apply(r, n);
-            o instanceof Promise ? o.then(s => we(e, s, r, n)).catch(s => J(s, i, t)) : e(o)
-        } else e(t)
+            o instanceof Promise ? o.then(s => Oe(e, s, r, n)).catch(s => Z(s, i, t)) : e(o)
+        } else typeof t == "object" && t instanceof Promise ? t.then(o => e(o)) : e(t)
     }
-    var ut = "x-";
+    var gt = "x-";
 
-    function E(e = "") {
-        return ut + e
+    function S(e = "") {
+        return gt + e
     }
 
-    function Xt(e) {
-        ut = e
+    function nr(e) {
+        gt = e
     }
-    var er = {};
+    var mt = {};
 
-    function d(e, t) {
-        er[e] = t
+    function p(e, t) {
+        return mt[e] = t, {
+            before(r) {
+                if (!mt[r]) {
+                    console.warn("Cannot find directive `${directive}`. `${name}` will use the default order of execution");
+                    return
+                }
+                let n = H.indexOf(r);
+                H.splice(n >= 0 ? n : H.indexOf("DEFAULT"), 0, e)
+            }
+        }
     }
 
-    function ne(e, t, r) {
+    function le(e, t, r) {
         if (t = Array.from(t), e._x_virtualDirectives) {
             let o = Object.entries(e._x_virtualDirectives).map(([a, c]) => ({
                     name: a,
                     value: c
                 })),
-                s = ft(o);
+                s = xt(o);
             o = o.map(a => s.find(c => c.name === a.name) ? {
                 name: `x-bind:${a.name}`,
                 value: `"${a.value}"`
             } : a), t = t.concat(o)
         }
         let n = {};
-        return t.map(tr((o, s) => n[o] = s)).filter(rr).map(xn(n, r)).sort(yn).map(o => gn(e, o))
+        return t.map(sr((o, s) => n[o] = s)).filter(cr).map(An(n, r)).sort(On).map(o => Sn(e, o))
     }
 
-    function ft(e) {
-        return Array.from(e).map(tr()).filter(t => !rr(t))
+    function xt(e) {
+        return Array.from(e).map(sr()).filter(t => !cr(t))
     }
-    var dt = !1,
-        ie = new Map,
-        nr = Symbol();
+    var ht = !1,
+        ce = new Map,
+        ir = Symbol();
 
-    function ir(e) {
-        dt = !0;
+    function or(e) {
+        ht = !0;
         let t = Symbol();
-        nr = t, ie.set(t, []);
+        ir = t, ce.set(t, []);
         let r = () => {
-                for (; ie.get(t).length;) ie.get(t).shift()();
-                ie.delete(t)
+                for (; ce.get(t).length;) ce.get(t).shift()();
+                ce.delete(t)
             },
             n = () => {
-                dt = !1, r()
+                ht = !1, r()
             };
         e(r), n()
     }
 
-    function at(e) {
+    function ft(e) {
         let t = [],
             r = a => t.push(a),
-            [n, i] = Ft(e);
+            [n, i] = Vt(e);
         return t.push(i), [{
-            Alpine: I,
+            Alpine: F,
             effect: n,
             cleanup: r,
-            evaluateLater: g.bind(g, e),
-            evaluate: P.bind(P, e)
+            evaluateLater: x.bind(x, e),
+            evaluate: I.bind(I, e)
         }, () => t.forEach(a => a())]
     }
 
-    function gn(e, t) {
+    function Sn(e, t) {
         let r = () => {},
-            n = er[t.type] || r,
-            [i, o] = at(e);
-        qt(e, t.original, o);
+            n = mt[t.type] || r,
+            [i, o] = ft(e);
+        Jt(e, t.original, o);
         let s = () => {
-            e._x_ignore || e._x_ignoreSelf || (n.inline && n.inline(e, t, i), n = n.bind(n, e, t, i), dt ? ie.get(nr).push(n) : n())
+            e._x_ignore || e._x_ignoreSelf || (n.inline && n.inline(e, t, i), n = n.bind(n, e, t, i), ht ? ce.get(ir).push(n) : n())
         };
         return s.runCleanups = o, s
     }
-    var Ee = (e, t) => ({
+    var Ce = (e, t) => ({
             name: r,
             value: n
         }) => (r.startsWith(e) && (r = r.replace(e, t)), {
             name: r,
             value: n
         }),
-        Se = e => e;
+        Te = e => e;
 
-    function tr(e = () => {}) {
+    function sr(e = () => {}) {
         return ({
             name: t,
             value: r
         }) => {
             let {
                 name: n,
                 value: i
-            } = or.reduce((o, s) => s(o), {
+            } = ar.reduce((o, s) => s(o), {
                 name: t,
                 value: r
             });
             return n !== t && e(n, t), {
                 name: n,
                 value: i
             }
         }
     }
-    var or = [];
+    var ar = [];
 
-    function Z(e) {
-        or.push(e)
+    function Q(e) {
+        ar.push(e)
     }
 
-    function rr({
+    function cr({
         name: e
     }) {
-        return sr().test(e)
+        return lr().test(e)
     }
-    var sr = () => new RegExp(`^${ut}([^:^.]+)\\b`);
+    var lr = () => new RegExp(`^${gt}([^:^.]+)\\b`);
 
-    function xn(e, t) {
+    function An(e, t) {
         return ({
             name: r,
             value: n
         }) => {
-            let i = r.match(sr()),
+            let i = r.match(lr()),
                 o = r.match(/:([a-zA-Z0-9\-:]+)/),
                 s = r.match(/\.[^.\]]+(?=[^\]]*$)/g) || [],
                 a = t || e[r] || r;
             return {
                 type: i ? i[1] : null,
                 value: o ? o[1] : null,
                 modifiers: s.map(c => c.replace(".", "")),
                 expression: n,
                 original: a
             }
         }
     }
-    var pt = "DEFAULT",
-        Ae = ["ignore", "ref", "data", "id", "radio", "tabs", "switch", "disclosure", "menu", "listbox", "list", "item", "combobox", "bind", "init", "for", "mask", "model", "modelable", "transition", "show", "if", pt, "teleport"];
+    var _t = "DEFAULT",
+        H = ["ignore", "ref", "data", "id", "bind", "init", "for", "model", "modelable", "transition", "show", "if", _t, "teleport"];
 
-    function yn(e, t) {
-        let r = Ae.indexOf(e.type) === -1 ? pt : e.type,
-            n = Ae.indexOf(t.type) === -1 ? pt : t.type;
-        return Ae.indexOf(r) - Ae.indexOf(n)
+    function On(e, t) {
+        let r = H.indexOf(e.type) === -1 ? _t : e.type,
+            n = H.indexOf(t.type) === -1 ? _t : t.type;
+        return H.indexOf(r) - H.indexOf(n)
     }
 
-    function z(e, t, r = {}) {
+    function q(e, t, r = {}) {
         e.dispatchEvent(new CustomEvent(t, {
             detail: r,
             bubbles: !0,
             composed: !0,
             cancelable: !0
         }))
     }
-    var mt = [],
-        ht = !1;
-
-    function Te(e = () => {}) {
-        return queueMicrotask(() => {
-            ht || setTimeout(() => {
-                Oe()
-            })
-        }), new Promise(t => {
-            mt.push(() => {
-                e(), t()
-            })
-        })
-    }
-
-    function Oe() {
-        for (ht = !1; mt.length;) mt.shift()()
-    }
 
-    function ar() {
-        ht = !0
-    }
-
-    function R(e, t) {
+    function A(e, t) {
         if (typeof ShadowRoot == "function" && e instanceof ShadowRoot) {
-            Array.from(e.children).forEach(i => R(i, t));
+            Array.from(e.children).forEach(i => A(i, t));
             return
         }
         let r = !1;
         if (t(e, () => r = !0), r) return;
         let n = e.firstElementChild;
-        for (; n;) R(n, t, !1), n = n.nextElementSibling
+        for (; n;) A(n, t, !1), n = n.nextElementSibling
     }
 
-    function O(e, ...t) {
+    function T(e, ...t) {
         console.warn(`Alpine Warning: ${e}`, ...t)
     }
 
-    function lr() {
-        document.body || O("Unable to initialize. Trying to load Alpine before `<body>` is available. Did you forget to add `defer` in Alpine's `<script>` tag?"), z(document, "alpine:init"), z(document, "alpine:initializing"), rt(), Vt(t => w(t, R)), _e(t => bn(t)), Ht((t, r) => {
-            ne(t, r).forEach(n => n())
+    function ur() {
+        document.body || T("Unable to initialize. Trying to load Alpine before `<body>` is available. Did you forget to add `defer` in Alpine's `<script>` tag?"), q(document, "alpine:init"), q(document, "alpine:initializing"), se(), Wt(t => v(t, A)), we(t => bt(t)), Gt((t, r) => {
+            le(t, r).forEach(n => n())
         });
-        let e = t => !V(t.parentElement, !0);
-        Array.from(document.querySelectorAll(cr())).filter(e).forEach(t => {
-            w(t)
-        }), z(document, "alpine:initialized")
+        let e = t => !U(t.parentElement, !0);
+        Array.from(document.querySelectorAll(pr())).filter(e).forEach(t => {
+            v(t)
+        }), q(document, "alpine:initialized")
     }
-    var _t = [],
-        ur = [];
+    var yt = [],
+        fr = [];
 
-    function fr() {
-        return _t.map(e => e())
+    function dr() {
+        return yt.map(e => e())
     }
 
-    function cr() {
-        return _t.concat(ur).map(e => e())
+    function pr() {
+        return yt.concat(fr).map(e => e())
     }
 
-    function Ce(e) {
-        _t.push(e)
+    function Me(e) {
+        yt.push(e)
     }
 
     function Re(e) {
-        ur.push(e)
+        fr.push(e)
     }
 
-    function V(e, t = !1) {
-        return Q(e, r => {
-            if ((t ? cr() : fr()).some(i => r.matches(i))) return !0
+    function U(e, t = !1) {
+        return X(e, r => {
+            if ((t ? pr() : dr()).some(i => r.matches(i))) return !0
         })
     }
 
-    function Q(e, t) {
-        if (!!e) {
+    function X(e, t) {
+        if (e) {
             if (t(e)) return e;
-            if (e._x_teleportBack && (e = e._x_teleportBack), !!e.parentElement) return Q(e.parentElement, t)
+            if (e._x_teleportBack && (e = e._x_teleportBack), !!e.parentElement) return X(e.parentElement, t)
         }
     }
 
-    function dr(e) {
-        return fr().some(t => e.matches(t))
+    function mr(e) {
+        return dr().some(t => e.matches(t))
+    }
+    var hr = [];
+
+    function _r(e) {
+        hr.push(e)
+    }
+
+    function v(e, t = A, r = () => {}) {
+        or(() => {
+            t(e, (n, i) => {
+                r(n, i), hr.forEach(o => o(n, i)), le(n, n.attributes).forEach(o => o()), n._x_ignore && i()
+            })
+        })
+    }
+
+    function bt(e) {
+        A(e, t => nt(t))
     }
+    var wt = [],
+        Et = !1;
 
-    function w(e, t = R) {
-        ir(() => {
-            t(e, (r, n) => {
-                ne(r, r.attributes).forEach(i => i()), r._x_ignore && n()
+    function ee(e = () => {}) {
+        return queueMicrotask(() => {
+            Et || setTimeout(() => {
+                Ne()
+            })
+        }), new Promise(t => {
+            wt.push(() => {
+                e(), t()
             })
         })
     }
 
-    function bn(e) {
-        R(e, t => Qe(t))
+    function Ne() {
+        for (Et = !1; wt.length;) wt.shift()()
     }
 
-    function oe(e, t) {
-        return Array.isArray(t) ? pr(e, t.join(" ")) : typeof t == "object" && t !== null ? vn(e, t) : typeof t == "function" ? oe(e, t()) : pr(e, t)
+    function gr() {
+        Et = !0
     }
 
-    function pr(e, t) {
+    function ue(e, t) {
+        return Array.isArray(t) ? xr(e, t.join(" ")) : typeof t == "object" && t !== null ? Cn(e, t) : typeof t == "function" ? ue(e, t()) : xr(e, t)
+    }
+
+    function xr(e, t) {
         let r = o => o.split(" ").filter(Boolean),
             n = o => o.split(" ").filter(s => !e.classList.contains(s)).filter(Boolean),
             i = o => (e.classList.add(...o), () => {
                 e.classList.remove(...o)
             });
         return t = t === !0 ? t = "" : t || "", i(n(t))
     }
 
-    function vn(e, t) {
+    function Cn(e, t) {
         let r = a => a.split(" ").filter(Boolean),
             n = Object.entries(t).flatMap(([a, c]) => c ? r(a) : !1).filter(Boolean),
             i = Object.entries(t).flatMap(([a, c]) => c ? !1 : r(a)).filter(Boolean),
             o = [],
             s = [];
         return i.forEach(a => {
             e.classList.contains(a) && (e.classList.remove(a), s.push(a))
         }), n.forEach(a => {
             e.classList.contains(a) || (e.classList.add(a), o.push(a))
         }), () => {
             s.forEach(a => e.classList.add(a)), o.forEach(a => e.classList.remove(a))
         }
     }
 
-    function H(e, t) {
-        return typeof t == "object" && t !== null ? wn(e, t) : En(e, t)
+    function W(e, t) {
+        return typeof t == "object" && t !== null ? Tn(e, t) : Mn(e, t)
     }
 
-    function wn(e, t) {
+    function Tn(e, t) {
         let r = {};
         return Object.entries(t).forEach(([n, i]) => {
-            r[n] = e.style[n], n.startsWith("--") || (n = Sn(n)), e.style.setProperty(n, i)
+            r[n] = e.style[n], n.startsWith("--") || (n = Rn(n)), e.style.setProperty(n, i)
         }), setTimeout(() => {
             e.style.length === 0 && e.removeAttribute("style")
         }), () => {
-            H(e, r)
+            W(e, r)
         }
     }
 
-    function En(e, t) {
+    function Mn(e, t) {
         let r = e.getAttribute("style", t);
         return e.setAttribute("style", t), () => {
             e.setAttribute("style", r || "")
         }
     }
 
-    function Sn(e) {
+    function Rn(e) {
         return e.replace(/([a-z])([A-Z])/g, "$1-$2").toLowerCase()
     }
 
-    function se(e, t = () => {}) {
+    function fe(e, t = () => {}) {
         let r = !1;
         return function() {
             r ? t.apply(this, arguments) : (r = !0, e.apply(this, arguments))
         }
     }
-    d("transition", (e, {
+    p("transition", (e, {
         value: t,
         modifiers: r,
         expression: n
     }, {
         evaluate: i
     }) => {
-        typeof n == "function" && (n = i(n)), n ? An(e, n, t) : On(e, r, t)
+        typeof n == "function" && (n = i(n)), n ? Nn(e, n, t) : Dn(e, r, t)
     });
 
-    function An(e, t, r) {
-        mr(e, oe, ""), {
+    function Nn(e, t, r) {
+        yr(e, ue, ""), {
             enter: i => {
                 e._x_transition.enter.during = i
             },
             "enter-start": i => {
                 e._x_transition.enter.start = i
             },
             "enter-end": i => {
@@ -717,79 +731,79 @@
             },
             "leave-end": i => {
                 e._x_transition.leave.end = i
             }
         } [r](t)
     }
 
-    function On(e, t, r) {
-        mr(e, H);
+    function Dn(e, t, r) {
+        yr(e, W);
         let n = !t.includes("in") && !t.includes("out") && !r,
             i = n || t.includes("in") || ["enter"].includes(r),
             o = n || t.includes("out") || ["leave"].includes(r);
-        t.includes("in") && !n && (t = t.filter((h, b) => b < t.indexOf("out"))), t.includes("out") && !n && (t = t.filter((h, b) => b > t.indexOf("out")));
+        t.includes("in") && !n && (t = t.filter((_, b) => b < t.indexOf("out"))), t.includes("out") && !n && (t = t.filter((_, b) => b > t.indexOf("out")));
         let s = !t.includes("opacity") && !t.includes("scale"),
             a = s || t.includes("opacity"),
             c = s || t.includes("scale"),
             l = a ? 0 : 1,
-            u = c ? ae(t, "scale", 95) / 100 : 1,
-            p = ae(t, "delay", 0),
-            y = ae(t, "origin", "center"),
-            N = "opacity, transform",
-            W = ae(t, "duration", 150) / 1e3,
-            pe = ae(t, "duration", 75) / 1e3,
+            u = c ? de(t, "scale", 95) / 100 : 1,
+            d = de(t, "delay", 0),
+            m = de(t, "origin", "center"),
+            w = "opacity, transform",
+            k = de(t, "duration", 150) / 1e3,
+            ge = de(t, "duration", 75) / 1e3,
             f = "cubic-bezier(0.4, 0.0, 0.2, 1)";
         i && (e._x_transition.enter.during = {
-            transformOrigin: y,
-            transitionDelay: p,
-            transitionProperty: N,
-            transitionDuration: `${W}s`,
+            transformOrigin: m,
+            transitionDelay: d,
+            transitionProperty: w,
+            transitionDuration: `${k}s`,
             transitionTimingFunction: f
         }, e._x_transition.enter.start = {
             opacity: l,
             transform: `scale(${u})`
         }, e._x_transition.enter.end = {
             opacity: 1,
             transform: "scale(1)"
         }), o && (e._x_transition.leave.during = {
-            transformOrigin: y,
-            transitionDelay: p,
-            transitionProperty: N,
-            transitionDuration: `${pe}s`,
+            transformOrigin: m,
+            transitionDelay: d,
+            transitionProperty: w,
+            transitionDuration: `${ge}s`,
             transitionTimingFunction: f
         }, e._x_transition.leave.start = {
             opacity: 1,
             transform: "scale(1)"
         }, e._x_transition.leave.end = {
             opacity: l,
             transform: `scale(${u})`
         })
     }
 
-    function mr(e, t, r = {}) {
+    function yr(e, t, r = {}) {
         e._x_transition || (e._x_transition = {
             enter: {
                 during: r,
                 start: r,
                 end: r
             },
             leave: {
                 during: r,
                 start: r,
                 end: r
             },
             in(n = () => {}, i = () => {}) {
-                Me(e, t, {
+                De(e, t, {
                     during: this.enter.during,
                     start: this.enter.start,
                     end: this.enter.end
                 }, n, i)
             },
             out(n = () => {}, i = () => {}) {
-                Me(e, t, {
+                De(e, t, {
                     during: this.leave.during,
                     start: this.leave.start,
                     end: this.leave.end
                 }, n, i)
             }
         })
     }
@@ -801,43 +815,43 @@
             return
         }
         e._x_hidePromise = e._x_transition ? new Promise((s, a) => {
             e._x_transition.out(() => {}, () => s(n)), e._x_transitioning.beforeCancel(() => a({
                 isFromCancelledTransition: !0
             }))
         }) : Promise.resolve(n), queueMicrotask(() => {
-            let s = hr(e);
+            let s = br(e);
             s ? (s._x_hideChildren || (s._x_hideChildren = []), s._x_hideChildren.push(e)) : i(() => {
                 let a = c => {
                     let l = Promise.all([c._x_hidePromise, ...(c._x_hideChildren || []).map(a)]).then(([u]) => u());
                     return delete c._x_hidePromise, delete c._x_hideChildren, l
                 };
                 a(e).catch(c => {
                     if (!c.isFromCancelledTransition) throw c
                 })
             })
         })
     };
 
-    function hr(e) {
+    function br(e) {
         let t = e.parentNode;
-        if (!!t) return t._x_hidePromise ? t : hr(t)
+        if (t) return t._x_hidePromise ? t : br(t)
     }
 
-    function Me(e, t, {
+    function De(e, t, {
         during: r,
         start: n,
         end: i
     } = {}, o = () => {}, s = () => {}) {
         if (e._x_transitioning && e._x_transitioning.cancel(), Object.keys(r).length === 0 && Object.keys(n).length === 0 && Object.keys(i).length === 0) {
             o(), s();
             return
         }
         let a, c, l;
-        Tn(e, {
+        Pn(e, {
             start() {
                 a = t(e, n)
             },
             during() {
                 c = t(e, r)
             },
             before: o,
@@ -847,444 +861,433 @@
             after: s,
             cleanup() {
                 c(), l()
             }
         })
     }
 
-    function Tn(e, t) {
-        let r, n, i, o = se(() => {
-            m(() => {
-                r = !0, n || t.before(), i || (t.end(), Oe()), t.after(), e.isConnected && t.cleanup(), delete e._x_transitioning
+    function Pn(e, t) {
+        let r, n, i, o = fe(() => {
+            h(() => {
+                r = !0, n || t.before(), i || (t.end(), Ne()), t.after(), e.isConnected && t.cleanup(), delete e._x_transitioning
             })
         });
         e._x_transitioning = {
             beforeCancels: [],
             beforeCancel(s) {
                 this.beforeCancels.push(s)
             },
-            cancel: se(function() {
+            cancel: fe(function() {
                 for (; this.beforeCancels.length;) this.beforeCancels.shift()();
                 o()
             }),
             finish: o
-        }, m(() => {
+        }, h(() => {
             t.start(), t.during()
-        }), ar(), requestAnimationFrame(() => {
+        }), gr(), requestAnimationFrame(() => {
             if (r) return;
             let s = Number(getComputedStyle(e).transitionDuration.replace(/,.*/, "").replace("s", "")) * 1e3,
                 a = Number(getComputedStyle(e).transitionDelay.replace(/,.*/, "").replace("s", "")) * 1e3;
-            s === 0 && (s = Number(getComputedStyle(e).animationDuration.replace("s", "")) * 1e3), m(() => {
+            s === 0 && (s = Number(getComputedStyle(e).animationDuration.replace("s", "")) * 1e3), h(() => {
                 t.before()
             }), n = !0, requestAnimationFrame(() => {
-                r || (m(() => {
+                r || (h(() => {
                     t.end()
-                }), Oe(), setTimeout(e._x_transitioning.finish, s + a), i = !0)
+                }), Ne(), setTimeout(e._x_transitioning.finish, s + a), i = !0)
             })
         })
     }
 
-    function ae(e, t, r) {
+    function de(e, t, r) {
         if (e.indexOf(t) === -1) return r;
         let n = e[e.indexOf(t) + 1];
         if (!n || t === "scale" && isNaN(n)) return r;
         if (t === "duration") {
             let i = n.match(/([0-9]+)ms/);
             if (i) return i[1]
         }
         return t === "origin" && ["top", "right", "left", "center", "bottom"].includes(e[e.indexOf(t) + 2]) ? [n, e[e.indexOf(t) + 2]].join(" ") : n
     }
-    var gt = !1;
+    var te = !1;
+
+    function N(e, t = () => {}) {
+        return (...r) => te ? t(...r) : e(...r)
+    }
 
-    function $(e, t = () => {}) {
-        return (...r) => gt ? t(...r) : e(...r)
+    function wr(e) {
+        return (...t) => te && e(...t)
     }
 
-    function _r(e, t) {
-        t._x_dataStack || (t._x_dataStack = e._x_dataStack), gt = !0, Rn(() => {
-            Cn(t)
-        }), gt = !1
+    function Er(e, t) {
+        t._x_dataStack || (t._x_dataStack = e._x_dataStack), te = !0, kn(() => {
+            In(t)
+        }), te = !1
     }
 
-    function Cn(e) {
+    function In(e) {
         let t = !1;
-        w(e, (n, i) => {
-            R(n, (o, s) => {
-                if (t && dr(o)) return s();
+        v(e, (n, i) => {
+            A(n, (o, s) => {
+                if (t && mr(o)) return s();
                 t = !0, i(o, s)
             })
         })
     }
 
-    function Rn(e) {
-        let t = K;
-        Ze((r, n) => {
+    function kn(e) {
+        let t = P;
+        tt((r, n) => {
             let i = t(r);
-            return Y(i), () => {}
-        }), e(), Ze(t)
+            return L(i), () => {}
+        }), e(), tt(t)
     }
 
-    function ce(e, t, r, n = []) {
-        switch (e._x_bindings || (e._x_bindings = A({})), e._x_bindings[t] = r, t = n.includes("camel") ? Dn(t) : t, t) {
+    function pe(e, t, r, n = []) {
+        switch (e._x_bindings || (e._x_bindings = C({})), e._x_bindings[t] = r, t = n.includes("camel") ? zn(t) : t, t) {
             case "value":
-                Mn(e, r);
+                Ln(e, r);
                 break;
             case "style":
-                Pn(e, r);
+                jn(e, r);
                 break;
             case "class":
-                Nn(e, r);
+                $n(e, r);
                 break;
             default:
-                kn(e, t, r);
+                Fn(e, t, r);
                 break
         }
     }
 
-    function Mn(e, t) {
-        if (e.type === "radio") e.attributes.value === void 0 && (e.value = t), window.fromModel && (e.checked = gr(e.value, t));
-        else if (e.type === "checkbox") Number.isInteger(t) ? e.value = t : !Number.isInteger(t) && !Array.isArray(t) && typeof t != "boolean" && ![null, void 0].includes(t) ? e.value = String(t) : Array.isArray(t) ? e.checked = t.some(r => gr(r, e.value)) : e.checked = !!t;
-        else if (e.tagName === "SELECT") In(e, t);
+    function Ln(e, t) {
+        if (e.type === "radio") e.attributes.value === void 0 && (e.value = t), window.fromModel && (e.checked = vr(e.value, t));
+        else if (e.type === "checkbox") Number.isInteger(t) ? e.value = t : !Number.isInteger(t) && !Array.isArray(t) && typeof t != "boolean" && ![null, void 0].includes(t) ? e.value = String(t) : Array.isArray(t) ? e.checked = t.some(r => vr(r, e.value)) : e.checked = !!t;
+        else if (e.tagName === "SELECT") Kn(e, t);
         else {
             if (e.value === t) return;
             e.value = t
         }
     }
 
-    function Nn(e, t) {
-        e._x_undoAddedClasses && e._x_undoAddedClasses(), e._x_undoAddedClasses = oe(e, t)
+    function $n(e, t) {
+        e._x_undoAddedClasses && e._x_undoAddedClasses(), e._x_undoAddedClasses = ue(e, t)
     }
 
-    function Pn(e, t) {
-        e._x_undoAddedStyles && e._x_undoAddedStyles(), e._x_undoAddedStyles = H(e, t)
+    function jn(e, t) {
+        e._x_undoAddedStyles && e._x_undoAddedStyles(), e._x_undoAddedStyles = W(e, t)
     }
 
-    function kn(e, t, r) {
-        [null, void 0, !1].includes(r) && Ln(t) ? e.removeAttribute(t) : (xr(t) && (r = t), $n(e, t, r))
+    function Fn(e, t, r) {
+        [null, void 0, !1].includes(r) && Vn(t) ? e.removeAttribute(t) : (Sr(t) && (r = t), Bn(e, t, r))
     }
 
-    function $n(e, t, r) {
+    function Bn(e, t, r) {
         e.getAttribute(t) != r && e.setAttribute(t, r)
     }
 
-    function In(e, t) {
+    function Kn(e, t) {
         let r = [].concat(t).map(n => n + "");
         Array.from(e.options).forEach(n => {
             n.selected = r.includes(n.value)
         })
     }
 
-    function Dn(e) {
+    function zn(e) {
         return e.toLowerCase().replace(/-(\w)/g, (t, r) => r.toUpperCase())
     }
 
-    function gr(e, t) {
+    function vr(e, t) {
         return e == t
     }
 
-    function xr(e) {
+    function Sr(e) {
         return ["disabled", "checked", "required", "readonly", "hidden", "open", "selected", "autofocus", "itemscope", "multiple", "novalidate", "allowfullscreen", "allowpaymentrequest", "formnovalidate", "autoplay", "controls", "loop", "muted", "playsinline", "default", "ismap", "reversed", "async", "defer", "nomodule"].includes(e)
     }
 
-    function Ln(e) {
+    function Vn(e) {
         return !["aria-pressed", "aria-checked", "aria-expanded", "aria-selected"].includes(e)
     }
 
-    function yr(e, t, r) {
+    function Ar(e, t, r) {
         if (e._x_bindings && e._x_bindings[t] !== void 0) return e._x_bindings[t];
         let n = e.getAttribute(t);
-        return n === null ? typeof r == "function" ? r() : r : n === "" ? !0 : xr(t) ? !![t, "true"].includes(n) : n
+        return n === null ? typeof r == "function" ? r() : r : n === "" ? !0 : Sr(t) ? !![t, "true"].includes(n) : n
     }
 
-    function Ne(e, t) {
+    function Pe(e, t) {
         var r;
         return function() {
             var n = this,
                 i = arguments,
                 o = function() {
                     r = null, e.apply(n, i)
                 };
             clearTimeout(r), r = setTimeout(o, t)
         }
     }
 
-    function Pe(e, t) {
+    function Ie(e, t) {
         let r;
         return function() {
             let n = this,
                 i = arguments;
             r || (e.apply(n, i), r = !0, setTimeout(() => r = !1, t))
         }
     }
 
-    function br(e) {
-        e(I)
+    function Or(e) {
+        e(F)
     }
-    var q = {},
-        vr = !1;
+    var G = {},
+        Cr = !1;
 
-    function wr(e, t) {
-        if (vr || (q = A(q), vr = !0), t === void 0) return q[e];
-        q[e] = t, typeof t == "object" && t !== null && t.hasOwnProperty("init") && typeof t.init == "function" && q[e].init(), ye(q[e])
+    function Tr(e, t) {
+        if (Cr || (G = C(G), Cr = !0), t === void 0) return G[e];
+        G[e] = t, typeof t == "object" && t !== null && t.hasOwnProperty("init") && typeof t.init == "function" && G[e].init(), ve(G[e])
     }
 
-    function Er() {
-        return q
+    function Mr() {
+        return G
     }
-    var Sr = {};
+    var Rr = {};
 
-    function Ar(e, t) {
+    function Nr(e, t) {
         let r = typeof t != "function" ? () => t : t;
-        e instanceof Element ? xt(e, r()) : Sr[e] = r
+        e instanceof Element ? vt(e, r()) : Rr[e] = r
     }
 
-    function Or(e) {
-        return Object.entries(Sr).forEach(([t, r]) => {
+    function Dr(e) {
+        return Object.entries(Rr).forEach(([t, r]) => {
             Object.defineProperty(e, t, {
                 get() {
                     return (...n) => r(...n)
                 }
             })
         }), e
     }
 
-    function xt(e, t, r) {
+    function vt(e, t, r) {
         let n = [];
         for (; n.length;) n.pop()();
         let i = Object.entries(t).map(([s, a]) => ({
                 name: s,
                 value: a
             })),
-            o = ft(i);
+            o = xt(i);
         i = i.map(s => o.find(a => a.name === s.name) ? {
             name: `x-bind:${s.name}`,
             value: `"${s.value}"`
-        } : s), ne(e, i, r).map(s => {
+        } : s), le(e, i, r).map(s => {
             n.push(s.runCleanups), s()
         })
     }
-    var Tr = {};
+    var Pr = {};
 
-    function Cr(e, t) {
-        Tr[e] = t
+    function Ir(e, t) {
+        Pr[e] = t
     }
 
-    function Rr(e, t) {
-        return Object.entries(Tr).forEach(([r, n]) => {
+    function kr(e, t) {
+        return Object.entries(Pr).forEach(([r, n]) => {
             Object.defineProperty(e, r, {
                 get() {
                     return (...i) => n.bind(t)(...i)
                 },
                 enumerable: !1
             })
         }), e
     }
-    var jn = {
+    var Hn = {
             get reactive() {
-                return A
+                return C
             },
             get release() {
-                return Y
+                return L
             },
             get effect() {
-                return K
+                return P
             },
             get raw() {
-                return Ye
+                return et
             },
-            version: "3.10.5",
-            flushAndStopDeferringMutations: Wt,
-            dontAutoEvaluateFunctions: Jt,
-            disableEffectScheduling: Lt,
-            setReactivityEngine: jt,
-            closestDataStack: k,
-            skipDuringClone: $,
-            addRootSelector: Ce,
+            version: "3.12.0",
+            flushAndStopDeferringMutations: Zt,
+            dontAutoEvaluateFunctions: er,
+            disableEffectScheduling: Kt,
+            startObservingMutations: se,
+            stopObservingMutations: st,
+            setReactivityEngine: zt,
+            closestDataStack: $,
+            skipDuringClone: N,
+            onlyDuringClone: wr,
+            addRootSelector: Me,
             addInitSelector: Re,
-            addScopeToNode: C,
-            deferMutations: Ut,
-            mapAttributes: Z,
-            evaluateLater: g,
-            setEvaluator: Qt,
-            mergeProxies: D,
-            findClosest: Q,
-            closestRoot: V,
-            interceptor: be,
-            transition: Me,
-            setStyles: H,
-            mutateDom: m,
-            directive: d,
-            throttle: Pe,
-            debounce: Ne,
-            evaluate: P,
-            initTree: w,
-            nextTick: Te,
-            prefixed: E,
-            prefix: Xt,
-            plugin: br,
-            magic: x,
-            store: wr,
-            start: lr,
-            clone: _r,
-            bound: yr,
-            $data: xe,
-            data: Cr,
-            bind: Ar
+            addScopeToNode: R,
+            deferMutations: Yt,
+            mapAttributes: Q,
+            evaluateLater: x,
+            interceptInit: _r,
+            setEvaluator: rr,
+            mergeProxies: j,
+            findClosest: X,
+            closestRoot: U,
+            destroyTree: bt,
+            interceptor: Se,
+            transition: De,
+            setStyles: W,
+            mutateDom: h,
+            directive: p,
+            throttle: Ie,
+            debounce: Pe,
+            evaluate: I,
+            initTree: v,
+            nextTick: ee,
+            prefixed: S,
+            prefix: nr,
+            plugin: Or,
+            magic: y,
+            store: Tr,
+            start: ur,
+            clone: Er,
+            bound: Ar,
+            $data: Ee,
+            walk: A,
+            data: Ir,
+            bind: Nr
         },
-        I = jn;
+        F = Hn;
 
-    function yt(e, t) {
+    function St(e, t) {
         let r = Object.create(null),
             n = e.split(",");
         for (let i = 0; i < n.length; i++) r[n[i]] = !0;
         return t ? i => !!r[i.toLowerCase()] : i => !!r[i]
     }
-    var ns = {
-            [1]: "TEXT",
-            [2]: "CLASS",
-            [4]: "STYLE",
-            [8]: "PROPS",
-            [16]: "FULL_PROPS",
-            [32]: "HYDRATE_EVENTS",
-            [64]: "STABLE_FRAGMENT",
-            [128]: "KEYED_FRAGMENT",
-            [256]: "UNKEYED_FRAGMENT",
-            [512]: "NEED_PATCH",
-            [1024]: "DYNAMIC_SLOTS",
-            [2048]: "DEV_ROOT_FRAGMENT",
-            [-1]: "HOISTED",
-            [-2]: "BAIL"
-        },
-        is = {
-            [1]: "STABLE",
-            [2]: "DYNAMIC",
-            [3]: "FORWARDED"
-        };
-    var Fn = "itemscope,allowfullscreen,formnovalidate,ismap,nomodule,novalidate,readonly";
-    var os = yt(Fn + ",async,autofocus,autoplay,controls,default,defer,disabled,hidden,loop,open,required,reversed,scoped,seamless,checked,muted,multiple,selected");
-    var Mr = Object.freeze({}),
-        ss = Object.freeze([]);
-    var bt = Object.assign;
-    var Bn = Object.prototype.hasOwnProperty,
-        le = (e, t) => Bn.call(e, t),
-        L = Array.isArray,
-        X = e => Nr(e) === "[object Map]";
-    var Kn = e => typeof e == "string",
+    var qn = "itemscope,allowfullscreen,formnovalidate,ismap,nomodule,novalidate,readonly";
+    var cs = St(qn + ",async,autofocus,autoplay,controls,default,defer,disabled,hidden,loop,open,required,reversed,scoped,seamless,checked,muted,multiple,selected");
+    var Lr = Object.freeze({}),
+        ls = Object.freeze([]);
+    var At = Object.assign;
+    var Un = Object.prototype.hasOwnProperty,
+        me = (e, t) => Un.call(e, t),
+        B = Array.isArray,
+        re = e => $r(e) === "[object Map]";
+    var Wn = e => typeof e == "string",
         ke = e => typeof e == "symbol",
-        ue = e => e !== null && typeof e == "object";
-    var zn = Object.prototype.toString,
-        Nr = e => zn.call(e),
-        vt = e => Nr(e).slice(8, -1);
-    var De = e => Kn(e) && e !== "NaN" && e[0] !== "-" && "" + parseInt(e, 10) === e;
-    var Ie = e => {
+        he = e => e !== null && typeof e == "object";
+    var Gn = Object.prototype.toString,
+        $r = e => Gn.call(e),
+        Ot = e => $r(e).slice(8, -1);
+    var Le = e => Wn(e) && e !== "NaN" && e[0] !== "-" && "" + parseInt(e, 10) === e;
+    var $e = e => {
             let t = Object.create(null);
             return r => t[r] || (t[r] = e(r))
         },
-        Vn = /-(\w)/g,
-        as = Ie(e => e.replace(Vn, (t, r) => r ? r.toUpperCase() : "")),
-        Hn = /\B([A-Z])/g,
-        cs = Ie(e => e.replace(Hn, "-$1").toLowerCase()),
-        wt = Ie(e => e.charAt(0).toUpperCase() + e.slice(1)),
-        ls = Ie(e => e ? `on${wt(e)}` : ""),
-        Et = (e, t) => e !== t && (e === e || t === t);
-    var St = new WeakMap,
-        fe = [],
-        M, U = Symbol("iterate"),
-        At = Symbol("Map key iterate");
+        Jn = /-(\w)/g,
+        us = $e(e => e.replace(Jn, (t, r) => r ? r.toUpperCase() : "")),
+        Yn = /\B([A-Z])/g,
+        fs = $e(e => e.replace(Yn, "-$1").toLowerCase()),
+        Ct = $e(e => e.charAt(0).toUpperCase() + e.slice(1)),
+        ds = $e(e => e ? `on${Ct(e)}` : ""),
+        Tt = (e, t) => e !== t && (e === e || t === t);
+    var Mt = new WeakMap,
+        _e = [],
+        D, J = Symbol("iterate"),
+        Rt = Symbol("Map key iterate");
 
-    function qn(e) {
+    function Zn(e) {
         return e && e._isEffect === !0
     }
 
-    function Pr(e, t = Mr) {
-        qn(e) && (e = e.raw);
-        let r = Un(e, t);
+    function jr(e, t = Lr) {
+        Zn(e) && (e = e.raw);
+        let r = Xn(e, t);
         return t.lazy || r(), r
     }
 
-    function Dr(e) {
-        e.active && (kr(e), e.options.onStop && e.options.onStop(), e.active = !1)
+    function Fr(e) {
+        e.active && (Br(e), e.options.onStop && e.options.onStop(), e.active = !1)
     }
-    var Wn = 0;
+    var Qn = 0;
 
-    function Un(e, t) {
+    function Xn(e, t) {
         let r = function() {
             if (!r.active) return e();
-            if (!fe.includes(r)) {
-                kr(r);
+            if (!_e.includes(r)) {
+                Br(r);
                 try {
-                    return Gn(), fe.push(r), M = r, e()
+                    return ti(), _e.push(r), D = r, e()
                 } finally {
-                    fe.pop(), Ir(), M = fe[fe.length - 1]
+                    _e.pop(), Kr(), D = _e[_e.length - 1]
                 }
             }
         };
-        return r.id = Wn++, r.allowRecurse = !!t.allowRecurse, r._isEffect = !0, r.active = !0, r.raw = e, r.deps = [], r.options = t, r
+        return r.id = Qn++, r.allowRecurse = !!t.allowRecurse, r._isEffect = !0, r.active = !0, r.raw = e, r.deps = [], r.options = t, r
     }
 
-    function kr(e) {
+    function Br(e) {
         let {
             deps: t
         } = e;
         if (t.length) {
             for (let r = 0; r < t.length; r++) t[r].delete(e);
             t.length = 0
         }
     }
-    var ee = !0,
-        Ot = [];
+    var ne = !0,
+        Dt = [];
 
-    function Yn() {
-        Ot.push(ee), ee = !1
+    function ei() {
+        Dt.push(ne), ne = !1
     }
 
-    function Gn() {
-        Ot.push(ee), ee = !0
+    function ti() {
+        Dt.push(ne), ne = !0
     }
 
-    function Ir() {
-        let e = Ot.pop();
-        ee = e === void 0 ? !0 : e
+    function Kr() {
+        let e = Dt.pop();
+        ne = e === void 0 ? !0 : e
     }
 
-    function T(e, t, r) {
-        if (!ee || M === void 0) return;
-        let n = St.get(e);
-        n || St.set(e, n = new Map);
+    function M(e, t, r) {
+        if (!ne || D === void 0) return;
+        let n = Mt.get(e);
+        n || Mt.set(e, n = new Map);
         let i = n.get(r);
-        i || n.set(r, i = new Set), i.has(M) || (i.add(M), M.deps.push(i), M.options.onTrack && M.options.onTrack({
-            effect: M,
+        i || n.set(r, i = new Set), i.has(D) || (i.add(D), D.deps.push(i), D.options.onTrack && D.options.onTrack({
+            effect: D,
             target: e,
             type: t,
             key: r
         }))
     }
 
-    function j(e, t, r, n, i, o) {
-        let s = St.get(e);
+    function z(e, t, r, n, i, o) {
+        let s = Mt.get(e);
         if (!s) return;
         let a = new Set,
             c = u => {
-                u && u.forEach(p => {
-                    (p !== M || p.allowRecurse) && a.add(p)
+                u && u.forEach(d => {
+                    (d !== D || d.allowRecurse) && a.add(d)
                 })
             };
         if (t === "clear") s.forEach(c);
-        else if (r === "length" && L(e)) s.forEach((u, p) => {
-            (p === "length" || p >= n) && c(u)
+        else if (r === "length" && B(e)) s.forEach((u, d) => {
+            (d === "length" || d >= n) && c(u)
         });
         else switch (r !== void 0 && c(s.get(r)), t) {
             case "add":
-                L(e) ? De(r) && c(s.get("length")) : (c(s.get(U)), X(e) && c(s.get(At)));
+                B(e) ? Le(r) && c(s.get("length")) : (c(s.get(J)), re(e) && c(s.get(Rt)));
                 break;
             case "delete":
-                L(e) || (c(s.get(U)), X(e) && c(s.get(At)));
+                B(e) || (c(s.get(J)), re(e) && c(s.get(Rt)));
                 break;
             case "set":
-                X(e) && c(s.get(U));
+                re(e) && c(s.get(J));
                 break
         }
         let l = u => {
             u.options.onTrigger && u.options.onTrigger({
                 effect: u,
                 target: e,
                 key: r,
@@ -1292,940 +1295,992 @@
                 newValue: n,
                 oldValue: i,
                 oldTarget: o
             }), u.options.scheduler ? u.options.scheduler(u) : u()
         };
         a.forEach(l)
     }
-    var Jn = yt("__proto__,__v_isRef,__isVue"),
-        $r = new Set(Object.getOwnPropertyNames(Symbol).map(e => Symbol[e]).filter(ke)),
-        Zn = $e(),
-        Qn = $e(!1, !0),
-        Xn = $e(!0),
-        ei = $e(!0, !0),
-        Le = {};
+    var ri = St("__proto__,__v_isRef,__isVue"),
+        zr = new Set(Object.getOwnPropertyNames(Symbol).map(e => Symbol[e]).filter(ke)),
+        ni = Be(),
+        ii = Be(!1, !0),
+        oi = Be(!0),
+        si = Be(!0, !0),
+        Fe = {};
     ["includes", "indexOf", "lastIndexOf"].forEach(e => {
         let t = Array.prototype[e];
-        Le[e] = function(...r) {
-            let n = _(this);
-            for (let o = 0, s = this.length; o < s; o++) T(n, "get", o + "");
+        Fe[e] = function(...r) {
+            let n = g(this);
+            for (let o = 0, s = this.length; o < s; o++) M(n, "get", o + "");
             let i = t.apply(n, r);
-            return i === -1 || i === !1 ? t.apply(n, r.map(_)) : i
+            return i === -1 || i === !1 ? t.apply(n, r.map(g)) : i
         }
     });
     ["push", "pop", "shift", "unshift", "splice"].forEach(e => {
         let t = Array.prototype[e];
-        Le[e] = function(...r) {
-            Yn();
+        Fe[e] = function(...r) {
+            ei();
             let n = t.apply(this, r);
-            return Ir(), n
+            return Kr(), n
         }
     });
 
-    function $e(e = !1, t = !1) {
+    function Be(e = !1, t = !1) {
         return function(n, i, o) {
             if (i === "__v_isReactive") return !e;
             if (i === "__v_isReadonly") return e;
-            if (i === "__v_raw" && o === (e ? t ? ri : jr : t ? ti : Lr).get(n)) return n;
-            let s = L(n);
-            if (!e && s && le(Le, i)) return Reflect.get(Le, i, o);
+            if (i === "__v_raw" && o === (e ? t ? _i : rn : t ? hi : tn).get(n)) return n;
+            let s = B(n);
+            if (!e && s && me(Fe, i)) return Reflect.get(Fe, i, o);
             let a = Reflect.get(n, i, o);
-            return (ke(i) ? $r.has(i) : Jn(i)) || (e || T(n, "get", i), t) ? a : Tt(a) ? !s || !De(i) ? a.value : a : ue(a) ? e ? Fr(a) : je(a) : a
+            return (ke(i) ? zr.has(i) : ri(i)) || (e || M(n, "get", i), t) ? a : Nt(a) ? !s || !Le(i) ? a.value : a : he(a) ? e ? nn(a) : We(a) : a
         }
     }
-    var ni = Br(),
-        ii = Br(!0);
+    var ai = Vr(),
+        ci = Vr(!0);
 
-    function Br(e = !1) {
+    function Vr(e = !1) {
         return function(r, n, i, o) {
             let s = r[n];
-            if (!e && (i = _(i), s = _(s), !L(r) && Tt(s) && !Tt(i))) return s.value = i, !0;
-            let a = L(r) && De(n) ? Number(n) < r.length : le(r, n),
+            if (!e && (i = g(i), s = g(s), !B(r) && Nt(s) && !Nt(i))) return s.value = i, !0;
+            let a = B(r) && Le(n) ? Number(n) < r.length : me(r, n),
                 c = Reflect.set(r, n, i, o);
-            return r === _(o) && (a ? Et(i, s) && j(r, "set", n, i, s) : j(r, "add", n, i)), c
+            return r === g(o) && (a ? Tt(i, s) && z(r, "set", n, i, s) : z(r, "add", n, i)), c
         }
     }
 
-    function oi(e, t) {
-        let r = le(e, t),
+    function li(e, t) {
+        let r = me(e, t),
             n = e[t],
             i = Reflect.deleteProperty(e, t);
-        return i && r && j(e, "delete", t, void 0, n), i
+        return i && r && z(e, "delete", t, void 0, n), i
     }
 
-    function si(e, t) {
+    function ui(e, t) {
         let r = Reflect.has(e, t);
-        return (!ke(t) || !$r.has(t)) && T(e, "has", t), r
+        return (!ke(t) || !zr.has(t)) && M(e, "has", t), r
     }
 
-    function ai(e) {
-        return T(e, "iterate", L(e) ? "length" : U), Reflect.ownKeys(e)
+    function fi(e) {
+        return M(e, "iterate", B(e) ? "length" : J), Reflect.ownKeys(e)
     }
-    var Kr = {
-            get: Zn,
-            set: ni,
-            deleteProperty: oi,
-            has: si,
-            ownKeys: ai
+    var Hr = {
+            get: ni,
+            set: ai,
+            deleteProperty: li,
+            has: ui,
+            ownKeys: fi
         },
-        zr = {
-            get: Xn,
+        qr = {
+            get: oi,
             set(e, t) {
                 return console.warn(`Set operation on key "${String(t)}" failed: target is readonly.`, e), !0
             },
             deleteProperty(e, t) {
                 return console.warn(`Delete operation on key "${String(t)}" failed: target is readonly.`, e), !0
             }
         },
-        hs = bt({}, Kr, {
-            get: Qn,
-            set: ii
+        xs = At({}, Hr, {
+            get: ii,
+            set: ci
         }),
-        _s = bt({}, zr, {
-            get: ei
+        ys = At({}, qr, {
+            get: si
         }),
-        Ct = e => ue(e) ? je(e) : e,
-        Rt = e => ue(e) ? Fr(e) : e,
-        Mt = e => e,
-        Fe = e => Reflect.getPrototypeOf(e);
+        Pt = e => he(e) ? We(e) : e,
+        It = e => he(e) ? nn(e) : e,
+        kt = e => e,
+        Ke = e => Reflect.getPrototypeOf(e);
 
-    function Be(e, t, r = !1, n = !1) {
+    function ze(e, t, r = !1, n = !1) {
         e = e.__v_raw;
-        let i = _(e),
-            o = _(t);
-        t !== o && !r && T(i, "get", t), !r && T(i, "get", o);
+        let i = g(e),
+            o = g(t);
+        t !== o && !r && M(i, "get", t), !r && M(i, "get", o);
         let {
             has: s
-        } = Fe(i), a = n ? Mt : r ? Rt : Ct;
+        } = Ke(i), a = n ? kt : r ? It : Pt;
         if (s.call(i, t)) return a(e.get(t));
         if (s.call(i, o)) return a(e.get(o));
         e !== i && e.get(t)
     }
 
-    function Ke(e, t = !1) {
+    function Ve(e, t = !1) {
         let r = this.__v_raw,
-            n = _(r),
-            i = _(e);
-        return e !== i && !t && T(n, "has", e), !t && T(n, "has", i), e === i ? r.has(e) : r.has(e) || r.has(i)
+            n = g(r),
+            i = g(e);
+        return e !== i && !t && M(n, "has", e), !t && M(n, "has", i), e === i ? r.has(e) : r.has(e) || r.has(i)
     }
 
-    function ze(e, t = !1) {
-        return e = e.__v_raw, !t && T(_(e), "iterate", U), Reflect.get(e, "size", e)
+    function He(e, t = !1) {
+        return e = e.__v_raw, !t && M(g(e), "iterate", J), Reflect.get(e, "size", e)
     }
 
-    function Vr(e) {
-        e = _(e);
-        let t = _(this);
-        return Fe(t).has.call(t, e) || (t.add(e), j(t, "add", e, e)), this
+    function Ur(e) {
+        e = g(e);
+        let t = g(this);
+        return Ke(t).has.call(t, e) || (t.add(e), z(t, "add", e, e)), this
     }
 
-    function qr(e, t) {
-        t = _(t);
-        let r = _(this),
+    function Wr(e, t) {
+        t = g(t);
+        let r = g(this),
             {
                 has: n,
                 get: i
-            } = Fe(r),
+            } = Ke(r),
             o = n.call(r, e);
-        o ? Hr(r, n, e) : (e = _(e), o = n.call(r, e));
+        o ? en(r, n, e) : (e = g(e), o = n.call(r, e));
         let s = i.call(r, e);
-        return r.set(e, t), o ? Et(t, s) && j(r, "set", e, t, s) : j(r, "add", e, t), this
+        return r.set(e, t), o ? Tt(t, s) && z(r, "set", e, t, s) : z(r, "add", e, t), this
     }
 
-    function Ur(e) {
-        let t = _(this),
+    function Gr(e) {
+        let t = g(this),
             {
                 has: r,
                 get: n
-            } = Fe(t),
+            } = Ke(t),
             i = r.call(t, e);
-        i ? Hr(t, r, e) : (e = _(e), i = r.call(t, e));
+        i ? en(t, r, e) : (e = g(e), i = r.call(t, e));
         let o = n ? n.call(t, e) : void 0,
             s = t.delete(e);
-        return i && j(t, "delete", e, void 0, o), s
+        return i && z(t, "delete", e, void 0, o), s
     }
 
-    function Wr() {
-        let e = _(this),
+    function Jr() {
+        let e = g(this),
             t = e.size !== 0,
-            r = X(e) ? new Map(e) : new Set(e),
+            r = re(e) ? new Map(e) : new Set(e),
             n = e.clear();
-        return t && j(e, "clear", void 0, void 0, r), n
+        return t && z(e, "clear", void 0, void 0, r), n
     }
 
-    function Ve(e, t) {
+    function qe(e, t) {
         return function(n, i) {
             let o = this,
                 s = o.__v_raw,
-                a = _(s),
-                c = t ? Mt : e ? Rt : Ct;
-            return !e && T(a, "iterate", U), s.forEach((l, u) => n.call(i, c(l), c(u), o))
+                a = g(s),
+                c = t ? kt : e ? It : Pt;
+            return !e && M(a, "iterate", J), s.forEach((l, u) => n.call(i, c(l), c(u), o))
         }
     }
 
-    function He(e, t, r) {
+    function je(e, t, r) {
         return function(...n) {
             let i = this.__v_raw,
-                o = _(i),
-                s = X(o),
+                o = g(i),
+                s = re(o),
                 a = e === "entries" || e === Symbol.iterator && s,
                 c = e === "keys" && s,
                 l = i[e](...n),
-                u = r ? Mt : t ? Rt : Ct;
-            return !t && T(o, "iterate", c ? At : U), {
+                u = r ? kt : t ? It : Pt;
+            return !t && M(o, "iterate", c ? Rt : J), {
                 next() {
                     let {
-                        value: p,
-                        done: y
+                        value: d,
+                        done: m
                     } = l.next();
-                    return y ? {
-                        value: p,
-                        done: y
+                    return m ? {
+                        value: d,
+                        done: m
                     } : {
-                        value: a ? [u(p[0]), u(p[1])] : u(p),
-                        done: y
+                        value: a ? [u(d[0]), u(d[1])] : u(d),
+                        done: m
                     }
                 },
                 [Symbol.iterator]() {
                     return this
                 }
             }
         }
     }
 
-    function F(e) {
+    function K(e) {
         return function(...t) {
             {
                 let r = t[0] ? `on key "${t[0]}" ` : "";
-                console.warn(`${wt(e)} operation ${r}failed: target is readonly.`, _(this))
+                console.warn(`${Ct(e)} operation ${r}failed: target is readonly.`, g(this))
             }
             return e === "delete" ? !1 : this
         }
     }
-    var Gr = {
+    var Yr = {
             get(e) {
-                return Be(this, e)
+                return ze(this, e)
             },
             get size() {
-                return ze(this)
+                return He(this)
             },
-            has: Ke,
-            add: Vr,
-            set: qr,
-            delete: Ur,
-            clear: Wr,
-            forEach: Ve(!1, !1)
+            has: Ve,
+            add: Ur,
+            set: Wr,
+            delete: Gr,
+            clear: Jr,
+            forEach: qe(!1, !1)
         },
-        Yr = {
+        Zr = {
             get(e) {
-                return Be(this, e, !1, !0)
+                return ze(this, e, !1, !0)
             },
             get size() {
-                return ze(this)
+                return He(this)
             },
-            has: Ke,
-            add: Vr,
-            set: qr,
-            delete: Ur,
-            clear: Wr,
-            forEach: Ve(!1, !0)
+            has: Ve,
+            add: Ur,
+            set: Wr,
+            delete: Gr,
+            clear: Jr,
+            forEach: qe(!1, !0)
         },
-        Jr = {
+        Qr = {
             get(e) {
-                return Be(this, e, !0)
+                return ze(this, e, !0)
             },
             get size() {
-                return ze(this, !0)
+                return He(this, !0)
             },
             has(e) {
-                return Ke.call(this, e, !0)
+                return Ve.call(this, e, !0)
             },
-            add: F("add"),
-            set: F("set"),
-            delete: F("delete"),
-            clear: F("clear"),
-            forEach: Ve(!0, !1)
+            add: K("add"),
+            set: K("set"),
+            delete: K("delete"),
+            clear: K("clear"),
+            forEach: qe(!0, !1)
         },
-        Zr = {
+        Xr = {
             get(e) {
-                return Be(this, e, !0, !0)
+                return ze(this, e, !0, !0)
             },
             get size() {
-                return ze(this, !0)
+                return He(this, !0)
             },
             has(e) {
-                return Ke.call(this, e, !0)
+                return Ve.call(this, e, !0)
             },
-            add: F("add"),
-            set: F("set"),
-            delete: F("delete"),
-            clear: F("clear"),
-            forEach: Ve(!0, !0)
+            add: K("add"),
+            set: K("set"),
+            delete: K("delete"),
+            clear: K("clear"),
+            forEach: qe(!0, !0)
         },
-        ci = ["keys", "values", "entries", Symbol.iterator];
-    ci.forEach(e => {
-        Gr[e] = He(e, !1, !1), Jr[e] = He(e, !0, !1), Yr[e] = He(e, !1, !0), Zr[e] = He(e, !0, !0)
+        di = ["keys", "values", "entries", Symbol.iterator];
+    di.forEach(e => {
+        Yr[e] = je(e, !1, !1), Qr[e] = je(e, !0, !1), Zr[e] = je(e, !1, !0), Xr[e] = je(e, !0, !0)
     });
 
-    function qe(e, t) {
-        let r = t ? e ? Zr : Yr : e ? Jr : Gr;
-        return (n, i, o) => i === "__v_isReactive" ? !e : i === "__v_isReadonly" ? e : i === "__v_raw" ? n : Reflect.get(le(r, i) && i in n ? r : n, i, o)
+    function Ue(e, t) {
+        let r = t ? e ? Xr : Zr : e ? Qr : Yr;
+        return (n, i, o) => i === "__v_isReactive" ? !e : i === "__v_isReadonly" ? e : i === "__v_raw" ? n : Reflect.get(me(r, i) && i in n ? r : n, i, o)
     }
-    var li = {
-            get: qe(!1, !1)
+    var pi = {
+            get: Ue(!1, !1)
         },
-        gs = {
-            get: qe(!1, !0)
+        bs = {
+            get: Ue(!1, !0)
         },
-        ui = {
-            get: qe(!0, !1)
+        mi = {
+            get: Ue(!0, !1)
         },
-        xs = {
-            get: qe(!0, !0)
+        ws = {
+            get: Ue(!0, !0)
         };
 
-    function Hr(e, t, r) {
-        let n = _(r);
+    function en(e, t, r) {
+        let n = g(r);
         if (n !== r && t.call(e, n)) {
-            let i = vt(e);
+            let i = Ot(e);
             console.warn(`Reactive ${i} contains both the raw and reactive versions of the same object${i==="Map"?" as keys":""}, which can lead to inconsistencies. Avoid differentiating between the raw and reactive versions of an object and only use the reactive version if possible.`)
         }
     }
-    var Lr = new WeakMap,
-        ti = new WeakMap,
-        jr = new WeakMap,
-        ri = new WeakMap;
+    var tn = new WeakMap,
+        hi = new WeakMap,
+        rn = new WeakMap,
+        _i = new WeakMap;
 
-    function fi(e) {
+    function gi(e) {
         switch (e) {
             case "Object":
             case "Array":
                 return 1;
             case "Map":
             case "Set":
             case "WeakMap":
             case "WeakSet":
                 return 2;
             default:
                 return 0
         }
     }
 
-    function di(e) {
-        return e.__v_skip || !Object.isExtensible(e) ? 0 : fi(vt(e))
+    function xi(e) {
+        return e.__v_skip || !Object.isExtensible(e) ? 0 : gi(Ot(e))
     }
 
-    function je(e) {
-        return e && e.__v_isReadonly ? e : Qr(e, !1, Kr, li, Lr)
+    function We(e) {
+        return e && e.__v_isReadonly ? e : on(e, !1, Hr, pi, tn)
     }
 
-    function Fr(e) {
-        return Qr(e, !0, zr, ui, jr)
+    function nn(e) {
+        return on(e, !0, qr, mi, rn)
     }
 
-    function Qr(e, t, r, n, i) {
-        if (!ue(e)) return console.warn(`value cannot be made reactive: ${String(e)}`), e;
+    function on(e, t, r, n, i) {
+        if (!he(e)) return console.warn(`value cannot be made reactive: ${String(e)}`), e;
         if (e.__v_raw && !(t && e.__v_isReactive)) return e;
         let o = i.get(e);
         if (o) return o;
-        let s = di(e);
+        let s = xi(e);
         if (s === 0) return e;
         let a = new Proxy(e, s === 2 ? n : r);
         return i.set(e, a), a
     }
 
-    function _(e) {
-        return e && _(e.__v_raw) || e
+    function g(e) {
+        return e && g(e.__v_raw) || e
     }
 
-    function Tt(e) {
+    function Nt(e) {
         return Boolean(e && e.__v_isRef === !0)
     }
-    x("nextTick", () => Te);
-    x("dispatch", e => z.bind(z, e));
-    x("watch", (e, {
+    y("nextTick", () => ee);
+    y("dispatch", e => q.bind(q, e));
+    y("watch", (e, {
         evaluateLater: t,
         effect: r
     }) => (n, i) => {
         let o = t(n),
             s = !0,
             a, c = r(() => o(l => {
                 JSON.stringify(l), s ? a = l : queueMicrotask(() => {
                     i(l, a), a = l
                 }), s = !1
             }));
         e._x_effects.delete(c)
     });
-    x("store", Er);
-    x("data", e => xe(e));
-    x("root", e => V(e));
-    x("refs", e => (e._x_refs_proxy || (e._x_refs_proxy = D(pi(e))), e._x_refs_proxy));
+    y("store", Mr);
+    y("data", e => Ee(e));
+    y("root", e => U(e));
+    y("refs", e => (e._x_refs_proxy || (e._x_refs_proxy = j(yi(e))), e._x_refs_proxy));
 
-    function pi(e) {
+    function yi(e) {
         let t = [],
             r = e;
         for (; r;) r._x_refs && t.push(r._x_refs), r = r.parentNode;
         return t
     }
-    var Nt = {};
+    var Lt = {};
 
-    function Pt(e) {
-        return Nt[e] || (Nt[e] = 0), ++Nt[e]
+    function $t(e) {
+        return Lt[e] || (Lt[e] = 0), ++Lt[e]
     }
 
-    function Xr(e, t) {
-        return Q(e, r => {
+    function sn(e, t) {
+        return X(e, r => {
             if (r._x_ids && r._x_ids[t]) return !0
         })
     }
 
-    function en(e, t) {
-        e._x_ids || (e._x_ids = {}), e._x_ids[t] || (e._x_ids[t] = Pt(t))
+    function an(e, t) {
+        e._x_ids || (e._x_ids = {}), e._x_ids[t] || (e._x_ids[t] = $t(t))
     }
-    x("id", e => (t, r = null) => {
-        let n = Xr(e, t),
-            i = n ? n._x_ids[t] : Pt(t);
+    y("id", e => (t, r = null) => {
+        let n = sn(e, t),
+            i = n ? n._x_ids[t] : $t(t);
         return r ? `${t}-${i}-${r}` : `${t}-${i}`
     });
-    x("el", e => e);
-    tn("Focus", "focus", "focus");
-    tn("Persist", "persist", "persist");
+    y("el", e => e);
+    cn("Focus", "focus", "focus");
+    cn("Persist", "persist", "persist");
+
+    function cn(e, t, r) {
+        y(t, n => T(`You can't use [$${directiveName}] without first installing the "${e}" plugin here: https://alpinejs.dev/plugins/${r}`, n))
+    }
 
-    function tn(e, t, r) {
-        x(t, n => O(`You can't use [$${directiveName}] without first installing the "${e}" plugin here: https://alpinejs.dev/plugins/${r}`, n))
+    function ln({
+        get: e,
+        set: t
+    }, {
+        get: r,
+        set: n
+    }) {
+        let i = !0,
+            o, s, a, c, l = P(() => {
+                let u, d;
+                i ? (u = e(), n(u), d = r(), i = !1) : (u = e(), d = r(), a = JSON.stringify(u), c = JSON.stringify(d), a !== o ? (d = r(), n(u), d = u) : (t(d), u = d)), o = JSON.stringify(u), s = JSON.stringify(d)
+            });
+        return () => {
+            L(l)
+        }
     }
-    d("modelable", (e, {
+    p("modelable", (e, {
         expression: t
     }, {
         effect: r,
-        evaluateLater: n
+        evaluateLater: n,
+        cleanup: i
     }) => {
-        let i = n(t),
-            o = () => {
-                let l;
-                return i(u => l = u), l
+        let o = n(t),
+            s = () => {
+                let u;
+                return o(d => u = d), u
             },
-            s = n(`${t} = __placeholder`),
-            a = l => s(() => {}, {
+            a = n(`${t} = __placeholder`),
+            c = u => a(() => {}, {
                 scope: {
-                    __placeholder: l
+                    __placeholder: u
                 }
             }),
-            c = o();
-        a(c), queueMicrotask(() => {
+            l = s();
+        c(l), queueMicrotask(() => {
             if (!e._x_model) return;
             e._x_removeModelListeners.default();
-            let l = e._x_model.get,
-                u = e._x_model.set;
-            r(() => a(l())), r(() => u(o()))
+            let u = e._x_model.get,
+                d = e._x_model.set,
+                m = ln({
+                    get() {
+                        return u()
+                    },
+                    set(w) {
+                        d(w)
+                    }
+                }, {
+                    get() {
+                        return s()
+                    },
+                    set(w) {
+                        c(w)
+                    }
+                });
+            i(m)
         })
     });
-    d("teleport", (e, {
-        expression: t
+    var bi = document.createElement("div");
+    p("teleport", (e, {
+        modifiers: t,
+        expression: r
     }, {
-        cleanup: r
+        cleanup: n
     }) => {
-        e.tagName.toLowerCase() !== "template" && O("x-teleport can only be used on a <template> tag", e);
-        let n = document.querySelector(t);
-        n || O(`Cannot find x-teleport element for selector: "${t}"`);
-        let i = e.content.cloneNode(!0).firstElementChild;
-        e._x_teleport = i, i._x_teleportBack = e, e._x_forwardEvents && e._x_forwardEvents.forEach(o => {
-            i.addEventListener(o, s => {
-                s.stopPropagation(), e.dispatchEvent(new s.constructor(s.type, s))
+        e.tagName.toLowerCase() !== "template" && T("x-teleport can only be used on a <template> tag", e);
+        let i = N(() => document.querySelector(r), () => bi)();
+        i || T(`Cannot find x-teleport element for selector: "${r}"`);
+        let o = e.content.cloneNode(!0).firstElementChild;
+        e._x_teleport = o, o._x_teleportBack = e, e._x_forwardEvents && e._x_forwardEvents.forEach(s => {
+            o.addEventListener(s, a => {
+                a.stopPropagation(), e.dispatchEvent(new a.constructor(a.type, a))
             })
-        }), C(i, {}, e), m(() => {
-            n.appendChild(i), w(i), i._x_ignore = !0
-        }), r(() => i.remove())
+        }), R(o, {}, e), h(() => {
+            t.includes("prepend") ? i.parentNode.insertBefore(o, i) : t.includes("append") ? i.parentNode.insertBefore(o, i.nextSibling) : i.appendChild(o), v(o), o._x_ignore = !0
+        }), n(() => o.remove())
     });
-    var rn = () => {};
-    rn.inline = (e, {
+    var un = () => {};
+    un.inline = (e, {
         modifiers: t
     }, {
         cleanup: r
     }) => {
         t.includes("self") ? e._x_ignoreSelf = !0 : e._x_ignore = !0, r(() => {
             t.includes("self") ? delete e._x_ignoreSelf : delete e._x_ignore
         })
     };
-    d("ignore", rn);
-    d("effect", (e, {
+    p("ignore", un);
+    p("effect", (e, {
         expression: t
     }, {
         effect: r
-    }) => r(g(e, t)));
+    }) => r(x(e, t)));
 
-    function de(e, t, r, n) {
+    function ie(e, t, r, n) {
         let i = e,
             o = c => n(c),
             s = {},
             a = (c, l) => u => l(c, u);
-        if (r.includes("dot") && (t = mi(t)), r.includes("camel") && (t = hi(t)), r.includes("passive") && (s.passive = !0), r.includes("capture") && (s.capture = !0), r.includes("window") && (i = window), r.includes("document") && (i = document), r.includes("prevent") && (o = a(o, (c, l) => {
+        if (r.includes("dot") && (t = wi(t)), r.includes("camel") && (t = Ei(t)), r.includes("passive") && (s.passive = !0), r.includes("capture") && (s.capture = !0), r.includes("window") && (i = window), r.includes("document") && (i = document), r.includes("prevent") && (o = a(o, (c, l) => {
                 l.preventDefault(), c(l)
             })), r.includes("stop") && (o = a(o, (c, l) => {
                 l.stopPropagation(), c(l)
             })), r.includes("self") && (o = a(o, (c, l) => {
                 l.target === e && c(l)
             })), (r.includes("away") || r.includes("outside")) && (i = document, o = a(o, (c, l) => {
                 e.contains(l.target) || l.target.isConnected !== !1 && (e.offsetWidth < 1 && e.offsetHeight < 1 || e._x_isShown !== !1 && c(l))
             })), r.includes("once") && (o = a(o, (c, l) => {
                 c(l), i.removeEventListener(t, o, s)
             })), o = a(o, (c, l) => {
-                _i(t) && gi(l, r) || c(l)
+                Si(t) && Ai(l, r) || c(l)
             }), r.includes("debounce")) {
             let c = r[r.indexOf("debounce") + 1] || "invalid-wait",
-                l = kt(c.split("ms")[0]) ? Number(c.split("ms")[0]) : 250;
-            o = Ne(o, l)
+                l = Ge(c.split("ms")[0]) ? Number(c.split("ms")[0]) : 250;
+            o = Pe(o, l)
         }
         if (r.includes("throttle")) {
             let c = r[r.indexOf("throttle") + 1] || "invalid-wait",
-                l = kt(c.split("ms")[0]) ? Number(c.split("ms")[0]) : 250;
-            o = Pe(o, l)
+                l = Ge(c.split("ms")[0]) ? Number(c.split("ms")[0]) : 250;
+            o = Ie(o, l)
         }
         return i.addEventListener(t, o, s), () => {
             i.removeEventListener(t, o, s)
         }
     }
 
-    function mi(e) {
+    function wi(e) {
         return e.replace(/-/g, ".")
     }
 
-    function hi(e) {
+    function Ei(e) {
         return e.toLowerCase().replace(/-(\w)/g, (t, r) => r.toUpperCase())
     }
 
-    function kt(e) {
+    function Ge(e) {
         return !Array.isArray(e) && !isNaN(e)
     }
 
-    function xi(e) {
-        return e.replace(/([a-z])([A-Z])/g, "$1-$2").replace(/[_\s]/, "-").toLowerCase()
+    function vi(e) {
+        return [" ", "_"].includes(e) ? e : e.replace(/([a-z])([A-Z])/g, "$1-$2").replace(/[_\s]/, "-").toLowerCase()
     }
 
-    function _i(e) {
+    function Si(e) {
         return ["keydown", "keyup"].includes(e)
     }
 
-    function gi(e, t) {
-        let r = t.filter(o => !["window", "document", "prevent", "stop", "once"].includes(o));
+    function Ai(e, t) {
+        let r = t.filter(o => !["window", "document", "prevent", "stop", "once", "capture"].includes(o));
         if (r.includes("debounce")) {
             let o = r.indexOf("debounce");
-            r.splice(o, kt((r[o + 1] || "invalid-wait").split("ms")[0]) ? 2 : 1)
+            r.splice(o, Ge((r[o + 1] || "invalid-wait").split("ms")[0]) ? 2 : 1)
         }
-        if (r.length === 0 || r.length === 1 && nn(e.key).includes(r[0])) return !1;
+        if (r.includes("throttle")) {
+            let o = r.indexOf("throttle");
+            r.splice(o, Ge((r[o + 1] || "invalid-wait").split("ms")[0]) ? 2 : 1)
+        }
+        if (r.length === 0 || r.length === 1 && fn(e.key).includes(r[0])) return !1;
         let i = ["ctrl", "shift", "alt", "meta", "cmd", "super"].filter(o => r.includes(o));
-        return r = r.filter(o => !i.includes(o)), !(i.length > 0 && i.filter(s => ((s === "cmd" || s === "super") && (s = "meta"), e[`${s}Key`])).length === i.length && nn(e.key).includes(r[0]))
+        return r = r.filter(o => !i.includes(o)), !(i.length > 0 && i.filter(s => ((s === "cmd" || s === "super") && (s = "meta"), e[`${s}Key`])).length === i.length && fn(e.key).includes(r[0]))
     }
 
-    function nn(e) {
+    function fn(e) {
         if (!e) return [];
-        e = xi(e);
+        e = vi(e);
         let t = {
             ctrl: "control",
             slash: "/",
-            space: "-",
-            spacebar: "-",
+            space: " ",
+            spacebar: " ",
             cmd: "meta",
             esc: "escape",
             up: "arrow-up",
             down: "arrow-down",
             left: "arrow-left",
             right: "arrow-right",
             period: ".",
-            equal: "="
+            equal: "=",
+            minus: "-",
+            underscore: "_"
         };
         return t[e] = e, Object.keys(t).map(r => {
             if (t[r] === e) return r
         }).filter(r => r)
     }
-    d("model", (e, {
+    p("model", (e, {
         modifiers: t,
         expression: r
     }, {
         effect: n,
         cleanup: i
     }) => {
-        let o = g(e, r),
-            s = `${r} = rightSideOfExpression($event, ${r})`,
-            a = g(e, s);
-        var c = e.tagName.toLowerCase() === "select" || ["checkbox", "radio"].includes(e.type) || t.includes("lazy") ? "change" : "input";
-        let l = yi(e, t, r),
-            u = de(e, c, t, y => {
-                a(() => {}, {
+        let o = e;
+        t.includes("parent") && (o = e.parentNode);
+        let s = x(o, r),
+            a;
+        typeof r == "string" ? a = x(o, `${r} = __placeholder`) : typeof r == "function" && typeof r() == "string" ? a = x(o, `${r()} = __placeholder`) : a = () => {};
+        let c = () => {
+                let m;
+                return s(w => m = w), dn(m) ? m.get() : m
+            },
+            l = m => {
+                let w;
+                s(k => w = k), dn(w) ? w.set(m) : a(() => {}, {
                     scope: {
-                        $event: y,
-                        rightSideOfExpression: l
+                        __placeholder: m
                     }
                 })
+            };
+        t.includes("fill") && e.hasAttribute("value") && (c() === null || c() === "") && l(e.value), typeof r == "string" && e.type === "radio" && h(() => {
+            e.hasAttribute("name") || e.setAttribute("name", r)
+        });
+        var u = e.tagName.toLowerCase() === "select" || ["checkbox", "radio"].includes(e.type) || t.includes("lazy") ? "change" : "input";
+        let d = te ? () => {} : ie(e, u, t, m => {
+            l(Oi(e, t, m, c()))
+        });
+        if (e._x_removeModelListeners || (e._x_removeModelListeners = {}), e._x_removeModelListeners.default = d, i(() => e._x_removeModelListeners.default()), e.form) {
+            let m = ie(e.form, "reset", [], w => {
+                ee(() => e._x_model && e._x_model.set(e.value))
             });
-        e._x_removeModelListeners || (e._x_removeModelListeners = {}), e._x_removeModelListeners.default = u, i(() => e._x_removeModelListeners.default());
-        let p = g(e, `${r} = __placeholder`);
+            i(() => m())
+        }
         e._x_model = {
             get() {
-                let y;
-                return o(N => y = N), y
+                return c()
             },
-            set(y) {
-                p(() => {}, {
-                    scope: {
-                        __placeholder: y
-                    }
-                })
+            set(m) {
+                l(m)
             }
-        }, e._x_forceModelUpdate = () => {
-            o(y => {
-                y === void 0 && r.match(/\./) && (y = ""), window.fromModel = !0, m(() => ce(e, "value", y)), delete window.fromModel
-            })
+        }, e._x_forceModelUpdate = m => {
+            m = m === void 0 ? c() : m, m === void 0 && typeof r == "string" && r.match(/\./) && (m = ""), window.fromModel = !0, h(() => pe(e, "value", m)), delete window.fromModel
         }, n(() => {
-            t.includes("unintrusive") && document.activeElement.isSameNode(e) || e._x_forceModelUpdate()
+            let m = c();
+            t.includes("unintrusive") && document.activeElement.isSameNode(e) || e._x_forceModelUpdate(m)
         })
     });
 
-    function yi(e, t, r) {
-        return e.type === "radio" && m(() => {
-            e.hasAttribute("name") || e.setAttribute("name", r)
-        }), (n, i) => m(() => {
-            if (n instanceof CustomEvent && n.detail !== void 0) return n.detail || n.target.value;
+    function Oi(e, t, r, n) {
+        return h(() => {
+            if (r instanceof CustomEvent && r.detail !== void 0) return typeof r.detail < "u" ? r.detail : r.target.value;
             if (e.type === "checkbox")
-                if (Array.isArray(i)) {
-                    let o = t.includes("number") ? Dt(n.target.value) : n.target.value;
-                    return n.target.checked ? i.concat([o]) : i.filter(s => !bi(s, o))
-                } else return n.target.checked;
+                if (Array.isArray(n)) {
+                    let i = t.includes("number") ? jt(r.target.value) : r.target.value;
+                    return r.target.checked ? n.concat([i]) : n.filter(o => !Ci(o, i))
+                } else return r.target.checked;
             else {
-                if (e.tagName.toLowerCase() === "select" && e.multiple) return t.includes("number") ? Array.from(n.target.selectedOptions).map(o => {
-                    let s = o.value || o.text;
-                    return Dt(s)
-                }) : Array.from(n.target.selectedOptions).map(o => o.value || o.text); {
-                    let o = n.target.value;
-                    return t.includes("number") ? Dt(o) : t.includes("trim") ? o.trim() : o
+                if (e.tagName.toLowerCase() === "select" && e.multiple) return t.includes("number") ? Array.from(r.target.selectedOptions).map(i => {
+                    let o = i.value || i.text;
+                    return jt(o)
+                }) : Array.from(r.target.selectedOptions).map(i => i.value || i.text); {
+                    let i = r.target.value;
+                    return t.includes("number") ? jt(i) : t.includes("trim") ? i.trim() : i
                 }
             }
         })
     }
 
-    function Dt(e) {
+    function jt(e) {
         let t = e ? parseFloat(e) : null;
-        return vi(t) ? t : e
+        return Ti(t) ? t : e
     }
 
-    function bi(e, t) {
+    function Ci(e, t) {
         return e == t
     }
 
-    function vi(e) {
+    function Ti(e) {
         return !Array.isArray(e) && !isNaN(e)
     }
-    d("cloak", e => queueMicrotask(() => m(() => e.removeAttribute(E("cloak")))));
-    Re(() => `[${E("init")}]`);
-    d("init", $((e, {
+
+    function dn(e) {
+        return e !== null && typeof e == "object" && typeof e.get == "function" && typeof e.set == "function"
+    }
+    p("cloak", e => queueMicrotask(() => h(() => e.removeAttribute(S("cloak")))));
+    Re(() => `[${S("init")}]`);
+    p("init", N((e, {
         expression: t
     }, {
         evaluate: r
     }) => typeof t == "string" ? !!t.trim() && r(t, {}, !1) : r(t, {}, !1)));
-    d("text", (e, {
+    p("text", (e, {
         expression: t
     }, {
         effect: r,
         evaluateLater: n
     }) => {
         let i = n(t);
         r(() => {
             i(o => {
-                m(() => {
+                h(() => {
                     e.textContent = o
                 })
             })
         })
     });
-    d("html", (e, {
+    p("html", (e, {
         expression: t
     }, {
         effect: r,
         evaluateLater: n
     }) => {
         let i = n(t);
         r(() => {
             i(o => {
-                m(() => {
-                    e.innerHTML = o, e._x_ignoreSelf = !0, w(e), delete e._x_ignoreSelf
+                h(() => {
+                    e.innerHTML = o, e._x_ignoreSelf = !0, v(e), delete e._x_ignoreSelf
                 })
             })
         })
     });
-    Z(Ee(":", Se(E("bind:"))));
-    d("bind", (e, {
+    Q(Ce(":", Te(S("bind:"))));
+    p("bind", (e, {
         value: t,
         modifiers: r,
         expression: n,
         original: i
     }, {
         effect: o
     }) => {
         if (!t) {
             let a = {};
-            Or(a), g(e, n)(l => {
-                xt(e, l, i)
+            Dr(a), x(e, n)(l => {
+                vt(e, l, i)
             }, {
                 scope: a
             });
             return
         }
-        if (t === "key") return wi(e, n);
-        let s = g(e, n);
+        if (t === "key") return Mi(e, n);
+        let s = x(e, n);
         o(() => s(a => {
-            a === void 0 && typeof n == "string" && n.match(/\./) && (a = ""), m(() => ce(e, t, a, r))
+            a === void 0 && typeof n == "string" && n.match(/\./) && (a = ""), h(() => pe(e, t, a, r))
         }))
     });
 
-    function wi(e, t) {
+    function Mi(e, t) {
         e._x_keyExpression = t
     }
-    Ce(() => `[${E("data")}]`);
-    d("data", $((e, {
+    Me(() => `[${S("data")}]`);
+    p("data", N((e, {
         expression: t
     }, {
         cleanup: r
     }) => {
         t = t === "" ? "{}" : t;
         let n = {};
-        re(n, e);
+        ae(n, e);
         let i = {};
-        Rr(i, n);
-        let o = P(e, t, {
+        kr(i, n);
+        let o = I(e, t, {
             scope: i
         });
-        o === void 0 && (o = {}), re(o, e);
-        let s = A(o);
-        ye(s);
-        let a = C(e, s);
-        s.init && P(e, s.init), r(() => {
-            s.destroy && P(e, s.destroy), a()
+        (o === void 0 || o === !0) && (o = {}), ae(o, e);
+        let s = C(o);
+        ve(s);
+        let a = R(e, s);
+        s.init && I(e, s.init), r(() => {
+            s.destroy && I(e, s.destroy), a()
         })
     }));
-    d("show", (e, {
+    p("show", (e, {
         modifiers: t,
         expression: r
     }, {
         effect: n
     }) => {
-        let i = g(e, r);
+        let i = x(e, r);
         e._x_doHide || (e._x_doHide = () => {
-            m(() => {
+            h(() => {
                 e.style.setProperty("display", "none", t.includes("important") ? "important" : void 0)
             })
         }), e._x_doShow || (e._x_doShow = () => {
-            m(() => {
+            h(() => {
                 e.style.length === 1 && e.style.display === "none" ? e.removeAttribute("style") : e.style.removeProperty("display")
             })
         });
         let o = () => {
                 e._x_doHide(), e._x_isShown = !1
             },
             s = () => {
                 e._x_doShow(), e._x_isShown = !0
             },
             a = () => setTimeout(s),
-            c = se(p => p ? s() : o(), p => {
-                typeof e._x_toggleAndCascadeWithTransitions == "function" ? e._x_toggleAndCascadeWithTransitions(e, p, s, o) : p ? a() : o()
+            c = fe(d => d ? s() : o(), d => {
+                typeof e._x_toggleAndCascadeWithTransitions == "function" ? e._x_toggleAndCascadeWithTransitions(e, d, s, o) : d ? a() : o()
             }),
             l, u = !0;
-        n(() => i(p => {
-            !u && p === l || (t.includes("immediate") && (p ? a() : o()), c(p), l = p, u = !1)
+        n(() => i(d => {
+            !u && d === l || (t.includes("immediate") && (d ? a() : o()), c(d), l = d, u = !1)
         }))
     });
-    d("for", (e, {
+    p("for", (e, {
         expression: t
     }, {
         effect: r,
         cleanup: n
     }) => {
-        let i = Si(t),
-            o = g(e, i.items),
-            s = g(e, e._x_keyExpression || "index");
-        e._x_prevKeys = [], e._x_lookup = {}, r(() => Ei(e, i, o, s)), n(() => {
+        let i = Ni(t),
+            o = x(e, i.items),
+            s = x(e, e._x_keyExpression || "index");
+        e._x_prevKeys = [], e._x_lookup = {}, r(() => Ri(e, i, o, s)), n(() => {
             Object.values(e._x_lookup).forEach(a => a.remove()), delete e._x_prevKeys, delete e._x_lookup
         })
     });
 
-    function Ei(e, t, r, n) {
+    function Ri(e, t, r, n) {
         let i = s => typeof s == "object" && !Array.isArray(s),
             o = e;
         r(s => {
-            Ai(s) && s >= 0 && (s = Array.from(Array(s).keys(), f => f + 1)), s === void 0 && (s = []);
+            Di(s) && s >= 0 && (s = Array.from(Array(s).keys(), f => f + 1)), s === void 0 && (s = []);
             let a = e._x_lookup,
                 c = e._x_prevKeys,
                 l = [],
                 u = [];
-            if (i(s)) s = Object.entries(s).map(([f, h]) => {
-                let b = on(t, h, f, s);
-                n(v => u.push(v), {
+            if (i(s)) s = Object.entries(s).map(([f, _]) => {
+                let b = pn(t, _, f, s);
+                n(E => u.push(E), {
                     scope: {
                         index: f,
                         ...b
                     }
                 }), l.push(b)
             });
             else
                 for (let f = 0; f < s.length; f++) {
-                    let h = on(t, s[f], f, s);
+                    let _ = pn(t, s[f], f, s);
                     n(b => u.push(b), {
                         scope: {
                             index: f,
-                            ...h
+                            ..._
                         }
-                    }), l.push(h)
+                    }), l.push(_)
                 }
-            let p = [],
-                y = [],
-                N = [],
-                W = [];
+            let d = [],
+                m = [],
+                w = [],
+                k = [];
             for (let f = 0; f < c.length; f++) {
-                let h = c[f];
-                u.indexOf(h) === -1 && N.push(h)
+                let _ = c[f];
+                u.indexOf(_) === -1 && w.push(_)
             }
-            c = c.filter(f => !N.includes(f));
-            let pe = "template";
+            c = c.filter(f => !w.includes(f));
+            let ge = "template";
             for (let f = 0; f < u.length; f++) {
-                let h = u[f],
-                    b = c.indexOf(h);
-                if (b === -1) c.splice(f, 0, h), p.push([pe, f]);
+                let _ = u[f],
+                    b = c.indexOf(_);
+                if (b === -1) c.splice(f, 0, _), d.push([ge, f]);
                 else if (b !== f) {
-                    let v = c.splice(f, 1)[0],
-                        S = c.splice(b - 1, 1)[0];
-                    c.splice(f, 0, S), c.splice(b, 0, v), y.push([v, S])
-                } else W.push(h);
-                pe = h
-            }
-            for (let f = 0; f < N.length; f++) {
-                let h = N[f];
-                a[h]._x_effects && a[h]._x_effects.forEach(he), a[h].remove(), a[h] = null, delete a[h]
-            }
-            for (let f = 0; f < y.length; f++) {
-                let [h, b] = y[f], v = a[h], S = a[b], G = document.createElement("div");
-                m(() => {
-                    S.after(G), v.after(S), S._x_currentIfEl && S.after(S._x_currentIfEl), G.before(v), v._x_currentIfEl && v.after(v._x_currentIfEl), G.remove()
-                }), ot(S, l[u.indexOf(b)])
-            }
-            for (let f = 0; f < p.length; f++) {
-                let [h, b] = p[f], v = h === "template" ? o : a[h];
-                v._x_currentIfEl && (v = v._x_currentIfEl);
-                let S = l[b],
-                    G = u[b],
-                    me = document.importNode(o.content, !0).firstElementChild;
-                C(me, A(S), o), m(() => {
-                    v.after(me), w(me)
-                }), typeof G == "object" && O("x-for key cannot be an object, it must be a string or an integer", o), a[G] = me
+                    let E = c.splice(f, 1)[0],
+                        O = c.splice(b - 1, 1)[0];
+                    c.splice(f, 0, O), c.splice(b, 0, E), m.push([E, O])
+                } else k.push(_);
+                ge = _
+            }
+            for (let f = 0; f < w.length; f++) {
+                let _ = w[f];
+                a[_]._x_effects && a[_]._x_effects.forEach(ye), a[_].remove(), a[_] = null, delete a[_]
             }
-            for (let f = 0; f < W.length; f++) ot(a[W[f]], l[u.indexOf(W[f])]);
+            for (let f = 0; f < m.length; f++) {
+                let [_, b] = m[f], E = a[_], O = a[b], Y = document.createElement("div");
+                h(() => {
+                    O.after(Y), E.after(O), O._x_currentIfEl && O.after(O._x_currentIfEl), Y.before(E), E._x_currentIfEl && E.after(E._x_currentIfEl), Y.remove()
+                }), lt(O, l[u.indexOf(b)])
+            }
+            for (let f = 0; f < d.length; f++) {
+                let [_, b] = d[f], E = _ === "template" ? o : a[_];
+                E._x_currentIfEl && (E = E._x_currentIfEl);
+                let O = l[b],
+                    Y = u[b],
+                    xe = document.importNode(o.content, !0).firstElementChild;
+                R(xe, C(O), o), h(() => {
+                    E.after(xe), v(xe)
+                }), typeof Y == "object" && T("x-for key cannot be an object, it must be a string or an integer", o), a[Y] = xe
+            }
+            for (let f = 0; f < k.length; f++) lt(a[k[f]], l[u.indexOf(k[f])]);
             o._x_prevKeys = u
         })
     }
 
-    function Si(e) {
+    function Ni(e) {
         let t = /,([^,\}\]]*)(?:,([^,\}\]]*))?$/,
             r = /^\s*\(|\)\s*$/g,
             n = /([\s\S]*?)\s+(?:in|of)\s+([\s\S]*)/,
             i = e.match(n);
         if (!i) return;
         let o = {};
         o.items = i[2].trim();
         let s = i[1].replace(r, "").trim(),
             a = s.match(t);
         return a ? (o.item = s.replace(t, "").trim(), o.index = a[1].trim(), a[2] && (o.collection = a[2].trim())) : o.item = s, o
     }
 
-    function on(e, t, r, n) {
+    function pn(e, t, r, n) {
         let i = {};
         return /^\[.*\]$/.test(e.item) && Array.isArray(t) ? e.item.replace("[", "").replace("]", "").split(",").map(s => s.trim()).forEach((s, a) => {
             i[s] = t[a]
         }) : /^\{.*\}$/.test(e.item) && !Array.isArray(t) && typeof t == "object" ? e.item.replace("{", "").replace("}", "").split(",").map(s => s.trim()).forEach(s => {
             i[s] = t[s]
         }) : i[e.item] = t, e.index && (i[e.index] = r), e.collection && (i[e.collection] = n), i
     }
 
-    function Ai(e) {
+    function Di(e) {
         return !Array.isArray(e) && !isNaN(e)
     }
 
-    function sn() {}
-    sn.inline = (e, {
+    function mn() {}
+    mn.inline = (e, {
         expression: t
     }, {
         cleanup: r
     }) => {
-        let n = V(e);
+        let n = U(e);
         n._x_refs || (n._x_refs = {}), n._x_refs[t] = e, r(() => delete n._x_refs[t])
     };
-    d("ref", sn);
-    d("if", (e, {
+    p("ref", mn);
+    p("if", (e, {
         expression: t
     }, {
         effect: r,
         cleanup: n
     }) => {
-        let i = g(e, t),
+        let i = x(e, t),
             o = () => {
                 if (e._x_currentIfEl) return e._x_currentIfEl;
                 let a = e.content.cloneNode(!0).firstElementChild;
-                return C(a, {}, e), m(() => {
-                    e.after(a), w(a)
+                return R(a, {}, e), h(() => {
+                    e.after(a), v(a)
                 }), e._x_currentIfEl = a, e._x_undoIf = () => {
-                    R(a, c => {
-                        c._x_effects && c._x_effects.forEach(he)
+                    A(a, c => {
+                        c._x_effects && c._x_effects.forEach(ye)
                     }), a.remove(), delete e._x_currentIfEl
                 }, a
             },
             s = () => {
-                !e._x_undoIf || (e._x_undoIf(), delete e._x_undoIf)
+                e._x_undoIf && (e._x_undoIf(), delete e._x_undoIf)
             };
         r(() => i(a => {
             a ? o() : s()
         })), n(() => e._x_undoIf && e._x_undoIf())
     });
-    d("id", (e, {
+    p("id", (e, {
         expression: t
     }, {
         evaluate: r
     }) => {
-        r(t).forEach(i => en(e, i))
+        r(t).forEach(i => an(e, i))
     });
-    Z(Ee("@", Se(E("on:"))));
-    d("on", $((e, {
+    Q(Ce("@", Te(S("on:"))));
+    p("on", N((e, {
         value: t,
         modifiers: r,
         expression: n
     }, {
         cleanup: i
     }) => {
-        let o = n ? g(e, n) : () => {};
+        let o = n ? x(e, n) : () => {};
         e.tagName.toLowerCase() === "template" && (e._x_forwardEvents || (e._x_forwardEvents = []), e._x_forwardEvents.includes(t) || e._x_forwardEvents.push(t));
-        let s = de(e, t, r, a => {
+        let s = ie(e, t, r, a => {
             o(() => {}, {
                 scope: {
                     $event: a
                 },
                 params: [a]
             })
         });
         i(() => s())
     }));
-    Ue("Collapse", "collapse", "collapse");
-    Ue("Intersect", "intersect", "intersect");
-    Ue("Focus", "trap", "focus");
-    Ue("Mask", "mask", "mask");
-
-    function Ue(e, t, r) {
-        d(t, n => O(`You can't use [x-${t}] without first installing the "${e}" plugin here: https://alpinejs.dev/plugins/${r}`, n))
-    }
-    I.setEvaluator(ct);
-    I.setReactivityEngine({
-        reactive: je,
-        effect: Pr,
-        release: Dr,
-        raw: _
+    Je("Collapse", "collapse", "collapse");
+    Je("Intersect", "intersect", "intersect");
+    Je("Focus", "trap", "focus");
+    Je("Mask", "mask", "mask");
+
+    function Je(e, t, r) {
+        p(t, n => T(`You can't use [x-${t}] without first installing the "${e}" plugin here: https://alpinejs.dev/plugins/${r}`, n))
+    }
+    F.setEvaluator(pt);
+    F.setReactivityEngine({
+        reactive: We,
+        effect: jr,
+        release: Fr,
+        raw: g
     });
-    var It = I;
-    window.Alpine = It;
+    var Ft = F;
+    window.Alpine = Ft;
     queueMicrotask(() => {
-        It.start()
+        Ft.start()
     });
 })();
```

### Comparing `django_unfold-0.5.3/src/unfold/static/unfold/js/app.js` & `django_unfold-0.6.0/src/unfold/static/unfold/js/app.js`

 * *Files identical despite different names*

### Comparing `django_unfold-0.5.3/src/unfold/static/unfold/js/htmx.js` & `django_unfold-0.6.0/src/unfold/static/unfold/js/htmx.js`

 * *Files 9% similar despite different names*

#### js-beautify {}

```diff
@@ -1,38 +1,40 @@
 (function(e, t) {
     if (typeof define === "function" && define.amd) {
         define([], t)
+    } else if (typeof module === "object" && module.exports) {
+        module.exports = t()
     } else {
         e.htmx = e.htmx || t()
     }
 })(typeof self !== "undefined" ? self : this, function() {
     return function() {
         "use strict";
-        var U = {
+        var z = {
             onLoad: t,
-            process: mt,
-            on: X,
-            off: F,
-            trigger: $,
-            ajax: or,
-            find: R,
-            findAll: O,
-            closest: N,
+            process: Tt,
+            on: le,
+            off: ue,
+            trigger: ie,
+            ajax: dr,
+            find: b,
+            findAll: f,
+            closest: d,
             values: function(e, t) {
-                var r = jt(e, t || "post");
+                var r = Jt(e, t || "post");
                 return r.values
             },
-            remove: q,
-            addClass: L,
-            removeClass: T,
-            toggleClass: H,
-            takeClass: A,
-            defineExtension: dr,
-            removeExtension: vr,
-            logAll: C,
+            remove: B,
+            addClass: j,
+            removeClass: n,
+            toggleClass: U,
+            takeClass: V,
+            defineExtension: yr,
+            removeExtension: br,
+            logAll: F,
             logger: null,
             config: {
                 historyEnabled: true,
                 historyCacheSize: 10,
                 refreshOnHistoryMiss: false,
                 defaultSwapStyle: "innerHTML",
                 defaultSwapDelay: 0,
@@ -45,59 +47,64 @@
                 swappingClass: "htmx-swapping",
                 allowEval: true,
                 inlineScriptNonce: "",
                 attributesToSettle: ["class", "style", "width", "height"],
                 withCredentials: false,
                 timeout: 0,
                 wsReconnectDelay: "full-jitter",
+                wsBinaryType: "blob",
                 disableSelector: "[hx-disable], [data-hx-disable]",
                 useTemplateFragments: false,
                 scrollBehavior: "smooth",
-                defaultFocusScroll: false
+                defaultFocusScroll: false,
+                getCacheBusterParam: false,
+                globalViewTransitions: false
             },
             parseInterval: v,
             _: e,
             createEventSource: function(e) {
                 return new EventSource(e, {
                     withCredentials: true
                 })
             },
             createWebSocket: function(e) {
-                return new WebSocket(e, [])
+                var t = new WebSocket(e, []);
+                t.binaryType = z.config.wsBinaryType;
+                return t
             },
-            version: "1.8.2"
+            version: "1.9.2"
         };
-        var r = {
-            addTriggerHandler: ft,
-            bodyContains: K,
-            canAccessLocalStorage: E,
-            filterValues: zt,
-            hasAttribute: o,
-            getAttributeValue: V,
-            getClosestMatch: h,
-            getExpressionVars: rr,
-            getHeaders: _t,
-            getInputValues: jt,
-            getInternalData: W,
-            getSwapSpecification: Gt,
-            getTriggerSpecs: Xe,
-            getTarget: re,
-            makeFragment: g,
-            mergeObjects: Y,
-            makeSettleInfo: Zt,
-            oobSwap: ae,
-            selectAndSwap: Oe,
-            settleImmediately: At,
-            shouldCancel: Ve,
-            triggerEvent: $,
-            triggerErrorEvent: J,
-            withExtensions: wt
+        var C = {
+            addTriggerHandler: xt,
+            bodyContains: ee,
+            canAccessLocalStorage: D,
+            filterValues: er,
+            hasAttribute: q,
+            getAttributeValue: G,
+            getClosestMatch: c,
+            getExpressionVars: fr,
+            getHeaders: Qt,
+            getInputValues: Jt,
+            getInternalData: Y,
+            getSwapSpecification: rr,
+            getTriggerSpecs: ze,
+            getTarget: de,
+            makeFragment: l,
+            mergeObjects: te,
+            makeSettleInfo: S,
+            oobSwap: me,
+            selectAndSwap: Me,
+            settleImmediately: Bt,
+            shouldCancel: Ke,
+            triggerEvent: ie,
+            triggerErrorEvent: ne,
+            withExtensions: w
         };
-        var n = ["get", "post", "put", "delete", "patch"];
-        var i = n.map(function(e) {
+        var R = ["get", "post", "put", "delete", "patch"];
+        var O = R.map(function(e) {
             return "[hx-" + e + "], [data-hx-" + e + "]"
         }).join(", ");
 
         function v(e) {
             if (e == undefined) {
                 return undefined
             }
@@ -109,827 +116,873 @@
             }
             if (e.slice(-1) == "m") {
                 return parseFloat(e.slice(0, -1)) * 1e3 * 60 || undefined
             }
             return parseFloat(e) || undefined
         }
 
-        function f(e, t) {
+        function $(e, t) {
             return e.getAttribute && e.getAttribute(t)
         }
 
-        function o(e, t) {
+        function q(e, t) {
             return e.hasAttribute && (e.hasAttribute(t) || e.hasAttribute("data-" + t))
         }
 
-        function V(e, t) {
-            return f(e, t) || f(e, "data-" + t)
+        function G(e, t) {
+            return $(e, t) || $(e, "data-" + t)
         }
 
         function u(e) {
             return e.parentElement
         }
 
-        function _() {
+        function J() {
             return document
         }
 
-        function h(e, t) {
+        function c(e, t) {
             while (e && !t(e)) {
                 e = u(e)
             }
             return e ? e : null
         }
 
-        function a(e, t, r) {
-            var n = V(t, r);
-            var i = V(t, "hx-disinherit");
+        function T(e, t, r) {
+            var n = G(t, r);
+            var i = G(t, "hx-disinherit");
             if (e !== t && i && (i === "*" || i.split(" ").indexOf(r) >= 0)) {
                 return "unset"
             } else {
                 return n
             }
         }
 
-        function z(t, r) {
+        function Z(t, r) {
             var n = null;
-            h(t, function(e) {
-                return n = a(t, e, r)
+            c(t, function(e) {
+                return n = T(t, e, r)
             });
             if (n !== "unset") {
                 return n
             }
         }
 
-        function d(e, t) {
+        function h(e, t) {
             var r = e.matches || e.matchesSelector || e.msMatchesSelector || e.mozMatchesSelector || e.webkitMatchesSelector || e.oMatchesSelector;
             return r && r.call(e, t)
         }
 
-        function s(e) {
+        function H(e) {
             var t = /<([a-z][^\/\0>\x20\t\r\n\f]*)/i;
             var r = t.exec(e);
             if (r) {
                 return r[1].toLowerCase()
             } else {
                 return ""
             }
         }
 
-        function l(e, t) {
+        function i(e, t) {
             var r = new DOMParser;
             var n = r.parseFromString(e, "text/html");
             var i = n.body;
             while (t > 0) {
                 t--;
                 i = i.firstChild
             }
             if (i == null) {
-                i = _().createDocumentFragment()
+                i = J().createDocumentFragment()
             }
             return i
         }
 
-        function g(e) {
-            if (U.config.useTemplateFragments) {
-                var t = l("<body><template>" + e + "</template></body>", 0);
-                return t.querySelector("template").content
+        function L(e) {
+            return e.match(/<body/)
+        }
+
+        function l(e) {
+            var t = !L(e);
+            if (z.config.useTemplateFragments && t) {
+                var r = i("<body><template>" + e + "</template></body>", 0);
+                return r.querySelector("template").content
             } else {
-                var r = s(e);
-                switch (r) {
+                var n = H(e);
+                switch (n) {
                     case "thead":
                     case "tbody":
                     case "tfoot":
                     case "colgroup":
                     case "caption":
-                        return l("<table>" + e + "</table>", 1);
+                        return i("<table>" + e + "</table>", 1);
                     case "col":
-                        return l("<table><colgroup>" + e + "</colgroup></table>", 2);
+                        return i("<table><colgroup>" + e + "</colgroup></table>", 2);
                     case "tr":
-                        return l("<table><tbody>" + e + "</tbody></table>", 2);
+                        return i("<table><tbody>" + e + "</tbody></table>", 2);
                     case "td":
                     case "th":
-                        return l("<table><tbody><tr>" + e + "</tr></tbody></table>", 3);
+                        return i("<table><tbody><tr>" + e + "</tr></tbody></table>", 3);
                     case "script":
-                        return l("<div>" + e + "</div>", 1);
+                        return i("<div>" + e + "</div>", 1);
                     default:
-                        return l(e, 0)
+                        return i(e, 0)
                 }
             }
         }
 
-        function Z(e) {
+        function K(e) {
             if (e) {
                 e()
             }
         }
 
-        function p(e, t) {
+        function A(e, t) {
             return Object.prototype.toString.call(e) === "[object " + t + "]"
         }
 
-        function m(e) {
-            return p(e, "Function")
+        function N(e) {
+            return A(e, "Function")
         }
 
-        function x(e) {
-            return p(e, "Object")
+        function I(e) {
+            return A(e, "Object")
         }
 
-        function W(e) {
+        function Y(e) {
             var t = "htmx-internal-data";
             var r = e[t];
             if (!r) {
                 r = e[t] = {}
             }
             return r
         }
 
-        function y(e) {
+        function k(e) {
             var t = [];
             if (e) {
                 for (var r = 0; r < e.length; r++) {
                     t.push(e[r])
                 }
             }
             return t
         }
 
-        function G(e, t) {
+        function Q(e, t) {
             if (e) {
                 for (var r = 0; r < e.length; r++) {
                     t(e[r])
                 }
             }
         }
 
-        function b(e) {
+        function P(e) {
             var t = e.getBoundingClientRect();
             var r = t.top;
             var n = t.bottom;
             return r < window.innerHeight && n >= 0
         }
 
-        function K(e) {
-            if (e.getRootNode() instanceof ShadowRoot) {
-                return _().body.contains(e.getRootNode().host)
+        function ee(e) {
+            if (e.getRootNode && e.getRootNode() instanceof ShadowRoot) {
+                return J().body.contains(e.getRootNode().host)
             } else {
-                return _().body.contains(e)
+                return J().body.contains(e)
             }
         }
 
-        function w(e) {
+        function M(e) {
             return e.trim().split(/\s+/)
         }
 
-        function Y(e, t) {
+        function te(e, t) {
             for (var r in t) {
                 if (t.hasOwnProperty(r)) {
                     e[r] = t[r]
                 }
             }
             return e
         }
 
-        function S(e) {
+        function y(e) {
             try {
                 return JSON.parse(e)
             } catch (e) {
-                St(e);
+                x(e);
                 return null
             }
         }
 
-        function E() {
+        function D() {
             var e = "htmx:localStorageTest";
             try {
                 localStorage.setItem(e, e);
                 localStorage.removeItem(e);
                 return true
             } catch (e) {
                 return false
             }
         }
 
+        function X(t) {
+            try {
+                var e = new URL(t);
+                if (e) {
+                    t = e.pathname + e.search
+                }
+                if (!t.match("^/$")) {
+                    t = t.replace(/\/+$/, "")
+                }
+                return t
+            } catch (e) {
+                return t
+            }
+        }
+
         function e(e) {
-            return Qt(_().body, function() {
+            return sr(J().body, function() {
                 return eval(e)
             })
         }
 
         function t(t) {
-            var e = U.on("htmx:load", function(e) {
+            var e = z.on("htmx:load", function(e) {
                 t(e.detail.elt)
             });
             return e
         }
 
-        function C() {
-            U.logger = function(e, t, r) {
+        function F() {
+            z.logger = function(e, t, r) {
                 if (console) {
                     console.log(t, e, r)
                 }
             }
         }
 
-        function R(e, t) {
+        function b(e, t) {
             if (t) {
                 return e.querySelector(t)
             } else {
-                return R(_(), e)
+                return b(J(), e)
             }
         }
 
-        function O(e, t) {
+        function f(e, t) {
             if (t) {
                 return e.querySelectorAll(t)
             } else {
-                return O(_(), e)
+                return f(J(), e)
             }
         }
 
-        function q(e, t) {
-            e = D(e);
+        function B(e, t) {
+            e = s(e);
             if (t) {
                 setTimeout(function() {
-                    q(e)
+                    B(e);
+                    e = null
                 }, t)
             } else {
                 e.parentElement.removeChild(e)
             }
         }
 
-        function L(e, t, r) {
-            e = D(e);
+        function j(e, t, r) {
+            e = s(e);
             if (r) {
                 setTimeout(function() {
-                    L(e, t)
+                    j(e, t);
+                    e = null
                 }, r)
             } else {
                 e.classList && e.classList.add(t)
             }
         }
 
-        function T(e, t, r) {
-            e = D(e);
+        function n(e, t, r) {
+            e = s(e);
             if (r) {
                 setTimeout(function() {
-                    T(e, t)
+                    n(e, t);
+                    e = null
                 }, r)
             } else {
                 if (e.classList) {
                     e.classList.remove(t);
                     if (e.classList.length === 0) {
                         e.removeAttribute("class")
                     }
                 }
             }
         }
 
-        function H(e, t) {
-            e = D(e);
+        function U(e, t) {
+            e = s(e);
             e.classList.toggle(t)
         }
 
-        function A(e, t) {
-            e = D(e);
-            G(e.parentElement.children, function(e) {
-                T(e, t)
+        function V(e, t) {
+            e = s(e);
+            Q(e.parentElement.children, function(e) {
+                n(e, t)
             });
-            L(e, t)
+            j(e, t)
         }
 
-        function N(e, t) {
-            e = D(e);
+        function d(e, t) {
+            e = s(e);
             if (e.closest) {
                 return e.closest(t)
             } else {
                 do {
-                    if (e == null || d(e, t)) {
+                    if (e == null || h(e, t)) {
                         return e
                     }
-                } while (e = e && u(e))
+                } while (e = e && u(e));
+                return null
             }
         }
 
-        function I(e, t) {
+        function r(e) {
+            var t = e.trim();
+            if (t.startsWith("<") && t.endsWith("/>")) {
+                return t.substring(1, t.length - 2)
+            } else {
+                return t
+            }
+        }
+
+        function _(e, t) {
             if (t.indexOf("closest ") === 0) {
-                return [N(e, t.substr(8))]
+                return [d(e, r(t.substr(8)))]
             } else if (t.indexOf("find ") === 0) {
-                return [R(e, t.substr(5))]
+                return [b(e, r(t.substr(5)))]
             } else if (t.indexOf("next ") === 0) {
-                return [k(e, t.substr(5))]
+                return [W(e, r(t.substr(5)))]
             } else if (t.indexOf("previous ") === 0) {
-                return [M(e, t.substr(9))]
+                return [oe(e, r(t.substr(9)))]
             } else if (t === "document") {
                 return [document]
             } else if (t === "window") {
                 return [window]
             } else {
-                return _().querySelectorAll(t)
+                return J().querySelectorAll(r(t))
             }
         }
-        var k = function(e, t) {
-            var r = _().querySelectorAll(t);
+        var W = function(e, t) {
+            var r = J().querySelectorAll(t);
             for (var n = 0; n < r.length; n++) {
                 var i = r[n];
                 if (i.compareDocumentPosition(e) === Node.DOCUMENT_POSITION_PRECEDING) {
                     return i
                 }
             }
         };
-        var M = function(e, t) {
-            var r = _().querySelectorAll(t);
+        var oe = function(e, t) {
+            var r = J().querySelectorAll(t);
             for (var n = r.length - 1; n >= 0; n--) {
                 var i = r[n];
                 if (i.compareDocumentPosition(e) === Node.DOCUMENT_POSITION_FOLLOWING) {
                     return i
                 }
             }
         };
 
-        function Q(e, t) {
+        function re(e, t) {
             if (t) {
-                return I(e, t)[0]
+                return _(e, t)[0]
             } else {
-                return I(_().body, e)[0]
+                return _(J().body, e)[0]
             }
         }
 
-        function D(e) {
-            if (p(e, "String")) {
-                return R(e)
+        function s(e) {
+            if (A(e, "String")) {
+                return b(e)
             } else {
                 return e
             }
         }
 
-        function P(e, t, r) {
-            if (m(t)) {
+        function se(e, t, r) {
+            if (N(t)) {
                 return {
-                    target: _().body,
+                    target: J().body,
                     event: e,
                     listener: t
                 }
             } else {
                 return {
-                    target: D(e),
+                    target: s(e),
                     event: t,
                     listener: r
                 }
             }
         }
 
-        function X(t, r, n) {
-            pr(function() {
-                var e = P(t, r, n);
+        function le(t, r, n) {
+            Sr(function() {
+                var e = se(t, r, n);
                 e.target.addEventListener(e.event, e.listener)
             });
-            var e = m(r);
+            var e = N(r);
             return e ? r : n
         }
 
-        function F(t, r, n) {
-            pr(function() {
-                var e = P(t, r, n);
+        function ue(t, r, n) {
+            Sr(function() {
+                var e = se(t, r, n);
                 e.target.removeEventListener(e.event, e.listener)
             });
-            return m(r) ? r : n
+            return N(r) ? r : n
         }
-        var ee = _().createElement("output");
+        var fe = J().createElement("output");
 
-        function j(e, t) {
-            var r = z(e, t);
+        function ce(e, t) {
+            var r = Z(e, t);
             if (r) {
                 if (r === "this") {
-                    return [te(e, t)]
+                    return [he(e, t)]
                 } else {
-                    var n = I(e, r);
+                    var n = _(e, r);
                     if (n.length === 0) {
-                        St('The selector "' + r + '" on ' + t + " returned no matches!");
-                        return [ee]
+                        x('The selector "' + r + '" on ' + t + " returned no matches!");
+                        return [fe]
                     } else {
                         return n
                     }
                 }
             }
         }
 
-        function te(e, t) {
-            return h(e, function(e) {
-                return V(e, t) != null
+        function he(e, t) {
+            return c(e, function(e) {
+                return G(e, t) != null
             })
         }
 
-        function re(e) {
-            var t = z(e, "hx-target");
+        function de(e) {
+            var t = Z(e, "hx-target");
             if (t) {
                 if (t === "this") {
-                    return te(e, "hx-target")
+                    return he(e, "hx-target")
                 } else {
-                    return Q(e, t)
+                    return re(e, t)
                 }
             } else {
-                var r = W(e);
+                var r = Y(e);
                 if (r.boosted) {
-                    return _().body
+                    return J().body
                 } else {
                     return e
                 }
             }
         }
 
-        function B(e) {
-            var t = U.config.attributesToSettle;
+        function ve(e) {
+            var t = z.config.attributesToSettle;
             for (var r = 0; r < t.length; r++) {
                 if (e === t[r]) {
                     return true
                 }
             }
             return false
         }
 
-        function ne(t, r) {
-            G(t.attributes, function(e) {
-                if (!r.hasAttribute(e.name) && B(e.name)) {
+        function ge(t, r) {
+            Q(t.attributes, function(e) {
+                if (!r.hasAttribute(e.name) && ve(e.name)) {
                     t.removeAttribute(e.name)
                 }
             });
-            G(r.attributes, function(e) {
-                if (B(e.name)) {
+            Q(r.attributes, function(e) {
+                if (ve(e.name)) {
                     t.setAttribute(e.name, e.value)
                 }
             })
         }
 
-        function ie(e, t) {
-            var r = gr(t);
+        function pe(e, t) {
+            var r = wr(t);
             for (var n = 0; n < r.length; n++) {
                 var i = r[n];
                 try {
                     if (i.isInlineSwap(e)) {
                         return true
                     }
                 } catch (e) {
-                    St(e)
+                    x(e)
                 }
             }
             return e === "outerHTML"
         }
 
-        function ae(e, i, a) {
+        function me(e, i, a) {
             var t = "#" + i.id;
             var o = "outerHTML";
             if (e === "true") {} else if (e.indexOf(":") > 0) {
                 o = e.substr(0, e.indexOf(":"));
                 t = e.substr(e.indexOf(":") + 1, e.length)
             } else {
                 o = e
             }
-            var r = _().querySelectorAll(t);
+            var r = J().querySelectorAll(t);
             if (r) {
-                G(r, function(e) {
+                Q(r, function(e) {
                     var t;
                     var r = i.cloneNode(true);
-                    t = _().createDocumentFragment();
+                    t = J().createDocumentFragment();
                     t.appendChild(r);
-                    if (!ie(o, e)) {
+                    if (!pe(o, e)) {
                         t = r
                     }
                     var n = {
                         shouldSwap: true,
                         target: e,
                         fragment: t
                     };
-                    if (!$(e, "htmx:oobBeforeSwap", n)) return;
+                    if (!ie(e, "htmx:oobBeforeSwap", n)) return;
                     e = n.target;
                     if (n["shouldSwap"]) {
-                        Ce(o, e, e, t, a)
+                        ke(o, e, e, t, a)
                     }
-                    G(a.elts, function(e) {
-                        $(e, "htmx:oobAfterSwap", n)
+                    Q(a.elts, function(e) {
+                        ie(e, "htmx:oobAfterSwap", n)
                     })
                 });
                 i.parentNode.removeChild(i)
             } else {
                 i.parentNode.removeChild(i);
-                J(_().body, "htmx:oobErrorNoTarget", {
+                ne(J().body, "htmx:oobErrorNoTarget", {
                     content: i
                 })
             }
             return e
         }
 
-        function oe(e, t, r) {
-            var n = z(e, "hx-select-oob");
+        function xe(e, t, r) {
+            var n = Z(e, "hx-select-oob");
             if (n) {
                 var i = n.split(",");
                 for (let e = 0; e < i.length; e++) {
                     var a = i[e].split(":", 2);
-                    var o = a[0];
+                    var o = a[0].trim();
                     if (o.indexOf("#") === 0) {
                         o = o.substring(1)
                     }
                     var s = a[1] || "true";
                     var l = t.querySelector("#" + o);
                     if (l) {
-                        ae(s, l, r)
+                        me(s, l, r)
                     }
                 }
             }
-            G(O(t, "[hx-swap-oob], [data-hx-swap-oob]"), function(e) {
-                var t = V(e, "hx-swap-oob");
+            Q(f(t, "[hx-swap-oob], [data-hx-swap-oob]"), function(e) {
+                var t = G(e, "hx-swap-oob");
                 if (t != null) {
-                    ae(t, e, r)
+                    me(t, e, r)
                 }
             })
         }
 
-        function se(e) {
-            G(O(e, "[hx-preserve], [data-hx-preserve]"), function(e) {
-                var t = V(e, "id");
-                var r = _().getElementById(t);
+        function ye(e) {
+            Q(f(e, "[hx-preserve], [data-hx-preserve]"), function(e) {
+                var t = G(e, "id");
+                var r = J().getElementById(t);
                 if (r != null) {
                     e.parentNode.replaceChild(r, e)
                 }
             })
         }
 
-        function le(n, e, i) {
-            G(e.querySelectorAll("[id]"), function(e) {
+        function be(a, e, o) {
+            Q(e.querySelectorAll("[id]"), function(e) {
                 if (e.id && e.id.length > 0) {
-                    var t = n.querySelector(e.tagName + "[id='" + e.id + "']");
-                    if (t && t !== n) {
-                        var r = e.cloneNode();
-                        ne(e, t);
-                        i.tasks.push(function() {
-                            ne(e, r)
+                    var t = e.id.replace("'", "\\'");
+                    var r = e.tagName.replace(":", "\\:");
+                    var n = a.querySelector(r + "[id='" + t + "']");
+                    if (n && n !== a) {
+                        var i = e.cloneNode();
+                        ge(e, n);
+                        o.tasks.push(function() {
+                            ge(e, i)
                         })
                     }
                 }
             })
         }
 
-        function ue(e) {
+        function we(e) {
             return function() {
-                T(e, U.config.addedClass);
-                mt(e);
-                ht(e);
-                fe(e);
-                $(e, "htmx:load")
+                n(e, z.config.addedClass);
+                Tt(e);
+                bt(e);
+                Se(e);
+                ie(e, "htmx:load")
             }
         }
 
-        function fe(e) {
+        function Se(e) {
             var t = "[autofocus]";
-            var r = d(e, t) ? e : e.querySelector(t);
+            var r = h(e, t) ? e : e.querySelector(t);
             if (r != null) {
                 r.focus()
             }
         }
 
-        function ce(e, t, r, n) {
-            le(e, r, n);
+        function a(e, t, r, n) {
+            be(e, r, n);
             while (r.childNodes.length > 0) {
                 var i = r.firstChild;
-                L(i, U.config.addedClass);
+                j(i, z.config.addedClass);
                 e.insertBefore(i, t);
                 if (i.nodeType !== Node.TEXT_NODE && i.nodeType !== Node.COMMENT_NODE) {
-                    n.tasks.push(ue(i))
+                    n.tasks.push(we(i))
                 }
             }
         }
 
-        function he(e, t) {
+        function Ee(e, t) {
             var r = 0;
             while (r < e.length) {
                 t = (t << 5) - t + e.charCodeAt(r++) | 0
             }
             return t
         }
 
-        function de(e) {
+        function Ce(e) {
             var t = 0;
-            for (var r = 0; r < e.attributes.length; r++) {
-                var n = e.attributes[r];
-                if (n.value) {
-                    t = he(n.name, t);
-                    t = he(n.value, t)
+            if (e.attributes) {
+                for (var r = 0; r < e.attributes.length; r++) {
+                    var n = e.attributes[r];
+                    if (n.value) {
+                        t = Ee(n.name, t);
+                        t = Ee(n.value, t)
+                    }
                 }
             }
             return t
         }
 
-        function ve(e) {
-            var t = W(e);
-            if (t.webSocket) {
-                t.webSocket.close()
+        function Re(t) {
+            var r = Y(t);
+            if (r.timeout) {
+                clearTimeout(r.timeout)
+            }
+            if (r.webSocket) {
+                r.webSocket.close()
             }
-            if (t.sseEventSource) {
-                t.sseEventSource.close()
+            if (r.sseEventSource) {
+                r.sseEventSource.close()
             }
-            if (t.listenerInfos) {
-                G(t.listenerInfos, function(e) {
+            if (r.listenerInfos) {
+                Q(r.listenerInfos, function(e) {
                     if (e.on) {
                         e.on.removeEventListener(e.trigger, e.listener)
                     }
                 })
             }
+            if (r.onHandlers) {
+                for (let e = 0; e < r.onHandlers.length; e++) {
+                    const n = r.onHandlers[e];
+                    t.removeEventListener(n.name, n.handler)
+                }
+            }
         }
 
-        function ge(e) {
-            $(e, "htmx:beforeCleanupElement");
-            ve(e);
+        function o(e) {
+            ie(e, "htmx:beforeCleanupElement");
+            Re(e);
             if (e.children) {
-                G(e.children, function(e) {
-                    ge(e)
+                Q(e.children, function(e) {
+                    o(e)
                 })
             }
         }
 
-        function pe(e, t, r) {
+        function Oe(e, t, r) {
             if (e.tagName === "BODY") {
-                return Se(e, t, r)
+                return Ne(e, t, r)
             } else {
                 var n;
                 var i = e.previousSibling;
-                ce(u(e), e, t, r);
+                a(u(e), e, t, r);
                 if (i == null) {
                     n = u(e).firstChild
                 } else {
                     n = i.nextSibling
                 }
-                W(e).replacedWith = n;
+                Y(e).replacedWith = n;
                 r.elts = [];
                 while (n && n !== e) {
                     if (n.nodeType === Node.ELEMENT_NODE) {
                         r.elts.push(n)
                     }
                     n = n.nextElementSibling
                 }
-                ge(e);
+                o(e);
                 u(e).removeChild(e)
             }
         }
 
-        function me(e, t, r) {
-            return ce(e, e.firstChild, t, r)
+        function qe(e, t, r) {
+            return a(e, e.firstChild, t, r)
         }
 
-        function xe(e, t, r) {
-            return ce(u(e), e, t, r)
+        function Te(e, t, r) {
+            return a(u(e), e, t, r)
         }
 
-        function ye(e, t, r) {
-            return ce(e, null, t, r)
+        function He(e, t, r) {
+            return a(e, null, t, r)
         }
 
-        function be(e, t, r) {
-            return ce(u(e), e.nextSibling, t, r)
+        function Le(e, t, r) {
+            return a(u(e), e.nextSibling, t, r)
         }
 
-        function we(e, t, r) {
-            ge(e);
+        function Ae(e, t, r) {
+            o(e);
             return u(e).removeChild(e)
         }
 
-        function Se(e, t, r) {
+        function Ne(e, t, r) {
             var n = e.firstChild;
-            ce(e, n, t, r);
+            a(e, n, t, r);
             if (n) {
                 while (n.nextSibling) {
-                    ge(n.nextSibling);
+                    o(n.nextSibling);
                     e.removeChild(n.nextSibling)
                 }
-                ge(n);
+                o(n);
                 e.removeChild(n)
             }
         }
 
-        function Ee(e, t) {
-            var r = z(e, "hx-select");
+        function Ie(e, t) {
+            var r = Z(e, "hx-select");
             if (r) {
-                var n = _().createDocumentFragment();
-                G(t.querySelectorAll(r), function(e) {
+                var n = J().createDocumentFragment();
+                Q(t.querySelectorAll(r), function(e) {
                     n.appendChild(e)
                 });
                 t = n
             }
             return t
         }
 
-        function Ce(e, t, r, n, i) {
+        function ke(e, t, r, n, i) {
             switch (e) {
                 case "none":
                     return;
                 case "outerHTML":
-                    pe(r, n, i);
+                    Oe(r, n, i);
                     return;
                 case "afterbegin":
-                    me(r, n, i);
+                    qe(r, n, i);
                     return;
                 case "beforebegin":
-                    xe(r, n, i);
+                    Te(r, n, i);
                     return;
                 case "beforeend":
-                    ye(r, n, i);
+                    He(r, n, i);
                     return;
                 case "afterend":
-                    be(r, n, i);
+                    Le(r, n, i);
                     return;
                 case "delete":
-                    we(r, n, i);
+                    Ae(r, n, i);
                     return;
                 default:
-                    var a = gr(t);
+                    var a = wr(t);
                     for (var o = 0; o < a.length; o++) {
-                        var f = a[o];
+                        var s = a[o];
                         try {
-                            var s = f.handleSwap(e, r, n, i);
-                            if (s) {
-                                if (typeof s.length !== "undefined") {
-                                    for (var l = 0; l < s.length; l++) {
-                                        var u = s[l];
-                                        if (u.nodeType !== Node.TEXT_NODE && u.nodeType !== Node.COMMENT_NODE) {
-                                            i.tasks.push(ue(u))
+                            var l = s.handleSwap(e, r, n, i);
+                            if (l) {
+                                if (typeof l.length !== "undefined") {
+                                    for (var u = 0; u < l.length; u++) {
+                                        var f = l[u];
+                                        if (f.nodeType !== Node.TEXT_NODE && f.nodeType !== Node.COMMENT_NODE) {
+                                            i.tasks.push(we(f))
                                         }
                                     }
                                 }
                                 return
                             }
                         } catch (e) {
-                            St(e)
+                            x(e)
                         }
                     }
                     if (e === "innerHTML") {
-                        Se(r, n, i)
+                        Ne(r, n, i)
                     } else {
-                        Ce(U.config.defaultSwapStyle, t, r, n, i)
+                        ke(z.config.defaultSwapStyle, t, r, n, i)
                     }
             }
         }
 
-        function Re(e) {
+        function Pe(e) {
             if (e.indexOf("<title") > -1) {
                 var t = e.replace(/<svg(\s[^>]*>|>)([\s\S]*?)<\/svg>/gim, "");
                 var r = t.match(/<title(\s[^>]*>|>)([\s\S]*?)<\/title>/im);
                 if (r) {
                     return r[2]
                 }
             }
         }
 
-        function Oe(e, t, r, n, i) {
-            i.title = Re(n);
-            var a = g(n);
+        function Me(e, t, r, n, i) {
+            i.title = Pe(n);
+            var a = l(n);
             if (a) {
-                oe(r, a, i);
-                a = Ee(r, a);
-                se(a);
-                return Ce(e, r, t, a, i)
+                xe(r, a, i);
+                a = Ie(r, a);
+                ye(a);
+                return ke(e, r, t, a, i)
             }
         }
 
-        function qe(e, t, r) {
+        function De(e, t, r) {
             var n = e.getResponseHeader(t);
             if (n.indexOf("{") === 0) {
-                var i = S(n);
+                var i = y(n);
                 for (var a in i) {
                     if (i.hasOwnProperty(a)) {
                         var o = i[a];
-                        if (!x(o)) {
+                        if (!I(o)) {
                             o = {
                                 value: o
                             }
                         }
-                        $(r, a, o)
+                        ie(r, a, o)
                     }
                 }
             } else {
-                $(r, n, [])
+                ie(r, n, [])
             }
         }
-        var Le = /\s/;
-        var Te = /[\s,]/;
-        var He = /[_$a-zA-Z]/;
-        var Ae = /[_$a-zA-Z0-9]/;
-        var Ne = ['"', "'", "/"];
-        var Ie = /[^\s]/;
+        var Xe = /\s/;
+        var g = /[\s,]/;
+        var Fe = /[_$a-zA-Z]/;
+        var Be = /[_$a-zA-Z0-9]/;
+        var je = ['"', "'", "/"];
+        var p = /[^\s]/;
 
-        function ke(e) {
+        function Ue(e) {
             var t = [];
             var r = 0;
             while (r < e.length) {
-                if (He.exec(e.charAt(r))) {
+                if (Fe.exec(e.charAt(r))) {
                     var n = r;
-                    while (Ae.exec(e.charAt(r + 1))) {
+                    while (Be.exec(e.charAt(r + 1))) {
                         r++
                     }
                     t.push(e.substr(n, r - n + 1))
-                } else if (Ne.indexOf(e.charAt(r)) !== -1) {
+                } else if (je.indexOf(e.charAt(r)) !== -1) {
                     var i = e.charAt(r);
                     var n = r;
                     r++;
                     while (r < e.length && e.charAt(r) !== i) {
                         if (e.charAt(r) === "\\") {
                             r++
                         }
@@ -941,19 +994,19 @@
                     t.push(a)
                 }
                 r++
             }
             return t
         }
 
-        function Me(e, t, r) {
-            return He.exec(e.charAt(0)) && e !== "true" && e !== "false" && e !== "this" && e !== r && t !== "."
+        function Ve(e, t, r) {
+            return Fe.exec(e.charAt(0)) && e !== "true" && e !== "false" && e !== "this" && e !== r && t !== "."
         }
 
-        function De(e, t, r) {
+        function _e(e, t, r) {
             if (t[0] === "[") {
                 t.shift();
                 var n = 1;
                 var i = " return (function(" + r + "){ return (";
                 var a = null;
                 while (t.length > 0) {
                     var o = t[0];
@@ -962,1023 +1015,1116 @@
                         if (n === 0) {
                             if (a === null) {
                                 i = i + "true"
                             }
                             t.shift();
                             i += ")})";
                             try {
-                                var s = Qt(e, function() {
+                                var s = sr(e, function() {
                                     return Function(i)()
                                 }, function() {
                                     return true
                                 });
                                 s.source = i;
                                 return s
                             } catch (e) {
-                                J(_().body, "htmx:syntax:error", {
+                                ne(J().body, "htmx:syntax:error", {
                                     error: e,
                                     source: i
                                 });
                                 return null
                             }
                         }
                     } else if (o === "[") {
                         n++
                     }
-                    if (Me(o, a, r)) {
+                    if (Ve(o, a, r)) {
                         i += "((" + r + "." + o + ") ? (" + r + "." + o + ") : (window." + o + "))"
                     } else {
                         i = i + o
                     }
                     a = t.shift()
                 }
             }
         }
 
-        function c(e, t) {
+        function m(e, t) {
             var r = "";
             while (e.length > 0 && !e[0].match(t)) {
                 r += e.shift()
             }
             return r
         }
-        var Pe = "input, textarea, select";
+        var We = "input, textarea, select";
 
-        function Xe(e) {
-            var t = V(e, "hx-trigger");
+        function ze(e) {
+            var t = G(e, "hx-trigger");
             var r = [];
             if (t) {
-                var n = ke(t);
+                var n = Ue(t);
                 do {
-                    c(n, Ie);
-                    var f = n.length;
-                    var i = c(n, /[,\[\s]/);
-                    if (i !== "") {
-                        if (i === "every") {
-                            var a = {
+                    m(n, p);
+                    var i = n.length;
+                    var a = m(n, /[,\[\s]/);
+                    if (a !== "") {
+                        if (a === "every") {
+                            var o = {
                                 trigger: "every"
                             };
-                            c(n, Ie);
-                            a.pollInterval = v(c(n, /[,\[\s]/));
-                            c(n, Ie);
-                            var o = De(e, n, "event");
-                            if (o) {
-                                a.eventFilter = o
+                            m(n, p);
+                            o.pollInterval = v(m(n, /[,\[\s]/));
+                            m(n, p);
+                            var s = _e(e, n, "event");
+                            if (s) {
+                                o.eventFilter = s
                             }
-                            r.push(a)
-                        } else if (i.indexOf("sse:") === 0) {
+                            r.push(o)
+                        } else if (a.indexOf("sse:") === 0) {
                             r.push({
                                 trigger: "sse",
-                                sseEvent: i.substr(4)
+                                sseEvent: a.substr(4)
                             })
                         } else {
-                            var s = {
-                                trigger: i
+                            var l = {
+                                trigger: a
                             };
-                            var o = De(e, n, "event");
-                            if (o) {
-                                s.eventFilter = o
+                            var s = _e(e, n, "event");
+                            if (s) {
+                                l.eventFilter = s
                             }
                             while (n.length > 0 && n[0] !== ",") {
-                                c(n, Ie);
-                                var l = n.shift();
-                                if (l === "changed") {
-                                    s.changed = true
-                                } else if (l === "once") {
-                                    s.once = true
-                                } else if (l === "consume") {
-                                    s.consume = true
-                                } else if (l === "delay" && n[0] === ":") {
+                                m(n, p);
+                                var u = n.shift();
+                                if (u === "changed") {
+                                    l.changed = true
+                                } else if (u === "once") {
+                                    l.once = true
+                                } else if (u === "consume") {
+                                    l.consume = true
+                                } else if (u === "delay" && n[0] === ":") {
                                     n.shift();
-                                    s.delay = v(c(n, Te))
-                                } else if (l === "from" && n[0] === ":") {
+                                    l.delay = v(m(n, g))
+                                } else if (u === "from" && n[0] === ":") {
                                     n.shift();
-                                    var u = c(n, Te);
-                                    if (u === "closest" || u === "find" || u === "next" || u === "previous") {
+                                    var f = m(n, g);
+                                    if (f === "closest" || f === "find" || f === "next" || f === "previous") {
                                         n.shift();
-                                        u += " " + c(n, Te)
+                                        f += " " + m(n, g)
                                     }
-                                    s.from = u
-                                } else if (l === "target" && n[0] === ":") {
+                                    l.from = f
+                                } else if (u === "target" && n[0] === ":") {
                                     n.shift();
-                                    s.target = c(n, Te)
-                                } else if (l === "throttle" && n[0] === ":") {
+                                    l.target = m(n, g)
+                                } else if (u === "throttle" && n[0] === ":") {
                                     n.shift();
-                                    s.throttle = v(c(n, Te))
-                                } else if (l === "queue" && n[0] === ":") {
+                                    l.throttle = v(m(n, g))
+                                } else if (u === "queue" && n[0] === ":") {
                                     n.shift();
-                                    s.queue = c(n, Te)
-                                } else if ((l === "root" || l === "threshold") && n[0] === ":") {
+                                    l.queue = m(n, g)
+                                } else if ((u === "root" || u === "threshold") && n[0] === ":") {
                                     n.shift();
-                                    s[l] = c(n, Te)
+                                    l[u] = m(n, g)
                                 } else {
-                                    J(e, "htmx:syntax:error", {
+                                    ne(e, "htmx:syntax:error", {
                                         token: n.shift()
                                     })
                                 }
                             }
-                            r.push(s)
+                            r.push(l)
                         }
                     }
-                    if (n.length === f) {
-                        J(e, "htmx:syntax:error", {
+                    if (n.length === i) {
+                        ne(e, "htmx:syntax:error", {
                             token: n.shift()
                         })
                     }
-                    c(n, Ie)
+                    m(n, p)
                 } while (n[0] === "," && n.shift())
             }
             if (r.length > 0) {
                 return r
-            } else if (d(e, "form")) {
+            } else if (h(e, "form")) {
                 return [{
                     trigger: "submit"
                 }]
-            } else if (d(e, 'input[type="button"]')) {
+            } else if (h(e, 'input[type="button"]')) {
                 return [{
                     trigger: "click"
                 }]
-            } else if (d(e, Pe)) {
+            } else if (h(e, We)) {
                 return [{
                     trigger: "change"
                 }]
             } else {
                 return [{
                     trigger: "click"
                 }]
             }
         }
 
-        function Fe(e) {
-            W(e).cancelled = true
+        function $e(e) {
+            Y(e).cancelled = true
         }
 
-        function je(e, t, r) {
-            var n = W(e);
+        function Ge(e, t, r) {
+            var n = Y(e);
             n.timeout = setTimeout(function() {
-                if (K(e) && n.cancelled !== true) {
-                    if (!ze(r, yt("hx:poll:trigger", {
+                if (ee(e) && n.cancelled !== true) {
+                    if (!Qe(r, Lt("hx:poll:trigger", {
                             triggerSpec: r,
                             target: e
                         }))) {
                         t(e)
                     }
-                    je(e, t, r)
+                    Ge(e, t, r)
                 }
             }, r.pollInterval)
         }
 
-        function Be(e) {
-            return location.hostname === e.hostname && f(e, "href") && f(e, "href").indexOf("#") !== 0
+        function Je(e) {
+            return location.hostname === e.hostname && $(e, "href") && $(e, "href").indexOf("#") !== 0
         }
 
-        function Ue(t, r, e) {
-            if (t.tagName === "A" && Be(t) && (t.target === "" || t.target === "_self") || t.tagName === "FORM") {
+        function Ze(t, r, e) {
+            if (t.tagName === "A" && Je(t) && (t.target === "" || t.target === "_self") || t.tagName === "FORM") {
                 r.boosted = true;
                 var n, i;
                 if (t.tagName === "A") {
                     n = "get";
-                    i = f(t, "href")
+                    i = t.href
                 } else {
-                    var a = f(t, "method");
+                    var a = $(t, "method");
                     n = a ? a.toLowerCase() : "get";
                     if (n === "get") {}
-                    i = f(t, "action")
+                    i = $(t, "action")
                 }
                 e.forEach(function(e) {
-                    We(t, function(e) {
-                        lr(n, i, t, e)
+                    et(t, function(e, t) {
+                        ae(n, i, e, t)
                     }, r, e, true)
                 })
             }
         }
 
-        function Ve(e, t) {
+        function Ke(e, t) {
             if (e.type === "submit" || e.type === "click") {
                 if (t.tagName === "FORM") {
                     return true
                 }
-                if (d(t, 'input[type="submit"], button') && N(t, "form") !== null) {
+                if (h(t, 'input[type="submit"], button') && d(t, "form") !== null) {
                     return true
                 }
                 if (t.tagName === "A" && t.href && (t.getAttribute("href") === "#" || t.getAttribute("href").indexOf("#") !== 0)) {
                     return true
                 }
             }
             return false
         }
 
-        function _e(e, t) {
-            return W(e).boosted && e.tagName === "A" && t.type === "click" && (t.ctrlKey || t.metaKey)
+        function Ye(e, t) {
+            return Y(e).boosted && e.tagName === "A" && t.type === "click" && (t.ctrlKey || t.metaKey)
         }
 
-        function ze(e, t) {
+        function Qe(e, t) {
             var r = e.eventFilter;
             if (r) {
                 try {
                     return r(t) !== true
                 } catch (e) {
-                    J(_().body, "htmx:eventFilter:error", {
+                    ne(J().body, "htmx:eventFilter:error", {
                         error: e,
                         source: r.source
                     });
                     return true
                 }
             }
             return false
         }
 
-        function We(a, o, e, s, l) {
+        function et(i, a, e, o, s) {
+            var l = Y(i);
             var t;
-            if (s.from) {
-                t = I(a, s.from)
+            if (o.from) {
+                t = _(i, o.from)
             } else {
-                t = [a]
+                t = [i]
             }
-            G(t, function(n) {
-                var i = function(e) {
-                    if (!K(a)) {
-                        n.removeEventListener(s.trigger, i);
+            if (o.changed) {
+                l.lastValue = i.value
+            }
+            Q(t, function(r) {
+                var n = function(e) {
+                    if (!ee(i)) {
+                        r.removeEventListener(o.trigger, n);
                         return
                     }
-                    if (_e(a, e)) {
+                    if (Ye(i, e)) {
                         return
                     }
-                    if (l || Ve(e, a)) {
+                    if (s || Ke(e, i)) {
                         e.preventDefault()
                     }
-                    if (ze(s, e)) {
+                    if (Qe(o, e)) {
                         return
                     }
-                    var t = W(e);
-                    t.triggerSpec = s;
+                    var t = Y(e);
+                    t.triggerSpec = o;
                     if (t.handledFor == null) {
                         t.handledFor = []
                     }
-                    var r = W(a);
-                    if (t.handledFor.indexOf(a) < 0) {
-                        t.handledFor.push(a);
-                        if (s.consume) {
+                    if (t.handledFor.indexOf(i) < 0) {
+                        t.handledFor.push(i);
+                        if (o.consume) {
                             e.stopPropagation()
                         }
-                        if (s.target && e.target) {
-                            if (!d(e.target, s.target)) {
+                        if (o.target && e.target) {
+                            if (!h(e.target, o.target)) {
                                 return
                             }
                         }
-                        if (s.once) {
-                            if (r.triggeredOnce) {
+                        if (o.once) {
+                            if (l.triggeredOnce) {
                                 return
                             } else {
-                                r.triggeredOnce = true
+                                l.triggeredOnce = true
                             }
                         }
-                        if (s.changed) {
-                            if (r.lastValue === a.value) {
+                        if (o.changed) {
+                            if (l.lastValue === i.value) {
                                 return
                             } else {
-                                r.lastValue = a.value
+                                l.lastValue = i.value
                             }
                         }
-                        if (r.delayed) {
-                            clearTimeout(r.delayed)
+                        if (l.delayed) {
+                            clearTimeout(l.delayed)
                         }
-                        if (r.throttle) {
+                        if (l.throttle) {
                             return
                         }
-                        if (s.throttle) {
-                            if (!r.throttle) {
-                                o(a, e);
-                                r.throttle = setTimeout(function() {
-                                    r.throttle = null
-                                }, s.throttle)
-                            }
-                        } else if (s.delay) {
-                            r.delayed = setTimeout(function() {
-                                o(a, e)
-                            }, s.delay)
+                        if (o.throttle) {
+                            if (!l.throttle) {
+                                a(i, e);
+                                l.throttle = setTimeout(function() {
+                                    l.throttle = null
+                                }, o.throttle)
+                            }
+                        } else if (o.delay) {
+                            l.delayed = setTimeout(function() {
+                                a(i, e)
+                            }, o.delay)
                         } else {
-                            o(a, e)
+                            ie(i, "htmx:trigger");
+                            a(i, e)
                         }
                     }
                 };
                 if (e.listenerInfos == null) {
                     e.listenerInfos = []
                 }
                 e.listenerInfos.push({
-                    trigger: s.trigger,
-                    listener: i,
-                    on: n
+                    trigger: o.trigger,
+                    listener: n,
+                    on: r
                 });
-                n.addEventListener(s.trigger, i)
+                r.addEventListener(o.trigger, n)
             })
         }
-        var Ge = false;
-        var Je = null;
+        var tt = false;
+        var rt = null;
 
-        function $e() {
-            if (!Je) {
-                Je = function() {
-                    Ge = true
+        function nt() {
+            if (!rt) {
+                rt = function() {
+                    tt = true
                 };
-                window.addEventListener("scroll", Je);
+                window.addEventListener("scroll", rt);
                 setInterval(function() {
-                    if (Ge) {
-                        Ge = false;
-                        G(_().querySelectorAll("[hx-trigger='revealed'],[data-hx-trigger='revealed']"), function(e) {
-                            Ze(e)
+                    if (tt) {
+                        tt = false;
+                        Q(J().querySelectorAll("[hx-trigger='revealed'],[data-hx-trigger='revealed']"), function(e) {
+                            it(e)
                         })
                     }
                 }, 200)
             }
         }
 
-        function Ze(t) {
-            if (!o(t, "data-hx-revealed") && b(t)) {
+        function it(t) {
+            if (!q(t, "data-hx-revealed") && P(t)) {
                 t.setAttribute("data-hx-revealed", "true");
-                var e = W(t);
+                var e = Y(t);
                 if (e.initHash) {
-                    $(t, "revealed")
+                    ie(t, "revealed")
                 } else {
                     t.addEventListener("htmx:afterProcessNode", function(e) {
-                        $(t, "revealed")
+                        ie(t, "revealed")
                     }, {
                         once: true
                     })
                 }
             }
         }
 
-        function Ke(e, t, r) {
-            var n = w(r);
+        function at(e, t, r) {
+            var n = M(r);
             for (var i = 0; i < n.length; i++) {
                 var a = n[i].split(/:(.+)/);
                 if (a[0] === "connect") {
-                    Ye(e, a[1], 0)
+                    ot(e, a[1], 0)
                 }
                 if (a[0] === "send") {
-                    et(e)
+                    lt(e)
                 }
             }
         }
 
-        function Ye(s, r, n) {
-            if (!K(s)) {
+        function ot(s, r, n) {
+            if (!ee(s)) {
                 return
             }
             if (r.indexOf("/") == 0) {
                 var e = location.hostname + (location.port ? ":" + location.port : "");
                 if (location.protocol == "https:") {
                     r = "wss://" + e + r
                 } else if (location.protocol == "http:") {
                     r = "ws://" + e + r
                 }
             }
-            var t = U.createWebSocket(r);
+            var t = z.createWebSocket(r);
             t.onerror = function(e) {
-                J(s, "htmx:wsError", {
+                ne(s, "htmx:wsError", {
                     error: e,
                     socket: t
                 });
-                Qe(s)
+                st(s)
             };
             t.onclose = function(e) {
                 if ([1006, 1012, 1013].indexOf(e.code) >= 0) {
-                    var t = tt(n);
+                    var t = ut(n);
                     setTimeout(function() {
-                        Ye(s, r, n + 1)
+                        ot(s, r, n + 1)
                     }, t)
                 }
             };
             t.onopen = function(e) {
                 n = 0
             };
-            W(s).webSocket = t;
+            Y(s).webSocket = t;
             t.addEventListener("message", function(e) {
-                if (Qe(s)) {
+                if (st(s)) {
                     return
                 }
                 var t = e.data;
-                wt(s, function(e) {
+                w(s, function(e) {
                     t = e.transformResponse(t, null, s)
                 });
-                var r = Zt(s);
-                var n = g(t);
-                var i = y(n.children);
+                var r = S(s);
+                var n = l(t);
+                var i = k(n.children);
                 for (var a = 0; a < i.length; a++) {
                     var o = i[a];
-                    ae(V(o, "hx-swap-oob") || "true", o, r)
+                    me(G(o, "hx-swap-oob") || "true", o, r)
                 }
-                At(r.tasks)
+                Bt(r.tasks)
             })
         }
 
-        function Qe(e) {
-            if (!K(e)) {
-                W(e).webSocket.close();
+        function st(e) {
+            if (!ee(e)) {
+                Y(e).webSocket.close();
                 return true
             }
         }
 
-        function et(u) {
-            var f = h(u, function(e) {
-                return W(e).webSocket != null
+        function lt(u) {
+            var f = c(u, function(e) {
+                return Y(e).webSocket != null
             });
             if (f) {
-                u.addEventListener(Xe(u)[0].trigger, function(e) {
-                    var t = W(f).webSocket;
-                    var r = _t(u, f);
-                    var n = jt(u, "post");
+                u.addEventListener(ze(u)[0].trigger, function(e) {
+                    var t = Y(f).webSocket;
+                    var r = Qt(u, f);
+                    var n = Jt(u, "post");
                     var i = n.errors;
                     var a = n.values;
-                    var o = rr(u);
-                    var s = Y(a, o);
-                    var l = zt(s, u);
+                    var o = fr(u);
+                    var s = te(a, o);
+                    var l = er(s, u);
                     l["HEADERS"] = r;
                     if (i && i.length > 0) {
-                        $(u, "htmx:validation:halted", i);
+                        ie(u, "htmx:validation:halted", i);
                         return
                     }
                     t.send(JSON.stringify(l));
-                    if (Ve(e, u)) {
+                    if (Ke(e, u)) {
                         e.preventDefault()
                     }
                 })
             } else {
-                J(u, "htmx:noWebSocketSourceError")
+                ne(u, "htmx:noWebSocketSourceError")
             }
         }
 
-        function tt(e) {
-            var t = U.config.wsReconnectDelay;
+        function ut(e) {
+            var t = z.config.wsReconnectDelay;
             if (typeof t === "function") {
                 return t(e)
             }
             if (t === "full-jitter") {
                 var r = Math.min(e, 6);
                 var n = 1e3 * Math.pow(2, r);
                 return n * Math.random()
             }
-            St('htmx.config.wsReconnectDelay must either be a function or the string "full-jitter"')
+            x('htmx.config.wsReconnectDelay must either be a function or the string "full-jitter"')
         }
 
-        function rt(e, t, r) {
-            var n = w(r);
+        function ft(e, t, r) {
+            var n = M(r);
             for (var i = 0; i < n.length; i++) {
                 var a = n[i].split(/:(.+)/);
                 if (a[0] === "connect") {
-                    nt(e, a[1])
+                    ct(e, a[1])
                 }
                 if (a[0] === "swap") {
-                    it(e, a[1])
+                    ht(e, a[1])
                 }
             }
         }
 
-        function nt(t, e) {
-            var r = U.createEventSource(e);
+        function ct(t, e) {
+            var r = z.createEventSource(e);
             r.onerror = function(e) {
-                J(t, "htmx:sseError", {
+                ne(t, "htmx:sseError", {
                     error: e,
                     source: r
                 });
-                ot(t)
+                vt(t)
             };
-            W(t).sseEventSource = r
+            Y(t).sseEventSource = r
         }
 
-        function it(a, o) {
-            var s = h(a, st);
+        function ht(a, o) {
+            var s = c(a, gt);
             if (s) {
-                var l = W(s).sseEventSource;
+                var l = Y(s).sseEventSource;
                 var u = function(e) {
-                    if (ot(s)) {
+                    if (vt(s)) {
                         l.removeEventListener(o, u);
                         return
                     }
                     var t = e.data;
-                    wt(a, function(e) {
+                    w(a, function(e) {
                         t = e.transformResponse(t, null, a)
                     });
-                    var r = Gt(a);
-                    var n = re(a);
-                    var i = Zt(a);
-                    Oe(r.swapStyle, a, n, t, i);
-                    At(i.tasks);
-                    $(a, "htmx:sseMessage", e)
+                    var r = rr(a);
+                    var n = de(a);
+                    var i = S(a);
+                    Me(r.swapStyle, a, n, t, i);
+                    Bt(i.tasks);
+                    ie(a, "htmx:sseMessage", e)
                 };
-                W(a).sseListener = u;
+                Y(a).sseListener = u;
                 l.addEventListener(o, u)
             } else {
-                J(a, "htmx:noSSESourceError")
+                ne(a, "htmx:noSSESourceError")
             }
         }
 
-        function at(e, t, r) {
-            var n = h(e, st);
+        function dt(e, t, r) {
+            var n = c(e, gt);
             if (n) {
-                var i = W(n).sseEventSource;
+                var i = Y(n).sseEventSource;
                 var a = function() {
-                    if (!ot(n)) {
-                        if (K(e)) {
+                    if (!vt(n)) {
+                        if (ee(e)) {
                             t(e)
                         } else {
                             i.removeEventListener(r, a)
                         }
                     }
                 };
-                W(e).sseListener = a;
+                Y(e).sseListener = a;
                 i.addEventListener(r, a)
             } else {
-                J(e, "htmx:noSSESourceError")
+                ne(e, "htmx:noSSESourceError")
             }
         }
 
-        function ot(e) {
-            if (!K(e)) {
-                W(e).sseEventSource.close();
+        function vt(e) {
+            if (!ee(e)) {
+                Y(e).sseEventSource.close();
                 return true
             }
         }
 
-        function st(e) {
-            return W(e).sseEventSource != null
+        function gt(e) {
+            return Y(e).sseEventSource != null
         }
 
-        function lt(e, t, r, n) {
+        function pt(e, t, r, n) {
             var i = function() {
                 if (!r.loaded) {
                     r.loaded = true;
                     t(e)
                 }
             };
             if (n) {
                 setTimeout(i, n)
             } else {
                 i()
             }
         }
 
-        function ut(t, i, e) {
+        function mt(t, i, e) {
             var a = false;
-            G(n, function(r) {
-                if (o(t, "hx-" + r)) {
-                    var n = V(t, "hx-" + r);
+            Q(R, function(r) {
+                if (q(t, "hx-" + r)) {
+                    var n = G(t, "hx-" + r);
                     a = true;
                     i.path = n;
                     i.verb = r;
                     e.forEach(function(e) {
-                        ft(t, e, i, function(e, t) {
-                            lr(r, n, e, t)
+                        xt(t, e, i, function(e, t) {
+                            ae(r, n, e, t)
                         })
                     })
                 }
             });
             return a
         }
 
-        function ft(n, e, t, r) {
+        function xt(n, e, t, r) {
             if (e.sseEvent) {
-                at(n, r, e.sseEvent)
+                dt(n, r, e.sseEvent)
             } else if (e.trigger === "revealed") {
-                $e();
-                We(n, r, t, e);
-                Ze(n)
+                nt();
+                et(n, r, t, e);
+                it(n)
             } else if (e.trigger === "intersect") {
                 var i = {};
                 if (e.root) {
-                    i.root = Q(n, e.root)
+                    i.root = re(n, e.root)
                 }
                 if (e.threshold) {
                     i.threshold = parseFloat(e.threshold)
                 }
                 var a = new IntersectionObserver(function(e) {
                     for (var t = 0; t < e.length; t++) {
                         var r = e[t];
                         if (r.isIntersecting) {
-                            $(n, "intersect");
+                            ie(n, "intersect");
                             break
                         }
                     }
                 }, i);
                 a.observe(n);
-                We(n, r, t, e)
+                et(n, r, t, e)
             } else if (e.trigger === "load") {
-                if (!ze(e, yt("load", {
+                if (!Qe(e, Lt("load", {
                         elt: n
                     }))) {
-                    lt(n, r, t, e.delay)
+                    pt(n, r, t, e.delay)
                 }
             } else if (e.pollInterval) {
                 t.polling = true;
-                je(n, r, e)
+                Ge(n, r, e)
             } else {
-                We(n, r, t, e)
+                et(n, r, t, e)
             }
         }
 
-        function ct(e) {
+        function yt(e) {
             if (e.type === "text/javascript" || e.type === "module" || e.type === "") {
-                var t = _().createElement("script");
-                G(e.attributes, function(e) {
+                var t = J().createElement("script");
+                Q(e.attributes, function(e) {
                     t.setAttribute(e.name, e.value)
                 });
                 t.textContent = e.textContent;
                 t.async = false;
-                if (U.config.inlineScriptNonce) {
-                    t.nonce = U.config.inlineScriptNonce
+                if (z.config.inlineScriptNonce) {
+                    t.nonce = z.config.inlineScriptNonce
                 }
                 var r = e.parentElement;
                 try {
                     r.insertBefore(t, e)
                 } catch (e) {
-                    St(e)
+                    x(e)
                 } finally {
-                    r.removeChild(e)
+                    if (e.parentElement) {
+                        e.parentElement.removeChild(e)
+                    }
                 }
             }
         }
 
-        function ht(e) {
-            if (d(e, "script")) {
-                ct(e)
+        function bt(e) {
+            if (h(e, "script")) {
+                yt(e)
             }
-            G(O(e, "script"), function(e) {
-                ct(e)
+            Q(f(e, "script"), function(e) {
+                yt(e)
             })
         }
 
-        function dt() {
+        function wt() {
             return document.querySelector("[hx-boost], [data-hx-boost]")
         }
 
-        function vt(e) {
+        function St(e) {
             if (e.querySelectorAll) {
-                var t = dt() ? ", a, form" : "";
-                var r = e.querySelectorAll(i + t + ", [hx-sse], [data-hx-sse], [hx-ws]," + " [data-hx-ws], [hx-ext], [data-hx-ext]");
+                var t = wt() ? ", a, form" : "";
+                var r = e.querySelectorAll(O + t + ", [hx-sse], [data-hx-sse], [hx-ws]," + " [data-hx-ws], [hx-ext], [data-hx-ext], [hx-trigger], [data-hx-trigger], [hx-on], [data-hx-on]");
                 return r
             } else {
                 return []
             }
         }
 
-        function gt(r) {
+        function Et(n) {
             var e = function(e) {
-                if (d(e.target, "button, input[type='submit']")) {
-                    var t = W(r);
-                    t.lastButtonClicked = e.target
+                var t = d(e.target, "button, input[type='submit']");
+                if (t !== null) {
+                    var r = Y(n);
+                    r.lastButtonClicked = t
                 }
             };
-            r.addEventListener("click", e);
-            r.addEventListener("focusin", e);
-            r.addEventListener("focusout", function(e) {
-                var t = W(r);
+            n.addEventListener("click", e);
+            n.addEventListener("focusin", e);
+            n.addEventListener("focusout", function(e) {
+                var t = Y(n);
                 t.lastButtonClicked = null
             })
         }
 
-        function pt(e) {
-            if (e.closest && e.closest(U.config.disableSelector)) {
+        function Ct(e) {
+            var t = Ue(e);
+            var r = 0;
+            for (let e = 0; e < t.length; e++) {
+                const n = t[e];
+                if (n === "{") {
+                    r++
+                } else if (n === "}") {
+                    r--
+                }
+            }
+            return r
+        }
+
+        function Rt(t, e, r) {
+            var n = Y(t);
+            n.onHandlers = [];
+            var i = new Function("event", r + "; return;");
+            var a = t.addEventListener(e, function(e) {
+                return i.call(t, e)
+            });
+            n.onHandlers.push({
+                event: e,
+                listener: a
+            });
+            return {
+                nodeData: n,
+                code: r,
+                func: i,
+                listener: a
+            }
+        }
+
+        function Ot(e) {
+            var t = G(e, "hx-on");
+            if (t) {
+                var r = {};
+                var n = t.split("\n");
+                var i = null;
+                var a = 0;
+                while (n.length > 0) {
+                    var o = n.shift();
+                    var s = o.match(/^\s*([a-zA-Z:\-]+:)(.*)/);
+                    if (a === 0 && s) {
+                        o.split(":");
+                        i = s[1].slice(0, -1);
+                        r[i] = s[2]
+                    } else {
+                        r[i] += o
+                    }
+                    a += Ct(o)
+                }
+                for (var l in r) {
+                    Rt(e, l, r[l])
+                }
+            }
+        }
+
+        function qt(t) {
+            if (t.closest && t.closest(z.config.disableSelector)) {
                 return
             }
-            var t = W(e);
-            if (t.initHash !== de(e)) {
-                t.initHash = de(e);
-                ve(e);
-                $(e, "htmx:beforeProcessNode");
-                if (e.value) {
-                    t.lastValue = e.value
-                }
-                var r = Xe(e);
-                var n = ut(e, t, r);
-                if (!n && z(e, "hx-boost") === "true") {
-                    Ue(e, t, r)
+            var r = Y(t);
+            if (r.initHash !== Ce(t)) {
+                r.initHash = Ce(t);
+                Re(t);
+                Ot(t);
+                ie(t, "htmx:beforeProcessNode");
+                if (t.value) {
+                    r.lastValue = t.value
+                }
+                var e = ze(t);
+                var n = mt(t, r, e);
+                if (!n) {
+                    if (Z(t, "hx-boost") === "true") {
+                        Ze(t, r, e)
+                    } else if (q(t, "hx-trigger")) {
+                        e.forEach(function(e) {
+                            xt(t, e, r, function() {})
+                        })
+                    }
                 }
-                if (e.tagName === "FORM") {
-                    gt(e)
+                if (t.tagName === "FORM") {
+                    Et(t)
                 }
-                var i = V(e, "hx-sse");
+                var i = G(t, "hx-sse");
                 if (i) {
-                    rt(e, t, i)
+                    ft(t, r, i)
                 }
-                var a = V(e, "hx-ws");
+                var a = G(t, "hx-ws");
                 if (a) {
-                    Ke(e, t, a)
+                    at(t, r, a)
                 }
-                $(e, "htmx:afterProcessNode")
+                ie(t, "htmx:afterProcessNode")
             }
         }
 
-        function mt(e) {
-            e = D(e);
-            pt(e);
-            G(vt(e), function(e) {
-                pt(e)
+        function Tt(e) {
+            e = s(e);
+            qt(e);
+            Q(St(e), function(e) {
+                qt(e)
             })
         }
 
-        function xt(e) {
+        function Ht(e) {
             return e.replace(/([a-z0-9])([A-Z])/g, "$1-$2").toLowerCase()
         }
 
-        function yt(e, t) {
+        function Lt(e, t) {
             var r;
             if (window.CustomEvent && typeof window.CustomEvent === "function") {
                 r = new CustomEvent(e, {
                     bubbles: true,
                     cancelable: true,
                     detail: t
                 })
             } else {
-                r = _().createEvent("CustomEvent");
+                r = J().createEvent("CustomEvent");
                 r.initCustomEvent(e, true, true, t)
             }
             return r
         }
 
-        function J(e, t, r) {
-            $(e, t, Y({
+        function ne(e, t, r) {
+            ie(e, t, te({
                 error: t
             }, r))
         }
 
-        function bt(e) {
+        function At(e) {
             return e === "htmx:afterProcessNode"
         }
 
-        function wt(e, t) {
-            G(gr(e), function(e) {
+        function w(e, t) {
+            Q(wr(e), function(e) {
                 try {
                     t(e)
                 } catch (e) {
-                    St(e)
+                    x(e)
                 }
             })
         }
 
-        function St(e) {
+        function x(e) {
             if (console.error) {
                 console.error(e)
             } else if (console.log) {
                 console.log("ERROR: ", e)
             }
         }
 
-        function $(e, t, r) {
-            e = D(e);
+        function ie(e, t, r) {
+            e = s(e);
             if (r == null) {
                 r = {}
             }
             r["elt"] = e;
-            var n = yt(t, r);
-            if (U.logger && !bt(t)) {
-                U.logger(e, t, r)
+            var n = Lt(t, r);
+            if (z.logger && !At(t)) {
+                z.logger(e, t, r)
             }
             if (r.error) {
-                St(r.error);
-                $(e, "htmx:error", {
+                x(r.error);
+                ie(e, "htmx:error", {
                     errorInfo: r
                 })
             }
             var i = e.dispatchEvent(n);
-            var a = xt(t);
+            var a = Ht(t);
             if (i && a !== t) {
-                var o = yt(a, n.detail);
+                var o = Lt(a, n.detail);
                 i = i && e.dispatchEvent(o)
             }
-            wt(e, function(e) {
+            w(e, function(e) {
                 i = i && e.onEvent(t, n) !== false
             });
             return i
         }
-        var Et = location.pathname + location.search;
+        var Nt = location.pathname + location.search;
 
-        function Ct() {
-            var e = _().querySelector("[hx-history-elt],[data-hx-history-elt]");
-            return e || _().body
+        function It() {
+            var e = J().querySelector("[hx-history-elt],[data-hx-history-elt]");
+            return e || J().body
         }
 
-        function Rt(e, t, r, n) {
-            if (!E()) {
+        function kt(e, t, r, n) {
+            if (!D()) {
                 return
             }
-            var i = S(localStorage.getItem("htmx-history-cache")) || [];
+            e = X(e);
+            var i = y(localStorage.getItem("htmx-history-cache")) || [];
             for (var a = 0; a < i.length; a++) {
                 if (i[a].url === e) {
                     i.splice(a, 1);
                     break
                 }
             }
-            i.push({
+            var o = {
                 url: e,
                 content: t,
                 title: r,
                 scroll: n
+            };
+            ie(J().body, "htmx:historyItemCreated", {
+                item: o,
+                cache: i
             });
-            while (i.length > U.config.historyCacheSize) {
+            i.push(o);
+            while (i.length > z.config.historyCacheSize) {
                 i.shift()
             }
             while (i.length > 0) {
                 try {
                     localStorage.setItem("htmx-history-cache", JSON.stringify(i));
                     break
                 } catch (e) {
-                    J(_().body, "htmx:historyCacheError", {
+                    ne(J().body, "htmx:historyCacheError", {
                         cause: e,
                         cache: i
                     });
                     i.shift()
                 }
             }
         }
 
-        function Ot(e) {
-            if (!E()) {
+        function Pt(e) {
+            if (!D()) {
                 return null
             }
-            var t = S(localStorage.getItem("htmx-history-cache")) || [];
+            e = X(e);
+            var t = y(localStorage.getItem("htmx-history-cache")) || [];
             for (var r = 0; r < t.length; r++) {
                 if (t[r].url === e) {
                     return t[r]
                 }
             }
             return null
         }
 
-        function qt(e) {
-            var t = U.config.requestClass;
+        function Mt(e) {
+            var t = z.config.requestClass;
             var r = e.cloneNode(true);
-            G(O(r, "." + t), function(e) {
-                T(e, t)
+            Q(f(r, "." + t), function(e) {
+                n(e, t)
             });
             return r.innerHTML
         }
 
-        function Lt() {
-            var e = Ct();
-            var t = Et || location.pathname + location.search;
-            $(_().body, "htmx:beforeHistorySave", {
-                path: t,
-                historyElt: e
-            });
-            if (U.config.historyEnabled) history.replaceState({
+        function Dt() {
+            var e = It();
+            var t = Nt || location.pathname + location.search;
+            var r = J().querySelector('[hx-history="false" i],[data-hx-history="false" i]');
+            if (!r) {
+                ie(J().body, "htmx:beforeHistorySave", {
+                    path: t,
+                    historyElt: e
+                });
+                kt(t, Mt(e), J().title, window.scrollY)
+            }
+            if (z.config.historyEnabled) history.replaceState({
                 htmx: true
-            }, _().title, window.location.href);
-            Rt(t, qt(e), _().title, window.scrollY)
+            }, J().title, window.location.href)
         }
 
-        function Tt(e) {
-            if (U.config.historyEnabled) history.pushState({
-                htmx: true
-            }, "", e);
-            Et = e
+        function Xt(e) {
+            if (z.config.getCacheBusterParam) {
+                e = e.replace(/org\.htmx\.cache-buster=[^&]*&?/, "");
+                if (e.endsWith("&") || e.endsWith("?")) {
+                    e = e.slice(0, -1)
+                }
+            }
+            if (z.config.historyEnabled) {
+                history.pushState({
+                    htmx: true
+                }, "", e)
+            }
+            Nt = e
         }
 
-        function Ht(e) {
-            if (U.config.historyEnabled) history.replaceState({
+        function Ft(e) {
+            if (z.config.historyEnabled) history.replaceState({
                 htmx: true
             }, "", e);
-            Et = e
+            Nt = e
         }
 
-        function At(e) {
-            G(e, function(e) {
+        function Bt(e) {
+            Q(e, function(e) {
                 e.call()
             })
         }
 
-        function Nt(a) {
+        function jt(a) {
             var e = new XMLHttpRequest;
             var o = {
                 path: a,
                 xhr: e
             };
-            $(_().body, "htmx:historyCacheMiss", o);
+            ie(J().body, "htmx:historyCacheMiss", o);
             e.open("GET", a, true);
             e.setRequestHeader("HX-History-Restore-Request", "true");
             e.onload = function() {
                 if (this.status >= 200 && this.status < 400) {
-                    $(_().body, "htmx:historyCacheMissLoad", o);
-                    var e = g(this.response);
+                    ie(J().body, "htmx:historyCacheMissLoad", o);
+                    var e = l(this.response);
                     e = e.querySelector("[hx-history-elt],[data-hx-history-elt]") || e;
-                    var t = Ct();
-                    var r = Zt(t);
-                    var n = Re(this.response);
+                    var t = It();
+                    var r = S(t);
+                    var n = Pe(this.response);
                     if (n) {
-                        var i = R("title");
+                        var i = b("title");
                         if (i) {
                             i.innerHTML = n
                         } else {
                             window.document.title = n
                         }
                     }
-                    Se(t, e, r);
-                    At(r.tasks);
-                    Et = a;
-                    $(_().body, "htmx:historyRestore", {
-                        path: a
+                    Ne(t, e, r);
+                    Bt(r.tasks);
+                    Nt = a;
+                    ie(J().body, "htmx:historyRestore", {
+                        path: a,
+                        cacheMiss: true,
+                        serverResponse: this.response
                     })
                 } else {
-                    J(_().body, "htmx:historyCacheMissLoadError", o)
+                    ne(J().body, "htmx:historyCacheMissLoadError", o)
                 }
             };
             e.send()
         }
 
-        function It(e) {
-            Lt();
+        function Ut(e) {
+            Dt();
             e = e || location.pathname + location.search;
-            var t = Ot(e);
+            var t = Pt(e);
             if (t) {
-                var r = g(t.content);
-                var n = Ct();
-                var i = Zt(n);
-                Se(n, r, i);
-                At(i.tasks);
+                var r = l(t.content);
+                var n = It();
+                var i = S(n);
+                Ne(n, r, i);
+                Bt(i.tasks);
                 document.title = t.title;
                 window.scrollTo(0, t.scroll);
-                Et = e;
-                $(_().body, "htmx:historyRestore", {
-                    path: e
+                Nt = e;
+                ie(J().body, "htmx:historyRestore", {
+                    path: e,
+                    item: t
                 })
             } else {
-                if (U.config.refreshOnHistoryMiss) {
+                if (z.config.refreshOnHistoryMiss) {
                     window.location.reload(true)
                 } else {
-                    Nt(e)
+                    jt(e)
                 }
             }
         }
 
-        function kt(e) {
-            var t = j(e, "hx-indicator");
+        function Vt(e) {
+            var t = ce(e, "hx-indicator");
             if (t == null) {
                 t = [e]
             }
-            G(t, function(e) {
-                var t = W(e);
+            Q(t, function(e) {
+                var t = Y(e);
                 t.requestCount = (t.requestCount || 0) + 1;
-                e.classList["add"].call(e.classList, U.config.requestClass)
+                e.classList["add"].call(e.classList, z.config.requestClass)
             });
             return t
         }
 
-        function Mt(e) {
-            G(e, function(e) {
-                var t = W(e);
+        function _t(e) {
+            Q(e, function(e) {
+                var t = Y(e);
                 t.requestCount = (t.requestCount || 0) - 1;
                 if (t.requestCount === 0) {
-                    e.classList["remove"].call(e.classList, U.config.requestClass)
+                    e.classList["remove"].call(e.classList, z.config.requestClass)
                 }
             })
         }
 
-        function Dt(e, t) {
+        function Wt(e, t) {
             for (var r = 0; r < e.length; r++) {
                 var n = e[r];
                 if (n.isSameNode(t)) {
                     return true
                 }
             }
             return false
         }
 
-        function Pt(e) {
+        function zt(e) {
             if (e.name === "" || e.name == null || e.disabled) {
                 return false
             }
             if (e.type === "button" || e.type === "submit" || e.tagName === "image" || e.tagName === "reset" || e.tagName === "file") {
                 return false
             }
             if (e.type === "checkbox" || e.type === "radio") {
                 return e.checked
             }
             return true
         }
 
-        function Xt(t, r, n, e, i) {
-            if (e == null || Dt(t, e)) {
+        function $t(t, r, n, e, i) {
+            if (e == null || Wt(t, e)) {
                 return
             } else {
                 t.push(e)
             }
-            if (Pt(e)) {
-                var a = f(e, "name");
+            if (zt(e)) {
+                var a = $(e, "name");
                 var o = e.value;
                 if (e.multiple) {
-                    o = y(e.querySelectorAll("option:checked")).map(function(e) {
+                    o = k(e.querySelectorAll("option:checked")).map(function(e) {
                         return e.value
                     })
                 }
                 if (e.files) {
-                    o = y(e.files)
+                    o = k(e.files)
                 }
                 if (a != null && o != null) {
                     var s = r[a];
-                    if (s) {
+                    if (s !== undefined) {
                         if (Array.isArray(s)) {
                             if (Array.isArray(o)) {
                                 r[a] = s.concat(o)
                             } else {
                                 s.push(o)
                             }
                         } else {
@@ -1989,256 +2135,259 @@
                             }
                         }
                     } else {
                         r[a] = o
                     }
                 }
                 if (i) {
-                    Ft(e, n)
+                    Gt(e, n)
                 }
             }
-            if (d(e, "form")) {
+            if (h(e, "form")) {
                 var l = e.elements;
-                G(l, function(e) {
-                    Xt(t, r, n, e, i)
+                Q(l, function(e) {
+                    $t(t, r, n, e, i)
                 })
             }
         }
 
-        function Ft(e, t) {
+        function Gt(e, t) {
             if (e.willValidate) {
-                $(e, "htmx:validation:validate");
+                ie(e, "htmx:validation:validate");
                 if (!e.checkValidity()) {
                     t.push({
                         elt: e,
                         message: e.validationMessage,
                         validity: e.validity
                     });
-                    $(e, "htmx:validation:failed", {
+                    ie(e, "htmx:validation:failed", {
                         message: e.validationMessage,
                         validity: e.validity
                     })
                 }
             }
         }
 
-        function jt(e, t) {
+        function Jt(e, t) {
             var r = [];
             var n = {};
             var i = {};
             var a = [];
-            var o = W(e);
-            var s = d(e, "form") && e.noValidate !== true || V(e, "hx-validate") === "true";
+            var o = Y(e);
+            var s = h(e, "form") && e.noValidate !== true || G(e, "hx-validate") === "true";
             if (o.lastButtonClicked) {
                 s = s && o.lastButtonClicked.formNoValidate !== true
             }
             if (t !== "get") {
-                Xt(r, i, a, N(e, "form"), s)
+                $t(r, i, a, d(e, "form"), s)
             }
-            Xt(r, n, a, e, s);
+            $t(r, n, a, e, s);
             if (o.lastButtonClicked) {
-                var l = f(o.lastButtonClicked, "name");
+                var l = $(o.lastButtonClicked, "name");
                 if (l) {
                     n[l] = o.lastButtonClicked.value
                 }
             }
-            var u = j(e, "hx-include");
-            G(u, function(e) {
-                Xt(r, n, a, e, s);
-                if (!d(e, "form")) {
-                    G(e.querySelectorAll(Pe), function(e) {
-                        Xt(r, n, a, e, s)
+            var u = ce(e, "hx-include");
+            Q(u, function(e) {
+                $t(r, n, a, e, s);
+                if (!h(e, "form")) {
+                    Q(e.querySelectorAll(We), function(e) {
+                        $t(r, n, a, e, s)
                     })
                 }
             });
-            n = Y(n, i);
+            n = te(n, i);
             return {
                 errors: a,
                 values: n
             }
         }
 
-        function Bt(e, t, r) {
+        function Zt(e, t, r) {
             if (e !== "") {
                 e += "&"
             }
             if (String(r) === "[object Object]") {
                 r = JSON.stringify(r)
             }
             var n = encodeURIComponent(r);
             e += encodeURIComponent(t) + "=" + n;
             return e
         }
 
-        function Ut(e) {
+        function Kt(e) {
             var t = "";
             for (var r in e) {
                 if (e.hasOwnProperty(r)) {
                     var n = e[r];
                     if (Array.isArray(n)) {
-                        G(n, function(e) {
-                            t = Bt(t, r, e)
+                        Q(n, function(e) {
+                            t = Zt(t, r, e)
                         })
                     } else {
-                        t = Bt(t, r, n)
+                        t = Zt(t, r, n)
                     }
                 }
             }
             return t
         }
 
-        function Vt(e) {
+        function Yt(e) {
             var t = new FormData;
             for (var r in e) {
                 if (e.hasOwnProperty(r)) {
                     var n = e[r];
                     if (Array.isArray(n)) {
-                        G(n, function(e) {
+                        Q(n, function(e) {
                             t.append(r, e)
                         })
                     } else {
                         t.append(r, n)
                     }
                 }
             }
             return t
         }
 
-        function _t(e, t, r) {
+        function Qt(e, t, r) {
             var n = {
                 "HX-Request": "true",
-                "HX-Trigger": f(e, "id"),
-                "HX-Trigger-Name": f(e, "name"),
-                "HX-Target": V(t, "id"),
-                "HX-Current-URL": _().location.href
+                "HX-Trigger": $(e, "id"),
+                "HX-Trigger-Name": $(e, "name"),
+                "HX-Target": G(t, "id"),
+                "HX-Current-URL": J().location.href
             };
-            Yt(e, "hx-headers", false, n);
+            or(e, "hx-headers", false, n);
             if (r !== undefined) {
                 n["HX-Prompt"] = r
             }
-            if (W(e).boosted) {
+            if (Y(e).boosted) {
                 n["HX-Boosted"] = "true"
             }
             return n
         }
 
-        function zt(t, e) {
-            var r = z(e, "hx-params");
+        function er(t, e) {
+            var r = Z(e, "hx-params");
             if (r) {
                 if (r === "none") {
                     return {}
                 } else if (r === "*") {
                     return t
                 } else if (r.indexOf("not ") === 0) {
-                    G(r.substr(4).split(","), function(e) {
+                    Q(r.substr(4).split(","), function(e) {
                         e = e.trim();
                         delete t[e]
                     });
                     return t
                 } else {
                     var n = {};
-                    G(r.split(","), function(e) {
+                    Q(r.split(","), function(e) {
                         e = e.trim();
                         n[e] = t[e]
                     });
                     return n
                 }
             } else {
                 return t
             }
         }
 
-        function Wt(e) {
-            return f(e, "href") && f(e, "href").indexOf("#") >= 0
+        function tr(e) {
+            return $(e, "href") && $(e, "href").indexOf("#") >= 0
         }
 
-        function Gt(e, t) {
-            var r = t ? t : z(e, "hx-swap");
+        function rr(e, t) {
+            var r = t ? t : Z(e, "hx-swap");
             var n = {
-                swapStyle: W(e).boosted ? "innerHTML" : U.config.defaultSwapStyle,
-                swapDelay: U.config.defaultSwapDelay,
-                settleDelay: U.config.defaultSettleDelay
+                swapStyle: Y(e).boosted ? "innerHTML" : z.config.defaultSwapStyle,
+                swapDelay: z.config.defaultSwapDelay,
+                settleDelay: z.config.defaultSettleDelay
             };
-            if (W(e).boosted && !Wt(e)) {
+            if (Y(e).boosted && !tr(e)) {
                 n["show"] = "top"
             }
             if (r) {
-                var i = w(r);
+                var i = M(r);
                 if (i.length > 0) {
                     n["swapStyle"] = i[0];
                     for (var a = 1; a < i.length; a++) {
                         var o = i[a];
                         if (o.indexOf("swap:") === 0) {
                             n["swapDelay"] = v(o.substr(5))
                         }
                         if (o.indexOf("settle:") === 0) {
                             n["settleDelay"] = v(o.substr(7))
                         }
+                        if (o.indexOf("transition:") === 0) {
+                            n["transition"] = o.substr(11) === "true"
+                        }
                         if (o.indexOf("scroll:") === 0) {
                             var s = o.substr(7);
                             var l = s.split(":");
-                            var f = l.pop();
-                            var u = l.length > 0 ? l.join(":") : null;
-                            n["scroll"] = f;
-                            n["scrollTarget"] = u
+                            var u = l.pop();
+                            var f = l.length > 0 ? l.join(":") : null;
+                            n["scroll"] = u;
+                            n["scrollTarget"] = f
                         }
                         if (o.indexOf("show:") === 0) {
                             var c = o.substr(5);
                             var l = c.split(":");
                             var h = l.pop();
-                            var u = l.length > 0 ? l.join(":") : null;
+                            var f = l.length > 0 ? l.join(":") : null;
                             n["show"] = h;
-                            n["showTarget"] = u
+                            n["showTarget"] = f
                         }
                         if (o.indexOf("focus-scroll:") === 0) {
                             var d = o.substr("focus-scroll:".length);
                             n["focusScroll"] = d == "true"
                         }
                     }
                 }
             }
             return n
         }
 
-        function Jt(e) {
-            return z(e, "hx-encoding") === "multipart/form-data" || d(e, "form") && f(e, "enctype") === "multipart/form-data"
+        function nr(e) {
+            return Z(e, "hx-encoding") === "multipart/form-data" || h(e, "form") && $(e, "enctype") === "multipart/form-data"
         }
 
-        function $t(t, r, n) {
+        function ir(t, r, n) {
             var i = null;
-            wt(r, function(e) {
+            w(r, function(e) {
                 if (i == null) {
                     i = e.encodeParameters(t, n, r)
                 }
             });
             if (i != null) {
                 return i
             } else {
-                if (Jt(r)) {
-                    return Vt(n)
+                if (nr(r)) {
+                    return Yt(n)
                 } else {
-                    return Ut(n)
+                    return Kt(n)
                 }
             }
         }
 
-        function Zt(e) {
+        function S(e) {
             return {
                 tasks: [],
                 elts: [e]
             }
         }
 
-        function Kt(e, t) {
+        function ar(e, t) {
             var r = e[0];
             var n = e[e.length - 1];
             if (t.scroll) {
                 var i = null;
                 if (t.scrollTarget) {
-                    i = Q(r, t.scrollTarget)
+                    i = re(r, t.scrollTarget)
                 }
                 if (t.scroll === "top" && (r || i)) {
                     i = i || r;
                     i.scrollTop = 0
                 }
                 if (t.scroll === "bottom" && (n || i)) {
                     i = i || n;
@@ -2248,41 +2397,41 @@
             if (t.show) {
                 var i = null;
                 if (t.showTarget) {
                     var a = t.showTarget;
                     if (t.showTarget === "window") {
                         a = "body"
                     }
-                    i = Q(r, a)
+                    i = re(r, a)
                 }
                 if (t.show === "top" && (r || i)) {
                     i = i || r;
                     i.scrollIntoView({
                         block: "start",
-                        behavior: U.config.scrollBehavior
+                        behavior: z.config.scrollBehavior
                     })
                 }
                 if (t.show === "bottom" && (n || i)) {
                     i = i || n;
                     i.scrollIntoView({
                         block: "end",
-                        behavior: U.config.scrollBehavior
+                        behavior: z.config.scrollBehavior
                     })
                 }
             }
         }
 
-        function Yt(e, t, r, n) {
+        function or(e, t, r, n) {
             if (n == null) {
                 n = {}
             }
             if (e == null) {
                 return n
             }
-            var i = V(e, t);
+            var i = G(e, t);
             if (i) {
                 var a = i.trim();
                 var o = r;
                 if (a === "unset") {
                     return null
                 }
                 if (a.indexOf("javascript:") === 0) {
@@ -2293,410 +2442,433 @@
                     o = true
                 }
                 if (a.indexOf("{") !== 0) {
                     a = "{" + a + "}"
                 }
                 var s;
                 if (o) {
-                    s = Qt(e, function() {
+                    s = sr(e, function() {
                         return Function("return (" + a + ")")()
                     }, {})
                 } else {
-                    s = S(a)
+                    s = y(a)
                 }
                 for (var l in s) {
                     if (s.hasOwnProperty(l)) {
                         if (n[l] == null) {
                             n[l] = s[l]
                         }
                     }
                 }
             }
-            return Yt(u(e), t, r, n)
+            return or(u(e), t, r, n)
         }
 
-        function Qt(e, t, r) {
-            if (U.config.allowEval) {
+        function sr(e, t, r) {
+            if (z.config.allowEval) {
                 return t()
             } else {
-                J(e, "htmx:evalDisallowedError");
+                ne(e, "htmx:evalDisallowedError");
                 return r
             }
         }
 
-        function er(e, t) {
-            return Yt(e, "hx-vars", true, t)
+        function lr(e, t) {
+            return or(e, "hx-vars", true, t)
         }
 
-        function tr(e, t) {
-            return Yt(e, "hx-vals", false, t)
+        function ur(e, t) {
+            return or(e, "hx-vals", false, t)
         }
 
-        function rr(e) {
-            return Y(er(e), tr(e))
+        function fr(e) {
+            return te(lr(e), ur(e))
         }
 
-        function nr(t, r, n) {
+        function cr(t, r, n) {
             if (n !== null) {
                 try {
                     t.setRequestHeader(r, n)
                 } catch (e) {
                     t.setRequestHeader(r, encodeURIComponent(n));
                     t.setRequestHeader(r + "-URI-AutoEncoded", "true")
                 }
             }
         }
 
-        function ir(t) {
+        function hr(t) {
             if (t.responseURL && typeof URL !== "undefined") {
                 try {
                     var e = new URL(t.responseURL);
                     return e.pathname + e.search
                 } catch (e) {
-                    J(_().body, "htmx:badResponseUrl", {
+                    ne(J().body, "htmx:badResponseUrl", {
                         url: t.responseURL
                     })
                 }
             }
         }
 
-        function ar(e, t) {
+        function E(e, t) {
             return e.getAllResponseHeaders().match(t)
         }
 
-        function or(e, t, r) {
+        function dr(e, t, r) {
             e = e.toLowerCase();
             if (r) {
-                if (r instanceof Element || p(r, "String")) {
-                    return lr(e, t, null, null, {
-                        targetOverride: D(r),
+                if (r instanceof Element || A(r, "String")) {
+                    return ae(e, t, null, null, {
+                        targetOverride: s(r),
                         returnPromise: true
                     })
                 } else {
-                    return lr(e, t, D(r.source), r.event, {
+                    return ae(e, t, s(r.source), r.event, {
                         handler: r.handler,
                         headers: r.headers,
                         values: r.values,
-                        targetOverride: D(r.target),
+                        targetOverride: s(r.target),
                         swapOverride: r.swap,
                         returnPromise: true
                     })
                 }
             } else {
-                return lr(e, t, null, null, {
+                return ae(e, t, null, null, {
                     returnPromise: true
                 })
             }
         }
 
-        function sr(e) {
+        function vr(e) {
             var t = [];
             while (e) {
                 t.push(e);
                 e = e.parentElement
             }
             return t
         }
 
-        function lr(e, t, n, f, r) {
-            var c = null;
-            var h = null;
-            r = r != null ? r : {};
-            if (r.returnPromise && typeof Promise !== "undefined") {
-                var d = new Promise(function(e, t) {
-                    c = e;
-                    h = t
+        function ae(e, t, n, r, i, M) {
+            var a = null;
+            var o = null;
+            i = i != null ? i : {};
+            if (i.returnPromise && typeof Promise !== "undefined") {
+                var s = new Promise(function(e, t) {
+                    a = e;
+                    o = t
                 })
             }
             if (n == null) {
-                n = _().body
+                n = J().body
             }
-            var v = r.handler || fr;
-            if (!K(n)) {
+            var D = i.handler || pr;
+            if (!ee(n)) {
                 return
             }
-            var g = r.targetOverride || re(n);
-            if (g == null || g == ee) {
-                J(n, "htmx:targetError", {
-                    target: V(n, "hx-target")
+            var l = i.targetOverride || de(n);
+            if (l == null || l == fe) {
+                ne(n, "htmx:targetError", {
+                    target: G(n, "hx-target")
                 });
                 return
             }
-            var p = n;
-            var i = W(n);
-            var a = z(n, "hx-sync");
-            var m = null;
-            var x = false;
-            if (a) {
-                var y = a.split(":");
-                var b = y[0].trim();
-                if (b === "this") {
-                    p = te(n, "hx-sync")
+            if (!M) {
+                var X = function() {
+                    return ae(e, t, n, r, i, true)
+                };
+                var F = {
+                    target: l,
+                    elt: n,
+                    path: t,
+                    verb: e,
+                    triggeringEvent: r,
+                    etc: i,
+                    issueRequest: X
+                };
+                if (ie(n, "htmx:confirm", F) === false) {
+                    return
+                }
+            }
+            var u = n;
+            var f = Y(n);
+            var c = Z(n, "hx-sync");
+            var h = null;
+            var d = false;
+            if (c) {
+                var v = c.split(":");
+                var g = v[0].trim();
+                if (g === "this") {
+                    u = he(n, "hx-sync")
                 } else {
-                    p = Q(n, b)
+                    u = re(n, g)
                 }
-                a = (y[1] || "drop").trim();
-                i = W(p);
-                if (a === "drop" && i.xhr && i.abortable !== true) {
+                c = (v[1] || "drop").trim();
+                f = Y(u);
+                if (c === "drop" && f.xhr && f.abortable !== true) {
                     return
-                } else if (a === "abort") {
-                    if (i.xhr) {
+                } else if (c === "abort") {
+                    if (f.xhr) {
                         return
                     } else {
-                        x = true
+                        d = true
                     }
-                } else if (a === "replace") {
-                    $(p, "htmx:abort")
-                } else if (a.indexOf("queue") === 0) {
-                    var w = a.split(" ");
-                    m = (w[1] || "last").trim()
+                } else if (c === "replace") {
+                    ie(u, "htmx:abort")
+                } else if (c.indexOf("queue") === 0) {
+                    var B = c.split(" ");
+                    h = (B[1] || "last").trim()
                 }
             }
-            if (i.xhr) {
-                if (i.abortable) {
-                    $(p, "htmx:abort")
+            if (f.xhr) {
+                if (f.abortable) {
+                    ie(u, "htmx:abort")
                 } else {
-                    if (m == null) {
-                        if (f) {
-                            var S = W(f);
-                            if (S && S.triggerSpec && S.triggerSpec.queue) {
-                                m = S.triggerSpec.queue
+                    if (h == null) {
+                        if (r) {
+                            var p = Y(r);
+                            if (p && p.triggerSpec && p.triggerSpec.queue) {
+                                h = p.triggerSpec.queue
                             }
                         }
-                        if (m == null) {
-                            m = "last"
+                        if (h == null) {
+                            h = "last"
                         }
                     }
-                    if (i.queuedRequests == null) {
-                        i.queuedRequests = []
+                    if (f.queuedRequests == null) {
+                        f.queuedRequests = []
                     }
-                    if (m === "first" && i.queuedRequests.length === 0) {
-                        i.queuedRequests.push(function() {
-                            lr(e, t, n, f, r)
+                    if (h === "first" && f.queuedRequests.length === 0) {
+                        f.queuedRequests.push(function() {
+                            ae(e, t, n, r, i)
                         })
-                    } else if (m === "all") {
-                        i.queuedRequests.push(function() {
-                            lr(e, t, n, f, r)
+                    } else if (h === "all") {
+                        f.queuedRequests.push(function() {
+                            ae(e, t, n, r, i)
                         })
-                    } else if (m === "last") {
-                        i.queuedRequests = [];
-                        i.queuedRequests.push(function() {
-                            lr(e, t, n, f, r)
+                    } else if (h === "last") {
+                        f.queuedRequests = [];
+                        f.queuedRequests.push(function() {
+                            ae(e, t, n, r, i)
                         })
                     }
                     return
                 }
             }
-            var o = new XMLHttpRequest;
-            i.xhr = o;
-            i.abortable = x;
-            var s = function() {
-                i.xhr = null;
-                i.abortable = false;
-                if (i.queuedRequests != null && i.queuedRequests.length > 0) {
-                    var e = i.queuedRequests.shift();
+            var m = new XMLHttpRequest;
+            f.xhr = m;
+            f.abortable = d;
+            var x = function() {
+                f.xhr = null;
+                f.abortable = false;
+                if (f.queuedRequests != null && f.queuedRequests.length > 0) {
+                    var e = f.queuedRequests.shift();
                     e()
                 }
             };
-            var E = z(n, "hx-prompt");
-            if (E) {
-                var C = prompt(E);
-                if (C === null || !$(n, "htmx:prompt", {
-                        prompt: C,
-                        target: g
+            var y = Z(n, "hx-prompt");
+            if (y) {
+                var b = prompt(y);
+                if (b === null || !ie(n, "htmx:prompt", {
+                        prompt: b,
+                        target: l
                     })) {
-                    Z(c);
-                    s();
-                    return d
-                }
-            }
-            var R = z(n, "hx-confirm");
-            if (R) {
-                if (!confirm(R)) {
-                    Z(c);
-                    s();
-                    return d
-                }
-            }
-            var O = _t(n, g, C);
-            if (r.headers) {
-                O = Y(O, r.headers)
-            }
-            var q = jt(n, e);
-            var L = q.errors;
-            var T = q.values;
-            if (r.values) {
-                T = Y(T, r.values)
-            }
-            var H = rr(n);
-            var A = Y(T, H);
-            var N = zt(A, n);
-            if (e !== "get" && !Jt(n)) {
-                O["Content-Type"] = "application/x-www-form-urlencoded"
+                    K(a);
+                    x();
+                    return s
+                }
+            }
+            var w = Z(n, "hx-confirm");
+            if (w) {
+                if (!confirm(w)) {
+                    K(a);
+                    x();
+                    return s
+                }
+            }
+            var S = Qt(n, l, b);
+            if (i.headers) {
+                S = te(S, i.headers)
+            }
+            var E = Jt(n, e);
+            var C = E.errors;
+            var R = E.values;
+            if (i.values) {
+                R = te(R, i.values)
+            }
+            var j = fr(n);
+            var O = te(R, j);
+            var q = er(O, n);
+            if (e !== "get" && !nr(n)) {
+                S["Content-Type"] = "application/x-www-form-urlencoded"
+            }
+            if (z.config.getCacheBusterParam && e === "get") {
+                q["org.htmx.cache-buster"] = $(l, "id") || "true"
             }
             if (t == null || t === "") {
-                t = _().location.href
+                t = J().location.href
             }
-            var I = Yt(n, "hx-request");
-            var l = {
-                parameters: N,
-                unfilteredParameters: A,
-                headers: O,
-                target: g,
+            var T = or(n, "hx-request");
+            var H = Y(n).boosted;
+            var L = {
+                boosted: H,
+                parameters: q,
+                unfilteredParameters: O,
+                headers: S,
+                target: l,
                 verb: e,
-                errors: L,
-                withCredentials: r.credentials || I.credentials || U.config.withCredentials,
-                timeout: r.timeout || I.timeout || U.config.timeout,
+                errors: C,
+                withCredentials: i.credentials || T.credentials || z.config.withCredentials,
+                timeout: i.timeout || T.timeout || z.config.timeout,
                 path: t,
-                triggeringEvent: f
+                triggeringEvent: r
             };
-            if (!$(n, "htmx:configRequest", l)) {
-                Z(c);
-                s();
-                return d
-            }
-            t = l.path;
-            e = l.verb;
-            O = l.headers;
-            N = l.parameters;
-            L = l.errors;
-            if (L && L.length > 0) {
-                $(n, "htmx:validation:halted", l);
-                Z(c);
-                s();
-                return d
-            }
-            var k = t.split("#");
-            var M = k[0];
-            var D = k[1];
-            var P = null;
+            if (!ie(n, "htmx:configRequest", L)) {
+                K(a);
+                x();
+                return s
+            }
+            t = L.path;
+            e = L.verb;
+            S = L.headers;
+            q = L.parameters;
+            C = L.errors;
+            if (C && C.length > 0) {
+                ie(n, "htmx:validation:halted", L);
+                K(a);
+                x();
+                return s
+            }
+            var U = t.split("#");
+            var V = U[0];
+            var A = U[1];
+            var N = null;
             if (e === "get") {
-                P = M;
-                var X = Object.keys(N).length !== 0;
-                if (X) {
-                    if (P.indexOf("?") < 0) {
-                        P += "?"
+                N = V;
+                var _ = Object.keys(q).length !== 0;
+                if (_) {
+                    if (N.indexOf("?") < 0) {
+                        N += "?"
                     } else {
-                        P += "&"
+                        N += "&"
                     }
-                    P += Ut(N);
-                    if (D) {
-                        P += "#" + D
+                    N += Kt(q);
+                    if (A) {
+                        N += "#" + A
                     }
                 }
-                o.open("GET", P, true)
+                m.open("GET", N, true)
             } else {
-                o.open(e.toUpperCase(), t, true)
+                m.open(e.toUpperCase(), t, true)
             }
-            o.overrideMimeType("text/html");
-            o.withCredentials = l.withCredentials;
-            o.timeout = l.timeout;
-            if (I.noHeaders) {} else {
-                for (var F in O) {
-                    if (O.hasOwnProperty(F)) {
-                        var j = O[F];
-                        nr(o, F, j)
+            m.overrideMimeType("text/html");
+            m.withCredentials = L.withCredentials;
+            m.timeout = L.timeout;
+            if (T.noHeaders) {} else {
+                for (var I in S) {
+                    if (S.hasOwnProperty(I)) {
+                        var W = S[I];
+                        cr(m, I, W)
                     }
                 }
             }
-            var u = {
-                xhr: o,
-                target: g,
-                requestConfig: l,
-                etc: r,
+            var k = {
+                xhr: m,
+                target: l,
+                requestConfig: L,
+                etc: i,
+                boosted: H,
                 pathInfo: {
                     requestPath: t,
-                    finalRequestPath: P || t,
-                    anchor: D
+                    finalRequestPath: N || t,
+                    anchor: A
                 }
             };
-            o.onload = function() {
+            m.onload = function() {
                 try {
-                    var e = sr(n);
-                    u.pathInfo.responsePath = ir(o);
-                    v(n, u);
-                    Mt(B);
-                    $(n, "htmx:afterRequest", u);
-                    $(n, "htmx:afterOnLoad", u);
-                    if (!K(n)) {
+                    var e = vr(n);
+                    k.pathInfo.responsePath = hr(m);
+                    D(n, k);
+                    _t(P);
+                    ie(n, "htmx:afterRequest", k);
+                    ie(n, "htmx:afterOnLoad", k);
+                    if (!ee(n)) {
                         var t = null;
                         while (e.length > 0 && t == null) {
                             var r = e.shift();
-                            if (K(r)) {
+                            if (ee(r)) {
                                 t = r
                             }
                         }
                         if (t) {
-                            $(t, "htmx:afterRequest", u);
-                            $(t, "htmx:afterOnLoad", u)
+                            ie(t, "htmx:afterRequest", k);
+                            ie(t, "htmx:afterOnLoad", k)
                         }
                     }
-                    Z(c);
-                    s()
+                    K(a);
+                    x()
                 } catch (e) {
-                    J(n, "htmx:onLoadError", Y({
+                    ne(n, "htmx:onLoadError", te({
                         error: e
-                    }, u));
+                    }, k));
                     throw e
                 }
             };
-            o.onerror = function() {
-                Mt(B);
-                J(n, "htmx:afterRequest", u);
-                J(n, "htmx:sendError", u);
-                Z(h);
-                s()
+            m.onerror = function() {
+                _t(P);
+                ne(n, "htmx:afterRequest", k);
+                ne(n, "htmx:sendError", k);
+                K(o);
+                x()
             };
-            o.onabort = function() {
-                Mt(B);
-                J(n, "htmx:afterRequest", u);
-                J(n, "htmx:sendAbort", u);
-                Z(h);
-                s()
+            m.onabort = function() {
+                _t(P);
+                ne(n, "htmx:afterRequest", k);
+                ne(n, "htmx:sendAbort", k);
+                K(o);
+                x()
             };
-            o.ontimeout = function() {
-                Mt(B);
-                J(n, "htmx:afterRequest", u);
-                J(n, "htmx:timeout", u);
-                Z(h);
-                s()
+            m.ontimeout = function() {
+                _t(P);
+                ne(n, "htmx:afterRequest", k);
+                ne(n, "htmx:timeout", k);
+                K(o);
+                x()
             };
-            if (!$(n, "htmx:beforeRequest", u)) {
-                Z(c);
-                s();
-                return d
-            }
-            var B = kt(n);
-            G(["loadstart", "loadend", "progress", "abort"], function(t) {
-                G([o, o.upload], function(e) {
+            if (!ie(n, "htmx:beforeRequest", k)) {
+                K(a);
+                x();
+                return s
+            }
+            var P = Vt(n);
+            Q(["loadstart", "loadend", "progress", "abort"], function(t) {
+                Q([m, m.upload], function(e) {
                     e.addEventListener(t, function(e) {
-                        $(n, "htmx:xhr:" + t, {
+                        ie(n, "htmx:xhr:" + t, {
                             lengthComputable: e.lengthComputable,
                             loaded: e.loaded,
                             total: e.total
                         })
                     })
                 })
             });
-            $(n, "htmx:beforeSend", u);
-            o.send(e === "get" ? null : $t(o, n, N));
-            return d
+            ie(n, "htmx:beforeSend", k);
+            m.send(e === "get" ? null : ir(m, n, q));
+            return s
         }
 
-        function ur(e, t) {
+        function gr(e, t) {
             var r = t.xhr;
             var n = null;
             var i = null;
-            if (ar(r, /HX-Push:/i)) {
+            if (E(r, /HX-Push:/i)) {
                 n = r.getResponseHeader("HX-Push");
                 i = "push"
-            } else if (ar(r, /HX-Push-Url:/i)) {
+            } else if (E(r, /HX-Push-Url:/i)) {
                 n = r.getResponseHeader("HX-Push-Url");
                 i = "push"
-            } else if (ar(r, /HX-Replace-Url:/i)) {
+            } else if (E(r, /HX-Replace-Url:/i)) {
                 n = r.getResponseHeader("HX-Replace-Url");
                 i = "replace"
             }
             if (n) {
                 if (n === "false") {
                     return {}
                 } else {
@@ -2704,227 +2876,251 @@
                         type: i,
                         path: n
                     }
                 }
             }
             var a = t.pathInfo.finalRequestPath;
             var o = t.pathInfo.responsePath;
-            var s = z(e, "hx-push-url");
-            var f = z(e, "hx-replace-url");
-            var c = W(e).boosted;
-            var l = null;
-            var u = null;
+            var s = Z(e, "hx-push-url");
+            var l = Z(e, "hx-replace-url");
+            var u = Y(e).boosted;
+            var f = null;
+            var c = null;
             if (s) {
-                l = "push";
-                u = s
-            } else if (f) {
-                l = "replace";
-                u = f
-            } else if (c) {
-                l = "push";
-                u = o || a
+                f = "push";
+                c = s
+            } else if (l) {
+                f = "replace";
+                c = l
+            } else if (u) {
+                f = "push";
+                c = o || a
             }
-            if (u) {
-                if (u === "false") {
+            if (c) {
+                if (c === "false") {
                     return {}
                 }
-                if (u === "true") {
-                    u = o || a
+                if (c === "true") {
+                    c = o || a
                 }
-                if (t.pathInfo.anchor && u.indexOf("#") === -1) {
-                    u = u + "#" + t.pathInfo.anchor
+                if (t.pathInfo.anchor && c.indexOf("#") === -1) {
+                    c = c + "#" + t.pathInfo.anchor
                 }
                 return {
-                    type: l,
-                    path: u
+                    type: f,
+                    path: c
                 }
             } else {
                 return {}
             }
         }
 
-        function fr(s, l) {
+        function pr(s, l) {
             var u = l.xhr;
             var f = l.target;
-            var n = l.etc;
-            if (!$(s, "htmx:beforeOnLoad", l)) return;
-            if (ar(u, /HX-Trigger:/i)) {
-                qe(u, "HX-Trigger", s)
-            }
-            if (ar(u, /HX-Location:/i)) {
-                Lt();
-                var e = u.getResponseHeader("HX-Location");
+            var e = l.etc;
+            if (!ie(s, "htmx:beforeOnLoad", l)) return;
+            if (E(u, /HX-Trigger:/i)) {
+                De(u, "HX-Trigger", s)
+            }
+            if (E(u, /HX-Location:/i)) {
+                Dt();
+                var t = u.getResponseHeader("HX-Location");
                 var c;
-                if (e.indexOf("{") === 0) {
-                    c = S(e);
-                    e = c["path"];
+                if (t.indexOf("{") === 0) {
+                    c = y(t);
+                    t = c["path"];
                     delete c["path"]
                 }
-                or("GET", e, c).then(() => {
-                    Tt(e)
+                dr("GET", t, c).then(function() {
+                    Xt(t)
                 });
                 return
             }
-            if (ar(u, /HX-Redirect:/i)) {
+            if (E(u, /HX-Redirect:/i)) {
                 location.href = u.getResponseHeader("HX-Redirect");
                 return
             }
-            if (ar(u, /HX-Refresh:/i)) {
+            if (E(u, /HX-Refresh:/i)) {
                 if ("true" === u.getResponseHeader("HX-Refresh")) {
                     location.reload();
                     return
                 }
             }
-            if (ar(u, /HX-Retarget:/i)) {
-                l.target = _().querySelector(u.getResponseHeader("HX-Retarget"))
+            if (E(u, /HX-Retarget:/i)) {
+                l.target = J().querySelector(u.getResponseHeader("HX-Retarget"))
             }
-            var h = ur(s, l);
-            var i = u.status >= 200 && u.status < 400 && u.status !== 204;
+            var h = gr(s, l);
+            var r = u.status >= 200 && u.status < 400 && u.status !== 204;
             var d = u.response;
-            var t = u.status >= 400;
-            var r = Y({
-                shouldSwap: i,
+            var n = u.status >= 400;
+            var i = te({
+                shouldSwap: r,
                 serverResponse: d,
-                isError: t
+                isError: n
             }, l);
-            if (!$(f, "htmx:beforeSwap", r)) return;
-            f = r.target;
-            d = r.serverResponse;
-            t = r.isError;
-            l.failed = t;
-            l.successful = !t;
-            if (r.shouldSwap) {
+            if (!ie(f, "htmx:beforeSwap", i)) return;
+            f = i.target;
+            d = i.serverResponse;
+            n = i.isError;
+            l.target = f;
+            l.failed = n;
+            l.successful = !n;
+            if (i.shouldSwap) {
                 if (u.status === 286) {
-                    Fe(s)
+                    $e(s)
                 }
-                wt(s, function(e) {
+                w(s, function(e) {
                     d = e.transformResponse(d, u, s)
                 });
                 if (h.type) {
-                    Lt()
+                    Dt()
                 }
-                var a = n.swapOverride;
-                if (ar(u, /HX-Reswap:/i)) {
+                var a = e.swapOverride;
+                if (E(u, /HX-Reswap:/i)) {
                     a = u.getResponseHeader("HX-Reswap")
                 }
-                var c = Gt(s, a);
-                f.classList.add(U.config.swappingClass);
+                var c = rr(s, a);
+                f.classList.add(z.config.swappingClass);
+                var v = null;
+                var g = null;
                 var o = function() {
                     try {
                         var e = document.activeElement;
                         var t = {};
                         try {
                             t = {
                                 elt: e,
                                 start: e ? e.selectionStart : null,
                                 end: e ? e.selectionEnd : null
                             }
                         } catch (e) {}
-                        var n = Zt(f);
-                        Oe(c.swapStyle, f, s, d, n);
-                        if (t.elt && !K(t.elt) && t.elt.id) {
+                        var n = S(f);
+                        Me(c.swapStyle, f, s, d, n);
+                        if (t.elt && !ee(t.elt) && t.elt.id) {
                             var r = document.getElementById(t.elt.id);
                             var i = {
-                                preventScroll: c.focusScroll !== undefined ? !c.focusScroll : !U.config.defaultFocusScroll
+                                preventScroll: c.focusScroll !== undefined ? !c.focusScroll : !z.config.defaultFocusScroll
                             };
                             if (r) {
                                 if (t.start && r.setSelectionRange) {
-                                    r.setSelectionRange(t.start, t.end)
+                                    try {
+                                        r.setSelectionRange(t.start, t.end)
+                                    } catch (e) {}
                                 }
                                 r.focus(i)
                             }
                         }
-                        f.classList.remove(U.config.swappingClass);
-                        G(n.elts, function(e) {
+                        f.classList.remove(z.config.swappingClass);
+                        Q(n.elts, function(e) {
                             if (e.classList) {
-                                e.classList.add(U.config.settlingClass)
+                                e.classList.add(z.config.settlingClass)
                             }
-                            $(e, "htmx:afterSwap", l)
+                            ie(e, "htmx:afterSwap", l)
                         });
-                        if (ar(u, /HX-Trigger-After-Swap:/i)) {
+                        if (E(u, /HX-Trigger-After-Swap:/i)) {
                             var a = s;
-                            if (!K(s)) {
-                                a = _().body
+                            if (!ee(s)) {
+                                a = J().body
                             }
-                            qe(u, "HX-Trigger-After-Swap", a)
+                            De(u, "HX-Trigger-After-Swap", a)
                         }
                         var o = function() {
-                            G(n.tasks, function(e) {
+                            Q(n.tasks, function(e) {
                                 e.call()
                             });
-                            G(n.elts, function(e) {
+                            Q(n.elts, function(e) {
                                 if (e.classList) {
-                                    e.classList.remove(U.config.settlingClass)
+                                    e.classList.remove(z.config.settlingClass)
                                 }
-                                $(e, "htmx:afterSettle", l)
+                                ie(e, "htmx:afterSettle", l)
                             });
                             if (h.type) {
                                 if (h.type === "push") {
-                                    Tt(h.path);
-                                    $(_().body, "htmx:pushedIntoHistory", {
+                                    Xt(h.path);
+                                    ie(J().body, "htmx:pushedIntoHistory", {
                                         path: h.path
                                     })
                                 } else {
-                                    Ht(h.path);
-                                    $(_().body, "htmx:replacedInHistory", {
+                                    Ft(h.path);
+                                    ie(J().body, "htmx:replacedInHistory", {
                                         path: h.path
                                     })
                                 }
                             }
                             if (l.pathInfo.anchor) {
-                                var e = R("#" + l.pathInfo.anchor);
+                                var e = b("#" + l.pathInfo.anchor);
                                 if (e) {
                                     e.scrollIntoView({
                                         block: "start",
                                         behavior: "auto"
                                     })
                                 }
                             }
                             if (n.title) {
-                                var t = R("title");
+                                var t = b("title");
                                 if (t) {
                                     t.innerHTML = n.title
                                 } else {
                                     window.document.title = n.title
                                 }
                             }
-                            Kt(n.elts, c);
-                            if (ar(u, /HX-Trigger-After-Settle:/i)) {
+                            ar(n.elts, c);
+                            if (E(u, /HX-Trigger-After-Settle:/i)) {
                                 var r = s;
-                                if (!K(s)) {
-                                    r = _().body
+                                if (!ee(s)) {
+                                    r = J().body
                                 }
-                                qe(u, "HX-Trigger-After-Settle", r)
+                                De(u, "HX-Trigger-After-Settle", r)
                             }
+                            K(v)
                         };
                         if (c.settleDelay > 0) {
                             setTimeout(o, c.settleDelay)
                         } else {
                             o()
                         }
                     } catch (e) {
-                        J(s, "htmx:swapError", l);
+                        ne(s, "htmx:swapError", l);
+                        K(g);
                         throw e
                     }
                 };
+                var p = z.config.globalViewTransitions;
+                if (c.hasOwnProperty("transition")) {
+                    p = c.transition
+                }
+                if (p && ie(s, "htmx:beforeTransition", l) && typeof Promise !== "undefined" && document.startViewTransition) {
+                    var m = new Promise(function(e, t) {
+                        v = e;
+                        g = t
+                    });
+                    var x = o;
+                    o = function() {
+                        document.startViewTransition(function() {
+                            x();
+                            return m
+                        })
+                    }
+                }
                 if (c.swapDelay > 0) {
                     setTimeout(o, c.swapDelay)
                 } else {
                     o()
                 }
             }
-            if (t) {
-                J(s, "htmx:responseError", Y({
-                    error: "Response Status Error Code " + u.status + " from " + l.pathInfo.path
+            if (n) {
+                ne(s, "htmx:responseError", te({
+                    error: "Response Status Error Code " + u.status + " from " + l.pathInfo.requestPath
                 }, l))
             }
         }
-        var cr = {};
+        var mr = {};
 
-        function hr() {
+        function xr() {
             return {
                 init: function(e) {
                     return null
                 },
                 onEvent: function(e, t) {
                     return true
                 },
@@ -2939,107 +3135,113 @@
                 },
                 encodeParameters: function(e, t, r) {
                     return null
                 }
             }
         }
 
-        function dr(e, t) {
+        function yr(e, t) {
             if (t.init) {
-                t.init(r)
+                t.init(C)
             }
-            cr[e] = Y(hr(), t)
+            mr[e] = te(xr(), t)
         }
 
-        function vr(e) {
-            delete cr[e]
+        function br(e) {
+            delete mr[e]
         }
 
-        function gr(e, r, n) {
+        function wr(e, r, n) {
             if (e == undefined) {
                 return r
             }
             if (r == undefined) {
                 r = []
             }
             if (n == undefined) {
                 n = []
             }
-            var t = V(e, "hx-ext");
+            var t = G(e, "hx-ext");
             if (t) {
-                G(t.split(","), function(e) {
+                Q(t.split(","), function(e) {
                     e = e.replace(/ /g, "");
                     if (e.slice(0, 7) == "ignore:") {
                         n.push(e.slice(7));
                         return
                     }
                     if (n.indexOf(e) < 0) {
-                        var t = cr[e];
+                        var t = mr[e];
                         if (t && r.indexOf(t) < 0) {
                             r.push(t)
                         }
                     }
                 })
             }
-            return gr(u(e), r, n)
+            return wr(u(e), r, n)
         }
 
-        function pr(e) {
-            if (_().readyState !== "loading") {
+        function Sr(e) {
+            if (J().readyState !== "loading") {
                 e()
             } else {
-                _().addEventListener("DOMContentLoaded", e)
+                J().addEventListener("DOMContentLoaded", e)
             }
         }
 
-        function mr() {
-            if (U.config.includeIndicatorStyles !== false) {
-                _().head.insertAdjacentHTML("beforeend", "<style>                      ." + U.config.indicatorClass + "{opacity:0;transition: opacity 200ms ease-in;}                      ." + U.config.requestClass + " ." + U.config.indicatorClass + "{opacity:1}                      ." + U.config.requestClass + "." + U.config.indicatorClass + "{opacity:1}                    </style>")
+        function Er() {
+            if (z.config.includeIndicatorStyles !== false) {
+                J().head.insertAdjacentHTML("beforeend", "<style>                      ." + z.config.indicatorClass + "{opacity:0;transition: opacity 200ms ease-in;}                      ." + z.config.requestClass + " ." + z.config.indicatorClass + "{opacity:1}                      ." + z.config.requestClass + "." + z.config.indicatorClass + "{opacity:1}                    </style>")
             }
         }
 
-        function xr() {
-            var e = _().querySelector('meta[name="htmx-config"]');
+        function Cr() {
+            var e = J().querySelector('meta[name="htmx-config"]');
             if (e) {
-                return S(e.content)
+                return y(e.content)
             } else {
                 return null
             }
         }
 
-        function yr() {
-            var e = xr();
+        function Rr() {
+            var e = Cr();
             if (e) {
-                U.config = Y(U.config, e)
+                z.config = te(z.config, e)
             }
         }
-        pr(function() {
-            yr();
-            mr();
-            var e = _().body;
-            mt(e);
-            var t = _().querySelectorAll("[hx-trigger='restored'],[data-hx-trigger='restored']");
+        Sr(function() {
+            Rr();
+            Er();
+            var e = J().body;
+            Tt(e);
+            var t = J().querySelectorAll("[hx-trigger='restored'],[data-hx-trigger='restored']");
             e.addEventListener("htmx:abort", function(e) {
                 var t = e.target;
-                var r = W(t);
+                var r = Y(t);
                 if (r && r.xhr) {
                     r.xhr.abort()
                 }
             });
+            var r = window.onpopstate;
             window.onpopstate = function(e) {
                 if (e.state && e.state.htmx) {
-                    It();
-                    G(t, function(e) {
-                        $(e, "htmx:restored", {
-                            document: _(),
-                            triggerEvent: $
+                    Ut();
+                    Q(t, function(e) {
+                        ie(e, "htmx:restored", {
+                            document: J(),
+                            triggerEvent: ie
                         })
                     })
+                } else {
+                    if (r) {
+                        r(e)
+                    }
                 }
             };
             setTimeout(function() {
-                $(e, "htmx:load", {})
+                ie(e, "htmx:load", {});
+                e = null
             }, 0)
         });
-        return U
+        return z
     }()
 });
```

### Comparing `django_unfold-0.5.3/src/unfold/static/unfold/js/simplebar.js` & `django_unfold-0.6.0/src/unfold/static/unfold/js/simplebar.js`

 * *Files identical despite different names*

### Comparing `django_unfold-0.5.3/src/unfold/templates/admin/actions.html` & `django_unfold-0.6.0/src/unfold/templates/admin/actions.html`

 * *Files identical despite different names*

### Comparing `django_unfold-0.5.3/src/unfold/templates/admin/app_index.html` & `django_unfold-0.6.0/src/unfold/templates/admin/app_index.html`

 * *Files identical despite different names*

### Comparing `django_unfold-0.5.3/src/unfold/templates/admin/app_list.html` & `django_unfold-0.6.0/src/unfold/templates/admin/app_list.html`

 * *Files identical despite different names*

### Comparing `django_unfold-0.5.3/src/unfold/templates/admin/auth/user/change_password.html` & `django_unfold-0.6.0/src/unfold/templates/admin/auth/user/change_password.html`

 * *Files 9% similar despite different names*

```diff
@@ -31,28 +31,29 @@
 {% endif %}
 
 {% block content %}
     <div id="content-main">
         <form{% if form_url %} action="{{ form_url }}"{% endif %} method="post" id="{{ opts.model_name }}_form">{% csrf_token %}{% block form_top %}{% endblock %}
             <input type="text" name="username" value="{{ original.get_username }}" class="hidden">
 
-            <div>
-                {% if is_popup %}
-                    <input type="hidden" name="{{ is_popup_var }}" value="1">
-                {% endif %}
+            {% if is_popup %}
+                <input type="hidden" name="{{ is_popup_var }}" value="1">
+            {% endif %}
 
-                {% include "unfold/helpers/messages/errornote.html" with errors=form.errors %}
+            {% include "unfold/helpers/messages/errornote.html" with errors=form.errors %}
 
-                {% blocktranslate with username=original asvar message %}Enter a new password for the user <strong>{{ username }}</strong>.{% endblocktranslate %}
-                {% include "unfold/helpers/messages/info.html" with message=message %}
+            {% blocktranslate with username=original asvar message %}Enter a new password for the user <strong>{{ username }}</strong>.{% endblocktranslate %}
+            {% include "unfold/helpers/messages/info.html" with message=message %}
+
+            <fieldset class="border border-gray-200 mb-8 rounded-md pt-3 px-3 shadow-sm dark:border-gray-800">
 
                 {% include "unfold/helpers/field.html" with field=form.password1 %}
 
                 {% include "unfold/helpers/field.html" with field=form.password2 %}
+            </fieldset>
 
-                <button type="submit" class="bg-primary-600 border border-transparent font-medium px-3 py-2 rounded-md text-sm text-white">
-                    {% translate 'Change password' %}
-                </button>
-            </div>
+            <button type="submit" class="bg-primary-600 border border-transparent font-medium px-3 py-2 rounded-md text-sm text-white">
+                {% translate 'Change password' %}
+            </button>
         </form>
     </div>
 {% endblock %}
```

### Comparing `django_unfold-0.5.3/src/unfold/templates/admin/base.html` & `django_unfold-0.6.0/src/unfold/templates/admin/base.html`

 * *Files identical despite different names*

### Comparing `django_unfold-0.5.3/src/unfold/templates/admin/change_form.html` & `django_unfold-0.6.0/src/unfold/templates/admin/change_form.html`

 * *Files identical despite different names*

### Comparing `django_unfold-0.5.3/src/unfold/templates/admin/change_form_object_tools.html` & `django_unfold-0.6.0/src/unfold/templates/admin/change_form_object_tools.html`

 * *Files identical despite different names*

### Comparing `django_unfold-0.5.3/src/unfold/templates/admin/change_list.html` & `django_unfold-0.6.0/src/unfold/templates/admin/change_list.html`

 * *Files identical despite different names*

### Comparing `django_unfold-0.5.3/src/unfold/templates/admin/change_list_object_tools.html` & `django_unfold-0.6.0/src/unfold/templates/admin/change_list_object_tools.html`

 * *Files identical despite different names*

### Comparing `django_unfold-0.5.3/src/unfold/templates/admin/change_list_results.html` & `django_unfold-0.6.0/src/unfold/templates/admin/change_list_results.html`

 * *Files 3% similar despite different names*

```diff
@@ -62,12 +62,13 @@
                     </tr>
                 {% endif %}
 
                 <tr class="{% cycle '' 'bg-gray-50 dark:bg-white/[.02]' %} block border mb-3 rounded-md shadow-sm lg:table-row lg:border-none lg:mb-0 lg:shadow-none dark:border-gray-800">
                     {% for item in result %}
                         {{ item }}
                     {% endfor %}
+                    {% include 'unfold/helpers/actions_row.html' with actions=actions_row instance_pk=result.instance_pk %}
                 </tr>
             {% endfor %}
         </tbody>
     </table>
 {% endif %}
```

### Comparing `django_unfold-0.5.3/src/unfold/templates/admin/date_hierarchy.html` & `django_unfold-0.6.0/src/unfold/templates/admin/date_hierarchy.html`

 * *Files identical despite different names*

### Comparing `django_unfold-0.5.3/src/unfold/templates/admin/delete_confirmation.html` & `django_unfold-0.6.0/src/unfold/templates/admin/delete_confirmation.html`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
         </div>
     {% elif protected %}
         <div class="border border-gray-200 rounded-md shadow-sm dark:border-gray-800">
             <p class="font-medium p-4 text-gray-700 text-sm dark:text-gray-200">
                 {% blocktranslate with escaped_object=object %}Deleting the {{ object_name }} '{{ escaped_object }}' would require deleting the following protected related objects:{% endblocktranslate %}
             </p>
 
-            <div class="bborder-gray-200  order-t p-4 dark:border-gray-800">
+            <div class="border-t border-gray-200  order-t p-4 dark:border-gray-800">
                 <ul class="leading-relaxed text-gray-500 text-sm dark:text-gray-400">
                     {% for obj in protected %}
                         <li>
                             {{ obj }}
                         </li>
                     {% endfor %}
                 </ul>
```

### Comparing `django_unfold-0.5.3/src/unfold/templates/admin/delete_selected_confirmation.html` & `django_unfold-0.6.0/src/unfold/templates/admin/delete_selected_confirmation.html`

 * *Files identical despite different names*

### Comparing `django_unfold-0.5.3/src/unfold/templates/admin/edit_inline/stacked.html` & `django_unfold-0.6.0/src/unfold/templates/admin/edit_inline/stacked.html`

 * *Files identical despite different names*

### Comparing `django_unfold-0.5.3/src/unfold/templates/admin/edit_inline/tabular.html` & `django_unfold-0.6.0/src/unfold/templates/admin/edit_inline/tabular.html`

 * *Files identical despite different names*

### Comparing `django_unfold-0.5.3/src/unfold/templates/admin/filter.html` & `django_unfold-0.6.0/src/unfold/templates/admin/filter.html`

 * *Files identical despite different names*

### Comparing `django_unfold-0.5.3/src/unfold/templates/admin/includes/fieldset.html` & `django_unfold-0.6.0/src/unfold/templates/admin/includes/fieldset.html`

 * *Files identical despite different names*

### Comparing `django_unfold-0.5.3/src/unfold/templates/admin/index.html` & `django_unfold-0.6.0/src/unfold/templates/admin/index.html`

 * *Files identical despite different names*

### Comparing `django_unfold-0.5.3/src/unfold/templates/admin/login.html` & `django_unfold-0.6.0/src/unfold/templates/admin/login.html`

 * *Files identical despite different names*

### Comparing `django_unfold-0.5.3/src/unfold/templates/admin/nav_sidebar.html` & `django_unfold-0.6.0/src/unfold/templates/admin/nav_sidebar.html`

 * *Files identical despite different names*

### Comparing `django_unfold-0.5.3/src/unfold/templates/admin/object_history.html` & `django_unfold-0.6.0/src/unfold/templates/admin/object_history.html`

 * *Files identical despite different names*

### Comparing `django_unfold-0.5.3/src/unfold/templates/admin/pagination.html` & `django_unfold-0.6.0/src/unfold/templates/admin/pagination.html`

 * *Files identical despite different names*

### Comparing `django_unfold-0.5.3/src/unfold/templates/admin/search_form.html` & `django_unfold-0.6.0/src/unfold/templates/admin/search_form.html`

 * *Files identical despite different names*

### Comparing `django_unfold-0.5.3/src/unfold/templates/admin/submit_line.html` & `django_unfold-0.6.0/src/unfold/templates/admin/submit_line.html`

 * *Files identical despite different names*

### Comparing `django_unfold-0.5.3/src/unfold/templates/admin/widgets/clearable_file_input.html` & `django_unfold-0.6.0/src/unfold/templates/admin/widgets/clearable_file_input.html`

 * *Files identical despite different names*

### Comparing `django_unfold-0.5.3/src/unfold/templates/admin/widgets/related_widget_wrapper.html` & `django_unfold-0.6.0/src/unfold/templates/admin/widgets/related_widget_wrapper.html`

 * *Files identical despite different names*

### Comparing `django_unfold-0.5.3/src/unfold/templates/admin/widgets/split_datetime.html` & `django_unfold-0.6.0/src/unfold/templates/admin/widgets/split_datetime.html`

 * *Files identical despite different names*

### Comparing `django_unfold-0.5.3/src/unfold/templates/auth/widgets/read_only_password_hash.html` & `django_unfold-0.6.0/src/unfold/templates/auth/widgets/read_only_password_hash.html`

 * *Files identical despite different names*

### Comparing `django_unfold-0.5.3/src/unfold/templates/registration/logged_out.html` & `django_unfold-0.6.0/src/unfold/templates/registration/logged_out.html`

 * *Files identical despite different names*

### Comparing `django_unfold-0.5.3/src/unfold/templates/registration/password_change_done.html` & `django_unfold-0.6.0/src/unfold/templates/registration/password_change_done.html`

 * *Files identical despite different names*

### Comparing `django_unfold-0.5.3/src/unfold/templates/registration/password_change_form.html` & `django_unfold-0.6.0/src/unfold/templates/registration/password_change_form.html`

 * *Files identical despite different names*

### Comparing `django_unfold-0.5.3/src/unfold/templates/unfold/helpers/app_list.html` & `django_unfold-0.6.0/src/unfold/templates/unfold/helpers/app_list.html`

 * *Files identical despite different names*

### Comparing `django_unfold-0.5.3/src/unfold/templates/unfold/helpers/app_list_default.html` & `django_unfold-0.6.0/src/unfold/templates/unfold/helpers/app_list_default.html`

 * *Files identical despite different names*

### Comparing `django_unfold-0.5.3/src/unfold/templates/unfold/helpers/display_label.html` & `django_unfold-0.6.0/src/unfold/templates/unfold/helpers/display_label.html`

 * *Files identical despite different names*

### Comparing `django_unfold-0.5.3/src/unfold/templates/unfold/helpers/history.html` & `django_unfold-0.6.0/src/unfold/templates/unfold/helpers/history.html`

 * *Files identical despite different names*

### Comparing `django_unfold-0.5.3/src/unfold/templates/unfold/helpers/messages/error.html` & `django_unfold-0.6.0/src/unfold/templates/unfold/helpers/messages/error.html`

 * *Files identical despite different names*

### Comparing `django_unfold-0.5.3/src/unfold/templates/unfold/helpers/messages.html` & `django_unfold-0.6.0/src/unfold/templates/unfold/helpers/messages.html`

 * *Files identical despite different names*

### Comparing `django_unfold-0.5.3/src/unfold/templates/unfold/helpers/navigation.html` & `django_unfold-0.6.0/src/unfold/templates/unfold/helpers/navigation.html`

 * *Files identical despite different names*

### Comparing `django_unfold-0.5.3/src/unfold/templates/unfold/helpers/search.html` & `django_unfold-0.6.0/src/unfold/templates/unfold/helpers/search.html`

 * *Files identical despite different names*

### Comparing `django_unfold-0.5.3/src/unfold/templates/unfold/helpers/search_results.html` & `django_unfold-0.6.0/src/unfold/templates/unfold/helpers/search_results.html`

 * *Files identical despite different names*

### Comparing `django_unfold-0.5.3/src/unfold/templates/unfold/helpers/tab_list.html` & `django_unfold-0.6.0/src/unfold/templates/unfold/helpers/tab_list.html`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 {% if not is_popup %}
-    {% if tab_list or actions_list %}
+    {% if tab_list or actions_list or actions_items %}
         <div class="flex items-start flex-col mb-2 text-gray-500 text-sm w-full md:border-b dark:md:border-gray-800 md:border-l-0 md:flex-row md:items-center md:justify-end dark:text-gray-400">
             {% if tab_list %}
                 <ul class="border rounded-md flex flex-col w-full md:flex-row md:border-b-0 md:border-t-0 md:border-l-0 md:border-r-0 dark:border-gray-800">
                     {% for item in tab_list %}
                         <li class="border-b last:border-b-0 md:border-b-0 md:mr-8 dark:border-gray-800">
-                            <a href="{{ item.link }}" class="block px-3 py-2 {% if item.link|stringformat:"s" in request.path %} border-b md:border-primary-600 dark:md:border-primary-600 font-medium -mb-px text-primary-600 hover:text-primary-600{% else %} hover:text-gray-700 dark:hover:text-gray-200{% endif %} md:py-4 md:px-0 dark:border-gray-800">
+                            <a href="{{ item.link }}" class="block px-3 py-2 {% if item.link|stringformat:"s" in request.path %} border-b md:border-primary-500 dark:md:border-primary-600 font-medium -mb-px text-primary-600 hover:text-primary-600 dark:text-primary-500{% else %} hover:text-gray-700 dark:hover:text-gray-200{% endif %} md:py-4 md:px-0 dark:border-gray-800">
                                 {{ item.title }}
                             </a>
                         </li>
                     {% endfor %}
                 </ul>
             {% endif %}
 
-            {% if actions_list %}
+            {% if actions_list or actions_items %}
                 <ul class="border flex mb-4 mt-2 rounded-md shadow-sm md:mb-2 md:mt-0 dark:border-gray-700 max-md:w-full">
                     {% for action in actions_list %}
                         <li class="border-r flex-grow text-center last:border-0 dark:border-gray-700">
                             <a href="{{ action.path }}" class="block px-4 py-2 text-gray-500 whitespace-nowrap hover:text-gray-700 dark:text-gray-400 hover:dark:text-gray-200">
                                 {{ action.title }}
                             </a>
                         </li>
                     {% endfor %}
+
+                    {% if actions_items %}
+                        {{ actions_items }}
+                    {% endif %}
                 </ul>
             {% endif %}
         </div>
     {% endif %}
 {% endif %}
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
-{% if not is_popup %} {% if tab_list or actions_list %}
+{% if not is_popup %} {% if tab_list or actions_list or actions_items %}
 {% if tab_list %}
     * {% for item in tab_list %}
-    *  in request.path %} border-b md:border-primary-600 dark:md:border-
-      primary-600 font-medium -mb-px text-primary-600 hover:text-primary-600{%
-      else %} hover:text-gray-700 dark:hover:text-gray-200{% endif %} md:py-
-      4 md:px-0 dark:border-gray-800"> {{ item.title }}
+    *  in request.path %} border-b md:border-primary-500 dark:md:border-
+      primary-600 font-medium -mb-px text-primary-600 hover:text-primary-600
+      dark:text-primary-500{% else %} hover:text-gray-700 dark:hover:text-gray-
+      200{% endif %} md:py-4 md:px-0 dark:border-gray-800"> {{ item.title }}
 {% endfor %}
-{% endif %} {% if actions_list %}
+{% endif %} {% if actions_list or actions_items %}
     * {% for action in actions_list %}
     * {{_action.title_}}
-    * {% endfor %}
+    * {% endfor %} {% if actions_items %} {{ actions_items }} {% endif %}
 {% endif %}
 {% endif %} {% endif %}
```

### Comparing `django_unfold-0.5.3/src/unfold/templates/unfold/helpers/userlinks.html` & `django_unfold-0.6.0/src/unfold/templates/unfold/helpers/userlinks.html`

 * *Files identical despite different names*

### Comparing `django_unfold-0.5.3/src/unfold/templates/unfold/helpers/welcomemsg.html` & `django_unfold-0.6.0/src/unfold/templates/unfold/helpers/welcomemsg.html`

 * *Files identical despite different names*

### Comparing `django_unfold-0.5.3/src/unfold/templates/unfold/layouts/base_simple.html` & `django_unfold-0.6.0/src/unfold/templates/unfold/layouts/base_simple.html`

 * *Files identical despite different names*

### Comparing `django_unfold-0.5.3/src/unfold/templates/unfold/layouts/skeleton.html` & `django_unfold-0.6.0/src/unfold/templates/unfold/layouts/skeleton.html`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 {% capture as branding silent %}{% block branding %}{% endblock %}{% endcapture %}
 {% capture as pretitle silent %}{% block pretitle %}{% endblock %}{% endcapture %}
 {% capture as content_title silent %}{% block content_title %}{% if title %}{{ title }}{% endif %}{% endblock %}{% endcapture %}
 {% capture as content_subtitle silent %}{% block content_subtitle %}{% if subtitle %}{{ subtitle }}{% endif %}{% endblock %}{% endcapture %}
 {% capture as nav_global silent %}{% block nav-global %}{% endblock %}{% endcapture %}
 {% capture as nav_global_side silent %}{% block nav-global-side %}{% endblock %}{% endcapture %}
+{% capture as actions_items silent %}{% block actions-items %}{% endblock %}{% endcapture %}
 
 <!DOCTYPE html>
 <html lang="{{ LANGUAGE_CODE|default:"en-us" }}" dir="{{ LANGUAGE_BIDI|yesno:"rtl,ltr,auto" }}" x-data="{ theme: $persist({'value': 'auto'}).as('theme') }" x-bind:class="theme.value && theme.value" x-cloak>
 
 <head>
     <title>{% block title %}{% endblock %}</title>
```

#### html2text {}

```diff
@@ -3,15 +3,16 @@
 {% block branding %}{% endblock %}{% endcapture %} {% capture as pretitle
 silent %}{% block pretitle %}{% endblock %}{% endcapture %} {% capture as
 content_title silent %}{% block content_title %}{% if title %}{{ title }}{%
 endif %}{% endblock %}{% endcapture %} {% capture as content_subtitle silent %}
 {% block content_subtitle %}{% if subtitle %}{{ subtitle }}{% endif %}{%
 endblock %}{% endcapture %} {% capture as nav_global silent %}{% block nav-
 global %}{% endblock %}{% endcapture %} {% capture as nav_global_side silent %}
-{% block nav-global-side %}{% endblock %}{% endcapture %}
+{% block nav-global-side %}{% endblock %}{% endcapture %} {% capture as
+actions_items silent %}{% block actions-items %}{% endblock %}{% endcapture %}
 
  }}" dir="{{ LANGUAGE_BIDI|yesno:"rtl,ltr,auto" }}" x-data="{ theme: $persist(
 {'value': 'auto'}).as('theme') }" x-bind:class="theme.value && theme.value" x-
 cloak>
 
  {% for style in styles %}
  {% endfor %}
```

### Comparing `django_unfold-0.5.3/src/unfold/templates/unfold/widgets/clearable_file_input_small.html` & `django_unfold-0.6.0/src/unfold/templates/unfold/widgets/clearable_file_input_small.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 {% load i18n static %}
 
 <div class="flex flex-row">
-    <div class="border flex items-center overflow-hidden rounded-md shadow-sm text-sm max-w-2xl dark:border-gray-700">
+    <div class="border flex items-center overflow-hidden rounded-md shadow-sm text-sm max-w-2xl w-full dark:border-gray-700">
         {% if widget.is_initial and not widget.required %}
             <div class="bg-gray-50 border-r flex flex-none items-center self-stretch px-3 dark:bg-gray-900">
                 <label for="{{ widget.checkbox_id }}" class="flex items-center">
                     <input type="checkbox" class="form-check-input" name="{{ widget.checkbox_name }}" id="{{ widget.checkbox_id }}" />
 
                     <span class="ml-2 text-gray-500">
                         {{ widget.clear_checkbox_label }}
```

### Comparing `django_unfold-0.5.3/src/unfold/templates/unfold/widgets/split_datetime_vertical.html` & `django_unfold-0.6.0/src/unfold/templates/unfold/widgets/split_datetime_vertical.html`

 * *Files identical despite different names*

### Comparing `django_unfold-0.5.3/src/unfold/templatetags/unfold.py` & `django_unfold-0.6.0/src/unfold/templatetags/unfold.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,45 +1,65 @@
+from typing import Any, Dict, Mapping, Union
+
 from django.template import Library, Node, TemplateSyntaxError
+from django.template.base import NodeList, Parser, Token
 from django.template.loader import render_to_string
+from django.utils.safestring import SafeText
 
 register = Library()
 
 
 @register.simple_tag(name="tab_list", takes_context=True)
-def tab_list(context, opts):
+def tab_list(context, opts) -> str:
     tabs = None
 
     for tab in context.get("tab_list"):
         if str(opts) in tab["models"]:
             tabs = tab["items"]
             break
 
     return render_to_string(
         "unfold/helpers/tab_list.html",
         request=context.request,
         context={
             "tab_list": tabs,
             "actions_list": context.get("actions_list"),
+            "actions_items": context.get("actions_items"),
             "is_popup": context.get("is_popup"),
         },
     )
 
 
 @register.filter
-def class_name(value):
+def class_name(value: Any) -> str:
     return value.__class__.__name__
 
 
 @register.filter
-def index(indexable, i):
+def index(indexable: Mapping[int, Any], i: int) -> Any:
     return indexable[i]
 
 
+class CaptureNode(Node):
+    def __init__(self, nodelist: NodeList, varname: str, silent: bool) -> None:
+        self.nodelist = nodelist
+        self.varname = varname
+        self.silent = silent
+
+    def render(self, context: Dict[str, Any]) -> Union[str, SafeText]:
+        output = self.nodelist.render(context)
+        context[self.varname] = output
+        if self.silent:
+            return ""
+        else:
+            return output
+
+
 @register.tag(name="capture")
-def do_capture(parser, token):
+def do_capture(parser: Parser, token: Token) -> CaptureNode:
     """
     Capture the contents of a tag output.
     Usage:
     .. code-block:: html+django
         {% capture %}..{% endcapture %}                    # output in {{ capture }}
         {% capture silent %}..{% endcapture %}             # output in {{ capture }} only
         {% capture as varname %}..{% endcapture %}         # output in {{ varname }}
@@ -83,22 +103,7 @@
         raise TemplateSyntaxError(
             "'capture' node expects 'as variable' or 'silent' syntax."
         )
 
     nodelist = parser.parse(("endcapture",))
     parser.delete_first_token()
     return CaptureNode(nodelist, var, silent)
-
-
-class CaptureNode(Node):
-    def __init__(self, nodelist, varname, silent):
-        self.nodelist = nodelist
-        self.varname = varname
-        self.silent = silent
-
-    def render(self, context):
-        output = self.nodelist.render(context)
-        context[self.varname] = output
-        if self.silent:
-            return ""
-        else:
-            return output
```

### Comparing `django_unfold-0.5.3/src/unfold/templatetags/unfold_list.py` & `django_unfold-0.6.0/src/unfold/templatetags/unfold_list.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,45 +1,49 @@
 import datetime
+from typing import Any, Dict, Optional, Union
 
 from django.contrib.admin.templatetags.admin_list import (
     ResultList,
     _coerce_field_name,
     result_headers,
     result_hidden_fields,
 )
 from django.contrib.admin.templatetags.admin_urls import add_preserved_filters
 from django.contrib.admin.templatetags.base import InclusionAdminNode
 from django.contrib.admin.utils import lookup_field
-from django.contrib.admin.views.main import PAGE_VAR
+from django.contrib.admin.views.main import PAGE_VAR, ChangeList
 from django.core.exceptions import ObjectDoesNotExist
 from django.db import models
+from django.forms import Form
+from django.http import HttpRequest
 from django.template import Library
+from django.template.base import Parser, Token
 from django.template.loader import render_to_string
 from django.urls import NoReverseMatch
 from django.utils.html import format_html
-from django.utils.safestring import mark_safe
+from django.utils.safestring import SafeText, mark_safe
 
 from ..utils import (
     display_for_field,
     display_for_header,
     display_for_label,
     display_for_value,
 )
 
 register = Library()
 
 LINK_CLASSES = ["text-gray-700 dark:text-gray-200"]
 
 
-def items_for_result(cl, result, form):
+def items_for_result(cl: ChangeList, result: HttpRequest, form) -> SafeText:
     """
     Generate the actual list of data.
     """
 
-    def link_in_col(is_first, field_name, cl):
+    def link_in_col(is_first: bool, field_name: str, cl: ChangeList) -> bool:
         if cl.list_display_links is None:
             return False
         if is_first and not cl.list_display_links:
             return True
         return field_name in cl.list_display_links
 
     first = True
@@ -200,54 +204,66 @@
                     result_repr,
                 )
 
     if form and not form[cl.model._meta.pk.name].is_hidden:
         yield format_html("<td>{}</td>", form[cl.model._meta.pk.name])
 
 
-def results(cl):
+class UnfoldResultList(ResultList):
+    def __init__(
+        self, instance_pk: Union[int, str], form: Optional[Form], *items: Any
+    ) -> None:
+        self.instance_pk = instance_pk
+        super().__init__(form, *items)
+
+
+def results(cl: ChangeList):
     if cl.formset:
         for res, form in zip(cl.result_list, cl.formset.forms):
-            yield ResultList(form, items_for_result(cl, res, form))
+            pk = cl.lookup_opts.pk.attname
+            pk_value = getattr(res, pk)
+            yield UnfoldResultList(pk_value, form, items_for_result(cl, res, form))
     else:
         for res in cl.result_list:
-            yield ResultList(None, items_for_result(cl, res, None))
+            pk = cl.lookup_opts.pk.attname
+            pk_value = getattr(res, pk)
+            yield UnfoldResultList(pk_value, None, items_for_result(cl, res, None))
 
 
-def result_list(cl):
+def result_list(context: Dict[str, Any], cl: ChangeList) -> Dict[str, Any]:
     """
     Display the headers and data list together.
     """
     headers = list(result_headers(cl))
     num_sorted_fields = 0
     for h in headers:
         if h["sortable"] and h["sorted"]:
             num_sorted_fields += 1
     return {
         "cl": cl,
         "result_hidden_fields": list(result_hidden_fields(cl)),
         "result_headers": headers,
         "num_sorted_fields": num_sorted_fields,
         "results": list(results(cl)),
+        "actions_row": context["actions_row"],
     }
 
 
 @register.tag(name="unfold_result_list")
-def result_list_tag(parser, token):
+def result_list_tag(parser: Parser, token: Token) -> InclusionAdminNode:
     return InclusionAdminNode(
         parser,
         token,
         func=result_list,
         template_name="change_list_results.html",
-        takes_context=False,
     )
 
 
 @register.simple_tag
-def paginator_number(cl, i):
+def paginator_number(cl: ChangeList, i: Union[str, int]) -> Union[str, SafeText]:
     """
     Generate an individual page index link in a paginated list.
     """
     if i == cl.paginator.ELLIPSIS:
         return render_to_string(
             "unfold/helpers/pagination_ellipsis.html",
             {"ellipsis": cl.paginator.ELLIPSIS},
```

### Comparing `django_unfold-0.5.3/src/unfold/utils.py` & `django_unfold-0.6.0/src/unfold/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,40 +1,41 @@
 import datetime
 import decimal
 import json
+from typing import Any, Iterable
 
 from django.db import models
 from django.template.loader import render_to_string
 from django.utils import formats, timezone
 from django.utils.hashable import make_hashable
 from django.utils.html import format_html
-from django.utils.safestring import mark_safe
+from django.utils.safestring import SafeText, mark_safe
 
 from .exceptions import UnfoldException
 
 
-def _boolean_icon(field_val):
+def _boolean_icon(field_val: Any) -> str:
     return render_to_string("unfold/helpers/boolean.html", {"value": field_val})
 
 
-def display_for_header(value, empty_value_display):
+def display_for_header(value: Iterable, empty_value_display: str) -> SafeText:
     if not isinstance(value, list) and not isinstance(value, tuple):
         raise UnfoldException("Display header requires list or tuple")
 
     return mark_safe(
         render_to_string(
             "unfold/helpers/display_header.html",
             {
                 "value": value,
             },
         )
     )
 
 
-def display_for_label(value, empty_value_display, label):
+def display_for_label(value: Any, empty_value_display: str, label: Any) -> SafeText:
     label_type = None
     multiple = False
 
     if isinstance(label, dict):
         if isinstance(value, tuple):
             try:
                 label_type = label[value[0]]
@@ -55,15 +56,17 @@
                 "label_type": label_type,
                 "multiple": multiple,
             },
         )
     )
 
 
-def display_for_value(value, empty_value_display, boolean=False):
+def display_for_value(
+    value: Any, empty_value_display: str, boolean: bool = False
+) -> str:
     if boolean:
         return _boolean_icon(value)
     elif value is None:
         return empty_value_display
     elif isinstance(value, bool):
         return str(value)
     elif isinstance(value, datetime.datetime):
@@ -74,15 +77,15 @@
         return formats.number_format(value)
     elif isinstance(value, (list, tuple)):
         return ", ".join(str(v) for v in value)
     else:
         return str(value)
 
 
-def display_for_field(value, field, empty_value_display):
+def display_for_field(value: Any, field: Any, empty_value_display: str) -> str:
     if getattr(field, "flatchoices", None):
         try:
             return dict(field.flatchoices).get(value, empty_value_display)
         except TypeError:
             # Allow list-like choices.
             flatchoices = make_hashable(field.flatchoices)
             value = make_hashable(value)
```

### Comparing `django_unfold-0.5.3/src/unfold/views.py` & `django_unfold-0.6.0/src/unfold/views.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,20 @@
+from typing import Any, Dict
+
 from django.contrib.auth.mixins import PermissionRequiredMixin
 
 from .exceptions import UnfoldException
 
 
 class UnfoldModelAdminViewMixin(PermissionRequiredMixin):
     """
     Prepares views to be displayed in admin
     """
 
-    def get_context_data(self, **kwargs):
+    def get_context_data(self, **kwargs) -> Dict[str, Any]:
         if "model_admin" not in self.kwargs:
             raise UnfoldException(
                 "UnfoldModelAdminViewMixin was not provided with 'model_admin' argument"
             )
         model_admin = self.kwargs["model_admin"]
         context_data = super().get_context_data(
             **kwargs, **model_admin.admin_site.each_context(self.request)
```

### Comparing `django_unfold-0.5.3/src/unfold/widgets.py` & `django_unfold-0.6.0/src/unfold/widgets.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from typing import Any, Callable, Dict, Optional, Tuple, Union
+
 from django.contrib.admin.widgets import (
     AdminBigIntegerFieldWidget,
     AdminDateWidget,
     AdminEmailInputWidget,
     AdminFileWidget,
     AdminIntegerFieldWidget,
     AdminSplitDateTime,
@@ -98,103 +100,115 @@
     "dark:prose-blockquote:text-gray-200",
     "dark:prose-headings:text-gray-200",
     "dark:prose-strong:text-gray-200",
 ]
 
 
 class UnfoldAdminTextInputWidget(AdminTextInputWidget):
-    def __init__(self, attrs=None):
+    def __init__(self, attrs: Optional[Dict[str, Any]] = None) -> None:
         super().__init__(attrs={"class": " ".join(INPUT_CLASSES), **(attrs or {})})
 
 
 class UnfoldAdminUUIDInputWidget(AdminUUIDInputWidget):
-    def __init__(self, attrs=None):
+    def __init__(self, attrs: Optional[Dict[str, Any]] = None) -> None:
         super().__init__(attrs={"class": " ".join(INPUT_CLASSES), **(attrs or {})})
 
 
 class UnfoldAdminIntegerRangeWidget(MultiWidget):
     template_name = "unfold/widgets/range.html"
 
-    def __init__(self, attrs=None):
+    def __init__(self, attrs: Optional[Dict[str, Any]] = None) -> None:
         if attrs is None:
             attrs = {}
 
         attrs["class"] = " ".join(INPUT_CLASSES)
 
         _widgets = (NumberInput(attrs=attrs), NumberInput(attrs=attrs))
 
         super().__init__(_widgets, attrs)
 
-    def decompress(self, value):
+    def decompress(self, value: Union[str, None]) -> Tuple[Optional[Callable], ...]:
         if value:
             return value.lower, value.upper
         return None, None
 
 
 class UnfoldAdminEmailInputWidget(AdminEmailInputWidget):
-    def __init__(self, attrs=None):
+    def __init__(self, attrs: Optional[Dict[str, Any]] = None) -> None:
         super().__init__(attrs={"class": " ".join(INPUT_CLASSES), **(attrs or {})})
 
 
 class UnfoldAdminImageFieldWidget(AdminFileWidget):
     pass
 
 
+class UnfoldAdminFileFieldWidget(AdminFileWidget):
+    template_name = "unfold/widgets/clearable_file_input_small.html"
+
+
 class UnfoldAdminImageSmallFieldWidget(AdminFileWidget):
     template_name = "unfold/widgets/clearable_file_input_small.html"
 
 
 class UnfoldAdminDateWidget(AdminDateWidget):
-    def __init__(self, attrs=None, format=None):
+    def __init__(
+        self, attrs: Optional[Dict[str, Any]] = None, format: Optional[str] = None
+    ) -> None:
         attrs = {
             "class": "vDateField w-36 lg:w-60 " + " ".join(INPUT_CLASSES),
             "size": "10",
             **(attrs or {}),
         }
         super().__init__(attrs=attrs, format=format)
 
 
 class UnfoldAdminSingleDateWidget(AdminDateWidget):
     template_name = "unfold/widgets/date.html"
 
-    def __init__(self, attrs=None, format=None):
+    def __init__(
+        self, attrs: Optional[Dict[str, Any]] = None, format: Optional[str] = None
+    ) -> None:
         attrs = {
             "class": "vDateField " + " ".join(INPUT_CLASSES),
             "size": "10",
             **(attrs or {}),
         }
         super().__init__(attrs=attrs, format=format)
 
 
 class UnfoldAdminTimeWidget(AdminTimeWidget):
-    def __init__(self, attrs=None, format=None):
+    def __init__(
+        self, attrs: Optional[Dict[str, Any]] = None, format: Optional[str] = None
+    ) -> None:
         attrs = {
             "class": "vTimeField w-36 lg:w-60 " + " ".join(INPUT_CLASSES),
             "size": "8",
             **(attrs or {}),
         }
         super().__init__(attrs=attrs, format=format)
 
 
 class UnfoldAdminSingleTimeWidget(AdminTimeWidget):
     template_name = "unfold/widgets/time.html"
 
-    def __init__(self, attrs=None, format=None):
+    def __init__(
+        self, attrs: Optional[Dict[str, Any]] = None, format: Optional[str] = None
+    ) -> None:
         attrs = {
             "class": "vTimeField w-36 lg:w-60 " + " ".join(INPUT_CLASSES),
             "size": "8",
             **(attrs or {}),
         }
         super().__init__(attrs=attrs, format=format)
 
 
 class UnfoldAdminTextareaWidget(AdminTextareaWidget):
     template_name = "unfold/widgets/textarea.html"
 
-    def __init__(self, attrs=None):
+    def __init__(self, attrs: Optional[Dict[str, Any]] = None) -> None:
         attrs = attrs or {}
 
         attrs.update({"rows": 2})
 
         super().__init__(
             attrs={
                 "class": "vLargeTextField "
@@ -203,40 +217,42 @@
                 + " ".join(TEXTAREA_EXPANDABLE_CLASSES),
                 **(attrs or {}),
             }
         )
 
 
 class UnfoldAdminSplitDateTimeWidget(AdminSplitDateTime):
-    def __init__(self, attrs=None):
+    def __init__(self, attrs: Optional[Dict[str, Any]] = None) -> None:
         widgets = [UnfoldAdminDateWidget, UnfoldAdminTimeWidget]
         MultiWidget.__init__(self, widgets, attrs)
 
 
 class UnfoldAdminSplitDateTimeVerticalWidget(AdminSplitDateTime):
     template_name = "unfold/widgets/split_datetime_vertical.html"
 
     def __init__(
         self,
-        attrs=None,
-        date_attrs=None,
-        time_attrs=None,
-        date_label=None,
-        time_label=None,
-    ):
+        attrs: Optional[Dict[str, Any]] = None,
+        date_attrs: Optional[Dict[str, Any]] = None,
+        time_attrs: Optional[Dict[str, Any]] = None,
+        date_label: Optional[str] = None,
+        time_label: Optional[str] = None,
+    ) -> None:
         self.date_label = date_label
         self.time_label = time_label
 
         widgets = [
             UnfoldAdminDateWidget(attrs=date_attrs),
             UnfoldAdminTimeWidget(attrs=time_attrs),
         ]
         MultiWidget.__init__(self, widgets, attrs)
 
-    def get_context(self, name, value, attrs):
+    def get_context(
+        self, name: str, value: Any, attrs: Optional[Dict[str, Any]]
+    ) -> Dict[str, Any]:
         context = super().get_context(name, value, attrs)
 
         if self.date_label is not None:
             context["date_label"] = self.date_label
         else:
             context["date_label"] = _("Date")
 
@@ -245,23 +261,23 @@
         else:
             context["time_label"] = _("Time")
 
         return context
 
 
 class UnfoldAdminIntegerFieldWidget(AdminIntegerFieldWidget):
-    def __init__(self, attrs=None):
+    def __init__(self, attrs: Optional[Dict[str, Any]] = None) -> None:
         super().__init__(attrs={"class": " ".join(INPUT_CLASSES), **(attrs or {})})
 
 
 class UnfoldAdminDecimalFieldWidget(AdminIntegerFieldWidget):
-    def __init__(self, attrs=None):
+    def __init__(self, attrs: Optional[Dict[str, Any]] = None) -> None:
         super().__init__(attrs={"class": " ".join(INPUT_CLASSES), **(attrs or {})})
 
 
 class UnfoldAdminBigIntegerFieldWidget(AdminBigIntegerFieldWidget):
-    def __init__(self, attrs=None):
+    def __init__(self, attrs: Optional[Dict[str, Any]] = None) -> None:
         super().__init__(attrs={"class": " ".join(INPUT_CLASSES), **(attrs or {})})
 
 
 class UnfoldAdminNullBooleanSelectWidget(NullBooleanSelect):
     pass
```

### Comparing `django_unfold-0.5.3/setup.py` & `django_unfold-0.6.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 {'': 'src'}
 
 packages = \
 ['unfold',
  'unfold.contrib',
  'unfold.contrib.filters',
  'unfold.contrib.forms',
+ 'unfold.contrib.import_export',
  'unfold.templatetags']
 
 package_data = \
 {'': ['*'],
  'unfold': ['static/unfold/css/*',
             'static/unfold/js/*',
             'templates/admin/*',
@@ -28,29 +29,30 @@
             'templates/unfold/widgets/*'],
  'unfold.contrib.filters': ['static/unfold/filters/css/*',
                             'static/unfold/filters/js/*',
                             'templates/unfold/filters/*'],
  'unfold.contrib.forms': ['static/unfold/forms/css/*',
                           'static/unfold/forms/js/*',
                           'templates/unfold/forms/*',
-                          'templates/unfold/forms/helpers/*']}
+                          'templates/unfold/forms/helpers/*'],
+ 'unfold.contrib.import_export': ['templates/admin/import_export/*']}
 
 install_requires = \
 ['django>=3.2']
 
 setup_kwargs = {
     'name': 'django-unfold',
-    'version': '0.5.3',
+    'version': '0.6.0',
     'description': 'Clean & minimal Django admin theme based on Tailwind CSS',
-    'long_description': '![Screenshot - Objects Listing](https://github.com/remastr/django-unfold/raw/main/screenshot-1.jpg)\n\n![Screenshot - Login Page](https://github.com/remastr/django-unfold/raw/main/screenshot-2.jpg)\n\n## Unfold Django Admin Theme\n\nUnfold is a new theme for Django Admin incorporating some most common practises for building full-fledged admin areas.\n\n- **Visual**: provides new user interface based on Tailwind CSS framework\n- **Sidebar:** simplifies definition of custom sidebar navigation\n- **Dark mode:** supports both light and dark mode versions\n- **Configuration:** most of the basic options can be changed in settings.py\n- **Dependencies:** completely based only on `django.contrib.admin`\n- **Filters:** custom widgets for filters (e.g. numeric filter)\n- **Actions:** multiple ways how to define actions within different parts of admin\n\n## Table of Contents\n\n- [Unfold Django Admin Theme](#unfold-django-admin-theme)\n- [Table of Contents](#table-of-contents)\n- [Installation](#installation)\n- [Configuration](#configuration)\n  - [Available settings.py options](#available-settingspy-options)\n  - [Available unfold.admin.ModelAdmin options](#available-unfoldadminmodeladmin-options)\n- [Decorators](#decorators)\n  - [@display](#display)\n- [Actions](#actions)\n  - [Actions overview](#actions-overview)\n  - [Custom unfold @action decorator](#custom-unfold-action-decorator)\n  - [Action handler functions](#action-handler-functions)\n    - [For submit row action](#for-submit-row-action)\n    - [For global, row and detail action](#for-global-row-and-detail-action)\n  - [Action examples](#action-examples)\n- [Filters](#filters)\n- [User Admin Form](#user-admin-form)\n- [Adding Custom Styles and Scripts](#adding-custom-styles-and-scripts)\n- [Project Level Tailwind Stylesheet](#project-level-tailwind-stylesheet)\n- [Custom Admin Dashboard](#custom-admin-dashboard)\n- [Unfold Development](#unfold-development)\n  - [Pre-commit](#pre-commit)\n  - [Poetry Configuration](#poetry-configuration)\n  - [Compiling Tailwind](#compiling-tailwind)\n\n## Installation\n\nThe installation process is minimal. Everything what is needed after installation is to put new application at the beginning of **INSTALLED_APPS**. Default admin configuration in urls.py can stay as it is and there are no changes required.\n\n```python\n# settings.py\n\nINSTALLED_APPS = [\n    "unfold",  # before django.contrib.admin\n    "unfold.contrib.filters",  # optional, if special filters are needed\n    "unfold.contrib.forms",  # optional, if special form elements are needed\n    "django.contrib.admin",  # required\n]\n```\n\nIn case you need installation command below are the versions for `pip` and `poetry` which needs to be executed in shell.\n\n```bash\npip install django-unfold\npoetry add django-unfold\n```\n\nJust for an example below is the minimal admin configuration in terms of adding Unfold into URL paths.\n\n```python\n# urls.py\n\nfrom django.contrib import admin\nfrom django.urls import path\n\nurlpatterns = [\n    path("admin/", admin.site.urls),\n    # Other URL paths\n]\n```\n\nAfter installation, it is required that admin classes are going to inherit from custom `ModelAdmin` available in `unfold.admin`.\n\n```python\n# admin.py\n\nfrom django.contrib import admin\nfrom unfold.admin import ModelAdmin\n\n\n@admin.register(MyModel)\nclass CustomAdminClass(ModelAdmin):\n    pass\n```\n\n**Note:** Registered admin models coming from third party packages are not going to properly work with Unfold because of parent class. By default, these models are registered by using `django.contrib.admin.ModelAdmin` but it is needed to use `unfold.admin.ModelAdmin`. Solution for this problem is to unregister model and then again register it back by using `unfold.admin.ModelAdmin`.\n\n```python\n# admin.py\nfrom django.contrib import admin\nfrom django.contrib.auth.admin import UserAdmin as BaseUserAdmin\nfrom django.contrib.auth.models import User\n\nfrom unfold.admin import ModelAdmin\n\n\nadmin.site.unregister(User)\n\n\n@admin.register(User)\nclass UserAdmin(BaseUserAdmin, ModelAdmin):\n    pass\n```\n\n## Configuration\n\n### Available settings.py options\n```python\n# settings.py\n\nfrom django.templatetags.static import static\nfrom django.urls import reverse_lazy\nfrom django.utils.translation import gettext_lazy as _\n\nUNFOLD = {\n    "SITE_TITLE": None,\n    "SITE_HEADER": None,\n    "SITE_URL": "/",\n    "SITE_ICON": lambda request: static("logo.svg"),\n    "SITE_SYMBOL": "speed",  # symbol from icon set\n    "DASHBOARD_CALLBACK": "sample_app.dashboard_callback",\n    "LOGIN": {\n        "image": lambda r: static("sample/login-bg.jpg"),\n        "redirect_after": lambda r: reverse_lazy("admin:APP_MODEL_changelist"),\n    },\n    "STYLES": [\n        lambda request: static("css/style.css"),\n    ],\n    "SCRIPTS": [\n        lambda request: static("js/script.js"),\n    ],\n    "COLORS": {\n        "primary": {\n            "50": "250 245 255",\n            "100": "243 232 255",\n            "200": "233 213 255",\n            "300": "216 180 254",\n            "400": "192 132 252",\n            "500": "168 85 247",\n            "600": "147 51 234",\n            "700": "126 34 206",\n            "800": "107 33 168",\n            "900": "88 28 135",\n        },\n    },\n    "EXTENSIONS": {\n        "modeltranslation": {\n            "flags": {\n                "en": "🇬🇧",\n                "fr": "🇫🇷",\n                "nl": "🇧🇪",\n            },\n        },\n    },\n    "SIDEBAR": {\n        "show_search": False,  # Search in applications and models names\n        "show_all_applications": False,  # Dropdown with all applications and models\n        "navigation": [\n            {\n                "title": _("Navigation"),\n                "separator": True,  # Top border\n                "items": [\n                    {\n                        "title": _("Dashboard"),\n                        "icon": "dashboard",  # Supported icon set: https://fonts.google.com/icons\n                        "link": reverse_lazy("admin:index"),\n                        "badge": "sample_app.badge_callback",\n                    },\n                    {\n                        "title": _("Users"),\n                        "icon": "people",\n                        "link": reverse_lazy("admin:users_user_changelist"),\n                    },\n                ],\n            },\n        ],\n    },\n    "TABS": [\n        {\n            "models": [\n                "app_label.model_name_in_lowercase",\n            ],\n            "items": [\n                {\n                    "title": _("Your custom title"),\n                    "link": reverse_lazy("admin:app_label_model_name_changelist"),\n                },\n            ],\n        },\n    ],\n}\n\n\ndef dashboard_callback(request, context):\n    """\n    Callback to prepare custom variables for index template which is used as dashboard\n    template. It can be overridden in application by creating custom admin/index.html.\n    """\n    context.update(\n        {\n            "sample": "example",  # this will be injected into templates/admin/index.html\n        }\n    )\n    return context\n\n\ndef badge_callback(request):\n    return 3\n```\n\n### Available unfold.admin.ModelAdmin options\n\n```python\nfrom django import models\nfrom django.contrib import admin\n\nfrom unfold.admin import ModelAdmin\nfrom unfold.contrib.forms.widgets import WysiwygWidget\n\n\n@admin.register(MyModel)\nclass CustomAdminClass(ModelAdmin):\n    # Preprocess content of readonly fields before render\n    readonly_preprocess_fields = {\n        "model_field_name": "html.unescape",\n        "other_field_name": lambda content: content.strip(),\n    }\n\n    # Display submit button in filters\n    list_filter_submit = False\n\n    # Custom actions\n    actions_list = []  # Displayed above the results list\n    actions_row = []  # Displayed in a table row in results list\n    actions_detail = []  # Displayed at the top of for in object detail\n    actions_submit_line = []  # Displayed near save in object detail\n\n    formfield_overrides = {\n        models.TextField: WysiwygWidget,\n    }\n```\n\n## Decorators\n\n### @display\n\nUnfold introduces it\'s own `unfold.decorators.display` decorator. By default it has exactly same behavior as native `django.contrib.admin.decorators.display` but it adds same customizations which helps to extends default logic.\n\n`@display(label=True)`, `@display(label={"value1": "success"})` displays a result as a label. This option fits for different types of statuses. Label can be either boolean indicating we want to use label with default color or dict where the dict is responsible for displaying labels in different colors. At the moment these color combinations are supported: success(green), info(blue), danger(red) and warning(orange).\n\n`@display(header=True)` displays in results list two information in one table cell. Good example is when we want to display customer information, first line is going to be customer\'s name and right below the name display corresponding email address. Method with such a decorator is supposed to return a list with two elements `return "Full name", "E-mail address"`.\n\n```python\n# models.py\n\nfrom django.db.models import TextChoices\nfrom django.utils.translation import gettext_lazy as _\n\nfrom unfold.admin import ModelAdmin\nfrom unfold.decorators import display\n\n\nclass UserStatus(TextChoices):\n    ACTIVE = "ACTIVE", _("Active")\n    PENDING = "PENDING", _("Pending")\n    INACTIVE = "INACTIVE", _("Inactive")\n    CANCELLED = "CANCELLED", _("Cancelled")\n\n\nclass UserAdmin(ModelAdmin):\n    list_display = [\n        "display_as_two_line_heading",\n        "show_status",\n        "show_status_with_custom_label",\n    ]\n\n    @display(\n        description=_("Status"),\n        ordering="status",\n        label=True,\n        mapping={\n            UserStatus.ACTIVE: "success",\n            UserStatus.PENDING: "info",\n            UserStatus.INACTIVE: "warning",\n            UserStatus.CANCELLED: "danger",\n        },\n    )\n    def show_status(self, obj):\n        return obj.status\n\n    @display(description=_("Status with label"), ordering="status", label=True)\n    def show_status_with_custom_label(self, obj):\n        return obj.status, obj.get_status_display()\n\n    @display(header=True)\n    def display_as_two_line_heading(self, obj):\n        return "First main heading", "Smaller additional description"\n```\n\n## Actions\n\nIt is highly recommended to read the base [Django actions documentation](https://docs.djangoproject.com/en/4.2/ref/contrib/admin/actions/) before reading this section, since Unfold actions are derived from Django actions.\n\n### Actions overview\n\nBesides traditional actions selected from dropdown, Unfold supports several other types of actions. Following table\ngives overview of all available actions together with their recommended usage:\n\n| Type of action | Appearance                               | Usage                                                                                      | Examples of usage                      |\n|----------------|------------------------------------------|--------------------------------------------------------------------------------------------|----------------------------------------|\n| Default        | List view - top of listing (in dropdown) | Actions, where you want to select specific subset of instances to perform this action upon | Bulk deleting, bulk activation         |\n| Global         | List view - top of listing (as buttons)  | General actions for model, without selecting specific instances                            | Import, export                         |\n| Row            | List view - in each row                  | Action for one specific instance, executable from listing                                  | Activation, sync with external service |\n| Detail         | Detail view - top of detail              | Action for one specific instance, executable from detail                                   | Activation, sync with external service |\n| Submit line    | Detail view - near submit button         | Action performed during form submit (instance save)                                        | Publishing article together with save  |\n\n### Custom unfold @action decorator\n\nUnfold also uses custom `@action` decorator, supporting 2 more parameters in comparison to base `@action` decorator:\n- `url_path`: Action path name, used to override the path under which the action will be available\n  (if not provided, URL path will be generated by Unfold)\n- `attrs`: Dictionary of the additional attributes added to the `<a>` element, used for e.g. opening action in new tab (`{"target": "_blank"}`)\n\n### Action handler functions\n\nThis section provides explanation of how the action handler functions should be constructed for Unfold actions.\nFor default actions, follow official Django admin documentation.\n\n#### For submit row action\n\nSubmit row actions work a bit differently when compared to other custom Unfold actions.\nThese actions first invoke form save (same as if you hit `Save` button) and then lets you\nperform additional logic on already saved instance.\n\n#### For global, row and detail action\n\nAll these actions are based on custom URLs generated for each of them. Handler function for these views is\nbasically function based view.\n\nFor actions without intermediate steps, you can write all the logic inside handler directly. Request and object ID\nare both passed to these action handler functions, so you are free to fetch the instance from database and perform any\noperations with it. In the end, it is recommended to return redirect back to either detail or listing, based on where\nthe action was triggered from.\n\nFor actions with intermediate steps, it is recommended to use handler function only to redirect to custom URL with custom\nview. This view can be extended from base Unfold view, to have unified experience.\n\nIf that\'s confusing, there are examples for both these actions in next section.\n\n### Action examples\n\n```python\n# admin.py\n\nfrom django.db.models import Model\nfrom django.contrib.admin import register\nfrom django.shortcuts import redirect\nfrom django.urls import reverse_lazy\nfrom django.utils.translation import gettext_lazy as _\nfrom django.http import HttpRequest\nfrom unfold.admin import ModelAdmin\nfrom unfold.decorators import action\n\n\nclass User(Model):\n    pass\n\n\n@register(User)\nclass UserAdmin(ModelAdmin):\n    actions_list = ["changelist_global_action_import"]\n    actions_row = ["changelist_row_action_view_on_website"]\n    actions_detail = ["change_detail_action_block"]\n    actions_submit_line = ["submit_line_action_activate"]\n\n    @action(description=_("Save & Activate"))\n    def submit_line_action_activate(self, request: HttpRequest, obj: User):\n        """\n        If instance is modified in any way, it also needs to be saved,\n        since this handler is invoked after instance is saved.\n        :param request:\n        :param obj: Model instance that was manipulated, with changes already saved to database\n        :return: None, this handler should not return anything\n        """\n        obj.is_active = True\n        obj.save()\n\n    @action(description=_("Import"), url_path="import")\n    def changelist_global_action_import(self, request: HttpRequest):\n        """\n        Handler for global actions does not receive any queryset or object ids, because it is\n        meant to be used for general actions for given model.\n        :param request:\n        :return: View, as described in section above\n        """\n        # This is example of action redirecting to custom page, where the action will be handled\n        # (with intermediate steps)\n        return redirect(\n          reverse_lazy("view-where-import-will-be-handled")\n        )\n\n    @action(description=_("Row"), url_path="row-action", attrs={"target": "_blank"})\n    def changelist_row_action_view_on_website(self, request: HttpRequest, object_id: int):\n        """\n        Handler for list row action.\n        :param request:\n        :param object_id: ID of instance that this action was invoked for\n        :return: View, as described in section above\n        """\n        return redirect(f"https://example.com/{object_id}")\n\n    @action(description=_("Detail"), url_path="detail-action", attrs={"target": "_blank"})\n    def change_detail_action_block(self, request: HttpRequest, object_id: int):\n        """\n        Handler for detail action.\n        :param request:\n        :param object_id: ID of instance that this action was invoked for\n        :return: View, as described in section above\n        """\n        # This is example of action that handled whole logic inside handler\n        # function and redirects back to object detail\n        user = User.objects.get(pk=object_id)\n        user.block()\n        return redirect(\n            reverse_lazy("admin:users_user_change", args=(object_id,))\n        )\n```\n\n## Filters\n\nBy default, Django admin handles all filters as regular HTML links pointing at the same URL with different query parameters. This approach is for basic filtering more than enough. In the case of more advanced filtering by incorporating input fields, it is not going to work.\n\nCurrently, Unfold implements numeric filters inside `unfold.contrib.filters` application. In order to use these filters, it is required to add this application into `INSTALLED_APPS` in `settings.py` right after `unfold` application.\n\n```python\n# admin.py\n\nfrom django.contrib import admin\nfrom django.contrib.auth.models import User\n\nfrom unfold.admin import ModelAdmin\nfrom unfold.contrib.filters.admin import (\n    RangeNumericListFilter,\n    RangeNumericFilter,\n    SingleNumericFilter,\n    SliderNumericFilter,\n    RangeDateFilter,\n    RangeDateTimeFilter,\n)\n\n\nclass CustomSliderNumericFilter(SliderNumericFilter):\n    MAX_DECIMALS = 2\n    STEP = 10\n\n\nclass CustomRangeNumericListFilter(RangeNumericListFilter):\n    parameter_name = "items_count"\n    title = "items"\n\n\n@admin.register(User)\nclass YourModelAdmin(ModelAdmin):\n    list_filter_submit = True  # Submit button at the bottom of the filter\n    list_filter = (\n        ("field_A", SingleNumericFilter),  # Numeric single field search, __gte lookup\n        ("field_B", RangeNumericFilter),  # Numeric range search, __gte and __lte lookup\n        ("field_C", SliderNumericFilter),  # Numeric range filter but with slider\n        ("field_D", CustomSliderNumericFilter),  # Numeric filter with custom attributes\n        ("field_E", RangeDateFilter),  # Date filter\n        ("field_F", RangeDateTimeFilter),  # Datetime filter\n        CustomRangeNumericListFilter,  # Numeric range search not restricted to a model field\n    )\n\n    def get_queryset(self, request):\n        return super().get_queryset().annotate(items_count=Count("item", distinct=True))\n```\n\n\n\n## User Admin Form\n\nUser\'s admin in Django is specific as it contains several forms which are requiring custom styling. All of these forms has been inherited and accordingly adjusted. In user admin class it is needed to use these inherited form classes to enable custom styling matching rest of the website.\n\n```python\n# models.py\n\nfrom django.contrib.admin import register\nfrom django.contrib.auth.models import User\nfrom django.contrib.auth.admin import UserAdmin as BaseUserAdmin\n\nfrom unfold.admin import ModelAdmin\nfrom unfold.forms import AdminPasswordChangeForm, UserChangeForm, UserCreationForm\n\n\n@register(User)\nclass UserAdmin(BaseUserAdmin, ModelAdmin):\n    form = UserChangeForm\n    add_form = UserCreationForm\n    change_password_form = AdminPasswordChangeForm\n```\n\n## Adding Custom Styles and Scripts\n\nTo add new custom styles, for example for custom dashboard, it is possible to load them via **STYLES** key in **UNFOLD** dict. This key accepts a list of strings or lambda functions which will be loaded on all pages. JavaScript files can be loaded by using similar apprach, but **SCRIPTS** is used.\n\n```python\n# settings.py\n\nfrom django.templatetags.static import static\n\nUNFOLD = {\n    "STYLES": [\n        lambda request: static("css/style.css"),\n    ],\n    "SCRIPTS": [\n        lambda request: static("js/script.js"),\n    ],\n}\n```\n\n## Project Level Tailwind Stylesheet\n\nWhen creating custom dashboard or adding custom components, it is needed to add own styles. Adding custom styles is described above. Most of the time, it is supposed that new elements are going to match with the rest of the administration panel. First of all, create tailwind.config.js in your application. Below is located minimal configuration for this file.\n\n```javascript\n// tailwind.config.js\n\nmodule.exports = {\n    content: [\n        "./your_project/**/*.{html,py,js}"\n    ],\n    // In case custom colors are defined in UNFOLD["COLORS"]\n    colors: {\n        primary: {\n          100: "rgb(var(--color-primary-100) / <alpha-value>)",\n          200: "rgb(var(--color-primary-200) / <alpha-value>)",\n          300: "rgb(var(--color-primary-300) / <alpha-value>)",\n          400: "rgb(var(--color-primary-400) / <alpha-value>)",\n          500: "rgb(var(--color-primary-500) / <alpha-value>)",\n          600: "rgb(var(--color-primary-600) / <alpha-value>)",\n          700: "rgb(var(--color-primary-700) / <alpha-value>)",\n          800: "rgb(var(--color-primary-800) / <alpha-value>)",\n          900: "rgb(var(--color-primary-900) / <alpha-value>)"\n        }\n    }\n}\n```\n\nOnce the configuration file is set, it is possible to compile new styles which can be loaded into admin by using **STYLES** key in **UNFOLD** dict.\n\n```bash\nnpx tailwindcss  -o your_project/static/css/styles.css --watch --minify\n```\n\n## Custom Admin Dashboard\n\nThe most common thing which needs to be adjusted for each project in admin is the dashboard. By default Unfold does not provide any dashboard components. The default dashboard experience with list of all applications and models is kept with proper styling matching rest of the components but thats it. Anyway, Unfold was created that creation of custom dashboard will be streamlined.\n\nCreate `templates/admin/index.html` in your project and paste the base template below into it. By default, all your custom styles here are not compiled because CSS classes are located in your specific project. Here it is needed to set up the Tailwind for your project and all requried instructions are located in [Project Level Tailwind Stylesheet](#project-level-tailwind-stylesheet) chapter.\n\n```\n{% extends \'unfold/layouts/base_simple.html\' %}\n\n{% load cache humanize i18n %}\n\n{% block breadcrumbs %}{% endblock %}\n\n{% block title %}{% if subtitle %}{{ subtitle }} | {% endif %}{{ title }} | {{ site_title|default:_(\'Django site admin\') }}{% endblock %}\n\n{% block branding %}\n    <h1 id="site-name"><a href="{% url \'admin:index\' %}">{{ site_header|default:_(\'Django administration\') }}</a></h1>\n{% endblock %}\n\n{% block content %}\n    Start creating your own Tailwind components here\n{% endblock %}\n```\n\nNote: In case that it is needed to pass custom variables into dashboard tamplate, check **DASHOARD_CALLBACK** in **UNFOLD** dict.\n\n## Unfold Development\n\n### Pre-commit\n\nBefore adding any source code, it is recommended to have pre-commit installed on your local computer to check for all potential issues when comitting the code.\n\n```bash\npip install pre-commit\npre-commit install\npre-commit install --hook-type commit-msg\n```\n\n### Poetry Configuration\n\nTo add a new feature or fix the easiest approach is to use django-unfold in combination with Poetry. The process looks like:\n\n- Install django-unfold via `poetry add django-unfold`\n- After that it is needed to git clone the repository somewhere on local computer.\n- Edit *pyproject.toml* and update django-unfold line `django-unfold = { path = "../django-unfold", develop = true}`\n- Lock and update via `poetry lock && poetry update`\n\n### Compiling Tailwind\n\nAt the moment project contains package.json with all dependencies required to compile new CSS file. Tailwind configuration file is set to check all html, js and py files for Tailwind\'s classeses occurrences.\n\n```bash\nnpm install\nnpx tailwindcss -i styles.css -o src/unfold/static/unfold/css/styles.css --watch --minify\n\nnpm run tailwind:watch # run after each change in code\nnpm run tailwind:build # run once\n```\n\nSome components like datepickers, calendars or selectors in admin was not possible to style by overriding html templates so their default styles are overriden in **styles.css**.\n\nNone: most of the custom styles localted in style.css are created via `@apply some-tailwind-class;`.\n',
+    'long_description': '![Screenshot - Objects Listing](https://github.com/remastr/django-unfold/raw/main/screenshot-1.jpg)\n\n![Screenshot - Login Page](https://github.com/remastr/django-unfold/raw/main/screenshot-2.jpg)\n\n## Unfold Django Admin Theme\n\nUnfold is a new theme for Django Admin incorporating some most common practises for building full-fledged admin areas.\n\n- **Visual**: provides new user interface based on Tailwind CSS framework\n- **Sidebar:** simplifies definition of custom sidebar navigation\n- **Dark mode:** supports both light and dark mode versions\n- **Configuration:** most of the basic options can be changed in settings.py\n- **Dependencies:** completely based only on `django.contrib.admin`\n- **Filters:** custom widgets for filters (e.g. numeric filter)\n- **Actions:** multiple ways how to define actions within different parts of admin\n\n## Table of Contents\n\n- [Unfold Django Admin Theme](#unfold-django-admin-theme)\n- [Table of Contents](#table-of-contents)\n- [Installation](#installation)\n- [Configuration](#configuration)\n  - [Available settings.py options](#available-settingspy-options)\n  - [Available unfold.admin.ModelAdmin options](#available-unfoldadminmodeladmin-options)\n- [Decorators](#decorators)\n  - [@display](#display)\n- [Actions](#actions)\n  - [Actions overview](#actions-overview)\n  - [Custom unfold @action decorator](#custom-unfold-action-decorator)\n  - [Action handler functions](#action-handler-functions)\n    - [For submit row action](#for-submit-row-action)\n    - [For global, row and detail action](#for-global-row-and-detail-action)\n  - [Action examples](#action-examples)\n- [Filters](#filters)\n- [Third party packages](#third-party-packages)\n  - [django-import-export](#django-import-export)\n- [User Admin Form](#user-admin-form)\n- [Adding Custom Styles and Scripts](#adding-custom-styles-and-scripts)\n- [Project Level Tailwind Stylesheet](#project-level-tailwind-stylesheet)\n- [Custom Admin Dashboard](#custom-admin-dashboard)\n- [Unfold Development](#unfold-development)\n  - [Pre-commit](#pre-commit)\n  - [Poetry Configuration](#poetry-configuration)\n  - [Compiling Tailwind](#compiling-tailwind)\n\n## Installation\n\nThe installation process is minimal. Everything what is needed after installation is to put new application at the beginning of **INSTALLED_APPS**. Default admin configuration in urls.py can stay as it is and there are no changes required.\n\n```python\n# settings.py\n\nINSTALLED_APPS = [\n    "unfold",  # before django.contrib.admin\n    "unfold.contrib.filters",  # optional, if special filters are needed\n    "unfold.contrib.forms",  # optional, if special form elements are needed\n    "unfold.contrib.import_export",  # optional, if django-import-export package is used\n    "django.contrib.admin",  # required\n]\n```\n\nIn case you need installation command below are the versions for `pip` and `poetry` which needs to be executed in shell.\n\n```bash\npip install django-unfold\npoetry add django-unfold\n```\n\nJust for an example below is the minimal admin configuration in terms of adding Unfold into URL paths.\n\n```python\n# urls.py\n\nfrom django.contrib import admin\nfrom django.urls import path\n\nurlpatterns = [\n    path("admin/", admin.site.urls),\n    # Other URL paths\n]\n```\n\nAfter installation, it is required that admin classes are going to inherit from custom `ModelAdmin` available in `unfold.admin`.\n\n```python\n# admin.py\n\nfrom django.contrib import admin\nfrom unfold.admin import ModelAdmin\n\n\n@admin.register(MyModel)\nclass CustomAdminClass(ModelAdmin):\n    pass\n```\n\n**Note:** Registered admin models coming from third party packages are not going to properly work with Unfold because of parent class. By default, these models are registered by using `django.contrib.admin.ModelAdmin` but it is needed to use `unfold.admin.ModelAdmin`. Solution for this problem is to unregister model and then again register it back by using `unfold.admin.ModelAdmin`.\n\n```python\n# admin.py\nfrom django.contrib import admin\nfrom django.contrib.auth.admin import UserAdmin as BaseUserAdmin\nfrom django.contrib.auth.models import User\n\nfrom unfold.admin import ModelAdmin\n\n\nadmin.site.unregister(User)\n\n\n@admin.register(User)\nclass UserAdmin(BaseUserAdmin, ModelAdmin):\n    pass\n```\n\n## Configuration\n\n### Available settings.py options\n```python\n# settings.py\n\nfrom django.templatetags.static import static\nfrom django.urls import reverse_lazy\nfrom django.utils.translation import gettext_lazy as _\n\nUNFOLD = {\n    "SITE_TITLE": None,\n    "SITE_HEADER": None,\n    "SITE_URL": "/",\n    "SITE_ICON": lambda request: static("logo.svg"),\n    "SITE_SYMBOL": "speed",  # symbol from icon set\n    "DASHBOARD_CALLBACK": "sample_app.dashboard_callback",\n    "LOGIN": {\n        "image": lambda r: static("sample/login-bg.jpg"),\n        "redirect_after": lambda r: reverse_lazy("admin:APP_MODEL_changelist"),\n    },\n    "STYLES": [\n        lambda request: static("css/style.css"),\n    ],\n    "SCRIPTS": [\n        lambda request: static("js/script.js"),\n    ],\n    "COLORS": {\n        "primary": {\n            "50": "250 245 255",\n            "100": "243 232 255",\n            "200": "233 213 255",\n            "300": "216 180 254",\n            "400": "192 132 252",\n            "500": "168 85 247",\n            "600": "147 51 234",\n            "700": "126 34 206",\n            "800": "107 33 168",\n            "900": "88 28 135",\n        },\n    },\n    "EXTENSIONS": {\n        "modeltranslation": {\n            "flags": {\n                "en": "🇬🇧",\n                "fr": "🇫🇷",\n                "nl": "🇧🇪",\n            },\n        },\n    },\n    "SIDEBAR": {\n        "show_search": False,  # Search in applications and models names\n        "show_all_applications": False,  # Dropdown with all applications and models\n        "navigation": [\n            {\n                "title": _("Navigation"),\n                "separator": True,  # Top border\n                "items": [\n                    {\n                        "title": _("Dashboard"),\n                        "icon": "dashboard",  # Supported icon set: https://fonts.google.com/icons\n                        "link": reverse_lazy("admin:index"),\n                        "badge": "sample_app.badge_callback",\n                    },\n                    {\n                        "title": _("Users"),\n                        "icon": "people",\n                        "link": reverse_lazy("admin:users_user_changelist"),\n                    },\n                ],\n            },\n        ],\n    },\n    "TABS": [\n        {\n            "models": [\n                "app_label.model_name_in_lowercase",\n            ],\n            "items": [\n                {\n                    "title": _("Your custom title"),\n                    "link": reverse_lazy("admin:app_label_model_name_changelist"),\n                },\n            ],\n        },\n    ],\n}\n\n\ndef dashboard_callback(request, context):\n    """\n    Callback to prepare custom variables for index template which is used as dashboard\n    template. It can be overridden in application by creating custom admin/index.html.\n    """\n    context.update(\n        {\n            "sample": "example",  # this will be injected into templates/admin/index.html\n        }\n    )\n    return context\n\n\ndef badge_callback(request):\n    return 3\n```\n\n### Available unfold.admin.ModelAdmin options\n\n```python\nfrom django import models\nfrom django.contrib import admin\n\nfrom unfold.admin import ModelAdmin\nfrom unfold.contrib.forms.widgets import WysiwygWidget\n\n\n@admin.register(MyModel)\nclass CustomAdminClass(ModelAdmin):\n    # Preprocess content of readonly fields before render\n    readonly_preprocess_fields = {\n        "model_field_name": "html.unescape",\n        "other_field_name": lambda content: content.strip(),\n    }\n\n    # Display submit button in filters\n    list_filter_submit = False\n\n    # Custom actions\n    actions_list = []  # Displayed above the results list\n    actions_row = []  # Displayed in a table row in results list\n    actions_detail = []  # Displayed at the top of for in object detail\n    actions_submit_line = []  # Displayed near save in object detail\n\n    formfield_overrides = {\n        models.TextField: WysiwygWidget,\n    }\n```\n\n## Decorators\n\n### @display\n\nUnfold introduces it\'s own `unfold.decorators.display` decorator. By default it has exactly same behavior as native `django.contrib.admin.decorators.display` but it adds same customizations which helps to extends default logic.\n\n`@display(label=True)`, `@display(label={"value1": "success"})` displays a result as a label. This option fits for different types of statuses. Label can be either boolean indicating we want to use label with default color or dict where the dict is responsible for displaying labels in different colors. At the moment these color combinations are supported: success(green), info(blue), danger(red) and warning(orange).\n\n`@display(header=True)` displays in results list two information in one table cell. Good example is when we want to display customer information, first line is going to be customer\'s name and right below the name display corresponding email address. Method with such a decorator is supposed to return a list with two elements `return "Full name", "E-mail address"`.\n\n```python\n# models.py\n\nfrom django.db.models import TextChoices\nfrom django.utils.translation import gettext_lazy as _\n\nfrom unfold.admin import ModelAdmin\nfrom unfold.decorators import display\n\n\nclass UserStatus(TextChoices):\n    ACTIVE = "ACTIVE", _("Active")\n    PENDING = "PENDING", _("Pending")\n    INACTIVE = "INACTIVE", _("Inactive")\n    CANCELLED = "CANCELLED", _("Cancelled")\n\n\nclass UserAdmin(ModelAdmin):\n    list_display = [\n        "display_as_two_line_heading",\n        "show_status",\n        "show_status_with_custom_label",\n    ]\n\n    @display(\n        description=_("Status"),\n        ordering="status",\n        label=True,\n        mapping={\n            UserStatus.ACTIVE: "success",\n            UserStatus.PENDING: "info",\n            UserStatus.INACTIVE: "warning",\n            UserStatus.CANCELLED: "danger",\n        },\n    )\n    def show_status(self, obj):\n        return obj.status\n\n    @display(description=_("Status with label"), ordering="status", label=True)\n    def show_status_with_custom_label(self, obj):\n        return obj.status, obj.get_status_display()\n\n    @display(header=True)\n    def display_as_two_line_heading(self, obj):\n        return "First main heading", "Smaller additional description"\n```\n\n## Actions\n\nIt is highly recommended to read the base [Django actions documentation](https://docs.djangoproject.com/en/4.2/ref/contrib/admin/actions/) before reading this section, since Unfold actions are derived from Django actions.\n\n### Actions overview\n\nBesides traditional actions selected from dropdown, Unfold supports several other types of actions. Following table\ngives overview of all available actions together with their recommended usage:\n\n| Type of action | Appearance                               | Usage                                                                                      | Examples of usage                      |\n|----------------|------------------------------------------|--------------------------------------------------------------------------------------------|----------------------------------------|\n| Default        | List view - top of listing (in dropdown) | Actions, where you want to select specific subset of instances to perform this action upon | Bulk deleting, bulk activation         |\n| Global         | List view - top of listing (as buttons)  | General actions for model, without selecting specific instances                            | Import, export                         |\n| Row            | List view - in each row                  | Action for one specific instance, executable from listing                                  | Activation, sync with external service |\n| Detail         | Detail view - top of detail              | Action for one specific instance, executable from detail                                   | Activation, sync with external service |\n| Submit line    | Detail view - near submit button         | Action performed during form submit (instance save)                                        | Publishing article together with save  |\n\n### Custom unfold @action decorator\n\nUnfold also uses custom `@action` decorator, supporting 2 more parameters in comparison to base `@action` decorator:\n- `url_path`: Action path name, used to override the path under which the action will be available\n  (if not provided, URL path will be generated by Unfold)\n- `attrs`: Dictionary of the additional attributes added to the `<a>` element, used for e.g. opening action in new tab (`{"target": "_blank"}`)\n\n### Action handler functions\n\nThis section provides explanation of how the action handler functions should be constructed for Unfold actions.\nFor default actions, follow official Django admin documentation.\n\n#### For submit row action\n\nSubmit row actions work a bit differently when compared to other custom Unfold actions.\nThese actions first invoke form save (same as if you hit `Save` button) and then lets you\nperform additional logic on already saved instance.\n\n#### For global, row and detail action\n\nAll these actions are based on custom URLs generated for each of them. Handler function for these views is\nbasically function based view.\n\nFor actions without intermediate steps, you can write all the logic inside handler directly. Request and object ID\nare both passed to these action handler functions, so you are free to fetch the instance from database and perform any\noperations with it. In the end, it is recommended to return redirect back to either detail or listing, based on where\nthe action was triggered from.\n\nFor actions with intermediate steps, it is recommended to use handler function only to redirect to custom URL with custom\nview. This view can be extended from base Unfold view, to have unified experience.\n\nIf that\'s confusing, there are examples for both these actions in next section.\n\n### Action examples\n\n```python\n# admin.py\n\nfrom django.db.models import Model\nfrom django.contrib.admin import register\nfrom django.shortcuts import redirect\nfrom django.urls import reverse_lazy\nfrom django.utils.translation import gettext_lazy as _\nfrom django.http import HttpRequest\nfrom unfold.admin import ModelAdmin\nfrom unfold.decorators import action\n\n\nclass User(Model):\n    pass\n\n\n@register(User)\nclass UserAdmin(ModelAdmin):\n    actions_list = ["changelist_global_action_import"]\n    actions_row = ["changelist_row_action_view_on_website"]\n    actions_detail = ["change_detail_action_block"]\n    actions_submit_line = ["submit_line_action_activate"]\n\n    @action(description=_("Save & Activate"))\n    def submit_line_action_activate(self, request: HttpRequest, obj: User):\n        """\n        If instance is modified in any way, it also needs to be saved,\n        since this handler is invoked after instance is saved.\n        :param request:\n        :param obj: Model instance that was manipulated, with changes already saved to database\n        :return: None, this handler should not return anything\n        """\n        obj.is_active = True\n        obj.save()\n\n    @action(description=_("Import"), url_path="import")\n    def changelist_global_action_import(self, request: HttpRequest):\n        """\n        Handler for global actions does not receive any queryset or object ids, because it is\n        meant to be used for general actions for given model.\n        :param request:\n        :return: View, as described in section above\n        """\n        # This is example of action redirecting to custom page, where the action will be handled\n        # (with intermediate steps)\n        return redirect(\n          reverse_lazy("view-where-import-will-be-handled")\n        )\n\n    @action(description=_("Row"), url_path="row-action", attrs={"target": "_blank"})\n    def changelist_row_action_view_on_website(self, request: HttpRequest, object_id: int):\n        """\n        Handler for list row action.\n        :param request:\n        :param object_id: ID of instance that this action was invoked for\n        :return: View, as described in section above\n        """\n        return redirect(f"https://example.com/{object_id}")\n\n    @action(description=_("Detail"), url_path="detail-action", attrs={"target": "_blank"})\n    def change_detail_action_block(self, request: HttpRequest, object_id: int):\n        """\n        Handler for detail action.\n        :param request:\n        :param object_id: ID of instance that this action was invoked for\n        :return: View, as described in section above\n        """\n        # This is example of action that handled whole logic inside handler\n        # function and redirects back to object detail\n        user = User.objects.get(pk=object_id)\n        user.block()\n        return redirect(\n            reverse_lazy("admin:users_user_change", args=(object_id,))\n        )\n```\n\n## Filters\n\nBy default, Django admin handles all filters as regular HTML links pointing at the same URL with different query parameters. This approach is for basic filtering more than enough. In the case of more advanced filtering by incorporating input fields, it is not going to work.\n\nCurrently, Unfold implements numeric filters inside `unfold.contrib.filters` application. In order to use these filters, it is required to add this application into `INSTALLED_APPS` in `settings.py` right after `unfold` application.\n\n```python\n# admin.py\n\nfrom django.contrib import admin\nfrom django.contrib.auth.models import User\n\nfrom unfold.admin import ModelAdmin\nfrom unfold.contrib.filters.admin import (\n    RangeNumericListFilter,\n    RangeNumericFilter,\n    SingleNumericFilter,\n    SliderNumericFilter,\n    RangeDateFilter,\n    RangeDateTimeFilter,\n)\n\n\nclass CustomSliderNumericFilter(SliderNumericFilter):\n    MAX_DECIMALS = 2\n    STEP = 10\n\n\nclass CustomRangeNumericListFilter(RangeNumericListFilter):\n    parameter_name = "items_count"\n    title = "items"\n\n\n@admin.register(User)\nclass YourModelAdmin(ModelAdmin):\n    list_filter_submit = True  # Submit button at the bottom of the filter\n    list_filter = (\n        ("field_A", SingleNumericFilter),  # Numeric single field search, __gte lookup\n        ("field_B", RangeNumericFilter),  # Numeric range search, __gte and __lte lookup\n        ("field_C", SliderNumericFilter),  # Numeric range filter but with slider\n        ("field_D", CustomSliderNumericFilter),  # Numeric filter with custom attributes\n        ("field_E", RangeDateFilter),  # Date filter\n        ("field_F", RangeDateTimeFilter),  # Datetime filter\n        CustomRangeNumericListFilter,  # Numeric range search not restricted to a model field\n    )\n\n    def get_queryset(self, request):\n        return super().get_queryset().annotate(items_count=Count("item", distinct=True))\n```\n\n\n## Third party packages\n\n\n### django-import-export\n\nTo get proper visual appearance for django-import-export, two things are needed\n\n1. Add `unfold.contrib.import_export` to `INSTALLED_APPS` at the begging of the file. This action will override all templates coming from the plugin.\n2. Change `import_form_class` and `export_form_class` in ModelAdmin which is inheriting from `ImportExportModelAdmin`. This chunk of code is responsible for adding proper styling to form elements.\n\n```python\nfrom unfold.admin import ModelAdmin\nfrom unfold.contrib.import_export.forms import ExportForm, ImportForm\n\nclass ExampleAdmin(ModelAdmin, ImportExportModelAdmin):\n    import_form_class = ImportForm\n    export_form_class = ExportForm\n```\n\n## User Admin Form\n\nUser\'s admin in Django is specific as it contains several forms which are requiring custom styling. All of these forms has been inherited and accordingly adjusted. In user admin class it is needed to use these inherited form classes to enable custom styling matching rest of the website.\n\n```python\n# models.py\n\nfrom django.contrib.admin import register\nfrom django.contrib.auth.models import User\nfrom django.contrib.auth.admin import UserAdmin as BaseUserAdmin\n\nfrom unfold.admin import ModelAdmin\nfrom unfold.forms import AdminPasswordChangeForm, UserChangeForm, UserCreationForm\n\n\n@register(User)\nclass UserAdmin(BaseUserAdmin, ModelAdmin):\n    form = UserChangeForm\n    add_form = UserCreationForm\n    change_password_form = AdminPasswordChangeForm\n```\n\n## Adding Custom Styles and Scripts\n\nTo add new custom styles, for example for custom dashboard, it is possible to load them via **STYLES** key in **UNFOLD** dict. This key accepts a list of strings or lambda functions which will be loaded on all pages. JavaScript files can be loaded by using similar apprach, but **SCRIPTS** is used.\n\n```python\n# settings.py\n\nfrom django.templatetags.static import static\n\nUNFOLD = {\n    "STYLES": [\n        lambda request: static("css/style.css"),\n    ],\n    "SCRIPTS": [\n        lambda request: static("js/script.js"),\n    ],\n}\n```\n\n## Project Level Tailwind Stylesheet\n\nWhen creating custom dashboard or adding custom components, it is needed to add own styles. Adding custom styles is described above. Most of the time, it is supposed that new elements are going to match with the rest of the administration panel. First of all, create tailwind.config.js in your application. Below is located minimal configuration for this file.\n\n```javascript\n// tailwind.config.js\n\nmodule.exports = {\n    content: [\n        "./your_project/**/*.{html,py,js}"\n    ],\n    // In case custom colors are defined in UNFOLD["COLORS"]\n    colors: {\n        primary: {\n          100: "rgb(var(--color-primary-100) / <alpha-value>)",\n          200: "rgb(var(--color-primary-200) / <alpha-value>)",\n          300: "rgb(var(--color-primary-300) / <alpha-value>)",\n          400: "rgb(var(--color-primary-400) / <alpha-value>)",\n          500: "rgb(var(--color-primary-500) / <alpha-value>)",\n          600: "rgb(var(--color-primary-600) / <alpha-value>)",\n          700: "rgb(var(--color-primary-700) / <alpha-value>)",\n          800: "rgb(var(--color-primary-800) / <alpha-value>)",\n          900: "rgb(var(--color-primary-900) / <alpha-value>)"\n        }\n    }\n}\n```\n\nOnce the configuration file is set, it is possible to compile new styles which can be loaded into admin by using **STYLES** key in **UNFOLD** dict.\n\n```bash\nnpx tailwindcss  -o your_project/static/css/styles.css --watch --minify\n```\n\n## Custom Admin Dashboard\n\nThe most common thing which needs to be adjusted for each project in admin is the dashboard. By default Unfold does not provide any dashboard components. The default dashboard experience with list of all applications and models is kept with proper styling matching rest of the components but thats it. Anyway, Unfold was created that creation of custom dashboard will be streamlined.\n\nCreate `templates/admin/index.html` in your project and paste the base template below into it. By default, all your custom styles here are not compiled because CSS classes are located in your specific project. Here it is needed to set up the Tailwind for your project and all requried instructions are located in [Project Level Tailwind Stylesheet](#project-level-tailwind-stylesheet) chapter.\n\n```\n{% extends \'unfold/layouts/base_simple.html\' %}\n\n{% load cache humanize i18n %}\n\n{% block breadcrumbs %}{% endblock %}\n\n{% block title %}{% if subtitle %}{{ subtitle }} | {% endif %}{{ title }} | {{ site_title|default:_(\'Django site admin\') }}{% endblock %}\n\n{% block branding %}\n    <h1 id="site-name"><a href="{% url \'admin:index\' %}">{{ site_header|default:_(\'Django administration\') }}</a></h1>\n{% endblock %}\n\n{% block content %}\n    Start creating your own Tailwind components here\n{% endblock %}\n```\n\nNote: In case that it is needed to pass custom variables into dashboard tamplate, check **DASHOARD_CALLBACK** in **UNFOLD** dict.\n\n## Unfold Development\n\n### Pre-commit\n\nBefore adding any source code, it is recommended to have pre-commit installed on your local computer to check for all potential issues when comitting the code.\n\n```bash\npip install pre-commit\npre-commit install\npre-commit install --hook-type commit-msg\n```\n\n### Poetry Configuration\n\nTo add a new feature or fix the easiest approach is to use django-unfold in combination with Poetry. The process looks like:\n\n- Install django-unfold via `poetry add django-unfold`\n- After that it is needed to git clone the repository somewhere on local computer.\n- Edit *pyproject.toml* and update django-unfold line `django-unfold = { path = "../django-unfold", develop = true}`\n- Lock and update via `poetry lock && poetry update`\n\n### Compiling Tailwind\n\nAt the moment project contains package.json with all dependencies required to compile new CSS file. Tailwind configuration file is set to check all html, js and py files for Tailwind\'s classeses occurrences.\n\n```bash\nnpm install\nnpx tailwindcss -i styles.css -o src/unfold/static/unfold/css/styles.css --watch --minify\n\nnpm run tailwind:watch # run after each change in code\nnpm run tailwind:build # run once\n```\n\nSome components like datepickers, calendars or selectors in admin was not possible to style by overriding html templates so their default styles are overriden in **styles.css**.\n\nNone: most of the custom styles localted in style.css are created via `@apply some-tailwind-class;`.\n',
     'author': 'None',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
-    'url': 'https://github.com/remastr/django-unfold',
+    'url': 'https://unfoldadmin.com',
     'package_dir': package_dir,
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'python_requires': '>=3.8',
 }
```

### Comparing `django_unfold-0.5.3/PKG-INFO` & `django_unfold-0.6.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: django-unfold
-Version: 0.5.3
+Version: 0.6.0
 Summary: Clean & minimal Django admin theme based on Tailwind CSS
-Home-page: https://github.com/remastr/django-unfold
+Home-page: https://unfoldadmin.com
 License: MIT
 Keywords: django,admin,tailwind,theme
 Requires-Python: >=3.8
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -54,14 +54,16 @@
   - [Actions overview](#actions-overview)
   - [Custom unfold @action decorator](#custom-unfold-action-decorator)
   - [Action handler functions](#action-handler-functions)
     - [For submit row action](#for-submit-row-action)
     - [For global, row and detail action](#for-global-row-and-detail-action)
   - [Action examples](#action-examples)
 - [Filters](#filters)
+- [Third party packages](#third-party-packages)
+  - [django-import-export](#django-import-export)
 - [User Admin Form](#user-admin-form)
 - [Adding Custom Styles and Scripts](#adding-custom-styles-and-scripts)
 - [Project Level Tailwind Stylesheet](#project-level-tailwind-stylesheet)
 - [Custom Admin Dashboard](#custom-admin-dashboard)
 - [Unfold Development](#unfold-development)
   - [Pre-commit](#pre-commit)
   - [Poetry Configuration](#poetry-configuration)
@@ -74,14 +76,15 @@
 ```python
 # settings.py
 
 INSTALLED_APPS = [
     "unfold",  # before django.contrib.admin
     "unfold.contrib.filters",  # optional, if special filters are needed
     "unfold.contrib.forms",  # optional, if special form elements are needed
+    "unfold.contrib.import_export",  # optional, if django-import-export package is used
     "django.contrib.admin",  # required
 ]
 ```
 
 In case you need installation command below are the versions for `pip` and `poetry` which needs to be executed in shell.
 
 ```bash
@@ -507,14 +510,32 @@
     )
 
     def get_queryset(self, request):
         return super().get_queryset().annotate(items_count=Count("item", distinct=True))
 ```
 
 
+## Third party packages
+
+
+### django-import-export
+
+To get proper visual appearance for django-import-export, two things are needed
+
+1. Add `unfold.contrib.import_export` to `INSTALLED_APPS` at the begging of the file. This action will override all templates coming from the plugin.
+2. Change `import_form_class` and `export_form_class` in ModelAdmin which is inheriting from `ImportExportModelAdmin`. This chunk of code is responsible for adding proper styling to form elements.
+
+```python
+from unfold.admin import ModelAdmin
+from unfold.contrib.import_export.forms import ExportForm, ImportForm
+
+class ExampleAdmin(ModelAdmin, ImportExportModelAdmin):
+    import_form_class = ImportForm
+    export_form_class = ExportForm
+```
 
 ## User Admin Form
 
 User's admin in Django is specific as it contains several forms which are requiring custom styling. All of these forms has been inherited and accordingly adjusted. In user admin class it is needed to use these inherited form classes to enable custom styling matching rest of the website.
 
 ```python
 # models.py
```

