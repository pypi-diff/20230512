# Comparing `tmp/lsqfit-9.4.tar.gz` & `tmp/lsqfit-9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/lsqfit-9.4.tar", last modified: Sun Jul  8 20:40:45 2018, max compression
+gzip compressed data, was "dist/lsqfit-9.5.tar", last modified: Sun Jul 15 18:36:18 2018, max compression
```

## Comparing `lsqfit-9.4.tar` & `lsqfit-9.5.tar`

### file list

```diff
@@ -1,172 +1,172 @@
-drwxr-xr-x   0 gpl        (503) staff       (20)        0 2018-07-08 20:40:45.000000 lsqfit-9.4/
--rw-r--r--   0 gpl        (503) staff       (20)     3199 2018-07-08 20:40:45.000000 lsqfit-9.4/PKG-INFO
--rw-r--r--   0 gpl        (503) staff       (20)     3272 2018-07-08 20:39:08.000000 lsqfit-9.4/makefile
-drwxr-xr-x   0 gpl        (503) staff       (20)        0 2018-07-08 20:40:45.000000 lsqfit-9.4/tests/
--rw-r--r--   0 gpl        (503) staff       (20)    16954 2018-07-07 13:56:49.000000 lsqfit-9.4/tests/test_multifitter.py
--rw-r--r--   0 gpl        (503) staff       (20)    70019 2018-04-26 13:13:10.000000 lsqfit-9.4/tests/test_lsqfit.py
--rw-r--r--   0 gpl        (503) staff       (20)      989 2013-01-13 22:28:17.000000 lsqfit-9.4/tests/makefile
--rw-r--r--   0 gpl        (503) staff       (20)      104 2012-06-18 04:03:00.000000 lsqfit-9.4/tests/__init__.py
--rw-r--r--   0 gpl        (503) staff       (20)      395 2012-06-18 08:13:19.000000 lsqfit-9.4/tests/README
--rw-r--r--   0 gpl        (503) staff       (20)      384 2018-03-30 14:28:05.000000 lsqfit-9.4/MANIFEST.in
--rw-r--r--   0 gpl        (503) staff       (20)    46060 2018-07-08 20:24:04.000000 lsqfit-9.4/CHANGES.txt
--rw-r--r--   0 gpl        (503) staff       (20)     4805 2018-07-08 19:37:53.000000 lsqfit-9.4/setup.py
-drwxr-xr-x   0 gpl        (503) staff       (20)        0 2018-07-08 20:40:45.000000 lsqfit-9.4/examples/
--rw-r--r--   0 gpl        (503) staff       (20)     1187 2017-01-09 17:45:08.000000 lsqfit-9.4/examples/x-err.out
--rw-r--r--   0 gpl        (503) staff       (20)    12053 2017-01-09 17:45:08.000000 lsqfit-9.4/examples/nist.out
--rw-r--r--   0 gpl        (503) staff       (20)    12734 2016-08-15 18:23:44.000000 lsqfit-9.4/examples/pendulum.pdf
--rw-r--r--   0 gpl        (503) staff       (20)     1363 2017-01-11 15:09:53.000000 lsqfit-9.4/examples/uncorrelated.py
--rw-r--r--   0 gpl        (503) staff       (20)     5739 2017-02-07 04:04:01.000000 lsqfit-9.4/examples/y-noerr.out
--rw-r--r--   0 gpl        (503) staff       (20)      435 2017-01-09 17:45:08.000000 lsqfit-9.4/examples/p-corr.out
--rw-r--r--   0 gpl        (503) staff       (20)      580 2017-02-07 04:17:35.000000 lsqfit-9.4/examples/xxxx
--rw-r--r--   0 gpl        (503) staff       (20)     4464 2017-01-09 17:45:08.000000 lsqfit-9.4/examples/y-vs-x.out
--rw-r--r--   0 gpl        (503) staff       (20)    66290 2018-03-18 18:26:10.000000 lsqfit-9.4/examples/nist.py
--rw-r--r--   0 gpl        (503) staff       (20)     1271 2017-01-09 17:45:08.000000 lsqfit-9.4/examples/empbayes.py
--rw-r--r--   0 gpl        (503) staff       (20)      580 2017-02-07 04:11:43.000000 lsqfit-9.4/examples/xxx.out
--rw-r--r--   0 gpl        (503) staff       (20)      580 2017-02-07 13:17:22.000000 lsqfit-9.4/examples/xxx
--rw-r--r--   0 gpl        (503) staff       (20)     2552 2017-01-09 18:18:12.000000 lsqfit-9.4/examples/makefile
--rw-r--r--   0 gpl        (503) staff       (20)      387 2017-01-09 17:45:08.000000 lsqfit-9.4/examples/uncorrelated.out
--rw-r--r--   0 gpl        (503) staff       (20)      852 2017-01-09 17:45:08.000000 lsqfit-9.4/examples/pendulum.out
--rw-r--r--   0 gpl        (503) staff       (20)     2148 2017-01-09 17:45:08.000000 lsqfit-9.4/examples/bayes.out
--rw-r--r--   0 gpl        (503) staff       (20)     4593 2017-01-09 18:56:23.000000 lsqfit-9.4/examples/y-vs-x.py
--rw-r--r--   0 gpl        (503) staff       (20)      798 2017-01-09 17:45:08.000000 lsqfit-9.4/examples/empbayes.out
-drwxr-xr-x   0 gpl        (503) staff       (20)        0 2018-07-08 20:40:45.000000 lsqfit-9.4/examples/nist/
--rw-r--r--   0 gpl        (503) staff       (20)     2431 2017-01-09 17:45:08.000000 lsqfit-9.4/examples/nist/roszman1.txt
--rw-r--r--   0 gpl        (503) staff       (20)     3025 2017-01-09 17:45:08.000000 lsqfit-9.4/examples/nist/thurber.txt
--rw-r--r--   0 gpl        (503) staff       (20)     6868 2017-01-09 17:45:08.000000 lsqfit-9.4/examples/nist/bennett5.txt
--rw-r--r--   0 gpl        (503) staff       (20)     1838 2017-01-09 17:45:08.000000 lsqfit-9.4/examples/nist/misra1c.txt
--rw-r--r--   0 gpl        (503) staff       (20)     6760 2017-01-09 17:45:08.000000 lsqfit-9.4/examples/nist/enso.txt
--rw-r--r--   0 gpl        (503) staff       (20)     7000 2017-01-09 17:45:08.000000 lsqfit-9.4/examples/nist/nelson.txt
--rw-r--r--   0 gpl        (503) staff       (20)     2573 2017-01-09 17:45:08.000000 lsqfit-9.4/examples/nist/lanczos3.txt
--rw-r--r--   0 gpl        (503) staff       (20)     2600 2017-01-09 17:45:08.000000 lsqfit-9.4/examples/nist/lanczos2.txt
--rw-r--r--   0 gpl        (503) staff       (20)     1844 2017-01-09 17:45:08.000000 lsqfit-9.4/examples/nist/misra1b.txt
--rw-r--r--   0 gpl        (503) staff       (20)    64851 2018-03-18 18:27:36.000000 lsqfit-9.4/examples/nist/1st_nist.py
--rw-r--r--   0 gpl        (503) staff       (20)     1872 2017-01-09 17:45:08.000000 lsqfit-9.4/examples/nist/rat42.txt
--rw-r--r--   0 gpl        (503) staff       (20)     2944 2017-01-09 17:45:08.000000 lsqfit-9.4/examples/nist/lanczos1.txt
--rw-r--r--   0 gpl        (503) staff       (20)     2071 2017-01-09 17:45:08.000000 lsqfit-9.4/examples/nist/rat43.txt
--rw-r--r--   0 gpl        (503) staff       (20)     1852 2017-01-09 17:45:08.000000 lsqfit-9.4/examples/nist/misra1a.txt
--rw-r--r--   0 gpl        (503) staff       (20)     1842 2017-01-09 17:45:08.000000 lsqfit-9.4/examples/nist/misra1d.txt
--rw-r--r--   0 gpl        (503) staff       (20)     1712 2017-01-09 17:45:08.000000 lsqfit-9.4/examples/nist/boxbod.txt
--rw-r--r--   0 gpl        (503) staff       (20)     2304 2017-01-09 17:45:08.000000 lsqfit-9.4/examples/nist/mgh09.txt
--rw-r--r--   0 gpl        (503) staff       (20)     2334 2017-01-09 17:45:08.000000 lsqfit-9.4/examples/nist/mgh10.txt
--rw-r--r--   0 gpl        (503) staff       (20)     6800 2017-02-06 20:28:57.000000 lsqfit-9.4/examples/nist/make_script.py
--rw-r--r--   0 gpl        (503) staff       (20)     3077 2017-01-09 17:45:08.000000 lsqfit-9.4/examples/nist/mgh17.txt
--rw-r--r--   0 gpl        (503) staff       (20)     9275 2017-01-09 17:45:08.000000 lsqfit-9.4/examples/nist/hahn1.txt
--rw-r--r--   0 gpl        (503) staff       (20)     8097 2017-01-09 17:45:08.000000 lsqfit-9.4/examples/nist/gauss1.txt
--rw-r--r--   0 gpl        (503) staff       (20)     2772 2017-01-09 17:45:08.000000 lsqfit-9.4/examples/nist/eckerle4.txt
--rw-r--r--   0 gpl        (503) staff       (20)     8099 2017-01-09 17:45:08.000000 lsqfit-9.4/examples/nist/gauss2.txt
--rw-r--r--   0 gpl        (503) staff       (20)     5857 2017-01-09 17:45:08.000000 lsqfit-9.4/examples/nist/kirby2.txt
--rw-r--r--   0 gpl        (503) staff       (20)     8101 2017-01-09 17:45:08.000000 lsqfit-9.4/examples/nist/gauss3.txt
--rw-r--r--   0 gpl        (503) staff       (20)    64931 2018-03-18 18:28:07.000000 lsqfit-9.4/examples/nist/2nd_nist.py
--rw-r--r--   0 gpl        (503) staff       (20)     3059 2017-01-09 17:45:08.000000 lsqfit-9.4/examples/nist/chwirut2.txt
--rw-r--r--   0 gpl        (503) staff       (20)     1989 2017-01-09 17:45:08.000000 lsqfit-9.4/examples/nist/danwood.txt
--rw-r--r--   0 gpl        (503) staff       (20)     7557 2017-01-09 17:45:08.000000 lsqfit-9.4/examples/nist/chwirut1.txt
--rw-r--r--   0 gpl        (503) staff       (20)      754 2017-01-09 17:45:08.000000 lsqfit-9.4/examples/README
--rw-r--r--   0 gpl        (503) staff       (20)     1670 2017-01-09 17:45:08.000000 lsqfit-9.4/examples/p-corr.py
--rw-r--r--   0 gpl        (503) staff       (20)     2758 2017-05-04 17:42:04.000000 lsqfit-9.4/examples/bayes.py
--rw-r--r--   0 gpl        (503) staff       (20)     1662 2017-01-09 18:49:37.000000 lsqfit-9.4/examples/x-err.py
--rw-r--r--   0 gpl        (503) staff       (20)      973 2017-01-09 17:45:08.000000 lsqfit-9.4/examples/simple.out
--rw-r--r--   0 gpl        (503) staff       (20)     2222 2014-06-26 08:07:55.000000 lsqfit-9.4/examples/simple.py
--rw-r--r--   0 gpl        (503) staff       (20)     4744 2016-08-15 01:11:44.000000 lsqfit-9.4/examples/pendulum.py
--rw-r--r--   0 gpl        (503) staff       (20)      547 2018-07-08 20:31:03.000000 lsqfit-9.4/examples/outputfile.p
--rw-r--r--   0 gpl        (503) staff       (20)     4459 2013-04-10 16:01:02.000000 lsqfit-9.4/examples/xxx.py
--rw-r--r--   0 gpl        (503) staff       (20)      828 2013-04-10 02:20:15.000000 lsqfit-9.4/examples/yyy.py
--rw-r--r--   0 gpl        (503) staff       (20)     2468 2017-02-07 04:03:39.000000 lsqfit-9.4/examples/y-noerr.py
-drwxr-xr-x   0 gpl        (503) staff       (20)        0 2018-07-08 20:40:45.000000 lsqfit-9.4/doc/
-drwxr-xr-x   0 gpl        (503) staff       (20)        0 2018-07-08 20:40:45.000000 lsqfit-9.4/doc/html/
--rw-r--r--   0 gpl        (503) staff       (20)   140100 2018-07-08 20:26:39.000000 lsqfit-9.4/doc/html/case-extrapolation.html
--rw-r--r--   0 gpl        (503) staff       (20)    11453 2018-07-08 20:26:39.000000 lsqfit-9.4/doc/html/index.html
--rw-r--r--   0 gpl        (503) staff       (20)    23754 2018-07-08 20:26:41.000000 lsqfit-9.4/doc/html/searchindex.js
--rw-r--r--   0 gpl        (503) staff       (20)    21666 2018-07-08 20:26:40.000000 lsqfit-9.4/doc/html/scipy.html
-drwxr-xr-x   0 gpl        (503) staff       (20)        0 2018-07-08 20:40:45.000000 lsqfit-9.4/doc/html/_sources/
--rw-r--r--   0 gpl        (503) staff       (20)     5977 2017-01-09 17:45:07.000000 lsqfit-9.4/doc/html/_sources/case-pendulum.rst.txt
--rw-r--r--   0 gpl        (503) staff       (20)    12347 2018-02-18 01:57:24.000000 lsqfit-9.4/doc/html/_sources/gsl.rst.txt
--rw-r--r--   0 gpl        (503) staff       (20)    12613 2017-01-09 17:45:07.000000 lsqfit-9.4/doc/html/_sources/case-extrapolation.rst.txt
--rw-r--r--   0 gpl        (503) staff       (20)    19810 2017-01-09 17:45:08.000000 lsqfit-9.4/doc/html/_sources/testing.rst.txt
--rw-r--r--   0 gpl        (503) staff       (20)    15264 2018-03-30 00:51:34.000000 lsqfit-9.4/doc/html/_sources/lsqfit.rst.txt
--rw-r--r--   0 gpl        (503) staff       (20)      557 2017-01-09 17:45:08.000000 lsqfit-9.4/doc/html/_sources/index.rst.txt
--rw-r--r--   0 gpl        (503) staff       (20)    12454 2017-01-09 17:45:07.000000 lsqfit-9.4/doc/html/_sources/case-outliers.rst.txt
--rw-r--r--   0 gpl        (503) staff       (20)    89266 2018-02-19 19:16:53.000000 lsqfit-9.4/doc/html/_sources/overview.rst.txt
--rw-r--r--   0 gpl        (503) staff       (20)      757 2017-01-09 17:45:08.000000 lsqfit-9.4/doc/html/_sources/scipy.rst.txt
--rw-r--r--   0 gpl        (503) staff       (20)     4090 2018-07-08 20:26:40.000000 lsqfit-9.4/doc/html/py-modindex.html
--rw-r--r--   0 gpl        (503) staff       (20)    31585 2018-07-08 20:26:39.000000 lsqfit-9.4/doc/html/gsl.html
-drwxr-xr-x   0 gpl        (503) staff       (20)        0 2018-07-08 20:40:45.000000 lsqfit-9.4/doc/html/_static/
--rw-r--r--   0 gpl        (503) staff       (20)      190 2018-04-14 14:27:05.000000 lsqfit-9.4/doc/html/_static/headerbg.png
--rw-r--r--   0 gpl        (503) staff       (20)       90 2018-04-14 14:27:04.000000 lsqfit-9.4/doc/html/_static/plus.png
--rw-r--r--   0 gpl        (503) staff       (20)      222 2018-04-14 14:27:04.000000 lsqfit-9.4/doc/html/_static/down-pressed.png
--rw-r--r--   0 gpl        (503) staff       (20)   268039 2018-04-21 10:37:14.000000 lsqfit-9.4/doc/html/_static/jquery-3.2.1.js
--rw-r--r--   0 gpl        (503) staff       (20)    12140 2018-03-26 12:10:55.000000 lsqfit-9.4/doc/html/_static/underscore.js
--rw-r--r--   0 gpl        (503) staff       (20)      673 2018-03-26 12:10:55.000000 lsqfit-9.4/doc/html/_static/ajax-loader.gif
--rw-r--r--   0 gpl        (503) staff       (20)      197 2018-07-08 20:26:40.000000 lsqfit-9.4/doc/html/_static/documentation_options.js
--rw-r--r--   0 gpl        (503) staff       (20)     1280 2018-04-14 14:27:05.000000 lsqfit-9.4/doc/html/_static/dialog-warning.png
--rw-r--r--   0 gpl        (503) staff       (20)    25449 2018-07-08 20:26:41.000000 lsqfit-9.4/doc/html/_static/searchtools.js
--rw-r--r--   0 gpl        (503) staff       (20)      203 2018-04-14 14:27:04.000000 lsqfit-9.4/doc/html/_static/up.png
--rw-r--r--   0 gpl        (503) staff       (20)      286 2018-04-14 14:27:04.000000 lsqfit-9.4/doc/html/_static/file.png
--rw-r--r--   0 gpl        (503) staff       (20)      214 2018-04-14 14:27:04.000000 lsqfit-9.4/doc/html/_static/up-pressed.png
--rw-r--r--   0 gpl        (503) staff       (20)      202 2018-04-14 14:27:04.000000 lsqfit-9.4/doc/html/_static/down.png
--rw-r--r--   0 gpl        (503) staff       (20)       49 2018-03-26 12:10:55.000000 lsqfit-9.4/doc/html/_static/transparent.gif
--rw-r--r--   0 gpl        (503) staff       (20)    35168 2018-04-14 14:27:04.000000 lsqfit-9.4/doc/html/_static/underscore-1.3.1.js
--rw-r--r--   0 gpl        (503) staff       (20)      726 2018-03-26 12:10:55.000000 lsqfit-9.4/doc/html/_static/ie6.css
--rw-r--r--   0 gpl        (503) staff       (20)       90 2018-04-14 14:27:04.000000 lsqfit-9.4/doc/html/_static/minus.png
--rw-r--r--   0 gpl        (503) staff       (20)     1186 2018-04-14 14:27:05.000000 lsqfit-9.4/doc/html/_static/dialog-todo.png
--rw-r--r--   0 gpl        (503) staff       (20)     5602 2018-04-21 10:37:14.000000 lsqfit-9.4/doc/html/_static/epub.css
--rw-r--r--   0 gpl        (503) staff       (20)     6335 2018-07-08 20:26:41.000000 lsqfit-9.4/doc/html/_static/pyramid.css
--rw-r--r--   0 gpl        (503) staff       (20)      641 2018-04-14 14:27:04.000000 lsqfit-9.4/doc/html/_static/comment.png
--rw-r--r--   0 gpl        (503) staff       (20)    10716 2018-07-08 20:26:41.000000 lsqfit-9.4/doc/html/_static/basic.css
--rw-r--r--   0 gpl        (503) staff       (20)     1351 2018-04-14 14:27:05.000000 lsqfit-9.4/doc/html/_static/dialog-seealso.png
--rw-r--r--   0 gpl        (503) staff       (20)      333 2018-03-26 12:10:55.000000 lsqfit-9.4/doc/html/_static/footerbg.png
--rw-r--r--   0 gpl        (503) staff       (20)     1798 2018-04-14 14:27:05.000000 lsqfit-9.4/doc/html/_static/dialog-topic.png
--rw-r--r--   0 gpl        (503) staff       (20)      101 2018-04-14 14:27:05.000000 lsqfit-9.4/doc/html/_static/middlebg.png
--rw-r--r--   0 gpl        (503) staff       (20)     4395 2018-07-08 20:26:40.000000 lsqfit-9.4/doc/html/_static/pygments.css
--rw-r--r--   0 gpl        (503) staff       (20)      829 2018-04-14 14:27:04.000000 lsqfit-9.4/doc/html/_static/comment-close.png
--rw-r--r--   0 gpl        (503) staff       (20)     1394 2018-04-14 14:27:05.000000 lsqfit-9.4/doc/html/_static/dialog-note.png
--rw-r--r--   0 gpl        (503) staff       (20)     9224 2018-07-08 20:26:40.000000 lsqfit-9.4/doc/html/_static/doctools.js
--rw-r--r--   0 gpl        (503) staff       (20)      756 2018-04-14 14:27:04.000000 lsqfit-9.4/doc/html/_static/comment-bright.png
--rw-r--r--   0 gpl        (503) staff       (20)    25355 2018-04-21 10:37:14.000000 lsqfit-9.4/doc/html/_static/websupport.js
--rw-r--r--   0 gpl        (503) staff       (20)    86659 2018-04-21 10:37:14.000000 lsqfit-9.4/doc/html/_static/jquery.js
--rw-r--r--   0 gpl        (503) staff       (20)   416466 2018-07-08 20:26:40.000000 lsqfit-9.4/doc/html/overview.html
--rw-r--r--   0 gpl        (503) staff       (20)      230 2018-07-08 20:26:41.000000 lsqfit-9.4/doc/html/.buildinfo
-drwxr-xr-x   0 gpl        (503) staff       (20)        0 2018-07-08 20:40:45.000000 lsqfit-9.4/doc/html/_images/
--rw-r--r--   0 gpl        (503) staff       (20)    14564 2017-01-09 17:45:07.000000 lsqfit-9.4/doc/html/_images/case-pendulum.png
--rw-r--r--   0 gpl        (503) staff       (20)    24033 2017-05-04 21:49:33.000000 lsqfit-9.4/doc/html/_images/eg-appendix1d.png
--rw-r--r--   0 gpl        (503) staff       (20)    18140 2017-01-09 17:45:07.000000 lsqfit-9.4/doc/html/_images/case-outliers1.png
--rw-r--r--   0 gpl        (503) staff       (20)    21412 2017-05-04 21:49:23.000000 lsqfit-9.4/doc/html/_images/eg-appendix1a.png
--rw-r--r--   0 gpl        (503) staff       (20)    27801 2017-01-09 17:45:07.000000 lsqfit-9.4/doc/html/_images/case-outliers2.png
--rw-r--r--   0 gpl        (503) staff       (20)    20998 2017-05-04 21:49:28.000000 lsqfit-9.4/doc/html/_images/eg-appendix1b.png
--rw-r--r--   0 gpl        (503) staff       (20)    12122 2017-05-04 21:49:30.000000 lsqfit-9.4/doc/html/_images/eg-appendix1c.png
--rw-r--r--   0 gpl        (503) staff       (20)    20077 2017-01-09 17:45:07.000000 lsqfit-9.4/doc/html/_images/eg3d.png
--rw-r--r--   0 gpl        (503) staff       (20)    40187 2017-01-09 17:45:07.000000 lsqfit-9.4/doc/html/_images/eg3e.png
--rw-r--r--   0 gpl        (503) staff       (20)    15462 2017-01-09 17:45:07.000000 lsqfit-9.4/doc/html/_images/eg3.png
--rw-r--r--   0 gpl        (503) staff       (20)    16438 2017-01-09 17:45:07.000000 lsqfit-9.4/doc/html/_images/eg2.png
--rw-r--r--   0 gpl        (503) staff       (20)    10831 2017-02-21 04:30:16.000000 lsqfit-9.4/doc/html/_images/eg1.png
--rw-r--r--   0 gpl        (503) staff       (20)    34279 2017-01-09 17:45:07.000000 lsqfit-9.4/doc/html/_images/eg5.png
--rw-r--r--   0 gpl        (503) staff       (20)    17680 2018-02-19 19:08:00.000000 lsqfit-9.4/doc/html/_images/eg6.png
--rw-r--r--   0 gpl        (503) staff       (20)    66498 2018-07-08 20:26:39.000000 lsqfit-9.4/doc/html/case-outliers.html
--rw-r--r--   0 gpl        (503) staff       (20)    33235 2018-07-08 20:26:39.000000 lsqfit-9.4/doc/html/case-pendulum.html
--rw-r--r--   0 gpl        (503) staff       (20)    17051 2018-07-08 20:26:40.000000 lsqfit-9.4/doc/html/genindex.html
--rw-r--r--   0 gpl        (503) staff       (20)   226511 2018-07-08 20:26:40.000000 lsqfit-9.4/doc/html/lsqfit.html
--rw-r--r--   0 gpl        (503) staff       (20)     4022 2018-07-08 20:26:40.000000 lsqfit-9.4/doc/html/search.html
-drwxr-xr-x   0 gpl        (503) staff       (20)        0 2018-07-08 20:40:45.000000 lsqfit-9.4/doc/html/.doctrees/
--rw-r--r--   0 gpl        (503) staff       (20)    28886 2018-07-08 20:26:37.000000 lsqfit-9.4/doc/html/.doctrees/case-pendulum.doctree
--rw-r--r--   0 gpl        (503) staff       (20)    94727 2018-07-08 20:26:36.000000 lsqfit-9.4/doc/html/.doctrees/case-extrapolation.doctree
--rw-r--r--   0 gpl        (503) staff       (20)   123341 2018-07-08 20:26:37.000000 lsqfit-9.4/doc/html/.doctrees/gsl.doctree
--rw-r--r--   0 gpl        (503) staff       (20)    91891 2018-07-08 20:26:39.000000 lsqfit-9.4/doc/html/.doctrees/testing.doctree
--rw-r--r--   0 gpl        (503) staff       (20)    37735 2018-07-08 20:26:39.000000 lsqfit-9.4/doc/html/.doctrees/environment.pickle
--rw-r--r--   0 gpl        (503) staff       (20)     5653 2018-07-08 20:26:37.000000 lsqfit-9.4/doc/html/.doctrees/index.doctree
--rw-r--r--   0 gpl        (503) staff       (20)   545164 2018-07-08 20:26:38.000000 lsqfit-9.4/doc/html/.doctrees/lsqfit.doctree
--rw-r--r--   0 gpl        (503) staff       (20)    50475 2018-07-08 20:26:37.000000 lsqfit-9.4/doc/html/.doctrees/case-outliers.doctree
--rw-r--r--   0 gpl        (503) staff       (20)    65567 2018-07-08 20:26:39.000000 lsqfit-9.4/doc/html/.doctrees/scipy.doctree
--rw-r--r--   0 gpl        (503) staff       (20)   462122 2018-07-08 20:26:39.000000 lsqfit-9.4/doc/html/.doctrees/overview.doctree
--rw-r--r--   0 gpl        (503) staff       (20)   124317 2018-07-08 20:26:40.000000 lsqfit-9.4/doc/html/testing.html
--rw-r--r--   0 gpl        (503) staff       (20)     1130 2018-07-08 20:26:41.000000 lsqfit-9.4/doc/html/objects.inv
--rw-r--r--   0 gpl        (503) staff       (20)     4663 2018-03-18 18:21:37.000000 lsqfit-9.4/INSTALLATION.txt
--rw-r--r--   0 gpl        (503) staff       (20)     1793 2018-07-08 20:21:48.000000 lsqfit-9.4/README.rst
--rw-r--r--   0 gpl        (503) staff       (20)    31996 2012-06-08 07:08:29.000000 lsqfit-9.4/LICENSE.txt
-drwxr-xr-x   0 gpl        (503) staff       (20)        0 2018-07-08 20:40:45.000000 lsqfit-9.4/src/
-drwxr-xr-x   0 gpl        (503) staff       (20)        0 2018-07-08 20:40:45.000000 lsqfit-9.4/src/lsqfit/
--rw-r--r--   0 gpl        (503) staff       (20)  1310204 2018-07-06 19:51:27.000000 lsqfit-9.4/src/lsqfit/_gsl.c
--rw-r--r--   0 gpl        (503) staff       (20)    89990 2018-06-16 22:07:34.000000 lsqfit-9.4/src/lsqfit/__init__.py
--rw-r--r--   0 gpl        (503) staff       (20)     8558 2017-09-23 20:50:51.000000 lsqfit-9.4/src/lsqfit/_scipy.py
--rw-r--r--   0 gpl        (503) staff       (20)    41384 2018-07-06 19:49:08.000000 lsqfit-9.4/src/lsqfit/_gsl.pyx
--rw-r--r--   0 gpl        (503) staff       (20)    60144 2018-03-30 00:46:38.000000 lsqfit-9.4/src/lsqfit/_extras.py
--rw-r--r--   0 gpl        (503) staff       (20)     5276 2018-07-08 20:23:32.000000 lsqfit-9.4/src/lsqfit/_utilities.pyx
--rw-r--r--   0 gpl        (503) staff       (20)  1238404 2018-07-08 20:24:49.000000 lsqfit-9.4/src/lsqfit/_utilities.c
+drwxr-xr-x   0 gpl        (503) staff       (20)        0 2018-07-15 18:36:18.000000 lsqfit-9.5/
+-rw-r--r--   0 gpl        (503) staff       (20)     3199 2018-07-15 18:36:18.000000 lsqfit-9.5/PKG-INFO
+-rw-r--r--   0 gpl        (503) staff       (20)     3274 2018-07-08 21:47:28.000000 lsqfit-9.5/makefile
+drwxr-xr-x   0 gpl        (503) staff       (20)        0 2018-07-15 18:36:18.000000 lsqfit-9.5/tests/
+-rw-r--r--   0 gpl        (503) staff       (20)    16954 2018-07-07 13:56:49.000000 lsqfit-9.5/tests/test_multifitter.py
+-rw-r--r--   0 gpl        (503) staff       (20)    71877 2018-07-14 21:47:09.000000 lsqfit-9.5/tests/test_lsqfit.py
+-rw-r--r--   0 gpl        (503) staff       (20)      989 2013-01-13 22:28:17.000000 lsqfit-9.5/tests/makefile
+-rw-r--r--   0 gpl        (503) staff       (20)      104 2012-06-18 04:03:00.000000 lsqfit-9.5/tests/__init__.py
+-rw-r--r--   0 gpl        (503) staff       (20)      395 2012-06-18 08:13:19.000000 lsqfit-9.5/tests/README
+-rw-r--r--   0 gpl        (503) staff       (20)      384 2018-03-30 14:28:05.000000 lsqfit-9.5/MANIFEST.in
+-rw-r--r--   0 gpl        (503) staff       (20)    46613 2018-07-15 18:26:06.000000 lsqfit-9.5/CHANGES.txt
+-rw-r--r--   0 gpl        (503) staff       (20)     4805 2018-07-15 18:29:38.000000 lsqfit-9.5/setup.py
+drwxr-xr-x   0 gpl        (503) staff       (20)        0 2018-07-15 18:36:18.000000 lsqfit-9.5/examples/
+-rw-r--r--   0 gpl        (503) staff       (20)     1187 2017-01-09 17:45:08.000000 lsqfit-9.5/examples/x-err.out
+-rw-r--r--   0 gpl        (503) staff       (20)    12053 2017-01-09 17:45:08.000000 lsqfit-9.5/examples/nist.out
+-rw-r--r--   0 gpl        (503) staff       (20)    12734 2016-08-15 18:23:44.000000 lsqfit-9.5/examples/pendulum.pdf
+-rw-r--r--   0 gpl        (503) staff       (20)     1363 2017-01-11 15:09:53.000000 lsqfit-9.5/examples/uncorrelated.py
+-rw-r--r--   0 gpl        (503) staff       (20)     5739 2017-02-07 04:04:01.000000 lsqfit-9.5/examples/y-noerr.out
+-rw-r--r--   0 gpl        (503) staff       (20)      435 2017-01-09 17:45:08.000000 lsqfit-9.5/examples/p-corr.out
+-rw-r--r--   0 gpl        (503) staff       (20)      580 2017-02-07 04:17:35.000000 lsqfit-9.5/examples/xxxx
+-rw-r--r--   0 gpl        (503) staff       (20)     4464 2017-01-09 17:45:08.000000 lsqfit-9.5/examples/y-vs-x.out
+-rw-r--r--   0 gpl        (503) staff       (20)    66290 2018-03-18 18:26:10.000000 lsqfit-9.5/examples/nist.py
+-rw-r--r--   0 gpl        (503) staff       (20)     1271 2017-01-09 17:45:08.000000 lsqfit-9.5/examples/empbayes.py
+-rw-r--r--   0 gpl        (503) staff       (20)      580 2017-02-07 04:11:43.000000 lsqfit-9.5/examples/xxx.out
+-rw-r--r--   0 gpl        (503) staff       (20)      580 2017-02-07 13:17:22.000000 lsqfit-9.5/examples/xxx
+-rw-r--r--   0 gpl        (503) staff       (20)     2552 2017-01-09 18:18:12.000000 lsqfit-9.5/examples/makefile
+-rw-r--r--   0 gpl        (503) staff       (20)      387 2017-01-09 17:45:08.000000 lsqfit-9.5/examples/uncorrelated.out
+-rw-r--r--   0 gpl        (503) staff       (20)      852 2017-01-09 17:45:08.000000 lsqfit-9.5/examples/pendulum.out
+-rw-r--r--   0 gpl        (503) staff       (20)     2148 2018-07-14 21:35:40.000000 lsqfit-9.5/examples/bayes.out
+-rw-r--r--   0 gpl        (503) staff       (20)     4593 2017-01-09 18:56:23.000000 lsqfit-9.5/examples/y-vs-x.py
+-rw-r--r--   0 gpl        (503) staff       (20)      798 2017-01-09 17:45:08.000000 lsqfit-9.5/examples/empbayes.out
+drwxr-xr-x   0 gpl        (503) staff       (20)        0 2018-07-15 18:36:18.000000 lsqfit-9.5/examples/nist/
+-rw-r--r--   0 gpl        (503) staff       (20)     2431 2017-01-09 17:45:08.000000 lsqfit-9.5/examples/nist/roszman1.txt
+-rw-r--r--   0 gpl        (503) staff       (20)     3025 2017-01-09 17:45:08.000000 lsqfit-9.5/examples/nist/thurber.txt
+-rw-r--r--   0 gpl        (503) staff       (20)     6868 2017-01-09 17:45:08.000000 lsqfit-9.5/examples/nist/bennett5.txt
+-rw-r--r--   0 gpl        (503) staff       (20)     1838 2017-01-09 17:45:08.000000 lsqfit-9.5/examples/nist/misra1c.txt
+-rw-r--r--   0 gpl        (503) staff       (20)     6760 2017-01-09 17:45:08.000000 lsqfit-9.5/examples/nist/enso.txt
+-rw-r--r--   0 gpl        (503) staff       (20)     7000 2017-01-09 17:45:08.000000 lsqfit-9.5/examples/nist/nelson.txt
+-rw-r--r--   0 gpl        (503) staff       (20)     2573 2017-01-09 17:45:08.000000 lsqfit-9.5/examples/nist/lanczos3.txt
+-rw-r--r--   0 gpl        (503) staff       (20)     2600 2017-01-09 17:45:08.000000 lsqfit-9.5/examples/nist/lanczos2.txt
+-rw-r--r--   0 gpl        (503) staff       (20)     1844 2017-01-09 17:45:08.000000 lsqfit-9.5/examples/nist/misra1b.txt
+-rw-r--r--   0 gpl        (503) staff       (20)    64851 2018-03-18 18:27:36.000000 lsqfit-9.5/examples/nist/1st_nist.py
+-rw-r--r--   0 gpl        (503) staff       (20)     1872 2017-01-09 17:45:08.000000 lsqfit-9.5/examples/nist/rat42.txt
+-rw-r--r--   0 gpl        (503) staff       (20)     2944 2017-01-09 17:45:08.000000 lsqfit-9.5/examples/nist/lanczos1.txt
+-rw-r--r--   0 gpl        (503) staff       (20)     2071 2017-01-09 17:45:08.000000 lsqfit-9.5/examples/nist/rat43.txt
+-rw-r--r--   0 gpl        (503) staff       (20)     1852 2017-01-09 17:45:08.000000 lsqfit-9.5/examples/nist/misra1a.txt
+-rw-r--r--   0 gpl        (503) staff       (20)     1842 2017-01-09 17:45:08.000000 lsqfit-9.5/examples/nist/misra1d.txt
+-rw-r--r--   0 gpl        (503) staff       (20)     1712 2017-01-09 17:45:08.000000 lsqfit-9.5/examples/nist/boxbod.txt
+-rw-r--r--   0 gpl        (503) staff       (20)     2304 2017-01-09 17:45:08.000000 lsqfit-9.5/examples/nist/mgh09.txt
+-rw-r--r--   0 gpl        (503) staff       (20)     2334 2017-01-09 17:45:08.000000 lsqfit-9.5/examples/nist/mgh10.txt
+-rw-r--r--   0 gpl        (503) staff       (20)     6800 2017-02-06 20:28:57.000000 lsqfit-9.5/examples/nist/make_script.py
+-rw-r--r--   0 gpl        (503) staff       (20)     3077 2017-01-09 17:45:08.000000 lsqfit-9.5/examples/nist/mgh17.txt
+-rw-r--r--   0 gpl        (503) staff       (20)     9275 2017-01-09 17:45:08.000000 lsqfit-9.5/examples/nist/hahn1.txt
+-rw-r--r--   0 gpl        (503) staff       (20)     8097 2017-01-09 17:45:08.000000 lsqfit-9.5/examples/nist/gauss1.txt
+-rw-r--r--   0 gpl        (503) staff       (20)     2772 2017-01-09 17:45:08.000000 lsqfit-9.5/examples/nist/eckerle4.txt
+-rw-r--r--   0 gpl        (503) staff       (20)     8099 2017-01-09 17:45:08.000000 lsqfit-9.5/examples/nist/gauss2.txt
+-rw-r--r--   0 gpl        (503) staff       (20)     5857 2017-01-09 17:45:08.000000 lsqfit-9.5/examples/nist/kirby2.txt
+-rw-r--r--   0 gpl        (503) staff       (20)     8101 2017-01-09 17:45:08.000000 lsqfit-9.5/examples/nist/gauss3.txt
+-rw-r--r--   0 gpl        (503) staff       (20)    64931 2018-03-18 18:28:07.000000 lsqfit-9.5/examples/nist/2nd_nist.py
+-rw-r--r--   0 gpl        (503) staff       (20)     3059 2017-01-09 17:45:08.000000 lsqfit-9.5/examples/nist/chwirut2.txt
+-rw-r--r--   0 gpl        (503) staff       (20)     1989 2017-01-09 17:45:08.000000 lsqfit-9.5/examples/nist/danwood.txt
+-rw-r--r--   0 gpl        (503) staff       (20)     7557 2017-01-09 17:45:08.000000 lsqfit-9.5/examples/nist/chwirut1.txt
+-rw-r--r--   0 gpl        (503) staff       (20)      754 2017-01-09 17:45:08.000000 lsqfit-9.5/examples/README
+-rw-r--r--   0 gpl        (503) staff       (20)     1670 2017-01-09 17:45:08.000000 lsqfit-9.5/examples/p-corr.py
+-rw-r--r--   0 gpl        (503) staff       (20)     2758 2017-05-04 17:42:04.000000 lsqfit-9.5/examples/bayes.py
+-rw-r--r--   0 gpl        (503) staff       (20)     1662 2017-01-09 18:49:37.000000 lsqfit-9.5/examples/x-err.py
+-rw-r--r--   0 gpl        (503) staff       (20)      973 2017-01-09 17:45:08.000000 lsqfit-9.5/examples/simple.out
+-rw-r--r--   0 gpl        (503) staff       (20)     2222 2014-06-26 08:07:55.000000 lsqfit-9.5/examples/simple.py
+-rw-r--r--   0 gpl        (503) staff       (20)     4744 2016-08-15 01:11:44.000000 lsqfit-9.5/examples/pendulum.py
+-rw-r--r--   0 gpl        (503) staff       (20)      547 2018-07-15 18:34:15.000000 lsqfit-9.5/examples/outputfile.p
+-rw-r--r--   0 gpl        (503) staff       (20)     4459 2013-04-10 16:01:02.000000 lsqfit-9.5/examples/xxx.py
+-rw-r--r--   0 gpl        (503) staff       (20)      828 2013-04-10 02:20:15.000000 lsqfit-9.5/examples/yyy.py
+-rw-r--r--   0 gpl        (503) staff       (20)     2468 2017-02-07 04:03:39.000000 lsqfit-9.5/examples/y-noerr.py
+drwxr-xr-x   0 gpl        (503) staff       (20)        0 2018-07-15 18:36:17.000000 lsqfit-9.5/doc/
+drwxr-xr-x   0 gpl        (503) staff       (20)        0 2018-07-15 18:36:17.000000 lsqfit-9.5/doc/html/
+-rw-r--r--   0 gpl        (503) staff       (20)   140100 2018-07-15 18:34:44.000000 lsqfit-9.5/doc/html/case-extrapolation.html
+-rw-r--r--   0 gpl        (503) staff       (20)    11453 2018-07-15 18:34:45.000000 lsqfit-9.5/doc/html/index.html
+-rw-r--r--   0 gpl        (503) staff       (20)    23714 2018-07-15 18:34:46.000000 lsqfit-9.5/doc/html/searchindex.js
+-rw-r--r--   0 gpl        (503) staff       (20)    21666 2018-07-15 18:34:46.000000 lsqfit-9.5/doc/html/scipy.html
+drwxr-xr-x   0 gpl        (503) staff       (20)        0 2018-07-15 18:36:18.000000 lsqfit-9.5/doc/html/_sources/
+-rw-r--r--   0 gpl        (503) staff       (20)     5977 2017-01-09 17:45:07.000000 lsqfit-9.5/doc/html/_sources/case-pendulum.rst.txt
+-rw-r--r--   0 gpl        (503) staff       (20)    12347 2018-02-18 01:57:24.000000 lsqfit-9.5/doc/html/_sources/gsl.rst.txt
+-rw-r--r--   0 gpl        (503) staff       (20)    12613 2017-01-09 17:45:07.000000 lsqfit-9.5/doc/html/_sources/case-extrapolation.rst.txt
+-rw-r--r--   0 gpl        (503) staff       (20)    19810 2017-01-09 17:45:08.000000 lsqfit-9.5/doc/html/_sources/testing.rst.txt
+-rw-r--r--   0 gpl        (503) staff       (20)    15127 2018-07-14 22:01:27.000000 lsqfit-9.5/doc/html/_sources/lsqfit.rst.txt
+-rw-r--r--   0 gpl        (503) staff       (20)      557 2017-01-09 17:45:08.000000 lsqfit-9.5/doc/html/_sources/index.rst.txt
+-rw-r--r--   0 gpl        (503) staff       (20)    12454 2017-01-09 17:45:07.000000 lsqfit-9.5/doc/html/_sources/case-outliers.rst.txt
+-rw-r--r--   0 gpl        (503) staff       (20)    89266 2018-02-19 19:16:53.000000 lsqfit-9.5/doc/html/_sources/overview.rst.txt
+-rw-r--r--   0 gpl        (503) staff       (20)      757 2017-01-09 17:45:08.000000 lsqfit-9.5/doc/html/_sources/scipy.rst.txt
+-rw-r--r--   0 gpl        (503) staff       (20)     4090 2018-07-15 18:34:46.000000 lsqfit-9.5/doc/html/py-modindex.html
+-rw-r--r--   0 gpl        (503) staff       (20)    31585 2018-07-15 18:34:44.000000 lsqfit-9.5/doc/html/gsl.html
+drwxr-xr-x   0 gpl        (503) staff       (20)        0 2018-07-15 18:36:18.000000 lsqfit-9.5/doc/html/_static/
+-rw-r--r--   0 gpl        (503) staff       (20)      190 2018-04-14 14:27:05.000000 lsqfit-9.5/doc/html/_static/headerbg.png
+-rw-r--r--   0 gpl        (503) staff       (20)       90 2018-04-14 14:27:04.000000 lsqfit-9.5/doc/html/_static/plus.png
+-rw-r--r--   0 gpl        (503) staff       (20)      222 2018-04-14 14:27:04.000000 lsqfit-9.5/doc/html/_static/down-pressed.png
+-rw-r--r--   0 gpl        (503) staff       (20)   268039 2018-04-21 10:37:14.000000 lsqfit-9.5/doc/html/_static/jquery-3.2.1.js
+-rw-r--r--   0 gpl        (503) staff       (20)    12140 2018-03-26 12:10:55.000000 lsqfit-9.5/doc/html/_static/underscore.js
+-rw-r--r--   0 gpl        (503) staff       (20)      673 2018-03-26 12:10:55.000000 lsqfit-9.5/doc/html/_static/ajax-loader.gif
+-rw-r--r--   0 gpl        (503) staff       (20)      197 2018-07-15 18:34:46.000000 lsqfit-9.5/doc/html/_static/documentation_options.js
+-rw-r--r--   0 gpl        (503) staff       (20)     1280 2018-04-14 14:27:05.000000 lsqfit-9.5/doc/html/_static/dialog-warning.png
+-rw-r--r--   0 gpl        (503) staff       (20)    25449 2018-07-15 18:34:46.000000 lsqfit-9.5/doc/html/_static/searchtools.js
+-rw-r--r--   0 gpl        (503) staff       (20)      203 2018-04-14 14:27:04.000000 lsqfit-9.5/doc/html/_static/up.png
+-rw-r--r--   0 gpl        (503) staff       (20)      286 2018-04-14 14:27:04.000000 lsqfit-9.5/doc/html/_static/file.png
+-rw-r--r--   0 gpl        (503) staff       (20)      214 2018-04-14 14:27:04.000000 lsqfit-9.5/doc/html/_static/up-pressed.png
+-rw-r--r--   0 gpl        (503) staff       (20)      202 2018-04-14 14:27:04.000000 lsqfit-9.5/doc/html/_static/down.png
+-rw-r--r--   0 gpl        (503) staff       (20)       49 2018-03-26 12:10:55.000000 lsqfit-9.5/doc/html/_static/transparent.gif
+-rw-r--r--   0 gpl        (503) staff       (20)    35168 2018-04-14 14:27:04.000000 lsqfit-9.5/doc/html/_static/underscore-1.3.1.js
+-rw-r--r--   0 gpl        (503) staff       (20)      726 2018-03-26 12:10:55.000000 lsqfit-9.5/doc/html/_static/ie6.css
+-rw-r--r--   0 gpl        (503) staff       (20)       90 2018-04-14 14:27:04.000000 lsqfit-9.5/doc/html/_static/minus.png
+-rw-r--r--   0 gpl        (503) staff       (20)     1186 2018-04-14 14:27:05.000000 lsqfit-9.5/doc/html/_static/dialog-todo.png
+-rw-r--r--   0 gpl        (503) staff       (20)     5602 2018-04-21 10:37:14.000000 lsqfit-9.5/doc/html/_static/epub.css
+-rw-r--r--   0 gpl        (503) staff       (20)     6335 2018-07-15 18:34:46.000000 lsqfit-9.5/doc/html/_static/pyramid.css
+-rw-r--r--   0 gpl        (503) staff       (20)      641 2018-04-14 14:27:04.000000 lsqfit-9.5/doc/html/_static/comment.png
+-rw-r--r--   0 gpl        (503) staff       (20)    10716 2018-07-15 18:34:46.000000 lsqfit-9.5/doc/html/_static/basic.css
+-rw-r--r--   0 gpl        (503) staff       (20)     1351 2018-04-14 14:27:05.000000 lsqfit-9.5/doc/html/_static/dialog-seealso.png
+-rw-r--r--   0 gpl        (503) staff       (20)      333 2018-03-26 12:10:55.000000 lsqfit-9.5/doc/html/_static/footerbg.png
+-rw-r--r--   0 gpl        (503) staff       (20)     1798 2018-04-14 14:27:05.000000 lsqfit-9.5/doc/html/_static/dialog-topic.png
+-rw-r--r--   0 gpl        (503) staff       (20)      101 2018-04-14 14:27:05.000000 lsqfit-9.5/doc/html/_static/middlebg.png
+-rw-r--r--   0 gpl        (503) staff       (20)     4395 2018-07-15 18:34:46.000000 lsqfit-9.5/doc/html/_static/pygments.css
+-rw-r--r--   0 gpl        (503) staff       (20)      829 2018-04-14 14:27:04.000000 lsqfit-9.5/doc/html/_static/comment-close.png
+-rw-r--r--   0 gpl        (503) staff       (20)     1394 2018-04-14 14:27:05.000000 lsqfit-9.5/doc/html/_static/dialog-note.png
+-rw-r--r--   0 gpl        (503) staff       (20)     9224 2018-07-15 18:34:46.000000 lsqfit-9.5/doc/html/_static/doctools.js
+-rw-r--r--   0 gpl        (503) staff       (20)      756 2018-04-14 14:27:04.000000 lsqfit-9.5/doc/html/_static/comment-bright.png
+-rw-r--r--   0 gpl        (503) staff       (20)    25355 2018-04-21 10:37:14.000000 lsqfit-9.5/doc/html/_static/websupport.js
+-rw-r--r--   0 gpl        (503) staff       (20)    86659 2018-04-21 10:37:14.000000 lsqfit-9.5/doc/html/_static/jquery.js
+-rw-r--r--   0 gpl        (503) staff       (20)   416466 2018-07-15 18:34:45.000000 lsqfit-9.5/doc/html/overview.html
+-rw-r--r--   0 gpl        (503) staff       (20)      230 2018-07-15 18:34:46.000000 lsqfit-9.5/doc/html/.buildinfo
+drwxr-xr-x   0 gpl        (503) staff       (20)        0 2018-07-15 18:36:18.000000 lsqfit-9.5/doc/html/_images/
+-rw-r--r--   0 gpl        (503) staff       (20)    14564 2017-01-09 17:45:07.000000 lsqfit-9.5/doc/html/_images/case-pendulum.png
+-rw-r--r--   0 gpl        (503) staff       (20)    24033 2017-05-04 21:49:33.000000 lsqfit-9.5/doc/html/_images/eg-appendix1d.png
+-rw-r--r--   0 gpl        (503) staff       (20)    18140 2017-01-09 17:45:07.000000 lsqfit-9.5/doc/html/_images/case-outliers1.png
+-rw-r--r--   0 gpl        (503) staff       (20)    21412 2017-05-04 21:49:23.000000 lsqfit-9.5/doc/html/_images/eg-appendix1a.png
+-rw-r--r--   0 gpl        (503) staff       (20)    27801 2017-01-09 17:45:07.000000 lsqfit-9.5/doc/html/_images/case-outliers2.png
+-rw-r--r--   0 gpl        (503) staff       (20)    20998 2017-05-04 21:49:28.000000 lsqfit-9.5/doc/html/_images/eg-appendix1b.png
+-rw-r--r--   0 gpl        (503) staff       (20)    12122 2017-05-04 21:49:30.000000 lsqfit-9.5/doc/html/_images/eg-appendix1c.png
+-rw-r--r--   0 gpl        (503) staff       (20)    20077 2017-01-09 17:45:07.000000 lsqfit-9.5/doc/html/_images/eg3d.png
+-rw-r--r--   0 gpl        (503) staff       (20)    40187 2017-01-09 17:45:07.000000 lsqfit-9.5/doc/html/_images/eg3e.png
+-rw-r--r--   0 gpl        (503) staff       (20)    15462 2017-01-09 17:45:07.000000 lsqfit-9.5/doc/html/_images/eg3.png
+-rw-r--r--   0 gpl        (503) staff       (20)    16438 2017-01-09 17:45:07.000000 lsqfit-9.5/doc/html/_images/eg2.png
+-rw-r--r--   0 gpl        (503) staff       (20)    10831 2017-02-21 04:30:16.000000 lsqfit-9.5/doc/html/_images/eg1.png
+-rw-r--r--   0 gpl        (503) staff       (20)    34279 2017-01-09 17:45:07.000000 lsqfit-9.5/doc/html/_images/eg5.png
+-rw-r--r--   0 gpl        (503) staff       (20)    17680 2018-02-19 19:08:00.000000 lsqfit-9.5/doc/html/_images/eg6.png
+-rw-r--r--   0 gpl        (503) staff       (20)    66498 2018-07-15 18:34:44.000000 lsqfit-9.5/doc/html/case-outliers.html
+-rw-r--r--   0 gpl        (503) staff       (20)    33235 2018-07-15 18:34:44.000000 lsqfit-9.5/doc/html/case-pendulum.html
+-rw-r--r--   0 gpl        (503) staff       (20)    16691 2018-07-15 18:34:46.000000 lsqfit-9.5/doc/html/genindex.html
+-rw-r--r--   0 gpl        (503) staff       (20)   223573 2018-07-15 18:34:45.000000 lsqfit-9.5/doc/html/lsqfit.html
+-rw-r--r--   0 gpl        (503) staff       (20)     4022 2018-07-15 18:34:46.000000 lsqfit-9.5/doc/html/search.html
+drwxr-xr-x   0 gpl        (503) staff       (20)        0 2018-07-15 18:36:17.000000 lsqfit-9.5/doc/html/.doctrees/
+-rw-r--r--   0 gpl        (503) staff       (20)    28886 2018-07-15 18:34:42.000000 lsqfit-9.5/doc/html/.doctrees/case-pendulum.doctree
+-rw-r--r--   0 gpl        (503) staff       (20)    94727 2018-07-15 18:34:42.000000 lsqfit-9.5/doc/html/.doctrees/case-extrapolation.doctree
+-rw-r--r--   0 gpl        (503) staff       (20)   123341 2018-07-15 18:34:42.000000 lsqfit-9.5/doc/html/.doctrees/gsl.doctree
+-rw-r--r--   0 gpl        (503) staff       (20)    91891 2018-07-15 18:34:44.000000 lsqfit-9.5/doc/html/.doctrees/testing.doctree
+-rw-r--r--   0 gpl        (503) staff       (20)    37339 2018-07-15 18:34:44.000000 lsqfit-9.5/doc/html/.doctrees/environment.pickle
+-rw-r--r--   0 gpl        (503) staff       (20)     5653 2018-07-15 18:34:42.000000 lsqfit-9.5/doc/html/.doctrees/index.doctree
+-rw-r--r--   0 gpl        (503) staff       (20)   538344 2018-07-15 18:34:43.000000 lsqfit-9.5/doc/html/.doctrees/lsqfit.doctree
+-rw-r--r--   0 gpl        (503) staff       (20)    50475 2018-07-15 18:34:42.000000 lsqfit-9.5/doc/html/.doctrees/case-outliers.doctree
+-rw-r--r--   0 gpl        (503) staff       (20)    65532 2018-07-15 18:34:44.000000 lsqfit-9.5/doc/html/.doctrees/scipy.doctree
+-rw-r--r--   0 gpl        (503) staff       (20)   462122 2018-07-15 18:34:44.000000 lsqfit-9.5/doc/html/.doctrees/overview.doctree
+-rw-r--r--   0 gpl        (503) staff       (20)   124317 2018-07-15 18:34:46.000000 lsqfit-9.5/doc/html/testing.html
+-rw-r--r--   0 gpl        (503) staff       (20)     1109 2018-07-15 18:34:46.000000 lsqfit-9.5/doc/html/objects.inv
+-rw-r--r--   0 gpl        (503) staff       (20)     4663 2018-03-18 18:21:37.000000 lsqfit-9.5/INSTALLATION.txt
+-rw-r--r--   0 gpl        (503) staff       (20)     1793 2018-07-08 20:21:48.000000 lsqfit-9.5/README.rst
+-rw-r--r--   0 gpl        (503) staff       (20)    31996 2012-06-08 07:08:29.000000 lsqfit-9.5/LICENSE.txt
+drwxr-xr-x   0 gpl        (503) staff       (20)        0 2018-07-15 18:36:17.000000 lsqfit-9.5/src/
+drwxr-xr-x   0 gpl        (503) staff       (20)        0 2018-07-15 18:36:18.000000 lsqfit-9.5/src/lsqfit/
+-rw-r--r--   0 gpl        (503) staff       (20)  1310204 2018-07-06 19:51:27.000000 lsqfit-9.5/src/lsqfit/_gsl.c
+-rw-r--r--   0 gpl        (503) staff       (20)    95068 2018-07-14 22:18:37.000000 lsqfit-9.5/src/lsqfit/__init__.py
+-rw-r--r--   0 gpl        (503) staff       (20)     8558 2017-09-23 20:50:51.000000 lsqfit-9.5/src/lsqfit/_scipy.py
+-rw-r--r--   0 gpl        (503) staff       (20)    41384 2018-07-06 19:49:08.000000 lsqfit-9.5/src/lsqfit/_gsl.pyx
+-rw-r--r--   0 gpl        (503) staff       (20)    61415 2018-07-13 01:48:02.000000 lsqfit-9.5/src/lsqfit/_extras.py
+-rw-r--r--   0 gpl        (503) staff       (20)     5276 2018-07-08 20:23:32.000000 lsqfit-9.5/src/lsqfit/_utilities.pyx
+-rw-r--r--   0 gpl        (503) staff       (20)  1238404 2018-07-08 20:24:49.000000 lsqfit-9.5/src/lsqfit/_utilities.c
```

### Comparing `lsqfit-9.4/PKG-INFO` & `lsqfit-9.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: lsqfit
-Version: 9.4
+Version: 9.5
 Summary: Utilities for nonlinear least-squares fits.
 Home-page: https://github.com/gplepage/lsqfit.git
 Author: G. Peter Lepage
 Author-email: g.p.lepage@cornell.edu
 License: GPLv3+
 Description: lsqfit
         ------
```

### Comparing `lsqfit-9.4/makefile` & `lsqfit-9.5/makefile`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 
 PIP = python -m pip
 PYTHON = python
 PYTHONVERSION = python`python -c 'import platform; print(platform.python_version())'`
-VERSION = `python -c 'import lsqfit; print lsqfit.__version__'`
+VERSION = `python -c 'import lsqfit; print (lsqfit.__version__)'`
 
 DOCFILES :=  $(shell ls doc/source/conf.py doc/source/*.{rst,out,png} 2>/dev/null)
 SRCFILES := $(shell ls setup.py src/lsqfit/*.{py,pyx})
 CYTHONFILES := src/lsqfit/_gsl.c src/lsqfit/_utilities.c
 
 install-user : $(CYTHONFILES)
 	$(PIP) install . --user
```

### Comparing `lsqfit-9.4/tests/test_multifitter.py` & `lsqfit-9.5/tests/test_multifitter.py`

 * *Files identical despite different names*

### Comparing `lsqfit-9.4/tests/test_lsqfit.py` & `lsqfit-9.5/tests/test_lsqfit.py`

 * *Files 1% similar despite different names*

```diff
@@ -128,14 +128,17 @@
         pr = gv.BufferDict()
         pcov = np.array([[2., .5], [.5, 1.]]) * pfac
         pr['p'] = gv.gvar([4., 16.], pcov)
         def fcn(x,p):
             return dict(y=p['p'] ** 2)
         y = dict(y=y)
         fit = nonlinear_fit(data=(None,y), prior=pr, fcn=fcn, p0=p0file, debug=True)
+        with open(p0file, 'rb') as f:
+            p0 = pickle.load(f)
+            self.assert_arraysclose(p0['p'], fit.pmean['p'])
         print_fit(fit,dict(y=wavg(fit.p['p']**2)))
         self.assertEqual(fit.dof, 2)
         self.assertAlmostEqual(fit.Q, 1.0)
         self.assertAlmostEqual(fit.chi2, 0.0)
         cd = {'data':fit.y, 'priors':fit.prior, 'p':[fit.prior['p']]}
         err = {}
         err['data'] = fit.p['p'][1].partialsdev(fit.y)
@@ -1232,29 +1235,29 @@
         self.assertEqual(newp[3],40)
         with self.assertRaises(ValueError):
             lsqfit._reformat(p,[10,20])
         with self.assertRaises(ValueError):
             lsqfit._reformat(p,[[10,20,30,40]])
 
 
-    def test_dump(self):
-        y = {0 : gv.gvar(1,2), 1 : gv.gvar(3,4)}
-        prior = {0 : gv.gvar(1.5, 1)}
-        def f(p):
-            return {0:p[0],1:p[0]}
-
-        fit = nonlinear_fit(data=y,prior=prior,fcn=f)
-        fit.dump_p("test-lsqfit.p")
-        p = nonlinear_fit.load_parameters("test-lsqfit.p")
-        self.assert_gvclose(p[0],fit.p[0])
-        self.assert_gvclose(p[0],wavg([y[0],y[1],prior[0]]))
-        fit.dump_pmean("test-lsqfit.p")
-        pmean = fit.load_parameters("test-lsqfit.p")
-        self.assertAlmostEqual(pmean[0],fit.pmean[0])
-        os.remove("test-lsqfit.p")
+    # def test_dump(self):
+    #     y = {0 : gv.gvar(1,2), 1 : gv.gvar(3,4)}
+    #     prior = {0 : gv.gvar(1.5, 1)}
+    #     def f(p):
+    #         return {0:p[0],1:p[0]}
+
+    #     fit = nonlinear_fit(data=y,prior=prior,fcn=f)
+    #     fit.dump_p("test-lsqfit.p")
+    #     p = nonlinear_fit.load_parameters("test-lsqfit.p")
+    #     self.assert_gvclose(p[0],fit.p[0])
+    #     self.assert_gvclose(p[0],wavg([y[0],y[1],prior[0]]))
+    #     fit.dump_pmean("test-lsqfit.p")
+    #     pmean = fit.load_parameters("test-lsqfit.p")
+    #     self.assertAlmostEqual(pmean[0],fit.pmean[0])
+    #     os.remove("test-lsqfit.p")
 
     def test_partialerr1(self):
         """ fit.p.der """
         # verifies that derivatives in fit.p relate properly to inputs
         #
         # data
         y = gvar(2.,0.125)
@@ -1416,14 +1419,56 @@
             "fit function"
             return N * [p['a']]
         fit = nonlinear_fit(prior=prior, data=(None,y), fcn=fcn, extend=True)
         self.assertTrue('a' in fit.p)
         self.assertTrue(gv.equivalent(fit.p['sqrt(a)'] ** 2, fit.p['a']))
         self.assertEqual(fit.p['a'].fmt(), "0.010(13)")
 
+    def test_linear_dict(self):
+        def fcn(p, t=np.arange(0.,1.,0.2)):
+            c = p['c']
+            E = np.cumsum(p['dE'])
+            i = (c != 0)
+            return np.sum(
+                c[None, i] * gv.exp(-E[None, i] * t[:, None]), axis=1
+                )
+        prior = gv.gvar(dict(c=2 * ['1.00(1)'], dE= 2 * ['0.500(1)']))
+        data = gv.gvar([
+            '2.0008(10)', '1.72452(86)', '1.49030(75)',
+            '1.29009(65)', '1.12017(57)'
+            ])
+        fita = nonlinear_fit(prior=prior, data=data, fcn=fcn)
+        fitb = nonlinear_fit(prior=prior, data=data, fcn=fcn, linear=['c'])
+        self.assertAlmostEqual(fita.chi2, fitb.chi2)
+        self.assertTrue(gv.equivalent(fita.p, fitb.p, rtol=1e-1))
+        np.testing.assert_allclose(
+            gv.mean(fita.p.flat), gv.mean(fitb.p.flat), rtol=1e-5
+            )
+
+    def test_linear_array(self):
+        def fcn(p, t=np.arange(0.,1.,0.2)):
+            c = p[:2]
+            E = np.cumsum(p[2:])
+            i = (c != 0)
+            return np.sum(
+                c[None, i] * gv.exp(-E[None, i] * t[:, None]), axis=1
+                )
+        prior = gv.gvar(2 * ['1.00(1)'] + 2 * ['0.500(1)'])
+        data = gv.gvar([
+            '2.0008(10)', '1.72452(86)', '1.49030(75)',
+            '1.29009(65)', '1.12017(57)'
+            ])
+        fita = nonlinear_fit(prior=prior, data=data, fcn=fcn)
+        fitb = nonlinear_fit(prior=prior, data=data, fcn=fcn, linear=[0,1])
+        self.assertAlmostEqual(fita.chi2, fitb.chi2)
+        self.assertTrue(gv.equivalent(fita.p, fitb.p, rtol=1e-1))
+        np.testing.assert_allclose(
+            gv.mean(fita.p.flat), gv.mean(fitb.p.flat), rtol=1e-5
+            )
+
     def test_multifit_exceptions(self):
         """ multifit exceptions """
         y = gv.gvar(["1(1)", "2(1)"])
         prior = gv.gvar(dict(a="0(2)"))
         with self.assertRaises(ValueError):
             def f(p):
                 return [p['a']]*3
```

### Comparing `lsqfit-9.4/tests/makefile` & `lsqfit-9.5/tests/makefile`

 * *Files identical despite different names*

### Comparing `lsqfit-9.4/CHANGES.txt` & `lsqfit-9.5/CHANGES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+Version 9.5 2018-07-15
+======================
+- lsqfit.nonlinear_fit has a new keyword: linear. This can be used
+  to specify a list of fit variables that appear linearly in the  fit
+  function. These are removed from the fit using variable projection, thereby
+  reducing the number of fit parameters; they are  reintroduced after the fit.
+  This parameter is optional and currently somewhat experimental.
+
+- nonlinear_fit methods load_parameters and dump_p are deprecated; use
+  gvar.load and gvar.dump instead. Similarly dump_pmean is
+  deprecated.
+
+
 Version 9.4 2018-07-08
 ======================
 - p0=True generates a random p0 from the prior in nonlinear_fit. This
   can be useful for fits that are sensitive to the starting point.
 
 - Updated time measurements for Python3.
```

### Comparing `lsqfit-9.4/setup.py` & `lsqfit-9.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 This program is distributed in the hope that it will be useful,
 but WITHOUT ANY WARRANTY; without even the implied warranty of
 MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 GNU General Public License for more details.
 """
 
-LSQFIT_VERSION = '9.4'
+LSQFIT_VERSION = '9.5'
 
 from distutils.core import setup
 from distutils.extension import Extension
 from distutils.command.build_ext import build_ext as _build_ext
 from distutils.command.build_py import build_py as _build_py
 
 # compile from existing .c files if USE_CYTHON is False
```

### Comparing `lsqfit-9.4/examples/x-err.out` & `lsqfit-9.5/examples/x-err.out`

 * *Files identical despite different names*

### Comparing `lsqfit-9.4/examples/nist.out` & `lsqfit-9.5/examples/nist.out`

 * *Files identical despite different names*

### Comparing `lsqfit-9.4/examples/pendulum.pdf` & `lsqfit-9.5/examples/pendulum.pdf`

 * *Files identical despite different names*

### Comparing `lsqfit-9.4/examples/uncorrelated.py` & `lsqfit-9.5/examples/uncorrelated.py`

 * *Files identical despite different names*

### Comparing `lsqfit-9.4/examples/y-noerr.out` & `lsqfit-9.5/examples/y-noerr.out`

 * *Files identical despite different names*

### Comparing `lsqfit-9.4/examples/xxxx` & `lsqfit-9.5/examples/xxxx`

 * *Files identical despite different names*

### Comparing `lsqfit-9.4/examples/y-vs-x.out` & `lsqfit-9.5/examples/y-vs-x.out`

 * *Files identical despite different names*

### Comparing `lsqfit-9.4/examples/nist.py` & `lsqfit-9.5/examples/nist.py`

 * *Files identical despite different names*

### Comparing `lsqfit-9.4/examples/empbayes.py` & `lsqfit-9.5/examples/empbayes.py`

 * *Files identical despite different names*

### Comparing `lsqfit-9.4/examples/xxx.out` & `lsqfit-9.5/examples/xxx.out`

 * *Files identical despite different names*

### Comparing `lsqfit-9.4/examples/xxx` & `lsqfit-9.5/examples/xxx`

 * *Files identical despite different names*

### Comparing `lsqfit-9.4/examples/makefile` & `lsqfit-9.5/examples/makefile`

 * *Files identical despite different names*

### Comparing `lsqfit-9.4/examples/pendulum.out` & `lsqfit-9.5/examples/pendulum.out`

 * *Files identical despite different names*

### Comparing `lsqfit-9.4/examples/bayes.out` & `lsqfit-9.5/examples/bayes.out`

 * *Files 0% similar despite different names*

```diff
@@ -12,22 +12,22 @@
 
 
 Iterations:
 itn   integral        average         chi2/dof        Q
 -------------------------------------------------------
   1   0.997(25)       0.997(25)           0.00     1.00
   2   0.980(20)       0.989(16)           0.58     1.00
-  3   1.044(28)       1.007(14)           0.59     1.00
+  3   1.044(28)       1.007(14)           0.58     1.00
   4   0.979(21)       1.000(12)           0.58     1.00
-  5   1.016(21)       1.003(10)           0.62     1.00
+  5   1.016(21)       1.003(10)           0.63     1.00
   6   1.017(38)       1.006(11)           0.64     1.00
   7   0.984(22)       1.0025(97)          0.65     1.00
   8   1.023(31)       1.0051(94)          0.63     1.00
   9   1.002(21)       1.0048(86)          0.67     1.00
- 10   1.034(26)       1.0077(82)          0.66     1.00
+ 10   1.034(26)       1.0077(82)          0.67     1.00
 
 Integration Results:
     mean(p) = [0.15497(18) 3.0978(37) 1.4385(69) 0.6985(33)]
     cov(p) =
  [[0.0002174(47) 0.004215(96) 0.00747(17) 0.001262(81)]
  [0.004215(96) 0.0919(20) 0.1508(35) 0.0268(17)]
  [0.00747(17) 0.1508(35) 0.3077(75) 0.0257(27)]
```

### Comparing `lsqfit-9.4/examples/y-vs-x.py` & `lsqfit-9.5/examples/y-vs-x.py`

 * *Files identical despite different names*

### Comparing `lsqfit-9.4/examples/empbayes.out` & `lsqfit-9.5/examples/empbayes.out`

 * *Files identical despite different names*

### Comparing `lsqfit-9.4/examples/nist/roszman1.txt` & `lsqfit-9.5/examples/nist/roszman1.txt`

 * *Files identical despite different names*

### Comparing `lsqfit-9.4/examples/nist/thurber.txt` & `lsqfit-9.5/examples/nist/thurber.txt`

 * *Files identical despite different names*

### Comparing `lsqfit-9.4/examples/nist/bennett5.txt` & `lsqfit-9.5/examples/nist/bennett5.txt`

 * *Files identical despite different names*

### Comparing `lsqfit-9.4/examples/nist/misra1c.txt` & `lsqfit-9.5/examples/nist/misra1c.txt`

 * *Files identical despite different names*

### Comparing `lsqfit-9.4/examples/nist/enso.txt` & `lsqfit-9.5/examples/nist/enso.txt`

 * *Files identical despite different names*

### Comparing `lsqfit-9.4/examples/nist/nelson.txt` & `lsqfit-9.5/examples/nist/nelson.txt`

 * *Files identical despite different names*

### Comparing `lsqfit-9.4/examples/nist/lanczos3.txt` & `lsqfit-9.5/examples/nist/lanczos3.txt`

 * *Files identical despite different names*

### Comparing `lsqfit-9.4/examples/nist/lanczos2.txt` & `lsqfit-9.5/examples/nist/lanczos2.txt`

 * *Files identical despite different names*

### Comparing `lsqfit-9.4/examples/nist/misra1b.txt` & `lsqfit-9.5/examples/nist/misra1b.txt`

 * *Files identical despite different names*

### Comparing `lsqfit-9.4/examples/nist/1st_nist.py` & `lsqfit-9.5/examples/nist/1st_nist.py`

 * *Files identical despite different names*

### Comparing `lsqfit-9.4/examples/nist/rat42.txt` & `lsqfit-9.5/examples/nist/rat42.txt`

 * *Files identical despite different names*

### Comparing `lsqfit-9.4/examples/nist/lanczos1.txt` & `lsqfit-9.5/examples/nist/lanczos1.txt`

 * *Files identical despite different names*

### Comparing `lsqfit-9.4/examples/nist/rat43.txt` & `lsqfit-9.5/examples/nist/rat43.txt`

 * *Files identical despite different names*

### Comparing `lsqfit-9.4/examples/nist/misra1a.txt` & `lsqfit-9.5/examples/nist/misra1a.txt`

 * *Files identical despite different names*

### Comparing `lsqfit-9.4/examples/nist/misra1d.txt` & `lsqfit-9.5/examples/nist/misra1d.txt`

 * *Files identical despite different names*

### Comparing `lsqfit-9.4/examples/nist/boxbod.txt` & `lsqfit-9.5/examples/nist/boxbod.txt`

 * *Files identical despite different names*

### Comparing `lsqfit-9.4/examples/nist/mgh09.txt` & `lsqfit-9.5/examples/nist/mgh09.txt`

 * *Files identical despite different names*

### Comparing `lsqfit-9.4/examples/nist/mgh10.txt` & `lsqfit-9.5/examples/nist/mgh10.txt`

 * *Files identical despite different names*

### Comparing `lsqfit-9.4/examples/nist/make_script.py` & `lsqfit-9.5/examples/nist/make_script.py`

 * *Files identical despite different names*

### Comparing `lsqfit-9.4/examples/nist/mgh17.txt` & `lsqfit-9.5/examples/nist/mgh17.txt`

 * *Files identical despite different names*

### Comparing `lsqfit-9.4/examples/nist/hahn1.txt` & `lsqfit-9.5/examples/nist/hahn1.txt`

 * *Files identical despite different names*

### Comparing `lsqfit-9.4/examples/nist/gauss1.txt` & `lsqfit-9.5/examples/nist/gauss1.txt`

 * *Files identical despite different names*

### Comparing `lsqfit-9.4/examples/nist/eckerle4.txt` & `lsqfit-9.5/examples/nist/eckerle4.txt`

 * *Files identical despite different names*

### Comparing `lsqfit-9.4/examples/nist/gauss2.txt` & `lsqfit-9.5/examples/nist/gauss2.txt`

 * *Files identical despite different names*

### Comparing `lsqfit-9.4/examples/nist/kirby2.txt` & `lsqfit-9.5/examples/nist/kirby2.txt`

 * *Files identical despite different names*

### Comparing `lsqfit-9.4/examples/nist/gauss3.txt` & `lsqfit-9.5/examples/nist/gauss3.txt`

 * *Files identical despite different names*

### Comparing `lsqfit-9.4/examples/nist/2nd_nist.py` & `lsqfit-9.5/examples/nist/2nd_nist.py`

 * *Files identical despite different names*

### Comparing `lsqfit-9.4/examples/nist/chwirut2.txt` & `lsqfit-9.5/examples/nist/chwirut2.txt`

 * *Files identical despite different names*

### Comparing `lsqfit-9.4/examples/nist/danwood.txt` & `lsqfit-9.5/examples/nist/danwood.txt`

 * *Files identical despite different names*

### Comparing `lsqfit-9.4/examples/nist/chwirut1.txt` & `lsqfit-9.5/examples/nist/chwirut1.txt`

 * *Files identical despite different names*

### Comparing `lsqfit-9.4/examples/README` & `lsqfit-9.5/examples/README`

 * *Files identical despite different names*

### Comparing `lsqfit-9.4/examples/p-corr.py` & `lsqfit-9.5/examples/p-corr.py`

 * *Files identical despite different names*

### Comparing `lsqfit-9.4/examples/bayes.py` & `lsqfit-9.5/examples/bayes.py`

 * *Files identical despite different names*

### Comparing `lsqfit-9.4/examples/x-err.py` & `lsqfit-9.5/examples/x-err.py`

 * *Files identical despite different names*

### Comparing `lsqfit-9.4/examples/simple.out` & `lsqfit-9.5/examples/simple.out`

 * *Files identical despite different names*

### Comparing `lsqfit-9.4/examples/simple.py` & `lsqfit-9.5/examples/simple.py`

 * *Files identical despite different names*

### Comparing `lsqfit-9.4/examples/pendulum.py` & `lsqfit-9.5/examples/pendulum.py`

 * *Files identical despite different names*

### Comparing `lsqfit-9.4/examples/outputfile.p` & `lsqfit-9.5/examples/outputfile.p`

 * *Files identical despite different names*

### Comparing `lsqfit-9.4/examples/xxx.py` & `lsqfit-9.5/examples/xxx.py`

 * *Files identical despite different names*

### Comparing `lsqfit-9.4/examples/yyy.py` & `lsqfit-9.5/examples/yyy.py`

 * *Files identical despite different names*

### Comparing `lsqfit-9.4/examples/y-noerr.py` & `lsqfit-9.5/examples/y-noerr.py`

 * *Files identical despite different names*

### Comparing `lsqfit-9.4/doc/html/case-extrapolation.html` & `lsqfit-9.5/doc/html/case-extrapolation.html`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 <!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Transitional//EN"
   "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
 
 <html xmlns="http://www.w3.org/1999/xhtml">
   <head>
     <meta http-equiv="X-UA-Compatible" content="IE=Edge" />
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
-    <title>Case Study: Simple Extrapolation &#8212; lsqfit 9.4 documentation</title>
+    <title>Case Study: Simple Extrapolation &#8212; lsqfit 9.5 documentation</title>
     <link rel="stylesheet" href="_static/pyramid.css" type="text/css" />
     <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
     <script type="text/javascript" src="_static/documentation_options.js"></script>
     <script type="text/javascript" src="_static/jquery.js"></script>
     <script type="text/javascript" src="_static/underscore.js"></script>
     <script type="text/javascript" src="_static/doctools.js"></script>
     <link rel="index" title="Index" href="genindex.html" />
@@ -36,15 +36,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="case-pendulum.html" title="Case Study: Pendulum"
              accesskey="N">next</a> |</li>
         <li class="right" >
           <a href="testing.html" title="Non-Gaussian Behavior; Testing Fits"
              accesskey="P">previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">lsqfit 9.4 documentation</a> &#187;</li> 
+        <li class="nav-item nav-item-0"><a href="index.html">lsqfit 9.5 documentation</a> &#187;</li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
           <div class="body" role="main">
@@ -748,15 +748,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="case-pendulum.html" title="Case Study: Pendulum"
              >next</a> |</li>
         <li class="right" >
           <a href="testing.html" title="Non-Gaussian Behavior; Testing Fits"
              >previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">lsqfit 9.4 documentation</a> &#187;</li> 
+        <li class="nav-item nav-item-0"><a href="index.html">lsqfit 9.5 documentation</a> &#187;</li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
         &#169; Copyright 2009-2018, G. P. Lepage.
       Created using <a href="http://sphinx-doc.org/">Sphinx</a> 1.7.4.
     </div>
   </body>
```

#### html2text {}

```diff
@@ -9,15 +9,15 @@
 
 
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * lsqfit_9.4_documentation »
+    * lsqfit_9.5_documentation »
 ****** Case Study: Simple ExtrapolationÂ¶ ******
 In this case study, we examine a simple extrapolation problem. We show first
 how not to solve this problem. A better solution follows, together with a
 discussion of priors and Bayes factors. Finally a very simple, alternative
 solution, using marginalization, is described.
 ***** The ProblemÂ¶ *****
 Consider a problem where we have five pieces of uncorrelated data for a
@@ -603,9 +603,9 @@
 **** Quick search ****
 [q                   ] [Go]
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * lsqfit_9.4_documentation »
+    * lsqfit_9.5_documentation »
 © Copyright 2009-2018, G. P. Lepage. Created using Sphinx 1.7.4.
```

### Comparing `lsqfit-9.4/doc/html/index.html` & `lsqfit-9.5/doc/html/index.html`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 <!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Transitional//EN"
   "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
 
 <html xmlns="http://www.w3.org/1999/xhtml">
   <head>
     <meta http-equiv="X-UA-Compatible" content="IE=Edge" />
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
-    <title>lsqfit Documentation &#8212; lsqfit 9.4 documentation</title>
+    <title>lsqfit Documentation &#8212; lsqfit 9.5 documentation</title>
     <link rel="stylesheet" href="_static/pyramid.css" type="text/css" />
     <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
     <script type="text/javascript" src="_static/documentation_options.js"></script>
     <script type="text/javascript" src="_static/jquery.js"></script>
     <script type="text/javascript" src="_static/underscore.js"></script>
     <script type="text/javascript" src="_static/doctools.js"></script>
     <link rel="index" title="Index" href="genindex.html" />
@@ -32,15 +32,15 @@
              accesskey="I">index</a></li>
         <li class="right" >
           <a href="py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
         <li class="right" >
           <a href="overview.html" title="Overview and Tutorial"
              accesskey="N">next</a> |</li>
-        <li class="nav-item nav-item-0"><a href="#">lsqfit 9.4 documentation</a> &#187;</li> 
+        <li class="nav-item nav-item-0"><a href="#">lsqfit 9.5 documentation</a> &#187;</li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
           <div class="body" role="main">
@@ -170,15 +170,15 @@
              >index</a></li>
         <li class="right" >
           <a href="py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
         <li class="right" >
           <a href="overview.html" title="Overview and Tutorial"
              >next</a> |</li>
-        <li class="nav-item nav-item-0"><a href="#">lsqfit 9.4 documentation</a> &#187;</li> 
+        <li class="nav-item nav-item-0"><a href="#">lsqfit 9.5 documentation</a> &#187;</li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
         &#169; Copyright 2009-2018, G. P. Lepage.
       Created using <a href="http://sphinx-doc.org/">Sphinx</a> 1.7.4.
     </div>
   </body>
```

#### html2text {}

```diff
@@ -7,15 +7,15 @@
 
 
 
 **** Navigation ****
     * index
     * modules |
     * next |
-    * lsqfit_9.4_documentation »
+    * lsqfit_9.5_documentation »
 ****** lsqfit DocumentationÂ¶ ******
 Contents:
     * Overview_and_Tutorial
           o Introduction
           o Gaussian_Random_Variables_and_Error_Propagation
           o Basic_Fits
           o Chained_Fits;_Large_Data_Sets
@@ -73,9 +73,9 @@
     * Show_Source
 **** Quick search ****
 [q                   ] [Go]
 **** Navigation ****
     * index
     * modules |
     * next |
-    * lsqfit_9.4_documentation »
+    * lsqfit_9.5_documentation »
 © Copyright 2009-2018, G. P. Lepage. Created using Sphinx 1.7.4.
```

### Comparing `lsqfit-9.4/doc/html/searchindex.js` & `lsqfit-9.5/doc/html/searchindex.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -35,20 +35,17 @@
         "lsqfit.nonlinear_fit": {
             Q: [5, 5, 1, ""],
             bootstrapped_fit_iter: [5, 3, 1, ""],
             check_roundoff: [5, 3, 1, ""],
             chi2: [5, 5, 1, ""],
             cov: [5, 5, 1, ""],
             dof: [5, 5, 1, ""],
-            dump_p: [5, 3, 1, ""],
-            dump_pmean: [5, 3, 1, ""],
             error: [5, 5, 1, ""],
             fitter_results: [5, 5, 1, ""],
             format: [5, 3, 1, ""],
-            load_parameters: [5, 4, 1, ""],
             logGBF: [5, 5, 1, ""],
             nblocks: [5, 5, 1, ""],
             p0: [5, 5, 1, ""],
             p: [5, 5, 1, ""],
             palt: [5, 5, 1, ""],
             pmean: [5, 5, 1, ""],
             prior: [5, 5, 1, ""],
@@ -585,16 +582,14 @@
         drop: [0, 1, 6],
         dt2: 2,
         dtheta: 2,
         dtheta_dt: 2,
         dtype: 6,
         due: [0, 2, 6],
         dump: [5, 6],
-        dump_p: 5,
-        dump_pmean: 5,
         dynam: 4,
         each: [0, 1, 2, 3, 5, 6, 8],
         earli: 6,
         earlier: [3, 5, 6],
         easi: 6,
         easier: 6,
         easili: [0, 1, 6],
@@ -654,16 +649,16 @@
         exclud: 6,
         exhibit: 2,
         exist: 6,
         exp: [0, 1, 5, 6, 8],
         expans: [0, 8],
         expect: [0, 1, 5, 6, 8],
         expens: 6,
-        experi: 6,
-        experiment: [2, 6],
+        experi: [5, 6],
+        experiment: [2, 5, 6],
         explain: 6,
         explan: [1, 5],
         explicitli: [5, 6],
         exploit: 6,
         explor: [5, 6],
         expon: 6,
         exponenti: [0, 5, 6],
@@ -690,18 +685,19 @@
         far: 6,
         fashion: [5, 6],
         fast: [5, 6],
         faster: [3, 4, 5],
         favor: 6,
         fcn: [0, 1, 2, 5, 6, 8],
         feasibl: 5,
-        featur: 6,
+        featur: [5, 6],
         fed: 5,
         feel: 6,
         few: [5, 6],
+        fewer: 5,
         field: 5,
         figur: [2, 6],
         file: [5, 6],
         filenam: 5,
         fill: 5,
         fill_between: 1,
         find: [3, 5, 6, 7],
@@ -865,15 +861,15 @@
         intact: 6,
         integ: 5,
         integr: [2, 4, 6],
         integrand: 8,
         intellig: 6,
         intercept: [1, 5],
         interest: 6,
-        interfac: 6,
+        interfac: [5, 6],
         intermedi: [3, 7],
         intern: [3, 7],
         interv: [1, 2, 6],
         intrins: 8,
         introduc: [0, 1, 6, 8],
         introduct: 4,
         invari: 3,
@@ -931,35 +927,34 @@
         lie: 6,
         like: [0, 5, 6, 8],
         likelihood: 6,
         limit: [5, 6],
         linalg: 6,
         line: [0, 1, 5, 6, 8],
         linear: [0, 1, 3, 5, 6],
+        linearli: 5,
         link: 5,
         linspac: 1,
         list: [0, 1, 5, 6, 8],
         littl: 6,
         lmaccel: 3,
         lmder: [3, 6],
         lmniel: 3,
         lmsder: [3, 6],
         load: [5, 6],
-        load_p: 5,
-        load_paramet: 5,
         locat: [3, 7],
         lock: 6,
         log: [5, 6],
         logarithm: [0, 1, 5, 6],
         logbf: 1,
         loggbf: [0, 1, 2, 3, 5, 6, 7, 8],
         loglog: 5,
         logp: 5,
         logpdf: 5,
-        longer: [6, 8],
+        longer: [5, 6, 8],
         look: [0, 5, 6, 8],
         loop: 6,
         lose: 5,
         loss: [5, 6, 7],
         lot: [5, 6],
         low: [6, 8],
         lower: [1, 6],
@@ -1231,15 +1226,15 @@
         process_data: 5,
         process_dataset: 5,
         processor: 8,
         prod: 1,
         produc: [6, 8],
         product: 1,
         program: [5, 6],
-        project: 6,
+        project: [5, 6],
         propag: [2, 4],
         proper: 5,
         proport: [5, 6, 8],
         protocol: 8,
         prove: 6,
         provid: [0, 3, 5, 6, 7, 8],
         psdev: 5,
@@ -1273,19 +1268,21 @@
         readi: 6,
         real: 8,
         realist: 6,
         realli: [0, 6],
         reason: [0, 1, 6],
         recent: [3, 7],
         recip: 6,
+        reconstruct: 5,
         recov: [5, 6],
         red: [1, 2],
         redefin: 6,
         redon: 5,
         reduc: [5, 6],
+        reexpress: 5,
         refer: 5,
         reflect: 7,
         region: [1, 3, 5, 7],
         regul: 6,
         regular: [0, 2],
         reject: 3,
         rel: [1, 3, 5, 6, 7, 8],
@@ -1319,15 +1316,15 @@
         retain: 5,
         revisit: 8,
         rewrit: 6,
         rid: 6,
         ridicul: 6,
         right: [6, 8],
         rightmost: 6,
-        robust: [3, 6],
+        robust: [3, 5, 6],
         role: 1,
         root: [5, 6],
         roughli: [0, 8],
         roundoff: [4, 5],
         routin: [4, 5, 6],
         row: 6,
         rtol: 5,
@@ -1376,15 +1373,15 @@
         shift: [3, 6, 8],
         should: [0, 5, 6, 8],
         show: [0, 1, 2, 5, 6, 8],
         show_plot: 5,
         shown: [5, 6],
         side: 5,
         sigma: [0, 1, 6],
-        sign: 6,
+        sign: [5, 6],
         signal: 0,
         signific: [5, 6],
         significantli: [5, 6, 8],
         similar: [0, 1, 5, 6, 8],
         simpl: [4, 5, 6, 8],
         simpler: 5,
         simplex: 3,
@@ -1637,15 +1634,15 @@
         weight: [0, 1, 5, 6, 8],
         well: [0, 5, 6, 8],
         were: [0, 1, 5, 6, 8],
         wgtd: 5,
         what: [1, 5, 6],
         when: [0, 3, 5, 6, 7, 8],
         where: [0, 1, 2, 3, 5, 6, 7, 8],
-        whether: [0, 6],
+        whether: [0, 5, 6],
         which: [0, 1, 2, 3, 5, 6, 8],
         whose: [2, 3, 5, 6, 7, 8],
         why: [1, 6],
         wide: [0, 6],
         width: [0, 6],
         window: 5,
         wish: 6,
```

### Comparing `lsqfit-9.4/doc/html/scipy.html` & `lsqfit-9.5/doc/html/scipy.html`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 <!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Transitional//EN"
   "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
 
 <html xmlns="http://www.w3.org/1999/xhtml">
   <head>
     <meta http-equiv="X-UA-Compatible" content="IE=Edge" />
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
-    <title>scipy Routines &#8212; lsqfit 9.4 documentation</title>
+    <title>scipy Routines &#8212; lsqfit 9.5 documentation</title>
     <link rel="stylesheet" href="_static/pyramid.css" type="text/css" />
     <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
     <script type="text/javascript" src="_static/documentation_options.js"></script>
     <script type="text/javascript" src="_static/jquery.js"></script>
     <script type="text/javascript" src="_static/underscore.js"></script>
     <script type="text/javascript" src="_static/doctools.js"></script>
     <link rel="index" title="Index" href="genindex.html" />
@@ -32,15 +32,15 @@
              accesskey="I">index</a></li>
         <li class="right" >
           <a href="py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
         <li class="right" >
           <a href="gsl.html" title="GSL Routines"
              accesskey="P">previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">lsqfit 9.4 documentation</a> &#187;</li> 
+        <li class="nav-item nav-item-0"><a href="index.html">lsqfit 9.5 documentation</a> &#187;</li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
           <div class="body" role="main">
@@ -298,15 +298,15 @@
              >index</a></li>
         <li class="right" >
           <a href="py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
         <li class="right" >
           <a href="gsl.html" title="GSL Routines"
              >previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">lsqfit 9.4 documentation</a> &#187;</li> 
+        <li class="nav-item nav-item-0"><a href="index.html">lsqfit 9.5 documentation</a> &#187;</li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
         &#169; Copyright 2009-2018, G. P. Lepage.
       Created using <a href="http://sphinx-doc.org/">Sphinx</a> 1.7.4.
     </div>
   </body>
```

#### html2text {}

```diff
@@ -7,15 +7,15 @@
 
 
 
 **** Navigation ****
     * index
     * modules |
     * previous |
-    * lsqfit_9.4_documentation »
+    * lsqfit_9.5_documentation »
 ****** scipy RoutinesÂ¶ ******
 ***** FitterÂ¶ *****
 lsqfit uses routines from the open-source scipy Python module provided it is
 installed. These routines are used in place of GSL routines if the latter are
 not installed. There is one fitter available for use by lsqfit.nonlinear_fit.
   classlsqfit.scipy_least_squares(x0, n, f, tol=(1e-08, 1e-08, 1e-08),
   maxit=1000, **extra_args)Â¶
@@ -125,9 +125,9 @@
     * Show_Source
 **** Quick search ****
 [q                   ] [Go]
 **** Navigation ****
     * index
     * modules |
     * previous |
-    * lsqfit_9.4_documentation »
+    * lsqfit_9.5_documentation »
 © Copyright 2009-2018, G. P. Lepage. Created using Sphinx 1.7.4.
```

### Comparing `lsqfit-9.4/doc/html/_sources/case-pendulum.rst.txt` & `lsqfit-9.5/doc/html/_sources/case-pendulum.rst.txt`

 * *Files identical despite different names*

### Comparing `lsqfit-9.4/doc/html/_sources/gsl.rst.txt` & `lsqfit-9.5/doc/html/_sources/gsl.rst.txt`

 * *Files identical despite different names*

### Comparing `lsqfit-9.4/doc/html/_sources/case-extrapolation.rst.txt` & `lsqfit-9.5/doc/html/_sources/case-extrapolation.rst.txt`

 * *Files identical despite different names*

### Comparing `lsqfit-9.4/doc/html/_sources/testing.rst.txt` & `lsqfit-9.5/doc/html/_sources/testing.rst.txt`

 * *Files identical despite different names*

### Comparing `lsqfit-9.4/doc/html/_sources/lsqfit.rst.txt` & `lsqfit-9.5/doc/html/_sources/lsqfit.rst.txt`

 * *Files 2% similar despite different names*

```diff
@@ -139,28 +139,22 @@
 
 .. autoclass:: lsqfit.nonlinear_fit(data, fcn, prior=None, p0=None, extend=False, svdcut=1e-12, debug=False, tol=1e-8, maxit=1000, fitter='gsl_multifit', **fitterargs)
 
    Additional methods are provided for printing out detailed information
    about the fit, testing fits with simulated data,
    doing bootstrap analyses of the fit errors,
    dumping (for later use) and loading parameter values, and checking for roundoff
-   errors in the final error estimates:
+   errors in the final error  estimates:
 
    .. automethod:: format(maxline=0, pstyle='v')
 
    .. automethod:: simulated_fit_iter(n=None, pexact=None, **kargs)
 
    .. automethod:: bootstrapped_fit_iter(n=None, datalist=None)
 
-   .. automethod:: dump_p(filename)
-
-   .. automethod:: dump_pmean(filename)
-
-   .. automethod:: nonlinear_fit.load_parameters(filename)
-
    .. automethod:: check_roundoff(rtol=0.25,atol=1e-6)
 
    .. automethod:: set(clear=False, **defaults)
 
 Functions
 ---------
 .. autofunction:: lsqfit.empbayes_fit
```

### Comparing `lsqfit-9.4/doc/html/_sources/index.rst.txt` & `lsqfit-9.5/doc/html/_sources/index.rst.txt`

 * *Files identical despite different names*

### Comparing `lsqfit-9.4/doc/html/_sources/case-outliers.rst.txt` & `lsqfit-9.5/doc/html/_sources/case-outliers.rst.txt`

 * *Files identical despite different names*

### Comparing `lsqfit-9.4/doc/html/_sources/overview.rst.txt` & `lsqfit-9.5/doc/html/_sources/overview.rst.txt`

 * *Files identical despite different names*

### Comparing `lsqfit-9.4/doc/html/_sources/scipy.rst.txt` & `lsqfit-9.5/doc/html/_sources/scipy.rst.txt`

 * *Files identical despite different names*

### Comparing `lsqfit-9.4/doc/html/py-modindex.html` & `lsqfit-9.5/doc/html/py-modindex.html`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 <!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Transitional//EN"
   "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
 
 <html xmlns="http://www.w3.org/1999/xhtml">
   <head>
     <meta http-equiv="X-UA-Compatible" content="IE=Edge" />
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
-    <title>Python Module Index &#8212; lsqfit 9.4 documentation</title>
+    <title>Python Module Index &#8212; lsqfit 9.5 documentation</title>
     <link rel="stylesheet" href="_static/pyramid.css" type="text/css" />
     <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
     <script type="text/javascript" src="_static/documentation_options.js"></script>
     <script type="text/javascript" src="_static/jquery.js"></script>
     <script type="text/javascript" src="_static/underscore.js"></script>
     <script type="text/javascript" src="_static/doctools.js"></script>
     <link rel="index" title="Index" href="genindex.html" />
@@ -35,15 +35,15 @@
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="genindex.html" title="General Index"
              accesskey="I">index</a></li>
         <li class="right" >
           <a href="#" title="Python Module Index"
              >modules</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">lsqfit 9.4 documentation</a> &#187;</li> 
+        <li class="nav-item nav-item-0"><a href="index.html">lsqfit 9.5 documentation</a> &#187;</li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
           <div class="body" role="main">
@@ -93,15 +93,15 @@
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="genindex.html" title="General Index"
              >index</a></li>
         <li class="right" >
           <a href="#" title="Python Module Index"
              >modules</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">lsqfit 9.4 documentation</a> &#187;</li> 
+        <li class="nav-item nav-item-0"><a href="index.html">lsqfit 9.5 documentation</a> &#187;</li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
         &#169; Copyright 2009-2018, G. P. Lepage.
       Created using <a href="http://sphinx-doc.org/">Sphinx</a> 1.7.4.
     </div>
   </body>
```

#### html2text {}

```diff
@@ -5,20 +5,20 @@
 
 
 
 
 **** Navigation ****
     * index
     * modules |
-    * lsqfit_9.4_documentation »
+    * lsqfit_9.5_documentation »
 ****** Python Module Index ******
 l
   
  l
  lsqfit Nonlinear least squares fitting.
 **** Quick search ****
 [q                   ] [Go]
 **** Navigation ****
     * index
     * modules |
-    * lsqfit_9.4_documentation »
+    * lsqfit_9.5_documentation »
 © Copyright 2009-2018, G. P. Lepage. Created using Sphinx 1.7.4.
```

### Comparing `lsqfit-9.4/doc/html/gsl.html` & `lsqfit-9.5/doc/html/gsl.html`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 <!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Transitional//EN"
   "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
 
 <html xmlns="http://www.w3.org/1999/xhtml">
   <head>
     <meta http-equiv="X-UA-Compatible" content="IE=Edge" />
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
-    <title>GSL Routines &#8212; lsqfit 9.4 documentation</title>
+    <title>GSL Routines &#8212; lsqfit 9.5 documentation</title>
     <link rel="stylesheet" href="_static/pyramid.css" type="text/css" />
     <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
     <script type="text/javascript" src="_static/documentation_options.js"></script>
     <script type="text/javascript" src="_static/jquery.js"></script>
     <script type="text/javascript" src="_static/underscore.js"></script>
     <script type="text/javascript" src="_static/doctools.js"></script>
     <link rel="index" title="Index" href="genindex.html" />
@@ -36,15 +36,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="scipy.html" title="scipy Routines"
              accesskey="N">next</a> |</li>
         <li class="right" >
           <a href="lsqfit.html" title="lsqfit - Nonlinear Least Squares Fitting"
              accesskey="P">previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">lsqfit 9.4 documentation</a> &#187;</li> 
+        <li class="nav-item nav-item-0"><a href="index.html">lsqfit 9.5 documentation</a> &#187;</li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
           <div class="body" role="main">
@@ -487,15 +487,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="scipy.html" title="scipy Routines"
              >next</a> |</li>
         <li class="right" >
           <a href="lsqfit.html" title="lsqfit - Nonlinear Least Squares Fitting"
              >previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">lsqfit 9.4 documentation</a> &#187;</li> 
+        <li class="nav-item nav-item-0"><a href="index.html">lsqfit 9.5 documentation</a> &#187;</li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
         &#169; Copyright 2009-2018, G. P. Lepage.
       Created using <a href="http://sphinx-doc.org/">Sphinx</a> 1.7.4.
     </div>
   </body>
```

#### html2text {}

```diff
@@ -9,15 +9,15 @@
 
 
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * lsqfit_9.4_documentation »
+    * lsqfit_9.5_documentation »
 ****** GSL RoutinesÂ¶ ******
 ***** FittersÂ¶ *****
 lsqfit uses routines from the GSL C-library provided it is installed; GSL is
 the open-source Gnu Scientific Library. There are two fitters that are
 available for use by lsqfit.nonlinear_fit.
   classlsqfit.gsl_multifit(n, f, tol=(1e-5, 0.0, 0.0), maxit=1000, alg='lm',
   solver='qr', scaler='more', factor_up=3.0, factor_down=2.0, avmax=0.75)Â¶
@@ -287,9 +287,9 @@
 **** Quick search ****
 [q                   ] [Go]
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * lsqfit_9.4_documentation »
+    * lsqfit_9.5_documentation »
 © Copyright 2009-2018, G. P. Lepage. Created using Sphinx 1.7.4.
```

### Comparing `lsqfit-9.4/doc/html/_static/jquery-3.2.1.js` & `lsqfit-9.5/doc/html/_static/jquery-3.2.1.js`

 * *Files identical despite different names*

### Comparing `lsqfit-9.4/doc/html/_static/underscore.js` & `lsqfit-9.5/doc/html/_static/underscore.js`

 * *Files identical despite different names*

### Comparing `lsqfit-9.4/doc/html/_static/ajax-loader.gif` & `lsqfit-9.5/doc/html/_static/ajax-loader.gif`

 * *Files identical despite different names*

### Comparing `lsqfit-9.4/doc/html/_static/dialog-warning.png` & `lsqfit-9.5/doc/html/_static/dialog-warning.png`

 * *Files identical despite different names*

### Comparing `lsqfit-9.4/doc/html/_static/searchtools.js` & `lsqfit-9.5/doc/html/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `lsqfit-9.4/doc/html/_static/underscore-1.3.1.js` & `lsqfit-9.5/doc/html/_static/underscore-1.3.1.js`

 * *Files identical despite different names*

### Comparing `lsqfit-9.4/doc/html/_static/ie6.css` & `lsqfit-9.5/doc/html/_static/ie6.css`

 * *Files identical despite different names*

### Comparing `lsqfit-9.4/doc/html/_static/dialog-todo.png` & `lsqfit-9.5/doc/html/_static/dialog-todo.png`

 * *Files identical despite different names*

### Comparing `lsqfit-9.4/doc/html/_static/epub.css` & `lsqfit-9.5/doc/html/_static/epub.css`

 * *Files identical despite different names*

### Comparing `lsqfit-9.4/doc/html/_static/pyramid.css` & `lsqfit-9.5/doc/html/_static/pyramid.css`

 * *Files identical despite different names*

### Comparing `lsqfit-9.4/doc/html/_static/comment.png` & `lsqfit-9.5/doc/html/_static/comment.png`

 * *Files identical despite different names*

### Comparing `lsqfit-9.4/doc/html/_static/basic.css` & `lsqfit-9.5/doc/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `lsqfit-9.4/doc/html/_static/dialog-seealso.png` & `lsqfit-9.5/doc/html/_static/dialog-seealso.png`

 * *Files identical despite different names*

### Comparing `lsqfit-9.4/doc/html/_static/dialog-topic.png` & `lsqfit-9.5/doc/html/_static/dialog-topic.png`

 * *Files identical despite different names*

### Comparing `lsqfit-9.4/doc/html/_static/pygments.css` & `lsqfit-9.5/doc/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `lsqfit-9.4/doc/html/_static/comment-close.png` & `lsqfit-9.5/doc/html/_static/comment-close.png`

 * *Files identical despite different names*

### Comparing `lsqfit-9.4/doc/html/_static/dialog-note.png` & `lsqfit-9.5/doc/html/_static/dialog-note.png`

 * *Files identical despite different names*

### Comparing `lsqfit-9.4/doc/html/_static/doctools.js` & `lsqfit-9.5/doc/html/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `lsqfit-9.4/doc/html/_static/comment-bright.png` & `lsqfit-9.5/doc/html/_static/comment-bright.png`

 * *Files identical despite different names*

### Comparing `lsqfit-9.4/doc/html/_static/websupport.js` & `lsqfit-9.5/doc/html/_static/websupport.js`

 * *Files identical despite different names*

### Comparing `lsqfit-9.4/doc/html/_static/jquery.js` & `lsqfit-9.5/doc/html/_static/jquery.js`

 * *Files identical despite different names*

### Comparing `lsqfit-9.4/doc/html/overview.html` & `lsqfit-9.5/doc/html/overview.html`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 <!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Transitional//EN"
   "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
 
 <html xmlns="http://www.w3.org/1999/xhtml">
   <head>
     <meta http-equiv="X-UA-Compatible" content="IE=Edge" />
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
-    <title>Overview and Tutorial &#8212; lsqfit 9.4 documentation</title>
+    <title>Overview and Tutorial &#8212; lsqfit 9.5 documentation</title>
     <link rel="stylesheet" href="_static/pyramid.css" type="text/css" />
     <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
     <script type="text/javascript" src="_static/documentation_options.js"></script>
     <script type="text/javascript" src="_static/jquery.js"></script>
     <script type="text/javascript" src="_static/underscore.js"></script>
     <script type="text/javascript" src="_static/doctools.js"></script>
     <link rel="index" title="Index" href="genindex.html" />
@@ -36,15 +36,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="testing.html" title="Non-Gaussian Behavior; Testing Fits"
              accesskey="N">next</a> |</li>
         <li class="right" >
           <a href="index.html" title="lsqfit Documentation"
              accesskey="P">previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">lsqfit 9.4 documentation</a> &#187;</li> 
+        <li class="nav-item nav-item-0"><a href="index.html">lsqfit 9.5 documentation</a> &#187;</li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
           <div class="body" role="main">
@@ -2695,15 +2695,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="testing.html" title="Non-Gaussian Behavior; Testing Fits"
              >next</a> |</li>
         <li class="right" >
           <a href="index.html" title="lsqfit Documentation"
              >previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">lsqfit 9.4 documentation</a> &#187;</li> 
+        <li class="nav-item nav-item-0"><a href="index.html">lsqfit 9.5 documentation</a> &#187;</li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
         &#169; Copyright 2009-2018, G. P. Lepage.
       Created using <a href="http://sphinx-doc.org/">Sphinx</a> 1.7.4.
     </div>
   </body>
```

#### html2text {}

```diff
@@ -9,15 +9,15 @@
 
 
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * lsqfit_9.4_documentation »
+    * lsqfit_9.5_documentation »
 ****** Overview and TutorialÂ¶ ******
 ***** IntroductionÂ¶ *****
 The lsqfit module is designed to facilitate least-squares fitting of noisy data
 by multi-dimensional, nonlinear functions of arbitrarily many parameters, each
 with a (Bayesian) prior. lsqfit makes heavy use of another module, gvar
 (distributed separately), which provides tools that simplify the analysis of
 error propagation, and also the creation of complicated multi-dimensional
@@ -2269,9 +2269,9 @@
 **** Quick search ****
 [q                   ] [Go]
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * lsqfit_9.4_documentation »
+    * lsqfit_9.5_documentation »
 © Copyright 2009-2018, G. P. Lepage. Created using Sphinx 1.7.4.
```

### Comparing `lsqfit-9.4/doc/html/_images/case-pendulum.png` & `lsqfit-9.5/doc/html/_images/case-pendulum.png`

 * *Files identical despite different names*

### Comparing `lsqfit-9.4/doc/html/_images/eg-appendix1d.png` & `lsqfit-9.5/doc/html/_images/eg-appendix1d.png`

 * *Files identical despite different names*

### Comparing `lsqfit-9.4/doc/html/_images/case-outliers1.png` & `lsqfit-9.5/doc/html/_images/case-outliers1.png`

 * *Files identical despite different names*

### Comparing `lsqfit-9.4/doc/html/_images/eg-appendix1a.png` & `lsqfit-9.5/doc/html/_images/eg-appendix1a.png`

 * *Files identical despite different names*

### Comparing `lsqfit-9.4/doc/html/_images/case-outliers2.png` & `lsqfit-9.5/doc/html/_images/case-outliers2.png`

 * *Files identical despite different names*

### Comparing `lsqfit-9.4/doc/html/_images/eg-appendix1b.png` & `lsqfit-9.5/doc/html/_images/eg-appendix1b.png`

 * *Files identical despite different names*

### Comparing `lsqfit-9.4/doc/html/_images/eg-appendix1c.png` & `lsqfit-9.5/doc/html/_images/eg-appendix1c.png`

 * *Files identical despite different names*

### Comparing `lsqfit-9.4/doc/html/_images/eg3d.png` & `lsqfit-9.5/doc/html/_images/eg3d.png`

 * *Files identical despite different names*

### Comparing `lsqfit-9.4/doc/html/_images/eg3e.png` & `lsqfit-9.5/doc/html/_images/eg3e.png`

 * *Files identical despite different names*

### Comparing `lsqfit-9.4/doc/html/_images/eg3.png` & `lsqfit-9.5/doc/html/_images/eg3.png`

 * *Files identical despite different names*

### Comparing `lsqfit-9.4/doc/html/_images/eg2.png` & `lsqfit-9.5/doc/html/_images/eg2.png`

 * *Files identical despite different names*

### Comparing `lsqfit-9.4/doc/html/_images/eg1.png` & `lsqfit-9.5/doc/html/_images/eg1.png`

 * *Files identical despite different names*

### Comparing `lsqfit-9.4/doc/html/_images/eg5.png` & `lsqfit-9.5/doc/html/_images/eg5.png`

 * *Files identical despite different names*

### Comparing `lsqfit-9.4/doc/html/_images/eg6.png` & `lsqfit-9.5/doc/html/_images/eg6.png`

 * *Files identical despite different names*

### Comparing `lsqfit-9.4/doc/html/case-outliers.html` & `lsqfit-9.5/doc/html/case-outliers.html`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 <!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Transitional//EN"
   "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
 
 <html xmlns="http://www.w3.org/1999/xhtml">
   <head>
     <meta http-equiv="X-UA-Compatible" content="IE=Edge" />
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
-    <title>Case Study: Outliers and Bayesian Integrals &#8212; lsqfit 9.4 documentation</title>
+    <title>Case Study: Outliers and Bayesian Integrals &#8212; lsqfit 9.5 documentation</title>
     <link rel="stylesheet" href="_static/pyramid.css" type="text/css" />
     <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
     <script type="text/javascript" src="_static/documentation_options.js"></script>
     <script type="text/javascript" src="_static/jquery.js"></script>
     <script type="text/javascript" src="_static/underscore.js"></script>
     <script type="text/javascript" src="_static/doctools.js"></script>
     <link rel="index" title="Index" href="genindex.html" />
@@ -36,15 +36,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="lsqfit.html" title="lsqfit - Nonlinear Least Squares Fitting"
              accesskey="N">next</a> |</li>
         <li class="right" >
           <a href="case-pendulum.html" title="Case Study: Pendulum"
              accesskey="P">previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">lsqfit 9.4 documentation</a> &#187;</li> 
+        <li class="nav-item nav-item-0"><a href="index.html">lsqfit 9.5 documentation</a> &#187;</li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
           <div class="body" role="main">
@@ -455,15 +455,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="lsqfit.html" title="lsqfit - Nonlinear Least Squares Fitting"
              >next</a> |</li>
         <li class="right" >
           <a href="case-pendulum.html" title="Case Study: Pendulum"
              >previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">lsqfit 9.4 documentation</a> &#187;</li> 
+        <li class="nav-item nav-item-0"><a href="index.html">lsqfit 9.5 documentation</a> &#187;</li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
         &#169; Copyright 2009-2018, G. P. Lepage.
       Created using <a href="http://sphinx-doc.org/">Sphinx</a> 1.7.4.
     </div>
   </body>
```

#### html2text {}

```diff
@@ -9,15 +9,15 @@
 
 
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * lsqfit_9.4_documentation »
+    * lsqfit_9.5_documentation »
 ****** Case Study: Outliers and Bayesian IntegralsÂ¶ ******
 In this case study, we analyze a fit with outliers in the data that distort the
 least-squares solution. We show one approach to dealing with the outliers that
 requires using Bayesian integrals in place of least-squares fitting, to fit the
 data while also modeling the outliers.
 This case study is adapted from an example by Jake Vanderplas on his Python
 blog.
@@ -349,9 +349,9 @@
 **** Quick search ****
 [q                   ] [Go]
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * lsqfit_9.4_documentation »
+    * lsqfit_9.5_documentation »
 © Copyright 2009-2018, G. P. Lepage. Created using Sphinx 1.7.4.
```

### Comparing `lsqfit-9.4/doc/html/case-pendulum.html` & `lsqfit-9.5/doc/html/case-pendulum.html`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 <!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Transitional//EN"
   "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
 
 <html xmlns="http://www.w3.org/1999/xhtml">
   <head>
     <meta http-equiv="X-UA-Compatible" content="IE=Edge" />
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
-    <title>Case Study: Pendulum &#8212; lsqfit 9.4 documentation</title>
+    <title>Case Study: Pendulum &#8212; lsqfit 9.5 documentation</title>
     <link rel="stylesheet" href="_static/pyramid.css" type="text/css" />
     <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
     <script type="text/javascript" src="_static/documentation_options.js"></script>
     <script type="text/javascript" src="_static/jquery.js"></script>
     <script type="text/javascript" src="_static/underscore.js"></script>
     <script type="text/javascript" src="_static/doctools.js"></script>
     <link rel="index" title="Index" href="genindex.html" />
@@ -36,15 +36,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="case-outliers.html" title="Case Study: Outliers and Bayesian Integrals"
              accesskey="N">next</a> |</li>
         <li class="right" >
           <a href="case-extrapolation.html" title="Case Study: Simple Extrapolation"
              accesskey="P">previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">lsqfit 9.4 documentation</a> &#187;</li> 
+        <li class="nav-item nav-item-0"><a href="index.html">lsqfit 9.5 documentation</a> &#187;</li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
           <div class="body" role="main">
@@ -286,15 +286,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="case-outliers.html" title="Case Study: Outliers and Bayesian Integrals"
              >next</a> |</li>
         <li class="right" >
           <a href="case-extrapolation.html" title="Case Study: Simple Extrapolation"
              >previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">lsqfit 9.4 documentation</a> &#187;</li> 
+        <li class="nav-item nav-item-0"><a href="index.html">lsqfit 9.5 documentation</a> &#187;</li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
         &#169; Copyright 2009-2018, G. P. Lepage.
       Created using <a href="http://sphinx-doc.org/">Sphinx</a> 1.7.4.
     </div>
   </body>
```

#### html2text {}

```diff
@@ -9,15 +9,15 @@
 
 
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * lsqfit_9.4_documentation »
+    * lsqfit_9.5_documentation »
 ****** Case Study: PendulumÂ¶ ******
 This case study shows how to fit a differential equation, using gvar.ode, and
 how to deal with uncertainty in the independent variable of a fit (that is, the
 x in a y versus x fit).
 ***** The ProblemÂ¶ *****
 A pendulum is released at time 0 from angle 1.571(50) (radians). Itâs angular
 position is measured at intervals of approximately a tenth of second:
@@ -184,9 +184,9 @@
 **** Quick search ****
 [q                   ] [Go]
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * lsqfit_9.4_documentation »
+    * lsqfit_9.5_documentation »
 © Copyright 2009-2018, G. P. Lepage. Created using Sphinx 1.7.4.
```

### Comparing `lsqfit-9.4/doc/html/genindex.html` & `lsqfit-9.5/doc/html/genindex.html`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 <!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Transitional//EN"
   "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
 
 <html xmlns="http://www.w3.org/1999/xhtml">
   <head>
     <meta http-equiv="X-UA-Compatible" content="IE=Edge" />
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
-    <title>Index &#8212; lsqfit 9.4 documentation</title>
+    <title>Index &#8212; lsqfit 9.5 documentation</title>
     <link rel="stylesheet" href="_static/pyramid.css" type="text/css" />
     <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
     <script type="text/javascript" src="_static/documentation_options.js"></script>
     <script type="text/javascript" src="_static/jquery.js"></script>
     <script type="text/javascript" src="_static/underscore.js"></script>
     <script type="text/javascript" src="_static/doctools.js"></script>
     <link rel="index" title="Index" href="#" />
@@ -29,15 +29,15 @@
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="#" title="General Index"
              accesskey="I">index</a></li>
         <li class="right" >
           <a href="py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">lsqfit 9.4 documentation</a> &#187;</li> 
+        <li class="nav-item nav-item-0"><a href="index.html">lsqfit 9.5 documentation</a> &#187;</li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
           <div class="body" role="main">
@@ -139,23 +139,19 @@
 <h2 id="D">D</h2>
 <table style="width: 100%" class="indextable genindextable"><tr>
   <td style="width: 33%; vertical-align: top;"><ul>
       <li><a href="lsqfit.html#lsqfit.MultiFitterModel.datatag">datatag (lsqfit.MultiFitterModel attribute)</a>
 </li>
       <li><a href="lsqfit.html#gvar.del_parameter_distribution">del_parameter_distribution() (in module gvar)</a>
 </li>
-      <li><a href="scipy.html#lsqfit.scipy_least_squares.description">description (lsqfit.scipy_least_squares attribute)</a>
-</li>
   </ul></td>
   <td style="width: 33%; vertical-align: top;"><ul>
-      <li><a href="lsqfit.html#lsqfit.nonlinear_fit.dof">dof (lsqfit.nonlinear_fit attribute)</a>
-</li>
-      <li><a href="lsqfit.html#lsqfit.nonlinear_fit.dump_p">dump_p() (lsqfit.nonlinear_fit method)</a>
+      <li><a href="scipy.html#lsqfit.scipy_least_squares.description">description (lsqfit.scipy_least_squares attribute)</a>
 </li>
-      <li><a href="lsqfit.html#lsqfit.nonlinear_fit.dump_pmean">dump_pmean() (lsqfit.nonlinear_fit method)</a>
+      <li><a href="lsqfit.html#lsqfit.nonlinear_fit.dof">dof (lsqfit.nonlinear_fit attribute)</a>
 </li>
   </ul></td>
 </tr></table>
 
 <h2 id="E">E</h2>
 <table style="width: 100%" class="indextable genindextable"><tr>
   <td style="width: 33%; vertical-align: top;"><ul>
@@ -213,16 +209,14 @@
 </li>
   </ul></td>
 </tr></table>
 
 <h2 id="L">L</h2>
 <table style="width: 100%" class="indextable genindextable"><tr>
   <td style="width: 33%; vertical-align: top;"><ul>
-      <li><a href="lsqfit.html#lsqfit.nonlinear_fit.load_parameters">load_parameters() (lsqfit.nonlinear_fit static method)</a>
-</li>
       <li><a href="lsqfit.html#lsqfit.nonlinear_fit.logGBF">logGBF (lsqfit.nonlinear_fit attribute)</a>
 </li>
       <li><a href="lsqfit.html#lsqfit.BayesPDF.logpdf">logpdf() (lsqfit.BayesPDF method)</a>
 </li>
       <li><a href="lsqfit.html#module-lsqfit">lsqfit (module)</a>
 </li>
   </ul></td>
@@ -410,15 +404,15 @@
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="#" title="General Index"
              >index</a></li>
         <li class="right" >
           <a href="py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">lsqfit 9.4 documentation</a> &#187;</li> 
+        <li class="nav-item nav-item-0"><a href="index.html">lsqfit 9.5 documentation</a> &#187;</li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
         &#169; Copyright 2009-2018, G. P. Lepage.
       Created using <a href="http://sphinx-doc.org/">Sphinx</a> 1.7.4.
     </div>
   </body>
```

#### html2text {}

```diff
@@ -5,15 +5,15 @@
 
 
 
 
 **** Navigation ****
     * index
     * modules |
-    * lsqfit_9.4_documentation »
+    * lsqfit_9.5_documentation »
 ****** Index ******
 _ | A | B | C | D | E | F | G | J | L | M | N | P | Q | R | S | T | W | X | Y
 ***** _ *****
     * __call__()_(lsqfit.BayesIntegrator_method)
           o (lsqfit.BayesPDF_method)
 ***** A *****
     * add_parameter_distribution()_(in     * add_parameter_parentheses()_(in
@@ -28,21 +28,19 @@
 ***** C *****
     * chained_lsqfit()_                 * chi2_(lsqfit.nonlinear_fit
       (lsqfit.MultiFitter_method)         attribute)
     * check_roundoff()_                 * cov_(lsqfit.nonlinear_fit_attribute)
       (lsqfit.nonlinear_fit_method)           o (lsqfit.scipy_least_squares
                                                 attribute)
 ***** D *****
-    * datatag_(lsqfit.MultiFitterModel     * dof_(lsqfit.nonlinear_fit
-      attribute)                             attribute)
-    * del_parameter_distribution()_(in     * dump_p()_(lsqfit.nonlinear_fit
-      module_gvar)                           method)
-    * description_                         * dump_pmean()_(lsqfit.nonlinear_fit
-      (lsqfit.scipy_least_squares            method)
-      attribute)
+    * datatag_(lsqfit.MultiFitterModel     * description_
+      attribute)                             (lsqfit.scipy_least_squares
+    * del_parameter_distribution()_(in       attribute)
+      module_gvar)                         * dof_(lsqfit.nonlinear_fit
+                                             attribute)
 ***** E *****
     * empbayes_fit()_(in_module_lsqfit)
     * error_(lsqfit.nonlinear_fit_attribute)
           o (lsqfit.scipy_least_squares_attribute)
           o (lsqfit.scipy_multiminex_attribute)
 ***** F *****
     * f_(lsqfit.scipy_least_squares         * fitter_results_
@@ -54,21 +52,21 @@
                                               method)
 ***** G *****
     * gammaQ()_(in_module_lsqfit)     * get_prior_keys()_
                                         (lsqfit.MultiFitterModel_static_method)
 ***** J *****
     * J_(lsqfit.scipy_least_squares_attribute)
 ***** L *****
-    * load_parameters()_                    * lsqfit()_(lsqfit.MultiFitter
-      (lsqfit.nonlinear_fit_static            method)
-      method)                               * lsqfit.gsl_multifit_(built-in
-    * logGBF_(lsqfit.nonlinear_fit            class)
-      attribute)                            * lsqfit.gsl_multiminex_(built-in
-    * logpdf()_(lsqfit.BayesPDF_method)       class)
-    * lsqfit_(module)                       * lsqfit.gsl_v1_multifit_(built-in
+                                            * lsqfit()_(lsqfit.MultiFitter
+                                              method)
+    * logGBF_(lsqfit.nonlinear_fit          * lsqfit.gsl_multifit_(built-in
+      attribute)                              class)
+    * logpdf()_(lsqfit.BayesPDF_method)     * lsqfit.gsl_multiminex_(built-in
+    * lsqfit_(module)                         class)
+                                            * lsqfit.gsl_v1_multifit_(built-in
                                               class)
 ***** M *****
     * MultiFitter_(class_in_lsqfit)     * MultiFitterModel_(class_in_lsqfit)
 ***** N *****
     * nblocks_(lsqfit.nonlinear_fit     * nit_(lsqfit.scipy_least_squares
       attribute)                          attribute)
     * ncg_(lsqfit.MultiFitterModel            o (lsqfit.scipy_multiminex
@@ -113,9 +111,9 @@
 ***** Y *****
     * y_(lsqfit.nonlinear_fit_attribute)
 **** Quick search ****
 [q                   ] [Go]
 **** Navigation ****
     * index
     * modules |
-    * lsqfit_9.4_documentation »
+    * lsqfit_9.5_documentation »
 © Copyright 2009-2018, G. P. Lepage. Created using Sphinx 1.7.4.
```

### Comparing `lsqfit-9.4/doc/html/lsqfit.html` & `lsqfit-9.5/doc/html/lsqfit.html`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 <!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Transitional//EN"
   "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
 
 <html xmlns="http://www.w3.org/1999/xhtml">
   <head>
     <meta http-equiv="X-UA-Compatible" content="IE=Edge" />
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
-    <title>lsqfit - Nonlinear Least Squares Fitting &#8212; lsqfit 9.4 documentation</title>
+    <title>lsqfit - Nonlinear Least Squares Fitting &#8212; lsqfit 9.5 documentation</title>
     <link rel="stylesheet" href="_static/pyramid.css" type="text/css" />
     <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
     <script type="text/javascript" src="_static/documentation_options.js"></script>
     <script type="text/javascript" src="_static/jquery.js"></script>
     <script type="text/javascript" src="_static/underscore.js"></script>
     <script type="text/javascript" src="_static/doctools.js"></script>
     <link rel="index" title="Index" href="genindex.html" />
@@ -36,15 +36,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="gsl.html" title="GSL Routines"
              accesskey="N">next</a> |</li>
         <li class="right" >
           <a href="case-outliers.html" title="Case Study: Outliers and Bayesian Integrals"
              accesskey="P">previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">lsqfit 9.4 documentation</a> &#187;</li> 
+        <li class="nav-item nav-item-0"><a href="index.html">lsqfit 9.5 documentation</a> &#187;</li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
           <div class="body" role="main">
@@ -217,14 +217,29 @@
 from that file; best-fit parameter values are written out to the
 same file after the fit (for priming future fits). If <code class="docutils literal notranslate"><span class="pre">p0</span></code> is
 <code class="docutils literal notranslate"><span class="pre">None</span></code> or the attempt to read the file fails, starting values
 are extracted from <code class="docutils literal notranslate"><span class="pre">prior</span></code>. If <code class="docutils literal notranslate"><span class="pre">p0</span></code> is <code class="docutils literal notranslate"><span class="pre">True</span></code>, it
 is replaced by a starting point drawn at random from the
 <code class="docutils literal notranslate"><span class="pre">prior</span></code> distribution. The default value is <code class="docutils literal notranslate"><span class="pre">None</span></code>;
 <code class="docutils literal notranslate"><span class="pre">p0</span></code> must be explicitly specified if <code class="docutils literal notranslate"><span class="pre">prior</span></code> is <code class="docutils literal notranslate"><span class="pre">None</span></code>.</li>
+<li><strong>linear</strong> (<em>list</em><em> or </em><em>None</em>) – Optional list of fit parameters that appear
+linearly in the fit function. The fit function can be reexpressed
+(using <em>variable projection</em>) as a function that is independent of
+its linear parameters. The resulting fit has fewer fit parameters
+and typically will converge in fewer iterations, but each
+iteration will take longer. Whether or not the fit is faster or
+more robust in any particular application is a matter for
+experiment, but answers should be the same either way. The linear
+parameters are reconstructed from the nonlinear parameters (and
+the data) after the fit. Parameter <code class="docutils literal notranslate"><span class="pre">linear</span></code> is either: a list of
+dictionary keys corresponding to linear parameters when the
+parameters are stored in a dictionary (see <code class="docutils literal notranslate"><span class="pre">prior</span></code>); or, a list
+of indices corresponding to these parameters when they are stored
+in an array. Note that this feature is experimental; the
+interface may change in the future.</li>
 <li><strong>svdcut</strong> (<em>float</em><em> or </em><em>None</em>) – If <code class="docutils literal notranslate"><span class="pre">svdcut</span></code> is nonzero
 (but not <code class="docutils literal notranslate"><span class="pre">None</span></code>), SVD cuts are applied to every block-diagonal
 sub-matrix of the covariance matrix for the data <code class="docutils literal notranslate"><span class="pre">y</span></code> and <code class="docutils literal notranslate"><span class="pre">prior</span></code>
 (if there is a prior). The blocks are first rescaled so that all
 diagonal elements equal 1 – that is, the blocks are replaced by
 the correlation matrices for the corresponding subsets of
 variables. Then, if <code class="docutils literal notranslate"><span class="pre">svdcut</span> <span class="pre">&gt;</span> <span class="pre">0</span></code>, eigenvalues of the rescaled
@@ -492,51 +507,55 @@
 ‘fitter’. Additional defaults can be added to that dictionary
 to be are passed through <a class="reference internal" href="#lsqfit.nonlinear_fit" title="lsqfit.nonlinear_fit"><code class="xref py py-class docutils literal notranslate"><span class="pre">lsqfit.nonlinear_fit</span></code></a> to the underlying
 fitter (via dictionary <code class="docutils literal notranslate"><span class="pre">fitterargs</span></code>).</p>
 <p>Additional methods are provided for printing out detailed information
 about the fit, testing fits with simulated data,
 doing bootstrap analyses of the fit errors,
 dumping (for later use) and loading parameter values, and checking for roundoff
-errors in the final error estimates:</p>
+errors in the final error  estimates:</p>
 <dl class="method">
 <dt id="lsqfit.nonlinear_fit.format">
 <code class="descname">format</code><span class="sig-paren">(</span><em>maxline=0</em>, <em>pstyle='v'</em><span class="sig-paren">)</span><a class="headerlink" href="#lsqfit.nonlinear_fit.format" title="Permalink to this definition">¶</a></dt>
 <dd><p>Formats fit output details into a string for printing.</p>
 <p>The output tabulates the <code class="docutils literal notranslate"><span class="pre">chi**2</span></code> per degree of freedom of the fit
-(<code class="docutils literal notranslate"><span class="pre">chi2/dof</span></code>), the number of degrees of freedom, the logarithm of the
-Gaussian Bayes Factor for the fit (<code class="docutils literal notranslate"><span class="pre">logGBF</span></code>), and the number of fit-
-algorithm iterations needed by the fit. Optionally, it will also list
-the best-fit values for the fit parameters together with the prior for
-each (in <code class="docutils literal notranslate"><span class="pre">[]</span></code> on each line). Lines for parameters that deviate from
-their prior by more than one (prior) standard deviation are marked
-with asterisks, with the number of asterisks equal to the number of
-standard deviations (up to five). <code class="docutils literal notranslate"><span class="pre">format</span></code> can also list all of the
-data and the corresponding values from the fit, again with asterisks
-on lines  where there is a significant discrepancy. At the end it
-lists the SVD cut, the number of eigenmodes modified by the SVD cut,
-the tolerances used in the fit, and the time in seconds needed to do
-the fit. The tolerance used to terminate the fit is marked with an
-asterisk.</p>
+(<code class="docutils literal notranslate"><span class="pre">chi2/dof</span></code>), the number of degrees of freedom, the <code class="docutils literal notranslate"><span class="pre">Q</span></code>  value of
+the fit (ie, p-value), and the logarithm of the Gaussian Bayes Factor
+for the fit (<code class="docutils literal notranslate"><span class="pre">logGBF</span></code>). At the end it lists the SVD cut, the number
+of eigenmodes modified by the SVD cut, the tolerances used in the fit,
+and the time in seconds needed to do the fit. The tolerance used to
+terminate the fit is marked with an asterisk. It also lists
+information about the fitter used if it is other than the standard
+choice.</p>
+<p>Optionally, <code class="docutils literal notranslate"><span class="pre">format</span></code> will also list the best-fit values
+for the fit parameters together with the prior for each (in <code class="docutils literal notranslate"><span class="pre">[]</span></code> on
+each line). Lines for parameters that deviate from their prior by more
+than one (prior) standard deviation are marked with asterisks, with
+the number of asterisks equal to the number of standard deviations (up
+to five). Lines for parameters designated as linear (see <code class="docutils literal notranslate"><span class="pre">linear</span></code>
+keyword) are marked with a minus sign after their prior.</p>
+<p><code class="docutils literal notranslate"><span class="pre">format</span></code> can also list all of the data and the corresponding values
+from the fit, again with asterisks on lines  where there is a
+significant discrepancy.</p>
 <table class="docutils field-list" frame="void" rules="none">
 <col class="field-name" />
 <col class="field-body" />
 <tbody valign="top">
 <tr class="field-odd field"><th class="field-name">Parameters:</th><td class="field-body"><ul class="first simple">
-<li><strong>maxline</strong> (<em>integer</em><em> or </em><em>bool</em>) – Maximum number of data points for which fit
-results and input data are tabulated. <code class="docutils literal notranslate"><span class="pre">maxline&lt;0</span></code> implies
-that only <code class="docutils literal notranslate"><span class="pre">chi2</span></code>, <code class="docutils literal notranslate"><span class="pre">Q</span></code>, <code class="docutils literal notranslate"><span class="pre">logGBF</span></code>, and <code class="docutils literal notranslate"><span class="pre">itns</span></code> are
-tabulated; no parameter values are included. Setting
+<li><strong>maxline</strong> (<em>int</em><em> or </em><em>bool</em>) – Maximum number of data points for which
+fit results and input data are tabulated. <code class="docutils literal notranslate"><span class="pre">maxline&lt;0</span></code>
+implies that only <code class="docutils literal notranslate"><span class="pre">chi2</span></code>, <code class="docutils literal notranslate"><span class="pre">Q</span></code>, <code class="docutils literal notranslate"><span class="pre">logGBF</span></code>, and <code class="docutils literal notranslate"><span class="pre">itns</span></code>
+are tabulated; no parameter values are included. Setting
 <code class="docutils literal notranslate"><span class="pre">maxline=True</span></code> prints all data points; setting it
 equal <code class="docutils literal notranslate"><span class="pre">None</span></code> or <code class="docutils literal notranslate"><span class="pre">False</span></code> is the same as setting
 it equal to <code class="docutils literal notranslate"><span class="pre">-1</span></code>. Default is <code class="docutils literal notranslate"><span class="pre">maxline=0</span></code>.</li>
-<li><strong>pstyle</strong> (‘vv’, ‘v’, ‘m’, or <code class="docutils literal notranslate"><span class="pre">None</span></code>) – Style used for parameter list. Supported values are
-‘vv’ for very verbose, ‘v’ for verbose, and ‘m’ for minimal.
-When ‘m’ is set, only parameters whose values differ from their
-prior values are listed. Setting <code class="docutils literal notranslate"><span class="pre">pstyle=None</span></code> implies
-no parameters are listed.</li>
+<li><strong>pstyle</strong> (<em>str</em><em> or </em><em>None</em>) – Style used for parameter list. Supported
+values are ‘vv’ for very verbose, ‘v’ for verbose, and ‘m’ for
+minimal. When ‘m’ is set, only parameters whose values differ
+from their prior values are listed. Setting <code class="docutils literal notranslate"><span class="pre">pstyle=None</span></code>
+implies no parameters are listed.</li>
 </ul>
 </td>
 </tr>
 <tr class="field-even field"><th class="field-name">Returns:</th><td class="field-body"><p class="first last">String containing detailed information about fit.</p>
 </td>
 </tr>
 </tbody>
@@ -692,50 +711,14 @@
 </td>
 </tr>
 </tbody>
 </table>
 </dd></dl>
 
 <dl class="method">
-<dt id="lsqfit.nonlinear_fit.dump_p">
-<code class="descname">dump_p</code><span class="sig-paren">(</span><em>filename</em><span class="sig-paren">)</span><a class="headerlink" href="#lsqfit.nonlinear_fit.dump_p" title="Permalink to this definition">¶</a></dt>
-<dd><p>Dump parameter values (<code class="docutils literal notranslate"><span class="pre">fit.p</span></code>) into file <code class="docutils literal notranslate"><span class="pre">filename</span></code>.</p>
-<p><code class="docutils literal notranslate"><span class="pre">fit.dump_p(filename)</span></code> saves the best-fit parameter values
-(<code class="docutils literal notranslate"><span class="pre">fit.p</span></code>) from a <code class="docutils literal notranslate"><span class="pre">nonlinear_fit</span></code> called <code class="docutils literal notranslate"><span class="pre">fit</span></code>. These values
-are recovered using
-<code class="docutils literal notranslate"><span class="pre">p</span> <span class="pre">=</span> <span class="pre">nonlinear_fit.load_parameters(filename)</span></code>
-where <code class="docutils literal notranslate"><span class="pre">p</span></code>’s layout is the same as that of <code class="docutils literal notranslate"><span class="pre">fit.p</span></code>.</p>
-</dd></dl>
-
-<dl class="method">
-<dt id="lsqfit.nonlinear_fit.dump_pmean">
-<code class="descname">dump_pmean</code><span class="sig-paren">(</span><em>filename</em><span class="sig-paren">)</span><a class="headerlink" href="#lsqfit.nonlinear_fit.dump_pmean" title="Permalink to this definition">¶</a></dt>
-<dd><p>Dump parameter means (<code class="docutils literal notranslate"><span class="pre">fit.pmean</span></code>) into file <code class="docutils literal notranslate"><span class="pre">filename</span></code>.</p>
-<p><code class="docutils literal notranslate"><span class="pre">fit.dump_pmean(filename)</span></code> saves the means of the best-fit
-parameter values (<code class="docutils literal notranslate"><span class="pre">fit.pmean</span></code>) from a <code class="docutils literal notranslate"><span class="pre">nonlinear_fit</span></code> called
-<code class="docutils literal notranslate"><span class="pre">fit</span></code>. These values are recovered using
-<code class="docutils literal notranslate"><span class="pre">p0</span> <span class="pre">=</span> <span class="pre">nonlinear_fit.load_parameters(filename)</span></code>
-where <code class="docutils literal notranslate"><span class="pre">p0</span></code>’s layout is the same as <code class="docutils literal notranslate"><span class="pre">fit.pmean</span></code>. The saved
-values can be used to initialize a later fit (<code class="docutils literal notranslate"><span class="pre">nonlinear_fit</span></code>
-parameter <code class="docutils literal notranslate"><span class="pre">p0</span></code>).</p>
-</dd></dl>
-
-<dl class="staticmethod">
-<dt id="lsqfit.nonlinear_fit.load_parameters">
-<em class="property">static </em><code class="descname">load_parameters</code><span class="sig-paren">(</span><em>filename</em><span class="sig-paren">)</span><a class="headerlink" href="#lsqfit.nonlinear_fit.load_parameters" title="Permalink to this definition">¶</a></dt>
-<dd><p>Load parameters stored in file <code class="docutils literal notranslate"><span class="pre">filename</span></code>.</p>
-<p><code class="docutils literal notranslate"><span class="pre">p</span> <span class="pre">=</span> <span class="pre">nonlinear_fit.load_p(filename)</span></code> is used to recover the
-values of fit parameters dumped using <code class="docutils literal notranslate"><span class="pre">fit.dump_p(filename)</span></code> (or
-<code class="docutils literal notranslate"><span class="pre">fit.dump_pmean(filename)</span></code>) where <code class="docutils literal notranslate"><span class="pre">fit</span></code> is of type
-<a class="reference internal" href="#lsqfit.nonlinear_fit" title="lsqfit.nonlinear_fit"><code class="xref py py-class docutils literal notranslate"><span class="pre">lsqfit.nonlinear_fit</span></code></a>. The layout of the returned
-parameters <code class="docutils literal notranslate"><span class="pre">p</span></code> is the same as that of <code class="docutils literal notranslate"><span class="pre">fit.p</span></code> (or
-<code class="docutils literal notranslate"><span class="pre">fit.pmean</span></code>).</p>
-</dd></dl>
-
-<dl class="method">
 <dt id="lsqfit.nonlinear_fit.check_roundoff">
 <code class="descname">check_roundoff</code><span class="sig-paren">(</span><em>rtol=0.25</em>, <em>atol=1e-6</em><span class="sig-paren">)</span><a class="headerlink" href="#lsqfit.nonlinear_fit.check_roundoff" title="Permalink to this definition">¶</a></dt>
 <dd><p>Check for roundoff errors in fit.p.</p>
 <p>Compares standard deviations from fit.p and fit.palt to see if they
 agree to within relative tolerance <code class="docutils literal notranslate"><span class="pre">rtol</span></code> and absolute tolerance
 <code class="docutils literal notranslate"><span class="pre">atol</span></code>. Generates a warning if they do not (in which
 case an SVD cut might be advisable).</p>
@@ -2022,15 +2005,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="gsl.html" title="GSL Routines"
              >next</a> |</li>
         <li class="right" >
           <a href="case-outliers.html" title="Case Study: Outliers and Bayesian Integrals"
              >previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">lsqfit 9.4 documentation</a> &#187;</li> 
+        <li class="nav-item nav-item-0"><a href="index.html">lsqfit 9.5 documentation</a> &#187;</li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
         &#169; Copyright 2009-2018, G. P. Lepage.
       Created using <a href="http://sphinx-doc.org/">Sphinx</a> 1.7.4.
     </div>
   </body>
```

#### html2text {}

```diff
@@ -9,15 +9,15 @@
 
 
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * lsqfit_9.4_documentation »
+    * lsqfit_9.5_documentation »
 ****** lsqfit - Nonlinear Least Squares FittingÂ¶ ******
 ***** IntroductionÂ¶ *****
 This package contains tools for nonlinear least-squares curve fitting of data.
 In general a fit has four inputs:
         1. The dependent data y that is to be fit â typically y is a
            Python dictionary in an lsqfit analysis. Its values y[k] are
            either gvar.GVars or arrays (any shape or dimension) of
@@ -146,18 +146,32 @@
                         parameters in fit. lsqfit.nonlinear_fit adjusts p0 to make it
                         consistent in shape and structure with prior when the latter is
                         specified: elements missing from p0 are filled in using prior, and
                         elements in p0 that are not in prior are discarded. If p0 is a string,
                         it is taken as a file name and lsqfit.nonlinear_fit attempts to read
                         starting values from that file; best-fit parameter values are written
                         out to the same file after the fit (for priming future fits). If p0 is
-      Parameters:       None or the attempt to read the file fails, starting values are
+                        None or the attempt to read the file fails, starting values are
                         extracted from prior. If p0 is True, it is replaced by a starting
                         point drawn at random from the prior distribution. The default value
                         is None; p0 must be explicitly specified if prior is None.
+                      * linear (listorNone) â Optional list of fit parameters that appear
+                        linearly in the fit function. The fit function can be reexpressed
+                        (using variable projection) as a function that is independent of its
+      Parameters:       linear parameters. The resulting fit has fewer fit parameters and
+                        typically will converge in fewer iterations, but each iteration will
+                        take longer. Whether or not the fit is faster or more robust in any
+                        particular application is a matter for experiment, but answers should
+                        be the same either way. The linear parameters are reconstructed from
+                        the nonlinear parameters (and the data) after the fit. Parameter
+                        linear is either: a list of dictionary keys corresponding to linear
+                        parameters when the parameters are stored in a dictionary (see prior);
+                        or, a list of indices corresponding to these parameters when they are
+                        stored in an array. Note that this feature is experimental; the
+                        interface may change in the future.
                       * svdcut (floatorNone) â If svdcut is nonzero (but not None), SVD cuts
                         are applied to every block-diagonal sub-matrix of the covariance
                         matrix for the data y and prior (if there is a prior). The blocks are
                         first rescaled so that all diagonal elements equal 1 â that is, the
                         blocks are replaced by the correlation matrices for the corresponding
                         subsets of variables. Then, if svdcut > 0, eigenvalues of the rescaled
                         matrices that are smaller than svdcut times the maximum eigenvalue are
@@ -323,37 +337,42 @@
       Additional methods are provided for printing out detailed information
       about the fit, testing fits with simulated data, doing bootstrap analyses
       of the fit errors, dumping (for later use) and loading parameter values,
       and checking for roundoff errors in the final error estimates:
         format(maxline=0, pstyle='v')Â¶
             Formats fit output details into a string for printing.
             The output tabulates the chi**2 per degree of freedom of the fit
-            (chi2/dof), the number of degrees of freedom, the logarithm of the
-            Gaussian Bayes Factor for the fit (logGBF), and the number of fit-
-            algorithm iterations needed by the fit. Optionally, it will also
-            list the best-fit values for the fit parameters together with the
-            prior for each (in [] on each line). Lines for parameters that
-            deviate from their prior by more than one (prior) standard
-            deviation are marked with asterisks, with the number of asterisks
-            equal to the number of standard deviations (up to five). format can
-            also list all of the data and the corresponding values from the
-            fit, again with asterisks on lines where there is a significant
-            discrepancy. At the end it lists the SVD cut, the number of
-            eigenmodes modified by the SVD cut, the tolerances used in the fit,
-            and the time in seconds needed to do the fit. The tolerance used to
-            terminate the fit is marked with an asterisk.
-                            * maxline (integerorbool) â Maximum number of data points for which fit results
-                              and input data are tabulated. maxline<0 implies that only chi2, Q, logGBF, and
-                              itns are tabulated; no parameter values are included. Setting maxline=True
-                              prints all data points; setting it equal None or False is the same as setting it
-            Parameters:       equal to -1. Default is maxline=0.
-                            * pstyle (âvvâ, âvâ, âmâ, or None) â Style used for parameter list.
-                              Supported values are âvvâ for very verbose, âvâ for verbose, and âmâ
-                              for minimal. When âmâ is set, only parameters whose values differ from their
-                              prior values are listed. Setting pstyle=None implies no parameters are listed.
+            (chi2/dof), the number of degrees of freedom, the Q value of the
+            fit (ie, p-value), and the logarithm of the Gaussian Bayes Factor
+            for the fit (logGBF). At the end it lists the SVD cut, the number
+            of eigenmodes modified by the SVD cut, the tolerances used in the
+            fit, and the time in seconds needed to do the fit. The tolerance
+            used to terminate the fit is marked with an asterisk. It also lists
+            information about the fitter used if it is other than the standard
+            choice.
+            Optionally, format will also list the best-fit values for the fit
+            parameters together with the prior for each (in [] on each line).
+            Lines for parameters that deviate from their prior by more than one
+            (prior) standard deviation are marked with asterisks, with the
+            number of asterisks equal to the number of standard deviations (up
+            to five). Lines for parameters designated as linear (see linear
+            keyword) are marked with a minus sign after their prior.
+            format can also list all of the data and the corresponding values
+            from the fit, again with asterisks on lines where there is a
+            significant discrepancy.
+                            * maxline (intorbool) â Maximum number of data points for which fit
+                              results and input data are tabulated. maxline<0 implies that only chi2,
+                              Q, logGBF, and itns are tabulated; no parameter values are included.
+                              Setting maxline=True prints all data points; setting it equal None or
+            Parameters:       False is the same as setting it equal to -1. Default is maxline=0.
+                            * pstyle (strorNone) â Style used for parameter list. Supported values
+                              are âvvâ for very verbose, âvâ for verbose, and âmâ for
+                              minimal. When âmâ is set, only parameters whose values differ from
+                              their prior values are listed. Setting pstyle=None implies no
+                              parameters are listed.
             Returns:    String containing detailed information about fit.
         simulated_fit_iter(n=None, pexact=None, **kargs)Â¶
             Iterator that returns simulation copies of a fit.
             Fit reliability can be tested using simulated data which replaces
             the mean values in self.y with random numbers drawn from a
             distribution whose mean equals self.fcn(pexact) and whose
             covariance matrix is the same as self.yâs. Simulated data is very
@@ -460,34 +479,14 @@
                             * n (int) â Maximum number of iterations if n is not None;
                               otherwise there is no maximum.
             Parameters:     * datalist (iter) â Collection of bootstrap data sets for
                               fitter.
                             * kargs (dict) â Overrides arguments in original fit.
             Returns:    Iterator that returns an lsqfit.nonlinear_fit object containing
                         results from the fit to the next data set in datalist.
-        dump_p(filename)Â¶
-            Dump parameter values (fit.p) into file filename.
-            fit.dump_p(filename) saves the best-fit parameter values (fit.p)
-            from a nonlinear_fit called fit. These values are recovered using p
-            = nonlinear_fit.load_parameters(filename) where pâs layout is the
-            same as that of fit.p.
-        dump_pmean(filename)Â¶
-            Dump parameter means (fit.pmean) into file filename.
-            fit.dump_pmean(filename) saves the means of the best-fit parameter
-            values (fit.pmean) from a nonlinear_fit called fit. These values
-            are recovered using p0 = nonlinear_fit.load_parameters(filename)
-            where p0âs layout is the same as fit.pmean. The saved values can
-            be used to initialize a later fit (nonlinear_fit parameter p0).
-        staticload_parameters(filename)Â¶
-            Load parameters stored in file filename.
-            p = nonlinear_fit.load_p(filename) is used to recover the values of
-            fit parameters dumped using fit.dump_p(filename) (or fit.dump_pmean
-            (filename)) where fit is of type lsqfit.nonlinear_fit. The layout
-            of the returned parameters p is the same as that of fit.p (or
-            fit.pmean).
         check_roundoff(rtol=0.25, atol=1e-6)Â¶
             Check for roundoff errors in fit.p.
             Compares standard deviations from fit.p and fit.palt to see if they
             agree to within relative tolerance rtol and absolute tolerance
             atol. Generates a warning if they do not (in which case an SVD cut
             might be advisable).
         staticset(clear=False, **defaults)Â¶
@@ -1330,9 +1329,9 @@
 **** Quick search ****
 [q                   ] [Go]
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * lsqfit_9.4_documentation »
+    * lsqfit_9.5_documentation »
 © Copyright 2009-2018, G. P. Lepage. Created using Sphinx 1.7.4.
```

### Comparing `lsqfit-9.4/doc/html/search.html` & `lsqfit-9.5/doc/html/search.html`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 <!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Transitional//EN"
   "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
 
 <html xmlns="http://www.w3.org/1999/xhtml">
   <head>
     <meta http-equiv="X-UA-Compatible" content="IE=Edge" />
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
-    <title>Search &#8212; lsqfit 9.4 documentation</title>
+    <title>Search &#8212; lsqfit 9.5 documentation</title>
     <link rel="stylesheet" href="_static/pyramid.css" type="text/css" />
     <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
     <script type="text/javascript" src="_static/documentation_options.js"></script>
     <script type="text/javascript" src="_static/jquery.js"></script>
     <script type="text/javascript" src="_static/underscore.js"></script>
     <script type="text/javascript" src="_static/doctools.js"></script>
     <script type="text/javascript" src="_static/searchtools.js"></script>
@@ -36,15 +36,15 @@
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="genindex.html" title="General Index"
              accesskey="I">index</a></li>
         <li class="right" >
           <a href="py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">lsqfit 9.4 documentation</a> &#187;</li> 
+        <li class="nav-item nav-item-0"><a href="index.html">lsqfit 9.5 documentation</a> &#187;</li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
           <div class="body" role="main">
@@ -87,15 +87,15 @@
       <ul>
         <li class="right" style="margin-right: 10px">
           <a href="genindex.html" title="General Index"
              >index</a></li>
         <li class="right" >
           <a href="py-modindex.html" title="Python Module Index"
              >modules</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">lsqfit 9.4 documentation</a> &#187;</li> 
+        <li class="nav-item nav-item-0"><a href="index.html">lsqfit 9.5 documentation</a> &#187;</li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
         &#169; Copyright 2009-2018, G. P. Lepage.
       Created using <a href="http://sphinx-doc.org/">Sphinx</a> 1.7.4.
     </div>
   </body>
```

### Comparing `lsqfit-9.4/doc/html/.doctrees/case-pendulum.doctree` & `lsqfit-9.5/doc/html/.doctrees/case-pendulum.doctree`

 * *Files identical despite different names*

### Comparing `lsqfit-9.4/doc/html/.doctrees/case-extrapolation.doctree` & `lsqfit-9.5/doc/html/.doctrees/case-extrapolation.doctree`

 * *Files identical despite different names*

### Comparing `lsqfit-9.4/doc/html/.doctrees/gsl.doctree` & `lsqfit-9.5/doc/html/.doctrees/gsl.doctree`

 * *Files identical despite different names*

### Comparing `lsqfit-9.4/doc/html/.doctrees/testing.doctree` & `lsqfit-9.5/doc/html/.doctrees/testing.doctree`

 * *Files identical despite different names*

### Comparing `lsqfit-9.4/doc/html/.doctrees/environment.pickle` & `lsqfit-9.5/doc/html/.doctrees/environment.pickle`

 * *Files 16% similar despite different names*

```diff
@@ -206,2154 +206,2129 @@
 00000cd0: 8658 2800 0000 6c73 7166 6974 2e4d 756c  .X(...lsqfit.Mul
 00000ce0: 7469 4669 7474 6572 2e62 6f6f 7473 7472  tiFitter.bootstr
 00000cf0: 6170 7065 645f 6669 745f 6974 6572 71ba  apped_fit_iterq.
 00000d00: 682b 5806 0000 006d 6574 686f 6471 bb86  h+X....methodq..
 00000d10: 5818 0000 006c 7371 6669 742e 6e6f 6e6c  X....lsqfit.nonl
 00000d20: 696e 6561 725f 6669 742e 636f 7671 bc68  inear_fit.covq.h
 00000d30: 2b58 0900 0000 6174 7472 6962 7574 6571  +X....attributeq
-00000d40: bd86 581b 0000 006c 7371 6669 742e 6e6f  ..X....lsqfit.no
-00000d50: 6e6c 696e 6561 725f 6669 742e 6475 6d70  nlinear_fit.dump
-00000d60: 5f70 71be 682b 5806 0000 006d 6574 686f  _pq.h+X....metho
-00000d70: 6471 bf86 5819 0000 006c 7371 6669 742e  dq..X....lsqfit.
-00000d80: 6e6f 6e6c 696e 6561 725f 6669 742e 7469  nonlinear_fit.ti
-00000d90: 6d65 71c0 682b 5809 0000 0061 7474 7269  meq.h+X....attri
-00000da0: 6275 7465 71c1 8658 1a00 0000 6c73 7166  buteq..X....lsqf
-00000db0: 6974 2e73 6369 7079 5f6c 6561 7374 5f73  it.scipy_least_s
-00000dc0: 7175 6172 6573 71c2 6858 5805 0000 0063  quaresq.hXX....c
-00000dd0: 6c61 7373 71c3 8658 1900 0000 6c73 7166  lassq..X....lsqf
-00000de0: 6974 2e4d 756c 7469 4669 7474 6572 2e6c  it.MultiFitter.l
-00000df0: 7371 6669 7471 c468 2b58 0600 0000 6d65  sqfitq.h+X....me
-00000e00: 7468 6f64 71c5 8658 1b00 0000 6c73 7166  thodq..X....lsqf
-00000e10: 6974 2e6e 6f6e 6c69 6e65 6172 5f66 6974  it.nonlinear_fit
-00000e20: 2e66 6f72 6d61 7471 c668 2b58 0600 0000  .formatq.h+X....
-00000e30: 6d65 7468 6f64 71c7 8658 1f00 0000 6776  methodq..X....gv
-00000e40: 6172 2e64 656c 5f70 6172 616d 6574 6572  ar.del_parameter
-00000e50: 5f64 6973 7472 6962 7574 696f 6e71 c868  _distributionq.h
-00000e60: 2b58 0800 0000 6675 6e63 7469 6f6e 71c9  +X....functionq.
-00000e70: 8658 1600 0000 6c73 7166 6974 2e42 6179  .X....lsqfit.Bay
-00000e80: 6573 496e 7465 6772 6174 6f72 71ca 682b  esIntegratorq.h+
-00000e90: 5805 0000 0063 6c61 7373 71cb 8658 2200  X....classq..X".
-00000ea0: 0000 6c73 7166 6974 2e6e 6f6e 6c69 6e65  ..lsqfit.nonline
-00000eb0: 6172 5f66 6974 2e73 7664 636f 7272 6563  ar_fit.svdcorrec
-00000ec0: 7469 6f6e 71cc 682b 5809 0000 0061 7474  tionq.h+X....att
-00000ed0: 7269 6275 7465 71cd 8658 1400 0000 6c73  ributeq..X....ls
-00000ee0: 7166 6974 2e6e 6f6e 6c69 6e65 6172 5f66  qfit.nonlinear_f
-00000ef0: 6974 71ce 682b 5805 0000 0063 6c61 7373  itq.h+X....class
-00000f00: 71cf 8658 1f00 0000 6c73 7166 6974 2e6e  q..X....lsqfit.n
-00000f10: 6f6e 6c69 6e65 6172 5f66 6974 2e64 756d  onlinear_fit.dum
-00000f20: 705f 706d 6561 6e71 d068 2b58 0600 0000  p_pmeanq.h+X....
-00000f30: 6d65 7468 6f64 71d1 8658 1700 0000 6c73  methodq..X....ls
-00000f40: 7166 6974 2e4d 756c 7469 4669 7474 6572  qfit.MultiFitter
-00000f50: 4d6f 6465 6c71 d268 2b58 0500 0000 636c  Modelq.h+X....cl
-00000f60: 6173 7371 d386 581f 0000 006c 7371 6669  assq..X....lsqfi
-00000f70: 742e 4261 7965 7349 6e74 6567 7261 746f  t.BayesIntegrato
-00000f80: 722e 5f5f 6361 6c6c 5f5f 71d4 682b 5806  r.__call__q.h+X.
-00000f90: 0000 006d 6574 686f 6471 d586 5819 0000  ...methodq..X...
-00000fa0: 006c 7371 6669 742e 6e6f 6e6c 696e 6561  .lsqfit.nonlinea
-00000fb0: 725f 6669 742e 6368 6932 71d6 682b 5809  r_fit.chi2q.h+X.
-00000fc0: 0000 0061 7474 7269 6275 7465 71d7 8658  ...attributeq..X
-00000fd0: 2200 0000 6c73 7166 6974 2e4d 756c 7469  "...lsqfit.Multi
-00000fe0: 4669 7474 6572 2e70 726f 6365 7373 5f64  Fitter.process_d
-00000ff0: 6174 6173 6574 71d8 682b 580c 0000 0073  atasetq.h+X....s
-00001000: 7461 7469 636d 6574 686f 6471 d986 581b  taticmethodq..X.
-00001010: 0000 006c 7371 6669 742e 7363 6970 795f  ...lsqfit.scipy_
-00001020: 6d75 6c74 696d 696e 6578 2e6e 6974 71da  multiminex.nitq.
-00001030: 6858 5809 0000 0061 7474 7269 6275 7465  hXX....attribute
-00001040: 71db 8658 1e00 0000 6c73 7166 6974 2e73  q..X....lsqfit.s
-00001050: 6369 7079 5f6c 6561 7374 5f73 7175 6172  cipy_least_squar
-00001060: 6573 2e6e 6974 71dc 6858 5809 0000 0061  es.nitq.hXX....a
-00001070: 7474 7269 6275 7465 71dd 8658 2400 0000  ttributeq..X$...
-00001080: 6c73 7166 6974 2e4d 756c 7469 4669 7474  lsqfit.MultiFitt
-00001090: 6572 4d6f 6465 6c2e 6275 696c 6464 6174  erModel.builddat
-000010a0: 6173 6574 71de 682b 5806 0000 006d 6574  asetq.h+X....met
-000010b0: 686f 6471 df86 581c 0000 006c 7371 6669  hodq..X....lsqfi
-000010c0: 742e 7363 6970 795f 6c65 6173 745f 7371  t.scipy_least_sq
-000010d0: 7561 7265 732e 4a71 e068 5858 0900 0000  uares.Jq.hXX....
-000010e0: 6174 7472 6962 7574 6571 e186 5820 0000  attributeq..X ..
-000010f0: 006c 7371 6669 742e 7363 6970 795f 6c65  .lsqfit.scipy_le
-00001100: 6173 745f 7371 7561 7265 732e 6572 726f  ast_squares.erro
-00001110: 7271 e268 5858 0900 0000 6174 7472 6962  rq.hXX....attrib
-00001120: 7574 6571 e386 5819 0000 006c 7371 6669  uteq..X....lsqfi
-00001130: 742e 6e6f 6e6c 696e 6561 725f 6669 742e  t.nonlinear_fit.
-00001140: 7061 6c74 71e4 682b 5809 0000 0061 7474  paltq.h+X....att
-00001150: 7269 6275 7465 71e5 8658 2200 0000 6c73  ributeq..X"...ls
-00001160: 7166 6974 2e4d 756c 7469 4669 7474 6572  qfit.MultiFitter
-00001170: 4d6f 6465 6c2e 6275 696c 6470 7269 6f72  Model.buildprior
-00001180: 71e6 682b 5806 0000 006d 6574 686f 6471  q.h+X....methodq
-00001190: e786 5813 0000 006c 7371 6669 742e 6773  ..X....lsqfit.gs
-000011a0: 6c5f 6d75 6c74 6966 6974 71e8 6871 5805  l_multifitq.hqX.
-000011b0: 0000 0063 6c61 7373 8658 1a00 0000 6c73  ...class.X....ls
-000011c0: 7166 6974 2e6e 6f6e 6c69 6e65 6172 5f66  qfit.nonlinear_f
-000011d0: 6974 2e70 6d65 616e 71e9 682b 5809 0000  it.pmeanq.h+X...
-000011e0: 0061 7474 7269 6275 7465 71ea 8658 2400  .attributeq..X$.
-000011f0: 0000 6c73 7166 6974 2e6e 6f6e 6c69 6e65  ..lsqfit.nonline
-00001200: 6172 5f66 6974 2e6c 6f61 645f 7061 7261  ar_fit.load_para
-00001210: 6d65 7465 7273 71eb 682b 580c 0000 0073  metersq.h+X....s
-00001220: 7461 7469 636d 6574 686f 6471 ec86 581a  taticmethodq..X.
-00001230: 0000 006c 7371 6669 742e 6e6f 6e6c 696e  ...lsqfit.nonlin
-00001240: 6561 725f 6669 742e 7072 696f 7271 ed68  ear_fit.priorq.h
-00001250: 2b58 0900 0000 6174 7472 6962 7574 6571  +X....attributeq
-00001260: ee86 5826 0000 006c 7371 6669 742e 7363  ..X&...lsqfit.sc
-00001270: 6970 795f 6c65 6173 745f 7371 7561 7265  ipy_least_square
-00001280: 732e 6465 7363 7269 7074 696f 6e71 ef68  s.descriptionq.h
-00001290: 5858 0900 0000 6174 7472 6962 7574 6571  XX....attributeq
-000012a0: f086 5818 0000 006c 7371 6669 742e 6e6f  ..X....lsqfit.no
-000012b0: 6e6c 696e 6561 725f 6669 742e 646f 6671  nlinear_fit.dofq
-000012c0: f168 2b58 0900 0000 6174 7472 6962 7574  .h+X....attribut
-000012d0: 6571 f286 580b 0000 006c 7371 6669 742e  eq..X....lsqfit.
-000012e0: 7761 7667 71f3 682b 5808 0000 0066 756e  wavgq.h+X....fun
-000012f0: 6374 696f 6e71 f486 580d 0000 006c 7371  ctionq..X....lsq
-00001300: 6669 742e 6761 6d6d 6151 71f5 682b 5808  fit.gammaQq.h+X.
-00001310: 0000 0066 756e 6374 696f 6e71 f686 5819  ...functionq..X.
-00001320: 0000 006c 7371 6669 742e 6e6f 6e6c 696e  ...lsqfit.nonlin
-00001330: 6561 725f 6669 742e 7376 646e 71f7 682b  ear_fit.svdnq.h+
-00001340: 5809 0000 0061 7474 7269 6275 7465 71f8  X....attributeq.
-00001350: 8658 1b00 0000 6c73 7166 6974 2e6e 6f6e  .X....lsqfit.non
-00001360: 6c69 6e65 6172 5f66 6974 2e6c 6f67 4742  linear_fit.logGB
-00001370: 4671 f968 2b58 0900 0000 6174 7472 6962  Fq.h+X....attrib
-00001380: 7574 6571 fa86 5826 0000 006c 7371 6669  uteq..X&...lsqfi
-00001390: 742e 4d75 6c74 6946 6974 7465 724d 6f64  t.MultiFitterMod
-000013a0: 656c 2e67 6574 5f70 7269 6f72 5f6b 6579  el.get_prior_key
-000013b0: 7371 fb68 2b58 0c00 0000 7374 6174 6963  sq.h+X....static
-000013c0: 6d65 7468 6f64 71fc 8658 1200 0000 6c73  methodq..X....ls
-000013d0: 7166 6974 2e4d 756c 7469 4669 7474 6572  qfit.MultiFitter
-000013e0: 71fd 682b 5805 0000 0063 6c61 7373 71fe  q.h+X....classq.
-000013f0: 8658 2700 0000 6c73 7166 6974 2e6e 6f6e  .X'...lsqfit.non
-00001400: 6c69 6e65 6172 5f66 6974 2e73 696d 756c  linear_fit.simul
-00001410: 6174 6564 5f66 6974 5f69 7465 7271 ff68  ated_fit_iterq.h
-00001420: 2b58 0600 0000 6d65 7468 6f64 7200 0100  +X....methodr...
-00001430: 0086 5817 0000 006c 7371 6669 742e 6e6f  ..X....lsqfit.no
-00001440: 6e6c 696e 6561 725f 6669 742e 7030 7201  nlinear_fit.p0r.
-00001450: 0100 0068 2b58 0900 0000 6174 7472 6962  ...h+X....attrib
-00001460: 7574 6572 0201 0000 8658 2a00 0000 6c73  uter.....X*...ls
-00001470: 7166 6974 2e6e 6f6e 6c69 6e65 6172 5f66  qfit.nonlinear_f
-00001480: 6974 2e62 6f6f 7473 7472 6170 7065 645f  it.bootstrapped_
-00001490: 6669 745f 6974 6572 7203 0100 0068 2b58  fit_iterr....h+X
-000014a0: 0600 0000 6d65 7468 6f64 7204 0100 0086  ....methodr.....
-000014b0: 581f 0000 006c 7371 6669 742e 4d75 6c74  X....lsqfit.Mult
-000014c0: 6946 6974 7465 722e 7072 6f63 6573 735f  iFitter.process_
-000014d0: 6461 7461 7205 0100 0068 2b58 0c00 0000  datar....h+X....
-000014e0: 7374 6174 6963 6d65 7468 6f64 7206 0100  staticmethodr...
-000014f0: 0086 581a 0000 006c 7371 6669 742e 6e6f  ..X....lsqfit.no
-00001500: 6e6c 696e 6561 725f 6669 742e 6572 726f  nlinear_fit.erro
-00001510: 7272 0701 0000 682b 5809 0000 0061 7474  rr....h+X....att
-00001520: 7269 6275 7465 7208 0100 0086 5816 0000  ributer.....X...
-00001530: 006c 7371 6669 742e 6e6f 6e6c 696e 6561  .lsqfit.nonlinea
-00001540: 725f 6669 742e 5172 0901 0000 682b 5809  r_fit.Qr....h+X.
-00001550: 0000 0061 7474 7269 6275 7465 720a 0100  ...attributer...
-00001560: 0086 5821 0000 006c 7371 6669 742e 4d75  ..X!...lsqfit.Mu
-00001570: 6c74 6946 6974 7465 724d 6f64 656c 2e70  ltiFitterModel.p
-00001580: 7269 6f72 5f6b 6579 720b 0100 0068 2b58  rior_keyr....h+X
-00001590: 0c00 0000 7374 6174 6963 6d65 7468 6f64  ....staticmethod
-000015a0: 720c 0100 0086 5817 0000 006c 7371 6669  r.....X....lsqfi
-000015b0: 742e 7363 6970 795f 6d75 6c74 696d 696e  t.scipy_multimin
-000015c0: 6578 720d 0100 0068 5858 0500 0000 636c  exr....hXX....cl
-000015d0: 6173 7372 0e01 0000 8658 1d00 0000 6c73  assr.....X....ls
-000015e0: 7166 6974 2e4d 756c 7469 4669 7474 6572  qfit.MultiFitter
-000015f0: 2e73 686f 775f 706c 6f74 7372 0f01 0000  .show_plotsr....
-00001600: 682b 580c 0000 0073 7461 7469 636d 6574  h+X....staticmet
-00001610: 686f 6472 1001 0000 8658 1e00 0000 6776  hodr.....X....gv
-00001620: 6172 2e61 6464 5f70 6172 616d 6574 6572  ar.add_parameter
-00001630: 5f70 6172 656e 7468 6573 6573 7211 0100  _parenthesesr...
-00001640: 0068 2b58 0800 0000 6675 6e63 7469 6f6e  .h+X....function
-00001650: 7212 0100 0086 581c 0000 006c 7371 6669  r.....X....lsqfi
-00001660: 742e 7363 6970 795f 6c65 6173 745f 7371  t.scipy_least_sq
-00001670: 7561 7265 732e 7872 1301 0000 6858 5809  uares.xr....hXX.
-00001680: 0000 0061 7474 7269 6275 7465 7214 0100  ...attributer...
-00001690: 0086 5818 0000 006c 7371 6669 742e 6e6f  ..X....lsqfit.no
-000016a0: 6e6c 696e 6561 725f 6669 742e 746f 6c72  nlinear_fit.tolr
-000016b0: 1501 0000 682b 5809 0000 0061 7474 7269  ....h+X....attri
-000016c0: 6275 7465 7216 0100 0086 581e 0000 006c  buter.....X....l
-000016d0: 7371 6669 742e 4d75 6c74 6946 6974 7465  sqfit.MultiFitte
-000016e0: 724d 6f64 656c 2e66 6974 6663 6e72 1701  rModel.fitfcnr..
-000016f0: 0000 682b 5806 0000 006d 6574 686f 6472  ..h+X....methodr
-00001700: 1801 0000 8658 1600 0000 6c73 7166 6974  .....X....lsqfit
-00001710: 2e67 736c 5f76 315f 6d75 6c74 6966 6974  .gsl_v1_multifit
-00001720: 7219 0100 0068 7158 0500 0000 636c 6173  r....hqX....clas
-00001730: 7386 5818 0000 006c 7371 6669 742e 6e6f  s.X....lsqfit.no
-00001740: 6e6c 696e 6561 725f 6669 742e 7365 7472  nlinear_fit.setr
-00001750: 1a01 0000 682b 580c 0000 0073 7461 7469  ....h+X....stati
-00001760: 636d 6574 686f 6472 1b01 0000 8658 1900  cmethodr.....X..
-00001770: 0000 6c73 7166 6974 2e73 6369 7079 5f6d  ..lsqfit.scipy_m
-00001780: 756c 7469 6d69 6e65 782e 7872 1c01 0000  ultiminex.xr....
-00001790: 6858 5809 0000 0061 7474 7269 6275 7465  hXX....attribute
-000017a0: 721d 0100 0086 5823 0000 006c 7371 6669  r.....X#...lsqfi
-000017b0: 742e 6e6f 6e6c 696e 6561 725f 6669 742e  t.nonlinear_fit.
-000017c0: 6669 7474 6572 5f72 6573 756c 7473 721e  fitter_resultsr.
-000017d0: 0100 0068 2b58 0900 0000 6174 7472 6962  ...h+X....attrib
-000017e0: 7574 6572 1f01 0000 8658 0f00 0000 6c73  uter.....X....ls
-000017f0: 7166 6974 2e42 6179 6573 5044 4672 2001  qfit.BayesPDFr .
-00001800: 0000 682b 5805 0000 0063 6c61 7373 7221  ..h+X....classr!
-00001810: 0100 0086 5821 0000 006c 7371 6669 742e  ....X!...lsqfit.
-00001820: 4d75 6c74 6946 6974 7465 724d 6f64 656c  MultiFitterModel
-00001830: 2e62 7569 6c64 6461 7461 7222 0100 0068  .builddatar"...h
-00001840: 2b58 0600 0000 6d65 7468 6f64 7223 0100  +X....methodr#..
-00001850: 0086 5818 0000 006c 7371 6669 742e 4261  ..X....lsqfit.Ba
-00001860: 7965 7350 4446 2e5f 5f63 616c 6c5f 5f72  yesPDF.__call__r
-00001870: 2401 0000 682b 5806 0000 006d 6574 686f  $...h+X....metho
-00001880: 6472 2501 0000 8658 1e00 0000 6c73 7166  dr%....X....lsqf
-00001890: 6974 2e73 6369 7079 5f6c 6561 7374 5f73  it.scipy_least_s
-000018a0: 7175 6172 6573 2e63 6f76 7226 0100 0068  quares.covr&...h
-000018b0: 5858 0900 0000 6174 7472 6962 7574 6572  XX....attributer
-000018c0: 2701 0000 8658 2100 0000 6c73 7166 6974  '....X!...lsqfit
-000018d0: 2e4d 756c 7469 4669 7474 6572 2e66 6c61  .MultiFitter.fla
-000018e0: 7474 656e 5f6d 6f64 656c 7372 2801 0000  tten_modelsr(...
-000018f0: 682b 580c 0000 0073 7461 7469 636d 6574  h+X....staticmet
-00001900: 686f 6472 2901 0000 8658 1600 0000 6c73  hodr)....X....ls
-00001910: 7166 6974 2e6e 6f6e 6c69 6e65 6172 5f66  qfit.nonlinear_f
-00001920: 6974 2e78 722a 0100 0068 2b58 0900 0000  it.xr*...h+X....
-00001930: 6174 7472 6962 7574 6572 2b01 0000 8658  attributer+....X
-00001940: 1300 0000 6c73 7166 6974 2e65 6d70 6261  ....lsqfit.empba
-00001950: 7965 735f 6669 7472 2c01 0000 682b 5808  yes_fitr,...h+X.
-00001960: 0000 0066 756e 6374 696f 6e72 2d01 0000  ...functionr-...
-00001970: 8658 1b00 0000 6c73 7166 6974 2e4d 756c  .X....lsqfit.Mul
-00001980: 7469 4669 7474 6572 4d6f 6465 6c2e 6e63  tiFitterModel.nc
-00001990: 6772 2e01 0000 682b 5809 0000 0061 7474  gr....h+X....att
-000019a0: 7269 6275 7465 722f 0100 0086 5821 0000  ributer/....X!..
-000019b0: 006c 7371 6669 742e 4d75 6c74 6946 6974  .lsqfit.MultiFit
-000019c0: 7465 722e 6368 6169 6e65 645f 6c73 7166  ter.chained_lsqf
-000019d0: 6974 7230 0100 0068 2b58 0600 0000 6d65  itr0...h+X....me
-000019e0: 7468 6f64 7231 0100 0086 5816 0000 006c  thodr1....X....l
-000019f0: 7371 6669 742e 6e6f 6e6c 696e 6561 725f  sqfit.nonlinear_
-00001a00: 6669 742e 7072 3201 0000 682b 5809 0000  fit.pr2...h+X...
-00001a10: 0061 7474 7269 6275 7465 7233 0100 0086  .attributer3....
-00001a20: 581c 0000 006c 7371 6669 742e 6e6f 6e6c  X....lsqfit.nonl
-00001a30: 696e 6561 725f 6669 742e 6e62 6c6f 636b  inear_fit.nblock
-00001a40: 7372 3401 0000 682b 5809 0000 0061 7474  sr4...h+X....att
-00001a50: 7269 6275 7465 7235 0100 0086 581f 0000  ributer5....X...
-00001a60: 006c 7371 6669 742e 4d75 6c74 6946 6974  .lsqfit.MultiFit
-00001a70: 7465 724d 6f64 656c 2e64 6174 6174 6167  terModel.datatag
-00001a80: 7236 0100 0068 2b58 0900 0000 6174 7472  r6...h+X....attr
-00001a90: 6962 7574 6572 3701 0000 8658 1900 0000  ibuter7....X....
-00001aa0: 6c73 7166 6974 2e73 6369 7079 5f6d 756c  lsqfit.scipy_mul
-00001ab0: 7469 6d69 6e65 782e 6672 3801 0000 6858  timinex.fr8...hX
-00001ac0: 5809 0000 0061 7474 7269 6275 7465 7239  X....attributer9
-00001ad0: 0100 0086 5816 0000 006c 7371 6669 742e  ....X....lsqfit.
-00001ae0: 6e6f 6e6c 696e 6561 725f 6669 742e 7972  nonlinear_fit.yr
-00001af0: 3a01 0000 682b 5809 0000 0061 7474 7269  :...h+X....attri
-00001b00: 6275 7465 723b 0100 0086 581a 0000 006c  buter;....X....l
-00001b10: 7371 6669 742e 6e6f 6e6c 696e 6561 725f  sqfit.nonlinear_
-00001b20: 6669 742e 7073 6465 7672 3c01 0000 682b  fit.psdevr<...h+
-00001b30: 5809 0000 0061 7474 7269 6275 7465 723d  X....attributer=
-00001b40: 0100 0086 581f 0000 0067 7661 722e 6164  ....X....gvar.ad
-00001b50: 645f 7061 7261 6d65 7465 725f 6469 7374  d_parameter_dist
-00001b60: 7269 6275 7469 6f6e 723e 0100 0068 2b58  ributionr>...h+X
-00001b70: 0800 0000 6675 6e63 7469 6f6e 723f 0100  ....functionr?..
-00001b80: 0086 7555 076d 6f64 756c 6573 7240 0100  ..uU.modulesr@..
-00001b90: 007d 7241 0100 0068 af28 682b 6364 6f63  .}rA...h.(h+cdoc
-00001ba0: 7574 696c 732e 6e6f 6465 730a 7265 7072  utils.nodes.repr
-00001bb0: 756e 6963 6f64 650a 7242 0100 0058 2000  unicode.rB...X .
-00001bc0: 0000 4e6f 6e6c 696e 6561 7220 6c65 6173  ..Nonlinear leas
-00001bd0: 7420 7371 7561 7265 7320 6669 7474 696e  t squares fittin
-00001be0: 672e 7243 0100 0085 8172 4401 0000 7d72  g.rC.....rD...}r
-00001bf0: 4501 0000 6255 0089 7473 6892 4b00 7555  E...bU..tsh.K.uU
-00001c00: 026a 7372 4601 0000 7d72 4701 0000 2868  .jsrF...}rG...(h
-00001c10: a27d 6a40 0100 007d 6892 4b00 7555 0363  .}j@...}h.K.uU.c
-00001c20: 7070 7248 0100 007d 7249 0100 0028 550b  pprH...}rI...(U.
-00001c30: 726f 6f74 5f73 796d 626f 6c72 4a01 0000  root_symbolrJ...
-00001c40: 6373 7068 696e 782e 646f 6d61 696e 732e  csphinx.domains.
-00001c50: 6370 700a 5379 6d62 6f6c 0a72 4b01 0000  cpp.Symbol.rK...
-00001c60: 2981 724c 0100 007d 724d 0100 0028 550f  ).rL...}rM...(U.
-00001c70: 6973 5265 6465 636c 6172 6174 696f 6e72  isRedeclarationr
-00001c80: 4e01 0000 8955 0e74 656d 706c 6174 6550  N....U.templateP
-00001c90: 6172 616d 7372 4f01 0000 4e68 1f4e 550c  aramsrO...Nh.NU.
-00001ca0: 7465 6d70 6c61 7465 4172 6773 7250 0100  templateArgsrP..
-00001cb0: 004e 550b 6465 636c 6172 6174 696f 6e72  .NU.declarationr
-00001cc0: 5101 0000 4e55 0764 6f63 6e61 6d65 7252  Q...NU.docnamerR
-00001cd0: 0100 004e 5509 6964 656e 744f 724f 7072  ...NU.identOrOpr
-00001ce0: 5301 0000 4e68 185d 7562 6892 4b00 6817  S...Nh.]ubh.K.h.
-00001cf0: 7d75 5503 7273 7472 5401 0000 7d72 5501  }uU.rstrT...}rU.
-00001d00: 0000 2868 a27d 6892 4b00 7555 046d 6174  ..(h.}h.K.uU.mat
-00001d10: 6872 5601 0000 7d72 5701 0000 2868 a27d  hrV...}rW...(h.}
-00001d20: 6892 4b00 7575 550d 676c 6f62 5f74 6f63  h.K.uuU.glob_toc
-00001d30: 7472 6565 7372 5801 0000 6807 5d85 5272  treesrX...h.].Rr
-00001d40: 5901 0000 550d 7265 7265 6164 5f61 6c77  Y...U.reread_alw
-00001d50: 6179 7372 5a01 0000 6807 5d85 5272 5b01  aysrZ...h.].Rr[.
-00001d60: 0000 550a 646f 6374 7265 6564 6972 725c  ..U.doctreedirr\
-00001d70: 0100 0058 3400 0000 2f55 7365 7273 2f67  ...X4.../Users/g
-00001d80: 706c 2f73 6f66 7477 6172 652f 7079 7468  pl/software/pyth
-00001d90: 6f6e 2f6c 7371 6669 742f 646f 632f 6874  on/lsqfit/doc/ht
-00001da0: 6d6c 2f2e 646f 6374 7265 6573 725d 0100  ml/.doctreesr]..
-00001db0: 0055 1476 6572 7369 6f6e 696e 675f 636f  .U.versioning_co
-00001dc0: 6e64 6974 696f 6e72 5e01 0000 8955 0e74  nditionr^....U.t
-00001dd0: 6f63 5f66 6967 6e75 6d62 6572 7372 5f01  oc_fignumbersr_.
-00001de0: 0000 7d55 0974 656d 705f 6461 7461 7260  ..}U.temp_datar`
-00001df0: 0100 007d 5512 6f72 6967 696e 616c 5f69  ...}U.original_i
-00001e00: 6d61 6765 5f75 7269 7261 0100 007d 6892  mage_urira...}h.
-00001e10: 4b34 5506 7372 6364 6972 7262 0100 0058  K4U.srcdirrb...X
-00001e20: 2c00 0000 2f55 7365 7273 2f67 706c 2f73  ,.../Users/gpl/s
-00001e30: 6f66 7477 6172 652f 7079 7468 6f6e 2f6c  oftware/python/l
-00001e40: 7371 6669 742f 646f 632f 736f 7572 6365  sqfit/doc/source
-00001e50: 7263 0100 0055 0663 6f6e 6669 6772 6401  rc...U.configrd.
-00001e60: 0000 6373 7068 696e 782e 636f 6e66 6967  ..csphinx.config
-00001e70: 0a43 6f6e 6669 670a 7265 0100 0029 8172  .Config.re...).r
-00001e80: 6601 0000 7d72 6701 0000 2855 216e 6170  f...}rg...(U!nap
-00001e90: 6f6c 656f 6e5f 696e 636c 7564 655f 7072  oleon_include_pr
-00001ea0: 6976 6174 655f 7769 7468 5f64 6f63 7268  ivate_with_docrh
-00001eb0: 0100 0089 5521 6e61 706f 6c65 6f6e 5f69  ....U!napoleon_i
-00001ec0: 6e63 6c75 6465 5f73 7065 6369 616c 5f77  nclude_special_w
-00001ed0: 6974 685f 646f 6372 6901 0000 8855 186e  ith_docri....U.n
-00001ee0: 6170 6f6c 656f 6e5f 6e75 6d70 795f 646f  apoleon_numpy_do
-00001ef0: 6373 7472 696e 6772 6a01 0000 8855 0e70  cstringrj....U.p
-00001f00: 7967 6d65 6e74 735f 7374 796c 6572 6b01  ygments_stylerk.
-00001f10: 0000 5506 7370 6869 6e78 726c 0100 0055  ..U.sphinxrl...U
-00001f20: 266e 6170 6f6c 656f 6e5f 7573 655f 6164  &napoleon_use_ad
-00001f30: 6d6f 6e69 7469 6f6e 5f66 6f72 5f72 6566  monition_for_ref
-00001f40: 6572 656e 6365 7372 6d01 0000 8955 1369  erencesrm....U.i
-00001f50: 6d67 6d61 7468 5f64 7669 706e 675f 6172  mgmath_dvipng_ar
-00001f60: 6773 726e 0100 005d 726f 0100 0028 5506  gsrn...]ro...(U.
-00001f70: 2d67 616d 6d61 7270 0100 0055 0430 2e33  -gammarp...U.0.3
-00001f80: 3572 7101 0000 5502 2d44 7272 0100 0055  5rq...U.-Drr...U
-00001f90: 0331 3130 7273 0100 0055 032d 6267 7274  .110rs...U.-bgrt
-00001fa0: 0100 0055 0b54 7261 6e73 7061 7265 6e74  ...U.Transparent
-00001fb0: 7275 0100 0065 5516 696d 676d 6174 685f  ru...eU.imgmath_
-00001fc0: 6c61 7465 785f 7072 6561 6d62 6c65 7276  latex_preamblerv
-00001fd0: 0100 0055 115c 7573 6570 6163 6b61 6765  ...U.\usepackage
-00001fe0: 7b61 7265 767d 5524 6e61 706f 6c65 6f6e  {arev}U$napoleon
-00001ff0: 5f75 7365 5f61 646d 6f6e 6974 696f 6e5f  _use_admonition_
-00002000: 666f 725f 6578 616d 706c 6573 7277 0100  for_examplesrw..
-00002010: 0089 550a 6d61 7374 6572 5f64 6f63 7278  ..U.master_docrx
-00002020: 0100 0055 0569 6e64 6578 7279 0100 0055  ...U.indexry...U
-00002030: 126e 6170 6f6c 656f 6e5f 7573 655f 7274  .napoleon_use_rt
-00002040: 7970 6572 7a01 0000 8855 0d73 6f75 7263  yperz....U.sourc
-00002050: 655f 7375 6666 6978 727b 0100 005d 727c  e_suffixr{...]r|
-00002060: 0100 0055 042e 7273 7472 7d01 0000 6155  ...U..rstr}...aU
-00002070: 0963 6f70 7972 6967 6874 727e 0100 0058  .copyrightr~...X
-00002080: 1700 0000 3230 3039 2d32 3031 382c 2047  ....2009-2018, G
-00002090: 2e20 502e 204c 6570 6167 6568 9255 0339  . P. Lepageh.U.9
-000020a0: 2e34 727f 0100 0055 1469 6d67 6d61 7468  .4r....U.imgmath
-000020b0: 5f69 6d61 6765 5f66 6f72 6d61 7472 8001  _image_formatr..
-000020c0: 0000 5503 706e 6772 8101 0000 550a 6874  ..U.pngr....U.ht
-000020d0: 6d6c 5f74 6865 6d65 7282 0100 0055 0770  ml_themer....U.p
-000020e0: 7972 616d 6964 7283 0100 0055 196e 6170  yramidr....U.nap
-000020f0: 6f6c 656f 6e5f 676f 6f67 6c65 5f64 6f63  oleon_google_doc
-00002100: 7374 7269 6e67 7284 0100 0088 5512 6e61  stringr.....U.na
-00002110: 706f 6c65 6f6e 5f75 7365 5f70 6172 616d  poleon_use_param
-00002120: 7285 0100 0088 550e 7465 6d70 6c61 7465  r.....U.template
-00002130: 735f 7061 7468 7286 0100 005d 7287 0100  s_pathr....]r...
-00002140: 0055 0a5f 7465 6d70 6c61 7465 7372 8801  .U._templatesr..
-00002150: 0000 6155 0f6c 6174 6578 5f64 6f63 756d  ..aU.latex_docum
-00002160: 656e 7473 7289 0100 005d 728a 0100 0028  entsr....]r....(
-00002170: 6a79 0100 0055 0a6c 7371 6669 742e 7465  jy...U.lsqfit.te
-00002180: 7858 1400 0000 6c73 7166 6974 2044 6f63  xX....lsqfit Doc
-00002190: 756d 656e 7461 7469 6f6e 580c 0000 0047  umentationX....G
-000021a0: 2e20 502e 204c 6570 6167 6555 066d 616e  . P. LepageU.man
-000021b0: 7561 6c72 8b01 0000 7472 8c01 0000 6155  ualr....tr....aU
-000021c0: 116e 6170 6f6c 656f 6e5f 7573 655f 6976  .napoleon_use_iv
-000021d0: 6172 728d 0100 0089 5510 6874 6d6c 5f73  arr.....U.html_s
-000021e0: 7461 7469 635f 7061 7468 728e 0100 005d  tatic_pathr....]
-000021f0: 728f 0100 0055 075f 7374 6174 6963 7290  r....U._staticr.
-00002200: 0100 0061 5509 6f76 6572 7269 6465 7372  ...aU.overridesr
-00002210: 9101 0000 7d55 1168 746d 6c68 656c 705f  ....}U.htmlhelp_
-00002220: 6261 7365 6e61 6d65 7292 0100 0055 096c  basenamer....U.l
-00002230: 7371 6669 7464 6f63 5513 696d 676d 6174  sqfitdocU.imgmat
-00002240: 685f 7573 655f 7072 6576 6965 7772 9301  h_use_previewr..
-00002250: 0000 8855 0770 726f 6a65 6374 7294 0100  ...U.projectr...
-00002260: 0058 0600 0000 6c73 7166 6974 550a 6578  .X....lsqfitU.ex
-00002270: 7465 6e73 696f 6e73 7295 0100 005d 7296  tensionsr....]r.
-00002280: 0100 0028 5512 7370 6869 6e78 2e65 7874  ...(U.sphinx.ext
-00002290: 2e61 7574 6f64 6f63 7297 0100 0055 1373  .autodocr....U.s
-000022a0: 7068 696e 782e 6578 742e 6e61 706f 6c65  phinx.ext.napole
-000022b0: 6f6e 7298 0100 0055 1273 7068 696e 782e  onr....U.sphinx.
-000022c0: 6578 742e 696d 676d 6174 6872 9901 0000  ext.imgmathr....
-000022d0: 6555 0772 656c 6561 7365 729a 0100 006a  eU.releaser....j
-000022e0: 7f01 0000 5521 6e61 706f 6c65 6f6e 5f75  ....U!napoleon_u
-000022f0: 7365 5f61 646d 6f6e 6974 696f 6e5f 666f  se_admonition_fo
-00002300: 725f 6e6f 7465 7372 9b01 0000 8955 0573  r_notesr.....U.s
-00002310: 6574 7570 729c 0100 004e 7562 5508 6d65  etupr....NubU.me
-00002320: 7461 6461 7461 729d 0100 0063 636f 6c6c  tadatar....ccoll
-00002330: 6563 7469 6f6e 730a 6465 6661 756c 7464  ections.defaultd
-00002340: 6963 740a 729e 0100 0063 5f5f 6275 696c  ict.r....c__buil
-00002350: 7469 6e5f 5f0a 6469 6374 0a72 9f01 0000  tin__.dict.r....
-00002360: 8552 72a0 0100 0028 680c 7d72 a101 0000  .Rr....(h.}r....
-00002370: 6822 7d72 a201 0000 682b 7d72 a301 0000  h"}r....h+}r....
-00002380: 683d 7d72 a401 0000 6846 7d72 a501 0000  h=}r....hF}r....
-00002390: 684f 7d72 a601 0000 6858 7d72 a701 0000  hO}r....hX}r....
-000023a0: 6868 7d72 a801 0000 6871 7d72 a901 0000  hh}r....hq}r....
-000023b0: 7555 0e76 6572 7369 6f6e 6368 616e 6765  uU.versionchange
-000023c0: 7372 aa01 0000 7d55 0f74 6f63 5f6e 756d  sr....}U.toc_num
-000023d0: 5f65 6e74 7269 6573 72ab 0100 007d 72ac  _entriesr....}r.
-000023e0: 0100 0028 680c 4b02 6822 4b05 682b 4b07  ...(h.K.h"K.h+K.
-000023f0: 683d 4b0e 6846 4b06 684f 4b04 6858 4b03  h=K.hFK.hOK.hXK.
-00002400: 6868 4b04 6871 4b03 7555 0669 6d61 6765  hhK.hqK.uU.image
-00002410: 7372 ad01 0000 6805 2981 72ae 0100 0028  sr....h.).r....(
-00002420: 5811 0000 0065 672d 6170 7065 6e64 6978  X....eg-appendix
-00002430: 3163 2e70 6e67 72af 0100 0068 075d 72b0  1c.pngr....h.]r.
-00002440: 0100 0068 4661 8552 72b1 0100 006a af01  ...hFa.Rr....j..
-00002450: 0000 8672 b201 0000 5811 0000 0065 672d  ...r....X....eg-
-00002460: 6170 7065 6e64 6978 3162 2e70 6e67 72b3  appendix1b.pngr.
-00002470: 0100 0068 075d 72b4 0100 0068 4661 8552  ...h.]r....hFa.R
-00002480: 72b5 0100 006a b301 0000 8672 b601 0000  r....j.....r....
-00002490: 5811 0000 0065 672d 6170 7065 6e64 6978  X....eg-appendix
-000024a0: 3161 2e70 6e67 72b7 0100 0068 075d 72b8  1a.pngr....h.]r.
-000024b0: 0100 0068 4661 8552 72b9 0100 006a b701  ...hFa.Rr....j..
-000024c0: 0000 8672 ba01 0000 5808 0000 0065 6733  ...r....X....eg3
-000024d0: 642e 706e 6772 bb01 0000 6807 5d72 bc01  d.pngr....h.]r..
-000024e0: 0000 6822 6185 5272 bd01 0000 6abb 0100  ..h"a.Rr....j...
-000024f0: 0086 72be 0100 0058 1100 0000 6567 2d61  ..r....X....eg-a
-00002500: 7070 656e 6469 7831 642e 706e 6772 bf01  ppendix1d.pngr..
-00002510: 0000 6807 5d72 c001 0000 6846 6185 5272  ..h.]r....hFa.Rr
-00002520: c101 0000 6abf 0100 0086 72c2 0100 0058  ....j.....r....X
-00002530: 0800 0000 6567 3365 2e70 6e67 72c3 0100  ....eg3e.pngr...
-00002540: 0068 075d 72c4 0100 0068 2261 8552 72c5  .h.]r....h"a.Rr.
-00002550: 0100 006a c301 0000 8672 c601 0000 5807  ...j.....r....X.
-00002560: 0000 0065 6731 2e70 6e67 72c7 0100 0068  ...eg1.pngr....h
-00002570: 075d 72c8 0100 0068 3d61 8552 72c9 0100  .]r....h=a.Rr...
-00002580: 006a c701 0000 8672 ca01 0000 5807 0000  .j.....r....X...
-00002590: 0065 6732 2e70 6e67 72cb 0100 0068 075d  .eg2.pngr....h.]
-000025a0: 72cc 0100 0068 3d61 8552 72cd 0100 006a  r....h=a.Rr....j
-000025b0: cb01 0000 8672 ce01 0000 5807 0000 0065  .....r....X....e
-000025c0: 6733 2e70 6e67 72cf 0100 0068 075d 72d0  g3.pngr....h.]r.
-000025d0: 0100 0068 3d61 8552 72d1 0100 006a cf01  ...h=a.Rr....j..
-000025e0: 0000 8672 d201 0000 5812 0000 0063 6173  ...r....X....cas
-000025f0: 652d 6f75 746c 6965 7273 312e 706e 6772  e-outliers1.pngr
-00002600: d301 0000 6807 5d72 d401 0000 684f 6185  ....h.]r....hOa.
-00002610: 5272 d501 0000 6ad3 0100 0086 72d6 0100  Rr....j.....r...
-00002620: 0058 1000 0000 6361 7365 2d70 656e 6475  .X....case-pendu
-00002630: 6c75 6d2e 7079 72d7 0100 0068 075d 72d8  lum.pyr....h.]r.
-00002640: 0100 0068 6861 8552 72d9 0100 006a d701  ...hha.Rr....j..
-00002650: 0000 8672 da01 0000 5811 0000 0063 6173  ...r....X....cas
-00002660: 652d 7065 6e64 756c 756d 2e70 6e67 72db  e-pendulum.pngr.
-00002670: 0100 0068 075d 72dc 0100 0068 6861 8552  ...h.]r....hha.R
-00002680: 72dd 0100 006a db01 0000 8672 de01 0000  r....j.....r....
-00002690: 5811 0000 0065 672d 6170 7065 6e64 6978  X....eg-appendix
-000026a0: 3164 2e6f 7574 72df 0100 0068 075d 72e0  1d.outr....h.]r.
-000026b0: 0100 0068 4661 8552 72e1 0100 006a df01  ...hFa.Rr....j..
-000026c0: 0000 8672 e201 0000 5807 0000 0065 6736  ...r....X....eg6
-000026d0: 2e70 6e67 72e3 0100 0068 075d 72e4 0100  .pngr....h.]r...
-000026e0: 0068 2261 8552 72e5 0100 006a e301 0000  .h"a.Rr....j....
-000026f0: 8672 e601 0000 5811 0000 0065 672d 6170  .r....X....eg-ap
-00002700: 7065 6e64 6978 3162 2e6f 7574 72e7 0100  pendix1b.outr...
-00002710: 0068 075d 72e8 0100 0068 4661 8552 72e9  .h.]r....hFa.Rr.
-00002720: 0100 006a e701 0000 8672 ea01 0000 5811  ...j.....r....X.
-00002730: 0000 0065 672d 6170 7065 6e64 6978 3163  ...eg-appendix1c
-00002740: 2e6f 7574 72eb 0100 0068 075d 72ec 0100  .outr....h.]r...
-00002750: 0068 4661 8552 72ed 0100 006a eb01 0000  .hFa.Rr....j....
-00002760: 8672 ee01 0000 5807 0000 0065 6735 2e70  .r....X....eg5.p
-00002770: 6e67 72ef 0100 0068 075d 72f0 0100 0068  ngr....h.]r....h
-00002780: 3d61 8552 72f1 0100 006a ef01 0000 8672  =a.Rr....j.....r
-00002790: f201 0000 5812 0000 0063 6173 652d 6f75  ....X....case-ou
-000027a0: 746c 6965 7273 322e 706e 6772 f301 0000  tliers2.pngr....
-000027b0: 6807 5d72 f401 0000 684f 6185 5272 f501  h.]r....hOa.Rr..
-000027c0: 0000 6af3 0100 0086 72f6 0100 0058 1100  ..j.....r....X..
-000027d0: 0000 6567 2d61 7070 656e 6469 7831 612e  ..eg-appendix1a.
-000027e0: 6f75 7472 f701 0000 6807 5d72 f801 0000  outr....h.]r....
-000027f0: 6846 6185 5272 f901 0000 6af7 0100 0086  hFa.Rr....j.....
-00002800: 72fa 0100 0075 6807 5d72 fb01 0000 286a  r....uh.]r....(j
-00002810: af01 0000 6ab3 0100 006a b701 0000 6abb  ....j....j....j.
-00002820: 0100 006a bf01 0000 6ac3 0100 006a c701  ...j....j....j..
-00002830: 0000 6acb 0100 006a cf01 0000 6ad3 0100  ..j....j....j...
-00002840: 006a d701 0000 6adb 0100 006a df01 0000  .j....j....j....
-00002850: 6ae3 0100 006a e701 0000 6aeb 0100 006a  j....j....j....j
-00002860: ef01 0000 6af3 0100 006a f701 0000 6585  ....j....j....e.
-00002870: 5272 fc01 0000 6255 116e 756d 6265 7265  Rr....bU.numbere
-00002880: 645f 746f 6374 7265 6573 72fd 0100 0068  d_toctreesr....h
-00002890: 075d 8552 72fe 0100 0055 0a66 6f75 6e64  .].Rr....U.found
-000028a0: 5f64 6f63 7372 ff01 0000 6807 5d72 0002  _docsr....h.]r..
-000028b0: 0000 2868 0c68 2b68 3d68 2268 4f68 5868  ..(h.h+h=h"hOhXh
-000028c0: 6868 4668 7165 8552 7201 0200 0055 0a6c  hhFhqe.Rr....U.l
-000028d0: 6f6e 6774 6974 6c65 7372 0202 0000 7d72  ongtitlesr....}r
-000028e0: 0302 0000 2868 0c68 0e68 2268 2368 2b68  ....(h.h.h"h#h+h
-000028f0: 2c68 3d68 3e68 4668 4768 4f68 5068 5868  ,h=h>hFhGhOhPhXh
-00002900: 5968 6868 6968 7168 7275 550c 6465 7065  YhhhihqhruU.depe
-00002910: 6e64 656e 6369 6573 7204 0200 006a 9e01  ndenciesr....j..
-00002920: 0000 6807 8552 7205 0200 0028 6822 6807  ..h..Rr....(h"h.
-00002930: 5d72 0602 0000 286a bb01 0000 6ac3 0100  ]r....(j....j...
-00002940: 0058 0800 0000 6567 3363 2e6f 7574 7207  .X....eg3c.outr.
-00002950: 0200 0058 0c00 0000 6567 362d 6869 7374  ...X....eg6-hist
-00002960: 2e6f 7574 7208 0200 006a e301 0000 5808  .outr....j....X.
-00002970: 0000 0065 6733 642e 6f75 7472 0902 0000  ...eg3d.outr....
-00002980: 5808 0000 0065 6733 662e 6f75 7472 0a02  X....eg3f.outr..
-00002990: 0000 5808 0000 0065 6733 652e 6f75 7472  ..X....eg3e.outr
-000029a0: 0b02 0000 6585 5272 0c02 0000 682b 6807  ....e.Rr....h+h.
-000029b0: 5d72 0d02 0000 2858 4600 0000 2e2e 2f2e  ]r....(XF...../.
-000029c0: 2e2f 2e2e 2f2e 2e2f 2e2e 2f61 6e61 636f  ./../../../anaco
-000029d0: 6e64 6132 2f6c 6962 2f70 7974 686f 6e32  nda2/lib/python2
-000029e0: 2e37 2f73 6974 652d 7061 636b 6167 6573  .7/site-packages
-000029f0: 2f67 7661 722f 5f5f 696e 6974 5f5f 2e70  /gvar/__init__.p
-00002a00: 7963 720e 0200 0058 4700 0000 2e2e 2f2e  ycr....XG...../.
-00002a10: 2e2f 2e2e 2f2e 2e2f 2e2e 2f61 6e61 636f  ./../../../anaco
-00002a20: 6e64 6132 2f6c 6962 2f70 7974 686f 6e32  nda2/lib/python2
-00002a30: 2e37 2f73 6974 652d 7061 636b 6167 6573  .7/site-packages
-00002a40: 2f6c 7371 6669 742f 5f5f 696e 6974 5f5f  /lsqfit/__init__
-00002a50: 2e70 7972 0f02 0000 5846 0000 002e 2e2f  .pyr....XF...../
-00002a60: 2e2e 2f2e 2e2f 2e2e 2f2e 2e2f 616e 6163  ../../../../anac
-00002a70: 6f6e 6461 322f 6c69 622f 7079 7468 6f6e  onda2/lib/python
-00002a80: 322e 372f 7369 7465 2d70 6163 6b61 6765  2.7/site-package
-00002a90: 732f 6c73 7166 6974 2f5f 6578 7472 6173  s/lsqfit/_extras
-00002aa0: 2e70 7972 1002 0000 5845 0000 002e 2e2f  .pyr....XE...../
-00002ab0: 2e2e 2f2e 2e2f 2e2e 2f2e 2e2f 616e 6163  ../../../../anac
-00002ac0: 6f6e 6461 322f 6c69 622f 7079 7468 6f6e  onda2/lib/python
-00002ad0: 322e 372f 7369 7465 2d70 6163 6b61 6765  2.7/site-package
-00002ae0: 732f 6776 6172 2f5f 5f69 6e69 745f 5f2e  s/gvar/__init__.
-00002af0: 7079 7211 0200 0058 4800 0000 2e2e 2f2e  pyr....XH...../.
-00002b00: 2e2f 2e2e 2f2e 2e2f 2e2e 2f61 6e61 636f  ./../../../anaco
-00002b10: 6e64 6132 2f6c 6962 2f70 7974 686f 6e32  nda2/lib/python2
-00002b20: 2e37 2f73 6974 652d 7061 636b 6167 6573  .7/site-packages
-00002b30: 2f6c 7371 6669 742f 5f5f 696e 6974 5f5f  /lsqfit/__init__
-00002b40: 2e70 7963 7212 0200 0065 8552 7213 0200  .pycr....e.Rr...
-00002b50: 0068 3d68 075d 7214 0200 0028 580d 0000  .h=h.]r....(X...
-00002b60: 0065 6736 2d6c 6f67 5f61 2e6f 7574 7215  .eg6-log_a.outr.
-00002b70: 0200 0058 0800 0000 6567 3462 2e6f 7574  ...X....eg4b.out
-00002b80: 7216 0200 0058 0800 0000 6567 3162 2e6f  r....X....eg1b.o
-00002b90: 7574 7217 0200 006a ef01 0000 5807 0000  utr....j....X...
-00002ba0: 0065 6730 2e6f 7574 7218 0200 0058 0900  .eg0.outr....X..
-00002bb0: 0000 6567 362d 612e 6f75 7472 1902 0000  ..eg6-a.outr....
-00002bc0: 5808 0000 0065 6737 622e 6f75 7472 1a02  X....eg7b.outr..
-00002bd0: 0000 6acb 0100 0058 0700 0000 6567 322e  ..j....X....eg2.
-00002be0: 6f75 7472 1b02 0000 5808 0000 0065 6739  outr....X....eg9
-00002bf0: 612e 6f75 7472 1c02 0000 5808 0000 0065  a.outr....X....e
-00002c00: 6733 622e 6f75 7472 1d02 0000 5808 0000  g3b.outr....X...
-00002c10: 0065 6737 612e 6f75 7472 1e02 0000 5808  .eg7a.outr....X.
-00002c20: 0000 0065 6735 622e 6f75 7472 1f02 0000  ...eg5b.outr....
-00002c30: 5808 0000 0065 6735 612e 6f75 7472 2002  X....eg5a.outr .
-00002c40: 0000 6acf 0100 0058 0800 0000 6567 3361  ..j....X....eg3a
-00002c50: 2e6f 7574 7221 0200 0058 0800 0000 6567  .outr!...X....eg
-00002c60: 3161 2e6f 7574 7222 0200 0058 0e00 0000  1a.outr"...X....
-00002c70: 6567 362d 6572 6669 6e76 2e6f 7574 7223  eg6-erfinv.outr#
-00002c80: 0200 006a c701 0000 5808 0000 0065 6734  ...j....X....eg4
-00002c90: 612e 6f75 7472 2402 0000 5807 0000 0065  a.outr$...X....e
-00002ca0: 6731 2e6f 7574 7225 0200 0065 8552 7226  g1.outr%...e.Rr&
-00002cb0: 0200 0068 4668 075d 7227 0200 0028 6aaf  ...hFh.]r'...(j.
-00002cc0: 0100 006a b301 0000 6ab7 0100 0058 1100  ...j....j....X..
-00002cd0: 0000 6567 2d61 7070 656e 6469 7831 672e  ..eg-appendix1g.
-00002ce0: 6f75 7472 2802 0000 6abf 0100 0058 1100  outr(...j....X..
-00002cf0: 0000 6567 2d61 7070 656e 6469 7831 642e  ..eg-appendix1d.
-00002d00: 6f75 7472 2902 0000 5811 0000 0065 672d  outr)...X....eg-
-00002d10: 6170 7065 6e64 6978 3162 2e6f 7574 722a  appendix1b.outr*
-00002d20: 0200 0058 1100 0000 6567 2d61 7070 656e  ...X....eg-appen
-00002d30: 6469 7831 632e 6f75 7472 2b02 0000 5811  dix1c.outr+...X.
-00002d40: 0000 0065 672d 6170 7065 6e64 6978 3165  ...eg-appendix1e
-00002d50: 2e6f 7574 722c 0200 0058 1100 0000 6567  .outr,...X....eg
-00002d60: 2d61 7070 656e 6469 7831 612e 6f75 7472  -appendix1a.outr
-00002d70: 2d02 0000 6585 5272 2e02 0000 684f 6807  -...e.Rr....hOh.
-00002d80: 5d72 2f02 0000 286a d301 0000 5815 0000  ]r/...(j....X...
-00002d90: 0063 6173 652d 6f75 746c 6965 7273 2d6c  .case-outliers-l
-00002da0: 7371 2e6f 7574 7230 0200 0058 1700 0000  sq.outr0...X....
-00002db0: 6361 7365 2d6f 7574 6c69 6572 732d 6d75  case-outliers-mu
-00002dc0: 6c74 692e 6f75 7472 3102 0000 5811 0000  lti.outr1...X...
-00002dd0: 0063 6173 652d 6f75 746c 6965 7273 2e6f  .case-outliers.o
-00002de0: 7574 7232 0200 006a f301 0000 6585 5272  utr2...j....e.Rr
-00002df0: 3302 0000 6858 6807 5d72 3402 0000 5845  3...hXh.]r4...XE
-00002e00: 0000 002e 2e2f 2e2e 2f2e 2e2f 2e2e 2f2e  ...../../../../.
-00002e10: 2e2f 616e 6163 6f6e 6461 322f 6c69 622f  ./anaconda2/lib/
-00002e20: 7079 7468 6f6e 322e 372f 7369 7465 2d70  python2.7/site-p
-00002e30: 6163 6b61 6765 732f 6c73 7166 6974 2f5f  ackages/lsqfit/_
-00002e40: 7363 6970 792e 7079 7235 0200 0061 8552  scipy.pyr5...a.R
-00002e50: 7236 0200 0068 6868 075d 7237 0200 0028  r6...hhh.]r7...(
-00002e60: 5811 0000 0063 6173 652d 7065 6e64 756c  X....case-pendul
-00002e70: 756d 2e6f 7574 7238 0200 006a db01 0000  um.outr8...j....
-00002e80: 6ad7 0100 0065 8552 7239 0200 0075 5510  j....e.Rr9...uU.
-00002e90: 746f 6374 7265 655f 696e 636c 7564 6573  toctree_includes
-00002ea0: 723a 0200 007d 723b 0200 0068 0c5d 723c  r:...}r;...h.]r<
-00002eb0: 0200 0028 5808 0000 006f 7665 7276 6965  ...(X....overvie
-00002ec0: 7772 3d02 0000 5807 0000 0074 6573 7469  wr=...X....testi
-00002ed0: 6e67 723e 0200 0058 1200 0000 6361 7365  ngr>...X....case
-00002ee0: 2d65 7874 7261 706f 6c61 7469 6f6e 723f  -extrapolationr?
-00002ef0: 0200 0058 0d00 0000 6361 7365 2d70 656e  ...X....case-pen
-00002f00: 6475 6c75 6d72 4002 0000 580d 0000 0063  dulumr@...X....c
-00002f10: 6173 652d 6f75 746c 6965 7273 7241 0200  ase-outliersrA..
-00002f20: 0058 0600 0000 6c73 7166 6974 7242 0200  .X....lsqfitrB..
-00002f30: 0058 0300 0000 6773 6c72 4302 0000 5805  .X....gslrC...X.
-00002f40: 0000 0073 6369 7079 7244 0200 0065 7355  ...scipyrD...esU
-00002f50: 0869 6e63 6c75 6465 6472 4502 0000 6807  .includedrE...h.
-00002f60: 5d85 5272 4602 0000 5504 746f 6373 7247  ].RrF...U.tocsrG
-00002f70: 0200 007d 7248 0200 0028 680c 6364 6f63  ...}rH...(h.cdoc
-00002f80: 7574 696c 732e 6e6f 6465 730a 6275 6c6c  utils.nodes.bull
-00002f90: 6574 5f6c 6973 740a 7249 0200 0029 8172  et_list.rI...).r
-00002fa0: 4a02 0000 7d72 4b02 0000 2868 1055 0068  J...}rK...(h.U.h
-00002fb0: 117d 724c 0200 0028 6813 5d68 145d 6815  .}rL...(h.]h.]h.
-00002fc0: 5d68 165d 6817 5d75 6818 5d72 4d02 0000  ]h.]h.]uh.]rM...
-00002fd0: 2863 646f 6375 7469 6c73 2e6e 6f64 6573  (cdocutils.nodes
-00002fe0: 0a6c 6973 745f 6974 656d 0a72 4e02 0000  .list_item.rN...
-00002ff0: 2981 724f 0200 007d 7250 0200 0028 6810  ).rO...}rP...(h.
-00003000: 5500 6811 7d72 5102 0000 2868 135d 6814  U.h.}rQ...(h.]h.
-00003010: 5d68 155d 6816 5d68 175d 7568 1f6a 4a02  ]h.]h.]h.]uh.jJ.
-00003020: 0000 6818 5d72 5202 0000 2863 7370 6869  ..h.]rR...(csphi
-00003030: 6e78 2e61 6464 6e6f 6465 730a 636f 6d70  nx.addnodes.comp
-00003040: 6163 745f 7061 7261 6772 6170 680a 7253  act_paragraph.rS
-00003050: 0200 0029 8172 5402 0000 7d72 5502 0000  ...).rT...}rU...
-00003060: 2868 1055 0068 117d 7256 0200 0028 6813  (h.U.h.}rV...(h.
-00003070: 5d68 145d 6815 5d68 165d 6817 5d75 681f  ]h.]h.]h.]h.]uh.
-00003080: 6a4f 0200 0068 185d 7257 0200 0063 646f  jO...h.]rW...cdo
-00003090: 6375 7469 6c73 2e6e 6f64 6573 0a72 6566  cutils.nodes.ref
-000030a0: 6572 656e 6365 0a72 5802 0000 2981 7259  erence.rX...).rY
-000030b0: 0200 007d 725a 0200 0028 6810 5500 6811  ...}rZ...(h.U.h.
-000030c0: 7d72 5b02 0000 2855 0a61 6e63 686f 726e  }r[...(U.anchorn
-000030d0: 616d 6555 0055 0672 6566 7572 6968 0c68  ameU.U.refurih.h
-000030e0: 165d 6815 5d68 135d 6814 5d68 175d 5508  .]h.]h.]h.]h.]U.
-000030f0: 696e 7465 726e 616c 8875 681f 6a54 0200  internal.uh.jT..
-00003100: 0068 185d 725c 0200 0068 1a58 1400 0000  .h.]r\...h.X....
-00003110: 6c73 7166 6974 2044 6f63 756d 656e 7461  lsqfit Documenta
-00003120: 7469 6f6e 725d 0200 0085 8172 5e02 0000  tionr].....r^...
-00003130: 7d72 5f02 0000 2868 1068 1e68 1f6a 5902  }r_...(h.h.h.jY.
-00003140: 0000 7562 6168 2055 0972 6566 6572 656e  ..ubah U.referen
-00003150: 6365 7260 0200 0075 6261 6820 5511 636f  cer`...ubah U.co
-00003160: 6d70 6163 745f 7061 7261 6772 6170 6872  mpact_paragraphr
-00003170: 6102 0000 7562 6a49 0200 0029 8172 6202  a...ubjI...).rb.
-00003180: 0000 7d72 6302 0000 2868 1055 0068 117d  ..}rc...(h.U.h.}
-00003190: 7264 0200 0028 6813 5d68 145d 6815 5d68  rd...(h.]h.]h.]h
-000031a0: 165d 6817 5d75 681f 6a4f 0200 0068 185d  .]h.]uh.jO...h.]
-000031b0: 7265 0200 0063 7370 6869 6e78 2e61 6464  re...csphinx.add
-000031c0: 6e6f 6465 730a 746f 6374 7265 650a 7266  nodes.toctree.rf
-000031d0: 0200 0029 8172 6702 0000 7d72 6802 0000  ...).rg...}rh...
-000031e0: 2868 1055 0068 1f6a 6202 0000 5506 736f  (h.U.h.jb...U.so
-000031f0: 7572 6365 7269 0200 0058 3600 0000 2f55  urceri...X6.../U
-00003200: 7365 7273 2f67 706c 2f73 6f66 7477 6172  sers/gpl/softwar
-00003210: 652f 7079 7468 6f6e 2f6c 7371 6669 742f  e/python/lsqfit/
-00003220: 646f 632f 736f 7572 6365 2f69 6e64 6578  doc/source/index
-00003230: 2e72 7374 6820 5507 746f 6374 7265 6572  .rsth U.toctreer
-00003240: 6a02 0000 6811 7d72 6b02 0000 2855 086e  j...h.}rk...(U.n
-00003250: 756d 6265 7265 644b 0055 0670 6172 656e  umberedK.U.paren
-00003260: 7468 0c55 0a74 6974 6c65 736f 6e6c 7989  th.U.titlesonly.
-00003270: 5508 6d61 7864 6570 7468 4b02 5504 676c  U.maxdepthK.U.gl
-00003280: 6f62 8968 165d 6815 5d68 135d 6814 5d68  ob.h.]h.]h.]h.]h
-00003290: 175d 5507 656e 7472 6965 735d 726c 0200  .]U.entries]rl..
-000032a0: 0028 4e6a 3d02 0000 8672 6d02 0000 4e6a  .(Nj=....rm...Nj
-000032b0: 3e02 0000 8672 6e02 0000 4e6a 3f02 0000  >....rn...Nj?...
-000032c0: 8672 6f02 0000 4e6a 4002 0000 8672 7002  .ro...Nj@....rp.
-000032d0: 0000 4e6a 4102 0000 8672 7102 0000 4e6a  ..NjA....rq...Nj
-000032e0: 4202 0000 8672 7202 0000 4e6a 4302 0000  B....rr...NjC...
-000032f0: 8672 7302 0000 4e6a 4402 0000 8672 7402  .rs...NjD....rt.
-00003300: 0000 6555 0668 6964 6465 6e89 5507 6361  ..eU.hidden.U.ca
-00003310: 7074 696f 6e4e 550c 696e 636c 7564 6566  ptionNU.includef
-00003320: 696c 6573 5d72 7502 0000 286a 3d02 0000  iles]ru...(j=...
-00003330: 6a3e 0200 006a 3f02 0000 6a40 0200 006a  j>...j?...j@...j
-00003340: 4102 0000 6a42 0200 006a 4302 0000 6a44  A...jB...jC...jD
-00003350: 0200 0065 550d 696e 636c 7564 6568 6964  ...eU.includehid
-00003360: 6465 6e89 7555 046c 696e 6572 7602 0000  den.uU.linerv...
-00003370: 4b0b 6818 5d75 6261 6820 550b 6275 6c6c  K.h.]ubah U.bull
-00003380: 6574 5f6c 6973 7472 7702 0000 7562 6568  et_listrw...ubeh
-00003390: 2055 096c 6973 745f 6974 656d 7278 0200   U.list_itemrx..
-000033a0: 0075 626a 4e02 0000 2981 7279 0200 007d  .ubjN...).ry...}
-000033b0: 727a 0200 0028 6810 5500 6811 7d72 7b02  rz...(h.U.h.}r{.
-000033c0: 0000 2868 135d 6814 5d68 155d 6816 5d68  ..(h.]h.]h.]h.]h
-000033d0: 175d 7568 1f6a 4a02 0000 6818 5d72 7c02  .]uh.jJ...h.]r|.
-000033e0: 0000 6a53 0200 0029 8172 7d02 0000 7d72  ..jS...).r}...}r
-000033f0: 7e02 0000 2868 1055 0068 117d 727f 0200  ~...(h.U.h.}r...
-00003400: 0028 6813 5d68 145d 6815 5d68 165d 6817  .(h.]h.]h.]h.]h.
-00003410: 5d75 681f 6a79 0200 0068 185d 7280 0200  ]uh.jy...h.]r...
-00003420: 006a 5802 0000 2981 7281 0200 007d 7282  .jX...).r....}r.
-00003430: 0200 0028 6810 5500 6811 7d72 8302 0000  ...(h.U.h.}r....
-00003440: 2855 0a61 6e63 686f 726e 616d 6555 1323  (U.anchornameU.#
-00003450: 696e 6469 6365 732d 616e 642d 7461 626c  indices-and-tabl
-00003460: 6573 5506 7265 6675 7269 680c 6816 5d68  esU.refurih.h.]h
-00003470: 155d 6813 5d68 145d 6817 5d55 0869 6e74  .]h.]h.]h.]U.int
-00003480: 6572 6e61 6c88 7568 1f6a 7d02 0000 6818  ernal.uh.j}...h.
-00003490: 5d72 8402 0000 681a 5812 0000 0049 6e64  ]r....h.X....Ind
-000034a0: 6963 6573 2061 6e64 2074 6162 6c65 7372  ices and tablesr
-000034b0: 8502 0000 8581 7286 0200 007d 7287 0200  ......r....}r...
-000034c0: 0028 6810 5812 0000 0049 6e64 6963 6573  .(h.X....Indices
-000034d0: 2061 6e64 2074 6162 6c65 7368 1f6a 8102   and tablesh.j..
-000034e0: 0000 7562 6168 206a 6002 0000 7562 6168  ..ubah j`...ubah
-000034f0: 206a 6102 0000 7562 6168 206a 7802 0000   ja...ubah jx...
-00003500: 7562 6568 206a 7702 0000 7562 6822 6a49  ubeh jw...ubh"jI
-00003510: 0200 0029 8172 8802 0000 7d72 8902 0000  ...).r....}r....
-00003520: 2868 1055 0068 117d 728a 0200 0028 6813  (h.U.h.}r....(h.
-00003530: 5d68 145d 6815 5d68 165d 6817 5d75 6818  ]h.]h.]h.]h.]uh.
-00003540: 5d72 8b02 0000 6a4e 0200 0029 8172 8c02  ]r....jN...).r..
-00003550: 0000 7d72 8d02 0000 2868 1055 0068 117d  ..}r....(h.U.h.}
-00003560: 728e 0200 0028 6813 5d68 145d 6815 5d68  r....(h.]h.]h.]h
-00003570: 165d 6817 5d75 681f 6a88 0200 0068 185d  .]h.]uh.j....h.]
-00003580: 728f 0200 0028 6a53 0200 0029 8172 9002  r....(jS...).r..
-00003590: 0000 7d72 9102 0000 2868 1055 0068 117d  ..}r....(h.U.h.}
-000035a0: 7292 0200 0028 6813 5d68 145d 6815 5d68  r....(h.]h.]h.]h
-000035b0: 165d 6817 5d75 681f 6a8c 0200 0068 185d  .]h.]uh.j....h.]
-000035c0: 7293 0200 006a 5802 0000 2981 7294 0200  r....jX...).r...
-000035d0: 007d 7295 0200 0028 6810 5500 6811 7d72  .}r....(h.U.h.}r
-000035e0: 9602 0000 2855 0a61 6e63 686f 726e 616d  ....(U.anchornam
-000035f0: 6555 0055 0672 6566 7572 6968 2268 165d  eU.U.refurih"h.]
-00003600: 6815 5d68 135d 6814 5d68 175d 5508 696e  h.]h.]h.]h.]U.in
-00003610: 7465 726e 616c 8875 681f 6a90 0200 0068  ternal.uh.j....h
-00003620: 185d 7297 0200 0068 1a58 2300 0000 4e6f  .]r....h.X#...No
-00003630: 6e2d 4761 7573 7369 616e 2042 6568 6176  n-Gaussian Behav
-00003640: 696f 723b 2054 6573 7469 6e67 2046 6974  ior; Testing Fit
-00003650: 7372 9802 0000 8581 7299 0200 007d 729a  sr......r....}r.
-00003660: 0200 0028 6810 682a 681f 6a94 0200 0075  ...(h.h*h.j....u
-00003670: 6261 6820 6a60 0200 0075 6261 6820 6a61  bah j`...ubah ja
-00003680: 0200 0075 626a 4902 0000 2981 729b 0200  ...ubjI...).r...
-00003690: 007d 729c 0200 0028 6810 5500 6811 7d72  .}r....(h.U.h.}r
-000036a0: 9d02 0000 2868 135d 6814 5d68 155d 6816  ....(h.]h.]h.]h.
-000036b0: 5d68 175d 7568 1f6a 8c02 0000 6818 5d72  ]h.]uh.j....h.]r
-000036c0: 9e02 0000 286a 4e02 0000 2981 729f 0200  ....(jN...).r...
-000036d0: 007d 72a0 0200 0028 6810 5500 6811 7d72  .}r....(h.U.h.}r
-000036e0: a102 0000 2868 135d 6814 5d68 155d 6816  ....(h.]h.]h.]h.
-000036f0: 5d68 175d 7568 1f6a 9b02 0000 6818 5d72  ]h.]uh.j....h.]r
-00003700: a202 0000 6a53 0200 0029 8172 a302 0000  ....jS...).r....
-00003710: 7d72 a402 0000 2868 1055 0068 117d 72a5  }r....(h.U.h.}r.
-00003720: 0200 0028 6813 5d68 145d 6815 5d68 165d  ...(h.]h.]h.]h.]
-00003730: 6817 5d75 681f 6a9f 0200 0068 185d 72a6  h.]uh.j....h.]r.
-00003740: 0200 006a 5802 0000 2981 72a7 0200 007d  ...jX...).r....}
-00003750: 72a8 0200 0028 6810 5500 6811 7d72 a902  r....(h.U.h.}r..
-00003760: 0000 2855 0a61 6e63 686f 726e 616d 6555  ..(U.anchornameU
-00003770: 0d23 696e 7472 6f64 7563 7469 6f6e 5506  .#introductionU.
-00003780: 7265 6675 7269 6822 6816 5d68 155d 6813  refurih"h.]h.]h.
-00003790: 5d68 145d 6817 5d55 0869 6e74 6572 6e61  ]h.]h.]U.interna
-000037a0: 6c88 7568 1f6a a302 0000 6818 5d72 aa02  l.uh.j....h.]r..
-000037b0: 0000 681a 580c 0000 0049 6e74 726f 6475  ..h.X....Introdu
-000037c0: 6374 696f 6e72 ab02 0000 8581 72ac 0200  ctionr......r...
-000037d0: 007d 72ad 0200 0028 6810 580c 0000 0049  .}r....(h.X....I
-000037e0: 6e74 726f 6475 6374 696f 6e72 ae02 0000  ntroductionr....
-000037f0: 681f 6aa7 0200 0075 6261 6820 6a60 0200  h.j....ubah j`..
-00003800: 0075 6261 6820 6a61 0200 0075 6261 6820  .ubah ja...ubah 
-00003810: 6a78 0200 0075 626a 4e02 0000 2981 72af  jx...ubjN...).r.
-00003820: 0200 007d 72b0 0200 0028 6810 5500 6811  ...}r....(h.U.h.
-00003830: 7d72 b102 0000 2868 135d 6814 5d68 155d  }r....(h.]h.]h.]
-00003840: 6816 5d68 175d 7568 1f6a 9b02 0000 6818  h.]h.]uh.j....h.
-00003850: 5d72 b202 0000 6a53 0200 0029 8172 b302  ]r....jS...).r..
-00003860: 0000 7d72 b402 0000 2868 1055 0068 117d  ..}r....(h.U.h.}
-00003870: 72b5 0200 0028 6813 5d68 145d 6815 5d68  r....(h.]h.]h.]h
-00003880: 165d 6817 5d75 681f 6aaf 0200 0068 185d  .]h.]uh.j....h.]
-00003890: 72b6 0200 006a 5802 0000 2981 72b7 0200  r....jX...).r...
-000038a0: 007d 72b8 0200 0028 6810 5500 6811 7d72  .}r....(h.U.h.}r
-000038b0: b902 0000 2855 0a61 6e63 686f 726e 616d  ....(U.anchornam
-000038c0: 6555 2d23 626f 6f74 7374 7261 702d 6572  eU-#bootstrap-er
-000038d0: 726f 722d 616e 616c 7973 6973 2d6e 6f6e  ror-analysis-non
-000038e0: 2d67 6175 7373 6961 6e2d 6f75 7470 7574  -gaussian-output
-000038f0: 5506 7265 6675 7269 6822 6816 5d68 155d  U.refurih"h.]h.]
-00003900: 6813 5d68 145d 6817 5d55 0869 6e74 6572  h.]h.]h.]U.inter
-00003910: 6e61 6c88 7568 1f6a b302 0000 6818 5d72  nal.uh.j....h.]r
-00003920: ba02 0000 681a 582d 0000 0042 6f6f 7473  ....h.X-...Boots
-00003930: 7472 6170 2045 7272 6f72 2041 6e61 6c79  trap Error Analy
-00003940: 7369 733b 204e 6f6e 2d47 6175 7373 6961  sis; Non-Gaussia
-00003950: 6e20 4f75 7470 7574 72bb 0200 0085 8172  n Outputr......r
-00003960: bc02 0000 7d72 bd02 0000 2868 1058 2d00  ....}r....(h.X-.
-00003970: 0000 426f 6f74 7374 7261 7020 4572 726f  ..Bootstrap Erro
-00003980: 7220 416e 616c 7973 6973 3b20 4e6f 6e2d  r Analysis; Non-
-00003990: 4761 7573 7369 616e 204f 7574 7075 7472  Gaussian Outputr
-000039a0: be02 0000 681f 6ab7 0200 0075 6261 6820  ....h.j....ubah 
-000039b0: 6a60 0200 0075 6261 6820 6a61 0200 0075  j`...ubah ja...u
-000039c0: 6261 6820 6a78 0200 0075 626a 4e02 0000  bah jx...ubjN...
-000039d0: 2981 72bf 0200 007d 72c0 0200 0028 6810  ).r....}r....(h.
-000039e0: 5500 6811 7d72 c102 0000 2868 135d 6814  U.h.}r....(h.]h.
-000039f0: 5d68 155d 6816 5d68 175d 7568 1f6a 9b02  ]h.]h.]h.]uh.j..
-00003a00: 0000 6818 5d72 c202 0000 6a53 0200 0029  ..h.]r....jS...)
-00003a10: 8172 c302 0000 7d72 c402 0000 2868 1055  .r....}r....(h.U
-00003a20: 0068 117d 72c5 0200 0028 6813 5d68 145d  .h.}r....(h.]h.]
-00003a30: 6815 5d68 165d 6817 5d75 681f 6abf 0200  h.]h.]h.]uh.j...
-00003a40: 0068 185d 72c6 0200 006a 5802 0000 2981  .h.]r....jX...).
-00003a50: 72c7 0200 007d 72c8 0200 0028 6810 5500  r....}r....(h.U.
-00003a60: 6811 7d72 c902 0000 2855 0a61 6e63 686f  h.}r....(U.ancho
-00003a70: 726e 616d 6555 1323 6261 7965 7369 616e  rnameU.#bayesian
-00003a80: 2d69 6e74 6567 7261 6c73 5506 7265 6675  -integralsU.refu
-00003a90: 7269 6822 6816 5d68 155d 6813 5d68 145d  rih"h.]h.]h.]h.]
-00003aa0: 6817 5d55 0869 6e74 6572 6e61 6c88 7568  h.]U.internal.uh
-00003ab0: 1f6a c302 0000 6818 5d72 ca02 0000 681a  .j....h.]r....h.
-00003ac0: 5812 0000 0042 6179 6573 6961 6e20 496e  X....Bayesian In
-00003ad0: 7465 6772 616c 7372 cb02 0000 8581 72cc  tegralsr......r.
-00003ae0: 0200 007d 72cd 0200 0028 6810 5812 0000  ...}r....(h.X...
-00003af0: 0042 6179 6573 6961 6e20 496e 7465 6772  .Bayesian Integr
-00003b00: 616c 7372 ce02 0000 681f 6ac7 0200 0075  alsr....h.j....u
-00003b10: 6261 6820 6a60 0200 0075 6261 6820 6a61  bah j`...ubah ja
-00003b20: 0200 0075 6261 6820 6a78 0200 0075 626a  ...ubah jx...ubj
-00003b30: 4e02 0000 2981 72cf 0200 007d 72d0 0200  N...).r....}r...
-00003b40: 0028 6810 5500 6811 7d72 d102 0000 2868  .(h.U.h.}r....(h
-00003b50: 135d 6814 5d68 155d 6816 5d68 175d 7568  .]h.]h.]h.]h.]uh
-00003b60: 1f6a 9b02 0000 6818 5d72 d202 0000 6a53  .j....h.]r....jS
-00003b70: 0200 0029 8172 d302 0000 7d72 d402 0000  ...).r....}r....
-00003b80: 2868 1055 0068 117d 72d5 0200 0028 6813  (h.U.h.}r....(h.
-00003b90: 5d68 145d 6815 5d68 165d 6817 5d75 681f  ]h.]h.]h.]h.]uh.
-00003ba0: 6acf 0200 0068 185d 72d6 0200 006a 5802  j....h.]r....jX.
-00003bb0: 0000 2981 72d7 0200 007d 72d8 0200 0028  ..).r....}r....(
-00003bc0: 6810 5500 6811 7d72 d902 0000 2855 0a61  h.U.h.}r....(U.a
-00003bd0: 6e63 686f 726e 616d 6555 2123 7465 7374  nchornameU!#test
-00003be0: 696e 672d 6669 7473 2d77 6974 682d 7369  ing-fits-with-si
-00003bf0: 6d75 6c61 7465 642d 6461 7461 5506 7265  mulated-dataU.re
-00003c00: 6675 7269 6822 6816 5d68 155d 6813 5d68  furih"h.]h.]h.]h
-00003c10: 145d 6817 5d55 0869 6e74 6572 6e61 6c88  .]h.]U.internal.
-00003c20: 7568 1f6a d302 0000 6818 5d72 da02 0000  uh.j....h.]r....
-00003c30: 681a 5820 0000 0054 6573 7469 6e67 2046  h.X ...Testing F
-00003c40: 6974 7320 7769 7468 2053 696d 756c 6174  its with Simulat
-00003c50: 6564 2044 6174 6172 db02 0000 8581 72dc  ed Datar......r.
-00003c60: 0200 007d 72dd 0200 0028 6810 5820 0000  ...}r....(h.X ..
-00003c70: 0054 6573 7469 6e67 2046 6974 7320 7769  .Testing Fits wi
-00003c80: 7468 2053 696d 756c 6174 6564 2044 6174  th Simulated Dat
-00003c90: 6172 de02 0000 681f 6ad7 0200 0075 6261  ar....h.j....uba
-00003ca0: 6820 6a60 0200 0075 6261 6820 6a61 0200  h j`...ubah ja..
-00003cb0: 0075 6261 6820 6a78 0200 0075 6265 6820  .ubah jx...ubeh 
-00003cc0: 6a77 0200 0075 6265 6820 6a78 0200 0075  jw...ubeh jx...u
-00003cd0: 6261 6820 6a77 0200 0075 6268 2b6a 4902  bah jw...ubh+jI.
-00003ce0: 0000 2981 72df 0200 007d 72e0 0200 0028  ..).r....}r....(
-00003cf0: 6810 5500 6811 7d72 e102 0000 2868 135d  h.U.h.}r....(h.]
-00003d00: 6814 5d68 155d 6816 5d68 175d 7568 185d  h.]h.]h.]h.]uh.]
-00003d10: 72e2 0200 006a 4e02 0000 2981 72e3 0200  r....jN...).r...
-00003d20: 007d 72e4 0200 0028 6810 5500 6811 7d72  .}r....(h.U.h.}r
-00003d30: e502 0000 2868 135d 6814 5d68 155d 6816  ....(h.]h.]h.]h.
-00003d40: 5d68 175d 7568 1f6a df02 0000 6818 5d72  ]h.]uh.j....h.]r
-00003d50: e602 0000 286a 5302 0000 2981 72e7 0200  ....(jS...).r...
-00003d60: 007d 72e8 0200 0028 6810 5500 6811 7d72  .}r....(h.U.h.}r
-00003d70: e902 0000 2868 135d 6814 5d68 155d 6816  ....(h.]h.]h.]h.
-00003d80: 5d68 175d 7568 1f6a e302 0000 6818 5d72  ]h.]uh.j....h.]r
-00003d90: ea02 0000 6a58 0200 0029 8172 eb02 0000  ....jX...).r....
-00003da0: 7d72 ec02 0000 2868 1055 0068 117d 72ed  }r....(h.U.h.}r.
-00003db0: 0200 0028 550a 616e 6368 6f72 6e61 6d65  ...(U.anchorname
-00003dc0: 5500 5506 7265 6675 7269 682b 6816 5d68  U.U.refurih+h.]h
-00003dd0: 155d 6813 5d68 145d 6817 5d55 0869 6e74  .]h.]h.]h.]U.int
-00003de0: 6572 6e61 6c88 7568 1f6a e702 0000 6818  ernal.uh.j....h.
-00003df0: 5d72 ee02 0000 2868 3029 8172 ef02 0000  ]r....(h0).r....
-00003e00: 7d72 f002 0000 2868 1058 0600 0000 6c73  }r....(h.X....ls
-00003e10: 7166 6974 6811 7d72 f102 0000 2868 135d  qfith.}r....(h.]
-00003e20: 6814 5d68 155d 6816 5d68 175d 7568 1f6a  h.]h.]h.]h.]uh.j
-00003e30: eb02 0000 6818 5d72 f202 0000 681a 5806  ....h.]r....h.X.
-00003e40: 0000 006c 7371 6669 7472 f302 0000 8581  ...lsqfitr......
-00003e50: 72f4 0200 007d 72f5 0200 0028 6810 5500  r....}r....(h.U.
-00003e60: 681f 6aef 0200 0075 6261 6820 6838 7562  h.j....ubah h8ub
-00003e70: 681a 5822 0000 0020 2d20 4e6f 6e6c 696e  h.X"... - Nonlin
-00003e80: 6561 7220 4c65 6173 7420 5371 7561 7265  ear Least Square
-00003e90: 7320 4669 7474 696e 6772 f602 0000 8581  s Fittingr......
-00003ea0: 72f7 0200 007d 72f8 0200 0028 6810 683c  r....}r....(h.h<
-00003eb0: 681f 6aeb 0200 0075 6265 6820 6a60 0200  h.j....ubeh j`..
-00003ec0: 0075 6261 6820 6a61 0200 0075 626a 4902  .ubah ja...ubjI.
-00003ed0: 0000 2981 72f9 0200 007d 72fa 0200 0028  ..).r....}r....(
-00003ee0: 6810 5500 6811 7d72 fb02 0000 2868 135d  h.U.h.}r....(h.]
-00003ef0: 6814 5d68 155d 6816 5d68 175d 7568 1f6a  h.]h.]h.]h.]uh.j
-00003f00: e302 0000 6818 5d72 fc02 0000 286a 4e02  ....h.]r....(jN.
-00003f10: 0000 2981 72fd 0200 007d 72fe 0200 0028  ..).r....}r....(
-00003f20: 6810 5500 6811 7d72 ff02 0000 2868 135d  h.U.h.}r....(h.]
-00003f30: 6814 5d68 155d 6816 5d68 175d 7568 1f6a  h.]h.]h.]h.]uh.j
-00003f40: f902 0000 6818 5d72 0003 0000 6a53 0200  ....h.]r....jS..
-00003f50: 0029 8172 0103 0000 7d72 0203 0000 2868  .).r....}r....(h
-00003f60: 1055 0068 117d 7203 0300 0028 6813 5d68  .U.h.}r....(h.]h
-00003f70: 145d 6815 5d68 165d 6817 5d75 681f 6afd  .]h.]h.]h.]uh.j.
-00003f80: 0200 0068 185d 7204 0300 006a 5802 0000  ...h.]r....jX...
-00003f90: 2981 7205 0300 007d 7206 0300 0028 6810  ).r....}r....(h.
-00003fa0: 5500 6811 7d72 0703 0000 2855 0a61 6e63  U.h.}r....(U.anc
-00003fb0: 686f 726e 616d 6555 0d23 696e 7472 6f64  hornameU.#introd
-00003fc0: 7563 7469 6f6e 5506 7265 6675 7269 682b  uctionU.refurih+
-00003fd0: 6816 5d68 155d 6813 5d68 145d 6817 5d55  h.]h.]h.]h.]h.]U
-00003fe0: 0869 6e74 6572 6e61 6c88 7568 1f6a 0103  .internal.uh.j..
-00003ff0: 0000 6818 5d72 0803 0000 681a 580c 0000  ..h.]r....h.X...
-00004000: 0049 6e74 726f 6475 6374 696f 6e72 0903  .Introductionr..
-00004010: 0000 8581 720a 0300 007d 720b 0300 0028  ....r....}r....(
-00004020: 6810 580c 0000 0049 6e74 726f 6475 6374  h.X....Introduct
-00004030: 696f 6e72 0c03 0000 681f 6a05 0300 0075  ionr....h.j....u
-00004040: 6261 6820 6a60 0200 0075 6261 6820 6a61  bah j`...ubah ja
-00004050: 0200 0075 6261 6820 6a78 0200 0075 626a  ...ubah jx...ubj
-00004060: 4e02 0000 2981 720d 0300 007d 720e 0300  N...).r....}r...
-00004070: 0028 6810 5500 6811 7d72 0f03 0000 2868  .(h.U.h.}r....(h
-00004080: 135d 6814 5d68 155d 6816 5d68 175d 7568  .]h.]h.]h.]h.]uh
-00004090: 1f6a f902 0000 6818 5d72 1003 0000 6a53  .j....h.]r....jS
-000040a0: 0200 0029 8172 1103 0000 7d72 1203 0000  ...).r....}r....
-000040b0: 2868 1055 0068 117d 7213 0300 0028 6813  (h.U.h.}r....(h.
-000040c0: 5d68 145d 6815 5d68 165d 6817 5d75 681f  ]h.]h.]h.]h.]uh.
-000040d0: 6a0d 0300 0068 185d 7214 0300 006a 5802  j....h.]r....jX.
-000040e0: 0000 2981 7215 0300 007d 7216 0300 0028  ..).r....}r....(
-000040f0: 6810 5500 6811 7d72 1703 0000 2855 0a61  h.U.h.}r....(U.a
-00004100: 6e63 686f 726e 616d 6555 1623 6e6f 6e6c  nchornameU.#nonl
-00004110: 696e 6561 722d 6669 742d 6f62 6a65 6374  inear-fit-object
-00004120: 7355 0672 6566 7572 6968 2b68 165d 6815  sU.refurih+h.]h.
-00004130: 5d68 135d 6814 5d68 175d 5508 696e 7465  ]h.]h.]h.]U.inte
-00004140: 726e 616c 8875 681f 6a11 0300 0068 185d  rnal.uh.j....h.]
-00004150: 7218 0300 0068 1a58 1500 0000 6e6f 6e6c  r....h.X....nonl
-00004160: 696e 6561 725f 6669 7420 4f62 6a65 6374  inear_fit Object
-00004170: 7372 1903 0000 8581 721a 0300 007d 721b  sr......r....}r.
-00004180: 0300 0028 6810 5815 0000 006e 6f6e 6c69  ...(h.X....nonli
-00004190: 6e65 6172 5f66 6974 204f 626a 6563 7473  near_fit Objects
-000041a0: 721c 0300 0068 1f6a 1503 0000 7562 6168  r....h.j....ubah
-000041b0: 206a 6002 0000 7562 6168 206a 6102 0000   j`...ubah ja...
-000041c0: 7562 6168 206a 7802 0000 7562 6a4e 0200  ubah jx...ubjN..
-000041d0: 0029 8172 1d03 0000 7d72 1e03 0000 2868  .).r....}r....(h
-000041e0: 1055 0068 117d 721f 0300 0028 6813 5d68  .U.h.}r....(h.]h
-000041f0: 145d 6815 5d68 165d 6817 5d75 681f 6af9  .]h.]h.]h.]uh.j.
-00004200: 0200 0068 185d 7220 0300 006a 5302 0000  ...h.]r ...jS...
-00004210: 2981 7221 0300 007d 7222 0300 0028 6810  ).r!...}r"...(h.
-00004220: 5500 6811 7d72 2303 0000 2868 135d 6814  U.h.}r#...(h.]h.
-00004230: 5d68 155d 6816 5d68 175d 7568 1f6a 1d03  ]h.]h.]h.]uh.j..
-00004240: 0000 6818 5d72 2403 0000 6a58 0200 0029  ..h.]r$...jX...)
-00004250: 8172 2503 0000 7d72 2603 0000 2868 1055  .r%...}r&...(h.U
-00004260: 0068 117d 7227 0300 0028 550a 616e 6368  .h.}r'...(U.anch
-00004270: 6f72 6e61 6d65 550a 2366 756e 6374 696f  ornameU.#functio
-00004280: 6e73 5506 7265 6675 7269 682b 6816 5d68  nsU.refurih+h.]h
-00004290: 155d 6813 5d68 145d 6817 5d55 0869 6e74  .]h.]h.]h.]U.int
-000042a0: 6572 6e61 6c88 7568 1f6a 2103 0000 6818  ernal.uh.j!...h.
-000042b0: 5d72 2803 0000 681a 5809 0000 0046 756e  ]r(...h.X....Fun
-000042c0: 6374 696f 6e73 7229 0300 0085 8172 2a03  ctionsr).....r*.
-000042d0: 0000 7d72 2b03 0000 2868 1058 0900 0000  ..}r+...(h.X....
-000042e0: 4675 6e63 7469 6f6e 7372 2c03 0000 681f  Functionsr,...h.
-000042f0: 6a25 0300 0075 6261 6820 6a60 0200 0075  j%...ubah j`...u
-00004300: 6261 6820 6a61 0200 0075 6261 6820 6a78  bah ja...ubah jx
-00004310: 0200 0075 626a 4e02 0000 2981 722d 0300  ...ubjN...).r-..
-00004320: 007d 722e 0300 0028 6810 5500 6811 7d72  .}r....(h.U.h.}r
-00004330: 2f03 0000 2868 135d 6814 5d68 155d 6816  /...(h.]h.]h.]h.
-00004340: 5d68 175d 7568 1f6a f902 0000 6818 5d72  ]h.]uh.j....h.]r
-00004350: 3003 0000 6a53 0200 0029 8172 3103 0000  0...jS...).r1...
-00004360: 7d72 3203 0000 2868 1055 0068 117d 7233  }r2...(h.U.h.}r3
-00004370: 0300 0028 6813 5d68 145d 6815 5d68 165d  ...(h.]h.]h.]h.]
-00004380: 6817 5d75 681f 6a2d 0300 0068 185d 7234  h.]uh.j-...h.]r4
-00004390: 0300 006a 5802 0000 2981 7235 0300 007d  ...jX...).r5...}
-000043a0: 7236 0300 0028 6810 5500 6811 7d72 3703  r6...(h.U.h.}r7.
-000043b0: 0000 2855 0a61 6e63 686f 726e 616d 6555  ..(U.anchornameU
-000043c0: 1f23 636c 6173 7365 732d 666f 722d 6261  .#classes-for-ba
-000043d0: 7965 7369 616e 2d69 6e74 6567 7261 6c73  yesian-integrals
-000043e0: 5506 7265 6675 7269 682b 6816 5d68 155d  U.refurih+h.]h.]
-000043f0: 6813 5d68 145d 6817 5d55 0869 6e74 6572  h.]h.]h.]U.inter
-00004400: 6e61 6c88 7568 1f6a 3103 0000 6818 5d72  nal.uh.j1...h.]r
-00004410: 3803 0000 681a 581e 0000 0043 6c61 7373  8...h.X....Class
-00004420: 6573 2066 6f72 2042 6179 6573 6961 6e20  es for Bayesian 
-00004430: 496e 7465 6772 616c 7372 3903 0000 8581  Integralsr9.....
-00004440: 723a 0300 007d 723b 0300 0028 6810 581e  r:...}r;...(h.X.
-00004450: 0000 0043 6c61 7373 6573 2066 6f72 2042  ...Classes for B
-00004460: 6179 6573 6961 6e20 496e 7465 6772 616c  ayesian Integral
-00004470: 7372 3c03 0000 681f 6a35 0300 0075 6261  sr<...h.j5...uba
-00004480: 6820 6a60 0200 0075 6261 6820 6a61 0200  h j`...ubah ja..
-00004490: 0075 6261 6820 6a78 0200 0075 626a 4e02  .ubah jx...ubjN.
-000044a0: 0000 2981 723d 0300 007d 723e 0300 0028  ..).r=...}r>...(
-000044b0: 6810 5500 6811 7d72 3f03 0000 2868 135d  h.U.h.}r?...(h.]
-000044c0: 6814 5d68 155d 6816 5d68 175d 7568 1f6a  h.]h.]h.]h.]uh.j
-000044d0: f902 0000 6818 5d72 4003 0000 6a53 0200  ....h.]r@...jS..
-000044e0: 0029 8172 4103 0000 7d72 4203 0000 2868  .).rA...}rB...(h
-000044f0: 1055 0068 117d 7243 0300 0028 6813 5d68  .U.h.}rC...(h.]h
-00004500: 145d 6815 5d68 165d 6817 5d75 681f 6a3d  .]h.]h.]h.]uh.j=
-00004510: 0300 0068 185d 7244 0300 006a 5802 0000  ...h.]rD...jX...
-00004520: 2981 7245 0300 007d 7246 0300 0028 6810  ).rE...}rF...(h.
-00004530: 5500 6811 7d72 4703 0000 2855 0a61 6e63  U.h.}rG...(U.anc
-00004540: 686f 726e 616d 6555 1b23 6c73 7166 6974  hornameU.#lsqfit
-00004550: 2d6d 756c 7469 6669 7474 6572 2d63 6c61  -multifitter-cla
-00004560: 7373 6573 5506 7265 6675 7269 682b 6816  ssesU.refurih+h.
-00004570: 5d68 155d 6813 5d68 145d 6817 5d55 0869  ]h.]h.]h.]h.]U.i
-00004580: 6e74 6572 6e61 6c88 7568 1f6a 4103 0000  nternal.uh.jA...
-00004590: 6818 5d72 4803 0000 2868 3029 8172 4903  h.]rH...(h0).rI.
-000045a0: 0000 7d72 4a03 0000 2868 1058 1200 0000  ..}rJ...(h.X....
-000045b0: 6c73 7166 6974 2e4d 756c 7469 4669 7474  lsqfit.MultiFitt
-000045c0: 6572 6811 7d72 4b03 0000 2868 135d 6814  erh.}rK...(h.]h.
-000045d0: 5d68 155d 6816 5d68 175d 7568 1f6a 4503  ]h.]h.]h.]uh.jE.
-000045e0: 0000 6818 5d72 4c03 0000 681a 5812 0000  ..h.]rL...h.X...
-000045f0: 006c 7371 6669 742e 4d75 6c74 6946 6974  .lsqfit.MultiFit
-00004600: 7465 7272 4d03 0000 8581 724e 0300 007d  terrM.....rN...}
-00004610: 724f 0300 0028 6810 5500 681f 6a49 0300  rO...(h.U.h.jI..
-00004620: 0075 6261 6820 6838 7562 681a 5808 0000  .ubah h8ubh.X...
-00004630: 0020 436c 6173 7365 7372 5003 0000 8581  . ClassesrP.....
-00004640: 7251 0300 007d 7252 0300 0028 6810 5808  rQ...}rR...(h.X.
-00004650: 0000 0020 436c 6173 7365 7372 5303 0000  ... ClassesrS...
-00004660: 681f 6a45 0300 0075 6265 6820 6a60 0200  h.jE...ubeh j`..
-00004670: 0075 6261 6820 6a61 0200 0075 6261 6820  .ubah ja...ubah 
-00004680: 6a78 0200 0075 626a 4e02 0000 2981 7254  jx...ubjN...).rT
-00004690: 0300 007d 7255 0300 0028 6810 5500 6811  ...}rU...(h.U.h.
-000046a0: 7d72 5603 0000 2868 135d 6814 5d68 155d  }rV...(h.]h.]h.]
-000046b0: 6816 5d68 175d 7568 1f6a f902 0000 6818  h.]h.]uh.j....h.
-000046c0: 5d72 5703 0000 6a53 0200 0029 8172 5803  ]rW...jS...).rX.
-000046d0: 0000 7d72 5903 0000 2868 1055 0068 117d  ..}rY...(h.U.h.}
-000046e0: 725a 0300 0028 6813 5d68 145d 6815 5d68  rZ...(h.]h.]h.]h
-000046f0: 165d 6817 5d75 681f 6a54 0300 0068 185d  .]h.]uh.jT...h.]
-00004700: 725b 0300 006a 5802 0000 2981 725c 0300  r[...jX...).r\..
-00004710: 007d 725d 0300 0028 6810 5500 6811 7d72  .}r]...(h.U.h.}r
-00004720: 5e03 0000 2855 0a61 6e63 686f 726e 616d  ^...(U.anchornam
-00004730: 6555 0d23 7265 7175 6972 656d 656e 7473  eU.#requirements
-00004740: 5506 7265 6675 7269 682b 6816 5d68 155d  U.refurih+h.]h.]
-00004750: 6813 5d68 145d 6817 5d55 0869 6e74 6572  h.]h.]h.]U.inter
-00004760: 6e61 6c88 7568 1f6a 5803 0000 6818 5d72  nal.uh.jX...h.]r
-00004770: 5f03 0000 681a 580c 0000 0052 6571 7569  _...h.X....Requi
-00004780: 7265 6d65 6e74 7372 6003 0000 8581 7261  rementsr`.....ra
-00004790: 0300 007d 7262 0300 0028 6810 580c 0000  ...}rb...(h.X...
-000047a0: 0052 6571 7569 7265 6d65 6e74 7372 6303  .Requirementsrc.
-000047b0: 0000 681f 6a5c 0300 0075 6261 6820 6a60  ..h.j\...ubah j`
-000047c0: 0200 0075 6261 6820 6a61 0200 0075 6261  ...ubah ja...uba
-000047d0: 6820 6a78 0200 0075 6265 6820 6a77 0200  h jx...ubeh jw..
-000047e0: 0075 6265 6820 6a78 0200 0075 6261 6820  .ubeh jx...ubah 
-000047f0: 6a77 0200 0075 6268 3d6a 4902 0000 2981  jw...ubh=jI...).
-00004800: 7264 0300 007d 7265 0300 0028 6810 5500  rd...}re...(h.U.
-00004810: 6811 7d72 6603 0000 2868 135d 6814 5d68  h.}rf...(h.]h.]h
-00004820: 155d 6816 5d68 175d 7568 185d 7267 0300  .]h.]h.]uh.]rg..
-00004830: 006a 4e02 0000 2981 7268 0300 007d 7269  .jN...).rh...}ri
-00004840: 0300 0028 6810 5500 6811 7d72 6a03 0000  ...(h.U.h.}rj...
-00004850: 2868 135d 6814 5d68 155d 6816 5d68 175d  (h.]h.]h.]h.]h.]
-00004860: 7568 1f6a 6403 0000 6818 5d72 6b03 0000  uh.jd...h.]rk...
-00004870: 286a 5302 0000 2981 726c 0300 007d 726d  (jS...).rl...}rm
-00004880: 0300 0028 6810 5500 6811 7d72 6e03 0000  ...(h.U.h.}rn...
-00004890: 2868 135d 6814 5d68 155d 6816 5d68 175d  (h.]h.]h.]h.]h.]
-000048a0: 7568 1f6a 6803 0000 6818 5d72 6f03 0000  uh.jh...h.]ro...
-000048b0: 6a58 0200 0029 8172 7003 0000 7d72 7103  jX...).rp...}rq.
-000048c0: 0000 2868 1055 0068 117d 7272 0300 0028  ..(h.U.h.}rr...(
-000048d0: 550a 616e 6368 6f72 6e61 6d65 5500 5506  U.anchornameU.U.
-000048e0: 7265 6675 7269 683d 6816 5d68 155d 6813  refurih=h.]h.]h.
-000048f0: 5d68 145d 6817 5d55 0869 6e74 6572 6e61  ]h.]h.]U.interna
-00004900: 6c88 7568 1f6a 6c03 0000 6818 5d72 7303  l.uh.jl...h.]rs.
-00004910: 0000 681a 5815 0000 004f 7665 7276 6965  ..h.X....Overvie
-00004920: 7720 616e 6420 5475 746f 7269 616c 7274  w and Tutorialrt
-00004930: 0300 0085 8172 7503 0000 7d72 7603 0000  .....ru...}rv...
-00004940: 2868 1068 4568 1f6a 7003 0000 7562 6168  (h.hEh.jp...ubah
-00004950: 206a 6002 0000 7562 6168 206a 6102 0000   j`...ubah ja...
-00004960: 7562 6a49 0200 0029 8172 7703 0000 7d72  ubjI...).rw...}r
-00004970: 7803 0000 2868 1055 0068 117d 7279 0300  x...(h.U.h.}ry..
-00004980: 0028 6813 5d68 145d 6815 5d68 165d 6817  .(h.]h.]h.]h.]h.
-00004990: 5d75 681f 6a68 0300 0068 185d 727a 0300  ]uh.jh...h.]rz..
-000049a0: 0028 6a4e 0200 0029 8172 7b03 0000 7d72  .(jN...).r{...}r
-000049b0: 7c03 0000 2868 1055 0068 117d 727d 0300  |...(h.U.h.}r}..
-000049c0: 0028 6813 5d68 145d 6815 5d68 165d 6817  .(h.]h.]h.]h.]h.
-000049d0: 5d75 681f 6a77 0300 0068 185d 727e 0300  ]uh.jw...h.]r~..
-000049e0: 006a 5302 0000 2981 727f 0300 007d 7280  .jS...).r....}r.
-000049f0: 0300 0028 6810 5500 6811 7d72 8103 0000  ...(h.U.h.}r....
-00004a00: 2868 135d 6814 5d68 155d 6816 5d68 175d  (h.]h.]h.]h.]h.]
-00004a10: 7568 1f6a 7b03 0000 6818 5d72 8203 0000  uh.j{...h.]r....
-00004a20: 6a58 0200 0029 8172 8303 0000 7d72 8403  jX...).r....}r..
-00004a30: 0000 2868 1055 0068 117d 7285 0300 0028  ..(h.U.h.}r....(
-00004a40: 550a 616e 6368 6f72 6e61 6d65 550d 2369  U.anchornameU.#i
-00004a50: 6e74 726f 6475 6374 696f 6e55 0672 6566  ntroductionU.ref
-00004a60: 7572 6968 3d68 165d 6815 5d68 135d 6814  urih=h.]h.]h.]h.
-00004a70: 5d68 175d 5508 696e 7465 726e 616c 8875  ]h.]U.internal.u
-00004a80: 681f 6a7f 0300 0068 185d 7286 0300 0068  h.j....h.]r....h
-00004a90: 1a58 0c00 0000 496e 7472 6f64 7563 7469  .X....Introducti
-00004aa0: 6f6e 7287 0300 0085 8172 8803 0000 7d72  onr......r....}r
-00004ab0: 8903 0000 2868 1058 0c00 0000 496e 7472  ....(h.X....Intr
-00004ac0: 6f64 7563 7469 6f6e 728a 0300 0068 1f6a  oductionr....h.j
-00004ad0: 8303 0000 7562 6168 206a 6002 0000 7562  ....ubah j`...ub
-00004ae0: 6168 206a 6102 0000 7562 6168 206a 7802  ah ja...ubah jx.
-00004af0: 0000 7562 6a4e 0200 0029 8172 8b03 0000  ..ubjN...).r....
-00004b00: 7d72 8c03 0000 2868 1055 0068 117d 728d  }r....(h.U.h.}r.
-00004b10: 0300 0028 6813 5d68 145d 6815 5d68 165d  ...(h.]h.]h.]h.]
-00004b20: 6817 5d75 681f 6a77 0300 0068 185d 728e  h.]uh.jw...h.]r.
-00004b30: 0300 006a 5302 0000 2981 728f 0300 007d  ...jS...).r....}
-00004b40: 7290 0300 0028 6810 5500 6811 7d72 9103  r....(h.U.h.}r..
-00004b50: 0000 2868 135d 6814 5d68 155d 6816 5d68  ..(h.]h.]h.]h.]h
-00004b60: 175d 7568 1f6a 8b03 0000 6818 5d72 9203  .]uh.j....h.]r..
-00004b70: 0000 6a58 0200 0029 8172 9303 0000 7d72  ..jX...).r....}r
-00004b80: 9403 0000 2868 1055 0068 117d 7295 0300  ....(h.U.h.}r...
-00004b90: 0028 550a 616e 6368 6f72 6e61 6d65 5530  .(U.anchornameU0
-00004ba0: 2367 6175 7373 6961 6e2d 7261 6e64 6f6d  #gaussian-random
-00004bb0: 2d76 6172 6961 626c 6573 2d61 6e64 2d65  -variables-and-e
-00004bc0: 7272 6f72 2d70 726f 7061 6761 7469 6f6e  rror-propagation
-00004bd0: 5506 7265 6675 7269 683d 6816 5d68 155d  U.refurih=h.]h.]
-00004be0: 6813 5d68 145d 6817 5d55 0869 6e74 6572  h.]h.]h.]U.inter
-00004bf0: 6e61 6c88 7568 1f6a 8f03 0000 6818 5d72  nal.uh.j....h.]r
-00004c00: 9603 0000 681a 582f 0000 0047 6175 7373  ....h.X/...Gauss
-00004c10: 6961 6e20 5261 6e64 6f6d 2056 6172 6961  ian Random Varia
-00004c20: 626c 6573 2061 6e64 2045 7272 6f72 2050  bles and Error P
-00004c30: 726f 7061 6761 7469 6f6e 7297 0300 0085  ropagationr.....
-00004c40: 8172 9803 0000 7d72 9903 0000 2868 1058  .r....}r....(h.X
-00004c50: 2f00 0000 4761 7573 7369 616e 2052 616e  /...Gaussian Ran
-00004c60: 646f 6d20 5661 7269 6162 6c65 7320 616e  dom Variables an
-00004c70: 6420 4572 726f 7220 5072 6f70 6167 6174  d Error Propagat
-00004c80: 696f 6e72 9a03 0000 681f 6a93 0300 0075  ionr....h.j....u
-00004c90: 6261 6820 6a60 0200 0075 6261 6820 6a61  bah j`...ubah ja
-00004ca0: 0200 0075 6261 6820 6a78 0200 0075 626a  ...ubah jx...ubj
-00004cb0: 4e02 0000 2981 729b 0300 007d 729c 0300  N...).r....}r...
-00004cc0: 0028 6810 5500 6811 7d72 9d03 0000 2868  .(h.U.h.}r....(h
-00004cd0: 135d 6814 5d68 155d 6816 5d68 175d 7568  .]h.]h.]h.]h.]uh
-00004ce0: 1f6a 7703 0000 6818 5d72 9e03 0000 6a53  .jw...h.]r....jS
-00004cf0: 0200 0029 8172 9f03 0000 7d72 a003 0000  ...).r....}r....
-00004d00: 2868 1055 0068 117d 72a1 0300 0028 6813  (h.U.h.}r....(h.
-00004d10: 5d68 145d 6815 5d68 165d 6817 5d75 681f  ]h.]h.]h.]h.]uh.
-00004d20: 6a9b 0300 0068 185d 72a2 0300 006a 5802  j....h.]r....jX.
-00004d30: 0000 2981 72a3 0300 007d 72a4 0300 0028  ..).r....}r....(
-00004d40: 6810 5500 6811 7d72 a503 0000 2855 0a61  h.U.h.}r....(U.a
-00004d50: 6e63 686f 726e 616d 6555 0b23 6261 7369  nchornameU.#basi
-00004d60: 632d 6669 7473 5506 7265 6675 7269 683d  c-fitsU.refurih=
-00004d70: 6816 5d68 155d 6813 5d68 145d 6817 5d55  h.]h.]h.]h.]h.]U
-00004d80: 0869 6e74 6572 6e61 6c88 7568 1f6a 9f03  .internal.uh.j..
-00004d90: 0000 6818 5d72 a603 0000 681a 580a 0000  ..h.]r....h.X...
-00004da0: 0042 6173 6963 2046 6974 7372 a703 0000  .Basic Fitsr....
-00004db0: 8581 72a8 0300 007d 72a9 0300 0028 6810  ..r....}r....(h.
-00004dc0: 580a 0000 0042 6173 6963 2046 6974 7372  X....Basic Fitsr
-00004dd0: aa03 0000 681f 6aa3 0300 0075 6261 6820  ....h.j....ubah 
-00004de0: 6a60 0200 0075 6261 6820 6a61 0200 0075  j`...ubah ja...u
-00004df0: 6261 6820 6a78 0200 0075 626a 4e02 0000  bah jx...ubjN...
-00004e00: 2981 72ab 0300 007d 72ac 0300 0028 6810  ).r....}r....(h.
-00004e10: 5500 6811 7d72 ad03 0000 2868 135d 6814  U.h.}r....(h.]h.
-00004e20: 5d68 155d 6816 5d68 175d 7568 1f6a 7703  ]h.]h.]h.]uh.jw.
-00004e30: 0000 6818 5d72 ae03 0000 6a53 0200 0029  ..h.]r....jS...)
-00004e40: 8172 af03 0000 7d72 b003 0000 2868 1055  .r....}r....(h.U
-00004e50: 0068 117d 72b1 0300 0028 6813 5d68 145d  .h.}r....(h.]h.]
-00004e60: 6815 5d68 165d 6817 5d75 681f 6aab 0300  h.]h.]h.]uh.j...
-00004e70: 0068 185d 72b2 0300 006a 5802 0000 2981  .h.]r....jX...).
-00004e80: 72b3 0300 007d 72b4 0300 0028 6810 5500  r....}r....(h.U.
-00004e90: 6811 7d72 b503 0000 2855 0a61 6e63 686f  h.}r....(U.ancho
-00004ea0: 726e 616d 6555 1d23 6368 6169 6e65 642d  rnameU.#chained-
-00004eb0: 6669 7473 2d6c 6172 6765 2d64 6174 612d  fits-large-data-
-00004ec0: 7365 7473 5506 7265 6675 7269 683d 6816  setsU.refurih=h.
-00004ed0: 5d68 155d 6813 5d68 145d 6817 5d55 0869  ]h.]h.]h.]h.]U.i
-00004ee0: 6e74 6572 6e61 6c88 7568 1f6a af03 0000  nternal.uh.j....
-00004ef0: 6818 5d72 b603 0000 681a 581d 0000 0043  h.]r....h.X....C
-00004f00: 6861 696e 6564 2046 6974 733b 204c 6172  hained Fits; Lar
-00004f10: 6765 2044 6174 6120 5365 7473 72b7 0300  ge Data Setsr...
-00004f20: 0085 8172 b803 0000 7d72 b903 0000 2868  ...r....}r....(h
-00004f30: 1058 1d00 0000 4368 6169 6e65 6420 4669  .X....Chained Fi
-00004f40: 7473 3b20 4c61 7267 6520 4461 7461 2053  ts; Large Data S
-00004f50: 6574 7372 ba03 0000 681f 6ab3 0300 0075  etsr....h.j....u
-00004f60: 6261 6820 6a60 0200 0075 6261 6820 6a61  bah j`...ubah ja
-00004f70: 0200 0075 6261 6820 6a78 0200 0075 626a  ...ubah jx...ubj
-00004f80: 4e02 0000 2981 72bb 0300 007d 72bc 0300  N...).r....}r...
-00004f90: 0028 6810 5500 6811 7d72 bd03 0000 2868  .(h.U.h.}r....(h
-00004fa0: 135d 6814 5d68 155d 6816 5d68 175d 7568  .]h.]h.]h.]h.]uh
-00004fb0: 1f6a 7703 0000 6818 5d72 be03 0000 6a53  .jw...h.]r....jS
-00004fc0: 0200 0029 8172 bf03 0000 7d72 c003 0000  ...).r....}r....
-00004fd0: 2868 1055 0068 117d 72c1 0300 0028 6813  (h.U.h.}r....(h.
-00004fe0: 5d68 145d 6815 5d68 165d 6817 5d75 681f  ]h.]h.]h.]h.]uh.
-00004ff0: 6abb 0300 0068 185d 72c2 0300 006a 5802  j....h.]r....jX.
-00005000: 0000 2981 72c3 0300 007d 72c4 0300 0028  ..).r....}r....(
-00005010: 6810 5500 6811 7d72 c503 0000 2855 0a61  h.U.h.}r....(U.a
-00005020: 6e63 686f 726e 616d 6555 0d23 782d 6861  nchornameU.#x-ha
-00005030: 732d 6572 726f 7273 5506 7265 6675 7269  s-errorsU.refuri
-00005040: 683d 6816 5d68 155d 6813 5d68 145d 6817  h=h.]h.]h.]h.]h.
-00005050: 5d55 0869 6e74 6572 6e61 6c88 7568 1f6a  ]U.internal.uh.j
-00005060: bf03 0000 6818 5d72 c603 0000 2868 3029  ....h.]r....(h0)
-00005070: 8172 c703 0000 7d72 c803 0000 2868 1058  .r....}r....(h.X
-00005080: 0500 0000 6060 7860 6072 c903 0000 681f  ....``x``r....h.
-00005090: 6ac3 0300 006a 6902 0000 4e68 2068 3868  j....ji...Nh h8h
-000050a0: 117d 72ca 0300 0028 6813 5d68 145d 6815  .}r....(h.]h.]h.
-000050b0: 5d68 165d 6817 5d75 6a76 0200 004e 6818  ]h.]h.]ujv...Nh.
-000050c0: 5d72 cb03 0000 681a 5801 0000 0078 8581  ]r....h.X....x..
-000050d0: 72cc 0300 007d 72cd 0300 0028 6810 5500  r....}r....(h.U.
-000050e0: 681f 6ac7 0300 0075 6261 7562 681a 580b  h.j....ubaubh.X.
-000050f0: 0000 0020 6861 7320 4572 726f 7273 72ce  ... has Errorsr.
-00005100: 0300 0085 8172 cf03 0000 7d72 d003 0000  .....r....}r....
-00005110: 2868 1058 0b00 0000 2068 6173 2045 7272  (h.X.... has Err
-00005120: 6f72 7372 d103 0000 681f 6ac3 0300 0075  orsr....h.j....u
-00005130: 6265 6820 6a60 0200 0075 6261 6820 6a61  beh j`...ubah ja
-00005140: 0200 0075 6261 6820 6a78 0200 0075 626a  ...ubah jx...ubj
-00005150: 4e02 0000 2981 72d2 0300 007d 72d3 0300  N...).r....}r...
-00005160: 0028 6810 5500 6811 7d72 d403 0000 2868  .(h.U.h.}r....(h
-00005170: 135d 6814 5d68 155d 6816 5d68 175d 7568  .]h.]h.]h.]h.]uh
-00005180: 1f6a 7703 0000 6818 5d72 d503 0000 6a53  .jw...h.]r....jS
-00005190: 0200 0029 8172 d603 0000 7d72 d703 0000  ...).r....}r....
-000051a0: 2868 1055 0068 117d 72d8 0300 0028 6813  (h.U.h.}r....(h.
-000051b0: 5d68 145d 6815 5d68 165d 6817 5d75 681f  ]h.]h.]h.]h.]uh.
-000051c0: 6ad2 0300 0068 185d 72d9 0300 006a 5802  j....h.]r....jX.
-000051d0: 0000 2981 72da 0300 007d 72db 0300 0028  ..).r....}r....(
-000051e0: 6810 5500 6811 7d72 dc03 0000 2855 0a61  h.U.h.}r....(U.a
-000051f0: 6e63 686f 726e 616d 6555 2c23 636f 7272  nchornameU,#corr
-00005200: 656c 6174 6564 2d70 6172 616d 6574 6572  elated-parameter
-00005210: 732d 6761 7573 7369 616e 2d62 6179 6573  s-gaussian-bayes
-00005220: 2d66 6163 746f 7255 0672 6566 7572 6968  -factorU.refurih
-00005230: 3d68 165d 6815 5d68 135d 6814 5d68 175d  =h.]h.]h.]h.]h.]
-00005240: 5508 696e 7465 726e 616c 8875 681f 6ad6  U.internal.uh.j.
-00005250: 0300 0068 185d 72dd 0300 0068 1a58 2c00  ...h.]r....h.X,.
-00005260: 0000 436f 7272 656c 6174 6564 2050 6172  ..Correlated Par
-00005270: 616d 6574 6572 733b 2047 6175 7373 6961  ameters; Gaussia
-00005280: 6e20 4261 7965 7320 4661 6374 6f72 72de  n Bayes Factorr.
-00005290: 0300 0085 8172 df03 0000 7d72 e003 0000  .....r....}r....
-000052a0: 2868 1058 2c00 0000 436f 7272 656c 6174  (h.X,...Correlat
-000052b0: 6564 2050 6172 616d 6574 6572 733b 2047  ed Parameters; G
-000052c0: 6175 7373 6961 6e20 4261 7965 7320 4661  aussian Bayes Fa
-000052d0: 6374 6f72 72e1 0300 0068 1f6a da03 0000  ctorr....h.j....
-000052e0: 7562 6168 206a 6002 0000 7562 6168 206a  ubah j`...ubah j
-000052f0: 6102 0000 7562 6168 206a 7802 0000 7562  a...ubah jx...ub
-00005300: 6a4e 0200 0029 8172 e203 0000 7d72 e303  jN...).r....}r..
-00005310: 0000 2868 1055 0068 117d 72e4 0300 0028  ..(h.U.h.}r....(
-00005320: 6813 5d68 145d 6815 5d68 165d 6817 5d75  h.]h.]h.]h.]h.]u
-00005330: 681f 6a77 0300 0068 185d 72e5 0300 006a  h.jw...h.]r....j
-00005340: 5302 0000 2981 72e6 0300 007d 72e7 0300  S...).r....}r...
-00005350: 0028 6810 5500 6811 7d72 e803 0000 2868  .(h.U.h.}r....(h
-00005360: 135d 6814 5d68 155d 6816 5d68 175d 7568  .]h.]h.]h.]h.]uh
-00005370: 1f6a e203 0000 6818 5d72 e903 0000 6a58  .j....h.]r....jX
-00005380: 0200 0029 8172 ea03 0000 7d72 eb03 0000  ...).r....}r....
-00005390: 2868 1055 0068 117d 72ec 0300 0028 550a  (h.U.h.}r....(U.
-000053a0: 616e 6368 6f72 6e61 6d65 551f 2379 2d68  anchornameU.#y-h
-000053b0: 6173 2d6e 6f2d 6572 726f 722d 6d61 7267  as-no-error-marg
-000053c0: 696e 616c 697a 6174 696f 6e55 0672 6566  inalizationU.ref
-000053d0: 7572 6968 3d68 165d 6815 5d68 135d 6814  urih=h.]h.]h.]h.
-000053e0: 5d68 175d 5508 696e 7465 726e 616c 8875  ]h.]U.internal.u
-000053f0: 681f 6ae6 0300 0068 185d 72ed 0300 0028  h.j....h.]r....(
-00005400: 6830 2981 72ee 0300 007d 72ef 0300 0028  h0).r....}r....(
-00005410: 6810 5805 0000 0060 6079 6060 72f0 0300  h.X....``y``r...
-00005420: 0068 1f6a ea03 0000 6a69 0200 004e 6820  .h.j....ji...Nh 
-00005430: 6838 6811 7d72 f103 0000 2868 135d 6814  h8h.}r....(h.]h.
-00005440: 5d68 155d 6816 5d68 175d 756a 7602 0000  ]h.]h.]h.]ujv...
-00005450: 4e68 185d 72f2 0300 0068 1a58 0100 0000  Nh.]r....h.X....
-00005460: 7985 8172 f303 0000 7d72 f403 0000 2868  y..r....}r....(h
-00005470: 1055 0068 1f6a ee03 0000 7562 6175 6268  .U.h.j....ubaubh
-00005480: 1a58 1e00 0000 2068 6173 204e 6f20 4572  .X.... has No Er
-00005490: 726f 723b 204d 6172 6769 6e61 6c69 7a61  ror; Marginaliza
-000054a0: 7469 6f6e 72f5 0300 0085 8172 f603 0000  tionr......r....
-000054b0: 7d72 f703 0000 2868 1058 1e00 0000 2068  }r....(h.X.... h
-000054c0: 6173 204e 6f20 4572 726f 723b 204d 6172  as No Error; Mar
-000054d0: 6769 6e61 6c69 7a61 7469 6f6e 72f8 0300  ginalizationr...
-000054e0: 0068 1f6a ea03 0000 7562 6568 206a 6002  .h.j....ubeh j`.
-000054f0: 0000 7562 6168 206a 6102 0000 7562 6168  ..ubah ja...ubah
-00005500: 206a 7802 0000 7562 6a4e 0200 0029 8172   jx...ubjN...).r
-00005510: f903 0000 7d72 fa03 0000 2868 1055 0068  ....}r....(h.U.h
-00005520: 117d 72fb 0300 0028 6813 5d68 145d 6815  .}r....(h.]h.]h.
-00005530: 5d68 165d 6817 5d75 681f 6a77 0300 0068  ]h.]h.]uh.jw...h
-00005540: 185d 72fc 0300 006a 5302 0000 2981 72fd  .]r....jS...).r.
-00005550: 0300 007d 72fe 0300 0028 6810 5500 6811  ...}r....(h.U.h.
-00005560: 7d72 ff03 0000 2868 135d 6814 5d68 155d  }r....(h.]h.]h.]
-00005570: 6816 5d68 175d 7568 1f6a f903 0000 6818  h.]h.]uh.j....h.
-00005580: 5d72 0004 0000 6a58 0200 0029 8172 0104  ]r....jX...).r..
-00005590: 0000 7d72 0204 0000 2868 1055 0068 117d  ..}r....(h.U.h.}
-000055a0: 7203 0400 0028 550a 616e 6368 6f72 6e61  r....(U.anchorna
-000055b0: 6d65 551c 2373 7664 2d63 7574 732d 616e  meU.#svd-cuts-an
-000055c0: 642d 726f 756e 646f 6666 2d65 7272 6f72  d-roundoff-error
-000055d0: 5506 7265 6675 7269 683d 6816 5d68 155d  U.refurih=h.]h.]
-000055e0: 6813 5d68 145d 6817 5d55 0869 6e74 6572  h.]h.]h.]U.inter
-000055f0: 6e61 6c88 7568 1f6a fd03 0000 6818 5d72  nal.uh.j....h.]r
-00005600: 0404 0000 681a 581b 0000 0053 5644 2043  ....h.X....SVD C
-00005610: 7574 7320 616e 6420 526f 756e 646f 6666  uts and Roundoff
-00005620: 2045 7272 6f72 7205 0400 0085 8172 0604   Errorr......r..
-00005630: 0000 7d72 0704 0000 2868 1058 1b00 0000  ..}r....(h.X....
-00005640: 5356 4420 4375 7473 2061 6e64 2052 6f75  SVD Cuts and Rou
-00005650: 6e64 6f66 6620 4572 726f 7272 0804 0000  ndoff Errorr....
-00005660: 681f 6a01 0400 0075 6261 6820 6a60 0200  h.j....ubah j`..
-00005670: 0075 6261 6820 6a61 0200 0075 6261 6820  .ubah ja...ubah 
-00005680: 6a78 0200 0075 626a 4e02 0000 2981 7209  jx...ubjN...).r.
-00005690: 0400 007d 720a 0400 0028 6810 5500 6811  ...}r....(h.U.h.
-000056a0: 7d72 0b04 0000 2868 135d 6814 5d68 155d  }r....(h.]h.]h.]
-000056b0: 6816 5d68 175d 7568 1f6a 7703 0000 6818  h.]h.]uh.jw...h.
-000056c0: 5d72 0c04 0000 6a53 0200 0029 8172 0d04  ]r....jS...).r..
-000056d0: 0000 7d72 0e04 0000 2868 1055 0068 117d  ..}r....(h.U.h.}
-000056e0: 720f 0400 0028 6813 5d68 145d 6815 5d68  r....(h.]h.]h.]h
-000056f0: 165d 6817 5d75 681f 6a09 0400 0068 185d  .]h.]uh.j....h.]
-00005700: 7210 0400 006a 5802 0000 2981 7211 0400  r....jX...).r...
-00005710: 007d 7212 0400 0028 6810 5500 6811 7d72  .}r....(h.U.h.}r
-00005720: 1304 0000 2855 0a61 6e63 686f 726e 616d  ....(U.anchornam
-00005730: 6555 1523 792d 6861 732d 756e 6b6e 6f77  eU.#y-has-unknow
-00005740: 6e2d 6572 726f 7273 5506 7265 6675 7269  n-errorsU.refuri
-00005750: 683d 6816 5d68 155d 6813 5d68 145d 6817  h=h.]h.]h.]h.]h.
-00005760: 5d55 0869 6e74 6572 6e61 6c88 7568 1f6a  ]U.internal.uh.j
-00005770: 0d04 0000 6818 5d72 1404 0000 2868 3029  ....h.]r....(h0)
-00005780: 8172 1504 0000 7d72 1604 0000 2868 1058  .r....}r....(h.X
-00005790: 0500 0000 6060 7960 6072 1704 0000 681f  ....``y``r....h.
-000057a0: 6a11 0400 006a 6902 0000 4e68 2068 3868  j....ji...Nh h8h
-000057b0: 117d 7218 0400 0028 6813 5d68 145d 6815  .}r....(h.]h.]h.
-000057c0: 5d68 165d 6817 5d75 6a76 0200 004e 6818  ]h.]h.]ujv...Nh.
-000057d0: 5d72 1904 0000 681a 5801 0000 0079 8581  ]r....h.X....y..
-000057e0: 721a 0400 007d 721b 0400 0028 6810 5500  r....}r....(h.U.
-000057f0: 681f 6a15 0400 0075 6261 7562 681a 5813  h.j....ubaubh.X.
-00005800: 0000 0020 6861 7320 556e 6b6e 6f77 6e20  ... has Unknown 
-00005810: 4572 726f 7273 721c 0400 0085 8172 1d04  Errorsr......r..
-00005820: 0000 7d72 1e04 0000 2868 1058 1300 0000  ..}r....(h.X....
-00005830: 2068 6173 2055 6e6b 6e6f 776e 2045 7272   has Unknown Err
-00005840: 6f72 7372 1f04 0000 681f 6a11 0400 0075  orsr....h.j....u
-00005850: 6265 6820 6a60 0200 0075 6261 6820 6a61  beh j`...ubah ja
-00005860: 0200 0075 6261 6820 6a78 0200 0075 626a  ...ubah jx...ubj
-00005870: 4e02 0000 2981 7220 0400 007d 7221 0400  N...).r ...}r!..
-00005880: 0028 6810 5500 6811 7d72 2204 0000 2868  .(h.U.h.}r"...(h
-00005890: 135d 6814 5d68 155d 6816 5d68 175d 7568  .]h.]h.]h.]h.]uh
-000058a0: 1f6a 7703 0000 6818 5d72 2304 0000 6a53  .jw...h.]r#...jS
-000058b0: 0200 0029 8172 2404 0000 7d72 2504 0000  ...).r$...}r%...
-000058c0: 2868 1055 0068 117d 7226 0400 0028 6813  (h.U.h.}r&...(h.
-000058d0: 5d68 145d 6815 5d68 165d 6817 5d75 681f  ]h.]h.]h.]h.]uh.
-000058e0: 6a20 0400 0068 185d 7227 0400 006a 5802  j ...h.]r'...jX.
-000058f0: 0000 2981 7228 0400 007d 7229 0400 0028  ..).r(...}r)...(
-00005900: 6810 5500 6811 7d72 2a04 0000 2855 0a61  h.U.h.}r*...(U.a
-00005910: 6e63 686f 726e 616d 6555 3123 7475 6e69  nchornameU1#tuni
-00005920: 6e67 2d70 7269 6f72 732d 7769 7468 2d74  ng-priors-with-t
-00005930: 6865 2d65 6d70 6972 6963 616c 2d62 6179  he-empirical-bay
-00005940: 6573 2d63 7269 7465 7269 6f6e 5506 7265  es-criterionU.re
-00005950: 6675 7269 683d 6816 5d68 155d 6813 5d68  furih=h.]h.]h.]h
-00005960: 145d 6817 5d55 0869 6e74 6572 6e61 6c88  .]h.]U.internal.
-00005970: 7568 1f6a 2404 0000 6818 5d72 2b04 0000  uh.j$...h.]r+...
-00005980: 681a 5830 0000 0054 756e 696e 6720 5072  h.X0...Tuning Pr
-00005990: 696f 7273 2077 6974 6820 7468 6520 456d  iors with the Em
-000059a0: 7069 7269 6361 6c20 4261 7965 7320 4372  pirical Bayes Cr
-000059b0: 6974 6572 696f 6e72 2c04 0000 8581 722d  iterionr,.....r-
-000059c0: 0400 007d 722e 0400 0028 6810 5830 0000  ...}r....(h.X0..
-000059d0: 0054 756e 696e 6720 5072 696f 7273 2077  .Tuning Priors w
-000059e0: 6974 6820 7468 6520 456d 7069 7269 6361  ith the Empirica
-000059f0: 6c20 4261 7965 7320 4372 6974 6572 696f  l Bayes Criterio
-00005a00: 6e72 2f04 0000 681f 6a28 0400 0075 6261  nr/...h.j(...uba
-00005a10: 6820 6a60 0200 0075 6261 6820 6a61 0200  h j`...ubah ja..
-00005a20: 0075 6261 6820 6a78 0200 0075 626a 4e02  .ubah jx...ubjN.
-00005a30: 0000 2981 7230 0400 007d 7231 0400 0028  ..).r0...}r1...(
-00005a40: 6810 5500 6811 7d72 3204 0000 2868 135d  h.U.h.}r2...(h.]
-00005a50: 6814 5d68 155d 6816 5d68 175d 7568 1f6a  h.]h.]h.]h.]uh.j
-00005a60: 7703 0000 6818 5d72 3304 0000 6a53 0200  w...h.]r3...jS..
-00005a70: 0029 8172 3404 0000 7d72 3504 0000 2868  .).r4...}r5...(h
-00005a80: 1055 0068 117d 7236 0400 0028 6813 5d68  .U.h.}r6...(h.]h
-00005a90: 145d 6815 5d68 165d 6817 5d75 681f 6a30  .]h.]h.]h.]uh.j0
-00005aa0: 0400 0068 185d 7237 0400 006a 5802 0000  ...h.]r7...jX...
-00005ab0: 2981 7238 0400 007d 7239 0400 0028 6810  ).r8...}r9...(h.
-00005ac0: 5500 6811 7d72 3a04 0000 2855 0a61 6e63  U.h.}r:...(U.anc
-00005ad0: 686f 726e 616d 6555 2823 706f 7369 7469  hornameU(#positi
-00005ae0: 7665 2d70 6172 616d 6574 6572 732d 6e6f  ve-parameters-no
-00005af0: 6e2d 6761 7573 7369 616e 2d70 7269 6f72  n-gaussian-prior
-00005b00: 7355 0672 6566 7572 6968 3d68 165d 6815  sU.refurih=h.]h.
-00005b10: 5d68 135d 6814 5d68 175d 5508 696e 7465  ]h.]h.]h.]U.inte
-00005b20: 726e 616c 8875 681f 6a34 0400 0068 185d  rnal.uh.j4...h.]
-00005b30: 723b 0400 0068 1a58 2800 0000 506f 7369  r;...h.X(...Posi
-00005b40: 7469 7665 2050 6172 616d 6574 6572 733b  tive Parameters;
-00005b50: 204e 6f6e 2d47 6175 7373 6961 6e20 5072   Non-Gaussian Pr
-00005b60: 696f 7273 723c 0400 0085 8172 3d04 0000  iorsr<.....r=...
-00005b70: 7d72 3e04 0000 2868 1058 2800 0000 506f  }r>...(h.X(...Po
-00005b80: 7369 7469 7665 2050 6172 616d 6574 6572  sitive Parameter
-00005b90: 733b 204e 6f6e 2d47 6175 7373 6961 6e20  s; Non-Gaussian 
-00005ba0: 5072 696f 7273 723f 0400 0068 1f6a 3804  Priorsr?...h.j8.
-00005bb0: 0000 7562 6168 206a 6002 0000 7562 6168  ..ubah j`...ubah
-00005bc0: 206a 6102 0000 7562 6168 206a 7802 0000   ja...ubah jx...
-00005bd0: 7562 6a4e 0200 0029 8172 4004 0000 7d72  ubjN...).r@...}r
-00005be0: 4104 0000 2868 1055 0068 117d 7242 0400  A...(h.U.h.}rB..
-00005bf0: 0028 6813 5d68 145d 6815 5d68 165d 6817  .(h.]h.]h.]h.]h.
-00005c00: 5d75 681f 6a77 0300 0068 185d 7243 0400  ]uh.jw...h.]rC..
-00005c10: 006a 5302 0000 2981 7244 0400 007d 7245  .jS...).rD...}rE
-00005c20: 0400 0028 6810 5500 6811 7d72 4604 0000  ...(h.U.h.}rF...
-00005c30: 2868 135d 6814 5d68 155d 6816 5d68 175d  (h.]h.]h.]h.]h.]
-00005c40: 7568 1f6a 4004 0000 6818 5d72 4704 0000  uh.j@...h.]rG...
-00005c50: 6a58 0200 0029 8172 4804 0000 7d72 4904  jX...).rH...}rI.
-00005c60: 0000 2868 1055 0068 117d 724a 0400 0028  ..(h.U.h.}rJ...(
-00005c70: 550a 616e 6368 6f72 6e61 6d65 550f 2366  U.anchornameU.#f
-00005c80: 6173 7465 722d 6669 7474 6572 7355 0672  aster-fittersU.r
-00005c90: 6566 7572 6968 3d68 165d 6815 5d68 135d  efurih=h.]h.]h.]
-00005ca0: 6814 5d68 175d 5508 696e 7465 726e 616c  h.]h.]U.internal
-00005cb0: 8875 681f 6a44 0400 0068 185d 724b 0400  .uh.jD...h.]rK..
-00005cc0: 0068 1a58 0e00 0000 4661 7374 6572 2046  .h.X....Faster F
-00005cd0: 6974 7465 7273 724c 0400 0085 8172 4d04  ittersrL.....rM.
-00005ce0: 0000 7d72 4e04 0000 2868 1058 0e00 0000  ..}rN...(h.X....
-00005cf0: 4661 7374 6572 2046 6974 7465 7273 724f  Faster FittersrO
-00005d00: 0400 0068 1f6a 4804 0000 7562 6168 206a  ...h.jH...ubah j
-00005d10: 6002 0000 7562 6168 206a 6102 0000 7562  `...ubah ja...ub
-00005d20: 6168 206a 7802 0000 7562 6a4e 0200 0029  ah jx...ubjN...)
-00005d30: 8172 5004 0000 7d72 5104 0000 2868 1055  .rP...}rQ...(h.U
-00005d40: 0068 117d 7252 0400 0028 6813 5d68 145d  .h.}rR...(h.]h.]
-00005d50: 6815 5d68 165d 6817 5d75 681f 6a77 0300  h.]h.]h.]uh.jw..
-00005d60: 0068 185d 7253 0400 006a 5302 0000 2981  .h.]rS...jS...).
-00005d70: 7254 0400 007d 7255 0400 0028 6810 5500  rT...}rU...(h.U.
-00005d80: 6811 7d72 5604 0000 2868 135d 6814 5d68  h.}rV...(h.]h.]h
-00005d90: 155d 6816 5d68 175d 7568 1f6a 5004 0000  .]h.]h.]uh.jP...
-00005da0: 6818 5d72 5704 0000 6a58 0200 0029 8172  h.]rW...jX...).r
-00005db0: 5804 0000 7d72 5904 0000 2868 1055 0068  X...}rY...(h.U.h
-00005dc0: 117d 725a 0400 0028 550a 616e 6368 6f72  .}rZ...(U.anchor
-00005dd0: 6e61 6d65 551e 2364 6562 7567 6769 6e67  nameU.#debugging
-00005de0: 2d61 6e64 2d74 726f 7562 6c65 7368 6f6f  -and-troubleshoo
-00005df0: 7469 6e67 5506 7265 6675 7269 683d 6816  tingU.refurih=h.
-00005e00: 5d68 155d 6813 5d68 145d 6817 5d55 0869  ]h.]h.]h.]h.]U.i
-00005e10: 6e74 6572 6e61 6c88 7568 1f6a 5404 0000  nternal.uh.jT...
-00005e20: 6818 5d72 5b04 0000 681a 581d 0000 0044  h.]r[...h.X....D
-00005e30: 6562 7567 6769 6e67 2061 6e64 2054 726f  ebugging and Tro
-00005e40: 7562 6c65 7368 6f6f 7469 6e67 725c 0400  ubleshootingr\..
-00005e50: 0085 8172 5d04 0000 7d72 5e04 0000 2868  ...r]...}r^...(h
-00005e60: 1058 1d00 0000 4465 6275 6767 696e 6720  .X....Debugging 
-00005e70: 616e 6420 5472 6f75 626c 6573 686f 6f74  and Troubleshoot
-00005e80: 696e 6772 5f04 0000 681f 6a58 0400 0075  ingr_...h.jX...u
-00005e90: 6261 6820 6a60 0200 0075 6261 6820 6a61  bah j`...ubah ja
-00005ea0: 0200 0075 6261 6820 6a78 0200 0075 6265  ...ubah jx...ube
-00005eb0: 6820 6a77 0200 0075 6265 6820 6a78 0200  h jw...ubeh jx..
-00005ec0: 0075 6261 6820 6a77 0200 0075 6268 466a  .ubah jw...ubhFj
-00005ed0: 4902 0000 2981 7260 0400 007d 7261 0400  I...).r`...}ra..
-00005ee0: 0028 6810 5500 6811 7d72 6204 0000 2868  .(h.U.h.}rb...(h
-00005ef0: 135d 6814 5d68 155d 6816 5d68 175d 7568  .]h.]h.]h.]h.]uh
-00005f00: 185d 7263 0400 006a 4e02 0000 2981 7264  .]rc...jN...).rd
-00005f10: 0400 007d 7265 0400 0028 6810 5500 6811  ...}re...(h.U.h.
-00005f20: 7d72 6604 0000 2868 135d 6814 5d68 155d  }rf...(h.]h.]h.]
-00005f30: 6816 5d68 175d 7568 1f6a 6004 0000 6818  h.]h.]uh.j`...h.
-00005f40: 5d72 6704 0000 286a 5302 0000 2981 7268  ]rg...(jS...).rh
-00005f50: 0400 007d 7269 0400 0028 6810 5500 6811  ...}ri...(h.U.h.
-00005f60: 7d72 6a04 0000 2868 135d 6814 5d68 155d  }rj...(h.]h.]h.]
-00005f70: 6816 5d68 175d 7568 1f6a 6404 0000 6818  h.]h.]uh.jd...h.
-00005f80: 5d72 6b04 0000 6a58 0200 0029 8172 6c04  ]rk...jX...).rl.
-00005f90: 0000 7d72 6d04 0000 2868 1055 0068 117d  ..}rm...(h.U.h.}
-00005fa0: 726e 0400 0028 550a 616e 6368 6f72 6e61  rn...(U.anchorna
-00005fb0: 6d65 5500 5506 7265 6675 7269 6846 6816  meU.U.refurihFh.
-00005fc0: 5d68 155d 6813 5d68 145d 6817 5d55 0869  ]h.]h.]h.]h.]U.i
-00005fd0: 6e74 6572 6e61 6c88 7568 1f6a 6804 0000  nternal.uh.jh...
-00005fe0: 6818 5d72 6f04 0000 681a 5820 0000 0043  h.]ro...h.X ...C
-00005ff0: 6173 6520 5374 7564 793a 2053 696d 706c  ase Study: Simpl
-00006000: 6520 4578 7472 6170 6f6c 6174 696f 6e72  e Extrapolationr
-00006010: 7004 0000 8581 7271 0400 007d 7272 0400  p.....rq...}rr..
-00006020: 0028 6810 684e 681f 6a6c 0400 0075 6261  .(h.hNh.jl...uba
-00006030: 6820 6a60 0200 0075 6261 6820 6a61 0200  h j`...ubah ja..
-00006040: 0075 626a 4902 0000 2981 7273 0400 007d  .ubjI...).rs...}
-00006050: 7274 0400 0028 6810 5500 6811 7d72 7504  rt...(h.U.h.}ru.
-00006060: 0000 2868 135d 6814 5d68 155d 6816 5d68  ..(h.]h.]h.]h.]h
-00006070: 175d 7568 1f6a 6404 0000 6818 5d72 7604  .]uh.jd...h.]rv.
-00006080: 0000 286a 4e02 0000 2981 7277 0400 007d  ..(jN...).rw...}
-00006090: 7278 0400 0028 6810 5500 6811 7d72 7904  rx...(h.U.h.}ry.
-000060a0: 0000 2868 135d 6814 5d68 155d 6816 5d68  ..(h.]h.]h.]h.]h
-000060b0: 175d 7568 1f6a 7304 0000 6818 5d72 7a04  .]uh.js...h.]rz.
-000060c0: 0000 6a53 0200 0029 8172 7b04 0000 7d72  ..jS...).r{...}r
-000060d0: 7c04 0000 2868 1055 0068 117d 727d 0400  |...(h.U.h.}r}..
-000060e0: 0028 6813 5d68 145d 6815 5d68 165d 6817  .(h.]h.]h.]h.]h.
-000060f0: 5d75 681f 6a77 0400 0068 185d 727e 0400  ]uh.jw...h.]r~..
-00006100: 006a 5802 0000 2981 727f 0400 007d 7280  .jX...).r....}r.
-00006110: 0400 0028 6810 5500 6811 7d72 8104 0000  ...(h.U.h.}r....
-00006120: 2855 0a61 6e63 686f 726e 616d 6555 0c23  (U.anchornameU.#
-00006130: 7468 652d 7072 6f62 6c65 6d55 0672 6566  the-problemU.ref
-00006140: 7572 6968 4668 165d 6815 5d68 135d 6814  urihFh.]h.]h.]h.
-00006150: 5d68 175d 5508 696e 7465 726e 616c 8875  ]h.]U.internal.u
-00006160: 681f 6a7b 0400 0068 185d 7282 0400 0068  h.j{...h.]r....h
-00006170: 1a58 0b00 0000 5468 6520 5072 6f62 6c65  .X....The Proble
-00006180: 6d72 8304 0000 8581 7284 0400 007d 7285  mr......r....}r.
-00006190: 0400 0028 6810 580b 0000 0054 6865 2050  ...(h.X....The P
-000061a0: 726f 626c 656d 681f 6a7f 0400 0075 6261  roblemh.j....uba
-000061b0: 6820 6a60 0200 0075 6261 6820 6a61 0200  h j`...ubah ja..
-000061c0: 0075 6261 6820 6a78 0200 0075 626a 4e02  .ubah jx...ubjN.
-000061d0: 0000 2981 7286 0400 007d 7287 0400 0028  ..).r....}r....(
-000061e0: 6810 5500 6811 7d72 8804 0000 2868 135d  h.U.h.}r....(h.]
-000061f0: 6814 5d68 155d 6816 5d68 175d 7568 1f6a  h.]h.]h.]h.]uh.j
-00006200: 7304 0000 6818 5d72 8904 0000 6a53 0200  s...h.]r....jS..
-00006210: 0029 8172 8a04 0000 7d72 8b04 0000 2868  .).r....}r....(h
-00006220: 1055 0068 117d 728c 0400 0028 6813 5d68  .U.h.}r....(h.]h
-00006230: 145d 6815 5d68 165d 6817 5d75 681f 6a86  .]h.]h.]h.]uh.j.
-00006240: 0400 0068 185d 728d 0400 006a 5802 0000  ...h.]r....jX...
-00006250: 2981 728e 0400 007d 728f 0400 0028 6810  ).r....}r....(h.
-00006260: 5500 6811 7d72 9004 0000 2855 0a61 6e63  U.h.}r....(U.anc
-00006270: 686f 726e 616d 6555 0f23 612d 6261 642d  hornameU.#a-bad-
-00006280: 736f 6c75 7469 6f6e 5506 7265 6675 7269  solutionU.refuri
-00006290: 6846 6816 5d68 155d 6813 5d68 145d 6817  hFh.]h.]h.]h.]h.
-000062a0: 5d55 0869 6e74 6572 6e61 6c88 7568 1f6a  ]U.internal.uh.j
-000062b0: 8a04 0000 6818 5d72 9104 0000 681a 580e  ....h.]r....h.X.
-000062c0: 0000 0041 2042 6164 2053 6f6c 7574 696f  ...A Bad Solutio
-000062d0: 6e72 9204 0000 8581 7293 0400 007d 7294  nr......r....}r.
-000062e0: 0400 0028 6810 580e 0000 0041 2042 6164  ...(h.X....A Bad
-000062f0: 2053 6f6c 7574 696f 6e68 1f6a 8e04 0000   Solutionh.j....
-00006300: 7562 6168 206a 6002 0000 7562 6168 206a  ubah j`...ubah j
-00006310: 6102 0000 7562 6168 206a 7802 0000 7562  a...ubah jx...ub
-00006320: 6a4e 0200 0029 8172 9504 0000 7d72 9604  jN...).r....}r..
-00006330: 0000 2868 1055 0068 117d 7297 0400 0028  ..(h.U.h.}r....(
-00006340: 6813 5d68 145d 6815 5d68 165d 6817 5d75  h.]h.]h.]h.]h.]u
-00006350: 681f 6a73 0400 0068 185d 7298 0400 006a  h.js...h.]r....j
-00006360: 5302 0000 2981 7299 0400 007d 729a 0400  S...).r....}r...
-00006370: 0028 6810 5500 6811 7d72 9b04 0000 2868  .(h.U.h.}r....(h
-00006380: 135d 6814 5d68 155d 6816 5d68 175d 7568  .]h.]h.]h.]h.]uh
-00006390: 1f6a 9504 0000 6818 5d72 9c04 0000 6a58  .j....h.]r....jX
-000063a0: 0200 0029 8172 9d04 0000 7d72 9e04 0000  ...).r....}r....
-000063b0: 2868 1055 0068 117d 729f 0400 0028 550a  (h.U.h.}r....(U.
-000063c0: 616e 6368 6f72 6e61 6d65 5519 2361 2d62  anchornameU.#a-b
-000063d0: 6574 7465 722d 736f 6c75 7469 6f6e 2d70  etter-solution-p
-000063e0: 7269 6f72 7355 0672 6566 7572 6968 4668  riorsU.refurihFh
-000063f0: 165d 6815 5d68 135d 6814 5d68 175d 5508  .]h.]h.]h.]h.]U.
-00006400: 696e 7465 726e 616c 8875 681f 6a99 0400  internal.uh.j...
-00006410: 0068 185d 72a0 0400 0068 1a58 1c00 0000  .h.]r....h.X....
-00006420: 4120 4265 7474 6572 2053 6f6c 7574 696f  A Better Solutio
-00006430: 6e20 e280 9420 5072 696f 7273 72a1 0400  n ... Priorsr...
-00006440: 0085 8172 a204 0000 7d72 a304 0000 2868  ...r....}r....(h
-00006450: 1058 1c00 0000 4120 4265 7474 6572 2053  .X....A Better S
-00006460: 6f6c 7574 696f 6e20 2d2d 2d20 5072 696f  olution --- Prio
-00006470: 7273 681f 6a9d 0400 0075 6261 6820 6a60  rsh.j....ubah j`
-00006480: 0200 0075 6261 6820 6a61 0200 0075 6261  ...ubah ja...uba
-00006490: 6820 6a78 0200 0075 626a 4e02 0000 2981  h jx...ubjN...).
-000064a0: 72a4 0400 007d 72a5 0400 0028 6810 5500  r....}r....(h.U.
-000064b0: 6811 7d72 a604 0000 2868 135d 6814 5d68  h.}r....(h.]h.]h
-000064c0: 155d 6816 5d68 175d 7568 1f6a 7304 0000  .]h.]h.]uh.js...
-000064d0: 6818 5d72 a704 0000 6a53 0200 0029 8172  h.]r....jS...).r
-000064e0: a804 0000 7d72 a904 0000 2868 1055 0068  ....}r....(h.U.h
-000064f0: 117d 72aa 0400 0028 6813 5d68 145d 6815  .}r....(h.]h.]h.
-00006500: 5d68 165d 6817 5d75 681f 6aa4 0400 0068  ]h.]h.]uh.j....h
-00006510: 185d 72ab 0400 006a 5802 0000 2981 72ac  .]r....jX...).r.
-00006520: 0400 007d 72ad 0400 0028 6810 5500 6811  ...}r....(h.U.h.
-00006530: 7d72 ae04 0000 2855 0a61 6e63 686f 726e  }r....(U.anchorn
-00006540: 616d 6555 0e23 6261 7965 732d 6661 6374  ameU.#bayes-fact
-00006550: 6f72 7355 0672 6566 7572 6968 4668 165d  orsU.refurihFh.]
-00006560: 6815 5d68 135d 6814 5d68 175d 5508 696e  h.]h.]h.]h.]U.in
-00006570: 7465 726e 616c 8875 681f 6aa8 0400 0068  ternal.uh.j....h
-00006580: 185d 72af 0400 0068 1a58 0d00 0000 4261  .]r....h.X....Ba
-00006590: 7965 7320 4661 6374 6f72 7372 b004 0000  yes Factorsr....
-000065a0: 8581 72b1 0400 007d 72b2 0400 0028 6810  ..r....}r....(h.
-000065b0: 580d 0000 0042 6179 6573 2046 6163 746f  X....Bayes Facto
-000065c0: 7273 681f 6aac 0400 0075 6261 6820 6a60  rsh.j....ubah j`
-000065d0: 0200 0075 6261 6820 6a61 0200 0075 6261  ...ubah ja...uba
-000065e0: 6820 6a78 0200 0075 626a 4e02 0000 2981  h jx...ubjN...).
-000065f0: 72b3 0400 007d 72b4 0400 0028 6810 5500  r....}r....(h.U.
-00006600: 6811 7d72 b504 0000 2868 135d 6814 5d68  h.}r....(h.]h.]h
-00006610: 155d 6816 5d68 175d 7568 1f6a 7304 0000  .]h.]h.]uh.js...
-00006620: 6818 5d72 b604 0000 6a53 0200 0029 8172  h.]r....jS...).r
-00006630: b704 0000 7d72 b804 0000 2868 1055 0068  ....}r....(h.U.h
-00006640: 117d 72b9 0400 0028 6813 5d68 145d 6815  .}r....(h.]h.]h.
-00006650: 5d68 165d 6817 5d75 681f 6ab3 0400 0068  ]h.]h.]uh.j....h
-00006660: 185d 72ba 0400 006a 5802 0000 2981 72bb  .]r....jX...).r.
-00006670: 0400 007d 72bc 0400 0028 6810 5500 6811  ...}r....(h.U.h.
-00006680: 7d72 bd04 0000 2855 0a61 6e63 686f 726e  }r....(U.anchorn
-00006690: 616d 6555 2123 616e 6f74 6865 722d 736f  ameU!#another-so
-000066a0: 6c75 7469 6f6e 2d6d 6172 6769 6e61 6c69  lution-marginali
-000066b0: 7a61 7469 6f6e 5506 7265 6675 7269 6846  zationU.refurihF
-000066c0: 6816 5d68 155d 6813 5d68 145d 6817 5d55  h.]h.]h.]h.]h.]U
-000066d0: 0869 6e74 6572 6e61 6c88 7568 1f6a b704  .internal.uh.j..
-000066e0: 0000 6818 5d72 be04 0000 681a 5824 0000  ..h.]r....h.X$..
-000066f0: 0041 6e6f 7468 6572 2053 6f6c 7574 696f  .Another Solutio
-00006700: 6e20 e280 9420 4d61 7267 696e 616c 697a  n ... Marginaliz
-00006710: 6174 696f 6e72 bf04 0000 8581 72c0 0400  ationr......r...
-00006720: 007d 72c1 0400 0028 6810 5824 0000 0041  .}r....(h.X$...A
-00006730: 6e6f 7468 6572 2053 6f6c 7574 696f 6e20  nother Solution 
-00006740: 2d2d 2d20 4d61 7267 696e 616c 697a 6174  --- Marginalizat
-00006750: 696f 6e68 1f6a bb04 0000 7562 6168 206a  ionh.j....ubah j
-00006760: 6002 0000 7562 6168 206a 6102 0000 7562  `...ubah ja...ub
-00006770: 6168 206a 7802 0000 7562 6568 206a 7702  ah jx...ubeh jw.
-00006780: 0000 7562 6568 206a 7802 0000 7562 6168  ..ubeh jx...ubah
-00006790: 206a 7702 0000 7562 684f 6a49 0200 0029   jw...ubhOjI...)
-000067a0: 8172 c204 0000 7d72 c304 0000 2868 1055  .r....}r....(h.U
-000067b0: 0068 117d 72c4 0400 0028 6813 5d68 145d  .h.}r....(h.]h.]
-000067c0: 6815 5d68 165d 6817 5d75 6818 5d72 c504  h.]h.]h.]uh.]r..
-000067d0: 0000 6a4e 0200 0029 8172 c604 0000 7d72  ..jN...).r....}r
-000067e0: c704 0000 2868 1055 0068 117d 72c8 0400  ....(h.U.h.}r...
-000067f0: 0028 6813 5d68 145d 6815 5d68 165d 6817  .(h.]h.]h.]h.]h.
-00006800: 5d75 681f 6ac2 0400 0068 185d 72c9 0400  ]uh.j....h.]r...
-00006810: 0028 6a53 0200 0029 8172 ca04 0000 7d72  .(jS...).r....}r
-00006820: cb04 0000 2868 1055 0068 117d 72cc 0400  ....(h.U.h.}r...
-00006830: 0028 6813 5d68 145d 6815 5d68 165d 6817  .(h.]h.]h.]h.]h.
-00006840: 5d75 681f 6ac6 0400 0068 185d 72cd 0400  ]uh.j....h.]r...
-00006850: 006a 5802 0000 2981 72ce 0400 007d 72cf  .jX...).r....}r.
-00006860: 0400 0028 6810 5500 6811 7d72 d004 0000  ...(h.U.h.}r....
-00006870: 2855 0a61 6e63 686f 726e 616d 6555 0055  (U.anchornameU.U
-00006880: 0672 6566 7572 6968 4f68 165d 6815 5d68  .refurihOh.]h.]h
-00006890: 135d 6814 5d68 175d 5508 696e 7465 726e  .]h.]h.]U.intern
-000068a0: 616c 8875 681f 6aca 0400 0068 185d 72d1  al.uh.j....h.]r.
-000068b0: 0400 0068 1a58 2b00 0000 4361 7365 2053  ...h.X+...Case S
-000068c0: 7475 6479 3a20 4f75 746c 6965 7273 2061  tudy: Outliers a
-000068d0: 6e64 2042 6179 6573 6961 6e20 496e 7465  nd Bayesian Inte
-000068e0: 6772 616c 7372 d204 0000 8581 72d3 0400  gralsr......r...
-000068f0: 007d 72d4 0400 0028 6810 6857 681f 6ace  .}r....(h.hWh.j.
-00006900: 0400 0075 6261 6820 6a60 0200 0075 6261  ...ubah j`...uba
-00006910: 6820 6a61 0200 0075 626a 4902 0000 2981  h ja...ubjI...).
-00006920: 72d5 0400 007d 72d6 0400 0028 6810 5500  r....}r....(h.U.
-00006930: 6811 7d72 d704 0000 2868 135d 6814 5d68  h.}r....(h.]h.]h
-00006940: 155d 6816 5d68 175d 7568 1f6a c604 0000  .]h.]h.]uh.j....
-00006950: 6818 5d72 d804 0000 286a 4e02 0000 2981  h.]r....(jN...).
-00006960: 72d9 0400 007d 72da 0400 0028 6810 5500  r....}r....(h.U.
-00006970: 6811 7d72 db04 0000 2868 135d 6814 5d68  h.}r....(h.]h.]h
-00006980: 155d 6816 5d68 175d 7568 1f6a d504 0000  .]h.]h.]uh.j....
-00006990: 6818 5d72 dc04 0000 6a53 0200 0029 8172  h.]r....jS...).r
-000069a0: dd04 0000 7d72 de04 0000 2868 1055 0068  ....}r....(h.U.h
-000069b0: 117d 72df 0400 0028 6813 5d68 145d 6815  .}r....(h.]h.]h.
-000069c0: 5d68 165d 6817 5d75 681f 6ad9 0400 0068  ]h.]h.]uh.j....h
-000069d0: 185d 72e0 0400 006a 5802 0000 2981 72e1  .]r....jX...).r.
-000069e0: 0400 007d 72e2 0400 0028 6810 5500 6811  ...}r....(h.U.h.
-000069f0: 7d72 e304 0000 2855 0a61 6e63 686f 726e  }r....(U.anchorn
-00006a00: 616d 6555 0c23 7468 652d 7072 6f62 6c65  ameU.#the-proble
-00006a10: 6d55 0672 6566 7572 6968 4f68 165d 6815  mU.refurihOh.]h.
-00006a20: 5d68 135d 6814 5d68 175d 5508 696e 7465  ]h.]h.]h.]U.inte
-00006a30: 726e 616c 8875 681f 6add 0400 0068 185d  rnal.uh.j....h.]
-00006a40: 72e4 0400 0068 1a58 0b00 0000 5468 6520  r....h.X....The 
-00006a50: 5072 6f62 6c65 6d72 e504 0000 8581 72e6  Problemr......r.
-00006a60: 0400 007d 72e7 0400 0028 6810 580b 0000  ...}r....(h.X...
-00006a70: 0054 6865 2050 726f 626c 656d 681f 6ae1  .The Problemh.j.
-00006a80: 0400 0075 6261 6820 6a60 0200 0075 6261  ...ubah j`...uba
-00006a90: 6820 6a61 0200 0075 6261 6820 6a78 0200  h ja...ubah jx..
-00006aa0: 0075 626a 4e02 0000 2981 72e8 0400 007d  .ubjN...).r....}
-00006ab0: 72e9 0400 0028 6810 5500 6811 7d72 ea04  r....(h.U.h.}r..
-00006ac0: 0000 2868 135d 6814 5d68 155d 6816 5d68  ..(h.]h.]h.]h.]h
-00006ad0: 175d 7568 1f6a d504 0000 6818 5d72 eb04  .]uh.j....h.]r..
-00006ae0: 0000 6a53 0200 0029 8172 ec04 0000 7d72  ..jS...).r....}r
-00006af0: ed04 0000 2868 1055 0068 117d 72ee 0400  ....(h.U.h.}r...
-00006b00: 0028 6813 5d68 145d 6815 5d68 165d 6817  .(h.]h.]h.]h.]h.
-00006b10: 5d75 681f 6ae8 0400 0068 185d 72ef 0400  ]uh.j....h.]r...
-00006b20: 006a 5802 0000 2981 72f0 0400 007d 72f1  .jX...).r....}r.
-00006b30: 0400 0028 6810 5500 6811 7d72 f204 0000  ...(h.U.h.}r....
-00006b40: 2855 0a61 6e63 686f 726e 616d 6555 0b23  (U.anchornameU.#
-00006b50: 612d 736f 6c75 7469 6f6e 5506 7265 6675  a-solutionU.refu
-00006b60: 7269 684f 6816 5d68 155d 6813 5d68 145d  rihOh.]h.]h.]h.]
-00006b70: 6817 5d55 0869 6e74 6572 6e61 6c88 7568  h.]U.internal.uh
-00006b80: 1f6a ec04 0000 6818 5d72 f304 0000 681a  .j....h.]r....h.
-00006b90: 580a 0000 0041 2053 6f6c 7574 696f 6e72  X....A Solutionr
-00006ba0: f404 0000 8581 72f5 0400 007d 72f6 0400  ......r....}r...
-00006bb0: 0028 6810 580a 0000 0041 2053 6f6c 7574  .(h.X....A Solut
-00006bc0: 696f 6e68 1f6a f004 0000 7562 6168 206a  ionh.j....ubah j
-00006bd0: 6002 0000 7562 6168 206a 6102 0000 7562  `...ubah ja...ub
-00006be0: 6168 206a 7802 0000 7562 6a4e 0200 0029  ah jx...ubjN...)
-00006bf0: 8172 f704 0000 7d72 f804 0000 2868 1055  .r....}r....(h.U
-00006c00: 0068 117d 72f9 0400 0028 6813 5d68 145d  .h.}r....(h.]h.]
-00006c10: 6815 5d68 165d 6817 5d75 681f 6ad5 0400  h.]h.]h.]uh.j...
-00006c20: 0068 185d 72fa 0400 006a 5302 0000 2981  .h.]r....jS...).
-00006c30: 72fb 0400 007d 72fc 0400 0028 6810 5500  r....}r....(h.U.
-00006c40: 6811 7d72 fd04 0000 2868 135d 6814 5d68  h.}r....(h.]h.]h
-00006c50: 155d 6816 5d68 175d 7568 1f6a f704 0000  .]h.]h.]uh.j....
-00006c60: 6818 5d72 fe04 0000 6a58 0200 0029 8172  h.]r....jX...).r
-00006c70: ff04 0000 7d72 0005 0000 2868 1055 0068  ....}r....(h.U.h
-00006c80: 117d 7201 0500 0028 550a 616e 6368 6f72  .}r....(U.anchor
-00006c90: 6e61 6d65 550c 2361 2d76 6172 6961 7469  nameU.#a-variati
-00006ca0: 6f6e 5506 7265 6675 7269 684f 6816 5d68  onU.refurihOh.]h
-00006cb0: 155d 6813 5d68 145d 6817 5d55 0869 6e74  .]h.]h.]h.]U.int
-00006cc0: 6572 6e61 6c88 7568 1f6a fb04 0000 6818  ernal.uh.j....h.
-00006cd0: 5d72 0205 0000 681a 580b 0000 0041 2056  ]r....h.X....A V
-00006ce0: 6172 6961 7469 6f6e 7203 0500 0085 8172  ariationr......r
-00006cf0: 0405 0000 7d72 0505 0000 2868 1058 0b00  ....}r....(h.X..
-00006d00: 0000 4120 5661 7269 6174 696f 6e68 1f6a  ..A Variationh.j
-00006d10: ff04 0000 7562 6168 206a 6002 0000 7562  ....ubah j`...ub
-00006d20: 6168 206a 6102 0000 7562 6168 206a 7802  ah ja...ubah jx.
-00006d30: 0000 7562 6568 206a 7702 0000 7562 6568  ..ubeh jw...ubeh
-00006d40: 206a 7802 0000 7562 6168 206a 7702 0000   jx...ubah jw...
-00006d50: 7562 6858 6a49 0200 0029 8172 0605 0000  ubhXjI...).r....
-00006d60: 7d72 0705 0000 2868 1055 0068 117d 7208  }r....(h.U.h.}r.
-00006d70: 0500 0028 6813 5d68 145d 6815 5d68 165d  ...(h.]h.]h.]h.]
-00006d80: 6817 5d75 6818 5d72 0905 0000 6a4e 0200  h.]uh.]r....jN..
-00006d90: 0029 8172 0a05 0000 7d72 0b05 0000 2868  .).r....}r....(h
-00006da0: 1055 0068 117d 720c 0500 0028 6813 5d68  .U.h.}r....(h.]h
-00006db0: 145d 6815 5d68 165d 6817 5d75 681f 6a06  .]h.]h.]h.]uh.j.
-00006dc0: 0500 0068 185d 720d 0500 0028 6a53 0200  ...h.]r....(jS..
-00006dd0: 0029 8172 0e05 0000 7d72 0f05 0000 2868  .).r....}r....(h
-00006de0: 1055 0068 117d 7210 0500 0028 6813 5d68  .U.h.}r....(h.]h
-00006df0: 145d 6815 5d68 165d 6817 5d75 681f 6a0a  .]h.]h.]h.]uh.j.
-00006e00: 0500 0068 185d 7211 0500 006a 5802 0000  ...h.]r....jX...
-00006e10: 2981 7212 0500 007d 7213 0500 0028 6810  ).r....}r....(h.
-00006e20: 5500 6811 7d72 1405 0000 2855 0a61 6e63  U.h.}r....(U.anc
-00006e30: 686f 726e 616d 6555 0055 0672 6566 7572  hornameU.U.refur
-00006e40: 6968 5868 165d 6815 5d68 135d 6814 5d68  ihXh.]h.]h.]h.]h
-00006e50: 175d 5508 696e 7465 726e 616c 8875 681f  .]U.internal.uh.
-00006e60: 6a0e 0500 0068 185d 7215 0500 0028 6830  j....h.]r....(h0
-00006e70: 2981 7216 0500 007d 7217 0500 0028 6810  ).r....}r....(h.
-00006e80: 5805 0000 0073 6369 7079 6811 7d72 1805  X....scipyh.}r..
-00006e90: 0000 2868 135d 6814 5d68 155d 6816 5d68  ..(h.]h.]h.]h.]h
-00006ea0: 175d 7568 1f6a 1205 0000 6818 5d72 1905  .]uh.j....h.]r..
-00006eb0: 0000 681a 5805 0000 0073 6369 7079 721a  ..h.X....scipyr.
-00006ec0: 0500 0085 8172 1b05 0000 7d72 1c05 0000  .....r....}r....
-00006ed0: 2868 1055 0068 1f6a 1605 0000 7562 6168  (h.U.h.j....ubah
-00006ee0: 2068 3875 6268 1a58 0900 0000 2052 6f75   h8ubh.X.... Rou
-00006ef0: 7469 6e65 7372 1d05 0000 8581 721e 0500  tinesr......r...
-00006f00: 007d 721f 0500 0028 6810 6867 681f 6a12  .}r....(h.hgh.j.
-00006f10: 0500 0075 6265 6820 6a60 0200 0075 6261  ...ubeh j`...uba
-00006f20: 6820 6a61 0200 0075 626a 4902 0000 2981  h ja...ubjI...).
-00006f30: 7220 0500 007d 7221 0500 0028 6810 5500  r ...}r!...(h.U.
-00006f40: 6811 7d72 2205 0000 2868 135d 6814 5d68  h.}r"...(h.]h.]h
-00006f50: 155d 6816 5d68 175d 7568 1f6a 0a05 0000  .]h.]h.]uh.j....
-00006f60: 6818 5d72 2305 0000 286a 4e02 0000 2981  h.]r#...(jN...).
-00006f70: 7224 0500 007d 7225 0500 0028 6810 5500  r$...}r%...(h.U.
-00006f80: 6811 7d72 2605 0000 2868 135d 6814 5d68  h.}r&...(h.]h.]h
-00006f90: 155d 6816 5d68 175d 7568 1f6a 2005 0000  .]h.]h.]uh.j ...
-00006fa0: 6818 5d72 2705 0000 6a53 0200 0029 8172  h.]r'...jS...).r
-00006fb0: 2805 0000 7d72 2905 0000 2868 1055 0068  (...}r)...(h.U.h
-00006fc0: 117d 722a 0500 0028 6813 5d68 145d 6815  .}r*...(h.]h.]h.
-00006fd0: 5d68 165d 6817 5d75 681f 6a24 0500 0068  ]h.]h.]uh.j$...h
-00006fe0: 185d 722b 0500 006a 5802 0000 2981 722c  .]r+...jX...).r,
-00006ff0: 0500 007d 722d 0500 0028 6810 5500 6811  ...}r-...(h.U.h.
-00007000: 7d72 2e05 0000 2855 0a61 6e63 686f 726e  }r....(U.anchorn
-00007010: 616d 6555 0723 6669 7474 6572 5506 7265  ameU.#fitterU.re
-00007020: 6675 7269 6858 6816 5d68 155d 6813 5d68  furihXh.]h.]h.]h
-00007030: 145d 6817 5d55 0869 6e74 6572 6e61 6c88  .]h.]U.internal.
-00007040: 7568 1f6a 2805 0000 6818 5d72 2f05 0000  uh.j(...h.]r/...
-00007050: 681a 5806 0000 0046 6974 7465 7272 3005  h.X....Fitterr0.
-00007060: 0000 8581 7231 0500 007d 7232 0500 0028  ....r1...}r2...(
-00007070: 6810 5806 0000 0046 6974 7465 7272 3305  h.X....Fitterr3.
-00007080: 0000 681f 6a2c 0500 0075 6261 6820 6a60  ..h.j,...ubah j`
-00007090: 0200 0075 6261 6820 6a61 0200 0075 6261  ...ubah ja...uba
-000070a0: 6820 6a78 0200 0075 626a 4e02 0000 2981  h jx...ubjN...).
-000070b0: 7234 0500 007d 7235 0500 0028 6810 5500  r4...}r5...(h.U.
-000070c0: 6811 7d72 3605 0000 2868 135d 6814 5d68  h.}r6...(h.]h.]h
-000070d0: 155d 6816 5d68 175d 7568 1f6a 2005 0000  .]h.]h.]uh.j ...
-000070e0: 6818 5d72 3705 0000 6a53 0200 0029 8172  h.]r7...jS...).r
-000070f0: 3805 0000 7d72 3905 0000 2868 1055 0068  8...}r9...(h.U.h
-00007100: 117d 723a 0500 0028 6813 5d68 145d 6815  .}r:...(h.]h.]h.
-00007110: 5d68 165d 6817 5d75 681f 6a34 0500 0068  ]h.]h.]uh.j4...h
-00007120: 185d 723b 0500 006a 5802 0000 2981 723c  .]r;...jX...).r<
-00007130: 0500 007d 723d 0500 0028 6810 5500 6811  ...}r=...(h.U.h.
-00007140: 7d72 3e05 0000 2855 0a61 6e63 686f 726e  }r>...(U.anchorn
-00007150: 616d 6555 0a23 6d69 6e69 6d69 7a65 7255  ameU.#minimizerU
-00007160: 0672 6566 7572 6968 5868 165d 6815 5d68  .refurihXh.]h.]h
-00007170: 135d 6814 5d68 175d 5508 696e 7465 726e  .]h.]h.]U.intern
-00007180: 616c 8875 681f 6a38 0500 0068 185d 723f  al.uh.j8...h.]r?
-00007190: 0500 0068 1a58 0900 0000 4d69 6e69 6d69  ...h.X....Minimi
-000071a0: 7a65 7272 4005 0000 8581 7241 0500 007d  zerr@.....rA...}
-000071b0: 7242 0500 0028 6810 5809 0000 004d 696e  rB...(h.X....Min
-000071c0: 696d 697a 6572 7243 0500 0068 1f6a 3c05  imizerrC...h.j<.
-000071d0: 0000 7562 6168 206a 6002 0000 7562 6168  ..ubah j`...ubah
-000071e0: 206a 6102 0000 7562 6168 206a 7802 0000   ja...ubah jx...
-000071f0: 7562 6568 206a 7702 0000 7562 6568 206a  ubeh jw...ubeh j
-00007200: 7802 0000 7562 6168 206a 7702 0000 7562  x...ubah jw...ub
-00007210: 6868 6a49 0200 0029 8172 4405 0000 7d72  hhjI...).rD...}r
-00007220: 4505 0000 2868 1055 0068 117d 7246 0500  E...(h.U.h.}rF..
-00007230: 0028 6813 5d68 145d 6815 5d68 165d 6817  .(h.]h.]h.]h.]h.
-00007240: 5d75 6818 5d72 4705 0000 6a4e 0200 0029  ]uh.]rG...jN...)
-00007250: 8172 4805 0000 7d72 4905 0000 2868 1055  .rH...}rI...(h.U
-00007260: 0068 117d 724a 0500 0028 6813 5d68 145d  .h.}rJ...(h.]h.]
-00007270: 6815 5d68 165d 6817 5d75 681f 6a44 0500  h.]h.]h.]uh.jD..
-00007280: 0068 185d 724b 0500 0028 6a53 0200 0029  .h.]rK...(jS...)
-00007290: 8172 4c05 0000 7d72 4d05 0000 2868 1055  .rL...}rM...(h.U
-000072a0: 0068 117d 724e 0500 0028 6813 5d68 145d  .h.}rN...(h.]h.]
-000072b0: 6815 5d68 165d 6817 5d75 681f 6a48 0500  h.]h.]h.]uh.jH..
-000072c0: 0068 185d 724f 0500 006a 5802 0000 2981  .h.]rO...jX...).
-000072d0: 7250 0500 007d 7251 0500 0028 6810 5500  rP...}rQ...(h.U.
-000072e0: 6811 7d72 5205 0000 2855 0a61 6e63 686f  h.}rR...(U.ancho
-000072f0: 726e 616d 6555 0055 0672 6566 7572 6968  rnameU.U.refurih
-00007300: 6868 165d 6815 5d68 135d 6814 5d68 175d  hh.]h.]h.]h.]h.]
-00007310: 5508 696e 7465 726e 616c 8875 681f 6a4c  U.internal.uh.jL
-00007320: 0500 0068 185d 7253 0500 0068 1a58 1400  ...h.]rS...h.X..
-00007330: 0000 4361 7365 2053 7475 6479 3a20 5065  ..Case Study: Pe
-00007340: 6e64 756c 756d 7254 0500 0085 8172 5505  ndulumrT.....rU.
-00007350: 0000 7d72 5605 0000 2868 1068 7068 1f6a  ..}rV...(h.hph.j
-00007360: 5005 0000 7562 6168 206a 6002 0000 7562  P...ubah j`...ub
-00007370: 6168 206a 6102 0000 7562 6a49 0200 0029  ah ja...ubjI...)
-00007380: 8172 5705 0000 7d72 5805 0000 2868 1055  .rW...}rX...(h.U
-00007390: 0068 117d 7259 0500 0028 6813 5d68 145d  .h.}rY...(h.]h.]
-000073a0: 6815 5d68 165d 6817 5d75 681f 6a48 0500  h.]h.]h.]uh.jH..
-000073b0: 0068 185d 725a 0500 0028 6a4e 0200 0029  .h.]rZ...(jN...)
-000073c0: 8172 5b05 0000 7d72 5c05 0000 2868 1055  .r[...}r\...(h.U
-000073d0: 0068 117d 725d 0500 0028 6813 5d68 145d  .h.}r]...(h.]h.]
-000073e0: 6815 5d68 165d 6817 5d75 681f 6a57 0500  h.]h.]h.]uh.jW..
-000073f0: 0068 185d 725e 0500 006a 5302 0000 2981  .h.]r^...jS...).
-00007400: 725f 0500 007d 7260 0500 0028 6810 5500  r_...}r`...(h.U.
-00007410: 6811 7d72 6105 0000 2868 135d 6814 5d68  h.}ra...(h.]h.]h
-00007420: 155d 6816 5d68 175d 7568 1f6a 5b05 0000  .]h.]h.]uh.j[...
-00007430: 6818 5d72 6205 0000 6a58 0200 0029 8172  h.]rb...jX...).r
-00007440: 6305 0000 7d72 6405 0000 2868 1055 0068  c...}rd...(h.U.h
-00007450: 117d 7265 0500 0028 550a 616e 6368 6f72  .}re...(U.anchor
-00007460: 6e61 6d65 550c 2374 6865 2d70 726f 626c  nameU.#the-probl
-00007470: 656d 5506 7265 6675 7269 6868 6816 5d68  emU.refurihhh.]h
-00007480: 155d 6813 5d68 145d 6817 5d55 0869 6e74  .]h.]h.]h.]U.int
-00007490: 6572 6e61 6c88 7568 1f6a 5f05 0000 6818  ernal.uh.j_...h.
-000074a0: 5d72 6605 0000 681a 580b 0000 0054 6865  ]rf...h.X....The
-000074b0: 2050 726f 626c 656d 7267 0500 0085 8172   Problemrg.....r
-000074c0: 6805 0000 7d72 6905 0000 2868 1058 0b00  h...}ri...(h.X..
-000074d0: 0000 5468 6520 5072 6f62 6c65 6d68 1f6a  ..The Problemh.j
-000074e0: 6305 0000 7562 6168 206a 6002 0000 7562  c...ubah j`...ub
-000074f0: 6168 206a 6102 0000 7562 6168 206a 7802  ah ja...ubah jx.
-00007500: 0000 7562 6a4e 0200 0029 8172 6a05 0000  ..ubjN...).rj...
-00007510: 7d72 6b05 0000 2868 1055 0068 117d 726c  }rk...(h.U.h.}rl
-00007520: 0500 0028 6813 5d68 145d 6815 5d68 165d  ...(h.]h.]h.]h.]
-00007530: 6817 5d75 681f 6a57 0500 0068 185d 726d  h.]uh.jW...h.]rm
-00007540: 0500 006a 5302 0000 2981 726e 0500 007d  ...jS...).rn...}
-00007550: 726f 0500 0028 6810 5500 6811 7d72 7005  ro...(h.U.h.}rp.
-00007560: 0000 2868 135d 6814 5d68 155d 6816 5d68  ..(h.]h.]h.]h.]h
-00007570: 175d 7568 1f6a 6a05 0000 6818 5d72 7105  .]uh.jj...h.]rq.
-00007580: 0000 6a58 0200 0029 8172 7205 0000 7d72  ..jX...).rr...}r
-00007590: 7305 0000 2868 1055 0068 117d 7274 0500  s...(h.U.h.}rt..
-000075a0: 0028 550a 616e 6368 6f72 6e61 6d65 5512  .(U.anchornameU.
-000075b0: 2370 656e 6475 6c75 6d2d 6479 6e61 6d69  #pendulum-dynami
-000075c0: 6373 5506 7265 6675 7269 6868 6816 5d68  csU.refurihhh.]h
-000075d0: 155d 6813 5d68 145d 6817 5d55 0869 6e74  .]h.]h.]h.]U.int
-000075e0: 6572 6e61 6c88 7568 1f6a 6e05 0000 6818  ernal.uh.jn...h.
-000075f0: 5d72 7505 0000 681a 5811 0000 0050 656e  ]ru...h.X....Pen
-00007600: 6475 6c75 6d20 4479 6e61 6d69 6373 7276  dulum Dynamicsrv
-00007610: 0500 0085 8172 7705 0000 7d72 7805 0000  .....rw...}rx...
-00007620: 2868 1058 1100 0000 5065 6e64 756c 756d  (h.X....Pendulum
-00007630: 2044 796e 616d 6963 7368 1f6a 7205 0000   Dynamicsh.jr...
-00007640: 7562 6168 206a 6002 0000 7562 6168 206a  ubah j`...ubah j
-00007650: 6102 0000 7562 6168 206a 7802 0000 7562  a...ubah jx...ub
-00007660: 6a4e 0200 0029 8172 7905 0000 7d72 7a05  jN...).ry...}rz.
-00007670: 0000 2868 1055 0068 117d 727b 0500 0028  ..(h.U.h.}r{...(
-00007680: 6813 5d68 145d 6815 5d68 165d 6817 5d75  h.]h.]h.]h.]h.]u
-00007690: 681f 6a57 0500 0068 185d 727c 0500 006a  h.jW...h.]r|...j
-000076a0: 5302 0000 2981 727d 0500 007d 727e 0500  S...).r}...}r~..
-000076b0: 0028 6810 5500 6811 7d72 7f05 0000 2868  .(h.U.h.}r....(h
-000076c0: 135d 6814 5d68 155d 6816 5d68 175d 7568  .]h.]h.]h.]h.]uh
-000076d0: 1f6a 7905 0000 6818 5d72 8005 0000 6a58  .jy...h.]r....jX
-000076e0: 0200 0029 8172 8105 0000 7d72 8205 0000  ...).r....}r....
-000076f0: 2868 1055 0068 117d 7283 0500 0028 550a  (h.U.h.}r....(U.
-00007700: 616e 6368 6f72 6e61 6d65 5518 2374 776f  anchornameU.#two
-00007710: 2d74 7970 6573 2d6f 662d 696e 7075 742d  -types-of-input-
-00007720: 6461 7461 5506 7265 6675 7269 6868 6816  dataU.refurihhh.
-00007730: 5d68 155d 6813 5d68 145d 6817 5d55 0869  ]h.]h.]h.]h.]U.i
-00007740: 6e74 6572 6e61 6c88 7568 1f6a 7d05 0000  nternal.uh.j}...
-00007750: 6818 5d72 8405 0000 681a 5817 0000 0054  h.]r....h.X....T
-00007760: 776f 2054 7970 6573 206f 6620 496e 7075  wo Types of Inpu
-00007770: 7420 4461 7461 7285 0500 0085 8172 8605  t Datar......r..
-00007780: 0000 7d72 8705 0000 2868 1058 1700 0000  ..}r....(h.X....
-00007790: 5477 6f20 5479 7065 7320 6f66 2049 6e70  Two Types of Inp
-000077a0: 7574 2044 6174 6168 1f6a 8105 0000 7562  ut Datah.j....ub
-000077b0: 6168 206a 6002 0000 7562 6168 206a 6102  ah j`...ubah ja.
-000077c0: 0000 7562 6168 206a 7802 0000 7562 6568  ..ubah jx...ubeh
-000077d0: 206a 7702 0000 7562 6568 206a 7802 0000   jw...ubeh jx...
-000077e0: 7562 6168 206a 7702 0000 7562 6871 6a49  ubah jw...ubhqjI
-000077f0: 0200 0029 8172 8805 0000 7d72 8905 0000  ...).r....}r....
-00007800: 2868 1055 0068 117d 728a 0500 0028 6813  (h.U.h.}r....(h.
-00007810: 5d68 145d 6815 5d68 165d 6817 5d75 6818  ]h.]h.]h.]h.]uh.
-00007820: 5d72 8b05 0000 6a4e 0200 0029 8172 8c05  ]r....jN...).r..
-00007830: 0000 7d72 8d05 0000 2868 1055 0068 117d  ..}r....(h.U.h.}
-00007840: 728e 0500 0028 6813 5d68 145d 6815 5d68  r....(h.]h.]h.]h
-00007850: 165d 6817 5d75 681f 6a88 0500 0068 185d  .]h.]uh.j....h.]
-00007860: 728f 0500 0028 6a53 0200 0029 8172 9005  r....(jS...).r..
-00007870: 0000 7d72 9105 0000 2868 1055 0068 117d  ..}r....(h.U.h.}
-00007880: 7292 0500 0028 6813 5d68 145d 6815 5d68  r....(h.]h.]h.]h
-00007890: 165d 6817 5d75 681f 6a8c 0500 0068 185d  .]h.]uh.j....h.]
-000078a0: 7293 0500 006a 5802 0000 2981 7294 0500  r....jX...).r...
-000078b0: 007d 7295 0500 0028 6810 5500 6811 7d72  .}r....(h.U.h.}r
-000078c0: 9605 0000 2855 0a61 6e63 686f 726e 616d  ....(U.anchornam
-000078d0: 6555 0055 0672 6566 7572 6968 7168 165d  eU.U.refurihqh.]
-000078e0: 6815 5d68 135d 6814 5d68 175d 5508 696e  h.]h.]h.]h.]U.in
-000078f0: 7465 726e 616c 8875 681f 6a90 0500 0068  ternal.uh.j....h
-00007900: 185d 7297 0500 0068 1a58 0c00 0000 4753  .]r....h.X....GS
-00007910: 4c20 526f 7574 696e 6573 7298 0500 0085  L Routinesr.....
-00007920: 8172 9905 0000 7d72 9a05 0000 2868 1068  .r....}r....(h.h
-00007930: 7968 1f6a 9405 0000 7562 6168 206a 6002  yh.j....ubah j`.
-00007940: 0000 7562 6168 206a 6102 0000 7562 6a49  ..ubah ja...ubjI
-00007950: 0200 0029 8172 9b05 0000 7d72 9c05 0000  ...).r....}r....
-00007960: 2868 1055 0068 117d 729d 0500 0028 6813  (h.U.h.}r....(h.
-00007970: 5d68 145d 6815 5d68 165d 6817 5d75 681f  ]h.]h.]h.]h.]uh.
-00007980: 6a8c 0500 0068 185d 729e 0500 0028 6a4e  j....h.]r....(jN
-00007990: 0200 0029 8172 9f05 0000 7d72 a005 0000  ...).r....}r....
-000079a0: 2868 1055 0068 117d 72a1 0500 0028 6813  (h.U.h.}r....(h.
-000079b0: 5d68 145d 6815 5d68 165d 6817 5d75 681f  ]h.]h.]h.]h.]uh.
-000079c0: 6a9b 0500 0068 185d 72a2 0500 006a 5302  j....h.]r....jS.
-000079d0: 0000 2981 72a3 0500 007d 72a4 0500 0028  ..).r....}r....(
-000079e0: 6810 5500 6811 7d72 a505 0000 2868 135d  h.U.h.}r....(h.]
-000079f0: 6814 5d68 155d 6816 5d68 175d 7568 1f6a  h.]h.]h.]h.]uh.j
-00007a00: 9f05 0000 6818 5d72 a605 0000 6a58 0200  ....h.]r....jX..
-00007a10: 0029 8172 a705 0000 7d72 a805 0000 2868  .).r....}r....(h
-00007a20: 1055 0068 117d 72a9 0500 0028 550a 616e  .U.h.}r....(U.an
-00007a30: 6368 6f72 6e61 6d65 5508 2366 6974 7465  chornameU.#fitte
-00007a40: 7273 5506 7265 6675 7269 6871 6816 5d68  rsU.refurihqh.]h
-00007a50: 155d 6813 5d68 145d 6817 5d55 0869 6e74  .]h.]h.]h.]U.int
-00007a60: 6572 6e61 6c88 7568 1f6a a305 0000 6818  ernal.uh.j....h.
-00007a70: 5d72 aa05 0000 681a 5807 0000 0046 6974  ]r....h.X....Fit
-00007a80: 7465 7273 72ab 0500 0085 8172 ac05 0000  tersr......r....
-00007a90: 7d72 ad05 0000 2868 1058 0700 0000 4669  }r....(h.X....Fi
-00007aa0: 7474 6572 7368 1f6a a705 0000 7562 6168  ttersh.j....ubah
-00007ab0: 206a 6002 0000 7562 6168 206a 6102 0000   j`...ubah ja...
-00007ac0: 7562 6168 206a 7802 0000 7562 6a4e 0200  ubah jx...ubjN..
-00007ad0: 0029 8172 ae05 0000 7d72 af05 0000 2868  .).r....}r....(h
-00007ae0: 1055 0068 117d 72b0 0500 0028 6813 5d68  .U.h.}r....(h.]h
-00007af0: 145d 6815 5d68 165d 6817 5d75 681f 6a9b  .]h.]h.]h.]uh.j.
-00007b00: 0500 0068 185d 72b1 0500 006a 5302 0000  ...h.]r....jS...
-00007b10: 2981 72b2 0500 007d 72b3 0500 0028 6810  ).r....}r....(h.
-00007b20: 5500 6811 7d72 b405 0000 2868 135d 6814  U.h.}r....(h.]h.
-00007b30: 5d68 155d 6816 5d68 175d 7568 1f6a ae05  ]h.]h.]h.]uh.j..
-00007b40: 0000 6818 5d72 b505 0000 6a58 0200 0029  ..h.]r....jX...)
-00007b50: 8172 b605 0000 7d72 b705 0000 2868 1055  .r....}r....(h.U
-00007b60: 0068 117d 72b8 0500 0028 550a 616e 6368  .h.}r....(U.anch
-00007b70: 6f72 6e61 6d65 550a 236d 696e 696d 697a  ornameU.#minimiz
-00007b80: 6572 5506 7265 6675 7269 6871 6816 5d68  erU.refurihqh.]h
-00007b90: 155d 6813 5d68 145d 6817 5d55 0869 6e74  .]h.]h.]h.]U.int
-00007ba0: 6572 6e61 6c88 7568 1f6a b205 0000 6818  ernal.uh.j....h.
-00007bb0: 5d72 b905 0000 681a 5809 0000 004d 696e  ]r....h.X....Min
-00007bc0: 696d 697a 6572 72ba 0500 0085 8172 bb05  imizerr......r..
-00007bd0: 0000 7d72 bc05 0000 2868 1058 0900 0000  ..}r....(h.X....
-00007be0: 4d69 6e69 6d69 7a65 7268 1f6a b605 0000  Minimizerh.j....
-00007bf0: 7562 6168 206a 6002 0000 7562 6168 206a  ubah j`...ubah j
-00007c00: 6102 0000 7562 6168 206a 7802 0000 7562  a...ubah jx...ub
-00007c10: 6568 206a 7702 0000 7562 6568 206a 7802  eh jw...ubeh jx.
-00007c20: 0000 7562 6168 206a 7702 0000 7562 7555  ..ubah jw...ubuU
-00007c30: 0c69 6e64 6578 656e 7472 6965 7372 bd05  .indexentriesr..
-00007c40: 0000 7d72 be05 0000 2868 0c5d 6822 5d68  ..}r....(h.]h"]h
-00007c50: 2b5d 72bf 0500 0028 2855 0673 696e 676c  +]r....((U.singl
-00007c60: 6572 c005 0000 580f 0000 006c 7371 6669  er....X....lsqfi
-00007c70: 7420 286d 6f64 756c 6529 580d 0000 006d  t (module)X....m
-00007c80: 6f64 756c 652d 6c73 7166 6974 5500 4e74  odule-lsqfitU.Nt
-00007c90: 72c1 0500 0028 6ac0 0500 0058 1f00 0000  r....(j....X....
-00007ca0: 6e6f 6e6c 696e 6561 725f 6669 7420 2863  nonlinear_fit (c
-00007cb0: 6c61 7373 2069 6e20 6c73 7166 6974 2968  lass in lsqfit)h
-00007cc0: ce55 004e 7472 c205 0000 286a c005 0000  .U.Ntr....(j....
-00007cd0: 5825 0000 0063 6869 3220 286c 7371 6669  X%...chi2 (lsqfi
-00007ce0: 742e 6e6f 6e6c 696e 6561 725f 6669 7420  t.nonlinear_fit 
-00007cf0: 6174 7472 6962 7574 6529 68d6 5500 4e74  attribute)h.U.Nt
-00007d00: 72c3 0500 0028 6ac0 0500 0058 2400 0000  r....(j....X$...
-00007d10: 636f 7620 286c 7371 6669 742e 6e6f 6e6c  cov (lsqfit.nonl
-00007d20: 696e 6561 725f 6669 7420 6174 7472 6962  inear_fit attrib
-00007d30: 7574 6529 68bc 5500 4e74 72c4 0500 0028  ute)h.U.Ntr....(
-00007d40: 6ac0 0500 0058 2400 0000 646f 6620 286c  j....X$...dof (l
-00007d50: 7371 6669 742e 6e6f 6e6c 696e 6561 725f  sqfit.nonlinear_
-00007d60: 6669 7420 6174 7472 6962 7574 6529 68f1  fit attribute)h.
-00007d70: 5500 4e74 72c5 0500 0028 6ac0 0500 0058  U.Ntr....(j....X
-00007d80: 2600 0000 6572 726f 7220 286c 7371 6669  &...error (lsqfi
-00007d90: 742e 6e6f 6e6c 696e 6561 725f 6669 7420  t.nonlinear_fit 
-00007da0: 6174 7472 6962 7574 6529 6a07 0100 0055  attribute)j....U
-00007db0: 004e 7472 c605 0000 286a c005 0000 582f  .Ntr....(j....X/
-00007dc0: 0000 0066 6974 7465 725f 7265 7375 6c74  ...fitter_result
-00007dd0: 7320 286c 7371 6669 742e 6e6f 6e6c 696e  s (lsqfit.nonlin
-00007de0: 6561 725f 6669 7420 6174 7472 6962 7574  ear_fit attribut
-00007df0: 6529 6a1e 0100 0055 004e 7472 c705 0000  e)j....U.Ntr....
-00007e00: 286a c005 0000 5827 0000 006c 6f67 4742  (j....X'...logGB
-00007e10: 4620 286c 7371 6669 742e 6e6f 6e6c 696e  F (lsqfit.nonlin
-00007e20: 6561 725f 6669 7420 6174 7472 6962 7574  ear_fit attribut
-00007e30: 6529 68f9 5500 4e74 72c8 0500 0028 6ac0  e)h.U.Ntr....(j.
-00007e40: 0500 0058 2200 0000 7020 286c 7371 6669  ...X"...p (lsqfi
-00007e50: 742e 6e6f 6e6c 696e 6561 725f 6669 7420  t.nonlinear_fit 
-00007e60: 6174 7472 6962 7574 6529 6a32 0100 0055  attribute)j2...U
-00007e70: 004e 7472 c905 0000 286a c005 0000 5826  .Ntr....(j....X&
-00007e80: 0000 0070 6d65 616e 2028 6c73 7166 6974  ...pmean (lsqfit
-00007e90: 2e6e 6f6e 6c69 6e65 6172 5f66 6974 2061  .nonlinear_fit a
-00007ea0: 7474 7269 6275 7465 2968 e955 004e 7472  ttribute)h.U.Ntr
-00007eb0: ca05 0000 286a c005 0000 5826 0000 0070  ....(j....X&...p
-00007ec0: 7364 6576 2028 6c73 7166 6974 2e6e 6f6e  sdev (lsqfit.non
-00007ed0: 6c69 6e65 6172 5f66 6974 2061 7474 7269  linear_fit attri
-00007ee0: 6275 7465 296a 3c01 0000 5500 4e74 72cb  bute)j<...U.Ntr.
-00007ef0: 0500 0028 6ac0 0500 0058 2500 0000 7061  ...(j....X%...pa
-00007f00: 6c74 2028 6c73 7166 6974 2e6e 6f6e 6c69  lt (lsqfit.nonli
-00007f10: 6e65 6172 5f66 6974 2061 7474 7269 6275  near_fit attribu
-00007f20: 7465 2968 e455 004e 7472 cc05 0000 286a  te)h.U.Ntr....(j
-00007f30: c005 0000 5823 0000 0070 3020 286c 7371  ....X#...p0 (lsq
-00007f40: 6669 742e 6e6f 6e6c 696e 6561 725f 6669  fit.nonlinear_fi
-00007f50: 7420 6174 7472 6962 7574 6529 6a01 0100  t attribute)j...
-00007f60: 0055 004e 7472 cd05 0000 286a c005 0000  .U.Ntr....(j....
-00007f70: 5826 0000 0070 7269 6f72 2028 6c73 7166  X&...prior (lsqf
-00007f80: 6974 2e6e 6f6e 6c69 6e65 6172 5f66 6974  it.nonlinear_fit
-00007f90: 2061 7474 7269 6275 7465 2968 ed55 004e   attribute)h.U.N
-00007fa0: 7472 ce05 0000 286a c005 0000 5822 0000  tr....(j....X"..
-00007fb0: 0051 2028 6c73 7166 6974 2e6e 6f6e 6c69  .Q (lsqfit.nonli
-00007fc0: 6e65 6172 5f66 6974 2061 7474 7269 6275  near_fit attribu
-00007fd0: 7465 296a 0901 0000 5500 4e74 72cf 0500  te)j....U.Ntr...
-00007fe0: 0028 6ac0 0500 0058 3300 0000 7374 6f70  .(j....X3...stop
-00007ff0: 7069 6e67 5f63 7269 7465 7269 6f6e 2028  ping_criterion (
-00008000: 6c73 7166 6974 2e6e 6f6e 6c69 6e65 6172  lsqfit.nonlinear
-00008010: 5f66 6974 2061 7474 7269 6275 7465 2968  _fit attribute)h
-00008020: b355 004e 7472 d005 0000 286a c005 0000  .U.Ntr....(j....
-00008030: 582e 0000 0073 7664 636f 7272 6563 7469  X....svdcorrecti
-00008040: 6f6e 2028 6c73 7166 6974 2e6e 6f6e 6c69  on (lsqfit.nonli
-00008050: 6e65 6172 5f66 6974 2061 7474 7269 6275  near_fit attribu
-00008060: 7465 2968 cc55 004e 7472 d105 0000 286a  te)h.U.Ntr....(j
-00008070: c005 0000 5825 0000 0073 7664 6e20 286c  ....X%...svdn (l
-00008080: 7371 6669 742e 6e6f 6e6c 696e 6561 725f  sqfit.nonlinear_
-00008090: 6669 7420 6174 7472 6962 7574 6529 68f7  fit attribute)h.
-000080a0: 5500 4e74 72d2 0500 0028 6ac0 0500 0058  U.Ntr....(j....X
-000080b0: 2500 0000 7469 6d65 2028 6c73 7166 6974  %...time (lsqfit
-000080c0: 2e6e 6f6e 6c69 6e65 6172 5f66 6974 2061  .nonlinear_fit a
-000080d0: 7474 7269 6275 7465 2968 c055 004e 7472  ttribute)h.U.Ntr
-000080e0: d305 0000 286a c005 0000 5824 0000 0074  ....(j....X$...t
-000080f0: 6f6c 2028 6c73 7166 6974 2e6e 6f6e 6c69  ol (lsqfit.nonli
-00008100: 6e65 6172 5f66 6974 2061 7474 7269 6275  near_fit attribu
-00008110: 7465 296a 1501 0000 5500 4e74 72d4 0500  te)j....U.Ntr...
-00008120: 0028 6ac0 0500 0058 2200 0000 7820 286c  .(j....X"...x (l
+00000d40: bd86 581f 0000 0067 7661 722e 6164 645f  ..X....gvar.add_
+00000d50: 7061 7261 6d65 7465 725f 6469 7374 7269  parameter_distri
+00000d60: 6275 7469 6f6e 71be 682b 5808 0000 0066  butionq.h+X....f
+00000d70: 756e 6374 696f 6e71 bf86 5819 0000 006c  unctionq..X....l
+00000d80: 7371 6669 742e 6e6f 6e6c 696e 6561 725f  sqfit.nonlinear_
+00000d90: 6669 742e 7469 6d65 71c0 682b 5809 0000  fit.timeq.h+X...
+00000da0: 0061 7474 7269 6275 7465 71c1 8658 1a00  .attributeq..X..
+00000db0: 0000 6c73 7166 6974 2e73 6369 7079 5f6c  ..lsqfit.scipy_l
+00000dc0: 6561 7374 5f73 7175 6172 6573 71c2 6858  east_squaresq.hX
+00000dd0: 5805 0000 0063 6c61 7373 71c3 8658 1900  X....classq..X..
+00000de0: 0000 6c73 7166 6974 2e4d 756c 7469 4669  ..lsqfit.MultiFi
+00000df0: 7474 6572 2e6c 7371 6669 7471 c468 2b58  tter.lsqfitq.h+X
+00000e00: 0600 0000 6d65 7468 6f64 71c5 8658 1b00  ....methodq..X..
+00000e10: 0000 6c73 7166 6974 2e6e 6f6e 6c69 6e65  ..lsqfit.nonline
+00000e20: 6172 5f66 6974 2e66 6f72 6d61 7471 c668  ar_fit.formatq.h
+00000e30: 2b58 0600 0000 6d65 7468 6f64 71c7 8658  +X....methodq..X
+00000e40: 1f00 0000 6776 6172 2e64 656c 5f70 6172  ....gvar.del_par
+00000e50: 616d 6574 6572 5f64 6973 7472 6962 7574  ameter_distribut
+00000e60: 696f 6e71 c868 2b58 0800 0000 6675 6e63  ionq.h+X....func
+00000e70: 7469 6f6e 71c9 8658 2200 0000 6c73 7166  tionq..X"...lsqf
+00000e80: 6974 2e6e 6f6e 6c69 6e65 6172 5f66 6974  it.nonlinear_fit
+00000e90: 2e73 7664 636f 7272 6563 7469 6f6e 71ca  .svdcorrectionq.
+00000ea0: 682b 5809 0000 0061 7474 7269 6275 7465  h+X....attribute
+00000eb0: 71cb 8658 1400 0000 6c73 7166 6974 2e6e  q..X....lsqfit.n
+00000ec0: 6f6e 6c69 6e65 6172 5f66 6974 71cc 682b  onlinear_fitq.h+
+00000ed0: 5805 0000 0063 6c61 7373 71cd 8658 1e00  X....classq..X..
+00000ee0: 0000 6776 6172 2e61 6464 5f70 6172 616d  ..gvar.add_param
+00000ef0: 6574 6572 5f70 6172 656e 7468 6573 6573  eter_parentheses
+00000f00: 71ce 682b 5808 0000 0066 756e 6374 696f  q.h+X....functio
+00000f10: 6e71 cf86 5817 0000 006c 7371 6669 742e  nq..X....lsqfit.
+00000f20: 4d75 6c74 6946 6974 7465 724d 6f64 656c  MultiFitterModel
+00000f30: 71d0 682b 5805 0000 0063 6c61 7373 71d1  q.h+X....classq.
+00000f40: 8658 1f00 0000 6c73 7166 6974 2e42 6179  .X....lsqfit.Bay
+00000f50: 6573 496e 7465 6772 6174 6f72 2e5f 5f63  esIntegrator.__c
+00000f60: 616c 6c5f 5f71 d268 2b58 0600 0000 6d65  all__q.h+X....me
+00000f70: 7468 6f64 71d3 8658 1900 0000 6c73 7166  thodq..X....lsqf
+00000f80: 6974 2e6e 6f6e 6c69 6e65 6172 5f66 6974  it.nonlinear_fit
+00000f90: 2e63 6869 3271 d468 2b58 0900 0000 6174  .chi2q.h+X....at
+00000fa0: 7472 6962 7574 6571 d586 5822 0000 006c  tributeq..X"...l
+00000fb0: 7371 6669 742e 4d75 6c74 6946 6974 7465  sqfit.MultiFitte
+00000fc0: 722e 7072 6f63 6573 735f 6461 7461 7365  r.process_datase
+00000fd0: 7471 d668 2b58 0c00 0000 7374 6174 6963  tq.h+X....static
+00000fe0: 6d65 7468 6f64 71d7 8658 1b00 0000 6c73  methodq..X....ls
+00000ff0: 7166 6974 2e73 6369 7079 5f6d 756c 7469  qfit.scipy_multi
+00001000: 6d69 6e65 782e 6e69 7471 d868 5858 0900  minex.nitq.hXX..
+00001010: 0000 6174 7472 6962 7574 6571 d986 581e  ..attributeq..X.
+00001020: 0000 006c 7371 6669 742e 7363 6970 795f  ...lsqfit.scipy_
+00001030: 6c65 6173 745f 7371 7561 7265 732e 6e69  least_squares.ni
+00001040: 7471 da68 5858 0900 0000 6174 7472 6962  tq.hXX....attrib
+00001050: 7574 6571 db86 5824 0000 006c 7371 6669  uteq..X$...lsqfi
+00001060: 742e 4d75 6c74 6946 6974 7465 724d 6f64  t.MultiFitterMod
+00001070: 656c 2e62 7569 6c64 6461 7461 7365 7471  el.builddatasetq
+00001080: dc68 2b58 0600 0000 6d65 7468 6f64 71dd  .h+X....methodq.
+00001090: 8658 1c00 0000 6c73 7166 6974 2e73 6369  .X....lsqfit.sci
+000010a0: 7079 5f6c 6561 7374 5f73 7175 6172 6573  py_least_squares
+000010b0: 2e4a 71de 6858 5809 0000 0061 7474 7269  .Jq.hXX....attri
+000010c0: 6275 7465 71df 8658 2000 0000 6c73 7166  buteq..X ...lsqf
+000010d0: 6974 2e73 6369 7079 5f6c 6561 7374 5f73  it.scipy_least_s
+000010e0: 7175 6172 6573 2e65 7272 6f72 71e0 6858  quares.errorq.hX
+000010f0: 5809 0000 0061 7474 7269 6275 7465 71e1  X....attributeq.
+00001100: 8658 1900 0000 6c73 7166 6974 2e6e 6f6e  .X....lsqfit.non
+00001110: 6c69 6e65 6172 5f66 6974 2e70 616c 7471  linear_fit.paltq
+00001120: e268 2b58 0900 0000 6174 7472 6962 7574  .h+X....attribut
+00001130: 6571 e386 5822 0000 006c 7371 6669 742e  eq..X"...lsqfit.
+00001140: 4d75 6c74 6946 6974 7465 724d 6f64 656c  MultiFitterModel
+00001150: 2e62 7569 6c64 7072 696f 7271 e468 2b58  .buildpriorq.h+X
+00001160: 0600 0000 6d65 7468 6f64 71e5 8658 1300  ....methodq..X..
+00001170: 0000 6c73 7166 6974 2e67 736c 5f6d 756c  ..lsqfit.gsl_mul
+00001180: 7469 6669 7471 e668 7158 0500 0000 636c  tifitq.hqX....cl
+00001190: 6173 7386 581a 0000 006c 7371 6669 742e  ass.X....lsqfit.
+000011a0: 6e6f 6e6c 696e 6561 725f 6669 742e 706d  nonlinear_fit.pm
+000011b0: 6561 6e71 e768 2b58 0900 0000 6174 7472  eanq.h+X....attr
+000011c0: 6962 7574 6571 e886 581a 0000 006c 7371  ibuteq..X....lsq
+000011d0: 6669 742e 6e6f 6e6c 696e 6561 725f 6669  fit.nonlinear_fi
+000011e0: 742e 7072 696f 7271 e968 2b58 0900 0000  t.priorq.h+X....
+000011f0: 6174 7472 6962 7574 6571 ea86 5826 0000  attributeq..X&..
+00001200: 006c 7371 6669 742e 7363 6970 795f 6c65  .lsqfit.scipy_le
+00001210: 6173 745f 7371 7561 7265 732e 6465 7363  ast_squares.desc
+00001220: 7269 7074 696f 6e71 eb68 5858 0900 0000  riptionq.hXX....
+00001230: 6174 7472 6962 7574 6571 ec86 5818 0000  attributeq..X...
+00001240: 006c 7371 6669 742e 6e6f 6e6c 696e 6561  .lsqfit.nonlinea
+00001250: 725f 6669 742e 646f 6671 ed68 2b58 0900  r_fit.dofq.h+X..
+00001260: 0000 6174 7472 6962 7574 6571 ee86 580b  ..attributeq..X.
+00001270: 0000 006c 7371 6669 742e 7761 7667 71ef  ...lsqfit.wavgq.
+00001280: 682b 5808 0000 0066 756e 6374 696f 6e71  h+X....functionq
+00001290: f086 580d 0000 006c 7371 6669 742e 6761  ..X....lsqfit.ga
+000012a0: 6d6d 6151 71f1 682b 5808 0000 0066 756e  mmaQq.h+X....fun
+000012b0: 6374 696f 6e71 f286 5819 0000 006c 7371  ctionq..X....lsq
+000012c0: 6669 742e 6e6f 6e6c 696e 6561 725f 6669  fit.nonlinear_fi
+000012d0: 742e 7376 646e 71f3 682b 5809 0000 0061  t.svdnq.h+X....a
+000012e0: 7474 7269 6275 7465 71f4 8658 1b00 0000  ttributeq..X....
+000012f0: 6c73 7166 6974 2e6e 6f6e 6c69 6e65 6172  lsqfit.nonlinear
+00001300: 5f66 6974 2e6c 6f67 4742 4671 f568 2b58  _fit.logGBFq.h+X
+00001310: 0900 0000 6174 7472 6962 7574 6571 f686  ....attributeq..
+00001320: 5826 0000 006c 7371 6669 742e 4d75 6c74  X&...lsqfit.Mult
+00001330: 6946 6974 7465 724d 6f64 656c 2e67 6574  iFitterModel.get
+00001340: 5f70 7269 6f72 5f6b 6579 7371 f768 2b58  _prior_keysq.h+X
+00001350: 0c00 0000 7374 6174 6963 6d65 7468 6f64  ....staticmethod
+00001360: 71f8 8658 1200 0000 6c73 7166 6974 2e4d  q..X....lsqfit.M
+00001370: 756c 7469 4669 7474 6572 71f9 682b 5805  ultiFitterq.h+X.
+00001380: 0000 0063 6c61 7373 71fa 8658 2700 0000  ...classq..X'...
+00001390: 6c73 7166 6974 2e6e 6f6e 6c69 6e65 6172  lsqfit.nonlinear
+000013a0: 5f66 6974 2e73 696d 756c 6174 6564 5f66  _fit.simulated_f
+000013b0: 6974 5f69 7465 7271 fb68 2b58 0600 0000  it_iterq.h+X....
+000013c0: 6d65 7468 6f64 71fc 8658 1700 0000 6c73  methodq..X....ls
+000013d0: 7166 6974 2e6e 6f6e 6c69 6e65 6172 5f66  qfit.nonlinear_f
+000013e0: 6974 2e70 3071 fd68 2b58 0900 0000 6174  it.p0q.h+X....at
+000013f0: 7472 6962 7574 6571 fe86 582a 0000 006c  tributeq..X*...l
+00001400: 7371 6669 742e 6e6f 6e6c 696e 6561 725f  sqfit.nonlinear_
+00001410: 6669 742e 626f 6f74 7374 7261 7070 6564  fit.bootstrapped
+00001420: 5f66 6974 5f69 7465 7271 ff68 2b58 0600  _fit_iterq.h+X..
+00001430: 0000 6d65 7468 6f64 7200 0100 0086 581f  ..methodr.....X.
+00001440: 0000 006c 7371 6669 742e 4d75 6c74 6946  ...lsqfit.MultiF
+00001450: 6974 7465 722e 7072 6f63 6573 735f 6461  itter.process_da
+00001460: 7461 7201 0100 0068 2b58 0c00 0000 7374  tar....h+X....st
+00001470: 6174 6963 6d65 7468 6f64 7202 0100 0086  aticmethodr.....
+00001480: 581a 0000 006c 7371 6669 742e 6e6f 6e6c  X....lsqfit.nonl
+00001490: 696e 6561 725f 6669 742e 6572 726f 7272  inear_fit.errorr
+000014a0: 0301 0000 682b 5809 0000 0061 7474 7269  ....h+X....attri
+000014b0: 6275 7465 7204 0100 0086 5816 0000 006c  buter.....X....l
+000014c0: 7371 6669 742e 6e6f 6e6c 696e 6561 725f  sqfit.nonlinear_
+000014d0: 6669 742e 5172 0501 0000 682b 5809 0000  fit.Qr....h+X...
+000014e0: 0061 7474 7269 6275 7465 7206 0100 0086  .attributer.....
+000014f0: 5821 0000 006c 7371 6669 742e 4d75 6c74  X!...lsqfit.Mult
+00001500: 6946 6974 7465 724d 6f64 656c 2e70 7269  iFitterModel.pri
+00001510: 6f72 5f6b 6579 7207 0100 0068 2b58 0c00  or_keyr....h+X..
+00001520: 0000 7374 6174 6963 6d65 7468 6f64 7208  ..staticmethodr.
+00001530: 0100 0086 5817 0000 006c 7371 6669 742e  ....X....lsqfit.
+00001540: 7363 6970 795f 6d75 6c74 696d 696e 6578  scipy_multiminex
+00001550: 7209 0100 0068 5858 0500 0000 636c 6173  r....hXX....clas
+00001560: 7372 0a01 0000 8658 1d00 0000 6c73 7166  sr.....X....lsqf
+00001570: 6974 2e4d 756c 7469 4669 7474 6572 2e73  it.MultiFitter.s
+00001580: 686f 775f 706c 6f74 7372 0b01 0000 682b  how_plotsr....h+
+00001590: 580c 0000 0073 7461 7469 636d 6574 686f  X....staticmetho
+000015a0: 6472 0c01 0000 8658 1600 0000 6c73 7166  dr.....X....lsqf
+000015b0: 6974 2e42 6179 6573 496e 7465 6772 6174  it.BayesIntegrat
+000015c0: 6f72 720d 0100 0068 2b58 0500 0000 636c  orr....h+X....cl
+000015d0: 6173 7372 0e01 0000 8658 1c00 0000 6c73  assr.....X....ls
+000015e0: 7166 6974 2e73 6369 7079 5f6c 6561 7374  qfit.scipy_least
+000015f0: 5f73 7175 6172 6573 2e78 720f 0100 0068  _squares.xr....h
+00001600: 5858 0900 0000 6174 7472 6962 7574 6572  XX....attributer
+00001610: 1001 0000 8658 1800 0000 6c73 7166 6974  .....X....lsqfit
+00001620: 2e6e 6f6e 6c69 6e65 6172 5f66 6974 2e74  .nonlinear_fit.t
+00001630: 6f6c 7211 0100 0068 2b58 0900 0000 6174  olr....h+X....at
+00001640: 7472 6962 7574 6572 1201 0000 8658 1e00  tributer.....X..
+00001650: 0000 6c73 7166 6974 2e4d 756c 7469 4669  ..lsqfit.MultiFi
+00001660: 7474 6572 4d6f 6465 6c2e 6669 7466 636e  tterModel.fitfcn
+00001670: 7213 0100 0068 2b58 0600 0000 6d65 7468  r....h+X....meth
+00001680: 6f64 7214 0100 0086 5816 0000 006c 7371  odr.....X....lsq
+00001690: 6669 742e 6773 6c5f 7631 5f6d 756c 7469  fit.gsl_v1_multi
+000016a0: 6669 7472 1501 0000 6871 5805 0000 0063  fitr....hqX....c
+000016b0: 6c61 7373 8658 1800 0000 6c73 7166 6974  lass.X....lsqfit
+000016c0: 2e6e 6f6e 6c69 6e65 6172 5f66 6974 2e73  .nonlinear_fit.s
+000016d0: 6574 7216 0100 0068 2b58 0c00 0000 7374  etr....h+X....st
+000016e0: 6174 6963 6d65 7468 6f64 7217 0100 0086  aticmethodr.....
+000016f0: 5819 0000 006c 7371 6669 742e 7363 6970  X....lsqfit.scip
+00001700: 795f 6d75 6c74 696d 696e 6578 2e78 7218  y_multiminex.xr.
+00001710: 0100 0068 5858 0900 0000 6174 7472 6962  ...hXX....attrib
+00001720: 7574 6572 1901 0000 8658 2300 0000 6c73  uter.....X#...ls
+00001730: 7166 6974 2e6e 6f6e 6c69 6e65 6172 5f66  qfit.nonlinear_f
+00001740: 6974 2e66 6974 7465 725f 7265 7375 6c74  it.fitter_result
+00001750: 7372 1a01 0000 682b 5809 0000 0061 7474  sr....h+X....att
+00001760: 7269 6275 7465 721b 0100 0086 580f 0000  ributer.....X...
+00001770: 006c 7371 6669 742e 4261 7965 7350 4446  .lsqfit.BayesPDF
+00001780: 721c 0100 0068 2b58 0500 0000 636c 6173  r....h+X....clas
+00001790: 7372 1d01 0000 8658 2100 0000 6c73 7166  sr.....X!...lsqf
+000017a0: 6974 2e4d 756c 7469 4669 7474 6572 4d6f  it.MultiFitterMo
+000017b0: 6465 6c2e 6275 696c 6464 6174 6172 1e01  del.builddatar..
+000017c0: 0000 682b 5806 0000 006d 6574 686f 6472  ..h+X....methodr
+000017d0: 1f01 0000 8658 1800 0000 6c73 7166 6974  .....X....lsqfit
+000017e0: 2e42 6179 6573 5044 462e 5f5f 6361 6c6c  .BayesPDF.__call
+000017f0: 5f5f 7220 0100 0068 2b58 0600 0000 6d65  __r ...h+X....me
+00001800: 7468 6f64 7221 0100 0086 581e 0000 006c  thodr!....X....l
+00001810: 7371 6669 742e 7363 6970 795f 6c65 6173  sqfit.scipy_leas
+00001820: 745f 7371 7561 7265 732e 636f 7672 2201  t_squares.covr".
+00001830: 0000 6858 5809 0000 0061 7474 7269 6275  ..hXX....attribu
+00001840: 7465 7223 0100 0086 5821 0000 006c 7371  ter#....X!...lsq
+00001850: 6669 742e 4d75 6c74 6946 6974 7465 722e  fit.MultiFitter.
+00001860: 666c 6174 7465 6e5f 6d6f 6465 6c73 7224  flatten_modelsr$
+00001870: 0100 0068 2b58 0c00 0000 7374 6174 6963  ...h+X....static
+00001880: 6d65 7468 6f64 7225 0100 0086 5816 0000  methodr%....X...
+00001890: 006c 7371 6669 742e 6e6f 6e6c 696e 6561  .lsqfit.nonlinea
+000018a0: 725f 6669 742e 7872 2601 0000 682b 5809  r_fit.xr&...h+X.
+000018b0: 0000 0061 7474 7269 6275 7465 7227 0100  ...attributer'..
+000018c0: 0086 5813 0000 006c 7371 6669 742e 656d  ..X....lsqfit.em
+000018d0: 7062 6179 6573 5f66 6974 7228 0100 0068  pbayes_fitr(...h
+000018e0: 2b58 0800 0000 6675 6e63 7469 6f6e 7229  +X....functionr)
+000018f0: 0100 0086 581b 0000 006c 7371 6669 742e  ....X....lsqfit.
+00001900: 4d75 6c74 6946 6974 7465 724d 6f64 656c  MultiFitterModel
+00001910: 2e6e 6367 722a 0100 0068 2b58 0900 0000  .ncgr*...h+X....
+00001920: 6174 7472 6962 7574 6572 2b01 0000 8658  attributer+....X
+00001930: 2100 0000 6c73 7166 6974 2e4d 756c 7469  !...lsqfit.Multi
+00001940: 4669 7474 6572 2e63 6861 696e 6564 5f6c  Fitter.chained_l
+00001950: 7371 6669 7472 2c01 0000 682b 5806 0000  sqfitr,...h+X...
+00001960: 006d 6574 686f 6472 2d01 0000 8658 1600  .methodr-....X..
+00001970: 0000 6c73 7166 6974 2e6e 6f6e 6c69 6e65  ..lsqfit.nonline
+00001980: 6172 5f66 6974 2e70 722e 0100 0068 2b58  ar_fit.pr....h+X
+00001990: 0900 0000 6174 7472 6962 7574 6572 2f01  ....attributer/.
+000019a0: 0000 8658 1c00 0000 6c73 7166 6974 2e6e  ...X....lsqfit.n
+000019b0: 6f6e 6c69 6e65 6172 5f66 6974 2e6e 626c  onlinear_fit.nbl
+000019c0: 6f63 6b73 7230 0100 0068 2b58 0900 0000  ocksr0...h+X....
+000019d0: 6174 7472 6962 7574 6572 3101 0000 8658  attributer1....X
+000019e0: 1f00 0000 6c73 7166 6974 2e4d 756c 7469  ....lsqfit.Multi
+000019f0: 4669 7474 6572 4d6f 6465 6c2e 6461 7461  FitterModel.data
+00001a00: 7461 6772 3201 0000 682b 5809 0000 0061  tagr2...h+X....a
+00001a10: 7474 7269 6275 7465 7233 0100 0086 5819  ttributer3....X.
+00001a20: 0000 006c 7371 6669 742e 7363 6970 795f  ...lsqfit.scipy_
+00001a30: 6d75 6c74 696d 696e 6578 2e66 7234 0100  multiminex.fr4..
+00001a40: 0068 5858 0900 0000 6174 7472 6962 7574  .hXX....attribut
+00001a50: 6572 3501 0000 8658 1600 0000 6c73 7166  er5....X....lsqf
+00001a60: 6974 2e6e 6f6e 6c69 6e65 6172 5f66 6974  it.nonlinear_fit
+00001a70: 2e79 7236 0100 0068 2b58 0900 0000 6174  .yr6...h+X....at
+00001a80: 7472 6962 7574 6572 3701 0000 8658 1a00  tributer7....X..
+00001a90: 0000 6c73 7166 6974 2e6e 6f6e 6c69 6e65  ..lsqfit.nonline
+00001aa0: 6172 5f66 6974 2e70 7364 6576 7238 0100  ar_fit.psdevr8..
+00001ab0: 0068 2b58 0900 0000 6174 7472 6962 7574  .h+X....attribut
+00001ac0: 6572 3901 0000 8675 5507 6d6f 6475 6c65  er9....uU.module
+00001ad0: 7372 3a01 0000 7d72 3b01 0000 68af 2868  sr:...}r;...h.(h
+00001ae0: 2b63 646f 6375 7469 6c73 2e6e 6f64 6573  +cdocutils.nodes
+00001af0: 0a72 6570 7275 6e69 636f 6465 0a72 3c01  .reprunicode.r<.
+00001b00: 0000 5820 0000 004e 6f6e 6c69 6e65 6172  ..X ...Nonlinear
+00001b10: 206c 6561 7374 2073 7175 6172 6573 2066   least squares f
+00001b20: 6974 7469 6e67 2e72 3d01 0000 8581 723e  itting.r=.....r>
+00001b30: 0100 007d 723f 0100 0062 5500 8974 7368  ...}r?...bU..tsh
+00001b40: 924b 0075 5502 6a73 7240 0100 007d 7241  .K.uU.jsr@...}rA
+00001b50: 0100 0028 68a2 7d6a 3a01 0000 7d68 924b  ...(h.}j:...}h.K
+00001b60: 0075 5503 6370 7072 4201 0000 7d72 4301  .uU.cpprB...}rC.
+00001b70: 0000 2855 0b72 6f6f 745f 7379 6d62 6f6c  ..(U.root_symbol
+00001b80: 7244 0100 0063 7370 6869 6e78 2e64 6f6d  rD...csphinx.dom
+00001b90: 6169 6e73 2e63 7070 0a53 796d 626f 6c0a  ains.cpp.Symbol.
+00001ba0: 7245 0100 0029 8172 4601 0000 7d72 4701  rE...).rF...}rG.
+00001bb0: 0000 2855 0f69 7352 6564 6563 6c61 7261  ..(U.isRedeclara
+00001bc0: 7469 6f6e 7248 0100 0089 550e 7465 6d70  tionrH....U.temp
+00001bd0: 6c61 7465 5061 7261 6d73 7249 0100 004e  lateParamsrI...N
+00001be0: 681f 4e55 0c74 656d 706c 6174 6541 7267  h.NU.templateArg
+00001bf0: 7372 4a01 0000 4e55 0b64 6563 6c61 7261  srJ...NU.declara
+00001c00: 7469 6f6e 724b 0100 004e 5507 646f 636e  tionrK...NU.docn
+00001c10: 616d 6572 4c01 0000 4e55 0969 6465 6e74  amerL...NU.ident
+00001c20: 4f72 4f70 724d 0100 004e 6818 5d75 6268  OrOprM...Nh.]ubh
+00001c30: 924b 0068 177d 7555 0372 7374 724e 0100  .K.h.}uU.rstrN..
+00001c40: 007d 724f 0100 0028 68a2 7d68 924b 0075  .}rO...(h.}h.K.u
+00001c50: 5504 6d61 7468 7250 0100 007d 7251 0100  U.mathrP...}rQ..
+00001c60: 0028 68a2 7d68 924b 0075 7555 0d67 6c6f  .(h.}h.K.uuU.glo
+00001c70: 625f 746f 6374 7265 6573 7252 0100 0068  b_toctreesrR...h
+00001c80: 075d 8552 7253 0100 0055 0d72 6572 6561  .].RrS...U.rerea
+00001c90: 645f 616c 7761 7973 7254 0100 0068 075d  d_alwaysrT...h.]
+00001ca0: 8552 7255 0100 0055 0a64 6f63 7472 6565  .RrU...U.doctree
+00001cb0: 6469 7272 5601 0000 5834 0000 002f 5573  dirrV...X4.../Us
+00001cc0: 6572 732f 6770 6c2f 736f 6674 7761 7265  ers/gpl/software
+00001cd0: 2f70 7974 686f 6e2f 6c73 7166 6974 2f64  /python/lsqfit/d
+00001ce0: 6f63 2f68 746d 6c2f 2e64 6f63 7472 6565  oc/html/.doctree
+00001cf0: 7372 5701 0000 5514 7665 7273 696f 6e69  srW...U.versioni
+00001d00: 6e67 5f63 6f6e 6469 7469 6f6e 7258 0100  ng_conditionrX..
+00001d10: 0089 550e 746f 635f 6669 676e 756d 6265  ..U.toc_fignumbe
+00001d20: 7273 7259 0100 007d 5509 7465 6d70 5f64  rsrY...}U.temp_d
+00001d30: 6174 6172 5a01 0000 7d55 126f 7269 6769  atarZ...}U.origi
+00001d40: 6e61 6c5f 696d 6167 655f 7572 6972 5b01  nal_image_urir[.
+00001d50: 0000 7d68 924b 3455 0673 7263 6469 7272  ..}h.K4U.srcdirr
+00001d60: 5c01 0000 582c 0000 002f 5573 6572 732f  \...X,.../Users/
+00001d70: 6770 6c2f 736f 6674 7761 7265 2f70 7974  gpl/software/pyt
+00001d80: 686f 6e2f 6c73 7166 6974 2f64 6f63 2f73  hon/lsqfit/doc/s
+00001d90: 6f75 7263 6572 5d01 0000 5506 636f 6e66  ourcer]...U.conf
+00001da0: 6967 725e 0100 0063 7370 6869 6e78 2e63  igr^...csphinx.c
+00001db0: 6f6e 6669 670a 436f 6e66 6967 0a72 5f01  onfig.Config.r_.
+00001dc0: 0000 2981 7260 0100 007d 7261 0100 0028  ..).r`...}ra...(
+00001dd0: 5521 6e61 706f 6c65 6f6e 5f69 6e63 6c75  U!napoleon_inclu
+00001de0: 6465 5f70 7269 7661 7465 5f77 6974 685f  de_private_with_
+00001df0: 646f 6372 6201 0000 8955 216e 6170 6f6c  docrb....U!napol
+00001e00: 656f 6e5f 696e 636c 7564 655f 7370 6563  eon_include_spec
+00001e10: 6961 6c5f 7769 7468 5f64 6f63 7263 0100  ial_with_docrc..
+00001e20: 0088 5518 6e61 706f 6c65 6f6e 5f6e 756d  ..U.napoleon_num
+00001e30: 7079 5f64 6f63 7374 7269 6e67 7264 0100  py_docstringrd..
+00001e40: 0088 550e 7079 676d 656e 7473 5f73 7479  ..U.pygments_sty
+00001e50: 6c65 7265 0100 0055 0673 7068 696e 7872  lere...U.sphinxr
+00001e60: 6601 0000 5526 6e61 706f 6c65 6f6e 5f75  f...U&napoleon_u
+00001e70: 7365 5f61 646d 6f6e 6974 696f 6e5f 666f  se_admonition_fo
+00001e80: 725f 7265 6665 7265 6e63 6573 7267 0100  r_referencesrg..
+00001e90: 0089 5513 696d 676d 6174 685f 6476 6970  ..U.imgmath_dvip
+00001ea0: 6e67 5f61 7267 7372 6801 0000 5d72 6901  ng_argsrh...]ri.
+00001eb0: 0000 2855 062d 6761 6d6d 6172 6a01 0000  ..(U.-gammarj...
+00001ec0: 5504 302e 3335 726b 0100 0055 022d 4472  U.0.35rk...U.-Dr
+00001ed0: 6c01 0000 5503 3131 3072 6d01 0000 5503  l...U.110rm...U.
+00001ee0: 2d62 6772 6e01 0000 550b 5472 616e 7370  -bgrn...U.Transp
+00001ef0: 6172 656e 7472 6f01 0000 6555 1669 6d67  arentro...eU.img
+00001f00: 6d61 7468 5f6c 6174 6578 5f70 7265 616d  math_latex_pream
+00001f10: 626c 6572 7001 0000 5511 5c75 7365 7061  blerp...U.\usepa
+00001f20: 636b 6167 657b 6172 6576 7d55 246e 6170  ckage{arev}U$nap
+00001f30: 6f6c 656f 6e5f 7573 655f 6164 6d6f 6e69  oleon_use_admoni
+00001f40: 7469 6f6e 5f66 6f72 5f65 7861 6d70 6c65  tion_for_example
+00001f50: 7372 7101 0000 8955 0a6d 6173 7465 725f  srq....U.master_
+00001f60: 646f 6372 7201 0000 5505 696e 6465 7872  docrr...U.indexr
+00001f70: 7301 0000 5512 6e61 706f 6c65 6f6e 5f75  s...U.napoleon_u
+00001f80: 7365 5f72 7479 7065 7274 0100 0088 550d  se_rtypert....U.
+00001f90: 736f 7572 6365 5f73 7566 6669 7872 7501  source_suffixru.
+00001fa0: 0000 5d72 7601 0000 5504 2e72 7374 7277  ..]rv...U..rstrw
+00001fb0: 0100 0061 5509 636f 7079 7269 6768 7472  ...aU.copyrightr
+00001fc0: 7801 0000 5817 0000 0032 3030 392d 3230  x...X....2009-20
+00001fd0: 3138 2c20 472e 2050 2e20 4c65 7061 6765  18, G. P. Lepage
+00001fe0: 6892 5503 392e 3572 7901 0000 5514 696d  h.U.9.5ry...U.im
+00001ff0: 676d 6174 685f 696d 6167 655f 666f 726d  gmath_image_form
+00002000: 6174 727a 0100 0055 0370 6e67 727b 0100  atrz...U.pngr{..
+00002010: 0055 0a68 746d 6c5f 7468 656d 6572 7c01  .U.html_themer|.
+00002020: 0000 5507 7079 7261 6d69 6472 7d01 0000  ..U.pyramidr}...
+00002030: 5519 6e61 706f 6c65 6f6e 5f67 6f6f 676c  U.napoleon_googl
+00002040: 655f 646f 6373 7472 696e 6772 7e01 0000  e_docstringr~...
+00002050: 8855 126e 6170 6f6c 656f 6e5f 7573 655f  .U.napoleon_use_
+00002060: 7061 7261 6d72 7f01 0000 8855 0e74 656d  paramr.....U.tem
+00002070: 706c 6174 6573 5f70 6174 6872 8001 0000  plates_pathr....
+00002080: 5d72 8101 0000 550a 5f74 656d 706c 6174  ]r....U._templat
+00002090: 6573 7282 0100 0061 550f 6c61 7465 785f  esr....aU.latex_
+000020a0: 646f 6375 6d65 6e74 7372 8301 0000 5d72  documentsr....]r
+000020b0: 8401 0000 286a 7301 0000 550a 6c73 7166  ....(js...U.lsqf
+000020c0: 6974 2e74 6578 5814 0000 006c 7371 6669  it.texX....lsqfi
+000020d0: 7420 446f 6375 6d65 6e74 6174 696f 6e58  t DocumentationX
+000020e0: 0c00 0000 472e 2050 2e20 4c65 7061 6765  ....G. P. Lepage
+000020f0: 5506 6d61 6e75 616c 7285 0100 0074 7286  U.manualr....tr.
+00002100: 0100 0061 5511 6e61 706f 6c65 6f6e 5f75  ...aU.napoleon_u
+00002110: 7365 5f69 7661 7272 8701 0000 8955 1068  se_ivarr.....U.h
+00002120: 746d 6c5f 7374 6174 6963 5f70 6174 6872  tml_static_pathr
+00002130: 8801 0000 5d72 8901 0000 5507 5f73 7461  ....]r....U._sta
+00002140: 7469 6372 8a01 0000 6155 096f 7665 7272  ticr....aU.overr
+00002150: 6964 6573 728b 0100 007d 5511 6874 6d6c  idesr....}U.html
+00002160: 6865 6c70 5f62 6173 656e 616d 6572 8c01  help_basenamer..
+00002170: 0000 5509 6c73 7166 6974 646f 6355 1369  ..U.lsqfitdocU.i
+00002180: 6d67 6d61 7468 5f75 7365 5f70 7265 7669  mgmath_use_previ
+00002190: 6577 728d 0100 0088 5507 7072 6f6a 6563  ewr.....U.projec
+000021a0: 7472 8e01 0000 5806 0000 006c 7371 6669  tr....X....lsqfi
+000021b0: 7455 0a65 7874 656e 7369 6f6e 7372 8f01  tU.extensionsr..
+000021c0: 0000 5d72 9001 0000 2855 1273 7068 696e  ..]r....(U.sphin
+000021d0: 782e 6578 742e 6175 746f 646f 6372 9101  x.ext.autodocr..
+000021e0: 0000 5513 7370 6869 6e78 2e65 7874 2e6e  ..U.sphinx.ext.n
+000021f0: 6170 6f6c 656f 6e72 9201 0000 5512 7370  apoleonr....U.sp
+00002200: 6869 6e78 2e65 7874 2e69 6d67 6d61 7468  hinx.ext.imgmath
+00002210: 7293 0100 0065 5507 7265 6c65 6173 6572  r....eU.releaser
+00002220: 9401 0000 6a79 0100 0055 216e 6170 6f6c  ....jy...U!napol
+00002230: 656f 6e5f 7573 655f 6164 6d6f 6e69 7469  eon_use_admoniti
+00002240: 6f6e 5f66 6f72 5f6e 6f74 6573 7295 0100  on_for_notesr...
+00002250: 0089 5505 7365 7475 7072 9601 0000 4e75  ..U.setupr....Nu
+00002260: 6255 086d 6574 6164 6174 6172 9701 0000  bU.metadatar....
+00002270: 6363 6f6c 6c65 6374 696f 6e73 0a64 6566  ccollections.def
+00002280: 6175 6c74 6469 6374 0a72 9801 0000 635f  aultdict.r....c_
+00002290: 5f62 7569 6c74 696e 5f5f 0a64 6963 740a  _builtin__.dict.
+000022a0: 7299 0100 0085 5272 9a01 0000 2868 0c7d  r.....Rr....(h.}
+000022b0: 729b 0100 0068 227d 729c 0100 0068 2b7d  r....h"}r....h+}
+000022c0: 729d 0100 0068 3d7d 729e 0100 0068 467d  r....h=}r....hF}
+000022d0: 729f 0100 0068 4f7d 72a0 0100 0068 587d  r....hO}r....hX}
+000022e0: 72a1 0100 0068 687d 72a2 0100 0068 717d  r....hh}r....hq}
+000022f0: 72a3 0100 0075 550e 7665 7273 696f 6e63  r....uU.versionc
+00002300: 6861 6e67 6573 72a4 0100 007d 550f 746f  hangesr....}U.to
+00002310: 635f 6e75 6d5f 656e 7472 6965 7372 a501  c_num_entriesr..
+00002320: 0000 7d72 a601 0000 2868 0c4b 0268 224b  ..}r....(h.K.h"K
+00002330: 0568 2b4b 0768 3d4b 0e68 464b 0668 4f4b  .h+K.h=K.hFK.hOK
+00002340: 0468 584b 0368 684b 0468 714b 0375 5506  .hXK.hhK.hqK.uU.
+00002350: 696d 6167 6573 72a7 0100 0068 0529 8172  imagesr....h.).r
+00002360: a801 0000 2858 1100 0000 6567 2d61 7070  ....(X....eg-app
+00002370: 656e 6469 7831 632e 706e 6772 a901 0000  endix1c.pngr....
+00002380: 6807 5d72 aa01 0000 6846 6185 5272 ab01  h.]r....hFa.Rr..
+00002390: 0000 6aa9 0100 0086 72ac 0100 0058 1100  ..j.....r....X..
+000023a0: 0000 6567 2d61 7070 656e 6469 7831 622e  ..eg-appendix1b.
+000023b0: 706e 6772 ad01 0000 6807 5d72 ae01 0000  pngr....h.]r....
+000023c0: 6846 6185 5272 af01 0000 6aad 0100 0086  hFa.Rr....j.....
+000023d0: 72b0 0100 0058 1100 0000 6567 2d61 7070  r....X....eg-app
+000023e0: 656e 6469 7831 612e 706e 6772 b101 0000  endix1a.pngr....
+000023f0: 6807 5d72 b201 0000 6846 6185 5272 b301  h.]r....hFa.Rr..
+00002400: 0000 6ab1 0100 0086 72b4 0100 0058 0800  ..j.....r....X..
+00002410: 0000 6567 3364 2e70 6e67 72b5 0100 0068  ..eg3d.pngr....h
+00002420: 075d 72b6 0100 0068 2261 8552 72b7 0100  .]r....h"a.Rr...
+00002430: 006a b501 0000 8672 b801 0000 5811 0000  .j.....r....X...
+00002440: 0065 672d 6170 7065 6e64 6978 3164 2e70  .eg-appendix1d.p
+00002450: 6e67 72b9 0100 0068 075d 72ba 0100 0068  ngr....h.]r....h
+00002460: 4661 8552 72bb 0100 006a b901 0000 8672  Fa.Rr....j.....r
+00002470: bc01 0000 5808 0000 0065 6733 652e 706e  ....X....eg3e.pn
+00002480: 6772 bd01 0000 6807 5d72 be01 0000 6822  gr....h.]r....h"
+00002490: 6185 5272 bf01 0000 6abd 0100 0086 72c0  a.Rr....j.....r.
+000024a0: 0100 0058 0700 0000 6567 312e 706e 6772  ...X....eg1.pngr
+000024b0: c101 0000 6807 5d72 c201 0000 683d 6185  ....h.]r....h=a.
+000024c0: 5272 c301 0000 6ac1 0100 0086 72c4 0100  Rr....j.....r...
+000024d0: 0058 0700 0000 6567 322e 706e 6772 c501  .X....eg2.pngr..
+000024e0: 0000 6807 5d72 c601 0000 683d 6185 5272  ..h.]r....h=a.Rr
+000024f0: c701 0000 6ac5 0100 0086 72c8 0100 0058  ....j.....r....X
+00002500: 0700 0000 6567 332e 706e 6772 c901 0000  ....eg3.pngr....
+00002510: 6807 5d72 ca01 0000 683d 6185 5272 cb01  h.]r....h=a.Rr..
+00002520: 0000 6ac9 0100 0086 72cc 0100 0058 1200  ..j.....r....X..
+00002530: 0000 6361 7365 2d6f 7574 6c69 6572 7331  ..case-outliers1
+00002540: 2e70 6e67 72cd 0100 0068 075d 72ce 0100  .pngr....h.]r...
+00002550: 0068 4f61 8552 72cf 0100 006a cd01 0000  .hOa.Rr....j....
+00002560: 8672 d001 0000 5810 0000 0063 6173 652d  .r....X....case-
+00002570: 7065 6e64 756c 756d 2e70 7972 d101 0000  pendulum.pyr....
+00002580: 6807 5d72 d201 0000 6868 6185 5272 d301  h.]r....hha.Rr..
+00002590: 0000 6ad1 0100 0086 72d4 0100 0058 1100  ..j.....r....X..
+000025a0: 0000 6361 7365 2d70 656e 6475 6c75 6d2e  ..case-pendulum.
+000025b0: 706e 6772 d501 0000 6807 5d72 d601 0000  pngr....h.]r....
+000025c0: 6868 6185 5272 d701 0000 6ad5 0100 0086  hha.Rr....j.....
+000025d0: 72d8 0100 0058 1100 0000 6567 2d61 7070  r....X....eg-app
+000025e0: 656e 6469 7831 642e 6f75 7472 d901 0000  endix1d.outr....
+000025f0: 6807 5d72 da01 0000 6846 6185 5272 db01  h.]r....hFa.Rr..
+00002600: 0000 6ad9 0100 0086 72dc 0100 0058 0700  ..j.....r....X..
+00002610: 0000 6567 362e 706e 6772 dd01 0000 6807  ..eg6.pngr....h.
+00002620: 5d72 de01 0000 6822 6185 5272 df01 0000  ]r....h"a.Rr....
+00002630: 6add 0100 0086 72e0 0100 0058 1100 0000  j.....r....X....
+00002640: 6567 2d61 7070 656e 6469 7831 622e 6f75  eg-appendix1b.ou
+00002650: 7472 e101 0000 6807 5d72 e201 0000 6846  tr....h.]r....hF
+00002660: 6185 5272 e301 0000 6ae1 0100 0086 72e4  a.Rr....j.....r.
+00002670: 0100 0058 1100 0000 6567 2d61 7070 656e  ...X....eg-appen
+00002680: 6469 7831 632e 6f75 7472 e501 0000 6807  dix1c.outr....h.
+00002690: 5d72 e601 0000 6846 6185 5272 e701 0000  ]r....hFa.Rr....
+000026a0: 6ae5 0100 0086 72e8 0100 0058 0700 0000  j.....r....X....
+000026b0: 6567 352e 706e 6772 e901 0000 6807 5d72  eg5.pngr....h.]r
+000026c0: ea01 0000 683d 6185 5272 eb01 0000 6ae9  ....h=a.Rr....j.
+000026d0: 0100 0086 72ec 0100 0058 1200 0000 6361  ....r....X....ca
+000026e0: 7365 2d6f 7574 6c69 6572 7332 2e70 6e67  se-outliers2.png
+000026f0: 72ed 0100 0068 075d 72ee 0100 0068 4f61  r....h.]r....hOa
+00002700: 8552 72ef 0100 006a ed01 0000 8672 f001  .Rr....j.....r..
+00002710: 0000 5811 0000 0065 672d 6170 7065 6e64  ..X....eg-append
+00002720: 6978 3161 2e6f 7574 72f1 0100 0068 075d  ix1a.outr....h.]
+00002730: 72f2 0100 0068 4661 8552 72f3 0100 006a  r....hFa.Rr....j
+00002740: f101 0000 8672 f401 0000 7568 075d 72f5  .....r....uh.]r.
+00002750: 0100 0028 6aa9 0100 006a ad01 0000 6ab1  ...(j....j....j.
+00002760: 0100 006a b501 0000 6ab9 0100 006a bd01  ...j....j....j..
+00002770: 0000 6ac1 0100 006a c501 0000 6ac9 0100  ..j....j....j...
+00002780: 006a cd01 0000 6ad1 0100 006a d501 0000  .j....j....j....
+00002790: 6ad9 0100 006a dd01 0000 6ae1 0100 006a  j....j....j....j
+000027a0: e501 0000 6ae9 0100 006a ed01 0000 6af1  ....j....j....j.
+000027b0: 0100 0065 8552 72f6 0100 0062 5511 6e75  ...e.Rr....bU.nu
+000027c0: 6d62 6572 6564 5f74 6f63 7472 6565 7372  mbered_toctreesr
+000027d0: f701 0000 6807 5d85 5272 f801 0000 550a  ....h.].Rr....U.
+000027e0: 666f 756e 645f 646f 6373 72f9 0100 0068  found_docsr....h
+000027f0: 075d 72fa 0100 0028 680c 682b 683d 6822  .]r....(h.h+h=h"
+00002800: 684f 6858 6868 6846 6871 6585 5272 fb01  hOhXhhhFhqe.Rr..
+00002810: 0000 550a 6c6f 6e67 7469 746c 6573 72fc  ..U.longtitlesr.
+00002820: 0100 007d 72fd 0100 0028 680c 680e 6822  ...}r....(h.h.h"
+00002830: 6823 682b 682c 683d 683e 6846 6847 684f  h#h+h,h=h>hFhGhO
+00002840: 6850 6858 6859 6868 6869 6871 6872 7555  hPhXhYhhhihqhruU
+00002850: 0c64 6570 656e 6465 6e63 6965 7372 fe01  .dependenciesr..
+00002860: 0000 6a98 0100 0068 0785 5272 ff01 0000  ..j....h..Rr....
+00002870: 2868 2268 075d 7200 0200 0028 6ab5 0100  (h"h.]r....(j...
+00002880: 006a bd01 0000 5808 0000 0065 6733 632e  .j....X....eg3c.
+00002890: 6f75 7472 0102 0000 580c 0000 0065 6736  outr....X....eg6
+000028a0: 2d68 6973 742e 6f75 7472 0202 0000 6add  -hist.outr....j.
+000028b0: 0100 0058 0800 0000 6567 3364 2e6f 7574  ...X....eg3d.out
+000028c0: 7203 0200 0058 0800 0000 6567 3366 2e6f  r....X....eg3f.o
+000028d0: 7574 7204 0200 0058 0800 0000 6567 3365  utr....X....eg3e
+000028e0: 2e6f 7574 7205 0200 0065 8552 7206 0200  .outr....e.Rr...
+000028f0: 0068 2b68 075d 7207 0200 0028 5846 0000  .h+h.]r....(XF..
+00002900: 002e 2e2f 2e2e 2f2e 2e2f 2e2e 2f2e 2e2f  .../../../../../
+00002910: 616e 6163 6f6e 6461 322f 6c69 622f 7079  anaconda2/lib/py
+00002920: 7468 6f6e 322e 372f 7369 7465 2d70 6163  thon2.7/site-pac
+00002930: 6b61 6765 732f 6776 6172 2f5f 5f69 6e69  kages/gvar/__ini
+00002940: 745f 5f2e 7079 6372 0802 0000 5847 0000  t__.pycr....XG..
+00002950: 002e 2e2f 2e2e 2f2e 2e2f 2e2e 2f2e 2e2f  .../../../../../
+00002960: 616e 6163 6f6e 6461 322f 6c69 622f 7079  anaconda2/lib/py
+00002970: 7468 6f6e 322e 372f 7369 7465 2d70 6163  thon2.7/site-pac
+00002980: 6b61 6765 732f 6c73 7166 6974 2f5f 5f69  kages/lsqfit/__i
+00002990: 6e69 745f 5f2e 7079 7209 0200 0058 4600  nit__.pyr....XF.
+000029a0: 0000 2e2e 2f2e 2e2f 2e2e 2f2e 2e2f 2e2e  ..../../../../..
+000029b0: 2f61 6e61 636f 6e64 6132 2f6c 6962 2f70  /anaconda2/lib/p
+000029c0: 7974 686f 6e32 2e37 2f73 6974 652d 7061  ython2.7/site-pa
+000029d0: 636b 6167 6573 2f6c 7371 6669 742f 5f65  ckages/lsqfit/_e
+000029e0: 7874 7261 732e 7079 720a 0200 0058 4500  xtras.pyr....XE.
+000029f0: 0000 2e2e 2f2e 2e2f 2e2e 2f2e 2e2f 2e2e  ..../../../../..
+00002a00: 2f61 6e61 636f 6e64 6132 2f6c 6962 2f70  /anaconda2/lib/p
+00002a10: 7974 686f 6e32 2e37 2f73 6974 652d 7061  ython2.7/site-pa
+00002a20: 636b 6167 6573 2f67 7661 722f 5f5f 696e  ckages/gvar/__in
+00002a30: 6974 5f5f 2e70 7972 0b02 0000 5848 0000  it__.pyr....XH..
+00002a40: 002e 2e2f 2e2e 2f2e 2e2f 2e2e 2f2e 2e2f  .../../../../../
+00002a50: 616e 6163 6f6e 6461 322f 6c69 622f 7079  anaconda2/lib/py
+00002a60: 7468 6f6e 322e 372f 7369 7465 2d70 6163  thon2.7/site-pac
+00002a70: 6b61 6765 732f 6c73 7166 6974 2f5f 5f69  kages/lsqfit/__i
+00002a80: 6e69 745f 5f2e 7079 6372 0c02 0000 6585  nit__.pycr....e.
+00002a90: 5272 0d02 0000 683d 6807 5d72 0e02 0000  Rr....h=h.]r....
+00002aa0: 2858 0d00 0000 6567 362d 6c6f 675f 612e  (X....eg6-log_a.
+00002ab0: 6f75 7472 0f02 0000 5808 0000 0065 6734  outr....X....eg4
+00002ac0: 622e 6f75 7472 1002 0000 5808 0000 0065  b.outr....X....e
+00002ad0: 6731 622e 6f75 7472 1102 0000 6ae9 0100  g1b.outr....j...
+00002ae0: 0058 0700 0000 6567 302e 6f75 7472 1202  .X....eg0.outr..
+00002af0: 0000 5809 0000 0065 6736 2d61 2e6f 7574  ..X....eg6-a.out
+00002b00: 7213 0200 0058 0800 0000 6567 3762 2e6f  r....X....eg7b.o
+00002b10: 7574 7214 0200 006a c501 0000 5807 0000  utr....j....X...
+00002b20: 0065 6732 2e6f 7574 7215 0200 0058 0800  .eg2.outr....X..
+00002b30: 0000 6567 3961 2e6f 7574 7216 0200 0058  ..eg9a.outr....X
+00002b40: 0800 0000 6567 3362 2e6f 7574 7217 0200  ....eg3b.outr...
+00002b50: 0058 0800 0000 6567 3761 2e6f 7574 7218  .X....eg7a.outr.
+00002b60: 0200 0058 0800 0000 6567 3562 2e6f 7574  ...X....eg5b.out
+00002b70: 7219 0200 0058 0800 0000 6567 3561 2e6f  r....X....eg5a.o
+00002b80: 7574 721a 0200 006a c901 0000 5808 0000  utr....j....X...
+00002b90: 0065 6733 612e 6f75 7472 1b02 0000 5808  .eg3a.outr....X.
+00002ba0: 0000 0065 6731 612e 6f75 7472 1c02 0000  ...eg1a.outr....
+00002bb0: 580e 0000 0065 6736 2d65 7266 696e 762e  X....eg6-erfinv.
+00002bc0: 6f75 7472 1d02 0000 6ac1 0100 0058 0800  outr....j....X..
+00002bd0: 0000 6567 3461 2e6f 7574 721e 0200 0058  ..eg4a.outr....X
+00002be0: 0700 0000 6567 312e 6f75 7472 1f02 0000  ....eg1.outr....
+00002bf0: 6585 5272 2002 0000 6846 6807 5d72 2102  e.Rr ...hFh.]r!.
+00002c00: 0000 286a a901 0000 6aad 0100 006a b101  ..(j....j....j..
+00002c10: 0000 5811 0000 0065 672d 6170 7065 6e64  ..X....eg-append
+00002c20: 6978 3167 2e6f 7574 7222 0200 006a b901  ix1g.outr"...j..
+00002c30: 0000 5811 0000 0065 672d 6170 7065 6e64  ..X....eg-append
+00002c40: 6978 3164 2e6f 7574 7223 0200 0058 1100  ix1d.outr#...X..
+00002c50: 0000 6567 2d61 7070 656e 6469 7831 622e  ..eg-appendix1b.
+00002c60: 6f75 7472 2402 0000 5811 0000 0065 672d  outr$...X....eg-
+00002c70: 6170 7065 6e64 6978 3163 2e6f 7574 7225  appendix1c.outr%
+00002c80: 0200 0058 1100 0000 6567 2d61 7070 656e  ...X....eg-appen
+00002c90: 6469 7831 652e 6f75 7472 2602 0000 5811  dix1e.outr&...X.
+00002ca0: 0000 0065 672d 6170 7065 6e64 6978 3161  ...eg-appendix1a
+00002cb0: 2e6f 7574 7227 0200 0065 8552 7228 0200  .outr'...e.Rr(..
+00002cc0: 0068 4f68 075d 7229 0200 0028 6acd 0100  .hOh.]r)...(j...
+00002cd0: 0058 1500 0000 6361 7365 2d6f 7574 6c69  .X....case-outli
+00002ce0: 6572 732d 6c73 712e 6f75 7472 2a02 0000  ers-lsq.outr*...
+00002cf0: 5817 0000 0063 6173 652d 6f75 746c 6965  X....case-outlie
+00002d00: 7273 2d6d 756c 7469 2e6f 7574 722b 0200  rs-multi.outr+..
+00002d10: 0058 1100 0000 6361 7365 2d6f 7574 6c69  .X....case-outli
+00002d20: 6572 732e 6f75 7472 2c02 0000 6aed 0100  ers.outr,...j...
+00002d30: 0065 8552 722d 0200 0068 5868 075d 722e  .e.Rr-...hXh.]r.
+00002d40: 0200 0058 4500 0000 2e2e 2f2e 2e2f 2e2e  ...XE...../../..
+00002d50: 2f2e 2e2f 2e2e 2f61 6e61 636f 6e64 6132  /../../anaconda2
+00002d60: 2f6c 6962 2f70 7974 686f 6e32 2e37 2f73  /lib/python2.7/s
+00002d70: 6974 652d 7061 636b 6167 6573 2f6c 7371  ite-packages/lsq
+00002d80: 6669 742f 5f73 6369 7079 2e70 7972 2f02  fit/_scipy.pyr/.
+00002d90: 0000 6185 5272 3002 0000 6868 6807 5d72  ..a.Rr0...hhh.]r
+00002da0: 3102 0000 2858 1100 0000 6361 7365 2d70  1...(X....case-p
+00002db0: 656e 6475 6c75 6d2e 6f75 7472 3202 0000  endulum.outr2...
+00002dc0: 6ad5 0100 006a d101 0000 6585 5272 3302  j....j....e.Rr3.
+00002dd0: 0000 7555 1074 6f63 7472 6565 5f69 6e63  ..uU.toctree_inc
+00002de0: 6c75 6465 7372 3402 0000 7d72 3502 0000  ludesr4...}r5...
+00002df0: 680c 5d72 3602 0000 2858 0800 0000 6f76  h.]r6...(X....ov
+00002e00: 6572 7669 6577 7237 0200 0058 0700 0000  erviewr7...X....
+00002e10: 7465 7374 696e 6772 3802 0000 5812 0000  testingr8...X...
+00002e20: 0063 6173 652d 6578 7472 6170 6f6c 6174  .case-extrapolat
+00002e30: 696f 6e72 3902 0000 580d 0000 0063 6173  ionr9...X....cas
+00002e40: 652d 7065 6e64 756c 756d 723a 0200 0058  e-pendulumr:...X
+00002e50: 0d00 0000 6361 7365 2d6f 7574 6c69 6572  ....case-outlier
+00002e60: 7372 3b02 0000 5806 0000 006c 7371 6669  sr;...X....lsqfi
+00002e70: 7472 3c02 0000 5803 0000 0067 736c 723d  tr<...X....gslr=
+00002e80: 0200 0058 0500 0000 7363 6970 7972 3e02  ...X....scipyr>.
+00002e90: 0000 6573 5508 696e 636c 7564 6564 723f  ..esU.includedr?
+00002ea0: 0200 0068 075d 8552 7240 0200 0055 0474  ...h.].Rr@...U.t
+00002eb0: 6f63 7372 4102 0000 7d72 4202 0000 2868  ocsrA...}rB...(h
+00002ec0: 0c63 646f 6375 7469 6c73 2e6e 6f64 6573  .cdocutils.nodes
+00002ed0: 0a62 756c 6c65 745f 6c69 7374 0a72 4302  .bullet_list.rC.
+00002ee0: 0000 2981 7244 0200 007d 7245 0200 0028  ..).rD...}rE...(
+00002ef0: 6810 5500 6811 7d72 4602 0000 2868 135d  h.U.h.}rF...(h.]
+00002f00: 6814 5d68 155d 6816 5d68 175d 7568 185d  h.]h.]h.]h.]uh.]
+00002f10: 7247 0200 0028 6364 6f63 7574 696c 732e  rG...(cdocutils.
+00002f20: 6e6f 6465 730a 6c69 7374 5f69 7465 6d0a  nodes.list_item.
+00002f30: 7248 0200 0029 8172 4902 0000 7d72 4a02  rH...).rI...}rJ.
+00002f40: 0000 2868 1055 0068 117d 724b 0200 0028  ..(h.U.h.}rK...(
+00002f50: 6813 5d68 145d 6815 5d68 165d 6817 5d75  h.]h.]h.]h.]h.]u
+00002f60: 681f 6a44 0200 0068 185d 724c 0200 0028  h.jD...h.]rL...(
+00002f70: 6373 7068 696e 782e 6164 646e 6f64 6573  csphinx.addnodes
+00002f80: 0a63 6f6d 7061 6374 5f70 6172 6167 7261  .compact_paragra
+00002f90: 7068 0a72 4d02 0000 2981 724e 0200 007d  ph.rM...).rN...}
+00002fa0: 724f 0200 0028 6810 5500 6811 7d72 5002  rO...(h.U.h.}rP.
+00002fb0: 0000 2868 135d 6814 5d68 155d 6816 5d68  ..(h.]h.]h.]h.]h
+00002fc0: 175d 7568 1f6a 4902 0000 6818 5d72 5102  .]uh.jI...h.]rQ.
+00002fd0: 0000 6364 6f63 7574 696c 732e 6e6f 6465  ..cdocutils.node
+00002fe0: 730a 7265 6665 7265 6e63 650a 7252 0200  s.reference.rR..
+00002ff0: 0029 8172 5302 0000 7d72 5402 0000 2868  .).rS...}rT...(h
+00003000: 1055 0068 117d 7255 0200 0028 550a 616e  .U.h.}rU...(U.an
+00003010: 6368 6f72 6e61 6d65 5500 5506 7265 6675  chornameU.U.refu
+00003020: 7269 680c 6816 5d68 155d 6813 5d68 145d  rih.h.]h.]h.]h.]
+00003030: 6817 5d55 0869 6e74 6572 6e61 6c88 7568  h.]U.internal.uh
+00003040: 1f6a 4e02 0000 6818 5d72 5602 0000 681a  .jN...h.]rV...h.
+00003050: 5814 0000 006c 7371 6669 7420 446f 6375  X....lsqfit Docu
+00003060: 6d65 6e74 6174 696f 6e72 5702 0000 8581  mentationrW.....
+00003070: 7258 0200 007d 7259 0200 0028 6810 681e  rX...}rY...(h.h.
+00003080: 681f 6a53 0200 0075 6261 6820 5509 7265  h.jS...ubah U.re
+00003090: 6665 7265 6e63 6572 5a02 0000 7562 6168  ferencerZ...ubah
+000030a0: 2055 1163 6f6d 7061 6374 5f70 6172 6167   U.compact_parag
+000030b0: 7261 7068 725b 0200 0075 626a 4302 0000  raphr[...ubjC...
+000030c0: 2981 725c 0200 007d 725d 0200 0028 6810  ).r\...}r]...(h.
+000030d0: 5500 6811 7d72 5e02 0000 2868 135d 6814  U.h.}r^...(h.]h.
+000030e0: 5d68 155d 6816 5d68 175d 7568 1f6a 4902  ]h.]h.]h.]uh.jI.
+000030f0: 0000 6818 5d72 5f02 0000 6373 7068 696e  ..h.]r_...csphin
+00003100: 782e 6164 646e 6f64 6573 0a74 6f63 7472  x.addnodes.toctr
+00003110: 6565 0a72 6002 0000 2981 7261 0200 007d  ee.r`...).ra...}
+00003120: 7262 0200 0028 6810 5500 681f 6a5c 0200  rb...(h.U.h.j\..
+00003130: 0055 0673 6f75 7263 6572 6302 0000 5836  .U.sourcerc...X6
+00003140: 0000 002f 5573 6572 732f 6770 6c2f 736f  .../Users/gpl/so
+00003150: 6674 7761 7265 2f70 7974 686f 6e2f 6c73  ftware/python/ls
+00003160: 7166 6974 2f64 6f63 2f73 6f75 7263 652f  qfit/doc/source/
+00003170: 696e 6465 782e 7273 7468 2055 0774 6f63  index.rsth U.toc
+00003180: 7472 6565 7264 0200 0068 117d 7265 0200  treerd...h.}re..
+00003190: 0028 5508 6e75 6d62 6572 6564 4b00 5506  .(U.numberedK.U.
+000031a0: 7061 7265 6e74 680c 550a 7469 746c 6573  parenth.U.titles
+000031b0: 6f6e 6c79 8955 086d 6178 6465 7074 684b  only.U.maxdepthK
+000031c0: 0255 0467 6c6f 6289 6816 5d68 155d 6813  .U.glob.h.]h.]h.
+000031d0: 5d68 145d 6817 5d55 0765 6e74 7269 6573  ]h.]h.]U.entries
+000031e0: 5d72 6602 0000 284e 6a37 0200 0086 7267  ]rf...(Nj7....rg
+000031f0: 0200 004e 6a38 0200 0086 7268 0200 004e  ...Nj8....rh...N
+00003200: 6a39 0200 0086 7269 0200 004e 6a3a 0200  j9....ri...Nj:..
+00003210: 0086 726a 0200 004e 6a3b 0200 0086 726b  ..rj...Nj;....rk
+00003220: 0200 004e 6a3c 0200 0086 726c 0200 004e  ...Nj<....rl...N
+00003230: 6a3d 0200 0086 726d 0200 004e 6a3e 0200  j=....rm...Nj>..
+00003240: 0086 726e 0200 0065 5506 6869 6464 656e  ..rn...eU.hidden
+00003250: 8955 0763 6170 7469 6f6e 4e55 0c69 6e63  .U.captionNU.inc
+00003260: 6c75 6465 6669 6c65 735d 726f 0200 0028  ludefiles]ro...(
+00003270: 6a37 0200 006a 3802 0000 6a39 0200 006a  j7...j8...j9...j
+00003280: 3a02 0000 6a3b 0200 006a 3c02 0000 6a3d  :...j;...j<...j=
+00003290: 0200 006a 3e02 0000 6555 0d69 6e63 6c75  ...j>...eU.inclu
+000032a0: 6465 6869 6464 656e 8975 5504 6c69 6e65  dehidden.uU.line
+000032b0: 7270 0200 004b 0b68 185d 7562 6168 2055  rp...K.h.]ubah U
+000032c0: 0b62 756c 6c65 745f 6c69 7374 7271 0200  .bullet_listrq..
+000032d0: 0075 6265 6820 5509 6c69 7374 5f69 7465  .ubeh U.list_ite
+000032e0: 6d72 7202 0000 7562 6a48 0200 0029 8172  mrr...ubjH...).r
+000032f0: 7302 0000 7d72 7402 0000 2868 1055 0068  s...}rt...(h.U.h
+00003300: 117d 7275 0200 0028 6813 5d68 145d 6815  .}ru...(h.]h.]h.
+00003310: 5d68 165d 6817 5d75 681f 6a44 0200 0068  ]h.]h.]uh.jD...h
+00003320: 185d 7276 0200 006a 4d02 0000 2981 7277  .]rv...jM...).rw
+00003330: 0200 007d 7278 0200 0028 6810 5500 6811  ...}rx...(h.U.h.
+00003340: 7d72 7902 0000 2868 135d 6814 5d68 155d  }ry...(h.]h.]h.]
+00003350: 6816 5d68 175d 7568 1f6a 7302 0000 6818  h.]h.]uh.js...h.
+00003360: 5d72 7a02 0000 6a52 0200 0029 8172 7b02  ]rz...jR...).r{.
+00003370: 0000 7d72 7c02 0000 2868 1055 0068 117d  ..}r|...(h.U.h.}
+00003380: 727d 0200 0028 550a 616e 6368 6f72 6e61  r}...(U.anchorna
+00003390: 6d65 5513 2369 6e64 6963 6573 2d61 6e64  meU.#indices-and
+000033a0: 2d74 6162 6c65 7355 0672 6566 7572 6968  -tablesU.refurih
+000033b0: 0c68 165d 6815 5d68 135d 6814 5d68 175d  .h.]h.]h.]h.]h.]
+000033c0: 5508 696e 7465 726e 616c 8875 681f 6a77  U.internal.uh.jw
+000033d0: 0200 0068 185d 727e 0200 0068 1a58 1200  ...h.]r~...h.X..
+000033e0: 0000 496e 6469 6365 7320 616e 6420 7461  ..Indices and ta
+000033f0: 626c 6573 727f 0200 0085 8172 8002 0000  blesr......r....
+00003400: 7d72 8102 0000 2868 1058 1200 0000 496e  }r....(h.X....In
+00003410: 6469 6365 7320 616e 6420 7461 626c 6573  dices and tables
+00003420: 681f 6a7b 0200 0075 6261 6820 6a5a 0200  h.j{...ubah jZ..
+00003430: 0075 6261 6820 6a5b 0200 0075 6261 6820  .ubah j[...ubah 
+00003440: 6a72 0200 0075 6265 6820 6a71 0200 0075  jr...ubeh jq...u
+00003450: 6268 226a 4302 0000 2981 7282 0200 007d  bh"jC...).r....}
+00003460: 7283 0200 0028 6810 5500 6811 7d72 8402  r....(h.U.h.}r..
+00003470: 0000 2868 135d 6814 5d68 155d 6816 5d68  ..(h.]h.]h.]h.]h
+00003480: 175d 7568 185d 7285 0200 006a 4802 0000  .]uh.]r....jH...
+00003490: 2981 7286 0200 007d 7287 0200 0028 6810  ).r....}r....(h.
+000034a0: 5500 6811 7d72 8802 0000 2868 135d 6814  U.h.}r....(h.]h.
+000034b0: 5d68 155d 6816 5d68 175d 7568 1f6a 8202  ]h.]h.]h.]uh.j..
+000034c0: 0000 6818 5d72 8902 0000 286a 4d02 0000  ..h.]r....(jM...
+000034d0: 2981 728a 0200 007d 728b 0200 0028 6810  ).r....}r....(h.
+000034e0: 5500 6811 7d72 8c02 0000 2868 135d 6814  U.h.}r....(h.]h.
+000034f0: 5d68 155d 6816 5d68 175d 7568 1f6a 8602  ]h.]h.]h.]uh.j..
+00003500: 0000 6818 5d72 8d02 0000 6a52 0200 0029  ..h.]r....jR...)
+00003510: 8172 8e02 0000 7d72 8f02 0000 2868 1055  .r....}r....(h.U
+00003520: 0068 117d 7290 0200 0028 550a 616e 6368  .h.}r....(U.anch
+00003530: 6f72 6e61 6d65 5500 5506 7265 6675 7269  ornameU.U.refuri
+00003540: 6822 6816 5d68 155d 6813 5d68 145d 6817  h"h.]h.]h.]h.]h.
+00003550: 5d55 0869 6e74 6572 6e61 6c88 7568 1f6a  ]U.internal.uh.j
+00003560: 8a02 0000 6818 5d72 9102 0000 681a 5823  ....h.]r....h.X#
+00003570: 0000 004e 6f6e 2d47 6175 7373 6961 6e20  ...Non-Gaussian 
+00003580: 4265 6861 7669 6f72 3b20 5465 7374 696e  Behavior; Testin
+00003590: 6720 4669 7473 7292 0200 0085 8172 9302  g Fitsr......r..
+000035a0: 0000 7d72 9402 0000 2868 1068 2a68 1f6a  ..}r....(h.h*h.j
+000035b0: 8e02 0000 7562 6168 206a 5a02 0000 7562  ....ubah jZ...ub
+000035c0: 6168 206a 5b02 0000 7562 6a43 0200 0029  ah j[...ubjC...)
+000035d0: 8172 9502 0000 7d72 9602 0000 2868 1055  .r....}r....(h.U
+000035e0: 0068 117d 7297 0200 0028 6813 5d68 145d  .h.}r....(h.]h.]
+000035f0: 6815 5d68 165d 6817 5d75 681f 6a86 0200  h.]h.]h.]uh.j...
+00003600: 0068 185d 7298 0200 0028 6a48 0200 0029  .h.]r....(jH...)
+00003610: 8172 9902 0000 7d72 9a02 0000 2868 1055  .r....}r....(h.U
+00003620: 0068 117d 729b 0200 0028 6813 5d68 145d  .h.}r....(h.]h.]
+00003630: 6815 5d68 165d 6817 5d75 681f 6a95 0200  h.]h.]h.]uh.j...
+00003640: 0068 185d 729c 0200 006a 4d02 0000 2981  .h.]r....jM...).
+00003650: 729d 0200 007d 729e 0200 0028 6810 5500  r....}r....(h.U.
+00003660: 6811 7d72 9f02 0000 2868 135d 6814 5d68  h.}r....(h.]h.]h
+00003670: 155d 6816 5d68 175d 7568 1f6a 9902 0000  .]h.]h.]uh.j....
+00003680: 6818 5d72 a002 0000 6a52 0200 0029 8172  h.]r....jR...).r
+00003690: a102 0000 7d72 a202 0000 2868 1055 0068  ....}r....(h.U.h
+000036a0: 117d 72a3 0200 0028 550a 616e 6368 6f72  .}r....(U.anchor
+000036b0: 6e61 6d65 550d 2369 6e74 726f 6475 6374  nameU.#introduct
+000036c0: 696f 6e55 0672 6566 7572 6968 2268 165d  ionU.refurih"h.]
+000036d0: 6815 5d68 135d 6814 5d68 175d 5508 696e  h.]h.]h.]h.]U.in
+000036e0: 7465 726e 616c 8875 681f 6a9d 0200 0068  ternal.uh.j....h
+000036f0: 185d 72a4 0200 0068 1a58 0c00 0000 496e  .]r....h.X....In
+00003700: 7472 6f64 7563 7469 6f6e 72a5 0200 0085  troductionr.....
+00003710: 8172 a602 0000 7d72 a702 0000 2868 1058  .r....}r....(h.X
+00003720: 0c00 0000 496e 7472 6f64 7563 7469 6f6e  ....Introduction
+00003730: 72a8 0200 0068 1f6a a102 0000 7562 6168  r....h.j....ubah
+00003740: 206a 5a02 0000 7562 6168 206a 5b02 0000   jZ...ubah j[...
+00003750: 7562 6168 206a 7202 0000 7562 6a48 0200  ubah jr...ubjH..
+00003760: 0029 8172 a902 0000 7d72 aa02 0000 2868  .).r....}r....(h
+00003770: 1055 0068 117d 72ab 0200 0028 6813 5d68  .U.h.}r....(h.]h
+00003780: 145d 6815 5d68 165d 6817 5d75 681f 6a95  .]h.]h.]h.]uh.j.
+00003790: 0200 0068 185d 72ac 0200 006a 4d02 0000  ...h.]r....jM...
+000037a0: 2981 72ad 0200 007d 72ae 0200 0028 6810  ).r....}r....(h.
+000037b0: 5500 6811 7d72 af02 0000 2868 135d 6814  U.h.}r....(h.]h.
+000037c0: 5d68 155d 6816 5d68 175d 7568 1f6a a902  ]h.]h.]h.]uh.j..
+000037d0: 0000 6818 5d72 b002 0000 6a52 0200 0029  ..h.]r....jR...)
+000037e0: 8172 b102 0000 7d72 b202 0000 2868 1055  .r....}r....(h.U
+000037f0: 0068 117d 72b3 0200 0028 550a 616e 6368  .h.}r....(U.anch
+00003800: 6f72 6e61 6d65 552d 2362 6f6f 7473 7472  ornameU-#bootstr
+00003810: 6170 2d65 7272 6f72 2d61 6e61 6c79 7369  ap-error-analysi
+00003820: 732d 6e6f 6e2d 6761 7573 7369 616e 2d6f  s-non-gaussian-o
+00003830: 7574 7075 7455 0672 6566 7572 6968 2268  utputU.refurih"h
+00003840: 165d 6815 5d68 135d 6814 5d68 175d 5508  .]h.]h.]h.]h.]U.
+00003850: 696e 7465 726e 616c 8875 681f 6aad 0200  internal.uh.j...
+00003860: 0068 185d 72b4 0200 0068 1a58 2d00 0000  .h.]r....h.X-...
+00003870: 426f 6f74 7374 7261 7020 4572 726f 7220  Bootstrap Error 
+00003880: 416e 616c 7973 6973 3b20 4e6f 6e2d 4761  Analysis; Non-Ga
+00003890: 7573 7369 616e 204f 7574 7075 7472 b502  ussian Outputr..
+000038a0: 0000 8581 72b6 0200 007d 72b7 0200 0028  ....r....}r....(
+000038b0: 6810 582d 0000 0042 6f6f 7473 7472 6170  h.X-...Bootstrap
+000038c0: 2045 7272 6f72 2041 6e61 6c79 7369 733b   Error Analysis;
+000038d0: 204e 6f6e 2d47 6175 7373 6961 6e20 4f75   Non-Gaussian Ou
+000038e0: 7470 7574 72b8 0200 0068 1f6a b102 0000  tputr....h.j....
+000038f0: 7562 6168 206a 5a02 0000 7562 6168 206a  ubah jZ...ubah j
+00003900: 5b02 0000 7562 6168 206a 7202 0000 7562  [...ubah jr...ub
+00003910: 6a48 0200 0029 8172 b902 0000 7d72 ba02  jH...).r....}r..
+00003920: 0000 2868 1055 0068 117d 72bb 0200 0028  ..(h.U.h.}r....(
+00003930: 6813 5d68 145d 6815 5d68 165d 6817 5d75  h.]h.]h.]h.]h.]u
+00003940: 681f 6a95 0200 0068 185d 72bc 0200 006a  h.j....h.]r....j
+00003950: 4d02 0000 2981 72bd 0200 007d 72be 0200  M...).r....}r...
+00003960: 0028 6810 5500 6811 7d72 bf02 0000 2868  .(h.U.h.}r....(h
+00003970: 135d 6814 5d68 155d 6816 5d68 175d 7568  .]h.]h.]h.]h.]uh
+00003980: 1f6a b902 0000 6818 5d72 c002 0000 6a52  .j....h.]r....jR
+00003990: 0200 0029 8172 c102 0000 7d72 c202 0000  ...).r....}r....
+000039a0: 2868 1055 0068 117d 72c3 0200 0028 550a  (h.U.h.}r....(U.
+000039b0: 616e 6368 6f72 6e61 6d65 5513 2362 6179  anchornameU.#bay
+000039c0: 6573 6961 6e2d 696e 7465 6772 616c 7355  esian-integralsU
+000039d0: 0672 6566 7572 6968 2268 165d 6815 5d68  .refurih"h.]h.]h
+000039e0: 135d 6814 5d68 175d 5508 696e 7465 726e  .]h.]h.]U.intern
+000039f0: 616c 8875 681f 6abd 0200 0068 185d 72c4  al.uh.j....h.]r.
+00003a00: 0200 0068 1a58 1200 0000 4261 7965 7369  ...h.X....Bayesi
+00003a10: 616e 2049 6e74 6567 7261 6c73 72c5 0200  an Integralsr...
+00003a20: 0085 8172 c602 0000 7d72 c702 0000 2868  ...r....}r....(h
+00003a30: 1058 1200 0000 4261 7965 7369 616e 2049  .X....Bayesian I
+00003a40: 6e74 6567 7261 6c73 72c8 0200 0068 1f6a  ntegralsr....h.j
+00003a50: c102 0000 7562 6168 206a 5a02 0000 7562  ....ubah jZ...ub
+00003a60: 6168 206a 5b02 0000 7562 6168 206a 7202  ah j[...ubah jr.
+00003a70: 0000 7562 6a48 0200 0029 8172 c902 0000  ..ubjH...).r....
+00003a80: 7d72 ca02 0000 2868 1055 0068 117d 72cb  }r....(h.U.h.}r.
+00003a90: 0200 0028 6813 5d68 145d 6815 5d68 165d  ...(h.]h.]h.]h.]
+00003aa0: 6817 5d75 681f 6a95 0200 0068 185d 72cc  h.]uh.j....h.]r.
+00003ab0: 0200 006a 4d02 0000 2981 72cd 0200 007d  ...jM...).r....}
+00003ac0: 72ce 0200 0028 6810 5500 6811 7d72 cf02  r....(h.U.h.}r..
+00003ad0: 0000 2868 135d 6814 5d68 155d 6816 5d68  ..(h.]h.]h.]h.]h
+00003ae0: 175d 7568 1f6a c902 0000 6818 5d72 d002  .]uh.j....h.]r..
+00003af0: 0000 6a52 0200 0029 8172 d102 0000 7d72  ..jR...).r....}r
+00003b00: d202 0000 2868 1055 0068 117d 72d3 0200  ....(h.U.h.}r...
+00003b10: 0028 550a 616e 6368 6f72 6e61 6d65 5521  .(U.anchornameU!
+00003b20: 2374 6573 7469 6e67 2d66 6974 732d 7769  #testing-fits-wi
+00003b30: 7468 2d73 696d 756c 6174 6564 2d64 6174  th-simulated-dat
+00003b40: 6155 0672 6566 7572 6968 2268 165d 6815  aU.refurih"h.]h.
+00003b50: 5d68 135d 6814 5d68 175d 5508 696e 7465  ]h.]h.]h.]U.inte
+00003b60: 726e 616c 8875 681f 6acd 0200 0068 185d  rnal.uh.j....h.]
+00003b70: 72d4 0200 0068 1a58 2000 0000 5465 7374  r....h.X ...Test
+00003b80: 696e 6720 4669 7473 2077 6974 6820 5369  ing Fits with Si
+00003b90: 6d75 6c61 7465 6420 4461 7461 72d5 0200  mulated Datar...
+00003ba0: 0085 8172 d602 0000 7d72 d702 0000 2868  ...r....}r....(h
+00003bb0: 1058 2000 0000 5465 7374 696e 6720 4669  .X ...Testing Fi
+00003bc0: 7473 2077 6974 6820 5369 6d75 6c61 7465  ts with Simulate
+00003bd0: 6420 4461 7461 72d8 0200 0068 1f6a d102  d Datar....h.j..
+00003be0: 0000 7562 6168 206a 5a02 0000 7562 6168  ..ubah jZ...ubah
+00003bf0: 206a 5b02 0000 7562 6168 206a 7202 0000   j[...ubah jr...
+00003c00: 7562 6568 206a 7102 0000 7562 6568 206a  ubeh jq...ubeh j
+00003c10: 7202 0000 7562 6168 206a 7102 0000 7562  r...ubah jq...ub
+00003c20: 682b 6a43 0200 0029 8172 d902 0000 7d72  h+jC...).r....}r
+00003c30: da02 0000 2868 1055 0068 117d 72db 0200  ....(h.U.h.}r...
+00003c40: 0028 6813 5d68 145d 6815 5d68 165d 6817  .(h.]h.]h.]h.]h.
+00003c50: 5d75 6818 5d72 dc02 0000 6a48 0200 0029  ]uh.]r....jH...)
+00003c60: 8172 dd02 0000 7d72 de02 0000 2868 1055  .r....}r....(h.U
+00003c70: 0068 117d 72df 0200 0028 6813 5d68 145d  .h.}r....(h.]h.]
+00003c80: 6815 5d68 165d 6817 5d75 681f 6ad9 0200  h.]h.]h.]uh.j...
+00003c90: 0068 185d 72e0 0200 0028 6a4d 0200 0029  .h.]r....(jM...)
+00003ca0: 8172 e102 0000 7d72 e202 0000 2868 1055  .r....}r....(h.U
+00003cb0: 0068 117d 72e3 0200 0028 6813 5d68 145d  .h.}r....(h.]h.]
+00003cc0: 6815 5d68 165d 6817 5d75 681f 6add 0200  h.]h.]h.]uh.j...
+00003cd0: 0068 185d 72e4 0200 006a 5202 0000 2981  .h.]r....jR...).
+00003ce0: 72e5 0200 007d 72e6 0200 0028 6810 5500  r....}r....(h.U.
+00003cf0: 6811 7d72 e702 0000 2855 0a61 6e63 686f  h.}r....(U.ancho
+00003d00: 726e 616d 6555 0055 0672 6566 7572 6968  rnameU.U.refurih
+00003d10: 2b68 165d 6815 5d68 135d 6814 5d68 175d  +h.]h.]h.]h.]h.]
+00003d20: 5508 696e 7465 726e 616c 8875 681f 6ae1  U.internal.uh.j.
+00003d30: 0200 0068 185d 72e8 0200 0028 6830 2981  ...h.]r....(h0).
+00003d40: 72e9 0200 007d 72ea 0200 0028 6810 5806  r....}r....(h.X.
+00003d50: 0000 006c 7371 6669 7468 117d 72eb 0200  ...lsqfith.}r...
+00003d60: 0028 6813 5d68 145d 6815 5d68 165d 6817  .(h.]h.]h.]h.]h.
+00003d70: 5d75 681f 6ae5 0200 0068 185d 72ec 0200  ]uh.j....h.]r...
+00003d80: 0068 1a58 0600 0000 6c73 7166 6974 72ed  .h.X....lsqfitr.
+00003d90: 0200 0085 8172 ee02 0000 7d72 ef02 0000  .....r....}r....
+00003da0: 2868 1055 0068 1f6a e902 0000 7562 6168  (h.U.h.j....ubah
+00003db0: 2068 3875 6268 1a58 2200 0000 202d 204e   h8ubh.X"... - N
+00003dc0: 6f6e 6c69 6e65 6172 204c 6561 7374 2053  onlinear Least S
+00003dd0: 7175 6172 6573 2046 6974 7469 6e67 72f0  quares Fittingr.
+00003de0: 0200 0085 8172 f102 0000 7d72 f202 0000  .....r....}r....
+00003df0: 2868 1068 3c68 1f6a e502 0000 7562 6568  (h.h<h.j....ubeh
+00003e00: 206a 5a02 0000 7562 6168 206a 5b02 0000   jZ...ubah j[...
+00003e10: 7562 6a43 0200 0029 8172 f302 0000 7d72  ubjC...).r....}r
+00003e20: f402 0000 2868 1055 0068 117d 72f5 0200  ....(h.U.h.}r...
+00003e30: 0028 6813 5d68 145d 6815 5d68 165d 6817  .(h.]h.]h.]h.]h.
+00003e40: 5d75 681f 6add 0200 0068 185d 72f6 0200  ]uh.j....h.]r...
+00003e50: 0028 6a48 0200 0029 8172 f702 0000 7d72  .(jH...).r....}r
+00003e60: f802 0000 2868 1055 0068 117d 72f9 0200  ....(h.U.h.}r...
+00003e70: 0028 6813 5d68 145d 6815 5d68 165d 6817  .(h.]h.]h.]h.]h.
+00003e80: 5d75 681f 6af3 0200 0068 185d 72fa 0200  ]uh.j....h.]r...
+00003e90: 006a 4d02 0000 2981 72fb 0200 007d 72fc  .jM...).r....}r.
+00003ea0: 0200 0028 6810 5500 6811 7d72 fd02 0000  ...(h.U.h.}r....
+00003eb0: 2868 135d 6814 5d68 155d 6816 5d68 175d  (h.]h.]h.]h.]h.]
+00003ec0: 7568 1f6a f702 0000 6818 5d72 fe02 0000  uh.j....h.]r....
+00003ed0: 6a52 0200 0029 8172 ff02 0000 7d72 0003  jR...).r....}r..
+00003ee0: 0000 2868 1055 0068 117d 7201 0300 0028  ..(h.U.h.}r....(
+00003ef0: 550a 616e 6368 6f72 6e61 6d65 550d 2369  U.anchornameU.#i
+00003f00: 6e74 726f 6475 6374 696f 6e55 0672 6566  ntroductionU.ref
+00003f10: 7572 6968 2b68 165d 6815 5d68 135d 6814  urih+h.]h.]h.]h.
+00003f20: 5d68 175d 5508 696e 7465 726e 616c 8875  ]h.]U.internal.u
+00003f30: 681f 6afb 0200 0068 185d 7202 0300 0068  h.j....h.]r....h
+00003f40: 1a58 0c00 0000 496e 7472 6f64 7563 7469  .X....Introducti
+00003f50: 6f6e 7203 0300 0085 8172 0403 0000 7d72  onr......r....}r
+00003f60: 0503 0000 2868 1058 0c00 0000 496e 7472  ....(h.X....Intr
+00003f70: 6f64 7563 7469 6f6e 7206 0300 0068 1f6a  oductionr....h.j
+00003f80: ff02 0000 7562 6168 206a 5a02 0000 7562  ....ubah jZ...ub
+00003f90: 6168 206a 5b02 0000 7562 6168 206a 7202  ah j[...ubah jr.
+00003fa0: 0000 7562 6a48 0200 0029 8172 0703 0000  ..ubjH...).r....
+00003fb0: 7d72 0803 0000 2868 1055 0068 117d 7209  }r....(h.U.h.}r.
+00003fc0: 0300 0028 6813 5d68 145d 6815 5d68 165d  ...(h.]h.]h.]h.]
+00003fd0: 6817 5d75 681f 6af3 0200 0068 185d 720a  h.]uh.j....h.]r.
+00003fe0: 0300 006a 4d02 0000 2981 720b 0300 007d  ...jM...).r....}
+00003ff0: 720c 0300 0028 6810 5500 6811 7d72 0d03  r....(h.U.h.}r..
+00004000: 0000 2868 135d 6814 5d68 155d 6816 5d68  ..(h.]h.]h.]h.]h
+00004010: 175d 7568 1f6a 0703 0000 6818 5d72 0e03  .]uh.j....h.]r..
+00004020: 0000 6a52 0200 0029 8172 0f03 0000 7d72  ..jR...).r....}r
+00004030: 1003 0000 2868 1055 0068 117d 7211 0300  ....(h.U.h.}r...
+00004040: 0028 550a 616e 6368 6f72 6e61 6d65 5516  .(U.anchornameU.
+00004050: 236e 6f6e 6c69 6e65 6172 2d66 6974 2d6f  #nonlinear-fit-o
+00004060: 626a 6563 7473 5506 7265 6675 7269 682b  bjectsU.refurih+
+00004070: 6816 5d68 155d 6813 5d68 145d 6817 5d55  h.]h.]h.]h.]h.]U
+00004080: 0869 6e74 6572 6e61 6c88 7568 1f6a 0b03  .internal.uh.j..
+00004090: 0000 6818 5d72 1203 0000 681a 5815 0000  ..h.]r....h.X...
+000040a0: 006e 6f6e 6c69 6e65 6172 5f66 6974 204f  .nonlinear_fit O
+000040b0: 626a 6563 7473 7213 0300 0085 8172 1403  bjectsr......r..
+000040c0: 0000 7d72 1503 0000 2868 1058 1500 0000  ..}r....(h.X....
+000040d0: 6e6f 6e6c 696e 6561 725f 6669 7420 4f62  nonlinear_fit Ob
+000040e0: 6a65 6374 7372 1603 0000 681f 6a0f 0300  jectsr....h.j...
+000040f0: 0075 6261 6820 6a5a 0200 0075 6261 6820  .ubah jZ...ubah 
+00004100: 6a5b 0200 0075 6261 6820 6a72 0200 0075  j[...ubah jr...u
+00004110: 626a 4802 0000 2981 7217 0300 007d 7218  bjH...).r....}r.
+00004120: 0300 0028 6810 5500 6811 7d72 1903 0000  ...(h.U.h.}r....
+00004130: 2868 135d 6814 5d68 155d 6816 5d68 175d  (h.]h.]h.]h.]h.]
+00004140: 7568 1f6a f302 0000 6818 5d72 1a03 0000  uh.j....h.]r....
+00004150: 6a4d 0200 0029 8172 1b03 0000 7d72 1c03  jM...).r....}r..
+00004160: 0000 2868 1055 0068 117d 721d 0300 0028  ..(h.U.h.}r....(
+00004170: 6813 5d68 145d 6815 5d68 165d 6817 5d75  h.]h.]h.]h.]h.]u
+00004180: 681f 6a17 0300 0068 185d 721e 0300 006a  h.j....h.]r....j
+00004190: 5202 0000 2981 721f 0300 007d 7220 0300  R...).r....}r ..
+000041a0: 0028 6810 5500 6811 7d72 2103 0000 2855  .(h.U.h.}r!...(U
+000041b0: 0a61 6e63 686f 726e 616d 6555 0a23 6675  .anchornameU.#fu
+000041c0: 6e63 7469 6f6e 7355 0672 6566 7572 6968  nctionsU.refurih
+000041d0: 2b68 165d 6815 5d68 135d 6814 5d68 175d  +h.]h.]h.]h.]h.]
+000041e0: 5508 696e 7465 726e 616c 8875 681f 6a1b  U.internal.uh.j.
+000041f0: 0300 0068 185d 7222 0300 0068 1a58 0900  ...h.]r"...h.X..
+00004200: 0000 4675 6e63 7469 6f6e 7372 2303 0000  ..Functionsr#...
+00004210: 8581 7224 0300 007d 7225 0300 0028 6810  ..r$...}r%...(h.
+00004220: 5809 0000 0046 756e 6374 696f 6e73 7226  X....Functionsr&
+00004230: 0300 0068 1f6a 1f03 0000 7562 6168 206a  ...h.j....ubah j
+00004240: 5a02 0000 7562 6168 206a 5b02 0000 7562  Z...ubah j[...ub
+00004250: 6168 206a 7202 0000 7562 6a48 0200 0029  ah jr...ubjH...)
+00004260: 8172 2703 0000 7d72 2803 0000 2868 1055  .r'...}r(...(h.U
+00004270: 0068 117d 7229 0300 0028 6813 5d68 145d  .h.}r)...(h.]h.]
+00004280: 6815 5d68 165d 6817 5d75 681f 6af3 0200  h.]h.]h.]uh.j...
+00004290: 0068 185d 722a 0300 006a 4d02 0000 2981  .h.]r*...jM...).
+000042a0: 722b 0300 007d 722c 0300 0028 6810 5500  r+...}r,...(h.U.
+000042b0: 6811 7d72 2d03 0000 2868 135d 6814 5d68  h.}r-...(h.]h.]h
+000042c0: 155d 6816 5d68 175d 7568 1f6a 2703 0000  .]h.]h.]uh.j'...
+000042d0: 6818 5d72 2e03 0000 6a52 0200 0029 8172  h.]r....jR...).r
+000042e0: 2f03 0000 7d72 3003 0000 2868 1055 0068  /...}r0...(h.U.h
+000042f0: 117d 7231 0300 0028 550a 616e 6368 6f72  .}r1...(U.anchor
+00004300: 6e61 6d65 551f 2363 6c61 7373 6573 2d66  nameU.#classes-f
+00004310: 6f72 2d62 6179 6573 6961 6e2d 696e 7465  or-bayesian-inte
+00004320: 6772 616c 7355 0672 6566 7572 6968 2b68  gralsU.refurih+h
+00004330: 165d 6815 5d68 135d 6814 5d68 175d 5508  .]h.]h.]h.]h.]U.
+00004340: 696e 7465 726e 616c 8875 681f 6a2b 0300  internal.uh.j+..
+00004350: 0068 185d 7232 0300 0068 1a58 1e00 0000  .h.]r2...h.X....
+00004360: 436c 6173 7365 7320 666f 7220 4261 7965  Classes for Baye
+00004370: 7369 616e 2049 6e74 6567 7261 6c73 7233  sian Integralsr3
+00004380: 0300 0085 8172 3403 0000 7d72 3503 0000  .....r4...}r5...
+00004390: 2868 1058 1e00 0000 436c 6173 7365 7320  (h.X....Classes 
+000043a0: 666f 7220 4261 7965 7369 616e 2049 6e74  for Bayesian Int
+000043b0: 6567 7261 6c73 7236 0300 0068 1f6a 2f03  egralsr6...h.j/.
+000043c0: 0000 7562 6168 206a 5a02 0000 7562 6168  ..ubah jZ...ubah
+000043d0: 206a 5b02 0000 7562 6168 206a 7202 0000   j[...ubah jr...
+000043e0: 7562 6a48 0200 0029 8172 3703 0000 7d72  ubjH...).r7...}r
+000043f0: 3803 0000 2868 1055 0068 117d 7239 0300  8...(h.U.h.}r9..
+00004400: 0028 6813 5d68 145d 6815 5d68 165d 6817  .(h.]h.]h.]h.]h.
+00004410: 5d75 681f 6af3 0200 0068 185d 723a 0300  ]uh.j....h.]r:..
+00004420: 006a 4d02 0000 2981 723b 0300 007d 723c  .jM...).r;...}r<
+00004430: 0300 0028 6810 5500 6811 7d72 3d03 0000  ...(h.U.h.}r=...
+00004440: 2868 135d 6814 5d68 155d 6816 5d68 175d  (h.]h.]h.]h.]h.]
+00004450: 7568 1f6a 3703 0000 6818 5d72 3e03 0000  uh.j7...h.]r>...
+00004460: 6a52 0200 0029 8172 3f03 0000 7d72 4003  jR...).r?...}r@.
+00004470: 0000 2868 1055 0068 117d 7241 0300 0028  ..(h.U.h.}rA...(
+00004480: 550a 616e 6368 6f72 6e61 6d65 551b 236c  U.anchornameU.#l
+00004490: 7371 6669 742d 6d75 6c74 6966 6974 7465  sqfit-multifitte
+000044a0: 722d 636c 6173 7365 7355 0672 6566 7572  r-classesU.refur
+000044b0: 6968 2b68 165d 6815 5d68 135d 6814 5d68  ih+h.]h.]h.]h.]h
+000044c0: 175d 5508 696e 7465 726e 616c 8875 681f  .]U.internal.uh.
+000044d0: 6a3b 0300 0068 185d 7242 0300 0028 6830  j;...h.]rB...(h0
+000044e0: 2981 7243 0300 007d 7244 0300 0028 6810  ).rC...}rD...(h.
+000044f0: 5812 0000 006c 7371 6669 742e 4d75 6c74  X....lsqfit.Mult
+00004500: 6946 6974 7465 7268 117d 7245 0300 0028  iFitterh.}rE...(
+00004510: 6813 5d68 145d 6815 5d68 165d 6817 5d75  h.]h.]h.]h.]h.]u
+00004520: 681f 6a3f 0300 0068 185d 7246 0300 0068  h.j?...h.]rF...h
+00004530: 1a58 1200 0000 6c73 7166 6974 2e4d 756c  .X....lsqfit.Mul
+00004540: 7469 4669 7474 6572 7247 0300 0085 8172  tiFitterrG.....r
+00004550: 4803 0000 7d72 4903 0000 2868 1055 0068  H...}rI...(h.U.h
+00004560: 1f6a 4303 0000 7562 6168 2068 3875 6268  .jC...ubah h8ubh
+00004570: 1a58 0800 0000 2043 6c61 7373 6573 724a  .X.... ClassesrJ
+00004580: 0300 0085 8172 4b03 0000 7d72 4c03 0000  .....rK...}rL...
+00004590: 2868 1058 0800 0000 2043 6c61 7373 6573  (h.X.... Classes
+000045a0: 724d 0300 0068 1f6a 3f03 0000 7562 6568  rM...h.j?...ubeh
+000045b0: 206a 5a02 0000 7562 6168 206a 5b02 0000   jZ...ubah j[...
+000045c0: 7562 6168 206a 7202 0000 7562 6a48 0200  ubah jr...ubjH..
+000045d0: 0029 8172 4e03 0000 7d72 4f03 0000 2868  .).rN...}rO...(h
+000045e0: 1055 0068 117d 7250 0300 0028 6813 5d68  .U.h.}rP...(h.]h
+000045f0: 145d 6815 5d68 165d 6817 5d75 681f 6af3  .]h.]h.]h.]uh.j.
+00004600: 0200 0068 185d 7251 0300 006a 4d02 0000  ...h.]rQ...jM...
+00004610: 2981 7252 0300 007d 7253 0300 0028 6810  ).rR...}rS...(h.
+00004620: 5500 6811 7d72 5403 0000 2868 135d 6814  U.h.}rT...(h.]h.
+00004630: 5d68 155d 6816 5d68 175d 7568 1f6a 4e03  ]h.]h.]h.]uh.jN.
+00004640: 0000 6818 5d72 5503 0000 6a52 0200 0029  ..h.]rU...jR...)
+00004650: 8172 5603 0000 7d72 5703 0000 2868 1055  .rV...}rW...(h.U
+00004660: 0068 117d 7258 0300 0028 550a 616e 6368  .h.}rX...(U.anch
+00004670: 6f72 6e61 6d65 550d 2372 6571 7569 7265  ornameU.#require
+00004680: 6d65 6e74 7355 0672 6566 7572 6968 2b68  mentsU.refurih+h
+00004690: 165d 6815 5d68 135d 6814 5d68 175d 5508  .]h.]h.]h.]h.]U.
+000046a0: 696e 7465 726e 616c 8875 681f 6a52 0300  internal.uh.jR..
+000046b0: 0068 185d 7259 0300 0068 1a58 0c00 0000  .h.]rY...h.X....
+000046c0: 5265 7175 6972 656d 656e 7473 725a 0300  RequirementsrZ..
+000046d0: 0085 8172 5b03 0000 7d72 5c03 0000 2868  ...r[...}r\...(h
+000046e0: 1058 0c00 0000 5265 7175 6972 656d 656e  .X....Requiremen
+000046f0: 7473 725d 0300 0068 1f6a 5603 0000 7562  tsr]...h.jV...ub
+00004700: 6168 206a 5a02 0000 7562 6168 206a 5b02  ah jZ...ubah j[.
+00004710: 0000 7562 6168 206a 7202 0000 7562 6568  ..ubah jr...ubeh
+00004720: 206a 7102 0000 7562 6568 206a 7202 0000   jq...ubeh jr...
+00004730: 7562 6168 206a 7102 0000 7562 683d 6a43  ubah jq...ubh=jC
+00004740: 0200 0029 8172 5e03 0000 7d72 5f03 0000  ...).r^...}r_...
+00004750: 2868 1055 0068 117d 7260 0300 0028 6813  (h.U.h.}r`...(h.
+00004760: 5d68 145d 6815 5d68 165d 6817 5d75 6818  ]h.]h.]h.]h.]uh.
+00004770: 5d72 6103 0000 6a48 0200 0029 8172 6203  ]ra...jH...).rb.
+00004780: 0000 7d72 6303 0000 2868 1055 0068 117d  ..}rc...(h.U.h.}
+00004790: 7264 0300 0028 6813 5d68 145d 6815 5d68  rd...(h.]h.]h.]h
+000047a0: 165d 6817 5d75 681f 6a5e 0300 0068 185d  .]h.]uh.j^...h.]
+000047b0: 7265 0300 0028 6a4d 0200 0029 8172 6603  re...(jM...).rf.
+000047c0: 0000 7d72 6703 0000 2868 1055 0068 117d  ..}rg...(h.U.h.}
+000047d0: 7268 0300 0028 6813 5d68 145d 6815 5d68  rh...(h.]h.]h.]h
+000047e0: 165d 6817 5d75 681f 6a62 0300 0068 185d  .]h.]uh.jb...h.]
+000047f0: 7269 0300 006a 5202 0000 2981 726a 0300  ri...jR...).rj..
+00004800: 007d 726b 0300 0028 6810 5500 6811 7d72  .}rk...(h.U.h.}r
+00004810: 6c03 0000 2855 0a61 6e63 686f 726e 616d  l...(U.anchornam
+00004820: 6555 0055 0672 6566 7572 6968 3d68 165d  eU.U.refurih=h.]
+00004830: 6815 5d68 135d 6814 5d68 175d 5508 696e  h.]h.]h.]h.]U.in
+00004840: 7465 726e 616c 8875 681f 6a66 0300 0068  ternal.uh.jf...h
+00004850: 185d 726d 0300 0068 1a58 1500 0000 4f76  .]rm...h.X....Ov
+00004860: 6572 7669 6577 2061 6e64 2054 7574 6f72  erview and Tutor
+00004870: 6961 6c72 6e03 0000 8581 726f 0300 007d  ialrn.....ro...}
+00004880: 7270 0300 0028 6810 6845 681f 6a6a 0300  rp...(h.hEh.jj..
+00004890: 0075 6261 6820 6a5a 0200 0075 6261 6820  .ubah jZ...ubah 
+000048a0: 6a5b 0200 0075 626a 4302 0000 2981 7271  j[...ubjC...).rq
+000048b0: 0300 007d 7272 0300 0028 6810 5500 6811  ...}rr...(h.U.h.
+000048c0: 7d72 7303 0000 2868 135d 6814 5d68 155d  }rs...(h.]h.]h.]
+000048d0: 6816 5d68 175d 7568 1f6a 6203 0000 6818  h.]h.]uh.jb...h.
+000048e0: 5d72 7403 0000 286a 4802 0000 2981 7275  ]rt...(jH...).ru
+000048f0: 0300 007d 7276 0300 0028 6810 5500 6811  ...}rv...(h.U.h.
+00004900: 7d72 7703 0000 2868 135d 6814 5d68 155d  }rw...(h.]h.]h.]
+00004910: 6816 5d68 175d 7568 1f6a 7103 0000 6818  h.]h.]uh.jq...h.
+00004920: 5d72 7803 0000 6a4d 0200 0029 8172 7903  ]rx...jM...).ry.
+00004930: 0000 7d72 7a03 0000 2868 1055 0068 117d  ..}rz...(h.U.h.}
+00004940: 727b 0300 0028 6813 5d68 145d 6815 5d68  r{...(h.]h.]h.]h
+00004950: 165d 6817 5d75 681f 6a75 0300 0068 185d  .]h.]uh.ju...h.]
+00004960: 727c 0300 006a 5202 0000 2981 727d 0300  r|...jR...).r}..
+00004970: 007d 727e 0300 0028 6810 5500 6811 7d72  .}r~...(h.U.h.}r
+00004980: 7f03 0000 2855 0a61 6e63 686f 726e 616d  ....(U.anchornam
+00004990: 6555 0d23 696e 7472 6f64 7563 7469 6f6e  eU.#introduction
+000049a0: 5506 7265 6675 7269 683d 6816 5d68 155d  U.refurih=h.]h.]
+000049b0: 6813 5d68 145d 6817 5d55 0869 6e74 6572  h.]h.]h.]U.inter
+000049c0: 6e61 6c88 7568 1f6a 7903 0000 6818 5d72  nal.uh.jy...h.]r
+000049d0: 8003 0000 681a 580c 0000 0049 6e74 726f  ....h.X....Intro
+000049e0: 6475 6374 696f 6e72 8103 0000 8581 7282  ductionr......r.
+000049f0: 0300 007d 7283 0300 0028 6810 580c 0000  ...}r....(h.X...
+00004a00: 0049 6e74 726f 6475 6374 696f 6e72 8403  .Introductionr..
+00004a10: 0000 681f 6a7d 0300 0075 6261 6820 6a5a  ..h.j}...ubah jZ
+00004a20: 0200 0075 6261 6820 6a5b 0200 0075 6261  ...ubah j[...uba
+00004a30: 6820 6a72 0200 0075 626a 4802 0000 2981  h jr...ubjH...).
+00004a40: 7285 0300 007d 7286 0300 0028 6810 5500  r....}r....(h.U.
+00004a50: 6811 7d72 8703 0000 2868 135d 6814 5d68  h.}r....(h.]h.]h
+00004a60: 155d 6816 5d68 175d 7568 1f6a 7103 0000  .]h.]h.]uh.jq...
+00004a70: 6818 5d72 8803 0000 6a4d 0200 0029 8172  h.]r....jM...).r
+00004a80: 8903 0000 7d72 8a03 0000 2868 1055 0068  ....}r....(h.U.h
+00004a90: 117d 728b 0300 0028 6813 5d68 145d 6815  .}r....(h.]h.]h.
+00004aa0: 5d68 165d 6817 5d75 681f 6a85 0300 0068  ]h.]h.]uh.j....h
+00004ab0: 185d 728c 0300 006a 5202 0000 2981 728d  .]r....jR...).r.
+00004ac0: 0300 007d 728e 0300 0028 6810 5500 6811  ...}r....(h.U.h.
+00004ad0: 7d72 8f03 0000 2855 0a61 6e63 686f 726e  }r....(U.anchorn
+00004ae0: 616d 6555 3023 6761 7573 7369 616e 2d72  ameU0#gaussian-r
+00004af0: 616e 646f 6d2d 7661 7269 6162 6c65 732d  andom-variables-
+00004b00: 616e 642d 6572 726f 722d 7072 6f70 6167  and-error-propag
+00004b10: 6174 696f 6e55 0672 6566 7572 6968 3d68  ationU.refurih=h
+00004b20: 165d 6815 5d68 135d 6814 5d68 175d 5508  .]h.]h.]h.]h.]U.
+00004b30: 696e 7465 726e 616c 8875 681f 6a89 0300  internal.uh.j...
+00004b40: 0068 185d 7290 0300 0068 1a58 2f00 0000  .h.]r....h.X/...
+00004b50: 4761 7573 7369 616e 2052 616e 646f 6d20  Gaussian Random 
+00004b60: 5661 7269 6162 6c65 7320 616e 6420 4572  Variables and Er
+00004b70: 726f 7220 5072 6f70 6167 6174 696f 6e72  ror Propagationr
+00004b80: 9103 0000 8581 7292 0300 007d 7293 0300  ......r....}r...
+00004b90: 0028 6810 582f 0000 0047 6175 7373 6961  .(h.X/...Gaussia
+00004ba0: 6e20 5261 6e64 6f6d 2056 6172 6961 626c  n Random Variabl
+00004bb0: 6573 2061 6e64 2045 7272 6f72 2050 726f  es and Error Pro
+00004bc0: 7061 6761 7469 6f6e 7294 0300 0068 1f6a  pagationr....h.j
+00004bd0: 8d03 0000 7562 6168 206a 5a02 0000 7562  ....ubah jZ...ub
+00004be0: 6168 206a 5b02 0000 7562 6168 206a 7202  ah j[...ubah jr.
+00004bf0: 0000 7562 6a48 0200 0029 8172 9503 0000  ..ubjH...).r....
+00004c00: 7d72 9603 0000 2868 1055 0068 117d 7297  }r....(h.U.h.}r.
+00004c10: 0300 0028 6813 5d68 145d 6815 5d68 165d  ...(h.]h.]h.]h.]
+00004c20: 6817 5d75 681f 6a71 0300 0068 185d 7298  h.]uh.jq...h.]r.
+00004c30: 0300 006a 4d02 0000 2981 7299 0300 007d  ...jM...).r....}
+00004c40: 729a 0300 0028 6810 5500 6811 7d72 9b03  r....(h.U.h.}r..
+00004c50: 0000 2868 135d 6814 5d68 155d 6816 5d68  ..(h.]h.]h.]h.]h
+00004c60: 175d 7568 1f6a 9503 0000 6818 5d72 9c03  .]uh.j....h.]r..
+00004c70: 0000 6a52 0200 0029 8172 9d03 0000 7d72  ..jR...).r....}r
+00004c80: 9e03 0000 2868 1055 0068 117d 729f 0300  ....(h.U.h.}r...
+00004c90: 0028 550a 616e 6368 6f72 6e61 6d65 550b  .(U.anchornameU.
+00004ca0: 2362 6173 6963 2d66 6974 7355 0672 6566  #basic-fitsU.ref
+00004cb0: 7572 6968 3d68 165d 6815 5d68 135d 6814  urih=h.]h.]h.]h.
+00004cc0: 5d68 175d 5508 696e 7465 726e 616c 8875  ]h.]U.internal.u
+00004cd0: 681f 6a99 0300 0068 185d 72a0 0300 0068  h.j....h.]r....h
+00004ce0: 1a58 0a00 0000 4261 7369 6320 4669 7473  .X....Basic Fits
+00004cf0: 72a1 0300 0085 8172 a203 0000 7d72 a303  r......r....}r..
+00004d00: 0000 2868 1058 0a00 0000 4261 7369 6320  ..(h.X....Basic 
+00004d10: 4669 7473 72a4 0300 0068 1f6a 9d03 0000  Fitsr....h.j....
+00004d20: 7562 6168 206a 5a02 0000 7562 6168 206a  ubah jZ...ubah j
+00004d30: 5b02 0000 7562 6168 206a 7202 0000 7562  [...ubah jr...ub
+00004d40: 6a48 0200 0029 8172 a503 0000 7d72 a603  jH...).r....}r..
+00004d50: 0000 2868 1055 0068 117d 72a7 0300 0028  ..(h.U.h.}r....(
+00004d60: 6813 5d68 145d 6815 5d68 165d 6817 5d75  h.]h.]h.]h.]h.]u
+00004d70: 681f 6a71 0300 0068 185d 72a8 0300 006a  h.jq...h.]r....j
+00004d80: 4d02 0000 2981 72a9 0300 007d 72aa 0300  M...).r....}r...
+00004d90: 0028 6810 5500 6811 7d72 ab03 0000 2868  .(h.U.h.}r....(h
+00004da0: 135d 6814 5d68 155d 6816 5d68 175d 7568  .]h.]h.]h.]h.]uh
+00004db0: 1f6a a503 0000 6818 5d72 ac03 0000 6a52  .j....h.]r....jR
+00004dc0: 0200 0029 8172 ad03 0000 7d72 ae03 0000  ...).r....}r....
+00004dd0: 2868 1055 0068 117d 72af 0300 0028 550a  (h.U.h.}r....(U.
+00004de0: 616e 6368 6f72 6e61 6d65 551d 2363 6861  anchornameU.#cha
+00004df0: 696e 6564 2d66 6974 732d 6c61 7267 652d  ined-fits-large-
+00004e00: 6461 7461 2d73 6574 7355 0672 6566 7572  data-setsU.refur
+00004e10: 6968 3d68 165d 6815 5d68 135d 6814 5d68  ih=h.]h.]h.]h.]h
+00004e20: 175d 5508 696e 7465 726e 616c 8875 681f  .]U.internal.uh.
+00004e30: 6aa9 0300 0068 185d 72b0 0300 0068 1a58  j....h.]r....h.X
+00004e40: 1d00 0000 4368 6169 6e65 6420 4669 7473  ....Chained Fits
+00004e50: 3b20 4c61 7267 6520 4461 7461 2053 6574  ; Large Data Set
+00004e60: 7372 b103 0000 8581 72b2 0300 007d 72b3  sr......r....}r.
+00004e70: 0300 0028 6810 581d 0000 0043 6861 696e  ...(h.X....Chain
+00004e80: 6564 2046 6974 733b 204c 6172 6765 2044  ed Fits; Large D
+00004e90: 6174 6120 5365 7473 72b4 0300 0068 1f6a  ata Setsr....h.j
+00004ea0: ad03 0000 7562 6168 206a 5a02 0000 7562  ....ubah jZ...ub
+00004eb0: 6168 206a 5b02 0000 7562 6168 206a 7202  ah j[...ubah jr.
+00004ec0: 0000 7562 6a48 0200 0029 8172 b503 0000  ..ubjH...).r....
+00004ed0: 7d72 b603 0000 2868 1055 0068 117d 72b7  }r....(h.U.h.}r.
+00004ee0: 0300 0028 6813 5d68 145d 6815 5d68 165d  ...(h.]h.]h.]h.]
+00004ef0: 6817 5d75 681f 6a71 0300 0068 185d 72b8  h.]uh.jq...h.]r.
+00004f00: 0300 006a 4d02 0000 2981 72b9 0300 007d  ...jM...).r....}
+00004f10: 72ba 0300 0028 6810 5500 6811 7d72 bb03  r....(h.U.h.}r..
+00004f20: 0000 2868 135d 6814 5d68 155d 6816 5d68  ..(h.]h.]h.]h.]h
+00004f30: 175d 7568 1f6a b503 0000 6818 5d72 bc03  .]uh.j....h.]r..
+00004f40: 0000 6a52 0200 0029 8172 bd03 0000 7d72  ..jR...).r....}r
+00004f50: be03 0000 2868 1055 0068 117d 72bf 0300  ....(h.U.h.}r...
+00004f60: 0028 550a 616e 6368 6f72 6e61 6d65 550d  .(U.anchornameU.
+00004f70: 2378 2d68 6173 2d65 7272 6f72 7355 0672  #x-has-errorsU.r
+00004f80: 6566 7572 6968 3d68 165d 6815 5d68 135d  efurih=h.]h.]h.]
+00004f90: 6814 5d68 175d 5508 696e 7465 726e 616c  h.]h.]U.internal
+00004fa0: 8875 681f 6ab9 0300 0068 185d 72c0 0300  .uh.j....h.]r...
+00004fb0: 0028 6830 2981 72c1 0300 007d 72c2 0300  .(h0).r....}r...
+00004fc0: 0028 6810 5805 0000 0060 6078 6060 72c3  .(h.X....``x``r.
+00004fd0: 0300 0068 1f6a bd03 0000 6a63 0200 004e  ...h.j....jc...N
+00004fe0: 6820 6838 6811 7d72 c403 0000 2868 135d  h h8h.}r....(h.]
+00004ff0: 6814 5d68 155d 6816 5d68 175d 756a 7002  h.]h.]h.]h.]ujp.
+00005000: 0000 4e68 185d 72c5 0300 0068 1a58 0100  ..Nh.]r....h.X..
+00005010: 0000 7885 8172 c603 0000 7d72 c703 0000  ..x..r....}r....
+00005020: 2868 1055 0068 1f6a c103 0000 7562 6175  (h.U.h.j....ubau
+00005030: 6268 1a58 0b00 0000 2068 6173 2045 7272  bh.X.... has Err
+00005040: 6f72 7372 c803 0000 8581 72c9 0300 007d  orsr......r....}
+00005050: 72ca 0300 0028 6810 580b 0000 0020 6861  r....(h.X.... ha
+00005060: 7320 4572 726f 7273 72cb 0300 0068 1f6a  s Errorsr....h.j
+00005070: bd03 0000 7562 6568 206a 5a02 0000 7562  ....ubeh jZ...ub
+00005080: 6168 206a 5b02 0000 7562 6168 206a 7202  ah j[...ubah jr.
+00005090: 0000 7562 6a48 0200 0029 8172 cc03 0000  ..ubjH...).r....
+000050a0: 7d72 cd03 0000 2868 1055 0068 117d 72ce  }r....(h.U.h.}r.
+000050b0: 0300 0028 6813 5d68 145d 6815 5d68 165d  ...(h.]h.]h.]h.]
+000050c0: 6817 5d75 681f 6a71 0300 0068 185d 72cf  h.]uh.jq...h.]r.
+000050d0: 0300 006a 4d02 0000 2981 72d0 0300 007d  ...jM...).r....}
+000050e0: 72d1 0300 0028 6810 5500 6811 7d72 d203  r....(h.U.h.}r..
+000050f0: 0000 2868 135d 6814 5d68 155d 6816 5d68  ..(h.]h.]h.]h.]h
+00005100: 175d 7568 1f6a cc03 0000 6818 5d72 d303  .]uh.j....h.]r..
+00005110: 0000 6a52 0200 0029 8172 d403 0000 7d72  ..jR...).r....}r
+00005120: d503 0000 2868 1055 0068 117d 72d6 0300  ....(h.U.h.}r...
+00005130: 0028 550a 616e 6368 6f72 6e61 6d65 552c  .(U.anchornameU,
+00005140: 2363 6f72 7265 6c61 7465 642d 7061 7261  #correlated-para
+00005150: 6d65 7465 7273 2d67 6175 7373 6961 6e2d  meters-gaussian-
+00005160: 6261 7965 732d 6661 6374 6f72 5506 7265  bayes-factorU.re
+00005170: 6675 7269 683d 6816 5d68 155d 6813 5d68  furih=h.]h.]h.]h
+00005180: 145d 6817 5d55 0869 6e74 6572 6e61 6c88  .]h.]U.internal.
+00005190: 7568 1f6a d003 0000 6818 5d72 d703 0000  uh.j....h.]r....
+000051a0: 681a 582c 0000 0043 6f72 7265 6c61 7465  h.X,...Correlate
+000051b0: 6420 5061 7261 6d65 7465 7273 3b20 4761  d Parameters; Ga
+000051c0: 7573 7369 616e 2042 6179 6573 2046 6163  ussian Bayes Fac
+000051d0: 746f 7272 d803 0000 8581 72d9 0300 007d  torr......r....}
+000051e0: 72da 0300 0028 6810 582c 0000 0043 6f72  r....(h.X,...Cor
+000051f0: 7265 6c61 7465 6420 5061 7261 6d65 7465  related Paramete
+00005200: 7273 3b20 4761 7573 7369 616e 2042 6179  rs; Gaussian Bay
+00005210: 6573 2046 6163 746f 7272 db03 0000 681f  es Factorr....h.
+00005220: 6ad4 0300 0075 6261 6820 6a5a 0200 0075  j....ubah jZ...u
+00005230: 6261 6820 6a5b 0200 0075 6261 6820 6a72  bah j[...ubah jr
+00005240: 0200 0075 626a 4802 0000 2981 72dc 0300  ...ubjH...).r...
+00005250: 007d 72dd 0300 0028 6810 5500 6811 7d72  .}r....(h.U.h.}r
+00005260: de03 0000 2868 135d 6814 5d68 155d 6816  ....(h.]h.]h.]h.
+00005270: 5d68 175d 7568 1f6a 7103 0000 6818 5d72  ]h.]uh.jq...h.]r
+00005280: df03 0000 6a4d 0200 0029 8172 e003 0000  ....jM...).r....
+00005290: 7d72 e103 0000 2868 1055 0068 117d 72e2  }r....(h.U.h.}r.
+000052a0: 0300 0028 6813 5d68 145d 6815 5d68 165d  ...(h.]h.]h.]h.]
+000052b0: 6817 5d75 681f 6adc 0300 0068 185d 72e3  h.]uh.j....h.]r.
+000052c0: 0300 006a 5202 0000 2981 72e4 0300 007d  ...jR...).r....}
+000052d0: 72e5 0300 0028 6810 5500 6811 7d72 e603  r....(h.U.h.}r..
+000052e0: 0000 2855 0a61 6e63 686f 726e 616d 6555  ..(U.anchornameU
+000052f0: 1f23 792d 6861 732d 6e6f 2d65 7272 6f72  .#y-has-no-error
+00005300: 2d6d 6172 6769 6e61 6c69 7a61 7469 6f6e  -marginalization
+00005310: 5506 7265 6675 7269 683d 6816 5d68 155d  U.refurih=h.]h.]
+00005320: 6813 5d68 145d 6817 5d55 0869 6e74 6572  h.]h.]h.]U.inter
+00005330: 6e61 6c88 7568 1f6a e003 0000 6818 5d72  nal.uh.j....h.]r
+00005340: e703 0000 2868 3029 8172 e803 0000 7d72  ....(h0).r....}r
+00005350: e903 0000 2868 1058 0500 0000 6060 7960  ....(h.X....``y`
+00005360: 6072 ea03 0000 681f 6ae4 0300 006a 6302  `r....h.j....jc.
+00005370: 0000 4e68 2068 3868 117d 72eb 0300 0028  ..Nh h8h.}r....(
+00005380: 6813 5d68 145d 6815 5d68 165d 6817 5d75  h.]h.]h.]h.]h.]u
+00005390: 6a70 0200 004e 6818 5d72 ec03 0000 681a  jp...Nh.]r....h.
+000053a0: 5801 0000 0079 8581 72ed 0300 007d 72ee  X....y..r....}r.
+000053b0: 0300 0028 6810 5500 681f 6ae8 0300 0075  ...(h.U.h.j....u
+000053c0: 6261 7562 681a 581e 0000 0020 6861 7320  baubh.X.... has 
+000053d0: 4e6f 2045 7272 6f72 3b20 4d61 7267 696e  No Error; Margin
+000053e0: 616c 697a 6174 696f 6e72 ef03 0000 8581  alizationr......
+000053f0: 72f0 0300 007d 72f1 0300 0028 6810 581e  r....}r....(h.X.
+00005400: 0000 0020 6861 7320 4e6f 2045 7272 6f72  ... has No Error
+00005410: 3b20 4d61 7267 696e 616c 697a 6174 696f  ; Marginalizatio
+00005420: 6e72 f203 0000 681f 6ae4 0300 0075 6265  nr....h.j....ube
+00005430: 6820 6a5a 0200 0075 6261 6820 6a5b 0200  h jZ...ubah j[..
+00005440: 0075 6261 6820 6a72 0200 0075 626a 4802  .ubah jr...ubjH.
+00005450: 0000 2981 72f3 0300 007d 72f4 0300 0028  ..).r....}r....(
+00005460: 6810 5500 6811 7d72 f503 0000 2868 135d  h.U.h.}r....(h.]
+00005470: 6814 5d68 155d 6816 5d68 175d 7568 1f6a  h.]h.]h.]h.]uh.j
+00005480: 7103 0000 6818 5d72 f603 0000 6a4d 0200  q...h.]r....jM..
+00005490: 0029 8172 f703 0000 7d72 f803 0000 2868  .).r....}r....(h
+000054a0: 1055 0068 117d 72f9 0300 0028 6813 5d68  .U.h.}r....(h.]h
+000054b0: 145d 6815 5d68 165d 6817 5d75 681f 6af3  .]h.]h.]h.]uh.j.
+000054c0: 0300 0068 185d 72fa 0300 006a 5202 0000  ...h.]r....jR...
+000054d0: 2981 72fb 0300 007d 72fc 0300 0028 6810  ).r....}r....(h.
+000054e0: 5500 6811 7d72 fd03 0000 2855 0a61 6e63  U.h.}r....(U.anc
+000054f0: 686f 726e 616d 6555 1c23 7376 642d 6375  hornameU.#svd-cu
+00005500: 7473 2d61 6e64 2d72 6f75 6e64 6f66 662d  ts-and-roundoff-
+00005510: 6572 726f 7255 0672 6566 7572 6968 3d68  errorU.refurih=h
+00005520: 165d 6815 5d68 135d 6814 5d68 175d 5508  .]h.]h.]h.]h.]U.
+00005530: 696e 7465 726e 616c 8875 681f 6af7 0300  internal.uh.j...
+00005540: 0068 185d 72fe 0300 0068 1a58 1b00 0000  .h.]r....h.X....
+00005550: 5356 4420 4375 7473 2061 6e64 2052 6f75  SVD Cuts and Rou
+00005560: 6e64 6f66 6620 4572 726f 7272 ff03 0000  ndoff Errorr....
+00005570: 8581 7200 0400 007d 7201 0400 0028 6810  ..r....}r....(h.
+00005580: 581b 0000 0053 5644 2043 7574 7320 616e  X....SVD Cuts an
+00005590: 6420 526f 756e 646f 6666 2045 7272 6f72  d Roundoff Error
+000055a0: 7202 0400 0068 1f6a fb03 0000 7562 6168  r....h.j....ubah
+000055b0: 206a 5a02 0000 7562 6168 206a 5b02 0000   jZ...ubah j[...
+000055c0: 7562 6168 206a 7202 0000 7562 6a48 0200  ubah jr...ubjH..
+000055d0: 0029 8172 0304 0000 7d72 0404 0000 2868  .).r....}r....(h
+000055e0: 1055 0068 117d 7205 0400 0028 6813 5d68  .U.h.}r....(h.]h
+000055f0: 145d 6815 5d68 165d 6817 5d75 681f 6a71  .]h.]h.]h.]uh.jq
+00005600: 0300 0068 185d 7206 0400 006a 4d02 0000  ...h.]r....jM...
+00005610: 2981 7207 0400 007d 7208 0400 0028 6810  ).r....}r....(h.
+00005620: 5500 6811 7d72 0904 0000 2868 135d 6814  U.h.}r....(h.]h.
+00005630: 5d68 155d 6816 5d68 175d 7568 1f6a 0304  ]h.]h.]h.]uh.j..
+00005640: 0000 6818 5d72 0a04 0000 6a52 0200 0029  ..h.]r....jR...)
+00005650: 8172 0b04 0000 7d72 0c04 0000 2868 1055  .r....}r....(h.U
+00005660: 0068 117d 720d 0400 0028 550a 616e 6368  .h.}r....(U.anch
+00005670: 6f72 6e61 6d65 5515 2379 2d68 6173 2d75  ornameU.#y-has-u
+00005680: 6e6b 6e6f 776e 2d65 7272 6f72 7355 0672  nknown-errorsU.r
+00005690: 6566 7572 6968 3d68 165d 6815 5d68 135d  efurih=h.]h.]h.]
+000056a0: 6814 5d68 175d 5508 696e 7465 726e 616c  h.]h.]U.internal
+000056b0: 8875 681f 6a07 0400 0068 185d 720e 0400  .uh.j....h.]r...
+000056c0: 0028 6830 2981 720f 0400 007d 7210 0400  .(h0).r....}r...
+000056d0: 0028 6810 5805 0000 0060 6079 6060 7211  .(h.X....``y``r.
+000056e0: 0400 0068 1f6a 0b04 0000 6a63 0200 004e  ...h.j....jc...N
+000056f0: 6820 6838 6811 7d72 1204 0000 2868 135d  h h8h.}r....(h.]
+00005700: 6814 5d68 155d 6816 5d68 175d 756a 7002  h.]h.]h.]h.]ujp.
+00005710: 0000 4e68 185d 7213 0400 0068 1a58 0100  ..Nh.]r....h.X..
+00005720: 0000 7985 8172 1404 0000 7d72 1504 0000  ..y..r....}r....
+00005730: 2868 1055 0068 1f6a 0f04 0000 7562 6175  (h.U.h.j....ubau
+00005740: 6268 1a58 1300 0000 2068 6173 2055 6e6b  bh.X.... has Unk
+00005750: 6e6f 776e 2045 7272 6f72 7372 1604 0000  nown Errorsr....
+00005760: 8581 7217 0400 007d 7218 0400 0028 6810  ..r....}r....(h.
+00005770: 5813 0000 0020 6861 7320 556e 6b6e 6f77  X.... has Unknow
+00005780: 6e20 4572 726f 7273 7219 0400 0068 1f6a  n Errorsr....h.j
+00005790: 0b04 0000 7562 6568 206a 5a02 0000 7562  ....ubeh jZ...ub
+000057a0: 6168 206a 5b02 0000 7562 6168 206a 7202  ah j[...ubah jr.
+000057b0: 0000 7562 6a48 0200 0029 8172 1a04 0000  ..ubjH...).r....
+000057c0: 7d72 1b04 0000 2868 1055 0068 117d 721c  }r....(h.U.h.}r.
+000057d0: 0400 0028 6813 5d68 145d 6815 5d68 165d  ...(h.]h.]h.]h.]
+000057e0: 6817 5d75 681f 6a71 0300 0068 185d 721d  h.]uh.jq...h.]r.
+000057f0: 0400 006a 4d02 0000 2981 721e 0400 007d  ...jM...).r....}
+00005800: 721f 0400 0028 6810 5500 6811 7d72 2004  r....(h.U.h.}r .
+00005810: 0000 2868 135d 6814 5d68 155d 6816 5d68  ..(h.]h.]h.]h.]h
+00005820: 175d 7568 1f6a 1a04 0000 6818 5d72 2104  .]uh.j....h.]r!.
+00005830: 0000 6a52 0200 0029 8172 2204 0000 7d72  ..jR...).r"...}r
+00005840: 2304 0000 2868 1055 0068 117d 7224 0400  #...(h.U.h.}r$..
+00005850: 0028 550a 616e 6368 6f72 6e61 6d65 5531  .(U.anchornameU1
+00005860: 2374 756e 696e 672d 7072 696f 7273 2d77  #tuning-priors-w
+00005870: 6974 682d 7468 652d 656d 7069 7269 6361  ith-the-empirica
+00005880: 6c2d 6261 7965 732d 6372 6974 6572 696f  l-bayes-criterio
+00005890: 6e55 0672 6566 7572 6968 3d68 165d 6815  nU.refurih=h.]h.
+000058a0: 5d68 135d 6814 5d68 175d 5508 696e 7465  ]h.]h.]h.]U.inte
+000058b0: 726e 616c 8875 681f 6a1e 0400 0068 185d  rnal.uh.j....h.]
+000058c0: 7225 0400 0068 1a58 3000 0000 5475 6e69  r%...h.X0...Tuni
+000058d0: 6e67 2050 7269 6f72 7320 7769 7468 2074  ng Priors with t
+000058e0: 6865 2045 6d70 6972 6963 616c 2042 6179  he Empirical Bay
+000058f0: 6573 2043 7269 7465 7269 6f6e 7226 0400  es Criterionr&..
+00005900: 0085 8172 2704 0000 7d72 2804 0000 2868  ...r'...}r(...(h
+00005910: 1058 3000 0000 5475 6e69 6e67 2050 7269  .X0...Tuning Pri
+00005920: 6f72 7320 7769 7468 2074 6865 2045 6d70  ors with the Emp
+00005930: 6972 6963 616c 2042 6179 6573 2043 7269  irical Bayes Cri
+00005940: 7465 7269 6f6e 7229 0400 0068 1f6a 2204  terionr)...h.j".
+00005950: 0000 7562 6168 206a 5a02 0000 7562 6168  ..ubah jZ...ubah
+00005960: 206a 5b02 0000 7562 6168 206a 7202 0000   j[...ubah jr...
+00005970: 7562 6a48 0200 0029 8172 2a04 0000 7d72  ubjH...).r*...}r
+00005980: 2b04 0000 2868 1055 0068 117d 722c 0400  +...(h.U.h.}r,..
+00005990: 0028 6813 5d68 145d 6815 5d68 165d 6817  .(h.]h.]h.]h.]h.
+000059a0: 5d75 681f 6a71 0300 0068 185d 722d 0400  ]uh.jq...h.]r-..
+000059b0: 006a 4d02 0000 2981 722e 0400 007d 722f  .jM...).r....}r/
+000059c0: 0400 0028 6810 5500 6811 7d72 3004 0000  ...(h.U.h.}r0...
+000059d0: 2868 135d 6814 5d68 155d 6816 5d68 175d  (h.]h.]h.]h.]h.]
+000059e0: 7568 1f6a 2a04 0000 6818 5d72 3104 0000  uh.j*...h.]r1...
+000059f0: 6a52 0200 0029 8172 3204 0000 7d72 3304  jR...).r2...}r3.
+00005a00: 0000 2868 1055 0068 117d 7234 0400 0028  ..(h.U.h.}r4...(
+00005a10: 550a 616e 6368 6f72 6e61 6d65 5528 2370  U.anchornameU(#p
+00005a20: 6f73 6974 6976 652d 7061 7261 6d65 7465  ositive-paramete
+00005a30: 7273 2d6e 6f6e 2d67 6175 7373 6961 6e2d  rs-non-gaussian-
+00005a40: 7072 696f 7273 5506 7265 6675 7269 683d  priorsU.refurih=
+00005a50: 6816 5d68 155d 6813 5d68 145d 6817 5d55  h.]h.]h.]h.]h.]U
+00005a60: 0869 6e74 6572 6e61 6c88 7568 1f6a 2e04  .internal.uh.j..
+00005a70: 0000 6818 5d72 3504 0000 681a 5828 0000  ..h.]r5...h.X(..
+00005a80: 0050 6f73 6974 6976 6520 5061 7261 6d65  .Positive Parame
+00005a90: 7465 7273 3b20 4e6f 6e2d 4761 7573 7369  ters; Non-Gaussi
+00005aa0: 616e 2050 7269 6f72 7372 3604 0000 8581  an Priorsr6.....
+00005ab0: 7237 0400 007d 7238 0400 0028 6810 5828  r7...}r8...(h.X(
+00005ac0: 0000 0050 6f73 6974 6976 6520 5061 7261  ...Positive Para
+00005ad0: 6d65 7465 7273 3b20 4e6f 6e2d 4761 7573  meters; Non-Gaus
+00005ae0: 7369 616e 2050 7269 6f72 7372 3904 0000  sian Priorsr9...
+00005af0: 681f 6a32 0400 0075 6261 6820 6a5a 0200  h.j2...ubah jZ..
+00005b00: 0075 6261 6820 6a5b 0200 0075 6261 6820  .ubah j[...ubah 
+00005b10: 6a72 0200 0075 626a 4802 0000 2981 723a  jr...ubjH...).r:
+00005b20: 0400 007d 723b 0400 0028 6810 5500 6811  ...}r;...(h.U.h.
+00005b30: 7d72 3c04 0000 2868 135d 6814 5d68 155d  }r<...(h.]h.]h.]
+00005b40: 6816 5d68 175d 7568 1f6a 7103 0000 6818  h.]h.]uh.jq...h.
+00005b50: 5d72 3d04 0000 6a4d 0200 0029 8172 3e04  ]r=...jM...).r>.
+00005b60: 0000 7d72 3f04 0000 2868 1055 0068 117d  ..}r?...(h.U.h.}
+00005b70: 7240 0400 0028 6813 5d68 145d 6815 5d68  r@...(h.]h.]h.]h
+00005b80: 165d 6817 5d75 681f 6a3a 0400 0068 185d  .]h.]uh.j:...h.]
+00005b90: 7241 0400 006a 5202 0000 2981 7242 0400  rA...jR...).rB..
+00005ba0: 007d 7243 0400 0028 6810 5500 6811 7d72  .}rC...(h.U.h.}r
+00005bb0: 4404 0000 2855 0a61 6e63 686f 726e 616d  D...(U.anchornam
+00005bc0: 6555 0f23 6661 7374 6572 2d66 6974 7465  eU.#faster-fitte
+00005bd0: 7273 5506 7265 6675 7269 683d 6816 5d68  rsU.refurih=h.]h
+00005be0: 155d 6813 5d68 145d 6817 5d55 0869 6e74  .]h.]h.]h.]U.int
+00005bf0: 6572 6e61 6c88 7568 1f6a 3e04 0000 6818  ernal.uh.j>...h.
+00005c00: 5d72 4504 0000 681a 580e 0000 0046 6173  ]rE...h.X....Fas
+00005c10: 7465 7220 4669 7474 6572 7372 4604 0000  ter FittersrF...
+00005c20: 8581 7247 0400 007d 7248 0400 0028 6810  ..rG...}rH...(h.
+00005c30: 580e 0000 0046 6173 7465 7220 4669 7474  X....Faster Fitt
+00005c40: 6572 7372 4904 0000 681f 6a42 0400 0075  ersrI...h.jB...u
+00005c50: 6261 6820 6a5a 0200 0075 6261 6820 6a5b  bah jZ...ubah j[
+00005c60: 0200 0075 6261 6820 6a72 0200 0075 626a  ...ubah jr...ubj
+00005c70: 4802 0000 2981 724a 0400 007d 724b 0400  H...).rJ...}rK..
+00005c80: 0028 6810 5500 6811 7d72 4c04 0000 2868  .(h.U.h.}rL...(h
+00005c90: 135d 6814 5d68 155d 6816 5d68 175d 7568  .]h.]h.]h.]h.]uh
+00005ca0: 1f6a 7103 0000 6818 5d72 4d04 0000 6a4d  .jq...h.]rM...jM
+00005cb0: 0200 0029 8172 4e04 0000 7d72 4f04 0000  ...).rN...}rO...
+00005cc0: 2868 1055 0068 117d 7250 0400 0028 6813  (h.U.h.}rP...(h.
+00005cd0: 5d68 145d 6815 5d68 165d 6817 5d75 681f  ]h.]h.]h.]h.]uh.
+00005ce0: 6a4a 0400 0068 185d 7251 0400 006a 5202  jJ...h.]rQ...jR.
+00005cf0: 0000 2981 7252 0400 007d 7253 0400 0028  ..).rR...}rS...(
+00005d00: 6810 5500 6811 7d72 5404 0000 2855 0a61  h.U.h.}rT...(U.a
+00005d10: 6e63 686f 726e 616d 6555 1e23 6465 6275  nchornameU.#debu
+00005d20: 6767 696e 672d 616e 642d 7472 6f75 626c  gging-and-troubl
+00005d30: 6573 686f 6f74 696e 6755 0672 6566 7572  eshootingU.refur
+00005d40: 6968 3d68 165d 6815 5d68 135d 6814 5d68  ih=h.]h.]h.]h.]h
+00005d50: 175d 5508 696e 7465 726e 616c 8875 681f  .]U.internal.uh.
+00005d60: 6a4e 0400 0068 185d 7255 0400 0068 1a58  jN...h.]rU...h.X
+00005d70: 1d00 0000 4465 6275 6767 696e 6720 616e  ....Debugging an
+00005d80: 6420 5472 6f75 626c 6573 686f 6f74 696e  d Troubleshootin
+00005d90: 6772 5604 0000 8581 7257 0400 007d 7258  grV.....rW...}rX
+00005da0: 0400 0028 6810 581d 0000 0044 6562 7567  ...(h.X....Debug
+00005db0: 6769 6e67 2061 6e64 2054 726f 7562 6c65  ging and Trouble
+00005dc0: 7368 6f6f 7469 6e67 7259 0400 0068 1f6a  shootingrY...h.j
+00005dd0: 5204 0000 7562 6168 206a 5a02 0000 7562  R...ubah jZ...ub
+00005de0: 6168 206a 5b02 0000 7562 6168 206a 7202  ah j[...ubah jr.
+00005df0: 0000 7562 6568 206a 7102 0000 7562 6568  ..ubeh jq...ubeh
+00005e00: 206a 7202 0000 7562 6168 206a 7102 0000   jr...ubah jq...
+00005e10: 7562 6846 6a43 0200 0029 8172 5a04 0000  ubhFjC...).rZ...
+00005e20: 7d72 5b04 0000 2868 1055 0068 117d 725c  }r[...(h.U.h.}r\
+00005e30: 0400 0028 6813 5d68 145d 6815 5d68 165d  ...(h.]h.]h.]h.]
+00005e40: 6817 5d75 6818 5d72 5d04 0000 6a48 0200  h.]uh.]r]...jH..
+00005e50: 0029 8172 5e04 0000 7d72 5f04 0000 2868  .).r^...}r_...(h
+00005e60: 1055 0068 117d 7260 0400 0028 6813 5d68  .U.h.}r`...(h.]h
+00005e70: 145d 6815 5d68 165d 6817 5d75 681f 6a5a  .]h.]h.]h.]uh.jZ
+00005e80: 0400 0068 185d 7261 0400 0028 6a4d 0200  ...h.]ra...(jM..
+00005e90: 0029 8172 6204 0000 7d72 6304 0000 2868  .).rb...}rc...(h
+00005ea0: 1055 0068 117d 7264 0400 0028 6813 5d68  .U.h.}rd...(h.]h
+00005eb0: 145d 6815 5d68 165d 6817 5d75 681f 6a5e  .]h.]h.]h.]uh.j^
+00005ec0: 0400 0068 185d 7265 0400 006a 5202 0000  ...h.]re...jR...
+00005ed0: 2981 7266 0400 007d 7267 0400 0028 6810  ).rf...}rg...(h.
+00005ee0: 5500 6811 7d72 6804 0000 2855 0a61 6e63  U.h.}rh...(U.anc
+00005ef0: 686f 726e 616d 6555 0055 0672 6566 7572  hornameU.U.refur
+00005f00: 6968 4668 165d 6815 5d68 135d 6814 5d68  ihFh.]h.]h.]h.]h
+00005f10: 175d 5508 696e 7465 726e 616c 8875 681f  .]U.internal.uh.
+00005f20: 6a62 0400 0068 185d 7269 0400 0068 1a58  jb...h.]ri...h.X
+00005f30: 2000 0000 4361 7365 2053 7475 6479 3a20   ...Case Study: 
+00005f40: 5369 6d70 6c65 2045 7874 7261 706f 6c61  Simple Extrapola
+00005f50: 7469 6f6e 726a 0400 0085 8172 6b04 0000  tionrj.....rk...
+00005f60: 7d72 6c04 0000 2868 1068 4e68 1f6a 6604  }rl...(h.hNh.jf.
+00005f70: 0000 7562 6168 206a 5a02 0000 7562 6168  ..ubah jZ...ubah
+00005f80: 206a 5b02 0000 7562 6a43 0200 0029 8172   j[...ubjC...).r
+00005f90: 6d04 0000 7d72 6e04 0000 2868 1055 0068  m...}rn...(h.U.h
+00005fa0: 117d 726f 0400 0028 6813 5d68 145d 6815  .}ro...(h.]h.]h.
+00005fb0: 5d68 165d 6817 5d75 681f 6a5e 0400 0068  ]h.]h.]uh.j^...h
+00005fc0: 185d 7270 0400 0028 6a48 0200 0029 8172  .]rp...(jH...).r
+00005fd0: 7104 0000 7d72 7204 0000 2868 1055 0068  q...}rr...(h.U.h
+00005fe0: 117d 7273 0400 0028 6813 5d68 145d 6815  .}rs...(h.]h.]h.
+00005ff0: 5d68 165d 6817 5d75 681f 6a6d 0400 0068  ]h.]h.]uh.jm...h
+00006000: 185d 7274 0400 006a 4d02 0000 2981 7275  .]rt...jM...).ru
+00006010: 0400 007d 7276 0400 0028 6810 5500 6811  ...}rv...(h.U.h.
+00006020: 7d72 7704 0000 2868 135d 6814 5d68 155d  }rw...(h.]h.]h.]
+00006030: 6816 5d68 175d 7568 1f6a 7104 0000 6818  h.]h.]uh.jq...h.
+00006040: 5d72 7804 0000 6a52 0200 0029 8172 7904  ]rx...jR...).ry.
+00006050: 0000 7d72 7a04 0000 2868 1055 0068 117d  ..}rz...(h.U.h.}
+00006060: 727b 0400 0028 550a 616e 6368 6f72 6e61  r{...(U.anchorna
+00006070: 6d65 550c 2374 6865 2d70 726f 626c 656d  meU.#the-problem
+00006080: 5506 7265 6675 7269 6846 6816 5d68 155d  U.refurihFh.]h.]
+00006090: 6813 5d68 145d 6817 5d55 0869 6e74 6572  h.]h.]h.]U.inter
+000060a0: 6e61 6c88 7568 1f6a 7504 0000 6818 5d72  nal.uh.ju...h.]r
+000060b0: 7c04 0000 681a 580b 0000 0054 6865 2050  |...h.X....The P
+000060c0: 726f 626c 656d 727d 0400 0085 8172 7e04  roblemr}.....r~.
+000060d0: 0000 7d72 7f04 0000 2868 1058 0b00 0000  ..}r....(h.X....
+000060e0: 5468 6520 5072 6f62 6c65 6d68 1f6a 7904  The Problemh.jy.
+000060f0: 0000 7562 6168 206a 5a02 0000 7562 6168  ..ubah jZ...ubah
+00006100: 206a 5b02 0000 7562 6168 206a 7202 0000   j[...ubah jr...
+00006110: 7562 6a48 0200 0029 8172 8004 0000 7d72  ubjH...).r....}r
+00006120: 8104 0000 2868 1055 0068 117d 7282 0400  ....(h.U.h.}r...
+00006130: 0028 6813 5d68 145d 6815 5d68 165d 6817  .(h.]h.]h.]h.]h.
+00006140: 5d75 681f 6a6d 0400 0068 185d 7283 0400  ]uh.jm...h.]r...
+00006150: 006a 4d02 0000 2981 7284 0400 007d 7285  .jM...).r....}r.
+00006160: 0400 0028 6810 5500 6811 7d72 8604 0000  ...(h.U.h.}r....
+00006170: 2868 135d 6814 5d68 155d 6816 5d68 175d  (h.]h.]h.]h.]h.]
+00006180: 7568 1f6a 8004 0000 6818 5d72 8704 0000  uh.j....h.]r....
+00006190: 6a52 0200 0029 8172 8804 0000 7d72 8904  jR...).r....}r..
+000061a0: 0000 2868 1055 0068 117d 728a 0400 0028  ..(h.U.h.}r....(
+000061b0: 550a 616e 6368 6f72 6e61 6d65 550f 2361  U.anchornameU.#a
+000061c0: 2d62 6164 2d73 6f6c 7574 696f 6e55 0672  -bad-solutionU.r
+000061d0: 6566 7572 6968 4668 165d 6815 5d68 135d  efurihFh.]h.]h.]
+000061e0: 6814 5d68 175d 5508 696e 7465 726e 616c  h.]h.]U.internal
+000061f0: 8875 681f 6a84 0400 0068 185d 728b 0400  .uh.j....h.]r...
+00006200: 0068 1a58 0e00 0000 4120 4261 6420 536f  .h.X....A Bad So
+00006210: 6c75 7469 6f6e 728c 0400 0085 8172 8d04  lutionr......r..
+00006220: 0000 7d72 8e04 0000 2868 1058 0e00 0000  ..}r....(h.X....
+00006230: 4120 4261 6420 536f 6c75 7469 6f6e 681f  A Bad Solutionh.
+00006240: 6a88 0400 0075 6261 6820 6a5a 0200 0075  j....ubah jZ...u
+00006250: 6261 6820 6a5b 0200 0075 6261 6820 6a72  bah j[...ubah jr
+00006260: 0200 0075 626a 4802 0000 2981 728f 0400  ...ubjH...).r...
+00006270: 007d 7290 0400 0028 6810 5500 6811 7d72  .}r....(h.U.h.}r
+00006280: 9104 0000 2868 135d 6814 5d68 155d 6816  ....(h.]h.]h.]h.
+00006290: 5d68 175d 7568 1f6a 6d04 0000 6818 5d72  ]h.]uh.jm...h.]r
+000062a0: 9204 0000 6a4d 0200 0029 8172 9304 0000  ....jM...).r....
+000062b0: 7d72 9404 0000 2868 1055 0068 117d 7295  }r....(h.U.h.}r.
+000062c0: 0400 0028 6813 5d68 145d 6815 5d68 165d  ...(h.]h.]h.]h.]
+000062d0: 6817 5d75 681f 6a8f 0400 0068 185d 7296  h.]uh.j....h.]r.
+000062e0: 0400 006a 5202 0000 2981 7297 0400 007d  ...jR...).r....}
+000062f0: 7298 0400 0028 6810 5500 6811 7d72 9904  r....(h.U.h.}r..
+00006300: 0000 2855 0a61 6e63 686f 726e 616d 6555  ..(U.anchornameU
+00006310: 1923 612d 6265 7474 6572 2d73 6f6c 7574  .#a-better-solut
+00006320: 696f 6e2d 7072 696f 7273 5506 7265 6675  ion-priorsU.refu
+00006330: 7269 6846 6816 5d68 155d 6813 5d68 145d  rihFh.]h.]h.]h.]
+00006340: 6817 5d55 0869 6e74 6572 6e61 6c88 7568  h.]U.internal.uh
+00006350: 1f6a 9304 0000 6818 5d72 9a04 0000 681a  .j....h.]r....h.
+00006360: 581c 0000 0041 2042 6574 7465 7220 536f  X....A Better So
+00006370: 6c75 7469 6f6e 20e2 8094 2050 7269 6f72  lution ... Prior
+00006380: 7372 9b04 0000 8581 729c 0400 007d 729d  sr......r....}r.
+00006390: 0400 0028 6810 581c 0000 0041 2042 6574  ...(h.X....A Bet
+000063a0: 7465 7220 536f 6c75 7469 6f6e 202d 2d2d  ter Solution ---
+000063b0: 2050 7269 6f72 7368 1f6a 9704 0000 7562   Priorsh.j....ub
+000063c0: 6168 206a 5a02 0000 7562 6168 206a 5b02  ah jZ...ubah j[.
+000063d0: 0000 7562 6168 206a 7202 0000 7562 6a48  ..ubah jr...ubjH
+000063e0: 0200 0029 8172 9e04 0000 7d72 9f04 0000  ...).r....}r....
+000063f0: 2868 1055 0068 117d 72a0 0400 0028 6813  (h.U.h.}r....(h.
+00006400: 5d68 145d 6815 5d68 165d 6817 5d75 681f  ]h.]h.]h.]h.]uh.
+00006410: 6a6d 0400 0068 185d 72a1 0400 006a 4d02  jm...h.]r....jM.
+00006420: 0000 2981 72a2 0400 007d 72a3 0400 0028  ..).r....}r....(
+00006430: 6810 5500 6811 7d72 a404 0000 2868 135d  h.U.h.}r....(h.]
+00006440: 6814 5d68 155d 6816 5d68 175d 7568 1f6a  h.]h.]h.]h.]uh.j
+00006450: 9e04 0000 6818 5d72 a504 0000 6a52 0200  ....h.]r....jR..
+00006460: 0029 8172 a604 0000 7d72 a704 0000 2868  .).r....}r....(h
+00006470: 1055 0068 117d 72a8 0400 0028 550a 616e  .U.h.}r....(U.an
+00006480: 6368 6f72 6e61 6d65 550e 2362 6179 6573  chornameU.#bayes
+00006490: 2d66 6163 746f 7273 5506 7265 6675 7269  -factorsU.refuri
+000064a0: 6846 6816 5d68 155d 6813 5d68 145d 6817  hFh.]h.]h.]h.]h.
+000064b0: 5d55 0869 6e74 6572 6e61 6c88 7568 1f6a  ]U.internal.uh.j
+000064c0: a204 0000 6818 5d72 a904 0000 681a 580d  ....h.]r....h.X.
+000064d0: 0000 0042 6179 6573 2046 6163 746f 7273  ...Bayes Factors
+000064e0: 72aa 0400 0085 8172 ab04 0000 7d72 ac04  r......r....}r..
+000064f0: 0000 2868 1058 0d00 0000 4261 7965 7320  ..(h.X....Bayes 
+00006500: 4661 6374 6f72 7368 1f6a a604 0000 7562  Factorsh.j....ub
+00006510: 6168 206a 5a02 0000 7562 6168 206a 5b02  ah jZ...ubah j[.
+00006520: 0000 7562 6168 206a 7202 0000 7562 6a48  ..ubah jr...ubjH
+00006530: 0200 0029 8172 ad04 0000 7d72 ae04 0000  ...).r....}r....
+00006540: 2868 1055 0068 117d 72af 0400 0028 6813  (h.U.h.}r....(h.
+00006550: 5d68 145d 6815 5d68 165d 6817 5d75 681f  ]h.]h.]h.]h.]uh.
+00006560: 6a6d 0400 0068 185d 72b0 0400 006a 4d02  jm...h.]r....jM.
+00006570: 0000 2981 72b1 0400 007d 72b2 0400 0028  ..).r....}r....(
+00006580: 6810 5500 6811 7d72 b304 0000 2868 135d  h.U.h.}r....(h.]
+00006590: 6814 5d68 155d 6816 5d68 175d 7568 1f6a  h.]h.]h.]h.]uh.j
+000065a0: ad04 0000 6818 5d72 b404 0000 6a52 0200  ....h.]r....jR..
+000065b0: 0029 8172 b504 0000 7d72 b604 0000 2868  .).r....}r....(h
+000065c0: 1055 0068 117d 72b7 0400 0028 550a 616e  .U.h.}r....(U.an
+000065d0: 6368 6f72 6e61 6d65 5521 2361 6e6f 7468  chornameU!#anoth
+000065e0: 6572 2d73 6f6c 7574 696f 6e2d 6d61 7267  er-solution-marg
+000065f0: 696e 616c 697a 6174 696f 6e55 0672 6566  inalizationU.ref
+00006600: 7572 6968 4668 165d 6815 5d68 135d 6814  urihFh.]h.]h.]h.
+00006610: 5d68 175d 5508 696e 7465 726e 616c 8875  ]h.]U.internal.u
+00006620: 681f 6ab1 0400 0068 185d 72b8 0400 0068  h.j....h.]r....h
+00006630: 1a58 2400 0000 416e 6f74 6865 7220 536f  .X$...Another So
+00006640: 6c75 7469 6f6e 20e2 8094 204d 6172 6769  lution ... Margi
+00006650: 6e61 6c69 7a61 7469 6f6e 72b9 0400 0085  nalizationr.....
+00006660: 8172 ba04 0000 7d72 bb04 0000 2868 1058  .r....}r....(h.X
+00006670: 2400 0000 416e 6f74 6865 7220 536f 6c75  $...Another Solu
+00006680: 7469 6f6e 202d 2d2d 204d 6172 6769 6e61  tion --- Margina
+00006690: 6c69 7a61 7469 6f6e 681f 6ab5 0400 0075  lizationh.j....u
+000066a0: 6261 6820 6a5a 0200 0075 6261 6820 6a5b  bah jZ...ubah j[
+000066b0: 0200 0075 6261 6820 6a72 0200 0075 6265  ...ubah jr...ube
+000066c0: 6820 6a71 0200 0075 6265 6820 6a72 0200  h jq...ubeh jr..
+000066d0: 0075 6261 6820 6a71 0200 0075 6268 4f6a  .ubah jq...ubhOj
+000066e0: 4302 0000 2981 72bc 0400 007d 72bd 0400  C...).r....}r...
+000066f0: 0028 6810 5500 6811 7d72 be04 0000 2868  .(h.U.h.}r....(h
+00006700: 135d 6814 5d68 155d 6816 5d68 175d 7568  .]h.]h.]h.]h.]uh
+00006710: 185d 72bf 0400 006a 4802 0000 2981 72c0  .]r....jH...).r.
+00006720: 0400 007d 72c1 0400 0028 6810 5500 6811  ...}r....(h.U.h.
+00006730: 7d72 c204 0000 2868 135d 6814 5d68 155d  }r....(h.]h.]h.]
+00006740: 6816 5d68 175d 7568 1f6a bc04 0000 6818  h.]h.]uh.j....h.
+00006750: 5d72 c304 0000 286a 4d02 0000 2981 72c4  ]r....(jM...).r.
+00006760: 0400 007d 72c5 0400 0028 6810 5500 6811  ...}r....(h.U.h.
+00006770: 7d72 c604 0000 2868 135d 6814 5d68 155d  }r....(h.]h.]h.]
+00006780: 6816 5d68 175d 7568 1f6a c004 0000 6818  h.]h.]uh.j....h.
+00006790: 5d72 c704 0000 6a52 0200 0029 8172 c804  ]r....jR...).r..
+000067a0: 0000 7d72 c904 0000 2868 1055 0068 117d  ..}r....(h.U.h.}
+000067b0: 72ca 0400 0028 550a 616e 6368 6f72 6e61  r....(U.anchorna
+000067c0: 6d65 5500 5506 7265 6675 7269 684f 6816  meU.U.refurihOh.
+000067d0: 5d68 155d 6813 5d68 145d 6817 5d55 0869  ]h.]h.]h.]h.]U.i
+000067e0: 6e74 6572 6e61 6c88 7568 1f6a c404 0000  nternal.uh.j....
+000067f0: 6818 5d72 cb04 0000 681a 582b 0000 0043  h.]r....h.X+...C
+00006800: 6173 6520 5374 7564 793a 204f 7574 6c69  ase Study: Outli
+00006810: 6572 7320 616e 6420 4261 7965 7369 616e  ers and Bayesian
+00006820: 2049 6e74 6567 7261 6c73 72cc 0400 0085   Integralsr.....
+00006830: 8172 cd04 0000 7d72 ce04 0000 2868 1068  .r....}r....(h.h
+00006840: 5768 1f6a c804 0000 7562 6168 206a 5a02  Wh.j....ubah jZ.
+00006850: 0000 7562 6168 206a 5b02 0000 7562 6a43  ..ubah j[...ubjC
+00006860: 0200 0029 8172 cf04 0000 7d72 d004 0000  ...).r....}r....
+00006870: 2868 1055 0068 117d 72d1 0400 0028 6813  (h.U.h.}r....(h.
+00006880: 5d68 145d 6815 5d68 165d 6817 5d75 681f  ]h.]h.]h.]h.]uh.
+00006890: 6ac0 0400 0068 185d 72d2 0400 0028 6a48  j....h.]r....(jH
+000068a0: 0200 0029 8172 d304 0000 7d72 d404 0000  ...).r....}r....
+000068b0: 2868 1055 0068 117d 72d5 0400 0028 6813  (h.U.h.}r....(h.
+000068c0: 5d68 145d 6815 5d68 165d 6817 5d75 681f  ]h.]h.]h.]h.]uh.
+000068d0: 6acf 0400 0068 185d 72d6 0400 006a 4d02  j....h.]r....jM.
+000068e0: 0000 2981 72d7 0400 007d 72d8 0400 0028  ..).r....}r....(
+000068f0: 6810 5500 6811 7d72 d904 0000 2868 135d  h.U.h.}r....(h.]
+00006900: 6814 5d68 155d 6816 5d68 175d 7568 1f6a  h.]h.]h.]h.]uh.j
+00006910: d304 0000 6818 5d72 da04 0000 6a52 0200  ....h.]r....jR..
+00006920: 0029 8172 db04 0000 7d72 dc04 0000 2868  .).r....}r....(h
+00006930: 1055 0068 117d 72dd 0400 0028 550a 616e  .U.h.}r....(U.an
+00006940: 6368 6f72 6e61 6d65 550c 2374 6865 2d70  chornameU.#the-p
+00006950: 726f 626c 656d 5506 7265 6675 7269 684f  roblemU.refurihO
+00006960: 6816 5d68 155d 6813 5d68 145d 6817 5d55  h.]h.]h.]h.]h.]U
+00006970: 0869 6e74 6572 6e61 6c88 7568 1f6a d704  .internal.uh.j..
+00006980: 0000 6818 5d72 de04 0000 681a 580b 0000  ..h.]r....h.X...
+00006990: 0054 6865 2050 726f 626c 656d 72df 0400  .The Problemr...
+000069a0: 0085 8172 e004 0000 7d72 e104 0000 2868  ...r....}r....(h
+000069b0: 1058 0b00 0000 5468 6520 5072 6f62 6c65  .X....The Proble
+000069c0: 6d68 1f6a db04 0000 7562 6168 206a 5a02  mh.j....ubah jZ.
+000069d0: 0000 7562 6168 206a 5b02 0000 7562 6168  ..ubah j[...ubah
+000069e0: 206a 7202 0000 7562 6a48 0200 0029 8172   jr...ubjH...).r
+000069f0: e204 0000 7d72 e304 0000 2868 1055 0068  ....}r....(h.U.h
+00006a00: 117d 72e4 0400 0028 6813 5d68 145d 6815  .}r....(h.]h.]h.
+00006a10: 5d68 165d 6817 5d75 681f 6acf 0400 0068  ]h.]h.]uh.j....h
+00006a20: 185d 72e5 0400 006a 4d02 0000 2981 72e6  .]r....jM...).r.
+00006a30: 0400 007d 72e7 0400 0028 6810 5500 6811  ...}r....(h.U.h.
+00006a40: 7d72 e804 0000 2868 135d 6814 5d68 155d  }r....(h.]h.]h.]
+00006a50: 6816 5d68 175d 7568 1f6a e204 0000 6818  h.]h.]uh.j....h.
+00006a60: 5d72 e904 0000 6a52 0200 0029 8172 ea04  ]r....jR...).r..
+00006a70: 0000 7d72 eb04 0000 2868 1055 0068 117d  ..}r....(h.U.h.}
+00006a80: 72ec 0400 0028 550a 616e 6368 6f72 6e61  r....(U.anchorna
+00006a90: 6d65 550b 2361 2d73 6f6c 7574 696f 6e55  meU.#a-solutionU
+00006aa0: 0672 6566 7572 6968 4f68 165d 6815 5d68  .refurihOh.]h.]h
+00006ab0: 135d 6814 5d68 175d 5508 696e 7465 726e  .]h.]h.]U.intern
+00006ac0: 616c 8875 681f 6ae6 0400 0068 185d 72ed  al.uh.j....h.]r.
+00006ad0: 0400 0068 1a58 0a00 0000 4120 536f 6c75  ...h.X....A Solu
+00006ae0: 7469 6f6e 72ee 0400 0085 8172 ef04 0000  tionr......r....
+00006af0: 7d72 f004 0000 2868 1058 0a00 0000 4120  }r....(h.X....A 
+00006b00: 536f 6c75 7469 6f6e 681f 6aea 0400 0075  Solutionh.j....u
+00006b10: 6261 6820 6a5a 0200 0075 6261 6820 6a5b  bah jZ...ubah j[
+00006b20: 0200 0075 6261 6820 6a72 0200 0075 626a  ...ubah jr...ubj
+00006b30: 4802 0000 2981 72f1 0400 007d 72f2 0400  H...).r....}r...
+00006b40: 0028 6810 5500 6811 7d72 f304 0000 2868  .(h.U.h.}r....(h
+00006b50: 135d 6814 5d68 155d 6816 5d68 175d 7568  .]h.]h.]h.]h.]uh
+00006b60: 1f6a cf04 0000 6818 5d72 f404 0000 6a4d  .j....h.]r....jM
+00006b70: 0200 0029 8172 f504 0000 7d72 f604 0000  ...).r....}r....
+00006b80: 2868 1055 0068 117d 72f7 0400 0028 6813  (h.U.h.}r....(h.
+00006b90: 5d68 145d 6815 5d68 165d 6817 5d75 681f  ]h.]h.]h.]h.]uh.
+00006ba0: 6af1 0400 0068 185d 72f8 0400 006a 5202  j....h.]r....jR.
+00006bb0: 0000 2981 72f9 0400 007d 72fa 0400 0028  ..).r....}r....(
+00006bc0: 6810 5500 6811 7d72 fb04 0000 2855 0a61  h.U.h.}r....(U.a
+00006bd0: 6e63 686f 726e 616d 6555 0c23 612d 7661  nchornameU.#a-va
+00006be0: 7269 6174 696f 6e55 0672 6566 7572 6968  riationU.refurih
+00006bf0: 4f68 165d 6815 5d68 135d 6814 5d68 175d  Oh.]h.]h.]h.]h.]
+00006c00: 5508 696e 7465 726e 616c 8875 681f 6af5  U.internal.uh.j.
+00006c10: 0400 0068 185d 72fc 0400 0068 1a58 0b00  ...h.]r....h.X..
+00006c20: 0000 4120 5661 7269 6174 696f 6e72 fd04  ..A Variationr..
+00006c30: 0000 8581 72fe 0400 007d 72ff 0400 0028  ....r....}r....(
+00006c40: 6810 580b 0000 0041 2056 6172 6961 7469  h.X....A Variati
+00006c50: 6f6e 681f 6af9 0400 0075 6261 6820 6a5a  onh.j....ubah jZ
+00006c60: 0200 0075 6261 6820 6a5b 0200 0075 6261  ...ubah j[...uba
+00006c70: 6820 6a72 0200 0075 6265 6820 6a71 0200  h jr...ubeh jq..
+00006c80: 0075 6265 6820 6a72 0200 0075 6261 6820  .ubeh jr...ubah 
+00006c90: 6a71 0200 0075 6268 586a 4302 0000 2981  jq...ubhXjC...).
+00006ca0: 7200 0500 007d 7201 0500 0028 6810 5500  r....}r....(h.U.
+00006cb0: 6811 7d72 0205 0000 2868 135d 6814 5d68  h.}r....(h.]h.]h
+00006cc0: 155d 6816 5d68 175d 7568 185d 7203 0500  .]h.]h.]uh.]r...
+00006cd0: 006a 4802 0000 2981 7204 0500 007d 7205  .jH...).r....}r.
+00006ce0: 0500 0028 6810 5500 6811 7d72 0605 0000  ...(h.U.h.}r....
+00006cf0: 2868 135d 6814 5d68 155d 6816 5d68 175d  (h.]h.]h.]h.]h.]
+00006d00: 7568 1f6a 0005 0000 6818 5d72 0705 0000  uh.j....h.]r....
+00006d10: 286a 4d02 0000 2981 7208 0500 007d 7209  (jM...).r....}r.
+00006d20: 0500 0028 6810 5500 6811 7d72 0a05 0000  ...(h.U.h.}r....
+00006d30: 2868 135d 6814 5d68 155d 6816 5d68 175d  (h.]h.]h.]h.]h.]
+00006d40: 7568 1f6a 0405 0000 6818 5d72 0b05 0000  uh.j....h.]r....
+00006d50: 6a52 0200 0029 8172 0c05 0000 7d72 0d05  jR...).r....}r..
+00006d60: 0000 2868 1055 0068 117d 720e 0500 0028  ..(h.U.h.}r....(
+00006d70: 550a 616e 6368 6f72 6e61 6d65 5500 5506  U.anchornameU.U.
+00006d80: 7265 6675 7269 6858 6816 5d68 155d 6813  refurihXh.]h.]h.
+00006d90: 5d68 145d 6817 5d55 0869 6e74 6572 6e61  ]h.]h.]U.interna
+00006da0: 6c88 7568 1f6a 0805 0000 6818 5d72 0f05  l.uh.j....h.]r..
+00006db0: 0000 2868 3029 8172 1005 0000 7d72 1105  ..(h0).r....}r..
+00006dc0: 0000 2868 1058 0500 0000 7363 6970 7968  ..(h.X....scipyh
+00006dd0: 117d 7212 0500 0028 6813 5d68 145d 6815  .}r....(h.]h.]h.
+00006de0: 5d68 165d 6817 5d75 681f 6a0c 0500 0068  ]h.]h.]uh.j....h
+00006df0: 185d 7213 0500 0068 1a58 0500 0000 7363  .]r....h.X....sc
+00006e00: 6970 7972 1405 0000 8581 7215 0500 007d  ipyr......r....}
+00006e10: 7216 0500 0028 6810 5500 681f 6a10 0500  r....(h.U.h.j...
+00006e20: 0075 6261 6820 6838 7562 681a 5809 0000  .ubah h8ubh.X...
+00006e30: 0020 526f 7574 696e 6573 7217 0500 0085  . Routinesr.....
+00006e40: 8172 1805 0000 7d72 1905 0000 2868 1068  .r....}r....(h.h
+00006e50: 6768 1f6a 0c05 0000 7562 6568 206a 5a02  gh.j....ubeh jZ.
+00006e60: 0000 7562 6168 206a 5b02 0000 7562 6a43  ..ubah j[...ubjC
+00006e70: 0200 0029 8172 1a05 0000 7d72 1b05 0000  ...).r....}r....
+00006e80: 2868 1055 0068 117d 721c 0500 0028 6813  (h.U.h.}r....(h.
+00006e90: 5d68 145d 6815 5d68 165d 6817 5d75 681f  ]h.]h.]h.]h.]uh.
+00006ea0: 6a04 0500 0068 185d 721d 0500 0028 6a48  j....h.]r....(jH
+00006eb0: 0200 0029 8172 1e05 0000 7d72 1f05 0000  ...).r....}r....
+00006ec0: 2868 1055 0068 117d 7220 0500 0028 6813  (h.U.h.}r ...(h.
+00006ed0: 5d68 145d 6815 5d68 165d 6817 5d75 681f  ]h.]h.]h.]h.]uh.
+00006ee0: 6a1a 0500 0068 185d 7221 0500 006a 4d02  j....h.]r!...jM.
+00006ef0: 0000 2981 7222 0500 007d 7223 0500 0028  ..).r"...}r#...(
+00006f00: 6810 5500 6811 7d72 2405 0000 2868 135d  h.U.h.}r$...(h.]
+00006f10: 6814 5d68 155d 6816 5d68 175d 7568 1f6a  h.]h.]h.]h.]uh.j
+00006f20: 1e05 0000 6818 5d72 2505 0000 6a52 0200  ....h.]r%...jR..
+00006f30: 0029 8172 2605 0000 7d72 2705 0000 2868  .).r&...}r'...(h
+00006f40: 1055 0068 117d 7228 0500 0028 550a 616e  .U.h.}r(...(U.an
+00006f50: 6368 6f72 6e61 6d65 5507 2366 6974 7465  chornameU.#fitte
+00006f60: 7255 0672 6566 7572 6968 5868 165d 6815  rU.refurihXh.]h.
+00006f70: 5d68 135d 6814 5d68 175d 5508 696e 7465  ]h.]h.]h.]U.inte
+00006f80: 726e 616c 8875 681f 6a22 0500 0068 185d  rnal.uh.j"...h.]
+00006f90: 7229 0500 0068 1a58 0600 0000 4669 7474  r)...h.X....Fitt
+00006fa0: 6572 722a 0500 0085 8172 2b05 0000 7d72  err*.....r+...}r
+00006fb0: 2c05 0000 2868 1058 0600 0000 4669 7474  ,...(h.X....Fitt
+00006fc0: 6572 722d 0500 0068 1f6a 2605 0000 7562  err-...h.j&...ub
+00006fd0: 6168 206a 5a02 0000 7562 6168 206a 5b02  ah jZ...ubah j[.
+00006fe0: 0000 7562 6168 206a 7202 0000 7562 6a48  ..ubah jr...ubjH
+00006ff0: 0200 0029 8172 2e05 0000 7d72 2f05 0000  ...).r....}r/...
+00007000: 2868 1055 0068 117d 7230 0500 0028 6813  (h.U.h.}r0...(h.
+00007010: 5d68 145d 6815 5d68 165d 6817 5d75 681f  ]h.]h.]h.]h.]uh.
+00007020: 6a1a 0500 0068 185d 7231 0500 006a 4d02  j....h.]r1...jM.
+00007030: 0000 2981 7232 0500 007d 7233 0500 0028  ..).r2...}r3...(
+00007040: 6810 5500 6811 7d72 3405 0000 2868 135d  h.U.h.}r4...(h.]
+00007050: 6814 5d68 155d 6816 5d68 175d 7568 1f6a  h.]h.]h.]h.]uh.j
+00007060: 2e05 0000 6818 5d72 3505 0000 6a52 0200  ....h.]r5...jR..
+00007070: 0029 8172 3605 0000 7d72 3705 0000 2868  .).r6...}r7...(h
+00007080: 1055 0068 117d 7238 0500 0028 550a 616e  .U.h.}r8...(U.an
+00007090: 6368 6f72 6e61 6d65 550a 236d 696e 696d  chornameU.#minim
+000070a0: 697a 6572 5506 7265 6675 7269 6858 6816  izerU.refurihXh.
+000070b0: 5d68 155d 6813 5d68 145d 6817 5d55 0869  ]h.]h.]h.]h.]U.i
+000070c0: 6e74 6572 6e61 6c88 7568 1f6a 3205 0000  nternal.uh.j2...
+000070d0: 6818 5d72 3905 0000 681a 5809 0000 004d  h.]r9...h.X....M
+000070e0: 696e 696d 697a 6572 723a 0500 0085 8172  inimizerr:.....r
+000070f0: 3b05 0000 7d72 3c05 0000 2868 1058 0900  ;...}r<...(h.X..
+00007100: 0000 4d69 6e69 6d69 7a65 7272 3d05 0000  ..Minimizerr=...
+00007110: 681f 6a36 0500 0075 6261 6820 6a5a 0200  h.j6...ubah jZ..
+00007120: 0075 6261 6820 6a5b 0200 0075 6261 6820  .ubah j[...ubah 
+00007130: 6a72 0200 0075 6265 6820 6a71 0200 0075  jr...ubeh jq...u
+00007140: 6265 6820 6a72 0200 0075 6261 6820 6a71  beh jr...ubah jq
+00007150: 0200 0075 6268 686a 4302 0000 2981 723e  ...ubhhjC...).r>
+00007160: 0500 007d 723f 0500 0028 6810 5500 6811  ...}r?...(h.U.h.
+00007170: 7d72 4005 0000 2868 135d 6814 5d68 155d  }r@...(h.]h.]h.]
+00007180: 6816 5d68 175d 7568 185d 7241 0500 006a  h.]h.]uh.]rA...j
+00007190: 4802 0000 2981 7242 0500 007d 7243 0500  H...).rB...}rC..
+000071a0: 0028 6810 5500 6811 7d72 4405 0000 2868  .(h.U.h.}rD...(h
+000071b0: 135d 6814 5d68 155d 6816 5d68 175d 7568  .]h.]h.]h.]h.]uh
+000071c0: 1f6a 3e05 0000 6818 5d72 4505 0000 286a  .j>...h.]rE...(j
+000071d0: 4d02 0000 2981 7246 0500 007d 7247 0500  M...).rF...}rG..
+000071e0: 0028 6810 5500 6811 7d72 4805 0000 2868  .(h.U.h.}rH...(h
+000071f0: 135d 6814 5d68 155d 6816 5d68 175d 7568  .]h.]h.]h.]h.]uh
+00007200: 1f6a 4205 0000 6818 5d72 4905 0000 6a52  .jB...h.]rI...jR
+00007210: 0200 0029 8172 4a05 0000 7d72 4b05 0000  ...).rJ...}rK...
+00007220: 2868 1055 0068 117d 724c 0500 0028 550a  (h.U.h.}rL...(U.
+00007230: 616e 6368 6f72 6e61 6d65 5500 5506 7265  anchornameU.U.re
+00007240: 6675 7269 6868 6816 5d68 155d 6813 5d68  furihhh.]h.]h.]h
+00007250: 145d 6817 5d55 0869 6e74 6572 6e61 6c88  .]h.]U.internal.
+00007260: 7568 1f6a 4605 0000 6818 5d72 4d05 0000  uh.jF...h.]rM...
+00007270: 681a 5814 0000 0043 6173 6520 5374 7564  h.X....Case Stud
+00007280: 793a 2050 656e 6475 6c75 6d72 4e05 0000  y: PendulumrN...
+00007290: 8581 724f 0500 007d 7250 0500 0028 6810  ..rO...}rP...(h.
+000072a0: 6870 681f 6a4a 0500 0075 6261 6820 6a5a  hph.jJ...ubah jZ
+000072b0: 0200 0075 6261 6820 6a5b 0200 0075 626a  ...ubah j[...ubj
+000072c0: 4302 0000 2981 7251 0500 007d 7252 0500  C...).rQ...}rR..
+000072d0: 0028 6810 5500 6811 7d72 5305 0000 2868  .(h.U.h.}rS...(h
+000072e0: 135d 6814 5d68 155d 6816 5d68 175d 7568  .]h.]h.]h.]h.]uh
+000072f0: 1f6a 4205 0000 6818 5d72 5405 0000 286a  .jB...h.]rT...(j
+00007300: 4802 0000 2981 7255 0500 007d 7256 0500  H...).rU...}rV..
+00007310: 0028 6810 5500 6811 7d72 5705 0000 2868  .(h.U.h.}rW...(h
+00007320: 135d 6814 5d68 155d 6816 5d68 175d 7568  .]h.]h.]h.]h.]uh
+00007330: 1f6a 5105 0000 6818 5d72 5805 0000 6a4d  .jQ...h.]rX...jM
+00007340: 0200 0029 8172 5905 0000 7d72 5a05 0000  ...).rY...}rZ...
+00007350: 2868 1055 0068 117d 725b 0500 0028 6813  (h.U.h.}r[...(h.
+00007360: 5d68 145d 6815 5d68 165d 6817 5d75 681f  ]h.]h.]h.]h.]uh.
+00007370: 6a55 0500 0068 185d 725c 0500 006a 5202  jU...h.]r\...jR.
+00007380: 0000 2981 725d 0500 007d 725e 0500 0028  ..).r]...}r^...(
+00007390: 6810 5500 6811 7d72 5f05 0000 2855 0a61  h.U.h.}r_...(U.a
+000073a0: 6e63 686f 726e 616d 6555 0c23 7468 652d  nchornameU.#the-
+000073b0: 7072 6f62 6c65 6d55 0672 6566 7572 6968  problemU.refurih
+000073c0: 6868 165d 6815 5d68 135d 6814 5d68 175d  hh.]h.]h.]h.]h.]
+000073d0: 5508 696e 7465 726e 616c 8875 681f 6a59  U.internal.uh.jY
+000073e0: 0500 0068 185d 7260 0500 0068 1a58 0b00  ...h.]r`...h.X..
+000073f0: 0000 5468 6520 5072 6f62 6c65 6d72 6105  ..The Problemra.
+00007400: 0000 8581 7262 0500 007d 7263 0500 0028  ....rb...}rc...(
+00007410: 6810 580b 0000 0054 6865 2050 726f 626c  h.X....The Probl
+00007420: 656d 681f 6a5d 0500 0075 6261 6820 6a5a  emh.j]...ubah jZ
+00007430: 0200 0075 6261 6820 6a5b 0200 0075 6261  ...ubah j[...uba
+00007440: 6820 6a72 0200 0075 626a 4802 0000 2981  h jr...ubjH...).
+00007450: 7264 0500 007d 7265 0500 0028 6810 5500  rd...}re...(h.U.
+00007460: 6811 7d72 6605 0000 2868 135d 6814 5d68  h.}rf...(h.]h.]h
+00007470: 155d 6816 5d68 175d 7568 1f6a 5105 0000  .]h.]h.]uh.jQ...
+00007480: 6818 5d72 6705 0000 6a4d 0200 0029 8172  h.]rg...jM...).r
+00007490: 6805 0000 7d72 6905 0000 2868 1055 0068  h...}ri...(h.U.h
+000074a0: 117d 726a 0500 0028 6813 5d68 145d 6815  .}rj...(h.]h.]h.
+000074b0: 5d68 165d 6817 5d75 681f 6a64 0500 0068  ]h.]h.]uh.jd...h
+000074c0: 185d 726b 0500 006a 5202 0000 2981 726c  .]rk...jR...).rl
+000074d0: 0500 007d 726d 0500 0028 6810 5500 6811  ...}rm...(h.U.h.
+000074e0: 7d72 6e05 0000 2855 0a61 6e63 686f 726e  }rn...(U.anchorn
+000074f0: 616d 6555 1223 7065 6e64 756c 756d 2d64  ameU.#pendulum-d
+00007500: 796e 616d 6963 7355 0672 6566 7572 6968  ynamicsU.refurih
+00007510: 6868 165d 6815 5d68 135d 6814 5d68 175d  hh.]h.]h.]h.]h.]
+00007520: 5508 696e 7465 726e 616c 8875 681f 6a68  U.internal.uh.jh
+00007530: 0500 0068 185d 726f 0500 0068 1a58 1100  ...h.]ro...h.X..
+00007540: 0000 5065 6e64 756c 756d 2044 796e 616d  ..Pendulum Dynam
+00007550: 6963 7372 7005 0000 8581 7271 0500 007d  icsrp.....rq...}
+00007560: 7272 0500 0028 6810 5811 0000 0050 656e  rr...(h.X....Pen
+00007570: 6475 6c75 6d20 4479 6e61 6d69 6373 681f  dulum Dynamicsh.
+00007580: 6a6c 0500 0075 6261 6820 6a5a 0200 0075  jl...ubah jZ...u
+00007590: 6261 6820 6a5b 0200 0075 6261 6820 6a72  bah j[...ubah jr
+000075a0: 0200 0075 626a 4802 0000 2981 7273 0500  ...ubjH...).rs..
+000075b0: 007d 7274 0500 0028 6810 5500 6811 7d72  .}rt...(h.U.h.}r
+000075c0: 7505 0000 2868 135d 6814 5d68 155d 6816  u...(h.]h.]h.]h.
+000075d0: 5d68 175d 7568 1f6a 5105 0000 6818 5d72  ]h.]uh.jQ...h.]r
+000075e0: 7605 0000 6a4d 0200 0029 8172 7705 0000  v...jM...).rw...
+000075f0: 7d72 7805 0000 2868 1055 0068 117d 7279  }rx...(h.U.h.}ry
+00007600: 0500 0028 6813 5d68 145d 6815 5d68 165d  ...(h.]h.]h.]h.]
+00007610: 6817 5d75 681f 6a73 0500 0068 185d 727a  h.]uh.js...h.]rz
+00007620: 0500 006a 5202 0000 2981 727b 0500 007d  ...jR...).r{...}
+00007630: 727c 0500 0028 6810 5500 6811 7d72 7d05  r|...(h.U.h.}r}.
+00007640: 0000 2855 0a61 6e63 686f 726e 616d 6555  ..(U.anchornameU
+00007650: 1823 7477 6f2d 7479 7065 732d 6f66 2d69  .#two-types-of-i
+00007660: 6e70 7574 2d64 6174 6155 0672 6566 7572  nput-dataU.refur
+00007670: 6968 6868 165d 6815 5d68 135d 6814 5d68  ihhh.]h.]h.]h.]h
+00007680: 175d 5508 696e 7465 726e 616c 8875 681f  .]U.internal.uh.
+00007690: 6a77 0500 0068 185d 727e 0500 0068 1a58  jw...h.]r~...h.X
+000076a0: 1700 0000 5477 6f20 5479 7065 7320 6f66  ....Two Types of
+000076b0: 2049 6e70 7574 2044 6174 6172 7f05 0000   Input Datar....
+000076c0: 8581 7280 0500 007d 7281 0500 0028 6810  ..r....}r....(h.
+000076d0: 5817 0000 0054 776f 2054 7970 6573 206f  X....Two Types o
+000076e0: 6620 496e 7075 7420 4461 7461 681f 6a7b  f Input Datah.j{
+000076f0: 0500 0075 6261 6820 6a5a 0200 0075 6261  ...ubah jZ...uba
+00007700: 6820 6a5b 0200 0075 6261 6820 6a72 0200  h j[...ubah jr..
+00007710: 0075 6265 6820 6a71 0200 0075 6265 6820  .ubeh jq...ubeh 
+00007720: 6a72 0200 0075 6261 6820 6a71 0200 0075  jr...ubah jq...u
+00007730: 6268 716a 4302 0000 2981 7282 0500 007d  bhqjC...).r....}
+00007740: 7283 0500 0028 6810 5500 6811 7d72 8405  r....(h.U.h.}r..
+00007750: 0000 2868 135d 6814 5d68 155d 6816 5d68  ..(h.]h.]h.]h.]h
+00007760: 175d 7568 185d 7285 0500 006a 4802 0000  .]uh.]r....jH...
+00007770: 2981 7286 0500 007d 7287 0500 0028 6810  ).r....}r....(h.
+00007780: 5500 6811 7d72 8805 0000 2868 135d 6814  U.h.}r....(h.]h.
+00007790: 5d68 155d 6816 5d68 175d 7568 1f6a 8205  ]h.]h.]h.]uh.j..
+000077a0: 0000 6818 5d72 8905 0000 286a 4d02 0000  ..h.]r....(jM...
+000077b0: 2981 728a 0500 007d 728b 0500 0028 6810  ).r....}r....(h.
+000077c0: 5500 6811 7d72 8c05 0000 2868 135d 6814  U.h.}r....(h.]h.
+000077d0: 5d68 155d 6816 5d68 175d 7568 1f6a 8605  ]h.]h.]h.]uh.j..
+000077e0: 0000 6818 5d72 8d05 0000 6a52 0200 0029  ..h.]r....jR...)
+000077f0: 8172 8e05 0000 7d72 8f05 0000 2868 1055  .r....}r....(h.U
+00007800: 0068 117d 7290 0500 0028 550a 616e 6368  .h.}r....(U.anch
+00007810: 6f72 6e61 6d65 5500 5506 7265 6675 7269  ornameU.U.refuri
+00007820: 6871 6816 5d68 155d 6813 5d68 145d 6817  hqh.]h.]h.]h.]h.
+00007830: 5d55 0869 6e74 6572 6e61 6c88 7568 1f6a  ]U.internal.uh.j
+00007840: 8a05 0000 6818 5d72 9105 0000 681a 580c  ....h.]r....h.X.
+00007850: 0000 0047 534c 2052 6f75 7469 6e65 7372  ...GSL Routinesr
+00007860: 9205 0000 8581 7293 0500 007d 7294 0500  ......r....}r...
+00007870: 0028 6810 6879 681f 6a8e 0500 0075 6261  .(h.hyh.j....uba
+00007880: 6820 6a5a 0200 0075 6261 6820 6a5b 0200  h jZ...ubah j[..
+00007890: 0075 626a 4302 0000 2981 7295 0500 007d  .ubjC...).r....}
+000078a0: 7296 0500 0028 6810 5500 6811 7d72 9705  r....(h.U.h.}r..
+000078b0: 0000 2868 135d 6814 5d68 155d 6816 5d68  ..(h.]h.]h.]h.]h
+000078c0: 175d 7568 1f6a 8605 0000 6818 5d72 9805  .]uh.j....h.]r..
+000078d0: 0000 286a 4802 0000 2981 7299 0500 007d  ..(jH...).r....}
+000078e0: 729a 0500 0028 6810 5500 6811 7d72 9b05  r....(h.U.h.}r..
+000078f0: 0000 2868 135d 6814 5d68 155d 6816 5d68  ..(h.]h.]h.]h.]h
+00007900: 175d 7568 1f6a 9505 0000 6818 5d72 9c05  .]uh.j....h.]r..
+00007910: 0000 6a4d 0200 0029 8172 9d05 0000 7d72  ..jM...).r....}r
+00007920: 9e05 0000 2868 1055 0068 117d 729f 0500  ....(h.U.h.}r...
+00007930: 0028 6813 5d68 145d 6815 5d68 165d 6817  .(h.]h.]h.]h.]h.
+00007940: 5d75 681f 6a99 0500 0068 185d 72a0 0500  ]uh.j....h.]r...
+00007950: 006a 5202 0000 2981 72a1 0500 007d 72a2  .jR...).r....}r.
+00007960: 0500 0028 6810 5500 6811 7d72 a305 0000  ...(h.U.h.}r....
+00007970: 2855 0a61 6e63 686f 726e 616d 6555 0823  (U.anchornameU.#
+00007980: 6669 7474 6572 7355 0672 6566 7572 6968  fittersU.refurih
+00007990: 7168 165d 6815 5d68 135d 6814 5d68 175d  qh.]h.]h.]h.]h.]
+000079a0: 5508 696e 7465 726e 616c 8875 681f 6a9d  U.internal.uh.j.
+000079b0: 0500 0068 185d 72a4 0500 0068 1a58 0700  ...h.]r....h.X..
+000079c0: 0000 4669 7474 6572 7372 a505 0000 8581  ..Fittersr......
+000079d0: 72a6 0500 007d 72a7 0500 0028 6810 5807  r....}r....(h.X.
+000079e0: 0000 0046 6974 7465 7273 681f 6aa1 0500  ...Fittersh.j...
+000079f0: 0075 6261 6820 6a5a 0200 0075 6261 6820  .ubah jZ...ubah 
+00007a00: 6a5b 0200 0075 6261 6820 6a72 0200 0075  j[...ubah jr...u
+00007a10: 626a 4802 0000 2981 72a8 0500 007d 72a9  bjH...).r....}r.
+00007a20: 0500 0028 6810 5500 6811 7d72 aa05 0000  ...(h.U.h.}r....
+00007a30: 2868 135d 6814 5d68 155d 6816 5d68 175d  (h.]h.]h.]h.]h.]
+00007a40: 7568 1f6a 9505 0000 6818 5d72 ab05 0000  uh.j....h.]r....
+00007a50: 6a4d 0200 0029 8172 ac05 0000 7d72 ad05  jM...).r....}r..
+00007a60: 0000 2868 1055 0068 117d 72ae 0500 0028  ..(h.U.h.}r....(
+00007a70: 6813 5d68 145d 6815 5d68 165d 6817 5d75  h.]h.]h.]h.]h.]u
+00007a80: 681f 6aa8 0500 0068 185d 72af 0500 006a  h.j....h.]r....j
+00007a90: 5202 0000 2981 72b0 0500 007d 72b1 0500  R...).r....}r...
+00007aa0: 0028 6810 5500 6811 7d72 b205 0000 2855  .(h.U.h.}r....(U
+00007ab0: 0a61 6e63 686f 726e 616d 6555 0a23 6d69  .anchornameU.#mi
+00007ac0: 6e69 6d69 7a65 7255 0672 6566 7572 6968  nimizerU.refurih
+00007ad0: 7168 165d 6815 5d68 135d 6814 5d68 175d  qh.]h.]h.]h.]h.]
+00007ae0: 5508 696e 7465 726e 616c 8875 681f 6aac  U.internal.uh.j.
+00007af0: 0500 0068 185d 72b3 0500 0068 1a58 0900  ...h.]r....h.X..
+00007b00: 0000 4d69 6e69 6d69 7a65 7272 b405 0000  ..Minimizerr....
+00007b10: 8581 72b5 0500 007d 72b6 0500 0028 6810  ..r....}r....(h.
+00007b20: 5809 0000 004d 696e 696d 697a 6572 681f  X....Minimizerh.
+00007b30: 6ab0 0500 0075 6261 6820 6a5a 0200 0075  j....ubah jZ...u
+00007b40: 6261 6820 6a5b 0200 0075 6261 6820 6a72  bah j[...ubah jr
+00007b50: 0200 0075 6265 6820 6a71 0200 0075 6265  ...ubeh jq...ube
+00007b60: 6820 6a72 0200 0075 6261 6820 6a71 0200  h jr...ubah jq..
+00007b70: 0075 6275 550c 696e 6465 7865 6e74 7269  .ubuU.indexentri
+00007b80: 6573 72b7 0500 007d 72b8 0500 0028 680c  esr....}r....(h.
+00007b90: 5d68 225d 682b 5d72 b905 0000 2828 5506  ]h"]h+]r....((U.
+00007ba0: 7369 6e67 6c65 72ba 0500 0058 0f00 0000  singler....X....
+00007bb0: 6c73 7166 6974 2028 6d6f 6475 6c65 2958  lsqfit (module)X
+00007bc0: 0d00 0000 6d6f 6475 6c65 2d6c 7371 6669  ....module-lsqfi
+00007bd0: 7455 004e 7472 bb05 0000 286a ba05 0000  tU.Ntr....(j....
+00007be0: 581f 0000 006e 6f6e 6c69 6e65 6172 5f66  X....nonlinear_f
+00007bf0: 6974 2028 636c 6173 7320 696e 206c 7371  it (class in lsq
+00007c00: 6669 7429 68cc 5500 4e74 72bc 0500 0028  fit)h.U.Ntr....(
+00007c10: 6aba 0500 0058 2500 0000 6368 6932 2028  j....X%...chi2 (
+00007c20: 6c73 7166 6974 2e6e 6f6e 6c69 6e65 6172  lsqfit.nonlinear
+00007c30: 5f66 6974 2061 7474 7269 6275 7465 2968  _fit attribute)h
+00007c40: d455 004e 7472 bd05 0000 286a ba05 0000  .U.Ntr....(j....
+00007c50: 5824 0000 0063 6f76 2028 6c73 7166 6974  X$...cov (lsqfit
+00007c60: 2e6e 6f6e 6c69 6e65 6172 5f66 6974 2061  .nonlinear_fit a
+00007c70: 7474 7269 6275 7465 2968 bc55 004e 7472  ttribute)h.U.Ntr
+00007c80: be05 0000 286a ba05 0000 5824 0000 0064  ....(j....X$...d
+00007c90: 6f66 2028 6c73 7166 6974 2e6e 6f6e 6c69  of (lsqfit.nonli
+00007ca0: 6e65 6172 5f66 6974 2061 7474 7269 6275  near_fit attribu
+00007cb0: 7465 2968 ed55 004e 7472 bf05 0000 286a  te)h.U.Ntr....(j
+00007cc0: ba05 0000 5826 0000 0065 7272 6f72 2028  ....X&...error (
+00007cd0: 6c73 7166 6974 2e6e 6f6e 6c69 6e65 6172  lsqfit.nonlinear
+00007ce0: 5f66 6974 2061 7474 7269 6275 7465 296a  _fit attribute)j
+00007cf0: 0301 0000 5500 4e74 72c0 0500 0028 6aba  ....U.Ntr....(j.
+00007d00: 0500 0058 2f00 0000 6669 7474 6572 5f72  ...X/...fitter_r
+00007d10: 6573 756c 7473 2028 6c73 7166 6974 2e6e  esults (lsqfit.n
+00007d20: 6f6e 6c69 6e65 6172 5f66 6974 2061 7474  onlinear_fit att
+00007d30: 7269 6275 7465 296a 1a01 0000 5500 4e74  ribute)j....U.Nt
+00007d40: 72c1 0500 0028 6aba 0500 0058 2700 0000  r....(j....X'...
+00007d50: 6c6f 6747 4246 2028 6c73 7166 6974 2e6e  logGBF (lsqfit.n
+00007d60: 6f6e 6c69 6e65 6172 5f66 6974 2061 7474  onlinear_fit att
+00007d70: 7269 6275 7465 2968 f555 004e 7472 c205  ribute)h.U.Ntr..
+00007d80: 0000 286a ba05 0000 5822 0000 0070 2028  ..(j....X"...p (
+00007d90: 6c73 7166 6974 2e6e 6f6e 6c69 6e65 6172  lsqfit.nonlinear
+00007da0: 5f66 6974 2061 7474 7269 6275 7465 296a  _fit attribute)j
+00007db0: 2e01 0000 5500 4e74 72c3 0500 0028 6aba  ....U.Ntr....(j.
+00007dc0: 0500 0058 2600 0000 706d 6561 6e20 286c  ...X&...pmean (l
+00007dd0: 7371 6669 742e 6e6f 6e6c 696e 6561 725f  sqfit.nonlinear_
+00007de0: 6669 7420 6174 7472 6962 7574 6529 68e7  fit attribute)h.
+00007df0: 5500 4e74 72c4 0500 0028 6aba 0500 0058  U.Ntr....(j....X
+00007e00: 2600 0000 7073 6465 7620 286c 7371 6669  &...psdev (lsqfi
+00007e10: 742e 6e6f 6e6c 696e 6561 725f 6669 7420  t.nonlinear_fit 
+00007e20: 6174 7472 6962 7574 6529 6a38 0100 0055  attribute)j8...U
+00007e30: 004e 7472 c505 0000 286a ba05 0000 5825  .Ntr....(j....X%
+00007e40: 0000 0070 616c 7420 286c 7371 6669 742e  ...palt (lsqfit.
+00007e50: 6e6f 6e6c 696e 6561 725f 6669 7420 6174  nonlinear_fit at
+00007e60: 7472 6962 7574 6529 68e2 5500 4e74 72c6  tribute)h.U.Ntr.
+00007e70: 0500 0028 6aba 0500 0058 2300 0000 7030  ...(j....X#...p0
+00007e80: 2028 6c73 7166 6974 2e6e 6f6e 6c69 6e65   (lsqfit.nonline
+00007e90: 6172 5f66 6974 2061 7474 7269 6275 7465  ar_fit attribute
+00007ea0: 2968 fd55 004e 7472 c705 0000 286a ba05  )h.U.Ntr....(j..
+00007eb0: 0000 5826 0000 0070 7269 6f72 2028 6c73  ..X&...prior (ls
+00007ec0: 7166 6974 2e6e 6f6e 6c69 6e65 6172 5f66  qfit.nonlinear_f
+00007ed0: 6974 2061 7474 7269 6275 7465 2968 e955  it attribute)h.U
+00007ee0: 004e 7472 c805 0000 286a ba05 0000 5822  .Ntr....(j....X"
+00007ef0: 0000 0051 2028 6c73 7166 6974 2e6e 6f6e  ...Q (lsqfit.non
+00007f00: 6c69 6e65 6172 5f66 6974 2061 7474 7269  linear_fit attri
+00007f10: 6275 7465 296a 0501 0000 5500 4e74 72c9  bute)j....U.Ntr.
+00007f20: 0500 0028 6aba 0500 0058 3300 0000 7374  ...(j....X3...st
+00007f30: 6f70 7069 6e67 5f63 7269 7465 7269 6f6e  opping_criterion
+00007f40: 2028 6c73 7166 6974 2e6e 6f6e 6c69 6e65   (lsqfit.nonline
+00007f50: 6172 5f66 6974 2061 7474 7269 6275 7465  ar_fit attribute
+00007f60: 2968 b355 004e 7472 ca05 0000 286a ba05  )h.U.Ntr....(j..
+00007f70: 0000 582e 0000 0073 7664 636f 7272 6563  ..X....svdcorrec
+00007f80: 7469 6f6e 2028 6c73 7166 6974 2e6e 6f6e  tion (lsqfit.non
+00007f90: 6c69 6e65 6172 5f66 6974 2061 7474 7269  linear_fit attri
+00007fa0: 6275 7465 2968 ca55 004e 7472 cb05 0000  bute)h.U.Ntr....
+00007fb0: 286a ba05 0000 5825 0000 0073 7664 6e20  (j....X%...svdn 
+00007fc0: 286c 7371 6669 742e 6e6f 6e6c 696e 6561  (lsqfit.nonlinea
+00007fd0: 725f 6669 7420 6174 7472 6962 7574 6529  r_fit attribute)
+00007fe0: 68f3 5500 4e74 72cc 0500 0028 6aba 0500  h.U.Ntr....(j...
+00007ff0: 0058 2500 0000 7469 6d65 2028 6c73 7166  .X%...time (lsqf
+00008000: 6974 2e6e 6f6e 6c69 6e65 6172 5f66 6974  it.nonlinear_fit
+00008010: 2061 7474 7269 6275 7465 2968 c055 004e   attribute)h.U.N
+00008020: 7472 cd05 0000 286a ba05 0000 5824 0000  tr....(j....X$..
+00008030: 0074 6f6c 2028 6c73 7166 6974 2e6e 6f6e  .tol (lsqfit.non
+00008040: 6c69 6e65 6172 5f66 6974 2061 7474 7269  linear_fit attri
+00008050: 6275 7465 296a 1101 0000 5500 4e74 72ce  bute)j....U.Ntr.
+00008060: 0500 0028 6aba 0500 0058 2200 0000 7820  ...(j....X"...x 
+00008070: 286c 7371 6669 742e 6e6f 6e6c 696e 6561  (lsqfit.nonlinea
+00008080: 725f 6669 7420 6174 7472 6962 7574 6529  r_fit attribute)
+00008090: 6a26 0100 0055 004e 7472 cf05 0000 286a  j&...U.Ntr....(j
+000080a0: ba05 0000 5822 0000 0079 2028 6c73 7166  ....X"...y (lsqf
+000080b0: 6974 2e6e 6f6e 6c69 6e65 6172 5f66 6974  it.nonlinear_fit
+000080c0: 2061 7474 7269 6275 7465 296a 3601 0000   attribute)j6...
+000080d0: 5500 4e74 72d0 0500 0028 6aba 0500 0058  U.Ntr....(j....X
+000080e0: 2800 0000 6e62 6c6f 636b 7320 286c 7371  (...nblocks (lsq
+000080f0: 6669 742e 6e6f 6e6c 696e 6561 725f 6669  fit.nonlinear_fi
+00008100: 7420 6174 7472 6962 7574 6529 6a30 0100  t attribute)j0..
+00008110: 0055 004e 7472 d105 0000 286a ba05 0000  .U.Ntr....(j....
+00008120: 5826 0000 0066 6f72 6d61 7428 2920 286c  X&...format() (l
 00008130: 7371 6669 742e 6e6f 6e6c 696e 6561 725f  sqfit.nonlinear_
-00008140: 6669 7420 6174 7472 6962 7574 6529 6a2a  fit attribute)j*
-00008150: 0100 0055 004e 7472 d505 0000 286a c005  ...U.Ntr....(j..
-00008160: 0000 5822 0000 0079 2028 6c73 7166 6974  ..X"...y (lsqfit
-00008170: 2e6e 6f6e 6c69 6e65 6172 5f66 6974 2061  .nonlinear_fit a
-00008180: 7474 7269 6275 7465 296a 3a01 0000 5500  ttribute)j:...U.
-00008190: 4e74 72d6 0500 0028 6ac0 0500 0058 2800  Ntr....(j....X(.
-000081a0: 0000 6e62 6c6f 636b 7320 286c 7371 6669  ..nblocks (lsqfi
-000081b0: 742e 6e6f 6e6c 696e 6561 725f 6669 7420  t.nonlinear_fit 
-000081c0: 6174 7472 6962 7574 6529 6a34 0100 0055  attribute)j4...U
-000081d0: 004e 7472 d705 0000 286a c005 0000 5826  .Ntr....(j....X&
-000081e0: 0000 0066 6f72 6d61 7428 2920 286c 7371  ...format() (lsq
-000081f0: 6669 742e 6e6f 6e6c 696e 6561 725f 6669  fit.nonlinear_fi
-00008200: 7420 6d65 7468 6f64 2968 c655 004e 7472  t method)h.U.Ntr
-00008210: d805 0000 286a c005 0000 5832 0000 0073  ....(j....X2...s
-00008220: 696d 756c 6174 6564 5f66 6974 5f69 7465  imulated_fit_ite
-00008230: 7228 2920 286c 7371 6669 742e 6e6f 6e6c  r() (lsqfit.nonl
-00008240: 696e 6561 725f 6669 7420 6d65 7468 6f64  inear_fit method
-00008250: 2968 ff55 004e 7472 d905 0000 286a c005  )h.U.Ntr....(j..
-00008260: 0000 5835 0000 0062 6f6f 7473 7472 6170  ..X5...bootstrap
-00008270: 7065 645f 6669 745f 6974 6572 2829 2028  ped_fit_iter() (
-00008280: 6c73 7166 6974 2e6e 6f6e 6c69 6e65 6172  lsqfit.nonlinear
-00008290: 5f66 6974 206d 6574 686f 6429 6a03 0100  _fit method)j...
-000082a0: 0055 004e 7472 da05 0000 286a c005 0000  .U.Ntr....(j....
-000082b0: 5826 0000 0064 756d 705f 7028 2920 286c  X&...dump_p() (l
-000082c0: 7371 6669 742e 6e6f 6e6c 696e 6561 725f  sqfit.nonlinear_
-000082d0: 6669 7420 6d65 7468 6f64 2968 be55 004e  fit method)h.U.N
-000082e0: 7472 db05 0000 286a c005 0000 582a 0000  tr....(j....X*..
-000082f0: 0064 756d 705f 706d 6561 6e28 2920 286c  .dump_pmean() (l
-00008300: 7371 6669 742e 6e6f 6e6c 696e 6561 725f  sqfit.nonlinear_
-00008310: 6669 7420 6d65 7468 6f64 2968 d055 004e  fit method)h.U.N
-00008320: 7472 dc05 0000 286a c005 0000 5836 0000  tr....(j....X6..
-00008330: 006c 6f61 645f 7061 7261 6d65 7465 7273  .load_parameters
-00008340: 2829 2028 6c73 7166 6974 2e6e 6f6e 6c69  () (lsqfit.nonli
-00008350: 6e65 6172 5f66 6974 2073 7461 7469 6320  near_fit static 
-00008360: 6d65 7468 6f64 2968 eb55 004e 7472 dd05  method)h.U.Ntr..
-00008370: 0000 286a c005 0000 582e 0000 0063 6865  ..(j....X....che
-00008380: 636b 5f72 6f75 6e64 6f66 6628 2920 286c  ck_roundoff() (l
-00008390: 7371 6669 742e 6e6f 6e6c 696e 6561 725f  sqfit.nonlinear_
-000083a0: 6669 7420 6d65 7468 6f64 2968 a955 004e  fit method)h.U.N
-000083b0: 7472 de05 0000 286a c005 0000 582a 0000  tr....(j....X*..
-000083c0: 0073 6574 2829 2028 6c73 7166 6974 2e6e  .set() (lsqfit.n
-000083d0: 6f6e 6c69 6e65 6172 5f66 6974 2073 7461  onlinear_fit sta
-000083e0: 7469 6320 6d65 7468 6f64 296a 1a01 0000  tic method)j....
-000083f0: 5500 4e74 72df 0500 0028 6ac0 0500 0058  U.Ntr....(j....X
-00008400: 2100 0000 656d 7062 6179 6573 5f66 6974  !...empbayes_fit
-00008410: 2829 2028 696e 206d 6f64 756c 6520 6c73  () (in module ls
-00008420: 7166 6974 296a 2c01 0000 5500 4e74 72e0  qfit)j,...U.Ntr.
-00008430: 0500 0028 6ac0 0500 0058 1900 0000 7761  ...(j....X....wa
-00008440: 7667 2829 2028 696e 206d 6f64 756c 6520  vg() (in module 
-00008450: 6c73 7166 6974 2968 f355 004e 7472 e105  lsqfit)h.U.Ntr..
-00008460: 0000 286a c005 0000 581b 0000 0067 616d  ..(j....X....gam
-00008470: 6d61 5128 2920 2869 6e20 6d6f 6475 6c65  maQ() (in module
-00008480: 206c 7371 6669 7429 68f5 5500 4e74 72e2   lsqfit)h.U.Ntr.
-00008490: 0500 0028 6ac0 0500 0058 2d00 0000 6164  ...(j....X-...ad
-000084a0: 645f 7061 7261 6d65 7465 725f 6469 7374  d_parameter_dist
-000084b0: 7269 6275 7469 6f6e 2829 2028 696e 206d  ribution() (in m
-000084c0: 6f64 756c 6520 6776 6172 296a 3e01 0000  odule gvar)j>...
-000084d0: 5500 4e74 72e3 0500 0028 6ac0 0500 0058  U.Ntr....(j....X
-000084e0: 2d00 0000 6465 6c5f 7061 7261 6d65 7465  -...del_paramete
-000084f0: 725f 6469 7374 7269 6275 7469 6f6e 2829  r_distribution()
-00008500: 2028 696e 206d 6f64 756c 6520 6776 6172   (in module gvar
-00008510: 2968 c855 004e 7472 e405 0000 286a c005  )h.U.Ntr....(j..
-00008520: 0000 582c 0000 0061 6464 5f70 6172 616d  ..X,...add_param
-00008530: 6574 6572 5f70 6172 656e 7468 6573 6573  eter_parentheses
-00008540: 2829 2028 696e 206d 6f64 756c 6520 6776  () (in module gv
-00008550: 6172 296a 1101 0000 5500 4e74 72e5 0500  ar)j....U.Ntr...
-00008560: 0028 6ac0 0500 0058 2100 0000 4261 7965  .(j....X!...Baye
-00008570: 7349 6e74 6567 7261 746f 7220 2863 6c61  sIntegrator (cla
-00008580: 7373 2069 6e20 6c73 7166 6974 2968 ca55  ss in lsqfit)h.U
-00008590: 004e 7472 e605 0000 286a c005 0000 582a  .Ntr....(j....X*
-000085a0: 0000 005f 5f63 616c 6c5f 5f28 2920 286c  ...__call__() (l
-000085b0: 7371 6669 742e 4261 7965 7349 6e74 6567  sqfit.BayesInteg
-000085c0: 7261 746f 7220 6d65 7468 6f64 2968 d455  rator method)h.U
-000085d0: 004e 7472 e705 0000 286a c005 0000 581a  .Ntr....(j....X.
-000085e0: 0000 0042 6179 6573 5044 4620 2863 6c61  ...BayesPDF (cla
-000085f0: 7373 2069 6e20 6c73 7166 6974 296a 2001  ss in lsqfit)j .
-00008600: 0000 5500 4e74 72e8 0500 0028 6ac0 0500  ..U.Ntr....(j...
-00008610: 0058 2300 0000 5f5f 6361 6c6c 5f5f 2829  .X#...__call__()
-00008620: 2028 6c73 7166 6974 2e42 6179 6573 5044   (lsqfit.BayesPD
-00008630: 4620 6d65 7468 6f64 296a 2401 0000 5500  F method)j$...U.
-00008640: 4e74 72e9 0500 0028 6ac0 0500 0058 2100  Ntr....(j....X!.
-00008650: 0000 6c6f 6770 6466 2829 2028 6c73 7166  ..logpdf() (lsqf
-00008660: 6974 2e42 6179 6573 5044 4620 6d65 7468  it.BayesPDF meth
-00008670: 6f64 2968 b155 004e 7472 ea05 0000 286a  od)h.U.Ntr....(j
-00008680: c005 0000 581d 0000 004d 756c 7469 4669  ....X....MultiFi
-00008690: 7474 6572 2028 636c 6173 7320 696e 206c  tter (class in l
-000086a0: 7371 6669 7429 68fd 5500 4e74 72eb 0500  sqfit)h.U.Ntr...
-000086b0: 0028 6ac0 0500 0058 2400 0000 6c73 7166  .(j....X$...lsqf
-000086c0: 6974 2829 2028 6c73 7166 6974 2e4d 756c  it() (lsqfit.Mul
-000086d0: 7469 4669 7474 6572 206d 6574 686f 6429  tiFitter method)
-000086e0: 68c4 5500 4e74 72ec 0500 0028 6ac0 0500  h.U.Ntr....(j...
-000086f0: 0058 2c00 0000 6368 6169 6e65 645f 6c73  .X,...chained_ls
-00008700: 7166 6974 2829 2028 6c73 7166 6974 2e4d  qfit() (lsqfit.M
-00008710: 756c 7469 4669 7474 6572 206d 6574 686f  ultiFitter metho
-00008720: 6429 6a30 0100 0055 004e 7472 ed05 0000  d)j0...U.Ntr....
-00008730: 286a c005 0000 5833 0000 0062 6f6f 7473  (j....X3...boots
-00008740: 7472 6170 7065 645f 6669 745f 6974 6572  trapped_fit_iter
-00008750: 2829 2028 6c73 7166 6974 2e4d 756c 7469  () (lsqfit.Multi
-00008760: 4669 7474 6572 206d 6574 686f 6429 68ba  Fitter method)h.
-00008770: 5500 4e74 72ee 0500 0028 6ac0 0500 0058  U.Ntr....(j....X
-00008780: 3100 0000 7072 6f63 6573 735f 6461 7461  1...process_data
-00008790: 2829 2028 6c73 7166 6974 2e4d 756c 7469  () (lsqfit.Multi
-000087a0: 4669 7474 6572 2073 7461 7469 6320 6d65  Fitter static me
-000087b0: 7468 6f64 296a 0501 0000 5500 4e74 72ef  thod)j....U.Ntr.
-000087c0: 0500 0028 6ac0 0500 0058 3400 0000 7072  ...(j....X4...pr
-000087d0: 6f63 6573 735f 6461 7461 7365 7428 2920  ocess_dataset() 
-000087e0: 286c 7371 6669 742e 4d75 6c74 6946 6974  (lsqfit.MultiFit
-000087f0: 7465 7220 7374 6174 6963 206d 6574 686f  ter static metho
-00008800: 6429 68d8 5500 4e74 72f0 0500 0028 6ac0  d)h.U.Ntr....(j.
-00008810: 0500 0058 2f00 0000 7368 6f77 5f70 6c6f  ...X/...show_plo
-00008820: 7473 2829 2028 6c73 7166 6974 2e4d 756c  ts() (lsqfit.Mul
-00008830: 7469 4669 7474 6572 2073 7461 7469 6320  tiFitter static 
-00008840: 6d65 7468 6f64 296a 0f01 0000 5500 4e74  method)j....U.Nt
-00008850: 72f1 0500 0028 6ac0 0500 0058 3300 0000  r....(j....X3...
-00008860: 666c 6174 7465 6e5f 6d6f 6465 6c73 2829  flatten_models()
-00008870: 2028 6c73 7166 6974 2e4d 756c 7469 4669   (lsqfit.MultiFi
-00008880: 7474 6572 2073 7461 7469 6320 6d65 7468  tter static meth
-00008890: 6f64 296a 2801 0000 5500 4e74 72f2 0500  od)j(...U.Ntr...
-000088a0: 0028 6ac0 0500 0058 2200 0000 4d75 6c74  .(j....X"...Mult
-000088b0: 6946 6974 7465 724d 6f64 656c 2028 636c  iFitterModel (cl
-000088c0: 6173 7320 696e 206c 7371 6669 7429 68d2  ass in lsqfit)h.
-000088d0: 5500 4e74 72f3 0500 0028 6ac0 0500 0058  U.Ntr....(j....X
-000088e0: 2b00 0000 6461 7461 7461 6720 286c 7371  +...datatag (lsq
-000088f0: 6669 742e 4d75 6c74 6946 6974 7465 724d  fit.MultiFitterM
-00008900: 6f64 656c 2061 7474 7269 6275 7465 296a  odel attribute)j
-00008910: 3601 0000 5500 4e74 72f4 0500 0028 6ac0  6...U.Ntr....(j.
-00008920: 0500 0058 2700 0000 6e63 6720 286c 7371  ...X'...ncg (lsq
-00008930: 6669 742e 4d75 6c74 6946 6974 7465 724d  fit.MultiFitterM
-00008940: 6f64 656c 2061 7474 7269 6275 7465 296a  odel attribute)j
-00008950: 2e01 0000 5500 4e74 72f5 0500 0028 6ac0  ....U.Ntr....(j.
-00008960: 0500 0058 2d00 0000 6275 696c 6470 7269  ...X-...buildpri
-00008970: 6f72 2829 2028 6c73 7166 6974 2e4d 756c  or() (lsqfit.Mul
-00008980: 7469 4669 7474 6572 4d6f 6465 6c20 6d65  tiFitterModel me
-00008990: 7468 6f64 2968 e655 004e 7472 f605 0000  thod)h.U.Ntr....
-000089a0: 286a c005 0000 582c 0000 0062 7569 6c64  (j....X,...build
-000089b0: 6461 7461 2829 2028 6c73 7166 6974 2e4d  data() (lsqfit.M
-000089c0: 756c 7469 4669 7474 6572 4d6f 6465 6c20  ultiFitterModel 
-000089d0: 6d65 7468 6f64 296a 2201 0000 5500 4e74  method)j"...U.Nt
-000089e0: 72f7 0500 0028 6ac0 0500 0058 2900 0000  r....(j....X)...
-000089f0: 6669 7466 636e 2829 2028 6c73 7166 6974  fitfcn() (lsqfit
-00008a00: 2e4d 756c 7469 4669 7474 6572 4d6f 6465  .MultiFitterMode
-00008a10: 6c20 6d65 7468 6f64 296a 1701 0000 5500  l method)j....U.
-00008a20: 4e74 72f8 0500 0028 6ac0 0500 0058 2f00  Ntr....(j....X/.
-00008a30: 0000 6275 696c 6464 6174 6173 6574 2829  ..builddataset()
-00008a40: 2028 6c73 7166 6974 2e4d 756c 7469 4669   (lsqfit.MultiFi
-00008a50: 7474 6572 4d6f 6465 6c20 6d65 7468 6f64  tterModel method
-00008a60: 2968 de55 004e 7472 f905 0000 286a c005  )h.U.Ntr....(j..
-00008a70: 0000 5838 0000 0067 6574 5f70 7269 6f72  ..X8...get_prior
-00008a80: 5f6b 6579 7328 2920 286c 7371 6669 742e  _keys() (lsqfit.
-00008a90: 4d75 6c74 6946 6974 7465 724d 6f64 656c  MultiFitterModel
-00008aa0: 2073 7461 7469 6320 6d65 7468 6f64 2968   static method)h
-00008ab0: fb55 004e 7472 fa05 0000 286a c005 0000  .U.Ntr....(j....
-00008ac0: 5833 0000 0070 7269 6f72 5f6b 6579 2829  X3...prior_key()
-00008ad0: 2028 6c73 7166 6974 2e4d 756c 7469 4669   (lsqfit.MultiFi
-00008ae0: 7474 6572 4d6f 6465 6c20 7374 6174 6963  tterModel static
-00008af0: 206d 6574 686f 6429 6a0b 0100 0055 004e   method)j....U.N
-00008b00: 7472 fb05 0000 6568 3d5d 6846 5d68 4f5d  tr....eh=]hF]hO]
-00008b10: 6858 5d72 fc05 0000 2828 6ac0 0500 0058  hX]r....((j....X
-00008b20: 2500 0000 7363 6970 795f 6c65 6173 745f  %...scipy_least_
-00008b30: 7371 7561 7265 7320 2863 6c61 7373 2069  squares (class i
-00008b40: 6e20 6c73 7166 6974 2968 c255 004e 7472  n lsqfit)h.U.Ntr
-00008b50: fd05 0000 286a c005 0000 5828 0000 0078  ....(j....X(...x
-00008b60: 2028 6c73 7166 6974 2e73 6369 7079 5f6c   (lsqfit.scipy_l
-00008b70: 6561 7374 5f73 7175 6172 6573 2061 7474  east_squares att
-00008b80: 7269 6275 7465 296a 1301 0000 5500 4e74  ribute)j....U.Nt
-00008b90: 72fe 0500 0028 6ac0 0500 0058 2a00 0000  r....(j....X*...
-00008ba0: 636f 7620 286c 7371 6669 742e 7363 6970  cov (lsqfit.scip
-00008bb0: 795f 6c65 6173 745f 7371 7561 7265 7320  y_least_squares 
-00008bc0: 6174 7472 6962 7574 6529 6a26 0100 0055  attribute)j&...U
-00008bd0: 004e 7472 ff05 0000 286a c005 0000 5832  .Ntr....(j....X2
-00008be0: 0000 0064 6573 6372 6970 7469 6f6e 2028  ...description (
-00008bf0: 6c73 7166 6974 2e73 6369 7079 5f6c 6561  lsqfit.scipy_lea
-00008c00: 7374 5f73 7175 6172 6573 2061 7474 7269  st_squares attri
-00008c10: 6275 7465 2968 ef55 004e 7472 0006 0000  bute)h.U.Ntr....
-00008c20: 286a c005 0000 5828 0000 0066 2028 6c73  (j....X(...f (ls
-00008c30: 7166 6974 2e73 6369 7079 5f6c 6561 7374  qfit.scipy_least
-00008c40: 5f73 7175 6172 6573 2061 7474 7269 6275  _squares attribu
-00008c50: 7465 2968 b655 004e 7472 0106 0000 286a  te)h.U.Ntr....(j
-00008c60: c005 0000 5828 0000 004a 2028 6c73 7166  ....X(...J (lsqf
-00008c70: 6974 2e73 6369 7079 5f6c 6561 7374 5f73  it.scipy_least_s
-00008c80: 7175 6172 6573 2061 7474 7269 6275 7465  quares attribute
-00008c90: 2968 e055 004e 7472 0206 0000 286a c005  )h.U.Ntr....(j..
-00008ca0: 0000 582a 0000 006e 6974 2028 6c73 7166  ..X*...nit (lsqf
-00008cb0: 6974 2e73 6369 7079 5f6c 6561 7374 5f73  it.scipy_least_s
-00008cc0: 7175 6172 6573 2061 7474 7269 6275 7465  quares attribute
-00008cd0: 2968 dc55 004e 7472 0306 0000 286a c005  )h.U.Ntr....(j..
-00008ce0: 0000 5839 0000 0073 746f 7070 696e 675f  ..X9...stopping_
-00008cf0: 6372 6974 6572 696f 6e20 286c 7371 6669  criterion (lsqfi
-00008d00: 742e 7363 6970 795f 6c65 6173 745f 7371  t.scipy_least_sq
-00008d10: 7561 7265 7320 6174 7472 6962 7574 6529  uares attribute)
-00008d20: 68ad 5500 4e74 7204 0600 0028 6ac0 0500  h.U.Ntr....(j...
-00008d30: 0058 2c00 0000 6572 726f 7220 286c 7371  .X,...error (lsq
-00008d40: 6669 742e 7363 6970 795f 6c65 6173 745f  fit.scipy_least_
-00008d50: 7371 7561 7265 7320 6174 7472 6962 7574  squares attribut
-00008d60: 6529 68e2 5500 4e74 7205 0600 0028 6ac0  e)h.U.Ntr....(j.
-00008d70: 0500 0058 2e00 0000 7265 7375 6c74 7320  ...X....results 
-00008d80: 286c 7371 6669 742e 7363 6970 795f 6c65  (lsqfit.scipy_le
-00008d90: 6173 745f 7371 7561 7265 7320 6174 7472  ast_squares attr
-00008da0: 6962 7574 6529 68b8 5500 4e74 7206 0600  ibute)h.U.Ntr...
-00008db0: 0028 6ac0 0500 0058 2200 0000 7363 6970  .(j....X"...scip
-00008dc0: 795f 6d75 6c74 696d 696e 6578 2028 636c  y_multiminex (cl
-00008dd0: 6173 7320 696e 206c 7371 6669 7429 6a0d  ass in lsqfit)j.
-00008de0: 0100 0055 004e 7472 0706 0000 286a c005  ...U.Ntr....(j..
-00008df0: 0000 5825 0000 0078 2028 6c73 7166 6974  ..X%...x (lsqfit
-00008e00: 2e73 6369 7079 5f6d 756c 7469 6d69 6e65  .scipy_multimine
-00008e10: 7820 6174 7472 6962 7574 6529 6a1c 0100  x attribute)j...
-00008e20: 0055 004e 7472 0806 0000 286a c005 0000  .U.Ntr....(j....
-00008e30: 5825 0000 0066 2028 6c73 7166 6974 2e73  X%...f (lsqfit.s
-00008e40: 6369 7079 5f6d 756c 7469 6d69 6e65 7820  cipy_multiminex 
-00008e50: 6174 7472 6962 7574 6529 6a38 0100 0055  attribute)j8...U
-00008e60: 004e 7472 0906 0000 286a c005 0000 5827  .Ntr....(j....X'
-00008e70: 0000 006e 6974 2028 6c73 7166 6974 2e73  ...nit (lsqfit.s
-00008e80: 6369 7079 5f6d 756c 7469 6d69 6e65 7820  cipy_multiminex 
-00008e90: 6174 7472 6962 7574 6529 68da 5500 4e74  attribute)h.U.Nt
-00008ea0: 720a 0600 0028 6ac0 0500 0058 2900 0000  r....(j....X)...
-00008eb0: 6572 726f 7220 286c 7371 6669 742e 7363  error (lsqfit.sc
-00008ec0: 6970 795f 6d75 6c74 696d 696e 6578 2061  ipy_multiminex a
-00008ed0: 7474 7269 6275 7465 2968 ab55 004e 7472  ttribute)h.U.Ntr
-00008ee0: 0b06 0000 6568 685d 6871 5d72 0c06 0000  ....ehh]hq]r....
-00008ef0: 2828 6ac0 0500 0058 2400 0000 6c73 7166  ((j....X$...lsqf
-00008f00: 6974 2e67 736c 5f6d 756c 7469 6669 7420  it.gsl_multifit 
-00008f10: 2862 7569 6c74 2d69 6e20 636c 6173 7329  (built-in class)
-00008f20: 68e8 5500 4e74 720d 0600 0028 6ac0 0500  h.U.Ntr....(j...
-00008f30: 0058 2700 0000 6c73 7166 6974 2e67 736c  .X'...lsqfit.gsl
-00008f40: 5f76 315f 6d75 6c74 6966 6974 2028 6275  _v1_multifit (bu
-00008f50: 696c 742d 696e 2063 6c61 7373 296a 1901  ilt-in class)j..
-00008f60: 0000 5500 4e74 720e 0600 0028 6ac0 0500  ..U.Ntr....(j...
-00008f70: 0058 2600 0000 6c73 7166 6974 2e67 736c  .X&...lsqfit.gsl
-00008f80: 5f6d 756c 7469 6d69 6e65 7820 2862 7569  _multiminex (bui
-00008f90: 6c74 2d69 6e20 636c 6173 7329 68b5 5500  lt-in class)h.U.
-00008fa0: 4e74 720f 0600 0065 7555 0861 6c6c 5f64  Ntr....euU.all_d
-00008fb0: 6f63 7372 1006 0000 7d72 1106 0000 2868  ocsr....}r....(h
-00008fc0: 0c47 41d6 d09c df52 f078 6822 4741 d6d0  .GA....R.xh"GA..
-00008fd0: 9cdf d181 5668 2b47 41d6 d09c dfa0 fdf0  ....Vh+GA.......
-00008fe0: 683d 4741 d6d0 9cdf c2f6 5168 4647 41d6  h=GA......QhFGA.
-00008ff0: d09c df3e 6b23 684f 4741 d6d0 9cdf 4476  ...>k#hOGA....Dv
-00009000: 3e68 5847 41d6 d09c dfcc 1566 6868 4741  >hXGA......fhhGA
-00009010: d6d0 9cdf 471a 5d68 7147 41d6 d09c df51  ....G.]hqGA....Q
-00009020: 4296 7555 0873 6574 7469 6e67 7372 1206  B.uU.settingsr..
-00009030: 0000 7d72 1306 0000 2855 1563 6c6f 616b  ..}r....(U.cloak
-00009040: 5f65 6d61 696c 5f61 6464 7265 7373 6573  _email_addresses
-00009050: 7214 0600 0088 550c 7065 705f 6261 7365  r.....U.pep_base
-00009060: 5f75 726c 7215 0600 0055 2068 7474 7073  _urlr....U https
-00009070: 3a2f 2f77 7777 2e70 7974 686f 6e2e 6f72  ://www.python.or
-00009080: 672f 6465 762f 7065 7073 2f72 1606 0000  g/dev/peps/r....
-00009090: 550a 6861 6c74 5f6c 6576 656c 7217 0600  U.halt_levelr...
-000090a0: 004b 0555 1273 6563 7473 7562 7469 746c  .K.U.sectsubtitl
-000090b0: 655f 7866 6f72 6d72 1806 0000 8955 0c73  e_xformr.....U.s
-000090c0: 6d61 7274 5f71 756f 7465 7372 1906 0000  mart_quotesr....
-000090d0: 8855 0e69 6e70 7574 5f65 6e63 6f64 696e  .U.input_encodin
-000090e0: 6772 1a06 0000 5509 7574 662d 382d 7369  gr....U.utf-8-si
-000090f0: 6772 1b06 0000 550c 7266 635f 6261 7365  gr....U.rfc_base
-00009100: 5f75 726c 721c 0600 0055 1c68 7474 7073  _urlr....U.https
-00009110: 3a2f 2f74 6f6f 6c73 2e69 6574 662e 6f72  ://tools.ietf.or
-00009120: 672f 6874 6d6c 2f72 1d06 0000 550e 7266  g/html/r....U.rf
-00009130: 635f 7265 6665 7265 6e63 6573 721e 0600  c_referencesr...
-00009140: 004e 550e 7065 705f 7265 6665 7265 6e63  .NU.pep_referenc
-00009150: 6573 721f 0600 004e 550d 6c61 6e67 7561  esr....NU.langua
-00009160: 6765 5f63 6f64 6572 2006 0000 5502 656e  ge_coder ...U.en
-00009170: 7221 0600 0055 0e64 6f63 7469 746c 655f  r!...U.doctitle_
-00009180: 7866 6f72 6d72 2206 0000 8955 1d74 7269  xformr"....U.tri
-00009190: 6d5f 666f 6f74 6e6f 7465 5f72 6566 6572  m_footnote_refer
-000091a0: 656e 6365 5f73 7061 6365 7223 0600 0089  ence_spacer#....
-000091b0: 5503 656e 7672 2406 0000 6802 5513 736d  U.envr$...h.U.sm
-000091c0: 6172 7471 756f 7465 735f 6c6f 6361 6c65  artquotes_locale
-000091d0: 7372 2506 0000 5d72 2606 0000 5516 6669  sr%...]r&...U.fi
-000091e0: 6c65 5f69 6e73 6572 7469 6f6e 5f65 6e61  le_insertion_ena
-000091f0: 626c 6564 7227 0600 0088 550f 6765 7474  bledr'....U.gett
-00009200: 6578 745f 636f 6d70 6163 7472 2806 0000  ext_compactr(...
-00009210: 8855 1065 6d62 6564 5f73 7479 6c65 7368  .U.embed_stylesh
-00009220: 6565 7472 2906 0000 8975 550b 7265 665f  eetr)....uU.ref_
-00009230: 636f 6e74 6578 7472 2a06 0000 7d55 1066  contextr*...}U.f
-00009240: 696c 6573 5f74 6f5f 7265 6275 696c 6472  iles_to_rebuildr
-00009250: 2b06 0000 7d72 2c06 0000 286a 4202 0000  +...}r,...(jB...
-00009260: 6807 5d72 2d06 0000 680c 6185 5272 2e06  h.]r-...h.a.Rr..
-00009270: 0000 6a3d 0200 0068 075d 722f 0600 0068  ..j=...h.]r/...h
-00009280: 0c61 8552 7230 0600 006a 3e02 0000 6807  .a.Rr0...j>...h.
-00009290: 5d72 3106 0000 680c 6185 5272 3206 0000  ]r1...h.a.Rr2...
-000092a0: 6a41 0200 0068 075d 7233 0600 0068 0c61  jA...h.]r3...h.a
-000092b0: 8552 7234 0600 006a 4402 0000 6807 5d72  .Rr4...jD...h.]r
-000092c0: 3506 0000 680c 6185 5272 3606 0000 6a40  5...h.a.Rr6...j@
-000092d0: 0200 0068 075d 7237 0600 0068 0c61 8552  ...h.]r7...h.a.R
-000092e0: 7238 0600 006a 3f02 0000 6807 5d72 3906  r8...j?...h.]r9.
-000092f0: 0000 680c 6185 5272 3a06 0000 6a43 0200  ..h.a.Rr:...jC..
-00009300: 0068 075d 723b 0600 0068 0c61 8552 723c  .h.]r;...h.a.Rr<
-00009310: 0600 0075 550e 746f 635f 7365 636e 756d  ...uU.toc_secnum
-00009320: 6265 7273 723d 0600 007d 5512 7665 7273  bersr=...}U.vers
-00009330: 696f 6e69 6e67 5f63 6f6d 7061 7265 723e  ioning_comparer>
-00009340: 0600 0089 550f 5f6e 6974 7069 636b 5f69  ....U._nitpick_i
-00009350: 676e 6f72 6572 3f06 0000 6807 5d85 5272  gnorer?...h.].Rr
-00009360: 4006 0000 7562 2e                        @...ub.
+00008140: 6669 7420 6d65 7468 6f64 2968 c655 004e  fit method)h.U.N
+00008150: 7472 d205 0000 286a ba05 0000 5832 0000  tr....(j....X2..
+00008160: 0073 696d 756c 6174 6564 5f66 6974 5f69  .simulated_fit_i
+00008170: 7465 7228 2920 286c 7371 6669 742e 6e6f  ter() (lsqfit.no
+00008180: 6e6c 696e 6561 725f 6669 7420 6d65 7468  nlinear_fit meth
+00008190: 6f64 2968 fb55 004e 7472 d305 0000 286a  od)h.U.Ntr....(j
+000081a0: ba05 0000 5835 0000 0062 6f6f 7473 7472  ....X5...bootstr
+000081b0: 6170 7065 645f 6669 745f 6974 6572 2829  apped_fit_iter()
+000081c0: 2028 6c73 7166 6974 2e6e 6f6e 6c69 6e65   (lsqfit.nonline
+000081d0: 6172 5f66 6974 206d 6574 686f 6429 68ff  ar_fit method)h.
+000081e0: 5500 4e74 72d4 0500 0028 6aba 0500 0058  U.Ntr....(j....X
+000081f0: 2e00 0000 6368 6563 6b5f 726f 756e 646f  ....check_roundo
+00008200: 6666 2829 2028 6c73 7166 6974 2e6e 6f6e  ff() (lsqfit.non
+00008210: 6c69 6e65 6172 5f66 6974 206d 6574 686f  linear_fit metho
+00008220: 6429 68a9 5500 4e74 72d5 0500 0028 6aba  d)h.U.Ntr....(j.
+00008230: 0500 0058 2a00 0000 7365 7428 2920 286c  ...X*...set() (l
+00008240: 7371 6669 742e 6e6f 6e6c 696e 6561 725f  sqfit.nonlinear_
+00008250: 6669 7420 7374 6174 6963 206d 6574 686f  fit static metho
+00008260: 6429 6a16 0100 0055 004e 7472 d605 0000  d)j....U.Ntr....
+00008270: 286a ba05 0000 5821 0000 0065 6d70 6261  (j....X!...empba
+00008280: 7965 735f 6669 7428 2920 2869 6e20 6d6f  yes_fit() (in mo
+00008290: 6475 6c65 206c 7371 6669 7429 6a28 0100  dule lsqfit)j(..
+000082a0: 0055 004e 7472 d705 0000 286a ba05 0000  .U.Ntr....(j....
+000082b0: 5819 0000 0077 6176 6728 2920 2869 6e20  X....wavg() (in 
+000082c0: 6d6f 6475 6c65 206c 7371 6669 7429 68ef  module lsqfit)h.
+000082d0: 5500 4e74 72d8 0500 0028 6aba 0500 0058  U.Ntr....(j....X
+000082e0: 1b00 0000 6761 6d6d 6151 2829 2028 696e  ....gammaQ() (in
+000082f0: 206d 6f64 756c 6520 6c73 7166 6974 2968   module lsqfit)h
+00008300: f155 004e 7472 d905 0000 286a ba05 0000  .U.Ntr....(j....
+00008310: 582d 0000 0061 6464 5f70 6172 616d 6574  X-...add_paramet
+00008320: 6572 5f64 6973 7472 6962 7574 696f 6e28  er_distribution(
+00008330: 2920 2869 6e20 6d6f 6475 6c65 2067 7661  ) (in module gva
+00008340: 7229 68be 5500 4e74 72da 0500 0028 6aba  r)h.U.Ntr....(j.
+00008350: 0500 0058 2d00 0000 6465 6c5f 7061 7261  ...X-...del_para
+00008360: 6d65 7465 725f 6469 7374 7269 6275 7469  meter_distributi
+00008370: 6f6e 2829 2028 696e 206d 6f64 756c 6520  on() (in module 
+00008380: 6776 6172 2968 c855 004e 7472 db05 0000  gvar)h.U.Ntr....
+00008390: 286a ba05 0000 582c 0000 0061 6464 5f70  (j....X,...add_p
+000083a0: 6172 616d 6574 6572 5f70 6172 656e 7468  arameter_parenth
+000083b0: 6573 6573 2829 2028 696e 206d 6f64 756c  eses() (in modul
+000083c0: 6520 6776 6172 2968 ce55 004e 7472 dc05  e gvar)h.U.Ntr..
+000083d0: 0000 286a ba05 0000 5821 0000 0042 6179  ..(j....X!...Bay
+000083e0: 6573 496e 7465 6772 6174 6f72 2028 636c  esIntegrator (cl
+000083f0: 6173 7320 696e 206c 7371 6669 7429 6a0d  ass in lsqfit)j.
+00008400: 0100 0055 004e 7472 dd05 0000 286a ba05  ...U.Ntr....(j..
+00008410: 0000 582a 0000 005f 5f63 616c 6c5f 5f28  ..X*...__call__(
+00008420: 2920 286c 7371 6669 742e 4261 7965 7349  ) (lsqfit.BayesI
+00008430: 6e74 6567 7261 746f 7220 6d65 7468 6f64  ntegrator method
+00008440: 2968 d255 004e 7472 de05 0000 286a ba05  )h.U.Ntr....(j..
+00008450: 0000 581a 0000 0042 6179 6573 5044 4620  ..X....BayesPDF 
+00008460: 2863 6c61 7373 2069 6e20 6c73 7166 6974  (class in lsqfit
+00008470: 296a 1c01 0000 5500 4e74 72df 0500 0028  )j....U.Ntr....(
+00008480: 6aba 0500 0058 2300 0000 5f5f 6361 6c6c  j....X#...__call
+00008490: 5f5f 2829 2028 6c73 7166 6974 2e42 6179  __() (lsqfit.Bay
+000084a0: 6573 5044 4620 6d65 7468 6f64 296a 2001  esPDF method)j .
+000084b0: 0000 5500 4e74 72e0 0500 0028 6aba 0500  ..U.Ntr....(j...
+000084c0: 0058 2100 0000 6c6f 6770 6466 2829 2028  .X!...logpdf() (
+000084d0: 6c73 7166 6974 2e42 6179 6573 5044 4620  lsqfit.BayesPDF 
+000084e0: 6d65 7468 6f64 2968 b155 004e 7472 e105  method)h.U.Ntr..
+000084f0: 0000 286a ba05 0000 581d 0000 004d 756c  ..(j....X....Mul
+00008500: 7469 4669 7474 6572 2028 636c 6173 7320  tiFitter (class 
+00008510: 696e 206c 7371 6669 7429 68f9 5500 4e74  in lsqfit)h.U.Nt
+00008520: 72e2 0500 0028 6aba 0500 0058 2400 0000  r....(j....X$...
+00008530: 6c73 7166 6974 2829 2028 6c73 7166 6974  lsqfit() (lsqfit
+00008540: 2e4d 756c 7469 4669 7474 6572 206d 6574  .MultiFitter met
+00008550: 686f 6429 68c4 5500 4e74 72e3 0500 0028  hod)h.U.Ntr....(
+00008560: 6aba 0500 0058 2c00 0000 6368 6169 6e65  j....X,...chaine
+00008570: 645f 6c73 7166 6974 2829 2028 6c73 7166  d_lsqfit() (lsqf
+00008580: 6974 2e4d 756c 7469 4669 7474 6572 206d  it.MultiFitter m
+00008590: 6574 686f 6429 6a2c 0100 0055 004e 7472  ethod)j,...U.Ntr
+000085a0: e405 0000 286a ba05 0000 5833 0000 0062  ....(j....X3...b
+000085b0: 6f6f 7473 7472 6170 7065 645f 6669 745f  ootstrapped_fit_
+000085c0: 6974 6572 2829 2028 6c73 7166 6974 2e4d  iter() (lsqfit.M
+000085d0: 756c 7469 4669 7474 6572 206d 6574 686f  ultiFitter metho
+000085e0: 6429 68ba 5500 4e74 72e5 0500 0028 6aba  d)h.U.Ntr....(j.
+000085f0: 0500 0058 3100 0000 7072 6f63 6573 735f  ...X1...process_
+00008600: 6461 7461 2829 2028 6c73 7166 6974 2e4d  data() (lsqfit.M
+00008610: 756c 7469 4669 7474 6572 2073 7461 7469  ultiFitter stati
+00008620: 6320 6d65 7468 6f64 296a 0101 0000 5500  c method)j....U.
+00008630: 4e74 72e6 0500 0028 6aba 0500 0058 3400  Ntr....(j....X4.
+00008640: 0000 7072 6f63 6573 735f 6461 7461 7365  ..process_datase
+00008650: 7428 2920 286c 7371 6669 742e 4d75 6c74  t() (lsqfit.Mult
+00008660: 6946 6974 7465 7220 7374 6174 6963 206d  iFitter static m
+00008670: 6574 686f 6429 68d6 5500 4e74 72e7 0500  ethod)h.U.Ntr...
+00008680: 0028 6aba 0500 0058 2f00 0000 7368 6f77  .(j....X/...show
+00008690: 5f70 6c6f 7473 2829 2028 6c73 7166 6974  _plots() (lsqfit
+000086a0: 2e4d 756c 7469 4669 7474 6572 2073 7461  .MultiFitter sta
+000086b0: 7469 6320 6d65 7468 6f64 296a 0b01 0000  tic method)j....
+000086c0: 5500 4e74 72e8 0500 0028 6aba 0500 0058  U.Ntr....(j....X
+000086d0: 3300 0000 666c 6174 7465 6e5f 6d6f 6465  3...flatten_mode
+000086e0: 6c73 2829 2028 6c73 7166 6974 2e4d 756c  ls() (lsqfit.Mul
+000086f0: 7469 4669 7474 6572 2073 7461 7469 6320  tiFitter static 
+00008700: 6d65 7468 6f64 296a 2401 0000 5500 4e74  method)j$...U.Nt
+00008710: 72e9 0500 0028 6aba 0500 0058 2200 0000  r....(j....X"...
+00008720: 4d75 6c74 6946 6974 7465 724d 6f64 656c  MultiFitterModel
+00008730: 2028 636c 6173 7320 696e 206c 7371 6669   (class in lsqfi
+00008740: 7429 68d0 5500 4e74 72ea 0500 0028 6aba  t)h.U.Ntr....(j.
+00008750: 0500 0058 2b00 0000 6461 7461 7461 6720  ...X+...datatag 
+00008760: 286c 7371 6669 742e 4d75 6c74 6946 6974  (lsqfit.MultiFit
+00008770: 7465 724d 6f64 656c 2061 7474 7269 6275  terModel attribu
+00008780: 7465 296a 3201 0000 5500 4e74 72eb 0500  te)j2...U.Ntr...
+00008790: 0028 6aba 0500 0058 2700 0000 6e63 6720  .(j....X'...ncg 
+000087a0: 286c 7371 6669 742e 4d75 6c74 6946 6974  (lsqfit.MultiFit
+000087b0: 7465 724d 6f64 656c 2061 7474 7269 6275  terModel attribu
+000087c0: 7465 296a 2a01 0000 5500 4e74 72ec 0500  te)j*...U.Ntr...
+000087d0: 0028 6aba 0500 0058 2d00 0000 6275 696c  .(j....X-...buil
+000087e0: 6470 7269 6f72 2829 2028 6c73 7166 6974  dprior() (lsqfit
+000087f0: 2e4d 756c 7469 4669 7474 6572 4d6f 6465  .MultiFitterMode
+00008800: 6c20 6d65 7468 6f64 2968 e455 004e 7472  l method)h.U.Ntr
+00008810: ed05 0000 286a ba05 0000 582c 0000 0062  ....(j....X,...b
+00008820: 7569 6c64 6461 7461 2829 2028 6c73 7166  uilddata() (lsqf
+00008830: 6974 2e4d 756c 7469 4669 7474 6572 4d6f  it.MultiFitterMo
+00008840: 6465 6c20 6d65 7468 6f64 296a 1e01 0000  del method)j....
+00008850: 5500 4e74 72ee 0500 0028 6aba 0500 0058  U.Ntr....(j....X
+00008860: 2900 0000 6669 7466 636e 2829 2028 6c73  )...fitfcn() (ls
+00008870: 7166 6974 2e4d 756c 7469 4669 7474 6572  qfit.MultiFitter
+00008880: 4d6f 6465 6c20 6d65 7468 6f64 296a 1301  Model method)j..
+00008890: 0000 5500 4e74 72ef 0500 0028 6aba 0500  ..U.Ntr....(j...
+000088a0: 0058 2f00 0000 6275 696c 6464 6174 6173  .X/...builddatas
+000088b0: 6574 2829 2028 6c73 7166 6974 2e4d 756c  et() (lsqfit.Mul
+000088c0: 7469 4669 7474 6572 4d6f 6465 6c20 6d65  tiFitterModel me
+000088d0: 7468 6f64 2968 dc55 004e 7472 f005 0000  thod)h.U.Ntr....
+000088e0: 286a ba05 0000 5838 0000 0067 6574 5f70  (j....X8...get_p
+000088f0: 7269 6f72 5f6b 6579 7328 2920 286c 7371  rior_keys() (lsq
+00008900: 6669 742e 4d75 6c74 6946 6974 7465 724d  fit.MultiFitterM
+00008910: 6f64 656c 2073 7461 7469 6320 6d65 7468  odel static meth
+00008920: 6f64 2968 f755 004e 7472 f105 0000 286a  od)h.U.Ntr....(j
+00008930: ba05 0000 5833 0000 0070 7269 6f72 5f6b  ....X3...prior_k
+00008940: 6579 2829 2028 6c73 7166 6974 2e4d 756c  ey() (lsqfit.Mul
+00008950: 7469 4669 7474 6572 4d6f 6465 6c20 7374  tiFitterModel st
+00008960: 6174 6963 206d 6574 686f 6429 6a07 0100  atic method)j...
+00008970: 0055 004e 7472 f205 0000 6568 3d5d 6846  .U.Ntr....eh=]hF
+00008980: 5d68 4f5d 6858 5d72 f305 0000 2828 6aba  ]hO]hX]r....((j.
+00008990: 0500 0058 2500 0000 7363 6970 795f 6c65  ...X%...scipy_le
+000089a0: 6173 745f 7371 7561 7265 7320 2863 6c61  ast_squares (cla
+000089b0: 7373 2069 6e20 6c73 7166 6974 2968 c255  ss in lsqfit)h.U
+000089c0: 004e 7472 f405 0000 286a ba05 0000 5828  .Ntr....(j....X(
+000089d0: 0000 0078 2028 6c73 7166 6974 2e73 6369  ...x (lsqfit.sci
+000089e0: 7079 5f6c 6561 7374 5f73 7175 6172 6573  py_least_squares
+000089f0: 2061 7474 7269 6275 7465 296a 0f01 0000   attribute)j....
+00008a00: 5500 4e74 72f5 0500 0028 6aba 0500 0058  U.Ntr....(j....X
+00008a10: 2a00 0000 636f 7620 286c 7371 6669 742e  *...cov (lsqfit.
+00008a20: 7363 6970 795f 6c65 6173 745f 7371 7561  scipy_least_squa
+00008a30: 7265 7320 6174 7472 6962 7574 6529 6a22  res attribute)j"
+00008a40: 0100 0055 004e 7472 f605 0000 286a ba05  ...U.Ntr....(j..
+00008a50: 0000 5832 0000 0064 6573 6372 6970 7469  ..X2...descripti
+00008a60: 6f6e 2028 6c73 7166 6974 2e73 6369 7079  on (lsqfit.scipy
+00008a70: 5f6c 6561 7374 5f73 7175 6172 6573 2061  _least_squares a
+00008a80: 7474 7269 6275 7465 2968 eb55 004e 7472  ttribute)h.U.Ntr
+00008a90: f705 0000 286a ba05 0000 5828 0000 0066  ....(j....X(...f
+00008aa0: 2028 6c73 7166 6974 2e73 6369 7079 5f6c   (lsqfit.scipy_l
+00008ab0: 6561 7374 5f73 7175 6172 6573 2061 7474  east_squares att
+00008ac0: 7269 6275 7465 2968 b655 004e 7472 f805  ribute)h.U.Ntr..
+00008ad0: 0000 286a ba05 0000 5828 0000 004a 2028  ..(j....X(...J (
+00008ae0: 6c73 7166 6974 2e73 6369 7079 5f6c 6561  lsqfit.scipy_lea
+00008af0: 7374 5f73 7175 6172 6573 2061 7474 7269  st_squares attri
+00008b00: 6275 7465 2968 de55 004e 7472 f905 0000  bute)h.U.Ntr....
+00008b10: 286a ba05 0000 582a 0000 006e 6974 2028  (j....X*...nit (
+00008b20: 6c73 7166 6974 2e73 6369 7079 5f6c 6561  lsqfit.scipy_lea
+00008b30: 7374 5f73 7175 6172 6573 2061 7474 7269  st_squares attri
+00008b40: 6275 7465 2968 da55 004e 7472 fa05 0000  bute)h.U.Ntr....
+00008b50: 286a ba05 0000 5839 0000 0073 746f 7070  (j....X9...stopp
+00008b60: 696e 675f 6372 6974 6572 696f 6e20 286c  ing_criterion (l
+00008b70: 7371 6669 742e 7363 6970 795f 6c65 6173  sqfit.scipy_leas
+00008b80: 745f 7371 7561 7265 7320 6174 7472 6962  t_squares attrib
+00008b90: 7574 6529 68ad 5500 4e74 72fb 0500 0028  ute)h.U.Ntr....(
+00008ba0: 6aba 0500 0058 2c00 0000 6572 726f 7220  j....X,...error 
+00008bb0: 286c 7371 6669 742e 7363 6970 795f 6c65  (lsqfit.scipy_le
+00008bc0: 6173 745f 7371 7561 7265 7320 6174 7472  ast_squares attr
+00008bd0: 6962 7574 6529 68e0 5500 4e74 72fc 0500  ibute)h.U.Ntr...
+00008be0: 0028 6aba 0500 0058 2e00 0000 7265 7375  .(j....X....resu
+00008bf0: 6c74 7320 286c 7371 6669 742e 7363 6970  lts (lsqfit.scip
+00008c00: 795f 6c65 6173 745f 7371 7561 7265 7320  y_least_squares 
+00008c10: 6174 7472 6962 7574 6529 68b8 5500 4e74  attribute)h.U.Nt
+00008c20: 72fd 0500 0028 6aba 0500 0058 2200 0000  r....(j....X"...
+00008c30: 7363 6970 795f 6d75 6c74 696d 696e 6578  scipy_multiminex
+00008c40: 2028 636c 6173 7320 696e 206c 7371 6669   (class in lsqfi
+00008c50: 7429 6a09 0100 0055 004e 7472 fe05 0000  t)j....U.Ntr....
+00008c60: 286a ba05 0000 5825 0000 0078 2028 6c73  (j....X%...x (ls
+00008c70: 7166 6974 2e73 6369 7079 5f6d 756c 7469  qfit.scipy_multi
+00008c80: 6d69 6e65 7820 6174 7472 6962 7574 6529  minex attribute)
+00008c90: 6a18 0100 0055 004e 7472 ff05 0000 286a  j....U.Ntr....(j
+00008ca0: ba05 0000 5825 0000 0066 2028 6c73 7166  ....X%...f (lsqf
+00008cb0: 6974 2e73 6369 7079 5f6d 756c 7469 6d69  it.scipy_multimi
+00008cc0: 6e65 7820 6174 7472 6962 7574 6529 6a34  nex attribute)j4
+00008cd0: 0100 0055 004e 7472 0006 0000 286a ba05  ...U.Ntr....(j..
+00008ce0: 0000 5827 0000 006e 6974 2028 6c73 7166  ..X'...nit (lsqf
+00008cf0: 6974 2e73 6369 7079 5f6d 756c 7469 6d69  it.scipy_multimi
+00008d00: 6e65 7820 6174 7472 6962 7574 6529 68d8  nex attribute)h.
+00008d10: 5500 4e74 7201 0600 0028 6aba 0500 0058  U.Ntr....(j....X
+00008d20: 2900 0000 6572 726f 7220 286c 7371 6669  )...error (lsqfi
+00008d30: 742e 7363 6970 795f 6d75 6c74 696d 696e  t.scipy_multimin
+00008d40: 6578 2061 7474 7269 6275 7465 2968 ab55  ex attribute)h.U
+00008d50: 004e 7472 0206 0000 6568 685d 6871 5d72  .Ntr....ehh]hq]r
+00008d60: 0306 0000 2828 6aba 0500 0058 2400 0000  ....((j....X$...
+00008d70: 6c73 7166 6974 2e67 736c 5f6d 756c 7469  lsqfit.gsl_multi
+00008d80: 6669 7420 2862 7569 6c74 2d69 6e20 636c  fit (built-in cl
+00008d90: 6173 7329 68e6 5500 4e74 7204 0600 0028  ass)h.U.Ntr....(
+00008da0: 6aba 0500 0058 2700 0000 6c73 7166 6974  j....X'...lsqfit
+00008db0: 2e67 736c 5f76 315f 6d75 6c74 6966 6974  .gsl_v1_multifit
+00008dc0: 2028 6275 696c 742d 696e 2063 6c61 7373   (built-in class
+00008dd0: 296a 1501 0000 5500 4e74 7205 0600 0028  )j....U.Ntr....(
+00008de0: 6aba 0500 0058 2600 0000 6c73 7166 6974  j....X&...lsqfit
+00008df0: 2e67 736c 5f6d 756c 7469 6d69 6e65 7820  .gsl_multiminex 
+00008e00: 2862 7569 6c74 2d69 6e20 636c 6173 7329  (built-in class)
+00008e10: 68b5 5500 4e74 7206 0600 0065 7555 0861  h.U.Ntr....euU.a
+00008e20: 6c6c 5f64 6f63 7372 0706 0000 7d72 0806  ll_docsr....}r..
+00008e30: 0000 2868 0c47 41d6 d2e4 f0ac 018e 6822  ..(h.GA.......h"
+00008e40: 4741 d6d2 e4f1 22ed 4e68 2b47 41d6 d2e4  GA....".Nh+GA...
+00008e50: f0f5 27bb 683d 4741 d6d2 e4f1 13f9 4d68  ..'.h=GA......Mh
+00008e60: 4647 41d6 d2e4 f097 aafc 684f 4741 d6d2  FGA.......hOGA..
+00008e70: e4f0 9c09 8168 5847 41d6 d2e4 f11d abcd  .....hXGA.......
+00008e80: 6868 4741 d6d2 e4f0 9e2a b768 7147 41d6  hhGA.....*.hqGA.
+00008e90: d2e4 f0a8 7875 7555 0873 6574 7469 6e67  ....xuuU.setting
+00008ea0: 7372 0906 0000 7d72 0a06 0000 2855 1563  sr....}r....(U.c
+00008eb0: 6c6f 616b 5f65 6d61 696c 5f61 6464 7265  loak_email_addre
+00008ec0: 7373 6573 720b 0600 0088 550c 7065 705f  ssesr.....U.pep_
+00008ed0: 6261 7365 5f75 726c 720c 0600 0055 2068  base_urlr....U h
+00008ee0: 7474 7073 3a2f 2f77 7777 2e70 7974 686f  ttps://www.pytho
+00008ef0: 6e2e 6f72 672f 6465 762f 7065 7073 2f72  n.org/dev/peps/r
+00008f00: 0d06 0000 550a 6861 6c74 5f6c 6576 656c  ....U.halt_level
+00008f10: 720e 0600 004b 0555 1273 6563 7473 7562  r....K.U.sectsub
+00008f20: 7469 746c 655f 7866 6f72 6d72 0f06 0000  title_xformr....
+00008f30: 8955 0c73 6d61 7274 5f71 756f 7465 7372  .U.smart_quotesr
+00008f40: 1006 0000 8855 0e69 6e70 7574 5f65 6e63  .....U.input_enc
+00008f50: 6f64 696e 6772 1106 0000 5509 7574 662d  odingr....U.utf-
+00008f60: 382d 7369 6772 1206 0000 550c 7266 635f  8-sigr....U.rfc_
+00008f70: 6261 7365 5f75 726c 7213 0600 0055 1c68  base_urlr....U.h
+00008f80: 7474 7073 3a2f 2f74 6f6f 6c73 2e69 6574  ttps://tools.iet
+00008f90: 662e 6f72 672f 6874 6d6c 2f72 1406 0000  f.org/html/r....
+00008fa0: 550e 7266 635f 7265 6665 7265 6e63 6573  U.rfc_references
+00008fb0: 7215 0600 004e 550e 7065 705f 7265 6665  r....NU.pep_refe
+00008fc0: 7265 6e63 6573 7216 0600 004e 550d 6c61  rencesr....NU.la
+00008fd0: 6e67 7561 6765 5f63 6f64 6572 1706 0000  nguage_coder....
+00008fe0: 5502 656e 7218 0600 0055 0e64 6f63 7469  U.enr....U.docti
+00008ff0: 746c 655f 7866 6f72 6d72 1906 0000 8955  tle_xformr.....U
+00009000: 1d74 7269 6d5f 666f 6f74 6e6f 7465 5f72  .trim_footnote_r
+00009010: 6566 6572 656e 6365 5f73 7061 6365 721a  eference_spacer.
+00009020: 0600 0089 5503 656e 7672 1b06 0000 6802  ....U.envr....h.
+00009030: 5513 736d 6172 7471 756f 7465 735f 6c6f  U.smartquotes_lo
+00009040: 6361 6c65 7372 1c06 0000 5d72 1d06 0000  calesr....]r....
+00009050: 5516 6669 6c65 5f69 6e73 6572 7469 6f6e  U.file_insertion
+00009060: 5f65 6e61 626c 6564 721e 0600 0088 550f  _enabledr.....U.
+00009070: 6765 7474 6578 745f 636f 6d70 6163 7472  gettext_compactr
+00009080: 1f06 0000 8855 1065 6d62 6564 5f73 7479  .....U.embed_sty
+00009090: 6c65 7368 6565 7472 2006 0000 8975 550b  lesheetr ....uU.
+000090a0: 7265 665f 636f 6e74 6578 7472 2106 0000  ref_contextr!...
+000090b0: 7d55 1066 696c 6573 5f74 6f5f 7265 6275  }U.files_to_rebu
+000090c0: 696c 6472 2206 0000 7d72 2306 0000 286a  ildr"...}r#...(j
+000090d0: 3c02 0000 6807 5d72 2406 0000 680c 6185  <...h.]r$...h.a.
+000090e0: 5272 2506 0000 6a37 0200 0068 075d 7226  Rr%...j7...h.]r&
+000090f0: 0600 0068 0c61 8552 7227 0600 006a 3802  ...h.a.Rr'...j8.
+00009100: 0000 6807 5d72 2806 0000 680c 6185 5272  ..h.]r(...h.a.Rr
+00009110: 2906 0000 6a3b 0200 0068 075d 722a 0600  )...j;...h.]r*..
+00009120: 0068 0c61 8552 722b 0600 006a 3e02 0000  .h.a.Rr+...j>...
+00009130: 6807 5d72 2c06 0000 680c 6185 5272 2d06  h.]r,...h.a.Rr-.
+00009140: 0000 6a3a 0200 0068 075d 722e 0600 0068  ..j:...h.]r....h
+00009150: 0c61 8552 722f 0600 006a 3902 0000 6807  .a.Rr/...j9...h.
+00009160: 5d72 3006 0000 680c 6185 5272 3106 0000  ]r0...h.a.Rr1...
+00009170: 6a3d 0200 0068 075d 7232 0600 0068 0c61  j=...h.]r2...h.a
+00009180: 8552 7233 0600 0075 550e 746f 635f 7365  .Rr3...uU.toc_se
+00009190: 636e 756d 6265 7273 7234 0600 007d 5512  cnumbersr4...}U.
+000091a0: 7665 7273 696f 6e69 6e67 5f63 6f6d 7061  versioning_compa
+000091b0: 7265 7235 0600 0089 550f 5f6e 6974 7069  rer5....U._nitpi
+000091c0: 636b 5f69 676e 6f72 6572 3606 0000 6807  ck_ignorer6...h.
+000091d0: 5d85 5272 3706 0000 7562 2e              ].Rr7...ub.
```

### Comparing `lsqfit-9.4/doc/html/.doctrees/index.doctree` & `lsqfit-9.5/doc/html/.doctrees/index.doctree`

 * *Files identical despite different names*

### Comparing `lsqfit-9.4/doc/html/.doctrees/case-outliers.doctree` & `lsqfit-9.5/doc/html/.doctrees/case-outliers.doctree`

 * *Files identical despite different names*

### Comparing `lsqfit-9.4/doc/html/.doctrees/scipy.doctree` & `lsqfit-9.5/doc/html/.doctrees/scipy.doctree`

 * *Files 2% similar despite different names*

```diff
@@ -716,3383 +716,3381 @@
 00002cb0: 8581 72fb 0100 007d 72fc 0100 0028 681e  ..r....}r....(h.
 00002cc0: 5500 681f 6ad9 0100 0075 6268 5258 2000  U.h.j....ubhRX .
 00002cd0: 0000 5374 6172 7469 6e67 2070 6f69 6e74  ..Starting point
 00002ce0: 2066 6f72 206d 696e 696d 697a 6174 696f   for minimizatio
 00002cf0: 6e2e 72fd 0100 0085 8172 fe01 0000 7d72  n.r......r....}r
 00002d00: ff01 0000 2868 1e58 2000 0000 5374 6172  ....(h.X ...Star
 00002d10: 7469 6e67 2070 6f69 6e74 2066 6f72 206d  ting point for m
-00002d20: 696e 696d 697a 6174 696f 6e2e 7200 0200  inimization.r...
-00002d30: 0068 234e 6831 4e68 3268 0268 1f6a d901  .h#Nh1Nh2h.h.j..
-00002d40: 0000 7562 6568 2568 9a75 6261 6825 5509  ..ubeh%h.ubah%U.
-00002d50: 6c69 7374 5f69 7465 6d72 0102 0000 7562  list_itemr....ub
-00002d60: 6ad4 0100 0029 8172 0202 0000 7d72 0302  j....).r....}r..
-00002d70: 0000 2868 1e55 0068 277d 7204 0200 0028  ..(h.U.h'}r....(
-00002d80: 6829 5d68 2a5d 682b 5d68 2c5d 682f 5d75  h)]h*]h+]h,]h/]u
-00002d90: 681f 6ad0 0100 0068 335d 7205 0200 0068  h.j....h3]r....h
-00002da0: 9729 8172 0602 0000 7d72 0702 0000 2868  .).r....}r....(h
-00002db0: 1e58 4700 0000 6e20 2870 6f73 6974 6976  .XG...n (positiv
-00002dc0: 6520 696e 7429 202d 2d20 4c65 6e67 7468  e int) -- Length
-00002dd0: 206f 6620 7665 6374 6f72 2072 6574 7572   of vector retur
-00002de0: 6e65 6420 6279 2074 6865 2066 6974 2066  ned by the fit f
-00002df0: 756e 6374 696f 6e20 6628 7829 2e68 277d  unction f(x).h'}
-00002e00: 7208 0200 0028 6829 5d68 2a5d 682b 5d68  r....(h)]h*]h+]h
-00002e10: 2c5d 682f 5d75 681f 6a02 0200 0068 335d  ,]h/]uh.j....h3]
-00002e20: 7209 0200 0028 6add 0100 0029 8172 0a02  r....(j....).r..
-00002e30: 0000 7d72 0b02 0000 2868 1e58 0100 0000  ..}r....(h.X....
-00002e40: 6e68 277d 720c 0200 0028 682c 5d68 2b5d  nh'}r....(h,]h+]
-00002e50: 6ae1 0100 0088 6829 5d68 2a5d 682f 5d75  j.....h)]h*]h/]u
-00002e60: 681f 6a06 0200 0068 335d 720d 0200 0068  h.j....h3]r....h
-00002e70: 5258 0100 0000 6e85 8172 0e02 0000 7d72  RX....n..r....}r
-00002e80: 0f02 0000 2868 1e55 0068 1f6a 0a02 0000  ....(h.U.h.j....
-00002e90: 7562 6168 256a e601 0000 7562 6852 5802  ubah%j....ubhRX.
-00002ea0: 0000 0020 2872 1002 0000 8581 7211 0200  ... (r......r...
-00002eb0: 007d 7212 0200 0028 681e 5500 681f 6a06  .}r....(h.U.h.j.
-00002ec0: 0200 0075 6268 3c29 8172 1302 0000 7d72  ...ubh<).r....}r
-00002ed0: 1402 0000 2868 1e55 0068 277d 7215 0200  ....(h.U.h'}r...
-00002ee0: 0028 5507 7265 6674 7970 6568 f26a e101  .(U.reftypeh.j..
-00002ef0: 0000 8855 0972 6566 7461 7267 6574 580c  ...U.reftargetX.
-00002f00: 0000 0070 6f73 6974 6976 6520 696e 7472  ...positive intr
-00002f10: 1602 0000 5509 7265 6664 6f6d 6169 6e68  ....U.refdomainh
-00002f20: de68 2c5d 682b 5d55 0b72 6566 6578 706c  .h,]h+]U.refexpl
-00002f30: 6963 6974 8968 295d 682a 5d68 2f5d 7568  icit.h)]h*]h/]uh
-00002f40: 1f6a 0602 0000 6833 5d72 1702 0000 6aef  .j....h3]r....j.
-00002f50: 0100 0029 8172 1802 0000 7d72 1902 0000  ...).r....}r....
-00002f60: 2868 1e6a 1602 0000 6827 7d72 1a02 0000  (h.j....h'}r....
-00002f70: 2868 295d 682a 5d68 2b5d 682c 5d68 2f5d  (h)]h*]h+]h,]h/]
-00002f80: 7568 1f6a 1302 0000 6833 5d72 1b02 0000  uh.j....h3]r....
-00002f90: 6852 580c 0000 0070 6f73 6974 6976 6520  hRX....positive 
-00002fa0: 696e 7472 1c02 0000 8581 721d 0200 007d  intr......r....}
-00002fb0: 721e 0200 0028 681e 5500 681f 6a18 0200  r....(h.U.h.j...
-00002fc0: 0075 6261 6825 6af7 0100 0075 6261 6825  .ubah%j....ubah%
-00002fd0: 6840 7562 6852 5801 0000 0029 8581 721f  h@ubhRX....)..r.
-00002fe0: 0200 007d 7220 0200 0028 681e 5500 681f  ...}r ...(h.U.h.
-00002ff0: 6a06 0200 0075 6268 5258 0500 0000 20e2  j....ubhRX.... .
-00003000: 8093 2072 2102 0000 8581 7222 0200 007d  .. r!.....r"...}
-00003010: 7223 0200 0028 681e 5500 681f 6a06 0200  r#...(h.U.h.j...
-00003020: 0075 6268 5258 2e00 0000 4c65 6e67 7468  .ubhRX....Length
-00003030: 206f 6620 7665 6374 6f72 2072 6574 7572   of vector retur
-00003040: 6e65 6420 6279 2074 6865 2066 6974 2066  ned by the fit f
-00003050: 756e 6374 696f 6e20 7224 0200 0085 8172  unction r$.....r
-00003060: 2502 0000 7d72 2602 0000 2868 1e58 2e00  %...}r&...(h.X..
-00003070: 0000 4c65 6e67 7468 206f 6620 7665 6374  ..Length of vect
-00003080: 6f72 2072 6574 7572 6e65 6420 6279 2074  or returned by t
-00003090: 6865 2066 6974 2066 756e 6374 696f 6e20  he fit function 
-000030a0: 7227 0200 0068 234e 6831 4e68 3268 0268  r'...h#Nh1Nh2h.h
-000030b0: 1f6a 0602 0000 7562 684a 2981 7228 0200  .j....ubhJ).r(..
-000030c0: 007d 7229 0200 0028 681e 5808 0000 0060  .}r)...(h.X....`
-000030d0: 6066 2878 2960 6068 1f6a 0602 0000 6823  `f(x)``h.j....h#
-000030e0: 4e68 2568 5668 277d 722a 0200 0028 6829  Nh%hVh'}r*...(h)
-000030f0: 5d68 2a5d 682b 5d68 2c5d 682f 5d75 6831  ]h*]h+]h,]h/]uh1
-00003100: 4e68 3268 0268 335d 722b 0200 0068 5258  Nh2h.h3]r+...hRX
-00003110: 0400 0000 6628 7829 722c 0200 0085 8172  ....f(x)r,.....r
-00003120: 2d02 0000 7d72 2e02 0000 2868 1e55 0068  -...}r....(h.U.h
-00003130: 234e 6831 4e68 3268 0268 1f6a 2802 0000  #Nh1Nh2h.h.j(...
-00003140: 7562 6175 6268 5258 0100 0000 2e85 8172  ubaubhRX.......r
-00003150: 2f02 0000 7d72 3002 0000 2868 1e58 0100  /...}r0...(h.X..
-00003160: 0000 2e68 234e 6831 4e68 3268 0268 1f6a  ...h#Nh1Nh2h.h.j
-00003170: 0602 0000 7562 6568 2568 9a75 6261 6825  ....ubeh%h.ubah%
-00003180: 6a01 0200 0075 626a d401 0000 2981 7231  j....ubj....).r1
-00003190: 0200 007d 7232 0200 0028 681e 5500 6827  ...}r2...(h.U.h'
-000031a0: 7d72 3302 0000 2868 295d 682a 5d68 2b5d  }r3...(h)]h*]h+]
-000031b0: 682c 5d68 2f5d 7568 1f6a d001 0000 6833  h,]h/]uh.j....h3
-000031c0: 5d72 3402 0000 6897 2981 7235 0200 007d  ]r4...h.).r5...}
-000031d0: 7236 0200 0028 681e 5898 0000 0066 2028  r6...(h.X....f (
-000031e0: 6172 7261 792d 7661 6c75 6564 2066 756e  array-valued fun
-000031f0: 6374 696f 6e29 202d 2d20 7375 6d5f 6920  ction) -- sum_i 
-00003200: 665f 6928 7829 2a2a 3220 6973 206d 696e  f_i(x)**2 is min
-00003210: 696d 697a 6564 0a62 7920 7661 7279 696e  imized.by varyin
-00003220: 6720 7061 7261 6d65 7465 7273 2078 2e20  g parameters x. 
-00003230: 5468 6520 7061 7261 6d65 7465 7273 2061  The parameters a
-00003240: 7265 2061 2031 2d64 0a6e 756d 7079 2061  re a 1-d.numpy a
-00003250: 7272 6179 206f 6620 6569 7468 6572 206e  rray of either n
-00003260: 756d 6265 7273 206f 7220 6776 6172 2e47  umbers or gvar.G
-00003270: 5661 7273 2e68 277d 7237 0200 0028 6829  Vars.h'}r7...(h)
-00003280: 5d68 2a5d 682b 5d68 2c5d 682f 5d75 681f  ]h*]h+]h,]h/]uh.
-00003290: 6a31 0200 0068 335d 7238 0200 0028 6add  j1...h3]r8...(j.
-000032a0: 0100 0029 8172 3902 0000 7d72 3a02 0000  ...).r9...}r:...
-000032b0: 2868 1e58 0100 0000 6668 277d 723b 0200  (h.X....fh'}r;..
-000032c0: 0028 682c 5d68 2b5d 6ae1 0100 0088 6829  .(h,]h+]j.....h)
-000032d0: 5d68 2a5d 682f 5d75 681f 6a35 0200 0068  ]h*]h/]uh.j5...h
-000032e0: 335d 723c 0200 0068 5258 0100 0000 6685  3]r<...hRX....f.
-000032f0: 8172 3d02 0000 7d72 3e02 0000 2868 1e55  .r=...}r>...(h.U
-00003300: 0068 1f6a 3902 0000 7562 6168 256a e601  .h.j9...ubah%j..
-00003310: 0000 7562 6852 5802 0000 0020 2872 3f02  ..ubhRX.... (r?.
-00003320: 0000 8581 7240 0200 007d 7241 0200 0028  ....r@...}rA...(
-00003330: 681e 5500 681f 6a35 0200 0075 6268 3c29  h.U.h.j5...ubh<)
-00003340: 8172 4202 0000 7d72 4302 0000 2868 1e55  .rB...}rC...(h.U
-00003350: 0068 277d 7244 0200 0028 5507 7265 6674  .h'}rD...(U.reft
-00003360: 7970 6568 f26a e101 0000 8855 0972 6566  ypeh.j.....U.ref
-00003370: 7461 7267 6574 5815 0000 0061 7272 6179  targetX....array
-00003380: 2d76 616c 7565 6420 6675 6e63 7469 6f6e  -valued function
-00003390: 7245 0200 0055 0972 6566 646f 6d61 696e  rE...U.refdomain
-000033a0: 68de 682c 5d68 2b5d 550b 7265 6665 7870  h.h,]h+]U.refexp
-000033b0: 6c69 6369 7489 6829 5d68 2a5d 682f 5d75  licit.h)]h*]h/]u
-000033c0: 681f 6a35 0200 0068 335d 7246 0200 006a  h.j5...h3]rF...j
-000033d0: ef01 0000 2981 7247 0200 007d 7248 0200  ....).rG...}rH..
-000033e0: 0028 681e 6a45 0200 0068 277d 7249 0200  .(h.jE...h'}rI..
-000033f0: 0028 6829 5d68 2a5d 682b 5d68 2c5d 682f  .(h)]h*]h+]h,]h/
-00003400: 5d75 681f 6a42 0200 0068 335d 724a 0200  ]uh.jB...h3]rJ..
-00003410: 0068 5258 1500 0000 6172 7261 792d 7661  .hRX....array-va
-00003420: 6c75 6564 2066 756e 6374 696f 6e72 4b02  lued functionrK.
-00003430: 0000 8581 724c 0200 007d 724d 0200 0028  ....rL...}rM...(
-00003440: 681e 5500 681f 6a47 0200 0075 6261 6825  h.U.h.jG...ubah%
-00003450: 6af7 0100 0075 6261 6825 6840 7562 6852  j....ubah%h@ubhR
-00003460: 5801 0000 0029 8581 724e 0200 007d 724f  X....)..rN...}rO
-00003470: 0200 0028 681e 5500 681f 6a35 0200 0075  ...(h.U.h.j5...u
-00003480: 6268 5258 0500 0000 20e2 8093 2072 5002  bhRX.... ... rP.
-00003490: 0000 8581 7251 0200 007d 7252 0200 0028  ....rQ...}rR...(
-000034a0: 681e 5500 681f 6a35 0200 0075 6268 4a29  h.U.h.j5...ubhJ)
-000034b0: 8172 5302 0000 7d72 5402 0000 2868 1e58  .rS...}rT...(h.X
-000034c0: 1300 0000 6060 7375 6d5f 6920 665f 6928  ....``sum_i f_i(
-000034d0: 7829 2a2a 3260 6068 1f6a 3502 0000 6823  x)**2``h.j5...h#
-000034e0: 4e68 2568 5668 277d 7255 0200 0028 6829  Nh%hVh'}rU...(h)
-000034f0: 5d68 2a5d 682b 5d68 2c5d 682f 5d75 6831  ]h*]h+]h,]h/]uh1
-00003500: 4e68 3268 0268 335d 7256 0200 0068 5258  Nh2h.h3]rV...hRX
-00003510: 0f00 0000 7375 6d5f 6920 665f 6928 7829  ....sum_i f_i(x)
-00003520: 2a2a 3272 5702 0000 8581 7258 0200 007d  **2rW.....rX...}
-00003530: 7259 0200 0028 681e 5500 6823 4e68 314e  rY...(h.U.h#Nh1N
-00003540: 6832 6802 681f 6a53 0200 0075 6261 7562  h2h.h.jS...ubaub
-00003550: 6852 5824 0000 0020 6973 206d 696e 696d  hRX$... is minim
-00003560: 697a 6564 0a62 7920 7661 7279 696e 6720  ized.by varying 
-00003570: 7061 7261 6d65 7465 7273 2072 5a02 0000  parameters rZ...
-00003580: 8581 725b 0200 007d 725c 0200 0028 681e  ..r[...}r\...(h.
-00003590: 5824 0000 0020 6973 206d 696e 696d 697a  X$... is minimiz
-000035a0: 6564 0a62 7920 7661 7279 696e 6720 7061  ed.by varying pa
-000035b0: 7261 6d65 7465 7273 2072 5d02 0000 6823  rameters r]...h#
-000035c0: 4e68 314e 6832 6802 681f 6a35 0200 0075  Nh1Nh2h.h.j5...u
-000035d0: 6268 4a29 8172 5e02 0000 7d72 5f02 0000  bhJ).r^...}r_...
-000035e0: 2868 1e58 0500 0000 6060 7860 6068 1f6a  (h.X....``x``h.j
-000035f0: 3502 0000 6823 4e68 2568 5668 277d 7260  5...h#Nh%hVh'}r`
-00003600: 0200 0028 6829 5d68 2a5d 682b 5d68 2c5d  ...(h)]h*]h+]h,]
-00003610: 682f 5d75 6831 4e68 3268 0268 335d 7261  h/]uh1Nh2h.h3]ra
-00003620: 0200 0068 5258 0100 0000 7885 8172 6202  ...hRX....x..rb.
-00003630: 0000 7d72 6302 0000 2868 1e55 0068 234e  ..}rc...(h.U.h#N
-00003640: 6831 4e68 3268 0268 1f6a 5e02 0000 7562  h1Nh2h.h.j^...ub
-00003650: 6175 6268 5258 1b00 0000 2e20 5468 6520  aubhRX..... The 
-00003660: 7061 7261 6d65 7465 7273 2061 7265 2061  parameters are a
-00003670: 2031 2d64 0a72 6402 0000 8581 7265 0200   1-d.rd.....re..
-00003680: 007d 7266 0200 0028 681e 581b 0000 002e  .}rf...(h.X.....
-00003690: 2054 6865 2070 6172 616d 6574 6572 7320   The parameters 
-000036a0: 6172 6520 6120 312d 640a 7267 0200 0068  are a 1-d.rg...h
-000036b0: 234e 6831 4e68 3268 0268 1f6a 3502 0000  #Nh1Nh2h.h.j5...
-000036c0: 7562 683c 2981 7268 0200 007d 7269 0200  ubh<).rh...}ri..
-000036d0: 0028 681e 580e 0000 003a 636c 6173 733a  .(h.X....:class:
-000036e0: 606e 756d 7079 6072 6a02 0000 681f 6a35  `numpy`rj...h.j5
-000036f0: 0200 0068 236a 5901 0000 6825 6840 6827  ...h#jY...h%h@h'
-00003700: 7d72 6b02 0000 2855 0772 6566 7479 7065  }rk...(U.reftype
-00003710: 5805 0000 0063 6c61 7373 6842 8968 4358  X....classhB.hCX
-00003720: 0500 0000 6e75 6d70 7955 0972 6566 646f  ....numpyU.refdo
-00003730: 6d61 696e 5802 0000 0070 7972 6c02 0000  mainX....pyrl...
-00003740: 682c 5d68 2b5d 550b 7265 6665 7870 6c69  h,]h+]U.refexpli
-00003750: 6369 7489 6829 5d68 2a5d 682f 5d68 4568  cit.h)]h*]h/]hEh
-00003760: 4668 4768 f168 4868 ed75 6831 4b0d 6832  FhGh.hHh.uh1K.h2
-00003770: 6802 6833 5d72 6d02 0000 684a 2981 726e  h.h3]rm...hJ).rn
-00003780: 0200 007d 726f 0200 0028 681e 6a6a 0200  ...}ro...(h.jj..
-00003790: 0068 277d 7270 0200 0028 6829 5d68 2a5d  .h'}rp...(h)]h*]
-000037a0: 7271 0200 0028 684f 6a6c 0200 0058 0800  rq...(hOjl...X..
-000037b0: 0000 7079 2d63 6c61 7373 7272 0200 0065  ..py-classrr...e
-000037c0: 682b 5d68 2c5d 682f 5d75 681f 6a68 0200  h+]h,]h/]uh.jh..
-000037d0: 0068 335d 7273 0200 0068 5258 0500 0000  .h3]rs...hRX....
-000037e0: 6e75 6d70 7972 7402 0000 8581 7275 0200  numpyrt.....ru..
-000037f0: 007d 7276 0200 0028 681e 5500 681f 6a6e  .}rv...(h.U.h.jn
-00003800: 0200 0075 6261 6825 6856 7562 6175 6268  ...ubah%hVubaubh
-00003810: 5258 1c00 0000 2061 7272 6179 206f 6620  RX.... array of 
-00003820: 6569 7468 6572 206e 756d 6265 7273 206f  either numbers o
-00003830: 7220 7277 0200 0085 8172 7802 0000 7d72  r rw.....rx...}r
-00003840: 7902 0000 2868 1e58 1c00 0000 2061 7272  y...(h.X.... arr
-00003850: 6179 206f 6620 6569 7468 6572 206e 756d  ay of either num
-00003860: 6265 7273 206f 7220 727a 0200 0068 234e  bers or rz...h#N
-00003870: 6831 4e68 3268 0268 1f6a 3502 0000 7562  h1Nh2h.h.j5...ub
-00003880: 683c 2981 727b 0200 007d 727c 0200 0028  h<).r{...}r|...(
-00003890: 681e 5812 0000 003a 636c 6173 733a 6067  h.X....:class:`g
-000038a0: 7661 722e 4756 6172 6072 7d02 0000 681f  var.GVar`r}...h.
-000038b0: 6a35 0200 0068 236a 5901 0000 6825 6840  j5...h#jY...h%h@
-000038c0: 6827 7d72 7e02 0000 2855 0772 6566 7479  h'}r~...(U.refty
-000038d0: 7065 5805 0000 0063 6c61 7373 6842 8968  peX....classhB.h
-000038e0: 4358 0900 0000 6776 6172 2e47 5661 7255  CX....gvar.GVarU
-000038f0: 0972 6566 646f 6d61 696e 5802 0000 0070  .refdomainX....p
-00003900: 7972 7f02 0000 682c 5d68 2b5d 550b 7265  yr....h,]h+]U.re
-00003910: 6665 7870 6c69 6369 7489 6829 5d68 2a5d  fexplicit.h)]h*]
-00003920: 682f 5d68 4568 4668 4768 f168 4868 ed75  h/]hEhFhGh.hHh.u
-00003930: 6831 4b0d 6832 6802 6833 5d72 8002 0000  h1K.h2h.h3]r....
-00003940: 684a 2981 7281 0200 007d 7282 0200 0028  hJ).r....}r....(
-00003950: 681e 6a7d 0200 0068 277d 7283 0200 0028  h.j}...h'}r....(
-00003960: 6829 5d68 2a5d 7284 0200 0028 684f 6a7f  h)]h*]r....(hOj.
-00003970: 0200 0058 0800 0000 7079 2d63 6c61 7373  ...X....py-class
-00003980: 7285 0200 0065 682b 5d68 2c5d 682f 5d75  r....eh+]h,]h/]u
-00003990: 681f 6a7b 0200 0068 335d 7286 0200 0068  h.j{...h3]r....h
-000039a0: 5258 0900 0000 6776 6172 2e47 5661 7272  RX....gvar.GVarr
-000039b0: 8702 0000 8581 7288 0200 007d 7289 0200  ......r....}r...
-000039c0: 0028 681e 5500 681f 6a81 0200 0075 6261  .(h.U.h.j....uba
-000039d0: 6825 6856 7562 6175 6268 5258 0200 0000  h%hVubaubhRX....
-000039e0: 732e 728a 0200 0085 8172 8b02 0000 7d72  s.r......r....}r
-000039f0: 8c02 0000 2868 1e58 0300 0000 5c73 2e72  ....(h.X....\s.r
-00003a00: 8d02 0000 6823 4e68 314e 6832 6802 681f  ....h#Nh1Nh2h.h.
-00003a10: 6a35 0200 0075 6265 6825 689a 7562 6168  j5...ubeh%h.ubah
-00003a20: 256a 0102 0000 7562 6ad4 0100 0029 8172  %j....ubj....).r
-00003a30: 8e02 0000 7d72 8f02 0000 2868 1e55 0068  ....}r....(h.U.h
-00003a40: 277d 7290 0200 0028 6829 5d68 2a5d 682b  '}r....(h)]h*]h+
-00003a50: 5d68 2c5d 682f 5d75 681f 6ad0 0100 0068  ]h,]h/]uh.j....h
-00003a60: 335d 7291 0200 0068 9729 8172 9202 0000  3]r....h.).r....
-00003a70: 7d72 9302 0000 2868 1e58 b102 0000 746f  }r....(h.X....to
-00003a80: 6c20 2866 6c6f 6174 206f 7220 7475 706c  l (float or tupl
-00003a90: 6529 202d 2d20 4173 7369 676e 696e 6720  e) -- Assigning 
-00003aa0: 746f 6c3d 2878 746f 6c2c 2067 746f 6c2c  tol=(xtol, gtol,
-00003ab0: 2066 746f 6c29 2063 6175 7365 7320 7468   ftol) causes th
-00003ac0: 650a 6669 7420 746f 2073 746f 7020 7365  e.fit to stop se
-00003ad0: 6172 6368 696e 6720 666f 7220 6120 6d69  arching for a mi
-00003ae0: 6e69 6d75 6d20 7768 656e 2061 6e79 206f  nimum when any o
-00003af0: 6678 746f 6c20 3e3d 2072 656c 6174 6976  fxtol >= relativ
-00003b00: 6520 6368 616e 6765 2069 6e20 7061 7261  e change in para
-00003b10: 6d65 7465 7273 2062 6574 7765 656e 2069  meters between i
-00003b20: 7465 7261 7469 6f6e 730a 0a67 746f 6c20  terations..gtol 
-00003b30: 3e3d 2072 656c 6174 6976 6520 7369 7a65  >= relative size
-00003b40: 206f 6620 6772 6164 6965 6e74 206f 6620   of gradient of 
-00003b50: 6368 692a 2a32 0a0a 6674 6f6c 203e 3d20  chi**2..ftol >= 
-00003b60: 7265 6c61 7469 7665 2063 6861 6e67 6520  relative change 
-00003b70: 696e 2063 6869 2a2a 3220 6265 7477 6565  in chi**2 betwee
-00003b80: 6e20 6974 6572 6174 696f 6e73 6973 2073  n iterationsis s
-00003b90: 7461 7469 7366 6965 642e 2053 6565 2074  tatisfied. See t
-00003ba0: 6865 2073 6369 7079 2e6f 7074 696d 697a  he scipy.optimiz
-00003bb0: 652e 6c65 6173 745f 7371 7561 7265 730a  e.least_squares.
-00003bc0: 646f 6375 6d65 6e74 6174 696f 6e20 6465  documentation de
-00003bd0: 7461 696c 6564 2064 6566 696e 6974 696f  tailed definitio
-00003be0: 6e73 206f 6620 7468 6520 7374 6f70 7069  ns of the stoppi
-00003bf0: 6e67 2063 6f6e 6469 7469 6f6e 732e 0a54  ng conditions..T
-00003c00: 7970 6963 616c 6c79 206f 6e65 2073 6574  ypically one set
-00003c10: 7320 7874 6f6c 3d31 2f31 302a 2a64 2077  s xtol=1/10**d w
-00003c20: 6865 7265 2064 2069 7320 7468 6520 6e75  here d is the nu
-00003c30: 6d62 6572 206f 660a 6469 6769 7473 206f  mber of.digits o
-00003c40: 6620 7072 6563 6973 696f 6e20 6465 7369  f precision desi
-00003c50: 7265 6420 696e 2074 6865 2072 6573 756c  red in the resul
-00003c60: 742c 2077 6869 6c65 2067 746f 6c3c 3c31  t, while gtol<<1
-00003c70: 2061 6e64 0a66 746f 6c3c 3c31 2e20 5365   and.ftol<<1. Se
-00003c80: 7474 696e 6720 746f 6c3d 6570 7320 7768  tting tol=eps wh
-00003c90: 6572 6520 6570 7320 6973 2061 206e 756d  ere eps is a num
-00003ca0: 6265 7220 6973 0a65 7175 6976 616c 656e  ber is.equivalen
-00003cb0: 7420 746f 2073 6574 7469 6e67 2074 6f6c  t to setting tol
-00003cc0: 3d28 6570 732c 3165 2d31 302c 3165 2d31  =(eps,1e-10,1e-1
-00003cd0: 3029 2e20 5365 7474 696e 670a 746f 6c3d  0). Setting.tol=
-00003ce0: 2865 7073 312c 6570 7332 2920 6973 2065  (eps1,eps2) is e
-00003cf0: 7175 6976 6c65 6e74 2074 6f20 7365 7474  quivlent to sett
-00003d00: 696e 670a 746f 6c3d 2865 7073 312c 6570  ing.tol=(eps1,ep
-00003d10: 7332 2c31 652d 3130 292e 2044 6566 6175  s2,1e-10). Defau
-00003d20: 6c74 2069 7320 746f 6c3d 3165 2d35 2e68  lt is tol=1e-5.h
-00003d30: 277d 7294 0200 0028 6829 5d68 2a5d 682b  '}r....(h)]h*]h+
-00003d40: 5d68 2c5d 682f 5d75 681f 6a8e 0200 0068  ]h,]h/]uh.j....h
-00003d50: 335d 7295 0200 0028 6add 0100 0029 8172  3]r....(j....).r
-00003d60: 9602 0000 7d72 9702 0000 2868 1e58 0300  ....}r....(h.X..
-00003d70: 0000 746f 6c68 277d 7298 0200 0028 682c  ..tolh'}r....(h,
-00003d80: 5d68 2b5d 6ae1 0100 0088 6829 5d68 2a5d  ]h+]j.....h)]h*]
-00003d90: 682f 5d75 681f 6a92 0200 0068 335d 7299  h/]uh.j....h3]r.
-00003da0: 0200 0068 5258 0300 0000 746f 6c72 9a02  ...hRX....tolr..
-00003db0: 0000 8581 729b 0200 007d 729c 0200 0028  ....r....}r....(
-00003dc0: 681e 5500 681f 6a96 0200 0075 6261 6825  h.U.h.j....ubah%
-00003dd0: 6ae6 0100 0075 6268 5258 0200 0000 2028  j....ubhRX.... (
-00003de0: 729d 0200 0085 8172 9e02 0000 7d72 9f02  r......r....}r..
-00003df0: 0000 2868 1e55 0068 1f6a 9202 0000 7562  ..(h.U.h.j....ub
-00003e00: 683c 2981 72a0 0200 007d 72a1 0200 0028  h<).r....}r....(
-00003e10: 681e 5500 6827 7d72 a202 0000 2855 0772  h.U.h'}r....(U.r
-00003e20: 6566 7479 7065 68f2 6ae1 0100 0088 5509  eftypeh.j.....U.
-00003e30: 7265 6674 6172 6765 7458 0500 0000 666c  reftargetX....fl
-00003e40: 6f61 7472 a302 0000 5509 7265 6664 6f6d  oatr....U.refdom
-00003e50: 6169 6e68 de68 2c5d 682b 5d55 0b72 6566  ainh.h,]h+]U.ref
-00003e60: 6578 706c 6963 6974 8968 295d 682a 5d68  explicit.h)]h*]h
-00003e70: 2f5d 7568 1f6a 9202 0000 6833 5d72 a402  /]uh.j....h3]r..
-00003e80: 0000 6aef 0100 0029 8172 a502 0000 7d72  ..j....).r....}r
-00003e90: a602 0000 2868 1e6a a302 0000 6827 7d72  ....(h.j....h'}r
-00003ea0: a702 0000 2868 295d 682a 5d68 2b5d 682c  ....(h)]h*]h+]h,
-00003eb0: 5d68 2f5d 7568 1f6a a002 0000 6833 5d72  ]h/]uh.j....h3]r
-00003ec0: a802 0000 6852 5805 0000 0066 6c6f 6174  ....hRX....float
-00003ed0: 72a9 0200 0085 8172 aa02 0000 7d72 ab02  r......r....}r..
-00003ee0: 0000 2868 1e55 0068 1f6a a502 0000 7562  ..(h.U.h.j....ub
-00003ef0: 6168 256a f701 0000 7562 6168 2568 4075  ah%j....ubah%h@u
-00003f00: 626a ef01 0000 2981 72ac 0200 007d 72ad  bj....).r....}r.
-00003f10: 0200 0028 681e 5804 0000 0020 6f72 2068  ...(h.X.... or h
-00003f20: 277d 72ae 0200 0028 6829 5d68 2a5d 682b  '}r....(h)]h*]h+
-00003f30: 5d68 2c5d 682f 5d75 681f 6a92 0200 0068  ]h,]h/]uh.j....h
-00003f40: 335d 72af 0200 0068 5258 0400 0000 206f  3]r....hRX.... o
-00003f50: 7220 72b0 0200 0085 8172 b102 0000 7d72  r r......r....}r
-00003f60: b202 0000 2868 1e55 0068 1f6a ac02 0000  ....(h.U.h.j....
-00003f70: 7562 6168 256a f701 0000 7562 683c 2981  ubah%j....ubh<).
-00003f80: 72b3 0200 007d 72b4 0200 0028 681e 5500  r....}r....(h.U.
-00003f90: 6827 7d72 b502 0000 2855 0772 6566 7479  h'}r....(U.refty
-00003fa0: 7065 68f2 6ae1 0100 0088 5509 7265 6674  peh.j.....U.reft
-00003fb0: 6172 6765 7458 0500 0000 7475 706c 6572  argetX....tupler
-00003fc0: b602 0000 5509 7265 6664 6f6d 6169 6e68  ....U.refdomainh
-00003fd0: de68 2c5d 682b 5d55 0b72 6566 6578 706c  .h,]h+]U.refexpl
-00003fe0: 6963 6974 8968 295d 682a 5d68 2f5d 7568  icit.h)]h*]h/]uh
-00003ff0: 1f6a 9202 0000 6833 5d72 b702 0000 6aef  .j....h3]r....j.
-00004000: 0100 0029 8172 b802 0000 7d72 b902 0000  ...).r....}r....
-00004010: 2868 1e6a b602 0000 6827 7d72 ba02 0000  (h.j....h'}r....
-00004020: 2868 295d 682a 5d68 2b5d 682c 5d68 2f5d  (h)]h*]h+]h,]h/]
-00004030: 7568 1f6a b302 0000 6833 5d72 bb02 0000  uh.j....h3]r....
-00004040: 6852 5805 0000 0074 7570 6c65 72bc 0200  hRX....tupler...
-00004050: 0085 8172 bd02 0000 7d72 be02 0000 2868  ...r....}r....(h
-00004060: 1e55 0068 1f6a b802 0000 7562 6168 256a  .U.h.j....ubah%j
-00004070: f701 0000 7562 6168 2568 4075 6268 5258  ....ubah%h@ubhRX
-00004080: 0100 0000 2985 8172 bf02 0000 7d72 c002  ....)..r....}r..
-00004090: 0000 2868 1e55 0068 1f6a 9202 0000 7562  ..(h.U.h.j....ub
-000040a0: 6852 5805 0000 0020 e280 9320 72c1 0200  hRX.... ... r...
-000040b0: 0085 8172 c202 0000 7d72 c302 0000 2868  ...r....}r....(h
-000040c0: 1e55 0068 1f6a 9202 0000 7562 6897 2981  .U.h.j....ubh.).
-000040d0: 72c4 0200 007d 72c5 0200 0028 681e 585f  r....}r....(h.X_
-000040e0: 0000 0041 7373 6967 6e69 6e67 2060 6074  ...Assigning ``t
-000040f0: 6f6c 3d28 7874 6f6c 2c20 6774 6f6c 2c20  ol=(xtol, gtol, 
-00004100: 6674 6f6c 2960 6020 6361 7573 6573 2074  ftol)`` causes t
-00004110: 6865 0a66 6974 2074 6f20 7374 6f70 2073  he.fit to stop s
-00004120: 6561 7263 6869 6e67 2066 6f72 2061 206d  earching for a m
-00004130: 696e 696d 756d 2077 6865 6e20 616e 7920  inimum when any 
-00004140: 6f66 681f 6a92 0200 0068 236a 5901 0000  ofh.j....h#jY...
-00004150: 6825 689a 6827 7d72 c602 0000 2868 295d  h%h.h'}r....(h)]
-00004160: 682a 5d68 2b5d 682c 5d68 2f5d 7568 314b  h*]h+]h,]h/]uh1K
-00004170: 1168 3268 0268 335d 72c7 0200 0028 6852  .h2h.h3]r....(hR
-00004180: 580a 0000 0041 7373 6967 6e69 6e67 2072  X....Assigning r
-00004190: c802 0000 8581 72c9 0200 007d 72ca 0200  ......r....}r...
-000041a0: 0028 681e 580a 0000 0041 7373 6967 6e69  .(h.X....Assigni
-000041b0: 6e67 2068 234e 6831 4e68 3268 0268 1f6a  ng h#Nh1Nh2h.h.j
-000041c0: c402 0000 7562 684a 2981 72cb 0200 007d  ....ubhJ).r....}
-000041d0: 72cc 0200 0028 681e 581a 0000 0060 6074  r....(h.X....``t
-000041e0: 6f6c 3d28 7874 6f6c 2c20 6774 6f6c 2c20  ol=(xtol, gtol, 
-000041f0: 6674 6f6c 2960 6068 277d 72cd 0200 0028  ftol)``h'}r....(
-00004200: 6829 5d68 2a5d 682b 5d68 2c5d 682f 5d75  h)]h*]h+]h,]h/]u
-00004210: 681f 6ac4 0200 0068 335d 72ce 0200 0068  h.j....h3]r....h
-00004220: 5258 1600 0000 746f 6c3d 2878 746f 6c2c  RX....tol=(xtol,
-00004230: 2067 746f 6c2c 2066 746f 6c29 72cf 0200   gtol, ftol)r...
-00004240: 0085 8172 d002 0000 7d72 d102 0000 2868  ...r....}r....(h
-00004250: 1e55 0068 1f6a cb02 0000 7562 6168 2568  .U.h.j....ubah%h
-00004260: 5675 6268 5258 3b00 0000 2063 6175 7365  VubhRX;... cause
-00004270: 7320 7468 650a 6669 7420 746f 2073 746f  s the.fit to sto
-00004280: 7020 7365 6172 6368 696e 6720 666f 7220  p searching for 
-00004290: 6120 6d69 6e69 6d75 6d20 7768 656e 2061  a minimum when a
-000042a0: 6e79 206f 6672 d202 0000 8581 72d3 0200  ny ofr......r...
-000042b0: 007d 72d4 0200 0028 681e 583b 0000 0020  .}r....(h.X;... 
-000042c0: 6361 7573 6573 2074 6865 0a66 6974 2074  causes the.fit t
-000042d0: 6f20 7374 6f70 2073 6561 7263 6869 6e67  o stop searching
-000042e0: 2066 6f72 2061 206d 696e 696d 756d 2077   for a minimum w
-000042f0: 6865 6e20 616e 7920 6f66 6823 4e68 314e  hen any ofh#Nh1N
-00004300: 6832 6802 681f 6ac4 0200 0075 6265 7562  h2h.h.j....ubeub
-00004310: 6364 6f63 7574 696c 732e 6e6f 6465 730a  cdocutils.nodes.
-00004320: 626c 6f63 6b5f 7175 6f74 650a 72d5 0200  block_quote.r...
-00004330: 0029 8172 d602 0000 7d72 d702 0000 2868  .).r....}r....(h
-00004340: 1e55 0068 1f6a 9202 0000 6823 4e68 2555  .U.h.j....h#Nh%U
-00004350: 0b62 6c6f 636b 5f71 756f 7465 72d8 0200  .block_quoter...
-00004360: 0068 277d 72d9 0200 0028 6829 5d68 2a5d  .h'}r....(h)]h*]
-00004370: 682b 5d68 2c5d 682f 5d75 6831 4e68 3268  h+]h,]h/]uh1Nh2h
-00004380: 0268 335d 72da 0200 0028 6897 2981 72db  .h3]r....(h.).r.
-00004390: 0200 007d 72dc 0200 0028 681e 583c 0000  ...}r....(h.X<..
-000043a0: 0060 6078 746f 6c20 3e3d 6060 2072 656c  .``xtol >=`` rel
-000043b0: 6174 6976 6520 6368 616e 6765 2069 6e20  ative change in 
-000043c0: 7061 7261 6d65 7465 7273 2062 6574 7765  parameters betwe
-000043d0: 656e 2069 7465 7261 7469 6f6e 7368 1f6a  en iterationsh.j
-000043e0: d602 0000 6823 6a59 0100 0068 2568 9a68  ....h#jY...h%h.h
-000043f0: 277d 72dd 0200 0028 6829 5d68 2a5d 682b  '}r....(h)]h*]h+
-00004400: 5d68 2c5d 682f 5d75 6831 4b14 6833 5d72  ]h,]h/]uh1K.h3]r
-00004410: de02 0000 2868 4a29 8172 df02 0000 7d72  ....(hJ).r....}r
-00004420: e002 0000 2868 1e58 0b00 0000 6060 7874  ....(h.X....``xt
-00004430: 6f6c 203e 3d60 6068 277d 72e1 0200 0028  ol >=``h'}r....(
-00004440: 6829 5d68 2a5d 682b 5d68 2c5d 682f 5d75  h)]h*]h+]h,]h/]u
-00004450: 681f 6adb 0200 0068 335d 72e2 0200 0068  h.j....h3]r....h
-00004460: 5258 0700 0000 7874 6f6c 203e 3d72 e302  RX....xtol >=r..
-00004470: 0000 8581 72e4 0200 007d 72e5 0200 0028  ....r....}r....(
-00004480: 681e 5500 681f 6adf 0200 0075 6261 6825  h.U.h.j....ubah%
-00004490: 6856 7562 6852 5831 0000 0020 7265 6c61  hVubhRX1... rela
-000044a0: 7469 7665 2063 6861 6e67 6520 696e 2070  tive change in p
-000044b0: 6172 616d 6574 6572 7320 6265 7477 6565  arameters betwee
-000044c0: 6e20 6974 6572 6174 696f 6e73 72e6 0200  n iterationsr...
-000044d0: 0085 8172 e702 0000 7d72 e802 0000 2868  ...r....}r....(h
-000044e0: 1e58 3100 0000 2072 656c 6174 6976 6520  .X1... relative 
-000044f0: 6368 616e 6765 2069 6e20 7061 7261 6d65  change in parame
-00004500: 7465 7273 2062 6574 7765 656e 2069 7465  ters between ite
-00004510: 7261 7469 6f6e 7368 1f6a db02 0000 7562  rationsh.j....ub
-00004520: 6575 6268 9729 8172 e902 0000 7d72 ea02  eubh.).r....}r..
-00004530: 0000 2868 1e58 3300 0000 6060 6774 6f6c  ..(h.X3...``gtol
-00004540: 203e 3d60 6020 7265 6c61 7469 7665 2073   >=`` relative s
-00004550: 697a 6520 6f66 2067 7261 6469 656e 7420  ize of gradient 
-00004560: 6f66 2060 6063 6869 2a2a 3260 6068 1f6a  of ``chi**2``h.j
-00004570: d602 0000 6823 6a59 0100 0068 2568 9a68  ....h#jY...h%h.h
-00004580: 277d 72eb 0200 0028 6829 5d68 2a5d 682b  '}r....(h)]h*]h+
-00004590: 5d68 2c5d 682f 5d75 6831 4b16 6833 5d72  ]h,]h/]uh1K.h3]r
-000045a0: ec02 0000 2868 4a29 8172 ed02 0000 7d72  ....(hJ).r....}r
-000045b0: ee02 0000 2868 1e58 0b00 0000 6060 6774  ....(h.X....``gt
-000045c0: 6f6c 203e 3d60 6068 277d 72ef 0200 0028  ol >=``h'}r....(
-000045d0: 6829 5d68 2a5d 682b 5d68 2c5d 682f 5d75  h)]h*]h+]h,]h/]u
-000045e0: 681f 6ae9 0200 0068 335d 72f0 0200 0068  h.j....h3]r....h
-000045f0: 5258 0700 0000 6774 6f6c 203e 3d72 f102  RX....gtol >=r..
-00004600: 0000 8581 72f2 0200 007d 72f3 0200 0028  ....r....}r....(
-00004610: 681e 5500 681f 6aed 0200 0075 6261 6825  h.U.h.j....ubah%
-00004620: 6856 7562 6852 581e 0000 0020 7265 6c61  hVubhRX.... rela
-00004630: 7469 7665 2073 697a 6520 6f66 2067 7261  tive size of gra
-00004640: 6469 656e 7420 6f66 2072 f402 0000 8581  dient of r......
-00004650: 72f5 0200 007d 72f6 0200 0028 681e 581e  r....}r....(h.X.
-00004660: 0000 0020 7265 6c61 7469 7665 2073 697a  ... relative siz
-00004670: 6520 6f66 2067 7261 6469 656e 7420 6f66  e of gradient of
-00004680: 2068 1f6a e902 0000 7562 684a 2981 72f7   h.j....ubhJ).r.
-00004690: 0200 007d 72f8 0200 0028 681e 580a 0000  ...}r....(h.X...
-000046a0: 0060 6063 6869 2a2a 3260 6068 277d 72f9  .``chi**2``h'}r.
-000046b0: 0200 0028 6829 5d68 2a5d 682b 5d68 2c5d  ...(h)]h*]h+]h,]
-000046c0: 682f 5d75 681f 6ae9 0200 0068 335d 72fa  h/]uh.j....h3]r.
-000046d0: 0200 0068 5258 0600 0000 6368 692a 2a32  ...hRX....chi**2
-000046e0: 72fb 0200 0085 8172 fc02 0000 7d72 fd02  r......r....}r..
-000046f0: 0000 2868 1e55 0068 1f6a f702 0000 7562  ..(h.U.h.j....ub
-00004700: 6168 2568 5675 6265 7562 6897 2981 72fe  ah%hVubeubh.).r.
-00004710: 0200 007d 72ff 0200 0028 681e 583c 0000  ...}r....(h.X<..
-00004720: 0060 6066 746f 6c20 3e3d 6060 2072 656c  .``ftol >=`` rel
-00004730: 6174 6976 6520 6368 616e 6765 2069 6e20  ative change in 
-00004740: 6060 6368 692a 2a32 6060 2062 6574 7765  ``chi**2`` betwe
-00004750: 656e 2069 7465 7261 7469 6f6e 7368 1f6a  en iterationsh.j
-00004760: d602 0000 6823 6a59 0100 0068 2568 9a68  ....h#jY...h%h.h
-00004770: 277d 7200 0300 0028 6829 5d68 2a5d 682b  '}r....(h)]h*]h+
-00004780: 5d68 2c5d 682f 5d75 6831 4b18 6833 5d72  ]h,]h/]uh1K.h3]r
-00004790: 0103 0000 2868 4a29 8172 0203 0000 7d72  ....(hJ).r....}r
-000047a0: 0303 0000 2868 1e58 0b00 0000 6060 6674  ....(h.X....``ft
-000047b0: 6f6c 203e 3d60 6068 277d 7204 0300 0028  ol >=``h'}r....(
-000047c0: 6829 5d68 2a5d 682b 5d68 2c5d 682f 5d75  h)]h*]h+]h,]h/]u
-000047d0: 681f 6afe 0200 0068 335d 7205 0300 0068  h.j....h3]r....h
-000047e0: 5258 0700 0000 6674 6f6c 203e 3d72 0603  RX....ftol >=r..
-000047f0: 0000 8581 7207 0300 007d 7208 0300 0028  ....r....}r....(
-00004800: 681e 5500 681f 6a02 0300 0075 6261 6825  h.U.h.j....ubah%
-00004810: 6856 7562 6852 5814 0000 0020 7265 6c61  hVubhRX.... rela
-00004820: 7469 7665 2063 6861 6e67 6520 696e 2072  tive change in r
-00004830: 0903 0000 8581 720a 0300 007d 720b 0300  ......r....}r...
-00004840: 0028 681e 5814 0000 0020 7265 6c61 7469  .(h.X.... relati
-00004850: 7665 2063 6861 6e67 6520 696e 2068 1f6a  ve change in h.j
-00004860: fe02 0000 7562 684a 2981 720c 0300 007d  ....ubhJ).r....}
-00004870: 720d 0300 0028 681e 580a 0000 0060 6063  r....(h.X....``c
-00004880: 6869 2a2a 3260 6068 277d 720e 0300 0028  hi**2``h'}r....(
-00004890: 6829 5d68 2a5d 682b 5d68 2c5d 682f 5d75  h)]h*]h+]h,]h/]u
-000048a0: 681f 6afe 0200 0068 335d 720f 0300 0068  h.j....h3]r....h
-000048b0: 5258 0600 0000 6368 692a 2a32 7210 0300  RX....chi**2r...
-000048c0: 0085 8172 1103 0000 7d72 1203 0000 2868  ...r....}r....(h
-000048d0: 1e55 0068 1f6a 0c03 0000 7562 6168 2568  .U.h.j....ubah%h
-000048e0: 5675 6268 5258 1300 0000 2062 6574 7765  VubhRX.... betwe
-000048f0: 656e 2069 7465 7261 7469 6f6e 7372 1303  en iterationsr..
-00004900: 0000 8581 7214 0300 007d 7215 0300 0028  ....r....}r....(
-00004910: 681e 5813 0000 0020 6265 7477 6565 6e20  h.X.... between 
-00004920: 6974 6572 6174 696f 6e73 681f 6afe 0200  iterationsh.j...
-00004930: 0075 6265 7562 6575 6268 9729 8172 1603  .ubeubeubh.).r..
-00004940: 0000 7d72 1703 0000 2868 1e58 cf01 0000  ..}r....(h.X....
-00004950: 6973 2073 7461 7469 7366 6965 642e 2053  is statisfied. S
-00004960: 6565 2074 6865 2060 6073 6369 7079 2e6f  ee the ``scipy.o
-00004970: 7074 696d 697a 652e 6c65 6173 745f 7371  ptimize.least_sq
-00004980: 7561 7265 7360 600a 646f 6375 6d65 6e74  uares``.document
-00004990: 6174 696f 6e20 6465 7461 696c 6564 2064  ation detailed d
-000049a0: 6566 696e 6974 696f 6e73 206f 6620 7468  efinitions of th
-000049b0: 6520 7374 6f70 7069 6e67 2063 6f6e 6469  e stopping condi
-000049c0: 7469 6f6e 732e 0a54 7970 6963 616c 6c79  tions..Typically
-000049d0: 206f 6e65 2073 6574 7320 6060 7874 6f6c   one sets ``xtol
-000049e0: 3d31 2f31 302a 2a64 6060 2077 6865 7265  =1/10**d`` where
-000049f0: 2060 6064 6060 2069 7320 7468 6520 6e75   ``d`` is the nu
-00004a00: 6d62 6572 206f 660a 6469 6769 7473 206f  mber of.digits o
-00004a10: 6620 7072 6563 6973 696f 6e20 6465 7369  f precision desi
-00004a20: 7265 6420 696e 2074 6865 2072 6573 756c  red in the resul
-00004a30: 742c 2077 6869 6c65 2060 6067 746f 6c3c  t, while ``gtol<
-00004a40: 3c31 6060 2061 6e64 0a60 6066 746f 6c3c  <1`` and.``ftol<
-00004a50: 3c31 6060 2e20 5365 7474 696e 6720 6060  <1``. Setting ``
-00004a60: 746f 6c3d 6570 7360 6020 7768 6572 6520  tol=eps`` where 
-00004a70: 6060 6570 7360 6020 6973 2061 206e 756d  ``eps`` is a num
-00004a80: 6265 7220 6973 0a65 7175 6976 616c 656e  ber is.equivalen
-00004a90: 7420 746f 2073 6574 7469 6e67 2060 6074  t to setting ``t
-00004aa0: 6f6c 3d28 6570 732c 3165 2d31 302c 3165  ol=(eps,1e-10,1e
-00004ab0: 2d31 3029 6060 2e20 5365 7474 696e 670a  -10)``. Setting.
-00004ac0: 6060 746f 6c3d 2865 7073 312c 6570 7332  ``tol=(eps1,eps2
-00004ad0: 2960 6020 6973 2065 7175 6976 6c65 6e74  )`` is equivlent
-00004ae0: 2074 6f20 7365 7474 696e 670a 6060 746f   to setting.``to
-00004af0: 6c3d 2865 7073 312c 6570 7332 2c31 652d  l=(eps1,eps2,1e-
-00004b00: 3130 2960 602e 2044 6566 6175 6c74 2069  10)``. Default i
-00004b10: 7320 6060 746f 6c3d 3165 2d35 6060 2e68  s ``tol=1e-5``.h
-00004b20: 1f6a 9202 0000 6823 6a59 0100 0068 2568  .j....h#jY...h%h
-00004b30: 9a68 277d 7218 0300 0028 6829 5d68 2a5d  .h'}r....(h)]h*]
-00004b40: 682b 5d68 2c5d 682f 5d75 6831 4b1a 6832  h+]h,]h/]uh1K.h2
-00004b50: 6802 6833 5d72 1903 0000 2868 5258 1700  h.h3]r....(hRX..
-00004b60: 0000 6973 2073 7461 7469 7366 6965 642e  ..is statisfied.
-00004b70: 2053 6565 2074 6865 2072 1a03 0000 8581   See the r......
-00004b80: 721b 0300 007d 721c 0300 0028 681e 5817  r....}r....(h.X.
-00004b90: 0000 0069 7320 7374 6174 6973 6669 6564  ...is statisfied
-00004ba0: 2e20 5365 6520 7468 6520 6823 4e68 314e  . See the h#Nh1N
-00004bb0: 6832 6802 681f 6a16 0300 0075 6268 4a29  h2h.h.j....ubhJ)
-00004bc0: 8172 1d03 0000 7d72 1e03 0000 2868 1e58  .r....}r....(h.X
-00004bd0: 2000 0000 6060 7363 6970 792e 6f70 7469   ...``scipy.opti
-00004be0: 6d69 7a65 2e6c 6561 7374 5f73 7175 6172  mize.least_squar
-00004bf0: 6573 6060 6827 7d72 1f03 0000 2868 295d  es``h'}r....(h)]
-00004c00: 682a 5d68 2b5d 682c 5d68 2f5d 7568 1f6a  h*]h+]h,]h/]uh.j
-00004c10: 1603 0000 6833 5d72 2003 0000 6852 581c  ....h3]r ...hRX.
-00004c20: 0000 0073 6369 7079 2e6f 7074 696d 697a  ...scipy.optimiz
-00004c30: 652e 6c65 6173 745f 7371 7561 7265 7372  e.least_squaresr
-00004c40: 2103 0000 8581 7222 0300 007d 7223 0300  !.....r"...}r#..
-00004c50: 0028 681e 5500 681f 6a1d 0300 0075 6261  .(h.U.h.j....uba
-00004c60: 6825 6856 7562 6852 5853 0000 000a 646f  h%hVubhRXS....do
-00004c70: 6375 6d65 6e74 6174 696f 6e20 6465 7461  cumentation deta
-00004c80: 696c 6564 2064 6566 696e 6974 696f 6e73  iled definitions
-00004c90: 206f 6620 7468 6520 7374 6f70 7069 6e67   of the stopping
-00004ca0: 2063 6f6e 6469 7469 6f6e 732e 0a54 7970   conditions..Typ
-00004cb0: 6963 616c 6c79 206f 6e65 2073 6574 7320  ically one sets 
-00004cc0: 7224 0300 0085 8172 2503 0000 7d72 2603  r$.....r%...}r&.
-00004cd0: 0000 2868 1e58 5300 0000 0a64 6f63 756d  ..(h.XS....docum
-00004ce0: 656e 7461 7469 6f6e 2064 6574 6169 6c65  entation detaile
-00004cf0: 6420 6465 6669 6e69 7469 6f6e 7320 6f66  d definitions of
-00004d00: 2074 6865 2073 746f 7070 696e 6720 636f   the stopping co
-00004d10: 6e64 6974 696f 6e73 2e0a 5479 7069 6361  nditions..Typica
-00004d20: 6c6c 7920 6f6e 6520 7365 7473 2068 234e  lly one sets h#N
-00004d30: 6831 4e68 3268 0268 1f6a 1603 0000 7562  h1Nh2h.h.j....ub
-00004d40: 684a 2981 7227 0300 007d 7228 0300 0028  hJ).r'...}r(...(
-00004d50: 681e 5810 0000 0060 6078 746f 6c3d 312f  h.X....``xtol=1/
-00004d60: 3130 2a2a 6460 6068 277d 7229 0300 0028  10**d``h'}r)...(
-00004d70: 6829 5d68 2a5d 682b 5d68 2c5d 682f 5d75  h)]h*]h+]h,]h/]u
-00004d80: 681f 6a16 0300 0068 335d 722a 0300 0068  h.j....h3]r*...h
-00004d90: 5258 0c00 0000 7874 6f6c 3d31 2f31 302a  RX....xtol=1/10*
-00004da0: 2a64 722b 0300 0085 8172 2c03 0000 7d72  *dr+.....r,...}r
-00004db0: 2d03 0000 2868 1e55 0068 1f6a 2703 0000  -...(h.U.h.j'...
-00004dc0: 7562 6168 2568 5675 6268 5258 0700 0000  ubah%hVubhRX....
-00004dd0: 2077 6865 7265 2072 2e03 0000 8581 722f   where r......r/
-00004de0: 0300 007d 7230 0300 0028 681e 5807 0000  ...}r0...(h.X...
-00004df0: 0020 7768 6572 6520 7231 0300 0068 234e  . where r1...h#N
-00004e00: 6831 4e68 3268 0268 1f6a 1603 0000 7562  h1Nh2h.h.j....ub
-00004e10: 684a 2981 7232 0300 007d 7233 0300 0028  hJ).r2...}r3...(
-00004e20: 681e 5805 0000 0060 6064 6060 6827 7d72  h.X....``d``h'}r
-00004e30: 3403 0000 2868 295d 682a 5d68 2b5d 682c  4...(h)]h*]h+]h,
-00004e40: 5d68 2f5d 7568 1f6a 1603 0000 6833 5d72  ]h/]uh.j....h3]r
-00004e50: 3503 0000 6852 5801 0000 0064 8581 7236  5...hRX....d..r6
-00004e60: 0300 007d 7237 0300 0028 681e 5500 681f  ...}r7...(h.U.h.
-00004e70: 6a32 0300 0075 6261 6825 6856 7562 6852  j2...ubah%hVubhR
-00004e80: 5843 0000 0020 6973 2074 6865 206e 756d  XC... is the num
-00004e90: 6265 7220 6f66 0a64 6967 6974 7320 6f66  ber of.digits of
-00004ea0: 2070 7265 6369 7369 6f6e 2064 6573 6972   precision desir
-00004eb0: 6564 2069 6e20 7468 6520 7265 7375 6c74  ed in the result
-00004ec0: 2c20 7768 696c 6520 7238 0300 0085 8172  , while r8.....r
-00004ed0: 3903 0000 7d72 3a03 0000 2868 1e58 4300  9...}r:...(h.XC.
-00004ee0: 0000 2069 7320 7468 6520 6e75 6d62 6572  .. is the number
-00004ef0: 206f 660a 6469 6769 7473 206f 6620 7072   of.digits of pr
-00004f00: 6563 6973 696f 6e20 6465 7369 7265 6420  ecision desired 
-00004f10: 696e 2074 6865 2072 6573 756c 742c 2077  in the result, w
-00004f20: 6869 6c65 2068 234e 6831 4e68 3268 0268  hile h#Nh1Nh2h.h
-00004f30: 1f6a 1603 0000 7562 684a 2981 723b 0300  .j....ubhJ).r;..
-00004f40: 007d 723c 0300 0028 681e 580b 0000 0060  .}r<...(h.X....`
-00004f50: 6067 746f 6c3c 3c31 6060 6827 7d72 3d03  `gtol<<1``h'}r=.
-00004f60: 0000 2868 295d 682a 5d68 2b5d 682c 5d68  ..(h)]h*]h+]h,]h
-00004f70: 2f5d 7568 1f6a 1603 0000 6833 5d72 3e03  /]uh.j....h3]r>.
-00004f80: 0000 6852 5807 0000 0067 746f 6c3c 3c31  ..hRX....gtol<<1
-00004f90: 723f 0300 0085 8172 4003 0000 7d72 4103  r?.....r@...}rA.
-00004fa0: 0000 2868 1e55 0068 1f6a 3b03 0000 7562  ..(h.U.h.j;...ub
-00004fb0: 6168 2568 5675 6268 5258 0500 0000 2061  ah%hVubhRX.... a
-00004fc0: 6e64 0a72 4203 0000 8581 7243 0300 007d  nd.rB.....rC...}
-00004fd0: 7244 0300 0028 681e 5805 0000 0020 616e  rD...(h.X.... an
-00004fe0: 640a 6823 4e68 314e 6832 6802 681f 6a16  d.h#Nh1Nh2h.h.j.
-00004ff0: 0300 0075 6268 4a29 8172 4503 0000 7d72  ...ubhJ).rE...}r
-00005000: 4603 0000 2868 1e58 0b00 0000 6060 6674  F...(h.X....``ft
-00005010: 6f6c 3c3c 3160 6068 277d 7247 0300 0028  ol<<1``h'}rG...(
-00005020: 6829 5d68 2a5d 682b 5d68 2c5d 682f 5d75  h)]h*]h+]h,]h/]u
-00005030: 681f 6a16 0300 0068 335d 7248 0300 0068  h.j....h3]rH...h
-00005040: 5258 0700 0000 6674 6f6c 3c3c 3172 4903  RX....ftol<<1rI.
-00005050: 0000 8581 724a 0300 007d 724b 0300 0028  ....rJ...}rK...(
-00005060: 681e 5500 681f 6a45 0300 0075 6261 6825  h.U.h.jE...ubah%
-00005070: 6856 7562 6852 580a 0000 002e 2053 6574  hVubhRX..... Set
-00005080: 7469 6e67 2072 4c03 0000 8581 724d 0300  ting rL.....rM..
-00005090: 007d 724e 0300 0028 681e 580a 0000 002e  .}rN...(h.X.....
-000050a0: 2053 6574 7469 6e67 2068 234e 6831 4e68   Setting h#Nh1Nh
-000050b0: 3268 0268 1f6a 1603 0000 7562 684a 2981  2h.h.j....ubhJ).
-000050c0: 724f 0300 007d 7250 0300 0028 681e 580b  rO...}rP...(h.X.
-000050d0: 0000 0060 6074 6f6c 3d65 7073 6060 6827  ...``tol=eps``h'
-000050e0: 7d72 5103 0000 2868 295d 682a 5d68 2b5d  }rQ...(h)]h*]h+]
-000050f0: 682c 5d68 2f5d 7568 1f6a 1603 0000 6833  h,]h/]uh.j....h3
-00005100: 5d72 5203 0000 6852 5807 0000 0074 6f6c  ]rR...hRX....tol
-00005110: 3d65 7073 7253 0300 0085 8172 5403 0000  =epsrS.....rT...
-00005120: 7d72 5503 0000 2868 1e55 0068 1f6a 4f03  }rU...(h.U.h.jO.
-00005130: 0000 7562 6168 2568 5675 6268 5258 0700  ..ubah%hVubhRX..
-00005140: 0000 2077 6865 7265 2072 5603 0000 8581  .. where rV.....
-00005150: 7257 0300 007d 7258 0300 0028 681e 6a31  rW...}rX...(h.j1
-00005160: 0300 0068 1f6a 1603 0000 7562 684a 2981  ...h.j....ubhJ).
-00005170: 7259 0300 007d 725a 0300 0028 681e 5807  rY...}rZ...(h.X.
-00005180: 0000 0060 6065 7073 6060 6827 7d72 5b03  ...``eps``h'}r[.
-00005190: 0000 2868 295d 682a 5d68 2b5d 682c 5d68  ..(h)]h*]h+]h,]h
-000051a0: 2f5d 7568 1f6a 1603 0000 6833 5d72 5c03  /]uh.j....h3]r\.
-000051b0: 0000 6852 5803 0000 0065 7073 725d 0300  ..hRX....epsr]..
-000051c0: 0085 8172 5e03 0000 7d72 5f03 0000 2868  ...r^...}r_...(h
-000051d0: 1e55 0068 1f6a 5903 0000 7562 6168 2568  .U.h.jY...ubah%h
-000051e0: 5675 6268 5258 2600 0000 2069 7320 6120  VubhRX&... is a 
-000051f0: 6e75 6d62 6572 2069 730a 6571 7569 7661  number is.equiva
-00005200: 6c65 6e74 2074 6f20 7365 7474 696e 6720  lent to setting 
-00005210: 7260 0300 0085 8172 6103 0000 7d72 6203  r`.....ra...}rb.
-00005220: 0000 2868 1e58 2600 0000 2069 7320 6120  ..(h.X&... is a 
-00005230: 6e75 6d62 6572 2069 730a 6571 7569 7661  number is.equiva
-00005240: 6c65 6e74 2074 6f20 7365 7474 696e 6720  lent to setting 
-00005250: 6823 4e68 314e 6832 6802 681f 6a16 0300  h#Nh1Nh2h.h.j...
-00005260: 0075 6268 4a29 8172 6303 0000 7d72 6403  .ubhJ).rc...}rd.
-00005270: 0000 2868 1e58 1900 0000 6060 746f 6c3d  ..(h.X....``tol=
-00005280: 2865 7073 2c31 652d 3130 2c31 652d 3130  (eps,1e-10,1e-10
-00005290: 2960 6068 277d 7265 0300 0028 6829 5d68  )``h'}re...(h)]h
-000052a0: 2a5d 682b 5d68 2c5d 682f 5d75 681f 6a16  *]h+]h,]h/]uh.j.
-000052b0: 0300 0068 335d 7266 0300 0068 5258 1500  ...h3]rf...hRX..
-000052c0: 0000 746f 6c3d 2865 7073 2c31 652d 3130  ..tol=(eps,1e-10
-000052d0: 2c31 652d 3130 2972 6703 0000 8581 7268  ,1e-10)rg.....rh
-000052e0: 0300 007d 7269 0300 0028 681e 5500 681f  ...}ri...(h.U.h.
-000052f0: 6a63 0300 0075 6261 6825 6856 7562 6852  jc...ubah%hVubhR
-00005300: 580a 0000 002e 2053 6574 7469 6e67 0a72  X..... Setting.r
-00005310: 6a03 0000 8581 726b 0300 007d 726c 0300  j.....rk...}rl..
-00005320: 0028 681e 580a 0000 002e 2053 6574 7469  .(h.X..... Setti
-00005330: 6e67 0a68 234e 6831 4e68 3268 0268 1f6a  ng.h#Nh1Nh2h.h.j
-00005340: 1603 0000 7562 684a 2981 726d 0300 007d  ....ubhJ).rm...}
-00005350: 726e 0300 0028 681e 5813 0000 0060 6074  rn...(h.X....``t
-00005360: 6f6c 3d28 6570 7331 2c65 7073 3229 6060  ol=(eps1,eps2)``
-00005370: 6827 7d72 6f03 0000 2868 295d 682a 5d68  h'}ro...(h)]h*]h
-00005380: 2b5d 682c 5d68 2f5d 7568 1f6a 1603 0000  +]h,]h/]uh.j....
-00005390: 6833 5d72 7003 0000 6852 580f 0000 0074  h3]rp...hRX....t
-000053a0: 6f6c 3d28 6570 7331 2c65 7073 3229 7271  ol=(eps1,eps2)rq
-000053b0: 0300 0085 8172 7203 0000 7d72 7303 0000  .....rr...}rs...
-000053c0: 2868 1e55 0068 1f6a 6d03 0000 7562 6168  (h.U.h.jm...ubah
-000053d0: 2568 5675 6268 5258 1900 0000 2069 7320  %hVubhRX.... is 
-000053e0: 6571 7569 766c 656e 7420 746f 2073 6574  equivlent to set
-000053f0: 7469 6e67 0a72 7403 0000 8581 7275 0300  ting.rt.....ru..
-00005400: 007d 7276 0300 0028 681e 5819 0000 0020  .}rv...(h.X.... 
-00005410: 6973 2065 7175 6976 6c65 6e74 2074 6f20  is equivlent to 
-00005420: 7365 7474 696e 670a 6823 4e68 314e 6832  setting.h#Nh1Nh2
-00005430: 6802 681f 6a16 0300 0075 6268 4a29 8172  h.h.j....ubhJ).r
-00005440: 7703 0000 7d72 7803 0000 2868 1e58 1900  w...}rx...(h.X..
-00005450: 0000 6060 746f 6c3d 2865 7073 312c 6570  ..``tol=(eps1,ep
-00005460: 7332 2c31 652d 3130 2960 6068 277d 7279  s2,1e-10)``h'}ry
-00005470: 0300 0028 6829 5d68 2a5d 682b 5d68 2c5d  ...(h)]h*]h+]h,]
-00005480: 682f 5d75 681f 6a16 0300 0068 335d 727a  h/]uh.j....h3]rz
-00005490: 0300 0068 5258 1500 0000 746f 6c3d 2865  ...hRX....tol=(e
-000054a0: 7073 312c 6570 7332 2c31 652d 3130 2972  ps1,eps2,1e-10)r
-000054b0: 7b03 0000 8581 727c 0300 007d 727d 0300  {.....r|...}r}..
-000054c0: 0028 681e 5500 681f 6a77 0300 0075 6261  .(h.U.h.jw...uba
-000054d0: 6825 6856 7562 6852 580d 0000 002e 2044  h%hVubhRX..... D
-000054e0: 6566 6175 6c74 2069 7320 727e 0300 0085  efault is r~....
-000054f0: 8172 7f03 0000 7d72 8003 0000 2868 1e58  .r....}r....(h.X
-00005500: 0d00 0000 2e20 4465 6661 756c 7420 6973  ..... Default is
-00005510: 2068 234e 6831 4e68 3268 0268 1f6a 1603   h#Nh1Nh2h.h.j..
-00005520: 0000 7562 684a 2981 7281 0300 007d 7282  ..ubhJ).r....}r.
-00005530: 0300 0028 681e 580c 0000 0060 6074 6f6c  ...(h.X....``tol
-00005540: 3d31 652d 3560 6068 277d 7283 0300 0028  =1e-5``h'}r....(
-00005550: 6829 5d68 2a5d 682b 5d68 2c5d 682f 5d75  h)]h*]h+]h,]h/]u
-00005560: 681f 6a16 0300 0068 335d 7284 0300 0068  h.j....h3]r....h
-00005570: 5258 0800 0000 746f 6c3d 3165 2d35 7285  RX....tol=1e-5r.
-00005580: 0300 0085 8172 8603 0000 7d72 8703 0000  .....r....}r....
-00005590: 2868 1e55 0068 1f6a 8103 0000 7562 6168  (h.U.h.j....ubah
-000055a0: 2568 5675 6268 5258 0100 0000 2e85 8172  %hVubhRX.......r
-000055b0: 8803 0000 7d72 8903 0000 2868 1e58 0100  ....}r....(h.X..
-000055c0: 0000 2e68 234e 6831 4e68 3268 0268 1f6a  ...h#Nh1Nh2h.h.j
-000055d0: 1603 0000 7562 6575 6265 6825 689a 7562  ....ubeubeh%h.ub
-000055e0: 6168 256a 0102 0000 7562 6ad4 0100 0029  ah%j....ubj....)
-000055f0: 8172 8a03 0000 7d72 8b03 0000 2868 1e55  .r....}r....(h.U
-00005600: 0068 277d 728c 0300 0028 6829 5d68 2a5d  .h'}r....(h)]h*]
-00005610: 682b 5d68 2c5d 682f 5d75 681f 6ad0 0100  h+]h,]h/]uh.j...
-00005620: 0068 335d 728d 0300 0068 9729 8172 8e03  .h3]r....h.).r..
-00005630: 0000 7d72 8f03 0000 2868 1e58 9b01 0000  ..}r....(h.X....
-00005640: 6d65 7468 6f64 2028 7374 7220 6f72 204e  method (str or N
-00005650: 6f6e 6529 202d 2d20 4d69 6e69 6d69 7a61  one) -- Minimiza
-00005660: 7469 6f6e 2061 6c67 6f72 6974 686d 2e20  tion algorithm. 
-00005670: 4f70 7469 6f6e 730a 696e 636c 7564 653a  Options.include:
-00005680: 2774 7266 270a 0a54 7275 7374 6564 2052  'trf'..Trusted R
-00005690: 6567 696f 6e20 5265 666c 6563 7469 7665  egion Reflective
-000056a0: 2061 6c67 6f72 6974 686d 2028 6465 6661   algorithm (defa
-000056b0: 756c 7429 2e20 4265 7374 0a63 686f 6963  ult). Best.choic
-000056c0: 6520 7769 7468 2062 6f75 6e64 6564 2070  e with bounded p
-000056d0: 6172 616d 6574 6572 732e 0a0a 2764 6f67  arameters...'dog
-000056e0: 626f 7827 0a0a 646f 676c 6567 2061 6c67  box'..dogleg alg
-000056f0: 6f72 6974 686d 2061 6461 7074 6564 2066  orithm adapted f
-00005700: 6f72 2062 6f75 6e64 6564 2070 6172 616d  or bounded param
-00005710: 6574 6572 732e 0a0a 276c 6d27 0a0a 4c65  eters...'lm'..Le
-00005720: 7665 6e62 6572 672d 4d61 7271 7561 7264  venberg-Marquard
-00005730: 7420 616c 676f 7269 7468 6d20 6173 2069  t algorithm as i
-00005740: 6d70 6c65 6d65 6e74 6564 2069 6e20 4d49  mplemented in MI
-00005750: 4e50 4143 4b2e 0a42 6573 7420 666f 7220  NPACK..Best for 
-00005760: 736d 616c 6c65 7220 7072 6f62 6c65 6d73  smaller problems
-00005770: 2e20 446f 6573 206e 6f74 2077 6f72 6b20  . Does not work 
-00005780: 7769 7468 2062 6f75 6e64 6564 0a70 6172  with bounded.par
-00005790: 616d 6574 6572 7320 2862 6f75 6e64 7320  ameters (bounds 
-000057a0: 6172 6520 6967 6e6f 7265 6429 2e53 6574  are ignored).Set
-000057b0: 7469 6e67 206d 6574 686f 643d 4e6f 6e65  ting method=None
-000057c0: 2069 6d70 6c69 6573 2074 6865 2064 6566   implies the def
-000057d0: 6175 6c74 2027 7472 6627 2e68 277d 7290  ault 'trf'.h'}r.
-000057e0: 0300 0028 6829 5d68 2a5d 682b 5d68 2c5d  ...(h)]h*]h+]h,]
-000057f0: 682f 5d75 681f 6a8a 0300 0068 335d 7291  h/]uh.j....h3]r.
-00005800: 0300 0028 6add 0100 0029 8172 9203 0000  ...(j....).r....
-00005810: 7d72 9303 0000 2868 1e58 0600 0000 6d65  }r....(h.X....me
-00005820: 7468 6f64 6827 7d72 9403 0000 2868 2c5d  thodh'}r....(h,]
-00005830: 682b 5d6a e101 0000 8868 295d 682a 5d68  h+]j.....h)]h*]h
-00005840: 2f5d 7568 1f6a 8e03 0000 6833 5d72 9503  /]uh.j....h3]r..
-00005850: 0000 6852 5806 0000 006d 6574 686f 6472  ..hRX....methodr
-00005860: 9603 0000 8581 7297 0300 007d 7298 0300  ......r....}r...
-00005870: 0028 681e 5500 681f 6a92 0300 0075 6261  .(h.U.h.j....uba
-00005880: 6825 6ae6 0100 0075 6268 5258 0200 0000  h%j....ubhRX....
-00005890: 2028 7299 0300 0085 8172 9a03 0000 7d72   (r......r....}r
-000058a0: 9b03 0000 2868 1e55 0068 1f6a 8e03 0000  ....(h.U.h.j....
-000058b0: 7562 683c 2981 729c 0300 007d 729d 0300  ubh<).r....}r...
-000058c0: 0028 681e 5500 6827 7d72 9e03 0000 2855  .(h.U.h'}r....(U
-000058d0: 0772 6566 7479 7065 68f2 6ae1 0100 0088  .reftypeh.j.....
-000058e0: 5509 7265 6674 6172 6765 7458 0300 0000  U.reftargetX....
-000058f0: 7374 7272 9f03 0000 5509 7265 6664 6f6d  strr....U.refdom
-00005900: 6169 6e68 de68 2c5d 682b 5d55 0b72 6566  ainh.h,]h+]U.ref
-00005910: 6578 706c 6963 6974 8968 295d 682a 5d68  explicit.h)]h*]h
-00005920: 2f5d 7568 1f6a 8e03 0000 6833 5d72 a003  /]uh.j....h3]r..
-00005930: 0000 6aef 0100 0029 8172 a103 0000 7d72  ..j....).r....}r
-00005940: a203 0000 2868 1e6a 9f03 0000 6827 7d72  ....(h.j....h'}r
-00005950: a303 0000 2868 295d 682a 5d68 2b5d 682c  ....(h)]h*]h+]h,
-00005960: 5d68 2f5d 7568 1f6a 9c03 0000 6833 5d72  ]h/]uh.j....h3]r
-00005970: a403 0000 6852 5803 0000 0073 7472 72a5  ....hRX....strr.
-00005980: 0300 0085 8172 a603 0000 7d72 a703 0000  .....r....}r....
-00005990: 2868 1e55 0068 1f6a a103 0000 7562 6168  (h.U.h.j....ubah
-000059a0: 256a f701 0000 7562 6168 2568 4075 626a  %j....ubah%h@ubj
-000059b0: ef01 0000 2981 72a8 0300 007d 72a9 0300  ....).r....}r...
-000059c0: 0028 681e 5804 0000 0020 6f72 2068 277d  .(h.X.... or h'}
-000059d0: 72aa 0300 0028 6829 5d68 2a5d 682b 5d68  r....(h)]h*]h+]h
-000059e0: 2c5d 682f 5d75 681f 6a8e 0300 0068 335d  ,]h/]uh.j....h3]
-000059f0: 72ab 0300 0068 5258 0400 0000 206f 7220  r....hRX.... or 
-00005a00: 72ac 0300 0085 8172 ad03 0000 7d72 ae03  r......r....}r..
-00005a10: 0000 2868 1e55 0068 1f6a a803 0000 7562  ..(h.U.h.j....ub
-00005a20: 6168 256a f701 0000 7562 683c 2981 72af  ah%j....ubh<).r.
-00005a30: 0300 007d 72b0 0300 0028 681e 5500 6827  ...}r....(h.U.h'
-00005a40: 7d72 b103 0000 2855 0772 6566 7479 7065  }r....(U.reftype
-00005a50: 68f2 6ae1 0100 0088 5509 7265 6674 6172  h.j.....U.reftar
-00005a60: 6765 7458 0400 0000 4e6f 6e65 72b2 0300  getX....Noner...
-00005a70: 0055 0972 6566 646f 6d61 696e 68de 682c  .U.refdomainh.h,
-00005a80: 5d68 2b5d 550b 7265 6665 7870 6c69 6369  ]h+]U.refexplici
-00005a90: 7489 6829 5d68 2a5d 682f 5d75 681f 6a8e  t.h)]h*]h/]uh.j.
-00005aa0: 0300 0068 335d 72b3 0300 006a ef01 0000  ...h3]r....j....
-00005ab0: 2981 72b4 0300 007d 72b5 0300 0028 681e  ).r....}r....(h.
-00005ac0: 6ab2 0300 0068 277d 72b6 0300 0028 6829  j....h'}r....(h)
-00005ad0: 5d68 2a5d 682b 5d68 2c5d 682f 5d75 681f  ]h*]h+]h,]h/]uh.
-00005ae0: 6aaf 0300 0068 335d 72b7 0300 0068 5258  j....h3]r....hRX
-00005af0: 0400 0000 4e6f 6e65 72b8 0300 0085 8172  ....Noner......r
-00005b00: b903 0000 7d72 ba03 0000 2868 1e55 0068  ....}r....(h.U.h
-00005b10: 1f6a b403 0000 7562 6168 256a f701 0000  .j....ubah%j....
-00005b20: 7562 6168 2568 4075 6268 5258 0100 0000  ubah%h@ubhRX....
-00005b30: 2985 8172 bb03 0000 7d72 bc03 0000 2868  )..r....}r....(h
-00005b40: 1e55 0068 1f6a 8e03 0000 7562 6852 5805  .U.h.j....ubhRX.
-00005b50: 0000 0020 e280 9320 72bd 0300 0085 8172  ... ... r......r
-00005b60: be03 0000 7d72 bf03 0000 2868 1e55 0068  ....}r....(h.U.h
-00005b70: 1f6a 8e03 0000 7562 6897 2981 72c0 0300  .j....ubh.).r...
-00005b80: 007d 72c1 0300 0028 681e 5828 0000 004d  .}r....(h.X(...M
-00005b90: 696e 696d 697a 6174 696f 6e20 616c 676f  inimization algo
-00005ba0: 7269 7468 6d2e 204f 7074 696f 6e73 0a69  rithm. Options.i
-00005bb0: 6e63 6c75 6465 3a72 c203 0000 681f 6a8e  nclude:r....h.j.
-00005bc0: 0300 0068 236a 5901 0000 6825 689a 6827  ...h#jY...h%h.h'
-00005bd0: 7d72 c303 0000 2868 295d 682a 5d68 2b5d  }r....(h)]h*]h+]
-00005be0: 682c 5d68 2f5d 7568 314b 2368 3268 0268  h,]h/]uh1K#h2h.h
-00005bf0: 335d 72c4 0300 0068 5258 2800 0000 4d69  3]r....hRX(...Mi
-00005c00: 6e69 6d69 7a61 7469 6f6e 2061 6c67 6f72  nimization algor
-00005c10: 6974 686d 2e20 4f70 7469 6f6e 730a 696e  ithm. Options.in
-00005c20: 636c 7564 653a 72c5 0300 0085 8172 c603  clude:r......r..
-00005c30: 0000 7d72 c703 0000 2868 1e6a c203 0000  ..}r....(h.j....
-00005c40: 6823 4e68 314e 6832 6802 681f 6ac0 0300  h#Nh1Nh2h.h.j...
-00005c50: 0075 6261 7562 6ad5 0200 0029 8172 c803  .ubaubj....).r..
-00005c60: 0000 7d72 c903 0000 2868 1e55 0068 1f6a  ..}r....(h.U.h.j
-00005c70: 8e03 0000 6823 4e68 256a d802 0000 6827  ....h#Nh%j....h'
-00005c80: 7d72 ca03 0000 2868 295d 682a 5d68 2b5d  }r....(h)]h*]h+]
-00005c90: 682c 5d68 2f5d 7568 314e 6832 6802 6833  h,]h/]uh1Nh2h.h3
-00005ca0: 5d72 cb03 0000 6364 6f63 7574 696c 732e  ]r....cdocutils.
-00005cb0: 6e6f 6465 730a 6465 6669 6e69 7469 6f6e  nodes.definition
-00005cc0: 5f6c 6973 740a 72cc 0300 0029 8172 cd03  _list.r....).r..
-00005cd0: 0000 7d72 ce03 0000 2868 1e55 0068 277d  ..}r....(h.U.h'}
-00005ce0: 72cf 0300 0028 6829 5d68 2a5d 682b 5d68  r....(h)]h*]h+]h
-00005cf0: 2c5d 682f 5d75 681f 6ac8 0300 0068 335d  ,]h/]uh.j....h3]
-00005d00: 72d0 0300 0028 6364 6f63 7574 696c 732e  r....(cdocutils.
-00005d10: 6e6f 6465 730a 6465 6669 6e69 7469 6f6e  nodes.definition
-00005d20: 5f6c 6973 745f 6974 656d 0a72 d103 0000  _list_item.r....
-00005d30: 2981 72d2 0300 007d 72d3 0300 0028 681e  ).r....}r....(h.
-00005d40: 585e 0000 0060 6027 7472 6627 6060 0a54  X^...``'trf'``.T
-00005d50: 7275 7374 6564 2052 6567 696f 6e20 5265  rusted Region Re
-00005d60: 666c 6563 7469 7665 2061 6c67 6f72 6974  flective algorit
-00005d70: 686d 2028 6465 6661 756c 7429 2e20 4265  hm (default). Be
-00005d80: 7374 0a63 686f 6963 6520 7769 7468 2062  st.choice with b
-00005d90: 6f75 6e64 6564 2070 6172 616d 6574 6572  ounded parameter
-00005da0: 732e 0a68 1f6a cd03 0000 6823 6a59 0100  s..h.j....h#jY..
-00005db0: 0068 2555 1464 6566 696e 6974 696f 6e5f  .h%U.definition_
-00005dc0: 6c69 7374 5f69 7465 6d72 d403 0000 6827  list_itemr....h'
-00005dd0: 7d72 d503 0000 2868 295d 682a 5d68 2b5d  }r....(h)]h*]h+]
-00005de0: 682c 5d68 2f5d 7568 314b 2868 335d 72d6  h,]h/]uh1K(h3]r.
-00005df0: 0300 0028 6364 6f63 7574 696c 732e 6e6f  ...(cdocutils.no
-00005e00: 6465 730a 7465 726d 0a72 d703 0000 2981  des.term.r....).
-00005e10: 72d8 0300 007d 72d9 0300 0028 681e 5809  r....}r....(h.X.
-00005e20: 0000 0060 6027 7472 6627 6060 72da 0300  ...``'trf'``r...
-00005e30: 0068 1f6a d203 0000 6823 6a59 0100 0068  .h.j....h#jY...h
-00005e40: 2555 0474 6572 6d72 db03 0000 6827 7d72  %U.termr....h'}r
-00005e50: dc03 0000 2868 295d 682a 5d68 2b5d 682c  ....(h)]h*]h+]h,
-00005e60: 5d68 2f5d 7568 314b 2868 335d 72dd 0300  ]h/]uh1K(h3]r...
-00005e70: 0068 4a29 8172 de03 0000 7d72 df03 0000  .hJ).r....}r....
-00005e80: 2868 1e6a da03 0000 6827 7d72 e003 0000  (h.j....h'}r....
-00005e90: 2868 295d 682a 5d68 2b5d 682c 5d68 2f5d  (h)]h*]h+]h,]h/]
-00005ea0: 7568 1f6a d803 0000 6833 5d72 e103 0000  uh.j....h3]r....
-00005eb0: 6852 5805 0000 0027 7472 6627 72e2 0300  hRX....'trf'r...
-00005ec0: 0085 8172 e303 0000 7d72 e403 0000 2868  ...r....}r....(h
-00005ed0: 1e55 0068 1f6a de03 0000 7562 6168 2568  .U.h.j....ubah%h
-00005ee0: 5675 6261 7562 6364 6f63 7574 696c 732e  Vubaubcdocutils.
-00005ef0: 6e6f 6465 730a 6465 6669 6e69 7469 6f6e  nodes.definition
-00005f00: 0a72 e503 0000 2981 72e6 0300 007d 72e7  .r....).r....}r.
-00005f10: 0300 0028 681e 5500 6827 7d72 e803 0000  ...(h.U.h'}r....
-00005f20: 2868 295d 682a 5d68 2b5d 682c 5d68 2f5d  (h)]h*]h+]h,]h/]
-00005f30: 7568 1f6a d203 0000 6833 5d72 e903 0000  uh.j....h3]r....
-00005f40: 6897 2981 72ea 0300 007d 72eb 0300 0028  h.).r....}r....(
-00005f50: 681e 5853 0000 0054 7275 7374 6564 2052  h.XS...Trusted R
-00005f60: 6567 696f 6e20 5265 666c 6563 7469 7665  egion Reflective
-00005f70: 2061 6c67 6f72 6974 686d 2028 6465 6661   algorithm (defa
-00005f80: 756c 7429 2e20 4265 7374 0a63 686f 6963  ult). Best.choic
-00005f90: 6520 7769 7468 2062 6f75 6e64 6564 2070  e with bounded p
-00005fa0: 6172 616d 6574 6572 732e 72ec 0300 0068  arameters.r....h
-00005fb0: 1f6a e603 0000 6823 6a59 0100 0068 2568  .j....h#jY...h%h
-00005fc0: 9a68 277d 72ed 0300 0028 6829 5d68 2a5d  .h'}r....(h)]h*]
-00005fd0: 682b 5d68 2c5d 682f 5d75 6831 4b27 6833  h+]h,]h/]uh1K'h3
-00005fe0: 5d72 ee03 0000 6852 5853 0000 0054 7275  ]r....hRXS...Tru
-00005ff0: 7374 6564 2052 6567 696f 6e20 5265 666c  sted Region Refl
-00006000: 6563 7469 7665 2061 6c67 6f72 6974 686d  ective algorithm
-00006010: 2028 6465 6661 756c 7429 2e20 4265 7374   (default). Best
-00006020: 0a63 686f 6963 6520 7769 7468 2062 6f75  .choice with bou
-00006030: 6e64 6564 2070 6172 616d 6574 6572 732e  nded parameters.
-00006040: 72ef 0300 0085 8172 f003 0000 7d72 f103  r......r....}r..
-00006050: 0000 2868 1e6a ec03 0000 681f 6aea 0300  ..(h.j....h.j...
-00006060: 0075 6261 7562 6168 2555 0a64 6566 696e  .ubaubah%U.defin
-00006070: 6974 696f 6e72 f203 0000 7562 6575 626a  itionr....ubeubj
-00006080: d103 0000 2981 72f3 0300 007d 72f4 0300  ....).r....}r...
-00006090: 0028 681e 583e 0000 0060 6027 646f 6762  .(h.X>...``'dogb
-000060a0: 6f78 2760 600a 646f 676c 6567 2061 6c67  ox'``.dogleg alg
-000060b0: 6f72 6974 686d 2061 6461 7074 6564 2066  orithm adapted f
-000060c0: 6f72 2062 6f75 6e64 6564 2070 6172 616d  or bounded param
-000060d0: 6574 6572 732e 0a68 1f6a cd03 0000 6823  eters..h.j....h#
-000060e0: 6a59 0100 0068 256a d403 0000 6827 7d72  jY...h%j....h'}r
-000060f0: f503 0000 2868 295d 682a 5d68 2b5d 682c  ....(h)]h*]h+]h,
-00006100: 5d68 2f5d 7568 314b 2b68 335d 72f6 0300  ]h/]uh1K+h3]r...
-00006110: 0028 6ad7 0300 0029 8172 f703 0000 7d72  .(j....).r....}r
-00006120: f803 0000 2868 1e58 0c00 0000 6060 2764  ....(h.X....``'d
-00006130: 6f67 626f 7827 6060 72f9 0300 0068 1f6a  ogbox'``r....h.j
-00006140: f303 0000 6823 6a59 0100 0068 256a db03  ....h#jY...h%j..
-00006150: 0000 6827 7d72 fa03 0000 2868 295d 682a  ..h'}r....(h)]h*
-00006160: 5d68 2b5d 682c 5d68 2f5d 7568 314b 2b68  ]h+]h,]h/]uh1K+h
-00006170: 335d 72fb 0300 0068 4a29 8172 fc03 0000  3]r....hJ).r....
-00006180: 7d72 fd03 0000 2868 1e6a f903 0000 6827  }r....(h.j....h'
-00006190: 7d72 fe03 0000 2868 295d 682a 5d68 2b5d  }r....(h)]h*]h+]
-000061a0: 682c 5d68 2f5d 7568 1f6a f703 0000 6833  h,]h/]uh.j....h3
-000061b0: 5d72 ff03 0000 6852 5808 0000 0027 646f  ]r....hRX....'do
-000061c0: 6762 6f78 2772 0004 0000 8581 7201 0400  gbox'r......r...
-000061d0: 007d 7202 0400 0028 681e 5500 681f 6afc  .}r....(h.U.h.j.
-000061e0: 0300 0075 6261 6825 6856 7562 6175 626a  ...ubah%hVubaubj
-000061f0: e503 0000 2981 7203 0400 007d 7204 0400  ....).r....}r...
-00006200: 0028 681e 5500 6827 7d72 0504 0000 2868  .(h.U.h'}r....(h
-00006210: 295d 682a 5d68 2b5d 682c 5d68 2f5d 7568  )]h*]h+]h,]h/]uh
-00006220: 1f6a f303 0000 6833 5d72 0604 0000 6897  .j....h3]r....h.
-00006230: 2981 7207 0400 007d 7208 0400 0028 681e  ).r....}r....(h.
-00006240: 5830 0000 0064 6f67 6c65 6720 616c 676f  X0...dogleg algo
-00006250: 7269 7468 6d20 6164 6170 7465 6420 666f  rithm adapted fo
-00006260: 7220 626f 756e 6465 6420 7061 7261 6d65  r bounded parame
-00006270: 7465 7273 2e72 0904 0000 681f 6a03 0400  ters.r....h.j...
-00006280: 0068 236a 5901 0000 6825 689a 6827 7d72  .h#jY...h%h.h'}r
-00006290: 0a04 0000 2868 295d 682a 5d68 2b5d 682c  ....(h)]h*]h+]h,
-000062a0: 5d68 2f5d 7568 314b 2b68 335d 720b 0400  ]h/]uh1K+h3]r...
-000062b0: 0068 5258 3000 0000 646f 676c 6567 2061  .hRX0...dogleg a
-000062c0: 6c67 6f72 6974 686d 2061 6461 7074 6564  lgorithm adapted
-000062d0: 2066 6f72 2062 6f75 6e64 6564 2070 6172   for bounded par
-000062e0: 616d 6574 6572 732e 720c 0400 0085 8172  ameters.r......r
-000062f0: 0d04 0000 7d72 0e04 0000 2868 1e6a 0904  ....}r....(h.j..
-00006300: 0000 681f 6a07 0400 0075 6261 7562 6168  ..h.j....ubaubah
-00006310: 256a f203 0000 7562 6575 626a d103 0000  %j....ubeubj....
-00006320: 2981 720f 0400 007d 7210 0400 0028 681e  ).r....}r....(h.
-00006330: 5899 0000 0060 6027 6c6d 2760 600a 4c65  X....``'lm'``.Le
-00006340: 7665 6e62 6572 672d 4d61 7271 7561 7264  venberg-Marquard
-00006350: 7420 616c 676f 7269 7468 6d20 6173 2069  t algorithm as i
-00006360: 6d70 6c65 6d65 6e74 6564 2069 6e20 4d49  mplemented in MI
-00006370: 4e50 4143 4b2e 0a42 6573 7420 666f 7220  NPACK..Best for 
-00006380: 736d 616c 6c65 7220 7072 6f62 6c65 6d73  smaller problems
-00006390: 2e20 446f 6573 206e 6f74 2077 6f72 6b20  . Does not work 
-000063a0: 7769 7468 2062 6f75 6e64 6564 0a70 6172  with bounded.par
-000063b0: 616d 6574 6572 7320 2862 6f75 6e64 7320  ameters (bounds 
-000063c0: 6172 6520 6967 6e6f 7265 6429 2e0a 681f  are ignored)..h.
-000063d0: 6acd 0300 0068 236a 5901 0000 6825 6ad4  j....h#jY...h%j.
-000063e0: 0300 0068 277d 7211 0400 0028 6829 5d68  ...h'}r....(h)]h
-000063f0: 2a5d 682b 5d68 2c5d 682f 5d75 6831 4b30  *]h+]h,]h/]uh1K0
-00006400: 6833 5d72 1204 0000 286a d703 0000 2981  h3]r....(j....).
-00006410: 7213 0400 007d 7214 0400 0028 681e 5808  r....}r....(h.X.
-00006420: 0000 0060 6027 6c6d 2760 6072 1504 0000  ...``'lm'``r....
-00006430: 681f 6a0f 0400 0068 236a 5901 0000 6825  h.j....h#jY...h%
-00006440: 6adb 0300 0068 277d 7216 0400 0028 6829  j....h'}r....(h)
-00006450: 5d68 2a5d 682b 5d68 2c5d 682f 5d75 6831  ]h*]h+]h,]h/]uh1
-00006460: 4b30 6833 5d72 1704 0000 684a 2981 7218  K0h3]r....hJ).r.
-00006470: 0400 007d 7219 0400 0028 681e 6a15 0400  ...}r....(h.j...
-00006480: 0068 277d 721a 0400 0028 6829 5d68 2a5d  .h'}r....(h)]h*]
-00006490: 682b 5d68 2c5d 682f 5d75 681f 6a13 0400  h+]h,]h/]uh.j...
-000064a0: 0068 335d 721b 0400 0068 5258 0400 0000  .h3]r....hRX....
-000064b0: 276c 6d27 721c 0400 0085 8172 1d04 0000  'lm'r......r....
-000064c0: 7d72 1e04 0000 2868 1e55 0068 1f6a 1804  }r....(h.U.h.j..
-000064d0: 0000 7562 6168 2568 5675 6261 7562 6ae5  ..ubah%hVubaubj.
-000064e0: 0300 0029 8172 1f04 0000 7d72 2004 0000  ...).r....}r ...
-000064f0: 2868 1e55 0068 277d 7221 0400 0028 6829  (h.U.h'}r!...(h)
-00006500: 5d68 2a5d 682b 5d68 2c5d 682f 5d75 681f  ]h*]h+]h,]h/]uh.
-00006510: 6a0f 0400 0068 335d 7222 0400 0068 9729  j....h3]r"...h.)
-00006520: 8172 2304 0000 7d72 2404 0000 2868 1e58  .r#...}r$...(h.X
-00006530: 8f00 0000 4c65 7665 6e62 6572 672d 4d61  ....Levenberg-Ma
-00006540: 7271 7561 7264 7420 616c 676f 7269 7468  rquardt algorith
-00006550: 6d20 6173 2069 6d70 6c65 6d65 6e74 6564  m as implemented
-00006560: 2069 6e20 4d49 4e50 4143 4b2e 0a42 6573   in MINPACK..Bes
-00006570: 7420 666f 7220 736d 616c 6c65 7220 7072  t for smaller pr
-00006580: 6f62 6c65 6d73 2e20 446f 6573 206e 6f74  oblems. Does not
-00006590: 2077 6f72 6b20 7769 7468 2062 6f75 6e64   work with bound
-000065a0: 6564 0a70 6172 616d 6574 6572 7320 2862  ed.parameters (b
-000065b0: 6f75 6e64 7320 6172 6520 6967 6e6f 7265  ounds are ignore
-000065c0: 6429 2e72 2504 0000 681f 6a1f 0400 0068  d).r%...h.j....h
-000065d0: 236a 5901 0000 6825 689a 6827 7d72 2604  #jY...h%h.h'}r&.
-000065e0: 0000 2868 295d 682a 5d68 2b5d 682c 5d68  ..(h)]h*]h+]h,]h
-000065f0: 2f5d 7568 314b 2e68 335d 7227 0400 0068  /]uh1K.h3]r'...h
-00006600: 5258 8f00 0000 4c65 7665 6e62 6572 672d  RX....Levenberg-
-00006610: 4d61 7271 7561 7264 7420 616c 676f 7269  Marquardt algori
-00006620: 7468 6d20 6173 2069 6d70 6c65 6d65 6e74  thm as implement
-00006630: 6564 2069 6e20 4d49 4e50 4143 4b2e 0a42  ed in MINPACK..B
-00006640: 6573 7420 666f 7220 736d 616c 6c65 7220  est for smaller 
-00006650: 7072 6f62 6c65 6d73 2e20 446f 6573 206e  problems. Does n
-00006660: 6f74 2077 6f72 6b20 7769 7468 2062 6f75  ot work with bou
-00006670: 6e64 6564 0a70 6172 616d 6574 6572 7320  nded.parameters 
-00006680: 2862 6f75 6e64 7320 6172 6520 6967 6e6f  (bounds are igno
-00006690: 7265 6429 2e72 2804 0000 8581 7229 0400  red).r(.....r)..
-000066a0: 007d 722a 0400 0028 681e 6a25 0400 0068  .}r*...(h.j%...h
-000066b0: 1f6a 2304 0000 7562 6175 6261 6825 6af2  .j#...ubaubah%j.
-000066c0: 0300 0075 6265 7562 6568 2555 0f64 6566  ...ubeubeh%U.def
-000066d0: 696e 6974 696f 6e5f 6c69 7374 722b 0400  inition_listr+..
-000066e0: 0075 6261 7562 6897 2981 722c 0400 007d  .ubaubh.).r,...}
-000066f0: 722d 0400 0028 681e 5836 0000 0053 6574  r-...(h.X6...Set
-00006700: 7469 6e67 2060 606d 6574 686f 643d 4e6f  ting ``method=No
-00006710: 6e65 6060 2069 6d70 6c69 6573 2074 6865  ne`` implies the
-00006720: 2064 6566 6175 6c74 2060 6027 7472 6627   default ``'trf'
-00006730: 6060 2e68 1f6a 8e03 0000 6823 6a59 0100  ``.h.j....h#jY..
-00006740: 0068 2568 9a68 277d 722e 0400 0028 6829  .h%h.h'}r....(h)
-00006750: 5d68 2a5d 682b 5d68 2c5d 682f 5d75 6831  ]h*]h+]h,]h/]uh1
-00006760: 4b32 6832 6802 6833 5d72 2f04 0000 2868  K2h2h.h3]r/...(h
-00006770: 5258 0800 0000 5365 7474 696e 6720 7230  RX....Setting r0
-00006780: 0400 0085 8172 3104 0000 7d72 3204 0000  .....r1...}r2...
-00006790: 2868 1e58 0800 0000 5365 7474 696e 6720  (h.X....Setting 
-000067a0: 6823 4e68 314e 6832 6802 681f 6a2c 0400  h#Nh1Nh2h.h.j,..
-000067b0: 0075 6268 4a29 8172 3304 0000 7d72 3404  .ubhJ).r3...}r4.
-000067c0: 0000 2868 1e58 0f00 0000 6060 6d65 7468  ..(h.X....``meth
-000067d0: 6f64 3d4e 6f6e 6560 6068 277d 7235 0400  od=None``h'}r5..
-000067e0: 0028 6829 5d68 2a5d 682b 5d68 2c5d 682f  .(h)]h*]h+]h,]h/
-000067f0: 5d75 681f 6a2c 0400 0068 335d 7236 0400  ]uh.j,...h3]r6..
-00006800: 0068 5258 0b00 0000 6d65 7468 6f64 3d4e  .hRX....method=N
-00006810: 6f6e 6572 3704 0000 8581 7238 0400 007d  oner7.....r8...}
-00006820: 7239 0400 0028 681e 5500 681f 6a33 0400  r9...(h.U.h.j3..
-00006830: 0075 6261 6825 6856 7562 6852 5815 0000  .ubah%hVubhRX...
-00006840: 0020 696d 706c 6965 7320 7468 6520 6465  . implies the de
-00006850: 6661 756c 7420 723a 0400 0085 8172 3b04  fault r:.....r;.
-00006860: 0000 7d72 3c04 0000 2868 1e58 1500 0000  ..}r<...(h.X....
-00006870: 2069 6d70 6c69 6573 2074 6865 2064 6566   implies the def
-00006880: 6175 6c74 2068 234e 6831 4e68 3268 0268  ault h#Nh1Nh2h.h
-00006890: 1f6a 2c04 0000 7562 684a 2981 723d 0400  .j,...ubhJ).r=..
-000068a0: 007d 723e 0400 0028 681e 5809 0000 0060  .}r>...(h.X....`
-000068b0: 6027 7472 6627 6060 6827 7d72 3f04 0000  `'trf'``h'}r?...
-000068c0: 2868 295d 682a 5d68 2b5d 682c 5d68 2f5d  (h)]h*]h+]h,]h/]
-000068d0: 7568 1f6a 2c04 0000 6833 5d72 4004 0000  uh.j,...h3]r@...
-000068e0: 6852 5805 0000 0027 7472 6627 7241 0400  hRX....'trf'rA..
-000068f0: 0085 8172 4204 0000 7d72 4304 0000 2868  ...rB...}rC...(h
-00006900: 1e55 0068 1f6a 3d04 0000 7562 6168 2568  .U.h.j=...ubah%h
-00006910: 5675 6268 5258 0100 0000 2e85 8172 4404  VubhRX.......rD.
-00006920: 0000 7d72 4504 0000 2868 1e58 0100 0000  ..}rE...(h.X....
-00006930: 2e68 234e 6831 4e68 3268 0268 1f6a 2c04  .h#Nh1Nh2h.h.j,.
-00006940: 0000 7562 6575 6265 6825 689a 7562 6168  ..ubeubeh%h.ubah
-00006950: 256a 0102 0000 7562 6ad4 0100 0029 8172  %j....ubj....).r
-00006960: 4604 0000 7d72 4704 0000 2868 1e55 0068  F...}rG...(h.U.h
-00006970: 277d 7248 0400 0028 6829 5d68 2a5d 682b  '}rH...(h)]h*]h+
-00006980: 5d68 2c5d 682f 5d75 681f 6ad0 0100 0068  ]h,]h/]uh.j....h
-00006990: 335d 7249 0400 0068 9729 8172 4a04 0000  3]rI...h.).rJ...
-000069a0: 7d72 4b04 0000 2868 1e58 5d00 0000 6d61  }rK...(h.X]...ma
-000069b0: 7869 7420 2869 6e74 2920 2d2d 204d 6178  xit (int) -- Max
-000069c0: 696d 756d 206e 756d 6265 7220 6f66 2066  imum number of f
-000069d0: 756e 6374 696f 6e20 6576 616c 7561 7469  unction evaluati
-000069e0: 6f6e 7320 696e 2073 6561 7263 680a 666f  ons in search.fo
-000069f0: 7220 6d69 6e69 6d75 6d3b 2064 6566 6175  r minimum; defau
-00006a00: 6c74 2069 7320 3130 3030 2e68 277d 724c  lt is 1000.h'}rL
-00006a10: 0400 0028 6829 5d68 2a5d 682b 5d68 2c5d  ...(h)]h*]h+]h,]
-00006a20: 682f 5d75 681f 6a46 0400 0068 335d 724d  h/]uh.jF...h3]rM
-00006a30: 0400 0028 6add 0100 0029 8172 4e04 0000  ...(j....).rN...
-00006a40: 7d72 4f04 0000 2868 1e58 0500 0000 6d61  }rO...(h.X....ma
-00006a50: 7869 7468 277d 7250 0400 0028 682c 5d68  xith'}rP...(h,]h
-00006a60: 2b5d 6ae1 0100 0088 6829 5d68 2a5d 682f  +]j.....h)]h*]h/
-00006a70: 5d75 681f 6a4a 0400 0068 335d 7251 0400  ]uh.jJ...h3]rQ..
-00006a80: 0068 5258 0500 0000 6d61 7869 7472 5204  .hRX....maxitrR.
-00006a90: 0000 8581 7253 0400 007d 7254 0400 0028  ....rS...}rT...(
-00006aa0: 681e 5500 681f 6a4e 0400 0075 6261 6825  h.U.h.jN...ubah%
-00006ab0: 6ae6 0100 0075 6268 5258 0200 0000 2028  j....ubhRX.... (
-00006ac0: 7255 0400 0085 8172 5604 0000 7d72 5704  rU.....rV...}rW.
-00006ad0: 0000 2868 1e55 0068 1f6a 4a04 0000 7562  ..(h.U.h.jJ...ub
-00006ae0: 683c 2981 7258 0400 007d 7259 0400 0028  h<).rX...}rY...(
-00006af0: 681e 5500 6827 7d72 5a04 0000 2855 0772  h.U.h'}rZ...(U.r
-00006b00: 6566 7479 7065 68f2 6ae1 0100 0088 5509  eftypeh.j.....U.
-00006b10: 7265 6674 6172 6765 7458 0300 0000 696e  reftargetX....in
-00006b20: 7472 5b04 0000 5509 7265 6664 6f6d 6169  tr[...U.refdomai
-00006b30: 6e68 de68 2c5d 682b 5d55 0b72 6566 6578  nh.h,]h+]U.refex
-00006b40: 706c 6963 6974 8968 295d 682a 5d68 2f5d  plicit.h)]h*]h/]
-00006b50: 7568 1f6a 4a04 0000 6833 5d72 5c04 0000  uh.jJ...h3]r\...
-00006b60: 6aef 0100 0029 8172 5d04 0000 7d72 5e04  j....).r]...}r^.
-00006b70: 0000 2868 1e6a 5b04 0000 6827 7d72 5f04  ..(h.j[...h'}r_.
-00006b80: 0000 2868 295d 682a 5d68 2b5d 682c 5d68  ..(h)]h*]h+]h,]h
-00006b90: 2f5d 7568 1f6a 5804 0000 6833 5d72 6004  /]uh.jX...h3]r`.
-00006ba0: 0000 6852 5803 0000 0069 6e74 7261 0400  ..hRX....intra..
-00006bb0: 0085 8172 6204 0000 7d72 6304 0000 2868  ...rb...}rc...(h
-00006bc0: 1e55 0068 1f6a 5d04 0000 7562 6168 256a  .U.h.j]...ubah%j
-00006bd0: f701 0000 7562 6168 2568 4075 6268 5258  ....ubah%h@ubhRX
-00006be0: 0100 0000 2985 8172 6404 0000 7d72 6504  ....)..rd...}re.
-00006bf0: 0000 2868 1e55 0068 1f6a 4a04 0000 7562  ..(h.U.h.jJ...ub
-00006c00: 6852 5805 0000 0020 e280 9320 7266 0400  hRX.... ... rf..
-00006c10: 0085 8172 6704 0000 7d72 6804 0000 2868  ...rg...}rh...(h
-00006c20: 1e55 0068 1f6a 4a04 0000 7562 6852 584e  .U.h.jJ...ubhRXN
-00006c30: 0000 004d 6178 696d 756d 206e 756d 6265  ...Maximum numbe
-00006c40: 7220 6f66 2066 756e 6374 696f 6e20 6576  r of function ev
-00006c50: 616c 7561 7469 6f6e 7320 696e 2073 6561  aluations in sea
-00006c60: 7263 680a 666f 7220 6d69 6e69 6d75 6d3b  rch.for minimum;
-00006c70: 2064 6566 6175 6c74 2069 7320 3130 3030   default is 1000
-00006c80: 2e72 6904 0000 8581 726a 0400 007d 726b  .ri.....rj...}rk
-00006c90: 0400 0028 681e 584e 0000 004d 6178 696d  ...(h.XN...Maxim
-00006ca0: 756d 206e 756d 6265 7220 6f66 2066 756e  um number of fun
-00006cb0: 6374 696f 6e20 6576 616c 7561 7469 6f6e  ction evaluation
-00006cc0: 7320 696e 2073 6561 7263 680a 666f 7220  s in search.for 
-00006cd0: 6d69 6e69 6d75 6d3b 2064 6566 6175 6c74  minimum; default
-00006ce0: 2069 7320 3130 3030 2e72 6c04 0000 6823   is 1000.rl...h#
-00006cf0: 4e68 314e 6832 6802 681f 6a4a 0400 0075  Nh1Nh2h.h.jJ...u
-00006d00: 6265 6825 689a 7562 6168 256a 0102 0000  beh%h.ubah%j....
-00006d10: 7562 6568 2555 0b62 756c 6c65 745f 6c69  ubeh%U.bullet_li
-00006d20: 7374 726d 0400 0075 6261 6825 550a 6669  strm...ubah%U.fi
-00006d30: 656c 645f 626f 6479 726e 0400 0075 6265  eld_bodyrn...ube
-00006d40: 6825 5505 6669 656c 6472 6f04 0000 7562  h%U.fieldro...ub
-00006d50: 6175 6268 9729 8172 7004 0000 7d72 7104  aubh.).rp...}rq.
-00006d60: 0000 2868 1e58 cf00 0000 4f74 6865 7220  ..(h.X....Other 
-00006d70: 6172 6775 6d65 6e74 7320 696e 636c 7564  arguments includ
-00006d80: 653a 2060 6078 5f6a 6163 6060 2c20 6060  e: ``x_jac``, ``
-00006d90: 6c6f 7373 6060 2c20 6060 7472 5f73 6f6c  loss``, ``tr_sol
-00006da0: 7665 7260 602c 0a60 6066 5f73 6361 6c65  ver``,.``f_scale
-00006db0: 6060 2c20 6060 7472 5f6f 7074 696f 6e73  ``, ``tr_options
-00006dc0: 6060 2c20 6060 626f 756e 6473 6060 2e20  ``, ``bounds``. 
-00006dd0: 5365 6520 7468 6520 646f 6375 6d65 6e74  See the document
-00006de0: 6174 696f 6e20 666f 720a 6060 7363 6970  ation for.``scip
-00006df0: 792e 6f70 7469 6d69 7a65 2e6c 6561 7374  y.optimize.least
-00006e00: 5f73 7175 6172 6573 6060 2066 6f72 2069  _squares`` for i
-00006e10: 6e66 6f72 6d61 7469 6f6e 2061 626f 7574  nformation about
-00006e20: 2074 6865 7365 2061 6e64 206f 7468 6572   these and other
-00006e30: 0a6f 7074 696f 6e73 2e68 1f6a 5101 0000  .options.h.jQ...
-00006e40: 6823 6a59 0100 0068 2568 9a68 277d 7272  h#jY...h%h.h'}rr
-00006e50: 0400 0028 6829 5d68 2a5d 682b 5d68 2c5d  ...(h)]h*]h+]h,]
-00006e60: 682f 5d75 6831 4b38 6832 6802 6833 5d72  h/]uh1K8h2h.h3]r
-00006e70: 7304 0000 2868 5258 1900 0000 4f74 6865  s...(hRX....Othe
-00006e80: 7220 6172 6775 6d65 6e74 7320 696e 636c  r arguments incl
-00006e90: 7564 653a 2072 7404 0000 8581 7275 0400  ude: rt.....ru..
-00006ea0: 007d 7276 0400 0028 681e 5819 0000 004f  .}rv...(h.X....O
-00006eb0: 7468 6572 2061 7267 756d 656e 7473 2069  ther arguments i
-00006ec0: 6e63 6c75 6465 3a20 6823 4e68 314e 6832  nclude: h#Nh1Nh2
-00006ed0: 6802 681f 6a70 0400 0075 6268 4a29 8172  h.h.jp...ubhJ).r
-00006ee0: 7704 0000 7d72 7804 0000 2868 1e58 0900  w...}rx...(h.X..
-00006ef0: 0000 6060 785f 6a61 6360 6068 277d 7279  ..``x_jac``h'}ry
-00006f00: 0400 0028 6829 5d68 2a5d 682b 5d68 2c5d  ...(h)]h*]h+]h,]
-00006f10: 682f 5d75 681f 6a70 0400 0068 335d 727a  h/]uh.jp...h3]rz
-00006f20: 0400 0068 5258 0500 0000 785f 6a61 6372  ...hRX....x_jacr
-00006f30: 7b04 0000 8581 727c 0400 007d 727d 0400  {.....r|...}r}..
-00006f40: 0028 681e 5500 681f 6a77 0400 0075 6261  .(h.U.h.jw...uba
-00006f50: 6825 6856 7562 6852 5802 0000 002c 2072  h%hVubhRX...., r
-00006f60: 7e04 0000 8581 727f 0400 007d 7280 0400  ~.....r....}r...
-00006f70: 0028 681e 5802 0000 002c 2072 8104 0000  .(h.X...., r....
-00006f80: 6823 4e68 314e 6832 6802 681f 6a70 0400  h#Nh1Nh2h.h.jp..
-00006f90: 0075 6268 4a29 8172 8204 0000 7d72 8304  .ubhJ).r....}r..
-00006fa0: 0000 2868 1e58 0800 0000 6060 6c6f 7373  ..(h.X....``loss
-00006fb0: 6060 6827 7d72 8404 0000 2868 295d 682a  ``h'}r....(h)]h*
-00006fc0: 5d68 2b5d 682c 5d68 2f5d 7568 1f6a 7004  ]h+]h,]h/]uh.jp.
-00006fd0: 0000 6833 5d72 8504 0000 6852 5804 0000  ..h3]r....hRX...
-00006fe0: 006c 6f73 7372 8604 0000 8581 7287 0400  .lossr......r...
-00006ff0: 007d 7288 0400 0028 681e 5500 681f 6a82  .}r....(h.U.h.j.
-00007000: 0400 0075 6261 6825 6856 7562 6852 5802  ...ubah%hVubhRX.
-00007010: 0000 002c 2072 8904 0000 8581 728a 0400  ..., r......r...
-00007020: 007d 728b 0400 0028 681e 5802 0000 002c  .}r....(h.X....,
-00007030: 2068 1f6a 7004 0000 7562 684a 2981 728c   h.jp...ubhJ).r.
-00007040: 0400 007d 728d 0400 0028 681e 580d 0000  ...}r....(h.X...
-00007050: 0060 6074 725f 736f 6c76 6572 6060 6827  .``tr_solver``h'
-00007060: 7d72 8e04 0000 2868 295d 682a 5d68 2b5d  }r....(h)]h*]h+]
-00007070: 682c 5d68 2f5d 7568 1f6a 7004 0000 6833  h,]h/]uh.jp...h3
-00007080: 5d72 8f04 0000 6852 5809 0000 0074 725f  ]r....hRX....tr_
-00007090: 736f 6c76 6572 7290 0400 0085 8172 9104  solverr......r..
-000070a0: 0000 7d72 9204 0000 2868 1e55 0068 1f6a  ..}r....(h.U.h.j
-000070b0: 8c04 0000 7562 6168 2568 5675 6268 5258  ....ubah%hVubhRX
-000070c0: 0200 0000 2c0a 7293 0400 0085 8172 9404  ....,.r......r..
-000070d0: 0000 7d72 9504 0000 2868 1e58 0200 0000  ..}r....(h.X....
-000070e0: 2c0a 6823 4e68 314e 6832 6802 681f 6a70  ,.h#Nh1Nh2h.h.jp
-000070f0: 0400 0075 6268 4a29 8172 9604 0000 7d72  ...ubhJ).r....}r
-00007100: 9704 0000 2868 1e58 0b00 0000 6060 665f  ....(h.X....``f_
-00007110: 7363 616c 6560 6068 277d 7298 0400 0028  scale``h'}r....(
-00007120: 6829 5d68 2a5d 682b 5d68 2c5d 682f 5d75  h)]h*]h+]h,]h/]u
-00007130: 681f 6a70 0400 0068 335d 7299 0400 0068  h.jp...h3]r....h
-00007140: 5258 0700 0000 665f 7363 616c 6572 9a04  RX....f_scaler..
-00007150: 0000 8581 729b 0400 007d 729c 0400 0028  ....r....}r....(
-00007160: 681e 5500 681f 6a96 0400 0075 6261 6825  h.U.h.j....ubah%
-00007170: 6856 7562 6852 5802 0000 002c 2072 9d04  hVubhRX...., r..
-00007180: 0000 8581 729e 0400 007d 729f 0400 0028  ....r....}r....(
-00007190: 681e 5802 0000 002c 2068 1f6a 7004 0000  h.X...., h.jp...
-000071a0: 7562 684a 2981 72a0 0400 007d 72a1 0400  ubhJ).r....}r...
-000071b0: 0028 681e 580e 0000 0060 6074 725f 6f70  .(h.X....``tr_op
-000071c0: 7469 6f6e 7360 6068 277d 72a2 0400 0028  tions``h'}r....(
-000071d0: 6829 5d68 2a5d 682b 5d68 2c5d 682f 5d75  h)]h*]h+]h,]h/]u
-000071e0: 681f 6a70 0400 0068 335d 72a3 0400 0068  h.jp...h3]r....h
-000071f0: 5258 0a00 0000 7472 5f6f 7074 696f 6e73  RX....tr_options
-00007200: 72a4 0400 0085 8172 a504 0000 7d72 a604  r......r....}r..
-00007210: 0000 2868 1e55 0068 1f6a a004 0000 7562  ..(h.U.h.j....ub
-00007220: 6168 2568 5675 6268 5258 0200 0000 2c20  ah%hVubhRX...., 
-00007230: 72a7 0400 0085 8172 a804 0000 7d72 a904  r......r....}r..
-00007240: 0000 2868 1e6a 8104 0000 681f 6a70 0400  ..(h.j....h.jp..
-00007250: 0075 6268 4a29 8172 aa04 0000 7d72 ab04  .ubhJ).r....}r..
-00007260: 0000 2868 1e58 0a00 0000 6060 626f 756e  ..(h.X....``boun
-00007270: 6473 6060 6827 7d72 ac04 0000 2868 295d  ds``h'}r....(h)]
-00007280: 682a 5d68 2b5d 682c 5d68 2f5d 7568 1f6a  h*]h+]h,]h/]uh.j
-00007290: 7004 0000 6833 5d72 ad04 0000 6852 5806  p...h3]r....hRX.
-000072a0: 0000 0062 6f75 6e64 7372 ae04 0000 8581  ...boundsr......
-000072b0: 72af 0400 007d 72b0 0400 0028 681e 5500  r....}r....(h.U.
-000072c0: 681f 6aaa 0400 0075 6261 6825 6856 7562  h.j....ubah%hVub
-000072d0: 6852 581c 0000 002e 2053 6565 2074 6865  hRX..... See the
-000072e0: 2064 6f63 756d 656e 7461 7469 6f6e 2066   documentation f
-000072f0: 6f72 0a72 b104 0000 8581 72b2 0400 007d  or.r......r....}
-00007300: 72b3 0400 0028 681e 581c 0000 002e 2053  r....(h.X..... S
-00007310: 6565 2074 6865 2064 6f63 756d 656e 7461  ee the documenta
-00007320: 7469 6f6e 2066 6f72 0a68 234e 6831 4e68  tion for.h#Nh1Nh
-00007330: 3268 0268 1f6a 7004 0000 7562 684a 2981  2h.h.jp...ubhJ).
-00007340: 72b4 0400 007d 72b5 0400 0028 681e 5820  r....}r....(h.X 
-00007350: 0000 0060 6073 6369 7079 2e6f 7074 696d  ...``scipy.optim
-00007360: 697a 652e 6c65 6173 745f 7371 7561 7265  ize.least_square
-00007370: 7360 6068 277d 72b6 0400 0028 6829 5d68  s``h'}r....(h)]h
-00007380: 2a5d 682b 5d68 2c5d 682f 5d75 681f 6a70  *]h+]h,]h/]uh.jp
-00007390: 0400 0068 335d 72b7 0400 0068 5258 1c00  ...h3]r....hRX..
-000073a0: 0000 7363 6970 792e 6f70 7469 6d69 7a65  ..scipy.optimize
-000073b0: 2e6c 6561 7374 5f73 7175 6172 6573 72b8  .least_squaresr.
-000073c0: 0400 0085 8172 b904 0000 7d72 ba04 0000  .....r....}r....
-000073d0: 2868 1e55 0068 1f6a b404 0000 7562 6168  (h.U.h.j....ubah
-000073e0: 2568 5675 6268 5258 2f00 0000 2066 6f72  %hVubhRX/... for
-000073f0: 2069 6e66 6f72 6d61 7469 6f6e 2061 626f   information abo
-00007400: 7574 2074 6865 7365 2061 6e64 206f 7468  ut these and oth
-00007410: 6572 0a6f 7074 696f 6e73 2e72 bb04 0000  er.options.r....
-00007420: 8581 72bc 0400 007d 72bd 0400 0028 681e  ..r....}r....(h.
-00007430: 582f 0000 0020 666f 7220 696e 666f 726d  X/... for inform
-00007440: 6174 696f 6e20 6162 6f75 7420 7468 6573  ation about thes
-00007450: 6520 616e 6420 6f74 6865 720a 6f70 7469  e and other.opti
-00007460: 6f6e 732e 6823 4e68 314e 6832 6802 681f  ons.h#Nh1Nh2h.h.
-00007470: 6a70 0400 0075 6265 7562 6897 2981 72be  jp...ubeubh.).r.
-00007480: 0400 007d 72bf 0400 0028 681e 584a 0000  ...}r....(h.XJ..
-00007490: 003a 636c 6173 733a 606c 7371 6669 742e  .:class:`lsqfit.
-000074a0: 7363 6970 795f 6c65 6173 745f 7371 7561  scipy_least_squa
-000074b0: 7265 7360 206f 626a 6563 7473 2068 6176  res` objects hav
-000074c0: 6520 7468 6520 666f 6c6c 6f77 696e 670a  e the following.
-000074d0: 6174 7472 6962 7574 6573 2e68 1f6a 5101  attributes.h.jQ.
-000074e0: 0000 6823 6a59 0100 0068 2568 9a68 277d  ..h#jY...h%h.h'}
-000074f0: 72c0 0400 0028 6829 5d68 2a5d 682b 5d68  r....(h)]h*]h+]h
-00007500: 2c5d 682f 5d75 6831 4b3d 6832 6802 6833  ,]h/]uh1K=h2h.h3
-00007510: 5d72 c104 0000 2868 3c29 8172 c204 0000  ]r....(h<).r....
-00007520: 7d72 c304 0000 2868 1e58 2300 0000 3a63  }r....(h.X#...:c
-00007530: 6c61 7373 3a60 6c73 7166 6974 2e73 6369  lass:`lsqfit.sci
-00007540: 7079 5f6c 6561 7374 5f73 7175 6172 6573  py_least_squares
-00007550: 6072 c404 0000 681f 6abe 0400 0068 236a  `r....h.j....h#j
-00007560: 5901 0000 6825 6840 6827 7d72 c504 0000  Y...h%h@h'}r....
-00007570: 2855 0772 6566 7479 7065 5805 0000 0063  (U.reftypeX....c
-00007580: 6c61 7373 6842 8968 4358 1a00 0000 6c73  lasshB.hCX....ls
-00007590: 7166 6974 2e73 6369 7079 5f6c 6561 7374  qfit.scipy_least
-000075a0: 5f73 7175 6172 6573 5509 7265 6664 6f6d  _squaresU.refdom
-000075b0: 6169 6e58 0200 0000 7079 72c6 0400 0068  ainX....pyr....h
-000075c0: 2c5d 682b 5d55 0b72 6566 6578 706c 6963  ,]h+]U.refexplic
-000075d0: 6974 8968 295d 682a 5d68 2f5d 6845 6846  it.h)]h*]h/]hEhF
-000075e0: 6847 68f1 6848 68ed 7568 314b 3d68 335d  hGh.hHh.uh1K=h3]
-000075f0: 72c7 0400 0068 4a29 8172 c804 0000 7d72  r....hJ).r....}r
-00007600: c904 0000 2868 1e6a c404 0000 6827 7d72  ....(h.j....h'}r
-00007610: ca04 0000 2868 295d 682a 5d72 cb04 0000  ....(h)]h*]r....
-00007620: 2868 4f6a c604 0000 5808 0000 0070 792d  (hOj....X....py-
-00007630: 636c 6173 7372 cc04 0000 6568 2b5d 682c  classr....eh+]h,
-00007640: 5d68 2f5d 7568 1f6a c204 0000 6833 5d72  ]h/]uh.j....h3]r
-00007650: cd04 0000 6852 581a 0000 006c 7371 6669  ....hRX....lsqfi
-00007660: 742e 7363 6970 795f 6c65 6173 745f 7371  t.scipy_least_sq
-00007670: 7561 7265 7372 ce04 0000 8581 72cf 0400  uaresr......r...
-00007680: 007d 72d0 0400 0028 681e 5500 681f 6ac8  .}r....(h.U.h.j.
-00007690: 0400 0075 6261 6825 6856 7562 6175 6268  ...ubah%hVubaubh
-000076a0: 5258 2700 0000 206f 626a 6563 7473 2068  RX'... objects h
-000076b0: 6176 6520 7468 6520 666f 6c6c 6f77 696e  ave the followin
-000076c0: 670a 6174 7472 6962 7574 6573 2e72 d104  g.attributes.r..
-000076d0: 0000 8581 72d2 0400 007d 72d3 0400 0028  ....r....}r....(
-000076e0: 681e 5827 0000 0020 6f62 6a65 6374 7320  h.X'... objects 
-000076f0: 6861 7665 2074 6865 2066 6f6c 6c6f 7769  have the followi
-00007700: 6e67 0a61 7474 7269 6275 7465 732e 6823  ng.attributes.h#
-00007710: 4e68 314e 6832 6802 681f 6abe 0400 0075  Nh1Nh2h.h.j....u
-00007720: 6265 7562 68cf 2981 72d4 0400 007d 72d5  beubh.).r....}r.
-00007730: 0400 0028 681e 5500 681f 6a51 0100 0068  ...(h.U.h.jQ...h
-00007740: 236a 5901 0000 6825 68d2 6827 7d72 d604  #jY...h%h.h'}r..
-00007750: 0000 2868 2c5d 682b 5d68 295d 682a 5d68  ..(h,]h+]h)]h*]h
-00007760: 2f5d 5507 656e 7472 6965 735d 72d7 0400  /]U.entries]r...
-00007770: 0028 68d5 5828 0000 0078 2028 6c73 7166  .(h.X(...x (lsqf
-00007780: 6974 2e73 6369 7079 5f6c 6561 7374 5f73  it.scipy_least_s
-00007790: 7175 6172 6573 2061 7474 7269 6275 7465  quares attribute
-000077a0: 2968 1555 004e 7472 d804 0000 6175 6831  )h.U.Ntr....auh1
-000077b0: 4e68 3268 0268 335d 7562 68d7 2981 72d9  Nh2h.h3]ubh.).r.
-000077c0: 0400 007d 72da 0400 0028 681e 5500 681f  ...}r....(h.U.h.
-000077d0: 6a51 0100 0068 236a 5901 0000 6825 68da  jQ...h#jY...h%h.
-000077e0: 6827 7d72 db04 0000 2868 dc89 68dd 5802  h'}r....(h..h.X.
-000077f0: 0000 0070 7968 2c5d 682b 5d68 295d 682a  ...pyh,]h+]h)]h*
-00007800: 5d68 2f5d 68df 5809 0000 0061 7474 7269  ]h/]h.X....attri
-00007810: 6275 7465 72dc 0400 0068 e16a dc04 0000  buter....h.j....
-00007820: 7568 314e 6832 6802 6833 5d72 dd04 0000  uh1Nh2h.h3]r....
-00007830: 2868 e329 8172 de04 0000 7d72 df04 0000  (h.).r....}r....
-00007840: 2868 1e58 0100 0000 7868 1f6a d904 0000  (h.X....xh.j....
-00007850: 6823 6a59 0100 0068 2568 e768 277d 72e0  h#jY...h%h.h'}r.
-00007860: 0400 0028 682c 5d72 e104 0000 6815 6168  ...(h,]r....h.ah
-00007870: ea68 ed68 2b5d 6829 5d68 2a5d 682f 5d72  .h.h+]h)]h*]h/]r
-00007880: e204 0000 6815 6168 f058 1500 0000 7363  ....h.ah.X....sc
-00007890: 6970 795f 6c65 6173 745f 7371 7561 7265  ipy_least_square
-000078a0: 732e 7868 f268 f168 f389 7568 314b 4368  s.xh.h.h..uh1KCh
-000078b0: 3268 0268 335d 72e3 0400 006a 0901 0000  2h.h3]r....j....
-000078c0: 2981 72e4 0400 007d 72e5 0400 0028 681e  ).r....}r....(h.
-000078d0: 5801 0000 0078 681f 6ade 0400 0068 236a  X....xh.j....h#j
-000078e0: 5901 0000 6825 6a0c 0100 0068 277d 72e6  Y...h%j....h'}r.
-000078f0: 0400 0028 68fa 68fb 682c 5d68 2b5d 6829  ...(h.h.h,]h+]h)
-00007900: 5d68 2a5d 682f 5d75 6831 4b43 6832 6802  ]h*]h/]uh1KCh2h.
-00007910: 6833 5d72 e704 0000 6852 5801 0000 0078  h3]r....hRX....x
-00007920: 8581 72e8 0400 007d 72e9 0400 0028 681e  ..r....}r....(h.
-00007930: 5500 6823 4e68 314e 6832 6802 681f 6ae4  U.h#Nh1Nh2h.h.j.
-00007940: 0400 0075 6261 7562 6175 626a 5001 0000  ...ubaubaubjP...
-00007950: 2981 72ea 0400 007d 72eb 0400 0028 681e  ).r....}r....(h.
-00007960: 5500 681f 6ad9 0400 0068 236a 5901 0000  U.h.j....h#jY...
-00007970: 6825 6a53 0100 0068 277d 72ec 0400 0028  h%jS...h'}r....(
-00007980: 6829 5d68 2a5d 682b 5d68 2c5d 682f 5d75  h)]h*]h+]h,]h/]u
-00007990: 6831 4b43 6832 6802 6833 5d72 ed04 0000  h1KCh2h.h3]r....
-000079a0: 6897 2981 72ee 0400 007d 72ef 0400 0028  h.).r....}r....(
-000079b0: 681e 5843 0000 002a 6172 7261 792a 202d  h.XC...*array* -
-000079c0: 2d20 4c6f 6361 7469 6f6e 206f 6620 7468  - Location of th
-000079d0: 6520 6d6f 7374 2072 6563 656e 746c 7920  e most recently 
-000079e0: 636f 6d70 7574 6564 2028 6265 7374 2920  computed (best) 
-000079f0: 6669 7420 706f 696e 742e 681f 6aea 0400  fit point.h.j...
-00007a00: 0068 236a 5901 0000 6825 689a 6827 7d72  .h#jY...h%h.h'}r
-00007a10: f004 0000 2868 295d 682a 5d68 2b5d 682c  ....(h)]h*]h+]h,
-00007a20: 5d68 2f5d 7568 314b 4268 3268 0268 335d  ]h/]uh1KBh2h.h3]
-00007a30: 72f1 0400 0028 6364 6f63 7574 696c 732e  r....(cdocutils.
-00007a40: 6e6f 6465 730a 656d 7068 6173 6973 0a72  nodes.emphasis.r
-00007a50: f204 0000 2981 72f3 0400 007d 72f4 0400  ....).r....}r...
-00007a60: 0028 681e 5807 0000 002a 6172 7261 792a  .(h.X....*array*
-00007a70: 6827 7d72 f504 0000 2868 295d 682a 5d68  h'}r....(h)]h*]h
-00007a80: 2b5d 682c 5d68 2f5d 7568 1f6a ee04 0000  +]h,]h/]uh.j....
-00007a90: 6833 5d72 f604 0000 6852 5805 0000 0061  h3]r....hRX....a
-00007aa0: 7272 6179 72f7 0400 0085 8172 f804 0000  rrayr......r....
-00007ab0: 7d72 f904 0000 2868 1e55 0068 1f6a f304  }r....(h.U.h.j..
-00007ac0: 0000 7562 6168 2555 0865 6d70 6861 7369  ..ubah%U.emphasi
-00007ad0: 7372 fa04 0000 7562 6852 583d 0000 0020  sr....ubhRX=... 
-00007ae0: e280 9320 4c6f 6361 7469 6f6e 206f 6620  ... Location of 
-00007af0: 7468 6520 6d6f 7374 2072 6563 656e 746c  the most recentl
-00007b00: 7920 636f 6d70 7574 6564 2028 6265 7374  y computed (best
-00007b10: 2920 6669 7420 706f 696e 742e 72fb 0400  ) fit point.r...
-00007b20: 0085 8172 fc04 0000 7d72 fd04 0000 2868  ...r....}r....(h
-00007b30: 1e58 3c00 0000 202d 2d20 4c6f 6361 7469  .X<... -- Locati
-00007b40: 6f6e 206f 6620 7468 6520 6d6f 7374 2072  on of the most r
-00007b50: 6563 656e 746c 7920 636f 6d70 7574 6564  ecently computed
-00007b60: 2028 6265 7374 2920 6669 7420 706f 696e   (best) fit poin
-00007b70: 742e 6823 4e68 314e 6832 6802 681f 6aee  t.h#Nh1Nh2h.h.j.
-00007b80: 0400 0075 6265 7562 6175 6265 7562 68cf  ...ubeubaubeubh.
-00007b90: 2981 72fe 0400 007d 72ff 0400 0028 681e  ).r....}r....(h.
-00007ba0: 5500 681f 6a51 0100 0068 236a 5901 0000  U.h.jQ...h#jY...
-00007bb0: 6825 68d2 6827 7d72 0005 0000 2868 2c5d  h%h.h'}r....(h,]
-00007bc0: 682b 5d68 295d 682a 5d68 2f5d 5507 656e  h+]h)]h*]h/]U.en
-00007bd0: 7472 6965 735d 7201 0500 0028 68d5 582a  tries]r....(h.X*
-00007be0: 0000 0063 6f76 2028 6c73 7166 6974 2e73  ...cov (lsqfit.s
-00007bf0: 6369 7079 5f6c 6561 7374 5f73 7175 6172  cipy_least_squar
-00007c00: 6573 2061 7474 7269 6275 7465 2968 1155  es attribute)h.U
-00007c10: 004e 7472 0205 0000 6175 6831 4e68 3268  .Ntr....auh1Nh2h
-00007c20: 0268 335d 7562 68d7 2981 7203 0500 007d  .h3]ubh.).r....}
-00007c30: 7204 0500 0028 681e 5500 681f 6a51 0100  r....(h.U.h.jQ..
-00007c40: 0068 236a 5901 0000 6825 68da 6827 7d72  .h#jY...h%h.h'}r
-00007c50: 0505 0000 2868 dc89 68dd 5802 0000 0070  ....(h..h.X....p
-00007c60: 7968 2c5d 682b 5d68 295d 682a 5d68 2f5d  yh,]h+]h)]h*]h/]
-00007c70: 68df 5809 0000 0061 7474 7269 6275 7465  h.X....attribute
-00007c80: 7206 0500 0068 e16a 0605 0000 7568 314e  r....h.j....uh1N
-00007c90: 6832 6802 6833 5d72 0705 0000 2868 e329  h2h.h3]r....(h.)
-00007ca0: 8172 0805 0000 7d72 0905 0000 2868 1e58  .r....}r....(h.X
-00007cb0: 0300 0000 636f 7672 0a05 0000 681f 6a03  ....covr....h.j.
-00007cc0: 0500 0068 236a 5901 0000 6825 68e7 6827  ...h#jY...h%h.h'
-00007cd0: 7d72 0b05 0000 2868 2c5d 720c 0500 0068  }r....(h,]r....h
-00007ce0: 1161 68ea 68ed 682b 5d68 295d 682a 5d68  .ah.h.h+]h)]h*]h
-00007cf0: 2f5d 720d 0500 0068 1161 68f0 5817 0000  /]r....h.ah.X...
-00007d00: 0073 6369 7079 5f6c 6561 7374 5f73 7175  .scipy_least_squ
-00007d10: 6172 6573 2e63 6f76 68f2 68f1 68f3 8975  ares.covh.h.h..u
-00007d20: 6831 4b47 6832 6802 6833 5d72 0e05 0000  h1KGh2h.h3]r....
-00007d30: 6a09 0100 0029 8172 0f05 0000 7d72 1005  j....).r....}r..
-00007d40: 0000 2868 1e6a 0a05 0000 681f 6a08 0500  ..(h.j....h.j...
-00007d50: 0068 236a 5901 0000 6825 6a0c 0100 0068  .h#jY...h%j....h
-00007d60: 277d 7211 0500 0028 68fa 68fb 682c 5d68  '}r....(h.h.h,]h
-00007d70: 2b5d 6829 5d68 2a5d 682f 5d75 6831 4b47  +]h)]h*]h/]uh1KG
-00007d80: 6832 6802 6833 5d72 1205 0000 6852 5803  h2h.h3]r....hRX.
-00007d90: 0000 0063 6f76 7213 0500 0085 8172 1405  ...covr......r..
-00007da0: 0000 7d72 1505 0000 2868 1e55 0068 234e  ..}r....(h.U.h#N
-00007db0: 6831 4e68 3268 0268 1f6a 0f05 0000 7562  h1Nh2h.h.j....ub
-00007dc0: 6175 6261 7562 6a50 0100 0029 8172 1605  aubaubjP...).r..
-00007dd0: 0000 7d72 1705 0000 2868 1e55 0068 1f6a  ..}r....(h.U.h.j
-00007de0: 0305 0000 6823 6a59 0100 0068 256a 5301  ....h#jY...h%jS.
-00007df0: 0000 6827 7d72 1805 0000 2868 295d 682a  ..h'}r....(h)]h*
-00007e00: 5d68 2b5d 682c 5d68 2f5d 7568 314b 4768  ]h+]h,]h/]uh1KGh
-00007e10: 3268 0268 335d 7219 0500 0068 9729 8172  2h.h3]r....h.).r
-00007e20: 1a05 0000 7d72 1b05 0000 2868 1e58 3200  ....}r....(h.X2.
-00007e30: 0000 2a61 7272 6179 2a20 2d2d 2043 6f76  ..*array* -- Cov
-00007e40: 6172 6961 6e63 6520 6d61 7472 6978 2061  ariance matrix a
-00007e50: 7420 7468 6520 6d69 6e69 6d75 6d20 706f  t the minimum po
-00007e60: 696e 742e 681f 6a16 0500 0068 236a 5901  int.h.j....h#jY.
-00007e70: 0000 6825 689a 6827 7d72 1c05 0000 2868  ..h%h.h'}r....(h
-00007e80: 295d 682a 5d68 2b5d 682c 5d68 2f5d 7568  )]h*]h+]h,]h/]uh
-00007e90: 314b 4668 3268 0268 335d 721d 0500 0028  1KFh2h.h3]r....(
-00007ea0: 6af2 0400 0029 8172 1e05 0000 7d72 1f05  j....).r....}r..
-00007eb0: 0000 2868 1e58 0700 0000 2a61 7272 6179  ..(h.X....*array
-00007ec0: 2a68 277d 7220 0500 0028 6829 5d68 2a5d  *h'}r ...(h)]h*]
-00007ed0: 682b 5d68 2c5d 682f 5d75 681f 6a1a 0500  h+]h,]h/]uh.j...
-00007ee0: 0068 335d 7221 0500 0068 5258 0500 0000  .h3]r!...hRX....
-00007ef0: 6172 7261 7972 2205 0000 8581 7223 0500  arrayr".....r#..
-00007f00: 007d 7224 0500 0028 681e 5500 681f 6a1e  .}r$...(h.U.h.j.
-00007f10: 0500 0075 6261 6825 6afa 0400 0075 6268  ...ubah%j....ubh
-00007f20: 5258 2c00 0000 20e2 8093 2043 6f76 6172  RX,... ... Covar
-00007f30: 6961 6e63 6520 6d61 7472 6978 2061 7420  iance matrix at 
-00007f40: 7468 6520 6d69 6e69 6d75 6d20 706f 696e  the minimum poin
-00007f50: 742e 7225 0500 0085 8172 2605 0000 7d72  t.r%.....r&...}r
-00007f60: 2705 0000 2868 1e58 2b00 0000 202d 2d20  '...(h.X+... -- 
-00007f70: 436f 7661 7269 616e 6365 206d 6174 7269  Covariance matri
-00007f80: 7820 6174 2074 6865 206d 696e 696d 756d  x at the minimum
-00007f90: 2070 6f69 6e74 2e68 234e 6831 4e68 3268   point.h#Nh1Nh2h
-00007fa0: 0268 1f6a 1a05 0000 7562 6575 6261 7562  .h.j....ubeubaub
-00007fb0: 6575 6268 cf29 8172 2805 0000 7d72 2905  eubh.).r(...}r).
-00007fc0: 0000 2868 1e55 0068 1f6a 5101 0000 6823  ..(h.U.h.jQ...h#
-00007fd0: 6a59 0100 0068 2568 d268 277d 722a 0500  jY...h%h.h'}r*..
-00007fe0: 0028 682c 5d68 2b5d 6829 5d68 2a5d 682f  .(h,]h+]h)]h*]h/
-00007ff0: 5d55 0765 6e74 7269 6573 5d72 2b05 0000  ]U.entries]r+...
-00008000: 2868 d558 3200 0000 6465 7363 7269 7074  (h.X2...descript
-00008010: 696f 6e20 286c 7371 6669 742e 7363 6970  ion (lsqfit.scip
-00008020: 795f 6c65 6173 745f 7371 7561 7265 7320  y_least_squares 
-00008030: 6174 7472 6962 7574 6529 6806 5500 4e74  attribute)h.U.Nt
-00008040: 722c 0500 0061 7568 314e 6832 6802 6833  r,...auh1Nh2h.h3
-00008050: 5d75 6268 d729 8172 2d05 0000 7d72 2e05  ]ubh.).r-...}r..
-00008060: 0000 2868 1e55 0068 1f6a 5101 0000 6823  ..(h.U.h.jQ...h#
-00008070: 6a59 0100 0068 2568 da68 277d 722f 0500  jY...h%h.h'}r/..
-00008080: 0028 68dc 8968 dd58 0200 0000 7079 682c  .(h..h.X....pyh,
-00008090: 5d68 2b5d 6829 5d68 2a5d 682f 5d68 df58  ]h+]h)]h*]h/]h.X
-000080a0: 0900 0000 6174 7472 6962 7574 6572 3005  ....attributer0.
-000080b0: 0000 68e1 6a30 0500 0075 6831 4e68 3268  ..h.j0...uh1Nh2h
-000080c0: 0268 335d 7231 0500 0028 68e3 2981 7232  .h3]r1...(h.).r2
-000080d0: 0500 007d 7233 0500 0028 681e 580b 0000  ...}r3...(h.X...
-000080e0: 0064 6573 6372 6970 7469 6f6e 7234 0500  .descriptionr4..
-000080f0: 0068 1f6a 2d05 0000 6823 6a59 0100 0068  .h.j-...h#jY...h
-00008100: 2568 e768 277d 7235 0500 0028 682c 5d72  %h.h'}r5...(h,]r
-00008110: 3605 0000 6806 6168 ea68 ed68 2b5d 6829  6...h.ah.h.h+]h)
-00008120: 5d68 2a5d 682f 5d72 3705 0000 6806 6168  ]h*]h/]r7...h.ah
-00008130: f058 1f00 0000 7363 6970 795f 6c65 6173  .X....scipy_leas
-00008140: 745f 7371 7561 7265 732e 6465 7363 7269  t_squares.descri
-00008150: 7074 696f 6e68 f268 f168 f389 7568 314b  ptionh.h.h..uh1K
-00008160: 4b68 3268 0268 335d 7238 0500 006a 0901  Kh2h.h3]r8...j..
-00008170: 0000 2981 7239 0500 007d 723a 0500 0028  ..).r9...}r:...(
-00008180: 681e 6a34 0500 0068 1f6a 3205 0000 6823  h.j4...h.j2...h#
-00008190: 6a59 0100 0068 256a 0c01 0000 6827 7d72  jY...h%j....h'}r
-000081a0: 3b05 0000 2868 fa68 fb68 2c5d 682b 5d68  ;...(h.h.h,]h+]h
-000081b0: 295d 682a 5d68 2f5d 7568 314b 4b68 3268  )]h*]h/]uh1KKh2h
-000081c0: 0268 335d 723c 0500 0068 5258 0b00 0000  .h3]r<...hRX....
-000081d0: 6465 7363 7269 7074 696f 6e72 3d05 0000  descriptionr=...
-000081e0: 8581 723e 0500 007d 723f 0500 0028 681e  ..r>...}r?...(h.
-000081f0: 5500 6823 4e68 314e 6832 6802 681f 6a39  U.h#Nh1Nh2h.h.j9
-00008200: 0500 0075 6261 7562 6175 626a 5001 0000  ...ubaubaubjP...
-00008210: 2981 7240 0500 007d 7241 0500 0028 681e  ).r@...}rA...(h.
-00008220: 5500 681f 6a2d 0500 0068 236a 5901 0000  U.h.j-...h#jY...
-00008230: 6825 6a53 0100 0068 277d 7242 0500 0028  h%jS...h'}rB...(
-00008240: 6829 5d68 2a5d 682b 5d68 2c5d 682f 5d75  h)]h*]h+]h,]h/]u
-00008250: 6831 4b4b 6832 6802 6833 5d72 4305 0000  h1KKh2h.h3]rC...
-00008260: 6897 2981 7244 0500 007d 7245 0500 0028  h.).rD...}rE...(
-00008270: 681e 5837 0000 002a 7374 722a 202d 2d20  h.X7...*str* -- 
-00008280: 5368 6f72 7420 6465 7363 7269 7074 696f  Short descriptio
-00008290: 6e20 6f66 2069 6e74 6572 6e61 6c20 6669  n of internal fi
-000082a0: 7474 6572 2073 6574 7469 6e67 732e 681f  tter settings.h.
-000082b0: 6a40 0500 0068 236a 5901 0000 6825 689a  j@...h#jY...h%h.
-000082c0: 6827 7d72 4605 0000 2868 295d 682a 5d68  h'}rF...(h)]h*]h
-000082d0: 2b5d 682c 5d68 2f5d 7568 314b 4a68 3268  +]h,]h/]uh1KJh2h
-000082e0: 0268 335d 7247 0500 0028 6af2 0400 0029  .h3]rG...(j....)
-000082f0: 8172 4805 0000 7d72 4905 0000 2868 1e58  .rH...}rI...(h.X
-00008300: 0500 0000 2a73 7472 2a68 277d 724a 0500  ....*str*h'}rJ..
-00008310: 0028 6829 5d68 2a5d 682b 5d68 2c5d 682f  .(h)]h*]h+]h,]h/
-00008320: 5d75 681f 6a44 0500 0068 335d 724b 0500  ]uh.jD...h3]rK..
-00008330: 0068 5258 0300 0000 7374 7272 4c05 0000  .hRX....strrL...
-00008340: 8581 724d 0500 007d 724e 0500 0028 681e  ..rM...}rN...(h.
-00008350: 5500 681f 6a48 0500 0075 6261 6825 6afa  U.h.jH...ubah%j.
-00008360: 0400 0075 6268 5258 3300 0000 20e2 8093  ...ubhRX3... ...
-00008370: 2053 686f 7274 2064 6573 6372 6970 7469   Short descripti
-00008380: 6f6e 206f 6620 696e 7465 726e 616c 2066  on of internal f
-00008390: 6974 7465 7220 7365 7474 696e 6773 2e72  itter settings.r
-000083a0: 4f05 0000 8581 7250 0500 007d 7251 0500  O.....rP...}rQ..
-000083b0: 0028 681e 5832 0000 0020 2d2d 2053 686f  .(h.X2... -- Sho
-000083c0: 7274 2064 6573 6372 6970 7469 6f6e 206f  rt description o
-000083d0: 6620 696e 7465 726e 616c 2066 6974 7465  f internal fitte
-000083e0: 7220 7365 7474 696e 6773 2e68 234e 6831  r settings.h#Nh1
-000083f0: 4e68 3268 0268 1f6a 4405 0000 7562 6575  Nh2h.h.jD...ubeu
-00008400: 6261 7562 6575 6268 cf29 8172 5205 0000  baubeubh.).rR...
-00008410: 7d72 5305 0000 2868 1e55 0068 1f6a 5101  }rS...(h.U.h.jQ.
-00008420: 0000 6823 6a59 0100 0068 2568 d268 277d  ..h#jY...h%h.h'}
-00008430: 7254 0500 0028 682c 5d68 2b5d 6829 5d68  rT...(h,]h+]h)]h
-00008440: 2a5d 682f 5d55 0765 6e74 7269 6573 5d72  *]h/]U.entries]r
-00008450: 5505 0000 2868 d558 2800 0000 6620 286c  U...(h.X(...f (l
-00008460: 7371 6669 742e 7363 6970 795f 6c65 6173  sqfit.scipy_leas
-00008470: 745f 7371 7561 7265 7320 6174 7472 6962  t_squares attrib
-00008480: 7574 6529 6808 5500 4e74 7256 0500 0061  ute)h.U.NtrV...a
-00008490: 7568 314e 6832 6802 6833 5d75 6268 d729  uh1Nh2h.h3]ubh.)
-000084a0: 8172 5705 0000 7d72 5805 0000 2868 1e55  .rW...}rX...(h.U
-000084b0: 0068 1f6a 5101 0000 6823 6a59 0100 0068  .h.jQ...h#jY...h
-000084c0: 2568 da68 277d 7259 0500 0028 68dc 8968  %h.h'}rY...(h..h
-000084d0: dd58 0200 0000 7079 682c 5d68 2b5d 6829  .X....pyh,]h+]h)
-000084e0: 5d68 2a5d 682f 5d68 df58 0900 0000 6174  ]h*]h/]h.X....at
-000084f0: 7472 6962 7574 6572 5a05 0000 68e1 6a5a  tributerZ...h.jZ
-00008500: 0500 0075 6831 4e68 3268 0268 335d 725b  ...uh1Nh2h.h3]r[
-00008510: 0500 0028 68e3 2981 725c 0500 007d 725d  ...(h.).r\...}r]
-00008520: 0500 0028 681e 5801 0000 0066 681f 6a57  ...(h.X....fh.jW
-00008530: 0500 0068 236a 5901 0000 6825 68e7 6827  ...h#jY...h%h.h'
-00008540: 7d72 5e05 0000 2868 2c5d 725f 0500 0068  }r^...(h,]r_...h
-00008550: 0861 68ea 68ed 682b 5d68 295d 682a 5d68  .ah.h.h+]h)]h*]h
-00008560: 2f5d 7260 0500 0068 0861 68f0 5815 0000  /]r`...h.ah.X...
-00008570: 0073 6369 7079 5f6c 6561 7374 5f73 7175  .scipy_least_squ
-00008580: 6172 6573 2e66 68f2 68f1 68f3 8975 6831  ares.fh.h.h..uh1
-00008590: 4b50 6832 6802 6833 5d72 6105 0000 6a09  KPh2h.h3]ra...j.
-000085a0: 0100 0029 8172 6205 0000 7d72 6305 0000  ...).rb...}rc...
-000085b0: 2868 1e58 0100 0000 6668 1f6a 5c05 0000  (h.X....fh.j\...
-000085c0: 6823 6a59 0100 0068 256a 0c01 0000 6827  h#jY...h%j....h'
-000085d0: 7d72 6405 0000 2868 fa68 fb68 2c5d 682b  }rd...(h.h.h,]h+
-000085e0: 5d68 295d 682a 5d68 2f5d 7568 314b 5068  ]h)]h*]h/]uh1KPh
-000085f0: 3268 0268 335d 7265 0500 0068 5258 0100  2h.h3]re...hRX..
-00008600: 0000 6685 8172 6605 0000 7d72 6705 0000  ..f..rf...}rg...
-00008610: 2868 1e55 0068 234e 6831 4e68 3268 0268  (h.U.h#Nh1Nh2h.h
-00008620: 1f6a 6205 0000 7562 6175 6261 7562 6a50  .jb...ubaubaubjP
-00008630: 0100 0029 8172 6805 0000 7d72 6905 0000  ...).rh...}ri...
-00008640: 2868 1e55 0068 1f6a 5705 0000 6823 6a59  (h.U.h.jW...h#jY
-00008650: 0100 0068 256a 5301 0000 6827 7d72 6a05  ...h%jS...h'}rj.
-00008660: 0000 2868 295d 682a 5d68 2b5d 682c 5d68  ..(h)]h*]h+]h,]h
-00008670: 2f5d 7568 314b 5068 3268 0268 335d 726b  /]uh1KPh2h.h3]rk
-00008680: 0500 0068 9729 8172 6c05 0000 7d72 6d05  ...h.).rl...}rm.
-00008690: 0000 2868 1e58 4d00 0000 2a61 7272 6179  ..(h.XM...*array
-000086a0: 2a20 2d2d 2046 6974 2066 756e 6374 696f  * -- Fit functio
-000086b0: 6e20 7661 6c75 6520 6060 6628 7829 6060  n value ``f(x)``
-000086c0: 2061 7420 7468 6520 6d69 6e69 6d75 6d20   at the minimum 
-000086d0: 696e 0a74 6865 206d 6f73 7420 7265 6365  in.the most rece
-000086e0: 6e74 2066 6974 2e68 1f6a 6805 0000 6823  nt fit.h.jh...h#
-000086f0: 6a59 0100 0068 2568 9a68 277d 726e 0500  jY...h%h.h'}rn..
-00008700: 0028 6829 5d68 2a5d 682b 5d68 2c5d 682f  .(h)]h*]h+]h,]h/
-00008710: 5d75 6831 4b4e 6832 6802 6833 5d72 6f05  ]uh1KNh2h.h3]ro.
-00008720: 0000 286a f204 0000 2981 7270 0500 007d  ..(j....).rp...}
-00008730: 7271 0500 0028 681e 5807 0000 002a 6172  rq...(h.X....*ar
-00008740: 7261 792a 6827 7d72 7205 0000 2868 295d  ray*h'}rr...(h)]
-00008750: 682a 5d68 2b5d 682c 5d68 2f5d 7568 1f6a  h*]h+]h,]h/]uh.j
-00008760: 6c05 0000 6833 5d72 7305 0000 6852 5805  l...h3]rs...hRX.
-00008770: 0000 0061 7272 6179 7274 0500 0085 8172  ...arrayrt.....r
-00008780: 7505 0000 7d72 7605 0000 2868 1e55 0068  u...}rv...(h.U.h
-00008790: 1f6a 7005 0000 7562 6168 256a fa04 0000  .jp...ubah%j....
-000087a0: 7562 6852 5818 0000 0020 e280 9320 4669  ubhRX.... ... Fi
-000087b0: 7420 6675 6e63 7469 6f6e 2076 616c 7565  t function value
-000087c0: 2072 7705 0000 8581 7278 0500 007d 7279   rw.....rx...}ry
-000087d0: 0500 0028 681e 5817 0000 0020 2d2d 2046  ...(h.X.... -- F
-000087e0: 6974 2066 756e 6374 696f 6e20 7661 6c75  it function valu
-000087f0: 6520 6823 4e68 314e 6832 6802 681f 6a6c  e h#Nh1Nh2h.h.jl
-00008800: 0500 0075 6268 4a29 8172 7a05 0000 7d72  ...ubhJ).rz...}r
-00008810: 7b05 0000 2868 1e58 0800 0000 6060 6628  {...(h.X....``f(
-00008820: 7829 6060 6827 7d72 7c05 0000 2868 295d  x)``h'}r|...(h)]
-00008830: 682a 5d68 2b5d 682c 5d68 2f5d 7568 1f6a  h*]h+]h,]h/]uh.j
-00008840: 6c05 0000 6833 5d72 7d05 0000 6852 5804  l...h3]r}...hRX.
-00008850: 0000 0066 2878 2972 7e05 0000 8581 727f  ...f(x)r~.....r.
-00008860: 0500 007d 7280 0500 0028 681e 5500 681f  ...}r....(h.U.h.
-00008870: 6a7a 0500 0075 6261 6825 6856 7562 6852  jz...ubah%hVubhR
-00008880: 5827 0000 0020 6174 2074 6865 206d 696e  X'... at the min
-00008890: 696d 756d 2069 6e0a 7468 6520 6d6f 7374  imum in.the most
-000088a0: 2072 6563 656e 7420 6669 742e 7281 0500   recent fit.r...
-000088b0: 0085 8172 8205 0000 7d72 8305 0000 2868  ...r....}r....(h
-000088c0: 1e58 2700 0000 2061 7420 7468 6520 6d69  .X'... at the mi
-000088d0: 6e69 6d75 6d20 696e 0a74 6865 206d 6f73  nimum in.the mos
-000088e0: 7420 7265 6365 6e74 2066 6974 2e68 234e  t recent fit.h#N
-000088f0: 6831 4e68 3268 0268 1f6a 6c05 0000 7562  h1Nh2h.h.jl...ub
-00008900: 6575 6261 7562 6575 6268 cf29 8172 8405  eubaubeubh.).r..
-00008910: 0000 7d72 8505 0000 2868 1e55 0068 1f6a  ..}r....(h.U.h.j
-00008920: 5101 0000 6823 6a59 0100 0068 2568 d268  Q...h#jY...h%h.h
-00008930: 277d 7286 0500 0028 682c 5d68 2b5d 6829  '}r....(h,]h+]h)
-00008940: 5d68 2a5d 682f 5d55 0765 6e74 7269 6573  ]h*]h/]U.entries
-00008950: 5d72 8705 0000 2868 d558 2800 0000 4a20  ]r....(h.X(...J 
-00008960: 286c 7371 6669 742e 7363 6970 795f 6c65  (lsqfit.scipy_le
-00008970: 6173 745f 7371 7561 7265 7320 6174 7472  ast_squares attr
-00008980: 6962 7574 6529 680f 5500 4e74 7288 0500  ibute)h.U.Ntr...
-00008990: 0061 7568 314e 6832 6802 6833 5d75 6268  .auh1Nh2h.h3]ubh
-000089a0: d729 8172 8905 0000 7d72 8a05 0000 2868  .).r....}r....(h
-000089b0: 1e55 0068 1f6a 5101 0000 6823 6a59 0100  .U.h.jQ...h#jY..
-000089c0: 0068 2568 da68 277d 728b 0500 0028 68dc  .h%h.h'}r....(h.
-000089d0: 8968 dd58 0200 0000 7079 682c 5d68 2b5d  .h.X....pyh,]h+]
-000089e0: 6829 5d68 2a5d 682f 5d68 df58 0900 0000  h)]h*]h/]h.X....
-000089f0: 6174 7472 6962 7574 6572 8c05 0000 68e1  attributer....h.
-00008a00: 6a8c 0500 0075 6831 4e68 3268 0268 335d  j....uh1Nh2h.h3]
-00008a10: 728d 0500 0028 68e3 2981 728e 0500 007d  r....(h.).r....}
-00008a20: 728f 0500 0028 681e 5801 0000 004a 681f  r....(h.X....Jh.
-00008a30: 6a89 0500 0068 236a 5901 0000 6825 68e7  j....h#jY...h%h.
-00008a40: 6827 7d72 9005 0000 2868 2c5d 7291 0500  h'}r....(h,]r...
-00008a50: 0068 0f61 68ea 68ed 682b 5d68 295d 682a  .h.ah.h.h+]h)]h*
-00008a60: 5d68 2f5d 7292 0500 0068 0f61 68f0 5815  ]h/]r....h.ah.X.
-00008a70: 0000 0073 6369 7079 5f6c 6561 7374 5f73  ...scipy_least_s
-00008a80: 7175 6172 6573 2e4a 68f2 68f1 68f3 8975  quares.Jh.h.h..u
-00008a90: 6831 4b54 6832 6802 6833 5d72 9305 0000  h1KTh2h.h3]r....
-00008aa0: 6a09 0100 0029 8172 9405 0000 7d72 9505  j....).r....}r..
-00008ab0: 0000 2868 1e58 0100 0000 4a68 1f6a 8e05  ..(h.X....Jh.j..
-00008ac0: 0000 6823 6a59 0100 0068 256a 0c01 0000  ..h#jY...h%j....
-00008ad0: 6827 7d72 9605 0000 2868 fa68 fb68 2c5d  h'}r....(h.h.h,]
-00008ae0: 682b 5d68 295d 682a 5d68 2f5d 7568 314b  h+]h)]h*]h/]uh1K
-00008af0: 5468 3268 0268 335d 7297 0500 0068 5258  Th2h.h3]r....hRX
-00008b00: 0100 0000 4a85 8172 9805 0000 7d72 9905  ....J..r....}r..
-00008b10: 0000 2868 1e55 0068 234e 6831 4e68 3268  ..(h.U.h#Nh1Nh2h
-00008b20: 0268 1f6a 9405 0000 7562 6175 6261 7562  .h.j....ubaubaub
-00008b30: 6a50 0100 0029 8172 9a05 0000 7d72 9b05  jP...).r....}r..
-00008b40: 0000 2868 1e55 0068 1f6a 8905 0000 6823  ..(h.U.h.j....h#
-00008b50: 6a59 0100 0068 256a 5301 0000 6827 7d72  jY...h%jS...h'}r
-00008b60: 9c05 0000 2868 295d 682a 5d68 2b5d 682c  ....(h)]h*]h+]h,
-00008b70: 5d68 2f5d 7568 314b 5468 3268 0268 335d  ]h/]uh1KTh2h.h3]
-00008b80: 729d 0500 0068 9729 8172 9e05 0000 7d72  r....h.).r....}r
-00008b90: 9f05 0000 2868 1e58 3e00 0000 2a61 7272  ....(h.X>...*arr
-00008ba0: 6179 2a20 2d2d 2047 7261 6469 656e 7420  ay* -- Gradient 
-00008bb0: 6060 4a5f 696a 203d 2064 665f 692f 6478  ``J_ij = df_i/dx
-00008bc0: 5b6a 5d60 6020 666f 7220 6d6f 7374 2072  [j]`` for most r
-00008bd0: 6563 656e 7420 6669 742e 681f 6a9a 0500  ecent fit.h.j...
-00008be0: 0068 236a 5901 0000 6825 689a 6827 7d72  .h#jY...h%h.h'}r
-00008bf0: a005 0000 2868 295d 682a 5d68 2b5d 682c  ....(h)]h*]h+]h,
-00008c00: 5d68 2f5d 7568 314b 5368 3268 0268 335d  ]h/]uh1KSh2h.h3]
-00008c10: 72a1 0500 0028 6af2 0400 0029 8172 a205  r....(j....).r..
-00008c20: 0000 7d72 a305 0000 2868 1e58 0700 0000  ..}r....(h.X....
-00008c30: 2a61 7272 6179 2a68 277d 72a4 0500 0028  *array*h'}r....(
-00008c40: 6829 5d68 2a5d 682b 5d68 2c5d 682f 5d75  h)]h*]h+]h,]h/]u
-00008c50: 681f 6a9e 0500 0068 335d 72a5 0500 0068  h.j....h3]r....h
-00008c60: 5258 0500 0000 6172 7261 7972 a605 0000  RX....arrayr....
-00008c70: 8581 72a7 0500 007d 72a8 0500 0028 681e  ..r....}r....(h.
-00008c80: 5500 681f 6aa2 0500 0075 6261 6825 6afa  U.h.j....ubah%j.
-00008c90: 0400 0075 6268 5258 0e00 0000 20e2 8093  ...ubhRX.... ...
-00008ca0: 2047 7261 6469 656e 7420 72a9 0500 0085   Gradient r.....
-00008cb0: 8172 aa05 0000 7d72 ab05 0000 2868 1e58  .r....}r....(h.X
-00008cc0: 0d00 0000 202d 2d20 4772 6164 6965 6e74  .... -- Gradient
-00008cd0: 2068 234e 6831 4e68 3268 0268 1f6a 9e05   h#Nh1Nh2h.h.j..
-00008ce0: 0000 7562 684a 2981 72ac 0500 007d 72ad  ..ubhJ).r....}r.
-00008cf0: 0500 0028 681e 5815 0000 0060 604a 5f69  ...(h.X....``J_i
-00008d00: 6a20 3d20 6466 5f69 2f64 785b 6a5d 6060  j = df_i/dx[j]``
-00008d10: 6827 7d72 ae05 0000 2868 295d 682a 5d68  h'}r....(h)]h*]h
-00008d20: 2b5d 682c 5d68 2f5d 7568 1f6a 9e05 0000  +]h,]h/]uh.j....
-00008d30: 6833 5d72 af05 0000 6852 5811 0000 004a  h3]r....hRX....J
-00008d40: 5f69 6a20 3d20 6466 5f69 2f64 785b 6a5d  _ij = df_i/dx[j]
-00008d50: 72b0 0500 0085 8172 b105 0000 7d72 b205  r......r....}r..
-00008d60: 0000 2868 1e55 0068 1f6a ac05 0000 7562  ..(h.U.h.j....ub
-00008d70: 6168 2568 5675 6268 5258 1500 0000 2066  ah%hVubhRX.... f
-00008d80: 6f72 206d 6f73 7420 7265 6365 6e74 2066  or most recent f
-00008d90: 6974 2e72 b305 0000 8581 72b4 0500 007d  it.r......r....}
-00008da0: 72b5 0500 0028 681e 5815 0000 0020 666f  r....(h.X.... fo
-00008db0: 7220 6d6f 7374 2072 6563 656e 7420 6669  r most recent fi
-00008dc0: 742e 6823 4e68 314e 6832 6802 681f 6a9e  t.h#Nh1Nh2h.h.j.
-00008dd0: 0500 0075 6265 7562 6175 6265 7562 68cf  ...ubeubaubeubh.
-00008de0: 2981 72b6 0500 007d 72b7 0500 0028 681e  ).r....}r....(h.
-00008df0: 5500 681f 6a51 0100 0068 236a 5901 0000  U.h.jQ...h#jY...
-00008e00: 6825 68d2 6827 7d72 b805 0000 2868 2c5d  h%h.h'}r....(h,]
-00008e10: 682b 5d68 295d 682a 5d68 2f5d 5507 656e  h+]h)]h*]h/]U.en
-00008e20: 7472 6965 735d 72b9 0500 0028 68d5 582a  tries]r....(h.X*
-00008e30: 0000 006e 6974 2028 6c73 7166 6974 2e73  ...nit (lsqfit.s
-00008e40: 6369 7079 5f6c 6561 7374 5f73 7175 6172  cipy_least_squar
-00008e50: 6573 2061 7474 7269 6275 7465 2968 0d55  es attribute)h.U
-00008e60: 004e 7472 ba05 0000 6175 6831 4e68 3268  .Ntr....auh1Nh2h
-00008e70: 0268 335d 7562 68d7 2981 72bb 0500 007d  .h3]ubh.).r....}
-00008e80: 72bc 0500 0028 681e 5500 681f 6a51 0100  r....(h.U.h.jQ..
-00008e90: 0068 236a 5901 0000 6825 68da 6827 7d72  .h#jY...h%h.h'}r
-00008ea0: bd05 0000 2868 dc89 68dd 5802 0000 0070  ....(h..h.X....p
-00008eb0: 7968 2c5d 682b 5d68 295d 682a 5d68 2f5d  yh,]h+]h)]h*]h/]
-00008ec0: 68df 5809 0000 0061 7474 7269 6275 7465  h.X....attribute
-00008ed0: 72be 0500 0068 e16a be05 0000 7568 314e  r....h.j....uh1N
-00008ee0: 6832 6802 6833 5d72 bf05 0000 2868 e329  h2h.h3]r....(h.)
-00008ef0: 8172 c005 0000 7d72 c105 0000 2868 1e58  .r....}r....(h.X
-00008f00: 0300 0000 6e69 7472 c205 0000 681f 6abb  ....nitr....h.j.
-00008f10: 0500 0068 236a 5901 0000 6825 68e7 6827  ...h#jY...h%h.h'
-00008f20: 7d72 c305 0000 2868 2c5d 72c4 0500 0068  }r....(h,]r....h
-00008f30: 0d61 68ea 68ed 682b 5d68 295d 682a 5d68  .ah.h.h+]h)]h*]h
-00008f40: 2f5d 72c5 0500 0068 0d61 68f0 5817 0000  /]r....h.ah.X...
-00008f50: 0073 6369 7079 5f6c 6561 7374 5f73 7175  .scipy_least_squ
-00008f60: 6172 6573 2e6e 6974 68f2 68f1 68f3 8975  ares.nith.h.h..u
-00008f70: 6831 4b59 6832 6802 6833 5d72 c605 0000  h1KYh2h.h3]r....
-00008f80: 6a09 0100 0029 8172 c705 0000 7d72 c805  j....).r....}r..
-00008f90: 0000 2868 1e6a c205 0000 681f 6ac0 0500  ..(h.j....h.j...
-00008fa0: 0068 236a 5901 0000 6825 6a0c 0100 0068  .h#jY...h%j....h
-00008fb0: 277d 72c9 0500 0028 68fa 68fb 682c 5d68  '}r....(h.h.h,]h
-00008fc0: 2b5d 6829 5d68 2a5d 682f 5d75 6831 4b59  +]h)]h*]h/]uh1KY
-00008fd0: 6832 6802 6833 5d72 ca05 0000 6852 5803  h2h.h3]r....hRX.
-00008fe0: 0000 006e 6974 72cb 0500 0085 8172 cc05  ...nitr......r..
-00008ff0: 0000 7d72 cd05 0000 2868 1e55 0068 234e  ..}r....(h.U.h#N
-00009000: 6831 4e68 3268 0268 1f6a c705 0000 7562  h1Nh2h.h.j....ub
-00009010: 6175 6261 7562 6a50 0100 0029 8172 ce05  aubaubjP...).r..
-00009020: 0000 7d72 cf05 0000 2868 1e55 0068 1f6a  ..}r....(h.U.h.j
-00009030: bb05 0000 6823 6a59 0100 0068 256a 5301  ....h#jY...h%jS.
-00009040: 0000 6827 7d72 d005 0000 2868 295d 682a  ..h'}r....(h)]h*
-00009050: 5d68 2b5d 682c 5d68 2f5d 7568 314b 5968  ]h+]h,]h/]uh1KYh
-00009060: 3268 0268 335d 72d1 0500 0068 9729 8172  2h.h3]r....h.).r
-00009070: d205 0000 7d72 d305 0000 2868 1e58 4d00  ....}r....(h.XM.
-00009080: 0000 2a69 6e74 2a20 2d2d 204e 756d 6265  ..*int* -- Numbe
-00009090: 7220 6f66 2066 756e 6374 696f 6e20 6576  r of function ev
-000090a0: 616c 7561 7469 6f6e 7320 7573 6564 2069  aluations used i
-000090b0: 6e20 6c61 7374 2066 6974 2074 6f20 6669  n last fit to fi
-000090c0: 6e64 0a74 6865 206d 696e 696d 756d 2e68  nd.the minimum.h
-000090d0: 1f6a ce05 0000 6823 6a59 0100 0068 2568  .j....h#jY...h%h
-000090e0: 9a68 277d 72d4 0500 0028 6829 5d68 2a5d  .h'}r....(h)]h*]
-000090f0: 682b 5d68 2c5d 682f 5d75 6831 4b57 6832  h+]h,]h/]uh1KWh2
-00009100: 6802 6833 5d72 d505 0000 286a f204 0000  h.h3]r....(j....
-00009110: 2981 72d6 0500 007d 72d7 0500 0028 681e  ).r....}r....(h.
-00009120: 5805 0000 002a 696e 742a 6827 7d72 d805  X....*int*h'}r..
-00009130: 0000 2868 295d 682a 5d68 2b5d 682c 5d68  ..(h)]h*]h+]h,]h
-00009140: 2f5d 7568 1f6a d205 0000 6833 5d72 d905  /]uh.j....h3]r..
-00009150: 0000 6852 5803 0000 0069 6e74 72da 0500  ..hRX....intr...
-00009160: 0085 8172 db05 0000 7d72 dc05 0000 2868  ...r....}r....(h
-00009170: 1e55 0068 1f6a d605 0000 7562 6168 256a  .U.h.j....ubah%j
-00009180: fa04 0000 7562 6852 5849 0000 0020 e280  ....ubhRXI... ..
-00009190: 9320 4e75 6d62 6572 206f 6620 6675 6e63  . Number of func
-000091a0: 7469 6f6e 2065 7661 6c75 6174 696f 6e73  tion evaluations
-000091b0: 2075 7365 6420 696e 206c 6173 7420 6669   used in last fi
-000091c0: 7420 746f 2066 696e 640a 7468 6520 6d69  t to find.the mi
-000091d0: 6e69 6d75 6d2e 72dd 0500 0085 8172 de05  nimum.r......r..
-000091e0: 0000 7d72 df05 0000 2868 1e58 4800 0000  ..}r....(h.XH...
-000091f0: 202d 2d20 4e75 6d62 6572 206f 6620 6675   -- Number of fu
-00009200: 6e63 7469 6f6e 2065 7661 6c75 6174 696f  nction evaluatio
-00009210: 6e73 2075 7365 6420 696e 206c 6173 7420  ns used in last 
-00009220: 6669 7420 746f 2066 696e 640a 7468 6520  fit to find.the 
-00009230: 6d69 6e69 6d75 6d2e 6823 4e68 314e 6832  minimum.h#Nh1Nh2
-00009240: 6802 681f 6ad2 0500 0075 6265 7562 6175  h.h.j....ubeubau
-00009250: 6265 7562 68cf 2981 72e0 0500 007d 72e1  beubh.).r....}r.
-00009260: 0500 0028 681e 5500 681f 6a51 0100 0068  ...(h.U.h.jQ...h
-00009270: 236a 5901 0000 6825 68d2 6827 7d72 e205  #jY...h%h.h'}r..
-00009280: 0000 2868 2c5d 682b 5d68 295d 682a 5d68  ..(h,]h+]h)]h*]h
-00009290: 2f5d 5507 656e 7472 6965 735d 72e3 0500  /]U.entries]r...
-000092a0: 0028 68d5 5839 0000 0073 746f 7070 696e  .(h.X9...stoppin
-000092b0: 675f 6372 6974 6572 696f 6e20 286c 7371  g_criterion (lsq
-000092c0: 6669 742e 7363 6970 795f 6c65 6173 745f  fit.scipy_least_
-000092d0: 7371 7561 7265 7320 6174 7472 6962 7574  squares attribut
-000092e0: 6529 680e 5500 4e74 72e4 0500 0061 7568  e)h.U.Ntr....auh
-000092f0: 314e 6832 6802 6833 5d75 6268 d729 8172  1Nh2h.h3]ubh.).r
-00009300: e505 0000 7d72 e605 0000 2868 1e55 0068  ....}r....(h.U.h
-00009310: 1f6a 5101 0000 6823 6a59 0100 0068 2568  .jQ...h#jY...h%h
-00009320: da68 277d 72e7 0500 0028 68dc 8968 dd58  .h'}r....(h..h.X
-00009330: 0200 0000 7079 682c 5d68 2b5d 6829 5d68  ....pyh,]h+]h)]h
-00009340: 2a5d 682f 5d68 df58 0900 0000 6174 7472  *]h/]h.X....attr
-00009350: 6962 7574 6572 e805 0000 68e1 6ae8 0500  ibuter....h.j...
-00009360: 0075 6831 4e68 3268 0268 335d 72e9 0500  .uh1Nh2h.h3]r...
-00009370: 0028 68e3 2981 72ea 0500 007d 72eb 0500  .(h.).r....}r...
-00009380: 0028 681e 5812 0000 0073 746f 7070 696e  .(h.X....stoppin
-00009390: 675f 6372 6974 6572 696f 6e72 ec05 0000  g_criterionr....
-000093a0: 681f 6ae5 0500 0068 236a 5901 0000 6825  h.j....h#jY...h%
-000093b0: 68e7 6827 7d72 ed05 0000 2868 2c5d 72ee  h.h'}r....(h,]r.
-000093c0: 0500 0068 0e61 68ea 68ed 682b 5d68 295d  ...h.ah.h.h+]h)]
-000093d0: 682a 5d68 2f5d 72ef 0500 0068 0e61 68f0  h*]h/]r....h.ah.
-000093e0: 5826 0000 0073 6369 7079 5f6c 6561 7374  X&...scipy_least
-000093f0: 5f73 7175 6172 6573 2e73 746f 7070 696e  _squares.stoppin
-00009400: 675f 6372 6974 6572 696f 6e68 f268 f168  g_criterionh.h.h
-00009410: f389 7568 314b 6668 3268 0268 335d 72f0  ..uh1Kfh2h.h3]r.
-00009420: 0500 006a 0901 0000 2981 72f1 0500 007d  ...j....).r....}
-00009430: 72f2 0500 0028 681e 6aec 0500 0068 1f6a  r....(h.j....h.j
-00009440: ea05 0000 6823 6a59 0100 0068 256a 0c01  ....h#jY...h%j..
-00009450: 0000 6827 7d72 f305 0000 2868 fa68 fb68  ..h'}r....(h.h.h
-00009460: 2c5d 682b 5d68 295d 682a 5d68 2f5d 7568  ,]h+]h)]h*]h/]uh
-00009470: 314b 6668 3268 0268 335d 72f4 0500 0068  1Kfh2h.h3]r....h
-00009480: 5258 1200 0000 7374 6f70 7069 6e67 5f63  RX....stopping_c
-00009490: 7269 7465 7269 6f6e 72f5 0500 0085 8172  riterionr......r
-000094a0: f605 0000 7d72 f705 0000 2868 1e55 0068  ....}r....(h.U.h
-000094b0: 234e 6831 4e68 3268 0268 1f6a f105 0000  #Nh1Nh2h.h.j....
-000094c0: 7562 6175 6261 7562 6a50 0100 0029 8172  ubaubaubjP...).r
-000094d0: f805 0000 7d72 f905 0000 2868 1e55 0068  ....}r....(h.U.h
-000094e0: 1f6a e505 0000 6823 6a59 0100 0068 256a  .j....h#jY...h%j
-000094f0: 5301 0000 6827 7d72 fa05 0000 2868 295d  S...h'}r....(h)]
-00009500: 682a 5d68 2b5d 682c 5d68 2f5d 7568 314b  h*]h+]h,]h/]uh1K
-00009510: 6668 3268 0268 335d 72fb 0500 0028 6897  fh2h.h3]r....(h.
-00009520: 2981 72fc 0500 007d 72fd 0500 0028 681e  ).r....}r....(h.
-00009530: 5824 0000 002a 696e 742a 202d 2d20 4372  X$...*int* -- Cr
-00009540: 6974 6572 696f 6e20 7573 6564 2074 6f0a  iterion used to.
-00009550: 7374 6f70 2066 6974 3a68 1f6a f805 0000  stop fit:h.j....
-00009560: 6823 6a59 0100 0068 2568 9a68 277d 72fe  h#jY...h%h.h'}r.
-00009570: 0500 0028 6829 5d68 2a5d 682b 5d68 2c5d  ...(h)]h*]h+]h,]
-00009580: 682f 5d75 6831 4b5c 6832 6802 6833 5d72  h/]uh1K\h2h.h3]r
-00009590: ff05 0000 286a f204 0000 2981 7200 0600  ....(j....).r...
-000095a0: 007d 7201 0600 0028 681e 5805 0000 002a  .}r....(h.X....*
-000095b0: 696e 742a 6827 7d72 0206 0000 2868 295d  int*h'}r....(h)]
-000095c0: 682a 5d68 2b5d 682c 5d68 2f5d 7568 1f6a  h*]h+]h,]h/]uh.j
-000095d0: fc05 0000 6833 5d72 0306 0000 6852 5803  ....h3]r....hRX.
-000095e0: 0000 0069 6e74 7204 0600 0085 8172 0506  ...intr......r..
-000095f0: 0000 7d72 0606 0000 2868 1e55 0068 1f6a  ..}r....(h.U.h.j
-00009600: 0006 0000 7562 6168 256a fa04 0000 7562  ....ubah%j....ub
-00009610: 6852 5820 0000 0020 e280 9320 4372 6974  hRX ... ... Crit
-00009620: 6572 696f 6e20 7573 6564 2074 6f0a 7374  erion used to.st
-00009630: 6f70 2066 6974 3a72 0706 0000 8581 7208  op fit:r......r.
-00009640: 0600 007d 7209 0600 0028 681e 581f 0000  ...}r....(h.X...
-00009650: 0020 2d2d 2043 7269 7465 7269 6f6e 2075  . -- Criterion u
-00009660: 7365 6420 746f 0a73 746f 7020 6669 743a  sed to.stop fit:
-00009670: 6823 4e68 314e 6832 6802 681f 6afc 0500  h#Nh1Nh2h.h.j...
-00009680: 0075 6265 7562 6ad5 0200 0029 8172 0a06  .ubeubj....).r..
-00009690: 0000 7d72 0b06 0000 2868 1e55 0068 1f6a  ..}r....(h.U.h.j
-000096a0: f805 0000 6823 4e68 256a d802 0000 6827  ....h#Nh%j....h'
-000096b0: 7d72 0c06 0000 2868 295d 682a 5d68 2b5d  }r....(h)]h*]h+]
-000096c0: 682c 5d68 2f5d 7568 314e 6832 6802 6833  h,]h/]uh1Nh2h.h3
-000096d0: 5d72 0d06 0000 6364 6f63 7574 696c 732e  ]r....cdocutils.
-000096e0: 6e6f 6465 730a 656e 756d 6572 6174 6564  nodes.enumerated
-000096f0: 5f6c 6973 740a 720e 0600 0029 8172 0f06  _list.r....).r..
-00009700: 0000 7d72 1006 0000 2868 1e55 0068 277d  ..}r....(h.U.h'}
-00009710: 7211 0600 0028 5506 7375 6666 6978 7212  r....(U.suffixr.
-00009720: 0600 0055 012e 5505 7374 6172 7472 1306  ...U..U.startr..
-00009730: 0000 4b00 682c 5d68 2b5d 6829 5d55 0670  ..K.h,]h+]h)]U.p
-00009740: 7265 6669 7872 1406 0000 5500 682a 5d68  refixr....U.h*]h
-00009750: 2f5d 5508 656e 756d 7479 7065 7215 0600  /]U.enumtyper...
-00009760: 0055 0661 7261 6269 6372 1606 0000 7568  .U.arabicr....uh
-00009770: 1f6a 0a06 0000 6833 5d72 1706 0000 286a  .j....h3]r....(j
-00009780: d401 0000 2981 7218 0600 007d 7219 0600  ....).r....}r...
-00009790: 0028 681e 5810 0000 0064 6964 6e27 7420  .(h.X....didn't 
-000097a0: 636f 6e76 6572 6765 0a68 277d 721a 0600  converge.h'}r...
-000097b0: 0028 6829 5d68 2a5d 682b 5d68 2c5d 682f  .(h)]h*]h+]h,]h/
-000097c0: 5d75 681f 6a0f 0600 0068 335d 721b 0600  ]uh.j....h3]r...
-000097d0: 0068 9729 8172 1c06 0000 7d72 1d06 0000  .h.).r....}r....
-000097e0: 2868 1e58 0f00 0000 6469 646e 2774 2063  (h.X....didn't c
-000097f0: 6f6e 7665 7267 6572 1e06 0000 681f 6a18  onverger....h.j.
-00009800: 0600 0068 236a 5901 0000 6825 689a 6827  ...h#jY...h%h.h'
-00009810: 7d72 1f06 0000 2868 295d 682a 5d68 2b5d  }r....(h)]h*]h+]
-00009820: 682c 5d68 2f5d 7568 314b 5f68 335d 7220  h,]h/]uh1K_h3]r 
-00009830: 0600 0068 5258 1100 0000 6469 646e e280  ...hRX....didn..
-00009840: 9974 2063 6f6e 7665 7267 6572 2106 0000  .t converger!...
-00009850: 8581 7222 0600 007d 7223 0600 0028 681e  ..r"...}r#...(h.
-00009860: 6a1e 0600 0068 1f6a 1c06 0000 7562 6175  j....h.j....ubau
-00009870: 6261 6825 6a01 0200 0075 626a d401 0000  bah%j....ubj....
-00009880: 2981 7224 0600 007d 7225 0600 0028 681e  ).r$...}r%...(h.
-00009890: 583d 0000 0060 6078 746f 6c20 3e3d 6060  X=...``xtol >=``
-000098a0: 2072 656c 6174 6976 6520 6368 616e 6765   relative change
-000098b0: 2069 6e20 7061 7261 6d65 7465 7273 2062   in parameters b
-000098c0: 6574 7765 656e 2069 7465 7261 7469 6f6e  etween iteration
-000098d0: 730a 6827 7d72 2606 0000 2868 295d 682a  s.h'}r&...(h)]h*
-000098e0: 5d68 2b5d 682c 5d68 2f5d 7568 1f6a 0f06  ]h+]h,]h/]uh.j..
-000098f0: 0000 6833 5d72 2706 0000 6897 2981 7228  ..h3]r'...h.).r(
-00009900: 0600 007d 7229 0600 0028 681e 583c 0000  ...}r)...(h.X<..
-00009910: 0060 6078 746f 6c20 3e3d 6060 2072 656c  .``xtol >=`` rel
-00009920: 6174 6976 6520 6368 616e 6765 2069 6e20  ative change in 
-00009930: 7061 7261 6d65 7465 7273 2062 6574 7765  parameters betwe
-00009940: 656e 2069 7465 7261 7469 6f6e 7368 1f6a  en iterationsh.j
-00009950: 2406 0000 6823 6a59 0100 0068 2568 9a68  $...h#jY...h%h.h
-00009960: 277d 722a 0600 0028 6829 5d68 2a5d 682b  '}r*...(h)]h*]h+
-00009970: 5d68 2c5d 682f 5d75 6831 4b61 6833 5d72  ]h,]h/]uh1Kah3]r
-00009980: 2b06 0000 2868 4a29 8172 2c06 0000 7d72  +...(hJ).r,...}r
-00009990: 2d06 0000 2868 1e58 0b00 0000 6060 7874  -...(h.X....``xt
-000099a0: 6f6c 203e 3d60 6068 277d 722e 0600 0028  ol >=``h'}r....(
-000099b0: 6829 5d68 2a5d 682b 5d68 2c5d 682f 5d75  h)]h*]h+]h,]h/]u
-000099c0: 681f 6a28 0600 0068 335d 722f 0600 0068  h.j(...h3]r/...h
-000099d0: 5258 0700 0000 7874 6f6c 203e 3d72 3006  RX....xtol >=r0.
-000099e0: 0000 8581 7231 0600 007d 7232 0600 0028  ....r1...}r2...(
-000099f0: 681e 5500 681f 6a2c 0600 0075 6261 6825  h.U.h.j,...ubah%
-00009a00: 6856 7562 6852 5831 0000 0020 7265 6c61  hVubhRX1... rela
-00009a10: 7469 7665 2063 6861 6e67 6520 696e 2070  tive change in p
-00009a20: 6172 616d 6574 6572 7320 6265 7477 6565  arameters betwee
-00009a30: 6e20 6974 6572 6174 696f 6e73 7233 0600  n iterationsr3..
-00009a40: 0085 8172 3406 0000 7d72 3506 0000 2868  ...r4...}r5...(h
-00009a50: 1e58 3100 0000 2072 656c 6174 6976 6520  .X1... relative 
-00009a60: 6368 616e 6765 2069 6e20 7061 7261 6d65  change in parame
-00009a70: 7465 7273 2062 6574 7765 656e 2069 7465  ters between ite
-00009a80: 7261 7469 6f6e 7368 1f6a 2806 0000 7562  rationsh.j(...ub
-00009a90: 6575 6261 6825 6a01 0200 0075 626a d401  eubah%j....ubj..
-00009aa0: 0000 2981 7236 0600 007d 7237 0600 0028  ..).r6...}r7...(
-00009ab0: 681e 5834 0000 0060 6067 746f 6c20 3e3d  h.X4...``gtol >=
-00009ac0: 6060 2072 656c 6174 6976 6520 7369 7a65  `` relative size
-00009ad0: 206f 6620 6772 6164 6965 6e74 206f 6620   of gradient of 
-00009ae0: 6060 6368 692a 2a32 6060 0a68 277d 7238  ``chi**2``.h'}r8
-00009af0: 0600 0028 6829 5d68 2a5d 682b 5d68 2c5d  ...(h)]h*]h+]h,]
-00009b00: 682f 5d75 681f 6a0f 0600 0068 335d 7239  h/]uh.j....h3]r9
-00009b10: 0600 0068 9729 8172 3a06 0000 7d72 3b06  ...h.).r:...}r;.
-00009b20: 0000 2868 1e58 3300 0000 6060 6774 6f6c  ..(h.X3...``gtol
-00009b30: 203e 3d60 6020 7265 6c61 7469 7665 2073   >=`` relative s
-00009b40: 697a 6520 6f66 2067 7261 6469 656e 7420  ize of gradient 
-00009b50: 6f66 2060 6063 6869 2a2a 3260 6068 1f6a  of ``chi**2``h.j
-00009b60: 3606 0000 6823 6a59 0100 0068 2568 9a68  6...h#jY...h%h.h
-00009b70: 277d 723c 0600 0028 6829 5d68 2a5d 682b  '}r<...(h)]h*]h+
-00009b80: 5d68 2c5d 682f 5d75 6831 4b63 6833 5d72  ]h,]h/]uh1Kch3]r
-00009b90: 3d06 0000 2868 4a29 8172 3e06 0000 7d72  =...(hJ).r>...}r
-00009ba0: 3f06 0000 2868 1e58 0b00 0000 6060 6774  ?...(h.X....``gt
-00009bb0: 6f6c 203e 3d60 6068 277d 7240 0600 0028  ol >=``h'}r@...(
-00009bc0: 6829 5d68 2a5d 682b 5d68 2c5d 682f 5d75  h)]h*]h+]h,]h/]u
-00009bd0: 681f 6a3a 0600 0068 335d 7241 0600 0068  h.j:...h3]rA...h
-00009be0: 5258 0700 0000 6774 6f6c 203e 3d72 4206  RX....gtol >=rB.
-00009bf0: 0000 8581 7243 0600 007d 7244 0600 0028  ....rC...}rD...(
-00009c00: 681e 5500 681f 6a3e 0600 0075 6261 6825  h.U.h.j>...ubah%
-00009c10: 6856 7562 6852 581e 0000 0020 7265 6c61  hVubhRX.... rela
-00009c20: 7469 7665 2073 697a 6520 6f66 2067 7261  tive size of gra
-00009c30: 6469 656e 7420 6f66 2072 4506 0000 8581  dient of rE.....
-00009c40: 7246 0600 007d 7247 0600 0028 681e 581e  rF...}rG...(h.X.
-00009c50: 0000 0020 7265 6c61 7469 7665 2073 697a  ... relative siz
-00009c60: 6520 6f66 2067 7261 6469 656e 7420 6f66  e of gradient of
-00009c70: 2068 1f6a 3a06 0000 7562 684a 2981 7248   h.j:...ubhJ).rH
-00009c80: 0600 007d 7249 0600 0028 681e 580a 0000  ...}rI...(h.X...
-00009c90: 0060 6063 6869 2a2a 3260 6068 277d 724a  .``chi**2``h'}rJ
-00009ca0: 0600 0028 6829 5d68 2a5d 682b 5d68 2c5d  ...(h)]h*]h+]h,]
-00009cb0: 682f 5d75 681f 6a3a 0600 0068 335d 724b  h/]uh.j:...h3]rK
-00009cc0: 0600 0068 5258 0600 0000 6368 692a 2a32  ...hRX....chi**2
-00009cd0: 724c 0600 0085 8172 4d06 0000 7d72 4e06  rL.....rM...}rN.
-00009ce0: 0000 2868 1e55 0068 1f6a 4806 0000 7562  ..(h.U.h.jH...ub
-00009cf0: 6168 2568 5675 6265 7562 6168 256a 0102  ah%hVubeubah%j..
-00009d00: 0000 7562 6ad4 0100 0029 8172 4f06 0000  ..ubj....).rO...
-00009d10: 7d72 5006 0000 2868 1e58 3c00 0000 6060  }rP...(h.X<...``
-00009d20: 6674 6f6c 203e 3d60 6020 7265 6c61 7469  ftol >=`` relati
-00009d30: 7665 2063 6861 6e67 6520 696e 2060 6063  ve change in ``c
-00009d40: 6869 2a2a 3260 6020 6265 7477 6565 6e20  hi**2`` between 
-00009d50: 6974 6572 6174 696f 6e73 7251 0600 0068  iterationsrQ...h
-00009d60: 277d 7252 0600 0028 6829 5d68 2a5d 682b  '}rR...(h)]h*]h+
-00009d70: 5d68 2c5d 682f 5d75 681f 6a0f 0600 0068  ]h,]h/]uh.j....h
-00009d80: 335d 7253 0600 0068 9729 8172 5406 0000  3]rS...h.).rT...
-00009d90: 7d72 5506 0000 2868 1e6a 5106 0000 681f  }rU...(h.jQ...h.
-00009da0: 6a4f 0600 0068 236a 5901 0000 6825 689a  jO...h#jY...h%h.
-00009db0: 6827 7d72 5606 0000 2868 295d 682a 5d68  h'}rV...(h)]h*]h
-00009dc0: 2b5d 682c 5d68 2f5d 7568 314b 6568 335d  +]h,]h/]uh1Keh3]
-00009dd0: 7257 0600 0028 684a 2981 7258 0600 007d  rW...(hJ).rX...}
-00009de0: 7259 0600 0028 681e 580b 0000 0060 6066  rY...(h.X....``f
-00009df0: 746f 6c20 3e3d 6060 6827 7d72 5a06 0000  tol >=``h'}rZ...
-00009e00: 2868 295d 682a 5d68 2b5d 682c 5d68 2f5d  (h)]h*]h+]h,]h/]
-00009e10: 7568 1f6a 5406 0000 6833 5d72 5b06 0000  uh.jT...h3]r[...
-00009e20: 6852 5807 0000 0066 746f 6c20 3e3d 725c  hRX....ftol >=r\
-00009e30: 0600 0085 8172 5d06 0000 7d72 5e06 0000  .....r]...}r^...
-00009e40: 2868 1e55 0068 1f6a 5806 0000 7562 6168  (h.U.h.jX...ubah
-00009e50: 2568 5675 6268 5258 1400 0000 2072 656c  %hVubhRX.... rel
-00009e60: 6174 6976 6520 6368 616e 6765 2069 6e20  ative change in 
-00009e70: 725f 0600 0085 8172 6006 0000 7d72 6106  r_.....r`...}ra.
-00009e80: 0000 2868 1e58 1400 0000 2072 656c 6174  ..(h.X.... relat
-00009e90: 6976 6520 6368 616e 6765 2069 6e20 681f  ive change in h.
-00009ea0: 6a54 0600 0075 6268 4a29 8172 6206 0000  jT...ubhJ).rb...
-00009eb0: 7d72 6306 0000 2868 1e58 0a00 0000 6060  }rc...(h.X....``
-00009ec0: 6368 692a 2a32 6060 6827 7d72 6406 0000  chi**2``h'}rd...
-00009ed0: 2868 295d 682a 5d68 2b5d 682c 5d68 2f5d  (h)]h*]h+]h,]h/]
-00009ee0: 7568 1f6a 5406 0000 6833 5d72 6506 0000  uh.jT...h3]re...
-00009ef0: 6852 5806 0000 0063 6869 2a2a 3272 6606  hRX....chi**2rf.
-00009f00: 0000 8581 7267 0600 007d 7268 0600 0028  ....rg...}rh...(
-00009f10: 681e 5500 681f 6a62 0600 0075 6261 6825  h.U.h.jb...ubah%
-00009f20: 6856 7562 6852 5813 0000 0020 6265 7477  hVubhRX.... betw
-00009f30: 6565 6e20 6974 6572 6174 696f 6e73 7269  een iterationsri
-00009f40: 0600 0085 8172 6a06 0000 7d72 6b06 0000  .....rj...}rk...
-00009f50: 2868 1e58 1300 0000 2062 6574 7765 656e  (h.X.... between
-00009f60: 2069 7465 7261 7469 6f6e 7368 1f6a 5406   iterationsh.jT.
-00009f70: 0000 7562 6575 6261 6825 6a01 0200 0075  ..ubeubah%j....u
-00009f80: 6265 6825 550f 656e 756d 6572 6174 6564  beh%U.enumerated
-00009f90: 5f6c 6973 7472 6c06 0000 7562 6175 6265  _listrl...ubaube
-00009fa0: 7562 6575 6268 cf29 8172 6d06 0000 7d72  ubeubh.).rm...}r
-00009fb0: 6e06 0000 2868 1e55 0068 1f6a 5101 0000  n...(h.U.h.jQ...
-00009fc0: 6823 6a59 0100 0068 2568 d268 277d 726f  h#jY...h%h.h'}ro
-00009fd0: 0600 0028 682c 5d68 2b5d 6829 5d68 2a5d  ...(h,]h+]h)]h*]
-00009fe0: 682f 5d55 0765 6e74 7269 6573 5d72 7006  h/]U.entries]rp.
-00009ff0: 0000 2868 d558 2c00 0000 6572 726f 7220  ..(h.X,...error 
-0000a000: 286c 7371 6669 742e 7363 6970 795f 6c65  (lsqfit.scipy_le
-0000a010: 6173 745f 7371 7561 7265 7320 6174 7472  ast_squares attr
-0000a020: 6962 7574 6529 6813 5500 4e74 7271 0600  ibute)h.U.Ntrq..
-0000a030: 0061 7568 314e 6832 6802 6833 5d75 6268  .auh1Nh2h.h3]ubh
-0000a040: d729 8172 7206 0000 7d72 7306 0000 2868  .).rr...}rs...(h
-0000a050: 1e55 0068 1f6a 5101 0000 6823 6a59 0100  .U.h.jQ...h#jY..
-0000a060: 0068 2568 da68 277d 7274 0600 0028 68dc  .h%h.h'}rt...(h.
-0000a070: 8968 dd58 0200 0000 7079 682c 5d68 2b5d  .h.X....pyh,]h+]
-0000a080: 6829 5d68 2a5d 682f 5d68 df58 0900 0000  h)]h*]h/]h.X....
-0000a090: 6174 7472 6962 7574 6572 7506 0000 68e1  attributeru...h.
-0000a0a0: 6a75 0600 0075 6831 4e68 3268 0268 335d  ju...uh1Nh2h.h3]
-0000a0b0: 7276 0600 0028 68e3 2981 7277 0600 007d  rv...(h.).rw...}
-0000a0c0: 7278 0600 0028 681e 5805 0000 0065 7272  rx...(h.X....err
-0000a0d0: 6f72 7279 0600 0068 1f6a 7206 0000 6823  orry...h.jr...h#
-0000a0e0: 6a59 0100 0068 2568 e768 277d 727a 0600  jY...h%h.h'}rz..
-0000a0f0: 0028 682c 5d72 7b06 0000 6813 6168 ea68  .(h,]r{...h.ah.h
-0000a100: ed68 2b5d 6829 5d68 2a5d 682f 5d72 7c06  .h+]h)]h*]h/]r|.
-0000a110: 0000 6813 6168 f058 1900 0000 7363 6970  ..h.ah.X....scip
-0000a120: 795f 6c65 6173 745f 7371 7561 7265 732e  y_least_squares.
-0000a130: 6572 726f 7268 f268 f168 f389 7568 314b  errorh.h.h..uh1K
-0000a140: 6b68 3268 0268 335d 727d 0600 006a 0901  kh2h.h3]r}...j..
-0000a150: 0000 2981 727e 0600 007d 727f 0600 0028  ..).r~...}r....(
-0000a160: 681e 6a79 0600 0068 1f6a 7706 0000 6823  h.jy...h.jw...h#
-0000a170: 6a59 0100 0068 256a 0c01 0000 6827 7d72  jY...h%j....h'}r
-0000a180: 8006 0000 2868 fa68 fb68 2c5d 682b 5d68  ....(h.h.h,]h+]h
-0000a190: 295d 682a 5d68 2f5d 7568 314b 6b68 3268  )]h*]h/]uh1Kkh2h
-0000a1a0: 0268 335d 7281 0600 0068 5258 0500 0000  .h3]r....hRX....
-0000a1b0: 6572 726f 7272 8206 0000 8581 7283 0600  errorr......r...
-0000a1c0: 007d 7284 0600 0028 681e 5500 6823 4e68  .}r....(h.U.h#Nh
-0000a1d0: 314e 6832 6802 681f 6a7e 0600 0075 6261  1Nh2h.h.j~...uba
-0000a1e0: 7562 6175 626a 5001 0000 2981 7285 0600  ubaubjP...).r...
-0000a1f0: 007d 7286 0600 0028 681e 5500 681f 6a72  .}r....(h.U.h.jr
-0000a200: 0600 0068 236a 5901 0000 6825 6a53 0100  ...h#jY...h%jS..
-0000a210: 0068 277d 7287 0600 0028 6829 5d68 2a5d  .h'}r....(h)]h*]
-0000a220: 682b 5d68 2c5d 682f 5d75 6831 4b6b 6832  h+]h,]h/]uh1Kkh2
-0000a230: 6802 6833 5d72 8806 0000 6897 2981 7289  h.h3]r....h.).r.
-0000a240: 0600 007d 728a 0600 0028 681e 5848 0000  ...}r....(h.XH..
-0000a250: 002a 7374 7220 6f72 204e 6f6e 652a 202d  .*str or None* -
-0000a260: 2d20 6060 4e6f 6e65 6060 2069 6620 6669  - ``None`` if fi
-0000a270: 7420 7375 6363 6573 7366 756c 3b20 616e  t successful; an
-0000a280: 2065 7272 6f72 0a6d 6573 7361 6765 206f   error.message o
-0000a290: 7468 6572 7769 7365 2e68 1f6a 8506 0000  therwise.h.j....
-0000a2a0: 6823 6a59 0100 0068 2568 9a68 277d 728b  h#jY...h%h.h'}r.
-0000a2b0: 0600 0028 6829 5d68 2a5d 682b 5d68 2c5d  ...(h)]h*]h+]h,]
-0000a2c0: 682f 5d75 6831 4b69 6832 6802 6833 5d72  h/]uh1Kih2h.h3]r
-0000a2d0: 8c06 0000 286a f204 0000 2981 728d 0600  ....(j....).r...
-0000a2e0: 007d 728e 0600 0028 681e 580d 0000 002a  .}r....(h.X....*
-0000a2f0: 7374 7220 6f72 204e 6f6e 652a 6827 7d72  str or None*h'}r
-0000a300: 8f06 0000 2868 295d 682a 5d68 2b5d 682c  ....(h)]h*]h+]h,
-0000a310: 5d68 2f5d 7568 1f6a 8906 0000 6833 5d72  ]h/]uh.j....h3]r
-0000a320: 9006 0000 6852 580b 0000 0073 7472 206f  ....hRX....str o
-0000a330: 7220 4e6f 6e65 7291 0600 0085 8172 9206  r Noner......r..
-0000a340: 0000 7d72 9306 0000 2868 1e55 0068 1f6a  ..}r....(h.U.h.j
-0000a350: 8d06 0000 7562 6168 256a fa04 0000 7562  ....ubah%j....ub
-0000a360: 6852 5805 0000 0020 e280 9320 7294 0600  hRX.... ... r...
-0000a370: 0085 8172 9506 0000 7d72 9606 0000 2868  ...r....}r....(h
-0000a380: 1e58 0400 0000 202d 2d20 6823 4e68 314e  .X.... -- h#Nh1N
-0000a390: 6832 6802 681f 6a89 0600 0075 6268 4a29  h2h.h.j....ubhJ)
-0000a3a0: 8172 9706 0000 7d72 9806 0000 2868 1e58  .r....}r....(h.X
-0000a3b0: 0800 0000 6060 4e6f 6e65 6060 6827 7d72  ....``None``h'}r
-0000a3c0: 9906 0000 2868 295d 682a 5d68 2b5d 682c  ....(h)]h*]h+]h,
-0000a3d0: 5d68 2f5d 7568 1f6a 8906 0000 6833 5d72  ]h/]uh.j....h3]r
-0000a3e0: 9a06 0000 6852 5804 0000 004e 6f6e 6572  ....hRX....Noner
-0000a3f0: 9b06 0000 8581 729c 0600 007d 729d 0600  ......r....}r...
-0000a400: 0028 681e 5500 681f 6a97 0600 0075 6261  .(h.U.h.j....uba
-0000a410: 6825 6856 7562 6852 582f 0000 0020 6966  h%hVubhRX/... if
-0000a420: 2066 6974 2073 7563 6365 7373 6675 6c3b   fit successful;
-0000a430: 2061 6e20 6572 726f 720a 6d65 7373 6167   an error.messag
-0000a440: 6520 6f74 6865 7277 6973 652e 729e 0600  e otherwise.r...
-0000a450: 0085 8172 9f06 0000 7d72 a006 0000 2868  ...r....}r....(h
-0000a460: 1e58 2f00 0000 2069 6620 6669 7420 7375  .X/... if fit su
-0000a470: 6363 6573 7366 756c 3b20 616e 2065 7272  ccessful; an err
-0000a480: 6f72 0a6d 6573 7361 6765 206f 7468 6572  or.message other
-0000a490: 7769 7365 2e68 234e 6831 4e68 3268 0268  wise.h#Nh1Nh2h.h
-0000a4a0: 1f6a 8906 0000 7562 6575 6261 7562 6575  .j....ubeubaubeu
-0000a4b0: 6268 cf29 8172 a106 0000 7d72 a206 0000  bh.).r....}r....
-0000a4c0: 2868 1e55 0068 1f6a 5101 0000 6823 6a59  (h.U.h.jQ...h#jY
-0000a4d0: 0100 0068 2568 d268 277d 72a3 0600 0028  ...h%h.h'}r....(
-0000a4e0: 682c 5d68 2b5d 6829 5d68 2a5d 682f 5d55  h,]h+]h)]h*]h/]U
-0000a4f0: 0765 6e74 7269 6573 5d72 a406 0000 2868  .entries]r....(h
-0000a500: d558 2e00 0000 7265 7375 6c74 7320 286c  .X....results (l
-0000a510: 7371 6669 742e 7363 6970 795f 6c65 6173  sqfit.scipy_leas
-0000a520: 745f 7371 7561 7265 7320 6174 7472 6962  t_squares attrib
-0000a530: 7574 6529 6810 5500 4e74 72a5 0600 0061  ute)h.U.Ntr....a
-0000a540: 7568 314e 6832 6802 6833 5d75 6268 d729  uh1Nh2h.h3]ubh.)
-0000a550: 8172 a606 0000 7d72 a706 0000 2868 1e55  .r....}r....(h.U
-0000a560: 0068 1f6a 5101 0000 6823 6a59 0100 0068  .h.jQ...h#jY...h
-0000a570: 2568 da68 277d 72a8 0600 0028 68dc 8968  %h.h'}r....(h..h
-0000a580: dd58 0200 0000 7079 682c 5d68 2b5d 6829  .X....pyh,]h+]h)
-0000a590: 5d68 2a5d 682f 5d68 df58 0900 0000 6174  ]h*]h/]h.X....at
-0000a5a0: 7472 6962 7574 6572 a906 0000 68e1 6aa9  tributer....h.j.
-0000a5b0: 0600 0075 6831 4e68 3268 0268 335d 72aa  ...uh1Nh2h.h3]r.
-0000a5c0: 0600 0028 68e3 2981 72ab 0600 007d 72ac  ...(h.).r....}r.
-0000a5d0: 0600 0028 681e 5807 0000 0072 6573 756c  ...(h.X....resul
-0000a5e0: 7473 72ad 0600 0068 1f6a a606 0000 6823  tsr....h.j....h#
-0000a5f0: 6a59 0100 0068 2568 e768 277d 72ae 0600  jY...h%h.h'}r...
-0000a600: 0028 682c 5d72 af06 0000 6810 6168 ea68  .(h,]r....h.ah.h
-0000a610: ed68 2b5d 6829 5d68 2a5d 682f 5d72 b006  .h+]h)]h*]h/]r..
-0000a620: 0000 6810 6168 f058 1b00 0000 7363 6970  ..h.ah.X....scip
-0000a630: 795f 6c65 6173 745f 7371 7561 7265 732e  y_least_squares.
-0000a640: 7265 7375 6c74 7368 f268 f168 f389 7568  resultsh.h.h..uh
-0000a650: 314b 6e68 3268 0268 335d 72b1 0600 006a  1Knh2h.h3]r....j
-0000a660: 0901 0000 2981 72b2 0600 007d 72b3 0600  ....).r....}r...
-0000a670: 0028 681e 6aad 0600 0068 1f6a ab06 0000  .(h.j....h.j....
-0000a680: 6823 6a59 0100 0068 256a 0c01 0000 6827  h#jY...h%j....h'
-0000a690: 7d72 b406 0000 2868 fa68 fb68 2c5d 682b  }r....(h.h.h,]h+
-0000a6a0: 5d68 295d 682a 5d68 2f5d 7568 314b 6e68  ]h)]h*]h/]uh1Knh
-0000a6b0: 3268 0268 335d 72b5 0600 0068 5258 0700  2h.h3]r....hRX..
-0000a6c0: 0000 7265 7375 6c74 7372 b606 0000 8581  ..resultsr......
-0000a6d0: 72b7 0600 007d 72b8 0600 0028 681e 5500  r....}r....(h.U.
-0000a6e0: 6823 4e68 314e 6832 6802 681f 6ab2 0600  h#Nh1Nh2h.h.j...
-0000a6f0: 0075 6261 7562 6175 626a 5001 0000 2981  .ubaubaubjP...).
-0000a700: 72b9 0600 007d 72ba 0600 0028 681e 5500  r....}r....(h.U.
-0000a710: 681f 6aa6 0600 0068 236a 5901 0000 6825  h.j....h#jY...h%
-0000a720: 6a53 0100 0068 277d 72bb 0600 0028 6829  jS...h'}r....(h)
-0000a730: 5d68 2a5d 682b 5d68 2c5d 682f 5d75 6831  ]h*]h+]h,]h/]uh1
-0000a740: 4b6e 6832 6802 6833 5d72 bc06 0000 6897  Knh2h.h3]r....h.
-0000a750: 2981 72bd 0600 007d 72be 0600 0028 681e  ).r....}r....(h.
-0000a760: 583f 0000 002a 6469 6374 2a20 2d2d 2052  X?...*dict* -- R
-0000a770: 6573 756c 7473 2072 6574 7572 6e65 6420  esults returned 
-0000a780: 6279 2060 6073 6369 7079 2e6f 7074 696d  by ``scipy.optim
-0000a790: 697a 652e 6c65 6173 745f 7371 7561 7265  ize.least_square
-0000a7a0: 7360 602e 681f 6ab9 0600 0068 236a 5901  s``.h.j....h#jY.
-0000a7b0: 0000 6825 689a 6827 7d72 bf06 0000 2868  ..h%h.h'}r....(h
-0000a7c0: 295d 682a 5d68 2b5d 682c 5d68 2f5d 7568  )]h*]h+]h,]h/]uh
-0000a7d0: 314b 6e68 3268 0268 335d 72c0 0600 0028  1Knh2h.h3]r....(
-0000a7e0: 6af2 0400 0029 8172 c106 0000 7d72 c206  j....).r....}r..
-0000a7f0: 0000 2868 1e58 0600 0000 2a64 6963 742a  ..(h.X....*dict*
-0000a800: 6827 7d72 c306 0000 2868 295d 682a 5d68  h'}r....(h)]h*]h
-0000a810: 2b5d 682c 5d68 2f5d 7568 1f6a bd06 0000  +]h,]h/]uh.j....
-0000a820: 6833 5d72 c406 0000 6852 5804 0000 0064  h3]r....hRX....d
-0000a830: 6963 7472 c506 0000 8581 72c6 0600 007d  ictr......r....}
-0000a840: 72c7 0600 0028 681e 5500 681f 6ac1 0600  r....(h.U.h.j...
-0000a850: 0075 6261 6825 6afa 0400 0075 6268 5258  .ubah%j....ubhRX
-0000a860: 1900 0000 20e2 8093 2052 6573 756c 7473  .... ... Results
-0000a870: 2072 6574 7572 6e65 6420 6279 2072 c806   returned by r..
-0000a880: 0000 8581 72c9 0600 007d 72ca 0600 0028  ....r....}r....(
-0000a890: 681e 5818 0000 0020 2d2d 2052 6573 756c  h.X.... -- Resul
-0000a8a0: 7473 2072 6574 7572 6e65 6420 6279 2068  ts returned by h
-0000a8b0: 234e 6831 4e68 3268 0268 1f6a bd06 0000  #Nh1Nh2h.h.j....
-0000a8c0: 7562 684a 2981 72cb 0600 007d 72cc 0600  ubhJ).r....}r...
-0000a8d0: 0028 681e 5820 0000 0060 6073 6369 7079  .(h.X ...``scipy
-0000a8e0: 2e6f 7074 696d 697a 652e 6c65 6173 745f  .optimize.least_
-0000a8f0: 7371 7561 7265 7360 6068 277d 72cd 0600  squares``h'}r...
-0000a900: 0028 6829 5d68 2a5d 682b 5d68 2c5d 682f  .(h)]h*]h+]h,]h/
-0000a910: 5d75 681f 6abd 0600 0068 335d 72ce 0600  ]uh.j....h3]r...
-0000a920: 0068 5258 1c00 0000 7363 6970 792e 6f70  .hRX....scipy.op
-0000a930: 7469 6d69 7a65 2e6c 6561 7374 5f73 7175  timize.least_squ
-0000a940: 6172 6573 72cf 0600 0085 8172 d006 0000  aresr......r....
-0000a950: 7d72 d106 0000 2868 1e55 0068 1f6a cb06  }r....(h.U.h.j..
-0000a960: 0000 7562 6168 2568 5675 6268 5258 0100  ..ubah%hVubhRX..
-0000a970: 0000 2e85 8172 d206 0000 7d72 d306 0000  .....r....}r....
-0000a980: 2868 1e58 0100 0000 2e68 234e 6831 4e68  (h.X.....h#Nh1Nh
-0000a990: 3268 0268 1f6a bd06 0000 7562 6575 6261  2h.h.j....ubeuba
-0000a9a0: 7562 6575 6265 7562 6575 6265 7562 6820  ubeubeubeubeubh 
-0000a9b0: 2981 72d4 0600 007d 72d5 0600 0028 681e  ).r....}r....(h.
-0000a9c0: 5500 681f 6821 6823 6824 6825 6826 6827  U.h.h!h#h$h%h&h'
-0000a9d0: 7d72 d606 0000 2868 295d 682a 5d68 2b5d  }r....(h)]h*]h+]
-0000a9e0: 682c 5d72 d706 0000 5509 6d69 6e69 6d69  h,]r....U.minimi
-0000a9f0: 7a65 7272 d806 0000 6168 2f5d 72d9 0600  zerr....ah/]r...
-0000aa00: 0068 1461 7568 314b 1368 3268 0268 335d  .h.auh1K.h2h.h3]
-0000aa10: 72da 0600 0028 6835 2981 72db 0600 007d  r....(h5).r....}
-0000aa20: 72dc 0600 0028 681e 5809 0000 004d 696e  r....(h.X....Min
-0000aa30: 696d 697a 6572 72dd 0600 0068 1f6a d406  imizerr....h.j..
-0000aa40: 0000 6823 6824 6825 6839 6827 7d72 de06  ..h#h$h%h9h'}r..
-0000aa50: 0000 2868 295d 682a 5d68 2b5d 682c 5d68  ..(h)]h*]h+]h,]h
-0000aa60: 2f5d 7568 314b 1368 3268 0268 335d 72df  /]uh1K.h2h.h3]r.
-0000aa70: 0600 0068 5258 0900 0000 4d69 6e69 6d69  ...hRX....Minimi
-0000aa80: 7a65 7272 e006 0000 8581 72e1 0600 007d  zerr......r....}
-0000aa90: 72e2 0600 0028 681e 6add 0600 0068 234e  r....(h.j....h#N
-0000aaa0: 6831 4e68 3268 0268 1f6a db06 0000 7562  h1Nh2h.h.j....ub
-0000aab0: 6175 6268 9729 8172 e306 0000 7d72 e406  aubh.).r....}r..
-0000aac0: 0000 2868 1e58 6500 0000 5468 6520 3a66  ..(h.Xe...The :f
-0000aad0: 756e 633a 606c 7371 6669 742e 656d 7062  unc:`lsqfit.empb
-0000aae0: 6179 6573 5f66 6974 6020 7573 6573 2061  ayes_fit` uses a
-0000aaf0: 206d 696e 696d 697a 6572 2066 726f 6d20   minimizer from 
-0000ab00: 7468 6520 3a6d 6f64 3a60 7363 6970 7960  the :mod:`scipy`
-0000ab10: 0a6d 6f64 756c 6520 746f 206d 696e 696d  .module to minim
-0000ab20: 697a 6520 6060 6c6f 6747 4246 6060 2e68  ize ``logGBF``.h
-0000ab30: 1f6a d406 0000 6823 6824 6825 689a 6827  .j....h#h$h%h.h'
-0000ab40: 7d72 e506 0000 2868 295d 682a 5d68 2b5d  }r....(h)]h*]h+]
-0000ab50: 682c 5d68 2f5d 7568 314b 1468 3268 0268  h,]h/]uh1K.h2h.h
-0000ab60: 335d 72e6 0600 0028 6852 5804 0000 0054  3]r....(hRX....T
-0000ab70: 6865 2072 e706 0000 8581 72e8 0600 007d  he r......r....}
-0000ab80: 72e9 0600 0028 681e 5804 0000 0054 6865  r....(h.X....The
-0000ab90: 2068 234e 6831 4e68 3268 0268 1f6a e306   h#Nh1Nh2h.h.j..
-0000aba0: 0000 7562 683c 2981 72ea 0600 007d 72eb  ..ubh<).r....}r.
-0000abb0: 0600 0028 681e 581b 0000 003a 6675 6e63  ...(h.X....:func
-0000abc0: 3a60 6c73 7166 6974 2e65 6d70 6261 7965  :`lsqfit.empbaye
-0000abd0: 735f 6669 7460 72ec 0600 0068 1f6a e306  s_fit`r....h.j..
-0000abe0: 0000 6823 6824 6825 6840 6827 7d72 ed06  ..h#h$h%h@h'}r..
-0000abf0: 0000 2855 0772 6566 7479 7065 5804 0000  ..(U.reftypeX...
-0000ac00: 0066 756e 6368 4289 6843 5813 0000 006c  .funchB.hCX....l
-0000ac10: 7371 6669 742e 656d 7062 6179 6573 5f66  sqfit.empbayes_f
-0000ac20: 6974 5509 7265 6664 6f6d 6169 6e58 0200  itU.refdomainX..
-0000ac30: 0000 7079 72ee 0600 0068 2c5d 682b 5d55  ..pyr....h,]h+]U
-0000ac40: 0b72 6566 6578 706c 6963 6974 8968 295d  .refexplicit.h)]
-0000ac50: 682a 5d68 2f5d 6845 6846 6847 4e68 484e  h*]h/]hEhFhGNhHN
-0000ac60: 7568 314b 1468 335d 72ef 0600 0068 4a29  uh1K.h3]r....hJ)
-0000ac70: 8172 f006 0000 7d72 f106 0000 2868 1e6a  .r....}r....(h.j
-0000ac80: ec06 0000 6827 7d72 f206 0000 2868 295d  ....h'}r....(h)]
-0000ac90: 682a 5d72 f306 0000 2868 4f6a ee06 0000  h*]r....(hOj....
-0000aca0: 5807 0000 0070 792d 6675 6e63 72f4 0600  X....py-funcr...
-0000acb0: 0065 682b 5d68 2c5d 682f 5d75 681f 6aea  .eh+]h,]h/]uh.j.
-0000acc0: 0600 0068 335d 72f5 0600 0068 5258 1500  ...h3]r....hRX..
-0000acd0: 0000 6c73 7166 6974 2e65 6d70 6261 7965  ..lsqfit.empbaye
-0000ace0: 735f 6669 7428 2972 f606 0000 8581 72f7  s_fit()r......r.
-0000acf0: 0600 007d 72f8 0600 0028 681e 5500 681f  ...}r....(h.U.h.
-0000ad00: 6af0 0600 0075 6261 6825 6856 7562 6175  j....ubah%hVubau
-0000ad10: 6268 5258 1b00 0000 2075 7365 7320 6120  bhRX.... uses a 
-0000ad20: 6d69 6e69 6d69 7a65 7220 6672 6f6d 2074  minimizer from t
-0000ad30: 6865 2072 f906 0000 8581 72fa 0600 007d  he r......r....}
-0000ad40: 72fb 0600 0028 681e 581b 0000 0020 7573  r....(h.X.... us
-0000ad50: 6573 2061 206d 696e 696d 697a 6572 2066  es a minimizer f
-0000ad60: 726f 6d20 7468 6520 6823 4e68 314e 6832  rom the h#Nh1Nh2
-0000ad70: 6802 681f 6ae3 0600 0075 6268 3c29 8172  h.h.j....ubh<).r
-0000ad80: fc06 0000 7d72 fd06 0000 2868 1e58 0c00  ....}r....(h.X..
-0000ad90: 0000 3a6d 6f64 3a60 7363 6970 7960 72fe  ..:mod:`scipy`r.
-0000ada0: 0600 0068 1f6a e306 0000 6823 6824 6825  ...h.j....h#h$h%
-0000adb0: 6840 6827 7d72 ff06 0000 2855 0772 6566  h@h'}r....(U.ref
-0000adc0: 7479 7065 5803 0000 006d 6f64 6842 8968  typeX....modhB.h
-0000add0: 4358 0500 0000 7363 6970 7955 0972 6566  CX....scipyU.ref
-0000ade0: 646f 6d61 696e 5802 0000 0070 7972 0007  domainX....pyr..
-0000adf0: 0000 682c 5d68 2b5d 550b 7265 6665 7870  ..h,]h+]U.refexp
-0000ae00: 6c69 6369 7489 6829 5d68 2a5d 682f 5d68  licit.h)]h*]h/]h
-0000ae10: 4568 4668 474e 6848 4e75 6831 4b14 6833  EhFhGNhHNuh1K.h3
-0000ae20: 5d72 0107 0000 684a 2981 7202 0700 007d  ]r....hJ).r....}
-0000ae30: 7203 0700 0028 681e 6afe 0600 0068 277d  r....(h.j....h'}
-0000ae40: 7204 0700 0028 6829 5d68 2a5d 7205 0700  r....(h)]h*]r...
-0000ae50: 0028 684f 6a00 0700 0058 0600 0000 7079  .(hOj....X....py
-0000ae60: 2d6d 6f64 7206 0700 0065 682b 5d68 2c5d  -modr....eh+]h,]
-0000ae70: 682f 5d75 681f 6afc 0600 0068 335d 7207  h/]uh.j....h3]r.
-0000ae80: 0700 0068 5258 0500 0000 7363 6970 7972  ...hRX....scipyr
-0000ae90: 0807 0000 8581 7209 0700 007d 720a 0700  ......r....}r...
-0000aea0: 0028 681e 5500 681f 6a02 0700 0075 6261  .(h.U.h.j....uba
-0000aeb0: 6825 6856 7562 6175 6268 5258 1400 0000  h%hVubaubhRX....
-0000aec0: 0a6d 6f64 756c 6520 746f 206d 696e 696d  .module to minim
-0000aed0: 697a 6520 720b 0700 0085 8172 0c07 0000  ize r......r....
-0000aee0: 7d72 0d07 0000 2868 1e58 1400 0000 0a6d  }r....(h.X.....m
-0000aef0: 6f64 756c 6520 746f 206d 696e 696d 697a  odule to minimiz
-0000af00: 6520 6823 4e68 314e 6832 6802 681f 6ae3  e h#Nh1Nh2h.h.j.
-0000af10: 0600 0075 6268 4a29 8172 0e07 0000 7d72  ...ubhJ).r....}r
-0000af20: 0f07 0000 2868 1e58 0a00 0000 6060 6c6f  ....(h.X....``lo
-0000af30: 6747 4246 6060 6827 7d72 1007 0000 2868  gGBF``h'}r....(h
-0000af40: 295d 682a 5d68 2b5d 682c 5d68 2f5d 7568  )]h*]h+]h,]h/]uh
-0000af50: 1f6a e306 0000 6833 5d72 1107 0000 6852  .j....h3]r....hR
-0000af60: 5806 0000 006c 6f67 4742 4672 1207 0000  X....logGBFr....
-0000af70: 8581 7213 0700 007d 7214 0700 0028 681e  ..r....}r....(h.
-0000af80: 5500 681f 6a0e 0700 0075 6261 6825 6856  U.h.j....ubah%hV
-0000af90: 7562 6852 5801 0000 002e 8581 7215 0700  ubhRX.......r...
-0000afa0: 007d 7216 0700 0028 681e 5801 0000 002e  .}r....(h.X.....
-0000afb0: 6823 4e68 314e 6832 6802 681f 6ae3 0600  h#Nh1Nh2h.h.j...
-0000afc0: 0075 6265 7562 68cf 2981 7217 0700 007d  .ubeubh.).r....}
-0000afd0: 7218 0700 0028 681e 5500 681f 6ad4 0600  r....(h.U.h.j...
-0000afe0: 0068 234e 6825 68d2 6827 7d72 1907 0000  .h#Nh%h.h'}r....
-0000aff0: 2868 2c5d 682b 5d68 295d 682a 5d68 2f5d  (h,]h+]h)]h*]h/]
-0000b000: 5507 656e 7472 6965 735d 721a 0700 0028  U.entries]r....(
-0000b010: 68d5 5822 0000 0073 6369 7079 5f6d 756c  h.X"...scipy_mul
-0000b020: 7469 6d69 6e65 7820 2863 6c61 7373 2069  timinex (class i
-0000b030: 6e20 6c73 7166 6974 2968 0755 004e 7472  n lsqfit)h.U.Ntr
-0000b040: 1b07 0000 6175 6831 4e68 3268 0268 335d  ....auh1Nh2h.h3]
-0000b050: 7562 68d7 2981 721c 0700 007d 721d 0700  ubh.).r....}r...
-0000b060: 0028 681e 5500 681f 6ad4 0600 0068 234e  .(h.U.h.j....h#N
-0000b070: 6825 68da 6827 7d72 1e07 0000 2868 dc89  h%h.h'}r....(h..
-0000b080: 68dd 5802 0000 0070 7972 1f07 0000 682c  h.X....pyr....h,
-0000b090: 5d68 2b5d 6829 5d68 2a5d 682f 5d68 df58  ]h+]h)]h*]h/]h.X
-0000b0a0: 0500 0000 636c 6173 7372 2007 0000 68e1  ....classr ...h.
-0000b0b0: 6a20 0700 0075 6831 4e68 3268 0268 335d  j ...uh1Nh2h.h3]
-0000b0c0: 7221 0700 0028 68e3 2981 7222 0700 007d  r!...(h.).r"...}
-0000b0d0: 7223 0700 0028 681e 5856 0000 0073 6369  r#...(h.XV...sci
-0000b0e0: 7079 5f6d 756c 7469 6d69 6e65 7828 7830  py_multiminex(x0
-0000b0f0: 2c20 662c 2074 6f6c 3d31 652d 342c 206d  , f, tol=1e-4, m
-0000b100: 6178 6974 3d31 3030 302c 2073 7465 703d  axit=1000, step=
-0000b110: 312c 2061 6c67 3d27 6e6d 7369 6d70 6c65  1, alg='nmsimple
-0000b120: 7832 272c 2061 6e61 6c79 7a65 723d 4e6f  x2', analyzer=No
-0000b130: 6e65 2968 1f6a 1c07 0000 6823 5866 0000  ne)h.j....h#Xf..
-0000b140: 002f 5573 6572 732f 6770 6c2f 616e 6163  ./Users/gpl/anac
-0000b150: 6f6e 6461 322f 6c69 622f 7079 7468 6f6e  onda2/lib/python
-0000b160: 322e 372f 7369 7465 2d70 6163 6b61 6765  2.7/site-package
-0000b170: 732f 6c73 7166 6974 2f5f 7363 6970 792e  s/lsqfit/_scipy.
-0000b180: 7079 3a64 6f63 7374 7269 6e67 206f 6620  py:docstring of 
-0000b190: 6c73 7166 6974 2e73 6369 7079 5f6d 756c  lsqfit.scipy_mul
-0000b1a0: 7469 6d69 6e65 7872 2407 0000 6825 68e7  timinexr$...h%h.
-0000b1b0: 6827 7d72 2507 0000 2868 2c5d 7226 0700  h'}r%...(h,]r&..
-0000b1c0: 0068 0761 68ea 68eb 5806 0000 006c 7371  .h.ah.h.X....lsq
-0000b1d0: 6669 7472 2707 0000 8581 7228 0700 007d  fitr'.....r(...}
-0000b1e0: 7229 0700 0062 682b 5d68 295d 682a 5d68  r)...bh+]h)]h*]h
-0000b1f0: 2f5d 722a 0700 0068 0761 68f0 5810 0000  /]r*...h.ah.X...
-0000b200: 0073 6369 7079 5f6d 756c 7469 6d69 6e65  .scipy_multimine
-0000b210: 7872 2b07 0000 68f2 5500 68f3 8975 6831  xr+...h.U.h..uh1
-0000b220: 4e68 3268 0268 335d 722c 0700 0028 68f5  Nh2h.h3]r,...(h.
-0000b230: 2981 722d 0700 007d 722e 0700 0028 681e  ).r-...}r....(h.
-0000b240: 5806 0000 0063 6c61 7373 2068 1f6a 2207  X....class h.j".
-0000b250: 0000 6823 6a24 0700 0068 2568 f868 277d  ..h#j$...h%h.h'}
-0000b260: 722f 0700 0028 68fa 68fb 682c 5d68 2b5d  r/...(h.h.h,]h+]
-0000b270: 6829 5d68 2a5d 682f 5d75 6831 4e68 3268  h)]h*]h/]uh1Nh2h
-0000b280: 0268 335d 7230 0700 0068 5258 0600 0000  .h3]r0...hRX....
-0000b290: 636c 6173 7320 7231 0700 0085 8172 3207  class r1.....r2.
-0000b2a0: 0000 7d72 3307 0000 2868 1e55 0068 234e  ..}r3...(h.U.h#N
-0000b2b0: 6831 4e68 3268 0268 1f6a 2d07 0000 7562  h1Nh2h.h.j-...ub
-0000b2c0: 6175 626a 0001 0000 2981 7234 0700 007d  aubj....).r4...}
-0000b2d0: 7235 0700 0028 681e 5807 0000 006c 7371  r5...(h.X....lsq
-0000b2e0: 6669 742e 681f 6a22 0700 0068 236a 2407  fit.h.j"...h#j$.
-0000b2f0: 0000 6825 6a03 0100 0068 277d 7236 0700  ..h%j....h'}r6..
-0000b300: 0028 68fa 68fb 682c 5d68 2b5d 6829 5d68  .(h.h.h,]h+]h)]h
-0000b310: 2a5d 682f 5d75 6831 4e68 3268 0268 335d  *]h/]uh1Nh2h.h3]
-0000b320: 7237 0700 0068 5258 0700 0000 6c73 7166  r7...hRX....lsqf
-0000b330: 6974 2e72 3807 0000 8581 7239 0700 007d  it.r8.....r9...}
-0000b340: 723a 0700 0028 681e 5500 6823 4e68 314e  r:...(h.U.h#Nh1N
-0000b350: 6832 6802 681f 6a34 0700 0075 6261 7562  h2h.h.j4...ubaub
-0000b360: 6a09 0100 0029 8172 3b07 0000 7d72 3c07  j....).r;...}r<.
-0000b370: 0000 2868 1e6a 2b07 0000 681f 6a22 0700  ..(h.j+...h.j"..
-0000b380: 0068 236a 2407 0000 6825 6a0c 0100 0068  .h#j$...h%j....h
-0000b390: 277d 723d 0700 0028 68fa 68fb 682c 5d68  '}r=...(h.h.h,]h
-0000b3a0: 2b5d 6829 5d68 2a5d 682f 5d75 6831 4e68  +]h)]h*]h/]uh1Nh
-0000b3b0: 3268 0268 335d 723e 0700 0068 5258 1000  2h.h3]r>...hRX..
-0000b3c0: 0000 7363 6970 795f 6d75 6c74 696d 696e  ..scipy_multimin
-0000b3d0: 6578 723f 0700 0085 8172 4007 0000 7d72  exr?.....r@...}r
-0000b3e0: 4107 0000 2868 1e55 0068 234e 6831 4e68  A...(h.U.h#Nh1Nh
-0000b3f0: 3268 0268 1f6a 3b07 0000 7562 6175 626a  2h.h.j;...ubaubj
-0000b400: 1201 0000 2981 7242 0700 007d 7243 0700  ....).rB...}rC..
-0000b410: 0028 681e 5844 0000 0078 302c 2066 2c20  .(h.XD...x0, f, 
-0000b420: 746f 6c3d 3165 2d34 2c20 6d61 7869 743d  tol=1e-4, maxit=
-0000b430: 3130 3030 2c20 7374 6570 3d31 2c20 616c  1000, step=1, al
-0000b440: 673d 276e 6d73 696d 706c 6578 3227 2c20  g='nmsimplex2', 
-0000b450: 616e 616c 797a 6572 3d4e 6f6e 6568 1f6a  analyzer=Noneh.j
-0000b460: 2207 0000 6823 6a24 0700 0068 256a 1501  "...h#j$...h%j..
-0000b470: 0000 6827 7d72 4407 0000 2868 fa68 fb68  ..h'}rD...(h.h.h
-0000b480: 2c5d 682b 5d68 295d 682a 5d68 2f5d 7568  ,]h+]h)]h*]h/]uh
-0000b490: 314e 6832 6802 6833 5d72 4507 0000 286a  1Nh2h.h3]rE...(j
-0000b4a0: 1801 0000 2981 7246 0700 007d 7247 0700  ....).rF...}rG..
-0000b4b0: 0028 681e 5802 0000 0078 3068 277d 7248  .(h.X....x0h'}rH
-0000b4c0: 0700 0028 68fa 68fb 682c 5d68 2b5d 6829  ...(h.h.h,]h+]h)
-0000b4d0: 5d68 2a5d 682f 5d75 681f 6a42 0700 0068  ]h*]h/]uh.jB...h
-0000b4e0: 335d 7249 0700 0068 5258 0200 0000 7830  3]rI...hRX....x0
-0000b4f0: 724a 0700 0085 8172 4b07 0000 7d72 4c07  rJ.....rK...}rL.
-0000b500: 0000 2868 1e55 0068 1f6a 4607 0000 7562  ..(h.U.h.jF...ub
-0000b510: 6168 256a 2001 0000 7562 6a18 0100 0029  ah%j ...ubj....)
-0000b520: 8172 4d07 0000 7d72 4e07 0000 2868 1e58  .rM...}rN...(h.X
-0000b530: 0100 0000 6668 277d 724f 0700 0028 68fa  ....fh'}rO...(h.
-0000b540: 68fb 682c 5d68 2b5d 6829 5d68 2a5d 682f  h.h,]h+]h)]h*]h/
-0000b550: 5d75 681f 6a42 0700 0068 335d 7250 0700  ]uh.jB...h3]rP..
-0000b560: 0068 5258 0100 0000 6685 8172 5107 0000  .hRX....f..rQ...
-0000b570: 7d72 5207 0000 2868 1e55 0068 1f6a 4d07  }rR...(h.U.h.jM.
-0000b580: 0000 7562 6168 256a 2001 0000 7562 6a18  ..ubah%j ...ubj.
-0000b590: 0100 0029 8172 5307 0000 7d72 5407 0000  ...).rS...}rT...
-0000b5a0: 2868 1e58 0800 0000 746f 6c3d 3165 2d34  (h.X....tol=1e-4
-0000b5b0: 6827 7d72 5507 0000 2868 fa68 fb68 2c5d  h'}rU...(h.h.h,]
-0000b5c0: 682b 5d68 295d 682a 5d68 2f5d 7568 1f6a  h+]h)]h*]h/]uh.j
-0000b5d0: 4207 0000 6833 5d72 5607 0000 6852 5808  B...h3]rV...hRX.
-0000b5e0: 0000 0074 6f6c 3d31 652d 3472 5707 0000  ...tol=1e-4rW...
-0000b5f0: 8581 7258 0700 007d 7259 0700 0028 681e  ..rX...}rY...(h.
-0000b600: 5500 681f 6a53 0700 0075 6261 6825 6a20  U.h.jS...ubah%j 
-0000b610: 0100 0075 626a 1801 0000 2981 725a 0700  ...ubj....).rZ..
-0000b620: 007d 725b 0700 0028 681e 580a 0000 006d  .}r[...(h.X....m
-0000b630: 6178 6974 3d31 3030 3068 277d 725c 0700  axit=1000h'}r\..
-0000b640: 0028 68fa 68fb 682c 5d68 2b5d 6829 5d68  .(h.h.h,]h+]h)]h
-0000b650: 2a5d 682f 5d75 681f 6a42 0700 0068 335d  *]h/]uh.jB...h3]
-0000b660: 725d 0700 0068 5258 0a00 0000 6d61 7869  r]...hRX....maxi
-0000b670: 743d 3130 3030 725e 0700 0085 8172 5f07  t=1000r^.....r_.
-0000b680: 0000 7d72 6007 0000 2868 1e55 0068 1f6a  ..}r`...(h.U.h.j
-0000b690: 5a07 0000 7562 6168 256a 2001 0000 7562  Z...ubah%j ...ub
-0000b6a0: 6a18 0100 0029 8172 6107 0000 7d72 6207  j....).ra...}rb.
-0000b6b0: 0000 2868 1e58 0600 0000 7374 6570 3d31  ..(h.X....step=1
-0000b6c0: 6827 7d72 6307 0000 2868 fa68 fb68 2c5d  h'}rc...(h.h.h,]
-0000b6d0: 682b 5d68 295d 682a 5d68 2f5d 7568 1f6a  h+]h)]h*]h/]uh.j
-0000b6e0: 4207 0000 6833 5d72 6407 0000 6852 5806  B...h3]rd...hRX.
-0000b6f0: 0000 0073 7465 703d 3172 6507 0000 8581  ...step=1re.....
-0000b700: 7266 0700 007d 7267 0700 0028 681e 5500  rf...}rg...(h.U.
-0000b710: 681f 6a61 0700 0075 6261 6825 6a20 0100  h.ja...ubah%j ..
-0000b720: 0075 626a 1801 0000 2981 7268 0700 007d  .ubj....).rh...}
-0000b730: 7269 0700 0028 681e 5810 0000 0061 6c67  ri...(h.X....alg
-0000b740: 3d27 6e6d 7369 6d70 6c65 7832 2768 277d  ='nmsimplex2'h'}
-0000b750: 726a 0700 0028 68fa 68fb 682c 5d68 2b5d  rj...(h.h.h,]h+]
-0000b760: 6829 5d68 2a5d 682f 5d75 681f 6a42 0700  h)]h*]h/]uh.jB..
-0000b770: 0068 335d 726b 0700 0068 5258 1000 0000  .h3]rk...hRX....
-0000b780: 616c 673d 276e 6d73 696d 706c 6578 3227  alg='nmsimplex2'
-0000b790: 726c 0700 0085 8172 6d07 0000 7d72 6e07  rl.....rm...}rn.
-0000b7a0: 0000 2868 1e55 0068 1f6a 6807 0000 7562  ..(h.U.h.jh...ub
-0000b7b0: 6168 256a 2001 0000 7562 6a18 0100 0029  ah%j ...ubj....)
-0000b7c0: 8172 6f07 0000 7d72 7007 0000 2868 1e58  .ro...}rp...(h.X
-0000b7d0: 0d00 0000 616e 616c 797a 6572 3d4e 6f6e  ....analyzer=Non
-0000b7e0: 6568 277d 7271 0700 0028 68fa 68fb 682c  eh'}rq...(h.h.h,
-0000b7f0: 5d68 2b5d 6829 5d68 2a5d 682f 5d75 681f  ]h+]h)]h*]h/]uh.
-0000b800: 6a42 0700 0068 335d 7272 0700 0068 5258  jB...h3]rr...hRX
-0000b810: 0d00 0000 616e 616c 797a 6572 3d4e 6f6e  ....analyzer=Non
-0000b820: 6572 7307 0000 8581 7274 0700 007d 7275  ers.....rt...}ru
-0000b830: 0700 0028 681e 5500 681f 6a6f 0700 0075  ...(h.U.h.jo...u
-0000b840: 6261 6825 6a20 0100 0075 6265 7562 6575  bah%j ...ubeubeu
-0000b850: 626a 5001 0000 2981 7276 0700 007d 7277  bjP...).rv...}rw
-0000b860: 0700 0028 681e 5500 681f 6a1c 0700 0068  ...(h.U.h.j....h
-0000b870: 236a 2407 0000 6825 6a53 0100 0068 277d  #j$...h%jS...h'}
-0000b880: 7278 0700 0028 6829 5d68 2a5d 682b 5d68  rx...(h)]h*]h+]h
-0000b890: 2c5d 682f 5d75 6831 4e68 3268 0268 335d  ,]h/]uh1Nh2h.h3]
-0000b8a0: 7279 0700 0028 6897 2981 727a 0700 007d  ry...(h.).rz...}
-0000b8b0: 727b 0700 0028 681e 5836 0000 003a 6d6f  r{...(h.X6...:mo
-0000b8c0: 643a 6073 6369 7079 6020 6d69 6e69 6d69  d:`scipy` minimi
-0000b8d0: 7a65 7220 666f 7220 6d75 6c74 6964 696d  zer for multidim
-0000b8e0: 656e 7369 6f6e 616c 2066 756e 6374 696f  ensional functio
-0000b8f0: 6e73 2e72 7c07 0000 681f 6a76 0700 0068  ns.r|...h.jv...h
-0000b900: 2358 6600 0000 2f55 7365 7273 2f67 706c  #Xf.../Users/gpl
-0000b910: 2f61 6e61 636f 6e64 6132 2f6c 6962 2f70  /anaconda2/lib/p
-0000b920: 7974 686f 6e32 2e37 2f73 6974 652d 7061  ython2.7/site-pa
-0000b930: 636b 6167 6573 2f6c 7371 6669 742f 5f73  ckages/lsqfit/_s
-0000b940: 6369 7079 2e70 793a 646f 6373 7472 696e  cipy.py:docstrin
-0000b950: 6720 6f66 206c 7371 6669 742e 7363 6970  g of lsqfit.scip
-0000b960: 795f 6d75 6c74 696d 696e 6578 727d 0700  y_multiminexr}..
-0000b970: 0068 2568 9a68 277d 727e 0700 0028 6829  .h%h.h'}r~...(h)
-0000b980: 5d68 2a5d 682b 5d68 2c5d 682f 5d75 6831  ]h*]h+]h,]h/]uh1
-0000b990: 4b01 6832 6802 6833 5d72 7f07 0000 2868  K.h2h.h3]r....(h
-0000b9a0: 3c29 8172 8007 0000 7d72 8107 0000 2868  <).r....}r....(h
-0000b9b0: 1e58 0c00 0000 3a6d 6f64 3a60 7363 6970  .X....:mod:`scip
-0000b9c0: 7960 7282 0700 0068 1f6a 7a07 0000 6823  y`r....h.jz...h#
-0000b9d0: 6a7d 0700 0068 2568 4068 277d 7283 0700  j}...h%h@h'}r...
-0000b9e0: 0028 5507 7265 6674 7970 6558 0300 0000  .(U.reftypeX....
-0000b9f0: 6d6f 6468 4289 6843 5805 0000 0073 6369  modhB.hCX....sci
-0000ba00: 7079 5509 7265 6664 6f6d 6169 6e58 0200  pyU.refdomainX..
-0000ba10: 0000 7079 7284 0700 0068 2c5d 682b 5d55  ..pyr....h,]h+]U
-0000ba20: 0b72 6566 6578 706c 6963 6974 8968 295d  .refexplicit.h)]
-0000ba30: 682a 5d68 2f5d 6845 6846 6847 6a2b 0700  h*]h/]hEhFhGj+..
-0000ba40: 0068 486a 2807 0000 7568 314b 0168 335d  .hHj(...uh1K.h3]
-0000ba50: 7285 0700 0068 4a29 8172 8607 0000 7d72  r....hJ).r....}r
-0000ba60: 8707 0000 2868 1e6a 8207 0000 6827 7d72  ....(h.j....h'}r
-0000ba70: 8807 0000 2868 295d 682a 5d72 8907 0000  ....(h)]h*]r....
-0000ba80: 2868 4f6a 8407 0000 5806 0000 0070 792d  (hOj....X....py-
-0000ba90: 6d6f 6472 8a07 0000 6568 2b5d 682c 5d68  modr....eh+]h,]h
-0000baa0: 2f5d 7568 1f6a 8007 0000 6833 5d72 8b07  /]uh.j....h3]r..
-0000bab0: 0000 6852 5805 0000 0073 6369 7079 728c  ..hRX....scipyr.
-0000bac0: 0700 0085 8172 8d07 0000 7d72 8e07 0000  .....r....}r....
-0000bad0: 2868 1e55 0068 1f6a 8607 0000 7562 6168  (h.U.h.j....ubah
-0000bae0: 2568 5675 6261 7562 6852 582a 0000 0020  %hVubaubhRX*... 
-0000baf0: 6d69 6e69 6d69 7a65 7220 666f 7220 6d75  minimizer for mu
-0000bb00: 6c74 6964 696d 656e 7369 6f6e 616c 2066  ltidimensional f
-0000bb10: 756e 6374 696f 6e73 2e72 8f07 0000 8581  unctions.r......
-0000bb20: 7290 0700 007d 7291 0700 0028 681e 582a  r....}r....(h.X*
-0000bb30: 0000 0020 6d69 6e69 6d69 7a65 7220 666f  ... minimizer fo
-0000bb40: 7220 6d75 6c74 6964 696d 656e 7369 6f6e  r multidimension
-0000bb50: 616c 2066 756e 6374 696f 6e73 2e68 234e  al functions.h#N
-0000bb60: 6831 4e68 3268 0268 1f6a 7a07 0000 7562  h1Nh2h.h.jz...ub
-0000bb70: 6575 6268 9729 8172 9207 0000 7d72 9307  eubh.).r....}r..
-0000bb80: 0000 2868 1e58 dd00 0000 3a63 6c61 7373  ..(h.X....:class
-0000bb90: 3a60 7363 6970 795f 6d75 6c74 696d 696e  :`scipy_multimin
-0000bba0: 6578 6020 6973 2061 2066 756e 6374 696f  ex` is a functio
-0000bbb0: 6e2d 636c 6173 7320 7768 6f73 6520 636f  n-class whose co
-0000bbc0: 6e73 7472 7563 746f 7220 6d69 6e69 6d69  nstructor minimi
-0000bbd0: 7a65 7320 610a 6d75 6c74 6964 696d 656e  zes a.multidimen
-0000bbe0: 7369 6f6e 616c 2066 756e 6374 696f 6e20  sional function 
-0000bbf0: 6060 6628 7829 6060 2062 7920 7661 7279  ``f(x)`` by vary
-0000bc00: 696e 6720 7665 6374 6f72 2060 6078 6060  ing vector ``x``
-0000bc10: 2e20 5468 6973 2072 6f75 7469 6e65 0a64  . This routine.d
-0000bc20: 6f65 7320 2a6e 6f74 2a20 7573 6520 7573  oes *not* use us
-0000bc30: 6572 2d73 7570 706c 6965 6420 696e 666f  er-supplied info
-0000bc40: 726d 6174 696f 6e20 6162 6f75 7420 7468  rmation about th
-0000bc50: 6520 6772 6164 6965 6e74 206f 6620 6060  e gradient of ``
-0000bc60: 6628 7829 6060 2e68 1f6a 7607 0000 6823  f(x)``.h.jv...h#
-0000bc70: 6a7d 0700 0068 2568 9a68 277d 7294 0700  j}...h%h.h'}r...
-0000bc80: 0028 6829 5d68 2a5d 682b 5d68 2c5d 682f  .(h)]h*]h+]h,]h/
-0000bc90: 5d75 6831 4b03 6832 6802 6833 5d72 9507  ]uh1K.h2h.h3]r..
-0000bca0: 0000 2868 3c29 8172 9607 0000 7d72 9707  ..(h<).r....}r..
-0000bcb0: 0000 2868 1e58 1900 0000 3a63 6c61 7373  ..(h.X....:class
-0000bcc0: 3a60 7363 6970 795f 6d75 6c74 696d 696e  :`scipy_multimin
-0000bcd0: 6578 6072 9807 0000 681f 6a92 0700 0068  ex`r....h.j....h
-0000bce0: 236a 7d07 0000 6825 6840 6827 7d72 9907  #j}...h%h@h'}r..
-0000bcf0: 0000 2855 0772 6566 7479 7065 5805 0000  ..(U.reftypeX...
-0000bd00: 0063 6c61 7373 6842 8968 4358 1000 0000  .classhB.hCX....
-0000bd10: 7363 6970 795f 6d75 6c74 696d 696e 6578  scipy_multiminex
-0000bd20: 5509 7265 6664 6f6d 6169 6e58 0200 0000  U.refdomainX....
-0000bd30: 7079 729a 0700 0068 2c5d 682b 5d55 0b72  pyr....h,]h+]U.r
-0000bd40: 6566 6578 706c 6963 6974 8968 295d 682a  efexplicit.h)]h*
-0000bd50: 5d68 2f5d 6845 6846 6847 6a2b 0700 0068  ]h/]hEhFhGj+...h
-0000bd60: 486a 2807 0000 7568 314b 0368 335d 729b  Hj(...uh1K.h3]r.
-0000bd70: 0700 0068 4a29 8172 9c07 0000 7d72 9d07  ...hJ).r....}r..
-0000bd80: 0000 2868 1e6a 9807 0000 6827 7d72 9e07  ..(h.j....h'}r..
-0000bd90: 0000 2868 295d 682a 5d72 9f07 0000 2868  ..(h)]h*]r....(h
-0000bda0: 4f6a 9a07 0000 5808 0000 0070 792d 636c  Oj....X....py-cl
-0000bdb0: 6173 7372 a007 0000 6568 2b5d 682c 5d68  assr....eh+]h,]h
-0000bdc0: 2f5d 7568 1f6a 9607 0000 6833 5d72 a107  /]uh.j....h3]r..
-0000bdd0: 0000 6852 5810 0000 0073 6369 7079 5f6d  ..hRX....scipy_m
-0000bde0: 756c 7469 6d69 6e65 7872 a207 0000 8581  ultiminexr......
-0000bdf0: 72a3 0700 007d 72a4 0700 0028 681e 5500  r....}r....(h.U.
-0000be00: 681f 6a9c 0700 0075 6261 6825 6856 7562  h.j....ubah%hVub
-0000be10: 6175 6268 5258 4d00 0000 2069 7320 6120  aubhRXM... is a 
-0000be20: 6675 6e63 7469 6f6e 2d63 6c61 7373 2077  function-class w
-0000be30: 686f 7365 2063 6f6e 7374 7275 6374 6f72  hose constructor
-0000be40: 206d 696e 696d 697a 6573 2061 0a6d 756c   minimizes a.mul
-0000be50: 7469 6469 6d65 6e73 696f 6e61 6c20 6675  tidimensional fu
-0000be60: 6e63 7469 6f6e 2072 a507 0000 8581 72a6  nction r......r.
-0000be70: 0700 007d 72a7 0700 0028 681e 584d 0000  ...}r....(h.XM..
-0000be80: 0020 6973 2061 2066 756e 6374 696f 6e2d  . is a function-
-0000be90: 636c 6173 7320 7768 6f73 6520 636f 6e73  class whose cons
-0000bea0: 7472 7563 746f 7220 6d69 6e69 6d69 7a65  tructor minimize
-0000beb0: 7320 610a 6d75 6c74 6964 696d 656e 7369  s a.multidimensi
-0000bec0: 6f6e 616c 2066 756e 6374 696f 6e20 6823  onal function h#
-0000bed0: 4e68 314e 6832 6802 681f 6a92 0700 0075  Nh1Nh2h.h.j....u
-0000bee0: 6268 4a29 8172 a807 0000 7d72 a907 0000  bhJ).r....}r....
-0000bef0: 2868 1e58 0800 0000 6060 6628 7829 6060  (h.X....``f(x)``
-0000bf00: 6827 7d72 aa07 0000 2868 295d 682a 5d68  h'}r....(h)]h*]h
-0000bf10: 2b5d 682c 5d68 2f5d 7568 1f6a 9207 0000  +]h,]h/]uh.j....
-0000bf20: 6833 5d72 ab07 0000 6852 5804 0000 0066  h3]r....hRX....f
-0000bf30: 2878 2972 ac07 0000 8581 72ad 0700 007d  (x)r......r....}
-0000bf40: 72ae 0700 0028 681e 5500 681f 6aa8 0700  r....(h.U.h.j...
-0000bf50: 0075 6261 6825 6856 7562 6852 5813 0000  .ubah%hVubhRX...
-0000bf60: 0020 6279 2076 6172 7969 6e67 2076 6563  . by varying vec
-0000bf70: 746f 7220 72af 0700 0085 8172 b007 0000  tor r......r....
-0000bf80: 7d72 b107 0000 2868 1e58 1300 0000 2062  }r....(h.X.... b
-0000bf90: 7920 7661 7279 696e 6720 7665 6374 6f72  y varying vector
-0000bfa0: 2068 234e 6831 4e68 3268 0268 1f6a 9207   h#Nh1Nh2h.h.j..
-0000bfb0: 0000 7562 684a 2981 72b2 0700 007d 72b3  ..ubhJ).r....}r.
-0000bfc0: 0700 0028 681e 5805 0000 0060 6078 6060  ...(h.X....``x``
-0000bfd0: 6827 7d72 b407 0000 2868 295d 682a 5d68  h'}r....(h)]h*]h
-0000bfe0: 2b5d 682c 5d68 2f5d 7568 1f6a 9207 0000  +]h,]h/]uh.j....
-0000bff0: 6833 5d72 b507 0000 6852 5801 0000 0078  h3]r....hRX....x
-0000c000: 8581 72b6 0700 007d 72b7 0700 0028 681e  ..r....}r....(h.
-0000c010: 5500 681f 6ab2 0700 0075 6261 6825 6856  U.h.j....ubah%hV
-0000c020: 7562 6852 5814 0000 002e 2054 6869 7320  ubhRX..... This 
-0000c030: 726f 7574 696e 650a 646f 6573 2072 b807  routine.does r..
-0000c040: 0000 8581 72b9 0700 007d 72ba 0700 0028  ....r....}r....(
-0000c050: 681e 5814 0000 002e 2054 6869 7320 726f  h.X..... This ro
-0000c060: 7574 696e 650a 646f 6573 2068 234e 6831  utine.does h#Nh1
-0000c070: 4e68 3268 0268 1f6a 9207 0000 7562 6af2  Nh2h.h.j....ubj.
-0000c080: 0400 0029 8172 bb07 0000 7d72 bc07 0000  ...).r....}r....
-0000c090: 2868 1e58 0500 0000 2a6e 6f74 2a68 277d  (h.X....*not*h'}
-0000c0a0: 72bd 0700 0028 6829 5d68 2a5d 682b 5d68  r....(h)]h*]h+]h
-0000c0b0: 2c5d 682f 5d75 681f 6a92 0700 0068 335d  ,]h/]uh.j....h3]
-0000c0c0: 72be 0700 0068 5258 0300 0000 6e6f 7472  r....hRX....notr
-0000c0d0: bf07 0000 8581 72c0 0700 007d 72c1 0700  ......r....}r...
-0000c0e0: 0028 681e 5500 681f 6abb 0700 0075 6261  .(h.U.h.j....uba
-0000c0f0: 6825 6afa 0400 0075 6268 5258 3500 0000  h%j....ubhRX5...
-0000c100: 2075 7365 2075 7365 722d 7375 7070 6c69   use user-suppli
-0000c110: 6564 2069 6e66 6f72 6d61 7469 6f6e 2061  ed information a
-0000c120: 626f 7574 2074 6865 2067 7261 6469 656e  bout the gradien
-0000c130: 7420 6f66 2072 c207 0000 8581 72c3 0700  t of r......r...
-0000c140: 007d 72c4 0700 0028 681e 5835 0000 0020  .}r....(h.X5... 
-0000c150: 7573 6520 7573 6572 2d73 7570 706c 6965  use user-supplie
-0000c160: 6420 696e 666f 726d 6174 696f 6e20 6162  d information ab
-0000c170: 6f75 7420 7468 6520 6772 6164 6965 6e74  out the gradient
-0000c180: 206f 6620 6823 4e68 314e 6832 6802 681f   of h#Nh1Nh2h.h.
-0000c190: 6a92 0700 0075 6268 4a29 8172 c507 0000  j....ubhJ).r....
-0000c1a0: 7d72 c607 0000 2868 1e58 0800 0000 6060  }r....(h.X....``
-0000c1b0: 6628 7829 6060 6827 7d72 c707 0000 2868  f(x)``h'}r....(h
-0000c1c0: 295d 682a 5d68 2b5d 682c 5d68 2f5d 7568  )]h*]h+]h,]h/]uh
-0000c1d0: 1f6a 9207 0000 6833 5d72 c807 0000 6852  .j....h3]r....hR
-0000c1e0: 5804 0000 0066 2878 2972 c907 0000 8581  X....f(x)r......
-0000c1f0: 72ca 0700 007d 72cb 0700 0028 681e 5500  r....}r....(h.U.
-0000c200: 681f 6ac5 0700 0075 6261 6825 6856 7562  h.j....ubah%hVub
-0000c210: 6852 5801 0000 002e 8581 72cc 0700 007d  hRX.......r....}
-0000c220: 72cd 0700 0028 681e 5801 0000 002e 6823  r....(h.X.....h#
-0000c230: 4e68 314e 6832 6802 681f 6a92 0700 0075  Nh1Nh2h.h.j....u
-0000c240: 6265 7562 6897 2981 72ce 0700 007d 72cf  beubh.).r....}r.
-0000c250: 0700 0028 681e 5881 0000 003a 636c 6173  ...(h.X....:clas
-0000c260: 733a 6073 6369 7079 5f6d 756c 7469 6d69  s:`scipy_multimi
-0000c270: 6e65 7860 2069 7320 6120 7772 6170 7065  nex` is a wrappe
-0000c280: 7220 666f 7220 7468 6520 6060 6d69 6e69  r for the ``mini
-0000c290: 6d69 7a65 6060 0a3a 6d6f 643a 6073 6369  mize``.:mod:`sci
-0000c2a0: 7079 6020 6675 6e63 7469 6f6e 2e20 4974  py` function. It
-0000c2b0: 2067 6976 6573 2061 6363 6573 7320 746f   gives access to
-0000c2c0: 206f 6e6c 7920 7061 7274 206f 6620 7468   only part of th
-0000c2d0: 6174 0a66 756e 6374 696f 6e2e 681f 6a76  at.function.h.jv
-0000c2e0: 0700 0068 236a 7d07 0000 6825 689a 6827  ...h#j}...h%h.h'
-0000c2f0: 7d72 d007 0000 2868 295d 682a 5d68 2b5d  }r....(h)]h*]h+]
-0000c300: 682c 5d68 2f5d 7568 314b 0768 3268 0268  h,]h/]uh1K.h2h.h
-0000c310: 335d 72d1 0700 0028 683c 2981 72d2 0700  3]r....(h<).r...
-0000c320: 007d 72d3 0700 0028 681e 5819 0000 003a  .}r....(h.X....:
-0000c330: 636c 6173 733a 6073 6369 7079 5f6d 756c  class:`scipy_mul
-0000c340: 7469 6d69 6e65 7860 72d4 0700 0068 1f6a  timinex`r....h.j
-0000c350: ce07 0000 6823 6a7d 0700 0068 2568 4068  ....h#j}...h%h@h
-0000c360: 277d 72d5 0700 0028 5507 7265 6674 7970  '}r....(U.reftyp
-0000c370: 6558 0500 0000 636c 6173 7368 4289 6843  eX....classhB.hC
-0000c380: 5810 0000 0073 6369 7079 5f6d 756c 7469  X....scipy_multi
-0000c390: 6d69 6e65 7855 0972 6566 646f 6d61 696e  minexU.refdomain
-0000c3a0: 5802 0000 0070 7972 d607 0000 682c 5d68  X....pyr....h,]h
-0000c3b0: 2b5d 550b 7265 6665 7870 6c69 6369 7489  +]U.refexplicit.
-0000c3c0: 6829 5d68 2a5d 682f 5d68 4568 4668 476a  h)]h*]h/]hEhFhGj
-0000c3d0: 2b07 0000 6848 6a28 0700 0075 6831 4b07  +...hHj(...uh1K.
-0000c3e0: 6833 5d72 d707 0000 684a 2981 72d8 0700  h3]r....hJ).r...
-0000c3f0: 007d 72d9 0700 0028 681e 6ad4 0700 0068  .}r....(h.j....h
-0000c400: 277d 72da 0700 0028 6829 5d68 2a5d 72db  '}r....(h)]h*]r.
-0000c410: 0700 0028 684f 6ad6 0700 0058 0800 0000  ...(hOj....X....
-0000c420: 7079 2d63 6c61 7373 72dc 0700 0065 682b  py-classr....eh+
-0000c430: 5d68 2c5d 682f 5d75 681f 6ad2 0700 0068  ]h,]h/]uh.j....h
-0000c440: 335d 72dd 0700 0068 5258 1000 0000 7363  3]r....hRX....sc
-0000c450: 6970 795f 6d75 6c74 696d 696e 6578 72de  ipy_multiminexr.
-0000c460: 0700 0085 8172 df07 0000 7d72 e007 0000  .....r....}r....
-0000c470: 2868 1e55 0068 1f6a d807 0000 7562 6168  (h.U.h.j....ubah
-0000c480: 2568 5675 6261 7562 6852 5816 0000 0020  %hVubaubhRX.... 
-0000c490: 6973 2061 2077 7261 7070 6572 2066 6f72  is a wrapper for
-0000c4a0: 2074 6865 2072 e107 0000 8581 72e2 0700   the r......r...
-0000c4b0: 007d 72e3 0700 0028 681e 5816 0000 0020  .}r....(h.X.... 
-0000c4c0: 6973 2061 2077 7261 7070 6572 2066 6f72  is a wrapper for
-0000c4d0: 2074 6865 2068 234e 6831 4e68 3268 0268   the h#Nh1Nh2h.h
-0000c4e0: 1f6a ce07 0000 7562 684a 2981 72e4 0700  .j....ubhJ).r...
-0000c4f0: 007d 72e5 0700 0028 681e 580c 0000 0060  .}r....(h.X....`
-0000c500: 606d 696e 696d 697a 6560 6068 277d 72e6  `minimize``h'}r.
-0000c510: 0700 0028 6829 5d68 2a5d 682b 5d68 2c5d  ...(h)]h*]h+]h,]
-0000c520: 682f 5d75 681f 6ace 0700 0068 335d 72e7  h/]uh.j....h3]r.
-0000c530: 0700 0068 5258 0800 0000 6d69 6e69 6d69  ...hRX....minimi
-0000c540: 7a65 72e8 0700 0085 8172 e907 0000 7d72  zer......r....}r
-0000c550: ea07 0000 2868 1e55 0068 1f6a e407 0000  ....(h.U.h.j....
-0000c560: 7562 6168 2568 5675 6268 5258 0100 0000  ubah%hVubhRX....
-0000c570: 0a85 8172 eb07 0000 7d72 ec07 0000 2868  ...r....}r....(h
-0000c580: 1e58 0100 0000 0a68 234e 6831 4e68 3268  .X.....h#Nh1Nh2h
-0000c590: 0268 1f6a ce07 0000 7562 683c 2981 72ed  .h.j....ubh<).r.
-0000c5a0: 0700 007d 72ee 0700 0028 681e 580c 0000  ...}r....(h.X...
-0000c5b0: 003a 6d6f 643a 6073 6369 7079 6072 ef07  .:mod:`scipy`r..
-0000c5c0: 0000 681f 6ace 0700 0068 236a 7d07 0000  ..h.j....h#j}...
-0000c5d0: 6825 6840 6827 7d72 f007 0000 2855 0772  h%h@h'}r....(U.r
-0000c5e0: 6566 7479 7065 5803 0000 006d 6f64 6842  eftypeX....modhB
-0000c5f0: 8968 4358 0500 0000 7363 6970 7955 0972  .hCX....scipyU.r
-0000c600: 6566 646f 6d61 696e 5802 0000 0070 7972  efdomainX....pyr
-0000c610: f107 0000 682c 5d68 2b5d 550b 7265 6665  ....h,]h+]U.refe
-0000c620: 7870 6c69 6369 7489 6829 5d68 2a5d 682f  xplicit.h)]h*]h/
-0000c630: 5d68 4568 4668 476a 2b07 0000 6848 6a28  ]hEhFhGj+...hHj(
-0000c640: 0700 0075 6831 4b07 6833 5d72 f207 0000  ...uh1K.h3]r....
-0000c650: 684a 2981 72f3 0700 007d 72f4 0700 0028  hJ).r....}r....(
-0000c660: 681e 6aef 0700 0068 277d 72f5 0700 0028  h.j....h'}r....(
-0000c670: 6829 5d68 2a5d 72f6 0700 0028 684f 6af1  h)]h*]r....(hOj.
-0000c680: 0700 0058 0600 0000 7079 2d6d 6f64 72f7  ...X....py-modr.
-0000c690: 0700 0065 682b 5d68 2c5d 682f 5d75 681f  ...eh+]h,]h/]uh.
-0000c6a0: 6aed 0700 0068 335d 72f8 0700 0068 5258  j....h3]r....hRX
-0000c6b0: 0500 0000 7363 6970 7972 f907 0000 8581  ....scipyr......
-0000c6c0: 72fa 0700 007d 72fb 0700 0028 681e 5500  r....}r....(h.U.
-0000c6d0: 681f 6af3 0700 0075 6261 6825 6856 7562  h.j....ubah%hVub
-0000c6e0: 6175 6268 5258 3900 0000 2066 756e 6374  aubhRX9... funct
-0000c6f0: 696f 6e2e 2049 7420 6769 7665 7320 6163  ion. It gives ac
-0000c700: 6365 7373 2074 6f20 6f6e 6c79 2070 6172  cess to only par
-0000c710: 7420 6f66 2074 6861 740a 6675 6e63 7469  t of that.functi
-0000c720: 6f6e 2e72 fc07 0000 8581 72fd 0700 007d  on.r......r....}
-0000c730: 72fe 0700 0028 681e 5839 0000 0020 6675  r....(h.X9... fu
-0000c740: 6e63 7469 6f6e 2e20 4974 2067 6976 6573  nction. It gives
-0000c750: 2061 6363 6573 7320 746f 206f 6e6c 7920   access to only 
-0000c760: 7061 7274 206f 6620 7468 6174 0a66 756e  part of that.fun
-0000c770: 6374 696f 6e2e 6823 4e68 314e 6832 6802  ction.h#Nh1Nh2h.
-0000c780: 681f 6ace 0700 0075 6265 7562 6ab6 0100  h.j....ubeubj...
-0000c790: 0029 8172 ff07 0000 7d72 0008 0000 2868  .).r....}r....(h
-0000c7a0: 1e55 0068 1f6a 7607 0000 6823 4e68 256a  .U.h.jv...h#Nh%j
-0000c7b0: b901 0000 6827 7d72 0108 0000 2868 295d  ....h'}r....(h)]
-0000c7c0: 682a 5d68 2b5d 682c 5d68 2f5d 7568 314e  h*]h+]h,]h/]uh1N
-0000c7d0: 6832 6802 6833 5d72 0208 0000 6abc 0100  h2h.h3]r....j...
-0000c7e0: 0029 8172 0308 0000 7d72 0408 0000 2868  .).r....}r....(h
-0000c7f0: 1e55 0068 277d 7205 0800 0028 6829 5d68  .U.h'}r....(h)]h
-0000c800: 2a5d 682b 5d68 2c5d 682f 5d75 681f 6aff  *]h+]h,]h/]uh.j.
-0000c810: 0700 0068 335d 7206 0800 0028 6ac1 0100  ...h3]r....(j...
-0000c820: 0029 8172 0708 0000 7d72 0808 0000 2868  .).r....}r....(h
-0000c830: 1e58 0a00 0000 5061 7261 6d65 7465 7273  .X....Parameters
-0000c840: 681f 6a03 0800 0068 236a 2407 0000 6825  h.j....h#j$...h%
-0000c850: 6ac4 0100 0068 277d 7209 0800 0028 6829  j....h'}r....(h)
-0000c860: 5d68 2a5d 682b 5d68 2c5d 682f 5d75 6831  ]h*]h+]h,]h/]uh1
-0000c870: 4b00 6833 5d72 0a08 0000 6852 580a 0000  K.h3]r....hRX...
-0000c880: 0050 6172 616d 6574 6572 7372 0b08 0000  .Parametersr....
-0000c890: 8581 720c 0800 007d 720d 0800 0028 681e  ..r....}r....(h.
-0000c8a0: 5500 681f 6a07 0800 0075 6261 7562 6aca  U.h.j....ubaubj.
-0000c8b0: 0100 0029 8172 0e08 0000 7d72 0f08 0000  ...).r....}r....
-0000c8c0: 2868 1e55 0068 277d 7210 0800 0028 6829  (h.U.h'}r....(h)
-0000c8d0: 5d68 2a5d 682b 5d68 2c5d 682f 5d75 681f  ]h*]h+]h,]h/]uh.
-0000c8e0: 6a03 0800 0068 335d 7211 0800 006a cf01  j....h3]r....j..
-0000c8f0: 0000 2981 7212 0800 007d 7213 0800 0028  ..).r....}r....(
-0000c900: 681e 5500 6827 7d72 1408 0000 2868 295d  h.U.h'}r....(h)]
-0000c910: 682a 5d68 2b5d 682c 5d68 2f5d 7568 1f6a  h*]h+]h,]h/]uh.j
-0000c920: 0e08 0000 6833 5d72 1508 0000 286a d401  ....h3]r....(j..
-0000c930: 0000 2981 7216 0800 007d 7217 0800 0028  ..).r....}r....(
-0000c940: 681e 5500 6827 7d72 1808 0000 2868 295d  h.U.h'}r....(h)]
-0000c950: 682a 5d68 2b5d 682c 5d68 2f5d 7568 1f6a  h*]h+]h,]h/]uh.j
-0000c960: 1208 0000 6833 5d72 1908 0000 6897 2981  ....h3]r....h.).
-0000c970: 721a 0800 007d 721b 0800 0028 681e 583f  r....}r....(h.X?
-0000c980: 0000 0078 3020 2861 7272 6179 206f 6620  ...x0 (array of 
-0000c990: 666c 6f61 7473 2920 2d2d 2053 7461 7274  floats) -- Start
-0000c9a0: 696e 6720 706f 696e 7420 666f 7220 6d69  ing point for mi
-0000c9b0: 6e69 6d69 7a61 7469 6f6e 2073 6561 7263  nimization searc
-0000c9c0: 682e 6827 7d72 1c08 0000 2868 295d 682a  h.h'}r....(h)]h*
-0000c9d0: 5d68 2b5d 682c 5d68 2f5d 7568 1f6a 1608  ]h+]h,]h/]uh.j..
-0000c9e0: 0000 6833 5d72 1d08 0000 286a dd01 0000  ..h3]r....(j....
-0000c9f0: 2981 721e 0800 007d 721f 0800 0028 681e  ).r....}r....(h.
-0000ca00: 5802 0000 0078 3068 277d 7220 0800 0028  X....x0h'}r ...(
-0000ca10: 682c 5d68 2b5d 6ae1 0100 0088 6829 5d68  h,]h+]j.....h)]h
-0000ca20: 2a5d 682f 5d75 681f 6a1a 0800 0068 335d  *]h/]uh.j....h3]
-0000ca30: 7221 0800 0068 5258 0200 0000 7830 7222  r!...hRX....x0r"
-0000ca40: 0800 0085 8172 2308 0000 7d72 2408 0000  .....r#...}r$...
-0000ca50: 2868 1e55 0068 1f6a 1e08 0000 7562 6168  (h.U.h.j....ubah
-0000ca60: 256a e601 0000 7562 6852 5802 0000 0020  %j....ubhRX.... 
-0000ca70: 2872 2508 0000 8581 7226 0800 007d 7227  (r%.....r&...}r'
-0000ca80: 0800 0028 681e 5500 681f 6a1a 0800 0075  ...(h.U.h.j....u
-0000ca90: 6268 3c29 8172 2808 0000 7d72 2908 0000  bh<).r(...}r)...
-0000caa0: 2868 1e55 0068 277d 722a 0800 0028 5507  (h.U.h'}r*...(U.
-0000cab0: 7265 6674 7970 6568 f26a e101 0000 8855  reftypeh.j.....U
-0000cac0: 0972 6566 7461 7267 6574 580f 0000 0061  .reftargetX....a
-0000cad0: 7272 6179 206f 6620 666c 6f61 7473 722b  rray of floatsr+
-0000cae0: 0800 0055 0972 6566 646f 6d61 696e 6a1f  ...U.refdomainj.
-0000caf0: 0700 0068 2c5d 682b 5d55 0b72 6566 6578  ...h,]h+]U.refex
-0000cb00: 706c 6963 6974 8968 295d 682a 5d68 2f5d  plicit.h)]h*]h/]
-0000cb10: 7568 1f6a 1a08 0000 6833 5d72 2c08 0000  uh.j....h3]r,...
-0000cb20: 6aef 0100 0029 8172 2d08 0000 7d72 2e08  j....).r-...}r..
-0000cb30: 0000 2868 1e6a 2b08 0000 6827 7d72 2f08  ..(h.j+...h'}r/.
-0000cb40: 0000 2868 295d 682a 5d68 2b5d 682c 5d68  ..(h)]h*]h+]h,]h
-0000cb50: 2f5d 7568 1f6a 2808 0000 6833 5d72 3008  /]uh.j(...h3]r0.
-0000cb60: 0000 6852 580f 0000 0061 7272 6179 206f  ..hRX....array o
-0000cb70: 6620 666c 6f61 7473 7231 0800 0085 8172  f floatsr1.....r
-0000cb80: 3208 0000 7d72 3308 0000 2868 1e55 0068  2...}r3...(h.U.h
-0000cb90: 1f6a 2d08 0000 7562 6168 256a f701 0000  .j-...ubah%j....
-0000cba0: 7562 6168 2568 4075 6268 5258 0100 0000  ubah%h@ubhRX....
-0000cbb0: 2985 8172 3408 0000 7d72 3508 0000 2868  )..r4...}r5...(h
-0000cbc0: 1e55 0068 1f6a 1a08 0000 7562 6852 5805  .U.h.j....ubhRX.
-0000cbd0: 0000 0020 e280 9320 7236 0800 0085 8172  ... ... r6.....r
-0000cbe0: 3708 0000 7d72 3808 0000 2868 1e55 0068  7...}r8...(h.U.h
-0000cbf0: 1f6a 1a08 0000 7562 6852 5827 0000 0053  .j....ubhRX'...S
-0000cc00: 7461 7274 696e 6720 706f 696e 7420 666f  tarting point fo
-0000cc10: 7220 6d69 6e69 6d69 7a61 7469 6f6e 2073  r minimization s
-0000cc20: 6561 7263 682e 7239 0800 0085 8172 3a08  earch.r9.....r:.
-0000cc30: 0000 7d72 3b08 0000 2868 1e58 2700 0000  ..}r;...(h.X'...
-0000cc40: 5374 6172 7469 6e67 2070 6f69 6e74 2066  Starting point f
-0000cc50: 6f72 206d 696e 696d 697a 6174 696f 6e20  or minimization 
-0000cc60: 7365 6172 6368 2e72 3c08 0000 6823 4e68  search.r<...h#Nh
-0000cc70: 314e 6832 6802 681f 6a1a 0800 0075 6265  1Nh2h.h.j....ube
-0000cc80: 6825 689a 7562 6168 256a 0102 0000 7562  h%h.ubah%j....ub
-0000cc90: 6ad4 0100 0029 8172 3d08 0000 7d72 3e08  j....).r=...}r>.
-0000cca0: 0000 2868 1e55 0068 277d 723f 0800 0028  ..(h.U.h'}r?...(
-0000ccb0: 6829 5d68 2a5d 682b 5d68 2c5d 682f 5d75  h)]h*]h+]h,]h/]u
-0000ccc0: 681f 6a12 0800 0068 335d 7240 0800 0068  h.j....h3]r@...h
-0000ccd0: 9729 8172 4108 0000 7d72 4208 0000 2868  .).rA...}rB...(h
-0000cce0: 1e58 3700 0000 6620 2d2d 2046 756e 6374  .X7...f -- Funct
-0000ccf0: 696f 6e20 6628 7829 2074 6f20 6265 206d  ion f(x) to be m
-0000cd00: 696e 696d 697a 6564 2062 7920 7661 7279  inimized by vary
-0000cd10: 696e 6720 7665 6374 6f72 2078 2e68 277d  ing vector x.h'}
-0000cd20: 7243 0800 0028 6829 5d68 2a5d 682b 5d68  rC...(h)]h*]h+]h
-0000cd30: 2c5d 682f 5d75 681f 6a3d 0800 0068 335d  ,]h/]uh.j=...h3]
-0000cd40: 7244 0800 0028 6add 0100 0029 8172 4508  rD...(j....).rE.
-0000cd50: 0000 7d72 4608 0000 2868 1e58 0100 0000  ..}rF...(h.X....
-0000cd60: 6668 277d 7247 0800 0028 682c 5d68 2b5d  fh'}rG...(h,]h+]
-0000cd70: 6ae1 0100 0088 6829 5d68 2a5d 682f 5d75  j.....h)]h*]h/]u
-0000cd80: 681f 6a41 0800 0068 335d 7248 0800 0068  h.jA...h3]rH...h
-0000cd90: 5258 0100 0000 6685 8172 4908 0000 7d72  RX....f..rI...}r
-0000cda0: 4a08 0000 2868 1e55 0068 1f6a 4508 0000  J...(h.U.h.jE...
-0000cdb0: 7562 6168 256a e601 0000 7562 6852 5805  ubah%j....ubhRX.
-0000cdc0: 0000 0020 e280 9320 724b 0800 0085 8172  ... ... rK.....r
-0000cdd0: 4c08 0000 7d72 4d08 0000 2868 1e55 0068  L...}rM...(h.U.h
-0000cde0: 1f6a 4108 0000 7562 6852 5809 0000 0046  .jA...ubhRX....F
-0000cdf0: 756e 6374 696f 6e20 724e 0800 0085 8172  unction rN.....r
-0000ce00: 4f08 0000 7d72 5008 0000 2868 1e58 0900  O...}rP...(h.X..
-0000ce10: 0000 4675 6e63 7469 6f6e 2072 5108 0000  ..Function rQ...
-0000ce20: 6823 4e68 314e 6832 6802 681f 6a41 0800  h#Nh1Nh2h.h.jA..
-0000ce30: 0075 6268 4a29 8172 5208 0000 7d72 5308  .ubhJ).rR...}rS.
-0000ce40: 0000 2868 1e58 0800 0000 6060 6628 7829  ..(h.X....``f(x)
-0000ce50: 6060 681f 6a41 0800 0068 234e 6825 6856  ``h.jA...h#Nh%hV
-0000ce60: 6827 7d72 5408 0000 2868 295d 682a 5d68  h'}rT...(h)]h*]h
-0000ce70: 2b5d 682c 5d68 2f5d 7568 314e 6832 6802  +]h,]h/]uh1Nh2h.
-0000ce80: 6833 5d72 5508 0000 6852 5804 0000 0066  h3]rU...hRX....f
-0000ce90: 2878 2972 5608 0000 8581 7257 0800 007d  (x)rV.....rW...}
-0000cea0: 7258 0800 0028 681e 5500 6823 4e68 314e  rX...(h.U.h#Nh1N
-0000ceb0: 6832 6802 681f 6a52 0800 0075 6261 7562  h2h.h.jR...ubaub
-0000cec0: 6852 5823 0000 0020 746f 2062 6520 6d69  hRX#... to be mi
-0000ced0: 6e69 6d69 7a65 6420 6279 2076 6172 7969  nimized by varyi
-0000cee0: 6e67 2076 6563 746f 7220 7259 0800 0085  ng vector rY....
-0000cef0: 8172 5a08 0000 7d72 5b08 0000 2868 1e58  .rZ...}r[...(h.X
-0000cf00: 2300 0000 2074 6f20 6265 206d 696e 696d  #... to be minim
-0000cf10: 697a 6564 2062 7920 7661 7279 696e 6720  ized by varying 
-0000cf20: 7665 6374 6f72 2072 5c08 0000 6823 4e68  vector r\...h#Nh
-0000cf30: 314e 6832 6802 681f 6a41 0800 0075 6268  1Nh2h.h.jA...ubh
-0000cf40: 4a29 8172 5d08 0000 7d72 5e08 0000 2868  J).r]...}r^...(h
-0000cf50: 1e58 0500 0000 6060 7860 6068 1f6a 4108  .X....``x``h.jA.
-0000cf60: 0000 6823 4e68 2568 5668 277d 725f 0800  ..h#Nh%hVh'}r_..
-0000cf70: 0028 6829 5d68 2a5d 682b 5d68 2c5d 682f  .(h)]h*]h+]h,]h/
-0000cf80: 5d75 6831 4e68 3268 0268 335d 7260 0800  ]uh1Nh2h.h3]r`..
-0000cf90: 0068 5258 0100 0000 7885 8172 6108 0000  .hRX....x..ra...
-0000cfa0: 7d72 6208 0000 2868 1e55 0068 234e 6831  }rb...(h.U.h#Nh1
-0000cfb0: 4e68 3268 0268 1f6a 5d08 0000 7562 6175  Nh2h.h.j]...ubau
-0000cfc0: 6268 5258 0100 0000 2e85 8172 6308 0000  bhRX.......rc...
-0000cfd0: 7d72 6408 0000 2868 1e58 0100 0000 2e68  }rd...(h.X.....h
-0000cfe0: 234e 6831 4e68 3268 0268 1f6a 4108 0000  #Nh1Nh2h.h.jA...
-0000cff0: 7562 6568 2568 9a75 6261 6825 6a01 0200  ubeh%h.ubah%j...
-0000d000: 0075 626a d401 0000 2981 7265 0800 007d  .ubj....).re...}
-0000d010: 7266 0800 0028 681e 5500 6827 7d72 6708  rf...(h.U.h'}rg.
-0000d020: 0000 2868 295d 682a 5d68 2b5d 682c 5d68  ..(h)]h*]h+]h,]h
-0000d030: 2f5d 7568 1f6a 1208 0000 6833 5d72 6808  /]uh.j....h3]rh.
-0000d040: 0000 6897 2981 7269 0800 007d 726a 0800  ..h.).ri...}rj..
-0000d050: 0028 681e 585e 0000 0074 6f6c 2028 666c  .(h.X^...tol (fl
-0000d060: 6f61 7429 202d 2d20 4d69 6e69 6d69 7a61  oat) -- Minimiza
-0000d070: 7469 6f6e 2073 746f 7073 2077 6865 6e20  tion stops when 
-0000d080: 7820 6861 7320 636f 6e76 6572 6765 6420  x has converged 
-0000d090: 746f 2077 6974 680a 746f 6c65 7261 6e63  to with.toleranc
-0000d0a0: 6520 746f 6c3b 2064 6566 6175 6c74 2069  e tol; default i
-0000d0b0: 7320 3165 2d34 2e68 277d 726b 0800 0028  s 1e-4.h'}rk...(
-0000d0c0: 6829 5d68 2a5d 682b 5d68 2c5d 682f 5d75  h)]h*]h+]h,]h/]u
-0000d0d0: 681f 6a65 0800 0068 335d 726c 0800 0028  h.je...h3]rl...(
-0000d0e0: 6add 0100 0029 8172 6d08 0000 7d72 6e08  j....).rm...}rn.
-0000d0f0: 0000 2868 1e58 0300 0000 746f 6c68 277d  ..(h.X....tolh'}
-0000d100: 726f 0800 0028 682c 5d68 2b5d 6ae1 0100  ro...(h,]h+]j...
-0000d110: 0088 6829 5d68 2a5d 682f 5d75 681f 6a69  ..h)]h*]h/]uh.ji
-0000d120: 0800 0068 335d 7270 0800 0068 5258 0300  ...h3]rp...hRX..
-0000d130: 0000 746f 6c72 7108 0000 8581 7272 0800  ..tolrq.....rr..
-0000d140: 007d 7273 0800 0028 681e 5500 681f 6a6d  .}rs...(h.U.h.jm
-0000d150: 0800 0075 6261 6825 6ae6 0100 0075 6268  ...ubah%j....ubh
-0000d160: 5258 0200 0000 2028 7274 0800 0085 8172  RX.... (rt.....r
-0000d170: 7508 0000 7d72 7608 0000 2868 1e55 0068  u...}rv...(h.U.h
-0000d180: 1f6a 6908 0000 7562 683c 2981 7277 0800  .ji...ubh<).rw..
-0000d190: 007d 7278 0800 0028 681e 5500 6827 7d72  .}rx...(h.U.h'}r
-0000d1a0: 7908 0000 2855 0772 6566 7479 7065 68f2  y...(U.reftypeh.
-0000d1b0: 6ae1 0100 0088 5509 7265 6674 6172 6765  j.....U.reftarge
-0000d1c0: 7458 0500 0000 666c 6f61 7472 7a08 0000  tX....floatrz...
-0000d1d0: 5509 7265 6664 6f6d 6169 6e6a 1f07 0000  U.refdomainj....
-0000d1e0: 682c 5d68 2b5d 550b 7265 6665 7870 6c69  h,]h+]U.refexpli
-0000d1f0: 6369 7489 6829 5d68 2a5d 682f 5d75 681f  cit.h)]h*]h/]uh.
-0000d200: 6a69 0800 0068 335d 727b 0800 006a ef01  ji...h3]r{...j..
-0000d210: 0000 2981 727c 0800 007d 727d 0800 0028  ..).r|...}r}...(
-0000d220: 681e 6a7a 0800 0068 277d 727e 0800 0028  h.jz...h'}r~...(
-0000d230: 6829 5d68 2a5d 682b 5d68 2c5d 682f 5d75  h)]h*]h+]h,]h/]u
-0000d240: 681f 6a77 0800 0068 335d 727f 0800 0068  h.jw...h3]r....h
-0000d250: 5258 0500 0000 666c 6f61 7472 8008 0000  RX....floatr....
-0000d260: 8581 7281 0800 007d 7282 0800 0028 681e  ..r....}r....(h.
-0000d270: 5500 681f 6a7c 0800 0075 6261 6825 6af7  U.h.j|...ubah%j.
-0000d280: 0100 0075 6261 6825 6840 7562 6852 5801  ...ubah%h@ubhRX.
-0000d290: 0000 0029 8581 7283 0800 007d 7284 0800  ...)..r....}r...
-0000d2a0: 0028 681e 5500 681f 6a69 0800 0075 6268  .(h.U.h.ji...ubh
-0000d2b0: 5258 0500 0000 20e2 8093 2072 8508 0000  RX.... ... r....
-0000d2c0: 8581 7286 0800 007d 7287 0800 0028 681e  ..r....}r....(h.
-0000d2d0: 5500 681f 6a69 0800 0075 6268 5258 1800  U.h.ji...ubhRX..
-0000d2e0: 0000 4d69 6e69 6d69 7a61 7469 6f6e 2073  ..Minimization s
-0000d2f0: 746f 7073 2077 6865 6e20 7288 0800 0085  tops when r.....
-0000d300: 8172 8908 0000 7d72 8a08 0000 2868 1e58  .r....}r....(h.X
-0000d310: 1800 0000 4d69 6e69 6d69 7a61 7469 6f6e  ....Minimization
-0000d320: 2073 746f 7073 2077 6865 6e20 728b 0800   stops when r...
-0000d330: 0068 234e 6831 4e68 3268 0268 1f6a 6908  .h#Nh1Nh2h.h.ji.
-0000d340: 0000 7562 684a 2981 728c 0800 007d 728d  ..ubhJ).r....}r.
-0000d350: 0800 0028 681e 5805 0000 0060 6078 6060  ...(h.X....``x``
-0000d360: 681f 6a69 0800 0068 234e 6825 6856 6827  h.ji...h#Nh%hVh'
-0000d370: 7d72 8e08 0000 2868 295d 682a 5d68 2b5d  }r....(h)]h*]h+]
-0000d380: 682c 5d68 2f5d 7568 314e 6832 6802 6833  h,]h/]uh1Nh2h.h3
-0000d390: 5d72 8f08 0000 6852 5801 0000 0078 8581  ]r....hRX....x..
-0000d3a0: 7290 0800 007d 7291 0800 0028 681e 5500  r....}r....(h.U.
-0000d3b0: 6823 4e68 314e 6832 6802 681f 6a8c 0800  h#Nh1Nh2h.h.j...
-0000d3c0: 0075 6261 7562 6852 5821 0000 0020 6861  .ubaubhRX!... ha
-0000d3d0: 7320 636f 6e76 6572 6765 6420 746f 2077  s converged to w
-0000d3e0: 6974 680a 746f 6c65 7261 6e63 6520 7292  ith.tolerance r.
-0000d3f0: 0800 0085 8172 9308 0000 7d72 9408 0000  .....r....}r....
-0000d400: 2868 1e58 2100 0000 2068 6173 2063 6f6e  (h.X!... has con
-0000d410: 7665 7267 6564 2074 6f20 7769 7468 0a74  verged to with.t
-0000d420: 6f6c 6572 616e 6365 2072 9508 0000 6823  olerance r....h#
-0000d430: 4e68 314e 6832 6802 681f 6a69 0800 0075  Nh1Nh2h.h.ji...u
-0000d440: 6268 4a29 8172 9608 0000 7d72 9708 0000  bhJ).r....}r....
-0000d450: 2868 1e58 0700 0000 6060 746f 6c60 6068  (h.X....``tol``h
-0000d460: 1f6a 6908 0000 6823 4e68 2568 5668 277d  .ji...h#Nh%hVh'}
-0000d470: 7298 0800 0028 6829 5d68 2a5d 682b 5d68  r....(h)]h*]h+]h
-0000d480: 2c5d 682f 5d75 6831 4e68 3268 0268 335d  ,]h/]uh1Nh2h.h3]
-0000d490: 7299 0800 0068 5258 0300 0000 746f 6c72  r....hRX....tolr
-0000d4a0: 9a08 0000 8581 729b 0800 007d 729c 0800  ......r....}r...
-0000d4b0: 0028 681e 5500 6823 4e68 314e 6832 6802  .(h.U.h#Nh1Nh2h.
-0000d4c0: 681f 6a96 0800 0075 6261 7562 6852 580d  h.j....ubaubhRX.
-0000d4d0: 0000 003b 2064 6566 6175 6c74 2069 7320  ...; default is 
-0000d4e0: 729d 0800 0085 8172 9e08 0000 7d72 9f08  r......r....}r..
-0000d4f0: 0000 2868 1e58 0d00 0000 3b20 6465 6661  ..(h.X....; defa
-0000d500: 756c 7420 6973 2072 a008 0000 6823 4e68  ult is r....h#Nh
-0000d510: 314e 6832 6802 681f 6a69 0800 0075 6268  1Nh2h.h.ji...ubh
-0000d520: 4a29 8172 a108 0000 7d72 a208 0000 2868  J).r....}r....(h
-0000d530: 1e58 0800 0000 6060 3165 2d34 6060 681f  .X....``1e-4``h.
-0000d540: 6a69 0800 0068 234e 6825 6856 6827 7d72  ji...h#Nh%hVh'}r
-0000d550: a308 0000 2868 295d 682a 5d68 2b5d 682c  ....(h)]h*]h+]h,
-0000d560: 5d68 2f5d 7568 314e 6832 6802 6833 5d72  ]h/]uh1Nh2h.h3]r
-0000d570: a408 0000 6852 5804 0000 0031 652d 3472  ....hRX....1e-4r
-0000d580: a508 0000 8581 72a6 0800 007d 72a7 0800  ......r....}r...
-0000d590: 0028 681e 5500 6823 4e68 314e 6832 6802  .(h.U.h#Nh1Nh2h.
-0000d5a0: 681f 6aa1 0800 0075 6261 7562 6852 5801  h.j....ubaubhRX.
-0000d5b0: 0000 002e 8581 72a8 0800 007d 72a9 0800  ......r....}r...
-0000d5c0: 0028 681e 5801 0000 002e 6823 4e68 314e  .(h.X.....h#Nh1N
-0000d5d0: 6832 6802 681f 6a69 0800 0075 6265 6825  h2h.h.ji...ubeh%
-0000d5e0: 689a 7562 6168 256a 0102 0000 7562 6ad4  h.ubah%j....ubj.
-0000d5f0: 0100 0029 8172 aa08 0000 7d72 ab08 0000  ...).r....}r....
-0000d600: 2868 1e55 0068 277d 72ac 0800 0028 6829  (h.U.h'}r....(h)
-0000d610: 5d68 2a5d 682b 5d68 2c5d 682f 5d75 681f  ]h*]h+]h,]h/]uh.
-0000d620: 6a12 0800 0068 335d 72ad 0800 0068 9729  j....h3]r....h.)
-0000d630: 8172 ae08 0000 7d72 af08 0000 2868 1e58  .r....}r....(h.X
-0000d640: 5c00 0000 6d61 7869 7420 2870 6f73 6974  \...maxit (posit
-0000d650: 6976 6520 696e 7429 202d 2d20 4d61 7869  ive int) -- Maxi
-0000d660: 6d75 6d20 6e75 6d62 6572 206f 6620 6974  mum number of it
-0000d670: 6572 6174 696f 6e73 2069 6e20 7365 6172  erations in sear
-0000d680: 6368 2066 6f72 206d 696e 696d 756d 3b0a  ch for minimum;.
-0000d690: 6465 6661 756c 7420 6973 2031 3030 302e  default is 1000.
-0000d6a0: 6827 7d72 b008 0000 2868 295d 682a 5d68  h'}r....(h)]h*]h
-0000d6b0: 2b5d 682c 5d68 2f5d 7568 1f6a aa08 0000  +]h,]h/]uh.j....
-0000d6c0: 6833 5d72 b108 0000 286a dd01 0000 2981  h3]r....(j....).
-0000d6d0: 72b2 0800 007d 72b3 0800 0028 681e 5805  r....}r....(h.X.
-0000d6e0: 0000 006d 6178 6974 6827 7d72 b408 0000  ...maxith'}r....
-0000d6f0: 2868 2c5d 682b 5d6a e101 0000 8868 295d  (h,]h+]j.....h)]
-0000d700: 682a 5d68 2f5d 7568 1f6a ae08 0000 6833  h*]h/]uh.j....h3
-0000d710: 5d72 b508 0000 6852 5805 0000 006d 6178  ]r....hRX....max
-0000d720: 6974 72b6 0800 0085 8172 b708 0000 7d72  itr......r....}r
-0000d730: b808 0000 2868 1e55 0068 1f6a b208 0000  ....(h.U.h.j....
-0000d740: 7562 6168 256a e601 0000 7562 6852 5802  ubah%j....ubhRX.
-0000d750: 0000 0020 2872 b908 0000 8581 72ba 0800  ... (r......r...
-0000d760: 007d 72bb 0800 0028 681e 5500 681f 6aae  .}r....(h.U.h.j.
-0000d770: 0800 0075 6268 3c29 8172 bc08 0000 7d72  ...ubh<).r....}r
-0000d780: bd08 0000 2868 1e55 0068 277d 72be 0800  ....(h.U.h'}r...
-0000d790: 0028 5507 7265 6674 7970 6568 f26a e101  .(U.reftypeh.j..
-0000d7a0: 0000 8855 0972 6566 7461 7267 6574 580c  ...U.reftargetX.
-0000d7b0: 0000 0070 6f73 6974 6976 6520 696e 7472  ...positive intr
-0000d7c0: bf08 0000 5509 7265 6664 6f6d 6169 6e6a  ....U.refdomainj
-0000d7d0: 1f07 0000 682c 5d68 2b5d 550b 7265 6665  ....h,]h+]U.refe
-0000d7e0: 7870 6c69 6369 7489 6829 5d68 2a5d 682f  xplicit.h)]h*]h/
-0000d7f0: 5d75 681f 6aae 0800 0068 335d 72c0 0800  ]uh.j....h3]r...
-0000d800: 006a ef01 0000 2981 72c1 0800 007d 72c2  .j....).r....}r.
-0000d810: 0800 0028 681e 6abf 0800 0068 277d 72c3  ...(h.j....h'}r.
-0000d820: 0800 0028 6829 5d68 2a5d 682b 5d68 2c5d  ...(h)]h*]h+]h,]
-0000d830: 682f 5d75 681f 6abc 0800 0068 335d 72c4  h/]uh.j....h3]r.
-0000d840: 0800 0068 5258 0c00 0000 706f 7369 7469  ...hRX....positi
-0000d850: 7665 2069 6e74 72c5 0800 0085 8172 c608  ve intr......r..
-0000d860: 0000 7d72 c708 0000 2868 1e55 0068 1f6a  ..}r....(h.U.h.j
-0000d870: c108 0000 7562 6168 256a f701 0000 7562  ....ubah%j....ub
-0000d880: 6168 2568 4075 6268 5258 0100 0000 2985  ah%h@ubhRX....).
-0000d890: 8172 c808 0000 7d72 c908 0000 2868 1e55  .r....}r....(h.U
-0000d8a0: 0068 1f6a ae08 0000 7562 6852 5805 0000  .h.j....ubhRX...
-0000d8b0: 0020 e280 9320 72ca 0800 0085 8172 cb08  . ... r......r..
-0000d8c0: 0000 7d72 cc08 0000 2868 1e55 0068 1f6a  ..}r....(h.U.h.j
-0000d8d0: ae08 0000 7562 6852 5844 0000 004d 6178  ....ubhRXD...Max
-0000d8e0: 696d 756d 206e 756d 6265 7220 6f66 2069  imum number of i
-0000d8f0: 7465 7261 7469 6f6e 7320 696e 2073 6561  terations in sea
-0000d900: 7263 6820 666f 7220 6d69 6e69 6d75 6d3b  rch for minimum;
-0000d910: 0a64 6566 6175 6c74 2069 7320 3130 3030  .default is 1000
-0000d920: 2e72 cd08 0000 8581 72ce 0800 007d 72cf  .r......r....}r.
-0000d930: 0800 0028 681e 5844 0000 004d 6178 696d  ...(h.XD...Maxim
-0000d940: 756d 206e 756d 6265 7220 6f66 2069 7465  um number of ite
-0000d950: 7261 7469 6f6e 7320 696e 2073 6561 7263  rations in searc
-0000d960: 6820 666f 7220 6d69 6e69 6d75 6d3b 0a64  h for minimum;.d
-0000d970: 6566 6175 6c74 2069 7320 3130 3030 2e72  efault is 1000.r
-0000d980: d008 0000 6823 4e68 314e 6832 6802 681f  ....h#Nh1Nh2h.h.
-0000d990: 6aae 0800 0075 6265 6825 689a 7562 6168  j....ubeh%h.ubah
-0000d9a0: 256a 0102 0000 7562 6ad4 0100 0029 8172  %j....ubj....).r
-0000d9b0: d108 0000 7d72 d208 0000 2868 1e55 0068  ....}r....(h.U.h
-0000d9c0: 277d 72d3 0800 0028 6829 5d68 2a5d 682b  '}r....(h)]h*]h+
-0000d9d0: 5d68 2c5d 682f 5d75 681f 6a12 0800 0068  ]h,]h/]uh.j....h
-0000d9e0: 335d 72d4 0800 0068 9729 8172 d508 0000  3]r....h.).r....
-0000d9f0: 7d72 d608 0000 2868 1e58 8900 0000 616e  }r....(h.X....an
-0000da00: 616c 797a 6572 2028 6675 6e63 7469 6f6e  alyzer (function
-0000da10: 2920 2d2d 204f 7074 696f 6e61 6c20 6675  ) -- Optional fu
-0000da20: 6e63 7469 6f6e 206f 6620 7468 6520 6375  nction of the cu
-0000da30: 7272 656e 7420 782e 0a54 6869 7320 6361  rrent x..This ca
-0000da40: 6e20 6265 2075 7365 6420 746f 2069 6e73  n be used to ins
-0000da50: 7065 6374 2069 6e74 6572 6d65 6469 6174  pect intermediat
-0000da60: 6520 7374 6570 7320 696e 2074 6865 0a6d  e steps in the.m
-0000da70: 696e 696d 697a 6174 696f 6e2c 2069 6620  inimization, if 
-0000da80: 6e65 6564 6564 2e68 277d 72d7 0800 0028  needed.h'}r....(
-0000da90: 6829 5d68 2a5d 682b 5d68 2c5d 682f 5d75  h)]h*]h+]h,]h/]u
-0000daa0: 681f 6ad1 0800 0068 335d 72d8 0800 0028  h.j....h3]r....(
-0000dab0: 6add 0100 0029 8172 d908 0000 7d72 da08  j....).r....}r..
-0000dac0: 0000 2868 1e58 0800 0000 616e 616c 797a  ..(h.X....analyz
-0000dad0: 6572 6827 7d72 db08 0000 2868 2c5d 682b  erh'}r....(h,]h+
-0000dae0: 5d6a e101 0000 8868 295d 682a 5d68 2f5d  ]j.....h)]h*]h/]
-0000daf0: 7568 1f6a d508 0000 6833 5d72 dc08 0000  uh.j....h3]r....
-0000db00: 6852 5808 0000 0061 6e61 6c79 7a65 7272  hRX....analyzerr
-0000db10: dd08 0000 8581 72de 0800 007d 72df 0800  ......r....}r...
-0000db20: 0028 681e 5500 681f 6ad9 0800 0075 6261  .(h.U.h.j....uba
-0000db30: 6825 6ae6 0100 0075 6268 5258 0200 0000  h%j....ubhRX....
-0000db40: 2028 72e0 0800 0085 8172 e108 0000 7d72   (r......r....}r
-0000db50: e208 0000 2868 1e55 0068 1f6a d508 0000  ....(h.U.h.j....
-0000db60: 7562 683c 2981 72e3 0800 007d 72e4 0800  ubh<).r....}r...
-0000db70: 0028 681e 5500 6827 7d72 e508 0000 2855  .(h.U.h'}r....(U
-0000db80: 0772 6566 7479 7065 68f2 6ae1 0100 0088  .reftypeh.j.....
-0000db90: 5509 7265 6674 6172 6765 7458 0800 0000  U.reftargetX....
-0000dba0: 6675 6e63 7469 6f6e 72e6 0800 0055 0972  functionr....U.r
-0000dbb0: 6566 646f 6d61 696e 6a1f 0700 0068 2c5d  efdomainj....h,]
-0000dbc0: 682b 5d55 0b72 6566 6578 706c 6963 6974  h+]U.refexplicit
-0000dbd0: 8968 295d 682a 5d68 2f5d 7568 1f6a d508  .h)]h*]h/]uh.j..
-0000dbe0: 0000 6833 5d72 e708 0000 6aef 0100 0029  ..h3]r....j....)
-0000dbf0: 8172 e808 0000 7d72 e908 0000 2868 1e6a  .r....}r....(h.j
-0000dc00: e608 0000 6827 7d72 ea08 0000 2868 295d  ....h'}r....(h)]
-0000dc10: 682a 5d68 2b5d 682c 5d68 2f5d 7568 1f6a  h*]h+]h,]h/]uh.j
-0000dc20: e308 0000 6833 5d72 eb08 0000 6852 5808  ....h3]r....hRX.
-0000dc30: 0000 0066 756e 6374 696f 6e72 ec08 0000  ...functionr....
-0000dc40: 8581 72ed 0800 007d 72ee 0800 0028 681e  ..r....}r....(h.
-0000dc50: 5500 681f 6ae8 0800 0075 6261 6825 6af7  U.h.j....ubah%j.
-0000dc60: 0100 0075 6261 6825 6840 7562 6852 5801  ...ubah%h@ubhRX.
-0000dc70: 0000 0029 8581 72ef 0800 007d 72f0 0800  ...)..r....}r...
-0000dc80: 0028 681e 5500 681f 6ad5 0800 0075 6268  .(h.U.h.j....ubh
-0000dc90: 5258 0500 0000 20e2 8093 2072 f108 0000  RX.... ... r....
-0000dca0: 8581 72f2 0800 007d 72f3 0800 0028 681e  ..r....}r....(h.
-0000dcb0: 5500 681f 6ad5 0800 0075 6268 5258 2100  U.h.j....ubhRX!.
-0000dcc0: 0000 4f70 7469 6f6e 616c 2066 756e 6374  ..Optional funct
-0000dcd0: 696f 6e20 6f66 2074 6865 2063 7572 7265  ion of the curre
-0000dce0: 6e74 2072 f408 0000 8581 72f5 0800 007d  nt r......r....}
-0000dcf0: 72f6 0800 0028 681e 5821 0000 004f 7074  r....(h.X!...Opt
-0000dd00: 696f 6e61 6c20 6675 6e63 7469 6f6e 206f  ional function o
-0000dd10: 6620 7468 6520 6375 7272 656e 7420 72f7  f the current r.
-0000dd20: 0800 0068 234e 6831 4e68 3268 0268 1f6a  ...h#Nh1Nh2h.h.j
-0000dd30: d508 0000 7562 684a 2981 72f8 0800 007d  ....ubhJ).r....}
-0000dd40: 72f9 0800 0028 681e 5805 0000 0060 6078  r....(h.X....``x
-0000dd50: 6060 681f 6ad5 0800 0068 234e 6825 6856  ``h.j....h#Nh%hV
-0000dd60: 6827 7d72 fa08 0000 2868 295d 682a 5d68  h'}r....(h)]h*]h
-0000dd70: 2b5d 682c 5d68 2f5d 7568 314e 6832 6802  +]h,]h/]uh1Nh2h.
-0000dd80: 6833 5d72 fb08 0000 6852 5801 0000 0078  h3]r....hRX....x
-0000dd90: 8581 72fc 0800 007d 72fd 0800 0028 681e  ..r....}r....(h.
-0000dda0: 5500 6823 4e68 314e 6832 6802 681f 6af8  U.h#Nh1Nh2h.h.j.
-0000ddb0: 0800 0075 6261 7562 6852 5850 0000 002e  ...ubaubhRXP....
-0000ddc0: 0a54 6869 7320 6361 6e20 6265 2075 7365  .This can be use
-0000ddd0: 6420 746f 2069 6e73 7065 6374 2069 6e74  d to inspect int
-0000dde0: 6572 6d65 6469 6174 6520 7374 6570 7320  ermediate steps 
-0000ddf0: 696e 2074 6865 0a6d 696e 696d 697a 6174  in the.minimizat
-0000de00: 696f 6e2c 2069 6620 6e65 6564 6564 2e72  ion, if needed.r
-0000de10: fe08 0000 8581 72ff 0800 007d 7200 0900  ......r....}r...
-0000de20: 0028 681e 5850 0000 002e 0a54 6869 7320  .(h.XP.....This 
-0000de30: 6361 6e20 6265 2075 7365 6420 746f 2069  can be used to i
-0000de40: 6e73 7065 6374 2069 6e74 6572 6d65 6469  nspect intermedi
-0000de50: 6174 6520 7374 6570 7320 696e 2074 6865  ate steps in the
-0000de60: 0a6d 696e 696d 697a 6174 696f 6e2c 2069  .minimization, i
-0000de70: 6620 6e65 6564 6564 2e72 0109 0000 6823  f needed.r....h#
-0000de80: 4e68 314e 6832 6802 681f 6ad5 0800 0075  Nh1Nh2h.h.j....u
-0000de90: 6265 6825 689a 7562 6168 256a 0102 0000  beh%h.ubah%j....
-0000dea0: 7562 6568 256a 6d04 0000 7562 6168 256a  ubeh%jm...ubah%j
-0000deb0: 6e04 0000 7562 6568 256a 6f04 0000 7562  n...ubeh%jo...ub
-0000dec0: 6175 6268 9729 8172 0209 0000 7d72 0309  aubh.).r....}r..
-0000ded0: 0000 2868 1e58 4700 0000 3a63 6c61 7373  ..(h.XG...:class
-0000dee0: 3a60 6c73 7166 6974 2e73 6369 7079 5f6d  :`lsqfit.scipy_m
-0000def0: 756c 7469 6d69 6e65 7860 206f 626a 6563  ultiminex` objec
-0000df00: 7473 2068 6176 6520 7468 6520 666f 6c6c  ts have the foll
-0000df10: 6f77 696e 6720 6174 7472 6962 7574 6573  owing attributes
-0000df20: 2e72 0409 0000 681f 6a76 0700 0068 236a  .r....h.jv...h#j
-0000df30: 7d07 0000 6825 689a 6827 7d72 0509 0000  }...h%h.h'}r....
-0000df40: 2868 295d 682a 5d68 2b5d 682c 5d68 2f5d  (h)]h*]h+]h,]h/]
-0000df50: 7568 314b 1968 3268 0268 335d 7206 0900  uh1K.h2h.h3]r...
-0000df60: 0028 683c 2981 7207 0900 007d 7208 0900  .(h<).r....}r...
-0000df70: 0028 681e 5820 0000 003a 636c 6173 733a  .(h.X ...:class:
-0000df80: 606c 7371 6669 742e 7363 6970 795f 6d75  `lsqfit.scipy_mu
-0000df90: 6c74 696d 696e 6578 6072 0909 0000 681f  ltiminex`r....h.
-0000dfa0: 6a02 0900 0068 236a 7d07 0000 6825 6840  j....h#j}...h%h@
-0000dfb0: 6827 7d72 0a09 0000 2855 0772 6566 7479  h'}r....(U.refty
-0000dfc0: 7065 5805 0000 0063 6c61 7373 6842 8968  peX....classhB.h
-0000dfd0: 4358 1700 0000 6c73 7166 6974 2e73 6369  CX....lsqfit.sci
-0000dfe0: 7079 5f6d 756c 7469 6d69 6e65 7855 0972  py_multiminexU.r
-0000dff0: 6566 646f 6d61 696e 5802 0000 0070 7972  efdomainX....pyr
-0000e000: 0b09 0000 682c 5d68 2b5d 550b 7265 6665  ....h,]h+]U.refe
-0000e010: 7870 6c69 6369 7489 6829 5d68 2a5d 682f  xplicit.h)]h*]h/
-0000e020: 5d68 4568 4668 476a 2b07 0000 6848 6a28  ]hEhFhGj+...hHj(
-0000e030: 0700 0075 6831 4b19 6833 5d72 0c09 0000  ...uh1K.h3]r....
-0000e040: 684a 2981 720d 0900 007d 720e 0900 0028  hJ).r....}r....(
-0000e050: 681e 6a09 0900 0068 277d 720f 0900 0028  h.j....h'}r....(
-0000e060: 6829 5d68 2a5d 7210 0900 0028 684f 6a0b  h)]h*]r....(hOj.
-0000e070: 0900 0058 0800 0000 7079 2d63 6c61 7373  ...X....py-class
-0000e080: 7211 0900 0065 682b 5d68 2c5d 682f 5d75  r....eh+]h,]h/]u
-0000e090: 681f 6a07 0900 0068 335d 7212 0900 0068  h.j....h3]r....h
-0000e0a0: 5258 1700 0000 6c73 7166 6974 2e73 6369  RX....lsqfit.sci
-0000e0b0: 7079 5f6d 756c 7469 6d69 6e65 7872 1309  py_multiminexr..
-0000e0c0: 0000 8581 7214 0900 007d 7215 0900 0028  ....r....}r....(
-0000e0d0: 681e 5500 681f 6a0d 0900 0075 6261 6825  h.U.h.j....ubah%
-0000e0e0: 6856 7562 6175 6268 5258 2700 0000 206f  hVubaubhRX'... o
-0000e0f0: 626a 6563 7473 2068 6176 6520 7468 6520  bjects have the 
-0000e100: 666f 6c6c 6f77 696e 6720 6174 7472 6962  following attrib
-0000e110: 7574 6573 2e72 1609 0000 8581 7217 0900  utes.r......r...
-0000e120: 007d 7218 0900 0028 681e 5827 0000 0020  .}r....(h.X'... 
-0000e130: 6f62 6a65 6374 7320 6861 7665 2074 6865  objects have the
-0000e140: 2066 6f6c 6c6f 7769 6e67 2061 7474 7269   following attri
-0000e150: 6275 7465 732e 6823 4e68 314e 6832 6802  butes.h#Nh1Nh2h.
-0000e160: 681f 6a02 0900 0075 6265 7562 68cf 2981  h.j....ubeubh.).
-0000e170: 7219 0900 007d 721a 0900 0028 681e 5500  r....}r....(h.U.
-0000e180: 681f 6a76 0700 0068 236a 7d07 0000 6825  h.jv...h#j}...h%
-0000e190: 68d2 6827 7d72 1b09 0000 2868 2c5d 682b  h.h'}r....(h,]h+
-0000e1a0: 5d68 295d 682a 5d68 2f5d 5507 656e 7472  ]h)]h*]h/]U.entr
-0000e1b0: 6965 735d 721c 0900 0028 68d5 5825 0000  ies]r....(h.X%..
-0000e1c0: 0078 2028 6c73 7166 6974 2e73 6369 7079  .x (lsqfit.scipy
-0000e1d0: 5f6d 756c 7469 6d69 6e65 7820 6174 7472  _multiminex attr
-0000e1e0: 6962 7574 6529 680a 5500 4e74 721d 0900  ibute)h.U.Ntr...
-0000e1f0: 0061 7568 314e 6832 6802 6833 5d75 6268  .auh1Nh2h.h3]ubh
-0000e200: d729 8172 1e09 0000 7d72 1f09 0000 2868  .).r....}r....(h
-0000e210: 1e55 0068 1f6a 7607 0000 6823 6a7d 0700  .U.h.jv...h#j}..
-0000e220: 0068 2568 da68 277d 7220 0900 0028 68dc  .h%h.h'}r ...(h.
-0000e230: 8968 dd58 0200 0000 7079 682c 5d68 2b5d  .h.X....pyh,]h+]
-0000e240: 6829 5d68 2a5d 682f 5d68 df58 0900 0000  h)]h*]h/]h.X....
-0000e250: 6174 7472 6962 7574 6572 2109 0000 68e1  attributer!...h.
-0000e260: 6a21 0900 0075 6831 4e68 3268 0268 335d  j!...uh1Nh2h.h3]
-0000e270: 7222 0900 0028 68e3 2981 7223 0900 007d  r"...(h.).r#...}
-0000e280: 7224 0900 0028 681e 5801 0000 0078 681f  r$...(h.X....xh.
-0000e290: 6a1e 0900 0068 236a 7d07 0000 6825 68e7  j....h#j}...h%h.
-0000e2a0: 6827 7d72 2509 0000 2868 2c5d 7226 0900  h'}r%...(h,]r&..
-0000e2b0: 0068 0a61 68ea 6a28 0700 0068 2b5d 6829  .h.ah.j(...h+]h)
-0000e2c0: 5d68 2a5d 682f 5d72 2709 0000 680a 6168  ]h*]h/]r'...h.ah
-0000e2d0: f058 1200 0000 7363 6970 795f 6d75 6c74  .X....scipy_mult
-0000e2e0: 696d 696e 6578 2e78 68f2 6a2b 0700 0068  iminex.xh.j+...h
-0000e2f0: f389 7568 314b 1e68 3268 0268 335d 7228  ..uh1K.h2h.h3]r(
-0000e300: 0900 006a 0901 0000 2981 7229 0900 007d  ...j....).r)...}
-0000e310: 722a 0900 0028 681e 5801 0000 0078 681f  r*...(h.X....xh.
-0000e320: 6a23 0900 0068 236a 7d07 0000 6825 6a0c  j#...h#j}...h%j.
-0000e330: 0100 0068 277d 722b 0900 0028 68fa 68fb  ...h'}r+...(h.h.
-0000e340: 682c 5d68 2b5d 6829 5d68 2a5d 682f 5d75  h,]h+]h)]h*]h/]u
-0000e350: 6831 4b1e 6832 6802 6833 5d72 2c09 0000  h1K.h2h.h3]r,...
-0000e360: 6852 5801 0000 0078 8581 722d 0900 007d  hRX....x..r-...}
-0000e370: 722e 0900 0028 681e 5500 6823 4e68 314e  r....(h.U.h#Nh1N
-0000e380: 6832 6802 681f 6a29 0900 0075 6261 7562  h2h.h.j)...ubaub
-0000e390: 6175 626a 5001 0000 2981 722f 0900 007d  aubjP...).r/...}
-0000e3a0: 7230 0900 0028 681e 5500 681f 6a1e 0900  r0...(h.U.h.j...
-0000e3b0: 0068 236a 7d07 0000 6825 6a53 0100 0068  .h#j}...h%jS...h
-0000e3c0: 277d 7231 0900 0028 6829 5d68 2a5d 682b  '}r1...(h)]h*]h+
-0000e3d0: 5d68 2c5d 682f 5d75 6831 4b1e 6832 6802  ]h,]h/]uh1K.h2h.
-0000e3e0: 6833 5d72 3209 0000 6897 2981 7233 0900  h3]r2...h.).r3..
-0000e3f0: 007d 7234 0900 0028 681e 5823 0000 002a  .}r4...(h.X#...*
-0000e400: 6172 7261 792a 202d 2d20 4c6f 6361 7469  array* -- Locati
-0000e410: 6f6e 206f 6620 7468 6520 6d69 6e69 6d75  on of the minimu
-0000e420: 6d2e 681f 6a2f 0900 0068 236a 7d07 0000  m.h.j/...h#j}...
-0000e430: 6825 689a 6827 7d72 3509 0000 2868 295d  h%h.h'}r5...(h)]
-0000e440: 682a 5d68 2b5d 682c 5d68 2f5d 7568 314b  h*]h+]h,]h/]uh1K
-0000e450: 1d68 3268 0268 335d 7236 0900 0028 6af2  .h2h.h3]r6...(j.
-0000e460: 0400 0029 8172 3709 0000 7d72 3809 0000  ...).r7...}r8...
-0000e470: 2868 1e58 0700 0000 2a61 7272 6179 2a68  (h.X....*array*h
-0000e480: 277d 7239 0900 0028 6829 5d68 2a5d 682b  '}r9...(h)]h*]h+
-0000e490: 5d68 2c5d 682f 5d75 681f 6a33 0900 0068  ]h,]h/]uh.j3...h
-0000e4a0: 335d 723a 0900 0068 5258 0500 0000 6172  3]r:...hRX....ar
-0000e4b0: 7261 7972 3b09 0000 8581 723c 0900 007d  rayr;.....r<...}
-0000e4c0: 723d 0900 0028 681e 5500 681f 6a37 0900  r=...(h.U.h.j7..
-0000e4d0: 0075 6261 6825 6afa 0400 0075 6268 5258  .ubah%j....ubhRX
-0000e4e0: 1d00 0000 20e2 8093 204c 6f63 6174 696f  .... ... Locatio
-0000e4f0: 6e20 6f66 2074 6865 206d 696e 696d 756d  n of the minimum
-0000e500: 2e72 3e09 0000 8581 723f 0900 007d 7240  .r>.....r?...}r@
-0000e510: 0900 0028 681e 581c 0000 0020 2d2d 204c  ...(h.X.... -- L
-0000e520: 6f63 6174 696f 6e20 6f66 2074 6865 206d  ocation of the m
-0000e530: 696e 696d 756d 2e68 234e 6831 4e68 3268  inimum.h#Nh1Nh2h
-0000e540: 0268 1f6a 3309 0000 7562 6575 6261 7562  .h.j3...ubeubaub
-0000e550: 6575 6268 cf29 8172 4109 0000 7d72 4209  eubh.).rA...}rB.
-0000e560: 0000 2868 1e55 0068 1f6a 7607 0000 6823  ..(h.U.h.jv...h#
-0000e570: 6a7d 0700 0068 2568 d268 277d 7243 0900  j}...h%h.h'}rC..
-0000e580: 0028 682c 5d68 2b5d 6829 5d68 2a5d 682f  .(h,]h+]h)]h*]h/
-0000e590: 5d55 0765 6e74 7269 6573 5d72 4409 0000  ]U.entries]rD...
-0000e5a0: 2868 d558 2500 0000 6620 286c 7371 6669  (h.X%...f (lsqfi
-0000e5b0: 742e 7363 6970 795f 6d75 6c74 696d 696e  t.scipy_multimin
-0000e5c0: 6578 2061 7474 7269 6275 7465 2968 0c55  ex attribute)h.U
-0000e5d0: 004e 7472 4509 0000 6175 6831 4e68 3268  .NtrE...auh1Nh2h
-0000e5e0: 0268 335d 7562 68d7 2981 7246 0900 007d  .h3]ubh.).rF...}
-0000e5f0: 7247 0900 0028 681e 5500 681f 6a76 0700  rG...(h.U.h.jv..
-0000e600: 0068 236a 7d07 0000 6825 68da 6827 7d72  .h#j}...h%h.h'}r
-0000e610: 4809 0000 2868 dc89 68dd 5802 0000 0070  H...(h..h.X....p
-0000e620: 7968 2c5d 682b 5d68 295d 682a 5d68 2f5d  yh,]h+]h)]h*]h/]
-0000e630: 68df 5809 0000 0061 7474 7269 6275 7465  h.X....attribute
-0000e640: 7249 0900 0068 e16a 4909 0000 7568 314e  rI...h.jI...uh1N
-0000e650: 6832 6802 6833 5d72 4a09 0000 2868 e329  h2h.h3]rJ...(h.)
-0000e660: 8172 4b09 0000 7d72 4c09 0000 2868 1e58  .rK...}rL...(h.X
-0000e670: 0100 0000 6668 1f6a 4609 0000 6823 6a7d  ....fh.jF...h#j}
-0000e680: 0700 0068 2568 e768 277d 724d 0900 0028  ...h%h.h'}rM...(
-0000e690: 682c 5d72 4e09 0000 680c 6168 ea6a 2807  h,]rN...h.ah.j(.
-0000e6a0: 0000 682b 5d68 295d 682a 5d68 2f5d 724f  ..h+]h)]h*]h/]rO
-0000e6b0: 0900 0068 0c61 68f0 5812 0000 0073 6369  ...h.ah.X....sci
-0000e6c0: 7079 5f6d 756c 7469 6d69 6e65 782e 6668  py_multiminex.fh
-0000e6d0: f26a 2b07 0000 68f3 8975 6831 4b22 6832  .j+...h..uh1K"h2
-0000e6e0: 6802 6833 5d72 5009 0000 6a09 0100 0029  h.h3]rP...j....)
-0000e6f0: 8172 5109 0000 7d72 5209 0000 2868 1e58  .rQ...}rR...(h.X
-0000e700: 0100 0000 6668 1f6a 4b09 0000 6823 6a7d  ....fh.jK...h#j}
-0000e710: 0700 0068 256a 0c01 0000 6827 7d72 5309  ...h%j....h'}rS.
-0000e720: 0000 2868 fa68 fb68 2c5d 682b 5d68 295d  ..(h.h.h,]h+]h)]
-0000e730: 682a 5d68 2f5d 7568 314b 2268 3268 0268  h*]h/]uh1K"h2h.h
-0000e740: 335d 7254 0900 0068 5258 0100 0000 6685  3]rT...hRX....f.
-0000e750: 8172 5509 0000 7d72 5609 0000 2868 1e55  .rU...}rV...(h.U
-0000e760: 0068 234e 6831 4e68 3268 0268 1f6a 5109  .h#Nh1Nh2h.h.jQ.
-0000e770: 0000 7562 6175 6261 7562 6a50 0100 0029  ..ubaubaubjP...)
-0000e780: 8172 5709 0000 7d72 5809 0000 2868 1e55  .rW...}rX...(h.U
-0000e790: 0068 1f6a 4609 0000 6823 6a7d 0700 0068  .h.jF...h#j}...h
-0000e7a0: 256a 5301 0000 6827 7d72 5909 0000 2868  %jS...h'}rY...(h
-0000e7b0: 295d 682a 5d68 2b5d 682c 5d68 2f5d 7568  )]h*]h+]h,]h/]uh
-0000e7c0: 314b 2268 3268 0268 335d 725a 0900 0068  1K"h2h.h3]rZ...h
-0000e7d0: 9729 8172 5b09 0000 7d72 5c09 0000 2868  .).r[...}r\...(h
-0000e7e0: 1e58 3500 0000 2a66 6c6f 6174 2a20 2d2d  .X5...*float* --
-0000e7f0: 2056 616c 7565 206f 6620 6675 6e63 7469   Value of functi
-0000e800: 6f6e 2060 6066 2878 2960 6020 6174 2074  on ``f(x)`` at t
-0000e810: 6865 206d 696e 696d 756d 2e68 1f6a 5709  he minimum.h.jW.
-0000e820: 0000 6823 6a7d 0700 0068 2568 9a68 277d  ..h#j}...h%h.h'}
-0000e830: 725d 0900 0028 6829 5d68 2a5d 682b 5d68  r]...(h)]h*]h+]h
-0000e840: 2c5d 682f 5d75 6831 4b21 6832 6802 6833  ,]h/]uh1K!h2h.h3
-0000e850: 5d72 5e09 0000 286a f204 0000 2981 725f  ]r^...(j....).r_
-0000e860: 0900 007d 7260 0900 0028 681e 5807 0000  ...}r`...(h.X...
-0000e870: 002a 666c 6f61 742a 6827 7d72 6109 0000  .*float*h'}ra...
-0000e880: 2868 295d 682a 5d68 2b5d 682c 5d68 2f5d  (h)]h*]h+]h,]h/]
-0000e890: 7568 1f6a 5b09 0000 6833 5d72 6209 0000  uh.j[...h3]rb...
-0000e8a0: 6852 5805 0000 0066 6c6f 6174 7263 0900  hRX....floatrc..
-0000e8b0: 0085 8172 6409 0000 7d72 6509 0000 2868  ...rd...}re...(h
-0000e8c0: 1e55 0068 1f6a 5f09 0000 7562 6168 256a  .U.h.j_...ubah%j
-0000e8d0: fa04 0000 7562 6852 5817 0000 0020 e280  ....ubhRX.... ..
-0000e8e0: 9320 5661 6c75 6520 6f66 2066 756e 6374  . Value of funct
-0000e8f0: 696f 6e20 7266 0900 0085 8172 6709 0000  ion rf.....rg...
-0000e900: 7d72 6809 0000 2868 1e58 1600 0000 202d  }rh...(h.X.... -
-0000e910: 2d20 5661 6c75 6520 6f66 2066 756e 6374  - Value of funct
-0000e920: 696f 6e20 6823 4e68 314e 6832 6802 681f  ion h#Nh1Nh2h.h.
-0000e930: 6a5b 0900 0075 6268 4a29 8172 6909 0000  j[...ubhJ).ri...
-0000e940: 7d72 6a09 0000 2868 1e58 0800 0000 6060  }rj...(h.X....``
-0000e950: 6628 7829 6060 6827 7d72 6b09 0000 2868  f(x)``h'}rk...(h
-0000e960: 295d 682a 5d68 2b5d 682c 5d68 2f5d 7568  )]h*]h+]h,]h/]uh
-0000e970: 1f6a 5b09 0000 6833 5d72 6c09 0000 6852  .j[...h3]rl...hR
-0000e980: 5804 0000 0066 2878 2972 6d09 0000 8581  X....f(x)rm.....
-0000e990: 726e 0900 007d 726f 0900 0028 681e 5500  rn...}ro...(h.U.
-0000e9a0: 681f 6a69 0900 0075 6261 6825 6856 7562  h.ji...ubah%hVub
-0000e9b0: 6852 5810 0000 0020 6174 2074 6865 206d  hRX.... at the m
-0000e9c0: 696e 696d 756d 2e72 7009 0000 8581 7271  inimum.rp.....rq
-0000e9d0: 0900 007d 7272 0900 0028 681e 5810 0000  ...}rr...(h.X...
-0000e9e0: 0020 6174 2074 6865 206d 696e 696d 756d  . at the minimum
-0000e9f0: 2e68 234e 6831 4e68 3268 0268 1f6a 5b09  .h#Nh1Nh2h.h.j[.
-0000ea00: 0000 7562 6575 6261 7562 6575 6268 cf29  ..ubeubaubeubh.)
-0000ea10: 8172 7309 0000 7d72 7409 0000 2868 1e55  .rs...}rt...(h.U
-0000ea20: 0068 1f6a 7607 0000 6823 6a7d 0700 0068  .h.jv...h#j}...h
-0000ea30: 2568 d268 277d 7275 0900 0028 682c 5d68  %h.h'}ru...(h,]h
-0000ea40: 2b5d 6829 5d68 2a5d 682f 5d55 0765 6e74  +]h)]h*]h/]U.ent
-0000ea50: 7269 6573 5d72 7609 0000 2868 d558 2700  ries]rv...(h.X'.
-0000ea60: 0000 6e69 7420 286c 7371 6669 742e 7363  ..nit (lsqfit.sc
-0000ea70: 6970 795f 6d75 6c74 696d 696e 6578 2061  ipy_multiminex a
-0000ea80: 7474 7269 6275 7465 2968 1655 004e 7472  ttribute)h.U.Ntr
-0000ea90: 7709 0000 6175 6831 4e68 3268 0268 335d  w...auh1Nh2h.h3]
-0000eaa0: 7562 68d7 2981 7278 0900 007d 7279 0900  ubh.).rx...}ry..
-0000eab0: 0028 681e 5500 681f 6a76 0700 0068 236a  .(h.U.h.jv...h#j
-0000eac0: 7d07 0000 6825 68da 6827 7d72 7a09 0000  }...h%h.h'}rz...
-0000ead0: 2868 dc89 68dd 5802 0000 0070 7968 2c5d  (h..h.X....pyh,]
-0000eae0: 682b 5d68 295d 682a 5d68 2f5d 68df 5809  h+]h)]h*]h/]h.X.
-0000eaf0: 0000 0061 7474 7269 6275 7465 727b 0900  ...attributer{..
-0000eb00: 0068 e16a 7b09 0000 7568 314e 6832 6802  .h.j{...uh1Nh2h.
-0000eb10: 6833 5d72 7c09 0000 2868 e329 8172 7d09  h3]r|...(h.).r}.
-0000eb20: 0000 7d72 7e09 0000 2868 1e58 0300 0000  ..}r~...(h.X....
-0000eb30: 6e69 7472 7f09 0000 681f 6a78 0900 0068  nitr....h.jx...h
-0000eb40: 236a 7d07 0000 6825 68e7 6827 7d72 8009  #j}...h%h.h'}r..
-0000eb50: 0000 2868 2c5d 7281 0900 0068 1661 68ea  ..(h,]r....h.ah.
-0000eb60: 6a28 0700 0068 2b5d 6829 5d68 2a5d 682f  j(...h+]h)]h*]h/
-0000eb70: 5d72 8209 0000 6816 6168 f058 1400 0000  ]r....h.ah.X....
-0000eb80: 7363 6970 795f 6d75 6c74 696d 696e 6578  scipy_multiminex
-0000eb90: 2e6e 6974 68f2 6a2b 0700 0068 f389 7568  .nith.j+...h..uh
-0000eba0: 314b 2668 3268 0268 335d 7283 0900 006a  1K&h2h.h3]r....j
-0000ebb0: 0901 0000 2981 7284 0900 007d 7285 0900  ....).r....}r...
-0000ebc0: 0028 681e 6a7f 0900 0068 1f6a 7d09 0000  .(h.j....h.j}...
-0000ebd0: 6823 6a7d 0700 0068 256a 0c01 0000 6827  h#j}...h%j....h'
-0000ebe0: 7d72 8609 0000 2868 fa68 fb68 2c5d 682b  }r....(h.h.h,]h+
-0000ebf0: 5d68 295d 682a 5d68 2f5d 7568 314b 2668  ]h)]h*]h/]uh1K&h
-0000ec00: 3268 0268 335d 7287 0900 0068 5258 0300  2h.h3]r....hRX..
-0000ec10: 0000 6e69 7472 8809 0000 8581 7289 0900  ..nitr......r...
-0000ec20: 007d 728a 0900 0028 681e 5500 6823 4e68  .}r....(h.U.h#Nh
-0000ec30: 314e 6832 6802 681f 6a84 0900 0075 6261  1Nh2h.h.j....uba
-0000ec40: 7562 6175 626a 5001 0000 2981 728b 0900  ubaubjP...).r...
-0000ec50: 007d 728c 0900 0028 681e 5500 681f 6a78  .}r....(h.U.h.jx
-0000ec60: 0900 0068 236a 7d07 0000 6825 6a53 0100  ...h#j}...h%jS..
-0000ec70: 0068 277d 728d 0900 0028 6829 5d68 2a5d  .h'}r....(h)]h*]
-0000ec80: 682b 5d68 2c5d 682f 5d75 6831 4b26 6832  h+]h,]h/]uh1K&h2
-0000ec90: 6802 6833 5d72 8e09 0000 6897 2981 728f  h.h3]r....h.).r.
-0000eca0: 0900 007d 7290 0900 0028 681e 583b 0000  ...}r....(h.X;..
-0000ecb0: 002a 696e 742a 202d 2d20 4e75 6d62 6572  .*int* -- Number
-0000ecc0: 206f 6620 6974 6572 6174 696f 6e73 2072   of iterations r
-0000ecd0: 6571 7569 7265 6420 746f 2066 696e 6420  equired to find 
-0000ece0: 7468 6520 6d69 6e69 6d75 6d2e 681f 6a8b  the minimum.h.j.
-0000ecf0: 0900 0068 236a 7d07 0000 6825 689a 6827  ...h#j}...h%h.h'
-0000ed00: 7d72 9109 0000 2868 295d 682a 5d68 2b5d  }r....(h)]h*]h+]
-0000ed10: 682c 5d68 2f5d 7568 314b 2568 3268 0268  h,]h/]uh1K%h2h.h
-0000ed20: 335d 7292 0900 0028 6af2 0400 0029 8172  3]r....(j....).r
-0000ed30: 9309 0000 7d72 9409 0000 2868 1e58 0500  ....}r....(h.X..
-0000ed40: 0000 2a69 6e74 2a68 277d 7295 0900 0028  ..*int*h'}r....(
-0000ed50: 6829 5d68 2a5d 682b 5d68 2c5d 682f 5d75  h)]h*]h+]h,]h/]u
-0000ed60: 681f 6a8f 0900 0068 335d 7296 0900 0068  h.j....h3]r....h
-0000ed70: 5258 0300 0000 696e 7472 9709 0000 8581  RX....intr......
-0000ed80: 7298 0900 007d 7299 0900 0028 681e 5500  r....}r....(h.U.
-0000ed90: 681f 6a93 0900 0075 6261 6825 6afa 0400  h.j....ubah%j...
-0000eda0: 0075 6268 5258 3700 0000 20e2 8093 204e  .ubhRX7... ... N
-0000edb0: 756d 6265 7220 6f66 2069 7465 7261 7469  umber of iterati
-0000edc0: 6f6e 7320 7265 7175 6972 6564 2074 6f20  ons required to 
-0000edd0: 6669 6e64 2074 6865 206d 696e 696d 756d  find the minimum
-0000ede0: 2e72 9a09 0000 8581 729b 0900 007d 729c  .r......r....}r.
-0000edf0: 0900 0028 681e 5836 0000 0020 2d2d 204e  ...(h.X6... -- N
-0000ee00: 756d 6265 7220 6f66 2069 7465 7261 7469  umber of iterati
-0000ee10: 6f6e 7320 7265 7175 6972 6564 2074 6f20  ons required to 
-0000ee20: 6669 6e64 2074 6865 206d 696e 696d 756d  find the minimum
-0000ee30: 2e68 234e 6831 4e68 3268 0268 1f6a 8f09  .h#Nh1Nh2h.h.j..
-0000ee40: 0000 7562 6575 6261 7562 6575 6268 cf29  ..ubeubaubeubh.)
-0000ee50: 8172 9d09 0000 7d72 9e09 0000 2868 1e55  .r....}r....(h.U
-0000ee60: 0068 1f6a 7607 0000 6823 6a7d 0700 0068  .h.jv...h#j}...h
-0000ee70: 2568 d268 277d 729f 0900 0028 682c 5d68  %h.h'}r....(h,]h
-0000ee80: 2b5d 6829 5d68 2a5d 682f 5d55 0765 6e74  +]h)]h*]h/]U.ent
-0000ee90: 7269 6573 5d72 a009 0000 2868 d558 2900  ries]r....(h.X).
-0000eea0: 0000 6572 726f 7220 286c 7371 6669 742e  ..error (lsqfit.
-0000eeb0: 7363 6970 795f 6d75 6c74 696d 696e 6578  scipy_multiminex
-0000eec0: 2061 7474 7269 6275 7465 2968 1755 004e   attribute)h.U.N
-0000eed0: 7472 a109 0000 6175 6831 4e68 3268 0268  tr....auh1Nh2h.h
-0000eee0: 335d 7562 68d7 2981 72a2 0900 007d 72a3  3]ubh.).r....}r.
-0000eef0: 0900 0028 681e 5500 681f 6a76 0700 0068  ...(h.U.h.jv...h
-0000ef00: 236a 7d07 0000 6825 68da 6827 7d72 a409  #j}...h%h.h'}r..
-0000ef10: 0000 2868 dc89 68dd 5802 0000 0070 7968  ..(h..h.X....pyh
-0000ef20: 2c5d 682b 5d68 295d 682a 5d68 2f5d 68df  ,]h+]h)]h*]h/]h.
-0000ef30: 5809 0000 0061 7474 7269 6275 7465 72a5  X....attributer.
-0000ef40: 0900 0068 e16a a509 0000 7568 314e 6832  ...h.j....uh1Nh2
-0000ef50: 6802 6833 5d72 a609 0000 2868 e329 8172  h.h3]r....(h.).r
-0000ef60: a709 0000 7d72 a809 0000 2868 1e58 0500  ....}r....(h.X..
-0000ef70: 0000 6572 726f 7272 a909 0000 681f 6aa2  ..errorr....h.j.
-0000ef80: 0900 0068 236a 7d07 0000 6825 68e7 6827  ...h#j}...h%h.h'
-0000ef90: 7d72 aa09 0000 2868 2c5d 72ab 0900 0068  }r....(h,]r....h
-0000efa0: 1761 68ea 6a28 0700 0068 2b5d 6829 5d68  .ah.j(...h+]h)]h
-0000efb0: 2a5d 682f 5d72 ac09 0000 6817 6168 f058  *]h/]r....h.ah.X
-0000efc0: 1600 0000 7363 6970 795f 6d75 6c74 696d  ....scipy_multim
-0000efd0: 696e 6578 2e65 7272 6f72 68f2 6a2b 0700  inex.errorh.j+..
-0000efe0: 0068 f389 7568 314b 2a68 3268 0268 335d  .h..uh1K*h2h.h3]
-0000eff0: 72ad 0900 006a 0901 0000 2981 72ae 0900  r....j....).r...
-0000f000: 007d 72af 0900 0028 681e 6aa9 0900 0068  .}r....(h.j....h
-0000f010: 1f6a a709 0000 6823 6a7d 0700 0068 256a  .j....h#j}...h%j
-0000f020: 0c01 0000 6827 7d72 b009 0000 2868 fa68  ....h'}r....(h.h
-0000f030: fb68 2c5d 682b 5d68 295d 682a 5d68 2f5d  .h,]h+]h)]h*]h/]
-0000f040: 7568 314b 2a68 3268 0268 335d 72b1 0900  uh1K*h2h.h3]r...
-0000f050: 0068 5258 0500 0000 6572 726f 7272 b209  .hRX....errorr..
-0000f060: 0000 8581 72b3 0900 007d 72b4 0900 0028  ....r....}r....(
-0000f070: 681e 5500 6823 4e68 314e 6832 6802 681f  h.U.h#Nh1Nh2h.h.
-0000f080: 6aae 0900 0075 6261 7562 6175 626a 5001  j....ubaubaubjP.
-0000f090: 0000 2981 72b5 0900 007d 72b6 0900 0028  ..).r....}r....(
-0000f0a0: 681e 5500 681f 6aa2 0900 0068 236a 7d07  h.U.h.j....h#j}.
-0000f0b0: 0000 6825 6a53 0100 0068 277d 72b7 0900  ..h%jS...h'}r...
-0000f0c0: 0028 6829 5d68 2a5d 682b 5d68 2c5d 682f  .(h)]h*]h+]h,]h/
-0000f0d0: 5d75 6831 4b2a 6832 6802 6833 5d72 b809  ]uh1K*h2h.h3]r..
-0000f0e0: 0000 6897 2981 72b9 0900 007d 72ba 0900  ..h.).r....}r...
-0000f0f0: 0028 681e 5847 0000 002a 4e6f 6520 6f72  .(h.XG...*Noe or
-0000f100: 2073 7472 2a20 2d2d 2060 604e 6f6e 6560   str* -- ``None`
-0000f110: 6020 6966 2066 6974 2073 7563 6365 7373  ` if fit success
-0000f120: 6675 6c3b 2061 6e20 6572 726f 720a 6d65  ful; an error.me
-0000f130: 7373 6167 6520 6f74 6865 7277 6973 652e  ssage otherwise.
-0000f140: 681f 6ab5 0900 0068 236a 7d07 0000 6825  h.j....h#j}...h%
-0000f150: 689a 6827 7d72 bb09 0000 2868 295d 682a  h.h'}r....(h)]h*
-0000f160: 5d68 2b5d 682c 5d68 2f5d 7568 314b 2968  ]h+]h,]h/]uh1K)h
-0000f170: 3268 0268 335d 72bc 0900 0028 6af2 0400  2h.h3]r....(j...
-0000f180: 0029 8172 bd09 0000 7d72 be09 0000 2868  .).r....}r....(h
-0000f190: 1e58 0c00 0000 2a4e 6f65 206f 7220 7374  .X....*Noe or st
-0000f1a0: 722a 6827 7d72 bf09 0000 2868 295d 682a  r*h'}r....(h)]h*
-0000f1b0: 5d68 2b5d 682c 5d68 2f5d 7568 1f6a b909  ]h+]h,]h/]uh.j..
-0000f1c0: 0000 6833 5d72 c009 0000 6852 580a 0000  ..h3]r....hRX...
-0000f1d0: 004e 6f65 206f 7220 7374 7272 c109 0000  .Noe or strr....
-0000f1e0: 8581 72c2 0900 007d 72c3 0900 0028 681e  ..r....}r....(h.
-0000f1f0: 5500 681f 6abd 0900 0075 6261 6825 6afa  U.h.j....ubah%j.
-0000f200: 0400 0075 6268 5258 0500 0000 20e2 8093  ...ubhRX.... ...
-0000f210: 2072 c409 0000 8581 72c5 0900 007d 72c6   r......r....}r.
-0000f220: 0900 0028 681e 5804 0000 0020 2d2d 2068  ...(h.X.... -- h
-0000f230: 234e 6831 4e68 3268 0268 1f6a b909 0000  #Nh1Nh2h.h.j....
-0000f240: 7562 684a 2981 72c7 0900 007d 72c8 0900  ubhJ).r....}r...
-0000f250: 0028 681e 5808 0000 0060 604e 6f6e 6560  .(h.X....``None`
-0000f260: 6068 277d 72c9 0900 0028 6829 5d68 2a5d  `h'}r....(h)]h*]
-0000f270: 682b 5d68 2c5d 682f 5d75 681f 6ab9 0900  h+]h,]h/]uh.j...
-0000f280: 0068 335d 72ca 0900 0068 5258 0400 0000  .h3]r....hRX....
-0000f290: 4e6f 6e65 72cb 0900 0085 8172 cc09 0000  Noner......r....
-0000f2a0: 7d72 cd09 0000 2868 1e55 0068 1f6a c709  }r....(h.U.h.j..
-0000f2b0: 0000 7562 6168 2568 5675 6268 5258 2f00  ..ubah%hVubhRX/.
-0000f2c0: 0000 2069 6620 6669 7420 7375 6363 6573  .. if fit succes
-0000f2d0: 7366 756c 3b20 616e 2065 7272 6f72 0a6d  sful; an error.m
-0000f2e0: 6573 7361 6765 206f 7468 6572 7769 7365  essage otherwise
-0000f2f0: 2e72 ce09 0000 8581 72cf 0900 007d 72d0  .r......r....}r.
-0000f300: 0900 0028 681e 582f 0000 0020 6966 2066  ...(h.X/... if f
-0000f310: 6974 2073 7563 6365 7373 6675 6c3b 2061  it successful; a
-0000f320: 6e20 6572 726f 720a 6d65 7373 6167 6520  n error.message 
-0000f330: 6f74 6865 7277 6973 652e 6823 4e68 314e  otherwise.h#Nh1N
-0000f340: 6832 6802 681f 6ab9 0900 0075 6265 7562  h2h.h.j....ubeub
-0000f350: 6175 6265 7562 6575 6265 7562 6575 6265  aubeubeubeubeube
-0000f360: 7562 6823 6824 6825 685d 6827 7d72 d109  ubh#h$h%h]h'}r..
-0000f370: 0000 2868 295d 682a 5d68 2b5d 682c 5d68  ..(h)]h*]h+]h,]h
-0000f380: 2f5d 72d2 0900 0068 1a61 7568 314b 0668  /]r....h.auh1K.h
-0000f390: 3268 0268 335d 72d3 0900 0068 3c29 8172  2h.h3]r....h<).r
-0000f3a0: d409 0000 7d72 d509 0000 2868 1e58 1800  ....}r....(h.X..
-0000f3b0: 0000 3a63 6c61 7373 3a60 6776 6172 2e42  ..:class:`gvar.B
-0000f3c0: 7566 6665 7244 6963 7460 72d6 0900 0068  ufferDict`r....h
-0000f3d0: 1f68 1c68 2368 2468 2568 4068 277d 72d7  .h.h#h$h%h@h'}r.
-0000f3e0: 0900 0028 5507 7265 6674 7970 6558 0500  ...(U.reftypeX..
-0000f3f0: 0000 636c 6173 7368 4289 6843 580f 0000  ..classhB.hCX...
-0000f400: 0067 7661 722e 4275 6666 6572 4469 6374  .gvar.BufferDict
-0000f410: 5509 7265 6664 6f6d 6169 6e58 0200 0000  U.refdomainX....
-0000f420: 7079 72d8 0900 0068 2c5d 682b 5d55 0b72  pyr....h,]h+]U.r
-0000f430: 6566 6578 706c 6963 6974 8968 295d 682a  efexplicit.h)]h*
-0000f440: 5d68 2f5d 6845 6846 6847 4e68 484e 7568  ]h/]hEhFhGNhHNuh
-0000f450: 314b 0668 335d 72d9 0900 0068 4a29 8172  1K.h3]r....hJ).r
-0000f460: da09 0000 7d72 db09 0000 2868 1e6a d609  ....}r....(h.j..
-0000f470: 0000 6827 7d72 dc09 0000 2868 295d 682a  ..h'}r....(h)]h*
-0000f480: 5d72 dd09 0000 2868 4f6a d809 0000 5808  ]r....(hOj....X.
-0000f490: 0000 0070 792d 636c 6173 7372 de09 0000  ...py-classr....
-0000f4a0: 6568 2b5d 682c 5d68 2f5d 7568 1f6a d409  eh+]h,]h/]uh.j..
-0000f4b0: 0000 6833 5d72 df09 0000 6852 580f 0000  ..h3]r....hRX...
-0000f4c0: 0067 7661 722e 4275 6666 6572 4469 6374  .gvar.BufferDict
-0000f4d0: 72e0 0900 0085 8172 e109 0000 7d72 e209  r......r....}r..
-0000f4e0: 0000 2868 1e55 0068 1f6a da09 0000 7562  ..(h.U.h.j....ub
-0000f4f0: 6168 2568 5675 6261 7562 6175 6268 7568  ah%hVubaubaubhuh
-0000f500: 7168 6068 5b75 550e 7061 7273 655f 6d65  qh`h[uU.parse_me
-0000f510: 7373 6167 6573 72e3 0900 005d 72e4 0900  ssagesr....]r...
-0000f520: 0063 646f 6375 7469 6c73 2e6e 6f64 6573  .cdocutils.nodes
-0000f530: 0a73 7973 7465 6d5f 6d65 7373 6167 650a  .system_message.
-0000f540: 72e5 0900 0029 8172 e609 0000 7d72 e709  r....).r....}r..
-0000f550: 0000 2868 1e55 0068 277d 72e8 0900 0028  ..(h.U.h'}r....(
-0000f560: 6829 5d55 056c 6576 656c 4b01 682c 5d68  h)]U.levelK.h,]h
-0000f570: 2b5d 5506 736f 7572 6365 6a59 0100 0068  +]U.sourcejY...h
-0000f580: 2a5d 682f 5d55 046c 696e 654b 6f55 0474  *]h/]U.lineKoU.t
-0000f590: 7970 6555 0449 4e46 4f72 e909 0000 7568  ypeU.INFOr....uh
-0000f5a0: 1f6a 0a06 0000 6833 5d72 ea09 0000 6897  .j....h3]r....h.
-0000f5b0: 2981 72eb 0900 007d 72ec 0900 0028 681e  ).r....}r....(h.
-0000f5c0: 583a 0000 0045 6e75 6d65 7261 7465 6420  X:...Enumerated 
-0000f5d0: 6c69 7374 2073 7461 7274 2076 616c 7565  list start value
-0000f5e0: 206e 6f74 206f 7264 696e 616c 2d31 3a20   not ordinal-1: 
-0000f5f0: 2230 2220 286f 7264 696e 616c 2030 2968  "0" (ordinal 0)h
-0000f600: 277d 72ed 0900 0028 6829 5d68 2a5d 682b  '}r....(h)]h*]h+
-0000f610: 5d68 2c5d 682f 5d75 681f 6ae6 0900 0068  ]h,]h/]uh.j....h
-0000f620: 335d 72ee 0900 0068 5258 3e00 0000 456e  3]r....hRX>...En
-0000f630: 756d 6572 6174 6564 206c 6973 7420 7374  umerated list st
-0000f640: 6172 7420 7661 6c75 6520 6e6f 7420 6f72  art value not or
-0000f650: 6469 6e61 6c2d 313a 20e2 809c 30e2 809d  dinal-1: ...0...
-0000f660: 2028 6f72 6469 6e61 6c20 3029 72ef 0900   (ordinal 0)r...
-0000f670: 0085 8172 f009 0000 7d72 f109 0000 2868  ...r....}r....(h
-0000f680: 1e55 0068 1f6a eb09 0000 7562 6168 2568  .U.h.j....ubah%h
-0000f690: 9a75 6261 6825 550e 7379 7374 656d 5f6d  .ubah%U.system_m
-0000f6a0: 6573 7361 6765 72f2 0900 0075 6261 550e  essager....ubaU.
-0000f6b0: 6375 7272 656e 745f 736f 7572 6365 72f3  current_sourcer.
-0000f6c0: 0900 004e 550a 6465 636f 7261 7469 6f6e  ...NU.decoration
-0000f6d0: 72f4 0900 004e 5512 6175 746f 666f 6f74  r....NU.autofoot
-0000f6e0: 6e6f 7465 5f73 7461 7274 72f5 0900 004b  note_startr....K
-0000f6f0: 0155 076e 616d 6569 6473 72f6 0900 007d  .U.nameidsr....}
-0000f700: 72f7 0900 0028 6806 6806 6807 6807 6808  r....(h.h.h.h.h.
-0000f710: 6808 6809 682e 680a 680a 680b 688c 680c  h.h.h.h.h.h.h.h.
-0000f720: 680c 680d 680d 680e 680e 680f 680f 6810  h.h.h.h.h.h.h.h.
-0000f730: 6810 6811 6811 6812 6812 6813 6813 6814  h.h.h.h.h.h.h.h.
-0000f740: 6ad8 0600 0068 1568 1568 1668 1668 1768  j....h.h.h.h.h.h
-0000f750: 1775 6833 5d72 f809 0000 6821 6168 1e55  .uh3]r....h!ah.U
-0000f760: 0055 0b74 7261 6e73 666f 726d 6572 72f9  .U.transformerr.
-0000f770: 0900 004e 550d 666f 6f74 6e6f 7465 5f72  ...NU.footnote_r
-0000f780: 6566 7372 fa09 0000 7d72 fb09 0000 5508  efsr....}r....U.
-0000f790: 7265 666e 616d 6573 72fc 0900 007d 72fd  refnamesr....}r.
-0000f7a0: 0900 0055 1073 796d 626f 6c5f 666f 6f74  ...U.symbol_foot
-0000f7b0: 6e6f 7465 7372 fe09 0000 5d72 ff09 0000  notesr....]r....
-0000f7c0: 5511 6175 746f 666f 6f74 6e6f 7465 5f72  U.autofootnote_r
-0000f7d0: 6566 7372 000a 0000 5d72 010a 0000 5514  efsr....]r....U.
-0000f7e0: 7379 6d62 6f6c 5f66 6f6f 746e 6f74 655f  symbol_footnote_
-0000f7f0: 7265 6673 7202 0a00 005d 7203 0a00 0055  refsr....]r....U
-0000f800: 0963 6974 6174 696f 6e73 7204 0a00 005d  .citationsr....]
-0000f810: 7205 0a00 0068 3268 0255 0c63 7572 7265  r....h2h.U.curre
-0000f820: 6e74 5f6c 696e 6572 060a 0000 4e55 1274  nt_liner....NU.t
-0000f830: 7261 6e73 666f 726d 5f6d 6573 7361 6765  ransform_message
-0000f840: 7372 070a 0000 5d72 080a 0000 5508 7265  sr....]r....U.re
-0000f850: 706f 7274 6572 7209 0a00 004e 5508 6964  porterr....NU.id
-0000f860: 5f73 7461 7274 720a 0a00 004b 0155 0d61  _startr....K.U.a
-0000f870: 7574 6f66 6f6f 746e 6f74 6573 720b 0a00  utofootnotesr...
-0000f880: 005d 720c 0a00 0055 0d63 6974 6174 696f  .]r....U.citatio
-0000f890: 6e5f 7265 6673 720d 0a00 007d 720e 0a00  n_refsr....}r...
-0000f8a0: 0055 1069 6e64 6972 6563 745f 7461 7267  .U.indirect_targ
-0000f8b0: 6574 7372 0f0a 0000 5d72 100a 0000 5508  etsr....]r....U.
-0000f8c0: 7365 7474 696e 6773 7211 0a00 0028 6364  settingsr....(cd
-0000f8d0: 6f63 7574 696c 732e 6672 6f6e 7465 6e64  ocutils.frontend
-0000f8e0: 0a56 616c 7565 730a 7212 0a00 006f 7213  .Values.r....or.
-0000f8f0: 0a00 007d 7214 0a00 0028 5512 666f 6f74  ...}r....(U.foot
-0000f900: 6e6f 7465 5f62 6163 6b6c 696e 6b73 7215  note_backlinksr.
-0000f910: 0a00 004b 0155 1372 6563 6f72 645f 6465  ...K.U.record_de
-0000f920: 7065 6e64 656e 6369 6573 7216 0a00 004e  pendenciesr....N
-0000f930: 550d 6c61 6e67 7561 6765 5f63 6f64 6572  U.language_coder
-0000f940: 170a 0000 5502 656e 7218 0a00 0055 0974  ....U.enr....U.t
-0000f950: 7261 6365 6261 636b 7219 0a00 0088 550e  racebackr.....U.
-0000f960: 7065 705f 7265 6665 7265 6e63 6573 721a  pep_referencesr.
-0000f970: 0a00 004e 550e 7374 7269 705f 636f 6d6d  ...NU.strip_comm
-0000f980: 656e 7473 721b 0a00 004e 550d 746f 635f  entsr....NU.toc_
-0000f990: 6261 636b 6c69 6e6b 7372 1c0a 0000 5505  backlinksr....U.
-0000f9a0: 656e 7472 7972 1d0a 0000 550c 7266 635f  entryr....U.rfc_
-0000f9b0: 6261 7365 5f75 726c 721e 0a00 0055 1c68  base_urlr....U.h
-0000f9c0: 7474 7073 3a2f 2f74 6f6f 6c73 2e69 6574  ttps://tools.iet
-0000f9d0: 662e 6f72 672f 6874 6d6c 2f72 1f0a 0000  f.org/html/r....
-0000f9e0: 5509 6461 7465 7374 616d 7072 200a 0000  U.datestampr ...
-0000f9f0: 4e55 0c72 6570 6f72 745f 6c65 7665 6c72  NU.report_levelr
-0000fa00: 210a 0000 4b02 5513 736d 6172 7471 756f  !...K.U.smartquo
-0000fa10: 7465 735f 6c6f 6361 6c65 7372 220a 0000  tes_localesr"...
-0000fa20: 5d72 230a 0000 550c 5f64 6573 7469 6e61  ]r#...U._destina
-0000fa30: 7469 6f6e 7224 0a00 004e 550a 6861 6c74  tionr$...NU.halt
-0000fa40: 5f6c 6576 656c 7225 0a00 004b 0555 0d73  _levelr%...K.U.s
-0000fa50: 7472 6970 5f63 6c61 7373 6573 7226 0a00  trip_classesr&..
-0000fa60: 004e 6839 4e55 1c65 7272 6f72 5f65 6e63  .Nh9NU.error_enc
-0000fa70: 6f64 696e 675f 6572 726f 725f 6861 6e64  oding_error_hand
-0000fa80: 6c65 7272 270a 0000 5510 6261 636b 736c  lerr'...U.backsl
-0000fa90: 6173 6872 6570 6c61 6365 7228 0a00 0055  ashreplacer(...U
-0000faa0: 0564 6562 7567 7229 0a00 004e 5510 656d  .debugr)...NU.em
-0000fab0: 6265 645f 7374 796c 6573 6865 6574 722a  bed_stylesheetr*
-0000fac0: 0a00 0089 551d 6f75 7470 7574 5f65 6e63  ....U.output_enc
-0000fad0: 6f64 696e 675f 6572 726f 725f 6861 6e64  oding_error_hand
-0000fae0: 6c65 7272 2b0a 0000 5506 7374 7269 6374  lerr+...U.strict
-0000faf0: 722c 0a00 0055 0d73 6563 746e 756d 5f78  r,...U.sectnum_x
-0000fb00: 666f 726d 722d 0a00 004b 0155 0f64 756d  formr-...K.U.dum
-0000fb10: 705f 7472 616e 7366 6f72 6d73 722e 0a00  p_transformsr...
-0000fb20: 004e 550d 646f 6369 6e66 6f5f 7866 6f72  .NU.docinfo_xfor
-0000fb30: 6d72 2f0a 0000 4b01 550e 7761 726e 696e  mr/...K.U.warnin
-0000fb40: 675f 7374 7265 616d 7230 0a00 004e 5515  g_streamr0...NU.
-0000fb50: 7065 705f 6669 6c65 5f75 726c 5f74 656d  pep_file_url_tem
-0000fb60: 706c 6174 6572 310a 0000 5508 7065 702d  plater1...U.pep-
-0000fb70: 2530 3464 7232 0a00 0055 1165 7869 745f  %04dr2...U.exit_
-0000fb80: 7374 6174 7573 5f6c 6576 656c 7233 0a00  status_levelr3..
-0000fb90: 004b 0555 0663 6f6e 6669 6772 340a 0000  .K.U.configr4...
-0000fba0: 4e55 0e73 7472 6963 745f 7669 7369 746f  NU.strict_visito
-0000fbb0: 7272 350a 0000 4e55 1563 6c6f 616b 5f65  rr5...NU.cloak_e
-0000fbc0: 6d61 696c 5f61 6464 7265 7373 6573 7236  mail_addressesr6
-0000fbd0: 0a00 0088 551d 7472 696d 5f66 6f6f 746e  ....U.trim_footn
-0000fbe0: 6f74 655f 7265 6665 7265 6e63 655f 7370  ote_reference_sp
-0000fbf0: 6163 6572 370a 0000 8955 0365 6e76 7238  acer7....U.envr8
-0000fc00: 0a00 004e 550f 6475 6d70 5f70 7365 7564  ...NU.dump_pseud
-0000fc10: 6f5f 786d 6c72 390a 0000 4e55 1065 7870  o_xmlr9...NU.exp
-0000fc20: 6f73 655f 696e 7465 726e 616c 7372 3a0a  ose_internalsr:.
-0000fc30: 0000 4e55 1273 6563 7473 7562 7469 746c  ..NU.sectsubtitl
-0000fc40: 655f 7866 6f72 6d72 3b0a 0000 8955 0b73  e_xformr;....U.s
-0000fc50: 6f75 7263 655f 6c69 6e6b 723c 0a00 004e  ource_linkr<...N
-0000fc60: 550e 7266 635f 7265 6665 7265 6e63 6573  U.rfc_references
-0000fc70: 723d 0a00 004e 550f 6f75 7470 7574 5f65  r=...NU.output_e
-0000fc80: 6e63 6f64 696e 6772 3e0a 0000 5505 7574  ncodingr>...U.ut
-0000fc90: 662d 3872 3f0a 0000 550a 736f 7572 6365  f-8r?...U.source
-0000fca0: 5f75 726c 7240 0a00 004e 550e 696e 7075  _urlr@...NU.inpu
-0000fcb0: 745f 656e 636f 6469 6e67 7241 0a00 0055  t_encodingrA...U
-0000fcc0: 0975 7466 2d38 2d73 6967 7242 0a00 0055  .utf-8-sigrB...U
-0000fcd0: 0f5f 6469 7361 626c 655f 636f 6e66 6967  ._disable_config
-0000fce0: 7243 0a00 004e 5509 6964 5f70 7265 6669  rC...NU.id_prefi
-0000fcf0: 7872 440a 0000 5500 551d 6368 6172 6163  xrD...U.U.charac
-0000fd00: 7465 725f 6c65 7665 6c5f 696e 6c69 6e65  ter_level_inline
-0000fd10: 5f6d 6172 6b75 7072 450a 0000 8955 0974  _markuprE....U.t
-0000fd20: 6162 5f77 6964 7468 7246 0a00 004b 0855  ab_widthrF...K.U
-0000fd30: 0e65 7272 6f72 5f65 6e63 6f64 696e 6772  .error_encodingr
-0000fd40: 470a 0000 5505 5554 462d 3872 480a 0000  G...U.UTF-8rH...
-0000fd50: 5507 5f73 6f75 7263 6572 490a 0000 6824  U._sourcerI...h$
-0000fd60: 550f 6765 7474 6578 745f 636f 6d70 6163  U.gettext_compac
-0000fd70: 7472 4a0a 0000 8855 0967 656e 6572 6174  trJ....U.generat
-0000fd80: 6f72 724b 0a00 004e 550e 6475 6d70 5f69  orrK...NU.dump_i
-0000fd90: 6e74 6572 6e61 6c73 724c 0a00 004e 550c  nternalsrL...NU.
-0000fda0: 736d 6172 745f 7175 6f74 6573 724d 0a00  smart_quotesrM..
-0000fdb0: 0088 550c 7065 705f 6261 7365 5f75 726c  ..U.pep_base_url
-0000fdc0: 724e 0a00 0055 2068 7474 7073 3a2f 2f77  rN...U https://w
-0000fdd0: 7777 2e70 7974 686f 6e2e 6f72 672f 6465  ww.python.org/de
-0000fde0: 762f 7065 7073 2f72 4f0a 0000 5510 7379  v/peps/rO...U.sy
-0000fdf0: 6e74 6178 5f68 6967 686c 6967 6874 7250  ntax_highlightrP
-0000fe00: 0a00 0055 046c 6f6e 6772 510a 0000 551c  ...U.longrQ...U.
-0000fe10: 696e 7075 745f 656e 636f 6469 6e67 5f65  input_encoding_e
-0000fe20: 7272 6f72 5f68 616e 646c 6572 7252 0a00  rror_handlerrR..
-0000fe30: 006a 2c0a 0000 550e 6175 746f 5f69 645f  .j,...U.auto_id_
-0000fe40: 7072 6566 6978 7253 0a00 0055 0269 6472  prefixrS...U.idr
-0000fe50: 540a 0000 550e 646f 6374 6974 6c65 5f78  T...U.doctitle_x
-0000fe60: 666f 726d 7255 0a00 0089 551b 7374 7269  formrU....U.stri
-0000fe70: 705f 656c 656d 656e 7473 5f77 6974 685f  p_elements_with_
-0000fe80: 636c 6173 7365 7372 560a 0000 4e55 0d5f  classesrV...NU._
-0000fe90: 636f 6e66 6967 5f66 696c 6573 7257 0a00  config_filesrW..
-0000fea0: 005d 5516 6669 6c65 5f69 6e73 6572 7469  .]U.file_inserti
-0000feb0: 6f6e 5f65 6e61 626c 6564 7258 0a00 0088  on_enabledrX....
-0000fec0: 550b 7261 775f 656e 6162 6c65 6472 590a  U.raw_enabledrY.
-0000fed0: 0000 4b01 550d 6475 6d70 5f73 6574 7469  ..K.U.dump_setti
-0000fee0: 6e67 7372 5a0a 0000 4e75 6255 1573 796d  ngsrZ...NubU.sym
-0000fef0: 626f 6c5f 666f 6f74 6e6f 7465 5f73 7461  bol_footnote_sta
-0000ff00: 7274 725b 0a00 004b 0068 2c7d 725c 0a00  rtr[...K.h,}r\..
-0000ff10: 0028 6806 6a32 0500 0068 076a 2207 0000  .(h.j2...h.j"...
-0000ff20: 6808 6a5c 0500 0068 0c6a 4b09 0000 680a  h.j\...h.jK...h.
-0000ff30: 6a23 0900 0068 8c68 8868 166a 7d09 0000  j#...h.h.h.j}...
-0000ff40: 680d 6ac0 0500 0068 0e6a ea05 0000 680f  h.j....h.j....h.
-0000ff50: 6a8e 0500 0068 106a ab06 0000 6811 6a08  j....h.j....h.j.
-0000ff60: 0500 0068 2e68 2168 1268 e468 136a 7706  ...h.h!h.h.h.jw.
-0000ff70: 0000 6ad8 0600 006a d406 0000 6815 6ade  ..j....j....h.j.
-0000ff80: 0400 0068 176a a709 0000 7555 1273 7562  ...h.j....uU.sub
-0000ff90: 7374 6974 7574 696f 6e5f 6e61 6d65 7372  stitution_namesr
-0000ffa0: 5d0a 0000 7d72 5e0a 0000 2858 0a00 0000  ]...}r^...(X....
-0000ffb0: 6275 6666 6572 6469 6374 681a 6875 6875  bufferdicth.huhu
-0000ffc0: 5804 0000 0067 7661 7268 6075 6825 6832  X....gvarh`uh%h2
-0000ffd0: 6827 7d72 5f0a 0000 2868 295d 682c 5d68  h'}r_...(h)]h,]h
-0000ffe0: 2b5d 5506 736f 7572 6365 6824 682a 5d68  +]U.sourceh$h*]h
-0000fff0: 2f5d 7555 0966 6f6f 746e 6f74 6573 7260  /]uU.footnotesr`
-00010000: 0a00 005d 7261 0a00 0055 0672 6566 6964  ...]ra...U.refid
-00010010: 7372 620a 0000 7d72 630a 0000 7562 2e    srb...}rc...ub.
+00002d20: 696e 696d 697a 6174 696f 6e2e 6823 4e68  inimization.h#Nh
+00002d30: 314e 6832 6802 681f 6ad9 0100 0075 6265  1Nh2h.h.j....ube
+00002d40: 6825 689a 7562 6168 2555 096c 6973 745f  h%h.ubah%U.list_
+00002d50: 6974 656d 7200 0200 0075 626a d401 0000  itemr....ubj....
+00002d60: 2981 7201 0200 007d 7202 0200 0028 681e  ).r....}r....(h.
+00002d70: 5500 6827 7d72 0302 0000 2868 295d 682a  U.h'}r....(h)]h*
+00002d80: 5d68 2b5d 682c 5d68 2f5d 7568 1f6a d001  ]h+]h,]h/]uh.j..
+00002d90: 0000 6833 5d72 0402 0000 6897 2981 7205  ..h3]r....h.).r.
+00002da0: 0200 007d 7206 0200 0028 681e 5847 0000  ...}r....(h.XG..
+00002db0: 006e 2028 706f 7369 7469 7665 2069 6e74  .n (positive int
+00002dc0: 2920 2d2d 204c 656e 6774 6820 6f66 2076  ) -- Length of v
+00002dd0: 6563 746f 7220 7265 7475 726e 6564 2062  ector returned b
+00002de0: 7920 7468 6520 6669 7420 6675 6e63 7469  y the fit functi
+00002df0: 6f6e 2066 2878 292e 6827 7d72 0702 0000  on f(x).h'}r....
+00002e00: 2868 295d 682a 5d68 2b5d 682c 5d68 2f5d  (h)]h*]h+]h,]h/]
+00002e10: 7568 1f6a 0102 0000 6833 5d72 0802 0000  uh.j....h3]r....
+00002e20: 286a dd01 0000 2981 7209 0200 007d 720a  (j....).r....}r.
+00002e30: 0200 0028 681e 5801 0000 006e 6827 7d72  ...(h.X....nh'}r
+00002e40: 0b02 0000 2868 2c5d 682b 5d6a e101 0000  ....(h,]h+]j....
+00002e50: 8868 295d 682a 5d68 2f5d 7568 1f6a 0502  .h)]h*]h/]uh.j..
+00002e60: 0000 6833 5d72 0c02 0000 6852 5801 0000  ..h3]r....hRX...
+00002e70: 006e 8581 720d 0200 007d 720e 0200 0028  .n..r....}r....(
+00002e80: 681e 5500 681f 6a09 0200 0075 6261 6825  h.U.h.j....ubah%
+00002e90: 6ae6 0100 0075 6268 5258 0200 0000 2028  j....ubhRX.... (
+00002ea0: 720f 0200 0085 8172 1002 0000 7d72 1102  r......r....}r..
+00002eb0: 0000 2868 1e55 0068 1f6a 0502 0000 7562  ..(h.U.h.j....ub
+00002ec0: 683c 2981 7212 0200 007d 7213 0200 0028  h<).r....}r....(
+00002ed0: 681e 5500 6827 7d72 1402 0000 2855 0772  h.U.h'}r....(U.r
+00002ee0: 6566 7479 7065 68f2 6ae1 0100 0088 5509  eftypeh.j.....U.
+00002ef0: 7265 6674 6172 6765 7458 0c00 0000 706f  reftargetX....po
+00002f00: 7369 7469 7665 2069 6e74 7215 0200 0055  sitive intr....U
+00002f10: 0972 6566 646f 6d61 696e 68de 682c 5d68  .refdomainh.h,]h
+00002f20: 2b5d 550b 7265 6665 7870 6c69 6369 7489  +]U.refexplicit.
+00002f30: 6829 5d68 2a5d 682f 5d75 681f 6a05 0200  h)]h*]h/]uh.j...
+00002f40: 0068 335d 7216 0200 006a ef01 0000 2981  .h3]r....j....).
+00002f50: 7217 0200 007d 7218 0200 0028 681e 6a15  r....}r....(h.j.
+00002f60: 0200 0068 277d 7219 0200 0028 6829 5d68  ...h'}r....(h)]h
+00002f70: 2a5d 682b 5d68 2c5d 682f 5d75 681f 6a12  *]h+]h,]h/]uh.j.
+00002f80: 0200 0068 335d 721a 0200 0068 5258 0c00  ...h3]r....hRX..
+00002f90: 0000 706f 7369 7469 7665 2069 6e74 721b  ..positive intr.
+00002fa0: 0200 0085 8172 1c02 0000 7d72 1d02 0000  .....r....}r....
+00002fb0: 2868 1e55 0068 1f6a 1702 0000 7562 6168  (h.U.h.j....ubah
+00002fc0: 256a f701 0000 7562 6168 2568 4075 6268  %j....ubah%h@ubh
+00002fd0: 5258 0100 0000 2985 8172 1e02 0000 7d72  RX....)..r....}r
+00002fe0: 1f02 0000 2868 1e55 0068 1f6a 0502 0000  ....(h.U.h.j....
+00002ff0: 7562 6852 5805 0000 0020 e280 9320 7220  ubhRX.... ... r 
+00003000: 0200 0085 8172 2102 0000 7d72 2202 0000  .....r!...}r"...
+00003010: 2868 1e55 0068 1f6a 0502 0000 7562 6852  (h.U.h.j....ubhR
+00003020: 582e 0000 004c 656e 6774 6820 6f66 2076  X....Length of v
+00003030: 6563 746f 7220 7265 7475 726e 6564 2062  ector returned b
+00003040: 7920 7468 6520 6669 7420 6675 6e63 7469  y the fit functi
+00003050: 6f6e 2072 2302 0000 8581 7224 0200 007d  on r#.....r$...}
+00003060: 7225 0200 0028 681e 582e 0000 004c 656e  r%...(h.X....Len
+00003070: 6774 6820 6f66 2076 6563 746f 7220 7265  gth of vector re
+00003080: 7475 726e 6564 2062 7920 7468 6520 6669  turned by the fi
+00003090: 7420 6675 6e63 7469 6f6e 2068 234e 6831  t function h#Nh1
+000030a0: 4e68 3268 0268 1f6a 0502 0000 7562 684a  Nh2h.h.j....ubhJ
+000030b0: 2981 7226 0200 007d 7227 0200 0028 681e  ).r&...}r'...(h.
+000030c0: 5808 0000 0060 6066 2878 2960 6068 1f6a  X....``f(x)``h.j
+000030d0: 0502 0000 6823 4e68 2568 5668 277d 7228  ....h#Nh%hVh'}r(
+000030e0: 0200 0028 6829 5d68 2a5d 682b 5d68 2c5d  ...(h)]h*]h+]h,]
+000030f0: 682f 5d75 6831 4e68 3268 0268 335d 7229  h/]uh1Nh2h.h3]r)
+00003100: 0200 0068 5258 0400 0000 6628 7829 722a  ...hRX....f(x)r*
+00003110: 0200 0085 8172 2b02 0000 7d72 2c02 0000  .....r+...}r,...
+00003120: 2868 1e55 0068 234e 6831 4e68 3268 0268  (h.U.h#Nh1Nh2h.h
+00003130: 1f6a 2602 0000 7562 6175 6268 5258 0100  .j&...ubaubhRX..
+00003140: 0000 2e85 8172 2d02 0000 7d72 2e02 0000  .....r-...}r....
+00003150: 2868 1e58 0100 0000 2e68 234e 6831 4e68  (h.X.....h#Nh1Nh
+00003160: 3268 0268 1f6a 0502 0000 7562 6568 2568  2h.h.j....ubeh%h
+00003170: 9a75 6261 6825 6a00 0200 0075 626a d401  .ubah%j....ubj..
+00003180: 0000 2981 722f 0200 007d 7230 0200 0028  ..).r/...}r0...(
+00003190: 681e 5500 6827 7d72 3102 0000 2868 295d  h.U.h'}r1...(h)]
+000031a0: 682a 5d68 2b5d 682c 5d68 2f5d 7568 1f6a  h*]h+]h,]h/]uh.j
+000031b0: d001 0000 6833 5d72 3202 0000 6897 2981  ....h3]r2...h.).
+000031c0: 7233 0200 007d 7234 0200 0028 681e 5898  r3...}r4...(h.X.
+000031d0: 0000 0066 2028 6172 7261 792d 7661 6c75  ...f (array-valu
+000031e0: 6564 2066 756e 6374 696f 6e29 202d 2d20  ed function) -- 
+000031f0: 7375 6d5f 6920 665f 6928 7829 2a2a 3220  sum_i f_i(x)**2 
+00003200: 6973 206d 696e 696d 697a 6564 0a62 7920  is minimized.by 
+00003210: 7661 7279 696e 6720 7061 7261 6d65 7465  varying paramete
+00003220: 7273 2078 2e20 5468 6520 7061 7261 6d65  rs x. The parame
+00003230: 7465 7273 2061 7265 2061 2031 2d64 0a6e  ters are a 1-d.n
+00003240: 756d 7079 2061 7272 6179 206f 6620 6569  umpy array of ei
+00003250: 7468 6572 206e 756d 6265 7273 206f 7220  ther numbers or 
+00003260: 6776 6172 2e47 5661 7273 2e68 277d 7235  gvar.GVars.h'}r5
+00003270: 0200 0028 6829 5d68 2a5d 682b 5d68 2c5d  ...(h)]h*]h+]h,]
+00003280: 682f 5d75 681f 6a2f 0200 0068 335d 7236  h/]uh.j/...h3]r6
+00003290: 0200 0028 6add 0100 0029 8172 3702 0000  ...(j....).r7...
+000032a0: 7d72 3802 0000 2868 1e58 0100 0000 6668  }r8...(h.X....fh
+000032b0: 277d 7239 0200 0028 682c 5d68 2b5d 6ae1  '}r9...(h,]h+]j.
+000032c0: 0100 0088 6829 5d68 2a5d 682f 5d75 681f  ....h)]h*]h/]uh.
+000032d0: 6a33 0200 0068 335d 723a 0200 0068 5258  j3...h3]r:...hRX
+000032e0: 0100 0000 6685 8172 3b02 0000 7d72 3c02  ....f..r;...}r<.
+000032f0: 0000 2868 1e55 0068 1f6a 3702 0000 7562  ..(h.U.h.j7...ub
+00003300: 6168 256a e601 0000 7562 6852 5802 0000  ah%j....ubhRX...
+00003310: 0020 2872 3d02 0000 8581 723e 0200 007d  . (r=.....r>...}
+00003320: 723f 0200 0028 681e 5500 681f 6a33 0200  r?...(h.U.h.j3..
+00003330: 0075 6268 3c29 8172 4002 0000 7d72 4102  .ubh<).r@...}rA.
+00003340: 0000 2868 1e55 0068 277d 7242 0200 0028  ..(h.U.h'}rB...(
+00003350: 5507 7265 6674 7970 6568 f26a e101 0000  U.reftypeh.j....
+00003360: 8855 0972 6566 7461 7267 6574 5815 0000  .U.reftargetX...
+00003370: 0061 7272 6179 2d76 616c 7565 6420 6675  .array-valued fu
+00003380: 6e63 7469 6f6e 7243 0200 0055 0972 6566  nctionrC...U.ref
+00003390: 646f 6d61 696e 68de 682c 5d68 2b5d 550b  domainh.h,]h+]U.
+000033a0: 7265 6665 7870 6c69 6369 7489 6829 5d68  refexplicit.h)]h
+000033b0: 2a5d 682f 5d75 681f 6a33 0200 0068 335d  *]h/]uh.j3...h3]
+000033c0: 7244 0200 006a ef01 0000 2981 7245 0200  rD...j....).rE..
+000033d0: 007d 7246 0200 0028 681e 6a43 0200 0068  .}rF...(h.jC...h
+000033e0: 277d 7247 0200 0028 6829 5d68 2a5d 682b  '}rG...(h)]h*]h+
+000033f0: 5d68 2c5d 682f 5d75 681f 6a40 0200 0068  ]h,]h/]uh.j@...h
+00003400: 335d 7248 0200 0068 5258 1500 0000 6172  3]rH...hRX....ar
+00003410: 7261 792d 7661 6c75 6564 2066 756e 6374  ray-valued funct
+00003420: 696f 6e72 4902 0000 8581 724a 0200 007d  ionrI.....rJ...}
+00003430: 724b 0200 0028 681e 5500 681f 6a45 0200  rK...(h.U.h.jE..
+00003440: 0075 6261 6825 6af7 0100 0075 6261 6825  .ubah%j....ubah%
+00003450: 6840 7562 6852 5801 0000 0029 8581 724c  h@ubhRX....)..rL
+00003460: 0200 007d 724d 0200 0028 681e 5500 681f  ...}rM...(h.U.h.
+00003470: 6a33 0200 0075 6268 5258 0500 0000 20e2  j3...ubhRX.... .
+00003480: 8093 2072 4e02 0000 8581 724f 0200 007d  .. rN.....rO...}
+00003490: 7250 0200 0028 681e 5500 681f 6a33 0200  rP...(h.U.h.j3..
+000034a0: 0075 6268 4a29 8172 5102 0000 7d72 5202  .ubhJ).rQ...}rR.
+000034b0: 0000 2868 1e58 1300 0000 6060 7375 6d5f  ..(h.X....``sum_
+000034c0: 6920 665f 6928 7829 2a2a 3260 6068 1f6a  i f_i(x)**2``h.j
+000034d0: 3302 0000 6823 4e68 2568 5668 277d 7253  3...h#Nh%hVh'}rS
+000034e0: 0200 0028 6829 5d68 2a5d 682b 5d68 2c5d  ...(h)]h*]h+]h,]
+000034f0: 682f 5d75 6831 4e68 3268 0268 335d 7254  h/]uh1Nh2h.h3]rT
+00003500: 0200 0068 5258 0f00 0000 7375 6d5f 6920  ...hRX....sum_i 
+00003510: 665f 6928 7829 2a2a 3272 5502 0000 8581  f_i(x)**2rU.....
+00003520: 7256 0200 007d 7257 0200 0028 681e 5500  rV...}rW...(h.U.
+00003530: 6823 4e68 314e 6832 6802 681f 6a51 0200  h#Nh1Nh2h.h.jQ..
+00003540: 0075 6261 7562 6852 5824 0000 0020 6973  .ubaubhRX$... is
+00003550: 206d 696e 696d 697a 6564 0a62 7920 7661   minimized.by va
+00003560: 7279 696e 6720 7061 7261 6d65 7465 7273  rying parameters
+00003570: 2072 5802 0000 8581 7259 0200 007d 725a   rX.....rY...}rZ
+00003580: 0200 0028 681e 5824 0000 0020 6973 206d  ...(h.X$... is m
+00003590: 696e 696d 697a 6564 0a62 7920 7661 7279  inimized.by vary
+000035a0: 696e 6720 7061 7261 6d65 7465 7273 2068  ing parameters h
+000035b0: 234e 6831 4e68 3268 0268 1f6a 3302 0000  #Nh1Nh2h.h.j3...
+000035c0: 7562 684a 2981 725b 0200 007d 725c 0200  ubhJ).r[...}r\..
+000035d0: 0028 681e 5805 0000 0060 6078 6060 681f  .(h.X....``x``h.
+000035e0: 6a33 0200 0068 234e 6825 6856 6827 7d72  j3...h#Nh%hVh'}r
+000035f0: 5d02 0000 2868 295d 682a 5d68 2b5d 682c  ]...(h)]h*]h+]h,
+00003600: 5d68 2f5d 7568 314e 6832 6802 6833 5d72  ]h/]uh1Nh2h.h3]r
+00003610: 5e02 0000 6852 5801 0000 0078 8581 725f  ^...hRX....x..r_
+00003620: 0200 007d 7260 0200 0028 681e 5500 6823  ...}r`...(h.U.h#
+00003630: 4e68 314e 6832 6802 681f 6a5b 0200 0075  Nh1Nh2h.h.j[...u
+00003640: 6261 7562 6852 581b 0000 002e 2054 6865  baubhRX..... The
+00003650: 2070 6172 616d 6574 6572 7320 6172 6520   parameters are 
+00003660: 6120 312d 640a 7261 0200 0085 8172 6202  a 1-d.ra.....rb.
+00003670: 0000 7d72 6302 0000 2868 1e58 1b00 0000  ..}rc...(h.X....
+00003680: 2e20 5468 6520 7061 7261 6d65 7465 7273  . The parameters
+00003690: 2061 7265 2061 2031 2d64 0a68 234e 6831   are a 1-d.h#Nh1
+000036a0: 4e68 3268 0268 1f6a 3302 0000 7562 683c  Nh2h.h.j3...ubh<
+000036b0: 2981 7264 0200 007d 7265 0200 0028 681e  ).rd...}re...(h.
+000036c0: 580e 0000 003a 636c 6173 733a 606e 756d  X....:class:`num
+000036d0: 7079 6072 6602 0000 681f 6a33 0200 0068  py`rf...h.j3...h
+000036e0: 236a 5901 0000 6825 6840 6827 7d72 6702  #jY...h%h@h'}rg.
+000036f0: 0000 2855 0772 6566 7479 7065 5805 0000  ..(U.reftypeX...
+00003700: 0063 6c61 7373 6842 8968 4358 0500 0000  .classhB.hCX....
+00003710: 6e75 6d70 7955 0972 6566 646f 6d61 696e  numpyU.refdomain
+00003720: 5802 0000 0070 7972 6802 0000 682c 5d68  X....pyrh...h,]h
+00003730: 2b5d 550b 7265 6665 7870 6c69 6369 7489  +]U.refexplicit.
+00003740: 6829 5d68 2a5d 682f 5d68 4568 4668 4768  h)]h*]h/]hEhFhGh
+00003750: f168 4868 ed75 6831 4b0d 6832 6802 6833  .hHh.uh1K.h2h.h3
+00003760: 5d72 6902 0000 684a 2981 726a 0200 007d  ]ri...hJ).rj...}
+00003770: 726b 0200 0028 681e 6a66 0200 0068 277d  rk...(h.jf...h'}
+00003780: 726c 0200 0028 6829 5d68 2a5d 726d 0200  rl...(h)]h*]rm..
+00003790: 0028 684f 6a68 0200 0058 0800 0000 7079  .(hOjh...X....py
+000037a0: 2d63 6c61 7373 726e 0200 0065 682b 5d68  -classrn...eh+]h
+000037b0: 2c5d 682f 5d75 681f 6a64 0200 0068 335d  ,]h/]uh.jd...h3]
+000037c0: 726f 0200 0068 5258 0500 0000 6e75 6d70  ro...hRX....nump
+000037d0: 7972 7002 0000 8581 7271 0200 007d 7272  yrp.....rq...}rr
+000037e0: 0200 0028 681e 5500 681f 6a6a 0200 0075  ...(h.U.h.jj...u
+000037f0: 6261 6825 6856 7562 6175 6268 5258 1c00  bah%hVubaubhRX..
+00003800: 0000 2061 7272 6179 206f 6620 6569 7468  .. array of eith
+00003810: 6572 206e 756d 6265 7273 206f 7220 7273  er numbers or rs
+00003820: 0200 0085 8172 7402 0000 7d72 7502 0000  .....rt...}ru...
+00003830: 2868 1e58 1c00 0000 2061 7272 6179 206f  (h.X.... array o
+00003840: 6620 6569 7468 6572 206e 756d 6265 7273  f either numbers
+00003850: 206f 7220 6823 4e68 314e 6832 6802 681f   or h#Nh1Nh2h.h.
+00003860: 6a33 0200 0075 6268 3c29 8172 7602 0000  j3...ubh<).rv...
+00003870: 7d72 7702 0000 2868 1e58 1200 0000 3a63  }rw...(h.X....:c
+00003880: 6c61 7373 3a60 6776 6172 2e47 5661 7260  lass:`gvar.GVar`
+00003890: 7278 0200 0068 1f6a 3302 0000 6823 6a59  rx...h.j3...h#jY
+000038a0: 0100 0068 2568 4068 277d 7279 0200 0028  ...h%h@h'}ry...(
+000038b0: 5507 7265 6674 7970 6558 0500 0000 636c  U.reftypeX....cl
+000038c0: 6173 7368 4289 6843 5809 0000 0067 7661  asshB.hCX....gva
+000038d0: 722e 4756 6172 5509 7265 6664 6f6d 6169  r.GVarU.refdomai
+000038e0: 6e58 0200 0000 7079 727a 0200 0068 2c5d  nX....pyrz...h,]
+000038f0: 682b 5d55 0b72 6566 6578 706c 6963 6974  h+]U.refexplicit
+00003900: 8968 295d 682a 5d68 2f5d 6845 6846 6847  .h)]h*]h/]hEhFhG
+00003910: 68f1 6848 68ed 7568 314b 0d68 3268 0268  h.hHh.uh1K.h2h.h
+00003920: 335d 727b 0200 0068 4a29 8172 7c02 0000  3]r{...hJ).r|...
+00003930: 7d72 7d02 0000 2868 1e6a 7802 0000 6827  }r}...(h.jx...h'
+00003940: 7d72 7e02 0000 2868 295d 682a 5d72 7f02  }r~...(h)]h*]r..
+00003950: 0000 2868 4f6a 7a02 0000 5808 0000 0070  ..(hOjz...X....p
+00003960: 792d 636c 6173 7372 8002 0000 6568 2b5d  y-classr....eh+]
+00003970: 682c 5d68 2f5d 7568 1f6a 7602 0000 6833  h,]h/]uh.jv...h3
+00003980: 5d72 8102 0000 6852 5809 0000 0067 7661  ]r....hRX....gva
+00003990: 722e 4756 6172 7282 0200 0085 8172 8302  r.GVarr......r..
+000039a0: 0000 7d72 8402 0000 2868 1e55 0068 1f6a  ..}r....(h.U.h.j
+000039b0: 7c02 0000 7562 6168 2568 5675 6261 7562  |...ubah%hVubaub
+000039c0: 6852 5802 0000 0073 2e72 8502 0000 8581  hRX....s.r......
+000039d0: 7286 0200 007d 7287 0200 0028 681e 5803  r....}r....(h.X.
+000039e0: 0000 005c 732e 6823 4e68 314e 6832 6802  ...\s.h#Nh1Nh2h.
+000039f0: 681f 6a33 0200 0075 6265 6825 689a 7562  h.j3...ubeh%h.ub
+00003a00: 6168 256a 0002 0000 7562 6ad4 0100 0029  ah%j....ubj....)
+00003a10: 8172 8802 0000 7d72 8902 0000 2868 1e55  .r....}r....(h.U
+00003a20: 0068 277d 728a 0200 0028 6829 5d68 2a5d  .h'}r....(h)]h*]
+00003a30: 682b 5d68 2c5d 682f 5d75 681f 6ad0 0100  h+]h,]h/]uh.j...
+00003a40: 0068 335d 728b 0200 0068 9729 8172 8c02  .h3]r....h.).r..
+00003a50: 0000 7d72 8d02 0000 2868 1e58 b102 0000  ..}r....(h.X....
+00003a60: 746f 6c20 2866 6c6f 6174 206f 7220 7475  tol (float or tu
+00003a70: 706c 6529 202d 2d20 4173 7369 676e 696e  ple) -- Assignin
+00003a80: 6720 746f 6c3d 2878 746f 6c2c 2067 746f  g tol=(xtol, gto
+00003a90: 6c2c 2066 746f 6c29 2063 6175 7365 7320  l, ftol) causes 
+00003aa0: 7468 650a 6669 7420 746f 2073 746f 7020  the.fit to stop 
+00003ab0: 7365 6172 6368 696e 6720 666f 7220 6120  searching for a 
+00003ac0: 6d69 6e69 6d75 6d20 7768 656e 2061 6e79  minimum when any
+00003ad0: 206f 6678 746f 6c20 3e3d 2072 656c 6174   ofxtol >= relat
+00003ae0: 6976 6520 6368 616e 6765 2069 6e20 7061  ive change in pa
+00003af0: 7261 6d65 7465 7273 2062 6574 7765 656e  rameters between
+00003b00: 2069 7465 7261 7469 6f6e 730a 0a67 746f   iterations..gto
+00003b10: 6c20 3e3d 2072 656c 6174 6976 6520 7369  l >= relative si
+00003b20: 7a65 206f 6620 6772 6164 6965 6e74 206f  ze of gradient o
+00003b30: 6620 6368 692a 2a32 0a0a 6674 6f6c 203e  f chi**2..ftol >
+00003b40: 3d20 7265 6c61 7469 7665 2063 6861 6e67  = relative chang
+00003b50: 6520 696e 2063 6869 2a2a 3220 6265 7477  e in chi**2 betw
+00003b60: 6565 6e20 6974 6572 6174 696f 6e73 6973  een iterationsis
+00003b70: 2073 7461 7469 7366 6965 642e 2053 6565   statisfied. See
+00003b80: 2074 6865 2073 6369 7079 2e6f 7074 696d   the scipy.optim
+00003b90: 697a 652e 6c65 6173 745f 7371 7561 7265  ize.least_square
+00003ba0: 730a 646f 6375 6d65 6e74 6174 696f 6e20  s.documentation 
+00003bb0: 6465 7461 696c 6564 2064 6566 696e 6974  detailed definit
+00003bc0: 696f 6e73 206f 6620 7468 6520 7374 6f70  ions of the stop
+00003bd0: 7069 6e67 2063 6f6e 6469 7469 6f6e 732e  ping conditions.
+00003be0: 0a54 7970 6963 616c 6c79 206f 6e65 2073  .Typically one s
+00003bf0: 6574 7320 7874 6f6c 3d31 2f31 302a 2a64  ets xtol=1/10**d
+00003c00: 2077 6865 7265 2064 2069 7320 7468 6520   where d is the 
+00003c10: 6e75 6d62 6572 206f 660a 6469 6769 7473  number of.digits
+00003c20: 206f 6620 7072 6563 6973 696f 6e20 6465   of precision de
+00003c30: 7369 7265 6420 696e 2074 6865 2072 6573  sired in the res
+00003c40: 756c 742c 2077 6869 6c65 2067 746f 6c3c  ult, while gtol<
+00003c50: 3c31 2061 6e64 0a66 746f 6c3c 3c31 2e20  <1 and.ftol<<1. 
+00003c60: 5365 7474 696e 6720 746f 6c3d 6570 7320  Setting tol=eps 
+00003c70: 7768 6572 6520 6570 7320 6973 2061 206e  where eps is a n
+00003c80: 756d 6265 7220 6973 0a65 7175 6976 616c  umber is.equival
+00003c90: 656e 7420 746f 2073 6574 7469 6e67 2074  ent to setting t
+00003ca0: 6f6c 3d28 6570 732c 3165 2d31 302c 3165  ol=(eps,1e-10,1e
+00003cb0: 2d31 3029 2e20 5365 7474 696e 670a 746f  -10). Setting.to
+00003cc0: 6c3d 2865 7073 312c 6570 7332 2920 6973  l=(eps1,eps2) is
+00003cd0: 2065 7175 6976 6c65 6e74 2074 6f20 7365   equivlent to se
+00003ce0: 7474 696e 670a 746f 6c3d 2865 7073 312c  tting.tol=(eps1,
+00003cf0: 6570 7332 2c31 652d 3130 292e 2044 6566  eps2,1e-10). Def
+00003d00: 6175 6c74 2069 7320 746f 6c3d 3165 2d35  ault is tol=1e-5
+00003d10: 2e68 277d 728e 0200 0028 6829 5d68 2a5d  .h'}r....(h)]h*]
+00003d20: 682b 5d68 2c5d 682f 5d75 681f 6a88 0200  h+]h,]h/]uh.j...
+00003d30: 0068 335d 728f 0200 0028 6add 0100 0029  .h3]r....(j....)
+00003d40: 8172 9002 0000 7d72 9102 0000 2868 1e58  .r....}r....(h.X
+00003d50: 0300 0000 746f 6c68 277d 7292 0200 0028  ....tolh'}r....(
+00003d60: 682c 5d68 2b5d 6ae1 0100 0088 6829 5d68  h,]h+]j.....h)]h
+00003d70: 2a5d 682f 5d75 681f 6a8c 0200 0068 335d  *]h/]uh.j....h3]
+00003d80: 7293 0200 0068 5258 0300 0000 746f 6c72  r....hRX....tolr
+00003d90: 9402 0000 8581 7295 0200 007d 7296 0200  ......r....}r...
+00003da0: 0028 681e 5500 681f 6a90 0200 0075 6261  .(h.U.h.j....uba
+00003db0: 6825 6ae6 0100 0075 6268 5258 0200 0000  h%j....ubhRX....
+00003dc0: 2028 7297 0200 0085 8172 9802 0000 7d72   (r......r....}r
+00003dd0: 9902 0000 2868 1e55 0068 1f6a 8c02 0000  ....(h.U.h.j....
+00003de0: 7562 683c 2981 729a 0200 007d 729b 0200  ubh<).r....}r...
+00003df0: 0028 681e 5500 6827 7d72 9c02 0000 2855  .(h.U.h'}r....(U
+00003e00: 0772 6566 7479 7065 68f2 6ae1 0100 0088  .reftypeh.j.....
+00003e10: 5509 7265 6674 6172 6765 7458 0500 0000  U.reftargetX....
+00003e20: 666c 6f61 7472 9d02 0000 5509 7265 6664  floatr....U.refd
+00003e30: 6f6d 6169 6e68 de68 2c5d 682b 5d55 0b72  omainh.h,]h+]U.r
+00003e40: 6566 6578 706c 6963 6974 8968 295d 682a  efexplicit.h)]h*
+00003e50: 5d68 2f5d 7568 1f6a 8c02 0000 6833 5d72  ]h/]uh.j....h3]r
+00003e60: 9e02 0000 6aef 0100 0029 8172 9f02 0000  ....j....).r....
+00003e70: 7d72 a002 0000 2868 1e6a 9d02 0000 6827  }r....(h.j....h'
+00003e80: 7d72 a102 0000 2868 295d 682a 5d68 2b5d  }r....(h)]h*]h+]
+00003e90: 682c 5d68 2f5d 7568 1f6a 9a02 0000 6833  h,]h/]uh.j....h3
+00003ea0: 5d72 a202 0000 6852 5805 0000 0066 6c6f  ]r....hRX....flo
+00003eb0: 6174 72a3 0200 0085 8172 a402 0000 7d72  atr......r....}r
+00003ec0: a502 0000 2868 1e55 0068 1f6a 9f02 0000  ....(h.U.h.j....
+00003ed0: 7562 6168 256a f701 0000 7562 6168 2568  ubah%j....ubah%h
+00003ee0: 4075 626a ef01 0000 2981 72a6 0200 007d  @ubj....).r....}
+00003ef0: 72a7 0200 0028 681e 5804 0000 0020 6f72  r....(h.X.... or
+00003f00: 2068 277d 72a8 0200 0028 6829 5d68 2a5d   h'}r....(h)]h*]
+00003f10: 682b 5d68 2c5d 682f 5d75 681f 6a8c 0200  h+]h,]h/]uh.j...
+00003f20: 0068 335d 72a9 0200 0068 5258 0400 0000  .h3]r....hRX....
+00003f30: 206f 7220 72aa 0200 0085 8172 ab02 0000   or r......r....
+00003f40: 7d72 ac02 0000 2868 1e55 0068 1f6a a602  }r....(h.U.h.j..
+00003f50: 0000 7562 6168 256a f701 0000 7562 683c  ..ubah%j....ubh<
+00003f60: 2981 72ad 0200 007d 72ae 0200 0028 681e  ).r....}r....(h.
+00003f70: 5500 6827 7d72 af02 0000 2855 0772 6566  U.h'}r....(U.ref
+00003f80: 7479 7065 68f2 6ae1 0100 0088 5509 7265  typeh.j.....U.re
+00003f90: 6674 6172 6765 7458 0500 0000 7475 706c  ftargetX....tupl
+00003fa0: 6572 b002 0000 5509 7265 6664 6f6d 6169  er....U.refdomai
+00003fb0: 6e68 de68 2c5d 682b 5d55 0b72 6566 6578  nh.h,]h+]U.refex
+00003fc0: 706c 6963 6974 8968 295d 682a 5d68 2f5d  plicit.h)]h*]h/]
+00003fd0: 7568 1f6a 8c02 0000 6833 5d72 b102 0000  uh.j....h3]r....
+00003fe0: 6aef 0100 0029 8172 b202 0000 7d72 b302  j....).r....}r..
+00003ff0: 0000 2868 1e6a b002 0000 6827 7d72 b402  ..(h.j....h'}r..
+00004000: 0000 2868 295d 682a 5d68 2b5d 682c 5d68  ..(h)]h*]h+]h,]h
+00004010: 2f5d 7568 1f6a ad02 0000 6833 5d72 b502  /]uh.j....h3]r..
+00004020: 0000 6852 5805 0000 0074 7570 6c65 72b6  ..hRX....tupler.
+00004030: 0200 0085 8172 b702 0000 7d72 b802 0000  .....r....}r....
+00004040: 2868 1e55 0068 1f6a b202 0000 7562 6168  (h.U.h.j....ubah
+00004050: 256a f701 0000 7562 6168 2568 4075 6268  %j....ubah%h@ubh
+00004060: 5258 0100 0000 2985 8172 b902 0000 7d72  RX....)..r....}r
+00004070: ba02 0000 2868 1e55 0068 1f6a 8c02 0000  ....(h.U.h.j....
+00004080: 7562 6852 5805 0000 0020 e280 9320 72bb  ubhRX.... ... r.
+00004090: 0200 0085 8172 bc02 0000 7d72 bd02 0000  .....r....}r....
+000040a0: 2868 1e55 0068 1f6a 8c02 0000 7562 6897  (h.U.h.j....ubh.
+000040b0: 2981 72be 0200 007d 72bf 0200 0028 681e  ).r....}r....(h.
+000040c0: 585f 0000 0041 7373 6967 6e69 6e67 2060  X_...Assigning `
+000040d0: 6074 6f6c 3d28 7874 6f6c 2c20 6774 6f6c  `tol=(xtol, gtol
+000040e0: 2c20 6674 6f6c 2960 6020 6361 7573 6573  , ftol)`` causes
+000040f0: 2074 6865 0a66 6974 2074 6f20 7374 6f70   the.fit to stop
+00004100: 2073 6561 7263 6869 6e67 2066 6f72 2061   searching for a
+00004110: 206d 696e 696d 756d 2077 6865 6e20 616e   minimum when an
+00004120: 7920 6f66 681f 6a8c 0200 0068 236a 5901  y ofh.j....h#jY.
+00004130: 0000 6825 689a 6827 7d72 c002 0000 2868  ..h%h.h'}r....(h
+00004140: 295d 682a 5d68 2b5d 682c 5d68 2f5d 7568  )]h*]h+]h,]h/]uh
+00004150: 314b 1168 3268 0268 335d 72c1 0200 0028  1K.h2h.h3]r....(
+00004160: 6852 580a 0000 0041 7373 6967 6e69 6e67  hRX....Assigning
+00004170: 2072 c202 0000 8581 72c3 0200 007d 72c4   r......r....}r.
+00004180: 0200 0028 681e 580a 0000 0041 7373 6967  ...(h.X....Assig
+00004190: 6e69 6e67 2068 234e 6831 4e68 3268 0268  ning h#Nh1Nh2h.h
+000041a0: 1f6a be02 0000 7562 684a 2981 72c5 0200  .j....ubhJ).r...
+000041b0: 007d 72c6 0200 0028 681e 581a 0000 0060  .}r....(h.X....`
+000041c0: 6074 6f6c 3d28 7874 6f6c 2c20 6774 6f6c  `tol=(xtol, gtol
+000041d0: 2c20 6674 6f6c 2960 6068 277d 72c7 0200  , ftol)``h'}r...
+000041e0: 0028 6829 5d68 2a5d 682b 5d68 2c5d 682f  .(h)]h*]h+]h,]h/
+000041f0: 5d75 681f 6abe 0200 0068 335d 72c8 0200  ]uh.j....h3]r...
+00004200: 0068 5258 1600 0000 746f 6c3d 2878 746f  .hRX....tol=(xto
+00004210: 6c2c 2067 746f 6c2c 2066 746f 6c29 72c9  l, gtol, ftol)r.
+00004220: 0200 0085 8172 ca02 0000 7d72 cb02 0000  .....r....}r....
+00004230: 2868 1e55 0068 1f6a c502 0000 7562 6168  (h.U.h.j....ubah
+00004240: 2568 5675 6268 5258 3b00 0000 2063 6175  %hVubhRX;... cau
+00004250: 7365 7320 7468 650a 6669 7420 746f 2073  ses the.fit to s
+00004260: 746f 7020 7365 6172 6368 696e 6720 666f  top searching fo
+00004270: 7220 6120 6d69 6e69 6d75 6d20 7768 656e  r a minimum when
+00004280: 2061 6e79 206f 6672 cc02 0000 8581 72cd   any ofr......r.
+00004290: 0200 007d 72ce 0200 0028 681e 583b 0000  ...}r....(h.X;..
+000042a0: 0020 6361 7573 6573 2074 6865 0a66 6974  . causes the.fit
+000042b0: 2074 6f20 7374 6f70 2073 6561 7263 6869   to stop searchi
+000042c0: 6e67 2066 6f72 2061 206d 696e 696d 756d  ng for a minimum
+000042d0: 2077 6865 6e20 616e 7920 6f66 6823 4e68   when any ofh#Nh
+000042e0: 314e 6832 6802 681f 6abe 0200 0075 6265  1Nh2h.h.j....ube
+000042f0: 7562 6364 6f63 7574 696c 732e 6e6f 6465  ubcdocutils.node
+00004300: 730a 626c 6f63 6b5f 7175 6f74 650a 72cf  s.block_quote.r.
+00004310: 0200 0029 8172 d002 0000 7d72 d102 0000  ...).r....}r....
+00004320: 2868 1e55 0068 1f6a 8c02 0000 6823 4e68  (h.U.h.j....h#Nh
+00004330: 2555 0b62 6c6f 636b 5f71 756f 7465 72d2  %U.block_quoter.
+00004340: 0200 0068 277d 72d3 0200 0028 6829 5d68  ...h'}r....(h)]h
+00004350: 2a5d 682b 5d68 2c5d 682f 5d75 6831 4e68  *]h+]h,]h/]uh1Nh
+00004360: 3268 0268 335d 72d4 0200 0028 6897 2981  2h.h3]r....(h.).
+00004370: 72d5 0200 007d 72d6 0200 0028 681e 583c  r....}r....(h.X<
+00004380: 0000 0060 6078 746f 6c20 3e3d 6060 2072  ...``xtol >=`` r
+00004390: 656c 6174 6976 6520 6368 616e 6765 2069  elative change i
+000043a0: 6e20 7061 7261 6d65 7465 7273 2062 6574  n parameters bet
+000043b0: 7765 656e 2069 7465 7261 7469 6f6e 7368  ween iterationsh
+000043c0: 1f6a d002 0000 6823 6a59 0100 0068 2568  .j....h#jY...h%h
+000043d0: 9a68 277d 72d7 0200 0028 6829 5d68 2a5d  .h'}r....(h)]h*]
+000043e0: 682b 5d68 2c5d 682f 5d75 6831 4b14 6833  h+]h,]h/]uh1K.h3
+000043f0: 5d72 d802 0000 2868 4a29 8172 d902 0000  ]r....(hJ).r....
+00004400: 7d72 da02 0000 2868 1e58 0b00 0000 6060  }r....(h.X....``
+00004410: 7874 6f6c 203e 3d60 6068 277d 72db 0200  xtol >=``h'}r...
+00004420: 0028 6829 5d68 2a5d 682b 5d68 2c5d 682f  .(h)]h*]h+]h,]h/
+00004430: 5d75 681f 6ad5 0200 0068 335d 72dc 0200  ]uh.j....h3]r...
+00004440: 0068 5258 0700 0000 7874 6f6c 203e 3d72  .hRX....xtol >=r
+00004450: dd02 0000 8581 72de 0200 007d 72df 0200  ......r....}r...
+00004460: 0028 681e 5500 681f 6ad9 0200 0075 6261  .(h.U.h.j....uba
+00004470: 6825 6856 7562 6852 5831 0000 0020 7265  h%hVubhRX1... re
+00004480: 6c61 7469 7665 2063 6861 6e67 6520 696e  lative change in
+00004490: 2070 6172 616d 6574 6572 7320 6265 7477   parameters betw
+000044a0: 6565 6e20 6974 6572 6174 696f 6e73 72e0  een iterationsr.
+000044b0: 0200 0085 8172 e102 0000 7d72 e202 0000  .....r....}r....
+000044c0: 2868 1e58 3100 0000 2072 656c 6174 6976  (h.X1... relativ
+000044d0: 6520 6368 616e 6765 2069 6e20 7061 7261  e change in para
+000044e0: 6d65 7465 7273 2062 6574 7765 656e 2069  meters between i
+000044f0: 7465 7261 7469 6f6e 7368 1f6a d502 0000  terationsh.j....
+00004500: 7562 6575 6268 9729 8172 e302 0000 7d72  ubeubh.).r....}r
+00004510: e402 0000 2868 1e58 3300 0000 6060 6774  ....(h.X3...``gt
+00004520: 6f6c 203e 3d60 6020 7265 6c61 7469 7665  ol >=`` relative
+00004530: 2073 697a 6520 6f66 2067 7261 6469 656e   size of gradien
+00004540: 7420 6f66 2060 6063 6869 2a2a 3260 6068  t of ``chi**2``h
+00004550: 1f6a d002 0000 6823 6a59 0100 0068 2568  .j....h#jY...h%h
+00004560: 9a68 277d 72e5 0200 0028 6829 5d68 2a5d  .h'}r....(h)]h*]
+00004570: 682b 5d68 2c5d 682f 5d75 6831 4b16 6833  h+]h,]h/]uh1K.h3
+00004580: 5d72 e602 0000 2868 4a29 8172 e702 0000  ]r....(hJ).r....
+00004590: 7d72 e802 0000 2868 1e58 0b00 0000 6060  }r....(h.X....``
+000045a0: 6774 6f6c 203e 3d60 6068 277d 72e9 0200  gtol >=``h'}r...
+000045b0: 0028 6829 5d68 2a5d 682b 5d68 2c5d 682f  .(h)]h*]h+]h,]h/
+000045c0: 5d75 681f 6ae3 0200 0068 335d 72ea 0200  ]uh.j....h3]r...
+000045d0: 0068 5258 0700 0000 6774 6f6c 203e 3d72  .hRX....gtol >=r
+000045e0: eb02 0000 8581 72ec 0200 007d 72ed 0200  ......r....}r...
+000045f0: 0028 681e 5500 681f 6ae7 0200 0075 6261  .(h.U.h.j....uba
+00004600: 6825 6856 7562 6852 581e 0000 0020 7265  h%hVubhRX.... re
+00004610: 6c61 7469 7665 2073 697a 6520 6f66 2067  lative size of g
+00004620: 7261 6469 656e 7420 6f66 2072 ee02 0000  radient of r....
+00004630: 8581 72ef 0200 007d 72f0 0200 0028 681e  ..r....}r....(h.
+00004640: 581e 0000 0020 7265 6c61 7469 7665 2073  X.... relative s
+00004650: 697a 6520 6f66 2067 7261 6469 656e 7420  ize of gradient 
+00004660: 6f66 2068 1f6a e302 0000 7562 684a 2981  of h.j....ubhJ).
+00004670: 72f1 0200 007d 72f2 0200 0028 681e 580a  r....}r....(h.X.
+00004680: 0000 0060 6063 6869 2a2a 3260 6068 277d  ...``chi**2``h'}
+00004690: 72f3 0200 0028 6829 5d68 2a5d 682b 5d68  r....(h)]h*]h+]h
+000046a0: 2c5d 682f 5d75 681f 6ae3 0200 0068 335d  ,]h/]uh.j....h3]
+000046b0: 72f4 0200 0068 5258 0600 0000 6368 692a  r....hRX....chi*
+000046c0: 2a32 72f5 0200 0085 8172 f602 0000 7d72  *2r......r....}r
+000046d0: f702 0000 2868 1e55 0068 1f6a f102 0000  ....(h.U.h.j....
+000046e0: 7562 6168 2568 5675 6265 7562 6897 2981  ubah%hVubeubh.).
+000046f0: 72f8 0200 007d 72f9 0200 0028 681e 583c  r....}r....(h.X<
+00004700: 0000 0060 6066 746f 6c20 3e3d 6060 2072  ...``ftol >=`` r
+00004710: 656c 6174 6976 6520 6368 616e 6765 2069  elative change i
+00004720: 6e20 6060 6368 692a 2a32 6060 2062 6574  n ``chi**2`` bet
+00004730: 7765 656e 2069 7465 7261 7469 6f6e 7368  ween iterationsh
+00004740: 1f6a d002 0000 6823 6a59 0100 0068 2568  .j....h#jY...h%h
+00004750: 9a68 277d 72fa 0200 0028 6829 5d68 2a5d  .h'}r....(h)]h*]
+00004760: 682b 5d68 2c5d 682f 5d75 6831 4b18 6833  h+]h,]h/]uh1K.h3
+00004770: 5d72 fb02 0000 2868 4a29 8172 fc02 0000  ]r....(hJ).r....
+00004780: 7d72 fd02 0000 2868 1e58 0b00 0000 6060  }r....(h.X....``
+00004790: 6674 6f6c 203e 3d60 6068 277d 72fe 0200  ftol >=``h'}r...
+000047a0: 0028 6829 5d68 2a5d 682b 5d68 2c5d 682f  .(h)]h*]h+]h,]h/
+000047b0: 5d75 681f 6af8 0200 0068 335d 72ff 0200  ]uh.j....h3]r...
+000047c0: 0068 5258 0700 0000 6674 6f6c 203e 3d72  .hRX....ftol >=r
+000047d0: 0003 0000 8581 7201 0300 007d 7202 0300  ......r....}r...
+000047e0: 0028 681e 5500 681f 6afc 0200 0075 6261  .(h.U.h.j....uba
+000047f0: 6825 6856 7562 6852 5814 0000 0020 7265  h%hVubhRX.... re
+00004800: 6c61 7469 7665 2063 6861 6e67 6520 696e  lative change in
+00004810: 2072 0303 0000 8581 7204 0300 007d 7205   r......r....}r.
+00004820: 0300 0028 681e 5814 0000 0020 7265 6c61  ...(h.X.... rela
+00004830: 7469 7665 2063 6861 6e67 6520 696e 2068  tive change in h
+00004840: 1f6a f802 0000 7562 684a 2981 7206 0300  .j....ubhJ).r...
+00004850: 007d 7207 0300 0028 681e 580a 0000 0060  .}r....(h.X....`
+00004860: 6063 6869 2a2a 3260 6068 277d 7208 0300  `chi**2``h'}r...
+00004870: 0028 6829 5d68 2a5d 682b 5d68 2c5d 682f  .(h)]h*]h+]h,]h/
+00004880: 5d75 681f 6af8 0200 0068 335d 7209 0300  ]uh.j....h3]r...
+00004890: 0068 5258 0600 0000 6368 692a 2a32 720a  .hRX....chi**2r.
+000048a0: 0300 0085 8172 0b03 0000 7d72 0c03 0000  .....r....}r....
+000048b0: 2868 1e55 0068 1f6a 0603 0000 7562 6168  (h.U.h.j....ubah
+000048c0: 2568 5675 6268 5258 1300 0000 2062 6574  %hVubhRX.... bet
+000048d0: 7765 656e 2069 7465 7261 7469 6f6e 7372  ween iterationsr
+000048e0: 0d03 0000 8581 720e 0300 007d 720f 0300  ......r....}r...
+000048f0: 0028 681e 5813 0000 0020 6265 7477 6565  .(h.X.... betwee
+00004900: 6e20 6974 6572 6174 696f 6e73 681f 6af8  n iterationsh.j.
+00004910: 0200 0075 6265 7562 6575 6268 9729 8172  ...ubeubeubh.).r
+00004920: 1003 0000 7d72 1103 0000 2868 1e58 cf01  ....}r....(h.X..
+00004930: 0000 6973 2073 7461 7469 7366 6965 642e  ..is statisfied.
+00004940: 2053 6565 2074 6865 2060 6073 6369 7079   See the ``scipy
+00004950: 2e6f 7074 696d 697a 652e 6c65 6173 745f  .optimize.least_
+00004960: 7371 7561 7265 7360 600a 646f 6375 6d65  squares``.docume
+00004970: 6e74 6174 696f 6e20 6465 7461 696c 6564  ntation detailed
+00004980: 2064 6566 696e 6974 696f 6e73 206f 6620   definitions of 
+00004990: 7468 6520 7374 6f70 7069 6e67 2063 6f6e  the stopping con
+000049a0: 6469 7469 6f6e 732e 0a54 7970 6963 616c  ditions..Typical
+000049b0: 6c79 206f 6e65 2073 6574 7320 6060 7874  ly one sets ``xt
+000049c0: 6f6c 3d31 2f31 302a 2a64 6060 2077 6865  ol=1/10**d`` whe
+000049d0: 7265 2060 6064 6060 2069 7320 7468 6520  re ``d`` is the 
+000049e0: 6e75 6d62 6572 206f 660a 6469 6769 7473  number of.digits
+000049f0: 206f 6620 7072 6563 6973 696f 6e20 6465   of precision de
+00004a00: 7369 7265 6420 696e 2074 6865 2072 6573  sired in the res
+00004a10: 756c 742c 2077 6869 6c65 2060 6067 746f  ult, while ``gto
+00004a20: 6c3c 3c31 6060 2061 6e64 0a60 6066 746f  l<<1`` and.``fto
+00004a30: 6c3c 3c31 6060 2e20 5365 7474 696e 6720  l<<1``. Setting 
+00004a40: 6060 746f 6c3d 6570 7360 6020 7768 6572  ``tol=eps`` wher
+00004a50: 6520 6060 6570 7360 6020 6973 2061 206e  e ``eps`` is a n
+00004a60: 756d 6265 7220 6973 0a65 7175 6976 616c  umber is.equival
+00004a70: 656e 7420 746f 2073 6574 7469 6e67 2060  ent to setting `
+00004a80: 6074 6f6c 3d28 6570 732c 3165 2d31 302c  `tol=(eps,1e-10,
+00004a90: 3165 2d31 3029 6060 2e20 5365 7474 696e  1e-10)``. Settin
+00004aa0: 670a 6060 746f 6c3d 2865 7073 312c 6570  g.``tol=(eps1,ep
+00004ab0: 7332 2960 6020 6973 2065 7175 6976 6c65  s2)`` is equivle
+00004ac0: 6e74 2074 6f20 7365 7474 696e 670a 6060  nt to setting.``
+00004ad0: 746f 6c3d 2865 7073 312c 6570 7332 2c31  tol=(eps1,eps2,1
+00004ae0: 652d 3130 2960 602e 2044 6566 6175 6c74  e-10)``. Default
+00004af0: 2069 7320 6060 746f 6c3d 3165 2d35 6060   is ``tol=1e-5``
+00004b00: 2e68 1f6a 8c02 0000 6823 6a59 0100 0068  .h.j....h#jY...h
+00004b10: 2568 9a68 277d 7212 0300 0028 6829 5d68  %h.h'}r....(h)]h
+00004b20: 2a5d 682b 5d68 2c5d 682f 5d75 6831 4b1a  *]h+]h,]h/]uh1K.
+00004b30: 6832 6802 6833 5d72 1303 0000 2868 5258  h2h.h3]r....(hRX
+00004b40: 1700 0000 6973 2073 7461 7469 7366 6965  ....is statisfie
+00004b50: 642e 2053 6565 2074 6865 2072 1403 0000  d. See the r....
+00004b60: 8581 7215 0300 007d 7216 0300 0028 681e  ..r....}r....(h.
+00004b70: 5817 0000 0069 7320 7374 6174 6973 6669  X....is statisfi
+00004b80: 6564 2e20 5365 6520 7468 6520 6823 4e68  ed. See the h#Nh
+00004b90: 314e 6832 6802 681f 6a10 0300 0075 6268  1Nh2h.h.j....ubh
+00004ba0: 4a29 8172 1703 0000 7d72 1803 0000 2868  J).r....}r....(h
+00004bb0: 1e58 2000 0000 6060 7363 6970 792e 6f70  .X ...``scipy.op
+00004bc0: 7469 6d69 7a65 2e6c 6561 7374 5f73 7175  timize.least_squ
+00004bd0: 6172 6573 6060 6827 7d72 1903 0000 2868  ares``h'}r....(h
+00004be0: 295d 682a 5d68 2b5d 682c 5d68 2f5d 7568  )]h*]h+]h,]h/]uh
+00004bf0: 1f6a 1003 0000 6833 5d72 1a03 0000 6852  .j....h3]r....hR
+00004c00: 581c 0000 0073 6369 7079 2e6f 7074 696d  X....scipy.optim
+00004c10: 697a 652e 6c65 6173 745f 7371 7561 7265  ize.least_square
+00004c20: 7372 1b03 0000 8581 721c 0300 007d 721d  sr......r....}r.
+00004c30: 0300 0028 681e 5500 681f 6a17 0300 0075  ...(h.U.h.j....u
+00004c40: 6261 6825 6856 7562 6852 5853 0000 000a  bah%hVubhRXS....
+00004c50: 646f 6375 6d65 6e74 6174 696f 6e20 6465  documentation de
+00004c60: 7461 696c 6564 2064 6566 696e 6974 696f  tailed definitio
+00004c70: 6e73 206f 6620 7468 6520 7374 6f70 7069  ns of the stoppi
+00004c80: 6e67 2063 6f6e 6469 7469 6f6e 732e 0a54  ng conditions..T
+00004c90: 7970 6963 616c 6c79 206f 6e65 2073 6574  ypically one set
+00004ca0: 7320 721e 0300 0085 8172 1f03 0000 7d72  s r......r....}r
+00004cb0: 2003 0000 2868 1e58 5300 0000 0a64 6f63   ...(h.XS....doc
+00004cc0: 756d 656e 7461 7469 6f6e 2064 6574 6169  umentation detai
+00004cd0: 6c65 6420 6465 6669 6e69 7469 6f6e 7320  led definitions 
+00004ce0: 6f66 2074 6865 2073 746f 7070 696e 6720  of the stopping 
+00004cf0: 636f 6e64 6974 696f 6e73 2e0a 5479 7069  conditions..Typi
+00004d00: 6361 6c6c 7920 6f6e 6520 7365 7473 2068  cally one sets h
+00004d10: 234e 6831 4e68 3268 0268 1f6a 1003 0000  #Nh1Nh2h.h.j....
+00004d20: 7562 684a 2981 7221 0300 007d 7222 0300  ubhJ).r!...}r"..
+00004d30: 0028 681e 5810 0000 0060 6078 746f 6c3d  .(h.X....``xtol=
+00004d40: 312f 3130 2a2a 6460 6068 277d 7223 0300  1/10**d``h'}r#..
+00004d50: 0028 6829 5d68 2a5d 682b 5d68 2c5d 682f  .(h)]h*]h+]h,]h/
+00004d60: 5d75 681f 6a10 0300 0068 335d 7224 0300  ]uh.j....h3]r$..
+00004d70: 0068 5258 0c00 0000 7874 6f6c 3d31 2f31  .hRX....xtol=1/1
+00004d80: 302a 2a64 7225 0300 0085 8172 2603 0000  0**dr%.....r&...
+00004d90: 7d72 2703 0000 2868 1e55 0068 1f6a 2103  }r'...(h.U.h.j!.
+00004da0: 0000 7562 6168 2568 5675 6268 5258 0700  ..ubah%hVubhRX..
+00004db0: 0000 2077 6865 7265 2072 2803 0000 8581  .. where r(.....
+00004dc0: 7229 0300 007d 722a 0300 0028 681e 5807  r)...}r*...(h.X.
+00004dd0: 0000 0020 7768 6572 6520 722b 0300 0068  ... where r+...h
+00004de0: 234e 6831 4e68 3268 0268 1f6a 1003 0000  #Nh1Nh2h.h.j....
+00004df0: 7562 684a 2981 722c 0300 007d 722d 0300  ubhJ).r,...}r-..
+00004e00: 0028 681e 5805 0000 0060 6064 6060 6827  .(h.X....``d``h'
+00004e10: 7d72 2e03 0000 2868 295d 682a 5d68 2b5d  }r....(h)]h*]h+]
+00004e20: 682c 5d68 2f5d 7568 1f6a 1003 0000 6833  h,]h/]uh.j....h3
+00004e30: 5d72 2f03 0000 6852 5801 0000 0064 8581  ]r/...hRX....d..
+00004e40: 7230 0300 007d 7231 0300 0028 681e 5500  r0...}r1...(h.U.
+00004e50: 681f 6a2c 0300 0075 6261 6825 6856 7562  h.j,...ubah%hVub
+00004e60: 6852 5843 0000 0020 6973 2074 6865 206e  hRXC... is the n
+00004e70: 756d 6265 7220 6f66 0a64 6967 6974 7320  umber of.digits 
+00004e80: 6f66 2070 7265 6369 7369 6f6e 2064 6573  of precision des
+00004e90: 6972 6564 2069 6e20 7468 6520 7265 7375  ired in the resu
+00004ea0: 6c74 2c20 7768 696c 6520 7232 0300 0085  lt, while r2....
+00004eb0: 8172 3303 0000 7d72 3403 0000 2868 1e58  .r3...}r4...(h.X
+00004ec0: 4300 0000 2069 7320 7468 6520 6e75 6d62  C... is the numb
+00004ed0: 6572 206f 660a 6469 6769 7473 206f 6620  er of.digits of 
+00004ee0: 7072 6563 6973 696f 6e20 6465 7369 7265  precision desire
+00004ef0: 6420 696e 2074 6865 2072 6573 756c 742c  d in the result,
+00004f00: 2077 6869 6c65 2068 234e 6831 4e68 3268   while h#Nh1Nh2h
+00004f10: 0268 1f6a 1003 0000 7562 684a 2981 7235  .h.j....ubhJ).r5
+00004f20: 0300 007d 7236 0300 0028 681e 580b 0000  ...}r6...(h.X...
+00004f30: 0060 6067 746f 6c3c 3c31 6060 6827 7d72  .``gtol<<1``h'}r
+00004f40: 3703 0000 2868 295d 682a 5d68 2b5d 682c  7...(h)]h*]h+]h,
+00004f50: 5d68 2f5d 7568 1f6a 1003 0000 6833 5d72  ]h/]uh.j....h3]r
+00004f60: 3803 0000 6852 5807 0000 0067 746f 6c3c  8...hRX....gtol<
+00004f70: 3c31 7239 0300 0085 8172 3a03 0000 7d72  <1r9.....r:...}r
+00004f80: 3b03 0000 2868 1e55 0068 1f6a 3503 0000  ;...(h.U.h.j5...
+00004f90: 7562 6168 2568 5675 6268 5258 0500 0000  ubah%hVubhRX....
+00004fa0: 2061 6e64 0a72 3c03 0000 8581 723d 0300   and.r<.....r=..
+00004fb0: 007d 723e 0300 0028 681e 5805 0000 0020  .}r>...(h.X.... 
+00004fc0: 616e 640a 6823 4e68 314e 6832 6802 681f  and.h#Nh1Nh2h.h.
+00004fd0: 6a10 0300 0075 6268 4a29 8172 3f03 0000  j....ubhJ).r?...
+00004fe0: 7d72 4003 0000 2868 1e58 0b00 0000 6060  }r@...(h.X....``
+00004ff0: 6674 6f6c 3c3c 3160 6068 277d 7241 0300  ftol<<1``h'}rA..
+00005000: 0028 6829 5d68 2a5d 682b 5d68 2c5d 682f  .(h)]h*]h+]h,]h/
+00005010: 5d75 681f 6a10 0300 0068 335d 7242 0300  ]uh.j....h3]rB..
+00005020: 0068 5258 0700 0000 6674 6f6c 3c3c 3172  .hRX....ftol<<1r
+00005030: 4303 0000 8581 7244 0300 007d 7245 0300  C.....rD...}rE..
+00005040: 0028 681e 5500 681f 6a3f 0300 0075 6261  .(h.U.h.j?...uba
+00005050: 6825 6856 7562 6852 580a 0000 002e 2053  h%hVubhRX..... S
+00005060: 6574 7469 6e67 2072 4603 0000 8581 7247  etting rF.....rG
+00005070: 0300 007d 7248 0300 0028 681e 580a 0000  ...}rH...(h.X...
+00005080: 002e 2053 6574 7469 6e67 2068 234e 6831  .. Setting h#Nh1
+00005090: 4e68 3268 0268 1f6a 1003 0000 7562 684a  Nh2h.h.j....ubhJ
+000050a0: 2981 7249 0300 007d 724a 0300 0028 681e  ).rI...}rJ...(h.
+000050b0: 580b 0000 0060 6074 6f6c 3d65 7073 6060  X....``tol=eps``
+000050c0: 6827 7d72 4b03 0000 2868 295d 682a 5d68  h'}rK...(h)]h*]h
+000050d0: 2b5d 682c 5d68 2f5d 7568 1f6a 1003 0000  +]h,]h/]uh.j....
+000050e0: 6833 5d72 4c03 0000 6852 5807 0000 0074  h3]rL...hRX....t
+000050f0: 6f6c 3d65 7073 724d 0300 0085 8172 4e03  ol=epsrM.....rN.
+00005100: 0000 7d72 4f03 0000 2868 1e55 0068 1f6a  ..}rO...(h.U.h.j
+00005110: 4903 0000 7562 6168 2568 5675 6268 5258  I...ubah%hVubhRX
+00005120: 0700 0000 2077 6865 7265 2072 5003 0000  .... where rP...
+00005130: 8581 7251 0300 007d 7252 0300 0028 681e  ..rQ...}rR...(h.
+00005140: 6a2b 0300 0068 1f6a 1003 0000 7562 684a  j+...h.j....ubhJ
+00005150: 2981 7253 0300 007d 7254 0300 0028 681e  ).rS...}rT...(h.
+00005160: 5807 0000 0060 6065 7073 6060 6827 7d72  X....``eps``h'}r
+00005170: 5503 0000 2868 295d 682a 5d68 2b5d 682c  U...(h)]h*]h+]h,
+00005180: 5d68 2f5d 7568 1f6a 1003 0000 6833 5d72  ]h/]uh.j....h3]r
+00005190: 5603 0000 6852 5803 0000 0065 7073 7257  V...hRX....epsrW
+000051a0: 0300 0085 8172 5803 0000 7d72 5903 0000  .....rX...}rY...
+000051b0: 2868 1e55 0068 1f6a 5303 0000 7562 6168  (h.U.h.jS...ubah
+000051c0: 2568 5675 6268 5258 2600 0000 2069 7320  %hVubhRX&... is 
+000051d0: 6120 6e75 6d62 6572 2069 730a 6571 7569  a number is.equi
+000051e0: 7661 6c65 6e74 2074 6f20 7365 7474 696e  valent to settin
+000051f0: 6720 725a 0300 0085 8172 5b03 0000 7d72  g rZ.....r[...}r
+00005200: 5c03 0000 2868 1e58 2600 0000 2069 7320  \...(h.X&... is 
+00005210: 6120 6e75 6d62 6572 2069 730a 6571 7569  a number is.equi
+00005220: 7661 6c65 6e74 2074 6f20 7365 7474 696e  valent to settin
+00005230: 6720 6823 4e68 314e 6832 6802 681f 6a10  g h#Nh1Nh2h.h.j.
+00005240: 0300 0075 6268 4a29 8172 5d03 0000 7d72  ...ubhJ).r]...}r
+00005250: 5e03 0000 2868 1e58 1900 0000 6060 746f  ^...(h.X....``to
+00005260: 6c3d 2865 7073 2c31 652d 3130 2c31 652d  l=(eps,1e-10,1e-
+00005270: 3130 2960 6068 277d 725f 0300 0028 6829  10)``h'}r_...(h)
+00005280: 5d68 2a5d 682b 5d68 2c5d 682f 5d75 681f  ]h*]h+]h,]h/]uh.
+00005290: 6a10 0300 0068 335d 7260 0300 0068 5258  j....h3]r`...hRX
+000052a0: 1500 0000 746f 6c3d 2865 7073 2c31 652d  ....tol=(eps,1e-
+000052b0: 3130 2c31 652d 3130 2972 6103 0000 8581  10,1e-10)ra.....
+000052c0: 7262 0300 007d 7263 0300 0028 681e 5500  rb...}rc...(h.U.
+000052d0: 681f 6a5d 0300 0075 6261 6825 6856 7562  h.j]...ubah%hVub
+000052e0: 6852 580a 0000 002e 2053 6574 7469 6e67  hRX..... Setting
+000052f0: 0a72 6403 0000 8581 7265 0300 007d 7266  .rd.....re...}rf
+00005300: 0300 0028 681e 580a 0000 002e 2053 6574  ...(h.X..... Set
+00005310: 7469 6e67 0a68 234e 6831 4e68 3268 0268  ting.h#Nh1Nh2h.h
+00005320: 1f6a 1003 0000 7562 684a 2981 7267 0300  .j....ubhJ).rg..
+00005330: 007d 7268 0300 0028 681e 5813 0000 0060  .}rh...(h.X....`
+00005340: 6074 6f6c 3d28 6570 7331 2c65 7073 3229  `tol=(eps1,eps2)
+00005350: 6060 6827 7d72 6903 0000 2868 295d 682a  ``h'}ri...(h)]h*
+00005360: 5d68 2b5d 682c 5d68 2f5d 7568 1f6a 1003  ]h+]h,]h/]uh.j..
+00005370: 0000 6833 5d72 6a03 0000 6852 580f 0000  ..h3]rj...hRX...
+00005380: 0074 6f6c 3d28 6570 7331 2c65 7073 3229  .tol=(eps1,eps2)
+00005390: 726b 0300 0085 8172 6c03 0000 7d72 6d03  rk.....rl...}rm.
+000053a0: 0000 2868 1e55 0068 1f6a 6703 0000 7562  ..(h.U.h.jg...ub
+000053b0: 6168 2568 5675 6268 5258 1900 0000 2069  ah%hVubhRX.... i
+000053c0: 7320 6571 7569 766c 656e 7420 746f 2073  s equivlent to s
+000053d0: 6574 7469 6e67 0a72 6e03 0000 8581 726f  etting.rn.....ro
+000053e0: 0300 007d 7270 0300 0028 681e 5819 0000  ...}rp...(h.X...
+000053f0: 0020 6973 2065 7175 6976 6c65 6e74 2074  . is equivlent t
+00005400: 6f20 7365 7474 696e 670a 6823 4e68 314e  o setting.h#Nh1N
+00005410: 6832 6802 681f 6a10 0300 0075 6268 4a29  h2h.h.j....ubhJ)
+00005420: 8172 7103 0000 7d72 7203 0000 2868 1e58  .rq...}rr...(h.X
+00005430: 1900 0000 6060 746f 6c3d 2865 7073 312c  ....``tol=(eps1,
+00005440: 6570 7332 2c31 652d 3130 2960 6068 277d  eps2,1e-10)``h'}
+00005450: 7273 0300 0028 6829 5d68 2a5d 682b 5d68  rs...(h)]h*]h+]h
+00005460: 2c5d 682f 5d75 681f 6a10 0300 0068 335d  ,]h/]uh.j....h3]
+00005470: 7274 0300 0068 5258 1500 0000 746f 6c3d  rt...hRX....tol=
+00005480: 2865 7073 312c 6570 7332 2c31 652d 3130  (eps1,eps2,1e-10
+00005490: 2972 7503 0000 8581 7276 0300 007d 7277  )ru.....rv...}rw
+000054a0: 0300 0028 681e 5500 681f 6a71 0300 0075  ...(h.U.h.jq...u
+000054b0: 6261 6825 6856 7562 6852 580d 0000 002e  bah%hVubhRX.....
+000054c0: 2044 6566 6175 6c74 2069 7320 7278 0300   Default is rx..
+000054d0: 0085 8172 7903 0000 7d72 7a03 0000 2868  ...ry...}rz...(h
+000054e0: 1e58 0d00 0000 2e20 4465 6661 756c 7420  .X..... Default 
+000054f0: 6973 2068 234e 6831 4e68 3268 0268 1f6a  is h#Nh1Nh2h.h.j
+00005500: 1003 0000 7562 684a 2981 727b 0300 007d  ....ubhJ).r{...}
+00005510: 727c 0300 0028 681e 580c 0000 0060 6074  r|...(h.X....``t
+00005520: 6f6c 3d31 652d 3560 6068 277d 727d 0300  ol=1e-5``h'}r}..
+00005530: 0028 6829 5d68 2a5d 682b 5d68 2c5d 682f  .(h)]h*]h+]h,]h/
+00005540: 5d75 681f 6a10 0300 0068 335d 727e 0300  ]uh.j....h3]r~..
+00005550: 0068 5258 0800 0000 746f 6c3d 3165 2d35  .hRX....tol=1e-5
+00005560: 727f 0300 0085 8172 8003 0000 7d72 8103  r......r....}r..
+00005570: 0000 2868 1e55 0068 1f6a 7b03 0000 7562  ..(h.U.h.j{...ub
+00005580: 6168 2568 5675 6268 5258 0100 0000 2e85  ah%hVubhRX......
+00005590: 8172 8203 0000 7d72 8303 0000 2868 1e58  .r....}r....(h.X
+000055a0: 0100 0000 2e68 234e 6831 4e68 3268 0268  .....h#Nh1Nh2h.h
+000055b0: 1f6a 1003 0000 7562 6575 6265 6825 689a  .j....ubeubeh%h.
+000055c0: 7562 6168 256a 0002 0000 7562 6ad4 0100  ubah%j....ubj...
+000055d0: 0029 8172 8403 0000 7d72 8503 0000 2868  .).r....}r....(h
+000055e0: 1e55 0068 277d 7286 0300 0028 6829 5d68  .U.h'}r....(h)]h
+000055f0: 2a5d 682b 5d68 2c5d 682f 5d75 681f 6ad0  *]h+]h,]h/]uh.j.
+00005600: 0100 0068 335d 7287 0300 0068 9729 8172  ...h3]r....h.).r
+00005610: 8803 0000 7d72 8903 0000 2868 1e58 9b01  ....}r....(h.X..
+00005620: 0000 6d65 7468 6f64 2028 7374 7220 6f72  ..method (str or
+00005630: 204e 6f6e 6529 202d 2d20 4d69 6e69 6d69   None) -- Minimi
+00005640: 7a61 7469 6f6e 2061 6c67 6f72 6974 686d  zation algorithm
+00005650: 2e20 4f70 7469 6f6e 730a 696e 636c 7564  . Options.includ
+00005660: 653a 2774 7266 270a 0a54 7275 7374 6564  e:'trf'..Trusted
+00005670: 2052 6567 696f 6e20 5265 666c 6563 7469   Region Reflecti
+00005680: 7665 2061 6c67 6f72 6974 686d 2028 6465  ve algorithm (de
+00005690: 6661 756c 7429 2e20 4265 7374 0a63 686f  fault). Best.cho
+000056a0: 6963 6520 7769 7468 2062 6f75 6e64 6564  ice with bounded
+000056b0: 2070 6172 616d 6574 6572 732e 0a0a 2764   parameters...'d
+000056c0: 6f67 626f 7827 0a0a 646f 676c 6567 2061  ogbox'..dogleg a
+000056d0: 6c67 6f72 6974 686d 2061 6461 7074 6564  lgorithm adapted
+000056e0: 2066 6f72 2062 6f75 6e64 6564 2070 6172   for bounded par
+000056f0: 616d 6574 6572 732e 0a0a 276c 6d27 0a0a  ameters...'lm'..
+00005700: 4c65 7665 6e62 6572 672d 4d61 7271 7561  Levenberg-Marqua
+00005710: 7264 7420 616c 676f 7269 7468 6d20 6173  rdt algorithm as
+00005720: 2069 6d70 6c65 6d65 6e74 6564 2069 6e20   implemented in 
+00005730: 4d49 4e50 4143 4b2e 0a42 6573 7420 666f  MINPACK..Best fo
+00005740: 7220 736d 616c 6c65 7220 7072 6f62 6c65  r smaller proble
+00005750: 6d73 2e20 446f 6573 206e 6f74 2077 6f72  ms. Does not wor
+00005760: 6b20 7769 7468 2062 6f75 6e64 6564 0a70  k with bounded.p
+00005770: 6172 616d 6574 6572 7320 2862 6f75 6e64  arameters (bound
+00005780: 7320 6172 6520 6967 6e6f 7265 6429 2e53  s are ignored).S
+00005790: 6574 7469 6e67 206d 6574 686f 643d 4e6f  etting method=No
+000057a0: 6e65 2069 6d70 6c69 6573 2074 6865 2064  ne implies the d
+000057b0: 6566 6175 6c74 2027 7472 6627 2e68 277d  efault 'trf'.h'}
+000057c0: 728a 0300 0028 6829 5d68 2a5d 682b 5d68  r....(h)]h*]h+]h
+000057d0: 2c5d 682f 5d75 681f 6a84 0300 0068 335d  ,]h/]uh.j....h3]
+000057e0: 728b 0300 0028 6add 0100 0029 8172 8c03  r....(j....).r..
+000057f0: 0000 7d72 8d03 0000 2868 1e58 0600 0000  ..}r....(h.X....
+00005800: 6d65 7468 6f64 6827 7d72 8e03 0000 2868  methodh'}r....(h
+00005810: 2c5d 682b 5d6a e101 0000 8868 295d 682a  ,]h+]j.....h)]h*
+00005820: 5d68 2f5d 7568 1f6a 8803 0000 6833 5d72  ]h/]uh.j....h3]r
+00005830: 8f03 0000 6852 5806 0000 006d 6574 686f  ....hRX....metho
+00005840: 6472 9003 0000 8581 7291 0300 007d 7292  dr......r....}r.
+00005850: 0300 0028 681e 5500 681f 6a8c 0300 0075  ...(h.U.h.j....u
+00005860: 6261 6825 6ae6 0100 0075 6268 5258 0200  bah%j....ubhRX..
+00005870: 0000 2028 7293 0300 0085 8172 9403 0000  .. (r......r....
+00005880: 7d72 9503 0000 2868 1e55 0068 1f6a 8803  }r....(h.U.h.j..
+00005890: 0000 7562 683c 2981 7296 0300 007d 7297  ..ubh<).r....}r.
+000058a0: 0300 0028 681e 5500 6827 7d72 9803 0000  ...(h.U.h'}r....
+000058b0: 2855 0772 6566 7479 7065 68f2 6ae1 0100  (U.reftypeh.j...
+000058c0: 0088 5509 7265 6674 6172 6765 7458 0300  ..U.reftargetX..
+000058d0: 0000 7374 7272 9903 0000 5509 7265 6664  ..strr....U.refd
+000058e0: 6f6d 6169 6e68 de68 2c5d 682b 5d55 0b72  omainh.h,]h+]U.r
+000058f0: 6566 6578 706c 6963 6974 8968 295d 682a  efexplicit.h)]h*
+00005900: 5d68 2f5d 7568 1f6a 8803 0000 6833 5d72  ]h/]uh.j....h3]r
+00005910: 9a03 0000 6aef 0100 0029 8172 9b03 0000  ....j....).r....
+00005920: 7d72 9c03 0000 2868 1e6a 9903 0000 6827  }r....(h.j....h'
+00005930: 7d72 9d03 0000 2868 295d 682a 5d68 2b5d  }r....(h)]h*]h+]
+00005940: 682c 5d68 2f5d 7568 1f6a 9603 0000 6833  h,]h/]uh.j....h3
+00005950: 5d72 9e03 0000 6852 5803 0000 0073 7472  ]r....hRX....str
+00005960: 729f 0300 0085 8172 a003 0000 7d72 a103  r......r....}r..
+00005970: 0000 2868 1e55 0068 1f6a 9b03 0000 7562  ..(h.U.h.j....ub
+00005980: 6168 256a f701 0000 7562 6168 2568 4075  ah%j....ubah%h@u
+00005990: 626a ef01 0000 2981 72a2 0300 007d 72a3  bj....).r....}r.
+000059a0: 0300 0028 681e 5804 0000 0020 6f72 2068  ...(h.X.... or h
+000059b0: 277d 72a4 0300 0028 6829 5d68 2a5d 682b  '}r....(h)]h*]h+
+000059c0: 5d68 2c5d 682f 5d75 681f 6a88 0300 0068  ]h,]h/]uh.j....h
+000059d0: 335d 72a5 0300 0068 5258 0400 0000 206f  3]r....hRX.... o
+000059e0: 7220 72a6 0300 0085 8172 a703 0000 7d72  r r......r....}r
+000059f0: a803 0000 2868 1e55 0068 1f6a a203 0000  ....(h.U.h.j....
+00005a00: 7562 6168 256a f701 0000 7562 683c 2981  ubah%j....ubh<).
+00005a10: 72a9 0300 007d 72aa 0300 0028 681e 5500  r....}r....(h.U.
+00005a20: 6827 7d72 ab03 0000 2855 0772 6566 7479  h'}r....(U.refty
+00005a30: 7065 68f2 6ae1 0100 0088 5509 7265 6674  peh.j.....U.reft
+00005a40: 6172 6765 7458 0400 0000 4e6f 6e65 72ac  argetX....Noner.
+00005a50: 0300 0055 0972 6566 646f 6d61 696e 68de  ...U.refdomainh.
+00005a60: 682c 5d68 2b5d 550b 7265 6665 7870 6c69  h,]h+]U.refexpli
+00005a70: 6369 7489 6829 5d68 2a5d 682f 5d75 681f  cit.h)]h*]h/]uh.
+00005a80: 6a88 0300 0068 335d 72ad 0300 006a ef01  j....h3]r....j..
+00005a90: 0000 2981 72ae 0300 007d 72af 0300 0028  ..).r....}r....(
+00005aa0: 681e 6aac 0300 0068 277d 72b0 0300 0028  h.j....h'}r....(
+00005ab0: 6829 5d68 2a5d 682b 5d68 2c5d 682f 5d75  h)]h*]h+]h,]h/]u
+00005ac0: 681f 6aa9 0300 0068 335d 72b1 0300 0068  h.j....h3]r....h
+00005ad0: 5258 0400 0000 4e6f 6e65 72b2 0300 0085  RX....Noner.....
+00005ae0: 8172 b303 0000 7d72 b403 0000 2868 1e55  .r....}r....(h.U
+00005af0: 0068 1f6a ae03 0000 7562 6168 256a f701  .h.j....ubah%j..
+00005b00: 0000 7562 6168 2568 4075 6268 5258 0100  ..ubah%h@ubhRX..
+00005b10: 0000 2985 8172 b503 0000 7d72 b603 0000  ..)..r....}r....
+00005b20: 2868 1e55 0068 1f6a 8803 0000 7562 6852  (h.U.h.j....ubhR
+00005b30: 5805 0000 0020 e280 9320 72b7 0300 0085  X.... ... r.....
+00005b40: 8172 b803 0000 7d72 b903 0000 2868 1e55  .r....}r....(h.U
+00005b50: 0068 1f6a 8803 0000 7562 6897 2981 72ba  .h.j....ubh.).r.
+00005b60: 0300 007d 72bb 0300 0028 681e 5828 0000  ...}r....(h.X(..
+00005b70: 004d 696e 696d 697a 6174 696f 6e20 616c  .Minimization al
+00005b80: 676f 7269 7468 6d2e 204f 7074 696f 6e73  gorithm. Options
+00005b90: 0a69 6e63 6c75 6465 3a72 bc03 0000 681f  .include:r....h.
+00005ba0: 6a88 0300 0068 236a 5901 0000 6825 689a  j....h#jY...h%h.
+00005bb0: 6827 7d72 bd03 0000 2868 295d 682a 5d68  h'}r....(h)]h*]h
+00005bc0: 2b5d 682c 5d68 2f5d 7568 314b 2368 3268  +]h,]h/]uh1K#h2h
+00005bd0: 0268 335d 72be 0300 0068 5258 2800 0000  .h3]r....hRX(...
+00005be0: 4d69 6e69 6d69 7a61 7469 6f6e 2061 6c67  Minimization alg
+00005bf0: 6f72 6974 686d 2e20 4f70 7469 6f6e 730a  orithm. Options.
+00005c00: 696e 636c 7564 653a 72bf 0300 0085 8172  include:r......r
+00005c10: c003 0000 7d72 c103 0000 2868 1e6a bc03  ....}r....(h.j..
+00005c20: 0000 6823 4e68 314e 6832 6802 681f 6aba  ..h#Nh1Nh2h.h.j.
+00005c30: 0300 0075 6261 7562 6acf 0200 0029 8172  ...ubaubj....).r
+00005c40: c203 0000 7d72 c303 0000 2868 1e55 0068  ....}r....(h.U.h
+00005c50: 1f6a 8803 0000 6823 4e68 256a d202 0000  .j....h#Nh%j....
+00005c60: 6827 7d72 c403 0000 2868 295d 682a 5d68  h'}r....(h)]h*]h
+00005c70: 2b5d 682c 5d68 2f5d 7568 314e 6832 6802  +]h,]h/]uh1Nh2h.
+00005c80: 6833 5d72 c503 0000 6364 6f63 7574 696c  h3]r....cdocutil
+00005c90: 732e 6e6f 6465 730a 6465 6669 6e69 7469  s.nodes.definiti
+00005ca0: 6f6e 5f6c 6973 740a 72c6 0300 0029 8172  on_list.r....).r
+00005cb0: c703 0000 7d72 c803 0000 2868 1e55 0068  ....}r....(h.U.h
+00005cc0: 277d 72c9 0300 0028 6829 5d68 2a5d 682b  '}r....(h)]h*]h+
+00005cd0: 5d68 2c5d 682f 5d75 681f 6ac2 0300 0068  ]h,]h/]uh.j....h
+00005ce0: 335d 72ca 0300 0028 6364 6f63 7574 696c  3]r....(cdocutil
+00005cf0: 732e 6e6f 6465 730a 6465 6669 6e69 7469  s.nodes.definiti
+00005d00: 6f6e 5f6c 6973 745f 6974 656d 0a72 cb03  on_list_item.r..
+00005d10: 0000 2981 72cc 0300 007d 72cd 0300 0028  ..).r....}r....(
+00005d20: 681e 585e 0000 0060 6027 7472 6627 6060  h.X^...``'trf'``
+00005d30: 0a54 7275 7374 6564 2052 6567 696f 6e20  .Trusted Region 
+00005d40: 5265 666c 6563 7469 7665 2061 6c67 6f72  Reflective algor
+00005d50: 6974 686d 2028 6465 6661 756c 7429 2e20  ithm (default). 
+00005d60: 4265 7374 0a63 686f 6963 6520 7769 7468  Best.choice with
+00005d70: 2062 6f75 6e64 6564 2070 6172 616d 6574   bounded paramet
+00005d80: 6572 732e 0a68 1f6a c703 0000 6823 6a59  ers..h.j....h#jY
+00005d90: 0100 0068 2555 1464 6566 696e 6974 696f  ...h%U.definitio
+00005da0: 6e5f 6c69 7374 5f69 7465 6d72 ce03 0000  n_list_itemr....
+00005db0: 6827 7d72 cf03 0000 2868 295d 682a 5d68  h'}r....(h)]h*]h
+00005dc0: 2b5d 682c 5d68 2f5d 7568 314b 2868 335d  +]h,]h/]uh1K(h3]
+00005dd0: 72d0 0300 0028 6364 6f63 7574 696c 732e  r....(cdocutils.
+00005de0: 6e6f 6465 730a 7465 726d 0a72 d103 0000  nodes.term.r....
+00005df0: 2981 72d2 0300 007d 72d3 0300 0028 681e  ).r....}r....(h.
+00005e00: 5809 0000 0060 6027 7472 6627 6060 72d4  X....``'trf'``r.
+00005e10: 0300 0068 1f6a cc03 0000 6823 6a59 0100  ...h.j....h#jY..
+00005e20: 0068 2555 0474 6572 6d72 d503 0000 6827  .h%U.termr....h'
+00005e30: 7d72 d603 0000 2868 295d 682a 5d68 2b5d  }r....(h)]h*]h+]
+00005e40: 682c 5d68 2f5d 7568 314b 2868 335d 72d7  h,]h/]uh1K(h3]r.
+00005e50: 0300 0068 4a29 8172 d803 0000 7d72 d903  ...hJ).r....}r..
+00005e60: 0000 2868 1e6a d403 0000 6827 7d72 da03  ..(h.j....h'}r..
+00005e70: 0000 2868 295d 682a 5d68 2b5d 682c 5d68  ..(h)]h*]h+]h,]h
+00005e80: 2f5d 7568 1f6a d203 0000 6833 5d72 db03  /]uh.j....h3]r..
+00005e90: 0000 6852 5805 0000 0027 7472 6627 72dc  ..hRX....'trf'r.
+00005ea0: 0300 0085 8172 dd03 0000 7d72 de03 0000  .....r....}r....
+00005eb0: 2868 1e55 0068 1f6a d803 0000 7562 6168  (h.U.h.j....ubah
+00005ec0: 2568 5675 6261 7562 6364 6f63 7574 696c  %hVubaubcdocutil
+00005ed0: 732e 6e6f 6465 730a 6465 6669 6e69 7469  s.nodes.definiti
+00005ee0: 6f6e 0a72 df03 0000 2981 72e0 0300 007d  on.r....).r....}
+00005ef0: 72e1 0300 0028 681e 5500 6827 7d72 e203  r....(h.U.h'}r..
+00005f00: 0000 2868 295d 682a 5d68 2b5d 682c 5d68  ..(h)]h*]h+]h,]h
+00005f10: 2f5d 7568 1f6a cc03 0000 6833 5d72 e303  /]uh.j....h3]r..
+00005f20: 0000 6897 2981 72e4 0300 007d 72e5 0300  ..h.).r....}r...
+00005f30: 0028 681e 5853 0000 0054 7275 7374 6564  .(h.XS...Trusted
+00005f40: 2052 6567 696f 6e20 5265 666c 6563 7469   Region Reflecti
+00005f50: 7665 2061 6c67 6f72 6974 686d 2028 6465  ve algorithm (de
+00005f60: 6661 756c 7429 2e20 4265 7374 0a63 686f  fault). Best.cho
+00005f70: 6963 6520 7769 7468 2062 6f75 6e64 6564  ice with bounded
+00005f80: 2070 6172 616d 6574 6572 732e 72e6 0300   parameters.r...
+00005f90: 0068 1f6a e003 0000 6823 6a59 0100 0068  .h.j....h#jY...h
+00005fa0: 2568 9a68 277d 72e7 0300 0028 6829 5d68  %h.h'}r....(h)]h
+00005fb0: 2a5d 682b 5d68 2c5d 682f 5d75 6831 4b27  *]h+]h,]h/]uh1K'
+00005fc0: 6833 5d72 e803 0000 6852 5853 0000 0054  h3]r....hRXS...T
+00005fd0: 7275 7374 6564 2052 6567 696f 6e20 5265  rusted Region Re
+00005fe0: 666c 6563 7469 7665 2061 6c67 6f72 6974  flective algorit
+00005ff0: 686d 2028 6465 6661 756c 7429 2e20 4265  hm (default). Be
+00006000: 7374 0a63 686f 6963 6520 7769 7468 2062  st.choice with b
+00006010: 6f75 6e64 6564 2070 6172 616d 6574 6572  ounded parameter
+00006020: 732e 72e9 0300 0085 8172 ea03 0000 7d72  s.r......r....}r
+00006030: eb03 0000 2868 1e6a e603 0000 681f 6ae4  ....(h.j....h.j.
+00006040: 0300 0075 6261 7562 6168 2555 0a64 6566  ...ubaubah%U.def
+00006050: 696e 6974 696f 6e72 ec03 0000 7562 6575  initionr....ubeu
+00006060: 626a cb03 0000 2981 72ed 0300 007d 72ee  bj....).r....}r.
+00006070: 0300 0028 681e 583e 0000 0060 6027 646f  ...(h.X>...``'do
+00006080: 6762 6f78 2760 600a 646f 676c 6567 2061  gbox'``.dogleg a
+00006090: 6c67 6f72 6974 686d 2061 6461 7074 6564  lgorithm adapted
+000060a0: 2066 6f72 2062 6f75 6e64 6564 2070 6172   for bounded par
+000060b0: 616d 6574 6572 732e 0a68 1f6a c703 0000  ameters..h.j....
+000060c0: 6823 6a59 0100 0068 256a ce03 0000 6827  h#jY...h%j....h'
+000060d0: 7d72 ef03 0000 2868 295d 682a 5d68 2b5d  }r....(h)]h*]h+]
+000060e0: 682c 5d68 2f5d 7568 314b 2b68 335d 72f0  h,]h/]uh1K+h3]r.
+000060f0: 0300 0028 6ad1 0300 0029 8172 f103 0000  ...(j....).r....
+00006100: 7d72 f203 0000 2868 1e58 0c00 0000 6060  }r....(h.X....``
+00006110: 2764 6f67 626f 7827 6060 72f3 0300 0068  'dogbox'``r....h
+00006120: 1f6a ed03 0000 6823 6a59 0100 0068 256a  .j....h#jY...h%j
+00006130: d503 0000 6827 7d72 f403 0000 2868 295d  ....h'}r....(h)]
+00006140: 682a 5d68 2b5d 682c 5d68 2f5d 7568 314b  h*]h+]h,]h/]uh1K
+00006150: 2b68 335d 72f5 0300 0068 4a29 8172 f603  +h3]r....hJ).r..
+00006160: 0000 7d72 f703 0000 2868 1e6a f303 0000  ..}r....(h.j....
+00006170: 6827 7d72 f803 0000 2868 295d 682a 5d68  h'}r....(h)]h*]h
+00006180: 2b5d 682c 5d68 2f5d 7568 1f6a f103 0000  +]h,]h/]uh.j....
+00006190: 6833 5d72 f903 0000 6852 5808 0000 0027  h3]r....hRX....'
+000061a0: 646f 6762 6f78 2772 fa03 0000 8581 72fb  dogbox'r......r.
+000061b0: 0300 007d 72fc 0300 0028 681e 5500 681f  ...}r....(h.U.h.
+000061c0: 6af6 0300 0075 6261 6825 6856 7562 6175  j....ubah%hVubau
+000061d0: 626a df03 0000 2981 72fd 0300 007d 72fe  bj....).r....}r.
+000061e0: 0300 0028 681e 5500 6827 7d72 ff03 0000  ...(h.U.h'}r....
+000061f0: 2868 295d 682a 5d68 2b5d 682c 5d68 2f5d  (h)]h*]h+]h,]h/]
+00006200: 7568 1f6a ed03 0000 6833 5d72 0004 0000  uh.j....h3]r....
+00006210: 6897 2981 7201 0400 007d 7202 0400 0028  h.).r....}r....(
+00006220: 681e 5830 0000 0064 6f67 6c65 6720 616c  h.X0...dogleg al
+00006230: 676f 7269 7468 6d20 6164 6170 7465 6420  gorithm adapted 
+00006240: 666f 7220 626f 756e 6465 6420 7061 7261  for bounded para
+00006250: 6d65 7465 7273 2e72 0304 0000 681f 6afd  meters.r....h.j.
+00006260: 0300 0068 236a 5901 0000 6825 689a 6827  ...h#jY...h%h.h'
+00006270: 7d72 0404 0000 2868 295d 682a 5d68 2b5d  }r....(h)]h*]h+]
+00006280: 682c 5d68 2f5d 7568 314b 2b68 335d 7205  h,]h/]uh1K+h3]r.
+00006290: 0400 0068 5258 3000 0000 646f 676c 6567  ...hRX0...dogleg
+000062a0: 2061 6c67 6f72 6974 686d 2061 6461 7074   algorithm adapt
+000062b0: 6564 2066 6f72 2062 6f75 6e64 6564 2070  ed for bounded p
+000062c0: 6172 616d 6574 6572 732e 7206 0400 0085  arameters.r.....
+000062d0: 8172 0704 0000 7d72 0804 0000 2868 1e6a  .r....}r....(h.j
+000062e0: 0304 0000 681f 6a01 0400 0075 6261 7562  ....h.j....ubaub
+000062f0: 6168 256a ec03 0000 7562 6575 626a cb03  ah%j....ubeubj..
+00006300: 0000 2981 7209 0400 007d 720a 0400 0028  ..).r....}r....(
+00006310: 681e 5899 0000 0060 6027 6c6d 2760 600a  h.X....``'lm'``.
+00006320: 4c65 7665 6e62 6572 672d 4d61 7271 7561  Levenberg-Marqua
+00006330: 7264 7420 616c 676f 7269 7468 6d20 6173  rdt algorithm as
+00006340: 2069 6d70 6c65 6d65 6e74 6564 2069 6e20   implemented in 
+00006350: 4d49 4e50 4143 4b2e 0a42 6573 7420 666f  MINPACK..Best fo
+00006360: 7220 736d 616c 6c65 7220 7072 6f62 6c65  r smaller proble
+00006370: 6d73 2e20 446f 6573 206e 6f74 2077 6f72  ms. Does not wor
+00006380: 6b20 7769 7468 2062 6f75 6e64 6564 0a70  k with bounded.p
+00006390: 6172 616d 6574 6572 7320 2862 6f75 6e64  arameters (bound
+000063a0: 7320 6172 6520 6967 6e6f 7265 6429 2e0a  s are ignored)..
+000063b0: 681f 6ac7 0300 0068 236a 5901 0000 6825  h.j....h#jY...h%
+000063c0: 6ace 0300 0068 277d 720b 0400 0028 6829  j....h'}r....(h)
+000063d0: 5d68 2a5d 682b 5d68 2c5d 682f 5d75 6831  ]h*]h+]h,]h/]uh1
+000063e0: 4b30 6833 5d72 0c04 0000 286a d103 0000  K0h3]r....(j....
+000063f0: 2981 720d 0400 007d 720e 0400 0028 681e  ).r....}r....(h.
+00006400: 5808 0000 0060 6027 6c6d 2760 6072 0f04  X....``'lm'``r..
+00006410: 0000 681f 6a09 0400 0068 236a 5901 0000  ..h.j....h#jY...
+00006420: 6825 6ad5 0300 0068 277d 7210 0400 0028  h%j....h'}r....(
+00006430: 6829 5d68 2a5d 682b 5d68 2c5d 682f 5d75  h)]h*]h+]h,]h/]u
+00006440: 6831 4b30 6833 5d72 1104 0000 684a 2981  h1K0h3]r....hJ).
+00006450: 7212 0400 007d 7213 0400 0028 681e 6a0f  r....}r....(h.j.
+00006460: 0400 0068 277d 7214 0400 0028 6829 5d68  ...h'}r....(h)]h
+00006470: 2a5d 682b 5d68 2c5d 682f 5d75 681f 6a0d  *]h+]h,]h/]uh.j.
+00006480: 0400 0068 335d 7215 0400 0068 5258 0400  ...h3]r....hRX..
+00006490: 0000 276c 6d27 7216 0400 0085 8172 1704  ..'lm'r......r..
+000064a0: 0000 7d72 1804 0000 2868 1e55 0068 1f6a  ..}r....(h.U.h.j
+000064b0: 1204 0000 7562 6168 2568 5675 6261 7562  ....ubah%hVubaub
+000064c0: 6adf 0300 0029 8172 1904 0000 7d72 1a04  j....).r....}r..
+000064d0: 0000 2868 1e55 0068 277d 721b 0400 0028  ..(h.U.h'}r....(
+000064e0: 6829 5d68 2a5d 682b 5d68 2c5d 682f 5d75  h)]h*]h+]h,]h/]u
+000064f0: 681f 6a09 0400 0068 335d 721c 0400 0068  h.j....h3]r....h
+00006500: 9729 8172 1d04 0000 7d72 1e04 0000 2868  .).r....}r....(h
+00006510: 1e58 8f00 0000 4c65 7665 6e62 6572 672d  .X....Levenberg-
+00006520: 4d61 7271 7561 7264 7420 616c 676f 7269  Marquardt algori
+00006530: 7468 6d20 6173 2069 6d70 6c65 6d65 6e74  thm as implement
+00006540: 6564 2069 6e20 4d49 4e50 4143 4b2e 0a42  ed in MINPACK..B
+00006550: 6573 7420 666f 7220 736d 616c 6c65 7220  est for smaller 
+00006560: 7072 6f62 6c65 6d73 2e20 446f 6573 206e  problems. Does n
+00006570: 6f74 2077 6f72 6b20 7769 7468 2062 6f75  ot work with bou
+00006580: 6e64 6564 0a70 6172 616d 6574 6572 7320  nded.parameters 
+00006590: 2862 6f75 6e64 7320 6172 6520 6967 6e6f  (bounds are igno
+000065a0: 7265 6429 2e72 1f04 0000 681f 6a19 0400  red).r....h.j...
+000065b0: 0068 236a 5901 0000 6825 689a 6827 7d72  .h#jY...h%h.h'}r
+000065c0: 2004 0000 2868 295d 682a 5d68 2b5d 682c   ...(h)]h*]h+]h,
+000065d0: 5d68 2f5d 7568 314b 2e68 335d 7221 0400  ]h/]uh1K.h3]r!..
+000065e0: 0068 5258 8f00 0000 4c65 7665 6e62 6572  .hRX....Levenber
+000065f0: 672d 4d61 7271 7561 7264 7420 616c 676f  g-Marquardt algo
+00006600: 7269 7468 6d20 6173 2069 6d70 6c65 6d65  rithm as impleme
+00006610: 6e74 6564 2069 6e20 4d49 4e50 4143 4b2e  nted in MINPACK.
+00006620: 0a42 6573 7420 666f 7220 736d 616c 6c65  .Best for smalle
+00006630: 7220 7072 6f62 6c65 6d73 2e20 446f 6573  r problems. Does
+00006640: 206e 6f74 2077 6f72 6b20 7769 7468 2062   not work with b
+00006650: 6f75 6e64 6564 0a70 6172 616d 6574 6572  ounded.parameter
+00006660: 7320 2862 6f75 6e64 7320 6172 6520 6967  s (bounds are ig
+00006670: 6e6f 7265 6429 2e72 2204 0000 8581 7223  nored).r".....r#
+00006680: 0400 007d 7224 0400 0028 681e 6a1f 0400  ...}r$...(h.j...
+00006690: 0068 1f6a 1d04 0000 7562 6175 6261 6825  .h.j....ubaubah%
+000066a0: 6aec 0300 0075 6265 7562 6568 2555 0f64  j....ubeubeh%U.d
+000066b0: 6566 696e 6974 696f 6e5f 6c69 7374 7225  efinition_listr%
+000066c0: 0400 0075 6261 7562 6897 2981 7226 0400  ...ubaubh.).r&..
+000066d0: 007d 7227 0400 0028 681e 5836 0000 0053  .}r'...(h.X6...S
+000066e0: 6574 7469 6e67 2060 606d 6574 686f 643d  etting ``method=
+000066f0: 4e6f 6e65 6060 2069 6d70 6c69 6573 2074  None`` implies t
+00006700: 6865 2064 6566 6175 6c74 2060 6027 7472  he default ``'tr
+00006710: 6627 6060 2e68 1f6a 8803 0000 6823 6a59  f'``.h.j....h#jY
+00006720: 0100 0068 2568 9a68 277d 7228 0400 0028  ...h%h.h'}r(...(
+00006730: 6829 5d68 2a5d 682b 5d68 2c5d 682f 5d75  h)]h*]h+]h,]h/]u
+00006740: 6831 4b32 6832 6802 6833 5d72 2904 0000  h1K2h2h.h3]r)...
+00006750: 2868 5258 0800 0000 5365 7474 696e 6720  (hRX....Setting 
+00006760: 722a 0400 0085 8172 2b04 0000 7d72 2c04  r*.....r+...}r,.
+00006770: 0000 2868 1e58 0800 0000 5365 7474 696e  ..(h.X....Settin
+00006780: 6720 6823 4e68 314e 6832 6802 681f 6a26  g h#Nh1Nh2h.h.j&
+00006790: 0400 0075 6268 4a29 8172 2d04 0000 7d72  ...ubhJ).r-...}r
+000067a0: 2e04 0000 2868 1e58 0f00 0000 6060 6d65  ....(h.X....``me
+000067b0: 7468 6f64 3d4e 6f6e 6560 6068 277d 722f  thod=None``h'}r/
+000067c0: 0400 0028 6829 5d68 2a5d 682b 5d68 2c5d  ...(h)]h*]h+]h,]
+000067d0: 682f 5d75 681f 6a26 0400 0068 335d 7230  h/]uh.j&...h3]r0
+000067e0: 0400 0068 5258 0b00 0000 6d65 7468 6f64  ...hRX....method
+000067f0: 3d4e 6f6e 6572 3104 0000 8581 7232 0400  =Noner1.....r2..
+00006800: 007d 7233 0400 0028 681e 5500 681f 6a2d  .}r3...(h.U.h.j-
+00006810: 0400 0075 6261 6825 6856 7562 6852 5815  ...ubah%hVubhRX.
+00006820: 0000 0020 696d 706c 6965 7320 7468 6520  ... implies the 
+00006830: 6465 6661 756c 7420 7234 0400 0085 8172  default r4.....r
+00006840: 3504 0000 7d72 3604 0000 2868 1e58 1500  5...}r6...(h.X..
+00006850: 0000 2069 6d70 6c69 6573 2074 6865 2064  .. implies the d
+00006860: 6566 6175 6c74 2068 234e 6831 4e68 3268  efault h#Nh1Nh2h
+00006870: 0268 1f6a 2604 0000 7562 684a 2981 7237  .h.j&...ubhJ).r7
+00006880: 0400 007d 7238 0400 0028 681e 5809 0000  ...}r8...(h.X...
+00006890: 0060 6027 7472 6627 6060 6827 7d72 3904  .``'trf'``h'}r9.
+000068a0: 0000 2868 295d 682a 5d68 2b5d 682c 5d68  ..(h)]h*]h+]h,]h
+000068b0: 2f5d 7568 1f6a 2604 0000 6833 5d72 3a04  /]uh.j&...h3]r:.
+000068c0: 0000 6852 5805 0000 0027 7472 6627 723b  ..hRX....'trf'r;
+000068d0: 0400 0085 8172 3c04 0000 7d72 3d04 0000  .....r<...}r=...
+000068e0: 2868 1e55 0068 1f6a 3704 0000 7562 6168  (h.U.h.j7...ubah
+000068f0: 2568 5675 6268 5258 0100 0000 2e85 8172  %hVubhRX.......r
+00006900: 3e04 0000 7d72 3f04 0000 2868 1e58 0100  >...}r?...(h.X..
+00006910: 0000 2e68 234e 6831 4e68 3268 0268 1f6a  ...h#Nh1Nh2h.h.j
+00006920: 2604 0000 7562 6575 6265 6825 689a 7562  &...ubeubeh%h.ub
+00006930: 6168 256a 0002 0000 7562 6ad4 0100 0029  ah%j....ubj....)
+00006940: 8172 4004 0000 7d72 4104 0000 2868 1e55  .r@...}rA...(h.U
+00006950: 0068 277d 7242 0400 0028 6829 5d68 2a5d  .h'}rB...(h)]h*]
+00006960: 682b 5d68 2c5d 682f 5d75 681f 6ad0 0100  h+]h,]h/]uh.j...
+00006970: 0068 335d 7243 0400 0068 9729 8172 4404  .h3]rC...h.).rD.
+00006980: 0000 7d72 4504 0000 2868 1e58 5d00 0000  ..}rE...(h.X]...
+00006990: 6d61 7869 7420 2869 6e74 2920 2d2d 204d  maxit (int) -- M
+000069a0: 6178 696d 756d 206e 756d 6265 7220 6f66  aximum number of
+000069b0: 2066 756e 6374 696f 6e20 6576 616c 7561   function evalua
+000069c0: 7469 6f6e 7320 696e 2073 6561 7263 680a  tions in search.
+000069d0: 666f 7220 6d69 6e69 6d75 6d3b 2064 6566  for minimum; def
+000069e0: 6175 6c74 2069 7320 3130 3030 2e68 277d  ault is 1000.h'}
+000069f0: 7246 0400 0028 6829 5d68 2a5d 682b 5d68  rF...(h)]h*]h+]h
+00006a00: 2c5d 682f 5d75 681f 6a40 0400 0068 335d  ,]h/]uh.j@...h3]
+00006a10: 7247 0400 0028 6add 0100 0029 8172 4804  rG...(j....).rH.
+00006a20: 0000 7d72 4904 0000 2868 1e58 0500 0000  ..}rI...(h.X....
+00006a30: 6d61 7869 7468 277d 724a 0400 0028 682c  maxith'}rJ...(h,
+00006a40: 5d68 2b5d 6ae1 0100 0088 6829 5d68 2a5d  ]h+]j.....h)]h*]
+00006a50: 682f 5d75 681f 6a44 0400 0068 335d 724b  h/]uh.jD...h3]rK
+00006a60: 0400 0068 5258 0500 0000 6d61 7869 7472  ...hRX....maxitr
+00006a70: 4c04 0000 8581 724d 0400 007d 724e 0400  L.....rM...}rN..
+00006a80: 0028 681e 5500 681f 6a48 0400 0075 6261  .(h.U.h.jH...uba
+00006a90: 6825 6ae6 0100 0075 6268 5258 0200 0000  h%j....ubhRX....
+00006aa0: 2028 724f 0400 0085 8172 5004 0000 7d72   (rO.....rP...}r
+00006ab0: 5104 0000 2868 1e55 0068 1f6a 4404 0000  Q...(h.U.h.jD...
+00006ac0: 7562 683c 2981 7252 0400 007d 7253 0400  ubh<).rR...}rS..
+00006ad0: 0028 681e 5500 6827 7d72 5404 0000 2855  .(h.U.h'}rT...(U
+00006ae0: 0772 6566 7479 7065 68f2 6ae1 0100 0088  .reftypeh.j.....
+00006af0: 5509 7265 6674 6172 6765 7458 0300 0000  U.reftargetX....
+00006b00: 696e 7472 5504 0000 5509 7265 6664 6f6d  intrU...U.refdom
+00006b10: 6169 6e68 de68 2c5d 682b 5d55 0b72 6566  ainh.h,]h+]U.ref
+00006b20: 6578 706c 6963 6974 8968 295d 682a 5d68  explicit.h)]h*]h
+00006b30: 2f5d 7568 1f6a 4404 0000 6833 5d72 5604  /]uh.jD...h3]rV.
+00006b40: 0000 6aef 0100 0029 8172 5704 0000 7d72  ..j....).rW...}r
+00006b50: 5804 0000 2868 1e6a 5504 0000 6827 7d72  X...(h.jU...h'}r
+00006b60: 5904 0000 2868 295d 682a 5d68 2b5d 682c  Y...(h)]h*]h+]h,
+00006b70: 5d68 2f5d 7568 1f6a 5204 0000 6833 5d72  ]h/]uh.jR...h3]r
+00006b80: 5a04 0000 6852 5803 0000 0069 6e74 725b  Z...hRX....intr[
+00006b90: 0400 0085 8172 5c04 0000 7d72 5d04 0000  .....r\...}r]...
+00006ba0: 2868 1e55 0068 1f6a 5704 0000 7562 6168  (h.U.h.jW...ubah
+00006bb0: 256a f701 0000 7562 6168 2568 4075 6268  %j....ubah%h@ubh
+00006bc0: 5258 0100 0000 2985 8172 5e04 0000 7d72  RX....)..r^...}r
+00006bd0: 5f04 0000 2868 1e55 0068 1f6a 4404 0000  _...(h.U.h.jD...
+00006be0: 7562 6852 5805 0000 0020 e280 9320 7260  ubhRX.... ... r`
+00006bf0: 0400 0085 8172 6104 0000 7d72 6204 0000  .....ra...}rb...
+00006c00: 2868 1e55 0068 1f6a 4404 0000 7562 6852  (h.U.h.jD...ubhR
+00006c10: 584e 0000 004d 6178 696d 756d 206e 756d  XN...Maximum num
+00006c20: 6265 7220 6f66 2066 756e 6374 696f 6e20  ber of function 
+00006c30: 6576 616c 7561 7469 6f6e 7320 696e 2073  evaluations in s
+00006c40: 6561 7263 680a 666f 7220 6d69 6e69 6d75  earch.for minimu
+00006c50: 6d3b 2064 6566 6175 6c74 2069 7320 3130  m; default is 10
+00006c60: 3030 2e72 6304 0000 8581 7264 0400 007d  00.rc.....rd...}
+00006c70: 7265 0400 0028 681e 584e 0000 004d 6178  re...(h.XN...Max
+00006c80: 696d 756d 206e 756d 6265 7220 6f66 2066  imum number of f
+00006c90: 756e 6374 696f 6e20 6576 616c 7561 7469  unction evaluati
+00006ca0: 6f6e 7320 696e 2073 6561 7263 680a 666f  ons in search.fo
+00006cb0: 7220 6d69 6e69 6d75 6d3b 2064 6566 6175  r minimum; defau
+00006cc0: 6c74 2069 7320 3130 3030 2e68 234e 6831  lt is 1000.h#Nh1
+00006cd0: 4e68 3268 0268 1f6a 4404 0000 7562 6568  Nh2h.h.jD...ubeh
+00006ce0: 2568 9a75 6261 6825 6a00 0200 0075 6265  %h.ubah%j....ube
+00006cf0: 6825 550b 6275 6c6c 6574 5f6c 6973 7472  h%U.bullet_listr
+00006d00: 6604 0000 7562 6168 2555 0a66 6965 6c64  f...ubah%U.field
+00006d10: 5f62 6f64 7972 6704 0000 7562 6568 2555  _bodyrg...ubeh%U
+00006d20: 0566 6965 6c64 7268 0400 0075 6261 7562  .fieldrh...ubaub
+00006d30: 6897 2981 7269 0400 007d 726a 0400 0028  h.).ri...}rj...(
+00006d40: 681e 58cf 0000 004f 7468 6572 2061 7267  h.X....Other arg
+00006d50: 756d 656e 7473 2069 6e63 6c75 6465 3a20  uments include: 
+00006d60: 6060 785f 6a61 6360 602c 2060 606c 6f73  ``x_jac``, ``los
+00006d70: 7360 602c 2060 6074 725f 736f 6c76 6572  s``, ``tr_solver
+00006d80: 6060 2c0a 6060 665f 7363 616c 6560 602c  ``,.``f_scale``,
+00006d90: 2060 6074 725f 6f70 7469 6f6e 7360 602c   ``tr_options``,
+00006da0: 2060 6062 6f75 6e64 7360 602e 2053 6565   ``bounds``. See
+00006db0: 2074 6865 2064 6f63 756d 656e 7461 7469   the documentati
+00006dc0: 6f6e 2066 6f72 0a60 6073 6369 7079 2e6f  on for.``scipy.o
+00006dd0: 7074 696d 697a 652e 6c65 6173 745f 7371  ptimize.least_sq
+00006de0: 7561 7265 7360 6020 666f 7220 696e 666f  uares`` for info
+00006df0: 726d 6174 696f 6e20 6162 6f75 7420 7468  rmation about th
+00006e00: 6573 6520 616e 6420 6f74 6865 720a 6f70  ese and other.op
+00006e10: 7469 6f6e 732e 681f 6a51 0100 0068 236a  tions.h.jQ...h#j
+00006e20: 5901 0000 6825 689a 6827 7d72 6b04 0000  Y...h%h.h'}rk...
+00006e30: 2868 295d 682a 5d68 2b5d 682c 5d68 2f5d  (h)]h*]h+]h,]h/]
+00006e40: 7568 314b 3868 3268 0268 335d 726c 0400  uh1K8h2h.h3]rl..
+00006e50: 0028 6852 5819 0000 004f 7468 6572 2061  .(hRX....Other a
+00006e60: 7267 756d 656e 7473 2069 6e63 6c75 6465  rguments include
+00006e70: 3a20 726d 0400 0085 8172 6e04 0000 7d72  : rm.....rn...}r
+00006e80: 6f04 0000 2868 1e58 1900 0000 4f74 6865  o...(h.X....Othe
+00006e90: 7220 6172 6775 6d65 6e74 7320 696e 636c  r arguments incl
+00006ea0: 7564 653a 2068 234e 6831 4e68 3268 0268  ude: h#Nh1Nh2h.h
+00006eb0: 1f6a 6904 0000 7562 684a 2981 7270 0400  .ji...ubhJ).rp..
+00006ec0: 007d 7271 0400 0028 681e 5809 0000 0060  .}rq...(h.X....`
+00006ed0: 6078 5f6a 6163 6060 6827 7d72 7204 0000  `x_jac``h'}rr...
+00006ee0: 2868 295d 682a 5d68 2b5d 682c 5d68 2f5d  (h)]h*]h+]h,]h/]
+00006ef0: 7568 1f6a 6904 0000 6833 5d72 7304 0000  uh.ji...h3]rs...
+00006f00: 6852 5805 0000 0078 5f6a 6163 7274 0400  hRX....x_jacrt..
+00006f10: 0085 8172 7504 0000 7d72 7604 0000 2868  ...ru...}rv...(h
+00006f20: 1e55 0068 1f6a 7004 0000 7562 6168 2568  .U.h.jp...ubah%h
+00006f30: 5675 6268 5258 0200 0000 2c20 7277 0400  VubhRX...., rw..
+00006f40: 0085 8172 7804 0000 7d72 7904 0000 2868  ...rx...}ry...(h
+00006f50: 1e58 0200 0000 2c20 727a 0400 0068 234e  .X...., rz...h#N
+00006f60: 6831 4e68 3268 0268 1f6a 6904 0000 7562  h1Nh2h.h.ji...ub
+00006f70: 684a 2981 727b 0400 007d 727c 0400 0028  hJ).r{...}r|...(
+00006f80: 681e 5808 0000 0060 606c 6f73 7360 6068  h.X....``loss``h
+00006f90: 277d 727d 0400 0028 6829 5d68 2a5d 682b  '}r}...(h)]h*]h+
+00006fa0: 5d68 2c5d 682f 5d75 681f 6a69 0400 0068  ]h,]h/]uh.ji...h
+00006fb0: 335d 727e 0400 0068 5258 0400 0000 6c6f  3]r~...hRX....lo
+00006fc0: 7373 727f 0400 0085 8172 8004 0000 7d72  ssr......r....}r
+00006fd0: 8104 0000 2868 1e55 0068 1f6a 7b04 0000  ....(h.U.h.j{...
+00006fe0: 7562 6168 2568 5675 6268 5258 0200 0000  ubah%hVubhRX....
+00006ff0: 2c20 7282 0400 0085 8172 8304 0000 7d72  , r......r....}r
+00007000: 8404 0000 2868 1e58 0200 0000 2c20 681f  ....(h.X...., h.
+00007010: 6a69 0400 0075 6268 4a29 8172 8504 0000  ji...ubhJ).r....
+00007020: 7d72 8604 0000 2868 1e58 0d00 0000 6060  }r....(h.X....``
+00007030: 7472 5f73 6f6c 7665 7260 6068 277d 7287  tr_solver``h'}r.
+00007040: 0400 0028 6829 5d68 2a5d 682b 5d68 2c5d  ...(h)]h*]h+]h,]
+00007050: 682f 5d75 681f 6a69 0400 0068 335d 7288  h/]uh.ji...h3]r.
+00007060: 0400 0068 5258 0900 0000 7472 5f73 6f6c  ...hRX....tr_sol
+00007070: 7665 7272 8904 0000 8581 728a 0400 007d  verr......r....}
+00007080: 728b 0400 0028 681e 5500 681f 6a85 0400  r....(h.U.h.j...
+00007090: 0075 6261 6825 6856 7562 6852 5802 0000  .ubah%hVubhRX...
+000070a0: 002c 0a72 8c04 0000 8581 728d 0400 007d  .,.r......r....}
+000070b0: 728e 0400 0028 681e 5802 0000 002c 0a68  r....(h.X....,.h
+000070c0: 234e 6831 4e68 3268 0268 1f6a 6904 0000  #Nh1Nh2h.h.ji...
+000070d0: 7562 684a 2981 728f 0400 007d 7290 0400  ubhJ).r....}r...
+000070e0: 0028 681e 580b 0000 0060 6066 5f73 6361  .(h.X....``f_sca
+000070f0: 6c65 6060 6827 7d72 9104 0000 2868 295d  le``h'}r....(h)]
+00007100: 682a 5d68 2b5d 682c 5d68 2f5d 7568 1f6a  h*]h+]h,]h/]uh.j
+00007110: 6904 0000 6833 5d72 9204 0000 6852 5807  i...h3]r....hRX.
+00007120: 0000 0066 5f73 6361 6c65 7293 0400 0085  ...f_scaler.....
+00007130: 8172 9404 0000 7d72 9504 0000 2868 1e55  .r....}r....(h.U
+00007140: 0068 1f6a 8f04 0000 7562 6168 2568 5675  .h.j....ubah%hVu
+00007150: 6268 5258 0200 0000 2c20 7296 0400 0085  bhRX...., r.....
+00007160: 8172 9704 0000 7d72 9804 0000 2868 1e58  .r....}r....(h.X
+00007170: 0200 0000 2c20 681f 6a69 0400 0075 6268  ...., h.ji...ubh
+00007180: 4a29 8172 9904 0000 7d72 9a04 0000 2868  J).r....}r....(h
+00007190: 1e58 0e00 0000 6060 7472 5f6f 7074 696f  .X....``tr_optio
+000071a0: 6e73 6060 6827 7d72 9b04 0000 2868 295d  ns``h'}r....(h)]
+000071b0: 682a 5d68 2b5d 682c 5d68 2f5d 7568 1f6a  h*]h+]h,]h/]uh.j
+000071c0: 6904 0000 6833 5d72 9c04 0000 6852 580a  i...h3]r....hRX.
+000071d0: 0000 0074 725f 6f70 7469 6f6e 7372 9d04  ...tr_optionsr..
+000071e0: 0000 8581 729e 0400 007d 729f 0400 0028  ....r....}r....(
+000071f0: 681e 5500 681f 6a99 0400 0075 6261 6825  h.U.h.j....ubah%
+00007200: 6856 7562 6852 5802 0000 002c 2072 a004  hVubhRX...., r..
+00007210: 0000 8581 72a1 0400 007d 72a2 0400 0028  ....r....}r....(
+00007220: 681e 6a7a 0400 0068 1f6a 6904 0000 7562  h.jz...h.ji...ub
+00007230: 684a 2981 72a3 0400 007d 72a4 0400 0028  hJ).r....}r....(
+00007240: 681e 580a 0000 0060 6062 6f75 6e64 7360  h.X....``bounds`
+00007250: 6068 277d 72a5 0400 0028 6829 5d68 2a5d  `h'}r....(h)]h*]
+00007260: 682b 5d68 2c5d 682f 5d75 681f 6a69 0400  h+]h,]h/]uh.ji..
+00007270: 0068 335d 72a6 0400 0068 5258 0600 0000  .h3]r....hRX....
+00007280: 626f 756e 6473 72a7 0400 0085 8172 a804  boundsr......r..
+00007290: 0000 7d72 a904 0000 2868 1e55 0068 1f6a  ..}r....(h.U.h.j
+000072a0: a304 0000 7562 6168 2568 5675 6268 5258  ....ubah%hVubhRX
+000072b0: 1c00 0000 2e20 5365 6520 7468 6520 646f  ..... See the do
+000072c0: 6375 6d65 6e74 6174 696f 6e20 666f 720a  cumentation for.
+000072d0: 72aa 0400 0085 8172 ab04 0000 7d72 ac04  r......r....}r..
+000072e0: 0000 2868 1e58 1c00 0000 2e20 5365 6520  ..(h.X..... See 
+000072f0: 7468 6520 646f 6375 6d65 6e74 6174 696f  the documentatio
+00007300: 6e20 666f 720a 6823 4e68 314e 6832 6802  n for.h#Nh1Nh2h.
+00007310: 681f 6a69 0400 0075 6268 4a29 8172 ad04  h.ji...ubhJ).r..
+00007320: 0000 7d72 ae04 0000 2868 1e58 2000 0000  ..}r....(h.X ...
+00007330: 6060 7363 6970 792e 6f70 7469 6d69 7a65  ``scipy.optimize
+00007340: 2e6c 6561 7374 5f73 7175 6172 6573 6060  .least_squares``
+00007350: 6827 7d72 af04 0000 2868 295d 682a 5d68  h'}r....(h)]h*]h
+00007360: 2b5d 682c 5d68 2f5d 7568 1f6a 6904 0000  +]h,]h/]uh.ji...
+00007370: 6833 5d72 b004 0000 6852 581c 0000 0073  h3]r....hRX....s
+00007380: 6369 7079 2e6f 7074 696d 697a 652e 6c65  cipy.optimize.le
+00007390: 6173 745f 7371 7561 7265 7372 b104 0000  ast_squaresr....
+000073a0: 8581 72b2 0400 007d 72b3 0400 0028 681e  ..r....}r....(h.
+000073b0: 5500 681f 6aad 0400 0075 6261 6825 6856  U.h.j....ubah%hV
+000073c0: 7562 6852 582f 0000 0020 666f 7220 696e  ubhRX/... for in
+000073d0: 666f 726d 6174 696f 6e20 6162 6f75 7420  formation about 
+000073e0: 7468 6573 6520 616e 6420 6f74 6865 720a  these and other.
+000073f0: 6f70 7469 6f6e 732e 72b4 0400 0085 8172  options.r......r
+00007400: b504 0000 7d72 b604 0000 2868 1e58 2f00  ....}r....(h.X/.
+00007410: 0000 2066 6f72 2069 6e66 6f72 6d61 7469  .. for informati
+00007420: 6f6e 2061 626f 7574 2074 6865 7365 2061  on about these a
+00007430: 6e64 206f 7468 6572 0a6f 7074 696f 6e73  nd other.options
+00007440: 2e68 234e 6831 4e68 3268 0268 1f6a 6904  .h#Nh1Nh2h.h.ji.
+00007450: 0000 7562 6575 6268 9729 8172 b704 0000  ..ubeubh.).r....
+00007460: 7d72 b804 0000 2868 1e58 4a00 0000 3a63  }r....(h.XJ...:c
+00007470: 6c61 7373 3a60 6c73 7166 6974 2e73 6369  lass:`lsqfit.sci
+00007480: 7079 5f6c 6561 7374 5f73 7175 6172 6573  py_least_squares
+00007490: 6020 6f62 6a65 6374 7320 6861 7665 2074  ` objects have t
+000074a0: 6865 2066 6f6c 6c6f 7769 6e67 0a61 7474  he following.att
+000074b0: 7269 6275 7465 732e 681f 6a51 0100 0068  ributes.h.jQ...h
+000074c0: 236a 5901 0000 6825 689a 6827 7d72 b904  #jY...h%h.h'}r..
+000074d0: 0000 2868 295d 682a 5d68 2b5d 682c 5d68  ..(h)]h*]h+]h,]h
+000074e0: 2f5d 7568 314b 3d68 3268 0268 335d 72ba  /]uh1K=h2h.h3]r.
+000074f0: 0400 0028 683c 2981 72bb 0400 007d 72bc  ...(h<).r....}r.
+00007500: 0400 0028 681e 5823 0000 003a 636c 6173  ...(h.X#...:clas
+00007510: 733a 606c 7371 6669 742e 7363 6970 795f  s:`lsqfit.scipy_
+00007520: 6c65 6173 745f 7371 7561 7265 7360 72bd  least_squares`r.
+00007530: 0400 0068 1f6a b704 0000 6823 6a59 0100  ...h.j....h#jY..
+00007540: 0068 2568 4068 277d 72be 0400 0028 5507  .h%h@h'}r....(U.
+00007550: 7265 6674 7970 6558 0500 0000 636c 6173  reftypeX....clas
+00007560: 7368 4289 6843 581a 0000 006c 7371 6669  shB.hCX....lsqfi
+00007570: 742e 7363 6970 795f 6c65 6173 745f 7371  t.scipy_least_sq
+00007580: 7561 7265 7355 0972 6566 646f 6d61 696e  uaresU.refdomain
+00007590: 5802 0000 0070 7972 bf04 0000 682c 5d68  X....pyr....h,]h
+000075a0: 2b5d 550b 7265 6665 7870 6c69 6369 7489  +]U.refexplicit.
+000075b0: 6829 5d68 2a5d 682f 5d68 4568 4668 4768  h)]h*]h/]hEhFhGh
+000075c0: f168 4868 ed75 6831 4b3d 6833 5d72 c004  .hHh.uh1K=h3]r..
+000075d0: 0000 684a 2981 72c1 0400 007d 72c2 0400  ..hJ).r....}r...
+000075e0: 0028 681e 6abd 0400 0068 277d 72c3 0400  .(h.j....h'}r...
+000075f0: 0028 6829 5d68 2a5d 72c4 0400 0028 684f  .(h)]h*]r....(hO
+00007600: 6abf 0400 0058 0800 0000 7079 2d63 6c61  j....X....py-cla
+00007610: 7373 72c5 0400 0065 682b 5d68 2c5d 682f  ssr....eh+]h,]h/
+00007620: 5d75 681f 6abb 0400 0068 335d 72c6 0400  ]uh.j....h3]r...
+00007630: 0068 5258 1a00 0000 6c73 7166 6974 2e73  .hRX....lsqfit.s
+00007640: 6369 7079 5f6c 6561 7374 5f73 7175 6172  cipy_least_squar
+00007650: 6573 72c7 0400 0085 8172 c804 0000 7d72  esr......r....}r
+00007660: c904 0000 2868 1e55 0068 1f6a c104 0000  ....(h.U.h.j....
+00007670: 7562 6168 2568 5675 6261 7562 6852 5827  ubah%hVubaubhRX'
+00007680: 0000 0020 6f62 6a65 6374 7320 6861 7665  ... objects have
+00007690: 2074 6865 2066 6f6c 6c6f 7769 6e67 0a61   the following.a
+000076a0: 7474 7269 6275 7465 732e 72ca 0400 0085  ttributes.r.....
+000076b0: 8172 cb04 0000 7d72 cc04 0000 2868 1e58  .r....}r....(h.X
+000076c0: 2700 0000 206f 626a 6563 7473 2068 6176  '... objects hav
+000076d0: 6520 7468 6520 666f 6c6c 6f77 696e 670a  e the following.
+000076e0: 6174 7472 6962 7574 6573 2e68 234e 6831  attributes.h#Nh1
+000076f0: 4e68 3268 0268 1f6a b704 0000 7562 6575  Nh2h.h.j....ubeu
+00007700: 6268 cf29 8172 cd04 0000 7d72 ce04 0000  bh.).r....}r....
+00007710: 2868 1e55 0068 1f6a 5101 0000 6823 6a59  (h.U.h.jQ...h#jY
+00007720: 0100 0068 2568 d268 277d 72cf 0400 0028  ...h%h.h'}r....(
+00007730: 682c 5d68 2b5d 6829 5d68 2a5d 682f 5d55  h,]h+]h)]h*]h/]U
+00007740: 0765 6e74 7269 6573 5d72 d004 0000 2868  .entries]r....(h
+00007750: d558 2800 0000 7820 286c 7371 6669 742e  .X(...x (lsqfit.
+00007760: 7363 6970 795f 6c65 6173 745f 7371 7561  scipy_least_squa
+00007770: 7265 7320 6174 7472 6962 7574 6529 6815  res attribute)h.
+00007780: 5500 4e74 72d1 0400 0061 7568 314e 6832  U.Ntr....auh1Nh2
+00007790: 6802 6833 5d75 6268 d729 8172 d204 0000  h.h3]ubh.).r....
+000077a0: 7d72 d304 0000 2868 1e55 0068 1f6a 5101  }r....(h.U.h.jQ.
+000077b0: 0000 6823 6a59 0100 0068 2568 da68 277d  ..h#jY...h%h.h'}
+000077c0: 72d4 0400 0028 68dc 8968 dd58 0200 0000  r....(h..h.X....
+000077d0: 7079 682c 5d68 2b5d 6829 5d68 2a5d 682f  pyh,]h+]h)]h*]h/
+000077e0: 5d68 df58 0900 0000 6174 7472 6962 7574  ]h.X....attribut
+000077f0: 6572 d504 0000 68e1 6ad5 0400 0075 6831  er....h.j....uh1
+00007800: 4e68 3268 0268 335d 72d6 0400 0028 68e3  Nh2h.h3]r....(h.
+00007810: 2981 72d7 0400 007d 72d8 0400 0028 681e  ).r....}r....(h.
+00007820: 5801 0000 0078 681f 6ad2 0400 0068 236a  X....xh.j....h#j
+00007830: 5901 0000 6825 68e7 6827 7d72 d904 0000  Y...h%h.h'}r....
+00007840: 2868 2c5d 72da 0400 0068 1561 68ea 68ed  (h,]r....h.ah.h.
+00007850: 682b 5d68 295d 682a 5d68 2f5d 72db 0400  h+]h)]h*]h/]r...
+00007860: 0068 1561 68f0 5815 0000 0073 6369 7079  .h.ah.X....scipy
+00007870: 5f6c 6561 7374 5f73 7175 6172 6573 2e78  _least_squares.x
+00007880: 68f2 68f1 68f3 8975 6831 4b43 6832 6802  h.h.h..uh1KCh2h.
+00007890: 6833 5d72 dc04 0000 6a09 0100 0029 8172  h3]r....j....).r
+000078a0: dd04 0000 7d72 de04 0000 2868 1e58 0100  ....}r....(h.X..
+000078b0: 0000 7868 1f6a d704 0000 6823 6a59 0100  ..xh.j....h#jY..
+000078c0: 0068 256a 0c01 0000 6827 7d72 df04 0000  .h%j....h'}r....
+000078d0: 2868 fa68 fb68 2c5d 682b 5d68 295d 682a  (h.h.h,]h+]h)]h*
+000078e0: 5d68 2f5d 7568 314b 4368 3268 0268 335d  ]h/]uh1KCh2h.h3]
+000078f0: 72e0 0400 0068 5258 0100 0000 7885 8172  r....hRX....x..r
+00007900: e104 0000 7d72 e204 0000 2868 1e55 0068  ....}r....(h.U.h
+00007910: 234e 6831 4e68 3268 0268 1f6a dd04 0000  #Nh1Nh2h.h.j....
+00007920: 7562 6175 6261 7562 6a50 0100 0029 8172  ubaubaubjP...).r
+00007930: e304 0000 7d72 e404 0000 2868 1e55 0068  ....}r....(h.U.h
+00007940: 1f6a d204 0000 6823 6a59 0100 0068 256a  .j....h#jY...h%j
+00007950: 5301 0000 6827 7d72 e504 0000 2868 295d  S...h'}r....(h)]
+00007960: 682a 5d68 2b5d 682c 5d68 2f5d 7568 314b  h*]h+]h,]h/]uh1K
+00007970: 4368 3268 0268 335d 72e6 0400 0068 9729  Ch2h.h3]r....h.)
+00007980: 8172 e704 0000 7d72 e804 0000 2868 1e58  .r....}r....(h.X
+00007990: 4300 0000 2a61 7272 6179 2a20 2d2d 204c  C...*array* -- L
+000079a0: 6f63 6174 696f 6e20 6f66 2074 6865 206d  ocation of the m
+000079b0: 6f73 7420 7265 6365 6e74 6c79 2063 6f6d  ost recently com
+000079c0: 7075 7465 6420 2862 6573 7429 2066 6974  puted (best) fit
+000079d0: 2070 6f69 6e74 2e68 1f6a e304 0000 6823   point.h.j....h#
+000079e0: 6a59 0100 0068 2568 9a68 277d 72e9 0400  jY...h%h.h'}r...
+000079f0: 0028 6829 5d68 2a5d 682b 5d68 2c5d 682f  .(h)]h*]h+]h,]h/
+00007a00: 5d75 6831 4b42 6832 6802 6833 5d72 ea04  ]uh1KBh2h.h3]r..
+00007a10: 0000 2863 646f 6375 7469 6c73 2e6e 6f64  ..(cdocutils.nod
+00007a20: 6573 0a65 6d70 6861 7369 730a 72eb 0400  es.emphasis.r...
+00007a30: 0029 8172 ec04 0000 7d72 ed04 0000 2868  .).r....}r....(h
+00007a40: 1e58 0700 0000 2a61 7272 6179 2a68 277d  .X....*array*h'}
+00007a50: 72ee 0400 0028 6829 5d68 2a5d 682b 5d68  r....(h)]h*]h+]h
+00007a60: 2c5d 682f 5d75 681f 6ae7 0400 0068 335d  ,]h/]uh.j....h3]
+00007a70: 72ef 0400 0068 5258 0500 0000 6172 7261  r....hRX....arra
+00007a80: 7972 f004 0000 8581 72f1 0400 007d 72f2  yr......r....}r.
+00007a90: 0400 0028 681e 5500 681f 6aec 0400 0075  ...(h.U.h.j....u
+00007aa0: 6261 6825 5508 656d 7068 6173 6973 72f3  bah%U.emphasisr.
+00007ab0: 0400 0075 6268 5258 3d00 0000 20e2 8093  ...ubhRX=... ...
+00007ac0: 204c 6f63 6174 696f 6e20 6f66 2074 6865   Location of the
+00007ad0: 206d 6f73 7420 7265 6365 6e74 6c79 2063   most recently c
+00007ae0: 6f6d 7075 7465 6420 2862 6573 7429 2066  omputed (best) f
+00007af0: 6974 2070 6f69 6e74 2e72 f404 0000 8581  it point.r......
+00007b00: 72f5 0400 007d 72f6 0400 0028 681e 583c  r....}r....(h.X<
+00007b10: 0000 0020 2d2d 204c 6f63 6174 696f 6e20  ... -- Location 
+00007b20: 6f66 2074 6865 206d 6f73 7420 7265 6365  of the most rece
+00007b30: 6e74 6c79 2063 6f6d 7075 7465 6420 2862  ntly computed (b
+00007b40: 6573 7429 2066 6974 2070 6f69 6e74 2e68  est) fit point.h
+00007b50: 234e 6831 4e68 3268 0268 1f6a e704 0000  #Nh1Nh2h.h.j....
+00007b60: 7562 6575 6261 7562 6575 6268 cf29 8172  ubeubaubeubh.).r
+00007b70: f704 0000 7d72 f804 0000 2868 1e55 0068  ....}r....(h.U.h
+00007b80: 1f6a 5101 0000 6823 6a59 0100 0068 2568  .jQ...h#jY...h%h
+00007b90: d268 277d 72f9 0400 0028 682c 5d68 2b5d  .h'}r....(h,]h+]
+00007ba0: 6829 5d68 2a5d 682f 5d55 0765 6e74 7269  h)]h*]h/]U.entri
+00007bb0: 6573 5d72 fa04 0000 2868 d558 2a00 0000  es]r....(h.X*...
+00007bc0: 636f 7620 286c 7371 6669 742e 7363 6970  cov (lsqfit.scip
+00007bd0: 795f 6c65 6173 745f 7371 7561 7265 7320  y_least_squares 
+00007be0: 6174 7472 6962 7574 6529 6811 5500 4e74  attribute)h.U.Nt
+00007bf0: 72fb 0400 0061 7568 314e 6832 6802 6833  r....auh1Nh2h.h3
+00007c00: 5d75 6268 d729 8172 fc04 0000 7d72 fd04  ]ubh.).r....}r..
+00007c10: 0000 2868 1e55 0068 1f6a 5101 0000 6823  ..(h.U.h.jQ...h#
+00007c20: 6a59 0100 0068 2568 da68 277d 72fe 0400  jY...h%h.h'}r...
+00007c30: 0028 68dc 8968 dd58 0200 0000 7079 682c  .(h..h.X....pyh,
+00007c40: 5d68 2b5d 6829 5d68 2a5d 682f 5d68 df58  ]h+]h)]h*]h/]h.X
+00007c50: 0900 0000 6174 7472 6962 7574 6572 ff04  ....attributer..
+00007c60: 0000 68e1 6aff 0400 0075 6831 4e68 3268  ..h.j....uh1Nh2h
+00007c70: 0268 335d 7200 0500 0028 68e3 2981 7201  .h3]r....(h.).r.
+00007c80: 0500 007d 7202 0500 0028 681e 5803 0000  ...}r....(h.X...
+00007c90: 0063 6f76 7203 0500 0068 1f6a fc04 0000  .covr....h.j....
+00007ca0: 6823 6a59 0100 0068 2568 e768 277d 7204  h#jY...h%h.h'}r.
+00007cb0: 0500 0028 682c 5d72 0505 0000 6811 6168  ...(h,]r....h.ah
+00007cc0: ea68 ed68 2b5d 6829 5d68 2a5d 682f 5d72  .h.h+]h)]h*]h/]r
+00007cd0: 0605 0000 6811 6168 f058 1700 0000 7363  ....h.ah.X....sc
+00007ce0: 6970 795f 6c65 6173 745f 7371 7561 7265  ipy_least_square
+00007cf0: 732e 636f 7668 f268 f168 f389 7568 314b  s.covh.h.h..uh1K
+00007d00: 4768 3268 0268 335d 7207 0500 006a 0901  Gh2h.h3]r....j..
+00007d10: 0000 2981 7208 0500 007d 7209 0500 0028  ..).r....}r....(
+00007d20: 681e 6a03 0500 0068 1f6a 0105 0000 6823  h.j....h.j....h#
+00007d30: 6a59 0100 0068 256a 0c01 0000 6827 7d72  jY...h%j....h'}r
+00007d40: 0a05 0000 2868 fa68 fb68 2c5d 682b 5d68  ....(h.h.h,]h+]h
+00007d50: 295d 682a 5d68 2f5d 7568 314b 4768 3268  )]h*]h/]uh1KGh2h
+00007d60: 0268 335d 720b 0500 0068 5258 0300 0000  .h3]r....hRX....
+00007d70: 636f 7672 0c05 0000 8581 720d 0500 007d  covr......r....}
+00007d80: 720e 0500 0028 681e 5500 6823 4e68 314e  r....(h.U.h#Nh1N
+00007d90: 6832 6802 681f 6a08 0500 0075 6261 7562  h2h.h.j....ubaub
+00007da0: 6175 626a 5001 0000 2981 720f 0500 007d  aubjP...).r....}
+00007db0: 7210 0500 0028 681e 5500 681f 6afc 0400  r....(h.U.h.j...
+00007dc0: 0068 236a 5901 0000 6825 6a53 0100 0068  .h#jY...h%jS...h
+00007dd0: 277d 7211 0500 0028 6829 5d68 2a5d 682b  '}r....(h)]h*]h+
+00007de0: 5d68 2c5d 682f 5d75 6831 4b47 6832 6802  ]h,]h/]uh1KGh2h.
+00007df0: 6833 5d72 1205 0000 6897 2981 7213 0500  h3]r....h.).r...
+00007e00: 007d 7214 0500 0028 681e 5832 0000 002a  .}r....(h.X2...*
+00007e10: 6172 7261 792a 202d 2d20 436f 7661 7269  array* -- Covari
+00007e20: 616e 6365 206d 6174 7269 7820 6174 2074  ance matrix at t
+00007e30: 6865 206d 696e 696d 756d 2070 6f69 6e74  he minimum point
+00007e40: 2e68 1f6a 0f05 0000 6823 6a59 0100 0068  .h.j....h#jY...h
+00007e50: 2568 9a68 277d 7215 0500 0028 6829 5d68  %h.h'}r....(h)]h
+00007e60: 2a5d 682b 5d68 2c5d 682f 5d75 6831 4b46  *]h+]h,]h/]uh1KF
+00007e70: 6832 6802 6833 5d72 1605 0000 286a eb04  h2h.h3]r....(j..
+00007e80: 0000 2981 7217 0500 007d 7218 0500 0028  ..).r....}r....(
+00007e90: 681e 5807 0000 002a 6172 7261 792a 6827  h.X....*array*h'
+00007ea0: 7d72 1905 0000 2868 295d 682a 5d68 2b5d  }r....(h)]h*]h+]
+00007eb0: 682c 5d68 2f5d 7568 1f6a 1305 0000 6833  h,]h/]uh.j....h3
+00007ec0: 5d72 1a05 0000 6852 5805 0000 0061 7272  ]r....hRX....arr
+00007ed0: 6179 721b 0500 0085 8172 1c05 0000 7d72  ayr......r....}r
+00007ee0: 1d05 0000 2868 1e55 0068 1f6a 1705 0000  ....(h.U.h.j....
+00007ef0: 7562 6168 256a f304 0000 7562 6852 582c  ubah%j....ubhRX,
+00007f00: 0000 0020 e280 9320 436f 7661 7269 616e  ... ... Covarian
+00007f10: 6365 206d 6174 7269 7820 6174 2074 6865  ce matrix at the
+00007f20: 206d 696e 696d 756d 2070 6f69 6e74 2e72   minimum point.r
+00007f30: 1e05 0000 8581 721f 0500 007d 7220 0500  ......r....}r ..
+00007f40: 0028 681e 582b 0000 0020 2d2d 2043 6f76  .(h.X+... -- Cov
+00007f50: 6172 6961 6e63 6520 6d61 7472 6978 2061  ariance matrix a
+00007f60: 7420 7468 6520 6d69 6e69 6d75 6d20 706f  t the minimum po
+00007f70: 696e 742e 6823 4e68 314e 6832 6802 681f  int.h#Nh1Nh2h.h.
+00007f80: 6a13 0500 0075 6265 7562 6175 6265 7562  j....ubeubaubeub
+00007f90: 68cf 2981 7221 0500 007d 7222 0500 0028  h.).r!...}r"...(
+00007fa0: 681e 5500 681f 6a51 0100 0068 236a 5901  h.U.h.jQ...h#jY.
+00007fb0: 0000 6825 68d2 6827 7d72 2305 0000 2868  ..h%h.h'}r#...(h
+00007fc0: 2c5d 682b 5d68 295d 682a 5d68 2f5d 5507  ,]h+]h)]h*]h/]U.
+00007fd0: 656e 7472 6965 735d 7224 0500 0028 68d5  entries]r$...(h.
+00007fe0: 5832 0000 0064 6573 6372 6970 7469 6f6e  X2...description
+00007ff0: 2028 6c73 7166 6974 2e73 6369 7079 5f6c   (lsqfit.scipy_l
+00008000: 6561 7374 5f73 7175 6172 6573 2061 7474  east_squares att
+00008010: 7269 6275 7465 2968 0655 004e 7472 2505  ribute)h.U.Ntr%.
+00008020: 0000 6175 6831 4e68 3268 0268 335d 7562  ..auh1Nh2h.h3]ub
+00008030: 68d7 2981 7226 0500 007d 7227 0500 0028  h.).r&...}r'...(
+00008040: 681e 5500 681f 6a51 0100 0068 236a 5901  h.U.h.jQ...h#jY.
+00008050: 0000 6825 68da 6827 7d72 2805 0000 2868  ..h%h.h'}r(...(h
+00008060: dc89 68dd 5802 0000 0070 7968 2c5d 682b  ..h.X....pyh,]h+
+00008070: 5d68 295d 682a 5d68 2f5d 68df 5809 0000  ]h)]h*]h/]h.X...
+00008080: 0061 7474 7269 6275 7465 7229 0500 0068  .attributer)...h
+00008090: e16a 2905 0000 7568 314e 6832 6802 6833  .j)...uh1Nh2h.h3
+000080a0: 5d72 2a05 0000 2868 e329 8172 2b05 0000  ]r*...(h.).r+...
+000080b0: 7d72 2c05 0000 2868 1e58 0b00 0000 6465  }r,...(h.X....de
+000080c0: 7363 7269 7074 696f 6e72 2d05 0000 681f  scriptionr-...h.
+000080d0: 6a26 0500 0068 236a 5901 0000 6825 68e7  j&...h#jY...h%h.
+000080e0: 6827 7d72 2e05 0000 2868 2c5d 722f 0500  h'}r....(h,]r/..
+000080f0: 0068 0661 68ea 68ed 682b 5d68 295d 682a  .h.ah.h.h+]h)]h*
+00008100: 5d68 2f5d 7230 0500 0068 0661 68f0 581f  ]h/]r0...h.ah.X.
+00008110: 0000 0073 6369 7079 5f6c 6561 7374 5f73  ...scipy_least_s
+00008120: 7175 6172 6573 2e64 6573 6372 6970 7469  quares.descripti
+00008130: 6f6e 68f2 68f1 68f3 8975 6831 4b4b 6832  onh.h.h..uh1KKh2
+00008140: 6802 6833 5d72 3105 0000 6a09 0100 0029  h.h3]r1...j....)
+00008150: 8172 3205 0000 7d72 3305 0000 2868 1e6a  .r2...}r3...(h.j
+00008160: 2d05 0000 681f 6a2b 0500 0068 236a 5901  -...h.j+...h#jY.
+00008170: 0000 6825 6a0c 0100 0068 277d 7234 0500  ..h%j....h'}r4..
+00008180: 0028 68fa 68fb 682c 5d68 2b5d 6829 5d68  .(h.h.h,]h+]h)]h
+00008190: 2a5d 682f 5d75 6831 4b4b 6832 6802 6833  *]h/]uh1KKh2h.h3
+000081a0: 5d72 3505 0000 6852 580b 0000 0064 6573  ]r5...hRX....des
+000081b0: 6372 6970 7469 6f6e 7236 0500 0085 8172  criptionr6.....r
+000081c0: 3705 0000 7d72 3805 0000 2868 1e55 0068  7...}r8...(h.U.h
+000081d0: 234e 6831 4e68 3268 0268 1f6a 3205 0000  #Nh1Nh2h.h.j2...
+000081e0: 7562 6175 6261 7562 6a50 0100 0029 8172  ubaubaubjP...).r
+000081f0: 3905 0000 7d72 3a05 0000 2868 1e55 0068  9...}r:...(h.U.h
+00008200: 1f6a 2605 0000 6823 6a59 0100 0068 256a  .j&...h#jY...h%j
+00008210: 5301 0000 6827 7d72 3b05 0000 2868 295d  S...h'}r;...(h)]
+00008220: 682a 5d68 2b5d 682c 5d68 2f5d 7568 314b  h*]h+]h,]h/]uh1K
+00008230: 4b68 3268 0268 335d 723c 0500 0068 9729  Kh2h.h3]r<...h.)
+00008240: 8172 3d05 0000 7d72 3e05 0000 2868 1e58  .r=...}r>...(h.X
+00008250: 3700 0000 2a73 7472 2a20 2d2d 2053 686f  7...*str* -- Sho
+00008260: 7274 2064 6573 6372 6970 7469 6f6e 206f  rt description o
+00008270: 6620 696e 7465 726e 616c 2066 6974 7465  f internal fitte
+00008280: 7220 7365 7474 696e 6773 2e68 1f6a 3905  r settings.h.j9.
+00008290: 0000 6823 6a59 0100 0068 2568 9a68 277d  ..h#jY...h%h.h'}
+000082a0: 723f 0500 0028 6829 5d68 2a5d 682b 5d68  r?...(h)]h*]h+]h
+000082b0: 2c5d 682f 5d75 6831 4b4a 6832 6802 6833  ,]h/]uh1KJh2h.h3
+000082c0: 5d72 4005 0000 286a eb04 0000 2981 7241  ]r@...(j....).rA
+000082d0: 0500 007d 7242 0500 0028 681e 5805 0000  ...}rB...(h.X...
+000082e0: 002a 7374 722a 6827 7d72 4305 0000 2868  .*str*h'}rC...(h
+000082f0: 295d 682a 5d68 2b5d 682c 5d68 2f5d 7568  )]h*]h+]h,]h/]uh
+00008300: 1f6a 3d05 0000 6833 5d72 4405 0000 6852  .j=...h3]rD...hR
+00008310: 5803 0000 0073 7472 7245 0500 0085 8172  X....strrE.....r
+00008320: 4605 0000 7d72 4705 0000 2868 1e55 0068  F...}rG...(h.U.h
+00008330: 1f6a 4105 0000 7562 6168 256a f304 0000  .jA...ubah%j....
+00008340: 7562 6852 5833 0000 0020 e280 9320 5368  ubhRX3... ... Sh
+00008350: 6f72 7420 6465 7363 7269 7074 696f 6e20  ort description 
+00008360: 6f66 2069 6e74 6572 6e61 6c20 6669 7474  of internal fitt
+00008370: 6572 2073 6574 7469 6e67 732e 7248 0500  er settings.rH..
+00008380: 0085 8172 4905 0000 7d72 4a05 0000 2868  ...rI...}rJ...(h
+00008390: 1e58 3200 0000 202d 2d20 5368 6f72 7420  .X2... -- Short 
+000083a0: 6465 7363 7269 7074 696f 6e20 6f66 2069  description of i
+000083b0: 6e74 6572 6e61 6c20 6669 7474 6572 2073  nternal fitter s
+000083c0: 6574 7469 6e67 732e 6823 4e68 314e 6832  ettings.h#Nh1Nh2
+000083d0: 6802 681f 6a3d 0500 0075 6265 7562 6175  h.h.j=...ubeubau
+000083e0: 6265 7562 68cf 2981 724b 0500 007d 724c  beubh.).rK...}rL
+000083f0: 0500 0028 681e 5500 681f 6a51 0100 0068  ...(h.U.h.jQ...h
+00008400: 236a 5901 0000 6825 68d2 6827 7d72 4d05  #jY...h%h.h'}rM.
+00008410: 0000 2868 2c5d 682b 5d68 295d 682a 5d68  ..(h,]h+]h)]h*]h
+00008420: 2f5d 5507 656e 7472 6965 735d 724e 0500  /]U.entries]rN..
+00008430: 0028 68d5 5828 0000 0066 2028 6c73 7166  .(h.X(...f (lsqf
+00008440: 6974 2e73 6369 7079 5f6c 6561 7374 5f73  it.scipy_least_s
+00008450: 7175 6172 6573 2061 7474 7269 6275 7465  quares attribute
+00008460: 2968 0855 004e 7472 4f05 0000 6175 6831  )h.U.NtrO...auh1
+00008470: 4e68 3268 0268 335d 7562 68d7 2981 7250  Nh2h.h3]ubh.).rP
+00008480: 0500 007d 7251 0500 0028 681e 5500 681f  ...}rQ...(h.U.h.
+00008490: 6a51 0100 0068 236a 5901 0000 6825 68da  jQ...h#jY...h%h.
+000084a0: 6827 7d72 5205 0000 2868 dc89 68dd 5802  h'}rR...(h..h.X.
+000084b0: 0000 0070 7968 2c5d 682b 5d68 295d 682a  ...pyh,]h+]h)]h*
+000084c0: 5d68 2f5d 68df 5809 0000 0061 7474 7269  ]h/]h.X....attri
+000084d0: 6275 7465 7253 0500 0068 e16a 5305 0000  buterS...h.jS...
+000084e0: 7568 314e 6832 6802 6833 5d72 5405 0000  uh1Nh2h.h3]rT...
+000084f0: 2868 e329 8172 5505 0000 7d72 5605 0000  (h.).rU...}rV...
+00008500: 2868 1e58 0100 0000 6668 1f6a 5005 0000  (h.X....fh.jP...
+00008510: 6823 6a59 0100 0068 2568 e768 277d 7257  h#jY...h%h.h'}rW
+00008520: 0500 0028 682c 5d72 5805 0000 6808 6168  ...(h,]rX...h.ah
+00008530: ea68 ed68 2b5d 6829 5d68 2a5d 682f 5d72  .h.h+]h)]h*]h/]r
+00008540: 5905 0000 6808 6168 f058 1500 0000 7363  Y...h.ah.X....sc
+00008550: 6970 795f 6c65 6173 745f 7371 7561 7265  ipy_least_square
+00008560: 732e 6668 f268 f168 f389 7568 314b 5068  s.fh.h.h..uh1KPh
+00008570: 3268 0268 335d 725a 0500 006a 0901 0000  2h.h3]rZ...j....
+00008580: 2981 725b 0500 007d 725c 0500 0028 681e  ).r[...}r\...(h.
+00008590: 5801 0000 0066 681f 6a55 0500 0068 236a  X....fh.jU...h#j
+000085a0: 5901 0000 6825 6a0c 0100 0068 277d 725d  Y...h%j....h'}r]
+000085b0: 0500 0028 68fa 68fb 682c 5d68 2b5d 6829  ...(h.h.h,]h+]h)
+000085c0: 5d68 2a5d 682f 5d75 6831 4b50 6832 6802  ]h*]h/]uh1KPh2h.
+000085d0: 6833 5d72 5e05 0000 6852 5801 0000 0066  h3]r^...hRX....f
+000085e0: 8581 725f 0500 007d 7260 0500 0028 681e  ..r_...}r`...(h.
+000085f0: 5500 6823 4e68 314e 6832 6802 681f 6a5b  U.h#Nh1Nh2h.h.j[
+00008600: 0500 0075 6261 7562 6175 626a 5001 0000  ...ubaubaubjP...
+00008610: 2981 7261 0500 007d 7262 0500 0028 681e  ).ra...}rb...(h.
+00008620: 5500 681f 6a50 0500 0068 236a 5901 0000  U.h.jP...h#jY...
+00008630: 6825 6a53 0100 0068 277d 7263 0500 0028  h%jS...h'}rc...(
+00008640: 6829 5d68 2a5d 682b 5d68 2c5d 682f 5d75  h)]h*]h+]h,]h/]u
+00008650: 6831 4b50 6832 6802 6833 5d72 6405 0000  h1KPh2h.h3]rd...
+00008660: 6897 2981 7265 0500 007d 7266 0500 0028  h.).re...}rf...(
+00008670: 681e 584d 0000 002a 6172 7261 792a 202d  h.XM...*array* -
+00008680: 2d20 4669 7420 6675 6e63 7469 6f6e 2076  - Fit function v
+00008690: 616c 7565 2060 6066 2878 2960 6020 6174  alue ``f(x)`` at
+000086a0: 2074 6865 206d 696e 696d 756d 2069 6e0a   the minimum in.
+000086b0: 7468 6520 6d6f 7374 2072 6563 656e 7420  the most recent 
+000086c0: 6669 742e 681f 6a61 0500 0068 236a 5901  fit.h.ja...h#jY.
+000086d0: 0000 6825 689a 6827 7d72 6705 0000 2868  ..h%h.h'}rg...(h
+000086e0: 295d 682a 5d68 2b5d 682c 5d68 2f5d 7568  )]h*]h+]h,]h/]uh
+000086f0: 314b 4e68 3268 0268 335d 7268 0500 0028  1KNh2h.h3]rh...(
+00008700: 6aeb 0400 0029 8172 6905 0000 7d72 6a05  j....).ri...}rj.
+00008710: 0000 2868 1e58 0700 0000 2a61 7272 6179  ..(h.X....*array
+00008720: 2a68 277d 726b 0500 0028 6829 5d68 2a5d  *h'}rk...(h)]h*]
+00008730: 682b 5d68 2c5d 682f 5d75 681f 6a65 0500  h+]h,]h/]uh.je..
+00008740: 0068 335d 726c 0500 0068 5258 0500 0000  .h3]rl...hRX....
+00008750: 6172 7261 7972 6d05 0000 8581 726e 0500  arrayrm.....rn..
+00008760: 007d 726f 0500 0028 681e 5500 681f 6a69  .}ro...(h.U.h.ji
+00008770: 0500 0075 6261 6825 6af3 0400 0075 6268  ...ubah%j....ubh
+00008780: 5258 1800 0000 20e2 8093 2046 6974 2066  RX.... ... Fit f
+00008790: 756e 6374 696f 6e20 7661 6c75 6520 7270  unction value rp
+000087a0: 0500 0085 8172 7105 0000 7d72 7205 0000  .....rq...}rr...
+000087b0: 2868 1e58 1700 0000 202d 2d20 4669 7420  (h.X.... -- Fit 
+000087c0: 6675 6e63 7469 6f6e 2076 616c 7565 2068  function value h
+000087d0: 234e 6831 4e68 3268 0268 1f6a 6505 0000  #Nh1Nh2h.h.je...
+000087e0: 7562 684a 2981 7273 0500 007d 7274 0500  ubhJ).rs...}rt..
+000087f0: 0028 681e 5808 0000 0060 6066 2878 2960  .(h.X....``f(x)`
+00008800: 6068 277d 7275 0500 0028 6829 5d68 2a5d  `h'}ru...(h)]h*]
+00008810: 682b 5d68 2c5d 682f 5d75 681f 6a65 0500  h+]h,]h/]uh.je..
+00008820: 0068 335d 7276 0500 0068 5258 0400 0000  .h3]rv...hRX....
+00008830: 6628 7829 7277 0500 0085 8172 7805 0000  f(x)rw.....rx...
+00008840: 7d72 7905 0000 2868 1e55 0068 1f6a 7305  }ry...(h.U.h.js.
+00008850: 0000 7562 6168 2568 5675 6268 5258 2700  ..ubah%hVubhRX'.
+00008860: 0000 2061 7420 7468 6520 6d69 6e69 6d75  .. at the minimu
+00008870: 6d20 696e 0a74 6865 206d 6f73 7420 7265  m in.the most re
+00008880: 6365 6e74 2066 6974 2e72 7a05 0000 8581  cent fit.rz.....
+00008890: 727b 0500 007d 727c 0500 0028 681e 5827  r{...}r|...(h.X'
+000088a0: 0000 0020 6174 2074 6865 206d 696e 696d  ... at the minim
+000088b0: 756d 2069 6e0a 7468 6520 6d6f 7374 2072  um in.the most r
+000088c0: 6563 656e 7420 6669 742e 6823 4e68 314e  ecent fit.h#Nh1N
+000088d0: 6832 6802 681f 6a65 0500 0075 6265 7562  h2h.h.je...ubeub
+000088e0: 6175 6265 7562 68cf 2981 727d 0500 007d  aubeubh.).r}...}
+000088f0: 727e 0500 0028 681e 5500 681f 6a51 0100  r~...(h.U.h.jQ..
+00008900: 0068 236a 5901 0000 6825 68d2 6827 7d72  .h#jY...h%h.h'}r
+00008910: 7f05 0000 2868 2c5d 682b 5d68 295d 682a  ....(h,]h+]h)]h*
+00008920: 5d68 2f5d 5507 656e 7472 6965 735d 7280  ]h/]U.entries]r.
+00008930: 0500 0028 68d5 5828 0000 004a 2028 6c73  ...(h.X(...J (ls
+00008940: 7166 6974 2e73 6369 7079 5f6c 6561 7374  qfit.scipy_least
+00008950: 5f73 7175 6172 6573 2061 7474 7269 6275  _squares attribu
+00008960: 7465 2968 0f55 004e 7472 8105 0000 6175  te)h.U.Ntr....au
+00008970: 6831 4e68 3268 0268 335d 7562 68d7 2981  h1Nh2h.h3]ubh.).
+00008980: 7282 0500 007d 7283 0500 0028 681e 5500  r....}r....(h.U.
+00008990: 681f 6a51 0100 0068 236a 5901 0000 6825  h.jQ...h#jY...h%
+000089a0: 68da 6827 7d72 8405 0000 2868 dc89 68dd  h.h'}r....(h..h.
+000089b0: 5802 0000 0070 7968 2c5d 682b 5d68 295d  X....pyh,]h+]h)]
+000089c0: 682a 5d68 2f5d 68df 5809 0000 0061 7474  h*]h/]h.X....att
+000089d0: 7269 6275 7465 7285 0500 0068 e16a 8505  ributer....h.j..
+000089e0: 0000 7568 314e 6832 6802 6833 5d72 8605  ..uh1Nh2h.h3]r..
+000089f0: 0000 2868 e329 8172 8705 0000 7d72 8805  ..(h.).r....}r..
+00008a00: 0000 2868 1e58 0100 0000 4a68 1f6a 8205  ..(h.X....Jh.j..
+00008a10: 0000 6823 6a59 0100 0068 2568 e768 277d  ..h#jY...h%h.h'}
+00008a20: 7289 0500 0028 682c 5d72 8a05 0000 680f  r....(h,]r....h.
+00008a30: 6168 ea68 ed68 2b5d 6829 5d68 2a5d 682f  ah.h.h+]h)]h*]h/
+00008a40: 5d72 8b05 0000 680f 6168 f058 1500 0000  ]r....h.ah.X....
+00008a50: 7363 6970 795f 6c65 6173 745f 7371 7561  scipy_least_squa
+00008a60: 7265 732e 4a68 f268 f168 f389 7568 314b  res.Jh.h.h..uh1K
+00008a70: 5468 3268 0268 335d 728c 0500 006a 0901  Th2h.h3]r....j..
+00008a80: 0000 2981 728d 0500 007d 728e 0500 0028  ..).r....}r....(
+00008a90: 681e 5801 0000 004a 681f 6a87 0500 0068  h.X....Jh.j....h
+00008aa0: 236a 5901 0000 6825 6a0c 0100 0068 277d  #jY...h%j....h'}
+00008ab0: 728f 0500 0028 68fa 68fb 682c 5d68 2b5d  r....(h.h.h,]h+]
+00008ac0: 6829 5d68 2a5d 682f 5d75 6831 4b54 6832  h)]h*]h/]uh1KTh2
+00008ad0: 6802 6833 5d72 9005 0000 6852 5801 0000  h.h3]r....hRX...
+00008ae0: 004a 8581 7291 0500 007d 7292 0500 0028  .J..r....}r....(
+00008af0: 681e 5500 6823 4e68 314e 6832 6802 681f  h.U.h#Nh1Nh2h.h.
+00008b00: 6a8d 0500 0075 6261 7562 6175 626a 5001  j....ubaubaubjP.
+00008b10: 0000 2981 7293 0500 007d 7294 0500 0028  ..).r....}r....(
+00008b20: 681e 5500 681f 6a82 0500 0068 236a 5901  h.U.h.j....h#jY.
+00008b30: 0000 6825 6a53 0100 0068 277d 7295 0500  ..h%jS...h'}r...
+00008b40: 0028 6829 5d68 2a5d 682b 5d68 2c5d 682f  .(h)]h*]h+]h,]h/
+00008b50: 5d75 6831 4b54 6832 6802 6833 5d72 9605  ]uh1KTh2h.h3]r..
+00008b60: 0000 6897 2981 7297 0500 007d 7298 0500  ..h.).r....}r...
+00008b70: 0028 681e 583e 0000 002a 6172 7261 792a  .(h.X>...*array*
+00008b80: 202d 2d20 4772 6164 6965 6e74 2060 604a   -- Gradient ``J
+00008b90: 5f69 6a20 3d20 6466 5f69 2f64 785b 6a5d  _ij = df_i/dx[j]
+00008ba0: 6060 2066 6f72 206d 6f73 7420 7265 6365  `` for most rece
+00008bb0: 6e74 2066 6974 2e68 1f6a 9305 0000 6823  nt fit.h.j....h#
+00008bc0: 6a59 0100 0068 2568 9a68 277d 7299 0500  jY...h%h.h'}r...
+00008bd0: 0028 6829 5d68 2a5d 682b 5d68 2c5d 682f  .(h)]h*]h+]h,]h/
+00008be0: 5d75 6831 4b53 6832 6802 6833 5d72 9a05  ]uh1KSh2h.h3]r..
+00008bf0: 0000 286a eb04 0000 2981 729b 0500 007d  ..(j....).r....}
+00008c00: 729c 0500 0028 681e 5807 0000 002a 6172  r....(h.X....*ar
+00008c10: 7261 792a 6827 7d72 9d05 0000 2868 295d  ray*h'}r....(h)]
+00008c20: 682a 5d68 2b5d 682c 5d68 2f5d 7568 1f6a  h*]h+]h,]h/]uh.j
+00008c30: 9705 0000 6833 5d72 9e05 0000 6852 5805  ....h3]r....hRX.
+00008c40: 0000 0061 7272 6179 729f 0500 0085 8172  ...arrayr......r
+00008c50: a005 0000 7d72 a105 0000 2868 1e55 0068  ....}r....(h.U.h
+00008c60: 1f6a 9b05 0000 7562 6168 256a f304 0000  .j....ubah%j....
+00008c70: 7562 6852 580e 0000 0020 e280 9320 4772  ubhRX.... ... Gr
+00008c80: 6164 6965 6e74 2072 a205 0000 8581 72a3  adient r......r.
+00008c90: 0500 007d 72a4 0500 0028 681e 580d 0000  ...}r....(h.X...
+00008ca0: 0020 2d2d 2047 7261 6469 656e 7420 6823  . -- Gradient h#
+00008cb0: 4e68 314e 6832 6802 681f 6a97 0500 0075  Nh1Nh2h.h.j....u
+00008cc0: 6268 4a29 8172 a505 0000 7d72 a605 0000  bhJ).r....}r....
+00008cd0: 2868 1e58 1500 0000 6060 4a5f 696a 203d  (h.X....``J_ij =
+00008ce0: 2064 665f 692f 6478 5b6a 5d60 6068 277d   df_i/dx[j]``h'}
+00008cf0: 72a7 0500 0028 6829 5d68 2a5d 682b 5d68  r....(h)]h*]h+]h
+00008d00: 2c5d 682f 5d75 681f 6a97 0500 0068 335d  ,]h/]uh.j....h3]
+00008d10: 72a8 0500 0068 5258 1100 0000 4a5f 696a  r....hRX....J_ij
+00008d20: 203d 2064 665f 692f 6478 5b6a 5d72 a905   = df_i/dx[j]r..
+00008d30: 0000 8581 72aa 0500 007d 72ab 0500 0028  ....r....}r....(
+00008d40: 681e 5500 681f 6aa5 0500 0075 6261 6825  h.U.h.j....ubah%
+00008d50: 6856 7562 6852 5815 0000 0020 666f 7220  hVubhRX.... for 
+00008d60: 6d6f 7374 2072 6563 656e 7420 6669 742e  most recent fit.
+00008d70: 72ac 0500 0085 8172 ad05 0000 7d72 ae05  r......r....}r..
+00008d80: 0000 2868 1e58 1500 0000 2066 6f72 206d  ..(h.X.... for m
+00008d90: 6f73 7420 7265 6365 6e74 2066 6974 2e68  ost recent fit.h
+00008da0: 234e 6831 4e68 3268 0268 1f6a 9705 0000  #Nh1Nh2h.h.j....
+00008db0: 7562 6575 6261 7562 6575 6268 cf29 8172  ubeubaubeubh.).r
+00008dc0: af05 0000 7d72 b005 0000 2868 1e55 0068  ....}r....(h.U.h
+00008dd0: 1f6a 5101 0000 6823 6a59 0100 0068 2568  .jQ...h#jY...h%h
+00008de0: d268 277d 72b1 0500 0028 682c 5d68 2b5d  .h'}r....(h,]h+]
+00008df0: 6829 5d68 2a5d 682f 5d55 0765 6e74 7269  h)]h*]h/]U.entri
+00008e00: 6573 5d72 b205 0000 2868 d558 2a00 0000  es]r....(h.X*...
+00008e10: 6e69 7420 286c 7371 6669 742e 7363 6970  nit (lsqfit.scip
+00008e20: 795f 6c65 6173 745f 7371 7561 7265 7320  y_least_squares 
+00008e30: 6174 7472 6962 7574 6529 680d 5500 4e74  attribute)h.U.Nt
+00008e40: 72b3 0500 0061 7568 314e 6832 6802 6833  r....auh1Nh2h.h3
+00008e50: 5d75 6268 d729 8172 b405 0000 7d72 b505  ]ubh.).r....}r..
+00008e60: 0000 2868 1e55 0068 1f6a 5101 0000 6823  ..(h.U.h.jQ...h#
+00008e70: 6a59 0100 0068 2568 da68 277d 72b6 0500  jY...h%h.h'}r...
+00008e80: 0028 68dc 8968 dd58 0200 0000 7079 682c  .(h..h.X....pyh,
+00008e90: 5d68 2b5d 6829 5d68 2a5d 682f 5d68 df58  ]h+]h)]h*]h/]h.X
+00008ea0: 0900 0000 6174 7472 6962 7574 6572 b705  ....attributer..
+00008eb0: 0000 68e1 6ab7 0500 0075 6831 4e68 3268  ..h.j....uh1Nh2h
+00008ec0: 0268 335d 72b8 0500 0028 68e3 2981 72b9  .h3]r....(h.).r.
+00008ed0: 0500 007d 72ba 0500 0028 681e 5803 0000  ...}r....(h.X...
+00008ee0: 006e 6974 72bb 0500 0068 1f6a b405 0000  .nitr....h.j....
+00008ef0: 6823 6a59 0100 0068 2568 e768 277d 72bc  h#jY...h%h.h'}r.
+00008f00: 0500 0028 682c 5d72 bd05 0000 680d 6168  ...(h,]r....h.ah
+00008f10: ea68 ed68 2b5d 6829 5d68 2a5d 682f 5d72  .h.h+]h)]h*]h/]r
+00008f20: be05 0000 680d 6168 f058 1700 0000 7363  ....h.ah.X....sc
+00008f30: 6970 795f 6c65 6173 745f 7371 7561 7265  ipy_least_square
+00008f40: 732e 6e69 7468 f268 f168 f389 7568 314b  s.nith.h.h..uh1K
+00008f50: 5968 3268 0268 335d 72bf 0500 006a 0901  Yh2h.h3]r....j..
+00008f60: 0000 2981 72c0 0500 007d 72c1 0500 0028  ..).r....}r....(
+00008f70: 681e 6abb 0500 0068 1f6a b905 0000 6823  h.j....h.j....h#
+00008f80: 6a59 0100 0068 256a 0c01 0000 6827 7d72  jY...h%j....h'}r
+00008f90: c205 0000 2868 fa68 fb68 2c5d 682b 5d68  ....(h.h.h,]h+]h
+00008fa0: 295d 682a 5d68 2f5d 7568 314b 5968 3268  )]h*]h/]uh1KYh2h
+00008fb0: 0268 335d 72c3 0500 0068 5258 0300 0000  .h3]r....hRX....
+00008fc0: 6e69 7472 c405 0000 8581 72c5 0500 007d  nitr......r....}
+00008fd0: 72c6 0500 0028 681e 5500 6823 4e68 314e  r....(h.U.h#Nh1N
+00008fe0: 6832 6802 681f 6ac0 0500 0075 6261 7562  h2h.h.j....ubaub
+00008ff0: 6175 626a 5001 0000 2981 72c7 0500 007d  aubjP...).r....}
+00009000: 72c8 0500 0028 681e 5500 681f 6ab4 0500  r....(h.U.h.j...
+00009010: 0068 236a 5901 0000 6825 6a53 0100 0068  .h#jY...h%jS...h
+00009020: 277d 72c9 0500 0028 6829 5d68 2a5d 682b  '}r....(h)]h*]h+
+00009030: 5d68 2c5d 682f 5d75 6831 4b59 6832 6802  ]h,]h/]uh1KYh2h.
+00009040: 6833 5d72 ca05 0000 6897 2981 72cb 0500  h3]r....h.).r...
+00009050: 007d 72cc 0500 0028 681e 584d 0000 002a  .}r....(h.XM...*
+00009060: 696e 742a 202d 2d20 4e75 6d62 6572 206f  int* -- Number o
+00009070: 6620 6675 6e63 7469 6f6e 2065 7661 6c75  f function evalu
+00009080: 6174 696f 6e73 2075 7365 6420 696e 206c  ations used in l
+00009090: 6173 7420 6669 7420 746f 2066 696e 640a  ast fit to find.
+000090a0: 7468 6520 6d69 6e69 6d75 6d2e 681f 6ac7  the minimum.h.j.
+000090b0: 0500 0068 236a 5901 0000 6825 689a 6827  ...h#jY...h%h.h'
+000090c0: 7d72 cd05 0000 2868 295d 682a 5d68 2b5d  }r....(h)]h*]h+]
+000090d0: 682c 5d68 2f5d 7568 314b 5768 3268 0268  h,]h/]uh1KWh2h.h
+000090e0: 335d 72ce 0500 0028 6aeb 0400 0029 8172  3]r....(j....).r
+000090f0: cf05 0000 7d72 d005 0000 2868 1e58 0500  ....}r....(h.X..
+00009100: 0000 2a69 6e74 2a68 277d 72d1 0500 0028  ..*int*h'}r....(
+00009110: 6829 5d68 2a5d 682b 5d68 2c5d 682f 5d75  h)]h*]h+]h,]h/]u
+00009120: 681f 6acb 0500 0068 335d 72d2 0500 0068  h.j....h3]r....h
+00009130: 5258 0300 0000 696e 7472 d305 0000 8581  RX....intr......
+00009140: 72d4 0500 007d 72d5 0500 0028 681e 5500  r....}r....(h.U.
+00009150: 681f 6acf 0500 0075 6261 6825 6af3 0400  h.j....ubah%j...
+00009160: 0075 6268 5258 4900 0000 20e2 8093 204e  .ubhRXI... ... N
+00009170: 756d 6265 7220 6f66 2066 756e 6374 696f  umber of functio
+00009180: 6e20 6576 616c 7561 7469 6f6e 7320 7573  n evaluations us
+00009190: 6564 2069 6e20 6c61 7374 2066 6974 2074  ed in last fit t
+000091a0: 6f20 6669 6e64 0a74 6865 206d 696e 696d  o find.the minim
+000091b0: 756d 2e72 d605 0000 8581 72d7 0500 007d  um.r......r....}
+000091c0: 72d8 0500 0028 681e 5848 0000 0020 2d2d  r....(h.XH... --
+000091d0: 204e 756d 6265 7220 6f66 2066 756e 6374   Number of funct
+000091e0: 696f 6e20 6576 616c 7561 7469 6f6e 7320  ion evaluations 
+000091f0: 7573 6564 2069 6e20 6c61 7374 2066 6974  used in last fit
+00009200: 2074 6f20 6669 6e64 0a74 6865 206d 696e   to find.the min
+00009210: 696d 756d 2e68 234e 6831 4e68 3268 0268  imum.h#Nh1Nh2h.h
+00009220: 1f6a cb05 0000 7562 6575 6261 7562 6575  .j....ubeubaubeu
+00009230: 6268 cf29 8172 d905 0000 7d72 da05 0000  bh.).r....}r....
+00009240: 2868 1e55 0068 1f6a 5101 0000 6823 6a59  (h.U.h.jQ...h#jY
+00009250: 0100 0068 2568 d268 277d 72db 0500 0028  ...h%h.h'}r....(
+00009260: 682c 5d68 2b5d 6829 5d68 2a5d 682f 5d55  h,]h+]h)]h*]h/]U
+00009270: 0765 6e74 7269 6573 5d72 dc05 0000 2868  .entries]r....(h
+00009280: d558 3900 0000 7374 6f70 7069 6e67 5f63  .X9...stopping_c
+00009290: 7269 7465 7269 6f6e 2028 6c73 7166 6974  riterion (lsqfit
+000092a0: 2e73 6369 7079 5f6c 6561 7374 5f73 7175  .scipy_least_squ
+000092b0: 6172 6573 2061 7474 7269 6275 7465 2968  ares attribute)h
+000092c0: 0e55 004e 7472 dd05 0000 6175 6831 4e68  .U.Ntr....auh1Nh
+000092d0: 3268 0268 335d 7562 68d7 2981 72de 0500  2h.h3]ubh.).r...
+000092e0: 007d 72df 0500 0028 681e 5500 681f 6a51  .}r....(h.U.h.jQ
+000092f0: 0100 0068 236a 5901 0000 6825 68da 6827  ...h#jY...h%h.h'
+00009300: 7d72 e005 0000 2868 dc89 68dd 5802 0000  }r....(h..h.X...
+00009310: 0070 7968 2c5d 682b 5d68 295d 682a 5d68  .pyh,]h+]h)]h*]h
+00009320: 2f5d 68df 5809 0000 0061 7474 7269 6275  /]h.X....attribu
+00009330: 7465 72e1 0500 0068 e16a e105 0000 7568  ter....h.j....uh
+00009340: 314e 6832 6802 6833 5d72 e205 0000 2868  1Nh2h.h3]r....(h
+00009350: e329 8172 e305 0000 7d72 e405 0000 2868  .).r....}r....(h
+00009360: 1e58 1200 0000 7374 6f70 7069 6e67 5f63  .X....stopping_c
+00009370: 7269 7465 7269 6f6e 72e5 0500 0068 1f6a  riterionr....h.j
+00009380: de05 0000 6823 6a59 0100 0068 2568 e768  ....h#jY...h%h.h
+00009390: 277d 72e6 0500 0028 682c 5d72 e705 0000  '}r....(h,]r....
+000093a0: 680e 6168 ea68 ed68 2b5d 6829 5d68 2a5d  h.ah.h.h+]h)]h*]
+000093b0: 682f 5d72 e805 0000 680e 6168 f058 2600  h/]r....h.ah.X&.
+000093c0: 0000 7363 6970 795f 6c65 6173 745f 7371  ..scipy_least_sq
+000093d0: 7561 7265 732e 7374 6f70 7069 6e67 5f63  uares.stopping_c
+000093e0: 7269 7465 7269 6f6e 68f2 68f1 68f3 8975  riterionh.h.h..u
+000093f0: 6831 4b66 6832 6802 6833 5d72 e905 0000  h1Kfh2h.h3]r....
+00009400: 6a09 0100 0029 8172 ea05 0000 7d72 eb05  j....).r....}r..
+00009410: 0000 2868 1e6a e505 0000 681f 6ae3 0500  ..(h.j....h.j...
+00009420: 0068 236a 5901 0000 6825 6a0c 0100 0068  .h#jY...h%j....h
+00009430: 277d 72ec 0500 0028 68fa 68fb 682c 5d68  '}r....(h.h.h,]h
+00009440: 2b5d 6829 5d68 2a5d 682f 5d75 6831 4b66  +]h)]h*]h/]uh1Kf
+00009450: 6832 6802 6833 5d72 ed05 0000 6852 5812  h2h.h3]r....hRX.
+00009460: 0000 0073 746f 7070 696e 675f 6372 6974  ...stopping_crit
+00009470: 6572 696f 6e72 ee05 0000 8581 72ef 0500  erionr......r...
+00009480: 007d 72f0 0500 0028 681e 5500 6823 4e68  .}r....(h.U.h#Nh
+00009490: 314e 6832 6802 681f 6aea 0500 0075 6261  1Nh2h.h.j....uba
+000094a0: 7562 6175 626a 5001 0000 2981 72f1 0500  ubaubjP...).r...
+000094b0: 007d 72f2 0500 0028 681e 5500 681f 6ade  .}r....(h.U.h.j.
+000094c0: 0500 0068 236a 5901 0000 6825 6a53 0100  ...h#jY...h%jS..
+000094d0: 0068 277d 72f3 0500 0028 6829 5d68 2a5d  .h'}r....(h)]h*]
+000094e0: 682b 5d68 2c5d 682f 5d75 6831 4b66 6832  h+]h,]h/]uh1Kfh2
+000094f0: 6802 6833 5d72 f405 0000 2868 9729 8172  h.h3]r....(h.).r
+00009500: f505 0000 7d72 f605 0000 2868 1e58 2400  ....}r....(h.X$.
+00009510: 0000 2a69 6e74 2a20 2d2d 2043 7269 7465  ..*int* -- Crite
+00009520: 7269 6f6e 2075 7365 6420 746f 0a73 746f  rion used to.sto
+00009530: 7020 6669 743a 681f 6af1 0500 0068 236a  p fit:h.j....h#j
+00009540: 5901 0000 6825 689a 6827 7d72 f705 0000  Y...h%h.h'}r....
+00009550: 2868 295d 682a 5d68 2b5d 682c 5d68 2f5d  (h)]h*]h+]h,]h/]
+00009560: 7568 314b 5c68 3268 0268 335d 72f8 0500  uh1K\h2h.h3]r...
+00009570: 0028 6aeb 0400 0029 8172 f905 0000 7d72  .(j....).r....}r
+00009580: fa05 0000 2868 1e58 0500 0000 2a69 6e74  ....(h.X....*int
+00009590: 2a68 277d 72fb 0500 0028 6829 5d68 2a5d  *h'}r....(h)]h*]
+000095a0: 682b 5d68 2c5d 682f 5d75 681f 6af5 0500  h+]h,]h/]uh.j...
+000095b0: 0068 335d 72fc 0500 0068 5258 0300 0000  .h3]r....hRX....
+000095c0: 696e 7472 fd05 0000 8581 72fe 0500 007d  intr......r....}
+000095d0: 72ff 0500 0028 681e 5500 681f 6af9 0500  r....(h.U.h.j...
+000095e0: 0075 6261 6825 6af3 0400 0075 6268 5258  .ubah%j....ubhRX
+000095f0: 2000 0000 20e2 8093 2043 7269 7465 7269   ... ... Criteri
+00009600: 6f6e 2075 7365 6420 746f 0a73 746f 7020  on used to.stop 
+00009610: 6669 743a 7200 0600 0085 8172 0106 0000  fit:r......r....
+00009620: 7d72 0206 0000 2868 1e58 1f00 0000 202d  }r....(h.X.... -
+00009630: 2d20 4372 6974 6572 696f 6e20 7573 6564  - Criterion used
+00009640: 2074 6f0a 7374 6f70 2066 6974 3a68 234e   to.stop fit:h#N
+00009650: 6831 4e68 3268 0268 1f6a f505 0000 7562  h1Nh2h.h.j....ub
+00009660: 6575 626a cf02 0000 2981 7203 0600 007d  eubj....).r....}
+00009670: 7204 0600 0028 681e 5500 681f 6af1 0500  r....(h.U.h.j...
+00009680: 0068 234e 6825 6ad2 0200 0068 277d 7205  .h#Nh%j....h'}r.
+00009690: 0600 0028 6829 5d68 2a5d 682b 5d68 2c5d  ...(h)]h*]h+]h,]
+000096a0: 682f 5d75 6831 4e68 3268 0268 335d 7206  h/]uh1Nh2h.h3]r.
+000096b0: 0600 0063 646f 6375 7469 6c73 2e6e 6f64  ...cdocutils.nod
+000096c0: 6573 0a65 6e75 6d65 7261 7465 645f 6c69  es.enumerated_li
+000096d0: 7374 0a72 0706 0000 2981 7208 0600 007d  st.r....).r....}
+000096e0: 7209 0600 0028 681e 5500 6827 7d72 0a06  r....(h.U.h'}r..
+000096f0: 0000 2855 0673 7566 6669 7872 0b06 0000  ..(U.suffixr....
+00009700: 5501 2e55 0573 7461 7274 720c 0600 004b  U..U.startr....K
+00009710: 0068 2c5d 682b 5d68 295d 5506 7072 6566  .h,]h+]h)]U.pref
+00009720: 6978 720d 0600 0055 0068 2a5d 682f 5d55  ixr....U.h*]h/]U
+00009730: 0865 6e75 6d74 7970 6572 0e06 0000 5506  .enumtyper....U.
+00009740: 6172 6162 6963 720f 0600 0075 681f 6a03  arabicr....uh.j.
+00009750: 0600 0068 335d 7210 0600 0028 6ad4 0100  ...h3]r....(j...
+00009760: 0029 8172 1106 0000 7d72 1206 0000 2868  .).r....}r....(h
+00009770: 1e58 1000 0000 6469 646e 2774 2063 6f6e  .X....didn't con
+00009780: 7665 7267 650a 6827 7d72 1306 0000 2868  verge.h'}r....(h
+00009790: 295d 682a 5d68 2b5d 682c 5d68 2f5d 7568  )]h*]h+]h,]h/]uh
+000097a0: 1f6a 0806 0000 6833 5d72 1406 0000 6897  .j....h3]r....h.
+000097b0: 2981 7215 0600 007d 7216 0600 0028 681e  ).r....}r....(h.
+000097c0: 580f 0000 0064 6964 6e27 7420 636f 6e76  X....didn't conv
+000097d0: 6572 6765 7217 0600 0068 1f6a 1106 0000  erger....h.j....
+000097e0: 6823 6a59 0100 0068 2568 9a68 277d 7218  h#jY...h%h.h'}r.
+000097f0: 0600 0028 6829 5d68 2a5d 682b 5d68 2c5d  ...(h)]h*]h+]h,]
+00009800: 682f 5d75 6831 4b5f 6833 5d72 1906 0000  h/]uh1K_h3]r....
+00009810: 6852 5811 0000 0064 6964 6ee2 8099 7420  hRX....didn...t 
+00009820: 636f 6e76 6572 6765 721a 0600 0085 8172  converger......r
+00009830: 1b06 0000 7d72 1c06 0000 2868 1e6a 1706  ....}r....(h.j..
+00009840: 0000 681f 6a15 0600 0075 6261 7562 6168  ..h.j....ubaubah
+00009850: 256a 0002 0000 7562 6ad4 0100 0029 8172  %j....ubj....).r
+00009860: 1d06 0000 7d72 1e06 0000 2868 1e58 3d00  ....}r....(h.X=.
+00009870: 0000 6060 7874 6f6c 203e 3d60 6020 7265  ..``xtol >=`` re
+00009880: 6c61 7469 7665 2063 6861 6e67 6520 696e  lative change in
+00009890: 2070 6172 616d 6574 6572 7320 6265 7477   parameters betw
+000098a0: 6565 6e20 6974 6572 6174 696f 6e73 0a68  een iterations.h
+000098b0: 277d 721f 0600 0028 6829 5d68 2a5d 682b  '}r....(h)]h*]h+
+000098c0: 5d68 2c5d 682f 5d75 681f 6a08 0600 0068  ]h,]h/]uh.j....h
+000098d0: 335d 7220 0600 0068 9729 8172 2106 0000  3]r ...h.).r!...
+000098e0: 7d72 2206 0000 2868 1e58 3c00 0000 6060  }r"...(h.X<...``
+000098f0: 7874 6f6c 203e 3d60 6020 7265 6c61 7469  xtol >=`` relati
+00009900: 7665 2063 6861 6e67 6520 696e 2070 6172  ve change in par
+00009910: 616d 6574 6572 7320 6265 7477 6565 6e20  ameters between 
+00009920: 6974 6572 6174 696f 6e73 681f 6a1d 0600  iterationsh.j...
+00009930: 0068 236a 5901 0000 6825 689a 6827 7d72  .h#jY...h%h.h'}r
+00009940: 2306 0000 2868 295d 682a 5d68 2b5d 682c  #...(h)]h*]h+]h,
+00009950: 5d68 2f5d 7568 314b 6168 335d 7224 0600  ]h/]uh1Kah3]r$..
+00009960: 0028 684a 2981 7225 0600 007d 7226 0600  .(hJ).r%...}r&..
+00009970: 0028 681e 580b 0000 0060 6078 746f 6c20  .(h.X....``xtol 
+00009980: 3e3d 6060 6827 7d72 2706 0000 2868 295d  >=``h'}r'...(h)]
+00009990: 682a 5d68 2b5d 682c 5d68 2f5d 7568 1f6a  h*]h+]h,]h/]uh.j
+000099a0: 2106 0000 6833 5d72 2806 0000 6852 5807  !...h3]r(...hRX.
+000099b0: 0000 0078 746f 6c20 3e3d 7229 0600 0085  ...xtol >=r)....
+000099c0: 8172 2a06 0000 7d72 2b06 0000 2868 1e55  .r*...}r+...(h.U
+000099d0: 0068 1f6a 2506 0000 7562 6168 2568 5675  .h.j%...ubah%hVu
+000099e0: 6268 5258 3100 0000 2072 656c 6174 6976  bhRX1... relativ
+000099f0: 6520 6368 616e 6765 2069 6e20 7061 7261  e change in para
+00009a00: 6d65 7465 7273 2062 6574 7765 656e 2069  meters between i
+00009a10: 7465 7261 7469 6f6e 7372 2c06 0000 8581  terationsr,.....
+00009a20: 722d 0600 007d 722e 0600 0028 681e 5831  r-...}r....(h.X1
+00009a30: 0000 0020 7265 6c61 7469 7665 2063 6861  ... relative cha
+00009a40: 6e67 6520 696e 2070 6172 616d 6574 6572  nge in parameter
+00009a50: 7320 6265 7477 6565 6e20 6974 6572 6174  s between iterat
+00009a60: 696f 6e73 681f 6a21 0600 0075 6265 7562  ionsh.j!...ubeub
+00009a70: 6168 256a 0002 0000 7562 6ad4 0100 0029  ah%j....ubj....)
+00009a80: 8172 2f06 0000 7d72 3006 0000 2868 1e58  .r/...}r0...(h.X
+00009a90: 3400 0000 6060 6774 6f6c 203e 3d60 6020  4...``gtol >=`` 
+00009aa0: 7265 6c61 7469 7665 2073 697a 6520 6f66  relative size of
+00009ab0: 2067 7261 6469 656e 7420 6f66 2060 6063   gradient of ``c
+00009ac0: 6869 2a2a 3260 600a 6827 7d72 3106 0000  hi**2``.h'}r1...
+00009ad0: 2868 295d 682a 5d68 2b5d 682c 5d68 2f5d  (h)]h*]h+]h,]h/]
+00009ae0: 7568 1f6a 0806 0000 6833 5d72 3206 0000  uh.j....h3]r2...
+00009af0: 6897 2981 7233 0600 007d 7234 0600 0028  h.).r3...}r4...(
+00009b00: 681e 5833 0000 0060 6067 746f 6c20 3e3d  h.X3...``gtol >=
+00009b10: 6060 2072 656c 6174 6976 6520 7369 7a65  `` relative size
+00009b20: 206f 6620 6772 6164 6965 6e74 206f 6620   of gradient of 
+00009b30: 6060 6368 692a 2a32 6060 681f 6a2f 0600  ``chi**2``h.j/..
+00009b40: 0068 236a 5901 0000 6825 689a 6827 7d72  .h#jY...h%h.h'}r
+00009b50: 3506 0000 2868 295d 682a 5d68 2b5d 682c  5...(h)]h*]h+]h,
+00009b60: 5d68 2f5d 7568 314b 6368 335d 7236 0600  ]h/]uh1Kch3]r6..
+00009b70: 0028 684a 2981 7237 0600 007d 7238 0600  .(hJ).r7...}r8..
+00009b80: 0028 681e 580b 0000 0060 6067 746f 6c20  .(h.X....``gtol 
+00009b90: 3e3d 6060 6827 7d72 3906 0000 2868 295d  >=``h'}r9...(h)]
+00009ba0: 682a 5d68 2b5d 682c 5d68 2f5d 7568 1f6a  h*]h+]h,]h/]uh.j
+00009bb0: 3306 0000 6833 5d72 3a06 0000 6852 5807  3...h3]r:...hRX.
+00009bc0: 0000 0067 746f 6c20 3e3d 723b 0600 0085  ...gtol >=r;....
+00009bd0: 8172 3c06 0000 7d72 3d06 0000 2868 1e55  .r<...}r=...(h.U
+00009be0: 0068 1f6a 3706 0000 7562 6168 2568 5675  .h.j7...ubah%hVu
+00009bf0: 6268 5258 1e00 0000 2072 656c 6174 6976  bhRX.... relativ
+00009c00: 6520 7369 7a65 206f 6620 6772 6164 6965  e size of gradie
+00009c10: 6e74 206f 6620 723e 0600 0085 8172 3f06  nt of r>.....r?.
+00009c20: 0000 7d72 4006 0000 2868 1e58 1e00 0000  ..}r@...(h.X....
+00009c30: 2072 656c 6174 6976 6520 7369 7a65 206f   relative size o
+00009c40: 6620 6772 6164 6965 6e74 206f 6620 681f  f gradient of h.
+00009c50: 6a33 0600 0075 6268 4a29 8172 4106 0000  j3...ubhJ).rA...
+00009c60: 7d72 4206 0000 2868 1e58 0a00 0000 6060  }rB...(h.X....``
+00009c70: 6368 692a 2a32 6060 6827 7d72 4306 0000  chi**2``h'}rC...
+00009c80: 2868 295d 682a 5d68 2b5d 682c 5d68 2f5d  (h)]h*]h+]h,]h/]
+00009c90: 7568 1f6a 3306 0000 6833 5d72 4406 0000  uh.j3...h3]rD...
+00009ca0: 6852 5806 0000 0063 6869 2a2a 3272 4506  hRX....chi**2rE.
+00009cb0: 0000 8581 7246 0600 007d 7247 0600 0028  ....rF...}rG...(
+00009cc0: 681e 5500 681f 6a41 0600 0075 6261 6825  h.U.h.jA...ubah%
+00009cd0: 6856 7562 6575 6261 6825 6a00 0200 0075  hVubeubah%j....u
+00009ce0: 626a d401 0000 2981 7248 0600 007d 7249  bj....).rH...}rI
+00009cf0: 0600 0028 681e 583c 0000 0060 6066 746f  ...(h.X<...``fto
+00009d00: 6c20 3e3d 6060 2072 656c 6174 6976 6520  l >=`` relative 
+00009d10: 6368 616e 6765 2069 6e20 6060 6368 692a  change in ``chi*
+00009d20: 2a32 6060 2062 6574 7765 656e 2069 7465  *2`` between ite
+00009d30: 7261 7469 6f6e 7372 4a06 0000 6827 7d72  rationsrJ...h'}r
+00009d40: 4b06 0000 2868 295d 682a 5d68 2b5d 682c  K...(h)]h*]h+]h,
+00009d50: 5d68 2f5d 7568 1f6a 0806 0000 6833 5d72  ]h/]uh.j....h3]r
+00009d60: 4c06 0000 6897 2981 724d 0600 007d 724e  L...h.).rM...}rN
+00009d70: 0600 0028 681e 6a4a 0600 0068 1f6a 4806  ...(h.jJ...h.jH.
+00009d80: 0000 6823 6a59 0100 0068 2568 9a68 277d  ..h#jY...h%h.h'}
+00009d90: 724f 0600 0028 6829 5d68 2a5d 682b 5d68  rO...(h)]h*]h+]h
+00009da0: 2c5d 682f 5d75 6831 4b65 6833 5d72 5006  ,]h/]uh1Keh3]rP.
+00009db0: 0000 2868 4a29 8172 5106 0000 7d72 5206  ..(hJ).rQ...}rR.
+00009dc0: 0000 2868 1e58 0b00 0000 6060 6674 6f6c  ..(h.X....``ftol
+00009dd0: 203e 3d60 6068 277d 7253 0600 0028 6829   >=``h'}rS...(h)
+00009de0: 5d68 2a5d 682b 5d68 2c5d 682f 5d75 681f  ]h*]h+]h,]h/]uh.
+00009df0: 6a4d 0600 0068 335d 7254 0600 0068 5258  jM...h3]rT...hRX
+00009e00: 0700 0000 6674 6f6c 203e 3d72 5506 0000  ....ftol >=rU...
+00009e10: 8581 7256 0600 007d 7257 0600 0028 681e  ..rV...}rW...(h.
+00009e20: 5500 681f 6a51 0600 0075 6261 6825 6856  U.h.jQ...ubah%hV
+00009e30: 7562 6852 5814 0000 0020 7265 6c61 7469  ubhRX.... relati
+00009e40: 7665 2063 6861 6e67 6520 696e 2072 5806  ve change in rX.
+00009e50: 0000 8581 7259 0600 007d 725a 0600 0028  ....rY...}rZ...(
+00009e60: 681e 5814 0000 0020 7265 6c61 7469 7665  h.X.... relative
+00009e70: 2063 6861 6e67 6520 696e 2068 1f6a 4d06   change in h.jM.
+00009e80: 0000 7562 684a 2981 725b 0600 007d 725c  ..ubhJ).r[...}r\
+00009e90: 0600 0028 681e 580a 0000 0060 6063 6869  ...(h.X....``chi
+00009ea0: 2a2a 3260 6068 277d 725d 0600 0028 6829  **2``h'}r]...(h)
+00009eb0: 5d68 2a5d 682b 5d68 2c5d 682f 5d75 681f  ]h*]h+]h,]h/]uh.
+00009ec0: 6a4d 0600 0068 335d 725e 0600 0068 5258  jM...h3]r^...hRX
+00009ed0: 0600 0000 6368 692a 2a32 725f 0600 0085  ....chi**2r_....
+00009ee0: 8172 6006 0000 7d72 6106 0000 2868 1e55  .r`...}ra...(h.U
+00009ef0: 0068 1f6a 5b06 0000 7562 6168 2568 5675  .h.j[...ubah%hVu
+00009f00: 6268 5258 1300 0000 2062 6574 7765 656e  bhRX.... between
+00009f10: 2069 7465 7261 7469 6f6e 7372 6206 0000   iterationsrb...
+00009f20: 8581 7263 0600 007d 7264 0600 0028 681e  ..rc...}rd...(h.
+00009f30: 5813 0000 0020 6265 7477 6565 6e20 6974  X.... between it
+00009f40: 6572 6174 696f 6e73 681f 6a4d 0600 0075  erationsh.jM...u
+00009f50: 6265 7562 6168 256a 0002 0000 7562 6568  beubah%j....ubeh
+00009f60: 2555 0f65 6e75 6d65 7261 7465 645f 6c69  %U.enumerated_li
+00009f70: 7374 7265 0600 0075 6261 7562 6575 6265  stre...ubaubeube
+00009f80: 7562 68cf 2981 7266 0600 007d 7267 0600  ubh.).rf...}rg..
+00009f90: 0028 681e 5500 681f 6a51 0100 0068 236a  .(h.U.h.jQ...h#j
+00009fa0: 5901 0000 6825 68d2 6827 7d72 6806 0000  Y...h%h.h'}rh...
+00009fb0: 2868 2c5d 682b 5d68 295d 682a 5d68 2f5d  (h,]h+]h)]h*]h/]
+00009fc0: 5507 656e 7472 6965 735d 7269 0600 0028  U.entries]ri...(
+00009fd0: 68d5 582c 0000 0065 7272 6f72 2028 6c73  h.X,...error (ls
+00009fe0: 7166 6974 2e73 6369 7079 5f6c 6561 7374  qfit.scipy_least
+00009ff0: 5f73 7175 6172 6573 2061 7474 7269 6275  _squares attribu
+0000a000: 7465 2968 1355 004e 7472 6a06 0000 6175  te)h.U.Ntrj...au
+0000a010: 6831 4e68 3268 0268 335d 7562 68d7 2981  h1Nh2h.h3]ubh.).
+0000a020: 726b 0600 007d 726c 0600 0028 681e 5500  rk...}rl...(h.U.
+0000a030: 681f 6a51 0100 0068 236a 5901 0000 6825  h.jQ...h#jY...h%
+0000a040: 68da 6827 7d72 6d06 0000 2868 dc89 68dd  h.h'}rm...(h..h.
+0000a050: 5802 0000 0070 7968 2c5d 682b 5d68 295d  X....pyh,]h+]h)]
+0000a060: 682a 5d68 2f5d 68df 5809 0000 0061 7474  h*]h/]h.X....att
+0000a070: 7269 6275 7465 726e 0600 0068 e16a 6e06  ributern...h.jn.
+0000a080: 0000 7568 314e 6832 6802 6833 5d72 6f06  ..uh1Nh2h.h3]ro.
+0000a090: 0000 2868 e329 8172 7006 0000 7d72 7106  ..(h.).rp...}rq.
+0000a0a0: 0000 2868 1e58 0500 0000 6572 726f 7272  ..(h.X....errorr
+0000a0b0: 7206 0000 681f 6a6b 0600 0068 236a 5901  r...h.jk...h#jY.
+0000a0c0: 0000 6825 68e7 6827 7d72 7306 0000 2868  ..h%h.h'}rs...(h
+0000a0d0: 2c5d 7274 0600 0068 1361 68ea 68ed 682b  ,]rt...h.ah.h.h+
+0000a0e0: 5d68 295d 682a 5d68 2f5d 7275 0600 0068  ]h)]h*]h/]ru...h
+0000a0f0: 1361 68f0 5819 0000 0073 6369 7079 5f6c  .ah.X....scipy_l
+0000a100: 6561 7374 5f73 7175 6172 6573 2e65 7272  east_squares.err
+0000a110: 6f72 68f2 68f1 68f3 8975 6831 4b6b 6832  orh.h.h..uh1Kkh2
+0000a120: 6802 6833 5d72 7606 0000 6a09 0100 0029  h.h3]rv...j....)
+0000a130: 8172 7706 0000 7d72 7806 0000 2868 1e6a  .rw...}rx...(h.j
+0000a140: 7206 0000 681f 6a70 0600 0068 236a 5901  r...h.jp...h#jY.
+0000a150: 0000 6825 6a0c 0100 0068 277d 7279 0600  ..h%j....h'}ry..
+0000a160: 0028 68fa 68fb 682c 5d68 2b5d 6829 5d68  .(h.h.h,]h+]h)]h
+0000a170: 2a5d 682f 5d75 6831 4b6b 6832 6802 6833  *]h/]uh1Kkh2h.h3
+0000a180: 5d72 7a06 0000 6852 5805 0000 0065 7272  ]rz...hRX....err
+0000a190: 6f72 727b 0600 0085 8172 7c06 0000 7d72  orr{.....r|...}r
+0000a1a0: 7d06 0000 2868 1e55 0068 234e 6831 4e68  }...(h.U.h#Nh1Nh
+0000a1b0: 3268 0268 1f6a 7706 0000 7562 6175 6261  2h.h.jw...ubauba
+0000a1c0: 7562 6a50 0100 0029 8172 7e06 0000 7d72  ubjP...).r~...}r
+0000a1d0: 7f06 0000 2868 1e55 0068 1f6a 6b06 0000  ....(h.U.h.jk...
+0000a1e0: 6823 6a59 0100 0068 256a 5301 0000 6827  h#jY...h%jS...h'
+0000a1f0: 7d72 8006 0000 2868 295d 682a 5d68 2b5d  }r....(h)]h*]h+]
+0000a200: 682c 5d68 2f5d 7568 314b 6b68 3268 0268  h,]h/]uh1Kkh2h.h
+0000a210: 335d 7281 0600 0068 9729 8172 8206 0000  3]r....h.).r....
+0000a220: 7d72 8306 0000 2868 1e58 4800 0000 2a73  }r....(h.XH...*s
+0000a230: 7472 206f 7220 4e6f 6e65 2a20 2d2d 2060  tr or None* -- `
+0000a240: 604e 6f6e 6560 6020 6966 2066 6974 2073  `None`` if fit s
+0000a250: 7563 6365 7373 6675 6c3b 2061 6e20 6572  uccessful; an er
+0000a260: 726f 720a 6d65 7373 6167 6520 6f74 6865  ror.message othe
+0000a270: 7277 6973 652e 681f 6a7e 0600 0068 236a  rwise.h.j~...h#j
+0000a280: 5901 0000 6825 689a 6827 7d72 8406 0000  Y...h%h.h'}r....
+0000a290: 2868 295d 682a 5d68 2b5d 682c 5d68 2f5d  (h)]h*]h+]h,]h/]
+0000a2a0: 7568 314b 6968 3268 0268 335d 7285 0600  uh1Kih2h.h3]r...
+0000a2b0: 0028 6aeb 0400 0029 8172 8606 0000 7d72  .(j....).r....}r
+0000a2c0: 8706 0000 2868 1e58 0d00 0000 2a73 7472  ....(h.X....*str
+0000a2d0: 206f 7220 4e6f 6e65 2a68 277d 7288 0600   or None*h'}r...
+0000a2e0: 0028 6829 5d68 2a5d 682b 5d68 2c5d 682f  .(h)]h*]h+]h,]h/
+0000a2f0: 5d75 681f 6a82 0600 0068 335d 7289 0600  ]uh.j....h3]r...
+0000a300: 0068 5258 0b00 0000 7374 7220 6f72 204e  .hRX....str or N
+0000a310: 6f6e 6572 8a06 0000 8581 728b 0600 007d  oner......r....}
+0000a320: 728c 0600 0028 681e 5500 681f 6a86 0600  r....(h.U.h.j...
+0000a330: 0075 6261 6825 6af3 0400 0075 6268 5258  .ubah%j....ubhRX
+0000a340: 0500 0000 20e2 8093 2072 8d06 0000 8581  .... ... r......
+0000a350: 728e 0600 007d 728f 0600 0028 681e 5804  r....}r....(h.X.
+0000a360: 0000 0020 2d2d 2068 234e 6831 4e68 3268  ... -- h#Nh1Nh2h
+0000a370: 0268 1f6a 8206 0000 7562 684a 2981 7290  .h.j....ubhJ).r.
+0000a380: 0600 007d 7291 0600 0028 681e 5808 0000  ...}r....(h.X...
+0000a390: 0060 604e 6f6e 6560 6068 277d 7292 0600  .``None``h'}r...
+0000a3a0: 0028 6829 5d68 2a5d 682b 5d68 2c5d 682f  .(h)]h*]h+]h,]h/
+0000a3b0: 5d75 681f 6a82 0600 0068 335d 7293 0600  ]uh.j....h3]r...
+0000a3c0: 0068 5258 0400 0000 4e6f 6e65 7294 0600  .hRX....Noner...
+0000a3d0: 0085 8172 9506 0000 7d72 9606 0000 2868  ...r....}r....(h
+0000a3e0: 1e55 0068 1f6a 9006 0000 7562 6168 2568  .U.h.j....ubah%h
+0000a3f0: 5675 6268 5258 2f00 0000 2069 6620 6669  VubhRX/... if fi
+0000a400: 7420 7375 6363 6573 7366 756c 3b20 616e  t successful; an
+0000a410: 2065 7272 6f72 0a6d 6573 7361 6765 206f   error.message o
+0000a420: 7468 6572 7769 7365 2e72 9706 0000 8581  therwise.r......
+0000a430: 7298 0600 007d 7299 0600 0028 681e 582f  r....}r....(h.X/
+0000a440: 0000 0020 6966 2066 6974 2073 7563 6365  ... if fit succe
+0000a450: 7373 6675 6c3b 2061 6e20 6572 726f 720a  ssful; an error.
+0000a460: 6d65 7373 6167 6520 6f74 6865 7277 6973  message otherwis
+0000a470: 652e 6823 4e68 314e 6832 6802 681f 6a82  e.h#Nh1Nh2h.h.j.
+0000a480: 0600 0075 6265 7562 6175 6265 7562 68cf  ...ubeubaubeubh.
+0000a490: 2981 729a 0600 007d 729b 0600 0028 681e  ).r....}r....(h.
+0000a4a0: 5500 681f 6a51 0100 0068 236a 5901 0000  U.h.jQ...h#jY...
+0000a4b0: 6825 68d2 6827 7d72 9c06 0000 2868 2c5d  h%h.h'}r....(h,]
+0000a4c0: 682b 5d68 295d 682a 5d68 2f5d 5507 656e  h+]h)]h*]h/]U.en
+0000a4d0: 7472 6965 735d 729d 0600 0028 68d5 582e  tries]r....(h.X.
+0000a4e0: 0000 0072 6573 756c 7473 2028 6c73 7166  ...results (lsqf
+0000a4f0: 6974 2e73 6369 7079 5f6c 6561 7374 5f73  it.scipy_least_s
+0000a500: 7175 6172 6573 2061 7474 7269 6275 7465  quares attribute
+0000a510: 2968 1055 004e 7472 9e06 0000 6175 6831  )h.U.Ntr....auh1
+0000a520: 4e68 3268 0268 335d 7562 68d7 2981 729f  Nh2h.h3]ubh.).r.
+0000a530: 0600 007d 72a0 0600 0028 681e 5500 681f  ...}r....(h.U.h.
+0000a540: 6a51 0100 0068 236a 5901 0000 6825 68da  jQ...h#jY...h%h.
+0000a550: 6827 7d72 a106 0000 2868 dc89 68dd 5802  h'}r....(h..h.X.
+0000a560: 0000 0070 7968 2c5d 682b 5d68 295d 682a  ...pyh,]h+]h)]h*
+0000a570: 5d68 2f5d 68df 5809 0000 0061 7474 7269  ]h/]h.X....attri
+0000a580: 6275 7465 72a2 0600 0068 e16a a206 0000  buter....h.j....
+0000a590: 7568 314e 6832 6802 6833 5d72 a306 0000  uh1Nh2h.h3]r....
+0000a5a0: 2868 e329 8172 a406 0000 7d72 a506 0000  (h.).r....}r....
+0000a5b0: 2868 1e58 0700 0000 7265 7375 6c74 7372  (h.X....resultsr
+0000a5c0: a606 0000 681f 6a9f 0600 0068 236a 5901  ....h.j....h#jY.
+0000a5d0: 0000 6825 68e7 6827 7d72 a706 0000 2868  ..h%h.h'}r....(h
+0000a5e0: 2c5d 72a8 0600 0068 1061 68ea 68ed 682b  ,]r....h.ah.h.h+
+0000a5f0: 5d68 295d 682a 5d68 2f5d 72a9 0600 0068  ]h)]h*]h/]r....h
+0000a600: 1061 68f0 581b 0000 0073 6369 7079 5f6c  .ah.X....scipy_l
+0000a610: 6561 7374 5f73 7175 6172 6573 2e72 6573  east_squares.res
+0000a620: 756c 7473 68f2 68f1 68f3 8975 6831 4b6e  ultsh.h.h..uh1Kn
+0000a630: 6832 6802 6833 5d72 aa06 0000 6a09 0100  h2h.h3]r....j...
+0000a640: 0029 8172 ab06 0000 7d72 ac06 0000 2868  .).r....}r....(h
+0000a650: 1e6a a606 0000 681f 6aa4 0600 0068 236a  .j....h.j....h#j
+0000a660: 5901 0000 6825 6a0c 0100 0068 277d 72ad  Y...h%j....h'}r.
+0000a670: 0600 0028 68fa 68fb 682c 5d68 2b5d 6829  ...(h.h.h,]h+]h)
+0000a680: 5d68 2a5d 682f 5d75 6831 4b6e 6832 6802  ]h*]h/]uh1Knh2h.
+0000a690: 6833 5d72 ae06 0000 6852 5807 0000 0072  h3]r....hRX....r
+0000a6a0: 6573 756c 7473 72af 0600 0085 8172 b006  esultsr......r..
+0000a6b0: 0000 7d72 b106 0000 2868 1e55 0068 234e  ..}r....(h.U.h#N
+0000a6c0: 6831 4e68 3268 0268 1f6a ab06 0000 7562  h1Nh2h.h.j....ub
+0000a6d0: 6175 6261 7562 6a50 0100 0029 8172 b206  aubaubjP...).r..
+0000a6e0: 0000 7d72 b306 0000 2868 1e55 0068 1f6a  ..}r....(h.U.h.j
+0000a6f0: 9f06 0000 6823 6a59 0100 0068 256a 5301  ....h#jY...h%jS.
+0000a700: 0000 6827 7d72 b406 0000 2868 295d 682a  ..h'}r....(h)]h*
+0000a710: 5d68 2b5d 682c 5d68 2f5d 7568 314b 6e68  ]h+]h,]h/]uh1Knh
+0000a720: 3268 0268 335d 72b5 0600 0068 9729 8172  2h.h3]r....h.).r
+0000a730: b606 0000 7d72 b706 0000 2868 1e58 3f00  ....}r....(h.X?.
+0000a740: 0000 2a64 6963 742a 202d 2d20 5265 7375  ..*dict* -- Resu
+0000a750: 6c74 7320 7265 7475 726e 6564 2062 7920  lts returned by 
+0000a760: 6060 7363 6970 792e 6f70 7469 6d69 7a65  ``scipy.optimize
+0000a770: 2e6c 6561 7374 5f73 7175 6172 6573 6060  .least_squares``
+0000a780: 2e68 1f6a b206 0000 6823 6a59 0100 0068  .h.j....h#jY...h
+0000a790: 2568 9a68 277d 72b8 0600 0028 6829 5d68  %h.h'}r....(h)]h
+0000a7a0: 2a5d 682b 5d68 2c5d 682f 5d75 6831 4b6e  *]h+]h,]h/]uh1Kn
+0000a7b0: 6832 6802 6833 5d72 b906 0000 286a eb04  h2h.h3]r....(j..
+0000a7c0: 0000 2981 72ba 0600 007d 72bb 0600 0028  ..).r....}r....(
+0000a7d0: 681e 5806 0000 002a 6469 6374 2a68 277d  h.X....*dict*h'}
+0000a7e0: 72bc 0600 0028 6829 5d68 2a5d 682b 5d68  r....(h)]h*]h+]h
+0000a7f0: 2c5d 682f 5d75 681f 6ab6 0600 0068 335d  ,]h/]uh.j....h3]
+0000a800: 72bd 0600 0068 5258 0400 0000 6469 6374  r....hRX....dict
+0000a810: 72be 0600 0085 8172 bf06 0000 7d72 c006  r......r....}r..
+0000a820: 0000 2868 1e55 0068 1f6a ba06 0000 7562  ..(h.U.h.j....ub
+0000a830: 6168 256a f304 0000 7562 6852 5819 0000  ah%j....ubhRX...
+0000a840: 0020 e280 9320 5265 7375 6c74 7320 7265  . ... Results re
+0000a850: 7475 726e 6564 2062 7920 72c1 0600 0085  turned by r.....
+0000a860: 8172 c206 0000 7d72 c306 0000 2868 1e58  .r....}r....(h.X
+0000a870: 1800 0000 202d 2d20 5265 7375 6c74 7320  .... -- Results 
+0000a880: 7265 7475 726e 6564 2062 7920 6823 4e68  returned by h#Nh
+0000a890: 314e 6832 6802 681f 6ab6 0600 0075 6268  1Nh2h.h.j....ubh
+0000a8a0: 4a29 8172 c406 0000 7d72 c506 0000 2868  J).r....}r....(h
+0000a8b0: 1e58 2000 0000 6060 7363 6970 792e 6f70  .X ...``scipy.op
+0000a8c0: 7469 6d69 7a65 2e6c 6561 7374 5f73 7175  timize.least_squ
+0000a8d0: 6172 6573 6060 6827 7d72 c606 0000 2868  ares``h'}r....(h
+0000a8e0: 295d 682a 5d68 2b5d 682c 5d68 2f5d 7568  )]h*]h+]h,]h/]uh
+0000a8f0: 1f6a b606 0000 6833 5d72 c706 0000 6852  .j....h3]r....hR
+0000a900: 581c 0000 0073 6369 7079 2e6f 7074 696d  X....scipy.optim
+0000a910: 697a 652e 6c65 6173 745f 7371 7561 7265  ize.least_square
+0000a920: 7372 c806 0000 8581 72c9 0600 007d 72ca  sr......r....}r.
+0000a930: 0600 0028 681e 5500 681f 6ac4 0600 0075  ...(h.U.h.j....u
+0000a940: 6261 6825 6856 7562 6852 5801 0000 002e  bah%hVubhRX.....
+0000a950: 8581 72cb 0600 007d 72cc 0600 0028 681e  ..r....}r....(h.
+0000a960: 5801 0000 002e 6823 4e68 314e 6832 6802  X.....h#Nh1Nh2h.
+0000a970: 681f 6ab6 0600 0075 6265 7562 6175 6265  h.j....ubeubaube
+0000a980: 7562 6575 6265 7562 6575 6268 2029 8172  ubeubeubeubh ).r
+0000a990: cd06 0000 7d72 ce06 0000 2868 1e55 0068  ....}r....(h.U.h
+0000a9a0: 1f68 2168 2368 2468 2568 2668 277d 72cf  .h!h#h$h%h&h'}r.
+0000a9b0: 0600 0028 6829 5d68 2a5d 682b 5d68 2c5d  ...(h)]h*]h+]h,]
+0000a9c0: 72d0 0600 0055 096d 696e 696d 697a 6572  r....U.minimizer
+0000a9d0: 72d1 0600 0061 682f 5d72 d206 0000 6814  r....ah/]r....h.
+0000a9e0: 6175 6831 4b13 6832 6802 6833 5d72 d306  auh1K.h2h.h3]r..
+0000a9f0: 0000 2868 3529 8172 d406 0000 7d72 d506  ..(h5).r....}r..
+0000aa00: 0000 2868 1e58 0900 0000 4d69 6e69 6d69  ..(h.X....Minimi
+0000aa10: 7a65 7272 d606 0000 681f 6acd 0600 0068  zerr....h.j....h
+0000aa20: 2368 2468 2568 3968 277d 72d7 0600 0028  #h$h%h9h'}r....(
+0000aa30: 6829 5d68 2a5d 682b 5d68 2c5d 682f 5d75  h)]h*]h+]h,]h/]u
+0000aa40: 6831 4b13 6832 6802 6833 5d72 d806 0000  h1K.h2h.h3]r....
+0000aa50: 6852 5809 0000 004d 696e 696d 697a 6572  hRX....Minimizer
+0000aa60: 72d9 0600 0085 8172 da06 0000 7d72 db06  r......r....}r..
+0000aa70: 0000 2868 1e6a d606 0000 6823 4e68 314e  ..(h.j....h#Nh1N
+0000aa80: 6832 6802 681f 6ad4 0600 0075 6261 7562  h2h.h.j....ubaub
+0000aa90: 6897 2981 72dc 0600 007d 72dd 0600 0028  h.).r....}r....(
+0000aaa0: 681e 5865 0000 0054 6865 203a 6675 6e63  h.Xe...The :func
+0000aab0: 3a60 6c73 7166 6974 2e65 6d70 6261 7965  :`lsqfit.empbaye
+0000aac0: 735f 6669 7460 2075 7365 7320 6120 6d69  s_fit` uses a mi
+0000aad0: 6e69 6d69 7a65 7220 6672 6f6d 2074 6865  nimizer from the
+0000aae0: 203a 6d6f 643a 6073 6369 7079 600a 6d6f   :mod:`scipy`.mo
+0000aaf0: 6475 6c65 2074 6f20 6d69 6e69 6d69 7a65  dule to minimize
+0000ab00: 2060 606c 6f67 4742 4660 602e 681f 6acd   ``logGBF``.h.j.
+0000ab10: 0600 0068 2368 2468 2568 9a68 277d 72de  ...h#h$h%h.h'}r.
+0000ab20: 0600 0028 6829 5d68 2a5d 682b 5d68 2c5d  ...(h)]h*]h+]h,]
+0000ab30: 682f 5d75 6831 4b14 6832 6802 6833 5d72  h/]uh1K.h2h.h3]r
+0000ab40: df06 0000 2868 5258 0400 0000 5468 6520  ....(hRX....The 
+0000ab50: 72e0 0600 0085 8172 e106 0000 7d72 e206  r......r....}r..
+0000ab60: 0000 2868 1e58 0400 0000 5468 6520 6823  ..(h.X....The h#
+0000ab70: 4e68 314e 6832 6802 681f 6adc 0600 0075  Nh1Nh2h.h.j....u
+0000ab80: 6268 3c29 8172 e306 0000 7d72 e406 0000  bh<).r....}r....
+0000ab90: 2868 1e58 1b00 0000 3a66 756e 633a 606c  (h.X....:func:`l
+0000aba0: 7371 6669 742e 656d 7062 6179 6573 5f66  sqfit.empbayes_f
+0000abb0: 6974 6072 e506 0000 681f 6adc 0600 0068  it`r....h.j....h
+0000abc0: 2368 2468 2568 4068 277d 72e6 0600 0028  #h$h%h@h'}r....(
+0000abd0: 5507 7265 6674 7970 6558 0400 0000 6675  U.reftypeX....fu
+0000abe0: 6e63 6842 8968 4358 1300 0000 6c73 7166  nchB.hCX....lsqf
+0000abf0: 6974 2e65 6d70 6261 7965 735f 6669 7455  it.empbayes_fitU
+0000ac00: 0972 6566 646f 6d61 696e 5802 0000 0070  .refdomainX....p
+0000ac10: 7972 e706 0000 682c 5d68 2b5d 550b 7265  yr....h,]h+]U.re
+0000ac20: 6665 7870 6c69 6369 7489 6829 5d68 2a5d  fexplicit.h)]h*]
+0000ac30: 682f 5d68 4568 4668 474e 6848 4e75 6831  h/]hEhFhGNhHNuh1
+0000ac40: 4b14 6833 5d72 e806 0000 684a 2981 72e9  K.h3]r....hJ).r.
+0000ac50: 0600 007d 72ea 0600 0028 681e 6ae5 0600  ...}r....(h.j...
+0000ac60: 0068 277d 72eb 0600 0028 6829 5d68 2a5d  .h'}r....(h)]h*]
+0000ac70: 72ec 0600 0028 684f 6ae7 0600 0058 0700  r....(hOj....X..
+0000ac80: 0000 7079 2d66 756e 6372 ed06 0000 6568  ..py-funcr....eh
+0000ac90: 2b5d 682c 5d68 2f5d 7568 1f6a e306 0000  +]h,]h/]uh.j....
+0000aca0: 6833 5d72 ee06 0000 6852 5815 0000 006c  h3]r....hRX....l
+0000acb0: 7371 6669 742e 656d 7062 6179 6573 5f66  sqfit.empbayes_f
+0000acc0: 6974 2829 72ef 0600 0085 8172 f006 0000  it()r......r....
+0000acd0: 7d72 f106 0000 2868 1e55 0068 1f6a e906  }r....(h.U.h.j..
+0000ace0: 0000 7562 6168 2568 5675 6261 7562 6852  ..ubah%hVubaubhR
+0000acf0: 581b 0000 0020 7573 6573 2061 206d 696e  X.... uses a min
+0000ad00: 696d 697a 6572 2066 726f 6d20 7468 6520  imizer from the 
+0000ad10: 72f2 0600 0085 8172 f306 0000 7d72 f406  r......r....}r..
+0000ad20: 0000 2868 1e58 1b00 0000 2075 7365 7320  ..(h.X.... uses 
+0000ad30: 6120 6d69 6e69 6d69 7a65 7220 6672 6f6d  a minimizer from
+0000ad40: 2074 6865 2068 234e 6831 4e68 3268 0268   the h#Nh1Nh2h.h
+0000ad50: 1f6a dc06 0000 7562 683c 2981 72f5 0600  .j....ubh<).r...
+0000ad60: 007d 72f6 0600 0028 681e 580c 0000 003a  .}r....(h.X....:
+0000ad70: 6d6f 643a 6073 6369 7079 6072 f706 0000  mod:`scipy`r....
+0000ad80: 681f 6adc 0600 0068 2368 2468 2568 4068  h.j....h#h$h%h@h
+0000ad90: 277d 72f8 0600 0028 5507 7265 6674 7970  '}r....(U.reftyp
+0000ada0: 6558 0300 0000 6d6f 6468 4289 6843 5805  eX....modhB.hCX.
+0000adb0: 0000 0073 6369 7079 5509 7265 6664 6f6d  ...scipyU.refdom
+0000adc0: 6169 6e58 0200 0000 7079 72f9 0600 0068  ainX....pyr....h
+0000add0: 2c5d 682b 5d55 0b72 6566 6578 706c 6963  ,]h+]U.refexplic
+0000ade0: 6974 8968 295d 682a 5d68 2f5d 6845 6846  it.h)]h*]h/]hEhF
+0000adf0: 6847 4e68 484e 7568 314b 1468 335d 72fa  hGNhHNuh1K.h3]r.
+0000ae00: 0600 0068 4a29 8172 fb06 0000 7d72 fc06  ...hJ).r....}r..
+0000ae10: 0000 2868 1e6a f706 0000 6827 7d72 fd06  ..(h.j....h'}r..
+0000ae20: 0000 2868 295d 682a 5d72 fe06 0000 2868  ..(h)]h*]r....(h
+0000ae30: 4f6a f906 0000 5806 0000 0070 792d 6d6f  Oj....X....py-mo
+0000ae40: 6472 ff06 0000 6568 2b5d 682c 5d68 2f5d  dr....eh+]h,]h/]
+0000ae50: 7568 1f6a f506 0000 6833 5d72 0007 0000  uh.j....h3]r....
+0000ae60: 6852 5805 0000 0073 6369 7079 7201 0700  hRX....scipyr...
+0000ae70: 0085 8172 0207 0000 7d72 0307 0000 2868  ...r....}r....(h
+0000ae80: 1e55 0068 1f6a fb06 0000 7562 6168 2568  .U.h.j....ubah%h
+0000ae90: 5675 6261 7562 6852 5814 0000 000a 6d6f  VubaubhRX.....mo
+0000aea0: 6475 6c65 2074 6f20 6d69 6e69 6d69 7a65  dule to minimize
+0000aeb0: 2072 0407 0000 8581 7205 0700 007d 7206   r......r....}r.
+0000aec0: 0700 0028 681e 5814 0000 000a 6d6f 6475  ...(h.X.....modu
+0000aed0: 6c65 2074 6f20 6d69 6e69 6d69 7a65 2068  le to minimize h
+0000aee0: 234e 6831 4e68 3268 0268 1f6a dc06 0000  #Nh1Nh2h.h.j....
+0000aef0: 7562 684a 2981 7207 0700 007d 7208 0700  ubhJ).r....}r...
+0000af00: 0028 681e 580a 0000 0060 606c 6f67 4742  .(h.X....``logGB
+0000af10: 4660 6068 277d 7209 0700 0028 6829 5d68  F``h'}r....(h)]h
+0000af20: 2a5d 682b 5d68 2c5d 682f 5d75 681f 6adc  *]h+]h,]h/]uh.j.
+0000af30: 0600 0068 335d 720a 0700 0068 5258 0600  ...h3]r....hRX..
+0000af40: 0000 6c6f 6747 4246 720b 0700 0085 8172  ..logGBFr......r
+0000af50: 0c07 0000 7d72 0d07 0000 2868 1e55 0068  ....}r....(h.U.h
+0000af60: 1f6a 0707 0000 7562 6168 2568 5675 6268  .j....ubah%hVubh
+0000af70: 5258 0100 0000 2e85 8172 0e07 0000 7d72  RX.......r....}r
+0000af80: 0f07 0000 2868 1e58 0100 0000 2e68 234e  ....(h.X.....h#N
+0000af90: 6831 4e68 3268 0268 1f6a dc06 0000 7562  h1Nh2h.h.j....ub
+0000afa0: 6575 6268 cf29 8172 1007 0000 7d72 1107  eubh.).r....}r..
+0000afb0: 0000 2868 1e55 0068 1f6a cd06 0000 6823  ..(h.U.h.j....h#
+0000afc0: 4e68 2568 d268 277d 7212 0700 0028 682c  Nh%h.h'}r....(h,
+0000afd0: 5d68 2b5d 6829 5d68 2a5d 682f 5d55 0765  ]h+]h)]h*]h/]U.e
+0000afe0: 6e74 7269 6573 5d72 1307 0000 2868 d558  ntries]r....(h.X
+0000aff0: 2200 0000 7363 6970 795f 6d75 6c74 696d  "...scipy_multim
+0000b000: 696e 6578 2028 636c 6173 7320 696e 206c  inex (class in l
+0000b010: 7371 6669 7429 6807 5500 4e74 7214 0700  sqfit)h.U.Ntr...
+0000b020: 0061 7568 314e 6832 6802 6833 5d75 6268  .auh1Nh2h.h3]ubh
+0000b030: d729 8172 1507 0000 7d72 1607 0000 2868  .).r....}r....(h
+0000b040: 1e55 0068 1f6a cd06 0000 6823 4e68 2568  .U.h.j....h#Nh%h
+0000b050: da68 277d 7217 0700 0028 68dc 8968 dd58  .h'}r....(h..h.X
+0000b060: 0200 0000 7079 7218 0700 0068 2c5d 682b  ....pyr....h,]h+
+0000b070: 5d68 295d 682a 5d68 2f5d 68df 5805 0000  ]h)]h*]h/]h.X...
+0000b080: 0063 6c61 7373 7219 0700 0068 e16a 1907  .classr....h.j..
+0000b090: 0000 7568 314e 6832 6802 6833 5d72 1a07  ..uh1Nh2h.h3]r..
+0000b0a0: 0000 2868 e329 8172 1b07 0000 7d72 1c07  ..(h.).r....}r..
+0000b0b0: 0000 2868 1e58 5600 0000 7363 6970 795f  ..(h.XV...scipy_
+0000b0c0: 6d75 6c74 696d 696e 6578 2878 302c 2066  multiminex(x0, f
+0000b0d0: 2c20 746f 6c3d 3165 2d34 2c20 6d61 7869  , tol=1e-4, maxi
+0000b0e0: 743d 3130 3030 2c20 7374 6570 3d31 2c20  t=1000, step=1, 
+0000b0f0: 616c 673d 276e 6d73 696d 706c 6578 3227  alg='nmsimplex2'
+0000b100: 2c20 616e 616c 797a 6572 3d4e 6f6e 6529  , analyzer=None)
+0000b110: 681f 6a15 0700 0068 2358 6600 0000 2f55  h.j....h#Xf.../U
+0000b120: 7365 7273 2f67 706c 2f61 6e61 636f 6e64  sers/gpl/anacond
+0000b130: 6132 2f6c 6962 2f70 7974 686f 6e32 2e37  a2/lib/python2.7
+0000b140: 2f73 6974 652d 7061 636b 6167 6573 2f6c  /site-packages/l
+0000b150: 7371 6669 742f 5f73 6369 7079 2e70 793a  sqfit/_scipy.py:
+0000b160: 646f 6373 7472 696e 6720 6f66 206c 7371  docstring of lsq
+0000b170: 6669 742e 7363 6970 795f 6d75 6c74 696d  fit.scipy_multim
+0000b180: 696e 6578 721d 0700 0068 2568 e768 277d  inexr....h%h.h'}
+0000b190: 721e 0700 0028 682c 5d72 1f07 0000 6807  r....(h,]r....h.
+0000b1a0: 6168 ea68 eb58 0600 0000 6c73 7166 6974  ah.h.X....lsqfit
+0000b1b0: 7220 0700 0085 8172 2107 0000 7d72 2207  r .....r!...}r".
+0000b1c0: 0000 6268 2b5d 6829 5d68 2a5d 682f 5d72  ..bh+]h)]h*]h/]r
+0000b1d0: 2307 0000 6807 6168 f058 1000 0000 7363  #...h.ah.X....sc
+0000b1e0: 6970 795f 6d75 6c74 696d 696e 6578 7224  ipy_multiminexr$
+0000b1f0: 0700 0068 f255 0068 f389 7568 314e 6832  ...h.U.h..uh1Nh2
+0000b200: 6802 6833 5d72 2507 0000 2868 f529 8172  h.h3]r%...(h.).r
+0000b210: 2607 0000 7d72 2707 0000 2868 1e58 0600  &...}r'...(h.X..
+0000b220: 0000 636c 6173 7320 681f 6a1b 0700 0068  ..class h.j....h
+0000b230: 236a 1d07 0000 6825 68f8 6827 7d72 2807  #j....h%h.h'}r(.
+0000b240: 0000 2868 fa68 fb68 2c5d 682b 5d68 295d  ..(h.h.h,]h+]h)]
+0000b250: 682a 5d68 2f5d 7568 314e 6832 6802 6833  h*]h/]uh1Nh2h.h3
+0000b260: 5d72 2907 0000 6852 5806 0000 0063 6c61  ]r)...hRX....cla
+0000b270: 7373 2072 2a07 0000 8581 722b 0700 007d  ss r*.....r+...}
+0000b280: 722c 0700 0028 681e 5500 6823 4e68 314e  r,...(h.U.h#Nh1N
+0000b290: 6832 6802 681f 6a26 0700 0075 6261 7562  h2h.h.j&...ubaub
+0000b2a0: 6a00 0100 0029 8172 2d07 0000 7d72 2e07  j....).r-...}r..
+0000b2b0: 0000 2868 1e58 0700 0000 6c73 7166 6974  ..(h.X....lsqfit
+0000b2c0: 2e68 1f6a 1b07 0000 6823 6a1d 0700 0068  .h.j....h#j....h
+0000b2d0: 256a 0301 0000 6827 7d72 2f07 0000 2868  %j....h'}r/...(h
+0000b2e0: fa68 fb68 2c5d 682b 5d68 295d 682a 5d68  .h.h,]h+]h)]h*]h
+0000b2f0: 2f5d 7568 314e 6832 6802 6833 5d72 3007  /]uh1Nh2h.h3]r0.
+0000b300: 0000 6852 5807 0000 006c 7371 6669 742e  ..hRX....lsqfit.
+0000b310: 7231 0700 0085 8172 3207 0000 7d72 3307  r1.....r2...}r3.
+0000b320: 0000 2868 1e55 0068 234e 6831 4e68 3268  ..(h.U.h#Nh1Nh2h
+0000b330: 0268 1f6a 2d07 0000 7562 6175 626a 0901  .h.j-...ubaubj..
+0000b340: 0000 2981 7234 0700 007d 7235 0700 0028  ..).r4...}r5...(
+0000b350: 681e 6a24 0700 0068 1f6a 1b07 0000 6823  h.j$...h.j....h#
+0000b360: 6a1d 0700 0068 256a 0c01 0000 6827 7d72  j....h%j....h'}r
+0000b370: 3607 0000 2868 fa68 fb68 2c5d 682b 5d68  6...(h.h.h,]h+]h
+0000b380: 295d 682a 5d68 2f5d 7568 314e 6832 6802  )]h*]h/]uh1Nh2h.
+0000b390: 6833 5d72 3707 0000 6852 5810 0000 0073  h3]r7...hRX....s
+0000b3a0: 6369 7079 5f6d 756c 7469 6d69 6e65 7872  cipy_multiminexr
+0000b3b0: 3807 0000 8581 7239 0700 007d 723a 0700  8.....r9...}r:..
+0000b3c0: 0028 681e 5500 6823 4e68 314e 6832 6802  .(h.U.h#Nh1Nh2h.
+0000b3d0: 681f 6a34 0700 0075 6261 7562 6a12 0100  h.j4...ubaubj...
+0000b3e0: 0029 8172 3b07 0000 7d72 3c07 0000 2868  .).r;...}r<...(h
+0000b3f0: 1e58 4400 0000 7830 2c20 662c 2074 6f6c  .XD...x0, f, tol
+0000b400: 3d31 652d 342c 206d 6178 6974 3d31 3030  =1e-4, maxit=100
+0000b410: 302c 2073 7465 703d 312c 2061 6c67 3d27  0, step=1, alg='
+0000b420: 6e6d 7369 6d70 6c65 7832 272c 2061 6e61  nmsimplex2', ana
+0000b430: 6c79 7a65 723d 4e6f 6e65 681f 6a1b 0700  lyzer=Noneh.j...
+0000b440: 0068 236a 1d07 0000 6825 6a15 0100 0068  .h#j....h%j....h
+0000b450: 277d 723d 0700 0028 68fa 68fb 682c 5d68  '}r=...(h.h.h,]h
+0000b460: 2b5d 6829 5d68 2a5d 682f 5d75 6831 4e68  +]h)]h*]h/]uh1Nh
+0000b470: 3268 0268 335d 723e 0700 0028 6a18 0100  2h.h3]r>...(j...
+0000b480: 0029 8172 3f07 0000 7d72 4007 0000 2868  .).r?...}r@...(h
+0000b490: 1e58 0200 0000 7830 6827 7d72 4107 0000  .X....x0h'}rA...
+0000b4a0: 2868 fa68 fb68 2c5d 682b 5d68 295d 682a  (h.h.h,]h+]h)]h*
+0000b4b0: 5d68 2f5d 7568 1f6a 3b07 0000 6833 5d72  ]h/]uh.j;...h3]r
+0000b4c0: 4207 0000 6852 5802 0000 0078 3072 4307  B...hRX....x0rC.
+0000b4d0: 0000 8581 7244 0700 007d 7245 0700 0028  ....rD...}rE...(
+0000b4e0: 681e 5500 681f 6a3f 0700 0075 6261 6825  h.U.h.j?...ubah%
+0000b4f0: 6a20 0100 0075 626a 1801 0000 2981 7246  j ...ubj....).rF
+0000b500: 0700 007d 7247 0700 0028 681e 5801 0000  ...}rG...(h.X...
+0000b510: 0066 6827 7d72 4807 0000 2868 fa68 fb68  .fh'}rH...(h.h.h
+0000b520: 2c5d 682b 5d68 295d 682a 5d68 2f5d 7568  ,]h+]h)]h*]h/]uh
+0000b530: 1f6a 3b07 0000 6833 5d72 4907 0000 6852  .j;...h3]rI...hR
+0000b540: 5801 0000 0066 8581 724a 0700 007d 724b  X....f..rJ...}rK
+0000b550: 0700 0028 681e 5500 681f 6a46 0700 0075  ...(h.U.h.jF...u
+0000b560: 6261 6825 6a20 0100 0075 626a 1801 0000  bah%j ...ubj....
+0000b570: 2981 724c 0700 007d 724d 0700 0028 681e  ).rL...}rM...(h.
+0000b580: 5808 0000 0074 6f6c 3d31 652d 3468 277d  X....tol=1e-4h'}
+0000b590: 724e 0700 0028 68fa 68fb 682c 5d68 2b5d  rN...(h.h.h,]h+]
+0000b5a0: 6829 5d68 2a5d 682f 5d75 681f 6a3b 0700  h)]h*]h/]uh.j;..
+0000b5b0: 0068 335d 724f 0700 0068 5258 0800 0000  .h3]rO...hRX....
+0000b5c0: 746f 6c3d 3165 2d34 7250 0700 0085 8172  tol=1e-4rP.....r
+0000b5d0: 5107 0000 7d72 5207 0000 2868 1e55 0068  Q...}rR...(h.U.h
+0000b5e0: 1f6a 4c07 0000 7562 6168 256a 2001 0000  .jL...ubah%j ...
+0000b5f0: 7562 6a18 0100 0029 8172 5307 0000 7d72  ubj....).rS...}r
+0000b600: 5407 0000 2868 1e58 0a00 0000 6d61 7869  T...(h.X....maxi
+0000b610: 743d 3130 3030 6827 7d72 5507 0000 2868  t=1000h'}rU...(h
+0000b620: fa68 fb68 2c5d 682b 5d68 295d 682a 5d68  .h.h,]h+]h)]h*]h
+0000b630: 2f5d 7568 1f6a 3b07 0000 6833 5d72 5607  /]uh.j;...h3]rV.
+0000b640: 0000 6852 580a 0000 006d 6178 6974 3d31  ..hRX....maxit=1
+0000b650: 3030 3072 5707 0000 8581 7258 0700 007d  000rW.....rX...}
+0000b660: 7259 0700 0028 681e 5500 681f 6a53 0700  rY...(h.U.h.jS..
+0000b670: 0075 6261 6825 6a20 0100 0075 626a 1801  .ubah%j ...ubj..
+0000b680: 0000 2981 725a 0700 007d 725b 0700 0028  ..).rZ...}r[...(
+0000b690: 681e 5806 0000 0073 7465 703d 3168 277d  h.X....step=1h'}
+0000b6a0: 725c 0700 0028 68fa 68fb 682c 5d68 2b5d  r\...(h.h.h,]h+]
+0000b6b0: 6829 5d68 2a5d 682f 5d75 681f 6a3b 0700  h)]h*]h/]uh.j;..
+0000b6c0: 0068 335d 725d 0700 0068 5258 0600 0000  .h3]r]...hRX....
+0000b6d0: 7374 6570 3d31 725e 0700 0085 8172 5f07  step=1r^.....r_.
+0000b6e0: 0000 7d72 6007 0000 2868 1e55 0068 1f6a  ..}r`...(h.U.h.j
+0000b6f0: 5a07 0000 7562 6168 256a 2001 0000 7562  Z...ubah%j ...ub
+0000b700: 6a18 0100 0029 8172 6107 0000 7d72 6207  j....).ra...}rb.
+0000b710: 0000 2868 1e58 1000 0000 616c 673d 276e  ..(h.X....alg='n
+0000b720: 6d73 696d 706c 6578 3227 6827 7d72 6307  msimplex2'h'}rc.
+0000b730: 0000 2868 fa68 fb68 2c5d 682b 5d68 295d  ..(h.h.h,]h+]h)]
+0000b740: 682a 5d68 2f5d 7568 1f6a 3b07 0000 6833  h*]h/]uh.j;...h3
+0000b750: 5d72 6407 0000 6852 5810 0000 0061 6c67  ]rd...hRX....alg
+0000b760: 3d27 6e6d 7369 6d70 6c65 7832 2772 6507  ='nmsimplex2're.
+0000b770: 0000 8581 7266 0700 007d 7267 0700 0028  ....rf...}rg...(
+0000b780: 681e 5500 681f 6a61 0700 0075 6261 6825  h.U.h.ja...ubah%
+0000b790: 6a20 0100 0075 626a 1801 0000 2981 7268  j ...ubj....).rh
+0000b7a0: 0700 007d 7269 0700 0028 681e 580d 0000  ...}ri...(h.X...
+0000b7b0: 0061 6e61 6c79 7a65 723d 4e6f 6e65 6827  .analyzer=Noneh'
+0000b7c0: 7d72 6a07 0000 2868 fa68 fb68 2c5d 682b  }rj...(h.h.h,]h+
+0000b7d0: 5d68 295d 682a 5d68 2f5d 7568 1f6a 3b07  ]h)]h*]h/]uh.j;.
+0000b7e0: 0000 6833 5d72 6b07 0000 6852 580d 0000  ..h3]rk...hRX...
+0000b7f0: 0061 6e61 6c79 7a65 723d 4e6f 6e65 726c  .analyzer=Nonerl
+0000b800: 0700 0085 8172 6d07 0000 7d72 6e07 0000  .....rm...}rn...
+0000b810: 2868 1e55 0068 1f6a 6807 0000 7562 6168  (h.U.h.jh...ubah
+0000b820: 256a 2001 0000 7562 6575 6265 7562 6a50  %j ...ubeubeubjP
+0000b830: 0100 0029 8172 6f07 0000 7d72 7007 0000  ...).ro...}rp...
+0000b840: 2868 1e55 0068 1f6a 1507 0000 6823 6a1d  (h.U.h.j....h#j.
+0000b850: 0700 0068 256a 5301 0000 6827 7d72 7107  ...h%jS...h'}rq.
+0000b860: 0000 2868 295d 682a 5d68 2b5d 682c 5d68  ..(h)]h*]h+]h,]h
+0000b870: 2f5d 7568 314e 6832 6802 6833 5d72 7207  /]uh1Nh2h.h3]rr.
+0000b880: 0000 2868 9729 8172 7307 0000 7d72 7407  ..(h.).rs...}rt.
+0000b890: 0000 2868 1e58 3600 0000 3a6d 6f64 3a60  ..(h.X6...:mod:`
+0000b8a0: 7363 6970 7960 206d 696e 696d 697a 6572  scipy` minimizer
+0000b8b0: 2066 6f72 206d 756c 7469 6469 6d65 6e73   for multidimens
+0000b8c0: 696f 6e61 6c20 6675 6e63 7469 6f6e 732e  ional functions.
+0000b8d0: 7275 0700 0068 1f6a 6f07 0000 6823 5866  ru...h.jo...h#Xf
+0000b8e0: 0000 002f 5573 6572 732f 6770 6c2f 616e  .../Users/gpl/an
+0000b8f0: 6163 6f6e 6461 322f 6c69 622f 7079 7468  aconda2/lib/pyth
+0000b900: 6f6e 322e 372f 7369 7465 2d70 6163 6b61  on2.7/site-packa
+0000b910: 6765 732f 6c73 7166 6974 2f5f 7363 6970  ges/lsqfit/_scip
+0000b920: 792e 7079 3a64 6f63 7374 7269 6e67 206f  y.py:docstring o
+0000b930: 6620 6c73 7166 6974 2e73 6369 7079 5f6d  f lsqfit.scipy_m
+0000b940: 756c 7469 6d69 6e65 7872 7607 0000 6825  ultiminexrv...h%
+0000b950: 689a 6827 7d72 7707 0000 2868 295d 682a  h.h'}rw...(h)]h*
+0000b960: 5d68 2b5d 682c 5d68 2f5d 7568 314b 0168  ]h+]h,]h/]uh1K.h
+0000b970: 3268 0268 335d 7278 0700 0028 683c 2981  2h.h3]rx...(h<).
+0000b980: 7279 0700 007d 727a 0700 0028 681e 580c  ry...}rz...(h.X.
+0000b990: 0000 003a 6d6f 643a 6073 6369 7079 6072  ...:mod:`scipy`r
+0000b9a0: 7b07 0000 681f 6a73 0700 0068 236a 7607  {...h.js...h#jv.
+0000b9b0: 0000 6825 6840 6827 7d72 7c07 0000 2855  ..h%h@h'}r|...(U
+0000b9c0: 0772 6566 7479 7065 5803 0000 006d 6f64  .reftypeX....mod
+0000b9d0: 6842 8968 4358 0500 0000 7363 6970 7955  hB.hCX....scipyU
+0000b9e0: 0972 6566 646f 6d61 696e 5802 0000 0070  .refdomainX....p
+0000b9f0: 7972 7d07 0000 682c 5d68 2b5d 550b 7265  yr}...h,]h+]U.re
+0000ba00: 6665 7870 6c69 6369 7489 6829 5d68 2a5d  fexplicit.h)]h*]
+0000ba10: 682f 5d68 4568 4668 476a 2407 0000 6848  h/]hEhFhGj$...hH
+0000ba20: 6a21 0700 0075 6831 4b01 6833 5d72 7e07  j!...uh1K.h3]r~.
+0000ba30: 0000 684a 2981 727f 0700 007d 7280 0700  ..hJ).r....}r...
+0000ba40: 0028 681e 6a7b 0700 0068 277d 7281 0700  .(h.j{...h'}r...
+0000ba50: 0028 6829 5d68 2a5d 7282 0700 0028 684f  .(h)]h*]r....(hO
+0000ba60: 6a7d 0700 0058 0600 0000 7079 2d6d 6f64  j}...X....py-mod
+0000ba70: 7283 0700 0065 682b 5d68 2c5d 682f 5d75  r....eh+]h,]h/]u
+0000ba80: 681f 6a79 0700 0068 335d 7284 0700 0068  h.jy...h3]r....h
+0000ba90: 5258 0500 0000 7363 6970 7972 8507 0000  RX....scipyr....
+0000baa0: 8581 7286 0700 007d 7287 0700 0028 681e  ..r....}r....(h.
+0000bab0: 5500 681f 6a7f 0700 0075 6261 6825 6856  U.h.j....ubah%hV
+0000bac0: 7562 6175 6268 5258 2a00 0000 206d 696e  ubaubhRX*... min
+0000bad0: 696d 697a 6572 2066 6f72 206d 756c 7469  imizer for multi
+0000bae0: 6469 6d65 6e73 696f 6e61 6c20 6675 6e63  dimensional func
+0000baf0: 7469 6f6e 732e 7288 0700 0085 8172 8907  tions.r......r..
+0000bb00: 0000 7d72 8a07 0000 2868 1e58 2a00 0000  ..}r....(h.X*...
+0000bb10: 206d 696e 696d 697a 6572 2066 6f72 206d   minimizer for m
+0000bb20: 756c 7469 6469 6d65 6e73 696f 6e61 6c20  ultidimensional 
+0000bb30: 6675 6e63 7469 6f6e 732e 6823 4e68 314e  functions.h#Nh1N
+0000bb40: 6832 6802 681f 6a73 0700 0075 6265 7562  h2h.h.js...ubeub
+0000bb50: 6897 2981 728b 0700 007d 728c 0700 0028  h.).r....}r....(
+0000bb60: 681e 58dd 0000 003a 636c 6173 733a 6073  h.X....:class:`s
+0000bb70: 6369 7079 5f6d 756c 7469 6d69 6e65 7860  cipy_multiminex`
+0000bb80: 2069 7320 6120 6675 6e63 7469 6f6e 2d63   is a function-c
+0000bb90: 6c61 7373 2077 686f 7365 2063 6f6e 7374  lass whose const
+0000bba0: 7275 6374 6f72 206d 696e 696d 697a 6573  ructor minimizes
+0000bbb0: 2061 0a6d 756c 7469 6469 6d65 6e73 696f   a.multidimensio
+0000bbc0: 6e61 6c20 6675 6e63 7469 6f6e 2060 6066  nal function ``f
+0000bbd0: 2878 2960 6020 6279 2076 6172 7969 6e67  (x)`` by varying
+0000bbe0: 2076 6563 746f 7220 6060 7860 602e 2054   vector ``x``. T
+0000bbf0: 6869 7320 726f 7574 696e 650a 646f 6573  his routine.does
+0000bc00: 202a 6e6f 742a 2075 7365 2075 7365 722d   *not* use user-
+0000bc10: 7375 7070 6c69 6564 2069 6e66 6f72 6d61  supplied informa
+0000bc20: 7469 6f6e 2061 626f 7574 2074 6865 2067  tion about the g
+0000bc30: 7261 6469 656e 7420 6f66 2060 6066 2878  radient of ``f(x
+0000bc40: 2960 602e 681f 6a6f 0700 0068 236a 7607  )``.h.jo...h#jv.
+0000bc50: 0000 6825 689a 6827 7d72 8d07 0000 2868  ..h%h.h'}r....(h
+0000bc60: 295d 682a 5d68 2b5d 682c 5d68 2f5d 7568  )]h*]h+]h,]h/]uh
+0000bc70: 314b 0368 3268 0268 335d 728e 0700 0028  1K.h2h.h3]r....(
+0000bc80: 683c 2981 728f 0700 007d 7290 0700 0028  h<).r....}r....(
+0000bc90: 681e 5819 0000 003a 636c 6173 733a 6073  h.X....:class:`s
+0000bca0: 6369 7079 5f6d 756c 7469 6d69 6e65 7860  cipy_multiminex`
+0000bcb0: 7291 0700 0068 1f6a 8b07 0000 6823 6a76  r....h.j....h#jv
+0000bcc0: 0700 0068 2568 4068 277d 7292 0700 0028  ...h%h@h'}r....(
+0000bcd0: 5507 7265 6674 7970 6558 0500 0000 636c  U.reftypeX....cl
+0000bce0: 6173 7368 4289 6843 5810 0000 0073 6369  asshB.hCX....sci
+0000bcf0: 7079 5f6d 756c 7469 6d69 6e65 7855 0972  py_multiminexU.r
+0000bd00: 6566 646f 6d61 696e 5802 0000 0070 7972  efdomainX....pyr
+0000bd10: 9307 0000 682c 5d68 2b5d 550b 7265 6665  ....h,]h+]U.refe
+0000bd20: 7870 6c69 6369 7489 6829 5d68 2a5d 682f  xplicit.h)]h*]h/
+0000bd30: 5d68 4568 4668 476a 2407 0000 6848 6a21  ]hEhFhGj$...hHj!
+0000bd40: 0700 0075 6831 4b03 6833 5d72 9407 0000  ...uh1K.h3]r....
+0000bd50: 684a 2981 7295 0700 007d 7296 0700 0028  hJ).r....}r....(
+0000bd60: 681e 6a91 0700 0068 277d 7297 0700 0028  h.j....h'}r....(
+0000bd70: 6829 5d68 2a5d 7298 0700 0028 684f 6a93  h)]h*]r....(hOj.
+0000bd80: 0700 0058 0800 0000 7079 2d63 6c61 7373  ...X....py-class
+0000bd90: 7299 0700 0065 682b 5d68 2c5d 682f 5d75  r....eh+]h,]h/]u
+0000bda0: 681f 6a8f 0700 0068 335d 729a 0700 0068  h.j....h3]r....h
+0000bdb0: 5258 1000 0000 7363 6970 795f 6d75 6c74  RX....scipy_mult
+0000bdc0: 696d 696e 6578 729b 0700 0085 8172 9c07  iminexr......r..
+0000bdd0: 0000 7d72 9d07 0000 2868 1e55 0068 1f6a  ..}r....(h.U.h.j
+0000bde0: 9507 0000 7562 6168 2568 5675 6261 7562  ....ubah%hVubaub
+0000bdf0: 6852 584d 0000 0020 6973 2061 2066 756e  hRXM... is a fun
+0000be00: 6374 696f 6e2d 636c 6173 7320 7768 6f73  ction-class whos
+0000be10: 6520 636f 6e73 7472 7563 746f 7220 6d69  e constructor mi
+0000be20: 6e69 6d69 7a65 7320 610a 6d75 6c74 6964  nimizes a.multid
+0000be30: 696d 656e 7369 6f6e 616c 2066 756e 6374  imensional funct
+0000be40: 696f 6e20 729e 0700 0085 8172 9f07 0000  ion r......r....
+0000be50: 7d72 a007 0000 2868 1e58 4d00 0000 2069  }r....(h.XM... i
+0000be60: 7320 6120 6675 6e63 7469 6f6e 2d63 6c61  s a function-cla
+0000be70: 7373 2077 686f 7365 2063 6f6e 7374 7275  ss whose constru
+0000be80: 6374 6f72 206d 696e 696d 697a 6573 2061  ctor minimizes a
+0000be90: 0a6d 756c 7469 6469 6d65 6e73 696f 6e61  .multidimensiona
+0000bea0: 6c20 6675 6e63 7469 6f6e 2068 234e 6831  l function h#Nh1
+0000beb0: 4e68 3268 0268 1f6a 8b07 0000 7562 684a  Nh2h.h.j....ubhJ
+0000bec0: 2981 72a1 0700 007d 72a2 0700 0028 681e  ).r....}r....(h.
+0000bed0: 5808 0000 0060 6066 2878 2960 6068 277d  X....``f(x)``h'}
+0000bee0: 72a3 0700 0028 6829 5d68 2a5d 682b 5d68  r....(h)]h*]h+]h
+0000bef0: 2c5d 682f 5d75 681f 6a8b 0700 0068 335d  ,]h/]uh.j....h3]
+0000bf00: 72a4 0700 0068 5258 0400 0000 6628 7829  r....hRX....f(x)
+0000bf10: 72a5 0700 0085 8172 a607 0000 7d72 a707  r......r....}r..
+0000bf20: 0000 2868 1e55 0068 1f6a a107 0000 7562  ..(h.U.h.j....ub
+0000bf30: 6168 2568 5675 6268 5258 1300 0000 2062  ah%hVubhRX.... b
+0000bf40: 7920 7661 7279 696e 6720 7665 6374 6f72  y varying vector
+0000bf50: 2072 a807 0000 8581 72a9 0700 007d 72aa   r......r....}r.
+0000bf60: 0700 0028 681e 5813 0000 0020 6279 2076  ...(h.X.... by v
+0000bf70: 6172 7969 6e67 2076 6563 746f 7220 6823  arying vector h#
+0000bf80: 4e68 314e 6832 6802 681f 6a8b 0700 0075  Nh1Nh2h.h.j....u
+0000bf90: 6268 4a29 8172 ab07 0000 7d72 ac07 0000  bhJ).r....}r....
+0000bfa0: 2868 1e58 0500 0000 6060 7860 6068 277d  (h.X....``x``h'}
+0000bfb0: 72ad 0700 0028 6829 5d68 2a5d 682b 5d68  r....(h)]h*]h+]h
+0000bfc0: 2c5d 682f 5d75 681f 6a8b 0700 0068 335d  ,]h/]uh.j....h3]
+0000bfd0: 72ae 0700 0068 5258 0100 0000 7885 8172  r....hRX....x..r
+0000bfe0: af07 0000 7d72 b007 0000 2868 1e55 0068  ....}r....(h.U.h
+0000bff0: 1f6a ab07 0000 7562 6168 2568 5675 6268  .j....ubah%hVubh
+0000c000: 5258 1400 0000 2e20 5468 6973 2072 6f75  RX..... This rou
+0000c010: 7469 6e65 0a64 6f65 7320 72b1 0700 0085  tine.does r.....
+0000c020: 8172 b207 0000 7d72 b307 0000 2868 1e58  .r....}r....(h.X
+0000c030: 1400 0000 2e20 5468 6973 2072 6f75 7469  ..... This routi
+0000c040: 6e65 0a64 6f65 7320 6823 4e68 314e 6832  ne.does h#Nh1Nh2
+0000c050: 6802 681f 6a8b 0700 0075 626a eb04 0000  h.h.j....ubj....
+0000c060: 2981 72b4 0700 007d 72b5 0700 0028 681e  ).r....}r....(h.
+0000c070: 5805 0000 002a 6e6f 742a 6827 7d72 b607  X....*not*h'}r..
+0000c080: 0000 2868 295d 682a 5d68 2b5d 682c 5d68  ..(h)]h*]h+]h,]h
+0000c090: 2f5d 7568 1f6a 8b07 0000 6833 5d72 b707  /]uh.j....h3]r..
+0000c0a0: 0000 6852 5803 0000 006e 6f74 72b8 0700  ..hRX....notr...
+0000c0b0: 0085 8172 b907 0000 7d72 ba07 0000 2868  ...r....}r....(h
+0000c0c0: 1e55 0068 1f6a b407 0000 7562 6168 256a  .U.h.j....ubah%j
+0000c0d0: f304 0000 7562 6852 5835 0000 0020 7573  ....ubhRX5... us
+0000c0e0: 6520 7573 6572 2d73 7570 706c 6965 6420  e user-supplied 
+0000c0f0: 696e 666f 726d 6174 696f 6e20 6162 6f75  information abou
+0000c100: 7420 7468 6520 6772 6164 6965 6e74 206f  t the gradient o
+0000c110: 6620 72bb 0700 0085 8172 bc07 0000 7d72  f r......r....}r
+0000c120: bd07 0000 2868 1e58 3500 0000 2075 7365  ....(h.X5... use
+0000c130: 2075 7365 722d 7375 7070 6c69 6564 2069   user-supplied i
+0000c140: 6e66 6f72 6d61 7469 6f6e 2061 626f 7574  nformation about
+0000c150: 2074 6865 2067 7261 6469 656e 7420 6f66   the gradient of
+0000c160: 2068 234e 6831 4e68 3268 0268 1f6a 8b07   h#Nh1Nh2h.h.j..
+0000c170: 0000 7562 684a 2981 72be 0700 007d 72bf  ..ubhJ).r....}r.
+0000c180: 0700 0028 681e 5808 0000 0060 6066 2878  ...(h.X....``f(x
+0000c190: 2960 6068 277d 72c0 0700 0028 6829 5d68  )``h'}r....(h)]h
+0000c1a0: 2a5d 682b 5d68 2c5d 682f 5d75 681f 6a8b  *]h+]h,]h/]uh.j.
+0000c1b0: 0700 0068 335d 72c1 0700 0068 5258 0400  ...h3]r....hRX..
+0000c1c0: 0000 6628 7829 72c2 0700 0085 8172 c307  ..f(x)r......r..
+0000c1d0: 0000 7d72 c407 0000 2868 1e55 0068 1f6a  ..}r....(h.U.h.j
+0000c1e0: be07 0000 7562 6168 2568 5675 6268 5258  ....ubah%hVubhRX
+0000c1f0: 0100 0000 2e85 8172 c507 0000 7d72 c607  .......r....}r..
+0000c200: 0000 2868 1e58 0100 0000 2e68 234e 6831  ..(h.X.....h#Nh1
+0000c210: 4e68 3268 0268 1f6a 8b07 0000 7562 6575  Nh2h.h.j....ubeu
+0000c220: 6268 9729 8172 c707 0000 7d72 c807 0000  bh.).r....}r....
+0000c230: 2868 1e58 8100 0000 3a63 6c61 7373 3a60  (h.X....:class:`
+0000c240: 7363 6970 795f 6d75 6c74 696d 696e 6578  scipy_multiminex
+0000c250: 6020 6973 2061 2077 7261 7070 6572 2066  ` is a wrapper f
+0000c260: 6f72 2074 6865 2060 606d 696e 696d 697a  or the ``minimiz
+0000c270: 6560 600a 3a6d 6f64 3a60 7363 6970 7960  e``.:mod:`scipy`
+0000c280: 2066 756e 6374 696f 6e2e 2049 7420 6769   function. It gi
+0000c290: 7665 7320 6163 6365 7373 2074 6f20 6f6e  ves access to on
+0000c2a0: 6c79 2070 6172 7420 6f66 2074 6861 740a  ly part of that.
+0000c2b0: 6675 6e63 7469 6f6e 2e68 1f6a 6f07 0000  function.h.jo...
+0000c2c0: 6823 6a76 0700 0068 2568 9a68 277d 72c9  h#jv...h%h.h'}r.
+0000c2d0: 0700 0028 6829 5d68 2a5d 682b 5d68 2c5d  ...(h)]h*]h+]h,]
+0000c2e0: 682f 5d75 6831 4b07 6832 6802 6833 5d72  h/]uh1K.h2h.h3]r
+0000c2f0: ca07 0000 2868 3c29 8172 cb07 0000 7d72  ....(h<).r....}r
+0000c300: cc07 0000 2868 1e58 1900 0000 3a63 6c61  ....(h.X....:cla
+0000c310: 7373 3a60 7363 6970 795f 6d75 6c74 696d  ss:`scipy_multim
+0000c320: 696e 6578 6072 cd07 0000 681f 6ac7 0700  inex`r....h.j...
+0000c330: 0068 236a 7607 0000 6825 6840 6827 7d72  .h#jv...h%h@h'}r
+0000c340: ce07 0000 2855 0772 6566 7479 7065 5805  ....(U.reftypeX.
+0000c350: 0000 0063 6c61 7373 6842 8968 4358 1000  ...classhB.hCX..
+0000c360: 0000 7363 6970 795f 6d75 6c74 696d 696e  ..scipy_multimin
+0000c370: 6578 5509 7265 6664 6f6d 6169 6e58 0200  exU.refdomainX..
+0000c380: 0000 7079 72cf 0700 0068 2c5d 682b 5d55  ..pyr....h,]h+]U
+0000c390: 0b72 6566 6578 706c 6963 6974 8968 295d  .refexplicit.h)]
+0000c3a0: 682a 5d68 2f5d 6845 6846 6847 6a24 0700  h*]h/]hEhFhGj$..
+0000c3b0: 0068 486a 2107 0000 7568 314b 0768 335d  .hHj!...uh1K.h3]
+0000c3c0: 72d0 0700 0068 4a29 8172 d107 0000 7d72  r....hJ).r....}r
+0000c3d0: d207 0000 2868 1e6a cd07 0000 6827 7d72  ....(h.j....h'}r
+0000c3e0: d307 0000 2868 295d 682a 5d72 d407 0000  ....(h)]h*]r....
+0000c3f0: 2868 4f6a cf07 0000 5808 0000 0070 792d  (hOj....X....py-
+0000c400: 636c 6173 7372 d507 0000 6568 2b5d 682c  classr....eh+]h,
+0000c410: 5d68 2f5d 7568 1f6a cb07 0000 6833 5d72  ]h/]uh.j....h3]r
+0000c420: d607 0000 6852 5810 0000 0073 6369 7079  ....hRX....scipy
+0000c430: 5f6d 756c 7469 6d69 6e65 7872 d707 0000  _multiminexr....
+0000c440: 8581 72d8 0700 007d 72d9 0700 0028 681e  ..r....}r....(h.
+0000c450: 5500 681f 6ad1 0700 0075 6261 6825 6856  U.h.j....ubah%hV
+0000c460: 7562 6175 6268 5258 1600 0000 2069 7320  ubaubhRX.... is 
+0000c470: 6120 7772 6170 7065 7220 666f 7220 7468  a wrapper for th
+0000c480: 6520 72da 0700 0085 8172 db07 0000 7d72  e r......r....}r
+0000c490: dc07 0000 2868 1e58 1600 0000 2069 7320  ....(h.X.... is 
+0000c4a0: 6120 7772 6170 7065 7220 666f 7220 7468  a wrapper for th
+0000c4b0: 6520 6823 4e68 314e 6832 6802 681f 6ac7  e h#Nh1Nh2h.h.j.
+0000c4c0: 0700 0075 6268 4a29 8172 dd07 0000 7d72  ...ubhJ).r....}r
+0000c4d0: de07 0000 2868 1e58 0c00 0000 6060 6d69  ....(h.X....``mi
+0000c4e0: 6e69 6d69 7a65 6060 6827 7d72 df07 0000  nimize``h'}r....
+0000c4f0: 2868 295d 682a 5d68 2b5d 682c 5d68 2f5d  (h)]h*]h+]h,]h/]
+0000c500: 7568 1f6a c707 0000 6833 5d72 e007 0000  uh.j....h3]r....
+0000c510: 6852 5808 0000 006d 696e 696d 697a 6572  hRX....minimizer
+0000c520: e107 0000 8581 72e2 0700 007d 72e3 0700  ......r....}r...
+0000c530: 0028 681e 5500 681f 6add 0700 0075 6261  .(h.U.h.j....uba
+0000c540: 6825 6856 7562 6852 5801 0000 000a 8581  h%hVubhRX.......
+0000c550: 72e4 0700 007d 72e5 0700 0028 681e 5801  r....}r....(h.X.
+0000c560: 0000 000a 6823 4e68 314e 6832 6802 681f  ....h#Nh1Nh2h.h.
+0000c570: 6ac7 0700 0075 6268 3c29 8172 e607 0000  j....ubh<).r....
+0000c580: 7d72 e707 0000 2868 1e58 0c00 0000 3a6d  }r....(h.X....:m
+0000c590: 6f64 3a60 7363 6970 7960 72e8 0700 0068  od:`scipy`r....h
+0000c5a0: 1f6a c707 0000 6823 6a76 0700 0068 2568  .j....h#jv...h%h
+0000c5b0: 4068 277d 72e9 0700 0028 5507 7265 6674  @h'}r....(U.reft
+0000c5c0: 7970 6558 0300 0000 6d6f 6468 4289 6843  ypeX....modhB.hC
+0000c5d0: 5805 0000 0073 6369 7079 5509 7265 6664  X....scipyU.refd
+0000c5e0: 6f6d 6169 6e58 0200 0000 7079 72ea 0700  omainX....pyr...
+0000c5f0: 0068 2c5d 682b 5d55 0b72 6566 6578 706c  .h,]h+]U.refexpl
+0000c600: 6963 6974 8968 295d 682a 5d68 2f5d 6845  icit.h)]h*]h/]hE
+0000c610: 6846 6847 6a24 0700 0068 486a 2107 0000  hFhGj$...hHj!...
+0000c620: 7568 314b 0768 335d 72eb 0700 0068 4a29  uh1K.h3]r....hJ)
+0000c630: 8172 ec07 0000 7d72 ed07 0000 2868 1e6a  .r....}r....(h.j
+0000c640: e807 0000 6827 7d72 ee07 0000 2868 295d  ....h'}r....(h)]
+0000c650: 682a 5d72 ef07 0000 2868 4f6a ea07 0000  h*]r....(hOj....
+0000c660: 5806 0000 0070 792d 6d6f 6472 f007 0000  X....py-modr....
+0000c670: 6568 2b5d 682c 5d68 2f5d 7568 1f6a e607  eh+]h,]h/]uh.j..
+0000c680: 0000 6833 5d72 f107 0000 6852 5805 0000  ..h3]r....hRX...
+0000c690: 0073 6369 7079 72f2 0700 0085 8172 f307  .scipyr......r..
+0000c6a0: 0000 7d72 f407 0000 2868 1e55 0068 1f6a  ..}r....(h.U.h.j
+0000c6b0: ec07 0000 7562 6168 2568 5675 6261 7562  ....ubah%hVubaub
+0000c6c0: 6852 5839 0000 0020 6675 6e63 7469 6f6e  hRX9... function
+0000c6d0: 2e20 4974 2067 6976 6573 2061 6363 6573  . It gives acces
+0000c6e0: 7320 746f 206f 6e6c 7920 7061 7274 206f  s to only part o
+0000c6f0: 6620 7468 6174 0a66 756e 6374 696f 6e2e  f that.function.
+0000c700: 72f5 0700 0085 8172 f607 0000 7d72 f707  r......r....}r..
+0000c710: 0000 2868 1e58 3900 0000 2066 756e 6374  ..(h.X9... funct
+0000c720: 696f 6e2e 2049 7420 6769 7665 7320 6163  ion. It gives ac
+0000c730: 6365 7373 2074 6f20 6f6e 6c79 2070 6172  cess to only par
+0000c740: 7420 6f66 2074 6861 740a 6675 6e63 7469  t of that.functi
+0000c750: 6f6e 2e68 234e 6831 4e68 3268 0268 1f6a  on.h#Nh1Nh2h.h.j
+0000c760: c707 0000 7562 6575 626a b601 0000 2981  ....ubeubj....).
+0000c770: 72f8 0700 007d 72f9 0700 0028 681e 5500  r....}r....(h.U.
+0000c780: 681f 6a6f 0700 0068 234e 6825 6ab9 0100  h.jo...h#Nh%j...
+0000c790: 0068 277d 72fa 0700 0028 6829 5d68 2a5d  .h'}r....(h)]h*]
+0000c7a0: 682b 5d68 2c5d 682f 5d75 6831 4e68 3268  h+]h,]h/]uh1Nh2h
+0000c7b0: 0268 335d 72fb 0700 006a bc01 0000 2981  .h3]r....j....).
+0000c7c0: 72fc 0700 007d 72fd 0700 0028 681e 5500  r....}r....(h.U.
+0000c7d0: 6827 7d72 fe07 0000 2868 295d 682a 5d68  h'}r....(h)]h*]h
+0000c7e0: 2b5d 682c 5d68 2f5d 7568 1f6a f807 0000  +]h,]h/]uh.j....
+0000c7f0: 6833 5d72 ff07 0000 286a c101 0000 2981  h3]r....(j....).
+0000c800: 7200 0800 007d 7201 0800 0028 681e 580a  r....}r....(h.X.
+0000c810: 0000 0050 6172 616d 6574 6572 7368 1f6a  ...Parametersh.j
+0000c820: fc07 0000 6823 6a1d 0700 0068 256a c401  ....h#j....h%j..
+0000c830: 0000 6827 7d72 0208 0000 2868 295d 682a  ..h'}r....(h)]h*
+0000c840: 5d68 2b5d 682c 5d68 2f5d 7568 314b 0068  ]h+]h,]h/]uh1K.h
+0000c850: 335d 7203 0800 0068 5258 0a00 0000 5061  3]r....hRX....Pa
+0000c860: 7261 6d65 7465 7273 7204 0800 0085 8172  rametersr......r
+0000c870: 0508 0000 7d72 0608 0000 2868 1e55 0068  ....}r....(h.U.h
+0000c880: 1f6a 0008 0000 7562 6175 626a ca01 0000  .j....ubaubj....
+0000c890: 2981 7207 0800 007d 7208 0800 0028 681e  ).r....}r....(h.
+0000c8a0: 5500 6827 7d72 0908 0000 2868 295d 682a  U.h'}r....(h)]h*
+0000c8b0: 5d68 2b5d 682c 5d68 2f5d 7568 1f6a fc07  ]h+]h,]h/]uh.j..
+0000c8c0: 0000 6833 5d72 0a08 0000 6acf 0100 0029  ..h3]r....j....)
+0000c8d0: 8172 0b08 0000 7d72 0c08 0000 2868 1e55  .r....}r....(h.U
+0000c8e0: 0068 277d 720d 0800 0028 6829 5d68 2a5d  .h'}r....(h)]h*]
+0000c8f0: 682b 5d68 2c5d 682f 5d75 681f 6a07 0800  h+]h,]h/]uh.j...
+0000c900: 0068 335d 720e 0800 0028 6ad4 0100 0029  .h3]r....(j....)
+0000c910: 8172 0f08 0000 7d72 1008 0000 2868 1e55  .r....}r....(h.U
+0000c920: 0068 277d 7211 0800 0028 6829 5d68 2a5d  .h'}r....(h)]h*]
+0000c930: 682b 5d68 2c5d 682f 5d75 681f 6a0b 0800  h+]h,]h/]uh.j...
+0000c940: 0068 335d 7212 0800 0068 9729 8172 1308  .h3]r....h.).r..
+0000c950: 0000 7d72 1408 0000 2868 1e58 3f00 0000  ..}r....(h.X?...
+0000c960: 7830 2028 6172 7261 7920 6f66 2066 6c6f  x0 (array of flo
+0000c970: 6174 7329 202d 2d20 5374 6172 7469 6e67  ats) -- Starting
+0000c980: 2070 6f69 6e74 2066 6f72 206d 696e 696d   point for minim
+0000c990: 697a 6174 696f 6e20 7365 6172 6368 2e68  ization search.h
+0000c9a0: 277d 7215 0800 0028 6829 5d68 2a5d 682b  '}r....(h)]h*]h+
+0000c9b0: 5d68 2c5d 682f 5d75 681f 6a0f 0800 0068  ]h,]h/]uh.j....h
+0000c9c0: 335d 7216 0800 0028 6add 0100 0029 8172  3]r....(j....).r
+0000c9d0: 1708 0000 7d72 1808 0000 2868 1e58 0200  ....}r....(h.X..
+0000c9e0: 0000 7830 6827 7d72 1908 0000 2868 2c5d  ..x0h'}r....(h,]
+0000c9f0: 682b 5d6a e101 0000 8868 295d 682a 5d68  h+]j.....h)]h*]h
+0000ca00: 2f5d 7568 1f6a 1308 0000 6833 5d72 1a08  /]uh.j....h3]r..
+0000ca10: 0000 6852 5802 0000 0078 3072 1b08 0000  ..hRX....x0r....
+0000ca20: 8581 721c 0800 007d 721d 0800 0028 681e  ..r....}r....(h.
+0000ca30: 5500 681f 6a17 0800 0075 6261 6825 6ae6  U.h.j....ubah%j.
+0000ca40: 0100 0075 6268 5258 0200 0000 2028 721e  ...ubhRX.... (r.
+0000ca50: 0800 0085 8172 1f08 0000 7d72 2008 0000  .....r....}r ...
+0000ca60: 2868 1e55 0068 1f6a 1308 0000 7562 683c  (h.U.h.j....ubh<
+0000ca70: 2981 7221 0800 007d 7222 0800 0028 681e  ).r!...}r"...(h.
+0000ca80: 5500 6827 7d72 2308 0000 2855 0772 6566  U.h'}r#...(U.ref
+0000ca90: 7479 7065 68f2 6ae1 0100 0088 5509 7265  typeh.j.....U.re
+0000caa0: 6674 6172 6765 7458 0f00 0000 6172 7261  ftargetX....arra
+0000cab0: 7920 6f66 2066 6c6f 6174 7372 2408 0000  y of floatsr$...
+0000cac0: 5509 7265 6664 6f6d 6169 6e6a 1807 0000  U.refdomainj....
+0000cad0: 682c 5d68 2b5d 550b 7265 6665 7870 6c69  h,]h+]U.refexpli
+0000cae0: 6369 7489 6829 5d68 2a5d 682f 5d75 681f  cit.h)]h*]h/]uh.
+0000caf0: 6a13 0800 0068 335d 7225 0800 006a ef01  j....h3]r%...j..
+0000cb00: 0000 2981 7226 0800 007d 7227 0800 0028  ..).r&...}r'...(
+0000cb10: 681e 6a24 0800 0068 277d 7228 0800 0028  h.j$...h'}r(...(
+0000cb20: 6829 5d68 2a5d 682b 5d68 2c5d 682f 5d75  h)]h*]h+]h,]h/]u
+0000cb30: 681f 6a21 0800 0068 335d 7229 0800 0068  h.j!...h3]r)...h
+0000cb40: 5258 0f00 0000 6172 7261 7920 6f66 2066  RX....array of f
+0000cb50: 6c6f 6174 7372 2a08 0000 8581 722b 0800  loatsr*.....r+..
+0000cb60: 007d 722c 0800 0028 681e 5500 681f 6a26  .}r,...(h.U.h.j&
+0000cb70: 0800 0075 6261 6825 6af7 0100 0075 6261  ...ubah%j....uba
+0000cb80: 6825 6840 7562 6852 5801 0000 0029 8581  h%h@ubhRX....)..
+0000cb90: 722d 0800 007d 722e 0800 0028 681e 5500  r-...}r....(h.U.
+0000cba0: 681f 6a13 0800 0075 6268 5258 0500 0000  h.j....ubhRX....
+0000cbb0: 20e2 8093 2072 2f08 0000 8581 7230 0800   ... r/.....r0..
+0000cbc0: 007d 7231 0800 0028 681e 5500 681f 6a13  .}r1...(h.U.h.j.
+0000cbd0: 0800 0075 6268 5258 2700 0000 5374 6172  ...ubhRX'...Star
+0000cbe0: 7469 6e67 2070 6f69 6e74 2066 6f72 206d  ting point for m
+0000cbf0: 696e 696d 697a 6174 696f 6e20 7365 6172  inimization sear
+0000cc00: 6368 2e72 3208 0000 8581 7233 0800 007d  ch.r2.....r3...}
+0000cc10: 7234 0800 0028 681e 5827 0000 0053 7461  r4...(h.X'...Sta
+0000cc20: 7274 696e 6720 706f 696e 7420 666f 7220  rting point for 
+0000cc30: 6d69 6e69 6d69 7a61 7469 6f6e 2073 6561  minimization sea
+0000cc40: 7263 682e 7235 0800 0068 234e 6831 4e68  rch.r5...h#Nh1Nh
+0000cc50: 3268 0268 1f6a 1308 0000 7562 6568 2568  2h.h.j....ubeh%h
+0000cc60: 9a75 6261 6825 6a00 0200 0075 626a d401  .ubah%j....ubj..
+0000cc70: 0000 2981 7236 0800 007d 7237 0800 0028  ..).r6...}r7...(
+0000cc80: 681e 5500 6827 7d72 3808 0000 2868 295d  h.U.h'}r8...(h)]
+0000cc90: 682a 5d68 2b5d 682c 5d68 2f5d 7568 1f6a  h*]h+]h,]h/]uh.j
+0000cca0: 0b08 0000 6833 5d72 3908 0000 6897 2981  ....h3]r9...h.).
+0000ccb0: 723a 0800 007d 723b 0800 0028 681e 5837  r:...}r;...(h.X7
+0000ccc0: 0000 0066 202d 2d20 4675 6e63 7469 6f6e  ...f -- Function
+0000ccd0: 2066 2878 2920 746f 2062 6520 6d69 6e69   f(x) to be mini
+0000cce0: 6d69 7a65 6420 6279 2076 6172 7969 6e67  mized by varying
+0000ccf0: 2076 6563 746f 7220 782e 6827 7d72 3c08   vector x.h'}r<.
+0000cd00: 0000 2868 295d 682a 5d68 2b5d 682c 5d68  ..(h)]h*]h+]h,]h
+0000cd10: 2f5d 7568 1f6a 3608 0000 6833 5d72 3d08  /]uh.j6...h3]r=.
+0000cd20: 0000 286a dd01 0000 2981 723e 0800 007d  ..(j....).r>...}
+0000cd30: 723f 0800 0028 681e 5801 0000 0066 6827  r?...(h.X....fh'
+0000cd40: 7d72 4008 0000 2868 2c5d 682b 5d6a e101  }r@...(h,]h+]j..
+0000cd50: 0000 8868 295d 682a 5d68 2f5d 7568 1f6a  ...h)]h*]h/]uh.j
+0000cd60: 3a08 0000 6833 5d72 4108 0000 6852 5801  :...h3]rA...hRX.
+0000cd70: 0000 0066 8581 7242 0800 007d 7243 0800  ...f..rB...}rC..
+0000cd80: 0028 681e 5500 681f 6a3e 0800 0075 6261  .(h.U.h.j>...uba
+0000cd90: 6825 6ae6 0100 0075 6268 5258 0500 0000  h%j....ubhRX....
+0000cda0: 20e2 8093 2072 4408 0000 8581 7245 0800   ... rD.....rE..
+0000cdb0: 007d 7246 0800 0028 681e 5500 681f 6a3a  .}rF...(h.U.h.j:
+0000cdc0: 0800 0075 6268 5258 0900 0000 4675 6e63  ...ubhRX....Func
+0000cdd0: 7469 6f6e 2072 4708 0000 8581 7248 0800  tion rG.....rH..
+0000cde0: 007d 7249 0800 0028 681e 5809 0000 0046  .}rI...(h.X....F
+0000cdf0: 756e 6374 696f 6e20 724a 0800 0068 234e  unction rJ...h#N
+0000ce00: 6831 4e68 3268 0268 1f6a 3a08 0000 7562  h1Nh2h.h.j:...ub
+0000ce10: 684a 2981 724b 0800 007d 724c 0800 0028  hJ).rK...}rL...(
+0000ce20: 681e 5808 0000 0060 6066 2878 2960 6068  h.X....``f(x)``h
+0000ce30: 1f6a 3a08 0000 6823 4e68 2568 5668 277d  .j:...h#Nh%hVh'}
+0000ce40: 724d 0800 0028 6829 5d68 2a5d 682b 5d68  rM...(h)]h*]h+]h
+0000ce50: 2c5d 682f 5d75 6831 4e68 3268 0268 335d  ,]h/]uh1Nh2h.h3]
+0000ce60: 724e 0800 0068 5258 0400 0000 6628 7829  rN...hRX....f(x)
+0000ce70: 724f 0800 0085 8172 5008 0000 7d72 5108  rO.....rP...}rQ.
+0000ce80: 0000 2868 1e55 0068 234e 6831 4e68 3268  ..(h.U.h#Nh1Nh2h
+0000ce90: 0268 1f6a 4b08 0000 7562 6175 6268 5258  .h.jK...ubaubhRX
+0000cea0: 2300 0000 2074 6f20 6265 206d 696e 696d  #... to be minim
+0000ceb0: 697a 6564 2062 7920 7661 7279 696e 6720  ized by varying 
+0000cec0: 7665 6374 6f72 2072 5208 0000 8581 7253  vector rR.....rS
+0000ced0: 0800 007d 7254 0800 0028 681e 5823 0000  ...}rT...(h.X#..
+0000cee0: 0020 746f 2062 6520 6d69 6e69 6d69 7a65  . to be minimize
+0000cef0: 6420 6279 2076 6172 7969 6e67 2076 6563  d by varying vec
+0000cf00: 746f 7220 7255 0800 0068 234e 6831 4e68  tor rU...h#Nh1Nh
+0000cf10: 3268 0268 1f6a 3a08 0000 7562 684a 2981  2h.h.j:...ubhJ).
+0000cf20: 7256 0800 007d 7257 0800 0028 681e 5805  rV...}rW...(h.X.
+0000cf30: 0000 0060 6078 6060 681f 6a3a 0800 0068  ...``x``h.j:...h
+0000cf40: 234e 6825 6856 6827 7d72 5808 0000 2868  #Nh%hVh'}rX...(h
+0000cf50: 295d 682a 5d68 2b5d 682c 5d68 2f5d 7568  )]h*]h+]h,]h/]uh
+0000cf60: 314e 6832 6802 6833 5d72 5908 0000 6852  1Nh2h.h3]rY...hR
+0000cf70: 5801 0000 0078 8581 725a 0800 007d 725b  X....x..rZ...}r[
+0000cf80: 0800 0028 681e 5500 6823 4e68 314e 6832  ...(h.U.h#Nh1Nh2
+0000cf90: 6802 681f 6a56 0800 0075 6261 7562 6852  h.h.jV...ubaubhR
+0000cfa0: 5801 0000 002e 8581 725c 0800 007d 725d  X.......r\...}r]
+0000cfb0: 0800 0028 681e 5801 0000 002e 6823 4e68  ...(h.X.....h#Nh
+0000cfc0: 314e 6832 6802 681f 6a3a 0800 0075 6265  1Nh2h.h.j:...ube
+0000cfd0: 6825 689a 7562 6168 256a 0002 0000 7562  h%h.ubah%j....ub
+0000cfe0: 6ad4 0100 0029 8172 5e08 0000 7d72 5f08  j....).r^...}r_.
+0000cff0: 0000 2868 1e55 0068 277d 7260 0800 0028  ..(h.U.h'}r`...(
+0000d000: 6829 5d68 2a5d 682b 5d68 2c5d 682f 5d75  h)]h*]h+]h,]h/]u
+0000d010: 681f 6a0b 0800 0068 335d 7261 0800 0068  h.j....h3]ra...h
+0000d020: 9729 8172 6208 0000 7d72 6308 0000 2868  .).rb...}rc...(h
+0000d030: 1e58 5e00 0000 746f 6c20 2866 6c6f 6174  .X^...tol (float
+0000d040: 2920 2d2d 204d 696e 696d 697a 6174 696f  ) -- Minimizatio
+0000d050: 6e20 7374 6f70 7320 7768 656e 2078 2068  n stops when x h
+0000d060: 6173 2063 6f6e 7665 7267 6564 2074 6f20  as converged to 
+0000d070: 7769 7468 0a74 6f6c 6572 616e 6365 2074  with.tolerance t
+0000d080: 6f6c 3b20 6465 6661 756c 7420 6973 2031  ol; default is 1
+0000d090: 652d 342e 6827 7d72 6408 0000 2868 295d  e-4.h'}rd...(h)]
+0000d0a0: 682a 5d68 2b5d 682c 5d68 2f5d 7568 1f6a  h*]h+]h,]h/]uh.j
+0000d0b0: 5e08 0000 6833 5d72 6508 0000 286a dd01  ^...h3]re...(j..
+0000d0c0: 0000 2981 7266 0800 007d 7267 0800 0028  ..).rf...}rg...(
+0000d0d0: 681e 5803 0000 0074 6f6c 6827 7d72 6808  h.X....tolh'}rh.
+0000d0e0: 0000 2868 2c5d 682b 5d6a e101 0000 8868  ..(h,]h+]j.....h
+0000d0f0: 295d 682a 5d68 2f5d 7568 1f6a 6208 0000  )]h*]h/]uh.jb...
+0000d100: 6833 5d72 6908 0000 6852 5803 0000 0074  h3]ri...hRX....t
+0000d110: 6f6c 726a 0800 0085 8172 6b08 0000 7d72  olrj.....rk...}r
+0000d120: 6c08 0000 2868 1e55 0068 1f6a 6608 0000  l...(h.U.h.jf...
+0000d130: 7562 6168 256a e601 0000 7562 6852 5802  ubah%j....ubhRX.
+0000d140: 0000 0020 2872 6d08 0000 8581 726e 0800  ... (rm.....rn..
+0000d150: 007d 726f 0800 0028 681e 5500 681f 6a62  .}ro...(h.U.h.jb
+0000d160: 0800 0075 6268 3c29 8172 7008 0000 7d72  ...ubh<).rp...}r
+0000d170: 7108 0000 2868 1e55 0068 277d 7272 0800  q...(h.U.h'}rr..
+0000d180: 0028 5507 7265 6674 7970 6568 f26a e101  .(U.reftypeh.j..
+0000d190: 0000 8855 0972 6566 7461 7267 6574 5805  ...U.reftargetX.
+0000d1a0: 0000 0066 6c6f 6174 7273 0800 0055 0972  ...floatrs...U.r
+0000d1b0: 6566 646f 6d61 696e 6a18 0700 0068 2c5d  efdomainj....h,]
+0000d1c0: 682b 5d55 0b72 6566 6578 706c 6963 6974  h+]U.refexplicit
+0000d1d0: 8968 295d 682a 5d68 2f5d 7568 1f6a 6208  .h)]h*]h/]uh.jb.
+0000d1e0: 0000 6833 5d72 7408 0000 6aef 0100 0029  ..h3]rt...j....)
+0000d1f0: 8172 7508 0000 7d72 7608 0000 2868 1e6a  .ru...}rv...(h.j
+0000d200: 7308 0000 6827 7d72 7708 0000 2868 295d  s...h'}rw...(h)]
+0000d210: 682a 5d68 2b5d 682c 5d68 2f5d 7568 1f6a  h*]h+]h,]h/]uh.j
+0000d220: 7008 0000 6833 5d72 7808 0000 6852 5805  p...h3]rx...hRX.
+0000d230: 0000 0066 6c6f 6174 7279 0800 0085 8172  ...floatry.....r
+0000d240: 7a08 0000 7d72 7b08 0000 2868 1e55 0068  z...}r{...(h.U.h
+0000d250: 1f6a 7508 0000 7562 6168 256a f701 0000  .ju...ubah%j....
+0000d260: 7562 6168 2568 4075 6268 5258 0100 0000  ubah%h@ubhRX....
+0000d270: 2985 8172 7c08 0000 7d72 7d08 0000 2868  )..r|...}r}...(h
+0000d280: 1e55 0068 1f6a 6208 0000 7562 6852 5805  .U.h.jb...ubhRX.
+0000d290: 0000 0020 e280 9320 727e 0800 0085 8172  ... ... r~.....r
+0000d2a0: 7f08 0000 7d72 8008 0000 2868 1e55 0068  ....}r....(h.U.h
+0000d2b0: 1f6a 6208 0000 7562 6852 5818 0000 004d  .jb...ubhRX....M
+0000d2c0: 696e 696d 697a 6174 696f 6e20 7374 6f70  inimization stop
+0000d2d0: 7320 7768 656e 2072 8108 0000 8581 7282  s when r......r.
+0000d2e0: 0800 007d 7283 0800 0028 681e 5818 0000  ...}r....(h.X...
+0000d2f0: 004d 696e 696d 697a 6174 696f 6e20 7374  .Minimization st
+0000d300: 6f70 7320 7768 656e 2072 8408 0000 6823  ops when r....h#
+0000d310: 4e68 314e 6832 6802 681f 6a62 0800 0075  Nh1Nh2h.h.jb...u
+0000d320: 6268 4a29 8172 8508 0000 7d72 8608 0000  bhJ).r....}r....
+0000d330: 2868 1e58 0500 0000 6060 7860 6068 1f6a  (h.X....``x``h.j
+0000d340: 6208 0000 6823 4e68 2568 5668 277d 7287  b...h#Nh%hVh'}r.
+0000d350: 0800 0028 6829 5d68 2a5d 682b 5d68 2c5d  ...(h)]h*]h+]h,]
+0000d360: 682f 5d75 6831 4e68 3268 0268 335d 7288  h/]uh1Nh2h.h3]r.
+0000d370: 0800 0068 5258 0100 0000 7885 8172 8908  ...hRX....x..r..
+0000d380: 0000 7d72 8a08 0000 2868 1e55 0068 234e  ..}r....(h.U.h#N
+0000d390: 6831 4e68 3268 0268 1f6a 8508 0000 7562  h1Nh2h.h.j....ub
+0000d3a0: 6175 6268 5258 2100 0000 2068 6173 2063  aubhRX!... has c
+0000d3b0: 6f6e 7665 7267 6564 2074 6f20 7769 7468  onverged to with
+0000d3c0: 0a74 6f6c 6572 616e 6365 2072 8b08 0000  .tolerance r....
+0000d3d0: 8581 728c 0800 007d 728d 0800 0028 681e  ..r....}r....(h.
+0000d3e0: 5821 0000 0020 6861 7320 636f 6e76 6572  X!... has conver
+0000d3f0: 6765 6420 746f 2077 6974 680a 746f 6c65  ged to with.tole
+0000d400: 7261 6e63 6520 728e 0800 0068 234e 6831  rance r....h#Nh1
+0000d410: 4e68 3268 0268 1f6a 6208 0000 7562 684a  Nh2h.h.jb...ubhJ
+0000d420: 2981 728f 0800 007d 7290 0800 0028 681e  ).r....}r....(h.
+0000d430: 5807 0000 0060 6074 6f6c 6060 681f 6a62  X....``tol``h.jb
+0000d440: 0800 0068 234e 6825 6856 6827 7d72 9108  ...h#Nh%hVh'}r..
+0000d450: 0000 2868 295d 682a 5d68 2b5d 682c 5d68  ..(h)]h*]h+]h,]h
+0000d460: 2f5d 7568 314e 6832 6802 6833 5d72 9208  /]uh1Nh2h.h3]r..
+0000d470: 0000 6852 5803 0000 0074 6f6c 7293 0800  ..hRX....tolr...
+0000d480: 0085 8172 9408 0000 7d72 9508 0000 2868  ...r....}r....(h
+0000d490: 1e55 0068 234e 6831 4e68 3268 0268 1f6a  .U.h#Nh1Nh2h.h.j
+0000d4a0: 8f08 0000 7562 6175 6268 5258 0d00 0000  ....ubaubhRX....
+0000d4b0: 3b20 6465 6661 756c 7420 6973 2072 9608  ; default is r..
+0000d4c0: 0000 8581 7297 0800 007d 7298 0800 0028  ....r....}r....(
+0000d4d0: 681e 580d 0000 003b 2064 6566 6175 6c74  h.X....; default
+0000d4e0: 2069 7320 7299 0800 0068 234e 6831 4e68   is r....h#Nh1Nh
+0000d4f0: 3268 0268 1f6a 6208 0000 7562 684a 2981  2h.h.jb...ubhJ).
+0000d500: 729a 0800 007d 729b 0800 0028 681e 5808  r....}r....(h.X.
+0000d510: 0000 0060 6031 652d 3460 6068 1f6a 6208  ...``1e-4``h.jb.
+0000d520: 0000 6823 4e68 2568 5668 277d 729c 0800  ..h#Nh%hVh'}r...
+0000d530: 0028 6829 5d68 2a5d 682b 5d68 2c5d 682f  .(h)]h*]h+]h,]h/
+0000d540: 5d75 6831 4e68 3268 0268 335d 729d 0800  ]uh1Nh2h.h3]r...
+0000d550: 0068 5258 0400 0000 3165 2d34 729e 0800  .hRX....1e-4r...
+0000d560: 0085 8172 9f08 0000 7d72 a008 0000 2868  ...r....}r....(h
+0000d570: 1e55 0068 234e 6831 4e68 3268 0268 1f6a  .U.h#Nh1Nh2h.h.j
+0000d580: 9a08 0000 7562 6175 6268 5258 0100 0000  ....ubaubhRX....
+0000d590: 2e85 8172 a108 0000 7d72 a208 0000 2868  ...r....}r....(h
+0000d5a0: 1e58 0100 0000 2e68 234e 6831 4e68 3268  .X.....h#Nh1Nh2h
+0000d5b0: 0268 1f6a 6208 0000 7562 6568 2568 9a75  .h.jb...ubeh%h.u
+0000d5c0: 6261 6825 6a00 0200 0075 626a d401 0000  bah%j....ubj....
+0000d5d0: 2981 72a3 0800 007d 72a4 0800 0028 681e  ).r....}r....(h.
+0000d5e0: 5500 6827 7d72 a508 0000 2868 295d 682a  U.h'}r....(h)]h*
+0000d5f0: 5d68 2b5d 682c 5d68 2f5d 7568 1f6a 0b08  ]h+]h,]h/]uh.j..
+0000d600: 0000 6833 5d72 a608 0000 6897 2981 72a7  ..h3]r....h.).r.
+0000d610: 0800 007d 72a8 0800 0028 681e 585c 0000  ...}r....(h.X\..
+0000d620: 006d 6178 6974 2028 706f 7369 7469 7665  .maxit (positive
+0000d630: 2069 6e74 2920 2d2d 204d 6178 696d 756d   int) -- Maximum
+0000d640: 206e 756d 6265 7220 6f66 2069 7465 7261   number of itera
+0000d650: 7469 6f6e 7320 696e 2073 6561 7263 6820  tions in search 
+0000d660: 666f 7220 6d69 6e69 6d75 6d3b 0a64 6566  for minimum;.def
+0000d670: 6175 6c74 2069 7320 3130 3030 2e68 277d  ault is 1000.h'}
+0000d680: 72a9 0800 0028 6829 5d68 2a5d 682b 5d68  r....(h)]h*]h+]h
+0000d690: 2c5d 682f 5d75 681f 6aa3 0800 0068 335d  ,]h/]uh.j....h3]
+0000d6a0: 72aa 0800 0028 6add 0100 0029 8172 ab08  r....(j....).r..
+0000d6b0: 0000 7d72 ac08 0000 2868 1e58 0500 0000  ..}r....(h.X....
+0000d6c0: 6d61 7869 7468 277d 72ad 0800 0028 682c  maxith'}r....(h,
+0000d6d0: 5d68 2b5d 6ae1 0100 0088 6829 5d68 2a5d  ]h+]j.....h)]h*]
+0000d6e0: 682f 5d75 681f 6aa7 0800 0068 335d 72ae  h/]uh.j....h3]r.
+0000d6f0: 0800 0068 5258 0500 0000 6d61 7869 7472  ...hRX....maxitr
+0000d700: af08 0000 8581 72b0 0800 007d 72b1 0800  ......r....}r...
+0000d710: 0028 681e 5500 681f 6aab 0800 0075 6261  .(h.U.h.j....uba
+0000d720: 6825 6ae6 0100 0075 6268 5258 0200 0000  h%j....ubhRX....
+0000d730: 2028 72b2 0800 0085 8172 b308 0000 7d72   (r......r....}r
+0000d740: b408 0000 2868 1e55 0068 1f6a a708 0000  ....(h.U.h.j....
+0000d750: 7562 683c 2981 72b5 0800 007d 72b6 0800  ubh<).r....}r...
+0000d760: 0028 681e 5500 6827 7d72 b708 0000 2855  .(h.U.h'}r....(U
+0000d770: 0772 6566 7479 7065 68f2 6ae1 0100 0088  .reftypeh.j.....
+0000d780: 5509 7265 6674 6172 6765 7458 0c00 0000  U.reftargetX....
+0000d790: 706f 7369 7469 7665 2069 6e74 72b8 0800  positive intr...
+0000d7a0: 0055 0972 6566 646f 6d61 696e 6a18 0700  .U.refdomainj...
+0000d7b0: 0068 2c5d 682b 5d55 0b72 6566 6578 706c  .h,]h+]U.refexpl
+0000d7c0: 6963 6974 8968 295d 682a 5d68 2f5d 7568  icit.h)]h*]h/]uh
+0000d7d0: 1f6a a708 0000 6833 5d72 b908 0000 6aef  .j....h3]r....j.
+0000d7e0: 0100 0029 8172 ba08 0000 7d72 bb08 0000  ...).r....}r....
+0000d7f0: 2868 1e6a b808 0000 6827 7d72 bc08 0000  (h.j....h'}r....
+0000d800: 2868 295d 682a 5d68 2b5d 682c 5d68 2f5d  (h)]h*]h+]h,]h/]
+0000d810: 7568 1f6a b508 0000 6833 5d72 bd08 0000  uh.j....h3]r....
+0000d820: 6852 580c 0000 0070 6f73 6974 6976 6520  hRX....positive 
+0000d830: 696e 7472 be08 0000 8581 72bf 0800 007d  intr......r....}
+0000d840: 72c0 0800 0028 681e 5500 681f 6aba 0800  r....(h.U.h.j...
+0000d850: 0075 6261 6825 6af7 0100 0075 6261 6825  .ubah%j....ubah%
+0000d860: 6840 7562 6852 5801 0000 0029 8581 72c1  h@ubhRX....)..r.
+0000d870: 0800 007d 72c2 0800 0028 681e 5500 681f  ...}r....(h.U.h.
+0000d880: 6aa7 0800 0075 6268 5258 0500 0000 20e2  j....ubhRX.... .
+0000d890: 8093 2072 c308 0000 8581 72c4 0800 007d  .. r......r....}
+0000d8a0: 72c5 0800 0028 681e 5500 681f 6aa7 0800  r....(h.U.h.j...
+0000d8b0: 0075 6268 5258 4400 0000 4d61 7869 6d75  .ubhRXD...Maximu
+0000d8c0: 6d20 6e75 6d62 6572 206f 6620 6974 6572  m number of iter
+0000d8d0: 6174 696f 6e73 2069 6e20 7365 6172 6368  ations in search
+0000d8e0: 2066 6f72 206d 696e 696d 756d 3b0a 6465   for minimum;.de
+0000d8f0: 6661 756c 7420 6973 2031 3030 302e 72c6  fault is 1000.r.
+0000d900: 0800 0085 8172 c708 0000 7d72 c808 0000  .....r....}r....
+0000d910: 2868 1e58 4400 0000 4d61 7869 6d75 6d20  (h.XD...Maximum 
+0000d920: 6e75 6d62 6572 206f 6620 6974 6572 6174  number of iterat
+0000d930: 696f 6e73 2069 6e20 7365 6172 6368 2066  ions in search f
+0000d940: 6f72 206d 696e 696d 756d 3b0a 6465 6661  or minimum;.defa
+0000d950: 756c 7420 6973 2031 3030 302e 72c9 0800  ult is 1000.r...
+0000d960: 0068 234e 6831 4e68 3268 0268 1f6a a708  .h#Nh1Nh2h.h.j..
+0000d970: 0000 7562 6568 2568 9a75 6261 6825 6a00  ..ubeh%h.ubah%j.
+0000d980: 0200 0075 626a d401 0000 2981 72ca 0800  ...ubj....).r...
+0000d990: 007d 72cb 0800 0028 681e 5500 6827 7d72  .}r....(h.U.h'}r
+0000d9a0: cc08 0000 2868 295d 682a 5d68 2b5d 682c  ....(h)]h*]h+]h,
+0000d9b0: 5d68 2f5d 7568 1f6a 0b08 0000 6833 5d72  ]h/]uh.j....h3]r
+0000d9c0: cd08 0000 6897 2981 72ce 0800 007d 72cf  ....h.).r....}r.
+0000d9d0: 0800 0028 681e 5889 0000 0061 6e61 6c79  ...(h.X....analy
+0000d9e0: 7a65 7220 2866 756e 6374 696f 6e29 202d  zer (function) -
+0000d9f0: 2d20 4f70 7469 6f6e 616c 2066 756e 6374  - Optional funct
+0000da00: 696f 6e20 6f66 2074 6865 2063 7572 7265  ion of the curre
+0000da10: 6e74 2078 2e0a 5468 6973 2063 616e 2062  nt x..This can b
+0000da20: 6520 7573 6564 2074 6f20 696e 7370 6563  e used to inspec
+0000da30: 7420 696e 7465 726d 6564 6961 7465 2073  t intermediate s
+0000da40: 7465 7073 2069 6e20 7468 650a 6d69 6e69  teps in the.mini
+0000da50: 6d69 7a61 7469 6f6e 2c20 6966 206e 6565  mization, if nee
+0000da60: 6465 642e 6827 7d72 d008 0000 2868 295d  ded.h'}r....(h)]
+0000da70: 682a 5d68 2b5d 682c 5d68 2f5d 7568 1f6a  h*]h+]h,]h/]uh.j
+0000da80: ca08 0000 6833 5d72 d108 0000 286a dd01  ....h3]r....(j..
+0000da90: 0000 2981 72d2 0800 007d 72d3 0800 0028  ..).r....}r....(
+0000daa0: 681e 5808 0000 0061 6e61 6c79 7a65 7268  h.X....analyzerh
+0000dab0: 277d 72d4 0800 0028 682c 5d68 2b5d 6ae1  '}r....(h,]h+]j.
+0000dac0: 0100 0088 6829 5d68 2a5d 682f 5d75 681f  ....h)]h*]h/]uh.
+0000dad0: 6ace 0800 0068 335d 72d5 0800 0068 5258  j....h3]r....hRX
+0000dae0: 0800 0000 616e 616c 797a 6572 72d6 0800  ....analyzerr...
+0000daf0: 0085 8172 d708 0000 7d72 d808 0000 2868  ...r....}r....(h
+0000db00: 1e55 0068 1f6a d208 0000 7562 6168 256a  .U.h.j....ubah%j
+0000db10: e601 0000 7562 6852 5802 0000 0020 2872  ....ubhRX.... (r
+0000db20: d908 0000 8581 72da 0800 007d 72db 0800  ......r....}r...
+0000db30: 0028 681e 5500 681f 6ace 0800 0075 6268  .(h.U.h.j....ubh
+0000db40: 3c29 8172 dc08 0000 7d72 dd08 0000 2868  <).r....}r....(h
+0000db50: 1e55 0068 277d 72de 0800 0028 5507 7265  .U.h'}r....(U.re
+0000db60: 6674 7970 6568 f26a e101 0000 8855 0972  ftypeh.j.....U.r
+0000db70: 6566 7461 7267 6574 5808 0000 0066 756e  eftargetX....fun
+0000db80: 6374 696f 6e72 df08 0000 5509 7265 6664  ctionr....U.refd
+0000db90: 6f6d 6169 6e6a 1807 0000 682c 5d68 2b5d  omainj....h,]h+]
+0000dba0: 550b 7265 6665 7870 6c69 6369 7489 6829  U.refexplicit.h)
+0000dbb0: 5d68 2a5d 682f 5d75 681f 6ace 0800 0068  ]h*]h/]uh.j....h
+0000dbc0: 335d 72e0 0800 006a ef01 0000 2981 72e1  3]r....j....).r.
+0000dbd0: 0800 007d 72e2 0800 0028 681e 6adf 0800  ...}r....(h.j...
+0000dbe0: 0068 277d 72e3 0800 0028 6829 5d68 2a5d  .h'}r....(h)]h*]
+0000dbf0: 682b 5d68 2c5d 682f 5d75 681f 6adc 0800  h+]h,]h/]uh.j...
+0000dc00: 0068 335d 72e4 0800 0068 5258 0800 0000  .h3]r....hRX....
+0000dc10: 6675 6e63 7469 6f6e 72e5 0800 0085 8172  functionr......r
+0000dc20: e608 0000 7d72 e708 0000 2868 1e55 0068  ....}r....(h.U.h
+0000dc30: 1f6a e108 0000 7562 6168 256a f701 0000  .j....ubah%j....
+0000dc40: 7562 6168 2568 4075 6268 5258 0100 0000  ubah%h@ubhRX....
+0000dc50: 2985 8172 e808 0000 7d72 e908 0000 2868  )..r....}r....(h
+0000dc60: 1e55 0068 1f6a ce08 0000 7562 6852 5805  .U.h.j....ubhRX.
+0000dc70: 0000 0020 e280 9320 72ea 0800 0085 8172  ... ... r......r
+0000dc80: eb08 0000 7d72 ec08 0000 2868 1e55 0068  ....}r....(h.U.h
+0000dc90: 1f6a ce08 0000 7562 6852 5821 0000 004f  .j....ubhRX!...O
+0000dca0: 7074 696f 6e61 6c20 6675 6e63 7469 6f6e  ptional function
+0000dcb0: 206f 6620 7468 6520 6375 7272 656e 7420   of the current 
+0000dcc0: 72ed 0800 0085 8172 ee08 0000 7d72 ef08  r......r....}r..
+0000dcd0: 0000 2868 1e58 2100 0000 4f70 7469 6f6e  ..(h.X!...Option
+0000dce0: 616c 2066 756e 6374 696f 6e20 6f66 2074  al function of t
+0000dcf0: 6865 2063 7572 7265 6e74 2072 f008 0000  he current r....
+0000dd00: 6823 4e68 314e 6832 6802 681f 6ace 0800  h#Nh1Nh2h.h.j...
+0000dd10: 0075 6268 4a29 8172 f108 0000 7d72 f208  .ubhJ).r....}r..
+0000dd20: 0000 2868 1e58 0500 0000 6060 7860 6068  ..(h.X....``x``h
+0000dd30: 1f6a ce08 0000 6823 4e68 2568 5668 277d  .j....h#Nh%hVh'}
+0000dd40: 72f3 0800 0028 6829 5d68 2a5d 682b 5d68  r....(h)]h*]h+]h
+0000dd50: 2c5d 682f 5d75 6831 4e68 3268 0268 335d  ,]h/]uh1Nh2h.h3]
+0000dd60: 72f4 0800 0068 5258 0100 0000 7885 8172  r....hRX....x..r
+0000dd70: f508 0000 7d72 f608 0000 2868 1e55 0068  ....}r....(h.U.h
+0000dd80: 234e 6831 4e68 3268 0268 1f6a f108 0000  #Nh1Nh2h.h.j....
+0000dd90: 7562 6175 6268 5258 5000 0000 2e0a 5468  ubaubhRXP.....Th
+0000dda0: 6973 2063 616e 2062 6520 7573 6564 2074  is can be used t
+0000ddb0: 6f20 696e 7370 6563 7420 696e 7465 726d  o inspect interm
+0000ddc0: 6564 6961 7465 2073 7465 7073 2069 6e20  ediate steps in 
+0000ddd0: 7468 650a 6d69 6e69 6d69 7a61 7469 6f6e  the.minimization
+0000dde0: 2c20 6966 206e 6565 6465 642e 72f7 0800  , if needed.r...
+0000ddf0: 0085 8172 f808 0000 7d72 f908 0000 2868  ...r....}r....(h
+0000de00: 1e58 5000 0000 2e0a 5468 6973 2063 616e  .XP.....This can
+0000de10: 2062 6520 7573 6564 2074 6f20 696e 7370   be used to insp
+0000de20: 6563 7420 696e 7465 726d 6564 6961 7465  ect intermediate
+0000de30: 2073 7465 7073 2069 6e20 7468 650a 6d69   steps in the.mi
+0000de40: 6e69 6d69 7a61 7469 6f6e 2c20 6966 206e  nimization, if n
+0000de50: 6565 6465 642e 72fa 0800 0068 234e 6831  eeded.r....h#Nh1
+0000de60: 4e68 3268 0268 1f6a ce08 0000 7562 6568  Nh2h.h.j....ubeh
+0000de70: 2568 9a75 6261 6825 6a00 0200 0075 6265  %h.ubah%j....ube
+0000de80: 6825 6a66 0400 0075 6261 6825 6a67 0400  h%jf...ubah%jg..
+0000de90: 0075 6265 6825 6a68 0400 0075 6261 7562  .ubeh%jh...ubaub
+0000dea0: 6897 2981 72fb 0800 007d 72fc 0800 0028  h.).r....}r....(
+0000deb0: 681e 5847 0000 003a 636c 6173 733a 606c  h.XG...:class:`l
+0000dec0: 7371 6669 742e 7363 6970 795f 6d75 6c74  sqfit.scipy_mult
+0000ded0: 696d 696e 6578 6020 6f62 6a65 6374 7320  iminex` objects 
+0000dee0: 6861 7665 2074 6865 2066 6f6c 6c6f 7769  have the followi
+0000def0: 6e67 2061 7474 7269 6275 7465 732e 72fd  ng attributes.r.
+0000df00: 0800 0068 1f6a 6f07 0000 6823 6a76 0700  ...h.jo...h#jv..
+0000df10: 0068 2568 9a68 277d 72fe 0800 0028 6829  .h%h.h'}r....(h)
+0000df20: 5d68 2a5d 682b 5d68 2c5d 682f 5d75 6831  ]h*]h+]h,]h/]uh1
+0000df30: 4b19 6832 6802 6833 5d72 ff08 0000 2868  K.h2h.h3]r....(h
+0000df40: 3c29 8172 0009 0000 7d72 0109 0000 2868  <).r....}r....(h
+0000df50: 1e58 2000 0000 3a63 6c61 7373 3a60 6c73  .X ...:class:`ls
+0000df60: 7166 6974 2e73 6369 7079 5f6d 756c 7469  qfit.scipy_multi
+0000df70: 6d69 6e65 7860 7202 0900 0068 1f6a fb08  minex`r....h.j..
+0000df80: 0000 6823 6a76 0700 0068 2568 4068 277d  ..h#jv...h%h@h'}
+0000df90: 7203 0900 0028 5507 7265 6674 7970 6558  r....(U.reftypeX
+0000dfa0: 0500 0000 636c 6173 7368 4289 6843 5817  ....classhB.hCX.
+0000dfb0: 0000 006c 7371 6669 742e 7363 6970 795f  ...lsqfit.scipy_
+0000dfc0: 6d75 6c74 696d 696e 6578 5509 7265 6664  multiminexU.refd
+0000dfd0: 6f6d 6169 6e58 0200 0000 7079 7204 0900  omainX....pyr...
+0000dfe0: 0068 2c5d 682b 5d55 0b72 6566 6578 706c  .h,]h+]U.refexpl
+0000dff0: 6963 6974 8968 295d 682a 5d68 2f5d 6845  icit.h)]h*]h/]hE
+0000e000: 6846 6847 6a24 0700 0068 486a 2107 0000  hFhGj$...hHj!...
+0000e010: 7568 314b 1968 335d 7205 0900 0068 4a29  uh1K.h3]r....hJ)
+0000e020: 8172 0609 0000 7d72 0709 0000 2868 1e6a  .r....}r....(h.j
+0000e030: 0209 0000 6827 7d72 0809 0000 2868 295d  ....h'}r....(h)]
+0000e040: 682a 5d72 0909 0000 2868 4f6a 0409 0000  h*]r....(hOj....
+0000e050: 5808 0000 0070 792d 636c 6173 7372 0a09  X....py-classr..
+0000e060: 0000 6568 2b5d 682c 5d68 2f5d 7568 1f6a  ..eh+]h,]h/]uh.j
+0000e070: 0009 0000 6833 5d72 0b09 0000 6852 5817  ....h3]r....hRX.
+0000e080: 0000 006c 7371 6669 742e 7363 6970 795f  ...lsqfit.scipy_
+0000e090: 6d75 6c74 696d 696e 6578 720c 0900 0085  multiminexr.....
+0000e0a0: 8172 0d09 0000 7d72 0e09 0000 2868 1e55  .r....}r....(h.U
+0000e0b0: 0068 1f6a 0609 0000 7562 6168 2568 5675  .h.j....ubah%hVu
+0000e0c0: 6261 7562 6852 5827 0000 0020 6f62 6a65  baubhRX'... obje
+0000e0d0: 6374 7320 6861 7665 2074 6865 2066 6f6c  cts have the fol
+0000e0e0: 6c6f 7769 6e67 2061 7474 7269 6275 7465  lowing attribute
+0000e0f0: 732e 720f 0900 0085 8172 1009 0000 7d72  s.r......r....}r
+0000e100: 1109 0000 2868 1e58 2700 0000 206f 626a  ....(h.X'... obj
+0000e110: 6563 7473 2068 6176 6520 7468 6520 666f  ects have the fo
+0000e120: 6c6c 6f77 696e 6720 6174 7472 6962 7574  llowing attribut
+0000e130: 6573 2e68 234e 6831 4e68 3268 0268 1f6a  es.h#Nh1Nh2h.h.j
+0000e140: fb08 0000 7562 6575 6268 cf29 8172 1209  ....ubeubh.).r..
+0000e150: 0000 7d72 1309 0000 2868 1e55 0068 1f6a  ..}r....(h.U.h.j
+0000e160: 6f07 0000 6823 6a76 0700 0068 2568 d268  o...h#jv...h%h.h
+0000e170: 277d 7214 0900 0028 682c 5d68 2b5d 6829  '}r....(h,]h+]h)
+0000e180: 5d68 2a5d 682f 5d55 0765 6e74 7269 6573  ]h*]h/]U.entries
+0000e190: 5d72 1509 0000 2868 d558 2500 0000 7820  ]r....(h.X%...x 
+0000e1a0: 286c 7371 6669 742e 7363 6970 795f 6d75  (lsqfit.scipy_mu
+0000e1b0: 6c74 696d 696e 6578 2061 7474 7269 6275  ltiminex attribu
+0000e1c0: 7465 2968 0a55 004e 7472 1609 0000 6175  te)h.U.Ntr....au
+0000e1d0: 6831 4e68 3268 0268 335d 7562 68d7 2981  h1Nh2h.h3]ubh.).
+0000e1e0: 7217 0900 007d 7218 0900 0028 681e 5500  r....}r....(h.U.
+0000e1f0: 681f 6a6f 0700 0068 236a 7607 0000 6825  h.jo...h#jv...h%
+0000e200: 68da 6827 7d72 1909 0000 2868 dc89 68dd  h.h'}r....(h..h.
+0000e210: 5802 0000 0070 7968 2c5d 682b 5d68 295d  X....pyh,]h+]h)]
+0000e220: 682a 5d68 2f5d 68df 5809 0000 0061 7474  h*]h/]h.X....att
+0000e230: 7269 6275 7465 721a 0900 0068 e16a 1a09  ributer....h.j..
+0000e240: 0000 7568 314e 6832 6802 6833 5d72 1b09  ..uh1Nh2h.h3]r..
+0000e250: 0000 2868 e329 8172 1c09 0000 7d72 1d09  ..(h.).r....}r..
+0000e260: 0000 2868 1e58 0100 0000 7868 1f6a 1709  ..(h.X....xh.j..
+0000e270: 0000 6823 6a76 0700 0068 2568 e768 277d  ..h#jv...h%h.h'}
+0000e280: 721e 0900 0028 682c 5d72 1f09 0000 680a  r....(h,]r....h.
+0000e290: 6168 ea6a 2107 0000 682b 5d68 295d 682a  ah.j!...h+]h)]h*
+0000e2a0: 5d68 2f5d 7220 0900 0068 0a61 68f0 5812  ]h/]r ...h.ah.X.
+0000e2b0: 0000 0073 6369 7079 5f6d 756c 7469 6d69  ...scipy_multimi
+0000e2c0: 6e65 782e 7868 f26a 2407 0000 68f3 8975  nex.xh.j$...h..u
+0000e2d0: 6831 4b1e 6832 6802 6833 5d72 2109 0000  h1K.h2h.h3]r!...
+0000e2e0: 6a09 0100 0029 8172 2209 0000 7d72 2309  j....).r"...}r#.
+0000e2f0: 0000 2868 1e58 0100 0000 7868 1f6a 1c09  ..(h.X....xh.j..
+0000e300: 0000 6823 6a76 0700 0068 256a 0c01 0000  ..h#jv...h%j....
+0000e310: 6827 7d72 2409 0000 2868 fa68 fb68 2c5d  h'}r$...(h.h.h,]
+0000e320: 682b 5d68 295d 682a 5d68 2f5d 7568 314b  h+]h)]h*]h/]uh1K
+0000e330: 1e68 3268 0268 335d 7225 0900 0068 5258  .h2h.h3]r%...hRX
+0000e340: 0100 0000 7885 8172 2609 0000 7d72 2709  ....x..r&...}r'.
+0000e350: 0000 2868 1e55 0068 234e 6831 4e68 3268  ..(h.U.h#Nh1Nh2h
+0000e360: 0268 1f6a 2209 0000 7562 6175 6261 7562  .h.j"...ubaubaub
+0000e370: 6a50 0100 0029 8172 2809 0000 7d72 2909  jP...).r(...}r).
+0000e380: 0000 2868 1e55 0068 1f6a 1709 0000 6823  ..(h.U.h.j....h#
+0000e390: 6a76 0700 0068 256a 5301 0000 6827 7d72  jv...h%jS...h'}r
+0000e3a0: 2a09 0000 2868 295d 682a 5d68 2b5d 682c  *...(h)]h*]h+]h,
+0000e3b0: 5d68 2f5d 7568 314b 1e68 3268 0268 335d  ]h/]uh1K.h2h.h3]
+0000e3c0: 722b 0900 0068 9729 8172 2c09 0000 7d72  r+...h.).r,...}r
+0000e3d0: 2d09 0000 2868 1e58 2300 0000 2a61 7272  -...(h.X#...*arr
+0000e3e0: 6179 2a20 2d2d 204c 6f63 6174 696f 6e20  ay* -- Location 
+0000e3f0: 6f66 2074 6865 206d 696e 696d 756d 2e68  of the minimum.h
+0000e400: 1f6a 2809 0000 6823 6a76 0700 0068 2568  .j(...h#jv...h%h
+0000e410: 9a68 277d 722e 0900 0028 6829 5d68 2a5d  .h'}r....(h)]h*]
+0000e420: 682b 5d68 2c5d 682f 5d75 6831 4b1d 6832  h+]h,]h/]uh1K.h2
+0000e430: 6802 6833 5d72 2f09 0000 286a eb04 0000  h.h3]r/...(j....
+0000e440: 2981 7230 0900 007d 7231 0900 0028 681e  ).r0...}r1...(h.
+0000e450: 5807 0000 002a 6172 7261 792a 6827 7d72  X....*array*h'}r
+0000e460: 3209 0000 2868 295d 682a 5d68 2b5d 682c  2...(h)]h*]h+]h,
+0000e470: 5d68 2f5d 7568 1f6a 2c09 0000 6833 5d72  ]h/]uh.j,...h3]r
+0000e480: 3309 0000 6852 5805 0000 0061 7272 6179  3...hRX....array
+0000e490: 7234 0900 0085 8172 3509 0000 7d72 3609  r4.....r5...}r6.
+0000e4a0: 0000 2868 1e55 0068 1f6a 3009 0000 7562  ..(h.U.h.j0...ub
+0000e4b0: 6168 256a f304 0000 7562 6852 581d 0000  ah%j....ubhRX...
+0000e4c0: 0020 e280 9320 4c6f 6361 7469 6f6e 206f  . ... Location o
+0000e4d0: 6620 7468 6520 6d69 6e69 6d75 6d2e 7237  f the minimum.r7
+0000e4e0: 0900 0085 8172 3809 0000 7d72 3909 0000  .....r8...}r9...
+0000e4f0: 2868 1e58 1c00 0000 202d 2d20 4c6f 6361  (h.X.... -- Loca
+0000e500: 7469 6f6e 206f 6620 7468 6520 6d69 6e69  tion of the mini
+0000e510: 6d75 6d2e 6823 4e68 314e 6832 6802 681f  mum.h#Nh1Nh2h.h.
+0000e520: 6a2c 0900 0075 6265 7562 6175 6265 7562  j,...ubeubaubeub
+0000e530: 68cf 2981 723a 0900 007d 723b 0900 0028  h.).r:...}r;...(
+0000e540: 681e 5500 681f 6a6f 0700 0068 236a 7607  h.U.h.jo...h#jv.
+0000e550: 0000 6825 68d2 6827 7d72 3c09 0000 2868  ..h%h.h'}r<...(h
+0000e560: 2c5d 682b 5d68 295d 682a 5d68 2f5d 5507  ,]h+]h)]h*]h/]U.
+0000e570: 656e 7472 6965 735d 723d 0900 0028 68d5  entries]r=...(h.
+0000e580: 5825 0000 0066 2028 6c73 7166 6974 2e73  X%...f (lsqfit.s
+0000e590: 6369 7079 5f6d 756c 7469 6d69 6e65 7820  cipy_multiminex 
+0000e5a0: 6174 7472 6962 7574 6529 680c 5500 4e74  attribute)h.U.Nt
+0000e5b0: 723e 0900 0061 7568 314e 6832 6802 6833  r>...auh1Nh2h.h3
+0000e5c0: 5d75 6268 d729 8172 3f09 0000 7d72 4009  ]ubh.).r?...}r@.
+0000e5d0: 0000 2868 1e55 0068 1f6a 6f07 0000 6823  ..(h.U.h.jo...h#
+0000e5e0: 6a76 0700 0068 2568 da68 277d 7241 0900  jv...h%h.h'}rA..
+0000e5f0: 0028 68dc 8968 dd58 0200 0000 7079 682c  .(h..h.X....pyh,
+0000e600: 5d68 2b5d 6829 5d68 2a5d 682f 5d68 df58  ]h+]h)]h*]h/]h.X
+0000e610: 0900 0000 6174 7472 6962 7574 6572 4209  ....attributerB.
+0000e620: 0000 68e1 6a42 0900 0075 6831 4e68 3268  ..h.jB...uh1Nh2h
+0000e630: 0268 335d 7243 0900 0028 68e3 2981 7244  .h3]rC...(h.).rD
+0000e640: 0900 007d 7245 0900 0028 681e 5801 0000  ...}rE...(h.X...
+0000e650: 0066 681f 6a3f 0900 0068 236a 7607 0000  .fh.j?...h#jv...
+0000e660: 6825 68e7 6827 7d72 4609 0000 2868 2c5d  h%h.h'}rF...(h,]
+0000e670: 7247 0900 0068 0c61 68ea 6a21 0700 0068  rG...h.ah.j!...h
+0000e680: 2b5d 6829 5d68 2a5d 682f 5d72 4809 0000  +]h)]h*]h/]rH...
+0000e690: 680c 6168 f058 1200 0000 7363 6970 795f  h.ah.X....scipy_
+0000e6a0: 6d75 6c74 696d 696e 6578 2e66 68f2 6a24  multiminex.fh.j$
+0000e6b0: 0700 0068 f389 7568 314b 2268 3268 0268  ...h..uh1K"h2h.h
+0000e6c0: 335d 7249 0900 006a 0901 0000 2981 724a  3]rI...j....).rJ
+0000e6d0: 0900 007d 724b 0900 0028 681e 5801 0000  ...}rK...(h.X...
+0000e6e0: 0066 681f 6a44 0900 0068 236a 7607 0000  .fh.jD...h#jv...
+0000e6f0: 6825 6a0c 0100 0068 277d 724c 0900 0028  h%j....h'}rL...(
+0000e700: 68fa 68fb 682c 5d68 2b5d 6829 5d68 2a5d  h.h.h,]h+]h)]h*]
+0000e710: 682f 5d75 6831 4b22 6832 6802 6833 5d72  h/]uh1K"h2h.h3]r
+0000e720: 4d09 0000 6852 5801 0000 0066 8581 724e  M...hRX....f..rN
+0000e730: 0900 007d 724f 0900 0028 681e 5500 6823  ...}rO...(h.U.h#
+0000e740: 4e68 314e 6832 6802 681f 6a4a 0900 0075  Nh1Nh2h.h.jJ...u
+0000e750: 6261 7562 6175 626a 5001 0000 2981 7250  baubaubjP...).rP
+0000e760: 0900 007d 7251 0900 0028 681e 5500 681f  ...}rQ...(h.U.h.
+0000e770: 6a3f 0900 0068 236a 7607 0000 6825 6a53  j?...h#jv...h%jS
+0000e780: 0100 0068 277d 7252 0900 0028 6829 5d68  ...h'}rR...(h)]h
+0000e790: 2a5d 682b 5d68 2c5d 682f 5d75 6831 4b22  *]h+]h,]h/]uh1K"
+0000e7a0: 6832 6802 6833 5d72 5309 0000 6897 2981  h2h.h3]rS...h.).
+0000e7b0: 7254 0900 007d 7255 0900 0028 681e 5835  rT...}rU...(h.X5
+0000e7c0: 0000 002a 666c 6f61 742a 202d 2d20 5661  ...*float* -- Va
+0000e7d0: 6c75 6520 6f66 2066 756e 6374 696f 6e20  lue of function 
+0000e7e0: 6060 6628 7829 6060 2061 7420 7468 6520  ``f(x)`` at the 
+0000e7f0: 6d69 6e69 6d75 6d2e 681f 6a50 0900 0068  minimum.h.jP...h
+0000e800: 236a 7607 0000 6825 689a 6827 7d72 5609  #jv...h%h.h'}rV.
+0000e810: 0000 2868 295d 682a 5d68 2b5d 682c 5d68  ..(h)]h*]h+]h,]h
+0000e820: 2f5d 7568 314b 2168 3268 0268 335d 7257  /]uh1K!h2h.h3]rW
+0000e830: 0900 0028 6aeb 0400 0029 8172 5809 0000  ...(j....).rX...
+0000e840: 7d72 5909 0000 2868 1e58 0700 0000 2a66  }rY...(h.X....*f
+0000e850: 6c6f 6174 2a68 277d 725a 0900 0028 6829  loat*h'}rZ...(h)
+0000e860: 5d68 2a5d 682b 5d68 2c5d 682f 5d75 681f  ]h*]h+]h,]h/]uh.
+0000e870: 6a54 0900 0068 335d 725b 0900 0068 5258  jT...h3]r[...hRX
+0000e880: 0500 0000 666c 6f61 7472 5c09 0000 8581  ....floatr\.....
+0000e890: 725d 0900 007d 725e 0900 0028 681e 5500  r]...}r^...(h.U.
+0000e8a0: 681f 6a58 0900 0075 6261 6825 6af3 0400  h.jX...ubah%j...
+0000e8b0: 0075 6268 5258 1700 0000 20e2 8093 2056  .ubhRX.... ... V
+0000e8c0: 616c 7565 206f 6620 6675 6e63 7469 6f6e  alue of function
+0000e8d0: 2072 5f09 0000 8581 7260 0900 007d 7261   r_.....r`...}ra
+0000e8e0: 0900 0028 681e 5816 0000 0020 2d2d 2056  ...(h.X.... -- V
+0000e8f0: 616c 7565 206f 6620 6675 6e63 7469 6f6e  alue of function
+0000e900: 2068 234e 6831 4e68 3268 0268 1f6a 5409   h#Nh1Nh2h.h.jT.
+0000e910: 0000 7562 684a 2981 7262 0900 007d 7263  ..ubhJ).rb...}rc
+0000e920: 0900 0028 681e 5808 0000 0060 6066 2878  ...(h.X....``f(x
+0000e930: 2960 6068 277d 7264 0900 0028 6829 5d68  )``h'}rd...(h)]h
+0000e940: 2a5d 682b 5d68 2c5d 682f 5d75 681f 6a54  *]h+]h,]h/]uh.jT
+0000e950: 0900 0068 335d 7265 0900 0068 5258 0400  ...h3]re...hRX..
+0000e960: 0000 6628 7829 7266 0900 0085 8172 6709  ..f(x)rf.....rg.
+0000e970: 0000 7d72 6809 0000 2868 1e55 0068 1f6a  ..}rh...(h.U.h.j
+0000e980: 6209 0000 7562 6168 2568 5675 6268 5258  b...ubah%hVubhRX
+0000e990: 1000 0000 2061 7420 7468 6520 6d69 6e69  .... at the mini
+0000e9a0: 6d75 6d2e 7269 0900 0085 8172 6a09 0000  mum.ri.....rj...
+0000e9b0: 7d72 6b09 0000 2868 1e58 1000 0000 2061  }rk...(h.X.... a
+0000e9c0: 7420 7468 6520 6d69 6e69 6d75 6d2e 6823  t the minimum.h#
+0000e9d0: 4e68 314e 6832 6802 681f 6a54 0900 0075  Nh1Nh2h.h.jT...u
+0000e9e0: 6265 7562 6175 6265 7562 68cf 2981 726c  beubaubeubh.).rl
+0000e9f0: 0900 007d 726d 0900 0028 681e 5500 681f  ...}rm...(h.U.h.
+0000ea00: 6a6f 0700 0068 236a 7607 0000 6825 68d2  jo...h#jv...h%h.
+0000ea10: 6827 7d72 6e09 0000 2868 2c5d 682b 5d68  h'}rn...(h,]h+]h
+0000ea20: 295d 682a 5d68 2f5d 5507 656e 7472 6965  )]h*]h/]U.entrie
+0000ea30: 735d 726f 0900 0028 68d5 5827 0000 006e  s]ro...(h.X'...n
+0000ea40: 6974 2028 6c73 7166 6974 2e73 6369 7079  it (lsqfit.scipy
+0000ea50: 5f6d 756c 7469 6d69 6e65 7820 6174 7472  _multiminex attr
+0000ea60: 6962 7574 6529 6816 5500 4e74 7270 0900  ibute)h.U.Ntrp..
+0000ea70: 0061 7568 314e 6832 6802 6833 5d75 6268  .auh1Nh2h.h3]ubh
+0000ea80: d729 8172 7109 0000 7d72 7209 0000 2868  .).rq...}rr...(h
+0000ea90: 1e55 0068 1f6a 6f07 0000 6823 6a76 0700  .U.h.jo...h#jv..
+0000eaa0: 0068 2568 da68 277d 7273 0900 0028 68dc  .h%h.h'}rs...(h.
+0000eab0: 8968 dd58 0200 0000 7079 682c 5d68 2b5d  .h.X....pyh,]h+]
+0000eac0: 6829 5d68 2a5d 682f 5d68 df58 0900 0000  h)]h*]h/]h.X....
+0000ead0: 6174 7472 6962 7574 6572 7409 0000 68e1  attributert...h.
+0000eae0: 6a74 0900 0075 6831 4e68 3268 0268 335d  jt...uh1Nh2h.h3]
+0000eaf0: 7275 0900 0028 68e3 2981 7276 0900 007d  ru...(h.).rv...}
+0000eb00: 7277 0900 0028 681e 5803 0000 006e 6974  rw...(h.X....nit
+0000eb10: 7278 0900 0068 1f6a 7109 0000 6823 6a76  rx...h.jq...h#jv
+0000eb20: 0700 0068 2568 e768 277d 7279 0900 0028  ...h%h.h'}ry...(
+0000eb30: 682c 5d72 7a09 0000 6816 6168 ea6a 2107  h,]rz...h.ah.j!.
+0000eb40: 0000 682b 5d68 295d 682a 5d68 2f5d 727b  ..h+]h)]h*]h/]r{
+0000eb50: 0900 0068 1661 68f0 5814 0000 0073 6369  ...h.ah.X....sci
+0000eb60: 7079 5f6d 756c 7469 6d69 6e65 782e 6e69  py_multiminex.ni
+0000eb70: 7468 f26a 2407 0000 68f3 8975 6831 4b26  th.j$...h..uh1K&
+0000eb80: 6832 6802 6833 5d72 7c09 0000 6a09 0100  h2h.h3]r|...j...
+0000eb90: 0029 8172 7d09 0000 7d72 7e09 0000 2868  .).r}...}r~...(h
+0000eba0: 1e6a 7809 0000 681f 6a76 0900 0068 236a  .jx...h.jv...h#j
+0000ebb0: 7607 0000 6825 6a0c 0100 0068 277d 727f  v...h%j....h'}r.
+0000ebc0: 0900 0028 68fa 68fb 682c 5d68 2b5d 6829  ...(h.h.h,]h+]h)
+0000ebd0: 5d68 2a5d 682f 5d75 6831 4b26 6832 6802  ]h*]h/]uh1K&h2h.
+0000ebe0: 6833 5d72 8009 0000 6852 5803 0000 006e  h3]r....hRX....n
+0000ebf0: 6974 7281 0900 0085 8172 8209 0000 7d72  itr......r....}r
+0000ec00: 8309 0000 2868 1e55 0068 234e 6831 4e68  ....(h.U.h#Nh1Nh
+0000ec10: 3268 0268 1f6a 7d09 0000 7562 6175 6261  2h.h.j}...ubauba
+0000ec20: 7562 6a50 0100 0029 8172 8409 0000 7d72  ubjP...).r....}r
+0000ec30: 8509 0000 2868 1e55 0068 1f6a 7109 0000  ....(h.U.h.jq...
+0000ec40: 6823 6a76 0700 0068 256a 5301 0000 6827  h#jv...h%jS...h'
+0000ec50: 7d72 8609 0000 2868 295d 682a 5d68 2b5d  }r....(h)]h*]h+]
+0000ec60: 682c 5d68 2f5d 7568 314b 2668 3268 0268  h,]h/]uh1K&h2h.h
+0000ec70: 335d 7287 0900 0068 9729 8172 8809 0000  3]r....h.).r....
+0000ec80: 7d72 8909 0000 2868 1e58 3b00 0000 2a69  }r....(h.X;...*i
+0000ec90: 6e74 2a20 2d2d 204e 756d 6265 7220 6f66  nt* -- Number of
+0000eca0: 2069 7465 7261 7469 6f6e 7320 7265 7175   iterations requ
+0000ecb0: 6972 6564 2074 6f20 6669 6e64 2074 6865  ired to find the
+0000ecc0: 206d 696e 696d 756d 2e68 1f6a 8409 0000   minimum.h.j....
+0000ecd0: 6823 6a76 0700 0068 2568 9a68 277d 728a  h#jv...h%h.h'}r.
+0000ece0: 0900 0028 6829 5d68 2a5d 682b 5d68 2c5d  ...(h)]h*]h+]h,]
+0000ecf0: 682f 5d75 6831 4b25 6832 6802 6833 5d72  h/]uh1K%h2h.h3]r
+0000ed00: 8b09 0000 286a eb04 0000 2981 728c 0900  ....(j....).r...
+0000ed10: 007d 728d 0900 0028 681e 5805 0000 002a  .}r....(h.X....*
+0000ed20: 696e 742a 6827 7d72 8e09 0000 2868 295d  int*h'}r....(h)]
+0000ed30: 682a 5d68 2b5d 682c 5d68 2f5d 7568 1f6a  h*]h+]h,]h/]uh.j
+0000ed40: 8809 0000 6833 5d72 8f09 0000 6852 5803  ....h3]r....hRX.
+0000ed50: 0000 0069 6e74 7290 0900 0085 8172 9109  ...intr......r..
+0000ed60: 0000 7d72 9209 0000 2868 1e55 0068 1f6a  ..}r....(h.U.h.j
+0000ed70: 8c09 0000 7562 6168 256a f304 0000 7562  ....ubah%j....ub
+0000ed80: 6852 5837 0000 0020 e280 9320 4e75 6d62  hRX7... ... Numb
+0000ed90: 6572 206f 6620 6974 6572 6174 696f 6e73  er of iterations
+0000eda0: 2072 6571 7569 7265 6420 746f 2066 696e   required to fin
+0000edb0: 6420 7468 6520 6d69 6e69 6d75 6d2e 7293  d the minimum.r.
+0000edc0: 0900 0085 8172 9409 0000 7d72 9509 0000  .....r....}r....
+0000edd0: 2868 1e58 3600 0000 202d 2d20 4e75 6d62  (h.X6... -- Numb
+0000ede0: 6572 206f 6620 6974 6572 6174 696f 6e73  er of iterations
+0000edf0: 2072 6571 7569 7265 6420 746f 2066 696e   required to fin
+0000ee00: 6420 7468 6520 6d69 6e69 6d75 6d2e 6823  d the minimum.h#
+0000ee10: 4e68 314e 6832 6802 681f 6a88 0900 0075  Nh1Nh2h.h.j....u
+0000ee20: 6265 7562 6175 6265 7562 68cf 2981 7296  beubaubeubh.).r.
+0000ee30: 0900 007d 7297 0900 0028 681e 5500 681f  ...}r....(h.U.h.
+0000ee40: 6a6f 0700 0068 236a 7607 0000 6825 68d2  jo...h#jv...h%h.
+0000ee50: 6827 7d72 9809 0000 2868 2c5d 682b 5d68  h'}r....(h,]h+]h
+0000ee60: 295d 682a 5d68 2f5d 5507 656e 7472 6965  )]h*]h/]U.entrie
+0000ee70: 735d 7299 0900 0028 68d5 5829 0000 0065  s]r....(h.X)...e
+0000ee80: 7272 6f72 2028 6c73 7166 6974 2e73 6369  rror (lsqfit.sci
+0000ee90: 7079 5f6d 756c 7469 6d69 6e65 7820 6174  py_multiminex at
+0000eea0: 7472 6962 7574 6529 6817 5500 4e74 729a  tribute)h.U.Ntr.
+0000eeb0: 0900 0061 7568 314e 6832 6802 6833 5d75  ...auh1Nh2h.h3]u
+0000eec0: 6268 d729 8172 9b09 0000 7d72 9c09 0000  bh.).r....}r....
+0000eed0: 2868 1e55 0068 1f6a 6f07 0000 6823 6a76  (h.U.h.jo...h#jv
+0000eee0: 0700 0068 2568 da68 277d 729d 0900 0028  ...h%h.h'}r....(
+0000eef0: 68dc 8968 dd58 0200 0000 7079 682c 5d68  h..h.X....pyh,]h
+0000ef00: 2b5d 6829 5d68 2a5d 682f 5d68 df58 0900  +]h)]h*]h/]h.X..
+0000ef10: 0000 6174 7472 6962 7574 6572 9e09 0000  ..attributer....
+0000ef20: 68e1 6a9e 0900 0075 6831 4e68 3268 0268  h.j....uh1Nh2h.h
+0000ef30: 335d 729f 0900 0028 68e3 2981 72a0 0900  3]r....(h.).r...
+0000ef40: 007d 72a1 0900 0028 681e 5805 0000 0065  .}r....(h.X....e
+0000ef50: 7272 6f72 72a2 0900 0068 1f6a 9b09 0000  rrorr....h.j....
+0000ef60: 6823 6a76 0700 0068 2568 e768 277d 72a3  h#jv...h%h.h'}r.
+0000ef70: 0900 0028 682c 5d72 a409 0000 6817 6168  ...(h,]r....h.ah
+0000ef80: ea6a 2107 0000 682b 5d68 295d 682a 5d68  .j!...h+]h)]h*]h
+0000ef90: 2f5d 72a5 0900 0068 1761 68f0 5816 0000  /]r....h.ah.X...
+0000efa0: 0073 6369 7079 5f6d 756c 7469 6d69 6e65  .scipy_multimine
+0000efb0: 782e 6572 726f 7268 f26a 2407 0000 68f3  x.errorh.j$...h.
+0000efc0: 8975 6831 4b2a 6832 6802 6833 5d72 a609  .uh1K*h2h.h3]r..
+0000efd0: 0000 6a09 0100 0029 8172 a709 0000 7d72  ..j....).r....}r
+0000efe0: a809 0000 2868 1e6a a209 0000 681f 6aa0  ....(h.j....h.j.
+0000eff0: 0900 0068 236a 7607 0000 6825 6a0c 0100  ...h#jv...h%j...
+0000f000: 0068 277d 72a9 0900 0028 68fa 68fb 682c  .h'}r....(h.h.h,
+0000f010: 5d68 2b5d 6829 5d68 2a5d 682f 5d75 6831  ]h+]h)]h*]h/]uh1
+0000f020: 4b2a 6832 6802 6833 5d72 aa09 0000 6852  K*h2h.h3]r....hR
+0000f030: 5805 0000 0065 7272 6f72 72ab 0900 0085  X....errorr.....
+0000f040: 8172 ac09 0000 7d72 ad09 0000 2868 1e55  .r....}r....(h.U
+0000f050: 0068 234e 6831 4e68 3268 0268 1f6a a709  .h#Nh1Nh2h.h.j..
+0000f060: 0000 7562 6175 6261 7562 6a50 0100 0029  ..ubaubaubjP...)
+0000f070: 8172 ae09 0000 7d72 af09 0000 2868 1e55  .r....}r....(h.U
+0000f080: 0068 1f6a 9b09 0000 6823 6a76 0700 0068  .h.j....h#jv...h
+0000f090: 256a 5301 0000 6827 7d72 b009 0000 2868  %jS...h'}r....(h
+0000f0a0: 295d 682a 5d68 2b5d 682c 5d68 2f5d 7568  )]h*]h+]h,]h/]uh
+0000f0b0: 314b 2a68 3268 0268 335d 72b1 0900 0068  1K*h2h.h3]r....h
+0000f0c0: 9729 8172 b209 0000 7d72 b309 0000 2868  .).r....}r....(h
+0000f0d0: 1e58 4700 0000 2a4e 6f65 206f 7220 7374  .XG...*Noe or st
+0000f0e0: 722a 202d 2d20 6060 4e6f 6e65 6060 2069  r* -- ``None`` i
+0000f0f0: 6620 6669 7420 7375 6363 6573 7366 756c  f fit successful
+0000f100: 3b20 616e 2065 7272 6f72 0a6d 6573 7361  ; an error.messa
+0000f110: 6765 206f 7468 6572 7769 7365 2e68 1f6a  ge otherwise.h.j
+0000f120: ae09 0000 6823 6a76 0700 0068 2568 9a68  ....h#jv...h%h.h
+0000f130: 277d 72b4 0900 0028 6829 5d68 2a5d 682b  '}r....(h)]h*]h+
+0000f140: 5d68 2c5d 682f 5d75 6831 4b29 6832 6802  ]h,]h/]uh1K)h2h.
+0000f150: 6833 5d72 b509 0000 286a eb04 0000 2981  h3]r....(j....).
+0000f160: 72b6 0900 007d 72b7 0900 0028 681e 580c  r....}r....(h.X.
+0000f170: 0000 002a 4e6f 6520 6f72 2073 7472 2a68  ...*Noe or str*h
+0000f180: 277d 72b8 0900 0028 6829 5d68 2a5d 682b  '}r....(h)]h*]h+
+0000f190: 5d68 2c5d 682f 5d75 681f 6ab2 0900 0068  ]h,]h/]uh.j....h
+0000f1a0: 335d 72b9 0900 0068 5258 0a00 0000 4e6f  3]r....hRX....No
+0000f1b0: 6520 6f72 2073 7472 72ba 0900 0085 8172  e or strr......r
+0000f1c0: bb09 0000 7d72 bc09 0000 2868 1e55 0068  ....}r....(h.U.h
+0000f1d0: 1f6a b609 0000 7562 6168 256a f304 0000  .j....ubah%j....
+0000f1e0: 7562 6852 5805 0000 0020 e280 9320 72bd  ubhRX.... ... r.
+0000f1f0: 0900 0085 8172 be09 0000 7d72 bf09 0000  .....r....}r....
+0000f200: 2868 1e58 0400 0000 202d 2d20 6823 4e68  (h.X.... -- h#Nh
+0000f210: 314e 6832 6802 681f 6ab2 0900 0075 6268  1Nh2h.h.j....ubh
+0000f220: 4a29 8172 c009 0000 7d72 c109 0000 2868  J).r....}r....(h
+0000f230: 1e58 0800 0000 6060 4e6f 6e65 6060 6827  .X....``None``h'
+0000f240: 7d72 c209 0000 2868 295d 682a 5d68 2b5d  }r....(h)]h*]h+]
+0000f250: 682c 5d68 2f5d 7568 1f6a b209 0000 6833  h,]h/]uh.j....h3
+0000f260: 5d72 c309 0000 6852 5804 0000 004e 6f6e  ]r....hRX....Non
+0000f270: 6572 c409 0000 8581 72c5 0900 007d 72c6  er......r....}r.
+0000f280: 0900 0028 681e 5500 681f 6ac0 0900 0075  ...(h.U.h.j....u
+0000f290: 6261 6825 6856 7562 6852 582f 0000 0020  bah%hVubhRX/... 
+0000f2a0: 6966 2066 6974 2073 7563 6365 7373 6675  if fit successfu
+0000f2b0: 6c3b 2061 6e20 6572 726f 720a 6d65 7373  l; an error.mess
+0000f2c0: 6167 6520 6f74 6865 7277 6973 652e 72c7  age otherwise.r.
+0000f2d0: 0900 0085 8172 c809 0000 7d72 c909 0000  .....r....}r....
+0000f2e0: 2868 1e58 2f00 0000 2069 6620 6669 7420  (h.X/... if fit 
+0000f2f0: 7375 6363 6573 7366 756c 3b20 616e 2065  successful; an e
+0000f300: 7272 6f72 0a6d 6573 7361 6765 206f 7468  rror.message oth
+0000f310: 6572 7769 7365 2e68 234e 6831 4e68 3268  erwise.h#Nh1Nh2h
+0000f320: 0268 1f6a b209 0000 7562 6575 6261 7562  .h.j....ubeubaub
+0000f330: 6575 6265 7562 6575 6265 7562 6575 6268  eubeubeubeubeubh
+0000f340: 2368 2468 2568 5d68 277d 72ca 0900 0028  #h$h%h]h'}r....(
+0000f350: 6829 5d68 2a5d 682b 5d68 2c5d 682f 5d72  h)]h*]h+]h,]h/]r
+0000f360: cb09 0000 681a 6175 6831 4b06 6832 6802  ....h.auh1K.h2h.
+0000f370: 6833 5d72 cc09 0000 683c 2981 72cd 0900  h3]r....h<).r...
+0000f380: 007d 72ce 0900 0028 681e 5818 0000 003a  .}r....(h.X....:
+0000f390: 636c 6173 733a 6067 7661 722e 4275 6666  class:`gvar.Buff
+0000f3a0: 6572 4469 6374 6072 cf09 0000 681f 681c  erDict`r....h.h.
+0000f3b0: 6823 6824 6825 6840 6827 7d72 d009 0000  h#h$h%h@h'}r....
+0000f3c0: 2855 0772 6566 7479 7065 5805 0000 0063  (U.reftypeX....c
+0000f3d0: 6c61 7373 6842 8968 4358 0f00 0000 6776  lasshB.hCX....gv
+0000f3e0: 6172 2e42 7566 6665 7244 6963 7455 0972  ar.BufferDictU.r
+0000f3f0: 6566 646f 6d61 696e 5802 0000 0070 7972  efdomainX....pyr
+0000f400: d109 0000 682c 5d68 2b5d 550b 7265 6665  ....h,]h+]U.refe
+0000f410: 7870 6c69 6369 7489 6829 5d68 2a5d 682f  xplicit.h)]h*]h/
+0000f420: 5d68 4568 4668 474e 6848 4e75 6831 4b06  ]hEhFhGNhHNuh1K.
+0000f430: 6833 5d72 d209 0000 684a 2981 72d3 0900  h3]r....hJ).r...
+0000f440: 007d 72d4 0900 0028 681e 6acf 0900 0068  .}r....(h.j....h
+0000f450: 277d 72d5 0900 0028 6829 5d68 2a5d 72d6  '}r....(h)]h*]r.
+0000f460: 0900 0028 684f 6ad1 0900 0058 0800 0000  ...(hOj....X....
+0000f470: 7079 2d63 6c61 7373 72d7 0900 0065 682b  py-classr....eh+
+0000f480: 5d68 2c5d 682f 5d75 681f 6acd 0900 0068  ]h,]h/]uh.j....h
+0000f490: 335d 72d8 0900 0068 5258 0f00 0000 6776  3]r....hRX....gv
+0000f4a0: 6172 2e42 7566 6665 7244 6963 7472 d909  ar.BufferDictr..
+0000f4b0: 0000 8581 72da 0900 007d 72db 0900 0028  ....r....}r....(
+0000f4c0: 681e 5500 681f 6ad3 0900 0075 6261 6825  h.U.h.j....ubah%
+0000f4d0: 6856 7562 6175 6261 7562 6875 6871 6860  hVubaubaubhuhqh`
+0000f4e0: 685b 7555 0e70 6172 7365 5f6d 6573 7361  h[uU.parse_messa
+0000f4f0: 6765 7372 dc09 0000 5d72 dd09 0000 6364  gesr....]r....cd
+0000f500: 6f63 7574 696c 732e 6e6f 6465 730a 7379  ocutils.nodes.sy
+0000f510: 7374 656d 5f6d 6573 7361 6765 0a72 de09  stem_message.r..
+0000f520: 0000 2981 72df 0900 007d 72e0 0900 0028  ..).r....}r....(
+0000f530: 681e 5500 6827 7d72 e109 0000 2868 295d  h.U.h'}r....(h)]
+0000f540: 5505 6c65 7665 6c4b 0168 2c5d 682b 5d55  U.levelK.h,]h+]U
+0000f550: 0673 6f75 7263 656a 5901 0000 682a 5d68  .sourcejY...h*]h
+0000f560: 2f5d 5504 6c69 6e65 4b6f 5504 7479 7065  /]U.lineKoU.type
+0000f570: 5504 494e 464f 72e2 0900 0075 681f 6a03  U.INFOr....uh.j.
+0000f580: 0600 0068 335d 72e3 0900 0068 9729 8172  ...h3]r....h.).r
+0000f590: e409 0000 7d72 e509 0000 2868 1e58 3a00  ....}r....(h.X:.
+0000f5a0: 0000 456e 756d 6572 6174 6564 206c 6973  ..Enumerated lis
+0000f5b0: 7420 7374 6172 7420 7661 6c75 6520 6e6f  t start value no
+0000f5c0: 7420 6f72 6469 6e61 6c2d 313a 2022 3022  t ordinal-1: "0"
+0000f5d0: 2028 6f72 6469 6e61 6c20 3029 6827 7d72   (ordinal 0)h'}r
+0000f5e0: e609 0000 2868 295d 682a 5d68 2b5d 682c  ....(h)]h*]h+]h,
+0000f5f0: 5d68 2f5d 7568 1f6a df09 0000 6833 5d72  ]h/]uh.j....h3]r
+0000f600: e709 0000 6852 583e 0000 0045 6e75 6d65  ....hRX>...Enume
+0000f610: 7261 7465 6420 6c69 7374 2073 7461 7274  rated list start
+0000f620: 2076 616c 7565 206e 6f74 206f 7264 696e   value not ordin
+0000f630: 616c 2d31 3a20 e280 9c30 e280 9d20 286f  al-1: ...0... (o
+0000f640: 7264 696e 616c 2030 2972 e809 0000 8581  rdinal 0)r......
+0000f650: 72e9 0900 007d 72ea 0900 0028 681e 5500  r....}r....(h.U.
+0000f660: 681f 6ae4 0900 0075 6261 6825 689a 7562  h.j....ubah%h.ub
+0000f670: 6168 2555 0e73 7973 7465 6d5f 6d65 7373  ah%U.system_mess
+0000f680: 6167 6572 eb09 0000 7562 6155 0e63 7572  ager....ubaU.cur
+0000f690: 7265 6e74 5f73 6f75 7263 6572 ec09 0000  rent_sourcer....
+0000f6a0: 4e55 0a64 6563 6f72 6174 696f 6e72 ed09  NU.decorationr..
+0000f6b0: 0000 4e55 1261 7574 6f66 6f6f 746e 6f74  ..NU.autofootnot
+0000f6c0: 655f 7374 6172 7472 ee09 0000 4b01 5507  e_startr....K.U.
+0000f6d0: 6e61 6d65 6964 7372 ef09 0000 7d72 f009  nameidsr....}r..
+0000f6e0: 0000 2868 0668 0668 0768 0768 0868 0868  ..(h.h.h.h.h.h.h
+0000f6f0: 0968 2e68 0a68 0a68 0b68 8c68 0c68 0c68  .h.h.h.h.h.h.h.h
+0000f700: 0d68 0d68 0e68 0e68 0f68 0f68 1068 1068  .h.h.h.h.h.h.h.h
+0000f710: 1168 1168 1268 1268 1368 1368 146a d106  .h.h.h.h.h.h.j..
+0000f720: 0000 6815 6815 6816 6816 6817 6817 7568  ..h.h.h.h.h.h.uh
+0000f730: 335d 72f1 0900 0068 2161 681e 5500 550b  3]r....h!ah.U.U.
+0000f740: 7472 616e 7366 6f72 6d65 7272 f209 0000  transformerr....
+0000f750: 4e55 0d66 6f6f 746e 6f74 655f 7265 6673  NU.footnote_refs
+0000f760: 72f3 0900 007d 72f4 0900 0055 0872 6566  r....}r....U.ref
+0000f770: 6e61 6d65 7372 f509 0000 7d72 f609 0000  namesr....}r....
+0000f780: 5510 7379 6d62 6f6c 5f66 6f6f 746e 6f74  U.symbol_footnot
+0000f790: 6573 72f7 0900 005d 72f8 0900 0055 1161  esr....]r....U.a
+0000f7a0: 7574 6f66 6f6f 746e 6f74 655f 7265 6673  utofootnote_refs
+0000f7b0: 72f9 0900 005d 72fa 0900 0055 1473 796d  r....]r....U.sym
+0000f7c0: 626f 6c5f 666f 6f74 6e6f 7465 5f72 6566  bol_footnote_ref
+0000f7d0: 7372 fb09 0000 5d72 fc09 0000 5509 6369  sr....]r....U.ci
+0000f7e0: 7461 7469 6f6e 7372 fd09 0000 5d72 fe09  tationsr....]r..
+0000f7f0: 0000 6832 6802 550c 6375 7272 656e 745f  ..h2h.U.current_
+0000f800: 6c69 6e65 72ff 0900 004e 5512 7472 616e  liner....NU.tran
+0000f810: 7366 6f72 6d5f 6d65 7373 6167 6573 7200  sform_messagesr.
+0000f820: 0a00 005d 7201 0a00 0055 0872 6570 6f72  ...]r....U.repor
+0000f830: 7465 7272 020a 0000 4e55 0869 645f 7374  terr....NU.id_st
+0000f840: 6172 7472 030a 0000 4b01 550d 6175 746f  artr....K.U.auto
+0000f850: 666f 6f74 6e6f 7465 7372 040a 0000 5d72  footnotesr....]r
+0000f860: 050a 0000 550d 6369 7461 7469 6f6e 5f72  ....U.citation_r
+0000f870: 6566 7372 060a 0000 7d72 070a 0000 5510  efsr....}r....U.
+0000f880: 696e 6469 7265 6374 5f74 6172 6765 7473  indirect_targets
+0000f890: 7208 0a00 005d 7209 0a00 0055 0873 6574  r....]r....U.set
+0000f8a0: 7469 6e67 7372 0a0a 0000 2863 646f 6375  tingsr....(cdocu
+0000f8b0: 7469 6c73 2e66 726f 6e74 656e 640a 5661  tils.frontend.Va
+0000f8c0: 6c75 6573 0a72 0b0a 0000 6f72 0c0a 0000  lues.r....or....
+0000f8d0: 7d72 0d0a 0000 2855 1266 6f6f 746e 6f74  }r....(U.footnot
+0000f8e0: 655f 6261 636b 6c69 6e6b 7372 0e0a 0000  e_backlinksr....
+0000f8f0: 4b01 5513 7265 636f 7264 5f64 6570 656e  K.U.record_depen
+0000f900: 6465 6e63 6965 7372 0f0a 0000 4e55 0d6c  denciesr....NU.l
+0000f910: 616e 6775 6167 655f 636f 6465 7210 0a00  anguage_coder...
+0000f920: 0055 0265 6e72 110a 0000 5509 7472 6163  .U.enr....U.trac
+0000f930: 6562 6163 6b72 120a 0000 8855 0e70 6570  ebackr.....U.pep
+0000f940: 5f72 6566 6572 656e 6365 7372 130a 0000  _referencesr....
+0000f950: 4e55 0e73 7472 6970 5f63 6f6d 6d65 6e74  NU.strip_comment
+0000f960: 7372 140a 0000 4e55 0d74 6f63 5f62 6163  sr....NU.toc_bac
+0000f970: 6b6c 696e 6b73 7215 0a00 0055 0565 6e74  klinksr....U.ent
+0000f980: 7279 7216 0a00 0055 0c72 6663 5f62 6173  ryr....U.rfc_bas
+0000f990: 655f 7572 6c72 170a 0000 551c 6874 7470  e_urlr....U.http
+0000f9a0: 733a 2f2f 746f 6f6c 732e 6965 7466 2e6f  s://tools.ietf.o
+0000f9b0: 7267 2f68 746d 6c2f 7218 0a00 0055 0964  rg/html/r....U.d
+0000f9c0: 6174 6573 7461 6d70 7219 0a00 004e 550c  atestampr....NU.
+0000f9d0: 7265 706f 7274 5f6c 6576 656c 721a 0a00  report_levelr...
+0000f9e0: 004b 0255 1373 6d61 7274 7175 6f74 6573  .K.U.smartquotes
+0000f9f0: 5f6c 6f63 616c 6573 721b 0a00 005d 721c  _localesr....]r.
+0000fa00: 0a00 0055 0c5f 6465 7374 696e 6174 696f  ...U._destinatio
+0000fa10: 6e72 1d0a 0000 4e55 0a68 616c 745f 6c65  nr....NU.halt_le
+0000fa20: 7665 6c72 1e0a 0000 4b05 550d 7374 7269  velr....K.U.stri
+0000fa30: 705f 636c 6173 7365 7372 1f0a 0000 4e68  p_classesr....Nh
+0000fa40: 394e 551c 6572 726f 725f 656e 636f 6469  9NU.error_encodi
+0000fa50: 6e67 5f65 7272 6f72 5f68 616e 646c 6572  ng_error_handler
+0000fa60: 7220 0a00 0055 1062 6163 6b73 6c61 7368  r ...U.backslash
+0000fa70: 7265 706c 6163 6572 210a 0000 5505 6465  replacer!...U.de
+0000fa80: 6275 6772 220a 0000 4e55 1065 6d62 6564  bugr"...NU.embed
+0000fa90: 5f73 7479 6c65 7368 6565 7472 230a 0000  _stylesheetr#...
+0000faa0: 8955 1d6f 7574 7075 745f 656e 636f 6469  .U.output_encodi
+0000fab0: 6e67 5f65 7272 6f72 5f68 616e 646c 6572  ng_error_handler
+0000fac0: 7224 0a00 0055 0673 7472 6963 7472 250a  r$...U.strictr%.
+0000fad0: 0000 550d 7365 6374 6e75 6d5f 7866 6f72  ..U.sectnum_xfor
+0000fae0: 6d72 260a 0000 4b01 550f 6475 6d70 5f74  mr&...K.U.dump_t
+0000faf0: 7261 6e73 666f 726d 7372 270a 0000 4e55  ransformsr'...NU
+0000fb00: 0d64 6f63 696e 666f 5f78 666f 726d 7228  .docinfo_xformr(
+0000fb10: 0a00 004b 0155 0e77 6172 6e69 6e67 5f73  ...K.U.warning_s
+0000fb20: 7472 6561 6d72 290a 0000 4e55 1570 6570  treamr)...NU.pep
+0000fb30: 5f66 696c 655f 7572 6c5f 7465 6d70 6c61  _file_url_templa
+0000fb40: 7465 722a 0a00 0055 0870 6570 2d25 3034  ter*...U.pep-%04
+0000fb50: 6472 2b0a 0000 5511 6578 6974 5f73 7461  dr+...U.exit_sta
+0000fb60: 7475 735f 6c65 7665 6c72 2c0a 0000 4b05  tus_levelr,...K.
+0000fb70: 5506 636f 6e66 6967 722d 0a00 004e 550e  U.configr-...NU.
+0000fb80: 7374 7269 6374 5f76 6973 6974 6f72 722e  strict_visitorr.
+0000fb90: 0a00 004e 5515 636c 6f61 6b5f 656d 6169  ...NU.cloak_emai
+0000fba0: 6c5f 6164 6472 6573 7365 7372 2f0a 0000  l_addressesr/...
+0000fbb0: 8855 1d74 7269 6d5f 666f 6f74 6e6f 7465  .U.trim_footnote
+0000fbc0: 5f72 6566 6572 656e 6365 5f73 7061 6365  _reference_space
+0000fbd0: 7230 0a00 0089 5503 656e 7672 310a 0000  r0....U.envr1...
+0000fbe0: 4e55 0f64 756d 705f 7073 6575 646f 5f78  NU.dump_pseudo_x
+0000fbf0: 6d6c 7232 0a00 004e 5510 6578 706f 7365  mlr2...NU.expose
+0000fc00: 5f69 6e74 6572 6e61 6c73 7233 0a00 004e  _internalsr3...N
+0000fc10: 5512 7365 6374 7375 6274 6974 6c65 5f78  U.sectsubtitle_x
+0000fc20: 666f 726d 7234 0a00 0089 550b 736f 7572  formr4....U.sour
+0000fc30: 6365 5f6c 696e 6b72 350a 0000 4e55 0e72  ce_linkr5...NU.r
+0000fc40: 6663 5f72 6566 6572 656e 6365 7372 360a  fc_referencesr6.
+0000fc50: 0000 4e55 0f6f 7574 7075 745f 656e 636f  ..NU.output_enco
+0000fc60: 6469 6e67 7237 0a00 0055 0575 7466 2d38  dingr7...U.utf-8
+0000fc70: 7238 0a00 0055 0a73 6f75 7263 655f 7572  r8...U.source_ur
+0000fc80: 6c72 390a 0000 4e55 0e69 6e70 7574 5f65  lr9...NU.input_e
+0000fc90: 6e63 6f64 696e 6772 3a0a 0000 5509 7574  ncodingr:...U.ut
+0000fca0: 662d 382d 7369 6772 3b0a 0000 550f 5f64  f-8-sigr;...U._d
+0000fcb0: 6973 6162 6c65 5f63 6f6e 6669 6772 3c0a  isable_configr<.
+0000fcc0: 0000 4e55 0969 645f 7072 6566 6978 723d  ..NU.id_prefixr=
+0000fcd0: 0a00 0055 0055 1d63 6861 7261 6374 6572  ...U.U.character
+0000fce0: 5f6c 6576 656c 5f69 6e6c 696e 655f 6d61  _level_inline_ma
+0000fcf0: 726b 7570 723e 0a00 0089 5509 7461 625f  rkupr>....U.tab_
+0000fd00: 7769 6474 6872 3f0a 0000 4b08 550e 6572  widthr?...K.U.er
+0000fd10: 726f 725f 656e 636f 6469 6e67 7240 0a00  ror_encodingr@..
+0000fd20: 0055 0555 5446 2d38 7241 0a00 0055 075f  .U.UTF-8rA...U._
+0000fd30: 736f 7572 6365 7242 0a00 0068 2455 0f67  sourcerB...h$U.g
+0000fd40: 6574 7465 7874 5f63 6f6d 7061 6374 7243  ettext_compactrC
+0000fd50: 0a00 0088 5509 6765 6e65 7261 746f 7272  ....U.generatorr
+0000fd60: 440a 0000 4e55 0e64 756d 705f 696e 7465  D...NU.dump_inte
+0000fd70: 726e 616c 7372 450a 0000 4e55 0c73 6d61  rnalsrE...NU.sma
+0000fd80: 7274 5f71 756f 7465 7372 460a 0000 8855  rt_quotesrF....U
+0000fd90: 0c70 6570 5f62 6173 655f 7572 6c72 470a  .pep_base_urlrG.
+0000fda0: 0000 5520 6874 7470 733a 2f2f 7777 772e  ..U https://www.
+0000fdb0: 7079 7468 6f6e 2e6f 7267 2f64 6576 2f70  python.org/dev/p
+0000fdc0: 6570 732f 7248 0a00 0055 1073 796e 7461  eps/rH...U.synta
+0000fdd0: 785f 6869 6768 6c69 6768 7472 490a 0000  x_highlightrI...
+0000fde0: 5504 6c6f 6e67 724a 0a00 0055 1c69 6e70  U.longrJ...U.inp
+0000fdf0: 7574 5f65 6e63 6f64 696e 675f 6572 726f  ut_encoding_erro
+0000fe00: 725f 6861 6e64 6c65 7272 4b0a 0000 6a25  r_handlerrK...j%
+0000fe10: 0a00 0055 0e61 7574 6f5f 6964 5f70 7265  ...U.auto_id_pre
+0000fe20: 6669 7872 4c0a 0000 5502 6964 724d 0a00  fixrL...U.idrM..
+0000fe30: 0055 0e64 6f63 7469 746c 655f 7866 6f72  .U.doctitle_xfor
+0000fe40: 6d72 4e0a 0000 8955 1b73 7472 6970 5f65  mrN....U.strip_e
+0000fe50: 6c65 6d65 6e74 735f 7769 7468 5f63 6c61  lements_with_cla
+0000fe60: 7373 6573 724f 0a00 004e 550d 5f63 6f6e  ssesrO...NU._con
+0000fe70: 6669 675f 6669 6c65 7372 500a 0000 5d55  fig_filesrP...]U
+0000fe80: 1666 696c 655f 696e 7365 7274 696f 6e5f  .file_insertion_
+0000fe90: 656e 6162 6c65 6472 510a 0000 8855 0b72  enabledrQ....U.r
+0000fea0: 6177 5f65 6e61 626c 6564 7252 0a00 004b  aw_enabledrR...K
+0000feb0: 0155 0d64 756d 705f 7365 7474 696e 6773  .U.dump_settings
+0000fec0: 7253 0a00 004e 7562 5515 7379 6d62 6f6c  rS...NubU.symbol
+0000fed0: 5f66 6f6f 746e 6f74 655f 7374 6172 7472  _footnote_startr
+0000fee0: 540a 0000 4b00 682c 7d72 550a 0000 2868  T...K.h,}rU...(h
+0000fef0: 066a 2b05 0000 6807 6a1b 0700 0068 086a  .j+...h.j....h.j
+0000ff00: 5505 0000 680c 6a44 0900 0068 0a6a 1c09  U...h.jD...h.j..
+0000ff10: 0000 688c 6888 6816 6a76 0900 0068 0d6a  ..h.h.h.jv...h.j
+0000ff20: b905 0000 680e 6ae3 0500 0068 0f6a 8705  ....h.j....h.j..
+0000ff30: 0000 6810 6aa4 0600 0068 116a 0105 0000  ..h.j....h.j....
+0000ff40: 682e 6821 6812 68e4 6813 6a70 0600 006a  h.h!h.h.h.jp...j
+0000ff50: d106 0000 6acd 0600 0068 156a d704 0000  ....j....h.j....
+0000ff60: 6817 6aa0 0900 0075 5512 7375 6273 7469  h.j....uU.substi
+0000ff70: 7475 7469 6f6e 5f6e 616d 6573 7256 0a00  tution_namesrV..
+0000ff80: 007d 7257 0a00 0028 580a 0000 0062 7566  .}rW...(X....buf
+0000ff90: 6665 7264 6963 7468 1a68 7568 7558 0400  ferdicth.huhuX..
+0000ffa0: 0000 6776 6172 6860 7568 2568 3268 277d  ..gvarh`uh%h2h'}
+0000ffb0: 7258 0a00 0028 6829 5d68 2c5d 682b 5d55  rX...(h)]h,]h+]U
+0000ffc0: 0673 6f75 7263 6568 2468 2a5d 682f 5d75  .sourceh$h*]h/]u
+0000ffd0: 5509 666f 6f74 6e6f 7465 7372 590a 0000  U.footnotesrY...
+0000ffe0: 5d72 5a0a 0000 5506 7265 6669 6473 725b  ]rZ...U.refidsr[
+0000fff0: 0a00 007d 725c 0a00 0075 622e            ...}r\...ub.
```

### Comparing `lsqfit-9.4/doc/html/.doctrees/overview.doctree` & `lsqfit-9.5/doc/html/.doctrees/overview.doctree`

 * *Files identical despite different names*

### Comparing `lsqfit-9.4/doc/html/testing.html` & `lsqfit-9.5/doc/html/testing.html`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 <!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Transitional//EN"
   "http://www.w3.org/TR/xhtml1/DTD/xhtml1-transitional.dtd">
 
 <html xmlns="http://www.w3.org/1999/xhtml">
   <head>
     <meta http-equiv="X-UA-Compatible" content="IE=Edge" />
     <meta http-equiv="Content-Type" content="text/html; charset=utf-8" />
-    <title>Non-Gaussian Behavior; Testing Fits &#8212; lsqfit 9.4 documentation</title>
+    <title>Non-Gaussian Behavior; Testing Fits &#8212; lsqfit 9.5 documentation</title>
     <link rel="stylesheet" href="_static/pyramid.css" type="text/css" />
     <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
     <script type="text/javascript" src="_static/documentation_options.js"></script>
     <script type="text/javascript" src="_static/jquery.js"></script>
     <script type="text/javascript" src="_static/underscore.js"></script>
     <script type="text/javascript" src="_static/doctools.js"></script>
     <link rel="index" title="Index" href="genindex.html" />
@@ -36,15 +36,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="case-extrapolation.html" title="Case Study: Simple Extrapolation"
              accesskey="N">next</a> |</li>
         <li class="right" >
           <a href="overview.html" title="Overview and Tutorial"
              accesskey="P">previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">lsqfit 9.4 documentation</a> &#187;</li> 
+        <li class="nav-item nav-item-0"><a href="index.html">lsqfit 9.5 documentation</a> &#187;</li> 
       </ul>
     </div>  
 
     <div class="document">
       <div class="documentwrapper">
         <div class="bodywrapper">
           <div class="body" role="main">
@@ -823,15 +823,15 @@
              >modules</a> |</li>
         <li class="right" >
           <a href="case-extrapolation.html" title="Case Study: Simple Extrapolation"
              >next</a> |</li>
         <li class="right" >
           <a href="overview.html" title="Overview and Tutorial"
              >previous</a> |</li>
-        <li class="nav-item nav-item-0"><a href="index.html">lsqfit 9.4 documentation</a> &#187;</li> 
+        <li class="nav-item nav-item-0"><a href="index.html">lsqfit 9.5 documentation</a> &#187;</li> 
       </ul>
     </div>
     <div class="footer" role="contentinfo">
         &#169; Copyright 2009-2018, G. P. Lepage.
       Created using <a href="http://sphinx-doc.org/">Sphinx</a> 1.7.4.
     </div>
   </body>
```

#### html2text {}

```diff
@@ -9,15 +9,15 @@
 
 
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * lsqfit_9.4_documentation »
+    * lsqfit_9.5_documentation »
 ****** Non-Gaussian Behavior; Testing FitsÂ¶ ******
 ***** IntroductionÂ¶ *****
 The various analyses in the Tutorial assume implicitly that every probability
 distribution relevant to a fit is Gaussian. The input data and priors are
 assumed Gaussian. The chi**2 function is assumed to be well approximated by a
 Gaussian in the vicinity of its minimum, in order to estimate uncertainties for
 the best-fit parameters. Functions of those parameters are assumed to yield
@@ -677,9 +677,9 @@
 **** Quick search ****
 [q                   ] [Go]
 **** Navigation ****
     * index
     * modules |
     * next |
     * previous |
-    * lsqfit_9.4_documentation »
+    * lsqfit_9.5_documentation »
 © Copyright 2009-2018, G. P. Lepage. Created using Sphinx 1.7.4.
```

### Comparing `lsqfit-9.4/INSTALLATION.txt` & `lsqfit-9.5/INSTALLATION.txt`

 * *Files identical despite different names*

### Comparing `lsqfit-9.4/README.rst` & `lsqfit-9.5/README.rst`

 * *Files identical despite different names*

### Comparing `lsqfit-9.4/LICENSE.txt` & `lsqfit-9.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `lsqfit-9.4/src/lsqfit/_gsl.c` & `lsqfit-9.5/src/lsqfit/_gsl.c`

 * *Files identical despite different names*

### Comparing `lsqfit-9.4/src/lsqfit/__init__.py` & `lsqfit-9.5/src/lsqfit/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -239,14 +239,30 @@
             same file after the fit (for priming future fits). If ``p0`` is
             ``None`` or the attempt to read the file fails, starting values
             are extracted from ``prior``. If ``p0`` is ``True``, it
             is replaced by a starting point drawn at random from the
             ``prior`` distribution. The default value is ``None``;
             ``p0`` must be explicitly specified if ``prior`` is ``None``.
 
+        linear (list or None): Optional list of fit parameters that appear
+            linearly in the fit function. The fit function can be reexpressed
+            (using *variable projection*) as a function that is independent of
+            its linear parameters. The resulting fit has fewer fit parameters
+            and typically will converge in fewer iterations, but each
+            iteration will take longer. Whether or not the fit is faster or
+            more robust in any particular application is a matter for
+            experiment, but answers should be the same either way. The linear
+            parameters are reconstructed from the nonlinear parameters (and
+            the data) after the fit. Parameter ``linear`` is either: a list of
+            dictionary keys corresponding to linear parameters when the
+            parameters are stored in a dictionary (see ``prior``); or, a list
+            of indices corresponding to these parameters when they are stored
+            in an array. Note that this feature is experimental; the
+            interface may change in the future.
+
         svdcut (float or None): If ``svdcut`` is nonzero
             (but not ``None``), SVD cuts are applied to every block-diagonal
             sub-matrix of the covariance matrix for the data ``y`` and ``prior``
             (if there is a prior). The blocks are first rescaled so that all
             diagonal elements equal 1 -- that is, the blocks are replaced by
             the correlation matrices for the corresponding subsets of
             variables. Then, if ``svdcut > 0``, eigenvalues of the rescaled
@@ -443,15 +459,15 @@
     DEFAULTS = {}
 
     FITTERS = _FITTERS
 
     def __init__(
         self, data=None, fcn=None, prior=None, p0=None, extend=None,
         svdcut=False, debug=None, tol=None, maxit=None, udata=None,
-        fitter=None, **fitterargs
+        linear=[], fitter=None, **fitterargs
         ):
 
         # check arguments
         if data is None and udata is None:
             raise ValueError('neither data nor udata is specified')
         if fcn is None:
             raise ValueError('no fit function specified')
@@ -535,16 +551,44 @@
         # create fit function chiv for multifit
         self._chiv, self._chivw = _build_chiv_chivw(
             fdata=fdata, fcn=flatfcn, prior=self.prior
             )
         self.dof = self._chiv.nf - self.p0.size
         nf = self._chiv.nf
 
+        # check for linear variables
+        if linear is not None:
+            if self.p0.shape is None:
+                self.linear = []
+                bufsize = len(self.p0.buf)
+                for k in linear:
+                    if k not in self.p0:
+                        raise ValueError('key {} not in prior'.format(k))
+                    sl = self.p0.slice(k)
+                    if isinstance(sl, slice):
+                        self.linear += range(
+                            sl.start, sl.stop,
+                            sl.step if sl.step is not None else 1
+                            )
+                    else:
+                        self.linear += [sl]
+            elif len(linear) > 0:
+                ptmp = numpy.zeros(self.p0.shape, dtype=bool)
+                ptmp[linear] = True
+                ptmp = ptmp.flatten()
+                self.linear = numpy.arange(len(ptmp))[ptmp]
+            else:
+                self.linear = []
+        else:
+            self.linear = []
+
         # trial run if debugging
         if self.debug:
+            if self.dof < 0:
+                raise RuntimeError('fewer data values than parameters')
             if self.prior is None:
                 p0gvar = numpy.array([p0i*_gvar.gvar(1, 1)
                                 for p0i in p0.flat])
                 nchivw = self.y.size
             else:
                 p0gvar = self.prior.flatten() + p0
                 nchivw = self.y.size + self.prior.size
@@ -590,17 +634,20 @@
             else:
                 lower, upper = self.fitterargs['bounds']
                 larray = numpy.reshape(lower, -1)
                 uarray = numpy.reshape(upper, -1)
             self.fitterargs['bounds'] = (larray, uarray)
 
         # do the fit and save results
-        fit = nonlinear_fit.FITTERS[self.fitter](
-            p0, nf, self._chiv, tol=tol, maxit=maxit, **self.fitterargs
-            )
+        if linear is not None and len(linear) > 0:
+            fit = self._varpro_fit(p0=p0, nf=nf, tol=tol, maxit=maxit)
+        else:
+            fit = nonlinear_fit.FITTERS[self.fitter](
+                p0, nf, self._chiv, tol=tol, maxit=maxit, **self.fitterargs
+                )
         self.error = fit.error
         self.cov = fit.cov
         self.chi2 = numpy.sum(fit.f**2)
         self.Q = gammaQ(self.dof/2., self.chi2/2.)
         self.nit = fit.nit
         self.tol = fit.tol
         self.stopping_criterion = fit.stopping_criterion
@@ -635,20 +682,73 @@
             self.logGBF = 0.5*(
                 logdet_cov - fdata.logdet - self.chi2 -
                 self.dof * numpy.log(2. * numpy.pi)
                 )
 
         # archive final parameter values if requested
         if self.p0file is not None:
-            self.dump_pmean(self.p0file)
+            with open(self.p0file, "wb") as f:
+                if self.p0.shape is not None:
+                    pickle.dump(numpy.array(self.pmean), f)
+                else:
+                    # dump as a dict
+                    pickle.dump(collections.OrderedDict(self.pmean), f)
 
         self.time = clock()-cpu_time
         if self.debug:
             self.check_roundoff()
 
+    def _varpro_fit(self, p0, nf, tol, maxit):
+        def lstsq(M, y):
+            try:
+                MTM = M.T.dot(M)
+                MTy = M.T.dot(y)
+                return _gvar.linalg.solve(MTM, MTy)
+            except:
+                return _gvar.linalg.lstsq(M, y)
+        def M_y(p):
+            " chiv = y - M @ p defines y and M "
+            p[self.linear] *= 0.0
+            y = self._chiv(p)
+            M = []
+            for i in self.linear:
+                p[i] -= 1.0
+                M.append(self._chiv(p) - y)
+                p[i] += 1.0
+            return numpy.transpose(M), y
+        def fitfcn(p):
+            M, y = M_y(p)
+            p[self.linear] = lstsq(M, y)
+            return self._chiv(p)
+        localgvar = _gvar.gvar_factory()
+        if len(self.linear) < len(p0):
+            fit = nonlinear_fit.FITTERS[self.fitter](
+                p0, nf, fitfcn, tol=tol, maxit=maxit, **self.fitterargs
+                )
+            p = localgvar(fit.x, fit.cov)
+        else:
+            class dummy:
+                def __init__(self):
+                    pass
+            fit = dummy()
+            fit.nit = 0
+            fit.tol = (1e-8, 1e-10, 1e-10)
+            fit.error = None
+            fit.results = None
+            fit.stopping_criterion = 0
+            fit.description = 'no fit - all parameters linear'
+            p = localgvar(p0, p0)
+        M, y = M_y(p)
+        y += localgvar(len(y) * ['0(1)'])
+        p[self.linear] = lstsq(M, y)
+        fit.x = _gvar.mean(p)
+        fit.cov = _gvar.evalcov(p)
+        fit.f = self._chiv(fit.x)
+        return fit
+
     @staticmethod
     def set(clear=False, **defaults):
         """ Set default parameters for :class:`lsqfit.nonlinear_fit`.
 
         Use to set default values for parameters: ``extend``, ``svdcut``,
         ``debug``, ``tol``, ``maxit``, and ``fitter``. Can also set
         parameters specific to the fitter specified by the ``fitter``
@@ -736,44 +836,51 @@
     fmt_errorbudget = _gvar.fmt_errorbudget
     fmt_values = _gvar.fmt_values
 
     def format(self, maxline=0, pstyle='v', nline=None):
         """ Formats fit output details into a string for printing.
 
         The output tabulates the ``chi**2`` per degree of freedom of the fit
-        (``chi2/dof``), the number of degrees of freedom, the logarithm of the
-        Gaussian Bayes Factor for the fit (``logGBF``), and the number of fit-
-        algorithm iterations needed by the fit. Optionally, it will also list
-        the best-fit values for the fit parameters together with the prior for
-        each (in ``[]`` on each line). Lines for parameters that deviate from
-        their prior by more than one (prior) standard deviation are marked
-        with asterisks, with the number of asterisks equal to the number of
-        standard deviations (up to five). ``format`` can also list all of the
-        data and the corresponding values from the fit, again with asterisks
-        on lines  where there is a significant discrepancy. At the end it
-        lists the SVD cut, the number of eigenmodes modified by the SVD cut,
-        the tolerances used in the fit, and the time in seconds needed to do
-        the fit. The tolerance used to terminate the fit is marked with an
-        asterisk.
-
-        :param maxline: Maximum number of data points for which fit
-            results and input data are tabulated. ``maxline<0`` implies
-            that only ``chi2``, ``Q``, ``logGBF``, and ``itns`` are
-            tabulated; no parameter values are included. Setting
-            ``maxline=True`` prints all data points; setting it
-            equal ``None`` or ``False`` is the same as setting
-            it equal to ``-1``. Default is ``maxline=0``.
-        :type maxline: integer or bool
-        :param pstyle: Style used for parameter list. Supported values are
-            'vv' for very verbose, 'v' for verbose, and 'm' for minimal.
-            When 'm' is set, only parameters whose values differ from their
-            prior values are listed. Setting ``pstyle=None`` implies
-            no parameters are listed.
-        :type pstyle: 'vv', 'v', 'm', or ``None``
-        :returns: String containing detailed information about fit.
+        (``chi2/dof``), the number of degrees of freedom, the ``Q``  value of
+        the fit (ie, p-value), and the logarithm of the Gaussian Bayes Factor
+        for the fit (``logGBF``). At the end it lists the SVD cut, the number
+        of eigenmodes modified by the SVD cut, the tolerances used in the fit,
+        and the time in seconds needed to do the fit. The tolerance used to
+        terminate the fit is marked with an asterisk. It also lists
+        information about the fitter used if it is other than the standard
+        choice.
+
+        Optionally, ``format`` will also list the best-fit values
+        for the fit parameters together with the prior for each (in ``[]`` on
+        each line). Lines for parameters that deviate from their prior by more
+        than one (prior) standard deviation are marked with asterisks, with
+        the number of asterisks equal to the number of standard deviations (up
+        to five). Lines for parameters designated as linear (see ``linear``
+        keyword) are marked with a minus sign after their prior.
+
+        ``format`` can also list all of the data and the corresponding values
+        from the fit, again with asterisks on lines  where there is a
+        significant discrepancy.
+
+        Args:
+            maxline (int or bool): Maximum number of data points for which
+                fit results and input data are tabulated. ``maxline<0``
+                implies that only ``chi2``, ``Q``, ``logGBF``, and ``itns``
+                are tabulated; no parameter values are included. Setting
+                ``maxline=True`` prints all data points; setting it
+                equal ``None`` or ``False`` is the same as setting
+                it equal to ``-1``. Default is ``maxline=0``.
+            pstyle (str or None): Style used for parameter list. Supported
+                values are 'vv' for very verbose, 'v' for verbose, and 'm' for
+                minimal. When 'm' is set, only parameters whose values differ
+                from their prior values are listed. Setting ``pstyle=None``
+                implies no parameters are listed.
+
+        Returns:
+            String containing detailed information about fit.
         """
         # unpack arguments
         if nline is not None and maxline == 0:
             maxline = nline         # for legacy code (old name)
         if maxline is True:
             # print all data
             maxline = sys.maxsize
@@ -935,24 +1042,32 @@
                     prior = self.p0 + _gvar.gvar(0,float('inf'))
             data = collect(self.palt, prior, style=pstyle, stride=1, extend=self.extend)
             w1, w2, w3 = collect.width
             fst = "%%%ds%s%%%ds%s[ %%%ds ]" % (
                 max(w1, 15), 3 * ' ',
                 max(w2, 10), int(max(w2,10)/2) * ' ', max(w3,10)
                 )
-            for di, stars in zip(data, collect.stars):
+            if len(self.linear) > 0:
+                spacer = [' ', '-']
+            else:
+                spacer = ['', '']
+            for i, (di, stars) in enumerate(zip(data, collect.stars)):
                 if di is None:
                     # marker for boundary between true fit parameters and derived parameters
                     ndashes = (
                         max(w1, 15) + 3 + max(w2, 10) + int(max(w2, 10)/2)
                         + 4 + max(w3, 10)
                         )
                     table += ndashes * '-' + '\n'
                     continue
-                table += (fst % tuple(di)) + stars + '\n'
+                table += (
+                    (fst % tuple(di)) +
+                    spacer[i in self.linear] +
+                    stars + '\n'
+                    )
 
         # settings
         settings = "\nSettings:"
         settings += "\n  svdcut/n = {svdcut}/{svdn}".format(
             svdcut=self.svdcut, svdn=self.svdn
             )
         fmtstr = [
@@ -1027,40 +1142,52 @@
         ``p = nonlinear_fit.load_p(filename)`` is used to recover the
         values of fit parameters dumped using ``fit.dump_p(filename)`` (or
         ``fit.dump_pmean(filename)``) where ``fit`` is of type
         :class:`lsqfit.nonlinear_fit`. The layout of the returned
         parameters ``p`` is the same as that of ``fit.p`` (or
         ``fit.pmean``).
         """
+        warnings.warn(
+            "nonlinear_fit.load_parameters deprecated; use pickle.load or gvar.load instead",
+            DeprecationWarning,
+            )
         with open(filename,"rb") as f:
             return pickle.load(f)
 
     def dump_p(self, filename):
         """ Dump parameter values (``fit.p``) into file ``filename``.
 
         ``fit.dump_p(filename)`` saves the best-fit parameter values
         (``fit.p``) from a ``nonlinear_fit`` called ``fit``. These values
         are recovered using
         ``p = nonlinear_fit.load_parameters(filename)``
         where ``p``'s layout is the same as that of ``fit.p``.
         """
+        warnings.warn(
+            "nonlinear_fit.dump_p deprecated; use gvar.dump instead",
+            DeprecationWarning
+            )
         with open(filename, "wb") as f:
             pickle.dump(self.palt, f) # dump as a dict
 
     def dump_pmean(self, filename):
         """ Dump parameter means (``fit.pmean``) into file ``filename``.
 
         ``fit.dump_pmean(filename)`` saves the means of the best-fit
         parameter values (``fit.pmean``) from a ``nonlinear_fit`` called
         ``fit``. These values are recovered using
         ``p0 = nonlinear_fit.load_parameters(filename)``
         where ``p0``'s layout is the same as ``fit.pmean``. The saved
         values can be used to initialize a later fit (``nonlinear_fit``
         parameter ``p0``).
         """
+        warnings.warn(
+            "nonlinear_fit.dump_pmean deprecated; use pickle.dump instead",
+            DeprecationWarning,
+            )
         with open(filename, "wb") as f:
             if self.p0.shape is not None:
                 pickle.dump(numpy.array(self.pmean), f)
             else:
                 pickle.dump(collections.OrderedDict(self.pmean), f) # dump as a dict
 
     def simulated_fit_iter(self, n, pexact=None, bootstrap=False, **kargs):
@@ -1459,17 +1586,16 @@
     removed from p0 if extend=True and there is no prior. There is
     no need to remove them if there is a prior, since its keys are
     used (and it has no redundant keys at this point).
     """
     if p0file is not None:
         # p0 is a filename; read in values
         try:
-            p0 = nonlinear_fit.load_parameters(p0file)
-            # with open(p0file, "rb") as f:
-            #     p0 = pickle.load(f)
+            with open(p0file, "rb") as f:
+                p0 = pickle.load(f)
         except (IOError, EOFError):
             if prior is None:
                 raise IOError(
                     "No prior and can't read parameters from " + p0file
                     )
             else:
                 p0 = None
```

### Comparing `lsqfit-9.4/src/lsqfit/_scipy.py` & `lsqfit-9.5/src/lsqfit/_scipy.py`

 * *Files identical despite different names*

### Comparing `lsqfit-9.4/src/lsqfit/_gsl.pyx` & `lsqfit-9.5/src/lsqfit/_gsl.pyx`

 * *Files identical despite different names*

### Comparing `lsqfit-9.4/src/lsqfit/_extras.py` & `lsqfit-9.5/src/lsqfit/_extras.py`

 * *Files 2% similar despite different names*

```diff
@@ -813,14 +813,45 @@
             else:
                 for m in mf['flatmodels']:
                     ii = (gvar.mean(f_all[m.datatag]) != 0)
                     ratio = f_trunc[m.datatag][ii] / f_all[m.datatag][ii]
                     pdata[m.datatag][ii] *= ratio
         return pdata
 
+    # @staticmethod
+    # def _update_prior(prior, update):
+    #     """ update prior[k] with dictionary update[k]
+
+    #     prior[k] is updated by update[k] provided update[k] is the
+    #     same shape and size, or provided update[k] has larger size.
+    #     """
+    #     for k in update:
+    #         if k not in prior:
+    #             prior[k] = update[k]
+    #         else:
+    #             pshape = numpy.shape(prior[k])
+    #             ushape = numpy.shape(update[k])
+    #             if (
+    #                 (pshape == ushape) or
+    #                 (numpy.size(prior[k]) >= numpy.size(update[k]))
+    #                 ):
+    #                 continue
+    #             if len(pshape) == len(ushape):
+    #                 if (
+    #                     pshape == ushape or
+    #                     numpy.size(prior[k]) < numpy.size(update[k])
+    #                     ):
+    #                     prior[k] = update[k]
+    #             else:
+    #                 raise ValueError(
+    #                     'mismatched prior shapes for {}: {} and {}'.format(
+    #                         str(k), pshape, ushape
+    #                         )
+    #                     )
+
     def buildprior(self, prior, mf=None):
         """ Create prior to fit models in list ``models``.
 
         Setting parameter ``fast=True`` strips any variable
         not required by the fit from the prior. This speeds
         fits but loses information about correlations between
         variables in the fit and those that are not. The
@@ -833,14 +864,15 @@
         nprior = gvar.BufferDict()
         # save mprior for chained_fit -- fast
         self.mprior = collections.OrderedDict()
         for m in mf['flatmodels']:
             self.mprior[m.datatag] = m.buildprior(
                 prior, mopt=mf['mopt'], extend=mf['extend']
                 )
+            # self._update_prior(nprior, self.mprior[m.datatag])
             nprior.update(self.mprior[m.datatag])
         if not mf['fast']:
             for k in prior:
                 if k not in nprior:
                     nprior[k] = prior[k]
         return nprior
```

### Comparing `lsqfit-9.4/src/lsqfit/_utilities.pyx` & `lsqfit-9.5/src/lsqfit/_utilities.pyx`

 * *Files identical despite different names*

### Comparing `lsqfit-9.4/src/lsqfit/_utilities.c` & `lsqfit-9.5/src/lsqfit/_utilities.c`

 * *Files identical despite different names*

