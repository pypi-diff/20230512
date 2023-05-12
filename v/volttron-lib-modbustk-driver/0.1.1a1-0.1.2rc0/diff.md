# Comparing `tmp/volttron_lib_modbustk_driver-0.1.1a1.tar.gz` & `tmp/volttron_lib_modbustk_driver-0.1.2rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "volttron_lib_modbustk_driver-0.1.1a1.tar", max compression
+gzip compressed data, was "volttron_lib_modbustk_driver-0.1.2rc0.tar", max compression
```

## Comparing `volttron_lib_modbustk_driver-0.1.1a1.tar` & `volttron_lib_modbustk_driver-0.1.2rc0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0    14453 2023-03-29 20:23:22.597655 volttron_lib_modbustk_driver-0.1.1a1/README.md
--rw-r--r--   0        0        0     1718 2023-03-29 20:25:23.985810 volttron_lib_modbustk_driver-0.1.1a1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-29 20:23:22.597655 volttron_lib_modbustk_driver-0.1.1a1/src/volttron/driver/interfaces/modbus_tk/__init__.py
--rw-r--r--   0        0        0    14591 2023-03-29 20:23:22.597655 volttron_lib_modbustk_driver-0.1.1a1/src/volttron/driver/interfaces/modbus_tk/modbus_tk.py
--rw-r--r--   0        0        0        0 2023-03-29 20:23:22.597655 volttron_lib_modbustk_driver-0.1.1a1/src/volttron/driver/interfaces/modbus_tk/utils/__init__.py
--rw-r--r--   0        0        0    29256 2023-03-29 20:23:22.597655 volttron_lib_modbustk_driver-0.1.1a1/src/volttron/driver/interfaces/modbus_tk/utils/client.py
--rw-r--r--   0        0        0    39596 2023-03-29 20:23:22.597655 volttron_lib_modbustk_driver-0.1.1a1/src/volttron/driver/interfaces/modbus_tk/utils/config_cmd.py
--rw-r--r--   0        0        0    10066 2023-03-29 20:23:22.597655 volttron_lib_modbustk_driver-0.1.1a1/src/volttron/driver/interfaces/modbus_tk/utils/helpers.py
--rw-r--r--   0        0        0    13035 2023-03-29 20:23:22.597655 volttron_lib_modbustk_driver-0.1.1a1/src/volttron/driver/interfaces/modbus_tk/utils/maps/__init__.py
--rw-r--r--   0        0        0     7097 2023-03-29 20:23:22.597655 volttron_lib_modbustk_driver-0.1.1a1/src/volttron/driver/interfaces/modbus_tk/utils/maps/battery_meter.csv
--rw-r--r--   0        0        0      635 2023-03-29 20:23:22.597655 volttron_lib_modbustk_driver-0.1.1a1/src/volttron/driver/interfaces/modbus_tk/utils/maps/ion6200.config
--rw-r--r--   0        0        0      361 2023-03-29 20:23:22.597655 volttron_lib_modbustk_driver-0.1.1a1/src/volttron/driver/interfaces/modbus_tk/utils/maps/ion6200.csv
--rw-r--r--   0        0        0     1431 2023-03-29 20:23:22.597655 volttron_lib_modbustk_driver-0.1.1a1/src/volttron/driver/interfaces/modbus_tk/utils/maps/ion6200_map.csv
--rw-r--r--   0        0        0      266 2023-03-29 20:23:22.597655 volttron_lib_modbustk_driver-0.1.1a1/src/volttron/driver/interfaces/modbus_tk/utils/maps/ion8600.csv
--rw-r--r--   0        0        0      563 2023-03-29 20:23:22.597655 volttron_lib_modbustk_driver-0.1.1a1/src/volttron/driver/interfaces/modbus_tk/utils/maps/ion8600_map.csv
--rw-r--r--   0        0        0     1436 2023-03-29 20:23:22.597655 volttron_lib_modbustk_driver-0.1.1a1/src/volttron/driver/interfaces/modbus_tk/utils/maps/maps.yaml
--rw-r--r--   0        0        0      359 2023-03-29 20:23:22.597655 volttron_lib_modbustk_driver-0.1.1a1/src/volttron/driver/interfaces/modbus_tk/utils/maps/mixed_endian_reg_map.csv
--rw-r--r--   0        0        0      645 2023-03-29 20:23:22.597655 volttron_lib_modbustk_driver-0.1.1a1/src/volttron/driver/interfaces/modbus_tk/utils/maps/modbus_tk_test.config
--rw-r--r--   0        0        0      262 2023-03-29 20:23:22.597655 volttron_lib_modbustk_driver-0.1.1a1/src/volttron/driver/interfaces/modbus_tk/utils/maps/modbus_tk_test.csv
--rw-r--r--   0        0        0      460 2023-03-29 20:23:22.597655 volttron_lib_modbustk_driver-0.1.1a1/src/volttron/driver/interfaces/modbus_tk/utils/maps/modbus_tk_test_map.csv
--rw-r--r--   0        0        0      341 2023-03-29 20:23:22.597655 volttron_lib_modbustk_driver-0.1.1a1/src/volttron/driver/interfaces/modbus_tk/utils/maps/scale_reg_map.csv
--rw-r--r--   0        0        0      368 2023-03-29 20:23:22.597655 volttron_lib_modbustk_driver-0.1.1a1/src/volttron/driver/interfaces/modbus_tk/utils/maps/scale_reg_pow_10_map.csv
--rw-r--r--   0        0        0      655 2023-03-29 20:23:22.597655 volttron_lib_modbustk_driver-0.1.1a1/src/volttron/driver/interfaces/modbus_tk/utils/maps/watts_on.config
--rw-r--r--   0        0        0      362 2023-03-29 20:23:22.597655 volttron_lib_modbustk_driver-0.1.1a1/src/volttron/driver/interfaces/modbus_tk/utils/maps/watts_on.csv
--rw-r--r--   0        0        0      414 2023-03-29 20:23:22.597655 volttron_lib_modbustk_driver-0.1.1a1/src/volttron/driver/interfaces/modbus_tk/utils/maps/watts_on_map.csv
--rw-r--r--   0        0        0      736 2023-03-29 20:23:22.597655 volttron_lib_modbustk_driver-0.1.1a1/src/volttron/driver/interfaces/modbus_tk/utils/maps/write_single_registers.config
--rw-r--r--   0        0        0       88 2023-03-29 20:23:22.597655 volttron_lib_modbustk_driver-0.1.1a1/src/volttron/driver/interfaces/modbus_tk/utils/maps/write_single_registers.csv
--rw-r--r--   0        0        0      149 2023-03-29 20:23:22.597655 volttron_lib_modbustk_driver-0.1.1a1/src/volttron/driver/interfaces/modbus_tk/utils/maps/write_single_registers_map.csv
--rw-r--r--   0        0        0    12145 2023-03-29 20:23:22.597655 volttron_lib_modbustk_driver-0.1.1a1/src/volttron/driver/interfaces/modbus_tk/utils/maps.py
--rw-r--r--   0        0        0    10891 2023-03-29 20:23:22.597655 volttron_lib_modbustk_driver-0.1.1a1/src/volttron/driver/interfaces/modbus_tk/utils/server.py
--rw-r--r--   0        0        0    15798 1970-01-01 00:00:00.000000 volttron_lib_modbustk_driver-0.1.1a1/setup.py
--rw-r--r--   0        0        0    15652 1970-01-01 00:00:00.000000 volttron_lib_modbustk_driver-0.1.1a1/PKG-INFO
+-rw-r--r--   0        0        0    11927 2023-05-12 16:54:03.174832 volttron_lib_modbustk_driver-0.1.2rc0/LICENSE
+-rw-r--r--   0        0        0    17194 2023-05-12 16:54:03.174832 volttron_lib_modbustk_driver-0.1.2rc0/README.md
+-rw-r--r--   0        0        0     1783 2023-05-12 16:55:35.095451 volttron_lib_modbustk_driver-0.1.2rc0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-12 16:54:03.178833 volttron_lib_modbustk_driver-0.1.2rc0/src/volttron/driver/interfaces/modbus_tk/__init__.py
+-rw-r--r--   0        0        0    14591 2023-05-12 16:54:03.178833 volttron_lib_modbustk_driver-0.1.2rc0/src/volttron/driver/interfaces/modbus_tk/modbus_tk.py
+-rw-r--r--   0        0        0        0 2023-05-12 16:54:03.178833 volttron_lib_modbustk_driver-0.1.2rc0/src/volttron/driver/interfaces/modbus_tk/utils/__init__.py
+-rw-r--r--   0        0        0    29256 2023-05-12 16:54:03.178833 volttron_lib_modbustk_driver-0.1.2rc0/src/volttron/driver/interfaces/modbus_tk/utils/client.py
+-rw-r--r--   0        0        0    39596 2023-05-12 16:54:03.178833 volttron_lib_modbustk_driver-0.1.2rc0/src/volttron/driver/interfaces/modbus_tk/utils/config_cmd.py
+-rw-r--r--   0        0        0    10066 2023-05-12 16:54:03.178833 volttron_lib_modbustk_driver-0.1.2rc0/src/volttron/driver/interfaces/modbus_tk/utils/helpers.py
+-rw-r--r--   0        0        0    13035 2023-05-12 16:54:03.178833 volttron_lib_modbustk_driver-0.1.2rc0/src/volttron/driver/interfaces/modbus_tk/utils/maps/__init__.py
+-rw-r--r--   0        0        0     7097 2023-05-12 16:54:03.178833 volttron_lib_modbustk_driver-0.1.2rc0/src/volttron/driver/interfaces/modbus_tk/utils/maps/battery_meter.csv
+-rw-r--r--   0        0        0      635 2023-05-12 16:54:03.178833 volttron_lib_modbustk_driver-0.1.2rc0/src/volttron/driver/interfaces/modbus_tk/utils/maps/ion6200.config
+-rw-r--r--   0        0        0      361 2023-05-12 16:54:03.178833 volttron_lib_modbustk_driver-0.1.2rc0/src/volttron/driver/interfaces/modbus_tk/utils/maps/ion6200.csv
+-rw-r--r--   0        0        0     1431 2023-05-12 16:54:03.178833 volttron_lib_modbustk_driver-0.1.2rc0/src/volttron/driver/interfaces/modbus_tk/utils/maps/ion6200_map.csv
+-rw-r--r--   0        0        0      266 2023-05-12 16:54:03.178833 volttron_lib_modbustk_driver-0.1.2rc0/src/volttron/driver/interfaces/modbus_tk/utils/maps/ion8600.csv
+-rw-r--r--   0        0        0      563 2023-05-12 16:54:03.178833 volttron_lib_modbustk_driver-0.1.2rc0/src/volttron/driver/interfaces/modbus_tk/utils/maps/ion8600_map.csv
+-rw-r--r--   0        0        0     1436 2023-05-12 16:54:03.178833 volttron_lib_modbustk_driver-0.1.2rc0/src/volttron/driver/interfaces/modbus_tk/utils/maps/maps.yaml
+-rw-r--r--   0        0        0      359 2023-05-12 16:54:03.178833 volttron_lib_modbustk_driver-0.1.2rc0/src/volttron/driver/interfaces/modbus_tk/utils/maps/mixed_endian_reg_map.csv
+-rw-r--r--   0        0        0      645 2023-05-12 16:54:03.178833 volttron_lib_modbustk_driver-0.1.2rc0/src/volttron/driver/interfaces/modbus_tk/utils/maps/modbus_tk_test.config
+-rw-r--r--   0        0        0      262 2023-05-12 16:54:03.178833 volttron_lib_modbustk_driver-0.1.2rc0/src/volttron/driver/interfaces/modbus_tk/utils/maps/modbus_tk_test.csv
+-rw-r--r--   0        0        0      460 2023-05-12 16:54:03.178833 volttron_lib_modbustk_driver-0.1.2rc0/src/volttron/driver/interfaces/modbus_tk/utils/maps/modbus_tk_test_map.csv
+-rw-r--r--   0        0        0      341 2023-05-12 16:54:03.178833 volttron_lib_modbustk_driver-0.1.2rc0/src/volttron/driver/interfaces/modbus_tk/utils/maps/scale_reg_map.csv
+-rw-r--r--   0        0        0      368 2023-05-12 16:54:03.178833 volttron_lib_modbustk_driver-0.1.2rc0/src/volttron/driver/interfaces/modbus_tk/utils/maps/scale_reg_pow_10_map.csv
+-rw-r--r--   0        0        0      655 2023-05-12 16:54:03.178833 volttron_lib_modbustk_driver-0.1.2rc0/src/volttron/driver/interfaces/modbus_tk/utils/maps/watts_on.config
+-rw-r--r--   0        0        0      362 2023-05-12 16:54:03.178833 volttron_lib_modbustk_driver-0.1.2rc0/src/volttron/driver/interfaces/modbus_tk/utils/maps/watts_on.csv
+-rw-r--r--   0        0        0      414 2023-05-12 16:54:03.178833 volttron_lib_modbustk_driver-0.1.2rc0/src/volttron/driver/interfaces/modbus_tk/utils/maps/watts_on_map.csv
+-rw-r--r--   0        0        0      736 2023-05-12 16:54:03.178833 volttron_lib_modbustk_driver-0.1.2rc0/src/volttron/driver/interfaces/modbus_tk/utils/maps/write_single_registers.config
+-rw-r--r--   0        0        0       88 2023-05-12 16:54:03.178833 volttron_lib_modbustk_driver-0.1.2rc0/src/volttron/driver/interfaces/modbus_tk/utils/maps/write_single_registers.csv
+-rw-r--r--   0        0        0      149 2023-05-12 16:54:03.178833 volttron_lib_modbustk_driver-0.1.2rc0/src/volttron/driver/interfaces/modbus_tk/utils/maps/write_single_registers_map.csv
+-rw-r--r--   0        0        0    12145 2023-05-12 16:54:03.178833 volttron_lib_modbustk_driver-0.1.2rc0/src/volttron/driver/interfaces/modbus_tk/utils/maps.py
+-rw-r--r--   0        0        0    10891 2023-05-12 16:54:03.178833 volttron_lib_modbustk_driver-0.1.2rc0/src/volttron/driver/interfaces/modbus_tk/utils/server.py
+-rw-r--r--   0        0        0    18295 1970-01-01 00:00:00.000000 volttron_lib_modbustk_driver-0.1.2rc0/PKG-INFO
```

### Comparing `volttron_lib_modbustk_driver-0.1.1a1/README.md` & `volttron_lib_modbustk_driver-0.1.2rc0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,904 +1,1075 @@
 00000000: 2320 766f 6c74 7472 6f6e 2d6c 6962 2d6d  # volttron-lib-m
 00000010: 6f64 6275 7374 6b2d 6472 6976 6572 0a0a  odbustk-driver..
-00000020: 215b 5061 7373 696e 673f 5d28 6874 7470  ![Passing?](http
-00000030: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f56  s://github.com/V
-00000040: 4f4c 5454 524f 4e2f 766f 6c74 7472 6f6e  OLTTRON/volttron
-00000050: 2d6c 6962 2d6d 6f64 6275 7374 6b2d 6472  -lib-modbustk-dr
-00000060: 6976 6572 2f61 6374 696f 6e73 2f77 6f72  iver/actions/wor
-00000070: 6b66 6c6f 7773 2f72 756e 2d74 6573 7473  kflows/run-tests
-00000080: 2e79 6d6c 2f62 6164 6765 2e73 7667 290a  .yml/badge.svg).
-00000090: 5b21 5b70 7970 6920 7665 7273 696f 6e5d  [![pypi version]
-000000a0: 2868 7474 7073 3a2f 2f69 6d67 2e73 6869  (https://img.shi
-000000b0: 656c 6473 2e69 6f2f 7079 7069 2f76 2f76  elds.io/pypi/v/v
-000000c0: 6f6c 7474 726f 6e2d 6c69 622d 6d6f 6462  olttron-lib-modb
-000000d0: 7573 746b 2d64 7269 7665 722e 7376 6729  ustk-driver.svg)
-000000e0: 5d28 6874 7470 733a 2f2f 7079 7069 2e6f  ](https://pypi.o
-000000f0: 7267 2f70 726f 6a65 6374 2f76 6f6c 7474  rg/project/voltt
-00000100: 726f 6e2d 6c69 622d 6d6f 6462 7573 746b  ron-lib-modbustk
-00000110: 2d64 7269 7665 722f 290a 0a56 4f4c 5454  -driver/)..VOLTT
-00000120: 524f 4ee2 8099 7320 4d6f 6462 7573 2d54  RON...s Modbus-T
-00000130: 4b20 6472 6976 6572 2c20 6275 696c 7420  K driver, built 
-00000140: 6f6e 2074 6865 2050 7974 686f 6e20 4d6f  on the Python Mo
-00000150: 6462 7573 2d54 4b20 6c69 6272 6172 792c  dbus-TK library,
-00000160: 2069 7320 616e 2061 6c74 6572 6e61 7469   is an alternati
-00000170: 7665 2074 6f20 7468 6520 6f72 6967 696e  ve to the origin
-00000180: 616c 2056 4f4c 5454 524f 4e20 6d6f 6462  al VOLTTRON modb
-00000190: 7573 2064 7269 7665 722e 2055 6e6c 696b  us driver. Unlik
-000001a0: 6520 7468 6520 6f72 6967 696e 616c 206d  e the original m
-000001b0: 6f64 6275 7320 6472 6976 6572 2c20 7468  odbus driver, th
-000001c0: 6520 4d6f 6462 7573 2d54 4b20 6472 6976  e Modbus-TK driv
-000001d0: 6572 2073 7570 706f 7274 7320 4d6f 6462  er supports Modb
-000001e0: 7573 2052 5455 2061 7320 7765 6c6c 2061  us RTU as well a
-000001f0: 7320 4d6f 6462 7573 206f 7665 7220 5443  s Modbus over TC
-00000200: 502f 4950 2e0a 0a23 2050 7265 7265 7175  P/IP...# Prerequ
-00000210: 6973 6974 6573 0a0a 2a20 5079 7468 6f6e  isites..* Python
-00000220: 2033 2e38 0a0a 2320 496e 7374 616c 6c61   3.8..# Installa
-00000230: 7469 6f6e 0a0a 312e 2043 7265 6174 6520  tion..1. Create 
-00000240: 616e 6420 6163 7469 7661 7465 2061 2076  and activate a v
-00000250: 6972 7475 616c 2065 6e76 6972 6f6e 6d65  irtual environme
-00000260: 6e74 2e0a 0a20 2020 2060 6060 7368 656c  nt...    ```shel
-00000270: 6c0a 2020 2020 7079 7468 6f6e 202d 6d20  l.    python -m 
-00000280: 7665 6e76 2065 6e76 0a20 2020 2073 6f75  venv env.    sou
-00000290: 7263 6520 656e 762f 6269 6e2f 6163 7469  rce env/bin/acti
-000002a0: 7661 7465 0a20 2020 2060 6060 0a0a 312e  vate.    ```..1.
-000002b0: 2049 6e73 7461 6c6c 2076 6f6c 7474 726f   Install volttro
-000002c0: 6e20 616e 6420 7374 6172 7420 7468 6520  n and start the 
-000002d0: 706c 6174 666f 726d 2e0a 0a20 2020 2060  platform...    `
-000002e0: 6060 7368 656c 6c0a 2020 2020 7069 7020  ``shell.    pip 
-000002f0: 696e 7374 616c 6c20 766f 6c74 7472 6f6e  install volttron
-00000300: 0a0a 2020 2020 2320 5374 6172 7420 706c  ..    # Start pl
-00000310: 6174 666f 726d 2077 6974 6820 6f75 7470  atform with outp
-00000320: 7574 2067 6f69 6e67 2074 6f20 766f 6c74  ut going to volt
-00000330: 7472 6f6e 2e6c 6f67 0a20 2020 2076 6f6c  tron.log.    vol
-00000340: 7474 726f 6e20 2d76 7620 2d6c 2076 6f6c  ttron -vv -l vol
-00000350: 7474 726f 6e2e 6c6f 6720 260a 2020 2020  ttron.log &.    
-00000360: 6060 600a 0a31 2e20 496e 7374 616c 6c20  ```..1. Install 
-00000370: 7468 6520 766f 6c74 7472 6f6e 2070 6c61  the volttron pla
-00000380: 7466 6f72 6d20 6472 6976 6572 3a0a 0a20  tform driver:.. 
-00000390: 2020 2060 6060 7368 656c 6c0a 2020 2020     ```shell.    
-000003a0: 7663 746c 2069 6e73 7461 6c6c 2076 6f6c  vctl install vol
-000003b0: 7474 726f 6e2d 706c 6174 666f 726d 2d64  ttron-platform-d
-000003c0: 7269 7665 7220 2d2d 7669 702d 6964 656e  river --vip-iden
-000003d0: 7469 7479 2070 6c61 7466 6f72 6d2e 6472  tity platform.dr
-000003e0: 6976 6572 202d 2d73 7461 7274 0a20 2020  iver --start.   
-000003f0: 2060 6060 0a0a 312e 2049 6e73 7461 6c6c   ```..1. Install
-00000400: 2074 6865 2076 6f6c 7474 726f 6e2d 6c69   the volttron-li
-00000410: 622d 6d6f 6462 7573 746b 2d64 7269 7665  b-modbustk-drive
-00000420: 7220 6c69 6272 6172 792e 0a0a 2020 2020  r library...    
-00000430: 6060 6073 6865 6c6c 0a20 2020 2070 6970  ```shell.    pip
-00000440: 2069 6e73 7461 6c6c 2076 6f6c 7474 726f   install volttro
-00000450: 6e2d 6c69 622d 6d6f 6462 7573 746b 2d64  n-lib-modbustk-d
-00000460: 7269 7665 720a 2020 2020 6060 600a 0a31  river.    ```..1
-00000470: 2e20 496e 7374 616c 6c20 7468 6520 6472  . Install the dr
-00000480: 6976 6572 206f 6e74 6f20 7468 6520 506c  iver onto the Pl
-00000490: 6174 666f 726d 2044 7269 7665 722e 0a0a  atform Driver...
-000004a0: 2020 2020 496e 7374 616c 6c69 6e67 2061      Installing a
-000004b0: 2064 7269 7665 7220 696e 2074 6865 2050   driver in the P
-000004c0: 6c61 7466 6f72 6d20 4472 6976 6572 2041  latform Driver A
-000004d0: 6765 6e74 2072 6571 7569 7265 7320 6164  gent requires ad
-000004e0: 6469 6e67 2063 6f70 6965 7320 6f66 2074  ding copies of t
-000004f0: 6865 2064 6576 6963 6520 636f 6e66 6967  he device config
-00000500: 7572 6174 696f 6e20 616e 6420 7265 6769  uration and regi
-00000510: 7374 7279 2063 6f6e 6669 6775 7261 7469  stry configurati
-00000520: 6f6e 2066 696c 6573 2074 6f20 7468 6520  on files to the 
-00000530: 506c 6174 666f 726d 2044 7269 7665 72e2  Platform Driver.
-00000540: 8099 7320 636f 6e66 6967 7572 6174 696f  ..s configuratio
-00000550: 6e20 7374 6f72 652e 0a0a 2020 2020 4372  n store...    Cr
-00000560: 6561 7465 2061 2063 6f6e 6669 6720 6469  eate a config di
-00000570: 7265 6374 6f72 7920 616e 6420 6e61 7669  rectory and navi
-00000580: 6761 7465 2074 6f20 6974 3a0a 0a20 2020  gate to it:..   
-00000590: 2060 6060 7368 656c 6c0a 2020 2020 6d6b   ```shell.    mk
-000005a0: 6469 7220 636f 6e66 6967 0a20 2020 2063  dir config.    c
-000005b0: 6420 636f 6e66 6967 0a20 2020 2060 6060  d config.    ```
-000005c0: 0a0a 312e 2041 6464 2064 7269 7665 7220  ..1. Add driver 
-000005d0: 636f 6e66 6967 7572 6174 696f 6e73 2074  configurations t
-000005e0: 6f20 7468 6520 506c 6174 666f 726d 2044  o the Platform D
-000005f0: 7269 7665 722e 0a0a 2020 2054 6865 204d  river...   The M
-00000600: 6f64 6275 732d 544b 2064 7269 7665 7220  odbus-TK driver 
-00000610: 6973 206d 6f73 746c 7920 6261 636b 7761  is mostly backwa
-00000620: 7264 2d63 6f6d 7061 7469 626c 6520 7769  rd-compatible wi
-00000630: 7468 2074 6865 2070 6172 616d 6574 6572  th the parameter
-00000640: 2064 6566 696e 6974 696f 6e73 2069 6e20   definitions in 
-00000650: 7468 6520 6f72 6967 696e 616c 204d 6f64  the original Mod
-00000660: 6275 7320 6472 6976 6572 e280 9973 2063  bus driver...s c
-00000670: 6f6e 6669 6775 7261 7469 6f6e 2028 2e63  onfiguration (.c
-00000680: 6f6e 6669 6720 616e 6420 2e63 7376 2066  onfig and .csv f
-00000690: 696c 6573 292e 2049 6620 7468 6520 636f  iles). If the co
-000006a0: 6e66 6967 2066 696c 65e2 8099 7320 7061  nfig file...s pa
-000006b0: 7261 6d65 7465 7220 6e61 6d65 7320 7573  rameter names us
-000006c0: 6520 7468 6520 4d6f 6462 7573 2064 7269  e the Modbus dri
-000006d0: 7665 72e2 8099 7320 6e61 6d65 2063 6f6e  ver...s name con
-000006e0: 7665 6e74 696f 6e73 2c20 7468 6579 2061  ventions, they a
-000006f0: 7265 2074 7261 6e73 6c61 7465 6420 746f  re translated to
-00000700: 2074 6865 204d 6f64 6275 732d 544b 206e   the Modbus-TK n
-00000710: 616d 6520 636f 6e76 656e 7469 6f6e 732c  ame conventions,
-00000720: 2065 2e67 2e20 6120 4d6f 6462 7573 2043   e.g. a Modbus C
-00000730: 5356 2066 696c 65e2 8099 7320 506f 696e  SV file...s Poin
-00000740: 7420 4164 6472 6573 7320 6973 2069 6e74  t Address is int
-00000750: 6572 7072 6574 6564 2061 7320 6120 4d6f  erpreted as a Mo
-00000760: 6462 7573 2d54 4b20 e280 9c41 6464 7265  dbus-TK ...Addre
-00000770: 7373 e280 9d2e 2042 6163 6b77 6172 642d  ss.... Backward-
-00000780: 636f 6d70 6174 6962 696c 6974 7920 6578  compatibility ex
-00000790: 6365 7074 696f 6e73 2061 7265 3a0a 0a20  ceptions are:.. 
-000007a0: 2020 2020 2020 202a 2049 6620 7468 6520         * If the 
-000007b0: 636f 6e66 6967 2066 696c 6520 6861 7320  config file has 
-000007c0: 6e6f 2070 6f72 742c 2074 6865 2064 6566  no port, the def
-000007d0: 6175 6c74 2069 7320 302c 206e 6f74 2035  ault is 0, not 5
-000007e0: 3032 2e0a 0a20 2020 2020 2020 202a 2049  02...        * I
-000007f0: 6620 7468 6520 636f 6e66 6967 2066 696c  f the config fil
-00000800: 6520 6861 7320 6e6f 2073 6c61 7665 5f69  e has no slave_i
-00000810: 642c 2074 6865 2064 6566 6175 6c74 2069  d, the default i
-00000820: 7320 312c 206e 6f74 2030 2e0a 0a20 2020  s 1, not 0...   
-00000830: 2054 6865 2064 7269 7665 725f 636f 6e66   The driver_conf
-00000840: 6967 2073 6563 7469 6f6e 206f 6620 6120  ig section of a 
-00000850: 4d6f 6462 7573 2d54 4b20 6465 7669 6365  Modbus-TK device
-00000860: 2063 6f6e 6669 6775 7261 7469 6f6e 2066   configuration f
-00000870: 696c 6520 7375 7070 6f72 7473 2061 2076  ile supports a v
-00000880: 6172 6965 7479 206f 6620 7061 7261 6d65  ariety of parame
-00000890: 7465 7220 6465 6669 6e69 7469 6f6e 732c  ter definitions,
-000008a0: 2062 7574 206f 6e6c 7920 2a64 6576 6963   but only *devic
-000008b0: 655f 6164 6472 6573 732a 2069 7320 7265  e_address* is re
-000008c0: 7175 6972 6564 3a0a 0a20 2020 202a 2064  quired:..    * d
-000008d0: 6576 6963 655f 6164 6472 6573 7320 2852  evice_address (R
-000008e0: 6571 7569 7265 6429 3a20 2049 5020 4164  equired):  IP Ad
-000008f0: 6472 6573 7320 6f66 2074 6865 2064 6576  dress of the dev
-00000900: 6963 652e 0a0a 2020 2020 2a20 6e61 6d65  ice...    * name
-00000910: 2028 4f70 7469 6f6e 616c 2920 2d20 4e61   (Optional) - Na
-00000920: 6d65 206f 6620 7468 6520 6465 7669 6365  me of the device
-00000930: 2e20 4465 6661 756c 7473 2074 6f20 e280  . Defaults to ..
-00000940: 9c55 4e4b 4e4f 574e e280 9d2e 0a0a 2020  .UNKNOWN......  
-00000950: 2020 2a20 6465 7669 6365 5f74 7970 6520    * device_type 
-00000960: 284f 7074 696f 6e61 6c29 202d 204e 616d  (Optional) - Nam
-00000970: 6520 6f66 2074 6865 2064 6576 6963 6520  e of the device 
-00000980: 7479 7065 2e20 4465 6661 756c 7473 2074  type. Defaults t
-00000990: 6f20 e280 9c55 4e4b 4e4f 574e e280 9d2e  o ...UNKNOWN....
-000009a0: 0a0a 2020 2020 2a20 706f 7274 2028 4f70  ..    * port (Op
-000009b0: 7469 6f6e 616c 2920 2d20 506f 7274 2074  tional) - Port t
-000009c0: 6865 2064 6576 6963 6520 6973 206c 6973  he device is lis
-000009d0: 7465 6e69 6e67 206f 6e2e 2044 6566 6175  tening on. Defau
-000009e0: 6c74 7320 746f 2030 2028 6e6f 2070 6f72  lts to 0 (no por
-000009f0: 7429 2e20 5573 6520 706f 7274 2030 2066  t). Use port 0 f
-00000a00: 6f72 2052 5455 2074 7261 6e73 706f 7274  or RTU transport
-00000a10: 2e0a 0a20 2020 202a 2073 6c61 7665 5f69  ...    * slave_i
-00000a20: 6420 284f 7074 696f 6e61 6c29 202d 2053  d (Optional) - S
-00000a30: 6c61 7665 2049 4420 6f66 2074 6865 2064  lave ID of the d
-00000a40: 6576 6963 652e 2044 6566 6175 6c74 7320  evice. Defaults 
-00000a50: 746f 2031 2e20 5573 6520 4944 2030 2066  to 1. Use ID 0 f
-00000a60: 6f72 206e 6f20 736c 6176 652e 0a0a 2020  or no slave...  
-00000a70: 2020 2a20 6261 7564 7261 7465 2028 4f70    * baudrate (Op
-00000a80: 7469 6f6e 616c 2920 2d20 5365 7269 616c  tional) - Serial
-00000a90: 2028 5254 5529 2062 6175 6420 7261 7465   (RTU) baud rate
-00000aa0: 2e20 4465 6661 756c 7473 2074 6f20 3936  . Defaults to 96
-00000ab0: 3030 2e0a 0a20 2020 202a 2062 7974 6573  00...    * bytes
-00000ac0: 697a 6520 284f 7074 696f 6e61 6c29 202d  ize (Optional) -
-00000ad0: 2053 6572 6961 6c20 2852 5455 2920 6279   Serial (RTU) by
-00000ae0: 7465 2073 697a 653a 2035 2c20 362c 2037  te size: 5, 6, 7
-00000af0: 2c20 6f72 2038 2e20 4465 6661 756c 7473  , or 8. Defaults
-00000b00: 2074 6f20 382e 0a0a 2020 2020 2a20 7061   to 8...    * pa
-00000b10: 7269 7479 2028 4f70 7469 6f6e 616c 2920  rity (Optional) 
-00000b20: 2d20 5365 7269 616c 2028 5254 5529 2070  - Serial (RTU) p
-00000b30: 6172 6974 793a 206e 6f6e 652c 2065 7665  arity: none, eve
-00000b40: 6e2c 206f 6464 2c20 6d61 726b 2c20 6f72  n, odd, mark, or
-00000b50: 2073 7061 6365 2e20 4465 6661 756c 7473   space. Defaults
-00000b60: 2074 6f20 4e6f 6e65 2e0a 0a20 2020 202a   to None...    *
-00000b70: 2073 746f 7062 6974 7320 284f 7074 696f   stopbits (Optio
-00000b80: 6e61 6c29 202d 2053 6572 6961 6c20 2852  nal) - Serial (R
-00000b90: 5455 2920 7374 6f70 2062 6974 733a 2031  TU) stop bits: 1
-00000ba0: 2c20 312e 352c 206f 7220 322e 2044 6566  , 1.5, or 2. Def
-00000bb0: 6175 6c74 7320 746f 2031 2e0a 0a20 2020  aults to 1...   
-00000bc0: 202a 2078 6f6e 786f 6666 2028 4f70 7469   * xonxoff (Opti
-00000bd0: 6f6e 616c 2920 2d20 5365 7269 616c 2028  onal) - Serial (
-00000be0: 5254 5529 2066 6c6f 7720 636f 6e74 726f  RTU) flow contro
-00000bf0: 6c3a 2030 206f 7220 312e 2044 6566 6175  l: 0 or 1. Defau
-00000c00: 6c74 7320 746f 2030 2e0a 0a20 2020 202a  lts to 0...    *
-00000c10: 2061 6464 7265 7373 696e 6720 284f 7074   addressing (Opt
-00000c20: 696f 6e61 6c29 202d 2044 6174 6120 6164  ional) - Data ad
-00000c30: 6472 6573 7320 7461 626c 653a 206f 6666  dress table: off
-00000c40: 7365 742c 206f 6666 7365 745f 706c 7573  set, offset_plus
-00000c50: 2c20 6f72 2061 6464 7265 7373 2e20 4465  , or address. De
-00000c60: 6661 756c 7473 2074 6f20 6f66 6673 6574  faults to offset
-00000c70: 2e0a 0a20 2020 2020 202a 2061 6464 7265  ...      * addre
-00000c80: 7373 3a20 5468 6520 6578 6163 7420 7661  ss: The exact va
-00000c90: 6c75 6520 6f66 2074 6865 2061 6464 7265  lue of the addre
-00000ca0: 7373 2077 6974 686f 7574 2061 6e79 206f  ss without any o
-00000cb0: 6666 7365 7420 7661 6c75 652e 0a0a 2020  ffset value...  
-00000cc0: 2020 2020 2a20 6f66 6673 6574 3a20 5468      * offset: Th
-00000cd0: 6520 7661 6c75 6520 6f66 2074 6865 2061  e value of the a
-00000ce0: 6464 7265 7373 2070 6c75 7320 7468 6520  ddress plus the 
-00000cf0: 6f66 6673 6574 2076 616c 7565 2e0a 0a20  offset value... 
-00000d00: 2020 2020 202a 206f 6666 7365 745f 706c       * offset_pl
-00000d10: 7573 3a20 5468 6520 7661 6c75 6520 6f66  us: The value of
-00000d20: 2074 6865 2061 6464 7265 7373 2070 6c75   the address plu
-00000d30: 7320 7468 6520 6f66 6673 6574 2076 616c  s the offset val
-00000d40: 7565 2070 6c75 7320 6f6e 652e 0a0a 2020  ue plus one...  
-00000d50: 2020 2020 2a20 3a20 4966 2061 6e20 6f66      * : If an of
-00000d60: 6673 6574 2076 616c 7565 2069 7320 746f  fset value is to
-00000d70: 2062 6520 6164 6465 642c 2069 7420 6973   be added, it is
-00000d80: 2064 6574 6572 6d69 6e65 6420 6261 7365   determined base
-00000d90: 6420 6f6e 2061 2070 6f69 6e74 e280 9973  d on a point...s
-00000da0: 2070 726f 7065 7274 6965 7320 696e 2074   properties in t
-00000db0: 6865 2043 5356 2066 696c 653a 0a0a 2020  he CSV file:..  
-00000dc0: 2020 2020 2020 2a20 5479 7065 3d62 6f6f        * Type=boo
-00000dd0: 6c2c 2057 7269 7461 626c 653d 5452 5545  l, Writable=TRUE
-00000de0: 3a20 300a 0a20 2020 2020 2020 202a 2054  : 0..        * T
-00000df0: 7970 653d 626f 6f6c 2c20 5772 6974 6162  ype=bool, Writab
-00000e00: 6c65 3d46 414c 5345 3a20 3130 3030 300a  le=FALSE: 10000.
-00000e10: 0a20 2020 2020 2020 202a 2054 7970 6521  .        * Type!
-00000e20: 3d62 6f6f 6c2c 2057 7269 7461 626c 653d  =bool, Writable=
-00000e30: 5452 5545 3a20 3330 3030 300a 0a20 2020  TRUE: 30000..   
-00000e40: 2020 2020 202a 2054 7970 6521 3d62 6f6f       * Type!=boo
-00000e50: 6c2c 2057 7269 7461 626c 653d 4641 4c53  l, Writable=FALS
-00000e60: 453a 2034 3030 3030 0a0a 2020 2020 2a20  E: 40000..    * 
-00000e70: 656e 6469 616e 2028 4f70 7469 6f6e 616c  endian (Optional
-00000e80: 2920 2d20 4279 7465 206f 7264 6572 3a20  ) - Byte order: 
-00000e90: 6269 6720 6f72 206c 6974 746c 652e 2044  big or little. D
-00000ea0: 6566 6175 6c74 7320 746f 2062 6967 2e0a  efaults to big..
-00000eb0: 0a20 2020 202a 2077 7269 7465 5f6d 756c  .    * write_mul
-00000ec0: 7469 706c 655f 7265 6769 7374 6572 7320  tiple_registers 
-00000ed0: 284f 7074 696f 6e61 6c29 202d 2057 7269  (Optional) - Wri
-00000ee0: 7465 206d 756c 7469 706c 6520 636f 696c  te multiple coil
-00000ef0: 7320 6f72 2072 6567 6973 7465 7273 2061  s or registers a
-00000f00: 7420 6120 7469 6d65 2e20 4465 6661 756c  t a time. Defaul
-00000f10: 7473 2074 6f20 7472 7565 2e0a 0a20 2020  ts to true...   
-00000f20: 2020 202a 2049 6620 7772 6974 655f 6d75     * If write_mu
-00000f30: 6c74 6970 6c65 5f72 6567 6973 7465 7273  ltiple_registers
-00000f40: 2069 7320 7365 7420 746f 2066 616c 7365   is set to false
-00000f50: 2c20 6f6e 6c79 2072 6567 6973 7465 7220  , only register 
-00000f60: 7479 7065 7320 756e 7369 676e 6564 2073  types unsigned s
-00000f70: 686f 7274 2028 7569 6e74 3136 2920 616e  hort (uint16) an
-00000f80: 6420 626f 6f6c 6561 6e20 2862 6f6f 6c29  d boolean (bool)
-00000f90: 2061 7265 2073 7570 706f 7274 6564 2e20   are supported. 
-00000fa0: 5468 6520 6578 6365 7074 696f 6e20 7261  The exception ra
-00000fb0: 6973 6564 2064 7572 696e 6720 7468 6520  ised during the 
-00000fc0: 636f 6e66 6967 7572 6520 7072 6f63 6573  configure proces
-00000fd0: 732e 0a0a 2020 2020 2a20 7265 6769 7374  s...    * regist
-00000fe0: 6572 5f6d 6170 2028 4f70 7469 6f6e 616c  er_map (Optional
-00000ff0: 2920 2d20 5265 6769 7374 6572 206d 6170  ) - Register map
-00001000: 2063 7376 206f 6620 756e 6368 616e 6765   csv of unchange
-00001010: 6420 7265 6769 7374 6572 2076 6172 6961  d register varia
-00001020: 626c 6573 2e20 4465 6661 756c 7473 2074  bles. Defaults t
-00001030: 6f20 7265 6769 7374 7279 5f63 6f6e 6669  o registry_confi
-00001040: 6720 6373 762e 0a0a 2020 2020 5468 6973  g csv...    This
-00001050: 2072 6570 6f20 7072 6f76 6964 6573 2061   repo provides a
-00001060: 6e20 6578 616d 706c 6520 636f 6e66 6967  n example config
-00001070: 7572 6174 696f 6e20 696e 2074 6865 2066  uration in the f
-00001080: 696c 6520 226d 6f64 6275 735f 746b 5f65  ile "modbus_tk_e
-00001090: 7861 6d70 6c65 2e63 6f6e 6669 6722 2e0a  xample.config"..
-000010a0: 0a20 2020 2048 6572 6520 6973 2061 6e20  .    Here is an 
-000010b0: 6578 616d 706c 6520 6465 7669 6365 2063  example device c
-000010c0: 6f6e 6669 6775 7261 7469 6f6e 2066 696c  onfiguration fil
-000010d0: 653a 0a0a 2020 2020 6060 606a 736f 6e0a  e:..    ```json.
-000010e0: 2020 2020 2020 2020 7b0a 2020 2020 2020          {.      
-000010f0: 2020 2264 7269 7665 725f 636f 6e66 6967    "driver_config
-00001100: 223a 207b 0a20 2020 2020 2020 2020 2020  ": {.           
-00001110: 2022 6465 7669 6365 5f61 6464 7265 7373   "device_address
-00001120: 223a 2022 3130 2e31 2e31 2e32 222c 0a20  ": "10.1.1.2",. 
-00001130: 2020 2020 2020 2020 2020 2022 706f 7274             "port
-00001140: 223a 2022 3530 3230 222c 0a20 2020 2020  ": "5020",.     
-00001150: 2020 2020 2020 2022 7265 6769 7374 6572         "register
-00001160: 5f6d 6170 223a 2022 636f 6e66 6967 3a2f  _map": "config:/
-00001170: 2f6d 6f64 6275 735f 746b 5f74 6573 745f  /modbus_tk_test_
-00001180: 6d61 702e 6373 7622 0a20 2020 2020 2020  map.csv".       
-00001190: 207d 2c0a 2020 2020 2020 2020 2264 7269   },.        "dri
-000011a0: 7665 725f 7479 7065 223a 2022 6d6f 6462  ver_type": "modb
-000011b0: 7573 5f74 6b22 2c0a 2020 2020 2020 2020  us_tk",.        
-000011c0: 2272 6567 6973 7472 795f 636f 6e66 6967  "registry_config
-000011d0: 223a 2022 636f 6e66 6967 3a2f 2f6d 6f64  ": "config://mod
-000011e0: 6275 735f 746b 5f74 6573 742e 6373 7622  bus_tk_test.csv"
-000011f0: 2c0a 2020 2020 2020 2020 2269 6e74 6572  ,.        "inter
-00001200: 7661 6c22 3a20 3630 2c0a 2020 2020 2020  val": 60,.      
-00001210: 2020 2274 696d 657a 6f6e 6522 3a20 2255    "timezone": "U
-00001220: 5443 222c 0a20 2020 2020 2020 2022 6865  TC",.        "he
-00001230: 6172 745f 6265 6174 5f70 6f69 6e74 223a  art_beat_point":
-00001240: 2022 6865 6172 7462 6561 7422 0a20 2020   "heartbeat".   
-00001250: 2020 2020 207d 0a20 2020 2060 6060 0a0a       }.    ```..
-00001260: 2020 2020 4166 7465 7220 6372 6561 7469      After creati
-00001270: 6e67 2061 2064 7269 7665 7220 636f 6e66  ng a driver conf
-00001280: 6967 7572 6174 696f 6e20 6669 6c65 206e  iguration file n
-00001290: 616d 6564 2022 6d6f 6462 7573 5f74 6b5f  amed "modbus_tk_
-000012a0: 6578 616d 706c 652e 636f 6e66 6967 222c  example.config",
-000012b0: 2061 6464 2069 7420 746f 2074 6865 2043   add it to the C
-000012c0: 6f6e 6669 6775 7261 7469 6f6e 2053 746f  onfiguration Sto
-000012d0: 7265 3a0a 0a20 2020 2060 6060 7368 656c  re:..    ```shel
-000012e0: 6c0a 2020 2020 7663 746c 2063 6f6e 6669  l.    vctl confi
-000012f0: 6720 7374 6f72 6520 706c 6174 666f 726d  g store platform
-00001300: 2e64 7269 7665 7220 6465 7669 6365 732f  .driver devices/
-00001310: 6d6f 6462 7573 746b 206d 6f64 6275 735f  modbustk modbus_
-00001320: 746b 5f65 7861 6d70 6c65 2e63 6f6e 6669  tk_example.confi
-00001330: 670a 2020 2020 6060 600a 0a31 2e20 4164  g.    ```..1. Ad
-00001340: 6420 6120 4d6f 6462 7573 2d54 4b20 5265  d a Modbus-TK Re
-00001350: 6769 7374 6572 204d 6170 2043 5356 2046  gister Map CSV F
-00001360: 696c 6520 746f 2074 6865 2050 6c61 7466  ile to the Platf
-00001370: 6f72 6d20 4472 6976 6572 2e0a 0a20 2020  orm Driver...   
-00001380: 204d 6f64 6275 7320 544b 2072 6571 7569   Modbus TK requi
-00001390: 7265 7320 616e 2061 6464 6974 696f 6e61  res an additiona
-000013a0: 6c20 7265 6769 7374 7279 2063 6f6e 6669  l registry confi
-000013b0: 6775 7261 7469 6f6e 2066 696c 6520 636f  guration file co
-000013c0: 6d70 6172 6564 2074 6f20 7468 6520 7061  mpared to the pa
-000013d0: 7261 6469 676d 206f 6620 6d6f 7374 206f  radigm of most o
-000013e0: 7468 6572 2064 7269 7665 7273 2e20 5468  ther drivers. Th
-000013f0: 6520 7265 6769 7374 7279 206d 6170 2066  e registry map f
-00001400: 696c 6520 6973 2061 6e20 616e 616c 6f67  ile is an analog
-00001410: 7565 2074 6f20 7468 6520 7479 7069 6361  ue to the typica
-00001420: 6c20 7265 6769 7374 7279 2063 6f6e 6669  l registry confi
-00001430: 6775 7261 7469 6f6e 2066 696c 652e 2054  guration file. T
-00001440: 6865 2072 6567 6973 7472 7920 636f 6e66  he registry conf
-00001450: 6967 7572 6174 696f 6e20 6669 6c65 2069  iguration file i
-00001460: 7320 6120 7369 6d70 6c65 2066 696c 6520  s a simple file 
-00001470: 7768 6963 6820 6d61 7073 2064 6576 6963  which maps devic
-00001480: 6520 706f 696e 7420 6e61 6d65 7320 746f  e point names to
-00001490: 2075 7365 7220 7370 6563 6966 6965 6420   user specified 
-000014a0: 706f 696e 7420 6e61 6d65 732e 0a0a 2020  point names...  
-000014b0: 2020 5468 6973 2072 6570 6f20 7072 6f76    This repo prov
-000014c0: 6964 6573 2061 6e20 6578 616d 706c 6520  ides an example 
-000014d0: 636f 6e66 6967 7572 6174 696f 6e20 696e  configuration in
-000014e0: 2074 6865 2066 696c 6520 226d 6f64 6275   the file "modbu
-000014f0: 735f 746b 5f74 6573 745f 6d61 702e 6373  s_tk_test_map.cs
-00001500: 7622 2e0a 0a20 2020 2054 6865 2072 6567  v"...    The reg
-00001510: 6973 7472 7920 6d61 7020 6669 6c65 2069  istry map file i
-00001520: 7320 6120 4353 5620 6669 6c65 2e20 4561  s a CSV file. Ea
-00001530: 6368 2072 6f77 2063 6f6e 6669 6775 7265  ch row configure
-00001540: 7320 6120 7265 6769 7374 6572 2064 6566  s a register def
-00001550: 696e 6974 696f 6e20 6f6e 2074 6865 2064  inition on the d
-00001560: 6576 6963 652e 0a0a 2020 2020 5265 6769  evice...    Regi
-00001570: 7374 6572 204e 616d 6520 2852 6571 7569  ster Name (Requi
-00001580: 7265 6429 202d 2054 6865 2066 6965 6c64  red) - The field
-00001590: 206e 616d 6520 696e 2074 6865 206d 6f64   name in the mod
-000015a0: 6275 7320 636c 6965 6e74 2e20 5468 6973  bus client. This
-000015b0: 2066 6965 6c64 2069 7320 6469 7374 696e   field is distin
-000015c0: 6374 2061 6e64 2075 6e63 6861 6e67 6561  ct and unchangea
-000015d0: 626c 652e 0a0a 2020 2020 4164 6472 6573  ble...    Addres
-000015e0: 7320 2852 6571 7569 7265 6429 202d 2054  s (Required) - T
-000015f0: 6865 2070 6f69 6e74 e280 9973 206d 6f64  he point...s mod
-00001600: 6275 7320 6164 6472 6573 732e 2054 6865  bus address. The
-00001610: 2061 6464 7265 7373 696e 6720 6f70 7469   addressing opti
-00001620: 6f6e 2069 6e20 7468 6520 6472 6976 6572  on in the driver
-00001630: 2063 6f6e 6669 6775 7261 7469 6f6e 2063   configuration c
-00001640: 6f6e 7472 6f6c 7320 7768 6574 6865 7220  ontrols whether 
-00001650: 7468 6973 2069 7320 696e 7465 7270 7265  this is interpre
-00001660: 7465 6420 6173 2061 6e20 6578 6163 7420  ted as an exact 
-00001670: 6164 6472 6573 7320 6f72 2061 6e20 6f66  address or an of
-00001680: 6673 6574 2e0a 0a20 2020 2054 7970 6520  fset...    Type 
-00001690: 2852 6571 7569 7265 6429 202d 2054 6865  (Required) - The
-000016a0: 2070 6f69 6e74 e280 9973 2064 6174 6120   point...s data 
-000016b0: 7479 7065 3a20 626f 6f6c 2c20 7374 7269  type: bool, stri
-000016c0: 6e67 5b6c 656e 6774 685d 2c20 666c 6f61  ng[length], floa
-000016d0: 742c 2069 6e74 3136 2c20 696e 7433 322c  t, int16, int32,
-000016e0: 2069 6e74 3634 2c20 7569 6e74 3136 2c20   int64, uint16, 
-000016f0: 7569 6e74 3332 2c20 6f72 2075 696e 7436  uint32, or uint6
-00001700: 342e 0a0a 2020 2020 556e 6974 7320 284f  4...    Units (O
-00001710: 7074 696f 6e61 6c29 202d 2055 7365 6420  ptional) - Used 
-00001720: 666f 7220 6d65 7461 6461 7461 2077 6865  for metadata whe
-00001730: 6e20 6372 6561 7469 6e67 2070 6f69 6e74  n creating point
-00001740: 2069 6e66 6f72 6d61 7469 6f6e 206f 6e20   information on 
-00001750: 6120 6869 7374 6f72 6961 6e2e 2044 6566  a historian. Def
-00001760: 6175 6c74 2069 7320 616e 2065 6d70 7479  ault is an empty
-00001770: 2073 7472 696e 672e 0a0a 2020 2020 5772   string...    Wr
-00001780: 6974 6162 6c65 2028 4f70 7469 6f6e 616c  itable (Optional
-00001790: 2920 2d20 5452 5545 2f46 414c 5345 2e20  ) - TRUE/FALSE. 
-000017a0: 4f6e 6c79 2070 6f69 6e74 7320 666f 7220  Only points for 
-000017b0: 7768 6963 6820 5772 6974 6162 6c65 3d54  which Writable=T
-000017c0: 5255 4520 6361 6e20 6265 2075 7064 6174  RUE can be updat
-000017d0: 6564 2062 7920 6120 564f 4c54 5452 4f4e  ed by a VOLTTRON
-000017e0: 2061 6765 6e74 2e20 4465 6661 756c 7420   agent. Default 
-000017f0: 6973 2046 414c 5345 2e0a 0a20 2020 2044  is FALSE...    D
-00001800: 6566 6175 6c74 2056 616c 7565 2028 4f70  efault Value (Op
-00001810: 7469 6f6e 616c 2920 2d20 5468 6520 706f  tional) - The po
-00001820: 696e 74e2 8099 7320 6465 6661 756c 7420  int...s default 
-00001830: 7661 6c75 652e 2049 6620 6974 2069 7320  value. If it is 
-00001840: 7265 7665 7274 6564 2062 7920 616e 2061  reverted by an a
-00001850: 6765 6e74 2c20 6974 2063 6861 6e67 6573  gent, it changes
-00001860: 2062 6163 6b20 746f 2074 6869 7320 7661   back to this va
-00001870: 6c75 652e 2049 6620 7468 6973 2076 616c  lue. If this val
-00001880: 7565 2069 7320 6d69 7373 696e 672c 2069  ue is missing, i
-00001890: 7420 7769 6c6c 2072 6576 6572 7420 746f  t will revert to
-000018a0: 2074 6865 206c 6173 7420 6b6e 6f77 6e20   the last known 
-000018b0: 7661 6c75 6520 6e6f 7420 7365 7420 6279  value not set by
-000018c0: 2061 6e20 6167 656e 742e 0a0a 2020 2020   an agent...    
-000018d0: 5472 616e 7366 6f72 6d20 284f 7074 696f  Transform (Optio
-000018e0: 6e61 6c29 202d 2053 6361 6c69 6e67 2061  nal) - Scaling a
-000018f0: 6c67 6f72 6974 686d 3a20 7363 616c 6528  lgorithm: scale(
-00001900: 6d75 6c74 6970 6c69 6572 292c 2073 6361  multiplier), sca
-00001910: 6c65 5f69 6e74 286d 756c 7469 706c 6965  le_int(multiplie
-00001920: 7229 2c20 7363 616c 655f 7265 6728 7265  r), scale_reg(re
-00001930: 6769 7374 6572 5f6e 616d 6529 2c20 7363  gister_name), sc
-00001940: 616c 655f 7265 675f 706f 7765 7231 3028  ale_reg_power10(
-00001950: 7265 6769 7374 6572 5f6e 616d 6529 2c20  register_name), 
-00001960: 7363 616c 655f 6465 6369 6d61 6c5f 696e  scale_decimal_in
-00001970: 745f 7369 676e 6564 286d 756c 7469 706c  t_signed(multipl
-00001980: 6965 7229 2c20 6d6f 6431 306b 2872 6576  ier), mod10k(rev
-00001990: 6572 7365 292c 206d 6f64 3130 6b36 3428  erse), mod10k64(
-000019a0: 7265 7665 7273 6529 2c20 6d6f 6431 306b  reverse), mod10k
-000019b0: 3438 2872 6576 6572 6573 2920 6f72 206e  48(reveres) or n
-000019c0: 6f6e 652e 2044 6566 6175 6c74 2069 7320  one. Default is 
-000019d0: 616e 2065 6d70 7479 2073 7472 696e 672e  an empty string.
-000019e0: 0a0a 2020 2020 5461 626c 6520 284f 7074  ..    Table (Opt
-000019f0: 696f 6e61 6c29 202d 2053 7461 6e64 6172  ional) - Standar
-00001a00: 6420 6d6f 6462 7573 2074 6162 6c65 206e  d modbus table n
-00001a10: 616d 6520 6465 6669 6e69 6e67 2068 6f77  ame defining how
-00001a20: 2069 6e66 6f72 6d61 7469 6f6e 2069 7320   information is 
-00001a30: 7374 6f72 6564 2069 6e20 736c 6176 6520  stored in slave 
-00001a40: 6465 7669 6365 2e20 5468 6572 6520 6172  device. There ar
-00001a50: 6520 3420 6469 6666 6572 656e 7420 7461  e 4 different ta
-00001a60: 626c 6573 3a0a 0a20 2020 2064 6973 6372  bles:..    discr
-00001a70: 6574 655f 6f75 7470 7574 5f63 6f69 6c73  ete_output_coils
-00001a80: 3a20 7265 6164 2f77 7269 7465 2063 6f69  : read/write coi
-00001a90: 6c20 6e75 6d62 6572 7320 312d 3939 3939  l numbers 1-9999
-00001aa0: 0a0a 2020 2020 6469 7363 7265 7465 5f69  ..    discrete_i
-00001ab0: 6e70 7574 5f63 6f6e 7461 6374 733a 2072  nput_contacts: r
-00001ac0: 6561 6420 6f6e 6c79 2063 6f69 6c20 6e75  ead only coil nu
-00001ad0: 6d62 6572 7320 3130 3030 312d 3139 3939  mbers 10001-1999
-00001ae0: 390a 0a20 2020 2061 6e61 6c6f 675f 696e  9..    analog_in
-00001af0: 7075 745f 7265 6769 7374 6572 733a 2072  put_registers: r
-00001b00: 6561 6420 6f6e 6c79 2072 6567 6973 7465  ead only registe
-00001b10: 7220 6e75 6d62 6572 7320 3330 3030 312d  r numbers 30001-
-00001b20: 3339 3939 390a 0a20 2020 2061 6e61 6c6f  39999..    analo
-00001b30: 675f 6f75 7470 7574 5f68 6f6c 6469 6e67  g_output_holding
-00001b40: 5f72 6567 6973 7465 7273 3a20 7265 6164  _registers: read
-00001b50: 2f77 7269 7465 2072 6567 6973 7465 7220  /write register 
-00001b60: 6e75 6d62 6572 7320 3430 3030 312d 3439  numbers 40001-49
-00001b70: 3939 390a 0a20 2020 2049 6620 7468 6973  999..    If this
-00001b80: 2066 6965 6c64 2069 7320 656d 7074 792c   field is empty,
-00001b90: 2074 6865 206d 6f64 6275 7320 7461 626c   the modbus tabl
-00001ba0: 6520 7769 6c6c 2062 6520 6465 6669 6e65  e will be define
-00001bb0: 6420 6279 2074 7970 6520 616e 6420 7772  d by type and wr
-00001bc0: 6974 6162 6c65 2066 6965 6c64 732e 2042  itable fields. B
-00001bd0: 7920 7468 6174 2c20 7768 656e 2075 7365  y that, when use
-00001be0: 7220 7365 7473 2072 6561 6420 6f6e 6c79  r sets read only
-00001bf0: 2066 6f72 2072 6561 642f 7772 6974 6520   for read/write 
-00001c00: 636f 696c 732f 7265 6769 7374 6572 7320  coils/registers 
-00001c10: 6f72 2073 6574 7320 7265 6164 2f77 7269  or sets read/wri
-00001c20: 7465 2066 6f72 2072 6561 6420 6f6e 6c79  te for read only
-00001c30: 2063 6f69 6c73 2f72 6567 6973 7465 7273   coils/registers
-00001c40: 2c20 6974 2077 696c 6c20 7365 6c65 6374  , it will select
-00001c50: 2077 726f 6e67 2074 6162 6c65 2c20 616e   wrong table, an
-00001c60: 6420 7468 6572 6566 6f72 6520 7261 6973  d therefore rais
-00001c70: 6520 6578 6365 7074 696f 6e2e 0a0a 2020  e exception...  
-00001c80: 2020 4d69 7865 6420 456e 6469 616e 2028    Mixed Endian (
-00001c90: 4f70 7469 6f6e 616c 2920 2d20 5452 5545  Optional) - TRUE
-00001ca0: 2f46 414c 5345 2e20 4966 204d 6978 6564  /FALSE. If Mixed
-00001cb0: 2045 6e64 6961 6e20 6973 2073 6574 2074   Endian is set t
-00001cc0: 6f20 5452 5545 2c20 7468 6520 6f72 6465  o TRUE, the orde
-00001cd0: 7220 6f66 2074 6865 204d 6f64 6275 7320  r of the Modbus 
-00001ce0: 7265 6769 7374 6572 7320 7769 6c6c 2062  registers will b
-00001cf0: 6520 7265 7665 7273 6564 2062 6566 6f72  e reversed befor
-00001d00: 6520 7061 7273 696e 6720 7468 6520 7661  e parsing the va
-00001d10: 6c75 6520 6f72 2077 7269 7469 6e67 2069  lue or writing i
-00001d20: 7420 6f75 7420 746f 2074 6865 2064 6576  t out to the dev
-00001d30: 6963 652e 2042 7920 7365 7474 696e 6720  ice. By setting 
-00001d40: 6d69 7865 6420 656e 6469 616e 2c20 7472  mixed endian, tr
-00001d50: 616e 7366 6f72 6d20 6d75 7374 2062 6520  ansform must be 
-00001d60: 4e6f 6e65 2028 6e6f 206f 7029 2e20 4465  None (no op). De
-00001d70: 6661 756c 7473 2074 6f20 4641 4c53 452e  faults to FALSE.
-00001d80: 0a0a 2020 2020 4465 7363 7269 7074 696f  ..    Descriptio
-00001d90: 6e20 284f 7074 696f 6e61 6c29 202d 2041  n (Optional) - A
-00001da0: 6464 6974 696f 6e61 6c20 696e 666f 726d  dditional inform
-00001db0: 6174 696f 6e20 6162 6f75 7420 7468 6520  ation about the 
-00001dc0: 706f 696e 742e 2044 6566 6175 6c74 2069  point. Default i
-00001dd0: 7320 616e 2065 6d70 7479 2073 7472 696e  s an empty strin
-00001de0: 672e 0a0a 2020 2020 4865 7265 2069 7320  g...    Here is 
-00001df0: 6120 7361 6d70 6c65 204d 6f64 6275 732d  a sample Modbus-
-00001e00: 544b 2072 6567 6973 7472 7920 6d61 703a  TK registry map:
-00001e10: 0a0a 2020 2020 6060 6063 7376 0a20 2020  ..    ```csv.   
-00001e20: 2052 6567 6973 7465 7220 4e61 6d65 2c41   Register Name,A
-00001e30: 6464 7265 7373 2c54 7970 652c 556e 6974  ddress,Type,Unit
-00001e40: 732c 5772 6974 6162 6c65 2c44 6566 6175  s,Writable,Defau
-00001e50: 6c74 2056 616c 7565 2c54 7261 6e73 666f  lt Value,Transfo
-00001e60: 726d 2c54 6162 6c65 0a20 2020 2075 6e73  rm,Table.    uns
-00001e70: 6967 6e65 645f 7368 6f72 742c 302c 7569  igned_short,0,ui
-00001e80: 6e74 3136 2c4e 6f6e 652c 5452 5545 2c30  nt16,None,TRUE,0
-00001e90: 2c73 6361 6c65 2831 3029 2c61 6e61 6c6f  ,scale(10),analo
-00001ea0: 675f 6f75 7470 7574 5f68 6f6c 6469 6e67  g_output_holding
-00001eb0: 5f72 6567 6973 7465 7273 0a20 2020 2075  _registers.    u
-00001ec0: 6e73 6967 6e65 645f 696e 742c 312c 7569  nsigned_int,1,ui
-00001ed0: 6e74 3332 2c4e 6f6e 652c 5452 5545 2c30  nt32,None,TRUE,0
-00001ee0: 2c73 6361 6c65 2831 3029 2c61 6e61 6c6f  ,scale(10),analo
-00001ef0: 675f 6f75 7470 7574 5f68 6f6c 6469 6e67  g_output_holding
-00001f00: 5f72 6567 6973 7465 7273 0a20 2020 2075  _registers.    u
-00001f10: 6e73 6967 6e65 645f 6c6f 6e67 2c33 2c75  nsigned_long,3,u
-00001f20: 696e 7436 342c 4e6f 6e65 2c54 5255 452c  int64,None,TRUE,
-00001f30: 302c 7363 616c 6528 3130 292c 616e 616c  0,scale(10),anal
-00001f40: 6f67 5f6f 7574 7075 745f 686f 6c64 696e  og_output_holdin
-00001f50: 675f 7265 6769 7374 6572 730a 2020 2020  g_registers.    
-00001f60: 7361 6d70 6c65 5f73 686f 7274 2c37 2c69  sample_short,7,i
-00001f70: 6e74 3136 2c4e 6f6e 652c 5452 5545 2c30  nt16,None,TRUE,0
-00001f80: 2c73 6361 6c65 2831 3029 2c61 6e61 6c6f  ,scale(10),analo
-00001f90: 675f 6f75 7470 7574 5f68 6f6c 6469 6e67  g_output_holding
-00001fa0: 5f72 6567 6973 7465 7273 0a20 2020 2073  _registers.    s
-00001fb0: 616d 706c 655f 696e 742c 382c 696e 7433  ample_int,8,int3
-00001fc0: 322c 4e6f 6e65 2c54 5255 452c 302c 7363  2,None,TRUE,0,sc
-00001fd0: 616c 6528 3130 292c 616e 616c 6f67 5f6f  ale(10),analog_o
-00001fe0: 7574 7075 745f 686f 6c64 696e 675f 7265  utput_holding_re
-00001ff0: 6769 7374 6572 730a 2020 2020 7361 6d70  gisters.    samp
-00002000: 6c65 5f66 6c6f 6174 2c31 302c 666c 6f61  le_float,10,floa
-00002010: 742c 4e6f 6e65 2c54 5255 452c 302e 302c  t,None,TRUE,0.0,
-00002020: 7363 616c 6528 3130 292c 616e 616c 6f67  scale(10),analog
-00002030: 5f6f 7574 7075 745f 686f 6c64 696e 675f  _output_holding_
-00002040: 7265 6769 7374 6572 730a 2020 2020 7361  registers.    sa
-00002050: 6d70 6c65 5f6c 6f6e 672c 3132 2c69 6e74  mple_long,12,int
-00002060: 3634 2c4e 6f6e 652c 5452 5545 2c30 2c73  64,None,TRUE,0,s
-00002070: 6361 6c65 2831 3029 2c61 6e61 6c6f 675f  cale(10),analog_
-00002080: 6f75 7470 7574 5f68 6f6c 6469 6e67 5f72  output_holding_r
-00002090: 6567 6973 7465 7273 0a20 2020 2073 616d  egisters.    sam
-000020a0: 706c 655f 626f 6f6c 2c31 362c 626f 6f6c  ple_bool,16,bool
-000020b0: 2c4e 6f6e 652c 5452 5545 2c46 616c 7365  ,None,TRUE,False
-000020c0: 2c2c 616e 616c 6f67 5f6f 7574 7075 745f  ,,analog_output_
-000020d0: 686f 6c64 696e 675f 7265 6769 7374 6572  holding_register
-000020e0: 730a 2020 2020 7361 6d70 6c65 5f73 7472  s.    sample_str
-000020f0: 2c31 372c 7374 7269 6e67 5b31 325d 2c4e  ,17,string[12],N
-00002100: 6f6e 652c 5452 5545 2c68 656c 6c6f 2077  one,TRUE,hello w
-00002110: 6f72 6c64 212c 2c61 6e61 6c6f 675f 6f75  orld!,,analog_ou
-00002120: 7470 7574 5f68 6f6c 6469 6e67 5f72 6567  tput_holding_reg
-00002130: 6973 7465 7273 0a20 2020 2060 6060 0a0a  isters.    ```..
-00002140: 2020 2020 4166 7465 7220 6372 6561 7469      After creati
-00002150: 6e67 2061 2072 6567 6973 7472 7920 6d61  ng a registry ma
-00002160: 7020 6e61 6d65 6420 226d 6f64 6275 735f  p named "modbus_
-00002170: 746b 5f74 6573 745f 6d61 702e 6373 7622  tk_test_map.csv"
-00002180: 2c20 6164 6420 6974 2074 6f20 7468 6520  , add it to the 
-00002190: 436f 6e66 6967 7572 6174 696f 6e20 5374  Configuration St
-000021a0: 6f72 653a 0a0a 2020 2020 6060 6073 6865  ore:..    ```she
-000021b0: 6c6c 0a20 2020 2076 6374 6c20 636f 6e66  ll.    vctl conf
-000021c0: 6967 2073 746f 7265 2070 6c61 7466 6f72  ig store platfor
-000021d0: 6d2e 6472 6976 6572 206d 6f64 6275 735f  m.driver modbus_
-000021e0: 746b 5f74 6573 745f 6d61 702e 6373 7620  tk_test_map.csv 
-000021f0: 6d6f 6462 7573 5f74 6b5f 7465 7374 5f6d  modbus_tk_test_m
-00002200: 6170 2e63 7376 202d 2d63 7376 0a20 2020  ap.csv --csv.   
-00002210: 2060 6060 0a0a 312e 2041 6464 2061 2072   ```..1. Add a r
-00002220: 6567 6973 7472 7920 636f 6e66 6967 7572  egistry configur
-00002230: 6174 696f 6e20 746f 2074 6865 2050 6c61  ation to the Pla
-00002240: 7466 6f72 6d44 7269 7665 722e 0a0a 2020  tformDriver...  
-00002250: 2020 5468 6520 7265 6769 7374 7279 2063    The registry c
-00002260: 6f6e 6669 6775 7261 7469 6f6e 2066 696c  onfiguration fil
-00002270: 6520 6973 2061 2043 5356 2066 696c 652e  e is a CSV file.
-00002280: 2045 6163 6820 726f 7720 636f 6e66 6967   Each row config
-00002290: 7572 6573 2061 2070 6f69 6e74 206f 6e20  ures a point on 
-000022a0: 7468 6520 6465 7669 6365 2e0a 0a20 2020  the device...   
-000022b0: 2020 2020 2056 6f6c 7474 726f 6e20 506f       Volttron Po
-000022c0: 696e 7420 4e61 6d65 2028 5265 7175 6972  int Name (Requir
-000022d0: 6564 2920 2d20 5468 6520 6e61 6d65 2062  ed) - The name b
-000022e0: 7920 7768 6963 6820 7468 6520 706c 6174  y which the plat
-000022f0: 666f 726d 2061 6e64 2061 6765 6e74 7320  form and agents 
-00002300: 7265 6665 7220 746f 2074 6865 2070 6f69  refer to the poi
-00002310: 6e74 2e20 466f 7220 696e 7374 616e 6365  nt. For instance
-00002320: 2c20 6966 2074 6865 2056 6f6c 7474 726f  , if the Volttro
-00002330: 6e20 506f 696e 7420 4e61 6d65 2069 7320  n Point Name is 
-00002340: 4865 6174 4361 6c6c 312c 2074 6865 6e20  HeatCall1, then 
-00002350: 616e 2061 6765 6e74 2077 6f75 6c64 2075  an agent would u
-00002360: 7365 206d 795f 6361 6d70 7573 2f62 7569  se my_campus/bui
-00002370: 6c64 696e 6732 2f68 7661 6331 2f48 6561  lding2/hvac1/Hea
-00002380: 7443 616c 6c31 2074 6f20 7265 6665 7220  tCall1 to refer 
-00002390: 746f 2074 6865 2070 6f69 6e74 2077 6865  to the point whe
-000023a0: 6e20 7573 696e 6720 7468 6520 5250 4320  n using the RPC 
-000023b0: 696e 7465 7266 6163 6520 6f66 2074 6865  interface of the
-000023c0: 2061 6374 7561 746f 7220 6167 656e 742e   actuator agent.
-000023d0: 0a0a 2020 2020 2020 2020 5265 6769 7374  ..        Regist
-000023e0: 6572 204e 616d 6520 2852 6571 7569 7265  er Name (Require
-000023f0: 6429 202d 2054 6865 2066 6965 6c64 206e  d) - The field n
-00002400: 616d 6520 696e 2074 6865 206d 6f64 6275  ame in the modbu
-00002410: 7320 636c 6965 6e74 2e20 4974 206d 7573  s client. It mus
-00002420: 7420 6265 206d 6174 6368 6564 2077 6974  t be matched wit
-00002430: 6820 7468 6520 6669 656c 6420 6e61 6d65  h the field name
-00002440: 2066 726f 6d20 7265 6769 7374 6572 5f6d   from register_m
-00002450: 6170 2e0a 0a20 2020 2041 6e79 2061 6464  ap...    Any add
-00002460: 6974 696f 6e61 6c20 636f 6c75 6d6e 7320  itional columns 
-00002470: 7769 6c6c 206f 7665 7272 6964 6520 7468  will override th
-00002480: 6520 6578 6973 7465 6420 6669 656c 6473  e existed fields
-00002490: 2066 726f 6d20 7265 6769 7374 6572 5f6d   from register_m
-000024a0: 6170 2e0a 0a20 2020 2048 6572 6520 6973  ap...    Here is
-000024b0: 2061 2073 616d 706c 6520 4d6f 6462 7573   a sample Modbus
-000024c0: 2d54 4b20 7265 6769 7374 7279 2063 6f6e  -TK registry con
-000024d0: 6669 6775 7261 7469 6f6e 2077 6974 6820  figuration with 
-000024e0: 6465 6669 6e65 6420 7265 6769 7374 6572  defined register
-000024f0: 5f6d 6170 3a0a 0a20 2020 2060 6060 6373  _map:..    ```cs
-00002500: 760a 2020 2020 566f 6c74 7472 6f6e 2050  v.    Volttron P
-00002510: 6f69 6e74 204e 616d 652c 5265 6769 7374  oint Name,Regist
-00002520: 6572 204e 616d 650a 2020 2020 756e 7369  er Name.    unsi
-00002530: 676e 6564 2073 686f 7274 2c75 6e73 6967  gned short,unsig
-00002540: 6e65 645f 7368 6f72 740a 2020 2020 756e  ned_short.    un
-00002550: 7369 676e 6564 2069 6e74 2c75 6e73 6967  signed int,unsig
-00002560: 6e65 645f 696e 740a 2020 2020 756e 7369  ned_int.    unsi
-00002570: 676e 6564 206c 6f6e 672c 756e 7369 676e  gned long,unsign
-00002580: 6564 5f6c 6f6e 670a 2020 2020 7361 6d70  ed_long.    samp
-00002590: 6c65 2073 686f 7274 2c73 616d 706c 655f  le short,sample_
-000025a0: 7368 6f72 740a 2020 2020 7361 6d70 6c65  short.    sample
-000025b0: 2069 6e74 2c73 616d 706c 655f 696e 740a   int,sample_int.
-000025c0: 2020 2020 7361 6d70 6c65 2066 6c6f 6174      sample float
-000025d0: 2c73 616d 706c 655f 666c 6f61 740a 2020  ,sample_float.  
-000025e0: 2020 7361 6d70 6c65 206c 6f6e 672c 7361    sample long,sa
-000025f0: 6d70 6c65 5f6c 6f6e 670a 2020 2020 7361  mple_long.    sa
-00002600: 6d70 6c65 2062 6f6f 6c2c 7361 6d70 6c65  mple bool,sample
-00002610: 5f62 6f6f 6c0a 2020 2020 7361 6d70 6c65  _bool.    sample
-00002620: 2073 7472 2c73 616d 706c 655f 7374 720a   str,sample_str.
-00002630: 2020 2020 6060 600a 0a20 2020 2041 6674      ```..    Aft
-00002640: 6572 2063 7265 6174 696e 6720 6120 7265  er creating a re
-00002650: 6769 7374 7279 206d 6170 206e 616d 6564  gistry map named
-00002660: 2022 6d6f 6462 7573 5f74 6b5f 7465 7374   "modbus_tk_test
-00002670: 2e63 7376 222c 2061 6464 2069 7420 746f  .csv", add it to
-00002680: 2074 6865 2043 6f6e 6669 6775 7261 7469   the Configurati
-00002690: 6f6e 2053 746f 7265 3a0a 0a20 2020 2060  on Store:..    `
-000026a0: 6060 7368 656c 6c0a 2020 2020 7663 746c  ``shell.    vctl
-000026b0: 2063 6f6e 6669 6720 7374 6f72 6520 706c   config store pl
-000026c0: 6174 666f 726d 2e64 7269 7665 7220 6d6f  atform.driver mo
-000026d0: 6462 7573 5f74 6b5f 7465 7374 2e63 7376  dbus_tk_test.csv
-000026e0: 206d 6f64 6275 735f 746b 5f74 6573 742e   modbus_tk_test.
-000026f0: 6373 7620 2d2d 6373 760a 2020 2020 6060  csv --csv.    ``
-00002700: 600a 0a31 2e20 4f62 7365 7276 6520 4461  `..1. Observe Da
-00002710: 7461 0a0a 2020 2020 546f 2073 6565 2064  ta..    To see d
-00002720: 6174 6120 6265 696e 6720 7075 626c 6973  ata being publis
-00002730: 6865 6420 746f 2074 6865 2062 7573 2c20  hed to the bus, 
-00002740: 696e 7374 616c 6c20 6120 5b4c 6973 7465  install a [Liste
-00002750: 6e65 7220 4167 656e 745d 2868 7474 7073  ner Agent](https
-00002760: 3a2f 2f70 7970 692e 6f72 672f 7072 6f6a  ://pypi.org/proj
-00002770: 6563 742f 766f 6c74 7472 6f6e 2d6c 6973  ect/volttron-lis
-00002780: 7465 6e65 722f 293a 0a0a 2020 2020 6060  tener/):..    ``
-00002790: 600a 2020 2020 7663 746c 2069 6e73 7461  `.    vctl insta
-000027a0: 6c6c 2076 6f6c 7474 726f 6e2d 6c69 7374  ll volttron-list
-000027b0: 656e 6572 202d 2d73 7461 7274 0a20 2020  ener --start.   
-000027c0: 2060 6060 0a0a 2020 2020 4f6e 6365 2069   ```..    Once i
-000027d0: 6e73 7461 6c6c 6564 2c20 796f 7520 7368  nstalled, you sh
-000027e0: 6f75 6c64 2073 6565 2074 6865 2064 6174  ould see the dat
-000027f0: 6120 6265 696e 6720 7075 626c 6973 6865  a being publishe
-00002800: 6420 6279 2076 6965 7769 6e67 2074 6865  d by viewing the
-00002810: 2056 6f6c 7474 726f 6e20 6c6f 6773 2066   Volttron logs f
-00002820: 696c 6520 7468 6174 2077 6173 2063 7265  ile that was cre
-00002830: 6174 6564 2069 6e20 7374 6570 2032 2e0a  ated in step 2..
-00002840: 2020 2020 546f 2077 6174 6368 2074 6865      To watch the
-00002850: 206c 6f67 732c 206f 7065 6e20 6120 7365   logs, open a se
-00002860: 7061 7261 7465 2074 6572 6d69 6e61 6c20  parate terminal 
-00002870: 616e 6420 7275 6e20 7468 6520 666f 6c6c  and run the foll
-00002880: 6f77 696e 6720 636f 6d6d 616e 643a 0a0a  owing command:..
-00002890: 2020 2020 6060 600a 2020 2020 7461 696c      ```.    tail
-000028a0: 202d 6620 3c70 6174 6820 746f 2066 6f6c   -f <path to fol
-000028b0: 6465 7220 636f 6e74 6169 6e69 6e67 2076  der containing v
-000028c0: 6f6c 7474 726f 6e2e 6c6f 673e 2f76 6f6c  olttron.log>/vol
-000028d0: 7474 726f 6e2e 6c6f 670a 2020 2020 6060  ttron.log.    ``
-000028e0: 600a 0a23 204d 6f64 6275 732d 544b 2043  `..# Modbus-TK C
-000028f0: 6f6e 6669 6720 436f 6d6d 616e 6420 546f  onfig Command To
-00002900: 6f6c 0a0a 6063 6f6e 6669 675f 636d 642e  ol..`config_cmd.
-00002910: 7079 6020 6973 2061 2063 6f6d 6d61 6e64  py` is a command
-00002920: 2d6c 696e 6520 746f 6f6c 2066 6f72 2063  -line tool for c
-00002930: 7265 6174 696e 6720 616e 6420 6d61 696e  reating and main
-00002940: 7461 696e 696e 6720 564f 4c54 5452 4f4e  taining VOLTTRON
-00002950: 2064 7269 7665 7220 636f 6e66 6967 7572   driver configur
-00002960: 6174 696f 6e73 2e20 5468 6520 746f 6f6c  ations. The tool
-00002970: 2072 756e 7320 6672 6f6d 2074 6865 2063   runs from the c
-00002980: 6f6d 6d61 6e64 206c 696e 653a 0a0a 636f  ommand line:..co
-00002990: 6e66 6967 5f63 6d64 2e70 7920 7375 7070  nfig_cmd.py supp
-000029a0: 6f72 7473 2074 6865 2066 6f6c 6c6f 7769  orts the followi
-000029b0: 6e67 2063 6f6d 6d61 6e64 733a 0a0a 2a20  ng commands:..* 
-000029c0: 6865 6c70 202d 204c 6973 7420 616c 6c20  help - List all 
-000029d0: 636f 6d6d 616e 6473 2e0a 0a2a 2071 7569  commands...* qui
-000029e0: 7420 2d20 5175 6974 2074 6865 2063 6f6d  t - Quit the com
-000029f0: 6d61 6e64 2d6c 696e 6520 746f 6f6c 2e0a  mand-line tool..
-00002a00: 0a2a 206c 6973 745f 6469 7265 6374 6f72  .* list_director
-00002a10: 6965 7320 2d20 4c69 7374 2061 6c6c 2073  ies - List all s
-00002a20: 6574 7570 2064 6972 6563 746f 7269 6573  etup directories
-00002a30: 2c20 7769 7468 2061 6e20 6f70 7469 6f6e  , with an option
-00002a40: 2074 6f20 6564 6974 2074 6865 6972 2070   to edit their p
-00002a50: 6174 6873 2e0a 0a0a 4279 2064 6566 6175  aths....By defau
-00002a60: 6c74 2c20 616c 6c20 6469 7265 6374 6f72  lt, all director
-00002a70: 6965 7320 6172 6520 696e 2074 6869 7320  ies are in this 
-00002a80: 7265 706f 2061 7420 7468 6520 666f 6c6c  repo at the foll
-00002a90: 6f77 696e 6720 666f 6c64 6572 3a20 766f  owing folder: vo
-00002aa0: 6c74 7472 6f6e 2f64 7269 7665 722f 696e  lttron/driver/in
-00002ab0: 7465 7266 6163 6573 2f6d 6f64 6275 735f  terfaces/modbus_
-00002ac0: 746b 2f75 7469 6c73 2f6d 6170 732e 0a0a  tk/utils/maps...
-00002ad0: 4974 2069 7320 696d 706f 7274 616e 7420  It is important 
-00002ae0: 746f 2075 7365 2074 6865 2063 6f72 7265  to use the corre
-00002af0: 6374 2064 6972 6563 746f 7269 6573 2077  ct directories w
-00002b00: 6865 6e20 6164 6469 6e67 2f65 6469 7469  hen adding/editi
-00002b10: 6e67 2064 6576 6963 6520 7479 7065 7320  ng device types 
-00002b20: 616e 6420 6472 6976 6572 2063 6f6e 6669  and driver confi
-00002b30: 6773 2c20 616e 6420 7768 656e 206c 6f61  gs, and when loa
-00002b40: 6469 6e67 2063 6f6e 6669 6775 7261 7469  ding configurati
-00002b50: 6f6e 7320 696e 746f 2056 4f4c 5454 524f  ons into VOLTTRO
-00002b60: 4e2e 0a0a 2a20 6d61 705f 6469 723a 2064  N...* map_dir: d
-00002b70: 6972 6563 746f 7279 2069 6e20 7768 6963  irectory in whic
-00002b80: 6820 6d61 7073 2e79 616d 6c20 6973 2073  h maps.yaml is s
-00002b90: 746f 7265 642e 0a0a 2a20 636f 6e66 6967  tored...* config
-00002ba0: 5f64 6972 3a20 6469 7265 6374 6f72 7920  _dir: directory 
-00002bb0: 696e 2077 6869 6368 2064 7269 7665 7220  in which driver 
-00002bc0: 636f 6e66 6967 2066 696c 6573 2061 7265  config files are
-00002bd0: 2073 746f 7265 642e 0a0a 2a20 6373 765f   stored...* csv_
-00002be0: 6469 723a 2064 6972 6563 746f 7279 2069  dir: directory i
-00002bf0: 6e20 7768 6963 6820 7265 6769 7374 7279  n which registry
-00002c00: 2063 6f6e 6669 6720 4353 5620 6669 6c65   config CSV file
-00002c10: 7320 6172 6520 7374 6f72 6564 2e0a 0a2a  s are stored...*
-00002c20: 2065 6469 745f 6469 7265 6374 6f72 6965   edit_directorie
-00002c30: 7320 2d20 4164 642f 4564 6974 206d 6170  s - Add/Edit map
-00002c40: 2064 6972 6563 746f 7279 2c20 6472 6976   directory, driv
-00002c50: 6572 2063 6f6e 6669 6720 6469 7265 6374  er config direct
-00002c60: 6f72 792c 2061 6e64 2f6f 7220 4353 5620  ory, and/or CSV 
-00002c70: 636f 6e66 6967 2064 6972 6563 746f 7279  config directory
-00002c80: 2e20 5072 6573 7320 3c45 6e74 6572 3e20  . Press <Enter> 
-00002c90: 6966 206e 6f20 6368 616e 6765 2069 7320  if no change is 
-00002ca0: 6e65 6564 6564 2e20 4578 6974 7320 6966  needed. Exits if
-00002cb0: 2074 6865 2064 6972 6563 746f 7279 2064   the directory d
-00002cc0: 6f65 7320 6e6f 7420 6578 6973 742e 0a0a  oes not exist...
-00002cd0: 2a20 6c69 7374 5f64 6576 6963 655f 7479  * list_device_ty
-00002ce0: 7065 5f64 6573 6372 6970 7469 6f6e 202d  pe_description -
-00002cf0: 204c 6973 7420 616c 6c20 6465 7669 6365   List all device
-00002d00: 2074 7970 6520 6465 7363 7269 7074 696f   type descriptio
-00002d10: 6e73 2069 6e20 6d61 7073 2e79 616d 6c2e  ns in maps.yaml.
-00002d20: 204f 7074 696f 6e20 746f 2065 6469 7420   Option to edit 
-00002d30: 6465 7669 6365 2074 7970 6520 6465 7363  device type desc
-00002d40: 7269 7074 696f 6e73 2e0a 0a2a 206c 6973  riptions...* lis
-00002d50: 745f 616c 6c5f 6465 7669 6365 5f74 7970  t_all_device_typ
-00002d60: 6573 202d 204c 6973 7420 616c 6c20 6465  es - List all de
-00002d70: 7669 6365 2074 7970 6520 696e 666f 726d  vice type inform
-00002d80: 6174 696f 6e20 696e 206d 6170 732e 7961  ation in maps.ya
-00002d90: 6d6c 2e20 4f70 7469 6f6e 2074 6f20 6164  ml. Option to ad
-00002da0: 6420 6d6f 7265 2064 6576 6963 6520 7479  d more device ty
-00002db0: 7065 732e 0a0a 2a20 6465 7669 6365 5f74  pes...* device_t
-00002dc0: 7970 6520 2d20 4c69 7374 2069 6e66 6f72  ype - List infor
-00002dd0: 6d61 7469 6f6e 2066 6f72 2061 2073 656c  mation for a sel
-00002de0: 6563 7465 6420 6465 7669 6365 2074 7970  ected device typ
-00002df0: 652e 204f 7074 696f 6e20 746f 2073 656c  e. Option to sel
-00002e00: 6563 7420 616e 6f74 6865 7220 6465 7669  ect another devi
-00002e10: 6365 2074 7970 652e 0a0a 2a20 6164 645f  ce type...* add_
-00002e20: 6465 7669 6365 5f74 7970 6520 2d20 4164  device_type - Ad
-00002e30: 6420 6120 6465 7669 6365 2074 7970 6520  d a device type 
-00002e40: 746f 206d 6170 732e 7961 6d6c 2e20 4f70  to maps.yaml. Op
-00002e50: 7469 6f6e 2074 6f20 6164 6420 6d6f 7265  tion to add more
-00002e60: 2074 6861 6e20 6f6e 6520 6465 7669 6365   than one device
-00002e70: 2074 7970 652e 2045 6163 6820 6465 7669   type. Each devi
-00002e80: 6365 2074 7970 6520 696e 636c 7564 6573  ce type includes
-00002e90: 2069 7473 206e 616d 652c 2043 5356 2066   its name, CSV f
-00002ea0: 696c 652c 2064 6573 6372 6970 7469 6f6e  ile, description
-00002eb0: 2c20 6164 6472 6573 7369 6e67 2c20 616e  , addressing, an
-00002ec0: 6420 656e 6469 616e 2c20 6173 2065 7870  d endian, as exp
-00002ed0: 6c61 696e 6564 2069 6e20 4d4f 4442 5553  lained in MODBUS
-00002ee0: 2d54 4b20 4472 6976 6572 204d 6170 732e  -TK Driver Maps.
-00002ef0: 2049 6620 616e 2069 6e76 616c 6964 2076   If an invalid v
-00002f00: 616c 7565 2069 7320 656e 7465 7265 6420  alue is entered 
-00002f10: 666f 7220 6164 6472 6573 7369 6e67 206f  for addressing o
-00002f20: 7220 656e 6469 616e 2c20 7468 6520 6465  r endian, the de
-00002f30: 6661 756c 7420 7661 6c75 6520 6973 2075  fault value is u
-00002f40: 7365 6420 696e 7374 6561 642e 0a0a 2a65  sed instead...*e
-00002f50: 6469 745f 6465 7669 6365 5f74 7970 6520  dit_device_type 
-00002f60: 2d20 4564 6974 2061 6e20 6578 6973 7469  - Edit an existi
-00002f70: 6e67 2064 6576 6963 6520 7479 7065 2e20  ng device type. 
-00002f80: 4966 2061 6e20 696e 7661 6c69 6420 7661  If an invalid va
-00002f90: 6c75 6520 6973 2065 6e74 6572 6564 2066  lue is entered f
-00002fa0: 6f72 2061 6464 7265 7373 696e 6720 6f72  or addressing or
-00002fb0: 2065 6e64 6961 6e2c 2074 6865 2070 7265   endian, the pre
-00002fc0: 7669 6f75 7320 7661 6c75 6520 6973 206c  vious value is l
-00002fd0: 6566 7420 756e 6368 616e 6765 642e 0a0a  eft unchanged...
-00002fe0: 2a20 6c69 7374 5f64 7269 7665 7273 202d  * list_drivers -
-00002ff0: 204c 6973 7420 616c 6c20 6472 6976 6572   List all driver
-00003000: 2063 6f6e 6669 6720 6e61 6d65 7320 696e   config names in
-00003010: 2063 6f6e 6669 675f 6469 722e 0a0a 2a20   config_dir...* 
-00003020: 6472 6976 6572 5f63 6f6e 6669 6720 3c64  driver_config <d
-00003030: 7269 7665 725f 6e61 6d65 3e20 2d20 4765  river_name> - Ge
-00003040: 7420 6120 6472 6976 6572 2063 6f6e 6669  t a driver confi
-00003050: 6720 6672 6f6d 2063 6f6e 6669 675f 6469  g from config_di
-00003060: 722e 204f 7074 696f 6e20 746f 2073 656c  r. Option to sel
-00003070: 6563 7420 7468 6520 6472 6976 6572 2069  ect the driver i
-00003080: 6620 6e6f 2064 7269 7665 7220 6973 2066  f no driver is f
-00003090: 6f75 6e64 2077 6974 6820 7468 6174 206e  ound with that n
-000030a0: 616d 652e 0a0a 2a20 6164 645f 6472 6976  ame...* add_driv
-000030b0: 6572 5f63 6f6e 6669 6720 3c64 7269 7665  er_config <drive
-000030c0: 725f 6e61 6d65 3e20 2d20 4164 642f 4564  r_name> - Add/Ed
-000030d0: 6974 203c 636f 6e66 6967 5f64 6972 3e2f  it <config_dir>/
-000030e0: 3c64 7269 7665 7220 6e61 6d65 3e2e 636f  <driver name>.co
-000030f0: 6e66 6967 2e20 4f70 7469 6f6e 2074 6f20  nfig. Option to 
-00003100: 7365 6c65 6374 2074 6865 2064 7269 7665  select the drive
-00003110: 7220 6966 206e 6f20 6472 6976 6572 2069  r if no driver i
-00003120: 7320 666f 756e 6420 7769 7468 2074 6861  s found with tha
-00003130: 7420 6e61 6d65 2e20 5072 6573 7320 3c45  t name. Press <E
-00003140: 6e74 6572 3e20 746f 2065 7869 742e 0a0a  nter> to exit...
-00003150: 2a20 6c6f 6164 5f76 6f6c 7474 726f 6e20  * load_volttron 
-00003160: 2d20 4c6f 6164 2061 2064 7269 7665 7220  - Load a driver 
-00003170: 636f 6e66 6967 2061 6e64 2043 5356 2069  config and CSV i
-00003180: 6e74 6f20 564f 4c54 5452 4f4e 2e20 4f70  nto VOLTTRON. Op
-00003190: 7469 6f6e 2074 6f20 6164 6420 7468 6520  tion to add the 
-000031a0: 636f 6e66 6967 206f 7220 4353 5620 6669  config or CSV fi
-000031b0: 6c65 2074 6f20 636f 6e66 6967 5f64 6972  le to config_dir
-000031c0: 206f 7220 746f 2063 7376 5f64 6972 2e20   or to csv_dir. 
-000031d0: 564f 4c54 5452 4f4e 206d 7573 7420 6265  VOLTTRON must be
-000031e0: 2072 756e 6e69 6e67 2077 6865 6e20 7468   running when th
-000031f0: 6973 2063 6f6d 6d61 6e64 2069 7320 7573  is command is us
-00003200: 6564 2e0a 0a2a 2064 656c 6574 655f 766f  ed...* delete_vo
-00003210: 6c74 7472 6f6e 5f63 6f6e 6669 6720 2d20  lttron_config - 
-00003220: 4465 6c65 7465 2061 2064 7269 7665 7220  Delete a driver 
-00003230: 636f 6e66 6967 2066 726f 6d20 564f 4c54  config from VOLT
-00003240: 5452 4f4e 2e20 564f 4c54 5452 4f4e 206d  TRON. VOLTTRON m
-00003250: 7573 7420 6265 2072 756e 6e69 6e67 2077  ust be running w
-00003260: 6865 6e20 7468 6973 2063 6f6d 6d61 6e64  hen this command
-00003270: 2069 7320 7573 6564 2e0a 0a2a 2064 656c   is used...* del
-00003280: 6574 655f 766f 6c74 7472 6f6e 5f63 7376  ete_volttron_csv
-00003290: 202d 2044 656c 6574 6520 6120 7265 6769   - Delete a regi
-000032a0: 7374 7279 2063 7376 2063 6f6e 6669 6720  stry csv config 
-000032b0: 6672 6f6d 2056 4f4c 5454 524f 4e2e 2056  from VOLTTRON. V
-000032c0: 4f4c 5454 524f 4e20 6d75 7374 2062 6520  OLTTRON must be 
-000032d0: 7275 6e6e 696e 6720 7768 656e 2074 6869  running when thi
-000032e0: 7320 636f 6d6d 616e 6420 6973 2075 7365  s command is use
-000032f0: 642e 0a0a 2320 4465 7665 6c6f 706d 656e  d...# Developmen
-00003300: 740a 0a50 6c65 6173 6520 7365 6520 7468  t..Please see th
-00003310: 6520 666f 6c6c 6f77 696e 6720 666f 7220  e following for 
-00003320: 636f 6e74 7269 6275 7469 6e67 2067 7569  contributing gui
-00003330: 6465 6c69 6e65 7320 5b63 6f6e 7472 6962  delines [contrib
-00003340: 7574 696e 675d 2868 7474 7073 3a2f 2f67  uting](https://g
-00003350: 6974 6875 622e 636f 6d2f 6563 6c69 7073  ithub.com/eclips
-00003360: 652d 766f 6c74 7472 6f6e 2f76 6f6c 7474  e-volttron/voltt
-00003370: 726f 6e2d 636f 7265 2f62 6c6f 622f 6465  ron-core/blob/de
-00003380: 7665 6c6f 702f 434f 4e54 5249 4255 5449  velop/CONTRIBUTI
-00003390: 4e47 2e6d 6429 2e0a 0a50 6c65 6173 6520  NG.md)...Please 
-000033a0: 7365 6520 7468 6520 666f 6c6c 6f77 696e  see the followin
-000033b0: 6720 6865 6c70 6675 6c20 6775 6964 6520  g helpful guide 
-000033c0: 6162 6f75 7420 5b64 6576 656c 6f70 696e  about [developin
-000033d0: 6720 6d6f 6475 6c61 7220 564f 4c54 5452  g modular VOLTTR
-000033e0: 4f4e 2061 6765 6e74 735d 2868 7474 7073  ON agents](https
-000033f0: 3a2f 2f67 6974 6875 622e 636f 6d2f 6563  ://github.com/ec
-00003400: 6c69 7073 652d 766f 6c74 7472 6f6e 2f76  lipse-volttron/v
-00003410: 6f6c 7474 726f 6e2d 636f 7265 2f62 6c6f  olttron-core/blo
-00003420: 622f 6465 7665 6c6f 702f 4445 5645 4c4f  b/develop/DEVELO
-00003430: 5049 4e47 5f4f 4e5f 4d4f 4455 4c41 522e  PING_ON_MODULAR.
-00003440: 6d64 290a 0a0a 2320 4469 7363 6c61 696d  md)...# Disclaim
-00003450: 6572 204e 6f74 6963 650a 0a54 6869 7320  er Notice..This 
-00003460: 6d61 7465 7269 616c 2077 6173 2070 7265  material was pre
-00003470: 7061 7265 6420 6173 2061 6e20 6163 636f  pared as an acco
-00003480: 756e 7420 6f66 2077 6f72 6b20 7370 6f6e  unt of work spon
-00003490: 736f 7265 6420 6279 2061 6e20 6167 656e  sored by an agen
-000034a0: 6379 206f 6620 7468 650a 556e 6974 6564  cy of the.United
-000034b0: 2053 7461 7465 7320 476f 7665 726e 6d65   States Governme
-000034c0: 6e74 2e20 204e 6569 7468 6572 2074 6865  nt.  Neither the
-000034d0: 2055 6e69 7465 6420 5374 6174 6573 2047   United States G
-000034e0: 6f76 6572 6e6d 656e 7420 6e6f 7220 7468  overnment nor th
-000034f0: 6520 556e 6974 6564 0a53 7461 7465 7320  e United.States 
-00003500: 4465 7061 7274 6d65 6e74 206f 6620 456e  Department of En
-00003510: 6572 6779 2c20 6e6f 7220 4261 7474 656c  ergy, nor Battel
-00003520: 6c65 2c20 6e6f 7220 616e 7920 6f66 2074  le, nor any of t
-00003530: 6865 6972 2065 6d70 6c6f 7965 6573 2c20  heir employees, 
-00003540: 6e6f 7220 616e 790a 6a75 7269 7364 6963  nor any.jurisdic
-00003550: 7469 6f6e 206f 7220 6f72 6761 6e69 7a61  tion or organiza
-00003560: 7469 6f6e 2074 6861 7420 6861 7320 636f  tion that has co
-00003570: 6f70 6572 6174 6564 2069 6e20 7468 6520  operated in the 
-00003580: 6465 7665 6c6f 706d 656e 7420 6f66 2074  development of t
-00003590: 6865 7365 0a6d 6174 6572 6961 6c73 2c20  hese.materials, 
-000035a0: 6d61 6b65 7320 616e 7920 7761 7272 616e  makes any warran
-000035b0: 7479 2c20 6578 7072 6573 7320 6f72 2069  ty, express or i
-000035c0: 6d70 6c69 6564 2c20 6f72 2061 7373 756d  mplied, or assum
-000035d0: 6573 2061 6e79 206c 6567 616c 0a6c 6961  es any legal.lia
-000035e0: 6269 6c69 7479 206f 7220 7265 7370 6f6e  bility or respon
-000035f0: 7369 6269 6c69 7479 2066 6f72 2074 6865  sibility for the
-00003600: 2061 6363 7572 6163 792c 2063 6f6d 706c   accuracy, compl
-00003610: 6574 656e 6573 732c 206f 7220 7573 6566  eteness, or usef
-00003620: 756c 6e65 7373 206f 7220 616e 790a 696e  ulness or any.in
-00003630: 666f 726d 6174 696f 6e2c 2061 7070 6172  formation, appar
-00003640: 6174 7573 2c20 7072 6f64 7563 742c 2073  atus, product, s
-00003650: 6f66 7477 6172 652c 206f 7220 7072 6f63  oftware, or proc
-00003660: 6573 7320 6469 7363 6c6f 7365 642c 206f  ess disclosed, o
-00003670: 7220 7265 7072 6573 656e 7473 0a74 6861  r represents.tha
-00003680: 7420 6974 7320 7573 6520 776f 756c 6420  t its use would 
-00003690: 6e6f 7420 696e 6672 696e 6765 2070 7269  not infringe pri
-000036a0: 7661 7465 6c79 206f 776e 6564 2072 6967  vately owned rig
-000036b0: 6874 732e 0a0a 5265 6665 7265 6e63 6520  hts...Reference 
-000036c0: 6865 7265 696e 2074 6f20 616e 7920 7370  herein to any sp
-000036d0: 6563 6966 6963 2063 6f6d 6d65 7263 6961  ecific commercia
-000036e0: 6c20 7072 6f64 7563 742c 2070 726f 6365  l product, proce
-000036f0: 7373 2c20 6f72 2073 6572 7669 6365 2062  ss, or service b
-00003700: 790a 7472 6164 6520 6e61 6d65 2c20 7472  y.trade name, tr
-00003710: 6164 656d 6172 6b2c 206d 616e 7566 6163  ademark, manufac
-00003720: 7475 7265 722c 206f 7220 6f74 6865 7277  turer, or otherw
-00003730: 6973 6520 646f 6573 206e 6f74 206e 6563  ise does not nec
-00003740: 6573 7361 7269 6c79 0a63 6f6e 7374 6974  essarily.constit
-00003750: 7574 6520 6f72 2069 6d70 6c79 2069 7473  ute or imply its
-00003760: 2065 6e64 6f72 7365 6d65 6e74 2c20 7265   endorsement, re
-00003770: 636f 6d6d 656e 6461 7469 6f6e 2c20 6f72  commendation, or
-00003780: 2066 6176 6f72 696e 6720 6279 2074 6865   favoring by the
-00003790: 2055 6e69 7465 640a 5374 6174 6573 2047   United.States G
-000037a0: 6f76 6572 6e6d 656e 7420 6f72 2061 6e79  overnment or any
-000037b0: 2061 6765 6e63 7920 7468 6572 656f 662c   agency thereof,
-000037c0: 206f 7220 4261 7474 656c 6c65 204d 656d   or Battelle Mem
-000037d0: 6f72 6961 6c20 496e 7374 6974 7574 652e  orial Institute.
-000037e0: 2054 6865 0a76 6965 7773 2061 6e64 206f   The.views and o
-000037f0: 7069 6e69 6f6e 7320 6f66 2061 7574 686f  pinions of autho
-00003800: 7273 2065 7870 7265 7373 6564 2068 6572  rs expressed her
-00003810: 6569 6e20 646f 206e 6f74 206e 6563 6573  ein do not neces
-00003820: 7361 7269 6c79 2073 7461 7465 206f 720a  sarily state or.
-00003830: 7265 666c 6563 7420 7468 6f73 6520 6f66  reflect those of
-00003840: 2074 6865 2055 6e69 7465 6420 5374 6174   the United Stat
-00003850: 6573 2047 6f76 6572 6e6d 656e 7420 6f72  es Government or
-00003860: 2061 6e79 2061 6765 6e63 7920 7468 6572   any agency ther
-00003870: 656f 662e 0a                             eof..
+00000020: 215b 4563 6c69 7073 6520 564f 4c54 5452  ![Eclipse VOLTTR
+00000030: 4f4e e284 a25d 2868 7474 7073 3a2f 2f69  ON...](https://i
+00000040: 6d67 2e73 6869 656c 6473 2e69 6f2f 6261  mg.shields.io/ba
+00000050: 6467 652f 4563 6c69 7073 6525 3230 564f  dge/Eclipse%20VO
+00000060: 4c54 5452 4f4e e284 a22d 2d72 6564 2e73  LTTRON...--red.s
+00000070: 7667 290a 215b 5079 7468 6f6e 2033 2e31  vg).![Python 3.1
+00000080: 305d 2868 7474 7073 3a2f 2f69 6d67 2e73  0](https://img.s
+00000090: 6869 656c 6473 2e69 6f2f 6261 6467 652f  hields.io/badge/
+000000a0: 7079 7468 6f6e 2d33 2e31 302d 626c 7565  python-3.10-blue
+000000b0: 2e73 7667 290a 215b 5079 7468 6f6e 2033  .svg).![Python 3
+000000c0: 2e31 315d 2868 7474 7073 3a2f 2f69 6d67  .11](https://img
+000000d0: 2e73 6869 656c 6473 2e69 6f2f 6261 6467  .shields.io/badg
+000000e0: 652f 7079 7468 6f6e 2d33 2e31 312d 626c  e/python-3.11-bl
+000000f0: 7565 2e73 7667 290a 5b21 5b50 6173 7369  ue.svg).[![Passi
+00000100: 6e67 3f5d 2868 7474 7073 3a2f 2f67 6974  ng?](https://git
+00000110: 6875 622e 636f 6d2f 564f 4c54 5452 4f4e  hub.com/VOLTTRON
+00000120: 2f76 6f6c 7474 726f 6e2d 6c69 622d 6d6f  /volttron-lib-mo
+00000130: 6462 7573 746b 2d64 7269 7665 722f 6163  dbustk-driver/ac
+00000140: 7469 6f6e 732f 776f 726b 666c 6f77 732f  tions/workflows/
+00000150: 7275 6e2d 7465 7374 732e 796d 6c2f 6261  run-tests.yml/ba
+00000160: 6467 652e 7376 6729 5d0a 5b21 5b70 7970  dge.svg)].[![pyp
+00000170: 6920 7665 7273 696f 6e5d 2868 7474 7073  i version](https
+00000180: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
+00000190: 6f2f 7079 7069 2f76 2f76 6f6c 7474 726f  o/pypi/v/volttro
+000001a0: 6e2d 6c69 622d 6d6f 6462 7573 746b 2d64  n-lib-modbustk-d
+000001b0: 7269 7665 722e 7376 6729 5d28 6874 7470  river.svg)](http
+000001c0: 733a 2f2f 7079 7069 2e6f 7267 2f70 726f  s://pypi.org/pro
+000001d0: 6a65 6374 2f76 6f6c 7474 726f 6e2d 6c69  ject/volttron-li
+000001e0: 622d 6d6f 6462 7573 746b 2d64 7269 7665  b-modbustk-drive
+000001f0: 722f 295d 0a0a 2323 2050 7265 7265 7175  r/)]..## Prerequ
+00000200: 6973 6974 6573 0a0a 2a20 5079 7468 6f6e  isites..* Python
+00000210: 2033 2e31 302b 0a2a 2045 636c 6970 7365   3.10+.* Eclipse
+00000220: 2056 4f4c 5454 524f 4e3c 7375 703e 746d   VOLTTRON<sup>tm
+00000230: 3c2f 7375 703e 2031 302e 302b 0a0a 2323  </sup> 10.0+..##
+00000240: 2320 5079 7468 6f6e 0a0a 3c64 6574 6169  # Python..<detai
+00000250: 6c73 3e0a 3c73 756d 6d61 7279 3e54 6f20  ls>.<summary>To 
+00000260: 696e 7374 616c 6c20 5079 7468 6f6e 2033  install Python 3
+00000270: 2e31 302c 2077 6520 7265 636f 6d6d 656e  .10, we recommen
+00000280: 6420 7573 696e 6720 3c61 2068 7265 663d  d using <a href=
+00000290: 2268 7474 7073 3a2f 2f67 6974 6875 622e  "https://github.
+000002a0: 636f 6d2f 7079 656e 762f 7079 656e 7622  com/pyenv/pyenv"
+000002b0: 3e3c 636f 6465 3e70 7965 6e76 3c2f 636f  ><code>pyenv</co
+000002c0: 6465 3e3c 2f61 3e2e 3c2f 7375 6d6d 6172  de></a>.</summar
+000002d0: 793e 0a0a 6060 6062 6173 680a 2320 696e  y>..```bash.# in
+000002e0: 7374 616c 6c20 7079 656e 760a 6769 7420  stall pyenv.git 
+000002f0: 636c 6f6e 6520 6874 7470 733a 2f2f 6769  clone https://gi
+00000300: 7468 7562 2e63 6f6d 2f70 7965 6e76 2f70  thub.com/pyenv/p
+00000310: 7965 6e76 207e 2f2e 7079 656e 760a 0a23  yenv ~/.pyenv..#
+00000320: 2073 6574 7570 2070 7965 6e76 2028 796f   setup pyenv (yo
+00000330: 7520 7368 6f75 6c64 2061 6c73 6f20 7075  u should also pu
+00000340: 7420 7468 6573 6520 7468 7265 6520 6c69  t these three li
+00000350: 6e65 7320 696e 202e 6261 7368 7263 206f  nes in .bashrc o
+00000360: 7220 7369 6d69 6c61 7229 0a65 7870 6f72  r similar).expor
+00000370: 7420 5041 5448 3d22 247b 484f 4d45 7d2f  t PATH="${HOME}/
+00000380: 2e70 7965 6e76 2f62 696e 3a24 7b50 4154  .pyenv/bin:${PAT
+00000390: 487d 220a 6578 706f 7274 2050 5945 4e56  H}".export PYENV
+000003a0: 5f52 4f4f 543d 2224 7b48 4f4d 457d 2f2e  _ROOT="${HOME}/.
+000003b0: 7079 656e 7622 0a65 7661 6c20 2224 2870  pyenv".eval "$(p
+000003c0: 7965 6e76 2069 6e69 7420 2d29 220a 0a23  yenv init -)"..#
+000003d0: 2069 6e73 7461 6c6c 2050 7974 686f 6e20   install Python 
+000003e0: 332e 380a 7079 656e 7620 696e 7374 616c  3.8.pyenv instal
+000003f0: 6c20 332e 3130 0a0a 2320 6d61 6b65 2069  l 3.10..# make i
+00000400: 7420 6176 6169 6c61 626c 6520 676c 6f62  t available glob
+00000410: 616c 6c79 0a70 7965 6e76 2067 6c6f 6261  ally.pyenv globa
+00000420: 6c20 7379 7374 656d 2033 2e31 300a 6060  l system 3.10.``
+00000430: 600a 3c2f 6465 7461 696c 733e 0a0a 0a23  `.</details>...#
+00000440: 2323 2050 6f65 7472 790a 0a54 6869 7320  ## Poetry..This 
+00000450: 7072 6f6a 6563 7420 7573 6573 2060 706f  project uses `po
+00000460: 6574 7279 6020 746f 2069 6e73 7461 6c6c  etry` to install
+00000470: 2061 6e64 206d 616e 6167 6520 6465 7065   and manage depe
+00000480: 6e64 656e 6369 6573 2e20 546f 2069 6e73  ndencies. To ins
+00000490: 7461 6c6c 2070 6f65 7472 792c 0a66 6f6c  tall poetry,.fol
+000004a0: 6c6f 7720 7468 6573 6520 5b69 6e73 7472  low these [instr
+000004b0: 7563 7469 6f6e 735d 2868 7474 7073 3a2f  uctions](https:/
+000004c0: 2f70 7974 686f 6e2d 706f 6574 7279 2e6f  /python-poetry.o
+000004d0: 7267 2f64 6f63 732f 6d61 7374 6572 2f23  rg/docs/master/#
+000004e0: 696e 7374 616c 6c61 7469 6f6e 292e 0a0a  installation)...
+000004f0: 2320 496e 7374 616c 6c61 7469 6f6e 0a0a  # Installation..
+00000500: 5769 7468 2060 7069 7060 3a0a 0a60 6060  With `pip`:..```
+00000510: 7368 656c 6c0a 7079 7468 6f6e 332e 3130  shell.python3.10
+00000520: 202d 6d20 7069 7020 696e 7374 616c 6c20   -m pip install 
+00000530: 766f 6c74 7472 6f6e 2d6c 6962 2d6d 6f64  volttron-lib-mod
+00000540: 6275 7374 6b2d 6472 6976 6572 0a0a 2320  bustk-driver..# 
+00000550: 4465 7665 6c6f 7020 6d6f 6465 0a70 7974  Develop mode.pyt
+00000560: 686f 6e33 2e31 3020 2d6d 2070 6970 2069  hon3.10 -m pip i
+00000570: 6e73 7461 6c6c 202d 2d65 6469 7461 626c  nstall --editabl
+00000580: 6520 766f 6c74 7472 6f6e 2d6c 6962 2d6d  e volttron-lib-m
+00000590: 6f64 6275 7374 6b2d 6472 6976 6572 0a60  odbustk-driver.`
+000005a0: 6060 0a0a 2323 2044 6576 656c 6f70 6d65  ``..## Developme
+000005b0: 6e74 0a0a 2323 2320 456e 7669 726f 6e6d  nt..### Environm
+000005c0: 656e 740a 0a53 6574 2074 6865 2065 6e76  ent..Set the env
+000005d0: 6972 6f6e 6d65 6e74 2074 6f20 6265 2069  ironment to be i
+000005e0: 6e20 796f 7572 2070 726f 6a65 6374 2064  n your project d
+000005f0: 6972 6563 746f 7279 3a0a 0a60 6060 706f  irectory:..```po
+00000600: 6574 7279 2063 6f6e 6669 6720 7669 7274  etry config virt
+00000610: 7561 6c65 6e76 732e 696e 2d70 726f 6a65  ualenvs.in-proje
+00000620: 6374 2074 7275 6560 6060 0a0a 4966 2079  ct true```..If y
+00000630: 6f75 2077 616e 7420 746f 2069 6e73 7461  ou want to insta
+00000640: 6c6c 2061 6c6c 2079 6f75 7220 6465 7065  ll all your depe
+00000650: 6e64 656e 6369 6573 2c20 696e 636c 7564  ndencies, includ
+00000660: 696e 6720 6465 7065 6e64 656e 6369 6573  ing dependencies
+00000670: 2074 6f20 6865 6c70 2077 6974 6820 6465   to help with de
+00000680: 7665 6c6f 7069 6e67 2079 6f75 7220 6167  veloping your ag
+00000690: 656e 742c 2072 756e 2074 6869 7320 636f  ent, run this co
+000006a0: 6d6d 616e 643a 0a0a 6060 6070 6f65 7472  mmand:..```poetr
+000006b0: 7920 696e 7374 616c 6c60 6060 0a0a 4966  y install```..If
+000006c0: 2079 6f75 2077 616e 7420 746f 2069 6e73   you want to ins
+000006d0: 7461 6c6c 206f 6e6c 7920 7468 6520 6465  tall only the de
+000006e0: 7065 6e64 656e 6369 6573 206e 6565 6465  pendencies neede
+000006f0: 6420 746f 2072 756e 2079 6f75 7220 6167  d to run your ag
+00000700: 656e 742c 2072 756e 2074 6869 7320 636f  ent, run this co
+00000710: 6d6d 616e 643a 0a0a 6060 6070 6f65 7472  mmand:..```poetr
+00000720: 7920 696e 7374 616c 6c20 2d2d 6e6f 2d64  y install --no-d
+00000730: 6576 6060 600a 0a41 6374 6976 6174 6520  ev```..Activate 
+00000740: 7468 6520 7669 7274 7561 6c20 656e 7669  the virtual envi
+00000750: 726f 6e6d 656e 743a 0a0a 6060 6073 6865  ronment:..```she
+00000760: 6c6c 0a23 2075 7369 6e67 2050 6f65 7472  ll.# using Poetr
+00000770: 790a 706f 6574 7279 2073 6865 6c6c 0a0a  y.poetry shell..
+00000780: 2320 7573 696e 6720 2773 6f75 7263 6527  # using 'source'
+00000790: 2063 6f6d 6d61 6e64 0a73 6f75 7263 6520   command.source 
+000007a0: 2224 2870 6f65 7472 7920 656e 7620 696e  "$(poetry env in
+000007b0: 666f 202d 2d70 6174 6829 2f62 696e 2f61  fo --path)/bin/a
+000007c0: 6374 6976 6174 6522 0a60 6060 0a0a 2323  ctivate".```..##
+000007d0: 2320 536f 7572 6365 2043 6f6e 7472 6f6c  # Source Control
+000007e0: 0a0a 312e 2054 6f20 7573 6520 6769 7420  ..1. To use git 
+000007f0: 746f 206d 616e 6167 6520 7665 7273 696f  to manage versio
+00000800: 6e20 636f 6e74 726f 6c2c 2063 7265 6174  n control, creat
+00000810: 6520 6120 6e65 7720 6769 7420 7265 706f  e a new git repo
+00000820: 7369 746f 7279 2069 6e20 796f 7572 206c  sitory in your l
+00000830: 6f63 616c 2061 6765 6e74 2070 726f 6a65  ocal agent proje
+00000840: 6374 2e0a 0a60 6060 6769 7420 696e 6974  ct...```git init
+00000850: 6060 600a 0a32 2e20 5468 656e 2063 7265  ```..2. Then cre
+00000860: 6174 6520 6120 6e65 7720 7265 706f 2069  ate a new repo i
+00000870: 6e20 796f 7572 2047 6974 6875 6220 6f72  n your Github or
+00000880: 2047 6974 6c61 6220 6163 636f 756e 742e   Gitlab account.
+00000890: 2043 6f70 7920 7468 6520 5552 4c20 7468   Copy the URL th
+000008a0: 6174 2070 6f69 6e74 7320 746f 2074 6861  at points to tha
+000008b0: 7420 6e65 7720 7265 706f 2069 6e0a 796f  t new repo in.yo
+000008c0: 7572 2047 6974 6875 6220 6f72 2047 6974  ur Github or Git
+000008d0: 6c61 6220 6163 636f 756e 742e 2054 6869  lab account. Thi
+000008e0: 7320 7769 6c6c 2062 6520 6b6e 6f77 6e20  s will be known 
+000008f0: 6173 206f 7572 2027 7265 6d6f 7465 272e  as our 'remote'.
+00000900: 0a0a 332e 2041 6464 2074 6865 2072 656d  ..3. Add the rem
+00000910: 6f74 6520 2869 2e65 2e20 7468 6520 6e65  ote (i.e. the ne
+00000920: 7720 7265 706f 2055 524c 2066 726f 6d20  w repo URL from 
+00000930: 796f 7572 2047 6974 6875 6220 6f72 2047  your Github or G
+00000940: 6974 6c61 6220 6163 636f 756e 7429 2074  itlab account) t
+00000950: 6f20 796f 7572 206c 6f63 616c 2072 6570  o your local rep
+00000960: 6f73 6974 6f72 792e 2052 756e 2074 6865  ository. Run the
+00000970: 2066 6f6c 6c6f 7769 6e67 2063 6f6d 6d61   following comma
+00000980: 6e64 3a0a 0a60 6060 6769 7420 7265 6d6f  nd:..```git remo
+00000990: 7465 2061 6464 206f 7269 6769 6e20 3c6d  te add origin <m
+000009a0: 7920 6769 7468 7562 2f67 6974 6c61 6220  y github/gitlab 
+000009b0: 5552 4c3e 6060 600a 0a57 6865 6e20 796f  URL>```..When yo
+000009c0: 7520 7075 7368 2074 6f20 796f 7572 2072  u push to your r
+000009d0: 6570 6f2c 206e 6f74 6520 7468 6174 2074  epo, note that t
+000009e0: 6865 2064 6566 6175 6c74 2062 7261 6e63  he default branc
+000009f0: 6820 6973 2063 616c 6c65 6420 276d 6169  h is called 'mai
+00000a00: 6e27 2e0a 0a0a 2323 2320 4f70 7469 6f6e  n'....### Option
+00000a10: 616c 2043 6f6e 6669 6775 7261 7469 6f6e  al Configuration
+00000a20: 730a 0a23 2323 2320 5072 6563 6f6d 6d69  s..#### Precommi
+00000a30: 740a 0a4e 6f74 653a 2045 6e73 7572 6520  t..Note: Ensure 
+00000a40: 7468 6174 2079 6f75 2068 6176 6520 6372  that you have cr
+00000a50: 6561 7465 6420 7468 6520 7669 7274 7561  eated the virtua
+00000a60: 6c20 656e 7669 726f 6e6d 656e 7420 7573  l environment us
+00000a70: 696e 6720 506f 6574 7279 0a0a 496e 7374  ing Poetry..Inst
+00000a80: 616c 6c20 7072 652d 636f 6d6d 6974 2068  all pre-commit h
+00000a90: 6f6f 6b73 3a0a 0a60 6060 706f 6574 7279  ooks:..```poetry
+00000aa0: 2072 756e 2070 7265 2d63 6f6d 6d69 7420   run pre-commit 
+00000ab0: 696e 7374 616c 6c60 6060 0a0a 546f 2072  install```..To r
+00000ac0: 756e 2070 7265 2d63 6f6d 6d69 7420 6f6e  un pre-commit on
+00000ad0: 2061 6c6c 2079 6f75 7220 6669 6c65 732c   all your files,
+00000ae0: 2072 756e 2074 6869 7320 636f 6d6d 616e   run this comman
+00000af0: 643a 0a0a 6060 6070 6f65 7472 7920 7275  d:..```poetry ru
+00000b00: 6e20 7072 652d 636f 6d6d 6974 2072 756e  n pre-commit run
+00000b10: 202d 2d61 6c6c 2d66 696c 6573 6060 600a   --all-files```.
+00000b20: 0a49 6620 796f 7520 6861 7665 2070 7265  .If you have pre
+00000b30: 636f 6d6d 6974 2069 6e73 7461 6c6c 6564  commit installed
+00000b40: 2061 6e64 2079 6f75 2077 616e 7420 746f   and you want to
+00000b50: 2069 676e 6f72 6520 7275 6e6e 696e 6720   ignore running 
+00000b60: 7468 6520 636f 6d6d 6974 2068 6f6f 6b73  the commit hooks
+00000b70: 0a65 7665 7279 2074 696d 6520 796f 7520  .every time you 
+00000b80: 7275 6e20 6120 636f 6d6d 6974 2c20 696e  run a commit, in
+00000b90: 636c 7564 6520 7468 6520 602d 2d6e 6f2d  clude the `--no-
+00000ba0: 7665 7269 6679 6020 666c 6167 2069 6e20  verify` flag in 
+00000bb0: 796f 7572 2063 6f6d 6d69 742e 2054 6865  your commit. The
+00000bc0: 2066 6f6c 6c6f 7769 6e67 0a69 7320 616e   following.is an
+00000bd0: 2065 7861 6d70 6c65 3a0a 0a60 6060 6769   example:..```gi
+00000be0: 7420 636f 6d6d 6974 202d 6d20 2253 6f6d  t commit -m "Som
+00000bf0: 6520 6d65 7373 6167 6522 202d 2d6e 6f2d  e message" --no-
+00000c00: 7665 7269 6679 6060 600a 0a0a 2323 2044  verify```...## D
+00000c10: 6f63 756d 656e 7461 7469 6f6e 0a0a 0a23  ocumentation...#
+00000c20: 2044 6f63 756d 656e 7461 7469 6f6e 0a4d   Documentation.M
+00000c30: 6f72 6520 6465 7461 696c 6564 2064 6f63  ore detailed doc
+00000c40: 756d 656e 7461 7469 6f6e 2063 616e 2062  umentation can b
+00000c50: 6520 666f 756e 6420 6f6e 205b 5265 6164  e found on [Read
+00000c60: 5468 6544 6f63 735d 2868 7474 7073 3a2f  TheDocs](https:/
+00000c70: 2f76 6f6c 7474 726f 6e2e 7265 6164 7468  /volttron.readth
+00000c80: 6564 6f63 732e 696f 2f65 6e2f 6d6f 6475  edocs.io/en/modu
+00000c90: 6c61 722f 292e 2054 6865 2052 5354 2073  lar/). The RST s
+00000ca0: 6f75 7263 650a 6f66 2074 6865 2064 6f63  ource.of the doc
+00000cb0: 756d 656e 7461 7469 6f6e 2066 6f72 2074  umentation for t
+00000cc0: 6869 7320 636f 6d70 6f6e 656e 7420 6973  his component is
+00000cd0: 206c 6f63 6174 6564 2069 6e20 7468 6520   located in the 
+00000ce0: 2264 6f63 7322 2064 6972 6563 746f 7279  "docs" directory
+00000cf0: 206f 6620 7468 6973 2072 6570 6f73 6974   of this reposit
+00000d00: 6f72 792e 0a0a 2320 496e 7374 616c 6c61  ory...# Installa
+00000d10: 7469 6f6e 0a0a 4265 666f 7265 2069 6e73  tion..Before ins
+00000d20: 7461 6c6c 696e 672c 2056 4f4c 5454 524f  talling, VOLTTRO
+00000d30: 4e20 7368 6f75 6c64 2062 6520 696e 7374  N should be inst
+00000d40: 616c 6c65 6420 616e 6420 7275 6e6e 696e  alled and runnin
+00000d50: 672e 2020 4974 7320 7669 7274 7561 6c20  g.  Its virtual 
+00000d60: 656e 7669 726f 6e6d 656e 7420 7368 6f75  environment shou
+00000d70: 6c64 2062 6520 6163 7469 7665 2e0a 496e  ld be active..In
+00000d80: 666f 726d 6174 696f 6e20 6f6e 2068 6f77  formation on how
+00000d90: 2074 6f20 696e 7374 616c 6c20 6f66 2074   to install of t
+00000da0: 6865 2056 4f4c 5454 524f 4e20 706c 6174  he VOLTTRON plat
+00000db0: 666f 726d 2063 616e 2062 6520 666f 756e  form can be foun
+00000dc0: 640a 5b68 6572 655d 2868 7474 7073 3a2f  d.[here](https:/
+00000dd0: 2f67 6974 6875 622e 636f 6d2f 6563 6c69  /github.com/ecli
+00000de0: 7073 652d 766f 6c74 7472 6f6e 2f76 6f6c  pse-volttron/vol
+00000df0: 7474 726f 6e2d 636f 7265 292e 0a0a 312e  ttron-core)...1.
+00000e00: 2049 6620 6974 2069 7320 6e6f 7420 616c   If it is not al
+00000e10: 7265 6164 792c 2069 6e73 7461 6c6c 2074  ready, install t
+00000e20: 6865 2056 4f4c 5454 524f 4e20 506c 6174  he VOLTTRON Plat
+00000e30: 666f 726d 2044 7269 7665 7220 4167 656e  form Driver Agen
+00000e40: 743a 0a0a 2020 2020 6060 6073 6865 6c6c  t:..    ```shell
+00000e50: 0a20 2020 2076 6374 6c20 696e 7374 616c  .    vctl instal
+00000e60: 6c20 766f 6c74 7472 6f6e 2d70 6c61 7466  l volttron-platf
+00000e70: 6f72 6d2d 6472 6976 6572 202d 2d76 6970  orm-driver --vip
+00000e80: 2d69 6465 6e74 6974 7920 706c 6174 666f  -identity platfo
+00000e90: 726d 2e64 7269 7665 7220 2d2d 7374 6172  rm.driver --star
+00000ea0: 740a 2020 2020 6060 600a 0a31 2e20 496e  t.    ```..1. In
+00000eb0: 7374 616c 6c20 7468 6520 766f 6c74 7472  stall the volttr
+00000ec0: 6f6e 2d6c 6962 2d6d 6f64 6275 7374 6b2d  on-lib-modbustk-
+00000ed0: 6472 6976 6572 206c 6962 7261 7279 2e0a  driver library..
+00000ee0: 0a20 2020 2060 6060 7368 656c 6c0a 2020  .    ```shell.  
+00000ef0: 2020 7069 7020 696e 7374 616c 6c20 766f    pip install vo
+00000f00: 6c74 7472 6f6e 2d6c 6962 2d6d 6f64 6275  lttron-lib-modbu
+00000f10: 7374 6b2d 6472 6976 6572 0a20 2020 2060  stk-driver.    `
+00000f20: 6060 0a0a 312e 2049 6e73 7461 6c6c 2074  ``..1. Install t
+00000f30: 6865 2064 7269 7665 7220 6f6e 746f 2074  he driver onto t
+00000f40: 6865 2050 6c61 7466 6f72 6d20 4472 6976  he Platform Driv
+00000f50: 6572 2e0a 0a20 2020 2049 6e73 7461 6c6c  er...    Install
+00000f60: 696e 6720 6120 6472 6976 6572 2069 6e20  ing a driver in 
+00000f70: 7468 6520 506c 6174 666f 726d 2044 7269  the Platform Dri
+00000f80: 7665 7220 4167 656e 7420 7265 7175 6972  ver Agent requir
+00000f90: 6573 2061 6464 696e 6720 636f 7069 6573  es adding copies
+00000fa0: 206f 6620 7468 6520 6465 7669 6365 2063   of the device c
+00000fb0: 6f6e 6669 6775 7261 7469 6f6e 2061 6e64  onfiguration and
+00000fc0: 2072 6567 6973 7472 7920 636f 6e66 6967   registry config
+00000fd0: 7572 6174 696f 6e20 6669 6c65 7320 746f  uration files to
+00000fe0: 2074 6865 2050 6c61 7466 6f72 6d20 4472   the Platform Dr
+00000ff0: 6976 6572 e280 9973 2063 6f6e 6669 6775  iver...s configu
+00001000: 7261 7469 6f6e 2073 746f 7265 2e0a 0a20  ration store... 
+00001010: 2020 2043 7265 6174 6520 6120 636f 6e66     Create a conf
+00001020: 6967 2064 6972 6563 746f 7279 2061 6e64  ig directory and
+00001030: 206e 6176 6967 6174 6520 746f 2069 743a   navigate to it:
+00001040: 0a0a 2020 2020 6060 6073 6865 6c6c 0a20  ..    ```shell. 
+00001050: 2020 206d 6b64 6972 2063 6f6e 6669 670a     mkdir config.
+00001060: 2020 2020 6364 2063 6f6e 6669 670a 2020      cd config.  
+00001070: 2020 6060 600a 0a31 2e20 4164 6420 6472    ```..1. Add dr
+00001080: 6976 6572 2063 6f6e 6669 6775 7261 7469  iver configurati
+00001090: 6f6e 7320 746f 2074 6865 2050 6c61 7466  ons to the Platf
+000010a0: 6f72 6d20 4472 6976 6572 2e0a 0a20 2020  orm Driver...   
+000010b0: 5468 6520 4d6f 6462 7573 2d54 4b20 6472  The Modbus-TK dr
+000010c0: 6976 6572 2069 7320 6d6f 7374 6c79 2062  iver is mostly b
+000010d0: 6163 6b77 6172 642d 636f 6d70 6174 6962  ackward-compatib
+000010e0: 6c65 2077 6974 6820 7468 6520 7061 7261  le with the para
+000010f0: 6d65 7465 7220 6465 6669 6e69 7469 6f6e  meter definition
+00001100: 7320 696e 2074 6865 206f 7269 6769 6e61  s in the origina
+00001110: 6c20 4d6f 6462 7573 2064 7269 7665 72e2  l Modbus driver.
+00001120: 8099 7320 636f 6e66 6967 7572 6174 696f  ..s configuratio
+00001130: 6e20 282e 636f 6e66 6967 2061 6e64 202e  n (.config and .
+00001140: 6373 7620 6669 6c65 7329 2e20 4966 2074  csv files). If t
+00001150: 6865 2063 6f6e 6669 6720 6669 6c65 e280  he config file..
+00001160: 9973 2070 6172 616d 6574 6572 206e 616d  .s parameter nam
+00001170: 6573 2075 7365 2074 6865 204d 6f64 6275  es use the Modbu
+00001180: 7320 6472 6976 6572 e280 9973 206e 616d  s driver...s nam
+00001190: 6520 636f 6e76 656e 7469 6f6e 732c 2074  e conventions, t
+000011a0: 6865 7920 6172 6520 7472 616e 736c 6174  hey are translat
+000011b0: 6564 2074 6f20 7468 6520 4d6f 6462 7573  ed to the Modbus
+000011c0: 2d54 4b20 6e61 6d65 2063 6f6e 7665 6e74  -TK name convent
+000011d0: 696f 6e73 2c20 652e 672e 2061 204d 6f64  ions, e.g. a Mod
+000011e0: 6275 7320 4353 5620 6669 6c65 e280 9973  bus CSV file...s
+000011f0: 2050 6f69 6e74 2041 6464 7265 7373 2069   Point Address i
+00001200: 7320 696e 7465 7270 7265 7465 6420 6173  s interpreted as
+00001210: 2061 204d 6f64 6275 732d 544b 20e2 809c   a Modbus-TK ...
+00001220: 4164 6472 6573 73e2 809d 2e20 4261 636b  Address.... Back
+00001230: 7761 7264 2d63 6f6d 7061 7469 6269 6c69  ward-compatibili
+00001240: 7479 2065 7863 6570 7469 6f6e 7320 6172  ty exceptions ar
+00001250: 653a 0a0a 2020 2020 2020 2020 2a20 4966  e:..        * If
+00001260: 2074 6865 2063 6f6e 6669 6720 6669 6c65   the config file
+00001270: 2068 6173 206e 6f20 706f 7274 2c20 7468   has no port, th
+00001280: 6520 6465 6661 756c 7420 6973 2030 2c20  e default is 0, 
+00001290: 6e6f 7420 3530 322e 0a0a 2020 2020 2020  not 502...      
+000012a0: 2020 2a20 4966 2074 6865 2063 6f6e 6669    * If the confi
+000012b0: 6720 6669 6c65 2068 6173 206e 6f20 736c  g file has no sl
+000012c0: 6176 655f 6964 2c20 7468 6520 6465 6661  ave_id, the defa
+000012d0: 756c 7420 6973 2031 2c20 6e6f 7420 302e  ult is 1, not 0.
+000012e0: 0a0a 2020 2020 5468 6520 6472 6976 6572  ..    The driver
+000012f0: 5f63 6f6e 6669 6720 7365 6374 696f 6e20  _config section 
+00001300: 6f66 2061 204d 6f64 6275 732d 544b 2064  of a Modbus-TK d
+00001310: 6576 6963 6520 636f 6e66 6967 7572 6174  evice configurat
+00001320: 696f 6e20 6669 6c65 2073 7570 706f 7274  ion file support
+00001330: 7320 6120 7661 7269 6574 7920 6f66 2070  s a variety of p
+00001340: 6172 616d 6574 6572 2064 6566 696e 6974  arameter definit
+00001350: 696f 6e73 2c20 6275 7420 6f6e 6c79 202a  ions, but only *
+00001360: 6465 7669 6365 5f61 6464 7265 7373 2a20  device_address* 
+00001370: 6973 2072 6571 7569 7265 643a 0a0a 2020  is required:..  
+00001380: 2020 2a20 6465 7669 6365 5f61 6464 7265    * device_addre
+00001390: 7373 2028 5265 7175 6972 6564 293a 2020  ss (Required):  
+000013a0: 4950 2041 6464 7265 7373 206f 6620 7468  IP Address of th
+000013b0: 6520 6465 7669 6365 2e0a 0a20 2020 202a  e device...    *
+000013c0: 206e 616d 6520 284f 7074 696f 6e61 6c29   name (Optional)
+000013d0: 202d 204e 616d 6520 6f66 2074 6865 2064   - Name of the d
+000013e0: 6576 6963 652e 2044 6566 6175 6c74 7320  evice. Defaults 
+000013f0: 746f 20e2 809c 554e 4b4e 4f57 4ee2 809d  to ...UNKNOWN...
+00001400: 2e0a 0a20 2020 202a 2064 6576 6963 655f  ...    * device_
+00001410: 7479 7065 2028 4f70 7469 6f6e 616c 2920  type (Optional) 
+00001420: 2d20 4e61 6d65 206f 6620 7468 6520 6465  - Name of the de
+00001430: 7669 6365 2074 7970 652e 2044 6566 6175  vice type. Defau
+00001440: 6c74 7320 746f 20e2 809c 554e 4b4e 4f57  lts to ...UNKNOW
+00001450: 4ee2 809d 2e0a 0a20 2020 202a 2070 6f72  N......    * por
+00001460: 7420 284f 7074 696f 6e61 6c29 202d 2050  t (Optional) - P
+00001470: 6f72 7420 7468 6520 6465 7669 6365 2069  ort the device i
+00001480: 7320 6c69 7374 656e 696e 6720 6f6e 2e20  s listening on. 
+00001490: 4465 6661 756c 7473 2074 6f20 3020 286e  Defaults to 0 (n
+000014a0: 6f20 706f 7274 292e 2055 7365 2070 6f72  o port). Use por
+000014b0: 7420 3020 666f 7220 5254 5520 7472 616e  t 0 for RTU tran
+000014c0: 7370 6f72 742e 0a0a 2020 2020 2a20 736c  sport...    * sl
+000014d0: 6176 655f 6964 2028 4f70 7469 6f6e 616c  ave_id (Optional
+000014e0: 2920 2d20 536c 6176 6520 4944 206f 6620  ) - Slave ID of 
+000014f0: 7468 6520 6465 7669 6365 2e20 4465 6661  the device. Defa
+00001500: 756c 7473 2074 6f20 312e 2055 7365 2049  ults to 1. Use I
+00001510: 4420 3020 666f 7220 6e6f 2073 6c61 7665  D 0 for no slave
+00001520: 2e0a 0a20 2020 202a 2062 6175 6472 6174  ...    * baudrat
+00001530: 6520 284f 7074 696f 6e61 6c29 202d 2053  e (Optional) - S
+00001540: 6572 6961 6c20 2852 5455 2920 6261 7564  erial (RTU) baud
+00001550: 2072 6174 652e 2044 6566 6175 6c74 7320   rate. Defaults 
+00001560: 746f 2039 3630 302e 0a0a 2020 2020 2a20  to 9600...    * 
+00001570: 6279 7465 7369 7a65 2028 4f70 7469 6f6e  bytesize (Option
+00001580: 616c 2920 2d20 5365 7269 616c 2028 5254  al) - Serial (RT
+00001590: 5529 2062 7974 6520 7369 7a65 3a20 352c  U) byte size: 5,
+000015a0: 2036 2c20 372c 206f 7220 382e 2044 6566   6, 7, or 8. Def
+000015b0: 6175 6c74 7320 746f 2038 2e0a 0a20 2020  aults to 8...   
+000015c0: 202a 2070 6172 6974 7920 284f 7074 696f   * parity (Optio
+000015d0: 6e61 6c29 202d 2053 6572 6961 6c20 2852  nal) - Serial (R
+000015e0: 5455 2920 7061 7269 7479 3a20 6e6f 6e65  TU) parity: none
+000015f0: 2c20 6576 656e 2c20 6f64 642c 206d 6172  , even, odd, mar
+00001600: 6b2c 206f 7220 7370 6163 652e 2044 6566  k, or space. Def
+00001610: 6175 6c74 7320 746f 204e 6f6e 652e 0a0a  aults to None...
+00001620: 2020 2020 2a20 7374 6f70 6269 7473 2028      * stopbits (
+00001630: 4f70 7469 6f6e 616c 2920 2d20 5365 7269  Optional) - Seri
+00001640: 616c 2028 5254 5529 2073 746f 7020 6269  al (RTU) stop bi
+00001650: 7473 3a20 312c 2031 2e35 2c20 6f72 2032  ts: 1, 1.5, or 2
+00001660: 2e20 4465 6661 756c 7473 2074 6f20 312e  . Defaults to 1.
+00001670: 0a0a 2020 2020 2a20 786f 6e78 6f66 6620  ..    * xonxoff 
+00001680: 284f 7074 696f 6e61 6c29 202d 2053 6572  (Optional) - Ser
+00001690: 6961 6c20 2852 5455 2920 666c 6f77 2063  ial (RTU) flow c
+000016a0: 6f6e 7472 6f6c 3a20 3020 6f72 2031 2e20  ontrol: 0 or 1. 
+000016b0: 4465 6661 756c 7473 2074 6f20 302e 0a0a  Defaults to 0...
+000016c0: 2020 2020 2a20 6164 6472 6573 7369 6e67      * addressing
+000016d0: 2028 4f70 7469 6f6e 616c 2920 2d20 4461   (Optional) - Da
+000016e0: 7461 2061 6464 7265 7373 2074 6162 6c65  ta address table
+000016f0: 3a20 6f66 6673 6574 2c20 6f66 6673 6574  : offset, offset
+00001700: 5f70 6c75 732c 206f 7220 6164 6472 6573  _plus, or addres
+00001710: 732e 2044 6566 6175 6c74 7320 746f 206f  s. Defaults to o
+00001720: 6666 7365 742e 0a0a 2020 2020 2020 2a20  ffset...      * 
+00001730: 6164 6472 6573 733a 2054 6865 2065 7861  address: The exa
+00001740: 6374 2076 616c 7565 206f 6620 7468 6520  ct value of the 
+00001750: 6164 6472 6573 7320 7769 7468 6f75 7420  address without 
+00001760: 616e 7920 6f66 6673 6574 2076 616c 7565  any offset value
+00001770: 2e0a 0a20 2020 2020 202a 206f 6666 7365  ...      * offse
+00001780: 743a 2054 6865 2076 616c 7565 206f 6620  t: The value of 
+00001790: 7468 6520 6164 6472 6573 7320 706c 7573  the address plus
+000017a0: 2074 6865 206f 6666 7365 7420 7661 6c75   the offset valu
+000017b0: 652e 0a0a 2020 2020 2020 2a20 6f66 6673  e...      * offs
+000017c0: 6574 5f70 6c75 733a 2054 6865 2076 616c  et_plus: The val
+000017d0: 7565 206f 6620 7468 6520 6164 6472 6573  ue of the addres
+000017e0: 7320 706c 7573 2074 6865 206f 6666 7365  s plus the offse
+000017f0: 7420 7661 6c75 6520 706c 7573 206f 6e65  t value plus one
+00001800: 2e0a 0a20 2020 2020 202a 203a 2049 6620  ...      * : If 
+00001810: 616e 206f 6666 7365 7420 7661 6c75 6520  an offset value 
+00001820: 6973 2074 6f20 6265 2061 6464 6564 2c20  is to be added, 
+00001830: 6974 2069 7320 6465 7465 726d 696e 6564  it is determined
+00001840: 2062 6173 6564 206f 6e20 6120 706f 696e   based on a poin
+00001850: 74e2 8099 7320 7072 6f70 6572 7469 6573  t...s properties
+00001860: 2069 6e20 7468 6520 4353 5620 6669 6c65   in the CSV file
+00001870: 3a0a 0a20 2020 2020 2020 202a 2054 7970  :..        * Typ
+00001880: 653d 626f 6f6c 2c20 5772 6974 6162 6c65  e=bool, Writable
+00001890: 3d54 5255 453a 2030 0a0a 2020 2020 2020  =TRUE: 0..      
+000018a0: 2020 2a20 5479 7065 3d62 6f6f 6c2c 2057    * Type=bool, W
+000018b0: 7269 7461 626c 653d 4641 4c53 453a 2031  ritable=FALSE: 1
+000018c0: 3030 3030 0a0a 2020 2020 2020 2020 2a20  0000..        * 
+000018d0: 5479 7065 213d 626f 6f6c 2c20 5772 6974  Type!=bool, Writ
+000018e0: 6162 6c65 3d54 5255 453a 2033 3030 3030  able=TRUE: 30000
+000018f0: 0a0a 2020 2020 2020 2020 2a20 5479 7065  ..        * Type
+00001900: 213d 626f 6f6c 2c20 5772 6974 6162 6c65  !=bool, Writable
+00001910: 3d46 414c 5345 3a20 3430 3030 300a 0a20  =FALSE: 40000.. 
+00001920: 2020 202a 2065 6e64 6961 6e20 284f 7074     * endian (Opt
+00001930: 696f 6e61 6c29 202d 2042 7974 6520 6f72  ional) - Byte or
+00001940: 6465 723a 2062 6967 206f 7220 6c69 7474  der: big or litt
+00001950: 6c65 2e20 4465 6661 756c 7473 2074 6f20  le. Defaults to 
+00001960: 6269 672e 0a0a 2020 2020 2a20 7772 6974  big...    * writ
+00001970: 655f 6d75 6c74 6970 6c65 5f72 6567 6973  e_multiple_regis
+00001980: 7465 7273 2028 4f70 7469 6f6e 616c 2920  ters (Optional) 
+00001990: 2d20 5772 6974 6520 6d75 6c74 6970 6c65  - Write multiple
+000019a0: 2063 6f69 6c73 206f 7220 7265 6769 7374   coils or regist
+000019b0: 6572 7320 6174 2061 2074 696d 652e 2044  ers at a time. D
+000019c0: 6566 6175 6c74 7320 746f 2074 7275 652e  efaults to true.
+000019d0: 0a0a 2020 2020 2020 2a20 4966 2077 7269  ..      * If wri
+000019e0: 7465 5f6d 756c 7469 706c 655f 7265 6769  te_multiple_regi
+000019f0: 7374 6572 7320 6973 2073 6574 2074 6f20  sters is set to 
+00001a00: 6661 6c73 652c 206f 6e6c 7920 7265 6769  false, only regi
+00001a10: 7374 6572 2074 7970 6573 2075 6e73 6967  ster types unsig
+00001a20: 6e65 6420 7368 6f72 7420 2875 696e 7431  ned short (uint1
+00001a30: 3629 2061 6e64 2062 6f6f 6c65 616e 2028  6) and boolean (
+00001a40: 626f 6f6c 2920 6172 6520 7375 7070 6f72  bool) are suppor
+00001a50: 7465 642e 2054 6865 2065 7863 6570 7469  ted. The excepti
+00001a60: 6f6e 2072 6169 7365 6420 6475 7269 6e67  on raised during
+00001a70: 2074 6865 2063 6f6e 6669 6775 7265 2070   the configure p
+00001a80: 726f 6365 7373 2e0a 0a20 2020 202a 2072  rocess...    * r
+00001a90: 6567 6973 7465 725f 6d61 7020 284f 7074  egister_map (Opt
+00001aa0: 696f 6e61 6c29 202d 2052 6567 6973 7465  ional) - Registe
+00001ab0: 7220 6d61 7020 6373 7620 6f66 2075 6e63  r map csv of unc
+00001ac0: 6861 6e67 6564 2072 6567 6973 7465 7220  hanged register 
+00001ad0: 7661 7269 6162 6c65 732e 2044 6566 6175  variables. Defau
+00001ae0: 6c74 7320 746f 2072 6567 6973 7472 795f  lts to registry_
+00001af0: 636f 6e66 6967 2063 7376 2e0a 0a20 2020  config csv...   
+00001b00: 2054 6869 7320 7265 706f 2070 726f 7669   This repo provi
+00001b10: 6465 7320 616e 2065 7861 6d70 6c65 2063  des an example c
+00001b20: 6f6e 6669 6775 7261 7469 6f6e 2069 6e20  onfiguration in 
+00001b30: 7468 6520 6669 6c65 2022 6d6f 6462 7573  the file "modbus
+00001b40: 5f74 6b5f 6578 616d 706c 652e 636f 6e66  _tk_example.conf
+00001b50: 6967 222e 0a0a 2020 2020 4865 7265 2069  ig"...    Here i
+00001b60: 7320 616e 2065 7861 6d70 6c65 2064 6576  s an example dev
+00001b70: 6963 6520 636f 6e66 6967 7572 6174 696f  ice configuratio
+00001b80: 6e20 6669 6c65 3a0a 0a20 2020 2060 6060  n file:..    ```
+00001b90: 6a73 6f6e 0a20 2020 2020 2020 207b 0a20  json.        {. 
+00001ba0: 2020 2020 2020 2022 6472 6976 6572 5f63         "driver_c
+00001bb0: 6f6e 6669 6722 3a20 7b0a 2020 2020 2020  onfig": {.      
+00001bc0: 2020 2020 2020 2264 6576 6963 655f 6164        "device_ad
+00001bd0: 6472 6573 7322 3a20 2231 302e 312e 312e  dress": "10.1.1.
+00001be0: 3222 2c0a 2020 2020 2020 2020 2020 2020  2",.            
+00001bf0: 2270 6f72 7422 3a20 2235 3032 3022 2c0a  "port": "5020",.
+00001c00: 2020 2020 2020 2020 2020 2020 2272 6567              "reg
+00001c10: 6973 7465 725f 6d61 7022 3a20 2263 6f6e  ister_map": "con
+00001c20: 6669 673a 2f2f 6d6f 6462 7573 5f74 6b5f  fig://modbus_tk_
+00001c30: 7465 7374 5f6d 6170 2e63 7376 220a 2020  test_map.csv".  
+00001c40: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
+00001c50: 2022 6472 6976 6572 5f74 7970 6522 3a20   "driver_type": 
+00001c60: 226d 6f64 6275 735f 746b 222c 0a20 2020  "modbus_tk",.   
+00001c70: 2020 2020 2022 7265 6769 7374 7279 5f63       "registry_c
+00001c80: 6f6e 6669 6722 3a20 2263 6f6e 6669 673a  onfig": "config:
+00001c90: 2f2f 6d6f 6462 7573 5f74 6b5f 7465 7374  //modbus_tk_test
+00001ca0: 2e63 7376 222c 0a20 2020 2020 2020 2022  .csv",.        "
+00001cb0: 696e 7465 7276 616c 223a 2036 302c 0a20  interval": 60,. 
+00001cc0: 2020 2020 2020 2022 7469 6d65 7a6f 6e65         "timezone
+00001cd0: 223a 2022 5554 4322 2c0a 2020 2020 2020  ": "UTC",.      
+00001ce0: 2020 2268 6561 7274 5f62 6561 745f 706f    "heart_beat_po
+00001cf0: 696e 7422 3a20 2268 6561 7274 6265 6174  int": "heartbeat
+00001d00: 220a 2020 2020 2020 2020 7d0a 2020 2020  ".        }.    
+00001d10: 6060 600a 0a20 2020 2041 6674 6572 2063  ```..    After c
+00001d20: 7265 6174 696e 6720 6120 6472 6976 6572  reating a driver
+00001d30: 2063 6f6e 6669 6775 7261 7469 6f6e 2066   configuration f
+00001d40: 696c 6520 6e61 6d65 6420 226d 6f64 6275  ile named "modbu
+00001d50: 735f 746b 5f65 7861 6d70 6c65 2e63 6f6e  s_tk_example.con
+00001d60: 6669 6722 2c20 6164 6420 6974 2074 6f20  fig", add it to 
+00001d70: 7468 6520 436f 6e66 6967 7572 6174 696f  the Configuratio
+00001d80: 6e20 5374 6f72 653a 0a0a 2020 2020 6060  n Store:..    ``
+00001d90: 6073 6865 6c6c 0a20 2020 2076 6374 6c20  `shell.    vctl 
+00001da0: 636f 6e66 6967 2073 746f 7265 2070 6c61  config store pla
+00001db0: 7466 6f72 6d2e 6472 6976 6572 2064 6576  tform.driver dev
+00001dc0: 6963 6573 2f6d 6f64 6275 7374 6b20 6d6f  ices/modbustk mo
+00001dd0: 6462 7573 5f74 6b5f 6578 616d 706c 652e  dbus_tk_example.
+00001de0: 636f 6e66 6967 0a20 2020 2060 6060 0a0a  config.    ```..
+00001df0: 312e 2041 6464 2061 204d 6f64 6275 732d  1. Add a Modbus-
+00001e00: 544b 2052 6567 6973 7465 7220 4d61 7020  TK Register Map 
+00001e10: 4353 5620 4669 6c65 2074 6f20 7468 6520  CSV File to the 
+00001e20: 506c 6174 666f 726d 2044 7269 7665 722e  Platform Driver.
+00001e30: 0a0a 2020 2020 4d6f 6462 7573 2054 4b20  ..    Modbus TK 
+00001e40: 7265 7175 6972 6573 2061 6e20 6164 6469  requires an addi
+00001e50: 7469 6f6e 616c 2072 6567 6973 7472 7920  tional registry 
+00001e60: 636f 6e66 6967 7572 6174 696f 6e20 6669  configuration fi
+00001e70: 6c65 2063 6f6d 7061 7265 6420 746f 2074  le compared to t
+00001e80: 6865 2070 6172 6164 6967 6d20 6f66 206d  he paradigm of m
+00001e90: 6f73 7420 6f74 6865 7220 6472 6976 6572  ost other driver
+00001ea0: 732e 2054 6865 2072 6567 6973 7472 7920  s. The registry 
+00001eb0: 6d61 7020 6669 6c65 2069 7320 616e 2061  map file is an a
+00001ec0: 6e61 6c6f 6775 6520 746f 2074 6865 2074  nalogue to the t
+00001ed0: 7970 6963 616c 2072 6567 6973 7472 7920  ypical registry 
+00001ee0: 636f 6e66 6967 7572 6174 696f 6e20 6669  configuration fi
+00001ef0: 6c65 2e20 5468 6520 7265 6769 7374 7279  le. The registry
+00001f00: 2063 6f6e 6669 6775 7261 7469 6f6e 2066   configuration f
+00001f10: 696c 6520 6973 2061 2073 696d 706c 6520  ile is a simple 
+00001f20: 6669 6c65 2077 6869 6368 206d 6170 7320  file which maps 
+00001f30: 6465 7669 6365 2070 6f69 6e74 206e 616d  device point nam
+00001f40: 6573 2074 6f20 7573 6572 2073 7065 6369  es to user speci
+00001f50: 6669 6564 2070 6f69 6e74 206e 616d 6573  fied point names
+00001f60: 2e0a 0a20 2020 2054 6869 7320 7265 706f  ...    This repo
+00001f70: 2070 726f 7669 6465 7320 616e 2065 7861   provides an exa
+00001f80: 6d70 6c65 2063 6f6e 6669 6775 7261 7469  mple configurati
+00001f90: 6f6e 2069 6e20 7468 6520 6669 6c65 2022  on in the file "
+00001fa0: 6d6f 6462 7573 5f74 6b5f 7465 7374 5f6d  modbus_tk_test_m
+00001fb0: 6170 2e63 7376 222e 0a0a 2020 2020 5468  ap.csv"...    Th
+00001fc0: 6520 7265 6769 7374 7279 206d 6170 2066  e registry map f
+00001fd0: 696c 6520 6973 2061 2043 5356 2066 696c  ile is a CSV fil
+00001fe0: 652e 2045 6163 6820 726f 7720 636f 6e66  e. Each row conf
+00001ff0: 6967 7572 6573 2061 2072 6567 6973 7465  igures a registe
+00002000: 7220 6465 6669 6e69 7469 6f6e 206f 6e20  r definition on 
+00002010: 7468 6520 6465 7669 6365 2e0a 0a20 2020  the device...   
+00002020: 2052 6567 6973 7465 7220 4e61 6d65 2028   Register Name (
+00002030: 5265 7175 6972 6564 2920 2d20 5468 6520  Required) - The 
+00002040: 6669 656c 6420 6e61 6d65 2069 6e20 7468  field name in th
+00002050: 6520 6d6f 6462 7573 2063 6c69 656e 742e  e modbus client.
+00002060: 2054 6869 7320 6669 656c 6420 6973 2064   This field is d
+00002070: 6973 7469 6e63 7420 616e 6420 756e 6368  istinct and unch
+00002080: 616e 6765 6162 6c65 2e0a 0a20 2020 2041  angeable...    A
+00002090: 6464 7265 7373 2028 5265 7175 6972 6564  ddress (Required
+000020a0: 2920 2d20 5468 6520 706f 696e 74e2 8099  ) - The point...
+000020b0: 7320 6d6f 6462 7573 2061 6464 7265 7373  s modbus address
+000020c0: 2e20 5468 6520 6164 6472 6573 7369 6e67  . The addressing
+000020d0: 206f 7074 696f 6e20 696e 2074 6865 2064   option in the d
+000020e0: 7269 7665 7220 636f 6e66 6967 7572 6174  river configurat
+000020f0: 696f 6e20 636f 6e74 726f 6c73 2077 6865  ion controls whe
+00002100: 7468 6572 2074 6869 7320 6973 2069 6e74  ther this is int
+00002110: 6572 7072 6574 6564 2061 7320 616e 2065  erpreted as an e
+00002120: 7861 6374 2061 6464 7265 7373 206f 7220  xact address or 
+00002130: 616e 206f 6666 7365 742e 0a0a 2020 2020  an offset...    
+00002140: 5479 7065 2028 5265 7175 6972 6564 2920  Type (Required) 
+00002150: 2d20 5468 6520 706f 696e 74e2 8099 7320  - The point...s 
+00002160: 6461 7461 2074 7970 653a 2062 6f6f 6c2c  data type: bool,
+00002170: 2073 7472 696e 675b 6c65 6e67 7468 5d2c   string[length],
+00002180: 2066 6c6f 6174 2c20 696e 7431 362c 2069   float, int16, i
+00002190: 6e74 3332 2c20 696e 7436 342c 2075 696e  nt32, int64, uin
+000021a0: 7431 362c 2075 696e 7433 322c 206f 7220  t16, uint32, or 
+000021b0: 7569 6e74 3634 2e0a 0a20 2020 2055 6e69  uint64...    Uni
+000021c0: 7473 2028 4f70 7469 6f6e 616c 2920 2d20  ts (Optional) - 
+000021d0: 5573 6564 2066 6f72 206d 6574 6164 6174  Used for metadat
+000021e0: 6120 7768 656e 2063 7265 6174 696e 6720  a when creating 
+000021f0: 706f 696e 7420 696e 666f 726d 6174 696f  point informatio
+00002200: 6e20 6f6e 2061 2068 6973 746f 7269 616e  n on a historian
+00002210: 2e20 4465 6661 756c 7420 6973 2061 6e20  . Default is an 
+00002220: 656d 7074 7920 7374 7269 6e67 2e0a 0a20  empty string... 
+00002230: 2020 2057 7269 7461 626c 6520 284f 7074     Writable (Opt
+00002240: 696f 6e61 6c29 202d 2054 5255 452f 4641  ional) - TRUE/FA
+00002250: 4c53 452e 204f 6e6c 7920 706f 696e 7473  LSE. Only points
+00002260: 2066 6f72 2077 6869 6368 2057 7269 7461   for which Writa
+00002270: 626c 653d 5452 5545 2063 616e 2062 6520  ble=TRUE can be 
+00002280: 7570 6461 7465 6420 6279 2061 2056 4f4c  updated by a VOL
+00002290: 5454 524f 4e20 6167 656e 742e 2044 6566  TTRON agent. Def
+000022a0: 6175 6c74 2069 7320 4641 4c53 452e 0a0a  ault is FALSE...
+000022b0: 2020 2020 4465 6661 756c 7420 5661 6c75      Default Valu
+000022c0: 6520 284f 7074 696f 6e61 6c29 202d 2054  e (Optional) - T
+000022d0: 6865 2070 6f69 6e74 e280 9973 2064 6566  he point...s def
+000022e0: 6175 6c74 2076 616c 7565 2e20 4966 2069  ault value. If i
+000022f0: 7420 6973 2072 6576 6572 7465 6420 6279  t is reverted by
+00002300: 2061 6e20 6167 656e 742c 2069 7420 6368   an agent, it ch
+00002310: 616e 6765 7320 6261 636b 2074 6f20 7468  anges back to th
+00002320: 6973 2076 616c 7565 2e20 4966 2074 6869  is value. If thi
+00002330: 7320 7661 6c75 6520 6973 206d 6973 7369  s value is missi
+00002340: 6e67 2c20 6974 2077 696c 6c20 7265 7665  ng, it will reve
+00002350: 7274 2074 6f20 7468 6520 6c61 7374 206b  rt to the last k
+00002360: 6e6f 776e 2076 616c 7565 206e 6f74 2073  nown value not s
+00002370: 6574 2062 7920 616e 2061 6765 6e74 2e0a  et by an agent..
+00002380: 0a20 2020 2054 7261 6e73 666f 726d 2028  .    Transform (
+00002390: 4f70 7469 6f6e 616c 2920 2d20 5363 616c  Optional) - Scal
+000023a0: 696e 6720 616c 676f 7269 7468 6d3a 2073  ing algorithm: s
+000023b0: 6361 6c65 286d 756c 7469 706c 6965 7229  cale(multiplier)
+000023c0: 2c20 7363 616c 655f 696e 7428 6d75 6c74  , scale_int(mult
+000023d0: 6970 6c69 6572 292c 2073 6361 6c65 5f72  iplier), scale_r
+000023e0: 6567 2872 6567 6973 7465 725f 6e61 6d65  eg(register_name
+000023f0: 292c 2073 6361 6c65 5f72 6567 5f70 6f77  ), scale_reg_pow
+00002400: 6572 3130 2872 6567 6973 7465 725f 6e61  er10(register_na
+00002410: 6d65 292c 2073 6361 6c65 5f64 6563 696d  me), scale_decim
+00002420: 616c 5f69 6e74 5f73 6967 6e65 6428 6d75  al_int_signed(mu
+00002430: 6c74 6970 6c69 6572 292c 206d 6f64 3130  ltiplier), mod10
+00002440: 6b28 7265 7665 7273 6529 2c20 6d6f 6431  k(reverse), mod1
+00002450: 306b 3634 2872 6576 6572 7365 292c 206d  0k64(reverse), m
+00002460: 6f64 3130 6b34 3828 7265 7665 7265 7329  od10k48(reveres)
+00002470: 206f 7220 6e6f 6e65 2e20 4465 6661 756c   or none. Defaul
+00002480: 7420 6973 2061 6e20 656d 7074 7920 7374  t is an empty st
+00002490: 7269 6e67 2e0a 0a20 2020 2054 6162 6c65  ring...    Table
+000024a0: 2028 4f70 7469 6f6e 616c 2920 2d20 5374   (Optional) - St
+000024b0: 616e 6461 7264 206d 6f64 6275 7320 7461  andard modbus ta
+000024c0: 626c 6520 6e61 6d65 2064 6566 696e 696e  ble name definin
+000024d0: 6720 686f 7720 696e 666f 726d 6174 696f  g how informatio
+000024e0: 6e20 6973 2073 746f 7265 6420 696e 2073  n is stored in s
+000024f0: 6c61 7665 2064 6576 6963 652e 2054 6865  lave device. The
+00002500: 7265 2061 7265 2034 2064 6966 6665 7265  re are 4 differe
+00002510: 6e74 2074 6162 6c65 733a 0a0a 2020 2020  nt tables:..    
+00002520: 6469 7363 7265 7465 5f6f 7574 7075 745f  discrete_output_
+00002530: 636f 696c 733a 2072 6561 642f 7772 6974  coils: read/writ
+00002540: 6520 636f 696c 206e 756d 6265 7273 2031  e coil numbers 1
+00002550: 2d39 3939 390a 0a20 2020 2064 6973 6372  -9999..    discr
+00002560: 6574 655f 696e 7075 745f 636f 6e74 6163  ete_input_contac
+00002570: 7473 3a20 7265 6164 206f 6e6c 7920 636f  ts: read only co
+00002580: 696c 206e 756d 6265 7273 2031 3030 3031  il numbers 10001
+00002590: 2d31 3939 3939 0a0a 2020 2020 616e 616c  -19999..    anal
+000025a0: 6f67 5f69 6e70 7574 5f72 6567 6973 7465  og_input_registe
+000025b0: 7273 3a20 7265 6164 206f 6e6c 7920 7265  rs: read only re
+000025c0: 6769 7374 6572 206e 756d 6265 7273 2033  gister numbers 3
+000025d0: 3030 3031 2d33 3939 3939 0a0a 2020 2020  0001-39999..    
+000025e0: 616e 616c 6f67 5f6f 7574 7075 745f 686f  analog_output_ho
+000025f0: 6c64 696e 675f 7265 6769 7374 6572 733a  lding_registers:
+00002600: 2072 6561 642f 7772 6974 6520 7265 6769   read/write regi
+00002610: 7374 6572 206e 756d 6265 7273 2034 3030  ster numbers 400
+00002620: 3031 2d34 3939 3939 0a0a 2020 2020 4966  01-49999..    If
+00002630: 2074 6869 7320 6669 656c 6420 6973 2065   this field is e
+00002640: 6d70 7479 2c20 7468 6520 6d6f 6462 7573  mpty, the modbus
+00002650: 2074 6162 6c65 2077 696c 6c20 6265 2064   table will be d
+00002660: 6566 696e 6564 2062 7920 7479 7065 2061  efined by type a
+00002670: 6e64 2077 7269 7461 626c 6520 6669 656c  nd writable fiel
+00002680: 6473 2e20 4279 2074 6861 742c 2077 6865  ds. By that, whe
+00002690: 6e20 7573 6572 2073 6574 7320 7265 6164  n user sets read
+000026a0: 206f 6e6c 7920 666f 7220 7265 6164 2f77   only for read/w
+000026b0: 7269 7465 2063 6f69 6c73 2f72 6567 6973  rite coils/regis
+000026c0: 7465 7273 206f 7220 7365 7473 2072 6561  ters or sets rea
+000026d0: 642f 7772 6974 6520 666f 7220 7265 6164  d/write for read
+000026e0: 206f 6e6c 7920 636f 696c 732f 7265 6769   only coils/regi
+000026f0: 7374 6572 732c 2069 7420 7769 6c6c 2073  sters, it will s
+00002700: 656c 6563 7420 7772 6f6e 6720 7461 626c  elect wrong tabl
+00002710: 652c 2061 6e64 2074 6865 7265 666f 7265  e, and therefore
+00002720: 2072 6169 7365 2065 7863 6570 7469 6f6e   raise exception
+00002730: 2e0a 0a20 2020 204d 6978 6564 2045 6e64  ...    Mixed End
+00002740: 6961 6e20 284f 7074 696f 6e61 6c29 202d  ian (Optional) -
+00002750: 2054 5255 452f 4641 4c53 452e 2049 6620   TRUE/FALSE. If 
+00002760: 4d69 7865 6420 456e 6469 616e 2069 7320  Mixed Endian is 
+00002770: 7365 7420 746f 2054 5255 452c 2074 6865  set to TRUE, the
+00002780: 206f 7264 6572 206f 6620 7468 6520 4d6f   order of the Mo
+00002790: 6462 7573 2072 6567 6973 7465 7273 2077  dbus registers w
+000027a0: 696c 6c20 6265 2072 6576 6572 7365 6420  ill be reversed 
+000027b0: 6265 666f 7265 2070 6172 7369 6e67 2074  before parsing t
+000027c0: 6865 2076 616c 7565 206f 7220 7772 6974  he value or writ
+000027d0: 696e 6720 6974 206f 7574 2074 6f20 7468  ing it out to th
+000027e0: 6520 6465 7669 6365 2e20 4279 2073 6574  e device. By set
+000027f0: 7469 6e67 206d 6978 6564 2065 6e64 6961  ting mixed endia
+00002800: 6e2c 2074 7261 6e73 666f 726d 206d 7573  n, transform mus
+00002810: 7420 6265 204e 6f6e 6520 286e 6f20 6f70  t be None (no op
+00002820: 292e 2044 6566 6175 6c74 7320 746f 2046  ). Defaults to F
+00002830: 414c 5345 2e0a 0a20 2020 2044 6573 6372  ALSE...    Descr
+00002840: 6970 7469 6f6e 2028 4f70 7469 6f6e 616c  iption (Optional
+00002850: 2920 2d20 4164 6469 7469 6f6e 616c 2069  ) - Additional i
+00002860: 6e66 6f72 6d61 7469 6f6e 2061 626f 7574  nformation about
+00002870: 2074 6865 2070 6f69 6e74 2e20 4465 6661   the point. Defa
+00002880: 756c 7420 6973 2061 6e20 656d 7074 7920  ult is an empty 
+00002890: 7374 7269 6e67 2e0a 0a20 2020 2048 6572  string...    Her
+000028a0: 6520 6973 2061 2073 616d 706c 6520 4d6f  e is a sample Mo
+000028b0: 6462 7573 2d54 4b20 7265 6769 7374 7279  dbus-TK registry
+000028c0: 206d 6170 3a0a 0a20 2020 2060 6060 6373   map:..    ```cs
+000028d0: 760a 2020 2020 5265 6769 7374 6572 204e  v.    Register N
+000028e0: 616d 652c 4164 6472 6573 732c 5479 7065  ame,Address,Type
+000028f0: 2c55 6e69 7473 2c57 7269 7461 626c 652c  ,Units,Writable,
+00002900: 4465 6661 756c 7420 5661 6c75 652c 5472  Default Value,Tr
+00002910: 616e 7366 6f72 6d2c 5461 626c 650a 2020  ansform,Table.  
+00002920: 2020 756e 7369 676e 6564 5f73 686f 7274    unsigned_short
+00002930: 2c30 2c75 696e 7431 362c 4e6f 6e65 2c54  ,0,uint16,None,T
+00002940: 5255 452c 302c 7363 616c 6528 3130 292c  RUE,0,scale(10),
+00002950: 616e 616c 6f67 5f6f 7574 7075 745f 686f  analog_output_ho
+00002960: 6c64 696e 675f 7265 6769 7374 6572 730a  lding_registers.
+00002970: 2020 2020 756e 7369 676e 6564 5f69 6e74      unsigned_int
+00002980: 2c31 2c75 696e 7433 322c 4e6f 6e65 2c54  ,1,uint32,None,T
+00002990: 5255 452c 302c 7363 616c 6528 3130 292c  RUE,0,scale(10),
+000029a0: 616e 616c 6f67 5f6f 7574 7075 745f 686f  analog_output_ho
+000029b0: 6c64 696e 675f 7265 6769 7374 6572 730a  lding_registers.
+000029c0: 2020 2020 756e 7369 676e 6564 5f6c 6f6e      unsigned_lon
+000029d0: 672c 332c 7569 6e74 3634 2c4e 6f6e 652c  g,3,uint64,None,
+000029e0: 5452 5545 2c30 2c73 6361 6c65 2831 3029  TRUE,0,scale(10)
+000029f0: 2c61 6e61 6c6f 675f 6f75 7470 7574 5f68  ,analog_output_h
+00002a00: 6f6c 6469 6e67 5f72 6567 6973 7465 7273  olding_registers
+00002a10: 0a20 2020 2073 616d 706c 655f 7368 6f72  .    sample_shor
+00002a20: 742c 372c 696e 7431 362c 4e6f 6e65 2c54  t,7,int16,None,T
+00002a30: 5255 452c 302c 7363 616c 6528 3130 292c  RUE,0,scale(10),
+00002a40: 616e 616c 6f67 5f6f 7574 7075 745f 686f  analog_output_ho
+00002a50: 6c64 696e 675f 7265 6769 7374 6572 730a  lding_registers.
+00002a60: 2020 2020 7361 6d70 6c65 5f69 6e74 2c38      sample_int,8
+00002a70: 2c69 6e74 3332 2c4e 6f6e 652c 5452 5545  ,int32,None,TRUE
+00002a80: 2c30 2c73 6361 6c65 2831 3029 2c61 6e61  ,0,scale(10),ana
+00002a90: 6c6f 675f 6f75 7470 7574 5f68 6f6c 6469  log_output_holdi
+00002aa0: 6e67 5f72 6567 6973 7465 7273 0a20 2020  ng_registers.   
+00002ab0: 2073 616d 706c 655f 666c 6f61 742c 3130   sample_float,10
+00002ac0: 2c66 6c6f 6174 2c4e 6f6e 652c 5452 5545  ,float,None,TRUE
+00002ad0: 2c30 2e30 2c73 6361 6c65 2831 3029 2c61  ,0.0,scale(10),a
+00002ae0: 6e61 6c6f 675f 6f75 7470 7574 5f68 6f6c  nalog_output_hol
+00002af0: 6469 6e67 5f72 6567 6973 7465 7273 0a20  ding_registers. 
+00002b00: 2020 2073 616d 706c 655f 6c6f 6e67 2c31     sample_long,1
+00002b10: 322c 696e 7436 342c 4e6f 6e65 2c54 5255  2,int64,None,TRU
+00002b20: 452c 302c 7363 616c 6528 3130 292c 616e  E,0,scale(10),an
+00002b30: 616c 6f67 5f6f 7574 7075 745f 686f 6c64  alog_output_hold
+00002b40: 696e 675f 7265 6769 7374 6572 730a 2020  ing_registers.  
+00002b50: 2020 7361 6d70 6c65 5f62 6f6f 6c2c 3136    sample_bool,16
+00002b60: 2c62 6f6f 6c2c 4e6f 6e65 2c54 5255 452c  ,bool,None,TRUE,
+00002b70: 4661 6c73 652c 2c61 6e61 6c6f 675f 6f75  False,,analog_ou
+00002b80: 7470 7574 5f68 6f6c 6469 6e67 5f72 6567  tput_holding_reg
+00002b90: 6973 7465 7273 0a20 2020 2073 616d 706c  isters.    sampl
+00002ba0: 655f 7374 722c 3137 2c73 7472 696e 675b  e_str,17,string[
+00002bb0: 3132 5d2c 4e6f 6e65 2c54 5255 452c 6865  12],None,TRUE,he
+00002bc0: 6c6c 6f20 776f 726c 6421 2c2c 616e 616c  llo world!,,anal
+00002bd0: 6f67 5f6f 7574 7075 745f 686f 6c64 696e  og_output_holdin
+00002be0: 675f 7265 6769 7374 6572 730a 2020 2020  g_registers.    
+00002bf0: 6060 600a 0a20 2020 2041 6674 6572 2063  ```..    After c
+00002c00: 7265 6174 696e 6720 6120 7265 6769 7374  reating a regist
+00002c10: 7279 206d 6170 206e 616d 6564 2022 6d6f  ry map named "mo
+00002c20: 6462 7573 5f74 6b5f 7465 7374 5f6d 6170  dbus_tk_test_map
+00002c30: 2e63 7376 222c 2061 6464 2069 7420 746f  .csv", add it to
+00002c40: 2074 6865 2043 6f6e 6669 6775 7261 7469   the Configurati
+00002c50: 6f6e 2053 746f 7265 3a0a 0a20 2020 2060  on Store:..    `
+00002c60: 6060 7368 656c 6c0a 2020 2020 7663 746c  ``shell.    vctl
+00002c70: 2063 6f6e 6669 6720 7374 6f72 6520 706c   config store pl
+00002c80: 6174 666f 726d 2e64 7269 7665 7220 6d6f  atform.driver mo
+00002c90: 6462 7573 5f74 6b5f 7465 7374 5f6d 6170  dbus_tk_test_map
+00002ca0: 2e63 7376 206d 6f64 6275 735f 746b 5f74  .csv modbus_tk_t
+00002cb0: 6573 745f 6d61 702e 6373 7620 2d2d 6373  est_map.csv --cs
+00002cc0: 760a 2020 2020 6060 600a 0a31 2e20 4164  v.    ```..1. Ad
+00002cd0: 6420 6120 7265 6769 7374 7279 2063 6f6e  d a registry con
+00002ce0: 6669 6775 7261 7469 6f6e 2074 6f20 7468  figuration to th
+00002cf0: 6520 506c 6174 666f 726d 4472 6976 6572  e PlatformDriver
+00002d00: 2e0a 0a20 2020 2054 6865 2072 6567 6973  ...    The regis
+00002d10: 7472 7920 636f 6e66 6967 7572 6174 696f  try configuratio
+00002d20: 6e20 6669 6c65 2069 7320 6120 4353 5620  n file is a CSV 
+00002d30: 6669 6c65 2e20 4561 6368 2072 6f77 2063  file. Each row c
+00002d40: 6f6e 6669 6775 7265 7320 6120 706f 696e  onfigures a poin
+00002d50: 7420 6f6e 2074 6865 2064 6576 6963 652e  t on the device.
+00002d60: 0a0a 2020 2020 2020 2020 566f 6c74 7472  ..        Volttr
+00002d70: 6f6e 2050 6f69 6e74 204e 616d 6520 2852  on Point Name (R
+00002d80: 6571 7569 7265 6429 202d 2054 6865 206e  equired) - The n
+00002d90: 616d 6520 6279 2077 6869 6368 2074 6865  ame by which the
+00002da0: 2070 6c61 7466 6f72 6d20 616e 6420 6167   platform and ag
+00002db0: 656e 7473 2072 6566 6572 2074 6f20 7468  ents refer to th
+00002dc0: 6520 706f 696e 742e 2046 6f72 2069 6e73  e point. For ins
+00002dd0: 7461 6e63 652c 2069 6620 7468 6520 566f  tance, if the Vo
+00002de0: 6c74 7472 6f6e 2050 6f69 6e74 204e 616d  lttron Point Nam
+00002df0: 6520 6973 2048 6561 7443 616c 6c31 2c20  e is HeatCall1, 
+00002e00: 7468 656e 2061 6e20 6167 656e 7420 776f  then an agent wo
+00002e10: 756c 6420 7573 6520 6d79 5f63 616d 7075  uld use my_campu
+00002e20: 732f 6275 696c 6469 6e67 322f 6876 6163  s/building2/hvac
+00002e30: 312f 4865 6174 4361 6c6c 3120 746f 2072  1/HeatCall1 to r
+00002e40: 6566 6572 2074 6f20 7468 6520 706f 696e  efer to the poin
+00002e50: 7420 7768 656e 2075 7369 6e67 2074 6865  t when using the
+00002e60: 2052 5043 2069 6e74 6572 6661 6365 206f   RPC interface o
+00002e70: 6620 7468 6520 6163 7475 6174 6f72 2061  f the actuator a
+00002e80: 6765 6e74 2e0a 0a20 2020 2020 2020 2052  gent...        R
+00002e90: 6567 6973 7465 7220 4e61 6d65 2028 5265  egister Name (Re
+00002ea0: 7175 6972 6564 2920 2d20 5468 6520 6669  quired) - The fi
+00002eb0: 656c 6420 6e61 6d65 2069 6e20 7468 6520  eld name in the 
+00002ec0: 6d6f 6462 7573 2063 6c69 656e 742e 2049  modbus client. I
+00002ed0: 7420 6d75 7374 2062 6520 6d61 7463 6865  t must be matche
+00002ee0: 6420 7769 7468 2074 6865 2066 6965 6c64  d with the field
+00002ef0: 206e 616d 6520 6672 6f6d 2072 6567 6973   name from regis
+00002f00: 7465 725f 6d61 702e 0a0a 2020 2020 416e  ter_map...    An
+00002f10: 7920 6164 6469 7469 6f6e 616c 2063 6f6c  y additional col
+00002f20: 756d 6e73 2077 696c 6c20 6f76 6572 7269  umns will overri
+00002f30: 6465 2074 6865 2065 7869 7374 6564 2066  de the existed f
+00002f40: 6965 6c64 7320 6672 6f6d 2072 6567 6973  ields from regis
+00002f50: 7465 725f 6d61 702e 0a0a 2020 2020 4865  ter_map...    He
+00002f60: 7265 2069 7320 6120 7361 6d70 6c65 204d  re is a sample M
+00002f70: 6f64 6275 732d 544b 2072 6567 6973 7472  odbus-TK registr
+00002f80: 7920 636f 6e66 6967 7572 6174 696f 6e20  y configuration 
+00002f90: 7769 7468 2064 6566 696e 6564 2072 6567  with defined reg
+00002fa0: 6973 7465 725f 6d61 703a 0a0a 2020 2020  ister_map:..    
+00002fb0: 6060 6063 7376 0a20 2020 2056 6f6c 7474  ```csv.    Voltt
+00002fc0: 726f 6e20 506f 696e 7420 4e61 6d65 2c52  ron Point Name,R
+00002fd0: 6567 6973 7465 7220 4e61 6d65 0a20 2020  egister Name.   
+00002fe0: 2075 6e73 6967 6e65 6420 7368 6f72 742c   unsigned short,
+00002ff0: 756e 7369 676e 6564 5f73 686f 7274 0a20  unsigned_short. 
+00003000: 2020 2075 6e73 6967 6e65 6420 696e 742c     unsigned int,
+00003010: 756e 7369 676e 6564 5f69 6e74 0a20 2020  unsigned_int.   
+00003020: 2075 6e73 6967 6e65 6420 6c6f 6e67 2c75   unsigned long,u
+00003030: 6e73 6967 6e65 645f 6c6f 6e67 0a20 2020  nsigned_long.   
+00003040: 2073 616d 706c 6520 7368 6f72 742c 7361   sample short,sa
+00003050: 6d70 6c65 5f73 686f 7274 0a20 2020 2073  mple_short.    s
+00003060: 616d 706c 6520 696e 742c 7361 6d70 6c65  ample int,sample
+00003070: 5f69 6e74 0a20 2020 2073 616d 706c 6520  _int.    sample 
+00003080: 666c 6f61 742c 7361 6d70 6c65 5f66 6c6f  float,sample_flo
+00003090: 6174 0a20 2020 2073 616d 706c 6520 6c6f  at.    sample lo
+000030a0: 6e67 2c73 616d 706c 655f 6c6f 6e67 0a20  ng,sample_long. 
+000030b0: 2020 2073 616d 706c 6520 626f 6f6c 2c73     sample bool,s
+000030c0: 616d 706c 655f 626f 6f6c 0a20 2020 2073  ample_bool.    s
+000030d0: 616d 706c 6520 7374 722c 7361 6d70 6c65  ample str,sample
+000030e0: 5f73 7472 0a20 2020 2060 6060 0a0a 2020  _str.    ```..  
+000030f0: 2020 4166 7465 7220 6372 6561 7469 6e67    After creating
+00003100: 2061 2072 6567 6973 7472 7920 6d61 7020   a registry map 
+00003110: 6e61 6d65 6420 226d 6f64 6275 735f 746b  named "modbus_tk
+00003120: 5f74 6573 742e 6373 7622 2c20 6164 6420  _test.csv", add 
+00003130: 6974 2074 6f20 7468 6520 436f 6e66 6967  it to the Config
+00003140: 7572 6174 696f 6e20 5374 6f72 653a 0a0a  uration Store:..
+00003150: 2020 2020 6060 6073 6865 6c6c 0a20 2020      ```shell.   
+00003160: 2076 6374 6c20 636f 6e66 6967 2073 746f   vctl config sto
+00003170: 7265 2070 6c61 7466 6f72 6d2e 6472 6976  re platform.driv
+00003180: 6572 206d 6f64 6275 735f 746b 5f74 6573  er modbus_tk_tes
+00003190: 742e 6373 7620 6d6f 6462 7573 5f74 6b5f  t.csv modbus_tk_
+000031a0: 7465 7374 2e63 7376 202d 2d63 7376 0a20  test.csv --csv. 
+000031b0: 2020 2060 6060 0a0a 312e 204f 6273 6572     ```..1. Obser
+000031c0: 7665 2044 6174 610a 0a20 2020 2054 6f20  ve Data..    To 
+000031d0: 7365 6520 6461 7461 2062 6569 6e67 2070  see data being p
+000031e0: 7562 6c69 7368 6564 2074 6f20 7468 6520  ublished to the 
+000031f0: 6275 732c 2069 6e73 7461 6c6c 2061 205b  bus, install a [
+00003200: 4c69 7374 656e 6572 2041 6765 6e74 5d28  Listener Agent](
+00003210: 6874 7470 733a 2f2f 7079 7069 2e6f 7267  https://pypi.org
+00003220: 2f70 726f 6a65 6374 2f76 6f6c 7474 726f  /project/volttro
+00003230: 6e2d 6c69 7374 656e 6572 2f29 3a0a 0a20  n-listener/):.. 
+00003240: 2020 2060 6060 0a20 2020 2076 6374 6c20     ```.    vctl 
+00003250: 696e 7374 616c 6c20 766f 6c74 7472 6f6e  install volttron
+00003260: 2d6c 6973 7465 6e65 7220 2d2d 7374 6172  -listener --star
+00003270: 740a 2020 2020 6060 600a 0a20 2020 204f  t.    ```..    O
+00003280: 6e63 6520 696e 7374 616c 6c65 642c 2079  nce installed, y
+00003290: 6f75 2073 686f 756c 6420 7365 6520 7468  ou should see th
+000032a0: 6520 6461 7461 2062 6569 6e67 2070 7562  e data being pub
+000032b0: 6c69 7368 6564 2062 7920 7669 6577 696e  lished by viewin
+000032c0: 6720 7468 6520 566f 6c74 7472 6f6e 206c  g the Volttron l
+000032d0: 6f67 7320 6669 6c65 2074 6861 7420 7761  ogs file that wa
+000032e0: 7320 6372 6561 7465 6420 696e 2073 7465  s created in ste
+000032f0: 7020 322e 0a20 2020 2054 6f20 7761 7463  p 2..    To watc
+00003300: 6820 7468 6520 6c6f 6773 2c20 6f70 656e  h the logs, open
+00003310: 2061 2073 6570 6172 6174 6520 7465 726d   a separate term
+00003320: 696e 616c 2061 6e64 2072 756e 2074 6865  inal and run the
+00003330: 2066 6f6c 6c6f 7769 6e67 2063 6f6d 6d61   following comma
+00003340: 6e64 3a0a 0a20 2020 2060 6060 0a20 2020  nd:..    ```.   
+00003350: 2074 6169 6c20 2d66 203c 7061 7468 2074   tail -f <path t
+00003360: 6f20 666f 6c64 6572 2063 6f6e 7461 696e  o folder contain
+00003370: 696e 6720 766f 6c74 7472 6f6e 2e6c 6f67  ing volttron.log
+00003380: 3e2f 766f 6c74 7472 6f6e 2e6c 6f67 0a20  >/volttron.log. 
+00003390: 2020 2060 6060 0a0a 2320 4d6f 6462 7573     ```..# Modbus
+000033a0: 2d54 4b20 436f 6e66 6967 2043 6f6d 6d61  -TK Config Comma
+000033b0: 6e64 2054 6f6f 6c0a 0a60 636f 6e66 6967  nd Tool..`config
+000033c0: 5f63 6d64 2e70 7960 2069 7320 6120 636f  _cmd.py` is a co
+000033d0: 6d6d 616e 642d 6c69 6e65 2074 6f6f 6c20  mmand-line tool 
+000033e0: 666f 7220 6372 6561 7469 6e67 2061 6e64  for creating and
+000033f0: 206d 6169 6e74 6169 6e69 6e67 2056 4f4c   maintaining VOL
+00003400: 5454 524f 4e20 6472 6976 6572 2063 6f6e  TTRON driver con
+00003410: 6669 6775 7261 7469 6f6e 732e 2054 6865  figurations. The
+00003420: 2074 6f6f 6c20 7275 6e73 2066 726f 6d20   tool runs from 
+00003430: 7468 6520 636f 6d6d 616e 6420 6c69 6e65  the command line
+00003440: 3a0a 0a63 6f6e 6669 675f 636d 642e 7079  :..config_cmd.py
+00003450: 2073 7570 706f 7274 7320 7468 6520 666f   supports the fo
+00003460: 6c6c 6f77 696e 6720 636f 6d6d 616e 6473  llowing commands
+00003470: 3a0a 0a2a 2068 656c 7020 2d20 4c69 7374  :..* help - List
+00003480: 2061 6c6c 2063 6f6d 6d61 6e64 732e 0a0a   all commands...
+00003490: 2a20 7175 6974 202d 2051 7569 7420 7468  * quit - Quit th
+000034a0: 6520 636f 6d6d 616e 642d 6c69 6e65 2074  e command-line t
+000034b0: 6f6f 6c2e 0a0a 2a20 6c69 7374 5f64 6972  ool...* list_dir
+000034c0: 6563 746f 7269 6573 202d 204c 6973 7420  ectories - List 
+000034d0: 616c 6c20 7365 7475 7020 6469 7265 6374  all setup direct
+000034e0: 6f72 6965 732c 2077 6974 6820 616e 206f  ories, with an o
+000034f0: 7074 696f 6e20 746f 2065 6469 7420 7468  ption to edit th
+00003500: 6569 7220 7061 7468 732e 0a0a 0a42 7920  eir paths....By 
+00003510: 6465 6661 756c 742c 2061 6c6c 2064 6972  default, all dir
+00003520: 6563 746f 7269 6573 2061 7265 2069 6e20  ectories are in 
+00003530: 7468 6973 2072 6570 6f20 6174 2074 6865  this repo at the
+00003540: 2066 6f6c 6c6f 7769 6e67 2066 6f6c 6465   following folde
+00003550: 723a 2076 6f6c 7474 726f 6e2f 6472 6976  r: volttron/driv
+00003560: 6572 2f69 6e74 6572 6661 6365 732f 6d6f  er/interfaces/mo
+00003570: 6462 7573 5f74 6b2f 7574 696c 732f 6d61  dbus_tk/utils/ma
+00003580: 7073 2e0a 0a49 7420 6973 2069 6d70 6f72  ps...It is impor
+00003590: 7461 6e74 2074 6f20 7573 6520 7468 6520  tant to use the 
+000035a0: 636f 7272 6563 7420 6469 7265 6374 6f72  correct director
+000035b0: 6965 7320 7768 656e 2061 6464 696e 672f  ies when adding/
+000035c0: 6564 6974 696e 6720 6465 7669 6365 2074  editing device t
+000035d0: 7970 6573 2061 6e64 2064 7269 7665 7220  ypes and driver 
+000035e0: 636f 6e66 6967 732c 2061 6e64 2077 6865  configs, and whe
+000035f0: 6e20 6c6f 6164 696e 6720 636f 6e66 6967  n loading config
+00003600: 7572 6174 696f 6e73 2069 6e74 6f20 564f  urations into VO
+00003610: 4c54 5452 4f4e 2e0a 0a2a 206d 6170 5f64  LTTRON...* map_d
+00003620: 6972 3a20 6469 7265 6374 6f72 7920 696e  ir: directory in
+00003630: 2077 6869 6368 206d 6170 732e 7961 6d6c   which maps.yaml
+00003640: 2069 7320 7374 6f72 6564 2e0a 0a2a 2063   is stored...* c
+00003650: 6f6e 6669 675f 6469 723a 2064 6972 6563  onfig_dir: direc
+00003660: 746f 7279 2069 6e20 7768 6963 6820 6472  tory in which dr
+00003670: 6976 6572 2063 6f6e 6669 6720 6669 6c65  iver config file
+00003680: 7320 6172 6520 7374 6f72 6564 2e0a 0a2a  s are stored...*
+00003690: 2063 7376 5f64 6972 3a20 6469 7265 6374   csv_dir: direct
+000036a0: 6f72 7920 696e 2077 6869 6368 2072 6567  ory in which reg
+000036b0: 6973 7472 7920 636f 6e66 6967 2043 5356  istry config CSV
+000036c0: 2066 696c 6573 2061 7265 2073 746f 7265   files are store
+000036d0: 642e 0a0a 2a20 6564 6974 5f64 6972 6563  d...* edit_direc
+000036e0: 746f 7269 6573 202d 2041 6464 2f45 6469  tories - Add/Edi
+000036f0: 7420 6d61 7020 6469 7265 6374 6f72 792c  t map directory,
+00003700: 2064 7269 7665 7220 636f 6e66 6967 2064   driver config d
+00003710: 6972 6563 746f 7279 2c20 616e 642f 6f72  irectory, and/or
+00003720: 2043 5356 2063 6f6e 6669 6720 6469 7265   CSV config dire
+00003730: 6374 6f72 792e 2050 7265 7373 203c 456e  ctory. Press <En
+00003740: 7465 723e 2069 6620 6e6f 2063 6861 6e67  ter> if no chang
+00003750: 6520 6973 206e 6565 6465 642e 2045 7869  e is needed. Exi
+00003760: 7473 2069 6620 7468 6520 6469 7265 6374  ts if the direct
+00003770: 6f72 7920 646f 6573 206e 6f74 2065 7869  ory does not exi
+00003780: 7374 2e0a 0a2a 206c 6973 745f 6465 7669  st...* list_devi
+00003790: 6365 5f74 7970 655f 6465 7363 7269 7074  ce_type_descript
+000037a0: 696f 6e20 2d20 4c69 7374 2061 6c6c 2064  ion - List all d
+000037b0: 6576 6963 6520 7479 7065 2064 6573 6372  evice type descr
+000037c0: 6970 7469 6f6e 7320 696e 206d 6170 732e  iptions in maps.
+000037d0: 7961 6d6c 2e20 4f70 7469 6f6e 2074 6f20  yaml. Option to 
+000037e0: 6564 6974 2064 6576 6963 6520 7479 7065  edit device type
+000037f0: 2064 6573 6372 6970 7469 6f6e 732e 0a0a   descriptions...
+00003800: 2a20 6c69 7374 5f61 6c6c 5f64 6576 6963  * list_all_devic
+00003810: 655f 7479 7065 7320 2d20 4c69 7374 2061  e_types - List a
+00003820: 6c6c 2064 6576 6963 6520 7479 7065 2069  ll device type i
+00003830: 6e66 6f72 6d61 7469 6f6e 2069 6e20 6d61  nformation in ma
+00003840: 7073 2e79 616d 6c2e 204f 7074 696f 6e20  ps.yaml. Option 
+00003850: 746f 2061 6464 206d 6f72 6520 6465 7669  to add more devi
+00003860: 6365 2074 7970 6573 2e0a 0a2a 2064 6576  ce types...* dev
+00003870: 6963 655f 7479 7065 202d 204c 6973 7420  ice_type - List 
+00003880: 696e 666f 726d 6174 696f 6e20 666f 7220  information for 
+00003890: 6120 7365 6c65 6374 6564 2064 6576 6963  a selected devic
+000038a0: 6520 7479 7065 2e20 4f70 7469 6f6e 2074  e type. Option t
+000038b0: 6f20 7365 6c65 6374 2061 6e6f 7468 6572  o select another
+000038c0: 2064 6576 6963 6520 7479 7065 2e0a 0a2a   device type...*
+000038d0: 2061 6464 5f64 6576 6963 655f 7479 7065   add_device_type
+000038e0: 202d 2041 6464 2061 2064 6576 6963 6520   - Add a device 
+000038f0: 7479 7065 2074 6f20 6d61 7073 2e79 616d  type to maps.yam
+00003900: 6c2e 204f 7074 696f 6e20 746f 2061 6464  l. Option to add
+00003910: 206d 6f72 6520 7468 616e 206f 6e65 2064   more than one d
+00003920: 6576 6963 6520 7479 7065 2e20 4561 6368  evice type. Each
+00003930: 2064 6576 6963 6520 7479 7065 2069 6e63   device type inc
+00003940: 6c75 6465 7320 6974 7320 6e61 6d65 2c20  ludes its name, 
+00003950: 4353 5620 6669 6c65 2c20 6465 7363 7269  CSV file, descri
+00003960: 7074 696f 6e2c 2061 6464 7265 7373 696e  ption, addressin
+00003970: 672c 2061 6e64 2065 6e64 6961 6e2c 2061  g, and endian, a
+00003980: 7320 6578 706c 6169 6e65 6420 696e 204d  s explained in M
+00003990: 4f44 4255 532d 544b 2044 7269 7665 7220  ODBUS-TK Driver 
+000039a0: 4d61 7073 2e20 4966 2061 6e20 696e 7661  Maps. If an inva
+000039b0: 6c69 6420 7661 6c75 6520 6973 2065 6e74  lid value is ent
+000039c0: 6572 6564 2066 6f72 2061 6464 7265 7373  ered for address
+000039d0: 696e 6720 6f72 2065 6e64 6961 6e2c 2074  ing or endian, t
+000039e0: 6865 2064 6566 6175 6c74 2076 616c 7565  he default value
+000039f0: 2069 7320 7573 6564 2069 6e73 7465 6164   is used instead
+00003a00: 2e0a 0a2a 6564 6974 5f64 6576 6963 655f  ...*edit_device_
+00003a10: 7479 7065 202d 2045 6469 7420 616e 2065  type - Edit an e
+00003a20: 7869 7374 696e 6720 6465 7669 6365 2074  xisting device t
+00003a30: 7970 652e 2049 6620 616e 2069 6e76 616c  ype. If an inval
+00003a40: 6964 2076 616c 7565 2069 7320 656e 7465  id value is ente
+00003a50: 7265 6420 666f 7220 6164 6472 6573 7369  red for addressi
+00003a60: 6e67 206f 7220 656e 6469 616e 2c20 7468  ng or endian, th
+00003a70: 6520 7072 6576 696f 7573 2076 616c 7565  e previous value
+00003a80: 2069 7320 6c65 6674 2075 6e63 6861 6e67   is left unchang
+00003a90: 6564 2e0a 0a2a 206c 6973 745f 6472 6976  ed...* list_driv
+00003aa0: 6572 7320 2d20 4c69 7374 2061 6c6c 2064  ers - List all d
+00003ab0: 7269 7665 7220 636f 6e66 6967 206e 616d  river config nam
+00003ac0: 6573 2069 6e20 636f 6e66 6967 5f64 6972  es in config_dir
+00003ad0: 2e0a 0a2a 2064 7269 7665 725f 636f 6e66  ...* driver_conf
+00003ae0: 6967 203c 6472 6976 6572 5f6e 616d 653e  ig <driver_name>
+00003af0: 202d 2047 6574 2061 2064 7269 7665 7220   - Get a driver 
+00003b00: 636f 6e66 6967 2066 726f 6d20 636f 6e66  config from conf
+00003b10: 6967 5f64 6972 2e20 4f70 7469 6f6e 2074  ig_dir. Option t
+00003b20: 6f20 7365 6c65 6374 2074 6865 2064 7269  o select the dri
+00003b30: 7665 7220 6966 206e 6f20 6472 6976 6572  ver if no driver
+00003b40: 2069 7320 666f 756e 6420 7769 7468 2074   is found with t
+00003b50: 6861 7420 6e61 6d65 2e0a 0a2a 2061 6464  hat name...* add
+00003b60: 5f64 7269 7665 725f 636f 6e66 6967 203c  _driver_config <
+00003b70: 6472 6976 6572 5f6e 616d 653e 202d 2041  driver_name> - A
+00003b80: 6464 2f45 6469 7420 3c63 6f6e 6669 675f  dd/Edit <config_
+00003b90: 6469 723e 2f3c 6472 6976 6572 206e 616d  dir>/<driver nam
+00003ba0: 653e 2e63 6f6e 6669 672e 204f 7074 696f  e>.config. Optio
+00003bb0: 6e20 746f 2073 656c 6563 7420 7468 6520  n to select the 
+00003bc0: 6472 6976 6572 2069 6620 6e6f 2064 7269  driver if no dri
+00003bd0: 7665 7220 6973 2066 6f75 6e64 2077 6974  ver is found wit
+00003be0: 6820 7468 6174 206e 616d 652e 2050 7265  h that name. Pre
+00003bf0: 7373 203c 456e 7465 723e 2074 6f20 6578  ss <Enter> to ex
+00003c00: 6974 2e0a 0a2a 206c 6f61 645f 766f 6c74  it...* load_volt
+00003c10: 7472 6f6e 202d 204c 6f61 6420 6120 6472  tron - Load a dr
+00003c20: 6976 6572 2063 6f6e 6669 6720 616e 6420  iver config and 
+00003c30: 4353 5620 696e 746f 2056 4f4c 5454 524f  CSV into VOLTTRO
+00003c40: 4e2e 204f 7074 696f 6e20 746f 2061 6464  N. Option to add
+00003c50: 2074 6865 2063 6f6e 6669 6720 6f72 2043   the config or C
+00003c60: 5356 2066 696c 6520 746f 2063 6f6e 6669  SV file to confi
+00003c70: 675f 6469 7220 6f72 2074 6f20 6373 765f  g_dir or to csv_
+00003c80: 6469 722e 2056 4f4c 5454 524f 4e20 6d75  dir. VOLTTRON mu
+00003c90: 7374 2062 6520 7275 6e6e 696e 6720 7768  st be running wh
+00003ca0: 656e 2074 6869 7320 636f 6d6d 616e 6420  en this command 
+00003cb0: 6973 2075 7365 642e 0a0a 2a20 6465 6c65  is used...* dele
+00003cc0: 7465 5f76 6f6c 7474 726f 6e5f 636f 6e66  te_volttron_conf
+00003cd0: 6967 202d 2044 656c 6574 6520 6120 6472  ig - Delete a dr
+00003ce0: 6976 6572 2063 6f6e 6669 6720 6672 6f6d  iver config from
+00003cf0: 2056 4f4c 5454 524f 4e2e 2056 4f4c 5454   VOLTTRON. VOLTT
+00003d00: 524f 4e20 6d75 7374 2062 6520 7275 6e6e  RON must be runn
+00003d10: 696e 6720 7768 656e 2074 6869 7320 636f  ing when this co
+00003d20: 6d6d 616e 6420 6973 2075 7365 642e 0a0a  mmand is used...
+00003d30: 2a20 6465 6c65 7465 5f76 6f6c 7474 726f  * delete_volttro
+00003d40: 6e5f 6373 7620 2d20 4465 6c65 7465 2061  n_csv - Delete a
+00003d50: 2072 6567 6973 7472 7920 6373 7620 636f   registry csv co
+00003d60: 6e66 6967 2066 726f 6d20 564f 4c54 5452  nfig from VOLTTR
+00003d70: 4f4e 2e20 564f 4c54 5452 4f4e 206d 7573  ON. VOLTTRON mus
+00003d80: 7420 6265 2072 756e 6e69 6e67 2077 6865  t be running whe
+00003d90: 6e20 7468 6973 2063 6f6d 6d61 6e64 2069  n this command i
+00003da0: 7320 7573 6564 2e0a 0a23 2044 6576 656c  s used...# Devel
+00003db0: 6f70 6d65 6e74 0a0a 506c 6561 7365 2073  opment..Please s
+00003dc0: 6565 2074 6865 2066 6f6c 6c6f 7769 6e67  ee the following
+00003dd0: 2066 6f72 2063 6f6e 7472 6962 7574 696e   for contributin
+00003de0: 6720 6775 6964 656c 696e 6573 205b 636f  g guidelines [co
+00003df0: 6e74 7269 6275 7469 6e67 5d28 6874 7470  ntributing](http
+00003e00: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f65  s://github.com/e
+00003e10: 636c 6970 7365 2d76 6f6c 7474 726f 6e2f  clipse-volttron/
+00003e20: 766f 6c74 7472 6f6e 2d63 6f72 652f 626c  volttron-core/bl
+00003e30: 6f62 2f64 6576 656c 6f70 2f43 4f4e 5452  ob/develop/CONTR
+00003e40: 4942 5554 494e 472e 6d64 292e 0a0a 506c  IBUTING.md)...Pl
+00003e50: 6561 7365 2073 6565 2074 6865 2066 6f6c  ease see the fol
+00003e60: 6c6f 7769 6e67 2068 656c 7066 756c 2067  lowing helpful g
+00003e70: 7569 6465 2061 626f 7574 205b 6465 7665  uide about [deve
+00003e80: 6c6f 7069 6e67 206d 6f64 756c 6172 2056  loping modular V
+00003e90: 4f4c 5454 524f 4e20 6167 656e 7473 5d28  OLTTRON agents](
+00003ea0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+00003eb0: 6f6d 2f65 636c 6970 7365 2d76 6f6c 7474  om/eclipse-voltt
+00003ec0: 726f 6e2f 766f 6c74 7472 6f6e 2d63 6f72  ron/volttron-cor
+00003ed0: 652f 626c 6f62 2f64 6576 656c 6f70 2f44  e/blob/develop/D
+00003ee0: 4556 454c 4f50 494e 475f 4f4e 5f4d 4f44  EVELOPING_ON_MOD
+00003ef0: 554c 4152 2e6d 6429 0a0a 0a23 2044 6973  ULAR.md)...# Dis
+00003f00: 636c 6169 6d65 7220 4e6f 7469 6365 0a0a  claimer Notice..
+00003f10: 5468 6973 206d 6174 6572 6961 6c20 7761  This material wa
+00003f20: 7320 7072 6570 6172 6564 2061 7320 616e  s prepared as an
+00003f30: 2061 6363 6f75 6e74 206f 6620 776f 726b   account of work
+00003f40: 2073 706f 6e73 6f72 6564 2062 7920 616e   sponsored by an
+00003f50: 2061 6765 6e63 7920 6f66 2074 6865 0a55   agency of the.U
+00003f60: 6e69 7465 6420 5374 6174 6573 2047 6f76  nited States Gov
+00003f70: 6572 6e6d 656e 742e 2020 4e65 6974 6865  ernment.  Neithe
+00003f80: 7220 7468 6520 556e 6974 6564 2053 7461  r the United Sta
+00003f90: 7465 7320 476f 7665 726e 6d65 6e74 206e  tes Government n
+00003fa0: 6f72 2074 6865 2055 6e69 7465 640a 5374  or the United.St
+00003fb0: 6174 6573 2044 6570 6172 746d 656e 7420  ates Department 
+00003fc0: 6f66 2045 6e65 7267 792c 206e 6f72 2042  of Energy, nor B
+00003fd0: 6174 7465 6c6c 652c 206e 6f72 2061 6e79  attelle, nor any
+00003fe0: 206f 6620 7468 6569 7220 656d 706c 6f79   of their employ
+00003ff0: 6565 732c 206e 6f72 2061 6e79 0a6a 7572  ees, nor any.jur
+00004000: 6973 6469 6374 696f 6e20 6f72 206f 7267  isdiction or org
+00004010: 616e 697a 6174 696f 6e20 7468 6174 2068  anization that h
+00004020: 6173 2063 6f6f 7065 7261 7465 6420 696e  as cooperated in
+00004030: 2074 6865 2064 6576 656c 6f70 6d65 6e74   the development
+00004040: 206f 6620 7468 6573 650a 6d61 7465 7269   of these.materi
+00004050: 616c 732c 206d 616b 6573 2061 6e79 2077  als, makes any w
+00004060: 6172 7261 6e74 792c 2065 7870 7265 7373  arranty, express
+00004070: 206f 7220 696d 706c 6965 642c 206f 7220   or implied, or 
+00004080: 6173 7375 6d65 7320 616e 7920 6c65 6761  assumes any lega
+00004090: 6c0a 6c69 6162 696c 6974 7920 6f72 2072  l.liability or r
+000040a0: 6573 706f 6e73 6962 696c 6974 7920 666f  esponsibility fo
+000040b0: 7220 7468 6520 6163 6375 7261 6379 2c20  r the accuracy, 
+000040c0: 636f 6d70 6c65 7465 6e65 7373 2c20 6f72  completeness, or
+000040d0: 2075 7365 6675 6c6e 6573 7320 6f72 2061   usefulness or a
+000040e0: 6e79 0a69 6e66 6f72 6d61 7469 6f6e 2c20  ny.information, 
+000040f0: 6170 7061 7261 7475 732c 2070 726f 6475  apparatus, produ
+00004100: 6374 2c20 736f 6674 7761 7265 2c20 6f72  ct, software, or
+00004110: 2070 726f 6365 7373 2064 6973 636c 6f73   process disclos
+00004120: 6564 2c20 6f72 2072 6570 7265 7365 6e74  ed, or represent
+00004130: 730a 7468 6174 2069 7473 2075 7365 2077  s.that its use w
+00004140: 6f75 6c64 206e 6f74 2069 6e66 7269 6e67  ould not infring
+00004150: 6520 7072 6976 6174 656c 7920 6f77 6e65  e privately owne
+00004160: 6420 7269 6768 7473 2e0a 0a52 6566 6572  d rights...Refer
+00004170: 656e 6365 2068 6572 6569 6e20 746f 2061  ence herein to a
+00004180: 6e79 2073 7065 6369 6669 6320 636f 6d6d  ny specific comm
+00004190: 6572 6369 616c 2070 726f 6475 6374 2c20  ercial product, 
+000041a0: 7072 6f63 6573 732c 206f 7220 7365 7276  process, or serv
+000041b0: 6963 6520 6279 0a74 7261 6465 206e 616d  ice by.trade nam
+000041c0: 652c 2074 7261 6465 6d61 726b 2c20 6d61  e, trademark, ma
+000041d0: 6e75 6661 6374 7572 6572 2c20 6f72 206f  nufacturer, or o
+000041e0: 7468 6572 7769 7365 2064 6f65 7320 6e6f  therwise does no
+000041f0: 7420 6e65 6365 7373 6172 696c 790a 636f  t necessarily.co
+00004200: 6e73 7469 7475 7465 206f 7220 696d 706c  nstitute or impl
+00004210: 7920 6974 7320 656e 646f 7273 656d 656e  y its endorsemen
+00004220: 742c 2072 6563 6f6d 6d65 6e64 6174 696f  t, recommendatio
+00004230: 6e2c 206f 7220 6661 766f 7269 6e67 2062  n, or favoring b
+00004240: 7920 7468 6520 556e 6974 6564 0a53 7461  y the United.Sta
+00004250: 7465 7320 476f 7665 726e 6d65 6e74 206f  tes Government o
+00004260: 7220 616e 7920 6167 656e 6379 2074 6865  r any agency the
+00004270: 7265 6f66 2c20 6f72 2042 6174 7465 6c6c  reof, or Battell
+00004280: 6520 4d65 6d6f 7269 616c 2049 6e73 7469  e Memorial Insti
+00004290: 7475 7465 2e20 5468 650a 7669 6577 7320  tute. The.views 
+000042a0: 616e 6420 6f70 696e 696f 6e73 206f 6620  and opinions of 
+000042b0: 6175 7468 6f72 7320 6578 7072 6573 7365  authors expresse
+000042c0: 6420 6865 7265 696e 2064 6f20 6e6f 7420  d herein do not 
+000042d0: 6e65 6365 7373 6172 696c 7920 7374 6174  necessarily stat
+000042e0: 6520 6f72 0a72 6566 6c65 6374 2074 686f  e or.reflect tho
+000042f0: 7365 206f 6620 7468 6520 556e 6974 6564  se of the United
+00004300: 2053 7461 7465 7320 476f 7665 726e 6d65   States Governme
+00004310: 6e74 206f 7220 616e 7920 6167 656e 6379  nt or any agency
+00004320: 2074 6865 7265 6f66 2e0a                  thereof..
```

### Comparing `volttron_lib_modbustk_driver-0.1.1a1/pyproject.toml` & `volttron_lib_modbustk_driver-0.1.2rc0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.mypy]
+python_version = 3.10
 show_error_context = true
 pretty = true
 show_column_numbers = true
-show_error_codes = true
-exclude = ['docs/']
+warn_return_any = true
+warn_unused_configs = true
 
-[tool.mypy-six.moves]
+[[tool.mypy.overrides]]
+module = [
+    "yaml",
+    "six"
+]
 ignore_missing_imports = true
 
 [tool.poetry]
 name = "volttron-lib-modbustk-driver"
-version = "0.1.1a1"
+version = "0.1.2rc0"
 description = "ModbusTK Driver supported and maintained by the Volttron team."
 authors = ["Mark Bonicillo <volttron@pnnl.gov>"]
 license = "Apache License 2.0"
 readme = "README.md"
 repository = "https://github.com/VOLTTRON/volttron-lib-modbustk-driver"
 homepage = "https://github.com/VOLTTRON/volttron-drivers/volttron-lib-modbustk-driver"
 keywords = []
@@ -29,19 +34,19 @@
     "Intended Audience :: Information Technology",
     "Intended Audience :: Developers",
     "Intended Audience :: Other Audience",
     "License :: OSI Approved :: Apache Software License"
 ]
 
 [tool.poetry.dependencies]
-python = ">=3.8,<4.0"
-volttron-lib-base-driver="^0.2.0rc0"
-modbus-tk = "^1.1.2"
+python = "^3.10"
+modbus-tk = "^1.1.3"
 pyserial = "^3.5"
 PyYAML = "^6.0"
+volttron-lib-base-driver = "^0.2.1rc2"
 
 [tool.poetry.group.dev.dependencies]
 volttron-testing = "^0.3.1a9"
 pytest = "^6.2.5"
 pytest-cov = "^3.0.0"
 mock = "^4.0.3"
 pre-commit = "^2.17.0"
@@ -64,7 +69,9 @@
 [tool.yapfignore]
 ignore_patterns = [
     ".venv/**",
     ".pytest_cache/**",
     "dist/**",
     "docs/**"
 ]
+
+
```

### Comparing `volttron_lib_modbustk_driver-0.1.1a1/src/volttron/driver/interfaces/modbus_tk/modbus_tk.py` & `volttron_lib_modbustk_driver-0.1.2rc0/src/volttron/driver/interfaces/modbus_tk/modbus_tk.py`

 * *Files identical despite different names*

### Comparing `volttron_lib_modbustk_driver-0.1.1a1/src/volttron/driver/interfaces/modbus_tk/utils/client.py` & `volttron_lib_modbustk_driver-0.1.2rc0/src/volttron/driver/interfaces/modbus_tk/utils/client.py`

 * *Files identical despite different names*

### Comparing `volttron_lib_modbustk_driver-0.1.1a1/src/volttron/driver/interfaces/modbus_tk/utils/config_cmd.py` & `volttron_lib_modbustk_driver-0.1.2rc0/src/volttron/driver/interfaces/modbus_tk/utils/config_cmd.py`

 * *Files identical despite different names*

### Comparing `volttron_lib_modbustk_driver-0.1.1a1/src/volttron/driver/interfaces/modbus_tk/utils/helpers.py` & `volttron_lib_modbustk_driver-0.1.2rc0/src/volttron/driver/interfaces/modbus_tk/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `volttron_lib_modbustk_driver-0.1.1a1/src/volttron/driver/interfaces/modbus_tk/utils/maps/__init__.py` & `volttron_lib_modbustk_driver-0.1.2rc0/src/volttron/driver/interfaces/modbus_tk/utils/maps/__init__.py`

 * *Files identical despite different names*

### Comparing `volttron_lib_modbustk_driver-0.1.1a1/src/volttron/driver/interfaces/modbus_tk/utils/maps/battery_meter.csv` & `volttron_lib_modbustk_driver-0.1.2rc0/src/volttron/driver/interfaces/modbus_tk/utils/maps/battery_meter.csv`

 * *Files identical despite different names*

### Comparing `volttron_lib_modbustk_driver-0.1.1a1/src/volttron/driver/interfaces/modbus_tk/utils/maps/ion6200.config` & `volttron_lib_modbustk_driver-0.1.2rc0/src/volttron/driver/interfaces/modbus_tk/utils/maps/ion6200.config`

 * *Files identical despite different names*

### Comparing `volttron_lib_modbustk_driver-0.1.1a1/src/volttron/driver/interfaces/modbus_tk/utils/maps/ion6200_map.csv` & `volttron_lib_modbustk_driver-0.1.2rc0/src/volttron/driver/interfaces/modbus_tk/utils/maps/ion6200_map.csv`

 * *Files identical despite different names*

### Comparing `volttron_lib_modbustk_driver-0.1.1a1/src/volttron/driver/interfaces/modbus_tk/utils/maps/ion8600_map.csv` & `volttron_lib_modbustk_driver-0.1.2rc0/src/volttron/driver/interfaces/modbus_tk/utils/maps/ion8600_map.csv`

 * *Files identical despite different names*

### Comparing `volttron_lib_modbustk_driver-0.1.1a1/src/volttron/driver/interfaces/modbus_tk/utils/maps/maps.yaml` & `volttron_lib_modbustk_driver-0.1.2rc0/src/volttron/driver/interfaces/modbus_tk/utils/maps/maps.yaml`

 * *Files identical despite different names*

### Comparing `volttron_lib_modbustk_driver-0.1.1a1/src/volttron/driver/interfaces/modbus_tk/utils/maps/modbus_tk_test.config` & `volttron_lib_modbustk_driver-0.1.2rc0/src/volttron/driver/interfaces/modbus_tk/utils/maps/modbus_tk_test.config`

 * *Files identical despite different names*

### Comparing `volttron_lib_modbustk_driver-0.1.1a1/src/volttron/driver/interfaces/modbus_tk/utils/maps/watts_on.config` & `volttron_lib_modbustk_driver-0.1.2rc0/src/volttron/driver/interfaces/modbus_tk/utils/maps/watts_on.config`

 * *Files identical despite different names*

### Comparing `volttron_lib_modbustk_driver-0.1.1a1/src/volttron/driver/interfaces/modbus_tk/utils/maps/write_single_registers.config` & `volttron_lib_modbustk_driver-0.1.2rc0/src/volttron/driver/interfaces/modbus_tk/utils/maps/write_single_registers.config`

 * *Files identical despite different names*

### Comparing `volttron_lib_modbustk_driver-0.1.1a1/src/volttron/driver/interfaces/modbus_tk/utils/maps.py` & `volttron_lib_modbustk_driver-0.1.2rc0/src/volttron/driver/interfaces/modbus_tk/utils/maps.py`

 * *Files identical despite different names*

### Comparing `volttron_lib_modbustk_driver-0.1.1a1/src/volttron/driver/interfaces/modbus_tk/utils/server.py` & `volttron_lib_modbustk_driver-0.1.2rc0/src/volttron/driver/interfaces/modbus_tk/utils/server.py`

 * *Files identical despite different names*

### Comparing `volttron_lib_modbustk_driver-0.1.1a1/PKG-INFO` & `volttron_lib_modbustk_driver-0.1.2rc0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,979 +1,1144 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 766f 6c74  : 2.1.Name: volt
 00000020: 7472 6f6e 2d6c 6962 2d6d 6f64 6275 7374  tron-lib-modbust
 00000030: 6b2d 6472 6976 6572 0a56 6572 7369 6f6e  k-driver.Version
-00000040: 3a20 302e 312e 3161 310a 5375 6d6d 6172  : 0.1.1a1.Summar
-00000050: 793a 204d 6f64 6275 7354 4b20 4472 6976  y: ModbusTK Driv
-00000060: 6572 2073 7570 706f 7274 6564 2061 6e64  er supported and
-00000070: 206d 6169 6e74 6169 6e65 6420 6279 2074   maintained by t
-00000080: 6865 2056 6f6c 7474 726f 6e20 7465 616d  he Volttron team
-00000090: 2e0a 486f 6d65 2d70 6167 653a 2068 7474  ..Home-page: htt
-000000a0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-000000b0: 564f 4c54 5452 4f4e 2f76 6f6c 7474 726f  VOLTTRON/volttro
-000000c0: 6e2d 6472 6976 6572 732f 766f 6c74 7472  n-drivers/volttr
-000000d0: 6f6e 2d6c 6962 2d6d 6f64 6275 7374 6b2d  on-lib-modbustk-
-000000e0: 6472 6976 6572 0a4c 6963 656e 7365 3a20  driver.License: 
-000000f0: 4170 6163 6865 2d32 2e30 0a41 7574 686f  Apache-2.0.Autho
-00000100: 723a 204d 6172 6b20 426f 6e69 6369 6c6c  r: Mark Bonicill
-00000110: 6f0a 4175 7468 6f72 2d65 6d61 696c 3a20  o.Author-email: 
-00000120: 766f 6c74 7472 6f6e 4070 6e6e 6c2e 676f  volttron@pnnl.go
-00000130: 760a 5265 7175 6972 6573 2d50 7974 686f  v.Requires-Pytho
-00000140: 6e3a 203e 3d33 2e38 2c3c 342e 300a 436c  n: >=3.8,<4.0.Cl
-00000150: 6173 7369 6669 6572 3a20 496e 7465 6e64  assifier: Intend
-00000160: 6564 2041 7564 6965 6e63 6520 3a3a 2044  ed Audience :: D
-00000170: 6576 656c 6f70 6572 730a 436c 6173 7369  evelopers.Classi
-00000180: 6669 6572 3a20 496e 7465 6e64 6564 2041  fier: Intended A
-00000190: 7564 6965 6e63 6520 3a3a 2049 6e66 6f72  udience :: Infor
-000001a0: 6d61 7469 6f6e 2054 6563 686e 6f6c 6f67  mation Technolog
-000001b0: 790a 436c 6173 7369 6669 6572 3a20 496e  y.Classifier: In
-000001c0: 7465 6e64 6564 2041 7564 6965 6e63 6520  tended Audience 
-000001d0: 3a3a 204f 7468 6572 2041 7564 6965 6e63  :: Other Audienc
-000001e0: 650a 436c 6173 7369 6669 6572 3a20 496e  e.Classifier: In
-000001f0: 7465 6e64 6564 2041 7564 6965 6e63 6520  tended Audience 
-00000200: 3a3a 2053 6369 656e 6365 2f52 6573 6561  :: Science/Resea
-00000210: 7263 680a 436c 6173 7369 6669 6572 3a20  rch.Classifier: 
-00000220: 4c69 6365 6e73 6520 3a3a 204f 5349 2041  License :: OSI A
-00000230: 7070 726f 7665 6420 3a3a 2041 7061 6368  pproved :: Apach
-00000240: 6520 536f 6674 7761 7265 204c 6963 656e  e Software Licen
-00000250: 7365 0a43 6c61 7373 6966 6965 723a 2050  se.Classifier: P
-00000260: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
-00000270: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
-00000280: 2033 0a43 6c61 7373 6966 6965 723a 2050   3.Classifier: P
-00000290: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
-000002a0: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
-000002b0: 2033 2e38 0a43 6c61 7373 6966 6965 723a   3.8.Classifier:
-000002c0: 2050 726f 6772 616d 6d69 6e67 204c 616e   Programming Lan
-000002d0: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
-000002e0: 3a3a 2033 2e39 0a43 6c61 7373 6966 6965  :: 3.9.Classifie
-000002f0: 723a 2050 726f 6772 616d 6d69 6e67 204c  r: Programming L
-00000300: 616e 6775 6167 6520 3a3a 2050 7974 686f  anguage :: Pytho
-00000310: 6e20 3a3a 2033 2e31 300a 436c 6173 7369  n :: 3.10.Classi
-00000320: 6669 6572 3a20 5072 6f67 7261 6d6d 696e  fier: Programmin
-00000330: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
-00000340: 7468 6f6e 203a 3a20 332e 3131 0a43 6c61  thon :: 3.11.Cla
-00000350: 7373 6966 6965 723a 2050 726f 6772 616d  ssifier: Program
-00000360: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
-00000370: 2050 7974 686f 6e20 3a3a 2033 203a 3a20   Python :: 3 :: 
-00000380: 4f6e 6c79 0a52 6571 7569 7265 732d 4469  Only.Requires-Di
-00000390: 7374 3a20 5079 5941 4d4c 2028 3e3d 362e  st: PyYAML (>=6.
-000003a0: 302c 3c37 2e30 290a 5265 7175 6972 6573  0,<7.0).Requires
-000003b0: 2d44 6973 743a 206d 6f64 6275 732d 746b  -Dist: modbus-tk
-000003c0: 2028 3e3d 312e 312e 322c 3c32 2e30 2e30   (>=1.1.2,<2.0.0
-000003d0: 290a 5265 7175 6972 6573 2d44 6973 743a  ).Requires-Dist:
-000003e0: 2070 7973 6572 6961 6c20 283e 3d33 2e35   pyserial (>=3.5
-000003f0: 2c3c 342e 3029 0a52 6571 7569 7265 732d  ,<4.0).Requires-
-00000400: 4469 7374 3a20 766f 6c74 7472 6f6e 2d6c  Dist: volttron-l
-00000410: 6962 2d62 6173 652d 6472 6976 6572 2028  ib-base-driver (
-00000420: 3e3d 302e 322e 3072 6330 2c3c 302e 332e  >=0.2.0rc0,<0.3.
-00000430: 3029 0a50 726f 6a65 6374 2d55 524c 3a20  0).Project-URL: 
-00000440: 5265 706f 7369 746f 7279 2c20 6874 7470  Repository, http
-00000450: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f56  s://github.com/V
-00000460: 4f4c 5454 524f 4e2f 766f 6c74 7472 6f6e  OLTTRON/volttron
-00000470: 2d6c 6962 2d6d 6f64 6275 7374 6b2d 6472  -lib-modbustk-dr
-00000480: 6976 6572 0a44 6573 6372 6970 7469 6f6e  iver.Description
-00000490: 2d43 6f6e 7465 6e74 2d54 7970 653a 2074  -Content-Type: t
-000004a0: 6578 742f 6d61 726b 646f 776e 0a0a 2320  ext/markdown..# 
-000004b0: 766f 6c74 7472 6f6e 2d6c 6962 2d6d 6f64  volttron-lib-mod
-000004c0: 6275 7374 6b2d 6472 6976 6572 0a0a 215b  bustk-driver..![
-000004d0: 5061 7373 696e 673f 5d28 6874 7470 733a  Passing?](https:
-000004e0: 2f2f 6769 7468 7562 2e63 6f6d 2f56 4f4c  //github.com/VOL
-000004f0: 5454 524f 4e2f 766f 6c74 7472 6f6e 2d6c  TTRON/volttron-l
-00000500: 6962 2d6d 6f64 6275 7374 6b2d 6472 6976  ib-modbustk-driv
-00000510: 6572 2f61 6374 696f 6e73 2f77 6f72 6b66  er/actions/workf
-00000520: 6c6f 7773 2f72 756e 2d74 6573 7473 2e79  lows/run-tests.y
-00000530: 6d6c 2f62 6164 6765 2e73 7667 290a 5b21  ml/badge.svg).[!
-00000540: 5b70 7970 6920 7665 7273 696f 6e5d 2868  [pypi version](h
-00000550: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
-00000560: 6473 2e69 6f2f 7079 7069 2f76 2f76 6f6c  ds.io/pypi/v/vol
+00000040: 3a20 302e 312e 3272 6330 0a53 756d 6d61  : 0.1.2rc0.Summa
+00000050: 7279 3a20 4d6f 6462 7573 544b 2044 7269  ry: ModbusTK Dri
+00000060: 7665 7220 7375 7070 6f72 7465 6420 616e  ver supported an
+00000070: 6420 6d61 696e 7461 696e 6564 2062 7920  d maintained by 
+00000080: 7468 6520 566f 6c74 7472 6f6e 2074 6561  the Volttron tea
+00000090: 6d2e 0a48 6f6d 652d 7061 6765 3a20 6874  m..Home-page: ht
+000000a0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+000000b0: 2f56 4f4c 5454 524f 4e2f 766f 6c74 7472  /VOLTTRON/volttr
+000000c0: 6f6e 2d64 7269 7665 7273 2f76 6f6c 7474  on-drivers/voltt
+000000d0: 726f 6e2d 6c69 622d 6d6f 6462 7573 746b  ron-lib-modbustk
+000000e0: 2d64 7269 7665 720a 4c69 6365 6e73 653a  -driver.License:
+000000f0: 2041 7061 6368 652d 322e 300a 4175 7468   Apache-2.0.Auth
+00000100: 6f72 3a20 4d61 726b 2042 6f6e 6963 696c  or: Mark Bonicil
+00000110: 6c6f 0a41 7574 686f 722d 656d 6169 6c3a  lo.Author-email:
+00000120: 2076 6f6c 7474 726f 6e40 706e 6e6c 2e67   volttron@pnnl.g
+00000130: 6f76 0a52 6571 7569 7265 732d 5079 7468  ov.Requires-Pyth
+00000140: 6f6e 3a20 3e3d 332e 3130 2c3c 342e 300a  on: >=3.10,<4.0.
+00000150: 436c 6173 7369 6669 6572 3a20 496e 7465  Classifier: Inte
+00000160: 6e64 6564 2041 7564 6965 6e63 6520 3a3a  nded Audience ::
+00000170: 2044 6576 656c 6f70 6572 730a 436c 6173   Developers.Clas
+00000180: 7369 6669 6572 3a20 496e 7465 6e64 6564  sifier: Intended
+00000190: 2041 7564 6965 6e63 6520 3a3a 2049 6e66   Audience :: Inf
+000001a0: 6f72 6d61 7469 6f6e 2054 6563 686e 6f6c  ormation Technol
+000001b0: 6f67 790a 436c 6173 7369 6669 6572 3a20  ogy.Classifier: 
+000001c0: 496e 7465 6e64 6564 2041 7564 6965 6e63  Intended Audienc
+000001d0: 6520 3a3a 204f 7468 6572 2041 7564 6965  e :: Other Audie
+000001e0: 6e63 650a 436c 6173 7369 6669 6572 3a20  nce.Classifier: 
+000001f0: 496e 7465 6e64 6564 2041 7564 6965 6e63  Intended Audienc
+00000200: 6520 3a3a 2053 6369 656e 6365 2f52 6573  e :: Science/Res
+00000210: 6561 7263 680a 436c 6173 7369 6669 6572  earch.Classifier
+00000220: 3a20 4c69 6365 6e73 6520 3a3a 204f 5349  : License :: OSI
+00000230: 2041 7070 726f 7665 6420 3a3a 2041 7061   Approved :: Apa
+00000240: 6368 6520 536f 6674 7761 7265 204c 6963  che Software Lic
+00000250: 656e 7365 0a43 6c61 7373 6966 6965 723a  ense.Classifier:
+00000260: 2050 726f 6772 616d 6d69 6e67 204c 616e   Programming Lan
+00000270: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
+00000280: 3a3a 2033 0a43 6c61 7373 6966 6965 723a  :: 3.Classifier:
+00000290: 2050 726f 6772 616d 6d69 6e67 204c 616e   Programming Lan
+000002a0: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
+000002b0: 3a3a 2033 2e31 300a 436c 6173 7369 6669  :: 3.10.Classifi
+000002c0: 6572 3a20 5072 6f67 7261 6d6d 696e 6720  er: Programming 
+000002d0: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
+000002e0: 6f6e 203a 3a20 332e 3131 0a43 6c61 7373  on :: 3.11.Class
+000002f0: 6966 6965 723a 2050 726f 6772 616d 6d69  ifier: Programmi
+00000300: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
+00000310: 7974 686f 6e20 3a3a 2033 203a 3a20 4f6e  ython :: 3 :: On
+00000320: 6c79 0a52 6571 7569 7265 732d 4469 7374  ly.Requires-Dist
+00000330: 3a20 5079 5941 4d4c 2028 3e3d 362e 302c  : PyYAML (>=6.0,
+00000340: 3c37 2e30 290a 5265 7175 6972 6573 2d44  <7.0).Requires-D
+00000350: 6973 743a 206d 6f64 6275 732d 746b 2028  ist: modbus-tk (
+00000360: 3e3d 312e 312e 332c 3c32 2e30 2e30 290a  >=1.1.3,<2.0.0).
+00000370: 5265 7175 6972 6573 2d44 6973 743a 2070  Requires-Dist: p
+00000380: 7973 6572 6961 6c20 283e 3d33 2e35 2c3c  yserial (>=3.5,<
+00000390: 342e 3029 0a52 6571 7569 7265 732d 4469  4.0).Requires-Di
+000003a0: 7374 3a20 766f 6c74 7472 6f6e 2d6c 6962  st: volttron-lib
+000003b0: 2d62 6173 652d 6472 6976 6572 2028 3e3d  -base-driver (>=
+000003c0: 302e 322e 3172 6332 2c3c 302e 332e 3029  0.2.1rc2,<0.3.0)
+000003d0: 0a50 726f 6a65 6374 2d55 524c 3a20 5265  .Project-URL: Re
+000003e0: 706f 7369 746f 7279 2c20 6874 7470 733a  pository, https:
+000003f0: 2f2f 6769 7468 7562 2e63 6f6d 2f56 4f4c  //github.com/VOL
+00000400: 5454 524f 4e2f 766f 6c74 7472 6f6e 2d6c  TTRON/volttron-l
+00000410: 6962 2d6d 6f64 6275 7374 6b2d 6472 6976  ib-modbustk-driv
+00000420: 6572 0a44 6573 6372 6970 7469 6f6e 2d43  er.Description-C
+00000430: 6f6e 7465 6e74 2d54 7970 653a 2074 6578  ontent-Type: tex
+00000440: 742f 6d61 726b 646f 776e 0a0a 2320 766f  t/markdown..# vo
+00000450: 6c74 7472 6f6e 2d6c 6962 2d6d 6f64 6275  lttron-lib-modbu
+00000460: 7374 6b2d 6472 6976 6572 0a0a 215b 4563  stk-driver..![Ec
+00000470: 6c69 7073 6520 564f 4c54 5452 4f4e e284  lipse VOLTTRON..
+00000480: a25d 2868 7474 7073 3a2f 2f69 6d67 2e73  .](https://img.s
+00000490: 6869 656c 6473 2e69 6f2f 6261 6467 652f  hields.io/badge/
+000004a0: 4563 6c69 7073 6525 3230 564f 4c54 5452  Eclipse%20VOLTTR
+000004b0: 4f4e e284 a22d 2d72 6564 2e73 7667 290a  ON...--red.svg).
+000004c0: 215b 5079 7468 6f6e 2033 2e31 305d 2868  ![Python 3.10](h
+000004d0: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
+000004e0: 6473 2e69 6f2f 6261 6467 652f 7079 7468  ds.io/badge/pyth
+000004f0: 6f6e 2d33 2e31 302d 626c 7565 2e73 7667  on-3.10-blue.svg
+00000500: 290a 215b 5079 7468 6f6e 2033 2e31 315d  ).![Python 3.11]
+00000510: 2868 7474 7073 3a2f 2f69 6d67 2e73 6869  (https://img.shi
+00000520: 656c 6473 2e69 6f2f 6261 6467 652f 7079  elds.io/badge/py
+00000530: 7468 6f6e 2d33 2e31 312d 626c 7565 2e73  thon-3.11-blue.s
+00000540: 7667 290a 5b21 5b50 6173 7369 6e67 3f5d  vg).[![Passing?]
+00000550: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+00000560: 636f 6d2f 564f 4c54 5452 4f4e 2f76 6f6c  com/VOLTTRON/vol
 00000570: 7474 726f 6e2d 6c69 622d 6d6f 6462 7573  ttron-lib-modbus
-00000580: 746b 2d64 7269 7665 722e 7376 6729 5d28  tk-driver.svg)](
-00000590: 6874 7470 733a 2f2f 7079 7069 2e6f 7267  https://pypi.org
-000005a0: 2f70 726f 6a65 6374 2f76 6f6c 7474 726f  /project/volttro
-000005b0: 6e2d 6c69 622d 6d6f 6462 7573 746b 2d64  n-lib-modbustk-d
-000005c0: 7269 7665 722f 290a 0a56 4f4c 5454 524f  river/)..VOLTTRO
-000005d0: 4ee2 8099 7320 4d6f 6462 7573 2d54 4b20  N...s Modbus-TK 
-000005e0: 6472 6976 6572 2c20 6275 696c 7420 6f6e  driver, built on
-000005f0: 2074 6865 2050 7974 686f 6e20 4d6f 6462   the Python Modb
-00000600: 7573 2d54 4b20 6c69 6272 6172 792c 2069  us-TK library, i
-00000610: 7320 616e 2061 6c74 6572 6e61 7469 7665  s an alternative
-00000620: 2074 6f20 7468 6520 6f72 6967 696e 616c   to the original
-00000630: 2056 4f4c 5454 524f 4e20 6d6f 6462 7573   VOLTTRON modbus
-00000640: 2064 7269 7665 722e 2055 6e6c 696b 6520   driver. Unlike 
-00000650: 7468 6520 6f72 6967 696e 616c 206d 6f64  the original mod
-00000660: 6275 7320 6472 6976 6572 2c20 7468 6520  bus driver, the 
-00000670: 4d6f 6462 7573 2d54 4b20 6472 6976 6572  Modbus-TK driver
-00000680: 2073 7570 706f 7274 7320 4d6f 6462 7573   supports Modbus
-00000690: 2052 5455 2061 7320 7765 6c6c 2061 7320   RTU as well as 
-000006a0: 4d6f 6462 7573 206f 7665 7220 5443 502f  Modbus over TCP/
-000006b0: 4950 2e0a 0a23 2050 7265 7265 7175 6973  IP...# Prerequis
-000006c0: 6974 6573 0a0a 2a20 5079 7468 6f6e 2033  ites..* Python 3
-000006d0: 2e38 0a0a 2320 496e 7374 616c 6c61 7469  .8..# Installati
-000006e0: 6f6e 0a0a 312e 2043 7265 6174 6520 616e  on..1. Create an
-000006f0: 6420 6163 7469 7661 7465 2061 2076 6972  d activate a vir
-00000700: 7475 616c 2065 6e76 6972 6f6e 6d65 6e74  tual environment
-00000710: 2e0a 0a20 2020 2060 6060 7368 656c 6c0a  ...    ```shell.
-00000720: 2020 2020 7079 7468 6f6e 202d 6d20 7665      python -m ve
-00000730: 6e76 2065 6e76 0a20 2020 2073 6f75 7263  nv env.    sourc
-00000740: 6520 656e 762f 6269 6e2f 6163 7469 7661  e env/bin/activa
-00000750: 7465 0a20 2020 2060 6060 0a0a 312e 2049  te.    ```..1. I
-00000760: 6e73 7461 6c6c 2076 6f6c 7474 726f 6e20  nstall volttron 
-00000770: 616e 6420 7374 6172 7420 7468 6520 706c  and start the pl
-00000780: 6174 666f 726d 2e0a 0a20 2020 2060 6060  atform...    ```
-00000790: 7368 656c 6c0a 2020 2020 7069 7020 696e  shell.    pip in
-000007a0: 7374 616c 6c20 766f 6c74 7472 6f6e 0a0a  stall volttron..
-000007b0: 2020 2020 2320 5374 6172 7420 706c 6174      # Start plat
-000007c0: 666f 726d 2077 6974 6820 6f75 7470 7574  form with output
-000007d0: 2067 6f69 6e67 2074 6f20 766f 6c74 7472   going to volttr
-000007e0: 6f6e 2e6c 6f67 0a20 2020 2076 6f6c 7474  on.log.    voltt
-000007f0: 726f 6e20 2d76 7620 2d6c 2076 6f6c 7474  ron -vv -l voltt
-00000800: 726f 6e2e 6c6f 6720 260a 2020 2020 6060  ron.log &.    ``
-00000810: 600a 0a31 2e20 496e 7374 616c 6c20 7468  `..1. Install th
-00000820: 6520 766f 6c74 7472 6f6e 2070 6c61 7466  e volttron platf
-00000830: 6f72 6d20 6472 6976 6572 3a0a 0a20 2020  orm driver:..   
-00000840: 2060 6060 7368 656c 6c0a 2020 2020 7663   ```shell.    vc
-00000850: 746c 2069 6e73 7461 6c6c 2076 6f6c 7474  tl install voltt
-00000860: 726f 6e2d 706c 6174 666f 726d 2d64 7269  ron-platform-dri
-00000870: 7665 7220 2d2d 7669 702d 6964 656e 7469  ver --vip-identi
-00000880: 7479 2070 6c61 7466 6f72 6d2e 6472 6976  ty platform.driv
-00000890: 6572 202d 2d73 7461 7274 0a20 2020 2060  er --start.    `
-000008a0: 6060 0a0a 312e 2049 6e73 7461 6c6c 2074  ``..1. Install t
-000008b0: 6865 2076 6f6c 7474 726f 6e2d 6c69 622d  he volttron-lib-
-000008c0: 6d6f 6462 7573 746b 2d64 7269 7665 7220  modbustk-driver 
-000008d0: 6c69 6272 6172 792e 0a0a 2020 2020 6060  library...    ``
-000008e0: 6073 6865 6c6c 0a20 2020 2070 6970 2069  `shell.    pip i
-000008f0: 6e73 7461 6c6c 2076 6f6c 7474 726f 6e2d  nstall volttron-
-00000900: 6c69 622d 6d6f 6462 7573 746b 2d64 7269  lib-modbustk-dri
-00000910: 7665 720a 2020 2020 6060 600a 0a31 2e20  ver.    ```..1. 
-00000920: 496e 7374 616c 6c20 7468 6520 6472 6976  Install the driv
-00000930: 6572 206f 6e74 6f20 7468 6520 506c 6174  er onto the Plat
-00000940: 666f 726d 2044 7269 7665 722e 0a0a 2020  form Driver...  
-00000950: 2020 496e 7374 616c 6c69 6e67 2061 2064    Installing a d
-00000960: 7269 7665 7220 696e 2074 6865 2050 6c61  river in the Pla
-00000970: 7466 6f72 6d20 4472 6976 6572 2041 6765  tform Driver Age
-00000980: 6e74 2072 6571 7569 7265 7320 6164 6469  nt requires addi
-00000990: 6e67 2063 6f70 6965 7320 6f66 2074 6865  ng copies of the
-000009a0: 2064 6576 6963 6520 636f 6e66 6967 7572   device configur
-000009b0: 6174 696f 6e20 616e 6420 7265 6769 7374  ation and regist
-000009c0: 7279 2063 6f6e 6669 6775 7261 7469 6f6e  ry configuration
-000009d0: 2066 696c 6573 2074 6f20 7468 6520 506c   files to the Pl
-000009e0: 6174 666f 726d 2044 7269 7665 72e2 8099  atform Driver...
-000009f0: 7320 636f 6e66 6967 7572 6174 696f 6e20  s configuration 
-00000a00: 7374 6f72 652e 0a0a 2020 2020 4372 6561  store...    Crea
-00000a10: 7465 2061 2063 6f6e 6669 6720 6469 7265  te a config dire
-00000a20: 6374 6f72 7920 616e 6420 6e61 7669 6761  ctory and naviga
-00000a30: 7465 2074 6f20 6974 3a0a 0a20 2020 2060  te to it:..    `
-00000a40: 6060 7368 656c 6c0a 2020 2020 6d6b 6469  ``shell.    mkdi
-00000a50: 7220 636f 6e66 6967 0a20 2020 2063 6420  r config.    cd 
-00000a60: 636f 6e66 6967 0a20 2020 2060 6060 0a0a  config.    ```..
-00000a70: 312e 2041 6464 2064 7269 7665 7220 636f  1. Add driver co
-00000a80: 6e66 6967 7572 6174 696f 6e73 2074 6f20  nfigurations to 
-00000a90: 7468 6520 506c 6174 666f 726d 2044 7269  the Platform Dri
-00000aa0: 7665 722e 0a0a 2020 2054 6865 204d 6f64  ver...   The Mod
-00000ab0: 6275 732d 544b 2064 7269 7665 7220 6973  bus-TK driver is
-00000ac0: 206d 6f73 746c 7920 6261 636b 7761 7264   mostly backward
-00000ad0: 2d63 6f6d 7061 7469 626c 6520 7769 7468  -compatible with
-00000ae0: 2074 6865 2070 6172 616d 6574 6572 2064   the parameter d
-00000af0: 6566 696e 6974 696f 6e73 2069 6e20 7468  efinitions in th
-00000b00: 6520 6f72 6967 696e 616c 204d 6f64 6275  e original Modbu
-00000b10: 7320 6472 6976 6572 e280 9973 2063 6f6e  s driver...s con
-00000b20: 6669 6775 7261 7469 6f6e 2028 2e63 6f6e  figuration (.con
-00000b30: 6669 6720 616e 6420 2e63 7376 2066 696c  fig and .csv fil
-00000b40: 6573 292e 2049 6620 7468 6520 636f 6e66  es). If the conf
-00000b50: 6967 2066 696c 65e2 8099 7320 7061 7261  ig file...s para
-00000b60: 6d65 7465 7220 6e61 6d65 7320 7573 6520  meter names use 
-00000b70: 7468 6520 4d6f 6462 7573 2064 7269 7665  the Modbus drive
-00000b80: 72e2 8099 7320 6e61 6d65 2063 6f6e 7665  r...s name conve
-00000b90: 6e74 696f 6e73 2c20 7468 6579 2061 7265  ntions, they are
-00000ba0: 2074 7261 6e73 6c61 7465 6420 746f 2074   translated to t
-00000bb0: 6865 204d 6f64 6275 732d 544b 206e 616d  he Modbus-TK nam
-00000bc0: 6520 636f 6e76 656e 7469 6f6e 732c 2065  e conventions, e
-00000bd0: 2e67 2e20 6120 4d6f 6462 7573 2043 5356  .g. a Modbus CSV
-00000be0: 2066 696c 65e2 8099 7320 506f 696e 7420   file...s Point 
-00000bf0: 4164 6472 6573 7320 6973 2069 6e74 6572  Address is inter
-00000c00: 7072 6574 6564 2061 7320 6120 4d6f 6462  preted as a Modb
-00000c10: 7573 2d54 4b20 e280 9c41 6464 7265 7373  us-TK ...Address
-00000c20: e280 9d2e 2042 6163 6b77 6172 642d 636f  .... Backward-co
-00000c30: 6d70 6174 6962 696c 6974 7920 6578 6365  mpatibility exce
-00000c40: 7074 696f 6e73 2061 7265 3a0a 0a20 2020  ptions are:..   
-00000c50: 2020 2020 202a 2049 6620 7468 6520 636f       * If the co
-00000c60: 6e66 6967 2066 696c 6520 6861 7320 6e6f  nfig file has no
-00000c70: 2070 6f72 742c 2074 6865 2064 6566 6175   port, the defau
-00000c80: 6c74 2069 7320 302c 206e 6f74 2035 3032  lt is 0, not 502
-00000c90: 2e0a 0a20 2020 2020 2020 202a 2049 6620  ...        * If 
-00000ca0: 7468 6520 636f 6e66 6967 2066 696c 6520  the config file 
-00000cb0: 6861 7320 6e6f 2073 6c61 7665 5f69 642c  has no slave_id,
-00000cc0: 2074 6865 2064 6566 6175 6c74 2069 7320   the default is 
-00000cd0: 312c 206e 6f74 2030 2e0a 0a20 2020 2054  1, not 0...    T
-00000ce0: 6865 2064 7269 7665 725f 636f 6e66 6967  he driver_config
-00000cf0: 2073 6563 7469 6f6e 206f 6620 6120 4d6f   section of a Mo
-00000d00: 6462 7573 2d54 4b20 6465 7669 6365 2063  dbus-TK device c
-00000d10: 6f6e 6669 6775 7261 7469 6f6e 2066 696c  onfiguration fil
-00000d20: 6520 7375 7070 6f72 7473 2061 2076 6172  e supports a var
-00000d30: 6965 7479 206f 6620 7061 7261 6d65 7465  iety of paramete
-00000d40: 7220 6465 6669 6e69 7469 6f6e 732c 2062  r definitions, b
-00000d50: 7574 206f 6e6c 7920 2a64 6576 6963 655f  ut only *device_
-00000d60: 6164 6472 6573 732a 2069 7320 7265 7175  address* is requ
-00000d70: 6972 6564 3a0a 0a20 2020 202a 2064 6576  ired:..    * dev
-00000d80: 6963 655f 6164 6472 6573 7320 2852 6571  ice_address (Req
-00000d90: 7569 7265 6429 3a20 2049 5020 4164 6472  uired):  IP Addr
-00000da0: 6573 7320 6f66 2074 6865 2064 6576 6963  ess of the devic
-00000db0: 652e 0a0a 2020 2020 2a20 6e61 6d65 2028  e...    * name (
-00000dc0: 4f70 7469 6f6e 616c 2920 2d20 4e61 6d65  Optional) - Name
-00000dd0: 206f 6620 7468 6520 6465 7669 6365 2e20   of the device. 
-00000de0: 4465 6661 756c 7473 2074 6f20 e280 9c55  Defaults to ...U
-00000df0: 4e4b 4e4f 574e e280 9d2e 0a0a 2020 2020  NKNOWN......    
-00000e00: 2a20 6465 7669 6365 5f74 7970 6520 284f  * device_type (O
-00000e10: 7074 696f 6e61 6c29 202d 204e 616d 6520  ptional) - Name 
-00000e20: 6f66 2074 6865 2064 6576 6963 6520 7479  of the device ty
-00000e30: 7065 2e20 4465 6661 756c 7473 2074 6f20  pe. Defaults to 
-00000e40: e280 9c55 4e4b 4e4f 574e e280 9d2e 0a0a  ...UNKNOWN......
-00000e50: 2020 2020 2a20 706f 7274 2028 4f70 7469      * port (Opti
-00000e60: 6f6e 616c 2920 2d20 506f 7274 2074 6865  onal) - Port the
-00000e70: 2064 6576 6963 6520 6973 206c 6973 7465   device is liste
-00000e80: 6e69 6e67 206f 6e2e 2044 6566 6175 6c74  ning on. Default
-00000e90: 7320 746f 2030 2028 6e6f 2070 6f72 7429  s to 0 (no port)
-00000ea0: 2e20 5573 6520 706f 7274 2030 2066 6f72  . Use port 0 for
-00000eb0: 2052 5455 2074 7261 6e73 706f 7274 2e0a   RTU transport..
-00000ec0: 0a20 2020 202a 2073 6c61 7665 5f69 6420  .    * slave_id 
-00000ed0: 284f 7074 696f 6e61 6c29 202d 2053 6c61  (Optional) - Sla
-00000ee0: 7665 2049 4420 6f66 2074 6865 2064 6576  ve ID of the dev
-00000ef0: 6963 652e 2044 6566 6175 6c74 7320 746f  ice. Defaults to
-00000f00: 2031 2e20 5573 6520 4944 2030 2066 6f72   1. Use ID 0 for
-00000f10: 206e 6f20 736c 6176 652e 0a0a 2020 2020   no slave...    
-00000f20: 2a20 6261 7564 7261 7465 2028 4f70 7469  * baudrate (Opti
-00000f30: 6f6e 616c 2920 2d20 5365 7269 616c 2028  onal) - Serial (
-00000f40: 5254 5529 2062 6175 6420 7261 7465 2e20  RTU) baud rate. 
-00000f50: 4465 6661 756c 7473 2074 6f20 3936 3030  Defaults to 9600
-00000f60: 2e0a 0a20 2020 202a 2062 7974 6573 697a  ...    * bytesiz
-00000f70: 6520 284f 7074 696f 6e61 6c29 202d 2053  e (Optional) - S
-00000f80: 6572 6961 6c20 2852 5455 2920 6279 7465  erial (RTU) byte
-00000f90: 2073 697a 653a 2035 2c20 362c 2037 2c20   size: 5, 6, 7, 
-00000fa0: 6f72 2038 2e20 4465 6661 756c 7473 2074  or 8. Defaults t
-00000fb0: 6f20 382e 0a0a 2020 2020 2a20 7061 7269  o 8...    * pari
-00000fc0: 7479 2028 4f70 7469 6f6e 616c 2920 2d20  ty (Optional) - 
-00000fd0: 5365 7269 616c 2028 5254 5529 2070 6172  Serial (RTU) par
-00000fe0: 6974 793a 206e 6f6e 652c 2065 7665 6e2c  ity: none, even,
-00000ff0: 206f 6464 2c20 6d61 726b 2c20 6f72 2073   odd, mark, or s
-00001000: 7061 6365 2e20 4465 6661 756c 7473 2074  pace. Defaults t
-00001010: 6f20 4e6f 6e65 2e0a 0a20 2020 202a 2073  o None...    * s
-00001020: 746f 7062 6974 7320 284f 7074 696f 6e61  topbits (Optiona
-00001030: 6c29 202d 2053 6572 6961 6c20 2852 5455  l) - Serial (RTU
-00001040: 2920 7374 6f70 2062 6974 733a 2031 2c20  ) stop bits: 1, 
-00001050: 312e 352c 206f 7220 322e 2044 6566 6175  1.5, or 2. Defau
-00001060: 6c74 7320 746f 2031 2e0a 0a20 2020 202a  lts to 1...    *
-00001070: 2078 6f6e 786f 6666 2028 4f70 7469 6f6e   xonxoff (Option
-00001080: 616c 2920 2d20 5365 7269 616c 2028 5254  al) - Serial (RT
-00001090: 5529 2066 6c6f 7720 636f 6e74 726f 6c3a  U) flow control:
-000010a0: 2030 206f 7220 312e 2044 6566 6175 6c74   0 or 1. Default
-000010b0: 7320 746f 2030 2e0a 0a20 2020 202a 2061  s to 0...    * a
-000010c0: 6464 7265 7373 696e 6720 284f 7074 696f  ddressing (Optio
-000010d0: 6e61 6c29 202d 2044 6174 6120 6164 6472  nal) - Data addr
-000010e0: 6573 7320 7461 626c 653a 206f 6666 7365  ess table: offse
-000010f0: 742c 206f 6666 7365 745f 706c 7573 2c20  t, offset_plus, 
-00001100: 6f72 2061 6464 7265 7373 2e20 4465 6661  or address. Defa
-00001110: 756c 7473 2074 6f20 6f66 6673 6574 2e0a  ults to offset..
-00001120: 0a20 2020 2020 202a 2061 6464 7265 7373  .      * address
-00001130: 3a20 5468 6520 6578 6163 7420 7661 6c75  : The exact valu
-00001140: 6520 6f66 2074 6865 2061 6464 7265 7373  e of the address
-00001150: 2077 6974 686f 7574 2061 6e79 206f 6666   without any off
-00001160: 7365 7420 7661 6c75 652e 0a0a 2020 2020  set value...    
-00001170: 2020 2a20 6f66 6673 6574 3a20 5468 6520    * offset: The 
-00001180: 7661 6c75 6520 6f66 2074 6865 2061 6464  value of the add
-00001190: 7265 7373 2070 6c75 7320 7468 6520 6f66  ress plus the of
-000011a0: 6673 6574 2076 616c 7565 2e0a 0a20 2020  fset value...   
-000011b0: 2020 202a 206f 6666 7365 745f 706c 7573     * offset_plus
-000011c0: 3a20 5468 6520 7661 6c75 6520 6f66 2074  : The value of t
-000011d0: 6865 2061 6464 7265 7373 2070 6c75 7320  he address plus 
-000011e0: 7468 6520 6f66 6673 6574 2076 616c 7565  the offset value
-000011f0: 2070 6c75 7320 6f6e 652e 0a0a 2020 2020   plus one...    
-00001200: 2020 2a20 3a20 4966 2061 6e20 6f66 6673    * : If an offs
-00001210: 6574 2076 616c 7565 2069 7320 746f 2062  et value is to b
-00001220: 6520 6164 6465 642c 2069 7420 6973 2064  e added, it is d
-00001230: 6574 6572 6d69 6e65 6420 6261 7365 6420  etermined based 
-00001240: 6f6e 2061 2070 6f69 6e74 e280 9973 2070  on a point...s p
-00001250: 726f 7065 7274 6965 7320 696e 2074 6865  roperties in the
-00001260: 2043 5356 2066 696c 653a 0a0a 2020 2020   CSV file:..    
-00001270: 2020 2020 2a20 5479 7065 3d62 6f6f 6c2c      * Type=bool,
-00001280: 2057 7269 7461 626c 653d 5452 5545 3a20   Writable=TRUE: 
-00001290: 300a 0a20 2020 2020 2020 202a 2054 7970  0..        * Typ
-000012a0: 653d 626f 6f6c 2c20 5772 6974 6162 6c65  e=bool, Writable
-000012b0: 3d46 414c 5345 3a20 3130 3030 300a 0a20  =FALSE: 10000.. 
-000012c0: 2020 2020 2020 202a 2054 7970 6521 3d62         * Type!=b
-000012d0: 6f6f 6c2c 2057 7269 7461 626c 653d 5452  ool, Writable=TR
-000012e0: 5545 3a20 3330 3030 300a 0a20 2020 2020  UE: 30000..     
-000012f0: 2020 202a 2054 7970 6521 3d62 6f6f 6c2c     * Type!=bool,
-00001300: 2057 7269 7461 626c 653d 4641 4c53 453a   Writable=FALSE:
-00001310: 2034 3030 3030 0a0a 2020 2020 2a20 656e   40000..    * en
-00001320: 6469 616e 2028 4f70 7469 6f6e 616c 2920  dian (Optional) 
-00001330: 2d20 4279 7465 206f 7264 6572 3a20 6269  - Byte order: bi
-00001340: 6720 6f72 206c 6974 746c 652e 2044 6566  g or little. Def
-00001350: 6175 6c74 7320 746f 2062 6967 2e0a 0a20  aults to big... 
-00001360: 2020 202a 2077 7269 7465 5f6d 756c 7469     * write_multi
-00001370: 706c 655f 7265 6769 7374 6572 7320 284f  ple_registers (O
-00001380: 7074 696f 6e61 6c29 202d 2057 7269 7465  ptional) - Write
-00001390: 206d 756c 7469 706c 6520 636f 696c 7320   multiple coils 
-000013a0: 6f72 2072 6567 6973 7465 7273 2061 7420  or registers at 
-000013b0: 6120 7469 6d65 2e20 4465 6661 756c 7473  a time. Defaults
-000013c0: 2074 6f20 7472 7565 2e0a 0a20 2020 2020   to true...     
-000013d0: 202a 2049 6620 7772 6974 655f 6d75 6c74   * If write_mult
-000013e0: 6970 6c65 5f72 6567 6973 7465 7273 2069  iple_registers i
-000013f0: 7320 7365 7420 746f 2066 616c 7365 2c20  s set to false, 
-00001400: 6f6e 6c79 2072 6567 6973 7465 7220 7479  only register ty
-00001410: 7065 7320 756e 7369 676e 6564 2073 686f  pes unsigned sho
-00001420: 7274 2028 7569 6e74 3136 2920 616e 6420  rt (uint16) and 
-00001430: 626f 6f6c 6561 6e20 2862 6f6f 6c29 2061  boolean (bool) a
-00001440: 7265 2073 7570 706f 7274 6564 2e20 5468  re supported. Th
-00001450: 6520 6578 6365 7074 696f 6e20 7261 6973  e exception rais
-00001460: 6564 2064 7572 696e 6720 7468 6520 636f  ed during the co
-00001470: 6e66 6967 7572 6520 7072 6f63 6573 732e  nfigure process.
-00001480: 0a0a 2020 2020 2a20 7265 6769 7374 6572  ..    * register
-00001490: 5f6d 6170 2028 4f70 7469 6f6e 616c 2920  _map (Optional) 
-000014a0: 2d20 5265 6769 7374 6572 206d 6170 2063  - Register map c
-000014b0: 7376 206f 6620 756e 6368 616e 6765 6420  sv of unchanged 
-000014c0: 7265 6769 7374 6572 2076 6172 6961 626c  register variabl
-000014d0: 6573 2e20 4465 6661 756c 7473 2074 6f20  es. Defaults to 
-000014e0: 7265 6769 7374 7279 5f63 6f6e 6669 6720  registry_config 
-000014f0: 6373 762e 0a0a 2020 2020 5468 6973 2072  csv...    This r
-00001500: 6570 6f20 7072 6f76 6964 6573 2061 6e20  epo provides an 
-00001510: 6578 616d 706c 6520 636f 6e66 6967 7572  example configur
-00001520: 6174 696f 6e20 696e 2074 6865 2066 696c  ation in the fil
-00001530: 6520 226d 6f64 6275 735f 746b 5f65 7861  e "modbus_tk_exa
-00001540: 6d70 6c65 2e63 6f6e 6669 6722 2e0a 0a20  mple.config"... 
-00001550: 2020 2048 6572 6520 6973 2061 6e20 6578     Here is an ex
-00001560: 616d 706c 6520 6465 7669 6365 2063 6f6e  ample device con
-00001570: 6669 6775 7261 7469 6f6e 2066 696c 653a  figuration file:
-00001580: 0a0a 2020 2020 6060 606a 736f 6e0a 2020  ..    ```json.  
-00001590: 2020 2020 2020 7b0a 2020 2020 2020 2020        {.        
-000015a0: 2264 7269 7665 725f 636f 6e66 6967 223a  "driver_config":
-000015b0: 207b 0a20 2020 2020 2020 2020 2020 2022   {.            "
-000015c0: 6465 7669 6365 5f61 6464 7265 7373 223a  device_address":
-000015d0: 2022 3130 2e31 2e31 2e32 222c 0a20 2020   "10.1.1.2",.   
-000015e0: 2020 2020 2020 2020 2022 706f 7274 223a           "port":
-000015f0: 2022 3530 3230 222c 0a20 2020 2020 2020   "5020",.       
-00001600: 2020 2020 2022 7265 6769 7374 6572 5f6d       "register_m
-00001610: 6170 223a 2022 636f 6e66 6967 3a2f 2f6d  ap": "config://m
-00001620: 6f64 6275 735f 746b 5f74 6573 745f 6d61  odbus_tk_test_ma
-00001630: 702e 6373 7622 0a20 2020 2020 2020 207d  p.csv".        }
-00001640: 2c0a 2020 2020 2020 2020 2264 7269 7665  ,.        "drive
-00001650: 725f 7479 7065 223a 2022 6d6f 6462 7573  r_type": "modbus
-00001660: 5f74 6b22 2c0a 2020 2020 2020 2020 2272  _tk",.        "r
-00001670: 6567 6973 7472 795f 636f 6e66 6967 223a  egistry_config":
-00001680: 2022 636f 6e66 6967 3a2f 2f6d 6f64 6275   "config://modbu
-00001690: 735f 746b 5f74 6573 742e 6373 7622 2c0a  s_tk_test.csv",.
-000016a0: 2020 2020 2020 2020 2269 6e74 6572 7661          "interva
-000016b0: 6c22 3a20 3630 2c0a 2020 2020 2020 2020  l": 60,.        
-000016c0: 2274 696d 657a 6f6e 6522 3a20 2255 5443  "timezone": "UTC
-000016d0: 222c 0a20 2020 2020 2020 2022 6865 6172  ",.        "hear
-000016e0: 745f 6265 6174 5f70 6f69 6e74 223a 2022  t_beat_point": "
-000016f0: 6865 6172 7462 6561 7422 0a20 2020 2020  heartbeat".     
-00001700: 2020 207d 0a20 2020 2060 6060 0a0a 2020     }.    ```..  
-00001710: 2020 4166 7465 7220 6372 6561 7469 6e67    After creating
-00001720: 2061 2064 7269 7665 7220 636f 6e66 6967   a driver config
-00001730: 7572 6174 696f 6e20 6669 6c65 206e 616d  uration file nam
-00001740: 6564 2022 6d6f 6462 7573 5f74 6b5f 6578  ed "modbus_tk_ex
-00001750: 616d 706c 652e 636f 6e66 6967 222c 2061  ample.config", a
-00001760: 6464 2069 7420 746f 2074 6865 2043 6f6e  dd it to the Con
-00001770: 6669 6775 7261 7469 6f6e 2053 746f 7265  figuration Store
-00001780: 3a0a 0a20 2020 2060 6060 7368 656c 6c0a  :..    ```shell.
-00001790: 2020 2020 7663 746c 2063 6f6e 6669 6720      vctl config 
-000017a0: 7374 6f72 6520 706c 6174 666f 726d 2e64  store platform.d
-000017b0: 7269 7665 7220 6465 7669 6365 732f 6d6f  river devices/mo
-000017c0: 6462 7573 746b 206d 6f64 6275 735f 746b  dbustk modbus_tk
-000017d0: 5f65 7861 6d70 6c65 2e63 6f6e 6669 670a  _example.config.
-000017e0: 2020 2020 6060 600a 0a31 2e20 4164 6420      ```..1. Add 
-000017f0: 6120 4d6f 6462 7573 2d54 4b20 5265 6769  a Modbus-TK Regi
-00001800: 7374 6572 204d 6170 2043 5356 2046 696c  ster Map CSV Fil
-00001810: 6520 746f 2074 6865 2050 6c61 7466 6f72  e to the Platfor
-00001820: 6d20 4472 6976 6572 2e0a 0a20 2020 204d  m Driver...    M
-00001830: 6f64 6275 7320 544b 2072 6571 7569 7265  odbus TK require
-00001840: 7320 616e 2061 6464 6974 696f 6e61 6c20  s an additional 
-00001850: 7265 6769 7374 7279 2063 6f6e 6669 6775  registry configu
-00001860: 7261 7469 6f6e 2066 696c 6520 636f 6d70  ration file comp
-00001870: 6172 6564 2074 6f20 7468 6520 7061 7261  ared to the para
-00001880: 6469 676d 206f 6620 6d6f 7374 206f 7468  digm of most oth
-00001890: 6572 2064 7269 7665 7273 2e20 5468 6520  er drivers. The 
-000018a0: 7265 6769 7374 7279 206d 6170 2066 696c  registry map fil
-000018b0: 6520 6973 2061 6e20 616e 616c 6f67 7565  e is an analogue
-000018c0: 2074 6f20 7468 6520 7479 7069 6361 6c20   to the typical 
-000018d0: 7265 6769 7374 7279 2063 6f6e 6669 6775  registry configu
-000018e0: 7261 7469 6f6e 2066 696c 652e 2054 6865  ration file. The
-000018f0: 2072 6567 6973 7472 7920 636f 6e66 6967   registry config
-00001900: 7572 6174 696f 6e20 6669 6c65 2069 7320  uration file is 
-00001910: 6120 7369 6d70 6c65 2066 696c 6520 7768  a simple file wh
-00001920: 6963 6820 6d61 7073 2064 6576 6963 6520  ich maps device 
-00001930: 706f 696e 7420 6e61 6d65 7320 746f 2075  point names to u
-00001940: 7365 7220 7370 6563 6966 6965 6420 706f  ser specified po
-00001950: 696e 7420 6e61 6d65 732e 0a0a 2020 2020  int names...    
-00001960: 5468 6973 2072 6570 6f20 7072 6f76 6964  This repo provid
-00001970: 6573 2061 6e20 6578 616d 706c 6520 636f  es an example co
-00001980: 6e66 6967 7572 6174 696f 6e20 696e 2074  nfiguration in t
-00001990: 6865 2066 696c 6520 226d 6f64 6275 735f  he file "modbus_
-000019a0: 746b 5f74 6573 745f 6d61 702e 6373 7622  tk_test_map.csv"
-000019b0: 2e0a 0a20 2020 2054 6865 2072 6567 6973  ...    The regis
-000019c0: 7472 7920 6d61 7020 6669 6c65 2069 7320  try map file is 
-000019d0: 6120 4353 5620 6669 6c65 2e20 4561 6368  a CSV file. Each
-000019e0: 2072 6f77 2063 6f6e 6669 6775 7265 7320   row configures 
-000019f0: 6120 7265 6769 7374 6572 2064 6566 696e  a register defin
-00001a00: 6974 696f 6e20 6f6e 2074 6865 2064 6576  ition on the dev
-00001a10: 6963 652e 0a0a 2020 2020 5265 6769 7374  ice...    Regist
-00001a20: 6572 204e 616d 6520 2852 6571 7569 7265  er Name (Require
-00001a30: 6429 202d 2054 6865 2066 6965 6c64 206e  d) - The field n
-00001a40: 616d 6520 696e 2074 6865 206d 6f64 6275  ame in the modbu
-00001a50: 7320 636c 6965 6e74 2e20 5468 6973 2066  s client. This f
-00001a60: 6965 6c64 2069 7320 6469 7374 696e 6374  ield is distinct
-00001a70: 2061 6e64 2075 6e63 6861 6e67 6561 626c   and unchangeabl
-00001a80: 652e 0a0a 2020 2020 4164 6472 6573 7320  e...    Address 
-00001a90: 2852 6571 7569 7265 6429 202d 2054 6865  (Required) - The
-00001aa0: 2070 6f69 6e74 e280 9973 206d 6f64 6275   point...s modbu
-00001ab0: 7320 6164 6472 6573 732e 2054 6865 2061  s address. The a
-00001ac0: 6464 7265 7373 696e 6720 6f70 7469 6f6e  ddressing option
-00001ad0: 2069 6e20 7468 6520 6472 6976 6572 2063   in the driver c
-00001ae0: 6f6e 6669 6775 7261 7469 6f6e 2063 6f6e  onfiguration con
-00001af0: 7472 6f6c 7320 7768 6574 6865 7220 7468  trols whether th
-00001b00: 6973 2069 7320 696e 7465 7270 7265 7465  is is interprete
-00001b10: 6420 6173 2061 6e20 6578 6163 7420 6164  d as an exact ad
-00001b20: 6472 6573 7320 6f72 2061 6e20 6f66 6673  dress or an offs
-00001b30: 6574 2e0a 0a20 2020 2054 7970 6520 2852  et...    Type (R
-00001b40: 6571 7569 7265 6429 202d 2054 6865 2070  equired) - The p
-00001b50: 6f69 6e74 e280 9973 2064 6174 6120 7479  oint...s data ty
-00001b60: 7065 3a20 626f 6f6c 2c20 7374 7269 6e67  pe: bool, string
-00001b70: 5b6c 656e 6774 685d 2c20 666c 6f61 742c  [length], float,
-00001b80: 2069 6e74 3136 2c20 696e 7433 322c 2069   int16, int32, i
-00001b90: 6e74 3634 2c20 7569 6e74 3136 2c20 7569  nt64, uint16, ui
-00001ba0: 6e74 3332 2c20 6f72 2075 696e 7436 342e  nt32, or uint64.
-00001bb0: 0a0a 2020 2020 556e 6974 7320 284f 7074  ..    Units (Opt
-00001bc0: 696f 6e61 6c29 202d 2055 7365 6420 666f  ional) - Used fo
-00001bd0: 7220 6d65 7461 6461 7461 2077 6865 6e20  r metadata when 
-00001be0: 6372 6561 7469 6e67 2070 6f69 6e74 2069  creating point i
-00001bf0: 6e66 6f72 6d61 7469 6f6e 206f 6e20 6120  nformation on a 
-00001c00: 6869 7374 6f72 6961 6e2e 2044 6566 6175  historian. Defau
-00001c10: 6c74 2069 7320 616e 2065 6d70 7479 2073  lt is an empty s
-00001c20: 7472 696e 672e 0a0a 2020 2020 5772 6974  tring...    Writ
-00001c30: 6162 6c65 2028 4f70 7469 6f6e 616c 2920  able (Optional) 
-00001c40: 2d20 5452 5545 2f46 414c 5345 2e20 4f6e  - TRUE/FALSE. On
-00001c50: 6c79 2070 6f69 6e74 7320 666f 7220 7768  ly points for wh
-00001c60: 6963 6820 5772 6974 6162 6c65 3d54 5255  ich Writable=TRU
-00001c70: 4520 6361 6e20 6265 2075 7064 6174 6564  E can be updated
-00001c80: 2062 7920 6120 564f 4c54 5452 4f4e 2061   by a VOLTTRON a
-00001c90: 6765 6e74 2e20 4465 6661 756c 7420 6973  gent. Default is
-00001ca0: 2046 414c 5345 2e0a 0a20 2020 2044 6566   FALSE...    Def
-00001cb0: 6175 6c74 2056 616c 7565 2028 4f70 7469  ault Value (Opti
-00001cc0: 6f6e 616c 2920 2d20 5468 6520 706f 696e  onal) - The poin
-00001cd0: 74e2 8099 7320 6465 6661 756c 7420 7661  t...s default va
-00001ce0: 6c75 652e 2049 6620 6974 2069 7320 7265  lue. If it is re
-00001cf0: 7665 7274 6564 2062 7920 616e 2061 6765  verted by an age
-00001d00: 6e74 2c20 6974 2063 6861 6e67 6573 2062  nt, it changes b
-00001d10: 6163 6b20 746f 2074 6869 7320 7661 6c75  ack to this valu
-00001d20: 652e 2049 6620 7468 6973 2076 616c 7565  e. If this value
-00001d30: 2069 7320 6d69 7373 696e 672c 2069 7420   is missing, it 
-00001d40: 7769 6c6c 2072 6576 6572 7420 746f 2074  will revert to t
-00001d50: 6865 206c 6173 7420 6b6e 6f77 6e20 7661  he last known va
-00001d60: 6c75 6520 6e6f 7420 7365 7420 6279 2061  lue not set by a
-00001d70: 6e20 6167 656e 742e 0a0a 2020 2020 5472  n agent...    Tr
-00001d80: 616e 7366 6f72 6d20 284f 7074 696f 6e61  ansform (Optiona
-00001d90: 6c29 202d 2053 6361 6c69 6e67 2061 6c67  l) - Scaling alg
-00001da0: 6f72 6974 686d 3a20 7363 616c 6528 6d75  orithm: scale(mu
-00001db0: 6c74 6970 6c69 6572 292c 2073 6361 6c65  ltiplier), scale
-00001dc0: 5f69 6e74 286d 756c 7469 706c 6965 7229  _int(multiplier)
-00001dd0: 2c20 7363 616c 655f 7265 6728 7265 6769  , scale_reg(regi
-00001de0: 7374 6572 5f6e 616d 6529 2c20 7363 616c  ster_name), scal
-00001df0: 655f 7265 675f 706f 7765 7231 3028 7265  e_reg_power10(re
-00001e00: 6769 7374 6572 5f6e 616d 6529 2c20 7363  gister_name), sc
-00001e10: 616c 655f 6465 6369 6d61 6c5f 696e 745f  ale_decimal_int_
-00001e20: 7369 676e 6564 286d 756c 7469 706c 6965  signed(multiplie
-00001e30: 7229 2c20 6d6f 6431 306b 2872 6576 6572  r), mod10k(rever
-00001e40: 7365 292c 206d 6f64 3130 6b36 3428 7265  se), mod10k64(re
-00001e50: 7665 7273 6529 2c20 6d6f 6431 306b 3438  verse), mod10k48
-00001e60: 2872 6576 6572 6573 2920 6f72 206e 6f6e  (reveres) or non
-00001e70: 652e 2044 6566 6175 6c74 2069 7320 616e  e. Default is an
-00001e80: 2065 6d70 7479 2073 7472 696e 672e 0a0a   empty string...
-00001e90: 2020 2020 5461 626c 6520 284f 7074 696f      Table (Optio
-00001ea0: 6e61 6c29 202d 2053 7461 6e64 6172 6420  nal) - Standard 
-00001eb0: 6d6f 6462 7573 2074 6162 6c65 206e 616d  modbus table nam
-00001ec0: 6520 6465 6669 6e69 6e67 2068 6f77 2069  e defining how i
-00001ed0: 6e66 6f72 6d61 7469 6f6e 2069 7320 7374  nformation is st
-00001ee0: 6f72 6564 2069 6e20 736c 6176 6520 6465  ored in slave de
-00001ef0: 7669 6365 2e20 5468 6572 6520 6172 6520  vice. There are 
-00001f00: 3420 6469 6666 6572 656e 7420 7461 626c  4 different tabl
-00001f10: 6573 3a0a 0a20 2020 2064 6973 6372 6574  es:..    discret
-00001f20: 655f 6f75 7470 7574 5f63 6f69 6c73 3a20  e_output_coils: 
-00001f30: 7265 6164 2f77 7269 7465 2063 6f69 6c20  read/write coil 
-00001f40: 6e75 6d62 6572 7320 312d 3939 3939 0a0a  numbers 1-9999..
-00001f50: 2020 2020 6469 7363 7265 7465 5f69 6e70      discrete_inp
-00001f60: 7574 5f63 6f6e 7461 6374 733a 2072 6561  ut_contacts: rea
-00001f70: 6420 6f6e 6c79 2063 6f69 6c20 6e75 6d62  d only coil numb
-00001f80: 6572 7320 3130 3030 312d 3139 3939 390a  ers 10001-19999.
-00001f90: 0a20 2020 2061 6e61 6c6f 675f 696e 7075  .    analog_inpu
-00001fa0: 745f 7265 6769 7374 6572 733a 2072 6561  t_registers: rea
-00001fb0: 6420 6f6e 6c79 2072 6567 6973 7465 7220  d only register 
-00001fc0: 6e75 6d62 6572 7320 3330 3030 312d 3339  numbers 30001-39
-00001fd0: 3939 390a 0a20 2020 2061 6e61 6c6f 675f  999..    analog_
-00001fe0: 6f75 7470 7574 5f68 6f6c 6469 6e67 5f72  output_holding_r
-00001ff0: 6567 6973 7465 7273 3a20 7265 6164 2f77  egisters: read/w
-00002000: 7269 7465 2072 6567 6973 7465 7220 6e75  rite register nu
-00002010: 6d62 6572 7320 3430 3030 312d 3439 3939  mbers 40001-4999
-00002020: 390a 0a20 2020 2049 6620 7468 6973 2066  9..    If this f
-00002030: 6965 6c64 2069 7320 656d 7074 792c 2074  ield is empty, t
-00002040: 6865 206d 6f64 6275 7320 7461 626c 6520  he modbus table 
-00002050: 7769 6c6c 2062 6520 6465 6669 6e65 6420  will be defined 
-00002060: 6279 2074 7970 6520 616e 6420 7772 6974  by type and writ
-00002070: 6162 6c65 2066 6965 6c64 732e 2042 7920  able fields. By 
-00002080: 7468 6174 2c20 7768 656e 2075 7365 7220  that, when user 
-00002090: 7365 7473 2072 6561 6420 6f6e 6c79 2066  sets read only f
-000020a0: 6f72 2072 6561 642f 7772 6974 6520 636f  or read/write co
-000020b0: 696c 732f 7265 6769 7374 6572 7320 6f72  ils/registers or
-000020c0: 2073 6574 7320 7265 6164 2f77 7269 7465   sets read/write
-000020d0: 2066 6f72 2072 6561 6420 6f6e 6c79 2063   for read only c
-000020e0: 6f69 6c73 2f72 6567 6973 7465 7273 2c20  oils/registers, 
-000020f0: 6974 2077 696c 6c20 7365 6c65 6374 2077  it will select w
-00002100: 726f 6e67 2074 6162 6c65 2c20 616e 6420  rong table, and 
-00002110: 7468 6572 6566 6f72 6520 7261 6973 6520  therefore raise 
-00002120: 6578 6365 7074 696f 6e2e 0a0a 2020 2020  exception...    
-00002130: 4d69 7865 6420 456e 6469 616e 2028 4f70  Mixed Endian (Op
-00002140: 7469 6f6e 616c 2920 2d20 5452 5545 2f46  tional) - TRUE/F
-00002150: 414c 5345 2e20 4966 204d 6978 6564 2045  ALSE. If Mixed E
-00002160: 6e64 6961 6e20 6973 2073 6574 2074 6f20  ndian is set to 
-00002170: 5452 5545 2c20 7468 6520 6f72 6465 7220  TRUE, the order 
-00002180: 6f66 2074 6865 204d 6f64 6275 7320 7265  of the Modbus re
-00002190: 6769 7374 6572 7320 7769 6c6c 2062 6520  gisters will be 
-000021a0: 7265 7665 7273 6564 2062 6566 6f72 6520  reversed before 
-000021b0: 7061 7273 696e 6720 7468 6520 7661 6c75  parsing the valu
-000021c0: 6520 6f72 2077 7269 7469 6e67 2069 7420  e or writing it 
-000021d0: 6f75 7420 746f 2074 6865 2064 6576 6963  out to the devic
-000021e0: 652e 2042 7920 7365 7474 696e 6720 6d69  e. By setting mi
-000021f0: 7865 6420 656e 6469 616e 2c20 7472 616e  xed endian, tran
-00002200: 7366 6f72 6d20 6d75 7374 2062 6520 4e6f  sform must be No
-00002210: 6e65 2028 6e6f 206f 7029 2e20 4465 6661  ne (no op). Defa
-00002220: 756c 7473 2074 6f20 4641 4c53 452e 0a0a  ults to FALSE...
-00002230: 2020 2020 4465 7363 7269 7074 696f 6e20      Description 
-00002240: 284f 7074 696f 6e61 6c29 202d 2041 6464  (Optional) - Add
-00002250: 6974 696f 6e61 6c20 696e 666f 726d 6174  itional informat
-00002260: 696f 6e20 6162 6f75 7420 7468 6520 706f  ion about the po
-00002270: 696e 742e 2044 6566 6175 6c74 2069 7320  int. Default is 
-00002280: 616e 2065 6d70 7479 2073 7472 696e 672e  an empty string.
-00002290: 0a0a 2020 2020 4865 7265 2069 7320 6120  ..    Here is a 
-000022a0: 7361 6d70 6c65 204d 6f64 6275 732d 544b  sample Modbus-TK
-000022b0: 2072 6567 6973 7472 7920 6d61 703a 0a0a   registry map:..
-000022c0: 2020 2020 6060 6063 7376 0a20 2020 2052      ```csv.    R
-000022d0: 6567 6973 7465 7220 4e61 6d65 2c41 6464  egister Name,Add
-000022e0: 7265 7373 2c54 7970 652c 556e 6974 732c  ress,Type,Units,
-000022f0: 5772 6974 6162 6c65 2c44 6566 6175 6c74  Writable,Default
-00002300: 2056 616c 7565 2c54 7261 6e73 666f 726d   Value,Transform
-00002310: 2c54 6162 6c65 0a20 2020 2075 6e73 6967  ,Table.    unsig
-00002320: 6e65 645f 7368 6f72 742c 302c 7569 6e74  ned_short,0,uint
-00002330: 3136 2c4e 6f6e 652c 5452 5545 2c30 2c73  16,None,TRUE,0,s
-00002340: 6361 6c65 2831 3029 2c61 6e61 6c6f 675f  cale(10),analog_
-00002350: 6f75 7470 7574 5f68 6f6c 6469 6e67 5f72  output_holding_r
-00002360: 6567 6973 7465 7273 0a20 2020 2075 6e73  egisters.    uns
-00002370: 6967 6e65 645f 696e 742c 312c 7569 6e74  igned_int,1,uint
-00002380: 3332 2c4e 6f6e 652c 5452 5545 2c30 2c73  32,None,TRUE,0,s
-00002390: 6361 6c65 2831 3029 2c61 6e61 6c6f 675f  cale(10),analog_
-000023a0: 6f75 7470 7574 5f68 6f6c 6469 6e67 5f72  output_holding_r
-000023b0: 6567 6973 7465 7273 0a20 2020 2075 6e73  egisters.    uns
-000023c0: 6967 6e65 645f 6c6f 6e67 2c33 2c75 696e  igned_long,3,uin
-000023d0: 7436 342c 4e6f 6e65 2c54 5255 452c 302c  t64,None,TRUE,0,
-000023e0: 7363 616c 6528 3130 292c 616e 616c 6f67  scale(10),analog
-000023f0: 5f6f 7574 7075 745f 686f 6c64 696e 675f  _output_holding_
-00002400: 7265 6769 7374 6572 730a 2020 2020 7361  registers.    sa
-00002410: 6d70 6c65 5f73 686f 7274 2c37 2c69 6e74  mple_short,7,int
-00002420: 3136 2c4e 6f6e 652c 5452 5545 2c30 2c73  16,None,TRUE,0,s
-00002430: 6361 6c65 2831 3029 2c61 6e61 6c6f 675f  cale(10),analog_
-00002440: 6f75 7470 7574 5f68 6f6c 6469 6e67 5f72  output_holding_r
-00002450: 6567 6973 7465 7273 0a20 2020 2073 616d  egisters.    sam
-00002460: 706c 655f 696e 742c 382c 696e 7433 322c  ple_int,8,int32,
-00002470: 4e6f 6e65 2c54 5255 452c 302c 7363 616c  None,TRUE,0,scal
-00002480: 6528 3130 292c 616e 616c 6f67 5f6f 7574  e(10),analog_out
-00002490: 7075 745f 686f 6c64 696e 675f 7265 6769  put_holding_regi
-000024a0: 7374 6572 730a 2020 2020 7361 6d70 6c65  sters.    sample
-000024b0: 5f66 6c6f 6174 2c31 302c 666c 6f61 742c  _float,10,float,
-000024c0: 4e6f 6e65 2c54 5255 452c 302e 302c 7363  None,TRUE,0.0,sc
-000024d0: 616c 6528 3130 292c 616e 616c 6f67 5f6f  ale(10),analog_o
-000024e0: 7574 7075 745f 686f 6c64 696e 675f 7265  utput_holding_re
-000024f0: 6769 7374 6572 730a 2020 2020 7361 6d70  gisters.    samp
-00002500: 6c65 5f6c 6f6e 672c 3132 2c69 6e74 3634  le_long,12,int64
-00002510: 2c4e 6f6e 652c 5452 5545 2c30 2c73 6361  ,None,TRUE,0,sca
-00002520: 6c65 2831 3029 2c61 6e61 6c6f 675f 6f75  le(10),analog_ou
-00002530: 7470 7574 5f68 6f6c 6469 6e67 5f72 6567  tput_holding_reg
-00002540: 6973 7465 7273 0a20 2020 2073 616d 706c  isters.    sampl
-00002550: 655f 626f 6f6c 2c31 362c 626f 6f6c 2c4e  e_bool,16,bool,N
-00002560: 6f6e 652c 5452 5545 2c46 616c 7365 2c2c  one,TRUE,False,,
-00002570: 616e 616c 6f67 5f6f 7574 7075 745f 686f  analog_output_ho
-00002580: 6c64 696e 675f 7265 6769 7374 6572 730a  lding_registers.
-00002590: 2020 2020 7361 6d70 6c65 5f73 7472 2c31      sample_str,1
-000025a0: 372c 7374 7269 6e67 5b31 325d 2c4e 6f6e  7,string[12],Non
-000025b0: 652c 5452 5545 2c68 656c 6c6f 2077 6f72  e,TRUE,hello wor
-000025c0: 6c64 212c 2c61 6e61 6c6f 675f 6f75 7470  ld!,,analog_outp
-000025d0: 7574 5f68 6f6c 6469 6e67 5f72 6567 6973  ut_holding_regis
-000025e0: 7465 7273 0a20 2020 2060 6060 0a0a 2020  ters.    ```..  
-000025f0: 2020 4166 7465 7220 6372 6561 7469 6e67    After creating
-00002600: 2061 2072 6567 6973 7472 7920 6d61 7020   a registry map 
-00002610: 6e61 6d65 6420 226d 6f64 6275 735f 746b  named "modbus_tk
-00002620: 5f74 6573 745f 6d61 702e 6373 7622 2c20  _test_map.csv", 
-00002630: 6164 6420 6974 2074 6f20 7468 6520 436f  add it to the Co
-00002640: 6e66 6967 7572 6174 696f 6e20 5374 6f72  nfiguration Stor
-00002650: 653a 0a0a 2020 2020 6060 6073 6865 6c6c  e:..    ```shell
-00002660: 0a20 2020 2076 6374 6c20 636f 6e66 6967  .    vctl config
-00002670: 2073 746f 7265 2070 6c61 7466 6f72 6d2e   store platform.
-00002680: 6472 6976 6572 206d 6f64 6275 735f 746b  driver modbus_tk
-00002690: 5f74 6573 745f 6d61 702e 6373 7620 6d6f  _test_map.csv mo
-000026a0: 6462 7573 5f74 6b5f 7465 7374 5f6d 6170  dbus_tk_test_map
-000026b0: 2e63 7376 202d 2d63 7376 0a20 2020 2060  .csv --csv.    `
-000026c0: 6060 0a0a 312e 2041 6464 2061 2072 6567  ``..1. Add a reg
-000026d0: 6973 7472 7920 636f 6e66 6967 7572 6174  istry configurat
-000026e0: 696f 6e20 746f 2074 6865 2050 6c61 7466  ion to the Platf
-000026f0: 6f72 6d44 7269 7665 722e 0a0a 2020 2020  ormDriver...    
-00002700: 5468 6520 7265 6769 7374 7279 2063 6f6e  The registry con
-00002710: 6669 6775 7261 7469 6f6e 2066 696c 6520  figuration file 
-00002720: 6973 2061 2043 5356 2066 696c 652e 2045  is a CSV file. E
-00002730: 6163 6820 726f 7720 636f 6e66 6967 7572  ach row configur
-00002740: 6573 2061 2070 6f69 6e74 206f 6e20 7468  es a point on th
-00002750: 6520 6465 7669 6365 2e0a 0a20 2020 2020  e device...     
-00002760: 2020 2056 6f6c 7474 726f 6e20 506f 696e     Volttron Poin
-00002770: 7420 4e61 6d65 2028 5265 7175 6972 6564  t Name (Required
-00002780: 2920 2d20 5468 6520 6e61 6d65 2062 7920  ) - The name by 
-00002790: 7768 6963 6820 7468 6520 706c 6174 666f  which the platfo
-000027a0: 726d 2061 6e64 2061 6765 6e74 7320 7265  rm and agents re
-000027b0: 6665 7220 746f 2074 6865 2070 6f69 6e74  fer to the point
-000027c0: 2e20 466f 7220 696e 7374 616e 6365 2c20  . For instance, 
-000027d0: 6966 2074 6865 2056 6f6c 7474 726f 6e20  if the Volttron 
-000027e0: 506f 696e 7420 4e61 6d65 2069 7320 4865  Point Name is He
-000027f0: 6174 4361 6c6c 312c 2074 6865 6e20 616e  atCall1, then an
-00002800: 2061 6765 6e74 2077 6f75 6c64 2075 7365   agent would use
-00002810: 206d 795f 6361 6d70 7573 2f62 7569 6c64   my_campus/build
-00002820: 696e 6732 2f68 7661 6331 2f48 6561 7443  ing2/hvac1/HeatC
-00002830: 616c 6c31 2074 6f20 7265 6665 7220 746f  all1 to refer to
-00002840: 2074 6865 2070 6f69 6e74 2077 6865 6e20   the point when 
-00002850: 7573 696e 6720 7468 6520 5250 4320 696e  using the RPC in
-00002860: 7465 7266 6163 6520 6f66 2074 6865 2061  terface of the a
-00002870: 6374 7561 746f 7220 6167 656e 742e 0a0a  ctuator agent...
-00002880: 2020 2020 2020 2020 5265 6769 7374 6572          Register
-00002890: 204e 616d 6520 2852 6571 7569 7265 6429   Name (Required)
-000028a0: 202d 2054 6865 2066 6965 6c64 206e 616d   - The field nam
-000028b0: 6520 696e 2074 6865 206d 6f64 6275 7320  e in the modbus 
-000028c0: 636c 6965 6e74 2e20 4974 206d 7573 7420  client. It must 
-000028d0: 6265 206d 6174 6368 6564 2077 6974 6820  be matched with 
-000028e0: 7468 6520 6669 656c 6420 6e61 6d65 2066  the field name f
-000028f0: 726f 6d20 7265 6769 7374 6572 5f6d 6170  rom register_map
-00002900: 2e0a 0a20 2020 2041 6e79 2061 6464 6974  ...    Any addit
-00002910: 696f 6e61 6c20 636f 6c75 6d6e 7320 7769  ional columns wi
-00002920: 6c6c 206f 7665 7272 6964 6520 7468 6520  ll override the 
-00002930: 6578 6973 7465 6420 6669 656c 6473 2066  existed fields f
-00002940: 726f 6d20 7265 6769 7374 6572 5f6d 6170  rom register_map
-00002950: 2e0a 0a20 2020 2048 6572 6520 6973 2061  ...    Here is a
-00002960: 2073 616d 706c 6520 4d6f 6462 7573 2d54   sample Modbus-T
-00002970: 4b20 7265 6769 7374 7279 2063 6f6e 6669  K registry confi
-00002980: 6775 7261 7469 6f6e 2077 6974 6820 6465  guration with de
-00002990: 6669 6e65 6420 7265 6769 7374 6572 5f6d  fined register_m
-000029a0: 6170 3a0a 0a20 2020 2060 6060 6373 760a  ap:..    ```csv.
-000029b0: 2020 2020 566f 6c74 7472 6f6e 2050 6f69      Volttron Poi
-000029c0: 6e74 204e 616d 652c 5265 6769 7374 6572  nt Name,Register
-000029d0: 204e 616d 650a 2020 2020 756e 7369 676e   Name.    unsign
-000029e0: 6564 2073 686f 7274 2c75 6e73 6967 6e65  ed short,unsigne
-000029f0: 645f 7368 6f72 740a 2020 2020 756e 7369  d_short.    unsi
-00002a00: 676e 6564 2069 6e74 2c75 6e73 6967 6e65  gned int,unsigne
-00002a10: 645f 696e 740a 2020 2020 756e 7369 676e  d_int.    unsign
-00002a20: 6564 206c 6f6e 672c 756e 7369 676e 6564  ed long,unsigned
-00002a30: 5f6c 6f6e 670a 2020 2020 7361 6d70 6c65  _long.    sample
-00002a40: 2073 686f 7274 2c73 616d 706c 655f 7368   short,sample_sh
-00002a50: 6f72 740a 2020 2020 7361 6d70 6c65 2069  ort.    sample i
-00002a60: 6e74 2c73 616d 706c 655f 696e 740a 2020  nt,sample_int.  
-00002a70: 2020 7361 6d70 6c65 2066 6c6f 6174 2c73    sample float,s
-00002a80: 616d 706c 655f 666c 6f61 740a 2020 2020  ample_float.    
-00002a90: 7361 6d70 6c65 206c 6f6e 672c 7361 6d70  sample long,samp
-00002aa0: 6c65 5f6c 6f6e 670a 2020 2020 7361 6d70  le_long.    samp
-00002ab0: 6c65 2062 6f6f 6c2c 7361 6d70 6c65 5f62  le bool,sample_b
-00002ac0: 6f6f 6c0a 2020 2020 7361 6d70 6c65 2073  ool.    sample s
-00002ad0: 7472 2c73 616d 706c 655f 7374 720a 2020  tr,sample_str.  
-00002ae0: 2020 6060 600a 0a20 2020 2041 6674 6572    ```..    After
-00002af0: 2063 7265 6174 696e 6720 6120 7265 6769   creating a regi
-00002b00: 7374 7279 206d 6170 206e 616d 6564 2022  stry map named "
-00002b10: 6d6f 6462 7573 5f74 6b5f 7465 7374 2e63  modbus_tk_test.c
-00002b20: 7376 222c 2061 6464 2069 7420 746f 2074  sv", add it to t
-00002b30: 6865 2043 6f6e 6669 6775 7261 7469 6f6e  he Configuration
-00002b40: 2053 746f 7265 3a0a 0a20 2020 2060 6060   Store:..    ```
-00002b50: 7368 656c 6c0a 2020 2020 7663 746c 2063  shell.    vctl c
-00002b60: 6f6e 6669 6720 7374 6f72 6520 706c 6174  onfig store plat
-00002b70: 666f 726d 2e64 7269 7665 7220 6d6f 6462  form.driver modb
-00002b80: 7573 5f74 6b5f 7465 7374 2e63 7376 206d  us_tk_test.csv m
-00002b90: 6f64 6275 735f 746b 5f74 6573 742e 6373  odbus_tk_test.cs
-00002ba0: 7620 2d2d 6373 760a 2020 2020 6060 600a  v --csv.    ```.
-00002bb0: 0a31 2e20 4f62 7365 7276 6520 4461 7461  .1. Observe Data
-00002bc0: 0a0a 2020 2020 546f 2073 6565 2064 6174  ..    To see dat
-00002bd0: 6120 6265 696e 6720 7075 626c 6973 6865  a being publishe
-00002be0: 6420 746f 2074 6865 2062 7573 2c20 696e  d to the bus, in
-00002bf0: 7374 616c 6c20 6120 5b4c 6973 7465 6e65  stall a [Listene
-00002c00: 7220 4167 656e 745d 2868 7474 7073 3a2f  r Agent](https:/
-00002c10: 2f70 7970 692e 6f72 672f 7072 6f6a 6563  /pypi.org/projec
-00002c20: 742f 766f 6c74 7472 6f6e 2d6c 6973 7465  t/volttron-liste
-00002c30: 6e65 722f 293a 0a0a 2020 2020 6060 600a  ner/):..    ```.
-00002c40: 2020 2020 7663 746c 2069 6e73 7461 6c6c      vctl install
-00002c50: 2076 6f6c 7474 726f 6e2d 6c69 7374 656e   volttron-listen
-00002c60: 6572 202d 2d73 7461 7274 0a20 2020 2060  er --start.    `
-00002c70: 6060 0a0a 2020 2020 4f6e 6365 2069 6e73  ``..    Once ins
-00002c80: 7461 6c6c 6564 2c20 796f 7520 7368 6f75  talled, you shou
-00002c90: 6c64 2073 6565 2074 6865 2064 6174 6120  ld see the data 
-00002ca0: 6265 696e 6720 7075 626c 6973 6865 6420  being published 
-00002cb0: 6279 2076 6965 7769 6e67 2074 6865 2056  by viewing the V
-00002cc0: 6f6c 7474 726f 6e20 6c6f 6773 2066 696c  olttron logs fil
-00002cd0: 6520 7468 6174 2077 6173 2063 7265 6174  e that was creat
-00002ce0: 6564 2069 6e20 7374 6570 2032 2e0a 2020  ed in step 2..  
-00002cf0: 2020 546f 2077 6174 6368 2074 6865 206c    To watch the l
-00002d00: 6f67 732c 206f 7065 6e20 6120 7365 7061  ogs, open a sepa
-00002d10: 7261 7465 2074 6572 6d69 6e61 6c20 616e  rate terminal an
-00002d20: 6420 7275 6e20 7468 6520 666f 6c6c 6f77  d run the follow
-00002d30: 696e 6720 636f 6d6d 616e 643a 0a0a 2020  ing command:..  
-00002d40: 2020 6060 600a 2020 2020 7461 696c 202d    ```.    tail -
-00002d50: 6620 3c70 6174 6820 746f 2066 6f6c 6465  f <path to folde
-00002d60: 7220 636f 6e74 6169 6e69 6e67 2076 6f6c  r containing vol
-00002d70: 7474 726f 6e2e 6c6f 673e 2f76 6f6c 7474  ttron.log>/voltt
-00002d80: 726f 6e2e 6c6f 670a 2020 2020 6060 600a  ron.log.    ```.
-00002d90: 0a23 204d 6f64 6275 732d 544b 2043 6f6e  .# Modbus-TK Con
-00002da0: 6669 6720 436f 6d6d 616e 6420 546f 6f6c  fig Command Tool
-00002db0: 0a0a 6063 6f6e 6669 675f 636d 642e 7079  ..`config_cmd.py
-00002dc0: 6020 6973 2061 2063 6f6d 6d61 6e64 2d6c  ` is a command-l
-00002dd0: 696e 6520 746f 6f6c 2066 6f72 2063 7265  ine tool for cre
-00002de0: 6174 696e 6720 616e 6420 6d61 696e 7461  ating and mainta
-00002df0: 696e 696e 6720 564f 4c54 5452 4f4e 2064  ining VOLTTRON d
-00002e00: 7269 7665 7220 636f 6e66 6967 7572 6174  river configurat
-00002e10: 696f 6e73 2e20 5468 6520 746f 6f6c 2072  ions. The tool r
-00002e20: 756e 7320 6672 6f6d 2074 6865 2063 6f6d  uns from the com
-00002e30: 6d61 6e64 206c 696e 653a 0a0a 636f 6e66  mand line:..conf
-00002e40: 6967 5f63 6d64 2e70 7920 7375 7070 6f72  ig_cmd.py suppor
-00002e50: 7473 2074 6865 2066 6f6c 6c6f 7769 6e67  ts the following
-00002e60: 2063 6f6d 6d61 6e64 733a 0a0a 2a20 6865   commands:..* he
-00002e70: 6c70 202d 204c 6973 7420 616c 6c20 636f  lp - List all co
-00002e80: 6d6d 616e 6473 2e0a 0a2a 2071 7569 7420  mmands...* quit 
-00002e90: 2d20 5175 6974 2074 6865 2063 6f6d 6d61  - Quit the comma
-00002ea0: 6e64 2d6c 696e 6520 746f 6f6c 2e0a 0a2a  nd-line tool...*
-00002eb0: 206c 6973 745f 6469 7265 6374 6f72 6965   list_directorie
-00002ec0: 7320 2d20 4c69 7374 2061 6c6c 2073 6574  s - List all set
-00002ed0: 7570 2064 6972 6563 746f 7269 6573 2c20  up directories, 
-00002ee0: 7769 7468 2061 6e20 6f70 7469 6f6e 2074  with an option t
-00002ef0: 6f20 6564 6974 2074 6865 6972 2070 6174  o edit their pat
-00002f00: 6873 2e0a 0a0a 4279 2064 6566 6175 6c74  hs....By default
-00002f10: 2c20 616c 6c20 6469 7265 6374 6f72 6965  , all directorie
-00002f20: 7320 6172 6520 696e 2074 6869 7320 7265  s are in this re
-00002f30: 706f 2061 7420 7468 6520 666f 6c6c 6f77  po at the follow
-00002f40: 696e 6720 666f 6c64 6572 3a20 766f 6c74  ing folder: volt
-00002f50: 7472 6f6e 2f64 7269 7665 722f 696e 7465  tron/driver/inte
-00002f60: 7266 6163 6573 2f6d 6f64 6275 735f 746b  rfaces/modbus_tk
-00002f70: 2f75 7469 6c73 2f6d 6170 732e 0a0a 4974  /utils/maps...It
-00002f80: 2069 7320 696d 706f 7274 616e 7420 746f   is important to
-00002f90: 2075 7365 2074 6865 2063 6f72 7265 6374   use the correct
-00002fa0: 2064 6972 6563 746f 7269 6573 2077 6865   directories whe
-00002fb0: 6e20 6164 6469 6e67 2f65 6469 7469 6e67  n adding/editing
-00002fc0: 2064 6576 6963 6520 7479 7065 7320 616e   device types an
-00002fd0: 6420 6472 6976 6572 2063 6f6e 6669 6773  d driver configs
-00002fe0: 2c20 616e 6420 7768 656e 206c 6f61 6469  , and when loadi
-00002ff0: 6e67 2063 6f6e 6669 6775 7261 7469 6f6e  ng configuration
-00003000: 7320 696e 746f 2056 4f4c 5454 524f 4e2e  s into VOLTTRON.
-00003010: 0a0a 2a20 6d61 705f 6469 723a 2064 6972  ..* map_dir: dir
-00003020: 6563 746f 7279 2069 6e20 7768 6963 6820  ectory in which 
-00003030: 6d61 7073 2e79 616d 6c20 6973 2073 746f  maps.yaml is sto
-00003040: 7265 642e 0a0a 2a20 636f 6e66 6967 5f64  red...* config_d
-00003050: 6972 3a20 6469 7265 6374 6f72 7920 696e  ir: directory in
-00003060: 2077 6869 6368 2064 7269 7665 7220 636f   which driver co
-00003070: 6e66 6967 2066 696c 6573 2061 7265 2073  nfig files are s
-00003080: 746f 7265 642e 0a0a 2a20 6373 765f 6469  tored...* csv_di
-00003090: 723a 2064 6972 6563 746f 7279 2069 6e20  r: directory in 
-000030a0: 7768 6963 6820 7265 6769 7374 7279 2063  which registry c
-000030b0: 6f6e 6669 6720 4353 5620 6669 6c65 7320  onfig CSV files 
-000030c0: 6172 6520 7374 6f72 6564 2e0a 0a2a 2065  are stored...* e
-000030d0: 6469 745f 6469 7265 6374 6f72 6965 7320  dit_directories 
-000030e0: 2d20 4164 642f 4564 6974 206d 6170 2064  - Add/Edit map d
-000030f0: 6972 6563 746f 7279 2c20 6472 6976 6572  irectory, driver
-00003100: 2063 6f6e 6669 6720 6469 7265 6374 6f72   config director
-00003110: 792c 2061 6e64 2f6f 7220 4353 5620 636f  y, and/or CSV co
-00003120: 6e66 6967 2064 6972 6563 746f 7279 2e20  nfig directory. 
-00003130: 5072 6573 7320 3c45 6e74 6572 3e20 6966  Press <Enter> if
-00003140: 206e 6f20 6368 616e 6765 2069 7320 6e65   no change is ne
-00003150: 6564 6564 2e20 4578 6974 7320 6966 2074  eded. Exits if t
-00003160: 6865 2064 6972 6563 746f 7279 2064 6f65  he directory doe
-00003170: 7320 6e6f 7420 6578 6973 742e 0a0a 2a20  s not exist...* 
-00003180: 6c69 7374 5f64 6576 6963 655f 7479 7065  list_device_type
-00003190: 5f64 6573 6372 6970 7469 6f6e 202d 204c  _description - L
-000031a0: 6973 7420 616c 6c20 6465 7669 6365 2074  ist all device t
-000031b0: 7970 6520 6465 7363 7269 7074 696f 6e73  ype descriptions
-000031c0: 2069 6e20 6d61 7073 2e79 616d 6c2e 204f   in maps.yaml. O
-000031d0: 7074 696f 6e20 746f 2065 6469 7420 6465  ption to edit de
-000031e0: 7669 6365 2074 7970 6520 6465 7363 7269  vice type descri
-000031f0: 7074 696f 6e73 2e0a 0a2a 206c 6973 745f  ptions...* list_
-00003200: 616c 6c5f 6465 7669 6365 5f74 7970 6573  all_device_types
-00003210: 202d 204c 6973 7420 616c 6c20 6465 7669   - List all devi
-00003220: 6365 2074 7970 6520 696e 666f 726d 6174  ce type informat
-00003230: 696f 6e20 696e 206d 6170 732e 7961 6d6c  ion in maps.yaml
-00003240: 2e20 4f70 7469 6f6e 2074 6f20 6164 6420  . Option to add 
-00003250: 6d6f 7265 2064 6576 6963 6520 7479 7065  more device type
-00003260: 732e 0a0a 2a20 6465 7669 6365 5f74 7970  s...* device_typ
-00003270: 6520 2d20 4c69 7374 2069 6e66 6f72 6d61  e - List informa
-00003280: 7469 6f6e 2066 6f72 2061 2073 656c 6563  tion for a selec
-00003290: 7465 6420 6465 7669 6365 2074 7970 652e  ted device type.
-000032a0: 204f 7074 696f 6e20 746f 2073 656c 6563   Option to selec
-000032b0: 7420 616e 6f74 6865 7220 6465 7669 6365  t another device
-000032c0: 2074 7970 652e 0a0a 2a20 6164 645f 6465   type...* add_de
-000032d0: 7669 6365 5f74 7970 6520 2d20 4164 6420  vice_type - Add 
-000032e0: 6120 6465 7669 6365 2074 7970 6520 746f  a device type to
-000032f0: 206d 6170 732e 7961 6d6c 2e20 4f70 7469   maps.yaml. Opti
-00003300: 6f6e 2074 6f20 6164 6420 6d6f 7265 2074  on to add more t
-00003310: 6861 6e20 6f6e 6520 6465 7669 6365 2074  han one device t
-00003320: 7970 652e 2045 6163 6820 6465 7669 6365  ype. Each device
-00003330: 2074 7970 6520 696e 636c 7564 6573 2069   type includes i
-00003340: 7473 206e 616d 652c 2043 5356 2066 696c  ts name, CSV fil
-00003350: 652c 2064 6573 6372 6970 7469 6f6e 2c20  e, description, 
-00003360: 6164 6472 6573 7369 6e67 2c20 616e 6420  addressing, and 
-00003370: 656e 6469 616e 2c20 6173 2065 7870 6c61  endian, as expla
-00003380: 696e 6564 2069 6e20 4d4f 4442 5553 2d54  ined in MODBUS-T
-00003390: 4b20 4472 6976 6572 204d 6170 732e 2049  K Driver Maps. I
-000033a0: 6620 616e 2069 6e76 616c 6964 2076 616c  f an invalid val
-000033b0: 7565 2069 7320 656e 7465 7265 6420 666f  ue is entered fo
-000033c0: 7220 6164 6472 6573 7369 6e67 206f 7220  r addressing or 
-000033d0: 656e 6469 616e 2c20 7468 6520 6465 6661  endian, the defa
-000033e0: 756c 7420 7661 6c75 6520 6973 2075 7365  ult value is use
-000033f0: 6420 696e 7374 6561 642e 0a0a 2a65 6469  d instead...*edi
-00003400: 745f 6465 7669 6365 5f74 7970 6520 2d20  t_device_type - 
-00003410: 4564 6974 2061 6e20 6578 6973 7469 6e67  Edit an existing
-00003420: 2064 6576 6963 6520 7479 7065 2e20 4966   device type. If
-00003430: 2061 6e20 696e 7661 6c69 6420 7661 6c75   an invalid valu
-00003440: 6520 6973 2065 6e74 6572 6564 2066 6f72  e is entered for
-00003450: 2061 6464 7265 7373 696e 6720 6f72 2065   addressing or e
-00003460: 6e64 6961 6e2c 2074 6865 2070 7265 7669  ndian, the previ
-00003470: 6f75 7320 7661 6c75 6520 6973 206c 6566  ous value is lef
-00003480: 7420 756e 6368 616e 6765 642e 0a0a 2a20  t unchanged...* 
-00003490: 6c69 7374 5f64 7269 7665 7273 202d 204c  list_drivers - L
-000034a0: 6973 7420 616c 6c20 6472 6976 6572 2063  ist all driver c
-000034b0: 6f6e 6669 6720 6e61 6d65 7320 696e 2063  onfig names in c
-000034c0: 6f6e 6669 675f 6469 722e 0a0a 2a20 6472  onfig_dir...* dr
-000034d0: 6976 6572 5f63 6f6e 6669 6720 3c64 7269  iver_config <dri
-000034e0: 7665 725f 6e61 6d65 3e20 2d20 4765 7420  ver_name> - Get 
-000034f0: 6120 6472 6976 6572 2063 6f6e 6669 6720  a driver config 
-00003500: 6672 6f6d 2063 6f6e 6669 675f 6469 722e  from config_dir.
-00003510: 204f 7074 696f 6e20 746f 2073 656c 6563   Option to selec
-00003520: 7420 7468 6520 6472 6976 6572 2069 6620  t the driver if 
-00003530: 6e6f 2064 7269 7665 7220 6973 2066 6f75  no driver is fou
-00003540: 6e64 2077 6974 6820 7468 6174 206e 616d  nd with that nam
-00003550: 652e 0a0a 2a20 6164 645f 6472 6976 6572  e...* add_driver
-00003560: 5f63 6f6e 6669 6720 3c64 7269 7665 725f  _config <driver_
-00003570: 6e61 6d65 3e20 2d20 4164 642f 4564 6974  name> - Add/Edit
-00003580: 203c 636f 6e66 6967 5f64 6972 3e2f 3c64   <config_dir>/<d
-00003590: 7269 7665 7220 6e61 6d65 3e2e 636f 6e66  river name>.conf
-000035a0: 6967 2e20 4f70 7469 6f6e 2074 6f20 7365  ig. Option to se
-000035b0: 6c65 6374 2074 6865 2064 7269 7665 7220  lect the driver 
-000035c0: 6966 206e 6f20 6472 6976 6572 2069 7320  if no driver is 
-000035d0: 666f 756e 6420 7769 7468 2074 6861 7420  found with that 
-000035e0: 6e61 6d65 2e20 5072 6573 7320 3c45 6e74  name. Press <Ent
-000035f0: 6572 3e20 746f 2065 7869 742e 0a0a 2a20  er> to exit...* 
-00003600: 6c6f 6164 5f76 6f6c 7474 726f 6e20 2d20  load_volttron - 
-00003610: 4c6f 6164 2061 2064 7269 7665 7220 636f  Load a driver co
-00003620: 6e66 6967 2061 6e64 2043 5356 2069 6e74  nfig and CSV int
-00003630: 6f20 564f 4c54 5452 4f4e 2e20 4f70 7469  o VOLTTRON. Opti
-00003640: 6f6e 2074 6f20 6164 6420 7468 6520 636f  on to add the co
-00003650: 6e66 6967 206f 7220 4353 5620 6669 6c65  nfig or CSV file
-00003660: 2074 6f20 636f 6e66 6967 5f64 6972 206f   to config_dir o
-00003670: 7220 746f 2063 7376 5f64 6972 2e20 564f  r to csv_dir. VO
-00003680: 4c54 5452 4f4e 206d 7573 7420 6265 2072  LTTRON must be r
-00003690: 756e 6e69 6e67 2077 6865 6e20 7468 6973  unning when this
-000036a0: 2063 6f6d 6d61 6e64 2069 7320 7573 6564   command is used
-000036b0: 2e0a 0a2a 2064 656c 6574 655f 766f 6c74  ...* delete_volt
-000036c0: 7472 6f6e 5f63 6f6e 6669 6720 2d20 4465  tron_config - De
-000036d0: 6c65 7465 2061 2064 7269 7665 7220 636f  lete a driver co
-000036e0: 6e66 6967 2066 726f 6d20 564f 4c54 5452  nfig from VOLTTR
-000036f0: 4f4e 2e20 564f 4c54 5452 4f4e 206d 7573  ON. VOLTTRON mus
-00003700: 7420 6265 2072 756e 6e69 6e67 2077 6865  t be running whe
-00003710: 6e20 7468 6973 2063 6f6d 6d61 6e64 2069  n this command i
-00003720: 7320 7573 6564 2e0a 0a2a 2064 656c 6574  s used...* delet
-00003730: 655f 766f 6c74 7472 6f6e 5f63 7376 202d  e_volttron_csv -
-00003740: 2044 656c 6574 6520 6120 7265 6769 7374   Delete a regist
-00003750: 7279 2063 7376 2063 6f6e 6669 6720 6672  ry csv config fr
-00003760: 6f6d 2056 4f4c 5454 524f 4e2e 2056 4f4c  om VOLTTRON. VOL
-00003770: 5454 524f 4e20 6d75 7374 2062 6520 7275  TTRON must be ru
-00003780: 6e6e 696e 6720 7768 656e 2074 6869 7320  nning when this 
-00003790: 636f 6d6d 616e 6420 6973 2075 7365 642e  command is used.
-000037a0: 0a0a 2320 4465 7665 6c6f 706d 656e 740a  ..# Development.
-000037b0: 0a50 6c65 6173 6520 7365 6520 7468 6520  .Please see the 
-000037c0: 666f 6c6c 6f77 696e 6720 666f 7220 636f  following for co
-000037d0: 6e74 7269 6275 7469 6e67 2067 7569 6465  ntributing guide
-000037e0: 6c69 6e65 7320 5b63 6f6e 7472 6962 7574  lines [contribut
-000037f0: 696e 675d 2868 7474 7073 3a2f 2f67 6974  ing](https://git
-00003800: 6875 622e 636f 6d2f 6563 6c69 7073 652d  hub.com/eclipse-
-00003810: 766f 6c74 7472 6f6e 2f76 6f6c 7474 726f  volttron/volttro
-00003820: 6e2d 636f 7265 2f62 6c6f 622f 6465 7665  n-core/blob/deve
-00003830: 6c6f 702f 434f 4e54 5249 4255 5449 4e47  lop/CONTRIBUTING
-00003840: 2e6d 6429 2e0a 0a50 6c65 6173 6520 7365  .md)...Please se
-00003850: 6520 7468 6520 666f 6c6c 6f77 696e 6720  e the following 
-00003860: 6865 6c70 6675 6c20 6775 6964 6520 6162  helpful guide ab
-00003870: 6f75 7420 5b64 6576 656c 6f70 696e 6720  out [developing 
-00003880: 6d6f 6475 6c61 7220 564f 4c54 5452 4f4e  modular VOLTTRON
-00003890: 2061 6765 6e74 735d 2868 7474 7073 3a2f   agents](https:/
-000038a0: 2f67 6974 6875 622e 636f 6d2f 6563 6c69  /github.com/ecli
-000038b0: 7073 652d 766f 6c74 7472 6f6e 2f76 6f6c  pse-volttron/vol
-000038c0: 7474 726f 6e2d 636f 7265 2f62 6c6f 622f  ttron-core/blob/
-000038d0: 6465 7665 6c6f 702f 4445 5645 4c4f 5049  develop/DEVELOPI
-000038e0: 4e47 5f4f 4e5f 4d4f 4455 4c41 522e 6d64  NG_ON_MODULAR.md
-000038f0: 290a 0a0a 2320 4469 7363 6c61 696d 6572  )...# Disclaimer
-00003900: 204e 6f74 6963 650a 0a54 6869 7320 6d61   Notice..This ma
-00003910: 7465 7269 616c 2077 6173 2070 7265 7061  terial was prepa
-00003920: 7265 6420 6173 2061 6e20 6163 636f 756e  red as an accoun
-00003930: 7420 6f66 2077 6f72 6b20 7370 6f6e 736f  t of work sponso
-00003940: 7265 6420 6279 2061 6e20 6167 656e 6379  red by an agency
-00003950: 206f 6620 7468 650a 556e 6974 6564 2053   of the.United S
-00003960: 7461 7465 7320 476f 7665 726e 6d65 6e74  tates Government
-00003970: 2e20 204e 6569 7468 6572 2074 6865 2055  .  Neither the U
-00003980: 6e69 7465 6420 5374 6174 6573 2047 6f76  nited States Gov
-00003990: 6572 6e6d 656e 7420 6e6f 7220 7468 6520  ernment nor the 
-000039a0: 556e 6974 6564 0a53 7461 7465 7320 4465  United.States De
-000039b0: 7061 7274 6d65 6e74 206f 6620 456e 6572  partment of Ener
-000039c0: 6779 2c20 6e6f 7220 4261 7474 656c 6c65  gy, nor Battelle
-000039d0: 2c20 6e6f 7220 616e 7920 6f66 2074 6865  , nor any of the
-000039e0: 6972 2065 6d70 6c6f 7965 6573 2c20 6e6f  ir employees, no
-000039f0: 7220 616e 790a 6a75 7269 7364 6963 7469  r any.jurisdicti
-00003a00: 6f6e 206f 7220 6f72 6761 6e69 7a61 7469  on or organizati
-00003a10: 6f6e 2074 6861 7420 6861 7320 636f 6f70  on that has coop
-00003a20: 6572 6174 6564 2069 6e20 7468 6520 6465  erated in the de
-00003a30: 7665 6c6f 706d 656e 7420 6f66 2074 6865  velopment of the
-00003a40: 7365 0a6d 6174 6572 6961 6c73 2c20 6d61  se.materials, ma
-00003a50: 6b65 7320 616e 7920 7761 7272 616e 7479  kes any warranty
-00003a60: 2c20 6578 7072 6573 7320 6f72 2069 6d70  , express or imp
-00003a70: 6c69 6564 2c20 6f72 2061 7373 756d 6573  lied, or assumes
-00003a80: 2061 6e79 206c 6567 616c 0a6c 6961 6269   any legal.liabi
-00003a90: 6c69 7479 206f 7220 7265 7370 6f6e 7369  lity or responsi
-00003aa0: 6269 6c69 7479 2066 6f72 2074 6865 2061  bility for the a
-00003ab0: 6363 7572 6163 792c 2063 6f6d 706c 6574  ccuracy, complet
-00003ac0: 656e 6573 732c 206f 7220 7573 6566 756c  eness, or useful
-00003ad0: 6e65 7373 206f 7220 616e 790a 696e 666f  ness or any.info
-00003ae0: 726d 6174 696f 6e2c 2061 7070 6172 6174  rmation, apparat
-00003af0: 7573 2c20 7072 6f64 7563 742c 2073 6f66  us, product, sof
-00003b00: 7477 6172 652c 206f 7220 7072 6f63 6573  tware, or proces
-00003b10: 7320 6469 7363 6c6f 7365 642c 206f 7220  s disclosed, or 
-00003b20: 7265 7072 6573 656e 7473 0a74 6861 7420  represents.that 
-00003b30: 6974 7320 7573 6520 776f 756c 6420 6e6f  its use would no
-00003b40: 7420 696e 6672 696e 6765 2070 7269 7661  t infringe priva
-00003b50: 7465 6c79 206f 776e 6564 2072 6967 6874  tely owned right
-00003b60: 732e 0a0a 5265 6665 7265 6e63 6520 6865  s...Reference he
-00003b70: 7265 696e 2074 6f20 616e 7920 7370 6563  rein to any spec
-00003b80: 6966 6963 2063 6f6d 6d65 7263 6961 6c20  ific commercial 
-00003b90: 7072 6f64 7563 742c 2070 726f 6365 7373  product, process
-00003ba0: 2c20 6f72 2073 6572 7669 6365 2062 790a  , or service by.
-00003bb0: 7472 6164 6520 6e61 6d65 2c20 7472 6164  trade name, trad
-00003bc0: 656d 6172 6b2c 206d 616e 7566 6163 7475  emark, manufactu
-00003bd0: 7265 722c 206f 7220 6f74 6865 7277 6973  rer, or otherwis
-00003be0: 6520 646f 6573 206e 6f74 206e 6563 6573  e does not neces
-00003bf0: 7361 7269 6c79 0a63 6f6e 7374 6974 7574  sarily.constitut
-00003c00: 6520 6f72 2069 6d70 6c79 2069 7473 2065  e or imply its e
-00003c10: 6e64 6f72 7365 6d65 6e74 2c20 7265 636f  ndorsement, reco
-00003c20: 6d6d 656e 6461 7469 6f6e 2c20 6f72 2066  mmendation, or f
-00003c30: 6176 6f72 696e 6720 6279 2074 6865 2055  avoring by the U
-00003c40: 6e69 7465 640a 5374 6174 6573 2047 6f76  nited.States Gov
-00003c50: 6572 6e6d 656e 7420 6f72 2061 6e79 2061  ernment or any a
-00003c60: 6765 6e63 7920 7468 6572 656f 662c 206f  gency thereof, o
-00003c70: 7220 4261 7474 656c 6c65 204d 656d 6f72  r Battelle Memor
-00003c80: 6961 6c20 496e 7374 6974 7574 652e 2054  ial Institute. T
-00003c90: 6865 0a76 6965 7773 2061 6e64 206f 7069  he.views and opi
-00003ca0: 6e69 6f6e 7320 6f66 2061 7574 686f 7273  nions of authors
-00003cb0: 2065 7870 7265 7373 6564 2068 6572 6569   expressed herei
-00003cc0: 6e20 646f 206e 6f74 206e 6563 6573 7361  n do not necessa
-00003cd0: 7269 6c79 2073 7461 7465 206f 720a 7265  rily state or.re
-00003ce0: 666c 6563 7420 7468 6f73 6520 6f66 2074  flect those of t
-00003cf0: 6865 2055 6e69 7465 6420 5374 6174 6573  he United States
-00003d00: 2047 6f76 6572 6e6d 656e 7420 6f72 2061   Government or a
-00003d10: 6e79 2061 6765 6e63 7920 7468 6572 656f  ny agency thereo
-00003d20: 662e 0a0a                                f...
+00000580: 746b 2d64 7269 7665 722f 6163 7469 6f6e  tk-driver/action
+00000590: 732f 776f 726b 666c 6f77 732f 7275 6e2d  s/workflows/run-
+000005a0: 7465 7374 732e 796d 6c2f 6261 6467 652e  tests.yml/badge.
+000005b0: 7376 6729 5d0a 5b21 5b70 7970 6920 7665  svg)].[![pypi ve
+000005c0: 7273 696f 6e5d 2868 7474 7073 3a2f 2f69  rsion](https://i
+000005d0: 6d67 2e73 6869 656c 6473 2e69 6f2f 7079  mg.shields.io/py
+000005e0: 7069 2f76 2f76 6f6c 7474 726f 6e2d 6c69  pi/v/volttron-li
+000005f0: 622d 6d6f 6462 7573 746b 2d64 7269 7665  b-modbustk-drive
+00000600: 722e 7376 6729 5d28 6874 7470 733a 2f2f  r.svg)](https://
+00000610: 7079 7069 2e6f 7267 2f70 726f 6a65 6374  pypi.org/project
+00000620: 2f76 6f6c 7474 726f 6e2d 6c69 622d 6d6f  /volttron-lib-mo
+00000630: 6462 7573 746b 2d64 7269 7665 722f 295d  dbustk-driver/)]
+00000640: 0a0a 2323 2050 7265 7265 7175 6973 6974  ..## Prerequisit
+00000650: 6573 0a0a 2a20 5079 7468 6f6e 2033 2e31  es..* Python 3.1
+00000660: 302b 0a2a 2045 636c 6970 7365 2056 4f4c  0+.* Eclipse VOL
+00000670: 5454 524f 4e3c 7375 703e 746d 3c2f 7375  TTRON<sup>tm</su
+00000680: 703e 2031 302e 302b 0a0a 2323 2320 5079  p> 10.0+..### Py
+00000690: 7468 6f6e 0a0a 3c64 6574 6169 6c73 3e0a  thon..<details>.
+000006a0: 3c73 756d 6d61 7279 3e54 6f20 696e 7374  <summary>To inst
+000006b0: 616c 6c20 5079 7468 6f6e 2033 2e31 302c  all Python 3.10,
+000006c0: 2077 6520 7265 636f 6d6d 656e 6420 7573   we recommend us
+000006d0: 696e 6720 3c61 2068 7265 663d 2268 7474  ing <a href="htt
+000006e0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+000006f0: 7079 656e 762f 7079 656e 7622 3e3c 636f  pyenv/pyenv"><co
+00000700: 6465 3e70 7965 6e76 3c2f 636f 6465 3e3c  de>pyenv</code><
+00000710: 2f61 3e2e 3c2f 7375 6d6d 6172 793e 0a0a  /a>.</summary>..
+00000720: 6060 6062 6173 680a 2320 696e 7374 616c  ```bash.# instal
+00000730: 6c20 7079 656e 760a 6769 7420 636c 6f6e  l pyenv.git clon
+00000740: 6520 6874 7470 733a 2f2f 6769 7468 7562  e https://github
+00000750: 2e63 6f6d 2f70 7965 6e76 2f70 7965 6e76  .com/pyenv/pyenv
+00000760: 207e 2f2e 7079 656e 760a 0a23 2073 6574   ~/.pyenv..# set
+00000770: 7570 2070 7965 6e76 2028 796f 7520 7368  up pyenv (you sh
+00000780: 6f75 6c64 2061 6c73 6f20 7075 7420 7468  ould also put th
+00000790: 6573 6520 7468 7265 6520 6c69 6e65 7320  ese three lines 
+000007a0: 696e 202e 6261 7368 7263 206f 7220 7369  in .bashrc or si
+000007b0: 6d69 6c61 7229 0a65 7870 6f72 7420 5041  milar).export PA
+000007c0: 5448 3d22 247b 484f 4d45 7d2f 2e70 7965  TH="${HOME}/.pye
+000007d0: 6e76 2f62 696e 3a24 7b50 4154 487d 220a  nv/bin:${PATH}".
+000007e0: 6578 706f 7274 2050 5945 4e56 5f52 4f4f  export PYENV_ROO
+000007f0: 543d 2224 7b48 4f4d 457d 2f2e 7079 656e  T="${HOME}/.pyen
+00000800: 7622 0a65 7661 6c20 2224 2870 7965 6e76  v".eval "$(pyenv
+00000810: 2069 6e69 7420 2d29 220a 0a23 2069 6e73   init -)"..# ins
+00000820: 7461 6c6c 2050 7974 686f 6e20 332e 380a  tall Python 3.8.
+00000830: 7079 656e 7620 696e 7374 616c 6c20 332e  pyenv install 3.
+00000840: 3130 0a0a 2320 6d61 6b65 2069 7420 6176  10..# make it av
+00000850: 6169 6c61 626c 6520 676c 6f62 616c 6c79  ailable globally
+00000860: 0a70 7965 6e76 2067 6c6f 6261 6c20 7379  .pyenv global sy
+00000870: 7374 656d 2033 2e31 300a 6060 600a 3c2f  stem 3.10.```.</
+00000880: 6465 7461 696c 733e 0a0a 0a23 2323 2050  details>...### P
+00000890: 6f65 7472 790a 0a54 6869 7320 7072 6f6a  oetry..This proj
+000008a0: 6563 7420 7573 6573 2060 706f 6574 7279  ect uses `poetry
+000008b0: 6020 746f 2069 6e73 7461 6c6c 2061 6e64  ` to install and
+000008c0: 206d 616e 6167 6520 6465 7065 6e64 656e   manage dependen
+000008d0: 6369 6573 2e20 546f 2069 6e73 7461 6c6c  cies. To install
+000008e0: 2070 6f65 7472 792c 0a66 6f6c 6c6f 7720   poetry,.follow 
+000008f0: 7468 6573 6520 5b69 6e73 7472 7563 7469  these [instructi
+00000900: 6f6e 735d 2868 7474 7073 3a2f 2f70 7974  ons](https://pyt
+00000910: 686f 6e2d 706f 6574 7279 2e6f 7267 2f64  hon-poetry.org/d
+00000920: 6f63 732f 6d61 7374 6572 2f23 696e 7374  ocs/master/#inst
+00000930: 616c 6c61 7469 6f6e 292e 0a0a 2320 496e  allation)...# In
+00000940: 7374 616c 6c61 7469 6f6e 0a0a 5769 7468  stallation..With
+00000950: 2060 7069 7060 3a0a 0a60 6060 7368 656c   `pip`:..```shel
+00000960: 6c0a 7079 7468 6f6e 332e 3130 202d 6d20  l.python3.10 -m 
+00000970: 7069 7020 696e 7374 616c 6c20 766f 6c74  pip install volt
+00000980: 7472 6f6e 2d6c 6962 2d6d 6f64 6275 7374  tron-lib-modbust
+00000990: 6b2d 6472 6976 6572 0a0a 2320 4465 7665  k-driver..# Deve
+000009a0: 6c6f 7020 6d6f 6465 0a70 7974 686f 6e33  lop mode.python3
+000009b0: 2e31 3020 2d6d 2070 6970 2069 6e73 7461  .10 -m pip insta
+000009c0: 6c6c 202d 2d65 6469 7461 626c 6520 766f  ll --editable vo
+000009d0: 6c74 7472 6f6e 2d6c 6962 2d6d 6f64 6275  lttron-lib-modbu
+000009e0: 7374 6b2d 6472 6976 6572 0a60 6060 0a0a  stk-driver.```..
+000009f0: 2323 2044 6576 656c 6f70 6d65 6e74 0a0a  ## Development..
+00000a00: 2323 2320 456e 7669 726f 6e6d 656e 740a  ### Environment.
+00000a10: 0a53 6574 2074 6865 2065 6e76 6972 6f6e  .Set the environ
+00000a20: 6d65 6e74 2074 6f20 6265 2069 6e20 796f  ment to be in yo
+00000a30: 7572 2070 726f 6a65 6374 2064 6972 6563  ur project direc
+00000a40: 746f 7279 3a0a 0a60 6060 706f 6574 7279  tory:..```poetry
+00000a50: 2063 6f6e 6669 6720 7669 7274 7561 6c65   config virtuale
+00000a60: 6e76 732e 696e 2d70 726f 6a65 6374 2074  nvs.in-project t
+00000a70: 7275 6560 6060 0a0a 4966 2079 6f75 2077  rue```..If you w
+00000a80: 616e 7420 746f 2069 6e73 7461 6c6c 2061  ant to install a
+00000a90: 6c6c 2079 6f75 7220 6465 7065 6e64 656e  ll your dependen
+00000aa0: 6369 6573 2c20 696e 636c 7564 696e 6720  cies, including 
+00000ab0: 6465 7065 6e64 656e 6369 6573 2074 6f20  dependencies to 
+00000ac0: 6865 6c70 2077 6974 6820 6465 7665 6c6f  help with develo
+00000ad0: 7069 6e67 2079 6f75 7220 6167 656e 742c  ping your agent,
+00000ae0: 2072 756e 2074 6869 7320 636f 6d6d 616e   run this comman
+00000af0: 643a 0a0a 6060 6070 6f65 7472 7920 696e  d:..```poetry in
+00000b00: 7374 616c 6c60 6060 0a0a 4966 2079 6f75  stall```..If you
+00000b10: 2077 616e 7420 746f 2069 6e73 7461 6c6c   want to install
+00000b20: 206f 6e6c 7920 7468 6520 6465 7065 6e64   only the depend
+00000b30: 656e 6369 6573 206e 6565 6465 6420 746f  encies needed to
+00000b40: 2072 756e 2079 6f75 7220 6167 656e 742c   run your agent,
+00000b50: 2072 756e 2074 6869 7320 636f 6d6d 616e   run this comman
+00000b60: 643a 0a0a 6060 6070 6f65 7472 7920 696e  d:..```poetry in
+00000b70: 7374 616c 6c20 2d2d 6e6f 2d64 6576 6060  stall --no-dev``
+00000b80: 600a 0a41 6374 6976 6174 6520 7468 6520  `..Activate the 
+00000b90: 7669 7274 7561 6c20 656e 7669 726f 6e6d  virtual environm
+00000ba0: 656e 743a 0a0a 6060 6073 6865 6c6c 0a23  ent:..```shell.#
+00000bb0: 2075 7369 6e67 2050 6f65 7472 790a 706f   using Poetry.po
+00000bc0: 6574 7279 2073 6865 6c6c 0a0a 2320 7573  etry shell..# us
+00000bd0: 696e 6720 2773 6f75 7263 6527 2063 6f6d  ing 'source' com
+00000be0: 6d61 6e64 0a73 6f75 7263 6520 2224 2870  mand.source "$(p
+00000bf0: 6f65 7472 7920 656e 7620 696e 666f 202d  oetry env info -
+00000c00: 2d70 6174 6829 2f62 696e 2f61 6374 6976  -path)/bin/activ
+00000c10: 6174 6522 0a60 6060 0a0a 2323 2320 536f  ate".```..### So
+00000c20: 7572 6365 2043 6f6e 7472 6f6c 0a0a 312e  urce Control..1.
+00000c30: 2054 6f20 7573 6520 6769 7420 746f 206d   To use git to m
+00000c40: 616e 6167 6520 7665 7273 696f 6e20 636f  anage version co
+00000c50: 6e74 726f 6c2c 2063 7265 6174 6520 6120  ntrol, create a 
+00000c60: 6e65 7720 6769 7420 7265 706f 7369 746f  new git reposito
+00000c70: 7279 2069 6e20 796f 7572 206c 6f63 616c  ry in your local
+00000c80: 2061 6765 6e74 2070 726f 6a65 6374 2e0a   agent project..
+00000c90: 0a60 6060 6769 7420 696e 6974 6060 600a  .```git init```.
+00000ca0: 0a32 2e20 5468 656e 2063 7265 6174 6520  .2. Then create 
+00000cb0: 6120 6e65 7720 7265 706f 2069 6e20 796f  a new repo in yo
+00000cc0: 7572 2047 6974 6875 6220 6f72 2047 6974  ur Github or Git
+00000cd0: 6c61 6220 6163 636f 756e 742e 2043 6f70  lab account. Cop
+00000ce0: 7920 7468 6520 5552 4c20 7468 6174 2070  y the URL that p
+00000cf0: 6f69 6e74 7320 746f 2074 6861 7420 6e65  oints to that ne
+00000d00: 7720 7265 706f 2069 6e0a 796f 7572 2047  w repo in.your G
+00000d10: 6974 6875 6220 6f72 2047 6974 6c61 6220  ithub or Gitlab 
+00000d20: 6163 636f 756e 742e 2054 6869 7320 7769  account. This wi
+00000d30: 6c6c 2062 6520 6b6e 6f77 6e20 6173 206f  ll be known as o
+00000d40: 7572 2027 7265 6d6f 7465 272e 0a0a 332e  ur 'remote'...3.
+00000d50: 2041 6464 2074 6865 2072 656d 6f74 6520   Add the remote 
+00000d60: 2869 2e65 2e20 7468 6520 6e65 7720 7265  (i.e. the new re
+00000d70: 706f 2055 524c 2066 726f 6d20 796f 7572  po URL from your
+00000d80: 2047 6974 6875 6220 6f72 2047 6974 6c61   Github or Gitla
+00000d90: 6220 6163 636f 756e 7429 2074 6f20 796f  b account) to yo
+00000da0: 7572 206c 6f63 616c 2072 6570 6f73 6974  ur local reposit
+00000db0: 6f72 792e 2052 756e 2074 6865 2066 6f6c  ory. Run the fol
+00000dc0: 6c6f 7769 6e67 2063 6f6d 6d61 6e64 3a0a  lowing command:.
+00000dd0: 0a60 6060 6769 7420 7265 6d6f 7465 2061  .```git remote a
+00000de0: 6464 206f 7269 6769 6e20 3c6d 7920 6769  dd origin <my gi
+00000df0: 7468 7562 2f67 6974 6c61 6220 5552 4c3e  thub/gitlab URL>
+00000e00: 6060 600a 0a57 6865 6e20 796f 7520 7075  ```..When you pu
+00000e10: 7368 2074 6f20 796f 7572 2072 6570 6f2c  sh to your repo,
+00000e20: 206e 6f74 6520 7468 6174 2074 6865 2064   note that the d
+00000e30: 6566 6175 6c74 2062 7261 6e63 6820 6973  efault branch is
+00000e40: 2063 616c 6c65 6420 276d 6169 6e27 2e0a   called 'main'..
+00000e50: 0a0a 2323 2320 4f70 7469 6f6e 616c 2043  ..### Optional C
+00000e60: 6f6e 6669 6775 7261 7469 6f6e 730a 0a23  onfigurations..#
+00000e70: 2323 2320 5072 6563 6f6d 6d69 740a 0a4e  ### Precommit..N
+00000e80: 6f74 653a 2045 6e73 7572 6520 7468 6174  ote: Ensure that
+00000e90: 2079 6f75 2068 6176 6520 6372 6561 7465   you have create
+00000ea0: 6420 7468 6520 7669 7274 7561 6c20 656e  d the virtual en
+00000eb0: 7669 726f 6e6d 656e 7420 7573 696e 6720  vironment using 
+00000ec0: 506f 6574 7279 0a0a 496e 7374 616c 6c20  Poetry..Install 
+00000ed0: 7072 652d 636f 6d6d 6974 2068 6f6f 6b73  pre-commit hooks
+00000ee0: 3a0a 0a60 6060 706f 6574 7279 2072 756e  :..```poetry run
+00000ef0: 2070 7265 2d63 6f6d 6d69 7420 696e 7374   pre-commit inst
+00000f00: 616c 6c60 6060 0a0a 546f 2072 756e 2070  all```..To run p
+00000f10: 7265 2d63 6f6d 6d69 7420 6f6e 2061 6c6c  re-commit on all
+00000f20: 2079 6f75 7220 6669 6c65 732c 2072 756e   your files, run
+00000f30: 2074 6869 7320 636f 6d6d 616e 643a 0a0a   this command:..
+00000f40: 6060 6070 6f65 7472 7920 7275 6e20 7072  ```poetry run pr
+00000f50: 652d 636f 6d6d 6974 2072 756e 202d 2d61  e-commit run --a
+00000f60: 6c6c 2d66 696c 6573 6060 600a 0a49 6620  ll-files```..If 
+00000f70: 796f 7520 6861 7665 2070 7265 636f 6d6d  you have precomm
+00000f80: 6974 2069 6e73 7461 6c6c 6564 2061 6e64  it installed and
+00000f90: 2079 6f75 2077 616e 7420 746f 2069 676e   you want to ign
+00000fa0: 6f72 6520 7275 6e6e 696e 6720 7468 6520  ore running the 
+00000fb0: 636f 6d6d 6974 2068 6f6f 6b73 0a65 7665  commit hooks.eve
+00000fc0: 7279 2074 696d 6520 796f 7520 7275 6e20  ry time you run 
+00000fd0: 6120 636f 6d6d 6974 2c20 696e 636c 7564  a commit, includ
+00000fe0: 6520 7468 6520 602d 2d6e 6f2d 7665 7269  e the `--no-veri
+00000ff0: 6679 6020 666c 6167 2069 6e20 796f 7572  fy` flag in your
+00001000: 2063 6f6d 6d69 742e 2054 6865 2066 6f6c   commit. The fol
+00001010: 6c6f 7769 6e67 0a69 7320 616e 2065 7861  lowing.is an exa
+00001020: 6d70 6c65 3a0a 0a60 6060 6769 7420 636f  mple:..```git co
+00001030: 6d6d 6974 202d 6d20 2253 6f6d 6520 6d65  mmit -m "Some me
+00001040: 7373 6167 6522 202d 2d6e 6f2d 7665 7269  ssage" --no-veri
+00001050: 6679 6060 600a 0a0a 2323 2044 6f63 756d  fy```...## Docum
+00001060: 656e 7461 7469 6f6e 0a0a 0a23 2044 6f63  entation...# Doc
+00001070: 756d 656e 7461 7469 6f6e 0a4d 6f72 6520  umentation.More 
+00001080: 6465 7461 696c 6564 2064 6f63 756d 656e  detailed documen
+00001090: 7461 7469 6f6e 2063 616e 2062 6520 666f  tation can be fo
+000010a0: 756e 6420 6f6e 205b 5265 6164 5468 6544  und on [ReadTheD
+000010b0: 6f63 735d 2868 7474 7073 3a2f 2f76 6f6c  ocs](https://vol
+000010c0: 7474 726f 6e2e 7265 6164 7468 6564 6f63  ttron.readthedoc
+000010d0: 732e 696f 2f65 6e2f 6d6f 6475 6c61 722f  s.io/en/modular/
+000010e0: 292e 2054 6865 2052 5354 2073 6f75 7263  ). The RST sourc
+000010f0: 650a 6f66 2074 6865 2064 6f63 756d 656e  e.of the documen
+00001100: 7461 7469 6f6e 2066 6f72 2074 6869 7320  tation for this 
+00001110: 636f 6d70 6f6e 656e 7420 6973 206c 6f63  component is loc
+00001120: 6174 6564 2069 6e20 7468 6520 2264 6f63  ated in the "doc
+00001130: 7322 2064 6972 6563 746f 7279 206f 6620  s" directory of 
+00001140: 7468 6973 2072 6570 6f73 6974 6f72 792e  this repository.
+00001150: 0a0a 2320 496e 7374 616c 6c61 7469 6f6e  ..# Installation
+00001160: 0a0a 4265 666f 7265 2069 6e73 7461 6c6c  ..Before install
+00001170: 696e 672c 2056 4f4c 5454 524f 4e20 7368  ing, VOLTTRON sh
+00001180: 6f75 6c64 2062 6520 696e 7374 616c 6c65  ould be installe
+00001190: 6420 616e 6420 7275 6e6e 696e 672e 2020  d and running.  
+000011a0: 4974 7320 7669 7274 7561 6c20 656e 7669  Its virtual envi
+000011b0: 726f 6e6d 656e 7420 7368 6f75 6c64 2062  ronment should b
+000011c0: 6520 6163 7469 7665 2e0a 496e 666f 726d  e active..Inform
+000011d0: 6174 696f 6e20 6f6e 2068 6f77 2074 6f20  ation on how to 
+000011e0: 696e 7374 616c 6c20 6f66 2074 6865 2056  install of the V
+000011f0: 4f4c 5454 524f 4e20 706c 6174 666f 726d  OLTTRON platform
+00001200: 2063 616e 2062 6520 666f 756e 640a 5b68   can be found.[h
+00001210: 6572 655d 2868 7474 7073 3a2f 2f67 6974  ere](https://git
+00001220: 6875 622e 636f 6d2f 6563 6c69 7073 652d  hub.com/eclipse-
+00001230: 766f 6c74 7472 6f6e 2f76 6f6c 7474 726f  volttron/volttro
+00001240: 6e2d 636f 7265 292e 0a0a 312e 2049 6620  n-core)...1. If 
+00001250: 6974 2069 7320 6e6f 7420 616c 7265 6164  it is not alread
+00001260: 792c 2069 6e73 7461 6c6c 2074 6865 2056  y, install the V
+00001270: 4f4c 5454 524f 4e20 506c 6174 666f 726d  OLTTRON Platform
+00001280: 2044 7269 7665 7220 4167 656e 743a 0a0a   Driver Agent:..
+00001290: 2020 2020 6060 6073 6865 6c6c 0a20 2020      ```shell.   
+000012a0: 2076 6374 6c20 696e 7374 616c 6c20 766f   vctl install vo
+000012b0: 6c74 7472 6f6e 2d70 6c61 7466 6f72 6d2d  lttron-platform-
+000012c0: 6472 6976 6572 202d 2d76 6970 2d69 6465  driver --vip-ide
+000012d0: 6e74 6974 7920 706c 6174 666f 726d 2e64  ntity platform.d
+000012e0: 7269 7665 7220 2d2d 7374 6172 740a 2020  river --start.  
+000012f0: 2020 6060 600a 0a31 2e20 496e 7374 616c    ```..1. Instal
+00001300: 6c20 7468 6520 766f 6c74 7472 6f6e 2d6c  l the volttron-l
+00001310: 6962 2d6d 6f64 6275 7374 6b2d 6472 6976  ib-modbustk-driv
+00001320: 6572 206c 6962 7261 7279 2e0a 0a20 2020  er library...   
+00001330: 2060 6060 7368 656c 6c0a 2020 2020 7069   ```shell.    pi
+00001340: 7020 696e 7374 616c 6c20 766f 6c74 7472  p install volttr
+00001350: 6f6e 2d6c 6962 2d6d 6f64 6275 7374 6b2d  on-lib-modbustk-
+00001360: 6472 6976 6572 0a20 2020 2060 6060 0a0a  driver.    ```..
+00001370: 312e 2049 6e73 7461 6c6c 2074 6865 2064  1. Install the d
+00001380: 7269 7665 7220 6f6e 746f 2074 6865 2050  river onto the P
+00001390: 6c61 7466 6f72 6d20 4472 6976 6572 2e0a  latform Driver..
+000013a0: 0a20 2020 2049 6e73 7461 6c6c 696e 6720  .    Installing 
+000013b0: 6120 6472 6976 6572 2069 6e20 7468 6520  a driver in the 
+000013c0: 506c 6174 666f 726d 2044 7269 7665 7220  Platform Driver 
+000013d0: 4167 656e 7420 7265 7175 6972 6573 2061  Agent requires a
+000013e0: 6464 696e 6720 636f 7069 6573 206f 6620  dding copies of 
+000013f0: 7468 6520 6465 7669 6365 2063 6f6e 6669  the device confi
+00001400: 6775 7261 7469 6f6e 2061 6e64 2072 6567  guration and reg
+00001410: 6973 7472 7920 636f 6e66 6967 7572 6174  istry configurat
+00001420: 696f 6e20 6669 6c65 7320 746f 2074 6865  ion files to the
+00001430: 2050 6c61 7466 6f72 6d20 4472 6976 6572   Platform Driver
+00001440: e280 9973 2063 6f6e 6669 6775 7261 7469  ...s configurati
+00001450: 6f6e 2073 746f 7265 2e0a 0a20 2020 2043  on store...    C
+00001460: 7265 6174 6520 6120 636f 6e66 6967 2064  reate a config d
+00001470: 6972 6563 746f 7279 2061 6e64 206e 6176  irectory and nav
+00001480: 6967 6174 6520 746f 2069 743a 0a0a 2020  igate to it:..  
+00001490: 2020 6060 6073 6865 6c6c 0a20 2020 206d    ```shell.    m
+000014a0: 6b64 6972 2063 6f6e 6669 670a 2020 2020  kdir config.    
+000014b0: 6364 2063 6f6e 6669 670a 2020 2020 6060  cd config.    ``
+000014c0: 600a 0a31 2e20 4164 6420 6472 6976 6572  `..1. Add driver
+000014d0: 2063 6f6e 6669 6775 7261 7469 6f6e 7320   configurations 
+000014e0: 746f 2074 6865 2050 6c61 7466 6f72 6d20  to the Platform 
+000014f0: 4472 6976 6572 2e0a 0a20 2020 5468 6520  Driver...   The 
+00001500: 4d6f 6462 7573 2d54 4b20 6472 6976 6572  Modbus-TK driver
+00001510: 2069 7320 6d6f 7374 6c79 2062 6163 6b77   is mostly backw
+00001520: 6172 642d 636f 6d70 6174 6962 6c65 2077  ard-compatible w
+00001530: 6974 6820 7468 6520 7061 7261 6d65 7465  ith the paramete
+00001540: 7220 6465 6669 6e69 7469 6f6e 7320 696e  r definitions in
+00001550: 2074 6865 206f 7269 6769 6e61 6c20 4d6f   the original Mo
+00001560: 6462 7573 2064 7269 7665 72e2 8099 7320  dbus driver...s 
+00001570: 636f 6e66 6967 7572 6174 696f 6e20 282e  configuration (.
+00001580: 636f 6e66 6967 2061 6e64 202e 6373 7620  config and .csv 
+00001590: 6669 6c65 7329 2e20 4966 2074 6865 2063  files). If the c
+000015a0: 6f6e 6669 6720 6669 6c65 e280 9973 2070  onfig file...s p
+000015b0: 6172 616d 6574 6572 206e 616d 6573 2075  arameter names u
+000015c0: 7365 2074 6865 204d 6f64 6275 7320 6472  se the Modbus dr
+000015d0: 6976 6572 e280 9973 206e 616d 6520 636f  iver...s name co
+000015e0: 6e76 656e 7469 6f6e 732c 2074 6865 7920  nventions, they 
+000015f0: 6172 6520 7472 616e 736c 6174 6564 2074  are translated t
+00001600: 6f20 7468 6520 4d6f 6462 7573 2d54 4b20  o the Modbus-TK 
+00001610: 6e61 6d65 2063 6f6e 7665 6e74 696f 6e73  name conventions
+00001620: 2c20 652e 672e 2061 204d 6f64 6275 7320  , e.g. a Modbus 
+00001630: 4353 5620 6669 6c65 e280 9973 2050 6f69  CSV file...s Poi
+00001640: 6e74 2041 6464 7265 7373 2069 7320 696e  nt Address is in
+00001650: 7465 7270 7265 7465 6420 6173 2061 204d  terpreted as a M
+00001660: 6f64 6275 732d 544b 20e2 809c 4164 6472  odbus-TK ...Addr
+00001670: 6573 73e2 809d 2e20 4261 636b 7761 7264  ess.... Backward
+00001680: 2d63 6f6d 7061 7469 6269 6c69 7479 2065  -compatibility e
+00001690: 7863 6570 7469 6f6e 7320 6172 653a 0a0a  xceptions are:..
+000016a0: 2020 2020 2020 2020 2a20 4966 2074 6865          * If the
+000016b0: 2063 6f6e 6669 6720 6669 6c65 2068 6173   config file has
+000016c0: 206e 6f20 706f 7274 2c20 7468 6520 6465   no port, the de
+000016d0: 6661 756c 7420 6973 2030 2c20 6e6f 7420  fault is 0, not 
+000016e0: 3530 322e 0a0a 2020 2020 2020 2020 2a20  502...        * 
+000016f0: 4966 2074 6865 2063 6f6e 6669 6720 6669  If the config fi
+00001700: 6c65 2068 6173 206e 6f20 736c 6176 655f  le has no slave_
+00001710: 6964 2c20 7468 6520 6465 6661 756c 7420  id, the default 
+00001720: 6973 2031 2c20 6e6f 7420 302e 0a0a 2020  is 1, not 0...  
+00001730: 2020 5468 6520 6472 6976 6572 5f63 6f6e    The driver_con
+00001740: 6669 6720 7365 6374 696f 6e20 6f66 2061  fig section of a
+00001750: 204d 6f64 6275 732d 544b 2064 6576 6963   Modbus-TK devic
+00001760: 6520 636f 6e66 6967 7572 6174 696f 6e20  e configuration 
+00001770: 6669 6c65 2073 7570 706f 7274 7320 6120  file supports a 
+00001780: 7661 7269 6574 7920 6f66 2070 6172 616d  variety of param
+00001790: 6574 6572 2064 6566 696e 6974 696f 6e73  eter definitions
+000017a0: 2c20 6275 7420 6f6e 6c79 202a 6465 7669  , but only *devi
+000017b0: 6365 5f61 6464 7265 7373 2a20 6973 2072  ce_address* is r
+000017c0: 6571 7569 7265 643a 0a0a 2020 2020 2a20  equired:..    * 
+000017d0: 6465 7669 6365 5f61 6464 7265 7373 2028  device_address (
+000017e0: 5265 7175 6972 6564 293a 2020 4950 2041  Required):  IP A
+000017f0: 6464 7265 7373 206f 6620 7468 6520 6465  ddress of the de
+00001800: 7669 6365 2e0a 0a20 2020 202a 206e 616d  vice...    * nam
+00001810: 6520 284f 7074 696f 6e61 6c29 202d 204e  e (Optional) - N
+00001820: 616d 6520 6f66 2074 6865 2064 6576 6963  ame of the devic
+00001830: 652e 2044 6566 6175 6c74 7320 746f 20e2  e. Defaults to .
+00001840: 809c 554e 4b4e 4f57 4ee2 809d 2e0a 0a20  ..UNKNOWN...... 
+00001850: 2020 202a 2064 6576 6963 655f 7479 7065     * device_type
+00001860: 2028 4f70 7469 6f6e 616c 2920 2d20 4e61   (Optional) - Na
+00001870: 6d65 206f 6620 7468 6520 6465 7669 6365  me of the device
+00001880: 2074 7970 652e 2044 6566 6175 6c74 7320   type. Defaults 
+00001890: 746f 20e2 809c 554e 4b4e 4f57 4ee2 809d  to ...UNKNOWN...
+000018a0: 2e0a 0a20 2020 202a 2070 6f72 7420 284f  ...    * port (O
+000018b0: 7074 696f 6e61 6c29 202d 2050 6f72 7420  ptional) - Port 
+000018c0: 7468 6520 6465 7669 6365 2069 7320 6c69  the device is li
+000018d0: 7374 656e 696e 6720 6f6e 2e20 4465 6661  stening on. Defa
+000018e0: 756c 7473 2074 6f20 3020 286e 6f20 706f  ults to 0 (no po
+000018f0: 7274 292e 2055 7365 2070 6f72 7420 3020  rt). Use port 0 
+00001900: 666f 7220 5254 5520 7472 616e 7370 6f72  for RTU transpor
+00001910: 742e 0a0a 2020 2020 2a20 736c 6176 655f  t...    * slave_
+00001920: 6964 2028 4f70 7469 6f6e 616c 2920 2d20  id (Optional) - 
+00001930: 536c 6176 6520 4944 206f 6620 7468 6520  Slave ID of the 
+00001940: 6465 7669 6365 2e20 4465 6661 756c 7473  device. Defaults
+00001950: 2074 6f20 312e 2055 7365 2049 4420 3020   to 1. Use ID 0 
+00001960: 666f 7220 6e6f 2073 6c61 7665 2e0a 0a20  for no slave... 
+00001970: 2020 202a 2062 6175 6472 6174 6520 284f     * baudrate (O
+00001980: 7074 696f 6e61 6c29 202d 2053 6572 6961  ptional) - Seria
+00001990: 6c20 2852 5455 2920 6261 7564 2072 6174  l (RTU) baud rat
+000019a0: 652e 2044 6566 6175 6c74 7320 746f 2039  e. Defaults to 9
+000019b0: 3630 302e 0a0a 2020 2020 2a20 6279 7465  600...    * byte
+000019c0: 7369 7a65 2028 4f70 7469 6f6e 616c 2920  size (Optional) 
+000019d0: 2d20 5365 7269 616c 2028 5254 5529 2062  - Serial (RTU) b
+000019e0: 7974 6520 7369 7a65 3a20 352c 2036 2c20  yte size: 5, 6, 
+000019f0: 372c 206f 7220 382e 2044 6566 6175 6c74  7, or 8. Default
+00001a00: 7320 746f 2038 2e0a 0a20 2020 202a 2070  s to 8...    * p
+00001a10: 6172 6974 7920 284f 7074 696f 6e61 6c29  arity (Optional)
+00001a20: 202d 2053 6572 6961 6c20 2852 5455 2920   - Serial (RTU) 
+00001a30: 7061 7269 7479 3a20 6e6f 6e65 2c20 6576  parity: none, ev
+00001a40: 656e 2c20 6f64 642c 206d 6172 6b2c 206f  en, odd, mark, o
+00001a50: 7220 7370 6163 652e 2044 6566 6175 6c74  r space. Default
+00001a60: 7320 746f 204e 6f6e 652e 0a0a 2020 2020  s to None...    
+00001a70: 2a20 7374 6f70 6269 7473 2028 4f70 7469  * stopbits (Opti
+00001a80: 6f6e 616c 2920 2d20 5365 7269 616c 2028  onal) - Serial (
+00001a90: 5254 5529 2073 746f 7020 6269 7473 3a20  RTU) stop bits: 
+00001aa0: 312c 2031 2e35 2c20 6f72 2032 2e20 4465  1, 1.5, or 2. De
+00001ab0: 6661 756c 7473 2074 6f20 312e 0a0a 2020  faults to 1...  
+00001ac0: 2020 2a20 786f 6e78 6f66 6620 284f 7074    * xonxoff (Opt
+00001ad0: 696f 6e61 6c29 202d 2053 6572 6961 6c20  ional) - Serial 
+00001ae0: 2852 5455 2920 666c 6f77 2063 6f6e 7472  (RTU) flow contr
+00001af0: 6f6c 3a20 3020 6f72 2031 2e20 4465 6661  ol: 0 or 1. Defa
+00001b00: 756c 7473 2074 6f20 302e 0a0a 2020 2020  ults to 0...    
+00001b10: 2a20 6164 6472 6573 7369 6e67 2028 4f70  * addressing (Op
+00001b20: 7469 6f6e 616c 2920 2d20 4461 7461 2061  tional) - Data a
+00001b30: 6464 7265 7373 2074 6162 6c65 3a20 6f66  ddress table: of
+00001b40: 6673 6574 2c20 6f66 6673 6574 5f70 6c75  fset, offset_plu
+00001b50: 732c 206f 7220 6164 6472 6573 732e 2044  s, or address. D
+00001b60: 6566 6175 6c74 7320 746f 206f 6666 7365  efaults to offse
+00001b70: 742e 0a0a 2020 2020 2020 2a20 6164 6472  t...      * addr
+00001b80: 6573 733a 2054 6865 2065 7861 6374 2076  ess: The exact v
+00001b90: 616c 7565 206f 6620 7468 6520 6164 6472  alue of the addr
+00001ba0: 6573 7320 7769 7468 6f75 7420 616e 7920  ess without any 
+00001bb0: 6f66 6673 6574 2076 616c 7565 2e0a 0a20  offset value... 
+00001bc0: 2020 2020 202a 206f 6666 7365 743a 2054       * offset: T
+00001bd0: 6865 2076 616c 7565 206f 6620 7468 6520  he value of the 
+00001be0: 6164 6472 6573 7320 706c 7573 2074 6865  address plus the
+00001bf0: 206f 6666 7365 7420 7661 6c75 652e 0a0a   offset value...
+00001c00: 2020 2020 2020 2a20 6f66 6673 6574 5f70        * offset_p
+00001c10: 6c75 733a 2054 6865 2076 616c 7565 206f  lus: The value o
+00001c20: 6620 7468 6520 6164 6472 6573 7320 706c  f the address pl
+00001c30: 7573 2074 6865 206f 6666 7365 7420 7661  us the offset va
+00001c40: 6c75 6520 706c 7573 206f 6e65 2e0a 0a20  lue plus one... 
+00001c50: 2020 2020 202a 203a 2049 6620 616e 206f       * : If an o
+00001c60: 6666 7365 7420 7661 6c75 6520 6973 2074  ffset value is t
+00001c70: 6f20 6265 2061 6464 6564 2c20 6974 2069  o be added, it i
+00001c80: 7320 6465 7465 726d 696e 6564 2062 6173  s determined bas
+00001c90: 6564 206f 6e20 6120 706f 696e 74e2 8099  ed on a point...
+00001ca0: 7320 7072 6f70 6572 7469 6573 2069 6e20  s properties in 
+00001cb0: 7468 6520 4353 5620 6669 6c65 3a0a 0a20  the CSV file:.. 
+00001cc0: 2020 2020 2020 202a 2054 7970 653d 626f         * Type=bo
+00001cd0: 6f6c 2c20 5772 6974 6162 6c65 3d54 5255  ol, Writable=TRU
+00001ce0: 453a 2030 0a0a 2020 2020 2020 2020 2a20  E: 0..        * 
+00001cf0: 5479 7065 3d62 6f6f 6c2c 2057 7269 7461  Type=bool, Writa
+00001d00: 626c 653d 4641 4c53 453a 2031 3030 3030  ble=FALSE: 10000
+00001d10: 0a0a 2020 2020 2020 2020 2a20 5479 7065  ..        * Type
+00001d20: 213d 626f 6f6c 2c20 5772 6974 6162 6c65  !=bool, Writable
+00001d30: 3d54 5255 453a 2033 3030 3030 0a0a 2020  =TRUE: 30000..  
+00001d40: 2020 2020 2020 2a20 5479 7065 213d 626f        * Type!=bo
+00001d50: 6f6c 2c20 5772 6974 6162 6c65 3d46 414c  ol, Writable=FAL
+00001d60: 5345 3a20 3430 3030 300a 0a20 2020 202a  SE: 40000..    *
+00001d70: 2065 6e64 6961 6e20 284f 7074 696f 6e61   endian (Optiona
+00001d80: 6c29 202d 2042 7974 6520 6f72 6465 723a  l) - Byte order:
+00001d90: 2062 6967 206f 7220 6c69 7474 6c65 2e20   big or little. 
+00001da0: 4465 6661 756c 7473 2074 6f20 6269 672e  Defaults to big.
+00001db0: 0a0a 2020 2020 2a20 7772 6974 655f 6d75  ..    * write_mu
+00001dc0: 6c74 6970 6c65 5f72 6567 6973 7465 7273  ltiple_registers
+00001dd0: 2028 4f70 7469 6f6e 616c 2920 2d20 5772   (Optional) - Wr
+00001de0: 6974 6520 6d75 6c74 6970 6c65 2063 6f69  ite multiple coi
+00001df0: 6c73 206f 7220 7265 6769 7374 6572 7320  ls or registers 
+00001e00: 6174 2061 2074 696d 652e 2044 6566 6175  at a time. Defau
+00001e10: 6c74 7320 746f 2074 7275 652e 0a0a 2020  lts to true...  
+00001e20: 2020 2020 2a20 4966 2077 7269 7465 5f6d      * If write_m
+00001e30: 756c 7469 706c 655f 7265 6769 7374 6572  ultiple_register
+00001e40: 7320 6973 2073 6574 2074 6f20 6661 6c73  s is set to fals
+00001e50: 652c 206f 6e6c 7920 7265 6769 7374 6572  e, only register
+00001e60: 2074 7970 6573 2075 6e73 6967 6e65 6420   types unsigned 
+00001e70: 7368 6f72 7420 2875 696e 7431 3629 2061  short (uint16) a
+00001e80: 6e64 2062 6f6f 6c65 616e 2028 626f 6f6c  nd boolean (bool
+00001e90: 2920 6172 6520 7375 7070 6f72 7465 642e  ) are supported.
+00001ea0: 2054 6865 2065 7863 6570 7469 6f6e 2072   The exception r
+00001eb0: 6169 7365 6420 6475 7269 6e67 2074 6865  aised during the
+00001ec0: 2063 6f6e 6669 6775 7265 2070 726f 6365   configure proce
+00001ed0: 7373 2e0a 0a20 2020 202a 2072 6567 6973  ss...    * regis
+00001ee0: 7465 725f 6d61 7020 284f 7074 696f 6e61  ter_map (Optiona
+00001ef0: 6c29 202d 2052 6567 6973 7465 7220 6d61  l) - Register ma
+00001f00: 7020 6373 7620 6f66 2075 6e63 6861 6e67  p csv of unchang
+00001f10: 6564 2072 6567 6973 7465 7220 7661 7269  ed register vari
+00001f20: 6162 6c65 732e 2044 6566 6175 6c74 7320  ables. Defaults 
+00001f30: 746f 2072 6567 6973 7472 795f 636f 6e66  to registry_conf
+00001f40: 6967 2063 7376 2e0a 0a20 2020 2054 6869  ig csv...    Thi
+00001f50: 7320 7265 706f 2070 726f 7669 6465 7320  s repo provides 
+00001f60: 616e 2065 7861 6d70 6c65 2063 6f6e 6669  an example confi
+00001f70: 6775 7261 7469 6f6e 2069 6e20 7468 6520  guration in the 
+00001f80: 6669 6c65 2022 6d6f 6462 7573 5f74 6b5f  file "modbus_tk_
+00001f90: 6578 616d 706c 652e 636f 6e66 6967 222e  example.config".
+00001fa0: 0a0a 2020 2020 4865 7265 2069 7320 616e  ..    Here is an
+00001fb0: 2065 7861 6d70 6c65 2064 6576 6963 6520   example device 
+00001fc0: 636f 6e66 6967 7572 6174 696f 6e20 6669  configuration fi
+00001fd0: 6c65 3a0a 0a20 2020 2060 6060 6a73 6f6e  le:..    ```json
+00001fe0: 0a20 2020 2020 2020 207b 0a20 2020 2020  .        {.     
+00001ff0: 2020 2022 6472 6976 6572 5f63 6f6e 6669     "driver_confi
+00002000: 6722 3a20 7b0a 2020 2020 2020 2020 2020  g": {.          
+00002010: 2020 2264 6576 6963 655f 6164 6472 6573    "device_addres
+00002020: 7322 3a20 2231 302e 312e 312e 3222 2c0a  s": "10.1.1.2",.
+00002030: 2020 2020 2020 2020 2020 2020 2270 6f72              "por
+00002040: 7422 3a20 2235 3032 3022 2c0a 2020 2020  t": "5020",.    
+00002050: 2020 2020 2020 2020 2272 6567 6973 7465          "registe
+00002060: 725f 6d61 7022 3a20 2263 6f6e 6669 673a  r_map": "config:
+00002070: 2f2f 6d6f 6462 7573 5f74 6b5f 7465 7374  //modbus_tk_test
+00002080: 5f6d 6170 2e63 7376 220a 2020 2020 2020  _map.csv".      
+00002090: 2020 7d2c 0a20 2020 2020 2020 2022 6472    },.        "dr
+000020a0: 6976 6572 5f74 7970 6522 3a20 226d 6f64  iver_type": "mod
+000020b0: 6275 735f 746b 222c 0a20 2020 2020 2020  bus_tk",.       
+000020c0: 2022 7265 6769 7374 7279 5f63 6f6e 6669   "registry_confi
+000020d0: 6722 3a20 2263 6f6e 6669 673a 2f2f 6d6f  g": "config://mo
+000020e0: 6462 7573 5f74 6b5f 7465 7374 2e63 7376  dbus_tk_test.csv
+000020f0: 222c 0a20 2020 2020 2020 2022 696e 7465  ",.        "inte
+00002100: 7276 616c 223a 2036 302c 0a20 2020 2020  rval": 60,.     
+00002110: 2020 2022 7469 6d65 7a6f 6e65 223a 2022     "timezone": "
+00002120: 5554 4322 2c0a 2020 2020 2020 2020 2268  UTC",.        "h
+00002130: 6561 7274 5f62 6561 745f 706f 696e 7422  eart_beat_point"
+00002140: 3a20 2268 6561 7274 6265 6174 220a 2020  : "heartbeat".  
+00002150: 2020 2020 2020 7d0a 2020 2020 6060 600a        }.    ```.
+00002160: 0a20 2020 2041 6674 6572 2063 7265 6174  .    After creat
+00002170: 696e 6720 6120 6472 6976 6572 2063 6f6e  ing a driver con
+00002180: 6669 6775 7261 7469 6f6e 2066 696c 6520  figuration file 
+00002190: 6e61 6d65 6420 226d 6f64 6275 735f 746b  named "modbus_tk
+000021a0: 5f65 7861 6d70 6c65 2e63 6f6e 6669 6722  _example.config"
+000021b0: 2c20 6164 6420 6974 2074 6f20 7468 6520  , add it to the 
+000021c0: 436f 6e66 6967 7572 6174 696f 6e20 5374  Configuration St
+000021d0: 6f72 653a 0a0a 2020 2020 6060 6073 6865  ore:..    ```she
+000021e0: 6c6c 0a20 2020 2076 6374 6c20 636f 6e66  ll.    vctl conf
+000021f0: 6967 2073 746f 7265 2070 6c61 7466 6f72  ig store platfor
+00002200: 6d2e 6472 6976 6572 2064 6576 6963 6573  m.driver devices
+00002210: 2f6d 6f64 6275 7374 6b20 6d6f 6462 7573  /modbustk modbus
+00002220: 5f74 6b5f 6578 616d 706c 652e 636f 6e66  _tk_example.conf
+00002230: 6967 0a20 2020 2060 6060 0a0a 312e 2041  ig.    ```..1. A
+00002240: 6464 2061 204d 6f64 6275 732d 544b 2052  dd a Modbus-TK R
+00002250: 6567 6973 7465 7220 4d61 7020 4353 5620  egister Map CSV 
+00002260: 4669 6c65 2074 6f20 7468 6520 506c 6174  File to the Plat
+00002270: 666f 726d 2044 7269 7665 722e 0a0a 2020  form Driver...  
+00002280: 2020 4d6f 6462 7573 2054 4b20 7265 7175    Modbus TK requ
+00002290: 6972 6573 2061 6e20 6164 6469 7469 6f6e  ires an addition
+000022a0: 616c 2072 6567 6973 7472 7920 636f 6e66  al registry conf
+000022b0: 6967 7572 6174 696f 6e20 6669 6c65 2063  iguration file c
+000022c0: 6f6d 7061 7265 6420 746f 2074 6865 2070  ompared to the p
+000022d0: 6172 6164 6967 6d20 6f66 206d 6f73 7420  aradigm of most 
+000022e0: 6f74 6865 7220 6472 6976 6572 732e 2054  other drivers. T
+000022f0: 6865 2072 6567 6973 7472 7920 6d61 7020  he registry map 
+00002300: 6669 6c65 2069 7320 616e 2061 6e61 6c6f  file is an analo
+00002310: 6775 6520 746f 2074 6865 2074 7970 6963  gue to the typic
+00002320: 616c 2072 6567 6973 7472 7920 636f 6e66  al registry conf
+00002330: 6967 7572 6174 696f 6e20 6669 6c65 2e20  iguration file. 
+00002340: 5468 6520 7265 6769 7374 7279 2063 6f6e  The registry con
+00002350: 6669 6775 7261 7469 6f6e 2066 696c 6520  figuration file 
+00002360: 6973 2061 2073 696d 706c 6520 6669 6c65  is a simple file
+00002370: 2077 6869 6368 206d 6170 7320 6465 7669   which maps devi
+00002380: 6365 2070 6f69 6e74 206e 616d 6573 2074  ce point names t
+00002390: 6f20 7573 6572 2073 7065 6369 6669 6564  o user specified
+000023a0: 2070 6f69 6e74 206e 616d 6573 2e0a 0a20   point names... 
+000023b0: 2020 2054 6869 7320 7265 706f 2070 726f     This repo pro
+000023c0: 7669 6465 7320 616e 2065 7861 6d70 6c65  vides an example
+000023d0: 2063 6f6e 6669 6775 7261 7469 6f6e 2069   configuration i
+000023e0: 6e20 7468 6520 6669 6c65 2022 6d6f 6462  n the file "modb
+000023f0: 7573 5f74 6b5f 7465 7374 5f6d 6170 2e63  us_tk_test_map.c
+00002400: 7376 222e 0a0a 2020 2020 5468 6520 7265  sv"...    The re
+00002410: 6769 7374 7279 206d 6170 2066 696c 6520  gistry map file 
+00002420: 6973 2061 2043 5356 2066 696c 652e 2045  is a CSV file. E
+00002430: 6163 6820 726f 7720 636f 6e66 6967 7572  ach row configur
+00002440: 6573 2061 2072 6567 6973 7465 7220 6465  es a register de
+00002450: 6669 6e69 7469 6f6e 206f 6e20 7468 6520  finition on the 
+00002460: 6465 7669 6365 2e0a 0a20 2020 2052 6567  device...    Reg
+00002470: 6973 7465 7220 4e61 6d65 2028 5265 7175  ister Name (Requ
+00002480: 6972 6564 2920 2d20 5468 6520 6669 656c  ired) - The fiel
+00002490: 6420 6e61 6d65 2069 6e20 7468 6520 6d6f  d name in the mo
+000024a0: 6462 7573 2063 6c69 656e 742e 2054 6869  dbus client. Thi
+000024b0: 7320 6669 656c 6420 6973 2064 6973 7469  s field is disti
+000024c0: 6e63 7420 616e 6420 756e 6368 616e 6765  nct and unchange
+000024d0: 6162 6c65 2e0a 0a20 2020 2041 6464 7265  able...    Addre
+000024e0: 7373 2028 5265 7175 6972 6564 2920 2d20  ss (Required) - 
+000024f0: 5468 6520 706f 696e 74e2 8099 7320 6d6f  The point...s mo
+00002500: 6462 7573 2061 6464 7265 7373 2e20 5468  dbus address. Th
+00002510: 6520 6164 6472 6573 7369 6e67 206f 7074  e addressing opt
+00002520: 696f 6e20 696e 2074 6865 2064 7269 7665  ion in the drive
+00002530: 7220 636f 6e66 6967 7572 6174 696f 6e20  r configuration 
+00002540: 636f 6e74 726f 6c73 2077 6865 7468 6572  controls whether
+00002550: 2074 6869 7320 6973 2069 6e74 6572 7072   this is interpr
+00002560: 6574 6564 2061 7320 616e 2065 7861 6374  eted as an exact
+00002570: 2061 6464 7265 7373 206f 7220 616e 206f   address or an o
+00002580: 6666 7365 742e 0a0a 2020 2020 5479 7065  ffset...    Type
+00002590: 2028 5265 7175 6972 6564 2920 2d20 5468   (Required) - Th
+000025a0: 6520 706f 696e 74e2 8099 7320 6461 7461  e point...s data
+000025b0: 2074 7970 653a 2062 6f6f 6c2c 2073 7472   type: bool, str
+000025c0: 696e 675b 6c65 6e67 7468 5d2c 2066 6c6f  ing[length], flo
+000025d0: 6174 2c20 696e 7431 362c 2069 6e74 3332  at, int16, int32
+000025e0: 2c20 696e 7436 342c 2075 696e 7431 362c  , int64, uint16,
+000025f0: 2075 696e 7433 322c 206f 7220 7569 6e74   uint32, or uint
+00002600: 3634 2e0a 0a20 2020 2055 6e69 7473 2028  64...    Units (
+00002610: 4f70 7469 6f6e 616c 2920 2d20 5573 6564  Optional) - Used
+00002620: 2066 6f72 206d 6574 6164 6174 6120 7768   for metadata wh
+00002630: 656e 2063 7265 6174 696e 6720 706f 696e  en creating poin
+00002640: 7420 696e 666f 726d 6174 696f 6e20 6f6e  t information on
+00002650: 2061 2068 6973 746f 7269 616e 2e20 4465   a historian. De
+00002660: 6661 756c 7420 6973 2061 6e20 656d 7074  fault is an empt
+00002670: 7920 7374 7269 6e67 2e0a 0a20 2020 2057  y string...    W
+00002680: 7269 7461 626c 6520 284f 7074 696f 6e61  ritable (Optiona
+00002690: 6c29 202d 2054 5255 452f 4641 4c53 452e  l) - TRUE/FALSE.
+000026a0: 204f 6e6c 7920 706f 696e 7473 2066 6f72   Only points for
+000026b0: 2077 6869 6368 2057 7269 7461 626c 653d   which Writable=
+000026c0: 5452 5545 2063 616e 2062 6520 7570 6461  TRUE can be upda
+000026d0: 7465 6420 6279 2061 2056 4f4c 5454 524f  ted by a VOLTTRO
+000026e0: 4e20 6167 656e 742e 2044 6566 6175 6c74  N agent. Default
+000026f0: 2069 7320 4641 4c53 452e 0a0a 2020 2020   is FALSE...    
+00002700: 4465 6661 756c 7420 5661 6c75 6520 284f  Default Value (O
+00002710: 7074 696f 6e61 6c29 202d 2054 6865 2070  ptional) - The p
+00002720: 6f69 6e74 e280 9973 2064 6566 6175 6c74  oint...s default
+00002730: 2076 616c 7565 2e20 4966 2069 7420 6973   value. If it is
+00002740: 2072 6576 6572 7465 6420 6279 2061 6e20   reverted by an 
+00002750: 6167 656e 742c 2069 7420 6368 616e 6765  agent, it change
+00002760: 7320 6261 636b 2074 6f20 7468 6973 2076  s back to this v
+00002770: 616c 7565 2e20 4966 2074 6869 7320 7661  alue. If this va
+00002780: 6c75 6520 6973 206d 6973 7369 6e67 2c20  lue is missing, 
+00002790: 6974 2077 696c 6c20 7265 7665 7274 2074  it will revert t
+000027a0: 6f20 7468 6520 6c61 7374 206b 6e6f 776e  o the last known
+000027b0: 2076 616c 7565 206e 6f74 2073 6574 2062   value not set b
+000027c0: 7920 616e 2061 6765 6e74 2e0a 0a20 2020  y an agent...   
+000027d0: 2054 7261 6e73 666f 726d 2028 4f70 7469   Transform (Opti
+000027e0: 6f6e 616c 2920 2d20 5363 616c 696e 6720  onal) - Scaling 
+000027f0: 616c 676f 7269 7468 6d3a 2073 6361 6c65  algorithm: scale
+00002800: 286d 756c 7469 706c 6965 7229 2c20 7363  (multiplier), sc
+00002810: 616c 655f 696e 7428 6d75 6c74 6970 6c69  ale_int(multipli
+00002820: 6572 292c 2073 6361 6c65 5f72 6567 2872  er), scale_reg(r
+00002830: 6567 6973 7465 725f 6e61 6d65 292c 2073  egister_name), s
+00002840: 6361 6c65 5f72 6567 5f70 6f77 6572 3130  cale_reg_power10
+00002850: 2872 6567 6973 7465 725f 6e61 6d65 292c  (register_name),
+00002860: 2073 6361 6c65 5f64 6563 696d 616c 5f69   scale_decimal_i
+00002870: 6e74 5f73 6967 6e65 6428 6d75 6c74 6970  nt_signed(multip
+00002880: 6c69 6572 292c 206d 6f64 3130 6b28 7265  lier), mod10k(re
+00002890: 7665 7273 6529 2c20 6d6f 6431 306b 3634  verse), mod10k64
+000028a0: 2872 6576 6572 7365 292c 206d 6f64 3130  (reverse), mod10
+000028b0: 6b34 3828 7265 7665 7265 7329 206f 7220  k48(reveres) or 
+000028c0: 6e6f 6e65 2e20 4465 6661 756c 7420 6973  none. Default is
+000028d0: 2061 6e20 656d 7074 7920 7374 7269 6e67   an empty string
+000028e0: 2e0a 0a20 2020 2054 6162 6c65 2028 4f70  ...    Table (Op
+000028f0: 7469 6f6e 616c 2920 2d20 5374 616e 6461  tional) - Standa
+00002900: 7264 206d 6f64 6275 7320 7461 626c 6520  rd modbus table 
+00002910: 6e61 6d65 2064 6566 696e 696e 6720 686f  name defining ho
+00002920: 7720 696e 666f 726d 6174 696f 6e20 6973  w information is
+00002930: 2073 746f 7265 6420 696e 2073 6c61 7665   stored in slave
+00002940: 2064 6576 6963 652e 2054 6865 7265 2061   device. There a
+00002950: 7265 2034 2064 6966 6665 7265 6e74 2074  re 4 different t
+00002960: 6162 6c65 733a 0a0a 2020 2020 6469 7363  ables:..    disc
+00002970: 7265 7465 5f6f 7574 7075 745f 636f 696c  rete_output_coil
+00002980: 733a 2072 6561 642f 7772 6974 6520 636f  s: read/write co
+00002990: 696c 206e 756d 6265 7273 2031 2d39 3939  il numbers 1-999
+000029a0: 390a 0a20 2020 2064 6973 6372 6574 655f  9..    discrete_
+000029b0: 696e 7075 745f 636f 6e74 6163 7473 3a20  input_contacts: 
+000029c0: 7265 6164 206f 6e6c 7920 636f 696c 206e  read only coil n
+000029d0: 756d 6265 7273 2031 3030 3031 2d31 3939  umbers 10001-199
+000029e0: 3939 0a0a 2020 2020 616e 616c 6f67 5f69  99..    analog_i
+000029f0: 6e70 7574 5f72 6567 6973 7465 7273 3a20  nput_registers: 
+00002a00: 7265 6164 206f 6e6c 7920 7265 6769 7374  read only regist
+00002a10: 6572 206e 756d 6265 7273 2033 3030 3031  er numbers 30001
+00002a20: 2d33 3939 3939 0a0a 2020 2020 616e 616c  -39999..    anal
+00002a30: 6f67 5f6f 7574 7075 745f 686f 6c64 696e  og_output_holdin
+00002a40: 675f 7265 6769 7374 6572 733a 2072 6561  g_registers: rea
+00002a50: 642f 7772 6974 6520 7265 6769 7374 6572  d/write register
+00002a60: 206e 756d 6265 7273 2034 3030 3031 2d34   numbers 40001-4
+00002a70: 3939 3939 0a0a 2020 2020 4966 2074 6869  9999..    If thi
+00002a80: 7320 6669 656c 6420 6973 2065 6d70 7479  s field is empty
+00002a90: 2c20 7468 6520 6d6f 6462 7573 2074 6162  , the modbus tab
+00002aa0: 6c65 2077 696c 6c20 6265 2064 6566 696e  le will be defin
+00002ab0: 6564 2062 7920 7479 7065 2061 6e64 2077  ed by type and w
+00002ac0: 7269 7461 626c 6520 6669 656c 6473 2e20  ritable fields. 
+00002ad0: 4279 2074 6861 742c 2077 6865 6e20 7573  By that, when us
+00002ae0: 6572 2073 6574 7320 7265 6164 206f 6e6c  er sets read onl
+00002af0: 7920 666f 7220 7265 6164 2f77 7269 7465  y for read/write
+00002b00: 2063 6f69 6c73 2f72 6567 6973 7465 7273   coils/registers
+00002b10: 206f 7220 7365 7473 2072 6561 642f 7772   or sets read/wr
+00002b20: 6974 6520 666f 7220 7265 6164 206f 6e6c  ite for read onl
+00002b30: 7920 636f 696c 732f 7265 6769 7374 6572  y coils/register
+00002b40: 732c 2069 7420 7769 6c6c 2073 656c 6563  s, it will selec
+00002b50: 7420 7772 6f6e 6720 7461 626c 652c 2061  t wrong table, a
+00002b60: 6e64 2074 6865 7265 666f 7265 2072 6169  nd therefore rai
+00002b70: 7365 2065 7863 6570 7469 6f6e 2e0a 0a20  se exception... 
+00002b80: 2020 204d 6978 6564 2045 6e64 6961 6e20     Mixed Endian 
+00002b90: 284f 7074 696f 6e61 6c29 202d 2054 5255  (Optional) - TRU
+00002ba0: 452f 4641 4c53 452e 2049 6620 4d69 7865  E/FALSE. If Mixe
+00002bb0: 6420 456e 6469 616e 2069 7320 7365 7420  d Endian is set 
+00002bc0: 746f 2054 5255 452c 2074 6865 206f 7264  to TRUE, the ord
+00002bd0: 6572 206f 6620 7468 6520 4d6f 6462 7573  er of the Modbus
+00002be0: 2072 6567 6973 7465 7273 2077 696c 6c20   registers will 
+00002bf0: 6265 2072 6576 6572 7365 6420 6265 666f  be reversed befo
+00002c00: 7265 2070 6172 7369 6e67 2074 6865 2076  re parsing the v
+00002c10: 616c 7565 206f 7220 7772 6974 696e 6720  alue or writing 
+00002c20: 6974 206f 7574 2074 6f20 7468 6520 6465  it out to the de
+00002c30: 7669 6365 2e20 4279 2073 6574 7469 6e67  vice. By setting
+00002c40: 206d 6978 6564 2065 6e64 6961 6e2c 2074   mixed endian, t
+00002c50: 7261 6e73 666f 726d 206d 7573 7420 6265  ransform must be
+00002c60: 204e 6f6e 6520 286e 6f20 6f70 292e 2044   None (no op). D
+00002c70: 6566 6175 6c74 7320 746f 2046 414c 5345  efaults to FALSE
+00002c80: 2e0a 0a20 2020 2044 6573 6372 6970 7469  ...    Descripti
+00002c90: 6f6e 2028 4f70 7469 6f6e 616c 2920 2d20  on (Optional) - 
+00002ca0: 4164 6469 7469 6f6e 616c 2069 6e66 6f72  Additional infor
+00002cb0: 6d61 7469 6f6e 2061 626f 7574 2074 6865  mation about the
+00002cc0: 2070 6f69 6e74 2e20 4465 6661 756c 7420   point. Default 
+00002cd0: 6973 2061 6e20 656d 7074 7920 7374 7269  is an empty stri
+00002ce0: 6e67 2e0a 0a20 2020 2048 6572 6520 6973  ng...    Here is
+00002cf0: 2061 2073 616d 706c 6520 4d6f 6462 7573   a sample Modbus
+00002d00: 2d54 4b20 7265 6769 7374 7279 206d 6170  -TK registry map
+00002d10: 3a0a 0a20 2020 2060 6060 6373 760a 2020  :..    ```csv.  
+00002d20: 2020 5265 6769 7374 6572 204e 616d 652c    Register Name,
+00002d30: 4164 6472 6573 732c 5479 7065 2c55 6e69  Address,Type,Uni
+00002d40: 7473 2c57 7269 7461 626c 652c 4465 6661  ts,Writable,Defa
+00002d50: 756c 7420 5661 6c75 652c 5472 616e 7366  ult Value,Transf
+00002d60: 6f72 6d2c 5461 626c 650a 2020 2020 756e  orm,Table.    un
+00002d70: 7369 676e 6564 5f73 686f 7274 2c30 2c75  signed_short,0,u
+00002d80: 696e 7431 362c 4e6f 6e65 2c54 5255 452c  int16,None,TRUE,
+00002d90: 302c 7363 616c 6528 3130 292c 616e 616c  0,scale(10),anal
+00002da0: 6f67 5f6f 7574 7075 745f 686f 6c64 696e  og_output_holdin
+00002db0: 675f 7265 6769 7374 6572 730a 2020 2020  g_registers.    
+00002dc0: 756e 7369 676e 6564 5f69 6e74 2c31 2c75  unsigned_int,1,u
+00002dd0: 696e 7433 322c 4e6f 6e65 2c54 5255 452c  int32,None,TRUE,
+00002de0: 302c 7363 616c 6528 3130 292c 616e 616c  0,scale(10),anal
+00002df0: 6f67 5f6f 7574 7075 745f 686f 6c64 696e  og_output_holdin
+00002e00: 675f 7265 6769 7374 6572 730a 2020 2020  g_registers.    
+00002e10: 756e 7369 676e 6564 5f6c 6f6e 672c 332c  unsigned_long,3,
+00002e20: 7569 6e74 3634 2c4e 6f6e 652c 5452 5545  uint64,None,TRUE
+00002e30: 2c30 2c73 6361 6c65 2831 3029 2c61 6e61  ,0,scale(10),ana
+00002e40: 6c6f 675f 6f75 7470 7574 5f68 6f6c 6469  log_output_holdi
+00002e50: 6e67 5f72 6567 6973 7465 7273 0a20 2020  ng_registers.   
+00002e60: 2073 616d 706c 655f 7368 6f72 742c 372c   sample_short,7,
+00002e70: 696e 7431 362c 4e6f 6e65 2c54 5255 452c  int16,None,TRUE,
+00002e80: 302c 7363 616c 6528 3130 292c 616e 616c  0,scale(10),anal
+00002e90: 6f67 5f6f 7574 7075 745f 686f 6c64 696e  og_output_holdin
+00002ea0: 675f 7265 6769 7374 6572 730a 2020 2020  g_registers.    
+00002eb0: 7361 6d70 6c65 5f69 6e74 2c38 2c69 6e74  sample_int,8,int
+00002ec0: 3332 2c4e 6f6e 652c 5452 5545 2c30 2c73  32,None,TRUE,0,s
+00002ed0: 6361 6c65 2831 3029 2c61 6e61 6c6f 675f  cale(10),analog_
+00002ee0: 6f75 7470 7574 5f68 6f6c 6469 6e67 5f72  output_holding_r
+00002ef0: 6567 6973 7465 7273 0a20 2020 2073 616d  egisters.    sam
+00002f00: 706c 655f 666c 6f61 742c 3130 2c66 6c6f  ple_float,10,flo
+00002f10: 6174 2c4e 6f6e 652c 5452 5545 2c30 2e30  at,None,TRUE,0.0
+00002f20: 2c73 6361 6c65 2831 3029 2c61 6e61 6c6f  ,scale(10),analo
+00002f30: 675f 6f75 7470 7574 5f68 6f6c 6469 6e67  g_output_holding
+00002f40: 5f72 6567 6973 7465 7273 0a20 2020 2073  _registers.    s
+00002f50: 616d 706c 655f 6c6f 6e67 2c31 322c 696e  ample_long,12,in
+00002f60: 7436 342c 4e6f 6e65 2c54 5255 452c 302c  t64,None,TRUE,0,
+00002f70: 7363 616c 6528 3130 292c 616e 616c 6f67  scale(10),analog
+00002f80: 5f6f 7574 7075 745f 686f 6c64 696e 675f  _output_holding_
+00002f90: 7265 6769 7374 6572 730a 2020 2020 7361  registers.    sa
+00002fa0: 6d70 6c65 5f62 6f6f 6c2c 3136 2c62 6f6f  mple_bool,16,boo
+00002fb0: 6c2c 4e6f 6e65 2c54 5255 452c 4661 6c73  l,None,TRUE,Fals
+00002fc0: 652c 2c61 6e61 6c6f 675f 6f75 7470 7574  e,,analog_output
+00002fd0: 5f68 6f6c 6469 6e67 5f72 6567 6973 7465  _holding_registe
+00002fe0: 7273 0a20 2020 2073 616d 706c 655f 7374  rs.    sample_st
+00002ff0: 722c 3137 2c73 7472 696e 675b 3132 5d2c  r,17,string[12],
+00003000: 4e6f 6e65 2c54 5255 452c 6865 6c6c 6f20  None,TRUE,hello 
+00003010: 776f 726c 6421 2c2c 616e 616c 6f67 5f6f  world!,,analog_o
+00003020: 7574 7075 745f 686f 6c64 696e 675f 7265  utput_holding_re
+00003030: 6769 7374 6572 730a 2020 2020 6060 600a  gisters.    ```.
+00003040: 0a20 2020 2041 6674 6572 2063 7265 6174  .    After creat
+00003050: 696e 6720 6120 7265 6769 7374 7279 206d  ing a registry m
+00003060: 6170 206e 616d 6564 2022 6d6f 6462 7573  ap named "modbus
+00003070: 5f74 6b5f 7465 7374 5f6d 6170 2e63 7376  _tk_test_map.csv
+00003080: 222c 2061 6464 2069 7420 746f 2074 6865  ", add it to the
+00003090: 2043 6f6e 6669 6775 7261 7469 6f6e 2053   Configuration S
+000030a0: 746f 7265 3a0a 0a20 2020 2060 6060 7368  tore:..    ```sh
+000030b0: 656c 6c0a 2020 2020 7663 746c 2063 6f6e  ell.    vctl con
+000030c0: 6669 6720 7374 6f72 6520 706c 6174 666f  fig store platfo
+000030d0: 726d 2e64 7269 7665 7220 6d6f 6462 7573  rm.driver modbus
+000030e0: 5f74 6b5f 7465 7374 5f6d 6170 2e63 7376  _tk_test_map.csv
+000030f0: 206d 6f64 6275 735f 746b 5f74 6573 745f   modbus_tk_test_
+00003100: 6d61 702e 6373 7620 2d2d 6373 760a 2020  map.csv --csv.  
+00003110: 2020 6060 600a 0a31 2e20 4164 6420 6120    ```..1. Add a 
+00003120: 7265 6769 7374 7279 2063 6f6e 6669 6775  registry configu
+00003130: 7261 7469 6f6e 2074 6f20 7468 6520 506c  ration to the Pl
+00003140: 6174 666f 726d 4472 6976 6572 2e0a 0a20  atformDriver... 
+00003150: 2020 2054 6865 2072 6567 6973 7472 7920     The registry 
+00003160: 636f 6e66 6967 7572 6174 696f 6e20 6669  configuration fi
+00003170: 6c65 2069 7320 6120 4353 5620 6669 6c65  le is a CSV file
+00003180: 2e20 4561 6368 2072 6f77 2063 6f6e 6669  . Each row confi
+00003190: 6775 7265 7320 6120 706f 696e 7420 6f6e  gures a point on
+000031a0: 2074 6865 2064 6576 6963 652e 0a0a 2020   the device...  
+000031b0: 2020 2020 2020 566f 6c74 7472 6f6e 2050        Volttron P
+000031c0: 6f69 6e74 204e 616d 6520 2852 6571 7569  oint Name (Requi
+000031d0: 7265 6429 202d 2054 6865 206e 616d 6520  red) - The name 
+000031e0: 6279 2077 6869 6368 2074 6865 2070 6c61  by which the pla
+000031f0: 7466 6f72 6d20 616e 6420 6167 656e 7473  tform and agents
+00003200: 2072 6566 6572 2074 6f20 7468 6520 706f   refer to the po
+00003210: 696e 742e 2046 6f72 2069 6e73 7461 6e63  int. For instanc
+00003220: 652c 2069 6620 7468 6520 566f 6c74 7472  e, if the Volttr
+00003230: 6f6e 2050 6f69 6e74 204e 616d 6520 6973  on Point Name is
+00003240: 2048 6561 7443 616c 6c31 2c20 7468 656e   HeatCall1, then
+00003250: 2061 6e20 6167 656e 7420 776f 756c 6420   an agent would 
+00003260: 7573 6520 6d79 5f63 616d 7075 732f 6275  use my_campus/bu
+00003270: 696c 6469 6e67 322f 6876 6163 312f 4865  ilding2/hvac1/He
+00003280: 6174 4361 6c6c 3120 746f 2072 6566 6572  atCall1 to refer
+00003290: 2074 6f20 7468 6520 706f 696e 7420 7768   to the point wh
+000032a0: 656e 2075 7369 6e67 2074 6865 2052 5043  en using the RPC
+000032b0: 2069 6e74 6572 6661 6365 206f 6620 7468   interface of th
+000032c0: 6520 6163 7475 6174 6f72 2061 6765 6e74  e actuator agent
+000032d0: 2e0a 0a20 2020 2020 2020 2052 6567 6973  ...        Regis
+000032e0: 7465 7220 4e61 6d65 2028 5265 7175 6972  ter Name (Requir
+000032f0: 6564 2920 2d20 5468 6520 6669 656c 6420  ed) - The field 
+00003300: 6e61 6d65 2069 6e20 7468 6520 6d6f 6462  name in the modb
+00003310: 7573 2063 6c69 656e 742e 2049 7420 6d75  us client. It mu
+00003320: 7374 2062 6520 6d61 7463 6865 6420 7769  st be matched wi
+00003330: 7468 2074 6865 2066 6965 6c64 206e 616d  th the field nam
+00003340: 6520 6672 6f6d 2072 6567 6973 7465 725f  e from register_
+00003350: 6d61 702e 0a0a 2020 2020 416e 7920 6164  map...    Any ad
+00003360: 6469 7469 6f6e 616c 2063 6f6c 756d 6e73  ditional columns
+00003370: 2077 696c 6c20 6f76 6572 7269 6465 2074   will override t
+00003380: 6865 2065 7869 7374 6564 2066 6965 6c64  he existed field
+00003390: 7320 6672 6f6d 2072 6567 6973 7465 725f  s from register_
+000033a0: 6d61 702e 0a0a 2020 2020 4865 7265 2069  map...    Here i
+000033b0: 7320 6120 7361 6d70 6c65 204d 6f64 6275  s a sample Modbu
+000033c0: 732d 544b 2072 6567 6973 7472 7920 636f  s-TK registry co
+000033d0: 6e66 6967 7572 6174 696f 6e20 7769 7468  nfiguration with
+000033e0: 2064 6566 696e 6564 2072 6567 6973 7465   defined registe
+000033f0: 725f 6d61 703a 0a0a 2020 2020 6060 6063  r_map:..    ```c
+00003400: 7376 0a20 2020 2056 6f6c 7474 726f 6e20  sv.    Volttron 
+00003410: 506f 696e 7420 4e61 6d65 2c52 6567 6973  Point Name,Regis
+00003420: 7465 7220 4e61 6d65 0a20 2020 2075 6e73  ter Name.    uns
+00003430: 6967 6e65 6420 7368 6f72 742c 756e 7369  igned short,unsi
+00003440: 676e 6564 5f73 686f 7274 0a20 2020 2075  gned_short.    u
+00003450: 6e73 6967 6e65 6420 696e 742c 756e 7369  nsigned int,unsi
+00003460: 676e 6564 5f69 6e74 0a20 2020 2075 6e73  gned_int.    uns
+00003470: 6967 6e65 6420 6c6f 6e67 2c75 6e73 6967  igned long,unsig
+00003480: 6e65 645f 6c6f 6e67 0a20 2020 2073 616d  ned_long.    sam
+00003490: 706c 6520 7368 6f72 742c 7361 6d70 6c65  ple short,sample
+000034a0: 5f73 686f 7274 0a20 2020 2073 616d 706c  _short.    sampl
+000034b0: 6520 696e 742c 7361 6d70 6c65 5f69 6e74  e int,sample_int
+000034c0: 0a20 2020 2073 616d 706c 6520 666c 6f61  .    sample floa
+000034d0: 742c 7361 6d70 6c65 5f66 6c6f 6174 0a20  t,sample_float. 
+000034e0: 2020 2073 616d 706c 6520 6c6f 6e67 2c73     sample long,s
+000034f0: 616d 706c 655f 6c6f 6e67 0a20 2020 2073  ample_long.    s
+00003500: 616d 706c 6520 626f 6f6c 2c73 616d 706c  ample bool,sampl
+00003510: 655f 626f 6f6c 0a20 2020 2073 616d 706c  e_bool.    sampl
+00003520: 6520 7374 722c 7361 6d70 6c65 5f73 7472  e str,sample_str
+00003530: 0a20 2020 2060 6060 0a0a 2020 2020 4166  .    ```..    Af
+00003540: 7465 7220 6372 6561 7469 6e67 2061 2072  ter creating a r
+00003550: 6567 6973 7472 7920 6d61 7020 6e61 6d65  egistry map name
+00003560: 6420 226d 6f64 6275 735f 746b 5f74 6573  d "modbus_tk_tes
+00003570: 742e 6373 7622 2c20 6164 6420 6974 2074  t.csv", add it t
+00003580: 6f20 7468 6520 436f 6e66 6967 7572 6174  o the Configurat
+00003590: 696f 6e20 5374 6f72 653a 0a0a 2020 2020  ion Store:..    
+000035a0: 6060 6073 6865 6c6c 0a20 2020 2076 6374  ```shell.    vct
+000035b0: 6c20 636f 6e66 6967 2073 746f 7265 2070  l config store p
+000035c0: 6c61 7466 6f72 6d2e 6472 6976 6572 206d  latform.driver m
+000035d0: 6f64 6275 735f 746b 5f74 6573 742e 6373  odbus_tk_test.cs
+000035e0: 7620 6d6f 6462 7573 5f74 6b5f 7465 7374  v modbus_tk_test
+000035f0: 2e63 7376 202d 2d63 7376 0a20 2020 2060  .csv --csv.    `
+00003600: 6060 0a0a 312e 204f 6273 6572 7665 2044  ``..1. Observe D
+00003610: 6174 610a 0a20 2020 2054 6f20 7365 6520  ata..    To see 
+00003620: 6461 7461 2062 6569 6e67 2070 7562 6c69  data being publi
+00003630: 7368 6564 2074 6f20 7468 6520 6275 732c  shed to the bus,
+00003640: 2069 6e73 7461 6c6c 2061 205b 4c69 7374   install a [List
+00003650: 656e 6572 2041 6765 6e74 5d28 6874 7470  ener Agent](http
+00003660: 733a 2f2f 7079 7069 2e6f 7267 2f70 726f  s://pypi.org/pro
+00003670: 6a65 6374 2f76 6f6c 7474 726f 6e2d 6c69  ject/volttron-li
+00003680: 7374 656e 6572 2f29 3a0a 0a20 2020 2060  stener/):..    `
+00003690: 6060 0a20 2020 2076 6374 6c20 696e 7374  ``.    vctl inst
+000036a0: 616c 6c20 766f 6c74 7472 6f6e 2d6c 6973  all volttron-lis
+000036b0: 7465 6e65 7220 2d2d 7374 6172 740a 2020  tener --start.  
+000036c0: 2020 6060 600a 0a20 2020 204f 6e63 6520    ```..    Once 
+000036d0: 696e 7374 616c 6c65 642c 2079 6f75 2073  installed, you s
+000036e0: 686f 756c 6420 7365 6520 7468 6520 6461  hould see the da
+000036f0: 7461 2062 6569 6e67 2070 7562 6c69 7368  ta being publish
+00003700: 6564 2062 7920 7669 6577 696e 6720 7468  ed by viewing th
+00003710: 6520 566f 6c74 7472 6f6e 206c 6f67 7320  e Volttron logs 
+00003720: 6669 6c65 2074 6861 7420 7761 7320 6372  file that was cr
+00003730: 6561 7465 6420 696e 2073 7465 7020 322e  eated in step 2.
+00003740: 0a20 2020 2054 6f20 7761 7463 6820 7468  .    To watch th
+00003750: 6520 6c6f 6773 2c20 6f70 656e 2061 2073  e logs, open a s
+00003760: 6570 6172 6174 6520 7465 726d 696e 616c  eparate terminal
+00003770: 2061 6e64 2072 756e 2074 6865 2066 6f6c   and run the fol
+00003780: 6c6f 7769 6e67 2063 6f6d 6d61 6e64 3a0a  lowing command:.
+00003790: 0a20 2020 2060 6060 0a20 2020 2074 6169  .    ```.    tai
+000037a0: 6c20 2d66 203c 7061 7468 2074 6f20 666f  l -f <path to fo
+000037b0: 6c64 6572 2063 6f6e 7461 696e 696e 6720  lder containing 
+000037c0: 766f 6c74 7472 6f6e 2e6c 6f67 3e2f 766f  volttron.log>/vo
+000037d0: 6c74 7472 6f6e 2e6c 6f67 0a20 2020 2060  lttron.log.    `
+000037e0: 6060 0a0a 2320 4d6f 6462 7573 2d54 4b20  ``..# Modbus-TK 
+000037f0: 436f 6e66 6967 2043 6f6d 6d61 6e64 2054  Config Command T
+00003800: 6f6f 6c0a 0a60 636f 6e66 6967 5f63 6d64  ool..`config_cmd
+00003810: 2e70 7960 2069 7320 6120 636f 6d6d 616e  .py` is a comman
+00003820: 642d 6c69 6e65 2074 6f6f 6c20 666f 7220  d-line tool for 
+00003830: 6372 6561 7469 6e67 2061 6e64 206d 6169  creating and mai
+00003840: 6e74 6169 6e69 6e67 2056 4f4c 5454 524f  ntaining VOLTTRO
+00003850: 4e20 6472 6976 6572 2063 6f6e 6669 6775  N driver configu
+00003860: 7261 7469 6f6e 732e 2054 6865 2074 6f6f  rations. The too
+00003870: 6c20 7275 6e73 2066 726f 6d20 7468 6520  l runs from the 
+00003880: 636f 6d6d 616e 6420 6c69 6e65 3a0a 0a63  command line:..c
+00003890: 6f6e 6669 675f 636d 642e 7079 2073 7570  onfig_cmd.py sup
+000038a0: 706f 7274 7320 7468 6520 666f 6c6c 6f77  ports the follow
+000038b0: 696e 6720 636f 6d6d 616e 6473 3a0a 0a2a  ing commands:..*
+000038c0: 2068 656c 7020 2d20 4c69 7374 2061 6c6c   help - List all
+000038d0: 2063 6f6d 6d61 6e64 732e 0a0a 2a20 7175   commands...* qu
+000038e0: 6974 202d 2051 7569 7420 7468 6520 636f  it - Quit the co
+000038f0: 6d6d 616e 642d 6c69 6e65 2074 6f6f 6c2e  mmand-line tool.
+00003900: 0a0a 2a20 6c69 7374 5f64 6972 6563 746f  ..* list_directo
+00003910: 7269 6573 202d 204c 6973 7420 616c 6c20  ries - List all 
+00003920: 7365 7475 7020 6469 7265 6374 6f72 6965  setup directorie
+00003930: 732c 2077 6974 6820 616e 206f 7074 696f  s, with an optio
+00003940: 6e20 746f 2065 6469 7420 7468 6569 7220  n to edit their 
+00003950: 7061 7468 732e 0a0a 0a42 7920 6465 6661  paths....By defa
+00003960: 756c 742c 2061 6c6c 2064 6972 6563 746f  ult, all directo
+00003970: 7269 6573 2061 7265 2069 6e20 7468 6973  ries are in this
+00003980: 2072 6570 6f20 6174 2074 6865 2066 6f6c   repo at the fol
+00003990: 6c6f 7769 6e67 2066 6f6c 6465 723a 2076  lowing folder: v
+000039a0: 6f6c 7474 726f 6e2f 6472 6976 6572 2f69  olttron/driver/i
+000039b0: 6e74 6572 6661 6365 732f 6d6f 6462 7573  nterfaces/modbus
+000039c0: 5f74 6b2f 7574 696c 732f 6d61 7073 2e0a  _tk/utils/maps..
+000039d0: 0a49 7420 6973 2069 6d70 6f72 7461 6e74  .It is important
+000039e0: 2074 6f20 7573 6520 7468 6520 636f 7272   to use the corr
+000039f0: 6563 7420 6469 7265 6374 6f72 6965 7320  ect directories 
+00003a00: 7768 656e 2061 6464 696e 672f 6564 6974  when adding/edit
+00003a10: 696e 6720 6465 7669 6365 2074 7970 6573  ing device types
+00003a20: 2061 6e64 2064 7269 7665 7220 636f 6e66   and driver conf
+00003a30: 6967 732c 2061 6e64 2077 6865 6e20 6c6f  igs, and when lo
+00003a40: 6164 696e 6720 636f 6e66 6967 7572 6174  ading configurat
+00003a50: 696f 6e73 2069 6e74 6f20 564f 4c54 5452  ions into VOLTTR
+00003a60: 4f4e 2e0a 0a2a 206d 6170 5f64 6972 3a20  ON...* map_dir: 
+00003a70: 6469 7265 6374 6f72 7920 696e 2077 6869  directory in whi
+00003a80: 6368 206d 6170 732e 7961 6d6c 2069 7320  ch maps.yaml is 
+00003a90: 7374 6f72 6564 2e0a 0a2a 2063 6f6e 6669  stored...* confi
+00003aa0: 675f 6469 723a 2064 6972 6563 746f 7279  g_dir: directory
+00003ab0: 2069 6e20 7768 6963 6820 6472 6976 6572   in which driver
+00003ac0: 2063 6f6e 6669 6720 6669 6c65 7320 6172   config files ar
+00003ad0: 6520 7374 6f72 6564 2e0a 0a2a 2063 7376  e stored...* csv
+00003ae0: 5f64 6972 3a20 6469 7265 6374 6f72 7920  _dir: directory 
+00003af0: 696e 2077 6869 6368 2072 6567 6973 7472  in which registr
+00003b00: 7920 636f 6e66 6967 2043 5356 2066 696c  y config CSV fil
+00003b10: 6573 2061 7265 2073 746f 7265 642e 0a0a  es are stored...
+00003b20: 2a20 6564 6974 5f64 6972 6563 746f 7269  * edit_directori
+00003b30: 6573 202d 2041 6464 2f45 6469 7420 6d61  es - Add/Edit ma
+00003b40: 7020 6469 7265 6374 6f72 792c 2064 7269  p directory, dri
+00003b50: 7665 7220 636f 6e66 6967 2064 6972 6563  ver config direc
+00003b60: 746f 7279 2c20 616e 642f 6f72 2043 5356  tory, and/or CSV
+00003b70: 2063 6f6e 6669 6720 6469 7265 6374 6f72   config director
+00003b80: 792e 2050 7265 7373 203c 456e 7465 723e  y. Press <Enter>
+00003b90: 2069 6620 6e6f 2063 6861 6e67 6520 6973   if no change is
+00003ba0: 206e 6565 6465 642e 2045 7869 7473 2069   needed. Exits i
+00003bb0: 6620 7468 6520 6469 7265 6374 6f72 7920  f the directory 
+00003bc0: 646f 6573 206e 6f74 2065 7869 7374 2e0a  does not exist..
+00003bd0: 0a2a 206c 6973 745f 6465 7669 6365 5f74  .* list_device_t
+00003be0: 7970 655f 6465 7363 7269 7074 696f 6e20  ype_description 
+00003bf0: 2d20 4c69 7374 2061 6c6c 2064 6576 6963  - List all devic
+00003c00: 6520 7479 7065 2064 6573 6372 6970 7469  e type descripti
+00003c10: 6f6e 7320 696e 206d 6170 732e 7961 6d6c  ons in maps.yaml
+00003c20: 2e20 4f70 7469 6f6e 2074 6f20 6564 6974  . Option to edit
+00003c30: 2064 6576 6963 6520 7479 7065 2064 6573   device type des
+00003c40: 6372 6970 7469 6f6e 732e 0a0a 2a20 6c69  criptions...* li
+00003c50: 7374 5f61 6c6c 5f64 6576 6963 655f 7479  st_all_device_ty
+00003c60: 7065 7320 2d20 4c69 7374 2061 6c6c 2064  pes - List all d
+00003c70: 6576 6963 6520 7479 7065 2069 6e66 6f72  evice type infor
+00003c80: 6d61 7469 6f6e 2069 6e20 6d61 7073 2e79  mation in maps.y
+00003c90: 616d 6c2e 204f 7074 696f 6e20 746f 2061  aml. Option to a
+00003ca0: 6464 206d 6f72 6520 6465 7669 6365 2074  dd more device t
+00003cb0: 7970 6573 2e0a 0a2a 2064 6576 6963 655f  ypes...* device_
+00003cc0: 7479 7065 202d 204c 6973 7420 696e 666f  type - List info
+00003cd0: 726d 6174 696f 6e20 666f 7220 6120 7365  rmation for a se
+00003ce0: 6c65 6374 6564 2064 6576 6963 6520 7479  lected device ty
+00003cf0: 7065 2e20 4f70 7469 6f6e 2074 6f20 7365  pe. Option to se
+00003d00: 6c65 6374 2061 6e6f 7468 6572 2064 6576  lect another dev
+00003d10: 6963 6520 7479 7065 2e0a 0a2a 2061 6464  ice type...* add
+00003d20: 5f64 6576 6963 655f 7479 7065 202d 2041  _device_type - A
+00003d30: 6464 2061 2064 6576 6963 6520 7479 7065  dd a device type
+00003d40: 2074 6f20 6d61 7073 2e79 616d 6c2e 204f   to maps.yaml. O
+00003d50: 7074 696f 6e20 746f 2061 6464 206d 6f72  ption to add mor
+00003d60: 6520 7468 616e 206f 6e65 2064 6576 6963  e than one devic
+00003d70: 6520 7479 7065 2e20 4561 6368 2064 6576  e type. Each dev
+00003d80: 6963 6520 7479 7065 2069 6e63 6c75 6465  ice type include
+00003d90: 7320 6974 7320 6e61 6d65 2c20 4353 5620  s its name, CSV 
+00003da0: 6669 6c65 2c20 6465 7363 7269 7074 696f  file, descriptio
+00003db0: 6e2c 2061 6464 7265 7373 696e 672c 2061  n, addressing, a
+00003dc0: 6e64 2065 6e64 6961 6e2c 2061 7320 6578  nd endian, as ex
+00003dd0: 706c 6169 6e65 6420 696e 204d 4f44 4255  plained in MODBU
+00003de0: 532d 544b 2044 7269 7665 7220 4d61 7073  S-TK Driver Maps
+00003df0: 2e20 4966 2061 6e20 696e 7661 6c69 6420  . If an invalid 
+00003e00: 7661 6c75 6520 6973 2065 6e74 6572 6564  value is entered
+00003e10: 2066 6f72 2061 6464 7265 7373 696e 6720   for addressing 
+00003e20: 6f72 2065 6e64 6961 6e2c 2074 6865 2064  or endian, the d
+00003e30: 6566 6175 6c74 2076 616c 7565 2069 7320  efault value is 
+00003e40: 7573 6564 2069 6e73 7465 6164 2e0a 0a2a  used instead...*
+00003e50: 6564 6974 5f64 6576 6963 655f 7479 7065  edit_device_type
+00003e60: 202d 2045 6469 7420 616e 2065 7869 7374   - Edit an exist
+00003e70: 696e 6720 6465 7669 6365 2074 7970 652e  ing device type.
+00003e80: 2049 6620 616e 2069 6e76 616c 6964 2076   If an invalid v
+00003e90: 616c 7565 2069 7320 656e 7465 7265 6420  alue is entered 
+00003ea0: 666f 7220 6164 6472 6573 7369 6e67 206f  for addressing o
+00003eb0: 7220 656e 6469 616e 2c20 7468 6520 7072  r endian, the pr
+00003ec0: 6576 696f 7573 2076 616c 7565 2069 7320  evious value is 
+00003ed0: 6c65 6674 2075 6e63 6861 6e67 6564 2e0a  left unchanged..
+00003ee0: 0a2a 206c 6973 745f 6472 6976 6572 7320  .* list_drivers 
+00003ef0: 2d20 4c69 7374 2061 6c6c 2064 7269 7665  - List all drive
+00003f00: 7220 636f 6e66 6967 206e 616d 6573 2069  r config names i
+00003f10: 6e20 636f 6e66 6967 5f64 6972 2e0a 0a2a  n config_dir...*
+00003f20: 2064 7269 7665 725f 636f 6e66 6967 203c   driver_config <
+00003f30: 6472 6976 6572 5f6e 616d 653e 202d 2047  driver_name> - G
+00003f40: 6574 2061 2064 7269 7665 7220 636f 6e66  et a driver conf
+00003f50: 6967 2066 726f 6d20 636f 6e66 6967 5f64  ig from config_d
+00003f60: 6972 2e20 4f70 7469 6f6e 2074 6f20 7365  ir. Option to se
+00003f70: 6c65 6374 2074 6865 2064 7269 7665 7220  lect the driver 
+00003f80: 6966 206e 6f20 6472 6976 6572 2069 7320  if no driver is 
+00003f90: 666f 756e 6420 7769 7468 2074 6861 7420  found with that 
+00003fa0: 6e61 6d65 2e0a 0a2a 2061 6464 5f64 7269  name...* add_dri
+00003fb0: 7665 725f 636f 6e66 6967 203c 6472 6976  ver_config <driv
+00003fc0: 6572 5f6e 616d 653e 202d 2041 6464 2f45  er_name> - Add/E
+00003fd0: 6469 7420 3c63 6f6e 6669 675f 6469 723e  dit <config_dir>
+00003fe0: 2f3c 6472 6976 6572 206e 616d 653e 2e63  /<driver name>.c
+00003ff0: 6f6e 6669 672e 204f 7074 696f 6e20 746f  onfig. Option to
+00004000: 2073 656c 6563 7420 7468 6520 6472 6976   select the driv
+00004010: 6572 2069 6620 6e6f 2064 7269 7665 7220  er if no driver 
+00004020: 6973 2066 6f75 6e64 2077 6974 6820 7468  is found with th
+00004030: 6174 206e 616d 652e 2050 7265 7373 203c  at name. Press <
+00004040: 456e 7465 723e 2074 6f20 6578 6974 2e0a  Enter> to exit..
+00004050: 0a2a 206c 6f61 645f 766f 6c74 7472 6f6e  .* load_volttron
+00004060: 202d 204c 6f61 6420 6120 6472 6976 6572   - Load a driver
+00004070: 2063 6f6e 6669 6720 616e 6420 4353 5620   config and CSV 
+00004080: 696e 746f 2056 4f4c 5454 524f 4e2e 204f  into VOLTTRON. O
+00004090: 7074 696f 6e20 746f 2061 6464 2074 6865  ption to add the
+000040a0: 2063 6f6e 6669 6720 6f72 2043 5356 2066   config or CSV f
+000040b0: 696c 6520 746f 2063 6f6e 6669 675f 6469  ile to config_di
+000040c0: 7220 6f72 2074 6f20 6373 765f 6469 722e  r or to csv_dir.
+000040d0: 2056 4f4c 5454 524f 4e20 6d75 7374 2062   VOLTTRON must b
+000040e0: 6520 7275 6e6e 696e 6720 7768 656e 2074  e running when t
+000040f0: 6869 7320 636f 6d6d 616e 6420 6973 2075  his command is u
+00004100: 7365 642e 0a0a 2a20 6465 6c65 7465 5f76  sed...* delete_v
+00004110: 6f6c 7474 726f 6e5f 636f 6e66 6967 202d  olttron_config -
+00004120: 2044 656c 6574 6520 6120 6472 6976 6572   Delete a driver
+00004130: 2063 6f6e 6669 6720 6672 6f6d 2056 4f4c   config from VOL
+00004140: 5454 524f 4e2e 2056 4f4c 5454 524f 4e20  TTRON. VOLTTRON 
+00004150: 6d75 7374 2062 6520 7275 6e6e 696e 6720  must be running 
+00004160: 7768 656e 2074 6869 7320 636f 6d6d 616e  when this comman
+00004170: 6420 6973 2075 7365 642e 0a0a 2a20 6465  d is used...* de
+00004180: 6c65 7465 5f76 6f6c 7474 726f 6e5f 6373  lete_volttron_cs
+00004190: 7620 2d20 4465 6c65 7465 2061 2072 6567  v - Delete a reg
+000041a0: 6973 7472 7920 6373 7620 636f 6e66 6967  istry csv config
+000041b0: 2066 726f 6d20 564f 4c54 5452 4f4e 2e20   from VOLTTRON. 
+000041c0: 564f 4c54 5452 4f4e 206d 7573 7420 6265  VOLTTRON must be
+000041d0: 2072 756e 6e69 6e67 2077 6865 6e20 7468   running when th
+000041e0: 6973 2063 6f6d 6d61 6e64 2069 7320 7573  is command is us
+000041f0: 6564 2e0a 0a23 2044 6576 656c 6f70 6d65  ed...# Developme
+00004200: 6e74 0a0a 506c 6561 7365 2073 6565 2074  nt..Please see t
+00004210: 6865 2066 6f6c 6c6f 7769 6e67 2066 6f72  he following for
+00004220: 2063 6f6e 7472 6962 7574 696e 6720 6775   contributing gu
+00004230: 6964 656c 696e 6573 205b 636f 6e74 7269  idelines [contri
+00004240: 6275 7469 6e67 5d28 6874 7470 733a 2f2f  buting](https://
+00004250: 6769 7468 7562 2e63 6f6d 2f65 636c 6970  github.com/eclip
+00004260: 7365 2d76 6f6c 7474 726f 6e2f 766f 6c74  se-volttron/volt
+00004270: 7472 6f6e 2d63 6f72 652f 626c 6f62 2f64  tron-core/blob/d
+00004280: 6576 656c 6f70 2f43 4f4e 5452 4942 5554  evelop/CONTRIBUT
+00004290: 494e 472e 6d64 292e 0a0a 506c 6561 7365  ING.md)...Please
+000042a0: 2073 6565 2074 6865 2066 6f6c 6c6f 7769   see the followi
+000042b0: 6e67 2068 656c 7066 756c 2067 7569 6465  ng helpful guide
+000042c0: 2061 626f 7574 205b 6465 7665 6c6f 7069   about [developi
+000042d0: 6e67 206d 6f64 756c 6172 2056 4f4c 5454  ng modular VOLTT
+000042e0: 524f 4e20 6167 656e 7473 5d28 6874 7470  RON agents](http
+000042f0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f65  s://github.com/e
+00004300: 636c 6970 7365 2d76 6f6c 7474 726f 6e2f  clipse-volttron/
+00004310: 766f 6c74 7472 6f6e 2d63 6f72 652f 626c  volttron-core/bl
+00004320: 6f62 2f64 6576 656c 6f70 2f44 4556 454c  ob/develop/DEVEL
+00004330: 4f50 494e 475f 4f4e 5f4d 4f44 554c 4152  OPING_ON_MODULAR
+00004340: 2e6d 6429 0a0a 0a23 2044 6973 636c 6169  .md)...# Disclai
+00004350: 6d65 7220 4e6f 7469 6365 0a0a 5468 6973  mer Notice..This
+00004360: 206d 6174 6572 6961 6c20 7761 7320 7072   material was pr
+00004370: 6570 6172 6564 2061 7320 616e 2061 6363  epared as an acc
+00004380: 6f75 6e74 206f 6620 776f 726b 2073 706f  ount of work spo
+00004390: 6e73 6f72 6564 2062 7920 616e 2061 6765  nsored by an age
+000043a0: 6e63 7920 6f66 2074 6865 0a55 6e69 7465  ncy of the.Unite
+000043b0: 6420 5374 6174 6573 2047 6f76 6572 6e6d  d States Governm
+000043c0: 656e 742e 2020 4e65 6974 6865 7220 7468  ent.  Neither th
+000043d0: 6520 556e 6974 6564 2053 7461 7465 7320  e United States 
+000043e0: 476f 7665 726e 6d65 6e74 206e 6f72 2074  Government nor t
+000043f0: 6865 2055 6e69 7465 640a 5374 6174 6573  he United.States
+00004400: 2044 6570 6172 746d 656e 7420 6f66 2045   Department of E
+00004410: 6e65 7267 792c 206e 6f72 2042 6174 7465  nergy, nor Batte
+00004420: 6c6c 652c 206e 6f72 2061 6e79 206f 6620  lle, nor any of 
+00004430: 7468 6569 7220 656d 706c 6f79 6565 732c  their employees,
+00004440: 206e 6f72 2061 6e79 0a6a 7572 6973 6469   nor any.jurisdi
+00004450: 6374 696f 6e20 6f72 206f 7267 616e 697a  ction or organiz
+00004460: 6174 696f 6e20 7468 6174 2068 6173 2063  ation that has c
+00004470: 6f6f 7065 7261 7465 6420 696e 2074 6865  ooperated in the
+00004480: 2064 6576 656c 6f70 6d65 6e74 206f 6620   development of 
+00004490: 7468 6573 650a 6d61 7465 7269 616c 732c  these.materials,
+000044a0: 206d 616b 6573 2061 6e79 2077 6172 7261   makes any warra
+000044b0: 6e74 792c 2065 7870 7265 7373 206f 7220  nty, express or 
+000044c0: 696d 706c 6965 642c 206f 7220 6173 7375  implied, or assu
+000044d0: 6d65 7320 616e 7920 6c65 6761 6c0a 6c69  mes any legal.li
+000044e0: 6162 696c 6974 7920 6f72 2072 6573 706f  ability or respo
+000044f0: 6e73 6962 696c 6974 7920 666f 7220 7468  nsibility for th
+00004500: 6520 6163 6375 7261 6379 2c20 636f 6d70  e accuracy, comp
+00004510: 6c65 7465 6e65 7373 2c20 6f72 2075 7365  leteness, or use
+00004520: 6675 6c6e 6573 7320 6f72 2061 6e79 0a69  fulness or any.i
+00004530: 6e66 6f72 6d61 7469 6f6e 2c20 6170 7061  nformation, appa
+00004540: 7261 7475 732c 2070 726f 6475 6374 2c20  ratus, product, 
+00004550: 736f 6674 7761 7265 2c20 6f72 2070 726f  software, or pro
+00004560: 6365 7373 2064 6973 636c 6f73 6564 2c20  cess disclosed, 
+00004570: 6f72 2072 6570 7265 7365 6e74 730a 7468  or represents.th
+00004580: 6174 2069 7473 2075 7365 2077 6f75 6c64  at its use would
+00004590: 206e 6f74 2069 6e66 7269 6e67 6520 7072   not infringe pr
+000045a0: 6976 6174 656c 7920 6f77 6e65 6420 7269  ivately owned ri
+000045b0: 6768 7473 2e0a 0a52 6566 6572 656e 6365  ghts...Reference
+000045c0: 2068 6572 6569 6e20 746f 2061 6e79 2073   herein to any s
+000045d0: 7065 6369 6669 6320 636f 6d6d 6572 6369  pecific commerci
+000045e0: 616c 2070 726f 6475 6374 2c20 7072 6f63  al product, proc
+000045f0: 6573 732c 206f 7220 7365 7276 6963 6520  ess, or service 
+00004600: 6279 0a74 7261 6465 206e 616d 652c 2074  by.trade name, t
+00004610: 7261 6465 6d61 726b 2c20 6d61 6e75 6661  rademark, manufa
+00004620: 6374 7572 6572 2c20 6f72 206f 7468 6572  cturer, or other
+00004630: 7769 7365 2064 6f65 7320 6e6f 7420 6e65  wise does not ne
+00004640: 6365 7373 6172 696c 790a 636f 6e73 7469  cessarily.consti
+00004650: 7475 7465 206f 7220 696d 706c 7920 6974  tute or imply it
+00004660: 7320 656e 646f 7273 656d 656e 742c 2072  s endorsement, r
+00004670: 6563 6f6d 6d65 6e64 6174 696f 6e2c 206f  ecommendation, o
+00004680: 7220 6661 766f 7269 6e67 2062 7920 7468  r favoring by th
+00004690: 6520 556e 6974 6564 0a53 7461 7465 7320  e United.States 
+000046a0: 476f 7665 726e 6d65 6e74 206f 7220 616e  Government or an
+000046b0: 7920 6167 656e 6379 2074 6865 7265 6f66  y agency thereof
+000046c0: 2c20 6f72 2042 6174 7465 6c6c 6520 4d65  , or Battelle Me
+000046d0: 6d6f 7269 616c 2049 6e73 7469 7475 7465  morial Institute
+000046e0: 2e20 5468 650a 7669 6577 7320 616e 6420  . The.views and 
+000046f0: 6f70 696e 696f 6e73 206f 6620 6175 7468  opinions of auth
+00004700: 6f72 7320 6578 7072 6573 7365 6420 6865  ors expressed he
+00004710: 7265 696e 2064 6f20 6e6f 7420 6e65 6365  rein do not nece
+00004720: 7373 6172 696c 7920 7374 6174 6520 6f72  ssarily state or
+00004730: 0a72 6566 6c65 6374 2074 686f 7365 206f  .reflect those o
+00004740: 6620 7468 6520 556e 6974 6564 2053 7461  f the United Sta
+00004750: 7465 7320 476f 7665 726e 6d65 6e74 206f  tes Government o
+00004760: 7220 616e 7920 6167 656e 6379 2074 6865  r any agency the
+00004770: 7265 6f66 2e0a 0a                        reof...
```

