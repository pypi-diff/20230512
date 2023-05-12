# Comparing `tmp/ritetag-1.3.2.tar.gz` & `tmp/ritetag-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ritetag-1.3.2.tar", last modified: Mon May 24 14:24:38 2021, max compression
+gzip compressed data, was "ritetag-1.3.3.tar", last modified: Fri May 12 12:29:01 2023, max compression
```

## Comparing `ritetag-1.3.2.tar` & `ritetag-1.3.3.tar`

### file list

```diff
@@ -1,24 +1,26 @@
-drwxrwxr-x   0 pavelhouzva  (1000) pavelhouzva  (1000)        0 2021-05-24 14:24:38.408764 ritetag-1.3.2/
--rw-rw-r--   0 pavelhouzva  (1000) pavelhouzva  (1000)      553 2021-05-12 11:50:43.000000 ritetag-1.3.2/LICENCE
--rw-rw-r--   0 pavelhouzva  (1000) pavelhouzva  (1000)     5668 2021-05-24 14:24:38.408764 ritetag-1.3.2/PKG-INFO
--rw-rw-r--   0 pavelhouzva  (1000) pavelhouzva  (1000)     3601 2021-05-19 14:26:06.000000 ritetag-1.3.2/README.md
-drwxrwxr-x   0 pavelhouzva  (1000) pavelhouzva  (1000)        0 2021-05-24 14:24:38.404765 ritetag-1.3.2/bin/
--rwxrwxr-x   0 pavelhouzva  (1000) pavelhouzva  (1000)       53 2021-05-12 11:50:43.000000 ritetag-1.3.2/bin/ritetag-api
-drwxrwxr-x   0 pavelhouzva  (1000) pavelhouzva  (1000)        0 2021-05-24 14:24:38.407765 ritetag-1.3.2/ritetag/
--rw-rw-r--   0 pavelhouzva  (1000) pavelhouzva  (1000)      193 2021-05-12 11:50:43.000000 ritetag-1.3.2/ritetag/__init__.py
--rw-rw-r--   0 pavelhouzva  (1000) pavelhouzva  (1000)      279 2021-05-24 14:24:03.000000 ritetag-1.3.2/ritetag/__version__.py
--rw-rw-r--   0 pavelhouzva  (1000) pavelhouzva  (1000)    18945 2021-05-19 13:22:43.000000 ritetag-1.3.2/ritetag/api.py
--rw-rw-r--   0 pavelhouzva  (1000) pavelhouzva  (1000)     2439 2021-05-12 11:50:43.000000 ritetag-1.3.2/ritetag/builders.py
--rw-rw-r--   0 pavelhouzva  (1000) pavelhouzva  (1000)     5863 2021-05-19 14:21:34.000000 ritetag-1.3.2/ritetag/console.py
--rw-rw-r--   0 pavelhouzva  (1000) pavelhouzva  (1000)      434 2021-05-12 11:50:43.000000 ritetag-1.3.2/ritetag/decorators.py
--rw-rw-r--   0 pavelhouzva  (1000) pavelhouzva  (1000)    30706 2021-05-12 11:50:43.000000 ritetag-1.3.2/ritetag/enums.py
--rw-rw-r--   0 pavelhouzva  (1000) pavelhouzva  (1000)      101 2021-05-12 11:50:43.000000 ritetag-1.3.2/ritetag/exceptions.py
--rw-rw-r--   0 pavelhouzva  (1000) pavelhouzva  (1000)      324 2021-05-12 11:50:43.000000 ritetag-1.3.2/ritetag/others.py
--rw-rw-r--   0 pavelhouzva  (1000) pavelhouzva  (1000)    11310 2021-05-24 14:23:41.000000 ritetag-1.3.2/ritetag/response.py
-drwxrwxr-x   0 pavelhouzva  (1000) pavelhouzva  (1000)        0 2021-05-24 14:24:38.407765 ritetag-1.3.2/ritetag.egg-info/
--rw-rw-r--   0 pavelhouzva  (1000) pavelhouzva  (1000)     5668 2021-05-24 14:24:38.000000 ritetag-1.3.2/ritetag.egg-info/PKG-INFO
--rw-rw-r--   0 pavelhouzva  (1000) pavelhouzva  (1000)      362 2021-05-24 14:24:38.000000 ritetag-1.3.2/ritetag.egg-info/SOURCES.txt
--rw-rw-r--   0 pavelhouzva  (1000) pavelhouzva  (1000)        1 2021-05-24 14:24:38.000000 ritetag-1.3.2/ritetag.egg-info/dependency_links.txt
--rw-rw-r--   0 pavelhouzva  (1000) pavelhouzva  (1000)        8 2021-05-24 14:24:38.000000 ritetag-1.3.2/ritetag.egg-info/top_level.txt
--rw-rw-r--   0 pavelhouzva  (1000) pavelhouzva  (1000)       38 2021-05-24 14:24:38.408764 ritetag-1.3.2/setup.cfg
--rw-rw-r--   0 pavelhouzva  (1000) pavelhouzva  (1000)     2055 2021-05-24 14:10:03.000000 ritetag-1.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-12 12:29:01.957950 ritetag-1.3.3/
+-rw-rw-rw-   0        0        0      565 2022-02-08 11:16:15.000000 ritetag-1.3.3/LICENCE
+-rw-rw-rw-   0        0        0     4583 2023-05-12 12:29:01.956950 ritetag-1.3.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3756 2022-02-08 11:16:15.000000 ritetag-1.3.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-12 12:29:01.926015 ritetag-1.3.3/bin/
+-rw-rw-rw-   0        0        0       58 2022-02-08 11:16:15.000000 ritetag-1.3.3/bin/ritetag-api
+drwxrwxrwx   0        0        0        0 2023-05-12 12:29:01.941475 ritetag-1.3.3/ritetag/
+-rw-rw-rw-   0        0        0      199 2022-02-08 11:16:15.000000 ritetag-1.3.3/ritetag/__init__.py
+-rw-rw-rw-   0        0        0      286 2023-05-12 12:24:35.000000 ritetag-1.3.3/ritetag/__version__.py
+-rw-rw-rw-   0        0        0    19600 2023-05-12 12:15:54.000000 ritetag-1.3.3/ritetag/api.py
+-rw-rw-rw-   0        0        0     2525 2022-02-08 11:16:15.000000 ritetag-1.3.3/ritetag/builders.py
+-rw-rw-rw-   0        0        0     6319 2023-05-12 12:21:52.000000 ritetag-1.3.3/ritetag/console.py
+-rw-rw-rw-   0        0        0      455 2022-02-08 11:16:15.000000 ritetag-1.3.3/ritetag/decorators.py
+-rw-rw-rw-   0        0        0    31746 2022-02-08 11:16:15.000000 ritetag-1.3.3/ritetag/enums.py
+-rw-rw-rw-   0        0        0      107 2022-02-08 11:16:15.000000 ritetag-1.3.3/ritetag/exceptions.py
+-rw-rw-rw-   0        0        0      338 2022-02-08 11:16:15.000000 ritetag-1.3.3/ritetag/others.py
+-rw-rw-rw-   0        0        0    11741 2022-02-08 11:16:15.000000 ritetag-1.3.3/ritetag/response.py
+drwxrwxrwx   0        0        0        0 2023-05-12 12:29:01.953570 ritetag-1.3.3/ritetag.egg-info/
+-rw-rw-rw-   0        0        0     4583 2023-05-12 12:29:01.000000 ritetag-1.3.3/ritetag.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      380 2023-05-12 12:29:01.000000 ritetag-1.3.3/ritetag.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-12 12:29:01.000000 ritetag-1.3.3/ritetag.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-05-12 12:29:01.000000 ritetag-1.3.3/ritetag.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-12 12:29:01.957950 ritetag-1.3.3/setup.cfg
+-rw-rw-rw-   0        0        0     2129 2022-02-08 11:16:15.000000 ritetag-1.3.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-12 12:29:01.955970 ritetag-1.3.3/tests/
+-rw-rw-rw-   0        0        0     1490 2022-02-08 11:16:15.000000 ritetag-1.3.3/tests/test_api.py
```

### Comparing `ritetag-1.3.2/README.md` & `ritetag-1.3.3/README.md`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,156 +1,156 @@
-# RiteTag API client
-
-Python API client
-
-## Documentation
-
-[API Documentation](https://documenter.getpostman.com/view/2010712/SzS7Qku5?version=latest#3a6540d0-61e3-4333-b353-f1072621a23b)
-
-## Installation
-
-`pip install --user ritetag`
-
-
-## Usage
-
-### In The Code
-```python
-from ritetag import RiteTagApi
-
-access_token = 'token'
-client = RiteTagApi(access_token)
-
-def limit_80_percentage_reached(limit):
-    message = 'Used {}% of API credits. The limit resets on {}'.format(limit.usage, limit.reset)
-    print(message)
-
-# The callback function is triggered when 80% of the API limit is reached
-client.on_limit(80, limit_80_percentage_reached)
-
-stats = client.hashtag_stats(['jobs', 'hello'])
-
-for data in stats:
-    print('#{}: {} tweets per hour'.format(data.hashtag, data.tweets))
-
-```
-
-output:
-
-```
-#jobs: 642 tweets per hour
-#hello: 25 tweets per hour
-```
-
-### In The Console
-
-```
-ritetag-api -h
-usage: ritetag-api [-h] [-t ACCESS_TOKEN] [-m MAX_HASHTAGS] [-p {auto,end}]
-                   [-f FILENAME] [-ci CTA_ID]
-                   {hashtag_stats,auto_hashtags,hashtag_suggestions,hashtag_history,emojis_suggestion,auto_emojify,company_logo,list_of_cta,shorten_link}
-                   [hashtags [hashtags ...]]
-
-RiteTag API console client.
-
-positional arguments:
-  {hashtag_stats,auto_hashtags,hashtag_suggestions,hashtag_history,emojis_suggestion,auto_emojify,company_logo,list_of_cta,shorten_link}
-                        action
-  hashtags              hashtags
-
-optional arguments:
-  -h, --help            show this help message and exit
-  -t ACCESS_TOKEN, --access_token ACCESS_TOKEN
-                        access token
-  -m MAX_HASHTAGS, --max_hashtags MAX_HASHTAGS
-  -p {auto,end}, --hashtag_position {auto,end}
-  -f FILENAME, --filename FILENAME
-  -ci CTA_ID, --cta_id CTA_ID
-```
-
-
-```
-export ACCESS_TOKEN={access_token}
-ritetag-api hashtag_stats jobs hello
-```
-
-or
-
-`ritetag-api -t {access_token} hashtag_stats jobs hello`
-
-output:
-
-```
-Used 19.89% of API credits. The limit resets on 2020-04-01.
-==== Stats of #jobs ====
-tweets: 642
-retweets: 62
-exposure: 1984429
-mentions: 9.03427%
-links: 35.04673%
-images: 35.04673%
-color: HOT_NOW
-media count: 3490073
-
-==== Stats of #hello ====
-tweets: 25
-retweets: 4
-exposure: 32567
-mentions: 32.0%
-links: 32.0%
-images: 32.0%
-color: HOT_NOW
-media count: 18896544
-
-```
-### Company logo API (console)
-
-##### Example 1 - google.com
-
-```shell
-# Company logo example
-ritetag-api -t {token} company_logo google.com
-```
-
-```
-Looking for logo - google.com
-Used 0.14% of API credits. The limit resets on 2021-06-01.
-Downloading logo - google.com
-Image is saved google_com.svg - google.com
-Downloading square logo - google.com
-Image is saved google.com - google_com_square.png
-
-```
-
-##### Example 2 - notfound.test with Generate fallback
-
-```shell
-# Company logo example
-ritetag-api -t {token} company_logo -g 1 company_logo notfound.test
-```
-
-```
-Looking for logo - notfound.test
-Used 0.14% of API credits. The limit resets on 2021-06-01.
-Logo is generated.
-Downloading logo - notfound.test
-Image is saved notfound_test.png - notfound.test
-Downloading square logo - notfound.test
-Image is saved notfound.test - notfound_test_square.png
-
-```
-
-##### Example 3 -  notfound.test without Generate fallback
-
-```shell
-# Company logo example
-ritetag-api -t {token} company_logo -g 0 company_logo notfound.test
-```
-
-```
-Looking for logo - notfound.test
-Used 0.14% of API credits. The limit resets on 2021-06-01.
-Downloading logo - notfound.test
-Error Logo not found - notfound.test
-Downloading square logo - notfound.test
-Error Logo not found - notfound.test
+# RiteTag API client
+
+Python API client
+
+## Documentation
+
+[API Documentation](https://documenter.getpostman.com/view/2010712/SzS7Qku5?version=latest#3a6540d0-61e3-4333-b353-f1072621a23b)
+
+## Installation
+
+`pip install --user ritetag`
+
+
+## Usage
+
+### In The Code
+```python
+from ritetag import RiteTagApi
+
+access_token = 'token'
+client = RiteTagApi(access_token)
+
+def limit_80_percentage_reached(limit):
+    message = 'Used {}% of API credits. The limit resets on {}'.format(limit.usage, limit.reset)
+    print(message)
+
+# The callback function is triggered when 80% of the API limit is reached
+client.on_limit(80, limit_80_percentage_reached)
+
+stats = client.hashtag_stats(['jobs', 'hello'])
+
+for data in stats:
+    print('#{}: {} tweets per hour'.format(data.hashtag, data.tweets))
+
+```
+
+output:
+
+```
+#jobs: 642 tweets per hour
+#hello: 25 tweets per hour
+```
+
+### In The Console
+
+```
+ritetag-api -h
+usage: ritetag-api [-h] [-t ACCESS_TOKEN] [-m MAX_HASHTAGS] [-p {auto,end}]
+                   [-f FILENAME] [-ci CTA_ID]
+                   {hashtag_stats,auto_hashtags,hashtag_suggestions,hashtag_history,emojis_suggestion,auto_emojify,company_logo,list_of_cta,shorten_link}
+                   [hashtags [hashtags ...]]
+
+RiteTag API console client.
+
+positional arguments:
+  {hashtag_stats,auto_hashtags,hashtag_suggestions,hashtag_history,emojis_suggestion,auto_emojify,company_logo,list_of_cta,shorten_link}
+                        action
+  hashtags              hashtags
+
+optional arguments:
+  -h, --help            show this help message and exit
+  -t ACCESS_TOKEN, --access_token ACCESS_TOKEN
+                        access token
+  -m MAX_HASHTAGS, --max_hashtags MAX_HASHTAGS
+  -p {auto,end}, --hashtag_position {auto,end}
+  -f FILENAME, --filename FILENAME
+  -ci CTA_ID, --cta_id CTA_ID
+```
+
+
+```
+export ACCESS_TOKEN={access_token}
+ritetag-api hashtag_stats jobs hello
+```
+
+or
+
+`ritetag-api -t {access_token} hashtag_stats jobs hello`
+
+output:
+
+```
+Used 19.89% of API credits. The limit resets on 2020-04-01.
+==== Stats of #jobs ====
+tweets: 642
+retweets: 62
+exposure: 1984429
+mentions: 9.03427%
+links: 35.04673%
+images: 35.04673%
+color: HOT_NOW
+media count: 3490073
+
+==== Stats of #hello ====
+tweets: 25
+retweets: 4
+exposure: 32567
+mentions: 32.0%
+links: 32.0%
+images: 32.0%
+color: HOT_NOW
+media count: 18896544
+
+```
+### Company logo API (console)
+
+##### Example 1 - google.com
+
+```shell
+# Company logo example
+ritetag-api -t {token} company_logo google.com
+```
+
+```
+Looking for logo - google.com
+Used 0.14% of API credits. The limit resets on 2021-06-01.
+Downloading logo - google.com
+Image is saved google_com.svg - google.com
+Downloading square logo - google.com
+Image is saved google.com - google_com_square.png
+
+```
+
+##### Example 2 - notfound.test with Generate fallback
+
+```shell
+# Company logo example
+ritetag-api -t {token} company_logo -g 1 company_logo notfound.test
+```
+
+```
+Looking for logo - notfound.test
+Used 0.14% of API credits. The limit resets on 2021-06-01.
+Logo is generated.
+Downloading logo - notfound.test
+Image is saved notfound_test.png - notfound.test
+Downloading square logo - notfound.test
+Image is saved notfound.test - notfound_test_square.png
+
+```
+
+##### Example 3 -  notfound.test without Generate fallback
+
+```shell
+# Company logo example
+ritetag-api -t {token} company_logo -g 0 company_logo notfound.test
+```
+
+```
+Looking for logo - notfound.test
+Used 0.14% of API credits. The limit resets on 2021-06-01.
+Downloading logo - notfound.test
+Error Logo not found - notfound.test
+Downloading square logo - notfound.test
+Error Logo not found - notfound.test
 ```
```

### Comparing `ritetag-1.3.2/ritetag/console.py` & `ritetag-1.3.3/ritetag/console.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,171 +1,174 @@
-import argparse
-import os
-from .api import *
-
-current_directory = os.getcwd()
-access_token = os.getenv('ACCESS_TOKEN', None)
-require_token = access_token is None
-
-
-class Action(Enum):
-    hashtag_stats = 'hashtag_stats'
-    auto_hashtags = 'auto_hashtags'
-    hashtag_suggestions_for_text = 'hashtag_suggestions_for_text'
-    hashtag_suggestions_for_image = 'hashtag_suggestions_for_image'
-    hashtag_history = 'hashtag_history'
-    emojis_suggestion = 'emojis_suggestion'
-    auto_emojify = 'auto_emojify'
-    text_to_image = 'text_to_image'
-    animate_image = 'animate_image'
-    company_logo = 'company_logo'
-    list_of_cta = 'list_of_cta'
-    shorten_link = 'shorten_link'
-
-    def __str__(self):
-        return '{0}'.format(self.value)
-
-
-actions = [str(x) for x in [
-    Action.hashtag_stats,
-    Action.auto_hashtags,
-    Action.hashtag_suggestions_for_text,
-    Action.hashtag_suggestions_for_image,
-    Action.hashtag_history,
-    Action.emojis_suggestion,
-    Action.auto_emojify,
-    # Action.text_to_image, not supported yet
-    # Action.animate_image, not supported yet
-    Action.company_logo,
-    Action.list_of_cta,
-    Action.shorten_link
-]]
-
-
-def get_hashtags(parser, args):
-    if args.hashtags is None or len(args.hashtags) == 0:
-        parser.error('missing hashtags')
-    return args.hashtags
-
-
-def get_hashtag(parser, args):
-    if args.hashtags is None or len(args.hashtags) == 0:
-        parser.error('missing hashtag')
-    elif len(args.hashtags) > 1:
-        parser.error('too many hashtags')
-    return args.hashtags[0]
-
-
-def get_domain(parser, args):
-    if args.hashtags is None or len(args.hashtags) == 0:
-        parser.error('missing domain')
-    elif len(args.hashtags) > 1:
-        parser.error('invalid domain')
-    return args.hashtags[0]
-
-
-def get_url(parser, args):
-    if args.hashtags is None or len(args.hashtags) == 0:
-        parser.error('missing url')
-    elif len(args.hashtags) > 1:
-        parser.error('invalid url')
-    return args.hashtags[0]
-
-
-def get_post(parser, args):
-    if args.hashtags is None or len(args.hashtags) == 0:
-        parser.error('missing post')
-    return ' '.join(args.hashtags)
-
-
-def run():
-    parser = argparse.ArgumentParser(description='RiteTag API console client.')
-    parser.add_argument('-t', '--access_token', type=str, help='access token', required=require_token)
-    parser.add_argument('action', choices=actions, help='action')
-    parser.add_argument('hashtags', type=str, nargs='*', help='hashtags')
-    parser.add_argument('-m', '--max_hashtags', type=int, default=2)
-    parser.add_argument('-p', '--hashtag_position', type=str, choices=['auto', 'end'], default='auto')
-    parser.add_argument('-f', '--filename', type=str)
-    parser.add_argument('-ci', '--cta_id', type=int)
-    parser.add_argument('-g', '--auto_generate', type=str, choices=['1', '0'], default='1')
-    args = parser.parse_args()
-
-    api = RiteTagApi(args.access_token if require_token else access_token)
-
-    def log(limit):
-        print(limit)
-
-    api.on_limit(0, log)
-
-    a = Action[args.action]
-
-    # print(args)
-    try:
-        if a == Action.hashtag_stats:
-            hashtags = get_hashtags(parser, args)
-            print('\n'.join([str(x) for x in api.hashtag_stats(hashtags)]))
-
-        elif a == Action.auto_hashtags:
-            post = get_post(parser, args)
-            log(api.auto_hashtag(post, args.max_hashtags))
-
-        elif a == Action.hashtag_suggestions_for_text:
-            post = get_post(parser, args)
-            [log(x) for x in api.hashtag_suggestion_for_text(post)]
-
-        elif a == Action.hashtag_suggestions_for_image:
-            post = get_url(parser, args)
-            [log(x) for x in api.hashtag_suggestion_for_image(post)]
-
-        elif a == Action.hashtag_history:
-            hashtag = get_hashtag(parser, args)
-            [log(x) for x in api.history(hashtag)]
-
-        elif a == Action.emojis_suggestion:
-            text = get_post(parser, args)
-            log(', '.join(api.emoji_suggestion(text)))
-
-        elif a == Action.auto_emojify:
-            text = get_post(parser, args)
-            log(api.auto_emojify(text))
-
-        elif a == Action.text_to_image:
-            parser.error("not implemented yet")
-
-        elif a == Action.animate_image:
-            parser.error('not implemented yet')
-
-        elif a == Action.company_logo:
-            domain = get_domain(parser, args)
-            log('Looking for logo - {}'.format(domain))
-            logo = api.company_logo_2(domain, True if args.auto_generate == '1' else False)
-            filename = domain.replace('.', '_') if args.filename is None else args.filename
-
-            if logo.is_generated:
-                log("Logo is generated.")
-
-            log("Downloading logo - {}".format(domain))
-            try:
-                original_path = '{}.{}'.format(filename, logo.logo_content_type())
-                Parser.download_file(logo.logo(), original_path)
-                log('Image is saved {} - {}'.format(original_path, domain))
-            except RiteTagException as e:
-                log('Error {} - {}'.format(e, domain))
-
-            log("Downloading square logo - {}".format(domain))
-            try:
-                square_path = '{}_square.{}'.format(filename, logo.square_logo_content_type())
-                Parser.download_file(logo.square_logo(), square_path)
-                log('Image is saved {} - {}'.format(domain, square_path))
-            except RiteTagException as e:
-                log('Error {} - {}'.format(e, domain))
-
-        elif a == Action.list_of_cta:
-            [log(x) for x in api.list_of_cta()]
-
-        elif a == Action.shorten_link:
-            url = get_domain(parser, args)
-            cta_id = args.cta_id
-            log(api.shorten_url(url, cta_id).url)
-    except RiteTagException as e:
-        parser.error(e)
-        # raise e
+import argparse
+import os
+from .api import *
+
+current_directory = os.getcwd()
+access_token = os.getenv('ACCESS_TOKEN', None)
+require_token = access_token is None
+
+
+class Action(Enum):
+    hashtag_stats = 'hashtag_stats'
+    auto_hashtags = 'auto_hashtags'
+    hashtag_suggestions_for_text = 'hashtag_suggestions_for_text'
+    hashtag_suggestions_for_image = 'hashtag_suggestions_for_image'
+    hashtag_history = 'hashtag_history'
+    emojis_suggestion = 'emojis_suggestion'
+    auto_emojify = 'auto_emojify'
+    text_to_image = 'text_to_image'
+    animate_image = 'animate_image'
+    company_logo = 'company_logo'
+    list_of_cta = 'list_of_cta'
+    shorten_link = 'shorten_link'
+
+    def __str__(self):
+        return '{0}'.format(self.value)
+
+
+actions = [str(x) for x in [
+    Action.hashtag_stats,
+    Action.auto_hashtags,
+    Action.hashtag_suggestions_for_text,
+    Action.hashtag_suggestions_for_image,
+    Action.hashtag_history,
+    Action.emojis_suggestion,
+    Action.auto_emojify,
+    # Action.text_to_image, not supported yet
+    # Action.animate_image, not supported yet
+    Action.company_logo,
+    Action.list_of_cta,
+    Action.shorten_link
+]]
+
+
+def get_hashtags(parser, args):
+    if args.hashtags is None or len(args.hashtags) == 0:
+        parser.error('missing hashtags')
+    return args.hashtags
+
+
+def get_hashtag(parser, args):
+    if args.hashtags is None or len(args.hashtags) == 0:
+        parser.error('missing hashtag')
+    elif len(args.hashtags) > 1:
+        parser.error('too many hashtags')
+    return args.hashtags[0]
+
+
+def get_domain(parser, args):
+    if args.hashtags is None or len(args.hashtags) == 0:
+        parser.error('missing domain')
+    elif len(args.hashtags) > 1:
+        parser.error('invalid domain')
+    return args.hashtags[0]
+
+
+def get_url(parser, args):
+    if args.hashtags is None or len(args.hashtags) == 0:
+        parser.error('missing url')
+    elif len(args.hashtags) > 1:
+        parser.error('invalid url')
+    return args.hashtags[0]
+
+
+def get_post(parser, args):
+    if args.hashtags is None or len(args.hashtags) == 0:
+        parser.error('missing post')
+    return ' '.join(args.hashtags)
+
+
+def run():
+    parser = argparse.ArgumentParser(description='RiteTag API console client.')
+    parser.add_argument('-t', '--access_token', type=str, help='access token', required=require_token)
+    parser.add_argument('action', choices=actions, help='action')
+    parser.add_argument('hashtags', type=str, nargs='*', help='hashtags')
+    parser.add_argument('-m', '--max_hashtags', type=int, default=2)
+    parser.add_argument('-p', '--hashtag_position', type=str, choices=['auto', 'end'], default='auto')
+    parser.add_argument('-f', '--filename', type=str)
+    parser.add_argument('-ci', '--cta_id', type=int)
+    parser.add_argument('-g', '--auto_generate', type=str, choices=['1', '0'], default='1')
+    parser.add_argument('-s', '--square_size', type=int, choices=range(1, 512), default=256)
+    parser.add_argument('-bg', '--square_background', type=str, choices=['original', 'remove', 'add'],
+                        default='original')
+    args = parser.parse_args()
+
+    api = RiteTagApi(args.access_token if require_token else access_token)
+
+    def log(limit):
+        print(limit)
+
+    api.on_limit(0, log)
+
+    a = Action[args.action]
+
+    # print(args)
+    try:
+        if a == Action.hashtag_stats:
+            hashtags = get_hashtags(parser, args)
+            print('\n'.join([str(x) for x in api.hashtag_stats(hashtags)]))
+
+        elif a == Action.auto_hashtags:
+            post = get_post(parser, args)
+            log(api.auto_hashtag(post, args.max_hashtags))
+
+        elif a == Action.hashtag_suggestions_for_text:
+            post = get_post(parser, args)
+            [log(x) for x in api.hashtag_suggestion_for_text(post)]
+
+        elif a == Action.hashtag_suggestions_for_image:
+            post = get_url(parser, args)
+            [log(x) for x in api.hashtag_suggestion_for_image(post)]
+
+        elif a == Action.hashtag_history:
+            hashtag = get_hashtag(parser, args)
+            [log(x) for x in api.history(hashtag)]
+
+        elif a == Action.emojis_suggestion:
+            text = get_post(parser, args)
+            log(', '.join(api.emoji_suggestion(text)))
+
+        elif a == Action.auto_emojify:
+            text = get_post(parser, args)
+            log(api.auto_emojify(text))
+
+        elif a == Action.text_to_image:
+            parser.error("not implemented yet")
+
+        elif a == Action.animate_image:
+            parser.error('not implemented yet')
+
+        elif a == Action.company_logo:
+            domain = get_domain(parser, args)
+            log('Looking for logo - {}'.format(domain))
+            logo = api.company_logo_2(domain, True if args.auto_generate == '1' else False, args.square_size, args.square_background)
+            filename = domain.replace('.', '_') if args.filename is None else args.filename
+
+            if logo.is_generated:
+                log("Logo is generated.")
+
+            log("Downloading logo - {}".format(domain))
+            try:
+                original_path = '{}.{}'.format(filename, logo.logo_content_type())
+                Parser.download_file(logo.logo(), original_path)
+                log('Image is saved {} - {}'.format(original_path, domain))
+            except RiteTagException as e:
+                log('Error {} - {}'.format(e, domain))
+
+            log("Downloading square logo - {}".format(domain))
+            try:
+                square_path = '{}_square.{}'.format(filename, logo.square_logo_content_type())
+                Parser.download_file(logo.square_logo(), square_path)
+                log('Image is saved {} - {}'.format(domain, square_path))
+            except RiteTagException as e:
+                log('Error {} - {}'.format(e, domain))
+
+        elif a == Action.list_of_cta:
+            [log(x) for x in api.list_of_cta()]
+
+        elif a == Action.shorten_link:
+            url = get_domain(parser, args)
+            cta_id = args.cta_id
+            log(api.shorten_url(url, cta_id).url)
+    except RiteTagException as e:
+        parser.error(e)
+        # raise e
```

### Comparing `ritetag-1.3.2/ritetag/enums.py` & `ritetag-1.3.3/ritetag/enums.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,1040 +1,1040 @@
-from enum import Enum
-
-
-class HashtagPosition(Enum):
-    auto = 'auto'
-    end = 'end'
-
-    def __str__(self):
-        return '{0}'.format(self.value)
-
-
-class AnimationType(Enum):
-    none = 'none'
-    rays = 'rays'
-    glint = 'glint'
-    circle = 'circle'
-
-    def __str__(self):
-        return '{0}'.format(self.value)
-
-
-class FontList(Enum):
-    ABeeZee = 'ABeeZee'
-    Abel = 'Abel'
-    Abhaya_Libre = 'Abhaya Libre'
-    Abril_Fatface = 'Abril Fatface'
-    Aclonica = 'Aclonica'
-    Acme = 'Acme'
-    Actor = 'Actor'
-    Adamina = 'Adamina'
-    Advent_Pro = 'Advent Pro'
-    Aguafina_Script = 'Aguafina Script'
-    Akronim = 'Akronim'
-    Aladin = 'Aladin'
-    Alata = 'Alata'
-    Alatsi = 'Alatsi'
-    Aldrich = 'Aldrich'
-    Alef = 'Alef'
-    Alegreya = 'Alegreya'
-    Alegreya_SC = 'Alegreya SC'
-    Alegreya_Sans = 'Alegreya Sans'
-    Alegreya_Sans_SC = 'Alegreya Sans SC'
-    Aleo = 'Aleo'
-    Alex_Brush = 'Alex Brush'
-    Alfa_Slab_One = 'Alfa Slab One'
-    Alice = 'Alice'
-    Alike = 'Alike'
-    Alike_Angular = 'Alike Angular'
-    Allan = 'Allan'
-    Allerta = 'Allerta'
-    Allerta_Stencil = 'Allerta Stencil'
-    Allura = 'Allura'
-    Almarai = 'Almarai'
-    Almendra = 'Almendra'
-    Almendra_Display = 'Almendra Display'
-    Almendra_SC = 'Almendra SC'
-    Amarante = 'Amarante'
-    Amaranth = 'Amaranth'
-    Amatic_SC = 'Amatic SC'
-    Amethysta = 'Amethysta'
-    Amiko = 'Amiko'
-    Amiri = 'Amiri'
-    Amita = 'Amita'
-    Anaheim = 'Anaheim'
-    Andada = 'Andada'
-    Andika = 'Andika'
-    Angkor = 'Angkor'
-    Annie_Use_Your_Telescope = 'Annie Use Your Telescope'
-    Anonymous_Pro = 'Anonymous Pro'
-    Antic = 'Antic'
-    Antic_Didone = 'Antic Didone'
-    Antic_Slab = 'Antic Slab'
-    Anton = 'Anton'
-    Arapey = 'Arapey'
-    Arbutus = 'Arbutus'
-    Arbutus_Slab = 'Arbutus Slab'
-    Architects_Daughter = 'Architects Daughter'
-    Archivo = 'Archivo'
-    Archivo_Black = 'Archivo Black'
-    Archivo_Narrow = 'Archivo Narrow'
-    Aref_Ruqaa = 'Aref Ruqaa'
-    Arima_Madurai = 'Arima Madurai'
-    Arimo = 'Arimo'
-    Arizonia = 'Arizonia'
-    Armata = 'Armata'
-    Arsenal = 'Arsenal'
-    Artifika = 'Artifika'
-    Arvo = 'Arvo'
-    Arya = 'Arya'
-    Asap = 'Asap'
-    Asap_Condensed = 'Asap Condensed'
-    Asar = 'Asar'
-    Asset = 'Asset'
-    Assistant = 'Assistant'
-    Astloch = 'Astloch'
-    Asul = 'Asul'
-    Athiti = 'Athiti'
-    Atma = 'Atma'
-    Atomic_Age = 'Atomic Age'
-    Aubrey = 'Aubrey'
-    Audiowide = 'Audiowide'
-    Autour_One = 'Autour One'
-    Average = 'Average'
-    Average_Sans = 'Average Sans'
-    Averia_Gruesa_Libre = 'Averia Gruesa Libre'
-    Averia_Libre = 'Averia Libre'
-    Averia_Sans_Libre = 'Averia Sans Libre'
-    Averia_Serif_Libre = 'Averia Serif Libre'
-    B612 = 'B612'
-    B612_Mono = 'B612 Mono'
-    Bad_Script = 'Bad Script'
-    Bahiana = 'Bahiana'
-    Bahianita = 'Bahianita'
-    Bai_Jamjuree = 'Bai Jamjuree'
-    Baloo_2 = 'Baloo 2'
-    Baloo_Bhai_2 = 'Baloo Bhai 2'
-    Baloo_Bhaina_2 = 'Baloo Bhaina 2'
-    Baloo_Chettan_2 = 'Baloo Chettan 2'
-    Baloo_Da_2 = 'Baloo Da 2'
-    Baloo_Paaji_2 = 'Baloo Paaji 2'
-    Baloo_Tamma_2 = 'Baloo Tamma 2'
-    Baloo_Tammudu_2 = 'Baloo Tammudu 2'
-    Baloo_Thambi_2 = 'Baloo Thambi 2'
-    Balsamiq_Sans = 'Balsamiq Sans'
-    Balthazar = 'Balthazar'
-    Bangers = 'Bangers'
-    Barlow = 'Barlow'
-    Barlow_Condensed = 'Barlow Condensed'
-    Barlow_Semi_Condensed = 'Barlow Semi Condensed'
-    Barriecito = 'Barriecito'
-    Barrio = 'Barrio'
-    Basic = 'Basic'
-    Baskervville = 'Baskervville'
-    Battambang = 'Battambang'
-    Baumans = 'Baumans'
-    Bayon = 'Bayon'
-    Be_Vietnam = 'Be Vietnam'
-    Bebas_Neue = 'Bebas Neue'
-    Belgrano = 'Belgrano'
-    Bellefair = 'Bellefair'
-    Belleza = 'Belleza'
-    Bellota = 'Bellota'
-    Bellota_Text = 'Bellota Text'
-    BenchNine = 'BenchNine'
-    Bentham = 'Bentham'
-    Berkshire_Swash = 'Berkshire Swash'
-    Beth_Ellen = 'Beth Ellen'
-    Bevan = 'Bevan'
-    Big_Shoulders_Display = 'Big Shoulders Display'
-    Big_Shoulders_Text = 'Big Shoulders Text'
-    Bigelow_Rules = 'Bigelow Rules'
-    Bigshot_One = 'Bigshot One'
-    Bilbo = 'Bilbo'
-    Bilbo_Swash_Caps = 'Bilbo Swash Caps'
-    BioRhyme = 'BioRhyme'
-    BioRhyme_Expanded = 'BioRhyme Expanded'
-    Biryani = 'Biryani'
-    Bitter = 'Bitter'
-    Black_And_White_Picture = 'Black And White Picture'
-    Black_Han_Sans = 'Black Han Sans'
-    Black_Ops_One = 'Black Ops One'
-    Blinker = 'Blinker'
-    Bokor = 'Bokor'
-    Bonbon = 'Bonbon'
-    Boogaloo = 'Boogaloo'
-    Bowlby_One = 'Bowlby One'
-    Bowlby_One_SC = 'Bowlby One SC'
-    Brawler = 'Brawler'
-    Bree_Serif = 'Bree Serif'
-    Bubblegum_Sans = 'Bubblegum Sans'
-    Bubbler_One = 'Bubbler One'
-    Buda = 'Buda'
-    Buenard = 'Buenard'
-    Bungee = 'Bungee'
-    Bungee_Hairline = 'Bungee Hairline'
-    Bungee_Inline = 'Bungee Inline'
-    Bungee_Outline = 'Bungee Outline'
-    Bungee_Shade = 'Bungee Shade'
-    Butcherman = 'Butcherman'
-    Butterfly_Kids = 'Butterfly Kids'
-    Cabin = 'Cabin'
-    Cabin_Condensed = 'Cabin Condensed'
-    Cabin_Sketch = 'Cabin Sketch'
-    Caesar_Dressing = 'Caesar Dressing'
-    Cagliostro = 'Cagliostro'
-    Cairo = 'Cairo'
-    Caladea = 'Caladea'
-    Calistoga = 'Calistoga'
-    Calligraffitti = 'Calligraffitti'
-    Cambay = 'Cambay'
-    Cambo = 'Cambo'
-    Candal = 'Candal'
-    Cantarell = 'Cantarell'
-    Cantata_One = 'Cantata One'
-    Cantora_One = 'Cantora One'
-    Capriola = 'Capriola'
-    Cardo = 'Cardo'
-    Carme = 'Carme'
-    Carrois_Gothic = 'Carrois Gothic'
-    Carrois_Gothic_SC = 'Carrois Gothic SC'
-    Carter_One = 'Carter One'
-    Catamaran = 'Catamaran'
-    Caudex = 'Caudex'
-    Caveat = 'Caveat'
-    Caveat_Brush = 'Caveat Brush'
-    Cedarville_Cursive = 'Cedarville Cursive'
-    Ceviche_One = 'Ceviche One'
-    Chakra_Petch = 'Chakra Petch'
-    Changa = 'Changa'
-    Changa_One = 'Changa One'
-    Chango = 'Chango'
-    Charm = 'Charm'
-    Charmonman = 'Charmonman'
-    Chathura = 'Chathura'
-    Chau_Philomene_One = 'Chau Philomene One'
-    Chela_One = 'Chela One'
-    Chelsea_Market = 'Chelsea Market'
-    Chenla = 'Chenla'
-    Cherry_Cream_Soda = 'Cherry Cream Soda'
-    Cherry_Swash = 'Cherry Swash'
-    Chewy = 'Chewy'
-    Chicle = 'Chicle'
-    Chilanka = 'Chilanka'
-    Chivo = 'Chivo'
-    Chonburi = 'Chonburi'
-    Cinzel = 'Cinzel'
-    Cinzel_Decorative = 'Cinzel Decorative'
-    Clicker_Script = 'Clicker Script'
-    Coda = 'Coda'
-    Coda_Caption = 'Coda Caption'
-    Codystar = 'Codystar'
-    Coiny = 'Coiny'
-    Combo = 'Combo'
-    Comfortaa = 'Comfortaa'
-    Comic_Neue = 'Comic Neue'
-    Coming_Soon = 'Coming Soon'
-    Concert_One = 'Concert One'
-    Condiment = 'Condiment'
-    Content = 'Content'
-    Contrail_One = 'Contrail One'
-    Convergence = 'Convergence'
-    Cookie = 'Cookie'
-    Copse = 'Copse'
-    Corben = 'Corben'
-    Cormorant = 'Cormorant'
-    Cormorant_Garamond = 'Cormorant Garamond'
-    Cormorant_Infant = 'Cormorant Infant'
-    Cormorant_SC = 'Cormorant SC'
-    Cormorant_Unicase = 'Cormorant Unicase'
-    Cormorant_Upright = 'Cormorant Upright'
-    Courgette = 'Courgette'
-    Courier_Prime = 'Courier Prime'
-    Cousine = 'Cousine'
-    Coustard = 'Coustard'
-    Covered_By_Your_Grace = 'Covered By Your Grace'
-    Crafty_Girls = 'Crafty Girls'
-    Creepster = 'Creepster'
-    Crete_Round = 'Crete Round'
-    Crimson_Pro = 'Crimson Pro'
-    Crimson_Text = 'Crimson Text'
-    Croissant_One = 'Croissant One'
-    Crushed = 'Crushed'
-    Cuprum = 'Cuprum'
-    Cute_Font = 'Cute Font'
-    Cutive = 'Cutive'
-    Cutive_Mono = 'Cutive Mono'
-    DM_Mono = 'DM Mono'
-    DM_Sans = 'DM Sans'
-    DM_Serif_Display = 'DM Serif Display'
-    DM_Serif_Text = 'DM Serif Text'
-    Damion = 'Damion'
-    Dancing_Script = 'Dancing Script'
-    Dangrek = 'Dangrek'
-    Darker_Grotesque = 'Darker Grotesque'
-    David_Libre = 'David Libre'
-    Dawning_of_a_New_Day = 'Dawning of a New Day'
-    Days_One = 'Days One'
-    Dekko = 'Dekko'
-    Delius = 'Delius'
-    Delius_Swash_Caps = 'Delius Swash Caps'
-    Delius_Unicase = 'Delius Unicase'
-    Della_Respira = 'Della Respira'
-    Denk_One = 'Denk One'
-    Devonshire = 'Devonshire'
-    Dhurjati = 'Dhurjati'
-    Didact_Gothic = 'Didact Gothic'
-    Diplomata = 'Diplomata'
-    Diplomata_SC = 'Diplomata SC'
-    Do_Hyeon = 'Do Hyeon'
-    Dokdo = 'Dokdo'
-    Domine = 'Domine'
-    Donegal_One = 'Donegal One'
-    Doppio_One = 'Doppio One'
-    Dorsa = 'Dorsa'
-    Dosis = 'Dosis'
-    Dr_Sugiyama = 'Dr Sugiyama'
-    Duru_Sans = 'Duru Sans'
-    Dynalight = 'Dynalight'
-    EB_Garamond = 'EB Garamond'
-    Eagle_Lake = 'Eagle Lake'
-    East_Sea_Dokdo = 'East Sea Dokdo'
-    Eater = 'Eater'
-    Economica = 'Economica'
-    Eczar = 'Eczar'
-    El_Messiri = 'El Messiri'
-    Electrolize = 'Electrolize'
-    Elsie = 'Elsie'
-    Elsie_Swash_Caps = 'Elsie Swash Caps'
-    Emblema_One = 'Emblema One'
-    Emilys_Candy = 'Emilys Candy'
-    Encode_Sans = 'Encode Sans'
-    Encode_Sans_Condensed = 'Encode Sans Condensed'
-    Encode_Sans_Expanded = 'Encode Sans Expanded'
-    Encode_Sans_Semi_Condensed = 'Encode Sans Semi Condensed'
-    Encode_Sans_Semi_Expanded = 'Encode Sans Semi Expanded'
-    Engagement = 'Engagement'
-    Englebert = 'Englebert'
-    Enriqueta = 'Enriqueta'
-    Epilogue = 'Epilogue'
-    Erica_One = 'Erica One'
-    Esteban = 'Esteban'
-    Euphoria_Script = 'Euphoria Script'
-    Ewert = 'Ewert'
-    Exo = 'Exo'
-    Exo_2 = 'Exo 2'
-    Expletus_Sans = 'Expletus Sans'
-    Fahkwang = 'Fahkwang'
-    Fanwood_Text = 'Fanwood Text'
-    Farro = 'Farro'
-    Farsan = 'Farsan'
-    Fascinate = 'Fascinate'
-    Fascinate_Inline = 'Fascinate Inline'
-    Faster_One = 'Faster One'
-    Fasthand = 'Fasthand'
-    Fauna_One = 'Fauna One'
-    Faustina = 'Faustina'
-    Federant = 'Federant'
-    Federo = 'Federo'
-    Felipa = 'Felipa'
-    Fenix = 'Fenix'
-    Finger_Paint = 'Finger Paint'
-    Fira_Code = 'Fira Code'
-    Fira_Mono = 'Fira Mono'
-    Fira_Sans = 'Fira Sans'
-    Fira_Sans_Condensed = 'Fira Sans Condensed'
-    Fira_Sans_Extra_Condensed = 'Fira Sans Extra Condensed'
-    Fjalla_One = 'Fjalla One'
-    Fjord_One = 'Fjord One'
-    Flamenco = 'Flamenco'
-    Flavors = 'Flavors'
-    Fondamento = 'Fondamento'
-    Fontdiner_Swanky = 'Fontdiner Swanky'
-    Forum = 'Forum'
-    Francois_One = 'Francois One'
-    Frank_Ruhl_Libre = 'Frank Ruhl Libre'
-    Freckle_Face = 'Freckle Face'
-    Fredericka_the_Great = 'Fredericka the Great'
-    Fredoka_One = 'Fredoka One'
-    Freehand = 'Freehand'
-    Fresca = 'Fresca'
-    Frijole = 'Frijole'
-    Fruktur = 'Fruktur'
-    Fugaz_One = 'Fugaz One'
-    GFS_Didot = 'GFS Didot'
-    GFS_Neohellenic = 'GFS Neohellenic'
-    Gabriela = 'Gabriela'
-    Gaegu = 'Gaegu'
-    Gafata = 'Gafata'
-    Galada = 'Galada'
-    Galdeano = 'Galdeano'
-    Galindo = 'Galindo'
-    Gamja_Flower = 'Gamja Flower'
-    Gayathri = 'Gayathri'
-    Gelasio = 'Gelasio'
-    Gentium_Basic = 'Gentium Basic'
-    Gentium_Book_Basic = 'Gentium Book Basic'
-    Geo = 'Geo'
-    Geostar = 'Geostar'
-    Geostar_Fill = 'Geostar Fill'
-    Germania_One = 'Germania One'
-    Gidugu = 'Gidugu'
-    Gilda_Display = 'Gilda Display'
-    Girassol = 'Girassol'
-    Give_You_Glory = 'Give You Glory'
-    Glass_Antiqua = 'Glass Antiqua'
-    Glegoo = 'Glegoo'
-    Gloria_Hallelujah = 'Gloria Hallelujah'
-    Goblin_One = 'Goblin One'
-    Gochi_Hand = 'Gochi Hand'
-    Gorditas = 'Gorditas'
-    Gothic_A1 = 'Gothic A1'
-    Gotu = 'Gotu'
-    Goudy_Bookletter_1911 = 'Goudy Bookletter 1911'
-    Graduate = 'Graduate'
-    Grand_Hotel = 'Grand Hotel'
-    Gravitas_One = 'Gravitas One'
-    Great_Vibes = 'Great Vibes'
-    Grenze = 'Grenze'
-    Grenze_Gotisch = 'Grenze Gotisch'
-    Griffy = 'Griffy'
-    Gruppo = 'Gruppo'
-    Gudea = 'Gudea'
-    Gugi = 'Gugi'
-    Gupter = 'Gupter'
-    Gurajada = 'Gurajada'
-    Habibi = 'Habibi'
-    Halant = 'Halant'
-    Hammersmith_One = 'Hammersmith One'
-    Hanalei = 'Hanalei'
-    Hanalei_Fill = 'Hanalei Fill'
-    Handlee = 'Handlee'
-    Hanuman = 'Hanuman'
-    Happy_Monkey = 'Happy Monkey'
-    Harmattan = 'Harmattan'
-    Headland_One = 'Headland One'
-    Heebo = 'Heebo'
-    Henny_Penny = 'Henny Penny'
-    Hepta_Slab = 'Hepta Slab'
-    Herr_Von_Muellerhoff = 'Herr Von Muellerhoff'
-    Hi_Melody = 'Hi Melody'
-    Hind = 'Hind'
-    Hind_Guntur = 'Hind Guntur'
-    Hind_Madurai = 'Hind Madurai'
-    Hind_Siliguri = 'Hind Siliguri'
-    Hind_Vadodara = 'Hind Vadodara'
-    Holtwood_One_SC = 'Holtwood One SC'
-    Homemade_Apple = 'Homemade Apple'
-    Homenaje = 'Homenaje'
-    IBM_Plex_Mono = 'IBM Plex Mono'
-    IBM_Plex_Sans = 'IBM Plex Sans'
-    IBM_Plex_Sans_Condensed = 'IBM Plex Sans Condensed'
-    IBM_Plex_Serif = 'IBM Plex Serif'
-    IM_Fell_DW_Pica = 'IM Fell DW Pica'
-    IM_Fell_DW_Pica_SC = 'IM Fell DW Pica SC'
-    IM_Fell_Double_Pica = 'IM Fell Double Pica'
-    IM_Fell_Double_Pica_SC = 'IM Fell Double Pica SC'
-    IM_Fell_English = 'IM Fell English'
-    IM_Fell_English_SC = 'IM Fell English SC'
-    IM_Fell_French_Canon = 'IM Fell French Canon'
-    IM_Fell_French_Canon_SC = 'IM Fell French Canon SC'
-    IM_Fell_Great_Primer = 'IM Fell Great Primer'
-    IM_Fell_Great_Primer_SC = 'IM Fell Great Primer SC'
-    Ibarra_Real_Nova = 'Ibarra Real Nova'
-    Iceberg = 'Iceberg'
-    Iceland = 'Iceland'
-    Imprima = 'Imprima'
-    Inconsolata = 'Inconsolata'
-    Inder = 'Inder'
-    Indie_Flower = 'Indie Flower'
-    Inika = 'Inika'
-    Inknut_Antiqua = 'Inknut Antiqua'
-    Inria_Sans = 'Inria Sans'
-    Inria_Serif = 'Inria Serif'
-    Inter = 'Inter'
-    Irish_Grover = 'Irish Grover'
-    Istok_Web = 'Istok Web'
-    Italiana = 'Italiana'
-    Italianno = 'Italianno'
-    Itim = 'Itim'
-    Jacques_Francois = 'Jacques Francois'
-    Jacques_Francois_Shadow = 'Jacques Francois Shadow'
-    Jaldi = 'Jaldi'
-    Jim_Nightshade = 'Jim Nightshade'
-    Jockey_One = 'Jockey One'
-    Jolly_Lodger = 'Jolly Lodger'
-    Jomhuria = 'Jomhuria'
-    Jomolhari = 'Jomolhari'
-    Josefin_Sans = 'Josefin Sans'
-    Josefin_Slab = 'Josefin Slab'
-    Jost = 'Jost'
-    Joti_One = 'Joti One'
-    Jua = 'Jua'
-    Judson = 'Judson'
-    Julee = 'Julee'
-    Julius_Sans_One = 'Julius Sans One'
-    Junge = 'Junge'
-    Jura = 'Jura'
-    Just_Another_Hand = 'Just Another Hand'
-    Just_Me_Again_Down_Here = 'Just Me Again Down Here'
-    K2D = 'K2D'
-    Kadwa = 'Kadwa'
-    Kalam = 'Kalam'
-    Kameron = 'Kameron'
-    Kanit = 'Kanit'
-    Kantumruy = 'Kantumruy'
-    Karla = 'Karla'
-    Karma = 'Karma'
-    Katibeh = 'Katibeh'
-    Kaushan_Script = 'Kaushan Script'
-    Kavivanar = 'Kavivanar'
-    Kavoon = 'Kavoon'
-    Kdam_Thmor = 'Kdam Thmor'
-    Keania_One = 'Keania One'
-    Kelly_Slab = 'Kelly Slab'
-    Kenia = 'Kenia'
-    Khand = 'Khand'
-    Khmer = 'Khmer'
-    Khula = 'Khula'
-    Kirang_Haerang = 'Kirang Haerang'
-    Kite_One = 'Kite One'
-    Knewave = 'Knewave'
-    KoHo = 'KoHo'
-    Kodchasan = 'Kodchasan'
-    Kosugi = 'Kosugi'
-    Kosugi_Maru = 'Kosugi Maru'
-    Kotta_One = 'Kotta One'
-    Koulen = 'Koulen'
-    Kranky = 'Kranky'
-    Kreon = 'Kreon'
-    Kristi = 'Kristi'
-    Krona_One = 'Krona One'
-    Krub = 'Krub'
-    Kulim_Park = 'Kulim Park'
-    Kumar_One = 'Kumar One'
-    Kumar_One_Outline = 'Kumar One Outline'
-    Kurale = 'Kurale'
-    La_Belle_Aurore = 'La Belle Aurore'
-    Lacquer = 'Lacquer'
-    Laila = 'Laila'
-    Lakki_Reddy = 'Lakki Reddy'
-    Lalezar = 'Lalezar'
-    Lancelot = 'Lancelot'
-    Lateef = 'Lateef'
-    Lato = 'Lato'
-    League_Script = 'League Script'
-    Leckerli_One = 'Leckerli One'
-    Ledger = 'Ledger'
-    Lekton = 'Lekton'
-    Lemon = 'Lemon'
-    Lemonada = 'Lemonada'
-    Lexend_Deca = 'Lexend Deca'
-    Lexend_Exa = 'Lexend Exa'
-    Lexend_Giga = 'Lexend Giga'
-    Lexend_Mega = 'Lexend Mega'
-    Lexend_Peta = 'Lexend Peta'
-    Lexend_Tera = 'Lexend Tera'
-    Lexend_Zetta = 'Lexend Zetta'
-    Libre_Barcode_128 = 'Libre Barcode 128'
-    Libre_Barcode_128_Text = 'Libre Barcode 128 Text'
-    Libre_Barcode_39 = 'Libre Barcode 39'
-    Libre_Barcode_39_Extended = 'Libre Barcode 39 Extended'
-    Libre_Barcode_39_Extended_Text = 'Libre Barcode 39 Extended Text'
-    Libre_Barcode_39_Text = 'Libre Barcode 39 Text'
-    Libre_Baskerville = 'Libre Baskerville'
-    Libre_Caslon_Display = 'Libre Caslon Display'
-    Libre_Caslon_Text = 'Libre Caslon Text'
-    Libre_Franklin = 'Libre Franklin'
-    Life_Savers = 'Life Savers'
-    Lilita_One = 'Lilita One'
-    Lily_Script_One = 'Lily Script One'
-    Limelight = 'Limelight'
-    Linden_Hill = 'Linden Hill'
-    Literata = 'Literata'
-    Liu_Jian_Mao_Cao = 'Liu Jian Mao Cao'
-    Livvic = 'Livvic'
-    Lobster = 'Lobster'
-    Lobster_Two = 'Lobster Two'
-    Londrina_Outline = 'Londrina Outline'
-    Londrina_Shadow = 'Londrina Shadow'
-    Londrina_Sketch = 'Londrina Sketch'
-    Londrina_Solid = 'Londrina Solid'
-    Long_Cang = 'Long Cang'
-    Lora = 'Lora'
-    Love_Ya_Like_A_Sister = 'Love Ya Like A Sister'
-    Loved_by_the_King = 'Loved by the King'
-    Lovers_Quarrel = 'Lovers Quarrel'
-    Luckiest_Guy = 'Luckiest Guy'
-    Lusitana = 'Lusitana'
-    Lustria = 'Lustria'
-    M_PLUS_1p = 'M PLUS 1p'
-    M_PLUS_Rounded_1c = 'M PLUS Rounded 1c'
-    Ma_Shan_Zheng = 'Ma Shan Zheng'
-    Macondo = 'Macondo'
-    Macondo_Swash_Caps = 'Macondo Swash Caps'
-    Mada = 'Mada'
-    Magra = 'Magra'
-    Maiden_Orange = 'Maiden Orange'
-    Maitree = 'Maitree'
-    Major_Mono_Display = 'Major Mono Display'
-    Mako = 'Mako'
-    Mali = 'Mali'
-    Mallanna = 'Mallanna'
-    Mandali = 'Mandali'
-    Manjari = 'Manjari'
-    Manrope = 'Manrope'
-    Mansalva = 'Mansalva'
-    Manuale = 'Manuale'
-    Marcellus = 'Marcellus'
-    Marcellus_SC = 'Marcellus SC'
-    Marck_Script = 'Marck Script'
-    Margarine = 'Margarine'
-    Markazi_Text = 'Markazi Text'
-    Marko_One = 'Marko One'
-    Marmelad = 'Marmelad'
-    Martel = 'Martel'
-    Martel_Sans = 'Martel Sans'
-    Marvel = 'Marvel'
-    Mate = 'Mate'
-    Mate_SC = 'Mate SC'
-    Maven_Pro = 'Maven Pro'
-    McLaren = 'McLaren'
-    Meddon = 'Meddon'
-    MedievalSharp = 'MedievalSharp'
-    Medula_One = 'Medula One'
-    Meera_Inimai = 'Meera Inimai'
-    Megrim = 'Megrim'
-    Meie_Script = 'Meie Script'
-    Merienda = 'Merienda'
-    Merienda_One = 'Merienda One'
-    Merriweather = 'Merriweather'
-    Merriweather_Sans = 'Merriweather Sans'
-    Metal = 'Metal'
-    Metal_Mania = 'Metal Mania'
-    Metamorphous = 'Metamorphous'
-    Metrophobic = 'Metrophobic'
-    Michroma = 'Michroma'
-    Milonga = 'Milonga'
-    Miltonian = 'Miltonian'
-    Miltonian_Tattoo = 'Miltonian Tattoo'
-    Mina = 'Mina'
-    Miniver = 'Miniver'
-    Miriam_Libre = 'Miriam Libre'
-    Mirza = 'Mirza'
-    Miss_Fajardose = 'Miss Fajardose'
-    Mitr = 'Mitr'
-    Modak = 'Modak'
-    Modern_Antiqua = 'Modern Antiqua'
-    Mogra = 'Mogra'
-    Molengo = 'Molengo'
-    Molle = 'Molle'
-    Monda = 'Monda'
-    Monofett = 'Monofett'
-    Monoton = 'Monoton'
-    Monsieur_La_Doulaise = 'Monsieur La Doulaise'
-    Montaga = 'Montaga'
-    Montez = 'Montez'
-    Montserrat = 'Montserrat'
-    Montserrat_Alternates = 'Montserrat Alternates'
-    Montserrat_Subrayada = 'Montserrat Subrayada'
-    Moul = 'Moul'
-    Moulpali = 'Moulpali'
-    Mountains_of_Christmas = 'Mountains of Christmas'
-    Mouse_Memoirs = 'Mouse Memoirs'
-    Mr_Bedfort = 'Mr Bedfort'
-    Mr_Dafoe = 'Mr Dafoe'
-    Mr_De_Haviland = 'Mr De Haviland'
-    Mrs_Saint_Delafield = 'Mrs Saint Delafield'
-    Mrs_Sheppards = 'Mrs Sheppards'
-    Mukta = 'Mukta'
-    Mukta_Mahee = 'Mukta Mahee'
-    Mukta_Malar = 'Mukta Malar'
-    Mukta_Vaani = 'Mukta Vaani'
-    Mulish = 'Mulish'
-    MuseoModerno = 'MuseoModerno'
-    Mystery_Quest = 'Mystery Quest'
-    NTR = 'NTR'
-    Nanum_Brush_Script = 'Nanum Brush Script'
-    Nanum_Gothic = 'Nanum Gothic'
-    Nanum_Gothic_Coding = 'Nanum Gothic Coding'
-    Nanum_Myeongjo = 'Nanum Myeongjo'
-    Nanum_Pen_Script = 'Nanum Pen Script'
-    Neucha = 'Neucha'
-    Neuton = 'Neuton'
-    New_Rocker = 'New Rocker'
-    News_Cycle = 'News Cycle'
-    Niconne = 'Niconne'
-    Niramit = 'Niramit'
-    Nixie_One = 'Nixie One'
-    Nobile = 'Nobile'
-    Nokora = 'Nokora'
-    Norican = 'Norican'
-    Nosifer = 'Nosifer'
-    Notable = 'Notable'
-    Nothing_You_Could_Do = 'Nothing You Could Do'
-    Noticia_Text = 'Noticia Text'
-    Noto_Sans = 'Noto Sans'
-    Noto_Sans_HK = 'Noto Sans HK'
-    Noto_Sans_JP = 'Noto Sans JP'
-    Noto_Sans_KR = 'Noto Sans KR'
-    Noto_Sans_SC = 'Noto Sans SC'
-    Noto_Sans_TC = 'Noto Sans TC'
-    Noto_Serif = 'Noto Serif'
-    Noto_Serif_JP = 'Noto Serif JP'
-    Noto_Serif_KR = 'Noto Serif KR'
-    Noto_Serif_SC = 'Noto Serif SC'
-    Noto_Serif_TC = 'Noto Serif TC'
-    Nova_Cut = 'Nova Cut'
-    Nova_Flat = 'Nova Flat'
-    Nova_Mono = 'Nova Mono'
-    Nova_Oval = 'Nova Oval'
-    Nova_Round = 'Nova Round'
-    Nova_Script = 'Nova Script'
-    Nova_Slim = 'Nova Slim'
-    Nova_Square = 'Nova Square'
-    Numans = 'Numans'
-    Nunito = 'Nunito'
-    Nunito_Sans = 'Nunito Sans'
-    Odibee_Sans = 'Odibee Sans'
-    Odor_Mean_Chey = 'Odor Mean Chey'
-    Offside = 'Offside'
-    Old_Standard_TT = 'Old Standard TT'
-    Oldenburg = 'Oldenburg'
-    Oleo_Script = 'Oleo Script'
-    Oleo_Script_Swash_Caps = 'Oleo Script Swash Caps'
-    Open_Sans = 'Open Sans'
-    Open_Sans_Condensed = 'Open Sans Condensed'
-    Oranienbaum = 'Oranienbaum'
-    Orbitron = 'Orbitron'
-    Oregano = 'Oregano'
-    Orienta = 'Orienta'
-    Original_Surfer = 'Original Surfer'
-    Oswald = 'Oswald'
-    Over_the_Rainbow = 'Over the Rainbow'
-    Overlock = 'Overlock'
-    Overlock_SC = 'Overlock SC'
-    Overpass = 'Overpass'
-    Overpass_Mono = 'Overpass Mono'
-    Ovo = 'Ovo'
-    Oxanium = 'Oxanium'
-    Oxygen = 'Oxygen'
-    Oxygen_Mono = 'Oxygen Mono'
-    PT_Mono = 'PT Mono'
-    PT_Sans = 'PT Sans'
-    PT_Sans_Caption = 'PT Sans Caption'
-    PT_Sans_Narrow = 'PT Sans Narrow'
-    PT_Serif = 'PT Serif'
-    PT_Serif_Caption = 'PT Serif Caption'
-    Pacifico = 'Pacifico'
-    Padauk = 'Padauk'
-    Palanquin = 'Palanquin'
-    Palanquin_Dark = 'Palanquin Dark'
-    Pangolin = 'Pangolin'
-    Paprika = 'Paprika'
-    Parisienne = 'Parisienne'
-    Passero_One = 'Passero One'
-    Passion_One = 'Passion One'
-    Pathway_Gothic_One = 'Pathway Gothic One'
-    Patrick_Hand = 'Patrick Hand'
-    Patrick_Hand_SC = 'Patrick Hand SC'
-    Pattaya = 'Pattaya'
-    Patua_One = 'Patua One'
-    Pavanam = 'Pavanam'
-    Paytone_One = 'Paytone One'
-    Peddana = 'Peddana'
-    Peralta = 'Peralta'
-    Permanent_Marker = 'Permanent Marker'
-    Petit_Formal_Script = 'Petit Formal Script'
-    Petrona = 'Petrona'
-    Philosopher = 'Philosopher'
-    Piedra = 'Piedra'
-    Pinyon_Script = 'Pinyon Script'
-    Pirata_One = 'Pirata One'
-    Plaster = 'Plaster'
-    Play = 'Play'
-    Playball = 'Playball'
-    Playfair_Display = 'Playfair Display'
-    Playfair_Display_SC = 'Playfair Display SC'
-    Podkova = 'Podkova'
-    Poiret_One = 'Poiret One'
-    Poller_One = 'Poller One'
-    Poly = 'Poly'
-    Pompiere = 'Pompiere'
-    Pontano_Sans = 'Pontano Sans'
-    Poor_Story = 'Poor Story'
-    Poppins = 'Poppins'
-    Port_Lligat_Sans = 'Port Lligat Sans'
-    Port_Lligat_Slab = 'Port Lligat Slab'
-    Pragati_Narrow = 'Pragati Narrow'
-    Prata = 'Prata'
-    Preahvihear = 'Preahvihear'
-    Press_Start_2P = 'Press Start 2P'
-    Pridi = 'Pridi'
-    Princess_Sofia = 'Princess Sofia'
-    Prociono = 'Prociono'
-    Prompt = 'Prompt'
-    Prosto_One = 'Prosto One'
-    Proza_Libre = 'Proza Libre'
-    Public_Sans = 'Public Sans'
-    Puritan = 'Puritan'
-    Purple_Purse = 'Purple Purse'
-    Quando = 'Quando'
-    Quantico = 'Quantico'
-    Quattrocento = 'Quattrocento'
-    Quattrocento_Sans = 'Quattrocento Sans'
-    Questrial = 'Questrial'
-    Quicksand = 'Quicksand'
-    Quintessential = 'Quintessential'
-    Qwigley = 'Qwigley'
-    Racing_Sans_One = 'Racing Sans One'
-    Radley = 'Radley'
-    Rajdhani = 'Rajdhani'
-    Rakkas = 'Rakkas'
-    Raleway = 'Raleway'
-    Raleway_Dots = 'Raleway Dots'
-    Ramabhadra = 'Ramabhadra'
-    Ramaraja = 'Ramaraja'
-    Rambla = 'Rambla'
-    Rammetto_One = 'Rammetto One'
-    Ranchers = 'Ranchers'
-    Rancho = 'Rancho'
-    Ranga = 'Ranga'
-    Rasa = 'Rasa'
-    Rationale = 'Rationale'
-    Ravi_Prakash = 'Ravi Prakash'
-    Recursive = 'Recursive'
-    Red_Hat_Display = 'Red Hat Display'
-    Red_Hat_Text = 'Red Hat Text'
-    Red_Rose = 'Red Rose'
-    Redressed = 'Redressed'
-    Reem_Kufi = 'Reem Kufi'
-    Reenie_Beanie = 'Reenie Beanie'
-    Revalia = 'Revalia'
-    Rhodium_Libre = 'Rhodium Libre'
-    Ribeye = 'Ribeye'
-    Ribeye_Marrow = 'Ribeye Marrow'
-    Righteous = 'Righteous'
-    Risque = 'Risque'
-    Roboto = 'Roboto'
-    Roboto_Condensed = 'Roboto Condensed'
-    Roboto_Mono = 'Roboto Mono'
-    Roboto_Slab = 'Roboto Slab'
-    Rochester = 'Rochester'
-    Rock_Salt = 'Rock Salt'
-    Rokkitt = 'Rokkitt'
-    Romanesco = 'Romanesco'
-    Ropa_Sans = 'Ropa Sans'
-    Rosario = 'Rosario'
-    Rosarivo = 'Rosarivo'
-    Rouge_Script = 'Rouge Script'
-    Rowdies = 'Rowdies'
-    Rozha_One = 'Rozha One'
-    Rubik = 'Rubik'
-    Rubik_Mono_One = 'Rubik Mono One'
-    Ruda = 'Ruda'
-    Rufina = 'Rufina'
-    Ruge_Boogie = 'Ruge Boogie'
-    Ruluko = 'Ruluko'
-    Rum_Raisin = 'Rum Raisin'
-    Ruslan_Display = 'Ruslan Display'
-    Russo_One = 'Russo One'
-    Ruthie = 'Ruthie'
-    Rye = 'Rye'
-    Sacramento = 'Sacramento'
-    Sahitya = 'Sahitya'
-    Sail = 'Sail'
-    Saira = 'Saira'
-    Saira_Condensed = 'Saira Condensed'
-    Saira_Extra_Condensed = 'Saira Extra Condensed'
-    Saira_Semi_Condensed = 'Saira Semi Condensed'
-    Saira_Stencil_One = 'Saira Stencil One'
-    Salsa = 'Salsa'
-    Sanchez = 'Sanchez'
-    Sancreek = 'Sancreek'
-    Sansita = 'Sansita'
-    Sarabun = 'Sarabun'
-    Sarala = 'Sarala'
-    Sarina = 'Sarina'
-    Sarpanch = 'Sarpanch'
-    Satisfy = 'Satisfy'
-    Sawarabi_Gothic = 'Sawarabi Gothic'
-    Sawarabi_Mincho = 'Sawarabi Mincho'
-    Scada = 'Scada'
-    Scheherazade = 'Scheherazade'
-    Schoolbell = 'Schoolbell'
-    Scope_One = 'Scope One'
-    Seaweed_Script = 'Seaweed Script'
-    Secular_One = 'Secular One'
-    Sedgwick_Ave = 'Sedgwick Ave'
-    Sedgwick_Ave_Display = 'Sedgwick Ave Display'
-    Sen = 'Sen'
-    Sevillana = 'Sevillana'
-    Seymour_One = 'Seymour One'
-    Shadows_Into_Light = 'Shadows Into Light'
-    Shadows_Into_Light_Two = 'Shadows Into Light Two'
-    Shanti = 'Shanti'
-    Share = 'Share'
-    Share_Tech = 'Share Tech'
-    Share_Tech_Mono = 'Share Tech Mono'
-    Shojumaru = 'Shojumaru'
-    Short_Stack = 'Short Stack'
-    Shrikhand = 'Shrikhand'
-    Siemreap = 'Siemreap'
-    Sigmar_One = 'Sigmar One'
-    Signika = 'Signika'
-    Signika_Negative = 'Signika Negative'
-    Simonetta = 'Simonetta'
-    Single_Day = 'Single Day'
-    Sintony = 'Sintony'
-    Sirin_Stencil = 'Sirin Stencil'
-    Six_Caps = 'Six Caps'
-    Skranji = 'Skranji'
-    Slabo_13px = 'Slabo 13px'
-    Slabo_27px = 'Slabo 27px'
-    Slackey = 'Slackey'
-    Smokum = 'Smokum'
-    Smythe = 'Smythe'
-    Sniglet = 'Sniglet'
-    Snippet = 'Snippet'
-    Snowburst_One = 'Snowburst One'
-    Sofadi_One = 'Sofadi One'
-    Sofia = 'Sofia'
-    Solway = 'Solway'
-    Song_Myung = 'Song Myung'
-    Sonsie_One = 'Sonsie One'
-    Sora = 'Sora'
-    Sorts_Mill_Goudy = 'Sorts Mill Goudy'
-    Source_Code_Pro = 'Source Code Pro'
-    Source_Sans_Pro = 'Source Sans Pro'
-    Source_Serif_Pro = 'Source Serif Pro'
-    Space_Mono = 'Space Mono'
-    Spartan = 'Spartan'
-    Special_Elite = 'Special Elite'
-    Spectral = 'Spectral'
-    Spectral_SC = 'Spectral SC'
-    Spicy_Rice = 'Spicy Rice'
-    Spinnaker = 'Spinnaker'
-    Spirax = 'Spirax'
-    Squada_One = 'Squada One'
-    Sree_Krushnadevaraya = 'Sree Krushnadevaraya'
-    Sriracha = 'Sriracha'
-    Srisakdi = 'Srisakdi'
-    Staatliches = 'Staatliches'
-    Stalemate = 'Stalemate'
-    Stalinist_One = 'Stalinist One'
-    Stardos_Stencil = 'Stardos Stencil'
-    Stint_Ultra_Condensed = 'Stint Ultra Condensed'
-    Stint_Ultra_Expanded = 'Stint Ultra Expanded'
-    Stoke = 'Stoke'
-    Strait = 'Strait'
-    Stylish = 'Stylish'
-    Sue_Ellen_Francisco = 'Sue Ellen Francisco'
-    Suez_One = 'Suez One'
-    Sulphur_Point = 'Sulphur Point'
-    Sumana = 'Sumana'
-    Sunflower = 'Sunflower'
-    Sunshiney = 'Sunshiney'
-    Supermercado_One = 'Supermercado One'
-    Sura = 'Sura'
-    Suranna = 'Suranna'
-    Suravaram = 'Suravaram'
-    Suwannaphum = 'Suwannaphum'
-    Swanky_and_Moo_Moo = 'Swanky and Moo Moo'
-    Syncopate = 'Syncopate'
-    Tajawal = 'Tajawal'
-    Tangerine = 'Tangerine'
-    Taprom = 'Taprom'
-    Tauri = 'Tauri'
-    Taviraj = 'Taviraj'
-    Teko = 'Teko'
-    Telex = 'Telex'
-    Tenali_Ramakrishna = 'Tenali Ramakrishna'
-    Tenor_Sans = 'Tenor Sans'
-    Text_Me_One = 'Text Me One'
-    Thasadith = 'Thasadith'
-    The_Girl_Next_Door = 'The Girl Next Door'
-    Tienne = 'Tienne'
-    Tillana = 'Tillana'
-    Timmana = 'Timmana'
-    Tinos = 'Tinos'
-    Titan_One = 'Titan One'
-    Titillium_Web = 'Titillium Web'
-    Tomorrow = 'Tomorrow'
-    Trade_Winds = 'Trade Winds'
-    Trirong = 'Trirong'
-    Trocchi = 'Trocchi'
-    Trochut = 'Trochut'
-    Trykker = 'Trykker'
-    Tulpen_One = 'Tulpen One'
-    Turret_Road = 'Turret Road'
-    Ubuntu = 'Ubuntu'
-    Ubuntu_Condensed = 'Ubuntu Condensed'
-    Ubuntu_Mono = 'Ubuntu Mono'
-    Ultra = 'Ultra'
-    Uncial_Antiqua = 'Uncial Antiqua'
-    Underdog = 'Underdog'
-    Unica_One = 'Unica One'
-    UnifrakturCook = 'UnifrakturCook'
-    UnifrakturMaguntia = 'UnifrakturMaguntia'
-    Unkempt = 'Unkempt'
-    Unlock = 'Unlock'
-    Unna = 'Unna'
-    VT323 = 'VT323'
-    Vampiro_One = 'Vampiro One'
-    Varela = 'Varela'
-    Varela_Round = 'Varela Round'
-    Varta = 'Varta'
-    Vast_Shadow = 'Vast Shadow'
-    Vesper_Libre = 'Vesper Libre'
-    Viaoda_Libre = 'Viaoda Libre'
-    Vibes = 'Vibes'
-    Vibur = 'Vibur'
-    Vidaloka = 'Vidaloka'
-    Viga = 'Viga'
-    Voces = 'Voces'
-    Volkhov = 'Volkhov'
-    Vollkorn = 'Vollkorn'
-    Vollkorn_SC = 'Vollkorn SC'
-    Voltaire = 'Voltaire'
-    Waiting_for_the_Sunrise = 'Waiting for the Sunrise'
-    Wallpoet = 'Wallpoet'
-    Walter_Turncoat = 'Walter Turncoat'
-    Warnes = 'Warnes'
-    Wellfleet = 'Wellfleet'
-    Wendy_One = 'Wendy One'
-    Wire_One = 'Wire One'
-    Work_Sans = 'Work Sans'
-    Yanone_Kaffeesatz = 'Yanone Kaffeesatz'
-    Yantramanav = 'Yantramanav'
-    Yatra_One = 'Yatra One'
-    Yellowtail = 'Yellowtail'
-    Yeon_Sung = 'Yeon Sung'
-    Yeseva_One = 'Yeseva One'
-    Yesteryear = 'Yesteryear'
-    Yrsa = 'Yrsa'
-    ZCOOL_KuaiLe = 'ZCOOL KuaiLe'
-    ZCOOL_QingKe_HuangYou = 'ZCOOL QingKe HuangYou'
-    ZCOOL_XiaoWei = 'ZCOOL XiaoWei'
-    Zeyada = 'Zeyada'
-    Zhi_Mang_Xing = 'Zhi Mang Xing'
-    Zilla_Slab = 'Zilla Slab'
-    Zilla_Slab_Highlight = 'Zilla Slab Highlight'
-
-    def __str__(self):
-        return '{0}'.format(self.value)
-
-
-class GradientType(Enum):
-    linear = 'linear',
-    radial = 'radial'
-
-    def __str__(self):
-        return '{0}'.format(self.value)
-
-class FontWeightType(Enum):
-    light = 300
-    normal = 400
-    bold = 700
-
-    def __str__(self):
-        return '{0}'.format(self.value)
+from enum import Enum
+
+
+class HashtagPosition(Enum):
+    auto = 'auto'
+    end = 'end'
+
+    def __str__(self):
+        return '{0}'.format(self.value)
+
+
+class AnimationType(Enum):
+    none = 'none'
+    rays = 'rays'
+    glint = 'glint'
+    circle = 'circle'
+
+    def __str__(self):
+        return '{0}'.format(self.value)
+
+
+class FontList(Enum):
+    ABeeZee = 'ABeeZee'
+    Abel = 'Abel'
+    Abhaya_Libre = 'Abhaya Libre'
+    Abril_Fatface = 'Abril Fatface'
+    Aclonica = 'Aclonica'
+    Acme = 'Acme'
+    Actor = 'Actor'
+    Adamina = 'Adamina'
+    Advent_Pro = 'Advent Pro'
+    Aguafina_Script = 'Aguafina Script'
+    Akronim = 'Akronim'
+    Aladin = 'Aladin'
+    Alata = 'Alata'
+    Alatsi = 'Alatsi'
+    Aldrich = 'Aldrich'
+    Alef = 'Alef'
+    Alegreya = 'Alegreya'
+    Alegreya_SC = 'Alegreya SC'
+    Alegreya_Sans = 'Alegreya Sans'
+    Alegreya_Sans_SC = 'Alegreya Sans SC'
+    Aleo = 'Aleo'
+    Alex_Brush = 'Alex Brush'
+    Alfa_Slab_One = 'Alfa Slab One'
+    Alice = 'Alice'
+    Alike = 'Alike'
+    Alike_Angular = 'Alike Angular'
+    Allan = 'Allan'
+    Allerta = 'Allerta'
+    Allerta_Stencil = 'Allerta Stencil'
+    Allura = 'Allura'
+    Almarai = 'Almarai'
+    Almendra = 'Almendra'
+    Almendra_Display = 'Almendra Display'
+    Almendra_SC = 'Almendra SC'
+    Amarante = 'Amarante'
+    Amaranth = 'Amaranth'
+    Amatic_SC = 'Amatic SC'
+    Amethysta = 'Amethysta'
+    Amiko = 'Amiko'
+    Amiri = 'Amiri'
+    Amita = 'Amita'
+    Anaheim = 'Anaheim'
+    Andada = 'Andada'
+    Andika = 'Andika'
+    Angkor = 'Angkor'
+    Annie_Use_Your_Telescope = 'Annie Use Your Telescope'
+    Anonymous_Pro = 'Anonymous Pro'
+    Antic = 'Antic'
+    Antic_Didone = 'Antic Didone'
+    Antic_Slab = 'Antic Slab'
+    Anton = 'Anton'
+    Arapey = 'Arapey'
+    Arbutus = 'Arbutus'
+    Arbutus_Slab = 'Arbutus Slab'
+    Architects_Daughter = 'Architects Daughter'
+    Archivo = 'Archivo'
+    Archivo_Black = 'Archivo Black'
+    Archivo_Narrow = 'Archivo Narrow'
+    Aref_Ruqaa = 'Aref Ruqaa'
+    Arima_Madurai = 'Arima Madurai'
+    Arimo = 'Arimo'
+    Arizonia = 'Arizonia'
+    Armata = 'Armata'
+    Arsenal = 'Arsenal'
+    Artifika = 'Artifika'
+    Arvo = 'Arvo'
+    Arya = 'Arya'
+    Asap = 'Asap'
+    Asap_Condensed = 'Asap Condensed'
+    Asar = 'Asar'
+    Asset = 'Asset'
+    Assistant = 'Assistant'
+    Astloch = 'Astloch'
+    Asul = 'Asul'
+    Athiti = 'Athiti'
+    Atma = 'Atma'
+    Atomic_Age = 'Atomic Age'
+    Aubrey = 'Aubrey'
+    Audiowide = 'Audiowide'
+    Autour_One = 'Autour One'
+    Average = 'Average'
+    Average_Sans = 'Average Sans'
+    Averia_Gruesa_Libre = 'Averia Gruesa Libre'
+    Averia_Libre = 'Averia Libre'
+    Averia_Sans_Libre = 'Averia Sans Libre'
+    Averia_Serif_Libre = 'Averia Serif Libre'
+    B612 = 'B612'
+    B612_Mono = 'B612 Mono'
+    Bad_Script = 'Bad Script'
+    Bahiana = 'Bahiana'
+    Bahianita = 'Bahianita'
+    Bai_Jamjuree = 'Bai Jamjuree'
+    Baloo_2 = 'Baloo 2'
+    Baloo_Bhai_2 = 'Baloo Bhai 2'
+    Baloo_Bhaina_2 = 'Baloo Bhaina 2'
+    Baloo_Chettan_2 = 'Baloo Chettan 2'
+    Baloo_Da_2 = 'Baloo Da 2'
+    Baloo_Paaji_2 = 'Baloo Paaji 2'
+    Baloo_Tamma_2 = 'Baloo Tamma 2'
+    Baloo_Tammudu_2 = 'Baloo Tammudu 2'
+    Baloo_Thambi_2 = 'Baloo Thambi 2'
+    Balsamiq_Sans = 'Balsamiq Sans'
+    Balthazar = 'Balthazar'
+    Bangers = 'Bangers'
+    Barlow = 'Barlow'
+    Barlow_Condensed = 'Barlow Condensed'
+    Barlow_Semi_Condensed = 'Barlow Semi Condensed'
+    Barriecito = 'Barriecito'
+    Barrio = 'Barrio'
+    Basic = 'Basic'
+    Baskervville = 'Baskervville'
+    Battambang = 'Battambang'
+    Baumans = 'Baumans'
+    Bayon = 'Bayon'
+    Be_Vietnam = 'Be Vietnam'
+    Bebas_Neue = 'Bebas Neue'
+    Belgrano = 'Belgrano'
+    Bellefair = 'Bellefair'
+    Belleza = 'Belleza'
+    Bellota = 'Bellota'
+    Bellota_Text = 'Bellota Text'
+    BenchNine = 'BenchNine'
+    Bentham = 'Bentham'
+    Berkshire_Swash = 'Berkshire Swash'
+    Beth_Ellen = 'Beth Ellen'
+    Bevan = 'Bevan'
+    Big_Shoulders_Display = 'Big Shoulders Display'
+    Big_Shoulders_Text = 'Big Shoulders Text'
+    Bigelow_Rules = 'Bigelow Rules'
+    Bigshot_One = 'Bigshot One'
+    Bilbo = 'Bilbo'
+    Bilbo_Swash_Caps = 'Bilbo Swash Caps'
+    BioRhyme = 'BioRhyme'
+    BioRhyme_Expanded = 'BioRhyme Expanded'
+    Biryani = 'Biryani'
+    Bitter = 'Bitter'
+    Black_And_White_Picture = 'Black And White Picture'
+    Black_Han_Sans = 'Black Han Sans'
+    Black_Ops_One = 'Black Ops One'
+    Blinker = 'Blinker'
+    Bokor = 'Bokor'
+    Bonbon = 'Bonbon'
+    Boogaloo = 'Boogaloo'
+    Bowlby_One = 'Bowlby One'
+    Bowlby_One_SC = 'Bowlby One SC'
+    Brawler = 'Brawler'
+    Bree_Serif = 'Bree Serif'
+    Bubblegum_Sans = 'Bubblegum Sans'
+    Bubbler_One = 'Bubbler One'
+    Buda = 'Buda'
+    Buenard = 'Buenard'
+    Bungee = 'Bungee'
+    Bungee_Hairline = 'Bungee Hairline'
+    Bungee_Inline = 'Bungee Inline'
+    Bungee_Outline = 'Bungee Outline'
+    Bungee_Shade = 'Bungee Shade'
+    Butcherman = 'Butcherman'
+    Butterfly_Kids = 'Butterfly Kids'
+    Cabin = 'Cabin'
+    Cabin_Condensed = 'Cabin Condensed'
+    Cabin_Sketch = 'Cabin Sketch'
+    Caesar_Dressing = 'Caesar Dressing'
+    Cagliostro = 'Cagliostro'
+    Cairo = 'Cairo'
+    Caladea = 'Caladea'
+    Calistoga = 'Calistoga'
+    Calligraffitti = 'Calligraffitti'
+    Cambay = 'Cambay'
+    Cambo = 'Cambo'
+    Candal = 'Candal'
+    Cantarell = 'Cantarell'
+    Cantata_One = 'Cantata One'
+    Cantora_One = 'Cantora One'
+    Capriola = 'Capriola'
+    Cardo = 'Cardo'
+    Carme = 'Carme'
+    Carrois_Gothic = 'Carrois Gothic'
+    Carrois_Gothic_SC = 'Carrois Gothic SC'
+    Carter_One = 'Carter One'
+    Catamaran = 'Catamaran'
+    Caudex = 'Caudex'
+    Caveat = 'Caveat'
+    Caveat_Brush = 'Caveat Brush'
+    Cedarville_Cursive = 'Cedarville Cursive'
+    Ceviche_One = 'Ceviche One'
+    Chakra_Petch = 'Chakra Petch'
+    Changa = 'Changa'
+    Changa_One = 'Changa One'
+    Chango = 'Chango'
+    Charm = 'Charm'
+    Charmonman = 'Charmonman'
+    Chathura = 'Chathura'
+    Chau_Philomene_One = 'Chau Philomene One'
+    Chela_One = 'Chela One'
+    Chelsea_Market = 'Chelsea Market'
+    Chenla = 'Chenla'
+    Cherry_Cream_Soda = 'Cherry Cream Soda'
+    Cherry_Swash = 'Cherry Swash'
+    Chewy = 'Chewy'
+    Chicle = 'Chicle'
+    Chilanka = 'Chilanka'
+    Chivo = 'Chivo'
+    Chonburi = 'Chonburi'
+    Cinzel = 'Cinzel'
+    Cinzel_Decorative = 'Cinzel Decorative'
+    Clicker_Script = 'Clicker Script'
+    Coda = 'Coda'
+    Coda_Caption = 'Coda Caption'
+    Codystar = 'Codystar'
+    Coiny = 'Coiny'
+    Combo = 'Combo'
+    Comfortaa = 'Comfortaa'
+    Comic_Neue = 'Comic Neue'
+    Coming_Soon = 'Coming Soon'
+    Concert_One = 'Concert One'
+    Condiment = 'Condiment'
+    Content = 'Content'
+    Contrail_One = 'Contrail One'
+    Convergence = 'Convergence'
+    Cookie = 'Cookie'
+    Copse = 'Copse'
+    Corben = 'Corben'
+    Cormorant = 'Cormorant'
+    Cormorant_Garamond = 'Cormorant Garamond'
+    Cormorant_Infant = 'Cormorant Infant'
+    Cormorant_SC = 'Cormorant SC'
+    Cormorant_Unicase = 'Cormorant Unicase'
+    Cormorant_Upright = 'Cormorant Upright'
+    Courgette = 'Courgette'
+    Courier_Prime = 'Courier Prime'
+    Cousine = 'Cousine'
+    Coustard = 'Coustard'
+    Covered_By_Your_Grace = 'Covered By Your Grace'
+    Crafty_Girls = 'Crafty Girls'
+    Creepster = 'Creepster'
+    Crete_Round = 'Crete Round'
+    Crimson_Pro = 'Crimson Pro'
+    Crimson_Text = 'Crimson Text'
+    Croissant_One = 'Croissant One'
+    Crushed = 'Crushed'
+    Cuprum = 'Cuprum'
+    Cute_Font = 'Cute Font'
+    Cutive = 'Cutive'
+    Cutive_Mono = 'Cutive Mono'
+    DM_Mono = 'DM Mono'
+    DM_Sans = 'DM Sans'
+    DM_Serif_Display = 'DM Serif Display'
+    DM_Serif_Text = 'DM Serif Text'
+    Damion = 'Damion'
+    Dancing_Script = 'Dancing Script'
+    Dangrek = 'Dangrek'
+    Darker_Grotesque = 'Darker Grotesque'
+    David_Libre = 'David Libre'
+    Dawning_of_a_New_Day = 'Dawning of a New Day'
+    Days_One = 'Days One'
+    Dekko = 'Dekko'
+    Delius = 'Delius'
+    Delius_Swash_Caps = 'Delius Swash Caps'
+    Delius_Unicase = 'Delius Unicase'
+    Della_Respira = 'Della Respira'
+    Denk_One = 'Denk One'
+    Devonshire = 'Devonshire'
+    Dhurjati = 'Dhurjati'
+    Didact_Gothic = 'Didact Gothic'
+    Diplomata = 'Diplomata'
+    Diplomata_SC = 'Diplomata SC'
+    Do_Hyeon = 'Do Hyeon'
+    Dokdo = 'Dokdo'
+    Domine = 'Domine'
+    Donegal_One = 'Donegal One'
+    Doppio_One = 'Doppio One'
+    Dorsa = 'Dorsa'
+    Dosis = 'Dosis'
+    Dr_Sugiyama = 'Dr Sugiyama'
+    Duru_Sans = 'Duru Sans'
+    Dynalight = 'Dynalight'
+    EB_Garamond = 'EB Garamond'
+    Eagle_Lake = 'Eagle Lake'
+    East_Sea_Dokdo = 'East Sea Dokdo'
+    Eater = 'Eater'
+    Economica = 'Economica'
+    Eczar = 'Eczar'
+    El_Messiri = 'El Messiri'
+    Electrolize = 'Electrolize'
+    Elsie = 'Elsie'
+    Elsie_Swash_Caps = 'Elsie Swash Caps'
+    Emblema_One = 'Emblema One'
+    Emilys_Candy = 'Emilys Candy'
+    Encode_Sans = 'Encode Sans'
+    Encode_Sans_Condensed = 'Encode Sans Condensed'
+    Encode_Sans_Expanded = 'Encode Sans Expanded'
+    Encode_Sans_Semi_Condensed = 'Encode Sans Semi Condensed'
+    Encode_Sans_Semi_Expanded = 'Encode Sans Semi Expanded'
+    Engagement = 'Engagement'
+    Englebert = 'Englebert'
+    Enriqueta = 'Enriqueta'
+    Epilogue = 'Epilogue'
+    Erica_One = 'Erica One'
+    Esteban = 'Esteban'
+    Euphoria_Script = 'Euphoria Script'
+    Ewert = 'Ewert'
+    Exo = 'Exo'
+    Exo_2 = 'Exo 2'
+    Expletus_Sans = 'Expletus Sans'
+    Fahkwang = 'Fahkwang'
+    Fanwood_Text = 'Fanwood Text'
+    Farro = 'Farro'
+    Farsan = 'Farsan'
+    Fascinate = 'Fascinate'
+    Fascinate_Inline = 'Fascinate Inline'
+    Faster_One = 'Faster One'
+    Fasthand = 'Fasthand'
+    Fauna_One = 'Fauna One'
+    Faustina = 'Faustina'
+    Federant = 'Federant'
+    Federo = 'Federo'
+    Felipa = 'Felipa'
+    Fenix = 'Fenix'
+    Finger_Paint = 'Finger Paint'
+    Fira_Code = 'Fira Code'
+    Fira_Mono = 'Fira Mono'
+    Fira_Sans = 'Fira Sans'
+    Fira_Sans_Condensed = 'Fira Sans Condensed'
+    Fira_Sans_Extra_Condensed = 'Fira Sans Extra Condensed'
+    Fjalla_One = 'Fjalla One'
+    Fjord_One = 'Fjord One'
+    Flamenco = 'Flamenco'
+    Flavors = 'Flavors'
+    Fondamento = 'Fondamento'
+    Fontdiner_Swanky = 'Fontdiner Swanky'
+    Forum = 'Forum'
+    Francois_One = 'Francois One'
+    Frank_Ruhl_Libre = 'Frank Ruhl Libre'
+    Freckle_Face = 'Freckle Face'
+    Fredericka_the_Great = 'Fredericka the Great'
+    Fredoka_One = 'Fredoka One'
+    Freehand = 'Freehand'
+    Fresca = 'Fresca'
+    Frijole = 'Frijole'
+    Fruktur = 'Fruktur'
+    Fugaz_One = 'Fugaz One'
+    GFS_Didot = 'GFS Didot'
+    GFS_Neohellenic = 'GFS Neohellenic'
+    Gabriela = 'Gabriela'
+    Gaegu = 'Gaegu'
+    Gafata = 'Gafata'
+    Galada = 'Galada'
+    Galdeano = 'Galdeano'
+    Galindo = 'Galindo'
+    Gamja_Flower = 'Gamja Flower'
+    Gayathri = 'Gayathri'
+    Gelasio = 'Gelasio'
+    Gentium_Basic = 'Gentium Basic'
+    Gentium_Book_Basic = 'Gentium Book Basic'
+    Geo = 'Geo'
+    Geostar = 'Geostar'
+    Geostar_Fill = 'Geostar Fill'
+    Germania_One = 'Germania One'
+    Gidugu = 'Gidugu'
+    Gilda_Display = 'Gilda Display'
+    Girassol = 'Girassol'
+    Give_You_Glory = 'Give You Glory'
+    Glass_Antiqua = 'Glass Antiqua'
+    Glegoo = 'Glegoo'
+    Gloria_Hallelujah = 'Gloria Hallelujah'
+    Goblin_One = 'Goblin One'
+    Gochi_Hand = 'Gochi Hand'
+    Gorditas = 'Gorditas'
+    Gothic_A1 = 'Gothic A1'
+    Gotu = 'Gotu'
+    Goudy_Bookletter_1911 = 'Goudy Bookletter 1911'
+    Graduate = 'Graduate'
+    Grand_Hotel = 'Grand Hotel'
+    Gravitas_One = 'Gravitas One'
+    Great_Vibes = 'Great Vibes'
+    Grenze = 'Grenze'
+    Grenze_Gotisch = 'Grenze Gotisch'
+    Griffy = 'Griffy'
+    Gruppo = 'Gruppo'
+    Gudea = 'Gudea'
+    Gugi = 'Gugi'
+    Gupter = 'Gupter'
+    Gurajada = 'Gurajada'
+    Habibi = 'Habibi'
+    Halant = 'Halant'
+    Hammersmith_One = 'Hammersmith One'
+    Hanalei = 'Hanalei'
+    Hanalei_Fill = 'Hanalei Fill'
+    Handlee = 'Handlee'
+    Hanuman = 'Hanuman'
+    Happy_Monkey = 'Happy Monkey'
+    Harmattan = 'Harmattan'
+    Headland_One = 'Headland One'
+    Heebo = 'Heebo'
+    Henny_Penny = 'Henny Penny'
+    Hepta_Slab = 'Hepta Slab'
+    Herr_Von_Muellerhoff = 'Herr Von Muellerhoff'
+    Hi_Melody = 'Hi Melody'
+    Hind = 'Hind'
+    Hind_Guntur = 'Hind Guntur'
+    Hind_Madurai = 'Hind Madurai'
+    Hind_Siliguri = 'Hind Siliguri'
+    Hind_Vadodara = 'Hind Vadodara'
+    Holtwood_One_SC = 'Holtwood One SC'
+    Homemade_Apple = 'Homemade Apple'
+    Homenaje = 'Homenaje'
+    IBM_Plex_Mono = 'IBM Plex Mono'
+    IBM_Plex_Sans = 'IBM Plex Sans'
+    IBM_Plex_Sans_Condensed = 'IBM Plex Sans Condensed'
+    IBM_Plex_Serif = 'IBM Plex Serif'
+    IM_Fell_DW_Pica = 'IM Fell DW Pica'
+    IM_Fell_DW_Pica_SC = 'IM Fell DW Pica SC'
+    IM_Fell_Double_Pica = 'IM Fell Double Pica'
+    IM_Fell_Double_Pica_SC = 'IM Fell Double Pica SC'
+    IM_Fell_English = 'IM Fell English'
+    IM_Fell_English_SC = 'IM Fell English SC'
+    IM_Fell_French_Canon = 'IM Fell French Canon'
+    IM_Fell_French_Canon_SC = 'IM Fell French Canon SC'
+    IM_Fell_Great_Primer = 'IM Fell Great Primer'
+    IM_Fell_Great_Primer_SC = 'IM Fell Great Primer SC'
+    Ibarra_Real_Nova = 'Ibarra Real Nova'
+    Iceberg = 'Iceberg'
+    Iceland = 'Iceland'
+    Imprima = 'Imprima'
+    Inconsolata = 'Inconsolata'
+    Inder = 'Inder'
+    Indie_Flower = 'Indie Flower'
+    Inika = 'Inika'
+    Inknut_Antiqua = 'Inknut Antiqua'
+    Inria_Sans = 'Inria Sans'
+    Inria_Serif = 'Inria Serif'
+    Inter = 'Inter'
+    Irish_Grover = 'Irish Grover'
+    Istok_Web = 'Istok Web'
+    Italiana = 'Italiana'
+    Italianno = 'Italianno'
+    Itim = 'Itim'
+    Jacques_Francois = 'Jacques Francois'
+    Jacques_Francois_Shadow = 'Jacques Francois Shadow'
+    Jaldi = 'Jaldi'
+    Jim_Nightshade = 'Jim Nightshade'
+    Jockey_One = 'Jockey One'
+    Jolly_Lodger = 'Jolly Lodger'
+    Jomhuria = 'Jomhuria'
+    Jomolhari = 'Jomolhari'
+    Josefin_Sans = 'Josefin Sans'
+    Josefin_Slab = 'Josefin Slab'
+    Jost = 'Jost'
+    Joti_One = 'Joti One'
+    Jua = 'Jua'
+    Judson = 'Judson'
+    Julee = 'Julee'
+    Julius_Sans_One = 'Julius Sans One'
+    Junge = 'Junge'
+    Jura = 'Jura'
+    Just_Another_Hand = 'Just Another Hand'
+    Just_Me_Again_Down_Here = 'Just Me Again Down Here'
+    K2D = 'K2D'
+    Kadwa = 'Kadwa'
+    Kalam = 'Kalam'
+    Kameron = 'Kameron'
+    Kanit = 'Kanit'
+    Kantumruy = 'Kantumruy'
+    Karla = 'Karla'
+    Karma = 'Karma'
+    Katibeh = 'Katibeh'
+    Kaushan_Script = 'Kaushan Script'
+    Kavivanar = 'Kavivanar'
+    Kavoon = 'Kavoon'
+    Kdam_Thmor = 'Kdam Thmor'
+    Keania_One = 'Keania One'
+    Kelly_Slab = 'Kelly Slab'
+    Kenia = 'Kenia'
+    Khand = 'Khand'
+    Khmer = 'Khmer'
+    Khula = 'Khula'
+    Kirang_Haerang = 'Kirang Haerang'
+    Kite_One = 'Kite One'
+    Knewave = 'Knewave'
+    KoHo = 'KoHo'
+    Kodchasan = 'Kodchasan'
+    Kosugi = 'Kosugi'
+    Kosugi_Maru = 'Kosugi Maru'
+    Kotta_One = 'Kotta One'
+    Koulen = 'Koulen'
+    Kranky = 'Kranky'
+    Kreon = 'Kreon'
+    Kristi = 'Kristi'
+    Krona_One = 'Krona One'
+    Krub = 'Krub'
+    Kulim_Park = 'Kulim Park'
+    Kumar_One = 'Kumar One'
+    Kumar_One_Outline = 'Kumar One Outline'
+    Kurale = 'Kurale'
+    La_Belle_Aurore = 'La Belle Aurore'
+    Lacquer = 'Lacquer'
+    Laila = 'Laila'
+    Lakki_Reddy = 'Lakki Reddy'
+    Lalezar = 'Lalezar'
+    Lancelot = 'Lancelot'
+    Lateef = 'Lateef'
+    Lato = 'Lato'
+    League_Script = 'League Script'
+    Leckerli_One = 'Leckerli One'
+    Ledger = 'Ledger'
+    Lekton = 'Lekton'
+    Lemon = 'Lemon'
+    Lemonada = 'Lemonada'
+    Lexend_Deca = 'Lexend Deca'
+    Lexend_Exa = 'Lexend Exa'
+    Lexend_Giga = 'Lexend Giga'
+    Lexend_Mega = 'Lexend Mega'
+    Lexend_Peta = 'Lexend Peta'
+    Lexend_Tera = 'Lexend Tera'
+    Lexend_Zetta = 'Lexend Zetta'
+    Libre_Barcode_128 = 'Libre Barcode 128'
+    Libre_Barcode_128_Text = 'Libre Barcode 128 Text'
+    Libre_Barcode_39 = 'Libre Barcode 39'
+    Libre_Barcode_39_Extended = 'Libre Barcode 39 Extended'
+    Libre_Barcode_39_Extended_Text = 'Libre Barcode 39 Extended Text'
+    Libre_Barcode_39_Text = 'Libre Barcode 39 Text'
+    Libre_Baskerville = 'Libre Baskerville'
+    Libre_Caslon_Display = 'Libre Caslon Display'
+    Libre_Caslon_Text = 'Libre Caslon Text'
+    Libre_Franklin = 'Libre Franklin'
+    Life_Savers = 'Life Savers'
+    Lilita_One = 'Lilita One'
+    Lily_Script_One = 'Lily Script One'
+    Limelight = 'Limelight'
+    Linden_Hill = 'Linden Hill'
+    Literata = 'Literata'
+    Liu_Jian_Mao_Cao = 'Liu Jian Mao Cao'
+    Livvic = 'Livvic'
+    Lobster = 'Lobster'
+    Lobster_Two = 'Lobster Two'
+    Londrina_Outline = 'Londrina Outline'
+    Londrina_Shadow = 'Londrina Shadow'
+    Londrina_Sketch = 'Londrina Sketch'
+    Londrina_Solid = 'Londrina Solid'
+    Long_Cang = 'Long Cang'
+    Lora = 'Lora'
+    Love_Ya_Like_A_Sister = 'Love Ya Like A Sister'
+    Loved_by_the_King = 'Loved by the King'
+    Lovers_Quarrel = 'Lovers Quarrel'
+    Luckiest_Guy = 'Luckiest Guy'
+    Lusitana = 'Lusitana'
+    Lustria = 'Lustria'
+    M_PLUS_1p = 'M PLUS 1p'
+    M_PLUS_Rounded_1c = 'M PLUS Rounded 1c'
+    Ma_Shan_Zheng = 'Ma Shan Zheng'
+    Macondo = 'Macondo'
+    Macondo_Swash_Caps = 'Macondo Swash Caps'
+    Mada = 'Mada'
+    Magra = 'Magra'
+    Maiden_Orange = 'Maiden Orange'
+    Maitree = 'Maitree'
+    Major_Mono_Display = 'Major Mono Display'
+    Mako = 'Mako'
+    Mali = 'Mali'
+    Mallanna = 'Mallanna'
+    Mandali = 'Mandali'
+    Manjari = 'Manjari'
+    Manrope = 'Manrope'
+    Mansalva = 'Mansalva'
+    Manuale = 'Manuale'
+    Marcellus = 'Marcellus'
+    Marcellus_SC = 'Marcellus SC'
+    Marck_Script = 'Marck Script'
+    Margarine = 'Margarine'
+    Markazi_Text = 'Markazi Text'
+    Marko_One = 'Marko One'
+    Marmelad = 'Marmelad'
+    Martel = 'Martel'
+    Martel_Sans = 'Martel Sans'
+    Marvel = 'Marvel'
+    Mate = 'Mate'
+    Mate_SC = 'Mate SC'
+    Maven_Pro = 'Maven Pro'
+    McLaren = 'McLaren'
+    Meddon = 'Meddon'
+    MedievalSharp = 'MedievalSharp'
+    Medula_One = 'Medula One'
+    Meera_Inimai = 'Meera Inimai'
+    Megrim = 'Megrim'
+    Meie_Script = 'Meie Script'
+    Merienda = 'Merienda'
+    Merienda_One = 'Merienda One'
+    Merriweather = 'Merriweather'
+    Merriweather_Sans = 'Merriweather Sans'
+    Metal = 'Metal'
+    Metal_Mania = 'Metal Mania'
+    Metamorphous = 'Metamorphous'
+    Metrophobic = 'Metrophobic'
+    Michroma = 'Michroma'
+    Milonga = 'Milonga'
+    Miltonian = 'Miltonian'
+    Miltonian_Tattoo = 'Miltonian Tattoo'
+    Mina = 'Mina'
+    Miniver = 'Miniver'
+    Miriam_Libre = 'Miriam Libre'
+    Mirza = 'Mirza'
+    Miss_Fajardose = 'Miss Fajardose'
+    Mitr = 'Mitr'
+    Modak = 'Modak'
+    Modern_Antiqua = 'Modern Antiqua'
+    Mogra = 'Mogra'
+    Molengo = 'Molengo'
+    Molle = 'Molle'
+    Monda = 'Monda'
+    Monofett = 'Monofett'
+    Monoton = 'Monoton'
+    Monsieur_La_Doulaise = 'Monsieur La Doulaise'
+    Montaga = 'Montaga'
+    Montez = 'Montez'
+    Montserrat = 'Montserrat'
+    Montserrat_Alternates = 'Montserrat Alternates'
+    Montserrat_Subrayada = 'Montserrat Subrayada'
+    Moul = 'Moul'
+    Moulpali = 'Moulpali'
+    Mountains_of_Christmas = 'Mountains of Christmas'
+    Mouse_Memoirs = 'Mouse Memoirs'
+    Mr_Bedfort = 'Mr Bedfort'
+    Mr_Dafoe = 'Mr Dafoe'
+    Mr_De_Haviland = 'Mr De Haviland'
+    Mrs_Saint_Delafield = 'Mrs Saint Delafield'
+    Mrs_Sheppards = 'Mrs Sheppards'
+    Mukta = 'Mukta'
+    Mukta_Mahee = 'Mukta Mahee'
+    Mukta_Malar = 'Mukta Malar'
+    Mukta_Vaani = 'Mukta Vaani'
+    Mulish = 'Mulish'
+    MuseoModerno = 'MuseoModerno'
+    Mystery_Quest = 'Mystery Quest'
+    NTR = 'NTR'
+    Nanum_Brush_Script = 'Nanum Brush Script'
+    Nanum_Gothic = 'Nanum Gothic'
+    Nanum_Gothic_Coding = 'Nanum Gothic Coding'
+    Nanum_Myeongjo = 'Nanum Myeongjo'
+    Nanum_Pen_Script = 'Nanum Pen Script'
+    Neucha = 'Neucha'
+    Neuton = 'Neuton'
+    New_Rocker = 'New Rocker'
+    News_Cycle = 'News Cycle'
+    Niconne = 'Niconne'
+    Niramit = 'Niramit'
+    Nixie_One = 'Nixie One'
+    Nobile = 'Nobile'
+    Nokora = 'Nokora'
+    Norican = 'Norican'
+    Nosifer = 'Nosifer'
+    Notable = 'Notable'
+    Nothing_You_Could_Do = 'Nothing You Could Do'
+    Noticia_Text = 'Noticia Text'
+    Noto_Sans = 'Noto Sans'
+    Noto_Sans_HK = 'Noto Sans HK'
+    Noto_Sans_JP = 'Noto Sans JP'
+    Noto_Sans_KR = 'Noto Sans KR'
+    Noto_Sans_SC = 'Noto Sans SC'
+    Noto_Sans_TC = 'Noto Sans TC'
+    Noto_Serif = 'Noto Serif'
+    Noto_Serif_JP = 'Noto Serif JP'
+    Noto_Serif_KR = 'Noto Serif KR'
+    Noto_Serif_SC = 'Noto Serif SC'
+    Noto_Serif_TC = 'Noto Serif TC'
+    Nova_Cut = 'Nova Cut'
+    Nova_Flat = 'Nova Flat'
+    Nova_Mono = 'Nova Mono'
+    Nova_Oval = 'Nova Oval'
+    Nova_Round = 'Nova Round'
+    Nova_Script = 'Nova Script'
+    Nova_Slim = 'Nova Slim'
+    Nova_Square = 'Nova Square'
+    Numans = 'Numans'
+    Nunito = 'Nunito'
+    Nunito_Sans = 'Nunito Sans'
+    Odibee_Sans = 'Odibee Sans'
+    Odor_Mean_Chey = 'Odor Mean Chey'
+    Offside = 'Offside'
+    Old_Standard_TT = 'Old Standard TT'
+    Oldenburg = 'Oldenburg'
+    Oleo_Script = 'Oleo Script'
+    Oleo_Script_Swash_Caps = 'Oleo Script Swash Caps'
+    Open_Sans = 'Open Sans'
+    Open_Sans_Condensed = 'Open Sans Condensed'
+    Oranienbaum = 'Oranienbaum'
+    Orbitron = 'Orbitron'
+    Oregano = 'Oregano'
+    Orienta = 'Orienta'
+    Original_Surfer = 'Original Surfer'
+    Oswald = 'Oswald'
+    Over_the_Rainbow = 'Over the Rainbow'
+    Overlock = 'Overlock'
+    Overlock_SC = 'Overlock SC'
+    Overpass = 'Overpass'
+    Overpass_Mono = 'Overpass Mono'
+    Ovo = 'Ovo'
+    Oxanium = 'Oxanium'
+    Oxygen = 'Oxygen'
+    Oxygen_Mono = 'Oxygen Mono'
+    PT_Mono = 'PT Mono'
+    PT_Sans = 'PT Sans'
+    PT_Sans_Caption = 'PT Sans Caption'
+    PT_Sans_Narrow = 'PT Sans Narrow'
+    PT_Serif = 'PT Serif'
+    PT_Serif_Caption = 'PT Serif Caption'
+    Pacifico = 'Pacifico'
+    Padauk = 'Padauk'
+    Palanquin = 'Palanquin'
+    Palanquin_Dark = 'Palanquin Dark'
+    Pangolin = 'Pangolin'
+    Paprika = 'Paprika'
+    Parisienne = 'Parisienne'
+    Passero_One = 'Passero One'
+    Passion_One = 'Passion One'
+    Pathway_Gothic_One = 'Pathway Gothic One'
+    Patrick_Hand = 'Patrick Hand'
+    Patrick_Hand_SC = 'Patrick Hand SC'
+    Pattaya = 'Pattaya'
+    Patua_One = 'Patua One'
+    Pavanam = 'Pavanam'
+    Paytone_One = 'Paytone One'
+    Peddana = 'Peddana'
+    Peralta = 'Peralta'
+    Permanent_Marker = 'Permanent Marker'
+    Petit_Formal_Script = 'Petit Formal Script'
+    Petrona = 'Petrona'
+    Philosopher = 'Philosopher'
+    Piedra = 'Piedra'
+    Pinyon_Script = 'Pinyon Script'
+    Pirata_One = 'Pirata One'
+    Plaster = 'Plaster'
+    Play = 'Play'
+    Playball = 'Playball'
+    Playfair_Display = 'Playfair Display'
+    Playfair_Display_SC = 'Playfair Display SC'
+    Podkova = 'Podkova'
+    Poiret_One = 'Poiret One'
+    Poller_One = 'Poller One'
+    Poly = 'Poly'
+    Pompiere = 'Pompiere'
+    Pontano_Sans = 'Pontano Sans'
+    Poor_Story = 'Poor Story'
+    Poppins = 'Poppins'
+    Port_Lligat_Sans = 'Port Lligat Sans'
+    Port_Lligat_Slab = 'Port Lligat Slab'
+    Pragati_Narrow = 'Pragati Narrow'
+    Prata = 'Prata'
+    Preahvihear = 'Preahvihear'
+    Press_Start_2P = 'Press Start 2P'
+    Pridi = 'Pridi'
+    Princess_Sofia = 'Princess Sofia'
+    Prociono = 'Prociono'
+    Prompt = 'Prompt'
+    Prosto_One = 'Prosto One'
+    Proza_Libre = 'Proza Libre'
+    Public_Sans = 'Public Sans'
+    Puritan = 'Puritan'
+    Purple_Purse = 'Purple Purse'
+    Quando = 'Quando'
+    Quantico = 'Quantico'
+    Quattrocento = 'Quattrocento'
+    Quattrocento_Sans = 'Quattrocento Sans'
+    Questrial = 'Questrial'
+    Quicksand = 'Quicksand'
+    Quintessential = 'Quintessential'
+    Qwigley = 'Qwigley'
+    Racing_Sans_One = 'Racing Sans One'
+    Radley = 'Radley'
+    Rajdhani = 'Rajdhani'
+    Rakkas = 'Rakkas'
+    Raleway = 'Raleway'
+    Raleway_Dots = 'Raleway Dots'
+    Ramabhadra = 'Ramabhadra'
+    Ramaraja = 'Ramaraja'
+    Rambla = 'Rambla'
+    Rammetto_One = 'Rammetto One'
+    Ranchers = 'Ranchers'
+    Rancho = 'Rancho'
+    Ranga = 'Ranga'
+    Rasa = 'Rasa'
+    Rationale = 'Rationale'
+    Ravi_Prakash = 'Ravi Prakash'
+    Recursive = 'Recursive'
+    Red_Hat_Display = 'Red Hat Display'
+    Red_Hat_Text = 'Red Hat Text'
+    Red_Rose = 'Red Rose'
+    Redressed = 'Redressed'
+    Reem_Kufi = 'Reem Kufi'
+    Reenie_Beanie = 'Reenie Beanie'
+    Revalia = 'Revalia'
+    Rhodium_Libre = 'Rhodium Libre'
+    Ribeye = 'Ribeye'
+    Ribeye_Marrow = 'Ribeye Marrow'
+    Righteous = 'Righteous'
+    Risque = 'Risque'
+    Roboto = 'Roboto'
+    Roboto_Condensed = 'Roboto Condensed'
+    Roboto_Mono = 'Roboto Mono'
+    Roboto_Slab = 'Roboto Slab'
+    Rochester = 'Rochester'
+    Rock_Salt = 'Rock Salt'
+    Rokkitt = 'Rokkitt'
+    Romanesco = 'Romanesco'
+    Ropa_Sans = 'Ropa Sans'
+    Rosario = 'Rosario'
+    Rosarivo = 'Rosarivo'
+    Rouge_Script = 'Rouge Script'
+    Rowdies = 'Rowdies'
+    Rozha_One = 'Rozha One'
+    Rubik = 'Rubik'
+    Rubik_Mono_One = 'Rubik Mono One'
+    Ruda = 'Ruda'
+    Rufina = 'Rufina'
+    Ruge_Boogie = 'Ruge Boogie'
+    Ruluko = 'Ruluko'
+    Rum_Raisin = 'Rum Raisin'
+    Ruslan_Display = 'Ruslan Display'
+    Russo_One = 'Russo One'
+    Ruthie = 'Ruthie'
+    Rye = 'Rye'
+    Sacramento = 'Sacramento'
+    Sahitya = 'Sahitya'
+    Sail = 'Sail'
+    Saira = 'Saira'
+    Saira_Condensed = 'Saira Condensed'
+    Saira_Extra_Condensed = 'Saira Extra Condensed'
+    Saira_Semi_Condensed = 'Saira Semi Condensed'
+    Saira_Stencil_One = 'Saira Stencil One'
+    Salsa = 'Salsa'
+    Sanchez = 'Sanchez'
+    Sancreek = 'Sancreek'
+    Sansita = 'Sansita'
+    Sarabun = 'Sarabun'
+    Sarala = 'Sarala'
+    Sarina = 'Sarina'
+    Sarpanch = 'Sarpanch'
+    Satisfy = 'Satisfy'
+    Sawarabi_Gothic = 'Sawarabi Gothic'
+    Sawarabi_Mincho = 'Sawarabi Mincho'
+    Scada = 'Scada'
+    Scheherazade = 'Scheherazade'
+    Schoolbell = 'Schoolbell'
+    Scope_One = 'Scope One'
+    Seaweed_Script = 'Seaweed Script'
+    Secular_One = 'Secular One'
+    Sedgwick_Ave = 'Sedgwick Ave'
+    Sedgwick_Ave_Display = 'Sedgwick Ave Display'
+    Sen = 'Sen'
+    Sevillana = 'Sevillana'
+    Seymour_One = 'Seymour One'
+    Shadows_Into_Light = 'Shadows Into Light'
+    Shadows_Into_Light_Two = 'Shadows Into Light Two'
+    Shanti = 'Shanti'
+    Share = 'Share'
+    Share_Tech = 'Share Tech'
+    Share_Tech_Mono = 'Share Tech Mono'
+    Shojumaru = 'Shojumaru'
+    Short_Stack = 'Short Stack'
+    Shrikhand = 'Shrikhand'
+    Siemreap = 'Siemreap'
+    Sigmar_One = 'Sigmar One'
+    Signika = 'Signika'
+    Signika_Negative = 'Signika Negative'
+    Simonetta = 'Simonetta'
+    Single_Day = 'Single Day'
+    Sintony = 'Sintony'
+    Sirin_Stencil = 'Sirin Stencil'
+    Six_Caps = 'Six Caps'
+    Skranji = 'Skranji'
+    Slabo_13px = 'Slabo 13px'
+    Slabo_27px = 'Slabo 27px'
+    Slackey = 'Slackey'
+    Smokum = 'Smokum'
+    Smythe = 'Smythe'
+    Sniglet = 'Sniglet'
+    Snippet = 'Snippet'
+    Snowburst_One = 'Snowburst One'
+    Sofadi_One = 'Sofadi One'
+    Sofia = 'Sofia'
+    Solway = 'Solway'
+    Song_Myung = 'Song Myung'
+    Sonsie_One = 'Sonsie One'
+    Sora = 'Sora'
+    Sorts_Mill_Goudy = 'Sorts Mill Goudy'
+    Source_Code_Pro = 'Source Code Pro'
+    Source_Sans_Pro = 'Source Sans Pro'
+    Source_Serif_Pro = 'Source Serif Pro'
+    Space_Mono = 'Space Mono'
+    Spartan = 'Spartan'
+    Special_Elite = 'Special Elite'
+    Spectral = 'Spectral'
+    Spectral_SC = 'Spectral SC'
+    Spicy_Rice = 'Spicy Rice'
+    Spinnaker = 'Spinnaker'
+    Spirax = 'Spirax'
+    Squada_One = 'Squada One'
+    Sree_Krushnadevaraya = 'Sree Krushnadevaraya'
+    Sriracha = 'Sriracha'
+    Srisakdi = 'Srisakdi'
+    Staatliches = 'Staatliches'
+    Stalemate = 'Stalemate'
+    Stalinist_One = 'Stalinist One'
+    Stardos_Stencil = 'Stardos Stencil'
+    Stint_Ultra_Condensed = 'Stint Ultra Condensed'
+    Stint_Ultra_Expanded = 'Stint Ultra Expanded'
+    Stoke = 'Stoke'
+    Strait = 'Strait'
+    Stylish = 'Stylish'
+    Sue_Ellen_Francisco = 'Sue Ellen Francisco'
+    Suez_One = 'Suez One'
+    Sulphur_Point = 'Sulphur Point'
+    Sumana = 'Sumana'
+    Sunflower = 'Sunflower'
+    Sunshiney = 'Sunshiney'
+    Supermercado_One = 'Supermercado One'
+    Sura = 'Sura'
+    Suranna = 'Suranna'
+    Suravaram = 'Suravaram'
+    Suwannaphum = 'Suwannaphum'
+    Swanky_and_Moo_Moo = 'Swanky and Moo Moo'
+    Syncopate = 'Syncopate'
+    Tajawal = 'Tajawal'
+    Tangerine = 'Tangerine'
+    Taprom = 'Taprom'
+    Tauri = 'Tauri'
+    Taviraj = 'Taviraj'
+    Teko = 'Teko'
+    Telex = 'Telex'
+    Tenali_Ramakrishna = 'Tenali Ramakrishna'
+    Tenor_Sans = 'Tenor Sans'
+    Text_Me_One = 'Text Me One'
+    Thasadith = 'Thasadith'
+    The_Girl_Next_Door = 'The Girl Next Door'
+    Tienne = 'Tienne'
+    Tillana = 'Tillana'
+    Timmana = 'Timmana'
+    Tinos = 'Tinos'
+    Titan_One = 'Titan One'
+    Titillium_Web = 'Titillium Web'
+    Tomorrow = 'Tomorrow'
+    Trade_Winds = 'Trade Winds'
+    Trirong = 'Trirong'
+    Trocchi = 'Trocchi'
+    Trochut = 'Trochut'
+    Trykker = 'Trykker'
+    Tulpen_One = 'Tulpen One'
+    Turret_Road = 'Turret Road'
+    Ubuntu = 'Ubuntu'
+    Ubuntu_Condensed = 'Ubuntu Condensed'
+    Ubuntu_Mono = 'Ubuntu Mono'
+    Ultra = 'Ultra'
+    Uncial_Antiqua = 'Uncial Antiqua'
+    Underdog = 'Underdog'
+    Unica_One = 'Unica One'
+    UnifrakturCook = 'UnifrakturCook'
+    UnifrakturMaguntia = 'UnifrakturMaguntia'
+    Unkempt = 'Unkempt'
+    Unlock = 'Unlock'
+    Unna = 'Unna'
+    VT323 = 'VT323'
+    Vampiro_One = 'Vampiro One'
+    Varela = 'Varela'
+    Varela_Round = 'Varela Round'
+    Varta = 'Varta'
+    Vast_Shadow = 'Vast Shadow'
+    Vesper_Libre = 'Vesper Libre'
+    Viaoda_Libre = 'Viaoda Libre'
+    Vibes = 'Vibes'
+    Vibur = 'Vibur'
+    Vidaloka = 'Vidaloka'
+    Viga = 'Viga'
+    Voces = 'Voces'
+    Volkhov = 'Volkhov'
+    Vollkorn = 'Vollkorn'
+    Vollkorn_SC = 'Vollkorn SC'
+    Voltaire = 'Voltaire'
+    Waiting_for_the_Sunrise = 'Waiting for the Sunrise'
+    Wallpoet = 'Wallpoet'
+    Walter_Turncoat = 'Walter Turncoat'
+    Warnes = 'Warnes'
+    Wellfleet = 'Wellfleet'
+    Wendy_One = 'Wendy One'
+    Wire_One = 'Wire One'
+    Work_Sans = 'Work Sans'
+    Yanone_Kaffeesatz = 'Yanone Kaffeesatz'
+    Yantramanav = 'Yantramanav'
+    Yatra_One = 'Yatra One'
+    Yellowtail = 'Yellowtail'
+    Yeon_Sung = 'Yeon Sung'
+    Yeseva_One = 'Yeseva One'
+    Yesteryear = 'Yesteryear'
+    Yrsa = 'Yrsa'
+    ZCOOL_KuaiLe = 'ZCOOL KuaiLe'
+    ZCOOL_QingKe_HuangYou = 'ZCOOL QingKe HuangYou'
+    ZCOOL_XiaoWei = 'ZCOOL XiaoWei'
+    Zeyada = 'Zeyada'
+    Zhi_Mang_Xing = 'Zhi Mang Xing'
+    Zilla_Slab = 'Zilla Slab'
+    Zilla_Slab_Highlight = 'Zilla Slab Highlight'
+
+    def __str__(self):
+        return '{0}'.format(self.value)
+
+
+class GradientType(Enum):
+    linear = 'linear',
+    radial = 'radial'
+
+    def __str__(self):
+        return '{0}'.format(self.value)
+
+class FontWeightType(Enum):
+    light = 300
+    normal = 400
+    bold = 700
+
+    def __str__(self):
+        return '{0}'.format(self.value)
```

