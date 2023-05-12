# Comparing `tmp/dbt-core-1.5.0rc2.tar.gz` & `tmp/dbt-core-1.5.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-core-1.5.0rc2.tar", last modified: Thu Apr 20 21:14:58 2023, max compression
+gzip compressed data, was "dbt-core-1.5.1rc1.tar", last modified: Fri May 12 15:32:15 2023, max compression
```

## Comparing `dbt-core-1.5.0rc2.tar` & `dbt-core-1.5.1rc1.tar`

### file list

```diff
@@ -1,312 +1,312 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:14:58.562554 dbt-core-1.5.0rc2/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3207 2023-04-20 21:14:58.562554 dbt-core-1.5.0rc2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:14:58.530555 dbt-core-1.5.0rc2/dbt/
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:14:58.530555 dbt-core-1.5.0rc2/dbt/adapters/
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/adapters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:14:58.534555 dbt-core-1.5.0rc2/dbt/adapters/base/
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/adapters/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5252 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/adapters/base/column.py
--rw-r--r--   0 runner    (1001) docker     (123)    15908 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/adapters/base/connections.py
--rw-r--r--   0 runner    (1001) docker     (123)    55030 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/adapters/base/impl.py
--rw-r--r--   0 runner    (1001) docker     (123)     4525 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/adapters/base/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/adapters/base/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/adapters/base/query_headers.py
--rw-r--r--   0 runner    (1001) docker     (123)    14913 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/adapters/base/relation.py
--rw-r--r--   0 runner    (1001) docker     (123)    19958 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/adapters/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     7859 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/adapters/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/adapters/protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/adapters/reference_keys.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:14:58.534555 dbt-core-1.5.0rc2/dbt/adapters/sql/
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/adapters/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6570 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/adapters/sql/connections.py
--rw-r--r--   0 runner    (1001) docker     (123)     8930 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/adapters/sql/impl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:14:58.534555 dbt-core-1.5.0rc2/dbt/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/cli/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/cli/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12739 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/cli/flags.py
--rw-r--r--   0 runner    (1001) docker     (123)    16615 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/cli/option_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/cli/options.py
--rw-r--r--   0 runner    (1001) docker     (123)    16863 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/cli/params.py
--rw-r--r--   0 runner    (1001) docker     (123)     8568 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/cli/requires.py
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/cli/resolvers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:14:58.534555 dbt-core-1.5.0rc2/dbt/clients/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12364 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/clients/_jinja_blocks.py
--rw-r--r--   0 runner    (1001) docker     (123)     7594 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/clients/agate_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     5240 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/clients/git.py
--rw-r--r--   0 runner    (1001) docker     (123)    21425 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/clients/jinja.py
--rw-r--r--   0 runner    (1001) docker     (123)     5237 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/clients/jinja_static.py
--rw-r--r--   0 runner    (1001) docker     (123)     7941 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/clients/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)    19144 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/clients/system.py
--rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/clients/yaml_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    19815 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/compilation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:14:58.538555 dbt-core-1.5.0rc2/dbt/config/
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16817 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/config/profile.py
--rw-r--r--   0 runner    (1001) docker     (123)    24994 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/config/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     7204 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/config/renderer.py
--rw-r--r--   0 runner    (1001) docker     (123)    16144 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/config/runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)     7862 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/config/selectors.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/config/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:14:58.538555 dbt-core-1.5.0rc2/dbt/context/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/context/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22970 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/context/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4343 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/context/configured.py
--rw-r--r--   0 runner    (1001) docker     (123)    12660 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/context/context_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/context/docs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4177 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/context/exceptions_jinja.py
--rw-r--r--   0 runner    (1001) docker     (123)     8605 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/context/macro_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     7335 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/context/macros.py
--rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/context/manifest.py
--rw-r--r--   0 runner    (1001) docker     (123)    57568 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/context/providers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/context/secret.py
--rw-r--r--   0 runner    (1001) docker     (123)     4163 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/context/target.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:14:58.538555 dbt-core-1.5.0rc2/dbt/contracts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/contracts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6768 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/contracts/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)    10372 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/contracts/files.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:14:58.542554 dbt-core-1.5.0rc2/dbt/contracts/graph/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/contracts/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    45991 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/contracts/graph/manifest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5169 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/contracts/graph/manifest_upgrade.py
--rw-r--r--   0 runner    (1001) docker     (123)     3224 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/contracts/graph/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    20939 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/contracts/graph/model_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    45470 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/contracts/graph/nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/contracts/graph/searcher.py
--rw-r--r--   0 runner    (1001) docker     (123)    20236 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/contracts/graph/unparsed.py
--rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/contracts/graph/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8863 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/contracts/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/contracts/relation.py
--rw-r--r--   0 runner    (1001) docker     (123)    13381 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/contracts/results.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/contracts/selection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/contracts/sql.py
--rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/contracts/state.py
--rw-r--r--   0 runner    (1001) docker     (123)     8798 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/contracts/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     5117 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/dataclass_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     3931 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/deprecations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:14:58.542554 dbt-core-1.5.0rc2/dbt/deps/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/deps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4672 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/deps/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4950 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/deps/git.py
--rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/deps/local.py
--rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/deps/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/deps/resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/deps/tarball.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:14:58.526554 dbt-core-1.5.0rc2/dbt/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:14:58.542554 dbt-core-1.5.0rc2/dbt/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:14:58.542554 dbt-core-1.5.0rc2/dbt/docs/source/_ext/
--rw-r--r--   0 runner    (1001) docker     (123)     3544 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/docs/source/_ext/dbt_click.py
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/docs/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:14:58.542554 dbt-core-1.5.0rc2/dbt/events/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/events/adapter_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     5312 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/events/base_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/events/contextvars.py
--rw-r--r--   0 runner    (1001) docker     (123)     7301 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/events/eventmgr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/events/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     9522 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/events/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/events/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    58511 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/events/types.py
--rw-r--r--   0 runner    (1001) docker     (123)   101429 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/events/types_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    74918 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/flags.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:14:58.546554 dbt-core-1.5.0rc2/dbt/graph/
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9593 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/graph/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4640 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/graph/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     7332 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/graph/queue.py
--rw-r--r--   0 runner    (1001) docker     (123)    13206 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/graph/selector.py
--rw-r--r--   0 runner    (1001) docker     (123)    27989 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/graph/selector_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     7103 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/graph/selector_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     5117 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/helper_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/hooks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:14:58.546554 dbt-core-1.5.0rc2/dbt/include/
--rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:14:58.546554 dbt-core-1.5.0rc2/dbt/include/global_project/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/global_project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/global_project/dbt_project.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:14:58.546554 dbt-core-1.5.0rc2/dbt/include/global_project/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/global_project/docs/overview.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:14:58.526554 dbt-core-1.5.0rc2/dbt/include/global_project/macros/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:14:58.546554 dbt-core-1.5.0rc2/dbt/include/global_project/macros/adapters/
--rw-r--r--   0 runner    (1001) docker     (123)     6825 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/global_project/macros/adapters/apply_grants.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4639 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/global_project/macros/adapters/columns.sql
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/global_project/macros/adapters/freshness.sql
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/global_project/macros/adapters/indexes.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/global_project/macros/adapters/metadata.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/global_project/macros/adapters/persist_docs.sql
--rw-r--r--   0 runner    (1001) docker     (123)     3730 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/global_project/macros/adapters/relation.sql
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/global_project/macros/adapters/schema.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/global_project/macros/adapters/timestamps.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:14:58.546554 dbt-core-1.5.0rc2/dbt/include/global_project/macros/etc/
--rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/global_project/macros/etc/datetime.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/global_project/macros/etc/statement.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:14:58.546554 dbt-core-1.5.0rc2/dbt/include/global_project/macros/generic_test_sql/
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/global_project/macros/generic_test_sql/accepted_values.sql
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/global_project/macros/generic_test_sql/not_null.sql
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/global_project/macros/generic_test_sql/relationships.sql
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/global_project/macros/generic_test_sql/unique.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:14:58.550554 dbt-core-1.5.0rc2/dbt/include/global_project/macros/get_custom_name/
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/global_project/macros/get_custom_name/get_custom_alias.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/global_project/macros/get_custom_name/get_custom_database.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/global_project/macros/get_custom_name/get_custom_schema.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:14:58.550554 dbt-core-1.5.0rc2/dbt/include/global_project/macros/materializations/
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/global_project/macros/materializations/configs.sql
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/global_project/macros/materializations/hooks.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:14:58.526554 dbt-core-1.5.0rc2/dbt/include/global_project/macros/materializations/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:14:58.550554 dbt-core-1.5.0rc2/dbt/include/global_project/macros/materializations/models/incremental/
--rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/global_project/macros/materializations/models/incremental/column_helpers.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4235 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/global_project/macros/materializations/models/incremental/incremental.sql
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/global_project/macros/materializations/models/incremental/is_incremental.sql
--rw-r--r--   0 runner    (1001) docker     (123)     5197 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/global_project/macros/materializations/models/incremental/merge.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4927 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/global_project/macros/materializations/models/incremental/on_schema_change.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/global_project/macros/materializations/models/incremental/strategies.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:14:58.550554 dbt-core-1.5.0rc2/dbt/include/global_project/macros/materializations/models/table/
--rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/global_project/macros/materializations/models/table/columns_spec_ddl.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/global_project/macros/materializations/models/table/create_table_as.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/global_project/macros/materializations/models/table/table.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:14:58.550554 dbt-core-1.5.0rc2/dbt/include/global_project/macros/materializations/models/view/
--rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/global_project/macros/materializations/models/view/create_or_replace_view.sql
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/global_project/macros/materializations/models/view/create_view_as.sql
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/global_project/macros/materializations/models/view/helpers.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/global_project/macros/materializations/models/view/view.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:14:58.550554 dbt-core-1.5.0rc2/dbt/include/global_project/macros/materializations/seeds/
--rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/global_project/macros/materializations/seeds/helpers.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/global_project/macros/materializations/seeds/seed.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:14:58.550554 dbt-core-1.5.0rc2/dbt/include/global_project/macros/materializations/snapshots/
--rw-r--r--   0 runner    (1001) docker     (123)     4807 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/global_project/macros/materializations/snapshots/helpers.sql
--rw-r--r--   0 runner    (1001) docker     (123)     3680 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/global_project/macros/materializations/snapshots/snapshot.sql
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/global_project/macros/materializations/snapshots/snapshot_merge.sql
--rw-r--r--   0 runner    (1001) docker     (123)     6286 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/global_project/macros/materializations/snapshots/strategies.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:14:58.550554 dbt-core-1.5.0rc2/dbt/include/global_project/macros/materializations/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/global_project/macros/materializations/tests/helpers.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/global_project/macros/materializations/tests/test.sql
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/global_project/macros/materializations/tests/where_subquery.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:14:58.550554 dbt-core-1.5.0rc2/dbt/include/global_project/macros/python_model/
--rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/global_project/macros/python_model/python.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:14:58.554554 dbt-core-1.5.0rc2/dbt/include/global_project/macros/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/global_project/macros/utils/any_value.sql
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/global_project/macros/utils/array_append.sql
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/global_project/macros/utils/array_concat.sql
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/global_project/macros/utils/array_construct.sql
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/global_project/macros/utils/bool_or.sql
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/global_project/macros/utils/cast_bool_to_text.sql
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/global_project/macros/utils/concat.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4416 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/global_project/macros/utils/data_types.sql
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/global_project/macros/utils/date_trunc.sql
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/global_project/macros/utils/dateadd.sql
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/global_project/macros/utils/datediff.sql
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/global_project/macros/utils/escape_single_quotes.sql
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/global_project/macros/utils/except.sql
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/global_project/macros/utils/hash.sql
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/global_project/macros/utils/intersect.sql
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/global_project/macros/utils/last_day.sql
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/global_project/macros/utils/length.sql
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/global_project/macros/utils/listagg.sql
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/global_project/macros/utils/literal.sql
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/global_project/macros/utils/position.sql
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/global_project/macros/utils/replace.sql
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/global_project/macros/utils/right.sql
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/global_project/macros/utils/safe_cast.sql
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/global_project/macros/utils/split_part.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:14:58.526554 dbt-core-1.5.0rc2/dbt/include/global_project/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:14:58.554554 dbt-core-1.5.0rc2/dbt/include/global_project/tests/generic/
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/global_project/tests/generic/builtin.sql
--rw-r--r--   0 runner    (1001) docker     (123)  1497701 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:14:58.554554 dbt-core-1.5.0rc2/dbt/include/starter_project/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/starter_project/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/starter_project/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/starter_project/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:14:58.554554 dbt-core-1.5.0rc2/dbt/include/starter_project/analyses/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/starter_project/analyses/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/starter_project/dbt_project.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:14:58.554554 dbt-core-1.5.0rc2/dbt/include/starter_project/macros/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/starter_project/macros/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:14:58.526554 dbt-core-1.5.0rc2/dbt/include/starter_project/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:14:58.554554 dbt-core-1.5.0rc2/dbt/include/starter_project/models/example/
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/starter_project/models/example/my_first_dbt_model.sql
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/starter_project/models/example/my_second_dbt_model.sql
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/starter_project/models/example/schema.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:14:58.554554 dbt-core-1.5.0rc2/dbt/include/starter_project/seeds/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/starter_project/seeds/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:14:58.554554 dbt-core-1.5.0rc2/dbt/include/starter_project/snapshots/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/starter_project/snapshots/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:14:58.554554 dbt-core-1.5.0rc2/dbt/include/starter_project/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/include/starter_project/tests/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/internal_deprecations.py
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/links.py
--rw-r--r--   0 runner    (1001) docker     (123)    19932 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/node_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:14:58.558554 dbt-core-1.5.0rc2/dbt/parser/
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/parser/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    16910 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/parser/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/parser/docs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3656 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/parser/generic_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    16770 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/parser/generic_test_builders.py
--rw-r--r--   0 runner    (1001) docker     (123)     3639 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/parser/hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/parser/macros.py
--rw-r--r--   0 runner    (1001) docker     (123)    62438 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/parser/manifest.py
--rw-r--r--   0 runner    (1001) docker     (123)    25716 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/parser/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    50860 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/parser/partial.py
--rw-r--r--   0 runner    (1001) docker     (123)    16958 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/parser/read_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/parser/schema_renderer.py
--rw-r--r--   0 runner    (1001) docker     (123)    59005 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/parser/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/parser/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/parser/seeds.py
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/parser/singular_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/parser/snapshots.py
--rw-r--r--   0 runner    (1001) docker     (123)    14106 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/parser/sources.py
--rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/parser/sql.py
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/selected_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)    13885 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/semver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:14:58.562554 dbt-core-1.5.0rc2/dbt/task/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/task/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16571 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/task/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/task/build.py
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/task/clean.py
--rw-r--r--   0 runner    (1001) docker     (123)     5627 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/task/compile.py
--rw-r--r--   0 runner    (1001) docker     (123)    14097 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/task/debug.py
--rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/task/deps.py
--rw-r--r--   0 runner    (1001) docker     (123)     6250 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/task/freshness.py
--rw-r--r--   0 runner    (1001) docker     (123)     9541 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/task/generate.py
--rw-r--r--   0 runner    (1001) docker     (123)    13795 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/task/init.py
--rw-r--r--   0 runner    (1001) docker     (123)     7181 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/task/list.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/task/parse.py
--rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/task/printer.py
--rw-r--r--   0 runner    (1001) docker     (123)    17788 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/task/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/task/run_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)    21143 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/task/runnable.py
--rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/task/seed.py
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/task/serve.py
--rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/task/show.py
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/task/snapshot.py
--rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/task/sql.py
--rw-r--r--   0 runner    (1001) docker     (123)     7043 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/task/test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:14:58.562554 dbt-core-1.5.0rc2/dbt/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:14:58.562554 dbt-core-1.5.0rc2/dbt/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/tests/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18424 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/tests/fixtures/project.py
--rw-r--r--   0 runner    (1001) docker     (123)    18179 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/tests/util.py
--rw-r--r--   0 runner    (1001) docker     (123)    14471 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/tracking.py
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/ui.py
--rw-r--r--   0 runner    (1001) docker     (123)    20505 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7398 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/dbt/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 21:14:58.562554 dbt-core-1.5.0rc2/dbt_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3207 2023-04-20 21:14:58.000000 dbt-core-1.5.0rc2/dbt_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9118 2023-04-20 21:14:58.000000 dbt-core-1.5.0rc2/dbt_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 21:14:58.000000 dbt-core-1.5.0rc2/dbt_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-20 21:14:58.000000 dbt-core-1.5.0rc2/dbt_core.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 21:14:58.000000 dbt-core-1.5.0rc2/dbt_core.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-04-20 21:14:58.000000 dbt-core-1.5.0rc2/dbt_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-20 21:14:58.000000 dbt-core-1.5.0rc2/dbt_core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 21:14:58.562554 dbt-core-1.5.0rc2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2778 2023-04-20 21:14:46.000000 dbt-core-1.5.0rc2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:32:15.852804 dbt-core-1.5.1rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3207 2023-05-12 15:32:15.852804 dbt-core-1.5.1rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:32:15.824803 dbt-core-1.5.1rc1/dbt/
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:32:15.824803 dbt-core-1.5.1rc1/dbt/adapters/
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/adapters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:32:15.824803 dbt-core-1.5.1rc1/dbt/adapters/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/adapters/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5252 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/adapters/base/column.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15908 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/adapters/base/connections.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55643 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/adapters/base/impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4525 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/adapters/base/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/adapters/base/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/adapters/base/query_headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14913 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/adapters/base/relation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19958 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/adapters/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7859 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/adapters/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/adapters/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/adapters/reference_keys.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:32:15.824803 dbt-core-1.5.1rc1/dbt/adapters/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/adapters/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6570 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/adapters/sql/connections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8930 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/adapters/sql/impl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:32:15.824803 dbt-core-1.5.1rc1/dbt/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/cli/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/cli/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12739 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/cli/flags.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16567 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/cli/option_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/cli/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16863 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/cli/params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8568 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/cli/requires.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/cli/resolvers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:32:15.828803 dbt-core-1.5.1rc1/dbt/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12364 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/clients/_jinja_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7594 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/clients/agate_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5240 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/clients/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21425 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/clients/jinja.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5237 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/clients/jinja_static.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7941 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/clients/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19144 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/clients/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/clients/yaml_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19815 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/compilation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:32:15.828803 dbt-core-1.5.1rc1/dbt/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16817 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/config/profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24994 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/config/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7204 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/config/renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16144 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/config/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7862 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/config/selectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/config/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:32:15.828803 dbt-core-1.5.1rc1/dbt/context/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/context/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22966 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/context/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4343 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/context/configured.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12660 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/context/context_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/context/docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4177 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/context/exceptions_jinja.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8605 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/context/macro_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7335 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/context/macros.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/context/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58069 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/context/providers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/context/secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4163 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/context/target.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:32:15.828803 dbt-core-1.5.1rc1/dbt/contracts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/contracts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6768 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/contracts/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10372 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/contracts/files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:32:15.832804 dbt-core-1.5.1rc1/dbt/contracts/graph/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/contracts/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47351 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/contracts/graph/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5169 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/contracts/graph/manifest_upgrade.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3224 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/contracts/graph/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20939 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/contracts/graph/model_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45470 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/contracts/graph/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/contracts/graph/searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20236 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/contracts/graph/unparsed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/contracts/graph/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8863 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/contracts/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/contracts/relation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13381 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/contracts/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/contracts/selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/contracts/sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/contracts/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8798 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/contracts/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5117 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/dataclass_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4123 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/deprecations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:32:15.832804 dbt-core-1.5.1rc1/dbt/deps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/deps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4672 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/deps/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4950 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/deps/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2447 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/deps/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/deps/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/deps/resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/deps/tarball.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:32:15.816803 dbt-core-1.5.1rc1/dbt/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:32:15.832804 dbt-core-1.5.1rc1/dbt/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:32:15.832804 dbt-core-1.5.1rc1/dbt/docs/source/_ext/
+-rw-r--r--   0 runner    (1001) docker     (123)     3544 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/docs/source/_ext/dbt_click.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/docs/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:32:15.832804 dbt-core-1.5.1rc1/dbt/events/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/events/adapter_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5312 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/events/base_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/events/contextvars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7301 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/events/eventmgr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/events/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9522 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/events/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/events/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60059 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/events/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)   102631 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/events/types_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74918 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/flags.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:32:15.836804 dbt-core-1.5.1rc1/dbt/graph/
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9593 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/graph/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4640 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/graph/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7332 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/graph/queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13206 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/graph/selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27989 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/graph/selector_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7103 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/graph/selector_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5117 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/helper_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/hooks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:32:15.836804 dbt-core-1.5.1rc1/dbt/include/
+-rw-r--r--   0 runner    (1001) docker     (123)     4794 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/include/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:32:15.836804 dbt-core-1.5.1rc1/dbt/include/global_project/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/include/global_project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/include/global_project/dbt_project.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:32:15.836804 dbt-core-1.5.1rc1/dbt/include/global_project/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/include/global_project/docs/overview.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:32:15.816803 dbt-core-1.5.1rc1/dbt/include/global_project/macros/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:32:15.836804 dbt-core-1.5.1rc1/dbt/include/global_project/macros/adapters/
+-rw-r--r--   0 runner    (1001) docker     (123)     6825 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/include/global_project/macros/adapters/apply_grants.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4639 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/include/global_project/macros/adapters/columns.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/include/global_project/macros/adapters/freshness.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/include/global_project/macros/adapters/indexes.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/include/global_project/macros/adapters/metadata.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/include/global_project/macros/adapters/persist_docs.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     3730 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/include/global_project/macros/adapters/relation.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/include/global_project/macros/adapters/schema.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/include/global_project/macros/adapters/timestamps.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:32:15.836804 dbt-core-1.5.1rc1/dbt/include/global_project/macros/etc/
+-rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/include/global_project/macros/etc/datetime.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/include/global_project/macros/etc/statement.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:32:15.840804 dbt-core-1.5.1rc1/dbt/include/global_project/macros/generic_test_sql/
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/include/global_project/macros/generic_test_sql/accepted_values.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/include/global_project/macros/generic_test_sql/not_null.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/include/global_project/macros/generic_test_sql/relationships.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/include/global_project/macros/generic_test_sql/unique.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:32:15.840804 dbt-core-1.5.1rc1/dbt/include/global_project/macros/get_custom_name/
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/include/global_project/macros/get_custom_name/get_custom_alias.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/include/global_project/macros/get_custom_name/get_custom_database.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/include/global_project/macros/get_custom_name/get_custom_schema.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:32:15.840804 dbt-core-1.5.1rc1/dbt/include/global_project/macros/materializations/
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/include/global_project/macros/materializations/configs.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/include/global_project/macros/materializations/hooks.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:32:15.816803 dbt-core-1.5.1rc1/dbt/include/global_project/macros/materializations/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:32:15.840804 dbt-core-1.5.1rc1/dbt/include/global_project/macros/materializations/models/incremental/
+-rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/include/global_project/macros/materializations/models/incremental/column_helpers.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4235 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/include/global_project/macros/materializations/models/incremental/incremental.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/include/global_project/macros/materializations/models/incremental/is_incremental.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     5197 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/include/global_project/macros/materializations/models/incremental/merge.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4927 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/include/global_project/macros/materializations/models/incremental/on_schema_change.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/include/global_project/macros/materializations/models/incremental/strategies.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:32:15.840804 dbt-core-1.5.1rc1/dbt/include/global_project/macros/materializations/models/table/
+-rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/include/global_project/macros/materializations/models/table/columns_spec_ddl.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/include/global_project/macros/materializations/models/table/create_table_as.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/include/global_project/macros/materializations/models/table/table.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:32:15.840804 dbt-core-1.5.1rc1/dbt/include/global_project/macros/materializations/models/view/
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/include/global_project/macros/materializations/models/view/create_or_replace_view.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/include/global_project/macros/materializations/models/view/create_view_as.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/include/global_project/macros/materializations/models/view/helpers.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/include/global_project/macros/materializations/models/view/view.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:32:15.840804 dbt-core-1.5.1rc1/dbt/include/global_project/macros/materializations/seeds/
+-rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/include/global_project/macros/materializations/seeds/helpers.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/include/global_project/macros/materializations/seeds/seed.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:32:15.840804 dbt-core-1.5.1rc1/dbt/include/global_project/macros/materializations/snapshots/
+-rw-r--r--   0 runner    (1001) docker     (123)     4807 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/include/global_project/macros/materializations/snapshots/helpers.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     3680 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/include/global_project/macros/materializations/snapshots/snapshot.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/include/global_project/macros/materializations/snapshots/snapshot_merge.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     6286 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/include/global_project/macros/materializations/snapshots/strategies.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:32:15.840804 dbt-core-1.5.1rc1/dbt/include/global_project/macros/materializations/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/include/global_project/macros/materializations/tests/helpers.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/include/global_project/macros/materializations/tests/test.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/include/global_project/macros/materializations/tests/where_subquery.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:32:15.840804 dbt-core-1.5.1rc1/dbt/include/global_project/macros/python_model/
+-rw-r--r--   0 runner    (1001) docker     (123)     3466 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/include/global_project/macros/python_model/python.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:32:15.844804 dbt-core-1.5.1rc1/dbt/include/global_project/macros/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/include/global_project/macros/utils/any_value.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/include/global_project/macros/utils/array_append.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/include/global_project/macros/utils/array_concat.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/include/global_project/macros/utils/array_construct.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/include/global_project/macros/utils/bool_or.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/include/global_project/macros/utils/cast_bool_to_text.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/include/global_project/macros/utils/concat.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4416 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/include/global_project/macros/utils/data_types.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/include/global_project/macros/utils/date_trunc.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/include/global_project/macros/utils/dateadd.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/include/global_project/macros/utils/datediff.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/include/global_project/macros/utils/escape_single_quotes.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/include/global_project/macros/utils/except.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/include/global_project/macros/utils/hash.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/include/global_project/macros/utils/intersect.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/include/global_project/macros/utils/last_day.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/include/global_project/macros/utils/length.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/include/global_project/macros/utils/listagg.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/include/global_project/macros/utils/literal.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/include/global_project/macros/utils/position.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/include/global_project/macros/utils/replace.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/include/global_project/macros/utils/right.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/include/global_project/macros/utils/safe_cast.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/include/global_project/macros/utils/split_part.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:32:15.820803 dbt-core-1.5.1rc1/dbt/include/global_project/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:32:15.844804 dbt-core-1.5.1rc1/dbt/include/global_project/tests/generic/
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/include/global_project/tests/generic/builtin.sql
+-rw-r--r--   0 runner    (1001) docker     (123)  1497701 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/include/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:32:15.844804 dbt-core-1.5.1rc1/dbt/include/starter_project/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/include/starter_project/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/include/starter_project/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/include/starter_project/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:32:15.844804 dbt-core-1.5.1rc1/dbt/include/starter_project/analyses/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/include/starter_project/analyses/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/include/starter_project/dbt_project.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:32:15.844804 dbt-core-1.5.1rc1/dbt/include/starter_project/macros/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/include/starter_project/macros/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:32:15.820803 dbt-core-1.5.1rc1/dbt/include/starter_project/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:32:15.844804 dbt-core-1.5.1rc1/dbt/include/starter_project/models/example/
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/include/starter_project/models/example/my_first_dbt_model.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/include/starter_project/models/example/my_second_dbt_model.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/include/starter_project/models/example/schema.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:32:15.848804 dbt-core-1.5.1rc1/dbt/include/starter_project/seeds/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/include/starter_project/seeds/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:32:15.848804 dbt-core-1.5.1rc1/dbt/include/starter_project/snapshots/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/include/starter_project/snapshots/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:32:15.848804 dbt-core-1.5.1rc1/dbt/include/starter_project/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/include/starter_project/tests/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/internal_deprecations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/links.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19932 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/node_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:32:15.848804 dbt-core-1.5.1rc1/dbt/parser/
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/parser/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16910 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/parser/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/parser/docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3656 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/parser/generic_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16770 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/parser/generic_test_builders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3639 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/parser/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/parser/macros.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62438 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/parser/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25704 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/parser/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51437 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/parser/partial.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16958 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/parser/read_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/parser/schema_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59386 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/parser/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/parser/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/parser/seeds.py
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/parser/singular_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/parser/snapshots.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14106 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/parser/sources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/parser/sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/selected_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13885 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/semver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:32:15.852804 dbt-core-1.5.1rc1/dbt/task/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/task/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16571 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/task/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/task/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/task/clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5627 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/task/compile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14097 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/task/debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/task/deps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6468 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/task/freshness.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9541 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/task/generate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13795 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/task/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7181 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/task/list.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/task/parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/task/printer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17788 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/task/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/task/run_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21143 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/task/runnable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/task/seed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/task/serve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3844 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/task/show.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/task/snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3489 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/task/sql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7043 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/task/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:32:15.852804 dbt-core-1.5.1rc1/dbt/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:32:15.852804 dbt-core-1.5.1rc1/dbt/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/tests/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18424 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/tests/fixtures/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18179 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/tests/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14471 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/tracking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20505 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7398 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/dbt/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:32:15.852804 dbt-core-1.5.1rc1/dbt_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3207 2023-05-12 15:32:15.000000 dbt-core-1.5.1rc1/dbt_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9118 2023-05-12 15:32:15.000000 dbt-core-1.5.1rc1/dbt_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 15:32:15.000000 dbt-core-1.5.1rc1/dbt_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-12 15:32:15.000000 dbt-core-1.5.1rc1/dbt_core.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 15:32:15.000000 dbt-core-1.5.1rc1/dbt_core.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-12 15:32:15.000000 dbt-core-1.5.1rc1/dbt_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-12 15:32:15.000000 dbt-core-1.5.1rc1/dbt_core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 15:32:15.852804 dbt-core-1.5.1rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-05-12 15:32:04.000000 dbt-core-1.5.1rc1/setup.py
```

### Comparing `dbt-core-1.5.0rc2/PKG-INFO` & `dbt-core-1.5.1rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-core
-Version: 1.5.0rc2
+Version: 1.5.1rc1
 Summary: With dbt, data analysts and engineers can build analytics the way engineers build applications.
 Home-page: https://github.com/dbt-labs/dbt-core
 Author: dbt Labs
 Author-email: info@dbtlabs.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dbt-core Version: 1.5.0rc2 Summary: With dbt, data
+Metadata-Version: 2.1 Name: dbt-core Version: 1.5.1rc1 Summary: With dbt, data
 analysts and engineers can build analytics the way engineers build
 applications. Home-page: https://github.com/dbt-labs/dbt-core Author: dbt Labs
 Author-email: info@dbtlabs.com Classifier: Development Status :: 5 -
 Production/Stable Classifier: License :: OSI Approved :: Apache Software
 License Classifier: Operating System :: Microsoft :: Windows Classifier:
 Operating System :: MacOS :: MacOS X Classifier: Operating System :: POSIX ::
 Linux Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
```

### Comparing `dbt-core-1.5.0rc2/README.md` & `dbt-core-1.5.1rc1/README.md`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/adapters/base/__init__.py` & `dbt-core-1.5.1rc1/dbt/adapters/base/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/adapters/base/column.py` & `dbt-core-1.5.1rc1/dbt/adapters/base/column.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/adapters/base/connections.py` & `dbt-core-1.5.1rc1/dbt/adapters/base/connections.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/adapters/base/impl.py` & `dbt-core-1.5.1rc1/dbt/adapters/base/impl.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,15 +67,15 @@
     BaseRelation,
     InformationSchema,
     SchemaSearchMap,
 )
 from dbt.adapters.base import Column as BaseColumn
 from dbt.adapters.base import Credentials
 from dbt.adapters.cache import RelationsCache, _make_ref_key_dict
-
+from dbt import deprecations
 
 GET_CATALOG_MACRO_NAME = "get_catalog"
 FRESHNESS_MACRO_NAME = "collect_freshness"
 
 
 class ConstraintSupport(str, Enum):
     ENFORCED = "enforced"
@@ -1100,25 +1100,36 @@
 
     def calculate_freshness(
         self,
         source: BaseRelation,
         loaded_at_field: str,
         filter: Optional[str],
         manifest: Optional[Manifest] = None,
-    ) -> Tuple[AdapterResponse, Dict[str, Any]]:
+    ) -> Tuple[Optional[AdapterResponse], Dict[str, Any]]:
         """Calculate the freshness of sources in dbt, and return it"""
         kwargs: Dict[str, Any] = {
             "source": source,
             "loaded_at_field": loaded_at_field,
             "filter": filter,
         }
 
         # run the macro
+        # in older versions of dbt-core, the 'collect_freshness' macro returned the table of results directly
+        # starting in v1.5, by default, we return both the table and the adapter response (metadata about the query)
+        result: Union[
+            AttrDict,  # current: contains AdapterResponse + agate.Table
+            agate.Table,  # previous: just table
+        ]
         result = self.execute_macro(FRESHNESS_MACRO_NAME, kwargs=kwargs, manifest=manifest)
-        adapter_response, table = result.response, result.table  # type: ignore[attr-defined]
+        if isinstance(result, agate.Table):
+            deprecations.warn("collect-freshness-return-signature")
+            adapter_response = None
+            table = result
+        else:
+            adapter_response, table = result.response, result.table  # type: ignore[attr-defined]
         # now we have a 1-row table of the maximum `loaded_at_field` value and
         # the current time according to the db.
         if len(table) != 1 or len(table[0]) != 2:
             raise MacroResultError(FRESHNESS_MACRO_NAME, table)
         if table[0][0] is None:
             # no records in the table, so really the max_loaded_at was
             # infinitely long ago. Just call it 0:00 January 1 year UTC
```

### Comparing `dbt-core-1.5.0rc2/dbt/adapters/base/meta.py` & `dbt-core-1.5.1rc1/dbt/adapters/base/meta.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/adapters/base/plugin.py` & `dbt-core-1.5.1rc1/dbt/adapters/base/plugin.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/adapters/base/query_headers.py` & `dbt-core-1.5.1rc1/dbt/adapters/base/query_headers.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/adapters/base/relation.py` & `dbt-core-1.5.1rc1/dbt/adapters/base/relation.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/adapters/cache.py` & `dbt-core-1.5.1rc1/dbt/adapters/cache.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/adapters/factory.py` & `dbt-core-1.5.1rc1/dbt/adapters/factory.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/adapters/protocol.py` & `dbt-core-1.5.1rc1/dbt/adapters/protocol.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/adapters/reference_keys.py` & `dbt-core-1.5.1rc1/dbt/adapters/reference_keys.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/adapters/sql/connections.py` & `dbt-core-1.5.1rc1/dbt/adapters/sql/connections.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/adapters/sql/impl.py` & `dbt-core-1.5.1rc1/dbt/adapters/sql/impl.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/cli/exceptions.py` & `dbt-core-1.5.1rc1/dbt/cli/exceptions.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/cli/flags.py` & `dbt-core-1.5.1rc1/dbt/cli/flags.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/cli/main.py` & `dbt-core-1.5.1rc1/dbt/cli/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -285,21 +285,19 @@
 @p.target
 @p.vars
 @requires.postflight
 @requires.preflight
 @requires.profile
 @requires.project
 @requires.runtime_config
-@requires.manifest
 def docs_serve(ctx, **kwargs):
     """Serve the documentation website for your project"""
     task = ServeTask(
         ctx.obj["flags"],
         ctx.obj["runtime_config"],
-        ctx.obj["manifest"],
     )
 
     results = task.run()
     success = task.interpret_results(results)
     return results, success
```

### Comparing `dbt-core-1.5.0rc2/dbt/cli/option_types.py` & `dbt-core-1.5.1rc1/dbt/cli/option_types.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/cli/options.py` & `dbt-core-1.5.1rc1/dbt/cli/options.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/cli/params.py` & `dbt-core-1.5.1rc1/dbt/cli/params.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/cli/requires.py` & `dbt-core-1.5.1rc1/dbt/cli/requires.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/cli/resolvers.py` & `dbt-core-1.5.1rc1/dbt/cli/resolvers.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/clients/_jinja_blocks.py` & `dbt-core-1.5.1rc1/dbt/clients/_jinja_blocks.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/clients/agate_helper.py` & `dbt-core-1.5.1rc1/dbt/clients/agate_helper.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/clients/git.py` & `dbt-core-1.5.1rc1/dbt/clients/git.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/clients/jinja.py` & `dbt-core-1.5.1rc1/dbt/clients/jinja.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/clients/jinja_static.py` & `dbt-core-1.5.1rc1/dbt/clients/jinja_static.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/clients/registry.py` & `dbt-core-1.5.1rc1/dbt/clients/registry.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/clients/system.py` & `dbt-core-1.5.1rc1/dbt/clients/system.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/clients/yaml_helper.py` & `dbt-core-1.5.1rc1/dbt/clients/yaml_helper.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/compilation.py` & `dbt-core-1.5.1rc1/dbt/compilation.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/config/profile.py` & `dbt-core-1.5.1rc1/dbt/config/profile.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/config/project.py` & `dbt-core-1.5.1rc1/dbt/config/project.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/config/renderer.py` & `dbt-core-1.5.1rc1/dbt/config/renderer.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/config/runtime.py` & `dbt-core-1.5.1rc1/dbt/config/runtime.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/config/selectors.py` & `dbt-core-1.5.1rc1/dbt/config/selectors.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/config/utils.py` & `dbt-core-1.5.1rc1/dbt/config/utils.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/context/base.py` & `dbt-core-1.5.1rc1/dbt/context/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -648,15 +648,15 @@
         > macros/my_log_macro.sql
 
             {% macro some_macro(arg1, arg2) %}
               {{ print("Running some_macro: " ~ arg1 ~ ", " ~ arg2) }}
             {% endmacro %}"
         """
 
-        if not get_flags().PRINT:
+        if get_flags().PRINT:
             print(msg)
         return ""
 
     @contextmember
     @staticmethod
     def diff_of_two_dicts(
         dict_a: Dict[str, List[str]], dict_b: Dict[str, List[str]]
```

### Comparing `dbt-core-1.5.0rc2/dbt/context/configured.py` & `dbt-core-1.5.1rc1/dbt/context/configured.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/context/context_config.py` & `dbt-core-1.5.1rc1/dbt/context/context_config.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/context/docs.py` & `dbt-core-1.5.1rc1/dbt/context/docs.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/context/exceptions_jinja.py` & `dbt-core-1.5.1rc1/dbt/context/exceptions_jinja.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/context/macro_resolver.py` & `dbt-core-1.5.1rc1/dbt/context/macro_resolver.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/context/macros.py` & `dbt-core-1.5.1rc1/dbt/context/macros.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/context/manifest.py` & `dbt-core-1.5.1rc1/dbt/context/manifest.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/context/providers.py` & `dbt-core-1.5.1rc1/dbt/context/providers.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,14 +34,15 @@
     Exposure,
     Metric,
     SeedNode,
     SourceDefinition,
     Resource,
     ManifestNode,
     RefArgs,
+    AccessType,
 )
 from dbt.contracts.graph.metrics import MetricReference, ResolvedMetricReference
 from dbt.contracts.graph.unparsed import NodeVersion
 from dbt.events.functions import get_metadata_vars
 from dbt.exceptions import (
     CompilationError,
     ConflictingConfigKeysError,
@@ -61,19 +62,20 @@
     PackageNotInDepsError,
     ParsingError,
     RefBadContextError,
     RefArgsError,
     DbtRuntimeError,
     TargetNotFoundError,
     DbtValidationError,
+    DbtReferenceError,
 )
 from dbt.config import IsFQNResource
 from dbt.node_types import NodeType, ModelLanguage
 
-from dbt.utils import merge, AttrDict, MultiDict, args_to_dict
+from dbt.utils import merge, AttrDict, MultiDict, args_to_dict, cast_to_str
 
 from dbt import selected_resources
 
 import agate
 
 
 _MISSING = object()
@@ -490,14 +492,25 @@
                 node=self.model,
                 target_name=target_name,
                 target_kind="node",
                 target_package=target_package,
                 target_version=target_version,
                 disabled=isinstance(target_model, Disabled),
             )
+        elif (
+            target_model.resource_type == NodeType.Model
+            and target_model.access == AccessType.Private
+        ):
+            if not self.model.group or self.model.group != target_model.group:
+                raise DbtReferenceError(
+                    unique_id=self.model.unique_id,
+                    ref_unique_id=target_model.unique_id,
+                    group=cast_to_str(target_model.group),
+                )
+
         self.validate(target_model, target_name, target_package, target_version)
         return self.create_relation(target_model)
 
     def create_relation(self, target_model: ManifestNode) -> RelationProxy:
         if target_model.is_ephemeral_model:
             self.model.set_cte(target_model.unique_id, None)
             return self.Relation.create_ephemeral_from_node(self.config, target_model)
```

### Comparing `dbt-core-1.5.0rc2/dbt/context/secret.py` & `dbt-core-1.5.1rc1/dbt/context/secret.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/context/target.py` & `dbt-core-1.5.1rc1/dbt/context/target.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/contracts/connection.py` & `dbt-core-1.5.1rc1/dbt/contracts/connection.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/contracts/files.py` & `dbt-core-1.5.1rc1/dbt/contracts/files.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/contracts/graph/manifest.py` & `dbt-core-1.5.1rc1/dbt/contracts/graph/manifest.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,28 +32,29 @@
     Group,
     UnpatchedSourceDefinition,
     ManifestNode,
     GraphMemberNode,
     ResultNode,
     BaseNode,
 )
-from dbt.contracts.graph.unparsed import SourcePatch, NodeVersion
+from dbt.contracts.graph.unparsed import SourcePatch, NodeVersion, UnparsedVersion
 from dbt.contracts.graph.manifest_upgrade import upgrade_manifest_json
 from dbt.contracts.files import SourceFile, SchemaSourceFile, FileHash, AnySourceFile
 from dbt.contracts.util import BaseArtifactMetadata, SourceKey, ArtifactMixin, schema_version
 from dbt.dataclass_schema import dbtClassMixin
 from dbt.exceptions import (
     CompilationError,
     DuplicateResourceNameError,
     DuplicateMacroInPackageError,
     DuplicateMaterializationNameError,
 )
 from dbt.helper_types import PathSet
 from dbt.events.functions import fire_event
-from dbt.events.types import MergedFromState
+from dbt.events.types import MergedFromState, UnpinnedRefNewVersionAvailable
+from dbt.events.contextvars import get_node_info
 from dbt.node_types import NodeType
 from dbt.flags import get_flags, MP_CONTEXT
 from dbt import tracking
 import dbt.utils
 
 NodeEdgeMap = Dict[str, List[str]]
 PackageName = str
@@ -165,15 +166,40 @@
         key,
         package: Optional[PackageName],
         version: Optional[NodeVersion],
         manifest: "Manifest",
     ):
         unique_id = self.get_unique_id(key, package, version)
         if unique_id is not None:
-            return self.perform_lookup(unique_id, manifest)
+            node = self.perform_lookup(unique_id, manifest)
+            # If this is an unpinned ref (no 'version' arg was passed),
+            # AND this is a versioned node,
+            # AND this ref is being resolved at runtime -- get_node_info != {}
+            if version is None and node.is_versioned and get_node_info():
+                # Check to see if newer versions are available, and log an "FYI" if so
+                max_version: UnparsedVersion = max(
+                    [
+                        UnparsedVersion(v.version)
+                        for v in manifest.nodes.values()
+                        if v.name == node.name and v.version is not None
+                    ]
+                )
+                assert node.latest_version  # for mypy, whenever i may find it
+                if max_version > UnparsedVersion(node.latest_version):
+                    fire_event(
+                        UnpinnedRefNewVersionAvailable(
+                            node_info=get_node_info(),
+                            ref_node_name=node.name,
+                            ref_node_package=node.package_name,
+                            ref_node_version=str(node.version),
+                            ref_max_version=str(max_version.v),
+                        )
+                    )
+
+            return node
         return None
 
     def add_node(self, node: ManifestNode):
         if node.resource_type in self._lookup_types:
             if node.name not in self.storage:
                 self.storage[node.name] = {}
```

### Comparing `dbt-core-1.5.0rc2/dbt/contracts/graph/manifest_upgrade.py` & `dbt-core-1.5.1rc1/dbt/contracts/graph/manifest_upgrade.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/contracts/graph/metrics.py` & `dbt-core-1.5.1rc1/dbt/contracts/graph/metrics.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/contracts/graph/model_config.py` & `dbt-core-1.5.1rc1/dbt/contracts/graph/model_config.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/contracts/graph/nodes.py` & `dbt-core-1.5.1rc1/dbt/contracts/graph/nodes.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/contracts/graph/unparsed.py` & `dbt-core-1.5.1rc1/dbt/contracts/graph/unparsed.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/contracts/graph/utils.py` & `dbt-core-1.5.1rc1/dbt/contracts/graph/utils.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/contracts/project.py` & `dbt-core-1.5.1rc1/dbt/contracts/project.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/contracts/relation.py` & `dbt-core-1.5.1rc1/dbt/contracts/relation.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/contracts/results.py` & `dbt-core-1.5.1rc1/dbt/contracts/results.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/contracts/selection.py` & `dbt-core-1.5.1rc1/dbt/contracts/selection.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/contracts/sql.py` & `dbt-core-1.5.1rc1/dbt/contracts/sql.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/contracts/state.py` & `dbt-core-1.5.1rc1/dbt/contracts/state.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/contracts/util.py` & `dbt-core-1.5.1rc1/dbt/contracts/util.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/dataclass_schema.py` & `dbt-core-1.5.1rc1/dbt/dataclass_schema.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/deprecations.py` & `dbt-core-1.5.1rc1/dbt/deprecations.py`

 * *Files 3% similar despite different names*

```diff
@@ -87,14 +87,19 @@
 
 
 class ConfigTargetPathDeprecation(DBTDeprecation):
     _name = "project-config-target-path"
     _event = "ConfigTargetPathDeprecation"
 
 
+class CollectFreshnessReturnSignature(DBTDeprecation):
+    _name = "collect-freshness-return-signature"
+    _event = "CollectFreshnessReturnSignature"
+
+
 def renamed_env_var(old_name: str, new_name: str):
     class EnvironmentVariableRenamed(DBTDeprecation):
         _name = f"environment-variable-renamed:{old_name}"
         _event = "EnvironmentVariableRenamed"
 
     dep = EnvironmentVariableRenamed()
     deprecations_list.append(dep)
@@ -124,14 +129,15 @@
     PackageInstallPathDeprecation(),
     ConfigSourcePathDeprecation(),
     ConfigDataPathDeprecation(),
     MetricAttributesRenamed(),
     ExposureNameDeprecation(),
     ConfigLogPathDeprecation(),
     ConfigTargetPathDeprecation(),
+    CollectFreshnessReturnSignature(),
 ]
 
 deprecations: Dict[str, DBTDeprecation] = {d.name: d for d in deprecations_list}
 
 
 def reset_deprecations():
     active_deprecations.clear()
```

### Comparing `dbt-core-1.5.0rc2/dbt/deps/base.py` & `dbt-core-1.5.1rc1/dbt/deps/base.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/deps/git.py` & `dbt-core-1.5.1rc1/dbt/deps/git.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/deps/local.py` & `dbt-core-1.5.1rc1/dbt/deps/local.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/deps/registry.py` & `dbt-core-1.5.1rc1/dbt/deps/registry.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/deps/resolver.py` & `dbt-core-1.5.1rc1/dbt/deps/resolver.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/deps/tarball.py` & `dbt-core-1.5.1rc1/dbt/deps/tarball.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/docs/source/_ext/dbt_click.py` & `dbt-core-1.5.1rc1/dbt/docs/source/_ext/dbt_click.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/docs/source/conf.py` & `dbt-core-1.5.1rc1/dbt/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/events/adapter_endpoint.py` & `dbt-core-1.5.1rc1/dbt/events/adapter_endpoint.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/events/base_types.py` & `dbt-core-1.5.1rc1/dbt/events/base_types.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/events/contextvars.py` & `dbt-core-1.5.1rc1/dbt/events/contextvars.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/events/eventmgr.py` & `dbt-core-1.5.1rc1/dbt/events/eventmgr.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/events/format.py` & `dbt-core-1.5.1rc1/dbt/events/format.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/events/functions.py` & `dbt-core-1.5.1rc1/dbt/events/functions.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/events/helpers.py` & `dbt-core-1.5.1rc1/dbt/events/helpers.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/events/types.py` & `dbt-core-1.5.1rc1/dbt/events/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -403,14 +403,27 @@
             f"and will no longer be supported in a future version of dbt-core. "
             f"If you wish to write dbt {output} to a custom directory, please use "
             f"the {cli_flag} CLI flag or {env_var} env var instead."
         )
         return line_wrap_message(warning_tag(f"Deprecated functionality\n\n{description}"))
 
 
+class CollectFreshnessReturnSignature(WarnLevel):
+    def code(self):
+        return "D012"
+
+    def message(self):
+        description = (
+            "The 'collect_freshness' macro signature has changed to return the full "
+            "query result, rather than just a table of values. See the v1.5 migration guide "
+            "for details on how to update your custom macro: https://docs.getdbt.com/guides/migration/versions/upgrading-to-v1.5"
+        )
+        return line_wrap_message(warning_tag(f"Deprecated functionality\n\n{description}"))
+
+
 # =======================================================
 # E - DB Adapter
 # =======================================================
 
 
 class AdapterEventDebug(DebugLevel):
     def code(self):
@@ -1114,14 +1127,31 @@
         return "I063"
 
     def message(self) -> str:
         # This is for the log method used in macros so msg cannot be built here
         return self.msg
 
 
+class UnpinnedRefNewVersionAvailable(InfoLevel):
+    def code(self):
+        return "I064"
+
+    def message(self) -> str:
+        msg = (
+            f"While compiling '{self.node_info.node_name}':\n"
+            f"Found an unpinned reference to versioned model '{self.ref_node_name}' in project '{self.ref_node_package}'.\n"
+            f"Resolving to latest version: {self.ref_node_name}.v{self.ref_node_version}\n"
+            f"A prerelease version {self.ref_max_version} is available. It has not yet been marked 'latest' by its maintainer.\n"
+            f"When that happens, this reference will resolve to {self.ref_node_name}.v{self.ref_max_version} instead.\n\n"
+            f"  Try out v{self.ref_max_version}: {{{{ ref('{self.ref_node_package}', '{self.ref_node_name}', v='{self.ref_max_version}') }}}}\n"
+            f"  Pin to  v{self.ref_node_version}: {{{{ ref('{self.ref_node_package}', '{self.ref_node_name}', v='{self.ref_node_version}') }}}}\n"
+        )
+        return msg
+
+
 # =======================================================
 # M - Deps generation
 # =======================================================
 
 
 class GitSparseCheckoutSubdirectory(DebugLevel):
     def code(self):
```

### Comparing `dbt-core-1.5.0rc2/dbt/events/types_pb2.py` & `dbt-core-1.5.1rc1/dbt/events/types_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 from google.protobuf import struct_pb2 as google_dot_protobuf_dot_struct__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0btypes.proto\x12\x0bproto_types\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1cgoogle/protobuf/struct.proto\"\x91\x02\n\tEventInfo\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04\x63ode\x18\x02 \x01(\t\x12\x0b\n\x03msg\x18\x03 \x01(\t\x12\r\n\x05level\x18\x04 \x01(\t\x12\x15\n\rinvocation_id\x18\x05 \x01(\t\x12\x0b\n\x03pid\x18\x06 \x01(\x05\x12\x0e\n\x06thread\x18\x07 \x01(\t\x12&\n\x02ts\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x30\n\x05\x65xtra\x18\t \x03(\x0b\x32!.proto_types.EventInfo.ExtraEntry\x12\x10\n\x08\x63\x61tegory\x18\n \x01(\t\x1a,\n\nExtraEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\x7f\n\rTimingInfoMsg\x12\x0c\n\x04name\x18\x01 \x01(\t\x12.\n\nstarted_at\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x30\n\x0c\x63ompleted_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"V\n\x0cNodeRelation\x12\x10\n\x08\x64\x61tabase\x18\n \x01(\t\x12\x0e\n\x06schema\x18\x0b \x01(\t\x12\r\n\x05\x61lias\x18\x0c \x01(\t\x12\x15\n\rrelation_name\x18\r \x01(\t\"\x91\x02\n\x08NodeInfo\x12\x11\n\tnode_path\x18\x01 \x01(\t\x12\x11\n\tnode_name\x18\x02 \x01(\t\x12\x11\n\tunique_id\x18\x03 \x01(\t\x12\x15\n\rresource_type\x18\x04 \x01(\t\x12\x14\n\x0cmaterialized\x18\x05 \x01(\t\x12\x13\n\x0bnode_status\x18\x06 \x01(\t\x12\x17\n\x0fnode_started_at\x18\x07 \x01(\t\x12\x18\n\x10node_finished_at\x18\x08 \x01(\t\x12%\n\x04meta\x18\t \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x30\n\rnode_relation\x18\n \x01(\x0b\x32\x19.proto_types.NodeRelation\"\xd1\x01\n\x0cRunResultMsg\x12\x0e\n\x06status\x18\x01 \x01(\t\x12\x0f\n\x07message\x18\x02 \x01(\t\x12/\n\x0btiming_info\x18\x03 \x03(\x0b\x32\x1a.proto_types.TimingInfoMsg\x12\x0e\n\x06thread\x18\x04 \x01(\t\x12\x16\n\x0e\x65xecution_time\x18\x05 \x01(\x02\x12\x31\n\x10\x61\x64\x61pter_response\x18\x06 \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x14\n\x0cnum_failures\x18\x07 \x01(\x05\"G\n\x0fReferenceKeyMsg\x12\x10\n\x08\x64\x61tabase\x18\x01 \x01(\t\x12\x0e\n\x06schema\x18\x02 \x01(\t\x12\x12\n\nidentifier\x18\x03 \x01(\t\"6\n\x0eGenericMessage\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\"9\n\x11MainReportVersion\x12\x0f\n\x07version\x18\x01 \x01(\t\x12\x13\n\x0blog_version\x18\x02 \x01(\x05\"j\n\x14MainReportVersionMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12,\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1e.proto_types.MainReportVersion\"r\n\x0eMainReportArgs\x12\x33\n\x04\x61rgs\x18\x01 \x03(\x0b\x32%.proto_types.MainReportArgs.ArgsEntry\x1a+\n\tArgsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"d\n\x11MainReportArgsMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.MainReportArgs\"+\n\x15MainTrackingUserState\x12\x12\n\nuser_state\x18\x01 \x01(\t\"r\n\x18MainTrackingUserStateMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x30\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\".proto_types.MainTrackingUserState\"5\n\x0fMergedFromState\x12\x12\n\nnum_merged\x18\x01 \x01(\x05\x12\x0e\n\x06sample\x18\x02 \x03(\t\"f\n\x12MergedFromStateMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.MergedFromState\"A\n\x14MissingProfileTarget\x12\x14\n\x0cprofile_name\x18\x01 \x01(\t\x12\x13\n\x0btarget_name\x18\x02 \x01(\t\"p\n\x17MissingProfileTargetMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.MissingProfileTarget\"(\n\x11InvalidOptionYAML\x12\x13\n\x0boption_name\x18\x01 \x01(\t\"j\n\x14InvalidOptionYAMLMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12,\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1e.proto_types.InvalidOptionYAML\"!\n\x12LogDbtProjectError\x12\x0b\n\x03\x65xc\x18\x01 \x01(\t\"l\n\x15LogDbtProjectErrorMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.LogDbtProjectError\"3\n\x12LogDbtProfileError\x12\x0b\n\x03\x65xc\x18\x01 \x01(\t\x12\x10\n\x08profiles\x18\x02 \x03(\t\"l\n\x15LogDbtProfileErrorMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.LogDbtProfileError\"!\n\x12StarterProjectPath\x12\x0b\n\x03\x64ir\x18\x01 \x01(\t\"l\n\x15StarterProjectPathMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.StarterProjectPath\"$\n\x15\x43onfigFolderDirectory\x12\x0b\n\x03\x64ir\x18\x01 \x01(\t\"r\n\x18\x43onfigFolderDirectoryMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x30\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\".proto_types.ConfigFolderDirectory\"\'\n\x14NoSampleProfileFound\x12\x0f\n\x07\x61\x64\x61pter\x18\x01 \x01(\t\"p\n\x17NoSampleProfileFoundMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.NoSampleProfileFound\"6\n\x18ProfileWrittenWithSample\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\"x\n\x1bProfileWrittenWithSampleMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x33\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32%.proto_types.ProfileWrittenWithSample\"B\n$ProfileWrittenWithTargetTemplateYAML\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\"\x90\x01\n\'ProfileWrittenWithTargetTemplateYAMLMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12?\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x31.proto_types.ProfileWrittenWithTargetTemplateYAML\"C\n%ProfileWrittenWithProjectTemplateYAML\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\"\x92\x01\n(ProfileWrittenWithProjectTemplateYAMLMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12@\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x32.proto_types.ProfileWrittenWithProjectTemplateYAML\"\x12\n\x10SettingUpProfile\"h\n\x13SettingUpProfileMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.proto_types.SettingUpProfile\"\x1c\n\x1aInvalidProfileTemplateYAML\"|\n\x1dInvalidProfileTemplateYAMLMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x35\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\'.proto_types.InvalidProfileTemplateYAML\"(\n\x18ProjectNameAlreadyExists\x12\x0c\n\x04name\x18\x01 \x01(\t\"x\n\x1bProjectNameAlreadyExistsMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x33\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32%.proto_types.ProjectNameAlreadyExists\"K\n\x0eProjectCreated\x12\x14\n\x0cproject_name\x18\x01 \x01(\t\x12\x10\n\x08\x64ocs_url\x18\x02 \x01(\t\x12\x11\n\tslack_url\x18\x03 \x01(\t\"d\n\x11ProjectCreatedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.ProjectCreated\"@\n\x1aPackageRedirectDeprecation\x12\x10\n\x08old_name\x18\x01 \x01(\t\x12\x10\n\x08new_name\x18\x02 \x01(\t\"|\n\x1dPackageRedirectDeprecationMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x35\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\'.proto_types.PackageRedirectDeprecation\"\x1f\n\x1dPackageInstallPathDeprecation\"\x82\x01\n PackageInstallPathDeprecationMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x38\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32*.proto_types.PackageInstallPathDeprecation\"H\n\x1b\x43onfigSourcePathDeprecation\x12\x17\n\x0f\x64\x65precated_path\x18\x01 \x01(\t\x12\x10\n\x08\x65xp_path\x18\x02 \x01(\t\"~\n\x1e\x43onfigSourcePathDeprecationMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x36\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32(.proto_types.ConfigSourcePathDeprecation\"F\n\x19\x43onfigDataPathDeprecation\x12\x17\n\x0f\x64\x65precated_path\x18\x01 \x01(\t\x12\x10\n\x08\x65xp_path\x18\x02 \x01(\t\"z\n\x1c\x43onfigDataPathDeprecationMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x34\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32&.proto_types.ConfigDataPathDeprecation\"?\n\x19\x41\x64\x61pterDeprecationWarning\x12\x10\n\x08old_name\x18\x01 \x01(\t\x12\x10\n\x08new_name\x18\x02 \x01(\t\"z\n\x1c\x41\x64\x61pterDeprecationWarningMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x34\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32&.proto_types.AdapterDeprecationWarning\".\n\x17MetricAttributesRenamed\x12\x13\n\x0bmetric_name\x18\x01 \x01(\t\"v\n\x1aMetricAttributesRenamedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x32\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32$.proto_types.MetricAttributesRenamed\"+\n\x17\x45xposureNameDeprecation\x12\x10\n\x08\x65xposure\x18\x01 \x01(\t\"v\n\x1a\x45xposureNameDeprecationMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x32\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32$.proto_types.ExposureNameDeprecation\"^\n\x13InternalDeprecation\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0e\n\x06reason\x18\x02 \x01(\t\x12\x18\n\x10suggested_action\x18\x03 \x01(\t\x12\x0f\n\x07version\x18\x04 \x01(\t\"n\n\x16InternalDeprecationMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32 .proto_types.InternalDeprecation\"@\n\x1a\x45nvironmentVariableRenamed\x12\x10\n\x08old_name\x18\x01 \x01(\t\x12\x10\n\x08new_name\x18\x02 \x01(\t\"|\n\x1d\x45nvironmentVariableRenamedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x35\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\'.proto_types.EnvironmentVariableRenamed\"3\n\x18\x43onfigLogPathDeprecation\x12\x17\n\x0f\x64\x65precated_path\x18\x01 \x01(\t\"x\n\x1b\x43onfigLogPathDeprecationMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x33\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32%.proto_types.ConfigLogPathDeprecation\"6\n\x1b\x43onfigTargetPathDeprecation\x12\x17\n\x0f\x64\x65precated_path\x18\x01 \x01(\t\"~\n\x1e\x43onfigTargetPathDeprecationMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x36\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32(.proto_types.ConfigTargetPathDeprecation\"\x87\x01\n\x11\x41\x64\x61pterEventDebug\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x10\n\x08\x62\x61se_msg\x18\x03 \x01(\t\x12(\n\x04\x61rgs\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.ListValue\"j\n\x14\x41\x64\x61pterEventDebugMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12,\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1e.proto_types.AdapterEventDebug\"\x86\x01\n\x10\x41\x64\x61pterEventInfo\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x10\n\x08\x62\x61se_msg\x18\x03 \x01(\t\x12(\n\x04\x61rgs\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.ListValue\"h\n\x13\x41\x64\x61pterEventInfoMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.proto_types.AdapterEventInfo\"\x89\x01\n\x13\x41\x64\x61pterEventWarning\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x10\n\x08\x62\x61se_msg\x18\x03 \x01(\t\x12(\n\x04\x61rgs\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.ListValue\"n\n\x16\x41\x64\x61pterEventWarningMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32 .proto_types.AdapterEventWarning\"\x99\x01\n\x11\x41\x64\x61pterEventError\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x10\n\x08\x62\x61se_msg\x18\x03 \x01(\t\x12(\n\x04\x61rgs\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.ListValue\x12\x10\n\x08\x65xc_info\x18\x05 \x01(\t\"j\n\x14\x41\x64\x61pterEventErrorMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12,\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1e.proto_types.AdapterEventError\"_\n\rNewConnection\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x11\n\tconn_type\x18\x02 \x01(\t\x12\x11\n\tconn_name\x18\x03 \x01(\t\"b\n\x10NewConnectionMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12(\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1a.proto_types.NewConnection\"=\n\x10\x43onnectionReused\x12\x11\n\tconn_name\x18\x01 \x01(\t\x12\x16\n\x0eorig_conn_name\x18\x02 \x01(\t\"h\n\x13\x43onnectionReusedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.proto_types.ConnectionReused\"0\n\x1b\x43onnectionLeftOpenInCleanup\x12\x11\n\tconn_name\x18\x01 \x01(\t\"~\n\x1e\x43onnectionLeftOpenInCleanupMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x36\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32(.proto_types.ConnectionLeftOpenInCleanup\".\n\x19\x43onnectionClosedInCleanup\x12\x11\n\tconn_name\x18\x01 \x01(\t\"z\n\x1c\x43onnectionClosedInCleanupMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x34\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32&.proto_types.ConnectionClosedInCleanup\"_\n\x0eRollbackFailed\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x11\n\tconn_name\x18\x02 \x01(\t\x12\x10\n\x08\x65xc_info\x18\x03 \x01(\t\"d\n\x11RollbackFailedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.RollbackFailed\"O\n\x10\x43onnectionClosed\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x11\n\tconn_name\x18\x02 \x01(\t\"h\n\x13\x43onnectionClosedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.proto_types.ConnectionClosed\"Q\n\x12\x43onnectionLeftOpen\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x11\n\tconn_name\x18\x02 \x01(\t\"l\n\x15\x43onnectionLeftOpenMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.ConnectionLeftOpen\"G\n\x08Rollback\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x11\n\tconn_name\x18\x02 \x01(\t\"X\n\x0bRollbackMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12#\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x15.proto_types.Rollback\"@\n\tCacheMiss\x12\x11\n\tconn_name\x18\x01 \x01(\t\x12\x10\n\x08\x64\x61tabase\x18\x02 \x01(\t\x12\x0e\n\x06schema\x18\x03 \x01(\t\"Z\n\x0c\x43\x61\x63heMissMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12$\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x16.proto_types.CacheMiss\"b\n\rListRelations\x12\x10\n\x08\x64\x61tabase\x18\x01 \x01(\t\x12\x0e\n\x06schema\x18\x02 \x01(\t\x12/\n\trelations\x18\x03 \x03(\x0b\x32\x1c.proto_types.ReferenceKeyMsg\"b\n\x10ListRelationsMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12(\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1a.proto_types.ListRelations\"`\n\x0e\x43onnectionUsed\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x11\n\tconn_type\x18\x02 \x01(\t\x12\x11\n\tconn_name\x18\x03 \x01(\t\"d\n\x11\x43onnectionUsedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.ConnectionUsed\"T\n\x08SQLQuery\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x11\n\tconn_name\x18\x02 \x01(\t\x12\x0b\n\x03sql\x18\x03 \x01(\t\"X\n\x0bSQLQueryMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12#\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x15.proto_types.SQLQuery\"[\n\x0eSQLQueryStatus\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x0e\n\x06status\x18\x02 \x01(\t\x12\x0f\n\x07\x65lapsed\x18\x03 \x01(\x02\"d\n\x11SQLQueryStatusMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.SQLQueryStatus\"H\n\tSQLCommit\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x11\n\tconn_name\x18\x02 \x01(\t\"Z\n\x0cSQLCommitMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12$\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x16.proto_types.SQLCommit\"a\n\rColTypeChange\x12\x11\n\torig_type\x18\x01 \x01(\t\x12\x10\n\x08new_type\x18\x02 \x01(\t\x12+\n\x05table\x18\x03 \x01(\x0b\x32\x1c.proto_types.ReferenceKeyMsg\"b\n\x10\x43olTypeChangeMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12(\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1a.proto_types.ColTypeChange\"@\n\x0eSchemaCreation\x12.\n\x08relation\x18\x01 \x01(\x0b\x32\x1c.proto_types.ReferenceKeyMsg\"d\n\x11SchemaCreationMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.SchemaCreation\"<\n\nSchemaDrop\x12.\n\x08relation\x18\x01 \x01(\x0b\x32\x1c.proto_types.ReferenceKeyMsg\"\\\n\rSchemaDropMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12%\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x17.proto_types.SchemaDrop\"\xde\x01\n\x0b\x43\x61\x63heAction\x12\x0e\n\x06\x61\x63tion\x18\x01 \x01(\t\x12-\n\x07ref_key\x18\x02 \x01(\x0b\x32\x1c.proto_types.ReferenceKeyMsg\x12/\n\tref_key_2\x18\x03 \x01(\x0b\x32\x1c.proto_types.ReferenceKeyMsg\x12/\n\tref_key_3\x18\x04 \x01(\x0b\x32\x1c.proto_types.ReferenceKeyMsg\x12.\n\x08ref_list\x18\x05 \x03(\x0b\x32\x1c.proto_types.ReferenceKeyMsg\"^\n\x0e\x43\x61\x63heActionMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12&\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x18.proto_types.CacheAction\"\x98\x01\n\x0e\x43\x61\x63heDumpGraph\x12\x33\n\x04\x64ump\x18\x01 \x03(\x0b\x32%.proto_types.CacheDumpGraph.DumpEntry\x12\x14\n\x0c\x62\x65\x66ore_after\x18\x02 \x01(\t\x12\x0e\n\x06\x61\x63tion\x18\x03 \x01(\t\x1a+\n\tDumpEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"d\n\x11\x43\x61\x63heDumpGraphMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.CacheDumpGraph\"!\n\x12\x41\x64\x61pterImportError\x12\x0b\n\x03\x65xc\x18\x01 \x01(\t\"l\n\x15\x41\x64\x61pterImportErrorMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.AdapterImportError\"#\n\x0fPluginLoadError\x12\x10\n\x08\x65xc_info\x18\x01 \x01(\t\"f\n\x12PluginLoadErrorMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.PluginLoadError\"Z\n\x14NewConnectionOpening\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x18\n\x10\x63onnection_state\x18\x02 \x01(\t\"p\n\x17NewConnectionOpeningMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.NewConnectionOpening\"8\n\rCodeExecution\x12\x11\n\tconn_name\x18\x01 \x01(\t\x12\x14\n\x0c\x63ode_content\x18\x02 \x01(\t\"b\n\x10\x43odeExecutionMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12(\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1a.proto_types.CodeExecution\"6\n\x13\x43odeExecutionStatus\x12\x0e\n\x06status\x18\x01 \x01(\t\x12\x0f\n\x07\x65lapsed\x18\x02 \x01(\x02\"n\n\x16\x43odeExecutionStatusMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32 .proto_types.CodeExecutionStatus\"%\n\x16\x43\x61talogGenerationError\x12\x0b\n\x03\x65xc\x18\x01 \x01(\t\"t\n\x19\x43\x61talogGenerationErrorMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x31\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32#.proto_types.CatalogGenerationError\"-\n\x13WriteCatalogFailure\x12\x16\n\x0enum_exceptions\x18\x01 \x01(\x05\"n\n\x16WriteCatalogFailureMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32 .proto_types.WriteCatalogFailure\"\x1e\n\x0e\x43\x61talogWritten\x12\x0c\n\x04path\x18\x01 \x01(\t\"d\n\x11\x43\x61talogWrittenMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.CatalogWritten\"\x14\n\x12\x43\x61nnotGenerateDocs\"l\n\x15\x43\x61nnotGenerateDocsMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.CannotGenerateDocs\"\x11\n\x0f\x42uildingCatalog\"f\n\x12\x42uildingCatalogMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.BuildingCatalog\"-\n\x18\x44\x61tabaseErrorRunningHook\x12\x11\n\thook_type\x18\x01 \x01(\t\"x\n\x1b\x44\x61tabaseErrorRunningHookMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x33\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32%.proto_types.DatabaseErrorRunningHook\"4\n\x0cHooksRunning\x12\x11\n\tnum_hooks\x18\x01 \x01(\x05\x12\x11\n\thook_type\x18\x02 \x01(\t\"`\n\x0fHooksRunningMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\'\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x19.proto_types.HooksRunning\"T\n\x14\x46inishedRunningStats\x12\x11\n\tstat_line\x18\x01 \x01(\t\x12\x11\n\texecution\x18\x02 \x01(\t\x12\x16\n\x0e\x65xecution_time\x18\x03 \x01(\x02\"p\n\x17\x46inishedRunningStatsMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.FinishedRunningStats\"<\n\x15\x43onstraintNotEnforced\x12\x12\n\nconstraint\x18\x01 \x01(\t\x12\x0f\n\x07\x61\x64\x61pter\x18\x02 \x01(\t\"r\n\x18\x43onstraintNotEnforcedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x30\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\".proto_types.ConstraintNotEnforced\"=\n\x16\x43onstraintNotSupported\x12\x12\n\nconstraint\x18\x01 \x01(\t\x12\x0f\n\x07\x61\x64\x61pter\x18\x02 \x01(\t\"t\n\x19\x43onstraintNotSupportedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x31\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32#.proto_types.ConstraintNotSupported\"7\n\x12InputFileDiffError\x12\x10\n\x08\x63\x61tegory\x18\x01 \x01(\t\x12\x0f\n\x07\x66ile_id\x18\x02 \x01(\t\"l\n\x15InputFileDiffErrorMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.InputFileDiffError\"?\n\x14InvalidValueForField\x12\x12\n\nfield_name\x18\x01 \x01(\t\x12\x13\n\x0b\x66ield_value\x18\x02 \x01(\t\"p\n\x17InvalidValueForFieldMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.InvalidValueForField\"Q\n\x11ValidationWarning\x12\x15\n\rresource_type\x18\x01 \x01(\t\x12\x12\n\nfield_name\x18\x02 \x01(\t\x12\x11\n\tnode_name\x18\x03 \x01(\t\"j\n\x14ValidationWarningMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12,\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1e.proto_types.ValidationWarning\"!\n\x11ParsePerfInfoPath\x12\x0c\n\x04path\x18\x01 \x01(\t\"j\n\x14ParsePerfInfoPathMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12,\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1e.proto_types.ParsePerfInfoPath\"$\n\x14GenericTestFileParse\x12\x0c\n\x04path\x18\x01 \x01(\t\"p\n\x17GenericTestFileParseMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.GenericTestFileParse\"\x1e\n\x0eMacroFileParse\x12\x0c\n\x04path\x18\x01 \x01(\t\"d\n\x11MacroFileParseMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.MacroFileParse\"1\n!PartialParsingErrorProcessingFile\x12\x0c\n\x04\x66ile\x18\x01 \x01(\t\"\x8a\x01\n$PartialParsingErrorProcessingFileMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12<\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32..proto_types.PartialParsingErrorProcessingFile\"\x86\x01\n\x13PartialParsingError\x12?\n\x08\x65xc_info\x18\x01 \x03(\x0b\x32-.proto_types.PartialParsingError.ExcInfoEntry\x1a.\n\x0c\x45xcInfoEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"n\n\x16PartialParsingErrorMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32 .proto_types.PartialParsingError\"\x1b\n\x19PartialParsingSkipParsing\"z\n\x1cPartialParsingSkipParsingMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x34\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32&.proto_types.PartialParsingSkipParsing\"&\n\x14UnableToPartialParse\x12\x0e\n\x06reason\x18\x01 \x01(\t\"p\n\x17UnableToPartialParseMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.UnableToPartialParse\"f\n\x12StateCheckVarsHash\x12\x10\n\x08\x63hecksum\x18\x01 \x01(\t\x12\x0c\n\x04vars\x18\x02 \x01(\t\x12\x0f\n\x07profile\x18\x03 \x01(\t\x12\x0e\n\x06target\x18\x04 \x01(\t\x12\x0f\n\x07version\x18\x05 \x01(\t\"l\n\x15StateCheckVarsHashMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.StateCheckVarsHash\"\x1a\n\x18PartialParsingNotEnabled\"x\n\x1bPartialParsingNotEnabledMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x33\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32%.proto_types.PartialParsingNotEnabled\"C\n\x14ParsedFileLoadFailed\x12\x0c\n\x04path\x18\x01 \x01(\t\x12\x0b\n\x03\x65xc\x18\x02 \x01(\t\x12\x10\n\x08\x65xc_info\x18\x03 \x01(\t\"p\n\x17ParsedFileLoadFailedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.ParsedFileLoadFailed\"H\n\x15PartialParsingEnabled\x12\x0f\n\x07\x64\x65leted\x18\x01 \x01(\x05\x12\r\n\x05\x61\x64\x64\x65\x64\x18\x02 \x01(\x05\x12\x0f\n\x07\x63hanged\x18\x03 \x01(\x05\"r\n\x18PartialParsingEnabledMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x30\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\".proto_types.PartialParsingEnabled\"8\n\x12PartialParsingFile\x12\x0f\n\x07\x66ile_id\x18\x01 \x01(\t\x12\x11\n\toperation\x18\x02 \x01(\t\"l\n\x15PartialParsingFileMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.PartialParsingFile\"\xaf\x01\n\x1fInvalidDisabledTargetInTestNode\x12\x1b\n\x13resource_type_title\x18\x01 \x01(\t\x12\x11\n\tunique_id\x18\x02 \x01(\t\x12\x1a\n\x12original_file_path\x18\x03 \x01(\t\x12\x13\n\x0btarget_kind\x18\x04 \x01(\t\x12\x13\n\x0btarget_name\x18\x05 \x01(\t\x12\x16\n\x0etarget_package\x18\x06 \x01(\t\"\x86\x01\n\"InvalidDisabledTargetInTestNodeMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12:\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32,.proto_types.InvalidDisabledTargetInTestNode\"7\n\x18UnusedResourceConfigPath\x12\x1b\n\x13unused_config_paths\x18\x01 \x03(\t\"x\n\x1bUnusedResourceConfigPathMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x33\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32%.proto_types.UnusedResourceConfigPath\"3\n\rSeedIncreased\x12\x14\n\x0cpackage_name\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\"b\n\x10SeedIncreasedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12(\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1a.proto_types.SeedIncreased\">\n\x18SeedExceedsLimitSamePath\x12\x14\n\x0cpackage_name\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\"x\n\x1bSeedExceedsLimitSamePathMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x33\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32%.proto_types.SeedExceedsLimitSamePath\"D\n\x1eSeedExceedsLimitAndPathChanged\x12\x14\n\x0cpackage_name\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\"\x84\x01\n!SeedExceedsLimitAndPathChangedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x39\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32+.proto_types.SeedExceedsLimitAndPathChanged\"\\\n\x1fSeedExceedsLimitChecksumChanged\x12\x14\n\x0cpackage_name\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x15\n\rchecksum_name\x18\x03 \x01(\t\"\x86\x01\n\"SeedExceedsLimitChecksumChangedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12:\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32,.proto_types.SeedExceedsLimitChecksumChanged\"%\n\x0cUnusedTables\x12\x15\n\runused_tables\x18\x01 \x03(\t\"`\n\x0fUnusedTablesMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\'\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x19.proto_types.UnusedTables\"\x87\x01\n\x17WrongResourceSchemaFile\x12\x12\n\npatch_name\x18\x01 \x01(\t\x12\x15\n\rresource_type\x18\x02 \x01(\t\x12\x1c\n\x14plural_resource_type\x18\x03 \x01(\t\x12\x10\n\x08yaml_key\x18\x04 \x01(\t\x12\x11\n\tfile_path\x18\x05 \x01(\t\"v\n\x1aWrongResourceSchemaFileMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x32\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32$.proto_types.WrongResourceSchemaFile\"K\n\x10NoNodeForYamlKey\x12\x12\n\npatch_name\x18\x01 \x01(\t\x12\x10\n\x08yaml_key\x18\x02 \x01(\t\x12\x11\n\tfile_path\x18\x03 \x01(\t\"h\n\x13NoNodeForYamlKeyMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.proto_types.NoNodeForYamlKey\"+\n\x15MacroNotFoundForPatch\x12\x12\n\npatch_name\x18\x01 \x01(\t\"r\n\x18MacroNotFoundForPatchMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x30\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\".proto_types.MacroNotFoundForPatch\"\xb8\x01\n\x16NodeNotFoundOrDisabled\x12\x1a\n\x12original_file_path\x18\x01 \x01(\t\x12\x11\n\tunique_id\x18\x02 \x01(\t\x12\x1b\n\x13resource_type_title\x18\x03 \x01(\t\x12\x13\n\x0btarget_name\x18\x04 \x01(\t\x12\x13\n\x0btarget_kind\x18\x05 \x01(\t\x12\x16\n\x0etarget_package\x18\x06 \x01(\t\x12\x10\n\x08\x64isabled\x18\x07 \x01(\t\"t\n\x19NodeNotFoundOrDisabledMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x31\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32#.proto_types.NodeNotFoundOrDisabled\"H\n\x0fJinjaLogWarning\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x0b\n\x03msg\x18\x02 \x01(\t\"f\n\x12JinjaLogWarningMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.JinjaLogWarning\"E\n\x0cJinjaLogInfo\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x0b\n\x03msg\x18\x02 \x01(\t\"`\n\x0fJinjaLogInfoMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\'\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x19.proto_types.JinjaLogInfo\"F\n\rJinjaLogDebug\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x0b\n\x03msg\x18\x02 \x01(\t\"b\n\x10JinjaLogDebugMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12(\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1a.proto_types.JinjaLogDebug\"/\n\x1dGitSparseCheckoutSubdirectory\x12\x0e\n\x06subdir\x18\x01 \x01(\t\"\x82\x01\n GitSparseCheckoutSubdirectoryMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x38\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32*.proto_types.GitSparseCheckoutSubdirectory\"/\n\x1bGitProgressCheckoutRevision\x12\x10\n\x08revision\x18\x01 \x01(\t\"~\n\x1eGitProgressCheckoutRevisionMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x36\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32(.proto_types.GitProgressCheckoutRevision\"4\n%GitProgressUpdatingExistingDependency\x12\x0b\n\x03\x64ir\x18\x01 \x01(\t\"\x92\x01\n(GitProgressUpdatingExistingDependencyMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12@\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x32.proto_types.GitProgressUpdatingExistingDependency\".\n\x1fGitProgressPullingNewDependency\x12\x0b\n\x03\x64ir\x18\x01 \x01(\t\"\x86\x01\n\"GitProgressPullingNewDependencyMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12:\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32,.proto_types.GitProgressPullingNewDependency\"\x1d\n\x0eGitNothingToDo\x12\x0b\n\x03sha\x18\x01 \x01(\t\"d\n\x11GitNothingToDoMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.GitNothingToDo\"E\n\x1fGitProgressUpdatedCheckoutRange\x12\x11\n\tstart_sha\x18\x01 \x01(\t\x12\x0f\n\x07\x65nd_sha\x18\x02 \x01(\t\"\x86\x01\n\"GitProgressUpdatedCheckoutRangeMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12:\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32,.proto_types.GitProgressUpdatedCheckoutRange\"*\n\x17GitProgressCheckedOutAt\x12\x0f\n\x07\x65nd_sha\x18\x01 \x01(\t\"v\n\x1aGitProgressCheckedOutAtMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x32\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32$.proto_types.GitProgressCheckedOutAt\")\n\x1aRegistryProgressGETRequest\x12\x0b\n\x03url\x18\x01 \x01(\t\"|\n\x1dRegistryProgressGETRequestMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x35\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\'.proto_types.RegistryProgressGETRequest\"=\n\x1bRegistryProgressGETResponse\x12\x0b\n\x03url\x18\x01 \x01(\t\x12\x11\n\tresp_code\x18\x02 \x01(\x05\"~\n\x1eRegistryProgressGETResponseMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x36\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32(.proto_types.RegistryProgressGETResponse\"_\n\x1dSelectorReportInvalidSelector\x12\x17\n\x0fvalid_selectors\x18\x01 \x01(\t\x12\x13\n\x0bspec_method\x18\x02 \x01(\t\x12\x10\n\x08raw_spec\x18\x03 \x01(\t\"\x82\x01\n SelectorReportInvalidSelectorMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x38\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32*.proto_types.SelectorReportInvalidSelector\"\x15\n\x13\x44\x65psNoPackagesFound\"n\n\x16\x44\x65psNoPackagesFoundMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32 .proto_types.DepsNoPackagesFound\"/\n\x17\x44\x65psStartPackageInstall\x12\x14\n\x0cpackage_name\x18\x01 \x01(\t\"v\n\x1a\x44\x65psStartPackageInstallMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x32\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32$.proto_types.DepsStartPackageInstall\"\'\n\x0f\x44\x65psInstallInfo\x12\x14\n\x0cversion_name\x18\x01 \x01(\t\"f\n\x12\x44\x65psInstallInfoMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.DepsInstallInfo\"-\n\x13\x44\x65psUpdateAvailable\x12\x16\n\x0eversion_latest\x18\x01 \x01(\t\"n\n\x16\x44\x65psUpdateAvailableMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32 .proto_types.DepsUpdateAvailable\"\x0e\n\x0c\x44\x65psUpToDate\"`\n\x0f\x44\x65psUpToDateMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\'\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x19.proto_types.DepsUpToDate\",\n\x14\x44\x65psListSubdirectory\x12\x14\n\x0csubdirectory\x18\x01 \x01(\t\"p\n\x17\x44\x65psListSubdirectoryMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.DepsListSubdirectory\".\n\x1a\x44\x65psNotifyUpdatesAvailable\x12\x10\n\x08packages\x18\x01 \x03(\t\"|\n\x1d\x44\x65psNotifyUpdatesAvailableMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x35\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\'.proto_types.DepsNotifyUpdatesAvailable\"1\n\x11RetryExternalCall\x12\x0f\n\x07\x61ttempt\x18\x01 \x01(\x05\x12\x0b\n\x03max\x18\x02 \x01(\x05\"j\n\x14RetryExternalCallMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12,\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1e.proto_types.RetryExternalCall\"#\n\x14RecordRetryException\x12\x0b\n\x03\x65xc\x18\x01 \x01(\t\"p\n\x17RecordRetryExceptionMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.RecordRetryException\".\n\x1fRegistryIndexProgressGETRequest\x12\x0b\n\x03url\x18\x01 \x01(\t\"\x86\x01\n\"RegistryIndexProgressGETRequestMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12:\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32,.proto_types.RegistryIndexProgressGETRequest\"B\n RegistryIndexProgressGETResponse\x12\x0b\n\x03url\x18\x01 \x01(\t\x12\x11\n\tresp_code\x18\x02 \x01(\x05\"\x88\x01\n#RegistryIndexProgressGETResponseMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12;\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32-.proto_types.RegistryIndexProgressGETResponse\"2\n\x1eRegistryResponseUnexpectedType\x12\x10\n\x08response\x18\x01 \x01(\t\"\x84\x01\n!RegistryResponseUnexpectedTypeMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x39\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32+.proto_types.RegistryResponseUnexpectedType\"2\n\x1eRegistryResponseMissingTopKeys\x12\x10\n\x08response\x18\x01 \x01(\t\"\x84\x01\n!RegistryResponseMissingTopKeysMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x39\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32+.proto_types.RegistryResponseMissingTopKeys\"5\n!RegistryResponseMissingNestedKeys\x12\x10\n\x08response\x18\x01 \x01(\t\"\x8a\x01\n$RegistryResponseMissingNestedKeysMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12<\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32..proto_types.RegistryResponseMissingNestedKeys\"3\n\x1fRegistryResponseExtraNestedKeys\x12\x10\n\x08response\x18\x01 \x01(\t\"\x86\x01\n\"RegistryResponseExtraNestedKeysMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12:\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32,.proto_types.RegistryResponseExtraNestedKeys\"(\n\x18\x44\x65psSetDownloadDirectory\x12\x0c\n\x04path\x18\x01 \x01(\t\"x\n\x1b\x44\x65psSetDownloadDirectoryMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x33\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32%.proto_types.DepsSetDownloadDirectory\"-\n\x0c\x44\x65psUnpinned\x12\x10\n\x08revision\x18\x01 \x01(\t\x12\x0b\n\x03git\x18\x02 \x01(\t\"`\n\x0f\x44\x65psUnpinnedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\'\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x19.proto_types.DepsUnpinned\"/\n\x1bNoNodesForSelectionCriteria\x12\x10\n\x08spec_raw\x18\x01 \x01(\t\"~\n\x1eNoNodesForSelectionCriteriaMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x36\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32(.proto_types.NoNodesForSelectionCriteria\"*\n\x1bRunningOperationCaughtError\x12\x0b\n\x03\x65xc\x18\x01 \x01(\t\"~\n\x1eRunningOperationCaughtErrorMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x36\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32(.proto_types.RunningOperationCaughtError\"\x11\n\x0f\x43ompileComplete\"f\n\x12\x43ompileCompleteMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.CompileComplete\"\x18\n\x16\x46reshnessCheckComplete\"t\n\x19\x46reshnessCheckCompleteMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x31\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32#.proto_types.FreshnessCheckComplete\"\x1c\n\nSeedHeader\x12\x0e\n\x06header\x18\x01 \x01(\t\"\\\n\rSeedHeaderMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12%\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x17.proto_types.SeedHeader\"3\n\x12SQLRunnerException\x12\x0b\n\x03\x65xc\x18\x01 \x01(\t\x12\x10\n\x08\x65xc_info\x18\x02 \x01(\t\"l\n\x15SQLRunnerExceptionMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.SQLRunnerException\"\xa8\x01\n\rLogTestResult\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0e\n\x06status\x18\x03 \x01(\t\x12\r\n\x05index\x18\x04 \x01(\x05\x12\x12\n\nnum_models\x18\x05 \x01(\x05\x12\x16\n\x0e\x65xecution_time\x18\x06 \x01(\x02\x12\x14\n\x0cnum_failures\x18\x07 \x01(\x05\"b\n\x10LogTestResultMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12(\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1a.proto_types.LogTestResult\"k\n\x0cLogStartLine\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\r\n\x05index\x18\x03 \x01(\x05\x12\r\n\x05total\x18\x04 \x01(\x05\"`\n\x0fLogStartLineMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\'\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x19.proto_types.LogStartLine\"\x95\x01\n\x0eLogModelResult\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x0e\n\x06status\x18\x03 \x01(\t\x12\r\n\x05index\x18\x04 \x01(\x05\x12\r\n\x05total\x18\x05 \x01(\x05\x12\x16\n\x0e\x65xecution_time\x18\x06 \x01(\x02\"d\n\x11LogModelResultMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.LogModelResult\"\xfa\x01\n\x11LogSnapshotResult\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x0e\n\x06status\x18\x03 \x01(\t\x12\r\n\x05index\x18\x04 \x01(\x05\x12\r\n\x05total\x18\x05 \x01(\x05\x12\x16\n\x0e\x65xecution_time\x18\x06 \x01(\x02\x12\x34\n\x03\x63\x66g\x18\x07 \x03(\x0b\x32\'.proto_types.LogSnapshotResult.CfgEntry\x1a*\n\x08\x43\x66gEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"j\n\x14LogSnapshotResultMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12,\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1e.proto_types.LogSnapshotResult\"\xb9\x01\n\rLogSeedResult\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x0e\n\x06status\x18\x02 \x01(\t\x12\x16\n\x0eresult_message\x18\x03 \x01(\t\x12\r\n\x05index\x18\x04 \x01(\x05\x12\r\n\x05total\x18\x05 \x01(\x05\x12\x16\n\x0e\x65xecution_time\x18\x06 \x01(\x02\x12\x0e\n\x06schema\x18\x07 \x01(\t\x12\x10\n\x08relation\x18\x08 \x01(\t\"b\n\x10LogSeedResultMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12(\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1a.proto_types.LogSeedResult\"\xad\x01\n\x12LogFreshnessResult\x12\x0e\n\x06status\x18\x01 \x01(\t\x12(\n\tnode_info\x18\x02 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\r\n\x05index\x18\x03 \x01(\x05\x12\r\n\x05total\x18\x04 \x01(\x05\x12\x16\n\x0e\x65xecution_time\x18\x05 \x01(\x02\x12\x13\n\x0bsource_name\x18\x06 \x01(\t\x12\x12\n\ntable_name\x18\x07 \x01(\t\"l\n\x15LogFreshnessResultMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.LogFreshnessResult\"\"\n\rLogCancelLine\x12\x11\n\tconn_name\x18\x01 \x01(\t\"b\n\x10LogCancelLineMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12(\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1a.proto_types.LogCancelLine\"\x1f\n\x0f\x44\x65\x66\x61ultSelector\x12\x0c\n\x04name\x18\x01 \x01(\t\"f\n\x12\x44\x65\x66\x61ultSelectorMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.DefaultSelector\"5\n\tNodeStart\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\"Z\n\x0cNodeStartMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12$\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x16.proto_types.NodeStart\"g\n\x0cNodeFinished\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12-\n\nrun_result\x18\x02 \x01(\x0b\x32\x19.proto_types.RunResultMsg\"`\n\x0fNodeFinishedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\'\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x19.proto_types.NodeFinished\"+\n\x1bQueryCancelationUnsupported\x12\x0c\n\x04type\x18\x01 \x01(\t\"~\n\x1eQueryCancelationUnsupportedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x36\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32(.proto_types.QueryCancelationUnsupported\"O\n\x0f\x43oncurrencyLine\x12\x13\n\x0bnum_threads\x18\x01 \x01(\x05\x12\x13\n\x0btarget_name\x18\x02 \x01(\t\x12\x12\n\nnode_count\x18\x03 \x01(\x05\"f\n\x12\x43oncurrencyLineMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.ConcurrencyLine\"E\n\x19WritingInjectedSQLForNode\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\"z\n\x1cWritingInjectedSQLForNodeMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x34\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32&.proto_types.WritingInjectedSQLForNode\"9\n\rNodeCompiling\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\"b\n\x10NodeCompilingMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12(\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1a.proto_types.NodeCompiling\"9\n\rNodeExecuting\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\"b\n\x10NodeExecutingMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12(\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1a.proto_types.NodeExecuting\"m\n\x10LogHookStartLine\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x11\n\tstatement\x18\x02 \x01(\t\x12\r\n\x05index\x18\x03 \x01(\x05\x12\r\n\x05total\x18\x04 \x01(\x05\"h\n\x13LogHookStartLineMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.proto_types.LogHookStartLine\"\x93\x01\n\x0eLogHookEndLine\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x11\n\tstatement\x18\x02 \x01(\t\x12\x0e\n\x06status\x18\x03 \x01(\t\x12\r\n\x05index\x18\x04 \x01(\x05\x12\r\n\x05total\x18\x05 \x01(\x05\x12\x16\n\x0e\x65xecution_time\x18\x06 \x01(\x02\"d\n\x11LogHookEndLineMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.LogHookEndLine\"\x93\x01\n\x0fSkippingDetails\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x15\n\rresource_type\x18\x02 \x01(\t\x12\x0e\n\x06schema\x18\x03 \x01(\t\x12\x11\n\tnode_name\x18\x04 \x01(\t\x12\r\n\x05index\x18\x05 \x01(\x05\x12\r\n\x05total\x18\x06 \x01(\x05\"f\n\x12SkippingDetailsMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.SkippingDetails\"\r\n\x0bNothingToDo\"^\n\x0eNothingToDoMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12&\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x18.proto_types.NothingToDo\",\n\x1dRunningOperationUncaughtError\x12\x0b\n\x03\x65xc\x18\x01 \x01(\t\"\x82\x01\n RunningOperationUncaughtErrorMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x38\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32*.proto_types.RunningOperationUncaughtError\"\x93\x01\n\x0c\x45ndRunResult\x12*\n\x07results\x18\x01 \x03(\x0b\x32\x19.proto_types.RunResultMsg\x12\x14\n\x0c\x65lapsed_time\x18\x02 \x01(\x02\x12\x30\n\x0cgenerated_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0f\n\x07success\x18\x04 \x01(\x08\"`\n\x0f\x45ndRunResultMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\'\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x19.proto_types.EndRunResult\"\x11\n\x0fNoNodesSelected\"f\n\x12NoNodesSelectedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.NoNodesSelected\"w\n\x10\x43ommandCompleted\x12\x0f\n\x07\x63ommand\x18\x01 \x01(\t\x12\x0f\n\x07success\x18\x02 \x01(\x08\x12\x30\n\x0c\x63ompleted_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0f\n\x07\x65lapsed\x18\x04 \x01(\x02\"h\n\x13\x43ommandCompletedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.proto_types.CommandCompleted\"k\n\x08ShowNode\x12\x11\n\tnode_name\x18\x01 \x01(\t\x12\x0f\n\x07preview\x18\x02 \x01(\t\x12\x11\n\tis_inline\x18\x03 \x01(\x08\x12\x15\n\routput_format\x18\x04 \x01(\t\x12\x11\n\tunique_id\x18\x05 \x01(\t\"X\n\x0bShowNodeMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12#\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x15.proto_types.ShowNode\"p\n\x0c\x43ompiledNode\x12\x11\n\tnode_name\x18\x01 \x01(\t\x12\x10\n\x08\x63ompiled\x18\x02 \x01(\t\x12\x11\n\tis_inline\x18\x03 \x01(\x08\x12\x15\n\routput_format\x18\x04 \x01(\t\x12\x11\n\tunique_id\x18\x05 \x01(\t\"`\n\x0f\x43ompiledNodeMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\'\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x19.proto_types.CompiledNode\"b\n\x17\x43\x61tchableExceptionOnRun\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x0b\n\x03\x65xc\x18\x02 \x01(\t\x12\x10\n\x08\x65xc_info\x18\x03 \x01(\t\"v\n\x1a\x43\x61tchableExceptionOnRunMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x32\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32$.proto_types.CatchableExceptionOnRun\"5\n\x12InternalErrorOnRun\x12\x12\n\nbuild_path\x18\x01 \x01(\t\x12\x0b\n\x03\x65xc\x18\x02 \x01(\t\"l\n\x15InternalErrorOnRunMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.InternalErrorOnRun\"K\n\x15GenericExceptionOnRun\x12\x12\n\nbuild_path\x18\x01 \x01(\t\x12\x11\n\tunique_id\x18\x02 \x01(\t\x12\x0b\n\x03\x65xc\x18\x03 \x01(\t\"r\n\x18GenericExceptionOnRunMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x30\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\".proto_types.GenericExceptionOnRun\"N\n\x1aNodeConnectionReleaseError\x12\x11\n\tnode_name\x18\x01 \x01(\t\x12\x0b\n\x03\x65xc\x18\x02 \x01(\t\x12\x10\n\x08\x65xc_info\x18\x03 \x01(\t\"|\n\x1dNodeConnectionReleaseErrorMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x35\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\'.proto_types.NodeConnectionReleaseError\"\x1f\n\nFoundStats\x12\x11\n\tstat_line\x18\x01 \x01(\t\"\\\n\rFoundStatsMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12%\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x17.proto_types.FoundStats\"\x17\n\x15MainKeyboardInterrupt\"r\n\x18MainKeyboardInterruptMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x30\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\".proto_types.MainKeyboardInterrupt\"#\n\x14MainEncounteredError\x12\x0b\n\x03\x65xc\x18\x01 \x01(\t\"p\n\x17MainEncounteredErrorMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.MainEncounteredError\"%\n\x0eMainStackTrace\x12\x13\n\x0bstack_trace\x18\x01 \x01(\t\"d\n\x11MainStackTraceMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.MainStackTrace\"@\n\x13SystemCouldNotWrite\x12\x0c\n\x04path\x18\x01 \x01(\t\x12\x0e\n\x06reason\x18\x02 \x01(\t\x12\x0b\n\x03\x65xc\x18\x03 \x01(\t\"n\n\x16SystemCouldNotWriteMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32 .proto_types.SystemCouldNotWrite\"!\n\x12SystemExecutingCmd\x12\x0b\n\x03\x63md\x18\x01 \x03(\t\"l\n\x15SystemExecutingCmdMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.SystemExecutingCmd\"\x1c\n\x0cSystemStdOut\x12\x0c\n\x04\x62msg\x18\x01 \x01(\t\"`\n\x0fSystemStdOutMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\'\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x19.proto_types.SystemStdOut\"\x1c\n\x0cSystemStdErr\x12\x0c\n\x04\x62msg\x18\x01 \x01(\t\"`\n\x0fSystemStdErrMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\'\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x19.proto_types.SystemStdErr\",\n\x16SystemReportReturnCode\x12\x12\n\nreturncode\x18\x01 \x01(\x05\"t\n\x19SystemReportReturnCodeMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x31\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32#.proto_types.SystemReportReturnCode\"p\n\x13TimingInfoCollected\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12/\n\x0btiming_info\x18\x02 \x01(\x0b\x32\x1a.proto_types.TimingInfoMsg\"n\n\x16TimingInfoCollectedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32 .proto_types.TimingInfoCollected\"&\n\x12LogDebugStackTrace\x12\x10\n\x08\x65xc_info\x18\x01 \x01(\t\"l\n\x15LogDebugStackTraceMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.LogDebugStackTrace\"\x1e\n\x0e\x43heckCleanPath\x12\x0c\n\x04path\x18\x01 \x01(\t\"d\n\x11\x43heckCleanPathMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.CheckCleanPath\" \n\x10\x43onfirmCleanPath\x12\x0c\n\x04path\x18\x01 \x01(\t\"h\n\x13\x43onfirmCleanPathMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.proto_types.ConfirmCleanPath\"\"\n\x12ProtectedCleanPath\x12\x0c\n\x04path\x18\x01 \x01(\t\"l\n\x15ProtectedCleanPathMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.ProtectedCleanPath\"\x14\n\x12\x46inishedCleanPaths\"l\n\x15\x46inishedCleanPathsMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.FinishedCleanPaths\"5\n\x0bOpenCommand\x12\x10\n\x08open_cmd\x18\x01 \x01(\t\x12\x14\n\x0cprofiles_dir\x18\x02 \x01(\t\"^\n\x0eOpenCommandMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12&\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x18.proto_types.OpenCommand\"\x19\n\nFormatting\x12\x0b\n\x03msg\x18\x01 \x01(\t\"\\\n\rFormattingMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12%\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x17.proto_types.Formatting\"0\n\x0fServingDocsPort\x12\x0f\n\x07\x61\x64\x64ress\x18\x01 \x01(\t\x12\x0c\n\x04port\x18\x02 \x01(\x05\"f\n\x12ServingDocsPortMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.ServingDocsPort\"%\n\x15ServingDocsAccessInfo\x12\x0c\n\x04port\x18\x01 \x01(\t\"r\n\x18ServingDocsAccessInfoMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x30\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\".proto_types.ServingDocsAccessInfo\"\x15\n\x13ServingDocsExitInfo\"n\n\x16ServingDocsExitInfoMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32 .proto_types.ServingDocsExitInfo\"J\n\x10RunResultWarning\x12\x15\n\rresource_type\x18\x01 \x01(\t\x12\x11\n\tnode_name\x18\x02 \x01(\t\x12\x0c\n\x04path\x18\x03 \x01(\t\"h\n\x13RunResultWarningMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.proto_types.RunResultWarning\"J\n\x10RunResultFailure\x12\x15\n\rresource_type\x18\x01 \x01(\t\x12\x11\n\tnode_name\x18\x02 \x01(\t\x12\x0c\n\x04path\x18\x03 \x01(\t\"h\n\x13RunResultFailureMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.proto_types.RunResultFailure\"k\n\tStatsLine\x12\x30\n\x05stats\x18\x01 \x03(\x0b\x32!.proto_types.StatsLine.StatsEntry\x1a,\n\nStatsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x05:\x02\x38\x01\"Z\n\x0cStatsLineMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12$\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x16.proto_types.StatsLine\"\x1d\n\x0eRunResultError\x12\x0b\n\x03msg\x18\x01 \x01(\t\"d\n\x11RunResultErrorMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.RunResultError\")\n\x17RunResultErrorNoMessage\x12\x0e\n\x06status\x18\x01 \x01(\t\"v\n\x1aRunResultErrorNoMessageMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x32\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32$.proto_types.RunResultErrorNoMessage\"\x1f\n\x0fSQLCompiledPath\x12\x0c\n\x04path\x18\x01 \x01(\t\"f\n\x12SQLCompiledPathMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.SQLCompiledPath\"-\n\x14\x43heckNodeTestFailure\x12\x15\n\rrelation_name\x18\x01 \x01(\t\"p\n\x17\x43heckNodeTestFailureMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.CheckNodeTestFailure\"\"\n\x13\x46irstRunResultError\x12\x0b\n\x03msg\x18\x01 \x01(\t\"n\n\x16\x46irstRunResultErrorMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32 .proto_types.FirstRunResultError\"\'\n\x18\x41\x66terFirstRunResultError\x12\x0b\n\x03msg\x18\x01 \x01(\t\"x\n\x1b\x41\x66terFirstRunResultErrorMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x33\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32%.proto_types.AfterFirstRunResultError\"W\n\x0f\x45ndOfRunSummary\x12\x12\n\nnum_errors\x18\x01 \x01(\x05\x12\x14\n\x0cnum_warnings\x18\x02 \x01(\x05\x12\x1a\n\x12keyboard_interrupt\x18\x03 \x01(\x08\"f\n\x12\x45ndOfRunSummaryMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.EndOfRunSummary\"U\n\x13LogSkipBecauseError\x12\x0e\n\x06schema\x18\x01 \x01(\t\x12\x10\n\x08relation\x18\x02 \x01(\t\x12\r\n\x05index\x18\x03 \x01(\x05\x12\r\n\x05total\x18\x04 \x01(\x05\"n\n\x16LogSkipBecauseErrorMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32 .proto_types.LogSkipBecauseError\"\x14\n\x12\x45nsureGitInstalled\"l\n\x15\x45nsureGitInstalledMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.EnsureGitInstalled\"\x1a\n\x18\x44\x65psCreatingLocalSymlink\"x\n\x1b\x44\x65psCreatingLocalSymlinkMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x33\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32%.proto_types.DepsCreatingLocalSymlink\"\x19\n\x17\x44\x65psSymlinkNotAvailable\"v\n\x1a\x44\x65psSymlinkNotAvailableMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x32\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32$.proto_types.DepsSymlinkNotAvailable\"\x11\n\x0f\x44isableTracking\"f\n\x12\x44isableTrackingMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.DisableTracking\"\x1e\n\x0cSendingEvent\x12\x0e\n\x06kwargs\x18\x01 \x01(\t\"`\n\x0fSendingEventMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\'\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x19.proto_types.SendingEvent\"\x12\n\x10SendEventFailure\"h\n\x13SendEventFailureMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.proto_types.SendEventFailure\"\r\n\x0b\x46lushEvents\"^\n\x0e\x46lushEventsMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12&\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x18.proto_types.FlushEvents\"\x14\n\x12\x46lushEventsFailure\"l\n\x15\x46lushEventsFailureMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.FlushEventsFailure\"-\n\x19TrackingInitializeFailure\x12\x10\n\x08\x65xc_info\x18\x01 \x01(\t\"z\n\x1cTrackingInitializeFailureMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x34\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32&.proto_types.TrackingInitializeFailure\"&\n\x17RunResultWarningMessage\x12\x0b\n\x03msg\x18\x01 \x01(\t\"v\n\x1aRunResultWarningMessageMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x32\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32$.proto_types.RunResultWarningMessage\"\x1a\n\x0b\x44\x65\x62ugCmdOut\x12\x0b\n\x03msg\x18\x01 \x01(\t\"^\n\x0e\x44\x65\x62ugCmdOutMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12&\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x18.proto_types.DebugCmdOut\"\x1d\n\x0e\x44\x65\x62ugCmdResult\x12\x0b\n\x03msg\x18\x01 \x01(\t\"d\n\x11\x44\x65\x62ugCmdResultMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.DebugCmdResult\"\x19\n\nListCmdOut\x12\x0b\n\x03msg\x18\x01 \x01(\t\"\\\n\rListCmdOutMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12%\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x17.proto_types.ListCmdOut\"\x13\n\x04Note\x12\x0b\n\x03msg\x18\x01 \x01(\t\"P\n\x07NoteMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x1f\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x11.proto_types.Noteb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0btypes.proto\x12\x0bproto_types\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1cgoogle/protobuf/struct.proto\"\x91\x02\n\tEventInfo\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04\x63ode\x18\x02 \x01(\t\x12\x0b\n\x03msg\x18\x03 \x01(\t\x12\r\n\x05level\x18\x04 \x01(\t\x12\x15\n\rinvocation_id\x18\x05 \x01(\t\x12\x0b\n\x03pid\x18\x06 \x01(\x05\x12\x0e\n\x06thread\x18\x07 \x01(\t\x12&\n\x02ts\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x30\n\x05\x65xtra\x18\t \x03(\x0b\x32!.proto_types.EventInfo.ExtraEntry\x12\x10\n\x08\x63\x61tegory\x18\n \x01(\t\x1a,\n\nExtraEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\x7f\n\rTimingInfoMsg\x12\x0c\n\x04name\x18\x01 \x01(\t\x12.\n\nstarted_at\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x30\n\x0c\x63ompleted_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"V\n\x0cNodeRelation\x12\x10\n\x08\x64\x61tabase\x18\n \x01(\t\x12\x0e\n\x06schema\x18\x0b \x01(\t\x12\r\n\x05\x61lias\x18\x0c \x01(\t\x12\x15\n\rrelation_name\x18\r \x01(\t\"\x91\x02\n\x08NodeInfo\x12\x11\n\tnode_path\x18\x01 \x01(\t\x12\x11\n\tnode_name\x18\x02 \x01(\t\x12\x11\n\tunique_id\x18\x03 \x01(\t\x12\x15\n\rresource_type\x18\x04 \x01(\t\x12\x14\n\x0cmaterialized\x18\x05 \x01(\t\x12\x13\n\x0bnode_status\x18\x06 \x01(\t\x12\x17\n\x0fnode_started_at\x18\x07 \x01(\t\x12\x18\n\x10node_finished_at\x18\x08 \x01(\t\x12%\n\x04meta\x18\t \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x30\n\rnode_relation\x18\n \x01(\x0b\x32\x19.proto_types.NodeRelation\"\xd1\x01\n\x0cRunResultMsg\x12\x0e\n\x06status\x18\x01 \x01(\t\x12\x0f\n\x07message\x18\x02 \x01(\t\x12/\n\x0btiming_info\x18\x03 \x03(\x0b\x32\x1a.proto_types.TimingInfoMsg\x12\x0e\n\x06thread\x18\x04 \x01(\t\x12\x16\n\x0e\x65xecution_time\x18\x05 \x01(\x02\x12\x31\n\x10\x61\x64\x61pter_response\x18\x06 \x01(\x0b\x32\x17.google.protobuf.Struct\x12\x14\n\x0cnum_failures\x18\x07 \x01(\x05\"G\n\x0fReferenceKeyMsg\x12\x10\n\x08\x64\x61tabase\x18\x01 \x01(\t\x12\x0e\n\x06schema\x18\x02 \x01(\t\x12\x12\n\nidentifier\x18\x03 \x01(\t\"6\n\x0eGenericMessage\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\"9\n\x11MainReportVersion\x12\x0f\n\x07version\x18\x01 \x01(\t\x12\x13\n\x0blog_version\x18\x02 \x01(\x05\"j\n\x14MainReportVersionMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12,\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1e.proto_types.MainReportVersion\"r\n\x0eMainReportArgs\x12\x33\n\x04\x61rgs\x18\x01 \x03(\x0b\x32%.proto_types.MainReportArgs.ArgsEntry\x1a+\n\tArgsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"d\n\x11MainReportArgsMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.MainReportArgs\"+\n\x15MainTrackingUserState\x12\x12\n\nuser_state\x18\x01 \x01(\t\"r\n\x18MainTrackingUserStateMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x30\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\".proto_types.MainTrackingUserState\"5\n\x0fMergedFromState\x12\x12\n\nnum_merged\x18\x01 \x01(\x05\x12\x0e\n\x06sample\x18\x02 \x03(\t\"f\n\x12MergedFromStateMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.MergedFromState\"A\n\x14MissingProfileTarget\x12\x14\n\x0cprofile_name\x18\x01 \x01(\t\x12\x13\n\x0btarget_name\x18\x02 \x01(\t\"p\n\x17MissingProfileTargetMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.MissingProfileTarget\"(\n\x11InvalidOptionYAML\x12\x13\n\x0boption_name\x18\x01 \x01(\t\"j\n\x14InvalidOptionYAMLMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12,\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1e.proto_types.InvalidOptionYAML\"!\n\x12LogDbtProjectError\x12\x0b\n\x03\x65xc\x18\x01 \x01(\t\"l\n\x15LogDbtProjectErrorMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.LogDbtProjectError\"3\n\x12LogDbtProfileError\x12\x0b\n\x03\x65xc\x18\x01 \x01(\t\x12\x10\n\x08profiles\x18\x02 \x03(\t\"l\n\x15LogDbtProfileErrorMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.LogDbtProfileError\"!\n\x12StarterProjectPath\x12\x0b\n\x03\x64ir\x18\x01 \x01(\t\"l\n\x15StarterProjectPathMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.StarterProjectPath\"$\n\x15\x43onfigFolderDirectory\x12\x0b\n\x03\x64ir\x18\x01 \x01(\t\"r\n\x18\x43onfigFolderDirectoryMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x30\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\".proto_types.ConfigFolderDirectory\"\'\n\x14NoSampleProfileFound\x12\x0f\n\x07\x61\x64\x61pter\x18\x01 \x01(\t\"p\n\x17NoSampleProfileFoundMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.NoSampleProfileFound\"6\n\x18ProfileWrittenWithSample\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\"x\n\x1bProfileWrittenWithSampleMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x33\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32%.proto_types.ProfileWrittenWithSample\"B\n$ProfileWrittenWithTargetTemplateYAML\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\"\x90\x01\n\'ProfileWrittenWithTargetTemplateYAMLMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12?\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x31.proto_types.ProfileWrittenWithTargetTemplateYAML\"C\n%ProfileWrittenWithProjectTemplateYAML\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\x02 \x01(\t\"\x92\x01\n(ProfileWrittenWithProjectTemplateYAMLMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12@\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x32.proto_types.ProfileWrittenWithProjectTemplateYAML\"\x12\n\x10SettingUpProfile\"h\n\x13SettingUpProfileMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.proto_types.SettingUpProfile\"\x1c\n\x1aInvalidProfileTemplateYAML\"|\n\x1dInvalidProfileTemplateYAMLMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x35\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\'.proto_types.InvalidProfileTemplateYAML\"(\n\x18ProjectNameAlreadyExists\x12\x0c\n\x04name\x18\x01 \x01(\t\"x\n\x1bProjectNameAlreadyExistsMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x33\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32%.proto_types.ProjectNameAlreadyExists\"K\n\x0eProjectCreated\x12\x14\n\x0cproject_name\x18\x01 \x01(\t\x12\x10\n\x08\x64ocs_url\x18\x02 \x01(\t\x12\x11\n\tslack_url\x18\x03 \x01(\t\"d\n\x11ProjectCreatedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.ProjectCreated\"@\n\x1aPackageRedirectDeprecation\x12\x10\n\x08old_name\x18\x01 \x01(\t\x12\x10\n\x08new_name\x18\x02 \x01(\t\"|\n\x1dPackageRedirectDeprecationMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x35\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\'.proto_types.PackageRedirectDeprecation\"\x1f\n\x1dPackageInstallPathDeprecation\"\x82\x01\n PackageInstallPathDeprecationMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x38\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32*.proto_types.PackageInstallPathDeprecation\"H\n\x1b\x43onfigSourcePathDeprecation\x12\x17\n\x0f\x64\x65precated_path\x18\x01 \x01(\t\x12\x10\n\x08\x65xp_path\x18\x02 \x01(\t\"~\n\x1e\x43onfigSourcePathDeprecationMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x36\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32(.proto_types.ConfigSourcePathDeprecation\"F\n\x19\x43onfigDataPathDeprecation\x12\x17\n\x0f\x64\x65precated_path\x18\x01 \x01(\t\x12\x10\n\x08\x65xp_path\x18\x02 \x01(\t\"z\n\x1c\x43onfigDataPathDeprecationMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x34\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32&.proto_types.ConfigDataPathDeprecation\"?\n\x19\x41\x64\x61pterDeprecationWarning\x12\x10\n\x08old_name\x18\x01 \x01(\t\x12\x10\n\x08new_name\x18\x02 \x01(\t\"z\n\x1c\x41\x64\x61pterDeprecationWarningMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x34\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32&.proto_types.AdapterDeprecationWarning\".\n\x17MetricAttributesRenamed\x12\x13\n\x0bmetric_name\x18\x01 \x01(\t\"v\n\x1aMetricAttributesRenamedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x32\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32$.proto_types.MetricAttributesRenamed\"+\n\x17\x45xposureNameDeprecation\x12\x10\n\x08\x65xposure\x18\x01 \x01(\t\"v\n\x1a\x45xposureNameDeprecationMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x32\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32$.proto_types.ExposureNameDeprecation\"^\n\x13InternalDeprecation\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0e\n\x06reason\x18\x02 \x01(\t\x12\x18\n\x10suggested_action\x18\x03 \x01(\t\x12\x0f\n\x07version\x18\x04 \x01(\t\"n\n\x16InternalDeprecationMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32 .proto_types.InternalDeprecation\"@\n\x1a\x45nvironmentVariableRenamed\x12\x10\n\x08old_name\x18\x01 \x01(\t\x12\x10\n\x08new_name\x18\x02 \x01(\t\"|\n\x1d\x45nvironmentVariableRenamedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x35\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\'.proto_types.EnvironmentVariableRenamed\"3\n\x18\x43onfigLogPathDeprecation\x12\x17\n\x0f\x64\x65precated_path\x18\x01 \x01(\t\"x\n\x1b\x43onfigLogPathDeprecationMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x33\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32%.proto_types.ConfigLogPathDeprecation\"6\n\x1b\x43onfigTargetPathDeprecation\x12\x17\n\x0f\x64\x65precated_path\x18\x01 \x01(\t\"~\n\x1e\x43onfigTargetPathDeprecationMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x36\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32(.proto_types.ConfigTargetPathDeprecation\"!\n\x1f\x43ollectFreshnessReturnSignature\"\x86\x01\n\"CollectFreshnessReturnSignatureMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12:\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32,.proto_types.CollectFreshnessReturnSignature\"\x87\x01\n\x11\x41\x64\x61pterEventDebug\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x10\n\x08\x62\x61se_msg\x18\x03 \x01(\t\x12(\n\x04\x61rgs\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.ListValue\"j\n\x14\x41\x64\x61pterEventDebugMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12,\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1e.proto_types.AdapterEventDebug\"\x86\x01\n\x10\x41\x64\x61pterEventInfo\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x10\n\x08\x62\x61se_msg\x18\x03 \x01(\t\x12(\n\x04\x61rgs\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.ListValue\"h\n\x13\x41\x64\x61pterEventInfoMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.proto_types.AdapterEventInfo\"\x89\x01\n\x13\x41\x64\x61pterEventWarning\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x10\n\x08\x62\x61se_msg\x18\x03 \x01(\t\x12(\n\x04\x61rgs\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.ListValue\"n\n\x16\x41\x64\x61pterEventWarningMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32 .proto_types.AdapterEventWarning\"\x99\x01\n\x11\x41\x64\x61pterEventError\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x10\n\x08\x62\x61se_msg\x18\x03 \x01(\t\x12(\n\x04\x61rgs\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.ListValue\x12\x10\n\x08\x65xc_info\x18\x05 \x01(\t\"j\n\x14\x41\x64\x61pterEventErrorMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12,\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1e.proto_types.AdapterEventError\"_\n\rNewConnection\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x11\n\tconn_type\x18\x02 \x01(\t\x12\x11\n\tconn_name\x18\x03 \x01(\t\"b\n\x10NewConnectionMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12(\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1a.proto_types.NewConnection\"=\n\x10\x43onnectionReused\x12\x11\n\tconn_name\x18\x01 \x01(\t\x12\x16\n\x0eorig_conn_name\x18\x02 \x01(\t\"h\n\x13\x43onnectionReusedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.proto_types.ConnectionReused\"0\n\x1b\x43onnectionLeftOpenInCleanup\x12\x11\n\tconn_name\x18\x01 \x01(\t\"~\n\x1e\x43onnectionLeftOpenInCleanupMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x36\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32(.proto_types.ConnectionLeftOpenInCleanup\".\n\x19\x43onnectionClosedInCleanup\x12\x11\n\tconn_name\x18\x01 \x01(\t\"z\n\x1c\x43onnectionClosedInCleanupMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x34\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32&.proto_types.ConnectionClosedInCleanup\"_\n\x0eRollbackFailed\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x11\n\tconn_name\x18\x02 \x01(\t\x12\x10\n\x08\x65xc_info\x18\x03 \x01(\t\"d\n\x11RollbackFailedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.RollbackFailed\"O\n\x10\x43onnectionClosed\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x11\n\tconn_name\x18\x02 \x01(\t\"h\n\x13\x43onnectionClosedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.proto_types.ConnectionClosed\"Q\n\x12\x43onnectionLeftOpen\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x11\n\tconn_name\x18\x02 \x01(\t\"l\n\x15\x43onnectionLeftOpenMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.ConnectionLeftOpen\"G\n\x08Rollback\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x11\n\tconn_name\x18\x02 \x01(\t\"X\n\x0bRollbackMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12#\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x15.proto_types.Rollback\"@\n\tCacheMiss\x12\x11\n\tconn_name\x18\x01 \x01(\t\x12\x10\n\x08\x64\x61tabase\x18\x02 \x01(\t\x12\x0e\n\x06schema\x18\x03 \x01(\t\"Z\n\x0c\x43\x61\x63heMissMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12$\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x16.proto_types.CacheMiss\"b\n\rListRelations\x12\x10\n\x08\x64\x61tabase\x18\x01 \x01(\t\x12\x0e\n\x06schema\x18\x02 \x01(\t\x12/\n\trelations\x18\x03 \x03(\x0b\x32\x1c.proto_types.ReferenceKeyMsg\"b\n\x10ListRelationsMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12(\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1a.proto_types.ListRelations\"`\n\x0e\x43onnectionUsed\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x11\n\tconn_type\x18\x02 \x01(\t\x12\x11\n\tconn_name\x18\x03 \x01(\t\"d\n\x11\x43onnectionUsedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.ConnectionUsed\"T\n\x08SQLQuery\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x11\n\tconn_name\x18\x02 \x01(\t\x12\x0b\n\x03sql\x18\x03 \x01(\t\"X\n\x0bSQLQueryMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12#\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x15.proto_types.SQLQuery\"[\n\x0eSQLQueryStatus\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x0e\n\x06status\x18\x02 \x01(\t\x12\x0f\n\x07\x65lapsed\x18\x03 \x01(\x02\"d\n\x11SQLQueryStatusMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.SQLQueryStatus\"H\n\tSQLCommit\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x11\n\tconn_name\x18\x02 \x01(\t\"Z\n\x0cSQLCommitMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12$\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x16.proto_types.SQLCommit\"a\n\rColTypeChange\x12\x11\n\torig_type\x18\x01 \x01(\t\x12\x10\n\x08new_type\x18\x02 \x01(\t\x12+\n\x05table\x18\x03 \x01(\x0b\x32\x1c.proto_types.ReferenceKeyMsg\"b\n\x10\x43olTypeChangeMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12(\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1a.proto_types.ColTypeChange\"@\n\x0eSchemaCreation\x12.\n\x08relation\x18\x01 \x01(\x0b\x32\x1c.proto_types.ReferenceKeyMsg\"d\n\x11SchemaCreationMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.SchemaCreation\"<\n\nSchemaDrop\x12.\n\x08relation\x18\x01 \x01(\x0b\x32\x1c.proto_types.ReferenceKeyMsg\"\\\n\rSchemaDropMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12%\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x17.proto_types.SchemaDrop\"\xde\x01\n\x0b\x43\x61\x63heAction\x12\x0e\n\x06\x61\x63tion\x18\x01 \x01(\t\x12-\n\x07ref_key\x18\x02 \x01(\x0b\x32\x1c.proto_types.ReferenceKeyMsg\x12/\n\tref_key_2\x18\x03 \x01(\x0b\x32\x1c.proto_types.ReferenceKeyMsg\x12/\n\tref_key_3\x18\x04 \x01(\x0b\x32\x1c.proto_types.ReferenceKeyMsg\x12.\n\x08ref_list\x18\x05 \x03(\x0b\x32\x1c.proto_types.ReferenceKeyMsg\"^\n\x0e\x43\x61\x63heActionMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12&\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x18.proto_types.CacheAction\"\x98\x01\n\x0e\x43\x61\x63heDumpGraph\x12\x33\n\x04\x64ump\x18\x01 \x03(\x0b\x32%.proto_types.CacheDumpGraph.DumpEntry\x12\x14\n\x0c\x62\x65\x66ore_after\x18\x02 \x01(\t\x12\x0e\n\x06\x61\x63tion\x18\x03 \x01(\t\x1a+\n\tDumpEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"d\n\x11\x43\x61\x63heDumpGraphMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.CacheDumpGraph\"!\n\x12\x41\x64\x61pterImportError\x12\x0b\n\x03\x65xc\x18\x01 \x01(\t\"l\n\x15\x41\x64\x61pterImportErrorMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.AdapterImportError\"#\n\x0fPluginLoadError\x12\x10\n\x08\x65xc_info\x18\x01 \x01(\t\"f\n\x12PluginLoadErrorMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.PluginLoadError\"Z\n\x14NewConnectionOpening\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x18\n\x10\x63onnection_state\x18\x02 \x01(\t\"p\n\x17NewConnectionOpeningMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.NewConnectionOpening\"8\n\rCodeExecution\x12\x11\n\tconn_name\x18\x01 \x01(\t\x12\x14\n\x0c\x63ode_content\x18\x02 \x01(\t\"b\n\x10\x43odeExecutionMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12(\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1a.proto_types.CodeExecution\"6\n\x13\x43odeExecutionStatus\x12\x0e\n\x06status\x18\x01 \x01(\t\x12\x0f\n\x07\x65lapsed\x18\x02 \x01(\x02\"n\n\x16\x43odeExecutionStatusMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32 .proto_types.CodeExecutionStatus\"%\n\x16\x43\x61talogGenerationError\x12\x0b\n\x03\x65xc\x18\x01 \x01(\t\"t\n\x19\x43\x61talogGenerationErrorMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x31\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32#.proto_types.CatalogGenerationError\"-\n\x13WriteCatalogFailure\x12\x16\n\x0enum_exceptions\x18\x01 \x01(\x05\"n\n\x16WriteCatalogFailureMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32 .proto_types.WriteCatalogFailure\"\x1e\n\x0e\x43\x61talogWritten\x12\x0c\n\x04path\x18\x01 \x01(\t\"d\n\x11\x43\x61talogWrittenMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.CatalogWritten\"\x14\n\x12\x43\x61nnotGenerateDocs\"l\n\x15\x43\x61nnotGenerateDocsMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.CannotGenerateDocs\"\x11\n\x0f\x42uildingCatalog\"f\n\x12\x42uildingCatalogMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.BuildingCatalog\"-\n\x18\x44\x61tabaseErrorRunningHook\x12\x11\n\thook_type\x18\x01 \x01(\t\"x\n\x1b\x44\x61tabaseErrorRunningHookMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x33\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32%.proto_types.DatabaseErrorRunningHook\"4\n\x0cHooksRunning\x12\x11\n\tnum_hooks\x18\x01 \x01(\x05\x12\x11\n\thook_type\x18\x02 \x01(\t\"`\n\x0fHooksRunningMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\'\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x19.proto_types.HooksRunning\"T\n\x14\x46inishedRunningStats\x12\x11\n\tstat_line\x18\x01 \x01(\t\x12\x11\n\texecution\x18\x02 \x01(\t\x12\x16\n\x0e\x65xecution_time\x18\x03 \x01(\x02\"p\n\x17\x46inishedRunningStatsMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.FinishedRunningStats\"<\n\x15\x43onstraintNotEnforced\x12\x12\n\nconstraint\x18\x01 \x01(\t\x12\x0f\n\x07\x61\x64\x61pter\x18\x02 \x01(\t\"r\n\x18\x43onstraintNotEnforcedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x30\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\".proto_types.ConstraintNotEnforced\"=\n\x16\x43onstraintNotSupported\x12\x12\n\nconstraint\x18\x01 \x01(\t\x12\x0f\n\x07\x61\x64\x61pter\x18\x02 \x01(\t\"t\n\x19\x43onstraintNotSupportedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x31\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32#.proto_types.ConstraintNotSupported\"7\n\x12InputFileDiffError\x12\x10\n\x08\x63\x61tegory\x18\x01 \x01(\t\x12\x0f\n\x07\x66ile_id\x18\x02 \x01(\t\"l\n\x15InputFileDiffErrorMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.InputFileDiffError\"?\n\x14InvalidValueForField\x12\x12\n\nfield_name\x18\x01 \x01(\t\x12\x13\n\x0b\x66ield_value\x18\x02 \x01(\t\"p\n\x17InvalidValueForFieldMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.InvalidValueForField\"Q\n\x11ValidationWarning\x12\x15\n\rresource_type\x18\x01 \x01(\t\x12\x12\n\nfield_name\x18\x02 \x01(\t\x12\x11\n\tnode_name\x18\x03 \x01(\t\"j\n\x14ValidationWarningMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12,\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1e.proto_types.ValidationWarning\"!\n\x11ParsePerfInfoPath\x12\x0c\n\x04path\x18\x01 \x01(\t\"j\n\x14ParsePerfInfoPathMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12,\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1e.proto_types.ParsePerfInfoPath\"$\n\x14GenericTestFileParse\x12\x0c\n\x04path\x18\x01 \x01(\t\"p\n\x17GenericTestFileParseMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.GenericTestFileParse\"\x1e\n\x0eMacroFileParse\x12\x0c\n\x04path\x18\x01 \x01(\t\"d\n\x11MacroFileParseMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.MacroFileParse\"1\n!PartialParsingErrorProcessingFile\x12\x0c\n\x04\x66ile\x18\x01 \x01(\t\"\x8a\x01\n$PartialParsingErrorProcessingFileMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12<\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32..proto_types.PartialParsingErrorProcessingFile\"\x86\x01\n\x13PartialParsingError\x12?\n\x08\x65xc_info\x18\x01 \x03(\x0b\x32-.proto_types.PartialParsingError.ExcInfoEntry\x1a.\n\x0c\x45xcInfoEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"n\n\x16PartialParsingErrorMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32 .proto_types.PartialParsingError\"\x1b\n\x19PartialParsingSkipParsing\"z\n\x1cPartialParsingSkipParsingMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x34\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32&.proto_types.PartialParsingSkipParsing\"&\n\x14UnableToPartialParse\x12\x0e\n\x06reason\x18\x01 \x01(\t\"p\n\x17UnableToPartialParseMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.UnableToPartialParse\"f\n\x12StateCheckVarsHash\x12\x10\n\x08\x63hecksum\x18\x01 \x01(\t\x12\x0c\n\x04vars\x18\x02 \x01(\t\x12\x0f\n\x07profile\x18\x03 \x01(\t\x12\x0e\n\x06target\x18\x04 \x01(\t\x12\x0f\n\x07version\x18\x05 \x01(\t\"l\n\x15StateCheckVarsHashMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.StateCheckVarsHash\"\x1a\n\x18PartialParsingNotEnabled\"x\n\x1bPartialParsingNotEnabledMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x33\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32%.proto_types.PartialParsingNotEnabled\"C\n\x14ParsedFileLoadFailed\x12\x0c\n\x04path\x18\x01 \x01(\t\x12\x0b\n\x03\x65xc\x18\x02 \x01(\t\x12\x10\n\x08\x65xc_info\x18\x03 \x01(\t\"p\n\x17ParsedFileLoadFailedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.ParsedFileLoadFailed\"H\n\x15PartialParsingEnabled\x12\x0f\n\x07\x64\x65leted\x18\x01 \x01(\x05\x12\r\n\x05\x61\x64\x64\x65\x64\x18\x02 \x01(\x05\x12\x0f\n\x07\x63hanged\x18\x03 \x01(\x05\"r\n\x18PartialParsingEnabledMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x30\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\".proto_types.PartialParsingEnabled\"8\n\x12PartialParsingFile\x12\x0f\n\x07\x66ile_id\x18\x01 \x01(\t\x12\x11\n\toperation\x18\x02 \x01(\t\"l\n\x15PartialParsingFileMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.PartialParsingFile\"\xaf\x01\n\x1fInvalidDisabledTargetInTestNode\x12\x1b\n\x13resource_type_title\x18\x01 \x01(\t\x12\x11\n\tunique_id\x18\x02 \x01(\t\x12\x1a\n\x12original_file_path\x18\x03 \x01(\t\x12\x13\n\x0btarget_kind\x18\x04 \x01(\t\x12\x13\n\x0btarget_name\x18\x05 \x01(\t\x12\x16\n\x0etarget_package\x18\x06 \x01(\t\"\x86\x01\n\"InvalidDisabledTargetInTestNodeMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12:\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32,.proto_types.InvalidDisabledTargetInTestNode\"7\n\x18UnusedResourceConfigPath\x12\x1b\n\x13unused_config_paths\x18\x01 \x03(\t\"x\n\x1bUnusedResourceConfigPathMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x33\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32%.proto_types.UnusedResourceConfigPath\"3\n\rSeedIncreased\x12\x14\n\x0cpackage_name\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\"b\n\x10SeedIncreasedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12(\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1a.proto_types.SeedIncreased\">\n\x18SeedExceedsLimitSamePath\x12\x14\n\x0cpackage_name\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\"x\n\x1bSeedExceedsLimitSamePathMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x33\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32%.proto_types.SeedExceedsLimitSamePath\"D\n\x1eSeedExceedsLimitAndPathChanged\x12\x14\n\x0cpackage_name\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\"\x84\x01\n!SeedExceedsLimitAndPathChangedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x39\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32+.proto_types.SeedExceedsLimitAndPathChanged\"\\\n\x1fSeedExceedsLimitChecksumChanged\x12\x14\n\x0cpackage_name\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x15\n\rchecksum_name\x18\x03 \x01(\t\"\x86\x01\n\"SeedExceedsLimitChecksumChangedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12:\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32,.proto_types.SeedExceedsLimitChecksumChanged\"%\n\x0cUnusedTables\x12\x15\n\runused_tables\x18\x01 \x03(\t\"`\n\x0fUnusedTablesMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\'\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x19.proto_types.UnusedTables\"\x87\x01\n\x17WrongResourceSchemaFile\x12\x12\n\npatch_name\x18\x01 \x01(\t\x12\x15\n\rresource_type\x18\x02 \x01(\t\x12\x1c\n\x14plural_resource_type\x18\x03 \x01(\t\x12\x10\n\x08yaml_key\x18\x04 \x01(\t\x12\x11\n\tfile_path\x18\x05 \x01(\t\"v\n\x1aWrongResourceSchemaFileMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x32\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32$.proto_types.WrongResourceSchemaFile\"K\n\x10NoNodeForYamlKey\x12\x12\n\npatch_name\x18\x01 \x01(\t\x12\x10\n\x08yaml_key\x18\x02 \x01(\t\x12\x11\n\tfile_path\x18\x03 \x01(\t\"h\n\x13NoNodeForYamlKeyMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.proto_types.NoNodeForYamlKey\"+\n\x15MacroNotFoundForPatch\x12\x12\n\npatch_name\x18\x01 \x01(\t\"r\n\x18MacroNotFoundForPatchMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x30\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\".proto_types.MacroNotFoundForPatch\"\xb8\x01\n\x16NodeNotFoundOrDisabled\x12\x1a\n\x12original_file_path\x18\x01 \x01(\t\x12\x11\n\tunique_id\x18\x02 \x01(\t\x12\x1b\n\x13resource_type_title\x18\x03 \x01(\t\x12\x13\n\x0btarget_name\x18\x04 \x01(\t\x12\x13\n\x0btarget_kind\x18\x05 \x01(\t\x12\x16\n\x0etarget_package\x18\x06 \x01(\t\x12\x10\n\x08\x64isabled\x18\x07 \x01(\t\"t\n\x19NodeNotFoundOrDisabledMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x31\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32#.proto_types.NodeNotFoundOrDisabled\"H\n\x0fJinjaLogWarning\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x0b\n\x03msg\x18\x02 \x01(\t\"f\n\x12JinjaLogWarningMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.JinjaLogWarning\"E\n\x0cJinjaLogInfo\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x0b\n\x03msg\x18\x02 \x01(\t\"`\n\x0fJinjaLogInfoMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\'\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x19.proto_types.JinjaLogInfo\"F\n\rJinjaLogDebug\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x0b\n\x03msg\x18\x02 \x01(\t\"b\n\x10JinjaLogDebugMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12(\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1a.proto_types.JinjaLogDebug\"\xae\x01\n\x1eUnpinnedRefNewVersionAvailable\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x15\n\rref_node_name\x18\x02 \x01(\t\x12\x18\n\x10ref_node_package\x18\x03 \x01(\t\x12\x18\n\x10ref_node_version\x18\x04 \x01(\t\x12\x17\n\x0fref_max_version\x18\x05 \x01(\t\"\x84\x01\n!UnpinnedRefNewVersionAvailableMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x39\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32+.proto_types.UnpinnedRefNewVersionAvailable\"/\n\x1dGitSparseCheckoutSubdirectory\x12\x0e\n\x06subdir\x18\x01 \x01(\t\"\x82\x01\n GitSparseCheckoutSubdirectoryMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x38\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32*.proto_types.GitSparseCheckoutSubdirectory\"/\n\x1bGitProgressCheckoutRevision\x12\x10\n\x08revision\x18\x01 \x01(\t\"~\n\x1eGitProgressCheckoutRevisionMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x36\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32(.proto_types.GitProgressCheckoutRevision\"4\n%GitProgressUpdatingExistingDependency\x12\x0b\n\x03\x64ir\x18\x01 \x01(\t\"\x92\x01\n(GitProgressUpdatingExistingDependencyMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12@\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x32.proto_types.GitProgressUpdatingExistingDependency\".\n\x1fGitProgressPullingNewDependency\x12\x0b\n\x03\x64ir\x18\x01 \x01(\t\"\x86\x01\n\"GitProgressPullingNewDependencyMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12:\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32,.proto_types.GitProgressPullingNewDependency\"\x1d\n\x0eGitNothingToDo\x12\x0b\n\x03sha\x18\x01 \x01(\t\"d\n\x11GitNothingToDoMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.GitNothingToDo\"E\n\x1fGitProgressUpdatedCheckoutRange\x12\x11\n\tstart_sha\x18\x01 \x01(\t\x12\x0f\n\x07\x65nd_sha\x18\x02 \x01(\t\"\x86\x01\n\"GitProgressUpdatedCheckoutRangeMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12:\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32,.proto_types.GitProgressUpdatedCheckoutRange\"*\n\x17GitProgressCheckedOutAt\x12\x0f\n\x07\x65nd_sha\x18\x01 \x01(\t\"v\n\x1aGitProgressCheckedOutAtMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x32\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32$.proto_types.GitProgressCheckedOutAt\")\n\x1aRegistryProgressGETRequest\x12\x0b\n\x03url\x18\x01 \x01(\t\"|\n\x1dRegistryProgressGETRequestMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x35\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\'.proto_types.RegistryProgressGETRequest\"=\n\x1bRegistryProgressGETResponse\x12\x0b\n\x03url\x18\x01 \x01(\t\x12\x11\n\tresp_code\x18\x02 \x01(\x05\"~\n\x1eRegistryProgressGETResponseMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x36\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32(.proto_types.RegistryProgressGETResponse\"_\n\x1dSelectorReportInvalidSelector\x12\x17\n\x0fvalid_selectors\x18\x01 \x01(\t\x12\x13\n\x0bspec_method\x18\x02 \x01(\t\x12\x10\n\x08raw_spec\x18\x03 \x01(\t\"\x82\x01\n SelectorReportInvalidSelectorMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x38\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32*.proto_types.SelectorReportInvalidSelector\"\x15\n\x13\x44\x65psNoPackagesFound\"n\n\x16\x44\x65psNoPackagesFoundMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32 .proto_types.DepsNoPackagesFound\"/\n\x17\x44\x65psStartPackageInstall\x12\x14\n\x0cpackage_name\x18\x01 \x01(\t\"v\n\x1a\x44\x65psStartPackageInstallMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x32\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32$.proto_types.DepsStartPackageInstall\"\'\n\x0f\x44\x65psInstallInfo\x12\x14\n\x0cversion_name\x18\x01 \x01(\t\"f\n\x12\x44\x65psInstallInfoMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.DepsInstallInfo\"-\n\x13\x44\x65psUpdateAvailable\x12\x16\n\x0eversion_latest\x18\x01 \x01(\t\"n\n\x16\x44\x65psUpdateAvailableMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32 .proto_types.DepsUpdateAvailable\"\x0e\n\x0c\x44\x65psUpToDate\"`\n\x0f\x44\x65psUpToDateMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\'\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x19.proto_types.DepsUpToDate\",\n\x14\x44\x65psListSubdirectory\x12\x14\n\x0csubdirectory\x18\x01 \x01(\t\"p\n\x17\x44\x65psListSubdirectoryMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.DepsListSubdirectory\".\n\x1a\x44\x65psNotifyUpdatesAvailable\x12\x10\n\x08packages\x18\x01 \x03(\t\"|\n\x1d\x44\x65psNotifyUpdatesAvailableMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x35\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\'.proto_types.DepsNotifyUpdatesAvailable\"1\n\x11RetryExternalCall\x12\x0f\n\x07\x61ttempt\x18\x01 \x01(\x05\x12\x0b\n\x03max\x18\x02 \x01(\x05\"j\n\x14RetryExternalCallMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12,\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1e.proto_types.RetryExternalCall\"#\n\x14RecordRetryException\x12\x0b\n\x03\x65xc\x18\x01 \x01(\t\"p\n\x17RecordRetryExceptionMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.RecordRetryException\".\n\x1fRegistryIndexProgressGETRequest\x12\x0b\n\x03url\x18\x01 \x01(\t\"\x86\x01\n\"RegistryIndexProgressGETRequestMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12:\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32,.proto_types.RegistryIndexProgressGETRequest\"B\n RegistryIndexProgressGETResponse\x12\x0b\n\x03url\x18\x01 \x01(\t\x12\x11\n\tresp_code\x18\x02 \x01(\x05\"\x88\x01\n#RegistryIndexProgressGETResponseMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12;\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32-.proto_types.RegistryIndexProgressGETResponse\"2\n\x1eRegistryResponseUnexpectedType\x12\x10\n\x08response\x18\x01 \x01(\t\"\x84\x01\n!RegistryResponseUnexpectedTypeMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x39\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32+.proto_types.RegistryResponseUnexpectedType\"2\n\x1eRegistryResponseMissingTopKeys\x12\x10\n\x08response\x18\x01 \x01(\t\"\x84\x01\n!RegistryResponseMissingTopKeysMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x39\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32+.proto_types.RegistryResponseMissingTopKeys\"5\n!RegistryResponseMissingNestedKeys\x12\x10\n\x08response\x18\x01 \x01(\t\"\x8a\x01\n$RegistryResponseMissingNestedKeysMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12<\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32..proto_types.RegistryResponseMissingNestedKeys\"3\n\x1fRegistryResponseExtraNestedKeys\x12\x10\n\x08response\x18\x01 \x01(\t\"\x86\x01\n\"RegistryResponseExtraNestedKeysMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12:\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32,.proto_types.RegistryResponseExtraNestedKeys\"(\n\x18\x44\x65psSetDownloadDirectory\x12\x0c\n\x04path\x18\x01 \x01(\t\"x\n\x1b\x44\x65psSetDownloadDirectoryMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x33\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32%.proto_types.DepsSetDownloadDirectory\"-\n\x0c\x44\x65psUnpinned\x12\x10\n\x08revision\x18\x01 \x01(\t\x12\x0b\n\x03git\x18\x02 \x01(\t\"`\n\x0f\x44\x65psUnpinnedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\'\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x19.proto_types.DepsUnpinned\"/\n\x1bNoNodesForSelectionCriteria\x12\x10\n\x08spec_raw\x18\x01 \x01(\t\"~\n\x1eNoNodesForSelectionCriteriaMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x36\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32(.proto_types.NoNodesForSelectionCriteria\"*\n\x1bRunningOperationCaughtError\x12\x0b\n\x03\x65xc\x18\x01 \x01(\t\"~\n\x1eRunningOperationCaughtErrorMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x36\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32(.proto_types.RunningOperationCaughtError\"\x11\n\x0f\x43ompileComplete\"f\n\x12\x43ompileCompleteMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.CompileComplete\"\x18\n\x16\x46reshnessCheckComplete\"t\n\x19\x46reshnessCheckCompleteMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x31\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32#.proto_types.FreshnessCheckComplete\"\x1c\n\nSeedHeader\x12\x0e\n\x06header\x18\x01 \x01(\t\"\\\n\rSeedHeaderMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12%\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x17.proto_types.SeedHeader\"3\n\x12SQLRunnerException\x12\x0b\n\x03\x65xc\x18\x01 \x01(\t\x12\x10\n\x08\x65xc_info\x18\x02 \x01(\t\"l\n\x15SQLRunnerExceptionMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.SQLRunnerException\"\xa8\x01\n\rLogTestResult\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0e\n\x06status\x18\x03 \x01(\t\x12\r\n\x05index\x18\x04 \x01(\x05\x12\x12\n\nnum_models\x18\x05 \x01(\x05\x12\x16\n\x0e\x65xecution_time\x18\x06 \x01(\x02\x12\x14\n\x0cnum_failures\x18\x07 \x01(\x05\"b\n\x10LogTestResultMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12(\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1a.proto_types.LogTestResult\"k\n\x0cLogStartLine\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\r\n\x05index\x18\x03 \x01(\x05\x12\r\n\x05total\x18\x04 \x01(\x05\"`\n\x0fLogStartLineMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\'\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x19.proto_types.LogStartLine\"\x95\x01\n\x0eLogModelResult\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x0e\n\x06status\x18\x03 \x01(\t\x12\r\n\x05index\x18\x04 \x01(\x05\x12\r\n\x05total\x18\x05 \x01(\x05\x12\x16\n\x0e\x65xecution_time\x18\x06 \x01(\x02\"d\n\x11LogModelResultMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.LogModelResult\"\xfa\x01\n\x11LogSnapshotResult\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x0e\n\x06status\x18\x03 \x01(\t\x12\r\n\x05index\x18\x04 \x01(\x05\x12\r\n\x05total\x18\x05 \x01(\x05\x12\x16\n\x0e\x65xecution_time\x18\x06 \x01(\x02\x12\x34\n\x03\x63\x66g\x18\x07 \x03(\x0b\x32\'.proto_types.LogSnapshotResult.CfgEntry\x1a*\n\x08\x43\x66gEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"j\n\x14LogSnapshotResultMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12,\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1e.proto_types.LogSnapshotResult\"\xb9\x01\n\rLogSeedResult\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x0e\n\x06status\x18\x02 \x01(\t\x12\x16\n\x0eresult_message\x18\x03 \x01(\t\x12\r\n\x05index\x18\x04 \x01(\x05\x12\r\n\x05total\x18\x05 \x01(\x05\x12\x16\n\x0e\x65xecution_time\x18\x06 \x01(\x02\x12\x0e\n\x06schema\x18\x07 \x01(\t\x12\x10\n\x08relation\x18\x08 \x01(\t\"b\n\x10LogSeedResultMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12(\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1a.proto_types.LogSeedResult\"\xad\x01\n\x12LogFreshnessResult\x12\x0e\n\x06status\x18\x01 \x01(\t\x12(\n\tnode_info\x18\x02 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\r\n\x05index\x18\x03 \x01(\x05\x12\r\n\x05total\x18\x04 \x01(\x05\x12\x16\n\x0e\x65xecution_time\x18\x05 \x01(\x02\x12\x13\n\x0bsource_name\x18\x06 \x01(\t\x12\x12\n\ntable_name\x18\x07 \x01(\t\"l\n\x15LogFreshnessResultMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.LogFreshnessResult\"\"\n\rLogCancelLine\x12\x11\n\tconn_name\x18\x01 \x01(\t\"b\n\x10LogCancelLineMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12(\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1a.proto_types.LogCancelLine\"\x1f\n\x0f\x44\x65\x66\x61ultSelector\x12\x0c\n\x04name\x18\x01 \x01(\t\"f\n\x12\x44\x65\x66\x61ultSelectorMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.DefaultSelector\"5\n\tNodeStart\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\"Z\n\x0cNodeStartMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12$\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x16.proto_types.NodeStart\"g\n\x0cNodeFinished\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12-\n\nrun_result\x18\x02 \x01(\x0b\x32\x19.proto_types.RunResultMsg\"`\n\x0fNodeFinishedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\'\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x19.proto_types.NodeFinished\"+\n\x1bQueryCancelationUnsupported\x12\x0c\n\x04type\x18\x01 \x01(\t\"~\n\x1eQueryCancelationUnsupportedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x36\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32(.proto_types.QueryCancelationUnsupported\"O\n\x0f\x43oncurrencyLine\x12\x13\n\x0bnum_threads\x18\x01 \x01(\x05\x12\x13\n\x0btarget_name\x18\x02 \x01(\t\x12\x12\n\nnode_count\x18\x03 \x01(\x05\"f\n\x12\x43oncurrencyLineMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.ConcurrencyLine\"E\n\x19WritingInjectedSQLForNode\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\"z\n\x1cWritingInjectedSQLForNodeMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x34\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32&.proto_types.WritingInjectedSQLForNode\"9\n\rNodeCompiling\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\"b\n\x10NodeCompilingMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12(\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1a.proto_types.NodeCompiling\"9\n\rNodeExecuting\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\"b\n\x10NodeExecutingMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12(\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1a.proto_types.NodeExecuting\"m\n\x10LogHookStartLine\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x11\n\tstatement\x18\x02 \x01(\t\x12\r\n\x05index\x18\x03 \x01(\x05\x12\r\n\x05total\x18\x04 \x01(\x05\"h\n\x13LogHookStartLineMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.proto_types.LogHookStartLine\"\x93\x01\n\x0eLogHookEndLine\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x11\n\tstatement\x18\x02 \x01(\t\x12\x0e\n\x06status\x18\x03 \x01(\t\x12\r\n\x05index\x18\x04 \x01(\x05\x12\r\n\x05total\x18\x05 \x01(\x05\x12\x16\n\x0e\x65xecution_time\x18\x06 \x01(\x02\"d\n\x11LogHookEndLineMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.LogHookEndLine\"\x93\x01\n\x0fSkippingDetails\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x15\n\rresource_type\x18\x02 \x01(\t\x12\x0e\n\x06schema\x18\x03 \x01(\t\x12\x11\n\tnode_name\x18\x04 \x01(\t\x12\r\n\x05index\x18\x05 \x01(\x05\x12\r\n\x05total\x18\x06 \x01(\x05\"f\n\x12SkippingDetailsMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.SkippingDetails\"\r\n\x0bNothingToDo\"^\n\x0eNothingToDoMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12&\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x18.proto_types.NothingToDo\",\n\x1dRunningOperationUncaughtError\x12\x0b\n\x03\x65xc\x18\x01 \x01(\t\"\x82\x01\n RunningOperationUncaughtErrorMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x38\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32*.proto_types.RunningOperationUncaughtError\"\x93\x01\n\x0c\x45ndRunResult\x12*\n\x07results\x18\x01 \x03(\x0b\x32\x19.proto_types.RunResultMsg\x12\x14\n\x0c\x65lapsed_time\x18\x02 \x01(\x02\x12\x30\n\x0cgenerated_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0f\n\x07success\x18\x04 \x01(\x08\"`\n\x0f\x45ndRunResultMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\'\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x19.proto_types.EndRunResult\"\x11\n\x0fNoNodesSelected\"f\n\x12NoNodesSelectedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.NoNodesSelected\"w\n\x10\x43ommandCompleted\x12\x0f\n\x07\x63ommand\x18\x01 \x01(\t\x12\x0f\n\x07success\x18\x02 \x01(\x08\x12\x30\n\x0c\x63ompleted_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0f\n\x07\x65lapsed\x18\x04 \x01(\x02\"h\n\x13\x43ommandCompletedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.proto_types.CommandCompleted\"k\n\x08ShowNode\x12\x11\n\tnode_name\x18\x01 \x01(\t\x12\x0f\n\x07preview\x18\x02 \x01(\t\x12\x11\n\tis_inline\x18\x03 \x01(\x08\x12\x15\n\routput_format\x18\x04 \x01(\t\x12\x11\n\tunique_id\x18\x05 \x01(\t\"X\n\x0bShowNodeMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12#\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x15.proto_types.ShowNode\"p\n\x0c\x43ompiledNode\x12\x11\n\tnode_name\x18\x01 \x01(\t\x12\x10\n\x08\x63ompiled\x18\x02 \x01(\t\x12\x11\n\tis_inline\x18\x03 \x01(\x08\x12\x15\n\routput_format\x18\x04 \x01(\t\x12\x11\n\tunique_id\x18\x05 \x01(\t\"`\n\x0f\x43ompiledNodeMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\'\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x19.proto_types.CompiledNode\"b\n\x17\x43\x61tchableExceptionOnRun\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12\x0b\n\x03\x65xc\x18\x02 \x01(\t\x12\x10\n\x08\x65xc_info\x18\x03 \x01(\t\"v\n\x1a\x43\x61tchableExceptionOnRunMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x32\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32$.proto_types.CatchableExceptionOnRun\"5\n\x12InternalErrorOnRun\x12\x12\n\nbuild_path\x18\x01 \x01(\t\x12\x0b\n\x03\x65xc\x18\x02 \x01(\t\"l\n\x15InternalErrorOnRunMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.InternalErrorOnRun\"K\n\x15GenericExceptionOnRun\x12\x12\n\nbuild_path\x18\x01 \x01(\t\x12\x11\n\tunique_id\x18\x02 \x01(\t\x12\x0b\n\x03\x65xc\x18\x03 \x01(\t\"r\n\x18GenericExceptionOnRunMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x30\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\".proto_types.GenericExceptionOnRun\"N\n\x1aNodeConnectionReleaseError\x12\x11\n\tnode_name\x18\x01 \x01(\t\x12\x0b\n\x03\x65xc\x18\x02 \x01(\t\x12\x10\n\x08\x65xc_info\x18\x03 \x01(\t\"|\n\x1dNodeConnectionReleaseErrorMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x35\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\'.proto_types.NodeConnectionReleaseError\"\x1f\n\nFoundStats\x12\x11\n\tstat_line\x18\x01 \x01(\t\"\\\n\rFoundStatsMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12%\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x17.proto_types.FoundStats\"\x17\n\x15MainKeyboardInterrupt\"r\n\x18MainKeyboardInterruptMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x30\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\".proto_types.MainKeyboardInterrupt\"#\n\x14MainEncounteredError\x12\x0b\n\x03\x65xc\x18\x01 \x01(\t\"p\n\x17MainEncounteredErrorMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.MainEncounteredError\"%\n\x0eMainStackTrace\x12\x13\n\x0bstack_trace\x18\x01 \x01(\t\"d\n\x11MainStackTraceMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.MainStackTrace\"@\n\x13SystemCouldNotWrite\x12\x0c\n\x04path\x18\x01 \x01(\t\x12\x0e\n\x06reason\x18\x02 \x01(\t\x12\x0b\n\x03\x65xc\x18\x03 \x01(\t\"n\n\x16SystemCouldNotWriteMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32 .proto_types.SystemCouldNotWrite\"!\n\x12SystemExecutingCmd\x12\x0b\n\x03\x63md\x18\x01 \x03(\t\"l\n\x15SystemExecutingCmdMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.SystemExecutingCmd\"\x1c\n\x0cSystemStdOut\x12\x0c\n\x04\x62msg\x18\x01 \x01(\t\"`\n\x0fSystemStdOutMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\'\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x19.proto_types.SystemStdOut\"\x1c\n\x0cSystemStdErr\x12\x0c\n\x04\x62msg\x18\x01 \x01(\t\"`\n\x0fSystemStdErrMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\'\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x19.proto_types.SystemStdErr\",\n\x16SystemReportReturnCode\x12\x12\n\nreturncode\x18\x01 \x01(\x05\"t\n\x19SystemReportReturnCodeMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x31\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32#.proto_types.SystemReportReturnCode\"p\n\x13TimingInfoCollected\x12(\n\tnode_info\x18\x01 \x01(\x0b\x32\x15.proto_types.NodeInfo\x12/\n\x0btiming_info\x18\x02 \x01(\x0b\x32\x1a.proto_types.TimingInfoMsg\"n\n\x16TimingInfoCollectedMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32 .proto_types.TimingInfoCollected\"&\n\x12LogDebugStackTrace\x12\x10\n\x08\x65xc_info\x18\x01 \x01(\t\"l\n\x15LogDebugStackTraceMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.LogDebugStackTrace\"\x1e\n\x0e\x43heckCleanPath\x12\x0c\n\x04path\x18\x01 \x01(\t\"d\n\x11\x43heckCleanPathMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.CheckCleanPath\" \n\x10\x43onfirmCleanPath\x12\x0c\n\x04path\x18\x01 \x01(\t\"h\n\x13\x43onfirmCleanPathMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.proto_types.ConfirmCleanPath\"\"\n\x12ProtectedCleanPath\x12\x0c\n\x04path\x18\x01 \x01(\t\"l\n\x15ProtectedCleanPathMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.ProtectedCleanPath\"\x14\n\x12\x46inishedCleanPaths\"l\n\x15\x46inishedCleanPathsMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.FinishedCleanPaths\"5\n\x0bOpenCommand\x12\x10\n\x08open_cmd\x18\x01 \x01(\t\x12\x14\n\x0cprofiles_dir\x18\x02 \x01(\t\"^\n\x0eOpenCommandMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12&\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x18.proto_types.OpenCommand\"\x19\n\nFormatting\x12\x0b\n\x03msg\x18\x01 \x01(\t\"\\\n\rFormattingMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12%\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x17.proto_types.Formatting\"0\n\x0fServingDocsPort\x12\x0f\n\x07\x61\x64\x64ress\x18\x01 \x01(\t\x12\x0c\n\x04port\x18\x02 \x01(\x05\"f\n\x12ServingDocsPortMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.ServingDocsPort\"%\n\x15ServingDocsAccessInfo\x12\x0c\n\x04port\x18\x01 \x01(\t\"r\n\x18ServingDocsAccessInfoMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x30\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\".proto_types.ServingDocsAccessInfo\"\x15\n\x13ServingDocsExitInfo\"n\n\x16ServingDocsExitInfoMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32 .proto_types.ServingDocsExitInfo\"J\n\x10RunResultWarning\x12\x15\n\rresource_type\x18\x01 \x01(\t\x12\x11\n\tnode_name\x18\x02 \x01(\t\x12\x0c\n\x04path\x18\x03 \x01(\t\"h\n\x13RunResultWarningMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.proto_types.RunResultWarning\"J\n\x10RunResultFailure\x12\x15\n\rresource_type\x18\x01 \x01(\t\x12\x11\n\tnode_name\x18\x02 \x01(\t\x12\x0c\n\x04path\x18\x03 \x01(\t\"h\n\x13RunResultFailureMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.proto_types.RunResultFailure\"k\n\tStatsLine\x12\x30\n\x05stats\x18\x01 \x03(\x0b\x32!.proto_types.StatsLine.StatsEntry\x1a,\n\nStatsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x05:\x02\x38\x01\"Z\n\x0cStatsLineMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12$\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x16.proto_types.StatsLine\"\x1d\n\x0eRunResultError\x12\x0b\n\x03msg\x18\x01 \x01(\t\"d\n\x11RunResultErrorMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.RunResultError\")\n\x17RunResultErrorNoMessage\x12\x0e\n\x06status\x18\x01 \x01(\t\"v\n\x1aRunResultErrorNoMessageMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x32\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32$.proto_types.RunResultErrorNoMessage\"\x1f\n\x0fSQLCompiledPath\x12\x0c\n\x04path\x18\x01 \x01(\t\"f\n\x12SQLCompiledPathMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.SQLCompiledPath\"-\n\x14\x43heckNodeTestFailure\x12\x15\n\rrelation_name\x18\x01 \x01(\t\"p\n\x17\x43heckNodeTestFailureMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12/\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32!.proto_types.CheckNodeTestFailure\"\"\n\x13\x46irstRunResultError\x12\x0b\n\x03msg\x18\x01 \x01(\t\"n\n\x16\x46irstRunResultErrorMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32 .proto_types.FirstRunResultError\"\'\n\x18\x41\x66terFirstRunResultError\x12\x0b\n\x03msg\x18\x01 \x01(\t\"x\n\x1b\x41\x66terFirstRunResultErrorMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x33\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32%.proto_types.AfterFirstRunResultError\"W\n\x0f\x45ndOfRunSummary\x12\x12\n\nnum_errors\x18\x01 \x01(\x05\x12\x14\n\x0cnum_warnings\x18\x02 \x01(\x05\x12\x1a\n\x12keyboard_interrupt\x18\x03 \x01(\x08\"f\n\x12\x45ndOfRunSummaryMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.EndOfRunSummary\"U\n\x13LogSkipBecauseError\x12\x0e\n\x06schema\x18\x01 \x01(\t\x12\x10\n\x08relation\x18\x02 \x01(\t\x12\r\n\x05index\x18\x03 \x01(\x05\x12\r\n\x05total\x18\x04 \x01(\x05\"n\n\x16LogSkipBecauseErrorMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12.\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32 .proto_types.LogSkipBecauseError\"\x14\n\x12\x45nsureGitInstalled\"l\n\x15\x45nsureGitInstalledMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.EnsureGitInstalled\"\x1a\n\x18\x44\x65psCreatingLocalSymlink\"x\n\x1b\x44\x65psCreatingLocalSymlinkMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x33\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32%.proto_types.DepsCreatingLocalSymlink\"\x19\n\x17\x44\x65psSymlinkNotAvailable\"v\n\x1a\x44\x65psSymlinkNotAvailableMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x32\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32$.proto_types.DepsSymlinkNotAvailable\"\x11\n\x0f\x44isableTracking\"f\n\x12\x44isableTrackingMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12*\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1c.proto_types.DisableTracking\"\x1e\n\x0cSendingEvent\x12\x0e\n\x06kwargs\x18\x01 \x01(\t\"`\n\x0fSendingEventMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\'\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x19.proto_types.SendingEvent\"\x12\n\x10SendEventFailure\"h\n\x13SendEventFailureMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12+\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1d.proto_types.SendEventFailure\"\r\n\x0b\x46lushEvents\"^\n\x0e\x46lushEventsMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12&\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x18.proto_types.FlushEvents\"\x14\n\x12\x46lushEventsFailure\"l\n\x15\x46lushEventsFailureMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12-\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1f.proto_types.FlushEventsFailure\"-\n\x19TrackingInitializeFailure\x12\x10\n\x08\x65xc_info\x18\x01 \x01(\t\"z\n\x1cTrackingInitializeFailureMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x34\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32&.proto_types.TrackingInitializeFailure\"&\n\x17RunResultWarningMessage\x12\x0b\n\x03msg\x18\x01 \x01(\t\"v\n\x1aRunResultWarningMessageMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x32\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32$.proto_types.RunResultWarningMessage\"\x1a\n\x0b\x44\x65\x62ugCmdOut\x12\x0b\n\x03msg\x18\x01 \x01(\t\"^\n\x0e\x44\x65\x62ugCmdOutMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12&\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x18.proto_types.DebugCmdOut\"\x1d\n\x0e\x44\x65\x62ugCmdResult\x12\x0b\n\x03msg\x18\x01 \x01(\t\"d\n\x11\x44\x65\x62ugCmdResultMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12)\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x1b.proto_types.DebugCmdResult\"\x19\n\nListCmdOut\x12\x0b\n\x03msg\x18\x01 \x01(\t\"\\\n\rListCmdOutMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12%\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x17.proto_types.ListCmdOut\"\x13\n\x04Note\x12\x0b\n\x03msg\x18\x01 \x01(\t\"P\n\x07NoteMsg\x12$\n\x04info\x18\x01 \x01(\x0b\x32\x16.proto_types.EventInfo\x12\x1f\n\x04\x64\x61ta\x18\x02 \x01(\x0b\x32\x11.proto_types.Noteb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'types_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   _EVENTINFO_EXTRAENTRY._options = None
@@ -164,712 +164,720 @@
   _CONFIGLOGPATHDEPRECATION._serialized_end=5964
   _CONFIGLOGPATHDEPRECATIONMSG._serialized_start=5966
   _CONFIGLOGPATHDEPRECATIONMSG._serialized_end=6086
   _CONFIGTARGETPATHDEPRECATION._serialized_start=6088
   _CONFIGTARGETPATHDEPRECATION._serialized_end=6142
   _CONFIGTARGETPATHDEPRECATIONMSG._serialized_start=6144
   _CONFIGTARGETPATHDEPRECATIONMSG._serialized_end=6270
-  _ADAPTEREVENTDEBUG._serialized_start=6273
-  _ADAPTEREVENTDEBUG._serialized_end=6408
-  _ADAPTEREVENTDEBUGMSG._serialized_start=6410
-  _ADAPTEREVENTDEBUGMSG._serialized_end=6516
-  _ADAPTEREVENTINFO._serialized_start=6519
-  _ADAPTEREVENTINFO._serialized_end=6653
-  _ADAPTEREVENTINFOMSG._serialized_start=6655
-  _ADAPTEREVENTINFOMSG._serialized_end=6759
-  _ADAPTEREVENTWARNING._serialized_start=6762
-  _ADAPTEREVENTWARNING._serialized_end=6899
-  _ADAPTEREVENTWARNINGMSG._serialized_start=6901
-  _ADAPTEREVENTWARNINGMSG._serialized_end=7011
-  _ADAPTEREVENTERROR._serialized_start=7014
-  _ADAPTEREVENTERROR._serialized_end=7167
-  _ADAPTEREVENTERRORMSG._serialized_start=7169
-  _ADAPTEREVENTERRORMSG._serialized_end=7275
-  _NEWCONNECTION._serialized_start=7277
-  _NEWCONNECTION._serialized_end=7372
-  _NEWCONNECTIONMSG._serialized_start=7374
-  _NEWCONNECTIONMSG._serialized_end=7472
-  _CONNECTIONREUSED._serialized_start=7474
-  _CONNECTIONREUSED._serialized_end=7535
-  _CONNECTIONREUSEDMSG._serialized_start=7537
-  _CONNECTIONREUSEDMSG._serialized_end=7641
-  _CONNECTIONLEFTOPENINCLEANUP._serialized_start=7643
-  _CONNECTIONLEFTOPENINCLEANUP._serialized_end=7691
-  _CONNECTIONLEFTOPENINCLEANUPMSG._serialized_start=7693
-  _CONNECTIONLEFTOPENINCLEANUPMSG._serialized_end=7819
-  _CONNECTIONCLOSEDINCLEANUP._serialized_start=7821
-  _CONNECTIONCLOSEDINCLEANUP._serialized_end=7867
-  _CONNECTIONCLOSEDINCLEANUPMSG._serialized_start=7869
-  _CONNECTIONCLOSEDINCLEANUPMSG._serialized_end=7991
-  _ROLLBACKFAILED._serialized_start=7993
-  _ROLLBACKFAILED._serialized_end=8088
-  _ROLLBACKFAILEDMSG._serialized_start=8090
-  _ROLLBACKFAILEDMSG._serialized_end=8190
-  _CONNECTIONCLOSED._serialized_start=8192
-  _CONNECTIONCLOSED._serialized_end=8271
-  _CONNECTIONCLOSEDMSG._serialized_start=8273
-  _CONNECTIONCLOSEDMSG._serialized_end=8377
-  _CONNECTIONLEFTOPEN._serialized_start=8379
-  _CONNECTIONLEFTOPEN._serialized_end=8460
-  _CONNECTIONLEFTOPENMSG._serialized_start=8462
-  _CONNECTIONLEFTOPENMSG._serialized_end=8570
-  _ROLLBACK._serialized_start=8572
-  _ROLLBACK._serialized_end=8643
-  _ROLLBACKMSG._serialized_start=8645
-  _ROLLBACKMSG._serialized_end=8733
-  _CACHEMISS._serialized_start=8735
-  _CACHEMISS._serialized_end=8799
-  _CACHEMISSMSG._serialized_start=8801
-  _CACHEMISSMSG._serialized_end=8891
-  _LISTRELATIONS._serialized_start=8893
-  _LISTRELATIONS._serialized_end=8991
-  _LISTRELATIONSMSG._serialized_start=8993
-  _LISTRELATIONSMSG._serialized_end=9091
-  _CONNECTIONUSED._serialized_start=9093
-  _CONNECTIONUSED._serialized_end=9189
-  _CONNECTIONUSEDMSG._serialized_start=9191
-  _CONNECTIONUSEDMSG._serialized_end=9291
-  _SQLQUERY._serialized_start=9293
-  _SQLQUERY._serialized_end=9377
-  _SQLQUERYMSG._serialized_start=9379
-  _SQLQUERYMSG._serialized_end=9467
-  _SQLQUERYSTATUS._serialized_start=9469
-  _SQLQUERYSTATUS._serialized_end=9560
-  _SQLQUERYSTATUSMSG._serialized_start=9562
-  _SQLQUERYSTATUSMSG._serialized_end=9662
-  _SQLCOMMIT._serialized_start=9664
-  _SQLCOMMIT._serialized_end=9736
-  _SQLCOMMITMSG._serialized_start=9738
-  _SQLCOMMITMSG._serialized_end=9828
-  _COLTYPECHANGE._serialized_start=9830
-  _COLTYPECHANGE._serialized_end=9927
-  _COLTYPECHANGEMSG._serialized_start=9929
-  _COLTYPECHANGEMSG._serialized_end=10027
-  _SCHEMACREATION._serialized_start=10029
-  _SCHEMACREATION._serialized_end=10093
-  _SCHEMACREATIONMSG._serialized_start=10095
-  _SCHEMACREATIONMSG._serialized_end=10195
-  _SCHEMADROP._serialized_start=10197
-  _SCHEMADROP._serialized_end=10257
-  _SCHEMADROPMSG._serialized_start=10259
-  _SCHEMADROPMSG._serialized_end=10351
-  _CACHEACTION._serialized_start=10354
-  _CACHEACTION._serialized_end=10576
-  _CACHEACTIONMSG._serialized_start=10578
-  _CACHEACTIONMSG._serialized_end=10672
-  _CACHEDUMPGRAPH._serialized_start=10675
-  _CACHEDUMPGRAPH._serialized_end=10827
-  _CACHEDUMPGRAPH_DUMPENTRY._serialized_start=10784
-  _CACHEDUMPGRAPH_DUMPENTRY._serialized_end=10827
-  _CACHEDUMPGRAPHMSG._serialized_start=10829
-  _CACHEDUMPGRAPHMSG._serialized_end=10929
-  _ADAPTERIMPORTERROR._serialized_start=10931
-  _ADAPTERIMPORTERROR._serialized_end=10964
-  _ADAPTERIMPORTERRORMSG._serialized_start=10966
-  _ADAPTERIMPORTERRORMSG._serialized_end=11074
-  _PLUGINLOADERROR._serialized_start=11076
-  _PLUGINLOADERROR._serialized_end=11111
-  _PLUGINLOADERRORMSG._serialized_start=11113
-  _PLUGINLOADERRORMSG._serialized_end=11215
-  _NEWCONNECTIONOPENING._serialized_start=11217
-  _NEWCONNECTIONOPENING._serialized_end=11307
-  _NEWCONNECTIONOPENINGMSG._serialized_start=11309
-  _NEWCONNECTIONOPENINGMSG._serialized_end=11421
-  _CODEEXECUTION._serialized_start=11423
-  _CODEEXECUTION._serialized_end=11479
-  _CODEEXECUTIONMSG._serialized_start=11481
-  _CODEEXECUTIONMSG._serialized_end=11579
-  _CODEEXECUTIONSTATUS._serialized_start=11581
-  _CODEEXECUTIONSTATUS._serialized_end=11635
-  _CODEEXECUTIONSTATUSMSG._serialized_start=11637
-  _CODEEXECUTIONSTATUSMSG._serialized_end=11747
-  _CATALOGGENERATIONERROR._serialized_start=11749
-  _CATALOGGENERATIONERROR._serialized_end=11786
-  _CATALOGGENERATIONERRORMSG._serialized_start=11788
-  _CATALOGGENERATIONERRORMSG._serialized_end=11904
-  _WRITECATALOGFAILURE._serialized_start=11906
-  _WRITECATALOGFAILURE._serialized_end=11951
-  _WRITECATALOGFAILUREMSG._serialized_start=11953
-  _WRITECATALOGFAILUREMSG._serialized_end=12063
-  _CATALOGWRITTEN._serialized_start=12065
-  _CATALOGWRITTEN._serialized_end=12095
-  _CATALOGWRITTENMSG._serialized_start=12097
-  _CATALOGWRITTENMSG._serialized_end=12197
-  _CANNOTGENERATEDOCS._serialized_start=12199
-  _CANNOTGENERATEDOCS._serialized_end=12219
-  _CANNOTGENERATEDOCSMSG._serialized_start=12221
-  _CANNOTGENERATEDOCSMSG._serialized_end=12329
-  _BUILDINGCATALOG._serialized_start=12331
-  _BUILDINGCATALOG._serialized_end=12348
-  _BUILDINGCATALOGMSG._serialized_start=12350
-  _BUILDINGCATALOGMSG._serialized_end=12452
-  _DATABASEERRORRUNNINGHOOK._serialized_start=12454
-  _DATABASEERRORRUNNINGHOOK._serialized_end=12499
-  _DATABASEERRORRUNNINGHOOKMSG._serialized_start=12501
-  _DATABASEERRORRUNNINGHOOKMSG._serialized_end=12621
-  _HOOKSRUNNING._serialized_start=12623
-  _HOOKSRUNNING._serialized_end=12675
-  _HOOKSRUNNINGMSG._serialized_start=12677
-  _HOOKSRUNNINGMSG._serialized_end=12773
-  _FINISHEDRUNNINGSTATS._serialized_start=12775
-  _FINISHEDRUNNINGSTATS._serialized_end=12859
-  _FINISHEDRUNNINGSTATSMSG._serialized_start=12861
-  _FINISHEDRUNNINGSTATSMSG._serialized_end=12973
-  _CONSTRAINTNOTENFORCED._serialized_start=12975
-  _CONSTRAINTNOTENFORCED._serialized_end=13035
-  _CONSTRAINTNOTENFORCEDMSG._serialized_start=13037
-  _CONSTRAINTNOTENFORCEDMSG._serialized_end=13151
-  _CONSTRAINTNOTSUPPORTED._serialized_start=13153
-  _CONSTRAINTNOTSUPPORTED._serialized_end=13214
-  _CONSTRAINTNOTSUPPORTEDMSG._serialized_start=13216
-  _CONSTRAINTNOTSUPPORTEDMSG._serialized_end=13332
-  _INPUTFILEDIFFERROR._serialized_start=13334
-  _INPUTFILEDIFFERROR._serialized_end=13389
-  _INPUTFILEDIFFERRORMSG._serialized_start=13391
-  _INPUTFILEDIFFERRORMSG._serialized_end=13499
-  _INVALIDVALUEFORFIELD._serialized_start=13501
-  _INVALIDVALUEFORFIELD._serialized_end=13564
-  _INVALIDVALUEFORFIELDMSG._serialized_start=13566
-  _INVALIDVALUEFORFIELDMSG._serialized_end=13678
-  _VALIDATIONWARNING._serialized_start=13680
-  _VALIDATIONWARNING._serialized_end=13761
-  _VALIDATIONWARNINGMSG._serialized_start=13763
-  _VALIDATIONWARNINGMSG._serialized_end=13869
-  _PARSEPERFINFOPATH._serialized_start=13871
-  _PARSEPERFINFOPATH._serialized_end=13904
-  _PARSEPERFINFOPATHMSG._serialized_start=13906
-  _PARSEPERFINFOPATHMSG._serialized_end=14012
-  _GENERICTESTFILEPARSE._serialized_start=14014
-  _GENERICTESTFILEPARSE._serialized_end=14050
-  _GENERICTESTFILEPARSEMSG._serialized_start=14052
-  _GENERICTESTFILEPARSEMSG._serialized_end=14164
-  _MACROFILEPARSE._serialized_start=14166
-  _MACROFILEPARSE._serialized_end=14196
-  _MACROFILEPARSEMSG._serialized_start=14198
-  _MACROFILEPARSEMSG._serialized_end=14298
-  _PARTIALPARSINGERRORPROCESSINGFILE._serialized_start=14300
-  _PARTIALPARSINGERRORPROCESSINGFILE._serialized_end=14349
-  _PARTIALPARSINGERRORPROCESSINGFILEMSG._serialized_start=14352
-  _PARTIALPARSINGERRORPROCESSINGFILEMSG._serialized_end=14490
-  _PARTIALPARSINGERROR._serialized_start=14493
-  _PARTIALPARSINGERROR._serialized_end=14627
-  _PARTIALPARSINGERROR_EXCINFOENTRY._serialized_start=14581
-  _PARTIALPARSINGERROR_EXCINFOENTRY._serialized_end=14627
-  _PARTIALPARSINGERRORMSG._serialized_start=14629
-  _PARTIALPARSINGERRORMSG._serialized_end=14739
-  _PARTIALPARSINGSKIPPARSING._serialized_start=14741
-  _PARTIALPARSINGSKIPPARSING._serialized_end=14768
-  _PARTIALPARSINGSKIPPARSINGMSG._serialized_start=14770
-  _PARTIALPARSINGSKIPPARSINGMSG._serialized_end=14892
-  _UNABLETOPARTIALPARSE._serialized_start=14894
-  _UNABLETOPARTIALPARSE._serialized_end=14932
-  _UNABLETOPARTIALPARSEMSG._serialized_start=14934
-  _UNABLETOPARTIALPARSEMSG._serialized_end=15046
-  _STATECHECKVARSHASH._serialized_start=15048
-  _STATECHECKVARSHASH._serialized_end=15150
-  _STATECHECKVARSHASHMSG._serialized_start=15152
-  _STATECHECKVARSHASHMSG._serialized_end=15260
-  _PARTIALPARSINGNOTENABLED._serialized_start=15262
-  _PARTIALPARSINGNOTENABLED._serialized_end=15288
-  _PARTIALPARSINGNOTENABLEDMSG._serialized_start=15290
-  _PARTIALPARSINGNOTENABLEDMSG._serialized_end=15410
-  _PARSEDFILELOADFAILED._serialized_start=15412
-  _PARSEDFILELOADFAILED._serialized_end=15479
-  _PARSEDFILELOADFAILEDMSG._serialized_start=15481
-  _PARSEDFILELOADFAILEDMSG._serialized_end=15593
-  _PARTIALPARSINGENABLED._serialized_start=15595
-  _PARTIALPARSINGENABLED._serialized_end=15667
-  _PARTIALPARSINGENABLEDMSG._serialized_start=15669
-  _PARTIALPARSINGENABLEDMSG._serialized_end=15783
-  _PARTIALPARSINGFILE._serialized_start=15785
-  _PARTIALPARSINGFILE._serialized_end=15841
-  _PARTIALPARSINGFILEMSG._serialized_start=15843
-  _PARTIALPARSINGFILEMSG._serialized_end=15951
-  _INVALIDDISABLEDTARGETINTESTNODE._serialized_start=15954
-  _INVALIDDISABLEDTARGETINTESTNODE._serialized_end=16129
-  _INVALIDDISABLEDTARGETINTESTNODEMSG._serialized_start=16132
-  _INVALIDDISABLEDTARGETINTESTNODEMSG._serialized_end=16266
-  _UNUSEDRESOURCECONFIGPATH._serialized_start=16268
-  _UNUSEDRESOURCECONFIGPATH._serialized_end=16323
-  _UNUSEDRESOURCECONFIGPATHMSG._serialized_start=16325
-  _UNUSEDRESOURCECONFIGPATHMSG._serialized_end=16445
-  _SEEDINCREASED._serialized_start=16447
-  _SEEDINCREASED._serialized_end=16498
-  _SEEDINCREASEDMSG._serialized_start=16500
-  _SEEDINCREASEDMSG._serialized_end=16598
-  _SEEDEXCEEDSLIMITSAMEPATH._serialized_start=16600
-  _SEEDEXCEEDSLIMITSAMEPATH._serialized_end=16662
-  _SEEDEXCEEDSLIMITSAMEPATHMSG._serialized_start=16664
-  _SEEDEXCEEDSLIMITSAMEPATHMSG._serialized_end=16784
-  _SEEDEXCEEDSLIMITANDPATHCHANGED._serialized_start=16786
-  _SEEDEXCEEDSLIMITANDPATHCHANGED._serialized_end=16854
-  _SEEDEXCEEDSLIMITANDPATHCHANGEDMSG._serialized_start=16857
-  _SEEDEXCEEDSLIMITANDPATHCHANGEDMSG._serialized_end=16989
-  _SEEDEXCEEDSLIMITCHECKSUMCHANGED._serialized_start=16991
-  _SEEDEXCEEDSLIMITCHECKSUMCHANGED._serialized_end=17083
-  _SEEDEXCEEDSLIMITCHECKSUMCHANGEDMSG._serialized_start=17086
-  _SEEDEXCEEDSLIMITCHECKSUMCHANGEDMSG._serialized_end=17220
-  _UNUSEDTABLES._serialized_start=17222
-  _UNUSEDTABLES._serialized_end=17259
-  _UNUSEDTABLESMSG._serialized_start=17261
-  _UNUSEDTABLESMSG._serialized_end=17357
-  _WRONGRESOURCESCHEMAFILE._serialized_start=17360
-  _WRONGRESOURCESCHEMAFILE._serialized_end=17495
-  _WRONGRESOURCESCHEMAFILEMSG._serialized_start=17497
-  _WRONGRESOURCESCHEMAFILEMSG._serialized_end=17615
-  _NONODEFORYAMLKEY._serialized_start=17617
-  _NONODEFORYAMLKEY._serialized_end=17692
-  _NONODEFORYAMLKEYMSG._serialized_start=17694
-  _NONODEFORYAMLKEYMSG._serialized_end=17798
-  _MACRONOTFOUNDFORPATCH._serialized_start=17800
-  _MACRONOTFOUNDFORPATCH._serialized_end=17843
-  _MACRONOTFOUNDFORPATCHMSG._serialized_start=17845
-  _MACRONOTFOUNDFORPATCHMSG._serialized_end=17959
-  _NODENOTFOUNDORDISABLED._serialized_start=17962
-  _NODENOTFOUNDORDISABLED._serialized_end=18146
-  _NODENOTFOUNDORDISABLEDMSG._serialized_start=18148
-  _NODENOTFOUNDORDISABLEDMSG._serialized_end=18264
-  _JINJALOGWARNING._serialized_start=18266
-  _JINJALOGWARNING._serialized_end=18338
-  _JINJALOGWARNINGMSG._serialized_start=18340
-  _JINJALOGWARNINGMSG._serialized_end=18442
-  _JINJALOGINFO._serialized_start=18444
-  _JINJALOGINFO._serialized_end=18513
-  _JINJALOGINFOMSG._serialized_start=18515
-  _JINJALOGINFOMSG._serialized_end=18611
-  _JINJALOGDEBUG._serialized_start=18613
-  _JINJALOGDEBUG._serialized_end=18683
-  _JINJALOGDEBUGMSG._serialized_start=18685
-  _JINJALOGDEBUGMSG._serialized_end=18783
-  _GITSPARSECHECKOUTSUBDIRECTORY._serialized_start=18785
-  _GITSPARSECHECKOUTSUBDIRECTORY._serialized_end=18832
-  _GITSPARSECHECKOUTSUBDIRECTORYMSG._serialized_start=18835
-  _GITSPARSECHECKOUTSUBDIRECTORYMSG._serialized_end=18965
-  _GITPROGRESSCHECKOUTREVISION._serialized_start=18967
-  _GITPROGRESSCHECKOUTREVISION._serialized_end=19014
-  _GITPROGRESSCHECKOUTREVISIONMSG._serialized_start=19016
-  _GITPROGRESSCHECKOUTREVISIONMSG._serialized_end=19142
-  _GITPROGRESSUPDATINGEXISTINGDEPENDENCY._serialized_start=19144
-  _GITPROGRESSUPDATINGEXISTINGDEPENDENCY._serialized_end=19196
-  _GITPROGRESSUPDATINGEXISTINGDEPENDENCYMSG._serialized_start=19199
-  _GITPROGRESSUPDATINGEXISTINGDEPENDENCYMSG._serialized_end=19345
-  _GITPROGRESSPULLINGNEWDEPENDENCY._serialized_start=19347
-  _GITPROGRESSPULLINGNEWDEPENDENCY._serialized_end=19393
-  _GITPROGRESSPULLINGNEWDEPENDENCYMSG._serialized_start=19396
-  _GITPROGRESSPULLINGNEWDEPENDENCYMSG._serialized_end=19530
-  _GITNOTHINGTODO._serialized_start=19532
-  _GITNOTHINGTODO._serialized_end=19561
-  _GITNOTHINGTODOMSG._serialized_start=19563
-  _GITNOTHINGTODOMSG._serialized_end=19663
-  _GITPROGRESSUPDATEDCHECKOUTRANGE._serialized_start=19665
-  _GITPROGRESSUPDATEDCHECKOUTRANGE._serialized_end=19734
-  _GITPROGRESSUPDATEDCHECKOUTRANGEMSG._serialized_start=19737
-  _GITPROGRESSUPDATEDCHECKOUTRANGEMSG._serialized_end=19871
-  _GITPROGRESSCHECKEDOUTAT._serialized_start=19873
-  _GITPROGRESSCHECKEDOUTAT._serialized_end=19915
-  _GITPROGRESSCHECKEDOUTATMSG._serialized_start=19917
-  _GITPROGRESSCHECKEDOUTATMSG._serialized_end=20035
-  _REGISTRYPROGRESSGETREQUEST._serialized_start=20037
-  _REGISTRYPROGRESSGETREQUEST._serialized_end=20078
-  _REGISTRYPROGRESSGETREQUESTMSG._serialized_start=20080
-  _REGISTRYPROGRESSGETREQUESTMSG._serialized_end=20204
-  _REGISTRYPROGRESSGETRESPONSE._serialized_start=20206
-  _REGISTRYPROGRESSGETRESPONSE._serialized_end=20267
-  _REGISTRYPROGRESSGETRESPONSEMSG._serialized_start=20269
-  _REGISTRYPROGRESSGETRESPONSEMSG._serialized_end=20395
-  _SELECTORREPORTINVALIDSELECTOR._serialized_start=20397
-  _SELECTORREPORTINVALIDSELECTOR._serialized_end=20492
-  _SELECTORREPORTINVALIDSELECTORMSG._serialized_start=20495
-  _SELECTORREPORTINVALIDSELECTORMSG._serialized_end=20625
-  _DEPSNOPACKAGESFOUND._serialized_start=20627
-  _DEPSNOPACKAGESFOUND._serialized_end=20648
-  _DEPSNOPACKAGESFOUNDMSG._serialized_start=20650
-  _DEPSNOPACKAGESFOUNDMSG._serialized_end=20760
-  _DEPSSTARTPACKAGEINSTALL._serialized_start=20762
-  _DEPSSTARTPACKAGEINSTALL._serialized_end=20809
-  _DEPSSTARTPACKAGEINSTALLMSG._serialized_start=20811
-  _DEPSSTARTPACKAGEINSTALLMSG._serialized_end=20929
-  _DEPSINSTALLINFO._serialized_start=20931
-  _DEPSINSTALLINFO._serialized_end=20970
-  _DEPSINSTALLINFOMSG._serialized_start=20972
-  _DEPSINSTALLINFOMSG._serialized_end=21074
-  _DEPSUPDATEAVAILABLE._serialized_start=21076
-  _DEPSUPDATEAVAILABLE._serialized_end=21121
-  _DEPSUPDATEAVAILABLEMSG._serialized_start=21123
-  _DEPSUPDATEAVAILABLEMSG._serialized_end=21233
-  _DEPSUPTODATE._serialized_start=21235
-  _DEPSUPTODATE._serialized_end=21249
-  _DEPSUPTODATEMSG._serialized_start=21251
-  _DEPSUPTODATEMSG._serialized_end=21347
-  _DEPSLISTSUBDIRECTORY._serialized_start=21349
-  _DEPSLISTSUBDIRECTORY._serialized_end=21393
-  _DEPSLISTSUBDIRECTORYMSG._serialized_start=21395
-  _DEPSLISTSUBDIRECTORYMSG._serialized_end=21507
-  _DEPSNOTIFYUPDATESAVAILABLE._serialized_start=21509
-  _DEPSNOTIFYUPDATESAVAILABLE._serialized_end=21555
-  _DEPSNOTIFYUPDATESAVAILABLEMSG._serialized_start=21557
-  _DEPSNOTIFYUPDATESAVAILABLEMSG._serialized_end=21681
-  _RETRYEXTERNALCALL._serialized_start=21683
-  _RETRYEXTERNALCALL._serialized_end=21732
-  _RETRYEXTERNALCALLMSG._serialized_start=21734
-  _RETRYEXTERNALCALLMSG._serialized_end=21840
-  _RECORDRETRYEXCEPTION._serialized_start=21842
-  _RECORDRETRYEXCEPTION._serialized_end=21877
-  _RECORDRETRYEXCEPTIONMSG._serialized_start=21879
-  _RECORDRETRYEXCEPTIONMSG._serialized_end=21991
-  _REGISTRYINDEXPROGRESSGETREQUEST._serialized_start=21993
-  _REGISTRYINDEXPROGRESSGETREQUEST._serialized_end=22039
-  _REGISTRYINDEXPROGRESSGETREQUESTMSG._serialized_start=22042
-  _REGISTRYINDEXPROGRESSGETREQUESTMSG._serialized_end=22176
-  _REGISTRYINDEXPROGRESSGETRESPONSE._serialized_start=22178
-  _REGISTRYINDEXPROGRESSGETRESPONSE._serialized_end=22244
-  _REGISTRYINDEXPROGRESSGETRESPONSEMSG._serialized_start=22247
-  _REGISTRYINDEXPROGRESSGETRESPONSEMSG._serialized_end=22383
-  _REGISTRYRESPONSEUNEXPECTEDTYPE._serialized_start=22385
-  _REGISTRYRESPONSEUNEXPECTEDTYPE._serialized_end=22435
-  _REGISTRYRESPONSEUNEXPECTEDTYPEMSG._serialized_start=22438
-  _REGISTRYRESPONSEUNEXPECTEDTYPEMSG._serialized_end=22570
-  _REGISTRYRESPONSEMISSINGTOPKEYS._serialized_start=22572
-  _REGISTRYRESPONSEMISSINGTOPKEYS._serialized_end=22622
-  _REGISTRYRESPONSEMISSINGTOPKEYSMSG._serialized_start=22625
-  _REGISTRYRESPONSEMISSINGTOPKEYSMSG._serialized_end=22757
-  _REGISTRYRESPONSEMISSINGNESTEDKEYS._serialized_start=22759
-  _REGISTRYRESPONSEMISSINGNESTEDKEYS._serialized_end=22812
-  _REGISTRYRESPONSEMISSINGNESTEDKEYSMSG._serialized_start=22815
-  _REGISTRYRESPONSEMISSINGNESTEDKEYSMSG._serialized_end=22953
-  _REGISTRYRESPONSEEXTRANESTEDKEYS._serialized_start=22955
-  _REGISTRYRESPONSEEXTRANESTEDKEYS._serialized_end=23006
-  _REGISTRYRESPONSEEXTRANESTEDKEYSMSG._serialized_start=23009
-  _REGISTRYRESPONSEEXTRANESTEDKEYSMSG._serialized_end=23143
-  _DEPSSETDOWNLOADDIRECTORY._serialized_start=23145
-  _DEPSSETDOWNLOADDIRECTORY._serialized_end=23185
-  _DEPSSETDOWNLOADDIRECTORYMSG._serialized_start=23187
-  _DEPSSETDOWNLOADDIRECTORYMSG._serialized_end=23307
-  _DEPSUNPINNED._serialized_start=23309
-  _DEPSUNPINNED._serialized_end=23354
-  _DEPSUNPINNEDMSG._serialized_start=23356
-  _DEPSUNPINNEDMSG._serialized_end=23452
-  _NONODESFORSELECTIONCRITERIA._serialized_start=23454
-  _NONODESFORSELECTIONCRITERIA._serialized_end=23501
-  _NONODESFORSELECTIONCRITERIAMSG._serialized_start=23503
-  _NONODESFORSELECTIONCRITERIAMSG._serialized_end=23629
-  _RUNNINGOPERATIONCAUGHTERROR._serialized_start=23631
-  _RUNNINGOPERATIONCAUGHTERROR._serialized_end=23673
-  _RUNNINGOPERATIONCAUGHTERRORMSG._serialized_start=23675
-  _RUNNINGOPERATIONCAUGHTERRORMSG._serialized_end=23801
-  _COMPILECOMPLETE._serialized_start=23803
-  _COMPILECOMPLETE._serialized_end=23820
-  _COMPILECOMPLETEMSG._serialized_start=23822
-  _COMPILECOMPLETEMSG._serialized_end=23924
-  _FRESHNESSCHECKCOMPLETE._serialized_start=23926
-  _FRESHNESSCHECKCOMPLETE._serialized_end=23950
-  _FRESHNESSCHECKCOMPLETEMSG._serialized_start=23952
-  _FRESHNESSCHECKCOMPLETEMSG._serialized_end=24068
-  _SEEDHEADER._serialized_start=24070
-  _SEEDHEADER._serialized_end=24098
-  _SEEDHEADERMSG._serialized_start=24100
-  _SEEDHEADERMSG._serialized_end=24192
-  _SQLRUNNEREXCEPTION._serialized_start=24194
-  _SQLRUNNEREXCEPTION._serialized_end=24245
-  _SQLRUNNEREXCEPTIONMSG._serialized_start=24247
-  _SQLRUNNEREXCEPTIONMSG._serialized_end=24355
-  _LOGTESTRESULT._serialized_start=24358
-  _LOGTESTRESULT._serialized_end=24526
-  _LOGTESTRESULTMSG._serialized_start=24528
-  _LOGTESTRESULTMSG._serialized_end=24626
-  _LOGSTARTLINE._serialized_start=24628
-  _LOGSTARTLINE._serialized_end=24735
-  _LOGSTARTLINEMSG._serialized_start=24737
-  _LOGSTARTLINEMSG._serialized_end=24833
-  _LOGMODELRESULT._serialized_start=24836
-  _LOGMODELRESULT._serialized_end=24985
-  _LOGMODELRESULTMSG._serialized_start=24987
-  _LOGMODELRESULTMSG._serialized_end=25087
-  _LOGSNAPSHOTRESULT._serialized_start=25090
-  _LOGSNAPSHOTRESULT._serialized_end=25340
-  _LOGSNAPSHOTRESULT_CFGENTRY._serialized_start=25298
-  _LOGSNAPSHOTRESULT_CFGENTRY._serialized_end=25340
-  _LOGSNAPSHOTRESULTMSG._serialized_start=25342
-  _LOGSNAPSHOTRESULTMSG._serialized_end=25448
-  _LOGSEEDRESULT._serialized_start=25451
-  _LOGSEEDRESULT._serialized_end=25636
-  _LOGSEEDRESULTMSG._serialized_start=25638
-  _LOGSEEDRESULTMSG._serialized_end=25736
-  _LOGFRESHNESSRESULT._serialized_start=25739
-  _LOGFRESHNESSRESULT._serialized_end=25912
-  _LOGFRESHNESSRESULTMSG._serialized_start=25914
-  _LOGFRESHNESSRESULTMSG._serialized_end=26022
-  _LOGCANCELLINE._serialized_start=26024
-  _LOGCANCELLINE._serialized_end=26058
-  _LOGCANCELLINEMSG._serialized_start=26060
-  _LOGCANCELLINEMSG._serialized_end=26158
-  _DEFAULTSELECTOR._serialized_start=26160
-  _DEFAULTSELECTOR._serialized_end=26191
-  _DEFAULTSELECTORMSG._serialized_start=26193
-  _DEFAULTSELECTORMSG._serialized_end=26295
-  _NODESTART._serialized_start=26297
-  _NODESTART._serialized_end=26350
-  _NODESTARTMSG._serialized_start=26352
-  _NODESTARTMSG._serialized_end=26442
-  _NODEFINISHED._serialized_start=26444
-  _NODEFINISHED._serialized_end=26547
-  _NODEFINISHEDMSG._serialized_start=26549
-  _NODEFINISHEDMSG._serialized_end=26645
-  _QUERYCANCELATIONUNSUPPORTED._serialized_start=26647
-  _QUERYCANCELATIONUNSUPPORTED._serialized_end=26690
-  _QUERYCANCELATIONUNSUPPORTEDMSG._serialized_start=26692
-  _QUERYCANCELATIONUNSUPPORTEDMSG._serialized_end=26818
-  _CONCURRENCYLINE._serialized_start=26820
-  _CONCURRENCYLINE._serialized_end=26899
-  _CONCURRENCYLINEMSG._serialized_start=26901
-  _CONCURRENCYLINEMSG._serialized_end=27003
-  _WRITINGINJECTEDSQLFORNODE._serialized_start=27005
-  _WRITINGINJECTEDSQLFORNODE._serialized_end=27074
-  _WRITINGINJECTEDSQLFORNODEMSG._serialized_start=27076
-  _WRITINGINJECTEDSQLFORNODEMSG._serialized_end=27198
-  _NODECOMPILING._serialized_start=27200
-  _NODECOMPILING._serialized_end=27257
-  _NODECOMPILINGMSG._serialized_start=27259
-  _NODECOMPILINGMSG._serialized_end=27357
-  _NODEEXECUTING._serialized_start=27359
-  _NODEEXECUTING._serialized_end=27416
-  _NODEEXECUTINGMSG._serialized_start=27418
-  _NODEEXECUTINGMSG._serialized_end=27516
-  _LOGHOOKSTARTLINE._serialized_start=27518
-  _LOGHOOKSTARTLINE._serialized_end=27627
-  _LOGHOOKSTARTLINEMSG._serialized_start=27629
-  _LOGHOOKSTARTLINEMSG._serialized_end=27733
-  _LOGHOOKENDLINE._serialized_start=27736
-  _LOGHOOKENDLINE._serialized_end=27883
-  _LOGHOOKENDLINEMSG._serialized_start=27885
-  _LOGHOOKENDLINEMSG._serialized_end=27985
-  _SKIPPINGDETAILS._serialized_start=27988
-  _SKIPPINGDETAILS._serialized_end=28135
-  _SKIPPINGDETAILSMSG._serialized_start=28137
-  _SKIPPINGDETAILSMSG._serialized_end=28239
-  _NOTHINGTODO._serialized_start=28241
-  _NOTHINGTODO._serialized_end=28254
-  _NOTHINGTODOMSG._serialized_start=28256
-  _NOTHINGTODOMSG._serialized_end=28350
-  _RUNNINGOPERATIONUNCAUGHTERROR._serialized_start=28352
-  _RUNNINGOPERATIONUNCAUGHTERROR._serialized_end=28396
-  _RUNNINGOPERATIONUNCAUGHTERRORMSG._serialized_start=28399
-  _RUNNINGOPERATIONUNCAUGHTERRORMSG._serialized_end=28529
-  _ENDRUNRESULT._serialized_start=28532
-  _ENDRUNRESULT._serialized_end=28679
-  _ENDRUNRESULTMSG._serialized_start=28681
-  _ENDRUNRESULTMSG._serialized_end=28777
-  _NONODESSELECTED._serialized_start=28779
-  _NONODESSELECTED._serialized_end=28796
-  _NONODESSELECTEDMSG._serialized_start=28798
-  _NONODESSELECTEDMSG._serialized_end=28900
-  _COMMANDCOMPLETED._serialized_start=28902
-  _COMMANDCOMPLETED._serialized_end=29021
-  _COMMANDCOMPLETEDMSG._serialized_start=29023
-  _COMMANDCOMPLETEDMSG._serialized_end=29127
-  _SHOWNODE._serialized_start=29129
-  _SHOWNODE._serialized_end=29236
-  _SHOWNODEMSG._serialized_start=29238
-  _SHOWNODEMSG._serialized_end=29326
-  _COMPILEDNODE._serialized_start=29328
-  _COMPILEDNODE._serialized_end=29440
-  _COMPILEDNODEMSG._serialized_start=29442
-  _COMPILEDNODEMSG._serialized_end=29538
-  _CATCHABLEEXCEPTIONONRUN._serialized_start=29540
-  _CATCHABLEEXCEPTIONONRUN._serialized_end=29638
-  _CATCHABLEEXCEPTIONONRUNMSG._serialized_start=29640
-  _CATCHABLEEXCEPTIONONRUNMSG._serialized_end=29758
-  _INTERNALERRORONRUN._serialized_start=29760
-  _INTERNALERRORONRUN._serialized_end=29813
-  _INTERNALERRORONRUNMSG._serialized_start=29815
-  _INTERNALERRORONRUNMSG._serialized_end=29923
-  _GENERICEXCEPTIONONRUN._serialized_start=29925
-  _GENERICEXCEPTIONONRUN._serialized_end=30000
-  _GENERICEXCEPTIONONRUNMSG._serialized_start=30002
-  _GENERICEXCEPTIONONRUNMSG._serialized_end=30116
-  _NODECONNECTIONRELEASEERROR._serialized_start=30118
-  _NODECONNECTIONRELEASEERROR._serialized_end=30196
-  _NODECONNECTIONRELEASEERRORMSG._serialized_start=30198
-  _NODECONNECTIONRELEASEERRORMSG._serialized_end=30322
-  _FOUNDSTATS._serialized_start=30324
-  _FOUNDSTATS._serialized_end=30355
-  _FOUNDSTATSMSG._serialized_start=30357
-  _FOUNDSTATSMSG._serialized_end=30449
-  _MAINKEYBOARDINTERRUPT._serialized_start=30451
-  _MAINKEYBOARDINTERRUPT._serialized_end=30474
-  _MAINKEYBOARDINTERRUPTMSG._serialized_start=30476
-  _MAINKEYBOARDINTERRUPTMSG._serialized_end=30590
-  _MAINENCOUNTEREDERROR._serialized_start=30592
-  _MAINENCOUNTEREDERROR._serialized_end=30627
-  _MAINENCOUNTEREDERRORMSG._serialized_start=30629
-  _MAINENCOUNTEREDERRORMSG._serialized_end=30741
-  _MAINSTACKTRACE._serialized_start=30743
-  _MAINSTACKTRACE._serialized_end=30780
-  _MAINSTACKTRACEMSG._serialized_start=30782
-  _MAINSTACKTRACEMSG._serialized_end=30882
-  _SYSTEMCOULDNOTWRITE._serialized_start=30884
-  _SYSTEMCOULDNOTWRITE._serialized_end=30948
-  _SYSTEMCOULDNOTWRITEMSG._serialized_start=30950
-  _SYSTEMCOULDNOTWRITEMSG._serialized_end=31060
-  _SYSTEMEXECUTINGCMD._serialized_start=31062
-  _SYSTEMEXECUTINGCMD._serialized_end=31095
-  _SYSTEMEXECUTINGCMDMSG._serialized_start=31097
-  _SYSTEMEXECUTINGCMDMSG._serialized_end=31205
-  _SYSTEMSTDOUT._serialized_start=31207
-  _SYSTEMSTDOUT._serialized_end=31235
-  _SYSTEMSTDOUTMSG._serialized_start=31237
-  _SYSTEMSTDOUTMSG._serialized_end=31333
-  _SYSTEMSTDERR._serialized_start=31335
-  _SYSTEMSTDERR._serialized_end=31363
-  _SYSTEMSTDERRMSG._serialized_start=31365
-  _SYSTEMSTDERRMSG._serialized_end=31461
-  _SYSTEMREPORTRETURNCODE._serialized_start=31463
-  _SYSTEMREPORTRETURNCODE._serialized_end=31507
-  _SYSTEMREPORTRETURNCODEMSG._serialized_start=31509
-  _SYSTEMREPORTRETURNCODEMSG._serialized_end=31625
-  _TIMINGINFOCOLLECTED._serialized_start=31627
-  _TIMINGINFOCOLLECTED._serialized_end=31739
-  _TIMINGINFOCOLLECTEDMSG._serialized_start=31741
-  _TIMINGINFOCOLLECTEDMSG._serialized_end=31851
-  _LOGDEBUGSTACKTRACE._serialized_start=31853
-  _LOGDEBUGSTACKTRACE._serialized_end=31891
-  _LOGDEBUGSTACKTRACEMSG._serialized_start=31893
-  _LOGDEBUGSTACKTRACEMSG._serialized_end=32001
-  _CHECKCLEANPATH._serialized_start=32003
-  _CHECKCLEANPATH._serialized_end=32033
-  _CHECKCLEANPATHMSG._serialized_start=32035
-  _CHECKCLEANPATHMSG._serialized_end=32135
-  _CONFIRMCLEANPATH._serialized_start=32137
-  _CONFIRMCLEANPATH._serialized_end=32169
-  _CONFIRMCLEANPATHMSG._serialized_start=32171
-  _CONFIRMCLEANPATHMSG._serialized_end=32275
-  _PROTECTEDCLEANPATH._serialized_start=32277
-  _PROTECTEDCLEANPATH._serialized_end=32311
-  _PROTECTEDCLEANPATHMSG._serialized_start=32313
-  _PROTECTEDCLEANPATHMSG._serialized_end=32421
-  _FINISHEDCLEANPATHS._serialized_start=32423
-  _FINISHEDCLEANPATHS._serialized_end=32443
-  _FINISHEDCLEANPATHSMSG._serialized_start=32445
-  _FINISHEDCLEANPATHSMSG._serialized_end=32553
-  _OPENCOMMAND._serialized_start=32555
-  _OPENCOMMAND._serialized_end=32608
-  _OPENCOMMANDMSG._serialized_start=32610
-  _OPENCOMMANDMSG._serialized_end=32704
-  _FORMATTING._serialized_start=32706
-  _FORMATTING._serialized_end=32731
-  _FORMATTINGMSG._serialized_start=32733
-  _FORMATTINGMSG._serialized_end=32825
-  _SERVINGDOCSPORT._serialized_start=32827
-  _SERVINGDOCSPORT._serialized_end=32875
-  _SERVINGDOCSPORTMSG._serialized_start=32877
-  _SERVINGDOCSPORTMSG._serialized_end=32979
-  _SERVINGDOCSACCESSINFO._serialized_start=32981
-  _SERVINGDOCSACCESSINFO._serialized_end=33018
-  _SERVINGDOCSACCESSINFOMSG._serialized_start=33020
-  _SERVINGDOCSACCESSINFOMSG._serialized_end=33134
-  _SERVINGDOCSEXITINFO._serialized_start=33136
-  _SERVINGDOCSEXITINFO._serialized_end=33157
-  _SERVINGDOCSEXITINFOMSG._serialized_start=33159
-  _SERVINGDOCSEXITINFOMSG._serialized_end=33269
-  _RUNRESULTWARNING._serialized_start=33271
-  _RUNRESULTWARNING._serialized_end=33345
-  _RUNRESULTWARNINGMSG._serialized_start=33347
-  _RUNRESULTWARNINGMSG._serialized_end=33451
-  _RUNRESULTFAILURE._serialized_start=33453
-  _RUNRESULTFAILURE._serialized_end=33527
-  _RUNRESULTFAILUREMSG._serialized_start=33529
-  _RUNRESULTFAILUREMSG._serialized_end=33633
-  _STATSLINE._serialized_start=33635
-  _STATSLINE._serialized_end=33742
-  _STATSLINE_STATSENTRY._serialized_start=33698
-  _STATSLINE_STATSENTRY._serialized_end=33742
-  _STATSLINEMSG._serialized_start=33744
-  _STATSLINEMSG._serialized_end=33834
-  _RUNRESULTERROR._serialized_start=33836
-  _RUNRESULTERROR._serialized_end=33865
-  _RUNRESULTERRORMSG._serialized_start=33867
-  _RUNRESULTERRORMSG._serialized_end=33967
-  _RUNRESULTERRORNOMESSAGE._serialized_start=33969
-  _RUNRESULTERRORNOMESSAGE._serialized_end=34010
-  _RUNRESULTERRORNOMESSAGEMSG._serialized_start=34012
-  _RUNRESULTERRORNOMESSAGEMSG._serialized_end=34130
-  _SQLCOMPILEDPATH._serialized_start=34132
-  _SQLCOMPILEDPATH._serialized_end=34163
-  _SQLCOMPILEDPATHMSG._serialized_start=34165
-  _SQLCOMPILEDPATHMSG._serialized_end=34267
-  _CHECKNODETESTFAILURE._serialized_start=34269
-  _CHECKNODETESTFAILURE._serialized_end=34314
-  _CHECKNODETESTFAILUREMSG._serialized_start=34316
-  _CHECKNODETESTFAILUREMSG._serialized_end=34428
-  _FIRSTRUNRESULTERROR._serialized_start=34430
-  _FIRSTRUNRESULTERROR._serialized_end=34464
-  _FIRSTRUNRESULTERRORMSG._serialized_start=34466
-  _FIRSTRUNRESULTERRORMSG._serialized_end=34576
-  _AFTERFIRSTRUNRESULTERROR._serialized_start=34578
-  _AFTERFIRSTRUNRESULTERROR._serialized_end=34617
-  _AFTERFIRSTRUNRESULTERRORMSG._serialized_start=34619
-  _AFTERFIRSTRUNRESULTERRORMSG._serialized_end=34739
-  _ENDOFRUNSUMMARY._serialized_start=34741
-  _ENDOFRUNSUMMARY._serialized_end=34828
-  _ENDOFRUNSUMMARYMSG._serialized_start=34830
-  _ENDOFRUNSUMMARYMSG._serialized_end=34932
-  _LOGSKIPBECAUSEERROR._serialized_start=34934
-  _LOGSKIPBECAUSEERROR._serialized_end=35019
-  _LOGSKIPBECAUSEERRORMSG._serialized_start=35021
-  _LOGSKIPBECAUSEERRORMSG._serialized_end=35131
-  _ENSUREGITINSTALLED._serialized_start=35133
-  _ENSUREGITINSTALLED._serialized_end=35153
-  _ENSUREGITINSTALLEDMSG._serialized_start=35155
-  _ENSUREGITINSTALLEDMSG._serialized_end=35263
-  _DEPSCREATINGLOCALSYMLINK._serialized_start=35265
-  _DEPSCREATINGLOCALSYMLINK._serialized_end=35291
-  _DEPSCREATINGLOCALSYMLINKMSG._serialized_start=35293
-  _DEPSCREATINGLOCALSYMLINKMSG._serialized_end=35413
-  _DEPSSYMLINKNOTAVAILABLE._serialized_start=35415
-  _DEPSSYMLINKNOTAVAILABLE._serialized_end=35440
-  _DEPSSYMLINKNOTAVAILABLEMSG._serialized_start=35442
-  _DEPSSYMLINKNOTAVAILABLEMSG._serialized_end=35560
-  _DISABLETRACKING._serialized_start=35562
-  _DISABLETRACKING._serialized_end=35579
-  _DISABLETRACKINGMSG._serialized_start=35581
-  _DISABLETRACKINGMSG._serialized_end=35683
-  _SENDINGEVENT._serialized_start=35685
-  _SENDINGEVENT._serialized_end=35715
-  _SENDINGEVENTMSG._serialized_start=35717
-  _SENDINGEVENTMSG._serialized_end=35813
-  _SENDEVENTFAILURE._serialized_start=35815
-  _SENDEVENTFAILURE._serialized_end=35833
-  _SENDEVENTFAILUREMSG._serialized_start=35835
-  _SENDEVENTFAILUREMSG._serialized_end=35939
-  _FLUSHEVENTS._serialized_start=35941
-  _FLUSHEVENTS._serialized_end=35954
-  _FLUSHEVENTSMSG._serialized_start=35956
-  _FLUSHEVENTSMSG._serialized_end=36050
-  _FLUSHEVENTSFAILURE._serialized_start=36052
-  _FLUSHEVENTSFAILURE._serialized_end=36072
-  _FLUSHEVENTSFAILUREMSG._serialized_start=36074
-  _FLUSHEVENTSFAILUREMSG._serialized_end=36182
-  _TRACKINGINITIALIZEFAILURE._serialized_start=36184
-  _TRACKINGINITIALIZEFAILURE._serialized_end=36229
-  _TRACKINGINITIALIZEFAILUREMSG._serialized_start=36231
-  _TRACKINGINITIALIZEFAILUREMSG._serialized_end=36353
-  _RUNRESULTWARNINGMESSAGE._serialized_start=36355
-  _RUNRESULTWARNINGMESSAGE._serialized_end=36393
-  _RUNRESULTWARNINGMESSAGEMSG._serialized_start=36395
-  _RUNRESULTWARNINGMESSAGEMSG._serialized_end=36513
-  _DEBUGCMDOUT._serialized_start=36515
-  _DEBUGCMDOUT._serialized_end=36541
-  _DEBUGCMDOUTMSG._serialized_start=36543
-  _DEBUGCMDOUTMSG._serialized_end=36637
-  _DEBUGCMDRESULT._serialized_start=36639
-  _DEBUGCMDRESULT._serialized_end=36668
-  _DEBUGCMDRESULTMSG._serialized_start=36670
-  _DEBUGCMDRESULTMSG._serialized_end=36770
-  _LISTCMDOUT._serialized_start=36772
-  _LISTCMDOUT._serialized_end=36797
-  _LISTCMDOUTMSG._serialized_start=36799
-  _LISTCMDOUTMSG._serialized_end=36891
-  _NOTE._serialized_start=36893
-  _NOTE._serialized_end=36912
-  _NOTEMSG._serialized_start=36914
-  _NOTEMSG._serialized_end=36994
+  _COLLECTFRESHNESSRETURNSIGNATURE._serialized_start=6272
+  _COLLECTFRESHNESSRETURNSIGNATURE._serialized_end=6305
+  _COLLECTFRESHNESSRETURNSIGNATUREMSG._serialized_start=6308
+  _COLLECTFRESHNESSRETURNSIGNATUREMSG._serialized_end=6442
+  _ADAPTEREVENTDEBUG._serialized_start=6445
+  _ADAPTEREVENTDEBUG._serialized_end=6580
+  _ADAPTEREVENTDEBUGMSG._serialized_start=6582
+  _ADAPTEREVENTDEBUGMSG._serialized_end=6688
+  _ADAPTEREVENTINFO._serialized_start=6691
+  _ADAPTEREVENTINFO._serialized_end=6825
+  _ADAPTEREVENTINFOMSG._serialized_start=6827
+  _ADAPTEREVENTINFOMSG._serialized_end=6931
+  _ADAPTEREVENTWARNING._serialized_start=6934
+  _ADAPTEREVENTWARNING._serialized_end=7071
+  _ADAPTEREVENTWARNINGMSG._serialized_start=7073
+  _ADAPTEREVENTWARNINGMSG._serialized_end=7183
+  _ADAPTEREVENTERROR._serialized_start=7186
+  _ADAPTEREVENTERROR._serialized_end=7339
+  _ADAPTEREVENTERRORMSG._serialized_start=7341
+  _ADAPTEREVENTERRORMSG._serialized_end=7447
+  _NEWCONNECTION._serialized_start=7449
+  _NEWCONNECTION._serialized_end=7544
+  _NEWCONNECTIONMSG._serialized_start=7546
+  _NEWCONNECTIONMSG._serialized_end=7644
+  _CONNECTIONREUSED._serialized_start=7646
+  _CONNECTIONREUSED._serialized_end=7707
+  _CONNECTIONREUSEDMSG._serialized_start=7709
+  _CONNECTIONREUSEDMSG._serialized_end=7813
+  _CONNECTIONLEFTOPENINCLEANUP._serialized_start=7815
+  _CONNECTIONLEFTOPENINCLEANUP._serialized_end=7863
+  _CONNECTIONLEFTOPENINCLEANUPMSG._serialized_start=7865
+  _CONNECTIONLEFTOPENINCLEANUPMSG._serialized_end=7991
+  _CONNECTIONCLOSEDINCLEANUP._serialized_start=7993
+  _CONNECTIONCLOSEDINCLEANUP._serialized_end=8039
+  _CONNECTIONCLOSEDINCLEANUPMSG._serialized_start=8041
+  _CONNECTIONCLOSEDINCLEANUPMSG._serialized_end=8163
+  _ROLLBACKFAILED._serialized_start=8165
+  _ROLLBACKFAILED._serialized_end=8260
+  _ROLLBACKFAILEDMSG._serialized_start=8262
+  _ROLLBACKFAILEDMSG._serialized_end=8362
+  _CONNECTIONCLOSED._serialized_start=8364
+  _CONNECTIONCLOSED._serialized_end=8443
+  _CONNECTIONCLOSEDMSG._serialized_start=8445
+  _CONNECTIONCLOSEDMSG._serialized_end=8549
+  _CONNECTIONLEFTOPEN._serialized_start=8551
+  _CONNECTIONLEFTOPEN._serialized_end=8632
+  _CONNECTIONLEFTOPENMSG._serialized_start=8634
+  _CONNECTIONLEFTOPENMSG._serialized_end=8742
+  _ROLLBACK._serialized_start=8744
+  _ROLLBACK._serialized_end=8815
+  _ROLLBACKMSG._serialized_start=8817
+  _ROLLBACKMSG._serialized_end=8905
+  _CACHEMISS._serialized_start=8907
+  _CACHEMISS._serialized_end=8971
+  _CACHEMISSMSG._serialized_start=8973
+  _CACHEMISSMSG._serialized_end=9063
+  _LISTRELATIONS._serialized_start=9065
+  _LISTRELATIONS._serialized_end=9163
+  _LISTRELATIONSMSG._serialized_start=9165
+  _LISTRELATIONSMSG._serialized_end=9263
+  _CONNECTIONUSED._serialized_start=9265
+  _CONNECTIONUSED._serialized_end=9361
+  _CONNECTIONUSEDMSG._serialized_start=9363
+  _CONNECTIONUSEDMSG._serialized_end=9463
+  _SQLQUERY._serialized_start=9465
+  _SQLQUERY._serialized_end=9549
+  _SQLQUERYMSG._serialized_start=9551
+  _SQLQUERYMSG._serialized_end=9639
+  _SQLQUERYSTATUS._serialized_start=9641
+  _SQLQUERYSTATUS._serialized_end=9732
+  _SQLQUERYSTATUSMSG._serialized_start=9734
+  _SQLQUERYSTATUSMSG._serialized_end=9834
+  _SQLCOMMIT._serialized_start=9836
+  _SQLCOMMIT._serialized_end=9908
+  _SQLCOMMITMSG._serialized_start=9910
+  _SQLCOMMITMSG._serialized_end=10000
+  _COLTYPECHANGE._serialized_start=10002
+  _COLTYPECHANGE._serialized_end=10099
+  _COLTYPECHANGEMSG._serialized_start=10101
+  _COLTYPECHANGEMSG._serialized_end=10199
+  _SCHEMACREATION._serialized_start=10201
+  _SCHEMACREATION._serialized_end=10265
+  _SCHEMACREATIONMSG._serialized_start=10267
+  _SCHEMACREATIONMSG._serialized_end=10367
+  _SCHEMADROP._serialized_start=10369
+  _SCHEMADROP._serialized_end=10429
+  _SCHEMADROPMSG._serialized_start=10431
+  _SCHEMADROPMSG._serialized_end=10523
+  _CACHEACTION._serialized_start=10526
+  _CACHEACTION._serialized_end=10748
+  _CACHEACTIONMSG._serialized_start=10750
+  _CACHEACTIONMSG._serialized_end=10844
+  _CACHEDUMPGRAPH._serialized_start=10847
+  _CACHEDUMPGRAPH._serialized_end=10999
+  _CACHEDUMPGRAPH_DUMPENTRY._serialized_start=10956
+  _CACHEDUMPGRAPH_DUMPENTRY._serialized_end=10999
+  _CACHEDUMPGRAPHMSG._serialized_start=11001
+  _CACHEDUMPGRAPHMSG._serialized_end=11101
+  _ADAPTERIMPORTERROR._serialized_start=11103
+  _ADAPTERIMPORTERROR._serialized_end=11136
+  _ADAPTERIMPORTERRORMSG._serialized_start=11138
+  _ADAPTERIMPORTERRORMSG._serialized_end=11246
+  _PLUGINLOADERROR._serialized_start=11248
+  _PLUGINLOADERROR._serialized_end=11283
+  _PLUGINLOADERRORMSG._serialized_start=11285
+  _PLUGINLOADERRORMSG._serialized_end=11387
+  _NEWCONNECTIONOPENING._serialized_start=11389
+  _NEWCONNECTIONOPENING._serialized_end=11479
+  _NEWCONNECTIONOPENINGMSG._serialized_start=11481
+  _NEWCONNECTIONOPENINGMSG._serialized_end=11593
+  _CODEEXECUTION._serialized_start=11595
+  _CODEEXECUTION._serialized_end=11651
+  _CODEEXECUTIONMSG._serialized_start=11653
+  _CODEEXECUTIONMSG._serialized_end=11751
+  _CODEEXECUTIONSTATUS._serialized_start=11753
+  _CODEEXECUTIONSTATUS._serialized_end=11807
+  _CODEEXECUTIONSTATUSMSG._serialized_start=11809
+  _CODEEXECUTIONSTATUSMSG._serialized_end=11919
+  _CATALOGGENERATIONERROR._serialized_start=11921
+  _CATALOGGENERATIONERROR._serialized_end=11958
+  _CATALOGGENERATIONERRORMSG._serialized_start=11960
+  _CATALOGGENERATIONERRORMSG._serialized_end=12076
+  _WRITECATALOGFAILURE._serialized_start=12078
+  _WRITECATALOGFAILURE._serialized_end=12123
+  _WRITECATALOGFAILUREMSG._serialized_start=12125
+  _WRITECATALOGFAILUREMSG._serialized_end=12235
+  _CATALOGWRITTEN._serialized_start=12237
+  _CATALOGWRITTEN._serialized_end=12267
+  _CATALOGWRITTENMSG._serialized_start=12269
+  _CATALOGWRITTENMSG._serialized_end=12369
+  _CANNOTGENERATEDOCS._serialized_start=12371
+  _CANNOTGENERATEDOCS._serialized_end=12391
+  _CANNOTGENERATEDOCSMSG._serialized_start=12393
+  _CANNOTGENERATEDOCSMSG._serialized_end=12501
+  _BUILDINGCATALOG._serialized_start=12503
+  _BUILDINGCATALOG._serialized_end=12520
+  _BUILDINGCATALOGMSG._serialized_start=12522
+  _BUILDINGCATALOGMSG._serialized_end=12624
+  _DATABASEERRORRUNNINGHOOK._serialized_start=12626
+  _DATABASEERRORRUNNINGHOOK._serialized_end=12671
+  _DATABASEERRORRUNNINGHOOKMSG._serialized_start=12673
+  _DATABASEERRORRUNNINGHOOKMSG._serialized_end=12793
+  _HOOKSRUNNING._serialized_start=12795
+  _HOOKSRUNNING._serialized_end=12847
+  _HOOKSRUNNINGMSG._serialized_start=12849
+  _HOOKSRUNNINGMSG._serialized_end=12945
+  _FINISHEDRUNNINGSTATS._serialized_start=12947
+  _FINISHEDRUNNINGSTATS._serialized_end=13031
+  _FINISHEDRUNNINGSTATSMSG._serialized_start=13033
+  _FINISHEDRUNNINGSTATSMSG._serialized_end=13145
+  _CONSTRAINTNOTENFORCED._serialized_start=13147
+  _CONSTRAINTNOTENFORCED._serialized_end=13207
+  _CONSTRAINTNOTENFORCEDMSG._serialized_start=13209
+  _CONSTRAINTNOTENFORCEDMSG._serialized_end=13323
+  _CONSTRAINTNOTSUPPORTED._serialized_start=13325
+  _CONSTRAINTNOTSUPPORTED._serialized_end=13386
+  _CONSTRAINTNOTSUPPORTEDMSG._serialized_start=13388
+  _CONSTRAINTNOTSUPPORTEDMSG._serialized_end=13504
+  _INPUTFILEDIFFERROR._serialized_start=13506
+  _INPUTFILEDIFFERROR._serialized_end=13561
+  _INPUTFILEDIFFERRORMSG._serialized_start=13563
+  _INPUTFILEDIFFERRORMSG._serialized_end=13671
+  _INVALIDVALUEFORFIELD._serialized_start=13673
+  _INVALIDVALUEFORFIELD._serialized_end=13736
+  _INVALIDVALUEFORFIELDMSG._serialized_start=13738
+  _INVALIDVALUEFORFIELDMSG._serialized_end=13850
+  _VALIDATIONWARNING._serialized_start=13852
+  _VALIDATIONWARNING._serialized_end=13933
+  _VALIDATIONWARNINGMSG._serialized_start=13935
+  _VALIDATIONWARNINGMSG._serialized_end=14041
+  _PARSEPERFINFOPATH._serialized_start=14043
+  _PARSEPERFINFOPATH._serialized_end=14076
+  _PARSEPERFINFOPATHMSG._serialized_start=14078
+  _PARSEPERFINFOPATHMSG._serialized_end=14184
+  _GENERICTESTFILEPARSE._serialized_start=14186
+  _GENERICTESTFILEPARSE._serialized_end=14222
+  _GENERICTESTFILEPARSEMSG._serialized_start=14224
+  _GENERICTESTFILEPARSEMSG._serialized_end=14336
+  _MACROFILEPARSE._serialized_start=14338
+  _MACROFILEPARSE._serialized_end=14368
+  _MACROFILEPARSEMSG._serialized_start=14370
+  _MACROFILEPARSEMSG._serialized_end=14470
+  _PARTIALPARSINGERRORPROCESSINGFILE._serialized_start=14472
+  _PARTIALPARSINGERRORPROCESSINGFILE._serialized_end=14521
+  _PARTIALPARSINGERRORPROCESSINGFILEMSG._serialized_start=14524
+  _PARTIALPARSINGERRORPROCESSINGFILEMSG._serialized_end=14662
+  _PARTIALPARSINGERROR._serialized_start=14665
+  _PARTIALPARSINGERROR._serialized_end=14799
+  _PARTIALPARSINGERROR_EXCINFOENTRY._serialized_start=14753
+  _PARTIALPARSINGERROR_EXCINFOENTRY._serialized_end=14799
+  _PARTIALPARSINGERRORMSG._serialized_start=14801
+  _PARTIALPARSINGERRORMSG._serialized_end=14911
+  _PARTIALPARSINGSKIPPARSING._serialized_start=14913
+  _PARTIALPARSINGSKIPPARSING._serialized_end=14940
+  _PARTIALPARSINGSKIPPARSINGMSG._serialized_start=14942
+  _PARTIALPARSINGSKIPPARSINGMSG._serialized_end=15064
+  _UNABLETOPARTIALPARSE._serialized_start=15066
+  _UNABLETOPARTIALPARSE._serialized_end=15104
+  _UNABLETOPARTIALPARSEMSG._serialized_start=15106
+  _UNABLETOPARTIALPARSEMSG._serialized_end=15218
+  _STATECHECKVARSHASH._serialized_start=15220
+  _STATECHECKVARSHASH._serialized_end=15322
+  _STATECHECKVARSHASHMSG._serialized_start=15324
+  _STATECHECKVARSHASHMSG._serialized_end=15432
+  _PARTIALPARSINGNOTENABLED._serialized_start=15434
+  _PARTIALPARSINGNOTENABLED._serialized_end=15460
+  _PARTIALPARSINGNOTENABLEDMSG._serialized_start=15462
+  _PARTIALPARSINGNOTENABLEDMSG._serialized_end=15582
+  _PARSEDFILELOADFAILED._serialized_start=15584
+  _PARSEDFILELOADFAILED._serialized_end=15651
+  _PARSEDFILELOADFAILEDMSG._serialized_start=15653
+  _PARSEDFILELOADFAILEDMSG._serialized_end=15765
+  _PARTIALPARSINGENABLED._serialized_start=15767
+  _PARTIALPARSINGENABLED._serialized_end=15839
+  _PARTIALPARSINGENABLEDMSG._serialized_start=15841
+  _PARTIALPARSINGENABLEDMSG._serialized_end=15955
+  _PARTIALPARSINGFILE._serialized_start=15957
+  _PARTIALPARSINGFILE._serialized_end=16013
+  _PARTIALPARSINGFILEMSG._serialized_start=16015
+  _PARTIALPARSINGFILEMSG._serialized_end=16123
+  _INVALIDDISABLEDTARGETINTESTNODE._serialized_start=16126
+  _INVALIDDISABLEDTARGETINTESTNODE._serialized_end=16301
+  _INVALIDDISABLEDTARGETINTESTNODEMSG._serialized_start=16304
+  _INVALIDDISABLEDTARGETINTESTNODEMSG._serialized_end=16438
+  _UNUSEDRESOURCECONFIGPATH._serialized_start=16440
+  _UNUSEDRESOURCECONFIGPATH._serialized_end=16495
+  _UNUSEDRESOURCECONFIGPATHMSG._serialized_start=16497
+  _UNUSEDRESOURCECONFIGPATHMSG._serialized_end=16617
+  _SEEDINCREASED._serialized_start=16619
+  _SEEDINCREASED._serialized_end=16670
+  _SEEDINCREASEDMSG._serialized_start=16672
+  _SEEDINCREASEDMSG._serialized_end=16770
+  _SEEDEXCEEDSLIMITSAMEPATH._serialized_start=16772
+  _SEEDEXCEEDSLIMITSAMEPATH._serialized_end=16834
+  _SEEDEXCEEDSLIMITSAMEPATHMSG._serialized_start=16836
+  _SEEDEXCEEDSLIMITSAMEPATHMSG._serialized_end=16956
+  _SEEDEXCEEDSLIMITANDPATHCHANGED._serialized_start=16958
+  _SEEDEXCEEDSLIMITANDPATHCHANGED._serialized_end=17026
+  _SEEDEXCEEDSLIMITANDPATHCHANGEDMSG._serialized_start=17029
+  _SEEDEXCEEDSLIMITANDPATHCHANGEDMSG._serialized_end=17161
+  _SEEDEXCEEDSLIMITCHECKSUMCHANGED._serialized_start=17163
+  _SEEDEXCEEDSLIMITCHECKSUMCHANGED._serialized_end=17255
+  _SEEDEXCEEDSLIMITCHECKSUMCHANGEDMSG._serialized_start=17258
+  _SEEDEXCEEDSLIMITCHECKSUMCHANGEDMSG._serialized_end=17392
+  _UNUSEDTABLES._serialized_start=17394
+  _UNUSEDTABLES._serialized_end=17431
+  _UNUSEDTABLESMSG._serialized_start=17433
+  _UNUSEDTABLESMSG._serialized_end=17529
+  _WRONGRESOURCESCHEMAFILE._serialized_start=17532
+  _WRONGRESOURCESCHEMAFILE._serialized_end=17667
+  _WRONGRESOURCESCHEMAFILEMSG._serialized_start=17669
+  _WRONGRESOURCESCHEMAFILEMSG._serialized_end=17787
+  _NONODEFORYAMLKEY._serialized_start=17789
+  _NONODEFORYAMLKEY._serialized_end=17864
+  _NONODEFORYAMLKEYMSG._serialized_start=17866
+  _NONODEFORYAMLKEYMSG._serialized_end=17970
+  _MACRONOTFOUNDFORPATCH._serialized_start=17972
+  _MACRONOTFOUNDFORPATCH._serialized_end=18015
+  _MACRONOTFOUNDFORPATCHMSG._serialized_start=18017
+  _MACRONOTFOUNDFORPATCHMSG._serialized_end=18131
+  _NODENOTFOUNDORDISABLED._serialized_start=18134
+  _NODENOTFOUNDORDISABLED._serialized_end=18318
+  _NODENOTFOUNDORDISABLEDMSG._serialized_start=18320
+  _NODENOTFOUNDORDISABLEDMSG._serialized_end=18436
+  _JINJALOGWARNING._serialized_start=18438
+  _JINJALOGWARNING._serialized_end=18510
+  _JINJALOGWARNINGMSG._serialized_start=18512
+  _JINJALOGWARNINGMSG._serialized_end=18614
+  _JINJALOGINFO._serialized_start=18616
+  _JINJALOGINFO._serialized_end=18685
+  _JINJALOGINFOMSG._serialized_start=18687
+  _JINJALOGINFOMSG._serialized_end=18783
+  _JINJALOGDEBUG._serialized_start=18785
+  _JINJALOGDEBUG._serialized_end=18855
+  _JINJALOGDEBUGMSG._serialized_start=18857
+  _JINJALOGDEBUGMSG._serialized_end=18955
+  _UNPINNEDREFNEWVERSIONAVAILABLE._serialized_start=18958
+  _UNPINNEDREFNEWVERSIONAVAILABLE._serialized_end=19132
+  _UNPINNEDREFNEWVERSIONAVAILABLEMSG._serialized_start=19135
+  _UNPINNEDREFNEWVERSIONAVAILABLEMSG._serialized_end=19267
+  _GITSPARSECHECKOUTSUBDIRECTORY._serialized_start=19269
+  _GITSPARSECHECKOUTSUBDIRECTORY._serialized_end=19316
+  _GITSPARSECHECKOUTSUBDIRECTORYMSG._serialized_start=19319
+  _GITSPARSECHECKOUTSUBDIRECTORYMSG._serialized_end=19449
+  _GITPROGRESSCHECKOUTREVISION._serialized_start=19451
+  _GITPROGRESSCHECKOUTREVISION._serialized_end=19498
+  _GITPROGRESSCHECKOUTREVISIONMSG._serialized_start=19500
+  _GITPROGRESSCHECKOUTREVISIONMSG._serialized_end=19626
+  _GITPROGRESSUPDATINGEXISTINGDEPENDENCY._serialized_start=19628
+  _GITPROGRESSUPDATINGEXISTINGDEPENDENCY._serialized_end=19680
+  _GITPROGRESSUPDATINGEXISTINGDEPENDENCYMSG._serialized_start=19683
+  _GITPROGRESSUPDATINGEXISTINGDEPENDENCYMSG._serialized_end=19829
+  _GITPROGRESSPULLINGNEWDEPENDENCY._serialized_start=19831
+  _GITPROGRESSPULLINGNEWDEPENDENCY._serialized_end=19877
+  _GITPROGRESSPULLINGNEWDEPENDENCYMSG._serialized_start=19880
+  _GITPROGRESSPULLINGNEWDEPENDENCYMSG._serialized_end=20014
+  _GITNOTHINGTODO._serialized_start=20016
+  _GITNOTHINGTODO._serialized_end=20045
+  _GITNOTHINGTODOMSG._serialized_start=20047
+  _GITNOTHINGTODOMSG._serialized_end=20147
+  _GITPROGRESSUPDATEDCHECKOUTRANGE._serialized_start=20149
+  _GITPROGRESSUPDATEDCHECKOUTRANGE._serialized_end=20218
+  _GITPROGRESSUPDATEDCHECKOUTRANGEMSG._serialized_start=20221
+  _GITPROGRESSUPDATEDCHECKOUTRANGEMSG._serialized_end=20355
+  _GITPROGRESSCHECKEDOUTAT._serialized_start=20357
+  _GITPROGRESSCHECKEDOUTAT._serialized_end=20399
+  _GITPROGRESSCHECKEDOUTATMSG._serialized_start=20401
+  _GITPROGRESSCHECKEDOUTATMSG._serialized_end=20519
+  _REGISTRYPROGRESSGETREQUEST._serialized_start=20521
+  _REGISTRYPROGRESSGETREQUEST._serialized_end=20562
+  _REGISTRYPROGRESSGETREQUESTMSG._serialized_start=20564
+  _REGISTRYPROGRESSGETREQUESTMSG._serialized_end=20688
+  _REGISTRYPROGRESSGETRESPONSE._serialized_start=20690
+  _REGISTRYPROGRESSGETRESPONSE._serialized_end=20751
+  _REGISTRYPROGRESSGETRESPONSEMSG._serialized_start=20753
+  _REGISTRYPROGRESSGETRESPONSEMSG._serialized_end=20879
+  _SELECTORREPORTINVALIDSELECTOR._serialized_start=20881
+  _SELECTORREPORTINVALIDSELECTOR._serialized_end=20976
+  _SELECTORREPORTINVALIDSELECTORMSG._serialized_start=20979
+  _SELECTORREPORTINVALIDSELECTORMSG._serialized_end=21109
+  _DEPSNOPACKAGESFOUND._serialized_start=21111
+  _DEPSNOPACKAGESFOUND._serialized_end=21132
+  _DEPSNOPACKAGESFOUNDMSG._serialized_start=21134
+  _DEPSNOPACKAGESFOUNDMSG._serialized_end=21244
+  _DEPSSTARTPACKAGEINSTALL._serialized_start=21246
+  _DEPSSTARTPACKAGEINSTALL._serialized_end=21293
+  _DEPSSTARTPACKAGEINSTALLMSG._serialized_start=21295
+  _DEPSSTARTPACKAGEINSTALLMSG._serialized_end=21413
+  _DEPSINSTALLINFO._serialized_start=21415
+  _DEPSINSTALLINFO._serialized_end=21454
+  _DEPSINSTALLINFOMSG._serialized_start=21456
+  _DEPSINSTALLINFOMSG._serialized_end=21558
+  _DEPSUPDATEAVAILABLE._serialized_start=21560
+  _DEPSUPDATEAVAILABLE._serialized_end=21605
+  _DEPSUPDATEAVAILABLEMSG._serialized_start=21607
+  _DEPSUPDATEAVAILABLEMSG._serialized_end=21717
+  _DEPSUPTODATE._serialized_start=21719
+  _DEPSUPTODATE._serialized_end=21733
+  _DEPSUPTODATEMSG._serialized_start=21735
+  _DEPSUPTODATEMSG._serialized_end=21831
+  _DEPSLISTSUBDIRECTORY._serialized_start=21833
+  _DEPSLISTSUBDIRECTORY._serialized_end=21877
+  _DEPSLISTSUBDIRECTORYMSG._serialized_start=21879
+  _DEPSLISTSUBDIRECTORYMSG._serialized_end=21991
+  _DEPSNOTIFYUPDATESAVAILABLE._serialized_start=21993
+  _DEPSNOTIFYUPDATESAVAILABLE._serialized_end=22039
+  _DEPSNOTIFYUPDATESAVAILABLEMSG._serialized_start=22041
+  _DEPSNOTIFYUPDATESAVAILABLEMSG._serialized_end=22165
+  _RETRYEXTERNALCALL._serialized_start=22167
+  _RETRYEXTERNALCALL._serialized_end=22216
+  _RETRYEXTERNALCALLMSG._serialized_start=22218
+  _RETRYEXTERNALCALLMSG._serialized_end=22324
+  _RECORDRETRYEXCEPTION._serialized_start=22326
+  _RECORDRETRYEXCEPTION._serialized_end=22361
+  _RECORDRETRYEXCEPTIONMSG._serialized_start=22363
+  _RECORDRETRYEXCEPTIONMSG._serialized_end=22475
+  _REGISTRYINDEXPROGRESSGETREQUEST._serialized_start=22477
+  _REGISTRYINDEXPROGRESSGETREQUEST._serialized_end=22523
+  _REGISTRYINDEXPROGRESSGETREQUESTMSG._serialized_start=22526
+  _REGISTRYINDEXPROGRESSGETREQUESTMSG._serialized_end=22660
+  _REGISTRYINDEXPROGRESSGETRESPONSE._serialized_start=22662
+  _REGISTRYINDEXPROGRESSGETRESPONSE._serialized_end=22728
+  _REGISTRYINDEXPROGRESSGETRESPONSEMSG._serialized_start=22731
+  _REGISTRYINDEXPROGRESSGETRESPONSEMSG._serialized_end=22867
+  _REGISTRYRESPONSEUNEXPECTEDTYPE._serialized_start=22869
+  _REGISTRYRESPONSEUNEXPECTEDTYPE._serialized_end=22919
+  _REGISTRYRESPONSEUNEXPECTEDTYPEMSG._serialized_start=22922
+  _REGISTRYRESPONSEUNEXPECTEDTYPEMSG._serialized_end=23054
+  _REGISTRYRESPONSEMISSINGTOPKEYS._serialized_start=23056
+  _REGISTRYRESPONSEMISSINGTOPKEYS._serialized_end=23106
+  _REGISTRYRESPONSEMISSINGTOPKEYSMSG._serialized_start=23109
+  _REGISTRYRESPONSEMISSINGTOPKEYSMSG._serialized_end=23241
+  _REGISTRYRESPONSEMISSINGNESTEDKEYS._serialized_start=23243
+  _REGISTRYRESPONSEMISSINGNESTEDKEYS._serialized_end=23296
+  _REGISTRYRESPONSEMISSINGNESTEDKEYSMSG._serialized_start=23299
+  _REGISTRYRESPONSEMISSINGNESTEDKEYSMSG._serialized_end=23437
+  _REGISTRYRESPONSEEXTRANESTEDKEYS._serialized_start=23439
+  _REGISTRYRESPONSEEXTRANESTEDKEYS._serialized_end=23490
+  _REGISTRYRESPONSEEXTRANESTEDKEYSMSG._serialized_start=23493
+  _REGISTRYRESPONSEEXTRANESTEDKEYSMSG._serialized_end=23627
+  _DEPSSETDOWNLOADDIRECTORY._serialized_start=23629
+  _DEPSSETDOWNLOADDIRECTORY._serialized_end=23669
+  _DEPSSETDOWNLOADDIRECTORYMSG._serialized_start=23671
+  _DEPSSETDOWNLOADDIRECTORYMSG._serialized_end=23791
+  _DEPSUNPINNED._serialized_start=23793
+  _DEPSUNPINNED._serialized_end=23838
+  _DEPSUNPINNEDMSG._serialized_start=23840
+  _DEPSUNPINNEDMSG._serialized_end=23936
+  _NONODESFORSELECTIONCRITERIA._serialized_start=23938
+  _NONODESFORSELECTIONCRITERIA._serialized_end=23985
+  _NONODESFORSELECTIONCRITERIAMSG._serialized_start=23987
+  _NONODESFORSELECTIONCRITERIAMSG._serialized_end=24113
+  _RUNNINGOPERATIONCAUGHTERROR._serialized_start=24115
+  _RUNNINGOPERATIONCAUGHTERROR._serialized_end=24157
+  _RUNNINGOPERATIONCAUGHTERRORMSG._serialized_start=24159
+  _RUNNINGOPERATIONCAUGHTERRORMSG._serialized_end=24285
+  _COMPILECOMPLETE._serialized_start=24287
+  _COMPILECOMPLETE._serialized_end=24304
+  _COMPILECOMPLETEMSG._serialized_start=24306
+  _COMPILECOMPLETEMSG._serialized_end=24408
+  _FRESHNESSCHECKCOMPLETE._serialized_start=24410
+  _FRESHNESSCHECKCOMPLETE._serialized_end=24434
+  _FRESHNESSCHECKCOMPLETEMSG._serialized_start=24436
+  _FRESHNESSCHECKCOMPLETEMSG._serialized_end=24552
+  _SEEDHEADER._serialized_start=24554
+  _SEEDHEADER._serialized_end=24582
+  _SEEDHEADERMSG._serialized_start=24584
+  _SEEDHEADERMSG._serialized_end=24676
+  _SQLRUNNEREXCEPTION._serialized_start=24678
+  _SQLRUNNEREXCEPTION._serialized_end=24729
+  _SQLRUNNEREXCEPTIONMSG._serialized_start=24731
+  _SQLRUNNEREXCEPTIONMSG._serialized_end=24839
+  _LOGTESTRESULT._serialized_start=24842
+  _LOGTESTRESULT._serialized_end=25010
+  _LOGTESTRESULTMSG._serialized_start=25012
+  _LOGTESTRESULTMSG._serialized_end=25110
+  _LOGSTARTLINE._serialized_start=25112
+  _LOGSTARTLINE._serialized_end=25219
+  _LOGSTARTLINEMSG._serialized_start=25221
+  _LOGSTARTLINEMSG._serialized_end=25317
+  _LOGMODELRESULT._serialized_start=25320
+  _LOGMODELRESULT._serialized_end=25469
+  _LOGMODELRESULTMSG._serialized_start=25471
+  _LOGMODELRESULTMSG._serialized_end=25571
+  _LOGSNAPSHOTRESULT._serialized_start=25574
+  _LOGSNAPSHOTRESULT._serialized_end=25824
+  _LOGSNAPSHOTRESULT_CFGENTRY._serialized_start=25782
+  _LOGSNAPSHOTRESULT_CFGENTRY._serialized_end=25824
+  _LOGSNAPSHOTRESULTMSG._serialized_start=25826
+  _LOGSNAPSHOTRESULTMSG._serialized_end=25932
+  _LOGSEEDRESULT._serialized_start=25935
+  _LOGSEEDRESULT._serialized_end=26120
+  _LOGSEEDRESULTMSG._serialized_start=26122
+  _LOGSEEDRESULTMSG._serialized_end=26220
+  _LOGFRESHNESSRESULT._serialized_start=26223
+  _LOGFRESHNESSRESULT._serialized_end=26396
+  _LOGFRESHNESSRESULTMSG._serialized_start=26398
+  _LOGFRESHNESSRESULTMSG._serialized_end=26506
+  _LOGCANCELLINE._serialized_start=26508
+  _LOGCANCELLINE._serialized_end=26542
+  _LOGCANCELLINEMSG._serialized_start=26544
+  _LOGCANCELLINEMSG._serialized_end=26642
+  _DEFAULTSELECTOR._serialized_start=26644
+  _DEFAULTSELECTOR._serialized_end=26675
+  _DEFAULTSELECTORMSG._serialized_start=26677
+  _DEFAULTSELECTORMSG._serialized_end=26779
+  _NODESTART._serialized_start=26781
+  _NODESTART._serialized_end=26834
+  _NODESTARTMSG._serialized_start=26836
+  _NODESTARTMSG._serialized_end=26926
+  _NODEFINISHED._serialized_start=26928
+  _NODEFINISHED._serialized_end=27031
+  _NODEFINISHEDMSG._serialized_start=27033
+  _NODEFINISHEDMSG._serialized_end=27129
+  _QUERYCANCELATIONUNSUPPORTED._serialized_start=27131
+  _QUERYCANCELATIONUNSUPPORTED._serialized_end=27174
+  _QUERYCANCELATIONUNSUPPORTEDMSG._serialized_start=27176
+  _QUERYCANCELATIONUNSUPPORTEDMSG._serialized_end=27302
+  _CONCURRENCYLINE._serialized_start=27304
+  _CONCURRENCYLINE._serialized_end=27383
+  _CONCURRENCYLINEMSG._serialized_start=27385
+  _CONCURRENCYLINEMSG._serialized_end=27487
+  _WRITINGINJECTEDSQLFORNODE._serialized_start=27489
+  _WRITINGINJECTEDSQLFORNODE._serialized_end=27558
+  _WRITINGINJECTEDSQLFORNODEMSG._serialized_start=27560
+  _WRITINGINJECTEDSQLFORNODEMSG._serialized_end=27682
+  _NODECOMPILING._serialized_start=27684
+  _NODECOMPILING._serialized_end=27741
+  _NODECOMPILINGMSG._serialized_start=27743
+  _NODECOMPILINGMSG._serialized_end=27841
+  _NODEEXECUTING._serialized_start=27843
+  _NODEEXECUTING._serialized_end=27900
+  _NODEEXECUTINGMSG._serialized_start=27902
+  _NODEEXECUTINGMSG._serialized_end=28000
+  _LOGHOOKSTARTLINE._serialized_start=28002
+  _LOGHOOKSTARTLINE._serialized_end=28111
+  _LOGHOOKSTARTLINEMSG._serialized_start=28113
+  _LOGHOOKSTARTLINEMSG._serialized_end=28217
+  _LOGHOOKENDLINE._serialized_start=28220
+  _LOGHOOKENDLINE._serialized_end=28367
+  _LOGHOOKENDLINEMSG._serialized_start=28369
+  _LOGHOOKENDLINEMSG._serialized_end=28469
+  _SKIPPINGDETAILS._serialized_start=28472
+  _SKIPPINGDETAILS._serialized_end=28619
+  _SKIPPINGDETAILSMSG._serialized_start=28621
+  _SKIPPINGDETAILSMSG._serialized_end=28723
+  _NOTHINGTODO._serialized_start=28725
+  _NOTHINGTODO._serialized_end=28738
+  _NOTHINGTODOMSG._serialized_start=28740
+  _NOTHINGTODOMSG._serialized_end=28834
+  _RUNNINGOPERATIONUNCAUGHTERROR._serialized_start=28836
+  _RUNNINGOPERATIONUNCAUGHTERROR._serialized_end=28880
+  _RUNNINGOPERATIONUNCAUGHTERRORMSG._serialized_start=28883
+  _RUNNINGOPERATIONUNCAUGHTERRORMSG._serialized_end=29013
+  _ENDRUNRESULT._serialized_start=29016
+  _ENDRUNRESULT._serialized_end=29163
+  _ENDRUNRESULTMSG._serialized_start=29165
+  _ENDRUNRESULTMSG._serialized_end=29261
+  _NONODESSELECTED._serialized_start=29263
+  _NONODESSELECTED._serialized_end=29280
+  _NONODESSELECTEDMSG._serialized_start=29282
+  _NONODESSELECTEDMSG._serialized_end=29384
+  _COMMANDCOMPLETED._serialized_start=29386
+  _COMMANDCOMPLETED._serialized_end=29505
+  _COMMANDCOMPLETEDMSG._serialized_start=29507
+  _COMMANDCOMPLETEDMSG._serialized_end=29611
+  _SHOWNODE._serialized_start=29613
+  _SHOWNODE._serialized_end=29720
+  _SHOWNODEMSG._serialized_start=29722
+  _SHOWNODEMSG._serialized_end=29810
+  _COMPILEDNODE._serialized_start=29812
+  _COMPILEDNODE._serialized_end=29924
+  _COMPILEDNODEMSG._serialized_start=29926
+  _COMPILEDNODEMSG._serialized_end=30022
+  _CATCHABLEEXCEPTIONONRUN._serialized_start=30024
+  _CATCHABLEEXCEPTIONONRUN._serialized_end=30122
+  _CATCHABLEEXCEPTIONONRUNMSG._serialized_start=30124
+  _CATCHABLEEXCEPTIONONRUNMSG._serialized_end=30242
+  _INTERNALERRORONRUN._serialized_start=30244
+  _INTERNALERRORONRUN._serialized_end=30297
+  _INTERNALERRORONRUNMSG._serialized_start=30299
+  _INTERNALERRORONRUNMSG._serialized_end=30407
+  _GENERICEXCEPTIONONRUN._serialized_start=30409
+  _GENERICEXCEPTIONONRUN._serialized_end=30484
+  _GENERICEXCEPTIONONRUNMSG._serialized_start=30486
+  _GENERICEXCEPTIONONRUNMSG._serialized_end=30600
+  _NODECONNECTIONRELEASEERROR._serialized_start=30602
+  _NODECONNECTIONRELEASEERROR._serialized_end=30680
+  _NODECONNECTIONRELEASEERRORMSG._serialized_start=30682
+  _NODECONNECTIONRELEASEERRORMSG._serialized_end=30806
+  _FOUNDSTATS._serialized_start=30808
+  _FOUNDSTATS._serialized_end=30839
+  _FOUNDSTATSMSG._serialized_start=30841
+  _FOUNDSTATSMSG._serialized_end=30933
+  _MAINKEYBOARDINTERRUPT._serialized_start=30935
+  _MAINKEYBOARDINTERRUPT._serialized_end=30958
+  _MAINKEYBOARDINTERRUPTMSG._serialized_start=30960
+  _MAINKEYBOARDINTERRUPTMSG._serialized_end=31074
+  _MAINENCOUNTEREDERROR._serialized_start=31076
+  _MAINENCOUNTEREDERROR._serialized_end=31111
+  _MAINENCOUNTEREDERRORMSG._serialized_start=31113
+  _MAINENCOUNTEREDERRORMSG._serialized_end=31225
+  _MAINSTACKTRACE._serialized_start=31227
+  _MAINSTACKTRACE._serialized_end=31264
+  _MAINSTACKTRACEMSG._serialized_start=31266
+  _MAINSTACKTRACEMSG._serialized_end=31366
+  _SYSTEMCOULDNOTWRITE._serialized_start=31368
+  _SYSTEMCOULDNOTWRITE._serialized_end=31432
+  _SYSTEMCOULDNOTWRITEMSG._serialized_start=31434
+  _SYSTEMCOULDNOTWRITEMSG._serialized_end=31544
+  _SYSTEMEXECUTINGCMD._serialized_start=31546
+  _SYSTEMEXECUTINGCMD._serialized_end=31579
+  _SYSTEMEXECUTINGCMDMSG._serialized_start=31581
+  _SYSTEMEXECUTINGCMDMSG._serialized_end=31689
+  _SYSTEMSTDOUT._serialized_start=31691
+  _SYSTEMSTDOUT._serialized_end=31719
+  _SYSTEMSTDOUTMSG._serialized_start=31721
+  _SYSTEMSTDOUTMSG._serialized_end=31817
+  _SYSTEMSTDERR._serialized_start=31819
+  _SYSTEMSTDERR._serialized_end=31847
+  _SYSTEMSTDERRMSG._serialized_start=31849
+  _SYSTEMSTDERRMSG._serialized_end=31945
+  _SYSTEMREPORTRETURNCODE._serialized_start=31947
+  _SYSTEMREPORTRETURNCODE._serialized_end=31991
+  _SYSTEMREPORTRETURNCODEMSG._serialized_start=31993
+  _SYSTEMREPORTRETURNCODEMSG._serialized_end=32109
+  _TIMINGINFOCOLLECTED._serialized_start=32111
+  _TIMINGINFOCOLLECTED._serialized_end=32223
+  _TIMINGINFOCOLLECTEDMSG._serialized_start=32225
+  _TIMINGINFOCOLLECTEDMSG._serialized_end=32335
+  _LOGDEBUGSTACKTRACE._serialized_start=32337
+  _LOGDEBUGSTACKTRACE._serialized_end=32375
+  _LOGDEBUGSTACKTRACEMSG._serialized_start=32377
+  _LOGDEBUGSTACKTRACEMSG._serialized_end=32485
+  _CHECKCLEANPATH._serialized_start=32487
+  _CHECKCLEANPATH._serialized_end=32517
+  _CHECKCLEANPATHMSG._serialized_start=32519
+  _CHECKCLEANPATHMSG._serialized_end=32619
+  _CONFIRMCLEANPATH._serialized_start=32621
+  _CONFIRMCLEANPATH._serialized_end=32653
+  _CONFIRMCLEANPATHMSG._serialized_start=32655
+  _CONFIRMCLEANPATHMSG._serialized_end=32759
+  _PROTECTEDCLEANPATH._serialized_start=32761
+  _PROTECTEDCLEANPATH._serialized_end=32795
+  _PROTECTEDCLEANPATHMSG._serialized_start=32797
+  _PROTECTEDCLEANPATHMSG._serialized_end=32905
+  _FINISHEDCLEANPATHS._serialized_start=32907
+  _FINISHEDCLEANPATHS._serialized_end=32927
+  _FINISHEDCLEANPATHSMSG._serialized_start=32929
+  _FINISHEDCLEANPATHSMSG._serialized_end=33037
+  _OPENCOMMAND._serialized_start=33039
+  _OPENCOMMAND._serialized_end=33092
+  _OPENCOMMANDMSG._serialized_start=33094
+  _OPENCOMMANDMSG._serialized_end=33188
+  _FORMATTING._serialized_start=33190
+  _FORMATTING._serialized_end=33215
+  _FORMATTINGMSG._serialized_start=33217
+  _FORMATTINGMSG._serialized_end=33309
+  _SERVINGDOCSPORT._serialized_start=33311
+  _SERVINGDOCSPORT._serialized_end=33359
+  _SERVINGDOCSPORTMSG._serialized_start=33361
+  _SERVINGDOCSPORTMSG._serialized_end=33463
+  _SERVINGDOCSACCESSINFO._serialized_start=33465
+  _SERVINGDOCSACCESSINFO._serialized_end=33502
+  _SERVINGDOCSACCESSINFOMSG._serialized_start=33504
+  _SERVINGDOCSACCESSINFOMSG._serialized_end=33618
+  _SERVINGDOCSEXITINFO._serialized_start=33620
+  _SERVINGDOCSEXITINFO._serialized_end=33641
+  _SERVINGDOCSEXITINFOMSG._serialized_start=33643
+  _SERVINGDOCSEXITINFOMSG._serialized_end=33753
+  _RUNRESULTWARNING._serialized_start=33755
+  _RUNRESULTWARNING._serialized_end=33829
+  _RUNRESULTWARNINGMSG._serialized_start=33831
+  _RUNRESULTWARNINGMSG._serialized_end=33935
+  _RUNRESULTFAILURE._serialized_start=33937
+  _RUNRESULTFAILURE._serialized_end=34011
+  _RUNRESULTFAILUREMSG._serialized_start=34013
+  _RUNRESULTFAILUREMSG._serialized_end=34117
+  _STATSLINE._serialized_start=34119
+  _STATSLINE._serialized_end=34226
+  _STATSLINE_STATSENTRY._serialized_start=34182
+  _STATSLINE_STATSENTRY._serialized_end=34226
+  _STATSLINEMSG._serialized_start=34228
+  _STATSLINEMSG._serialized_end=34318
+  _RUNRESULTERROR._serialized_start=34320
+  _RUNRESULTERROR._serialized_end=34349
+  _RUNRESULTERRORMSG._serialized_start=34351
+  _RUNRESULTERRORMSG._serialized_end=34451
+  _RUNRESULTERRORNOMESSAGE._serialized_start=34453
+  _RUNRESULTERRORNOMESSAGE._serialized_end=34494
+  _RUNRESULTERRORNOMESSAGEMSG._serialized_start=34496
+  _RUNRESULTERRORNOMESSAGEMSG._serialized_end=34614
+  _SQLCOMPILEDPATH._serialized_start=34616
+  _SQLCOMPILEDPATH._serialized_end=34647
+  _SQLCOMPILEDPATHMSG._serialized_start=34649
+  _SQLCOMPILEDPATHMSG._serialized_end=34751
+  _CHECKNODETESTFAILURE._serialized_start=34753
+  _CHECKNODETESTFAILURE._serialized_end=34798
+  _CHECKNODETESTFAILUREMSG._serialized_start=34800
+  _CHECKNODETESTFAILUREMSG._serialized_end=34912
+  _FIRSTRUNRESULTERROR._serialized_start=34914
+  _FIRSTRUNRESULTERROR._serialized_end=34948
+  _FIRSTRUNRESULTERRORMSG._serialized_start=34950
+  _FIRSTRUNRESULTERRORMSG._serialized_end=35060
+  _AFTERFIRSTRUNRESULTERROR._serialized_start=35062
+  _AFTERFIRSTRUNRESULTERROR._serialized_end=35101
+  _AFTERFIRSTRUNRESULTERRORMSG._serialized_start=35103
+  _AFTERFIRSTRUNRESULTERRORMSG._serialized_end=35223
+  _ENDOFRUNSUMMARY._serialized_start=35225
+  _ENDOFRUNSUMMARY._serialized_end=35312
+  _ENDOFRUNSUMMARYMSG._serialized_start=35314
+  _ENDOFRUNSUMMARYMSG._serialized_end=35416
+  _LOGSKIPBECAUSEERROR._serialized_start=35418
+  _LOGSKIPBECAUSEERROR._serialized_end=35503
+  _LOGSKIPBECAUSEERRORMSG._serialized_start=35505
+  _LOGSKIPBECAUSEERRORMSG._serialized_end=35615
+  _ENSUREGITINSTALLED._serialized_start=35617
+  _ENSUREGITINSTALLED._serialized_end=35637
+  _ENSUREGITINSTALLEDMSG._serialized_start=35639
+  _ENSUREGITINSTALLEDMSG._serialized_end=35747
+  _DEPSCREATINGLOCALSYMLINK._serialized_start=35749
+  _DEPSCREATINGLOCALSYMLINK._serialized_end=35775
+  _DEPSCREATINGLOCALSYMLINKMSG._serialized_start=35777
+  _DEPSCREATINGLOCALSYMLINKMSG._serialized_end=35897
+  _DEPSSYMLINKNOTAVAILABLE._serialized_start=35899
+  _DEPSSYMLINKNOTAVAILABLE._serialized_end=35924
+  _DEPSSYMLINKNOTAVAILABLEMSG._serialized_start=35926
+  _DEPSSYMLINKNOTAVAILABLEMSG._serialized_end=36044
+  _DISABLETRACKING._serialized_start=36046
+  _DISABLETRACKING._serialized_end=36063
+  _DISABLETRACKINGMSG._serialized_start=36065
+  _DISABLETRACKINGMSG._serialized_end=36167
+  _SENDINGEVENT._serialized_start=36169
+  _SENDINGEVENT._serialized_end=36199
+  _SENDINGEVENTMSG._serialized_start=36201
+  _SENDINGEVENTMSG._serialized_end=36297
+  _SENDEVENTFAILURE._serialized_start=36299
+  _SENDEVENTFAILURE._serialized_end=36317
+  _SENDEVENTFAILUREMSG._serialized_start=36319
+  _SENDEVENTFAILUREMSG._serialized_end=36423
+  _FLUSHEVENTS._serialized_start=36425
+  _FLUSHEVENTS._serialized_end=36438
+  _FLUSHEVENTSMSG._serialized_start=36440
+  _FLUSHEVENTSMSG._serialized_end=36534
+  _FLUSHEVENTSFAILURE._serialized_start=36536
+  _FLUSHEVENTSFAILURE._serialized_end=36556
+  _FLUSHEVENTSFAILUREMSG._serialized_start=36558
+  _FLUSHEVENTSFAILUREMSG._serialized_end=36666
+  _TRACKINGINITIALIZEFAILURE._serialized_start=36668
+  _TRACKINGINITIALIZEFAILURE._serialized_end=36713
+  _TRACKINGINITIALIZEFAILUREMSG._serialized_start=36715
+  _TRACKINGINITIALIZEFAILUREMSG._serialized_end=36837
+  _RUNRESULTWARNINGMESSAGE._serialized_start=36839
+  _RUNRESULTWARNINGMESSAGE._serialized_end=36877
+  _RUNRESULTWARNINGMESSAGEMSG._serialized_start=36879
+  _RUNRESULTWARNINGMESSAGEMSG._serialized_end=36997
+  _DEBUGCMDOUT._serialized_start=36999
+  _DEBUGCMDOUT._serialized_end=37025
+  _DEBUGCMDOUTMSG._serialized_start=37027
+  _DEBUGCMDOUTMSG._serialized_end=37121
+  _DEBUGCMDRESULT._serialized_start=37123
+  _DEBUGCMDRESULT._serialized_end=37152
+  _DEBUGCMDRESULTMSG._serialized_start=37154
+  _DEBUGCMDRESULTMSG._serialized_end=37254
+  _LISTCMDOUT._serialized_start=37256
+  _LISTCMDOUT._serialized_end=37281
+  _LISTCMDOUTMSG._serialized_start=37283
+  _LISTCMDOUTMSG._serialized_end=37375
+  _NOTE._serialized_start=37377
+  _NOTE._serialized_end=37396
+  _NOTEMSG._serialized_start=37398
+  _NOTEMSG._serialized_end=37478
 # @@protoc_insertion_point(module_scope)
```

### Comparing `dbt-core-1.5.0rc2/dbt/exceptions.py` & `dbt-core-1.5.1rc1/dbt/exceptions.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/flags.py` & `dbt-core-1.5.1rc1/dbt/flags.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/graph/cli.py` & `dbt-core-1.5.1rc1/dbt/graph/cli.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/graph/graph.py` & `dbt-core-1.5.1rc1/dbt/graph/graph.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/graph/queue.py` & `dbt-core-1.5.1rc1/dbt/graph/queue.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/graph/selector.py` & `dbt-core-1.5.1rc1/dbt/graph/selector.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/graph/selector_methods.py` & `dbt-core-1.5.1rc1/dbt/graph/selector_methods.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/graph/selector_spec.py` & `dbt-core-1.5.1rc1/dbt/graph/selector_spec.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/helper_types.py` & `dbt-core-1.5.1rc1/dbt/helper_types.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/include/README.md` & `dbt-core-1.5.1rc1/dbt/include/README.md`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/include/global_project/docs/overview.md` & `dbt-core-1.5.1rc1/dbt/include/global_project/docs/overview.md`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/include/global_project/macros/adapters/apply_grants.sql` & `dbt-core-1.5.1rc1/dbt/include/global_project/macros/adapters/apply_grants.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/include/global_project/macros/adapters/columns.sql` & `dbt-core-1.5.1rc1/dbt/include/global_project/macros/adapters/columns.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/include/global_project/macros/adapters/freshness.sql` & `dbt-core-1.5.1rc1/dbt/include/global_project/macros/adapters/freshness.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/include/global_project/macros/adapters/indexes.sql` & `dbt-core-1.5.1rc1/dbt/include/global_project/macros/adapters/indexes.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/include/global_project/macros/adapters/metadata.sql` & `dbt-core-1.5.1rc1/dbt/include/global_project/macros/adapters/metadata.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/include/global_project/macros/adapters/persist_docs.sql` & `dbt-core-1.5.1rc1/dbt/include/global_project/macros/adapters/persist_docs.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/include/global_project/macros/adapters/relation.sql` & `dbt-core-1.5.1rc1/dbt/include/global_project/macros/adapters/relation.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/include/global_project/macros/adapters/schema.sql` & `dbt-core-1.5.1rc1/dbt/include/global_project/macros/adapters/schema.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/include/global_project/macros/adapters/timestamps.sql` & `dbt-core-1.5.1rc1/dbt/include/global_project/macros/adapters/timestamps.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/include/global_project/macros/etc/datetime.sql` & `dbt-core-1.5.1rc1/dbt/include/global_project/macros/etc/datetime.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/include/global_project/macros/etc/statement.sql` & `dbt-core-1.5.1rc1/dbt/include/global_project/macros/etc/statement.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/include/global_project/macros/generic_test_sql/accepted_values.sql` & `dbt-core-1.5.1rc1/dbt/include/global_project/macros/generic_test_sql/accepted_values.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/include/global_project/macros/get_custom_name/get_custom_alias.sql` & `dbt-core-1.5.1rc1/dbt/include/global_project/macros/get_custom_name/get_custom_alias.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/include/global_project/macros/get_custom_name/get_custom_database.sql` & `dbt-core-1.5.1rc1/dbt/include/global_project/macros/get_custom_name/get_custom_database.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/include/global_project/macros/get_custom_name/get_custom_schema.sql` & `dbt-core-1.5.1rc1/dbt/include/global_project/macros/get_custom_name/get_custom_schema.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/include/global_project/macros/materializations/configs.sql` & `dbt-core-1.5.1rc1/dbt/include/global_project/macros/materializations/configs.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/include/global_project/macros/materializations/hooks.sql` & `dbt-core-1.5.1rc1/dbt/include/global_project/macros/materializations/hooks.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/include/global_project/macros/materializations/models/incremental/column_helpers.sql` & `dbt-core-1.5.1rc1/dbt/include/global_project/macros/materializations/models/incremental/column_helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/include/global_project/macros/materializations/models/incremental/incremental.sql` & `dbt-core-1.5.1rc1/dbt/include/global_project/macros/materializations/models/incremental/incremental.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/include/global_project/macros/materializations/models/incremental/merge.sql` & `dbt-core-1.5.1rc1/dbt/include/global_project/macros/materializations/models/incremental/merge.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/include/global_project/macros/materializations/models/incremental/on_schema_change.sql` & `dbt-core-1.5.1rc1/dbt/include/global_project/macros/materializations/models/incremental/on_schema_change.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/include/global_project/macros/materializations/models/incremental/strategies.sql` & `dbt-core-1.5.1rc1/dbt/include/global_project/macros/materializations/models/incremental/strategies.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/include/global_project/macros/materializations/models/table/columns_spec_ddl.sql` & `dbt-core-1.5.1rc1/dbt/include/global_project/macros/materializations/models/table/columns_spec_ddl.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/include/global_project/macros/materializations/models/table/create_table_as.sql` & `dbt-core-1.5.1rc1/dbt/include/global_project/macros/materializations/models/table/create_table_as.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/include/global_project/macros/materializations/models/table/table.sql` & `dbt-core-1.5.1rc1/dbt/include/global_project/macros/materializations/models/table/table.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/include/global_project/macros/materializations/models/view/create_or_replace_view.sql` & `dbt-core-1.5.1rc1/dbt/include/global_project/macros/materializations/models/view/create_or_replace_view.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/include/global_project/macros/materializations/models/view/create_view_as.sql` & `dbt-core-1.5.1rc1/dbt/include/global_project/macros/materializations/models/view/create_view_as.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/include/global_project/macros/materializations/models/view/view.sql` & `dbt-core-1.5.1rc1/dbt/include/global_project/macros/materializations/models/view/view.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/include/global_project/macros/materializations/seeds/helpers.sql` & `dbt-core-1.5.1rc1/dbt/include/global_project/macros/materializations/seeds/helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/include/global_project/macros/materializations/seeds/seed.sql` & `dbt-core-1.5.1rc1/dbt/include/global_project/macros/materializations/seeds/seed.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/include/global_project/macros/materializations/snapshots/helpers.sql` & `dbt-core-1.5.1rc1/dbt/include/global_project/macros/materializations/snapshots/helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/include/global_project/macros/materializations/snapshots/snapshot.sql` & `dbt-core-1.5.1rc1/dbt/include/global_project/macros/materializations/snapshots/snapshot.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/include/global_project/macros/materializations/snapshots/snapshot_merge.sql` & `dbt-core-1.5.1rc1/dbt/include/global_project/macros/materializations/snapshots/snapshot_merge.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/include/global_project/macros/materializations/snapshots/strategies.sql` & `dbt-core-1.5.1rc1/dbt/include/global_project/macros/materializations/snapshots/strategies.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/include/global_project/macros/materializations/tests/helpers.sql` & `dbt-core-1.5.1rc1/dbt/include/global_project/macros/materializations/tests/helpers.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/include/global_project/macros/materializations/tests/test.sql` & `dbt-core-1.5.1rc1/dbt/include/global_project/macros/materializations/tests/test.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/include/global_project/macros/python_model/python.sql` & `dbt-core-1.5.1rc1/dbt/include/global_project/macros/python_model/python.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/include/global_project/macros/utils/data_types.sql` & `dbt-core-1.5.1rc1/dbt/include/global_project/macros/utils/data_types.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/include/global_project/macros/utils/listagg.sql` & `dbt-core-1.5.1rc1/dbt/include/global_project/macros/utils/listagg.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/include/global_project/macros/utils/split_part.sql` & `dbt-core-1.5.1rc1/dbt/include/global_project/macros/utils/split_part.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/include/global_project/tests/generic/builtin.sql` & `dbt-core-1.5.1rc1/dbt/include/global_project/tests/generic/builtin.sql`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/include/index.html` & `dbt-core-1.5.1rc1/dbt/include/index.html`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/include/starter_project/README.md` & `dbt-core-1.5.1rc1/dbt/include/starter_project/README.md`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/include/starter_project/dbt_project.yml` & `dbt-core-1.5.1rc1/dbt/include/starter_project/dbt_project.yml`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/internal_deprecations.py` & `dbt-core-1.5.1rc1/dbt/internal_deprecations.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/logger.py` & `dbt-core-1.5.1rc1/dbt/logger.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/node_types.py` & `dbt-core-1.5.1rc1/dbt/node_types.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/parser/__init__.py` & `dbt-core-1.5.1rc1/dbt/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/parser/analysis.py` & `dbt-core-1.5.1rc1/dbt/parser/analysis.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/parser/base.py` & `dbt-core-1.5.1rc1/dbt/parser/base.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/parser/docs.py` & `dbt-core-1.5.1rc1/dbt/parser/docs.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/parser/generic_test.py` & `dbt-core-1.5.1rc1/dbt/parser/generic_test.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/parser/generic_test_builders.py` & `dbt-core-1.5.1rc1/dbt/parser/generic_test_builders.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/parser/hooks.py` & `dbt-core-1.5.1rc1/dbt/parser/hooks.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/parser/macros.py` & `dbt-core-1.5.1rc1/dbt/parser/macros.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/parser/manifest.py` & `dbt-core-1.5.1rc1/dbt/parser/manifest.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/parser/models.py` & `dbt-core-1.5.1rc1/dbt/parser/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -488,15 +488,15 @@
 
         # set refs and sources on the node object
         refs: List[RefArgs] = []
         for ref in statically_parsed["refs"]:
             if len(ref) == 1:
                 package, name = None, ref[0]
             else:
-                package, name = ref[0], refs[1]
+                package, name = ref
 
             refs.append(RefArgs(package=package, name=name))
 
         node.refs += refs
         node.sources += statically_parsed["sources"]
 
         # configs don't need to be merged into the node because they
```

### Comparing `dbt-core-1.5.0rc2/dbt/parser/partial.py` & `dbt-core-1.5.1rc1/dbt/parser/partial.py`

 * *Files 1% similar despite different names*

```diff
@@ -847,14 +847,20 @@
                     file_id = node.file_id
                     # need to copy new file to saved files in order to get content
                     if file_id in self.new_files:
                         self.saved_files[file_id] = deepcopy(self.new_files[file_id])
                     if self.saved_files[file_id]:
                         source_file = self.saved_files[file_id]
                         self.add_to_pp_files(source_file)
+                    # if the node's group has changed - need to reparse all referencing nodes to ensure valid ref access
+                    if node.group != elem.get("group"):
+                        self.schedule_referencing_nodes_for_parsing(node.unique_id)
+                    # if the node's latest version has changed - need to reparse all referencing nodes to ensure correct ref resolution
+                    if node.is_versioned and node.latest_version != elem.get("latest_version"):
+                        self.schedule_referencing_nodes_for_parsing(node.unique_id)
             # remove from patches
             schema_file.node_patches.remove(elem_unique_id)
 
         # for models, seeds, snapshots (not analyses)
         if dict_key in ["models", "seeds", "snapshots"]:
             # find related tests and remove them
             self.remove_tests(schema_file, dict_key, elem["name"])
```

### Comparing `dbt-core-1.5.0rc2/dbt/parser/read_files.py` & `dbt-core-1.5.1rc1/dbt/parser/read_files.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/parser/schema_renderer.py` & `dbt-core-1.5.1rc1/dbt/parser/schema_renderer.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/parser/schemas.py` & `dbt-core-1.5.1rc1/dbt/parser/schemas.py`

 * *Files 0% similar despite different names*

```diff
@@ -1078,14 +1078,21 @@
                 # ref lookup without version - version is not set yet
                 versioned_model_unique_id = self.manifest.ref_lookup.get_unique_id(
                     versioned_model_name, None, None
                 )
 
                 versioned_model_node = None
                 add_node_nofile_fn: Callable
+
+                # If this is the latest version, it's allowed to define itself in a model file name that doesn't have a suffix
+                if versioned_model_unique_id is None and unparsed_version.v == latest_version:
+                    versioned_model_unique_id = self.manifest.ref_lookup.get_unique_id(
+                        block.name, None, None
+                    )
+
                 if versioned_model_unique_id is None:
                     # Node might be disabled. Following call returns list of matching disabled nodes
                     found_nodes = self.manifest.disabled_lookup.find(versioned_model_name, None)
                     if found_nodes:
                         if len(found_nodes) > 1 and target.config.get("enabled"):
                             # There are multiple disabled nodes for this model and the schema file wants to enable one.
                             # We have no way to know which one to enable.
```

### Comparing `dbt-core-1.5.0rc2/dbt/parser/search.py` & `dbt-core-1.5.1rc1/dbt/parser/search.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/parser/seeds.py` & `dbt-core-1.5.1rc1/dbt/parser/seeds.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/parser/singular_test.py` & `dbt-core-1.5.1rc1/dbt/parser/singular_test.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/parser/snapshots.py` & `dbt-core-1.5.1rc1/dbt/parser/snapshots.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/parser/sources.py` & `dbt-core-1.5.1rc1/dbt/parser/sources.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/parser/sql.py` & `dbt-core-1.5.1rc1/dbt/parser/sql.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/semver.py` & `dbt-core-1.5.1rc1/dbt/semver.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/task/base.py` & `dbt-core-1.5.1rc1/dbt/task/base.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/task/build.py` & `dbt-core-1.5.1rc1/dbt/task/build.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/task/clean.py` & `dbt-core-1.5.1rc1/dbt/task/clean.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/task/compile.py` & `dbt-core-1.5.1rc1/dbt/task/compile.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/task/debug.py` & `dbt-core-1.5.1rc1/dbt/task/debug.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/task/deps.py` & `dbt-core-1.5.1rc1/dbt/task/deps.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/task/freshness.py` & `dbt-core-1.5.1rc1/dbt/task/freshness.py`

 * *Files 6% similar despite different names*

```diff
@@ -113,22 +113,27 @@
                 compiled_node.loaded_at_field,
                 compiled_node.freshness.filter,
                 manifest=manifest,
             )
 
         status = compiled_node.freshness.status(freshness["age"])
 
+        # adapter_response was not returned in previous versions, so this will be None
+        # we cannot call to_dict() on NoneType
+        if adapter_response:
+            adapter_response = adapter_response.to_dict(omit_none=True)
+
         return SourceFreshnessResult(
             node=compiled_node,
             status=status,
             thread_id=threading.current_thread().name,
             timing=[],
             execution_time=0,
             message=None,
-            adapter_response=adapter_response.to_dict(omit_none=True),
+            adapter_response=adapter_response or {},
             failures=None,
             **freshness,
         )
 
     def compile(self, manifest):
         if self.node.resource_type != NodeType.Source:
             # should be unreachable...
```

### Comparing `dbt-core-1.5.0rc2/dbt/task/generate.py` & `dbt-core-1.5.1rc1/dbt/task/generate.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/task/init.py` & `dbt-core-1.5.1rc1/dbt/task/init.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/task/list.py` & `dbt-core-1.5.1rc1/dbt/task/list.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/task/printer.py` & `dbt-core-1.5.1rc1/dbt/task/printer.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/task/run.py` & `dbt-core-1.5.1rc1/dbt/task/run.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/task/run_operation.py` & `dbt-core-1.5.1rc1/dbt/task/run_operation.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/task/runnable.py` & `dbt-core-1.5.1rc1/dbt/task/runnable.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/task/seed.py` & `dbt-core-1.5.1rc1/dbt/task/seed.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/task/serve.py` & `dbt-core-1.5.1rc1/dbt/task/serve.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/task/show.py` & `dbt-core-1.5.1rc1/dbt/task/show.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,34 @@
 import io
 import threading
 import time
 
+from dbt.contracts.graph.nodes import SeedNode
 from dbt.contracts.results import RunResult, RunStatus
 from dbt.events.base_types import EventLevel
 from dbt.events.functions import fire_event
 from dbt.events.types import ShowNode, Note
 from dbt.exceptions import DbtRuntimeError
 from dbt.task.compile import CompileTask, CompileRunner
+from dbt.task.seed import SeedRunner
 
 
 class ShowRunner(CompileRunner):
     def __init__(self, config, adapter, node, node_index, num_nodes):
         super().__init__(config, adapter, node, node_index, num_nodes)
         self.run_ephemeral_models = True
 
     def execute(self, compiled_node, manifest):
         start_time = time.time()
+
+        if "sql_header" in compiled_node.unrendered_config:
+            compiled_node.compiled_code = (
+                compiled_node.unrendered_config["sql_header"] + compiled_node.compiled_code
+            )
+
         adapter_response, execute_result = self.adapter.execute(
             compiled_node.compiled_code, fetch=True
         )
         end_time = time.time()
 
         return RunResult(
             node=compiled_node,
@@ -37,16 +45,19 @@
 
 class ShowTask(CompileTask):
     def _runtime_initialize(self):
         if not (self.args.select or getattr(self.args, "inline", None)):
             raise DbtRuntimeError("Either --select or --inline must be passed to show")
         super()._runtime_initialize()
 
-    def get_runner_type(self, _):
-        return ShowRunner
+    def get_runner_type(self, node):
+        if isinstance(node, SeedNode):
+            return SeedRunner
+        else:
+            return ShowRunner
 
     def task_end_messages(self, results):
         is_inline = bool(getattr(self.args, "inline", None))
 
         if is_inline:
             matched_results = [result for result in results if result.node.name == "inline_query"]
         else:
@@ -71,17 +82,22 @@
             # Hack to get Agate table output as string
             output = io.StringIO()
             if self.args.output == "json":
                 table.to_json(path=output)
             else:
                 table.print_table(output=output, max_rows=None)
 
+            node_name = result.node.name
+
+            if hasattr(result.node, "version") and result.node.version:
+                node_name += f".v{result.node.version}"
+
             fire_event(
                 ShowNode(
-                    node_name=result.node.name,
+                    node_name=node_name,
                     preview=output.getvalue(),
                     is_inline=is_inline,
                     output_format=self.args.output,
                     unique_id=result.node.unique_id,
                 )
             )
```

### Comparing `dbt-core-1.5.0rc2/dbt/task/snapshot.py` & `dbt-core-1.5.1rc1/dbt/task/snapshot.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/task/sql.py` & `dbt-core-1.5.1rc1/dbt/task/sql.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/task/test.py` & `dbt-core-1.5.1rc1/dbt/task/test.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/tests/fixtures/project.py` & `dbt-core-1.5.1rc1/dbt/tests/fixtures/project.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/tests/util.py` & `dbt-core-1.5.1rc1/dbt/tests/util.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/tracking.py` & `dbt-core-1.5.1rc1/dbt/tracking.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/ui.py` & `dbt-core-1.5.1rc1/dbt/ui.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/utils.py` & `dbt-core-1.5.1rc1/dbt/utils.py`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/dbt/version.py` & `dbt-core-1.5.1rc1/dbt/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -228,9 +228,9 @@
             # the path is like .../dbt/adapters/{plugin_name}/__version__.py
             # except it could be \\ on windows!
             plugin_root, _ = os.path.split(version_path)
             _, plugin_name = os.path.split(plugin_root)
             yield plugin_name
 
 
-__version__ = "1.5.0rc2"
+__version__ = "1.5.1rc1"
 installed = get_installed_version()
```

### Comparing `dbt-core-1.5.0rc2/dbt_core.egg-info/PKG-INFO` & `dbt-core-1.5.1rc1/dbt_core.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-core
-Version: 1.5.0rc2
+Version: 1.5.1rc1
 Summary: With dbt, data analysts and engineers can build analytics the way engineers build applications.
 Home-page: https://github.com/dbt-labs/dbt-core
 Author: dbt Labs
 Author-email: info@dbtlabs.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dbt-core Version: 1.5.0rc2 Summary: With dbt, data
+Metadata-Version: 2.1 Name: dbt-core Version: 1.5.1rc1 Summary: With dbt, data
 analysts and engineers can build analytics the way engineers build
 applications. Home-page: https://github.com/dbt-labs/dbt-core Author: dbt Labs
 Author-email: info@dbtlabs.com Classifier: Development Status :: 5 -
 Production/Stable Classifier: License :: OSI Approved :: Apache Software
 License Classifier: Operating System :: Microsoft :: Windows Classifier:
 Operating System :: MacOS :: MacOS X Classifier: Operating System :: POSIX ::
 Linux Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
```

### Comparing `dbt-core-1.5.0rc2/dbt_core.egg-info/SOURCES.txt` & `dbt-core-1.5.1rc1/dbt_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbt-core-1.5.0rc2/setup.py` & `dbt-core-1.5.1rc1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 this_directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(this_directory, "README.md")) as f:
     long_description = f.read()
 
 
 package_name = "dbt-core"
-package_version = "1.5.0rc2"
+package_version = "1.5.1rc1"
 description = """With dbt, data analysts and engineers can build analytics \
 the way engineers build applications."""
 
 
 setup(
     name=package_name,
     version=package_version,
@@ -59,15 +59,15 @@
         "networkx>=2.3,<3;python_version>='3.8'",
         "packaging>20.9",
         "sqlparse>=0.2.3,<0.4.4",
         "dbt-extractor~=0.4.1",
         "typing-extensions>=3.7.4",
         "werkzeug>=1,<3",
         "pathspec>=0.9,<0.12",
-        "protobuf>=3.18.3",
+        "protobuf>=4.0.0",
         "pytz>=2015.7",
         # the following are all to match snowflake-connector-python
         "requests<3.0.0",
         "idna>=2.5,<4",
         "cffi>=1.9,<2.0.0",
         "pyyaml>=6.0",
     ],
```

