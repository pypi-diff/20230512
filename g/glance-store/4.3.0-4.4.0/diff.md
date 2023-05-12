# Comparing `tmp/glance_store-4.3.0.tar.gz` & `tmp/glance_store-4.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glance_store-4.3.0.tar", last modified: Fri Feb 10 16:03:17 2023, max compression
+gzip compressed data, was "glance_store-4.4.0.tar", last modified: Fri May 12 14:50:07 2023, max compression
```

## Comparing `glance_store-4.3.0.tar` & `glance_store-4.4.0.tar`

### file list

```diff
@@ -1,228 +1,231 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:03:17.398118 glance_store-4.3.0/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       57 2023-02-10 16:02:40.000000 glance_store-4.3.0/.stestr.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6002 2023-02-10 16:02:40.000000 glance_store-4.3.0/.zuul.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6192 2023-02-10 16:03:17.000000 glance_store-4.3.0/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    28712 2023-02-10 16:03:17.000000 glance_store-4.3.0/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2023-02-10 16:02:40.000000 glance_store-4.3.0/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2727 2023-02-10 16:03:17.398118 glance_store-4.3.0/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1396 2023-02-10 16:02:40.000000 glance_store-4.3.0/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:03:17.370118 glance_store-4.3.0/doc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      337 2023-02-10 16:02:40.000000 glance_store-4.3.0/doc/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:03:17.370118 glance_store-4.3.0/doc/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3964 2023-02-10 16:02:40.000000 glance_store-4.3.0/doc/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      720 2023-02-10 16:02:40.000000 glance_store-4.3.0/doc/source/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:03:17.370118 glance_store-4.3.0/doc/source/reference/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2023-02-10 16:02:40.000000 glance_store-4.3.0/doc/source/reference/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:03:17.370118 glance_store-4.3.0/doc/source/user/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1142 2023-02-10 16:02:40.000000 glance_store-4.3.0/doc/source/user/drivers.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      127 2023-02-10 16:02:40.000000 glance_store-4.3.0/doc/source/user/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:03:17.362118 glance_store-4.3.0/etc/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:03:17.370118 glance_store-4.3.0/etc/glance/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      972 2023-02-10 16:02:40.000000 glance_store-4.3.0/etc/glance/rootwrap.conf
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:03:17.370118 glance_store-4.3.0/etc/glance/rootwrap.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      721 2023-02-10 16:02:40.000000 glance_store-4.3.0/etc/glance/rootwrap.d/glance_cinder_store.filters
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:03:17.370118 glance_store-4.3.0/glance_store/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      761 2023-02-10 16:02:40.000000 glance_store-4.3.0/glance_store/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:03:17.374118 glance_store-4.3.0/glance_store/_drivers/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:02:40.000000 glance_store-4.3.0/glance_store/_drivers/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:03:17.374118 glance_store-4.3.0/glance_store/_drivers/cinder/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      685 2023-02-10 16:02:40.000000 glance_store-4.3.0/glance_store/_drivers/cinder/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2364 2023-02-10 16:02:40.000000 glance_store-4.3.0/glance_store/_drivers/cinder/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4106 2023-02-10 16:02:40.000000 glance_store-4.3.0/glance_store/_drivers/cinder/nfs.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3074 2023-02-10 16:02:40.000000 glance_store-4.3.0/glance_store/_drivers/cinder/scaleio.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    42949 2023-02-10 16:02:40.000000 glance_store-4.3.0/glance_store/_drivers/cinder/store.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    31286 2023-02-10 16:02:40.000000 glance_store-4.3.0/glance_store/_drivers/filesystem.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12238 2023-02-10 16:02:40.000000 glance_store-4.3.0/glance_store/_drivers/http.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    27712 2023-02-10 16:02:40.000000 glance_store-4.3.0/glance_store/_drivers/rbd.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    37711 2023-02-10 16:02:40.000000 glance_store-4.3.0/glance_store/_drivers/s3.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:03:17.374118 glance_store-4.3.0/glance_store/_drivers/swift/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      739 2023-02-10 16:02:40.000000 glance_store-4.3.0/glance_store/_drivers/swift/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6698 2023-02-10 16:02:40.000000 glance_store-4.3.0/glance_store/_drivers/swift/buffered.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9117 2023-02-10 16:02:40.000000 glance_store-4.3.0/glance_store/_drivers/swift/connection_manager.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    69799 2023-02-10 16:02:40.000000 glance_store-4.3.0/glance_store/_drivers/swift/store.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8362 2023-02-10 16:02:40.000000 glance_store-4.3.0/glance_store/_drivers/swift/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    32181 2023-02-10 16:02:40.000000 glance_store-4.3.0/glance_store/_drivers/vmware_datastore.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17462 2023-02-10 16:02:40.000000 glance_store-4.3.0/glance_store/backend.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5630 2023-02-10 16:02:40.000000 glance_store-4.3.0/glance_store/capabilities.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:03:17.378118 glance_store-4.3.0/glance_store/common/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:02:40.000000 glance_store-4.3.0/glance_store/common/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9510 2023-02-10 16:02:40.000000 glance_store-4.3.0/glance_store/common/attachment_state_manager.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9744 2023-02-10 16:02:40.000000 glance_store-4.3.0/glance_store/common/cinder_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14677 2023-02-10 16:02:40.000000 glance_store-4.3.0/glance_store/common/fs_mount.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4731 2023-02-10 16:02:40.000000 glance_store-4.3.0/glance_store/common/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10356 2023-02-10 16:02:40.000000 glance_store-4.3.0/glance_store/driver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5400 2023-02-10 16:02:40.000000 glance_store-4.3.0/glance_store/exceptions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1113 2023-02-10 16:02:40.000000 glance_store-4.3.0/glance_store/i18n.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:03:17.366118 glance_store-4.3.0/glance_store/locale/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:03:17.366118 glance_store-4.3.0/glance_store/locale/en_GB/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:03:17.378118 glance_store-4.3.0/glance_store/locale/en_GB/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8378 2023-02-10 16:02:40.000000 glance_store-4.3.0/glance_store/locale/en_GB/LC_MESSAGES/glance_store.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:03:17.366118 glance_store-4.3.0/glance_store/locale/ko_KR/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:03:17.378118 glance_store-4.3.0/glance_store/locale/ko_KR/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6352 2023-02-10 16:02:40.000000 glance_store-4.3.0/glance_store/locale/ko_KR/LC_MESSAGES/glance_store.po
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8655 2023-02-10 16:02:40.000000 glance_store-4.3.0/glance_store/location.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    22611 2023-02-10 16:02:40.000000 glance_store-4.3.0/glance_store/multi_backend.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:03:17.378118 glance_store-4.3.0/glance_store/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:02:40.000000 glance_store-4.3.0/glance_store/tests/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4234 2023-02-10 16:02:40.000000 glance_store-4.3.0/glance_store/tests/base.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:03:17.378118 glance_store-4.3.0/glance_store/tests/etc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      954 2023-02-10 16:02:40.000000 glance_store-4.3.0/glance_store/tests/etc/glance-swift.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      834 2023-02-10 16:02:40.000000 glance_store-4.3.0/glance_store/tests/fakes.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:03:17.378118 glance_store-4.3.0/glance_store/tests/functional/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2909 2023-02-10 16:02:40.000000 glance_store-4.3.0/glance_store/tests/functional/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:02:40.000000 glance_store-4.3.0/glance_store/tests/functional/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3915 2023-02-10 16:02:40.000000 glance_store-4.3.0/glance_store/tests/functional/base.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:03:17.378118 glance_store-4.3.0/glance_store/tests/functional/filesystem/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:02:40.000000 glance_store-4.3.0/glance_store/tests/functional/filesystem/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1359 2023-02-10 16:02:40.000000 glance_store-4.3.0/glance_store/tests/functional/filesystem/test_functional_filesystem.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:03:17.378118 glance_store-4.3.0/glance_store/tests/functional/swift/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:02:40.000000 glance_store-4.3.0/glance_store/tests/functional/swift/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3228 2023-02-10 16:02:40.000000 glance_store-4.3.0/glance_store/tests/functional/swift/test_functional_swift.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:03:17.382118 glance_store-4.3.0/glance_store/tests/unit/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:02:40.000000 glance_store-4.3.0/glance_store/tests/unit/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:03:17.382118 glance_store-4.3.0/glance_store/tests/unit/cinder/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4649 2023-02-10 16:02:40.000000 glance_store-4.3.0/glance_store/tests/unit/cinder/test_base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    40760 2023-02-10 16:02:40.000000 glance_store-4.3.0/glance_store/tests/unit/cinder/test_cinder_base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6764 2023-02-10 16:02:40.000000 glance_store-4.3.0/glance_store/tests/unit/cinder/test_cinder_store.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12926 2023-02-10 16:02:40.000000 glance_store-4.3.0/glance_store/tests/unit/cinder/test_multistore_cinder.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3933 2023-02-10 16:02:40.000000 glance_store-4.3.0/glance_store/tests/unit/cinder/test_nfs.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1849 2023-02-10 16:02:40.000000 glance_store-4.3.0/glance_store/tests/unit/cinder/test_scaleio.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:03:17.386118 glance_store-4.3.0/glance_store/tests/unit/common/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:02:40.000000 glance_store-4.3.0/glance_store/tests/unit/common/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4716 2023-02-10 16:02:40.000000 glance_store-4.3.0/glance_store/tests/unit/common/test_attachment_state_manager.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7621 2023-02-10 16:02:40.000000 glance_store-4.3.0/glance_store/tests/unit/common/test_cinder_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5763 2023-02-10 16:02:40.000000 glance_store-4.3.0/glance_store/tests/unit/common/test_fs_mount.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1144 2023-02-10 16:02:40.000000 glance_store-4.3.0/glance_store/tests/unit/common/test_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5862 2023-02-10 16:02:40.000000 glance_store-4.3.0/glance_store/tests/unit/test_backend.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8014 2023-02-10 16:02:40.000000 glance_store-4.3.0/glance_store/tests/unit/test_connection_manager.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16806 2023-02-10 16:02:40.000000 glance_store-4.3.0/glance_store/tests/unit/test_driver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2223 2023-02-10 16:02:40.000000 glance_store-4.3.0/glance_store/tests/unit/test_exceptions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    35512 2023-02-10 16:02:40.000000 glance_store-4.3.0/glance_store/tests/unit/test_filesystem_store.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8581 2023-02-10 16:02:40.000000 glance_store-4.3.0/glance_store/tests/unit/test_http_store.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1204 2023-02-10 16:02:40.000000 glance_store-4.3.0/glance_store/tests/unit/test_location.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    35205 2023-02-10 16:02:40.000000 glance_store-4.3.0/glance_store/tests/unit/test_multistore_filesystem.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17509 2023-02-10 16:02:40.000000 glance_store-4.3.0/glance_store/tests/unit/test_multistore_rbd.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    24725 2023-02-10 16:02:40.000000 glance_store-4.3.0/glance_store/tests/unit/test_multistore_s3.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    29875 2023-02-10 16:02:40.000000 glance_store-4.3.0/glance_store/tests/unit/test_multistore_vmware.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5643 2023-02-10 16:02:40.000000 glance_store-4.3.0/glance_store/tests/unit/test_opts.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    26314 2023-02-10 16:02:40.000000 glance_store-4.3.0/glance_store/tests/unit/test_rbd_store.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    23476 2023-02-10 16:02:40.000000 glance_store-4.3.0/glance_store/tests/unit/test_s3_store.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3408 2023-02-10 16:02:40.000000 glance_store-4.3.0/glance_store/tests/unit/test_store_base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6435 2023-02-10 16:02:40.000000 glance_store-4.3.0/glance_store/tests/unit/test_store_capabilities.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   101255 2023-02-10 16:02:40.000000 glance_store-4.3.0/glance_store/tests/unit/test_swift_store.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    97793 2023-02-10 16:02:40.000000 glance_store-4.3.0/glance_store/tests/unit/test_swift_store_multibackend.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6319 2023-02-10 16:02:40.000000 glance_store-4.3.0/glance_store/tests/unit/test_swift_store_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1349 2023-02-10 16:02:40.000000 glance_store-4.3.0/glance_store/tests/unit/test_test_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    30386 2023-02-10 16:02:40.000000 glance_store-4.3.0/glance_store/tests/unit/test_vmware_store.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3780 2023-02-10 16:02:40.000000 glance_store-4.3.0/glance_store/tests/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:03:17.374118 glance_store-4.3.0/glance_store.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2727 2023-02-10 16:03:17.000000 glance_store-4.3.0/glance_store.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8228 2023-02-10 16:03:17.000000 glance_store-4.3.0/glance_store.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-02-10 16:03:17.000000 glance_store-4.3.0/glance_store.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1021 2023-02-10 16:03:17.000000 glance_store-4.3.0/glance_store.egg-info/entry_points.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-02-10 16:03:17.000000 glance_store-4.3.0/glance_store.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2023-02-10 16:03:17.000000 glance_store-4.3.0/glance_store.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      814 2023-02-10 16:03:17.000000 glance_store-4.3.0/glance_store.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       13 2023-02-10 16:03:17.000000 glance_store-4.3.0/glance_store.egg-info/top_level.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:03:17.366118 glance_store-4.3.0/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:03:17.394118 glance_store-4.3.0/releasenotes/notes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:02:40.000000 glance_store-4.3.0/releasenotes/notes/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      724 2023-02-10 16:02:40.000000 glance_store-4.3.0/releasenotes/notes/0.29.1-notes-ded2a1d473a306c7.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1216 2023-02-10 16:02:40.000000 glance_store-4.3.0/releasenotes/notes/Stein_final_release-c7df5838028b8c7e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      176 2023-02-10 16:02:40.000000 glance_store-4.3.0/releasenotes/notes/block-creating-encrypted-nfs-volumes-d0ff370ab762042e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      302 2023-02-10 16:02:40.000000 glance_store-4.3.0/releasenotes/notes/bug-1620999-8b76a0ad14826197.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      437 2023-02-10 16:02:40.000000 glance_store-4.3.0/releasenotes/notes/bug-1820817-0ee70781918d232e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      238 2023-02-10 16:02:40.000000 glance_store-4.3.0/releasenotes/notes/bug-1915602-fcc807a435d8a6bf.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      444 2023-02-10 16:02:40.000000 glance_store-4.3.0/releasenotes/notes/bug-1954883-3666d63a3c0233f1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      165 2023-02-10 16:02:40.000000 glance_store-4.3.0/releasenotes/notes/cinder-fix-nfs-sparse-vol-create-76631ce05f86257c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      217 2023-02-10 16:02:40.000000 glance_store-4.3.0/releasenotes/notes/cinder-nfs-block-qcow2-vol-4fed58b0afafc980.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      398 2023-02-10 16:02:40.000000 glance_store-4.3.0/releasenotes/notes/cinder-support-extend-in-use-volume-c6292f950ff75cca.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      318 2023-02-10 16:02:40.000000 glance_store-4.3.0/releasenotes/notes/deprecate-rados_connect_timeout-767ed1eaa026196e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      546 2023-02-10 16:02:40.000000 glance_store-4.3.0/releasenotes/notes/deprecate-sheepdog-driver-1f9689c327f313d4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      797 2023-02-10 16:02:40.000000 glance_store-4.3.0/releasenotes/notes/deprecate-store_add_to_backend-f419e5c4210613d2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      680 2023-02-10 16:02:40.000000 glance_store-4.3.0/releasenotes/notes/deprecate-store_capabilities_update_min_interval-039389fa296e2494.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      209 2023-02-10 16:02:40.000000 glance_store-4.3.0/releasenotes/notes/drop-py-2-7-345cafc9c1d3f892.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      129 2023-02-10 16:02:40.000000 glance_store-4.3.0/releasenotes/notes/drop-python-3-6-and-3-7-41af87576c4fd7b1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      219 2023-02-10 16:02:40.000000 glance_store-4.3.0/releasenotes/notes/fix-exception-logging-during-attach-9546e24189db83c4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      249 2023-02-10 16:02:40.000000 glance_store-4.3.0/releasenotes/notes/fix-interval-in-retries-471155ff34d9f0e9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      225 2023-02-10 16:02:40.000000 glance_store-4.3.0/releasenotes/notes/fix-ip-in-connector-info-36b95d9959f10f63.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      215 2023-02-10 16:02:40.000000 glance_store-4.3.0/releasenotes/notes/fix-wait-device-resize-c282940b71a3748e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      124 2023-02-10 16:02:40.000000 glance_store-4.3.0/releasenotes/notes/fs-drv-chunk-sz-a1b2f6a72fad92d5.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      664 2023-02-10 16:02:40.000000 glance_store-4.3.0/releasenotes/notes/handle-sparse-image-a3ecfc4ae1c00d48.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1342 2023-02-10 16:02:40.000000 glance_store-4.3.0/releasenotes/notes/improved-configuration-options-3635b56aba3072c9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      485 2023-02-10 16:02:40.000000 glance_store-4.3.0/releasenotes/notes/lock_path-cef9d6f5f52c3211.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      201 2023-02-10 16:02:40.000000 glance_store-4.3.0/releasenotes/notes/move-rootwrap-config-f2cf435c548aab5c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      686 2023-02-10 16:02:40.000000 glance_store-4.3.0/releasenotes/notes/multi-store-0c004fc8aba2a25d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      385 2023-02-10 16:02:40.000000 glance_store-4.3.0/releasenotes/notes/multi-tenant-store-058b67ce5b7f3bd0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      379 2023-02-10 16:02:40.000000 glance_store-4.3.0/releasenotes/notes/multiattach-volume-handling-1a8446a64463f2cf.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      636 2023-02-10 16:02:40.000000 glance_store-4.3.0/releasenotes/notes/multihash-support-629e9cbc283a8b47.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2459 2023-02-10 16:02:40.000000 glance_store-4.3.0/releasenotes/notes/pike-relnote-9f547df14184d18c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      585 2023-02-10 16:02:40.000000 glance_store-4.3.0/releasenotes/notes/prevent-unauthorized-errors-ebb9cf2236595cd0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2561 2023-02-10 16:02:40.000000 glance_store-4.3.0/releasenotes/notes/queens-relnote-5fa2d009d9a9e458.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2096 2023-02-10 16:02:40.000000 glance_store-4.3.0/releasenotes/notes/release-1.0.0-7ab43e91523eb3c8.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      693 2023-02-10 16:02:40.000000 glance_store-4.3.0/releasenotes/notes/release-1.0.1-098b1487ac8cc9a1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1384 2023-02-10 16:02:40.000000 glance_store-4.3.0/releasenotes/notes/release-1.2.0-8d239f01cd8ff0bf.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      627 2023-02-10 16:02:40.000000 glance_store-4.3.0/releasenotes/notes/releasenote-0.17.0-efee3f557ea2096a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      353 2023-02-10 16:02:40.000000 glance_store-4.3.0/releasenotes/notes/remove-cinder-experimental-fbf9dea32c84dc9b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      218 2023-02-10 16:02:40.000000 glance_store-4.3.0/releasenotes/notes/remove-gridfs-driver-09286e27613b4353.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      693 2023-02-10 16:02:40.000000 glance_store-4.3.0/releasenotes/notes/remove-s3-driver-f432afa1f53ecdf8.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      300 2023-02-10 16:02:40.000000 glance_store-4.3.0/releasenotes/notes/remove-store-cap-update-min-interval-21fea4173ed4a09b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      429 2023-02-10 16:02:40.000000 glance_store-4.3.0/releasenotes/notes/rethinking-filesystem-access-5ab872fd0c0d27db.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      452 2023-02-10 16:02:40.000000 glance_store-4.3.0/releasenotes/notes/rocky-bugfixes-adefa8f47db16a2d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      242 2023-02-10 16:02:40.000000 glance_store-4.3.0/releasenotes/notes/set-documented-default-directory-for-filesystem-9b417a29416d3a94.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      625 2023-02-10 16:02:40.000000 glance_store-4.3.0/releasenotes/notes/sorted-drivers-for-configs-a905f07d3bf9c973.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       57 2023-02-10 16:02:40.000000 glance_store-4.3.0/releasenotes/notes/start-using-reno-73ef709807e37b74.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      347 2023-02-10 16:02:40.000000 glance_store-4.3.0/releasenotes/notes/support-cinder-multiple-stores-6cc8489f8f4f8ff3.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      412 2023-02-10 16:02:40.000000 glance_store-4.3.0/releasenotes/notes/support-cinder-upload-c85849d9c88bbd7e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      443 2023-02-10 16:02:40.000000 glance_store-4.3.0/releasenotes/notes/support-cinder-user-domain-420c76053dd50534.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      221 2023-02-10 16:02:40.000000 glance_store-4.3.0/releasenotes/notes/support-s3-driver-a4158f9fa35931d5.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      195 2023-02-10 16:02:40.000000 glance_store-4.3.0/releasenotes/notes/update-stein-deprecations-3c2f6ffeab22b558.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      300 2023-02-10 16:02:40.000000 glance_store-4.3.0/releasenotes/notes/victoria-milestone-1-c1f9de5b90e8c326.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      316 2023-02-10 16:02:40.000000 glance_store-4.3.0/releasenotes/notes/vmware-store-requests-369485d2cfdb6175.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      530 2023-02-10 16:02:40.000000 glance_store-4.3.0/releasenotes/notes/volume-type-validation-check-011a400d7fb3b307.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      300 2023-02-10 16:02:40.000000 glance_store-4.3.0/releasenotes/notes/wallaby-final-release-00f0f851ff7d93ab.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      573 2023-02-10 16:02:40.000000 glance_store-4.3.0/releasenotes/notes/xena-final-release-3c6e19dfba43b40d.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:03:17.394118 glance_store-4.3.0/releasenotes/source/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:03:17.394118 glance_store-4.3.0/releasenotes/source/_static/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:02:40.000000 glance_store-4.3.0/releasenotes/source/_static/.placeholder
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:03:17.394118 glance_store-4.3.0/releasenotes/source/_templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:02:40.000000 glance_store-4.3.0/releasenotes/source/_templates/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8972 2023-02-10 16:02:40.000000 glance_store-4.3.0/releasenotes/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      272 2023-02-10 16:02:40.000000 glance_store-4.3.0/releasenotes/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      146 2023-02-10 16:02:40.000000 glance_store-4.3.0/releasenotes/source/liberty.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:03:17.366118 glance_store-4.3.0/releasenotes/source/locale/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:03:17.366118 glance_store-4.3.0/releasenotes/source/locale/de/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:03:17.394118 glance_store-4.3.0/releasenotes/source/locale/de/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2551 2023-02-10 16:02:40.000000 glance_store-4.3.0/releasenotes/source/locale/de/LC_MESSAGES/releasenotes.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:03:17.366118 glance_store-4.3.0/releasenotes/source/locale/en_GB/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:03:17.394118 glance_store-4.3.0/releasenotes/source/locale/en_GB/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    56798 2023-02-10 16:02:40.000000 glance_store-4.3.0/releasenotes/source/locale/en_GB/LC_MESSAGES/releasenotes.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:03:17.366118 glance_store-4.3.0/releasenotes/source/locale/zh_CN/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:03:17.394118 glance_store-4.3.0/releasenotes/source/locale/zh_CN/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2420 2023-02-10 16:02:40.000000 glance_store-4.3.0/releasenotes/source/locale/zh_CN/LC_MESSAGES/releasenotes.po
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2023-02-10 16:02:40.000000 glance_store-4.3.0/releasenotes/source/mitaka.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2023-02-10 16:02:40.000000 glance_store-4.3.0/releasenotes/source/newton.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2023-02-10 16:02:40.000000 glance_store-4.3.0/releasenotes/source/ocata.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2023-02-10 16:02:40.000000 glance_store-4.3.0/releasenotes/source/pike.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2023-02-10 16:02:40.000000 glance_store-4.3.0/releasenotes/source/queens.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-02-10 16:02:40.000000 glance_store-4.3.0/releasenotes/source/rocky.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-02-10 16:02:40.000000 glance_store-4.3.0/releasenotes/source/stein.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2023-02-10 16:02:40.000000 glance_store-4.3.0/releasenotes/source/train.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2023-02-10 16:02:40.000000 glance_store-4.3.0/releasenotes/source/unreleased.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-02-10 16:02:40.000000 glance_store-4.3.0/releasenotes/source/ussuri.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2023-02-10 16:02:40.000000 glance_store-4.3.0/releasenotes/source/victoria.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2023-02-10 16:02:40.000000 glance_store-4.3.0/releasenotes/source/wallaby.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-02-10 16:02:40.000000 glance_store-4.3.0/releasenotes/source/xena.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-02-10 16:02:40.000000 glance_store-4.3.0/releasenotes/source/yoga.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2023-02-10 16:02:40.000000 glance_store-4.3.0/releasenotes/source/zed.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      594 2023-02-10 16:02:40.000000 glance_store-4.3.0/requirements.txt
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     7157 2023-02-10 16:02:40.000000 glance_store-4.3.0/run_tests.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2345 2023-02-10 16:03:17.398118 glance_store-4.3.0/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2023-02-10 16:02:40.000000 glance_store-4.3.0/setup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      918 2023-02-10 16:02:40.000000 glance_store-4.3.0/test-requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-02-10 16:03:17.398118 glance_store-4.3.0/tools/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11648 2023-02-10 16:02:40.000000 glance_store-4.3.0/tools/colorizer.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2348 2023-02-10 16:02:40.000000 glance_store-4.3.0/tools/install_venv.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5647 2023-02-10 16:02:40.000000 glance_store-4.3.0/tools/install_venv_common.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      218 2023-02-10 16:02:40.000000 glance_store-4.3.0/tools/with_venv.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2185 2023-02-10 16:02:40.000000 glance_store-4.3.0/tox.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:50:07.612553 glance_store-4.4.0/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       57 2023-05-12 14:49:16.000000 glance_store-4.4.0/.stestr.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6002 2023-05-12 14:49:16.000000 glance_store-4.4.0/.zuul.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6304 2023-05-12 14:50:07.000000 glance_store-4.4.0/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    29174 2023-05-12 14:50:07.000000 glance_store-4.4.0/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2023-05-12 14:49:16.000000 glance_store-4.4.0/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2727 2023-05-12 14:50:07.616553 glance_store-4.4.0/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1396 2023-05-12 14:49:16.000000 glance_store-4.4.0/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:50:07.580552 glance_store-4.4.0/doc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      337 2023-05-12 14:49:16.000000 glance_store-4.4.0/doc/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:50:07.580552 glance_store-4.4.0/doc/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3964 2023-05-12 14:49:16.000000 glance_store-4.4.0/doc/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      720 2023-05-12 14:49:16.000000 glance_store-4.4.0/doc/source/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:50:07.580552 glance_store-4.4.0/doc/source/reference/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2023-05-12 14:49:16.000000 glance_store-4.4.0/doc/source/reference/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:50:07.580552 glance_store-4.4.0/doc/source/user/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1142 2023-05-12 14:49:16.000000 glance_store-4.4.0/doc/source/user/drivers.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      127 2023-05-12 14:49:16.000000 glance_store-4.4.0/doc/source/user/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:50:07.572552 glance_store-4.4.0/etc/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:50:07.580552 glance_store-4.4.0/etc/glance/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      972 2023-05-12 14:49:16.000000 glance_store-4.4.0/etc/glance/rootwrap.conf
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:50:07.580552 glance_store-4.4.0/etc/glance/rootwrap.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      721 2023-05-12 14:49:16.000000 glance_store-4.4.0/etc/glance/rootwrap.d/glance_cinder_store.filters
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:50:07.584552 glance_store-4.4.0/glance_store/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      761 2023-05-12 14:49:16.000000 glance_store-4.4.0/glance_store/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:50:07.584552 glance_store-4.4.0/glance_store/_drivers/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:49:16.000000 glance_store-4.4.0/glance_store/_drivers/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:50:07.588552 glance_store-4.4.0/glance_store/_drivers/cinder/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      685 2023-05-12 14:49:16.000000 glance_store-4.4.0/glance_store/_drivers/cinder/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2440 2023-05-12 14:49:16.000000 glance_store-4.4.0/glance_store/_drivers/cinder/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4106 2023-05-12 14:49:16.000000 glance_store-4.4.0/glance_store/_drivers/cinder/nfs.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3074 2023-05-12 14:49:16.000000 glance_store-4.4.0/glance_store/_drivers/cinder/scaleio.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    43313 2023-05-12 14:49:16.000000 glance_store-4.4.0/glance_store/_drivers/cinder/store.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    31286 2023-05-12 14:49:16.000000 glance_store-4.4.0/glance_store/_drivers/filesystem.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12238 2023-05-12 14:49:16.000000 glance_store-4.4.0/glance_store/_drivers/http.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    28145 2023-05-12 14:49:16.000000 glance_store-4.4.0/glance_store/_drivers/rbd.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    38109 2023-05-12 14:49:16.000000 glance_store-4.4.0/glance_store/_drivers/s3.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:50:07.588552 glance_store-4.4.0/glance_store/_drivers/swift/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      739 2023-05-12 14:49:16.000000 glance_store-4.4.0/glance_store/_drivers/swift/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6698 2023-05-12 14:49:16.000000 glance_store-4.4.0/glance_store/_drivers/swift/buffered.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9117 2023-05-12 14:49:16.000000 glance_store-4.4.0/glance_store/_drivers/swift/connection_manager.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    69799 2023-05-12 14:49:16.000000 glance_store-4.4.0/glance_store/_drivers/swift/store.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8362 2023-05-12 14:49:16.000000 glance_store-4.4.0/glance_store/_drivers/swift/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    32181 2023-05-12 14:49:16.000000 glance_store-4.4.0/glance_store/_drivers/vmware_datastore.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17462 2023-05-12 14:49:16.000000 glance_store-4.4.0/glance_store/backend.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5630 2023-05-12 14:49:16.000000 glance_store-4.4.0/glance_store/capabilities.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:50:07.588552 glance_store-4.4.0/glance_store/common/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:49:16.000000 glance_store-4.4.0/glance_store/common/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9510 2023-05-12 14:49:16.000000 glance_store-4.4.0/glance_store/common/attachment_state_manager.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9744 2023-05-12 14:49:16.000000 glance_store-4.4.0/glance_store/common/cinder_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14677 2023-05-12 14:49:16.000000 glance_store-4.4.0/glance_store/common/fs_mount.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4731 2023-05-12 14:49:16.000000 glance_store-4.4.0/glance_store/common/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10356 2023-05-12 14:49:16.000000 glance_store-4.4.0/glance_store/driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5400 2023-05-12 14:49:16.000000 glance_store-4.4.0/glance_store/exceptions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1113 2023-05-12 14:49:16.000000 glance_store-4.4.0/glance_store/i18n.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:50:07.572552 glance_store-4.4.0/glance_store/locale/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:50:07.572552 glance_store-4.4.0/glance_store/locale/en_GB/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:50:07.588552 glance_store-4.4.0/glance_store/locale/en_GB/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8378 2023-05-12 14:49:16.000000 glance_store-4.4.0/glance_store/locale/en_GB/LC_MESSAGES/glance_store.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:50:07.572552 glance_store-4.4.0/glance_store/locale/ko_KR/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:50:07.588552 glance_store-4.4.0/glance_store/locale/ko_KR/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6352 2023-05-12 14:49:16.000000 glance_store-4.4.0/glance_store/locale/ko_KR/LC_MESSAGES/glance_store.po
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8655 2023-05-12 14:49:16.000000 glance_store-4.4.0/glance_store/location.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    22611 2023-05-12 14:49:16.000000 glance_store-4.4.0/glance_store/multi_backend.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:50:07.588552 glance_store-4.4.0/glance_store/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:49:16.000000 glance_store-4.4.0/glance_store/tests/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4234 2023-05-12 14:49:16.000000 glance_store-4.4.0/glance_store/tests/base.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:50:07.588552 glance_store-4.4.0/glance_store/tests/etc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      954 2023-05-12 14:49:16.000000 glance_store-4.4.0/glance_store/tests/etc/glance-swift.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      834 2023-05-12 14:49:16.000000 glance_store-4.4.0/glance_store/tests/fakes.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:50:07.592552 glance_store-4.4.0/glance_store/tests/functional/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2909 2023-05-12 14:49:16.000000 glance_store-4.4.0/glance_store/tests/functional/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:49:16.000000 glance_store-4.4.0/glance_store/tests/functional/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3915 2023-05-12 14:49:16.000000 glance_store-4.4.0/glance_store/tests/functional/base.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:50:07.592552 glance_store-4.4.0/glance_store/tests/functional/filesystem/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:49:16.000000 glance_store-4.4.0/glance_store/tests/functional/filesystem/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1359 2023-05-12 14:49:16.000000 glance_store-4.4.0/glance_store/tests/functional/filesystem/test_functional_filesystem.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:50:07.592552 glance_store-4.4.0/glance_store/tests/functional/swift/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:49:16.000000 glance_store-4.4.0/glance_store/tests/functional/swift/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3228 2023-05-12 14:49:16.000000 glance_store-4.4.0/glance_store/tests/functional/swift/test_functional_swift.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:50:07.596552 glance_store-4.4.0/glance_store/tests/unit/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:49:16.000000 glance_store-4.4.0/glance_store/tests/unit/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:50:07.596552 glance_store-4.4.0/glance_store/tests/unit/cinder/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:49:16.000000 glance_store-4.4.0/glance_store/tests/unit/cinder/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4661 2023-05-12 14:49:16.000000 glance_store-4.4.0/glance_store/tests/unit/cinder/test_base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    41368 2023-05-12 14:49:16.000000 glance_store-4.4.0/glance_store/tests/unit/cinder/test_cinder_base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6764 2023-05-12 14:49:16.000000 glance_store-4.4.0/glance_store/tests/unit/cinder/test_cinder_store.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12926 2023-05-12 14:49:16.000000 glance_store-4.4.0/glance_store/tests/unit/cinder/test_multistore_cinder.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3933 2023-05-12 14:49:16.000000 glance_store-4.4.0/glance_store/tests/unit/cinder/test_nfs.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1849 2023-05-12 14:49:16.000000 glance_store-4.4.0/glance_store/tests/unit/cinder/test_scaleio.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:50:07.596552 glance_store-4.4.0/glance_store/tests/unit/common/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:49:16.000000 glance_store-4.4.0/glance_store/tests/unit/common/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4716 2023-05-12 14:49:16.000000 glance_store-4.4.0/glance_store/tests/unit/common/test_attachment_state_manager.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7621 2023-05-12 14:49:16.000000 glance_store-4.4.0/glance_store/tests/unit/common/test_cinder_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5763 2023-05-12 14:49:16.000000 glance_store-4.4.0/glance_store/tests/unit/common/test_fs_mount.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1144 2023-05-12 14:49:16.000000 glance_store-4.4.0/glance_store/tests/unit/common/test_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5862 2023-05-12 14:49:16.000000 glance_store-4.4.0/glance_store/tests/unit/test_backend.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8014 2023-05-12 14:49:16.000000 glance_store-4.4.0/glance_store/tests/unit/test_connection_manager.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16806 2023-05-12 14:49:16.000000 glance_store-4.4.0/glance_store/tests/unit/test_driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2223 2023-05-12 14:49:16.000000 glance_store-4.4.0/glance_store/tests/unit/test_exceptions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    35512 2023-05-12 14:49:16.000000 glance_store-4.4.0/glance_store/tests/unit/test_filesystem_store.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8581 2023-05-12 14:49:16.000000 glance_store-4.4.0/glance_store/tests/unit/test_http_store.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1204 2023-05-12 14:49:16.000000 glance_store-4.4.0/glance_store/tests/unit/test_location.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    35205 2023-05-12 14:49:16.000000 glance_store-4.4.0/glance_store/tests/unit/test_multistore_filesystem.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17509 2023-05-12 14:49:16.000000 glance_store-4.4.0/glance_store/tests/unit/test_multistore_rbd.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    24725 2023-05-12 14:49:16.000000 glance_store-4.4.0/glance_store/tests/unit/test_multistore_s3.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    29875 2023-05-12 14:49:16.000000 glance_store-4.4.0/glance_store/tests/unit/test_multistore_vmware.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5643 2023-05-12 14:49:16.000000 glance_store-4.4.0/glance_store/tests/unit/test_opts.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    28572 2023-05-12 14:49:16.000000 glance_store-4.4.0/glance_store/tests/unit/test_rbd_store.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    23476 2023-05-12 14:49:16.000000 glance_store-4.4.0/glance_store/tests/unit/test_s3_store.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3408 2023-05-12 14:49:16.000000 glance_store-4.4.0/glance_store/tests/unit/test_store_base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6435 2023-05-12 14:49:16.000000 glance_store-4.4.0/glance_store/tests/unit/test_store_capabilities.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   101249 2023-05-12 14:49:16.000000 glance_store-4.4.0/glance_store/tests/unit/test_swift_store.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    97793 2023-05-12 14:49:16.000000 glance_store-4.4.0/glance_store/tests/unit/test_swift_store_multibackend.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6319 2023-05-12 14:49:16.000000 glance_store-4.4.0/glance_store/tests/unit/test_swift_store_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1349 2023-05-12 14:49:16.000000 glance_store-4.4.0/glance_store/tests/unit/test_test_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    30386 2023-05-12 14:49:16.000000 glance_store-4.4.0/glance_store/tests/unit/test_vmware_store.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3780 2023-05-12 14:49:16.000000 glance_store-4.4.0/glance_store/tests/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:50:07.584552 glance_store-4.4.0/glance_store.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2727 2023-05-12 14:50:07.000000 glance_store-4.4.0/glance_store.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8355 2023-05-12 14:50:07.000000 glance_store-4.4.0/glance_store.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-05-12 14:50:07.000000 glance_store-4.4.0/glance_store.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1021 2023-05-12 14:50:07.000000 glance_store-4.4.0/glance_store.egg-info/entry_points.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-05-12 14:50:07.000000 glance_store-4.4.0/glance_store.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2023-05-12 14:50:07.000000 glance_store-4.4.0/glance_store.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      825 2023-05-12 14:50:07.000000 glance_store-4.4.0/glance_store.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       13 2023-05-12 14:50:07.000000 glance_store-4.4.0/glance_store.egg-info/top_level.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:50:07.572552 glance_store-4.4.0/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:50:07.608553 glance_store-4.4.0/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:49:16.000000 glance_store-4.4.0/releasenotes/notes/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      724 2023-05-12 14:49:16.000000 glance_store-4.4.0/releasenotes/notes/0.29.1-notes-ded2a1d473a306c7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1216 2023-05-12 14:49:16.000000 glance_store-4.4.0/releasenotes/notes/Stein_final_release-c7df5838028b8c7e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      176 2023-05-12 14:49:16.000000 glance_store-4.4.0/releasenotes/notes/block-creating-encrypted-nfs-volumes-d0ff370ab762042e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      302 2023-05-12 14:49:16.000000 glance_store-4.4.0/releasenotes/notes/bug-1620999-8b76a0ad14826197.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      437 2023-05-12 14:49:16.000000 glance_store-4.4.0/releasenotes/notes/bug-1820817-0ee70781918d232e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      238 2023-05-12 14:49:16.000000 glance_store-4.4.0/releasenotes/notes/bug-1915602-fcc807a435d8a6bf.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      444 2023-05-12 14:49:16.000000 glance_store-4.4.0/releasenotes/notes/bug-1954883-3666d63a3c0233f1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      451 2023-05-12 14:49:16.000000 glance_store-4.4.0/releasenotes/notes/bug-2004555-4fd67fce86c07461.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      165 2023-05-12 14:49:16.000000 glance_store-4.4.0/releasenotes/notes/cinder-fix-nfs-sparse-vol-create-76631ce05f86257c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      217 2023-05-12 14:49:16.000000 glance_store-4.4.0/releasenotes/notes/cinder-nfs-block-qcow2-vol-4fed58b0afafc980.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      398 2023-05-12 14:49:16.000000 glance_store-4.4.0/releasenotes/notes/cinder-support-extend-in-use-volume-c6292f950ff75cca.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      318 2023-05-12 14:49:16.000000 glance_store-4.4.0/releasenotes/notes/deprecate-rados_connect_timeout-767ed1eaa026196e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      546 2023-05-12 14:49:16.000000 glance_store-4.4.0/releasenotes/notes/deprecate-sheepdog-driver-1f9689c327f313d4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      797 2023-05-12 14:49:16.000000 glance_store-4.4.0/releasenotes/notes/deprecate-store_add_to_backend-f419e5c4210613d2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      680 2023-05-12 14:49:16.000000 glance_store-4.4.0/releasenotes/notes/deprecate-store_capabilities_update_min_interval-039389fa296e2494.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      209 2023-05-12 14:49:16.000000 glance_store-4.4.0/releasenotes/notes/drop-py-2-7-345cafc9c1d3f892.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      129 2023-05-12 14:49:16.000000 glance_store-4.4.0/releasenotes/notes/drop-python-3-6-and-3-7-41af87576c4fd7b1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      219 2023-05-12 14:49:16.000000 glance_store-4.4.0/releasenotes/notes/fix-exception-logging-during-attach-9546e24189db83c4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      249 2023-05-12 14:49:16.000000 glance_store-4.4.0/releasenotes/notes/fix-interval-in-retries-471155ff34d9f0e9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      225 2023-05-12 14:49:16.000000 glance_store-4.4.0/releasenotes/notes/fix-ip-in-connector-info-36b95d9959f10f63.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      215 2023-05-12 14:49:16.000000 glance_store-4.4.0/releasenotes/notes/fix-wait-device-resize-c282940b71a3748e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      124 2023-05-12 14:49:16.000000 glance_store-4.4.0/releasenotes/notes/fs-drv-chunk-sz-a1b2f6a72fad92d5.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      664 2023-05-12 14:49:16.000000 glance_store-4.4.0/releasenotes/notes/handle-sparse-image-a3ecfc4ae1c00d48.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1342 2023-05-12 14:49:16.000000 glance_store-4.4.0/releasenotes/notes/improved-configuration-options-3635b56aba3072c9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      485 2023-05-12 14:49:16.000000 glance_store-4.4.0/releasenotes/notes/lock_path-cef9d6f5f52c3211.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      201 2023-05-12 14:49:16.000000 glance_store-4.4.0/releasenotes/notes/move-rootwrap-config-f2cf435c548aab5c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      686 2023-05-12 14:49:16.000000 glance_store-4.4.0/releasenotes/notes/multi-store-0c004fc8aba2a25d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      385 2023-05-12 14:49:16.000000 glance_store-4.4.0/releasenotes/notes/multi-tenant-store-058b67ce5b7f3bd0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      379 2023-05-12 14:49:16.000000 glance_store-4.4.0/releasenotes/notes/multiattach-volume-handling-1a8446a64463f2cf.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      636 2023-05-12 14:49:16.000000 glance_store-4.4.0/releasenotes/notes/multihash-support-629e9cbc283a8b47.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2459 2023-05-12 14:49:16.000000 glance_store-4.4.0/releasenotes/notes/pike-relnote-9f547df14184d18c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      585 2023-05-12 14:49:16.000000 glance_store-4.4.0/releasenotes/notes/prevent-unauthorized-errors-ebb9cf2236595cd0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2561 2023-05-12 14:49:16.000000 glance_store-4.4.0/releasenotes/notes/queens-relnote-5fa2d009d9a9e458.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2096 2023-05-12 14:49:16.000000 glance_store-4.4.0/releasenotes/notes/release-1.0.0-7ab43e91523eb3c8.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      693 2023-05-12 14:49:16.000000 glance_store-4.4.0/releasenotes/notes/release-1.0.1-098b1487ac8cc9a1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1384 2023-05-12 14:49:16.000000 glance_store-4.4.0/releasenotes/notes/release-1.2.0-8d239f01cd8ff0bf.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      627 2023-05-12 14:49:16.000000 glance_store-4.4.0/releasenotes/notes/releasenote-0.17.0-efee3f557ea2096a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      353 2023-05-12 14:49:16.000000 glance_store-4.4.0/releasenotes/notes/remove-cinder-experimental-fbf9dea32c84dc9b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      218 2023-05-12 14:49:16.000000 glance_store-4.4.0/releasenotes/notes/remove-gridfs-driver-09286e27613b4353.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      693 2023-05-12 14:49:16.000000 glance_store-4.4.0/releasenotes/notes/remove-s3-driver-f432afa1f53ecdf8.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      300 2023-05-12 14:49:16.000000 glance_store-4.4.0/releasenotes/notes/remove-store-cap-update-min-interval-21fea4173ed4a09b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      429 2023-05-12 14:49:16.000000 glance_store-4.4.0/releasenotes/notes/rethinking-filesystem-access-5ab872fd0c0d27db.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      452 2023-05-12 14:49:16.000000 glance_store-4.4.0/releasenotes/notes/rocky-bugfixes-adefa8f47db16a2d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      242 2023-05-12 14:49:16.000000 glance_store-4.4.0/releasenotes/notes/set-documented-default-directory-for-filesystem-9b417a29416d3a94.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      625 2023-05-12 14:49:16.000000 glance_store-4.4.0/releasenotes/notes/sorted-drivers-for-configs-a905f07d3bf9c973.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       57 2023-05-12 14:49:16.000000 glance_store-4.4.0/releasenotes/notes/start-using-reno-73ef709807e37b74.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      347 2023-05-12 14:49:16.000000 glance_store-4.4.0/releasenotes/notes/support-cinder-multiple-stores-6cc8489f8f4f8ff3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      412 2023-05-12 14:49:16.000000 glance_store-4.4.0/releasenotes/notes/support-cinder-upload-c85849d9c88bbd7e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      443 2023-05-12 14:49:16.000000 glance_store-4.4.0/releasenotes/notes/support-cinder-user-domain-420c76053dd50534.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      221 2023-05-12 14:49:16.000000 glance_store-4.4.0/releasenotes/notes/support-s3-driver-a4158f9fa35931d5.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      195 2023-05-12 14:49:16.000000 glance_store-4.4.0/releasenotes/notes/update-stein-deprecations-3c2f6ffeab22b558.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      300 2023-05-12 14:49:16.000000 glance_store-4.4.0/releasenotes/notes/victoria-milestone-1-c1f9de5b90e8c326.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      316 2023-05-12 14:49:16.000000 glance_store-4.4.0/releasenotes/notes/vmware-store-requests-369485d2cfdb6175.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      530 2023-05-12 14:49:16.000000 glance_store-4.4.0/releasenotes/notes/volume-type-validation-check-011a400d7fb3b307.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      300 2023-05-12 14:49:16.000000 glance_store-4.4.0/releasenotes/notes/wallaby-final-release-00f0f851ff7d93ab.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      573 2023-05-12 14:49:16.000000 glance_store-4.4.0/releasenotes/notes/xena-final-release-3c6e19dfba43b40d.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:50:07.612553 glance_store-4.4.0/releasenotes/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-05-12 14:49:16.000000 glance_store-4.4.0/releasenotes/source/2023.1.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:50:07.612553 glance_store-4.4.0/releasenotes/source/_static/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:49:16.000000 glance_store-4.4.0/releasenotes/source/_static/.placeholder
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:50:07.612553 glance_store-4.4.0/releasenotes/source/_templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:49:16.000000 glance_store-4.4.0/releasenotes/source/_templates/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8972 2023-05-12 14:49:16.000000 glance_store-4.4.0/releasenotes/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      282 2023-05-12 14:49:16.000000 glance_store-4.4.0/releasenotes/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      146 2023-05-12 14:49:16.000000 glance_store-4.4.0/releasenotes/source/liberty.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:50:07.576552 glance_store-4.4.0/releasenotes/source/locale/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:50:07.576552 glance_store-4.4.0/releasenotes/source/locale/de/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:50:07.612553 glance_store-4.4.0/releasenotes/source/locale/de/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2551 2023-05-12 14:49:16.000000 glance_store-4.4.0/releasenotes/source/locale/de/LC_MESSAGES/releasenotes.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:50:07.576552 glance_store-4.4.0/releasenotes/source/locale/en_GB/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:50:07.612553 glance_store-4.4.0/releasenotes/source/locale/en_GB/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    58144 2023-05-12 14:49:16.000000 glance_store-4.4.0/releasenotes/source/locale/en_GB/LC_MESSAGES/releasenotes.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:50:07.576552 glance_store-4.4.0/releasenotes/source/locale/zh_CN/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:50:07.612553 glance_store-4.4.0/releasenotes/source/locale/zh_CN/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2420 2023-05-12 14:49:16.000000 glance_store-4.4.0/releasenotes/source/locale/zh_CN/LC_MESSAGES/releasenotes.po
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2023-05-12 14:49:16.000000 glance_store-4.4.0/releasenotes/source/mitaka.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2023-05-12 14:49:16.000000 glance_store-4.4.0/releasenotes/source/newton.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2023-05-12 14:49:16.000000 glance_store-4.4.0/releasenotes/source/ocata.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2023-05-12 14:49:16.000000 glance_store-4.4.0/releasenotes/source/pike.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2023-05-12 14:49:16.000000 glance_store-4.4.0/releasenotes/source/queens.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-05-12 14:49:16.000000 glance_store-4.4.0/releasenotes/source/rocky.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-05-12 14:49:16.000000 glance_store-4.4.0/releasenotes/source/stein.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2023-05-12 14:49:16.000000 glance_store-4.4.0/releasenotes/source/train.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2023-05-12 14:49:16.000000 glance_store-4.4.0/releasenotes/source/unreleased.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-05-12 14:49:16.000000 glance_store-4.4.0/releasenotes/source/ussuri.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2023-05-12 14:49:16.000000 glance_store-4.4.0/releasenotes/source/victoria.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2023-05-12 14:49:16.000000 glance_store-4.4.0/releasenotes/source/wallaby.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-05-12 14:49:16.000000 glance_store-4.4.0/releasenotes/source/xena.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-05-12 14:49:16.000000 glance_store-4.4.0/releasenotes/source/yoga.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2023-05-12 14:49:16.000000 glance_store-4.4.0/releasenotes/source/zed.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      594 2023-05-12 14:49:16.000000 glance_store-4.4.0/requirements.txt
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     7157 2023-05-12 14:49:16.000000 glance_store-4.4.0/run_tests.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2345 2023-05-12 14:50:07.616553 glance_store-4.4.0/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2023-05-12 14:49:16.000000 glance_store-4.4.0/setup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      935 2023-05-12 14:49:16.000000 glance_store-4.4.0/test-requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-12 14:50:07.612553 glance_store-4.4.0/tools/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11648 2023-05-12 14:49:16.000000 glance_store-4.4.0/tools/colorizer.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2348 2023-05-12 14:49:16.000000 glance_store-4.4.0/tools/install_venv.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5647 2023-05-12 14:49:16.000000 glance_store-4.4.0/tools/install_venv_common.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      218 2023-05-12 14:49:16.000000 glance_store-4.4.0/tools/with_venv.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2098 2023-05-12 14:49:16.000000 glance_store-4.4.0/tox.ini
```

### Comparing `glance_store-4.3.0/.zuul.yaml` & `glance_store-4.4.0/.zuul.yaml`

 * *Files identical despite different names*

### Comparing `glance_store-4.3.0/AUTHORS` & `glance_store-4.4.0/AUTHORS`

 * *Files 2% similar despite different names*

```diff
@@ -109,14 +109,15 @@
 Stephen Finucane <stephenfin@redhat.com>
 Stuart McLaren <stuart.mclaren@hp.com>
 Stuart McLaren <stuart.​mclaren@hp.​com>
 Szymon Datko <szymon.datko@corp.ovh.com>
 Sławek Kapłoński <slawek@kaplonski.pl>
 THOMAS J. COCOZZELLO <tjcocozz@us.ibm.com>
 Takashi Kajinami <tkajinam@redhat.com>
+Takashi Natsume <takanattie@gmail.com>
 Taylor Peoples <tpeoples@us.ibm.com>
 Thomas Bechtold <tbechtold@suse.com>
 Tim Burke <tim.burke@gmail.com>
 Tom Cocozzello <tjcocozz@us.ibm.com>
 Tomoki Sekiyama <tomoki.sekiyama.qu@hitachi.com>
 Tomoki Sekiyama <tomoki.sekiyama@gmail.com>
 Tony Breeds <tony@bakeyournoodle.com>
@@ -124,19 +125,21 @@
 Victor Sergeyev <vsergeyev@mirantis.com>
 Victor Stinner <vstinner@redhat.com>
 Vikhyat Umrao <vumrao@redhat.com>
 Vincent Untz <vuntz@suse.com>
 Vladislav Kuzmin <vkuzmin@mirantis.com>
 Weijin Wang <wiwang@vmware.com>
 XiaojueGuan <guanalbertjone@gmail.com>
+Xinxin Shen <shenxinxin@inspur.com>
 XinxinShen <shenxinxin@inspur.com>
 YAMADA Hideki <yamada.hideki@lab.ntt.co.jp>
 Yu Shengzuo <yu.shengzuo@99cloud.net>
 Zhi Yan Liu <zhiyanl@cn.ibm.com>
 Zoltan Arnold Nagy <nag@zurich.ibm.com>
+anguoming <agm_daydayup@foxmail.com>
 ankitagrawal <ankit11.agrawal@nttdata.com>
 asmita singh <asmita.singh@nttdata.com>
 caoyuan <cao.yuan@99cloud.net>
 chenjiao <chenjiao@inspur.com>
 gengchc2 <geng.changcai2@zte.com.cn>
 hgangwx@cn.ibm.com <hgangwx@cn.ibm.com>
 kairat_kushaev <kkushaev@mirantis.com>
```

### Comparing `glance_store-4.3.0/ChangeLog` & `glance_store-4.4.0/ChangeLog`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,28 @@
 CHANGES
 =======
 
+4.4.0
+-----
+
+* Add force to os-brick disconnect
+* Run cinder driver unit tests
+* RBD: Wrap RBD calls in native threads
+* Update master for stable/2023.1
+* Do not always import boto3
+* rbd: Disable rbd stores if libraries are not available
+* cinder: Disable cinder stores if cinderclient is not installed
+* move attachment\_update to try block
+* Fix misuse of assertTrue
+* Imported Translations from Zanata
+
 4.3.0
 -----
 
+* Replace deprecated UPPER\_CONSTRAINTS\_FILE variable
 * Imported Translations from Zanata
 * Cinder: Add support to extend attached volumes
 * Refactor/restructure glance cinder store
 
 4.2.0
 -----
```

### Comparing `glance_store-4.3.0/LICENSE` & `glance_store-4.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `glance_store-4.3.0/PKG-INFO` & `glance_store-4.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glance_store
-Version: 4.3.0
+Version: 4.4.0
 Summary: OpenStack Image Service Store Library
 Home-page: https://docs.openstack.org/glance_store/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ========================
         Team and repository tags
```

### Comparing `glance_store-4.3.0/README.rst` & `glance_store-4.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `glance_store-4.3.0/doc/source/conf.py` & `glance_store-4.4.0/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.3.0/doc/source/index.rst` & `glance_store-4.4.0/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `glance_store-4.3.0/doc/source/user/drivers.rst` & `glance_store-4.4.0/doc/source/user/drivers.rst`

 * *Files identical despite different names*

### Comparing `glance_store-4.3.0/etc/glance/rootwrap.conf` & `glance_store-4.4.0/etc/glance/rootwrap.conf`

 * *Files identical despite different names*

### Comparing `glance_store-4.3.0/etc/glance/rootwrap.d/glance_cinder_store.filters` & `glance_store-4.4.0/etc/glance/rootwrap.d/glance_cinder_store.filters`

 * *Files identical despite different names*

### Comparing `glance_store-4.3.0/glance_store/__init__.py` & `glance_store-4.4.0/glance_store/__init__.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.3.0/glance_store/_drivers/cinder/__init__.py` & `glance_store-4.4.0/glance_store/_drivers/cinder/__init__.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.3.0/glance_store/_drivers/cinder/base.py` & `glance_store-4.4.0/glance_store/_drivers/cinder/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -46,15 +46,16 @@
             conn=self.connection_info, use_multipath=self.use_multipath)
 
     def connect_volume(self, volume):
         device = self.conn.connect_volume(self.connection_info)
         return device
 
     def disconnect_volume(self, device):
-        self.conn.disconnect_volume(self.connection_info, device)
+        # Bug #2004555: use force so there aren't any leftovers
+        self.conn.disconnect_volume(self.connection_info, device, force=True)
 
     def extend_volume(self):
         self.conn.extend_volume(self.connection_info)
 
     def yield_path(self, volume, volume_path):
         """
         This method returns the volume file path.
```

### Comparing `glance_store-4.3.0/glance_store/_drivers/cinder/nfs.py` & `glance_store-4.4.0/glance_store/_drivers/cinder/nfs.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.3.0/glance_store/_drivers/cinder/scaleio.py` & `glance_store-4.4.0/glance_store/_drivers/cinder/scaleio.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.3.0/glance_store/_drivers/cinder/store.py` & `glance_store-4.4.0/glance_store/_drivers/cinder/store.py`

 * *Files 1% similar despite different names*

```diff
@@ -510,14 +510,20 @@
             self._url_prefix = "cinder://%s" % self.backend_group
 
     def configure_add(self):
         """
         Check to verify if the volume types configured for the cinder store
         exist in deployment and if not, log a warning.
         """
+        if cinderclient is None:
+            reason = _("cinderclient is not available.")
+            LOG.error(reason)
+            raise exceptions.BadStoreConfiguration(store_name="cinder",
+                                                   reason=reason)
+
         cinder_volume_type = self.store_conf.cinder_volume_type
         if cinder_volume_type:
             # NOTE: `cinder_volume_type` is configured, check
             # configured volume_type is available in cinder or not
             cinder_client = self.get_cinderclient()
             try:
                 # We don't even need the volume type object, as long
@@ -718,42 +724,44 @@
                                                          host,
                                                          mode=attach_mode)
         else:
             attachment = self.volume_api.attachment_create(client, volume_id,
                                                            mode=attach_mode)
         LOG.debug('Attachment %(attachment_id)s created successfully.',
                   {'attachment_id': attachment['id']})
-        attachment = self.volume_api.attachment_update(
-            client, attachment['id'], connector_prop,
-            mountpoint='glance_store')
-        LOG.debug('Attachment %(attachment_id)s updated successfully with '
-                  'connection info %(conn_info)s',
-                  {'attachment_id': attachment.id,
-                   'conn_info': strutils.mask_dict_password(
-                       attachment.connection_info)})
-        volume = volume.manager.get(volume_id)
-        connection_info = attachment.connection_info
 
+        volume = volume.manager.get(volume_id)
+        attachment_id = attachment['id']
+        connection_info = None
         try:
+            attachment = self.volume_api.attachment_update(
+                client, attachment_id, connector_prop,
+                mountpoint='glance_store')
+            LOG.debug('Attachment %(attachment_id)s updated successfully with '
+                      'connection info %(conn_info)s',
+                      {'attachment_id': attachment_id,
+                       'conn_info': strutils.mask_dict_password(
+                           attachment.connection_info)})
+            connection_info = attachment.connection_info
             conn = base.factory(
                 connection_info['driver_volume_type'],
                 volume=volume,
                 connection_info=connection_info,
                 root_helper=root_helper,
                 use_multipath=use_multipath,
                 mountpoint_base=self.store_conf.cinder_mount_point_base,
                 attachment_obj=attachment,
                 client=client)
             device = conn.connect_volume(volume)
 
             # Complete the attachment (marking the volume "in-use") after
             # the connection with os-brick is complete
-            self.volume_api.attachment_complete(client, attachment.id)
+            self.volume_api.attachment_complete(client, attachment_id)
             LOG.debug('Attachment %(attachment_id)s completed successfully.',
-                      {'attachment_id': attachment.id})
+                      {'attachment_id': attachment_id})
 
             self.volume_connector_map[volume.id] = conn
             if (connection_info['driver_volume_type'] == 'rbd' and
                not conn.conn.do_local_attach):
                 yield device['path']
             else:
                 with self.temporary_chown(
@@ -764,27 +772,27 @@
                               '%(volume_id)s.'), {'volume_id': volume.id})
             raise
         finally:
             if device:
                 try:
                     if volume.multiattach:
                         attachment_state_manager.detach(
-                            client, attachment.id, volume_id, host, conn,
+                            client, attachment_id, volume_id, host, conn,
                             connection_info, device)
                     else:
                         conn.disconnect_volume(device)
                         if self.volume_connector_map.get(volume.id):
                             del self.volume_connector_map[volume.id]
                 except Exception:
                     LOG.exception(_LE('Failed to disconnect volume '
                                       '%(volume_id)s.'),
                                   {'volume_id': volume.id})
 
             if not volume.multiattach:
-                self.volume_api.attachment_delete(client, attachment.id)
+                self.volume_api.attachment_delete(client, attachment_id)
 
     def _cinder_volume_data_iterator(self, client, volume, max_size, offset=0,
                                      chunk_size=None, partial_length=None):
         chunk_size = chunk_size if chunk_size else self.READ_CHUNKSIZE
         partial = partial_length is not None
         with self._open_cinder_volume(client, volume, 'rb') as fp:
             if offset:
```

### Comparing `glance_store-4.3.0/glance_store/_drivers/filesystem.py` & `glance_store-4.4.0/glance_store/_drivers/filesystem.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.3.0/glance_store/_drivers/http.py` & `glance_store-4.4.0/glance_store/_drivers/http.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.3.0/glance_store/_drivers/rbd.py` & `glance_store-4.4.0/glance_store/_drivers/rbd.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
    (RADOS (Reliable Autonomic Distributed Object Store) Block Device)"""
 
 import contextlib
 import logging
 import math
 import urllib
 
+from eventlet import tpool
 from oslo_config import cfg
 from oslo_utils import encodeutils
 from oslo_utils import units
 
 from glance_store import capabilities
 from glance_store.common import utils
 from glance_store import driver
@@ -286,14 +287,17 @@
     OPTIONS = _RBD_OPTS
 
     EXAMPLE_URL = "rbd://<FSID>/<POOL>/<IMAGE>/<SNAP>"
 
     def get_schemes(self):
         return ('rbd',)
 
+    def RBDProxy(self):
+        return tpool.Proxy(rbd.RBD())
+
     @contextlib.contextmanager
     def get_connection(self, conffile, rados_id):
         client = rados.Rados(conffile=conffile, rados_id=rados_id)
 
         try:
             client.connect()
         except (rados.Error, rados.ObjectNotFound) as e:
@@ -314,14 +318,21 @@
     def configure_add(self):
         """
         Configure the Store to use the stored configuration options
         Any store that needs special configuration should implement
         this method. If the store was not able to successfully configure
         itself, it should raise `exceptions.BadStoreConfiguration`
         """
+        if rbd is None or rados is None:
+            reason = _("The required libraries(rbd and rados) are not "
+                       "available")
+            LOG.error(reason)
+            raise exceptions.BadStoreConfiguration(store_name='rbd',
+                                                   reason=reason)
+
         try:
             if self.backend_group:
                 chunk = getattr(self.conf,
                                 self.backend_group).rbd_store_chunk_size
                 pool = getattr(self.conf, self.backend_group).rbd_store_pool
                 user = getattr(self.conf, self.backend_group).rbd_store_user
                 conf_file = getattr(self.conf,
@@ -420,20 +431,20 @@
         make it a cloneable snapshot, so that copy-on-write
         volumes can be created from it.
 
         :param image_name: Image's name
 
         :returns: `glance_store.rbd.StoreLocation` object
         """
-        librbd = rbd.RBD()
         features = conn.conf_get('rbd_default_features')
         if ((features is None) or (int(features) == 0)):
             features = rbd.RBD_FEATURE_LAYERING
-        librbd.create(ioctx, image_name, size, order, old_format=False,
-                      features=int(features))
+        self.RBDProxy().create(ioctx, image_name, size, order,
+                               old_format=False,
+                               features=int(features))
         return StoreLocation({
             'fsid': fsid,
             'pool': self.pool,
             'image': image_name,
             'snapshot': DEFAULT_SNAPNAME,
         }, self.conf)
 
@@ -485,15 +496,15 @@
                                                "%(snap_exc)s "
                                                "Snapshot is in use.") %
                                            {'snap_exc': exc})
                                 LOG.warning(log_msg)
                                 raise exceptions.InUseByStore()
 
                     # Then delete image.
-                    rbd.RBD().remove(ioctx, image_name)
+                    self.RBDProxy().remove(ioctx, image_name)
                 except rbd.ImageHasSnapshots:
                     log_msg = (_LW("Remove image %(img_name)s failed. "
                                    "It has snapshot(s) left.") %
                                {'img_name': image_name})
                     LOG.warning(log_msg)
                     raise exceptions.HasSnapshot()
                 except rbd.ImageBusy:
```

### Comparing `glance_store-4.3.0/glance_store/_drivers/s3.py` & `glance_store-4.4.0/glance_store/_drivers/s3.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,18 +17,25 @@
 
 import io
 import logging
 import math
 import re
 import urllib
 
-from boto3 import session as boto_session
-from botocore import client as boto_client
-from botocore import exceptions as boto_exceptions
-from botocore import utils as boto_utils
+try:
+    from boto3 import session as boto_session
+    from botocore import client as boto_client
+    from botocore import exceptions as boto_exceptions
+    from botocore import utils as boto_utils
+except ImportError:
+    boto_session = None
+    boto_client = None
+    boto_exceptions = None
+    boto_utils = None
+
 import eventlet
 from oslo_config import cfg
 from oslo_utils import encodeutils
 from oslo_utils import units
 
 import glance_store
 from glance_store import capabilities
@@ -386,14 +393,20 @@
     def configure_add(self):
         """
         Configure the Store to use the stored configuration options
         Any store that needs special configuration should implement
         this method. If the store was not able to successfully configure
         itself, it should raise `exceptions.BadStoreConfiguration`
         """
+        if boto_session is None:
+            reason = _("boto3 or botocore is not available.")
+            LOG.error(reason)
+            raise exceptions.BadStoreConfiguration(store_name="s3",
+                                                   reason=reason)
+
         self.s3_host = self._option_get('s3_store_host')
         self.region_name = self._option_get('s3_store_region_name')
         self.access_key = self._option_get('s3_store_access_key')
         self.secret_key = self._option_get('s3_store_secret_key')
         self.bucket = self._option_get('s3_store_bucket')
 
         self.scheme = 's3'
```

### Comparing `glance_store-4.3.0/glance_store/_drivers/swift/__init__.py` & `glance_store-4.4.0/glance_store/_drivers/swift/__init__.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.3.0/glance_store/_drivers/swift/buffered.py` & `glance_store-4.4.0/glance_store/_drivers/swift/buffered.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.3.0/glance_store/_drivers/swift/connection_manager.py` & `glance_store-4.4.0/glance_store/_drivers/swift/connection_manager.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.3.0/glance_store/_drivers/swift/store.py` & `glance_store-4.4.0/glance_store/_drivers/swift/store.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.3.0/glance_store/_drivers/swift/utils.py` & `glance_store-4.4.0/glance_store/_drivers/swift/utils.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.3.0/glance_store/_drivers/vmware_datastore.py` & `glance_store-4.4.0/glance_store/_drivers/vmware_datastore.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.3.0/glance_store/backend.py` & `glance_store-4.4.0/glance_store/backend.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.3.0/glance_store/capabilities.py` & `glance_store-4.4.0/glance_store/capabilities.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.3.0/glance_store/common/attachment_state_manager.py` & `glance_store-4.4.0/glance_store/common/attachment_state_manager.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.3.0/glance_store/common/cinder_utils.py` & `glance_store-4.4.0/glance_store/common/cinder_utils.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.3.0/glance_store/common/fs_mount.py` & `glance_store-4.4.0/glance_store/common/fs_mount.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.3.0/glance_store/common/utils.py` & `glance_store-4.4.0/glance_store/common/utils.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.3.0/glance_store/driver.py` & `glance_store-4.4.0/glance_store/driver.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.3.0/glance_store/exceptions.py` & `glance_store-4.4.0/glance_store/exceptions.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.3.0/glance_store/i18n.py` & `glance_store-4.4.0/glance_store/i18n.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.3.0/glance_store/locale/en_GB/LC_MESSAGES/glance_store.po` & `glance_store-4.4.0/glance_store/locale/en_GB/LC_MESSAGES/glance_store.po`

 * *Files identical despite different names*

### Comparing `glance_store-4.3.0/glance_store/locale/ko_KR/LC_MESSAGES/glance_store.po` & `glance_store-4.4.0/glance_store/locale/ko_KR/LC_MESSAGES/glance_store.po`

 * *Files identical despite different names*

### Comparing `glance_store-4.3.0/glance_store/location.py` & `glance_store-4.4.0/glance_store/location.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.3.0/glance_store/multi_backend.py` & `glance_store-4.4.0/glance_store/multi_backend.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.3.0/glance_store/tests/base.py` & `glance_store-4.4.0/glance_store/tests/base.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.3.0/glance_store/tests/etc/glance-swift.conf` & `glance_store-4.4.0/glance_store/tests/etc/glance-swift.conf`

 * *Files identical despite different names*

### Comparing `glance_store-4.3.0/glance_store/tests/fakes.py` & `glance_store-4.4.0/glance_store/tests/fakes.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.3.0/glance_store/tests/functional/README.rst` & `glance_store-4.4.0/glance_store/tests/functional/README.rst`

 * *Files identical despite different names*

### Comparing `glance_store-4.3.0/glance_store/tests/functional/base.py` & `glance_store-4.4.0/glance_store/tests/functional/base.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.3.0/glance_store/tests/functional/filesystem/test_functional_filesystem.py` & `glance_store-4.4.0/glance_store/tests/functional/filesystem/test_functional_filesystem.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.3.0/glance_store/tests/functional/swift/test_functional_swift.py` & `glance_store-4.4.0/glance_store/tests/functional/swift/test_functional_swift.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.3.0/glance_store/tests/unit/cinder/test_base.py` & `glance_store-4.4.0/glance_store/tests/unit/cinder/test_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,15 +98,15 @@
         self.assertEqual(fake_path['path'], fake_dev_path['path'])
 
     def test_disconnect_volume(self):
         fake_device = 'fake_dev_path'
         self.mock_object(self.connector.conn, 'disconnect_volume')
         self.connector.disconnect_volume(fake_device)
         self.connector.conn.disconnect_volume.assert_called_once_with(
-            self.connection_info, fake_device)
+            self.connection_info, fake_device, force=True)
 
     def test_extend_volume(self):
         self.mock_object(self.connector.conn, 'extend_volume')
         self.connector.extend_volume()
         self.connector.conn.extend_volume.assert_called_once_with(
             self.connection_info)
```

### Comparing `glance_store-4.3.0/glance_store/tests/unit/cinder/test_cinder_base.py` & `glance_store-4.4.0/glance_store/tests/unit/cinder/test_cinder_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -203,15 +203,16 @@
                           volume_available, 'available', 'in-use')
         fake_manager.get.assert_called_with('fake-id')
 
     def _test_open_cinder_volume(self, open_mode, attach_mode, error,
                                  multipath_supported=False,
                                  enforce_multipath=False,
                                  encrypted_nfs=False, qcow2_vol=False,
-                                 multiattach=False):
+                                 multiattach=False,
+                                 update_attachment_error=None):
         fake_volume = mock.MagicMock(id=str(uuid.uuid4()), status='available',
                                      multiattach=multiattach)
         fake_volume.manager.get.return_value = fake_volume
         fake_attachment_id = str(uuid.uuid4())
         fake_attachment_create = {'id': fake_attachment_id}
         if encrypted_nfs or qcow2_vol:
             fake_attachment_update = mock.MagicMock(
@@ -280,14 +281,17 @@
                                   'attachment_complete') as attach_complete, \
                 mock.patch.object(socket,
                                   'gethostname') as mock_get_host, \
                 mock.patch.object(socket,
                                   'getaddrinfo') as mock_get_host_ip, \
                 mock.patch.object(cinder.strutils, 'mask_dict_password'):
 
+            if update_attachment_error:
+                attach_update.side_effect = update_attachment_error
+
             fake_host = 'fake_host'
             fake_addr_info = [[0, 1, 2, 3, ['127.0.0.1']]]
             fake_ip = fake_addr_info[0][4][0]
             mock_get_host.return_value = fake_host
             mock_get_host_ip.return_value = fake_addr_info
 
             with mock.patch.object(connector,
@@ -305,25 +309,30 @@
                     try:
                         with self.store._open_cinder_volume(
                                 fake_client, fake_volume, open_mode):
                             pass
                     except exceptions.BackendException:
                         attach_delete.assert_called_once_with(
                             fake_client, fake_attachment_id)
+                elif update_attachment_error:
+                    self.assertRaises(type(update_attachment_error), do_open)
                 else:
                     do_open()
-                if not (encrypted_nfs or qcow2_vol):
+                if update_attachment_error:
+                    attach_delete.assert_called_once_with(
+                        fake_client, fake_attachment_id)
+                elif not (encrypted_nfs or qcow2_vol):
                     mock_conn.assert_called_once_with(
                         root_helper, fake_ip,
                         multipath_supported, enforce_multipath,
                         host=fake_host)
                     fake_connector.connect_volume.assert_called_once_with(
                         mock.ANY)
                     fake_connector.disconnect_volume.assert_called_once_with(
-                        mock.ANY, fake_devinfo)
+                        mock.ANY, fake_devinfo, force=True)
                     fake_conn_obj.assert_called_once_with(
                         mock.ANY, root_helper, conn=mock.ANY,
                         use_multipath=multipath_supported)
                     attach_create.assert_called_once_with(
                         fake_client, fake_volume.id, mode=attach_mode)
                     attach_update.assert_called_once_with(
                         fake_client, fake_attachment_id,
@@ -349,16 +358,18 @@
 
     def test_open_cinder_volume_rw(self):
         self._test_open_cinder_volume('wb', 'rw', None)
 
     def test_open_cinder_volume_ro(self):
         self._test_open_cinder_volume('rb', 'ro', None)
 
-    def test_open_cinder_volume_error(self):
-        self._test_open_cinder_volume('wb', 'rw', IOError)
+    def test_open_cinder_volume_update_attachment_error(self):
+        err = Exception("update attachment fake error")
+        self._test_open_cinder_volume('rb', 'ro', None,
+                                      update_attachment_error=err)
 
     def test_open_cinder_volume_nfs_encrypted(self):
         self._test_open_cinder_volume('rb', 'ro', None, encrypted_nfs=True)
 
     def test_open_cinder_volume_nfs_qcow2_volume(self):
         self._test_open_cinder_volume('rb', 'ro', None, qcow2_vol=True)
```

### Comparing `glance_store-4.3.0/glance_store/tests/unit/cinder/test_cinder_store.py` & `glance_store-4.4.0/glance_store/tests/unit/cinder/test_cinder_store.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.3.0/glance_store/tests/unit/cinder/test_multistore_cinder.py` & `glance_store-4.4.0/glance_store/tests/unit/cinder/test_multistore_cinder.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.3.0/glance_store/tests/unit/cinder/test_nfs.py` & `glance_store-4.4.0/glance_store/tests/unit/cinder/test_nfs.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.3.0/glance_store/tests/unit/cinder/test_scaleio.py` & `glance_store-4.4.0/glance_store/tests/unit/cinder/test_scaleio.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.3.0/glance_store/tests/unit/common/test_attachment_state_manager.py` & `glance_store-4.4.0/glance_store/tests/unit/common/test_attachment_state_manager.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.3.0/glance_store/tests/unit/common/test_cinder_utils.py` & `glance_store-4.4.0/glance_store/tests/unit/common/test_cinder_utils.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.3.0/glance_store/tests/unit/common/test_fs_mount.py` & `glance_store-4.4.0/glance_store/tests/unit/common/test_fs_mount.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.3.0/glance_store/tests/unit/common/test_utils.py` & `glance_store-4.4.0/glance_store/tests/unit/common/test_utils.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.3.0/glance_store/tests/unit/test_backend.py` & `glance_store-4.4.0/glance_store/tests/unit/test_backend.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.3.0/glance_store/tests/unit/test_connection_manager.py` & `glance_store-4.4.0/glance_store/tests/unit/test_connection_manager.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.3.0/glance_store/tests/unit/test_driver.py` & `glance_store-4.4.0/glance_store/tests/unit/test_driver.py`

 * *Files 13% similar despite different names*

```diff
@@ -71,257 +71,257 @@
     def test_old_style_3_args(self):
         x = self.fake_store.add(self.img_id, self.img_file, self.img_size)
         self.assertEqual(tuple, type(x))
         self.assertEqual(4, len(x))
         self.assertIn(self.img_id, x[0])
         self.assertEqual(self.img_size, x[1])
         self.assertEqual(self.img_checksum, x[2])
-        self.assertTrue(dict, type(x[3]))
+        self.assertIsInstance(x[3], dict)
         self.assertIsNone(x[3]['context_obj'])
         self.assertIsNone(x[3]['verifier_obj'])
 
     def test_old_style_4_args(self):
         x = self.fake_store.add(self.img_id, self.img_file, self.img_size,
                                 self.fake_context)
         self.assertEqual(tuple, type(x))
         self.assertEqual(4, len(x))
         self.assertIn(self.img_id, x[0])
         self.assertEqual(self.img_size, x[1])
         self.assertEqual(self.img_checksum, x[2])
-        self.assertTrue(dict, type(x[3]))
+        self.assertIsInstance(x[3], dict)
         self.assertEqual('context', x[3]['context_obj'])
         self.assertIsNone(x[3]['verifier_obj'])
 
     def test_old_style_5_args(self):
         x = self.fake_store.add(self.img_id, self.img_file, self.img_size,
                                 self.fake_context, self.fake_verifier)
         self.assertEqual(tuple, type(x))
         self.assertEqual(4, len(x))
         self.assertIn(self.img_id, x[0])
         self.assertEqual(self.img_size, x[1])
         self.assertEqual(self.img_checksum, x[2])
-        self.assertTrue(dict, type(x[3]))
+        self.assertIsInstance(x[3], dict)
         self.assertEqual('context', x[3]['context_obj'])
         self.assertEqual('verifier', x[3]['verifier_obj'])
 
     def test_old_style_3_args_kw_context(self):
         x = self.fake_store.add(self.img_id, self.img_file, self.img_size,
                                 context=self.fake_context)
         self.assertEqual(tuple, type(x))
         self.assertEqual(4, len(x))
         self.assertIn(self.img_id, x[0])
         self.assertEqual(self.img_size, x[1])
         self.assertEqual(self.img_checksum, x[2])
-        self.assertTrue(dict, type(x[3]))
+        self.assertIsInstance(x[3], dict)
         self.assertEqual('context', x[3]['context_obj'])
         self.assertIsNone(x[3]['verifier_obj'])
 
     def test_old_style_3_args_kw_verifier(self):
         x = self.fake_store.add(self.img_id, self.img_file, self.img_size,
                                 verifier=self.fake_verifier)
         self.assertEqual(tuple, type(x))
         self.assertEqual(4, len(x))
         self.assertIn(self.img_id, x[0])
         self.assertEqual(self.img_size, x[1])
         self.assertEqual(self.img_checksum, x[2])
-        self.assertTrue(dict, type(x[3]))
+        self.assertIsInstance(x[3], dict)
         self.assertIsNone(x[3]['context_obj'])
         self.assertEqual('verifier', x[3]['verifier_obj'])
 
     def test_old_style_4_args_kw_verifier(self):
         x = self.fake_store.add(self.img_id, self.img_file, self.img_size,
                                 self.fake_context, verifier=self.fake_verifier)
         self.assertEqual(tuple, type(x))
         self.assertEqual(4, len(x))
         self.assertIn(self.img_id, x[0])
         self.assertEqual(self.img_size, x[1])
         self.assertEqual(self.img_checksum, x[2])
-        self.assertTrue(dict, type(x[3]))
+        self.assertIsInstance(x[3], dict)
         self.assertEqual('context', x[3]['context_obj'])
         self.assertEqual('verifier', x[3]['verifier_obj'])
 
     def test_old_style_3_args_kws_context_verifier(self):
         x = self.fake_store.add(self.img_id, self.img_file, self.img_size,
                                 context=self.fake_context,
                                 verifier=self.fake_verifier)
         self.assertEqual(tuple, type(x))
         self.assertEqual(4, len(x))
         self.assertIn(self.img_id, x[0])
         self.assertEqual(self.img_size, x[1])
         self.assertEqual(self.img_checksum, x[2])
-        self.assertTrue(dict, type(x[3]))
+        self.assertIsInstance(x[3], dict)
         self.assertEqual('context', x[3]['context_obj'])
         self.assertEqual('verifier', x[3]['verifier_obj'])
 
     def test_old_style_all_kw_in_order(self):
         x = self.fake_store.add(image_id=self.img_id,
                                 image_file=self.img_file,
                                 image_size=self.img_size,
                                 context=self.fake_context,
                                 verifier=self.fake_verifier)
         self.assertEqual(tuple, type(x))
         self.assertEqual(4, len(x))
         self.assertIn(self.img_id, x[0])
         self.assertEqual(self.img_size, x[1])
         self.assertEqual(self.img_checksum, x[2])
-        self.assertTrue(dict, type(x[3]))
+        self.assertIsInstance(x[3], dict)
         self.assertEqual('context', x[3]['context_obj'])
         self.assertEqual('verifier', x[3]['verifier_obj'])
 
     def test_old_style_all_kw_random_order(self):
         x = self.fake_store.add(image_file=self.img_file,
                                 context=self.fake_context,
                                 image_size=self.img_size,
                                 verifier=self.fake_verifier,
                                 image_id=self.img_id)
         self.assertEqual(tuple, type(x))
         self.assertEqual(4, len(x))
         self.assertIn(self.img_id, x[0])
         self.assertEqual(self.img_size, x[1])
         self.assertEqual(self.img_checksum, x[2])
-        self.assertTrue(dict, type(x[3]))
+        self.assertIsInstance(x[3], dict)
         self.assertEqual('context', x[3]['context_obj'])
         self.assertEqual('verifier', x[3]['verifier_obj'])
 
     def test_new_style_6_args(self):
         x = self.fake_store.add(self.img_id, self.img_file, self.img_size,
                                 self.hashing_algo, self.fake_context,
                                 self.fake_verifier)
         self.assertEqual(tuple, type(x))
         self.assertEqual(5, len(x))
         self.assertIn(self.img_id, x[0])
         self.assertEqual(self.img_size, x[1])
         self.assertEqual(self.img_checksum, x[2])
         self.assertEqual(self.img_sha256, x[3])
-        self.assertTrue(dict, type(x[4]))
+        self.assertIsInstance(x[4], dict)
         self.assertEqual('context', x[4]['context_obj'])
         self.assertEqual('verifier', x[4]['verifier_obj'])
 
     def test_new_style_3_args_kw_hash(self):
         x = self.fake_store.add(self.img_id, self.img_file, self.img_size,
                                 hashing_algo=self.hashing_algo)
         self.assertEqual(tuple, type(x))
         self.assertEqual(5, len(x))
         self.assertIn(self.img_id, x[0])
         self.assertEqual(self.img_size, x[1])
         self.assertEqual(self.img_checksum, x[2])
         self.assertEqual(self.img_sha256, x[3])
-        self.assertTrue(dict, type(x[4]))
+        self.assertIsInstance(x[4], dict)
         self.assertIsNone(x[4]['context_obj'])
         self.assertIsNone(x[4]['verifier_obj'])
 
     def test_new_style_3_args_kws_context_hash(self):
         x = self.fake_store.add(self.img_id, self.img_file, self.img_size,
                                 context=self.fake_context,
                                 hashing_algo=self.hashing_algo)
         self.assertEqual(tuple, type(x))
         self.assertEqual(5, len(x))
         self.assertIn(self.img_id, x[0])
         self.assertEqual(self.img_size, x[1])
         self.assertEqual(self.img_checksum, x[2])
         self.assertEqual(self.img_sha256, x[3])
-        self.assertTrue(dict, type(x[4]))
+        self.assertIsInstance(x[4], dict)
         self.assertEqual('context', x[4]['context_obj'])
         self.assertIsNone(x[4]['verifier_obj'])
 
     def test_new_style_3_args_kws_verifier_hash(self):
         x = self.fake_store.add(self.img_id, self.img_file, self.img_size,
                                 hashing_algo=self.hashing_algo,
                                 verifier=self.fake_verifier)
         self.assertEqual(tuple, type(x))
         self.assertEqual(5, len(x))
         self.assertIn(self.img_id, x[0])
         self.assertEqual(self.img_size, x[1])
         self.assertEqual(self.img_checksum, x[2])
         self.assertEqual(self.img_sha256, x[3])
-        self.assertTrue(dict, type(x[4]))
+        self.assertIsInstance(x[4], dict)
         self.assertIsNone(x[4]['context_obj'])
         self.assertEqual('verifier', x[4]['verifier_obj'])
 
     def test_new_style_3_args_kws_hash_context_verifier(self):
         x = self.fake_store.add(self.img_id, self.img_file, self.img_size,
                                 hashing_algo=self.hashing_algo,
                                 context=self.fake_context,
                                 verifier=self.fake_verifier)
         self.assertEqual(tuple, type(x))
         self.assertEqual(5, len(x))
         self.assertIn(self.img_id, x[0])
         self.assertEqual(self.img_size, x[1])
         self.assertEqual(self.img_checksum, x[2])
         self.assertEqual(self.img_sha256, x[3])
-        self.assertTrue(dict, type(x[4]))
+        self.assertIsInstance(x[4], dict)
         self.assertEqual('context', x[4]['context_obj'])
         self.assertEqual('verifier', x[4]['verifier_obj'])
 
     def test_new_style_4_args(self):
         x = self.fake_store.add(self.img_id, self.img_file, self.img_size,
                                 self.hashing_algo)
         self.assertEqual(tuple, type(x))
         self.assertEqual(5, len(x))
         self.assertIn(self.img_id, x[0])
         self.assertEqual(self.img_size, x[1])
         self.assertEqual(self.img_checksum, x[2])
         self.assertEqual(self.img_sha256, x[3])
-        self.assertTrue(dict, type(x[4]))
+        self.assertIsInstance(x[4], dict)
         self.assertIsNone(x[4]['context_obj'])
         self.assertIsNone(x[4]['verifier_obj'])
 
     def test_new_style_4_args_kw_context(self):
         x = self.fake_store.add(self.img_id, self.img_file, self.img_size,
                                 self.hashing_algo, context=self.fake_context)
         self.assertEqual(tuple, type(x))
         self.assertEqual(5, len(x))
         self.assertIn(self.img_id, x[0])
         self.assertEqual(self.img_size, x[1])
         self.assertEqual(self.img_checksum, x[2])
         self.assertEqual(self.img_sha256, x[3])
-        self.assertTrue(dict, type(x[4]))
+        self.assertIsInstance(x[4], dict)
         self.assertEqual('context', x[4]['context_obj'])
         self.assertIsNone(x[4]['verifier_obj'])
 
     def test_new_style_4_args_kws_verifier_context(self):
         x = self.fake_store.add(self.img_id, self.img_file, self.img_size,
                                 self.hashing_algo,
                                 context=self.fake_context,
                                 verifier=self.fake_verifier)
         self.assertEqual(tuple, type(x))
         self.assertEqual(5, len(x))
         self.assertIn(self.img_id, x[0])
         self.assertEqual(self.img_size, x[1])
         self.assertEqual(self.img_checksum, x[2])
         self.assertEqual(self.img_sha256, x[3])
-        self.assertTrue(dict, type(x[4]))
+        self.assertIsInstance(x[4], dict)
         self.assertEqual('context', x[4]['context_obj'])
         self.assertEqual('verifier', x[4]['verifier_obj'])
 
     def test_new_style_5_args_kw_verifier(self):
         x = self.fake_store.add(self.img_id, self.img_file, self.img_size,
                                 self.hashing_algo, self.fake_context,
                                 verifier=self.fake_verifier)
         self.assertEqual(tuple, type(x))
         self.assertEqual(5, len(x))
         self.assertIn(self.img_id, x[0])
         self.assertEqual(self.img_size, x[1])
         self.assertEqual(self.img_checksum, x[2])
         self.assertEqual(self.img_sha256, x[3])
-        self.assertTrue(dict, type(x[4]))
+        self.assertIsInstance(x[4], dict)
         self.assertEqual('context', x[4]['context_obj'])
         self.assertEqual('verifier', x[4]['verifier_obj'])
 
     def test_new_style_6_args_no_kw(self):
         x = self.fake_store.add(self.img_id, self.img_file, self.img_size,
                                 self.hashing_algo, self.fake_context,
                                 self.fake_verifier)
         self.assertEqual(tuple, type(x))
         self.assertEqual(5, len(x))
         self.assertIn(self.img_id, x[0])
         self.assertEqual(self.img_size, x[1])
         self.assertEqual(self.img_checksum, x[2])
         self.assertEqual(self.img_sha256, x[3])
-        self.assertTrue(dict, type(x[4]))
+        self.assertIsInstance(x[4], dict)
         self.assertEqual('context', x[4]['context_obj'])
         self.assertEqual('verifier', x[4]['verifier_obj'])
 
     def test_new_style_all_kw_in_order(self):
         x = self.fake_store.add(image_id=self.img_id,
                                 image_file=self.img_file,
                                 image_size=self.img_size,
@@ -330,15 +330,15 @@
                                 verifier=self.fake_verifier)
         self.assertEqual(tuple, type(x))
         self.assertEqual(5, len(x))
         self.assertIn(self.img_id, x[0])
         self.assertEqual(self.img_size, x[1])
         self.assertEqual(self.img_checksum, x[2])
         self.assertEqual(self.img_sha256, x[3])
-        self.assertTrue(dict, type(x[4]))
+        self.assertIsInstance(x[4], dict)
         self.assertEqual('context', x[4]['context_obj'])
         self.assertEqual('verifier', x[4]['verifier_obj'])
 
     def test_new_style_all_kw_random_order(self):
         x = self.fake_store.add(hashing_algo=self.hashing_algo,
                                 image_file=self.img_file,
                                 context=self.fake_context,
@@ -347,15 +347,15 @@
                                 image_id=self.img_id)
         self.assertEqual(tuple, type(x))
         self.assertEqual(5, len(x))
         self.assertIn(self.img_id, x[0])
         self.assertEqual(self.img_size, x[1])
         self.assertEqual(self.img_checksum, x[2])
         self.assertEqual(self.img_sha256, x[3])
-        self.assertTrue(dict, type(x[4]))
+        self.assertIsInstance(x[4], dict)
         self.assertEqual('context', x[4]['context_obj'])
         self.assertEqual('verifier', x[4]['verifier_obj'])
 
     def test_neg_too_few_args(self):
         self.assertRaises(TypeError,
                           self.fake_store.add,
                           self.img_id,
```

### Comparing `glance_store-4.3.0/glance_store/tests/unit/test_exceptions.py` & `glance_store-4.4.0/glance_store/tests/unit/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.3.0/glance_store/tests/unit/test_filesystem_store.py` & `glance_store-4.4.0/glance_store/tests/unit/test_filesystem_store.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.3.0/glance_store/tests/unit/test_http_store.py` & `glance_store-4.4.0/glance_store/tests/unit/test_http_store.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.3.0/glance_store/tests/unit/test_location.py` & `glance_store-4.4.0/glance_store/tests/unit/test_location.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.3.0/glance_store/tests/unit/test_multistore_filesystem.py` & `glance_store-4.4.0/glance_store/tests/unit/test_multistore_filesystem.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.3.0/glance_store/tests/unit/test_multistore_rbd.py` & `glance_store-4.4.0/glance_store/tests/unit/test_multistore_rbd.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.3.0/glance_store/tests/unit/test_multistore_s3.py` & `glance_store-4.4.0/glance_store/tests/unit/test_multistore_s3.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.3.0/glance_store/tests/unit/test_multistore_vmware.py` & `glance_store-4.4.0/glance_store/tests/unit/test_multistore_vmware.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.3.0/glance_store/tests/unit/test_opts.py` & `glance_store-4.4.0/glance_store/tests/unit/test_opts.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.3.0/glance_store/tests/unit/test_rbd_store.py` & `glance_store-4.4.0/glance_store/tests/unit/test_rbd_store.py`

 * *Files 10% similar despite different names*

```diff
@@ -688,7 +688,57 @@
         create_mock.assert_called_once_with(ioctxt, name, size, order,
                                             old_format=False, features=3)
 
     def tearDown(self):
         self.assertEqual(self.called_commands_expected,
                          self.called_commands_actual)
         super(TestStore, self).tearDown()
+
+    def test_create_image_in_native_thread(self):
+        # Tests that we use non-0 features from ceph.conf and cast to int.
+        fsid = 'fake'
+        features = '3'
+        conf_get_mock = mock.Mock(return_value=features)
+        conn = mock.Mock(conf_get=conf_get_mock)
+        ioctxt = mock.sentinel.ioctxt
+        name = '1'
+        size = 1024
+        order = 3
+        fake_proxy = mock.MagicMock()
+        fake_rbd = mock.MagicMock()
+
+        with mock.patch.object(rbd_store.tpool, 'Proxy') as tpool_mock, \
+                mock.patch.object(rbd_store.rbd, 'RBD') as rbd_mock:
+            tpool_mock.return_value = fake_proxy
+            rbd_mock.return_value = fake_rbd
+            location = self.store._create_image(
+                fsid, conn, ioctxt, name, size, order)
+            self.assertEqual(fsid, location.specs['fsid'])
+            self.assertEqual(rbd_store.DEFAULT_POOL, location.specs['pool'])
+            self.assertEqual(name, location.specs['image'])
+            self.assertEqual(rbd_store.DEFAULT_SNAPNAME,
+                             location.specs['snapshot'])
+
+        tpool_mock.assert_called_once_with(fake_rbd)
+        fake_proxy.create.assert_called_once_with(ioctxt, name, size, order,
+                                                  old_format=False, features=3)
+
+    def test_delete_image_in_native_thread(self):
+        fake_proxy = mock.MagicMock()
+        fake_rbd = mock.MagicMock()
+        fake_ioctx = mock.MagicMock()
+
+        with mock.patch.object(rbd_store.tpool, 'Proxy') as tpool_mock, \
+                mock.patch.object(rbd_store.rbd, 'RBD') as rbd_mock, \
+                mock.patch.object(self.store, 'get_connection') as mock_conn:
+
+            mock_get_conn = mock_conn.return_value.__enter__.return_value
+            mock_ioctx = mock_get_conn.open_ioctx.return_value.__enter__
+            mock_ioctx.return_value = fake_ioctx
+            tpool_mock.return_value = fake_proxy
+            rbd_mock.return_value = fake_rbd
+
+            self.store._delete_image('fake_pool', self.location.image)
+
+            tpool_mock.assert_called_once_with(fake_rbd)
+            fake_proxy.remove.assert_called_once_with(fake_ioctx,
+                                                      self.location.image)
```

### Comparing `glance_store-4.3.0/glance_store/tests/unit/test_s3_store.py` & `glance_store-4.4.0/glance_store/tests/unit/test_s3_store.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.3.0/glance_store/tests/unit/test_store_base.py` & `glance_store-4.4.0/glance_store/tests/unit/test_store_base.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.3.0/glance_store/tests/unit/test_store_capabilities.py` & `glance_store-4.4.0/glance_store/tests/unit/test_store_capabilities.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.3.0/glance_store/tests/unit/test_swift_store.py` & `glance_store-4.4.0/glance_store/tests/unit/test_swift_store.py`

 * *Files 0% similar despite different names*

```diff
@@ -2177,15 +2177,15 @@
 
     def tearDown(self):
         super(TestBufferedReader, self).tearDown()
         self.reader.__exit__(None, None, None)
 
     def test_buffer(self):
         self.reader.read(4)
-        self.assertTrue(self.reader._buffered, True)
+        self.assertTrue(self.reader._buffered)
 
         # test buffer position
         self.assertEqual(4, self.reader.tell())
 
         # also test buffer contents
         buf = self.reader._tmpfile
         buf.seek(0)
```

### Comparing `glance_store-4.3.0/glance_store/tests/unit/test_swift_store_multibackend.py` & `glance_store-4.4.0/glance_store/tests/unit/test_swift_store_multibackend.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.3.0/glance_store/tests/unit/test_swift_store_utils.py` & `glance_store-4.4.0/glance_store/tests/unit/test_swift_store_utils.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.3.0/glance_store/tests/unit/test_test_utils.py` & `glance_store-4.4.0/glance_store/tests/unit/test_test_utils.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.3.0/glance_store/tests/unit/test_vmware_store.py` & `glance_store-4.4.0/glance_store/tests/unit/test_vmware_store.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.3.0/glance_store/tests/utils.py` & `glance_store-4.4.0/glance_store/tests/utils.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.3.0/glance_store.egg-info/PKG-INFO` & `glance_store-4.4.0/glance_store.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glance-store
-Version: 4.3.0
+Version: 4.4.0
 Summary: OpenStack Image Service Store Library
 Home-page: https://docs.openstack.org/glance_store/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ========================
         Team and repository tags
```

### Comparing `glance_store-4.3.0/glance_store.egg-info/SOURCES.txt` & `glance_store-4.4.0/glance_store.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -87,14 +87,15 @@
 glance_store/tests/unit/test_store_base.py
 glance_store/tests/unit/test_store_capabilities.py
 glance_store/tests/unit/test_swift_store.py
 glance_store/tests/unit/test_swift_store_multibackend.py
 glance_store/tests/unit/test_swift_store_utils.py
 glance_store/tests/unit/test_test_utils.py
 glance_store/tests/unit/test_vmware_store.py
+glance_store/tests/unit/cinder/__init__.py
 glance_store/tests/unit/cinder/test_base.py
 glance_store/tests/unit/cinder/test_cinder_base.py
 glance_store/tests/unit/cinder/test_cinder_store.py
 glance_store/tests/unit/cinder/test_multistore_cinder.py
 glance_store/tests/unit/cinder/test_nfs.py
 glance_store/tests/unit/cinder/test_scaleio.py
 glance_store/tests/unit/common/__init__.py
@@ -106,14 +107,15 @@
 releasenotes/notes/0.29.1-notes-ded2a1d473a306c7.yaml
 releasenotes/notes/Stein_final_release-c7df5838028b8c7e.yaml
 releasenotes/notes/block-creating-encrypted-nfs-volumes-d0ff370ab762042e.yaml
 releasenotes/notes/bug-1620999-8b76a0ad14826197.yaml
 releasenotes/notes/bug-1820817-0ee70781918d232e.yaml
 releasenotes/notes/bug-1915602-fcc807a435d8a6bf.yaml
 releasenotes/notes/bug-1954883-3666d63a3c0233f1.yaml
+releasenotes/notes/bug-2004555-4fd67fce86c07461.yaml
 releasenotes/notes/cinder-fix-nfs-sparse-vol-create-76631ce05f86257c.yaml
 releasenotes/notes/cinder-nfs-block-qcow2-vol-4fed58b0afafc980.yaml
 releasenotes/notes/cinder-support-extend-in-use-volume-c6292f950ff75cca.yaml
 releasenotes/notes/deprecate-rados_connect_timeout-767ed1eaa026196e.yaml
 releasenotes/notes/deprecate-sheepdog-driver-1f9689c327f313d4.yaml
 releasenotes/notes/deprecate-store_add_to_backend-f419e5c4210613d2.yaml
 releasenotes/notes/deprecate-store_capabilities_update_min_interval-039389fa296e2494.yaml
@@ -154,14 +156,15 @@
 releasenotes/notes/support-s3-driver-a4158f9fa35931d5.yaml
 releasenotes/notes/update-stein-deprecations-3c2f6ffeab22b558.yaml
 releasenotes/notes/victoria-milestone-1-c1f9de5b90e8c326.yaml
 releasenotes/notes/vmware-store-requests-369485d2cfdb6175.yaml
 releasenotes/notes/volume-type-validation-check-011a400d7fb3b307.yaml
 releasenotes/notes/wallaby-final-release-00f0f851ff7d93ab.yaml
 releasenotes/notes/xena-final-release-3c6e19dfba43b40d.yaml
+releasenotes/source/2023.1.rst
 releasenotes/source/conf.py
 releasenotes/source/index.rst
 releasenotes/source/liberty.rst
 releasenotes/source/mitaka.rst
 releasenotes/source/newton.rst
 releasenotes/source/ocata.rst
 releasenotes/source/pike.rst
```

### Comparing `glance_store-4.3.0/glance_store.egg-info/entry_points.txt` & `glance_store-4.4.0/glance_store.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `glance_store-4.3.0/glance_store.egg-info/requires.txt` & `glance_store-4.4.0/glance_store.egg-info/requires.txt`

 * *Files 1% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 [swift]
 httplib2>=0.9.1
 python-swiftclient>=3.2.0
 
 [test]
 boto3>=1.9.199
 coverage!=4.4,>=4.0
+ddt>=1.4.4
 doc8>=0.6.0
 fixtures>=3.0.0
 hacking<3.1.0,>=3.0.1
 httplib2>=0.9.1
 os-brick>=2.6.0
 oslo.privsep>=1.23.0
 oslo.rootwrap>=5.8.0
```

### Comparing `glance_store-4.3.0/releasenotes/notes/0.29.1-notes-ded2a1d473a306c7.yaml` & `glance_store-4.4.0/releasenotes/notes/0.29.1-notes-ded2a1d473a306c7.yaml`

 * *Files identical despite different names*

### Comparing `glance_store-4.3.0/releasenotes/notes/Stein_final_release-c7df5838028b8c7e.yaml` & `glance_store-4.4.0/releasenotes/notes/Stein_final_release-c7df5838028b8c7e.yaml`

 * *Files identical despite different names*

### Comparing `glance_store-4.3.0/releasenotes/notes/deprecate-sheepdog-driver-1f9689c327f313d4.yaml` & `glance_store-4.4.0/releasenotes/notes/deprecate-sheepdog-driver-1f9689c327f313d4.yaml`

 * *Files identical despite different names*

### Comparing `glance_store-4.3.0/releasenotes/notes/deprecate-store_add_to_backend-f419e5c4210613d2.yaml` & `glance_store-4.4.0/releasenotes/notes/deprecate-store_add_to_backend-f419e5c4210613d2.yaml`

 * *Files identical despite different names*

### Comparing `glance_store-4.3.0/releasenotes/notes/deprecate-store_capabilities_update_min_interval-039389fa296e2494.yaml` & `glance_store-4.4.0/releasenotes/notes/deprecate-store_capabilities_update_min_interval-039389fa296e2494.yaml`

 * *Files identical despite different names*

### Comparing `glance_store-4.3.0/releasenotes/notes/handle-sparse-image-a3ecfc4ae1c00d48.yaml` & `glance_store-4.4.0/releasenotes/notes/handle-sparse-image-a3ecfc4ae1c00d48.yaml`

 * *Files identical despite different names*

### Comparing `glance_store-4.3.0/releasenotes/notes/improved-configuration-options-3635b56aba3072c9.yaml` & `glance_store-4.4.0/releasenotes/notes/improved-configuration-options-3635b56aba3072c9.yaml`

 * *Files identical despite different names*

### Comparing `glance_store-4.3.0/releasenotes/notes/multi-store-0c004fc8aba2a25d.yaml` & `glance_store-4.4.0/releasenotes/notes/multi-store-0c004fc8aba2a25d.yaml`

 * *Files identical despite different names*

### Comparing `glance_store-4.3.0/releasenotes/notes/multihash-support-629e9cbc283a8b47.yaml` & `glance_store-4.4.0/releasenotes/notes/multihash-support-629e9cbc283a8b47.yaml`

 * *Files identical despite different names*

### Comparing `glance_store-4.3.0/releasenotes/notes/pike-relnote-9f547df14184d18c.yaml` & `glance_store-4.4.0/releasenotes/notes/pike-relnote-9f547df14184d18c.yaml`

 * *Files identical despite different names*

### Comparing `glance_store-4.3.0/releasenotes/notes/prevent-unauthorized-errors-ebb9cf2236595cd0.yaml` & `glance_store-4.4.0/releasenotes/notes/prevent-unauthorized-errors-ebb9cf2236595cd0.yaml`

 * *Files identical despite different names*

### Comparing `glance_store-4.3.0/releasenotes/notes/queens-relnote-5fa2d009d9a9e458.yaml` & `glance_store-4.4.0/releasenotes/notes/queens-relnote-5fa2d009d9a9e458.yaml`

 * *Files identical despite different names*

### Comparing `glance_store-4.3.0/releasenotes/notes/release-1.0.0-7ab43e91523eb3c8.yaml` & `glance_store-4.4.0/releasenotes/notes/release-1.0.0-7ab43e91523eb3c8.yaml`

 * *Files identical despite different names*

### Comparing `glance_store-4.3.0/releasenotes/notes/release-1.0.1-098b1487ac8cc9a1.yaml` & `glance_store-4.4.0/releasenotes/notes/release-1.0.1-098b1487ac8cc9a1.yaml`

 * *Files identical despite different names*

### Comparing `glance_store-4.3.0/releasenotes/notes/release-1.2.0-8d239f01cd8ff0bf.yaml` & `glance_store-4.4.0/releasenotes/notes/release-1.2.0-8d239f01cd8ff0bf.yaml`

 * *Files identical despite different names*

### Comparing `glance_store-4.3.0/releasenotes/notes/releasenote-0.17.0-efee3f557ea2096a.yaml` & `glance_store-4.4.0/releasenotes/notes/releasenote-0.17.0-efee3f557ea2096a.yaml`

 * *Files identical despite different names*

### Comparing `glance_store-4.3.0/releasenotes/notes/remove-s3-driver-f432afa1f53ecdf8.yaml` & `glance_store-4.4.0/releasenotes/notes/remove-s3-driver-f432afa1f53ecdf8.yaml`

 * *Files identical despite different names*

### Comparing `glance_store-4.3.0/releasenotes/notes/sorted-drivers-for-configs-a905f07d3bf9c973.yaml` & `glance_store-4.4.0/releasenotes/notes/sorted-drivers-for-configs-a905f07d3bf9c973.yaml`

 * *Files identical despite different names*

### Comparing `glance_store-4.3.0/releasenotes/notes/volume-type-validation-check-011a400d7fb3b307.yaml` & `glance_store-4.4.0/releasenotes/notes/volume-type-validation-check-011a400d7fb3b307.yaml`

 * *Files identical despite different names*

### Comparing `glance_store-4.3.0/releasenotes/notes/xena-final-release-3c6e19dfba43b40d.yaml` & `glance_store-4.4.0/releasenotes/notes/xena-final-release-3c6e19dfba43b40d.yaml`

 * *Files identical despite different names*

### Comparing `glance_store-4.3.0/releasenotes/source/conf.py` & `glance_store-4.4.0/releasenotes/source/conf.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.3.0/releasenotes/source/locale/de/LC_MESSAGES/releasenotes.po` & `glance_store-4.4.0/releasenotes/source/locale/de/LC_MESSAGES/releasenotes.po`

 * *Files identical despite different names*

### Comparing `glance_store-4.3.0/releasenotes/source/locale/en_GB/LC_MESSAGES/releasenotes.po` & `glance_store-4.4.0/releasenotes/source/locale/en_GB/LC_MESSAGES/releasenotes.po`

 * *Files 1% similar despite different names*

```diff
@@ -6,19 +6,19 @@
 # Andi Chandler <andi@gowling.com>, 2021. #zanata
 # Andi Chandler <andi@gowling.com>, 2022. #zanata
 # Andi Chandler <andi@gowling.com>, 2023. #zanata
 msgid ""
 msgstr ""
 "Project-Id-Version: Glance_store Release Notes\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-02-03 12:21+0000\n"
+"POT-Creation-Date: 2023-02-09 16:32+0000\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"PO-Revision-Date: 2023-02-03 04:34+0000\n"
+"PO-Revision-Date: 2023-02-10 12:11+0000\n"
 "Last-Translator: Andi Chandler <andi@gowling.com>\n"
 "Language-Team: English (United Kingdom)\n"
 "Language: en_GB\n"
 "X-Generator: Zanata 4.3.3\n"
 "Plural-Forms: nplurals=2; plural=(n != 1)\n"
 
 msgid ""
@@ -121,16 +121,16 @@
 
 msgid "4.0.1"
 msgstr "4.0.1"
 
 msgid "4.1.0"
 msgstr "4.1.0"
 
-msgid "4.2.0-1"
-msgstr "4.2.0-1"
+msgid "4.2.0-5"
+msgstr "4.2.0-5"
 
 msgid ""
 "A `BufferedReader`_ has been added to the Swift store driver in order to "
 "enable better recovery from errors during uploads of large image files.  "
 "Because this reader buffers image data, it could cause Glance to use a much "
 "larger amount of disk space, and so the Buffered Reader is *not* enabled by "
 "default."
@@ -208,14 +208,27 @@
 "cinder store."
 msgstr ""
 "Added support for cinder multiple stores. Operators can now configure "
 "multiple cinder stores by configuring a unique cinder_volume_type for each "
 "Cinder store."
 
 msgid ""
+"Added support for extending in-use volumes in cinder store. A new boolean "
+"config option ``cinder_do_extend_attached`` is added which allows operators "
+"to enable/disable extending in-use volume support when creating an image. By "
+"default, ``cinder_do_extend_attached`` will be ``False`` i.e. old flow of "
+"detaching, extending and attaching will be used."
+msgstr ""
+"Added support for extending in-use volumes in Cinder store. A new boolean "
+"config option ``cinder_do_extend_attached`` is added which allows operators "
+"to enable/disable extending in-use volume support when creating an image. By "
+"default, ``cinder_do_extend_attached`` will be ``False`` i.e. old flow of "
+"detaching, extending and attaching will be used."
+
+msgid ""
 "Allow glance_store to refresh token when upload or download data to Swift "
 "store. glance_store identifies if token is going to expire soon when "
 "executing request to Swift and refresh the token. For multi-tenant swift "
 "store glance_store uses trusts, for single-tenant swift store glance_store "
 "uses credentials from swift store configurations. Please also note that this "
 "feature is enabled if and only if Keystone V3 API is available and enabled."
 msgstr ""
@@ -765,14 +778,25 @@
 "Swift backend now can use custom CA bundle to verify SSL connection to "
 "Keystone without adding this bundle to global system ones. For this it re-"
 "uses the CA bundle specified as ``swift_store_cacert`` config option, so "
 "this bundle must verify both certificates of Swift and Keystone API "
 "endpoints."
 
 msgid ""
+"The 'rados_connect_timeout' config option for the RBD store has been "
+"deprecated and will be removed in the future. It has been silently ignored "
+"for multiple releases. Users willing to set a timeout for the connection to "
+"the cluster can use Ceph's 'client_mount_timeout' option."
+msgstr ""
+"The 'rados_connect_timeout' config option for the RBD store has been "
+"deprecated and will be removed in the future. It has been silently ignored "
+"for multiple releases. Users willing to set a timeout for the connection to "
+"the cluster can use Ceph's 'client_mount_timeout' option."
+
+msgid ""
 "The 'stores' and 'default_store' configuration options have been deprecated "
 "for removal since the OpenStack Rocky release.  They are subject to removal "
 "early in the 'U' development cycle.  When these options are removed, the "
 "``glance_store.backend`` module, that depends on them, will be removed as "
 "well."
 msgstr ""
 "The 'stores' and 'default_store' configuration options have been deprecated "
```

### Comparing `glance_store-4.3.0/releasenotes/source/locale/zh_CN/LC_MESSAGES/releasenotes.po` & `glance_store-4.4.0/releasenotes/source/locale/zh_CN/LC_MESSAGES/releasenotes.po`

 * *Files identical despite different names*

### Comparing `glance_store-4.3.0/requirements.txt` & `glance_store-4.4.0/requirements.txt`

 * *Files identical despite different names*

### Comparing `glance_store-4.3.0/run_tests.sh` & `glance_store-4.4.0/run_tests.sh`

 * *Files identical despite different names*

### Comparing `glance_store-4.3.0/setup.cfg` & `glance_store-4.4.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `glance_store-4.3.0/setup.py` & `glance_store-4.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.3.0/test-requirements.txt` & `glance_store-4.4.0/test-requirements.txt`

 * *Files 10% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 # Documentation style
 doc8>=0.6.0 # Apache-2.0
 
 # Packaging
 
 # Unit testing
 coverage!=4.4,>=4.0 # Apache-2.0
+ddt>=1.4.4 # MIT
 fixtures>=3.0.0 # Apache-2.0/BSD
 python-subunit>=1.0.0 # Apache-2.0/BSD
 requests-mock>=1.2.0 # Apache-2.0
 retrying>=1.3.3
 stestr>=2.0.0 # Apache-2.0
 testscenarios>=0.4 # Apache-2.0/BSD
 testtools>=2.2.0 # MIT
```

### Comparing `glance_store-4.3.0/tools/colorizer.py` & `glance_store-4.4.0/tools/colorizer.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.3.0/tools/install_venv.py` & `glance_store-4.4.0/tools/install_venv.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.3.0/tools/install_venv_common.py` & `glance_store-4.4.0/tools/install_venv_common.py`

 * *Files identical despite different names*

### Comparing `glance_store-4.3.0/tox.ini` & `glance_store-4.4.0/tox.ini`

 * *Files 16% similar despite different names*

```diff
@@ -4,29 +4,29 @@
 ignore_basepython_conflict = True
 
 [testenv]
 basepython = python3
 setenv = VIRTUAL_ENV={envdir}
 usedevelop = True
 deps =
-   -c{env:UPPER_CONSTRAINTS_FILE:https://opendev.org/openstack/requirements/raw/branch/master/upper-constraints.txt}
+   -c{env:TOX_CONSTRAINTS_FILE:https://releases.openstack.org/constraints/upper/master}
    -r{toxinidir}/requirements.txt
    -r{toxinidir}/test-requirements.txt
 passenv = OS_TEST_*
 commands = stestr run --slowest {posargs}
 
 [testenv:docs]
 deps =
-   -c{env:UPPER_CONSTRAINTS_FILE:https://opendev.org/openstack/requirements/raw/branch/master/upper-constraints.txt}
+   -c{env:TOX_CONSTRAINTS_FILE:https://releases.openstack.org/constraints/upper/master}
    -r{toxinidir}/doc/requirements.txt
 commands = sphinx-build -W -b html doc/source doc/build/html
 
 [testenv:releasenotes]
 deps =
-   -c{env:UPPER_CONSTRAINTS_FILE:https://opendev.org/openstack/requirements/raw/branch/master/upper-constraints.txt}
+   -c{env:TOX_CONSTRAINTS_FILE:https://releases.openstack.org/constraints/upper/master}
    -r{toxinidir}/doc/requirements.txt
 commands = sphinx-build -a -E -W -d releasenotes/build/.doctrees -b html releasenotes/source releasenotes/build/html
 
 [testenv:pep8]
 commands =
   flake8 {posargs}
   doc8 {posargs}
```

