# Comparing `tmp/twitwi-0.9.2.tar.gz` & `tmp/twitwi-0.9.3a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/twitwi-0.9.2.tar", last modified: Wed Sep 15 09:45:36 2021, max compression
+gzip compressed data, was "twitwi-0.9.3a1.tar", last modified: Thu Jan 27 11:19:58 2022, max compression
```

## Comparing `twitwi-0.9.2.tar` & `twitwi-0.9.3a1.tar`

### file list

```diff
@@ -1,20 +1,22 @@
-drwxrwxr-x   0 yomguithereal  (1000) yomguithereal  (1000)        0 2021-09-15 09:45:36.000000 twitwi-0.9.2/
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      820 2021-09-15 09:45:03.000000 twitwi-0.9.2/setup.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     5090 2021-09-15 09:45:36.000000 twitwi-0.9.2/PKG-INFO
-drwxrwxr-x   0 yomguithereal  (1000) yomguithereal  (1000)        0 2021-09-15 09:45:36.000000 twitwi-0.9.2/twitwi.egg-info/
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)        1 2021-09-15 09:45:36.000000 twitwi-0.9.2/twitwi.egg-info/zip-safe
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)        1 2021-09-15 09:45:36.000000 twitwi-0.9.2/twitwi.egg-info/dependency_links.txt
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     5090 2021-09-15 09:45:36.000000 twitwi-0.9.2/twitwi.egg-info/PKG-INFO
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)        7 2021-09-15 09:45:36.000000 twitwi-0.9.2/twitwi.egg-info/top_level.txt
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      336 2021-09-15 09:45:36.000000 twitwi-0.9.2/twitwi.egg-info/SOURCES.txt
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)       42 2021-09-15 09:45:36.000000 twitwi-0.9.2/twitwi.egg-info/requires.txt
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     3646 2021-04-22 12:15:48.000000 twitwi-0.9.2/README.md
-drwxrwxr-x   0 yomguithereal  (1000) yomguithereal  (1000)        0 2021-09-15 09:45:36.000000 twitwi-0.9.2/twitwi/
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     3872 2021-03-10 14:04:57.000000 twitwi-0.9.2/twitwi/client_wrapper.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     1726 2021-06-16 15:47:53.000000 twitwi-0.9.2/twitwi/utils.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)    24268 2021-06-16 15:47:53.000000 twitwi-0.9.2/twitwi/normalizers.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)     2813 2021-06-16 15:47:53.000000 twitwi-0.9.2/twitwi/formatters.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)    10716 2021-06-16 15:47:53.000000 twitwi-0.9.2/twitwi/constants.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      622 2021-06-16 15:47:53.000000 twitwi-0.9.2/twitwi/__init__.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)      331 2021-02-11 13:09:21.000000 twitwi-0.9.2/twitwi/exceptions.py
--rw-rw-r--   0 yomguithereal  (1000) yomguithereal  (1000)       38 2021-09-15 09:45:36.000000 twitwi-0.9.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-27 11:19:58.232173 twitwi-0.9.3a1/
+-rw-r--r--   0 runner    (1001) docker     (121)     1099 2022-01-27 11:19:45.000000 twitwi-0.9.3a1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     4091 2022-01-27 11:19:58.232173 twitwi-0.9.3a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3670 2022-01-27 11:19:45.000000 twitwi-0.9.3a1/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-01-27 11:19:58.232173 twitwi-0.9.3a1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      826 2022-01-27 11:19:45.000000 twitwi-0.9.3a1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-27 11:19:58.232173 twitwi-0.9.3a1/twitwi/
+-rw-r--r--   0 runner    (1001) docker     (121)      622 2022-01-27 11:19:45.000000 twitwi-0.9.3a1/twitwi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4523 2022-01-27 11:19:45.000000 twitwi-0.9.3a1/twitwi/client_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10716 2022-01-27 11:19:45.000000 twitwi-0.9.3a1/twitwi/constants.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7486 2022-01-27 11:19:45.000000 twitwi-0.9.3a1/twitwi/constants_api_v2.py
+-rw-r--r--   0 runner    (1001) docker     (121)      378 2022-01-27 11:19:45.000000 twitwi-0.9.3a1/twitwi/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2813 2022-01-27 11:19:45.000000 twitwi-0.9.3a1/twitwi/formatters.py
+-rw-r--r--   0 runner    (1001) docker     (121)    25367 2022-01-27 11:19:45.000000 twitwi-0.9.3a1/twitwi/normalizers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1581 2022-01-27 11:19:45.000000 twitwi-0.9.3a1/twitwi/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-27 11:19:58.232173 twitwi-0.9.3a1/twitwi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     4091 2022-01-27 11:19:58.000000 twitwi-0.9.3a1/twitwi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      375 2022-01-27 11:19:58.000000 twitwi-0.9.3a1/twitwi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-27 11:19:58.000000 twitwi-0.9.3a1/twitwi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       41 2022-01-27 11:19:58.000000 twitwi-0.9.3a1/twitwi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        7 2022-01-27 11:19:58.000000 twitwi-0.9.3a1/twitwi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-27 11:19:58.000000 twitwi-0.9.3a1/twitwi.egg-info/zip-safe
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `twitwi-0.9.2/setup.py` & `twitwi-0.9.3a1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from setuptools import setup, find_packages
 
 with open('./README.md', 'r') as f:
     long_description = f.read()
 
 setup(name='twitwi',
-      version='0.9.2',
+      version='0.9.3-alpha1',
       description='A collection of Twitter-related helper functions for python.',
       long_description=long_description,
       long_description_content_type='text/markdown',
       url='http://github.com/medialab/twitwi',
       license='MIT',
       author='Béatrice Mazoyer, Guillaume Plique, Benjamin Ooghe-Tabanou',
       author_email='guillaume.plique@sciencespo.fr',
       keywords='twitter',
       python_requires='>=3.4',
       packages=find_packages(exclude=['scripts', 'test']),
       package_data={'docs': ['README.md']},
       install_requires=[
         'pytz>=2019.3',
-        'twitter>=1.19.3',
+        'twitter==2.0a0',
         'ural>=0.31.1'
       ],
       zip_safe=True)
```

### Comparing `twitwi-0.9.2/README.md` & `twitwi-0.9.3a1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,22 @@
-[![Build Status](https://travis-ci.org/medialab/twitwi.svg)](https://travis-ci.org/medialab/twitwi)
+Metadata-Version: 2.1
+Name: twitwi
+Version: 0.9.3a1
+Summary: A collection of Twitter-related helper functions for python.
+Home-page: http://github.com/medialab/twitwi
+Author: Béatrice Mazoyer, Guillaume Plique, Benjamin Ooghe-Tabanou
+Author-email: guillaume.plique@sciencespo.fr
+License: MIT
+Keywords: twitter
+Platform: UNKNOWN
+Requires-Python: >=3.4
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+[![Build Status](https://github.com/medialab/twitwi/workflows/Tests/badge.svg)](https://github.com/medialab/twitwi/actions)
 
 # Twitwi
 
 A collection of Twitter-related helper functions for python.
 
 ## Installation
 
@@ -124,7 +138,9 @@
 w = csv.writer(f)
 w.writerow(USER_FIELDS)
 
 # Using csv.DictWriter
 w = csv.DictWriter(f, fieldnames=USER_FIELDS)
 w.writeheader()
 ```
+
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `twitwi-0.9.2/twitwi/client_wrapper.py` & `twitwi-0.9.3a1/twitwi/client_wrapper.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,17 +4,18 @@
 #
 # Wrapper for the `twitter` library API client able to rotate the two possible
 # endpoints to maximize throughput.
 #
 import json
 from time import sleep, time
 from operator import itemgetter
-from twitter import Twitter, OAuth, OAuth2, TwitterHTTPError
+from twitter import Twitter, OAuth, OAuth2, TwitterHTTPError, Twitter2
 
-from twitwi.exceptions import TwitterWrapperMaxAttemptsExceeded
+from twitwi.exceptions import TwitterWrapperMaxAttemptsExceeded, ApiVersionError
+from twitwi.constants_api_v2 import APP_ONLY_ROUTES
 
 DEFAULT_MAX_ATTEMPTS = 5
 
 # Established from: https://developer.twitter.com/en/support/twitter-api/error-troubleshooting
 NO_RETRY_STATUSES = set([
     400,
     401,
@@ -25,15 +26,22 @@
     422
 ])
 
 
 class TwitterWrapper(object):
 
     def __init__(self, token, token_secret, consumer_key, consumer_secret,
-                 listener=None):
+                 listener=None, api_version='1.1'):
+
+        if not isinstance(api_version, str):
+            api_version = str(api_version)
+
+        if api_version not in ['1.1', '2']:
+            raise ApiVersionError('API version can only be \'1.1\' or \'2\'.')
+
         self.oauth = OAuth(
             token,
             token_secret,
             consumer_key,
             consumer_secret
         )
 
@@ -46,21 +54,32 @@
 
         bearer_token = json.loads(
             bearer_token_client.oauth2.token(grant_type='client_credentials')
         )['access_token']
 
         self.oauth2 = OAuth2(bearer_token=bearer_token)
 
-        self.endpoints = {
-            'user': Twitter(auth=self.oauth),
-            'app': Twitter(auth=self.oauth2)
-        }
-
-        self.waits = {}
         self.auth = {}
+        self.waits = {}
+
+        if api_version == '2':
+            self.endpoints = {
+                'user': Twitter2(auth=self.oauth),
+                'app': Twitter2(auth=self.oauth2)
+            }
+
+            for route in APP_ONLY_ROUTES:
+                self.auth[route] = 'app'
+                self.waits[route] = {'app': 0}
+
+        else:
+            self.endpoints = {
+                'user': Twitter(auth=self.oauth),
+                'app': Twitter(auth=self.oauth2)
+            }
 
         self.listener = listener
 
     def call(self, route, max_attempts=DEFAULT_MAX_ATTEMPTS, **kwargs):
         attempts = 0
 
         if not isinstance(route, list):
```

### Comparing `twitwi-0.9.2/twitwi/utils.py` & `twitwi-0.9.3a1/twitwi/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -48,15 +48,11 @@
     if not isinstance(payload, dict):
         return False
 
     if 'data' not in payload or not isinstance(payload['data'], list):
         return False
 
     # NOTE: not sure it cannot be absent altogether
-    if 'meta' not in payload or not isinstance(payload['meta'], dict):
-        return False
-
-    # NOTE: not sure it cannot be absent altogether
     if 'includes' not in payload or not isinstance(payload['includes'], dict):
         return False
 
     return True
```

### Comparing `twitwi-0.9.2/twitwi/normalizers.py` & `twitwi-0.9.3a1/twitwi/normalizers.py`

 * *Files 4% similar despite different names*

```diff
@@ -376,21 +376,23 @@
 
 
 def resolve_user_entities(user):
     if 'entities' in user:
         for k in user['entities']:
             if 'urls' in user['entities'][k]:
                 for url in user['entities'][k]['urls']:
+                    if 'expanded_url' not in url:
+                        continue
                     if not url['expanded_url']:
                         continue
                     if k in user:
                         user[k] = user[k].replace(url['url'], url['expanded_url'])
 
 
-def normalize_user(user, locale=None, pure=True):
+def normalize_user(user, locale=None, pure=True, v2=False):
     """
     Function "normalizing" a user as returned by Twitter's API in order to
     cleanup and optimize some fields.
 
     Note that this function mutates the argument to work.
 
     Args:
@@ -405,37 +407,45 @@
     """
 
     if pure:
         user = deepcopy(user)
 
     resolve_user_entities(user)
 
-    timestamp_utc, local_time = get_dates(user['created_at'], locale)
+    timestamp_utc, local_time = get_dates(user['created_at'], locale, v2)
+
+    if v2 and 'withheld' in user:
+        withheld = user['withheld']
+        withheld_in_countries = withheld.get('country_codes', [])
+        withheld_scope = withheld.get('withheld_scope', '')
+    else:
+        withheld_in_countries = []
+        withheld_scope = ''
 
     normalized_user = {
-        'id': user['id_str'],
-        'screen_name': user['screen_name'],
+        'id': user['id_str'] if not v2 else user['id'],
+        'screen_name': user['screen_name'] if not v2 else user['username'],
         'name': user['name'],
         'description': user['description'],
         'url': user['url'],
         'timestamp_utc': timestamp_utc,
         'local_time': local_time,
-        'location': user.get('location'),
+        'location': user.get('location', ''),
         'verified': user.get('verified'),
         'protected': user.get('protected'),
-        'tweets': user['statuses_count'],
-        'followers': user['followers_count'],
-        'friends': user['friends_count'],
-        'likes': user['favourites_count'],
-        'lists': user['listed_count'],
-        'image': user.get('profile_image_url_https'),
-        'default_profile': user.get('default_profile'),
-        'default_profile_image': user.get('default_profile_image'),
-        'witheld_in_countries': user.get('witheld_in_countries', []),
-        'witheld_scope': user.get('witheld_scope')
+        'tweets': user['statuses_count'] if not v2 else user['public_metrics']['tweet_count'],
+        'followers': user['followers_count'] if not v2 else user['public_metrics']['followers_count'],
+        'friends': user['friends_count'] if not v2 else user['public_metrics']['following_count'],
+        'likes': user['favourites_count'] if not v2 else 0,
+        'lists': user['listed_count'] if not v2 else user['public_metrics']['listed_count'],
+        'image': user.get('profile_image_url_https') if not v2 else user.get('profile_image_url'),
+        'default_profile': user.get('default_profile', ''),
+        'default_profile_image': user.get('default_profile_image', ''),
+        'witheld_in_countries': user.get('witheld_in_countries', []) if not v2 else withheld_in_countries,
+        'witheld_scope': user.get('witheld_scope') if not v2 else withheld_scope
     }
 
     return normalized_user
 
 
 def includes_index(payload, key, index_key='id'):
     return {item[index_key]: item for item in payload['includes'].get(key, [])}
@@ -464,18 +474,21 @@
     referenced_tweets = tweet.get('referenced_tweets', [])
 
     hashtags = set()
 
     for hashtag in entities.get('hashtags', []):
         hashtags.add(hashtag['tag'])
 
-    mentions = set()
+    mentions = {}
 
     for mention in entities.get('mentions', []):
-        mentions.add(mention['username'])
+        if 'id' in mention:
+            mentions[mention['username']] = mention['id']
+        else:
+            mentions[mention['username']] = users_by_screen_name[mention['username']]['id']
 
     place_info = {}
 
     if 'geo' in tweet:
         geo_data = tweet['geo']
 
         if 'coordinates' in geo_data:
@@ -483,15 +496,15 @@
 
             if point['type'] == 'Point':
                 lng, lat = point['coordinates']
                 place_info['lng'] = lng
                 place_info['lat'] = lat
 
         if 'place_id' in geo_data:
-            place_data = places_by_id[geo_data['place_id']]
+            place_data = places_by_id.get(geo_data['place_id'], {})
 
             if 'country_code' in place_data:
                 place_info['place_country_code'] = place_data['country_code']
 
             if 'full_name' in place_data:
                 place_info['place_name'] = place_data['full_name']
 
@@ -507,18 +520,21 @@
     # References
     refs = {t['type']: t['id'] for t in referenced_tweets}
 
     # Reply
     reply_info = {}
 
     if 'replied_to' in refs:
-        reply = tweets_by_id[refs['replied_to']]
-        reply_info['to_username'] = users_by_id[reply['author_id']]['username']
-        reply_info['to_userid'] = reply['author_id']
-        reply_info['to_tweetid'] = reply['id']
+        reply = tweets_by_id.get(refs['replied_to'], {})
+        if 'author_id' in reply:
+            reply_info['to_username'] = users_by_id[reply['author_id']]['username']
+        else:
+            reply_info['to_username'] = ''
+        reply_info['to_userid'] = reply.get('author_id', '')
+        reply_info['to_tweetid'] = reply.get('id', '')
 
     # Retweet
     retweet_info = {}
     normalized_retweet = None
 
     if 'retweeted' in refs:
         retweet_info['retweeted_id'] = refs['retweeted']
@@ -607,31 +623,33 @@
         source_id = refs.get('retweeted_id', tweet['id'])
 
         for media_key in tweet['attachments']['media_keys']:
             if media_key in media_by_key:
                 media_data = media_by_key[media_key]
 
                 medias.append((
-                    media_data['url'],
-                    '%s_%s' % (source_id, extract_media_name_from_url(media_data['url'])),
+                    media_data.get('url', ''),
+                    '%s_%s' % (source_id, extract_media_name_from_url(media_data.get('url', ''))),
                     media_data['type']
                 ))
 
     if collection_source is None:
         collection_source = tweet.get('collection_source')
 
+    sorted_mentions = sorted(mentions.keys())
+
     normalized_tweet = {
         'id': tweet['id'],
         'local_time': local_time,
         'timestamp_utc': timestamp_utc,
         'text': unescape(text),
         'url': format_tweet_url(user['username'], tweet['id']),
         'hashtags': sorted(hashtags),
-        'mentioned_names': sorted(mentions),
-        'mentioned_ids': sorted(users_by_screen_name[name]['id'] for name in mentions),
+        'mentioned_names': sorted_mentions,
+        'mentioned_ids': [mentions[k] for k in sorted_mentions],
         'collection_time': get_collection_time(),
         'user_id': user['id'],
         'user_screen_name': user['username'],
         'user_name': user['name'],
         'user_image': user['profile_image_url'],
         'user_url': user_url or None,
         'user_location': user.get('location'),
```

### Comparing `twitwi-0.9.2/twitwi/formatters.py` & `twitwi-0.9.3a1/twitwi/formatters.py`

 * *Files identical despite different names*

### Comparing `twitwi-0.9.2/twitwi/constants.py` & `twitwi-0.9.3a1/twitwi/constants.py`

 * *Files identical despite different names*

### Comparing `twitwi-0.9.2/twitwi/__init__.py` & `twitwi-0.9.3a1/twitwi/__init__.py`

 * *Files identical despite different names*

