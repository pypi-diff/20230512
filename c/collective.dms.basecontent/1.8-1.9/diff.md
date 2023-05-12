# Comparing `tmp/collective.dms.basecontent-1.8.tar.gz` & `tmp/collective.dms.basecontent-1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "collective.dms.basecontent-1.8.tar", last modified: Fri Jul  1 09:38:44 2022, max compression
+gzip compressed data, was "collective.dms.basecontent-1.9.tar", last modified: Fri Oct 28 11:31:31 2022, max compression
```

## Comparing `collective.dms.basecontent-1.8.tar` & `collective.dms.basecontent-1.9.tar`

### file list

```diff
@@ -1,110 +1,111 @@
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2022-07-01 09:38:44.343126 collective.dms.basecontent-1.8/
--rw-rw-r--   0 sge       (1000) sge       (1000)      173 2022-07-01 09:38:44.000000 collective.dms.basecontent-1.8/.gitignore
--rw-rw-r--   0 sge       (1000) sge       (1000)      296 2022-07-01 09:38:44.000000 collective.dms.basecontent-1.8/.travis.yml
--rw-rw-r--   0 sge       (1000) sge       (1000)     2787 2022-07-01 09:38:44.000000 collective.dms.basecontent-1.8/CHANGES.rst
--rw-rw-r--   0 sge       (1000) sge       (1000)      138 2022-07-01 09:38:44.000000 collective.dms.basecontent-1.8/CONTRIBUTORS.rst
--rw-rw-r--   0 sge       (1000) sge       (1000)       78 2022-07-01 09:38:44.000000 collective.dms.basecontent-1.8/MANIFEST.in
--rw-rw-r--   0 sge       (1000) sge       (1000)     4922 2022-07-01 09:38:44.343126 collective.dms.basecontent-1.8/PKG-INFO
--rw-rw-r--   0 sge       (1000) sge       (1000)     1032 2022-07-01 09:38:44.000000 collective.dms.basecontent-1.8/README.rst
--rw-rw-r--   0 sge       (1000) sge       (1000)      275 2022-07-01 09:38:44.000000 collective.dms.basecontent-1.8/base.cfg
--rw-rw-r--   0 sge       (1000) sge       (1000)     7458 2022-07-01 09:38:44.000000 collective.dms.basecontent-1.8/bootstrap.py
--rw-rw-r--   0 sge       (1000) sge       (1000)      141 2022-07-01 09:38:44.000000 collective.dms.basecontent-1.8/buildout.cfg
--rw-rw-r--   0 sge       (1000) sge       (1000)      161 2022-07-01 09:38:44.000000 collective.dms.basecontent-1.8/checkouts.cfg
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2022-07-01 09:38:44.343126 collective.dms.basecontent-1.8/docs/
--rw-rw-r--   0 sge       (1000) sge       (1000)    18092 2022-07-01 09:38:44.000000 collective.dms.basecontent-1.8/docs/LICENSE.GPL
--rw-rw-r--   0 sge       (1000) sge       (1000)      738 2022-07-01 09:38:44.000000 collective.dms.basecontent-1.8/docs/LICENSE.txt
--rw-rw-r--   0 sge       (1000) sge       (1000)      727 2022-07-01 09:38:44.000000 collective.dms.basecontent-1.8/jenkins-base.cfg
--rw-rw-r--   0 sge       (1000) sge       (1000)       96 2022-07-01 09:38:44.000000 collective.dms.basecontent-1.8/jenkins.cfg
--rw-rw-r--   0 sge       (1000) sge       (1000)       38 2022-07-01 09:38:44.343126 collective.dms.basecontent-1.8/setup.cfg
--rw-rw-r--   0 sge       (1000) sge       (1000)     2331 2022-07-01 09:38:44.000000 collective.dms.basecontent-1.8/setup.py
--rw-rw-r--   0 sge       (1000) sge       (1000)      638 2022-07-01 09:38:44.000000 collective.dms.basecontent-1.8/sources.cfg
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2022-07-01 09:38:44.339126 collective.dms.basecontent-1.8/src/
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2022-07-01 09:38:44.343126 collective.dms.basecontent-1.8/src/collective/
--rw-rw-r--   0 sge       (1000) sge       (1000)       56 2022-07-01 09:38:44.000000 collective.dms.basecontent-1.8/src/collective/__init__.py
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2022-07-01 09:38:44.343126 collective.dms.basecontent-1.8/src/collective/dms/
--rw-rw-r--   0 sge       (1000) sge       (1000)       56 2022-07-01 09:38:44.000000 collective.dms.basecontent-1.8/src/collective/dms/__init__.py
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2022-07-01 09:38:44.343126 collective.dms.basecontent-1.8/src/collective/dms/basecontent/
--rw-rw-r--   0 sge       (1000) sge       (1000)      183 2022-07-01 09:38:44.000000 collective.dms.basecontent-1.8/src/collective/dms/basecontent/__init__.py
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2022-07-01 09:38:44.343126 collective.dms.basecontent-1.8/src/collective/dms/basecontent/browser/
--rw-rw-r--   0 sge       (1000) sge       (1000)        1 2022-07-01 09:38:44.000000 collective.dms.basecontent-1.8/src/collective/dms/basecontent/browser/__init__.py
--rw-rw-r--   0 sge       (1000) sge       (1000)     5093 2022-07-01 09:38:44.000000 collective.dms.basecontent-1.8/src/collective/dms/basecontent/browser/batch.py
--rw-rw-r--   0 sge       (1000) sge       (1000)     7086 2022-07-01 09:38:44.000000 collective.dms.basecontent-1.8/src/collective/dms/basecontent/browser/column.py
--rw-rw-r--   0 sge       (1000) sge       (1000)     1476 2022-07-01 09:38:44.000000 collective.dms.basecontent-1.8/src/collective/dms/basecontent/browser/configure.zcml
--rw-rw-r--   0 sge       (1000) sge       (1000)     3109 2022-07-01 09:38:44.000000 collective.dms.basecontent-1.8/src/collective/dms/basecontent/browser/listing.py
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2022-07-01 09:38:44.339126 collective.dms.basecontent-1.8/src/collective/dms/basecontent/browser/static/
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2022-07-01 09:38:44.343126 collective.dms.basecontent-1.8/src/collective/dms/basecontent/browser/static/img/
--rw-rw-r--   0 sge       (1000) sge       (1000)      334 2022-07-01 09:38:44.000000 collective.dms.basecontent-1.8/src/collective/dms/basecontent/browser/static/img/dmsappendixfile_icon.png
--rw-rw-r--   0 sge       (1000) sge       (1000)      249 2022-07-01 09:38:44.000000 collective.dms.basecontent-1.8/src/collective/dms/basecontent/browser/static/img/dmsdocument_icon.png
--rw-rw-r--   0 sge       (1000) sge       (1000)      675 2022-07-01 09:38:44.000000 collective.dms.basecontent-1.8/src/collective/dms/basecontent/browser/static/img/dmsmainfile_icon.png
--rw-rw-r--   0 sge       (1000) sge       (1000)      330 2022-07-01 09:38:44.000000 collective.dms.basecontent-1.8/src/collective/dms/basecontent/browser/static/img/fade_edit.png
--rw-rw-r--   0 sge       (1000) sge       (1000)     3308 2022-07-01 09:38:44.000000 collective.dms.basecontent-1.8/src/collective/dms/basecontent/browser/table.py
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2022-07-01 09:38:44.343126 collective.dms.basecontent-1.8/src/collective/dms/basecontent/browser/templates/
--rw-rw-r--   0 sge       (1000) sge       (1000)     2845 2022-07-01 09:38:44.000000 collective.dms.basecontent-1.8/src/collective/dms/basecontent/browser/templates/dmsdocument_edit.pt
--rw-rw-r--   0 sge       (1000) sge       (1000)     2701 2022-07-01 09:38:44.000000 collective.dms.basecontent-1.8/src/collective/dms/basecontent/browser/templates/dmsdocument_view.pt
--rw-rw-r--   0 sge       (1000) sge       (1000)      241 2022-07-01 09:38:44.000000 collective.dms.basecontent-1.8/src/collective/dms/basecontent/browser/templates/filesviewlet.pt
--rw-rw-r--   0 sge       (1000) sge       (1000)     2265 2022-07-01 09:38:44.000000 collective.dms.basecontent-1.8/src/collective/dms/basecontent/browser/templates/versionsviewlet.pt
--rw-rw-r--   0 sge       (1000) sge       (1000)     1426 2022-07-01 09:38:44.000000 collective.dms.basecontent-1.8/src/collective/dms/basecontent/browser/templates/versionviewer.pt
--rw-rw-r--   0 sge       (1000) sge       (1000)     2645 2022-07-01 09:38:44.000000 collective.dms.basecontent-1.8/src/collective/dms/basecontent/browser/viewlets.py
--rw-rw-r--   0 sge       (1000) sge       (1000)     1288 2022-07-01 09:38:44.000000 collective.dms.basecontent-1.8/src/collective/dms/basecontent/browser/views.py
--rw-rw-r--   0 sge       (1000) sge       (1000)     2198 2022-07-01 09:38:44.000000 collective.dms.basecontent-1.8/src/collective/dms/basecontent/configure.zcml
--rw-rw-r--   0 sge       (1000) sge       (1000)     1616 2022-07-01 09:38:44.000000 collective.dms.basecontent-1.8/src/collective/dms/basecontent/dmsdocument.py
--rw-rw-r--   0 sge       (1000) sge       (1000)     2677 2022-07-01 09:38:44.000000 collective.dms.basecontent-1.8/src/collective/dms/basecontent/dmsfile.py
--rw-rw-r--   0 sge       (1000) sge       (1000)     1939 2022-07-01 09:38:44.000000 collective.dms.basecontent-1.8/src/collective/dms/basecontent/indexers.py
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2022-07-01 09:38:44.343126 collective.dms.basecontent-1.8/src/collective/dms/basecontent/locales/
--rw-rw-r--   0 sge       (1000) sge       (1000)     1533 2022-07-01 09:38:44.000000 collective.dms.basecontent-1.8/src/collective/dms/basecontent/locales/collective.dms.basecontent.pot
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2022-07-01 09:38:44.339126 collective.dms.basecontent-1.8/src/collective/dms/basecontent/locales/en/
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2022-07-01 09:38:44.343126 collective.dms.basecontent-1.8/src/collective/dms/basecontent/locales/en/LC_MESSAGES/
--rw-rw-r--   0 sge       (1000) sge       (1000)     1468 2022-07-01 09:38:44.000000 collective.dms.basecontent-1.8/src/collective/dms/basecontent/locales/en/LC_MESSAGES/collective.dms.basecontent.po
--rw-rw-r--   0 sge       (1000) sge       (1000)     1230 2022-07-01 09:38:44.000000 collective.dms.basecontent-1.8/src/collective/dms/basecontent/locales/en/LC_MESSAGES/plone.po
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2022-07-01 09:38:44.339126 collective.dms.basecontent-1.8/src/collective/dms/basecontent/locales/fr/
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2022-07-01 09:38:44.343126 collective.dms.basecontent-1.8/src/collective/dms/basecontent/locales/fr/LC_MESSAGES/
--rw-rw-r--   0 sge       (1000) sge       (1000)     1735 2022-07-01 09:38:44.000000 collective.dms.basecontent-1.8/src/collective/dms/basecontent/locales/fr/LC_MESSAGES/collective.dms.basecontent.po
--rw-rw-r--   0 sge       (1000) sge       (1000)     1330 2022-07-01 09:38:44.000000 collective.dms.basecontent-1.8/src/collective/dms/basecontent/locales/fr/LC_MESSAGES/plone.po
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2022-07-01 09:38:44.339126 collective.dms.basecontent-1.8/src/collective/dms/basecontent/locales/nl/
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2022-07-01 09:38:44.343126 collective.dms.basecontent-1.8/src/collective/dms/basecontent/locales/nl/LC_MESSAGES/
--rw-rw-r--   0 sge       (1000) sge       (1000)     1454 2022-07-01 09:38:44.000000 collective.dms.basecontent-1.8/src/collective/dms/basecontent/locales/nl/LC_MESSAGES/collective.dms.basecontent.po
--rw-rw-r--   0 sge       (1000) sge       (1000)     1183 2022-07-01 09:38:44.000000 collective.dms.basecontent-1.8/src/collective/dms/basecontent/locales/nl/LC_MESSAGES/plone.po
--rw-rw-r--   0 sge       (1000) sge       (1000)     1262 2022-07-01 09:38:44.000000 collective.dms.basecontent-1.8/src/collective/dms/basecontent/locales/plone.pot
--rwxrwxr-x   0 sge       (1000) sge       (1000)      259 2022-07-01 09:38:44.000000 collective.dms.basecontent-1.8/src/collective/dms/basecontent/locales/update.sh
--rw-rw-r--   0 sge       (1000) sge       (1000)      250 2022-07-01 09:38:44.000000 collective.dms.basecontent-1.8/src/collective/dms/basecontent/permissions.zcml
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2022-07-01 09:38:44.339126 collective.dms.basecontent-1.8/src/collective/dms/basecontent/profiles/
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2022-07-01 09:38:44.343126 collective.dms.basecontent-1.8/src/collective/dms/basecontent/profiles/default/
--rw-rw-r--   0 sge       (1000) sge       (1000)      384 2022-07-01 09:38:44.000000 collective.dms.basecontent-1.8/src/collective/dms/basecontent/profiles/default/catalog.xml
--rw-rw-r--   0 sge       (1000) sge       (1000)       14 2022-07-01 09:38:44.000000 collective.dms.basecontent-1.8/src/collective/dms/basecontent/profiles/default/collective_dms_basecontent_marker.txt
--rw-rw-r--   0 sge       (1000) sge       (1000)      379 2022-07-01 09:38:44.000000 collective.dms.basecontent-1.8/src/collective/dms/basecontent/profiles/default/metadata.xml
--rw-rw-r--   0 sge       (1000) sge       (1000)      482 2022-07-01 09:38:44.000000 collective.dms.basecontent-1.8/src/collective/dms/basecontent/profiles/default/portal_atct.xml
--rw-rw-r--   0 sge       (1000) sge       (1000)      791 2022-07-01 09:38:44.000000 collective.dms.basecontent-1.8/src/collective/dms/basecontent/profiles/default/propertiestool.xml
--rw-rw-r--   0 sge       (1000) sge       (1000)      359 2022-07-01 09:38:44.000000 collective.dms.basecontent-1.8/src/collective/dms/basecontent/profiles/default/rolemap.xml
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2022-07-01 09:38:44.343126 collective.dms.basecontent-1.8/src/collective/dms/basecontent/profiles/default/types/
--rw-rw-r--   0 sge       (1000) sge       (1000)     2182 2022-07-01 09:38:44.000000 collective.dms.basecontent-1.8/src/collective/dms/basecontent/profiles/default/types/dmsappendixfile.xml
--rw-rw-r--   0 sge       (1000) sge       (1000)     2371 2022-07-01 09:38:44.000000 collective.dms.basecontent-1.8/src/collective/dms/basecontent/profiles/default/types/dmsdocument.xml
--rw-rw-r--   0 sge       (1000) sge       (1000)     2129 2022-07-01 09:38:44.000000 collective.dms.basecontent-1.8/src/collective/dms/basecontent/profiles/default/types/dmsmainfile.xml
--rw-rw-r--   0 sge       (1000) sge       (1000)      349 2022-07-01 09:38:44.000000 collective.dms.basecontent-1.8/src/collective/dms/basecontent/profiles/default/types.xml
--rw-rw-r--   0 sge       (1000) sge       (1000)      295 2022-07-01 09:38:44.000000 collective.dms.basecontent-1.8/src/collective/dms/basecontent/profiles/default/workflows.xml
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2022-07-01 09:38:44.343126 collective.dms.basecontent-1.8/src/collective/dms/basecontent/profiles/testing/
--rw-rw-r--   0 sge       (1000) sge       (1000)       71 2022-07-01 09:38:44.000000 collective.dms.basecontent-1.8/src/collective/dms/basecontent/profiles/testing/metadata.xml
--rw-rw-r--   0 sge       (1000) sge       (1000)      873 2022-07-01 09:38:44.000000 collective.dms.basecontent-1.8/src/collective/dms/basecontent/related-docs-display.pt
--rw-rw-r--   0 sge       (1000) sge       (1000)     3106 2022-07-01 09:38:44.000000 collective.dms.basecontent-1.8/src/collective/dms/basecontent/relateddocs.py
--rw-rw-r--   0 sge       (1000) sge       (1000)      567 2022-07-01 09:38:44.000000 collective.dms.basecontent-1.8/src/collective/dms/basecontent/setuphandlers.py
--rw-rw-r--   0 sge       (1000) sge       (1000)     2344 2022-07-01 09:38:44.000000 collective.dms.basecontent-1.8/src/collective/dms/basecontent/source.py
--rw-rw-r--   0 sge       (1000) sge       (1000)      689 2022-07-01 09:38:44.000000 collective.dms.basecontent-1.8/src/collective/dms/basecontent/testing.py
--rw-rw-r--   0 sge       (1000) sge       (1000)      502 2022-07-01 09:38:44.000000 collective.dms.basecontent-1.8/src/collective/dms/basecontent/testing.zcml
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2022-07-01 09:38:44.343126 collective.dms.basecontent-1.8/src/collective/dms/basecontent/tests/
--rw-rw-r--   0 sge       (1000) sge       (1000)        0 2022-07-01 09:38:44.000000 collective.dms.basecontent-1.8/src/collective/dms/basecontent/tests/__init__.py
--rw-rw-r--   0 sge       (1000) sge       (1000)     1404 2022-07-01 09:38:44.000000 collective.dms.basecontent-1.8/src/collective/dms/basecontent/tests/test_dmsdocument.py
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2022-07-01 09:38:44.343126 collective.dms.basecontent-1.8/src/collective/dms/basecontent/upgrades/
--rw-rw-r--   0 sge       (1000) sge       (1000)        0 2022-07-01 09:38:44.000000 collective.dms.basecontent-1.8/src/collective/dms/basecontent/upgrades/__init__.py
--rw-rw-r--   0 sge       (1000) sge       (1000)      442 2022-07-01 09:38:44.000000 collective.dms.basecontent-1.8/src/collective/dms/basecontent/upgrades/configure.zcml
--rw-rw-r--   0 sge       (1000) sge       (1000)     1620 2022-07-01 09:38:44.000000 collective.dms.basecontent-1.8/src/collective/dms/basecontent/upgrades/upgrades.py
--rw-rw-r--   0 sge       (1000) sge       (1000)      389 2022-07-01 09:38:44.000000 collective.dms.basecontent-1.8/src/collective/dms/basecontent/widget.py
-drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2022-07-01 09:38:44.343126 collective.dms.basecontent-1.8/src/collective.dms.basecontent.egg-info/
--rw-rw-r--   0 sge       (1000) sge       (1000)     4922 2022-07-01 09:38:44.000000 collective.dms.basecontent-1.8/src/collective.dms.basecontent.egg-info/PKG-INFO
--rw-rw-r--   0 sge       (1000) sge       (1000)     4000 2022-07-01 09:38:44.000000 collective.dms.basecontent-1.8/src/collective.dms.basecontent.egg-info/SOURCES.txt
--rw-rw-r--   0 sge       (1000) sge       (1000)        1 2022-07-01 09:38:44.000000 collective.dms.basecontent-1.8/src/collective.dms.basecontent.egg-info/dependency_links.txt
--rw-rw-r--   0 sge       (1000) sge       (1000)       81 2022-07-01 09:38:44.000000 collective.dms.basecontent-1.8/src/collective.dms.basecontent.egg-info/entry_points.txt
--rw-rw-r--   0 sge       (1000) sge       (1000)       26 2022-07-01 09:38:44.000000 collective.dms.basecontent-1.8/src/collective.dms.basecontent.egg-info/namespace_packages.txt
--rw-rw-r--   0 sge       (1000) sge       (1000)        1 2022-07-01 09:38:44.000000 collective.dms.basecontent-1.8/src/collective.dms.basecontent.egg-info/not-zip-safe
--rw-rw-r--   0 sge       (1000) sge       (1000)      373 2022-07-01 09:38:44.000000 collective.dms.basecontent-1.8/src/collective.dms.basecontent.egg-info/requires.txt
--rw-rw-r--   0 sge       (1000) sge       (1000)       11 2022-07-01 09:38:44.000000 collective.dms.basecontent-1.8/src/collective.dms.basecontent.egg-info/top_level.txt
--rw-rw-r--   0 sge       (1000) sge       (1000)      145 2022-07-01 09:38:44.000000 collective.dms.basecontent-1.8/travis.cfg
--rw-rw-r--   0 sge       (1000) sge       (1000)      571 2022-07-01 09:38:44.000000 collective.dms.basecontent-1.8/versions.cfg
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2022-10-28 11:31:31.115691 collective.dms.basecontent-1.9/
+-rw-rw-r--   0 sge       (1000) sge       (1000)      173 2022-10-28 11:31:30.000000 collective.dms.basecontent-1.9/.gitignore
+-rw-rw-r--   0 sge       (1000) sge       (1000)      296 2022-10-28 11:31:30.000000 collective.dms.basecontent-1.9/.travis.yml
+-rw-rw-r--   0 sge       (1000) sge       (1000)     2938 2022-10-28 11:31:30.000000 collective.dms.basecontent-1.9/CHANGES.rst
+-rw-rw-r--   0 sge       (1000) sge       (1000)      138 2022-10-28 11:31:30.000000 collective.dms.basecontent-1.9/CONTRIBUTORS.rst
+-rw-rw-r--   0 sge       (1000) sge       (1000)       78 2022-10-28 11:31:30.000000 collective.dms.basecontent-1.9/MANIFEST.in
+-rw-rw-r--   0 sge       (1000) sge       (1000)     5073 2022-10-28 11:31:31.115691 collective.dms.basecontent-1.9/PKG-INFO
+-rw-rw-r--   0 sge       (1000) sge       (1000)     1032 2022-10-28 11:31:30.000000 collective.dms.basecontent-1.9/README.rst
+-rw-rw-r--   0 sge       (1000) sge       (1000)      275 2022-10-28 11:31:30.000000 collective.dms.basecontent-1.9/base.cfg
+-rw-rw-r--   0 sge       (1000) sge       (1000)     7458 2022-10-28 11:31:30.000000 collective.dms.basecontent-1.9/bootstrap.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)      141 2022-10-28 11:31:30.000000 collective.dms.basecontent-1.9/buildout.cfg
+-rw-rw-r--   0 sge       (1000) sge       (1000)      162 2022-10-28 11:31:30.000000 collective.dms.basecontent-1.9/checkouts.cfg
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2022-10-28 11:31:31.111691 collective.dms.basecontent-1.9/docs/
+-rw-rw-r--   0 sge       (1000) sge       (1000)    18092 2022-10-28 11:31:30.000000 collective.dms.basecontent-1.9/docs/LICENSE.GPL
+-rw-rw-r--   0 sge       (1000) sge       (1000)      738 2022-10-28 11:31:30.000000 collective.dms.basecontent-1.9/docs/LICENSE.txt
+-rw-rw-r--   0 sge       (1000) sge       (1000)      727 2022-10-28 11:31:30.000000 collective.dms.basecontent-1.9/jenkins-base.cfg
+-rw-rw-r--   0 sge       (1000) sge       (1000)       96 2022-10-28 11:31:30.000000 collective.dms.basecontent-1.9/jenkins.cfg
+-rw-rw-r--   0 sge       (1000) sge       (1000)       43 2022-10-28 11:31:30.000000 collective.dms.basecontent-1.9/requirements.txt
+-rw-rw-r--   0 sge       (1000) sge       (1000)       38 2022-10-28 11:31:31.115691 collective.dms.basecontent-1.9/setup.cfg
+-rw-rw-r--   0 sge       (1000) sge       (1000)     2378 2022-10-28 11:31:30.000000 collective.dms.basecontent-1.9/setup.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)      638 2022-10-28 11:31:30.000000 collective.dms.basecontent-1.9/sources.cfg
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2022-10-28 11:31:31.111691 collective.dms.basecontent-1.9/src/
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2022-10-28 11:31:31.111691 collective.dms.basecontent-1.9/src/collective/
+-rw-rw-r--   0 sge       (1000) sge       (1000)       56 2022-10-28 11:31:30.000000 collective.dms.basecontent-1.9/src/collective/__init__.py
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2022-10-28 11:31:31.111691 collective.dms.basecontent-1.9/src/collective/dms/
+-rw-rw-r--   0 sge       (1000) sge       (1000)       56 2022-10-28 11:31:30.000000 collective.dms.basecontent-1.9/src/collective/dms/__init__.py
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2022-10-28 11:31:31.111691 collective.dms.basecontent-1.9/src/collective/dms/basecontent/
+-rw-rw-r--   0 sge       (1000) sge       (1000)      183 2022-10-28 11:31:30.000000 collective.dms.basecontent-1.9/src/collective/dms/basecontent/__init__.py
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2022-10-28 11:31:31.111691 collective.dms.basecontent-1.9/src/collective/dms/basecontent/browser/
+-rw-rw-r--   0 sge       (1000) sge       (1000)        1 2022-10-28 11:31:30.000000 collective.dms.basecontent-1.9/src/collective/dms/basecontent/browser/__init__.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)     5093 2022-10-28 11:31:30.000000 collective.dms.basecontent-1.9/src/collective/dms/basecontent/browser/batch.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)     7086 2022-10-28 11:31:30.000000 collective.dms.basecontent-1.9/src/collective/dms/basecontent/browser/column.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)     1476 2022-10-28 11:31:30.000000 collective.dms.basecontent-1.9/src/collective/dms/basecontent/browser/configure.zcml
+-rw-rw-r--   0 sge       (1000) sge       (1000)     3109 2022-10-28 11:31:30.000000 collective.dms.basecontent-1.9/src/collective/dms/basecontent/browser/listing.py
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2022-10-28 11:31:31.111691 collective.dms.basecontent-1.9/src/collective/dms/basecontent/browser/static/
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2022-10-28 11:31:31.111691 collective.dms.basecontent-1.9/src/collective/dms/basecontent/browser/static/img/
+-rw-rw-r--   0 sge       (1000) sge       (1000)      334 2022-10-28 11:31:30.000000 collective.dms.basecontent-1.9/src/collective/dms/basecontent/browser/static/img/dmsappendixfile_icon.png
+-rw-rw-r--   0 sge       (1000) sge       (1000)      249 2022-10-28 11:31:30.000000 collective.dms.basecontent-1.9/src/collective/dms/basecontent/browser/static/img/dmsdocument_icon.png
+-rw-rw-r--   0 sge       (1000) sge       (1000)      675 2022-10-28 11:31:30.000000 collective.dms.basecontent-1.9/src/collective/dms/basecontent/browser/static/img/dmsmainfile_icon.png
+-rw-rw-r--   0 sge       (1000) sge       (1000)      330 2022-10-28 11:31:30.000000 collective.dms.basecontent-1.9/src/collective/dms/basecontent/browser/static/img/fade_edit.png
+-rw-rw-r--   0 sge       (1000) sge       (1000)     3308 2022-10-28 11:31:30.000000 collective.dms.basecontent-1.9/src/collective/dms/basecontent/browser/table.py
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2022-10-28 11:31:31.111691 collective.dms.basecontent-1.9/src/collective/dms/basecontent/browser/templates/
+-rw-rw-r--   0 sge       (1000) sge       (1000)     2845 2022-10-28 11:31:30.000000 collective.dms.basecontent-1.9/src/collective/dms/basecontent/browser/templates/dmsdocument_edit.pt
+-rw-rw-r--   0 sge       (1000) sge       (1000)     2701 2022-10-28 11:31:30.000000 collective.dms.basecontent-1.9/src/collective/dms/basecontent/browser/templates/dmsdocument_view.pt
+-rw-rw-r--   0 sge       (1000) sge       (1000)      241 2022-10-28 11:31:30.000000 collective.dms.basecontent-1.9/src/collective/dms/basecontent/browser/templates/filesviewlet.pt
+-rw-rw-r--   0 sge       (1000) sge       (1000)     2265 2022-10-28 11:31:30.000000 collective.dms.basecontent-1.9/src/collective/dms/basecontent/browser/templates/versionsviewlet.pt
+-rw-rw-r--   0 sge       (1000) sge       (1000)     1426 2022-10-28 11:31:30.000000 collective.dms.basecontent-1.9/src/collective/dms/basecontent/browser/templates/versionviewer.pt
+-rw-rw-r--   0 sge       (1000) sge       (1000)     2645 2022-10-28 11:31:30.000000 collective.dms.basecontent-1.9/src/collective/dms/basecontent/browser/viewlets.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)     1288 2022-10-28 11:31:30.000000 collective.dms.basecontent-1.9/src/collective/dms/basecontent/browser/views.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)     2198 2022-10-28 11:31:30.000000 collective.dms.basecontent-1.9/src/collective/dms/basecontent/configure.zcml
+-rw-rw-r--   0 sge       (1000) sge       (1000)     1741 2022-10-28 11:31:30.000000 collective.dms.basecontent-1.9/src/collective/dms/basecontent/dmsdocument.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)     2677 2022-10-28 11:31:30.000000 collective.dms.basecontent-1.9/src/collective/dms/basecontent/dmsfile.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)     1939 2022-10-28 11:31:30.000000 collective.dms.basecontent-1.9/src/collective/dms/basecontent/indexers.py
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2022-10-28 11:31:31.111691 collective.dms.basecontent-1.9/src/collective/dms/basecontent/locales/
+-rw-rw-r--   0 sge       (1000) sge       (1000)     1533 2022-10-28 11:31:30.000000 collective.dms.basecontent-1.9/src/collective/dms/basecontent/locales/collective.dms.basecontent.pot
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2022-10-28 11:31:31.111691 collective.dms.basecontent-1.9/src/collective/dms/basecontent/locales/en/
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2022-10-28 11:31:31.111691 collective.dms.basecontent-1.9/src/collective/dms/basecontent/locales/en/LC_MESSAGES/
+-rw-rw-r--   0 sge       (1000) sge       (1000)     1468 2022-10-28 11:31:30.000000 collective.dms.basecontent-1.9/src/collective/dms/basecontent/locales/en/LC_MESSAGES/collective.dms.basecontent.po
+-rw-rw-r--   0 sge       (1000) sge       (1000)     1230 2022-10-28 11:31:30.000000 collective.dms.basecontent-1.9/src/collective/dms/basecontent/locales/en/LC_MESSAGES/plone.po
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2022-10-28 11:31:31.111691 collective.dms.basecontent-1.9/src/collective/dms/basecontent/locales/fr/
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2022-10-28 11:31:31.111691 collective.dms.basecontent-1.9/src/collective/dms/basecontent/locales/fr/LC_MESSAGES/
+-rw-rw-r--   0 sge       (1000) sge       (1000)     1735 2022-10-28 11:31:30.000000 collective.dms.basecontent-1.9/src/collective/dms/basecontent/locales/fr/LC_MESSAGES/collective.dms.basecontent.po
+-rw-rw-r--   0 sge       (1000) sge       (1000)     1330 2022-10-28 11:31:30.000000 collective.dms.basecontent-1.9/src/collective/dms/basecontent/locales/fr/LC_MESSAGES/plone.po
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2022-10-28 11:31:31.111691 collective.dms.basecontent-1.9/src/collective/dms/basecontent/locales/nl/
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2022-10-28 11:31:31.111691 collective.dms.basecontent-1.9/src/collective/dms/basecontent/locales/nl/LC_MESSAGES/
+-rw-rw-r--   0 sge       (1000) sge       (1000)     1454 2022-10-28 11:31:30.000000 collective.dms.basecontent-1.9/src/collective/dms/basecontent/locales/nl/LC_MESSAGES/collective.dms.basecontent.po
+-rw-rw-r--   0 sge       (1000) sge       (1000)     1183 2022-10-28 11:31:30.000000 collective.dms.basecontent-1.9/src/collective/dms/basecontent/locales/nl/LC_MESSAGES/plone.po
+-rw-rw-r--   0 sge       (1000) sge       (1000)     1262 2022-10-28 11:31:30.000000 collective.dms.basecontent-1.9/src/collective/dms/basecontent/locales/plone.pot
+-rwxrwxr-x   0 sge       (1000) sge       (1000)      259 2022-10-28 11:31:30.000000 collective.dms.basecontent-1.9/src/collective/dms/basecontent/locales/update.sh
+-rw-rw-r--   0 sge       (1000) sge       (1000)      250 2022-10-28 11:31:30.000000 collective.dms.basecontent-1.9/src/collective/dms/basecontent/permissions.zcml
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2022-10-28 11:31:31.111691 collective.dms.basecontent-1.9/src/collective/dms/basecontent/profiles/
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2022-10-28 11:31:31.115691 collective.dms.basecontent-1.9/src/collective/dms/basecontent/profiles/default/
+-rw-rw-r--   0 sge       (1000) sge       (1000)      384 2022-10-28 11:31:30.000000 collective.dms.basecontent-1.9/src/collective/dms/basecontent/profiles/default/catalog.xml
+-rw-rw-r--   0 sge       (1000) sge       (1000)       14 2022-10-28 11:31:30.000000 collective.dms.basecontent-1.9/src/collective/dms/basecontent/profiles/default/collective_dms_basecontent_marker.txt
+-rw-rw-r--   0 sge       (1000) sge       (1000)      379 2022-10-28 11:31:30.000000 collective.dms.basecontent-1.9/src/collective/dms/basecontent/profiles/default/metadata.xml
+-rw-rw-r--   0 sge       (1000) sge       (1000)      482 2022-10-28 11:31:30.000000 collective.dms.basecontent-1.9/src/collective/dms/basecontent/profiles/default/portal_atct.xml
+-rw-rw-r--   0 sge       (1000) sge       (1000)      791 2022-10-28 11:31:30.000000 collective.dms.basecontent-1.9/src/collective/dms/basecontent/profiles/default/propertiestool.xml
+-rw-rw-r--   0 sge       (1000) sge       (1000)      359 2022-10-28 11:31:30.000000 collective.dms.basecontent-1.9/src/collective/dms/basecontent/profiles/default/rolemap.xml
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2022-10-28 11:31:31.115691 collective.dms.basecontent-1.9/src/collective/dms/basecontent/profiles/default/types/
+-rw-rw-r--   0 sge       (1000) sge       (1000)     2182 2022-10-28 11:31:30.000000 collective.dms.basecontent-1.9/src/collective/dms/basecontent/profiles/default/types/dmsappendixfile.xml
+-rw-rw-r--   0 sge       (1000) sge       (1000)     2371 2022-10-28 11:31:30.000000 collective.dms.basecontent-1.9/src/collective/dms/basecontent/profiles/default/types/dmsdocument.xml
+-rw-rw-r--   0 sge       (1000) sge       (1000)     2129 2022-10-28 11:31:30.000000 collective.dms.basecontent-1.9/src/collective/dms/basecontent/profiles/default/types/dmsmainfile.xml
+-rw-rw-r--   0 sge       (1000) sge       (1000)      349 2022-10-28 11:31:30.000000 collective.dms.basecontent-1.9/src/collective/dms/basecontent/profiles/default/types.xml
+-rw-rw-r--   0 sge       (1000) sge       (1000)      295 2022-10-28 11:31:30.000000 collective.dms.basecontent-1.9/src/collective/dms/basecontent/profiles/default/workflows.xml
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2022-10-28 11:31:31.115691 collective.dms.basecontent-1.9/src/collective/dms/basecontent/profiles/testing/
+-rw-rw-r--   0 sge       (1000) sge       (1000)      178 2022-10-28 11:31:30.000000 collective.dms.basecontent-1.9/src/collective/dms/basecontent/profiles/testing/metadata.xml
+-rw-rw-r--   0 sge       (1000) sge       (1000)      873 2022-10-28 11:31:30.000000 collective.dms.basecontent-1.9/src/collective/dms/basecontent/related-docs-display.pt
+-rw-rw-r--   0 sge       (1000) sge       (1000)     3106 2022-10-28 11:31:30.000000 collective.dms.basecontent-1.9/src/collective/dms/basecontent/relateddocs.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)      567 2022-10-28 11:31:30.000000 collective.dms.basecontent-1.9/src/collective/dms/basecontent/setuphandlers.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)     2344 2022-10-28 11:31:30.000000 collective.dms.basecontent-1.9/src/collective/dms/basecontent/source.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)      689 2022-10-28 11:31:30.000000 collective.dms.basecontent-1.9/src/collective/dms/basecontent/testing.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)      502 2022-10-28 11:31:30.000000 collective.dms.basecontent-1.9/src/collective/dms/basecontent/testing.zcml
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2022-10-28 11:31:31.115691 collective.dms.basecontent-1.9/src/collective/dms/basecontent/tests/
+-rw-rw-r--   0 sge       (1000) sge       (1000)        0 2022-10-28 11:31:30.000000 collective.dms.basecontent-1.9/src/collective/dms/basecontent/tests/__init__.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)     2284 2022-10-28 11:31:30.000000 collective.dms.basecontent-1.9/src/collective/dms/basecontent/tests/test_dmsdocument.py
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2022-10-28 11:31:31.115691 collective.dms.basecontent-1.9/src/collective/dms/basecontent/upgrades/
+-rw-rw-r--   0 sge       (1000) sge       (1000)        0 2022-10-28 11:31:30.000000 collective.dms.basecontent-1.9/src/collective/dms/basecontent/upgrades/__init__.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)      442 2022-10-28 11:31:30.000000 collective.dms.basecontent-1.9/src/collective/dms/basecontent/upgrades/configure.zcml
+-rw-rw-r--   0 sge       (1000) sge       (1000)     1620 2022-10-28 11:31:30.000000 collective.dms.basecontent-1.9/src/collective/dms/basecontent/upgrades/upgrades.py
+-rw-rw-r--   0 sge       (1000) sge       (1000)      389 2022-10-28 11:31:30.000000 collective.dms.basecontent-1.9/src/collective/dms/basecontent/widget.py
+drwxrwxr-x   0 sge       (1000) sge       (1000)        0 2022-10-28 11:31:31.111691 collective.dms.basecontent-1.9/src/collective.dms.basecontent.egg-info/
+-rw-rw-r--   0 sge       (1000) sge       (1000)     5073 2022-10-28 11:31:31.000000 collective.dms.basecontent-1.9/src/collective.dms.basecontent.egg-info/PKG-INFO
+-rw-rw-r--   0 sge       (1000) sge       (1000)     4017 2022-10-28 11:31:31.000000 collective.dms.basecontent-1.9/src/collective.dms.basecontent.egg-info/SOURCES.txt
+-rw-rw-r--   0 sge       (1000) sge       (1000)        1 2022-10-28 11:31:31.000000 collective.dms.basecontent-1.9/src/collective.dms.basecontent.egg-info/dependency_links.txt
+-rw-rw-r--   0 sge       (1000) sge       (1000)       81 2022-10-28 11:31:31.000000 collective.dms.basecontent-1.9/src/collective.dms.basecontent.egg-info/entry_points.txt
+-rw-rw-r--   0 sge       (1000) sge       (1000)       26 2022-10-28 11:31:31.000000 collective.dms.basecontent-1.9/src/collective.dms.basecontent.egg-info/namespace_packages.txt
+-rw-rw-r--   0 sge       (1000) sge       (1000)        1 2022-10-28 11:31:31.000000 collective.dms.basecontent-1.9/src/collective.dms.basecontent.egg-info/not-zip-safe
+-rw-rw-r--   0 sge       (1000) sge       (1000)      398 2022-10-28 11:31:31.000000 collective.dms.basecontent-1.9/src/collective.dms.basecontent.egg-info/requires.txt
+-rw-rw-r--   0 sge       (1000) sge       (1000)       11 2022-10-28 11:31:31.000000 collective.dms.basecontent-1.9/src/collective.dms.basecontent.egg-info/top_level.txt
+-rw-rw-r--   0 sge       (1000) sge       (1000)      145 2022-10-28 11:31:30.000000 collective.dms.basecontent-1.9/travis.cfg
+-rw-rw-r--   0 sge       (1000) sge       (1000)      681 2022-10-28 11:31:30.000000 collective.dms.basecontent-1.9/versions.cfg
```

### Comparing `collective.dms.basecontent-1.8/CHANGES.rst` & `collective.dms.basecontent-1.9/CHANGES.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,18 @@
 Changelog
 =========
 
+1.9 (2022-10-28)
+----------------
+
+- Made buildout running again.
+  [sgeulette]
+- Added `DmsDocument.get_mainfiles` to get dmsmainfiles
+  [sgeulette]
+
 1.8 (2022-07-01)
 ----------------
 
 - Corrected UnicodeEncodeError.
   [sgeulette]
 
 1.7 (2022-06-21)
```

### Comparing `collective.dms.basecontent-1.8/PKG-INFO` & `collective.dms.basecontent-1.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: collective.dms.basecontent
-Version: 1.8
+Version: 1.9
 Summary: Base content types for document management system
 Home-page: https://github.com/collective/collective.dms.basecontent
 Author: Ecreall, Entrouvert, IMIO
 Author-email: cedricmessiant@ecreall.com
 License: gpl
 Download-URL: https://pypi.org/project/collective.dms.basecontent
 Keywords: document management system dms viewer
@@ -62,14 +62,22 @@
 - Vincent Fretin, Ecreall
 - Cédric Messiant, Ecreall
 - Frédéric Peters, Entr'ouvert
 
 Changelog
 =========
 
+1.9 (2022-10-28)
+----------------
+
+- Made buildout running again.
+  [sgeulette]
+- Added `DmsDocument.get_mainfiles` to get dmsmainfiles
+  [sgeulette]
+
 1.8 (2022-07-01)
 ----------------
 
 - Corrected UnicodeEncodeError.
   [sgeulette]
 
 1.7 (2022-06-21)
```

### Comparing `collective.dms.basecontent-1.8/README.rst` & `collective.dms.basecontent-1.9/README.rst`

 * *Files identical despite different names*

### Comparing `collective.dms.basecontent-1.8/bootstrap.py` & `collective.dms.basecontent-1.9/bootstrap.py`

 * *Files identical despite different names*

### Comparing `collective.dms.basecontent-1.8/docs/LICENSE.GPL` & `collective.dms.basecontent-1.9/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `collective.dms.basecontent-1.8/docs/LICENSE.txt` & `collective.dms.basecontent-1.9/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `collective.dms.basecontent-1.8/jenkins-base.cfg` & `collective.dms.basecontent-1.9/jenkins-base.cfg`

 * *Files identical despite different names*

### Comparing `collective.dms.basecontent-1.8/setup.py` & `collective.dms.basecontent-1.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #! -*- coding: utf8 -*-
 from setuptools import setup, find_packages
 
-version = '1.8'
+version = '1.9'
 
 long_description = (
     open('README.rst').read()
     + '\n' +
     'Contributors\n'
     '============\n'
     + '\n' +
@@ -46,14 +46,16 @@
     zip_safe=False,
     install_requires=[
         'setuptools',
         'five.grok',
         'collective.documentviewer',
         'dexterity.localrolesfield',
         'future',
+        'imio.helpers>=0.42',
+        'pdbpp',
         'plone.api',
         'plone.app.dexterity',
         'plone.directives.form',
         'plone.namedfile',
         'z3c.blobfile',
         'plone.app.contenttypes',
         'plone.app.relationfield',
```

### Comparing `collective.dms.basecontent-1.8/sources.cfg` & `collective.dms.basecontent-1.9/sources.cfg`

 * *Files identical despite different names*

### Comparing `collective.dms.basecontent-1.8/src/collective/dms/basecontent/browser/batch.py` & `collective.dms.basecontent-1.9/src/collective/dms/basecontent/browser/batch.py`

 * *Files identical despite different names*

### Comparing `collective.dms.basecontent-1.8/src/collective/dms/basecontent/browser/column.py` & `collective.dms.basecontent-1.9/src/collective/dms/basecontent/browser/column.py`

 * *Files identical despite different names*

### Comparing `collective.dms.basecontent-1.8/src/collective/dms/basecontent/browser/configure.zcml` & `collective.dms.basecontent-1.9/src/collective/dms/basecontent/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `collective.dms.basecontent-1.8/src/collective/dms/basecontent/browser/listing.py` & `collective.dms.basecontent-1.9/src/collective/dms/basecontent/browser/listing.py`

 * *Files identical despite different names*

### Comparing `collective.dms.basecontent-1.8/src/collective/dms/basecontent/browser/static/img/dmsmainfile_icon.png` & `collective.dms.basecontent-1.9/src/collective/dms/basecontent/browser/static/img/dmsmainfile_icon.png`

 * *Files identical despite different names*

### Comparing `collective.dms.basecontent-1.8/src/collective/dms/basecontent/browser/table.py` & `collective.dms.basecontent-1.9/src/collective/dms/basecontent/browser/table.py`

 * *Files identical despite different names*

### Comparing `collective.dms.basecontent-1.8/src/collective/dms/basecontent/browser/templates/dmsdocument_edit.pt` & `collective.dms.basecontent-1.9/src/collective/dms/basecontent/browser/templates/dmsdocument_edit.pt`

 * *Files identical despite different names*

### Comparing `collective.dms.basecontent-1.8/src/collective/dms/basecontent/browser/templates/dmsdocument_view.pt` & `collective.dms.basecontent-1.9/src/collective/dms/basecontent/browser/templates/dmsdocument_view.pt`

 * *Files identical despite different names*

### Comparing `collective.dms.basecontent-1.8/src/collective/dms/basecontent/browser/templates/versionsviewlet.pt` & `collective.dms.basecontent-1.9/src/collective/dms/basecontent/browser/templates/versionsviewlet.pt`

 * *Files identical despite different names*

### Comparing `collective.dms.basecontent-1.8/src/collective/dms/basecontent/browser/templates/versionviewer.pt` & `collective.dms.basecontent-1.9/src/collective/dms/basecontent/browser/templates/versionviewer.pt`

 * *Files identical despite different names*

### Comparing `collective.dms.basecontent-1.8/src/collective/dms/basecontent/browser/viewlets.py` & `collective.dms.basecontent-1.9/src/collective/dms/basecontent/browser/viewlets.py`

 * *Files identical despite different names*

### Comparing `collective.dms.basecontent-1.8/src/collective/dms/basecontent/browser/views.py` & `collective.dms.basecontent-1.9/src/collective/dms/basecontent/browser/views.py`

 * *Files identical despite different names*

### Comparing `collective.dms.basecontent-1.8/src/collective/dms/basecontent/configure.zcml` & `collective.dms.basecontent-1.9/src/collective/dms/basecontent/configure.zcml`

 * *Files identical despite different names*

### Comparing `collective.dms.basecontent-1.8/src/collective/dms/basecontent/dmsdocument.py` & `collective.dms.basecontent-1.9/src/collective/dms/basecontent/dmsdocument.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from imio.helpers.content import object_values
 from zope import schema
 from zope.interface import implements
 from zope.schema.fieldproperty import FieldProperty
 
 from plone.autoform import directives as form
 from plone.dexterity.content import Container
 from plone.dexterity.schema import DexteritySchemaPolicy
@@ -45,13 +46,16 @@
 
 class DmsDocument(Container):
     """DmsDocument"""
     implements(IDmsDocument)
     # disable local roles inheritance
     __ac_local_roles_block__ = True
 
+    def get_mainfiles(self):
+        return object_values(self, ['DmsFile'])
+
 
 class DmsDocumentSchemaPolicy(DexteritySchemaPolicy):
     """DmsDocument schema policy"""
 
     def bases(self, schemaName, tree):
         return (IDmsDocument, )
```

### Comparing `collective.dms.basecontent-1.8/src/collective/dms/basecontent/dmsfile.py` & `collective.dms.basecontent-1.9/src/collective/dms/basecontent/dmsfile.py`

 * *Files identical despite different names*

### Comparing `collective.dms.basecontent-1.8/src/collective/dms/basecontent/indexers.py` & `collective.dms.basecontent-1.9/src/collective/dms/basecontent/indexers.py`

 * *Files identical despite different names*

### Comparing `collective.dms.basecontent-1.8/src/collective/dms/basecontent/locales/collective.dms.basecontent.pot` & `collective.dms.basecontent-1.9/src/collective/dms/basecontent/locales/collective.dms.basecontent.pot`

 * *Files identical despite different names*

### Comparing `collective.dms.basecontent-1.8/src/collective/dms/basecontent/locales/en/LC_MESSAGES/collective.dms.basecontent.po` & `collective.dms.basecontent-1.9/src/collective/dms/basecontent/locales/en/LC_MESSAGES/collective.dms.basecontent.po`

 * *Files identical despite different names*

### Comparing `collective.dms.basecontent-1.8/src/collective/dms/basecontent/locales/en/LC_MESSAGES/plone.po` & `collective.dms.basecontent-1.9/src/collective/dms/basecontent/locales/en/LC_MESSAGES/plone.po`

 * *Files identical despite different names*

### Comparing `collective.dms.basecontent-1.8/src/collective/dms/basecontent/locales/fr/LC_MESSAGES/collective.dms.basecontent.po` & `collective.dms.basecontent-1.9/src/collective/dms/basecontent/locales/fr/LC_MESSAGES/collective.dms.basecontent.po`

 * *Files identical despite different names*

### Comparing `collective.dms.basecontent-1.8/src/collective/dms/basecontent/locales/fr/LC_MESSAGES/plone.po` & `collective.dms.basecontent-1.9/src/collective/dms/basecontent/locales/fr/LC_MESSAGES/plone.po`

 * *Files identical despite different names*

### Comparing `collective.dms.basecontent-1.8/src/collective/dms/basecontent/locales/nl/LC_MESSAGES/collective.dms.basecontent.po` & `collective.dms.basecontent-1.9/src/collective/dms/basecontent/locales/nl/LC_MESSAGES/collective.dms.basecontent.po`

 * *Files identical despite different names*

### Comparing `collective.dms.basecontent-1.8/src/collective/dms/basecontent/locales/nl/LC_MESSAGES/plone.po` & `collective.dms.basecontent-1.9/src/collective/dms/basecontent/locales/nl/LC_MESSAGES/plone.po`

 * *Files identical despite different names*

### Comparing `collective.dms.basecontent-1.8/src/collective/dms/basecontent/locales/plone.pot` & `collective.dms.basecontent-1.9/src/collective/dms/basecontent/locales/plone.pot`

 * *Files identical despite different names*

### Comparing `collective.dms.basecontent-1.8/src/collective/dms/basecontent/profiles/default/propertiestool.xml` & `collective.dms.basecontent-1.9/src/collective/dms/basecontent/profiles/default/propertiestool.xml`

 * *Files identical despite different names*

### Comparing `collective.dms.basecontent-1.8/src/collective/dms/basecontent/profiles/default/types/dmsappendixfile.xml` & `collective.dms.basecontent-1.9/src/collective/dms/basecontent/profiles/default/types/dmsappendixfile.xml`

 * *Files identical despite different names*

### Comparing `collective.dms.basecontent-1.8/src/collective/dms/basecontent/profiles/default/types/dmsdocument.xml` & `collective.dms.basecontent-1.9/src/collective/dms/basecontent/profiles/default/types/dmsdocument.xml`

 * *Files identical despite different names*

### Comparing `collective.dms.basecontent-1.8/src/collective/dms/basecontent/profiles/default/types/dmsmainfile.xml` & `collective.dms.basecontent-1.9/src/collective/dms/basecontent/profiles/default/types/dmsmainfile.xml`

 * *Files identical despite different names*

### Comparing `collective.dms.basecontent-1.8/src/collective/dms/basecontent/related-docs-display.pt` & `collective.dms.basecontent-1.9/src/collective/dms/basecontent/related-docs-display.pt`

 * *Files identical despite different names*

### Comparing `collective.dms.basecontent-1.8/src/collective/dms/basecontent/relateddocs.py` & `collective.dms.basecontent-1.9/src/collective/dms/basecontent/relateddocs.py`

 * *Files identical despite different names*

### Comparing `collective.dms.basecontent-1.8/src/collective/dms/basecontent/setuphandlers.py` & `collective.dms.basecontent-1.9/src/collective/dms/basecontent/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `collective.dms.basecontent-1.8/src/collective/dms/basecontent/source.py` & `collective.dms.basecontent-1.9/src/collective/dms/basecontent/source.py`

 * *Files identical despite different names*

### Comparing `collective.dms.basecontent-1.8/src/collective/dms/basecontent/testing.py` & `collective.dms.basecontent-1.9/src/collective/dms/basecontent/testing.py`

 * *Files identical despite different names*

### Comparing `collective.dms.basecontent-1.8/src/collective/dms/basecontent/upgrades/upgrades.py` & `collective.dms.basecontent-1.9/src/collective/dms/basecontent/upgrades/upgrades.py`

 * *Files identical despite different names*

### Comparing `collective.dms.basecontent-1.8/src/collective.dms.basecontent.egg-info/PKG-INFO` & `collective.dms.basecontent-1.9/src/collective.dms.basecontent.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: collective.dms.basecontent
-Version: 1.8
+Version: 1.9
 Summary: Base content types for document management system
 Home-page: https://github.com/collective/collective.dms.basecontent
 Author: Ecreall, Entrouvert, IMIO
 Author-email: cedricmessiant@ecreall.com
 License: gpl
 Download-URL: https://pypi.org/project/collective.dms.basecontent
 Keywords: document management system dms viewer
@@ -62,14 +62,22 @@
 - Vincent Fretin, Ecreall
 - Cédric Messiant, Ecreall
 - Frédéric Peters, Entr'ouvert
 
 Changelog
 =========
 
+1.9 (2022-10-28)
+----------------
+
+- Made buildout running again.
+  [sgeulette]
+- Added `DmsDocument.get_mainfiles` to get dmsmainfiles
+  [sgeulette]
+
 1.8 (2022-07-01)
 ----------------
 
 - Corrected UnicodeEncodeError.
   [sgeulette]
 
 1.7 (2022-06-21)
```

### Comparing `collective.dms.basecontent-1.8/src/collective.dms.basecontent.egg-info/SOURCES.txt` & `collective.dms.basecontent-1.9/src/collective.dms.basecontent.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 README.rst
 base.cfg
 bootstrap.py
 buildout.cfg
 checkouts.cfg
 jenkins-base.cfg
 jenkins.cfg
+requirements.txt
 setup.py
 sources.cfg
 travis.cfg
 versions.cfg
 docs/LICENSE.GPL
 docs/LICENSE.txt
 src/collective/__init__.py
```

### Comparing `collective.dms.basecontent-1.8/versions.cfg` & `collective.dms.basecontent-1.9/versions.cfg`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 [versions]
-setuptools =
-zc.buildout =
+setuptools = 39.2.0
+zc.buildout = 2.13.3
 
-Products.DateRecurringIndex = 2.1
+#Products.DateRecurringIndex = 2.1
 collective.documentviewer = 3.0.3
 collective.elephantvocabulary = 0.2.5
 collective.js.chosen = 1.4
-collective.z3cform.chosen = 1.2.1
-collective.z3cform.datagridfield = 1.3.1
+collective.fingerpointing = 1.8.2
+collective.z3cform.chosen = 1.2.2
+collective.z3cform.datagridfield = 1.3.3
 demjson = 2.2.4
 ecreall.helpers.testing = 1.7
-icalendar = 3.11.4
-ipdb = 0.10.3
-ipython = 5.3.0
-future = 0.16.0
-plone.app.contenttypes = 1.1.1
-plone.event = 1.3.3
-plone.formwidget.datetime = 1.3
-plone.formwidget.querystring = 1.1.9
+icalendar = 4.0.3
+ipdb = 0.13.9
+ipython = 5.10.0
+future = 0.18.2
+#plone.app.contenttypes = 1.1.1
+plone.event = 1.4.0
+plone.formwidget.datetime = 1.3.5
+#plone.formwidget.querystring = 1.1.9
 plone.principalsource = 1.0
 repoze.catalog = 0.8.3
-z3c.table = 2.0.1
 z3c.unconfigure = 1.0.1
+# needed to upgrade from zope toolkit for fingerpointing
+zc.lockfile = 1.4
```

