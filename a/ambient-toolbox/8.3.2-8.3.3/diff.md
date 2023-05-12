# Comparing `tmp/ambient-toolbox-8.3.2.tar.gz` & `tmp/ambient-toolbox-8.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ambient-toolbox-8.3.2.tar", last modified: Thu May 11 17:22:58 2023, max compression
+gzip compressed data, was "ambient-toolbox-8.3.3.tar", last modified: Fri May 12 06:13:57 2023, max compression
```

## Comparing `ambient-toolbox-8.3.2.tar` & `ambient-toolbox-8.3.3.tar`

### file list

```diff
@@ -1,220 +1,220 @@
--rw-r--r--   0        0        0     3087 2023-05-09 14:44:04.411372 ambient-toolbox-8.3.2/.ambient-package-update/metadata.py
--rw-r--r--   0        0        0       82 2023-05-10 08:29:28.641744 ambient-toolbox-8.3.2/.coveragerc
--rw-r--r--   0        0        0      288 2023-05-10 08:29:28.641744 ambient-toolbox-8.3.2/.editorconfig
--rw-r--r--   0        0        0     1700 2023-05-10 08:29:28.669738 ambient-toolbox-8.3.2/.github/workflows/ci.yml
--rw-r--r--   0        0        0     3461 2023-05-04 10:28:20.851321 ambient-toolbox-8.3.2/.gitignore
--rw-r--r--   0        0        0     3942 2023-05-04 10:28:20.851321 ambient-toolbox-8.3.2/.gitlab-ci.yml
--rw-r--r--   0        0        0      904 2023-05-10 08:29:28.641744 ambient-toolbox-8.3.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0      551 2023-05-10 08:29:28.641744 ambient-toolbox-8.3.2/.readthedocs.yml
--rw-r--r--   0        0        0    18823 2023-05-11 17:22:39.847018 ambient-toolbox-8.3.2/CHANGES.md
--rw-r--r--   0        0        0      964 2023-05-04 10:28:20.851321 ambient-toolbox-8.3.2/Dockerfile
--rw-r--r--   0        0        0     1107 2023-05-10 08:29:28.641744 ambient-toolbox-8.3.2/LICENSE.md
--rw-r--r--   0        0        0      134 2023-05-10 08:29:28.650251 ambient-toolbox-8.3.2/MANIFEST.in
--rw-r--r--   0        0        0     5853 2023-05-10 08:29:28.665928 ambient-toolbox-8.3.2/README.md
--rw-r--r--   0        0        0      116 2023-05-11 17:22:39.859059 ambient-toolbox-8.3.2/ambient_toolbox/__init__.py
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.851321 ambient-toolbox-8.3.2/ambient_toolbox/admin/__init__.py
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.851321 ambient-toolbox-8.3.2/ambient_toolbox/admin/model_admins/__init__.py
--rw-r--r--   0        0        0     1644 2023-05-04 10:28:20.851321 ambient-toolbox-8.3.2/ambient_toolbox/admin/model_admins/classes.py
--rw-r--r--   0        0        0      824 2023-05-04 10:28:20.851321 ambient-toolbox-8.3.2/ambient_toolbox/admin/model_admins/inlines.py
--rw-r--r--   0        0        0     4623 2023-05-04 10:28:20.851321 ambient-toolbox-8.3.2/ambient_toolbox/admin/model_admins/mixins.py
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.851321 ambient-toolbox-8.3.2/ambient_toolbox/admin/views/__init__.py
--rw-r--r--   0        0        0     1100 2023-05-04 10:28:20.851321 ambient-toolbox-8.3.2/ambient_toolbox/admin/views/forms.py
--rw-r--r--   0        0        0     2427 2023-05-04 10:28:20.851321 ambient-toolbox-8.3.2/ambient_toolbox/admin/views/mixins.py
--rw-r--r--   0        0        0      206 2023-05-04 10:28:20.851321 ambient-toolbox-8.3.2/ambient_toolbox/apps.py
--rw-r--r--   0        0        0      942 2023-05-04 10:28:20.851321 ambient-toolbox-8.3.2/ambient_toolbox/context_manager.py
--rw-r--r--   0        0        0      147 2023-05-04 10:28:20.851321 ambient-toolbox-8.3.2/ambient_toolbox/context_processors.py
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.851321 ambient-toolbox-8.3.2/ambient_toolbox/drf/__init__.py
--rw-r--r--   0        0        0     1031 2023-05-04 10:28:20.851321 ambient-toolbox-8.3.2/ambient_toolbox/drf/fields.py
--rw-r--r--   0        0        0     1143 2023-05-04 10:28:20.851321 ambient-toolbox-8.3.2/ambient_toolbox/drf/serializers.py
--rw-r--r--   0        0        0     3226 2023-05-04 10:28:20.863829 ambient-toolbox-8.3.2/ambient_toolbox/drf/tests.py
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.863829 ambient-toolbox-8.3.2/ambient_toolbox/gitlab/__init__.py
--rw-r--r--   0        0        0     9623 2023-05-04 10:28:20.863829 ambient-toolbox-8.3.2/ambient_toolbox/gitlab/coverage.py
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.863829 ambient-toolbox-8.3.2/ambient_toolbox/graphql/__init__.py
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.863829 ambient-toolbox-8.3.2/ambient_toolbox/graphql/forms/__init__.py
--rw-r--r--   0        0        0     1687 2023-05-04 10:28:20.863829 ambient-toolbox-8.3.2/ambient_toolbox/graphql/forms/mutations.py
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.863829 ambient-toolbox-8.3.2/ambient_toolbox/graphql/schemes/__init__.py
--rw-r--r--   0        0        0     2065 2023-05-04 10:28:20.863829 ambient-toolbox-8.3.2/ambient_toolbox/graphql/schemes/mutations.py
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.863829 ambient-toolbox-8.3.2/ambient_toolbox/graphql/sentry/__init__.py
--rw-r--r--   0        0        0      419 2023-05-04 10:28:20.863829 ambient-toolbox-8.3.2/ambient_toolbox/graphql/sentry/utils.py
--rw-r--r--   0        0        0     1342 2023-05-04 10:28:20.863829 ambient-toolbox-8.3.2/ambient_toolbox/graphql/sentry/views.py
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.863829 ambient-toolbox-8.3.2/ambient_toolbox/graphql/tests/__init__.py
--rw-r--r--   0        0        0     2144 2023-05-04 10:28:20.863829 ambient-toolbox-8.3.2/ambient_toolbox/graphql/tests/base_test.py
--rw-r--r--   0        0        0     1360 2023-05-04 10:28:20.863829 ambient-toolbox-8.3.2/ambient_toolbox/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     2177 2023-05-04 10:28:20.863829 ambient-toolbox-8.3.2/ambient_toolbox/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.863829 ambient-toolbox-8.3.2/ambient_toolbox/mail/__init__.py
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.863829 ambient-toolbox-8.3.2/ambient_toolbox/mail/backends/__init__.py
--rw-r--r--   0        0        0     3226 2023-05-04 10:28:20.863829 ambient-toolbox-8.3.2/ambient_toolbox/mail/backends/whitelist_smtp.py
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.863829 ambient-toolbox-8.3.2/ambient_toolbox/management/__init__.py
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.863829 ambient-toolbox-8.3.2/ambient_toolbox/management/commands/__init__.py
--rw-r--r--   0        0        0     1745 2023-05-11 17:08:22.645616 ambient-toolbox-8.3.2/ambient_toolbox/management/commands/install_permission_fixtures.py
--rw-r--r--   0        0        0      303 2023-05-04 10:28:20.863829 ambient-toolbox-8.3.2/ambient_toolbox/management/commands/validate_test_structure.py
--rw-r--r--   0        0        0     2550 2023-05-04 10:28:20.863829 ambient-toolbox-8.3.2/ambient_toolbox/managers.py
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.863829 ambient-toolbox-8.3.2/ambient_toolbox/middleware/__init__.py
--rw-r--r--   0        0        0     1050 2023-05-04 10:28:20.863829 ambient-toolbox-8.3.2/ambient_toolbox/middleware/current_user.py
--rw-r--r--   0        0        0       31 2023-05-04 10:28:20.863829 ambient-toolbox-8.3.2/ambient_toolbox/mixins/__init__.py
--rw-r--r--   0        0        0     1958 2023-05-04 10:28:20.863829 ambient-toolbox-8.3.2/ambient_toolbox/mixins/bleacher.py
--rw-r--r--   0        0        0     1378 2023-05-04 10:28:20.863829 ambient-toolbox-8.3.2/ambient_toolbox/mixins/models.py
--rw-r--r--   0        0        0      246 2023-05-04 10:28:20.863829 ambient-toolbox-8.3.2/ambient_toolbox/mixins/validation.py
--rw-r--r--   0        0        0     2592 2023-05-04 10:28:20.863829 ambient-toolbox-8.3.2/ambient_toolbox/models.py
--rw-r--r--   0        0        0        0 2023-05-11 13:43:18.462606 ambient-toolbox-8.3.2/ambient_toolbox/permissions/__init__.py
--rw-r--r--   0        0        0        0 2023-05-11 13:46:58.441382 ambient-toolbox-8.3.2/ambient_toolbox/permissions/fixtures/__init__.py
--rw-r--r--   0        0        0      282 2023-05-10 12:00:00.846663 ambient-toolbox-8.3.2/ambient_toolbox/permissions/fixtures/declarations.py
--rw-r--r--   0        0        0      206 2023-05-11 11:24:03.329388 ambient-toolbox-8.3.2/ambient_toolbox/permissions/fixtures/helpers.py
--rw-r--r--   0        0        0     3051 2023-05-11 13:57:05.202800 ambient-toolbox-8.3.2/ambient_toolbox/permissions/fixtures/services.py
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.863829 ambient-toolbox-8.3.2/ambient_toolbox/selectors/__init__.py
--rw-r--r--   0        0        0      362 2023-05-04 10:28:20.863829 ambient-toolbox-8.3.2/ambient_toolbox/selectors/base.py
--rw-r--r--   0        0        0     1061 2023-05-04 10:28:20.863829 ambient-toolbox-8.3.2/ambient_toolbox/selectors/permission.py
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.863829 ambient-toolbox-8.3.2/ambient_toolbox/sentry/__init__.py
--rw-r--r--   0        0        0     2155 2023-05-09 14:45:08.006243 ambient-toolbox-8.3.2/ambient_toolbox/sentry/helpers.py
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.863829 ambient-toolbox-8.3.2/ambient_toolbox/services/__init__.py
--rw-r--r--   0        0        0     3223 2023-05-04 10:28:20.863829 ambient-toolbox-8.3.2/ambient_toolbox/services/custom_scrubber.py
--rw-r--r--   0        0        0       31 2023-05-04 10:28:20.863829 ambient-toolbox-8.3.2/ambient_toolbox/templatetags/__init__.py
--rw-r--r--   0        0        0      244 2023-05-04 10:28:20.863829 ambient-toolbox-8.3.2/ambient_toolbox/templatetags/ai_date_tags.py
--rw-r--r--   0        0        0      675 2023-05-04 10:28:20.879472 ambient-toolbox-8.3.2/ambient_toolbox/templatetags/ai_email_tags.py
--rw-r--r--   0        0        0      807 2023-05-04 10:28:20.879472 ambient-toolbox-8.3.2/ambient_toolbox/templatetags/ai_file_tags.py
--rw-r--r--   0        0        0      194 2023-05-04 10:28:20.879472 ambient-toolbox-8.3.2/ambient_toolbox/templatetags/ai_helper_tags.py
--rw-r--r--   0        0        0     1375 2023-05-04 10:28:20.879472 ambient-toolbox-8.3.2/ambient_toolbox/templatetags/ai_number_tags.py
--rw-r--r--   0        0        0      384 2023-05-04 10:28:20.879472 ambient-toolbox-8.3.2/ambient_toolbox/templatetags/ai_object_tags.py
--rw-r--r--   0        0        0      654 2023-05-04 10:28:20.879472 ambient-toolbox-8.3.2/ambient_toolbox/templatetags/ai_string_tags.py
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.879472 ambient-toolbox-8.3.2/ambient_toolbox/tests/__init__.py
--rw-r--r--   0        0        0       60 2023-05-04 10:28:20.879472 ambient-toolbox-8.3.2/ambient_toolbox/tests/errors.py
--rw-r--r--   0        0        0     5145 2023-05-04 10:28:20.879472 ambient-toolbox-8.3.2/ambient_toolbox/tests/mixins.py
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.879472 ambient-toolbox-8.3.2/ambient_toolbox/tests/structure_validator/__init__.py
--rw-r--r--   0        0        0      397 2023-05-04 10:28:20.879472 ambient-toolbox-8.3.2/ambient_toolbox/tests/structure_validator/settings.py
--rw-r--r--   0        0        0     4634 2023-05-04 10:28:20.883484 ambient-toolbox-8.3.2/ambient_toolbox/tests/structure_validator/test_structure_validator.py
--rw-r--r--   0        0        0      261 2023-05-04 10:28:20.883484 ambient-toolbox-8.3.2/ambient_toolbox/utils/__init__.py
--rw-r--r--   0        0        0      127 2023-05-04 10:28:20.883484 ambient-toolbox-8.3.2/ambient_toolbox/utils/cache.py
--rw-r--r--   0        0        0     5971 2023-05-04 10:28:20.883484 ambient-toolbox-8.3.2/ambient_toolbox/utils/date.py
--rw-r--r--   0        0        0     1469 2023-05-04 10:28:20.883484 ambient-toolbox-8.3.2/ambient_toolbox/utils/file.py
--rw-r--r--   0        0        0      343 2023-05-04 10:28:20.883484 ambient-toolbox-8.3.2/ambient_toolbox/utils/log_whodid.py
--rw-r--r--   0        0        0      574 2023-05-04 10:28:20.883484 ambient-toolbox-8.3.2/ambient_toolbox/utils/math.py
--rw-r--r--   0        0        0      935 2023-05-04 10:28:20.883484 ambient-toolbox-8.3.2/ambient_toolbox/utils/model.py
--rw-r--r--   0        0        0     3970 2023-05-04 10:28:20.883484 ambient-toolbox-8.3.2/ambient_toolbox/utils/named_tuple.py
--rw-r--r--   0        0        0     3804 2023-05-04 10:28:20.883484 ambient-toolbox-8.3.2/ambient_toolbox/utils/string.py
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.883484 ambient-toolbox-8.3.2/ambient_toolbox/view_layer/__init__.py
--rw-r--r--   0        0        0      750 2023-05-04 10:28:20.883484 ambient-toolbox-8.3.2/ambient_toolbox/view_layer/form_mixins.py
--rw-r--r--   0        0        0      485 2023-05-04 10:28:20.883484 ambient-toolbox-8.3.2/ambient_toolbox/view_layer/formset_mixins.py
--rw-r--r--   0        0        0     2998 2023-05-04 10:28:20.883484 ambient-toolbox-8.3.2/ambient_toolbox/view_layer/formset_view_mixin.py
--rw-r--r--   0        0        0     1585 2023-05-04 10:28:20.883484 ambient-toolbox-8.3.2/ambient_toolbox/view_layer/htmx_mixins.py
--rw-r--r--   0        0        0     2110 2023-05-04 10:28:20.883484 ambient-toolbox-8.3.2/ambient_toolbox/view_layer/mixins.py
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.883484 ambient-toolbox-8.3.2/ambient_toolbox/view_layer/tests/__init__.py
--rw-r--r--   0        0        0     4124 2023-05-04 10:28:20.883484 ambient-toolbox-8.3.2/ambient_toolbox/view_layer/tests/mixins.py
--rw-r--r--   0        0        0     1882 2023-05-04 10:28:20.883484 ambient-toolbox-8.3.2/ambient_toolbox/view_layer/views.py
--rw-r--r--   0        0        0      654 2023-05-10 08:29:28.674940 ambient-toolbox-8.3.2/docs/Makefile
--rw-r--r--   0        0        0     2803 2023-05-10 08:29:28.671819 ambient-toolbox-8.3.2/docs/conf.py
--rw-r--r--   0        0        0     6731 2023-05-04 10:28:20.883484 ambient-toolbox-8.3.2/docs/features/admin.md
--rw-r--r--   0        0        0       35 2023-05-04 10:28:20.883484 ambient-toolbox-8.3.2/docs/features/changelog.rst
--rw-r--r--   0        0        0     2313 2023-05-04 10:28:20.883484 ambient-toolbox-8.3.2/docs/features/context_manager.md
--rw-r--r--   0        0        0      549 2023-05-04 10:28:20.883484 ambient-toolbox-8.3.2/docs/features/context_processors.md
--rw-r--r--   0        0        0     7273 2023-05-04 10:28:20.883484 ambient-toolbox-8.3.2/docs/features/database_anonymisation.md
--rw-r--r--   0        0        0     6807 2023-05-04 10:28:20.883484 ambient-toolbox-8.3.2/docs/features/djangorestframework.md
--rw-r--r--   0        0        0     2554 2023-05-04 10:28:20.883484 ambient-toolbox-8.3.2/docs/features/gitlab.md
--rw-r--r--   0        0        0     6567 2023-05-04 10:28:20.883484 ambient-toolbox-8.3.2/docs/features/graphql.md
--rw-r--r--   0        0        0     1020 2023-05-04 10:28:20.895496 ambient-toolbox-8.3.2/docs/features/mail.md
--rw-r--r--   0        0        0     5891 2023-05-04 10:28:20.895496 ambient-toolbox-8.3.2/docs/features/managers.md
--rw-r--r--   0        0        0     5951 2023-05-04 10:28:20.895496 ambient-toolbox-8.3.2/docs/features/mixins.md
--rw-r--r--   0        0        0     1553 2023-05-04 10:28:20.895496 ambient-toolbox-8.3.2/docs/features/models.md
--rw-r--r--   0        0        0     5637 2023-05-11 17:22:39.859059 ambient-toolbox-8.3.2/docs/features/permissions.md
--rw-r--r--   0        0        0     4454 2023-05-04 10:28:20.895496 ambient-toolbox-8.3.2/docs/features/selectors.md
--rw-r--r--   0        0        0     3290 2023-05-09 14:44:04.411372 ambient-toolbox-8.3.2/docs/features/sentry.md
--rw-r--r--   0        0        0     4978 2023-05-04 10:28:20.895496 ambient-toolbox-8.3.2/docs/features/services.md
--rw-r--r--   0        0        0     1574 2023-05-04 10:28:20.895496 ambient-toolbox-8.3.2/docs/features/setup.md
--rw-r--r--   0        0        0     5338 2023-05-04 10:28:20.895496 ambient-toolbox-8.3.2/docs/features/tests.md
--rw-r--r--   0        0        0      232 2023-05-04 10:28:20.895496 ambient-toolbox-8.3.2/docs/features/utils.rst
--rw-r--r--   0        0        0      527 2023-05-04 10:28:20.895496 ambient-toolbox-8.3.2/docs/features/utils/cache.md
--rw-r--r--   0        0        0     7417 2023-05-04 10:28:20.895496 ambient-toolbox-8.3.2/docs/features/utils/date.md
--rw-r--r--   0        0        0      737 2023-05-04 10:28:20.895496 ambient-toolbox-8.3.2/docs/features/utils/math.md
--rw-r--r--   0        0        0     1100 2023-05-04 10:28:20.895496 ambient-toolbox-8.3.2/docs/features/utils/model.md
--rw-r--r--   0        0        0     2405 2023-05-04 10:28:20.895496 ambient-toolbox-8.3.2/docs/features/utils/named_tuple.md
--rw-r--r--   0        0        0     5861 2023-05-04 10:28:20.895496 ambient-toolbox-8.3.2/docs/features/utils/string.md
--rw-r--r--   0        0        0    15067 2023-05-04 10:28:20.895496 ambient-toolbox-8.3.2/docs/features/view-layer.md
--rw-r--r--   0        0        0     1142 2023-05-11 16:39:56.593947 ambient-toolbox-8.3.2/docs/index.rst
--rwxr-xr-x   0        0        0      795 2023-05-10 08:29:28.673380 ambient-toolbox-8.3.2/docs/make.bat
--rw-r--r--   0        0        0      677 2023-05-04 10:28:20.895496 ambient-toolbox-8.3.2/manage.py
--rw-r--r--   0        0        0     4100 2023-05-10 08:29:28.650251 ambient-toolbox-8.3.2/pyproject.toml
--rw-r--r--   0        0        0       56 2023-05-04 10:28:20.895496 ambient-toolbox-8.3.2/pytest.ini
--rw-r--r--   0        0        0       56 2023-05-10 08:29:28.650251 ambient-toolbox-8.3.2/pytest.init
--rw-r--r--   0        0        0       50 2023-05-10 08:29:28.676006 ambient-toolbox-8.3.2/scripts/publish_to_pypi.ps1
--rw-r--r--   0        0        0       50 2023-05-10 08:29:28.677568 ambient-toolbox-8.3.2/scripts/publish_to_pypi.sh
--rw-r--r--   0        0        0     1704 2023-05-11 16:23:28.767887 ambient-toolbox-8.3.2/settings.py
--rw-r--r--   0        0        0       69 2023-05-10 08:29:28.667948 ambient-toolbox-8.3.2/setup.cfg
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.895496 ambient-toolbox-8.3.2/testapp/__init__.py
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.895496 ambient-toolbox-8.3.2/testapp/api/__init__.py
--rw-r--r--   0        0        0      287 2023-05-04 10:28:20.895496 ambient-toolbox-8.3.2/testapp/api/serializers.py
--rw-r--r--   0        0        0      257 2023-05-04 10:28:20.895496 ambient-toolbox-8.3.2/testapp/api/urls.py
--rw-r--r--   0        0        0      524 2023-05-04 10:28:20.895496 ambient-toolbox-8.3.2/testapp/api/views.py
--rw-r--r--   0        0        0      219 2023-05-04 10:28:20.895496 ambient-toolbox-8.3.2/testapp/forms.py
--rw-r--r--   0        0        0       97 2023-05-04 10:28:20.895496 ambient-toolbox-8.3.2/testapp/managers.py
--rw-r--r--   0        0        0     6151 2023-05-04 10:28:20.895496 ambient-toolbox-8.3.2/testapp/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.895496 ambient-toolbox-8.3.2/testapp/migrations/__init__.py
--rw-r--r--   0        0        0     3363 2023-05-04 10:28:20.895496 ambient-toolbox-8.3.2/testapp/models.py
--rw-r--r--   0        0        0      406 2023-05-11 17:08:22.631636 ambient-toolbox-8.3.2/testapp/permissions.py
--rw-r--r--   0        0        0      162 2023-05-04 10:28:20.895496 ambient-toolbox-8.3.2/testapp/selectors.py
--rw-r--r--   0        0        0     1449 2023-05-04 10:28:20.895496 ambient-toolbox-8.3.2/testapp/templates/403.html
--rw-r--r--   0        0        0      145 2023-05-04 10:28:20.895496 ambient-toolbox-8.3.2/testapp/templates/testapp/test_template.html
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.895496 ambient-toolbox-8.3.2/testapp/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.895496 ambient-toolbox-8.3.2/testapp/tests/missing_init/test_ok.py
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.895496 ambient-toolbox-8.3.2/testapp/tests/subdirectory/__init__.py
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.2/testapp/tests/subdirectory/missing_test_prefix.py
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.2/testapp/tests/subdirectory/test_ok.py
--rw-r--r--   0        0        0      382 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.2/testapp/urls.py
--rw-r--r--   0        0        0      505 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.2/testapp/views.py
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.2/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.2/tests/admin/__init__.py
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.2/tests/admin/model_admin_mixins/__init__.py
--rw-r--r--   0        0        0     2607 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.2/tests/admin/model_admin_mixins/test_admin_common_info_mixin.py
--rw-r--r--   0        0        0     1900 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.2/tests/admin/model_admin_mixins/test_admin_create_form_mixin.py
--rw-r--r--   0        0        0     1683 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.2/tests/admin/model_admin_mixins/test_admin_no_inlines_for_create_mixin.py
--rw-r--r--   0        0        0     1184 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.2/tests/admin/model_admin_mixins/test_admin_request_in_form_mixin.py
--rw-r--r--   0        0        0     3871 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.2/tests/admin/model_admin_mixins/test_deactivatable_change_view_admin_mixin.py
--rw-r--r--   0        0        0     1492 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.2/tests/admin/model_admin_mixins/test_fetch_object_mixin.py
--rw-r--r--   0        0        0     1909 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.2/tests/admin/model_admin_mixins/test_fetch_parent_object_inline_mixin.py
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.2/tests/ambient_toolbox/__init__.py
--rw-r--r--   0        0        0     7503 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.2/tests/ambient_toolbox/test_test_structure_validator.py
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.2/tests/drf/__init__.py
--rw-r--r--   0        0        0     2579 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.2/tests/drf/test_fields.py
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.2/tests/mixins/__init__.py
--rw-r--r--   0        0        0      364 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.2/tests/mixins/validation.py
--rw-r--r--   0        0        0        0 2023-05-11 13:44:55.711963 ambient-toolbox-8.3.2/tests/permissions/__init__.py
--rw-r--r--   0        0        0        0 2023-05-11 13:47:09.381858 ambient-toolbox-8.3.2/tests/permissions/fixtures/__init__.py
--rw-r--r--   0        0        0     1064 2023-05-11 13:57:05.255995 ambient-toolbox-8.3.2/tests/permissions/fixtures/test_declarations.py
--rw-r--r--   0        0        0      564 2023-05-11 13:57:05.238632 ambient-toolbox-8.3.2/tests/permissions/fixtures/test_helpers.py
--rw-r--r--   0        0        0     7052 2023-05-11 17:08:22.706284 ambient-toolbox-8.3.2/tests/permissions/fixtures/test_services_setup_service.py
--rw-r--r--   0        0        0      963 2023-05-11 17:08:22.645616 ambient-toolbox-8.3.2/tests/permissions/test_install_permission_fixtures_command.py
--rw-r--r--   0        0        0      499 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.2/tests/query_selectors/test_base.py
--rw-r--r--   0        0        0     1631 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.2/tests/query_selectors/test_permission.py
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.2/tests/selectors/__init__.py
--rw-r--r--   0        0        0        0 2023-05-09 14:44:04.427021 ambient-toolbox-8.3.2/tests/sentry/__init__.py
--rw-r--r--   0        0        0     6196 2023-05-09 14:44:04.427021 ambient-toolbox-8.3.2/tests/sentry/mock_data.py
--rw-r--r--   0        0        0     1583 2023-05-09 14:44:04.427021 ambient-toolbox-8.3.2/tests/sentry/test_sentry_helper.py
--rw-r--r--   0        0        0      553 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.2/tests/test_admin_forms.py
--rw-r--r--   0        0        0     1612 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.2/tests/test_admin_inlines.py
--rw-r--r--   0        0        0     2651 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.2/tests/test_admin_model_admins_classes.py
--rw-r--r--   0        0        0     2899 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.2/tests/test_admin_view_mixins.py
--rw-r--r--   0        0        0     2218 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.2/tests/test_context_manager.py
--rw-r--r--   0        0        0      822 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.2/tests/test_log_whodid.py
--rw-r--r--   0        0        0     1169 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.2/tests/test_managers.py
--rw-r--r--   0        0        0     1628 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.2/tests/test_math.py
--rw-r--r--   0        0        0     2593 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.2/tests/test_middleware.py
--rw-r--r--   0        0        0     1200 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.2/tests/test_mixins_models.py
--rw-r--r--   0        0        0     1669 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.2/tests/test_models.py
--rw-r--r--   0        0        0     1780 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.2/tests/test_rest_api_mixins.py
--rw-r--r--   0        0        0      664 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.2/tests/test_scrubbing_service.py
--rw-r--r--   0        0        0      289 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.2/tests/test_utils_cache.py
--rw-r--r--   0        0        0    12741 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.2/tests/test_utils_date.py
--rw-r--r--   0        0        0     1593 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.2/tests/test_utils_file.py
--rw-r--r--   0        0        0      933 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.2/tests/test_utils_model.py
--rw-r--r--   0        0        0     3807 2023-05-04 10:28:20.926757 ambient-toolbox-8.3.2/tests/test_utils_named_tuple.py
--rw-r--r--   0        0        0     5343 2023-05-04 10:28:20.926757 ambient-toolbox-8.3.2/tests/test_utils_string.py
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.926757 ambient-toolbox-8.3.2/tests/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.926757 ambient-toolbox-8.3.2/tests/tests/mixins/__init__.py
--rw-r--r--   0        0        0      371 2023-05-04 10:28:20.926757 ambient-toolbox-8.3.2/tests/tests/mixins/models.py
--rw-r--r--   0        0        0      817 2023-05-04 10:28:20.926757 ambient-toolbox-8.3.2/tests/tests/mixins/test_django_message_framework.py
--rw-r--r--   0        0        0     2483 2023-05-04 10:28:20.926757 ambient-toolbox-8.3.2/tests/tests/mixins/test_request_provider_mixin.py
--rw-r--r--   0        0        0     2057 2023-05-04 10:28:20.926757 ambient-toolbox-8.3.2/tests/tests/test_mail_backends.py
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.926757 ambient-toolbox-8.3.2/tests/view_layer/__init__.py
--rw-r--r--   0        0        0     1891 2023-05-04 10:28:20.926757 ambient-toolbox-8.3.2/tests/view_layer/test_formset_mixins.py
--rw-r--r--   0        0        0     1564 2023-05-04 10:28:20.926757 ambient-toolbox-8.3.2/tests/view_layer/test_htmx_response_mixin.py
--rw-r--r--   0        0        0     3458 2023-05-04 10:28:20.926757 ambient-toolbox-8.3.2/tests/view_layer/test_meta_mixins.py
--rw-r--r--   0        0        0     1361 2023-05-04 10:28:20.926757 ambient-toolbox-8.3.2/tests/view_layer/test_views.py
--rw-r--r--   0        0        0     8311 1970-01-01 00:00:00.000000 ambient-toolbox-8.3.2/PKG-INFO
+-rw-r--r--   0        0        0     3087 2023-05-09 14:44:04.411372 ambient-toolbox-8.3.3/.ambient-package-update/metadata.py
+-rw-r--r--   0        0        0       82 2023-05-10 08:29:28.641744 ambient-toolbox-8.3.3/.coveragerc
+-rw-r--r--   0        0        0      288 2023-05-10 08:29:28.641744 ambient-toolbox-8.3.3/.editorconfig
+-rw-r--r--   0        0        0     1700 2023-05-10 08:29:28.669738 ambient-toolbox-8.3.3/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     3461 2023-05-04 10:28:20.851321 ambient-toolbox-8.3.3/.gitignore
+-rw-r--r--   0        0        0     3942 2023-05-04 10:28:20.851321 ambient-toolbox-8.3.3/.gitlab-ci.yml
+-rw-r--r--   0        0        0      904 2023-05-12 06:09:33.558023 ambient-toolbox-8.3.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      551 2023-05-10 08:29:28.641744 ambient-toolbox-8.3.3/.readthedocs.yml
+-rw-r--r--   0        0        0    18875 2023-05-12 06:10:25.038287 ambient-toolbox-8.3.3/CHANGES.md
+-rw-r--r--   0        0        0      964 2023-05-04 10:28:20.851321 ambient-toolbox-8.3.3/Dockerfile
+-rw-r--r--   0        0        0     1107 2023-05-10 08:29:28.641744 ambient-toolbox-8.3.3/LICENSE.md
+-rw-r--r--   0        0        0      134 2023-05-10 08:29:28.650251 ambient-toolbox-8.3.3/MANIFEST.in
+-rw-r--r--   0        0        0     5853 2023-05-10 08:29:28.665928 ambient-toolbox-8.3.3/README.md
+-rw-r--r--   0        0        0      116 2023-05-12 06:10:25.038287 ambient-toolbox-8.3.3/ambient_toolbox/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.851321 ambient-toolbox-8.3.3/ambient_toolbox/admin/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.851321 ambient-toolbox-8.3.3/ambient_toolbox/admin/model_admins/__init__.py
+-rw-r--r--   0        0        0     1644 2023-05-04 10:28:20.851321 ambient-toolbox-8.3.3/ambient_toolbox/admin/model_admins/classes.py
+-rw-r--r--   0        0        0      824 2023-05-04 10:28:20.851321 ambient-toolbox-8.3.3/ambient_toolbox/admin/model_admins/inlines.py
+-rw-r--r--   0        0        0     4623 2023-05-04 10:28:20.851321 ambient-toolbox-8.3.3/ambient_toolbox/admin/model_admins/mixins.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.851321 ambient-toolbox-8.3.3/ambient_toolbox/admin/views/__init__.py
+-rw-r--r--   0        0        0     1100 2023-05-04 10:28:20.851321 ambient-toolbox-8.3.3/ambient_toolbox/admin/views/forms.py
+-rw-r--r--   0        0        0     2427 2023-05-04 10:28:20.851321 ambient-toolbox-8.3.3/ambient_toolbox/admin/views/mixins.py
+-rw-r--r--   0        0        0      206 2023-05-04 10:28:20.851321 ambient-toolbox-8.3.3/ambient_toolbox/apps.py
+-rw-r--r--   0        0        0      942 2023-05-04 10:28:20.851321 ambient-toolbox-8.3.3/ambient_toolbox/context_manager.py
+-rw-r--r--   0        0        0      147 2023-05-04 10:28:20.851321 ambient-toolbox-8.3.3/ambient_toolbox/context_processors.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.851321 ambient-toolbox-8.3.3/ambient_toolbox/drf/__init__.py
+-rw-r--r--   0        0        0     1031 2023-05-04 10:28:20.851321 ambient-toolbox-8.3.3/ambient_toolbox/drf/fields.py
+-rw-r--r--   0        0        0     1143 2023-05-04 10:28:20.851321 ambient-toolbox-8.3.3/ambient_toolbox/drf/serializers.py
+-rw-r--r--   0        0        0     3226 2023-05-04 10:28:20.863829 ambient-toolbox-8.3.3/ambient_toolbox/drf/tests.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.863829 ambient-toolbox-8.3.3/ambient_toolbox/gitlab/__init__.py
+-rw-r--r--   0        0        0     9623 2023-05-04 10:28:20.863829 ambient-toolbox-8.3.3/ambient_toolbox/gitlab/coverage.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.863829 ambient-toolbox-8.3.3/ambient_toolbox/graphql/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.863829 ambient-toolbox-8.3.3/ambient_toolbox/graphql/forms/__init__.py
+-rw-r--r--   0        0        0     1687 2023-05-04 10:28:20.863829 ambient-toolbox-8.3.3/ambient_toolbox/graphql/forms/mutations.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.863829 ambient-toolbox-8.3.3/ambient_toolbox/graphql/schemes/__init__.py
+-rw-r--r--   0        0        0     2065 2023-05-04 10:28:20.863829 ambient-toolbox-8.3.3/ambient_toolbox/graphql/schemes/mutations.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.863829 ambient-toolbox-8.3.3/ambient_toolbox/graphql/sentry/__init__.py
+-rw-r--r--   0        0        0      419 2023-05-04 10:28:20.863829 ambient-toolbox-8.3.3/ambient_toolbox/graphql/sentry/utils.py
+-rw-r--r--   0        0        0     1342 2023-05-04 10:28:20.863829 ambient-toolbox-8.3.3/ambient_toolbox/graphql/sentry/views.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.863829 ambient-toolbox-8.3.3/ambient_toolbox/graphql/tests/__init__.py
+-rw-r--r--   0        0        0     2144 2023-05-04 10:28:20.863829 ambient-toolbox-8.3.3/ambient_toolbox/graphql/tests/base_test.py
+-rw-r--r--   0        0        0     1360 2023-05-04 10:28:20.863829 ambient-toolbox-8.3.3/ambient_toolbox/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     2177 2023-05-04 10:28:20.863829 ambient-toolbox-8.3.3/ambient_toolbox/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.863829 ambient-toolbox-8.3.3/ambient_toolbox/mail/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.863829 ambient-toolbox-8.3.3/ambient_toolbox/mail/backends/__init__.py
+-rw-r--r--   0        0        0     3226 2023-05-04 10:28:20.863829 ambient-toolbox-8.3.3/ambient_toolbox/mail/backends/whitelist_smtp.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.863829 ambient-toolbox-8.3.3/ambient_toolbox/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.863829 ambient-toolbox-8.3.3/ambient_toolbox/management/commands/__init__.py
+-rw-r--r--   0        0        0     1745 2023-05-11 17:08:22.645616 ambient-toolbox-8.3.3/ambient_toolbox/management/commands/install_permission_fixtures.py
+-rw-r--r--   0        0        0      303 2023-05-04 10:28:20.863829 ambient-toolbox-8.3.3/ambient_toolbox/management/commands/validate_test_structure.py
+-rw-r--r--   0        0        0     2550 2023-05-04 10:28:20.863829 ambient-toolbox-8.3.3/ambient_toolbox/managers.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.863829 ambient-toolbox-8.3.3/ambient_toolbox/middleware/__init__.py
+-rw-r--r--   0        0        0     1050 2023-05-04 10:28:20.863829 ambient-toolbox-8.3.3/ambient_toolbox/middleware/current_user.py
+-rw-r--r--   0        0        0       31 2023-05-04 10:28:20.863829 ambient-toolbox-8.3.3/ambient_toolbox/mixins/__init__.py
+-rw-r--r--   0        0        0     1958 2023-05-04 10:28:20.863829 ambient-toolbox-8.3.3/ambient_toolbox/mixins/bleacher.py
+-rw-r--r--   0        0        0     1378 2023-05-04 10:28:20.863829 ambient-toolbox-8.3.3/ambient_toolbox/mixins/models.py
+-rw-r--r--   0        0        0      246 2023-05-04 10:28:20.863829 ambient-toolbox-8.3.3/ambient_toolbox/mixins/validation.py
+-rw-r--r--   0        0        0     2592 2023-05-04 10:28:20.863829 ambient-toolbox-8.3.3/ambient_toolbox/models.py
+-rw-r--r--   0        0        0        0 2023-05-11 13:43:18.462606 ambient-toolbox-8.3.3/ambient_toolbox/permissions/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-11 13:46:58.441382 ambient-toolbox-8.3.3/ambient_toolbox/permissions/fixtures/__init__.py
+-rw-r--r--   0        0        0      292 2023-05-11 17:30:53.043646 ambient-toolbox-8.3.3/ambient_toolbox/permissions/fixtures/declarations.py
+-rw-r--r--   0        0        0      232 2023-05-12 06:07:29.953470 ambient-toolbox-8.3.3/ambient_toolbox/permissions/fixtures/helpers.py
+-rw-r--r--   0        0        0     3116 2023-05-12 06:08:39.395472 ambient-toolbox-8.3.3/ambient_toolbox/permissions/fixtures/services.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.863829 ambient-toolbox-8.3.3/ambient_toolbox/selectors/__init__.py
+-rw-r--r--   0        0        0      362 2023-05-04 10:28:20.863829 ambient-toolbox-8.3.3/ambient_toolbox/selectors/base.py
+-rw-r--r--   0        0        0     1061 2023-05-04 10:28:20.863829 ambient-toolbox-8.3.3/ambient_toolbox/selectors/permission.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.863829 ambient-toolbox-8.3.3/ambient_toolbox/sentry/__init__.py
+-rw-r--r--   0        0        0     2155 2023-05-09 14:45:08.006243 ambient-toolbox-8.3.3/ambient_toolbox/sentry/helpers.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.863829 ambient-toolbox-8.3.3/ambient_toolbox/services/__init__.py
+-rw-r--r--   0        0        0     3223 2023-05-04 10:28:20.863829 ambient-toolbox-8.3.3/ambient_toolbox/services/custom_scrubber.py
+-rw-r--r--   0        0        0       31 2023-05-04 10:28:20.863829 ambient-toolbox-8.3.3/ambient_toolbox/templatetags/__init__.py
+-rw-r--r--   0        0        0      244 2023-05-04 10:28:20.863829 ambient-toolbox-8.3.3/ambient_toolbox/templatetags/ai_date_tags.py
+-rw-r--r--   0        0        0      675 2023-05-04 10:28:20.879472 ambient-toolbox-8.3.3/ambient_toolbox/templatetags/ai_email_tags.py
+-rw-r--r--   0        0        0      807 2023-05-04 10:28:20.879472 ambient-toolbox-8.3.3/ambient_toolbox/templatetags/ai_file_tags.py
+-rw-r--r--   0        0        0      194 2023-05-04 10:28:20.879472 ambient-toolbox-8.3.3/ambient_toolbox/templatetags/ai_helper_tags.py
+-rw-r--r--   0        0        0     1375 2023-05-04 10:28:20.879472 ambient-toolbox-8.3.3/ambient_toolbox/templatetags/ai_number_tags.py
+-rw-r--r--   0        0        0      384 2023-05-04 10:28:20.879472 ambient-toolbox-8.3.3/ambient_toolbox/templatetags/ai_object_tags.py
+-rw-r--r--   0        0        0      654 2023-05-04 10:28:20.879472 ambient-toolbox-8.3.3/ambient_toolbox/templatetags/ai_string_tags.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.879472 ambient-toolbox-8.3.3/ambient_toolbox/tests/__init__.py
+-rw-r--r--   0        0        0       60 2023-05-04 10:28:20.879472 ambient-toolbox-8.3.3/ambient_toolbox/tests/errors.py
+-rw-r--r--   0        0        0     5145 2023-05-04 10:28:20.879472 ambient-toolbox-8.3.3/ambient_toolbox/tests/mixins.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.879472 ambient-toolbox-8.3.3/ambient_toolbox/tests/structure_validator/__init__.py
+-rw-r--r--   0        0        0      397 2023-05-04 10:28:20.879472 ambient-toolbox-8.3.3/ambient_toolbox/tests/structure_validator/settings.py
+-rw-r--r--   0        0        0     4634 2023-05-04 10:28:20.883484 ambient-toolbox-8.3.3/ambient_toolbox/tests/structure_validator/test_structure_validator.py
+-rw-r--r--   0        0        0      261 2023-05-04 10:28:20.883484 ambient-toolbox-8.3.3/ambient_toolbox/utils/__init__.py
+-rw-r--r--   0        0        0      127 2023-05-04 10:28:20.883484 ambient-toolbox-8.3.3/ambient_toolbox/utils/cache.py
+-rw-r--r--   0        0        0     5971 2023-05-04 10:28:20.883484 ambient-toolbox-8.3.3/ambient_toolbox/utils/date.py
+-rw-r--r--   0        0        0     1469 2023-05-04 10:28:20.883484 ambient-toolbox-8.3.3/ambient_toolbox/utils/file.py
+-rw-r--r--   0        0        0      343 2023-05-04 10:28:20.883484 ambient-toolbox-8.3.3/ambient_toolbox/utils/log_whodid.py
+-rw-r--r--   0        0        0      574 2023-05-04 10:28:20.883484 ambient-toolbox-8.3.3/ambient_toolbox/utils/math.py
+-rw-r--r--   0        0        0      935 2023-05-04 10:28:20.883484 ambient-toolbox-8.3.3/ambient_toolbox/utils/model.py
+-rw-r--r--   0        0        0     3970 2023-05-04 10:28:20.883484 ambient-toolbox-8.3.3/ambient_toolbox/utils/named_tuple.py
+-rw-r--r--   0        0        0     3804 2023-05-04 10:28:20.883484 ambient-toolbox-8.3.3/ambient_toolbox/utils/string.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.883484 ambient-toolbox-8.3.3/ambient_toolbox/view_layer/__init__.py
+-rw-r--r--   0        0        0      750 2023-05-04 10:28:20.883484 ambient-toolbox-8.3.3/ambient_toolbox/view_layer/form_mixins.py
+-rw-r--r--   0        0        0      485 2023-05-04 10:28:20.883484 ambient-toolbox-8.3.3/ambient_toolbox/view_layer/formset_mixins.py
+-rw-r--r--   0        0        0     2998 2023-05-04 10:28:20.883484 ambient-toolbox-8.3.3/ambient_toolbox/view_layer/formset_view_mixin.py
+-rw-r--r--   0        0        0     1585 2023-05-04 10:28:20.883484 ambient-toolbox-8.3.3/ambient_toolbox/view_layer/htmx_mixins.py
+-rw-r--r--   0        0        0     2110 2023-05-04 10:28:20.883484 ambient-toolbox-8.3.3/ambient_toolbox/view_layer/mixins.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.883484 ambient-toolbox-8.3.3/ambient_toolbox/view_layer/tests/__init__.py
+-rw-r--r--   0        0        0     4124 2023-05-04 10:28:20.883484 ambient-toolbox-8.3.3/ambient_toolbox/view_layer/tests/mixins.py
+-rw-r--r--   0        0        0     1882 2023-05-04 10:28:20.883484 ambient-toolbox-8.3.3/ambient_toolbox/view_layer/views.py
+-rw-r--r--   0        0        0      654 2023-05-10 08:29:28.674940 ambient-toolbox-8.3.3/docs/Makefile
+-rw-r--r--   0        0        0     2803 2023-05-10 08:29:28.671819 ambient-toolbox-8.3.3/docs/conf.py
+-rw-r--r--   0        0        0     6731 2023-05-04 10:28:20.883484 ambient-toolbox-8.3.3/docs/features/admin.md
+-rw-r--r--   0        0        0       35 2023-05-04 10:28:20.883484 ambient-toolbox-8.3.3/docs/features/changelog.rst
+-rw-r--r--   0        0        0     2313 2023-05-04 10:28:20.883484 ambient-toolbox-8.3.3/docs/features/context_manager.md
+-rw-r--r--   0        0        0      549 2023-05-04 10:28:20.883484 ambient-toolbox-8.3.3/docs/features/context_processors.md
+-rw-r--r--   0        0        0     7273 2023-05-04 10:28:20.883484 ambient-toolbox-8.3.3/docs/features/database_anonymisation.md
+-rw-r--r--   0        0        0     6807 2023-05-04 10:28:20.883484 ambient-toolbox-8.3.3/docs/features/djangorestframework.md
+-rw-r--r--   0        0        0     2554 2023-05-04 10:28:20.883484 ambient-toolbox-8.3.3/docs/features/gitlab.md
+-rw-r--r--   0        0        0     6567 2023-05-04 10:28:20.883484 ambient-toolbox-8.3.3/docs/features/graphql.md
+-rw-r--r--   0        0        0     1020 2023-05-04 10:28:20.895496 ambient-toolbox-8.3.3/docs/features/mail.md
+-rw-r--r--   0        0        0     5891 2023-05-04 10:28:20.895496 ambient-toolbox-8.3.3/docs/features/managers.md
+-rw-r--r--   0        0        0     5951 2023-05-04 10:28:20.895496 ambient-toolbox-8.3.3/docs/features/mixins.md
+-rw-r--r--   0        0        0     1553 2023-05-04 10:28:20.895496 ambient-toolbox-8.3.3/docs/features/models.md
+-rw-r--r--   0        0        0     5637 2023-05-11 17:22:39.859059 ambient-toolbox-8.3.3/docs/features/permissions.md
+-rw-r--r--   0        0        0     4454 2023-05-04 10:28:20.895496 ambient-toolbox-8.3.3/docs/features/selectors.md
+-rw-r--r--   0        0        0     3290 2023-05-09 14:44:04.411372 ambient-toolbox-8.3.3/docs/features/sentry.md
+-rw-r--r--   0        0        0     4978 2023-05-04 10:28:20.895496 ambient-toolbox-8.3.3/docs/features/services.md
+-rw-r--r--   0        0        0     1574 2023-05-04 10:28:20.895496 ambient-toolbox-8.3.3/docs/features/setup.md
+-rw-r--r--   0        0        0     5338 2023-05-04 10:28:20.895496 ambient-toolbox-8.3.3/docs/features/tests.md
+-rw-r--r--   0        0        0      232 2023-05-04 10:28:20.895496 ambient-toolbox-8.3.3/docs/features/utils.rst
+-rw-r--r--   0        0        0      527 2023-05-04 10:28:20.895496 ambient-toolbox-8.3.3/docs/features/utils/cache.md
+-rw-r--r--   0        0        0     7417 2023-05-04 10:28:20.895496 ambient-toolbox-8.3.3/docs/features/utils/date.md
+-rw-r--r--   0        0        0      737 2023-05-04 10:28:20.895496 ambient-toolbox-8.3.3/docs/features/utils/math.md
+-rw-r--r--   0        0        0     1100 2023-05-04 10:28:20.895496 ambient-toolbox-8.3.3/docs/features/utils/model.md
+-rw-r--r--   0        0        0     2405 2023-05-04 10:28:20.895496 ambient-toolbox-8.3.3/docs/features/utils/named_tuple.md
+-rw-r--r--   0        0        0     5861 2023-05-04 10:28:20.895496 ambient-toolbox-8.3.3/docs/features/utils/string.md
+-rw-r--r--   0        0        0    15067 2023-05-04 10:28:20.895496 ambient-toolbox-8.3.3/docs/features/view-layer.md
+-rw-r--r--   0        0        0     1142 2023-05-11 16:39:56.593947 ambient-toolbox-8.3.3/docs/index.rst
+-rwxr-xr-x   0        0        0      795 2023-05-10 08:29:28.673380 ambient-toolbox-8.3.3/docs/make.bat
+-rw-r--r--   0        0        0      677 2023-05-04 10:28:20.895496 ambient-toolbox-8.3.3/manage.py
+-rw-r--r--   0        0        0     4100 2023-05-10 08:29:28.650251 ambient-toolbox-8.3.3/pyproject.toml
+-rw-r--r--   0        0        0       56 2023-05-04 10:28:20.895496 ambient-toolbox-8.3.3/pytest.ini
+-rw-r--r--   0        0        0       56 2023-05-10 08:29:28.650251 ambient-toolbox-8.3.3/pytest.init
+-rw-r--r--   0        0        0       50 2023-05-10 08:29:28.676006 ambient-toolbox-8.3.3/scripts/publish_to_pypi.ps1
+-rw-r--r--   0        0        0       50 2023-05-10 08:29:28.677568 ambient-toolbox-8.3.3/scripts/publish_to_pypi.sh
+-rw-r--r--   0        0        0     1704 2023-05-11 16:23:28.767887 ambient-toolbox-8.3.3/settings.py
+-rw-r--r--   0        0        0       69 2023-05-10 08:29:28.667948 ambient-toolbox-8.3.3/setup.cfg
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.895496 ambient-toolbox-8.3.3/testapp/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.895496 ambient-toolbox-8.3.3/testapp/api/__init__.py
+-rw-r--r--   0        0        0      287 2023-05-04 10:28:20.895496 ambient-toolbox-8.3.3/testapp/api/serializers.py
+-rw-r--r--   0        0        0      257 2023-05-04 10:28:20.895496 ambient-toolbox-8.3.3/testapp/api/urls.py
+-rw-r--r--   0        0        0      524 2023-05-04 10:28:20.895496 ambient-toolbox-8.3.3/testapp/api/views.py
+-rw-r--r--   0        0        0      219 2023-05-04 10:28:20.895496 ambient-toolbox-8.3.3/testapp/forms.py
+-rw-r--r--   0        0        0       97 2023-05-04 10:28:20.895496 ambient-toolbox-8.3.3/testapp/managers.py
+-rw-r--r--   0        0        0     6151 2023-05-04 10:28:20.895496 ambient-toolbox-8.3.3/testapp/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.895496 ambient-toolbox-8.3.3/testapp/migrations/__init__.py
+-rw-r--r--   0        0        0     3363 2023-05-04 10:28:20.895496 ambient-toolbox-8.3.3/testapp/models.py
+-rw-r--r--   0        0        0      406 2023-05-11 17:08:22.631636 ambient-toolbox-8.3.3/testapp/permissions.py
+-rw-r--r--   0        0        0      162 2023-05-04 10:28:20.895496 ambient-toolbox-8.3.3/testapp/selectors.py
+-rw-r--r--   0        0        0     1449 2023-05-04 10:28:20.895496 ambient-toolbox-8.3.3/testapp/templates/403.html
+-rw-r--r--   0        0        0      145 2023-05-04 10:28:20.895496 ambient-toolbox-8.3.3/testapp/templates/testapp/test_template.html
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.895496 ambient-toolbox-8.3.3/testapp/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.895496 ambient-toolbox-8.3.3/testapp/tests/missing_init/test_ok.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.895496 ambient-toolbox-8.3.3/testapp/tests/subdirectory/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.3/testapp/tests/subdirectory/missing_test_prefix.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.3/testapp/tests/subdirectory/test_ok.py
+-rw-r--r--   0        0        0      382 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.3/testapp/urls.py
+-rw-r--r--   0        0        0      505 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.3/testapp/views.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.3/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.3/tests/admin/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.3/tests/admin/model_admin_mixins/__init__.py
+-rw-r--r--   0        0        0     2607 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.3/tests/admin/model_admin_mixins/test_admin_common_info_mixin.py
+-rw-r--r--   0        0        0     1900 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.3/tests/admin/model_admin_mixins/test_admin_create_form_mixin.py
+-rw-r--r--   0        0        0     1683 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.3/tests/admin/model_admin_mixins/test_admin_no_inlines_for_create_mixin.py
+-rw-r--r--   0        0        0     1184 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.3/tests/admin/model_admin_mixins/test_admin_request_in_form_mixin.py
+-rw-r--r--   0        0        0     3871 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.3/tests/admin/model_admin_mixins/test_deactivatable_change_view_admin_mixin.py
+-rw-r--r--   0        0        0     1492 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.3/tests/admin/model_admin_mixins/test_fetch_object_mixin.py
+-rw-r--r--   0        0        0     1909 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.3/tests/admin/model_admin_mixins/test_fetch_parent_object_inline_mixin.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.3/tests/ambient_toolbox/__init__.py
+-rw-r--r--   0        0        0     7503 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.3/tests/ambient_toolbox/test_test_structure_validator.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.3/tests/drf/__init__.py
+-rw-r--r--   0        0        0     2579 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.3/tests/drf/test_fields.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.3/tests/mixins/__init__.py
+-rw-r--r--   0        0        0      364 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.3/tests/mixins/validation.py
+-rw-r--r--   0        0        0        0 2023-05-11 13:44:55.711963 ambient-toolbox-8.3.3/tests/permissions/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-11 13:47:09.381858 ambient-toolbox-8.3.3/tests/permissions/fixtures/__init__.py
+-rw-r--r--   0        0        0     1064 2023-05-11 13:57:05.255995 ambient-toolbox-8.3.3/tests/permissions/fixtures/test_declarations.py
+-rw-r--r--   0        0        0      564 2023-05-11 13:57:05.238632 ambient-toolbox-8.3.3/tests/permissions/fixtures/test_helpers.py
+-rw-r--r--   0        0        0     7053 2023-05-11 17:28:06.152820 ambient-toolbox-8.3.3/tests/permissions/fixtures/test_services_setup_service.py
+-rw-r--r--   0        0        0      963 2023-05-11 17:08:22.645616 ambient-toolbox-8.3.3/tests/permissions/test_install_permission_fixtures_command.py
+-rw-r--r--   0        0        0      499 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.3/tests/query_selectors/test_base.py
+-rw-r--r--   0        0        0     1631 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.3/tests/query_selectors/test_permission.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.3/tests/selectors/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-09 14:44:04.427021 ambient-toolbox-8.3.3/tests/sentry/__init__.py
+-rw-r--r--   0        0        0     6196 2023-05-09 14:44:04.427021 ambient-toolbox-8.3.3/tests/sentry/mock_data.py
+-rw-r--r--   0        0        0     1583 2023-05-09 14:44:04.427021 ambient-toolbox-8.3.3/tests/sentry/test_sentry_helper.py
+-rw-r--r--   0        0        0      553 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.3/tests/test_admin_forms.py
+-rw-r--r--   0        0        0     1612 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.3/tests/test_admin_inlines.py
+-rw-r--r--   0        0        0     2651 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.3/tests/test_admin_model_admins_classes.py
+-rw-r--r--   0        0        0     2899 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.3/tests/test_admin_view_mixins.py
+-rw-r--r--   0        0        0     2218 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.3/tests/test_context_manager.py
+-rw-r--r--   0        0        0      822 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.3/tests/test_log_whodid.py
+-rw-r--r--   0        0        0     1169 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.3/tests/test_managers.py
+-rw-r--r--   0        0        0     1628 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.3/tests/test_math.py
+-rw-r--r--   0        0        0     2593 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.3/tests/test_middleware.py
+-rw-r--r--   0        0        0     1200 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.3/tests/test_mixins_models.py
+-rw-r--r--   0        0        0     1669 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.3/tests/test_models.py
+-rw-r--r--   0        0        0     1780 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.3/tests/test_rest_api_mixins.py
+-rw-r--r--   0        0        0      664 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.3/tests/test_scrubbing_service.py
+-rw-r--r--   0        0        0      289 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.3/tests/test_utils_cache.py
+-rw-r--r--   0        0        0    12741 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.3/tests/test_utils_date.py
+-rw-r--r--   0        0        0     1593 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.3/tests/test_utils_file.py
+-rw-r--r--   0        0        0      933 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.3/tests/test_utils_model.py
+-rw-r--r--   0        0        0     3807 2023-05-04 10:28:20.926757 ambient-toolbox-8.3.3/tests/test_utils_named_tuple.py
+-rw-r--r--   0        0        0     5343 2023-05-04 10:28:20.926757 ambient-toolbox-8.3.3/tests/test_utils_string.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.926757 ambient-toolbox-8.3.3/tests/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.926757 ambient-toolbox-8.3.3/tests/tests/mixins/__init__.py
+-rw-r--r--   0        0        0      371 2023-05-04 10:28:20.926757 ambient-toolbox-8.3.3/tests/tests/mixins/models.py
+-rw-r--r--   0        0        0      817 2023-05-04 10:28:20.926757 ambient-toolbox-8.3.3/tests/tests/mixins/test_django_message_framework.py
+-rw-r--r--   0        0        0     2483 2023-05-04 10:28:20.926757 ambient-toolbox-8.3.3/tests/tests/mixins/test_request_provider_mixin.py
+-rw-r--r--   0        0        0     2057 2023-05-04 10:28:20.926757 ambient-toolbox-8.3.3/tests/tests/test_mail_backends.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.926757 ambient-toolbox-8.3.3/tests/view_layer/__init__.py
+-rw-r--r--   0        0        0     1891 2023-05-04 10:28:20.926757 ambient-toolbox-8.3.3/tests/view_layer/test_formset_mixins.py
+-rw-r--r--   0        0        0     1564 2023-05-04 10:28:20.926757 ambient-toolbox-8.3.3/tests/view_layer/test_htmx_response_mixin.py
+-rw-r--r--   0        0        0     3458 2023-05-04 10:28:20.926757 ambient-toolbox-8.3.3/tests/view_layer/test_meta_mixins.py
+-rw-r--r--   0        0        0     1361 2023-05-04 10:28:20.926757 ambient-toolbox-8.3.3/tests/view_layer/test_views.py
+-rw-r--r--   0        0        0     8311 1970-01-01 00:00:00.000000 ambient-toolbox-8.3.3/PKG-INFO
```

### Comparing `ambient-toolbox-8.3.2/.ambient-package-update/metadata.py` & `ambient-toolbox-8.3.3/.ambient-package-update/metadata.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.2/.github/workflows/ci.yml` & `ambient-toolbox-8.3.3/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.2/.gitignore` & `ambient-toolbox-8.3.3/.gitignore`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.2/.gitlab-ci.yml` & `ambient-toolbox-8.3.3/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.2/.pre-commit-config.yaml` & `ambient-toolbox-8.3.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.2/.readthedocs.yml` & `ambient-toolbox-8.3.3/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.2/CHANGES.md` & `ambient-toolbox-8.3.3/CHANGES.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 # Changelog
 
+**8.3.3** (2023-05-12)
+  * Fixed Python 3.8 compat
+
 **8.3.2** (2023-05-11)
   * Updated docs about permission settings setup
 
 **8.3.1** (2023-05-11)
   * Updated docs about permission feature limitations
 
 **8.3.0** (2023-05-11)
```

### Comparing `ambient-toolbox-8.3.2/Dockerfile` & `ambient-toolbox-8.3.3/Dockerfile`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.2/LICENSE.md` & `ambient-toolbox-8.3.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.2/README.md` & `ambient-toolbox-8.3.3/README.md`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.2/ambient_toolbox/admin/model_admins/classes.py` & `ambient-toolbox-8.3.3/ambient_toolbox/admin/model_admins/classes.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.2/ambient_toolbox/admin/model_admins/inlines.py` & `ambient-toolbox-8.3.3/ambient_toolbox/admin/model_admins/inlines.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.2/ambient_toolbox/admin/model_admins/mixins.py` & `ambient-toolbox-8.3.3/ambient_toolbox/admin/model_admins/mixins.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.2/ambient_toolbox/admin/views/forms.py` & `ambient-toolbox-8.3.3/ambient_toolbox/admin/views/forms.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.2/ambient_toolbox/admin/views/mixins.py` & `ambient-toolbox-8.3.3/ambient_toolbox/admin/views/mixins.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.2/ambient_toolbox/context_manager.py` & `ambient-toolbox-8.3.3/ambient_toolbox/context_manager.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.2/ambient_toolbox/drf/fields.py` & `ambient-toolbox-8.3.3/ambient_toolbox/drf/fields.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.2/ambient_toolbox/drf/serializers.py` & `ambient-toolbox-8.3.3/ambient_toolbox/drf/serializers.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.2/ambient_toolbox/drf/tests.py` & `ambient-toolbox-8.3.3/ambient_toolbox/drf/tests.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.2/ambient_toolbox/gitlab/coverage.py` & `ambient-toolbox-8.3.3/ambient_toolbox/gitlab/coverage.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.2/ambient_toolbox/graphql/forms/mutations.py` & `ambient-toolbox-8.3.3/ambient_toolbox/graphql/forms/mutations.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.2/ambient_toolbox/graphql/schemes/mutations.py` & `ambient-toolbox-8.3.3/ambient_toolbox/graphql/schemes/mutations.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.2/ambient_toolbox/graphql/sentry/views.py` & `ambient-toolbox-8.3.3/ambient_toolbox/graphql/sentry/views.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.2/ambient_toolbox/graphql/tests/base_test.py` & `ambient-toolbox-8.3.3/ambient_toolbox/graphql/tests/base_test.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.2/ambient_toolbox/locale/de/LC_MESSAGES/django.mo` & `ambient-toolbox-8.3.3/ambient_toolbox/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.2/ambient_toolbox/locale/de/LC_MESSAGES/django.po` & `ambient-toolbox-8.3.3/ambient_toolbox/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.2/ambient_toolbox/mail/backends/whitelist_smtp.py` & `ambient-toolbox-8.3.3/ambient_toolbox/mail/backends/whitelist_smtp.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.2/ambient_toolbox/management/commands/install_permission_fixtures.py` & `ambient-toolbox-8.3.3/ambient_toolbox/management/commands/install_permission_fixtures.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.2/ambient_toolbox/managers.py` & `ambient-toolbox-8.3.3/ambient_toolbox/managers.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.2/ambient_toolbox/middleware/current_user.py` & `ambient-toolbox-8.3.3/ambient_toolbox/middleware/current_user.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.2/ambient_toolbox/mixins/bleacher.py` & `ambient-toolbox-8.3.3/ambient_toolbox/mixins/bleacher.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.2/ambient_toolbox/mixins/models.py` & `ambient-toolbox-8.3.3/ambient_toolbox/mixins/models.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.2/ambient_toolbox/models.py` & `ambient-toolbox-8.3.3/ambient_toolbox/models.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.2/ambient_toolbox/permissions/fixtures/services.py` & `ambient-toolbox-8.3.3/ambient_toolbox/permissions/fixtures/services.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from typing import List
+
 from django.contrib.auth.models import Group, Permission
 from django.contrib.contenttypes.models import ContentType
 from django.db import transaction
 
 from ambient_toolbox.permissions.fixtures.declarations import GroupPermissionDeclaration
 
 
@@ -12,15 +14,15 @@
     def __init__(self, group_declaration: GroupPermissionDeclaration, dry_run: bool = False) -> None:
         super().__init__()
 
         self.group_declaration = group_declaration
         self.dry_run = dry_run
 
     @transaction.atomic
-    def process(self):
+    def process(self) -> (List[Permission], List[Permission]):
         # Fetch or create group
         group, created = Group.objects.get_or_create(name=self.group_declaration.name)
 
         # Declare lists where we'll sort in the permissions
         defined_permission_list = []
         new_permissions = []
         removed_permissions = []
```

### Comparing `ambient-toolbox-8.3.2/ambient_toolbox/selectors/permission.py` & `ambient-toolbox-8.3.3/ambient_toolbox/selectors/permission.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.2/ambient_toolbox/sentry/helpers.py` & `ambient-toolbox-8.3.3/ambient_toolbox/sentry/helpers.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.2/ambient_toolbox/services/custom_scrubber.py` & `ambient-toolbox-8.3.3/ambient_toolbox/services/custom_scrubber.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.2/ambient_toolbox/templatetags/ai_email_tags.py` & `ambient-toolbox-8.3.3/ambient_toolbox/templatetags/ai_email_tags.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.2/ambient_toolbox/templatetags/ai_file_tags.py` & `ambient-toolbox-8.3.3/ambient_toolbox/templatetags/ai_file_tags.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.2/ambient_toolbox/templatetags/ai_number_tags.py` & `ambient-toolbox-8.3.3/ambient_toolbox/templatetags/ai_number_tags.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.2/ambient_toolbox/templatetags/ai_string_tags.py` & `ambient-toolbox-8.3.3/ambient_toolbox/templatetags/ai_string_tags.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.2/ambient_toolbox/tests/mixins.py` & `ambient-toolbox-8.3.3/ambient_toolbox/tests/mixins.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.2/ambient_toolbox/tests/structure_validator/test_structure_validator.py` & `ambient-toolbox-8.3.3/ambient_toolbox/tests/structure_validator/test_structure_validator.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.2/ambient_toolbox/utils/date.py` & `ambient-toolbox-8.3.3/ambient_toolbox/utils/date.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.2/ambient_toolbox/utils/file.py` & `ambient-toolbox-8.3.3/ambient_toolbox/utils/file.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.2/ambient_toolbox/utils/math.py` & `ambient-toolbox-8.3.3/ambient_toolbox/utils/math.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.2/ambient_toolbox/utils/model.py` & `ambient-toolbox-8.3.3/ambient_toolbox/utils/model.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.2/ambient_toolbox/utils/named_tuple.py` & `ambient-toolbox-8.3.3/ambient_toolbox/utils/named_tuple.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.2/ambient_toolbox/utils/string.py` & `ambient-toolbox-8.3.3/ambient_toolbox/utils/string.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.2/ambient_toolbox/view_layer/form_mixins.py` & `ambient-toolbox-8.3.3/ambient_toolbox/view_layer/form_mixins.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.2/ambient_toolbox/view_layer/formset_view_mixin.py` & `ambient-toolbox-8.3.3/ambient_toolbox/view_layer/formset_view_mixin.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.2/ambient_toolbox/view_layer/htmx_mixins.py` & `ambient-toolbox-8.3.3/ambient_toolbox/view_layer/htmx_mixins.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.2/ambient_toolbox/view_layer/mixins.py` & `ambient-toolbox-8.3.3/ambient_toolbox/view_layer/mixins.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.2/ambient_toolbox/view_layer/tests/mixins.py` & `ambient-toolbox-8.3.3/ambient_toolbox/view_layer/tests/mixins.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.2/ambient_toolbox/view_layer/views.py` & `ambient-toolbox-8.3.3/ambient_toolbox/view_layer/views.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.2/docs/Makefile` & `ambient-toolbox-8.3.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.2/docs/conf.py` & `ambient-toolbox-8.3.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.2/docs/features/admin.md` & `ambient-toolbox-8.3.3/docs/features/admin.md`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.2/docs/features/context_manager.md` & `ambient-toolbox-8.3.3/docs/features/context_manager.md`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.2/docs/features/context_processors.md` & `ambient-toolbox-8.3.3/docs/features/context_processors.md`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.2/docs/features/database_anonymisation.md` & `ambient-toolbox-8.3.3/docs/features/database_anonymisation.md`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.2/docs/features/djangorestframework.md` & `ambient-toolbox-8.3.3/docs/features/djangorestframework.md`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.2/docs/features/gitlab.md` & `ambient-toolbox-8.3.3/docs/features/gitlab.md`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.2/docs/features/graphql.md` & `ambient-toolbox-8.3.3/docs/features/graphql.md`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.2/docs/features/mail.md` & `ambient-toolbox-8.3.3/docs/features/mail.md`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.2/docs/features/managers.md` & `ambient-toolbox-8.3.3/docs/features/managers.md`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.2/docs/features/mixins.md` & `ambient-toolbox-8.3.3/docs/features/mixins.md`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.2/docs/features/models.md` & `ambient-toolbox-8.3.3/docs/features/models.md`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.2/docs/features/permissions.md` & `ambient-toolbox-8.3.3/docs/features/permissions.md`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.2/docs/features/selectors.md` & `ambient-toolbox-8.3.3/docs/features/selectors.md`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.2/docs/features/sentry.md` & `ambient-toolbox-8.3.3/docs/features/sentry.md`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.2/docs/features/services.md` & `ambient-toolbox-8.3.3/docs/features/services.md`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.2/docs/features/setup.md` & `ambient-toolbox-8.3.3/docs/features/setup.md`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.2/docs/features/tests.md` & `ambient-toolbox-8.3.3/docs/features/tests.md`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.2/docs/features/utils/cache.md` & `ambient-toolbox-8.3.3/docs/features/utils/cache.md`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.2/docs/features/utils/date.md` & `ambient-toolbox-8.3.3/docs/features/utils/date.md`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.2/docs/features/utils/math.md` & `ambient-toolbox-8.3.3/docs/features/utils/math.md`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.2/docs/features/utils/model.md` & `ambient-toolbox-8.3.3/docs/features/utils/model.md`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.2/docs/features/utils/named_tuple.md` & `ambient-toolbox-8.3.3/docs/features/utils/named_tuple.md`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.2/docs/features/utils/string.md` & `ambient-toolbox-8.3.3/docs/features/utils/string.md`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.2/docs/features/view-layer.md` & `ambient-toolbox-8.3.3/docs/features/view-layer.md`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.2/docs/index.rst` & `ambient-toolbox-8.3.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.2/docs/make.bat` & `ambient-toolbox-8.3.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.2/manage.py` & `ambient-toolbox-8.3.3/manage.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.2/pyproject.toml` & `ambient-toolbox-8.3.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.2/settings.py` & `ambient-toolbox-8.3.3/settings.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.2/testapp/api/views.py` & `ambient-toolbox-8.3.3/testapp/api/views.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.2/testapp/migrations/0001_initial.py` & `ambient-toolbox-8.3.3/testapp/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.2/testapp/models.py` & `ambient-toolbox-8.3.3/testapp/models.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.2/testapp/templates/403.html` & `ambient-toolbox-8.3.3/testapp/templates/403.html`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.2/tests/admin/model_admin_mixins/test_admin_common_info_mixin.py` & `ambient-toolbox-8.3.3/tests/admin/model_admin_mixins/test_admin_common_info_mixin.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.2/tests/admin/model_admin_mixins/test_admin_create_form_mixin.py` & `ambient-toolbox-8.3.3/tests/admin/model_admin_mixins/test_admin_create_form_mixin.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.2/tests/admin/model_admin_mixins/test_admin_no_inlines_for_create_mixin.py` & `ambient-toolbox-8.3.3/tests/admin/model_admin_mixins/test_admin_no_inlines_for_create_mixin.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.2/tests/admin/model_admin_mixins/test_admin_request_in_form_mixin.py` & `ambient-toolbox-8.3.3/tests/admin/model_admin_mixins/test_admin_request_in_form_mixin.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.2/tests/admin/model_admin_mixins/test_deactivatable_change_view_admin_mixin.py` & `ambient-toolbox-8.3.3/tests/admin/model_admin_mixins/test_deactivatable_change_view_admin_mixin.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.2/tests/admin/model_admin_mixins/test_fetch_object_mixin.py` & `ambient-toolbox-8.3.3/tests/admin/model_admin_mixins/test_fetch_object_mixin.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.2/tests/admin/model_admin_mixins/test_fetch_parent_object_inline_mixin.py` & `ambient-toolbox-8.3.3/tests/admin/model_admin_mixins/test_fetch_parent_object_inline_mixin.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.2/tests/ambient_toolbox/test_test_structure_validator.py` & `ambient-toolbox-8.3.3/tests/ambient_toolbox/test_test_structure_validator.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.2/tests/drf/test_fields.py` & `ambient-toolbox-8.3.3/tests/drf/test_fields.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.2/tests/permissions/fixtures/test_declarations.py` & `ambient-toolbox-8.3.3/tests/permissions/fixtures/test_declarations.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.2/tests/permissions/fixtures/test_helpers.py` & `ambient-toolbox-8.3.3/tests/permissions/fixtures/test_helpers.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.2/tests/permissions/fixtures/test_services_setup_service.py` & `ambient-toolbox-8.3.3/tests/permissions/fixtures/test_services_setup_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         )
 
     def test_init_regular(self):
         group_declaration = GroupPermissionDeclaration(name='my_group', permission_list=[])
         service = PermissionSetupService(group_declaration=group_declaration)
 
         self.assertEqual(service.group_declaration, group_declaration)
-        self.assertTrue(service.dry_run)
+        self.assertFalse(service.dry_run)
 
     def test_process_add_permission(self):
         group_declaration = GroupPermissionDeclaration(
             name='my_group',
             permission_list=[
                 PermissionModelDeclaration(
                     app_label='testapp', codename_list=['change_mysinglesignalmodel'], model='mysinglesignalmodel'
```

### Comparing `ambient-toolbox-8.3.2/tests/permissions/test_install_permission_fixtures_command.py` & `ambient-toolbox-8.3.3/tests/permissions/test_install_permission_fixtures_command.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.2/tests/query_selectors/test_permission.py` & `ambient-toolbox-8.3.3/tests/query_selectors/test_permission.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.2/tests/sentry/mock_data.py` & `ambient-toolbox-8.3.3/tests/sentry/mock_data.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.2/tests/sentry/test_sentry_helper.py` & `ambient-toolbox-8.3.3/tests/sentry/test_sentry_helper.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.2/tests/test_admin_forms.py` & `ambient-toolbox-8.3.3/tests/test_admin_forms.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.2/tests/test_admin_inlines.py` & `ambient-toolbox-8.3.3/tests/test_admin_inlines.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.2/tests/test_admin_model_admins_classes.py` & `ambient-toolbox-8.3.3/tests/test_admin_model_admins_classes.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.2/tests/test_admin_view_mixins.py` & `ambient-toolbox-8.3.3/tests/test_admin_view_mixins.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.2/tests/test_context_manager.py` & `ambient-toolbox-8.3.3/tests/test_context_manager.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.2/tests/test_log_whodid.py` & `ambient-toolbox-8.3.3/tests/test_log_whodid.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.2/tests/test_managers.py` & `ambient-toolbox-8.3.3/tests/test_managers.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.2/tests/test_math.py` & `ambient-toolbox-8.3.3/tests/test_math.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.2/tests/test_middleware.py` & `ambient-toolbox-8.3.3/tests/test_middleware.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.2/tests/test_mixins_models.py` & `ambient-toolbox-8.3.3/tests/test_mixins_models.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.2/tests/test_models.py` & `ambient-toolbox-8.3.3/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.2/tests/test_rest_api_mixins.py` & `ambient-toolbox-8.3.3/tests/test_rest_api_mixins.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.2/tests/test_scrubbing_service.py` & `ambient-toolbox-8.3.3/tests/test_scrubbing_service.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.2/tests/test_utils_date.py` & `ambient-toolbox-8.3.3/tests/test_utils_date.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.2/tests/test_utils_file.py` & `ambient-toolbox-8.3.3/tests/test_utils_file.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.2/tests/test_utils_model.py` & `ambient-toolbox-8.3.3/tests/test_utils_model.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.2/tests/test_utils_named_tuple.py` & `ambient-toolbox-8.3.3/tests/test_utils_named_tuple.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.2/tests/test_utils_string.py` & `ambient-toolbox-8.3.3/tests/test_utils_string.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.2/tests/tests/mixins/test_django_message_framework.py` & `ambient-toolbox-8.3.3/tests/tests/mixins/test_django_message_framework.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.2/tests/tests/mixins/test_request_provider_mixin.py` & `ambient-toolbox-8.3.3/tests/tests/mixins/test_request_provider_mixin.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.2/tests/tests/test_mail_backends.py` & `ambient-toolbox-8.3.3/tests/tests/test_mail_backends.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.2/tests/view_layer/test_formset_mixins.py` & `ambient-toolbox-8.3.3/tests/view_layer/test_formset_mixins.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.2/tests/view_layer/test_htmx_response_mixin.py` & `ambient-toolbox-8.3.3/tests/view_layer/test_htmx_response_mixin.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.2/tests/view_layer/test_meta_mixins.py` & `ambient-toolbox-8.3.3/tests/view_layer/test_meta_mixins.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.2/tests/view_layer/test_views.py` & `ambient-toolbox-8.3.3/tests/view_layer/test_views.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.2/PKG-INFO` & `ambient-toolbox-8.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ambient-toolbox
-Version: 8.3.2
+Version: 8.3.3
 Summary: Python toolbox of Ambient Digital containing an abundance of useful tools and gadgets.
 Author-email: Ambient Digital <hello@ambient.digital>
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 2.2
```

