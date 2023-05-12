# Comparing `tmp/repository_service_tuf-0.1.1a3.tar.gz` & `tmp/repository_service_tuf-0.1.2a1.tar.gz`

## Comparing `repository_service_tuf-0.1.1a3.tar` & `repository_service_tuf-0.1.2a1.tar`

### file list

```diff
@@ -1,86 +1,80 @@
--rw-r--r--   0        0        0     1886 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/.gitignore
--rw-r--r--   0        0        0     1332 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/.pre-commit-config.yaml
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/.readthedocs.yaml
--rw-r--r--   0        0        0     5444 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/CODE_OF_CONDUCT.rst
--rw-r--r--   0        0        0     4117 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/CONTRIBUTING.rst
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/LICENSE
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/MAINTAINERS.rst
--rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/Makefile
--rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/Pipfile
--rw-r--r--   0        0        0    80773 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/Pipfile.lock
--rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/README.rst
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/id_ed25519
--rwxr-xr-x   0        0        0      180 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/id_ed25519.pub
--rw-r--r--   0        0        0     1471 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/pyproject.toml
--rw-r--r--   0        0        0     3326 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/requirements-dev.txt
--rw-r--r--   0        0        0     1036 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/requirements.txt
--rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/rstuf.ini
--rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/tox.ini
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/.github/dependabot.yml
--rw-r--r--   0        0        0     1437 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/.github/ISSUE_TEMPLATE/bug.yml
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/.github/ISSUE_TEMPLATE/other.yml
--rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/.github/ISSUE_TEMPLATE/task.yml
--rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/.github/PULL_REQUEST_TEMPLATE/pr.yml
--rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/.github/workflows/cd.yml
--rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/.github/workflows/ci.yml
--rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/.github/workflows/update-python-deps.yml
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/docs/Makefile
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/docs/make.bat
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/docs/requirements.txt
--rw-r--r--   0        0        0     2941 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/docs/diagrams/repository-service-tuf-cli-C1.puml
--rw-r--r--   0        0        0     5408 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/docs/diagrams/repository-service-tuf-cli-C2.puml
--rw-r--r--   0        0        0     4192 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/docs/diagrams/repository-service-tuf-cli-C3.puml
--rw-r--r--   0        0        0     2081 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/docs/source/conf.py
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/docs/source/index.rst
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/docs/source/_static/INFO
--rw-r--r--   0        0        0    19648 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/docs/source/_static/repository-service-tuf-cli-C1.png
--rw-r--r--   0        0        0    41916 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/docs/source/_static/repository-service-tuf-cli-C2.png
--rw-r--r--   0        0        0    94852 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/docs/source/_static/repository-service-tuf-cli-C3.png
--rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/docs/source/devel/design.rst
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/docs/source/devel/index.rst
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/docs/source/devel/modules.rst
--rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/docs/source/devel/repository_service_tuf.cli.admin.rst
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/docs/source/devel/repository_service_tuf.cli.key.rst
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/docs/source/devel/repository_service_tuf.cli.rst
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/docs/source/devel/repository_service_tuf.helpers.rst
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/docs/source/devel/repository_service_tuf.rst
--rw-r--r--   0        0        0    45409 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/docs/source/guide/index.rst
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/repository_service_tuf/__init__.py
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/repository_service_tuf/__version__.py
--rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/repository_service_tuf/constants.py
--rw-r--r--   0        0        0     2262 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/repository_service_tuf/cli/__init__.py
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/repository_service_tuf/cli/admin/__init__.py
--rw-r--r--   0        0        0    24979 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/repository_service_tuf/cli/admin/ceremony.py
--rw-r--r--   0        0        0     6165 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/repository_service_tuf/cli/admin/import_targets.py
--rw-r--r--   0        0        0     3954 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/repository_service_tuf/cli/admin/login.py
--rw-r--r--   0        0        0     2679 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/repository_service_tuf/cli/admin/token.py
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/repository_service_tuf/cli/key/__init__.py
--rw-r--r--   0        0        0     2447 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/repository_service_tuf/cli/key/generate_key.py
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/repository_service_tuf/helpers/__init__.py
--rw-r--r--   0        0        0     5928 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/repository_service_tuf/helpers/api_client.py
--rw-r--r--   0        0        0     7454 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/repository_service_tuf/helpers/tuf.py
--rwxr-xr-x   0        0        0      861 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/tests/2.targets.json
--rw-r--r--   0        0        0     3718 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/tests/conftest.py
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/tests/test_tuf_repository_service.py
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/tests/files/README.md
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/tests/files/key_storage/JanisJoplin.key
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/tests/files/key_storage/JanisJoplin.pub
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/tests/files/key_storage/JimiHendrix.key
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/tests/files/key_storage/JimiHendrix.pub
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/tests/files/key_storage/JoeCocker.key
--rwxr-xr-x   0        0        0      180 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/tests/files/key_storage/JoeCocker.key.pub
--rw-r--r--   0        0        0     2546 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/tests/files/key_storage/online-rsa.key
--rwxr-xr-x   0        0        0      624 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/tests/files/key_storage/online-rsa.pub
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/tests/files/key_storage/online.key
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/tests/files/key_storage/online.pub
--rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/tests/unit/cli/test__init__.py
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/tests/unit/cli/admin/__init__.py
--rw-r--r--   0        0        0    30164 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/tests/unit/cli/admin/test_ceremony.py
--rw-r--r--   0        0        0    15993 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/tests/unit/cli/admin/test_import_targets.py
--rw-r--r--   0        0        0    11817 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/tests/unit/cli/admin/test_login.py
--rw-r--r--   0        0        0     5620 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/tests/unit/cli/key/test_generate_key.py
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/tests/unit/helpers/__init__.py
--rw-r--r--   0        0        0    21182 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/tests/unit/helpers/test_api_client.py
--rw-r--r--   0        0        0    12210 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/tests/unit/helpers/test_tuf.py
--rw-r--r--   0        0        0     2894 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.1a3/PKG-INFO
+-rw-r--r--   0        0        0     1886 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/.gitignore
+-rw-r--r--   0        0        0     1332 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/.readthedocs.yaml
+-rw-r--r--   0        0        0     5444 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/CODE_OF_CONDUCT.rst
+-rw-r--r--   0        0        0     4149 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/CONTRIBUTING.rst
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/LICENSE
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/MAINTAINERS.rst
+-rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/Makefile
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/Pipfile
+-rw-r--r--   0        0        0    80651 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/Pipfile.lock
+-rw-r--r--   0        0        0     1885 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/README.rst
+-rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/pyproject.toml
+-rw-r--r--   0        0        0     3264 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/requirements-dev.txt
+-rw-r--r--   0        0        0      977 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/requirements.txt
+-rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/tox.ini
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/.github/dependabot.yml
+-rw-r--r--   0        0        0     1437 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/.github/ISSUE_TEMPLATE/bug.yml
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/.github/ISSUE_TEMPLATE/other.yml
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/.github/ISSUE_TEMPLATE/task.yml
+-rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/.github/PULL_REQUEST_TEMPLATE/pr.yml
+-rw-r--r--   0        0        0     3507 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/.github/workflows/cd.yml
+-rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/.github/workflows/update-python-deps.yml
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/docs/Makefile
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/docs/make.bat
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/docs/requirements.txt
+-rw-r--r--   0        0        0     2941 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/docs/diagrams/repository-service-tuf-cli-C1.puml
+-rw-r--r--   0        0        0     5408 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/docs/diagrams/repository-service-tuf-cli-C2.puml
+-rw-r--r--   0        0        0     4192 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/docs/diagrams/repository-service-tuf-cli-C3.puml
+-rw-r--r--   0        0        0     2081 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/docs/source/conf.py
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/docs/source/index.rst
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/docs/source/_static/INFO
+-rw-r--r--   0        0        0    19648 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/docs/source/_static/repository-service-tuf-cli-C1.png
+-rw-r--r--   0        0        0    41916 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/docs/source/_static/repository-service-tuf-cli-C2.png
+-rw-r--r--   0        0        0    94852 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/docs/source/_static/repository-service-tuf-cli-C3.png
+-rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/docs/source/devel/design.rst
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/docs/source/devel/index.rst
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/docs/source/devel/modules.rst
+-rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/docs/source/devel/repository_service_tuf.cli.admin.rst
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/docs/source/devel/repository_service_tuf.cli.key.rst
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/docs/source/devel/repository_service_tuf.cli.rst
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/docs/source/devel/repository_service_tuf.helpers.rst
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/docs/source/devel/repository_service_tuf.rst
+-rw-r--r--   0        0        0    45538 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/docs/source/guide/index.rst
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/repository_service_tuf/__init__.py
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/repository_service_tuf/__version__.py
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/repository_service_tuf/constants.py
+-rw-r--r--   0        0        0     2262 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/repository_service_tuf/cli/__init__.py
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/repository_service_tuf/cli/admin/__init__.py
+-rw-r--r--   0        0        0    25465 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/repository_service_tuf/cli/admin/ceremony.py
+-rw-r--r--   0        0        0     6165 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/repository_service_tuf/cli/admin/import_targets.py
+-rw-r--r--   0        0        0     3954 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/repository_service_tuf/cli/admin/login.py
+-rw-r--r--   0        0        0     2679 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/repository_service_tuf/cli/admin/token.py
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/repository_service_tuf/cli/key/__init__.py
+-rw-r--r--   0        0        0     2505 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/repository_service_tuf/cli/key/generate_key.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/repository_service_tuf/helpers/__init__.py
+-rw-r--r--   0        0        0     5928 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/repository_service_tuf/helpers/api_client.py
+-rw-r--r--   0        0        0     8014 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/repository_service_tuf/helpers/tuf.py
+-rw-r--r--   0        0        0     3879 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/tests/conftest.py
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/tests/test_tuf_repository_service.py
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/tests/files/README.md
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/tests/files/key_storage/JanisJoplin.key
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/tests/files/key_storage/JanisJoplin.pub
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/tests/files/key_storage/JimiHendrix.key
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/tests/files/key_storage/JimiHendrix.pub
+-rw-r--r--   0        0        0     2546 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/tests/files/key_storage/online-rsa.key
+-rwxr-xr-x   0        0        0      624 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/tests/files/key_storage/online-rsa.pub
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/tests/files/key_storage/online.key
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/tests/files/key_storage/online.pub
+-rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/tests/unit/cli/test__init__.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/tests/unit/cli/admin/__init__.py
+-rw-r--r--   0        0        0    32379 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/tests/unit/cli/admin/test_ceremony.py
+-rw-r--r--   0        0        0    15993 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/tests/unit/cli/admin/test_import_targets.py
+-rw-r--r--   0        0        0    11817 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/tests/unit/cli/admin/test_login.py
+-rw-r--r--   0        0        0     7313 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/tests/unit/cli/key/test_generate_key.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/tests/unit/helpers/__init__.py
+-rw-r--r--   0        0        0    21182 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/tests/unit/helpers/test_api_client.py
+-rw-r--r--   0        0        0    13747 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/tests/unit/helpers/test_tuf.py
+-rw-r--r--   0        0        0     2940 2020-02-02 00:00:00.000000 repository_service_tuf-0.1.2a1/PKG-INFO
```

### Comparing `repository_service_tuf-0.1.1a3/.gitignore` & `repository_service_tuf-0.1.2a1/.gitignore`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.1a3/.pre-commit-config.yaml` & `repository_service_tuf-0.1.2a1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.1a3/.readthedocs.yaml` & `repository_service_tuf-0.1.2a1/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.1a3/CODE_OF_CONDUCT.rst` & `repository_service_tuf-0.1.2a1/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.1a3/CONTRIBUTING.rst` & `repository_service_tuf-0.1.2a1/CONTRIBUTING.rst`

 * *Files 2% similar despite different names*

```diff
@@ -39,37 +39,37 @@
 
 Development
 ===========
 
 Requirements
 -------------
 
-- Python >=3.9
+- Python >=3.8
 - Pipenv
 
 Getting the source code
 -----------------------
 
 `Fork <https://docs.github.com/en/get-started/quickstart/fork-a-repo>`_ the
-repository on `GitHub <https://github.com/vmware/repository-service-tuf-cli>`_ and
+repository on `GitHub <https://github.com/repository-service-tuf/repository-service-tuf-cli>`_ and
 `clone <https://docs.github.com/en/repositories/creating-and-managing-repositories/cloning-a-repository>`_
 it to your local machine:
 
 .. code-block:: console
 
     git clone git@github.com:YOUR-USERNAME/repository-service-tuf-cli.git
 
 Add a `remote
 <https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/working-with-forks/configuring-a-remote-for-a-fork>`_ and
 regularly `sync <https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/working-with-forks/syncing-a-fork>`_ to make sure
 you stay up-to-date with our repository:
 
 .. code-block:: console
 
-    git remote add upstream https://github.com/vmware/repository-service-tuf-cli
+    git remote add upstream https://github.com/repository-service-tuf/repository-service-tuf-cli
     git checkout main
     git fetch upstream
     git merge upstream/main
 
 Preparing the environment
 -------------------------
```

### Comparing `repository_service_tuf-0.1.1a3/LICENSE` & `repository_service_tuf-0.1.2a1/LICENSE`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.1a3/Pipfile` & `repository_service_tuf-0.1.2a1/Pipfile`

 * *Files 2% similar despite different names*

```diff
@@ -38,8 +38,8 @@
 hatchling = "==0.22.0"
 build = "*"
 pre-commit = "*"
 bandit = "*"
 types-requests = "*"
 
 [requires]
-python_version = "3.10"
+python_version = "3.8"
```

### Comparing `repository_service_tuf-0.1.1a3/Pipfile.lock` & `repository_service_tuf-0.1.2a1/Pipfile.lock`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9830479452054793%*

 * *Differences: {"'default'": "{'certifi': {'hashes': "*

 * *              "['sha256:0f0d56dc5a6ad56fd4ba36484d6cc34451e1c6548c61daad8c320169f91eddc7', "*

 * *              "'sha256:c6c2e98f5c7869efca1f8916fed228dd91539f9f1b444c314c06eef02980c716'], "*

 * *              "'version': '==2023.5.7'}, 'cryptography': {'hashes': "*

 * *              "['sha256:05dc219433b14046c476f6f09d7636b92a1c3e5808b9a6536adf4932b3b2c440', "*

 * *              "'sha256:0dcca15d3a19a66e63662dc8d30f8036b07be851a8680eda92d079868f106288', "*

 * *              "'sha256:142bae53 […]*

```diff
@@ -14,19 +14,19 @@
                 "verify_ssl": true
             }
         ]
     },
     "default": {
         "certifi": {
             "hashes": [
-                "sha256:35824b4c3a97115964b408844d64aa14db1cc518f6562e8d7261699d1350a9e3",
-                "sha256:4ad3232f5e926d6718ec31cfc1fcadfde020920e278684144551c91769c7bc18"
+                "sha256:0f0d56dc5a6ad56fd4ba36484d6cc34451e1c6548c61daad8c320169f91eddc7",
+                "sha256:c6c2e98f5c7869efca1f8916fed228dd91539f9f1b444c314c06eef02980c716"
             ],
             "markers": "python_version >= '3.6'",
-            "version": "==2022.12.7"
+            "version": "==2023.5.7"
         },
         "cffi": {
             "hashes": [
                 "sha256:00a9ed42e88df81ffae7a8ab6d9356b371399b91dbdf0c3cb1e84c03a13aceb5",
                 "sha256:03425bdae262c76aad70202debd780501fabeaca237cdfddc008987c0e0f59ef",
                 "sha256:04ed324bda3cda42b9b695d51bb7d54b680b9719cfab04227cdd1e04e5de3104",
                 "sha256:0e2642fe3142e4cc4af0799748233ad6da94c62a8bec3a6648bf8ee68b1c7426",
@@ -188,35 +188,35 @@
                 "sha256:a7a8c6ab7daade85c3f329931a807c8aee750a2494363934f8ea84d8a54c87ea",
                 "sha256:d808d7e04e6f81fbb23d5ac2cd50e69ccbee58eaf9360eb89ede22d93216a314"
             ],
             "version": "==5.0.8"
         },
         "cryptography": {
             "hashes": [
-                "sha256:0a4e3406cfed6b1f6d6e87ed243363652b2586b2d917b0609ca4f97072994405",
-                "sha256:1e0af458515d5e4028aad75f3bb3fe7a31e46ad920648cd59b64d3da842e4356",
-                "sha256:2803f2f8b1e95f614419926c7e6f55d828afc614ca5ed61543877ae668cc3472",
-                "sha256:28d63d75bf7ae4045b10de5413fb1d6338616e79015999ad9cf6fc538f772d41",
-                "sha256:32057d3d0ab7d4453778367ca43e99ddb711770477c4f072a51b3ca69602780a",
-                "sha256:3a4805a4ca729d65570a1b7cac84eac1e431085d40387b7d3bbaa47e39890b88",
-                "sha256:63dac2d25c47f12a7b8aa60e528bfb3c51c5a6c5a9f7c86987909c6c79765554",
-                "sha256:650883cc064297ef3676b1db1b7b1df6081794c4ada96fa457253c4cc40f97db",
-                "sha256:6f2bbd72f717ce33100e6467572abaedc61f1acb87b8d546001328d7f466b778",
-                "sha256:7c872413353c70e0263a9368c4993710070e70ab3e5318d85510cc91cce77e7c",
-                "sha256:918cb89086c7d98b1b86b9fdb70c712e5a9325ba6f7d7cfb509e784e0cfc6917",
-                "sha256:9618a87212cb5200500e304e43691111570e1f10ec3f35569fdfcd17e28fd797",
-                "sha256:a805a7bce4a77d51696410005b3e85ae2839bad9aa38894afc0aa99d8e0c3160",
-                "sha256:cc3a621076d824d75ab1e1e530e66e7e8564e357dd723f2533225d40fe35c60c",
-                "sha256:cd033d74067d8928ef00a6b1327c8ea0452523967ca4463666eeba65ca350d4c",
-                "sha256:cf91e428c51ef692b82ce786583e214f58392399cf65c341bc7301d096fa3ba2",
-                "sha256:d36bbeb99704aabefdca5aee4eba04455d7a27ceabd16f3b3ba9bdcc31da86c4",
-                "sha256:d8aa3609d337ad85e4eb9bb0f8bcf6e4409bfb86e706efa9a027912169e89122",
-                "sha256:f5d7b79fa56bc29580faafc2ff736ce05ba31feaa9d4735048b0de7d9ceb2b94"
+                "sha256:05dc219433b14046c476f6f09d7636b92a1c3e5808b9a6536adf4932b3b2c440",
+                "sha256:0dcca15d3a19a66e63662dc8d30f8036b07be851a8680eda92d079868f106288",
+                "sha256:142bae539ef28a1c76794cca7f49729e7c54423f615cfd9b0b1fa90ebe53244b",
+                "sha256:3daf9b114213f8ba460b829a02896789751626a2a4e7a43a28ee77c04b5e4958",
+                "sha256:48f388d0d153350f378c7f7b41497a54ff1513c816bcbbcafe5b829e59b9ce5b",
+                "sha256:4df2af28d7bedc84fe45bd49bc35d710aede676e2a4cb7fc6d103a2adc8afe4d",
+                "sha256:4f01c9863da784558165f5d4d916093737a75203a5c5286fde60e503e4276c7a",
+                "sha256:7a38250f433cd41df7fcb763caa3ee9362777fdb4dc642b9a349721d2bf47404",
+                "sha256:8f79b5ff5ad9d3218afb1e7e20ea74da5f76943ee5edb7f76e56ec5161ec782b",
+                "sha256:956ba8701b4ffe91ba59665ed170a2ebbdc6fc0e40de5f6059195d9f2b33ca0e",
+                "sha256:a04386fb7bc85fab9cd51b6308633a3c271e3d0d3eae917eebab2fac6219b6d2",
+                "sha256:a95f4802d49faa6a674242e25bfeea6fc2acd915b5e5e29ac90a32b1139cae1c",
+                "sha256:adc0d980fd2760c9e5de537c28935cc32b9353baaf28e0814df417619c6c8c3b",
+                "sha256:aecbb1592b0188e030cb01f82d12556cf72e218280f621deed7d806afd2113f9",
+                "sha256:b12794f01d4cacfbd3177b9042198f3af1c856eedd0a98f10f141385c809a14b",
+                "sha256:c0764e72b36a3dc065c155e5b22f93df465da9c39af65516fe04ed3c68c92636",
+                "sha256:c33c0d32b8594fa647d2e01dbccc303478e16fdd7cf98652d5b3ed11aa5e5c99",
+                "sha256:cbaba590180cba88cb99a5f76f90808a624f18b169b90a4abb40c1fd8c19420e",
+                "sha256:d5a1bd0e9e2031465761dfa920c16b0065ad77321d8a8c1f5ee331021fda65e9"
             ],
-            "version": "==40.0.1"
+            "version": "==40.0.2"
         },
         "dynaconf": {
             "extras": [
                 "ini"
             ],
             "hashes": [
                 "sha256:11a60bcd735f82b8a47b288f99e4ffbbd08c6c130a7be93c5d03e93fc260a5e1",
@@ -347,19 +347,19 @@
                 "sha256:8ee45429555515e1f6b185e78100aea234072576aa43ab53aefcae078162fca9",
                 "sha256:e644fdec12f7872f86c58ff790da456218b10f863970249516d60a5eaca77206"
             ],
             "version": "==2.21"
         },
         "pygments": {
             "hashes": [
-                "sha256:77a3299119af881904cd5ecd1ac6a66214b6e9bed1f2db16993b54adede64094",
-                "sha256:f7e36cffc4c517fbc252861b9a6e4644ca0e5abadf9a113c72d1358ad09b9500"
+                "sha256:8ace4d3c1dd481894b2005f560ead0f9f19ee64fe983366be1a21e171d12775c",
+                "sha256:db2db3deb4b4179f399a09054b023b6a586b76499d36965813c71aa8ed7b5fd1"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==2.15.0"
+            "version": "==2.15.1"
         },
         "pynacl": {
             "hashes": [
                 "sha256:06b8f6fa7f5de8d5d2f7573fe8c863c051225a27b61e6860fd047b1775807858",
                 "sha256:0c84947a22519e013607c9be43706dd42513f9e6ae5d39d3613ca1e142fba44d",
                 "sha256:20f42270d27e1b6a29f54032090b972d97f0a1b0948cc52392041ef7831fee93",
                 "sha256:401002a4aaa07c9414132aaed7f6836ff98f59277a234704ff66878c2ee4a0d1",
@@ -371,101 +371,101 @@
                 "sha256:e46dae94e34b085175f8abb3b0aaa7da40767865ac82c928eeb9e57e1ea8a543"
             ],
             "index": "pypi",
             "version": "==1.5.0"
         },
         "requests": {
             "hashes": [
-                "sha256:64299f4909223da747622c030b781c0d7811e359c37124b4bd368fb8c6518baa",
-                "sha256:98b1b2782e3c6c4904938b84c0eb932721069dfdb9134313beff7c83c2df24bf"
+                "sha256:10e94cc4f3121ee6da529d358cdaeaff2f1c409cd377dbc72b825852f2f7e294",
+                "sha256:239d7d4458afcb28a692cdd298d87542235f4ca8d36d03a15bfc128a6559a2f4"
             ],
             "index": "pypi",
-            "version": "==2.28.2"
+            "version": "==2.30.0"
         },
         "rich": {
             "hashes": [
-                "sha256:22b74cae0278fd5086ff44144d3813be1cedc9115bdfabbfefd86400cb88b20a",
-                "sha256:b5d573e13605423ec80bdd0cd5f8541f7844a0e71a13f74cf454ccb2f490708b"
+                "sha256:2d11b9b8dd03868f09b4fffadc84a6a8cda574e40dc90821bd845720ebb8e89c",
+                "sha256:69cdf53799e63f38b95b9bf9c875f8c90e78dd62b2f00c13a911c7a3b9fa4704"
             ],
             "index": "pypi",
-            "version": "==13.3.4"
+            "version": "==13.3.5"
         },
         "rich-click": {
             "hashes": [
                 "sha256:0fcf4d1a09029d79322dd814ab0b2e66ac183633037561881d45abae8a161d95",
                 "sha256:f8ff96693ec6e261d1544e9f7d9a5811c5ef5d74c8adb4978430fc0dac16777e"
             ],
             "index": "pypi",
             "version": "==1.6.1"
         },
         "securesystemslib": {
             "extras": [
                 "crypto"
             ],
             "hashes": [
-                "sha256:27fab4aae9adaf82530dc58f8e85a546f637d5ec5c5ef00d261689985420a70b",
-                "sha256:7ba326a41f980b3897356663144f6091531bf3d4e8333b821164526ce8e9f48d"
+                "sha256:9e6b9abe36a511d4f52c759069db8f6f650362ba82d6efc7bc7466a458b3f499",
+                "sha256:a27e519247576f2a77b97fb03267d8eeb88eba715d12da64109e845616f919c6"
             ],
             "index": "pypi",
-            "version": "==0.27.0"
+            "version": "==0.28.0"
         },
         "six": {
             "hashes": [
                 "sha256:1e61c37477a1626458e36f7b1d82aa5c9b094fa4802892072e49de9c60c4c926",
                 "sha256:8abb2f1d86890a2dfb989f9a77cfcfd3e47c2a354b01111771326f8aa26e0254"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'",
             "version": "==1.16.0"
         },
         "sqlalchemy": {
             "hashes": [
-                "sha256:07950fc82f844a2de67ddb4e535f29b65652b4d95e8b847823ce66a6d540a41d",
-                "sha256:0a865b5ec4ba24f57c33b633b728e43fde77b968911a6046443f581b25d29dd9",
-                "sha256:0b49f1f71d7a44329a43d3edd38cc5ee4c058dfef4487498393d16172007954b",
-                "sha256:13f984a190d249769a050634b248aef8991acc035e849d02b634ea006c028fa8",
-                "sha256:1b69666e25cc03c602d9d3d460e1281810109e6546739187044fc256c67941ef",
-                "sha256:1d06e119cf79a3d80ab069f064a07152eb9ba541d084bdaee728d8a6f03fd03d",
-                "sha256:246712af9fc761d6c13f4f065470982e175d902e77aa4218c9cb9fc9ff565a0c",
-                "sha256:34eb96c1de91d8f31e988302243357bef3f7785e1b728c7d4b98bd0c117dafeb",
-                "sha256:4c3020afb144572c7bfcba9d7cce57ad42bff6e6115dffcfe2d4ae6d444a214f",
-                "sha256:4f759eccb66e6d495fb622eb7f4ac146ae674d829942ec18b7f5a35ddf029597",
-                "sha256:68ed381bc340b4a3d373dbfec1a8b971f6350139590c4ca3cb722fdb50035777",
-                "sha256:6b72dccc5864ea95c93e0a9c4e397708917fb450f96737b4a8395d009f90b868",
-                "sha256:6e84ab63d25d8564d7a8c05dc080659931a459ee27f6ed1cf4c91f292d184038",
-                "sha256:734805708632e3965c2c40081f9a59263c29ffa27cba9b02d4d92dfd57ba869f",
-                "sha256:78612edf4ba50d407d0eb3a64e9ec76e6efc2b5d9a5c63415d53e540266a230a",
-                "sha256:7e472e9627882f2d75b87ff91c5a2bc45b31a226efc7cc0a054a94fffef85862",
-                "sha256:865392a50a721445156809c1a6d6ab6437be70c1c2599f591a8849ed95d3c693",
-                "sha256:8d118e233f416d713aac715e2c1101e17f91e696ff315fc9efbc75b70d11e740",
-                "sha256:8d3ece5960b3e821e43a4927cc851b6e84a431976d3ffe02aadb96519044807e",
-                "sha256:93c78d42c14aa9a9e0866eacd5b48df40a50d0e2790ee377af7910d224afddcf",
-                "sha256:95719215e3ec7337b9f57c3c2eda0e6a7619be194a5166c07c1e599f6afc20fa",
-                "sha256:9838bd247ee42eb74193d865e48dd62eb50e45e3fdceb0fdef3351133ee53dcf",
-                "sha256:aa5c270ece17c0c0e0a38f2530c16b20ea05d8b794e46c79171a86b93b758891",
-                "sha256:ac6a0311fb21a99855953f84c43fcff4bdca27a2ffcc4f4d806b26b54b5cddc9",
-                "sha256:ad5363a1c65fde7b7466769d4261126d07d872fc2e816487ae6cec93da604b6b",
-                "sha256:b3e5864eba71a3718236a120547e52c8da2ccb57cc96cecd0480106a0c799c92",
-                "sha256:bbda1da8d541904ba262825a833c9f619e93cb3fd1156be0a5e43cd54d588dcd",
-                "sha256:c6e27189ff9aebfb2c02fd252c629ea58657e7a5ff1a321b7fc9c2bf6dc0b5f3",
-                "sha256:c8239ce63a90007bce479adf5460d48c1adae4b933d8e39a4eafecfc084e503c",
-                "sha256:d209594e68bec103ad5243ecac1b40bf5770c9ebf482df7abf175748a34f4853",
-                "sha256:d5327f54a9c39e7871fc532639616f3777304364a0bb9b89d6033ad34ef6c5f8",
-                "sha256:db4bd1c4792da753f914ff0b688086b9a8fd78bb9bc5ae8b6d2e65f176b81eb9",
-                "sha256:e4780be0f19e5894c17f75fc8de2fe1ae233ab37827125239ceb593c6f6bd1e2",
-                "sha256:e4a019f723b6c1e6b3781be00fb9e0844bc6156f9951c836ff60787cc3938d76",
-                "sha256:e62c4e762d6fd2901692a093f208a6a6575b930e9458ad58c2a7f080dd6132da",
-                "sha256:e730603cae5747bc6d6dece98b45a57d647ed553c8d5ecef602697b1c1501cf2",
-                "sha256:ebc4eeb1737a5a9bdb0c24f4c982319fa6edd23cdee27180978c29cbb026f2bd",
-                "sha256:ee2946042cc7851842d7a086a92b9b7b494cbe8c3e7e4627e27bc912d3a7655e",
-                "sha256:f005245e1cb9b8ca53df73ee85e029ac43155e062405015e49ec6187a2e3fb44",
-                "sha256:f49c5d3c070a72ecb96df703966c9678dda0d4cb2e2736f88d15f5e1203b4159",
-                "sha256:f61ab84956dc628c8dfe9d105b6aec38afb96adae3e5e7da6085b583ff6ea789"
+                "sha256:03206576ca53f55b9de6e890273e498f4b2e6e687a9db9859bdcd21df5a63e53",
+                "sha256:09205893a84b6bedae0453d3f384f5d2a6499b6e45ad977549894cdcd85d8f1c",
+                "sha256:0e5501c78b5ab917f0f0f75ce7f0018f683a0a76e95f30e6561bf61c9ff69d43",
+                "sha256:10f1ff0ebe21d2cea89ead231ba3ecf75678463ab85f19ce2ce91207620737f3",
+                "sha256:1fac17c866111283cbcdb7024d646abb71fdd95f3ce975cf3710258bc55742fd",
+                "sha256:297b752d4f30350b64175bbbd57dc94c061a35f5d1dba088d0a367dbbebabc94",
+                "sha256:2a3101252f3de9a18561c1fb0a68b1ee465485990aba458d4510f214bd5a582c",
+                "sha256:32762dba51b663609757f861584a722093487f53737e76474cc6e190904dc31b",
+                "sha256:369f6564e68a9c60f0b9dde121def491e651a4ba8dcdd652a93f1cd5977cd85c",
+                "sha256:3745dee26a7ee012598577ad3b8f6e6cd50a49b2afa0cde9db668da6bf2c2319",
+                "sha256:3c053c3f4c4e45d4c8b27977647566c140d6de3f61a4e2acb92ea24cf9911c7f",
+                "sha256:4ad525b9dd17b478a2ed8580d7f2bc46b0f5889153c6b1c099729583e395b4b9",
+                "sha256:53b2c8adbcbb59732fb21a024aaa261983655845d86e3fc26a5676cec0ebaa09",
+                "sha256:5d709f43caee115b03b707b8cbbcb8b303045dd7cdc825b6d29857d71f3425ae",
+                "sha256:5e9d390727c11b9a7e583bf6770de36895c0936bddb98ae93ae99282e6428d5f",
+                "sha256:6b1fa0ffc378a7061c452cb4a1f804fad1b3b8aa8d0552725531d27941b2e3ed",
+                "sha256:6e1d50592cb24d1947c374c666add65ded7c181ec98a89ed17abbe9b8b2e2ff4",
+                "sha256:77a06b0983faf9aa48ee6219d41ade39dee16ce90857cc181dbcf6918acd234d",
+                "sha256:7eb25b981cbc9e7df9f56ad7ec4c6d77323090ca4b7147fcdc09d66535377759",
+                "sha256:85b0efe1c71459ba435a6593f54a0e39334b16ba383e8010fdb9d0127ca51ba8",
+                "sha256:87b2c2d13c3d1384859b60eabb3139e169ce68ada1d2963dbd0c7af797f16efe",
+                "sha256:8aad66215a3817a7a1d535769773333250de2653c89b53f7e2d42b677d398027",
+                "sha256:91f4b1bdc987ef85fe3a0ce5d26ac72ff8f60207b08272aa2a65494836391d69",
+                "sha256:978bee4ecbcdadf087220618409fb9be9509458df479528b70308f0599c7c519",
+                "sha256:9fe98e9d26778d7711ceee2c671741b4f54c74677668481d733d6f70747d7690",
+                "sha256:a022c588c0f413f8cddf9fcc597dbf317efeac4186d8bff9aa7f3219258348b0",
+                "sha256:a4709457f1c317e347051498b91fa2b86c4bcdebf93c84e6d121a4fc8a397307",
+                "sha256:aec5fb36b53125554ecc2285526eb5cc31b21f6cb059993c1c5ca831959de052",
+                "sha256:b6ceca432ce88ad12aab5b5896c343a1993c90b325d9193dcd055e73e18a0439",
+                "sha256:b76c2fde827522e21922418325c1b95c2d795cdecfb4bc261e4d37965199ee7f",
+                "sha256:bddfc5bd1dee5db0fddc9dab26f800c283f3243e7281bbf107200fed30125f9c",
+                "sha256:bf83700faa9642388fbd3167db3f6cbb2e88cc8367b8c22204f3f408ee782d25",
+                "sha256:c5268ec05c21e2ecf5bca09314bcaadfec01f02163088cd602db4379862958dd",
+                "sha256:d9796d5c13b2b7f05084d0ce52528cf919f9bde9e0f10672a6393a4490415695",
+                "sha256:dc67efd00ce7f428a446ce012673c03c63c5abb5dec3f33750087b8bdc173bf0",
+                "sha256:dfd6385b662aea83e63dd4db5fe116eb11914022deb1745f0b57fa8470c18ffe",
+                "sha256:e495ad05a13171fbb5d72fe5993469c8bceac42bcf6b8f9f117a518ee7fbc353",
+                "sha256:e752c34f7a2057ebe82c856698b9f277c633d4aad006bddf7af74598567c8931",
+                "sha256:f0843132168b44ca33c5e5a2046c954775dde8c580ce27f5cf2e134d0d9919e4",
+                "sha256:f30c5608c64fc9c1fa9a16277eb4784f782362566fe40ff8d283358c8f2c5fe0",
+                "sha256:f6ebadefc4331dda83c22519e1ea1e61104df6eb38abbb80ab91b0a8527a5c19"
             ],
             "index": "pypi",
-            "version": "==2.0.9"
+            "version": "==2.0.12"
         },
         "tuf": {
             "hashes": [
                 "sha256:1524b0fbd8504245f600f121daf86b8fdcb30df74410acc9655944c4868e461c",
                 "sha256:76e7f2a7aced84466865fac2a7127b6085afae51d4328af896fb46f952dd3a53"
             ],
             "index": "pypi",
@@ -477,19 +477,19 @@
                 "sha256:fb33085c39dd998ac16d1431ebc293a8b3eedd00fd4a32de0ff79002c19511b4"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==4.5.0"
         },
         "urllib3": {
             "hashes": [
-                "sha256:8a388717b9476f934a21484e8c8e61875ab60644d29b9b39e11e4b9dc1c6b305",
-                "sha256:aa751d169e23c7479ce47a0cb0da579e3ede798f994f5816a74e4f4500dcea42"
+                "sha256:61717a1095d7e155cdb737ac7bb2f4324a858a1e2e6466f6d03ff630ca68d3cc",
+                "sha256:d055c2f9d38dc53c808f6fdc8eab7360b6fdbbde02340ed25cfbcd817c62469e"
             ],
-            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5'",
-            "version": "==1.26.15"
+            "markers": "python_version >= '3.7'",
+            "version": "==2.0.2"
         }
     },
     "develop": {
         "alabaster": {
             "hashes": [
                 "sha256:1ee19aca801bbabb5ba3f5f258e4422dfa86f82f3e9cefb0859b283cdd7f62a3",
                 "sha256:a27a4a084d5e690e16e01e03ad2b2e552c61a65469419b907243193de1a84ae2"
@@ -558,19 +558,19 @@
                 "sha256:429e1a1e845c008ea6c85aa35d4b98b65d6a9763eeef3e37e92728a12d1de9d4"
             ],
             "markers": "python_version ~= '3.7'",
             "version": "==5.3.0"
         },
         "certifi": {
             "hashes": [
-                "sha256:35824b4c3a97115964b408844d64aa14db1cc518f6562e8d7261699d1350a9e3",
-                "sha256:4ad3232f5e926d6718ec31cfc1fcadfde020920e278684144551c91769c7bc18"
+                "sha256:0f0d56dc5a6ad56fd4ba36484d6cc34451e1c6548c61daad8c320169f91eddc7",
+                "sha256:c6c2e98f5c7869efca1f8916fed228dd91539f9f1b444c314c06eef02980c716"
             ],
             "markers": "python_version >= '3.6'",
-            "version": "==2022.12.7"
+            "version": "==2023.5.7"
         },
         "cfgv": {
             "hashes": [
                 "sha256:c6a0883f3917a037485059700b9e75da2464e6c27051014ad85ba6aaa5884426",
                 "sha256:f5a830efb9ce7a445376bb66ec94c638a9787422f96264c98edc6bdeed8ab736"
             ],
             "markers": "python_full_version >= '3.6.1'",
@@ -679,68 +679,68 @@
                 "sha256:4f1d9991f5acc0ca119f9d443620b77f9d6b33703e51011c16baf57afb285fc6"
             ],
             "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5, 3.6'",
             "version": "==0.4.6"
         },
         "coverage": {
             "hashes": [
-                "sha256:06ddd9c0249a0546997fdda5a30fbcb40f23926df0a874a60a8a185bc3a87d93",
-                "sha256:0743b0035d4b0e32bc1df5de70fba3059662ace5b9a2a86a9f894cfe66569013",
-                "sha256:0f3736a5d34e091b0a611964c6262fd68ca4363df56185902528f0b75dbb9c1f",
-                "sha256:1127b16220f7bfb3f1049ed4a62d26d81970a723544e8252db0efde853268e21",
-                "sha256:172db976ae6327ed4728e2507daf8a4de73c7cc89796483e0a9198fd2e47b462",
-                "sha256:182eb9ac3f2b4874a1f41b78b87db20b66da6b9cdc32737fbbf4fea0c35b23fc",
-                "sha256:1bb1e77a9a311346294621be905ea8a2c30d3ad371fc15bb72e98bfcfae532df",
-                "sha256:1fd78b911aea9cec3b7e1e2622c8018d51c0d2bbcf8faaf53c2497eb114911c1",
-                "sha256:20d1a2a76bb4eb00e4d36b9699f9b7aba93271c9c29220ad4c6a9581a0320235",
-                "sha256:21b154aba06df42e4b96fc915512ab39595105f6c483991287021ed95776d934",
-                "sha256:2c2e58e45fe53fab81f85474e5d4d226eeab0f27b45aa062856c89389da2f0d9",
-                "sha256:2c3b2803e730dc2797a017335827e9da6da0e84c745ce0f552e66400abdfb9a1",
-                "sha256:3146b8e16fa60427e03884301bf8209221f5761ac754ee6b267642a2fd354c48",
-                "sha256:344e714bd0fe921fc72d97404ebbdbf9127bac0ca1ff66d7b79efc143cf7c0c4",
-                "sha256:387065e420aed3c71b61af7e82c7b6bc1c592f7e3c7a66e9f78dd178699da4fe",
-                "sha256:3f04becd4fcda03c0160d0da9c8f0c246bc78f2f7af0feea1ec0930e7c93fa4a",
-                "sha256:4a42e1eff0ca9a7cb7dc9ecda41dfc7cbc17cb1d02117214be0561bd1134772b",
-                "sha256:4ea748802cc0de4de92ef8244dd84ffd793bd2e7be784cd8394d557a3c751e21",
-                "sha256:55416d7385774285b6e2a5feca0af9652f7f444a4fa3d29d8ab052fafef9d00d",
-                "sha256:5d0391fb4cfc171ce40437f67eb050a340fdbd0f9f49d6353a387f1b7f9dd4fa",
-                "sha256:63cdeaac4ae85a179a8d6bc09b77b564c096250d759eed343a89d91bce8b6367",
-                "sha256:72fcae5bcac3333a4cf3b8f34eec99cea1187acd55af723bcbd559adfdcb5535",
-                "sha256:7c4ed4e9f3b123aa403ab424430b426a1992e6f4c8fd3cb56ea520446e04d152",
-                "sha256:83957d349838a636e768251c7e9979e899a569794b44c3728eaebd11d848e58e",
-                "sha256:87ecc7c9a1a9f912e306997ffee020297ccb5ea388421fe62a2a02747e4d5539",
-                "sha256:8f69770f5ca1994cb32c38965e95f57504d3aea96b6c024624fdd5bb1aa494a1",
-                "sha256:8f6c930fd70d91ddee53194e93029e3ef2aabe26725aa3c2753df057e296b925",
-                "sha256:965ee3e782c7892befc25575fa171b521d33798132692df428a09efacaffe8d0",
-                "sha256:974bc90d6f6c1e59ceb1516ab00cf1cdfbb2e555795d49fa9571d611f449bcb2",
-                "sha256:981b4df72c93e3bc04478153df516d385317628bd9c10be699c93c26ddcca8ab",
-                "sha256:aa784405f0c640940595fa0f14064d8e84aff0b0f762fa18393e2760a2cf5841",
-                "sha256:ae7863a1d8db6a014b6f2ff9c1582ab1aad55a6d25bac19710a8df68921b6e30",
-                "sha256:aeae2aa38395b18106e552833f2a50c27ea0000122bde421c31d11ed7e6f9c91",
-                "sha256:b2317d5ed777bf5a033e83d4f1389fd4ef045763141d8f10eb09a7035cee774c",
-                "sha256:be19931a8dcbe6ab464f3339966856996b12a00f9fe53f346ab3be872d03e257",
-                "sha256:be9824c1c874b73b96288c6d3de793bf7f3a597770205068c6163ea1f326e8b9",
-                "sha256:c0045f8f23a5fb30b2eb3b8a83664d8dc4fb58faddf8155d7109166adb9f2040",
-                "sha256:c86bd45d1659b1ae3d0ba1909326b03598affbc9ed71520e0ff8c31a993ad911",
-                "sha256:ca0f34363e2634deffd390a0fef1aa99168ae9ed2af01af4a1f5865e362f8623",
-                "sha256:d298c2815fa4891edd9abe5ad6e6cb4207104c7dd9fd13aea3fdebf6f9b91259",
-                "sha256:d2a3a6146fe9319926e1d477842ca2a63fe99af5ae690b1f5c11e6af074a6b5c",
-                "sha256:dfd393094cd82ceb9b40df4c77976015a314b267d498268a076e940fe7be6b79",
-                "sha256:e58c0d41d336569d63d1b113bd573db8363bc4146f39444125b7f8060e4e04f5",
-                "sha256:ea3f5bc91d7d457da7d48c7a732beaf79d0c8131df3ab278e6bba6297e23c6c4",
-                "sha256:ea53151d87c52e98133eb8ac78f1206498c015849662ca8dc246255265d9c3c4",
-                "sha256:eb0edc3ce9760d2f21637766c3aa04822030e7451981ce569a1b3456b7053f22",
-                "sha256:f649dd53833b495c3ebd04d6eec58479454a1784987af8afb77540d6c1767abd",
-                "sha256:f760073fcf8f3d6933178d67754f4f2d4e924e321f4bb0dcef0424ca0215eba1",
-                "sha256:fa546d66639d69aa967bf08156eb8c9d0cd6f6de84be9e8c9819f52ad499c910",
-                "sha256:fd214917cabdd6f673a29d708574e9fbdb892cb77eb426d0eae3490d95ca7859",
-                "sha256:fff5aaa6becf2c6a1699ae6a39e2e6fb0672c2d42eca8eb0cafa91cf2e9bd312"
+                "sha256:0342a28617e63ad15d96dca0f7ae9479a37b7d8a295f749c14f3436ea59fdcb3",
+                "sha256:066b44897c493e0dcbc9e6a6d9f8bbb6607ef82367cf6810d387c09f0cd4fe9a",
+                "sha256:10b15394c13544fce02382360cab54e51a9e0fd1bd61ae9ce012c0d1e103c813",
+                "sha256:12580845917b1e59f8a1c2ffa6af6d0908cb39220f3019e36c110c943dc875b0",
+                "sha256:156192e5fd3dbbcb11cd777cc469cf010a294f4c736a2b2c891c77618cb1379a",
+                "sha256:1637253b11a18f453e34013c665d8bf15904c9e3c44fbda34c643fbdc9d452cd",
+                "sha256:292300f76440651529b8ceec283a9370532f4ecba9ad67d120617021bb5ef139",
+                "sha256:30dcaf05adfa69c2a7b9f7dfd9f60bc8e36b282d7ed25c308ef9e114de7fc23b",
+                "sha256:338aa9d9883aaaad53695cb14ccdeb36d4060485bb9388446330bef9c361c252",
+                "sha256:373ea34dca98f2fdb3e5cb33d83b6d801007a8074f992b80311fc589d3e6b790",
+                "sha256:38c0a497a000d50491055805313ed83ddba069353d102ece8aef5d11b5faf045",
+                "sha256:40cc0f91c6cde033da493227797be2826cbf8f388eaa36a0271a97a332bfd7ce",
+                "sha256:4436cc9ba5414c2c998eaedee5343f49c02ca93b21769c5fdfa4f9d799e84200",
+                "sha256:509ecd8334c380000d259dc66feb191dd0a93b21f2453faa75f7f9cdcefc0718",
+                "sha256:5c587f52c81211d4530fa6857884d37f514bcf9453bdeee0ff93eaaf906a5c1b",
+                "sha256:5f3671662dc4b422b15776cdca89c041a6349b4864a43aa2350b6b0b03bbcc7f",
+                "sha256:6599bf92f33ab041e36e06d25890afbdf12078aacfe1f1d08c713906e49a3fe5",
+                "sha256:6e8a95f243d01ba572341c52f89f3acb98a3b6d1d5d830efba86033dd3687ade",
+                "sha256:706ec567267c96717ab9363904d846ec009a48d5f832140b6ad08aad3791b1f5",
+                "sha256:780551e47d62095e088f251f5db428473c26db7829884323e56d9c0c3118791a",
+                "sha256:7ff8f3fb38233035028dbc93715551d81eadc110199e14bbbfa01c5c4a43f8d8",
+                "sha256:828189fcdda99aae0d6bf718ea766b2e715eabc1868670a0a07bf8404bf58c33",
+                "sha256:857abe2fa6a4973f8663e039ead8d22215d31db613ace76e4a98f52ec919068e",
+                "sha256:883123d0bbe1c136f76b56276074b0c79b5817dd4238097ffa64ac67257f4b6c",
+                "sha256:8877d9b437b35a85c18e3c6499b23674684bf690f5d96c1006a1ef61f9fdf0f3",
+                "sha256:8e575a59315a91ccd00c7757127f6b2488c2f914096077c745c2f1ba5b8c0969",
+                "sha256:97072cc90f1009386c8a5b7de9d4fc1a9f91ba5ef2146c55c1f005e7b5c5e068",
+                "sha256:9a22cbb5ede6fade0482111fa7f01115ff04039795d7092ed0db43522431b4f2",
+                "sha256:a063aad9f7b4c9f9da7b2550eae0a582ffc7623dca1c925e50c3fbde7a579771",
+                "sha256:a08c7401d0b24e8c2982f4e307124b671c6736d40d1c39e09d7a8687bddf83ed",
+                "sha256:a0b273fe6dc655b110e8dc89b8ec7f1a778d78c9fd9b4bda7c384c8906072212",
+                "sha256:a2b3b05e22a77bb0ae1a3125126a4e08535961c946b62f30985535ed40e26614",
+                "sha256:a66e055254a26c82aead7ff420d9fa8dc2da10c82679ea850d8feebf11074d88",
+                "sha256:aa387bd7489f3e1787ff82068b295bcaafbf6f79c3dad3cbc82ef88ce3f48ad3",
+                "sha256:ae453f655640157d76209f42c62c64c4d4f2c7f97256d3567e3b439bd5c9b06c",
+                "sha256:b5016e331b75310610c2cf955d9f58a9749943ed5f7b8cfc0bb89c6134ab0a84",
+                "sha256:b9a4ee55174b04f6af539218f9f8083140f61a46eabcaa4234f3c2a452c4ed11",
+                "sha256:bd3b4b8175c1db502adf209d06136c000df4d245105c8839e9d0be71c94aefe1",
+                "sha256:bebea5f5ed41f618797ce3ffb4606c64a5de92e9c3f26d26c2e0aae292f015c1",
+                "sha256:c10fbc8a64aa0f3ed136b0b086b6b577bc64d67d5581acd7cc129af52654384e",
+                "sha256:c2c41c1b1866b670573657d584de413df701f482574bad7e28214a2362cb1fd1",
+                "sha256:cf97ed82ca986e5c637ea286ba2793c85325b30f869bf64d3009ccc1a31ae3fd",
+                "sha256:d1f25ee9de21a39b3a8516f2c5feb8de248f17da7eead089c2e04aa097936b47",
+                "sha256:d2fbc2a127e857d2f8898aaabcc34c37771bf78a4d5e17d3e1f5c30cd0cbc62a",
+                "sha256:dc945064a8783b86fcce9a0a705abd7db2117d95e340df8a4333f00be5efb64c",
+                "sha256:ddc5a54edb653e9e215f75de377354e2455376f416c4378e1d43b08ec50acc31",
+                "sha256:e8834e5f17d89e05697c3c043d3e58a8b19682bf365048837383abfe39adaed5",
+                "sha256:ef9659d1cda9ce9ac9585c045aaa1e59223b143f2407db0eaee0b61a4f266fb6",
+                "sha256:f6f5cab2d7f0c12f8187a376cc6582c477d2df91d63f75341307fcdcb5d60303",
+                "sha256:f81c9b4bd8aa747d417407a7f6f0b1469a43b36a85748145e144ac4e8d303cb5",
+                "sha256:f99ef080288f09ffc687423b8d60978cf3a465d3f404a18d1a05474bd8575a47"
             ],
             "index": "pypi",
-            "version": "==7.2.3"
+            "version": "==7.2.5"
         },
         "distlib": {
             "hashes": [
                 "sha256:14bad2d9b04d3a36127ac97f30b12a19268f211063d8f8ee4f47108896e11b46",
                 "sha256:f35c4b692542ca110de7ef0bea44d73981caeb34ca0b9b6b2e6d7790dda8f80e"
             ],
             "version": "==0.3.6"
@@ -767,19 +767,19 @@
                 "sha256:d484c3090ba2889ae2928419117447a14daf3c1231d5e30d0aae34f354f01785"
             ],
             "markers": "python_version < '3.11'",
             "version": "==1.1.1"
         },
         "filelock": {
             "hashes": [
-                "sha256:3618c0da67adcc0506b015fd11ef7faf1b493f0b40d87728e19986b536890c37",
-                "sha256:f08a52314748335c6460fc8fe40cd5638b85001225db78c2aa01c8c0db83b318"
+                "sha256:ad98852315c2ab702aeb628412cbf7e95b7ce8c3bf9565670b4eaecf1db370a9",
+                "sha256:fc03ae43288c013d2ea83c8597001b1129db351aad9c57fe2409327916b8e718"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==3.11.0"
+            "version": "==3.12.0"
         },
         "flake8": {
             "hashes": [
                 "sha256:3833794e27ff64ea4e9cf5d410082a8b97ff1a06c16aa3d2027339cd0f1195c7",
                 "sha256:c61007e76655af75e6785a931f452915b371dc48f56efd765247c8fe68f2b181"
             ],
             "index": "pypi",
@@ -807,19 +807,19 @@
                 "sha256:81f2e6063cdbdf17ea11cffe603dfa3fba781da0c127a2814ab1eb5b864de2c0"
             ],
             "index": "pypi",
             "version": "==0.22.0"
         },
         "identify": {
             "hashes": [
-                "sha256:f0faad595a4687053669c112004178149f6c326db71ee999ae4636685753ad2f",
-                "sha256:f7a93d6cf98e29bd07663c60728e7a4057615068d7a639d132dc883b2d54d31e"
+                "sha256:0aac67d5b4812498056d28a9a512a483f5085cc28640b02b258a59dac34301d4",
+                "sha256:986dbfb38b1140e763e413e6feb44cd731faf72d1909543178aa79b0e258265d"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==2.5.22"
+            "version": "==2.5.24"
         },
         "idna": {
             "hashes": [
                 "sha256:814f528e8dead7d329833b91c5faa87d60bf71824cd12a7530b5526063d02cb4",
                 "sha256:90b77e79eaa3eba6de819a0c442c0b4ceefc341a7a2ab77d7562bf49f425c5c2"
             ],
             "markers": "python_version >= '3.5'",
@@ -1007,43 +1007,43 @@
                 "sha256:aefc51675b0b533d56bb5fd1c8c6c0522fe31896679882e1c4c63d5e4a0fccb3"
             ],
             "markers": "python_version >= '2.6'",
             "version": "==5.11.1"
         },
         "pip": {
             "hashes": [
-                "sha256:236bcb61156d76c4b8a05821b988c7b8c35bf0da28a4b614e8d6ab5212c25c6f",
-                "sha256:cd015ea1bfb0fcef59d8a286c1f8bebcb983f6317719d415dc5351efb7cd7024"
+                "sha256:0e7c86f486935893c708287b30bd050a36ac827ec7fe5e43fe7cb198dd835fba",
+                "sha256:3ef6ac33239e4027d9a5598a381b9d30880a1477e50039db2eac6e8a8f6d1b18"
             ],
             "index": "pypi",
-            "version": "==23.0.1"
+            "version": "==23.1.2"
         },
         "platformdirs": {
             "hashes": [
-                "sha256:d5b638ca397f25f979350ff789db335903d7ea010ab28903f57b27e1b16c2b08",
-                "sha256:ebe11c0d7a805086e99506aa331612429a72ca7cd52a1f0d277dc4adc20cb10e"
+                "sha256:47692bc24c1958e8b0f13dd727307cff1db103fca36399f457da8e05f222fdc4",
+                "sha256:7954a68d0ba23558d753f73437c55f89027cf8f5108c19844d4b82e5af396335"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==3.2.0"
+            "version": "==3.5.0"
         },
         "pluggy": {
             "hashes": [
                 "sha256:4224373bacce55f955a878bf9cfa763c1e360858e330072059e10bad68531159",
                 "sha256:74134bbf457f031a36d68416e1509f34bd5ccc019f0bcc952c7b909d06b37bd3"
             ],
             "markers": "python_version >= '3.1'",
             "version": "==1.0.0"
         },
         "pre-commit": {
             "hashes": [
-                "sha256:0b4210aea813fe81144e87c5a291f09ea66f199f367fa1df41b55e1d26e1e2b4",
-                "sha256:5b808fcbda4afbccf6d6633a56663fed35b6c2bc08096fd3d47ce197ac351d9d"
+                "sha256:218e9e3f7f7f3271ebc355a15598a4d3893ad9fc7b57fe446db75644543323b9",
+                "sha256:733f78c9a056cdd169baa6cd4272d51ecfda95346ef8a89bf93712706021b907"
             ],
             "index": "pypi",
-            "version": "==3.2.2"
+            "version": "==3.3.1"
         },
         "pretend": {
             "hashes": [
                 "sha256:c90eb810cde8ebb06dafcb8796f9a95228ce796531bc806e794c2f4649aa1b10",
                 "sha256:e389b12b7073604be67845dbe32bf8297360ad9a609b24846fe15d86e0b7dc01"
             ],
             "index": "pypi",
@@ -1063,19 +1063,19 @@
                 "sha256:ec8b276a6b60bd80defed25add7e439881c19e64850afd9b346283d4165fd0fd"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==3.0.1"
         },
         "pygments": {
             "hashes": [
-                "sha256:77a3299119af881904cd5ecd1ac6a66214b6e9bed1f2db16993b54adede64094",
-                "sha256:f7e36cffc4c517fbc252861b9a6e4644ca0e5abadf9a113c72d1358ad09b9500"
+                "sha256:8ace4d3c1dd481894b2005f560ead0f9f19ee64fe983366be1a21e171d12775c",
+                "sha256:db2db3deb4b4179f399a09054b023b6a586b76499d36965813c71aa8ed7b5fd1"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==2.15.0"
+            "version": "==2.15.1"
         },
         "pyproject-api": {
             "hashes": [
                 "sha256:435f46547a9ff22cf4208ee274fca3e2869aeb062a4834adfc99a4dd64af3cf9",
                 "sha256:4698a3777c2e0f6b624f8a4599131e2a25376d90fe8d146d7ac74c67c6f97c43"
             ],
             "markers": "python_version >= '3.7'",
@@ -1087,19 +1087,19 @@
                 "sha256:f271b298b97f5955d53fb12b72c1fb1948c22c1a6b70b315c54cedaca0264ef5"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==1.0.0"
         },
         "pytest": {
             "hashes": [
-                "sha256:58ecc27ebf0ea643ebfdf7fb1249335da761a00c9f955bcd922349bcb68ee57d",
-                "sha256:933051fa1bfbd38a21e73c3960cebdad4cf59483ddba7696c48509727e17f201"
+                "sha256:3799fa815351fea3a5e96ac7e503a96fa51cc9942c3753cda7651b93c1cfa362",
+                "sha256:434afafd78b1d78ed0addf160ad2b77a30d35d4bdf8af234fe621919d9ed15e3"
             ],
             "index": "pypi",
-            "version": "==7.3.0"
+            "version": "==7.3.1"
         },
         "pyyaml": {
             "hashes": [
                 "sha256:01b45c0191e6d66c470b6cf1b9531a771a83c1c4208272ead47a3ae4f2f603bf",
                 "sha256:0283c35a6a9fbf047493e3a0ce8d79ef5030852c51e9d911a27badfde0605293",
                 "sha256:055d937d65826939cb044fc8c9b08889e8c743fdc6a32b33e2390f66013e449b",
                 "sha256:07751360502caac1c067a8132d150cf3d61339af5691fe9e87803040dbc5db57",
@@ -1141,35 +1141,35 @@
                 "sha256:f84fbc98b019fef2ee9a1cb3ce93e3187a6df0b2538a651bfb890254ba9f90b5"
             ],
             "markers": "python_version >= '3.6'",
             "version": "==6.0"
         },
         "requests": {
             "hashes": [
-                "sha256:64299f4909223da747622c030b781c0d7811e359c37124b4bd368fb8c6518baa",
-                "sha256:98b1b2782e3c6c4904938b84c0eb932721069dfdb9134313beff7c83c2df24bf"
+                "sha256:10e94cc4f3121ee6da529d358cdaeaff2f1c409cd377dbc72b825852f2f7e294",
+                "sha256:239d7d4458afcb28a692cdd298d87542235f4ca8d36d03a15bfc128a6559a2f4"
             ],
             "index": "pypi",
-            "version": "==2.28.2"
+            "version": "==2.30.0"
         },
         "rich": {
             "hashes": [
-                "sha256:22b74cae0278fd5086ff44144d3813be1cedc9115bdfabbfefd86400cb88b20a",
-                "sha256:b5d573e13605423ec80bdd0cd5f8541f7844a0e71a13f74cf454ccb2f490708b"
+                "sha256:2d11b9b8dd03868f09b4fffadc84a6a8cda574e40dc90821bd845720ebb8e89c",
+                "sha256:69cdf53799e63f38b95b9bf9c875f8c90e78dd62b2f00c13a911c7a3b9fa4704"
             ],
             "index": "pypi",
-            "version": "==13.3.4"
+            "version": "==13.3.5"
         },
         "setuptools": {
             "hashes": [
-                "sha256:257de92a9d50a60b8e22abfcbb771571fde0dbf3ec234463212027a4eeecbe9a",
-                "sha256:e728ca814a823bf7bf60162daf9db95b93d532948c4c0bea762ce62f60189078"
+                "sha256:23aaf86b85ca52ceb801d32703f12d77517b2556af839621c641fca11287952b",
+                "sha256:f104fa03692a2602fa0fec6c6a9e63b6c8a968de13e17c026957dd1f53d80990"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==67.6.1"
+            "version": "==67.7.2"
         },
         "smmap": {
             "hashes": [
                 "sha256:2aba19d6a040e78d8b09de5c57e96207b09ed71d8e55ce0959eeee6c8e190d94",
                 "sha256:c840e62059cd3be204b0c9c9f74be2c09d5648eddd4580d9314c3ecde0b30936"
             ],
             "markers": "python_version >= '3.6'",
@@ -1180,19 +1180,19 @@
                 "sha256:09b16deb8547d3412ad7b590689584cd0fe25ec8db3be37788be3810cbf19cb1",
                 "sha256:c8e1716e83cc398ae16824e5572ae04e0d9fc2c6b985fb0f900f5f0c96ecba1a"
             ],
             "version": "==2.2.0"
         },
         "sphinx": {
             "hashes": [
-                "sha256:0dac3b698538ffef41716cf97ba26c1c7788dba73ce6f150c1ff5b4720786dd2",
-                "sha256:807d1cb3d6be87eb78a381c3e70ebd8d346b9a25f3753e9947e866b2786865fc"
+                "sha256:6d56a34697bb749ffa0152feafc4b19836c755d90a7c59b72bc7dfd371b9cc6b",
+                "sha256:97787ff1fa3256a3eef9eda523a63dbf299f7b47e053cfcf684a1c2a8380c912"
             ],
             "index": "pypi",
-            "version": "==6.1.3"
+            "version": "==6.2.1"
         },
         "sphinx-rtd-theme": {
             "hashes": [
                 "sha256:a0d8bd1a2ed52e0b338cbe19c4b2eef3c5e7a048769753dac6a9f059c7b641b8",
                 "sha256:f823f7e71890abe0ac6aaa6013361ea2696fc8d3e1fa798f463e82bdb77eeff2"
             ],
             "index": "pypi",
@@ -1275,54 +1275,54 @@
                 "sha256:de526c12914f0c550d15924c62d72abc48d6fe7364aa87328337a31007fe8a4f"
             ],
             "markers": "python_version >= '3.1'",
             "version": "==2.0.1"
         },
         "tox": {
             "hashes": [
-                "sha256:740f5209d0dec19451b951ee5b1cce4a207acdc7357af84dbc8ec35bcf2c454e",
-                "sha256:d4be558809d86fad13f4553976b0500352630a8fbfa39ea4b1ce3bd945ba680b"
+                "sha256:5a2eac5fb816779dfdf5cb00fecbc27eb0524e4626626bb1de84747b24cacc56",
+                "sha256:d25a2e6cb261adc489604fafd76cd689efeadfa79709965e965668d6d3f63046"
             ],
             "index": "pypi",
-            "version": "==4.4.12"
+            "version": "==4.5.1"
         },
         "types-requests": {
             "hashes": [
-                "sha256:0d580652ce903f643f8c3b494dd01d29367ea57cea0c7ad7f65cf3169092edb0",
-                "sha256:cc1aba862575019306b2ed134eb1ea994cab1c887a22e18d3383e6dd42e9789b"
+                "sha256:c6cf08e120ca9f0dc4fa4e32c3f953c3fba222bcc1db6b97695bce8da1ba9864",
+                "sha256:dec781054324a70ba64430ae9e62e7e9c8e4618c185a5cb3f87a6738251b5a31"
             ],
             "index": "pypi",
-            "version": "==2.28.11.17"
+            "version": "==2.30.0.0"
         },
         "types-urllib3": {
             "hashes": [
-                "sha256:12c744609d588340a07e45d333bf870069fc8793bcf96bae7a96d4712a42591d",
-                "sha256:c44881cde9fc8256d05ad6b21f50c4681eb20092552351570ab0a8a0653286d6"
+                "sha256:3ba3d3a8ee46e0d5512c6bd0594da4f10b2584b47a470f8422044a2ab462f1df",
+                "sha256:a1557355ce8d350a555d142589f3001903757d2d36c18a66f588d9659bbc917d"
             ],
-            "version": "==1.26.25.10"
+            "version": "==1.26.25.12"
         },
         "typing-extensions": {
             "hashes": [
                 "sha256:5cb5f4a79139d699607b3ef622a1dedafa84e115ab0024e0d9c044a9479ca7cb",
                 "sha256:fb33085c39dd998ac16d1431ebc293a8b3eedd00fd4a32de0ff79002c19511b4"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==4.5.0"
         },
         "urllib3": {
             "hashes": [
-                "sha256:8a388717b9476f934a21484e8c8e61875ab60644d29b9b39e11e4b9dc1c6b305",
-                "sha256:aa751d169e23c7479ce47a0cb0da579e3ede798f994f5816a74e4f4500dcea42"
+                "sha256:61717a1095d7e155cdb737ac7bb2f4324a858a1e2e6466f6d03ff630ca68d3cc",
+                "sha256:d055c2f9d38dc53c808f6fdc8eab7360b6fdbbde02340ed25cfbcd817c62469e"
             ],
-            "markers": "python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5'",
-            "version": "==1.26.15"
+            "markers": "python_version >= '3.7'",
+            "version": "==2.0.2"
         },
         "virtualenv": {
             "hashes": [
-                "sha256:31712f8f2a17bd06234fa97fdf19609e789dd4e3e4bf108c3da71d710651adbc",
-                "sha256:f50e3e60f990a0757c9b68333c9fdaa72d7188caa417f96af9e52407831a3b68"
+                "sha256:6abec7670e5802a528357fdc75b26b9f57d5d92f29c5462ba0fbe45feacc685e",
+                "sha256:a85caa554ced0c0afbd0d638e7e2d7b5f92d23478d05d17a76daeac8f279f924"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==20.21.0"
+            "version": "==20.23.0"
         }
     }
 }
```

### Comparing `repository_service_tuf-0.1.1a3/README.rst` & `repository_service_tuf-0.1.2a1/README.rst`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 #################################################
 Repository Service for TUF Command Line Interface
 #################################################
 
 |Tests and Lint| |Coverage|
 
-.. |Tests and Lint| image:: https://github.com/vmware/repository-service-tuf-cli/actions/workflows/ci.yml/badge.svg
-  :target: https://github.com/vmware/repository-service-tuf-cli/actions/workflows/ci.yml
-.. |Coverage| image:: https://codecov.io/gh/vmware/repository-service-tuf-cli/branch/main/graph/badge.svg
-  :target: https://codecov.io/gh/vmware/repository-service-tuf-cli
+.. |Tests and Lint| image:: https://github.com/repository-service-tuf/repository-service-tuf-cli/actions/workflows/ci.yml/badge.svg
+  :target: https://github.com/repository-service-tuf/repository-service-tuf-cli/actions/workflows/ci.yml
+.. |Coverage| image:: https://codecov.io/gh/repository-service-tuf/repository-service-tuf-cli/branch/main/graph/badge.svg
+  :target: https://codecov.io/gh/repository-service-tuf/repository-service-tuf-cli
 
 The Repository Service for TUF Command Line Interface (CLI) is a CLI Python
 application to manage the Repository Service for TUF.
 
 The CLI supports the initial setup, termed a ceremony, where the first repository
 metadata are signed and the service is configured, generating tokens to be used
 by integration (i.e., CI/CD tools).
@@ -38,13 +38,13 @@
 
 Contributing
 ============
 
 Please, visit the `Repository Service for TUF Development Guide
 <https://repository-service-tuf.readthedocs.io/en/latest/devel/index.html#development-guide>`_.
 
-Check our `CONTRIBUTING.rst <https://github.com/vmware/repository-service-tuf-cli/blob/main/CONTRIBUTING.rst>`_
+Check our `CONTRIBUTING.rst <https://github.com/repository-service-tuf/repository-service-tuf-cli/blob/main/CONTRIBUTING.rst>`_
 for more details on how to contribute to this repository.
 
 License
 =======
-`MIT <https://github.com/vmware/repository-service-tuf-cli/blob/main/LICENSE>`_
+`MIT <https://github.com/repository-service-tuf/repository-service-tuf-cli/blob/main/LICENSE>`_
```

### Comparing `repository_service_tuf-0.1.1a3/pyproject.toml` & `repository_service_tuf-0.1.2a1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -3,24 +3,23 @@
 requires = ["hatchling==0.22.0"]
 build-backend = "hatchling.build"
 
 [project]
 name = "repository-service-tuf"
 description = 'Repository Service for TUF Command Line Interface'
 readme = "README.rst"
-requires-python = ">=3.9"
+requires-python = ">=3.8"
 license = { text = "MIT"}
 keywords = []
 authors = [
   { name = "Kairo de Araujo", email = "kairo@dearaujo.nl" },
 ]
 classifiers = [
   "Development Status :: 4 - Beta",
   "Programming Language :: Python",
-  "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
```

### Comparing `repository_service_tuf-0.1.1a3/requirements-dev.txt` & `repository_service_tuf-0.1.2a1/requirements-dev.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 -i https://pypi.org/simple
 alabaster==0.7.13 ; python_version >= '3.6'
 babel==2.12.1 ; python_version >= '3.7'
 bandit==1.7.5
 black==23.3.0
 build==0.10.0
 cachetools==5.3.0 ; python_version ~= '3.7'
-certifi==2022.12.7 ; python_version >= '3.6'
+certifi==2023.5.7 ; python_version >= '3.6'
 cfgv==3.3.1 ; python_full_version >= '3.6.1'
 chardet==5.1.0 ; python_version >= '3.7'
 charset-normalizer==3.1.0 ; python_full_version >= '3.7.0'
 click==8.1.3
 colorama==0.4.6 ; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5, 3.6'
-coverage==7.2.3
+coverage==7.2.5
 distlib==0.3.6
 docutils==0.18.1 ; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4'
 editables==0.3 ; python_version >= '3.1'
 exceptiongroup==1.1.1 ; python_version < '3.11'
-filelock==3.11.0 ; python_version >= '3.7'
+filelock==3.12.0 ; python_version >= '3.7'
 flake8==6.0.0
 gitdb==4.0.10 ; python_version >= '3.7'
 gitpython==3.1.31 ; python_version >= '3.7'
 hatchling==0.22.0
-identify==2.5.22 ; python_version >= '3.7'
+identify==2.5.24 ; python_version >= '3.7'
 idna==3.4 ; python_version >= '3.5'
 imagesize==1.4.1 ; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'
 iniconfig==2.0.0 ; python_version >= '3.7'
 isort==5.12.0
 jinja2==3.1.2 ; python_version >= '3.7'
 markdown-it-py==2.2.0 ; python_version >= '3.7'
 markupsafe==2.1.2 ; python_version >= '3.7'
@@ -33,55 +33,55 @@
 mdurl==0.1.2 ; python_version >= '3.7'
 mypy==1.2.0
 mypy-extensions==1.0.0 ; python_version >= '3.5'
 nodeenv==1.7.0 ; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5, 3.6'
 packaging==23.1 ; python_version >= '3.1'
 pathspec==0.11.1 ; python_version >= '3.7'
 pbr==5.11.1 ; python_version >= '2.6'
-pip==23.0.1
-platformdirs==3.2.0 ; python_version >= '3.7'
+pip==23.1.2
+platformdirs==3.5.0 ; python_version >= '3.7'
 pluggy==1.0.0 ; python_version >= '3.1'
-pre-commit==3.2.2
+pre-commit==3.3.1
 pretend==1.0.9
 pycodestyle==2.10.0 ; python_version >= '3.6'
 pyflakes==3.0.1 ; python_version >= '3.6'
-pygments==2.15.0 ; python_version >= '3.7'
+pygments==2.15.1 ; python_version >= '3.7'
 pyproject-api==1.5.1 ; python_version >= '3.7'
 pyproject-hooks==1.0.0 ; python_version >= '3.7'
-pytest==7.3.0
+pytest==7.3.1
 pyyaml==6.0 ; python_version >= '3.6'
-requests==2.28.2
-rich==13.3.4
-setuptools==67.6.1 ; python_version >= '3.7'
+requests==2.30.0
+rich==13.3.5
+setuptools==67.7.2 ; python_version >= '3.7'
 smmap==5.0.0 ; python_version >= '3.6'
 snowballstemmer==2.2.0
-sphinx==6.1.3
+sphinx==6.2.1
 sphinx-rtd-theme==1.2.0
 sphinxcontrib-applehelp==1.0.4
 sphinxcontrib-devhelp==1.0.2
 sphinxcontrib-htmlhelp==2.0.1
 sphinxcontrib-jquery==4.1 ; python_version >= '3.1'
 sphinxcontrib-jsmath==1.0.1
 sphinxcontrib-plantuml==0.25
 sphinxcontrib-qthelp==1.0.3
 sphinxcontrib-serializinghtml==1.1.5
 stevedore==5.0.0 ; python_version >= '3.8'
 tomli==2.0.1 ; python_version >= '3.1'
-tox==4.4.12
-types-requests==2.28.11.17
-types-urllib3==1.26.25.10
+tox==4.5.1
+types-requests==2.30.0.0
+types-urllib3==1.26.25.12
 typing-extensions==4.5.0 ; python_version >= '3.7'
-urllib3==1.26.15 ; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5'
-virtualenv==20.21.0 ; python_version >= '3.7'
+urllib3==2.0.2 ; python_version >= '3.7'
+virtualenv==20.23.0 ; python_version >= '3.7'
 cffi==1.15.1
 configobj==5.0.8
-cryptography==40.0.1
+cryptography==40.0.2
 dynaconf[ini]==3.1.12
 greenlet==2.0.2 ; platform_machine == 'aarch64' or (platform_machine == 'ppc64le' or (platform_machine == 'x86_64' or (platform_machine == 'amd64' or (platform_machine == 'AMD64' or (platform_machine == 'win32' or platform_machine == 'WIN32')))))
 psycopg2==2.9.6
 pycparser==2.21
 pynacl==1.5.0
 rich-click==1.6.1
-securesystemslib[crypto]==0.27.0
+securesystemslib[crypto]==0.28.0
 six==1.16.0 ; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'
-sqlalchemy==2.0.9
+sqlalchemy==2.0.12
 tuf==2.0.0
```

### Comparing `repository_service_tuf-0.1.1a3/requirements.txt` & `repository_service_tuf-0.1.2a1/requirements.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 -i https://pypi.org/simple
-certifi==2022.12.7 ; python_version >= '3.6'
+certifi==2023.5.7 ; python_version >= '3.6'
 cffi==1.15.1
 charset-normalizer==3.1.0 ; python_full_version >= '3.7.0'
 click==8.1.3
 configobj==5.0.8
-cryptography==40.0.1
+cryptography==40.0.2
 dynaconf[ini]==3.1.12
 greenlet==2.0.2 ; platform_machine == 'aarch64' or (platform_machine == 'ppc64le' or (platform_machine == 'x86_64' or (platform_machine == 'amd64' or (platform_machine == 'AMD64' or (platform_machine == 'win32' or platform_machine == 'WIN32')))))
 idna==3.4 ; python_version >= '3.5'
 isort==5.12.0
 markdown-it-py==2.2.0 ; python_version >= '3.7'
 mdurl==0.1.2 ; python_version >= '3.7'
 psycopg2==2.9.6
 pycparser==2.21
-pygments==2.15.0 ; python_version >= '3.7'
+pygments==2.15.1 ; python_version >= '3.7'
 pynacl==1.5.0
-requests==2.28.2
-rich==13.3.4
+requests==2.30.0
+rich==13.3.5
 rich-click==1.6.1
-securesystemslib[crypto]==0.27.0
+securesystemslib[crypto]==0.28.0
 six==1.16.0 ; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3'
-sqlalchemy==2.0.9
+sqlalchemy==2.0.12
 tuf==2.0.0
 typing-extensions==4.5.0 ; python_version >= '3.7'
-urllib3==1.26.15 ; python_version >= '2.7' and python_version not in '3.0, 3.1, 3.2, 3.3, 3.4, 3.5'
+urllib3==2.0.2 ; python_version >= '3.7'
```

### Comparing `repository_service_tuf-0.1.1a3/tox.ini` & `repository_service_tuf-0.1.2a1/tox.ini`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tox]
 isolated_build = true
-envlist = py310,py311,lint,typing,requirements,test
+envlist = py38,py39,py310,py311,lint,typing,requirements,test
 skipsdist = true
 
 
 [flake8]
 exclude = repository_service_tuf/__init__.py,venv,.venv,settings.py,.git,.tox,dist,docs,*lib/python*,*egg,build,tools
 
 [testenv]
@@ -50,9 +50,11 @@
 commands =
     plantuml -o ../source/_static/ -tpng docs/diagrams/*.puml
 	sphinx-apidoc -o  docs/source/devel/ repository_service_tuf
 	sphinx-build -E -W -b html docs/source docs/build/html
 
 [gh-actions]
 python =
+    3.8: py38,pep8,lint,typing,requirements,test,docs
+    3.9: py39,pep8,lint,typing,requirements,test,docs
     3.10: py310,pep8,lint,typing,requirements,test,docs
     3.11: py311,pep8,lint,typing,requirements,test,docs
```

### Comparing `repository_service_tuf-0.1.1a3/.github/ISSUE_TEMPLATE/bug.yml` & `repository_service_tuf-0.1.2a1/.github/ISSUE_TEMPLATE/bug.yml`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.1a3/.github/ISSUE_TEMPLATE/other.yml` & `repository_service_tuf-0.1.2a1/.github/ISSUE_TEMPLATE/other.yml`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.1a3/.github/ISSUE_TEMPLATE/task.yml` & `repository_service_tuf-0.1.2a1/.github/ISSUE_TEMPLATE/task.yml`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.1a3/.github/PULL_REQUEST_TEMPLATE/pr.yml` & `repository_service_tuf-0.1.2a1/.github/PULL_REQUEST_TEMPLATE/pr.yml`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.1a3/.github/workflows/cd.yml` & `repository_service_tuf-0.1.2a1/.github/workflows/cd.yml`

 * *Files 26% similar despite different names*

```diff
@@ -7,15 +7,15 @@
       - v*
 
 permissions:
   contents: write
 
 jobs:
   functional-latest:
-    uses: vmware/repository-service-tuf/.github/workflows/functional.yml@main
+    uses: repository-service-tuf/repository-service-tuf/.github/workflows/functional.yml@main
     with:
       worker_version: latest
       api_version: latest
       cli_version: dev
 
   build:
     name: Build
@@ -26,26 +26,29 @@
     steps:
       - name: Checkout release tag
         uses: actions/checkout@8e5e7e5ab8b370d6c329ec480221332ada57f0ab
         with:
           ref: ${{ github.event.workflow_run.head_branch }}
 
       - name: Set up Python
-        uses: actions/setup-python@d27e3f3d7c64b4bbf8e4abfb9b63b83e846e0435
+        uses: actions/setup-python@57ded4d7d5e986d7296eab16560982c6dd7c923b
         with:
           python-version: '3.x'
 
       - name: Install build dependency
-        run: python3 -m pip install --upgrade pip build
+        run: python3 -m pip install --upgrade pip build twine
 
       - name: Build binary wheel and source tarball
         run: python3 -m build --sdist --wheel --outdir dist/ .
 
+      - name: Check distribution's long description rendering on PyPI
+        run: twine check dist/*
+
       - id: gh-release
-        name: Publish GitHub release candiate
+        name: Publish GitHub release candidate
         uses: softprops/action-gh-release@de2c0eb89ae2a093876385947365aca7b0e5f844
         with:
           name: ${{ github.ref_name }}-rc
           tag_name: ${{ github.ref }}
           body: "Release waiting for review..."
           files: dist/*
 
@@ -59,14 +62,17 @@
           path: dist
 
   release:
     name: Release
     runs-on: ubuntu-latest
     needs: build
     environment: release
+    permissions:
+      contents: write  # to update GitHub releases
+      id-token: write  # IMPORTANT: this permission is mandatory for trusted publishing
     steps:
       - name: Fetch build artifacts
         uses: actions/download-artifact@9bc31d5ccc31df68ecc42ccf4149144866c47d8a
         with:
           name: build-artifacts
           path: dist
 
@@ -75,8 +81,25 @@
         with:
           script: |
             await github.rest.repos.updateRelease({
               owner: context.repo.owner,
               repo: context.repo.repo,
               release_id: '${{ needs.build.outputs.release_id }}',
               name: '${{ github.ref_name }}',
-            })
+            })
+
+      - name: Publish distribution 📦 to Test PyPI
+        env:
+          name: testpypi
+          url: https://pypi.org/p/repository-service-tuf
+        if: github.repository == 'repository-service-tuf/repository-service-tuf-cli'
+        uses: pypa/gh-action-pypi-publish@a56da0b891b3dc519c7ee3284aff1fad93cc8598
+        with:
+          repository-url: https://test.pypi.org/legacy/
+
+      - name: Publish binary wheel and source tarball 📦 on PyPI
+        env:
+          name: pypi
+          url: https://pypi.org/p/repository-service-tuf
+        # Only attempt PyPI upload in upstream repository
+        if: github.repository == 'repository-service-tuf/repository-service-tuf-cli'
+        uses: pypa/gh-action-pypi-publish@a56da0b891b3dc519c7ee3284aff1fad93cc8598
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `repository_service_tuf-0.1.1a3/docs/Makefile` & `repository_service_tuf-0.1.2a1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.1a3/docs/make.bat` & `repository_service_tuf-0.1.2a1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.1a3/docs/diagrams/repository-service-tuf-cli-C1.puml` & `repository_service_tuf-0.1.2a1/docs/diagrams/repository-service-tuf-cli-C1.puml`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.1a3/docs/diagrams/repository-service-tuf-cli-C2.puml` & `repository_service_tuf-0.1.2a1/docs/diagrams/repository-service-tuf-cli-C2.puml`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.1a3/docs/diagrams/repository-service-tuf-cli-C3.puml` & `repository_service_tuf-0.1.2a1/docs/diagrams/repository-service-tuf-cli-C3.puml`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.1a3/docs/source/conf.py` & `repository_service_tuf-0.1.2a1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.1a3/docs/source/_static/repository-service-tuf-cli-C1.png` & `repository_service_tuf-0.1.2a1/docs/source/_static/repository-service-tuf-cli-C1.png`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.1a3/docs/source/_static/repository-service-tuf-cli-C2.png` & `repository_service_tuf-0.1.2a1/docs/source/_static/repository-service-tuf-cli-C2.png`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.1a3/docs/source/_static/repository-service-tuf-cli-C3.png` & `repository_service_tuf-0.1.2a1/docs/source/_static/repository-service-tuf-cli-C3.png`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.1a3/docs/source/devel/design.rst` & `repository_service_tuf-0.1.2a1/docs/source/devel/design.rst`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.1a3/docs/source/devel/repository_service_tuf.cli.admin.rst` & `repository_service_tuf-0.1.2a1/docs/source/devel/repository_service_tuf.cli.admin.rst`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.1a3/docs/source/devel/repository_service_tuf.helpers.rst` & `repository_service_tuf-0.1.2a1/docs/source/devel/repository_service_tuf.helpers.rst`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.1a3/docs/source/guide/index.rst` & `repository_service_tuf-0.1.2a1/docs/source/guide/index.rst`

 * *Files 3% similar despite different names*

```diff
@@ -218,14 +218,15 @@
     The RSTUF Worker uses this key during the process of managing the metadata.
 
     Note: the ceremony process won't show any password or key content.
 
     Choose 1/1 ONLINE key type [ed25519/ecdsa/rsa] (ed25519):
     Enter 1/1 the ONLINE`s private key path: tests/files/online.key
     Enter 1/1 the ONLINE`s private key password:
+    [Optional] Give a name/tag to the key:
     ✅ Key 1/1 Verified
 
     Step 3: Validate the information/settings
     .........................................
 
     After confirming all details, the initial payload for bootstrap will be
     complete (without the offline keys).
@@ -254,19 +255,21 @@
     personally.
 
     Note: the ceremony process won't show any password or key content.
 
     Choose 1/2 root key type [ed25519/ecdsa/rsa] (ed25519):
     Enter 1/2 the root`s private key path: tests/files/JanisJoplin.key
     Enter 1/2 the root`s private key password:
+    [Optional] Give a name/tag to the key:
     ✅ Key 1/2 Verified
 
     Choose 2/2 root key type [ed25519/ecdsa/rsa] (ed25519):
     Enter 2/2 the root`s private key path: tests/files/JimiHendrix.key
     Enter 2/2 the root`s private key password:
+    [Optional] Give a name/tag to the key:
     ✅ Key 2/2 Verified
 
 Step 4: Validate Configuration
 ..............................
 
 .. code::
```

### Comparing `repository_service_tuf-0.1.1a3/repository_service_tuf/constants.py` & `repository_service_tuf-0.1.2a1/repository_service_tuf/constants.py`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.1a3/repository_service_tuf/cli/__init__.py` & `repository_service_tuf-0.1.2a1/repository_service_tuf/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.1a3/repository_service_tuf/cli/admin/ceremony.py` & `repository_service_tuf-0.1.2a1/repository_service_tuf/cli/admin/ceremony.py`

 * *Files 2% similar despite different names*

```diff
@@ -244,41 +244,43 @@
     },
     services=ServiceSettings(),
     number_of_keys={Roles.ROOT: 2, Roles.TARGETS: 1},
     threshold={
         Roles.ROOT: 1,
         Roles.TARGETS: 1,
     },
-    root_keys=[],
+    root_keys={},
     online_key=RSTUFKey(),
 )
 
 
 def _key_already_in_use(key: Dict[str, Any]) -> bool:
     """Check if a key is duplicated, used in a role or the online_key"""
     if key is None:
         return False
 
-    keyid = key.get("keyid")
+    keyid = key["keyid"]
     if keyid == setup.online_key.key.get("keyid"):
         return True
 
-    for root_key in setup.root_keys:
-        if keyid == root_key.key.get("keyid"):
-            return True
+    if setup.root_keys.get(keyid) is not None:
+        return True
 
     return False
 
 
 def _load_key(
-    filepath: str, keytype: str, password: Optional[str]
+    filepath: str, keytype: str, password: Optional[str], name: str
 ) -> RSTUFKey:
     try:
         key = import_privatekey_from_file(filepath, keytype, password)
-        return RSTUFKey(key=key, key_path=filepath)
+        # Make sure name cannot be an empty string.
+        # If no name is given use first 7 letters of the keyid.
+        name = name if name != "" else key["keyid"][:7]
+        return RSTUFKey(key=key, key_path=filepath, name=name)
     except CryptoError as err:
         return RSTUFKey(
             error=(
                 f":cross_mark: [red]Failed[/]: {str(err)} Check the"
                 " password, type, etc"
             )
         )
@@ -433,15 +435,20 @@
         )
 
         password = click.prompt(
             f"Enter {key_count}/{number_of_keys} the "
             f"{role}`s private key password",
             hide_input=True,
         )
-        role_key: RSTUFKey = _load_key(filepath, key_type, password)
+        name = prompt.Prompt.ask(
+            "[Optional] Give a name/tag to the key",
+            default="",
+            show_default=False,
+        )
+        role_key: RSTUFKey = _load_key(filepath, key_type, password, name)
 
         if role_key.error:
             console.print(role_key.error)
             try_again = prompt.Confirm.ask("Try again?", default="y")
             if try_again:
                 continue
             else:
@@ -479,28 +486,30 @@
         keys_table = table.Table(box=box.MINIMAL)
         if path is True:
             keys_table.add_column(
                 "path", justify="right", style="cyan", no_wrap=True
             )
         keys_table.add_column("type", justify="center")
         keys_table.add_column("verified", justify="center")
+        keys_table.add_column("name/tag", justify="center")
         keys_table.add_column("id", justify="center")
 
         return keys_table
 
     # Validations
     #
     # Online key validation
     while True:
         online_key_table = _init_summary_table("ONLINE KEY SUMMARY")
         keys_table = _init_keys_table()
         keys_table.add_row(
             f"[yellow]{setup.online_key.key_path}[/]",
             "[green]Online[/]",
             ":white_heavy_check_mark:",
+            f"[yellow]{setup.online_key.name}",
             f"[yellow]{setup.online_key.key.get('keyid')}[/]",
         )
 
         online_key_table.add_row(keys_table)
         console.print("\n", online_key_table)
 
         confirm_config = prompt.Confirm.ask(
@@ -519,19 +528,20 @@
     for role in Roles:
         while True:
             role_table = _init_summary_table("ROLE SUMMARY")
             role_table.add_column("KEYS", justify="center", vertical="middle")
 
             if role == Roles.ROOT:
                 keys_table = _init_keys_table()
-                for key in setup.root_keys:
+                for key in setup.root_keys.values():
                     keys_table.add_row(
                         f"[yellow]{key.key_path}[/]",
                         "[bright_blue]Offline[/]",
                         ":white_heavy_check_mark:",
+                        f"[yellow]{key.name}",
                         key.key.get("keyid"),
                     )
 
                 role_table.add_row(
                     (
                         f"Role: [cyan]{role.value}[/]"
                         f"\nNumber of Keys: [yellow]{len(setup.root_keys)}[/]"
@@ -544,15 +554,16 @@
                 )
             else:
                 keys_table = _init_keys_table(path=False)
                 if setup.online_key.key is not None:
                     keys_table.add_row(
                         "[green]Online[/]",
                         ":white_heavy_check_mark:",
-                        setup.online_key.key.get("keyid"),
+                        f"[yellow]{setup.online_key.name}",
+                        key.key.get("keyid"),
                     )
                 role_table.add_row(
                     (
                         f"Role: [cyan]{role.value}[/]"
                         f"\nRole Expiration: [yellow]{setup.expiration[role]} "
                         "[/]days"
                     ),
@@ -585,15 +596,15 @@
                 # if root, reconfigure also the keys
                 if role == Roles.ROOT:
                     setup.root_keys.clear()
                     for key in _configure_keys(
                         role.value,
                         setup.number_of_keys[Roles.ROOT],
                     ):
-                        setup.root_keys.append(key)
+                        setup.root_keys[key.key["keyid"]] = key
             else:
                 break
 
 
 def _run_ceremony_steps(save: bool) -> Dict[str, Any]:
     console.print(markdown.Markdown(CEREMONY_INTRO), width=100)
 
@@ -623,22 +634,21 @@
     )
     if start_ceremony is False:
         raise click.ClickException("Ceremony aborted.")
 
     # STEP 2: configure the online key (one)
     console.print(markdown.Markdown(STEP_2), width=100)
     for key in _configure_keys("ONLINE", number_of_keys=1):
-        setup.online_key.key = key.key
-        setup.online_key.key_path = key.key_path
+        setup.online_key = key
 
     # STEP 3: load the root keys
     console.print(markdown.Markdown(STEP_3), width=100)
     root = Roles.ROOT.value
     for key in _configure_keys(root, setup.number_of_keys[Roles.ROOT]):
-        setup.root_keys.append(key)
+        setup.root_keys[key.key["keyid"]] = key
 
     # STEP 4: user validation
     console.print(markdown.Markdown(STEP_4), width=100)
     _run_user_validation()
 
     tuf_management = TUFManagement(setup, save)
     metadata = tuf_management.initialize_metadata()
```

### Comparing `repository_service_tuf-0.1.1a3/repository_service_tuf/cli/admin/import_targets.py` & `repository_service_tuf-0.1.2a1/repository_service_tuf/cli/admin/import_targets.py`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.1a3/repository_service_tuf/cli/admin/login.py` & `repository_service_tuf-0.1.2a1/repository_service_tuf/cli/admin/login.py`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.1a3/repository_service_tuf/cli/admin/token.py` & `repository_service_tuf-0.1.2a1/repository_service_tuf/cli/admin/token.py`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.1a3/repository_service_tuf/cli/key/generate_key.py` & `repository_service_tuf-0.1.2a1/repository_service_tuf/cli/key/generate_key.py`

 * *Files 14% similar despite different names*

```diff
@@ -58,25 +58,19 @@
             f"Do you want to [red]overwrite[/] the existing '{filename}' file?"
         )
         if overwrite is False:
             raise click.ClickException("Key creation aborted.")
 
     password = _verify_password(filename)
 
-    match key_type:
-        case KeyType.KEY_TYPE_ED25519.value:
-            _generate_and_write_ed25519_keypair(
-                password=password, filepath=filename
-            )
-
-        case KeyType.KEY_TYPE_ECDSA.value:
-            _generate_and_write_ecdsa_keypair(
-                password=password, filepath=filename
-            )
-
-        case KeyType.KEY_TYPE_RSA.value:
-            _generate_and_write_rsa_keypair(
-                password=password, filepath=filename
-            )
-
-        case _:
-            raise ValueError(f"Key type `{key_type}` is not supported!")
+    if key_type == KeyType.KEY_TYPE_ED25519.value:
+        _generate_and_write_ed25519_keypair(
+            password=password, filepath=filename
+        )
+    elif key_type == KeyType.KEY_TYPE_ECDSA.value:
+        _generate_and_write_ecdsa_keypair(password=password, filepath=filename)
+    elif key_type == KeyType.KEY_TYPE_RSA.value:
+        _generate_and_write_rsa_keypair(password=password, filepath=filename)
+    else:  # pragma: no cover
+        # Current click configuration will never trigger this case, adding
+        # this as a fail-safe if we add new key-types
+        raise ValueError(f"Key type `{key_type}` is not supported!")
```

### Comparing `repository_service_tuf-0.1.1a3/repository_service_tuf/helpers/api_client.py` & `repository_service_tuf-0.1.2a1/repository_service_tuf/helpers/api_client.py`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.1a3/repository_service_tuf/helpers/tuf.py` & `repository_service_tuf-0.1.2a1/repository_service_tuf/helpers/tuf.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,24 +33,25 @@
         return asdict(self)
 
 
 @dataclass
 class RSTUFKey:
     key: dict = field(default_factory=dict)
     key_path: Optional[str] = None
+    name: Optional[str] = None
     error: Optional[str] = None
 
 
 @dataclass
 class BootstrapSetup:
     expiration: Dict[Roles, int]
     services: ServiceSettings
     number_of_keys: Dict[Literal[Roles.ROOT, Roles.TARGETS], int]
     threshold: Dict[Literal[Roles.ROOT, Roles.TARGETS], int]
-    root_keys: List[RSTUFKey] = field(default_factory=list)
+    root_keys: Dict[str, RSTUFKey] = field(default_factory=Dict)
     online_key: RSTUFKey = field(default_factory=RSTUFKey)
 
     def to_dict(self):
         return {
             "expiration": {k.value: v for k, v in self.expiration.items()},
             "services": self.services.to_dict(),
         }
@@ -65,15 +66,17 @@
         self.setup = setup
         self.save = save
         self.repository_metadata: Dict[str, Metadata] = {}
 
     def _signers(self, role: Roles) -> List[Signer]:
         """Returns all Signers from the settings for a specific role name"""
         if role == Roles.ROOT:
-            return [SSlibSigner(key.key) for key in self.setup.root_keys]
+            return [
+                SSlibSigner(key.key) for key in self.setup.root_keys.values()
+            ]
         else:
             return [SSlibSigner(self.setup.online_key.key)]
 
     def _sign(self, role: Metadata, role_name: str) -> None:
         """Re-signs metadata with role-specific key from global key store.
         The metadata role type is used as default key id. This is only allowed
         for top-level roles.
@@ -153,14 +156,26 @@
         self._verify_correct_keys_usage(root_metadata.signed)
 
         metadata_type = root_metadata.signed.type
         self._bump_expiry(root_metadata, metadata_type)
         self._sign(root_metadata, metadata_type)
         self._add_payload(root_metadata, metadata_type)
 
+    def _setup_key_name(self, key: Key, role: str):
+        rstuf_key: Optional[RSTUFKey]
+        if role == Roles.ROOT.value:
+            rstuf_key = self.setup.root_keys.get(key.keyid)
+
+        else:
+            if self.setup.online_key.key["keyid"] == key.keyid:
+                rstuf_key = self.setup.online_key
+
+        if rstuf_key is not None and rstuf_key.name is not None:
+            key.unrecognized_fields["name"] = rstuf_key.name
+
     def initialize_metadata(self) -> Dict[str, Metadata]:
         """
         Creates TUF top-level role metadata (root, targets, snapshot and
         timestamp).
         """
         # Populate public key store, and define trusted signing keys and
         # required signature thresholds for each top-level role in 'root'.
@@ -183,15 +198,15 @@
                 raise ValueError(
                     f"not enough keys ({len(signers)}) for "
                     f"signing threshold '{threshold}'"
                 )
             add_key_args[role_name] = []
             roles[role_name] = Role([], threshold)
             for signer in signers:
-                add_key_args[role_name].append(
-                    Key.from_securesystemslib_key(signer.key_dict)
-                )
+                key = Key.from_securesystemslib_key(signer.key_dict)
+                self._setup_key_name(key, role_name)
+                add_key_args[role_name].append(key)
 
         self._prepare_root_and_add_it_to_payload(roles, add_key_args)
         self._validate_root_payload_exist()
 
         return self.repository_metadata
```

### Comparing `repository_service_tuf-0.1.1a3/tests/conftest.py` & `repository_service_tuf-0.1.2a1/tests/conftest.py`

 * *Files 7% similar despite different names*

```diff
@@ -45,15 +45,15 @@
         },
         services=ServiceSettings(),
         number_of_keys={Roles.ROOT: 2, Roles.TARGETS: 1},
         threshold={
             Roles.ROOT: 1,
             Roles.TARGETS: 1,
         },
-        root_keys=[],
+        root_keys={},
         online_key=RSTUFKey(),
     )
 
     return setup
 
 
 @pytest.fixture
@@ -77,23 +77,26 @@
         "",  # What is the metadata expiration for the timestamp role?(Days) (365)?  # noqa
         "",  # What is the metadata expiration for the bins role?(Days) (365)?
         "Y",  # Ready to start loading the keys? Passwords will be required for keys [y/n]  # noqa
     ]
     input_step2 = [
         "",  # Choose 1/1 ONLINE key type [ed25519/ecdsa/rsa]
         "tests/files/key_storage/online.key",  # Enter 1/1 the ONLINE`s private key path  # noqa
-        "strongPass",  # Enter 1/1 the ONLINE`s private key password
+        "strongPass",  # Enter 1/1 the ONLINE`s private key password,
+        "",  # [Optional] Give a name/tag to the key:
     ]
     input_step3 = [
         "",  # Choose 1/2 root key type [ed25519/ecdsa/rsa]
-        "tests/files/key_storage/JanisJoplin.key",  # Enter 1/2 the root`s private key pathh  # noqa
+        "tests/files/key_storage/JanisJoplin.key",  # Enter 1/2 the root`s private key path  # noqa
         "strongPass",  # Enter 1/2 the root`s private key password
+        "",  # [Optional] Give a name/tag to the key:
         "",  # Choose 2/2 root key type [ed25519/ecdsa/rsa]
-        "tests/files/key_storage/JimiHendrix.key",  # Enter 2/2 the root`s private key pathh  # noqa
+        "tests/files/key_storage/JimiHendrix.key",  # Enter 2/2 the root`s private key path  # noqa
         "strongPass",  # Enter 2/2 the root`s private key password:
+        "",  # [Optional] Give a name/tag to the key:
     ]
     input_step4 = [
         "y",  # Is the online key configuration correct? [y/n]
         "y",  # Is the root configuration correct? [y/n]
         "y",  # Is the targets configuration correct? [y/n]
         "y",  # Is the snapshot configuration correct? [y/n]
         "y",  # Is the timestamp configuration correct? [y/n]
```

### Comparing `repository_service_tuf-0.1.1a3/tests/test_tuf_repository_service.py` & `repository_service_tuf-0.1.2a1/tests/test_tuf_repository_service.py`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.1a3/tests/files/key_storage/JanisJoplin.key` & `repository_service_tuf-0.1.2a1/tests/files/key_storage/JanisJoplin.key`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.1a3/tests/files/key_storage/JimiHendrix.key` & `repository_service_tuf-0.1.2a1/tests/files/key_storage/JimiHendrix.key`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.1a3/tests/files/key_storage/online-rsa.key` & `repository_service_tuf-0.1.2a1/tests/files/key_storage/online-rsa.key`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.1a3/tests/files/key_storage/online-rsa.pub` & `repository_service_tuf-0.1.2a1/tests/files/key_storage/online-rsa.pub`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.1a3/tests/files/key_storage/online.key` & `repository_service_tuf-0.1.2a1/tests/files/key_storage/online.key`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.1a3/tests/unit/cli/test__init__.py` & `repository_service_tuf-0.1.2a1/tests/unit/cli/test__init__.py`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.1a3/tests/unit/cli/admin/test_ceremony.py` & `repository_service_tuf-0.1.2a1/tests/unit/cli/admin/test_ceremony.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 class TestCeremonyFunctions:
     def test__key_already_in_use(self, test_setup):
         ceremony.setup = test_setup
         result = ceremony._key_already_in_use({"keyid": "ema"})
         assert result is False
 
     def test__key_already_in_use_exists_in_role(self, test_setup):
-        test_setup.root_keys = [ceremony.RSTUFKey(key={"keyid": "ema"})]
+        test_setup.root_keys["ema"] = ceremony.RSTUFKey(key={"keyid": "ema"})
         ceremony.setup = test_setup
         result = ceremony._key_already_in_use({"keyid": "ema"})
         assert result is True
 
     def test__key_already_in_use_exists_in_online_key(self, test_setup):
         test_setup.online_key = ceremony.RSTUFKey(key={"keyid": "ema"})
 
@@ -32,30 +32,30 @@
         monkeypatch.setattr(
             ceremony,
             "import_privatekey_from_file",
             pretend.call_recorder(lambda *a: {"keyid": "ema"}),
         )
 
         result = ceremony._load_key(
-            "/p/key", KeyType.KEY_TYPE_ED25519.value, "pwd"
+            "/p/key", KeyType.KEY_TYPE_ED25519.value, "pwd", None
         )
         assert result == ceremony.RSTUFKey({"keyid": "ema"}, "/p/key", None)
         assert ceremony.import_privatekey_from_file.calls == [
             pretend.call("/p/key", KeyType.KEY_TYPE_ED25519.value, "pwd")
         ]
 
     def test__load_key_CryptoError(self, monkeypatch):
         monkeypatch.setattr(
             ceremony,
             "import_privatekey_from_file",
             pretend.raiser(ceremony.CryptoError("wrong password")),
         )
 
         result = ceremony._load_key(
-            "/p/key", KeyType.KEY_TYPE_ED25519.value, "pwd"
+            "/p/key", KeyType.KEY_TYPE_ED25519.value, "pwd", None
         )
         assert result == ceremony.RSTUFKey(
             {},
             None,
             error=(
                 ":cross_mark: [red]Failed[/]: wrong password Check the "
                 "password, type, etc"
@@ -65,15 +65,15 @@
     def test__load_key_OSError(self, monkeypatch):
         monkeypatch.setattr(
             ceremony,
             "import_privatekey_from_file",
             pretend.raiser(OSError("permission denied")),
         )
         result = ceremony._load_key(
-            "/p/key", KeyType.KEY_TYPE_ED25519.value, "pwd"
+            "/p/key", KeyType.KEY_TYPE_ED25519.value, "pwd", None
         )
         assert result == ceremony.RSTUFKey(
             {}, None, error=":cross_mark: [red]Failed[/]: permission denied"
         )
 
     def test__send_bootstrap(self, test_context):
         test_context["settings"].SERVER = "http://fake-rstuf"
@@ -392,18 +392,20 @@
         input_step1, input_step2, input_step3, input_step4 = test_inputs
 
         # overwrite the input_step2
         input_step2 = [
             "",  # Choose 1/1 ONLINE key type [ed25519/ecdsa/rsa]
             "tests/files/key_storage/online.key",  # Enter 1/1 the ONLINE`s private key path  # noqa
             "wrong password",  # Enter 1/1 the ONLINE`s private key password
+            "",  # [Optional] Give a name/tag to the key
             "y",  # Try again?
             "",  # Choose 1/1 ONLINE key type [ed25519/ecdsa/rsa]
             "tests/files/key_storage/online.key",  # Enter 1/1 the ONLINE`s private key path  # noqa
             "strongPass",  # Enter 1/1 the ONLINE`s private key password
+            "",  # [Optional] Give a name/tag to the key
         ]
 
         test_result = client.invoke(
             ceremony.ceremony,
             input="\n".join(
                 input_step1 + input_step2 + input_step3 + input_step4
             ),
@@ -422,14 +424,15 @@
         input_step1, input_step2, input_step3, input_step4 = test_inputs
 
         # overwrite the input_step2
         input_step2 = [
             "",  # Choose 1/1 ONLINE key type [ed25519/ecdsa/rsa]
             "tests/files/key_storage/online.key",  # Enter 1/1 the ONLINE`s private key path  # noqa
             "wrong password",  # Enter 1/1 the ONLINE`s private key password
+            "",  # [Optional] Give a name/tag to the key
             "n",  # Try again?
         ]
 
         test_result = client.invoke(
             ceremony.ceremony,
             input="\n".join(
                 input_step1 + input_step2 + input_step3 + input_step4
@@ -438,31 +441,70 @@
         )
 
         assert test_result.exit_code == 1, test_result.output
         assert "Required key not validated." in test_result.output
         # passwords not shown in output
         assert "strongPass" not in test_result.output
 
+    def test_ceremony_key_with_name(
+        self, client, test_context, test_inputs, test_setup
+    ):
+        # Test a case when the user gives custom names to the keys.
+        ceremony.setup = test_setup
+        input_step1, input_step2, input_step3, input_step4 = test_inputs
+        input_step2 = [
+            "",  # Choose 1/1 ONLINE key type [ed25519/ecdsa/rsa]
+            "tests/files/key_storage/online.key",  # Enter 1/1 the ONLINE`s private key path  # noqa
+            "strongPass",  # Enter 1/1 the ONLINE`s private key password,
+            "Online key",  # [Optional] Give a name/tag to the key
+        ]
+        input_step3 = [
+            "",  # Choose 1/2 root key type [ed25519/ecdsa/rsa]
+            "tests/files/key_storage/JanisJoplin.key",  # Enter 1/2 the root`s private key path  # noqa
+            "strongPass",  # Enter 1/2 the root`s private key password
+            "Martin's Key",  # [Optional] Give a name/tag to the key
+            "",  # Choose 2/2 root key type [ed25519/ecdsa/rsa]
+            "tests/files/key_storage/JimiHendrix.key",  # Enter 2/2 the root`s private key path  # noqa
+            "strongPass",  # Enter 2/2 the root`s private key password:
+            "Steven's Key",  # [Optional] Give a name/tag to the key
+        ]
+
+        test_result = client.invoke(
+            ceremony.ceremony,
+            input="\n".join(
+                input_step1 + input_step2 + input_step3 + input_step4
+            ),
+            obj=test_context,
+        )
+
+        assert test_result.exit_code == 0, test_result.output
+        assert "Ceremony done. 🔐 🎉." in test_result.output
+        # passwords not shown in output
+        assert "strongPass" not in test_result.output
+
     def test_ceremony_key_duplicated_try_again_yes(
         self, client, test_context, test_inputs, test_setup
     ):
         ceremony.setup = test_setup
         input_step1, input_step2, input_step3, input_step4 = test_inputs
 
         # overwrite the input_step3 with same key in input_step2 (online key)
         input_step3 = [
             "",  # Choose 1/2 root key type [ed25519/ecdsa/rsa]
             "tests/files/key_storage/online.key",  # Enter 1/2 the root`s private key path  # noqa
             "strongPass",  # Enter 1/2 the root`s private key password
+            "",  # [Optional] Give a name/tag to the key
             "",  # Choose 1/2 root key type [ed25519/ecdsa/rsa]
             "tests/files/key_storage/JanisJoplin.key",  # Enter 1/2 the root`s private key path  # noqa
             "strongPass",  # Enter 1/2 the root`s private key password
+            "",  # [Optional] Give a name/tag to the key
             "",  # Choose 2/2 root key type [ed25519/ecdsa/rsa]
             "tests/files/key_storage/JimiHendrix.key",  # Enter 2/2 the root`s private key path  # noqa
             "strongPass",  # Enter 2/2 the root`s private key password:
+            "",  # [Optional] Give a name/tag to the key
         ]
 
         test_result = client.invoke(
             ceremony.ceremony,
             input="\n".join(
                 input_step1 + input_step2 + input_step3 + input_step4
             ),
@@ -484,14 +526,15 @@
         # Say online key configuration is not correct, update with online-ecdsa
         # key and confirm the configuration
         input_step4 = [
             "n",  # Is the online key configuration correct? [y/n]
             "rsa",  # Choose 1/1 ONLINE key type [ed25519/ecdsa/rsa]
             "tests/files/key_storage/online-rsa.key",  # Enter 1/1 the ONLINE`s private key path  # noqa
             "strongPass",  # Enter 1/1 the ONLINE`s private key password
+            "",  # [Optional] Give a name/tag to the key
             "y",  # Is the online key configuration correct? [y/n]
             "y",  # Is the root configuration correct? [y/n]
             "y",  # Is the targets configuration correct? [y/n]
             "y",  # Is the snapshot configuration correct? [y/n]
             "y",  # Is the timestamp configuration correct? [y/n]
             "y",  # Is the bins configuration correct? [y/n]
         ]
@@ -523,14 +566,15 @@
             "y",  # Is the online key configuration correct? [y/n]
             "n",  # Is the root configuration correct? [y/n]
             "",  # What is the metadata expiration for the root role?(Days)
             "1",  # What is the number of keys for the root role? (2)
             "",  # Choose 1/1 root key type [ed25519/ecdsa/rsa]
             "tests/files/key_storage/JanisJoplin.key",  # Enter 1/1 the root`s private key path  # noqa
             "strongPass",  # Enter 1/2 the root`s private key password
+            "",  # [Optional] Give a name/tag to the key
             "y",  # Is the root configuration correct? [y/n]
             "y",  # Is the targets configuration correct? [y/n]
             "y",  # Is the snapshot configuration correct? [y/n]
             "y",  # Is the timestamp configuration correct? [y/n]
             "y",  # Is the bins configuration correct? [y/n]
         ]
 
@@ -731,15 +775,15 @@
             pretend.call(test_context["settings"], {"k": "v"})
         ]
         assert ceremony.task_status.calls == [
             pretend.call(
                 "fake_task_id", test_context["settings"], "Bootstrap status: "
             )
         ]
-        # test regression https://github.com/vmware/repository-service-tuf-cli/pull/259  # noqa
+        # test regression https://github.com/repository-service-tuf/repository-service-tuf-cli/pull/259  # noqa
         assert test_context["settings"].SERVER is not None
 
     def test_ceremony_option_bootstrap_upload_no_auth(
         self, client, test_context
     ):
         ceremony.bootstrap_status = pretend.call_recorder(
             lambda *a: {"data": {"bootstrap": False}}
```

### Comparing `repository_service_tuf-0.1.1a3/tests/unit/cli/admin/test_import_targets.py` & `repository_service_tuf-0.1.2a1/tests/unit/cli/admin/test_import_targets.py`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.1a3/tests/unit/cli/admin/test_login.py` & `repository_service_tuf-0.1.2a1/tests/unit/cli/admin/test_login.py`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.1a3/tests/unit/cli/key/test_generate_key.py` & `repository_service_tuf-0.1.2a1/tests/unit/cli/key/test_generate_key.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # SPDX-FileCopyrightText: 2022-2023 VMware Inc
 #
 # SPDX-License-Identifier: MIT
 from pathlib import Path
 from unittest import mock
+from unittest.mock import patch
 
 import pretend
 import pytest
 from securesystemslib.exceptions import FormatError  # type: ignore
 
 from repository_service_tuf.cli.key import generate_key
 from repository_service_tuf.cli.key.generate_key import _verify_password
@@ -36,14 +37,63 @@
         assert (
             "Please select one of the available options"
             not in test_result.output
         )
 
         assert test_result.exit_code == 1
 
+    @pytest.mark.parametrize("key_type", KeyType.get_all_members() + ["test"])
+    def test_generate_key_types_generation(
+        self, key_type, client, monkeypatch
+    ) -> None:
+        """
+        Test that all `KeyType` enum members input choices call the appropriate
+        keypair generate function
+        """
+
+        password = "test-password"
+        filename = "test-filename"
+        inputs = [
+            key_type,  # Choose key type [ed25519/ecdsa/rsa] (ed25519)
+            filename,  # Enter the keys' filename ...
+            "n",  # Do you want to overwrite the existing 'test-filename' file?
+        ]
+
+        generate_key._verify_password = pretend.call_recorder(
+            lambda a: password
+        )
+
+        mock_file_path = "repository_service_tuf.cli.key.generate_key."
+        mocked_functions = {
+            "ed25519": "_generate_and_write_ed25519_keypair",
+            "ecdsa": "_generate_and_write_ecdsa_keypair",
+            "rsa": "_generate_and_write_rsa_keypair",
+        }
+
+        if key_type in KeyType.get_all_members():
+            with patch(
+                mock_file_path + mocked_functions[key_type],
+                return_value=None,
+            ) as mock_keypair:
+                test_result = client.invoke(
+                    generate_key.generate,
+                    input="\n".join(inputs),
+                )
+
+                mock_keypair.called_once()
+                assert test_result.exit_code == 0
+
+        else:
+            test_result = client.invoke(
+                generate_key.generate,
+                input="\n".join(inputs),
+            )
+
+            assert test_result.exit_code == 1
+
     @pytest.mark.parametrize("filename", ["\n", "test-filename"])
     def test_generate(self, filename: str, client, monkeypatch) -> None:
         """
         Test all the steps in the `generate` sub-command work as expected
 
         Note: We also test that a default ('\n') filename value is set
         """
```

### Comparing `repository_service_tuf-0.1.1a3/tests/unit/helpers/test_api_client.py` & `repository_service_tuf-0.1.2a1/tests/unit/helpers/test_api_client.py`

 * *Files identical despite different names*

### Comparing `repository_service_tuf-0.1.1a3/tests/unit/helpers/test_tuf.py` & `repository_service_tuf-0.1.2a1/tests/unit/helpers/test_tuf.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from typing import Dict, List
 
 import pretend
 import pytest
 
 from repository_service_tuf.helpers import tuf
 from repository_service_tuf.helpers.tuf import (
+    Key,
     Metadata,
     Roles,
     Root,
     RSTUFKey,
     TUFManagement,
 )
 
@@ -26,18 +27,18 @@
         result = {}
         for filename in filenames:
             result[filename] = filename
 
         return result
 
     def test__signers_root_keys(self, test_tuf_management: TUFManagement):
-        test_tuf_management.setup.root_keys = [
-            RSTUFKey({"a": "b"}),
-            RSTUFKey({"c": "d"}),
-        ]
+        test_tuf_management.setup.root_keys = {
+            "id1": RSTUFKey({"a": "b"}),
+            "id2": RSTUFKey({"c": "d"}),
+        }
         tuf.SSlibSigner = pretend.call_recorder(lambda *a: None)
         result = test_tuf_management._signers(Roles.ROOT)
         assert result == [None, None]
         assert tuf.SSlibSigner.calls == [
             pretend.call({"a": "b"}),
             pretend.call({"c": "d"}),
         ]
@@ -250,14 +251,38 @@
         assert test_tuf_management._sign.calls == [
             pretend.call(fake_root, "root"),
         ]
         assert test_tuf_management._add_payload.calls == [
             pretend.call(fake_root, "root"),
         ]
 
+    def test_setup_key_name_root_key(self, test_tuf_management: TUFManagement):
+        key = Key("id", "ed25519", "ed25519-sha256", {"sha256": "abc"})
+        test_tuf_management.setup.root_keys["id"] = RSTUFKey({}, "", "my-key")
+        test_tuf_management._setup_key_name(key, Roles.ROOT.value)
+        assert key.unrecognized_fields["name"] == "my-key"
+
+    def test_setup_key_name_root_key_no_key_name(
+        self, test_tuf_management: TUFManagement
+    ):
+        key = Key("id", "ed25519", "ed25519-sha256", {"sha256": "abc"})
+        test_tuf_management.setup.root_keys["id"] = RSTUFKey({}, "")
+        test_tuf_management._setup_key_name(key, Roles.ROOT.value)
+        assert key.unrecognized_fields == {}
+
+    def test_setup_key_name_online_key(
+        self, test_tuf_management: TUFManagement
+    ):
+        key = Key("id", "ed25519", "ed25519-sha256", {"sha256": "abc"})
+        test_tuf_management.setup.online_key = RSTUFKey(
+            {"keyid": "id"}, "", "my-key"
+        )
+        test_tuf_management._setup_key_name(key, Roles.TIMESTAMP.value)
+        assert key.unrecognized_fields["name"] == "my-key"
+
     def test_initialize_metadata(self, test_tuf_management: TUFManagement):
         signers_mock = unittest.mock.Mock()
         root_signer = pretend.stub(key_dict="root")
         timestamp_signer = pretend.stub(key_dict="timestamp")
         snapshot_signer = pretend.stub(key_dict="snapshot")
         targets_signer = pretend.stub(key_dict="targets")
         signers_mock.side_effect = [
@@ -270,14 +295,17 @@
         tuf.Role = pretend.call_recorder(lambda *a: "role")
 
         key_from_securesystemslib_mock = pretend.call_recorder(
             lambda role_name: f"{role_name}_key"
         )
 
         tuf.Key.from_securesystemslib_key = key_from_securesystemslib_mock
+        test_tuf_management._setup_key_name = pretend.call_recorder(
+            lambda *a: None
+        )
         test_tuf_management._prepare_root_and_add_it_to_payload = (
             pretend.call_recorder(lambda *a: None)
         )
         test_tuf_management._validate_root_payload_exist = (
             pretend.call_recorder(lambda *a: None)
         )
         result = test_tuf_management.initialize_metadata()
@@ -293,14 +321,20 @@
         )
         assert tuf.Key.from_securesystemslib_key.calls == [
             pretend.call("root"),
             pretend.call("timestamp"),
             pretend.call("snapshot"),
             pretend.call("targets"),
         ]
+        assert test_tuf_management._setup_key_name.calls == [
+            pretend.call("root_key", "root"),
+            pretend.call("timestamp_key", "timestamp"),
+            pretend.call("snapshot_key", "snapshot"),
+            pretend.call("targets_key", "targets"),
+        ]
         expected_roles: Dict[str, str] = {
             "root": "role",
             "timestamp": "role",
             "snapshot": "role",
             "targets": "role",
         }
         expected_add_key_args: Dict[str, List[str]] = {
```

### Comparing `repository_service_tuf-0.1.1a3/PKG-INFO` & `repository_service_tuf-0.1.2a1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: repository-service-tuf
-Version: 0.1.1a3
+Version: 0.1.2a1
 Summary: Repository Service for TUF Command Line Interface
 Author-email: Kairo de Araujo <kairo@dearaujo.nl>
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.9
+Requires-Python: >=3.8
 Requires-Dist: click
 Requires-Dist: dynaconf[ini]==3.1.9
 Requires-Dist: pynacl
 Requires-Dist: requests
 Requires-Dist: rich
 Requires-Dist: rich-click
 Requires-Dist: securesystemslib[crypto]
@@ -30,18 +29,18 @@
 
 #################################################
 Repository Service for TUF Command Line Interface
 #################################################
 
 |Tests and Lint| |Coverage|
 
-.. |Tests and Lint| image:: https://github.com/vmware/repository-service-tuf-cli/actions/workflows/ci.yml/badge.svg
-  :target: https://github.com/vmware/repository-service-tuf-cli/actions/workflows/ci.yml
-.. |Coverage| image:: https://codecov.io/gh/vmware/repository-service-tuf-cli/branch/main/graph/badge.svg
-  :target: https://codecov.io/gh/vmware/repository-service-tuf-cli
+.. |Tests and Lint| image:: https://github.com/repository-service-tuf/repository-service-tuf-cli/actions/workflows/ci.yml/badge.svg
+  :target: https://github.com/repository-service-tuf/repository-service-tuf-cli/actions/workflows/ci.yml
+.. |Coverage| image:: https://codecov.io/gh/repository-service-tuf/repository-service-tuf-cli/branch/main/graph/badge.svg
+  :target: https://codecov.io/gh/repository-service-tuf/repository-service-tuf-cli
 
 The Repository Service for TUF Command Line Interface (CLI) is a CLI Python
 application to manage the Repository Service for TUF.
 
 The CLI supports the initial setup, termed a ceremony, where the first repository
 metadata are signed and the service is configured, generating tokens to be used
 by integration (i.e., CI/CD tools).
@@ -68,13 +67,13 @@
 
 Contributing
 ============
 
 Please, visit the `Repository Service for TUF Development Guide
 <https://repository-service-tuf.readthedocs.io/en/latest/devel/index.html#development-guide>`_.
 
-Check our `CONTRIBUTING.rst <https://github.com/vmware/repository-service-tuf-cli/blob/main/CONTRIBUTING.rst>`_
+Check our `CONTRIBUTING.rst <https://github.com/repository-service-tuf/repository-service-tuf-cli/blob/main/CONTRIBUTING.rst>`_
 for more details on how to contribute to this repository.
 
 License
 =======
-`MIT <https://github.com/vmware/repository-service-tuf-cli/blob/main/LICENSE>`_
+`MIT <https://github.com/repository-service-tuf/repository-service-tuf-cli/blob/main/LICENSE>`_
```

