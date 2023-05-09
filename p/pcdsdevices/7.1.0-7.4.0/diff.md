# Comparing `tmp/pcdsdevices-7.1.0.tar.gz` & `tmp/pcdsdevices-7.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pcdsdevices-7.1.0.tar", last modified: Tue Nov  8 01:58:33 2022, max compression
+gzip compressed data, was "pcdsdevices-7.4.0.tar", last modified: Tue May  9 00:02:58 2023, max compression
```

## Comparing `pcdsdevices-7.1.0.tar` & `pcdsdevices-7.4.0.tar`

### file list

```diff
@@ -1,217 +1,278 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-11-08 01:58:33.366795 pcdsdevices-7.1.0/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2468 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/LICENSE.md
--rw-rw-r--   0 travis    (2000) travis    (2000)      253 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)      224 2022-11-08 01:58:33.366795 pcdsdevices-7.1.0/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     2827 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/README.md
--rw-rw-r--   0 travis    (2000) travis    (2000)       40 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/dev-requirements.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/docs-requirements.txt
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-11-08 01:58:33.366795 pcdsdevices-7.1.0/pcdsdevices/
--rw-rw-r--   0 travis    (2000) travis    (2000)      820 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1425 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/_html.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      497 2022-11-08 01:58:33.370793 pcdsdevices-7.1.0/pcdsdevices/_version.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7887 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/analog_signals.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-11-08 01:58:33.354801 pcdsdevices-7.1.0/pcdsdevices/areadetector/
--rw-rw-r--   0 travis    (2000) travis    (2000)      137 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/areadetector/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6132 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/areadetector/cam.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    17900 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/areadetector/detectors.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6459 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/areadetector/plugins.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2860 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/atm.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    52575 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/attenuator.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    12442 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/beam_stats.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    39266 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/ccm.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      190 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/component.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6410 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/crix_motion.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2077 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/cvmi_motion.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3410 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/dc_devices.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3668 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/delay_generator.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    17685 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/device.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2189 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/device_types.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    30560 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/digitizers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1970 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/doc_stubs.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1452 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/energy_monitor.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    48029 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/epics_motor.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1451 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/evr.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    16504 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/gauge.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    22654 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/gon.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-11-08 01:58:33.354801 pcdsdevices-7.1.0/pcdsdevices/happi/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/happi/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    28992 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/happi/containers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9123 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/inout.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    64181 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/interface.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    19462 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/ipm.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3114 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/jet.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4264 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/lamp_motion.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-11-08 01:58:33.354801 pcdsdevices-7.1.0/pcdsdevices/lasers/
--rw-rw-r--   0 travis    (2000) travis    (2000)      231 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/lasers/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    19743 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/lasers/btms_config.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    22945 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/lasers/btps.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1546 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/lasers/counters.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1368 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/lasers/dicon.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1342 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/lasers/ek9000.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5259 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/lasers/elliptec.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4446 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/lasers/qmini.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    15460 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/lasers/rfof.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4132 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/lasers/thorlabsWFS.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5563 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/lasers/tuttifrutti.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1978 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/lasers/zoomtelescope.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    21112 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/lens.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1244 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/lic.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      839 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/light_control.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    73216 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/lodcm.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    16678 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/lxe.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6021 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/make_ophyd_device.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    48111 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/mirror.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      877 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/movablestand.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8077 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/mpod.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     8327 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/mpod_apalis.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7641 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/mps.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1170 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/mrco_motion.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      241 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/mv_interface.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3120 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/piezo.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    20273 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/pim.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      957 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/pmps.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7324 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/positioner.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    38988 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/pseudopos.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6901 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/pulsepicker.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    15271 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/pump.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5607 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/pv_positioner.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      645 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/radiation.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1722 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/ref.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      114 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/registry.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2269 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/rs_powersupply.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2439 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/rtds_ebd.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11767 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/sample_delivery.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1363 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/sensors.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11909 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/sequencer.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    58220 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/signal.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3214 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/sim.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    25872 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/slits.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    15570 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/spectrometer.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    29135 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/state.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6245 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/stopper.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1211 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/sxr_test_absorber.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      380 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/tags.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    48282 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/targets.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-11-08 01:58:33.362797 pcdsdevices-7.1.0/pcdsdevices/tests/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/tests/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7927 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/tests/conftest.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3583 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/tests/test_analog_signals.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      249 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/tests/test_atm.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5353 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/tests/test_attenuator.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4656 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/tests/test_beam_stats.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    14530 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/tests/test_btms.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10004 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/tests/test_ccm.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2270 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/tests/test_crix_motion.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      758 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/tests/test_dc_devices.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6658 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/tests/test_device.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       81 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/tests/test_device_types.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1034 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/tests/test_disconnected.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    18227 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/tests/test_epics_motor.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      497 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/tests/test_evr.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1812 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/tests/test_gauge.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8662 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/tests/test_gon.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2532 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/tests/test_inout.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9560 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/tests/test_interface.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5782 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/tests/test_ipm.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      971 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/tests/test_jet.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5696 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/tests/test_lens.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-11-08 01:58:33.362797 pcdsdevices-7.1.0/pcdsdevices/tests/test_lens_sets/
--rw-rw-r--   0 travis    (2000) travis    (2000)       26 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/tests/test_lens_sets/original.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)       22 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/tests/test_lens_sets/test
--rw-rw-r--   0 travis    (2000) travis    (2000)       26 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/tests/test_lens_sets/test.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)      243 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/tests/test_lic.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    19101 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/tests/test_lodcm.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9693 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/tests/test_lxe.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4986 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/tests/test_mirror.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      581 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/tests/test_movablestand.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4925 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/tests/test_mpod.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4079 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/tests/test_mpod_apalis.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3113 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/tests/test_mps.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4157 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/tests/test_pim.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2637 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/tests/test_positioner.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6499 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/tests/test_pseudopos.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4270 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/tests/test_pulsepicker.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1125 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/tests/test_pump.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      237 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/tests/test_ref.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5738 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/tests/test_sample_delivery.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5249 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/tests/test_sequencer.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    16240 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/tests/test_signal.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4421 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/tests/test_slits.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1352 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/tests/test_spectrometer.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10923 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/tests/test_state.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    17155 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/tests/test_targets.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1703 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/tests/test_timetool.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      207 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/tests/test_ui.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7503 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/tests/test_utils.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3147 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/tests/test_valve.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10713 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/tests/test_variety.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      255 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/tests/test_wfs.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      605 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/tests/xcslt8717_wpcalib_opa
--rw-rw-r--   0 travis    (2000) travis    (2000)     2294 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/timetool.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      954 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/type_hints.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-11-08 01:58:33.366795 pcdsdevices-7.1.0/pcdsdevices/ui/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2418 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/ui/AT2L0.detailed.ui
--rw-rw-r--   0 travis    (2000) travis    (2000)     2418 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/ui/AT2L0.embedded.ui
--rw-rw-r--   0 travis    (2000) travis    (2000)     5902 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/ui/AttenuatorCalculatorSXR_Blade.embedded.ui
--rw-rw-r--   0 travis    (2000) travis    (2000)     6586 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/ui/AttenuatorCalculatorSXR_Blade_config.embedded.ui
--rw-rw-r--   0 travis    (2000) travis    (2000)     4934 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/ui/AttenuatorCalculatorSXR_FourBlade.detailed.ui
--rw-rw-r--   0 travis    (2000) travis    (2000)     3251 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/ui/AttenuatorCalculatorSXR_FourBlade.ui
--rw-rw-r--   0 travis    (2000) travis    (2000)     6218 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/ui/AttenuatorCalculatorSXR_FourBlade_all_filters.ui
--rw-rw-r--   0 travis    (2000) travis    (2000)     6388 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/ui/AttenuatorCalculatorSXR_FourBlade_blade_all_filters.ui
--rw-rw-r--   0 travis    (2000) travis    (2000)    25452 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/ui/AttenuatorCalculatorSXR_FourBlade_calc.ui
--rw-rw-r--   0 travis    (2000) travis    (2000)     5729 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/ui/AttenuatorCalculatorSXR_FourBlade_filters.ui
--rw-rw-r--   0 travis    (2000) travis    (2000)    18911 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/ui/AttenuatorCalculatorSXR_FourBlade_overview.ui
--rw-rw-r--   0 travis    (2000) travis    (2000)     3949 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/ui/AttenuatorCalculator_AT2L0.detailed.ui
--rw-rw-r--   0 travis    (2000) travis    (2000)     3237 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/ui/AttenuatorCalculator_AT2L0.ui
--rw-rw-r--   0 travis    (2000) travis    (2000)    17847 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/ui/AttenuatorCalculator_AT2L0_calc.ui
--rw-rw-r--   0 travis    (2000) travis    (2000)     3916 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/ui/AttenuatorCalculator_AT2L0_filters.ui
--rw-rw-r--   0 travis    (2000) travis    (2000)    15571 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/ui/AttenuatorCalculator_AT2L0_overview.ui
--rw-rw-r--   0 travis    (2000) travis    (2000)     5918 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/ui/AttenuatorCalculator_filter.ui
--rw-rw-r--   0 travis    (2000) travis    (2000)     2418 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/ui/AttenuatorSXR_Ladder.detailed.ui
--rw-rw-r--   0 travis    (2000) travis    (2000)     2418 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/ui/AttenuatorSXR_Ladder.embedded.ui
--rw-rw-r--   0 travis    (2000) travis    (2000)     9614 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/ui/BeckhoffAxis.detailed.ui
--rw-rw-r--   0 travis    (2000) travis    (2000)     3268 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/ui/BeckhoffAxis.embedded.ui
--rw-rw-r--   0 travis    (2000) travis    (2000)    41696 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/ui/BeckhoffSlits.detailed.ui
--rw-rw-r--   0 travis    (2000) travis    (2000)    25557 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/ui/BeckhoffSlits.embedded.ui
--rw-rw-r--   0 travis    (2000) travis    (2000)    12365 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/ui/BtpsState.detailed.ui
--rw-rw-r--   0 travis    (2000) travis    (2000)    12365 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/ui/BtpsState.embedded.ui
--rw-rw-r--   0 travis    (2000) travis    (2000)    60307 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/ui/JJSlits.detailed.ui
--rw-rw-r--   0 travis    (2000) travis    (2000)     5052 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/ui/LightControl.ui
--rw-rw-r--   0 travis    (2000) travis    (2000)    51167 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/ui/PowerSlits.detailed.ui
--rw-rw-r--   0 travis    (2000) travis    (2000)    34999 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/ui/PowerSlits.embedded.ui
--rw-rw-r--   0 travis    (2000) travis    (2000)    24349 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/ui/QminiSpectrometer.embedded.ui
--rw-rw-r--   0 travis    (2000) travis    (2000)    10488 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/ui/QuadraticBeckhoffMotor.detailed.ui
--rw-rw-r--   0 travis    (2000) travis    (2000)     4220 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/ui/QuadraticBeckhoffMotor.embedded.ui
--rw-rw-r--   0 travis    (2000) travis    (2000)    10138 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/ui/StatePositioner.detailed.ui
--rw-rw-r--   0 travis    (2000) travis    (2000)     3795 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/ui/StatePositioner.embedded.ui
--rw-rw-r--   0 travis    (2000) travis    (2000)    10236 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/ui/TwinCATStatePositioner.detailed.ui
--rw-rw-r--   0 travis    (2000) travis    (2000)     3891 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/ui/TwinCATStatePositioner.embedded.ui
--rw-rw-r--   0 travis    (2000) travis    (2000)      156 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/ui/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      325 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/ui/at2l0_filters.json
--rw-rw-r--   0 travis    (2000) travis    (2000)    15242 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/ui/btps-camera-summary.ui
--rw-rw-r--   0 travis    (2000) travis    (2000)    12171 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/ui/btps-config.ui
--rw-rw-r--   0 travis    (2000) travis    (2000)    33295 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/ui/btps-overview.ui
--rw-rw-r--   0 travis    (2000) travis    (2000)    12410 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/ui/btps-range-config.ui
--rw-rw-r--   0 travis    (2000) travis    (2000)     9784 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/ui/btps-range-summary.ui
--rw-rw-r--   0 travis    (2000) travis    (2000)    46416 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/ui/btps-source-dest.ui
--rw-rw-r--   0 travis    (2000) travis    (2000)     4749 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/ui/btps-source-tabs-config.ui
--rw-rw-r--   0 travis    (2000) travis    (2000)     5766 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/ui/btps-source-tabs.ui
--rw-rw-r--   0 travis    (2000) travis    (2000)     3074 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/ui/btps-source-valves.ui
--rw-rw-r--   0 travis    (2000) travis    (2000)    12365 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/ui/btps.ui
--rw-rw-r--   0 travis    (2000) travis    (2000)     2418 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/ui/detailed_tree.ui
--rw-rw-r--   0 travis    (2000) travis    (2000)     1776 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/usb_encoder.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    27920 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/utils.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    18486 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/valve.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9018 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/variety.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1689 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/pcdsdevices/wfs.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2022-11-08 01:58:33.354801 pcdsdevices-7.1.0/pcdsdevices.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)      224 2022-11-08 01:58:33.000000 pcdsdevices-7.1.0/pcdsdevices.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     6607 2022-11-08 01:58:33.000000 pcdsdevices-7.1.0/pcdsdevices.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2022-11-08 01:58:33.000000 pcdsdevices-7.1.0/pcdsdevices.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      109 2022-11-08 01:58:33.000000 pcdsdevices-7.1.0/pcdsdevices.egg-info/entry_points.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      166 2022-11-08 01:58:33.000000 pcdsdevices-7.1.0/pcdsdevices.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       12 2022-11-08 01:58:33.000000 pcdsdevices-7.1.0/pcdsdevices.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      166 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/requirements.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      297 2022-11-08 01:58:33.366795 pcdsdevices-7.1.0/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)      777 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/setup.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    68576 2022-11-08 01:58:18.000000 pcdsdevices-7.1.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 00:02:58.789744 pcdsdevices-7.4.0/
+-rw-r--r--   0 runner    (1001) docker     (122)      142 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (122)      161 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/.flake8
+-rw-r--r--   0 runner    (1001) docker     (122)      125 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       32 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 00:02:58.745744 pcdsdevices-7.4.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (122)     1062 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1213 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 00:02:58.745744 pcdsdevices-7.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)      786 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/.github/workflows/standard.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      159 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (122)      790 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      174 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     3032 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     2468 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (122)      253 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     5747 2023-05-09 00:02:58.789744 pcdsdevices-7.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2590 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 00:02:58.745744 pcdsdevices-7.4.0/conda-recipe/
+-rw-r--r--   0 runner    (1001) docker     (122)     1265 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/conda-recipe/meta.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       40 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 00:02:58.745744 pcdsdevices-7.4.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (122)      739 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/docs/Makefile
+-rwxr-xr-x   0 runner    (1001) docker     (122)      901 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/docs/pre-release-notes.sh
+-rw-r--r--   0 runner    (1001) docker     (122)     3431 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/docs/release_notes.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 00:02:58.749744 pcdsdevices-7.4.0/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (122)     1009 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/docs/source/README.inc
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 00:02:58.741744 pcdsdevices-7.4.0/docs/source/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 00:02:58.749744 pcdsdevices-7.4.0/docs/source/_templates/autosummary/
+-rw-r--r--   0 runner    (1001) docker     (122)      106 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/docs/source/_templates/autosummary/base.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     2108 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/docs/source/_templates/autosummary/class.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      717 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/docs/source/_templates/autosummary/module.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    29251 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/docs/source/api.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     2695 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/docs/source/base_classes.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     8755 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (122)      343 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      925 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/docs/source/mv.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     2706 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/docs/source/presets.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    77002 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/docs/source/releases.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    12052 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/docs/source/signals.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      207 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/docs/source/sim_types.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      764 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/docs/source/tab.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      405 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/docs/source/ui.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      108 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/docs/source/upcoming_changes.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 00:02:58.749744 pcdsdevices-7.4.0/docs/source/upcoming_release_notes/
+-rw-r--r--   0 runner    (1001) docker     (122)     1360 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/docs/source/upcoming_release_notes/template-full.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      249 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/docs/source/upcoming_release_notes/template-short.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1661 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/docs/update_api_list.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)       43 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/docs/view-build.sh
+-rw-r--r--   0 runner    (1001) docker     (122)      167 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/docs-requirements.txt
+-rwxr-xr-x   0 runner    (1001) docker     (122)      168 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/make_ophyd_device
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 00:02:58.761744 pcdsdevices-7.4.0/pcdsdevices/
+-rw-r--r--   0 runner    (1001) docker     (122)      774 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1425 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/_html.py
+-rw-r--r--   0 runner    (1001) docker     (122)      160 2023-05-09 00:02:58.000000 pcdsdevices-7.4.0/pcdsdevices/_version.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7887 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/analog_signals.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 00:02:58.765744 pcdsdevices-7.4.0/pcdsdevices/areadetector/
+-rw-r--r--   0 runner    (1001) docker     (122)      175 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/areadetector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5220 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/areadetector/cam.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19375 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/areadetector/detectors.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6459 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/areadetector/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2860 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/atm.py
+-rw-r--r--   0 runner    (1001) docker     (122)    60210 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/attenuator.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12442 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/beam_stats.py
+-rw-r--r--   0 runner    (1001) docker     (122)    39229 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/ccm.py
+-rw-r--r--   0 runner    (1001) docker     (122)      186 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/component.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6406 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/crix_motion.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2077 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/cvmi_motion.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3410 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/dc_devices.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3664 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/delay_generator.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17619 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/device.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2189 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/device_types.py
+-rw-r--r--   0 runner    (1001) docker     (122)    30560 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/digitizers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1970 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/doc_stubs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1452 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/energy_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (122)    51429 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/epics_motor.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1451 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/evr.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14511 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/fms.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16504 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/gauge.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22654 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/gon.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 00:02:58.765744 pcdsdevices-7.4.0/pcdsdevices/happi/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/happi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    29150 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/happi/containers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9121 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/inout.py
+-rw-r--r--   0 runner    (1001) docker     (122)    64069 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/interface.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19459 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/ipm.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3114 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/jet.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4264 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/lamp_motion.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 00:02:58.765744 pcdsdevices-7.4.0/pcdsdevices/lasers/
+-rw-r--r--   0 runner    (1001) docker     (122)      231 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/lasers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19804 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/lasers/btms_config.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22910 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/lasers/btps.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1546 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/lasers/counters.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1368 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/lasers/dicon.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1342 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/lasers/ek9000.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5767 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/lasers/elliptec.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4446 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/lasers/qmini.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15417 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/lasers/rfof.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4132 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/lasers/thorlabsWFS.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5563 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/lasers/tuttifrutti.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1978 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/lasers/zoomtelescope.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21112 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/lens.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1244 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/lic.py
+-rw-r--r--   0 runner    (1001) docker     (122)      839 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/light_control.py
+-rw-r--r--   0 runner    (1001) docker     (122)    74029 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/lodcm.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16653 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/lxe.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6005 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/make_ophyd_device.py
+-rw-r--r--   0 runner    (1001) docker     (122)    49040 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/mirror.py
+-rw-r--r--   0 runner    (1001) docker     (122)      877 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/movablestand.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8077 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/mpod.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     8327 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/mpod_apalis.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7637 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/mps.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1170 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/mrco_motion.py
+-rw-r--r--   0 runner    (1001) docker     (122)      241 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/mv_interface.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3120 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/piezo.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20301 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/pim.py
+-rw-r--r--   0 runner    (1001) docker     (122)      957 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/pmps.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3267 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/pneumatic.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7358 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/positioner.py
+-rw-r--r--   0 runner    (1001) docker     (122)    39960 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/pseudopos.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6901 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/pulsepicker.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15271 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/pump.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5607 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/pv_positioner.py
+-rw-r--r--   0 runner    (1001) docker     (122)      645 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/radiation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1722 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/ref.py
+-rw-r--r--   0 runner    (1001) docker     (122)      114 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/registry.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2665 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/rs_powersupply.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3328 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/rtds_ebd.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11767 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/sample_delivery.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1363 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/sensors.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11909 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/sequencer.py
+-rw-r--r--   0 runner    (1001) docker     (122)    58121 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/signal.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3214 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/sim.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26203 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/slits.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15582 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/spectrometer.py
+-rw-r--r--   0 runner    (1001) docker     (122)    29013 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/state.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6245 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/stopper.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1211 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/sxr_test_absorber.py
+-rw-r--r--   0 runner    (1001) docker     (122)      380 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/tags.py
+-rw-r--r--   0 runner    (1001) docker     (122)    48269 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/targets.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 00:02:58.777744 pcdsdevices-7.4.0/pcdsdevices/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7915 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3583 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/tests/test_analog_signals.py
+-rw-r--r--   0 runner    (1001) docker     (122)      249 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/tests/test_atm.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5851 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/tests/test_attenuator.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4656 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/tests/test_beam_stats.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14520 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/tests/test_btms.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10004 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/tests/test_ccm.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2270 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/tests/test_crix_motion.py
+-rw-r--r--   0 runner    (1001) docker     (122)      758 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/tests/test_dc_devices.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6658 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/tests/test_device.py
+-rw-r--r--   0 runner    (1001) docker     (122)       81 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/tests/test_device_types.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1034 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/tests/test_disconnected.py
+-rw-r--r--   0 runner    (1001) docker     (122)      868 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/tests/test_entrypoints.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18227 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/tests/test_epics_motor.py
+-rw-r--r--   0 runner    (1001) docker     (122)      497 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/tests/test_evr.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1812 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/tests/test_gauge.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8654 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/tests/test_gon.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2532 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/tests/test_inout.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9560 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/tests/test_interface.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5780 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/tests/test_ipm.py
+-rw-r--r--   0 runner    (1001) docker     (122)      971 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/tests/test_jet.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5692 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/tests/test_lens.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 00:02:58.777744 pcdsdevices-7.4.0/pcdsdevices/tests/test_lens_sets/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/tests/test_lens_sets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)       26 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/tests/test_lens_sets/original.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       23 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/tests/test_lens_sets/test
+-rw-r--r--   0 runner    (1001) docker     (122)       26 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/tests/test_lens_sets/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)      243 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/tests/test_lic.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19101 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/tests/test_lodcm.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9693 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/tests/test_lxe.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4986 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/tests/test_mirror.py
+-rw-r--r--   0 runner    (1001) docker     (122)      581 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/tests/test_movablestand.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4925 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/tests/test_mpod.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4079 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/tests/test_mpod_apalis.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3113 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/tests/test_mps.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4155 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/tests/test_pim.py
+-rw-r--r--   0 runner    (1001) docker     (122)      678 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/tests/test_pneumatic.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2629 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/tests/test_positioner.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9239 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/tests/test_pseudopos.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4270 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/tests/test_pulsepicker.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1125 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/tests/test_pump.py
+-rw-r--r--   0 runner    (1001) docker     (122)      237 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/tests/test_ref.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5738 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/tests/test_sample_delivery.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5215 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/tests/test_sequencer.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16240 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/tests/test_signal.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4421 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/tests/test_slits.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1352 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/tests/test_spectrometer.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10914 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/tests/test_state.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17153 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/tests/test_targets.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1703 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/tests/test_timetool.py
+-rw-r--r--   0 runner    (1001) docker     (122)      207 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/tests/test_ui.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7478 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3147 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/tests/test_valve.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10913 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/tests/test_variety.py
+-rw-r--r--   0 runner    (1001) docker     (122)      255 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/tests/test_wfs.py
+-rw-r--r--   0 runner    (1001) docker     (122)      605 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/tests/xcslt8717_wpcalib_opa
+-rw-r--r--   0 runner    (1001) docker     (122)     2294 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/timetool.py
+-rw-r--r--   0 runner    (1001) docker     (122)      935 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/type_hints.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 00:02:58.789744 pcdsdevices-7.4.0/pcdsdevices/ui/
+-rw-r--r--   0 runner    (1001) docker     (122)     2418 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/ui/AT1K2.detailed.ui
+-rw-r--r--   0 runner    (1001) docker     (122)     2418 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/ui/AT1K2.embedded.ui
+-rw-r--r--   0 runner    (1001) docker     (122)     2418 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/ui/AT2L0.detailed.ui
+-rw-r--r--   0 runner    (1001) docker     (122)     2418 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/ui/AT2L0.embedded.ui
+-rw-r--r--   0 runner    (1001) docker     (122)     5902 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/ui/AttenuatorCalculatorSXR_Blade.embedded.ui
+-rw-r--r--   0 runner    (1001) docker     (122)     6586 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/ui/AttenuatorCalculatorSXR_Blade_config.embedded.ui
+-rw-r--r--   0 runner    (1001) docker     (122)     4934 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/ui/AttenuatorCalculatorSXR_FourBlade.detailed.ui
+-rw-r--r--   0 runner    (1001) docker     (122)     3251 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/ui/AttenuatorCalculatorSXR_FourBlade.ui
+-rw-r--r--   0 runner    (1001) docker     (122)     6218 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/ui/AttenuatorCalculatorSXR_FourBlade_all_filters.ui
+-rw-r--r--   0 runner    (1001) docker     (122)     6388 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/ui/AttenuatorCalculatorSXR_FourBlade_blade_all_filters.ui
+-rw-r--r--   0 runner    (1001) docker     (122)    25452 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/ui/AttenuatorCalculatorSXR_FourBlade_calc.ui
+-rw-r--r--   0 runner    (1001) docker     (122)     5729 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/ui/AttenuatorCalculatorSXR_FourBlade_filters.ui
+-rw-r--r--   0 runner    (1001) docker     (122)    18911 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/ui/AttenuatorCalculatorSXR_FourBlade_overview.ui
+-rw-r--r--   0 runner    (1001) docker     (122)     4930 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/ui/AttenuatorCalculatorSXR_TwoBlade.detailed.ui
+-rw-r--r--   0 runner    (1001) docker     (122)     3249 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/ui/AttenuatorCalculatorSXR_TwoBlade.ui
+-rw-r--r--   0 runner    (1001) docker     (122)     4876 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/ui/AttenuatorCalculatorSXR_TwoBlade_all_filters.ui
+-rw-r--r--   0 runner    (1001) docker     (122)     2066 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/ui/AttenuatorCalculatorSXR_TwoBlade_blade_all_filters.ui
+-rw-r--r--   0 runner    (1001) docker     (122)    22407 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/ui/AttenuatorCalculatorSXR_TwoBlade_calc.ui
+-rw-r--r--   0 runner    (1001) docker     (122)     4753 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/ui/AttenuatorCalculatorSXR_TwoBlade_filters.ui
+-rw-r--r--   0 runner    (1001) docker     (122)    14678 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/ui/AttenuatorCalculatorSXR_TwoBlade_overview.ui
+-rw-r--r--   0 runner    (1001) docker     (122)     3949 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/ui/AttenuatorCalculator_AT2L0.detailed.ui
+-rw-r--r--   0 runner    (1001) docker     (122)     3237 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/ui/AttenuatorCalculator_AT2L0.ui
+-rw-r--r--   0 runner    (1001) docker     (122)    17847 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/ui/AttenuatorCalculator_AT2L0_calc.ui
+-rw-r--r--   0 runner    (1001) docker     (122)     3916 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/ui/AttenuatorCalculator_AT2L0_filters.ui
+-rw-r--r--   0 runner    (1001) docker     (122)    15571 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/ui/AttenuatorCalculator_AT2L0_overview.ui
+-rw-r--r--   0 runner    (1001) docker     (122)     5918 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/ui/AttenuatorCalculator_filter.ui
+-rw-r--r--   0 runner    (1001) docker     (122)     2418 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/ui/AttenuatorSXR_Ladder.detailed.ui
+-rw-r--r--   0 runner    (1001) docker     (122)     2418 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/ui/AttenuatorSXR_Ladder.embedded.ui
+-rw-r--r--   0 runner    (1001) docker     (122)     9614 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/ui/BeckhoffAxis.detailed.ui
+-rw-r--r--   0 runner    (1001) docker     (122)     3268 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/ui/BeckhoffAxis.embedded.ui
+-rw-r--r--   0 runner    (1001) docker     (122)    41696 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/ui/BeckhoffSlits.detailed.ui
+-rw-r--r--   0 runner    (1001) docker     (122)    25557 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/ui/BeckhoffSlits.embedded.ui
+-rw-r--r--   0 runner    (1001) docker     (122)    12365 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/ui/BtpsState.detailed.ui
+-rw-r--r--   0 runner    (1001) docker     (122)    12365 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/ui/BtpsState.embedded.ui
+-rw-r--r--   0 runner    (1001) docker     (122)    60307 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/ui/JJSlits.detailed.ui
+-rw-r--r--   0 runner    (1001) docker     (122)     8513 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/ui/LCP.detailed.ui
+-rw-r--r--   0 runner    (1001) docker     (122)     4685 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/ui/Leviton1.detailed.ui
+-rw-r--r--   0 runner    (1001) docker     (122)     5052 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/ui/LightControl.ui
+-rw-r--r--   0 runner    (1001) docker     (122)    51167 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/ui/PowerSlits.detailed.ui
+-rw-r--r--   0 runner    (1001) docker     (122)    34999 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/ui/PowerSlits.embedded.ui
+-rw-r--r--   0 runner    (1001) docker     (122)    24349 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/ui/QminiSpectrometer.embedded.ui
+-rw-r--r--   0 runner    (1001) docker     (122)    10488 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/ui/QuadraticBeckhoffMotor.detailed.ui
+-rw-r--r--   0 runner    (1001) docker     (122)     4220 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/ui/QuadraticBeckhoffMotor.embedded.ui
+-rw-r--r--   0 runner    (1001) docker     (122)    22511 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/ui/Setra5000.detailed.ui
+-rw-r--r--   0 runner    (1001) docker     (122)    10138 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/ui/StatePositioner.detailed.ui
+-rw-r--r--   0 runner    (1001) docker     (122)     3795 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/ui/StatePositioner.embedded.ui
+-rw-r--r--   0 runner    (1001) docker     (122)    10236 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/ui/TwinCATStatePositioner.detailed.ui
+-rw-r--r--   0 runner    (1001) docker     (122)     3891 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/ui/TwinCATStatePositioner.embedded.ui
+-rw-r--r--   0 runner    (1001) docker     (122)      156 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      325 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/ui/at2l0_filters.json
+-rw-r--r--   0 runner    (1001) docker     (122)    15242 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/ui/btps-camera-summary.ui
+-rw-r--r--   0 runner    (1001) docker     (122)    12171 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/ui/btps-config.ui
+-rw-r--r--   0 runner    (1001) docker     (122)    33295 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/ui/btps-overview.ui
+-rw-r--r--   0 runner    (1001) docker     (122)    12410 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/ui/btps-range-config.ui
+-rw-r--r--   0 runner    (1001) docker     (122)     9784 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/ui/btps-range-summary.ui
+-rw-r--r--   0 runner    (1001) docker     (122)    46416 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/ui/btps-source-dest.ui
+-rw-r--r--   0 runner    (1001) docker     (122)     4749 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/ui/btps-source-tabs-config.ui
+-rw-r--r--   0 runner    (1001) docker     (122)     5766 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/ui/btps-source-tabs.ui
+-rw-r--r--   0 runner    (1001) docker     (122)     3074 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/ui/btps-source-valves.ui
+-rw-r--r--   0 runner    (1001) docker     (122)    12365 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/ui/btps.ui
+-rw-r--r--   0 runner    (1001) docker     (122)     2418 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/ui/detailed_tree.ui
+-rw-r--r--   0 runner    (1001) docker     (122)     1776 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/usb_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (122)    27787 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23272 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/valve.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9015 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/variety.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1913 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/version.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1689 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pcdsdevices/wfs.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-09 00:02:58.761744 pcdsdevices-7.4.0/pcdsdevices.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     5747 2023-05-09 00:02:58.000000 pcdsdevices-7.4.0/pcdsdevices.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     8262 2023-05-09 00:02:58.000000 pcdsdevices-7.4.0/pcdsdevices.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-09 00:02:58.000000 pcdsdevices-7.4.0/pcdsdevices.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      109 2023-05-09 00:02:58.000000 pcdsdevices-7.4.0/pcdsdevices.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      339 2023-05-09 00:02:58.000000 pcdsdevices-7.4.0/pcdsdevices.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       12 2023-05-09 00:02:58.000000 pcdsdevices-7.4.0/pcdsdevices.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1210 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)      196 2023-05-09 00:02:40.000000 pcdsdevices-7.4.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-09 00:02:58.789744 pcdsdevices-7.4.0/setup.cfg
```

### Comparing `pcdsdevices-7.1.0/LICENSE.md` & `pcdsdevices-7.4.0/LICENSE.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2018, The Board of Trustees of the Leland Stanford Junior
+Copyright (c) 2023, The Board of Trustees of the Leland Stanford Junior
 University, through SLAC National Accelerator Laboratory (subject to receipt
 of any required approvals from the U.S. Dept. of Energy). All rights reserved.
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 (1) Redistributions of source code must retain the above copyright notice,
     this list of conditions and the following disclaimer.
```

### Comparing `pcdsdevices-7.1.0/README.md` & `pcdsdevices-7.4.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -5,23 +5,14 @@
 </div>
 
 <p align="center">
   <a href="#motivation">Motivation</a> •
   <a href="#installation">Installation</a>
 </p>
 
-<div align="center">
-  <!-- Build Status -->
-  <a href="https://travis-ci.org/pcdshub/pcdsdevices">
-    <img
-src="https://img.shields.io/travis/pcdshub/pcdsdevices/master.svg?style=flat-square"
-      alt="Build Status" />
-  </a>
-</div>
-
 ## Motivation
 
 Ophyd presents a uniform set of abstractions for EPICS devices. Many devices at
 the LCLS are covered by ophyd-provided classes such as ``EpicsMotor`` and
 ``AreaDetector``, but there are also many more custom and unique devices.
 
 This repository:
```

#### html2text {}

```diff
@@ -1,11 +1,10 @@
                           ****** PCDS Devices ******
          Collection of Ophyd Device subclasses for IOCs unique to PCDS
                           Motivation â¢ Installation
-                                 [Build_Status]
 ## Motivation Ophyd presents a uniform set of abstractions for EPICS devices.
 Many devices at the LCLS are covered by ophyd-provided classes such as
 ``EpicsMotor`` and ``AreaDetector``, but there are also many more custom and
 unique devices. This repository: * Defines unique device classes required by
 the LCLS, referenced by happi and our [device_config](https://github.com/
 pcdshub/device_config/) database. * Offers LCLS-tailored solutions for
 functionality not provided by ophyd * Provides essential tools to aid in the
```

### Comparing `pcdsdevices-7.1.0/pcdsdevices/__init__.py` & `pcdsdevices-7.4.0/pcdsdevices/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Hacky ophyd and pyepics hotfixes
 import epics.ca
 from ophyd.device import Device
 
-from ._version import get_versions
 from .registry import device_registry  # NOQA
+from .version import __version__  # noqa: F401
 
 
 def __contains__(self, value):
     return value in self._OphydAttrList__internal_list()
 
 
 Device.OphydAttrList.__contains__ = __contains__
@@ -29,10 +29,7 @@
     epics.ca.BYTES2STR = make_new_bts(epics.ca.BYTES2STR)
     epics.ca.bytes2str = make_new_bts(epics.ca.bytes2str)
 except AttributeError:
     pass
 
 del epics
 del make_new_bts
-
-__version__ = get_versions()['version']
-del get_versions
```

### Comparing `pcdsdevices-7.1.0/pcdsdevices/_html.py` & `pcdsdevices-7.4.0/pcdsdevices/_html.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.1.0/pcdsdevices/analog_signals.py` & `pcdsdevices-7.4.0/pcdsdevices/analog_signals.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.1.0/pcdsdevices/areadetector/cam.py` & `pcdsdevices-7.4.0/pcdsdevices/areadetector/cam.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,17 @@
 """
 PCDS cams and overrides for ophyd Cams.
 
 All components (EPICS PVs) associated with a specific camera are added here.
 """
 import logging
 
-import ophyd
-from ophyd import (Component, DynamicDeviceComponent, EpicsSignal,
-                   EpicsSignalRO, FormattedComponent, cam)
-from ophyd.areadetector.base import ADBase, ADComponent, EpicsSignalWithRBV
+from ophyd import Component, EpicsSignal, EpicsSignalRO, cam
+from ophyd.areadetector.base import ADComponent, EpicsSignalWithRBV
 from ophyd.sim import SynSignal
-from ophyd.utils import enum
 
 logger = logging.getLogger(__name__)
 
 __all__ = ['FeeOpalCam']
 
 
 class FeeOpalCam(cam.CamBase):
@@ -96,25 +93,21 @@
 
     # Overridden Components
     # array_rate = Component(Signal)
     array_rate = Component(EpicsSignalRO, 'FrameRate')
     acquire = Component(EpicsSignal, 'Acquire')
 
     # Attrs that arent in the fee opal
-    array_counter = Component(SynSignal) # C(SignalWithRBV, 'ArrayCounter')
-    nd_attributes_file = Component(SynSignal) # C(EpicsSignal, 'NDAttributesFile', string=True)
-    pool_alloc_buffers = Component(SynSignal) # C(EpicsSignalRO, 'PoolAllocBuffers')
-    pool_free_buffers = Component(SynSignal) # C(EpicsSignalRO, 'PoolFreeBuffers')
-    pool_max_buffers = Component(SynSignal) # C(EpicsSignalRO, 'PoolMaxBuffers')
-    pool_max_mem = Component(SynSignal) # C(EpicsSignalRO, 'PoolMaxMem')
-    pool_used_buffers = Component(SynSignal) # C(EpicsSignalRO, 'PoolUsedBuffers')
-    pool_used_mem = Component(SynSignal) # C(EpicsSignalRO, 'PoolUsedMem')
-    port_name = Component(SynSignal) # C(EpicsSignalRO, 'PortName_RBV', string=True)
-    array_callbacks = Component(SynSignal) # C(SignalWithRBV, 'ArrayCallbacks')
-    array_size = Component(SynSignal) # DDC(ad_group(EpicsSignalRO,
-                 #              (('array_size_x', 'ArraySizeX_RBV'),
-                 #               ('array_size_y', 'ArraySizeY_RBV'),
-                 #               ('array_size_z', 'ArraySizeZ_RBV'))),
-                 #     doc='Size of the array in the XYZ dimensions')
-    color_mode = Component(SynSignal) # C(SignalWithRBV, 'ColorMode')
-    data_type = Component(SynSignal) # C(SignalWithRBV, 'DataType')
-    array_size_bytes = Component(SynSignal) # C(EpicsSignalRO, 'ArraySize_RBV')
+    array_counter = Component(SynSignal)
+    nd_attributes_file = Component(SynSignal)
+    pool_alloc_buffers = Component(SynSignal)
+    pool_free_buffers = Component(SynSignal)
+    pool_max_buffers = Component(SynSignal)
+    pool_max_mem = Component(SynSignal)
+    pool_used_buffers = Component(SynSignal)
+    pool_used_mem = Component(SynSignal)
+    port_name = Component(SynSignal)
+    array_callbacks = Component(SynSignal)
+    array_size = Component(SynSignal)
+    color_mode = Component(SynSignal)
+    data_type = Component(SynSignal)
+    array_size_bytes = Component(SynSignal)
```

### Comparing `pcdsdevices-7.1.0/pcdsdevices/areadetector/detectors.py` & `pcdsdevices-7.4.0/pcdsdevices/areadetector/detectors.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,20 +4,18 @@
 All components at the detector level such as plugins or image processing
 functions needed by all instances of a detector are added here.
 """
 import logging
 import shutil
 import subprocess
 import time
-import warnings
 
 from ophyd import Device
 from ophyd.areadetector import cam
-from ophyd.areadetector.base import (ADComponent, EpicsSignalWithRBV,
-                                     NDDerivedSignal)
+from ophyd.areadetector.base import ADComponent, EpicsSignalWithRBV
 from ophyd.areadetector.detectors import DetectorBase
 from ophyd.areadetector.trigger_mixins import SingleTrigger
 from ophyd.device import Component as Cpt
 from ophyd.ophydobj import OphydObject
 from ophyd.signal import AttributeSignal, EpicsSignal, EpicsSignalRO
 from pcdsutils.ext_scripts import get_hutch_name
 
@@ -60,30 +58,35 @@
         port_edges = [(src, dest) for src, dest in graph.edges
                       if src != cam_port or include_cam]
         if use_names:
             port_edges = [(port_map[src].name, port_map[dest].name)
                           for src, dest in port_edges]
         return port_edges
 
-    def screen(self, main: bool=False) -> None:
+    def screen(self, main: bool = False) -> None:
         """
         Open camViewer screen for camera.
 
         Parameters
         ----------
         main : bool, optional
             Set to True to bring up 'main' edm config screen.
             Defaults to False, which opens python viewer.
         """
         if not shutil.which('camViewer'):
             logger.error('no camViewer available')
             return
 
-        arglist = ['camViewer', '-H', str(get_hutch_name()).lower(),
-                    '-c', self.name]
+        arglist = [
+            'camViewer',
+            '-H',
+            str(get_hutch_name()).lower(),
+            '-c',
+            self.name,
+        ]
         if main:
             arglist.append('-m')
 
         logger.info('starting camviewer')
         subprocess.run(arglist, check=False)
 
 
@@ -151,14 +154,15 @@
     hdf51 = ADComponent(
         HDF5FileStore,
         'HDF51:',
         write_path_template='/dev/null',
         kind='normal',
         doc='Save output as an HDF5 file'
     )
+
     def __init__(
         self,
         *args,
         write_path: str,
         always_acquire: bool = True,
         **kwargs,
     ):
@@ -357,14 +361,20 @@
     # Acquisition settings
     exposure = Cpt(EpicsSignalWithRBV, 'AcquireTime', kind='config')
     gain = Cpt(EpicsSignalWithRBV, 'Gain', kind='config')
     num_images = Cpt(EpicsSignalWithRBV, 'NumImages', kind='config')
     image_mode = Cpt(EpicsSignalWithRBV, 'ImageMode', kind='config')
     trigger_mode = Cpt(EpicsSignalWithRBV, 'TriggerMode', kind='config')
     acquisition_period = Cpt(EpicsSignalWithRBV, 'AcquirePeriod', kind='config')
+    bin_x = Cpt(EpicsSignalWithRBV, 'BinX', kind='config')
+    bin_y = Cpt(EpicsSignalWithRBV, 'BinY', kind='config')
+    region_start_x = Cpt(EpicsSignalWithRBV, 'MinX', kind='config')
+    region_size_x = Cpt(EpicsSignalWithRBV, 'SizeX', kind='config')
+    region_start_y = Cpt(EpicsSignalWithRBV, 'MinY', kind='config')
+    region_size_y = Cpt(EpicsSignalWithRBV, 'SizeY', kind='config')
 
     # Image collection settings
     acquire = Cpt(EpicsSignal, 'Acquire', kind='normal')
     acquire_rbv = Cpt(EpicsSignalRO, 'DetectorState_RBV', kind='normal')
     image_counter = Cpt(EpicsSignalRO, 'NumImagesCounter_RBV', kind='normal')
 
     # TJ: removing from the class for now. May be useful later.
@@ -473,8 +483,39 @@
     pass
 
 
 class LasBasler(PCDSAreaDetectorTyphosBeamStats, BaslerBase):
     """
     Class for the Basler cameras used in the laser control system.
     """
-    pass
+    # Configuration dictionary for camera
+    _conf_d = {}
+
+    # Make button available in Typhos screen
+    auto_configure = Cpt(AttributeSignal, attr='_auto_configure', kind='normal')
+    set_metadata(auto_configure, dict(variety='command-proc', value=1))
+
+    @property
+    def _auto_configure(self):
+        return 0
+
+    @_auto_configure.setter
+    def _auto_configure(self, value):
+        self.configure(self._conf_d)
+
+
+class LasBaslerNF(LasBasler):
+    """
+    Class for the near-field Basler cameras used in the laser control system.
+    """
+    _conf_d = {'data_type': 1, 'exposure': 0.005, 'trigger_mode': 0,
+               'acquisition_period': 0.5, 'centroid_enable': 1, 'bin_x': 2,
+               'bin_y': 2, 'stats_enable': 1, 'centroid_threshold': 1000}
+
+
+class LasBaslerFF(LasBasler):
+    """
+    Class for the far-field Basler cameras used in the laser control system.
+    """
+    _conf_d = {'data_type': 1, 'exposure': 0.010, 'trigger_mode': 0,
+               'acquisition_period': 0.5, 'centroid_enable': 1, 'bin_x': 1,
+               'bin_y': 1, 'stats_enable': 1, 'centroid_threshold': 50}
```

### Comparing `pcdsdevices-7.1.0/pcdsdevices/areadetector/plugins.py` & `pcdsdevices-7.4.0/pcdsdevices/areadetector/plugins.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.1.0/pcdsdevices/atm.py` & `pcdsdevices-7.4.0/pcdsdevices/atm.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.1.0/pcdsdevices/attenuator.py` & `pcdsdevices-7.4.0/pcdsdevices/attenuator.py`

 * *Files 3% similar despite different names*

```diff
@@ -175,15 +175,15 @@
 
     def __init__(self, prefix, *, name, **kwargs):
         super().__init__(prefix, name=name, limits=(0, 1), **kwargs)
         self.filters = []
         self._has_subscribed_state = False
         for i in range(1, MAX_FILTERS + 1):
             try:
-                self.filters.append(getattr(self, 'filter{}'.format(i)))
+                self.filters.append(getattr(self, f'filter{i}'))
             except AttributeError:
                 break
 
     @property
     def actuate_value(self):
         """
         Sets the value we use in the 'GO' command.
@@ -439,22 +439,22 @@
 
 def _make_att_classes(max_filters, base_with_3rd_harmonic, name):
     """Generate all possible subclasses."""
     att_classes = {}
     for i in range(1, max_filters + 1):
         att_ns = {}
         for n in range(1, i + 1):
-            comp = Cpt(Filter, ':{:02}'.format(n))
-            att_ns['filter{}'.format(n)] = comp
+            comp = Cpt(Filter, f':{n:02}')
+            att_ns[f'filter{n}'] = comp
 
         if issubclass(base_with_3rd_harmonic, LightpathInOutCptMixin):
             att_ns['lightpath_cpts'] = [
-                f'filter{i}' for i in range(1, i+1)
+                f'filter{i}' for i in range(1, i + 1)
             ]
-        cls_name = '{}{}'.format(name, i)
+        cls_name = f'{name}{i}'
         cls = type(cls_name, (base_with_3rd_harmonic,), att_ns)
         cls.num_att = i
         att_classes[i] = cls
     return att_classes
 
 
 _att_classes = _make_att_classes(
@@ -589,15 +589,15 @@
                        )
     set_metadata(transmission, dict(variety='scalar',
                                     display_format='exponential'))
 
     transmission_3omega = Cpt(
         EpicsSignalRO, 'Transmission3Omega_RBV', kind='normal',
         doc='Normalized transmission at 3 * the reported energy',
-                              )
+    )
     set_metadata(transmission_3omega, dict(variety='scalar',
                                            display_format='exponential'))
 
     def __init__(self, *args, index, **kwargs):
         super().__init__(*args, **kwargs)
         self.index = index
 
@@ -898,14 +898,49 @@
         return f'''\
 {inserted_info}
 
 {table}
 '''
 
 
+class AttenuatorCalculatorSXR_TwoBlade(AttenuatorCalculatorBase):
+    """
+    2 blade x 8 filter solid attenuator variant from the L2SI project.
+
+    Parameters
+    ----------
+    prefix : str
+        Full Solid Attenuator base PV.
+
+    name : str
+        Alias for the Solid Attenuator.
+    """
+
+    tab_component_names = True
+    first_filter = 1
+    num_filters = 2
+    # Not using "DDC" here, so the parent is `self`:
+    _filter_parent = None
+    _filter_index_to_attr = {
+        1: 'blade_01',
+        2: 'blade_02',
+    }
+
+    blade_01 = Cpt(AttenuatorCalculatorSXR_Blade, ':AXIS:01:', index=1)
+    blade_02 = Cpt(AttenuatorCalculatorSXR_Blade, ':AXIS:02:', index=2)
+
+    def format_status_info(self, status_info):
+        """
+        Override status info handler to render the attenuator.
+        """
+        return utils.combine_status_info(
+            self, status_info, self._filter_index_to_attr.values(),
+        )
+
+
 class AttenuatorCalculatorSXR_FourBlade(AttenuatorCalculatorBase):
     """
     4 blade x 8 filter solid attenuator variant from the L2SI project.
 
     Parameters
     ----------
     prefix : str
@@ -1100,14 +1135,178 @@
         return f"""
 {table}
 Transmission (E={energy} keV): {transmission}
 Transmission for 3rd harmonic (E={energy_3} keV): {transmission_3}
 """
 
 
+class AttenuatorSXR_LadderTwoBladeLBD(FltMvInterface, PVPositionerPC,
+                                      LightpathMixin):
+    """
+    Ladder-style solid attenuator variant from the LCLS-II L2SI project.
+
+    This has 2 blades, each with up to 8 filters each.
+    This class includes a calculator to aid in determining which filters to
+    insert for a given attenuation at a specific energy.
+    This class also includes control for the Kurt J. Lesker LBD stage.
+
+    Parameters
+    ----------
+    prefix : str
+        Solid Attenuator base PV.
+
+    name : str
+        Alias for the Solid Attenuator.
+
+    calculator_prefix : str
+        The prefix for the calculator PVs.
+    """
+
+    # QIcon for UX
+    _icon = 'fa.barcode'
+    tab_component_names = True
+
+    # Register that all blades are needed for lightpath calc
+    lightpath_cpts = [f'blade_{idx:02}.state.state' for idx in range(1, 4)]
+
+    # Summary for lightpath view
+    num_in = Cpt(InternalSignal, kind='hinted')
+    num_out = Cpt(InternalSignal, kind='hinted')
+
+    calculator = UCpt(AttenuatorCalculatorSXR_TwoBlade)
+    blade_01 = Cpt(SXRLadderAttenuatorBlade, ':MMS:01')
+    blade_02 = Cpt(SXRLadderAttenuatorBlade, ':MMS:02')
+    # LBD Stage
+    blade_03 = Cpt(FEESolidAttenuatorBlade, ':MMS:03')
+
+    def __init__(self, *args, limits=None, **kwargs):
+        UCpt.collect_prefixes(self, kwargs)
+        limits = limits or (0.0, 1.0)
+        super().__init__(*args, limits=limits, **kwargs)
+
+    @property
+    def setpoint(self):
+        """(PVPositioner compat) - use desired transmission as setpoint."""
+        return self.calculator.desired_transmission
+
+    @property
+    def readback(self):
+        """(PVPositioner compat) - use actual transmission as readback."""
+        return self.calculator.actual_transmission
+
+    @property
+    def actuate(self):
+        """(PVPositioner compat) - use apply_config as an actuation signal."""
+        return self.calculator.apply_config
+
+    def _setup_move(self, position):
+        """(PVPositioner compat) - calculate, then move."""
+        # Do not call `calculator.calculate()` here to respect the current
+        # calculator settings:
+        self.calculator.desired_transmission.put(position)
+        self.calculator.run_calculation.put(1, wait=True)
+        return super()._setup_move(position)
+
+    def get_lightpath_state(self, use_cache=True) -> LightpathState:
+        """
+        Grab slightly different PV values for use in same inout calc fn
+        The state is nested one device deeper than LightpathInOutCptMixin
+        expects.
+        """
+        if (not use_cache) or (self._cached_state is None):
+            lightpath_kwargs = {}
+            lp_sigs = self.lightpath_summary._signals.keys()
+            for sig in lp_sigs:
+                # want to get name of blade_0x from dev_blade_0x_state_state
+                cpt_name = sig.name.removeprefix(self.name + '_')
+                cpt_name = cpt_name.removesuffix('_state_state')
+                lightpath_kwargs[cpt_name] = sig.get()
+
+            self._cached_state = self.calc_lightpath_state(**lightpath_kwargs)
+
+        return self._cached_state
+
+    def calc_lightpath_state(self, **lightpath_kwargs) -> LightpathState:
+        # Repeat lightpath logic to extract num_in, num_out
+        in_check = []
+        out_check = []
+        trans_check = []
+        for sig_name, sig_value in lightpath_kwargs.items():
+            # InOut positioner is not the parent component, but the .state
+            obj = getattr(self, sig_name).state
+            if not obj._state_initialized:
+                # This would prevent make check_inserted, etc. fail
+                utils.schedule_task(self._calc_cache_lightpath_state,
+                                    delay=2.0)
+
+                return LightpathState(
+                    inserted=True,
+                    removed=True,
+                    output={self.output_branches[0]: 1}
+                )
+            # get state of the InOutPositioner and check status
+            in_check.append(obj.check_inserted(sig_value))
+            out_check.append(obj.check_removed(sig_value))
+            trans_check.append(obj.check_transmission(sig_value))
+        self._inserted = any(in_check)
+        self._removed = all(out_check)
+        self._transmission = functools.reduce(lambda a, b: a*b, trans_check)
+
+        self.num_in.put(in_check.count(True), force=True)
+        self.num_out.put(out_check.count(True), force=True)
+        return LightpathState(
+            inserted=self._inserted,
+            removed=self._removed,
+            output={self.output_branches[0]: self._transmission}
+        )
+
+    def format_status_info(self, status_info):
+        """
+        Override status info handler to render the attenuator.
+        """
+        calc_status = status_info.get('calculator', {})
+        transmission = get_status_float(
+            calc_status, 'actual_transmission', 'value',
+            format='E', precision=3,
+        )
+        transmission_3 = get_status_float(
+            calc_status, 'actual_transmission_3omega', 'value',
+            format='E', precision=3,
+        )
+        energy = get_status_float(
+            calc_status, 'energy_actual', 'value',
+            scale=1e-3,
+        )
+        energy_3 = get_status_float(
+            calc_status, 'energy_actual', 'value',
+            scale=3 * 1e-3,
+        )
+        blade_names = [cpt.split('.', 1)[0] for cpt in self.lightpath_cpts]
+        cpt_states = [
+            get_status_value(
+                status_info, cpt, 'state', 'state', 'value',
+                default_value=0
+            )
+            for cpt in blade_names
+        ]
+
+        table = prettytable.PrettyTable()
+        table.field_names = ['State'] + list(blade_names)
+        for state in LadderBladeState:
+            row = [state.name] + ['X' if cpt_state == state.value else ''
+                                  for cpt_state in cpt_states]
+            table.add_row(row)
+
+        return f"""
+{table}
+Transmission (E={energy} keV): {transmission}
+Transmission for 3rd harmonic (E={energy_3} keV): {transmission_3}
+"""
+
+
 class AT1K4(AttenuatorSXR_Ladder):
     """
     AT1K4 solid attenuator variant from the LCLS-II L2SI project.
 
     This has 4 blades, each with up to 8 filters each.
     This class includes a calculator to aid in determining which filters to
     insert for a given attenuation at a specific energy.
@@ -1121,14 +1320,37 @@
         Alias for the Solid Attenuator.
 
     calculator_prefix : str
         The prefix for the calculator PVs.
     """
 
 
+class AT1K2(AttenuatorSXR_LadderTwoBladeLBD):
+    """
+    AT1K2 solid attenuator variant from the LCLS-II L2SI project.
+
+    This has 2 blades, each with up to 8 filters each.
+    This class includes a calculator to aid in determining which filters to
+    insert for a given attenuation at a specific energy.
+    This class also includes control for the Kurt J. Lesker LBD system,
+    allowing IN/OUT state for mirror mount.
+
+    Parameters
+    ----------
+    prefix : str
+        Solid Attenuator base PV.
+
+    name : str
+        Alias for the Solid Attenuator.
+
+    calculator_prefix : str
+        The prefix for the calculator PVs.
+    """
+
+
 class AT2K2(AttenuatorSXR_Ladder):
     """
     AT2K2 solid attenuator variant from the LCLS-II L2SI project.
 
     This has 4 blades, each with up to 8 filters each.
     This class includes a calculator to aid in determining which filters to
     insert for a given attenuation at a specific energy.
@@ -1411,15 +1633,15 @@
             get_status_value(
                 status_info, cpt.split('.', 1)[0], 'state', 'state', 'value',
                 default_value=0
             )
             for cpt in self.lightpath_cpts
         ]
 
-        table = '\n'.join(render_ascii_att(cpt_states,  start_index=1))
+        table = '\n'.join(render_ascii_att(cpt_states, start_index=1))
 
         return f"""
 {table}
 Transmission (E={energy} keV): {transmission}
 Transmission for 3rd harmonic (E={energy_3} keV): {transmission_3}
 Error Summary: {error_sum}
 """
```

### Comparing `pcdsdevices-7.1.0/pcdsdevices/beam_stats.py` & `pcdsdevices-7.4.0/pcdsdevices/beam_stats.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.1.0/pcdsdevices/ccm.py` & `pcdsdevices-7.4.0/pcdsdevices/ccm.py`

 * *Files 0% similar despite different names*

```diff
@@ -693,15 +693,14 @@
         """
         if kill:
             # Must always wait if we are killing the PID
             wait = True
         st = super().move(*args, wait=wait, **kwargs)
         time.sleep(0.01)  # safety wait. Necessary?
         if kill:
-            print('Kill alio PID')
             self.alio.kill()
         return st
 
 
 class CCMEnergyWithVernier(CCMEnergy):
     """
     CCM energy motor and the vernier.
@@ -1110,16 +1109,16 @@
     Converts alio position (mm) to theta angle (rad).
 
     Conversion function
     theta_angle = f(x) = 2arctan * [(sqrt(x^2 + D^2 + 2Rx) - D)/(2R + x)]
     Note that for x = −R, θ = 2 arctan(−R/D)
     """
     return theta0 + 2 * np.arctan(
-         (np.sqrt(alio ** 2 + gd ** 2 + 2 * gr * alio) - gd) / (2 * gr + alio)
-     )
+        (np.sqrt(alio ** 2 + gd ** 2 + 2 * gr * alio) - gd) / (2 * gr + alio)
+    )
 
 
 def wavelength_to_theta(wavelength: float, dspacing: float) -> float:
     """Converts wavelength (A) to theta angle (rad)."""
     return np.arcsin(wavelength/2/dspacing)
```

### Comparing `pcdsdevices-7.1.0/pcdsdevices/crix_motion.py` & `pcdsdevices-7.4.0/pcdsdevices/crix_motion.py`

 * *Files 0% similar despite different names*

```diff
@@ -120,15 +120,15 @@
         the pseudo limits to keep us within the range that this
         calculation is valid and non-nan.
         """
         calc = pseudo_pos.calc
         real = (
             -self.cb
             + self.pol * np.sqrt(self.cb**2 - 4*self.ca*(self.cc - calc))
-            ) / (2*self.ca)
+        ) / (2*self.ca)
         return self.RealPosition(real=real)
 
     @real_position_argument
     def inverse(self, real_pos: typing.NamedTuple) -> typing.NamedTuple:
         """
         Calculate the position of the crystal in mrad given the mm position.
```

### Comparing `pcdsdevices-7.1.0/pcdsdevices/cvmi_motion.py` & `pcdsdevices-7.4.0/pcdsdevices/cvmi_motion.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.1.0/pcdsdevices/dc_devices.py` & `pcdsdevices-7.4.0/pcdsdevices/dc_devices.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.1.0/pcdsdevices/delay_generator.py` & `pcdsdevices-7.4.0/pcdsdevices/delay_generator.py`

 * *Files 0% similar despite different names*

```diff
@@ -120,11 +120,11 @@
         return
 
 
 channel_cpts = {}
 for channel in CHANNELS[:-1]:
     channel_cpts[f'ch{channel}'] = Cpt(
         DgChannel, f":{channel.lower()}", name=f"ch{channel}"
-        )
+    )
 
 DelayGenerator = type('DelayGenerator', (DelayGeneratorBase, ), channel_cpts)
 Dg = DelayGenerator
```

### Comparing `pcdsdevices-7.1.0/pcdsdevices/device.py` & `pcdsdevices-7.4.0/pcdsdevices/device.py`

 * *Files 0% similar despite different names*

```diff
@@ -224,23 +224,21 @@
 
         for cpt_name in self.component_names:
             cpt = getattr(self.__class__, cpt_name)
             if isinstance(cpt, InterfaceComponent):
                 try:
                     obj = kwargs.pop(cpt_name)
                 except KeyError:
-                    raise TypeError(
-                        f'Missing required kwarg {cpt_name}'
-                        ) from None
+                    raise TypeError(f'Missing required kwarg {cpt_name}') from None
                 if isinstance(obj, cpt.cls):
                     self._interface_obj[cpt_name] = obj
                 else:
                     raise TypeError(
                         f'{cpt_name} must be of type {cpt.cls}'
-                        )
+                    )
 
         super().__init__(*args, **kwargs)
 
 
 def to_interface(device_class):
     """
     Convert an arbitrary `Device` into an `InterfaceDevice`.
@@ -266,15 +264,15 @@
         cpt = getattr(device_class, cpt_name)
         interface_cpts[cpt_name] = InterfaceComponent(cpt.cls)
 
     return type(
         device_class.__name__ + 'Interface',
         (InterfaceDevice, device_class),
         interface_cpts
-        )
+    )
 
 
 class UpdateComponent(Component):
     """
     A component that copies and updates a parent component in a subclass.
 
     Use this like any other component, adding it to your device that is a
@@ -409,15 +407,15 @@
     needs_parent: list[type[OphydObject]] = [
         AttributeSignal,
         DerivedSignal,
         PluginBase,
         PseudoSingle,
         PVStateSignal,
         AggregateSignal
-        ]
+    ]
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         # Remove references to parent (in this case, self)
         for cpt_name in self.component_names:
             cpt = getattr(self, cpt_name)
             # The following types break without parents
@@ -432,15 +430,15 @@
 
     def __init_subclass__(cls, **kwargs):
         super().__init_subclass__(**kwargs)
         if hasattr(cls, 'set') and cls.stage_group is None:
             raise TypeError(
                 f"Must specify a stage_group in {cls.__name__} because it "
                 "is a movable device. See the GroupDevice docs."
-                )
+            )
         if cls.stage_group is not None:
             for cpt in cls.stage_group:
                 if not isinstance(cpt, Component):
                     raise TypeError(
                         f"Found non-Component {cpt} in stage_group for "
                         f"{cls.__name__}! Only Component types are allowed!"
                     )
```

### Comparing `pcdsdevices-7.1.0/pcdsdevices/device_types.py` & `pcdsdevices-7.4.0/pcdsdevices/device_types.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.1.0/pcdsdevices/digitizers.py` & `pcdsdevices-7.4.0/pcdsdevices/digitizers.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.1.0/pcdsdevices/doc_stubs.py` & `pcdsdevices-7.4.0/pcdsdevices/doc_stubs.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.1.0/pcdsdevices/energy_monitor.py` & `pcdsdevices-7.4.0/pcdsdevices/energy_monitor.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.1.0/pcdsdevices/epics_motor.py` & `pcdsdevices-7.4.0/pcdsdevices/epics_motor.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 from ophyd.ophydobj import Kind
 from ophyd.signal import EpicsSignal, EpicsSignalRO, Signal
 from ophyd.status import DeviceStatus, MoveStatus, SubscriptionStatus
 from ophyd.status import wait as status_wait
 from ophyd.utils import LimitError
 from ophyd.utils.epics_pvs import raise_if_disconnected, set_and_wait
 from pcdsutils.ext_scripts import get_hutch_name
+from prettytable import PrettyTable
 
 from pcdsdevices.pv_positioner import PVPositionerComparator
 
 from .device import UpdateComponent as UpCpt
 from .doc_stubs import basic_positioner_init
 from .interface import FltMvInterface
 from .pseudopos import OffsetMotorBase, delay_class_factory
@@ -608,15 +609,18 @@
 
     tab_whitelist = [
         'reinitialize',
         'acceleration',
         'clear_.*',
         'configure',
         'get_configuration',
+        'get_configuration_values',
+        'get_current_values',
         'find_configuration',
+        'diff_configuration'
     ]
 
     # The singleton parameter manager object.
     _pm = None
     # If we fail to create _pm, set bool to only try once
     _pm_init_error = False
 
@@ -679,15 +683,15 @@
 
         # Generate a status
         st = SubscriptionStatus(
             self.error_severity,
             initialize_complete,
             timeout=timeout,
             settle_time=0.5,
-            )
+        )
         # Wait on status if requested
         if wait:
             status_wait(st)
         return st
 
     def clear_all_flags(self):
         """Clear all the flags from the IMS motor."""
@@ -730,14 +734,42 @@
         self.seq_seln.put(flag_info['clear'])
         # Generate a status
         st = SubscriptionStatus(self.bit_status, flag_is_cleared)
         if wait:
             status_wait(st, timeout=timeout)
         return st
 
+    @property
+    def md(self):
+        if self._md is None:
+            raise AttributeError('Device does not have an attached md, '
+                                 'and was likely not initialized from happi')
+        return self._md
+
+    @md.setter
+    def md(self, new_md):
+        """ initialize attributes when md is set """
+        self._md = new_md
+        self._extra = self._md.extraneous
+        self._id = self._extra.get('_id')
+        self._pvbase = self._extra.get('pvbase')
+        self._stageidentity = self._extra.get('stageidentity')
+        if self._stageidentity is None:
+            logger.warning(f"Stage Identity has not been set for this object: {self._id}. Configure manually.")
+            return
+        elif self._stageidentity == "NEW":
+            logger.warning(f"This is a new stage, parameter manager configuration does not exist yet. Please manually configure {self._id}")
+            return
+        else:
+            try:
+                IMS._setup_and_check_pmgr()
+                self._pm.set_config(self._pvbase, self._stageidentity)
+            except Exception:
+                return
+
     def configure(self, cfgname=None):
         """
         Use the parameter manager to configure the motor.
 
         cfgname : str | None
             The name of the configuration to apply.  If None, use the
             configuration saved in the database.
@@ -753,16 +785,57 @@
 
         Returns the current configuration name as a string or throws an
         exception.
         """
         self._setup_and_check_pmgr()
         return self._pm.get_config(self.prefix)
 
+    def get_configuration_values(self, cfgname=None):
+        """
+        Return the current configuration parameters of the motor
+        in the parameter manager
+
+        Parameters
+        ----------
+        cfgname : str
+               The name of the configuration
+
+        Returns
+        -------
+        A dictionary mapping field names to the configured values
+        """
+        self._setup_and_check_pmgr()
+        if not cfgname:
+            cfgname = self.get_configuration()
+        return self._pm.get_config_values(cfgname)
+
+    def get_current_values(self, pv=None):
+        """
+        Returns the current parameters for a given pv.
+
+        Parameters
+        ----------
+        pv : str
+          Default is None
+
+        Returns
+        -------
+        cdict : dict
+            A dictionary mapping field names (str) to values.
+        """
+
+        pv = self.prefix
+        self._setup_and_check_pmgr()
+
+        self._pm.update_db()
+        o = self._pm._search(self._pm.pm.objs, 'rec_base', pv)
+        return self._pm.pm.getActualConfig(o['id'])
+
     @staticmethod
-    def find_configuration(pattern, case_insensitive=True, display=20):
+    def find_configuration(pattern, case_insensitive=True, display=30):
         """
         Find parameter manager configurations that match the pattern.
 
         pattern : str
             The substring to match.  "." matches any character, and "*"
             matches any string.  These maybe quoted using "\".
 
@@ -773,26 +846,57 @@
         display : int | None
             The maximum number of configurations to display.  If None,
             don't display any, but return a list of all matches.
 
         Returns a list of strings if display is None, and nothing otherwise.
         """
         IMS._setup_and_check_pmgr()
-        matches = IMS._pm.match_config(pattern, ci=case_insensitive)
+        matches = IMS._pm.match_config(pattern, ci=case_insensitive, parent='USR')
         if display is None:
             return matches
         if len(matches) >= display:
             print("'%s' matches %d configurations." % (pattern, len(matches)))
             print("Use a more restrictive pattern or "
                   "larger value for display (%d)." % display)
         else:
             print("Matches for '%s':" % pattern)
             for m in matches:
                 print("    %s" % m)
 
+    def diff_configuration(self, cfgname=None):
+        """
+        Find the differences between the actual motor settings and the
+        current parameter manager configuration.
+
+        Parameters
+        ----------
+        cfgname : str
+            The name of the configuration to compare the settings to.  If
+            this is None, use the current configuration.
+
+        Returns
+        -------
+        diff : PrettyTable
+            A table with headers "Parameter", "Actual", and "Configuration",
+            showing the differences between the live values and the configured
+            values.
+
+        Raises an exception if the comparison fails for any reason.
+        """
+        IMS._setup_and_check_pmgr()
+
+        d = self._pm.diff_config(self.prefix, cfgname)
+        table = PrettyTable()
+        table.field_names = ["Parameter", "Actual", "Configuration"]
+        for key, value in d.items():
+            actual = value[0]
+            configuration = value[1]
+            table.add_row([key, actual, configuration])
+        return table
+
     @staticmethod
     def setup_pmgr():
         try:
             from pmgr import pmgrAPI
         except ImportError:
             logger.error('Failed to import pmgr!')
             logger.debug('', exc_info=True)
```

### Comparing `pcdsdevices-7.1.0/pcdsdevices/evr.py` & `pcdsdevices-7.4.0/pcdsdevices/evr.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.1.0/pcdsdevices/gauge.py` & `pcdsdevices-7.4.0/pcdsdevices/gauge.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.1.0/pcdsdevices/gon.py` & `pcdsdevices-7.4.0/pcdsdevices/gon.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.1.0/pcdsdevices/happi/containers.py` & `pcdsdevices-7.4.0/pcdsdevices/happi/containers.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,19 +116,20 @@
                        'enter the name', enforce=str)
     args = copy(HappiItem.args)
     args.default = ['{{prefix}}']
     kwargs = copy(HappiItem.kwargs)
     kwargs.default = {'name': '{{name}}'}
 
     def __repr__(self):
-        return '{} (name={}, prefix={}, z={})'.format(
-                                    self.__class__.__name__,
-                                    self.name,
-                                    self.prefix,
-                                    self.z)
+        return "{} (name={}, prefix={}, z={})".format(
+            self.__class__.__name__,
+            self.name,
+            self.prefix,
+            self.z,
+        )
 
     @property
     def screen(self):
         warnings.warn("The 'screen' keyword is no longer used in Happi as it "
                       "lacks specificity. Use one of detailed_screen, "
                       "embedded_screen, or engineering screen instead",
                       DeprecationWarning)
@@ -661,7 +662,14 @@
     ioc_type = copy(LCLSItem.ioc_type)
     ioc_type.default = 'EK9000'
     ioc_ip = EntryInfo(('Netconfig name of the EK9000 the sensors are '
                         'connected to. Used to build IOC configs.'),
                        optional=True, enforce=str)
     ioc_base = EntryInfo('Base PV of the EK9000 IOC', optional=True,
                          enforce=str)
+
+
+class Leviton(LCLSItem):
+    kwargs = deepcopy(LCLSItem.kwargs)
+    kwargs.default['elevations'] = "{{elevations}}"
+    elevations = EntryInfo(doc='List of elevation numbers for rack',
+                           optional=False, enforce=list)
```

### Comparing `pcdsdevices-7.1.0/pcdsdevices/inout.py` & `pcdsdevices-7.4.0/pcdsdevices/inout.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,16 +58,17 @@
     _transmission = {}
     _in_if_not_out = False
 
     tab_whitelist = ['inserted', 'removed', 'insert', 'remove', 'transmission']
 
     def __init__(self, prefix, *, name, **kwargs):
         if self.__class__ is InOutPositioner:
-            raise TypeError(('InOutPositioner must be subclassed with at '
-                             'least a state signal'))
+            raise TypeError(
+                'InOutPositioner must be subclassed with at least a state signal'
+            )
         super().__init__(prefix, name=name, **kwargs)
 
     @required_for_connection
     def _state_init(self):
         super()._state_init()
         if self._in_if_not_out:
             outish_states = [
@@ -216,17 +217,19 @@
     :class:`PVStatePositioner` documentation for more information.
     """
 
     __doc__ += basic_positioner_init
 
     def __init__(self, *args, **kwargs):
         if self.__class__ is InOutPVStatePositioner:
-            raise TypeError(('InOutPVStatePositioner must be subclassed, '
-                             'adding signals and filling in the '
-                             '_state_logic dict.'))
+            raise TypeError(
+                'InOutPVStatePositioner must be subclassed, '
+                'adding signals and filling in the '
+                '_state_logic dict.'
+            )
         super().__init__(*args, **kwargs)
 
 
 class TwinCATInOutPositioner(TwinCATStatePositioner, InOutPositioner):
     """
     :class:`InOutPositioner` on top of a :class:`TwinCATStatePositioner`.
```

### Comparing `pcdsdevices-7.1.0/pcdsdevices/interface.py` & `pcdsdevices-7.4.0/pcdsdevices/interface.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 
 
 class _TabCompletionHelper:
     """
     Base class for `TabCompletionHelperClass`, `TabCompletionHelperInstance`.
     """
 
-    _includes: typing.Set[str]
+    _includes: set[str]
     _regex: typing.Optional[typing.Pattern]
 
     def __init__(self):
         self._includes = set()
         self._regex = None
         self.reset()
 
@@ -95,15 +95,15 @@
 
     Parameters
     ----------
     cls : subclass of BaseInterface
         Class type object to generate tab completion information from.
     """
 
-    cls: typing.Type['BaseInterface']
+    cls: type['BaseInterface']
 
     def __init__(self, cls):
         self.cls = cls
         super().__init__()
 
     def reset(self):
         """Reset the attribute includes to those annotated in the class."""
@@ -142,41 +142,41 @@
 
     class_helper : TabCompletionHelperClass
         Class helper for defaults.
     """
 
     class_helper: TabCompletionHelperClass
     instance: 'BaseInterface'
-    super_dir: typing.Callable[[], typing.List[str]]
+    super_dir: typing.Callable[[], list[str]]
 
     def __init__(self, instance, class_helper):
         assert isinstance(instance, BaseInterface), 'Must mix in BaseInterface'
 
         self.class_helper = class_helper
         self.instance = instance
         self.super_dir = super(BaseInterface, instance).__dir__
         super().__init__()
 
     def reset(self):
         """Reset the attribute includes to that defined by the class."""
         super().reset()
         self._includes = set(self.class_helper._includes)
 
-    def get_filtered_dir_list(self) -> typing.List[str]:
+    def get_filtered_dir_list(self) -> list[str]:
         """Get the dir list, filtered based on the whitelist."""
         if self._regex is None:
             self.build_regex()
 
         return [
             elem
             for elem in self.super_dir()
             if self._regex.fullmatch(elem)
         ]
 
-    def get_dir(self) -> typing.List[str]:
+    def get_dir(self) -> list[str]:
         """Get the dir list based on the engineering mode settings."""
         if get_engineering_mode():
             return self.super_dir()
         return self.get_filtered_dir_list()
 
 
 class BaseInterface:
@@ -191,17 +191,21 @@
 
     Attributes
     ----------
     tab_whitelist : list
         List of string regex to show in autocomplete for non-engineering mode.
     """
 
-    tab_whitelist = (OphydObject_whitelist + BlueskyInterface_whitelist +
-                     Device_whitelist + Signal_whitelist +
-                     Positioner_whitelist)
+    tab_whitelist = (
+        OphydObject_whitelist
+        + BlueskyInterface_whitelist
+        + Device_whitelist
+        + Signal_whitelist
+        + Positioner_whitelist
+    )
 
     _class_tab: TabCompletionHelperClass
     _tab: TabCompletionHelperInstance
 
     def __init_subclass__(cls, **kwargs):
         super().__init_subclass__(**kwargs)
         mro = cls.mro()
@@ -698,15 +702,15 @@
         :meth:`end_monitor_thread`, which may be useful when this is called in
         a background thread.
         """
 
         try:
             self._mov_ev.clear()
             while not self._mov_ev.is_set():
-                print("\r {0:4f}".format(self.wm()), end=" ")
+                print(f"\r {self.wm():4f}", end=" ")
                 self._mov_ev.wait(0.1)
         except KeyboardInterrupt:
             pass
         finally:
             self._mov_ev.clear()
 
     # Legacy alias
@@ -846,16 +850,15 @@
         If there are existing plots, this will be the position on the most
         recently active plot. If there are no existing plots, an empty plot
         will be created with the motor's limits as the range.
         """
 
         # Importing forces backend selection, so do inside method
         import matplotlib.pyplot as plt  # NOQA
-        logger.info(("Select new motor x-position in current plot "
-                     "by mouseclick"))
+        logger.info("Select new motor x-position in current plot by mouseclick")
         if not plt.get_fignums():
             upper_limit = 0
             lower_limit = self.limits[0]
             if self.limits[0] == self.limits[1]:
                 upper_limit = self.limits[0]+100
             else:
                 upper_limit = self.limits[1]
@@ -1034,19 +1037,21 @@
         the history accordingly.
         """
 
         logger.debug(('call %s presets._update(%s, %s, value=%s, comment=%s, '
                       'active=%s)'), self._device.name, preset_type, name,
                      value, comment, active)
         if not isinstance(name, str):
-            raise TypeError(('name must be of type <str>, not type'
-                             '{}'.format(type(name))))
+            raise TypeError(
+                f"name must be of type <str>, not type {type(name)}"
+            )
         if value is not None and not isinstance(value, numbers.Real):
-            raise TypeError(('value must be a real numeric type, not type'
-                             '{}'.format(type(value))))
+            raise TypeError(
+                f"value must be a real numeric type, not type {type(value)}"
+            )
         try:
             path = self._path(preset_type)
             if not path.exists():
                 path.touch()
                 path.chmod(0o666)
             with self._file_open_rlock(preset_type):
                 data = self._read(preset_type)
@@ -1058,15 +1063,15 @@
                     ts = time.strftime('%d %b %Y %H:%M:%S')
                     data[name]['value'] = value
                     history = data[name].get('history', {})
                     if comment:
                         comment = ' ' + comment
                     else:
                         comment = ''
-                    history[ts] = '{:10.4f}{}'.format(value, comment)
+                    history[ts] = f'{value:10.4f}{comment}'
                     data[name]['history'] = history
                 if active:
                     data[name]['active'] = True
                 else:
                     data[name]['active'] = False
                 self._write(preset_type, data)
         except BlockingIOError:
@@ -1465,15 +1470,15 @@
                 args[1].umvr(scale, log=False, newline=False)
             elif direction == down:
                 args[1].umvr(-scale, log=False, newline=False)
         except Exception as exc:
             logger.error('Error in tweak move: %s', exc)
             logger.debug('', exc_info=True)
 
-    start_text = ['{} at {:.4f}'.format(mot.name, mot.wm()) for mot in args]
+    start_text = [f'{mot.name} at {mot.wm():.4f}' for mot in args]
     logger.info('Started tweak of ' + ', '.join(start_text))
 
     # Loop takes in user key input and stops when 'q' is pressed
     is_input = True
     while is_input is True:
         show_status()
         inp = utils.get_input()
@@ -1813,15 +1818,15 @@
             utils.schedule_task(self._calc_cache_lightpath_state,
                                 delay=self.retry_delay)
 
             return LightpathState(
                 inserted=True,
                 removed=True,
                 output={self.output_branches[0]: 1}
-                )
+            )
 
         self._inserted = self.check_inserted(state)
         self._removed = self.check_removed(state)
         self._transmission = self.check_transmission(state)
         return LightpathState(
             inserted=self._inserted,
             removed=self._removed,
```

### Comparing `pcdsdevices-7.1.0/pcdsdevices/ipm.py` & `pcdsdevices-7.4.0/pcdsdevices/ipm.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,15 +83,15 @@
     """
 
     tab_whitelist = ['x_motor', 'y_motor', 'insert', 'remove']
 
     x_motor = Cpt(IMS, ':X_MOTOR', kind='normal')
     state = Cpt(InOutRecordPositioner, '', kind='normal')
 
-    def __init__(self, prefix, *, name,  **kwargs):
+    def __init__(self, prefix, *, name, **kwargs):
         super().__init__(prefix, name=name, **kwargs)
         self.y_motor = self.state.motor
 
     @property
     def inserted(self):
         """Returns `True` if diode is inserted."""
         return self.state.inserted
@@ -313,15 +313,15 @@
                 kind='config', string=True)
 
     base = FCpt(EpicsSignal, '{self.prefix}:CH{self.channel_index}_BASE',
                 kind='config')
     scale = FCpt(EpicsSignal, '{self.prefix}:CH{self.channel_index}_SCALE',
                  kind='config')
 
-    def __init__(self, prefix, *, name, channel_index,  **kwargs):
+    def __init__(self, prefix, *, name, channel_index, **kwargs):
         self.channel_index = channel_index
         super().__init__(prefix, name=name, **kwargs)
 
 
 class IPIMB(BaseInterface, GroupDevice):
     """
     Class for an IPIMB box.
@@ -417,15 +417,15 @@
         EpicsSignal, '{self.prefix}:NumberOfSamples{self.channel_index}_RBV',
         write_pv='{self.prefix}:NumberOfSamples{self.channel_index}',
         kind='config')
     delay = FCpt(
         EpicsSignal, '{self.prefix}:Delay{self.channel_index}_RBV',
         write_pv='{self.prefix}:Delay{self.channel_index}', kind='config')
 
-    def __init__(self, prefix, *, name, channel_index,  **kwargs):
+    def __init__(self, prefix, *, name, channel_index, **kwargs):
         self.channel_index = channel_index
         super().__init__(prefix, name=name, **kwargs)
 
 
 class Wave8(BaseInterface, GroupDevice):
     """
     Class for a wave8.
```

### Comparing `pcdsdevices-7.1.0/pcdsdevices/jet.py` & `pcdsdevices-7.4.0/pcdsdevices/jet.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.1.0/pcdsdevices/lamp_motion.py` & `pcdsdevices-7.4.0/pcdsdevices/lamp_motion.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.1.0/pcdsdevices/lasers/btms_config.py` & `pcdsdevices-7.4.0/pcdsdevices/lasers/btms_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 import dataclasses
 import enum
 import logging
-from typing import Dict, List, Optional, Tuple, Union
+from typing import Union
 
 logger = logging.getLogger(__name__)
 
 
 POSITION_DIAGRAM = """
 
              LD8   LD9  LD10  LD11  LD12  LD13  LD14
@@ -35,15 +35,15 @@
     STAGE_CHAR = "*"
     BEAM_CHAR_UP = "^"
     BEAM_CHAR_DOWN = "v"
 
     def __init__(self):
         self.text = POSITION_DIAGRAM
 
-    def _find_line_col(self, text: str) -> Tuple[int, int]:
+    def _find_line_col(self, text: str) -> tuple[int, int]:
         """Get the line and column of ``text``."""
         for lineno, line in enumerate(self.text.splitlines()):
             if text in line:
                 return lineno, line.index(text)
         raise ValueError(f"{text} not found")
 
     def _fill(
@@ -126,14 +126,17 @@
     ls6 = "LS6"
     ls2 = "LS2"
     ls7 = "LS7"
     ls3 = "LS3"
     ls8 = "LS8"
     ls4 = "LS4"
 
+    def __str__(self) -> str:
+        return self.value
+
     @classmethod
     def from_index(cls, index: int) -> SourcePosition:
         """"
         Get a SourcePosition given its integer index.
         """
         try:
             return getattr(cls, f"ls{index}")
@@ -179,32 +182,32 @@
             SourcePosition.ls1,
             SourcePosition.ls2,
             SourcePosition.ls3,
             SourcePosition.ls4,
         )
 
     @property
-    def bay(self) -> Optional[int]:
+    def bay(self) -> int | None:
         """The near field camera prefix associated with this source position."""
         return {
             SourcePosition.ls1: 1,
             SourcePosition.ls5: 3,
             SourcePosition.ls8: 4,
         }.get(self, None)
 
     @property
-    def near_field_camera_prefix(self) -> Optional[str]:
+    def near_field_camera_prefix(self) -> str | None:
         """The near field camera prefix associated with this source position."""
         bay = self.bay
         if bay is not None:
             return f"LAS:LHN:BAY{bay}:CAM:01:"
         return None
 
     @property
-    def far_field_camera_prefix(self) -> Optional[str]:
+    def far_field_camera_prefix(self) -> str | None:
         """The far field camera prefix associated with this source position."""
         bay = self.bay
         if bay is not None:
             return f"LAS:LHN:BAY{bay}:CAM:02:"
         return None
 
 
@@ -231,14 +234,17 @@
     ld12 = "LD12"  # top
     ld5 = "LD5"    # bottom
     ld13 = "LD13"  # top
     ld6 = "LD6"    # bottom
     ld14 = "LD14"  # top
     ld7 = "LD7"    # bottom
 
+    def __str__(self) -> str:
+        return self.value
+
     @property
     def name_and_desc(self) -> str:
         """Name and description in the form: 'LDx (desc).'"""
         return f"{self.value} ({self.description})"
 
     @property
     def description(self) -> str:
@@ -274,15 +280,15 @@
         """"
         Get an integer index from the source position.
         """
         return int(self.name.lstrip("ld"))
 
     def path_to(
         self, target: DestinationPosition
-    ) -> Tuple[DestinationPosition, ...]:
+    ) -> tuple[DestinationPosition, ...]:
         """
         Get crossed destinations on the path from ``self`` to ``target``.
 
         The resulting path excludes the starting position (``self``), but
         includes ``target``.
 
         The first ``DestinationPosition`` in the returned tuple will be the
@@ -315,21 +321,21 @@
 ALL_DESTINATIONS = tuple(DestinationPosition)
 AnyPosition = Union[SourcePosition, DestinationPosition]
 
 
 PORT_SPACING_MM = 215.9  # 8.5 in
 
 # PV source index (bay) to installed LS port
-valid_sources: Tuple[SourcePosition, ...] = (
+valid_sources: tuple[SourcePosition, ...] = (
     SourcePosition.ls1,  # Bay 1
     SourcePosition.ls5,  # Bay 3
     SourcePosition.ls8,  # Bay 4
 )
 # PV destination index (bay) to installed LD port
-valid_destinations: Tuple[DestinationPosition, ...] = (
+valid_destinations: tuple[DestinationPosition, ...] = (
     DestinationPosition.ld2,   # TMO IP3
     DestinationPosition.ld4,   # RIX ChemRIXS
     DestinationPosition.ld6,   # RIX QRIXS
     DestinationPosition.ld8,   # TMO IP1
     DestinationPosition.ld9,   # Laser Lab
     DestinationPosition.ld10,  # TMO IP2
     DestinationPosition.ld14,  # XPP
@@ -417,15 +423,15 @@
         The "target destination" is the one that the linear stage for the
         indicated source is aiming at.
 
     beam_status : bool
         Indicates if the beam is active for the given source.
     """
     source: SourcePosition
-    destination: Optional[DestinationPosition]
+    destination: DestinationPosition | None
     beam_status: bool
 
 
 @dataclasses.dataclass
 class BtmsDestinationState:
     """
     Per-destination status.
@@ -449,26 +455,26 @@
     sources : dict of SourcePosition to BtmsSourceState
         Per-source status.
     destinations : dict of DestinationPosition to BtmsDestinationState
         Per-destination status.
     maintenance_mode : bool
         System-level maintenance mode setting.
     """
-    sources: Dict[SourcePosition, BtmsSourceState] = dataclasses.field(
+    sources: dict[SourcePosition, BtmsSourceState] = dataclasses.field(
         default_factory=dict
     )
-    destinations: Dict[DestinationPosition, BtmsDestinationState] = dataclasses.field(
+    destinations: dict[DestinationPosition, BtmsDestinationState] = dataclasses.field(
         default_factory=lambda: {
             pos: BtmsDestinationState()
             for pos in DestinationPosition
         }
     )
     maintenance_mode: bool = False
 
-    def check_configuration(self) -> List[MoveError]:
+    def check_configuration(self) -> list[MoveError]:
         """
         Check the current configuration for any logical errors/conflicts.
         """
         errors = []
         if self.maintenance_mode:
             errors.append(
                 MaintenanceModeActiveError(
@@ -487,17 +493,17 @@
                     )
                 )
         return errors
 
     def check_move_all(
         self,
         moving_source: SourcePosition,
-        closest_destination: Optional[DestinationPosition],
+        closest_destination: DestinationPosition | None,
         target_destination: DestinationPosition,
-    ) -> List[MoveError]:
+    ) -> list[MoveError]:
         """
         Check motion of ``moving_source`` from ``closest_destination`` to
         ``target_destination``.
 
         Returns all conflicts along the way.
 
         Parameters
@@ -516,18 +522,18 @@
             Any detected issues for the given move request.
         """
         errors = self.check_configuration()
 
         if closest_destination is None:
             closest_destination = self.sources[moving_source].destination
 
-        dest_to_source = dict(
-            (source.destination, source.source)
+        dest_to_source = {
+            source.destination: source.source
             for source in self.sources.values()
-        )
+        }
 
         for other_source in self.sources:
             if other_source == moving_source:
                 ...
             elif self.sources[other_source].destination == target_destination:
                 errors.append(
                     DestinationInUseError(
@@ -595,15 +601,15 @@
                     )
                 )
         return errors
 
     def check_move(
         self,
         moving_source: SourcePosition,
-        closest_destination: Optional[DestinationPosition],
+        closest_destination: DestinationPosition | None,
         target_destination: DestinationPosition,
     ) -> None:
         """
         Check motion of ``moving_source`` from ``closest_destination`` to
         ``target_destination``.
 
         Parameters
```

### Comparing `pcdsdevices-7.1.0/pcdsdevices/lasers/btps.py` & `pcdsdevices-7.4.0/pcdsdevices/lasers/btps.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-from typing import Dict, List, Optional, Tuple, cast
+from typing import cast
 
 from ophyd.device import Component as Cpt
 from ophyd.device import Device
 from ophyd.signal import EpicsSignalRO
 from ophyd.status import AndStatus, MoveStatus
 
 from pcdsdevices.valve import VGC
@@ -83,15 +83,15 @@
         PytmcSignal,
         "Inclusive",
         io="io",
         kind="normal",
         doc="Is the value comparison exclusive or inclusive?",
     )
 
-    def get_delta(self, value: Optional[float] = None) -> float:
+    def get_delta(self, value: float | None = None) -> float:
         """
         Get the delta to the nominal value.
 
         If ``value`` is provided, it will be used in place of the PLC-
         specified value (i.e., ``self.value``).
 
         Returns
@@ -126,15 +126,15 @@
 class SourceToDestinationConfig(BaseInterface, Device):
     """BTPS per-(source, destination) configuration settings and state."""
 
     def __init__(
         self,
         prefix: str,
         source_pos: SourcePosition,
-        destination_pos: Optional[btms.DestinationPosition] = None,
+        destination_pos: btms.DestinationPosition | None = None,
         **kwargs
     ):
         self.source_pos = source_pos
         super().__init__(prefix, **kwargs)
 
         if destination_pos is None:
             try:
@@ -213,15 +213,15 @@
         kind="normal",
         doc=(
             "Set if the mirror assembly for this source is in position for "
             "this laser destination"
         ),
     )
 
-    def summarize_checks(self) -> List[str]:
+    def summarize_checks(self) -> list[str]:
         """
         Summarize all checks into a user-readable form.
 
         Returns
         -------
         list of str
         """
@@ -354,15 +354,15 @@
         "LS8:",
         source_pos=SourcePosition.ls8,
         doc="Settings for source LS8 (bay 4) to this destination",
     )
     exit_valve = Cpt(BtpsVGC, "VGC:01", kind="normal", doc="Destination exit valve")
 
     @property
-    def sources(self) -> Dict[SourcePosition, SourceToDestinationConfig]:
+    def sources(self) -> dict[SourcePosition, SourceToDestinationConfig]:
         """
 
         Returns
         -------
         Dict[SourcePosition, SourceToDestinationConfig]
 
         """
@@ -516,15 +516,15 @@
         Move to the target destination and return a combined status for all motion.
         """
         linear_status, rotary_status, goniometer_status = self.set_with_movestatus(dest, check=check)
         return AndStatus(AndStatus(linear_status, rotary_status), goniometer_status)
 
     def set_with_movestatus(
         self, dest: DestinationPosition, check: bool = True
-    ) -> Tuple[MoveStatus, MoveStatus, MoveStatus]:
+    ) -> tuple[MoveStatus, MoveStatus, MoveStatus]:
         """
         Move to the target destination and return statuses for each motion.
         """
         if check:
             self.check_move(dest)
 
         config = self.parent.destinations[dest].sources[self.source_pos]
@@ -575,15 +575,15 @@
         ------
         MoveError
             Raises specific ``MoveError`` subclass based on the reason.
         """
         state = self.parent.to_btms_state()
         state.check_move(self.source_pos, None, dest)
 
-    def check_move_all(self, dest: DestinationPosition) -> List[MoveError]:
+    def check_move_all(self, dest: DestinationPosition) -> list[MoveError]:
         """
         Check for conflicts moving this source to ``dest``.
 
         Parameters
         ----------
         dest : DestinationPosition
             The target destination for the source to move to.
@@ -624,16 +624,16 @@
                 # self.ld11,
                 # self.ld12,
                 # self.ld13,
                 self.ld14,
             )
         }
 
-    sources: Dict[SourcePosition, BtpsSourceStatus]
-    destinations: Dict[btms.DestinationPosition, DestinationConfig]
+    sources: dict[SourcePosition, BtpsSourceStatus]
+    destinations: dict[btms.DestinationPosition, DestinationConfig]
 
     config = Cpt(
         GlobalConfig,
         "LTLHN:BTPS:Config:",
         doc="Global BTPS configuration",
     )
 
@@ -723,15 +723,15 @@
         Move ``source`` to the target destination ``dest`` and return a combined
         status object.
         """
         return self.sources[source].set(dest)
 
     def set_source_to_destination_with_movestatus(
         self, source: SourcePosition, dest: DestinationPosition
-    ) -> Tuple[MoveStatus, MoveStatus, MoveStatus]:
+    ) -> tuple[MoveStatus, MoveStatus, MoveStatus]:
         """
         Move ``source`` to the target destination ``dest`` and return statuses
         for each motion.
         """
         return self.sources[source].set_with_movestatus(dest)
 
     def to_btms_state(self) -> BtmsState:
@@ -774,12 +774,12 @@
             dest_state.yields_control = bool(
                 dest.yields_control.get()
             )
 
         state.maintenance_mode = bool(self.config.maintenance_mode.get())
         return state
 
-    def status_info(self) -> Dict[str, BtmsState]:
+    def status_info(self) -> dict[str, BtmsState]:
         return {"state": self.to_btms_state()}
 
     def format_status_info(self, state_dict: dict):
         return str(state_dict["state"])
```

### Comparing `pcdsdevices-7.1.0/pcdsdevices/lasers/counters.py` & `pcdsdevices-7.4.0/pcdsdevices/lasers/counters.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.1.0/pcdsdevices/lasers/dicon.py` & `pcdsdevices-7.4.0/pcdsdevices/lasers/dicon.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.1.0/pcdsdevices/lasers/ek9000.py` & `pcdsdevices-7.4.0/pcdsdevices/lasers/ek9000.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.1.0/pcdsdevices/lasers/elliptec.py` & `pcdsdevices-7.4.0/pcdsdevices/lasers/elliptec.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 """
 Classes for ThorLabs Elliptec motors.
 """
 
 
-from ophyd import Device
 from ophyd import FormattedComponent as FCpt
 from ophyd.signal import EpicsSignal, EpicsSignalRO
 
+from pcdsdevices.pv_positioner import PVPositionerIsClose
 from pcdsdevices.variety import set_metadata
 
 
-class EllBase(Device):
+class EllBase(PVPositionerIsClose):
     """
     Base class for Elliptec stages.
     """
     set_position = FCpt(EpicsSignal, '{prefix}:M{self._channel}:CURPOS',
                         write_pv='{prefix}:M{self._channel}:MOVE',
                         kind='normal')
 
@@ -40,14 +40,24 @@
     _save = FCpt(EpicsSignal, '{prefix}:PORT{self._port}:SAVE',
                  kind='omitted')
     _command = FCpt(EpicsSignal, '{prefix}:PORT{self._port}:CMD',
                     kind='omitted')
     _response = FCpt(EpicsSignalRO, '{prefix}:PORT{self._port}:RESPONSE',
                      kind='omitted')
 
+    # Scanning Interface
+    setpoint = FCpt(EpicsSignal, '{prefix}:M{self._channel}:MOVE',
+                    kind='omitted')
+    readback = FCpt(EpicsSignal, '{prefix}:M{self._channel}:CURPOS',
+                    kind='omitted')
+    user_setpoint = FCpt(EpicsSignal, '{prefix}:M{self._channel}:MOVE',
+                         kind='omitted')
+    user_readback = FCpt(EpicsSignal, '{prefix}:M{self._channel}:CURPOS',
+                         kind='omitted')
+
     def __init__(self, prefix, port=0, channel=1, **kwargs):
         self._port = port
         self._channel = channel
         super().__init__(prefix, **kwargs)
 
 
 class Ell6(EllBase):
```

### Comparing `pcdsdevices-7.1.0/pcdsdevices/lasers/qmini.py` & `pcdsdevices-7.4.0/pcdsdevices/lasers/qmini.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.1.0/pcdsdevices/lasers/rfof.py` & `pcdsdevices-7.4.0/pcdsdevices/lasers/rfof.py`

 * *Files 0% similar despite different names*

```diff
@@ -231,18 +231,15 @@
         kind="normal",
         doc="Input RF power (dBm)"
     )
     pd1_rf_power_return = Cpt(
         EpicsSignalRO,
         ":TX_PD1_RF",
         kind="normal",
-        doc=(
-            "PD1 RF power - returned "
-            "optical signal (dBm)"
-            )
+        doc="PD1 RF power - returned optical signal (dBm)"
     )
     pd2_rf_power_transmit = Cpt(
         EpicsSignalRO,
         ":TX_PD2_RF",
         kind="normal",
         doc=(
             "PD2 RF power - transmitted "
```

### Comparing `pcdsdevices-7.1.0/pcdsdevices/lasers/thorlabsWFS.py` & `pcdsdevices-7.4.0/pcdsdevices/lasers/thorlabsWFS.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.1.0/pcdsdevices/lasers/tuttifrutti.py` & `pcdsdevices-7.4.0/pcdsdevices/lasers/tuttifrutti.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.1.0/pcdsdevices/lasers/zoomtelescope.py` & `pcdsdevices-7.4.0/pcdsdevices/lasers/zoomtelescope.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.1.0/pcdsdevices/lens.py` & `pcdsdevices-7.4.0/pcdsdevices/lens.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.1.0/pcdsdevices/lic.py` & `pcdsdevices-7.4.0/pcdsdevices/lic.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.1.0/pcdsdevices/light_control.py` & `pcdsdevices-7.4.0/pcdsdevices/light_control.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.1.0/pcdsdevices/lodcm.py` & `pcdsdevices-7.4.0/pcdsdevices/lodcm.py`

 * *Files 1% similar despite different names*

```diff
@@ -443,19 +443,19 @@
                  add_prefix=('prefix', 'motor_prefix'), kind='normal',
                  doc='Chi 2 motor offset for C [deg]')
     chi2Si = FCpt(OffsetIMSWithPreset, prefix='{self._prefix}:CHI2:OFF_Si',
                   name='chi2_si',
                   motor_prefix='{self._hutch_prefix}:MON:MMS:14',
                   add_prefix=('prefix', 'motor_prefix'), kind='normal',
                   doc='Chi 2 motor offset for Si [deg]')
-    h2nC = FCpt(OffsetIMSWithPreset, prefix='{self._prefix}:H2N:OFF_C',
+    h2nC = FCpt(OffsetMotor, prefix='{self._prefix}:H2N:OFF_C',
                 name='h2n_c', motor_prefix='{self._hutch_prefix}:MON:MMS:15',
                 add_prefix=('prefix', 'motor_prefix'), kind='normal',
                 doc=' H2n motor offset for C [mm]')
-    h2nSi = FCpt(OffsetIMSWithPreset, prefix='{self._prefix}:H2N:OFF_Si',
+    h2nSi = FCpt(OffsetMotor, prefix='{self._prefix}:H2N:OFF_Si',
                  name='h2n_si', motor_prefix='{self._hutch_prefix}:MON:MMS:15',
                  add_prefix=('prefix', 'motor_prefix'), kind='normal',
                  doc='H2n motor offset for Si [mm]')
 
     tab_component_names = True
     tab_whitelist = ['is_diamond', 'is_silicon', 'get_reflection',
                      'get_material']
@@ -573,36 +573,36 @@
             status_info, 'x2', 'dial_position', 'value')
 
         th_units = get_status_value(
             status_info, 'th2', 'user_setpoint', 'units')
         th_user = get_status_float(
             status_info, 'th2', 'position')
         th_dial = get_status_float(
-            status_info,  'th2', 'dial_position', 'value')
+            status_info, 'th2', 'dial_position', 'value')
 
         chi_units = get_status_value(
             status_info, 'chi2', 'user_setpoint', 'units')
         chi_user = get_status_float(
-            status_info,  'chi2', 'position')
+            status_info, 'chi2', 'position')
         chi_dial = get_status_float(
-            status_info,  'chi2', 'dial_position', 'value')
+            status_info, 'chi2', 'dial_position', 'value')
 
         y_units = get_status_value(
             status_info, 'y2', 'user_setpoint', 'units')
         y_user = get_status_float(
-            status_info,  'y2', 'position')
+            status_info, 'y2', 'position')
         y_dial = get_status_float(
-            status_info,  'y2', 'dial_position', 'value')
+            status_info, 'y2', 'dial_position', 'value')
 
         hn_units = get_status_value(
             status_info, 'h2n', 'user_setpoint', 'units')
         hn_user = get_status_float(
-            status_info,  'h2n', 'position')
+            status_info, 'h2n', 'position')
         hn_dial = get_status_float(
-            status_info,  'h2n', 'dial_position', 'value')
+            status_info, 'h2n', 'dial_position', 'value')
 
         diode_units = get_status_value(
             status_info, 'diode2', 'user_setpoint', 'units')
         diode_user = get_status_float(
             status_info, 'diode2', 'position')
         diode_dial = get_status_float(
             status_info, 'diode2', 'dial_position', 'value')
@@ -685,15 +685,15 @@
             status_info, 'dh', 'position')
         dh_dial = get_status_float(
             status_info, 'dh', 'dial_position', 'value')
 
         dv_units = get_status_value(
             status_info, 'dv', 'user_setpoint', 'units')
         dv_user = get_status_float(
-            status_info,  'dv', 'position')
+            status_info, 'dv', 'position')
         dv_dial = get_status_float(
             status_info, 'dv', 'dial_position', 'value')
 
         dr_units = get_status_value(
             status_info, 'dr', 'user_setpoint', 'units')
         dr_user = get_status_float(
             status_info, 'dr', 'position')
@@ -909,14 +909,22 @@
         if length == 0:
             # don't bother transforming this
             # TODO maybe catch error in common.wave.. when send 0
             return 0
         energy = common.wavelength_to_energy(length) / 1000
         return self.PseudoPosition(energy=energy)
 
+    def setE(self, energy):
+        self.set_current_position(energy)
+        return
+
+    def status_info(self):
+        """Overwrites interface status_info to make things faster."""
+        return None
+
     def format_status_info(self, status_info):
         """Override status info handler to render the energy si."""
         hutch = ''
         if 'XPP' in self.prefix:
             hutch = 'XPP '
         elif 'XCS' in self.prefix:
             hutch = 'XCS '
@@ -931,25 +939,25 @@
         elif material == 'Si':
             configuration = 'Silicon'
         else:
             configuration = 'Unknown'
 
         try:
             energy = self.get_energy()
-            energy = "{:.4f}".format(energy)
+            energy = f"{energy:.4f}"
         except Exception:
             energy = 'Unknown'
 
         try:
             ref = self.get_reflection()
             ref = ''.join(map(str, ref))
         except Exception:
             ref = 'Unknown'
 
-            return f"""\
+        return f"""\
 {hutch}LODCM Energy Si
 Current Configuration: {configuration} ({ref})
 Photon Energy: {energy} [keV]
 """
 
 
 class LODCMEnergyC(FltMvInterface, PseudoPositioner, GroupDevice):
@@ -1129,14 +1137,22 @@
         if length == 0:
             # don't bother transforming this
             # TODO maybe catch error in common.wave.. when send 0
             return 0
         energy = common.wavelength_to_energy(length) / 1000
         return self.PseudoPosition(energy=energy)
 
+    def setE(self, energy):
+        self.set_current_position(energy)
+        return
+
+    def status_info(self):
+        """Overwrites interface status_info to make things faster."""
+        return None
+
     def format_status_info(self, status_info):
         """Override status info handler to render the energy c."""
         hutch = ''
         if 'XPP' in self.prefix:
             hutch = 'XPP '
         elif 'XCS' in self.prefix:
             hutch = 'XCS '
@@ -1151,25 +1167,25 @@
         elif material == 'Si':
             configuration = 'Silicon'
         else:
             configuration = 'Unknown'
 
         try:
             energy = self.get_energy()
-            energy = "{:.4f}".format(energy)
+            energy = f"{energy:.4f}"
         except Exception:
             energy = 'Unknown'
 
         try:
             ref = self.get_reflection()
             ref = ''.join(map(str, ref))
         except Exception:
             ref = 'Unknown'
 
-            return f"""\
+        return f"""\
 {hutch}LODCM Energy C
 Current Configuration: {configuration} ({ref})
 Photon Energy: {energy} [keV]
 """
 
 
 class LODCM(BaseInterface, GroupDevice, LightpathMixin):
@@ -1214,15 +1230,16 @@
     energy_si = FCpt(LODCMEnergySi, '{self._prefix}', kind='normal')
     energy_c = FCpt(LODCMEnergyC, '{self._prefix}', kind='normal')
     # QIcon for UX
     _icon = 'fa.share-alt-square'
 
     tab_whitelist = ['h1n_state', 'yag', 'dectris', 'diode', 'foil',
                      'remove_dia', 'tower1', 'tower2',
-                     'diag_tower', 'calc']
+                     'diag_tower', 'calc', 'E', 'EC', 'ESi', 'tweak_x',
+                     'tweakXC']
 
     lightpath_cpts = ['tower1.h1n_state.state']
 
     def __init__(self, prefix, *, name, main_line='MAIN', mono_line='MONO',
                  **kwargs):
         self._prefix = prefix
         self._hutch_prefix = ''
@@ -1260,15 +1277,15 @@
         # states
         self.h1n_state = self.tower1.h1n_state
         self.y1_state = self.tower1.y1_state
         self.chi1_state = self.tower1.chi1_state
         self.h2n_state = self.tower2.h2n_state
         self.y2_state = self.tower2.y2_state
         self.chi2_state = self.tower2.chi2_state
-        # # offset positioners - tower 1
+        # offset positioners - tower 1
         self.th1Si = self.energy_si.th1Si
         self.z1Si = self.energy_si.z1Si
         self.th1C = self.energy_c.th1C
         self.z1C = self.energy_c.z1C
 
         self.x1C = self.tower1.x1C
         self.x1Si = self.tower1.x1Si
@@ -1276,41 +1293,49 @@
         self.y1Si = self.tower1.y1Si
         self.chi1C = self.tower1.chi1C
         self.chi1Si = self.tower1.chi1Si
         self.h1nC = self.tower1.h1nC
         self.h1nSi = self.tower1.h1nSi
         self.h1pC = self.tower1.h1pC
         self.h1pSi = self.tower1.h1pSi
-        # # offset positioners - tower 2
+        # offset positioners - tower 2
         self.th2Si = self.energy_si.th2Si
         self.z2Si = self.energy_si.z2Si
         self.th2C = self.energy_c.th2C
         self.z2C = self.energy_c.z2C
 
         self.x2C = self.tower2.x2C
         self.x2Si = self.tower2.x2Si
         self.y2C = self.tower2.y2C
         self.y2Si = self.tower2.y2Si
         self.chi2C = self.tower2.chi2C
         self.chi2Si = self.tower2.chi2Si
         self.h2nC = self.tower2.h2nC
         self.h2nSi = self.tower2.h2nSi
 
+        # energy aliases
+        self.EC = self.energy_c
+        self.ESi = self.energy_si
+
     @property
     def energy(self):
         material = self.get_material()
         if material == 'C':
             return self.energy_c
         elif material == 'Si':
             return self.energy_si
         # return energy_c as default if could not determine the material
         # TODO consider "energy" proxy motor object that picks where to
         # forward the commands instead of this property
         return self.energy_c
 
+    @property
+    def E(self):
+        return self.energy
+
     def calc_lightpath_state(
         self,
         tower1_h1n_state_state: Union[int, str]
     ) -> LightpathState:
         return LightpathState(
             inserted=True,
             removed=True,
@@ -1567,14 +1592,17 @@
                            "Check the motors, now at: %f, deadband %f" % (
                                start_x + x_value, end_x, self.x2.position))
         if abs(dz - z_value) > self.tower2.z2_retry_deadband.get():
             logger.warning("z2 did not reach the desired position of %f! "
                            "Check the motors, now at %f, deadband %f" % (
                                start_z + z_value, end_z, self.z2.position))
 
+    def tweakXC(self, x, wait=False):
+        self.tweak_x(x, material='C', wait=wait)
+
     def tweak_parallel(self, p_value, material=None, wait=False):
         """
         Tweak the `x2` and `z2` motors.
 
         Parameters
         ----------
         p_value : number
@@ -1639,15 +1667,15 @@
         elif material == 'Si':
             configuration = 'Silicon'
         else:
             configuration = 'Unknown'
 
         try:
             energy = self.get_energy()
-            energy = "{:.4f}".format(energy)
+            energy = f"{energy:.4f}"
         except Exception:
             energy = 'Unknown'
 
         try:
             ref = self.get_reflection()
             ref = ''.join(map(str, ref))
         except Exception:
@@ -1943,19 +1971,22 @@
                 output={'L0': 0}
             )
 
         inserted = self.tower1.h1n_state.check_inserted(h1n_state)
         removed = self.tower1.h1n_state.check_removed(h1n_state)
 
         if inserted and not removed:
-            output = {'L0': 0.5,
-                      'L1': 0.5}
+            # ignore attenuation from the LODCM splitting beam
+            output = {'L0': 1,
+                      'L2': 1}
         elif not inserted and removed:
+            # if removed, full transmission through L0
             output = {'L0': 1}
         else:
+            # for unknown states, mark as blocking
             output = {'L0': 0}
 
         return LightpathState(
             inserted=inserted,
             removed=removed,
             output=output
         )
```

### Comparing `pcdsdevices-7.1.0/pcdsdevices/lxe.py` & `pcdsdevices-7.4.0/pcdsdevices/lxe.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,17 +48,15 @@
 from .sim import FastMotor
 from .utils import convert_unit, get_status_float, get_status_value
 
 if typing.TYPE_CHECKING:
     import matplotlib  # noqa
 
 
-def load_calibration_file(
-        filename: typing.Union[pathlib.Path, str]
-        ) -> np.ndarray:
+def load_calibration_file(filename: typing.Union[pathlib.Path, str]) -> np.ndarray:
     """
     Load a calibration file.
 
     Data will be sorted by position and need not be pre-sorted.
 
     Two columns of data in a space-delimited text file.  No header:
         Column 1: waveplate position [mm?]
@@ -81,15 +79,15 @@
                             ])
 
 
 class LaserEnergyPlotContext:
     table: np.ndarray
     figure: 'matplotlib.figure.Figure'
     pyplot: types.ModuleType  # matplotlib.pyplot
-    column_names: typing.Tuple[str, ...]
+    column_names: tuple[str, ...]
     _subplot: 'matplotlib.axes._subplots.AxesSubplot'
 
     def __init__(self, *,
                  table: np.ndarray,
                  column_names: typing.Sequence[str]):
         self.table = table
```

### Comparing `pcdsdevices-7.1.0/pcdsdevices/make_ophyd_device.py` & `pcdsdevices-7.4.0/pcdsdevices/make_ophyd_device.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,23 +40,23 @@
     lines.append(s.format(suffix.lower(), suffix))
 
 
 def make_class_name(pv):
     """
     Make a class name based on a given PV.
     """
-    return '{}'.format(pv.title())
+    return f'{pv.title()}'
 
 
 def make_class_line(name, lines):
     """
     Make the first line of a class definition, based on a given PV or name.
     Appends the generated line to a list of lines.
     """
-    s = 'class {}(BaseInterface, Device):'.format(make_class_name(name))
+    s = f'class {make_class_name(name)}(BaseInterface, Device):'
     lines.append(s)
 
 
 def make_cpt(name, lines):
     """
     Make a component line for a sub-class, based on the supplied name.
     Appends the generated line to a list of lines.
```

### Comparing `pcdsdevices-7.1.0/pcdsdevices/mirror.py` & `pcdsdevices-7.4.0/pcdsdevices/mirror.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 This module contains all the classes relating to the offset mirrors used in the
 FEE and XRT. Each offset mirror contains a stepper motor and piezo motor to
 control the pitch, and two pairs of motors to control the horizontal and
 vertical gantries.
 """
 import logging
-from typing import List, Tuple, Union
+from typing import Union
 
 import numpy as np
 from lightpath import LightpathState
 from ophyd import Component as Cpt
 from ophyd import Device, EpicsSignal, EpicsSignalRO
 from ophyd import FormattedComponent as FCpt
 from ophyd import PVPositioner
@@ -78,15 +78,15 @@
         LimitError
             If the position is outside the soft limits.
         """
 
         # Check that we do not have a NaN or an Inf as those will
         # will make the PLC very unhappy ...
         if position is None or np.isnan(position) or np.isinf(position):
-            raise ValueError("Invalid value inputted: '{0}'".format(position))
+            raise ValueError(f"Invalid value inputted: '{position}'")
         # Use the built-in PVPositioner check_value
         super().check_value(position)
 
 
 class Pitch(OMMotor):
     """
     HOMS Pitch Mechanism.
@@ -408,17 +408,17 @@
     # that of the bare signal (x_up.user_readback -> x_up)
     lightpath_cpts = ['x_up.user_readback', 'y_up.user_readback',
                       'pitch.user_readback']
 
     def __init__(
         self,
         *args,
-        x_ranges: List[List[int]] = [],
-        y_ranges: List[List[int]] = [],
-        pitch_ranges: List[List[List[int]]] = [],
+        x_ranges: list[list[int]] = [],
+        y_ranges: list[list[int]] = [],
+        pitch_ranges: list[list[list[int]]] = [],
         **kwargs
     ) -> None:
         # insertion status, [[min_x_out, max_x_out], [min_x_in, max_x_in]]
         self.x_ranges = x_ranges
         # coating status.  (n_coatings * 2) array
         # [ [min_y_coat1, max_y_coat1],
         #   [min_y_coat2, max_y_coat2],
@@ -501,17 +501,17 @@
                 inserted=False,
                 removed=False,
                 output={self.output_branches[0]: 0}
             )
 
     def _find_matching_range_indices(
         self,
-        ranges: List[List[numeric]],
+        ranges: list[list[numeric]],
         value: numeric
-    ) -> List[bool]:
+    ) -> list[bool]:
         """
         Helper function for finding the range a particular value falls into
 
         Parameters
         ----------
         ranges : List[List[numeric]]
             A list of ranges.  Each range has a max and min value (exclusive)
@@ -528,15 +528,15 @@
             raise MirrorLogicError(
                 "Provided ranges must be a list of ranges (min, max).  "
                 f"Received an array of shape: {np.shape(ranges)}"
             )
 
         return [limit[0] < value < limit[1] for limit in ranges]
 
-    def _get_insertion_state(self, x: float) -> Tuple[bool, bool]:
+    def _get_insertion_state(self, x: float) -> tuple[bool, bool]:
         """
         Interpret x-position as inserted or removed, based on ranges
         provided at init.
 
         Assumes first range is OUT, second range is IN
 
         Parameters
@@ -770,14 +770,19 @@
     bender_ds_enc_rms = Cpt(PytmcSignal, ':ENC:DS:RMS', io='i',
                             kind='normal')
 
     # Bender RTD Cpts:
     us_rtd = Cpt(EpicsSignalRO, ':RTD:US:1_RBV', kind='normal')
     ds_rtd = Cpt(EpicsSignalRO, ':RTD:DS:1_RBV', kind='normal')
 
+    # Cooling
+    cool_flow1 = Cpt(EpicsSignalRO, ':FWM:1_RBV', kind='normal')
+    cool_flow2 = Cpt(EpicsSignalRO, ':FWM:2_RBV', kind='normal')
+    cool_press = Cpt(EpicsSignalRO, ':PRSM:1_RBV', kind='normal')
+
     # Tab config: show components
     tab_component_names = True
 
     def calc_lightpath_state(
         self,
         x_up: float,
         y_up: float,
@@ -1056,18 +1061,18 @@
     ----------
     prefix : str
         Base PV for the mirror.
 
     name : str
         Alias for the device.
     """
-    # Cooling water flow and pressure sensors
-    cool_flow1 = Cpt(EpicsSignalRO, ':FLOW:1_RBV', kind='normal')
-    cool_flow2 = Cpt(EpicsSignalRO, ':FLOW:2_RBV', kind='normal')
-    cool_press = Cpt(EpicsSignalRO, ':PRESS:1_RBV', kind='normal')
+    # Cooling water flow and pressure meters
+    cool_flow1 = Cpt(EpicsSignalRO, ':FWM:1_RBV', kind='normal')
+    cool_flow2 = Cpt(EpicsSignalRO, ':FWM:2_RBV', kind='normal')
+    cool_press = Cpt(EpicsSignalRO, ':PRSM:1_RBV', kind='normal')
 
     # Tab config: show components
     tab_component_names = True
 
 
 class FFMirror(BaseInterface, GroupDevice, LightpathMixin):
     """
@@ -1278,25 +1283,23 @@
     """
     coating = Cpt(TwinCATMirrorStripe, ':COATING:STATE', kind='hinted',
                   doc='Control of the coating states via saved positions.')
     # Tab config: show components
     tab_component_names = True
 
 
-class CoatingState(Device):
-    """
-    Extra parent class to put "coating" as the first device in order.
-
-    This makes it appear at the top of the screen in typhos.
-    """
-    coating = Cpt(TwinCATMirrorStripe, ':COATING:STATE', kind='hinted',
-                  doc='Control of the coating states via saved positions.')
-
-
-class XOffsetMirrorState(XOffsetMirror, CoatingState):
+@reorder_components(
+    end_with=[
+        'coating', 'y_up', 'x_up', 'pitch', 'bender', 'y_dwn',
+        'x_dwn', 'gantry_x', 'gantry_y', 'couple_y', 'couple_x', 'decouple_y',
+        'decouple_x', 'couple_status_y', 'couple_status_x', 'y_enc_rms',
+        'x_enc_rms', 'pitch_enc_rms', 'bender_enc_rms'
+    ]
+)
+class XOffsetMirrorState(XOffsetMirror):
     """
     X-ray Offset Mirror with Yleft/Yright
 
     1st and 2nd gen Axilon designs with LCLS-II Beckhoff motion architecture.
 
     With Coating State selection implemented
 
@@ -1304,14 +1307,17 @@
     ----------
     prefix : str
         Base PV for the mirror.
 
     name : str
         Alias for the device.
     """
+    coating = Cpt(TwinCATMirrorStripe, ':COATING:STATE', kind='hinted',
+                  doc='Control of the coating states via saved positions.')
+
     # UI representation
     _icon = 'fa.minus-square'
 
     lightpath_cpts = ['x_up.user_readback', 'coating.state',
                       'pitch.user_readback']
 
     def _get_coating_index(self, y: int) -> int:
@@ -1343,14 +1349,38 @@
         x_up: float,
         coating_state: int,
         pitch: float
     ) -> LightpathState:
         return self._calc_lightpath_state(x_up, coating_state, pitch)
 
 
+class XOffsetMirrorStateCool(XOffsetMirrorState):
+    """
+    X-ray Offset Mirror with Yleft/Yright
+
+    1st and 2nd gen Axilon designs with LCLS-II Beckhoff motion architecture.
+
+    With Coating State selection implemented.
+
+    With cooling and pressure meters installed.
+
+    Parameters
+    ----------
+    prefix : str
+        Base PV for the mirror.
+
+    name : str
+        Alias for the device.
+    """
+    # Cooling
+    cool_flow1 = Cpt(EpicsSignalRO, ':FWM:1_RBV', kind='normal')
+    cool_flow2 = Cpt(EpicsSignalRO, ':FWM:2_RBV', kind='normal')
+    cool_press = Cpt(EpicsSignalRO, ':PRSM:1_RBV', kind='normal')
+
+
 class MirrorInsertState(TwinCATStatePMPS):
     """
     A state positioner with two states (3 including Unknown) representing
     insertion state of mirror
     """
     _in_if_not_out = True
 
@@ -1375,15 +1405,15 @@
 
     lightpath_cpts = ['insertion.state', 'coating.state',
                       'pitch.user_readback']
 
     def _get_insertion_state(
         self,
         insertion_state: int
-    ) -> Tuple[bool, bool]:
+    ) -> tuple[bool, bool]:
         """
         return insertion state, given presence of state PV's
 
         Parameters
         ----------
         insertion_state : int
             insertion state (0: unknown, 1: out, 2: in)
```

### Comparing `pcdsdevices-7.1.0/pcdsdevices/movablestand.py` & `pcdsdevices-7.4.0/pcdsdevices/movablestand.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.1.0/pcdsdevices/mpod.py` & `pcdsdevices-7.4.0/pcdsdevices/mpod.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.1.0/pcdsdevices/mpod_apalis.py` & `pcdsdevices-7.4.0/pcdsdevices/mpod_apalis.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.1.0/pcdsdevices/mps.py` & `pcdsdevices-7.4.0/pcdsdevices/mps.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,15 +101,15 @@
 
     veto : bool, optional
         Whether or not the the device is capable of vetoing downstream faults.
     """
 
     # Signals
     fault = Cpt(EpicsSignalRO, '_MPSC', kind='hinted')
-    bypass = Cpt(EpicsSignal,   '_BYPS', kind='config')
+    bypass = Cpt(EpicsSignal, '_BYPS', kind='config')
 
     tab_whitelist = ['faulted', 'bypassed']
 
     @property
     def faulted(self):
         """Whether the MPS bit is faulted or not."""
         return bool(self.fault.get())
@@ -123,15 +123,15 @@
         """
         Subscribe to child signals
         """
         self.fault.subscribe(self._fault_change, run=False)
         self.bypass.subscribe(self._fault_change, run=False)
 
 
-def mps_factory(clsname, cls,  *args, mps_prefix, veto=False,  **kwargs):
+def mps_factory(clsname, cls, *args, mps_prefix, veto=False, **kwargs):
     """
     Create a new object of arbitrary class capable of storing MPS information.
 
     A new class identical to the provided one is created, but with additional
     attribute ``mps`` that relies upon the provided `.mps_prefix`. All other
     information is passed through to the class constructor as args and kwargs
```

### Comparing `pcdsdevices-7.1.0/pcdsdevices/mrco_motion.py` & `pcdsdevices-7.4.0/pcdsdevices/mrco_motion.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.1.0/pcdsdevices/piezo.py` & `pcdsdevices-7.4.0/pcdsdevices/piezo.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.1.0/pcdsdevices/pim.py` & `pcdsdevices-7.4.0/pcdsdevices/pim.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,16 +36,17 @@
     """
     Standard Y-motor for a Profile Intensity Monitor.
 
     This can move the stage to insert the YAG or diode, or retract from the
     beam path.
     """
 
-    states_list = ['DIODE', 'YAG', 'OUT']
-    in_states = ['YAG', 'DIODE']
+    # Automatically discover states (not all PIMs have DIODE)
+    states_list = []
+    _in_if_not_out = True
 
     _states_alias = {'YAG': 'IN'}
     # QIcon for UX
     _icon = 'fa.camera-retro'
 
     tab_whitelist = ['stage']
     _pre_stage_state = None
@@ -98,16 +99,18 @@
 
     lightpath_cpts = ['state']
 
     def infer_prefix(self, prefix):
         """Pulls out the first two segments of the prefix PV, if not already
            done"""
         if not self._prefix_start:
-            self._prefix_start = '{0}:{1}:'.format(prefix.split(':')[0],
-                                                   prefix.split(':')[1])
+            self._prefix_start = '{}:{}:'.format(
+                prefix.split(':')[0],
+                prefix.split(':')[1],
+            )
 
     def format_status_info(self, status_info):
         """
         Override status info handler to render the PIM.
 
         Display pim status info in the ipython terminal.
```

### Comparing `pcdsdevices-7.1.0/pcdsdevices/pmps.py` & `pcdsdevices-7.4.0/pcdsdevices/pmps.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.1.0/pcdsdevices/positioner.py` & `pcdsdevices-7.4.0/pcdsdevices/positioner.py`

 * *Files 3% similar despite different names*

```diff
@@ -78,19 +78,33 @@
 
     notepad_pv : str, optional
         If provided, a PV to put to whenever we move. This can be used to allow
         other elements in the control system to see what this positioner is
         doing.
     """
     def __init__(
-            self, *, name, move, get_pos, set_pos=None, stop=None, done=None,
-            check_value=None, info=None, egu='', limits=None, update_rate=1,
-            timeout=60, notepad_pv=None, parent=None, kind=None,
-            **kwargs
-            ):
+        self,
+        *,
+        name,
+        move,
+        get_pos,
+        set_pos=None,
+        stop=None,
+        done=None,
+        check_value=None,
+        info=None,
+        egu="",
+        limits=None,
+        update_rate=1,
+        timeout=60,
+        notepad_pv=None,
+        parent=None,
+        kind=None,
+        **kwargs
+    ):
         self._check_signature('move', move, 1)
         self._move = move
         self._check_signature('get_pos', get_pos, 0)
         self._get_pos = get_pos
         self._check_signature('set_pos', set_pos, 1)
         self._set_pos = set_pos
         self._check_signature('stop', stop, 0)
@@ -119,29 +133,29 @@
         sig = inspect.signature(func)
         try:
             sig.bind(*(0,) * nargs)
         except TypeError:
             raise ValueError(
                 f'FuncPositioner recieved {name} with an incorrect. '
                 f'signature. Must be able to take {nargs} args.'
-                ) from None
+            ) from None
 
     def _setup_move(self, position, status):
         self._run_subs(sub_type=self.SUB_START, timestamp=time.time())
         self._goal = position
         self._started_moving = True
         self._moving = True
         self._finished = False
         self._move(position)
         self._new_update(status)
 
     def _new_update(self, status):
         schedule_task(
             self._update_task, args=(status,), delay=self.update_rate
-            )
+        )
 
     def _update_task(self, status):
         self._update_position()
         if self._check_finished():
             self._started_moving = False
             self._moving = False
             self._update_position(force=True)
@@ -172,27 +186,25 @@
         if finished:
             self._done_moving()
         return finished
 
     def set_position(self, position):
         if self._set_pos is None:
             raise NotImplementedError(
-                f'FuncPositioner {self.name} was not '
-                'given a set_pos argument.'
-                )
+                f'FuncPositioner {self.name} was not given a set_pos argument.'
+            )
         else:
             self._set_pos(position)
 
     def stop(self, *args, **kwargs):
         if self._stop is None:
             # Often called by bluesky, don't throw an exception
             self.log.warning(
-                f'Called stop on FuncPositioner {self.name}, '
-                'but was not given a stop argument.'
-                )
+                f'Called stop on FuncPositioner {self.name}, but was not given a stop argument.'
+            )
         else:
             self._stop()
         super().stop(*args, **kwargs)
 
     def check_value(self, pos):
         super().check_value(pos)
         if self._check is not None:
```

### Comparing `pcdsdevices-7.1.0/pcdsdevices/pseudopos.py` & `pcdsdevices-7.4.0/pcdsdevices/pseudopos.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import copy
 import enum
 import logging
-import typing
+import time
 import warnings
 
 import numpy as np
 import ophyd
 import ophyd.pseudopos
 from ophyd.device import Component as Cpt
 from ophyd.device import FormattedComponent as FCpt
@@ -120,22 +120,27 @@
     * Makes scalar ``RealPosition`` and ``PseudoPosition`` easily convert
       to floating point values.
     * Adds a set_current_position helper method
 
     """ + ophyd.pseudopos.PseudoPositioner.__doc__
 
     def __init__(self, *args, **kwargs):
+        self._my_move = False
+        self._move_time = 0
+        self._my_move_timeout = 10
         super().__init__(*args, **kwargs)
 
         if len(self.RealPosition._fields) == 1:
             self.RealPosition.__float__ = _as_float
 
         if len(self.PseudoPosition._fields) == 1:
             self.PseudoPosition.__float__ = _as_float
 
+        self._sub_our_move_checks()
+
     def _update_notepad_ioc(self, position, attr):
         """
         Update the notepad IOC with a fully-specified ``PseudoPos``.
 
         Parameters
         ----------
         position : PseudoPos
@@ -190,23 +195,26 @@
 
         ValueError
             On invalid positions.
 
         RuntimeError
             If motion fails other than timing out.
         '''
+        self._my_move = True
+        self._move_time = time.monotonic()
         status = super().move(position, wait=wait, timeout=timeout,
                               moved_cb=moved_cb)
         self._update_notepad_ioc(position, 'notepad_setpoint')
         return status
 
     def _update_position(self):
         """Update the pseudo position based on that of the real positioners."""
         position = super()._update_position()
-        self._update_notepad_ioc(position, 'notepad_readback')
+        if self._my_move:
+            self._update_notepad_ioc(position, 'notepad_readback')
         return position
 
     def set_current_position(self, position):
         """
         Adjust all offsets so that the pseudo position matches the input.
 
         This will raise an AttributeError if any of the real motors is missing
@@ -217,14 +225,43 @@
         position : PseudoPos
             The position
         """
         real_pos = self.forward(position)
         for motor, pos in zip(self._real, real_pos):
             motor.set_current_position(pos)
 
+    def _our_move_check(self, **kwargs):
+        """
+        If a different session moves this device, it's not our move!
+
+        This callback will set the self._my_move flag to False if the setpoint
+        updates far apart in time from our last move.
+
+        This will stop this instance from updating the notepad_readback
+        signals.
+        """
+        if time.monotonic() - self._move_time > self._my_move_timeout:
+            self._my_move = False
+
+    def _sub_our_move_checks(self):
+        """
+        Set up subscriptions for self._our_move_check
+        """
+        for positioner in self._pseudo:
+            try:
+                signal = getattr(positioner, 'notepad_setpoint', None)
+                if signal is None:
+                    continue
+                signal.subscribe(self._our_move_check)
+            except Exception as ex:
+                self.log.debug(
+                    'Failed to set up _our_move_check subscriptions.',
+                    exc_info=ex,
+                )
+
 
 class SyncAxesBase(FltMvInterface, PseudoPositioner):
     """
     Synchronized Axes.
 
     This class is deprecated. Use `SyncAxis` instead.
 
@@ -253,17 +290,17 @@
 
     def __init__(self, *args, **kwargs):
         warnings.warn(
             'SyncAxesBase is deprecated and will be removed in a future '
             'release. Please switch to SyncAxis.',
             DeprecationWarning)
         if self.__class__ is SyncAxesBase:
-            raise TypeError(('SyncAxesBase must be subclassed with '
-                             'the axes to synchronize included as '
-                             'components'))
+            raise TypeError(
+                "SyncAxesBase must be subclassed with the axes to synchronize included as components"
+            )
         super().__init__(*args, **kwargs)
         self._offsets = None
 
     def calc_combined(self, real_position):
         """
         Calculate the combined pseudo position.
 
@@ -438,45 +475,39 @@
         if self.sync_limits is not None:
             self.sync._limits = tuple(self.sync_limits)
 
     def _check_settings(self):
         """Mostly just a typo check."""
         if self.__class__ is SyncAxis:
             raise TypeError(
-                'SyncAxis must be subclassed with '
-                'the axes to synchronize included as '
-                'components'
-                )
+                "SyncAxis must be subclassed with the axes to synchronize included as components"
+            )
         try:
             self.offset_mode = SyncAxisOffsetMode(self.offset_mode)
         except ValueError:
             try:
                 self.offset_mode = SyncAxisOffsetMode[self.offset_mode]
             except KeyError:
-                raise ValueError(
-                    f'Invalid offset_mode: {self.offset_mode}'
-                    ) from None
+                raise ValueError(f'Invalid offset_mode: {self.offset_mode}') from None
         self._check_info_dict(self.offsets, 'offsets')
         self._check_info_dict(self.scales, 'scales')
         if (self.fix_sync_keep_still is not None
                 and self.fix_sync_keep_still not in self.component_names):
             raise ValueError(
-                f'Invalid fix_sync_keep_still == {self.fix_sync_keep_still}. '
-                'Must match a motor.'
-                )
+                f'Invalid fix_sync_keep_still == {self.fix_sync_keep_still}. Must match a motor.'
+            )
 
     def _check_info_dict(self, setting, info_kind):
         """Helper function to check that all keys in the dict are Cpts"""
         if setting is not None:
             for attr, _ in setting.items():
                 if attr not in self.component_names:
                     raise ValueError(
-                        f'Invalid key {attr} in {info_kind}. '
-                        'Must match a motor.'
-                        )
+                        f'Invalid key {attr} in {info_kind}. Must match a motor.'
+                    )
 
     def _fill_info_dict(self, setting, default, info_kind):
         """Helper function to fill default values into the dict"""
         if setting is None:
             setting = {}
         elif isinstance(setting, dict):
             setting = copy.copy(setting)
@@ -580,18 +611,15 @@
                 return False
         return True
 
     def consistency_warning(self):
         """
         Return the consistency warning text
         """
-        return (
-            f'{self.name} is in an inconsistent state. Call '
-            'set_current_position or fix_sync to resolve.'
-            )
+        return f'{self.name} is in an inconsistent state. Call set_current_position or fix_sync to resolve.'
 
     def fix_sync(self, confirm=True, wait=True, timeout=10):
         """
         Method to re-synchronize the axes via motion.
 
         This will move every motor except the one defined by the
         fix_sync_keep_still attribute, which will be used to define the
@@ -717,16 +745,17 @@
     delay = FCpt(PseudoSingleInterface, egu='{self.egu}', add_prefix=['egu'])
     user_offset = Cpt(NotepadLinkedSignal, ':OphydOffset',
                       notepad_metadata={'record': 'ao', 'default_value': 0.0})
     motor = None
 
     def __init__(self, *args, egu='s', n_bounces=2, invert=False, **kwargs):
         if self.__class__ is DelayBase:
-            raise TypeError(('DelayBase must be subclassed with '
-                             'a "motor" component, the real motor to move.'))
+            raise TypeError(
+                'DelayBase must be subclassed with a "motor" component, the real motor to move.'
+            )
         self.n_bounces = n_bounces
         if invert:
             self.n_bounces *= -1
         super().__init__(*args, egu=egu, **kwargs)
 
     @pseudo_position_argument   # TODO: upstream this fix
     def check_value(self, value):
@@ -824,16 +853,16 @@
             {'motor': Cpt(motor_class, '')}
         )
         delay_classes[motor_class] = cls
     return cls
 
 
 def delay_instance_factory(
-        prefix, motor_class, egu='s', n_bounces=2, invert=False, **kwargs
-        ):
+    prefix, motor_class, egu='s', n_bounces=2, invert=False, **kwargs
+):
     cls = delay_class_factory(motor_class)
     return cls(prefix, egu=egu, n_bounces=n_bounces, invert=invert, **kwargs)
 
 
 delay_instance_factory.__doc__ = DelayBase.__doc__
 
 
@@ -869,24 +898,24 @@
     invert : bool, optional
         If True, increasing the real motor will decrease the delay.
         If False (default), increasing the real motor will increase the delay.
     """
     motor = ICpt(PositionerBase)
 
     def __init__(
-            self, motor, name=None, egu='s', n_bounces=2, invert=False,
-            **kwargs,
-            ):
+        self, motor, name=None, egu='s', n_bounces=2, invert=False,
+        **kwargs,
+    ):
         if name is None:
             name = motor.name + '_delay_motor'
         super().__init__(
             motor.prefix, name=name,
             egu=egu, n_bounces=n_bounces, invert=invert,
             motor=motor, **kwargs,
-            )
+        )
 
 
 class SimDelayStage(DelayBase):
     motor = Cpt(FastMotor, init_pos=0, egu='mm')
 
 
 delay_classes[FastMotor] = SimDelayStage
@@ -915,20 +944,20 @@
     column_names : list of str
         List of column names, corresponding to the component attribute names.
         That is, if you have a real motor ``mtr = Cpt(EpicsMotor, ...)``,
         ``"mtr"`` should be in the list of column names of the table.
     """
 
     table: np.ndarray
-    column_names: typing.Tuple[str, ...]
-    _table_data_by_name: typing.Dict[str, np.ndarray]
+    column_names: tuple[str, ...]
+    _table_data_by_name: dict[str, np.ndarray]
 
     def __init__(self, *args,
                  table: np.ndarray,
-                 column_names: typing.List[str],
+                 column_names: list[str],
                  **kwargs):
         super().__init__(*args, **kwargs)
         self.table = table
         self.column_names = tuple(column_names)
         missing = set()
         for positioner in self._real + self._pseudo:
             if positioner.attr_name not in column_names:
```

### Comparing `pcdsdevices-7.1.0/pcdsdevices/pulsepicker.py` & `pcdsdevices-7.4.0/pcdsdevices/pulsepicker.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.1.0/pcdsdevices/pump.py` & `pcdsdevices-7.4.0/pcdsdevices/pump.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.1.0/pcdsdevices/pv_positioner.py` & `pcdsdevices-7.4.0/pcdsdevices/pv_positioner.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.1.0/pcdsdevices/radiation.py` & `pcdsdevices-7.4.0/pcdsdevices/radiation.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.1.0/pcdsdevices/ref.py` & `pcdsdevices-7.4.0/pcdsdevices/ref.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.1.0/pcdsdevices/rs_powersupply.py` & `pcdsdevices-7.4.0/pcdsdevices/rs_powersupply.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,15 +13,14 @@
     Parameters
     ----------
     prefix: str
         The base PV of the relevant Rohde-Schwarz channel.
     name: str, keyword-only
         A name to refer to the relevant Rohde-Schwarz channel.
     """
-
     current = Cpt(EpicsSignal, 'CURR', kind='normal',
                   doc='Current Setpoint in Amps')
     current_step = Cpt(EpicsSignal, 'CURR_STEP', write_pv='CURR_STEP',
                        kind='hinted', doc='Step size for Current in Amps')
     current_twk = Cpt(EpicsSignal, 'CURR_TWK', kind='normal')
     select = Cpt(EpicsSignal, 'SELECT', kind='normal')
     set_current = Cpt(EpicsSignal, 'SET_CURR', write_pv='SET_CURR',
@@ -47,12 +46,20 @@
     Parameters
     ----------
     prefix: str
         The base PV of the relevant RohdeSchwarzPowersupply.
     name: str, keyword-only
         A name to refer to the relevant RohdeSchwazPowersupply.
     """
+    re_connect = Cpt(EpicsSignal, ':RECONNECT', kind='normal',
+                     doc='Connect button')
+    id = Cpt(EpicsSignal, ':IDN', kind='hinted',
+             doc='Device ID')
+    remote_mode = Cpt(EpicsSignal, ':MODE', kind='normal',
+                      doc='Remote mode')
+    output = Cpt(EpicsSignal, ':OUTPUT', kind='normal',
+                 doc='Turn on/off all channel outputs')
 
     ch1 = Cpt(RSChannel, ':1:', kind='normal')
     ch2 = Cpt(RSChannel, ':2:', kind='normal')
     ch3 = Cpt(RSChannel, ':3:', kind='normal')
     ch4 = Cpt(RSChannel, ':4:', kind='normal')
```

### Comparing `pcdsdevices-7.1.0/pcdsdevices/rtds_ebd.py` & `pcdsdevices-7.4.0/pcdsdevices/rtds_ebd.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,16 @@
+from lightpath import LightpathState
 from ophyd import Component as Cpt
 from ophyd import Signal
 
 from .device import GroupDevice
+from .epics_motor import BeckhoffAxis
 from .inout import InOutPositioner
-from .interface import BaseInterface, LightpathInOutCptMixin
-from .signal import PytmcSignal
+from .interface import BaseInterface, LightpathInOutCptMixin, LightpathMixin
+from .signal import EpicsSignalRO, PytmcSignal
 
 
 class PneumaticActuator(InOutPositioner):
     states_list = ['RETRACTED', 'INSERTED', 'MOVING', 'INVALID']
     in_states = ['INSERTED']
     out_states = ['RETRACTED']
     _invalid_states = ['MOVING', 'INVALID']
@@ -40,14 +42,35 @@
         """
         if state.name == 'INSERTED':
             self.in_cmd.put(1)
         elif state.name == 'RETRACTED':
             self.out_cmd.put(1)
 
 
+class RTDSX0ThreeStage(BaseInterface, LightpathMixin):
+    """Three stages X,Y,Z, for solid drilling experiments"""
+
+    mmsx = Cpt(BeckhoffAxis, ':MMS:X', kind='normal')
+    mmsy = Cpt(BeckhoffAxis, ':MMS:Y', kind='normal')
+    mmsz = Cpt(BeckhoffAxis, ':MMS:Z', kind='normal')
+
+    # Determine if the y stage is at it's outer limit switch
+    open_limit = Cpt(EpicsSignalRO, ':MMS:Y.HLS', kind='normal',
+                     doc='Reads if the y-stage is at its outer limit.')
+    lightpath_cpts = ['open_limit']
+
+    def calc_lightpath_state(self, open_limit=None):
+        # Logic, calculations using open_limit for y-stage
+        status = LightpathState(
+            inserted=not open_limit, removed=open_limit,
+            output={'K0' : 0.0}
+        )
+        return status
+
+
 class RTDSBase(BaseInterface, GroupDevice, LightpathInOutCptMixin):
     """Rapid Turnaround Diagnostic Station."""
     lightpath_cpts = ['mpa1', 'mpa2', 'mpa3', 'mpa4']
 
     _icon = 'fa.stop-circle'
 
     mpa1 = Cpt(PneumaticActuator, ':MPA:01', kind='normal')
```

### Comparing `pcdsdevices-7.1.0/pcdsdevices/sample_delivery.py` & `pcdsdevices-7.4.0/pcdsdevices/sample_delivery.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.1.0/pcdsdevices/sensors.py` & `pcdsdevices-7.4.0/pcdsdevices/sensors.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.1.0/pcdsdevices/sequencer.py` & `pcdsdevices-7.4.0/pcdsdevices/sequencer.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.1.0/pcdsdevices/signal.py` & `pcdsdevices-7.4.0/pcdsdevices/signal.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 import dataclasses
 import inspect
 import itertools
 import logging
 import numbers
 import typing
 from threading import RLock
-from typing import Any, Dict, Generator, List, Mapping, Optional, Tuple, Union
+from typing import Any, Generator, Mapping, Optional, Union
 
 import numpy as np
 import ophyd
 from ophyd.signal import (DEFAULT_WRITE_TIMEOUT, DerivedSignal, EpicsSignal,
                           EpicsSignalBase, EpicsSignalRO, Signal, SignalRO)
 from ophyd.sim import FakeEpicsSignal, FakeEpicsSignalRO, fake_device_cache
 from ophyd.utils import ReadOnlyError
@@ -153,15 +153,15 @@
 
     This signal type is intended to be used programmatically with a subclass.
     For simple per-device usage, see :class:`MultiDerivedSignal`.
     """
 
     _update_only_on_change: bool = True
     _has_subscribed: bool
-    _signals: Dict[Signal, _AggregateSignalState]
+    _signals: dict[Signal, _AggregateSignalState]
 
     def __init__(self, *, name, value=None, **kwargs):
         super().__init__(name=name, value=value, **kwargs)
         self._has_subscribed = False
         self._lock = RLock()
         self._signals = {}
 
@@ -316,15 +316,15 @@
             )
 
         # Only check connectivity status of the signal; cross fingers that it
         # reflects both being connected and having a not-None value.
         return all(signal.connected for signal in self._signals)
 
     @contextlib.contextmanager
-    def _check_connectivity(self) -> Generator[Dict[str, bool], None, None]:
+    def _check_connectivity(self) -> Generator[dict[str, bool], None, None]:
         """
         Context manager for checking connectivity.
 
         The block for the context manager should perform some operation
         to change the state of the signal.
 
         Returns state information as a dictionary, accessible after the
@@ -452,21 +452,21 @@
     def __init__(self, *, name, **kwargs):
         super().__init__(name=name, **kwargs)
         for attr_name in self.parent._state_logic:
             self.add_signal_by_attr_name(attr_name)
         self._has_setpoint_md = False
 
     @property
-    def enum_strs(self) -> Tuple[str, ...]:
+    def enum_strs(self) -> tuple[str, ...]:
         """
         Mimic the epics signal property for enum strings.
         """
         return tuple(state.name for state in self.parent.states_enum)
 
-    def describe(self) -> Dict[str, Dict[str, Any]]:
+    def describe(self) -> dict[str, dict[str, Any]]:
         """
         Make sure a reasonable description exists for bluesky scans.
         """
         # Base description information
         sub_sigs = [sig.name for sig in self._signals]
         desc = {
             'source': 'SUM:{}'.format(','.join(sub_sigs)),
@@ -698,15 +698,15 @@
                 f"MultiDerivedSignal.  It should take two parameters, "
                 f"'mds' and 'value' as either positional or keyword "
                 f"arguments. For {parent_name}.{self.attr_name}:"
                 f"{func_name}{sig}"
             )
 
     @property
-    def signals(self) -> List[Signal]:
+    def signals(self) -> list[Signal]:
         """The signals used to calculate_on_get this MultiDerivedSignal."""
         return list(self._signals)
 
     def _calc_readback(self) -> OphydDataType:
         """calculate_on_get the new readback value."""
         items = {sig: siginfo.value for sig, siginfo in self._signals.items()}
         return self.calculate_on_get(mds=self, items=items)
@@ -1118,21 +1118,24 @@
     **kwargs :
         Keyword arguments are passed to the superclass.
     """
 
     derived_units: str
     original_units: str
 
-    def __init__(self, derived_from, *,
-                 derived_units: str,
-                 original_units: typing.Optional[str] = None,
-                 user_offset: typing.Optional[numbers.Real] = 0,
-                 limits: typing.Optional[typing.Tuple[numbers.Real,
-                                                      numbers.Real]] = None,
-                 **kwargs):
+    def __init__(
+        self,
+        derived_from,
+        *,
+        derived_units: str,
+        original_units: typing.Optional[str] = None,
+        user_offset: typing.Optional[numbers.Real] = 0,
+        limits: typing.Optional[tuple[numbers.Real, numbers.Real]] = None,
+        **kwargs
+    ):
         self.derived_units = derived_units
         self.original_units = original_units
         self._user_offset = user_offset
         self._custom_limits = limits
         super().__init__(derived_from, **kwargs)
         self._metadata['units'] = derived_units
 
@@ -1254,15 +1257,15 @@
         """
         for key in md.keys():
             if key not in self._metadata_keys:
                 raise ValueError(
                     f'Tried to override metadata key {key} in {self.name}, '
                     'but this is not one of the metadata keys: '
                     f'{self._metadata_keys}'
-                    )
+                )
         try:
             self._metadata_override.update(**md)
         except AttributeError:
             self._metadata_override = md
         self._run_metadata_callbacks()
 
     @property
```

### Comparing `pcdsdevices-7.1.0/pcdsdevices/sim.py` & `pcdsdevices-7.4.0/pcdsdevices/sim.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.1.0/pcdsdevices/slits.py` & `pcdsdevices-7.4.0/pcdsdevices/slits.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 from ophyd.signal import Signal, SignalRO
 from ophyd.status import Status
 from ophyd.status import wait as status_wait
 
 from .areadetector.detectors import PCDSAreaDetectorTyphosTrigger
 from .device import GroupDevice
 from .device import UpdateComponent as UpCpt
-from .epics_motor import BeckhoffAxis, BeckhoffAxisNoOffset
+from .epics_motor import BeckhoffAxis, BeckhoffAxisNoOffset, PCDSMotorBase
 from .interface import (BaseInterface, FltMvInterface, LightpathInOutCptMixin,
                         LightpathMixin, MvInterface)
 from .pmps import TwinCATStatePMPS
 from .sensors import RTD, TwinCATTempSensor
 from .signal import NotImplementedSignal, PytmcSignal
 from .sim import FastMotor
 from .utils import get_status_float, get_status_value, schedule_task
@@ -261,15 +261,15 @@
         Restore the initial values of the aperture position.
         """
         if self._pre_stage_gap is not None:
             self.move(
                 self._pre_stage_gap[0],
                 self._pre_stage_gap[1],
                 wait=True
-                )
+            )
         self._pre_stage_gap = None
         return super().unstage()
 
     def subscribe(self, cb, event_type=None, run=True):
         """
         Subscribe to changes of the slits.
         Parameters
@@ -292,15 +292,15 @@
             self._has_subscribed = True
         return super().subscribe(cb, event_type=event_type, run=run)
 
     def _aperture_changed(self, *args, **kwargs):
         """Callback run when slit size is adjusted."""
         # Avoid duplicate keywords
         kwargs.pop('sub_type', None)
-        kwargs.pop('obj',      None)
+        kwargs.pop('obj', None)
         # Run subscriptions
         self._run_subs(sub_type=self.SUB_STATE, obj=self, **kwargs)
 
     def calc_lightpath_state(
         self,
         xwidth: float,
         ywidth: float
@@ -420,20 +420,27 @@
 
     # Base class overrides
     xwidth = Cpt(LusiSlitPositioner, '', slit_type='XWIDTH', kind='hinted')
     ywidth = Cpt(LusiSlitPositioner, '', slit_type='YWIDTH', kind='hinted')
     xcenter = Cpt(LusiSlitPositioner, '', slit_type='XCENTER', kind='normal')
     ycenter = Cpt(LusiSlitPositioner, '', slit_type='YCENTER', kind='normal')
 
+    # Individual blade aliases
+    blade_top = Cpt(PCDSMotorBase, ':TOP', kind='normal')
+    blade_bottom = Cpt(PCDSMotorBase, ':BOTTOM', kind='normal')
+    blade_north = Cpt(PCDSMotorBase, ':NORTH', kind='normal')
+    blade_south = Cpt(PCDSMotorBase, ':SOUTH', kind='normal')
+
     # Local PVs
     blocked = Cpt(EpicsSignalRO, ':BLOCKED', kind='omitted')
     open_cmd = Cpt(EpicsSignal, ':OPEN', kind='omitted')
     close_cmd = Cpt(EpicsSignal, ':CLOSE', kind='omitted')
     block_cmd = Cpt(EpicsSignal, ':BLOCK', kind='omitted')
 
+    tab_whitelist = ['blade_top', 'blade_bottom', 'blade_north', 'blade_south']
     lightpath_cpts = ['xwidth.readback', 'ywidth.readback']
 
     def open(self):
         """Uses the built-in 'OPEN' record to move open the aperture."""
         self.open_cmd.put(1)
 
     def close(self):
@@ -592,16 +599,16 @@
                                             ywidth=ywidth_readback)
 
 
 def _rtd_fields(cls, attr_base, range_, **kwargs):
     padding = max(range_)//10 + 2
     defn = OrderedDict()
     for i in range_:
-        attr = '{attr}{i}'.format(attr=attr_base, i=i)
-        suffix = ':RTD:{i}'.format(i=str(i).zfill(padding))
+        attr = f'{attr_base}{i}'
+        suffix = f':RTD:{str(i).zfill(padding)}'
         defn[attr] = (cls, suffix, kwargs)
     return defn
 
 
 class PowerSlits(BeckhoffSlits):
     """
     'SL*:POWER'.
```

### Comparing `pcdsdevices-7.1.0/pcdsdevices/spectrometer.py` & `pcdsdevices-7.4.0/pcdsdevices/spectrometer.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from ophyd.device import FormattedComponent as FCpt
 
 from .device import GroupDevice
 from .epics_motor import (IMS, BeckhoffAxis, BeckhoffAxisNoOffset,
                           EpicsMotorInterface)
 from .interface import BaseInterface, LightpathMixin
 from .signal import InternalSignal, PytmcSignal
+from .state import StateRecordPositioner
 
 
 class Kmono(BaseInterface, GroupDevice, LightpathMixin):
     """
     K-edge Monochromator: Used for Undulator tuning and other experiments.
 
     This device has 3 main members: the crystal (xtal), the reticle
@@ -259,21 +260,21 @@
     led_power_1 = Cpt(PytmcSignal, ':LED:01:PWR', io='io', kind='config',
                       doc='LED power supply controls.')
     led_power_2 = Cpt(PytmcSignal, ':LED:02:PWR', io='io', kind='config',
                       doc='LED power supply controls.')
     led_power_3 = Cpt(PytmcSignal, ':LED:03:PWR', io='io', kind='config',
                       doc='LED power supply controls.')
 
-    # Flow switches
-    flow_1 = Cpt(PytmcSignal, ':FSW:01', io='i', kind='normal',
-                 doc='flow switch 1')
-    flow_2 = Cpt(PytmcSignal, ':FSW:02', io='i', kind='normal',
-                 doc='flow switch 2')
-    pres_1 = Cpt(PytmcSignal, ':P1', io='i', kind='normal',
-                 doc='pressure sensor 1')
+    # Flow meters
+    flow_1 = Cpt(PytmcSignal, ':FWM:1', io='i', kind='normal',
+                 doc='flow meter 1')
+    flow_2 = Cpt(PytmcSignal, ':FWM:2', io='i', kind='normal',
+                 doc='flow meter 2')
+    pres_1 = Cpt(PytmcSignal, ':PRSM:1', io='i', kind='normal',
+                 doc='pressure meter 1')
 
     # RTDs
     rtd_1 = Cpt(PytmcSignal, ':RTD:01:TEMP', io='i', kind='normal',
                 doc='RTD 1 [deg C]')
     rtd_2 = Cpt(PytmcSignal, ':RTD:02:TEMP', io='i', kind='normal',
                 doc='RTD 2 [deg C]')
     rtd_3 = Cpt(PytmcSignal, ':RTD:03:TEMP', io='i', kind='normal',
@@ -378,16 +379,15 @@
               doc='camera angle')
     camd = Cpt(IMS, ':444:MOTR', kind='normal',
                doc='camera distance')
     camy = Cpt(IMS, ':447:MOTR', kind='normal',
                doc='camera y')
     iris = Cpt(IMS, ':445:MOTR', kind='normal',
                doc='camera iris')
-    filter = Cpt(IMS, ':446:MOTR', kind='normal',
-                 doc='filter wheel, tbd if necessary')
+    filter = FCpt(StateRecordPositioner, 'XRT:HXS:FILTER', doc='filter wheel')
 
     # Lightpath constants
     inserted = True
     removed = False
     transmission = 1
     SUB_STATE = 'state'
```

### Comparing `pcdsdevices-7.1.0/pcdsdevices/state.py` & `pcdsdevices-7.4.0/pcdsdevices/state.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 Module to define positioners that move between discrete named states.
 """
 from __future__ import annotations
 
 import copy
 import functools
 import logging
-from typing import Any, ClassVar, Dict, List, Optional
+from typing import Any, ClassVar
 
 from ophyd.device import Component as Cpt
 from ophyd.device import Device, required_for_connection
 from ophyd.positioner import PositionerBase
 from ophyd.signal import EpicsSignal
 from ophyd.sim import fake_device_cache, make_fake_device
 from ophyd.status import SubscriptionStatus
@@ -80,16 +80,15 @@
     _default_sub = SUB_STATE
     _state_meta_sub = EpicsSignal.SUB_VALUE
 
     egu = 'state'
 
     def __init__(self, prefix, *, name, **kwargs):
         if self.__class__ is StatePositioner:
-            raise TypeError(('StatePositioner must be subclassed with at '
-                             'least a state signal'))
+            raise TypeError('StatePositioner must be subclassed with at least a state signal')
         self._state_initialized = False
         self._has_subscribed_state = False
         super().__init__(prefix, name=name, **kwargs)
         if self.states_list:
             self._state_init()
 
     def __init_subclass__(cls, **kwargs):
@@ -109,15 +108,15 @@
             if not hasattr(self, 'states_enum'):
                 self.states_enum = self._create_states_enum()
             self._state_initialized = True
 
     def _late_state_init(
         self,
         *args,
-        enum_strs: Optional[List[str]] = None,
+        enum_strs: list[str] | None = None,
         **kwargs
     ):
         if enum_strs is not None and not self.states_list:
             self.states_list = list(enum_strs)
             # Unknown state reserved for slot zero, automatically added later
             # Removing and auto re-adding *feels* silly, but it was easy to do
             if self._unknown:
@@ -308,17 +307,18 @@
                 state_def[aliases] = i
             else:
                 for alias in aliases:
                     state_def[alias] = i
         enum_name = self.__class__.__name__ + 'States'
         enum = HelpfulIntEnum(enum_name, state_def, start=0, module=__name__)
         if len(enum) != state_count:
-            raise ValueError(('Bad states definition! Inconsistency in '
-                              'states_list {} or _states_alias {}'
-                              ''.format(self.states_list, self._states_alias)))
+            raise ValueError(
+                'Bad states definition! Inconsistency in states_list {} or _states_alias {}'
+                ''.format(self.states_list, self._states_alias)
+            )
         return enum
 
     @property
     def stop(self):
         """
         Hide the stop method behind an AttributeError.
 
@@ -368,35 +368,37 @@
         metadata on the state signal if provided.
     """
 
     __doc__ = __doc__ % basic_positioner_init
 
     state = Cpt(PVStateSignal, kind='hinted')
 
-    _state_logic: ClassVar[Dict[str, Dict[Any, str]]] = {}
+    _state_logic: ClassVar[dict[str, dict[Any, str]]] = {}
     _state_logic_mode: ClassVar[str] = 'ALL'
-    _state_logic_set_ref: ClassVar[Optional[str]] = None
+    _state_logic_set_ref: ClassVar[str | None] = None
 
     def __init__(self, prefix, *, name, **kwargs):
         if self.__class__ is PVStatePositioner:
-            raise TypeError(('PVStatePositioner must be subclassed, '
-                             'adding signals and filling in the '
-                             '_state_logic dict.'))
+            raise TypeError(
+                "PVStatePositioner must be subclassed, adding signals and filling in the "
+                "_state_logic dict."
+            )
         if self._state_logic and not self.states_list:
             self.states_list = []
             for state_mapping in self._state_logic.values():
                 for state_name in state_mapping.values():
                     if state_name not in (self._unknown, 'defer'):
                         if state_name not in self.states_list:
                             self.states_list.append(state_name)
         super().__init__(prefix, name=name, **kwargs)
 
     def _do_move(self, state):
-        raise NotImplementedError(('Class must implement a _do_move method or '
-                                   'override the move and set methods'))
+        raise NotImplementedError(
+            "Class must implement a _do_move method or override the move and set methods"
+        )
 
 
 class StateRecordPositionerBase(StatePositioner, GroupDevice):
     """
     A `StatePositioner` for an EPICS states record.
 
     `states_list` does not have to be provided.
@@ -611,15 +613,15 @@
     -------
     state_attr : str
         The corresponding attribute name.
     """
     return f'state{state_index:02}'
 
 
-def state_config_dotted_names(state_count: int) -> list[Optional[str]]:
+def state_config_dotted_names(state_count: int) -> list[str | None]:
     """
     Returns the full dotted names of the state config state_name components.
 
     This includes None for the Unknown state and is valid for use in
     EpicsSignalEditMD's enum_attrs argument, matching the structure found in
     TwinCATStatePositioner.
 
@@ -635,15 +637,15 @@
     """
     return [None] + [
         f'config.{get_dynamic_state_attr(num)}.state_name'
         for num in range(1, state_count + 1)
     ]
 
 
-def state_config_dotted_velos(state_count: int) -> list[Optional[str]]:
+def state_config_dotted_velos(state_count: int) -> list[str | None]:
     """
     Returns the full dotted names of the state config velo components.
 
     This does not include any entry for the unknown state and can be
     passed directly into the velocity summary MultiDerivedSignal attrs.
 
     Parameters
```

### Comparing `pcdsdevices-7.1.0/pcdsdevices/stopper.py` & `pcdsdevices-7.4.0/pcdsdevices/stopper.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.1.0/pcdsdevices/sxr_test_absorber.py` & `pcdsdevices-7.4.0/pcdsdevices/sxr_test_absorber.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.1.0/pcdsdevices/targets.py` & `pcdsdevices-7.4.0/pcdsdevices/targets.py`

 * *Files 0% similar despite different names*

```diff
@@ -627,18 +627,22 @@
         x_pos = self.x.position
         y_pos = self.y.position
         data = self.get_sample_data(self.current_sample)
         try:
             xx = data['xx']
             yy = data['yy']
 
-            x_index = next((index for (index, d) in enumerate(xx)
-                            if np.isclose(d["pos"], x_pos)))
-            y_index = next((index for (index, d) in enumerate(yy)
-                            if np.isclose(d["pos"], y_pos)))
+            x_index = next(
+                index for (index, d) in enumerate(xx)
+                if np.isclose(d["pos"], x_pos)
+            )
+            y_index = next(
+                index for (index, d) in enumerate(yy)
+                if np.isclose(d["pos"], y_pos)
+            )
         except Exception:
             logger.warning('Could not determine the m n points from position.')
         n_points = self.m_n_points[1]
 
         x_index += 1
         m = int(np.ceil(x_index / n_points))
         res = np.mod(x_index, 2 * n_points)
@@ -689,16 +693,15 @@
         sample_name : str
             Name of the sample to load.
         path : str, optional
             Path where the samples yaml file exists.
         """
         path = path or self._path
         entry = os.path.join(path, sample_name + '.yml')
-        m_points, n_points, coeffs = self.get_sample_map_info(
-                                            str(sample_name), path=entry)
+        m_points, n_points, coeffs = self.get_sample_map_info(str(sample_name), path=entry)
         self.m_n_points = m_points, n_points
         self.coefficients = coeffs
         # make this sample the current one
         self.current_sample = str(sample_name)
 
     def get_sample_data(self, sample_name, path=None):
         """
```

### Comparing `pcdsdevices-7.1.0/pcdsdevices/tests/conftest.py` & `pcdsdevices-7.4.0/pcdsdevices/tests/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import os
 import pkgutil
 import shutil
 import sys
 import warnings
 from pathlib import Path
 from types import ModuleType, SimpleNamespace
-from typing import Any, Callable, Dict, List, Optional
+from typing import Any, Callable, Optional
 
 import ophyd
 import pytest
 from epics import PV
 from ophyd.signal import LimitError
 from ophyd.sim import FakeEpicsSignal, make_fake_device
 
@@ -89,15 +89,15 @@
     os.makedirs(user)
     setup_preset_paths(hutch=hutch, user=user)
     yield
     setup_preset_paths()
     shutil.rmtree(folder)
 
 
-def find_pcdsdevices_submodules() -> Dict[str, ModuleType]:
+def find_pcdsdevices_submodules() -> dict[str, ModuleType]:
     """Find all pcdsdevices submodules, as a dictionary of name to module."""
     modules = {}
     package_root = str(MODULE_PATH.parent)
     for item in pkgutil.walk_packages(path=[package_root],
                                       prefix='pcdsdevices.'):
         try:
             modules[item.name] = sys.modules[item.name]
@@ -109,15 +109,15 @@
                 )
             except Exception:
                 logger.exception('Failed to import %s', item.name)
 
     return modules
 
 
-def find_all_classes(classes, skip: Optional[List[str]] = None) -> List[Any]:
+def find_all_classes(classes, skip: Optional[list[str]] = None) -> list[Any]:
     """Find all device classes in pcdsdevices and return them as a list."""
     skip = skip or []
 
     def should_include(obj):
         return (
             inspect.isclass(obj) and
             issubclass(obj, classes) and
@@ -135,25 +135,25 @@
         for _, obj in inspect.getmembers(module, predicate=should_include)
     ]
 
     return list(sorted(set(devices), key=sort_key))
 
 
 def find_all_device_classes(
-    skip: Optional[List[str]] = None
-) -> List[ophyd.Device]:
+    skip: Optional[list[str]] = None
+) -> list[ophyd.Device]:
     """
     Find all device classes in pcdsdevices and return them as a list.
     Skip any devices with their name in ``skip``
     """
     skip = skip or []
     return find_all_classes(ophyd.Device, skip=skip)
 
 
-def find_all_callables() -> List[Callable]:
+def find_all_callables() -> list[Callable]:
     """Find all callables in pcdsdevices and return them as a list."""
     def should_include(obj):
         try:
             name = obj.__name__
             module = obj.__module__
         except AttributeError:
             return False
```

### Comparing `pcdsdevices-7.1.0/pcdsdevices/tests/test_analog_signals.py` & `pcdsdevices-7.4.0/pcdsdevices/tests/test_analog_signals.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.1.0/pcdsdevices/tests/test_attenuator.py` & `pcdsdevices-7.4.0/pcdsdevices/tests/test_attenuator.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 import time
 from unittest.mock import Mock
 
 import pytest
 from ophyd.sim import make_fake_device
 from ophyd.status import wait as status_wait
 
-from ..attenuator import (AT1K4, AT2L0, MAX_FILTERS, AttBase, Attenuator,
-                          _att_classes)
+from ..attenuator import (AT1K2, AT1K4, AT2K2, AT2L0, MAX_FILTERS, AttBase,
+                          Attenuator, _att_classes)
 
 logger = logging.getLogger(__name__)
 
 
 # Replace all the Attenuator classes with fake classes
 for name, cls in _att_classes.items():
     _att_classes[name] = make_fake_device(cls)
@@ -165,24 +165,35 @@
 
 @pytest.mark.timeout(5)
 def test_attenuator_disconnected():
     AttBase('TST:ATT', name='test_att')
 
 
 @pytest.fixture(
-    params=['at2l0', 'at1k4']
+    params=['at2l0', 'at1k4', 'at1k2', 'at2k2']
 )
 def fake_new_attenuator(request):
-    """AT2L0, AT1K4 - attenuators new to LCLS-II."""
-    if request.param == 'at2l0':
+    """Attenuators new to LCLS-II."""
+    attname = request.param
+    if attname == 'at2l0':
         FakeAT2L0 = make_fake_device(AT2L0)
         return FakeAT2L0('AT2L0:', name='fake_at2l0')
-    FakeAT1K4 = make_fake_device(AT1K4)
-    return FakeAT1K4('AT1K4:', calculator_prefix='AT1K4:CALC',
-                     name='fake_at1k4')
+    if attname == 'at1k4':
+        FakeAT1K4 = make_fake_device(AT1K4)
+        return FakeAT1K4('AT1K4:', calculator_prefix='AT1K4:CALC',
+                         name='fake_at1k4')
+    if attname == 'at1k2':
+        FakeAT1K2 = make_fake_device(AT1K2)
+        return FakeAT1K2('AT1K2:', calculator_prefix='AT1K2:CALC',
+                         name='fake_at1k2')
+    if attname == 'at2k2':
+        FakeAT2K2 = make_fake_device(AT2K2)
+        return FakeAT2K2('AT2K2:', calculator_prefix='AT2K2:CALC',
+                         name='fake_at2k2')
+    raise RuntimeError(f'Unknown attenuator {attname}')
 
 
 def test_new_attenuator_smoke(fake_new_attenuator):
     fake_new_attenuator.setpoint
     fake_new_attenuator.readback
     fake_new_attenuator.actuate
     fake_new_attenuator(0.0)
```

### Comparing `pcdsdevices-7.1.0/pcdsdevices/tests/test_beam_stats.py` & `pcdsdevices-7.4.0/pcdsdevices/tests/test_beam_stats.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.1.0/pcdsdevices/tests/test_btms.py` & `pcdsdevices-7.4.0/pcdsdevices/tests/test_btms.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Optional, Tuple
+from typing import Optional
 
 import pytest
 
 from ..lasers.btms_config import (BtmsDestinationState, BtmsSourceState,
                                   BtmsState, DestinationInControlError,
                                   DestinationInUseError, DestinationPosition,
                                   MaintenanceModeActiveError,
@@ -44,15 +44,15 @@
             (DestinationPosition.ld7,),
         ),
     ],
 )
 def test_destination_position_path(
     dest1: DestinationPosition,
     dest2: DestinationPosition,
-    path: Tuple[DestinationPosition, ...],
+    path: tuple[DestinationPosition, ...],
 ):
     assert dest1.path_to(dest2) == path
 
 
 @pytest.mark.parametrize(
     "dest, top",
     [
@@ -368,18 +368,18 @@
         },
     )
 
     print(str(state))
 
     for source in state.sources:
         start_pos = state.sources[source].destination
-        other_destinations = set(
+        other_destinations = {
             state.sources[other].destination for other in state.sources
             if state.sources[other].destination != start_pos
-        )
+        }
         assert len(other_destinations) > 1
         for dest in other_destinations:
             if dest is not None:
                 print("Checking", source, start_pos, "->", dest)
                 with pytest.raises(DestinationInUseError):
                     state.check_move(source, start_pos, dest)
```

### Comparing `pcdsdevices-7.1.0/pcdsdevices/tests/test_ccm.py` & `pcdsdevices-7.4.0/pcdsdevices/tests/test_ccm.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.1.0/pcdsdevices/tests/test_crix_motion.py` & `pcdsdevices-7.4.0/pcdsdevices/tests/test_crix_motion.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.1.0/pcdsdevices/tests/test_dc_devices.py` & `pcdsdevices-7.4.0/pcdsdevices/tests/test_dc_devices.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.1.0/pcdsdevices/tests/test_device.py` & `pcdsdevices-7.4.0/pcdsdevices/tests/test_device.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.1.0/pcdsdevices/tests/test_disconnected.py` & `pcdsdevices-7.4.0/pcdsdevices/tests/test_disconnected.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.1.0/pcdsdevices/tests/test_epics_motor.py` & `pcdsdevices-7.4.0/pcdsdevices/tests/test_epics_motor.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.1.0/pcdsdevices/tests/test_gauge.py` & `pcdsdevices-7.4.0/pcdsdevices/tests/test_gauge.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.1.0/pcdsdevices/tests/test_gon.py` & `pcdsdevices-7.4.0/pcdsdevices/tests/test_gon.py`

 * *Files 1% similar despite different names*

```diff
@@ -200,28 +200,28 @@
     assert not status.success
 
 
 @pytest.mark.parametrize("eta,kappa,phi", [
     (0, 0, 0), (1, 2, 3), (10, 20, 30), (45, 45, 45),
     (6, 2, 6), (42, 0, 0), (0, 42, 0), (0, 0, 42),
     (7, 7, 7), (-1, -2, -3), (-10, 25, -30), (9, -1, 1),
-    ])
+])
 def test_kappa_calculations(fake_kappa, eta, kappa, phi):
     e_eta, e_chi, e_phi = fake_kappa.k_to_e(eta, kappa, phi)
     k_eta, k_kap, k_phi = fake_kappa.e_to_k(e_eta, e_chi, e_phi)
     assert np.isclose(eta, k_eta)
     assert np.isclose(kappa, k_kap)
     assert np.isclose(phi, k_phi)
 
 
 @pytest.mark.parametrize("eta,kappa,phi", [
     (0, 225, 0), (1, 227, 3), (10, 245, 30), (45, 270, 45),
     (6, 227, 6), (42, 225, 0), (0, 267, 0), (0, 225, 42),
     (7, 232, 7), (-1, 223, -3), (-10, 250, -30), (9, 224, 1),
-    ])
+])
 def test_kappa_calculations_big_kap(fake_kappa, eta, kappa, phi):
     fake_kappa.kappa.move(225, wait=True)
     e_eta, e_chi, e_phi = fake_kappa.k_to_e(eta, kappa, phi)
     k_eta, k_kap, k_phi = fake_kappa.e_to_k(e_eta, e_chi, e_phi)
     assert np.isclose(eta, k_eta)
     assert np.isclose(kappa, k_kap)
     assert np.isclose(phi, k_phi)
```

### Comparing `pcdsdevices-7.1.0/pcdsdevices/tests/test_inout.py` & `pcdsdevices-7.4.0/pcdsdevices/tests/test_inout.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.1.0/pcdsdevices/tests/test_interface.py` & `pcdsdevices-7.4.0/pcdsdevices/tests/test_interface.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.1.0/pcdsdevices/tests/test_ipm.py` & `pcdsdevices-7.4.0/pcdsdevices/tests/test_ipm.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,18 +119,18 @@
     status = ipm.target_in(4)
     status.wait(timeout=1)
     assert ipm.target.state.get() == 4
     assert status.done and status.success
     # Target_in with callback
     cb = Mock()
     status = ipm.target_in(3, moved_cb=cb).wait(timeout=1)
-    assert(cb.called)
+    assert cb.called
     # Target_in with wait
     ipm.target_in('TARGET2', wait=True)
-    assert(ipm.target.state.get() == 2)
+    assert ipm.target.state.get() == 2
     # Target_in invalid state
     with pytest.raises(ValueError):
         ipm.target_in('TARGET9')
 
 
 def test_ipm_subscriptions(fake_ipm):
     logger.debug('test_ipm_subscriptions')
```

### Comparing `pcdsdevices-7.1.0/pcdsdevices/tests/test_jet.py` & `pcdsdevices-7.4.0/pcdsdevices/tests/test_jet.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.1.0/pcdsdevices/tests/test_lens.py` & `pcdsdevices-7.4.0/pcdsdevices/tests/test_lens.py`

 * *Files 0% similar despite different names*

```diff
@@ -131,15 +131,15 @@
     lensstack.align(0)
     assert np.isclose(lensstack.beam_size.position, 500e-6, rtol=0.1, atol=0)
 
 
 @pytest.mark.skipif(
     sys.platform == "win32",
     reason="Fails on Windows, presets needed and not supported.",
-    )
+)
 def test_lensstack_align(presets, monkeypatch, fake_lensstack):
     logger.debug('test_lensstack_align')
 
     def mocktweak(self):
         lens.x.move(lens.x.position+1)
         lens.y.move(lens.y.position+1)
     lens = fake_lensstack
```

### Comparing `pcdsdevices-7.1.0/pcdsdevices/tests/test_lodcm.py` & `pcdsdevices-7.4.0/pcdsdevices/tests/test_lodcm.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.1.0/pcdsdevices/tests/test_lxe.py` & `pcdsdevices-7.4.0/pcdsdevices/tests/test_lxe.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.1.0/pcdsdevices/tests/test_mirror.py` & `pcdsdevices-7.4.0/pcdsdevices/tests/test_mirror.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.1.0/pcdsdevices/tests/test_movablestand.py` & `pcdsdevices-7.4.0/pcdsdevices/tests/test_movablestand.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.1.0/pcdsdevices/tests/test_mpod.py` & `pcdsdevices-7.4.0/pcdsdevices/tests/test_mpod.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.1.0/pcdsdevices/tests/test_mpod_apalis.py` & `pcdsdevices-7.4.0/pcdsdevices/tests/test_mpod_apalis.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.1.0/pcdsdevices/tests/test_mps.py` & `pcdsdevices-7.4.0/pcdsdevices/tests/test_mps.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.1.0/pcdsdevices/tests/test_pim.py` & `pcdsdevices-7.4.0/pcdsdevices/tests/test_pim.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import logging
 from unittest.mock import Mock
 
 import pytest
 from ophyd.sim import make_fake_device
 
-from ..pim import PIM, PIMY, PPM, XPIM, PIMWithBoth, PIMWithFocus, PIMWithLED
+from ..pim import PIM, PPM, XPIM, PIMWithBoth, PIMWithFocus, PIMWithLED
 
 logger = logging.getLogger(__name__)
 
 
 @pytest.fixture(scope='function')
 def fake_pim():
     FakePIM = make_fake_device(PIM)
     pim = FakePIM('Test:Yag', name='test')
     pim.state.state.sim_put(0)
-    pim.state.state.sim_set_enum_strs(['Unknown'] + PIMY.states_list)
+    pim.state.state.sim_set_enum_strs(['Unknown', 'DIODE', 'YAG', 'OUT'])
     pim.y.error_severity.sim_put(0)
     pim.y.bit_status.sim_put(0)
     pim.y.motor_spg.sim_put(2)
     return pim
 
 
 @pytest.mark.timeout(5)
```

### Comparing `pcdsdevices-7.1.0/pcdsdevices/tests/test_positioner.py` & `pcdsdevices-7.4.0/pcdsdevices/tests/test_positioner.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 def basic():
     pos = Signal(name='pos')
     return FuncPositioner(
         name='basic',
         move=pos.put,
         get_pos=pos.get,
         update_rate=0.1,
-        )
+    )
 
 
 @pytest.fixture(scope='function')
 def advanced():
     pos = FastMotor()
 
     fpstate = dict(status=None)
@@ -54,15 +54,15 @@
     pos = SlowMotor()
     return FuncPositioner(
         name='slow',
         move=pos.move,
         get_pos=lambda: pos.position,
         update_rate=0.1,
         timeout=0.1,
-        )
+    )
 
 
 def move_and_check(positioner, points):
     for pos in points:
         positioner.move(pos, wait=True)
         assert positioner.position == pos
         assert positioner.notepad_signal.get() == pos
```

### Comparing `pcdsdevices-7.1.0/pcdsdevices/tests/test_pseudopos.py` & `pcdsdevices-7.4.0/pcdsdevices/tests/test_pseudopos.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 import logging
+import time
+from typing import Any
 
 import numpy as np
 import pytest
 from ophyd.device import Component as Cpt
 from ophyd.positioner import SoftPositioner
+from ophyd.sim import make_fake_device
 
 from ..pseudopos import (DelayBase, LookupTablePositioner, OffsetMotorBase,
                          PseudoSingleInterface, SimDelayStage, SyncAxesBase,
                          SyncAxis, SyncAxisOffsetMode)
 from ..sim import FastMotor
 
 logger = logging.getLogger(__name__)
@@ -224,7 +227,99 @@
 
     lut.move(100, wait=True)
     np.testing.assert_allclose(lut.pseudo.position, 100)
     np.testing.assert_allclose(lut.real.position, 6)
 
     assert lut.real.limits == (0, 9)
     assert lut.pseudo.limits == (40, 400)
+
+
+FakeDelayBase = make_fake_device(DelayBase)
+
+
+class FakeDelay(FakeDelayBase):
+    motor = Cpt(FastMotor, egu='mm')
+
+
+def link_two_signals(signal1, signal2):
+    def put_to_1(value, old_value, **kwargs):
+        if value != old_value:
+            signal1.put(value)
+
+    def put_to_2(value, old_value, **kwargs):
+        if value != old_value:
+            signal2.put(value)
+
+    signal1.subscribe(put_to_2)
+    signal2.subscribe(put_to_1)
+
+
+@pytest.fixture(scope='function')
+def linked_delays():
+    delay_one = FakeDelay('SIM', name='delay_one', n_bounces=1)
+    delay_two = FakeDelay('SIM', name='delay_two', n_bounces=2)
+    link_two_signals(
+        delay_one.delay.notepad_readback,
+        delay_two.delay.notepad_readback,
+    )
+    link_two_signals(
+        delay_one.delay.notepad_setpoint,
+        delay_two.delay.notepad_setpoint,
+    )
+    delay_one._my_move_timeout = 0.4
+    delay_two._my_move_timeout = 0.4
+    return delay_one, delay_two
+
+
+def wait_for(
+    obj: Any,
+    attr: str,
+    value: Any,
+    timeout: float = 1,
+    dt: float = 0.1,
+):
+    start_time = time.monotonic()
+    while time.monotonic() - start_time > timeout:
+        if getattr(obj, attr) == value:
+            return
+        time.sleep(dt)
+    assert getattr(obj, attr) == value
+
+
+def test_implicit_mutex(linked_delays: tuple[FakeDelay, FakeDelay]):
+    # Previous bug: two delays could fight over control of ophyd_readback
+    delay_one, delay_two = linked_delays
+
+    def assert_no_updates():
+        value1 = delay_one.delay.notepad_readback.get()
+        value2 = delay_two.delay.notepad_readback.get()
+        if not delay_one._my_move:
+            delay_one._update_position()
+        if not delay_two._my_move:
+            delay_two._update_position()
+        assert delay_one.delay.notepad_readback.get() == value1
+        assert delay_two.delay.notepad_readback.get() == value2
+
+    # Let's do moves and check _my_move attribute
+    assert not delay_one._my_move
+    assert not delay_two._my_move
+    assert_no_updates()
+
+    # First move: delay_one should immediately grab _my_move
+    delay_one.move(1, wait=False)
+    assert delay_one._my_move
+    assert not delay_two._my_move
+    assert_no_updates()
+
+    # Second move: after _my_move_tomeout, delay_one should drop _my_move
+    time.sleep(delay_one._my_move_timeout)
+    delay_two.move(2, wait=False)
+    assert delay_two._my_move
+    wait_for(delay_one, '_my_move', False)
+    assert_no_updates()
+
+    # Do it again but the other way
+    time.sleep(delay_two._my_move_timeout)
+    delay_one.move(3, wait=False)
+    assert delay_one._my_move
+    wait_for(delay_two, '_my_move', False)
+    assert_no_updates()
```

### Comparing `pcdsdevices-7.1.0/pcdsdevices/tests/test_pulsepicker.py` & `pcdsdevices-7.4.0/pcdsdevices/tests/test_pulsepicker.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.1.0/pcdsdevices/tests/test_pump.py` & `pcdsdevices-7.4.0/pcdsdevices/tests/test_pump.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.1.0/pcdsdevices/tests/test_sample_delivery.py` & `pcdsdevices-7.4.0/pcdsdevices/tests/test_sample_delivery.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.1.0/pcdsdevices/tests/test_sequencer.py` & `pcdsdevices-7.4.0/pcdsdevices/tests/test_sequencer.py`

 * *Files 1% similar despite different names*

```diff
@@ -160,18 +160,20 @@
     # Run the plan
     RE(plan())
 
 
 def test_sequence_get_put():
     seq = SimSequencer('ECS:TST:100', name='seq')
 
-    dummy_sequence = [[1,  2,  3,  4],
-                      [5,  6,  7,  8],
-                      [9, 10, 11, 12],
-                      [13, 14, 15, 16]]
+    dummy_sequence = [
+        [1, 2, 3, 4],
+        [5, 6, 7, 8],
+        [9, 10, 11, 12],
+        [13, 14, 15, 16]
+    ]
 
     # Write the dummy sequence
     seq.sequence.put_seq(dummy_sequence)
 
     # Read back the sequence, and compare to dummy sequence
     curr_seq = seq.sequence.get_seq()
```

### Comparing `pcdsdevices-7.1.0/pcdsdevices/tests/test_signal.py` & `pcdsdevices-7.4.0/pcdsdevices/tests/test_signal.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.1.0/pcdsdevices/tests/test_slits.py` & `pcdsdevices-7.4.0/pcdsdevices/tests/test_slits.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.1.0/pcdsdevices/tests/test_spectrometer.py` & `pcdsdevices-7.4.0/pcdsdevices/tests/test_spectrometer.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.1.0/pcdsdevices/tests/test_state.py` & `pcdsdevices-7.4.0/pcdsdevices/tests/test_state.py`

 * *Files 8% similar despite different names*

```diff
@@ -77,26 +77,26 @@
     logger.debug('test_pvstate_positioner')
     lim_obj = LimCls('BASE', name='test')
 
     # Check the state machine
     # Limits are defered
     lim_obj.lowlim.put(1)
     lim_obj.highlim.put(1)
-    assert(lim_obj.position == 'Unknown')
+    assert lim_obj.position == 'Unknown'
     # Limits are out
     lim_obj.highlim.put(0)
-    assert(lim_obj.position == 'OUT')
+    assert lim_obj.position == 'OUT'
     # Limits are in
     lim_obj.lowlim.put(0)
     lim_obj.highlim.put(1)
-    assert(lim_obj.position == 'IN')
+    assert lim_obj.position == 'IN'
     # Limits are in conflicting state
     lim_obj.lowlim.put(0)
     lim_obj.highlim.put(0)
-    assert(lim_obj.position == 'Unknown')
+    assert lim_obj.position == 'Unknown'
 
     with pytest.raises(NotImplementedError):
         lim_obj.move('IN')
 
     lim_obj.states_enum['IN']
     lim_obj.states_enum['OUT']
     lim_obj.states_enum['Unknown']
@@ -169,27 +169,27 @@
     lim_obj2 = LimCls2('BASE', name='test')
     with pytest.raises(ValueError):
         lim_obj2.move('asdfe')
     with pytest.raises(ValueError):
         lim_obj2.move('Unknown')
     cb = Mock()
     lim_obj2.move('OUT', moved_cb=cb).wait(timeout=1)
-    assert(cb.called)
-    assert(lim_obj2.position == 'OUT')
+    assert cb.called
+    assert lim_obj2.position == 'OUT'
     lim_obj2.move('IN', wait=True)
-    assert(lim_obj2.position == 'IN')
+    assert lim_obj2.position == 'IN'
 
     lim_obj2.move(2)
-    assert(lim_obj2.position == 'OUT')
+    assert lim_obj2.position == 'OUT'
 
     with pytest.raises(TypeError):
         lim_obj2.move(123.456)
 
     lim_obj2.state.put('IN')
-    assert(lim_obj2.position == 'IN')
+    assert lim_obj2.position == 'IN'
     lim_obj2.destroy()
 
 
 def test_basic_subscribe():
     logger.debug('test_basic_subscribe')
     lim_obj = LimCls('BASE', name='test')
     cb = Mock()
```

### Comparing `pcdsdevices-7.1.0/pcdsdevices/tests/test_targets.py` & `pcdsdevices-7.4.0/pcdsdevices/tests/test_targets.py`

 * *Files 0% similar despite different names*

```diff
@@ -301,20 +301,20 @@
     with pytest.raises(Exception):
         stage.m_n_points = 23
 
 
 def test_mesh_interpolation():
     a_coeffs, b_coeffs = mesh_interpolation((0, 0), (4, 0), (4, 4),
                                             (0, 4))
-    assert np.isclose(a_coeffs, [0.0, 4.0,  0.0, 0.0]).all()
+    assert np.isclose(a_coeffs, [0.0, 4.0, 0.0, 0.0]).all()
     assert np.isclose(b_coeffs, [0.0, 0.0, 4.0, 0.0]).all()
     # test with slope -0.25
     a_coeffs, b_coeffs = mesh_interpolation((0, 0), (4, -1), (5, 3),
                                             (1, 4))
-    assert np.isclose(a_coeffs, [0.0, 4.0,  1.0, 0.0]).all()
+    assert np.isclose(a_coeffs, [0.0, 4.0, 1.0, 0.0]).all()
     assert np.isclose(b_coeffs, [0.0, -1.0, 4.0, 0.0]).all()
 
 
 def test_get_unit_meshgrid():
     grid = get_unit_meshgrid(m_rows=5, n_columns=5)
     xx_expected = [[0, 0.25, 0.5, 0.75, 1.0],
                    [0, 0.25, 0.5, 0.75, 1.0],
```

### Comparing `pcdsdevices-7.1.0/pcdsdevices/tests/test_timetool.py` & `pcdsdevices-7.4.0/pcdsdevices/tests/test_timetool.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.1.0/pcdsdevices/tests/test_utils.py` & `pcdsdevices-7.4.0/pcdsdevices/tests/test_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 logger = logging.getLogger(__name__)
 pty_missing = "Fails on Windows, pty not supported in Windows Python."
 
 
 @pytest.fixture(scope='function')
 def sim_input(monkeypatch):
     master, slave = pty.openpty()
-    with open(slave, 'r') as fake_stdin:
+    with open(slave) as fake_stdin:
         with open(master, 'w') as sim_input:
             monkeypatch.setattr(sys, 'stdin', fake_stdin)
             yield sim_input
 
 
 def input_later(sim_input, inp, delay=0.1):
     def inner():
@@ -38,58 +38,58 @@
         sim_input.write(inp)
     threading.Thread(target=inner, args=()).start()
 
 
 @pytest.mark.skipif(
     sys.platform == "win32",
     reason=pty_missing,
-    )
+)
 def test_is_input(sim_input):
     logger.debug('test_is_input')
     sim_input.write('a\n')
     assert utils.is_input()
 
 
 @pytest.mark.skipif(
     sys.platform == "win32",
     reason=pty_missing,
-    )
+)
 @pytest.mark.timeout(5)
 def test_get_input_waits(sim_input):
     logger.debug('test_get_input_waits')
     input_later(sim_input, 'a\n', delay=2)
     assert utils.get_input() == 'a'
 
 
 @pytest.mark.skipif(
     sys.platform == "win32",
     reason=pty_missing,
-    )
+)
 @pytest.mark.timeout(0.5)
 def test_get_input_arrow(sim_input):
     logger.debug('test_get_input_arrow')
     input_later(sim_input, utils.arrow_up + '\n')
     assert utils.get_input() == utils.arrow_up
 
 
 @pytest.mark.skipif(
     sys.platform == "win32",
     reason=pty_missing,
-    )
+)
 @pytest.mark.timeout(0.5)
 def test_get_input_shift_arrow(sim_input):
     logger.debug('test_get_input_arrow')
     input_later(sim_input, utils.shift_arrow_up + '\n')
     assert utils.get_input() == utils.shift_arrow_up
 
 
 @pytest.mark.skipif(
     sys.platform == "win32",
     reason=pty_missing,
-    )
+)
 @pytest.mark.timeout(0.5)
 def test_cbreak(sim_input):
     logger.debug('test_cbreak')
     # send the ctrl+c character
     input_later(sim_input, '\x03\n')
     assert utils.get_input() == '\n'
```

### Comparing `pcdsdevices-7.1.0/pcdsdevices/tests/test_valve.py` & `pcdsdevices-7.4.0/pcdsdevices/tests/test_valve.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.1.0/pcdsdevices/tests/test_variety.py` & `pcdsdevices-7.4.0/pcdsdevices/tests/test_variety.py`

 * *Files 4% similar despite different names*

```diff
@@ -318,99 +318,82 @@
         print(tag, tags.explain_tag(tag))
 
     with pytest.raises(KeyError):
         tags.explain_tag('this-is-a-bad-tag')
 
 
 @pytest.mark.parametrize(
-    'value, expected',
-    [pytest.param(
-        {},
-        {}
-     ),
-
-     pytest.param(
-         {'a..': {}},
-         ValueError,
-         id='empty_dot',
-     ),
-
-     pytest.param(
-         {'a': {'b': 3}, 'a.b': {}},
-         ValueError,
-         id='overwrite_dict',
-     ),
-
-     pytest.param(
-         {'a': {'b': {}}, 'a.b.c': 3},
-         {'a': {'b': {'c': 3}}},
-         id='nested_3',
-     ),
-
-     pytest.param(
-         {'a.b': {}},
-         {'a': {'b': {}}},
-         id='nested_ab',
-     ),
-
-     pytest.param(
-         {'a': {}, 'a.b': 4},
-         dict(a=dict(b=4))
-     ),
-
-     pytest.param(
-         {'a.b.c': 1, 'a.b': {'d': 4}},
-         dict(a=dict(b=dict(c=1, d=4)))
-     ),
-
-     pytest.param(
-         {'a.b.c': {}, 'a.b': {'d': 4}},
-         dict(a=dict(b=dict(c={}, d=4)))
-     ),
-
-     pytest.param(
-         {'a': {}, 'a.b': '3', 'a.c': '4'},
-         {'a': {'b': '3', 'c': '4'}},
-     ),
-
-     pytest.param(
-         {'a': {'b': '2'}, 'a.b': '3', 'a.c': '4'},
-         {'a': {'b': '3', 'c': '4'}},
-         id='update_value',
-     ),
-
-     pytest.param(
-        {'variety': 'scalar-tweakable',
-         'delta.value': 0.5,
-         'delta.range': [-1, 1],
-         'range.source': 'custom',
-         'range.value': [-1, 1],
-         },
-        {'variety': 'scalar-tweakable',
-         'delta': {'value': 0.5,
-                   'range': [-1, 1],
-                   },
-         'range': {'source': 'custom',
-                   'value': [-1, 1],
-                   },
-         },
-        id='real_world',
-     ),
-
-     pytest.param(
-        {'variety': 'scalar-tweakable',
-         'delta.value': 0.5,
-         'delta.range': [-1, 1],
-         'range': [-1, 1],  # <-- range specified as a value, not a dict
-         'range.source': 'custom',  # <-- range.source update fails
-         },
-        ValueError,
-        id='real_world_oops',
-     ),
-     ]
+    "value, expected",
+    [
+        pytest.param({}, {}),
+        pytest.param(
+            {"a..": {}},
+            ValueError,
+            id="empty_dot",
+        ),
+        pytest.param(
+            {"a": {"b": 3}, "a.b": {}},
+            ValueError,
+            id="overwrite_dict",
+        ),
+        pytest.param(
+            {"a": {"b": {}}, "a.b.c": 3},
+            {"a": {"b": {"c": 3}}},
+            id="nested_3",
+        ),
+        pytest.param(
+            {"a.b": {}},
+            {"a": {"b": {}}},
+            id="nested_ab",
+        ),
+        pytest.param({"a": {}, "a.b": 4}, dict(a=dict(b=4))),
+        pytest.param({"a.b.c": 1, "a.b": {"d": 4}}, dict(a=dict(b=dict(c=1, d=4)))),
+        pytest.param({"a.b.c": {}, "a.b": {"d": 4}}, dict(a=dict(b=dict(c={}, d=4)))),
+        pytest.param(
+            {"a": {}, "a.b": "3", "a.c": "4"},
+            {"a": {"b": "3", "c": "4"}},
+        ),
+        pytest.param(
+            {"a": {"b": "2"}, "a.b": "3", "a.c": "4"},
+            {"a": {"b": "3", "c": "4"}},
+            id="update_value",
+        ),
+        pytest.param(
+            {
+                "variety": "scalar-tweakable",
+                "delta.value": 0.5,
+                "delta.range": [-1, 1],
+                "range.source": "custom",
+                "range.value": [-1, 1],
+            },
+            {
+                "variety": "scalar-tweakable",
+                "delta": {
+                    "value": 0.5,
+                    "range": [-1, 1],
+                },
+                "range": {
+                    "source": "custom",
+                    "value": [-1, 1],
+                },
+            },
+            id="real_world",
+        ),
+        pytest.param(
+            {
+                "variety": "scalar-tweakable",
+                "delta.value": 0.5,
+                "delta.range": [-1, 1],
+                "range": [-1, 1],  # <-- range specified as a value, not a dict
+                "range.source": "custom",  # <-- range.source update fails
+            },
+            ValueError,
+            id="real_world_oops",
+        ),
+    ],
 )
 def test_dotted_dict(value, expected):
     if isinstance(expected, dict):
         assert expand_dotted_dict(value) == expected
     else:
         with pytest.raises(expected):
             expand_dotted_dict(value)
```

### Comparing `pcdsdevices-7.1.0/pcdsdevices/tests/xcslt8717_wpcalib_opa` & `pcdsdevices-7.4.0/pcdsdevices/tests/xcslt8717_wpcalib_opa`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.1.0/pcdsdevices/timetool.py` & `pcdsdevices-7.4.0/pcdsdevices/timetool.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.1.0/pcdsdevices/ui/AT2L0.detailed.ui` & `pcdsdevices-7.4.0/pcdsdevices/ui/AT1K2.detailed.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.1.0/pcdsdevices/ui/AT2L0.embedded.ui` & `pcdsdevices-7.4.0/pcdsdevices/ui/AT1K2.embedded.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.1.0/pcdsdevices/ui/AttenuatorCalculatorSXR_Blade.embedded.ui` & `pcdsdevices-7.4.0/pcdsdevices/ui/AttenuatorCalculatorSXR_Blade.embedded.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.1.0/pcdsdevices/ui/AttenuatorCalculatorSXR_Blade_config.embedded.ui` & `pcdsdevices-7.4.0/pcdsdevices/ui/AttenuatorCalculatorSXR_Blade_config.embedded.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.1.0/pcdsdevices/ui/AttenuatorCalculatorSXR_FourBlade.detailed.ui` & `pcdsdevices-7.4.0/pcdsdevices/ui/AttenuatorCalculatorSXR_FourBlade.detailed.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.1.0/pcdsdevices/ui/AttenuatorCalculatorSXR_FourBlade.ui` & `pcdsdevices-7.4.0/pcdsdevices/ui/AttenuatorCalculatorSXR_FourBlade.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.1.0/pcdsdevices/ui/AttenuatorCalculatorSXR_FourBlade_all_filters.ui` & `pcdsdevices-7.4.0/pcdsdevices/ui/AttenuatorCalculatorSXR_FourBlade_all_filters.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.1.0/pcdsdevices/ui/AttenuatorCalculatorSXR_FourBlade_blade_all_filters.ui` & `pcdsdevices-7.4.0/pcdsdevices/ui/AttenuatorCalculatorSXR_FourBlade_blade_all_filters.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.1.0/pcdsdevices/ui/AttenuatorCalculatorSXR_FourBlade_calc.ui` & `pcdsdevices-7.4.0/pcdsdevices/ui/AttenuatorCalculatorSXR_FourBlade_calc.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.1.0/pcdsdevices/ui/AttenuatorCalculatorSXR_FourBlade_filters.ui` & `pcdsdevices-7.4.0/pcdsdevices/ui/AttenuatorCalculatorSXR_FourBlade_filters.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.1.0/pcdsdevices/ui/AttenuatorCalculatorSXR_FourBlade_overview.ui` & `pcdsdevices-7.4.0/pcdsdevices/ui/AttenuatorCalculatorSXR_FourBlade_overview.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.1.0/pcdsdevices/ui/AttenuatorCalculator_AT2L0.detailed.ui` & `pcdsdevices-7.4.0/pcdsdevices/ui/AttenuatorCalculator_AT2L0.detailed.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.1.0/pcdsdevices/ui/AttenuatorCalculator_AT2L0.ui` & `pcdsdevices-7.4.0/pcdsdevices/ui/AttenuatorCalculator_AT2L0.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.1.0/pcdsdevices/ui/AttenuatorCalculator_AT2L0_calc.ui` & `pcdsdevices-7.4.0/pcdsdevices/ui/AttenuatorCalculator_AT2L0_calc.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.1.0/pcdsdevices/ui/AttenuatorCalculator_AT2L0_filters.ui` & `pcdsdevices-7.4.0/pcdsdevices/ui/AttenuatorCalculator_AT2L0_filters.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.1.0/pcdsdevices/ui/AttenuatorCalculator_AT2L0_overview.ui` & `pcdsdevices-7.4.0/pcdsdevices/ui/AttenuatorCalculator_AT2L0_overview.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.1.0/pcdsdevices/ui/AttenuatorCalculator_filter.ui` & `pcdsdevices-7.4.0/pcdsdevices/ui/AttenuatorCalculator_filter.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.1.0/pcdsdevices/ui/AttenuatorSXR_Ladder.detailed.ui` & `pcdsdevices-7.4.0/pcdsdevices/ui/AT2L0.detailed.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.1.0/pcdsdevices/ui/AttenuatorSXR_Ladder.embedded.ui` & `pcdsdevices-7.4.0/pcdsdevices/ui/AT2L0.embedded.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.1.0/pcdsdevices/ui/BeckhoffAxis.detailed.ui` & `pcdsdevices-7.4.0/pcdsdevices/ui/BeckhoffAxis.detailed.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.1.0/pcdsdevices/ui/BeckhoffAxis.embedded.ui` & `pcdsdevices-7.4.0/pcdsdevices/ui/BeckhoffAxis.embedded.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.1.0/pcdsdevices/ui/BeckhoffSlits.detailed.ui` & `pcdsdevices-7.4.0/pcdsdevices/ui/BeckhoffSlits.detailed.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.1.0/pcdsdevices/ui/BeckhoffSlits.embedded.ui` & `pcdsdevices-7.4.0/pcdsdevices/ui/BeckhoffSlits.embedded.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.1.0/pcdsdevices/ui/BtpsState.detailed.ui` & `pcdsdevices-7.4.0/pcdsdevices/ui/BtpsState.detailed.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.1.0/pcdsdevices/ui/BtpsState.embedded.ui` & `pcdsdevices-7.4.0/pcdsdevices/ui/BtpsState.embedded.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.1.0/pcdsdevices/ui/JJSlits.detailed.ui` & `pcdsdevices-7.4.0/pcdsdevices/ui/JJSlits.detailed.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.1.0/pcdsdevices/ui/LightControl.ui` & `pcdsdevices-7.4.0/pcdsdevices/ui/LightControl.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.1.0/pcdsdevices/ui/PowerSlits.detailed.ui` & `pcdsdevices-7.4.0/pcdsdevices/ui/PowerSlits.detailed.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.1.0/pcdsdevices/ui/PowerSlits.embedded.ui` & `pcdsdevices-7.4.0/pcdsdevices/ui/PowerSlits.embedded.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.1.0/pcdsdevices/ui/QminiSpectrometer.embedded.ui` & `pcdsdevices-7.4.0/pcdsdevices/ui/QminiSpectrometer.embedded.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.1.0/pcdsdevices/ui/QuadraticBeckhoffMotor.detailed.ui` & `pcdsdevices-7.4.0/pcdsdevices/ui/QuadraticBeckhoffMotor.detailed.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.1.0/pcdsdevices/ui/QuadraticBeckhoffMotor.embedded.ui` & `pcdsdevices-7.4.0/pcdsdevices/ui/QuadraticBeckhoffMotor.embedded.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.1.0/pcdsdevices/ui/StatePositioner.detailed.ui` & `pcdsdevices-7.4.0/pcdsdevices/ui/StatePositioner.detailed.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.1.0/pcdsdevices/ui/StatePositioner.embedded.ui` & `pcdsdevices-7.4.0/pcdsdevices/ui/StatePositioner.embedded.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.1.0/pcdsdevices/ui/TwinCATStatePositioner.detailed.ui` & `pcdsdevices-7.4.0/pcdsdevices/ui/TwinCATStatePositioner.detailed.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.1.0/pcdsdevices/ui/TwinCATStatePositioner.embedded.ui` & `pcdsdevices-7.4.0/pcdsdevices/ui/TwinCATStatePositioner.embedded.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.1.0/pcdsdevices/ui/btps-camera-summary.ui` & `pcdsdevices-7.4.0/pcdsdevices/ui/btps-camera-summary.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.1.0/pcdsdevices/ui/btps-config.ui` & `pcdsdevices-7.4.0/pcdsdevices/ui/btps-config.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.1.0/pcdsdevices/ui/btps-overview.ui` & `pcdsdevices-7.4.0/pcdsdevices/ui/btps-overview.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.1.0/pcdsdevices/ui/btps-range-config.ui` & `pcdsdevices-7.4.0/pcdsdevices/ui/btps-range-config.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.1.0/pcdsdevices/ui/btps-range-summary.ui` & `pcdsdevices-7.4.0/pcdsdevices/ui/btps-range-summary.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.1.0/pcdsdevices/ui/btps-source-dest.ui` & `pcdsdevices-7.4.0/pcdsdevices/ui/btps-source-dest.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.1.0/pcdsdevices/ui/btps-source-tabs-config.ui` & `pcdsdevices-7.4.0/pcdsdevices/ui/btps-source-tabs-config.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.1.0/pcdsdevices/ui/btps-source-tabs.ui` & `pcdsdevices-7.4.0/pcdsdevices/ui/btps-source-tabs.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.1.0/pcdsdevices/ui/btps-source-valves.ui` & `pcdsdevices-7.4.0/pcdsdevices/ui/btps-source-valves.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.1.0/pcdsdevices/ui/btps.ui` & `pcdsdevices-7.4.0/pcdsdevices/ui/btps.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.1.0/pcdsdevices/ui/detailed_tree.ui` & `pcdsdevices-7.4.0/pcdsdevices/ui/AttenuatorSXR_Ladder.detailed.ui`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.1.0/pcdsdevices/usb_encoder.py` & `pcdsdevices-7.4.0/pcdsdevices/usb_encoder.py`

 * *Files identical despite different names*

### Comparing `pcdsdevices-7.1.0/pcdsdevices/utils.py` & `pcdsdevices-7.4.0/pcdsdevices/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import subprocess
 import sys
 import threading
 import time
 from collections.abc import Iterable
 from functools import reduce
 from types import MethodType
-from typing import Callable, Dict, Iterator, List, Optional, Union
+from typing import Callable, Iterator, Union
 
 import ophyd
 import prettytable
 from ophyd.device import Component as Cpt
 from ophyd.device import Device
 from ophyd.ophydobj import Kind
 
@@ -157,16 +157,15 @@
     if (dettype == 'IPIMB'):
         executable = '/reg/g/pcds/controls/pycaqt/ipimb/ipimb'
     elif (dettype == 'Wave8'):
         executable = '/reg/g/pcds/pyps/apps/wave8/latest/wave8'
     else:
         raise ValueError('Unknown detector type')
     if shutil.which(executable) is None:
-        raise EnvironmentError('%s is not on path, we cannot start the screen'
-                               % executable)
+        raise OSError(f"{executable} is not on path, we cannot start the screen")
 
     logger.info(f'Opening {dettype} screen for {prefix}...')
     arglist = [executable, '--base', prefix, '--ioc', prefix_ioc,
                '--evr', prefix+':TRIG']
     _ = subprocess.Popen(arglist)
 
 
@@ -467,19 +466,19 @@
             A set whose elements are the valid enum objects not associated
             with the input identifiers.
         """
         return set(cls.__members__.values()) - cls.include(identifiers)
 
 
 def set_many(
-    to_set: Dict[ophyd.Signal, OphydDataType],
+    to_set: dict[ophyd.Signal, OphydDataType],
     *,
-    owner: Optional[ophyd.ophydobj.OphydObject] = None,
-    timeout: Optional[Number] = None,
-    settle_time: Optional[Number] = None,
+    owner: ophyd.ophydobj.OphydObject | None = None,
+    timeout: Number | None = None,
+    settle_time: Number | None = None,
     raise_on_set_failure: bool = False
 ) -> ophyd.status.StatusBase:
     """
     Call ``set`` on all given signal-to-value pairs with a single Status
     return value.
 
     Parameters
@@ -529,16 +528,16 @@
     status = statuses[0]
     for st in statuses[1:]:
         status = ophyd.status.AndStatus(status, st)
     return status
 
 
 def maybe_make_method(
-    func: Optional[Callable], owner: object
-) -> Optional[Callable]:
+    func: Callable | None, owner: object
+) -> Callable | None:
     """
     Bind ``func`` as a method of ``owner`` if ``self`` is the first parameter.
 
     Additionally, this accepts ``None`` and passes it through.
 
     Parameters
     ----------
@@ -692,18 +691,18 @@
     final_post = collapse_list_head + post + collapse_list_tail
 
     hutch_elog.post(final_post, tags=['ophyd_status'],
                     title='ophyd status report')
 
 
 def reorder_components(
-    cls: Optional[type[Device]] = None,
-    start_with: Optional[List[Union[str, Cpt]]] = None,
-    end_with: Optional[List[Union[str, Cpt]]] = None,
-) -> Union[type[Device], Callable[[type[Device]], type[Device]]]:
+    cls: type[Device] | None = None,
+    start_with: list[str | Cpt] | None = None,
+    end_with: list[str | Cpt] | None = None,
+) -> type[Device] | Callable[[type[Device]], type[Device]]:
     """
     Rearrange the components in cls for typhos displays.
 
     Internally, this works by switching around the keys in the _sig_attrs
     OrderedDict.
 
     Parameters
@@ -738,16 +737,16 @@
         return inner(cls)
     # For decorator with args
     return inner
 
 
 def _normalize_reorder_list(
     cls: type[Device],
-    cpts_or_names: Optional[List[Union[str, Cpt]]],
-) -> List[str]:
+    cpts_or_names: list[str | Cpt] | None,
+) -> list[str]:
     """
     Simplify the user's variable arguments for the component reordering.
     """
     if cpts_or_names is None:
         return []
     reverse_map = {cpt: name for name, cpt in cls._sig_attrs.items()}
     output = []
@@ -767,17 +766,17 @@
             raise TypeError(
                 f'Received object {obj}, which is not a str or Component.'
             )
     return output
 
 
 def move_subdevices_to_start(
-    cls: Optional[type[Device]] = None,
+    cls: type[Device] | None = None,
     subdevice_cls: type[Device] = Device,
-) -> Union[type[Device], Callable[[type[Device]], type[Device]]]:
+) -> type[Device] | Callable[[type[Device]], type[Device]]:
     """
     Arrange the component order of a device class to put subdevices first.
 
     This can be useful to bring e.g. all the motors to the top for the
     typhos screen.
 
     The relative ordering of subdevices is preserved.
@@ -811,17 +810,17 @@
         # For function call or no-args decorator
         return inner(cls)
     # For decorator with args
     return inner
 
 
 def sort_components_by_name(
-    cls: Optional[type[Device]] = None,
+    cls: type[Device] | None = None,
     reverse: bool = False,
-) -> Union[type[Device], Callable[[type[Device]], type[Device]]]:
+) -> type[Device] | Callable[[type[Device]], type[Device]]:
     """
     Arrange the component order of a device class in alphabetical order.
 
     This can be useful as a first step before bringing specific components
     to the top of the queue for the typhos screen.
 
     Parameters
```

### Comparing `pcdsdevices-7.1.0/pcdsdevices/variety.py` & `pcdsdevices-7.4.0/pcdsdevices/variety.py`

 * *Files 1% similar despite different names*

```diff
@@ -200,15 +200,15 @@
                                  f'({part} of {key})')
 
             dct = dct[part]
 
         return dct
 
     def set_values(dct, value):
-        dotted_keys = set(key for key in value if '.' in key)
+        dotted_keys = {key for key in value if '.' in key}
         non_dotted = set(value) - dotted_keys
 
         for key in non_dotted:
             if key in dct:
                 raise KeyError(f'Key specified multiple times: {key}')
             dct[key] = value[key]
```

### Comparing `pcdsdevices-7.1.0/pcdsdevices/wfs.py` & `pcdsdevices-7.4.0/pcdsdevices/wfs.py`

 * *Files identical despite different names*

