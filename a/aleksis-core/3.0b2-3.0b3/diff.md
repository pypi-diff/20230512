# Comparing `tmp/aleksis_core-3.0b2.tar.gz` & `tmp/aleksis_core-3.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aleksis_core-3.0b2.tar", max compression
+gzip compressed data, was "aleksis_core-3.0b3.tar", max compression
```

## Comparing `aleksis_core-3.0b2.tar` & `aleksis_core-3.0b3.tar`

### file list

```diff
@@ -1,479 +1,479 @@
--rw-r--r--   0        0        0    33437 2023-03-09 21:28:25.700627 aleksis_core-3.0b2/CHANGELOG.rst
--rw-r--r--   0        0        0    14353 2023-03-09 21:28:25.700627 aleksis_core-3.0b2/LICENCE.rst
--rw-r--r--   0        0        0     3780 2023-03-09 21:28:25.700627 aleksis_core-3.0b2/README.rst
--rw-r--r--   0        0        0      194 2023-03-09 21:28:25.700627 aleksis_core-3.0b2/aleksis/core/__init__.py
--rw-r--r--   0        0        0      464 2023-03-09 21:28:25.700627 aleksis_core-3.0b2/aleksis/core/__main__.py
--rw-r--r--   0        0        0      510 2023-03-09 21:36:20.447814 aleksis_core-3.0b2/aleksis/core/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     1068 2023-03-09 21:36:20.983813 aleksis_core-3.0b2/aleksis/core/__pycache__/__main__.cpython-311.pyc
--rw-r--r--   0        0        0     2061 2023-03-09 21:36:22.651810 aleksis_core-3.0b2/aleksis/core/__pycache__/admin.cpython-311.pyc
--rw-r--r--   0        0        0    10911 2023-03-09 21:36:21.535812 aleksis_core-3.0b2/aleksis/core/__pycache__/apps.cpython-311.pyc
--rw-r--r--   0        0        0     2533 2023-03-09 21:36:20.499814 aleksis_core-3.0b2/aleksis/core/__pycache__/celery.cpython-311.pyc
--rw-r--r--   0        0        0     3716 2023-03-09 21:36:22.731810 aleksis_core-3.0b2/aleksis/core/__pycache__/checks.cpython-311.pyc
--rw-r--r--   0        0        0    17897 2023-03-09 21:36:22.459810 aleksis_core-3.0b2/aleksis/core/__pycache__/data_checks.cpython-311.pyc
--rw-r--r--   0        0        0     5154 2023-03-09 21:36:22.739810 aleksis_core-3.0b2/aleksis/core/__pycache__/health_checks.cpython-311.pyc
--rw-r--r--   0        0        0     8423 2023-03-09 21:36:22.479810 aleksis_core-3.0b2/aleksis/core/__pycache__/managers.cpython-311.pyc
--rw-r--r--   0        0        0    30729 2023-03-09 21:36:22.467810 aleksis_core-3.0b2/aleksis/core/__pycache__/mixins.cpython-311.pyc
--rw-r--r--   0        0        0    84345 2023-03-09 21:36:22.215811 aleksis_core-3.0b2/aleksis/core/__pycache__/models.cpython-311.pyc
--rw-r--r--   0        0        0    22958 2023-03-09 21:36:22.771810 aleksis_core-3.0b2/aleksis/core/__pycache__/preferences.cpython-311.pyc
--rw-r--r--   0        0        0     1370 2023-03-09 21:36:21.543812 aleksis_core-3.0b2/aleksis/core/__pycache__/registries.cpython-311.pyc
--rw-r--r--   0        0        0    16322 2023-03-09 21:36:22.671810 aleksis_core-3.0b2/aleksis/core/__pycache__/rules.cpython-311.pyc
--rw-r--r--   0        0        0    43405 2023-03-09 21:36:20.995813 aleksis_core-3.0b2/aleksis/core/__pycache__/settings.cpython-311.pyc
--rw-r--r--   0        0        0     3825 2023-03-09 21:36:22.491810 aleksis_core-3.0b2/aleksis/core/__pycache__/tasks.cpython-311.pyc
--rw-r--r--   0        0        0      950 2023-03-09 21:28:25.700627 aleksis_core-3.0b2/aleksis/core/admin.py
--rw-r--r--   0        0        0     8274 2023-03-09 21:28:25.700627 aleksis_core-3.0b2/aleksis/core/apps.py
--rw-r--r--   0        0        0     1338 2023-03-09 21:28:25.700627 aleksis_core-3.0b2/aleksis/core/celery.py
--rw-r--r--   0        0        0     2751 2023-03-09 21:28:25.700627 aleksis_core-3.0b2/aleksis/core/checks.py
--rw-r--r--   0        0        0    11534 2023-03-09 21:28:25.700627 aleksis_core-3.0b2/aleksis/core/data_checks.py
--rw-r--r--   0        0        0      741 2023-03-09 21:28:25.700627 aleksis_core-3.0b2/aleksis/core/decorators.py
--rw-r--r--   0        0        0     5556 2023-03-09 21:28:25.704627 aleksis_core-3.0b2/aleksis/core/filters.py
--rw-r--r--   0        0        0    30812 2023-03-09 21:28:25.704627 aleksis_core-3.0b2/aleksis/core/forms.py
--rw-r--r--   0        0        0     3000 2023-03-09 21:28:25.704627 aleksis_core-3.0b2/aleksis/core/frontend/app/apollo.js
--rw-r--r--   0        0        0      803 2023-03-09 21:28:25.704627 aleksis_core-3.0b2/aleksis/core/frontend/app/dateTimeFormats.js
--rw-r--r--   0        0        0      197 2023-03-09 21:28:25.704627 aleksis_core-3.0b2/aleksis/core/frontend/app/i18n.js
--rw-r--r--   0        0        0      157 2023-03-09 21:28:25.704627 aleksis_core-3.0b2/aleksis/core/frontend/app/router.js
--rw-r--r--   0        0        0      133 2023-03-09 21:28:25.704627 aleksis_core-3.0b2/aleksis/core/frontend/app/sentry.js
--rw-r--r--   0        0        0      793 2023-03-09 21:28:25.704627 aleksis_core-3.0b2/aleksis/core/frontend/app/vuetify.js
--rw-r--r--   0        0        0     3014 2023-03-09 21:28:25.704627 aleksis_core-3.0b2/aleksis/core/frontend/components/LegacyBaseTemplate.vue
--rw-r--r--   0        0        0      158 2023-03-09 21:28:25.704627 aleksis_core-3.0b2/aleksis/core/frontend/components/Parent.vue
--rw-r--r--   0        0        0      335 2023-03-09 21:28:25.704627 aleksis_core-3.0b2/aleksis/core/frontend/components/about/About.vue
--rw-r--r--   0        0        0     1971 2023-03-09 21:28:25.704627 aleksis_core-3.0b2/aleksis/core/frontend/components/about/AboutAleksis.vue
--rw-r--r--   0        0        0     3831 2023-03-09 21:28:25.704627 aleksis_core-3.0b2/aleksis/core/frontend/components/about/InstalledAppCard.vue
--rw-r--r--   0        0        0     1003 2023-03-09 21:28:25.704627 aleksis_core-3.0b2/aleksis/core/frontend/components/about/InstalledAppsList.vue
--rw-r--r--   0        0        0      351 2023-03-09 21:28:25.704627 aleksis_core-3.0b2/aleksis/core/frontend/components/about/installedApps.graphql
--rw-r--r--   0        0        0     2411 2023-03-09 21:28:25.704627 aleksis_core-3.0b2/aleksis/core/frontend/components/app/AccountMenu.vue
--rw-r--r--   0        0        0     9194 2023-03-09 21:28:25.704627 aleksis_core-3.0b2/aleksis/core/frontend/components/app/App.vue
--rw-r--r--   0        0        0      314 2023-03-09 21:28:25.704627 aleksis_core-3.0b2/aleksis/core/frontend/components/app/BrandLogo.vue
--rw-r--r--   0        0        0     1064 2023-03-09 21:28:25.704627 aleksis_core-3.0b2/aleksis/core/frontend/components/app/ErrorPage.vue
--rw-r--r--   0        0        0     1036 2023-03-09 21:28:25.704627 aleksis_core-3.0b2/aleksis/core/frontend/components/app/LanguageForm.vue
--rw-r--r--   0        0        0     3480 2023-03-09 21:28:25.704627 aleksis_core-3.0b2/aleksis/core/frontend/components/app/SideNav.vue
--rw-r--r--   0        0        0     1454 2023-03-09 21:28:25.704627 aleksis_core-3.0b2/aleksis/core/frontend/components/app/SidenavSearch.vue
--rw-r--r--   0        0        0      747 2023-03-09 21:28:25.704627 aleksis_core-3.0b2/aleksis/core/frontend/components/app/SnackbarItem.vue
--rw-r--r--   0        0        0     1932 2023-03-09 21:28:25.704627 aleksis_core-3.0b2/aleksis/core/frontend/components/app/Splash.vue
--rw-r--r--   0        0        0      124 2023-03-09 21:28:25.704627 aleksis_core-3.0b2/aleksis/core/frontend/components/app/customMenu.graphql
--rw-r--r--   0        0        0      205 2023-03-09 21:28:25.704627 aleksis_core-3.0b2/aleksis/core/frontend/components/app/dynamicRoutes.graphql
--rw-r--r--   0        0        0       42 2023-03-09 21:28:25.704627 aleksis_core-3.0b2/aleksis/core/frontend/components/app/messages.graphql
--rw-r--r--   0        0        0       59 2023-03-09 21:28:25.704627 aleksis_core-3.0b2/aleksis/core/frontend/components/app/ping.graphql
--rw-r--r--   0        0        0      139 2023-03-09 21:28:25.704627 aleksis_core-3.0b2/aleksis/core/frontend/components/app/searchSnippets.graphql
--rw-r--r--   0        0        0      323 2023-03-09 21:28:25.704627 aleksis_core-3.0b2/aleksis/core/frontend/components/app/systemProperties.graphql
--rw-r--r--   0        0        0      318 2023-03-09 21:28:25.704627 aleksis_core-3.0b2/aleksis/core/frontend/components/app/whoAmI.graphql
--rw-r--r--   0        0        0     3444 2023-03-09 21:28:25.704627 aleksis_core-3.0b2/aleksis/core/frontend/components/celery_progress/CeleryProgress.vue
--rw-r--r--   0        0        0     1455 2023-03-09 21:28:25.704627 aleksis_core-3.0b2/aleksis/core/frontend/components/celery_progress/CeleryProgressBottom.vue
--rw-r--r--   0        0        0      925 2023-03-09 21:28:25.704627 aleksis_core-3.0b2/aleksis/core/frontend/components/celery_progress/TaskListItem.vue
--rw-r--r--   0        0        0      432 2023-03-09 21:28:25.704627 aleksis_core-3.0b2/aleksis/core/frontend/components/celery_progress/celeryProgress.graphql
--rw-r--r--   0        0        0      191 2023-03-09 21:28:25.704627 aleksis_core-3.0b2/aleksis/core/frontend/components/celery_progress/celeryProgressBottom.graphql
--rw-r--r--   0        0        0      118 2023-03-09 21:28:25.704627 aleksis_core-3.0b2/aleksis/core/frontend/components/celery_progress/celeryProgressFetched.graphql
--rw-r--r--   0        0        0      655 2023-03-09 21:28:25.704627 aleksis_core-3.0b2/aleksis/core/frontend/components/generic/AvatarClickbox.vue
--rw-r--r--   0        0        0      212 2023-03-09 21:28:25.704627 aleksis_core-3.0b2/aleksis/core/frontend/components/generic/BackButton.vue
--rw-r--r--   0        0        0      598 2023-03-09 21:28:25.704627 aleksis_core-3.0b2/aleksis/core/frontend/components/generic/ButtonMenu.vue
--rw-r--r--   0        0        0      981 2023-03-09 21:28:25.704627 aleksis_core-3.0b2/aleksis/core/frontend/components/generic/DetailView.vue
--rw-r--r--   0        0        0      408 2023-03-09 21:28:25.704627 aleksis_core-3.0b2/aleksis/core/frontend/components/generic/ListView.vue
--rw-r--r--   0        0        0      268 2023-03-09 21:28:25.704627 aleksis_core-3.0b2/aleksis/core/frontend/components/generic/MessageBox.vue
--rw-r--r--   0        0        0     1914 2023-03-09 21:28:25.704627 aleksis_core-3.0b2/aleksis/core/frontend/components/generic/ObjectOverview.vue
--rw-r--r--   0        0        0      269 2023-03-09 21:28:25.704627 aleksis_core-3.0b2/aleksis/core/frontend/components/generic/SmallContainer.vue
--rw-r--r--   0        0        0      706 2023-03-09 21:28:25.704627 aleksis_core-3.0b2/aleksis/core/frontend/components/group/GroupCollection.vue
--rw-r--r--   0        0        0     3034 2023-03-09 21:28:25.704627 aleksis_core-3.0b2/aleksis/core/frontend/components/notifications/NotificationItem.vue
--rw-r--r--   0        0        0     2438 2023-03-09 21:28:25.708627 aleksis_core-3.0b2/aleksis/core/frontend/components/notifications/NotificationList.vue
--rw-r--r--   0        0        0      107 2023-03-09 21:28:25.708627 aleksis_core-3.0b2/aleksis/core/frontend/components/notifications/markNotificationRead.graphql
--rw-r--r--   0        0        0      231 2023-03-09 21:28:25.708627 aleksis_core-3.0b2/aleksis/core/frontend/components/notifications/myNotifications.graphql
--rw-r--r--   0        0        0     1017 2023-03-09 21:28:25.708627 aleksis_core-3.0b2/aleksis/core/frontend/components/pdf/DownloadPDF.vue
--rw-r--r--   0        0        0       78 2023-03-09 21:28:25.708627 aleksis_core-3.0b2/aleksis/core/frontend/components/pdf/pdf.graphql
--rw-r--r--   0        0        0     1410 2023-03-09 21:28:25.708627 aleksis_core-3.0b2/aleksis/core/frontend/components/person/AdditionalImage.vue
--rw-r--r--   0        0        0     1082 2023-03-09 21:28:25.708627 aleksis_core-3.0b2/aleksis/core/frontend/components/person/AvatarContent.vue
--rw-r--r--   0        0        0     2892 2023-03-09 21:28:25.708627 aleksis_core-3.0b2/aleksis/core/frontend/components/person/PersonActions.vue
--rw-r--r--   0        0        0      527 2023-03-09 21:28:25.708627 aleksis_core-3.0b2/aleksis/core/frontend/components/person/PersonAvatarClickbox.vue
--rw-r--r--   0        0        0      759 2023-03-09 21:28:25.708627 aleksis_core-3.0b2/aleksis/core/frontend/components/person/PersonCollection.vue
--rw-r--r--   0        0        0     7423 2023-03-09 21:28:25.708627 aleksis_core-3.0b2/aleksis/core/frontend/components/person/PersonOverview.vue
--rw-r--r--   0        0        0      108 2023-03-09 21:28:25.708627 aleksis_core-3.0b2/aleksis/core/frontend/components/person/avatarContent.graphql
--rw-r--r--   0        0        0      196 2023-03-09 21:28:25.708627 aleksis_core-3.0b2/aleksis/core/frontend/components/person/personActions.graphql
--rw-r--r--   0        0        0      575 2023-03-09 21:28:25.708627 aleksis_core-3.0b2/aleksis/core/frontend/components/person/personOverview.graphql
--rw-r--r--   0        0        0     3922 2023-03-09 21:28:25.708627 aleksis_core-3.0b2/aleksis/core/frontend/components/two_factor/TwoFactor.vue
--rw-r--r--   0        0        0     1512 2023-03-09 21:28:25.708627 aleksis_core-3.0b2/aleksis/core/frontend/components/two_factor/TwoFactorDevice.vue
--rw-r--r--   0        0        0      589 2023-03-09 21:28:25.708627 aleksis_core-3.0b2/aleksis/core/frontend/components/two_factor/TwoFactorDeviceBase.vue
--rw-r--r--   0        0        0      385 2023-03-09 21:28:25.708627 aleksis_core-3.0b2/aleksis/core/frontend/components/two_factor/twoFactor.graphql
--rw-r--r--   0        0        0      390 2023-03-09 21:28:25.708627 aleksis_core-3.0b2/aleksis/core/frontend/css/global.scss
--rw-r--r--   0        0        0     2080 2023-03-09 21:28:25.708627 aleksis_core-3.0b2/aleksis/core/frontend/index.js
--rw-r--r--   0        0        0     7121 2023-03-09 21:28:25.708627 aleksis_core-3.0b2/aleksis/core/frontend/messages/de.json
--rw-r--r--   0        0        0     8723 2023-03-09 21:28:25.708627 aleksis_core-3.0b2/aleksis/core/frontend/messages/en.json
--rw-r--r--   0        0        0     9410 2023-03-09 21:28:25.708627 aleksis_core-3.0b2/aleksis/core/frontend/messages/uk.json
--rw-r--r--   0        0        0     1223 2023-03-09 21:28:25.708627 aleksis_core-3.0b2/aleksis/core/frontend/mixins/aleksis.js
--rw-r--r--   0        0        0     3782 2023-03-09 21:28:25.708627 aleksis_core-3.0b2/aleksis/core/frontend/mixins/menus.js
--rw-r--r--   0        0        0     2256 2023-03-09 21:28:25.708627 aleksis_core-3.0b2/aleksis/core/frontend/mixins/offline.js
--rw-r--r--   0        0        0     1708 2023-03-09 21:28:25.708627 aleksis_core-3.0b2/aleksis/core/frontend/mixins/routes.js
--rw-r--r--   0        0        0     1619 2023-03-09 21:28:25.708627 aleksis_core-3.0b2/aleksis/core/frontend/mixins/useRegisterSW.js
--rw-r--r--   0        0        0     4988 2023-03-09 21:28:25.708627 aleksis_core-3.0b2/aleksis/core/frontend/plugins/aleksis.js
--rw-r--r--   0        0        0      450 2023-03-09 21:28:25.708627 aleksis_core-3.0b2/aleksis/core/frontend/routeValidators.js
--rw-r--r--   0        0        0    36469 2023-03-09 21:28:25.708627 aleksis_core-3.0b2/aleksis/core/frontend/routes.js
--rw-r--r--   0        0        0     2642 2023-03-09 21:28:25.708627 aleksis_core-3.0b2/aleksis/core/health_checks.py
--rw-r--r--   0        0        0      487 2023-03-09 21:36:23.227809 aleksis_core-3.0b2/aleksis/core/locale/ar/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    74177 2023-03-09 21:28:25.712627 aleksis_core-3.0b2/aleksis/core/locale/ar/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      463 2023-03-09 21:36:23.255809 aleksis_core-3.0b2/aleksis/core/locale/ar/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0      894 2023-03-09 21:28:25.712627 aleksis_core-3.0b2/aleksis/core/locale/ar/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0    63478 2023-03-09 21:36:23.239809 aleksis_core-3.0b2/aleksis/core/locale/de_DE/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0   124380 2023-03-09 21:28:25.712627 aleksis_core-3.0b2/aleksis/core/locale/de_DE/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      567 2023-03-09 21:36:23.231809 aleksis_core-3.0b2/aleksis/core/locale/de_DE/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0     1118 2023-03-09 21:28:25.712627 aleksis_core-3.0b2/aleksis/core/locale/de_DE/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0      942 2023-03-09 21:36:23.139809 aleksis_core-3.0b2/aleksis/core/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    77598 2023-03-09 21:28:25.712627 aleksis_core-3.0b2/aleksis/core/locale/fr/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      379 2023-03-09 21:36:23.151809 aleksis_core-3.0b2/aleksis/core/locale/fr/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0      810 2023-03-09 21:28:25.712627 aleksis_core-3.0b2/aleksis/core/locale/fr/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0     2584 2023-03-09 21:36:23.039809 aleksis_core-3.0b2/aleksis/core/locale/la/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    82641 2023-03-09 21:28:25.712627 aleksis_core-3.0b2/aleksis/core/locale/la/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      337 2023-03-09 21:36:23.195809 aleksis_core-3.0b2/aleksis/core/locale/la/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0      764 2023-03-09 21:28:25.712627 aleksis_core-3.0b2/aleksis/core/locale/la/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0      361 2023-03-09 21:36:23.079809 aleksis_core-3.0b2/aleksis/core/locale/nb_NO/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    74107 2023-03-09 21:28:25.712627 aleksis_core-3.0b2/aleksis/core/locale/nb_NO/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      337 2023-03-09 21:36:23.091809 aleksis_core-3.0b2/aleksis/core/locale/nb_NO/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0      764 2023-03-09 21:28:25.712627 aleksis_core-3.0b2/aleksis/core/locale/nb_NO/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0    75414 2023-03-09 21:36:23.195809 aleksis_core-3.0b2/aleksis/core/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0   133798 2023-03-09 21:28:25.712627 aleksis_core-3.0b2/aleksis/core/locale/ru/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      713 2023-03-09 21:36:23.123809 aleksis_core-3.0b2/aleksis/core/locale/ru/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0     1321 2023-03-09 21:28:25.712627 aleksis_core-3.0b2/aleksis/core/locale/ru/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0      361 2023-03-09 21:36:23.111809 aleksis_core-3.0b2/aleksis/core/locale/tr_TR/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    74047 2023-03-09 21:28:25.712627 aleksis_core-3.0b2/aleksis/core/locale/tr_TR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      337 2023-03-09 21:36:23.055809 aleksis_core-3.0b2/aleksis/core/locale/tr_TR/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0      764 2023-03-09 21:28:25.712627 aleksis_core-3.0b2/aleksis/core/locale/tr_TR/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0    74488 2023-03-09 21:36:23.259809 aleksis_core-3.0b2/aleksis/core/locale/uk/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0   132729 2023-03-09 21:28:25.716627 aleksis_core-3.0b2/aleksis/core/locale/uk/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      713 2023-03-09 21:36:23.263809 aleksis_core-3.0b2/aleksis/core/locale/uk/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0     1331 2023-03-09 21:28:25.716627 aleksis_core-3.0b2/aleksis/core/locale/uk/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0        0 2023-03-09 21:28:25.716627 aleksis_core-3.0b2/aleksis/core/management/__init__.py
--rw-r--r--   0        0        0     3957 2023-03-09 21:28:25.716627 aleksis_core-3.0b2/aleksis/core/management/commands/convert_urls_to_routes.py
--rw-r--r--   0        0        0      945 2023-03-09 21:28:25.716627 aleksis_core-3.0b2/aleksis/core/management/commands/vite.py
--rw-r--r--   0        0        0      439 2023-03-09 21:28:25.716627 aleksis_core-3.0b2/aleksis/core/management/commands/webpack_bundle.py
--rw-r--r--   0        0        0     4690 2023-03-09 21:28:25.716627 aleksis_core-3.0b2/aleksis/core/managers.py
--rw-r--r--   0        0        0    51004 2023-03-09 21:28:25.716627 aleksis_core-3.0b2/aleksis/core/migrations/0001_initial.py
--rw-r--r--   0        0        0     2473 2023-03-09 21:28:25.716627 aleksis_core-3.0b2/aleksis/core/migrations/0002_school_term.py
--rw-r--r--   0        0        0      531 2023-03-09 21:28:25.716627 aleksis_core-3.0b2/aleksis/core/migrations/0003_drop_image_cropping.py
--rw-r--r--   0        0        0      796 2023-03-09 21:28:25.716627 aleksis_core-3.0b2/aleksis/core/migrations/0004_add_permissions_for_group_stats.py
--rw-r--r--   0        0        0     1252 2023-03-09 21:28:25.716627 aleksis_core-3.0b2/aleksis/core/migrations/0005_timestamped_activity_notification.py
--rw-r--r--   0        0        0     1567 2023-03-09 21:28:25.716627 aleksis_core-3.0b2/aleksis/core/migrations/0006_dashboard_widget_size.py
--rw-r--r--   0        0        0     1396 2023-03-09 21:28:25.716627 aleksis_core-3.0b2/aleksis/core/migrations/0007_dashboard_widget_order.py
--rw-r--r--   0        0        0     2311 2023-03-09 21:28:25.716627 aleksis_core-3.0b2/aleksis/core/migrations/0008_data_check_result.py
--rw-r--r--   0        0        0     1052 2023-03-09 21:28:25.716627 aleksis_core-3.0b2/aleksis/core/migrations/0009_default_dashboard.py
--rw-r--r--   0        0        0      952 2023-03-09 21:28:25.716627 aleksis_core-3.0b2/aleksis/core/migrations/0010_external_link_widget.py
--rw-r--r--   0        0        0      829 2023-03-09 21:28:25.716627 aleksis_core-3.0b2/aleksis/core/migrations/0011_globalpermissions_options.py
--rw-r--r--   0        0        0      501 2023-03-09 21:28:25.716627 aleksis_core-3.0b2/aleksis/core/migrations/0012_valid_from_announcement.py
--rw-r--r--   0        0        0     2270 2023-03-09 21:28:25.716627 aleksis_core-3.0b2/aleksis/core/migrations/0013_pdf_file.py
--rw-r--r--   0        0        0      533 2023-03-09 21:28:25.716627 aleksis_core-3.0b2/aleksis/core/migrations/0014_alter_pdffile_file.py
--rw-r--r--   0        0        0     1174 2023-03-09 21:28:25.716627 aleksis_core-3.0b2/aleksis/core/migrations/0015_oauth_permissions.py
--rw-r--r--   0        0        0     1538 2023-03-09 21:28:25.716627 aleksis_core-3.0b2/aleksis/core/migrations/0016_taskuserassignment.py
--rw-r--r--   0        0        0      426 2023-03-09 21:28:25.716627 aleksis_core-3.0b2/aleksis/core/migrations/0017_dashboardwidget_broken.py
--rw-r--r--   0        0        0      897 2023-03-09 21:28:25.716627 aleksis_core-3.0b2/aleksis/core/migrations/0018_pdffile_html_file.py
--rw-r--r--   0        0        0     2177 2023-03-09 21:28:25.716627 aleksis_core-3.0b2/aleksis/core/migrations/0019_fix_uniqueness_per_site.py
--rw-r--r--   0        0        0      542 2023-03-09 21:28:25.716627 aleksis_core-3.0b2/aleksis/core/migrations/0020_pdf_file_person_optional.py
--rw-r--r--   0        0        0     1084 2023-03-09 21:28:25.716627 aleksis_core-3.0b2/aleksis/core/migrations/0021_drop_persons_accounts_perm.py
--rw-r--r--   0        0        0      923 2023-03-09 21:28:25.716627 aleksis_core-3.0b2/aleksis/core/migrations/0022_public_favicon.py
--rw-r--r--   0        0        0     6340 2023-03-09 21:28:25.716627 aleksis_core-3.0b2/aleksis/core/migrations/0023_oauth_application_model.py
--rw-r--r--   0        0        0      714 2023-03-09 21:28:25.716627 aleksis_core-3.0b2/aleksis/core/migrations/0024_oauth_grant_types_optional.py
--rw-r--r--   0        0        0     1717 2023-03-09 21:28:25.716627 aleksis_core-3.0b2/aleksis/core/migrations/0025_oauth_align_user_fk.py
--rw-r--r--   0        0        0      582 2023-03-09 21:28:25.716627 aleksis_core-3.0b2/aleksis/core/migrations/0026_oauthapplication_allowed_scopes.py
--rw-r--r--   0        0        0      457 2023-03-09 21:28:25.716627 aleksis_core-3.0b2/aleksis/core/migrations/0027_person_place_of_birth.py
--rw-r--r--   0        0        0      947 2023-03-09 21:28:25.716627 aleksis_core-3.0b2/aleksis/core/migrations/0028_char_field_not_null.py
--rw-r--r--   0        0        0     1465 2023-03-09 21:28:25.716627 aleksis_core-3.0b2/aleksis/core/migrations/0029_invitations.py
--rw-r--r--   0        0        0     1776 2023-03-09 21:28:25.716627 aleksis_core-3.0b2/aleksis/core/migrations/0030_user_attributes.py
--rw-r--r--   0        0        0      526 2023-03-09 21:28:25.716627 aleksis_core-3.0b2/aleksis/core/migrations/0031_oauthapplication_icon.py
--rw-r--r--   0        0        0      340 2023-03-09 21:28:25.716627 aleksis_core-3.0b2/aleksis/core/migrations/0032_remove_person_is_active.py
--rw-r--r--   0        0        0     2416 2023-03-09 21:28:25.716627 aleksis_core-3.0b2/aleksis/core/migrations/0033_update_photo_avatar.py
--rw-r--r--   0        0        0      816 2023-03-09 21:28:25.716627 aleksis_core-3.0b2/aleksis/core/migrations/0034_invite_permission.py
--rw-r--r--   0        0        0     1781 2023-03-09 21:28:25.716627 aleksis_core-3.0b2/aleksis/core/migrations/0035_preference_model_unique.py
--rw-r--r--   0        0        0      626 2023-03-09 21:28:25.716627 aleksis_core-3.0b2/aleksis/core/migrations/0036_additionalfields_helptext_required.py
--rw-r--r--   0        0        0      917 2023-03-09 21:28:25.716627 aleksis_core-3.0b2/aleksis/core/migrations/0037_add_static_content_widget.py
--rw-r--r--   0        0        0      522 2023-03-09 21:28:25.716627 aleksis_core-3.0b2/aleksis/core/migrations/0038_notification_send_at.py
--rw-r--r--   0        0        0     1029 2023-03-09 21:28:25.716627 aleksis_core-3.0b2/aleksis/core/migrations/0039_personal_ical_url.py
--rw-r--r--   0        0        0      613 2023-03-09 21:28:25.716627 aleksis_core-3.0b2/aleksis/core/migrations/0040_oauth_allowed_scopes_max_length_255.py
--rw-r--r--   0        0        0      516 2023-03-09 21:28:25.716627 aleksis_core-3.0b2/aleksis/core/migrations/0041_update_gender_choices.py
--rw-r--r--   0        0        0      547 2023-03-09 21:28:25.716627 aleksis_core-3.0b2/aleksis/core/migrations/0042_pdffile_empty.py
--rw-r--r--   0        0        0     2261 2023-03-09 21:28:25.716627 aleksis_core-3.0b2/aleksis/core/migrations/0043_task_assignment_meta.py
--rw-r--r--   0        0        0      532 2023-03-09 21:28:25.716627 aleksis_core-3.0b2/aleksis/core/migrations/0044_task_assignment_result_fetched.py
--rw-r--r--   0        0        0      486 2023-03-09 21:28:25.716627 aleksis_core-3.0b2/aleksis/core/migrations/0045_data_check_result_fix_check_field.py
--rw-r--r--   0        0        0   290966 2023-03-09 21:28:25.720627 aleksis_core-3.0b2/aleksis/core/migrations/0046_notification_create_field_icon.py
--rw-r--r--   0        0        0     2717 2023-03-09 21:28:25.720627 aleksis_core-3.0b2/aleksis/core/migrations/0047_add_room_model.py
--rw-r--r--   0        0        0   893996 2023-03-09 21:28:25.724627 aleksis_core-3.0b2/aleksis/core/migrations/0048_delete_personalicalurl.py
--rw-r--r--   0        0        0        0 2023-03-09 21:28:25.724627 aleksis_core-3.0b2/aleksis/core/migrations/__init__.py
--rw-r--r--   0        0        0    19163 2023-03-09 21:28:25.724627 aleksis_core-3.0b2/aleksis/core/mixins.py
--rw-r--r--   0        0        0    50787 2023-03-09 21:28:25.724627 aleksis_core-3.0b2/aleksis/core/models.py
--rw-r--r--   0        0        0    13810 2023-03-09 21:28:25.724627 aleksis_core-3.0b2/aleksis/core/preferences.py
--rw-r--r--   0        0        0      692 2023-03-09 21:28:25.724627 aleksis_core-3.0b2/aleksis/core/registries.py
--rw-r--r--   0        0        0    15800 2023-03-09 21:28:25.724627 aleksis_core-3.0b2/aleksis/core/rules.py
--rw-r--r--   0        0        0     7090 2023-03-09 21:28:25.728627 aleksis_core-3.0b2/aleksis/core/schema/__init__.py
--rw-r--r--   0        0        0      695 2023-03-09 21:28:25.728627 aleksis_core-3.0b2/aleksis/core/schema/base.py
--rw-r--r--   0        0        0     3052 2023-03-09 21:28:25.728627 aleksis_core-3.0b2/aleksis/core/schema/celery_progress.py
--rw-r--r--   0        0        0      585 2023-03-09 21:28:25.728627 aleksis_core-3.0b2/aleksis/core/schema/custom_menu.py
--rw-r--r--   0        0        0      459 2023-03-09 21:28:25.728627 aleksis_core-3.0b2/aleksis/core/schema/dynamic_routes.py
--rw-r--r--   0        0        0      148 2023-03-09 21:28:25.728627 aleksis_core-3.0b2/aleksis/core/schema/group.py
--rw-r--r--   0        0        0     1743 2023-03-09 21:28:25.728627 aleksis_core-3.0b2/aleksis/core/schema/installed_apps.py
--rw-r--r--   0        0        0      265 2023-03-09 21:28:25.728627 aleksis_core-3.0b2/aleksis/core/schema/message.py
--rw-r--r--   0        0        0      789 2023-03-09 21:28:25.728627 aleksis_core-3.0b2/aleksis/core/schema/notification.py
--rw-r--r--   0        0        0      276 2023-03-09 21:28:25.728627 aleksis_core-3.0b2/aleksis/core/schema/pdf.py
--rw-r--r--   0        0        0      124 2023-03-09 21:28:25.728627 aleksis_core-3.0b2/aleksis/core/schema/permissions.py
--rw-r--r--   0        0        0     7929 2023-03-09 21:28:25.728627 aleksis_core-3.0b2/aleksis/core/schema/person.py
--rw-r--r--   0        0        0      163 2023-03-09 21:28:25.728627 aleksis_core-3.0b2/aleksis/core/schema/school_term.py
--rw-r--r--   0        0        0      868 2023-03-09 21:28:25.728627 aleksis_core-3.0b2/aleksis/core/schema/search.py
--rw-r--r--   0        0        0     1343 2023-03-09 21:28:25.728627 aleksis_core-3.0b2/aleksis/core/schema/site_preferences.py
--rw-r--r--   0        0        0     1395 2023-03-09 21:28:25.728627 aleksis_core-3.0b2/aleksis/core/schema/system_properties.py
--rw-r--r--   0        0        0     3297 2023-03-09 21:28:25.728627 aleksis_core-3.0b2/aleksis/core/schema/two_factor.py
--rw-r--r--   0        0        0      789 2023-03-09 21:28:25.728627 aleksis_core-3.0b2/aleksis/core/schema/user.py
--rw-r--r--   0        0        0      418 2023-03-09 21:28:25.728627 aleksis_core-3.0b2/aleksis/core/search_indexes.py
--rw-r--r--   0        0        0    39383 2023-03-09 21:28:25.728627 aleksis_core-3.0b2/aleksis/core/settings.py
--rw-r--r--   0        0        0    49621 2023-03-09 21:28:25.728627 aleksis_core-3.0b2/aleksis/core/static/img/aleksis-banner.svg
--rw-r--r--   0        0        0     1862 2023-03-09 21:28:25.728627 aleksis_core-3.0b2/aleksis/core/static/img/aleksis-favicon.png
--rw-r--r--   0        0        0    17172 2023-03-09 21:28:25.728627 aleksis_core-3.0b2/aleksis/core/static/img/aleksis-icon-maskable.png
--rw-r--r--   0        0        0     7843 2023-03-09 21:28:25.728627 aleksis_core-3.0b2/aleksis/core/static/img/aleksis-icon-maskable.svg
--rw-r--r--   0        0        0    31902 2023-03-09 21:28:25.728627 aleksis_core-3.0b2/aleksis/core/static/img/aleksis-icon.png
--rw-r--r--   0        0        0     7346 2023-03-09 21:28:25.728627 aleksis_core-3.0b2/aleksis/core/static/img/aleksis-icon.svg
--rw-r--r--   0        0        0    19126 2023-03-09 21:28:25.728627 aleksis_core-3.0b2/aleksis/core/static/img/fallback.png
--rw-r--r--   0        0        0     2237 2023-03-09 21:28:25.728627 aleksis_core-3.0b2/aleksis/core/static/img/hero.svg
--rw-r--r--   0        0        0      490 2023-03-09 21:28:25.728627 aleksis_core-3.0b2/aleksis/core/static/js/copy_button.js
--rw-r--r--   0        0        0      521 2023-03-09 21:28:25.728627 aleksis_core-3.0b2/aleksis/core/static/js/edit_dashboard.js
--rw-r--r--   0        0        0      618 2023-03-09 21:28:25.728627 aleksis_core-3.0b2/aleksis/core/static/js/helper.js
--rw-r--r--   0        0        0      984 2023-03-09 21:28:25.728627 aleksis_core-3.0b2/aleksis/core/static/js/include_ajax_live.js
--rw-r--r--   0        0        0     4350 2023-03-09 21:28:25.728627 aleksis_core-3.0b2/aleksis/core/static/js/main.js
--rw-r--r--   0        0        0     1654 2023-03-09 21:28:25.732627 aleksis_core-3.0b2/aleksis/core/static/js/multi_select.js
--rw-r--r--   0        0        0     3495 2023-03-09 21:28:25.732627 aleksis_core-3.0b2/aleksis/core/static/js/search.js
--rw-r--r--   0        0        0     2578 2023-03-09 21:28:25.732627 aleksis_core-3.0b2/aleksis/core/static/js/serviceworker.js
--rw-r--r--   0        0        0      271 2023-03-09 21:28:25.732627 aleksis_core-3.0b2/aleksis/core/static/print-simple.css
--rw-r--r--   0        0        0     1627 2023-03-09 21:28:25.732627 aleksis_core-3.0b2/aleksis/core/static/print.css
--rw-r--r--   0        0        0      187 2023-03-09 21:28:25.732627 aleksis_core-3.0b2/aleksis/core/static/print_landscape.css
--rw-r--r--   0        0        0     1064 2023-03-09 21:28:25.732627 aleksis_core-3.0b2/aleksis/core/static/public/materialize-custom.scss
--rw-r--r--   0        0        0    15745 2023-03-09 21:28:25.732627 aleksis_core-3.0b2/aleksis/core/static/public/style.scss
--rw-r--r--   0        0        0    11345 2023-03-09 21:28:25.732627 aleksis_core-3.0b2/aleksis/core/static/public/theme.scss
--rw-r--r--   0        0        0     7038 2023-03-09 21:28:25.732627 aleksis_core-3.0b2/aleksis/core/tables.py
--rw-r--r--   0        0        0     2330 2023-03-09 21:28:25.732627 aleksis_core-3.0b2/aleksis/core/tasks.py
--rw-r--r--   0        0        0      838 2023-03-09 21:28:25.732627 aleksis_core-3.0b2/aleksis/core/templates/403.html
--rw-r--r--   0        0        0      789 2023-03-09 21:28:25.732627 aleksis_core-3.0b2/aleksis/core/templates/404.html
--rw-r--r--   0        0        0      921 2023-03-09 21:28:25.732627 aleksis_core-3.0b2/aleksis/core/templates/500.html
--rw-r--r--   0        0        0       76 2023-03-09 21:28:25.732627 aleksis_core-3.0b2/aleksis/core/templates/503.html
--rw-r--r--   0        0        0      851 2023-03-09 21:28:25.732627 aleksis_core-3.0b2/aleksis/core/templates/account/account_inactive.html
--rw-r--r--   0        0        0      169 2023-03-09 21:28:25.732627 aleksis_core-3.0b2/aleksis/core/templates/account/email/base_message.txt
--rw-r--r--   0        0        0     1255 2023-03-09 21:28:25.732627 aleksis_core-3.0b2/aleksis/core/templates/account/email_confirm.html
--rw-r--r--   0        0        0      804 2023-03-09 21:28:25.732627 aleksis_core-3.0b2/aleksis/core/templates/account/password_change.html
--rw-r--r--   0        0        0      888 2023-03-09 21:28:25.732627 aleksis_core-3.0b2/aleksis/core/templates/account/password_change_disabled.html
--rw-r--r--   0        0        0     1376 2023-03-09 21:28:25.732627 aleksis_core-3.0b2/aleksis/core/templates/account/password_reset.html
--rw-r--r--   0        0        0      825 2023-03-09 21:28:25.732627 aleksis_core-3.0b2/aleksis/core/templates/account/password_reset_done.html
--rw-r--r--   0        0        0     2305 2023-03-09 21:28:25.732627 aleksis_core-3.0b2/aleksis/core/templates/account/password_reset_from_key.html
--rw-r--r--   0        0        0      649 2023-03-09 21:28:25.732627 aleksis_core-3.0b2/aleksis/core/templates/account/password_reset_from_key_done.html
--rw-r--r--   0        0        0      500 2023-03-09 21:28:25.732627 aleksis_core-3.0b2/aleksis/core/templates/account/password_set.html
--rw-r--r--   0        0        0      888 2023-03-09 21:28:25.732627 aleksis_core-3.0b2/aleksis/core/templates/account/signup.html
--rw-r--r--   0        0        0      838 2023-03-09 21:28:25.732627 aleksis_core-3.0b2/aleksis/core/templates/account/signup_closed.html
--rw-r--r--   0        0        0      820 2023-03-09 21:28:25.732627 aleksis_core-3.0b2/aleksis/core/templates/account/verification_email_required.html
--rw-r--r--   0        0        0     1160 2023-03-09 21:28:25.732627 aleksis_core-3.0b2/aleksis/core/templates/account/verification_sent.html
--rw-r--r--   0        0        0      979 2023-03-09 21:28:25.732627 aleksis_core-3.0b2/aleksis/core/templates/components/chips.html
--rw-r--r--   0        0        0      350 2023-03-09 21:28:25.732627 aleksis_core-3.0b2/aleksis/core/templates/components/materialize-chips.html
--rw-r--r--   0        0        0      225 2023-03-09 21:28:25.732627 aleksis_core-3.0b2/aleksis/core/templates/components/msgbox.html
--rw-r--r--   0        0        0      958 2023-03-09 21:28:25.732627 aleksis_core-3.0b2/aleksis/core/templates/components/pagination.html
--rw-r--r--   0        0        0      486 2023-03-09 21:28:25.732627 aleksis_core-3.0b2/aleksis/core/templates/components/text_collapsible.html
--rw-r--r--   0        0        0      483 2023-03-09 21:28:25.732627 aleksis_core-3.0b2/aleksis/core/templates/core/additional_field/edit.html
--rw-r--r--   0        0        0      594 2023-03-09 21:28:25.732627 aleksis_core-3.0b2/aleksis/core/templates/core/additional_field/list.html
--rw-r--r--   0        0        0     1053 2023-03-09 21:28:25.732627 aleksis_core-3.0b2/aleksis/core/templates/core/announcement/form.html
--rw-r--r--   0        0        0     1900 2023-03-09 21:28:25.732627 aleksis_core-3.0b2/aleksis/core/templates/core/announcement/list.html
--rw-r--r--   0        0        0     3099 2023-03-09 21:28:25.732627 aleksis_core-3.0b2/aleksis/core/templates/core/base.html
--rw-r--r--   0        0        0     2454 2023-03-09 21:28:25.732627 aleksis_core-3.0b2/aleksis/core/templates/core/base_print.html
--rw-r--r--   0        0        0     1178 2023-03-09 21:28:25.732627 aleksis_core-3.0b2/aleksis/core/templates/core/base_simple_print.html
--rw-r--r--   0        0        0      628 2023-03-09 21:28:25.732627 aleksis_core-3.0b2/aleksis/core/templates/core/dashboard_widget/create.html
--rw-r--r--   0        0        0      635 2023-03-09 21:28:25.732627 aleksis_core-3.0b2/aleksis/core/templates/core/dashboard_widget/dashboardwidget_broken.html
--rw-r--r--   0        0        0      626 2023-03-09 21:28:25.732627 aleksis_core-3.0b2/aleksis/core/templates/core/dashboard_widget/edit.html
--rw-r--r--   0        0        0      262 2023-03-09 21:28:25.732627 aleksis_core-3.0b2/aleksis/core/templates/core/dashboard_widget/external_link_widget.html
--rw-r--r--   0        0        0     1349 2023-03-09 21:28:25.732627 aleksis_core-3.0b2/aleksis/core/templates/core/dashboard_widget/list.html
--rw-r--r--   0        0        0      226 2023-03-09 21:28:25.732627 aleksis_core-3.0b2/aleksis/core/templates/core/dashboard_widget/static_content_widget.html
--rw-r--r--   0        0        0     3746 2023-03-09 21:28:25.732627 aleksis_core-3.0b2/aleksis/core/templates/core/data_check/list.html
--rw-r--r--   0        0        0     2233 2023-03-09 21:28:25.732627 aleksis_core-3.0b2/aleksis/core/templates/core/edit_dashboard.html
--rw-r--r--   0        0        0        0 2023-03-09 21:28:25.732627 aleksis_core-3.0b2/aleksis/core/templates/core/empty.html
--rw-r--r--   0        0        0     5310 2023-03-09 21:28:25.732627 aleksis_core-3.0b2/aleksis/core/templates/core/group/child_groups.html
--rw-r--r--   0        0        0      650 2023-03-09 21:28:25.732627 aleksis_core-3.0b2/aleksis/core/templates/core/group/edit.html
--rw-r--r--   0        0        0     3382 2023-03-09 21:28:25.732627 aleksis_core-3.0b2/aleksis/core/templates/core/group/full.html
--rw-r--r--   0        0        0     1019 2023-03-09 21:28:25.732627 aleksis_core-3.0b2/aleksis/core/templates/core/group/list.html
--rw-r--r--   0        0        0      465 2023-03-09 21:28:25.732627 aleksis_core-3.0b2/aleksis/core/templates/core/group_type/edit.html
--rw-r--r--   0        0        0      564 2023-03-09 21:28:25.732627 aleksis_core-3.0b2/aleksis/core/templates/core/group_type/list.html
--rw-r--r--   0        0        0     2504 2023-03-09 21:28:25.732627 aleksis_core-3.0b2/aleksis/core/templates/core/index.html
--rw-r--r--   0        0        0      777 2023-03-09 21:28:25.732627 aleksis_core-3.0b2/aleksis/core/templates/core/pages/delete.html
--rw-r--r--   0        0        0     6835 2023-03-09 21:28:25.736627 aleksis_core-3.0b2/aleksis/core/templates/core/pages/system_status.html
--rw-r--r--   0        0        0      603 2023-03-09 21:28:25.736627 aleksis_core-3.0b2/aleksis/core/templates/core/pages/test_pdf.html
--rw-r--r--   0        0        0       93 2023-03-09 21:28:25.736627 aleksis_core-3.0b2/aleksis/core/templates/core/partials/address.html
--rw-r--r--   0        0        0      189 2023-03-09 21:28:25.736627 aleksis_core-3.0b2/aleksis/core/templates/core/partials/admins_list.html
--rw-r--r--   0        0        0     1632 2023-03-09 21:28:25.736627 aleksis_core-3.0b2/aleksis/core/templates/core/partials/announcements.html
--rw-r--r--   0        0        0     1472 2023-03-09 21:28:25.736627 aleksis_core-3.0b2/aleksis/core/templates/core/partials/avatar_content.html
--rw-r--r--   0        0        0      319 2023-03-09 21:28:25.736627 aleksis_core-3.0b2/aleksis/core/templates/core/partials/copy_button.html
--rw-r--r--   0        0        0     1089 2023-03-09 21:28:25.736627 aleksis_core-3.0b2/aleksis/core/templates/core/partials/crud_events.html
--rw-r--r--   0        0        0      389 2023-03-09 21:28:25.736627 aleksis_core-3.0b2/aleksis/core/templates/core/partials/edit_dashboard_widget.html
--rw-r--r--   0        0        0     1624 2023-03-09 21:28:25.736627 aleksis_core-3.0b2/aleksis/core/templates/core/partials/meta.html
--rw-r--r--   0        0        0      414 2023-03-09 21:28:25.736627 aleksis_core-3.0b2/aleksis/core/templates/core/partials/on_page_menu.html
--rw-r--r--   0        0        0      260 2023-03-09 21:28:25.736627 aleksis_core-3.0b2/aleksis/core/templates/core/partials/save_button.html
--rw-r--r--   0        0        0     2374 2023-03-09 21:28:25.736627 aleksis_core-3.0b2/aleksis/core/templates/core/partials/splash_screen.html
--rw-r--r--   0        0        0      325 2023-03-09 21:28:25.736627 aleksis_core-3.0b2/aleksis/core/templates/core/partials/turnable.html
--rw-r--r--   0        0        0      915 2023-03-09 21:28:25.736627 aleksis_core-3.0b2/aleksis/core/templates/core/perms/assign.html
--rw-r--r--   0        0        0     2478 2023-03-09 21:28:25.736627 aleksis_core-3.0b2/aleksis/core/templates/core/perms/list.html
--rw-r--r--   0        0        0      376 2023-03-09 21:28:25.736627 aleksis_core-3.0b2/aleksis/core/templates/core/person/collection.html
--rw-r--r--   0        0        0      649 2023-03-09 21:28:25.736627 aleksis_core-3.0b2/aleksis/core/templates/core/person/create.html
--rw-r--r--   0        0        0      645 2023-03-09 21:28:25.736627 aleksis_core-3.0b2/aleksis/core/templates/core/person/edit.html
--rw-r--r--   0        0        0     1165 2023-03-09 21:28:25.736627 aleksis_core-3.0b2/aleksis/core/templates/core/person/list.html
--rw-r--r--   0        0        0      455 2023-03-09 21:28:25.736627 aleksis_core-3.0b2/aleksis/core/templates/core/school_term/create.html
--rw-r--r--   0        0        0      451 2023-03-09 21:28:25.736627 aleksis_core-3.0b2/aleksis/core/templates/core/school_term/edit.html
--rw-r--r--   0        0        0      556 2023-03-09 21:28:25.736627 aleksis_core-3.0b2/aleksis/core/templates/core/school_term/list.html
--rw-r--r--   0        0        0      935 2023-03-09 21:28:25.736627 aleksis_core-3.0b2/aleksis/core/templates/core/vue_index.html
--rw-r--r--   0        0        0     3921 2023-03-09 21:28:25.736627 aleksis_core-3.0b2/aleksis/core/templates/django_tables2/materialize.html
--rw-r--r--   0        0        0      981 2023-03-09 21:28:25.736627 aleksis_core-3.0b2/aleksis/core/templates/dynamic_preferences/form.html
--rw-r--r--   0        0        0      376 2023-03-09 21:28:25.736627 aleksis_core-3.0b2/aleksis/core/templates/dynamic_preferences/sections.html
--rw-r--r--   0        0        0      764 2023-03-09 21:28:25.736627 aleksis_core-3.0b2/aleksis/core/templates/invitations/disabled.html
--rw-r--r--   0        0        0     1281 2023-03-09 21:28:25.736627 aleksis_core-3.0b2/aleksis/core/templates/invitations/enter.html
--rw-r--r--   0        0        0     1060 2023-03-09 21:28:25.736627 aleksis_core-3.0b2/aleksis/core/templates/invitations/forms/_invite.html
--rw-r--r--   0        0        0      102 2023-03-09 21:28:25.736627 aleksis_core-3.0b2/aleksis/core/templates/invitations/messages/invite_accepted.txt
--rw-r--r--   0        0        0      171 2023-03-09 21:28:25.736627 aleksis_core-3.0b2/aleksis/core/templates/material/field_errors.html
--rw-r--r--   0        0        0     1232 2023-03-09 21:28:25.736627 aleksis_core-3.0b2/aleksis/core/templates/material/fields/ckeditor_ckeditorwidget.html
--rw-r--r--   0        0        0     1897 2023-03-09 21:28:25.736627 aleksis_core-3.0b2/aleksis/core/templates/material/fields/colorfield_colorwidget.html
--rw-r--r--   0        0        0     1009 2023-03-09 21:28:25.736627 aleksis_core-3.0b2/aleksis/core/templates/material/fields/django_select2_modelselect2multiplewidget.html
--rw-r--r--   0        0        0     1009 2023-03-09 21:28:25.736627 aleksis_core-3.0b2/aleksis/core/templates/material/fields/django_select2_select2widget.html
--rw-r--r--   0        0        0      253 2023-03-09 21:28:25.736627 aleksis_core-3.0b2/aleksis/core/templates/material/non_field_errors.html
--rw-r--r--   0        0        0      663 2023-03-09 21:28:25.736627 aleksis_core-3.0b2/aleksis/core/templates/oauth2_provider/application/create.html
--rw-r--r--   0        0        0     2335 2023-03-09 21:28:25.736627 aleksis_core-3.0b2/aleksis/core/templates/oauth2_provider/application/detail.html
--rw-r--r--   0        0        0      669 2023-03-09 21:28:25.736627 aleksis_core-3.0b2/aleksis/core/templates/oauth2_provider/application/edit.html
--rw-r--r--   0        0        0     1074 2023-03-09 21:28:25.736627 aleksis_core-3.0b2/aleksis/core/templates/oauth2_provider/application/list.html
--rw-r--r--   0        0        0     2686 2023-03-09 21:28:25.736627 aleksis_core-3.0b2/aleksis/core/templates/oauth2_provider/authorize.html
--rw-r--r--   0        0        0      877 2023-03-09 21:28:25.736627 aleksis_core-3.0b2/aleksis/core/templates/oauth2_provider/authorized-token-delete.html
--rw-r--r--   0        0        0     1256 2023-03-09 21:28:25.736627 aleksis_core-3.0b2/aleksis/core/templates/oauth2_provider/authorized-tokens.html
--rw-r--r--   0        0        0      759 2023-03-09 21:28:25.736627 aleksis_core-3.0b2/aleksis/core/templates/offline.html
--rw-r--r--   0        0        0       42 2023-03-09 21:28:25.736627 aleksis_core-3.0b2/aleksis/core/templates/search/indexes/core/group_text.txt
--rw-r--r--   0        0        0       69 2023-03-09 21:28:25.736627 aleksis_core-3.0b2/aleksis/core/templates/search/indexes/core/person_text.txt
--rw-r--r--   0        0        0       42 2023-03-09 21:28:25.736627 aleksis_core-3.0b2/aleksis/core/templates/search/indexes/core/room_text.txt
--rw-r--r--   0        0        0     3171 2023-03-09 21:28:25.736627 aleksis_core-3.0b2/aleksis/core/templates/search/search.html
--rw-r--r--   0        0        0      243 2023-03-09 21:28:25.736627 aleksis_core-3.0b2/aleksis/core/templates/search/searchbar_snippet.html
--rw-r--r--   0        0        0      150 2023-03-09 21:28:25.736627 aleksis_core-3.0b2/aleksis/core/templates/search/searchbar_snippets.html
--rw-r--r--   0        0        0      169 2023-03-09 21:28:25.736627 aleksis_core-3.0b2/aleksis/core/templates/sms/notification.txt
--rw-r--r--   0        0        0      893 2023-03-09 21:28:25.736627 aleksis_core-3.0b2/aleksis/core/templates/socialaccount/authentication_error.html
--rw-r--r--   0        0        0     1268 2023-03-09 21:28:25.736627 aleksis_core-3.0b2/aleksis/core/templates/socialaccount/connections.html
--rw-r--r--   0        0        0     1289 2023-03-09 21:28:25.736627 aleksis_core-3.0b2/aleksis/core/templates/socialaccount/login.html
--rw-r--r--   0        0        0      809 2023-03-09 21:28:25.736627 aleksis_core-3.0b2/aleksis/core/templates/socialaccount/login_cancelled.html
--rw-r--r--   0        0        0     1012 2023-03-09 21:28:25.736627 aleksis_core-3.0b2/aleksis/core/templates/socialaccount/signup.html
--rw-r--r--   0        0        0     1434 2023-03-09 21:28:25.736627 aleksis_core-3.0b2/aleksis/core/templates/socialaccount/snippets/provider_list.html
--rw-r--r--   0        0        0      630 2023-03-09 21:28:25.736627 aleksis_core-3.0b2/aleksis/core/templates/templated_email/base.email
--rw-r--r--   0        0        0     1527 2023-03-09 21:28:25.736627 aleksis_core-3.0b2/aleksis/core/templates/templated_email/celery_failure.email
--rw-r--r--   0        0        0      994 2023-03-09 21:28:25.736627 aleksis_core-3.0b2/aleksis/core/templates/templated_email/data_checks.email
--rw-r--r--   0        0        0      990 2023-03-09 21:28:25.736627 aleksis_core-3.0b2/aleksis/core/templates/templated_email/email.css
--rw-r--r--   0        0        0     1461 2023-03-09 21:28:25.736627 aleksis_core-3.0b2/aleksis/core/templates/templated_email/notification.email
--rw-r--r--   0        0        0      668 2023-03-09 21:28:25.736627 aleksis_core-3.0b2/aleksis/core/templates/templated_email/person_changed.email
--rw-r--r--   0        0        0      219 2023-03-09 21:28:25.736627 aleksis_core-3.0b2/aleksis/core/templates/two_factor/_base_focus.html
--rw-r--r--   0        0        0      877 2023-03-09 21:28:25.736627 aleksis_core-3.0b2/aleksis/core/templates/two_factor/_wizard_actions.html
--rw-r--r--   0        0        0      119 2023-03-09 21:28:25.736627 aleksis_core-3.0b2/aleksis/core/templates/two_factor/_wizard_forms.html
--rw-r--r--   0        0        0     1780 2023-03-09 21:28:25.736627 aleksis_core-3.0b2/aleksis/core/templates/two_factor/core/backup_tokens.html
--rw-r--r--   0        0        0     6712 2023-03-09 21:28:25.736627 aleksis_core-3.0b2/aleksis/core/templates/two_factor/core/login.html
--rw-r--r--   0        0        0      943 2023-03-09 21:28:25.740627 aleksis_core-3.0b2/aleksis/core/templates/two_factor/core/otp_required.html
--rw-r--r--   0        0        0      986 2023-03-09 21:28:25.740627 aleksis_core-3.0b2/aleksis/core/templates/two_factor/core/phone_register.html
--rw-r--r--   0        0        0     3312 2023-03-09 21:28:25.740627 aleksis_core-3.0b2/aleksis/core/templates/two_factor/core/setup.html
--rw-r--r--   0        0        0     2127 2023-03-09 21:28:25.740627 aleksis_core-3.0b2/aleksis/core/templates/two_factor/core/setup_complete.html
--rw-r--r--   0        0        0      786 2023-03-09 21:28:25.740627 aleksis_core-3.0b2/aleksis/core/templates/two_factor/profile/disable.html
--rw-r--r--   0        0        0        0 2023-03-09 21:28:25.740627 aleksis_core-3.0b2/aleksis/core/templatetags/__init__.py
--rw-r--r--   0        0        0       99 2023-03-09 21:28:25.740627 aleksis_core-3.0b2/aleksis/core/templatetags/apps.py
--rw-r--r--   0        0        0      394 2023-03-09 21:28:25.740627 aleksis_core-3.0b2/aleksis/core/templatetags/dashboard.py
--rw-r--r--   0        0        0     1618 2023-03-09 21:28:25.740627 aleksis_core-3.0b2/aleksis/core/templatetags/data_helpers.py
--rw-r--r--   0        0        0     1134 2023-03-09 21:28:25.740627 aleksis_core-3.0b2/aleksis/core/templatetags/html_helpers.py
--rw-r--r--   0        0        0      206 2023-03-09 21:28:25.740627 aleksis_core-3.0b2/aleksis/core/templatetags/msg_box.py
--rw-r--r--   0        0        0     3696 2023-03-09 21:28:25.740627 aleksis_core-3.0b2/aleksis/core/tests/browser/test_selenium.py
--rw-r--r--   0        0        0     6596 2023-03-09 21:28:25.740627 aleksis_core-3.0b2/aleksis/core/tests/models/test.pdf
--rw-r--r--   0        0        0     6562 2023-03-09 21:28:25.740627 aleksis_core-3.0b2/aleksis/core/tests/models/test_group.py
--rw-r--r--   0        0        0     1520 2023-03-09 21:28:25.740627 aleksis_core-3.0b2/aleksis/core/tests/models/test_group_sync.py
--rw-r--r--   0        0        0     3049 2023-03-09 21:28:25.740627 aleksis_core-3.0b2/aleksis/core/tests/models/test_notification.py
--rw-r--r--   0        0        0     4003 2023-03-09 21:28:25.740627 aleksis_core-3.0b2/aleksis/core/tests/models/test_pdffile.py
--rw-r--r--   0        0        0      427 2023-03-09 21:28:25.740627 aleksis_core-3.0b2/aleksis/core/tests/models/test_person.py
--rw-r--r--   0        0        0     5503 2023-03-09 21:28:25.740627 aleksis_core-3.0b2/aleksis/core/tests/regression/test_regression.py
--rw-r--r--   0        0        0      683 2023-03-09 21:28:25.740627 aleksis_core-3.0b2/aleksis/core/tests/regression/view_oauth.py
--rw-r--r--   0        0        0     1021 2023-03-09 21:28:25.740627 aleksis_core-3.0b2/aleksis/core/tests/templatetags/test_data_helpers.py
--rw-r--r--   0        0        0     2292 2023-03-09 21:28:25.740627 aleksis_core-3.0b2/aleksis/core/tests/views/test_account.py
--rw-r--r--   0        0        0    18516 2023-03-09 21:28:25.740627 aleksis_core-3.0b2/aleksis/core/urls.py
--rw-r--r--   0        0        0        0 2023-03-09 21:28:25.740627 aleksis_core-3.0b2/aleksis/core/util/__init__.py
--rw-r--r--   0        0        0      176 2023-03-09 21:36:20.699813 aleksis_core-3.0b2/aleksis/core/util/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0    13545 2023-03-09 21:36:21.547812 aleksis_core-3.0b2/aleksis/core/util/__pycache__/apps.cpython-311.pyc
--rw-r--r--   0        0        0    10101 2023-03-09 21:36:22.487810 aleksis_core-3.0b2/aleksis/core/util/__pycache__/celery_progress.cpython-311.pyc
--rw-r--r--   0        0        0    24932 2023-03-09 21:36:20.707813 aleksis_core-3.0b2/aleksis/core/util/__pycache__/core_helpers.cpython-311.pyc
--rw-r--r--   0        0        0     1500 2023-03-09 21:36:20.883813 aleksis_core-3.0b2/aleksis/core/util/__pycache__/email.cpython-311.pyc
--rw-r--r--   0        0        0      771 2023-03-09 21:36:22.499810 aleksis_core-3.0b2/aleksis/core/util/__pycache__/model_helpers.cpython-311.pyc
--rw-r--r--   0        0        0     5712 2023-03-09 21:36:22.491810 aleksis_core-3.0b2/aleksis/core/util/__pycache__/notifications.cpython-311.pyc
--rw-r--r--   0        0        0     9548 2023-03-09 21:36:22.675810 aleksis_core-3.0b2/aleksis/core/util/__pycache__/predicates.cpython-311.pyc
--rw-r--r--   0        0        0     2181 2023-03-09 21:36:21.555812 aleksis_core-3.0b2/aleksis/core/util/__pycache__/sass_helpers.cpython-311.pyc
--rw-r--r--   0        0        0      664 2023-03-09 21:36:21.551812 aleksis_core-3.0b2/aleksis/core/util/__pycache__/spdx.cpython-311.pyc
--rw-r--r--   0        0        0    10028 2023-03-09 21:28:25.740627 aleksis_core-3.0b2/aleksis/core/util/apps.py
--rw-r--r--   0        0        0     5970 2023-03-09 21:28:25.740627 aleksis_core-3.0b2/aleksis/core/util/auth_helpers.py
--rw-r--r--   0        0        0     7920 2023-03-09 21:28:25.740627 aleksis_core-3.0b2/aleksis/core/util/celery_progress.py
--rw-r--r--   0        0        0      197 2023-03-09 21:28:25.740627 aleksis_core-3.0b2/aleksis/core/util/context_processors.py
--rw-r--r--   0        0        0    16042 2023-03-09 21:28:25.740627 aleksis_core-3.0b2/aleksis/core/util/core_helpers.py
--rw-r--r--   0        0        0      986 2023-03-09 21:28:25.740627 aleksis_core-3.0b2/aleksis/core/util/email.py
--rw-r--r--   0        0        0     1175 2023-03-09 21:28:25.740627 aleksis_core-3.0b2/aleksis/core/util/forms.py
--rw-r--r--   0        0        0     2895 2023-03-09 21:28:25.740627 aleksis_core-3.0b2/aleksis/core/util/frontend_helpers.py
--rw-r--r--   0        0        0     2375 2023-03-09 21:28:25.740627 aleksis_core-3.0b2/aleksis/core/util/ldap.py
--rw-r--r--   0        0        0   192829 2023-03-09 21:28:25.740627 aleksis_core-3.0b2/aleksis/core/util/licenses.json
--rw-r--r--   0        0        0     2255 2023-03-09 21:28:25.740627 aleksis_core-3.0b2/aleksis/core/util/messages.py
--rw-r--r--   0        0        0     2091 2023-03-09 21:28:25.740627 aleksis_core-3.0b2/aleksis/core/util/middlewares.py
--rw-r--r--   0        0        0      850 2023-03-09 21:28:25.740627 aleksis_core-3.0b2/aleksis/core/util/model_helpers.py
--rw-r--r--   0        0        0     3732 2023-03-09 21:28:25.740627 aleksis_core-3.0b2/aleksis/core/util/notifications.py
--rw-r--r--   0        0        0     6131 2023-03-09 21:28:25.744627 aleksis_core-3.0b2/aleksis/core/util/pdf.py
--rw-r--r--   0        0        0     5583 2023-03-09 21:28:25.744627 aleksis_core-3.0b2/aleksis/core/util/predicates.py
--rw-r--r--   0        0        0      936 2023-03-09 21:28:25.744627 aleksis_core-3.0b2/aleksis/core/util/sass_helpers.py
--rw-r--r--   0        0        0      524 2023-03-09 21:28:25.744627 aleksis_core-3.0b2/aleksis/core/util/search.py
--rw-r--r--   0        0        0      130 2023-03-09 21:28:25.744627 aleksis_core-3.0b2/aleksis/core/util/spdx.py
--rw-r--r--   0        0        0     1673 2023-03-09 21:28:25.744627 aleksis_core-3.0b2/aleksis/core/util/tables.py
--rw-r--r--   0        0        0    54591 2023-03-09 21:28:25.744627 aleksis_core-3.0b2/aleksis/core/views.py
--rw-r--r--   0        0        0    10201 2023-03-09 21:28:25.744627 aleksis_core-3.0b2/aleksis/core/vite.config.js
--rw-r--r--   0        0        0      173 2023-03-09 21:28:25.744627 aleksis_core-3.0b2/aleksis/core/wsgi.py
--rw-r--r--   0        0        0       45 2023-03-09 21:28:25.744627 aleksis_core-3.0b2/conftest.py
--rw-r--r--   0        0        0      581 2023-03-09 21:28:25.744627 aleksis_core-3.0b2/docs/Makefile
--rw-r--r--   0        0        0   127432 2023-03-09 21:28:25.744627 aleksis_core-3.0b2/docs/_static/2fa.png
--rw-r--r--   0        0        0    71362 2023-03-09 21:28:25.744627 aleksis_core-3.0b2/docs/_static/accept_invite.png
--rw-r--r--   0        0        0    72621 2023-03-09 21:28:25.748627 aleksis_core-3.0b2/docs/_static/create_dashboard_widget.png
--rw-r--r--   0        0        0    41935 2023-03-09 21:28:25.748627 aleksis_core-3.0b2/docs/_static/create_social_application.png
--rw-r--r--   0        0        0    72508 2023-03-09 21:28:25.748627 aleksis_core-3.0b2/docs/_static/dashboard.png
--rw-r--r--   0        0        0    87601 2023-03-09 21:28:25.748627 aleksis_core-3.0b2/docs/_static/dashboard_widgets.png
--rw-r--r--   0        0        0   119523 2023-03-09 21:28:25.748627 aleksis_core-3.0b2/docs/_static/data_checks.png
--rw-r--r--   0        0        0    81386 2023-03-09 21:28:25.748627 aleksis_core-3.0b2/docs/_static/edit_dashboard.png
--rw-r--r--   0        0        0    85722 2023-03-09 21:28:25.752627 aleksis_core-3.0b2/docs/_static/edit_default_dashboard.png
--rw-r--r--   0        0        0   107979 2023-03-09 21:28:25.752627 aleksis_core-3.0b2/docs/_static/invitations.png
--rw-r--r--   0        0        0   177681 2023-03-09 21:28:25.752627 aleksis_core-3.0b2/docs/_static/invite_existing.png
--rw-r--r--   0        0        0    44868 2023-03-09 21:28:25.752627 aleksis_core-3.0b2/docs/_static/pwa_desktop_chromium.png
--rw-r--r--   0        0        0    69215 2023-03-09 21:28:25.756627 aleksis_core-3.0b2/docs/_static/pwa_mobile_chromium.png
--rw-r--r--   0        0        0   128479 2023-03-09 21:28:25.756627 aleksis_core-3.0b2/docs/_static/pwa_mobile_firefox.png
--rw-r--r--   0        0        0   108973 2023-03-09 21:28:25.756627 aleksis_core-3.0b2/docs/_static/pwa_mobile_safari.png
--rw-r--r--   0        0        0    69804 2023-03-09 21:28:25.756627 aleksis_core-3.0b2/docs/_static/signup.png
--rw-r--r--   0        0        0      132 2023-03-09 21:28:25.756627 aleksis_core-3.0b2/docs/admin/00_index.rst
--rw-r--r--   0        0        0     4231 2023-03-09 21:28:25.756627 aleksis_core-3.0b2/docs/admin/01_core_concepts.rst
--rw-r--r--   0        0        0     8059 2023-03-09 21:28:25.756627 aleksis_core-3.0b2/docs/admin/10_install.rst
--rw-r--r--   0        0        0     1872 2023-03-09 21:28:25.756627 aleksis_core-3.0b2/docs/admin/15_config_files.rst
--rw-r--r--   0        0        0     1982 2023-03-09 21:28:25.756627 aleksis_core-3.0b2/docs/admin/16_config_options.rst
--rw-r--r--   0        0        0     1648 2023-03-09 21:28:25.756627 aleksis_core-3.0b2/docs/admin/17_storage.rst
--rw-r--r--   0        0        0      803 2023-03-09 21:28:25.756627 aleksis_core-3.0b2/docs/admin/18_mail.rst
--rw-r--r--   0        0        0     1509 2023-03-09 21:28:25.756627 aleksis_core-3.0b2/docs/admin/21_ldap.rst
--rw-r--r--   0        0        0     3037 2023-03-09 21:28:25.756627 aleksis_core-3.0b2/docs/admin/22_registration.rst
--rw-r--r--   0        0        0     1467 2023-03-09 21:28:25.756627 aleksis_core-3.0b2/docs/admin/23_socialaccounts.rst
--rw-r--r--   0        0        0     3218 2023-03-09 21:28:25.756627 aleksis_core-3.0b2/docs/admin/31_monitoring.rst
--rw-r--r--   0        0        0     1012 2023-03-09 21:28:25.756627 aleksis_core-3.0b2/docs/admin/32_tasks.rst
--rw-r--r--   0        0        0     1393 2023-03-09 21:28:25.756627 aleksis_core-3.0b2/docs/admin/33_data_checks.rst
--rw-r--r--   0        0        0     4610 2023-03-09 21:28:25.756627 aleksis_core-3.0b2/docs/admin/50_dashboard.rst
--rw-r--r--   0        0        0     6393 2023-03-09 21:28:25.760627 aleksis_core-3.0b2/docs/conf.py
--rw-r--r--   0        0        0      132 2023-03-09 21:28:25.760627 aleksis_core-3.0b2/docs/dev/00_index.rst
--rw-r--r--   0        0        0     4002 2023-03-09 21:28:25.760627 aleksis_core-3.0b2/docs/dev/01_setup.rst
--rw-r--r--   0        0        0     1427 2023-03-09 21:28:25.760627 aleksis_core-3.0b2/docs/dev/02_install_apps.rst
--rw-r--r--   0        0        0     3117 2023-03-09 21:28:25.760627 aleksis_core-3.0b2/docs/dev/03_run_tests.rst
--rw-r--r--   0        0        0     4519 2023-03-09 21:28:25.760627 aleksis_core-3.0b2/docs/dev/04_materialize_templates.rst
--rw-r--r--   0        0        0      289 2023-03-09 21:28:25.760627 aleksis_core-3.0b2/docs/dev/05_extensible_models.rst
--rw-r--r--   0        0        0     1148 2023-03-09 21:28:25.760627 aleksis_core-3.0b2/docs/dev/06_merging_app_settings.rst
--rw-r--r--   0        0        0     1349 2023-03-09 21:28:25.760627 aleksis_core-3.0b2/docs/dev/10_dashboard_widgets.rst
--rw-r--r--   0        0        0      514 2023-03-09 21:28:25.760627 aleksis_core-3.0b2/docs/index.rst
--rw-r--r--   0        0        0      787 2023-03-09 21:28:25.760627 aleksis_core-3.0b2/docs/make.bat
--rw-r--r--   0        0        0       95 2023-03-09 21:28:25.760627 aleksis_core-3.0b2/docs/ref/00_index.rst
--rw-r--r--   0        0        0       69 2023-03-09 21:28:25.760627 aleksis_core-3.0b2/docs/ref/core/01_checks.rst
--rw-r--r--   0        0        0       70 2023-03-09 21:28:25.760627 aleksis_core-3.0b2/docs/ref/core/02_managers.rst
--rw-r--r--   0        0        0       64 2023-03-09 21:28:25.760627 aleksis_core-3.0b2/docs/ref/core/03_mixins.rst
--rw-r--r--   0        0        0       84 2023-03-09 21:28:25.760627 aleksis_core-3.0b2/docs/ref/core/04_models.rst
--rw-r--r--   0        0        0      108 2023-03-09 21:28:25.760627 aleksis_core-3.0b2/docs/ref/core/05_registries.rst
--rw-r--r--   0        0        0       93 2023-03-09 21:28:25.760627 aleksis_core-3.0b2/docs/ref/core/06_search_indexes.rst
--rw-r--r--   0        0        0       79 2023-03-09 21:28:25.760627 aleksis_core-3.0b2/docs/ref/core/07_tables.rst
--rw-r--r--   0        0        0       90 2023-03-09 21:28:25.760627 aleksis_core-3.0b2/docs/ref/core/08_tasks.rst
--rw-r--r--   0        0        0     1017 2023-03-09 21:28:25.760627 aleksis_core-3.0b2/docs/ref/core/09_utils.rst
--rw-r--r--   0        0        0       71 2023-03-09 21:28:25.760627 aleksis_core-3.0b2/docs/ref/core/10_views.rst
--rw-r--r--   0        0        0       77 2023-03-09 21:28:25.760627 aleksis_core-3.0b2/docs/ref/core/11_filters.rst
--rw-r--r--   0        0        0      373 2023-03-09 21:28:25.760627 aleksis_core-3.0b2/docs/ref/core/12_template_tags.rst
--rw-r--r--   0        0        0      112 2023-03-09 21:28:25.760627 aleksis_core-3.0b2/docs/user/00_index.rst
--rw-r--r--   0        0        0     1152 2023-03-09 21:28:25.760627 aleksis_core-3.0b2/docs/user/01_registration.rst
--rw-r--r--   0        0        0     3465 2023-03-09 21:28:25.760627 aleksis_core-3.0b2/docs/user/02_personal_account.rst
--rw-r--r--   0        0        0     1770 2023-03-09 21:28:25.760627 aleksis_core-3.0b2/docs/user/10_dashboard.rst
--rw-r--r--   0        0        0     2607 2023-03-09 21:28:25.760627 aleksis_core-3.0b2/docs/user/20_pwa.rst
--rw-r--r--   0        0        0     4574 2023-03-09 21:34:54.479961 aleksis_core-3.0b2/pyproject.toml
--rw-r--r--   0        0        0     2599 2023-03-09 21:28:25.760627 aleksis_core-3.0b2/tox.ini
--rw-r--r--   0        0        0    10359 1970-01-01 00:00:00.000000 aleksis_core-3.0b2/setup.py
--rw-r--r--   0        0        0     8557 1970-01-01 00:00:00.000000 aleksis_core-3.0b2/PKG-INFO
+-rw-r--r--   0        0        0    33652 2023-03-19 19:24:31.222830 aleksis_core-3.0b3/CHANGELOG.rst
+-rw-r--r--   0        0        0    14353 2023-03-19 19:24:31.222830 aleksis_core-3.0b3/LICENCE.rst
+-rw-r--r--   0        0        0     3780 2023-03-19 19:24:31.222830 aleksis_core-3.0b3/README.rst
+-rw-r--r--   0        0        0      194 2023-03-19 19:24:31.222830 aleksis_core-3.0b3/aleksis/core/__init__.py
+-rw-r--r--   0        0        0      464 2023-03-19 19:24:31.222830 aleksis_core-3.0b3/aleksis/core/__main__.py
+-rw-r--r--   0        0        0      510 2023-03-19 19:32:06.766033 aleksis_core-3.0b3/aleksis/core/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1068 2023-03-19 19:32:07.526031 aleksis_core-3.0b3/aleksis/core/__pycache__/__main__.cpython-311.pyc
+-rw-r--r--   0        0        0     2061 2023-03-19 19:32:09.306028 aleksis_core-3.0b3/aleksis/core/__pycache__/admin.cpython-311.pyc
+-rw-r--r--   0        0        0    10911 2023-03-19 19:32:08.114030 aleksis_core-3.0b3/aleksis/core/__pycache__/apps.cpython-311.pyc
+-rw-r--r--   0        0        0     2533 2023-03-19 19:32:06.834032 aleksis_core-3.0b3/aleksis/core/__pycache__/celery.cpython-311.pyc
+-rw-r--r--   0        0        0     3716 2023-03-19 19:32:09.362028 aleksis_core-3.0b3/aleksis/core/__pycache__/checks.cpython-311.pyc
+-rw-r--r--   0        0        0    17897 2023-03-19 19:32:09.130028 aleksis_core-3.0b3/aleksis/core/__pycache__/data_checks.cpython-311.pyc
+-rw-r--r--   0        0        0     5154 2023-03-19 19:32:09.370028 aleksis_core-3.0b3/aleksis/core/__pycache__/health_checks.cpython-311.pyc
+-rw-r--r--   0        0        0     8423 2023-03-19 19:32:09.146028 aleksis_core-3.0b3/aleksis/core/__pycache__/managers.cpython-311.pyc
+-rw-r--r--   0        0        0    30729 2023-03-19 19:32:09.134028 aleksis_core-3.0b3/aleksis/core/__pycache__/mixins.cpython-311.pyc
+-rw-r--r--   0        0        0    84345 2023-03-19 19:32:08.922029 aleksis_core-3.0b3/aleksis/core/__pycache__/models.cpython-311.pyc
+-rw-r--r--   0        0        0    22958 2023-03-19 19:32:09.390028 aleksis_core-3.0b3/aleksis/core/__pycache__/preferences.cpython-311.pyc
+-rw-r--r--   0        0        0     1370 2023-03-19 19:32:08.130030 aleksis_core-3.0b3/aleksis/core/__pycache__/registries.cpython-311.pyc
+-rw-r--r--   0        0        0    16523 2023-03-19 19:32:09.322028 aleksis_core-3.0b3/aleksis/core/__pycache__/rules.cpython-311.pyc
+-rw-r--r--   0        0        0    43405 2023-03-19 19:32:07.542031 aleksis_core-3.0b3/aleksis/core/__pycache__/settings.cpython-311.pyc
+-rw-r--r--   0        0        0     3825 2023-03-19 19:32:09.154028 aleksis_core-3.0b3/aleksis/core/__pycache__/tasks.cpython-311.pyc
+-rw-r--r--   0        0        0      950 2023-03-19 19:24:31.222830 aleksis_core-3.0b3/aleksis/core/admin.py
+-rw-r--r--   0        0        0     8274 2023-03-19 19:24:31.222830 aleksis_core-3.0b3/aleksis/core/apps.py
+-rw-r--r--   0        0        0     1338 2023-03-19 19:24:31.222830 aleksis_core-3.0b3/aleksis/core/celery.py
+-rw-r--r--   0        0        0     2751 2023-03-19 19:24:31.222830 aleksis_core-3.0b3/aleksis/core/checks.py
+-rw-r--r--   0        0        0    11534 2023-03-19 19:24:31.222830 aleksis_core-3.0b3/aleksis/core/data_checks.py
+-rw-r--r--   0        0        0      741 2023-03-19 19:24:31.222830 aleksis_core-3.0b3/aleksis/core/decorators.py
+-rw-r--r--   0        0        0     5556 2023-03-19 19:24:31.222830 aleksis_core-3.0b3/aleksis/core/filters.py
+-rw-r--r--   0        0        0    30812 2023-03-19 19:24:31.222830 aleksis_core-3.0b3/aleksis/core/forms.py
+-rw-r--r--   0        0        0     3000 2023-03-19 19:24:31.226830 aleksis_core-3.0b3/aleksis/core/frontend/app/apollo.js
+-rw-r--r--   0        0        0      803 2023-03-19 19:24:31.226830 aleksis_core-3.0b3/aleksis/core/frontend/app/dateTimeFormats.js
+-rw-r--r--   0        0        0      197 2023-03-19 19:24:31.226830 aleksis_core-3.0b3/aleksis/core/frontend/app/i18n.js
+-rw-r--r--   0        0        0      157 2023-03-19 19:24:31.226830 aleksis_core-3.0b3/aleksis/core/frontend/app/router.js
+-rw-r--r--   0        0        0      133 2023-03-19 19:24:31.226830 aleksis_core-3.0b3/aleksis/core/frontend/app/sentry.js
+-rw-r--r--   0        0        0      793 2023-03-19 19:24:31.226830 aleksis_core-3.0b3/aleksis/core/frontend/app/vuetify.js
+-rw-r--r--   0        0        0     3014 2023-03-19 19:24:31.226830 aleksis_core-3.0b3/aleksis/core/frontend/components/LegacyBaseTemplate.vue
+-rw-r--r--   0        0        0      158 2023-03-19 19:24:31.226830 aleksis_core-3.0b3/aleksis/core/frontend/components/Parent.vue
+-rw-r--r--   0        0        0      335 2023-03-19 19:24:31.226830 aleksis_core-3.0b3/aleksis/core/frontend/components/about/About.vue
+-rw-r--r--   0        0        0     1971 2023-03-19 19:24:31.226830 aleksis_core-3.0b3/aleksis/core/frontend/components/about/AboutAleksis.vue
+-rw-r--r--   0        0        0     3831 2023-03-19 19:24:31.226830 aleksis_core-3.0b3/aleksis/core/frontend/components/about/InstalledAppCard.vue
+-rw-r--r--   0        0        0     1003 2023-03-19 19:24:31.226830 aleksis_core-3.0b3/aleksis/core/frontend/components/about/InstalledAppsList.vue
+-rw-r--r--   0        0        0      351 2023-03-19 19:24:31.226830 aleksis_core-3.0b3/aleksis/core/frontend/components/about/installedApps.graphql
+-rw-r--r--   0        0        0     2411 2023-03-19 19:24:31.226830 aleksis_core-3.0b3/aleksis/core/frontend/components/app/AccountMenu.vue
+-rw-r--r--   0        0        0     9194 2023-03-19 19:24:31.226830 aleksis_core-3.0b3/aleksis/core/frontend/components/app/App.vue
+-rw-r--r--   0        0        0      314 2023-03-19 19:24:31.226830 aleksis_core-3.0b3/aleksis/core/frontend/components/app/BrandLogo.vue
+-rw-r--r--   0        0        0     1064 2023-03-19 19:24:31.226830 aleksis_core-3.0b3/aleksis/core/frontend/components/app/ErrorPage.vue
+-rw-r--r--   0        0        0     1036 2023-03-19 19:24:31.226830 aleksis_core-3.0b3/aleksis/core/frontend/components/app/LanguageForm.vue
+-rw-r--r--   0        0        0     3480 2023-03-19 19:24:31.226830 aleksis_core-3.0b3/aleksis/core/frontend/components/app/SideNav.vue
+-rw-r--r--   0        0        0     1454 2023-03-19 19:24:31.226830 aleksis_core-3.0b3/aleksis/core/frontend/components/app/SidenavSearch.vue
+-rw-r--r--   0        0        0      747 2023-03-19 19:24:31.226830 aleksis_core-3.0b3/aleksis/core/frontend/components/app/SnackbarItem.vue
+-rw-r--r--   0        0        0     1932 2023-03-19 19:24:31.226830 aleksis_core-3.0b3/aleksis/core/frontend/components/app/Splash.vue
+-rw-r--r--   0        0        0      124 2023-03-19 19:24:31.226830 aleksis_core-3.0b3/aleksis/core/frontend/components/app/customMenu.graphql
+-rw-r--r--   0        0        0      205 2023-03-19 19:24:31.226830 aleksis_core-3.0b3/aleksis/core/frontend/components/app/dynamicRoutes.graphql
+-rw-r--r--   0        0        0       42 2023-03-19 19:24:31.226830 aleksis_core-3.0b3/aleksis/core/frontend/components/app/messages.graphql
+-rw-r--r--   0        0        0       59 2023-03-19 19:24:31.226830 aleksis_core-3.0b3/aleksis/core/frontend/components/app/ping.graphql
+-rw-r--r--   0        0        0      139 2023-03-19 19:24:31.226830 aleksis_core-3.0b3/aleksis/core/frontend/components/app/searchSnippets.graphql
+-rw-r--r--   0        0        0      323 2023-03-19 19:24:31.226830 aleksis_core-3.0b3/aleksis/core/frontend/components/app/systemProperties.graphql
+-rw-r--r--   0        0        0      318 2023-03-19 19:24:31.226830 aleksis_core-3.0b3/aleksis/core/frontend/components/app/whoAmI.graphql
+-rw-r--r--   0        0        0     3444 2023-03-19 19:24:31.226830 aleksis_core-3.0b3/aleksis/core/frontend/components/celery_progress/CeleryProgress.vue
+-rw-r--r--   0        0        0     1455 2023-03-19 19:24:31.226830 aleksis_core-3.0b3/aleksis/core/frontend/components/celery_progress/CeleryProgressBottom.vue
+-rw-r--r--   0        0        0      925 2023-03-19 19:24:31.226830 aleksis_core-3.0b3/aleksis/core/frontend/components/celery_progress/TaskListItem.vue
+-rw-r--r--   0        0        0      432 2023-03-19 19:24:31.226830 aleksis_core-3.0b3/aleksis/core/frontend/components/celery_progress/celeryProgress.graphql
+-rw-r--r--   0        0        0      191 2023-03-19 19:24:31.226830 aleksis_core-3.0b3/aleksis/core/frontend/components/celery_progress/celeryProgressBottom.graphql
+-rw-r--r--   0        0        0      118 2023-03-19 19:24:31.226830 aleksis_core-3.0b3/aleksis/core/frontend/components/celery_progress/celeryProgressFetched.graphql
+-rw-r--r--   0        0        0      655 2023-03-19 19:24:31.226830 aleksis_core-3.0b3/aleksis/core/frontend/components/generic/AvatarClickbox.vue
+-rw-r--r--   0        0        0      212 2023-03-19 19:24:31.226830 aleksis_core-3.0b3/aleksis/core/frontend/components/generic/BackButton.vue
+-rw-r--r--   0        0        0      598 2023-03-19 19:24:31.226830 aleksis_core-3.0b3/aleksis/core/frontend/components/generic/ButtonMenu.vue
+-rw-r--r--   0        0        0      981 2023-03-19 19:24:31.226830 aleksis_core-3.0b3/aleksis/core/frontend/components/generic/DetailView.vue
+-rw-r--r--   0        0        0      408 2023-03-19 19:24:31.226830 aleksis_core-3.0b3/aleksis/core/frontend/components/generic/ListView.vue
+-rw-r--r--   0        0        0      268 2023-03-19 19:24:31.226830 aleksis_core-3.0b3/aleksis/core/frontend/components/generic/MessageBox.vue
+-rw-r--r--   0        0        0     1914 2023-03-19 19:24:31.226830 aleksis_core-3.0b3/aleksis/core/frontend/components/generic/ObjectOverview.vue
+-rw-r--r--   0        0        0      269 2023-03-19 19:24:31.226830 aleksis_core-3.0b3/aleksis/core/frontend/components/generic/SmallContainer.vue
+-rw-r--r--   0        0        0      706 2023-03-19 19:24:31.226830 aleksis_core-3.0b3/aleksis/core/frontend/components/group/GroupCollection.vue
+-rw-r--r--   0        0        0     3034 2023-03-19 19:24:31.226830 aleksis_core-3.0b3/aleksis/core/frontend/components/notifications/NotificationItem.vue
+-rw-r--r--   0        0        0     2438 2023-03-19 19:24:31.226830 aleksis_core-3.0b3/aleksis/core/frontend/components/notifications/NotificationList.vue
+-rw-r--r--   0        0        0      107 2023-03-19 19:24:31.226830 aleksis_core-3.0b3/aleksis/core/frontend/components/notifications/markNotificationRead.graphql
+-rw-r--r--   0        0        0      231 2023-03-19 19:24:31.226830 aleksis_core-3.0b3/aleksis/core/frontend/components/notifications/myNotifications.graphql
+-rw-r--r--   0        0        0     1017 2023-03-19 19:24:31.226830 aleksis_core-3.0b3/aleksis/core/frontend/components/pdf/DownloadPDF.vue
+-rw-r--r--   0        0        0       78 2023-03-19 19:24:31.226830 aleksis_core-3.0b3/aleksis/core/frontend/components/pdf/pdf.graphql
+-rw-r--r--   0        0        0     1410 2023-03-19 19:24:31.226830 aleksis_core-3.0b3/aleksis/core/frontend/components/person/AdditionalImage.vue
+-rw-r--r--   0        0        0     1082 2023-03-19 19:24:31.226830 aleksis_core-3.0b3/aleksis/core/frontend/components/person/AvatarContent.vue
+-rw-r--r--   0        0        0     2892 2023-03-19 19:24:31.226830 aleksis_core-3.0b3/aleksis/core/frontend/components/person/PersonActions.vue
+-rw-r--r--   0        0        0      527 2023-03-19 19:24:31.226830 aleksis_core-3.0b3/aleksis/core/frontend/components/person/PersonAvatarClickbox.vue
+-rw-r--r--   0        0        0      759 2023-03-19 19:24:31.226830 aleksis_core-3.0b3/aleksis/core/frontend/components/person/PersonCollection.vue
+-rw-r--r--   0        0        0     7423 2023-03-19 19:24:31.226830 aleksis_core-3.0b3/aleksis/core/frontend/components/person/PersonOverview.vue
+-rw-r--r--   0        0        0      108 2023-03-19 19:24:31.226830 aleksis_core-3.0b3/aleksis/core/frontend/components/person/avatarContent.graphql
+-rw-r--r--   0        0        0      196 2023-03-19 19:24:31.226830 aleksis_core-3.0b3/aleksis/core/frontend/components/person/personActions.graphql
+-rw-r--r--   0        0        0      575 2023-03-19 19:24:31.226830 aleksis_core-3.0b3/aleksis/core/frontend/components/person/personOverview.graphql
+-rw-r--r--   0        0        0     3922 2023-03-19 19:24:31.230830 aleksis_core-3.0b3/aleksis/core/frontend/components/two_factor/TwoFactor.vue
+-rw-r--r--   0        0        0     1512 2023-03-19 19:24:31.230830 aleksis_core-3.0b3/aleksis/core/frontend/components/two_factor/TwoFactorDevice.vue
+-rw-r--r--   0        0        0      589 2023-03-19 19:24:31.230830 aleksis_core-3.0b3/aleksis/core/frontend/components/two_factor/TwoFactorDeviceBase.vue
+-rw-r--r--   0        0        0      385 2023-03-19 19:24:31.230830 aleksis_core-3.0b3/aleksis/core/frontend/components/two_factor/twoFactor.graphql
+-rw-r--r--   0        0        0      390 2023-03-19 19:24:31.230830 aleksis_core-3.0b3/aleksis/core/frontend/css/global.scss
+-rw-r--r--   0        0        0     2080 2023-03-19 19:24:31.230830 aleksis_core-3.0b3/aleksis/core/frontend/index.js
+-rw-r--r--   0        0        0     7121 2023-03-19 19:24:31.230830 aleksis_core-3.0b3/aleksis/core/frontend/messages/de.json
+-rw-r--r--   0        0        0     8723 2023-03-19 19:24:31.230830 aleksis_core-3.0b3/aleksis/core/frontend/messages/en.json
+-rw-r--r--   0        0        0     9410 2023-03-19 19:24:31.230830 aleksis_core-3.0b3/aleksis/core/frontend/messages/uk.json
+-rw-r--r--   0        0        0     1223 2023-03-19 19:24:31.230830 aleksis_core-3.0b3/aleksis/core/frontend/mixins/aleksis.js
+-rw-r--r--   0        0        0     3782 2023-03-19 19:24:31.230830 aleksis_core-3.0b3/aleksis/core/frontend/mixins/menus.js
+-rw-r--r--   0        0        0     2256 2023-03-19 19:24:31.230830 aleksis_core-3.0b3/aleksis/core/frontend/mixins/offline.js
+-rw-r--r--   0        0        0     1708 2023-03-19 19:24:31.230830 aleksis_core-3.0b3/aleksis/core/frontend/mixins/routes.js
+-rw-r--r--   0        0        0     1619 2023-03-19 19:24:31.230830 aleksis_core-3.0b3/aleksis/core/frontend/mixins/useRegisterSW.js
+-rw-r--r--   0        0        0     4988 2023-03-19 19:24:31.230830 aleksis_core-3.0b3/aleksis/core/frontend/plugins/aleksis.js
+-rw-r--r--   0        0        0      450 2023-03-19 19:24:31.230830 aleksis_core-3.0b3/aleksis/core/frontend/routeValidators.js
+-rw-r--r--   0        0        0    36469 2023-03-19 19:24:31.230830 aleksis_core-3.0b3/aleksis/core/frontend/routes.js
+-rw-r--r--   0        0        0     2642 2023-03-19 19:24:31.230830 aleksis_core-3.0b3/aleksis/core/health_checks.py
+-rw-r--r--   0        0        0      487 2023-03-19 19:32:09.598028 aleksis_core-3.0b3/aleksis/core/locale/ar/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    74177 2023-03-19 19:24:31.230830 aleksis_core-3.0b3/aleksis/core/locale/ar/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      463 2023-03-19 19:32:09.606027 aleksis_core-3.0b3/aleksis/core/locale/ar/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0      894 2023-03-19 19:24:31.230830 aleksis_core-3.0b3/aleksis/core/locale/ar/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0    63478 2023-03-19 19:32:09.614028 aleksis_core-3.0b3/aleksis/core/locale/de_DE/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0   124380 2023-03-19 19:24:31.230830 aleksis_core-3.0b3/aleksis/core/locale/de_DE/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      567 2023-03-19 19:32:09.562028 aleksis_core-3.0b3/aleksis/core/locale/de_DE/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0     1118 2023-03-19 19:24:31.230830 aleksis_core-3.0b3/aleksis/core/locale/de_DE/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0      942 2023-03-19 19:32:09.634028 aleksis_core-3.0b3/aleksis/core/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    77598 2023-03-19 19:24:31.230830 aleksis_core-3.0b3/aleksis/core/locale/fr/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      379 2023-03-19 19:32:09.638028 aleksis_core-3.0b3/aleksis/core/locale/fr/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0      810 2023-03-19 19:24:31.230830 aleksis_core-3.0b3/aleksis/core/locale/fr/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0     2584 2023-03-19 19:32:09.666027 aleksis_core-3.0b3/aleksis/core/locale/la/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    82641 2023-03-19 19:24:31.234830 aleksis_core-3.0b3/aleksis/core/locale/la/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      337 2023-03-19 19:32:09.654027 aleksis_core-3.0b3/aleksis/core/locale/la/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0      764 2023-03-19 19:24:31.234830 aleksis_core-3.0b3/aleksis/core/locale/la/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0      361 2023-03-19 19:32:09.574028 aleksis_core-3.0b3/aleksis/core/locale/nb_NO/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    74107 2023-03-19 19:24:31.234830 aleksis_core-3.0b3/aleksis/core/locale/nb_NO/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      337 2023-03-19 19:32:09.606027 aleksis_core-3.0b3/aleksis/core/locale/nb_NO/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0      764 2023-03-19 19:24:31.234830 aleksis_core-3.0b3/aleksis/core/locale/nb_NO/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0    75414 2023-03-19 19:32:09.702027 aleksis_core-3.0b3/aleksis/core/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0   133798 2023-03-19 19:24:31.234830 aleksis_core-3.0b3/aleksis/core/locale/ru/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      713 2023-03-19 19:32:09.646027 aleksis_core-3.0b3/aleksis/core/locale/ru/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0     1321 2023-03-19 19:24:31.234830 aleksis_core-3.0b3/aleksis/core/locale/ru/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0      361 2023-03-19 19:32:09.626027 aleksis_core-3.0b3/aleksis/core/locale/tr_TR/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    74047 2023-03-19 19:24:31.234830 aleksis_core-3.0b3/aleksis/core/locale/tr_TR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      337 2023-03-19 19:32:09.622027 aleksis_core-3.0b3/aleksis/core/locale/tr_TR/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0      764 2023-03-19 19:24:31.234830 aleksis_core-3.0b3/aleksis/core/locale/tr_TR/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0    74488 2023-03-19 19:32:09.710027 aleksis_core-3.0b3/aleksis/core/locale/uk/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0   132729 2023-03-19 19:24:31.234830 aleksis_core-3.0b3/aleksis/core/locale/uk/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      713 2023-03-19 19:32:09.646027 aleksis_core-3.0b3/aleksis/core/locale/uk/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0     1331 2023-03-19 19:24:31.234830 aleksis_core-3.0b3/aleksis/core/locale/uk/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0        0 2023-03-19 19:24:31.234830 aleksis_core-3.0b3/aleksis/core/management/__init__.py
+-rw-r--r--   0        0        0     3957 2023-03-19 19:24:31.234830 aleksis_core-3.0b3/aleksis/core/management/commands/convert_urls_to_routes.py
+-rw-r--r--   0        0        0      945 2023-03-19 19:24:31.234830 aleksis_core-3.0b3/aleksis/core/management/commands/vite.py
+-rw-r--r--   0        0        0      439 2023-03-19 19:24:31.234830 aleksis_core-3.0b3/aleksis/core/management/commands/webpack_bundle.py
+-rw-r--r--   0        0        0     4690 2023-03-19 19:24:31.234830 aleksis_core-3.0b3/aleksis/core/managers.py
+-rw-r--r--   0        0        0    51004 2023-03-19 19:24:31.234830 aleksis_core-3.0b3/aleksis/core/migrations/0001_initial.py
+-rw-r--r--   0        0        0     2473 2023-03-19 19:24:31.234830 aleksis_core-3.0b3/aleksis/core/migrations/0002_school_term.py
+-rw-r--r--   0        0        0      531 2023-03-19 19:24:31.234830 aleksis_core-3.0b3/aleksis/core/migrations/0003_drop_image_cropping.py
+-rw-r--r--   0        0        0      796 2023-03-19 19:24:31.234830 aleksis_core-3.0b3/aleksis/core/migrations/0004_add_permissions_for_group_stats.py
+-rw-r--r--   0        0        0     1252 2023-03-19 19:24:31.234830 aleksis_core-3.0b3/aleksis/core/migrations/0005_timestamped_activity_notification.py
+-rw-r--r--   0        0        0     1567 2023-03-19 19:24:31.234830 aleksis_core-3.0b3/aleksis/core/migrations/0006_dashboard_widget_size.py
+-rw-r--r--   0        0        0     1396 2023-03-19 19:24:31.234830 aleksis_core-3.0b3/aleksis/core/migrations/0007_dashboard_widget_order.py
+-rw-r--r--   0        0        0     2311 2023-03-19 19:24:31.234830 aleksis_core-3.0b3/aleksis/core/migrations/0008_data_check_result.py
+-rw-r--r--   0        0        0     1052 2023-03-19 19:24:31.234830 aleksis_core-3.0b3/aleksis/core/migrations/0009_default_dashboard.py
+-rw-r--r--   0        0        0      952 2023-03-19 19:24:31.234830 aleksis_core-3.0b3/aleksis/core/migrations/0010_external_link_widget.py
+-rw-r--r--   0        0        0      829 2023-03-19 19:24:31.234830 aleksis_core-3.0b3/aleksis/core/migrations/0011_globalpermissions_options.py
+-rw-r--r--   0        0        0      501 2023-03-19 19:24:31.234830 aleksis_core-3.0b3/aleksis/core/migrations/0012_valid_from_announcement.py
+-rw-r--r--   0        0        0     2270 2023-03-19 19:24:31.234830 aleksis_core-3.0b3/aleksis/core/migrations/0013_pdf_file.py
+-rw-r--r--   0        0        0      533 2023-03-19 19:24:31.234830 aleksis_core-3.0b3/aleksis/core/migrations/0014_alter_pdffile_file.py
+-rw-r--r--   0        0        0     1174 2023-03-19 19:24:31.234830 aleksis_core-3.0b3/aleksis/core/migrations/0015_oauth_permissions.py
+-rw-r--r--   0        0        0     1538 2023-03-19 19:24:31.234830 aleksis_core-3.0b3/aleksis/core/migrations/0016_taskuserassignment.py
+-rw-r--r--   0        0        0      426 2023-03-19 19:24:31.234830 aleksis_core-3.0b3/aleksis/core/migrations/0017_dashboardwidget_broken.py
+-rw-r--r--   0        0        0      897 2023-03-19 19:24:31.234830 aleksis_core-3.0b3/aleksis/core/migrations/0018_pdffile_html_file.py
+-rw-r--r--   0        0        0     2177 2023-03-19 19:24:31.234830 aleksis_core-3.0b3/aleksis/core/migrations/0019_fix_uniqueness_per_site.py
+-rw-r--r--   0        0        0      542 2023-03-19 19:24:31.234830 aleksis_core-3.0b3/aleksis/core/migrations/0020_pdf_file_person_optional.py
+-rw-r--r--   0        0        0     1084 2023-03-19 19:24:31.234830 aleksis_core-3.0b3/aleksis/core/migrations/0021_drop_persons_accounts_perm.py
+-rw-r--r--   0        0        0      923 2023-03-19 19:24:31.234830 aleksis_core-3.0b3/aleksis/core/migrations/0022_public_favicon.py
+-rw-r--r--   0        0        0     6340 2023-03-19 19:24:31.234830 aleksis_core-3.0b3/aleksis/core/migrations/0023_oauth_application_model.py
+-rw-r--r--   0        0        0      714 2023-03-19 19:24:31.234830 aleksis_core-3.0b3/aleksis/core/migrations/0024_oauth_grant_types_optional.py
+-rw-r--r--   0        0        0     1717 2023-03-19 19:24:31.234830 aleksis_core-3.0b3/aleksis/core/migrations/0025_oauth_align_user_fk.py
+-rw-r--r--   0        0        0      582 2023-03-19 19:24:31.234830 aleksis_core-3.0b3/aleksis/core/migrations/0026_oauthapplication_allowed_scopes.py
+-rw-r--r--   0        0        0      457 2023-03-19 19:24:31.234830 aleksis_core-3.0b3/aleksis/core/migrations/0027_person_place_of_birth.py
+-rw-r--r--   0        0        0      947 2023-03-19 19:24:31.234830 aleksis_core-3.0b3/aleksis/core/migrations/0028_char_field_not_null.py
+-rw-r--r--   0        0        0     1465 2023-03-19 19:24:31.234830 aleksis_core-3.0b3/aleksis/core/migrations/0029_invitations.py
+-rw-r--r--   0        0        0     1776 2023-03-19 19:24:31.234830 aleksis_core-3.0b3/aleksis/core/migrations/0030_user_attributes.py
+-rw-r--r--   0        0        0      526 2023-03-19 19:24:31.234830 aleksis_core-3.0b3/aleksis/core/migrations/0031_oauthapplication_icon.py
+-rw-r--r--   0        0        0      340 2023-03-19 19:24:31.234830 aleksis_core-3.0b3/aleksis/core/migrations/0032_remove_person_is_active.py
+-rw-r--r--   0        0        0     2416 2023-03-19 19:24:31.238830 aleksis_core-3.0b3/aleksis/core/migrations/0033_update_photo_avatar.py
+-rw-r--r--   0        0        0      816 2023-03-19 19:24:31.238830 aleksis_core-3.0b3/aleksis/core/migrations/0034_invite_permission.py
+-rw-r--r--   0        0        0     1781 2023-03-19 19:24:31.238830 aleksis_core-3.0b3/aleksis/core/migrations/0035_preference_model_unique.py
+-rw-r--r--   0        0        0      626 2023-03-19 19:24:31.238830 aleksis_core-3.0b3/aleksis/core/migrations/0036_additionalfields_helptext_required.py
+-rw-r--r--   0        0        0      917 2023-03-19 19:24:31.238830 aleksis_core-3.0b3/aleksis/core/migrations/0037_add_static_content_widget.py
+-rw-r--r--   0        0        0      522 2023-03-19 19:24:31.238830 aleksis_core-3.0b3/aleksis/core/migrations/0038_notification_send_at.py
+-rw-r--r--   0        0        0     1029 2023-03-19 19:24:31.238830 aleksis_core-3.0b3/aleksis/core/migrations/0039_personal_ical_url.py
+-rw-r--r--   0        0        0      613 2023-03-19 19:24:31.238830 aleksis_core-3.0b3/aleksis/core/migrations/0040_oauth_allowed_scopes_max_length_255.py
+-rw-r--r--   0        0        0      516 2023-03-19 19:24:31.238830 aleksis_core-3.0b3/aleksis/core/migrations/0041_update_gender_choices.py
+-rw-r--r--   0        0        0      547 2023-03-19 19:24:31.238830 aleksis_core-3.0b3/aleksis/core/migrations/0042_pdffile_empty.py
+-rw-r--r--   0        0        0     2261 2023-03-19 19:24:31.238830 aleksis_core-3.0b3/aleksis/core/migrations/0043_task_assignment_meta.py
+-rw-r--r--   0        0        0      532 2023-03-19 19:24:31.238830 aleksis_core-3.0b3/aleksis/core/migrations/0044_task_assignment_result_fetched.py
+-rw-r--r--   0        0        0      486 2023-03-19 19:24:31.238830 aleksis_core-3.0b3/aleksis/core/migrations/0045_data_check_result_fix_check_field.py
+-rw-r--r--   0        0        0   290966 2023-03-19 19:24:31.238830 aleksis_core-3.0b3/aleksis/core/migrations/0046_notification_create_field_icon.py
+-rw-r--r--   0        0        0     2717 2023-03-19 19:24:31.238830 aleksis_core-3.0b3/aleksis/core/migrations/0047_add_room_model.py
+-rw-r--r--   0        0        0   893996 2023-03-19 19:24:31.242830 aleksis_core-3.0b3/aleksis/core/migrations/0048_delete_personalicalurl.py
+-rw-r--r--   0        0        0        0 2023-03-19 19:24:31.242830 aleksis_core-3.0b3/aleksis/core/migrations/__init__.py
+-rw-r--r--   0        0        0    19163 2023-03-19 19:24:31.242830 aleksis_core-3.0b3/aleksis/core/mixins.py
+-rw-r--r--   0        0        0    50787 2023-03-19 19:24:31.242830 aleksis_core-3.0b3/aleksis/core/models.py
+-rw-r--r--   0        0        0    13810 2023-03-19 19:24:31.242830 aleksis_core-3.0b3/aleksis/core/preferences.py
+-rw-r--r--   0        0        0      692 2023-03-19 19:24:31.242830 aleksis_core-3.0b3/aleksis/core/registries.py
+-rw-r--r--   0        0        0    16018 2023-03-19 19:24:31.242830 aleksis_core-3.0b3/aleksis/core/rules.py
+-rw-r--r--   0        0        0     7090 2023-03-19 19:24:31.242830 aleksis_core-3.0b3/aleksis/core/schema/__init__.py
+-rw-r--r--   0        0        0      695 2023-03-19 19:24:31.242830 aleksis_core-3.0b3/aleksis/core/schema/base.py
+-rw-r--r--   0        0        0     3052 2023-03-19 19:24:31.242830 aleksis_core-3.0b3/aleksis/core/schema/celery_progress.py
+-rw-r--r--   0        0        0      585 2023-03-19 19:24:31.242830 aleksis_core-3.0b3/aleksis/core/schema/custom_menu.py
+-rw-r--r--   0        0        0      459 2023-03-19 19:24:31.242830 aleksis_core-3.0b3/aleksis/core/schema/dynamic_routes.py
+-rw-r--r--   0        0        0     2001 2023-03-19 19:24:31.242830 aleksis_core-3.0b3/aleksis/core/schema/group.py
+-rw-r--r--   0        0        0     1743 2023-03-19 19:24:31.242830 aleksis_core-3.0b3/aleksis/core/schema/installed_apps.py
+-rw-r--r--   0        0        0      265 2023-03-19 19:24:31.242830 aleksis_core-3.0b3/aleksis/core/schema/message.py
+-rw-r--r--   0        0        0     1278 2023-03-19 19:24:31.242830 aleksis_core-3.0b3/aleksis/core/schema/notification.py
+-rw-r--r--   0        0        0      535 2023-03-19 19:24:31.242830 aleksis_core-3.0b3/aleksis/core/schema/pdf.py
+-rw-r--r--   0        0        0      124 2023-03-19 19:24:31.242830 aleksis_core-3.0b3/aleksis/core/schema/permissions.py
+-rw-r--r--   0        0        0     9204 2023-03-19 19:24:31.242830 aleksis_core-3.0b3/aleksis/core/schema/person.py
+-rw-r--r--   0        0        0      163 2023-03-19 19:24:31.242830 aleksis_core-3.0b3/aleksis/core/schema/school_term.py
+-rw-r--r--   0        0        0      868 2023-03-19 19:24:31.242830 aleksis_core-3.0b3/aleksis/core/schema/search.py
+-rw-r--r--   0        0        0     1343 2023-03-19 19:24:31.242830 aleksis_core-3.0b3/aleksis/core/schema/site_preferences.py
+-rw-r--r--   0        0        0     1395 2023-03-19 19:24:31.242830 aleksis_core-3.0b3/aleksis/core/schema/system_properties.py
+-rw-r--r--   0        0        0     3297 2023-03-19 19:24:31.242830 aleksis_core-3.0b3/aleksis/core/schema/two_factor.py
+-rw-r--r--   0        0        0      789 2023-03-19 19:24:31.242830 aleksis_core-3.0b3/aleksis/core/schema/user.py
+-rw-r--r--   0        0        0      418 2023-03-19 19:24:31.242830 aleksis_core-3.0b3/aleksis/core/search_indexes.py
+-rw-r--r--   0        0        0    39383 2023-03-19 19:24:31.246830 aleksis_core-3.0b3/aleksis/core/settings.py
+-rw-r--r--   0        0        0    49621 2023-03-19 19:24:31.246830 aleksis_core-3.0b3/aleksis/core/static/img/aleksis-banner.svg
+-rw-r--r--   0        0        0     1862 2023-03-19 19:24:31.246830 aleksis_core-3.0b3/aleksis/core/static/img/aleksis-favicon.png
+-rw-r--r--   0        0        0    17172 2023-03-19 19:24:31.246830 aleksis_core-3.0b3/aleksis/core/static/img/aleksis-icon-maskable.png
+-rw-r--r--   0        0        0     7843 2023-03-19 19:24:31.246830 aleksis_core-3.0b3/aleksis/core/static/img/aleksis-icon-maskable.svg
+-rw-r--r--   0        0        0    31902 2023-03-19 19:24:31.246830 aleksis_core-3.0b3/aleksis/core/static/img/aleksis-icon.png
+-rw-r--r--   0        0        0     7346 2023-03-19 19:24:31.246830 aleksis_core-3.0b3/aleksis/core/static/img/aleksis-icon.svg
+-rw-r--r--   0        0        0    19126 2023-03-19 19:24:31.246830 aleksis_core-3.0b3/aleksis/core/static/img/fallback.png
+-rw-r--r--   0        0        0     2237 2023-03-19 19:24:31.246830 aleksis_core-3.0b3/aleksis/core/static/img/hero.svg
+-rw-r--r--   0        0        0      490 2023-03-19 19:24:31.246830 aleksis_core-3.0b3/aleksis/core/static/js/copy_button.js
+-rw-r--r--   0        0        0      521 2023-03-19 19:24:31.246830 aleksis_core-3.0b3/aleksis/core/static/js/edit_dashboard.js
+-rw-r--r--   0        0        0      618 2023-03-19 19:24:31.246830 aleksis_core-3.0b3/aleksis/core/static/js/helper.js
+-rw-r--r--   0        0        0      984 2023-03-19 19:24:31.246830 aleksis_core-3.0b3/aleksis/core/static/js/include_ajax_live.js
+-rw-r--r--   0        0        0     4350 2023-03-19 19:24:31.246830 aleksis_core-3.0b3/aleksis/core/static/js/main.js
+-rw-r--r--   0        0        0     1654 2023-03-19 19:24:31.246830 aleksis_core-3.0b3/aleksis/core/static/js/multi_select.js
+-rw-r--r--   0        0        0     3495 2023-03-19 19:24:31.246830 aleksis_core-3.0b3/aleksis/core/static/js/search.js
+-rw-r--r--   0        0        0     2578 2023-03-19 19:24:31.246830 aleksis_core-3.0b3/aleksis/core/static/js/serviceworker.js
+-rw-r--r--   0        0        0      271 2023-03-19 19:24:31.246830 aleksis_core-3.0b3/aleksis/core/static/print-simple.css
+-rw-r--r--   0        0        0     1627 2023-03-19 19:24:31.246830 aleksis_core-3.0b3/aleksis/core/static/print.css
+-rw-r--r--   0        0        0      187 2023-03-19 19:24:31.246830 aleksis_core-3.0b3/aleksis/core/static/print_landscape.css
+-rw-r--r--   0        0        0     1064 2023-03-19 19:24:31.246830 aleksis_core-3.0b3/aleksis/core/static/public/materialize-custom.scss
+-rw-r--r--   0        0        0    15745 2023-03-19 19:24:31.246830 aleksis_core-3.0b3/aleksis/core/static/public/style.scss
+-rw-r--r--   0        0        0    11345 2023-03-19 19:24:31.246830 aleksis_core-3.0b3/aleksis/core/static/public/theme.scss
+-rw-r--r--   0        0        0     7038 2023-03-19 19:24:31.246830 aleksis_core-3.0b3/aleksis/core/tables.py
+-rw-r--r--   0        0        0     2330 2023-03-19 19:24:31.246830 aleksis_core-3.0b3/aleksis/core/tasks.py
+-rw-r--r--   0        0        0      838 2023-03-19 19:24:31.246830 aleksis_core-3.0b3/aleksis/core/templates/403.html
+-rw-r--r--   0        0        0      789 2023-03-19 19:24:31.246830 aleksis_core-3.0b3/aleksis/core/templates/404.html
+-rw-r--r--   0        0        0      921 2023-03-19 19:24:31.246830 aleksis_core-3.0b3/aleksis/core/templates/500.html
+-rw-r--r--   0        0        0       76 2023-03-19 19:24:31.246830 aleksis_core-3.0b3/aleksis/core/templates/503.html
+-rw-r--r--   0        0        0      851 2023-03-19 19:24:31.246830 aleksis_core-3.0b3/aleksis/core/templates/account/account_inactive.html
+-rw-r--r--   0        0        0      169 2023-03-19 19:24:31.246830 aleksis_core-3.0b3/aleksis/core/templates/account/email/base_message.txt
+-rw-r--r--   0        0        0     1255 2023-03-19 19:24:31.246830 aleksis_core-3.0b3/aleksis/core/templates/account/email_confirm.html
+-rw-r--r--   0        0        0      804 2023-03-19 19:24:31.246830 aleksis_core-3.0b3/aleksis/core/templates/account/password_change.html
+-rw-r--r--   0        0        0      888 2023-03-19 19:24:31.246830 aleksis_core-3.0b3/aleksis/core/templates/account/password_change_disabled.html
+-rw-r--r--   0        0        0     1376 2023-03-19 19:24:31.246830 aleksis_core-3.0b3/aleksis/core/templates/account/password_reset.html
+-rw-r--r--   0        0        0      825 2023-03-19 19:24:31.246830 aleksis_core-3.0b3/aleksis/core/templates/account/password_reset_done.html
+-rw-r--r--   0        0        0     2305 2023-03-19 19:24:31.246830 aleksis_core-3.0b3/aleksis/core/templates/account/password_reset_from_key.html
+-rw-r--r--   0        0        0      649 2023-03-19 19:24:31.250830 aleksis_core-3.0b3/aleksis/core/templates/account/password_reset_from_key_done.html
+-rw-r--r--   0        0        0      500 2023-03-19 19:24:31.250830 aleksis_core-3.0b3/aleksis/core/templates/account/password_set.html
+-rw-r--r--   0        0        0      888 2023-03-19 19:24:31.250830 aleksis_core-3.0b3/aleksis/core/templates/account/signup.html
+-rw-r--r--   0        0        0      838 2023-03-19 19:24:31.250830 aleksis_core-3.0b3/aleksis/core/templates/account/signup_closed.html
+-rw-r--r--   0        0        0      820 2023-03-19 19:24:31.250830 aleksis_core-3.0b3/aleksis/core/templates/account/verification_email_required.html
+-rw-r--r--   0        0        0     1160 2023-03-19 19:24:31.250830 aleksis_core-3.0b3/aleksis/core/templates/account/verification_sent.html
+-rw-r--r--   0        0        0      979 2023-03-19 19:24:31.250830 aleksis_core-3.0b3/aleksis/core/templates/components/chips.html
+-rw-r--r--   0        0        0      350 2023-03-19 19:24:31.250830 aleksis_core-3.0b3/aleksis/core/templates/components/materialize-chips.html
+-rw-r--r--   0        0        0      225 2023-03-19 19:24:31.250830 aleksis_core-3.0b3/aleksis/core/templates/components/msgbox.html
+-rw-r--r--   0        0        0      958 2023-03-19 19:24:31.250830 aleksis_core-3.0b3/aleksis/core/templates/components/pagination.html
+-rw-r--r--   0        0        0      486 2023-03-19 19:24:31.250830 aleksis_core-3.0b3/aleksis/core/templates/components/text_collapsible.html
+-rw-r--r--   0        0        0      483 2023-03-19 19:24:31.250830 aleksis_core-3.0b3/aleksis/core/templates/core/additional_field/edit.html
+-rw-r--r--   0        0        0      594 2023-03-19 19:24:31.250830 aleksis_core-3.0b3/aleksis/core/templates/core/additional_field/list.html
+-rw-r--r--   0        0        0     1053 2023-03-19 19:24:31.250830 aleksis_core-3.0b3/aleksis/core/templates/core/announcement/form.html
+-rw-r--r--   0        0        0     1900 2023-03-19 19:24:31.250830 aleksis_core-3.0b3/aleksis/core/templates/core/announcement/list.html
+-rw-r--r--   0        0        0     3099 2023-03-19 19:24:31.250830 aleksis_core-3.0b3/aleksis/core/templates/core/base.html
+-rw-r--r--   0        0        0     2454 2023-03-19 19:24:31.250830 aleksis_core-3.0b3/aleksis/core/templates/core/base_print.html
+-rw-r--r--   0        0        0     1178 2023-03-19 19:24:31.250830 aleksis_core-3.0b3/aleksis/core/templates/core/base_simple_print.html
+-rw-r--r--   0        0        0      628 2023-03-19 19:24:31.250830 aleksis_core-3.0b3/aleksis/core/templates/core/dashboard_widget/create.html
+-rw-r--r--   0        0        0      635 2023-03-19 19:24:31.250830 aleksis_core-3.0b3/aleksis/core/templates/core/dashboard_widget/dashboardwidget_broken.html
+-rw-r--r--   0        0        0      626 2023-03-19 19:24:31.250830 aleksis_core-3.0b3/aleksis/core/templates/core/dashboard_widget/edit.html
+-rw-r--r--   0        0        0      262 2023-03-19 19:24:31.250830 aleksis_core-3.0b3/aleksis/core/templates/core/dashboard_widget/external_link_widget.html
+-rw-r--r--   0        0        0     1349 2023-03-19 19:24:31.250830 aleksis_core-3.0b3/aleksis/core/templates/core/dashboard_widget/list.html
+-rw-r--r--   0        0        0      226 2023-03-19 19:24:31.250830 aleksis_core-3.0b3/aleksis/core/templates/core/dashboard_widget/static_content_widget.html
+-rw-r--r--   0        0        0     3746 2023-03-19 19:24:31.250830 aleksis_core-3.0b3/aleksis/core/templates/core/data_check/list.html
+-rw-r--r--   0        0        0     2233 2023-03-19 19:24:31.250830 aleksis_core-3.0b3/aleksis/core/templates/core/edit_dashboard.html
+-rw-r--r--   0        0        0        0 2023-03-19 19:24:31.250830 aleksis_core-3.0b3/aleksis/core/templates/core/empty.html
+-rw-r--r--   0        0        0     5310 2023-03-19 19:24:31.250830 aleksis_core-3.0b3/aleksis/core/templates/core/group/child_groups.html
+-rw-r--r--   0        0        0      650 2023-03-19 19:24:31.250830 aleksis_core-3.0b3/aleksis/core/templates/core/group/edit.html
+-rw-r--r--   0        0        0     3382 2023-03-19 19:24:31.250830 aleksis_core-3.0b3/aleksis/core/templates/core/group/full.html
+-rw-r--r--   0        0        0     1019 2023-03-19 19:24:31.250830 aleksis_core-3.0b3/aleksis/core/templates/core/group/list.html
+-rw-r--r--   0        0        0      465 2023-03-19 19:24:31.250830 aleksis_core-3.0b3/aleksis/core/templates/core/group_type/edit.html
+-rw-r--r--   0        0        0      564 2023-03-19 19:24:31.250830 aleksis_core-3.0b3/aleksis/core/templates/core/group_type/list.html
+-rw-r--r--   0        0        0     2504 2023-03-19 19:24:31.250830 aleksis_core-3.0b3/aleksis/core/templates/core/index.html
+-rw-r--r--   0        0        0      777 2023-03-19 19:24:31.250830 aleksis_core-3.0b3/aleksis/core/templates/core/pages/delete.html
+-rw-r--r--   0        0        0     6835 2023-03-19 19:24:31.250830 aleksis_core-3.0b3/aleksis/core/templates/core/pages/system_status.html
+-rw-r--r--   0        0        0      603 2023-03-19 19:24:31.250830 aleksis_core-3.0b3/aleksis/core/templates/core/pages/test_pdf.html
+-rw-r--r--   0        0        0       93 2023-03-19 19:24:31.250830 aleksis_core-3.0b3/aleksis/core/templates/core/partials/address.html
+-rw-r--r--   0        0        0      189 2023-03-19 19:24:31.250830 aleksis_core-3.0b3/aleksis/core/templates/core/partials/admins_list.html
+-rw-r--r--   0        0        0     1632 2023-03-19 19:24:31.250830 aleksis_core-3.0b3/aleksis/core/templates/core/partials/announcements.html
+-rw-r--r--   0        0        0     1472 2023-03-19 19:24:31.250830 aleksis_core-3.0b3/aleksis/core/templates/core/partials/avatar_content.html
+-rw-r--r--   0        0        0      319 2023-03-19 19:24:31.250830 aleksis_core-3.0b3/aleksis/core/templates/core/partials/copy_button.html
+-rw-r--r--   0        0        0     1089 2023-03-19 19:24:31.250830 aleksis_core-3.0b3/aleksis/core/templates/core/partials/crud_events.html
+-rw-r--r--   0        0        0      389 2023-03-19 19:24:31.250830 aleksis_core-3.0b3/aleksis/core/templates/core/partials/edit_dashboard_widget.html
+-rw-r--r--   0        0        0     1624 2023-03-19 19:24:31.250830 aleksis_core-3.0b3/aleksis/core/templates/core/partials/meta.html
+-rw-r--r--   0        0        0      414 2023-03-19 19:24:31.250830 aleksis_core-3.0b3/aleksis/core/templates/core/partials/on_page_menu.html
+-rw-r--r--   0        0        0      260 2023-03-19 19:24:31.250830 aleksis_core-3.0b3/aleksis/core/templates/core/partials/save_button.html
+-rw-r--r--   0        0        0     2374 2023-03-19 19:24:31.250830 aleksis_core-3.0b3/aleksis/core/templates/core/partials/splash_screen.html
+-rw-r--r--   0        0        0      325 2023-03-19 19:24:31.250830 aleksis_core-3.0b3/aleksis/core/templates/core/partials/turnable.html
+-rw-r--r--   0        0        0      915 2023-03-19 19:24:31.250830 aleksis_core-3.0b3/aleksis/core/templates/core/perms/assign.html
+-rw-r--r--   0        0        0     2478 2023-03-19 19:24:31.250830 aleksis_core-3.0b3/aleksis/core/templates/core/perms/list.html
+-rw-r--r--   0        0        0      376 2023-03-19 19:24:31.250830 aleksis_core-3.0b3/aleksis/core/templates/core/person/collection.html
+-rw-r--r--   0        0        0      649 2023-03-19 19:24:31.250830 aleksis_core-3.0b3/aleksis/core/templates/core/person/create.html
+-rw-r--r--   0        0        0      645 2023-03-19 19:24:31.250830 aleksis_core-3.0b3/aleksis/core/templates/core/person/edit.html
+-rw-r--r--   0        0        0     1165 2023-03-19 19:24:31.250830 aleksis_core-3.0b3/aleksis/core/templates/core/person/list.html
+-rw-r--r--   0        0        0      455 2023-03-19 19:24:31.250830 aleksis_core-3.0b3/aleksis/core/templates/core/school_term/create.html
+-rw-r--r--   0        0        0      451 2023-03-19 19:24:31.250830 aleksis_core-3.0b3/aleksis/core/templates/core/school_term/edit.html
+-rw-r--r--   0        0        0      556 2023-03-19 19:24:31.250830 aleksis_core-3.0b3/aleksis/core/templates/core/school_term/list.html
+-rw-r--r--   0        0        0      935 2023-03-19 19:24:31.250830 aleksis_core-3.0b3/aleksis/core/templates/core/vue_index.html
+-rw-r--r--   0        0        0     3921 2023-03-19 19:24:31.250830 aleksis_core-3.0b3/aleksis/core/templates/django_tables2/materialize.html
+-rw-r--r--   0        0        0      981 2023-03-19 19:24:31.250830 aleksis_core-3.0b3/aleksis/core/templates/dynamic_preferences/form.html
+-rw-r--r--   0        0        0      376 2023-03-19 19:24:31.250830 aleksis_core-3.0b3/aleksis/core/templates/dynamic_preferences/sections.html
+-rw-r--r--   0        0        0      764 2023-03-19 19:24:31.250830 aleksis_core-3.0b3/aleksis/core/templates/invitations/disabled.html
+-rw-r--r--   0        0        0     1281 2023-03-19 19:24:31.250830 aleksis_core-3.0b3/aleksis/core/templates/invitations/enter.html
+-rw-r--r--   0        0        0     1060 2023-03-19 19:24:31.250830 aleksis_core-3.0b3/aleksis/core/templates/invitations/forms/_invite.html
+-rw-r--r--   0        0        0      102 2023-03-19 19:24:31.250830 aleksis_core-3.0b3/aleksis/core/templates/invitations/messages/invite_accepted.txt
+-rw-r--r--   0        0        0      171 2023-03-19 19:24:31.250830 aleksis_core-3.0b3/aleksis/core/templates/material/field_errors.html
+-rw-r--r--   0        0        0     1232 2023-03-19 19:24:31.250830 aleksis_core-3.0b3/aleksis/core/templates/material/fields/ckeditor_ckeditorwidget.html
+-rw-r--r--   0        0        0     1897 2023-03-19 19:24:31.250830 aleksis_core-3.0b3/aleksis/core/templates/material/fields/colorfield_colorwidget.html
+-rw-r--r--   0        0        0     1009 2023-03-19 19:24:31.250830 aleksis_core-3.0b3/aleksis/core/templates/material/fields/django_select2_modelselect2multiplewidget.html
+-rw-r--r--   0        0        0     1009 2023-03-19 19:24:31.250830 aleksis_core-3.0b3/aleksis/core/templates/material/fields/django_select2_select2widget.html
+-rw-r--r--   0        0        0      253 2023-03-19 19:24:31.250830 aleksis_core-3.0b3/aleksis/core/templates/material/non_field_errors.html
+-rw-r--r--   0        0        0      663 2023-03-19 19:24:31.250830 aleksis_core-3.0b3/aleksis/core/templates/oauth2_provider/application/create.html
+-rw-r--r--   0        0        0     2335 2023-03-19 19:24:31.250830 aleksis_core-3.0b3/aleksis/core/templates/oauth2_provider/application/detail.html
+-rw-r--r--   0        0        0      669 2023-03-19 19:24:31.250830 aleksis_core-3.0b3/aleksis/core/templates/oauth2_provider/application/edit.html
+-rw-r--r--   0        0        0     1074 2023-03-19 19:24:31.250830 aleksis_core-3.0b3/aleksis/core/templates/oauth2_provider/application/list.html
+-rw-r--r--   0        0        0     2686 2023-03-19 19:24:31.250830 aleksis_core-3.0b3/aleksis/core/templates/oauth2_provider/authorize.html
+-rw-r--r--   0        0        0      877 2023-03-19 19:24:31.250830 aleksis_core-3.0b3/aleksis/core/templates/oauth2_provider/authorized-token-delete.html
+-rw-r--r--   0        0        0     1256 2023-03-19 19:24:31.250830 aleksis_core-3.0b3/aleksis/core/templates/oauth2_provider/authorized-tokens.html
+-rw-r--r--   0        0        0      759 2023-03-19 19:24:31.250830 aleksis_core-3.0b3/aleksis/core/templates/offline.html
+-rw-r--r--   0        0        0       42 2023-03-19 19:24:31.250830 aleksis_core-3.0b3/aleksis/core/templates/search/indexes/core/group_text.txt
+-rw-r--r--   0        0        0       69 2023-03-19 19:24:31.250830 aleksis_core-3.0b3/aleksis/core/templates/search/indexes/core/person_text.txt
+-rw-r--r--   0        0        0       42 2023-03-19 19:24:31.250830 aleksis_core-3.0b3/aleksis/core/templates/search/indexes/core/room_text.txt
+-rw-r--r--   0        0        0     3171 2023-03-19 19:24:31.254830 aleksis_core-3.0b3/aleksis/core/templates/search/search.html
+-rw-r--r--   0        0        0      243 2023-03-19 19:24:31.254830 aleksis_core-3.0b3/aleksis/core/templates/search/searchbar_snippet.html
+-rw-r--r--   0        0        0      150 2023-03-19 19:24:31.254830 aleksis_core-3.0b3/aleksis/core/templates/search/searchbar_snippets.html
+-rw-r--r--   0        0        0      169 2023-03-19 19:24:31.254830 aleksis_core-3.0b3/aleksis/core/templates/sms/notification.txt
+-rw-r--r--   0        0        0      893 2023-03-19 19:24:31.254830 aleksis_core-3.0b3/aleksis/core/templates/socialaccount/authentication_error.html
+-rw-r--r--   0        0        0     1268 2023-03-19 19:24:31.254830 aleksis_core-3.0b3/aleksis/core/templates/socialaccount/connections.html
+-rw-r--r--   0        0        0     1289 2023-03-19 19:24:31.254830 aleksis_core-3.0b3/aleksis/core/templates/socialaccount/login.html
+-rw-r--r--   0        0        0      809 2023-03-19 19:24:31.254830 aleksis_core-3.0b3/aleksis/core/templates/socialaccount/login_cancelled.html
+-rw-r--r--   0        0        0     1012 2023-03-19 19:24:31.254830 aleksis_core-3.0b3/aleksis/core/templates/socialaccount/signup.html
+-rw-r--r--   0        0        0     1434 2023-03-19 19:24:31.254830 aleksis_core-3.0b3/aleksis/core/templates/socialaccount/snippets/provider_list.html
+-rw-r--r--   0        0        0      630 2023-03-19 19:24:31.254830 aleksis_core-3.0b3/aleksis/core/templates/templated_email/base.email
+-rw-r--r--   0        0        0     1527 2023-03-19 19:24:31.254830 aleksis_core-3.0b3/aleksis/core/templates/templated_email/celery_failure.email
+-rw-r--r--   0        0        0      994 2023-03-19 19:24:31.254830 aleksis_core-3.0b3/aleksis/core/templates/templated_email/data_checks.email
+-rw-r--r--   0        0        0      990 2023-03-19 19:24:31.254830 aleksis_core-3.0b3/aleksis/core/templates/templated_email/email.css
+-rw-r--r--   0        0        0     1461 2023-03-19 19:24:31.254830 aleksis_core-3.0b3/aleksis/core/templates/templated_email/notification.email
+-rw-r--r--   0        0        0      668 2023-03-19 19:24:31.254830 aleksis_core-3.0b3/aleksis/core/templates/templated_email/person_changed.email
+-rw-r--r--   0        0        0      219 2023-03-19 19:24:31.254830 aleksis_core-3.0b3/aleksis/core/templates/two_factor/_base_focus.html
+-rw-r--r--   0        0        0      877 2023-03-19 19:24:31.254830 aleksis_core-3.0b3/aleksis/core/templates/two_factor/_wizard_actions.html
+-rw-r--r--   0        0        0      119 2023-03-19 19:24:31.254830 aleksis_core-3.0b3/aleksis/core/templates/two_factor/_wizard_forms.html
+-rw-r--r--   0        0        0     1780 2023-03-19 19:24:31.254830 aleksis_core-3.0b3/aleksis/core/templates/two_factor/core/backup_tokens.html
+-rw-r--r--   0        0        0     6712 2023-03-19 19:24:31.254830 aleksis_core-3.0b3/aleksis/core/templates/two_factor/core/login.html
+-rw-r--r--   0        0        0      943 2023-03-19 19:24:31.254830 aleksis_core-3.0b3/aleksis/core/templates/two_factor/core/otp_required.html
+-rw-r--r--   0        0        0      986 2023-03-19 19:24:31.254830 aleksis_core-3.0b3/aleksis/core/templates/two_factor/core/phone_register.html
+-rw-r--r--   0        0        0     3312 2023-03-19 19:24:31.254830 aleksis_core-3.0b3/aleksis/core/templates/two_factor/core/setup.html
+-rw-r--r--   0        0        0     2127 2023-03-19 19:24:31.254830 aleksis_core-3.0b3/aleksis/core/templates/two_factor/core/setup_complete.html
+-rw-r--r--   0        0        0      786 2023-03-19 19:24:31.254830 aleksis_core-3.0b3/aleksis/core/templates/two_factor/profile/disable.html
+-rw-r--r--   0        0        0        0 2023-03-19 19:24:31.254830 aleksis_core-3.0b3/aleksis/core/templatetags/__init__.py
+-rw-r--r--   0        0        0       99 2023-03-19 19:24:31.254830 aleksis_core-3.0b3/aleksis/core/templatetags/apps.py
+-rw-r--r--   0        0        0      394 2023-03-19 19:24:31.254830 aleksis_core-3.0b3/aleksis/core/templatetags/dashboard.py
+-rw-r--r--   0        0        0     1618 2023-03-19 19:24:31.254830 aleksis_core-3.0b3/aleksis/core/templatetags/data_helpers.py
+-rw-r--r--   0        0        0     1134 2023-03-19 19:24:31.254830 aleksis_core-3.0b3/aleksis/core/templatetags/html_helpers.py
+-rw-r--r--   0        0        0      206 2023-03-19 19:24:31.254830 aleksis_core-3.0b3/aleksis/core/templatetags/msg_box.py
+-rw-r--r--   0        0        0     3696 2023-03-19 19:24:31.254830 aleksis_core-3.0b3/aleksis/core/tests/browser/test_selenium.py
+-rw-r--r--   0        0        0     6596 2023-03-19 19:24:31.254830 aleksis_core-3.0b3/aleksis/core/tests/models/test.pdf
+-rw-r--r--   0        0        0     6562 2023-03-19 19:24:31.254830 aleksis_core-3.0b3/aleksis/core/tests/models/test_group.py
+-rw-r--r--   0        0        0     1520 2023-03-19 19:24:31.254830 aleksis_core-3.0b3/aleksis/core/tests/models/test_group_sync.py
+-rw-r--r--   0        0        0     3049 2023-03-19 19:24:31.254830 aleksis_core-3.0b3/aleksis/core/tests/models/test_notification.py
+-rw-r--r--   0        0        0     4003 2023-03-19 19:24:31.254830 aleksis_core-3.0b3/aleksis/core/tests/models/test_pdffile.py
+-rw-r--r--   0        0        0      427 2023-03-19 19:24:31.254830 aleksis_core-3.0b3/aleksis/core/tests/models/test_person.py
+-rw-r--r--   0        0        0     5503 2023-03-19 19:24:31.254830 aleksis_core-3.0b3/aleksis/core/tests/regression/test_regression.py
+-rw-r--r--   0        0        0      683 2023-03-19 19:24:31.254830 aleksis_core-3.0b3/aleksis/core/tests/regression/view_oauth.py
+-rw-r--r--   0        0        0     1021 2023-03-19 19:24:31.254830 aleksis_core-3.0b3/aleksis/core/tests/templatetags/test_data_helpers.py
+-rw-r--r--   0        0        0     2292 2023-03-19 19:24:31.254830 aleksis_core-3.0b3/aleksis/core/tests/views/test_account.py
+-rw-r--r--   0        0        0    18516 2023-03-19 19:24:31.254830 aleksis_core-3.0b3/aleksis/core/urls.py
+-rw-r--r--   0        0        0        0 2023-03-19 19:24:31.254830 aleksis_core-3.0b3/aleksis/core/util/__init__.py
+-rw-r--r--   0        0        0      176 2023-03-19 19:32:07.238032 aleksis_core-3.0b3/aleksis/core/util/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0    13545 2023-03-19 19:32:08.134030 aleksis_core-3.0b3/aleksis/core/util/__pycache__/apps.cpython-311.pyc
+-rw-r--r--   0        0        0    10101 2023-03-19 19:32:09.154028 aleksis_core-3.0b3/aleksis/core/util/__pycache__/celery_progress.cpython-311.pyc
+-rw-r--r--   0        0        0    24932 2023-03-19 19:32:07.242032 aleksis_core-3.0b3/aleksis/core/util/__pycache__/core_helpers.cpython-311.pyc
+-rw-r--r--   0        0        0     1500 2023-03-19 19:32:07.434031 aleksis_core-3.0b3/aleksis/core/util/__pycache__/email.cpython-311.pyc
+-rw-r--r--   0        0        0      771 2023-03-19 19:32:09.158028 aleksis_core-3.0b3/aleksis/core/util/__pycache__/model_helpers.cpython-311.pyc
+-rw-r--r--   0        0        0     5712 2023-03-19 19:32:09.154028 aleksis_core-3.0b3/aleksis/core/util/__pycache__/notifications.cpython-311.pyc
+-rw-r--r--   0        0        0     9548 2023-03-19 19:32:09.326028 aleksis_core-3.0b3/aleksis/core/util/__pycache__/predicates.cpython-311.pyc
+-rw-r--r--   0        0        0     2181 2023-03-19 19:32:08.142030 aleksis_core-3.0b3/aleksis/core/util/__pycache__/sass_helpers.cpython-311.pyc
+-rw-r--r--   0        0        0      664 2023-03-19 19:32:08.138030 aleksis_core-3.0b3/aleksis/core/util/__pycache__/spdx.cpython-311.pyc
+-rw-r--r--   0        0        0    10028 2023-03-19 19:24:31.254830 aleksis_core-3.0b3/aleksis/core/util/apps.py
+-rw-r--r--   0        0        0     5970 2023-03-19 19:24:31.254830 aleksis_core-3.0b3/aleksis/core/util/auth_helpers.py
+-rw-r--r--   0        0        0     7920 2023-03-19 19:24:31.254830 aleksis_core-3.0b3/aleksis/core/util/celery_progress.py
+-rw-r--r--   0        0        0      197 2023-03-19 19:24:31.254830 aleksis_core-3.0b3/aleksis/core/util/context_processors.py
+-rw-r--r--   0        0        0    16042 2023-03-19 19:24:31.254830 aleksis_core-3.0b3/aleksis/core/util/core_helpers.py
+-rw-r--r--   0        0        0      986 2023-03-19 19:24:31.254830 aleksis_core-3.0b3/aleksis/core/util/email.py
+-rw-r--r--   0        0        0     1175 2023-03-19 19:24:31.254830 aleksis_core-3.0b3/aleksis/core/util/forms.py
+-rw-r--r--   0        0        0     2895 2023-03-19 19:24:31.254830 aleksis_core-3.0b3/aleksis/core/util/frontend_helpers.py
+-rw-r--r--   0        0        0     2375 2023-03-19 19:24:31.254830 aleksis_core-3.0b3/aleksis/core/util/ldap.py
+-rw-r--r--   0        0        0   192829 2023-03-19 19:24:31.254830 aleksis_core-3.0b3/aleksis/core/util/licenses.json
+-rw-r--r--   0        0        0     2255 2023-03-19 19:24:31.254830 aleksis_core-3.0b3/aleksis/core/util/messages.py
+-rw-r--r--   0        0        0     2091 2023-03-19 19:24:31.254830 aleksis_core-3.0b3/aleksis/core/util/middlewares.py
+-rw-r--r--   0        0        0      850 2023-03-19 19:24:31.258830 aleksis_core-3.0b3/aleksis/core/util/model_helpers.py
+-rw-r--r--   0        0        0     3732 2023-03-19 19:24:31.258830 aleksis_core-3.0b3/aleksis/core/util/notifications.py
+-rw-r--r--   0        0        0     6131 2023-03-19 19:24:31.258830 aleksis_core-3.0b3/aleksis/core/util/pdf.py
+-rw-r--r--   0        0        0     5583 2023-03-19 19:24:31.258830 aleksis_core-3.0b3/aleksis/core/util/predicates.py
+-rw-r--r--   0        0        0      936 2023-03-19 19:24:31.258830 aleksis_core-3.0b3/aleksis/core/util/sass_helpers.py
+-rw-r--r--   0        0        0      524 2023-03-19 19:24:31.258830 aleksis_core-3.0b3/aleksis/core/util/search.py
+-rw-r--r--   0        0        0      130 2023-03-19 19:24:31.258830 aleksis_core-3.0b3/aleksis/core/util/spdx.py
+-rw-r--r--   0        0        0     1673 2023-03-19 19:24:31.258830 aleksis_core-3.0b3/aleksis/core/util/tables.py
+-rw-r--r--   0        0        0    54591 2023-03-19 19:24:31.258830 aleksis_core-3.0b3/aleksis/core/views.py
+-rw-r--r--   0        0        0    10201 2023-03-19 19:24:31.258830 aleksis_core-3.0b3/aleksis/core/vite.config.js
+-rw-r--r--   0        0        0      173 2023-03-19 19:24:31.258830 aleksis_core-3.0b3/aleksis/core/wsgi.py
+-rw-r--r--   0        0        0       45 2023-03-19 19:24:31.258830 aleksis_core-3.0b3/conftest.py
+-rw-r--r--   0        0        0      581 2023-03-19 19:24:31.258830 aleksis_core-3.0b3/docs/Makefile
+-rw-r--r--   0        0        0   127432 2023-03-19 19:24:31.258830 aleksis_core-3.0b3/docs/_static/2fa.png
+-rw-r--r--   0        0        0    71362 2023-03-19 19:24:31.258830 aleksis_core-3.0b3/docs/_static/accept_invite.png
+-rw-r--r--   0        0        0    72621 2023-03-19 19:24:31.258830 aleksis_core-3.0b3/docs/_static/create_dashboard_widget.png
+-rw-r--r--   0        0        0    41935 2023-03-19 19:24:31.258830 aleksis_core-3.0b3/docs/_static/create_social_application.png
+-rw-r--r--   0        0        0    72508 2023-03-19 19:24:31.262830 aleksis_core-3.0b3/docs/_static/dashboard.png
+-rw-r--r--   0        0        0    87601 2023-03-19 19:24:31.262830 aleksis_core-3.0b3/docs/_static/dashboard_widgets.png
+-rw-r--r--   0        0        0   119523 2023-03-19 19:24:31.262830 aleksis_core-3.0b3/docs/_static/data_checks.png
+-rw-r--r--   0        0        0    81386 2023-03-19 19:24:31.262830 aleksis_core-3.0b3/docs/_static/edit_dashboard.png
+-rw-r--r--   0        0        0    85722 2023-03-19 19:24:31.262830 aleksis_core-3.0b3/docs/_static/edit_default_dashboard.png
+-rw-r--r--   0        0        0   107979 2023-03-19 19:24:31.266830 aleksis_core-3.0b3/docs/_static/invitations.png
+-rw-r--r--   0        0        0   177681 2023-03-19 19:24:31.266830 aleksis_core-3.0b3/docs/_static/invite_existing.png
+-rw-r--r--   0        0        0    44868 2023-03-19 19:24:31.266830 aleksis_core-3.0b3/docs/_static/pwa_desktop_chromium.png
+-rw-r--r--   0        0        0    69215 2023-03-19 19:24:31.266830 aleksis_core-3.0b3/docs/_static/pwa_mobile_chromium.png
+-rw-r--r--   0        0        0   128479 2023-03-19 19:24:31.266830 aleksis_core-3.0b3/docs/_static/pwa_mobile_firefox.png
+-rw-r--r--   0        0        0   108973 2023-03-19 19:24:31.266830 aleksis_core-3.0b3/docs/_static/pwa_mobile_safari.png
+-rw-r--r--   0        0        0    69804 2023-03-19 19:24:31.270830 aleksis_core-3.0b3/docs/_static/signup.png
+-rw-r--r--   0        0        0      132 2023-03-19 19:24:31.270830 aleksis_core-3.0b3/docs/admin/00_index.rst
+-rw-r--r--   0        0        0     4231 2023-03-19 19:24:31.270830 aleksis_core-3.0b3/docs/admin/01_core_concepts.rst
+-rw-r--r--   0        0        0     8059 2023-03-19 19:24:31.270830 aleksis_core-3.0b3/docs/admin/10_install.rst
+-rw-r--r--   0        0        0     1872 2023-03-19 19:24:31.270830 aleksis_core-3.0b3/docs/admin/15_config_files.rst
+-rw-r--r--   0        0        0     1982 2023-03-19 19:24:31.270830 aleksis_core-3.0b3/docs/admin/16_config_options.rst
+-rw-r--r--   0        0        0     1648 2023-03-19 19:24:31.270830 aleksis_core-3.0b3/docs/admin/17_storage.rst
+-rw-r--r--   0        0        0      803 2023-03-19 19:24:31.270830 aleksis_core-3.0b3/docs/admin/18_mail.rst
+-rw-r--r--   0        0        0     1509 2023-03-19 19:24:31.270830 aleksis_core-3.0b3/docs/admin/21_ldap.rst
+-rw-r--r--   0        0        0     3037 2023-03-19 19:24:31.270830 aleksis_core-3.0b3/docs/admin/22_registration.rst
+-rw-r--r--   0        0        0     1467 2023-03-19 19:24:31.270830 aleksis_core-3.0b3/docs/admin/23_socialaccounts.rst
+-rw-r--r--   0        0        0     3218 2023-03-19 19:24:31.270830 aleksis_core-3.0b3/docs/admin/31_monitoring.rst
+-rw-r--r--   0        0        0     1012 2023-03-19 19:24:31.270830 aleksis_core-3.0b3/docs/admin/32_tasks.rst
+-rw-r--r--   0        0        0     1393 2023-03-19 19:24:31.270830 aleksis_core-3.0b3/docs/admin/33_data_checks.rst
+-rw-r--r--   0        0        0     4610 2023-03-19 19:24:31.270830 aleksis_core-3.0b3/docs/admin/50_dashboard.rst
+-rw-r--r--   0        0        0     6393 2023-03-19 19:24:31.270830 aleksis_core-3.0b3/docs/conf.py
+-rw-r--r--   0        0        0      132 2023-03-19 19:24:31.270830 aleksis_core-3.0b3/docs/dev/00_index.rst
+-rw-r--r--   0        0        0     4002 2023-03-19 19:24:31.270830 aleksis_core-3.0b3/docs/dev/01_setup.rst
+-rw-r--r--   0        0        0     1427 2023-03-19 19:24:31.270830 aleksis_core-3.0b3/docs/dev/02_install_apps.rst
+-rw-r--r--   0        0        0     3117 2023-03-19 19:24:31.270830 aleksis_core-3.0b3/docs/dev/03_run_tests.rst
+-rw-r--r--   0        0        0     4519 2023-03-19 19:24:31.270830 aleksis_core-3.0b3/docs/dev/04_materialize_templates.rst
+-rw-r--r--   0        0        0      289 2023-03-19 19:24:31.270830 aleksis_core-3.0b3/docs/dev/05_extensible_models.rst
+-rw-r--r--   0        0        0     1148 2023-03-19 19:24:31.270830 aleksis_core-3.0b3/docs/dev/06_merging_app_settings.rst
+-rw-r--r--   0        0        0     1349 2023-03-19 19:24:31.270830 aleksis_core-3.0b3/docs/dev/10_dashboard_widgets.rst
+-rw-r--r--   0        0        0      514 2023-03-19 19:24:31.270830 aleksis_core-3.0b3/docs/index.rst
+-rw-r--r--   0        0        0      787 2023-03-19 19:24:31.270830 aleksis_core-3.0b3/docs/make.bat
+-rw-r--r--   0        0        0       95 2023-03-19 19:24:31.270830 aleksis_core-3.0b3/docs/ref/00_index.rst
+-rw-r--r--   0        0        0       69 2023-03-19 19:24:31.270830 aleksis_core-3.0b3/docs/ref/core/01_checks.rst
+-rw-r--r--   0        0        0       70 2023-03-19 19:24:31.270830 aleksis_core-3.0b3/docs/ref/core/02_managers.rst
+-rw-r--r--   0        0        0       64 2023-03-19 19:24:31.270830 aleksis_core-3.0b3/docs/ref/core/03_mixins.rst
+-rw-r--r--   0        0        0       84 2023-03-19 19:24:31.270830 aleksis_core-3.0b3/docs/ref/core/04_models.rst
+-rw-r--r--   0        0        0      108 2023-03-19 19:24:31.270830 aleksis_core-3.0b3/docs/ref/core/05_registries.rst
+-rw-r--r--   0        0        0       93 2023-03-19 19:24:31.270830 aleksis_core-3.0b3/docs/ref/core/06_search_indexes.rst
+-rw-r--r--   0        0        0       79 2023-03-19 19:24:31.270830 aleksis_core-3.0b3/docs/ref/core/07_tables.rst
+-rw-r--r--   0        0        0       90 2023-03-19 19:24:31.270830 aleksis_core-3.0b3/docs/ref/core/08_tasks.rst
+-rw-r--r--   0        0        0     1017 2023-03-19 19:24:31.270830 aleksis_core-3.0b3/docs/ref/core/09_utils.rst
+-rw-r--r--   0        0        0       71 2023-03-19 19:24:31.270830 aleksis_core-3.0b3/docs/ref/core/10_views.rst
+-rw-r--r--   0        0        0       77 2023-03-19 19:24:31.270830 aleksis_core-3.0b3/docs/ref/core/11_filters.rst
+-rw-r--r--   0        0        0      373 2023-03-19 19:24:31.270830 aleksis_core-3.0b3/docs/ref/core/12_template_tags.rst
+-rw-r--r--   0        0        0      112 2023-03-19 19:24:31.270830 aleksis_core-3.0b3/docs/user/00_index.rst
+-rw-r--r--   0        0        0     1152 2023-03-19 19:24:31.270830 aleksis_core-3.0b3/docs/user/01_registration.rst
+-rw-r--r--   0        0        0     3465 2023-03-19 19:24:31.270830 aleksis_core-3.0b3/docs/user/02_personal_account.rst
+-rw-r--r--   0        0        0     1770 2023-03-19 19:24:31.270830 aleksis_core-3.0b3/docs/user/10_dashboard.rst
+-rw-r--r--   0        0        0     2607 2023-03-19 19:24:31.270830 aleksis_core-3.0b3/docs/user/20_pwa.rst
+-rw-r--r--   0        0        0     4574 2023-03-19 19:29:01.086357 aleksis_core-3.0b3/pyproject.toml
+-rw-r--r--   0        0        0     2599 2023-03-19 19:24:31.270830 aleksis_core-3.0b3/tox.ini
+-rw-r--r--   0        0        0    10359 1970-01-01 00:00:00.000000 aleksis_core-3.0b3/setup.py
+-rw-r--r--   0        0        0     8557 1970-01-01 00:00:00.000000 aleksis_core-3.0b3/PKG-INFO
```

### Comparing `aleksis_core-3.0b2/CHANGELOG.rst` & `aleksis_core-3.0b3/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,24 @@
 =========
 
 All notable changes to this project will be documented in this file.
 
 The format is based on `Keep a Changelog`_,
 and this project adheres to `Semantic Versioning`_.
 
-`3.0b2` - 2023-03-09
---------------------
+`3.0b3`_ - 2023-03-19
+---------------------
+
+Fixed
+~~~~~
+
+* Some GraphQL queries could return more data than permitted in related fields.
+
+`3.0b2`_ - 2023-03-09
+---------------------
 
 Changed
 ~~~~~~~
 
 * Change default network policy of the Apollo client to `cache-and-network`.
 
 Fixed
@@ -20,24 +28,24 @@
 * In case the status code of a response was not in the range between 200 and 299
   but still indicates that the response should be delivered, e. g. in the case
   of a redirected request, the service worker served the offline fallback page.
 * In some cases, the resize listener for the IFrame in the `LegacyBaseTemplate`
   did not trigger.
 * [Dev] Allow apps to declare URLs in the non-legacy namespace again
 
-`3.0b1` - 2023-02-27
---------------------
+`3.0b1`_ - 2023-02-27
+---------------------
 
 Added
 ~~~~~
 
 * Support for two factor authentication via email codes and Webauthn.
 
-`3.0b0` - 2023-02-15
---------------------
+`3.0b0`_ - 2023-02-15
+---------------------
 
 This release starts a new era of the AlekSIS® framework, by introducing a
 dynamic frontend app written in Vue.js which communicates with the backend
 through GraphQL.  Support for legacy views (Django templates and
 Materialize) was removed; while there is backwards compatibility for now,
 this is only used by official apps until their views are fully migrated.
 
@@ -104,16 +112,16 @@
 ~~~~~~~
 
 * iCal feed URLs for birthdays (will be reintroduced later)
 * [Dev] Django debug toolbar
   * It caused major performance issues and is not useful with the new
     frontend anymore
 
-`2.12.3` - 2023-03-07
----------------------
+`2.12.3`_ - 2023-03-07
+----------------------
 
 Fixed
 ~~~~~
 
 * The permission check for the dashboard edit page failed when the user had no person assigned.
 * OIDC scope "phone" had no claims.
 * AlekSIS groups were not synced to Django groups on registration of existing persons
@@ -1082,7 +1090,8 @@
 .. _2.12: https://edugit.org/AlekSIS/Official/AlekSIS/-/tags/2.12
 .. _2.12.1: https://edugit.org/AlekSIS/Official/AlekSIS/-/tags/2.12.1
 .. _2.12.2: https://edugit.org/AlekSIS/Official/AlekSIS/-/tags/2.12.2
 .. _2.12.3: https://edugit.org/AlekSIS/Official/AlekSIS/-/tags/2.12.3
 .. _3.0b0: https://edugit.org/AlekSIS/Official/AlekSIS/-/tags/3.0b0
 .. _3.0b1: https://edugit.org/AlekSIS/Official/AlekSIS/-/tags/3.0b1
 .. _3.0b2: https://edugit.org/AlekSIS/Official/AlekSIS/-/tags/3.0b2
+.. _3.0b3: https://edugit.org/AlekSIS/Official/AlekSIS/-/tags/3.0b3
```

### Comparing `aleksis_core-3.0b2/LICENCE.rst` & `aleksis_core-3.0b3/LICENCE.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/README.rst` & `aleksis_core-3.0b3/README.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/__pycache__/__main__.cpython-311.pyc` & `aleksis_core-3.0b3/aleksis/core/__pycache__/__main__.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x794f0a64 (Thu Mar  9 21:28:25 2023 UTC)
+moddate:  0x6f611764 (Sun Mar 19 19:24:31 2023 UTC)
 files sz: 464
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
```

### Comparing `aleksis_core-3.0b2/aleksis/core/__pycache__/admin.cpython-311.pyc` & `aleksis_core-3.0b3/aleksis/core/__pycache__/admin.cpython-311.pyc`

 * *Files 5% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x794f0a64 (Thu Mar  9 21:28:25 2023 UTC)
+moddate:  0x6f611764 (Sun Mar 19 19:24:31 2023 UTC)
 files sz: 950
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 6
    flags     : 0
    code
```

### Comparing `aleksis_core-3.0b2/aleksis/core/__pycache__/apps.cpython-311.pyc` & `aleksis_core-3.0b3/aleksis/core/__pycache__/apps.cpython-311.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x794f0a64 (Thu Mar  9 21:28:25 2023 UTC)
+moddate:  0x6f611764 (Sun Mar 19 19:24:31 2023 UTC)
 files sz: 8274
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### Comparing `aleksis_core-3.0b2/aleksis/core/__pycache__/celery.cpython-311.pyc` & `aleksis_core-3.0b3/aleksis/core/__pycache__/celery.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x794f0a64 (Thu Mar  9 21:28:25 2023 UTC)
+moddate:  0x6f611764 (Sun Mar 19 19:24:31 2023 UTC)
 files sz: 1338
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
```

### Comparing `aleksis_core-3.0b2/aleksis/core/__pycache__/checks.cpython-311.pyc` & `aleksis_core-3.0b3/aleksis/core/__pycache__/checks.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x794f0a64 (Thu Mar  9 21:28:25 2023 UTC)
+moddate:  0x6f611764 (Sun Mar 19 19:24:31 2023 UTC)
 files sz: 2751
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 6
    flags     : 0
    code
```

### Comparing `aleksis_core-3.0b2/aleksis/core/__pycache__/data_checks.cpython-311.pyc` & `aleksis_core-3.0b3/aleksis/core/__pycache__/data_checks.cpython-311.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x794f0a64 (Thu Mar  9 21:28:25 2023 UTC)
+moddate:  0x6f611764 (Sun Mar 19 19:24:31 2023 UTC)
 files sz: 11534
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 8
    flags     : 0
    code
```

### Comparing `aleksis_core-3.0b2/aleksis/core/__pycache__/health_checks.cpython-311.pyc` & `aleksis_core-3.0b3/aleksis/core/__pycache__/health_checks.cpython-311.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x794f0a64 (Thu Mar  9 21:28:25 2023 UTC)
+moddate:  0x6f611764 (Sun Mar 19 19:24:31 2023 UTC)
 files sz: 2642
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### Comparing `aleksis_core-3.0b2/aleksis/core/__pycache__/managers.cpython-311.pyc` & `aleksis_core-3.0b3/aleksis/core/__pycache__/managers.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x794f0a64 (Thu Mar  9 21:28:25 2023 UTC)
+moddate:  0x6f611764 (Sun Mar 19 19:24:31 2023 UTC)
 files sz: 4690
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 6
    flags     : 0
    code
```

### Comparing `aleksis_core-3.0b2/aleksis/core/__pycache__/mixins.cpython-311.pyc` & `aleksis_core-3.0b3/aleksis/core/__pycache__/mixins.cpython-311.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x794f0a64 (Thu Mar  9 21:28:25 2023 UTC)
+moddate:  0x6f611764 (Sun Mar 19 19:24:31 2023 UTC)
 files sz: 19163
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 7
    flags     : 0
    code
```

### Comparing `aleksis_core-3.0b2/aleksis/core/__pycache__/models.cpython-311.pyc` & `aleksis_core-3.0b3/aleksis/core/__pycache__/models.cpython-311.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x794f0a64 (Thu Mar  9 21:28:25 2023 UTC)
+moddate:  0x6f611764 (Sun Mar 19 19:24:31 2023 UTC)
 files sz: 50787
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 16
    flags     : 0
    code
```

### Comparing `aleksis_core-3.0b2/aleksis/core/__pycache__/preferences.cpython-311.pyc` & `aleksis_core-3.0b3/aleksis/core/__pycache__/preferences.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x794f0a64 (Thu Mar  9 21:28:25 2023 UTC)
+moddate:  0x6f611764 (Sun Mar 19 19:24:31 2023 UTC)
 files sz: 13810
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 7
    flags     : 0
    code
```

### Comparing `aleksis_core-3.0b2/aleksis/core/__pycache__/registries.cpython-311.pyc` & `aleksis_core-3.0b3/aleksis/core/__pycache__/registries.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x794f0a64 (Thu Mar  9 21:28:25 2023 UTC)
+moddate:  0x6f611764 (Sun Mar 19 19:24:31 2023 UTC)
 files sz: 692
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### Comparing `aleksis_core-3.0b2/aleksis/core/__pycache__/rules.cpython-311.pyc` & `aleksis_core-3.0b3/aleksis/core/__pycache__/rules.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,14 +1,14 @@
 magic:    0xa70d0d0a
-moddate:  0x794f0a64 (Thu Mar  9 21:28:25 2023 UTC)
-files sz: 15800
+moddate:  0x6f611764 (Sun Mar 19 19:24:31 2023 UTC)
+files sz: 16018
 code
    argcount  : 0
    nlocals   : 0
-   stacksize : 7
+   stacksize : 6
    flags     : 0
    code
       0x9700640064016c005a00640064026c006d015a010100640364046c026d
       035a036d045a046d055a056d065a066d075a070100640364056c086d095a
       096d0a5a0a6d0b5a0b6d0c5a0c6d0d5a0d6d0e5a0e6d0f5a0f6d105a106d
       115a116d125a120100020065006a130000000000000000640665006a1400
       00000000000000a6020000ab0200000000000000000100650d5a15020065
@@ -23,36 +23,36 @@
       0000000000650c7a0700005a1b020065006a130000000000000000640f65
       1ba6020000ab0200000000000000000100020065006a1300000000000000
       006410650ca6020000ab0200000000000000000100650c0200650a6411a6
       010000ab0100000000000000007a0100005a1c020065006a130000000000
       0000006412651ca6020000ab0200000000000000000100650c0200650a64
       13a6010000ab0100000000000000000200650964136507a6020000ab0200
       000000000000007a0700007a0100005a1d020065006a1300000000000000
-      006414651da6020000ab0200000000000000000100650c0200650a6413a6
-      010000ab0100000000000000000200650b6413a6010000ab010000000000
-      0000007a070000650e7a0700007a0100005a1e020065006a130000000000
-      0000006415651ea6020000ab0200000000000000000100650c0200650a64
-      16a6010000ab0100000000000000000200650b6416a6010000ab01000000
-      00000000007a070000650e7a0700007a0100005a1f020065006a13000000
-      00000000006417651fa6020000ab0200000000000000000100650c020065
-      0a6418a6010000ab0100000000000000000200650b6418a6010000ab0100
-      000000000000007a070000650e7a0700007a0100005a20020065006a1300
-      0000000000000064196520a6020000ab0200000000000000000100650c02
-      00650a641aa6010000ab0100000000000000000200650b641aa6010000ab
-      0100000000000000007a070000650e7a0700007a0100005a21020065006a
+      006414651da6020000ab0200000000000000000100650c650e0200650a64
+      13a6010000ab0100000000000000007a0700000200650b6413a6010000ab
+      0100000000000000007a0700007a0100005a1e020065006a130000000000
+      0000006415651ea6020000ab0200000000000000000100650c650e020065
+      0a6416a6010000ab0100000000000000007a0700000200650b6416a60100
+      00ab0100000000000000007a0700007a0100005a1f020065006a13000000
+      00000000006417651fa6020000ab0200000000000000000100650c650e02
+      00650a6418a6010000ab0100000000000000007a0700000200650b6418a6
+      010000ab0100000000000000007a0700007a0100005a20020065006a1300
+      0000000000000064196520a6020000ab0200000000000000000100650c65
+      0e0200650a641aa6010000ab0100000000000000007a0700000200650b64
+      1aa6010000ab0100000000000000007a0700007a0100005a21020065006a
       130000000000000000641b6521a6020000ab020000000000000000010065
-      0c0200650a641ca6010000ab0100000000000000000200650b641ca60100
-      00ab0100000000000000007a070000650e7a0700007a0100005a22020065
+      0c650e0200650a641ca6010000ab0100000000000000007a070000020065
+      0b641ca6010000ab0100000000000000007a0700007a0100005a22020065
       006a130000000000000000641d6522a6020000ab02000000000000000001
-      00650c0200650a641ea6010000ab0100000000000000000200650b641ea6
-      010000ab0100000000000000007a070000650e7a0700007a0100005a2302
+      00650c650e0200650a641ea6010000ab0100000000000000007a07000002
+      00650b641ea6010000ab0100000000000000007a0700007a0100005a2302
       0065006a130000000000000000641f6523a6020000ab0200000000000000
-      000100650c0200650a6420a6010000ab0100000000000000000200650b64
-      20a6010000ab0100000000000000007a070000650e0200651264216422a6
-      020000ab0200000000000000007a0100007a0700007a0100005a24020065
+      000100650c650e0200651264206421a6020000ab0200000000000000007a
+      0100000200650a6422a6010000ab0100000000000000007a070000020065
+      0b6422a6010000ab0100000000000000007a0700007a0100005a24020065
       006a13000000000000000064236524a6020000ab02000000000000000001
       00650c0200650a6424a6010000ab0100000000000000000200650b6424a6
       010000ab0100000000000000007a0700007a0100005a25020065006a1300
       0000000000000064256525a6020000ab0200000000000000000100650c02
       00650a6426a6010000ab0100000000000000000200650964266505a60200
       00ab0200000000000000007a0700007a0100005a23020065006a13000000
       000000000064276523a6020000ab0200000000000000000100650c020065
@@ -83,22 +83,22 @@
       0000007a0700007a0100005a2f020065006a130000000000000000643a65
       2fa6020000ab0200000000000000000100650c0200650a643ba6010000ab
       0100000000000000007a0100005a30020065006a13000000000000000064
       3c6530a6020000ab0200000000000000000100650c0200650a643da60100
       00ab0100000000000000007a0100005a31020065006a1300000000000000
       00643e6531a6020000ab0200000000000000000100020065006a13000000
       0000000000643f650c651d65237a07000065297a0700007a010000a60200
-      00ab0200000000000000000100650c0200650a6440a6010000ab01000000
-      00000000000200650b6440a6010000ab0100000000000000007a07000065
-      0e7a0700007a0100005a32020065006a13000000000000000064416532a6
+      00ab0200000000000000000100650c650e0200650a6440a6010000ab0100
+      000000000000007a0700000200650b6440a6010000ab0100000000000000
+      007a0700007a0100005a32020065006a13000000000000000064416532a6
       020000ab0200000000000000000100650c0200650a6442a6010000ab0100
       000000000000000200650b6442a6010000ab0100000000000000007a0700
       007a0100005a33020065006a13000000000000000064436533a6020000ab
-      0200000000000000000100650c0200650a6444a6010000ab010000000000
-      0000000200650b6444a6010000ab0100000000000000007a070000650e7a
+      0200000000000000000100650c650e0200650a6444a6010000ab01000000
+      00000000007a0700000200650b6444a6010000ab0100000000000000007a
       0700007a0100005a34020065006a13000000000000000064456534a60200
       00ab0200000000000000000100650c5a35020065006a1300000000000000
       0064466535a6020000ab0200000000000000000100650c0200650a6447a6
       010000ab0100000000000000000200650b6447a6010000ab010000000000
       0000007a070000650f7a0700007a0100005a36020065006a130000000000
       00000064486536a6020000ab0200000000000000000100650c0200650a64
       49a6010000ab0100000000000000000200650b6449a6010000ab01000000
@@ -117,85 +117,88 @@
       3b020065006a1300000000000000006452653ba6020000ab020000000000
       0000000100650c0200650a6453a6010000ab010000000000000000020065
       0b6453a6010000ab0100000000000000007a0700007a0100005a3c020065
       006a1300000000000000006454653ca6020000ab02000000000000000001
       00650c0200650a6455a6010000ab0100000000000000000200650b6455a6
       010000ab0100000000000000007a0700007a0100005a3d020065006a1300
       000000000000006456653da6020000ab0200000000000000000100650c02
-      00650a6457a6010000ab0100000000000000000200650964576506a60200
-      00ab0200000000000000007a0700007a0100005a3e020065006a13000000
-      00000000006458653ea6020000ab0200000000000000000100650c020065
-      0a6459a6010000ab0100000000000000000200650b6459a6010000ab0100
+      00650a6457a6010000ab0100000000000000000200650b6457a6010000ab
+      0100000000000000007a0700007a0100005a3e020065006a130000000000
+      0000006458653ea6020000ab0200000000000000000100650c0200650a64
+      51a6010000ab0100000000000000000200650964516506a6020000ab0200
       000000000000007a0700007a0100005a3f020065006a1300000000000000
-      00645a653fa6020000ab0200000000000000000100650c0200650a645ba6
-      010000ab0100000000000000000200650b645ba6010000ab010000000000
-      0000007a0700007a0100005a40020065006a130000000000000000645c65
-      40a6020000ab0200000000000000000100650c0200650a645da6010000ab
-      0100000000000000007a0100005a41020065006a13000000000000000064
-      5e6541a6020000ab0200000000000000000100650c0200650a645fa60100
-      00ab0100000000000000007a0100005a42020065006a1300000000000000
-      0064606542a6020000ab0200000000000000000100650c0200650a6461a6
-      010000ab0100000000000000007a0100005a43020065006a130000000000
-      00000064626543a6020000ab0200000000000000000100650c0200650a64
-      63a6010000ab0100000000000000000200650b6463a6010000ab01000000
-      00000000007a0700007a0100005a44020065006a13000000000000000064
-      646544a6020000ab0200000000000000000100650c0200650a6465a60100
-      00ab0100000000000000007a0100005a45020065006a1300000000000000
-      0064666545a6020000ab0200000000000000000100650c65457a01000002
-      00650a6467a6010000ab0100000000000000007a0100005a46020065006a
-      13000000000000000064686546a6020000ab020000000000000000010065
-      0c65457a0100000200650a6469a6010000ab0100000000000000007a0100
-      005a47020065006a130000000000000000646a6547a6020000ab02000000
-      00000000000100650c0200650a646ba6010000ab0100000000000000007a
-      0100005a48020065006a130000000000000000646c6548a6020000ab0200
-      000000000000000100650c0200650a646da6010000ab0100000000000000
-      007a0100005a49020065006a130000000000000000646e6549a6020000ab
-      0200000000000000000100650c0200650a646fa6010000ab010000000000
-      0000007a0100005a4a020065006a1300000000000000006470654aa60200
-      00ab0200000000000000000100650c0200650a6471a6010000ab01000000
-      00000000007a0100005a4b020065006a1300000000000000006472654ba6
-      020000ab020000000000000000010002006512640d6473a6020000ab0200
-      00000000000000650c7a0100005a4c020065006a13000000000000000064
-      74654ca6020000ab0200000000000000000100650c0200650a6475a60100
-      00ab0100000000000000007a0100005a4d020065006a1300000000000000
-      006476654da6020000ab02000000000000000001000200651264776478ac
-      79a6020000ab0200000000000000005a4e020065006a1300000000000000
-      00647a654ea6020000ab0200000000000000000100020065126477647bac
-      79a6020000ab0200000000000000005a4f020065006a1300000000000000
-      00647c654fa6020000ab0200000000000000000100020065126477647dac
-      79a6020000ab0200000000000000005a50020065006a1300000000000000
-      00647e6550a6020000ab0200000000000000000100020065126477647fac
-      79a6020000ab0200000000000000005a51020065006a1300000000000000
-      0064806551a6020000ab0200000000000000000100650c65517a0100005a
-      52020065006a13000000000000000064816552a6020000ab020000000000
-      0000000100650c65517a0100000200650a6482a6010000ab010000000000
-      0000007a0100005a53020065006a13000000000000000064836553a60200
-      00ab0200000000000000000100650c0200650a6484a6010000ab01000000
-      00000000007a0100005a54020065006a13000000000000000064856554a6
-      020000ab0200000000000000000100650c0200650a6486a6010000ab0100
-      000000000000007a0100005a55020065006a130000000000000000648765
-      55a6020000ab0200000000000000000100650c0200650a6486a6010000ab
-      0100000000000000007a0100005a56020065006a13000000000000000064
-      886556a6020000ab0200000000000000000100650c0200650a6489a60100
-      00ab0100000000000000007a0100005a57020065006a1300000000000000
-      00648a6557a6020000ab0200000000000000000100650c0200650a648ba6
-      010000ab0100000000000000007a0100005a58020065006a130000000000
-      000000648c6558a6020000ab0200000000000000000100650c65017a0100
-      005a59020065006a130000000000000000648d6559a6020000ab02000000
-      00000000000100650c652b65417a07000065307a07000065317a07000065
-      2d7a07000065457a07000065557a07000065487a07000065597a0700007a
-      0100005a5a020065006a130000000000000000648e655aa6020000ab0200
-      000000000000000100650c0200650a648fa6010000ab0100000000000000
-      007a0100005a5b020065006a1300000000000000006490655ba6020000ab
-      0200000000000000000100650c65017a0100005a5c020065006a13000000
-      00000000006491655ca6020000ab0200000000000000000100650c020065
-      0a6492a6010000ab0100000000000000007a0100005a5d020065006a1300
-      000000000000006493655da6020000ab0200000000000000000100650c65
-      117a0100005a5e020065006a1300000000000000006494655ea6020000ab
-      020000000000000000010064015300
+      006459653fa6020000ab0200000000000000000100650c0200650a645aa6
+      010000ab0100000000000000000200650b645aa6010000ab010000000000
+      0000007a0700007a0100005a40020065006a130000000000000000645b65
+      40a6020000ab0200000000000000000100650c0200650a645ca6010000ab
+      0100000000000000000200650b645ca6010000ab0100000000000000007a
+      0700007a0100005a41020065006a130000000000000000645d6541a60200
+      00ab0200000000000000000100650c0200650a645ea6010000ab01000000
+      00000000007a0100005a42020065006a130000000000000000645f6542a6
+      020000ab0200000000000000000100650c0200650a6460a6010000ab0100
+      000000000000007a0100005a43020065006a130000000000000000646165
+      43a6020000ab0200000000000000000100650c0200650a6462a6010000ab
+      0100000000000000007a0100005a44020065006a13000000000000000064
+      636544a6020000ab0200000000000000000100650c0200650a6464a60100
+      00ab0100000000000000000200650b6464a6010000ab0100000000000000
+      007a0700007a0100005a45020065006a13000000000000000064656545a6
+      020000ab0200000000000000000100650c0200650a6466a6010000ab0100
+      000000000000007a0100005a46020065006a130000000000000000646765
+      46a6020000ab0200000000000000000100650c65467a0100000200650a64
+      68a6010000ab0100000000000000007a0100005a47020065006a13000000
+      000000000064696547a6020000ab0200000000000000000100650c65467a
+      0100000200650a646aa6010000ab0100000000000000007a0100005a4802
+      0065006a130000000000000000646b6548a6020000ab0200000000000000
+      000100650c0200650a646ca6010000ab0100000000000000007a0100005a
+      49020065006a130000000000000000646d6549a6020000ab020000000000
+      0000000100650c0200650a646ea6010000ab0100000000000000007a0100
+      005a4a020065006a130000000000000000646f654aa6020000ab02000000
+      00000000000100650c0200650a6470a6010000ab0100000000000000007a
+      0100005a4b020065006a1300000000000000006471654ba6020000ab0200
+      000000000000000100650c0200650a6472a6010000ab0100000000000000
+      007a0100005a4c020065006a1300000000000000006473654ca6020000ab
+      020000000000000000010002006512640d6474a6020000ab020000000000
+      000000650c7a0100005a4d020065006a1300000000000000006475654da6
+      020000ab0200000000000000000100650c0200650a6476a6010000ab0100
+      000000000000007a0100005a4e020065006a130000000000000000647765
+      4ea6020000ab02000000000000000001000200651264786479ac7aa60200
+      00ab0200000000000000005a4f020065006a130000000000000000647b65
+      4fa6020000ab0200000000000000000100020065126478647cac7aa60200
+      00ab0200000000000000005a50020065006a130000000000000000647d65
+      50a6020000ab0200000000000000000100020065126478647eac7aa60200
+      00ab0200000000000000005a51020065006a130000000000000000647f65
+      51a6020000ab02000000000000000001000200651264786480ac7aa60200
+      00ab0200000000000000005a52020065006a130000000000000000648165
+      52a6020000ab0200000000000000000100650c65527a0100005a53020065
+      006a13000000000000000064826553a6020000ab02000000000000000001
+      00650c65527a0100000200650a6483a6010000ab0100000000000000007a
+      0100005a54020065006a13000000000000000064846554a6020000ab0200
+      000000000000000100650c0200650a6485a6010000ab0100000000000000
+      007a0100005a55020065006a13000000000000000064866555a6020000ab
+      0200000000000000000100650c0200650a6487a6010000ab010000000000
+      0000007a0100005a56020065006a13000000000000000064886556a60200
+      00ab0200000000000000000100650c0200650a6487a6010000ab01000000
+      00000000007a0100005a57020065006a13000000000000000064896557a6
+      020000ab0200000000000000000100650c0200650a648aa6010000ab0100
+      000000000000007a0100005a58020065006a130000000000000000648b65
+      58a6020000ab0200000000000000000100650c0200650a648ca6010000ab
+      0100000000000000007a0100005a59020065006a13000000000000000064
+      8d6559a6020000ab0200000000000000000100650c65017a0100005a5a02
+      0065006a130000000000000000648e655aa6020000ab0200000000000000
+      000100650c652b65427a07000065307a07000065317a070000652d7a0700
+      0065467a07000065567a07000065497a070000655a7a0700007a0100005a
+      5b020065006a130000000000000000648f655ba6020000ab020000000000
+      0000000100650c0200650a6490a6010000ab0100000000000000007a0100
+      005a5c020065006a1300000000000000006491655ca6020000ab02000000
+      00000000000100650c65017a0100005a5d020065006a1300000000000000
+      006492655da6020000ab0200000000000000000100650c0200650a6493a6
+      010000ab0100000000000000007a0100005a5e020065006a130000000000
+      0000006494655ea6020000ab0200000000000000000100650c65117a0100
+      005a5f020065006a1300000000000000006495655fa6020000ab02000000
+      0000000000010064015300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (None)
                  6 IMPORT_NAME              0 (rules)
                  8 STORE_NAME               0 (rules)
    
@@ -400,26 +403,26 @@
                602 LOAD_NAME               29 (view_persons_predicate)
                604 PRECALL                  2
                608 CALL                     2
                618 POP_TOP
    
     62         620 LOAD_NAME               12 (has_person)
    
-    63         622 PUSH_NULL
-               624 LOAD_NAME               10 (has_global_perm)
-               626 LOAD_CONST              19 ('core.view_person')
-               628 PRECALL                  1
-               632 CALL                     1
-               642 PUSH_NULL
-               644 LOAD_NAME               11 (has_object_perm)
-               646 LOAD_CONST              19 ('core.view_person')
-               648 PRECALL                  1
-               652 CALL                     1
-               662 BINARY_OP                7 (|)
-               666 LOAD_NAME               14 (is_current_person)
+    63         622 LOAD_NAME               14 (is_current_person)
+               624 PUSH_NULL
+               626 LOAD_NAME               10 (has_global_perm)
+               628 LOAD_CONST              19 ('core.view_person')
+               630 PRECALL                  1
+               634 CALL                     1
+               644 BINARY_OP                7 (|)
+               648 PUSH_NULL
+               650 LOAD_NAME               11 (has_object_perm)
+               652 LOAD_CONST              19 ('core.view_person')
+               654 PRECALL                  1
+               658 CALL                     1
                668 BINARY_OP                7 (|)
    
     62         672 BINARY_OP                1 (&)
                676 STORE_NAME              30 (view_person_predicate)
    
     65         678 PUSH_NULL
                680 LOAD_NAME                0 (rules)
@@ -428,26 +431,26 @@
                694 LOAD_NAME               30 (view_person_predicate)
                696 PRECALL                  2
                700 CALL                     2
                710 POP_TOP
    
     68         712 LOAD_NAME               12 (has_person)
    
-    69         714 PUSH_NULL
-               716 LOAD_NAME               10 (has_global_perm)
-               718 LOAD_CONST              22 ('core.view_address')
-               720 PRECALL                  1
-               724 CALL                     1
-               734 PUSH_NULL
-               736 LOAD_NAME               11 (has_object_perm)
-               738 LOAD_CONST              22 ('core.view_address')
-               740 PRECALL                  1
-               744 CALL                     1
-               754 BINARY_OP                7 (|)
-               758 LOAD_NAME               14 (is_current_person)
+    69         714 LOAD_NAME               14 (is_current_person)
+               716 PUSH_NULL
+               718 LOAD_NAME               10 (has_global_perm)
+               720 LOAD_CONST              22 ('core.view_address')
+               722 PRECALL                  1
+               726 CALL                     1
+               736 BINARY_OP                7 (|)
+               740 PUSH_NULL
+               742 LOAD_NAME               11 (has_object_perm)
+               744 LOAD_CONST              22 ('core.view_address')
+               746 PRECALL                  1
+               750 CALL                     1
                760 BINARY_OP                7 (|)
    
     68         764 BINARY_OP                1 (&)
                768 STORE_NAME              31 (view_address_predicate)
    
     71         770 PUSH_NULL
                772 LOAD_NAME                0 (rules)
@@ -456,29 +459,29 @@
                786 LOAD_NAME               31 (view_address_predicate)
                788 PRECALL                  2
                792 CALL                     2
                802 POP_TOP
    
     74         804 LOAD_NAME               12 (has_person)
    
-    75         806 PUSH_NULL
-               808 LOAD_NAME               10 (has_global_perm)
-               810 LOAD_CONST              24 ('core.view_contact_details')
-               812 PRECALL                  1
-               816 CALL                     1
-   
-    76         826 PUSH_NULL
-               828 LOAD_NAME               11 (has_object_perm)
-               830 LOAD_CONST              24 ('core.view_contact_details')
-               832 PRECALL                  1
-               836 CALL                     1
+    75         806 LOAD_NAME               14 (is_current_person)
    
-    75         846 BINARY_OP                7 (|)
-   
-    77         850 LOAD_NAME               14 (is_current_person)
+    76         808 PUSH_NULL
+               810 LOAD_NAME               10 (has_global_perm)
+               812 LOAD_CONST              24 ('core.view_contact_details')
+               814 PRECALL                  1
+               818 CALL                     1
+   
+    75         828 BINARY_OP                7 (|)
+   
+    77         832 PUSH_NULL
+               834 LOAD_NAME               11 (has_object_perm)
+               836 LOAD_CONST              24 ('core.view_contact_details')
+               838 PRECALL                  1
+               842 CALL                     1
    
     75         852 BINARY_OP                7 (|)
    
     74         856 BINARY_OP                1 (&)
                860 STORE_NAME              32 (view_contact_details_predicate)
    
     79         862 PUSH_NULL
@@ -488,26 +491,26 @@
                878 LOAD_NAME               32 (view_contact_details_predicate)
                880 PRECALL                  2
                884 CALL                     2
                894 POP_TOP
    
     82         896 LOAD_NAME               12 (has_person)
    
-    83         898 PUSH_NULL
-               900 LOAD_NAME               10 (has_global_perm)
-               902 LOAD_CONST              26 ('core.view_photo')
-               904 PRECALL                  1
-               908 CALL                     1
-               918 PUSH_NULL
-               920 LOAD_NAME               11 (has_object_perm)
-               922 LOAD_CONST              26 ('core.view_photo')
-               924 PRECALL                  1
-               928 CALL                     1
-               938 BINARY_OP                7 (|)
-               942 LOAD_NAME               14 (is_current_person)
+    83         898 LOAD_NAME               14 (is_current_person)
+               900 PUSH_NULL
+               902 LOAD_NAME               10 (has_global_perm)
+               904 LOAD_CONST              26 ('core.view_photo')
+               906 PRECALL                  1
+               910 CALL                     1
+               920 BINARY_OP                7 (|)
+               924 PUSH_NULL
+               926 LOAD_NAME               11 (has_object_perm)
+               928 LOAD_CONST              26 ('core.view_photo')
+               930 PRECALL                  1
+               934 CALL                     1
                944 BINARY_OP                7 (|)
    
     82         948 BINARY_OP                1 (&)
                952 STORE_NAME              33 (view_photo_predicate)
    
     85         954 PUSH_NULL
                956 LOAD_NAME                0 (rules)
@@ -516,26 +519,26 @@
                970 LOAD_NAME               33 (view_photo_predicate)
                972 PRECALL                  2
                976 CALL                     2
                986 POP_TOP
    
     88         988 LOAD_NAME               12 (has_person)
    
-    89         990 PUSH_NULL
-               992 LOAD_NAME               10 (has_global_perm)
-               994 LOAD_CONST              28 ('core.view_avatar')
-               996 PRECALL                  1
-              1000 CALL                     1
-              1010 PUSH_NULL
-              1012 LOAD_NAME               11 (has_object_perm)
-              1014 LOAD_CONST              28 ('core.view_avatar')
-              1016 PRECALL                  1
-              1020 CALL                     1
-              1030 BINARY_OP                7 (|)
-              1034 LOAD_NAME               14 (is_current_person)
+    89         990 LOAD_NAME               14 (is_current_person)
+               992 PUSH_NULL
+               994 LOAD_NAME               10 (has_global_perm)
+               996 LOAD_CONST              28 ('core.view_avatar')
+               998 PRECALL                  1
+              1002 CALL                     1
+              1012 BINARY_OP                7 (|)
+              1016 PUSH_NULL
+              1018 LOAD_NAME               11 (has_object_perm)
+              1020 LOAD_CONST              28 ('core.view_avatar')
+              1022 PRECALL                  1
+              1026 CALL                     1
               1036 BINARY_OP                7 (|)
    
     88        1040 BINARY_OP                1 (&)
               1044 STORE_NAME              34 (view_avatar_predicate)
    
     91        1046 PUSH_NULL
               1048 LOAD_NAME                0 (rules)
@@ -544,29 +547,29 @@
               1062 LOAD_NAME               34 (view_avatar_predicate)
               1064 PRECALL                  2
               1068 CALL                     2
               1078 POP_TOP
    
     94        1080 LOAD_NAME               12 (has_person)
    
-    95        1082 PUSH_NULL
-              1084 LOAD_NAME               10 (has_global_perm)
-              1086 LOAD_CONST              30 ('core.view_person_groups')
-              1088 PRECALL                  1
-              1092 CALL                     1
-   
-    96        1102 PUSH_NULL
-              1104 LOAD_NAME               11 (has_object_perm)
-              1106 LOAD_CONST              30 ('core.view_person_groups')
-              1108 PRECALL                  1
-              1112 CALL                     1
-   
-    95        1122 BINARY_OP                7 (|)
+    95        1082 LOAD_NAME               14 (is_current_person)
    
-    97        1126 LOAD_NAME               14 (is_current_person)
+    96        1084 PUSH_NULL
+              1086 LOAD_NAME               10 (has_global_perm)
+              1088 LOAD_CONST              30 ('core.view_person_groups')
+              1090 PRECALL                  1
+              1094 CALL                     1
+   
+    95        1104 BINARY_OP                7 (|)
+   
+    97        1108 PUSH_NULL
+              1110 LOAD_NAME               11 (has_object_perm)
+              1112 LOAD_CONST              30 ('core.view_person_groups')
+              1114 PRECALL                  1
+              1118 CALL                     1
    
     95        1128 BINARY_OP                7 (|)
    
     94        1132 BINARY_OP                1 (&)
               1136 STORE_NAME              35 (view_groups_predicate)
    
     99        1138 PUSH_NULL
@@ -576,36 +579,36 @@
               1154 LOAD_NAME               35 (view_groups_predicate)
               1156 PRECALL                  2
               1160 CALL                     2
               1170 POP_TOP
    
    102        1172 LOAD_NAME               12 (has_person)
    
-   103        1174 PUSH_NULL
-              1176 LOAD_NAME               10 (has_global_perm)
-              1178 LOAD_CONST              32 ('core.change_person')
-              1180 PRECALL                  1
-              1184 CALL                     1
-   
-   104        1194 PUSH_NULL
-              1196 LOAD_NAME               11 (has_object_perm)
-              1198 LOAD_CONST              32 ('core.change_person')
-              1200 PRECALL                  1
-              1204 CALL                     1
-   
-   103        1214 BINARY_OP                7 (|)
-   
-   105        1218 LOAD_NAME               14 (is_current_person)
-              1220 PUSH_NULL
-              1222 LOAD_NAME               18 (is_site_preference_set)
-              1224 LOAD_CONST              33 ('account')
-              1226 LOAD_CONST              34 ('editable_fields_person')
-              1228 PRECALL                  2
-              1232 CALL                     2
-              1242 BINARY_OP                1 (&)
+   103        1174 LOAD_NAME               14 (is_current_person)
+              1176 PUSH_NULL
+              1178 LOAD_NAME               18 (is_site_preference_set)
+              1180 LOAD_CONST              32 ('account')
+              1182 LOAD_CONST              33 ('editable_fields_person')
+              1184 PRECALL                  2
+              1188 CALL                     2
+              1198 BINARY_OP                1 (&)
+   
+   104        1202 PUSH_NULL
+              1204 LOAD_NAME               10 (has_global_perm)
+              1206 LOAD_CONST              34 ('core.change_person')
+              1208 PRECALL                  1
+              1212 CALL                     1
+   
+   103        1222 BINARY_OP                7 (|)
+   
+   105        1226 PUSH_NULL
+              1228 LOAD_NAME               11 (has_object_perm)
+              1230 LOAD_CONST              34 ('core.change_person')
+              1232 PRECALL                  1
+              1236 CALL                     1
    
    103        1246 BINARY_OP                7 (|)
    
    102        1250 BINARY_OP                1 (&)
               1254 STORE_NAME              36 (edit_person_predicate)
    
    107        1256 PUSH_NULL
@@ -961,29 +964,29 @@
    
    186        2396 PRECALL                  2
               2400 CALL                     2
               2410 POP_TOP
    
    193        2412 LOAD_NAME               12 (has_person)
    
-   194        2414 PUSH_NULL
-              2416 LOAD_NAME               10 (has_global_perm)
-              2418 LOAD_CONST              64 ('core.view_personal_details')
-              2420 PRECALL                  1
-              2424 CALL                     1
-   
-   195        2434 PUSH_NULL
-              2436 LOAD_NAME               11 (has_object_perm)
-              2438 LOAD_CONST              64 ('core.view_personal_details')
-              2440 PRECALL                  1
-              2444 CALL                     1
+   194        2414 LOAD_NAME               14 (is_current_person)
    
-   194        2454 BINARY_OP                7 (|)
-   
-   196        2458 LOAD_NAME               14 (is_current_person)
+   195        2416 PUSH_NULL
+              2418 LOAD_NAME               10 (has_global_perm)
+              2420 LOAD_CONST              64 ('core.view_personal_details')
+              2422 PRECALL                  1
+              2426 CALL                     1
+   
+   194        2436 BINARY_OP                7 (|)
+   
+   196        2440 PUSH_NULL
+              2442 LOAD_NAME               11 (has_object_perm)
+              2444 LOAD_CONST              64 ('core.view_personal_details')
+              2446 PRECALL                  1
+              2450 CALL                     1
    
    194        2460 BINARY_OP                7 (|)
    
    193        2464 BINARY_OP                1 (&)
               2468 STORE_NAME              50 (view_personal_details_predicate)
    
    198        2470 PUSH_NULL
@@ -1021,29 +1024,29 @@
               2572 LOAD_NAME               51 (change_site_preferences)
               2574 PRECALL                  2
               2578 CALL                     2
               2588 POP_TOP
    
    208        2590 LOAD_NAME               12 (has_person)
    
-   209        2592 PUSH_NULL
-              2594 LOAD_NAME               10 (has_global_perm)
-              2596 LOAD_CONST              68 ('core.change_person_preferences')
-              2598 PRECALL                  1
-              2602 CALL                     1
-   
-   210        2612 PUSH_NULL
-              2614 LOAD_NAME               11 (has_object_perm)
-              2616 LOAD_CONST              68 ('core.change_person_preferences')
-              2618 PRECALL                  1
-              2622 CALL                     1
-   
-   209        2632 BINARY_OP                7 (|)
+   209        2592 LOAD_NAME               14 (is_current_person)
    
-   211        2636 LOAD_NAME               14 (is_current_person)
+   210        2594 PUSH_NULL
+              2596 LOAD_NAME               10 (has_global_perm)
+              2598 LOAD_CONST              68 ('core.change_person_preferences')
+              2600 PRECALL                  1
+              2604 CALL                     1
+   
+   209        2614 BINARY_OP                7 (|)
+   
+   211        2618 PUSH_NULL
+              2620 LOAD_NAME               11 (has_object_perm)
+              2622 LOAD_CONST              68 ('core.change_person_preferences')
+              2624 PRECALL                  1
+              2628 CALL                     1
    
    209        2638 BINARY_OP                7 (|)
    
    208        2642 BINARY_OP                1 (&)
               2646 STORE_NAME              52 (change_person_preferences)
    
    213        2648 PUSH_NULL
@@ -1206,739 +1209,765 @@
               3146 CALL                     2
               3156 POP_TOP
    
    255        3158 LOAD_NAME               12 (has_person)
    
    256        3160 PUSH_NULL
               3162 LOAD_NAME               10 (has_global_perm)
-              3164 LOAD_CONST              81 ('core.change_grouptype')
+              3164 LOAD_CONST              81 ('core.view_grouptype')
               3166 PRECALL                  1
               3170 CALL                     1
               3180 PUSH_NULL
               3182 LOAD_NAME               11 (has_object_perm)
-              3184 LOAD_CONST              81 ('core.change_grouptype')
+              3184 LOAD_CONST              81 ('core.view_grouptype')
               3186 PRECALL                  1
               3190 CALL                     1
               3200 BINARY_OP                7 (|)
    
    255        3204 BINARY_OP                1 (&)
-              3208 STORE_NAME              59 (change_group_type_predicate)
+              3208 STORE_NAME              59 (view_group_type_predicate)
    
    258        3210 PUSH_NULL
               3212 LOAD_NAME                0 (rules)
               3214 LOAD_ATTR               19 (add_perm)
-              3224 LOAD_CONST              82 ('core.edit_grouptype_rule')
-              3226 LOAD_NAME               59 (change_group_type_predicate)
+              3224 LOAD_CONST              82 ('core.view_grouptype_rule')
+              3226 LOAD_NAME               59 (view_group_type_predicate)
               3228 PRECALL                  2
               3232 CALL                     2
               3242 POP_TOP
    
    261        3244 LOAD_NAME               12 (has_person)
    
    262        3246 PUSH_NULL
               3248 LOAD_NAME               10 (has_global_perm)
-              3250 LOAD_CONST              83 ('core.add_grouptype')
+              3250 LOAD_CONST              83 ('core.change_grouptype')
               3252 PRECALL                  1
               3256 CALL                     1
               3266 PUSH_NULL
               3268 LOAD_NAME               11 (has_object_perm)
-              3270 LOAD_CONST              83 ('core.add_grouptype')
+              3270 LOAD_CONST              83 ('core.change_grouptype')
               3272 PRECALL                  1
               3276 CALL                     1
               3286 BINARY_OP                7 (|)
    
    261        3290 BINARY_OP                1 (&)
-              3294 STORE_NAME              60 (create_group_type_predicate)
+              3294 STORE_NAME              60 (change_group_type_predicate)
    
    264        3296 PUSH_NULL
               3298 LOAD_NAME                0 (rules)
               3300 LOAD_ATTR               19 (add_perm)
-              3310 LOAD_CONST              84 ('core.create_grouptype_rule')
-              3312 LOAD_NAME               60 (create_group_type_predicate)
+              3310 LOAD_CONST              84 ('core.edit_grouptype_rule')
+              3312 LOAD_NAME               60 (change_group_type_predicate)
               3314 PRECALL                  2
               3318 CALL                     2
               3328 POP_TOP
    
-   268        3330 LOAD_NAME               12 (has_person)
+   267        3330 LOAD_NAME               12 (has_person)
    
-   269        3332 PUSH_NULL
+   268        3332 PUSH_NULL
               3334 LOAD_NAME               10 (has_global_perm)
-              3336 LOAD_CONST              85 ('core.delete_grouptype')
+              3336 LOAD_CONST              85 ('core.add_grouptype')
               3338 PRECALL                  1
               3342 CALL                     1
               3352 PUSH_NULL
               3354 LOAD_NAME               11 (has_object_perm)
-              3356 LOAD_CONST              85 ('core.delete_grouptype')
+              3356 LOAD_CONST              85 ('core.add_grouptype')
               3358 PRECALL                  1
               3362 CALL                     1
               3372 BINARY_OP                7 (|)
    
-   268        3376 BINARY_OP                1 (&)
-              3380 STORE_NAME              61 (delete_group_type_predicate)
+   267        3376 BINARY_OP                1 (&)
+              3380 STORE_NAME              61 (create_group_type_predicate)
    
-   271        3382 PUSH_NULL
+   270        3382 PUSH_NULL
               3384 LOAD_NAME                0 (rules)
               3386 LOAD_ATTR               19 (add_perm)
-              3396 LOAD_CONST              86 ('core.delete_grouptype_rule')
-              3398 LOAD_NAME               61 (delete_group_type_predicate)
+              3396 LOAD_CONST              86 ('core.create_grouptype_rule')
+              3398 LOAD_NAME               61 (create_group_type_predicate)
               3400 PRECALL                  2
               3404 CALL                     2
               3414 POP_TOP
    
    274        3416 LOAD_NAME               12 (has_person)
    
    275        3418 PUSH_NULL
               3420 LOAD_NAME               10 (has_global_perm)
-              3422 LOAD_CONST              87 ('core.view_grouptype')
+              3422 LOAD_CONST              87 ('core.delete_grouptype')
               3424 PRECALL                  1
               3428 CALL                     1
               3438 PUSH_NULL
-              3440 LOAD_NAME                9 (has_any_object)
-              3442 LOAD_CONST              87 ('core.view_grouptype')
-              3444 LOAD_NAME                6 (GroupType)
-              3446 PRECALL                  2
-              3450 CALL                     2
-              3460 BINARY_OP                7 (|)
-   
-   274        3464 BINARY_OP                1 (&)
-              3468 STORE_NAME              62 (view_group_types_predicate)
-   
-   277        3470 PUSH_NULL
-              3472 LOAD_NAME                0 (rules)
-              3474 LOAD_ATTR               19 (add_perm)
-              3484 LOAD_CONST              88 ('core.view_grouptypes_rule')
-              3486 LOAD_NAME               62 (view_group_types_predicate)
-              3488 PRECALL                  2
-              3492 CALL                     2
-              3502 POP_TOP
-   
-   280        3504 LOAD_NAME               12 (has_person)
-   
-   281        3506 PUSH_NULL
-              3508 LOAD_NAME               10 (has_global_perm)
-              3510 LOAD_CONST              89 ('core.add_person')
-              3512 PRECALL                  1
-              3516 CALL                     1
-              3526 PUSH_NULL
-              3528 LOAD_NAME               11 (has_object_perm)
-              3530 LOAD_CONST              89 ('core.add_person')
-              3532 PRECALL                  1
-              3536 CALL                     1
+              3440 LOAD_NAME               11 (has_object_perm)
+              3442 LOAD_CONST              87 ('core.delete_grouptype')
+              3444 PRECALL                  1
+              3448 CALL                     1
+              3458 BINARY_OP                7 (|)
+   
+   274        3462 BINARY_OP                1 (&)
+              3466 STORE_NAME              62 (delete_group_type_predicate)
+   
+   277        3468 PUSH_NULL
+              3470 LOAD_NAME                0 (rules)
+              3472 LOAD_ATTR               19 (add_perm)
+              3482 LOAD_CONST              88 ('core.delete_grouptype_rule')
+              3484 LOAD_NAME               62 (delete_group_type_predicate)
+              3486 PRECALL                  2
+              3490 CALL                     2
+              3500 POP_TOP
+   
+   280        3502 LOAD_NAME               12 (has_person)
+   
+   281        3504 PUSH_NULL
+              3506 LOAD_NAME               10 (has_global_perm)
+              3508 LOAD_CONST              81 ('core.view_grouptype')
+              3510 PRECALL                  1
+              3514 CALL                     1
+              3524 PUSH_NULL
+              3526 LOAD_NAME                9 (has_any_object)
+              3528 LOAD_CONST              81 ('core.view_grouptype')
+              3530 LOAD_NAME                6 (GroupType)
+              3532 PRECALL                  2
+              3536 CALL                     2
               3546 BINARY_OP                7 (|)
    
    280        3550 BINARY_OP                1 (&)
-              3554 STORE_NAME              63 (create_person_predicate)
+              3554 STORE_NAME              63 (view_group_types_predicate)
    
    283        3556 PUSH_NULL
               3558 LOAD_NAME                0 (rules)
               3560 LOAD_ATTR               19 (add_perm)
-              3570 LOAD_CONST              90 ('core.create_person_rule')
-              3572 LOAD_NAME               63 (create_person_predicate)
+              3570 LOAD_CONST              89 ('core.view_grouptypes_rule')
+              3572 LOAD_NAME               63 (view_group_types_predicate)
               3574 PRECALL                  2
               3578 CALL                     2
               3588 POP_TOP
    
    286        3590 LOAD_NAME               12 (has_person)
    
    287        3592 PUSH_NULL
               3594 LOAD_NAME               10 (has_global_perm)
-              3596 LOAD_CONST              91 ('core.add_group')
+              3596 LOAD_CONST              90 ('core.add_person')
               3598 PRECALL                  1
               3602 CALL                     1
               3612 PUSH_NULL
               3614 LOAD_NAME               11 (has_object_perm)
-              3616 LOAD_CONST              91 ('core.add_group')
+              3616 LOAD_CONST              90 ('core.add_person')
               3618 PRECALL                  1
               3622 CALL                     1
               3632 BINARY_OP                7 (|)
    
    286        3636 BINARY_OP                1 (&)
-              3640 STORE_NAME              64 (create_group_predicate)
+              3640 STORE_NAME              64 (create_person_predicate)
    
    289        3642 PUSH_NULL
               3644 LOAD_NAME                0 (rules)
               3646 LOAD_ATTR               19 (add_perm)
-              3656 LOAD_CONST              92 ('core.create_group_rule')
-              3658 LOAD_NAME               64 (create_group_predicate)
+              3656 LOAD_CONST              91 ('core.create_person_rule')
+              3658 LOAD_NAME               64 (create_person_predicate)
               3660 PRECALL                  2
               3664 CALL                     2
               3674 POP_TOP
    
    292        3676 LOAD_NAME               12 (has_person)
-              3678 PUSH_NULL
+   
+   293        3678 PUSH_NULL
               3680 LOAD_NAME               10 (has_global_perm)
-              3682 LOAD_CONST              93 ('core.view_schoolterm')
+              3682 LOAD_CONST              92 ('core.add_group')
               3684 PRECALL                  1
               3688 CALL                     1
-              3698 BINARY_OP                1 (&)
-              3702 STORE_NAME              65 (view_school_term_predicate)
-   
-   293        3704 PUSH_NULL
-              3706 LOAD_NAME                0 (rules)
-              3708 LOAD_ATTR               19 (add_perm)
-              3718 LOAD_CONST              94 ('core.view_schoolterm_rule')
-              3720 LOAD_NAME               65 (view_school_term_predicate)
-              3722 PRECALL                  2
-              3726 CALL                     2
-              3736 POP_TOP
-   
-   295        3738 LOAD_NAME               12 (has_person)
-              3740 PUSH_NULL
-              3742 LOAD_NAME               10 (has_global_perm)
-              3744 LOAD_CONST              95 ('core.add_schoolterm')
-              3746 PRECALL                  1
-              3750 CALL                     1
-              3760 BINARY_OP                1 (&)
-              3764 STORE_NAME              66 (create_school_term_predicate)
-   
-   296        3766 PUSH_NULL
-              3768 LOAD_NAME                0 (rules)
-              3770 LOAD_ATTR               19 (add_perm)
-              3780 LOAD_CONST              96 ('core.create_schoolterm_rule')
-              3782 LOAD_NAME               66 (create_school_term_predicate)
-              3784 PRECALL                  2
-              3788 CALL                     2
-              3798 POP_TOP
-   
-   298        3800 LOAD_NAME               12 (has_person)
-              3802 PUSH_NULL
-              3804 LOAD_NAME               10 (has_global_perm)
-              3806 LOAD_CONST              97 ('core.change_schoolterm')
-              3808 PRECALL                  1
-              3812 CALL                     1
-              3822 BINARY_OP                1 (&)
-              3826 STORE_NAME              67 (edit_school_term_predicate)
-   
-   299        3828 PUSH_NULL
-              3830 LOAD_NAME                0 (rules)
-              3832 LOAD_ATTR               19 (add_perm)
-              3842 LOAD_CONST              98 ('core.edit_schoolterm_rule')
-              3844 LOAD_NAME               67 (edit_school_term_predicate)
-              3846 PRECALL                  2
-              3850 CALL                     2
-              3860 POP_TOP
-   
-   302        3862 LOAD_NAME               12 (has_person)
-   
-   303        3864 PUSH_NULL
-              3866 LOAD_NAME               10 (has_global_perm)
-              3868 LOAD_CONST              99 ('core.view_group_stats')
-              3870 PRECALL                  1
-              3874 CALL                     1
-              3884 PUSH_NULL
-              3886 LOAD_NAME               11 (has_object_perm)
-              3888 LOAD_CONST              99 ('core.view_group_stats')
-              3890 PRECALL                  1
-              3894 CALL                     1
-              3904 BINARY_OP                7 (|)
-   
-   302        3908 BINARY_OP                1 (&)
-              3912 STORE_NAME              68 (view_group_stats_predicate)
+              3698 PUSH_NULL
+              3700 LOAD_NAME               11 (has_object_perm)
+              3702 LOAD_CONST              92 ('core.add_group')
+              3704 PRECALL                  1
+              3708 CALL                     1
+              3718 BINARY_OP                7 (|)
+   
+   292        3722 BINARY_OP                1 (&)
+              3726 STORE_NAME              65 (create_group_predicate)
+   
+   295        3728 PUSH_NULL
+              3730 LOAD_NAME                0 (rules)
+              3732 LOAD_ATTR               19 (add_perm)
+              3742 LOAD_CONST              93 ('core.create_group_rule')
+              3744 LOAD_NAME               65 (create_group_predicate)
+              3746 PRECALL                  2
+              3750 CALL                     2
+              3760 POP_TOP
+   
+   298        3762 LOAD_NAME               12 (has_person)
+              3764 PUSH_NULL
+              3766 LOAD_NAME               10 (has_global_perm)
+              3768 LOAD_CONST              94 ('core.view_schoolterm')
+              3770 PRECALL                  1
+              3774 CALL                     1
+              3784 BINARY_OP                1 (&)
+              3788 STORE_NAME              66 (view_school_term_predicate)
+   
+   299        3790 PUSH_NULL
+              3792 LOAD_NAME                0 (rules)
+              3794 LOAD_ATTR               19 (add_perm)
+              3804 LOAD_CONST              95 ('core.view_schoolterm_rule')
+              3806 LOAD_NAME               66 (view_school_term_predicate)
+              3808 PRECALL                  2
+              3812 CALL                     2
+              3822 POP_TOP
+   
+   301        3824 LOAD_NAME               12 (has_person)
+              3826 PUSH_NULL
+              3828 LOAD_NAME               10 (has_global_perm)
+              3830 LOAD_CONST              96 ('core.add_schoolterm')
+              3832 PRECALL                  1
+              3836 CALL                     1
+              3846 BINARY_OP                1 (&)
+              3850 STORE_NAME              67 (create_school_term_predicate)
+   
+   302        3852 PUSH_NULL
+              3854 LOAD_NAME                0 (rules)
+              3856 LOAD_ATTR               19 (add_perm)
+              3866 LOAD_CONST              97 ('core.create_schoolterm_rule')
+              3868 LOAD_NAME               67 (create_school_term_predicate)
+              3870 PRECALL                  2
+              3874 CALL                     2
+              3884 POP_TOP
+   
+   304        3886 LOAD_NAME               12 (has_person)
+              3888 PUSH_NULL
+              3890 LOAD_NAME               10 (has_global_perm)
+              3892 LOAD_CONST              98 ('core.change_schoolterm')
+              3894 PRECALL                  1
+              3898 CALL                     1
+              3908 BINARY_OP                1 (&)
+              3912 STORE_NAME              68 (edit_school_term_predicate)
    
    305        3914 PUSH_NULL
               3916 LOAD_NAME                0 (rules)
               3918 LOAD_ATTR               19 (add_perm)
-              3928 LOAD_CONST             100 ('core.view_group_stats_rule')
-              3930 LOAD_NAME               68 (view_group_stats_predicate)
+              3928 LOAD_CONST              99 ('core.edit_schoolterm_rule')
+              3930 LOAD_NAME               68 (edit_school_term_predicate)
               3932 PRECALL                  2
               3936 CALL                     2
               3946 POP_TOP
    
    308        3948 LOAD_NAME               12 (has_person)
-              3950 PUSH_NULL
+   
+   309        3950 PUSH_NULL
               3952 LOAD_NAME               10 (has_global_perm)
-              3954 LOAD_CONST             101 ('core.view_datacheckresult')
+              3954 LOAD_CONST             100 ('core.view_group_stats')
               3956 PRECALL                  1
               3960 CALL                     1
-              3970 BINARY_OP                1 (&)
-              3974 STORE_NAME              69 (view_data_check_results_predicate)
+              3970 PUSH_NULL
+              3972 LOAD_NAME               11 (has_object_perm)
+              3974 LOAD_CONST             100 ('core.view_group_stats')
+              3976 PRECALL                  1
+              3980 CALL                     1
+              3990 BINARY_OP                7 (|)
+   
+   308        3994 BINARY_OP                1 (&)
+              3998 STORE_NAME              69 (view_group_stats_predicate)
+   
+   311        4000 PUSH_NULL
+              4002 LOAD_NAME                0 (rules)
+              4004 LOAD_ATTR               19 (add_perm)
+              4014 LOAD_CONST             101 ('core.view_group_stats_rule')
+              4016 LOAD_NAME               69 (view_group_stats_predicate)
+              4018 PRECALL                  2
+              4022 CALL                     2
+              4032 POP_TOP
+   
+   314        4034 LOAD_NAME               12 (has_person)
+              4036 PUSH_NULL
+              4038 LOAD_NAME               10 (has_global_perm)
+              4040 LOAD_CONST             102 ('core.view_datacheckresult')
+              4042 PRECALL                  1
+              4046 CALL                     1
+              4056 BINARY_OP                1 (&)
+              4060 STORE_NAME              70 (view_data_check_results_predicate)
+   
+   315        4062 PUSH_NULL
+              4064 LOAD_NAME                0 (rules)
+              4066 LOAD_ATTR               19 (add_perm)
+              4076 LOAD_CONST             103 ('core.view_datacheckresults_rule')
+              4078 LOAD_NAME               70 (view_data_check_results_predicate)
+              4080 PRECALL                  2
+              4084 CALL                     2
+              4094 POP_TOP
+   
+   319        4096 LOAD_NAME               12 (has_person)
+              4098 LOAD_NAME               70 (view_data_check_results_predicate)
+              4100 BINARY_OP                1 (&)
+              4104 PUSH_NULL
+              4106 LOAD_NAME               10 (has_global_perm)
+              4108 LOAD_CONST             104 ('core.run_data_checks')
+              4110 PRECALL                  1
+              4114 CALL                     1
+              4124 BINARY_OP                1 (&)
+   
+   318        4128 STORE_NAME              71 (run_data_checks_predicate)
+   
+   321        4130 PUSH_NULL
+              4132 LOAD_NAME                0 (rules)
+              4134 LOAD_ATTR               19 (add_perm)
+              4144 LOAD_CONST             105 ('core.run_data_checks_rule')
+              4146 LOAD_NAME               71 (run_data_checks_predicate)
+              4148 PRECALL                  2
+              4152 CALL                     2
+              4162 POP_TOP
    
-   309        3976 PUSH_NULL
-              3978 LOAD_NAME                0 (rules)
-              3980 LOAD_ATTR               19 (add_perm)
-              3990 LOAD_CONST             102 ('core.view_datacheckresults_rule')
-              3992 LOAD_NAME               69 (view_data_check_results_predicate)
-              3994 PRECALL                  2
-              3998 CALL                     2
-              4008 POP_TOP
-   
-   313        4010 LOAD_NAME               12 (has_person)
-              4012 LOAD_NAME               69 (view_data_check_results_predicate)
-              4014 BINARY_OP                1 (&)
-              4018 PUSH_NULL
-              4020 LOAD_NAME               10 (has_global_perm)
-              4022 LOAD_CONST             103 ('core.run_data_checks')
-              4024 PRECALL                  1
-              4028 CALL                     1
-              4038 BINARY_OP                1 (&)
-   
-   312        4042 STORE_NAME              70 (run_data_checks_predicate)
-   
-   315        4044 PUSH_NULL
-              4046 LOAD_NAME                0 (rules)
-              4048 LOAD_ATTR               19 (add_perm)
-              4058 LOAD_CONST             104 ('core.run_data_checks_rule')
-              4060 LOAD_NAME               70 (run_data_checks_predicate)
-              4062 PRECALL                  2
-              4066 CALL                     2
-              4076 POP_TOP
-   
-   319        4078 LOAD_NAME               12 (has_person)
-              4080 LOAD_NAME               69 (view_data_check_results_predicate)
-              4082 BINARY_OP                1 (&)
-              4086 PUSH_NULL
-              4088 LOAD_NAME               10 (has_global_perm)
-              4090 LOAD_CONST             105 ('core.solve_data_problem')
-              4092 PRECALL                  1
-              4096 CALL                     1
-              4106 BINARY_OP                1 (&)
-   
-   318        4110 STORE_NAME              71 (solve_data_problem_predicate)
-   
-   321        4112 PUSH_NULL
-              4114 LOAD_NAME                0 (rules)
-              4116 LOAD_ATTR               19 (add_perm)
-              4126 LOAD_CONST             106 ('core.solve_data_problem_rule')
-              4128 LOAD_NAME               71 (solve_data_problem_predicate)
-              4130 PRECALL                  2
-              4134 CALL                     2
-              4144 POP_TOP
-   
-   323        4146 LOAD_NAME               12 (has_person)
-              4148 PUSH_NULL
-              4150 LOAD_NAME               10 (has_global_perm)
-              4152 LOAD_CONST             107 ('core.view_dashboardwidget')
-              4154 PRECALL                  1
-              4158 CALL                     1
+   325        4164 LOAD_NAME               12 (has_person)
+              4166 LOAD_NAME               70 (view_data_check_results_predicate)
               4168 BINARY_OP                1 (&)
-              4172 STORE_NAME              72 (view_dashboard_widget_predicate)
-   
-   324        4174 PUSH_NULL
-              4176 LOAD_NAME                0 (rules)
-              4178 LOAD_ATTR               19 (add_perm)
-              4188 LOAD_CONST             108 ('core.view_dashboardwidget_rule')
-              4190 LOAD_NAME               72 (view_dashboard_widget_predicate)
-              4192 PRECALL                  2
-              4196 CALL                     2
-              4206 POP_TOP
-   
-   326        4208 LOAD_NAME               12 (has_person)
-              4210 PUSH_NULL
-              4212 LOAD_NAME               10 (has_global_perm)
-              4214 LOAD_CONST             109 ('core.add_dashboardwidget')
-              4216 PRECALL                  1
-              4220 CALL                     1
-              4230 BINARY_OP                1 (&)
-              4234 STORE_NAME              73 (create_dashboard_widget_predicate)
-   
-   327        4236 PUSH_NULL
-              4238 LOAD_NAME                0 (rules)
-              4240 LOAD_ATTR               19 (add_perm)
-              4250 LOAD_CONST             110 ('core.create_dashboardwidget_rule')
-              4252 LOAD_NAME               73 (create_dashboard_widget_predicate)
-              4254 PRECALL                  2
-              4258 CALL                     2
-              4268 POP_TOP
-   
-   329        4270 LOAD_NAME               12 (has_person)
-              4272 PUSH_NULL
-              4274 LOAD_NAME               10 (has_global_perm)
-              4276 LOAD_CONST             111 ('core.change_dashboardwidget')
-              4278 PRECALL                  1
-              4282 CALL                     1
-              4292 BINARY_OP                1 (&)
-              4296 STORE_NAME              74 (edit_dashboard_widget_predicate)
-   
-   330        4298 PUSH_NULL
-              4300 LOAD_NAME                0 (rules)
-              4302 LOAD_ATTR               19 (add_perm)
-              4312 LOAD_CONST             112 ('core.edit_dashboardwidget_rule')
-              4314 LOAD_NAME               74 (edit_dashboard_widget_predicate)
-              4316 PRECALL                  2
-              4320 CALL                     2
-              4330 POP_TOP
-   
-   332        4332 LOAD_NAME               12 (has_person)
-              4334 PUSH_NULL
-              4336 LOAD_NAME               10 (has_global_perm)
-              4338 LOAD_CONST             113 ('core.delete_dashboardwidget')
-              4340 PRECALL                  1
-              4344 CALL                     1
-              4354 BINARY_OP                1 (&)
-              4358 STORE_NAME              75 (delete_dashboard_widget_predicate)
-   
-   333        4360 PUSH_NULL
-              4362 LOAD_NAME                0 (rules)
-              4364 LOAD_ATTR               19 (add_perm)
-              4374 LOAD_CONST             114 ('core.delete_dashboardwidget_rule')
-              4376 LOAD_NAME               75 (delete_dashboard_widget_predicate)
-              4378 PRECALL                  2
-              4382 CALL                     2
-              4392 POP_TOP
-   
-   335        4394 PUSH_NULL
-              4396 LOAD_NAME               18 (is_site_preference_set)
-              4398 LOAD_CONST              13 ('general')
-              4400 LOAD_CONST             115 ('dashboard_editing')
+              4172 PUSH_NULL
+              4174 LOAD_NAME               10 (has_global_perm)
+              4176 LOAD_CONST             106 ('core.solve_data_problem')
+              4178 PRECALL                  1
+              4182 CALL                     1
+              4192 BINARY_OP                1 (&)
+   
+   324        4196 STORE_NAME              72 (solve_data_problem_predicate)
+   
+   327        4198 PUSH_NULL
+              4200 LOAD_NAME                0 (rules)
+              4202 LOAD_ATTR               19 (add_perm)
+              4212 LOAD_CONST             107 ('core.solve_data_problem_rule')
+              4214 LOAD_NAME               72 (solve_data_problem_predicate)
+              4216 PRECALL                  2
+              4220 CALL                     2
+              4230 POP_TOP
+   
+   329        4232 LOAD_NAME               12 (has_person)
+              4234 PUSH_NULL
+              4236 LOAD_NAME               10 (has_global_perm)
+              4238 LOAD_CONST             108 ('core.view_dashboardwidget')
+              4240 PRECALL                  1
+              4244 CALL                     1
+              4254 BINARY_OP                1 (&)
+              4258 STORE_NAME              73 (view_dashboard_widget_predicate)
+   
+   330        4260 PUSH_NULL
+              4262 LOAD_NAME                0 (rules)
+              4264 LOAD_ATTR               19 (add_perm)
+              4274 LOAD_CONST             109 ('core.view_dashboardwidget_rule')
+              4276 LOAD_NAME               73 (view_dashboard_widget_predicate)
+              4278 PRECALL                  2
+              4282 CALL                     2
+              4292 POP_TOP
+   
+   332        4294 LOAD_NAME               12 (has_person)
+              4296 PUSH_NULL
+              4298 LOAD_NAME               10 (has_global_perm)
+              4300 LOAD_CONST             110 ('core.add_dashboardwidget')
+              4302 PRECALL                  1
+              4306 CALL                     1
+              4316 BINARY_OP                1 (&)
+              4320 STORE_NAME              74 (create_dashboard_widget_predicate)
+   
+   333        4322 PUSH_NULL
+              4324 LOAD_NAME                0 (rules)
+              4326 LOAD_ATTR               19 (add_perm)
+              4336 LOAD_CONST             111 ('core.create_dashboardwidget_rule')
+              4338 LOAD_NAME               74 (create_dashboard_widget_predicate)
+              4340 PRECALL                  2
+              4344 CALL                     2
+              4354 POP_TOP
+   
+   335        4356 LOAD_NAME               12 (has_person)
+              4358 PUSH_NULL
+              4360 LOAD_NAME               10 (has_global_perm)
+              4362 LOAD_CONST             112 ('core.change_dashboardwidget')
+              4364 PRECALL                  1
+              4368 CALL                     1
+              4378 BINARY_OP                1 (&)
+              4382 STORE_NAME              75 (edit_dashboard_widget_predicate)
+   
+   336        4384 PUSH_NULL
+              4386 LOAD_NAME                0 (rules)
+              4388 LOAD_ATTR               19 (add_perm)
+              4398 LOAD_CONST             113 ('core.edit_dashboardwidget_rule')
+              4400 LOAD_NAME               75 (edit_dashboard_widget_predicate)
               4402 PRECALL                  2
               4406 CALL                     2
-              4416 LOAD_NAME               12 (has_person)
-              4418 BINARY_OP                1 (&)
-              4422 STORE_NAME              76 (edit_dashboard_predicate)
-   
-   336        4424 PUSH_NULL
-              4426 LOAD_NAME                0 (rules)
-              4428 LOAD_ATTR               19 (add_perm)
-              4438 LOAD_CONST             116 ('core.edit_dashboard_rule')
-              4440 LOAD_NAME               76 (edit_dashboard_predicate)
-              4442 PRECALL                  2
-              4446 CALL                     2
-              4456 POP_TOP
-   
-   338        4458 LOAD_NAME               12 (has_person)
-              4460 PUSH_NULL
-              4462 LOAD_NAME               10 (has_global_perm)
-              4464 LOAD_CONST             117 ('core.edit_default_dashboard')
-              4466 PRECALL                  1
-              4470 CALL                     1
-              4480 BINARY_OP                1 (&)
-              4484 STORE_NAME              77 (edit_default_dashboard_predicate)
-   
-   339        4486 PUSH_NULL
-              4488 LOAD_NAME                0 (rules)
-              4490 LOAD_ATTR               19 (add_perm)
-              4500 LOAD_CONST             118 ('core.edit_default_dashboard_rule')
-              4502 LOAD_NAME               77 (edit_default_dashboard_predicate)
-              4504 PRECALL                  2
-              4508 CALL                     2
-              4518 POP_TOP
-   
-   342        4520 PUSH_NULL
-              4522 LOAD_NAME               18 (is_site_preference_set)
-              4524 LOAD_CONST             119 ('auth')
-              4526 LOAD_CONST             120 ('signup_enabled')
-              4528 KW_NAMES               121
-              4530 PRECALL                  2
-              4534 CALL                     2
-              4544 STORE_NAME              78 (signup_predicate)
-   
-   343        4546 PUSH_NULL
-              4548 LOAD_NAME                0 (rules)
-              4550 LOAD_ATTR               19 (add_perm)
-              4560 LOAD_CONST             122 ('core.signup_rule')
-              4562 LOAD_NAME               78 (signup_predicate)
-              4564 PRECALL                  2
-              4568 CALL                     2
-              4578 POP_TOP
-   
-   345        4580 PUSH_NULL
-              4582 LOAD_NAME               18 (is_site_preference_set)
-              4584 LOAD_CONST             119 ('auth')
-              4586 LOAD_CONST             123 ('allow_password_change')
-              4588 KW_NAMES               121
+              4416 POP_TOP
+   
+   338        4418 LOAD_NAME               12 (has_person)
+              4420 PUSH_NULL
+              4422 LOAD_NAME               10 (has_global_perm)
+              4424 LOAD_CONST             114 ('core.delete_dashboardwidget')
+              4426 PRECALL                  1
+              4430 CALL                     1
+              4440 BINARY_OP                1 (&)
+              4444 STORE_NAME              76 (delete_dashboard_widget_predicate)
+   
+   339        4446 PUSH_NULL
+              4448 LOAD_NAME                0 (rules)
+              4450 LOAD_ATTR               19 (add_perm)
+              4460 LOAD_CONST             115 ('core.delete_dashboardwidget_rule')
+              4462 LOAD_NAME               76 (delete_dashboard_widget_predicate)
+              4464 PRECALL                  2
+              4468 CALL                     2
+              4478 POP_TOP
+   
+   341        4480 PUSH_NULL
+              4482 LOAD_NAME               18 (is_site_preference_set)
+              4484 LOAD_CONST              13 ('general')
+              4486 LOAD_CONST             116 ('dashboard_editing')
+              4488 PRECALL                  2
+              4492 CALL                     2
+              4502 LOAD_NAME               12 (has_person)
+              4504 BINARY_OP                1 (&)
+              4508 STORE_NAME              77 (edit_dashboard_predicate)
+   
+   342        4510 PUSH_NULL
+              4512 LOAD_NAME                0 (rules)
+              4514 LOAD_ATTR               19 (add_perm)
+              4524 LOAD_CONST             117 ('core.edit_dashboard_rule')
+              4526 LOAD_NAME               77 (edit_dashboard_predicate)
+              4528 PRECALL                  2
+              4532 CALL                     2
+              4542 POP_TOP
+   
+   344        4544 LOAD_NAME               12 (has_person)
+              4546 PUSH_NULL
+              4548 LOAD_NAME               10 (has_global_perm)
+              4550 LOAD_CONST             118 ('core.edit_default_dashboard')
+              4552 PRECALL                  1
+              4556 CALL                     1
+              4566 BINARY_OP                1 (&)
+              4570 STORE_NAME              78 (edit_default_dashboard_predicate)
+   
+   345        4572 PUSH_NULL
+              4574 LOAD_NAME                0 (rules)
+              4576 LOAD_ATTR               19 (add_perm)
+              4586 LOAD_CONST             119 ('core.edit_default_dashboard_rule')
+              4588 LOAD_NAME               78 (edit_default_dashboard_predicate)
               4590 PRECALL                  2
               4594 CALL                     2
-              4604 STORE_NAME              79 (change_password_predicate)
+              4604 POP_TOP
    
-   346        4606 PUSH_NULL
-              4608 LOAD_NAME                0 (rules)
-              4610 LOAD_ATTR               19 (add_perm)
-              4620 LOAD_CONST             124 ('core.change_password_rule')
-              4622 LOAD_NAME               79 (change_password_predicate)
-              4624 PRECALL                  2
-              4628 CALL                     2
-              4638 POP_TOP
-   
-   348        4640 PUSH_NULL
-              4642 LOAD_NAME               18 (is_site_preference_set)
-              4644 LOAD_CONST             119 ('auth')
-              4646 LOAD_CONST             125 ('allow_password_reset')
-              4648 KW_NAMES               121
+   348        4606 PUSH_NULL
+              4608 LOAD_NAME               18 (is_site_preference_set)
+              4610 LOAD_CONST             120 ('auth')
+              4612 LOAD_CONST             121 ('signup_enabled')
+              4614 KW_NAMES               122
+              4616 PRECALL                  2
+              4620 CALL                     2
+              4630 STORE_NAME              79 (signup_predicate)
+   
+   349        4632 PUSH_NULL
+              4634 LOAD_NAME                0 (rules)
+              4636 LOAD_ATTR               19 (add_perm)
+              4646 LOAD_CONST             123 ('core.signup_rule')
+              4648 LOAD_NAME               79 (signup_predicate)
               4650 PRECALL                  2
               4654 CALL                     2
-              4664 STORE_NAME              80 (reset_password_predicate)
+              4664 POP_TOP
    
-   349        4666 PUSH_NULL
-              4668 LOAD_NAME                0 (rules)
-              4670 LOAD_ATTR               19 (add_perm)
-              4680 LOAD_CONST             126 ('core.reset_password_rule')
-              4682 LOAD_NAME               80 (reset_password_predicate)
-              4684 PRECALL                  2
-              4688 CALL                     2
-              4698 POP_TOP
-   
-   352        4700 PUSH_NULL
-              4702 LOAD_NAME               18 (is_site_preference_set)
-              4704 LOAD_CONST             119 ('auth')
-              4706 LOAD_CONST             127 ('invite_enabled')
-              4708 KW_NAMES               121
+   351        4666 PUSH_NULL
+              4668 LOAD_NAME               18 (is_site_preference_set)
+              4670 LOAD_CONST             120 ('auth')
+              4672 LOAD_CONST             124 ('allow_password_change')
+              4674 KW_NAMES               122
+              4676 PRECALL                  2
+              4680 CALL                     2
+              4690 STORE_NAME              80 (change_password_predicate)
+   
+   352        4692 PUSH_NULL
+              4694 LOAD_NAME                0 (rules)
+              4696 LOAD_ATTR               19 (add_perm)
+              4706 LOAD_CONST             125 ('core.change_password_rule')
+              4708 LOAD_NAME               80 (change_password_predicate)
               4710 PRECALL                  2
               4714 CALL                     2
-              4724 STORE_NAME              81 (invite_enabled_predicate)
+              4724 POP_TOP
    
-   353        4726 PUSH_NULL
-              4728 LOAD_NAME                0 (rules)
-              4730 LOAD_ATTR               19 (add_perm)
-              4740 LOAD_CONST             128 ('core.invite_enabled')
-              4742 LOAD_NAME               81 (invite_enabled_predicate)
-              4744 PRECALL                  2
-              4748 CALL                     2
-              4758 POP_TOP
-   
-   355        4760 LOAD_NAME               12 (has_person)
-              4762 LOAD_NAME               81 (invite_enabled_predicate)
-              4764 BINARY_OP                1 (&)
-              4768 STORE_NAME              82 (accept_invite_predicate)
-   
-   356        4770 PUSH_NULL
-              4772 LOAD_NAME                0 (rules)
-              4774 LOAD_ATTR               19 (add_perm)
-              4784 LOAD_CONST             129 ('core.accept_invite_rule')
-              4786 LOAD_NAME               82 (accept_invite_predicate)
-              4788 PRECALL                  2
-              4792 CALL                     2
-              4802 POP_TOP
-   
-   358        4804 LOAD_NAME               12 (has_person)
-              4806 LOAD_NAME               81 (invite_enabled_predicate)
-              4808 BINARY_OP                1 (&)
-              4812 PUSH_NULL
-              4814 LOAD_NAME               10 (has_global_perm)
-              4816 LOAD_CONST             130 ('core.invite')
-              4818 PRECALL                  1
-              4822 CALL                     1
-              4832 BINARY_OP                1 (&)
-              4836 STORE_NAME              83 (invite_predicate)
-   
-   359        4838 PUSH_NULL
-              4840 LOAD_NAME                0 (rules)
-              4842 LOAD_ATTR               19 (add_perm)
-              4852 LOAD_CONST             131 ('core.invite_rule')
-              4854 LOAD_NAME               83 (invite_predicate)
-              4856 PRECALL                  2
-              4860 CALL                     2
-              4870 POP_TOP
-   
-   362        4872 LOAD_NAME               12 (has_person)
-              4874 PUSH_NULL
-              4876 LOAD_NAME               10 (has_global_perm)
-              4878 LOAD_CONST             132 ('core.add_oauthapplication')
-              4880 PRECALL                  1
-              4884 CALL                     1
-              4894 BINARY_OP                1 (&)
-              4898 STORE_NAME              84 (create_oauthapplication_predicate)
+   354        4726 PUSH_NULL
+              4728 LOAD_NAME               18 (is_site_preference_set)
+              4730 LOAD_CONST             120 ('auth')
+              4732 LOAD_CONST             126 ('allow_password_reset')
+              4734 KW_NAMES               122
+              4736 PRECALL                  2
+              4740 CALL                     2
+              4750 STORE_NAME              81 (reset_password_predicate)
+   
+   355        4752 PUSH_NULL
+              4754 LOAD_NAME                0 (rules)
+              4756 LOAD_ATTR               19 (add_perm)
+              4766 LOAD_CONST             127 ('core.reset_password_rule')
+              4768 LOAD_NAME               81 (reset_password_predicate)
+              4770 PRECALL                  2
+              4774 CALL                     2
+              4784 POP_TOP
+   
+   358        4786 PUSH_NULL
+              4788 LOAD_NAME               18 (is_site_preference_set)
+              4790 LOAD_CONST             120 ('auth')
+              4792 LOAD_CONST             128 ('invite_enabled')
+              4794 KW_NAMES               122
+              4796 PRECALL                  2
+              4800 CALL                     2
+              4810 STORE_NAME              82 (invite_enabled_predicate)
+   
+   359        4812 PUSH_NULL
+              4814 LOAD_NAME                0 (rules)
+              4816 LOAD_ATTR               19 (add_perm)
+              4826 LOAD_CONST             129 ('core.invite_enabled')
+              4828 LOAD_NAME               82 (invite_enabled_predicate)
+              4830 PRECALL                  2
+              4834 CALL                     2
+              4844 POP_TOP
+   
+   361        4846 LOAD_NAME               12 (has_person)
+              4848 LOAD_NAME               82 (invite_enabled_predicate)
+              4850 BINARY_OP                1 (&)
+              4854 STORE_NAME              83 (accept_invite_predicate)
+   
+   362        4856 PUSH_NULL
+              4858 LOAD_NAME                0 (rules)
+              4860 LOAD_ATTR               19 (add_perm)
+              4870 LOAD_CONST             130 ('core.accept_invite_rule')
+              4872 LOAD_NAME               83 (accept_invite_predicate)
+              4874 PRECALL                  2
+              4878 CALL                     2
+              4888 POP_TOP
    
-   363        4900 PUSH_NULL
-              4902 LOAD_NAME                0 (rules)
-              4904 LOAD_ATTR               19 (add_perm)
-              4914 LOAD_CONST             133 ('core.create_oauthapplication_rule')
-              4916 LOAD_NAME               84 (create_oauthapplication_predicate)
-              4918 PRECALL                  2
-              4922 CALL                     2
-              4932 POP_TOP
-   
-   365        4934 LOAD_NAME               12 (has_person)
-              4936 PUSH_NULL
-              4938 LOAD_NAME               10 (has_global_perm)
-              4940 LOAD_CONST             134 ('core.view_oauthapplication')
-              4942 PRECALL                  1
-              4946 CALL                     1
-              4956 BINARY_OP                1 (&)
-              4960 STORE_NAME              85 (view_oauth_applications_predicate)
-   
-   366        4962 PUSH_NULL
-              4964 LOAD_NAME                0 (rules)
-              4966 LOAD_ATTR               19 (add_perm)
-              4976 LOAD_CONST             135 ('core.view_oauthapplications_rule')
-              4978 LOAD_NAME               85 (view_oauth_applications_predicate)
-              4980 PRECALL                  2
-              4984 CALL                     2
-              4994 POP_TOP
-   
-   368        4996 LOAD_NAME               12 (has_person)
-              4998 PUSH_NULL
-              5000 LOAD_NAME               10 (has_global_perm)
-              5002 LOAD_CONST             134 ('core.view_oauthapplication')
-              5004 PRECALL                  1
-              5008 CALL                     1
-              5018 BINARY_OP                1 (&)
-              5022 STORE_NAME              86 (view_oauth_application_predicate)
-   
-   369        5024 PUSH_NULL
-              5026 LOAD_NAME                0 (rules)
-              5028 LOAD_ATTR               19 (add_perm)
-              5038 LOAD_CONST             136 ('core.view_oauthapplication_rule')
-              5040 LOAD_NAME               86 (view_oauth_application_predicate)
-              5042 PRECALL                  2
-              5046 CALL                     2
-              5056 POP_TOP
-   
-   371        5058 LOAD_NAME               12 (has_person)
-              5060 PUSH_NULL
-              5062 LOAD_NAME               10 (has_global_perm)
-              5064 LOAD_CONST             137 ('core.change_oauthapplication')
-              5066 PRECALL                  1
-              5070 CALL                     1
-              5080 BINARY_OP                1 (&)
-              5084 STORE_NAME              87 (edit_oauth_application_predicate)
-   
-   372        5086 PUSH_NULL
-              5088 LOAD_NAME                0 (rules)
-              5090 LOAD_ATTR               19 (add_perm)
-              5100 LOAD_CONST             138 ('core.edit_oauthapplication_rule')
-              5102 LOAD_NAME               87 (edit_oauth_application_predicate)
-              5104 PRECALL                  2
-              5108 CALL                     2
-              5118 POP_TOP
-   
-   374        5120 LOAD_NAME               12 (has_person)
-              5122 PUSH_NULL
-              5124 LOAD_NAME               10 (has_global_perm)
-              5126 LOAD_CONST             139 ('core.delete_oauth_applications')
-              5128 PRECALL                  1
-              5132 CALL                     1
-              5142 BINARY_OP                1 (&)
-              5146 STORE_NAME              88 (delete_oauth_applications_predicate)
-   
-   375        5148 PUSH_NULL
-              5150 LOAD_NAME                0 (rules)
-              5152 LOAD_ATTR               19 (add_perm)
-              5162 LOAD_CONST             140 ('core.delete_oauth_applications_rule')
-              5164 LOAD_NAME               88 (delete_oauth_applications_predicate)
-              5166 PRECALL                  2
-              5170 CALL                     2
-              5180 POP_TOP
-   
-   377        5182 LOAD_NAME               12 (has_person)
-              5184 LOAD_NAME                1 (is_superuser)
-              5186 BINARY_OP                1 (&)
-              5190 STORE_NAME              89 (view_django_admin_predicate)
-   
-   378        5192 PUSH_NULL
-              5194 LOAD_NAME                0 (rules)
-              5196 LOAD_ATTR               19 (add_perm)
-              5206 LOAD_CONST             141 ('core.view_django_admin_rule')
-              5208 LOAD_NAME               89 (view_django_admin_predicate)
-              5210 PRECALL                  2
-              5214 CALL                     2
-              5224 POP_TOP
-   
-   381        5226 LOAD_NAME               12 (has_person)
-   
-   382        5228 LOAD_NAME               43 (manage_data_predicate)
-   
-   383        5230 LOAD_NAME               65 (view_school_term_predicate)
-   
-   382        5232 BINARY_OP                7 (|)
-   
-   384        5236 LOAD_NAME               48 (impersonate_predicate)
-   
-   382        5238 BINARY_OP                7 (|)
-   
-   385        5242 LOAD_NAME               49 (view_system_status_predicate)
-   
-   382        5244 BINARY_OP                7 (|)
-   
-   386        5248 LOAD_NAME               45 (view_announcements_predicate)
-   
-   382        5250 BINARY_OP                7 (|)
-   
-   387        5254 LOAD_NAME               69 (view_data_check_results_predicate)
-   
-   382        5256 BINARY_OP                7 (|)
-   
-   388        5260 LOAD_NAME               85 (view_oauth_applications_predicate)
-   
-   382        5262 BINARY_OP                7 (|)
-   
-   389        5266 LOAD_NAME               72 (view_dashboard_widget_predicate)
-   
-   382        5268 BINARY_OP                7 (|)
-   
-   390        5272 LOAD_NAME               89 (view_django_admin_predicate)
-   
-   382        5274 BINARY_OP                7 (|)
-   
-   381        5278 BINARY_OP                1 (&)
-              5282 STORE_NAME              90 (view_admin_menu_predicate)
-   
-   392        5284 PUSH_NULL
-              5286 LOAD_NAME                0 (rules)
-              5288 LOAD_ATTR               19 (add_perm)
-              5298 LOAD_CONST             142 ('core.view_admin_menu_rule')
-              5300 LOAD_NAME               90 (view_admin_menu_predicate)
-              5302 PRECALL                  2
-              5306 CALL                     2
-              5316 POP_TOP
-   
-   395        5318 LOAD_NAME               12 (has_person)
-              5320 PUSH_NULL
-              5322 LOAD_NAME               10 (has_global_perm)
-              5324 LOAD_CONST             143 ('core.upload_files_ckeditor')
-              5326 PRECALL                  1
-              5330 CALL                     1
-              5340 BINARY_OP                1 (&)
-              5344 STORE_NAME              91 (upload_files_ckeditor_predicate)
-   
-   396        5346 PUSH_NULL
-              5348 LOAD_NAME                0 (rules)
-              5350 LOAD_ATTR               19 (add_perm)
-              5360 LOAD_CONST             144 ('core.upload_files_ckeditor_rule')
-              5362 LOAD_NAME               91 (upload_files_ckeditor_predicate)
-              5364 PRECALL                  2
-              5368 CALL                     2
-              5378 POP_TOP
-   
-   398        5380 LOAD_NAME               12 (has_person)
-              5382 LOAD_NAME                1 (is_superuser)
-              5384 BINARY_OP                1 (&)
-              5388 STORE_NAME              92 (manage_person_permissions_predicate)
-   
-   399        5390 PUSH_NULL
-              5392 LOAD_NAME                0 (rules)
-              5394 LOAD_ATTR               19 (add_perm)
-              5404 LOAD_CONST             145 ('core.manage_permissions_rule')
-              5406 LOAD_NAME               92 (manage_person_permissions_predicate)
-              5408 PRECALL                  2
-              5412 CALL                     2
-              5422 POP_TOP
-   
-   401        5424 LOAD_NAME               12 (has_person)
-              5426 PUSH_NULL
-              5428 LOAD_NAME               10 (has_global_perm)
-              5430 LOAD_CONST             146 ('core.test_pdf')
-              5432 PRECALL                  1
-              5436 CALL                     1
-              5446 BINARY_OP                1 (&)
-              5450 STORE_NAME              93 (test_pdf_generation_predicate)
-   
-   402        5452 PUSH_NULL
-              5454 LOAD_NAME                0 (rules)
-              5456 LOAD_ATTR               19 (add_perm)
-              5466 LOAD_CONST             147 ('core.test_pdf_rule')
-              5468 LOAD_NAME               93 (test_pdf_generation_predicate)
-              5470 PRECALL                  2
-              5474 CALL                     2
-              5484 POP_TOP
-   
-   404        5486 LOAD_NAME               12 (has_person)
-              5488 LOAD_NAME               17 (is_own_celery_task)
-              5490 BINARY_OP                1 (&)
-              5494 STORE_NAME              94 (view_progress_predicate)
-   
-   405        5496 PUSH_NULL
-              5498 LOAD_NAME                0 (rules)
-              5500 LOAD_ATTR               19 (add_perm)
-              5510 LOAD_CONST             148 ('core.view_progress_rule')
-              5512 LOAD_NAME               94 (view_progress_predicate)
-              5514 PRECALL                  2
-              5518 CALL                     2
-              5528 POP_TOP
-              5530 LOAD_CONST               1 (None)
-              5532 RETURN_VALUE
+   364        4890 LOAD_NAME               12 (has_person)
+              4892 LOAD_NAME               82 (invite_enabled_predicate)
+              4894 BINARY_OP                1 (&)
+              4898 PUSH_NULL
+              4900 LOAD_NAME               10 (has_global_perm)
+              4902 LOAD_CONST             131 ('core.invite')
+              4904 PRECALL                  1
+              4908 CALL                     1
+              4918 BINARY_OP                1 (&)
+              4922 STORE_NAME              84 (invite_predicate)
+   
+   365        4924 PUSH_NULL
+              4926 LOAD_NAME                0 (rules)
+              4928 LOAD_ATTR               19 (add_perm)
+              4938 LOAD_CONST             132 ('core.invite_rule')
+              4940 LOAD_NAME               84 (invite_predicate)
+              4942 PRECALL                  2
+              4946 CALL                     2
+              4956 POP_TOP
+   
+   368        4958 LOAD_NAME               12 (has_person)
+              4960 PUSH_NULL
+              4962 LOAD_NAME               10 (has_global_perm)
+              4964 LOAD_CONST             133 ('core.add_oauthapplication')
+              4966 PRECALL                  1
+              4970 CALL                     1
+              4980 BINARY_OP                1 (&)
+              4984 STORE_NAME              85 (create_oauthapplication_predicate)
+   
+   369        4986 PUSH_NULL
+              4988 LOAD_NAME                0 (rules)
+              4990 LOAD_ATTR               19 (add_perm)
+              5000 LOAD_CONST             134 ('core.create_oauthapplication_rule')
+              5002 LOAD_NAME               85 (create_oauthapplication_predicate)
+              5004 PRECALL                  2
+              5008 CALL                     2
+              5018 POP_TOP
+   
+   371        5020 LOAD_NAME               12 (has_person)
+              5022 PUSH_NULL
+              5024 LOAD_NAME               10 (has_global_perm)
+              5026 LOAD_CONST             135 ('core.view_oauthapplication')
+              5028 PRECALL                  1
+              5032 CALL                     1
+              5042 BINARY_OP                1 (&)
+              5046 STORE_NAME              86 (view_oauth_applications_predicate)
+   
+   372        5048 PUSH_NULL
+              5050 LOAD_NAME                0 (rules)
+              5052 LOAD_ATTR               19 (add_perm)
+              5062 LOAD_CONST             136 ('core.view_oauthapplications_rule')
+              5064 LOAD_NAME               86 (view_oauth_applications_predicate)
+              5066 PRECALL                  2
+              5070 CALL                     2
+              5080 POP_TOP
+   
+   374        5082 LOAD_NAME               12 (has_person)
+              5084 PUSH_NULL
+              5086 LOAD_NAME               10 (has_global_perm)
+              5088 LOAD_CONST             135 ('core.view_oauthapplication')
+              5090 PRECALL                  1
+              5094 CALL                     1
+              5104 BINARY_OP                1 (&)
+              5108 STORE_NAME              87 (view_oauth_application_predicate)
+   
+   375        5110 PUSH_NULL
+              5112 LOAD_NAME                0 (rules)
+              5114 LOAD_ATTR               19 (add_perm)
+              5124 LOAD_CONST             137 ('core.view_oauthapplication_rule')
+              5126 LOAD_NAME               87 (view_oauth_application_predicate)
+              5128 PRECALL                  2
+              5132 CALL                     2
+              5142 POP_TOP
+   
+   377        5144 LOAD_NAME               12 (has_person)
+              5146 PUSH_NULL
+              5148 LOAD_NAME               10 (has_global_perm)
+              5150 LOAD_CONST             138 ('core.change_oauthapplication')
+              5152 PRECALL                  1
+              5156 CALL                     1
+              5166 BINARY_OP                1 (&)
+              5170 STORE_NAME              88 (edit_oauth_application_predicate)
+   
+   378        5172 PUSH_NULL
+              5174 LOAD_NAME                0 (rules)
+              5176 LOAD_ATTR               19 (add_perm)
+              5186 LOAD_CONST             139 ('core.edit_oauthapplication_rule')
+              5188 LOAD_NAME               88 (edit_oauth_application_predicate)
+              5190 PRECALL                  2
+              5194 CALL                     2
+              5204 POP_TOP
+   
+   380        5206 LOAD_NAME               12 (has_person)
+              5208 PUSH_NULL
+              5210 LOAD_NAME               10 (has_global_perm)
+              5212 LOAD_CONST             140 ('core.delete_oauth_applications')
+              5214 PRECALL                  1
+              5218 CALL                     1
+              5228 BINARY_OP                1 (&)
+              5232 STORE_NAME              89 (delete_oauth_applications_predicate)
+   
+   381        5234 PUSH_NULL
+              5236 LOAD_NAME                0 (rules)
+              5238 LOAD_ATTR               19 (add_perm)
+              5248 LOAD_CONST             141 ('core.delete_oauth_applications_rule')
+              5250 LOAD_NAME               89 (delete_oauth_applications_predicate)
+              5252 PRECALL                  2
+              5256 CALL                     2
+              5266 POP_TOP
+   
+   383        5268 LOAD_NAME               12 (has_person)
+              5270 LOAD_NAME                1 (is_superuser)
+              5272 BINARY_OP                1 (&)
+              5276 STORE_NAME              90 (view_django_admin_predicate)
+   
+   384        5278 PUSH_NULL
+              5280 LOAD_NAME                0 (rules)
+              5282 LOAD_ATTR               19 (add_perm)
+              5292 LOAD_CONST             142 ('core.view_django_admin_rule')
+              5294 LOAD_NAME               90 (view_django_admin_predicate)
+              5296 PRECALL                  2
+              5300 CALL                     2
+              5310 POP_TOP
+   
+   387        5312 LOAD_NAME               12 (has_person)
+   
+   388        5314 LOAD_NAME               43 (manage_data_predicate)
+   
+   389        5316 LOAD_NAME               66 (view_school_term_predicate)
+   
+   388        5318 BINARY_OP                7 (|)
+   
+   390        5322 LOAD_NAME               48 (impersonate_predicate)
+   
+   388        5324 BINARY_OP                7 (|)
+   
+   391        5328 LOAD_NAME               49 (view_system_status_predicate)
+   
+   388        5330 BINARY_OP                7 (|)
+   
+   392        5334 LOAD_NAME               45 (view_announcements_predicate)
+   
+   388        5336 BINARY_OP                7 (|)
+   
+   393        5340 LOAD_NAME               70 (view_data_check_results_predicate)
+   
+   388        5342 BINARY_OP                7 (|)
+   
+   394        5346 LOAD_NAME               86 (view_oauth_applications_predicate)
+   
+   388        5348 BINARY_OP                7 (|)
+   
+   395        5352 LOAD_NAME               73 (view_dashboard_widget_predicate)
+   
+   388        5354 BINARY_OP                7 (|)
+   
+   396        5358 LOAD_NAME               90 (view_django_admin_predicate)
+   
+   388        5360 BINARY_OP                7 (|)
+   
+   387        5364 BINARY_OP                1 (&)
+              5368 STORE_NAME              91 (view_admin_menu_predicate)
+   
+   398        5370 PUSH_NULL
+              5372 LOAD_NAME                0 (rules)
+              5374 LOAD_ATTR               19 (add_perm)
+              5384 LOAD_CONST             143 ('core.view_admin_menu_rule')
+              5386 LOAD_NAME               91 (view_admin_menu_predicate)
+              5388 PRECALL                  2
+              5392 CALL                     2
+              5402 POP_TOP
+   
+   401        5404 LOAD_NAME               12 (has_person)
+              5406 PUSH_NULL
+              5408 LOAD_NAME               10 (has_global_perm)
+              5410 LOAD_CONST             144 ('core.upload_files_ckeditor')
+              5412 PRECALL                  1
+              5416 CALL                     1
+              5426 BINARY_OP                1 (&)
+              5430 STORE_NAME              92 (upload_files_ckeditor_predicate)
+   
+   402        5432 PUSH_NULL
+              5434 LOAD_NAME                0 (rules)
+              5436 LOAD_ATTR               19 (add_perm)
+              5446 LOAD_CONST             145 ('core.upload_files_ckeditor_rule')
+              5448 LOAD_NAME               92 (upload_files_ckeditor_predicate)
+              5450 PRECALL                  2
+              5454 CALL                     2
+              5464 POP_TOP
+   
+   404        5466 LOAD_NAME               12 (has_person)
+              5468 LOAD_NAME                1 (is_superuser)
+              5470 BINARY_OP                1 (&)
+              5474 STORE_NAME              93 (manage_person_permissions_predicate)
+   
+   405        5476 PUSH_NULL
+              5478 LOAD_NAME                0 (rules)
+              5480 LOAD_ATTR               19 (add_perm)
+              5490 LOAD_CONST             146 ('core.manage_permissions_rule')
+              5492 LOAD_NAME               93 (manage_person_permissions_predicate)
+              5494 PRECALL                  2
+              5498 CALL                     2
+              5508 POP_TOP
+   
+   407        5510 LOAD_NAME               12 (has_person)
+              5512 PUSH_NULL
+              5514 LOAD_NAME               10 (has_global_perm)
+              5516 LOAD_CONST             147 ('core.test_pdf')
+              5518 PRECALL                  1
+              5522 CALL                     1
+              5532 BINARY_OP                1 (&)
+              5536 STORE_NAME              94 (test_pdf_generation_predicate)
+   
+   408        5538 PUSH_NULL
+              5540 LOAD_NAME                0 (rules)
+              5542 LOAD_ATTR               19 (add_perm)
+              5552 LOAD_CONST             148 ('core.test_pdf_rule')
+              5554 LOAD_NAME               94 (test_pdf_generation_predicate)
+              5556 PRECALL                  2
+              5560 CALL                     2
+              5570 POP_TOP
+   
+   410        5572 LOAD_NAME               12 (has_person)
+              5574 LOAD_NAME               17 (is_own_celery_task)
+              5576 BINARY_OP                1 (&)
+              5580 STORE_NAME              95 (view_progress_predicate)
+   
+   411        5582 PUSH_NULL
+              5584 LOAD_NAME                0 (rules)
+              5586 LOAD_ATTR               19 (add_perm)
+              5596 LOAD_CONST             149 ('core.view_progress_rule')
+              5598 LOAD_NAME               95 (view_progress_predicate)
+              5600 PRECALL                  2
+              5604 CALL                     2
+              5614 POP_TOP
+              5616 LOAD_CONST               1 (None)
+              5618 RETURN_VALUE
    consts
       0
       None
       ('is_superuser',)
       1
       ('AdditionalField', 'Announcement', 'Group', 'GroupType', 'Person')
       ('has_any_object', 'has_global_perm', 'has_object_perm', 'has_person', 'is_anonymous', 'is_current_person', 'is_group_owner', 'is_notification_recipient', 'is_own_celery_task', 'is_site_preference_set')
@@ -1964,17 +1993,17 @@
       'core.view_contact_details_rule'
       'core.view_photo'
       'core.view_photo_rule'
       'core.view_avatar'
       'core.view_avatar_rule'
       'core.view_person_groups'
       'core.view_person_groups_rule'
-      'core.change_person'
       'account'
       'editable_fields_person'
+      'core.change_person'
       'core.edit_person_rule'
       'core.delete_person'
       'core.delete_person_rule'
       'core.view_group'
       'core.view_groups_rule'
       'core.view_group_rule'
       'core.change_group'
@@ -2013,21 +2042,22 @@
       'core.change_additionalfield_rule'
       'core.add_additionalfield'
       'core.create_additionalfield_rule'
       'core.delete_additionalfield'
       'core.delete_additionalfield_rule'
       'core.view_additionalfield'
       'core.view_additionalfields_rule'
+      'core.view_grouptype'
+      'core.view_grouptype_rule'
       'core.change_grouptype'
       'core.edit_grouptype_rule'
       'core.add_grouptype'
       'core.create_grouptype_rule'
       'core.delete_grouptype'
       'core.delete_grouptype_rule'
-      'core.view_grouptype'
       'core.view_grouptypes_rule'
       'core.add_person'
       'core.create_person_rule'
       'core.add_group'
       'core.create_group_rule'
       'core.view_schoolterm'
       'core.view_schoolterm_rule'
@@ -2081,34 +2111,34 @@
       'core.view_admin_menu_rule'
       'core.upload_files_ckeditor'
       'core.upload_files_ckeditor_rule'
       'core.manage_permissions_rule'
       'core.test_pdf'
       'core.test_pdf_rule'
       'core.view_progress_rule'
-   names      ('rules', 'is_superuser', 'models', 'AdditionalField', 'Announcement', 'Group', 'GroupType', 'Person', 'util.predicates', 'has_any_object', 'has_global_perm', 'has_object_perm', 'has_person', 'is_anonymous', 'is_current_person', 'is_group_owner', 'is_notification_recipient', 'is_own_celery_task', 'is_site_preference_set', 'add_perm', 'always_allow', 'login_predicate', 'logout_predicate', 'view_account_predicate', 'manage_2fa_predicate', 'manage_social_connections_predicate', 'manage_authorized_tokens_predicate', 'view_dashboard_predicate', 'search_predicate', 'view_persons_predicate', 'view_person_predicate', 'view_address_predicate', 'view_contact_details_predicate', 'view_photo_predicate', 'view_avatar_predicate', 'view_groups_predicate', 'edit_person_predicate', 'delete_person_predicate', 'view_group_predicate', 'edit_group_predicate', 'delete_group_predicate', 'assign_child_groups_to_groups_predicate', 'edit_school_information_predicate', 'manage_data_predicate', 'mark_notification_as_read_predicate', 'view_announcements_predicate', 'create_or_edit_announcement_predicate', 'delete_announcement_predicate', 'impersonate_predicate', 'view_system_status_predicate', 'view_personal_details_predicate', 'change_site_preferences', 'change_person_preferences', 'change_account_preferences', 'change_group_preferences', 'change_additional_field_predicate', 'create_additional_field_predicate', 'delete_additional_field_predicate', 'view_additional_fields_predicate', 'change_group_type_predicate', 'create_group_type_predicate', 'delete_group_type_predicate', 'view_group_types_predicate', 'create_person_predicate', 'create_group_predicate', 'view_school_term_predicate', 'create_school_term_predicate', 'edit_school_term_predicate', 'view_group_stats_predicate', 'view_data_check_results_predicate', 'run_data_checks_predicate', 'solve_data_problem_predicate', 'view_dashboard_widget_predicate', 'create_dashboard_widget_predicate', 'edit_dashboard_widget_predicate', 'delete_dashboard_widget_predicate', 'edit_dashboard_predicate', 'edit_default_dashboard_predicate', 'signup_predicate', 'change_password_predicate', 'reset_password_predicate', 'invite_enabled_predicate', 'accept_invite_predicate', 'invite_predicate', 'create_oauthapplication_predicate', 'view_oauth_applications_predicate', 'view_oauth_application_predicate', 'edit_oauth_application_predicate', 'delete_oauth_applications_predicate', 'view_django_admin_predicate', 'view_admin_menu_predicate', 'upload_files_ckeditor_predicate', 'manage_person_permissions_predicate', 'test_pdf_generation_predicate', 'view_progress_predicate')
+   names      ('rules', 'is_superuser', 'models', 'AdditionalField', 'Announcement', 'Group', 'GroupType', 'Person', 'util.predicates', 'has_any_object', 'has_global_perm', 'has_object_perm', 'has_person', 'is_anonymous', 'is_current_person', 'is_group_owner', 'is_notification_recipient', 'is_own_celery_task', 'is_site_preference_set', 'add_perm', 'always_allow', 'login_predicate', 'logout_predicate', 'view_account_predicate', 'manage_2fa_predicate', 'manage_social_connections_predicate', 'manage_authorized_tokens_predicate', 'view_dashboard_predicate', 'search_predicate', 'view_persons_predicate', 'view_person_predicate', 'view_address_predicate', 'view_contact_details_predicate', 'view_photo_predicate', 'view_avatar_predicate', 'view_groups_predicate', 'edit_person_predicate', 'delete_person_predicate', 'view_group_predicate', 'edit_group_predicate', 'delete_group_predicate', 'assign_child_groups_to_groups_predicate', 'edit_school_information_predicate', 'manage_data_predicate', 'mark_notification_as_read_predicate', 'view_announcements_predicate', 'create_or_edit_announcement_predicate', 'delete_announcement_predicate', 'impersonate_predicate', 'view_system_status_predicate', 'view_personal_details_predicate', 'change_site_preferences', 'change_person_preferences', 'change_account_preferences', 'change_group_preferences', 'change_additional_field_predicate', 'create_additional_field_predicate', 'delete_additional_field_predicate', 'view_additional_fields_predicate', 'view_group_type_predicate', 'change_group_type_predicate', 'create_group_type_predicate', 'delete_group_type_predicate', 'view_group_types_predicate', 'create_person_predicate', 'create_group_predicate', 'view_school_term_predicate', 'create_school_term_predicate', 'edit_school_term_predicate', 'view_group_stats_predicate', 'view_data_check_results_predicate', 'run_data_checks_predicate', 'solve_data_problem_predicate', 'view_dashboard_widget_predicate', 'create_dashboard_widget_predicate', 'edit_dashboard_widget_predicate', 'delete_dashboard_widget_predicate', 'edit_dashboard_predicate', 'edit_default_dashboard_predicate', 'signup_predicate', 'change_password_predicate', 'reset_password_predicate', 'invite_enabled_predicate', 'accept_invite_predicate', 'invite_predicate', 'create_oauthapplication_predicate', 'view_oauth_applications_predicate', 'view_oauth_application_predicate', 'edit_oauth_application_predicate', 'delete_oauth_applications_predicate', 'view_django_admin_predicate', 'view_admin_menu_predicate', 'upload_files_ckeditor_predicate', 'manage_person_permissions_predicate', 'test_pdf_generation_predicate', 'view_progress_predicate')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/builds/AlekSIS/official/AlekSIS-Core/aleksis/core/rules.py'
    name       '<module>'
    firstlineno 1
    lnotab
       0x00ff020108010c021c01300d2c03040122030601220304012203040122
       0304012203040122031e01220322031c01220302012eff06032203020132
-      ff06032203020132ff060322030201140114ff040202fe04ff0605220302
-      0132ff06032203020132ff060322030201140114ff040202fe04ff060522
-      030201140114ff04021cfe04ff0605220302012cff0603220302012eff06
+      ff06032203020132ff060322030201020114ff040214fe04ff0605220302
+      0132ff06032203020132ff060322030201020114ff040214fe04ff060522
+      0302011c0114ff040214fe04ff0605220302012cff0603220302012eff06
       03220302012cff0603220302012cff0603220302012cff06032203060102
       ff140322031c0122031c0122030a0122030201140116ff04ff0604220302
       0114012cff04ff0604220302012cff060322031c0122031c0122030e0102
-      0102010eff04fe10070201140114ff040202fe04ff060522030201140114
-      ff04ff060422030201140114ff040202fe04ff0605220304012203020114
+      0102010eff04fe10070201020114ff040214fe04ff060522030201140114
+      ff04ff060422030201020114ff040214fe04ff0605220304012203020114
       0114ff040202fe04ff0605220402012cff0603220302012cff0603220402
       012cff060322030201140116ff04ff0604220302012cff0603220302012c
-      ff0603220402012cff0603220302012eff0603220302012cff0603220302
-      012cff060322031c0122021c0122021c01220302012cff060322031c0122
-      0420ff0203220420ff020322021c0122021c0122021c0122021c0122021e
-      0122021c0122031a0122021a0122021a0122031a0122020a012202220122
-      031c0122021c0122021c0122021c0122021c0122020a0122030201020102
-      ff040202fe040302fd040402fc040502fb040602fa040702f9040802f804
-      ff060b22031c0122020a0122021c0122020a01
+      ff0603220302012cff0603220402012cff0603220302012eff0603220302
+      012cff0603220302012cff060322031c0122021c0122021c01220302012c
+      ff060322031c01220420ff0203220420ff020322021c0122021c0122021c
+      0122021c0122021e0122021c0122031a0122021a0122021a0122031a0122
+      020a012202220122031c0122021c0122021c0122021c0122021c0122020a
+      0122030201020102ff040202fe040302fd040402fc040502fb040602fa04
+      0702f9040802f804ff060b22031c0122020a0122021c0122020a01
```

### Comparing `aleksis_core-3.0b2/aleksis/core/__pycache__/settings.cpython-311.pyc` & `aleksis_core-3.0b3/aleksis/core/__pycache__/settings.cpython-311.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x794f0a64 (Thu Mar  9 21:28:25 2023 UTC)
+moddate:  0x6f611764 (Sun Mar 19 19:24:31 2023 UTC)
 files sz: 39383
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 18
    flags     : 0
    code
```

### Comparing `aleksis_core-3.0b2/aleksis/core/__pycache__/tasks.cpython-311.pyc` & `aleksis_core-3.0b3/aleksis/core/__pycache__/tasks.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x794f0a64 (Thu Mar  9 21:28:25 2023 UTC)
+moddate:  0x6f611764 (Sun Mar 19 19:24:31 2023 UTC)
 files sz: 2330
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 8
    flags     : 0
    code
```

### Comparing `aleksis_core-3.0b2/aleksis/core/admin.py` & `aleksis_core-3.0b3/aleksis/core/admin.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/apps.py` & `aleksis_core-3.0b3/aleksis/core/apps.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/celery.py` & `aleksis_core-3.0b3/aleksis/core/celery.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/checks.py` & `aleksis_core-3.0b3/aleksis/core/checks.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/data_checks.py` & `aleksis_core-3.0b3/aleksis/core/data_checks.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/decorators.py` & `aleksis_core-3.0b3/aleksis/core/decorators.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/filters.py` & `aleksis_core-3.0b3/aleksis/core/filters.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/forms.py` & `aleksis_core-3.0b3/aleksis/core/forms.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/frontend/app/apollo.js` & `aleksis_core-3.0b3/aleksis/core/frontend/app/apollo.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/frontend/app/dateTimeFormats.js` & `aleksis_core-3.0b3/aleksis/core/frontend/app/dateTimeFormats.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/frontend/app/vuetify.js` & `aleksis_core-3.0b3/aleksis/core/frontend/app/vuetify.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/frontend/components/LegacyBaseTemplate.vue` & `aleksis_core-3.0b3/aleksis/core/frontend/components/LegacyBaseTemplate.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/frontend/components/about/AboutAleksis.vue` & `aleksis_core-3.0b3/aleksis/core/frontend/components/about/AboutAleksis.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/frontend/components/about/InstalledAppCard.vue` & `aleksis_core-3.0b3/aleksis/core/frontend/components/about/InstalledAppCard.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/frontend/components/about/InstalledAppsList.vue` & `aleksis_core-3.0b3/aleksis/core/frontend/components/about/InstalledAppsList.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/frontend/components/app/AccountMenu.vue` & `aleksis_core-3.0b3/aleksis/core/frontend/components/app/AccountMenu.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/frontend/components/app/App.vue` & `aleksis_core-3.0b3/aleksis/core/frontend/components/app/App.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/frontend/components/app/ErrorPage.vue` & `aleksis_core-3.0b3/aleksis/core/frontend/components/app/ErrorPage.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/frontend/components/app/LanguageForm.vue` & `aleksis_core-3.0b3/aleksis/core/frontend/components/app/LanguageForm.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/frontend/components/app/SideNav.vue` & `aleksis_core-3.0b3/aleksis/core/frontend/components/app/SideNav.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/frontend/components/app/SidenavSearch.vue` & `aleksis_core-3.0b3/aleksis/core/frontend/components/app/SidenavSearch.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/frontend/components/app/SnackbarItem.vue` & `aleksis_core-3.0b3/aleksis/core/frontend/components/app/SnackbarItem.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/frontend/components/app/Splash.vue` & `aleksis_core-3.0b3/aleksis/core/frontend/components/app/Splash.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/frontend/components/celery_progress/CeleryProgress.vue` & `aleksis_core-3.0b3/aleksis/core/frontend/components/celery_progress/CeleryProgress.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/frontend/components/celery_progress/CeleryProgressBottom.vue` & `aleksis_core-3.0b3/aleksis/core/frontend/components/celery_progress/CeleryProgressBottom.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/frontend/components/celery_progress/TaskListItem.vue` & `aleksis_core-3.0b3/aleksis/core/frontend/components/celery_progress/TaskListItem.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/frontend/components/generic/AvatarClickbox.vue` & `aleksis_core-3.0b3/aleksis/core/frontend/components/generic/AvatarClickbox.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/frontend/components/generic/ButtonMenu.vue` & `aleksis_core-3.0b3/aleksis/core/frontend/components/generic/ButtonMenu.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/frontend/components/generic/DetailView.vue` & `aleksis_core-3.0b3/aleksis/core/frontend/components/generic/DetailView.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/frontend/components/generic/ObjectOverview.vue` & `aleksis_core-3.0b3/aleksis/core/frontend/components/generic/ObjectOverview.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/frontend/components/group/GroupCollection.vue` & `aleksis_core-3.0b3/aleksis/core/frontend/components/group/GroupCollection.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/frontend/components/notifications/NotificationItem.vue` & `aleksis_core-3.0b3/aleksis/core/frontend/components/notifications/NotificationItem.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/frontend/components/notifications/NotificationList.vue` & `aleksis_core-3.0b3/aleksis/core/frontend/components/notifications/NotificationList.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/frontend/components/pdf/DownloadPDF.vue` & `aleksis_core-3.0b3/aleksis/core/frontend/components/pdf/DownloadPDF.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/frontend/components/person/AdditionalImage.vue` & `aleksis_core-3.0b3/aleksis/core/frontend/components/person/AdditionalImage.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/frontend/components/person/AvatarContent.vue` & `aleksis_core-3.0b3/aleksis/core/frontend/components/person/AvatarContent.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/frontend/components/person/PersonActions.vue` & `aleksis_core-3.0b3/aleksis/core/frontend/components/person/PersonActions.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/frontend/components/person/PersonAvatarClickbox.vue` & `aleksis_core-3.0b3/aleksis/core/frontend/components/person/PersonAvatarClickbox.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/frontend/components/person/PersonCollection.vue` & `aleksis_core-3.0b3/aleksis/core/frontend/components/person/PersonCollection.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/frontend/components/person/PersonOverview.vue` & `aleksis_core-3.0b3/aleksis/core/frontend/components/person/PersonOverview.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/frontend/components/person/personOverview.graphql` & `aleksis_core-3.0b3/aleksis/core/frontend/components/person/personOverview.graphql`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/frontend/components/two_factor/TwoFactor.vue` & `aleksis_core-3.0b3/aleksis/core/frontend/components/two_factor/TwoFactor.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/frontend/components/two_factor/TwoFactorDevice.vue` & `aleksis_core-3.0b3/aleksis/core/frontend/components/two_factor/TwoFactorDevice.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/frontend/components/two_factor/TwoFactorDeviceBase.vue` & `aleksis_core-3.0b3/aleksis/core/frontend/components/two_factor/TwoFactorDeviceBase.vue`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/frontend/index.js` & `aleksis_core-3.0b3/aleksis/core/frontend/index.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/frontend/messages/de.json` & `aleksis_core-3.0b3/aleksis/core/frontend/messages/de.json`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/frontend/messages/en.json` & `aleksis_core-3.0b3/aleksis/core/frontend/messages/en.json`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/frontend/messages/uk.json` & `aleksis_core-3.0b3/aleksis/core/frontend/messages/uk.json`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/frontend/mixins/aleksis.js` & `aleksis_core-3.0b3/aleksis/core/frontend/mixins/aleksis.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/frontend/mixins/menus.js` & `aleksis_core-3.0b3/aleksis/core/frontend/mixins/menus.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/frontend/mixins/offline.js` & `aleksis_core-3.0b3/aleksis/core/frontend/mixins/offline.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/frontend/mixins/routes.js` & `aleksis_core-3.0b3/aleksis/core/frontend/mixins/routes.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/frontend/mixins/useRegisterSW.js` & `aleksis_core-3.0b3/aleksis/core/frontend/mixins/useRegisterSW.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/frontend/plugins/aleksis.js` & `aleksis_core-3.0b3/aleksis/core/frontend/plugins/aleksis.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/frontend/routes.js` & `aleksis_core-3.0b3/aleksis/core/frontend/routes.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/health_checks.py` & `aleksis_core-3.0b3/aleksis/core/health_checks.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/locale/ar/LC_MESSAGES/django.po` & `aleksis_core-3.0b3/aleksis/core/locale/ar/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/locale/ar/LC_MESSAGES/djangojs.po` & `aleksis_core-3.0b3/aleksis/core/locale/ar/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/locale/de_DE/LC_MESSAGES/django.mo` & `aleksis_core-3.0b3/aleksis/core/locale/de_DE/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/locale/de_DE/LC_MESSAGES/django.po` & `aleksis_core-3.0b3/aleksis/core/locale/de_DE/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/locale/de_DE/LC_MESSAGES/djangojs.mo` & `aleksis_core-3.0b3/aleksis/core/locale/de_DE/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/locale/de_DE/LC_MESSAGES/djangojs.po` & `aleksis_core-3.0b3/aleksis/core/locale/de_DE/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/locale/fr/LC_MESSAGES/django.mo` & `aleksis_core-3.0b3/aleksis/core/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/locale/fr/LC_MESSAGES/django.po` & `aleksis_core-3.0b3/aleksis/core/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/locale/fr/LC_MESSAGES/djangojs.po` & `aleksis_core-3.0b3/aleksis/core/locale/fr/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/locale/la/LC_MESSAGES/django.mo` & `aleksis_core-3.0b3/aleksis/core/locale/la/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/locale/la/LC_MESSAGES/django.po` & `aleksis_core-3.0b3/aleksis/core/locale/la/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/locale/la/LC_MESSAGES/djangojs.po` & `aleksis_core-3.0b3/aleksis/core/locale/la/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/locale/nb_NO/LC_MESSAGES/django.po` & `aleksis_core-3.0b3/aleksis/core/locale/nb_NO/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/locale/nb_NO/LC_MESSAGES/djangojs.po` & `aleksis_core-3.0b3/aleksis/core/locale/nb_NO/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/locale/ru/LC_MESSAGES/django.mo` & `aleksis_core-3.0b3/aleksis/core/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/locale/ru/LC_MESSAGES/django.po` & `aleksis_core-3.0b3/aleksis/core/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/locale/ru/LC_MESSAGES/djangojs.mo` & `aleksis_core-3.0b3/aleksis/core/locale/ru/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/locale/ru/LC_MESSAGES/djangojs.po` & `aleksis_core-3.0b3/aleksis/core/locale/ru/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/locale/tr_TR/LC_MESSAGES/django.po` & `aleksis_core-3.0b3/aleksis/core/locale/tr_TR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/locale/tr_TR/LC_MESSAGES/djangojs.po` & `aleksis_core-3.0b3/aleksis/core/locale/tr_TR/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/locale/uk/LC_MESSAGES/django.mo` & `aleksis_core-3.0b3/aleksis/core/locale/uk/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/locale/uk/LC_MESSAGES/django.po` & `aleksis_core-3.0b3/aleksis/core/locale/uk/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/locale/uk/LC_MESSAGES/djangojs.mo` & `aleksis_core-3.0b3/aleksis/core/locale/uk/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/locale/uk/LC_MESSAGES/djangojs.po` & `aleksis_core-3.0b3/aleksis/core/locale/uk/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/management/commands/convert_urls_to_routes.py` & `aleksis_core-3.0b3/aleksis/core/management/commands/convert_urls_to_routes.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/management/commands/vite.py` & `aleksis_core-3.0b3/aleksis/core/management/commands/vite.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/managers.py` & `aleksis_core-3.0b3/aleksis/core/managers.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/migrations/0001_initial.py` & `aleksis_core-3.0b3/aleksis/core/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/migrations/0002_school_term.py` & `aleksis_core-3.0b3/aleksis/core/migrations/0002_school_term.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/migrations/0003_drop_image_cropping.py` & `aleksis_core-3.0b3/aleksis/core/migrations/0003_drop_image_cropping.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/migrations/0004_add_permissions_for_group_stats.py` & `aleksis_core-3.0b3/aleksis/core/migrations/0004_add_permissions_for_group_stats.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/migrations/0005_timestamped_activity_notification.py` & `aleksis_core-3.0b3/aleksis/core/migrations/0005_timestamped_activity_notification.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/migrations/0006_dashboard_widget_size.py` & `aleksis_core-3.0b3/aleksis/core/migrations/0006_dashboard_widget_size.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/migrations/0007_dashboard_widget_order.py` & `aleksis_core-3.0b3/aleksis/core/migrations/0007_dashboard_widget_order.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/migrations/0008_data_check_result.py` & `aleksis_core-3.0b3/aleksis/core/migrations/0008_data_check_result.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/migrations/0009_default_dashboard.py` & `aleksis_core-3.0b3/aleksis/core/migrations/0009_default_dashboard.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/migrations/0010_external_link_widget.py` & `aleksis_core-3.0b3/aleksis/core/migrations/0010_external_link_widget.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/migrations/0011_globalpermissions_options.py` & `aleksis_core-3.0b3/aleksis/core/migrations/0011_globalpermissions_options.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/migrations/0013_pdf_file.py` & `aleksis_core-3.0b3/aleksis/core/migrations/0013_pdf_file.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/migrations/0014_alter_pdffile_file.py` & `aleksis_core-3.0b3/aleksis/core/migrations/0014_alter_pdffile_file.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/migrations/0015_oauth_permissions.py` & `aleksis_core-3.0b3/aleksis/core/migrations/0015_oauth_permissions.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/migrations/0016_taskuserassignment.py` & `aleksis_core-3.0b3/aleksis/core/migrations/0016_taskuserassignment.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/migrations/0018_pdffile_html_file.py` & `aleksis_core-3.0b3/aleksis/core/migrations/0018_pdffile_html_file.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/migrations/0019_fix_uniqueness_per_site.py` & `aleksis_core-3.0b3/aleksis/core/migrations/0019_fix_uniqueness_per_site.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/migrations/0020_pdf_file_person_optional.py` & `aleksis_core-3.0b3/aleksis/core/migrations/0020_pdf_file_person_optional.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/migrations/0021_drop_persons_accounts_perm.py` & `aleksis_core-3.0b3/aleksis/core/migrations/0021_drop_persons_accounts_perm.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/migrations/0022_public_favicon.py` & `aleksis_core-3.0b3/aleksis/core/migrations/0022_public_favicon.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/migrations/0023_oauth_application_model.py` & `aleksis_core-3.0b3/aleksis/core/migrations/0023_oauth_application_model.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/migrations/0024_oauth_grant_types_optional.py` & `aleksis_core-3.0b3/aleksis/core/migrations/0024_oauth_grant_types_optional.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/migrations/0025_oauth_align_user_fk.py` & `aleksis_core-3.0b3/aleksis/core/migrations/0025_oauth_align_user_fk.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/migrations/0026_oauthapplication_allowed_scopes.py` & `aleksis_core-3.0b3/aleksis/core/migrations/0026_oauthapplication_allowed_scopes.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/migrations/0028_char_field_not_null.py` & `aleksis_core-3.0b3/aleksis/core/migrations/0028_char_field_not_null.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/migrations/0029_invitations.py` & `aleksis_core-3.0b3/aleksis/core/migrations/0029_invitations.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/migrations/0030_user_attributes.py` & `aleksis_core-3.0b3/aleksis/core/migrations/0030_user_attributes.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/migrations/0031_oauthapplication_icon.py` & `aleksis_core-3.0b3/aleksis/core/migrations/0031_oauthapplication_icon.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/migrations/0033_update_photo_avatar.py` & `aleksis_core-3.0b3/aleksis/core/migrations/0033_update_photo_avatar.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/migrations/0034_invite_permission.py` & `aleksis_core-3.0b3/aleksis/core/migrations/0034_invite_permission.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/migrations/0035_preference_model_unique.py` & `aleksis_core-3.0b3/aleksis/core/migrations/0035_preference_model_unique.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/migrations/0036_additionalfields_helptext_required.py` & `aleksis_core-3.0b3/aleksis/core/migrations/0036_additionalfields_helptext_required.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/migrations/0037_add_static_content_widget.py` & `aleksis_core-3.0b3/aleksis/core/migrations/0037_add_static_content_widget.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/migrations/0038_notification_send_at.py` & `aleksis_core-3.0b3/aleksis/core/migrations/0038_notification_send_at.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/migrations/0039_personal_ical_url.py` & `aleksis_core-3.0b3/aleksis/core/migrations/0039_personal_ical_url.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/migrations/0040_oauth_allowed_scopes_max_length_255.py` & `aleksis_core-3.0b3/aleksis/core/migrations/0040_oauth_allowed_scopes_max_length_255.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/migrations/0041_update_gender_choices.py` & `aleksis_core-3.0b3/aleksis/core/migrations/0041_update_gender_choices.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/migrations/0042_pdffile_empty.py` & `aleksis_core-3.0b3/aleksis/core/migrations/0042_pdffile_empty.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/migrations/0043_task_assignment_meta.py` & `aleksis_core-3.0b3/aleksis/core/migrations/0043_task_assignment_meta.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/migrations/0044_task_assignment_result_fetched.py` & `aleksis_core-3.0b3/aleksis/core/migrations/0044_task_assignment_result_fetched.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/migrations/0046_notification_create_field_icon.py` & `aleksis_core-3.0b3/aleksis/core/migrations/0046_notification_create_field_icon.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/migrations/0047_add_room_model.py` & `aleksis_core-3.0b3/aleksis/core/migrations/0047_add_room_model.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/migrations/0048_delete_personalicalurl.py` & `aleksis_core-3.0b3/aleksis/core/migrations/0048_delete_personalicalurl.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/mixins.py` & `aleksis_core-3.0b3/aleksis/core/mixins.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/models.py` & `aleksis_core-3.0b3/aleksis/core/models.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/preferences.py` & `aleksis_core-3.0b3/aleksis/core/preferences.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/registries.py` & `aleksis_core-3.0b3/aleksis/core/registries.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/rules.py` & `aleksis_core-3.0b3/aleksis/core/rules.py`

 * *Files 4% similar despite different names*

```diff
@@ -56,57 +56,57 @@
 view_persons_predicate = has_person & (
     has_global_perm("core.view_person") | has_any_object("core.view_person", Person)
 )
 rules.add_perm("core.view_persons_rule", view_persons_predicate)
 
 # View person
 view_person_predicate = has_person & (
-    has_global_perm("core.view_person") | has_object_perm("core.view_person") | is_current_person
+    is_current_person | has_global_perm("core.view_person") | has_object_perm("core.view_person")
 )
 rules.add_perm("core.view_person_rule", view_person_predicate)
 
 # View person address
 view_address_predicate = has_person & (
-    has_global_perm("core.view_address") | has_object_perm("core.view_address") | is_current_person
+    is_current_person | has_global_perm("core.view_address") | has_object_perm("core.view_address")
 )
 rules.add_perm("core.view_address_rule", view_address_predicate)
 
 # View person contact details
 view_contact_details_predicate = has_person & (
-    has_global_perm("core.view_contact_details")
+    is_current_person
+    | has_global_perm("core.view_contact_details")
     | has_object_perm("core.view_contact_details")
-    | is_current_person
 )
 rules.add_perm("core.view_contact_details_rule", view_contact_details_predicate)
 
 # View person photo
 view_photo_predicate = has_person & (
-    has_global_perm("core.view_photo") | has_object_perm("core.view_photo") | is_current_person
+    is_current_person | has_global_perm("core.view_photo") | has_object_perm("core.view_photo")
 )
 rules.add_perm("core.view_photo_rule", view_photo_predicate)
 
 # View person avatar image
 view_avatar_predicate = has_person & (
-    has_global_perm("core.view_avatar") | has_object_perm("core.view_avatar") | is_current_person
+    is_current_person | has_global_perm("core.view_avatar") | has_object_perm("core.view_avatar")
 )
 rules.add_perm("core.view_avatar_rule", view_avatar_predicate)
 
 # View persons groups
 view_groups_predicate = has_person & (
-    has_global_perm("core.view_person_groups")
+    is_current_person
+    | has_global_perm("core.view_person_groups")
     | has_object_perm("core.view_person_groups")
-    | is_current_person
 )
 rules.add_perm("core.view_person_groups_rule", view_groups_predicate)
 
 # Edit person
 edit_person_predicate = has_person & (
-    has_global_perm("core.change_person")
+    is_current_person & is_site_preference_set("account", "editable_fields_person")
+    | has_global_perm("core.change_person")
     | has_object_perm("core.change_person")
-    | is_current_person & is_site_preference_set("account", "editable_fields_person")
 )
 rules.add_perm("core.edit_person_rule", edit_person_predicate)
 
 # Delete person
 delete_person_predicate = has_person & (
     has_global_perm("core.delete_person") | has_object_perm("core.delete_person")
 )
@@ -187,32 +187,32 @@
     "core.view_people_menu_rule",
     has_person
     & (view_persons_predicate | view_groups_predicate | assign_child_groups_to_groups_predicate),
 )
 
 # View person personal details
 view_personal_details_predicate = has_person & (
-    has_global_perm("core.view_personal_details")
+    is_current_person
+    | has_global_perm("core.view_personal_details")
     | has_object_perm("core.view_personal_details")
-    | is_current_person
 )
 rules.add_perm("core.view_personal_details_rule", view_personal_details_predicate)
 
 # Change site preferences
 change_site_preferences = has_person & (
     has_global_perm("core.change_site_preferences")
     | has_object_perm("core.change_site_preferences")
 )
 rules.add_perm("core.change_site_preferences_rule", change_site_preferences)
 
 # Change person preferences
 change_person_preferences = has_person & (
-    has_global_perm("core.change_person_preferences")
+    is_current_person
+    | has_global_perm("core.change_person_preferences")
     | has_object_perm("core.change_person_preferences")
-    | is_current_person
 )
 rules.add_perm("core.change_person_preferences_rule", change_person_preferences)
 
 # Change account preferences
 change_account_preferences = has_person
 rules.add_perm("core.change_account_preferences_rule", change_account_preferences)
 
@@ -247,14 +247,20 @@
 # View additional fields
 view_additional_fields_predicate = has_person & (
     has_global_perm("core.view_additionalfield")
     | has_any_object("core.view_additionalfield", AdditionalField)
 )
 rules.add_perm("core.view_additionalfields_rule", view_additional_fields_predicate)
 
+# View group type
+view_group_type_predicate = has_person & (
+    has_global_perm("core.view_grouptype") | has_object_perm("core.view_grouptype")
+)
+rules.add_perm("core.view_grouptype_rule", view_group_type_predicate)
+
 # Edit group type
 change_group_type_predicate = has_person & (
     has_global_perm("core.change_grouptype") | has_object_perm("core.change_grouptype")
 )
 rules.add_perm("core.edit_grouptype_rule", change_group_type_predicate)
 
 # Create group type
```

### Comparing `aleksis_core-3.0b2/aleksis/core/schema/__init__.py` & `aleksis_core-3.0b3/aleksis/core/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/schema/base.py` & `aleksis_core-3.0b3/aleksis/core/schema/base.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/schema/celery_progress.py` & `aleksis_core-3.0b3/aleksis/core/schema/celery_progress.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/schema/custom_menu.py` & `aleksis_core-3.0b3/aleksis/core/schema/custom_menu.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/schema/installed_apps.py` & `aleksis_core-3.0b3/aleksis/core/schema/installed_apps.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/schema/person.py` & `aleksis_core-3.0b3/aleksis/core/schema/person.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,32 +2,58 @@
 
 from django.core.exceptions import PermissionDenied
 from django.utils import timezone
 
 import graphene
 from graphene_django import DjangoObjectType
 from graphene_django.forms.mutation import DjangoModelFormMutation
+from guardian.shortcuts import get_objects_for_user
 
 from ..forms import PersonForm
 from ..models import DummyPerson, Person
-from ..util.core_helpers import get_site_preferences, is_impersonate
+from ..util.core_helpers import get_site_preferences, has_person, is_impersonate
 from .base import FieldFileType
 from .notification import NotificationType
 
 
 class PersonPreferencesType(graphene.ObjectType):
     theme_design_mode = graphene.String()
 
     def resolve_theme_design_mode(parent, info, **kwargs):
         return parent["theme__design"]
 
 
 class PersonType(DjangoObjectType):
     class Meta:
         model = Person
+        fields = [
+            "user",
+            "first_name",
+            "last_name",
+            "additional_name",
+            "short_name",
+            "street",
+            "housenumber",
+            "postal_code",
+            "place",
+            "phone_number",
+            "mobile_number",
+            "email",
+            "date_of_birth",
+            "place_of_birth",
+            "sex",
+            "photo",
+            "avatar",
+            "guardians",
+            "primary_group",
+            "description",
+            "children",
+            "owner_of",
+            "member_of",
+        ]
 
     full_name = graphene.String()
     username = graphene.String()
     userid = graphene.ID()
     photo = graphene.Field(FieldFileType)
     avatar = graphene.Field(FieldFileType)
     avatar_url = graphene.String()
@@ -90,32 +116,37 @@
     def resolve_place_of_birth(root, info, **kwargs):  # noqa
         if info.context.user.has_perm("core.view_personal_details_rule", root):
             return root.place_of_birth
         return None
 
     def resolve_children(root, info, **kwargs):  # noqa
         if info.context.user.has_perm("core.view_personal_details_rule", root):
-            return root.children.all()
+            return get_objects_for_user(info.context.user, "core.view_person", root.children.all())
         return []
 
     def resolve_guardians(root, info, **kwargs):  # noqa
         if info.context.user.has_perm("core.view_personal_details_rule", root):
-            return root.guardians.all()
+            return get_objects_for_user(info.context.user, "core.view_person", root.guardians.all())
         return []
 
     def resolve_member_of(root, info, **kwargs):  # noqa
         if info.context.user.has_perm("core.view_person_groups_rule", root):
-            return root.member_of.all()
+            return get_objects_for_user(info.context.user, "core.view_group", root.member_of.all())
         return []
 
     def resolve_owner_of(root, info, **kwargs):  # noqa
         if info.context.user.has_perm("core.view_person_groups_rule", root):
-            return root.owner_of.all()
+            return get_objects_for_user(info.context.user, "core.view_group", root.owner_of.all())
         return []
 
+    def resolve_primary_group(root, info, **kwargs):  # noqa
+        if info.context.user.has_perm("core.view_group_rule", root.primary_group):
+            return root.primary_group
+        raise PermissionDenied()
+
     def resolve_username(root, info, **kwargs):  # noqa
         return root.user.username if root.user else None
 
     def resolve_userid(root, info, **kwargs):  # noqa
         return root.user.id if root.user else None
 
     def resolve_unread_notifications_count(root, info, **kwargs):  # noqa
@@ -167,15 +198,19 @@
     def resolve_is_dummy(root: Union[Person, DummyPerson], info, **kwargs):
         return root.is_dummy if hasattr(root, "is_dummy") else False
 
     def resolve_is_impersonate(root: Person, info, **kwargs):
         return is_impersonate(info.context)
 
     def resolve_notifications(root: Person, info, **kwargs):
-        return root.notifications.filter(send_at__lte=timezone.now()).order_by("read", "-created")
+        if has_person(info.context.user) and info.context.user.person == root:
+            return root.notifications.filter(send_at__lte=timezone.now()).order_by(
+                "read", "-created"
+            )
+        raise PermissionDenied()
 
     def resolve_can_edit_person(root, info, **kwargs):  # noqa
         return info.context.user.has_perm("core.edit_person_rule", root)
 
     def resolve_can_delete_person(root, info, **kwargs):  # noqa
         return info.context.user.has_perm("core.delete_person_rule", root)
```

### Comparing `aleksis_core-3.0b2/aleksis/core/schema/search.py` & `aleksis_core-3.0b3/aleksis/core/schema/search.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/schema/site_preferences.py` & `aleksis_core-3.0b3/aleksis/core/schema/site_preferences.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/schema/system_properties.py` & `aleksis_core-3.0b3/aleksis/core/schema/system_properties.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/schema/two_factor.py` & `aleksis_core-3.0b3/aleksis/core/schema/two_factor.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/schema/user.py` & `aleksis_core-3.0b3/aleksis/core/schema/user.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/settings.py` & `aleksis_core-3.0b3/aleksis/core/settings.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/static/img/aleksis-banner.svg` & `aleksis_core-3.0b3/aleksis/core/static/img/aleksis-banner.svg`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/static/img/aleksis-favicon.png` & `aleksis_core-3.0b3/aleksis/core/static/img/aleksis-favicon.png`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/static/img/aleksis-icon-maskable.png` & `aleksis_core-3.0b3/aleksis/core/static/img/aleksis-icon-maskable.png`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/static/img/aleksis-icon-maskable.svg` & `aleksis_core-3.0b3/aleksis/core/static/img/aleksis-icon-maskable.svg`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/static/img/aleksis-icon.png` & `aleksis_core-3.0b3/aleksis/core/static/img/aleksis-icon.png`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/static/img/aleksis-icon.svg` & `aleksis_core-3.0b3/aleksis/core/static/img/aleksis-icon.svg`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/static/img/fallback.png` & `aleksis_core-3.0b3/aleksis/core/static/img/fallback.png`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/static/img/hero.svg` & `aleksis_core-3.0b3/aleksis/core/static/img/hero.svg`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/static/js/edit_dashboard.js` & `aleksis_core-3.0b3/aleksis/core/static/js/edit_dashboard.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/static/js/helper.js` & `aleksis_core-3.0b3/aleksis/core/static/js/helper.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/static/js/include_ajax_live.js` & `aleksis_core-3.0b3/aleksis/core/static/js/include_ajax_live.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/static/js/main.js` & `aleksis_core-3.0b3/aleksis/core/static/js/main.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/static/js/multi_select.js` & `aleksis_core-3.0b3/aleksis/core/static/js/multi_select.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/static/js/search.js` & `aleksis_core-3.0b3/aleksis/core/static/js/search.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/static/js/serviceworker.js` & `aleksis_core-3.0b3/aleksis/core/static/js/serviceworker.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/static/print.css` & `aleksis_core-3.0b3/aleksis/core/static/print.css`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/static/public/materialize-custom.scss` & `aleksis_core-3.0b3/aleksis/core/static/public/materialize-custom.scss`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/static/public/style.scss` & `aleksis_core-3.0b3/aleksis/core/static/public/style.scss`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/static/public/theme.scss` & `aleksis_core-3.0b3/aleksis/core/static/public/theme.scss`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/tables.py` & `aleksis_core-3.0b3/aleksis/core/tables.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/tasks.py` & `aleksis_core-3.0b3/aleksis/core/tasks.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/templates/403.html` & `aleksis_core-3.0b3/aleksis/core/templates/403.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/templates/404.html` & `aleksis_core-3.0b3/aleksis/core/templates/404.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/templates/500.html` & `aleksis_core-3.0b3/aleksis/core/templates/500.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/templates/account/account_inactive.html` & `aleksis_core-3.0b3/aleksis/core/templates/account/account_inactive.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/templates/account/email_confirm.html` & `aleksis_core-3.0b3/aleksis/core/templates/account/email_confirm.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/templates/account/password_change.html` & `aleksis_core-3.0b3/aleksis/core/templates/account/password_change.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/templates/account/password_change_disabled.html` & `aleksis_core-3.0b3/aleksis/core/templates/account/password_change_disabled.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/templates/account/password_reset.html` & `aleksis_core-3.0b3/aleksis/core/templates/account/password_reset.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/templates/account/password_reset_done.html` & `aleksis_core-3.0b3/aleksis/core/templates/account/password_reset_done.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/templates/account/password_reset_from_key.html` & `aleksis_core-3.0b3/aleksis/core/templates/account/password_reset_from_key.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/templates/account/password_reset_from_key_done.html` & `aleksis_core-3.0b3/aleksis/core/templates/account/password_reset_from_key_done.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/templates/account/signup.html` & `aleksis_core-3.0b3/aleksis/core/templates/account/signup.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/templates/account/signup_closed.html` & `aleksis_core-3.0b3/aleksis/core/templates/account/signup_closed.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/templates/account/verification_email_required.html` & `aleksis_core-3.0b3/aleksis/core/templates/account/verification_email_required.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/templates/account/verification_sent.html` & `aleksis_core-3.0b3/aleksis/core/templates/account/verification_sent.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/templates/components/chips.html` & `aleksis_core-3.0b3/aleksis/core/templates/components/chips.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/templates/components/pagination.html` & `aleksis_core-3.0b3/aleksis/core/templates/components/pagination.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/templates/core/additional_field/list.html` & `aleksis_core-3.0b3/aleksis/core/templates/core/additional_field/list.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/templates/core/announcement/form.html` & `aleksis_core-3.0b3/aleksis/core/templates/core/announcement/form.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/templates/core/announcement/list.html` & `aleksis_core-3.0b3/aleksis/core/templates/core/announcement/list.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/templates/core/base.html` & `aleksis_core-3.0b3/aleksis/core/templates/core/base.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/templates/core/base_print.html` & `aleksis_core-3.0b3/aleksis/core/templates/core/base_print.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/templates/core/base_simple_print.html` & `aleksis_core-3.0b3/aleksis/core/templates/core/base_simple_print.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/templates/core/dashboard_widget/create.html` & `aleksis_core-3.0b3/aleksis/core/templates/core/dashboard_widget/create.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/templates/core/dashboard_widget/dashboardwidget_broken.html` & `aleksis_core-3.0b3/aleksis/core/templates/core/dashboard_widget/dashboardwidget_broken.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/templates/core/dashboard_widget/edit.html` & `aleksis_core-3.0b3/aleksis/core/templates/core/dashboard_widget/edit.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/templates/core/dashboard_widget/list.html` & `aleksis_core-3.0b3/aleksis/core/templates/core/dashboard_widget/list.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/templates/core/data_check/list.html` & `aleksis_core-3.0b3/aleksis/core/templates/core/data_check/list.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/templates/core/edit_dashboard.html` & `aleksis_core-3.0b3/aleksis/core/templates/core/edit_dashboard.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/templates/core/group/child_groups.html` & `aleksis_core-3.0b3/aleksis/core/templates/core/group/child_groups.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/templates/core/group/edit.html` & `aleksis_core-3.0b3/aleksis/core/templates/core/group/edit.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/templates/core/group/full.html` & `aleksis_core-3.0b3/aleksis/core/templates/core/group/full.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/templates/core/group/list.html` & `aleksis_core-3.0b3/aleksis/core/templates/core/group/list.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/templates/core/group_type/list.html` & `aleksis_core-3.0b3/aleksis/core/templates/core/group_type/list.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/templates/core/index.html` & `aleksis_core-3.0b3/aleksis/core/templates/core/index.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/templates/core/pages/delete.html` & `aleksis_core-3.0b3/aleksis/core/templates/core/pages/delete.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/templates/core/pages/system_status.html` & `aleksis_core-3.0b3/aleksis/core/templates/core/pages/system_status.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/templates/core/pages/test_pdf.html` & `aleksis_core-3.0b3/aleksis/core/templates/core/pages/test_pdf.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/templates/core/partials/announcements.html` & `aleksis_core-3.0b3/aleksis/core/templates/core/partials/announcements.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/templates/core/partials/avatar_content.html` & `aleksis_core-3.0b3/aleksis/core/templates/core/partials/avatar_content.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/templates/core/partials/crud_events.html` & `aleksis_core-3.0b3/aleksis/core/templates/core/partials/crud_events.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/templates/core/partials/meta.html` & `aleksis_core-3.0b3/aleksis/core/templates/core/partials/meta.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/templates/core/partials/splash_screen.html` & `aleksis_core-3.0b3/aleksis/core/templates/core/partials/splash_screen.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/templates/core/perms/assign.html` & `aleksis_core-3.0b3/aleksis/core/templates/core/perms/assign.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/templates/core/perms/list.html` & `aleksis_core-3.0b3/aleksis/core/templates/core/perms/list.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/templates/core/person/create.html` & `aleksis_core-3.0b3/aleksis/core/templates/core/person/create.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/templates/core/person/edit.html` & `aleksis_core-3.0b3/aleksis/core/templates/core/person/edit.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/templates/core/person/list.html` & `aleksis_core-3.0b3/aleksis/core/templates/core/person/list.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/templates/core/school_term/list.html` & `aleksis_core-3.0b3/aleksis/core/templates/core/school_term/list.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/templates/core/vue_index.html` & `aleksis_core-3.0b3/aleksis/core/templates/core/vue_index.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/templates/django_tables2/materialize.html` & `aleksis_core-3.0b3/aleksis/core/templates/django_tables2/materialize.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/templates/dynamic_preferences/form.html` & `aleksis_core-3.0b3/aleksis/core/templates/dynamic_preferences/form.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/templates/invitations/disabled.html` & `aleksis_core-3.0b3/aleksis/core/templates/invitations/disabled.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/templates/invitations/enter.html` & `aleksis_core-3.0b3/aleksis/core/templates/invitations/enter.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/templates/invitations/forms/_invite.html` & `aleksis_core-3.0b3/aleksis/core/templates/invitations/forms/_invite.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/templates/material/fields/ckeditor_ckeditorwidget.html` & `aleksis_core-3.0b3/aleksis/core/templates/material/fields/ckeditor_ckeditorwidget.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/templates/material/fields/colorfield_colorwidget.html` & `aleksis_core-3.0b3/aleksis/core/templates/material/fields/colorfield_colorwidget.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/templates/material/fields/django_select2_modelselect2multiplewidget.html` & `aleksis_core-3.0b3/aleksis/core/templates/material/fields/django_select2_modelselect2multiplewidget.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/templates/material/fields/django_select2_select2widget.html` & `aleksis_core-3.0b3/aleksis/core/templates/material/fields/django_select2_select2widget.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/templates/oauth2_provider/application/create.html` & `aleksis_core-3.0b3/aleksis/core/templates/oauth2_provider/application/create.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/templates/oauth2_provider/application/detail.html` & `aleksis_core-3.0b3/aleksis/core/templates/oauth2_provider/application/detail.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/templates/oauth2_provider/application/edit.html` & `aleksis_core-3.0b3/aleksis/core/templates/oauth2_provider/application/edit.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/templates/oauth2_provider/application/list.html` & `aleksis_core-3.0b3/aleksis/core/templates/oauth2_provider/application/list.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/templates/oauth2_provider/authorize.html` & `aleksis_core-3.0b3/aleksis/core/templates/oauth2_provider/authorize.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/templates/oauth2_provider/authorized-token-delete.html` & `aleksis_core-3.0b3/aleksis/core/templates/oauth2_provider/authorized-token-delete.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/templates/oauth2_provider/authorized-tokens.html` & `aleksis_core-3.0b3/aleksis/core/templates/oauth2_provider/authorized-tokens.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/templates/offline.html` & `aleksis_core-3.0b3/aleksis/core/templates/offline.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/templates/search/search.html` & `aleksis_core-3.0b3/aleksis/core/templates/search/search.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/templates/socialaccount/authentication_error.html` & `aleksis_core-3.0b3/aleksis/core/templates/socialaccount/authentication_error.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/templates/socialaccount/connections.html` & `aleksis_core-3.0b3/aleksis/core/templates/socialaccount/connections.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/templates/socialaccount/login.html` & `aleksis_core-3.0b3/aleksis/core/templates/socialaccount/login.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/templates/socialaccount/login_cancelled.html` & `aleksis_core-3.0b3/aleksis/core/templates/socialaccount/login_cancelled.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/templates/socialaccount/signup.html` & `aleksis_core-3.0b3/aleksis/core/templates/socialaccount/signup.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/templates/socialaccount/snippets/provider_list.html` & `aleksis_core-3.0b3/aleksis/core/templates/socialaccount/snippets/provider_list.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/templates/templated_email/base.email` & `aleksis_core-3.0b3/aleksis/core/templates/templated_email/base.email`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/templates/templated_email/celery_failure.email` & `aleksis_core-3.0b3/aleksis/core/templates/templated_email/celery_failure.email`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/templates/templated_email/data_checks.email` & `aleksis_core-3.0b3/aleksis/core/templates/templated_email/data_checks.email`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/templates/templated_email/email.css` & `aleksis_core-3.0b3/aleksis/core/templates/templated_email/email.css`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/templates/templated_email/notification.email` & `aleksis_core-3.0b3/aleksis/core/templates/templated_email/notification.email`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/templates/templated_email/person_changed.email` & `aleksis_core-3.0b3/aleksis/core/templates/templated_email/person_changed.email`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/templates/two_factor/_wizard_actions.html` & `aleksis_core-3.0b3/aleksis/core/templates/two_factor/_wizard_actions.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/templates/two_factor/core/backup_tokens.html` & `aleksis_core-3.0b3/aleksis/core/templates/two_factor/core/backup_tokens.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/templates/two_factor/core/login.html` & `aleksis_core-3.0b3/aleksis/core/templates/two_factor/core/login.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/templates/two_factor/core/otp_required.html` & `aleksis_core-3.0b3/aleksis/core/templates/two_factor/core/otp_required.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/templates/two_factor/core/phone_register.html` & `aleksis_core-3.0b3/aleksis/core/templates/two_factor/core/phone_register.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/templates/two_factor/core/setup.html` & `aleksis_core-3.0b3/aleksis/core/templates/two_factor/core/setup.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/templates/two_factor/core/setup_complete.html` & `aleksis_core-3.0b3/aleksis/core/templates/two_factor/core/setup_complete.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/templates/two_factor/profile/disable.html` & `aleksis_core-3.0b3/aleksis/core/templates/two_factor/profile/disable.html`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/templatetags/data_helpers.py` & `aleksis_core-3.0b3/aleksis/core/templatetags/data_helpers.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/templatetags/html_helpers.py` & `aleksis_core-3.0b3/aleksis/core/templatetags/html_helpers.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/tests/browser/test_selenium.py` & `aleksis_core-3.0b3/aleksis/core/tests/browser/test_selenium.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/tests/models/test.pdf` & `aleksis_core-3.0b3/aleksis/core/tests/models/test.pdf`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/tests/models/test_group.py` & `aleksis_core-3.0b3/aleksis/core/tests/models/test_group.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/tests/models/test_group_sync.py` & `aleksis_core-3.0b3/aleksis/core/tests/models/test_group_sync.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/tests/models/test_notification.py` & `aleksis_core-3.0b3/aleksis/core/tests/models/test_notification.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/tests/models/test_pdffile.py` & `aleksis_core-3.0b3/aleksis/core/tests/models/test_pdffile.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/tests/regression/test_regression.py` & `aleksis_core-3.0b3/aleksis/core/tests/regression/test_regression.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/tests/regression/view_oauth.py` & `aleksis_core-3.0b3/aleksis/core/tests/regression/view_oauth.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/tests/templatetags/test_data_helpers.py` & `aleksis_core-3.0b3/aleksis/core/tests/templatetags/test_data_helpers.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/tests/views/test_account.py` & `aleksis_core-3.0b3/aleksis/core/tests/views/test_account.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/urls.py` & `aleksis_core-3.0b3/aleksis/core/urls.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/util/__pycache__/apps.cpython-311.pyc` & `aleksis_core-3.0b3/aleksis/core/util/__pycache__/apps.cpython-311.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x794f0a64 (Thu Mar  9 21:28:25 2023 UTC)
+moddate:  0x6f611764 (Sun Mar 19 19:24:31 2023 UTC)
 files sz: 10028
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### Comparing `aleksis_core-3.0b2/aleksis/core/util/__pycache__/celery_progress.cpython-311.pyc` & `aleksis_core-3.0b3/aleksis/core/util/__pycache__/celery_progress.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x794f0a64 (Thu Mar  9 21:28:25 2023 UTC)
+moddate:  0x6f611764 (Sun Mar 19 19:24:31 2023 UTC)
 files sz: 7920
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 26
    flags     : 0
    code
```

### Comparing `aleksis_core-3.0b2/aleksis/core/util/__pycache__/core_helpers.cpython-311.pyc` & `aleksis_core-3.0b3/aleksis/core/util/__pycache__/core_helpers.cpython-311.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x794f0a64 (Thu Mar  9 21:28:25 2023 UTC)
+moddate:  0x6f611764 (Sun Mar 19 19:24:31 2023 UTC)
 files sz: 16042
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 12
    flags     : 0
    code
```

### Comparing `aleksis_core-3.0b2/aleksis/core/util/__pycache__/email.cpython-311.pyc` & `aleksis_core-3.0b3/aleksis/core/util/__pycache__/email.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x794f0a64 (Thu Mar  9 21:28:25 2023 UTC)
+moddate:  0x6f611764 (Sun Mar 19 19:24:31 2023 UTC)
 files sz: 986
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 10
    flags     : 0
    code
```

### Comparing `aleksis_core-3.0b2/aleksis/core/util/__pycache__/model_helpers.cpython-311.pyc` & `aleksis_core-3.0b3/aleksis/core/util/__pycache__/model_helpers.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x794f0a64 (Thu Mar  9 21:28:25 2023 UTC)
+moddate:  0x6f611764 (Sun Mar 19 19:24:31 2023 UTC)
 files sz: 850
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 4
    flags     : 0
    code
```

### Comparing `aleksis_core-3.0b2/aleksis/core/util/__pycache__/notifications.cpython-311.pyc` & `aleksis_core-3.0b3/aleksis/core/util/__pycache__/notifications.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x794f0a64 (Thu Mar  9 21:28:25 2023 UTC)
+moddate:  0x6f611764 (Sun Mar 19 19:24:31 2023 UTC)
 files sz: 3732
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 10
    flags     : 0
    code
```

### Comparing `aleksis_core-3.0b2/aleksis/core/util/__pycache__/predicates.cpython-311.pyc` & `aleksis_core-3.0b3/aleksis/core/util/__pycache__/predicates.cpython-311.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x794f0a64 (Thu Mar  9 21:28:25 2023 UTC)
+moddate:  0x6f611764 (Sun Mar 19 19:24:31 2023 UTC)
 files sz: 5583
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 11
    flags     : 0
    code
```

### Comparing `aleksis_core-3.0b2/aleksis/core/util/__pycache__/sass_helpers.cpython-311.pyc` & `aleksis_core-3.0b3/aleksis/core/util/__pycache__/sass_helpers.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x794f0a64 (Thu Mar  9 21:28:25 2023 UTC)
+moddate:  0x6f611764 (Sun Mar 19 19:24:31 2023 UTC)
 files sz: 936
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 6
    flags     : 0
    code
```

### Comparing `aleksis_core-3.0b2/aleksis/core/util/__pycache__/spdx.cpython-311.pyc` & `aleksis_core-3.0b3/aleksis/core/util/__pycache__/spdx.cpython-311.pyc`

 * *Files 4% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x794f0a64 (Thu Mar  9 21:28:25 2023 UTC)
+moddate:  0x6f611764 (Sun Mar 19 19:24:31 2023 UTC)
 files sz: 130
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 7
    flags     : 0
    code
```

### Comparing `aleksis_core-3.0b2/aleksis/core/util/apps.py` & `aleksis_core-3.0b3/aleksis/core/util/apps.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/util/auth_helpers.py` & `aleksis_core-3.0b3/aleksis/core/util/auth_helpers.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/util/celery_progress.py` & `aleksis_core-3.0b3/aleksis/core/util/celery_progress.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/util/core_helpers.py` & `aleksis_core-3.0b3/aleksis/core/util/core_helpers.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/util/email.py` & `aleksis_core-3.0b3/aleksis/core/util/email.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/util/forms.py` & `aleksis_core-3.0b3/aleksis/core/util/forms.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/util/frontend_helpers.py` & `aleksis_core-3.0b3/aleksis/core/util/frontend_helpers.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/util/ldap.py` & `aleksis_core-3.0b3/aleksis/core/util/ldap.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/util/licenses.json` & `aleksis_core-3.0b3/aleksis/core/util/licenses.json`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/util/messages.py` & `aleksis_core-3.0b3/aleksis/core/util/messages.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/util/middlewares.py` & `aleksis_core-3.0b3/aleksis/core/util/middlewares.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/util/model_helpers.py` & `aleksis_core-3.0b3/aleksis/core/util/model_helpers.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/util/notifications.py` & `aleksis_core-3.0b3/aleksis/core/util/notifications.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/util/pdf.py` & `aleksis_core-3.0b3/aleksis/core/util/pdf.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/util/predicates.py` & `aleksis_core-3.0b3/aleksis/core/util/predicates.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/util/sass_helpers.py` & `aleksis_core-3.0b3/aleksis/core/util/sass_helpers.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/util/search.py` & `aleksis_core-3.0b3/aleksis/core/util/search.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/util/tables.py` & `aleksis_core-3.0b3/aleksis/core/util/tables.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/views.py` & `aleksis_core-3.0b3/aleksis/core/views.py`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/aleksis/core/vite.config.js` & `aleksis_core-3.0b3/aleksis/core/vite.config.js`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/docs/Makefile` & `aleksis_core-3.0b3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/docs/_static/2fa.png` & `aleksis_core-3.0b3/docs/_static/2fa.png`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/docs/_static/accept_invite.png` & `aleksis_core-3.0b3/docs/_static/accept_invite.png`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/docs/_static/create_dashboard_widget.png` & `aleksis_core-3.0b3/docs/_static/create_dashboard_widget.png`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/docs/_static/create_social_application.png` & `aleksis_core-3.0b3/docs/_static/create_social_application.png`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/docs/_static/dashboard.png` & `aleksis_core-3.0b3/docs/_static/dashboard.png`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/docs/_static/dashboard_widgets.png` & `aleksis_core-3.0b3/docs/_static/dashboard_widgets.png`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/docs/_static/data_checks.png` & `aleksis_core-3.0b3/docs/_static/data_checks.png`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/docs/_static/edit_dashboard.png` & `aleksis_core-3.0b3/docs/_static/edit_dashboard.png`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/docs/_static/edit_default_dashboard.png` & `aleksis_core-3.0b3/docs/_static/edit_default_dashboard.png`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/docs/_static/invitations.png` & `aleksis_core-3.0b3/docs/_static/invitations.png`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/docs/_static/invite_existing.png` & `aleksis_core-3.0b3/docs/_static/invite_existing.png`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/docs/_static/pwa_desktop_chromium.png` & `aleksis_core-3.0b3/docs/_static/pwa_desktop_chromium.png`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/docs/_static/pwa_mobile_chromium.png` & `aleksis_core-3.0b3/docs/_static/pwa_mobile_chromium.png`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/docs/_static/pwa_mobile_firefox.png` & `aleksis_core-3.0b3/docs/_static/pwa_mobile_firefox.png`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/docs/_static/pwa_mobile_safari.png` & `aleksis_core-3.0b3/docs/_static/pwa_mobile_safari.png`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/docs/_static/signup.png` & `aleksis_core-3.0b3/docs/_static/signup.png`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/docs/admin/01_core_concepts.rst` & `aleksis_core-3.0b3/docs/admin/01_core_concepts.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/docs/admin/10_install.rst` & `aleksis_core-3.0b3/docs/admin/10_install.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/docs/admin/15_config_files.rst` & `aleksis_core-3.0b3/docs/admin/15_config_files.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/docs/admin/16_config_options.rst` & `aleksis_core-3.0b3/docs/admin/16_config_options.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/docs/admin/17_storage.rst` & `aleksis_core-3.0b3/docs/admin/17_storage.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/docs/admin/18_mail.rst` & `aleksis_core-3.0b3/docs/admin/18_mail.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/docs/admin/21_ldap.rst` & `aleksis_core-3.0b3/docs/admin/21_ldap.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/docs/admin/22_registration.rst` & `aleksis_core-3.0b3/docs/admin/22_registration.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/docs/admin/23_socialaccounts.rst` & `aleksis_core-3.0b3/docs/admin/23_socialaccounts.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/docs/admin/31_monitoring.rst` & `aleksis_core-3.0b3/docs/admin/31_monitoring.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/docs/admin/32_tasks.rst` & `aleksis_core-3.0b3/docs/admin/32_tasks.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/docs/admin/33_data_checks.rst` & `aleksis_core-3.0b3/docs/admin/33_data_checks.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/docs/admin/50_dashboard.rst` & `aleksis_core-3.0b3/docs/admin/50_dashboard.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/docs/conf.py` & `aleksis_core-3.0b3/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 project = "AlekSIS-Core"
 copyright = "2019-2022 The AlekSIS team"
 author = "The AlekSIS Team"
 
 # The short X.Y version
 version = "3.0"
 # The full version, including alpha/beta/rc tags
-release = "3.0b2"
+release = "3.0b3"
 
 
 # -- General configuration ---------------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
 #
 # needs_sphinx = '1.0'
```

### Comparing `aleksis_core-3.0b2/docs/dev/01_setup.rst` & `aleksis_core-3.0b3/docs/dev/01_setup.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/docs/dev/02_install_apps.rst` & `aleksis_core-3.0b3/docs/dev/02_install_apps.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/docs/dev/03_run_tests.rst` & `aleksis_core-3.0b3/docs/dev/03_run_tests.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/docs/dev/04_materialize_templates.rst` & `aleksis_core-3.0b3/docs/dev/04_materialize_templates.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/docs/dev/06_merging_app_settings.rst` & `aleksis_core-3.0b3/docs/dev/06_merging_app_settings.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/docs/dev/10_dashboard_widgets.rst` & `aleksis_core-3.0b3/docs/dev/10_dashboard_widgets.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/docs/index.rst` & `aleksis_core-3.0b3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/docs/make.bat` & `aleksis_core-3.0b3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/docs/ref/core/09_utils.rst` & `aleksis_core-3.0b3/docs/ref/core/09_utils.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/docs/user/01_registration.rst` & `aleksis_core-3.0b3/docs/user/01_registration.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/docs/user/02_personal_account.rst` & `aleksis_core-3.0b3/docs/user/02_personal_account.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/docs/user/10_dashboard.rst` & `aleksis_core-3.0b3/docs/user/10_dashboard.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/docs/user/20_pwa.rst` & `aleksis_core-3.0b3/docs/user/20_pwa.rst`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/pyproject.toml` & `aleksis_core-3.0b3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "AlekSIS-Core"
-version = "3.0b2"
+version = "3.0b3"
 packages = [
     { include = "aleksis" }
 ]
 readme = "README.rst"
 include = [
     { path = "aleksis/**/*.mo", format = ["sdist", "wheel"] },
     { path = "*.rst", format = "sdist" },
@@ -102,15 +102,15 @@
 celery-progress = "^0.1.0"
 django-cachalot = "^2.3.2"
 django-prometheus = "^2.1.0"
 django-model-utils = "^4.0.0"
 bs4 = "^0.0.1"
 django-invitations = "^2.0.0"
 django-cleavejs = "^0.1.0"
-django-allauth = "^0.52.0"
+django-allauth = "^0.53.0"
 django-uwsgi-ng = "^2.0"
 django-extensions = "^3.1.1"
 ipython = "^8.0.0"
 django-oauth-toolkit = "^2.0.0"
 django-storages = {version = "^1.11.1", optional = true}
 boto3 = {version = "^1.17.33", optional = true}
 django-cleanup = "^7.0.0"
```

### Comparing `aleksis_core-3.0b2/tox.ini` & `aleksis_core-3.0b3/tox.ini`

 * *Files identical despite different names*

### Comparing `aleksis_core-3.0b2/setup.py` & `aleksis_core-3.0b3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -87,15 +87,15 @@
  'Whoosh>=2.7.4,<3.0.0',
  'bs4>=0.0.1,<0.0.2',
  'calendarweek>=0.5.0,<0.6.0',
  'celery-haystack-ng>=2.0,<3.0',
  'celery-progress>=0.1.0,<0.2.0',
  'colour>=0.1.5,<0.2.0',
  'customidenticon>=0.1.5,<0.2.0',
- 'django-allauth>=0.52.0,<0.53.0',
+ 'django-allauth>=0.53.0,<0.54.0',
  'django-any-js>=1.1,<2.0',
  'django-bleach>=3.0.0,<4.0.0',
  'django-cachalot>=2.3.2,<3.0.0',
  'django-cache-memoize>=0.1.6,<0.2.0',
  'django-celery-beat>=2.2.0,<3.0.0',
  'django-celery-email>=3.0.0,<4.0.0',
  'django-celery-results>=2.0.1,<3.0.0',
@@ -156,15 +156,15 @@
  'sentry': ['sentry-sdk>=1.4.3,<2.0.0']}
 
 entry_points = \
 {'console_scripts': ['aleksis-admin = aleksis.core.__main__:aleksis_cmd']}
 
 setup_kwargs = {
     'name': 'aleksis-core',
-    'version': '3.0b2',
+    'version': '3.0b3',
     'description': 'AlekSIS (School Information System)\u200a—\u200aCore',
     'long_description': 'AlekSIS (School Information System)\u200a—\u200aCore (Core functionality and app framework)\n=================================================================================\n\nThis is the core of the AlekSIS framework and the official distribution\n(see below). It bundles functionality for all apps, and utilities for\ndevelopers and administrators.\n\nIf you are looking for the AlekSIS standard distribution, i.e. the complete\nsoftware product ready for installation and usage, please visit the `AlekSIS®`_\nwebsite or the distribution repository on `EduGit`_.\n\nFeatures\n--------\n\nThe AlekSIS core currently provides the following features:\n\n* For users:\n\n * Authentication via local account, LDAP, or social accounts\n * Two factor authentication via Yubikey, OTP or SMS\n * Configurable dashboard with widgets\n * User-specific preferences\n * Global search\n * Manage announcements\n * Manage groups and types of groups\n * Manage roles and additional, informative fields per group\n * Manage persons\n * Notifications via SMS, email or dashboard\n * PWA with offline caching\n * User registration, password changes and password reset\n * User invitations with invite codes and targeted invites\n\n* For admins\n\n * `aleksis-admin` script to wrap django-admin with pre-configured settings\n * Manage school terms\n * Custom menu entries (e.g. in footer)\n * Automatic backup of database, static and media files\n * OAuth2 and OpenID Connect provider support\n * Serve prometheus metrics\n * System health and data checks\n * Configuration of low-level settings via configuration files\n * System-wide preferenes\n * Creating dashboard widgets for external links/apps\n\n* For developers\n\n * Generic PDF generation with chromium\n * Caching with Redis\n * Django REST framework for apps to use at own discretion\n * Injection of fields, methods, permissions and properties via custom `ExtensibleModel`\n * K8s compatible, read-only Docker image\n * Object-level permissions and rules with `django-guardian` and `django-rules`\n * Query caching with `django-cachalot`\n * uWSGI and Celery via `django-uwsgi` in development\n * Extensible dashbaord widget system\n * Extensible OAuth/OpenID Connect scope and claims system\n\nLicence\n-------\n\n::\n\n  Copyright © 2017, 2018, 2019, 2020, 2021, 2022, 2023 Jonathan Weth <dev@jonathanweth.de>\n  Copyright © 2017, 2018, 2019, 2020 Frank Poetzsch-Heffter <p-h@katharineum.de>\n  Copyright © 2018, 2019, 2020, 2021, 2022, 2023 Hangzhi Yu <yuha@katharineum.de>\n  Copyright © 2018, 2019, 2020, 2021, 2022, 2023 Julian Leucker <leuckeju@katharineum.de>\n  Copyright © 2019, 2020, 2021, 2022, 2023 Dominik George <dominik.george@teckids.org>\n  Copyright © 2019, 2020, 2021, 2022 Tom Teichler <tom.teichler@teckids.org>\n  Copyright © 2019 mirabilos <thorsten.glaser@teckids.org>\n  Copyright © 2021, 2022 magicfelix <felix@felix-zauberer.de>\n  Copyright © 2021 Lloyd Meins <meinsll@katharineum.de>\n  Copyright © 2022 Benedict Suska <benedict.suska@teckids.org>\n  Copyright © 2022 Lukas Weichelt <lukas.weichelt@teckids.org>\n\n  Licenced under the EUPL, version 1.2 or later, by Teckids e.V. (Bonn, Germany).\n\nPlease see the LICENCE.rst file accompanying this distribution for the\nfull licence text or on the `European Union Public Licence`_ website\nhttps://joinup.ec.europa.eu/collection/eupl/guidelines-users-and-developers\n(including all other official language versions).\n\nTrademark\n---------\n\nAlekSIS® is a registered trademark of the AlekSIS open source project, represented\nby Teckids e.V. Please refer to the `trademark policy`_ for hints on using the trademark\nAlekSIS®.\n\n.. _AlekSIS®: https://aleksis.org\n.. _European Union Public Licence: https://eupl.eu/\n.. _EduGit: https://edugit.org/AlekSIS/official/AlekSIS\n.. _trademark policy: https://aleksis.org/pages/about\n',
     'author': 'Dominik George',
     'author_email': 'dominik.george@teckids.org',
     'maintainer': 'Jonathan Weth',
     'maintainer_email': 'dev@jonathanweth.de',
     'url': 'https://aleksis.org/',
```

### Comparing `aleksis_core-3.0b2/PKG-INFO` & `aleksis_core-3.0b3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aleksis-core
-Version: 3.0b2
+Version: 3.0b3
 Summary: AlekSIS (School Information System) — Core
 Home-page: https://aleksis.org/
 License: EUPL-1.2-or-later
 Keywords: SIS,education,school,digitisation,school apps
 Author: Dominik George
 Author-email: dominik.george@teckids.org
 Maintainer: Jonathan Weth
@@ -33,15 +33,15 @@
 Requires-Dist: boto3 (>=1.17.33,<2.0.0) ; extra == "s3"
 Requires-Dist: bs4 (>=0.0.1,<0.0.2)
 Requires-Dist: calendarweek (>=0.5.0,<0.6.0)
 Requires-Dist: celery-haystack-ng (>=2.0,<3.0)
 Requires-Dist: celery-progress (>=0.1.0,<0.2.0)
 Requires-Dist: colour (>=0.1.5,<0.2.0)
 Requires-Dist: customidenticon (>=0.1.5,<0.2.0)
-Requires-Dist: django-allauth (>=0.52.0,<0.53.0)
+Requires-Dist: django-allauth (>=0.53.0,<0.54.0)
 Requires-Dist: django-any-js (>=1.1,<2.0)
 Requires-Dist: django-auth-ldap (>=4.0,<5.0) ; extra == "ldap"
 Requires-Dist: django-bleach (>=3.0.0,<4.0.0)
 Requires-Dist: django-cachalot (>=2.3.2,<3.0.0)
 Requires-Dist: django-cache-memoize (>=0.1.6,<0.2.0)
 Requires-Dist: django-celery-beat (>=2.2.0,<3.0.0)
 Requires-Dist: django-celery-email (>=3.0.0,<4.0.0)
```

