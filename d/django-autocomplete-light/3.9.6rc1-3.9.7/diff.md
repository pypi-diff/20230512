# Comparing `tmp/django-autocomplete-light-3.9.6rc1.tar.gz` & `tmp/django-autocomplete-light-3.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-autocomplete-light-3.9.6rc1.tar", last modified: Fri May 12 15:55:59 2023, max compression
+gzip compressed data, was "django-autocomplete-light-3.9.7.tar", last modified: Fri May 12 16:01:04 2023, max compression
```

## Comparing `django-autocomplete-light-3.9.6rc1.tar` & `django-autocomplete-light-3.9.7.tar`

### file list

```diff
@@ -1,276 +1,276 @@
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-05-12 15:55:59.114524 django-autocomplete-light-3.9.6rc1/
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1625 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.6rc1/AUTHORS
--rw-r--r--   0 jpic      (1000) jpic      (1000)    47188 2023-05-12 15:55:58.000000 django-autocomplete-light-3.9.6rc1/CHANGELOG
--rw-r--r--   0 jpic      (1000) jpic      (1000)    47188 2023-05-12 15:55:58.000000 django-autocomplete-light-3.9.6rc1/CHANGES.txt
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1076 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.6rc1/LICENSE
--rw-r--r--   0 jpic      (1000) jpic      (1000)      302 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.6rc1/MANIFEST.in
--rw-r--r--   0 jpic      (1000) jpic      (1000)     3326 2023-05-12 15:55:59.114524 django-autocomplete-light-3.9.6rc1/PKG-INFO
--rw-r--r--   0 jpic      (1000) jpic      (1000)     2221 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.6rc1/README
--rw-r--r--   0 jpic      (1000) jpic      (1000)     2221 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.6rc1/README.rst
--rw-r--r--   0 jpic      (1000) jpic      (1000)       38 2023-05-12 15:55:59.114524 django-autocomplete-light-3.9.6rc1/setup.cfg
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1836 2023-05-12 15:55:58.000000 django-autocomplete-light-3.9.6rc1/setup.py
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-05-12 15:55:59.104524 django-autocomplete-light-3.9.6rc1/src/
--rw-r--r--   0 jpic      (1000) jpic      (1000)       37 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.6rc1/src/__init__.py
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-05-12 15:55:59.104524 django-autocomplete-light-3.9.6rc1/src/dal/
--rw-r--r--   0 jpic      (1000) jpic      (1000)      112 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.6rc1/src/dal/__init__.py
--rw-r--r--   0 jpic      (1000) jpic      (1000)     2751 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.6rc1/src/dal/autocomplete.py
--rw-r--r--   0 jpic      (1000) jpic      (1000)     6762 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.6rc1/src/dal/forms.py
--rw-r--r--   0 jpic      (1000) jpic      (1000)     4633 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.6rc1/src/dal/forward.py
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-05-12 15:55:59.101191 django-autocomplete-light-3.9.6rc1/src/dal/static/
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-05-12 15:55:59.104524 django-autocomplete-light-3.9.6rc1/src/dal/static/autocomplete_light/
--rw-r--r--   0 jpic      (1000) jpic      (1000)    18327 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.6rc1/src/dal/static/autocomplete_light/autocomplete_light.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     5423 2023-05-12 15:55:58.000000 django-autocomplete-light-3.9.6rc1/src/dal/static/autocomplete_light/autocomplete_light.min.js
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-05-12 15:55:59.107857 django-autocomplete-light-3.9.6rc1/src/dal/static/autocomplete_light/i18n/
--rw-r--r--   0 jpic      (1000) jpic      (1000)      950 2023-05-12 15:55:57.000000 django-autocomplete-light-3.9.6rc1/src/dal/static/autocomplete_light/i18n/af.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)      989 2023-05-12 15:55:57.000000 django-autocomplete-light-3.9.6rc1/src/dal/static/autocomplete_light/i18n/ar.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)      805 2023-05-12 15:55:57.000000 django-autocomplete-light-3.9.6rc1/src/dal/static/autocomplete_light/i18n/az.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1052 2023-05-12 15:55:57.000000 django-autocomplete-light-3.9.6rc1/src/dal/static/autocomplete_light/i18n/bg.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1359 2023-05-12 15:55:57.000000 django-autocomplete-light-3.9.6rc1/src/dal/static/autocomplete_light/i18n/bn.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1019 2023-05-12 15:55:57.000000 django-autocomplete-light-3.9.6rc1/src/dal/static/autocomplete_light/i18n/bs.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)      968 2023-05-12 15:55:57.000000 django-autocomplete-light-3.9.6rc1/src/dal/static/autocomplete_light/i18n/ca.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1364 2023-05-12 15:55:57.000000 django-autocomplete-light-3.9.6rc1/src/dal/static/autocomplete_light/i18n/cs.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)      912 2023-05-12 15:55:57.000000 django-autocomplete-light-3.9.6rc1/src/dal/static/autocomplete_light/i18n/da.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)      949 2023-05-12 15:55:57.000000 django-autocomplete-light-3.9.6rc1/src/dal/static/autocomplete_light/i18n/de.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1093 2023-05-12 15:55:57.000000 django-autocomplete-light-3.9.6rc1/src/dal/static/autocomplete_light/i18n/dsb.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1266 2023-05-12 15:55:57.000000 django-autocomplete-light-3.9.6rc1/src/dal/static/autocomplete_light/i18n/el.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1005 2023-05-12 15:55:57.000000 django-autocomplete-light-3.9.6rc1/src/dal/static/autocomplete_light/i18n/en.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)      943 2023-05-12 15:55:57.000000 django-autocomplete-light-3.9.6rc1/src/dal/static/autocomplete_light/i18n/eo.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)      990 2023-05-12 15:55:57.000000 django-autocomplete-light-3.9.6rc1/src/dal/static/autocomplete_light/i18n/es.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)      882 2023-05-12 15:55:57.000000 django-autocomplete-light-3.9.6rc1/src/dal/static/autocomplete_light/i18n/et.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)      948 2023-05-12 15:55:57.000000 django-autocomplete-light-3.9.6rc1/src/dal/static/autocomplete_light/i18n/eu.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1107 2023-05-12 15:55:57.000000 django-autocomplete-light-3.9.6rc1/src/dal/static/autocomplete_light/i18n/fa.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)      887 2023-05-12 15:55:57.000000 django-autocomplete-light-3.9.6rc1/src/dal/static/autocomplete_light/i18n/fi.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1053 2023-05-12 15:55:57.000000 django-autocomplete-light-3.9.6rc1/src/dal/static/autocomplete_light/i18n/fr.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)      998 2023-05-12 15:55:57.000000 django-autocomplete-light-3.9.6rc1/src/dal/static/autocomplete_light/i18n/gl.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1056 2023-05-12 15:55:57.000000 django-autocomplete-light-3.9.6rc1/src/dal/static/autocomplete_light/i18n/he.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1246 2023-05-12 15:55:57.000000 django-autocomplete-light-3.9.6rc1/src/dal/static/autocomplete_light/i18n/hi.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)      936 2023-05-12 15:55:57.000000 django-autocomplete-light-3.9.6rc1/src/dal/static/autocomplete_light/i18n/hr.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1094 2023-05-12 15:55:57.000000 django-autocomplete-light-3.9.6rc1/src/dal/static/autocomplete_light/i18n/hsb.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1003 2023-05-12 15:55:57.000000 django-autocomplete-light-3.9.6rc1/src/dal/static/autocomplete_light/i18n/hu.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1112 2023-05-12 15:55:57.000000 django-autocomplete-light-3.9.6rc1/src/dal/static/autocomplete_light/i18n/hy.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)      852 2023-05-12 15:55:57.000000 django-autocomplete-light-3.9.6rc1/src/dal/static/autocomplete_light/i18n/id.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)      890 2023-05-12 15:55:57.000000 django-autocomplete-light-3.9.6rc1/src/dal/static/autocomplete_light/i18n/is.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)      972 2023-05-12 15:55:57.000000 django-autocomplete-light-3.9.6rc1/src/dal/static/autocomplete_light/i18n/it.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)      946 2023-05-12 15:55:57.000000 django-autocomplete-light-3.9.6rc1/src/dal/static/autocomplete_light/i18n/ja.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1279 2023-05-12 15:55:57.000000 django-autocomplete-light-3.9.6rc1/src/dal/static/autocomplete_light/i18n/ka.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1172 2023-05-12 15:55:57.000000 django-autocomplete-light-3.9.6rc1/src/dal/static/autocomplete_light/i18n/km.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)      939 2023-05-12 15:55:57.000000 django-autocomplete-light-3.9.6rc1/src/dal/static/autocomplete_light/i18n/ko.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)      998 2023-05-12 15:55:57.000000 django-autocomplete-light-3.9.6rc1/src/dal/static/autocomplete_light/i18n/lt.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)      959 2023-05-12 15:55:57.000000 django-autocomplete-light-3.9.6rc1/src/dal/static/autocomplete_light/i18n/lv.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1122 2023-05-12 15:55:57.000000 django-autocomplete-light-3.9.6rc1/src/dal/static/autocomplete_light/i18n/mk.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)      895 2023-05-12 15:55:57.000000 django-autocomplete-light-3.9.6rc1/src/dal/static/autocomplete_light/i18n/ms.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)      862 2023-05-12 15:55:57.000000 django-autocomplete-light-3.9.6rc1/src/dal/static/autocomplete_light/i18n/nb.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1438 2023-05-12 15:55:57.000000 django-autocomplete-light-3.9.6rc1/src/dal/static/autocomplete_light/i18n/ne.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)      985 2023-05-12 15:55:57.000000 django-autocomplete-light-3.9.6rc1/src/dal/static/autocomplete_light/i18n/nl.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1450 2023-05-12 15:55:57.000000 django-autocomplete-light-3.9.6rc1/src/dal/static/autocomplete_light/i18n/pa.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1022 2023-05-12 15:55:57.000000 django-autocomplete-light-3.9.6rc1/src/dal/static/autocomplete_light/i18n/pl.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1127 2023-05-12 15:55:57.000000 django-autocomplete-light-3.9.6rc1/src/dal/static/autocomplete_light/i18n/ps.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)      963 2023-05-12 15:55:57.000000 django-autocomplete-light-3.9.6rc1/src/dal/static/autocomplete_light/i18n/pt-BR.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)      946 2023-05-12 15:55:57.000000 django-autocomplete-light-3.9.6rc1/src/dal/static/autocomplete_light/i18n/pt.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1021 2023-05-12 15:55:57.000000 django-autocomplete-light-3.9.6rc1/src/dal/static/autocomplete_light/i18n/ro.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1233 2023-05-12 15:55:57.000000 django-autocomplete-light-3.9.6rc1/src/dal/static/autocomplete_light/i18n/ru.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1382 2023-05-12 15:55:57.000000 django-autocomplete-light-3.9.6rc1/src/dal/static/autocomplete_light/i18n/sk.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1009 2023-05-12 15:55:57.000000 django-autocomplete-light-3.9.6rc1/src/dal/static/autocomplete_light/i18n/sl.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)      987 2023-05-12 15:55:57.000000 django-autocomplete-light-3.9.6rc1/src/dal/static/autocomplete_light/i18n/sq.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1168 2023-05-12 15:55:57.000000 django-autocomplete-light-3.9.6rc1/src/dal/static/autocomplete_light/i18n/sr-Cyrl.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1034 2023-05-12 15:55:57.000000 django-autocomplete-light-3.9.6rc1/src/dal/static/autocomplete_light/i18n/sr.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)      870 2023-05-12 15:55:57.000000 django-autocomplete-light-3.9.6rc1/src/dal/static/autocomplete_light/i18n/sv.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1433 2023-05-12 15:55:57.000000 django-autocomplete-light-3.9.6rc1/src/dal/static/autocomplete_light/i18n/te.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1158 2023-05-12 15:55:57.000000 django-autocomplete-light-3.9.6rc1/src/dal/static/autocomplete_light/i18n/th.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)      855 2023-05-12 15:55:57.000000 django-autocomplete-light-3.9.6rc1/src/dal/static/autocomplete_light/i18n/tk.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)      859 2023-05-12 15:55:57.000000 django-autocomplete-light-3.9.6rc1/src/dal/static/autocomplete_light/i18n/tr.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1240 2023-05-12 15:55:57.000000 django-autocomplete-light-3.9.6rc1/src/dal/static/autocomplete_light/i18n/uk.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)      880 2023-05-12 15:55:57.000000 django-autocomplete-light-3.9.6rc1/src/dal/static/autocomplete_light/i18n/vi.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)      855 2023-05-12 15:55:57.000000 django-autocomplete-light-3.9.6rc1/src/dal/static/autocomplete_light/i18n/zh-CN.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)      794 2023-05-12 15:55:57.000000 django-autocomplete-light-3.9.6rc1/src/dal/static/autocomplete_light/i18n/zh-TW.js
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-05-12 15:55:59.107857 django-autocomplete-light-3.9.6rc1/src/dal/test/
--rw-r--r--   0 jpic      (1000) jpic      (1000)       36 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.6rc1/src/dal/test/__init__.py
--rw-r--r--   0 jpic      (1000) jpic      (1000)     3375 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.6rc1/src/dal/test/case.py
--rw-r--r--   0 jpic      (1000) jpic      (1000)    13961 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.6rc1/src/dal/test/stories.py
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1926 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.6rc1/src/dal/test/utils.py
--rw-r--r--   0 jpic      (1000) jpic      (1000)     7695 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.6rc1/src/dal/views.py
--rw-r--r--   0 jpic      (1000) jpic      (1000)     6595 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.6rc1/src/dal/widgets.py
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-05-12 15:55:59.107857 django-autocomplete-light-3.9.6rc1/src/dal_contenttypes/
--rw-r--r--   0 jpic      (1000) jpic      (1000)       53 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.6rc1/src/dal_contenttypes/__init__.py
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1962 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.6rc1/src/dal_contenttypes/fields.py
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-05-12 15:55:59.107857 django-autocomplete-light-3.9.6rc1/src/dal_genericm2m/
--rw-r--r--   0 jpic      (1000) jpic      (1000)       42 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.6rc1/src/dal_genericm2m/__init__.py
--rw-r--r--   0 jpic      (1000) jpic      (1000)      708 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.6rc1/src/dal_genericm2m/fields.py
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-05-12 15:55:59.107857 django-autocomplete-light-3.9.6rc1/src/dal_genericm2m_queryset_sequence/
--rw-r--r--   0 jpic      (1000) jpic      (1000)       65 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.6rc1/src/dal_genericm2m_queryset_sequence/__init__.py
--rw-r--r--   0 jpic      (1000) jpic      (1000)      424 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.6rc1/src/dal_genericm2m_queryset_sequence/fields.py
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-05-12 15:55:59.107857 django-autocomplete-light-3.9.6rc1/src/dal_gm2m/
--rw-r--r--   0 jpic      (1000) jpic      (1000)       35 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.6rc1/src/dal_gm2m/__init__.py
--rw-r--r--   0 jpic      (1000) jpic      (1000)      534 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.6rc1/src/dal_gm2m/fields.py
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-05-12 15:55:59.107857 django-autocomplete-light-3.9.6rc1/src/dal_gm2m_queryset_sequence/
--rw-r--r--   0 jpic      (1000) jpic      (1000)       70 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.6rc1/src/dal_gm2m_queryset_sequence/__init__.py
--rw-r--r--   0 jpic      (1000) jpic      (1000)      377 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.6rc1/src/dal_gm2m_queryset_sequence/fields.py
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-05-12 15:55:59.107857 django-autocomplete-light-3.9.6rc1/src/dal_legacy_static/
--rw-r--r--   0 jpic      (1000) jpic      (1000)       37 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.6rc1/src/dal_legacy_static/__init__.py
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-05-12 15:55:59.101191 django-autocomplete-light-3.9.6rc1/src/dal_legacy_static/static/
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-05-12 15:55:59.101191 django-autocomplete-light-3.9.6rc1/src/dal_legacy_static/static/admin/
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-05-12 15:55:59.107857 django-autocomplete-light-3.9.6rc1/src/dal_legacy_static/static/admin/css/
--rw-r--r--   0 jpic      (1000) jpic      (1000)     8440 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.6rc1/src/dal_legacy_static/static/admin/css/autocomplete.css
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-05-12 15:55:59.101191 django-autocomplete-light-3.9.6rc1/src/dal_legacy_static/static/admin/css/vendor/
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-05-12 15:55:59.107857 django-autocomplete-light-3.9.6rc1/src/dal_legacy_static/static/admin/css/vendor/select2/
--rwxr-xr-x   0 jpic      (1000) jpic      (1000)    17636 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.6rc1/src/dal_legacy_static/static/admin/css/vendor/select2/select2.css
--rwxr-xr-x   0 jpic      (1000) jpic      (1000)    15196 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.6rc1/src/dal_legacy_static/static/admin/css/vendor/select2/select2.min.css
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-05-12 15:55:59.107857 django-autocomplete-light-3.9.6rc1/src/dal_legacy_static/static/admin/js/
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1124 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.6rc1/src/dal_legacy_static/static/admin/js/autocomplete.js
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-05-12 15:55:59.101191 django-autocomplete-light-3.9.6rc1/src/dal_legacy_static/static/admin/js/vendor/
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-05-12 15:55:59.107857 django-autocomplete-light-3.9.6rc1/src/dal_legacy_static/static/admin/js/vendor/select2/
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-05-12 15:55:59.111191 django-autocomplete-light-3.9.6rc1/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/
--rwxr-xr-x   0 jpic      (1000) jpic      (1000)      887 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.6rc1/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/ar.js
--rwxr-xr-x   0 jpic      (1000) jpic      (1000)      701 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.6rc1/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/az.js
--rwxr-xr-x   0 jpic      (1000) jpic      (1000)      906 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.6rc1/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/bg.js
--rwxr-xr-x   0 jpic      (1000) jpic      (1000)      876 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.6rc1/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/ca.js
--rwxr-xr-x   0 jpic      (1000) jpic      (1000)     1236 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.6rc1/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/cs.js
--rwxr-xr-x   0 jpic      (1000) jpic      (1000)      818 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.6rc1/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/da.js
--rwxr-xr-x   0 jpic      (1000) jpic      (1000)      775 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.6rc1/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/de.js
--rwxr-xr-x   0 jpic      (1000) jpic      (1000)     1132 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.6rc1/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/el.js
--rwxr-xr-x   0 jpic      (1000) jpic      (1000)      827 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.6rc1/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/en.js
--rwxr-xr-x   0 jpic      (1000) jpic      (1000)      871 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.6rc1/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/es.js
--rwxr-xr-x   0 jpic      (1000) jpic      (1000)      775 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.6rc1/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/et.js
--rwxr-xr-x   0 jpic      (1000) jpic      (1000)      844 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.6rc1/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/eu.js
--rwxr-xr-x   0 jpic      (1000) jpic      (1000)     1004 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.6rc1/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/fa.js
--rwxr-xr-x   0 jpic      (1000) jpic      (1000)      703 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.6rc1/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/fi.js
--rwxr-xr-x   0 jpic      (1000) jpic      (1000)      902 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.6rc1/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/fr.js
--rwxr-xr-x   0 jpic      (1000) jpic      (1000)      800 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.6rc1/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/gl.js
--rwxr-xr-x   0 jpic      (1000) jpic      (1000)      951 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.6rc1/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/he.js
--rwxr-xr-x   0 jpic      (1000) jpic      (1000)     1125 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.6rc1/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/hi.js
--rwxr-xr-x   0 jpic      (1000) jpic      (1000)      839 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.6rc1/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/hr.js
--rwxr-xr-x   0 jpic      (1000) jpic      (1000)      727 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.6rc1/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/hu.js
--rwxr-xr-x   0 jpic      (1000) jpic      (1000)      752 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.6rc1/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/id.js
--rwxr-xr-x   0 jpic      (1000) jpic      (1000)      773 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.6rc1/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/is.js
--rwxr-xr-x   0 jpic      (1000) jpic      (1000)      876 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.6rc1/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/it.js
--rwxr-xr-x   0 jpic      (1000) jpic      (1000)      848 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.6rc1/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/ja.js
--rwxr-xr-x   0 jpic      (1000) jpic      (1000)     1065 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.6rc1/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/km.js
--rwxr-xr-x   0 jpic      (1000) jpic      (1000)      854 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.6rc1/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/ko.js
--rwxr-xr-x   0 jpic      (1000) jpic      (1000)      913 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.6rc1/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/lt.js
--rwxr-xr-x   0 jpic      (1000) jpic      (1000)      872 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.6rc1/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/lv.js
--rwxr-xr-x   0 jpic      (1000) jpic      (1000)      979 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.6rc1/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/mk.js
--rwxr-xr-x   0 jpic      (1000) jpic      (1000)      791 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.6rc1/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/ms.js
--rwxr-xr-x   0 jpic      (1000) jpic      (1000)      785 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.6rc1/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/nb.js
--rwxr-xr-x   0 jpic      (1000) jpic      (1000)      896 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.6rc1/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/nl.js
--rwxr-xr-x   0 jpic      (1000) jpic      (1000)      925 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.6rc1/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/pl.js
--rwxr-xr-x   0 jpic      (1000) jpic      (1000)      853 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.6rc1/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/pt-BR.js
--rwxr-xr-x   0 jpic      (1000) jpic      (1000)      859 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.6rc1/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/pt.js
--rwxr-xr-x   0 jpic      (1000) jpic      (1000)      909 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.6rc1/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/ro.js
--rwxr-xr-x   0 jpic      (1000) jpic      (1000)     1127 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.6rc1/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/ru.js
--rwxr-xr-x   0 jpic      (1000) jpic      (1000)     1184 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.6rc1/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/sk.js
--rwxr-xr-x   0 jpic      (1000) jpic      (1000)     1067 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.6rc1/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/sr-Cyrl.js
--rwxr-xr-x   0 jpic      (1000) jpic      (1000)      938 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.6rc1/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/sr.js
--rwxr-xr-x   0 jpic      (1000) jpic      (1000)      786 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.6rc1/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/sv.js
--rwxr-xr-x   0 jpic      (1000) jpic      (1000)      951 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.6rc1/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/th.js
--rwxr-xr-x   0 jpic      (1000) jpic      (1000)      720 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.6rc1/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/tr.js
--rwxr-xr-x   0 jpic      (1000) jpic      (1000)     1117 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.6rc1/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/uk.js
--rwxr-xr-x   0 jpic      (1000) jpic      (1000)      801 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.6rc1/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/vi.js
--rwxr-xr-x   0 jpic      (1000) jpic      (1000)      769 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.6rc1/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/zh-CN.js
--rwxr-xr-x   0 jpic      (1000) jpic      (1000)      708 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.6rc1/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/zh-TW.js
--rwxr-xr-x   0 jpic      (1000) jpic      (1000)   161832 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.6rc1/src/dal_legacy_static/static/admin/js/vendor/select2/select2.full.js
--rwxr-xr-x   0 jpic      (1000) jpic      (1000)    75005 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.6rc1/src/dal_legacy_static/static/admin/js/vendor/select2/select2.full.min.js
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-05-12 15:55:59.111191 django-autocomplete-light-3.9.6rc1/src/dal_queryset_sequence/
--rw-r--r--   0 jpic      (1000) jpic      (1000)       40 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.6rc1/src/dal_queryset_sequence/__init__.py
--rw-r--r--   0 jpic      (1000) jpic      (1000)     6355 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.6rc1/src/dal_queryset_sequence/fields.py
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-05-12 15:55:59.111191 django-autocomplete-light-3.9.6rc1/src/dal_queryset_sequence/tests/
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1545 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.6rc1/src/dal_queryset_sequence/tests/test_views.py
--rw-r--r--   0 jpic      (1000) jpic      (1000)     2298 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.6rc1/src/dal_queryset_sequence/views.py
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1703 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.6rc1/src/dal_queryset_sequence/widgets.py
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-05-12 15:55:59.111191 django-autocomplete-light-3.9.6rc1/src/dal_select2/
--rw-r--r--   0 jpic      (1000) jpic      (1000)      149 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.6rc1/src/dal_select2/__init__.py
--rw-r--r--   0 jpic      (1000) jpic      (1000)      274 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.6rc1/src/dal_select2/apps.py
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1795 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.6rc1/src/dal_select2/fields.py
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-05-12 15:55:59.104524 django-autocomplete-light-3.9.6rc1/src/dal_select2/locale/
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-05-12 15:55:59.101191 django-autocomplete-light-3.9.6rc1/src/dal_select2/locale/bg/
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-05-12 15:55:59.111191 django-autocomplete-light-3.9.6rc1/src/dal_select2/locale/bg/LC_MESSAGES/
--rw-r--r--   0 jpic      (1000) jpic      (1000)      508 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.6rc1/src/dal_select2/locale/bg/LC_MESSAGES/django.mo
--rw-r--r--   0 jpic      (1000) jpic      (1000)      671 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.6rc1/src/dal_select2/locale/bg/LC_MESSAGES/django.po
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-05-12 15:55:59.101191 django-autocomplete-light-3.9.6rc1/src/dal_select2/locale/cs/
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-05-12 15:55:59.114524 django-autocomplete-light-3.9.6rc1/src/dal_select2/locale/cs/LC_MESSAGES/
--rw-r--r--   0 jpic      (1000) jpic      (1000)      528 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.6rc1/src/dal_select2/locale/cs/LC_MESSAGES/django.mo
--rw-r--r--   0 jpic      (1000) jpic      (1000)      691 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.6rc1/src/dal_select2/locale/cs/LC_MESSAGES/django.po
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-05-12 15:55:59.101191 django-autocomplete-light-3.9.6rc1/src/dal_select2/locale/de/
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-05-12 15:55:59.114524 django-autocomplete-light-3.9.6rc1/src/dal_select2/locale/de/LC_MESSAGES/
--rw-r--r--   0 jpic      (1000) jpic      (1000)      501 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.6rc1/src/dal_select2/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 jpic      (1000) jpic      (1000)      664 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.6rc1/src/dal_select2/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-05-12 15:55:59.101191 django-autocomplete-light-3.9.6rc1/src/dal_select2/locale/es/
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-05-12 15:55:59.114524 django-autocomplete-light-3.9.6rc1/src/dal_select2/locale/es/LC_MESSAGES/
--rw-r--r--   0 jpic      (1000) jpic      (1000)      497 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.6rc1/src/dal_select2/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0 jpic      (1000) jpic      (1000)      660 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.6rc1/src/dal_select2/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-05-12 15:55:59.101191 django-autocomplete-light-3.9.6rc1/src/dal_select2/locale/fi/
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-05-12 15:55:59.114524 django-autocomplete-light-3.9.6rc1/src/dal_select2/locale/fi/LC_MESSAGES/
--rw-r--r--   0 jpic      (1000) jpic      (1000)      488 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.6rc1/src/dal_select2/locale/fi/LC_MESSAGES/django.mo
--rw-r--r--   0 jpic      (1000) jpic      (1000)      684 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.6rc1/src/dal_select2/locale/fi/LC_MESSAGES/django.po
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-05-12 15:55:59.101191 django-autocomplete-light-3.9.6rc1/src/dal_select2/locale/fr/
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-05-12 15:55:59.114524 django-autocomplete-light-3.9.6rc1/src/dal_select2/locale/fr/LC_MESSAGES/
--rw-r--r--   0 jpic      (1000) jpic      (1000)      497 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.6rc1/src/dal_select2/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0 jpic      (1000) jpic      (1000)      660 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.6rc1/src/dal_select2/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-05-12 15:55:59.101191 django-autocomplete-light-3.9.6rc1/src/dal_select2/locale/it/
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-05-12 15:55:59.114524 django-autocomplete-light-3.9.6rc1/src/dal_select2/locale/it/LC_MESSAGES/
--rw-r--r--   0 jpic      (1000) jpic      (1000)      498 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.6rc1/src/dal_select2/locale/it/LC_MESSAGES/django.mo
--rw-r--r--   0 jpic      (1000) jpic      (1000)      661 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.6rc1/src/dal_select2/locale/it/LC_MESSAGES/django.po
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-05-12 15:55:59.104524 django-autocomplete-light-3.9.6rc1/src/dal_select2/locale/ja/
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-05-12 15:55:59.114524 django-autocomplete-light-3.9.6rc1/src/dal_select2/locale/ja/LC_MESSAGES/
--rw-r--r--   0 jpic      (1000) jpic      (1000)      497 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.6rc1/src/dal_select2/locale/ja/LC_MESSAGES/django.mo
--rw-r--r--   0 jpic      (1000) jpic      (1000)      660 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.6rc1/src/dal_select2/locale/ja/LC_MESSAGES/django.po
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-05-12 15:55:59.104524 django-autocomplete-light-3.9.6rc1/src/dal_select2/locale/nl/
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-05-12 15:55:59.114524 django-autocomplete-light-3.9.6rc1/src/dal_select2/locale/nl/LC_MESSAGES/
--rw-r--r--   0 jpic      (1000) jpic      (1000)      500 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.6rc1/src/dal_select2/locale/nl/LC_MESSAGES/django.mo
--rw-r--r--   0 jpic      (1000) jpic      (1000)      663 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.6rc1/src/dal_select2/locale/nl/LC_MESSAGES/django.po
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-05-12 15:55:59.104524 django-autocomplete-light-3.9.6rc1/src/dal_select2/locale/pl/
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-05-12 15:55:59.114524 django-autocomplete-light-3.9.6rc1/src/dal_select2/locale/pl/LC_MESSAGES/
--rw-r--r--   0 jpic      (1000) jpic      (1000)      557 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.6rc1/src/dal_select2/locale/pl/LC_MESSAGES/django.mo
--rw-r--r--   0 jpic      (1000) jpic      (1000)      723 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.6rc1/src/dal_select2/locale/pl/LC_MESSAGES/django.po
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-05-12 15:55:59.104524 django-autocomplete-light-3.9.6rc1/src/dal_select2/locale/pt-br/
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-05-12 15:55:59.114524 django-autocomplete-light-3.9.6rc1/src/dal_select2/locale/pt-br/LC_MESSAGES/
--rw-r--r--   0 jpic      (1000) jpic      (1000)      503 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.6rc1/src/dal_select2/locale/pt-br/LC_MESSAGES/django.mo
--rw-r--r--   0 jpic      (1000) jpic      (1000)      670 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.6rc1/src/dal_select2/locale/pt-br/LC_MESSAGES/django.po
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-05-12 15:55:59.104524 django-autocomplete-light-3.9.6rc1/src/dal_select2/locale/ru/
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-05-12 15:55:59.114524 django-autocomplete-light-3.9.6rc1/src/dal_select2/locale/ru/LC_MESSAGES/
--rw-r--r--   0 jpic      (1000) jpic      (1000)      644 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.6rc1/src/dal_select2/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0 jpic      (1000) jpic      (1000)      813 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.6rc1/src/dal_select2/locale/ru/LC_MESSAGES/django.po
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-05-12 15:55:59.104524 django-autocomplete-light-3.9.6rc1/src/dal_select2/locale/tr/
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-05-12 15:55:59.114524 django-autocomplete-light-3.9.6rc1/src/dal_select2/locale/tr/LC_MESSAGES/
--rw-r--r--   0 jpic      (1000) jpic      (1000)      492 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.6rc1/src/dal_select2/locale/tr/LC_MESSAGES/django.mo
--rw-r--r--   0 jpic      (1000) jpic      (1000)      741 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.6rc1/src/dal_select2/locale/tr/LC_MESSAGES/django.po
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-05-12 15:55:59.104524 django-autocomplete-light-3.9.6rc1/src/dal_select2/locale/uk/
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-05-12 15:55:59.114524 django-autocomplete-light-3.9.6rc1/src/dal_select2/locale/uk/LC_MESSAGES/
--rw-r--r--   0 jpic      (1000) jpic      (1000)      582 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.6rc1/src/dal_select2/locale/uk/LC_MESSAGES/django.mo
--rw-r--r--   0 jpic      (1000) jpic      (1000)      748 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.6rc1/src/dal_select2/locale/uk/LC_MESSAGES/django.po
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-05-12 15:55:59.104524 django-autocomplete-light-3.9.6rc1/src/dal_select2/locale/zh-cn/
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-05-12 15:55:59.114524 django-autocomplete-light-3.9.6rc1/src/dal_select2/locale/zh-cn/LC_MESSAGES/
--rw-r--r--   0 jpic      (1000) jpic      (1000)      458 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.6rc1/src/dal_select2/locale/zh-cn/LC_MESSAGES/django.mo
--rw-r--r--   0 jpic      (1000) jpic      (1000)      617 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.6rc1/src/dal_select2/locale/zh-cn/LC_MESSAGES/django.po
--rw-r--r--   0 jpic      (1000) jpic      (1000)       46 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.6rc1/src/dal_select2/models.py
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-05-12 15:55:59.104524 django-autocomplete-light-3.9.6rc1/src/dal_select2/static/
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-05-12 15:55:59.114524 django-autocomplete-light-3.9.6rc1/src/dal_select2/static/autocomplete_light/
--rw-r--r--   0 jpic      (1000) jpic      (1000)     2765 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.6rc1/src/dal_select2/static/autocomplete_light/select2.css
--rw-r--r--   0 jpic      (1000) jpic      (1000)     4937 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.6rc1/src/dal_select2/static/autocomplete_light/select2.js
--rw-r--r--   0 jpic      (1000) jpic      (1000)     2014 2023-05-12 15:55:58.000000 django-autocomplete-light-3.9.6rc1/src/dal_select2/static/autocomplete_light/select2.min.js
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-05-12 15:55:59.104524 django-autocomplete-light-3.9.6rc1/src/dal_select2/static/vendor/
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-05-12 15:55:59.104524 django-autocomplete-light-3.9.6rc1/src/dal_select2/static/vendor/select2/
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-05-12 15:55:59.104524 django-autocomplete-light-3.9.6rc1/src/dal_select2/static/vendor/select2/dist/
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-05-12 15:55:59.114524 django-autocomplete-light-3.9.6rc1/src/dal_select2/static/vendor/select2/dist/css/
--rw-r--r--   0 jpic      (1000) jpic      (1000)    18931 2023-05-12 15:55:57.000000 django-autocomplete-light-3.9.6rc1/src/dal_select2/static/vendor/select2/dist/css/select2.css
--rw-r--r--   0 jpic      (1000) jpic      (1000)    16264 2023-05-12 15:55:57.000000 django-autocomplete-light-3.9.6rc1/src/dal_select2/static/vendor/select2/dist/css/select2.min.css
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1071 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.6rc1/src/dal_select2/test.py
--rw-r--r--   0 jpic      (1000) jpic      (1000)    10574 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.6rc1/src/dal_select2/views.py
--rw-r--r--   0 jpic      (1000) jpic      (1000)     6206 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.6rc1/src/dal_select2/widgets.py
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-05-12 15:55:59.114524 django-autocomplete-light-3.9.6rc1/src/dal_select2_queryset_sequence/
--rw-r--r--   0 jpic      (1000) jpic      (1000)      580 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.6rc1/src/dal_select2_queryset_sequence/__init__.py
--rw-r--r--   0 jpic      (1000) jpic      (1000)     2704 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.6rc1/src/dal_select2_queryset_sequence/fields.py
--rw-r--r--   0 jpic      (1000) jpic      (1000)     3501 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.6rc1/src/dal_select2_queryset_sequence/views.py
--rw-r--r--   0 jpic      (1000) jpic      (1000)      975 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.6rc1/src/dal_select2_queryset_sequence/widgets.py
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-05-12 15:55:59.114524 django-autocomplete-light-3.9.6rc1/src/dal_select2_tagging/
--rw-r--r--   0 jpic      (1000) jpic      (1000)       50 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.6rc1/src/dal_select2_tagging/__init__.py
--rw-r--r--   0 jpic      (1000) jpic      (1000)      895 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.6rc1/src/dal_select2_tagging/widgets.py
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-05-12 15:55:59.114524 django-autocomplete-light-3.9.6rc1/src/dal_select2_taggit/
--rw-r--r--   0 jpic      (1000) jpic      (1000)       42 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.6rc1/src/dal_select2_taggit/__init__.py
--rw-r--r--   0 jpic      (1000) jpic      (1000)     1834 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.6rc1/src/dal_select2_taggit/widgets.py
-drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-05-12 15:55:59.114524 django-autocomplete-light-3.9.6rc1/src/django_autocomplete_light.egg-info/
--rw-r--r--   0 jpic      (1000) jpic      (1000)     3326 2023-05-12 15:55:58.000000 django-autocomplete-light-3.9.6rc1/src/django_autocomplete_light.egg-info/PKG-INFO
--rw-r--r--   0 jpic      (1000) jpic      (1000)     9762 2023-05-12 15:55:59.000000 django-autocomplete-light-3.9.6rc1/src/django_autocomplete_light.egg-info/SOURCES.txt
--rw-r--r--   0 jpic      (1000) jpic      (1000)        1 2023-05-12 15:55:58.000000 django-autocomplete-light-3.9.6rc1/src/django_autocomplete_light.egg-info/dependency_links.txt
--rw-r--r--   0 jpic      (1000) jpic      (1000)        1 2023-05-12 15:43:49.000000 django-autocomplete-light-3.9.6rc1/src/django_autocomplete_light.egg-info/not-zip-safe
--rw-r--r--   0 jpic      (1000) jpic      (1000)      146 2023-05-12 15:55:58.000000 django-autocomplete-light-3.9.6rc1/src/django_autocomplete_light.egg-info/requires.txt
--rw-r--r--   0 jpic      (1000) jpic      (1000)      226 2023-05-12 15:55:58.000000 django-autocomplete-light-3.9.6rc1/src/django_autocomplete_light.egg-info/top_level.txt
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-05-12 16:01:04.207870 django-autocomplete-light-3.9.7/
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1625 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.7/AUTHORS
+-rw-r--r--   0 jpic      (1000) jpic      (1000)    47190 2023-05-12 16:01:03.000000 django-autocomplete-light-3.9.7/CHANGELOG
+-rw-r--r--   0 jpic      (1000) jpic      (1000)    47190 2023-05-12 16:01:03.000000 django-autocomplete-light-3.9.7/CHANGES.txt
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1076 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.7/LICENSE
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      302 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.7/MANIFEST.in
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     3323 2023-05-12 16:01:04.207870 django-autocomplete-light-3.9.7/PKG-INFO
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     2221 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.7/README
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     2221 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.7/README.rst
+-rw-r--r--   0 jpic      (1000) jpic      (1000)       38 2023-05-12 16:01:04.207870 django-autocomplete-light-3.9.7/setup.cfg
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1833 2023-05-12 16:01:03.000000 django-autocomplete-light-3.9.7/setup.py
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-05-12 16:01:04.194537 django-autocomplete-light-3.9.7/src/
+-rw-r--r--   0 jpic      (1000) jpic      (1000)       37 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.7/src/__init__.py
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-05-12 16:01:04.194537 django-autocomplete-light-3.9.7/src/dal/
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      112 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.7/src/dal/__init__.py
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     2751 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.7/src/dal/autocomplete.py
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     6762 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.7/src/dal/forms.py
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     4633 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.7/src/dal/forward.py
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-05-12 16:01:04.194537 django-autocomplete-light-3.9.7/src/dal/static/
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-05-12 16:01:04.194537 django-autocomplete-light-3.9.7/src/dal/static/autocomplete_light/
+-rw-r--r--   0 jpic      (1000) jpic      (1000)    18327 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.7/src/dal/static/autocomplete_light/autocomplete_light.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     5423 2023-05-12 16:01:03.000000 django-autocomplete-light-3.9.7/src/dal/static/autocomplete_light/autocomplete_light.min.js
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-05-12 16:01:04.201203 django-autocomplete-light-3.9.7/src/dal/static/autocomplete_light/i18n/
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      950 2023-05-12 16:01:02.000000 django-autocomplete-light-3.9.7/src/dal/static/autocomplete_light/i18n/af.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      989 2023-05-12 16:01:02.000000 django-autocomplete-light-3.9.7/src/dal/static/autocomplete_light/i18n/ar.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      805 2023-05-12 16:01:02.000000 django-autocomplete-light-3.9.7/src/dal/static/autocomplete_light/i18n/az.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1052 2023-05-12 16:01:02.000000 django-autocomplete-light-3.9.7/src/dal/static/autocomplete_light/i18n/bg.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1359 2023-05-12 16:01:02.000000 django-autocomplete-light-3.9.7/src/dal/static/autocomplete_light/i18n/bn.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1019 2023-05-12 16:01:02.000000 django-autocomplete-light-3.9.7/src/dal/static/autocomplete_light/i18n/bs.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      968 2023-05-12 16:01:02.000000 django-autocomplete-light-3.9.7/src/dal/static/autocomplete_light/i18n/ca.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1364 2023-05-12 16:01:02.000000 django-autocomplete-light-3.9.7/src/dal/static/autocomplete_light/i18n/cs.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      912 2023-05-12 16:01:02.000000 django-autocomplete-light-3.9.7/src/dal/static/autocomplete_light/i18n/da.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      949 2023-05-12 16:01:02.000000 django-autocomplete-light-3.9.7/src/dal/static/autocomplete_light/i18n/de.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1093 2023-05-12 16:01:02.000000 django-autocomplete-light-3.9.7/src/dal/static/autocomplete_light/i18n/dsb.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1266 2023-05-12 16:01:02.000000 django-autocomplete-light-3.9.7/src/dal/static/autocomplete_light/i18n/el.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1005 2023-05-12 16:01:02.000000 django-autocomplete-light-3.9.7/src/dal/static/autocomplete_light/i18n/en.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      943 2023-05-12 16:01:02.000000 django-autocomplete-light-3.9.7/src/dal/static/autocomplete_light/i18n/eo.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      990 2023-05-12 16:01:02.000000 django-autocomplete-light-3.9.7/src/dal/static/autocomplete_light/i18n/es.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      882 2023-05-12 16:01:02.000000 django-autocomplete-light-3.9.7/src/dal/static/autocomplete_light/i18n/et.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      948 2023-05-12 16:01:02.000000 django-autocomplete-light-3.9.7/src/dal/static/autocomplete_light/i18n/eu.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1107 2023-05-12 16:01:02.000000 django-autocomplete-light-3.9.7/src/dal/static/autocomplete_light/i18n/fa.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      887 2023-05-12 16:01:02.000000 django-autocomplete-light-3.9.7/src/dal/static/autocomplete_light/i18n/fi.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1053 2023-05-12 16:01:02.000000 django-autocomplete-light-3.9.7/src/dal/static/autocomplete_light/i18n/fr.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      998 2023-05-12 16:01:02.000000 django-autocomplete-light-3.9.7/src/dal/static/autocomplete_light/i18n/gl.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1056 2023-05-12 16:01:02.000000 django-autocomplete-light-3.9.7/src/dal/static/autocomplete_light/i18n/he.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1246 2023-05-12 16:01:02.000000 django-autocomplete-light-3.9.7/src/dal/static/autocomplete_light/i18n/hi.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      936 2023-05-12 16:01:02.000000 django-autocomplete-light-3.9.7/src/dal/static/autocomplete_light/i18n/hr.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1094 2023-05-12 16:01:02.000000 django-autocomplete-light-3.9.7/src/dal/static/autocomplete_light/i18n/hsb.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1003 2023-05-12 16:01:02.000000 django-autocomplete-light-3.9.7/src/dal/static/autocomplete_light/i18n/hu.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1112 2023-05-12 16:01:02.000000 django-autocomplete-light-3.9.7/src/dal/static/autocomplete_light/i18n/hy.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      852 2023-05-12 16:01:02.000000 django-autocomplete-light-3.9.7/src/dal/static/autocomplete_light/i18n/id.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      890 2023-05-12 16:01:02.000000 django-autocomplete-light-3.9.7/src/dal/static/autocomplete_light/i18n/is.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      972 2023-05-12 16:01:02.000000 django-autocomplete-light-3.9.7/src/dal/static/autocomplete_light/i18n/it.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      946 2023-05-12 16:01:02.000000 django-autocomplete-light-3.9.7/src/dal/static/autocomplete_light/i18n/ja.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1279 2023-05-12 16:01:02.000000 django-autocomplete-light-3.9.7/src/dal/static/autocomplete_light/i18n/ka.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1172 2023-05-12 16:01:02.000000 django-autocomplete-light-3.9.7/src/dal/static/autocomplete_light/i18n/km.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      939 2023-05-12 16:01:02.000000 django-autocomplete-light-3.9.7/src/dal/static/autocomplete_light/i18n/ko.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      998 2023-05-12 16:01:02.000000 django-autocomplete-light-3.9.7/src/dal/static/autocomplete_light/i18n/lt.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      959 2023-05-12 16:01:02.000000 django-autocomplete-light-3.9.7/src/dal/static/autocomplete_light/i18n/lv.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1122 2023-05-12 16:01:02.000000 django-autocomplete-light-3.9.7/src/dal/static/autocomplete_light/i18n/mk.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      895 2023-05-12 16:01:02.000000 django-autocomplete-light-3.9.7/src/dal/static/autocomplete_light/i18n/ms.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      862 2023-05-12 16:01:02.000000 django-autocomplete-light-3.9.7/src/dal/static/autocomplete_light/i18n/nb.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1438 2023-05-12 16:01:02.000000 django-autocomplete-light-3.9.7/src/dal/static/autocomplete_light/i18n/ne.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      985 2023-05-12 16:01:02.000000 django-autocomplete-light-3.9.7/src/dal/static/autocomplete_light/i18n/nl.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1450 2023-05-12 16:01:02.000000 django-autocomplete-light-3.9.7/src/dal/static/autocomplete_light/i18n/pa.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1022 2023-05-12 16:01:02.000000 django-autocomplete-light-3.9.7/src/dal/static/autocomplete_light/i18n/pl.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1127 2023-05-12 16:01:02.000000 django-autocomplete-light-3.9.7/src/dal/static/autocomplete_light/i18n/ps.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      963 2023-05-12 16:01:02.000000 django-autocomplete-light-3.9.7/src/dal/static/autocomplete_light/i18n/pt-BR.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      946 2023-05-12 16:01:02.000000 django-autocomplete-light-3.9.7/src/dal/static/autocomplete_light/i18n/pt.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1021 2023-05-12 16:01:02.000000 django-autocomplete-light-3.9.7/src/dal/static/autocomplete_light/i18n/ro.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1233 2023-05-12 16:01:02.000000 django-autocomplete-light-3.9.7/src/dal/static/autocomplete_light/i18n/ru.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1382 2023-05-12 16:01:02.000000 django-autocomplete-light-3.9.7/src/dal/static/autocomplete_light/i18n/sk.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1009 2023-05-12 16:01:02.000000 django-autocomplete-light-3.9.7/src/dal/static/autocomplete_light/i18n/sl.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      987 2023-05-12 16:01:02.000000 django-autocomplete-light-3.9.7/src/dal/static/autocomplete_light/i18n/sq.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1168 2023-05-12 16:01:02.000000 django-autocomplete-light-3.9.7/src/dal/static/autocomplete_light/i18n/sr-Cyrl.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1034 2023-05-12 16:01:02.000000 django-autocomplete-light-3.9.7/src/dal/static/autocomplete_light/i18n/sr.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      870 2023-05-12 16:01:02.000000 django-autocomplete-light-3.9.7/src/dal/static/autocomplete_light/i18n/sv.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1433 2023-05-12 16:01:02.000000 django-autocomplete-light-3.9.7/src/dal/static/autocomplete_light/i18n/te.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1158 2023-05-12 16:01:02.000000 django-autocomplete-light-3.9.7/src/dal/static/autocomplete_light/i18n/th.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      855 2023-05-12 16:01:02.000000 django-autocomplete-light-3.9.7/src/dal/static/autocomplete_light/i18n/tk.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      859 2023-05-12 16:01:02.000000 django-autocomplete-light-3.9.7/src/dal/static/autocomplete_light/i18n/tr.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1240 2023-05-12 16:01:02.000000 django-autocomplete-light-3.9.7/src/dal/static/autocomplete_light/i18n/uk.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      880 2023-05-12 16:01:02.000000 django-autocomplete-light-3.9.7/src/dal/static/autocomplete_light/i18n/vi.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      855 2023-05-12 16:01:02.000000 django-autocomplete-light-3.9.7/src/dal/static/autocomplete_light/i18n/zh-CN.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      794 2023-05-12 16:01:02.000000 django-autocomplete-light-3.9.7/src/dal/static/autocomplete_light/i18n/zh-TW.js
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-05-12 16:01:04.201203 django-autocomplete-light-3.9.7/src/dal/test/
+-rw-r--r--   0 jpic      (1000) jpic      (1000)       36 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.7/src/dal/test/__init__.py
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     3375 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.7/src/dal/test/case.py
+-rw-r--r--   0 jpic      (1000) jpic      (1000)    13961 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.7/src/dal/test/stories.py
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1926 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.7/src/dal/test/utils.py
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     7695 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.7/src/dal/views.py
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     6595 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.7/src/dal/widgets.py
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-05-12 16:01:04.201203 django-autocomplete-light-3.9.7/src/dal_contenttypes/
+-rw-r--r--   0 jpic      (1000) jpic      (1000)       53 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.7/src/dal_contenttypes/__init__.py
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1962 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.7/src/dal_contenttypes/fields.py
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-05-12 16:01:04.201203 django-autocomplete-light-3.9.7/src/dal_genericm2m/
+-rw-r--r--   0 jpic      (1000) jpic      (1000)       42 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.7/src/dal_genericm2m/__init__.py
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      708 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.7/src/dal_genericm2m/fields.py
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-05-12 16:01:04.201203 django-autocomplete-light-3.9.7/src/dal_genericm2m_queryset_sequence/
+-rw-r--r--   0 jpic      (1000) jpic      (1000)       65 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.7/src/dal_genericm2m_queryset_sequence/__init__.py
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      424 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.7/src/dal_genericm2m_queryset_sequence/fields.py
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-05-12 16:01:04.201203 django-autocomplete-light-3.9.7/src/dal_gm2m/
+-rw-r--r--   0 jpic      (1000) jpic      (1000)       35 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.7/src/dal_gm2m/__init__.py
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      534 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.7/src/dal_gm2m/fields.py
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-05-12 16:01:04.201203 django-autocomplete-light-3.9.7/src/dal_gm2m_queryset_sequence/
+-rw-r--r--   0 jpic      (1000) jpic      (1000)       70 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.7/src/dal_gm2m_queryset_sequence/__init__.py
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      377 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.7/src/dal_gm2m_queryset_sequence/fields.py
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-05-12 16:01:04.201203 django-autocomplete-light-3.9.7/src/dal_legacy_static/
+-rw-r--r--   0 jpic      (1000) jpic      (1000)       37 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.7/src/dal_legacy_static/__init__.py
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-05-12 16:01:04.194537 django-autocomplete-light-3.9.7/src/dal_legacy_static/static/
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-05-12 16:01:04.194537 django-autocomplete-light-3.9.7/src/dal_legacy_static/static/admin/
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-05-12 16:01:04.201203 django-autocomplete-light-3.9.7/src/dal_legacy_static/static/admin/css/
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     8440 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.7/src/dal_legacy_static/static/admin/css/autocomplete.css
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-05-12 16:01:04.194537 django-autocomplete-light-3.9.7/src/dal_legacy_static/static/admin/css/vendor/
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-05-12 16:01:04.201203 django-autocomplete-light-3.9.7/src/dal_legacy_static/static/admin/css/vendor/select2/
+-rwxr-xr-x   0 jpic      (1000) jpic      (1000)    17636 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.7/src/dal_legacy_static/static/admin/css/vendor/select2/select2.css
+-rwxr-xr-x   0 jpic      (1000) jpic      (1000)    15196 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.7/src/dal_legacy_static/static/admin/css/vendor/select2/select2.min.css
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-05-12 16:01:04.201203 django-autocomplete-light-3.9.7/src/dal_legacy_static/static/admin/js/
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1124 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.7/src/dal_legacy_static/static/admin/js/autocomplete.js
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-05-12 16:01:04.194537 django-autocomplete-light-3.9.7/src/dal_legacy_static/static/admin/js/vendor/
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-05-12 16:01:04.201203 django-autocomplete-light-3.9.7/src/dal_legacy_static/static/admin/js/vendor/select2/
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-05-12 16:01:04.204537 django-autocomplete-light-3.9.7/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/
+-rwxr-xr-x   0 jpic      (1000) jpic      (1000)      887 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.7/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/ar.js
+-rwxr-xr-x   0 jpic      (1000) jpic      (1000)      701 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.7/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/az.js
+-rwxr-xr-x   0 jpic      (1000) jpic      (1000)      906 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.7/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/bg.js
+-rwxr-xr-x   0 jpic      (1000) jpic      (1000)      876 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.7/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/ca.js
+-rwxr-xr-x   0 jpic      (1000) jpic      (1000)     1236 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.7/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/cs.js
+-rwxr-xr-x   0 jpic      (1000) jpic      (1000)      818 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.7/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/da.js
+-rwxr-xr-x   0 jpic      (1000) jpic      (1000)      775 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.7/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/de.js
+-rwxr-xr-x   0 jpic      (1000) jpic      (1000)     1132 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.7/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/el.js
+-rwxr-xr-x   0 jpic      (1000) jpic      (1000)      827 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.7/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/en.js
+-rwxr-xr-x   0 jpic      (1000) jpic      (1000)      871 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.7/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/es.js
+-rwxr-xr-x   0 jpic      (1000) jpic      (1000)      775 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.7/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/et.js
+-rwxr-xr-x   0 jpic      (1000) jpic      (1000)      844 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.7/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/eu.js
+-rwxr-xr-x   0 jpic      (1000) jpic      (1000)     1004 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.7/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/fa.js
+-rwxr-xr-x   0 jpic      (1000) jpic      (1000)      703 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.7/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/fi.js
+-rwxr-xr-x   0 jpic      (1000) jpic      (1000)      902 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.7/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/fr.js
+-rwxr-xr-x   0 jpic      (1000) jpic      (1000)      800 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.7/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/gl.js
+-rwxr-xr-x   0 jpic      (1000) jpic      (1000)      951 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.7/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/he.js
+-rwxr-xr-x   0 jpic      (1000) jpic      (1000)     1125 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.7/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/hi.js
+-rwxr-xr-x   0 jpic      (1000) jpic      (1000)      839 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.7/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/hr.js
+-rwxr-xr-x   0 jpic      (1000) jpic      (1000)      727 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.7/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/hu.js
+-rwxr-xr-x   0 jpic      (1000) jpic      (1000)      752 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.7/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/id.js
+-rwxr-xr-x   0 jpic      (1000) jpic      (1000)      773 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.7/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/is.js
+-rwxr-xr-x   0 jpic      (1000) jpic      (1000)      876 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.7/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/it.js
+-rwxr-xr-x   0 jpic      (1000) jpic      (1000)      848 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.7/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/ja.js
+-rwxr-xr-x   0 jpic      (1000) jpic      (1000)     1065 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.7/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/km.js
+-rwxr-xr-x   0 jpic      (1000) jpic      (1000)      854 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.7/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/ko.js
+-rwxr-xr-x   0 jpic      (1000) jpic      (1000)      913 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.7/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/lt.js
+-rwxr-xr-x   0 jpic      (1000) jpic      (1000)      872 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.7/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/lv.js
+-rwxr-xr-x   0 jpic      (1000) jpic      (1000)      979 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.7/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/mk.js
+-rwxr-xr-x   0 jpic      (1000) jpic      (1000)      791 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.7/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/ms.js
+-rwxr-xr-x   0 jpic      (1000) jpic      (1000)      785 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.7/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/nb.js
+-rwxr-xr-x   0 jpic      (1000) jpic      (1000)      896 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.7/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/nl.js
+-rwxr-xr-x   0 jpic      (1000) jpic      (1000)      925 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.7/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/pl.js
+-rwxr-xr-x   0 jpic      (1000) jpic      (1000)      853 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.7/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/pt-BR.js
+-rwxr-xr-x   0 jpic      (1000) jpic      (1000)      859 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.7/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/pt.js
+-rwxr-xr-x   0 jpic      (1000) jpic      (1000)      909 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.7/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/ro.js
+-rwxr-xr-x   0 jpic      (1000) jpic      (1000)     1127 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.7/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/ru.js
+-rwxr-xr-x   0 jpic      (1000) jpic      (1000)     1184 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.7/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/sk.js
+-rwxr-xr-x   0 jpic      (1000) jpic      (1000)     1067 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.7/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/sr-Cyrl.js
+-rwxr-xr-x   0 jpic      (1000) jpic      (1000)      938 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.7/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/sr.js
+-rwxr-xr-x   0 jpic      (1000) jpic      (1000)      786 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.7/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/sv.js
+-rwxr-xr-x   0 jpic      (1000) jpic      (1000)      951 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.7/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/th.js
+-rwxr-xr-x   0 jpic      (1000) jpic      (1000)      720 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.7/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/tr.js
+-rwxr-xr-x   0 jpic      (1000) jpic      (1000)     1117 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.7/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/uk.js
+-rwxr-xr-x   0 jpic      (1000) jpic      (1000)      801 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.7/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/vi.js
+-rwxr-xr-x   0 jpic      (1000) jpic      (1000)      769 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.7/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/zh-CN.js
+-rwxr-xr-x   0 jpic      (1000) jpic      (1000)      708 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.7/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/zh-TW.js
+-rwxr-xr-x   0 jpic      (1000) jpic      (1000)   161832 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.7/src/dal_legacy_static/static/admin/js/vendor/select2/select2.full.js
+-rwxr-xr-x   0 jpic      (1000) jpic      (1000)    75005 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.7/src/dal_legacy_static/static/admin/js/vendor/select2/select2.full.min.js
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-05-12 16:01:04.204537 django-autocomplete-light-3.9.7/src/dal_queryset_sequence/
+-rw-r--r--   0 jpic      (1000) jpic      (1000)       40 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.7/src/dal_queryset_sequence/__init__.py
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     6355 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.7/src/dal_queryset_sequence/fields.py
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-05-12 16:01:04.204537 django-autocomplete-light-3.9.7/src/dal_queryset_sequence/tests/
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1545 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.7/src/dal_queryset_sequence/tests/test_views.py
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     2298 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.7/src/dal_queryset_sequence/views.py
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1703 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.7/src/dal_queryset_sequence/widgets.py
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-05-12 16:01:04.204537 django-autocomplete-light-3.9.7/src/dal_select2/
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      149 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.7/src/dal_select2/__init__.py
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      274 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.7/src/dal_select2/apps.py
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1795 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.7/src/dal_select2/fields.py
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-05-12 16:01:04.194537 django-autocomplete-light-3.9.7/src/dal_select2/locale/
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-05-12 16:01:04.194537 django-autocomplete-light-3.9.7/src/dal_select2/locale/bg/
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-05-12 16:01:04.204537 django-autocomplete-light-3.9.7/src/dal_select2/locale/bg/LC_MESSAGES/
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      508 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.7/src/dal_select2/locale/bg/LC_MESSAGES/django.mo
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      671 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.7/src/dal_select2/locale/bg/LC_MESSAGES/django.po
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-05-12 16:01:04.194537 django-autocomplete-light-3.9.7/src/dal_select2/locale/cs/
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-05-12 16:01:04.204537 django-autocomplete-light-3.9.7/src/dal_select2/locale/cs/LC_MESSAGES/
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      528 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.7/src/dal_select2/locale/cs/LC_MESSAGES/django.mo
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      691 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.7/src/dal_select2/locale/cs/LC_MESSAGES/django.po
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-05-12 16:01:04.194537 django-autocomplete-light-3.9.7/src/dal_select2/locale/de/
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-05-12 16:01:04.204537 django-autocomplete-light-3.9.7/src/dal_select2/locale/de/LC_MESSAGES/
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      501 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.7/src/dal_select2/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      664 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.7/src/dal_select2/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-05-12 16:01:04.194537 django-autocomplete-light-3.9.7/src/dal_select2/locale/es/
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-05-12 16:01:04.204537 django-autocomplete-light-3.9.7/src/dal_select2/locale/es/LC_MESSAGES/
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      497 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.7/src/dal_select2/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      660 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.7/src/dal_select2/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-05-12 16:01:04.194537 django-autocomplete-light-3.9.7/src/dal_select2/locale/fi/
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-05-12 16:01:04.204537 django-autocomplete-light-3.9.7/src/dal_select2/locale/fi/LC_MESSAGES/
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      488 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.7/src/dal_select2/locale/fi/LC_MESSAGES/django.mo
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      684 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.7/src/dal_select2/locale/fi/LC_MESSAGES/django.po
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-05-12 16:01:04.194537 django-autocomplete-light-3.9.7/src/dal_select2/locale/fr/
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-05-12 16:01:04.204537 django-autocomplete-light-3.9.7/src/dal_select2/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      497 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.7/src/dal_select2/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      660 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.7/src/dal_select2/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-05-12 16:01:04.194537 django-autocomplete-light-3.9.7/src/dal_select2/locale/it/
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-05-12 16:01:04.204537 django-autocomplete-light-3.9.7/src/dal_select2/locale/it/LC_MESSAGES/
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      498 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.7/src/dal_select2/locale/it/LC_MESSAGES/django.mo
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      661 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.7/src/dal_select2/locale/it/LC_MESSAGES/django.po
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-05-12 16:01:04.194537 django-autocomplete-light-3.9.7/src/dal_select2/locale/ja/
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-05-12 16:01:04.204537 django-autocomplete-light-3.9.7/src/dal_select2/locale/ja/LC_MESSAGES/
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      497 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.7/src/dal_select2/locale/ja/LC_MESSAGES/django.mo
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      660 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.7/src/dal_select2/locale/ja/LC_MESSAGES/django.po
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-05-12 16:01:04.194537 django-autocomplete-light-3.9.7/src/dal_select2/locale/nl/
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-05-12 16:01:04.204537 django-autocomplete-light-3.9.7/src/dal_select2/locale/nl/LC_MESSAGES/
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      500 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.7/src/dal_select2/locale/nl/LC_MESSAGES/django.mo
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      663 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.7/src/dal_select2/locale/nl/LC_MESSAGES/django.po
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-05-12 16:01:04.194537 django-autocomplete-light-3.9.7/src/dal_select2/locale/pl/
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-05-12 16:01:04.207870 django-autocomplete-light-3.9.7/src/dal_select2/locale/pl/LC_MESSAGES/
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      557 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.7/src/dal_select2/locale/pl/LC_MESSAGES/django.mo
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      723 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.7/src/dal_select2/locale/pl/LC_MESSAGES/django.po
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-05-12 16:01:04.194537 django-autocomplete-light-3.9.7/src/dal_select2/locale/pt-br/
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-05-12 16:01:04.207870 django-autocomplete-light-3.9.7/src/dal_select2/locale/pt-br/LC_MESSAGES/
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      503 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.7/src/dal_select2/locale/pt-br/LC_MESSAGES/django.mo
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      670 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.7/src/dal_select2/locale/pt-br/LC_MESSAGES/django.po
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-05-12 16:01:04.194537 django-autocomplete-light-3.9.7/src/dal_select2/locale/ru/
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-05-12 16:01:04.207870 django-autocomplete-light-3.9.7/src/dal_select2/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      644 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.7/src/dal_select2/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      813 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.7/src/dal_select2/locale/ru/LC_MESSAGES/django.po
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-05-12 16:01:04.194537 django-autocomplete-light-3.9.7/src/dal_select2/locale/tr/
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-05-12 16:01:04.207870 django-autocomplete-light-3.9.7/src/dal_select2/locale/tr/LC_MESSAGES/
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      492 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.7/src/dal_select2/locale/tr/LC_MESSAGES/django.mo
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      741 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.7/src/dal_select2/locale/tr/LC_MESSAGES/django.po
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-05-12 16:01:04.194537 django-autocomplete-light-3.9.7/src/dal_select2/locale/uk/
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-05-12 16:01:04.207870 django-autocomplete-light-3.9.7/src/dal_select2/locale/uk/LC_MESSAGES/
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      582 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.7/src/dal_select2/locale/uk/LC_MESSAGES/django.mo
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      748 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.7/src/dal_select2/locale/uk/LC_MESSAGES/django.po
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-05-12 16:01:04.194537 django-autocomplete-light-3.9.7/src/dal_select2/locale/zh-cn/
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-05-12 16:01:04.207870 django-autocomplete-light-3.9.7/src/dal_select2/locale/zh-cn/LC_MESSAGES/
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      458 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.7/src/dal_select2/locale/zh-cn/LC_MESSAGES/django.mo
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      617 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.7/src/dal_select2/locale/zh-cn/LC_MESSAGES/django.po
+-rw-r--r--   0 jpic      (1000) jpic      (1000)       46 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.7/src/dal_select2/models.py
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-05-12 16:01:04.194537 django-autocomplete-light-3.9.7/src/dal_select2/static/
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-05-12 16:01:04.207870 django-autocomplete-light-3.9.7/src/dal_select2/static/autocomplete_light/
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     2765 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.7/src/dal_select2/static/autocomplete_light/select2.css
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     4937 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.7/src/dal_select2/static/autocomplete_light/select2.js
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     2014 2023-05-12 16:01:03.000000 django-autocomplete-light-3.9.7/src/dal_select2/static/autocomplete_light/select2.min.js
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-05-12 16:01:04.194537 django-autocomplete-light-3.9.7/src/dal_select2/static/vendor/
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-05-12 16:01:04.194537 django-autocomplete-light-3.9.7/src/dal_select2/static/vendor/select2/
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-05-12 16:01:04.194537 django-autocomplete-light-3.9.7/src/dal_select2/static/vendor/select2/dist/
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-05-12 16:01:04.207870 django-autocomplete-light-3.9.7/src/dal_select2/static/vendor/select2/dist/css/
+-rw-r--r--   0 jpic      (1000) jpic      (1000)    18931 2023-05-12 16:01:02.000000 django-autocomplete-light-3.9.7/src/dal_select2/static/vendor/select2/dist/css/select2.css
+-rw-r--r--   0 jpic      (1000) jpic      (1000)    16264 2023-05-12 16:01:02.000000 django-autocomplete-light-3.9.7/src/dal_select2/static/vendor/select2/dist/css/select2.min.css
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1071 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.7/src/dal_select2/test.py
+-rw-r--r--   0 jpic      (1000) jpic      (1000)    10574 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.7/src/dal_select2/views.py
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     6206 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.7/src/dal_select2/widgets.py
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-05-12 16:01:04.207870 django-autocomplete-light-3.9.7/src/dal_select2_queryset_sequence/
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      580 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.7/src/dal_select2_queryset_sequence/__init__.py
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     2704 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.7/src/dal_select2_queryset_sequence/fields.py
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     3501 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.7/src/dal_select2_queryset_sequence/views.py
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      975 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.7/src/dal_select2_queryset_sequence/widgets.py
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-05-12 16:01:04.207870 django-autocomplete-light-3.9.7/src/dal_select2_tagging/
+-rw-r--r--   0 jpic      (1000) jpic      (1000)       50 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.7/src/dal_select2_tagging/__init__.py
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      895 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.7/src/dal_select2_tagging/widgets.py
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-05-12 16:01:04.207870 django-autocomplete-light-3.9.7/src/dal_select2_taggit/
+-rw-r--r--   0 jpic      (1000) jpic      (1000)       42 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.7/src/dal_select2_taggit/__init__.py
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1834 2023-05-12 15:37:43.000000 django-autocomplete-light-3.9.7/src/dal_select2_taggit/widgets.py
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-05-12 16:01:04.207870 django-autocomplete-light-3.9.7/src/django_autocomplete_light.egg-info/
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     3323 2023-05-12 16:01:04.000000 django-autocomplete-light-3.9.7/src/django_autocomplete_light.egg-info/PKG-INFO
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     9762 2023-05-12 16:01:04.000000 django-autocomplete-light-3.9.7/src/django_autocomplete_light.egg-info/SOURCES.txt
+-rw-r--r--   0 jpic      (1000) jpic      (1000)        1 2023-05-12 16:01:04.000000 django-autocomplete-light-3.9.7/src/django_autocomplete_light.egg-info/dependency_links.txt
+-rw-r--r--   0 jpic      (1000) jpic      (1000)        1 2023-05-12 15:43:49.000000 django-autocomplete-light-3.9.7/src/django_autocomplete_light.egg-info/not-zip-safe
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      146 2023-05-12 16:01:04.000000 django-autocomplete-light-3.9.7/src/django_autocomplete_light.egg-info/requires.txt
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      226 2023-05-12 16:01:04.000000 django-autocomplete-light-3.9.7/src/django_autocomplete_light.egg-info/top_level.txt
```

### Comparing `django-autocomplete-light-3.9.6rc1/AUTHORS` & `django-autocomplete-light-3.9.7/AUTHORS`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/CHANGELOG` & `django-autocomplete-light-3.9.7/CHANGELOG`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 
 
 
 
+
+
 3.9.5-rc6
 
     2023-04-07 Release 3.9.5-rc6
     dea11bf changelog.py: fix release dates and tag commits by jpic
 
 3.9.5-rc5
```

### Comparing `django-autocomplete-light-3.9.6rc1/CHANGES.txt` & `django-autocomplete-light-3.9.7/CHANGES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 
 
 
 
+
+
 3.9.5-rc6
 
     2023-04-07 Release 3.9.5-rc6
     dea11bf changelog.py: fix release dates and tag commits by jpic
 
 3.9.5-rc5
```

### Comparing `django-autocomplete-light-3.9.6rc1/LICENSE` & `django-autocomplete-light-3.9.7/LICENSE`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/PKG-INFO` & `django-autocomplete-light-3.9.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-autocomplete-light
-Version: 3.9.6rc1
+Version: 3.9.7
 Summary: Fresh autocompletes for Django
 Home-page: http://django-autocomplete-light.rtfd.org
 Author: James Pic
 Author-email: jamespic@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/yourlabs/django-autocomplete-light
 Keywords: django autocomplete
```

### Comparing `django-autocomplete-light-3.9.6rc1/README` & `django-autocomplete-light-3.9.7/README`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/README.rst` & `django-autocomplete-light-3.9.7/README.rst`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/setup.py` & `django-autocomplete-light-3.9.7/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # README file and 2) it's easier to type in the README file than to put a raw
 # string in below ...
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 setup(
     name='django-autocomplete-light',
-    version='3.9.6rc1',
+    version='3.9.7',
     description='Fresh autocompletes for Django',
     author='James Pic',
     author_email='jamespic@gmail.com',
     url='http://django-autocomplete-light.rtfd.org',
     project_urls={
         'Source': 'https://github.com/yourlabs/django-autocomplete-light',
     },
```

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal/autocomplete.py` & `django-autocomplete-light-3.9.7/src/dal/autocomplete.py`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal/forms.py` & `django-autocomplete-light-3.9.7/src/dal/forms.py`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal/forward.py` & `django-autocomplete-light-3.9.7/src/dal/forward.py`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal/static/autocomplete_light/autocomplete_light.js` & `django-autocomplete-light-3.9.7/src/dal/static/autocomplete_light/autocomplete_light.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal/static/autocomplete_light/autocomplete_light.min.js` & `django-autocomplete-light-3.9.7/src/dal/static/autocomplete_light/autocomplete_light.min.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal/static/autocomplete_light/i18n/af.js` & `django-autocomplete-light-3.9.7/src/dal/static/autocomplete_light/i18n/af.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal/static/autocomplete_light/i18n/ar.js` & `django-autocomplete-light-3.9.7/src/dal/static/autocomplete_light/i18n/ar.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal/static/autocomplete_light/i18n/az.js` & `django-autocomplete-light-3.9.7/src/dal/static/autocomplete_light/i18n/az.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal/static/autocomplete_light/i18n/bg.js` & `django-autocomplete-light-3.9.7/src/dal/static/autocomplete_light/i18n/bg.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal/static/autocomplete_light/i18n/bn.js` & `django-autocomplete-light-3.9.7/src/dal/static/autocomplete_light/i18n/bn.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal/static/autocomplete_light/i18n/bs.js` & `django-autocomplete-light-3.9.7/src/dal/static/autocomplete_light/i18n/bs.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal/static/autocomplete_light/i18n/ca.js` & `django-autocomplete-light-3.9.7/src/dal/static/autocomplete_light/i18n/ca.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal/static/autocomplete_light/i18n/cs.js` & `django-autocomplete-light-3.9.7/src/dal/static/autocomplete_light/i18n/cs.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal/static/autocomplete_light/i18n/da.js` & `django-autocomplete-light-3.9.7/src/dal/static/autocomplete_light/i18n/da.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal/static/autocomplete_light/i18n/de.js` & `django-autocomplete-light-3.9.7/src/dal/static/autocomplete_light/i18n/de.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal/static/autocomplete_light/i18n/dsb.js` & `django-autocomplete-light-3.9.7/src/dal/static/autocomplete_light/i18n/dsb.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal/static/autocomplete_light/i18n/el.js` & `django-autocomplete-light-3.9.7/src/dal/static/autocomplete_light/i18n/el.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal/static/autocomplete_light/i18n/en.js` & `django-autocomplete-light-3.9.7/src/dal/static/autocomplete_light/i18n/en.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal/static/autocomplete_light/i18n/eo.js` & `django-autocomplete-light-3.9.7/src/dal/static/autocomplete_light/i18n/eo.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal/static/autocomplete_light/i18n/es.js` & `django-autocomplete-light-3.9.7/src/dal/static/autocomplete_light/i18n/es.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal/static/autocomplete_light/i18n/et.js` & `django-autocomplete-light-3.9.7/src/dal/static/autocomplete_light/i18n/et.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal/static/autocomplete_light/i18n/eu.js` & `django-autocomplete-light-3.9.7/src/dal/static/autocomplete_light/i18n/eu.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal/static/autocomplete_light/i18n/fa.js` & `django-autocomplete-light-3.9.7/src/dal/static/autocomplete_light/i18n/fa.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal/static/autocomplete_light/i18n/fi.js` & `django-autocomplete-light-3.9.7/src/dal/static/autocomplete_light/i18n/fi.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal/static/autocomplete_light/i18n/fr.js` & `django-autocomplete-light-3.9.7/src/dal/static/autocomplete_light/i18n/fr.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal/static/autocomplete_light/i18n/gl.js` & `django-autocomplete-light-3.9.7/src/dal/static/autocomplete_light/i18n/gl.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal/static/autocomplete_light/i18n/he.js` & `django-autocomplete-light-3.9.7/src/dal/static/autocomplete_light/i18n/he.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal/static/autocomplete_light/i18n/hi.js` & `django-autocomplete-light-3.9.7/src/dal/static/autocomplete_light/i18n/hi.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal/static/autocomplete_light/i18n/hr.js` & `django-autocomplete-light-3.9.7/src/dal/static/autocomplete_light/i18n/hr.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal/static/autocomplete_light/i18n/hsb.js` & `django-autocomplete-light-3.9.7/src/dal/static/autocomplete_light/i18n/hsb.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal/static/autocomplete_light/i18n/hu.js` & `django-autocomplete-light-3.9.7/src/dal/static/autocomplete_light/i18n/hu.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal/static/autocomplete_light/i18n/hy.js` & `django-autocomplete-light-3.9.7/src/dal/static/autocomplete_light/i18n/hy.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal/static/autocomplete_light/i18n/id.js` & `django-autocomplete-light-3.9.7/src/dal/static/autocomplete_light/i18n/id.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal/static/autocomplete_light/i18n/is.js` & `django-autocomplete-light-3.9.7/src/dal/static/autocomplete_light/i18n/is.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal/static/autocomplete_light/i18n/it.js` & `django-autocomplete-light-3.9.7/src/dal/static/autocomplete_light/i18n/it.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal/static/autocomplete_light/i18n/ja.js` & `django-autocomplete-light-3.9.7/src/dal/static/autocomplete_light/i18n/ja.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal/static/autocomplete_light/i18n/ka.js` & `django-autocomplete-light-3.9.7/src/dal/static/autocomplete_light/i18n/ka.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal/static/autocomplete_light/i18n/km.js` & `django-autocomplete-light-3.9.7/src/dal/static/autocomplete_light/i18n/km.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal/static/autocomplete_light/i18n/ko.js` & `django-autocomplete-light-3.9.7/src/dal/static/autocomplete_light/i18n/ko.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal/static/autocomplete_light/i18n/lt.js` & `django-autocomplete-light-3.9.7/src/dal/static/autocomplete_light/i18n/lt.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal/static/autocomplete_light/i18n/lv.js` & `django-autocomplete-light-3.9.7/src/dal/static/autocomplete_light/i18n/lv.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal/static/autocomplete_light/i18n/mk.js` & `django-autocomplete-light-3.9.7/src/dal/static/autocomplete_light/i18n/mk.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal/static/autocomplete_light/i18n/ms.js` & `django-autocomplete-light-3.9.7/src/dal/static/autocomplete_light/i18n/ms.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal/static/autocomplete_light/i18n/nb.js` & `django-autocomplete-light-3.9.7/src/dal/static/autocomplete_light/i18n/nb.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal/static/autocomplete_light/i18n/ne.js` & `django-autocomplete-light-3.9.7/src/dal/static/autocomplete_light/i18n/ne.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal/static/autocomplete_light/i18n/nl.js` & `django-autocomplete-light-3.9.7/src/dal/static/autocomplete_light/i18n/nl.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal/static/autocomplete_light/i18n/pa.js` & `django-autocomplete-light-3.9.7/src/dal/static/autocomplete_light/i18n/pa.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal/static/autocomplete_light/i18n/pl.js` & `django-autocomplete-light-3.9.7/src/dal/static/autocomplete_light/i18n/pl.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal/static/autocomplete_light/i18n/ps.js` & `django-autocomplete-light-3.9.7/src/dal/static/autocomplete_light/i18n/ps.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal/static/autocomplete_light/i18n/pt-BR.js` & `django-autocomplete-light-3.9.7/src/dal/static/autocomplete_light/i18n/pt-BR.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal/static/autocomplete_light/i18n/pt.js` & `django-autocomplete-light-3.9.7/src/dal/static/autocomplete_light/i18n/pt.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal/static/autocomplete_light/i18n/ro.js` & `django-autocomplete-light-3.9.7/src/dal/static/autocomplete_light/i18n/ro.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal/static/autocomplete_light/i18n/ru.js` & `django-autocomplete-light-3.9.7/src/dal/static/autocomplete_light/i18n/ru.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal/static/autocomplete_light/i18n/sk.js` & `django-autocomplete-light-3.9.7/src/dal/static/autocomplete_light/i18n/sk.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal/static/autocomplete_light/i18n/sl.js` & `django-autocomplete-light-3.9.7/src/dal/static/autocomplete_light/i18n/sl.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal/static/autocomplete_light/i18n/sq.js` & `django-autocomplete-light-3.9.7/src/dal/static/autocomplete_light/i18n/sq.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal/static/autocomplete_light/i18n/sr-Cyrl.js` & `django-autocomplete-light-3.9.7/src/dal/static/autocomplete_light/i18n/sr-Cyrl.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal/static/autocomplete_light/i18n/sr.js` & `django-autocomplete-light-3.9.7/src/dal/static/autocomplete_light/i18n/sr.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal/static/autocomplete_light/i18n/sv.js` & `django-autocomplete-light-3.9.7/src/dal/static/autocomplete_light/i18n/sv.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal/static/autocomplete_light/i18n/te.js` & `django-autocomplete-light-3.9.7/src/dal/static/autocomplete_light/i18n/te.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal/static/autocomplete_light/i18n/th.js` & `django-autocomplete-light-3.9.7/src/dal/static/autocomplete_light/i18n/th.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal/static/autocomplete_light/i18n/tk.js` & `django-autocomplete-light-3.9.7/src/dal/static/autocomplete_light/i18n/tk.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal/static/autocomplete_light/i18n/tr.js` & `django-autocomplete-light-3.9.7/src/dal/static/autocomplete_light/i18n/tr.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal/static/autocomplete_light/i18n/uk.js` & `django-autocomplete-light-3.9.7/src/dal/static/autocomplete_light/i18n/uk.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal/static/autocomplete_light/i18n/vi.js` & `django-autocomplete-light-3.9.7/src/dal/static/autocomplete_light/i18n/vi.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal/static/autocomplete_light/i18n/zh-CN.js` & `django-autocomplete-light-3.9.7/src/dal/static/autocomplete_light/i18n/zh-CN.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal/static/autocomplete_light/i18n/zh-TW.js` & `django-autocomplete-light-3.9.7/src/dal/static/autocomplete_light/i18n/zh-TW.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal/test/case.py` & `django-autocomplete-light-3.9.7/src/dal/test/case.py`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal/test/stories.py` & `django-autocomplete-light-3.9.7/src/dal/test/stories.py`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal/test/utils.py` & `django-autocomplete-light-3.9.7/src/dal/test/utils.py`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal/views.py` & `django-autocomplete-light-3.9.7/src/dal/views.py`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal/widgets.py` & `django-autocomplete-light-3.9.7/src/dal/widgets.py`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal_contenttypes/fields.py` & `django-autocomplete-light-3.9.7/src/dal_contenttypes/fields.py`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal_genericm2m/fields.py` & `django-autocomplete-light-3.9.7/src/dal_genericm2m/fields.py`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal_gm2m/fields.py` & `django-autocomplete-light-3.9.7/src/dal_gm2m/fields.py`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal_legacy_static/static/admin/css/autocomplete.css` & `django-autocomplete-light-3.9.7/src/dal_legacy_static/static/admin/css/autocomplete.css`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal_legacy_static/static/admin/css/vendor/select2/select2.css` & `django-autocomplete-light-3.9.7/src/dal_legacy_static/static/admin/css/vendor/select2/select2.css`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal_legacy_static/static/admin/css/vendor/select2/select2.min.css` & `django-autocomplete-light-3.9.7/src/dal_legacy_static/static/admin/css/vendor/select2/select2.min.css`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal_legacy_static/static/admin/js/autocomplete.js` & `django-autocomplete-light-3.9.7/src/dal_legacy_static/static/admin/js/autocomplete.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/ar.js` & `django-autocomplete-light-3.9.7/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/ar.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/az.js` & `django-autocomplete-light-3.9.7/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/az.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/bg.js` & `django-autocomplete-light-3.9.7/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/bg.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/ca.js` & `django-autocomplete-light-3.9.7/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/ca.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/cs.js` & `django-autocomplete-light-3.9.7/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/cs.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/da.js` & `django-autocomplete-light-3.9.7/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/da.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/de.js` & `django-autocomplete-light-3.9.7/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/de.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/el.js` & `django-autocomplete-light-3.9.7/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/el.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/en.js` & `django-autocomplete-light-3.9.7/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/en.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/es.js` & `django-autocomplete-light-3.9.7/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/es.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/et.js` & `django-autocomplete-light-3.9.7/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/et.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/eu.js` & `django-autocomplete-light-3.9.7/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/eu.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/fa.js` & `django-autocomplete-light-3.9.7/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/fa.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/fi.js` & `django-autocomplete-light-3.9.7/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/fi.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/fr.js` & `django-autocomplete-light-3.9.7/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/fr.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/gl.js` & `django-autocomplete-light-3.9.7/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/gl.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/he.js` & `django-autocomplete-light-3.9.7/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/he.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/hi.js` & `django-autocomplete-light-3.9.7/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/hi.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/hr.js` & `django-autocomplete-light-3.9.7/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/hr.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/hu.js` & `django-autocomplete-light-3.9.7/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/hu.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/id.js` & `django-autocomplete-light-3.9.7/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/id.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/is.js` & `django-autocomplete-light-3.9.7/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/is.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/it.js` & `django-autocomplete-light-3.9.7/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/it.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/ja.js` & `django-autocomplete-light-3.9.7/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/ja.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/km.js` & `django-autocomplete-light-3.9.7/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/km.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/ko.js` & `django-autocomplete-light-3.9.7/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/ko.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/lt.js` & `django-autocomplete-light-3.9.7/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/lt.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/lv.js` & `django-autocomplete-light-3.9.7/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/lv.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/mk.js` & `django-autocomplete-light-3.9.7/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/mk.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/ms.js` & `django-autocomplete-light-3.9.7/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/ms.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/nb.js` & `django-autocomplete-light-3.9.7/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/nb.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/nl.js` & `django-autocomplete-light-3.9.7/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/nl.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/pl.js` & `django-autocomplete-light-3.9.7/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/pl.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/pt-BR.js` & `django-autocomplete-light-3.9.7/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/pt-BR.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/pt.js` & `django-autocomplete-light-3.9.7/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/pt.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/ro.js` & `django-autocomplete-light-3.9.7/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/ro.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/ru.js` & `django-autocomplete-light-3.9.7/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/ru.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/sk.js` & `django-autocomplete-light-3.9.7/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/sk.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/sr-Cyrl.js` & `django-autocomplete-light-3.9.7/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/sr-Cyrl.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/sr.js` & `django-autocomplete-light-3.9.7/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/sr.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/sv.js` & `django-autocomplete-light-3.9.7/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/sv.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/th.js` & `django-autocomplete-light-3.9.7/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/th.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/tr.js` & `django-autocomplete-light-3.9.7/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/tr.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/uk.js` & `django-autocomplete-light-3.9.7/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/uk.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/vi.js` & `django-autocomplete-light-3.9.7/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/vi.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/zh-CN.js` & `django-autocomplete-light-3.9.7/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/zh-CN.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/zh-TW.js` & `django-autocomplete-light-3.9.7/src/dal_legacy_static/static/admin/js/vendor/select2/i18n/zh-TW.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal_legacy_static/static/admin/js/vendor/select2/select2.full.js` & `django-autocomplete-light-3.9.7/src/dal_legacy_static/static/admin/js/vendor/select2/select2.full.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal_legacy_static/static/admin/js/vendor/select2/select2.full.min.js` & `django-autocomplete-light-3.9.7/src/dal_legacy_static/static/admin/js/vendor/select2/select2.full.min.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal_queryset_sequence/fields.py` & `django-autocomplete-light-3.9.7/src/dal_queryset_sequence/fields.py`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal_queryset_sequence/tests/test_views.py` & `django-autocomplete-light-3.9.7/src/dal_queryset_sequence/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal_queryset_sequence/views.py` & `django-autocomplete-light-3.9.7/src/dal_queryset_sequence/views.py`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal_queryset_sequence/widgets.py` & `django-autocomplete-light-3.9.7/src/dal_queryset_sequence/widgets.py`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal_select2/fields.py` & `django-autocomplete-light-3.9.7/src/dal_select2/fields.py`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal_select2/locale/bg/LC_MESSAGES/django.po` & `django-autocomplete-light-3.9.7/src/dal_select2/locale/bg/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal_select2/locale/cs/LC_MESSAGES/django.mo` & `django-autocomplete-light-3.9.7/src/dal_select2/locale/cs/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal_select2/locale/cs/LC_MESSAGES/django.po` & `django-autocomplete-light-3.9.7/src/dal_select2/locale/cs/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal_select2/locale/de/LC_MESSAGES/django.po` & `django-autocomplete-light-3.9.7/src/dal_select2/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal_select2/locale/es/LC_MESSAGES/django.po` & `django-autocomplete-light-3.9.7/src/dal_select2/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal_select2/locale/fi/LC_MESSAGES/django.po` & `django-autocomplete-light-3.9.7/src/dal_select2/locale/fi/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal_select2/locale/fr/LC_MESSAGES/django.po` & `django-autocomplete-light-3.9.7/src/dal_select2/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal_select2/locale/it/LC_MESSAGES/django.po` & `django-autocomplete-light-3.9.7/src/dal_select2/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal_select2/locale/ja/LC_MESSAGES/django.po` & `django-autocomplete-light-3.9.7/src/dal_select2/locale/ja/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal_select2/locale/nl/LC_MESSAGES/django.po` & `django-autocomplete-light-3.9.7/src/dal_select2/locale/nl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal_select2/locale/pl/LC_MESSAGES/django.mo` & `django-autocomplete-light-3.9.7/src/dal_select2/locale/pl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal_select2/locale/pl/LC_MESSAGES/django.po` & `django-autocomplete-light-3.9.7/src/dal_select2/locale/pl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal_select2/locale/pt-br/LC_MESSAGES/django.po` & `django-autocomplete-light-3.9.7/src/dal_select2/locale/pt-br/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal_select2/locale/ru/LC_MESSAGES/django.mo` & `django-autocomplete-light-3.9.7/src/dal_select2/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal_select2/locale/ru/LC_MESSAGES/django.po` & `django-autocomplete-light-3.9.7/src/dal_select2/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal_select2/locale/tr/LC_MESSAGES/django.po` & `django-autocomplete-light-3.9.7/src/dal_select2/locale/tr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal_select2/locale/uk/LC_MESSAGES/django.mo` & `django-autocomplete-light-3.9.7/src/dal_select2/locale/uk/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal_select2/locale/uk/LC_MESSAGES/django.po` & `django-autocomplete-light-3.9.7/src/dal_select2/locale/uk/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal_select2/locale/zh-cn/LC_MESSAGES/django.po` & `django-autocomplete-light-3.9.7/src/dal_select2/locale/zh-cn/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal_select2/static/autocomplete_light/select2.css` & `django-autocomplete-light-3.9.7/src/dal_select2/static/autocomplete_light/select2.css`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal_select2/static/autocomplete_light/select2.js` & `django-autocomplete-light-3.9.7/src/dal_select2/static/autocomplete_light/select2.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal_select2/static/autocomplete_light/select2.min.js` & `django-autocomplete-light-3.9.7/src/dal_select2/static/autocomplete_light/select2.min.js`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal_select2/static/vendor/select2/dist/css/select2.css` & `django-autocomplete-light-3.9.7/src/dal_select2/static/vendor/select2/dist/css/select2.css`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal_select2/static/vendor/select2/dist/css/select2.min.css` & `django-autocomplete-light-3.9.7/src/dal_select2/static/vendor/select2/dist/css/select2.min.css`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal_select2/test.py` & `django-autocomplete-light-3.9.7/src/dal_select2/test.py`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal_select2/views.py` & `django-autocomplete-light-3.9.7/src/dal_select2/views.py`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal_select2/widgets.py` & `django-autocomplete-light-3.9.7/src/dal_select2/widgets.py`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal_select2_queryset_sequence/__init__.py` & `django-autocomplete-light-3.9.7/src/dal_select2_queryset_sequence/__init__.py`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal_select2_queryset_sequence/fields.py` & `django-autocomplete-light-3.9.7/src/dal_select2_queryset_sequence/fields.py`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal_select2_queryset_sequence/views.py` & `django-autocomplete-light-3.9.7/src/dal_select2_queryset_sequence/views.py`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal_select2_queryset_sequence/widgets.py` & `django-autocomplete-light-3.9.7/src/dal_select2_queryset_sequence/widgets.py`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal_select2_tagging/widgets.py` & `django-autocomplete-light-3.9.7/src/dal_select2_tagging/widgets.py`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/dal_select2_taggit/widgets.py` & `django-autocomplete-light-3.9.7/src/dal_select2_taggit/widgets.py`

 * *Files identical despite different names*

### Comparing `django-autocomplete-light-3.9.6rc1/src/django_autocomplete_light.egg-info/PKG-INFO` & `django-autocomplete-light-3.9.7/src/django_autocomplete_light.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-autocomplete-light
-Version: 3.9.6rc1
+Version: 3.9.7
 Summary: Fresh autocompletes for Django
 Home-page: http://django-autocomplete-light.rtfd.org
 Author: James Pic
 Author-email: jamespic@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/yourlabs/django-autocomplete-light
 Keywords: django autocomplete
```

### Comparing `django-autocomplete-light-3.9.6rc1/src/django_autocomplete_light.egg-info/SOURCES.txt` & `django-autocomplete-light-3.9.7/src/django_autocomplete_light.egg-info/SOURCES.txt`

 * *Files identical despite different names*

