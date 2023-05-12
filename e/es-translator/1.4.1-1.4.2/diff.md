# Comparing `tmp/es_translator-1.4.1.tar.gz` & `tmp/es_translator-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "es_translator-1.4.1.tar", max compression
+gzip compressed data, was "es_translator-1.4.2.tar", max compression
```

## Comparing `es_translator-1.4.1.tar` & `es_translator-1.4.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0    34551 2022-06-20 12:45:46.179755 es_translator-1.4.1/LICENSE.txt
--rw-r--r--   0        0        0     3704 2023-05-10 10:53:32.886660 es_translator-1.4.1/README.md
--rw-r--r--   0        0        0      136 2022-07-26 11:37:09.729633 es_translator-1.4.1/es_translator/__init__.py
--rw-r--r--   0        0        0      490 2022-06-20 12:45:46.183755 es_translator-1.4.1/es_translator/alpha.py
--rw-r--r--   0        0        0     4932 2023-05-10 10:52:28.954000 es_translator-1.4.1/es_translator/cli.py
--rw-r--r--   0        0        0     1893 2022-07-26 11:37:09.729633 es_translator-1.4.1/es_translator/es.py
--rw-r--r--   0        0        0     5325 2022-07-26 11:37:09.729633 es_translator-1.4.1/es_translator/es_translator.py
--rw-r--r--   0        0        0       55 2022-07-26 11:37:09.729633 es_translator-1.4.1/es_translator/interpreters/__init__.py
--rw-r--r--   0        0        0     1690 2022-07-26 11:37:09.729633 es_translator-1.4.1/es_translator/interpreters/abstract.py
--rw-r--r--   0        0        0       30 2022-07-26 11:37:09.729633 es_translator-1.4.1/es_translator/interpreters/apertium/__init__.py
--rw-r--r--   0        0        0     6069 2022-07-26 11:37:09.729633 es_translator-1.4.1/es_translator/interpreters/apertium/apertium.py
--rw-r--r--   0        0        0      722 2022-07-26 11:37:09.729633 es_translator-1.4.1/es_translator/interpreters/apertium/pairs.py
--rw-r--r--   0        0        0     5390 2022-12-15 10:03:37.305408 es_translator-1.4.1/es_translator/interpreters/apertium/repository.py
--rw-r--r--   0        0        0       24 2022-07-26 11:37:09.729633 es_translator-1.4.1/es_translator/interpreters/argos/__init__.py
--rw-r--r--   0        0        0     2553 2022-07-26 11:37:09.729633 es_translator-1.4.1/es_translator/interpreters/argos/argos.py
--rw-r--r--   0        0        0      912 2022-07-26 11:37:09.729633 es_translator-1.4.1/es_translator/logger.py
--rw-r--r--   0        0        0      267 2022-06-20 12:45:46.183755 es_translator-1.4.1/es_translator/symlink.py
--rw-r--r--   0        0        0      842 2023-05-10 15:37:53.241163 es_translator-1.4.1/pyproject.toml
--rw-r--r--   0        0        0     4996 1970-01-01 00:00:00.000000 es_translator-1.4.1/setup.py
--rw-r--r--   0        0        0     4654 1970-01-01 00:00:00.000000 es_translator-1.4.1/PKG-INFO
+-rw-r--r--   0        0        0    34551 2022-06-20 12:45:46.179755 es_translator-1.4.2/LICENSE.txt
+-rw-r--r--   0        0        0     3704 2023-05-10 10:53:32.886660 es_translator-1.4.2/README.md
+-rw-r--r--   0        0        0      136 2022-07-26 11:37:09.729633 es_translator-1.4.2/es_translator/__init__.py
+-rw-r--r--   0        0        0      490 2022-06-20 12:45:46.183755 es_translator-1.4.2/es_translator/alpha.py
+-rw-r--r--   0        0        0     5013 2023-05-12 13:02:30.048545 es_translator-1.4.2/es_translator/cli.py
+-rw-r--r--   0        0        0     1893 2022-07-26 11:37:09.729633 es_translator-1.4.2/es_translator/es.py
+-rw-r--r--   0        0        0     5325 2022-07-26 11:37:09.729633 es_translator-1.4.2/es_translator/es_translator.py
+-rw-r--r--   0        0        0       55 2022-07-26 11:37:09.729633 es_translator-1.4.2/es_translator/interpreters/__init__.py
+-rw-r--r--   0        0        0     1690 2022-07-26 11:37:09.729633 es_translator-1.4.2/es_translator/interpreters/abstract.py
+-rw-r--r--   0        0        0       30 2022-07-26 11:37:09.729633 es_translator-1.4.2/es_translator/interpreters/apertium/__init__.py
+-rw-r--r--   0        0        0     6069 2022-07-26 11:37:09.729633 es_translator-1.4.2/es_translator/interpreters/apertium/apertium.py
+-rw-r--r--   0        0        0      722 2022-07-26 11:37:09.729633 es_translator-1.4.2/es_translator/interpreters/apertium/pairs.py
+-rw-r--r--   0        0        0     5390 2022-12-15 10:03:37.305408 es_translator-1.4.2/es_translator/interpreters/apertium/repository.py
+-rw-r--r--   0        0        0       24 2022-07-26 11:37:09.729633 es_translator-1.4.2/es_translator/interpreters/argos/__init__.py
+-rw-r--r--   0        0        0     2553 2022-07-26 11:37:09.729633 es_translator-1.4.2/es_translator/interpreters/argos/argos.py
+-rw-r--r--   0        0        0      912 2022-07-26 11:37:09.729633 es_translator-1.4.2/es_translator/logger.py
+-rw-r--r--   0        0        0      267 2022-06-20 12:45:46.183755 es_translator-1.4.2/es_translator/symlink.py
+-rw-r--r--   0        0        0      842 2023-05-12 13:31:48.466306 es_translator-1.4.2/pyproject.toml
+-rw-r--r--   0        0        0     4996 1970-01-01 00:00:00.000000 es_translator-1.4.2/setup.py
+-rw-r--r--   0        0        0     4654 1970-01-01 00:00:00.000000 es_translator-1.4.2/PKG-INFO
```

### Comparing `es_translator-1.4.1/LICENSE.txt` & `es_translator-1.4.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `es_translator-1.4.1/README.md` & `es_translator-1.4.2/README.md`

 * *Files identical despite different names*

### Comparing `es_translator-1.4.1/es_translator/cli.py` & `es_translator-1.4.2/es_translator/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,35 +30,35 @@
         if value.upper() == interpreter.name.upper():
             return interpreter
     names = (interpreter.name for interpreter in interpreters)
     raise click.BadParameter('must be a valid interpreter name (%s)' % ', '.join(names))
 
 
 @click.command()
-@click.option('--url', help='Elastichsearch URL', required=True)
-@click.option('--index', help='Elastichsearch Index', required=True)
-@click.option('--interpreter', help='Interpreter to use to perform the translation', default='ARGOS', callback=validate_interpreter)
-@click.option('--source-language', help='Source language to translate from', required=True, default=None)
-@click.option('--target-language', help='Target language to translate to', required=True, default=None)
+@click.option('-u', '--url', help='Elastichsearch URL', default="http://localhost:9200", required=True)
+@click.option('-i', '--index', help='Elastichsearch Index', required=True)
+@click.option('-r', '--interpreter', help='Interpreter to use to perform the translation', default='ARGOS', callback=validate_interpreter)
+@click.option('-s', '--source-language', help='Source language to translate from', required=True, default=None)
+@click.option('-t', '--target-language', help='Target language to translate to', required=True, default=None)
 @click.option('--intermediary-language', help='An intermediary language to use when no translation is available between the source and the target. If none is provided this will be calculated automatically.')
 @click.option('--source-field', help='Document field to translate', default="content")
 @click.option('--target-field', help='Document field where the translations are stored', default="content_translated")
-@click.option('--query-string', help='Search query string to filter result')
-@click.option('--data-dir', help='Path to the directory where to language model will be downloaded', type=click.Path(exists=True, dir_okay=True, writable=True, readable=True), default=mkdtemp())
+@click.option('-q', '--query-string', help='Search query string to filter result')
+@click.option('-d', '--data-dir', help='Path to the directory where to language model will be downloaded', type=click.Path(exists=True, dir_okay=True, writable=True, readable=True), default=mkdtemp())
 @click.option('--scan-scroll', help='Scroll duration (set to higher value if you\'re processing a lot of documents)', default="5m")
 @click.option('--dry-run', help='Don\'t save anything in Elasticsearch', is_flag=True, default=False)
 @click.option('--pool-size', help='Number of parallel processes to start', default=1)
 @click.option('--pool-timeout', help='Timeout to add a translation', default=60 * 30)
 @click.option('--throttle', help='Throttle between each translation (in ms)', default=0)
 @click.option('--syslog-address', help='Syslog address', default='localhost')
 @click.option('--syslog-port', help='Syslog port', default=514)
 @click.option('--syslog-facility', help='Syslog facility', default='local7')
 @click.option('--stdout-loglevel', help='Change the default log level for stdout error handler', default='ERROR',
               callback=validate_loglevel)
-@click.option('--progressbar/--no-progressbar', help='Display a progressbar', default=None,
+@click.option('-p', '--progressbar/--no-progressbar', help='Display a progressbar', default=None,
             callback=validate_progressbar)
 def translate(syslog_address, syslog_port, syslog_facility, **options):
     # Configure Syslog handler
     add_syslog_handler(syslog_address, syslog_port, syslog_facility)
     add_stdout_handler(options['stdout_loglevel'])
     # We pass all options to EsTranslator then we start the translation
     # from Elasticsearch. This will download required pairs if needed.
```

### Comparing `es_translator-1.4.1/es_translator/es.py` & `es_translator-1.4.2/es_translator/es.py`

 * *Files identical despite different names*

### Comparing `es_translator-1.4.1/es_translator/es_translator.py` & `es_translator-1.4.2/es_translator/es_translator.py`

 * *Files identical despite different names*

### Comparing `es_translator-1.4.1/es_translator/interpreters/abstract.py` & `es_translator-1.4.2/es_translator/interpreters/abstract.py`

 * *Files identical despite different names*

### Comparing `es_translator-1.4.1/es_translator/interpreters/apertium/apertium.py` & `es_translator-1.4.2/es_translator/interpreters/apertium/apertium.py`

 * *Files identical despite different names*

### Comparing `es_translator-1.4.1/es_translator/interpreters/apertium/pairs.py` & `es_translator-1.4.2/es_translator/interpreters/apertium/pairs.py`

 * *Files identical despite different names*

### Comparing `es_translator-1.4.1/es_translator/interpreters/apertium/repository.py` & `es_translator-1.4.2/es_translator/interpreters/apertium/repository.py`

 * *Files identical despite different names*

### Comparing `es_translator-1.4.1/es_translator/interpreters/argos/argos.py` & `es_translator-1.4.2/es_translator/interpreters/argos/argos.py`

 * *Files identical despite different names*

### Comparing `es_translator-1.4.1/es_translator/logger.py` & `es_translator-1.4.2/es_translator/logger.py`

 * *Files identical despite different names*

### Comparing `es_translator-1.4.1/pyproject.toml` & `es_translator-1.4.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "es-translator"
-version = "1.4.1"
+version = "1.4.2"
 description = "A lazy yet bulletproof machine translation tool for Elastichsearch."
 authors = ["ICIJ <engineering@icij.org>"]
 readme = "README.md"
 license = "GNU AFFERO GENERAL PUBLIC LICENSE"
 packages = [{include = "es_translator"}]
 
 [tool.poetry.dependencies]
```

### Comparing `es_translator-1.4.1/setup.py` & `es_translator-1.4.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 entry_points = \
 {'console_scripts': ['es-translator = es_translator.cli:translate',
                      'es-translator-pairs = es_translator.cli:pairs']}
 
 setup_kwargs = {
     'name': 'es-translator',
-    'version': '1.4.1',
+    'version': '1.4.2',
     'description': 'A lazy yet bulletproof machine translation tool for Elastichsearch.',
     'long_description': '# ES Translator\n\n[![CircleCI](https://circleci.com/gh/ICIJ/es-translator.svg?style=svg)](https://circleci.com/gh/ICIJ/es-translator)\n\nA lazy yet bulletproof machine translation tool for Elastichsearch.\n\n```\nUsage: es-translator [OPTIONS]\n\nOptions:\n  --url TEXT                    Elastichsearch URL  [required]\n  --index TEXT                  Elastichsearch Index  [required]\n  --interpreter TEXT            Interpreter to use to perform the translation\n  --source-language TEXT        Source language to translate from  [required]\n  --target-language TEXT        Target language to translate to  [required]\n  --intermediary-language TEXT  An intermediary language to use when no\n                                translation is available between the source\n                                and the target. If none is provided this will\n                                be calculated automatically.\n  --source-field TEXT           Document field to translate\n  --target-field TEXT           Document field where the translations are\n                                stored\n  --query-string TEXT           Search query string to filter result\n  --data-dir PATH               Path to the directory where to language model\n                                will be downloaded\n  --scan-scroll TEXT            Scroll duration (set to higher value if you\'re\n                                processing a lot of documents)\n  --dry-run                     Don\'t save anything in Elasticsearch\n  --pool-size INTEGER           Number of parallel processes to start\n  --pool-timeout INTEGER        Timeout to add a translation\n  --syslog-address TEXT         Syslog address\n  --syslog-port INTEGER         Syslog port\n  --syslog-facility TEXT        Syslog facility\n  --stdout-loglevel TEXT        Change the default log level for stdout error\n                                handler\n  --help                        Show this message and exit.\n```\n\n## Installation (Ubuntu)\n\nInstall Apertium:\n\n```\nwget https://apertium.projectjj.com/apt/install-nightly.sh -O - | sudo bash\nsudo apt install apertium-all-dev\n```\n\nCreate a Virtualenv and install Pip packages with Poetry:\n\n```\nmake install\n```\n\nOn Ubuntu 22.04 some additional packages might be needed if you use the version from Ubuntu\'s repository:\n\n```\nsudo apt install cg3 apertium-get apertium-lex-tools\n```\n\n\n## Installation (Docker)\n\nNothing to do as long as you have Docker on your system:\n\n```\ndocker run -it icij/es-translator poetry run es-translator --help\n```\n\n## Examples\n\nTranslates documents from French to Spanish on a local Elasticsearch. The translated field is `content` (the default).\n\n```bash\npoetry run es-translator --url "http://localhost:9200" --index my-index --source-language fr --target-language es\n```\n\nTranslates documents from French to English on a local Elasticsearch using Apertium:\n\n```bash\npoetry run es-translator --url "http://localhost:9200" --index my-index --source-language fr --target-language en --interpreter apertium\n```\n\nTo translate the `title` field we could do:\n\n```bash\npoetry run es-translator --url "http://localhost:9200" --index my-index --source-language fr --target-language es --source-field title\n```\n\nTranslates documents from English to Spanish on a local Elasticsearch using 4 threads:\n\n```bash\npoetry run es-translator --url "http://localhost:9200" --index my-index --source-language en --target-language es --pool-size 4\n```\n\nTranslates documents from Portuguese to English, using an intermediary language (Apertium doesn\'t offer this translation pair):\n\n```bash\npoetry run es-translator --url "http://localhost:9200" --index my-index --source-language pt --intermediary-language es --target-language en\n```\n',
     'author': 'ICIJ',
     'author_email': 'engineering@icij.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `es_translator-1.4.1/PKG-INFO` & `es_translator-1.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: es-translator
-Version: 1.4.1
+Version: 1.4.2
 Summary: A lazy yet bulletproof machine translation tool for Elastichsearch.
 License: GNU AFFERO GENERAL PUBLIC LICENSE
 Author: ICIJ
 Author-email: engineering@icij.org
 Requires-Python: >=3.8,<3.11
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

