# Comparing `tmp/ebau-gwr-0.6.1.tar.gz` & `tmp/ebau_gwr-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ebau-gwr-0.6.1.tar", max compression
+gzip compressed data, was "ebau_gwr-0.6.2.tar", max compression
```

## Comparing `ebau-gwr-0.6.1.tar` & `ebau_gwr-0.6.2.tar`

### file list

```diff
@@ -1,43 +1,42 @@
--rw-r--r--   0        0        0     4255 2022-09-21 08:50:59.765143 ebau-gwr-0.6.1/CHANGELOG.md
--rw-r--r--   0        0        0    35149 2022-09-21 08:50:59.765143 ebau-gwr-0.6.1/LICENSE
--rw-r--r--   0        0        0     2948 2022-09-21 08:50:59.765143 ebau-gwr-0.6.1/README.md
--rw-r--r--   0        0        0        0 2022-09-21 08:50:59.765143 ebau-gwr-0.6.1/ebau_gwr/__init__.py
--rw-r--r--   0        0        0        0 2022-09-21 08:50:59.765143 ebau-gwr-0.6.1/ebau_gwr/linker/__init__.py
--rw-r--r--   0        0        0       96 2022-09-21 08:50:59.765143 ebau-gwr-0.6.1/ebau_gwr/linker/apps.py
--rw-r--r--   0        0        0      927 2022-09-21 08:50:59.765143 ebau-gwr-0.6.1/ebau_gwr/linker/conftest.py
--rw-r--r--   0        0        0      259 2022-09-21 08:50:59.765143 ebau-gwr-0.6.1/ebau_gwr/linker/factories.py
--rw-r--r--   0        0        0     2459 2022-09-21 08:50:59.765143 ebau-gwr-0.6.1/ebau_gwr/linker/filters.py
--rw-r--r--   0        0        0     1039 2022-09-21 08:50:59.765143 ebau-gwr-0.6.1/ebau_gwr/linker/migrations/0001_initial.py
--rw-r--r--   0        0        0      299 2022-09-21 08:50:59.765143 ebau-gwr-0.6.1/ebau_gwr/linker/migrations/0002_set_default_ordering.py
--rw-r--r--   0        0        0      363 2022-09-21 08:50:59.765143 ebau-gwr-0.6.1/ebau_gwr/linker/migrations/0003_deprecated_json_field.py
--rw-r--r--   0        0        0        0 2022-09-21 08:50:59.765143 ebau-gwr-0.6.1/ebau_gwr/linker/migrations/__init__.py
--rw-r--r--   0        0        0      757 2022-09-21 08:50:59.765143 ebau-gwr-0.6.1/ebau_gwr/linker/models.py
--rw-r--r--   0        0        0      289 2022-09-21 08:50:59.765143 ebau-gwr-0.6.1/ebau_gwr/linker/serializers.py
--rw-r--r--   0        0        0      179 2022-09-21 08:50:59.765143 ebau-gwr-0.6.1/ebau_gwr/linker/urls.py
--rw-r--r--   0        0        0      652 2022-09-21 08:50:59.765143 ebau-gwr-0.6.1/ebau_gwr/linker/views.py
--rw-r--r--   0        0        0        0 2022-09-21 08:50:59.765143 ebau-gwr-0.6.1/ebau_gwr/oidc_auth/__init__.py
--rw-r--r--   0        0        0     2895 2022-09-21 08:50:59.765143 ebau-gwr-0.6.1/ebau_gwr/oidc_auth/authentication.py
--rw-r--r--   0        0        0     1021 2022-09-21 08:50:59.765143 ebau-gwr-0.6.1/ebau_gwr/oidc_auth/models.py
--rw-r--r--   0        0        0     6177 2022-09-21 08:50:59.765143 ebau-gwr-0.6.1/ebau_gwr/settings.py
--rw-r--r--   0        0        0        0 2022-09-21 08:50:59.765143 ebau-gwr-0.6.1/ebau_gwr/token_proxy/__init__.py
--rw-r--r--   0        0        0      296 2022-09-21 08:50:59.765143 ebau-gwr-0.6.1/ebau_gwr/token_proxy/app_settings.py
--rw-r--r--   0        0        0      784 2022-09-21 08:50:59.769143 ebau-gwr-0.6.1/ebau_gwr/token_proxy/apps.py
--rw-r--r--   0        0        0     1012 2022-09-21 08:50:59.769143 ebau-gwr-0.6.1/ebau_gwr/token_proxy/client.py
--rw-r--r--   0        0        0      363 2022-09-21 08:50:59.769143 ebau-gwr-0.6.1/ebau_gwr/token_proxy/factories.py
--rw-r--r--   0        0        0        0 2022-09-21 08:50:59.769143 ebau-gwr-0.6.1/ebau_gwr/token_proxy/management/__init__.py
--rw-r--r--   0        0        0        0 2022-09-21 08:50:59.769143 ebau-gwr-0.6.1/ebau_gwr/token_proxy/management/commands/__init__.py
--rw-r--r--   0        0        0      298 2022-09-21 08:50:59.769143 ebau-gwr-0.6.1/ebau_gwr/token_proxy/management/commands/generate_fernet_key.py
--rw-r--r--   0        0        0      874 2022-09-21 08:50:59.769143 ebau-gwr-0.6.1/ebau_gwr/token_proxy/migrations/0001_initial.py
--rw-r--r--   0        0        0      432 2022-09-21 08:50:59.769143 ebau-gwr-0.6.1/ebau_gwr/token_proxy/migrations/0002_housingstatcreds_municipality.py
--rw-r--r--   0        0        0      658 2022-09-21 08:50:59.769143 ebau-gwr-0.6.1/ebau_gwr/token_proxy/migrations/0003_housingstatcreds_group.py
--rw-r--r--   0        0        0      405 2022-09-21 08:50:59.769143 ebau-gwr-0.6.1/ebau_gwr/token_proxy/migrations/0004_alter_housingstatcreds_owner.py
--rw-r--r--   0        0        0        0 2022-09-21 08:50:59.769143 ebau-gwr-0.6.1/ebau_gwr/token_proxy/migrations/__init__.py
--rw-r--r--   0        0        0     1100 2022-09-21 08:50:59.769143 ebau-gwr-0.6.1/ebau_gwr/token_proxy/models.py
--rw-r--r--   0        0        0     2726 2022-09-21 08:50:59.769143 ebau-gwr-0.6.1/ebau_gwr/token_proxy/serializers.py
--rw-r--r--   0        0        0      217 2022-09-21 08:50:59.769143 ebau-gwr-0.6.1/ebau_gwr/token_proxy/urls.py
--rw-r--r--   0        0        0      990 2022-09-21 08:50:59.769143 ebau-gwr-0.6.1/ebau_gwr/token_proxy/views.py
--rw-r--r--   0        0        0      205 2022-09-21 08:50:59.769143 ebau-gwr-0.6.1/ebau_gwr/urls.py
--rw-r--r--   0        0        0      398 2022-09-21 08:50:59.769143 ebau-gwr-0.6.1/ebau_gwr/wsgi.py
--rw-r--r--   0        0        0     3000 2022-09-21 08:50:59.769143 ebau-gwr-0.6.1/pyproject.toml
--rw-r--r--   0        0        0     4231 1970-01-01 00:00:00.000000 ebau-gwr-0.6.1/setup.py
--rw-r--r--   0        0        0     4462 1970-01-01 00:00:00.000000 ebau-gwr-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0     4291 2023-05-12 18:42:56.542833 ebau_gwr-0.6.2/CHANGELOG.md
+-rw-r--r--   0        0        0    35149 2023-05-12 18:42:56.542833 ebau_gwr-0.6.2/LICENSE
+-rw-r--r--   0        0        0     2911 2023-05-12 18:42:56.542833 ebau_gwr-0.6.2/README.md
+-rw-r--r--   0        0        0        0 2023-05-12 18:42:56.542833 ebau_gwr-0.6.2/ebau_gwr/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-12 18:42:56.542833 ebau_gwr-0.6.2/ebau_gwr/linker/__init__.py
+-rw-r--r--   0        0        0       96 2023-05-12 18:42:56.542833 ebau_gwr-0.6.2/ebau_gwr/linker/apps.py
+-rw-r--r--   0        0        0      927 2023-05-12 18:42:56.542833 ebau_gwr-0.6.2/ebau_gwr/linker/conftest.py
+-rw-r--r--   0        0        0      259 2023-05-12 18:42:56.542833 ebau_gwr-0.6.2/ebau_gwr/linker/factories.py
+-rw-r--r--   0        0        0     2459 2023-05-12 18:42:56.542833 ebau_gwr-0.6.2/ebau_gwr/linker/filters.py
+-rw-r--r--   0        0        0     1038 2023-05-12 18:42:56.542833 ebau_gwr-0.6.2/ebau_gwr/linker/migrations/0001_initial.py
+-rw-r--r--   0        0        0      298 2023-05-12 18:42:56.542833 ebau_gwr-0.6.2/ebau_gwr/linker/migrations/0002_set_default_ordering.py
+-rw-r--r--   0        0        0      362 2023-05-12 18:42:56.542833 ebau_gwr-0.6.2/ebau_gwr/linker/migrations/0003_deprecated_json_field.py
+-rw-r--r--   0        0        0        0 2023-05-12 18:42:56.542833 ebau_gwr-0.6.2/ebau_gwr/linker/migrations/__init__.py
+-rw-r--r--   0        0        0      757 2023-05-12 18:42:56.542833 ebau_gwr-0.6.2/ebau_gwr/linker/models.py
+-rw-r--r--   0        0        0      289 2023-05-12 18:42:56.542833 ebau_gwr-0.6.2/ebau_gwr/linker/serializers.py
+-rw-r--r--   0        0        0      179 2023-05-12 18:42:56.542833 ebau_gwr-0.6.2/ebau_gwr/linker/urls.py
+-rw-r--r--   0        0        0      652 2023-05-12 18:42:56.542833 ebau_gwr-0.6.2/ebau_gwr/linker/views.py
+-rw-r--r--   0        0        0        0 2023-05-12 18:42:56.546833 ebau_gwr-0.6.2/ebau_gwr/oidc_auth/__init__.py
+-rw-r--r--   0        0        0     2895 2023-05-12 18:42:56.546833 ebau_gwr-0.6.2/ebau_gwr/oidc_auth/authentication.py
+-rw-r--r--   0        0        0     1021 2023-05-12 18:42:56.546833 ebau_gwr-0.6.2/ebau_gwr/oidc_auth/models.py
+-rw-r--r--   0        0        0     6177 2023-05-12 18:42:56.546833 ebau_gwr-0.6.2/ebau_gwr/settings.py
+-rw-r--r--   0        0        0        0 2023-05-12 18:42:56.546833 ebau_gwr-0.6.2/ebau_gwr/token_proxy/__init__.py
+-rw-r--r--   0        0        0      296 2023-05-12 18:42:56.546833 ebau_gwr-0.6.2/ebau_gwr/token_proxy/app_settings.py
+-rw-r--r--   0        0        0      784 2023-05-12 18:42:56.546833 ebau_gwr-0.6.2/ebau_gwr/token_proxy/apps.py
+-rw-r--r--   0        0        0     1012 2023-05-12 18:42:56.546833 ebau_gwr-0.6.2/ebau_gwr/token_proxy/client.py
+-rw-r--r--   0        0        0      363 2023-05-12 18:42:56.546833 ebau_gwr-0.6.2/ebau_gwr/token_proxy/factories.py
+-rw-r--r--   0        0        0        0 2023-05-12 18:42:56.546833 ebau_gwr-0.6.2/ebau_gwr/token_proxy/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-12 18:42:56.546833 ebau_gwr-0.6.2/ebau_gwr/token_proxy/management/commands/__init__.py
+-rw-r--r--   0        0        0      298 2023-05-12 18:42:56.546833 ebau_gwr-0.6.2/ebau_gwr/token_proxy/management/commands/generate_fernet_key.py
+-rw-r--r--   0        0        0      873 2023-05-12 18:42:56.546833 ebau_gwr-0.6.2/ebau_gwr/token_proxy/migrations/0001_initial.py
+-rw-r--r--   0        0        0      431 2023-05-12 18:42:56.546833 ebau_gwr-0.6.2/ebau_gwr/token_proxy/migrations/0002_housingstatcreds_municipality.py
+-rw-r--r--   0        0        0      657 2023-05-12 18:42:56.546833 ebau_gwr-0.6.2/ebau_gwr/token_proxy/migrations/0003_housingstatcreds_group.py
+-rw-r--r--   0        0        0      404 2023-05-12 18:42:56.546833 ebau_gwr-0.6.2/ebau_gwr/token_proxy/migrations/0004_alter_housingstatcreds_owner.py
+-rw-r--r--   0        0        0        0 2023-05-12 18:42:56.546833 ebau_gwr-0.6.2/ebau_gwr/token_proxy/migrations/__init__.py
+-rw-r--r--   0        0        0     1100 2023-05-12 18:42:56.546833 ebau_gwr-0.6.2/ebau_gwr/token_proxy/models.py
+-rw-r--r--   0        0        0     2726 2023-05-12 18:42:56.546833 ebau_gwr-0.6.2/ebau_gwr/token_proxy/serializers.py
+-rw-r--r--   0        0        0      217 2023-05-12 18:42:56.546833 ebau_gwr-0.6.2/ebau_gwr/token_proxy/urls.py
+-rw-r--r--   0        0        0      990 2023-05-12 18:42:56.546833 ebau_gwr-0.6.2/ebau_gwr/token_proxy/views.py
+-rw-r--r--   0        0        0      205 2023-05-12 18:42:56.546833 ebau_gwr-0.6.2/ebau_gwr/urls.py
+-rw-r--r--   0        0        0      398 2023-05-12 18:42:56.546833 ebau_gwr-0.6.2/ebau_gwr/wsgi.py
+-rw-r--r--   0        0        0     2986 2023-05-12 18:42:56.546833 ebau_gwr-0.6.2/pyproject.toml
+-rw-r--r--   0        0        0     4413 1970-01-01 00:00:00.000000 ebau_gwr-0.6.2/PKG-INFO
```

### Comparing `ebau-gwr-0.6.1/CHANGELOG.md` & `ebau_gwr-0.6.2/CHANGELOG.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,66 +1,71 @@
 # Changelog
 
+## v0.6.2 (2023-05-12)
+
+### Fix
+* **deps:** Update dependencies ([`e259b36`](https://github.com/inosca/ebau-gwr/commit/e259b362e87931d2258767c716ee4638eb3be351))
+
 ## v0.6.1 (2022-09-21)
 
 ### Fix
-* **linker:** Allow "in" lookup for gwr-link eproid filter ([`bcaa1d1`](https://github.com/luytena/ebau-gwr/commit/bcaa1d1b58c285019db2bff466c23c2902a6e41d))
+* **linker:** Allow "in" lookup for gwr-link eproid filter ([`bcaa1d1`](https://github.com/inosca/ebau-gwr/commit/bcaa1d1b58c285019db2bff466c23c2902a6e41d))
 
 ## v0.6.0 (2022-09-02)
 
 ### Feature
-* **hous_stat_creds:** Creds are identified by user and x-camac-group ([`7894081`](https://github.com/adfinis-sygroup/ebau-gwr/commit/789408155bcf92450efac7bf90a42dfe4bf070f2))
+* **hous_stat_creds:** Creds are identified by user and x-camac-group ([`7894081`](https://github.com/inosca/ebau-gwr/commit/789408155bcf92450efac7bf90a42dfe4bf070f2))
 
 ### Fix
-* **docker:** Run server with poetry so deps are found ([`cbbbd71`](https://github.com/adfinis-sygroup/ebau-gwr/commit/cbbbd717f670ee9b2ee6ec3af86704bc340ad670))
+* **docker:** Run server with poetry so deps are found ([`cbbbd71`](https://github.com/inosca/ebau-gwr/commit/cbbbd717f670ee9b2ee6ec3af86704bc340ad670))
 
 ## v0.5.2 (2022-06-20)
 
 ### Fix
-* **deps:** Update dependencies ([`be92236`](https://github.com/adfinis-sygroup/ebau-gwr/commit/be92236798245053c44d51cac5ec454f1d2be9fb))
+* **deps:** Update dependencies ([`be92236`](https://github.com/inosca/ebau-gwr/commit/be92236798245053c44d51cac5ec454f1d2be9fb))
 
 ## v0.5.1 (2022-04-21)
 
 ### Fix
-* **deps:** Update dependencies ([`fc7415e`](https://github.com/adfinis-sygroup/ebau-gwr/commit/fc7415e1e1db9445652d3da22d9fe4cb9a03fa20))
+* **deps:** Update dependencies ([`fc7415e`](https://github.com/inosca/ebau-gwr/commit/fc7415e1e1db9445652d3da22d9fe4cb9a03fa20))
 
 ## v0.5.0 (2022-03-03)
 
 ### Breaking
-* This commit updates django to version 3.2 which is a new major version. If this package is consumed as django app, the host app needs to update django as well: ([`4adaec2`](https://github.com/adfinis-sygroup/ebau-gwr/commit/4adaec29c7475b99f411d81de2947f8b9a2c0794))
+* This commit updates django to version 3.2 which is a new major version. If this package is consumed as django app, the host app needs to update django as well: ([`4adaec2`](https://github.com/inosca/ebau-gwr/commit/4adaec29c7475b99f411d81de2947f8b9a2c0794))
 
 ### Documentation
-* **readme:** Fix build status badge ([`66d222a`](https://github.com/adfinis-sygroup/ebau-gwr/commit/66d222acf85df447f5fd1af3c102751a3b5f62ec))
+* **readme:** Fix build status badge ([`66d222a`](https://github.com/inosca/ebau-gwr/commit/66d222acf85df447f5fd1af3c102751a3b5f62ec))
 
 ## v0.4.1 (2021-10-27)
 
 ### Fix
-* Gwr base uri config settings ([`9f215b9`](https://github.com/adfinis-sygroup/ebau-gwr/commit/9f215b96dd087524548d60cd65f5b2fa17530ed3))
-* License identifier ([`c01f050`](https://github.com/adfinis-sygroup/ebau-gwr/commit/c01f0509a2dd16ea3a34eef5dd9dc3625f99a8f4))
+* Gwr base uri config settings ([`9f215b9`](https://github.com/inosca/ebau-gwr/commit/9f215b96dd087524548d60cd65f5b2fa17530ed3))
+* License identifier ([`c01f050`](https://github.com/inosca/ebau-gwr/commit/c01f0509a2dd16ea3a34eef5dd9dc3625f99a8f4))
 
 ## v0.4.0 (2021-07-08)
 
 ### Feature
-* Allow removal of housing stat credentials ([`20c1f09`](https://github.com/adfinis-sygroup/ebau-gwr/commit/20c1f09e0d9871236cd6950b89e55e10fb0bfe2c))
+* Allow removal of housing stat credentials ([`20c1f09`](https://github.com/inosca/ebau-gwr/commit/20c1f09e0d9871236cd6950b89e55e10fb0bfe2c))
 # v0.3.0 (2021-05-06)
 
 ### Feature
-* **token_proxy:** Add municipality as a field ([`a08e989`](https://github.com/adfinis-sygroup/ebau-gwr/commit/a08e989864063e17803dc2a17da2ce6b58aa1040))
+* **token_proxy:** Add municipality as a field ([`a08e989`](https://github.com/inosca/ebau-gwr/commit/a08e989864063e17803dc2a17da2ce6b58aa1040))
 
 ## v0.2.0 (2021-04-14)
 
 ### Feature
-* Introduce command to generate fernet key ([`949ef82`](https://github.com/adfinis-sygroup/ebau-gwr/commit/949ef82fe407680b2e961d1564aba5ac956ab50b))
-* Introduce token_proxy app ([`65f4323`](https://github.com/adfinis-sygroup/ebau-gwr/commit/65f43238b5a27cc55d7b087565b179a53aa4f2c4))
+* Introduce command to generate fernet key ([`949ef82`](https://github.com/inosca/ebau-gwr/commit/949ef82fe407680b2e961d1564aba5ac956ab50b))
+* Introduce token_proxy app ([`65f4323`](https://github.com/inosca/ebau-gwr/commit/65f43238b5a27cc55d7b087565b179a53aa4f2c4))
 
 ### Fix
-* Define default ordering on GWRLink model ([`4a1fae3`](https://github.com/adfinis-sygroup/ebau-gwr/commit/4a1fae352ce4d3a269e111ddeb43a0d055926d89))
+* Define default ordering on GWRLink model ([`4a1fae3`](https://github.com/inosca/ebau-gwr/commit/4a1fae352ce4d3a269e111ddeb43a0d055926d89))
 
 ### Documentation
-* **readme:** Document correct env var name for wsk_id ([`39140c9`](https://github.com/adfinis-sygroup/ebau-gwr/commit/39140c97feb94cd8bcdff053b82c6d0e2790386c))
+* **readme:** Document correct env var name for wsk_id ([`39140c9`](https://github.com/inosca/ebau-gwr/commit/39140c97feb94cd8bcdff053b82c6d0e2790386c))
 
 ## v0.1.0 (2021-02-22)
 
 ### Feature
 * Integrate django-generic-api-permissions ([`eea32d9`](https://github.com/czosel/ebau-gwr/commit/eea32d9b74416fa75d4a9e667993162b110bba1a))
 * **linker:** Introduce linker app ([`94afc2a`](https://github.com/czosel/ebau-gwr/commit/94afc2a1dd11c99f7a73bac0e03327a16637d088))
 * Introduce /construction_project retrieve view ([`7dc0de9`](https://github.com/czosel/ebau-gwr/commit/7dc0de97cc910e3e98e73fbc3bfe40a11e73a646))
```

### Comparing `ebau-gwr-0.6.1/LICENSE` & `ebau_gwr-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ebau-gwr-0.6.1/README.md` & `ebau_gwr-0.6.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # ebau-gwr
 
-[![Build Status](https://github.com/adfinis-sygroup/ebau-gwr/workflows/Tests/badge.svg)](https://github.com/adfinis-sygroup/ebau-gwr/actions?query=workflow%3ATests)
-[![Coverage](https://img.shields.io/badge/coverage-100%25-brightgreen.svg)](https://github.com/adfinis-sygroup/ebau-gwr/blob/main/pyproject.toml#L99)
-[![Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/adfinis-sygroup/ebau-gwr)
+[![Build Status](https://github.com/inosca/ebau-gwr/workflows/Tests/badge.svg)](https://github.com/inosca/ebau-gwr/actions?query=workflow%3ATests)
+[![Coverage](https://img.shields.io/badge/coverage-100%25-brightgreen.svg)](https://github.com/inosca/ebau-gwr/blob/main/pyproject.toml#L99)
+[![Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/inosca/ebau-gwr)
 
 GWR synchronisation for ebau projects
 
 ## Getting started
 
 ### Installation
 
 **Requirements**
 
 - docker
 - docker-compose
 
-After installing and configuring those, download [docker-compose.yml](https://raw.githubusercontent.com/adfinis/ebau-gwr/main/docker-compose.yml) and run the following command:
+After installing and configuring those, download [docker-compose.yml](https://raw.githubusercontent.com/inosca/ebau-gwr/main/docker-compose.yml) and run the following command:
 
 ```bash
 docker-compose up -d
 ```
 
 You can now access the api at [http://localhost:8000/api/v1/](http://localhost:8000/api/v1/).
```

### Comparing `ebau-gwr-0.6.1/ebau_gwr/linker/conftest.py` & `ebau_gwr-0.6.2/ebau_gwr/linker/conftest.py`

 * *Files identical despite different names*

### Comparing `ebau-gwr-0.6.1/ebau_gwr/linker/filters.py` & `ebau_gwr-0.6.2/ebau_gwr/linker/filters.py`

 * *Files identical despite different names*

### Comparing `ebau-gwr-0.6.1/ebau_gwr/linker/migrations/0001_initial.py` & `ebau_gwr-0.6.2/ebau_gwr/linker/migrations/0001_initial.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 import django.contrib.postgres.fields.jsonb
 from django.db import migrations, models
 
 import ebau_gwr.linker.models
 
 
 class Migration(migrations.Migration):
-
     initial = True
 
     dependencies = []
 
     operations = [
         migrations.CreateModel(
             name="GWRLink",
```

### Comparing `ebau-gwr-0.6.1/ebau_gwr/linker/models.py` & `ebau_gwr-0.6.2/ebau_gwr/linker/models.py`

 * *Files identical despite different names*

### Comparing `ebau-gwr-0.6.1/ebau_gwr/linker/views.py` & `ebau_gwr-0.6.2/ebau_gwr/linker/views.py`

 * *Files identical despite different names*

### Comparing `ebau-gwr-0.6.1/ebau_gwr/oidc_auth/authentication.py` & `ebau_gwr-0.6.2/ebau_gwr/oidc_auth/authentication.py`

 * *Files identical despite different names*

### Comparing `ebau-gwr-0.6.1/ebau_gwr/oidc_auth/models.py` & `ebau_gwr-0.6.2/ebau_gwr/oidc_auth/models.py`

 * *Files identical despite different names*

### Comparing `ebau-gwr-0.6.1/ebau_gwr/settings.py` & `ebau_gwr-0.6.2/ebau_gwr/settings.py`

 * *Files identical despite different names*

### Comparing `ebau-gwr-0.6.1/ebau_gwr/token_proxy/apps.py` & `ebau_gwr-0.6.2/ebau_gwr/token_proxy/apps.py`

 * *Files identical despite different names*

### Comparing `ebau-gwr-0.6.1/ebau_gwr/token_proxy/client.py` & `ebau_gwr-0.6.2/ebau_gwr/token_proxy/client.py`

 * *Files identical despite different names*

### Comparing `ebau-gwr-0.6.1/ebau_gwr/token_proxy/migrations/0001_initial.py` & `ebau_gwr-0.6.2/ebau_gwr/token_proxy/migrations/0001_initial.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 
 from django.db import migrations, models
 
 import ebau_gwr.token_proxy.models
 
 
 class Migration(migrations.Migration):
-
     initial = True
 
     dependencies = []
 
     operations = [
         migrations.CreateModel(
             name="HousingStatCreds",
```

### Comparing `ebau-gwr-0.6.1/ebau_gwr/token_proxy/migrations/0003_housingstatcreds_group.py` & `ebau_gwr-0.6.2/ebau_gwr/token_proxy/migrations/0003_housingstatcreds_group.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 
 def delete_credentials(apps, schema_editor):
     HousingStatCreds = apps.get_model("token_proxy", "HousingStatCreds")
     HousingStatCreds.objects.all().delete()
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
         ("token_proxy", "0002_housingstatcreds_municipality"),
     ]
 
     operations = [
         migrations.RunPython(delete_credentials),
         migrations.AddField(
```

### Comparing `ebau-gwr-0.6.1/ebau_gwr/token_proxy/models.py` & `ebau_gwr-0.6.2/ebau_gwr/token_proxy/models.py`

 * *Files identical despite different names*

### Comparing `ebau-gwr-0.6.1/ebau_gwr/token_proxy/serializers.py` & `ebau_gwr-0.6.2/ebau_gwr/token_proxy/serializers.py`

 * *Files identical despite different names*

### Comparing `ebau-gwr-0.6.1/ebau_gwr/token_proxy/views.py` & `ebau_gwr-0.6.2/ebau_gwr/token_proxy/views.py`

 * *Files identical despite different names*

### Comparing `ebau-gwr-0.6.1/pyproject.toml` & `ebau_gwr-0.6.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "ebau-gwr"
-version = "0.6.1"
+version = "0.6.2"
 description = "GWR synchronisation for ebau projects"
-homepage = "https://github.com/adfinis-sygroup/ebau-gwr"
-repository = "https://github.com/adfinis-sygroup/ebau-gwr"
+homepage = "https://github.com/inosca/ebau-gwr"
+repository = "https://github.com/inosca/ebau-gwr"
 authors = ["Adfinis AG"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
     "Operating System :: OS Independent",
@@ -19,55 +19,55 @@
 include = ["CHANGELOG.md"]
 exclude = [
     "ebau_gwr/conftest.py",
     "ebau_gwr/**/tests",
 ]
 
 [tool.poetry.dependencies]
-python = "^3.8"
-cryptography = ">=37.0.2,<39.0.0"
+python = "^3.8.1"
+cryptography = ">=37.0.2,<41.0.0"
 Django = "^3.2.13"
-django-environ = "^0.9.0"
-django-filter = "^22.1"
+django-environ = "^0.10.0"
+django-filter = "^23.1"
 django-generic-api-permissions = "^0.2.0"
 djangorestframework = "^3.13.1"
 djangorestframework-jsonapi = "^5.0.0"
 mozilla-django-oidc = "^2.0.0"
 psycopg2-binary = "^2.9.3"
 requests = "^2.28.0"
 uWSGI = "^2.0.20"
 
 [tool.poetry.dev-dependencies]
-black = "22.8.0"
+black = "23.3.0"
 django-extensions = "3.2.1"
 factory-boy = "3.2.1"
-flake8 = "4.0.1"
+flake8 = "6.0.0"
 flake8-blind-except = "0.2.1"
 flake8-debugger = "4.1.2"
-flake8-docstrings = "1.6.0"
-flake8-isort = "4.2.0"
+flake8-docstrings = "1.7.0"
+flake8-isort = "6.0.0"
 flake8-string-format = "0.3.0"
 flake8-tuple = "0.4.1"
-gitlint = "0.17.0"
-ipython = "8.5.0"
-isort = "5.10.1"
-lxml = "4.9.1"
+gitlint = "0.19.1"
+ipython = "8.12.2"
+isort = "5.12.0"
+lxml = "4.9.2"
 pdbpp = "0.10.3"
-pre-commit = "2.20.0"
-pytest = "7.1.3"
-pytest-cov = "3.0.0"
+pre-commit = "3.3.1"
+pytest = "7.3.1"
+pytest-cov = "4.0.0"
 pytest-django = "4.5.2"
-pytest-env = "0.6.2"
-pytest-factoryboy = "2.5.0"
-pytest-mock = "3.8.2"
+pytest-env = "0.8.1"
+pytest-factoryboy = "2.5.1"
+pytest-mock = "3.10.0"
 pytest-randomly = "3.12.0"
-python-semantic-release = "7.31.4"
+python-semantic-release = "7.33.3"
 requests-mock = "1.10.0"
 snapshottest = "0.6.0"
-xmlschema = "2.0.4"
+xmlschema = "2.2.3"
 
 [tool.isort]
 skip = [
   "migrations",
   "snapshots",
 ]
 known_first_party = "ebau_gwr"
```

### Comparing `ebau-gwr-0.6.1/PKG-INFO` & `ebau_gwr-0.6.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,59 +1,59 @@
 Metadata-Version: 2.1
 Name: ebau-gwr
-Version: 0.6.1
+Version: 0.6.2
 Summary: GWR synchronisation for ebau projects
-Home-page: https://github.com/adfinis-sygroup/ebau-gwr
+Home-page: https://github.com/inosca/ebau-gwr
 License: GPL-3.0-or-later
 Author: Adfinis AG
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.8.1,<4.0.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django :: 3.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Requires-Dist: Django (>=3.2.13,<4.0.0)
-Requires-Dist: cryptography (>=37.0.2,<39.0.0)
-Requires-Dist: django-environ (>=0.9.0,<0.10.0)
-Requires-Dist: django-filter (>=22.1,<23.0)
+Requires-Dist: cryptography (>=37.0.2,<41.0.0)
+Requires-Dist: django-environ (>=0.10.0,<0.11.0)
+Requires-Dist: django-filter (>=23.1,<24.0)
 Requires-Dist: django-generic-api-permissions (>=0.2.0,<0.3.0)
 Requires-Dist: djangorestframework (>=3.13.1,<4.0.0)
 Requires-Dist: djangorestframework-jsonapi (>=5.0.0,<6.0.0)
 Requires-Dist: mozilla-django-oidc (>=2.0.0,<3.0.0)
 Requires-Dist: psycopg2-binary (>=2.9.3,<3.0.0)
 Requires-Dist: requests (>=2.28.0,<3.0.0)
 Requires-Dist: uWSGI (>=2.0.20,<3.0.0)
-Project-URL: Repository, https://github.com/adfinis-sygroup/ebau-gwr
+Project-URL: Repository, https://github.com/inosca/ebau-gwr
 Description-Content-Type: text/markdown
 
 # ebau-gwr
 
-[![Build Status](https://github.com/adfinis-sygroup/ebau-gwr/workflows/Tests/badge.svg)](https://github.com/adfinis-sygroup/ebau-gwr/actions?query=workflow%3ATests)
-[![Coverage](https://img.shields.io/badge/coverage-100%25-brightgreen.svg)](https://github.com/adfinis-sygroup/ebau-gwr/blob/main/pyproject.toml#L99)
-[![Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/adfinis-sygroup/ebau-gwr)
+[![Build Status](https://github.com/inosca/ebau-gwr/workflows/Tests/badge.svg)](https://github.com/inosca/ebau-gwr/actions?query=workflow%3ATests)
+[![Coverage](https://img.shields.io/badge/coverage-100%25-brightgreen.svg)](https://github.com/inosca/ebau-gwr/blob/main/pyproject.toml#L99)
+[![Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/inosca/ebau-gwr)
 
 GWR synchronisation for ebau projects
 
 ## Getting started
 
 ### Installation
 
 **Requirements**
 
 - docker
 - docker-compose
 
-After installing and configuring those, download [docker-compose.yml](https://raw.githubusercontent.com/adfinis/ebau-gwr/main/docker-compose.yml) and run the following command:
+After installing and configuring those, download [docker-compose.yml](https://raw.githubusercontent.com/inosca/ebau-gwr/main/docker-compose.yml) and run the following command:
 
 ```bash
 docker-compose up -d
 ```
 
 You can now access the api at [http://localhost:8000/api/v1/](http://localhost:8000/api/v1/).
```

