# Comparing `tmp/ambient-toolbox-8.3.3.tar.gz` & `tmp/ambient-toolbox-8.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ambient-toolbox-8.3.3.tar", last modified: Fri May 12 06:13:57 2023, max compression
+gzip compressed data, was "ambient-toolbox-8.3.4.tar", last modified: Fri May 12 09:03:32 2023, max compression
```

## Comparing `ambient-toolbox-8.3.3.tar` & `ambient-toolbox-8.3.4.tar`

### file list

```diff
@@ -1,220 +1,220 @@
--rw-r--r--   0        0        0     3087 2023-05-09 14:44:04.411372 ambient-toolbox-8.3.3/.ambient-package-update/metadata.py
--rw-r--r--   0        0        0       82 2023-05-10 08:29:28.641744 ambient-toolbox-8.3.3/.coveragerc
--rw-r--r--   0        0        0      288 2023-05-10 08:29:28.641744 ambient-toolbox-8.3.3/.editorconfig
--rw-r--r--   0        0        0     1700 2023-05-10 08:29:28.669738 ambient-toolbox-8.3.3/.github/workflows/ci.yml
--rw-r--r--   0        0        0     3461 2023-05-04 10:28:20.851321 ambient-toolbox-8.3.3/.gitignore
--rw-r--r--   0        0        0     3942 2023-05-04 10:28:20.851321 ambient-toolbox-8.3.3/.gitlab-ci.yml
--rw-r--r--   0        0        0      904 2023-05-12 06:09:33.558023 ambient-toolbox-8.3.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0      551 2023-05-10 08:29:28.641744 ambient-toolbox-8.3.3/.readthedocs.yml
--rw-r--r--   0        0        0    18875 2023-05-12 06:10:25.038287 ambient-toolbox-8.3.3/CHANGES.md
--rw-r--r--   0        0        0      964 2023-05-04 10:28:20.851321 ambient-toolbox-8.3.3/Dockerfile
--rw-r--r--   0        0        0     1107 2023-05-10 08:29:28.641744 ambient-toolbox-8.3.3/LICENSE.md
--rw-r--r--   0        0        0      134 2023-05-10 08:29:28.650251 ambient-toolbox-8.3.3/MANIFEST.in
--rw-r--r--   0        0        0     5853 2023-05-10 08:29:28.665928 ambient-toolbox-8.3.3/README.md
--rw-r--r--   0        0        0      116 2023-05-12 06:10:25.038287 ambient-toolbox-8.3.3/ambient_toolbox/__init__.py
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.851321 ambient-toolbox-8.3.3/ambient_toolbox/admin/__init__.py
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.851321 ambient-toolbox-8.3.3/ambient_toolbox/admin/model_admins/__init__.py
--rw-r--r--   0        0        0     1644 2023-05-04 10:28:20.851321 ambient-toolbox-8.3.3/ambient_toolbox/admin/model_admins/classes.py
--rw-r--r--   0        0        0      824 2023-05-04 10:28:20.851321 ambient-toolbox-8.3.3/ambient_toolbox/admin/model_admins/inlines.py
--rw-r--r--   0        0        0     4623 2023-05-04 10:28:20.851321 ambient-toolbox-8.3.3/ambient_toolbox/admin/model_admins/mixins.py
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.851321 ambient-toolbox-8.3.3/ambient_toolbox/admin/views/__init__.py
--rw-r--r--   0        0        0     1100 2023-05-04 10:28:20.851321 ambient-toolbox-8.3.3/ambient_toolbox/admin/views/forms.py
--rw-r--r--   0        0        0     2427 2023-05-04 10:28:20.851321 ambient-toolbox-8.3.3/ambient_toolbox/admin/views/mixins.py
--rw-r--r--   0        0        0      206 2023-05-04 10:28:20.851321 ambient-toolbox-8.3.3/ambient_toolbox/apps.py
--rw-r--r--   0        0        0      942 2023-05-04 10:28:20.851321 ambient-toolbox-8.3.3/ambient_toolbox/context_manager.py
--rw-r--r--   0        0        0      147 2023-05-04 10:28:20.851321 ambient-toolbox-8.3.3/ambient_toolbox/context_processors.py
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.851321 ambient-toolbox-8.3.3/ambient_toolbox/drf/__init__.py
--rw-r--r--   0        0        0     1031 2023-05-04 10:28:20.851321 ambient-toolbox-8.3.3/ambient_toolbox/drf/fields.py
--rw-r--r--   0        0        0     1143 2023-05-04 10:28:20.851321 ambient-toolbox-8.3.3/ambient_toolbox/drf/serializers.py
--rw-r--r--   0        0        0     3226 2023-05-04 10:28:20.863829 ambient-toolbox-8.3.3/ambient_toolbox/drf/tests.py
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.863829 ambient-toolbox-8.3.3/ambient_toolbox/gitlab/__init__.py
--rw-r--r--   0        0        0     9623 2023-05-04 10:28:20.863829 ambient-toolbox-8.3.3/ambient_toolbox/gitlab/coverage.py
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.863829 ambient-toolbox-8.3.3/ambient_toolbox/graphql/__init__.py
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.863829 ambient-toolbox-8.3.3/ambient_toolbox/graphql/forms/__init__.py
--rw-r--r--   0        0        0     1687 2023-05-04 10:28:20.863829 ambient-toolbox-8.3.3/ambient_toolbox/graphql/forms/mutations.py
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.863829 ambient-toolbox-8.3.3/ambient_toolbox/graphql/schemes/__init__.py
--rw-r--r--   0        0        0     2065 2023-05-04 10:28:20.863829 ambient-toolbox-8.3.3/ambient_toolbox/graphql/schemes/mutations.py
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.863829 ambient-toolbox-8.3.3/ambient_toolbox/graphql/sentry/__init__.py
--rw-r--r--   0        0        0      419 2023-05-04 10:28:20.863829 ambient-toolbox-8.3.3/ambient_toolbox/graphql/sentry/utils.py
--rw-r--r--   0        0        0     1342 2023-05-04 10:28:20.863829 ambient-toolbox-8.3.3/ambient_toolbox/graphql/sentry/views.py
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.863829 ambient-toolbox-8.3.3/ambient_toolbox/graphql/tests/__init__.py
--rw-r--r--   0        0        0     2144 2023-05-04 10:28:20.863829 ambient-toolbox-8.3.3/ambient_toolbox/graphql/tests/base_test.py
--rw-r--r--   0        0        0     1360 2023-05-04 10:28:20.863829 ambient-toolbox-8.3.3/ambient_toolbox/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     2177 2023-05-04 10:28:20.863829 ambient-toolbox-8.3.3/ambient_toolbox/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.863829 ambient-toolbox-8.3.3/ambient_toolbox/mail/__init__.py
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.863829 ambient-toolbox-8.3.3/ambient_toolbox/mail/backends/__init__.py
--rw-r--r--   0        0        0     3226 2023-05-04 10:28:20.863829 ambient-toolbox-8.3.3/ambient_toolbox/mail/backends/whitelist_smtp.py
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.863829 ambient-toolbox-8.3.3/ambient_toolbox/management/__init__.py
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.863829 ambient-toolbox-8.3.3/ambient_toolbox/management/commands/__init__.py
--rw-r--r--   0        0        0     1745 2023-05-11 17:08:22.645616 ambient-toolbox-8.3.3/ambient_toolbox/management/commands/install_permission_fixtures.py
--rw-r--r--   0        0        0      303 2023-05-04 10:28:20.863829 ambient-toolbox-8.3.3/ambient_toolbox/management/commands/validate_test_structure.py
--rw-r--r--   0        0        0     2550 2023-05-04 10:28:20.863829 ambient-toolbox-8.3.3/ambient_toolbox/managers.py
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.863829 ambient-toolbox-8.3.3/ambient_toolbox/middleware/__init__.py
--rw-r--r--   0        0        0     1050 2023-05-04 10:28:20.863829 ambient-toolbox-8.3.3/ambient_toolbox/middleware/current_user.py
--rw-r--r--   0        0        0       31 2023-05-04 10:28:20.863829 ambient-toolbox-8.3.3/ambient_toolbox/mixins/__init__.py
--rw-r--r--   0        0        0     1958 2023-05-04 10:28:20.863829 ambient-toolbox-8.3.3/ambient_toolbox/mixins/bleacher.py
--rw-r--r--   0        0        0     1378 2023-05-04 10:28:20.863829 ambient-toolbox-8.3.3/ambient_toolbox/mixins/models.py
--rw-r--r--   0        0        0      246 2023-05-04 10:28:20.863829 ambient-toolbox-8.3.3/ambient_toolbox/mixins/validation.py
--rw-r--r--   0        0        0     2592 2023-05-04 10:28:20.863829 ambient-toolbox-8.3.3/ambient_toolbox/models.py
--rw-r--r--   0        0        0        0 2023-05-11 13:43:18.462606 ambient-toolbox-8.3.3/ambient_toolbox/permissions/__init__.py
--rw-r--r--   0        0        0        0 2023-05-11 13:46:58.441382 ambient-toolbox-8.3.3/ambient_toolbox/permissions/fixtures/__init__.py
--rw-r--r--   0        0        0      292 2023-05-11 17:30:53.043646 ambient-toolbox-8.3.3/ambient_toolbox/permissions/fixtures/declarations.py
--rw-r--r--   0        0        0      232 2023-05-12 06:07:29.953470 ambient-toolbox-8.3.3/ambient_toolbox/permissions/fixtures/helpers.py
--rw-r--r--   0        0        0     3116 2023-05-12 06:08:39.395472 ambient-toolbox-8.3.3/ambient_toolbox/permissions/fixtures/services.py
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.863829 ambient-toolbox-8.3.3/ambient_toolbox/selectors/__init__.py
--rw-r--r--   0        0        0      362 2023-05-04 10:28:20.863829 ambient-toolbox-8.3.3/ambient_toolbox/selectors/base.py
--rw-r--r--   0        0        0     1061 2023-05-04 10:28:20.863829 ambient-toolbox-8.3.3/ambient_toolbox/selectors/permission.py
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.863829 ambient-toolbox-8.3.3/ambient_toolbox/sentry/__init__.py
--rw-r--r--   0        0        0     2155 2023-05-09 14:45:08.006243 ambient-toolbox-8.3.3/ambient_toolbox/sentry/helpers.py
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.863829 ambient-toolbox-8.3.3/ambient_toolbox/services/__init__.py
--rw-r--r--   0        0        0     3223 2023-05-04 10:28:20.863829 ambient-toolbox-8.3.3/ambient_toolbox/services/custom_scrubber.py
--rw-r--r--   0        0        0       31 2023-05-04 10:28:20.863829 ambient-toolbox-8.3.3/ambient_toolbox/templatetags/__init__.py
--rw-r--r--   0        0        0      244 2023-05-04 10:28:20.863829 ambient-toolbox-8.3.3/ambient_toolbox/templatetags/ai_date_tags.py
--rw-r--r--   0        0        0      675 2023-05-04 10:28:20.879472 ambient-toolbox-8.3.3/ambient_toolbox/templatetags/ai_email_tags.py
--rw-r--r--   0        0        0      807 2023-05-04 10:28:20.879472 ambient-toolbox-8.3.3/ambient_toolbox/templatetags/ai_file_tags.py
--rw-r--r--   0        0        0      194 2023-05-04 10:28:20.879472 ambient-toolbox-8.3.3/ambient_toolbox/templatetags/ai_helper_tags.py
--rw-r--r--   0        0        0     1375 2023-05-04 10:28:20.879472 ambient-toolbox-8.3.3/ambient_toolbox/templatetags/ai_number_tags.py
--rw-r--r--   0        0        0      384 2023-05-04 10:28:20.879472 ambient-toolbox-8.3.3/ambient_toolbox/templatetags/ai_object_tags.py
--rw-r--r--   0        0        0      654 2023-05-04 10:28:20.879472 ambient-toolbox-8.3.3/ambient_toolbox/templatetags/ai_string_tags.py
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.879472 ambient-toolbox-8.3.3/ambient_toolbox/tests/__init__.py
--rw-r--r--   0        0        0       60 2023-05-04 10:28:20.879472 ambient-toolbox-8.3.3/ambient_toolbox/tests/errors.py
--rw-r--r--   0        0        0     5145 2023-05-04 10:28:20.879472 ambient-toolbox-8.3.3/ambient_toolbox/tests/mixins.py
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.879472 ambient-toolbox-8.3.3/ambient_toolbox/tests/structure_validator/__init__.py
--rw-r--r--   0        0        0      397 2023-05-04 10:28:20.879472 ambient-toolbox-8.3.3/ambient_toolbox/tests/structure_validator/settings.py
--rw-r--r--   0        0        0     4634 2023-05-04 10:28:20.883484 ambient-toolbox-8.3.3/ambient_toolbox/tests/structure_validator/test_structure_validator.py
--rw-r--r--   0        0        0      261 2023-05-04 10:28:20.883484 ambient-toolbox-8.3.3/ambient_toolbox/utils/__init__.py
--rw-r--r--   0        0        0      127 2023-05-04 10:28:20.883484 ambient-toolbox-8.3.3/ambient_toolbox/utils/cache.py
--rw-r--r--   0        0        0     5971 2023-05-04 10:28:20.883484 ambient-toolbox-8.3.3/ambient_toolbox/utils/date.py
--rw-r--r--   0        0        0     1469 2023-05-04 10:28:20.883484 ambient-toolbox-8.3.3/ambient_toolbox/utils/file.py
--rw-r--r--   0        0        0      343 2023-05-04 10:28:20.883484 ambient-toolbox-8.3.3/ambient_toolbox/utils/log_whodid.py
--rw-r--r--   0        0        0      574 2023-05-04 10:28:20.883484 ambient-toolbox-8.3.3/ambient_toolbox/utils/math.py
--rw-r--r--   0        0        0      935 2023-05-04 10:28:20.883484 ambient-toolbox-8.3.3/ambient_toolbox/utils/model.py
--rw-r--r--   0        0        0     3970 2023-05-04 10:28:20.883484 ambient-toolbox-8.3.3/ambient_toolbox/utils/named_tuple.py
--rw-r--r--   0        0        0     3804 2023-05-04 10:28:20.883484 ambient-toolbox-8.3.3/ambient_toolbox/utils/string.py
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.883484 ambient-toolbox-8.3.3/ambient_toolbox/view_layer/__init__.py
--rw-r--r--   0        0        0      750 2023-05-04 10:28:20.883484 ambient-toolbox-8.3.3/ambient_toolbox/view_layer/form_mixins.py
--rw-r--r--   0        0        0      485 2023-05-04 10:28:20.883484 ambient-toolbox-8.3.3/ambient_toolbox/view_layer/formset_mixins.py
--rw-r--r--   0        0        0     2998 2023-05-04 10:28:20.883484 ambient-toolbox-8.3.3/ambient_toolbox/view_layer/formset_view_mixin.py
--rw-r--r--   0        0        0     1585 2023-05-04 10:28:20.883484 ambient-toolbox-8.3.3/ambient_toolbox/view_layer/htmx_mixins.py
--rw-r--r--   0        0        0     2110 2023-05-04 10:28:20.883484 ambient-toolbox-8.3.3/ambient_toolbox/view_layer/mixins.py
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.883484 ambient-toolbox-8.3.3/ambient_toolbox/view_layer/tests/__init__.py
--rw-r--r--   0        0        0     4124 2023-05-04 10:28:20.883484 ambient-toolbox-8.3.3/ambient_toolbox/view_layer/tests/mixins.py
--rw-r--r--   0        0        0     1882 2023-05-04 10:28:20.883484 ambient-toolbox-8.3.3/ambient_toolbox/view_layer/views.py
--rw-r--r--   0        0        0      654 2023-05-10 08:29:28.674940 ambient-toolbox-8.3.3/docs/Makefile
--rw-r--r--   0        0        0     2803 2023-05-10 08:29:28.671819 ambient-toolbox-8.3.3/docs/conf.py
--rw-r--r--   0        0        0     6731 2023-05-04 10:28:20.883484 ambient-toolbox-8.3.3/docs/features/admin.md
--rw-r--r--   0        0        0       35 2023-05-04 10:28:20.883484 ambient-toolbox-8.3.3/docs/features/changelog.rst
--rw-r--r--   0        0        0     2313 2023-05-04 10:28:20.883484 ambient-toolbox-8.3.3/docs/features/context_manager.md
--rw-r--r--   0        0        0      549 2023-05-04 10:28:20.883484 ambient-toolbox-8.3.3/docs/features/context_processors.md
--rw-r--r--   0        0        0     7273 2023-05-04 10:28:20.883484 ambient-toolbox-8.3.3/docs/features/database_anonymisation.md
--rw-r--r--   0        0        0     6807 2023-05-04 10:28:20.883484 ambient-toolbox-8.3.3/docs/features/djangorestframework.md
--rw-r--r--   0        0        0     2554 2023-05-04 10:28:20.883484 ambient-toolbox-8.3.3/docs/features/gitlab.md
--rw-r--r--   0        0        0     6567 2023-05-04 10:28:20.883484 ambient-toolbox-8.3.3/docs/features/graphql.md
--rw-r--r--   0        0        0     1020 2023-05-04 10:28:20.895496 ambient-toolbox-8.3.3/docs/features/mail.md
--rw-r--r--   0        0        0     5891 2023-05-04 10:28:20.895496 ambient-toolbox-8.3.3/docs/features/managers.md
--rw-r--r--   0        0        0     5951 2023-05-04 10:28:20.895496 ambient-toolbox-8.3.3/docs/features/mixins.md
--rw-r--r--   0        0        0     1553 2023-05-04 10:28:20.895496 ambient-toolbox-8.3.3/docs/features/models.md
--rw-r--r--   0        0        0     5637 2023-05-11 17:22:39.859059 ambient-toolbox-8.3.3/docs/features/permissions.md
--rw-r--r--   0        0        0     4454 2023-05-04 10:28:20.895496 ambient-toolbox-8.3.3/docs/features/selectors.md
--rw-r--r--   0        0        0     3290 2023-05-09 14:44:04.411372 ambient-toolbox-8.3.3/docs/features/sentry.md
--rw-r--r--   0        0        0     4978 2023-05-04 10:28:20.895496 ambient-toolbox-8.3.3/docs/features/services.md
--rw-r--r--   0        0        0     1574 2023-05-04 10:28:20.895496 ambient-toolbox-8.3.3/docs/features/setup.md
--rw-r--r--   0        0        0     5338 2023-05-04 10:28:20.895496 ambient-toolbox-8.3.3/docs/features/tests.md
--rw-r--r--   0        0        0      232 2023-05-04 10:28:20.895496 ambient-toolbox-8.3.3/docs/features/utils.rst
--rw-r--r--   0        0        0      527 2023-05-04 10:28:20.895496 ambient-toolbox-8.3.3/docs/features/utils/cache.md
--rw-r--r--   0        0        0     7417 2023-05-04 10:28:20.895496 ambient-toolbox-8.3.3/docs/features/utils/date.md
--rw-r--r--   0        0        0      737 2023-05-04 10:28:20.895496 ambient-toolbox-8.3.3/docs/features/utils/math.md
--rw-r--r--   0        0        0     1100 2023-05-04 10:28:20.895496 ambient-toolbox-8.3.3/docs/features/utils/model.md
--rw-r--r--   0        0        0     2405 2023-05-04 10:28:20.895496 ambient-toolbox-8.3.3/docs/features/utils/named_tuple.md
--rw-r--r--   0        0        0     5861 2023-05-04 10:28:20.895496 ambient-toolbox-8.3.3/docs/features/utils/string.md
--rw-r--r--   0        0        0    15067 2023-05-04 10:28:20.895496 ambient-toolbox-8.3.3/docs/features/view-layer.md
--rw-r--r--   0        0        0     1142 2023-05-11 16:39:56.593947 ambient-toolbox-8.3.3/docs/index.rst
--rwxr-xr-x   0        0        0      795 2023-05-10 08:29:28.673380 ambient-toolbox-8.3.3/docs/make.bat
--rw-r--r--   0        0        0      677 2023-05-04 10:28:20.895496 ambient-toolbox-8.3.3/manage.py
--rw-r--r--   0        0        0     4100 2023-05-10 08:29:28.650251 ambient-toolbox-8.3.3/pyproject.toml
--rw-r--r--   0        0        0       56 2023-05-04 10:28:20.895496 ambient-toolbox-8.3.3/pytest.ini
--rw-r--r--   0        0        0       56 2023-05-10 08:29:28.650251 ambient-toolbox-8.3.3/pytest.init
--rw-r--r--   0        0        0       50 2023-05-10 08:29:28.676006 ambient-toolbox-8.3.3/scripts/publish_to_pypi.ps1
--rw-r--r--   0        0        0       50 2023-05-10 08:29:28.677568 ambient-toolbox-8.3.3/scripts/publish_to_pypi.sh
--rw-r--r--   0        0        0     1704 2023-05-11 16:23:28.767887 ambient-toolbox-8.3.3/settings.py
--rw-r--r--   0        0        0       69 2023-05-10 08:29:28.667948 ambient-toolbox-8.3.3/setup.cfg
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.895496 ambient-toolbox-8.3.3/testapp/__init__.py
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.895496 ambient-toolbox-8.3.3/testapp/api/__init__.py
--rw-r--r--   0        0        0      287 2023-05-04 10:28:20.895496 ambient-toolbox-8.3.3/testapp/api/serializers.py
--rw-r--r--   0        0        0      257 2023-05-04 10:28:20.895496 ambient-toolbox-8.3.3/testapp/api/urls.py
--rw-r--r--   0        0        0      524 2023-05-04 10:28:20.895496 ambient-toolbox-8.3.3/testapp/api/views.py
--rw-r--r--   0        0        0      219 2023-05-04 10:28:20.895496 ambient-toolbox-8.3.3/testapp/forms.py
--rw-r--r--   0        0        0       97 2023-05-04 10:28:20.895496 ambient-toolbox-8.3.3/testapp/managers.py
--rw-r--r--   0        0        0     6151 2023-05-04 10:28:20.895496 ambient-toolbox-8.3.3/testapp/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.895496 ambient-toolbox-8.3.3/testapp/migrations/__init__.py
--rw-r--r--   0        0        0     3363 2023-05-04 10:28:20.895496 ambient-toolbox-8.3.3/testapp/models.py
--rw-r--r--   0        0        0      406 2023-05-11 17:08:22.631636 ambient-toolbox-8.3.3/testapp/permissions.py
--rw-r--r--   0        0        0      162 2023-05-04 10:28:20.895496 ambient-toolbox-8.3.3/testapp/selectors.py
--rw-r--r--   0        0        0     1449 2023-05-04 10:28:20.895496 ambient-toolbox-8.3.3/testapp/templates/403.html
--rw-r--r--   0        0        0      145 2023-05-04 10:28:20.895496 ambient-toolbox-8.3.3/testapp/templates/testapp/test_template.html
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.895496 ambient-toolbox-8.3.3/testapp/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.895496 ambient-toolbox-8.3.3/testapp/tests/missing_init/test_ok.py
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.895496 ambient-toolbox-8.3.3/testapp/tests/subdirectory/__init__.py
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.3/testapp/tests/subdirectory/missing_test_prefix.py
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.3/testapp/tests/subdirectory/test_ok.py
--rw-r--r--   0        0        0      382 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.3/testapp/urls.py
--rw-r--r--   0        0        0      505 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.3/testapp/views.py
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.3/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.3/tests/admin/__init__.py
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.3/tests/admin/model_admin_mixins/__init__.py
--rw-r--r--   0        0        0     2607 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.3/tests/admin/model_admin_mixins/test_admin_common_info_mixin.py
--rw-r--r--   0        0        0     1900 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.3/tests/admin/model_admin_mixins/test_admin_create_form_mixin.py
--rw-r--r--   0        0        0     1683 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.3/tests/admin/model_admin_mixins/test_admin_no_inlines_for_create_mixin.py
--rw-r--r--   0        0        0     1184 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.3/tests/admin/model_admin_mixins/test_admin_request_in_form_mixin.py
--rw-r--r--   0        0        0     3871 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.3/tests/admin/model_admin_mixins/test_deactivatable_change_view_admin_mixin.py
--rw-r--r--   0        0        0     1492 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.3/tests/admin/model_admin_mixins/test_fetch_object_mixin.py
--rw-r--r--   0        0        0     1909 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.3/tests/admin/model_admin_mixins/test_fetch_parent_object_inline_mixin.py
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.3/tests/ambient_toolbox/__init__.py
--rw-r--r--   0        0        0     7503 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.3/tests/ambient_toolbox/test_test_structure_validator.py
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.3/tests/drf/__init__.py
--rw-r--r--   0        0        0     2579 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.3/tests/drf/test_fields.py
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.3/tests/mixins/__init__.py
--rw-r--r--   0        0        0      364 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.3/tests/mixins/validation.py
--rw-r--r--   0        0        0        0 2023-05-11 13:44:55.711963 ambient-toolbox-8.3.3/tests/permissions/__init__.py
--rw-r--r--   0        0        0        0 2023-05-11 13:47:09.381858 ambient-toolbox-8.3.3/tests/permissions/fixtures/__init__.py
--rw-r--r--   0        0        0     1064 2023-05-11 13:57:05.255995 ambient-toolbox-8.3.3/tests/permissions/fixtures/test_declarations.py
--rw-r--r--   0        0        0      564 2023-05-11 13:57:05.238632 ambient-toolbox-8.3.3/tests/permissions/fixtures/test_helpers.py
--rw-r--r--   0        0        0     7053 2023-05-11 17:28:06.152820 ambient-toolbox-8.3.3/tests/permissions/fixtures/test_services_setup_service.py
--rw-r--r--   0        0        0      963 2023-05-11 17:08:22.645616 ambient-toolbox-8.3.3/tests/permissions/test_install_permission_fixtures_command.py
--rw-r--r--   0        0        0      499 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.3/tests/query_selectors/test_base.py
--rw-r--r--   0        0        0     1631 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.3/tests/query_selectors/test_permission.py
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.3/tests/selectors/__init__.py
--rw-r--r--   0        0        0        0 2023-05-09 14:44:04.427021 ambient-toolbox-8.3.3/tests/sentry/__init__.py
--rw-r--r--   0        0        0     6196 2023-05-09 14:44:04.427021 ambient-toolbox-8.3.3/tests/sentry/mock_data.py
--rw-r--r--   0        0        0     1583 2023-05-09 14:44:04.427021 ambient-toolbox-8.3.3/tests/sentry/test_sentry_helper.py
--rw-r--r--   0        0        0      553 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.3/tests/test_admin_forms.py
--rw-r--r--   0        0        0     1612 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.3/tests/test_admin_inlines.py
--rw-r--r--   0        0        0     2651 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.3/tests/test_admin_model_admins_classes.py
--rw-r--r--   0        0        0     2899 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.3/tests/test_admin_view_mixins.py
--rw-r--r--   0        0        0     2218 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.3/tests/test_context_manager.py
--rw-r--r--   0        0        0      822 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.3/tests/test_log_whodid.py
--rw-r--r--   0        0        0     1169 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.3/tests/test_managers.py
--rw-r--r--   0        0        0     1628 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.3/tests/test_math.py
--rw-r--r--   0        0        0     2593 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.3/tests/test_middleware.py
--rw-r--r--   0        0        0     1200 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.3/tests/test_mixins_models.py
--rw-r--r--   0        0        0     1669 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.3/tests/test_models.py
--rw-r--r--   0        0        0     1780 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.3/tests/test_rest_api_mixins.py
--rw-r--r--   0        0        0      664 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.3/tests/test_scrubbing_service.py
--rw-r--r--   0        0        0      289 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.3/tests/test_utils_cache.py
--rw-r--r--   0        0        0    12741 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.3/tests/test_utils_date.py
--rw-r--r--   0        0        0     1593 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.3/tests/test_utils_file.py
--rw-r--r--   0        0        0      933 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.3/tests/test_utils_model.py
--rw-r--r--   0        0        0     3807 2023-05-04 10:28:20.926757 ambient-toolbox-8.3.3/tests/test_utils_named_tuple.py
--rw-r--r--   0        0        0     5343 2023-05-04 10:28:20.926757 ambient-toolbox-8.3.3/tests/test_utils_string.py
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.926757 ambient-toolbox-8.3.3/tests/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.926757 ambient-toolbox-8.3.3/tests/tests/mixins/__init__.py
--rw-r--r--   0        0        0      371 2023-05-04 10:28:20.926757 ambient-toolbox-8.3.3/tests/tests/mixins/models.py
--rw-r--r--   0        0        0      817 2023-05-04 10:28:20.926757 ambient-toolbox-8.3.3/tests/tests/mixins/test_django_message_framework.py
--rw-r--r--   0        0        0     2483 2023-05-04 10:28:20.926757 ambient-toolbox-8.3.3/tests/tests/mixins/test_request_provider_mixin.py
--rw-r--r--   0        0        0     2057 2023-05-04 10:28:20.926757 ambient-toolbox-8.3.3/tests/tests/test_mail_backends.py
--rw-r--r--   0        0        0        0 2023-05-04 10:28:20.926757 ambient-toolbox-8.3.3/tests/view_layer/__init__.py
--rw-r--r--   0        0        0     1891 2023-05-04 10:28:20.926757 ambient-toolbox-8.3.3/tests/view_layer/test_formset_mixins.py
--rw-r--r--   0        0        0     1564 2023-05-04 10:28:20.926757 ambient-toolbox-8.3.3/tests/view_layer/test_htmx_response_mixin.py
--rw-r--r--   0        0        0     3458 2023-05-04 10:28:20.926757 ambient-toolbox-8.3.3/tests/view_layer/test_meta_mixins.py
--rw-r--r--   0        0        0     1361 2023-05-04 10:28:20.926757 ambient-toolbox-8.3.3/tests/view_layer/test_views.py
--rw-r--r--   0        0        0     8311 1970-01-01 00:00:00.000000 ambient-toolbox-8.3.3/PKG-INFO
+-rw-r--r--   0        0        0     3087 2023-05-09 14:44:04.411372 ambient-toolbox-8.3.4/.ambient-package-update/metadata.py
+-rw-r--r--   0        0        0       82 2023-05-10 08:29:28.641744 ambient-toolbox-8.3.4/.coveragerc
+-rw-r--r--   0        0        0      288 2023-05-10 08:29:28.641744 ambient-toolbox-8.3.4/.editorconfig
+-rw-r--r--   0        0        0     1700 2023-05-10 08:29:28.669738 ambient-toolbox-8.3.4/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     3461 2023-05-04 10:28:20.851321 ambient-toolbox-8.3.4/.gitignore
+-rw-r--r--   0        0        0     3942 2023-05-04 10:28:20.851321 ambient-toolbox-8.3.4/.gitlab-ci.yml
+-rw-r--r--   0        0        0      904 2023-05-12 06:09:33.558023 ambient-toolbox-8.3.4/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      551 2023-05-10 08:29:28.641744 ambient-toolbox-8.3.4/.readthedocs.yml
+-rw-r--r--   0        0        0    18964 2023-05-12 07:05:14.151973 ambient-toolbox-8.3.4/CHANGES.md
+-rw-r--r--   0        0        0      964 2023-05-04 10:28:20.851321 ambient-toolbox-8.3.4/Dockerfile
+-rw-r--r--   0        0        0     1107 2023-05-10 08:29:28.641744 ambient-toolbox-8.3.4/LICENSE.md
+-rw-r--r--   0        0        0      134 2023-05-10 08:29:28.650251 ambient-toolbox-8.3.4/MANIFEST.in
+-rw-r--r--   0        0        0     5853 2023-05-10 08:29:28.665928 ambient-toolbox-8.3.4/README.md
+-rw-r--r--   0        0        0      116 2023-05-12 07:05:14.158110 ambient-toolbox-8.3.4/ambient_toolbox/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.851321 ambient-toolbox-8.3.4/ambient_toolbox/admin/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.851321 ambient-toolbox-8.3.4/ambient_toolbox/admin/model_admins/__init__.py
+-rw-r--r--   0        0        0     1644 2023-05-04 10:28:20.851321 ambient-toolbox-8.3.4/ambient_toolbox/admin/model_admins/classes.py
+-rw-r--r--   0        0        0      824 2023-05-04 10:28:20.851321 ambient-toolbox-8.3.4/ambient_toolbox/admin/model_admins/inlines.py
+-rw-r--r--   0        0        0     4623 2023-05-04 10:28:20.851321 ambient-toolbox-8.3.4/ambient_toolbox/admin/model_admins/mixins.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.851321 ambient-toolbox-8.3.4/ambient_toolbox/admin/views/__init__.py
+-rw-r--r--   0        0        0     1100 2023-05-04 10:28:20.851321 ambient-toolbox-8.3.4/ambient_toolbox/admin/views/forms.py
+-rw-r--r--   0        0        0     2427 2023-05-04 10:28:20.851321 ambient-toolbox-8.3.4/ambient_toolbox/admin/views/mixins.py
+-rw-r--r--   0        0        0      206 2023-05-04 10:28:20.851321 ambient-toolbox-8.3.4/ambient_toolbox/apps.py
+-rw-r--r--   0        0        0      942 2023-05-04 10:28:20.851321 ambient-toolbox-8.3.4/ambient_toolbox/context_manager.py
+-rw-r--r--   0        0        0      147 2023-05-04 10:28:20.851321 ambient-toolbox-8.3.4/ambient_toolbox/context_processors.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.851321 ambient-toolbox-8.3.4/ambient_toolbox/drf/__init__.py
+-rw-r--r--   0        0        0     1031 2023-05-04 10:28:20.851321 ambient-toolbox-8.3.4/ambient_toolbox/drf/fields.py
+-rw-r--r--   0        0        0     1143 2023-05-04 10:28:20.851321 ambient-toolbox-8.3.4/ambient_toolbox/drf/serializers.py
+-rw-r--r--   0        0        0     3226 2023-05-04 10:28:20.863829 ambient-toolbox-8.3.4/ambient_toolbox/drf/tests.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.863829 ambient-toolbox-8.3.4/ambient_toolbox/gitlab/__init__.py
+-rw-r--r--   0        0        0     9623 2023-05-04 10:28:20.863829 ambient-toolbox-8.3.4/ambient_toolbox/gitlab/coverage.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.863829 ambient-toolbox-8.3.4/ambient_toolbox/graphql/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.863829 ambient-toolbox-8.3.4/ambient_toolbox/graphql/forms/__init__.py
+-rw-r--r--   0        0        0     1687 2023-05-04 10:28:20.863829 ambient-toolbox-8.3.4/ambient_toolbox/graphql/forms/mutations.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.863829 ambient-toolbox-8.3.4/ambient_toolbox/graphql/schemes/__init__.py
+-rw-r--r--   0        0        0     2065 2023-05-04 10:28:20.863829 ambient-toolbox-8.3.4/ambient_toolbox/graphql/schemes/mutations.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.863829 ambient-toolbox-8.3.4/ambient_toolbox/graphql/sentry/__init__.py
+-rw-r--r--   0        0        0      419 2023-05-04 10:28:20.863829 ambient-toolbox-8.3.4/ambient_toolbox/graphql/sentry/utils.py
+-rw-r--r--   0        0        0     1342 2023-05-04 10:28:20.863829 ambient-toolbox-8.3.4/ambient_toolbox/graphql/sentry/views.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.863829 ambient-toolbox-8.3.4/ambient_toolbox/graphql/tests/__init__.py
+-rw-r--r--   0        0        0     2144 2023-05-04 10:28:20.863829 ambient-toolbox-8.3.4/ambient_toolbox/graphql/tests/base_test.py
+-rw-r--r--   0        0        0     1360 2023-05-04 10:28:20.863829 ambient-toolbox-8.3.4/ambient_toolbox/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     2177 2023-05-04 10:28:20.863829 ambient-toolbox-8.3.4/ambient_toolbox/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.863829 ambient-toolbox-8.3.4/ambient_toolbox/mail/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.863829 ambient-toolbox-8.3.4/ambient_toolbox/mail/backends/__init__.py
+-rw-r--r--   0        0        0     3226 2023-05-04 10:28:20.863829 ambient-toolbox-8.3.4/ambient_toolbox/mail/backends/whitelist_smtp.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.863829 ambient-toolbox-8.3.4/ambient_toolbox/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.863829 ambient-toolbox-8.3.4/ambient_toolbox/management/commands/__init__.py
+-rw-r--r--   0        0        0     1789 2023-05-12 07:03:57.505757 ambient-toolbox-8.3.4/ambient_toolbox/management/commands/install_permission_fixtures.py
+-rw-r--r--   0        0        0      303 2023-05-04 10:28:20.863829 ambient-toolbox-8.3.4/ambient_toolbox/management/commands/validate_test_structure.py
+-rw-r--r--   0        0        0     2550 2023-05-04 10:28:20.863829 ambient-toolbox-8.3.4/ambient_toolbox/managers.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.863829 ambient-toolbox-8.3.4/ambient_toolbox/middleware/__init__.py
+-rw-r--r--   0        0        0     1050 2023-05-04 10:28:20.863829 ambient-toolbox-8.3.4/ambient_toolbox/middleware/current_user.py
+-rw-r--r--   0        0        0       31 2023-05-04 10:28:20.863829 ambient-toolbox-8.3.4/ambient_toolbox/mixins/__init__.py
+-rw-r--r--   0        0        0     1958 2023-05-04 10:28:20.863829 ambient-toolbox-8.3.4/ambient_toolbox/mixins/bleacher.py
+-rw-r--r--   0        0        0     1378 2023-05-04 10:28:20.863829 ambient-toolbox-8.3.4/ambient_toolbox/mixins/models.py
+-rw-r--r--   0        0        0      246 2023-05-04 10:28:20.863829 ambient-toolbox-8.3.4/ambient_toolbox/mixins/validation.py
+-rw-r--r--   0        0        0     2592 2023-05-04 10:28:20.863829 ambient-toolbox-8.3.4/ambient_toolbox/models.py
+-rw-r--r--   0        0        0        0 2023-05-12 07:03:57.505757 ambient-toolbox-8.3.4/ambient_toolbox/permissions/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-12 07:03:57.505757 ambient-toolbox-8.3.4/ambient_toolbox/permissions/fixtures/__init__.py
+-rw-r--r--   0        0        0      307 2023-05-12 07:03:57.505757 ambient-toolbox-8.3.4/ambient_toolbox/permissions/fixtures/declarations.py
+-rw-r--r--   0        0        0      242 2023-05-12 07:03:57.505757 ambient-toolbox-8.3.4/ambient_toolbox/permissions/fixtures/helpers.py
+-rw-r--r--   0        0        0     3189 2023-05-12 07:03:57.505757 ambient-toolbox-8.3.4/ambient_toolbox/permissions/fixtures/services.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.863829 ambient-toolbox-8.3.4/ambient_toolbox/selectors/__init__.py
+-rw-r--r--   0        0        0      362 2023-05-04 10:28:20.863829 ambient-toolbox-8.3.4/ambient_toolbox/selectors/base.py
+-rw-r--r--   0        0        0     1061 2023-05-04 10:28:20.863829 ambient-toolbox-8.3.4/ambient_toolbox/selectors/permission.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.863829 ambient-toolbox-8.3.4/ambient_toolbox/sentry/__init__.py
+-rw-r--r--   0        0        0     2155 2023-05-09 14:45:08.006243 ambient-toolbox-8.3.4/ambient_toolbox/sentry/helpers.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.863829 ambient-toolbox-8.3.4/ambient_toolbox/services/__init__.py
+-rw-r--r--   0        0        0     3223 2023-05-04 10:28:20.863829 ambient-toolbox-8.3.4/ambient_toolbox/services/custom_scrubber.py
+-rw-r--r--   0        0        0       31 2023-05-04 10:28:20.863829 ambient-toolbox-8.3.4/ambient_toolbox/templatetags/__init__.py
+-rw-r--r--   0        0        0      244 2023-05-04 10:28:20.863829 ambient-toolbox-8.3.4/ambient_toolbox/templatetags/ai_date_tags.py
+-rw-r--r--   0        0        0      675 2023-05-04 10:28:20.879472 ambient-toolbox-8.3.4/ambient_toolbox/templatetags/ai_email_tags.py
+-rw-r--r--   0        0        0      807 2023-05-04 10:28:20.879472 ambient-toolbox-8.3.4/ambient_toolbox/templatetags/ai_file_tags.py
+-rw-r--r--   0        0        0      194 2023-05-04 10:28:20.879472 ambient-toolbox-8.3.4/ambient_toolbox/templatetags/ai_helper_tags.py
+-rw-r--r--   0        0        0     1375 2023-05-04 10:28:20.879472 ambient-toolbox-8.3.4/ambient_toolbox/templatetags/ai_number_tags.py
+-rw-r--r--   0        0        0      384 2023-05-04 10:28:20.879472 ambient-toolbox-8.3.4/ambient_toolbox/templatetags/ai_object_tags.py
+-rw-r--r--   0        0        0      654 2023-05-04 10:28:20.879472 ambient-toolbox-8.3.4/ambient_toolbox/templatetags/ai_string_tags.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.879472 ambient-toolbox-8.3.4/ambient_toolbox/tests/__init__.py
+-rw-r--r--   0        0        0       60 2023-05-04 10:28:20.879472 ambient-toolbox-8.3.4/ambient_toolbox/tests/errors.py
+-rw-r--r--   0        0        0     5145 2023-05-04 10:28:20.879472 ambient-toolbox-8.3.4/ambient_toolbox/tests/mixins.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.879472 ambient-toolbox-8.3.4/ambient_toolbox/tests/structure_validator/__init__.py
+-rw-r--r--   0        0        0      397 2023-05-04 10:28:20.879472 ambient-toolbox-8.3.4/ambient_toolbox/tests/structure_validator/settings.py
+-rw-r--r--   0        0        0     4634 2023-05-04 10:28:20.883484 ambient-toolbox-8.3.4/ambient_toolbox/tests/structure_validator/test_structure_validator.py
+-rw-r--r--   0        0        0      261 2023-05-04 10:28:20.883484 ambient-toolbox-8.3.4/ambient_toolbox/utils/__init__.py
+-rw-r--r--   0        0        0      127 2023-05-04 10:28:20.883484 ambient-toolbox-8.3.4/ambient_toolbox/utils/cache.py
+-rw-r--r--   0        0        0     5971 2023-05-04 10:28:20.883484 ambient-toolbox-8.3.4/ambient_toolbox/utils/date.py
+-rw-r--r--   0        0        0     1469 2023-05-04 10:28:20.883484 ambient-toolbox-8.3.4/ambient_toolbox/utils/file.py
+-rw-r--r--   0        0        0      343 2023-05-04 10:28:20.883484 ambient-toolbox-8.3.4/ambient_toolbox/utils/log_whodid.py
+-rw-r--r--   0        0        0      574 2023-05-04 10:28:20.883484 ambient-toolbox-8.3.4/ambient_toolbox/utils/math.py
+-rw-r--r--   0        0        0      935 2023-05-04 10:28:20.883484 ambient-toolbox-8.3.4/ambient_toolbox/utils/model.py
+-rw-r--r--   0        0        0     3970 2023-05-04 10:28:20.883484 ambient-toolbox-8.3.4/ambient_toolbox/utils/named_tuple.py
+-rw-r--r--   0        0        0     3804 2023-05-04 10:28:20.883484 ambient-toolbox-8.3.4/ambient_toolbox/utils/string.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.883484 ambient-toolbox-8.3.4/ambient_toolbox/view_layer/__init__.py
+-rw-r--r--   0        0        0      750 2023-05-04 10:28:20.883484 ambient-toolbox-8.3.4/ambient_toolbox/view_layer/form_mixins.py
+-rw-r--r--   0        0        0      485 2023-05-04 10:28:20.883484 ambient-toolbox-8.3.4/ambient_toolbox/view_layer/formset_mixins.py
+-rw-r--r--   0        0        0     2998 2023-05-04 10:28:20.883484 ambient-toolbox-8.3.4/ambient_toolbox/view_layer/formset_view_mixin.py
+-rw-r--r--   0        0        0     1585 2023-05-04 10:28:20.883484 ambient-toolbox-8.3.4/ambient_toolbox/view_layer/htmx_mixins.py
+-rw-r--r--   0        0        0     2110 2023-05-04 10:28:20.883484 ambient-toolbox-8.3.4/ambient_toolbox/view_layer/mixins.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.883484 ambient-toolbox-8.3.4/ambient_toolbox/view_layer/tests/__init__.py
+-rw-r--r--   0        0        0     4124 2023-05-04 10:28:20.883484 ambient-toolbox-8.3.4/ambient_toolbox/view_layer/tests/mixins.py
+-rw-r--r--   0        0        0     1882 2023-05-04 10:28:20.883484 ambient-toolbox-8.3.4/ambient_toolbox/view_layer/views.py
+-rw-r--r--   0        0        0      654 2023-05-10 08:29:28.674940 ambient-toolbox-8.3.4/docs/Makefile
+-rw-r--r--   0        0        0     2803 2023-05-10 08:29:28.671819 ambient-toolbox-8.3.4/docs/conf.py
+-rw-r--r--   0        0        0     6731 2023-05-04 10:28:20.883484 ambient-toolbox-8.3.4/docs/features/admin.md
+-rw-r--r--   0        0        0       35 2023-05-04 10:28:20.883484 ambient-toolbox-8.3.4/docs/features/changelog.rst
+-rw-r--r--   0        0        0     2313 2023-05-04 10:28:20.883484 ambient-toolbox-8.3.4/docs/features/context_manager.md
+-rw-r--r--   0        0        0      549 2023-05-04 10:28:20.883484 ambient-toolbox-8.3.4/docs/features/context_processors.md
+-rw-r--r--   0        0        0     7273 2023-05-04 10:28:20.883484 ambient-toolbox-8.3.4/docs/features/database_anonymisation.md
+-rw-r--r--   0        0        0     6807 2023-05-04 10:28:20.883484 ambient-toolbox-8.3.4/docs/features/djangorestframework.md
+-rw-r--r--   0        0        0     2554 2023-05-04 10:28:20.883484 ambient-toolbox-8.3.4/docs/features/gitlab.md
+-rw-r--r--   0        0        0     6567 2023-05-04 10:28:20.883484 ambient-toolbox-8.3.4/docs/features/graphql.md
+-rw-r--r--   0        0        0     1020 2023-05-04 10:28:20.895496 ambient-toolbox-8.3.4/docs/features/mail.md
+-rw-r--r--   0        0        0     5891 2023-05-04 10:28:20.895496 ambient-toolbox-8.3.4/docs/features/managers.md
+-rw-r--r--   0        0        0     5951 2023-05-04 10:28:20.895496 ambient-toolbox-8.3.4/docs/features/mixins.md
+-rw-r--r--   0        0        0     1553 2023-05-04 10:28:20.895496 ambient-toolbox-8.3.4/docs/features/models.md
+-rw-r--r--   0        0        0     6340 2023-05-12 07:04:33.511067 ambient-toolbox-8.3.4/docs/features/permissions.md
+-rw-r--r--   0        0        0     4454 2023-05-04 10:28:20.895496 ambient-toolbox-8.3.4/docs/features/selectors.md
+-rw-r--r--   0        0        0     3290 2023-05-09 14:44:04.411372 ambient-toolbox-8.3.4/docs/features/sentry.md
+-rw-r--r--   0        0        0     4978 2023-05-04 10:28:20.895496 ambient-toolbox-8.3.4/docs/features/services.md
+-rw-r--r--   0        0        0     1574 2023-05-04 10:28:20.895496 ambient-toolbox-8.3.4/docs/features/setup.md
+-rw-r--r--   0        0        0     5338 2023-05-04 10:28:20.895496 ambient-toolbox-8.3.4/docs/features/tests.md
+-rw-r--r--   0        0        0      232 2023-05-04 10:28:20.895496 ambient-toolbox-8.3.4/docs/features/utils.rst
+-rw-r--r--   0        0        0      527 2023-05-04 10:28:20.895496 ambient-toolbox-8.3.4/docs/features/utils/cache.md
+-rw-r--r--   0        0        0     7417 2023-05-04 10:28:20.895496 ambient-toolbox-8.3.4/docs/features/utils/date.md
+-rw-r--r--   0        0        0      737 2023-05-04 10:28:20.895496 ambient-toolbox-8.3.4/docs/features/utils/math.md
+-rw-r--r--   0        0        0     1100 2023-05-04 10:28:20.895496 ambient-toolbox-8.3.4/docs/features/utils/model.md
+-rw-r--r--   0        0        0     2405 2023-05-04 10:28:20.895496 ambient-toolbox-8.3.4/docs/features/utils/named_tuple.md
+-rw-r--r--   0        0        0     5861 2023-05-04 10:28:20.895496 ambient-toolbox-8.3.4/docs/features/utils/string.md
+-rw-r--r--   0        0        0    15067 2023-05-04 10:28:20.895496 ambient-toolbox-8.3.4/docs/features/view-layer.md
+-rw-r--r--   0        0        0     1185 2023-05-12 07:03:57.521398 ambient-toolbox-8.3.4/docs/index.rst
+-rwxr-xr-x   0        0        0      795 2023-05-10 08:29:28.673380 ambient-toolbox-8.3.4/docs/make.bat
+-rw-r--r--   0        0        0      677 2023-05-04 10:28:20.895496 ambient-toolbox-8.3.4/manage.py
+-rw-r--r--   0        0        0     4100 2023-05-10 08:29:28.650251 ambient-toolbox-8.3.4/pyproject.toml
+-rw-r--r--   0        0        0       56 2023-05-04 10:28:20.895496 ambient-toolbox-8.3.4/pytest.ini
+-rw-r--r--   0        0        0       56 2023-05-10 08:29:28.650251 ambient-toolbox-8.3.4/pytest.init
+-rw-r--r--   0        0        0       50 2023-05-10 08:29:28.676006 ambient-toolbox-8.3.4/scripts/publish_to_pypi.ps1
+-rw-r--r--   0        0        0       50 2023-05-10 08:29:28.677568 ambient-toolbox-8.3.4/scripts/publish_to_pypi.sh
+-rw-r--r--   0        0        0     1704 2023-05-11 16:23:28.767887 ambient-toolbox-8.3.4/settings.py
+-rw-r--r--   0        0        0       69 2023-05-10 08:29:28.667948 ambient-toolbox-8.3.4/setup.cfg
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.895496 ambient-toolbox-8.3.4/testapp/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.895496 ambient-toolbox-8.3.4/testapp/api/__init__.py
+-rw-r--r--   0        0        0      287 2023-05-04 10:28:20.895496 ambient-toolbox-8.3.4/testapp/api/serializers.py
+-rw-r--r--   0        0        0      257 2023-05-04 10:28:20.895496 ambient-toolbox-8.3.4/testapp/api/urls.py
+-rw-r--r--   0        0        0      524 2023-05-04 10:28:20.895496 ambient-toolbox-8.3.4/testapp/api/views.py
+-rw-r--r--   0        0        0      219 2023-05-04 10:28:20.895496 ambient-toolbox-8.3.4/testapp/forms.py
+-rw-r--r--   0        0        0       97 2023-05-04 10:28:20.895496 ambient-toolbox-8.3.4/testapp/managers.py
+-rw-r--r--   0        0        0     6151 2023-05-04 10:28:20.895496 ambient-toolbox-8.3.4/testapp/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.895496 ambient-toolbox-8.3.4/testapp/migrations/__init__.py
+-rw-r--r--   0        0        0     3363 2023-05-04 10:28:20.895496 ambient-toolbox-8.3.4/testapp/models.py
+-rw-r--r--   0        0        0      418 2023-05-12 07:03:57.521398 ambient-toolbox-8.3.4/testapp/permissions.py
+-rw-r--r--   0        0        0      162 2023-05-04 10:28:20.895496 ambient-toolbox-8.3.4/testapp/selectors.py
+-rw-r--r--   0        0        0     1449 2023-05-04 10:28:20.895496 ambient-toolbox-8.3.4/testapp/templates/403.html
+-rw-r--r--   0        0        0      145 2023-05-04 10:28:20.895496 ambient-toolbox-8.3.4/testapp/templates/testapp/test_template.html
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.895496 ambient-toolbox-8.3.4/testapp/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.895496 ambient-toolbox-8.3.4/testapp/tests/missing_init/test_ok.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.895496 ambient-toolbox-8.3.4/testapp/tests/subdirectory/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.4/testapp/tests/subdirectory/missing_test_prefix.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.4/testapp/tests/subdirectory/test_ok.py
+-rw-r--r--   0        0        0      382 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.4/testapp/urls.py
+-rw-r--r--   0        0        0      505 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.4/testapp/views.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.4/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.4/tests/admin/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.4/tests/admin/model_admin_mixins/__init__.py
+-rw-r--r--   0        0        0     2607 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.4/tests/admin/model_admin_mixins/test_admin_common_info_mixin.py
+-rw-r--r--   0        0        0     1900 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.4/tests/admin/model_admin_mixins/test_admin_create_form_mixin.py
+-rw-r--r--   0        0        0     1683 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.4/tests/admin/model_admin_mixins/test_admin_no_inlines_for_create_mixin.py
+-rw-r--r--   0        0        0     1184 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.4/tests/admin/model_admin_mixins/test_admin_request_in_form_mixin.py
+-rw-r--r--   0        0        0     3871 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.4/tests/admin/model_admin_mixins/test_deactivatable_change_view_admin_mixin.py
+-rw-r--r--   0        0        0     1492 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.4/tests/admin/model_admin_mixins/test_fetch_object_mixin.py
+-rw-r--r--   0        0        0     1909 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.4/tests/admin/model_admin_mixins/test_fetch_parent_object_inline_mixin.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.4/tests/ambient_toolbox/__init__.py
+-rw-r--r--   0        0        0     7503 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.4/tests/ambient_toolbox/test_test_structure_validator.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.4/tests/drf/__init__.py
+-rw-r--r--   0        0        0     2579 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.4/tests/drf/test_fields.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.4/tests/mixins/__init__.py
+-rw-r--r--   0        0        0      364 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.4/tests/mixins/validation.py
+-rw-r--r--   0        0        0        0 2023-05-12 07:03:57.521398 ambient-toolbox-8.3.4/tests/permissions/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-12 07:03:57.521398 ambient-toolbox-8.3.4/tests/permissions/fixtures/__init__.py
+-rw-r--r--   0        0        0     1094 2023-05-12 07:03:57.521398 ambient-toolbox-8.3.4/tests/permissions/fixtures/test_declarations.py
+-rw-r--r--   0        0        0      578 2023-05-12 07:03:57.521398 ambient-toolbox-8.3.4/tests/permissions/fixtures/test_helpers.py
+-rw-r--r--   0        0        0     7227 2023-05-12 07:03:57.521398 ambient-toolbox-8.3.4/tests/permissions/fixtures/test_services_setup_service.py
+-rw-r--r--   0        0        0      991 2023-05-12 07:03:57.521398 ambient-toolbox-8.3.4/tests/permissions/test_install_permission_fixtures_command.py
+-rw-r--r--   0        0        0      499 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.4/tests/query_selectors/test_base.py
+-rw-r--r--   0        0        0     1631 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.4/tests/query_selectors/test_permission.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.4/tests/selectors/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-09 14:44:04.427021 ambient-toolbox-8.3.4/tests/sentry/__init__.py
+-rw-r--r--   0        0        0     6196 2023-05-09 14:44:04.427021 ambient-toolbox-8.3.4/tests/sentry/mock_data.py
+-rw-r--r--   0        0        0     1583 2023-05-09 14:44:04.427021 ambient-toolbox-8.3.4/tests/sentry/test_sentry_helper.py
+-rw-r--r--   0        0        0      553 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.4/tests/test_admin_forms.py
+-rw-r--r--   0        0        0     1612 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.4/tests/test_admin_inlines.py
+-rw-r--r--   0        0        0     2651 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.4/tests/test_admin_model_admins_classes.py
+-rw-r--r--   0        0        0     2899 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.4/tests/test_admin_view_mixins.py
+-rw-r--r--   0        0        0     2218 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.4/tests/test_context_manager.py
+-rw-r--r--   0        0        0      822 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.4/tests/test_log_whodid.py
+-rw-r--r--   0        0        0     1169 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.4/tests/test_managers.py
+-rw-r--r--   0        0        0     1628 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.4/tests/test_math.py
+-rw-r--r--   0        0        0     2593 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.4/tests/test_middleware.py
+-rw-r--r--   0        0        0     1200 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.4/tests/test_mixins_models.py
+-rw-r--r--   0        0        0     1669 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.4/tests/test_models.py
+-rw-r--r--   0        0        0     1780 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.4/tests/test_rest_api_mixins.py
+-rw-r--r--   0        0        0      664 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.4/tests/test_scrubbing_service.py
+-rw-r--r--   0        0        0      289 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.4/tests/test_utils_cache.py
+-rw-r--r--   0        0        0    12741 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.4/tests/test_utils_date.py
+-rw-r--r--   0        0        0     1593 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.4/tests/test_utils_file.py
+-rw-r--r--   0        0        0      933 2023-05-04 10:28:20.911132 ambient-toolbox-8.3.4/tests/test_utils_model.py
+-rw-r--r--   0        0        0     3807 2023-05-04 10:28:20.926757 ambient-toolbox-8.3.4/tests/test_utils_named_tuple.py
+-rw-r--r--   0        0        0     5343 2023-05-04 10:28:20.926757 ambient-toolbox-8.3.4/tests/test_utils_string.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.926757 ambient-toolbox-8.3.4/tests/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.926757 ambient-toolbox-8.3.4/tests/tests/mixins/__init__.py
+-rw-r--r--   0        0        0      371 2023-05-04 10:28:20.926757 ambient-toolbox-8.3.4/tests/tests/mixins/models.py
+-rw-r--r--   0        0        0      817 2023-05-04 10:28:20.926757 ambient-toolbox-8.3.4/tests/tests/mixins/test_django_message_framework.py
+-rw-r--r--   0        0        0     2483 2023-05-04 10:28:20.926757 ambient-toolbox-8.3.4/tests/tests/mixins/test_request_provider_mixin.py
+-rw-r--r--   0        0        0     2057 2023-05-04 10:28:20.926757 ambient-toolbox-8.3.4/tests/tests/test_mail_backends.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:28:20.926757 ambient-toolbox-8.3.4/tests/view_layer/__init__.py
+-rw-r--r--   0        0        0     1891 2023-05-04 10:28:20.926757 ambient-toolbox-8.3.4/tests/view_layer/test_formset_mixins.py
+-rw-r--r--   0        0        0     1564 2023-05-04 10:28:20.926757 ambient-toolbox-8.3.4/tests/view_layer/test_htmx_response_mixin.py
+-rw-r--r--   0        0        0     3458 2023-05-04 10:28:20.926757 ambient-toolbox-8.3.4/tests/view_layer/test_meta_mixins.py
+-rw-r--r--   0        0        0     1361 2023-05-04 10:28:20.926757 ambient-toolbox-8.3.4/tests/view_layer/test_views.py
+-rw-r--r--   0        0        0     8311 1970-01-01 00:00:00.000000 ambient-toolbox-8.3.4/PKG-INFO
```

### Comparing `ambient-toolbox-8.3.3/.ambient-package-update/metadata.py` & `ambient-toolbox-8.3.4/.ambient-package-update/metadata.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.3/.github/workflows/ci.yml` & `ambient-toolbox-8.3.4/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.3/.gitignore` & `ambient-toolbox-8.3.4/.gitignore`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.3/.gitlab-ci.yml` & `ambient-toolbox-8.3.4/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.3/.pre-commit-config.yaml` & `ambient-toolbox-8.3.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.3/.readthedocs.yml` & `ambient-toolbox-8.3.4/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.3/CHANGES.md` & `ambient-toolbox-8.3.4/CHANGES.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 # Changelog
 
+**8.3.4** (2023-05-12)
+  * Added docs about integration testing for permission fixtures
+
 **8.3.3** (2023-05-12)
   * Fixed Python 3.8 compat
 
 **8.3.2** (2023-05-11)
   * Updated docs about permission settings setup
 
 **8.3.1** (2023-05-11)
```

### Comparing `ambient-toolbox-8.3.3/Dockerfile` & `ambient-toolbox-8.3.4/Dockerfile`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.3/LICENSE.md` & `ambient-toolbox-8.3.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.3/README.md` & `ambient-toolbox-8.3.4/README.md`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.3/ambient_toolbox/admin/model_admins/classes.py` & `ambient-toolbox-8.3.4/ambient_toolbox/admin/model_admins/classes.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.3/ambient_toolbox/admin/model_admins/inlines.py` & `ambient-toolbox-8.3.4/ambient_toolbox/admin/model_admins/inlines.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.3/ambient_toolbox/admin/model_admins/mixins.py` & `ambient-toolbox-8.3.4/ambient_toolbox/admin/model_admins/mixins.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.3/ambient_toolbox/admin/views/forms.py` & `ambient-toolbox-8.3.4/ambient_toolbox/admin/views/forms.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.3/ambient_toolbox/admin/views/mixins.py` & `ambient-toolbox-8.3.4/ambient_toolbox/admin/views/mixins.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.3/ambient_toolbox/context_manager.py` & `ambient-toolbox-8.3.4/ambient_toolbox/context_manager.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.3/ambient_toolbox/drf/fields.py` & `ambient-toolbox-8.3.4/ambient_toolbox/drf/fields.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.3/ambient_toolbox/drf/serializers.py` & `ambient-toolbox-8.3.4/ambient_toolbox/drf/serializers.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.3/ambient_toolbox/drf/tests.py` & `ambient-toolbox-8.3.4/ambient_toolbox/drf/tests.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.3/ambient_toolbox/gitlab/coverage.py` & `ambient-toolbox-8.3.4/ambient_toolbox/gitlab/coverage.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.3/ambient_toolbox/graphql/forms/mutations.py` & `ambient-toolbox-8.3.4/ambient_toolbox/graphql/forms/mutations.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.3/ambient_toolbox/graphql/schemes/mutations.py` & `ambient-toolbox-8.3.4/ambient_toolbox/graphql/schemes/mutations.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.3/ambient_toolbox/graphql/sentry/views.py` & `ambient-toolbox-8.3.4/ambient_toolbox/graphql/sentry/views.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.3/ambient_toolbox/graphql/tests/base_test.py` & `ambient-toolbox-8.3.4/ambient_toolbox/graphql/tests/base_test.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.3/ambient_toolbox/locale/de/LC_MESSAGES/django.mo` & `ambient-toolbox-8.3.4/ambient_toolbox/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.3/ambient_toolbox/locale/de/LC_MESSAGES/django.po` & `ambient-toolbox-8.3.4/ambient_toolbox/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.3/ambient_toolbox/mail/backends/whitelist_smtp.py` & `ambient-toolbox-8.3.4/ambient_toolbox/mail/backends/whitelist_smtp.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.3/ambient_toolbox/management/commands/install_permission_fixtures.py` & `ambient-toolbox-8.3.4/ambient_toolbox/management/commands/install_permission_fixtures.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,44 +1,44 @@
-from pydoc import locate
-
-from django.conf import settings
-from django.core.management.base import BaseCommand
-
-from ambient_toolbox.permissions.fixtures.declarations import GroupPermissionDeclaration
-from ambient_toolbox.permissions.fixtures.services import PermissionSetupService
-
-
-class Command(BaseCommand):
-    help = "Installs Ambient toolbox improved group permission fixtures"
-
-    def add_arguments(self, parser):
-        parser.add_argument(
-            "--dry-run",
-            action="store_true",
-            help="Doesn't persist any changes in the database",
-        )
-
-    def handle(self, *args, **options):
-        dry_run = options.get('dry_run')
-        if dry_run:
-            print('Starting in "dry-run" mode...')
-
-        try:
-            fixture_declaration_list = settings.GROUP_PERMISSION_FIXTURES
-        except AttributeError:
-            print('No fixtures found in Django settings.')
-            fixture_declaration_list = []
-
-        for declaration_path in fixture_declaration_list:
-            print(f'Reading fixture declaration "{declaration_path}"...')
-            declaration_class: GroupPermissionDeclaration = locate(declaration_path)
-
-            assert isinstance(
-                declaration_class, type(GroupPermissionDeclaration)
-            ), f"Could\'t load group declaration \"{declaration_path}\"."
-
-            print(f'> Installing permissions of group "{declaration_class.name}"...')
-            service = PermissionSetupService(group_declaration=declaration_class, dry_run=dry_run)
-            new_permissions, removed_permissions = service.process()
-
-            print(f'> Newly installed permissions: {new_permissions}')
-            print(f'> Removed permissions: {removed_permissions}\n')
+from pydoc import locate
+
+from django.conf import settings
+from django.core.management.base import BaseCommand
+
+from ambient_toolbox.permissions.fixtures.declarations import GroupPermissionDeclaration
+from ambient_toolbox.permissions.fixtures.services import PermissionSetupService
+
+
+class Command(BaseCommand):
+    help = "Installs Ambient toolbox improved group permission fixtures"
+
+    def add_arguments(self, parser):
+        parser.add_argument(
+            "--dry-run",
+            action="store_true",
+            help="Doesn't persist any changes in the database",
+        )
+
+    def handle(self, *args, **options):
+        dry_run = options.get('dry_run')
+        if dry_run:
+            print('Starting in "dry-run" mode...')
+
+        try:
+            fixture_declaration_list = settings.GROUP_PERMISSION_FIXTURES
+        except AttributeError:
+            print('No fixtures found in Django settings.')
+            fixture_declaration_list = []
+
+        for declaration_path in fixture_declaration_list:
+            print(f'Reading fixture declaration "{declaration_path}"...')
+            declaration_class: GroupPermissionDeclaration = locate(declaration_path)
+
+            assert isinstance(
+                declaration_class, type(GroupPermissionDeclaration)
+            ), f"Could\'t load group declaration \"{declaration_path}\"."
+
+            print(f'> Installing permissions of group "{declaration_class.name}"...')
+            service = PermissionSetupService(group_declaration=declaration_class, dry_run=dry_run)
+            new_permissions, removed_permissions = service.process()
+
+            print(f'> Newly installed permissions: {new_permissions}')
+            print(f'> Removed permissions: {removed_permissions}\n')
```

### Comparing `ambient-toolbox-8.3.3/ambient_toolbox/managers.py` & `ambient-toolbox-8.3.4/ambient_toolbox/managers.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.3/ambient_toolbox/middleware/current_user.py` & `ambient-toolbox-8.3.4/ambient_toolbox/middleware/current_user.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.3/ambient_toolbox/mixins/bleacher.py` & `ambient-toolbox-8.3.4/ambient_toolbox/mixins/bleacher.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.3/ambient_toolbox/mixins/models.py` & `ambient-toolbox-8.3.4/ambient_toolbox/mixins/models.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.3/ambient_toolbox/models.py` & `ambient-toolbox-8.3.4/ambient_toolbox/models.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.3/ambient_toolbox/permissions/fixtures/services.py` & `ambient-toolbox-8.3.4/ambient_toolbox/permissions/fixtures/services.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,73 +1,73 @@
-from typing import List
-
-from django.contrib.auth.models import Group, Permission
-from django.contrib.contenttypes.models import ContentType
-from django.db import transaction
-
-from ambient_toolbox.permissions.fixtures.declarations import GroupPermissionDeclaration
-
-
-class PermissionSetupService:
-    group_declaration: GroupPermissionDeclaration
-    dry_run: bool
-
-    def __init__(self, group_declaration: GroupPermissionDeclaration, dry_run: bool = False) -> None:
-        super().__init__()
-
-        self.group_declaration = group_declaration
-        self.dry_run = dry_run
-
-    @transaction.atomic
-    def process(self) -> (List[Permission], List[Permission]):
-        # Fetch or create group
-        group, created = Group.objects.get_or_create(name=self.group_declaration.name)
-
-        # Declare lists where we'll sort in the permissions
-        defined_permission_list = []
-        new_permissions = []
-        removed_permissions = []
-
-        # Iterate all in fixtures defined permission models...
-        for permission_declaration in self.group_declaration.permission_list:
-            # Iterate all fixture permissions...
-            for codename in permission_declaration.codename_list:
-                # Instantiate permission as ORM object
-                try:
-                    new_permission = Permission.objects.get_by_natural_key(
-                        app_label=permission_declaration.app_label,
-                        codename=codename,
-                        model=permission_declaration.model,
-                    )
-                except Permission.DoesNotExist as e:
-                    raise ValueError(f'Invalid permission "{permission_declaration.model}.{codename}" declared.') from e
-                except ContentType.DoesNotExist as e:
-                    raise ValueError(
-                        f'Invalid content type "{permission_declaration.app_label}'
-                        f'.{permission_declaration.model}" declared.'
-                    ) from e
-
-                # Add permission object to list
-                if new_permission in defined_permission_list:
-                    raise ValueError(f'Permission {new_permission} declared twice.')
-                defined_permission_list.append(new_permission)
-
-                # Check if permission is already set in the group
-                if new_permission not in group.permissions.all():
-                    new_permissions.append(new_permission)
-
-        # Check which permissions were removed for the given group
-        for existing_permission in group.permissions.all():
-            if existing_permission not in defined_permission_list:
-                removed_permissions.append(existing_permission)
-
-        if not self.dry_run:
-            # Persist changes on removed permissions
-            if len(removed_permissions):
-                group.permissions.remove(*removed_permissions)
-
-            # Persist changes on added permissions
-            if len(new_permissions):
-                group.permissions.add(*new_permissions)
-
-        # Return changes
-        return new_permissions, removed_permissions
+from typing import List
+
+from django.contrib.auth.models import Group, Permission
+from django.contrib.contenttypes.models import ContentType
+from django.db import transaction
+
+from ambient_toolbox.permissions.fixtures.declarations import GroupPermissionDeclaration
+
+
+class PermissionSetupService:
+    group_declaration: GroupPermissionDeclaration
+    dry_run: bool
+
+    def __init__(self, group_declaration: GroupPermissionDeclaration, dry_run: bool = False) -> None:
+        super().__init__()
+
+        self.group_declaration = group_declaration
+        self.dry_run = dry_run
+
+    @transaction.atomic
+    def process(self) -> (List[Permission], List[Permission]):
+        # Fetch or create group
+        group, created = Group.objects.get_or_create(name=self.group_declaration.name)
+
+        # Declare lists where we'll sort in the permissions
+        defined_permission_list = []
+        new_permissions = []
+        removed_permissions = []
+
+        # Iterate all in fixtures defined permission models...
+        for permission_declaration in self.group_declaration.permission_list:
+            # Iterate all fixture permissions...
+            for codename in permission_declaration.codename_list:
+                # Instantiate permission as ORM object
+                try:
+                    new_permission = Permission.objects.get_by_natural_key(
+                        app_label=permission_declaration.app_label,
+                        codename=codename,
+                        model=permission_declaration.model,
+                    )
+                except Permission.DoesNotExist as e:
+                    raise ValueError(f'Invalid permission "{permission_declaration.model}.{codename}" declared.') from e
+                except ContentType.DoesNotExist as e:
+                    raise ValueError(
+                        f'Invalid content type "{permission_declaration.app_label}'
+                        f'.{permission_declaration.model}" declared.'
+                    ) from e
+
+                # Add permission object to list
+                if new_permission in defined_permission_list:
+                    raise ValueError(f'Permission {new_permission} declared twice.')
+                defined_permission_list.append(new_permission)
+
+                # Check if permission is already set in the group
+                if new_permission not in group.permissions.all():
+                    new_permissions.append(new_permission)
+
+        # Check which permissions were removed for the given group
+        for existing_permission in group.permissions.all():
+            if existing_permission not in defined_permission_list:
+                removed_permissions.append(existing_permission)
+
+        if not self.dry_run:
+            # Persist changes on removed permissions
+            if len(removed_permissions):
+                group.permissions.remove(*removed_permissions)
+
+            # Persist changes on added permissions
+            if len(new_permissions):
+                group.permissions.add(*new_permissions)
+
+        # Return changes
+        return new_permissions, removed_permissions
```

### Comparing `ambient-toolbox-8.3.3/ambient_toolbox/selectors/permission.py` & `ambient-toolbox-8.3.4/ambient_toolbox/selectors/permission.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.3/ambient_toolbox/sentry/helpers.py` & `ambient-toolbox-8.3.4/ambient_toolbox/sentry/helpers.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.3/ambient_toolbox/services/custom_scrubber.py` & `ambient-toolbox-8.3.4/ambient_toolbox/services/custom_scrubber.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.3/ambient_toolbox/templatetags/ai_email_tags.py` & `ambient-toolbox-8.3.4/ambient_toolbox/templatetags/ai_email_tags.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.3/ambient_toolbox/templatetags/ai_file_tags.py` & `ambient-toolbox-8.3.4/ambient_toolbox/templatetags/ai_file_tags.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.3/ambient_toolbox/templatetags/ai_number_tags.py` & `ambient-toolbox-8.3.4/ambient_toolbox/templatetags/ai_number_tags.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.3/ambient_toolbox/templatetags/ai_string_tags.py` & `ambient-toolbox-8.3.4/ambient_toolbox/templatetags/ai_string_tags.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.3/ambient_toolbox/tests/mixins.py` & `ambient-toolbox-8.3.4/ambient_toolbox/tests/mixins.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.3/ambient_toolbox/tests/structure_validator/test_structure_validator.py` & `ambient-toolbox-8.3.4/ambient_toolbox/tests/structure_validator/test_structure_validator.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.3/ambient_toolbox/utils/date.py` & `ambient-toolbox-8.3.4/ambient_toolbox/utils/date.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.3/ambient_toolbox/utils/file.py` & `ambient-toolbox-8.3.4/ambient_toolbox/utils/file.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.3/ambient_toolbox/utils/math.py` & `ambient-toolbox-8.3.4/ambient_toolbox/utils/math.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.3/ambient_toolbox/utils/model.py` & `ambient-toolbox-8.3.4/ambient_toolbox/utils/model.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.3/ambient_toolbox/utils/named_tuple.py` & `ambient-toolbox-8.3.4/ambient_toolbox/utils/named_tuple.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.3/ambient_toolbox/utils/string.py` & `ambient-toolbox-8.3.4/ambient_toolbox/utils/string.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.3/ambient_toolbox/view_layer/form_mixins.py` & `ambient-toolbox-8.3.4/ambient_toolbox/view_layer/form_mixins.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.3/ambient_toolbox/view_layer/formset_view_mixin.py` & `ambient-toolbox-8.3.4/ambient_toolbox/view_layer/formset_view_mixin.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.3/ambient_toolbox/view_layer/htmx_mixins.py` & `ambient-toolbox-8.3.4/ambient_toolbox/view_layer/htmx_mixins.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.3/ambient_toolbox/view_layer/mixins.py` & `ambient-toolbox-8.3.4/ambient_toolbox/view_layer/mixins.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.3/ambient_toolbox/view_layer/tests/mixins.py` & `ambient-toolbox-8.3.4/ambient_toolbox/view_layer/tests/mixins.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.3/ambient_toolbox/view_layer/views.py` & `ambient-toolbox-8.3.4/ambient_toolbox/view_layer/views.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.3/docs/Makefile` & `ambient-toolbox-8.3.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.3/docs/conf.py` & `ambient-toolbox-8.3.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.3/docs/features/admin.md` & `ambient-toolbox-8.3.4/docs/features/admin.md`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.3/docs/features/context_manager.md` & `ambient-toolbox-8.3.4/docs/features/context_manager.md`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.3/docs/features/context_processors.md` & `ambient-toolbox-8.3.4/docs/features/context_processors.md`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.3/docs/features/database_anonymisation.md` & `ambient-toolbox-8.3.4/docs/features/database_anonymisation.md`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.3/docs/features/djangorestframework.md` & `ambient-toolbox-8.3.4/docs/features/djangorestframework.md`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.3/docs/features/gitlab.md` & `ambient-toolbox-8.3.4/docs/features/gitlab.md`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.3/docs/features/graphql.md` & `ambient-toolbox-8.3.4/docs/features/graphql.md`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.3/docs/features/mail.md` & `ambient-toolbox-8.3.4/docs/features/mail.md`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.3/docs/features/managers.md` & `ambient-toolbox-8.3.4/docs/features/managers.md`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.3/docs/features/mixins.md` & `ambient-toolbox-8.3.4/docs/features/mixins.md`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.3/docs/features/models.md` & `ambient-toolbox-8.3.4/docs/features/models.md`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.3/docs/features/permissions.md` & `ambient-toolbox-8.3.4/docs/features/permissions.md`

 * *Files 10% similar despite different names*

```diff
@@ -161,12 +161,30 @@
 
 ### Validation / pipeline check
 
 If you want to validate that you didn't make any mistakes, you can run the same command as a "dry-run" in your CI/CD.
 
 > python ./manage.py install_permission_fixtures --dry-run
 
+### Testing
+
+To ensure that your setup is correct, and you use only valid and existing permissions, you can write a quick integration
+test. Note that removing a Django permission code-wise won't result in removing it in the database. So having a
+non-existing permission in your permission fixtures might not necessarily lead to an error. The test database on the
+other hand is created from scratch and therefore only contains valid permissions.
+
+````python
+from django.core.management import call_command
+from django.test import TestCase
+
+
+class PermissionFixturesIntegrationTest(TestCase):
+
+    def test_integration_regular(self):
+        call_command('install_permission_fixtures', '--dry-run')
+````
+
 ### Limitations
 
 Please note that new groups will be created but the service won't **delete** any groups. The simple reason is that if
 you rename a group, this would count as a "delete" and a "create" operation. The new group would have all permissions
 but all user assignment would be lost on deleting the previous group.
```

### Comparing `ambient-toolbox-8.3.3/docs/features/selectors.md` & `ambient-toolbox-8.3.4/docs/features/selectors.md`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.3/docs/features/sentry.md` & `ambient-toolbox-8.3.4/docs/features/sentry.md`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.3/docs/features/services.md` & `ambient-toolbox-8.3.4/docs/features/services.md`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.3/docs/features/setup.md` & `ambient-toolbox-8.3.4/docs/features/setup.md`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.3/docs/features/tests.md` & `ambient-toolbox-8.3.4/docs/features/tests.md`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.3/docs/features/utils/cache.md` & `ambient-toolbox-8.3.4/docs/features/utils/cache.md`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.3/docs/features/utils/date.md` & `ambient-toolbox-8.3.4/docs/features/utils/date.md`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.3/docs/features/utils/math.md` & `ambient-toolbox-8.3.4/docs/features/utils/math.md`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.3/docs/features/utils/model.md` & `ambient-toolbox-8.3.4/docs/features/utils/model.md`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.3/docs/features/utils/named_tuple.md` & `ambient-toolbox-8.3.4/docs/features/utils/named_tuple.md`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.3/docs/features/utils/string.md` & `ambient-toolbox-8.3.4/docs/features/utils/string.md`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.3/docs/features/view-layer.md` & `ambient-toolbox-8.3.4/docs/features/view-layer.md`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.3/docs/index.rst` & `ambient-toolbox-8.3.4/docs/index.rst`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-ambient-toolbox
-==============
-
-Welcome to the Ambient Toolbox ``ambient-toolbox``!
-
-Since 2012 we are gathering tools and useful code snippets to share them across projects. The toolbox ``ambient-toolbox``
-provides utilities for a wide range of applications. Please have a look at the following chapters to familiarise
-yourself with them.
-
-The package is published at pypi under the following link: `https://pypi.org/project/ambient-toolbox/ <https://pypi.org/project/ambient-toolbox/>`_
-
-
-.. toctree::
-   :maxdepth: 1
-   :caption: Contents:
-
-   features/setup.md
-   features/admin.md
-   features/context_manager.md
-   features/context_processors.md
-   features/database_anonymisation.md
-   features/djangorestframework.md
-   features/gitlab.md
-   features/graphql.md
-   features/managers.md
-   features/mail.md
-   features/models.md
-   features/mixins.md
-   features/permissions.md
-   features/selectors.md
-   features/sentry.md
-   features/services.md
-   features/tests.md
-   features/utils.rst
-   features/view-layer.rst
-   features/changelog.md
-
-Indices and tables
-==================
-
-* :ref:`genindex`
-* :ref:`modindex`
-* :ref:`search`
+ambient-toolbox
+==============
+
+Welcome to the Ambient Toolbox ``ambient-toolbox``!
+
+Since 2012 we are gathering tools and useful code snippets to share them across projects. The toolbox ``ambient-toolbox``
+provides utilities for a wide range of applications. Please have a look at the following chapters to familiarise
+yourself with them.
+
+The package is published at pypi under the following link: `https://pypi.org/project/ambient-toolbox/ <https://pypi.org/project/ambient-toolbox/>`_
+
+
+.. toctree::
+   :maxdepth: 1
+   :caption: Contents:
+
+   features/setup.md
+   features/admin.md
+   features/context_manager.md
+   features/context_processors.md
+   features/database_anonymisation.md
+   features/djangorestframework.md
+   features/gitlab.md
+   features/graphql.md
+   features/managers.md
+   features/mail.md
+   features/models.md
+   features/mixins.md
+   features/permissions.md
+   features/selectors.md
+   features/sentry.md
+   features/services.md
+   features/tests.md
+   features/utils.rst
+   features/view-layer.rst
+   features/changelog.md
+
+Indices and tables
+==================
+
+* :ref:`genindex`
+* :ref:`modindex`
+* :ref:`search`
```

### Comparing `ambient-toolbox-8.3.3/docs/make.bat` & `ambient-toolbox-8.3.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.3/manage.py` & `ambient-toolbox-8.3.4/manage.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.3/pyproject.toml` & `ambient-toolbox-8.3.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.3/settings.py` & `ambient-toolbox-8.3.4/settings.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.3/testapp/api/views.py` & `ambient-toolbox-8.3.4/testapp/api/views.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.3/testapp/migrations/0001_initial.py` & `ambient-toolbox-8.3.4/testapp/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.3/testapp/models.py` & `ambient-toolbox-8.3.4/testapp/models.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.3/testapp/templates/403.html` & `ambient-toolbox-8.3.4/testapp/templates/403.html`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.3/tests/admin/model_admin_mixins/test_admin_common_info_mixin.py` & `ambient-toolbox-8.3.4/tests/admin/model_admin_mixins/test_admin_common_info_mixin.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.3/tests/admin/model_admin_mixins/test_admin_create_form_mixin.py` & `ambient-toolbox-8.3.4/tests/admin/model_admin_mixins/test_admin_create_form_mixin.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.3/tests/admin/model_admin_mixins/test_admin_no_inlines_for_create_mixin.py` & `ambient-toolbox-8.3.4/tests/admin/model_admin_mixins/test_admin_no_inlines_for_create_mixin.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.3/tests/admin/model_admin_mixins/test_admin_request_in_form_mixin.py` & `ambient-toolbox-8.3.4/tests/admin/model_admin_mixins/test_admin_request_in_form_mixin.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.3/tests/admin/model_admin_mixins/test_deactivatable_change_view_admin_mixin.py` & `ambient-toolbox-8.3.4/tests/admin/model_admin_mixins/test_deactivatable_change_view_admin_mixin.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.3/tests/admin/model_admin_mixins/test_fetch_object_mixin.py` & `ambient-toolbox-8.3.4/tests/admin/model_admin_mixins/test_fetch_object_mixin.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.3/tests/admin/model_admin_mixins/test_fetch_parent_object_inline_mixin.py` & `ambient-toolbox-8.3.4/tests/admin/model_admin_mixins/test_fetch_parent_object_inline_mixin.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.3/tests/ambient_toolbox/test_test_structure_validator.py` & `ambient-toolbox-8.3.4/tests/ambient_toolbox/test_test_structure_validator.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.3/tests/drf/test_fields.py` & `ambient-toolbox-8.3.4/tests/drf/test_fields.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.3/tests/permissions/fixtures/test_declarations.py` & `ambient-toolbox-8.3.4/tests/permissions/fixtures/test_declarations.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-from django.test import TestCase
-
-from ambient_toolbox.permissions.fixtures.declarations import GroupPermissionDeclaration, PermissionModelDeclaration
-
-
-class PermissionFixtureDeclarationTest(TestCase):
-    def test_permission_model_declaration_regular(self):
-        permission = PermissionModelDeclaration(
-            app_label='my_app',
-            codename_list=['view_mymodel'],
-            model='mymodel',
-        )
-
-        self.assertEqual(permission.app_label, 'my_app')
-        self.assertEqual(permission.codename_list, ['view_mymodel'])
-        self.assertEqual(permission.model, 'mymodel')
-
-    def test_group_permission_declaration_regular(self):
-        permission = PermissionModelDeclaration(
-            app_label='my_app',
-            codename_list=['view_mymodel'],
-            model='mymodel',
-        )
-        group = GroupPermissionDeclaration(
-            name='my_group',
-            permission_list=[permission],
-        )
-
-        self.assertEqual(group.name, 'my_group')
-        self.assertEqual(group.permission_list, [permission])
+from django.test import TestCase
+
+from ambient_toolbox.permissions.fixtures.declarations import GroupPermissionDeclaration, PermissionModelDeclaration
+
+
+class PermissionFixtureDeclarationTest(TestCase):
+    def test_permission_model_declaration_regular(self):
+        permission = PermissionModelDeclaration(
+            app_label='my_app',
+            codename_list=['view_mymodel'],
+            model='mymodel',
+        )
+
+        self.assertEqual(permission.app_label, 'my_app')
+        self.assertEqual(permission.codename_list, ['view_mymodel'])
+        self.assertEqual(permission.model, 'mymodel')
+
+    def test_group_permission_declaration_regular(self):
+        permission = PermissionModelDeclaration(
+            app_label='my_app',
+            codename_list=['view_mymodel'],
+            model='mymodel',
+        )
+        group = GroupPermissionDeclaration(
+            name='my_group',
+            permission_list=[permission],
+        )
+
+        self.assertEqual(group.name, 'my_group')
+        self.assertEqual(group.permission_list, [permission])
```

### Comparing `ambient-toolbox-8.3.3/tests/permissions/fixtures/test_helpers.py` & `ambient-toolbox-8.3.4/tests/permissions/fixtures/test_helpers.py`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-from django.test import TestCase
-
-from ambient_toolbox.permissions.fixtures.helpers import generate_default_permissions
-
-
-class PermissionFixtureHelperTest(TestCase):
-    def test_generate_default_permissions_regular(self):
-        permission_list = generate_default_permissions('mymodel')
-
-        self.assertEqual(len(permission_list), 4)
-        self.assertIn('add_mymodel', permission_list)
-        self.assertIn('change_mymodel', permission_list)
-        self.assertIn('delete_mymodel', permission_list)
-        self.assertIn('view_mymodel', permission_list)
+from django.test import TestCase
+
+from ambient_toolbox.permissions.fixtures.helpers import generate_default_permissions
+
+
+class PermissionFixtureHelperTest(TestCase):
+    def test_generate_default_permissions_regular(self):
+        permission_list = generate_default_permissions('mymodel')
+
+        self.assertEqual(len(permission_list), 4)
+        self.assertIn('add_mymodel', permission_list)
+        self.assertIn('change_mymodel', permission_list)
+        self.assertIn('delete_mymodel', permission_list)
+        self.assertIn('view_mymodel', permission_list)
```

### Comparing `ambient-toolbox-8.3.3/tests/permissions/test_install_permission_fixtures_command.py` & `ambient-toolbox-8.3.4/tests/permissions/test_install_permission_fixtures_command.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-from unittest import mock
-
-from django.test import TestCase
-from django.test.utils import override_settings
-
-from ambient_toolbox.management.commands.install_permission_fixtures import Command
-from ambient_toolbox.permissions.fixtures.services import PermissionSetupService
-
-
-class InstallPermissionFixturesCommandTest(TestCase):
-    @classmethod
-    def setUpTestData(cls):
-        super().setUpTestData()
-
-    @override_settings(GROUP_PERMISSION_FIXTURES=['testapp.permissions.TestGroupDeclaration'])
-    @mock.patch.object(PermissionSetupService, 'process', return_value=([], []))
-    def test_run_command_regular(self, mocked_process):
-        command = Command()
-        command.handle()
-
-        mocked_process.assert_called_once()
-
-    @mock.patch.object(PermissionSetupService, 'process')
-    def test_run_command_no_settings_variable(self, mocked_process):
-        command = Command()
-        command.handle()
-
-        mocked_process.assert_not_called()
+from unittest import mock
+
+from django.test import TestCase
+from django.test.utils import override_settings
+
+from ambient_toolbox.management.commands.install_permission_fixtures import Command
+from ambient_toolbox.permissions.fixtures.services import PermissionSetupService
+
+
+class InstallPermissionFixturesCommandTest(TestCase):
+    @classmethod
+    def setUpTestData(cls):
+        super().setUpTestData()
+
+    @override_settings(GROUP_PERMISSION_FIXTURES=['testapp.permissions.TestGroupDeclaration'])
+    @mock.patch.object(PermissionSetupService, 'process', return_value=([], []))
+    def test_run_command_regular(self, mocked_process):
+        command = Command()
+        command.handle()
+
+        mocked_process.assert_called_once()
+
+    @mock.patch.object(PermissionSetupService, 'process')
+    def test_run_command_no_settings_variable(self, mocked_process):
+        command = Command()
+        command.handle()
+
+        mocked_process.assert_not_called()
```

### Comparing `ambient-toolbox-8.3.3/tests/query_selectors/test_permission.py` & `ambient-toolbox-8.3.4/tests/query_selectors/test_permission.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.3/tests/sentry/mock_data.py` & `ambient-toolbox-8.3.4/tests/sentry/mock_data.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.3/tests/sentry/test_sentry_helper.py` & `ambient-toolbox-8.3.4/tests/sentry/test_sentry_helper.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.3/tests/test_admin_forms.py` & `ambient-toolbox-8.3.4/tests/test_admin_forms.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.3/tests/test_admin_inlines.py` & `ambient-toolbox-8.3.4/tests/test_admin_inlines.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.3/tests/test_admin_model_admins_classes.py` & `ambient-toolbox-8.3.4/tests/test_admin_model_admins_classes.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.3/tests/test_admin_view_mixins.py` & `ambient-toolbox-8.3.4/tests/test_admin_view_mixins.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.3/tests/test_context_manager.py` & `ambient-toolbox-8.3.4/tests/test_context_manager.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.3/tests/test_log_whodid.py` & `ambient-toolbox-8.3.4/tests/test_log_whodid.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.3/tests/test_managers.py` & `ambient-toolbox-8.3.4/tests/test_managers.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.3/tests/test_math.py` & `ambient-toolbox-8.3.4/tests/test_math.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.3/tests/test_middleware.py` & `ambient-toolbox-8.3.4/tests/test_middleware.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.3/tests/test_mixins_models.py` & `ambient-toolbox-8.3.4/tests/test_mixins_models.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.3/tests/test_models.py` & `ambient-toolbox-8.3.4/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.3/tests/test_rest_api_mixins.py` & `ambient-toolbox-8.3.4/tests/test_rest_api_mixins.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.3/tests/test_scrubbing_service.py` & `ambient-toolbox-8.3.4/tests/test_scrubbing_service.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.3/tests/test_utils_date.py` & `ambient-toolbox-8.3.4/tests/test_utils_date.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.3/tests/test_utils_file.py` & `ambient-toolbox-8.3.4/tests/test_utils_file.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.3/tests/test_utils_model.py` & `ambient-toolbox-8.3.4/tests/test_utils_model.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.3/tests/test_utils_named_tuple.py` & `ambient-toolbox-8.3.4/tests/test_utils_named_tuple.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.3/tests/test_utils_string.py` & `ambient-toolbox-8.3.4/tests/test_utils_string.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.3/tests/tests/mixins/test_django_message_framework.py` & `ambient-toolbox-8.3.4/tests/tests/mixins/test_django_message_framework.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.3/tests/tests/mixins/test_request_provider_mixin.py` & `ambient-toolbox-8.3.4/tests/tests/mixins/test_request_provider_mixin.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.3/tests/tests/test_mail_backends.py` & `ambient-toolbox-8.3.4/tests/tests/test_mail_backends.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.3/tests/view_layer/test_formset_mixins.py` & `ambient-toolbox-8.3.4/tests/view_layer/test_formset_mixins.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.3/tests/view_layer/test_htmx_response_mixin.py` & `ambient-toolbox-8.3.4/tests/view_layer/test_htmx_response_mixin.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.3/tests/view_layer/test_meta_mixins.py` & `ambient-toolbox-8.3.4/tests/view_layer/test_meta_mixins.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.3/tests/view_layer/test_views.py` & `ambient-toolbox-8.3.4/tests/view_layer/test_views.py`

 * *Files identical despite different names*

### Comparing `ambient-toolbox-8.3.3/PKG-INFO` & `ambient-toolbox-8.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ambient-toolbox
-Version: 8.3.3
+Version: 8.3.4
 Summary: Python toolbox of Ambient Digital containing an abundance of useful tools and gadgets.
 Author-email: Ambient Digital <hello@ambient.digital>
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 2.2
```

