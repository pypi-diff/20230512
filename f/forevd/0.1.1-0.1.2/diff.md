# Comparing `tmp/forevd-0.1.1.tar.gz` & `tmp/forevd-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "forevd-0.1.1.tar", max compression
+gzip compressed data, was "forevd-0.1.2.tar", max compression
```

## Comparing `forevd-0.1.1.tar` & `forevd-0.1.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    11357 2023-05-10 03:19:40.654211 forevd-0.1.1/LICENSE
--rw-r--r--   0        0        0      486 2023-05-10 03:19:40.654211 forevd-0.1.1/README.md
--rw-r--r--   0        0        0        0 2023-05-10 03:19:40.654211 forevd-0.1.1/forevd/__init__.py
--rw-r--r--   0        0        0     4390 2023-05-10 03:19:40.654211 forevd-0.1.1/forevd/__main__.py
--rw-r--r--   0        0        0     1498 2023-05-10 03:19:40.654211 forevd-0.1.1/forevd/apache/__init__.py
--rw-r--r--   0        0        0     3370 2023-05-10 03:19:40.654211 forevd-0.1.1/forevd/apache/httpd.conf
--rw-r--r--   0        0        0        0 2023-05-10 03:19:40.654211 forevd-0.1.1/forevd/resources/__init__.py
--rw-r--r--   0        0        0        0 2023-05-10 03:19:40.658211 forevd-0.1.1/forevd/resources/logging/__init__.py
--rw-r--r--   0        0        0      387 2023-05-10 03:19:40.658211 forevd-0.1.1/forevd/resources/logging/cli.conf
--rw-r--r--   0        0        0      844 2023-05-10 03:19:40.658211 forevd-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1107 1970-01-01 00:00:00.000000 forevd-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-12 13:20:03.959275 forevd-0.1.2/LICENSE
+-rw-r--r--   0        0        0      832 2023-05-12 13:20:03.959275 forevd-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2023-05-12 13:20:03.959275 forevd-0.1.2/forevd/__init__.py
+-rw-r--r--   0        0        0     4390 2023-05-12 13:20:03.959275 forevd-0.1.2/forevd/__main__.py
+-rw-r--r--   0        0        0     1498 2023-05-12 13:20:03.959275 forevd-0.1.2/forevd/apache/__init__.py
+-rw-r--r--   0        0        0     3428 2023-05-12 13:20:03.959275 forevd-0.1.2/forevd/apache/httpd.conf
+-rw-r--r--   0        0        0        0 2023-05-12 13:20:03.959275 forevd-0.1.2/forevd/resources/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-12 13:20:03.959275 forevd-0.1.2/forevd/resources/logging/__init__.py
+-rw-r--r--   0        0        0      387 2023-05-12 13:20:03.959275 forevd-0.1.2/forevd/resources/logging/cli.conf
+-rw-r--r--   0        0        0      844 2023-05-12 13:20:03.963276 forevd-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1453 1970-01-01 00:00:00.000000 forevd-0.1.2/PKG-INFO
```

### Comparing `forevd-0.1.1/LICENSE` & `forevd-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `forevd-0.1.1/forevd/__main__.py` & `forevd-0.1.2/forevd/__main__.py`

 * *Files identical despite different names*

### Comparing `forevd-0.1.1/forevd/apache/__init__.py` & `forevd-0.1.2/forevd/apache/__init__.py`

 * *Files identical despite different names*

### Comparing `forevd-0.1.1/forevd/apache/httpd.conf` & `forevd-0.1.2/forevd/apache/httpd.conf`

 * *Files 4% similar despite different names*

```diff
@@ -11,36 +11,40 @@
 
 LoadModule proxy_module modules/mod_proxy.so
 LoadModule proxy_http_module modules/mod_proxy_http.so
 
 {% if cert -%}
 LoadModule ssl_module modules/mod_ssl.so
 LoadModule socache_shmcb_module modules/mod_socache_shmcb.so
-{% endif -%}
+{% endif %}
 {% if oidc -%}
 LoadModule authz_user_module modules/mod_authz_user.so
 LoadModule auth_openidc_module modules/mod_auth_openidc.so
-{% endif -%}
+{% endif %}
 
 ServerName {{ server_name }}
-#ServerAdmin erick@jeb.ca
+Listen {{ listen }}
 
-ServerTokens Prod
 UseCanonicalName On
-TraceEnable Off
 
 Timeout 10
 MaxRequestWorkers 100
 
-Listen {{ listen }}
+{% if debug %}
+LogLevel debug
+TraceEnable Off
+{% else %}
+LogLevel info
+{% endif %}
 
-LogLevel {% if debug %}debug{% else %}info{% endif %}
 ErrorLog {{ err_log }}
 CustomLog {{ access_log }} common
 
+Mutex posixem
+
 {% raw %}
 ErrorLogFormat "[%{cu}t] [%-m:%-l] %-a %-L %M"
 LogFormat "%h %l %u [%{%Y-%m-%d %H:%M:%S}t.%{usec_frac}t] \"%r\" %>s %b \ \"%{Referer}i\" \"%{User-Agent}i\"" combined
 {% endraw %}
 
 {% if cert -%}
 SSLEngine on
@@ -72,15 +76,15 @@
 {% if oidc["provider_token_auth_endpoint"] -%}
 OIDCProviderTokenEndpointAuth {{ oidc["provider_token_auth_endpoint"] }}
 {% endif -%}
 {% if oidc["provider_user_info_endpoint"] -%}
 OIDCProviderUserInfoEndpoint {{ oidc["provider_user_info_endpoint"] }}
 {% endif -%}
 # OIDCRedirectURI is a vanity URL that must point to a path protected by this module but must NOT point to any content
-OIDCRedirectURI https://{{ server_name }}/secure/redirect_uri
+OIDCRedirectURI {% if oidc["redirect_uri"] %}{{ oidc["redirect_uri"] }}{% else %}https://{{ server_name }}/secure/redirect_uri{% endif %}
 
 OIDCCryptoPassphrase {% if oidc["crypto_passphrase"] %}{{ oidc["crypto_passphrase"] }}{% else %}"exec:/bin/bash -c \"head /dev/urandom | tr -dc A-Za-z0-9 | head -c 32\""{% endif %}
 {% endif -%}
 
 {% for location in locations %}
 <Location "{{ location }}">
     ProxyPass {{ locations[location]["backend"] }}/
```

### Comparing `forevd-0.1.1/pyproject.toml` & `forevd-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "forevd"
-version = "0.1.1"
+version = "0.1.2"
 description = "Forward and reverse proxy using nginx or apache"
 authors = ["Erick Bourgeois <erick@jeb.ca>"]
 license = "LICENSE"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

