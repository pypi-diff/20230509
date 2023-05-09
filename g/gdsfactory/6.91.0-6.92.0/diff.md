# Comparing `tmp/gdsfactory-6.91.0.tar.gz` & `tmp/gdsfactory-6.92.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gdsfactory-6.91.0.tar", last modified: Fri May  5 22:23:31 2023, max compression
+gzip compressed data, was "gdsfactory-6.92.0.tar", last modified: Tue May  9 00:30:39 2023, max compression
```

## Comparing `gdsfactory-6.91.0.tar` & `gdsfactory-6.92.0.tar`

### file list

```diff
@@ -1,667 +1,683 @@
--rw-r--r--   0        0        0     1072 2023-05-05 22:23:15.371309 gdsfactory-6.91.0/LICENSE
--rw-r--r--   0        0        0    14276 2023-05-05 22:23:15.371309 gdsfactory-6.91.0/README.md
--rw-r--r--   0        0        0     3415 2023-05-05 22:23:15.379309 gdsfactory-6.91.0/gdsfactory/__init__.py
--rw-r--r--   0        0        0     2096 2023-05-05 22:23:15.379309 gdsfactory-6.91.0/gdsfactory/add_keepout.py
--rw-r--r--   0        0        0    12629 2023-05-05 22:23:15.379309 gdsfactory-6.91.0/gdsfactory/add_labels.py
--rw-r--r--   0        0        0     3711 2023-05-05 22:23:15.379309 gdsfactory-6.91.0/gdsfactory/add_loopback.py
--rw-r--r--   0        0        0     5054 2023-05-05 22:23:15.379309 gdsfactory-6.91.0/gdsfactory/add_padding.py
--rw-r--r--   0        0        0    15465 2023-05-05 22:23:15.379309 gdsfactory-6.91.0/gdsfactory/add_pins.py
--rw-r--r--   0        0        0    14700 2023-05-05 22:23:15.379309 gdsfactory-6.91.0/gdsfactory/add_ports.py
--rw-r--r--   0        0        0     2884 2023-05-05 22:23:15.379309 gdsfactory-6.91.0/gdsfactory/add_tapers.py
--rw-r--r--   0        0        0     2257 2023-05-05 22:23:15.379309 gdsfactory-6.91.0/gdsfactory/add_tapers_cross_section.py
--rw-r--r--   0        0        0     1831 2023-05-05 22:23:15.379309 gdsfactory-6.91.0/gdsfactory/add_termination.py
--rw-r--r--   0        0        0     1676 2023-05-05 22:23:15.379309 gdsfactory-6.91.0/gdsfactory/asserts.py
--rw-r--r--   0        0        0    11843 2023-05-05 22:23:15.379309 gdsfactory-6.91.0/gdsfactory/cell.py
--rw-r--r--   0        0        0    15946 2023-05-05 22:23:15.379309 gdsfactory-6.91.0/gdsfactory/circuitviz.py
--rw-r--r--   0        0        0     5325 2023-05-05 22:23:15.379309 gdsfactory-6.91.0/gdsfactory/cli.py
--rw-r--r--   0        0        0    99019 2023-05-05 22:23:15.379309 gdsfactory-6.91.0/gdsfactory/component.py
--rw-r--r--   0        0        0    23360 2023-05-05 22:23:15.379309 gdsfactory-6.91.0/gdsfactory/component_layout.py
--rw-r--r--   0        0        0    29699 2023-05-05 22:23:15.379309 gdsfactory-6.91.0/gdsfactory/component_reference.py
--rw-r--r--   0        0        0     1205 2023-05-05 22:23:15.379309 gdsfactory-6.91.0/gdsfactory/components/C.py
--rw-r--r--   0        0        0     1144 2023-05-05 22:23:15.379309 gdsfactory-6.91.0/gdsfactory/components/L.py
--rw-r--r--   0        0        0    20964 2023-05-05 22:23:15.379309 gdsfactory-6.91.0/gdsfactory/components/__init__.py
--rw-r--r--   0        0        0     2621 2023-05-05 22:23:15.379309 gdsfactory-6.91.0/gdsfactory/components/add_fiducials.py
--rw-r--r--   0        0        0    14087 2023-05-05 22:23:15.379309 gdsfactory-6.91.0/gdsfactory/components/add_grating_couplers.py
--rw-r--r--   0        0        0     2014 2023-05-05 22:23:15.379309 gdsfactory-6.91.0/gdsfactory/components/add_trenches.py
--rw-r--r--   0        0        0     3207 2023-05-05 22:23:15.379309 gdsfactory-6.91.0/gdsfactory/components/align.py
--rw-r--r--   0        0        0     2622 2023-05-05 22:23:15.379309 gdsfactory-6.91.0/gdsfactory/components/array_component.py
--rw-r--r--   0        0        0     4705 2023-05-05 22:23:15.379309 gdsfactory-6.91.0/gdsfactory/components/array_with_fanout.py
--rw-r--r--   0        0        0     4322 2023-05-05 22:23:15.379309 gdsfactory-6.91.0/gdsfactory/components/array_with_via.py
--rw-r--r--   0        0        0     4042 2023-05-05 22:23:15.379309 gdsfactory-6.91.0/gdsfactory/components/awg.py
--rw-r--r--   0        0        0     1269 2023-05-05 22:23:15.379309 gdsfactory-6.91.0/gdsfactory/components/bbox.py
--rw-r--r--   0        0        0     2851 2023-05-05 22:23:15.379309 gdsfactory-6.91.0/gdsfactory/components/bend_circular.py
--rw-r--r--   0        0        0     2649 2023-05-05 22:23:15.379309 gdsfactory-6.91.0/gdsfactory/components/bend_circular_heater.py
--rw-r--r--   0        0        0     7882 2023-05-05 22:23:15.379309 gdsfactory-6.91.0/gdsfactory/components/bend_euler.py
--rw-r--r--   0        0        0     2682 2023-05-05 22:23:15.379309 gdsfactory-6.91.0/gdsfactory/components/bend_port.py
--rw-r--r--   0        0        0     3664 2023-05-05 22:23:15.379309 gdsfactory-6.91.0/gdsfactory/components/bend_s.py
--rw-r--r--   0        0        0     5373 2023-05-05 22:23:15.379309 gdsfactory-6.91.0/gdsfactory/components/bezier.py
--rw-r--r--   0        0        0     1605 2023-05-05 22:23:15.379309 gdsfactory-6.91.0/gdsfactory/components/cavity.py
--rw-r--r--   0        0        0     5766 2023-05-05 22:23:15.379309 gdsfactory-6.91.0/gdsfactory/components/cdc.py
--rw-r--r--   0        0        0     2929 2023-05-05 22:23:15.379309 gdsfactory-6.91.0/gdsfactory/components/cdsem_all.py
--rw-r--r--   0        0        0     1788 2023-05-05 22:23:15.379309 gdsfactory-6.91.0/gdsfactory/components/cdsem_bend180.py
--rw-r--r--   0        0        0     1631 2023-05-05 22:23:15.379309 gdsfactory-6.91.0/gdsfactory/components/cdsem_coupler.py
--rw-r--r--   0        0        0     1412 2023-05-05 22:23:15.379309 gdsfactory-6.91.0/gdsfactory/components/cdsem_straight.py
--rw-r--r--   0        0        0     1565 2023-05-05 22:23:15.379309 gdsfactory-6.91.0/gdsfactory/components/cdsem_straight_density.py
--rw-r--r--   0        0        0      793 2023-05-05 22:23:15.379309 gdsfactory-6.91.0/gdsfactory/components/circle.py
--rw-r--r--   0        0        0     5722 2023-05-05 22:23:15.379309 gdsfactory-6.91.0/gdsfactory/components/coh_rx_dual_pol.py
--rw-r--r--   0        0        0     8922 2023-05-05 22:23:15.379309 gdsfactory-6.91.0/gdsfactory/components/coh_rx_single_pol.py
--rw-r--r--   0        0        0     5043 2023-05-05 22:23:15.379309 gdsfactory-6.91.0/gdsfactory/components/coh_tx_dual_pol.py
--rw-r--r--   0        0        0     6118 2023-05-05 22:23:15.379309 gdsfactory-6.91.0/gdsfactory/components/coh_tx_single_pol.py
--rw-r--r--   0        0        0     2548 2023-05-05 22:23:15.379309 gdsfactory-6.91.0/gdsfactory/components/compass.py
--rw-r--r--   0        0        0     9856 2023-05-05 22:23:15.379309 gdsfactory-6.91.0/gdsfactory/components/component_lattice.py
--rw-r--r--   0        0        0     7174 2023-05-05 22:23:15.379309 gdsfactory-6.91.0/gdsfactory/components/component_sequence.py
--rw-r--r--   0        0        0      812 2023-05-05 22:23:15.379309 gdsfactory-6.91.0/gdsfactory/components/copy_layers.py
--rw-r--r--   0        0        0     3460 2023-05-05 22:23:15.379309 gdsfactory-6.91.0/gdsfactory/components/coupler.py
--rw-r--r--   0        0        0     2113 2023-05-05 22:23:15.379309 gdsfactory-6.91.0/gdsfactory/components/coupler90.py
--rw-r--r--   0        0        0     1802 2023-05-05 22:23:15.379309 gdsfactory-6.91.0/gdsfactory/components/coupler90bend.py
--rw-r--r--   0        0        0     4666 2023-05-05 22:23:15.379309 gdsfactory-6.91.0/gdsfactory/components/coupler_adiabatic.py
--rw-r--r--   0        0        0     1909 2023-05-05 22:23:15.379309 gdsfactory-6.91.0/gdsfactory/components/coupler_asymmetric.py
--rw-r--r--   0        0        0     3970 2023-05-05 22:23:15.379309 gdsfactory-6.91.0/gdsfactory/components/coupler_full.py
--rw-r--r--   0        0        0     3414 2023-05-05 22:23:15.379309 gdsfactory-6.91.0/gdsfactory/components/coupler_ring.py
--rw-r--r--   0        0        0     1060 2023-05-05 22:23:15.379309 gdsfactory-6.91.0/gdsfactory/components/coupler_straight.py
--rw-r--r--   0        0        0     1164 2023-05-05 22:23:15.379309 gdsfactory-6.91.0/gdsfactory/components/coupler_straight_asymmetric.py
--rw-r--r--   0        0        0     2192 2023-05-05 22:23:15.379309 gdsfactory-6.91.0/gdsfactory/components/coupler_symmetric.py
--rw-r--r--   0        0        0     1848 2023-05-05 22:23:15.379309 gdsfactory-6.91.0/gdsfactory/components/cross.py
--rw-r--r--   0        0        0    12873 2023-05-05 22:23:15.379309 gdsfactory-6.91.0/gdsfactory/components/crossing_waveguide.py
--rw-r--r--   0        0        0      500 2023-05-05 22:23:15.379309 gdsfactory-6.91.0/gdsfactory/components/csv_data/grating_coupler_1etch_h220_e70.csv
--rw-r--r--   0        0        0     1014 2023-05-05 22:23:15.379309 gdsfactory-6.91.0/gdsfactory/components/csv_data/grating_coupler_2etch_h220_e70_e220.csv
--rw-r--r--   0        0        0    19749 2023-05-05 22:23:15.379309 gdsfactory-6.91.0/gdsfactory/components/csv_data/taper_strip_0p5_10_100.csv
--rw-r--r--   0        0        0    19751 2023-05-05 22:23:15.383309 gdsfactory-6.91.0/gdsfactory/components/csv_data/taper_strip_0p5_10_150.csv
--rw-r--r--   0        0        0    19749 2023-05-05 22:23:15.383309 gdsfactory-6.91.0/gdsfactory/components/csv_data/taper_strip_0p5_10_200.csv
--rw-r--r--   0        0        0    19751 2023-05-05 22:23:15.383309 gdsfactory-6.91.0/gdsfactory/components/csv_data/taper_strip_0p5_11_200.csv
--rw-r--r--   0        0        0    19775 2023-05-05 22:23:15.383309 gdsfactory-6.91.0/gdsfactory/components/csv_data/taper_strip_0p5_12_200.csv
--rw-r--r--   0        0        0     3143 2023-05-05 22:23:15.383309 gdsfactory-6.91.0/gdsfactory/components/csv_data/taper_strip_0p5_3_36.csv
--rw-r--r--   0        0        0     5272 2023-05-05 22:23:15.383309 gdsfactory-6.91.0/gdsfactory/components/cutback_2x2.py
--rw-r--r--   0        0        0     6450 2023-05-05 22:23:15.383309 gdsfactory-6.91.0/gdsfactory/components/cutback_bend.py
--rw-r--r--   0        0        0     3765 2023-05-05 22:23:15.383309 gdsfactory-6.91.0/gdsfactory/components/cutback_component.py
--rw-r--r--   0        0        0     2721 2023-05-05 22:23:15.383309 gdsfactory-6.91.0/gdsfactory/components/cutback_splitter.py
--rw-r--r--   0        0        0     2971 2023-05-05 22:23:15.383309 gdsfactory-6.91.0/gdsfactory/components/dbr.py
--rw-r--r--   0        0        0     4288 2023-05-05 22:23:15.383309 gdsfactory-6.91.0/gdsfactory/components/dbr_tapered.py
--rw-r--r--   0        0        0     2486 2023-05-05 22:23:15.383309 gdsfactory-6.91.0/gdsfactory/components/delay_snake.py
--rw-r--r--   0        0        0     3177 2023-05-05 22:23:15.383309 gdsfactory-6.91.0/gdsfactory/components/delay_snake2.py
--rw-r--r--   0        0        0     3237 2023-05-05 22:23:15.383309 gdsfactory-6.91.0/gdsfactory/components/delay_snake3.py
--rw-r--r--   0        0        0     4319 2023-05-05 22:23:15.383309 gdsfactory-6.91.0/gdsfactory/components/delay_snake_sbend.py
--rw-r--r--   0        0        0     1226 2023-05-05 22:23:15.383309 gdsfactory-6.91.0/gdsfactory/components/dicing_lane.py
--rw-r--r--   0        0        0     3471 2023-05-05 22:23:15.383309 gdsfactory-6.91.0/gdsfactory/components/die.py
--rw-r--r--   0        0        0     2975 2023-05-05 22:23:15.383309 gdsfactory-6.91.0/gdsfactory/components/die_bbox.py
--rw-r--r--   0        0        0     2863 2023-05-05 22:23:15.383309 gdsfactory-6.91.0/gdsfactory/components/die_bbox_frame.py
--rw-r--r--   0        0        0     8015 2023-05-05 22:23:15.383309 gdsfactory-6.91.0/gdsfactory/components/disk.py
--rw-r--r--   0        0        0     4112 2023-05-05 22:23:15.383309 gdsfactory-6.91.0/gdsfactory/components/edge_coupler_array.py
--rw-r--r--   0        0        0     1214 2023-05-05 22:23:15.383309 gdsfactory-6.91.0/gdsfactory/components/ellipse.py
--rw-r--r--   0        0        0     1800 2023-05-05 22:23:15.383309 gdsfactory-6.91.0/gdsfactory/components/extend_ports_list.py
--rw-r--r--   0        0        0     7944 2023-05-05 22:23:15.383309 gdsfactory-6.91.0/gdsfactory/components/extension.py
--rw-r--r--   0        0        0      981 2023-05-05 22:23:15.383309 gdsfactory-6.91.0/gdsfactory/components/fiber.py
--rw-r--r--   0        0        0     1432 2023-05-05 22:23:15.383309 gdsfactory-6.91.0/gdsfactory/components/fiber_array.py
--rw-r--r--   0        0        0      722 2023-05-05 22:23:15.383309 gdsfactory-6.91.0/gdsfactory/components/fiducial_squares.py
--rw-r--r--   0        0        0     3290 2023-05-05 22:23:15.383309 gdsfactory-6.91.0/gdsfactory/components/ge_detector_straight_si_contacts.py
--rw-r--r--   0        0        0     1063 2023-05-05 22:23:15.383309 gdsfactory-6.91.0/gdsfactory/components/grating_coupler_array.py
--rw-r--r--   0        0        0     4682 2023-05-05 22:23:15.383309 gdsfactory-6.91.0/gdsfactory/components/grating_coupler_dual_pol.py
--rw-r--r--   0        0        0     7110 2023-05-05 22:23:15.383309 gdsfactory-6.91.0/gdsfactory/components/grating_coupler_elliptical.py
--rw-r--r--   0        0        0     7221 2023-05-05 22:23:15.383309 gdsfactory-6.91.0/gdsfactory/components/grating_coupler_elliptical_arbitrary.py
--rw-r--r--   0        0        0     4960 2023-05-05 22:23:15.383309 gdsfactory-6.91.0/gdsfactory/components/grating_coupler_elliptical_lumerical.py
--rw-r--r--   0        0        0     4592 2023-05-05 22:23:15.383309 gdsfactory-6.91.0/gdsfactory/components/grating_coupler_elliptical_trenches.py
--rw-r--r--   0        0        0     1773 2023-05-05 22:23:15.383309 gdsfactory-6.91.0/gdsfactory/components/grating_coupler_functions.py
--rw-r--r--   0        0        0     9058 2023-05-05 22:23:15.383309 gdsfactory-6.91.0/gdsfactory/components/grating_coupler_loss.py
--rw-r--r--   0        0        0     1786 2023-05-05 22:23:15.383309 gdsfactory-6.91.0/gdsfactory/components/grating_coupler_loss_fiber_single.py
--rw-r--r--   0        0        0     4142 2023-05-05 22:23:15.383309 gdsfactory-6.91.0/gdsfactory/components/grating_coupler_rectangular.py
--rw-r--r--   0        0        0     4685 2023-05-05 22:23:15.383309 gdsfactory-6.91.0/gdsfactory/components/grating_coupler_rectangular_arbitrary.py
--rw-r--r--   0        0        0     3887 2023-05-05 22:23:15.383309 gdsfactory-6.91.0/gdsfactory/components/grating_coupler_rectangular_arbitrary_slab.py
--rw-r--r--   0        0        0     1578 2023-05-05 22:23:15.383309 gdsfactory-6.91.0/gdsfactory/components/grating_coupler_tree.py
--rw-r--r--   0        0        0     8773 2023-05-05 22:23:15.383309 gdsfactory-6.91.0/gdsfactory/components/greek_cross.py
--rw-r--r--   0        0        0     1019 2023-05-05 22:23:15.383309 gdsfactory-6.91.0/gdsfactory/components/hline.py
--rw-r--r--   0        0        0     3687 2023-05-05 22:23:15.383309 gdsfactory-6.91.0/gdsfactory/components/interdigital_capacitor.py
--rw-r--r--   0        0        0     1825 2023-05-05 22:23:15.383309 gdsfactory-6.91.0/gdsfactory/components/litho_calipers.py
--rw-r--r--   0        0        0     1244 2023-05-05 22:23:15.383309 gdsfactory-6.91.0/gdsfactory/components/litho_ruler.py
--rw-r--r--   0        0        0     1304 2023-05-05 22:23:15.383309 gdsfactory-6.91.0/gdsfactory/components/litho_steps.py
--rw-r--r--   0        0        0      650 2023-05-05 22:23:15.383309 gdsfactory-6.91.0/gdsfactory/components/logo.py
--rw-r--r--   0        0        0     1679 2023-05-05 22:23:15.383309 gdsfactory-6.91.0/gdsfactory/components/loop_mirror.py
--rw-r--r--   0        0        0     3873 2023-05-05 22:23:15.383309 gdsfactory-6.91.0/gdsfactory/components/mmi1x2.py
--rw-r--r--   0        0        0     2814 2023-05-05 22:23:15.383309 gdsfactory-6.91.0/gdsfactory/components/mmi1x2_with_sbend.py
--rw-r--r--   0        0        0     3858 2023-05-05 22:23:15.383309 gdsfactory-6.91.0/gdsfactory/components/mmi2x2.py
--rw-r--r--   0        0        0     3299 2023-05-05 22:23:15.383309 gdsfactory-6.91.0/gdsfactory/components/mmi2x2_with_sbend.py
--rw-r--r--   0        0        0     4947 2023-05-05 22:23:15.383309 gdsfactory-6.91.0/gdsfactory/components/mmi_90degree_hybrid.py
--rw-r--r--   0        0        0     3265 2023-05-05 22:23:15.383309 gdsfactory-6.91.0/gdsfactory/components/mode_converter.py
--rw-r--r--   0        0        0     7414 2023-05-05 22:23:15.383309 gdsfactory-6.91.0/gdsfactory/components/mzi.py
--rw-r--r--   0        0        0     2499 2023-05-05 22:23:15.383309 gdsfactory-6.91.0/gdsfactory/components/mzi_arm.py
--rw-r--r--   0        0        0     5835 2023-05-05 22:23:15.383309 gdsfactory-6.91.0/gdsfactory/components/mzi_arms.py
--rw-r--r--   0        0        0    12214 2023-05-05 22:23:15.383309 gdsfactory-6.91.0/gdsfactory/components/mzi_lattice.py
--rw-r--r--   0        0        0     4025 2023-05-05 22:23:15.383309 gdsfactory-6.91.0/gdsfactory/components/mzi_pads_center.py
--rw-r--r--   0        0        0     1064 2023-05-05 22:23:15.383309 gdsfactory-6.91.0/gdsfactory/components/mzi_phase_shifter.py
--rw-r--r--   0        0        0     6342 2023-05-05 22:23:15.383309 gdsfactory-6.91.0/gdsfactory/components/mzit.py
--rw-r--r--   0        0        0     3502 2023-05-05 22:23:15.383309 gdsfactory-6.91.0/gdsfactory/components/mzit_lattice.py
--rw-r--r--   0        0        0     6047 2023-05-05 22:23:15.383309 gdsfactory-6.91.0/gdsfactory/components/mzm.py
--rw-r--r--   0        0        0     3518 2023-05-05 22:23:15.383309 gdsfactory-6.91.0/gdsfactory/components/nxn.py
--rw-r--r--   0        0        0     1940 2023-05-05 22:23:15.383309 gdsfactory-6.91.0/gdsfactory/components/optimal_90deg.py
--rw-r--r--   0        0        0     3876 2023-05-05 22:23:15.383309 gdsfactory-6.91.0/gdsfactory/components/optimal_hairpin.py
--rw-r--r--   0        0        0     6131 2023-05-05 22:23:15.383309 gdsfactory-6.91.0/gdsfactory/components/optimal_step.py
--rw-r--r--   0        0        0     6327 2023-05-05 22:23:15.383309 gdsfactory-6.91.0/gdsfactory/components/pack_doe.py
--rw-r--r--   0        0        0     3860 2023-05-05 22:23:15.383309 gdsfactory-6.91.0/gdsfactory/components/pad.py
--rw-r--r--   0        0        0     1890 2023-05-05 22:23:15.383309 gdsfactory-6.91.0/gdsfactory/components/pad_gsg.py
--rw-r--r--   0        0        0     1157 2023-05-05 22:23:15.383309 gdsfactory-6.91.0/gdsfactory/components/pads_shorted.py
--rw-r--r--   0        0        0     3833 2023-05-05 22:23:15.383309 gdsfactory-6.91.0/gdsfactory/components/polarization_splitter_rotator.py
--rw-r--r--   0        0        0     1147 2023-05-05 22:23:15.383309 gdsfactory-6.91.0/gdsfactory/components/ramp.py
--rw-r--r--   0        0        0     1508 2023-05-05 22:23:15.383309 gdsfactory-6.91.0/gdsfactory/components/rectangle.py
--rw-r--r--   0        0        0     2972 2023-05-05 22:23:15.383309 gdsfactory-6.91.0/gdsfactory/components/rectangle_with_slits.py
--rw-r--r--   0        0        0     1508 2023-05-05 22:23:15.383309 gdsfactory-6.91.0/gdsfactory/components/regular_polygon.py
--rw-r--r--   0        0        0     3302 2023-05-05 22:23:15.383309 gdsfactory-6.91.0/gdsfactory/components/resistance_meander.py
--rw-r--r--   0        0        0     2642 2023-05-05 22:23:15.383309 gdsfactory-6.91.0/gdsfactory/components/resistance_sheet.py
--rw-r--r--   0        0        0     1273 2023-05-05 22:23:15.383309 gdsfactory-6.91.0/gdsfactory/components/ring.py
--rw-r--r--   0        0        0     4143 2023-05-05 22:23:15.383309 gdsfactory-6.91.0/gdsfactory/components/ring_crow.py
--rw-r--r--   0        0        0     3272 2023-05-05 22:23:15.383309 gdsfactory-6.91.0/gdsfactory/components/ring_crow_couplers.py
--rw-r--r--   0        0        0     2267 2023-05-05 22:23:15.383309 gdsfactory-6.91.0/gdsfactory/components/ring_double.py
--rw-r--r--   0        0        0     3846 2023-05-05 22:23:15.387309 gdsfactory-6.91.0/gdsfactory/components/ring_double_heater.py
--rw-r--r--   0        0        0     7757 2023-05-05 22:23:15.387309 gdsfactory-6.91.0/gdsfactory/components/ring_double_pn.py
--rw-r--r--   0        0        0    12137 2023-05-05 22:23:15.387309 gdsfactory-6.91.0/gdsfactory/components/ring_section_based.py
--rw-r--r--   0        0        0     2719 2023-05-05 22:23:15.387309 gdsfactory-6.91.0/gdsfactory/components/ring_single.py
--rw-r--r--   0        0        0     1968 2023-05-05 22:23:15.387309 gdsfactory-6.91.0/gdsfactory/components/ring_single_array.py
--rw-r--r--   0        0        0     6098 2023-05-05 22:23:15.387309 gdsfactory-6.91.0/gdsfactory/components/ring_single_bend_coupler.py
--rw-r--r--   0        0        0     2714 2023-05-05 22:23:15.387309 gdsfactory-6.91.0/gdsfactory/components/ring_single_dut.py
--rw-r--r--   0        0        0     4018 2023-05-05 22:23:15.387309 gdsfactory-6.91.0/gdsfactory/components/ring_single_heater.py
--rw-r--r--   0        0        0     5267 2023-05-05 22:23:15.387309 gdsfactory-6.91.0/gdsfactory/components/ring_single_pn.py
--rw-r--r--   0        0        0     2282 2023-05-05 22:23:15.387309 gdsfactory-6.91.0/gdsfactory/components/seal_ring.py
--rw-r--r--   0        0        0     3758 2023-05-05 22:23:15.387309 gdsfactory-6.91.0/gdsfactory/components/snspd.py
--rw-r--r--   0        0        0     2059 2023-05-05 22:23:15.387309 gdsfactory-6.91.0/gdsfactory/components/spiral_double.py
--rw-r--r--   0        0        0     5871 2023-05-05 22:23:15.387309 gdsfactory-6.91.0/gdsfactory/components/spiral_external_io.py
--rw-r--r--   0        0        0    16658 2023-05-05 22:23:15.387309 gdsfactory-6.91.0/gdsfactory/components/spiral_heater.py
--rw-r--r--   0        0        0     9181 2023-05-05 22:23:15.387309 gdsfactory-6.91.0/gdsfactory/components/spiral_inner_io.py
--rw-r--r--   0        0        0     1754 2023-05-05 22:23:15.387309 gdsfactory-6.91.0/gdsfactory/components/splitter_chain.py
--rw-r--r--   0        0        0     5327 2023-05-05 22:23:15.387309 gdsfactory-6.91.0/gdsfactory/components/splitter_tree.py
--rw-r--r--   0        0        0     2526 2023-05-05 22:23:15.387309 gdsfactory-6.91.0/gdsfactory/components/straight.py
--rw-r--r--   0        0        0     1033 2023-05-05 22:23:15.387309 gdsfactory-6.91.0/gdsfactory/components/straight_array.py
--rw-r--r--   0        0        0     7914 2023-05-05 22:23:15.387309 gdsfactory-6.91.0/gdsfactory/components/straight_heater_doped_rib.py
--rw-r--r--   0        0        0     1922 2023-05-05 22:23:15.387309 gdsfactory-6.91.0/gdsfactory/components/straight_heater_doped_strip.py
--rw-r--r--   0        0        0     7891 2023-05-05 22:23:15.387309 gdsfactory-6.91.0/gdsfactory/components/straight_heater_meander.py
--rw-r--r--   0        0        0     8090 2023-05-05 22:23:15.387309 gdsfactory-6.91.0/gdsfactory/components/straight_heater_meander_doped.py
--rw-r--r--   0        0        0     5686 2023-05-05 22:23:15.387309 gdsfactory-6.91.0/gdsfactory/components/straight_heater_metal.py
--rw-r--r--   0        0        0     2809 2023-05-05 22:23:15.387309 gdsfactory-6.91.0/gdsfactory/components/straight_pin.py
--rw-r--r--   0        0        0     3974 2023-05-05 22:23:15.387309 gdsfactory-6.91.0/gdsfactory/components/straight_pin_slot.py
--rw-r--r--   0        0        0      655 2023-05-05 22:23:15.387309 gdsfactory-6.91.0/gdsfactory/components/straight_rib.py
--rw-r--r--   0        0        0      820 2023-05-05 22:23:15.387309 gdsfactory-6.91.0/gdsfactory/components/switch_tree.py
--rw-r--r--   0        0        0     7713 2023-05-05 22:23:15.387309 gdsfactory-6.91.0/gdsfactory/components/taper.py
--rw-r--r--   0        0        0     3530 2023-05-05 22:23:15.387309 gdsfactory-6.91.0/gdsfactory/components/taper_adiabatic.py
--rw-r--r--   0        0        0     2457 2023-05-05 22:23:15.387309 gdsfactory-6.91.0/gdsfactory/components/taper_cross_section.py
--rw-r--r--   0        0        0     2363 2023-05-05 22:23:15.387309 gdsfactory-6.91.0/gdsfactory/components/taper_from_csv.py
--rw-r--r--   0        0        0     1215 2023-05-05 22:23:15.387309 gdsfactory-6.91.0/gdsfactory/components/taper_parabolic.py
--rw-r--r--   0        0        0     1635 2023-05-05 22:23:15.387309 gdsfactory-6.91.0/gdsfactory/components/terminator.py
--rw-r--r--   0        0        0     2913 2023-05-05 22:23:15.387309 gdsfactory-6.91.0/gdsfactory/components/text.py
--rw-r--r--   0        0        0     3821 2023-05-05 22:23:15.387309 gdsfactory-6.91.0/gdsfactory/components/text_freetype.py
--rw-r--r--   0        0        0     3156 2023-05-05 22:23:15.387309 gdsfactory-6.91.0/gdsfactory/components/text_rectangular.py
--rw-r--r--   0        0        0     3943 2023-05-05 22:23:15.387309 gdsfactory-6.91.0/gdsfactory/components/text_rectangular_font.py
--rw-r--r--   0        0        0     2536 2023-05-05 22:23:15.387309 gdsfactory-6.91.0/gdsfactory/components/triangles.py
--rw-r--r--   0        0        0      715 2023-05-05 22:23:15.387309 gdsfactory-6.91.0/gdsfactory/components/verniers.py
--rw-r--r--   0        0        0     2468 2023-05-05 22:23:15.387309 gdsfactory-6.91.0/gdsfactory/components/version_stamp.py
--rw-r--r--   0        0        0     2436 2023-05-05 22:23:15.387309 gdsfactory-6.91.0/gdsfactory/components/via.py
--rw-r--r--   0        0        0     3060 2023-05-05 22:23:15.387309 gdsfactory-6.91.0/gdsfactory/components/via_corner.py
--rw-r--r--   0        0        0     5342 2023-05-05 22:23:15.387309 gdsfactory-6.91.0/gdsfactory/components/via_cutback.py
--rw-r--r--   0        0        0    15574 2023-05-05 22:23:15.387309 gdsfactory-6.91.0/gdsfactory/components/via_stack.py
--rw-r--r--   0        0        0     4554 2023-05-05 22:23:15.387309 gdsfactory-6.91.0/gdsfactory/components/via_stack_slot.py
--rw-r--r--   0        0        0     4944 2023-05-05 22:23:15.387309 gdsfactory-6.91.0/gdsfactory/components/via_stack_with_offset.py
--rw-r--r--   0        0        0     1088 2023-05-05 22:23:15.387309 gdsfactory-6.91.0/gdsfactory/components/wafer.py
--rw-r--r--   0        0        0     2542 2023-05-05 22:23:15.387309 gdsfactory-6.91.0/gdsfactory/components/wire.py
--rw-r--r--   0        0        0      978 2023-05-05 22:23:15.387309 gdsfactory-6.91.0/gdsfactory/components/wire_sbend.py
--rw-r--r--   0        0        0     7919 2023-05-05 22:23:15.387309 gdsfactory-6.91.0/gdsfactory/config.py
--rw-r--r--   0        0        0      481 2023-05-05 22:23:15.387309 gdsfactory-6.91.0/gdsfactory/conftest.py
--rw-r--r--   0        0        0    38409 2023-05-05 22:23:15.387309 gdsfactory-6.91.0/gdsfactory/constants.py
--rw-r--r--   0        0        0     1476 2023-05-05 22:23:15.387309 gdsfactory-6.91.0/gdsfactory/containers.py
--rw-r--r--   0        0        0    82607 2023-05-05 22:23:15.387309 gdsfactory-6.91.0/gdsfactory/cross_section.py
--rw-r--r--   0        0        0     2974 2023-05-05 22:23:15.387309 gdsfactory-6.91.0/gdsfactory/decorators.py
--rw-r--r--   0        0        0     6884 2023-05-05 22:23:15.387309 gdsfactory-6.91.0/gdsfactory/difftest.py
--rw-r--r--   0        0        0      988 2023-05-05 22:23:15.387309 gdsfactory-6.91.0/gdsfactory/events.py
--rw-r--r--   0        0        0      204 2023-05-05 22:23:15.387309 gdsfactory-6.91.0/gdsfactory/export/__init__.py
--rw-r--r--   0        0        0     3353 2023-05-05 22:23:15.387309 gdsfactory-6.91.0/gdsfactory/export/to_3d.py
--rw-r--r--   0        0        0     1940 2023-05-05 22:23:15.387309 gdsfactory-6.91.0/gdsfactory/export/to_np.py
--rw-r--r--   0        0        0     3058 2023-05-05 22:23:15.387309 gdsfactory-6.91.0/gdsfactory/export/to_stl.py
--rw-r--r--   0        0        0     7438 2023-05-05 22:23:15.387309 gdsfactory-6.91.0/gdsfactory/export/write_gerbers.py
--rw-r--r--   0        0        0     2968 2023-05-05 22:23:15.387309 gdsfactory-6.91.0/gdsfactory/filestorage.py
--rw-r--r--   0        0        0    11802 2023-05-05 22:23:15.387309 gdsfactory-6.91.0/gdsfactory/fill.py
--rw-r--r--   0        0        0     7799 2023-05-05 22:23:15.387309 gdsfactory-6.91.0/gdsfactory/font.py
--rw-r--r--   0        0        0     8073 2023-05-05 22:23:15.387309 gdsfactory-6.91.0/gdsfactory/functions.py
--rw-r--r--   0        0        0       20 2023-05-05 22:23:15.387309 gdsfactory-6.91.0/gdsfactory/gdsdiff/.gitattributes
--rw-r--r--   0        0        0       83 2023-05-05 22:23:15.387309 gdsfactory-6.91.0/gdsfactory/gdsdiff/.gitconfig
--rw-r--r--   0        0        0       72 2023-05-05 22:23:15.387309 gdsfactory-6.91.0/gdsfactory/gdsdiff/__init__.py
--rw-r--r--   0        0        0     1069 2023-05-05 22:23:15.387309 gdsfactory-6.91.0/gdsfactory/gdsdiff/gds_diff_git.py
--rw-r--r--   0        0        0     2935 2023-05-05 22:23:15.387309 gdsfactory-6.91.0/gdsfactory/gdsdiff/gdsdiff.py
--rw-r--r--   0        0        0      708 2023-05-05 22:23:15.387309 gdsfactory-6.91.0/gdsfactory/gdsdiff/install.py
--rw-r--r--   0        0        0      271 2023-05-05 22:23:15.387309 gdsfactory-6.91.0/gdsfactory/gdsdiff/sample.py
--rw-r--r--   0        0        0     1059 2023-05-05 22:23:15.387309 gdsfactory-6.91.0/gdsfactory/gdsdiff/test_xor.py
--rw-r--r--   0        0        0     1100 2023-05-05 22:23:15.387309 gdsfactory-6.91.0/gdsfactory/generic_tech/README.md
--rw-r--r--   0        0        0     1722 2023-05-05 22:23:15.387309 gdsfactory-6.91.0/gdsfactory/generic_tech/__init__.py
--rw-r--r--   0        0        0      169 2023-05-05 22:23:15.387309 gdsfactory-6.91.0/gdsfactory/generic_tech/generic_tech.sh
--rw-r--r--   0        0        0     8142 2023-05-05 22:23:15.387309 gdsfactory-6.91.0/gdsfactory/generic_tech/get_klayout_pyxs.py
--rw-r--r--   0        0        0       44 2023-05-05 22:23:15.391309 gdsfactory-6.91.0/gdsfactory/generic_tech/klayout/README.md
--rw-r--r--   0        0        0      104 2023-05-05 22:23:15.391309 gdsfactory-6.91.0/gdsfactory/generic_tech/klayout/drc/Makefile
--rw-r--r--   0        0        0        0 2023-05-05 22:23:15.391309 gdsfactory-6.91.0/gdsfactory/generic_tech/klayout/drc/__init__.py
--rw-r--r--   0        0        0     2842 2023-05-05 22:23:15.391309 gdsfactory-6.91.0/gdsfactory/generic_tech/klayout/drc/errors.py
--rw-r--r--   0        0        0      579 2023-05-05 22:23:15.391309 gdsfactory-6.91.0/gdsfactory/generic_tech/klayout/drc/generic.drc
--rw-r--r--   0        0        0     2929 2023-05-05 22:23:15.391309 gdsfactory-6.91.0/gdsfactory/generic_tech/klayout/drc/generic.lydrc
--rw-r--r--   0        0        0     1014 2023-05-05 22:23:15.391309 gdsfactory-6.91.0/gdsfactory/generic_tech/klayout/drc/write_drc.py
--rw-r--r--   0        0        0     6193 2023-05-05 22:23:15.391309 gdsfactory-6.91.0/gdsfactory/generic_tech/klayout/grain.xml
--rw-r--r--   0        0        0    10140 2023-05-05 22:23:15.391309 gdsfactory-6.91.0/gdsfactory/generic_tech/klayout/icon_128x128.png
--rw-r--r--   0        0        0     4248 2023-05-05 22:23:15.391309 gdsfactory-6.91.0/gdsfactory/generic_tech/klayout/icon_64x64.png
--rw-r--r--   0        0        0    10945 2023-05-05 22:23:15.391309 gdsfactory-6.91.0/gdsfactory/generic_tech/klayout/pymacros/import_generic_pcells.lym
--rw-r--r--   0        0        0      710 2023-05-05 22:23:15.391309 gdsfactory-6.91.0/gdsfactory/generic_tech/klayout/pymacros/set_menus.lym
--rw-r--r--   0        0        0      538 2023-05-05 22:23:15.391309 gdsfactory-6.91.0/gdsfactory/generic_tech/klayout/pymacros/set_shortcuts.lym
--rw-r--r--   0        0        0        0 2023-05-05 22:23:15.391309 gdsfactory-6.91.0/gdsfactory/generic_tech/klayout/python/__init__.py
--rw-r--r--   0        0        0      114 2023-05-05 22:23:15.391309 gdsfactory-6.91.0/gdsfactory/generic_tech/klayout/python/kgdsfactory/__init__.py
--rw-r--r--   0        0        0     4303 2023-05-05 22:23:15.391309 gdsfactory-6.91.0/gdsfactory/generic_tech/klayout/python/kgdsfactory/shortcuts.py
--rw-r--r--   0        0        0      269 2023-05-05 22:23:15.391309 gdsfactory-6.91.0/gdsfactory/generic_tech/klayout/tech/Makefile
--rw-r--r--   0        0        0     1519 2023-05-05 22:23:15.391309 gdsfactory-6.91.0/gdsfactory/generic_tech/klayout/tech/generic.layerstack
--rw-r--r--   0        0        0    40153 2023-05-05 22:23:15.391309 gdsfactory-6.91.0/gdsfactory/generic_tech/klayout/tech/generic_tech.lyp
--rw-r--r--   0        0        0     7689 2023-05-05 22:23:15.391309 gdsfactory-6.91.0/gdsfactory/generic_tech/klayout/tech/generic_tech.lyt
--rw-r--r--   0        0        0     4258 2023-05-05 22:23:15.391309 gdsfactory-6.91.0/gdsfactory/generic_tech/klayout/tech/xsection_generic.pyxs
--rw-r--r--   0        0        0     4537 2023-05-05 22:23:15.391309 gdsfactory-6.91.0/gdsfactory/generic_tech/klayout/tech/xsection_generic.xs
--rw-r--r--   0        0        0     4690 2023-05-05 22:23:15.391309 gdsfactory-6.91.0/gdsfactory/generic_tech/klayout/tech/xsection_planarized.pyxs
--rw-r--r--   0        0        0     5508 2023-05-05 22:23:15.391309 gdsfactory-6.91.0/gdsfactory/generic_tech/klayout/tech/xsection_planarized.xs
--rw-r--r--   0        0        0     1855 2023-05-05 22:23:15.391309 gdsfactory-6.91.0/gdsfactory/generic_tech/layer_map.py
--rw-r--r--   0        0        0     6511 2023-05-05 22:23:15.391309 gdsfactory-6.91.0/gdsfactory/generic_tech/layer_stack.py
--rw-r--r--   0        0        0    10547 2023-05-05 22:23:15.391309 gdsfactory-6.91.0/gdsfactory/generic_tech/layer_views.yaml
--rw-r--r--   0        0        0      158 2023-05-05 22:23:15.391309 gdsfactory-6.91.0/gdsfactory/generic_tech/simulation_settings.py
--rw-r--r--   0        0        0     1431 2023-05-05 22:23:15.391309 gdsfactory-6.91.0/gdsfactory/geometry/__init__.py
--rw-r--r--   0        0        0     4917 2023-05-05 22:23:15.391309 gdsfactory-6.91.0/gdsfactory/geometry/boolean.py
--rw-r--r--   0        0        0     3814 2023-05-05 22:23:15.391309 gdsfactory-6.91.0/gdsfactory/geometry/boolean_klayout.py
--rw-r--r--   0        0        0     1904 2023-05-05 22:23:15.391309 gdsfactory-6.91.0/gdsfactory/geometry/boolean_polygons.py
--rw-r--r--   0        0        0      598 2023-05-05 22:23:15.391309 gdsfactory-6.91.0/gdsfactory/geometry/check_duplicated_cells.py
--rw-r--r--   0        0        0     2719 2023-05-05 22:23:15.391309 gdsfactory-6.91.0/gdsfactory/geometry/check_exclusion.py
--rw-r--r--   0        0        0     2829 2023-05-05 22:23:15.391309 gdsfactory-6.91.0/gdsfactory/geometry/check_inclusion.py
--rw-r--r--   0        0        0     3566 2023-05-05 22:23:15.391309 gdsfactory-6.91.0/gdsfactory/geometry/check_space.py
--rw-r--r--   0        0        0     1904 2023-05-05 22:23:15.391309 gdsfactory-6.91.0/gdsfactory/geometry/check_width.py
--rw-r--r--   0        0        0     5005 2023-05-05 22:23:15.391309 gdsfactory-6.91.0/gdsfactory/geometry/fill_klayout.py
--rw-r--r--   0        0        0     7084 2023-05-05 22:23:15.391309 gdsfactory-6.91.0/gdsfactory/geometry/fill_tiled.py
--rw-r--r--   0        0        0     1697 2023-05-05 22:23:15.391309 gdsfactory-6.91.0/gdsfactory/geometry/fillet.py
--rw-r--r--   0        0        0     6664 2023-05-05 22:23:15.391309 gdsfactory-6.91.0/gdsfactory/geometry/functions.py
--rw-r--r--   0        0        0     2167 2023-05-05 22:23:15.391309 gdsfactory-6.91.0/gdsfactory/geometry/invert.py
--rw-r--r--   0        0        0     3685 2023-05-05 22:23:15.391309 gdsfactory-6.91.0/gdsfactory/geometry/layer_priority.py
--rw-r--r--   0        0        0     3046 2023-05-05 22:23:15.391309 gdsfactory-6.91.0/gdsfactory/geometry/manhattanize.py
--rw-r--r--   0        0        0     4192 2023-05-05 22:23:15.391309 gdsfactory-6.91.0/gdsfactory/geometry/maskprep.py
--rw-r--r--   0        0        0     4744 2023-05-05 22:23:15.391309 gdsfactory-6.91.0/gdsfactory/geometry/maskprep_flat.py
--rw-r--r--   0        0        0     3250 2023-05-05 22:23:15.391309 gdsfactory-6.91.0/gdsfactory/geometry/offset.py
--rw-r--r--   0        0        0     3842 2023-05-05 22:23:15.391309 gdsfactory-6.91.0/gdsfactory/geometry/outline.py
--rw-r--r--   0        0        0     2510 2023-05-05 22:23:15.391309 gdsfactory-6.91.0/gdsfactory/geometry/trim.py
--rw-r--r--   0        0        0     2948 2023-05-05 22:23:15.391309 gdsfactory-6.91.0/gdsfactory/geometry/union.py
--rw-r--r--   0        0        0     9629 2023-05-05 22:23:15.391309 gdsfactory-6.91.0/gdsfactory/geometry/write_drc.py
--rw-r--r--   0        0        0     1783 2023-05-05 22:23:15.391309 gdsfactory-6.91.0/gdsfactory/geometry/xor_diff.py
--rw-r--r--   0        0        0     1158 2023-05-05 22:23:15.391309 gdsfactory-6.91.0/gdsfactory/get_factories.py
--rw-r--r--   0        0        0    23562 2023-05-05 22:23:15.391309 gdsfactory-6.91.0/gdsfactory/get_netlist.py
--rw-r--r--   0        0        0    14426 2023-05-05 22:23:15.391309 gdsfactory-6.91.0/gdsfactory/get_netlist_flat.py
--rw-r--r--   0        0        0      682 2023-05-05 22:23:15.391309 gdsfactory-6.91.0/gdsfactory/get_netlist_klayout.py
--rw-r--r--   0        0        0     9455 2023-05-05 22:23:15.391309 gdsfactory-6.91.0/gdsfactory/grid.py
--rw-r--r--   0        0        0     4363 2023-05-05 22:23:15.391309 gdsfactory-6.91.0/gdsfactory/install.py
--rw-r--r--   0        0        0     1340 2023-05-05 22:23:15.391309 gdsfactory-6.91.0/gdsfactory/klive.py
--rw-r--r--   0        0        0      585 2023-05-05 22:23:15.391309 gdsfactory-6.91.0/gdsfactory/labels/__init__.py
--rw-r--r--   0        0        0     3563 2023-05-05 22:23:15.391309 gdsfactory-6.91.0/gdsfactory/labels/add_label_yaml.py
--rw-r--r--   0        0        0     3847 2023-05-05 22:23:15.391309 gdsfactory-6.91.0/gdsfactory/labels/ehva.py
--rw-r--r--   0        0        0     3810 2023-05-05 22:23:15.391309 gdsfactory-6.91.0/gdsfactory/labels/merge_test_metadata.py
--rw-r--r--   0        0        0     4668 2023-05-05 22:23:15.391309 gdsfactory-6.91.0/gdsfactory/labels/siepic.py
--rw-r--r--   0        0        0     4847 2023-05-05 22:23:15.391309 gdsfactory-6.91.0/gdsfactory/labels/write_labels.py
--rw-r--r--   0        0        0     1149 2023-05-05 22:23:15.391309 gdsfactory-6.91.0/gdsfactory/materials.py
--rw-r--r--   0        0        0     5247 2023-05-05 22:23:15.391309 gdsfactory-6.91.0/gdsfactory/name.py
--rw-r--r--   0        0        0    11237 2023-05-05 22:23:15.391309 gdsfactory-6.91.0/gdsfactory/pack.py
--rw-r--r--   0        0        0    50880 2023-05-05 22:23:15.391309 gdsfactory-6.91.0/gdsfactory/path.py
--rw-r--r--   0        0        0    25849 2023-05-05 22:23:15.391309 gdsfactory-6.91.0/gdsfactory/pdk.py
--rw-r--r--   0        0        0     6170 2023-05-05 22:23:15.391309 gdsfactory-6.91.0/gdsfactory/picmodel.py
--rw-r--r--   0        0        0     5068 2023-05-05 22:23:15.391309 gdsfactory-6.91.0/gdsfactory/pixelate.py
--rw-r--r--   0        0        0        0 2023-05-05 22:23:15.391309 gdsfactory-6.91.0/gdsfactory/plugins/dagster/__init__.py
--rw-r--r--   0        0        0      976 2023-05-05 22:23:15.391309 gdsfactory-6.91.0/gdsfactory/plugins/dagster/workflow.py
--rw-r--r--   0        0        0      566 2023-05-05 22:23:15.391309 gdsfactory-6.91.0/gdsfactory/plugins/database/README.md
--rw-r--r--   0        0        0     1592 2023-05-05 22:23:15.391309 gdsfactory-6.91.0/gdsfactory/plugins/database/__init__.py
--rw-r--r--   0        0        0     6216 2023-05-05 22:23:15.391309 gdsfactory-6.91.0/gdsfactory/plugins/database/db_upload.py
--rw-r--r--   0        0        0    16143 2023-05-05 22:23:15.395309 gdsfactory-6.91.0/gdsfactory/plugins/database/models.py
--rw-r--r--   0        0        0    32084 2023-05-05 22:23:15.395309 gdsfactory-6.91.0/gdsfactory/port.py
--rw-r--r--   0        0        0    37609 2023-05-05 22:23:15.395309 gdsfactory-6.91.0/gdsfactory/quickplotter.py
--rw-r--r--   0        0        0      696 2023-05-05 22:23:15.395309 gdsfactory-6.91.0/gdsfactory/read/__init__.py
--rw-r--r--   0        0        0     1639 2023-05-05 22:23:15.395309 gdsfactory-6.91.0/gdsfactory/read/from_dphox.py
--rw-r--r--   0        0        0     1285 2023-05-05 22:23:15.395309 gdsfactory-6.91.0/gdsfactory/read/from_gdspaths.py
--rw-r--r--   0        0        0     1953 2023-05-05 22:23:15.395309 gdsfactory-6.91.0/gdsfactory/read/from_np.py
--rw-r--r--   0        0        0     2813 2023-05-05 22:23:15.395309 gdsfactory-6.91.0/gdsfactory/read/from_phidl.py
--rw-r--r--   0        0        0    38082 2023-05-05 22:23:15.395309 gdsfactory-6.91.0/gdsfactory/read/from_yaml.py
--rw-r--r--   0        0        0     5897 2023-05-05 22:23:15.395309 gdsfactory-6.91.0/gdsfactory/read/from_yaml_template.py
--rw-r--r--   0        0        0     5688 2023-05-05 22:23:15.395309 gdsfactory-6.91.0/gdsfactory/read/import_gds.py
--rw-r--r--   0        0        0     3407 2023-05-05 22:23:15.395309 gdsfactory-6.91.0/gdsfactory/read/labels.py
--rw-r--r--   0        0        0     3769 2023-05-05 22:23:15.395309 gdsfactory-6.91.0/gdsfactory/routing/__init__.py
--rw-r--r--   0        0        0     2920 2023-05-05 22:23:15.395309 gdsfactory-6.91.0/gdsfactory/routing/add_electrical_pads_shortest.py
--rw-r--r--   0        0        0     3015 2023-05-05 22:23:15.395309 gdsfactory-6.91.0/gdsfactory/routing/add_electrical_pads_top.py
--rw-r--r--   0        0        0     3035 2023-05-05 22:23:15.395309 gdsfactory-6.91.0/gdsfactory/routing/add_electrical_pads_top_dc.py
--rw-r--r--   0        0        0     8715 2023-05-05 22:23:15.395309 gdsfactory-6.91.0/gdsfactory/routing/add_fiber_array.py
--rw-r--r--   0        0        0    10624 2023-05-05 22:23:15.395309 gdsfactory-6.91.0/gdsfactory/routing/add_fiber_single.py
--rw-r--r--   0        0        0     8967 2023-05-05 22:23:15.395309 gdsfactory-6.91.0/gdsfactory/routing/add_pads.py
--rw-r--r--   0        0        0    38940 2023-05-05 22:23:15.395309 gdsfactory-6.91.0/gdsfactory/routing/all_angle.py
--rw-r--r--   0        0        0     3916 2023-05-05 22:23:15.395309 gdsfactory-6.91.0/gdsfactory/routing/auto_taper.py
--rw-r--r--   0        0        0      982 2023-05-05 22:23:15.395309 gdsfactory-6.91.0/gdsfactory/routing/factories.py
--rw-r--r--   0        0        0     4415 2023-05-05 22:23:15.395309 gdsfactory-6.91.0/gdsfactory/routing/fanout.py
--rw-r--r--   0        0        0     2800 2023-05-05 22:23:15.395309 gdsfactory-6.91.0/gdsfactory/routing/fanout2x2.py
--rw-r--r--   0        0        0    24342 2023-05-05 22:23:15.395309 gdsfactory-6.91.0/gdsfactory/routing/get_bundle.py
--rw-r--r--   0        0        0     8632 2023-05-05 22:23:15.395309 gdsfactory-6.91.0/gdsfactory/routing/get_bundle_corner.py
--rw-r--r--   0        0        0     6900 2023-05-05 22:23:15.395309 gdsfactory-6.91.0/gdsfactory/routing/get_bundle_from_steps.py
--rw-r--r--   0        0        0    12949 2023-05-05 22:23:15.395309 gdsfactory-6.91.0/gdsfactory/routing/get_bundle_from_waypoints.py
--rw-r--r--   0        0        0     5284 2023-05-05 22:23:15.395309 gdsfactory-6.91.0/gdsfactory/routing/get_bundle_path_length_match.py
--rw-r--r--   0        0        0     1937 2023-05-05 22:23:15.395309 gdsfactory-6.91.0/gdsfactory/routing/get_bundle_sbend.py
--rw-r--r--   0        0        0    17064 2023-05-05 22:23:15.395309 gdsfactory-6.91.0/gdsfactory/routing/get_bundle_u.py
--rw-r--r--   0        0        0     1510 2023-05-05 22:23:15.395309 gdsfactory-6.91.0/gdsfactory/routing/get_input_labels.py
--rw-r--r--   0        0        0     9233 2023-05-05 22:23:15.395309 gdsfactory-6.91.0/gdsfactory/routing/get_route.py
--rw-r--r--   0        0        0    10824 2023-05-05 22:23:15.395309 gdsfactory-6.91.0/gdsfactory/routing/get_route_astar.py
--rw-r--r--   0        0        0     6119 2023-05-05 22:23:15.395309 gdsfactory-6.91.0/gdsfactory/routing/get_route_from_steps.py
--rw-r--r--   0        0        0     2766 2023-05-05 22:23:15.395309 gdsfactory-6.91.0/gdsfactory/routing/get_route_sbend.py
--rw-r--r--   0        0        0     3311 2023-05-05 22:23:15.395309 gdsfactory-6.91.0/gdsfactory/routing/get_routes_bend180.py
--rw-r--r--   0        0        0     1854 2023-05-05 22:23:15.395309 gdsfactory-6.91.0/gdsfactory/routing/get_routes_straight.py
--rw-r--r--   0        0        0    34394 2023-05-05 22:23:15.395309 gdsfactory-6.91.0/gdsfactory/routing/manhattan.py
--rw-r--r--   0        0        0    10081 2023-05-05 22:23:15.395309 gdsfactory-6.91.0/gdsfactory/routing/path_length_matching.py
--rw-r--r--   0        0        0    22568 2023-05-05 22:23:15.395309 gdsfactory-6.91.0/gdsfactory/routing/route_fiber_array.py
--rw-r--r--   0        0        0     8679 2023-05-05 22:23:15.395309 gdsfactory-6.91.0/gdsfactory/routing/route_fiber_single.py
--rw-r--r--   0        0        0    18132 2023-05-05 22:23:15.395309 gdsfactory-6.91.0/gdsfactory/routing/route_ports_to_side.py
--rw-r--r--   0        0        0     4361 2023-05-05 22:23:15.395309 gdsfactory-6.91.0/gdsfactory/routing/route_quad.py
--rw-r--r--   0        0        0    14370 2023-05-05 22:23:15.395309 gdsfactory-6.91.0/gdsfactory/routing/route_sharp.py
--rw-r--r--   0        0        0    10167 2023-05-05 22:23:15.395309 gdsfactory-6.91.0/gdsfactory/routing/route_south.py
--rw-r--r--   0        0        0     5072 2023-05-05 22:23:15.395309 gdsfactory-6.91.0/gdsfactory/routing/sort_ports.py
--rw-r--r--   0        0        0     2477 2023-05-05 22:23:15.395309 gdsfactory-6.91.0/gdsfactory/routing/utils.py
--rw-r--r--   0        0        0     2889 2023-05-05 22:23:15.395309 gdsfactory-6.91.0/gdsfactory/samples/01_component_pcell.py
--rw-r--r--   0        0        0      646 2023-05-05 22:23:15.395309 gdsfactory-6.91.0/gdsfactory/samples/01_component_pcell/test_straight_wide.yml
--rw-r--r--   0        0        0     1101 2023-05-05 22:23:15.395309 gdsfactory-6.91.0/gdsfactory/samples/01_component_pcell_with_pins.py
--rw-r--r--   0        0        0      664 2023-05-05 22:23:15.395309 gdsfactory-6.91.0/gdsfactory/samples/01_component_pcell_with_pins/test_straight_narrow.yml
--rw-r--r--   0        0        0      347 2023-05-05 22:23:15.395309 gdsfactory-6.91.0/gdsfactory/samples/02_component_autoname.py
--rw-r--r--   0        0        0      887 2023-05-05 22:23:15.395309 gdsfactory-6.91.0/gdsfactory/samples/03_move.py
--rw-r--r--   0        0        0      881 2023-05-05 22:23:15.395309 gdsfactory-6.91.0/gdsfactory/samples/04_connect.py
--rw-r--r--   0        0        0      710 2023-05-05 22:23:15.395309 gdsfactory-6.91.0/gdsfactory/samples/05_remove_layers.py
--rw-r--r--   0        0        0      931 2023-05-05 22:23:15.395309 gdsfactory-6.91.0/gdsfactory/samples/06_remapping_layers.py
--rw-r--r--   0        0        0     1082 2023-05-05 22:23:15.395309 gdsfactory-6.91.0/gdsfactory/samples/07_flattening_device.py
--rw-r--r--   0        0        0      475 2023-05-05 22:23:15.395309 gdsfactory-6.91.0/gdsfactory/samples/08_group.py
--rw-r--r--   0        0        0     1631 2023-05-05 22:23:15.395309 gdsfactory-6.91.0/gdsfactory/samples/11_component_layout.py
--rw-r--r--   0        0        0     2245 2023-05-05 22:23:15.395309 gdsfactory-6.91.0/gdsfactory/samples/12_component_refs.py
--rw-r--r--   0        0        0      955 2023-05-05 22:23:15.395309 gdsfactory-6.91.0/gdsfactory/samples/13_component_netlist.py
--rw-r--r--   0        0        0     2592 2023-05-05 22:23:15.395309 gdsfactory-6.91.0/gdsfactory/samples/14_component_connectivity.py
--rw-r--r--   0        0        0     1636 2023-05-05 22:23:15.395309 gdsfactory-6.91.0/gdsfactory/samples/15_component_sequence1.py
--rw-r--r--   0        0        0     1680 2023-05-05 22:23:15.395309 gdsfactory-6.91.0/gdsfactory/samples/16_component_sequence2.py
--rw-r--r--   0        0        0      965 2023-05-05 22:23:15.395309 gdsfactory-6.91.0/gdsfactory/samples/17_ports.py
--rw-r--r--   0        0        0      489 2023-05-05 22:23:15.399309 gdsfactory-6.91.0/gdsfactory/samples/18_port_markers.py
--rw-r--r--   0        0        0      361 2023-05-05 22:23:15.399309 gdsfactory-6.91.0/gdsfactory/samples/19_references.py
--rw-r--r--   0        0        0      533 2023-05-05 22:23:15.399309 gdsfactory-6.91.0/gdsfactory/samples/20_components.py
--rw-r--r--   0        0        0      507 2023-05-05 22:23:15.399309 gdsfactory-6.91.0/gdsfactory/samples/21_add_fiber_array.py
--rw-r--r--   0        0        0      493 2023-05-05 22:23:15.399309 gdsfactory-6.91.0/gdsfactory/samples/22_add_fiber_single.py
--rw-r--r--   0        0        0      569 2023-05-05 22:23:15.399309 gdsfactory-6.91.0/gdsfactory/samples/22_add_pads.py
--rw-r--r--   0        0        0      848 2023-05-05 22:23:15.399309 gdsfactory-6.91.0/gdsfactory/samples/23_reticle.py
--rw-r--r--   0        0        0     1588 2023-05-05 22:23:15.399309 gdsfactory-6.91.0/gdsfactory/samples/23_reticle_passives.py
--rw-r--r--   0        0        0      457 2023-05-05 22:23:15.399309 gdsfactory-6.91.0/gdsfactory/samples/24_doe.py
--rw-r--r--   0        0        0      687 2023-05-05 22:23:15.399309 gdsfactory-6.91.0/gdsfactory/samples/24_doe_2.py
--rw-r--r--   0        0        0      692 2023-05-05 22:23:15.399309 gdsfactory-6.91.0/gdsfactory/samples/24_doe_3.py
--rw-r--r--   0        0        0      306 2023-05-05 22:23:15.399309 gdsfactory-6.91.0/gdsfactory/samples/25_slot_cross_section.py
--rw-r--r--   0        0        0     1363 2023-05-05 22:23:15.399309 gdsfactory-6.91.0/gdsfactory/samples/30_lidar.py
--rw-r--r--   0        0        0     1412 2023-05-05 22:23:15.399309 gdsfactory-6.91.0/gdsfactory/samples/30_lidar_pcell.py
--rw-r--r--   0        0        0     1943 2023-05-05 22:23:15.399309 gdsfactory-6.91.0/gdsfactory/samples/30_lidar_with_pads.py
--rw-r--r--   0        0        0        0 2023-05-05 22:23:15.399309 gdsfactory-6.91.0/gdsfactory/samples/__init__.py
--rw-r--r--   0        0        0     1307 2023-05-05 22:23:15.399309 gdsfactory-6.91.0/gdsfactory/samples/all_angle_routing.py
--rw-r--r--   0        0        0      558 2023-05-05 22:23:15.399309 gdsfactory-6.91.0/gdsfactory/samples/all_angle_routing/aar_basic_01.pic.yml
--rw-r--r--   0        0        0     6062 2023-05-05 22:23:15.399309 gdsfactory-6.91.0/gdsfactory/samples/all_angle_routing/aar_bundles.pic.yml
--rw-r--r--   0        0        0      444 2023-05-05 22:23:15.399309 gdsfactory-6.91.0/gdsfactory/samples/all_angle_routing/aar_error_intermediate_180.pic.yml
--rw-r--r--   0        0        0      463 2023-05-05 22:23:15.399309 gdsfactory-6.91.0/gdsfactory/samples/all_angle_routing/aar_error_overconstrained.pic.yml
--rw-r--r--   0        0        0     1552 2023-05-05 22:23:15.399309 gdsfactory-6.91.0/gdsfactory/samples/all_angle_routing/aar_gone_wrong.pic.yml
--rw-r--r--   0        0        0     1315 2023-05-05 22:23:15.399309 gdsfactory-6.91.0/gdsfactory/samples/all_angle_routing/aar_implicit_final_angle.pic.yml
--rw-r--r--   0        0        0      602 2023-05-05 22:23:15.399309 gdsfactory-6.91.0/gdsfactory/samples/all_angle_routing/aar_slalom.pic.yml
--rw-r--r--   0        0        0     3317 2023-05-05 22:23:15.399309 gdsfactory-6.91.0/gdsfactory/samples/all_angle_routing/aar_start_end_customizations.pic.yml
--rw-r--r--   0        0        0     1484 2023-05-05 22:23:15.399309 gdsfactory-6.91.0/gdsfactory/samples/all_angle_routing/aar_step_definitions.pic.yml
--rw-r--r--   0        0        0     3045 2023-05-05 22:23:15.399309 gdsfactory-6.91.0/gdsfactory/samples/all_angle_routing/aar_tricky_connections.pic.yml
--rw-r--r--   0        0        0     3782 2023-05-05 22:23:15.399309 gdsfactory-6.91.0/gdsfactory/samples/all_angle_routing/all_angle_routes.pic.yml
--rw-r--r--   0        0        0     1988 2023-05-05 22:23:15.399309 gdsfactory-6.91.0/gdsfactory/samples/big_device.py
--rw-r--r--   0        0        0       19 2023-05-05 22:23:15.399309 gdsfactory-6.91.0/gdsfactory/samples/demo/Makefile
--rw-r--r--   0        0        0        0 2023-05-05 22:23:15.399309 gdsfactory-6.91.0/gdsfactory/samples/demo/__init__.py
--rw-r--r--   0        0        0     1129 2023-05-05 22:23:15.399309 gdsfactory-6.91.0/gdsfactory/samples/demo/benchmark/fill_demo.py
--rw-r--r--   0        0        0      343 2023-05-05 22:23:15.399309 gdsfactory-6.91.0/gdsfactory/samples/demo/benchmark/snap_demo_phidl.py
--rw-r--r--   0        0        0      637 2023-05-05 22:23:15.399309 gdsfactory-6.91.0/gdsfactory/samples/demo/circuits/mask.pic.yml
--rw-r--r--   0        0        0      622 2023-05-05 22:23:15.399309 gdsfactory-6.91.0/gdsfactory/samples/demo/circuits/mzi_lattice_filter.pic.yml
--rw-r--r--   0        0        0      569 2023-05-05 22:23:15.399309 gdsfactory-6.91.0/gdsfactory/samples/demo/circuits/mzi_ubcpdk.pic.yml
--rw-r--r--   0        0        0      453 2023-05-05 22:23:15.399309 gdsfactory-6.91.0/gdsfactory/samples/demo/circuits/pads.pic.yml
--rw-r--r--   0        0        0      287 2023-05-05 22:23:15.399309 gdsfactory-6.91.0/gdsfactory/samples/demo/circuits/rectangles.pic.yml
--rw-r--r--   0        0        0     2260 2023-05-05 22:23:15.399309 gdsfactory-6.91.0/gdsfactory/samples/demo/drc_errors.py
--rw-r--r--   0        0        0     1014 2023-05-05 22:23:15.399309 gdsfactory-6.91.0/gdsfactory/samples/demo/drc_write.py
--rw-r--r--   0        0        0     4530 2023-05-05 22:23:15.399309 gdsfactory-6.91.0/gdsfactory/samples/demo/layers.py
--rw-r--r--   0        0        0      158 2023-05-05 22:23:15.399309 gdsfactory-6.91.0/gdsfactory/samples/demo/layers_sky130.py
--rw-r--r--   0        0        0      364 2023-05-05 22:23:15.399309 gdsfactory-6.91.0/gdsfactory/samples/demo/layers_xsection.py
--rw-r--r--   0        0        0      708 2023-05-05 22:23:15.399309 gdsfactory-6.91.0/gdsfactory/samples/demo/lvs.py
--rw-r--r--   0        0        0      574 2023-05-05 22:23:15.399309 gdsfactory-6.91.0/gdsfactory/samples/demo/pcell.py
--rw-r--r--   0        0        0     4174 2023-05-05 22:23:15.399309 gdsfactory-6.91.0/gdsfactory/samples/netlists/mzi.yml
--rw-r--r--   0        0        0     5840 2023-05-05 22:23:15.399309 gdsfactory-6.91.0/gdsfactory/samples/netlists/mzi_full.yml
--rw-r--r--   0        0        0        0 2023-05-05 22:23:15.399309 gdsfactory-6.91.0/gdsfactory/samples/pdk/__init__.py
--rw-r--r--   0        0        0     4235 2023-05-05 22:23:15.399309 gdsfactory-6.91.0/gdsfactory/samples/pdk/fab_c.py
--rw-r--r--   0        0        0      475 2023-05-05 22:23:15.399309 gdsfactory-6.91.0/gdsfactory/samples/pdk/fab_d/__init__.py
--rw-r--r--   0        0        0     1880 2023-05-05 22:23:15.399309 gdsfactory-6.91.0/gdsfactory/samples/pdk/fab_d/phase_shifters.py
--rw-r--r--   0        0        0     1715 2023-05-05 22:23:15.399309 gdsfactory-6.91.0/gdsfactory/samples/pdk/test_fab_c.py
--rw-r--r--   0        0        0       50 2023-05-05 22:23:15.399309 gdsfactory-6.91.0/gdsfactory/samples/pdk/test_fab_c/test_ports_bend_euler_c_.csv
--rw-r--r--   0        0        0       93 2023-05-05 22:23:15.399309 gdsfactory-6.91.0/gdsfactory/samples/pdk/test_fab_c/test_ports_gc_nitride_c_.csv
--rw-r--r--   0        0        0       85 2023-05-05 22:23:15.399309 gdsfactory-6.91.0/gdsfactory/samples/pdk/test_fab_c/test_ports_mmi1x2_nitride_c_.csv
--rw-r--r--   0        0        0      139 2023-05-05 22:23:15.399309 gdsfactory-6.91.0/gdsfactory/samples/pdk/test_fab_c/test_ports_mmi1x2_nitride_o_.csv
--rw-r--r--   0        0        0       90 2023-05-05 22:23:15.399309 gdsfactory-6.91.0/gdsfactory/samples/pdk/test_fab_c/test_ports_mzi_nitride_c_.csv
--rw-r--r--   0        0        0      126 2023-05-05 22:23:15.399309 gdsfactory-6.91.0/gdsfactory/samples/pdk/test_fab_c/test_ports_mzi_nitride_o_.csv
--rw-r--r--   0        0        0       48 2023-05-05 22:23:15.399309 gdsfactory-6.91.0/gdsfactory/samples/pdk/test_fab_c/test_ports_straight_c_.csv
--rw-r--r--   0        0        0     1023 2023-05-05 22:23:15.399309 gdsfactory-6.91.0/gdsfactory/samples/pdk/test_fab_c/test_settings_bend_euler_c_.yml
--rw-r--r--   0        0        0     2100 2023-05-05 22:23:15.399309 gdsfactory-6.91.0/gdsfactory/samples/pdk/test_fab_c/test_settings_bend_euler_nc_.yml
--rw-r--r--   0        0        0     1839 2023-05-05 22:23:15.399309 gdsfactory-6.91.0/gdsfactory/samples/pdk/test_fab_c/test_settings_gc_nc_.yml
--rw-r--r--   0        0        0     1267 2023-05-05 22:23:15.399309 gdsfactory-6.91.0/gdsfactory/samples/pdk/test_fab_c/test_settings_gc_nitride_c_.yml
--rw-r--r--   0        0        0     1592 2023-05-05 22:23:15.399309 gdsfactory-6.91.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mmi1x2_nc_.yml
--rw-r--r--   0        0        0     1061 2023-05-05 22:23:15.399309 gdsfactory-6.91.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mmi1x2_nitride_c_.yml
--rw-r--r--   0        0        0     1054 2023-05-05 22:23:15.399309 gdsfactory-6.91.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mmi1x2_nitride_o_.yml
--rw-r--r--   0        0        0     1577 2023-05-05 22:23:15.399309 gdsfactory-6.91.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mmi1x2_no_.yml
--rw-r--r--   0        0        0     4313 2023-05-05 22:23:15.399309 gdsfactory-6.91.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mzi_nc_.yml
--rw-r--r--   0        0        0     3625 2023-05-05 22:23:15.399309 gdsfactory-6.91.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mzi_nitride_c_.yml
--rw-r--r--   0        0        0     3603 2023-05-05 22:23:15.399309 gdsfactory-6.91.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mzi_nitride_o_.yml
--rw-r--r--   0        0        0     4271 2023-05-05 22:23:15.399309 gdsfactory-6.91.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mzi_no_.yml
--rw-r--r--   0        0        0      840 2023-05-05 22:23:15.399309 gdsfactory-6.91.0/gdsfactory/samples/pdk/test_fab_c/test_settings_straight_c_.yml
--rw-r--r--   0        0        0     2171 2023-05-05 22:23:15.399309 gdsfactory-6.91.0/gdsfactory/samples/pdk/test_fab_c/test_settings_straight_nc_.yml
--rw-r--r--   0        0        0      316 2023-05-05 22:23:15.399309 gdsfactory-6.91.0/gdsfactory/schematic.py
--rw-r--r--   0        0        0    17692 2023-05-05 22:23:15.399309 gdsfactory-6.91.0/gdsfactory/schematic_editor.py
--rw-r--r--   0        0        0     4194 2023-05-05 22:23:15.399309 gdsfactory-6.91.0/gdsfactory/serialization.py
--rw-r--r--   0        0        0     1612 2023-05-05 22:23:15.399309 gdsfactory-6.91.0/gdsfactory/show.py
--rw-r--r--   0        0        0      724 2023-05-05 22:23:15.399309 gdsfactory-6.91.0/gdsfactory/simulation/__init__.py
--rw-r--r--   0        0        0     4369 2023-05-05 22:23:15.399309 gdsfactory-6.91.0/gdsfactory/simulation/add_simulation_markers.py
--rw-r--r--   0        0        0     2476 2023-05-05 22:23:15.399309 gdsfactory-6.91.0/gdsfactory/simulation/convert_sparameters.py
--rw-r--r--   0        0        0      547 2023-05-05 22:23:15.399309 gdsfactory-6.91.0/gdsfactory/simulation/devsim/__init__.py
--rw-r--r--   0        0        0     2559 2023-05-05 22:23:15.399309 gdsfactory-6.91.0/gdsfactory/simulation/devsim/doping.py
--rw-r--r--   0        0        0    11977 2023-05-05 22:23:15.399309 gdsfactory-6.91.0/gdsfactory/simulation/devsim/get_simulation.py
--rw-r--r--   0        0        0    23601 2023-05-05 22:23:15.399309 gdsfactory-6.91.0/gdsfactory/simulation/devsim/get_simulation_xsection.py
--rw-r--r--   0        0        0    19708 2023-05-05 22:23:15.399309 gdsfactory-6.91.0/gdsfactory/simulation/devsim/get_solver.py
--rw-r--r--   0        0        0     1632 2023-05-05 22:23:15.399309 gdsfactory-6.91.0/gdsfactory/simulation/devsim/test_devsim.py
--rw-r--r--   0        0        0      189 2023-05-05 22:23:15.399309 gdsfactory-6.91.0/gdsfactory/simulation/disable_print.py
--rw-r--r--   0        0        0       79 2023-05-05 22:23:15.399309 gdsfactory-6.91.0/gdsfactory/simulation/eme/__init__.py
--rw-r--r--   0        0        0    14784 2023-05-05 22:23:15.399309 gdsfactory-6.91.0/gdsfactory/simulation/eme/meow_eme.py
--rw-r--r--   0        0        0     1771 2023-05-05 22:23:15.399309 gdsfactory-6.91.0/gdsfactory/simulation/eme/test_meow_simulation.py
--rw-r--r--   0        0        0        0 2023-05-05 22:23:15.399309 gdsfactory-6.91.0/gdsfactory/simulation/fem/__init__.py
--rw-r--r--   0        0        0     8968 2023-05-05 22:23:15.399309 gdsfactory-6.91.0/gdsfactory/simulation/fem/mode_solver.py
--rw-r--r--   0        0        0     2205 2023-05-05 22:23:15.399309 gdsfactory-6.91.0/gdsfactory/simulation/fem/test_mode_solver.py
--rw-r--r--   0        0        0     3351 2023-05-05 22:23:15.399309 gdsfactory-6.91.0/gdsfactory/simulation/get_effective_indices.py
--rw-r--r--   0        0        0     3109 2023-05-05 22:23:15.399309 gdsfactory-6.91.0/gdsfactory/simulation/get_modes_path.py
--rw-r--r--   0        0        0     3888 2023-05-05 22:23:15.399309 gdsfactory-6.91.0/gdsfactory/simulation/get_sparameters_path.py
--rw-r--r--   0        0        0     1863 2023-05-05 22:23:15.399309 gdsfactory-6.91.0/gdsfactory/simulation/gmeep/__init__.py
--rw-r--r--   0        0        0     3194 2023-05-05 22:23:15.399309 gdsfactory-6.91.0/gdsfactory/simulation/gmeep/get_material.py
--rw-r--r--   0        0        0     6137 2023-05-05 22:23:15.399309 gdsfactory-6.91.0/gdsfactory/simulation/gmeep/get_meep_geometry.py
--rw-r--r--   0        0        0     6054 2023-05-05 22:23:15.399309 gdsfactory-6.91.0/gdsfactory/simulation/gmeep/get_port_eigenmode.py
--rw-r--r--   0        0        0    11014 2023-05-05 22:23:15.399309 gdsfactory-6.91.0/gdsfactory/simulation/gmeep/get_simulation.py
--rw-r--r--   0        0        0    15701 2023-05-05 22:23:15.399309 gdsfactory-6.91.0/gdsfactory/simulation/gmeep/get_simulation_grating_farfield.py
--rw-r--r--   0        0        0    17944 2023-05-05 22:23:15.399309 gdsfactory-6.91.0/gdsfactory/simulation/gmeep/get_simulation_grating_fiber.py
--rw-r--r--   0        0        0    12302 2023-05-05 22:23:15.399309 gdsfactory-6.91.0/gdsfactory/simulation/gmeep/meep_adjoint_optimization.py
--rw-r--r--   0        0        0    11914 2023-05-05 22:23:15.399309 gdsfactory-6.91.0/gdsfactory/simulation/gmeep/test_eigenmode.py
--rw-r--r--   0        0        0      832 2023-05-05 22:23:15.399309 gdsfactory-6.91.0/gdsfactory/simulation/gmeep/test_materials.py
--rw-r--r--   0        0        0    10128 2023-05-05 22:23:15.403309 gdsfactory-6.91.0/gdsfactory/simulation/gmeep/test_sparameterNxN/test_sparameterNxN_crossing.csv
--rw-r--r--   0        0        0    10128 2023-05-05 22:23:15.403309 gdsfactory-6.91.0/gdsfactory/simulation/gmeep/test_sparameterNxN/test_sparameterNxN_straight.csv
--rw-r--r--   0        0        0     6642 2023-05-05 22:23:15.403309 gdsfactory-6.91.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep.py
--rw-r--r--   0        0        0    10128 2023-05-05 22:23:15.403309 gdsfactory-6.91.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameterNxN_crossing.csv
--rw-r--r--   0        0        0    10128 2023-05-05 22:23:15.403309 gdsfactory-6.91.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameterNxN_straight.csv
--rw-r--r--   0        0        0    10093 2023-05-05 22:23:15.403309 gdsfactory-6.91.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameterNxN_symmetries_straight.csv
--rw-r--r--   0        0        0    10085 2023-05-05 22:23:15.403309 gdsfactory-6.91.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameter_straight_mpi.csv
--rw-r--r--   0        0        0    10085 2023-05-05 22:23:15.403309 gdsfactory-6.91.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameter_straight_mpi_pool.csv
--rw-r--r--   0        0        0    34701 2023-05-05 22:23:15.403309 gdsfactory-6.91.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameters_crossing_symmetric.csv
--rw-r--r--   0        0        0    10123 2023-05-05 22:23:15.403309 gdsfactory-6.91.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameters_straight.csv
--rw-r--r--   0        0        0     9966 2023-05-05 22:23:15.403309 gdsfactory-6.91.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameters_straight_batch.csv
--rw-r--r--   0        0        0     9966 2023-05-05 22:23:15.403309 gdsfactory-6.91.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameters_straight_mpi.csv
--rw-r--r--   0        0        0    10085 2023-05-05 22:23:15.403309 gdsfactory-6.91.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameters_straight_mpi_pool.csv
--rw-r--r--   0        0        0    10129 2023-05-05 22:23:15.403309 gdsfactory-6.91.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameters_straight_symmetric.csv
--rw-r--r--   0        0        0    13951 2023-05-05 22:23:15.403309 gdsfactory-6.91.0/gdsfactory/simulation/gmeep/write_sparameters_grating.py
--rw-r--r--   0        0        0    21273 2023-05-05 22:23:15.403309 gdsfactory-6.91.0/gdsfactory/simulation/gmeep/write_sparameters_meep.py
--rw-r--r--   0        0        0     8135 2023-05-05 22:23:15.403309 gdsfactory-6.91.0/gdsfactory/simulation/gmeep/write_sparameters_meep_batch.py
--rw-r--r--   0        0        0     9561 2023-05-05 22:23:15.403309 gdsfactory-6.91.0/gdsfactory/simulation/gmeep/write_sparameters_meep_mpi.py
--rw-r--r--   0        0        0     1246 2023-05-05 22:23:15.403309 gdsfactory-6.91.0/gdsfactory/simulation/gmsh/__init__.py
--rw-r--r--   0        0        0     6653 2023-05-05 22:23:15.403309 gdsfactory-6.91.0/gdsfactory/simulation/gmsh/break_geometry.py
--rw-r--r--   0        0        0    11250 2023-05-05 22:23:15.403309 gdsfactory-6.91.0/gdsfactory/simulation/gmsh/mesh.py
--rw-r--r--   0        0        0    11808 2023-05-05 22:23:15.403309 gdsfactory-6.91.0/gdsfactory/simulation/gmsh/meshtracker.py
--rw-r--r--   0        0        0     7752 2023-05-05 22:23:15.403309 gdsfactory-6.91.0/gdsfactory/simulation/gmsh/parse_component.py
--rw-r--r--   0        0        0     3644 2023-05-05 22:23:15.403309 gdsfactory-6.91.0/gdsfactory/simulation/gmsh/parse_gds.py
--rw-r--r--   0        0        0     3605 2023-05-05 22:23:15.403309 gdsfactory-6.91.0/gdsfactory/simulation/gmsh/parse_layerstack.py
--rw-r--r--   0        0        0     2990 2023-05-05 22:23:15.403309 gdsfactory-6.91.0/gdsfactory/simulation/gmsh/refine.py
--rw-r--r--   0        0        0    10851 2023-05-05 22:23:15.403309 gdsfactory-6.91.0/gdsfactory/simulation/gmsh/scratch/mesh3D.py
--rw-r--r--   0        0        0     2489 2023-05-05 22:23:15.403309 gdsfactory-6.91.0/gdsfactory/simulation/gmsh/tests/test_meshing.py
--rw-r--r--   0        0        0    14168 2023-05-05 22:23:15.403309 gdsfactory-6.91.0/gdsfactory/simulation/gmsh/uz_xsection_mesh.py
--rw-r--r--   0        0        0     7441 2023-05-05 22:23:15.403309 gdsfactory-6.91.0/gdsfactory/simulation/gmsh/xy_xsection_mesh.py
--rw-r--r--   0        0        0    16326 2023-05-05 22:23:15.403309 gdsfactory-6.91.0/gdsfactory/simulation/gmsh/xyz_mesh.py
--rw-r--r--   0        0        0     1524 2023-05-05 22:23:15.403309 gdsfactory-6.91.0/gdsfactory/simulation/gtidy3d/__init__.py
--rw-r--r--   0        0        0     4368 2023-05-05 22:23:15.403309 gdsfactory-6.91.0/gdsfactory/simulation/gtidy3d/get_results.py
--rw-r--r--   0        0        0    20009 2023-05-05 22:23:15.403309 gdsfactory-6.91.0/gdsfactory/simulation/gtidy3d/get_simulation.py
--rw-r--r--   0        0        0    21061 2023-05-05 22:23:15.403309 gdsfactory-6.91.0/gdsfactory/simulation/gtidy3d/get_simulation_grating_coupler.py
--rw-r--r--   0        0        0     2821 2023-05-05 22:23:15.403309 gdsfactory-6.91.0/gdsfactory/simulation/gtidy3d/materials.py
--rw-r--r--   0        0        0    39677 2023-05-05 22:23:15.403309 gdsfactory-6.91.0/gdsfactory/simulation/gtidy3d/modes.py
--rw-r--r--   0        0        0     8941 2023-05-05 22:23:15.403309 gdsfactory-6.91.0/gdsfactory/simulation/gtidy3d/sim_run.yaml
--rw-r--r--   0        0        0     8114 2023-05-05 22:23:15.403309 gdsfactory-6.91.0/gdsfactory/simulation/gtidy3d/tests/sim_ref.yaml
--rw-r--r--   0        0        0     8114 2023-05-05 22:23:15.403309 gdsfactory-6.91.0/gdsfactory/simulation/gtidy3d/tests/sim_run.yaml
--rw-r--r--   0        0        0     1597 2023-05-05 22:23:15.403309 gdsfactory-6.91.0/gdsfactory/simulation/gtidy3d/tests/test_modes.py
--rw-r--r--   0        0        0      262 2023-05-05 22:23:15.403309 gdsfactory-6.91.0/gdsfactory/simulation/gtidy3d/tests/test_modes/test_sweep_width.csv
--rw-r--r--   0        0        0      879 2023-05-05 22:23:15.403309 gdsfactory-6.91.0/gdsfactory/simulation/gtidy3d/tests/test_results.py
--rw-r--r--   0        0        0     1505 2023-05-05 22:23:15.403309 gdsfactory-6.91.0/gdsfactory/simulation/gtidy3d/tests/test_simulation.py
--rw-r--r--   0        0        0     1270 2023-05-05 22:23:15.403309 gdsfactory-6.91.0/gdsfactory/simulation/gtidy3d/tests/test_write_sparameters.py
--rw-r--r--   0        0        0     9297 2023-05-05 22:23:15.403309 gdsfactory-6.91.0/gdsfactory/simulation/gtidy3d/tests/test_write_sparameters/test_sparameters_straight.csv
--rw-r--r--   0        0        0     1732 2023-05-05 22:23:15.403309 gdsfactory-6.91.0/gdsfactory/simulation/gtidy3d/tests/test_write_sparameters_grating_coupler.py
--rw-r--r--   0        0        0     1224 2023-05-05 22:23:15.403309 gdsfactory-6.91.0/gdsfactory/simulation/gtidy3d/utils.py
--rw-r--r--   0        0        0    10515 2023-05-05 22:23:15.403309 gdsfactory-6.91.0/gdsfactory/simulation/gtidy3d/write_sparameters.py
--rw-r--r--   0        0        0     7695 2023-05-05 22:23:15.403309 gdsfactory-6.91.0/gdsfactory/simulation/gtidy3d/write_sparameters_grating_coupler.py
--rw-r--r--   0        0        0      588 2023-05-05 22:23:15.403309 gdsfactory-6.91.0/gdsfactory/simulation/lumerical/__init__.py
--rw-r--r--   0        0        0    16011 2023-05-05 22:23:15.403309 gdsfactory-6.91.0/gdsfactory/simulation/lumerical/interconnect.py
--rw-r--r--   0        0        0     4286 2023-05-05 22:23:15.403309 gdsfactory-6.91.0/gdsfactory/simulation/lumerical/read.py
--rw-r--r--   0        0        0     3569 2023-05-05 22:23:15.403309 gdsfactory-6.91.0/gdsfactory/simulation/lumerical/settings.py
--rw-r--r--   0        0        0     2348 2023-05-05 22:23:15.407309 gdsfactory-6.91.0/gdsfactory/simulation/lumerical/test_read_sparameters.py
--rw-r--r--   0        0        0    19865 2023-05-05 22:23:15.407309 gdsfactory-6.91.0/gdsfactory/simulation/lumerical/write_sparameters_lumerical.py
--rw-r--r--   0        0        0     1504 2023-05-05 22:23:15.407309 gdsfactory-6.91.0/gdsfactory/simulation/lumerical/write_sparameters_lumerical_components.py
--rw-r--r--   0        0        0      932 2023-05-05 22:23:15.407309 gdsfactory-6.91.0/gdsfactory/simulation/modes/__init__.py
--rw-r--r--   0        0        0     1574 2023-05-05 22:23:15.407309 gdsfactory-6.91.0/gdsfactory/simulation/modes/coupler.py
--rw-r--r--   0        0        0     4132 2023-05-05 22:23:15.407309 gdsfactory-6.91.0/gdsfactory/simulation/modes/find_coupling_vs_gap.py
--rw-r--r--   0        0        0     2534 2023-05-05 22:23:15.407309 gdsfactory-6.91.0/gdsfactory/simulation/modes/find_mode_dispersion.py
--rw-r--r--   0        0        0     8846 2023-05-05 22:23:15.407309 gdsfactory-6.91.0/gdsfactory/simulation/modes/find_modes.py
--rwxr-xr-x   0        0        0     7032 2023-05-05 22:23:15.407309 gdsfactory-6.91.0/gdsfactory/simulation/modes/find_modes_cross_section.py
--rw-r--r--   0        0        0     4448 2023-05-05 22:23:15.407309 gdsfactory-6.91.0/gdsfactory/simulation/modes/find_neff_ng_dw_dh.py
--rw-r--r--   0        0        0     2706 2023-05-05 22:23:15.407309 gdsfactory-6.91.0/gdsfactory/simulation/modes/find_neff_vs_width.py
--rw-r--r--   0        0        0     6956 2023-05-05 22:23:15.407309 gdsfactory-6.91.0/gdsfactory/simulation/modes/get_mode_solver_coupler.py
--rwxr-xr-x   0        0        0     4462 2023-05-05 22:23:15.407309 gdsfactory-6.91.0/gdsfactory/simulation/modes/get_mode_solver_cross_section.py
--rw-r--r--   0        0        0     5257 2023-05-05 22:23:15.407309 gdsfactory-6.91.0/gdsfactory/simulation/modes/get_mode_solver_rib.py
--rw-r--r--   0        0        0     1110 2023-05-05 22:23:15.407309 gdsfactory-6.91.0/gdsfactory/simulation/modes/modes/neff_vs_width_nitride.csv
--rw-r--r--   0        0        0     1102 2023-05-05 22:23:15.407309 gdsfactory-6.91.0/gdsfactory/simulation/modes/modes/neff_vs_width_rib.csv
--rw-r--r--   0        0        0     1110 2023-05-05 22:23:15.407309 gdsfactory-6.91.0/gdsfactory/simulation/modes/modes/neff_vs_width_strip.csv
--rw-r--r--   0        0        0     7979 2023-05-05 22:23:15.407309 gdsfactory-6.91.0/gdsfactory/simulation/modes/neff_convergence_test.py
--rw-r--r--   0        0        0      267 2023-05-05 22:23:15.407309 gdsfactory-6.91.0/gdsfactory/simulation/modes/neff_vs_width.csv
--rw-r--r--   0        0        0     2469 2023-05-05 22:23:15.407309 gdsfactory-6.91.0/gdsfactory/simulation/modes/overlap.py
--rw-r--r--   0        0        0      418 2023-05-05 22:23:15.407309 gdsfactory-6.91.0/gdsfactory/simulation/modes/tests/test_dw_dh.py
--rw-r--r--   0        0        0       83 2023-05-05 22:23:15.407309 gdsfactory-6.91.0/gdsfactory/simulation/modes/tests/test_dw_dh/test_dw_dh.csv
--rw-r--r--   0        0        0      548 2023-05-05 22:23:15.407309 gdsfactory-6.91.0/gdsfactory/simulation/modes/tests/test_dw_dh/test_dw_dh_dispersion.csv
--rw-r--r--   0        0        0     1131 2023-05-05 22:23:15.407309 gdsfactory-6.91.0/gdsfactory/simulation/modes/tests/test_find_modes.py
--rw-r--r--   0        0        0      647 2023-05-05 22:23:15.407309 gdsfactory-6.91.0/gdsfactory/simulation/modes/tests/test_find_modes_dispersion.py
--rw-r--r--   0        0        0      354 2023-05-05 22:23:15.407309 gdsfactory-6.91.0/gdsfactory/simulation/modes/tests/test_neff_vs_width.py
--rw-r--r--   0        0        0      113 2023-05-05 22:23:15.407309 gdsfactory-6.91.0/gdsfactory/simulation/modes/tests/test_neff_vs_width/test_neff_vs_width.csv
--rw-r--r--   0        0        0    15452 2023-05-05 22:23:15.407309 gdsfactory-6.91.0/gdsfactory/simulation/modes/types.py
--rw-r--r--   0        0        0     1145 2023-05-05 22:23:15.407309 gdsfactory-6.91.0/gdsfactory/simulation/modes/waveguide.py
--rw-r--r--   0        0        0     2013 2023-05-05 22:23:15.407309 gdsfactory-6.91.0/gdsfactory/simulation/photonic_circuit_models/__init__.py
--rw-r--r--   0        0        0      597 2023-05-05 22:23:15.407309 gdsfactory-6.91.0/gdsfactory/simulation/photonic_circuit_models/coupler.py
--rw-r--r--   0        0        0      377 2023-05-05 22:23:15.407309 gdsfactory-6.91.0/gdsfactory/simulation/photonic_circuit_models/fsr.py
--rw-r--r--   0        0        0      418 2023-05-05 22:23:15.407309 gdsfactory-6.91.0/gdsfactory/simulation/photonic_circuit_models/heater.py
--rw-r--r--   0        0        0     3063 2023-05-05 22:23:15.407309 gdsfactory-6.91.0/gdsfactory/simulation/photonic_circuit_models/mzi.py
--rw-r--r--   0        0        0     2616 2023-05-05 22:23:15.407309 gdsfactory-6.91.0/gdsfactory/simulation/photonic_circuit_models/ring.py
--rw-r--r--   0        0        0     7332 2023-05-05 22:23:15.407309 gdsfactory-6.91.0/gdsfactory/simulation/plot.py
--rw-r--r--   0        0        0     2480 2023-05-05 22:23:15.407309 gdsfactory-6.91.0/gdsfactory/simulation/plot_csv.py
--rw-r--r--   0        0        0      703 2023-05-05 22:23:15.407309 gdsfactory-6.91.0/gdsfactory/simulation/port_symmetries.py
--rw-r--r--   0        0        0     4637 2023-05-05 22:23:15.407309 gdsfactory-6.91.0/gdsfactory/simulation/process/diffusion.py
--rw-r--r--   0        0        0     5317 2023-05-05 22:23:15.407309 gdsfactory-6.91.0/gdsfactory/simulation/process/implant_tables.py
--rw-r--r--   0        0        0     6784 2023-05-05 22:23:15.407309 gdsfactory-6.91.0/gdsfactory/simulation/process/pysrim.py
--rw-r--r--   0        0        0     2182 2023-05-05 22:23:15.407309 gdsfactory-6.91.0/gdsfactory/simulation/process/silicon.py
--rw-r--r--   0        0        0     1861 2023-05-05 22:23:15.407309 gdsfactory-6.91.0/gdsfactory/simulation/process/skew/antimony_si_skew.csv
--rw-r--r--   0        0        0     1050 2023-05-05 22:23:15.407309 gdsfactory-6.91.0/gdsfactory/simulation/process/skew/arsenic_si_skew.csv
--rw-r--r--   0        0        0     1468 2023-05-05 22:23:15.407309 gdsfactory-6.91.0/gdsfactory/simulation/process/skew/boron_si_skew.csv
--rw-r--r--   0        0        0     1118 2023-05-05 22:23:15.407309 gdsfactory-6.91.0/gdsfactory/simulation/process/skew/phosphorus_si_skew.csv
--rw-r--r--   0        0        0      191 2023-05-05 22:23:15.407309 gdsfactory-6.91.0/gdsfactory/simulation/sax/__init__.py
--rw-r--r--   0        0        0    14792 2023-05-05 22:23:15.407309 gdsfactory-6.91.0/gdsfactory/simulation/sax/build_model.py
--rw-r--r--   0        0        0     7449 2023-05-05 22:23:15.407309 gdsfactory-6.91.0/gdsfactory/simulation/sax/femwell_waveguide_model.py
--rw-r--r--   0        0        0     1571 2023-05-05 22:23:15.407309 gdsfactory-6.91.0/gdsfactory/simulation/sax/interpolators.py
--rw-r--r--   0        0        0     6755 2023-05-05 22:23:15.407309 gdsfactory-6.91.0/gdsfactory/simulation/sax/meep_FDTD_model.py
--rw-r--r--   0        0        0     4528 2023-05-05 22:23:15.407309 gdsfactory-6.91.0/gdsfactory/simulation/sax/meow_eme_model.py
--rw-r--r--   0        0        0     5613 2023-05-05 22:23:15.407309 gdsfactory-6.91.0/gdsfactory/simulation/sax/mlp.py
--rw-r--r--   0        0        0     7358 2023-05-05 22:23:15.407309 gdsfactory-6.91.0/gdsfactory/simulation/sax/models.py
--rw-r--r--   0        0        0    13884 2023-05-05 22:23:15.407309 gdsfactory-6.91.0/gdsfactory/simulation/sax/parameter.py
--rwxr-xr-x   0        0        0     2205 2023-05-05 22:23:15.407309 gdsfactory-6.91.0/gdsfactory/simulation/sax/plot_model.py
--rw-r--r--   0        0        0     6805 2023-05-05 22:23:15.407309 gdsfactory-6.91.0/gdsfactory/simulation/sax/read.py
--rw-r--r--   0        0        0     1350 2023-05-05 22:23:15.407309 gdsfactory-6.91.0/gdsfactory/simulation/sax/tests/test_mzi.py
--rw-r--r--   0        0        0     2220 2023-05-05 22:23:15.407309 gdsfactory-6.91.0/gdsfactory/simulation/sax/tests/test_mzi_lattice.py
--rw-r--r--   0        0        0     1397 2023-05-05 22:23:15.407309 gdsfactory-6.91.0/gdsfactory/simulation/sax/tests/test_parameters.py
--rw-r--r--   0        0        0     1357 2023-05-05 22:23:15.407309 gdsfactory-6.91.0/gdsfactory/simulation/simphony/__init__.py
--rw-r--r--   0        0        0     1573 2023-05-05 22:23:15.407309 gdsfactory-6.91.0/gdsfactory/simulation/simphony/add_gc.py
--rw-r--r--   0        0        0     3383 2023-05-05 22:23:15.407309 gdsfactory-6.91.0/gdsfactory/simulation/simphony/circuit.py
--rw-r--r--   0        0        0      891 2023-05-05 22:23:15.407309 gdsfactory-6.91.0/gdsfactory/simulation/simphony/components/__init__.py
--rw-r--r--   0        0        0     1295 2023-05-05 22:23:15.407309 gdsfactory-6.91.0/gdsfactory/simulation/simphony/components/bend_circular.py
--rw-r--r--   0        0        0     1388 2023-05-05 22:23:15.407309 gdsfactory-6.91.0/gdsfactory/simulation/simphony/components/bend_euler.py
--rw-r--r--   0        0        0     2560 2023-05-05 22:23:15.407309 gdsfactory-6.91.0/gdsfactory/simulation/simphony/components/coupler.py
--rw-r--r--   0        0        0     1046 2023-05-05 22:23:15.407309 gdsfactory-6.91.0/gdsfactory/simulation/simphony/components/coupler_fdtd.py
--rw-r--r--   0        0        0     1848 2023-05-05 22:23:15.407309 gdsfactory-6.91.0/gdsfactory/simulation/simphony/components/coupler_ring.py
--rw-r--r--   0        0        0     1329 2023-05-05 22:23:15.407309 gdsfactory-6.91.0/gdsfactory/simulation/simphony/components/coupler_ring_fdtd.py
--rw-r--r--   0        0        0      589 2023-05-05 22:23:15.407309 gdsfactory-6.91.0/gdsfactory/simulation/simphony/components/coupler_ring_siepic.py
--rw-r--r--   0        0        0      913 2023-05-05 22:23:15.407309 gdsfactory-6.91.0/gdsfactory/simulation/simphony/components/gc.py
--rw-r--r--   0        0        0     2032 2023-05-05 22:23:15.407309 gdsfactory-6.91.0/gdsfactory/simulation/simphony/components/mmi1x2.py
--rw-r--r--   0        0        0     1910 2023-05-05 22:23:15.407309 gdsfactory-6.91.0/gdsfactory/simulation/simphony/components/mmi2x2.py
--rw-r--r--   0        0        0     2618 2023-05-05 22:23:15.407309 gdsfactory-6.91.0/gdsfactory/simulation/simphony/components/mzi.py
--rw-r--r--   0        0        0     1759 2023-05-05 22:23:15.407309 gdsfactory-6.91.0/gdsfactory/simulation/simphony/components/mzi_siepic.py
--rw-r--r--   0        0        0      487 2023-05-05 22:23:15.407309 gdsfactory-6.91.0/gdsfactory/simulation/simphony/components/mzi_thermal.py
--rw-r--r--   0        0        0     2597 2023-05-05 22:23:15.407309 gdsfactory-6.91.0/gdsfactory/simulation/simphony/components/ring_double.py
--rw-r--r--   0        0        0     1665 2023-05-05 22:23:15.407309 gdsfactory-6.91.0/gdsfactory/simulation/simphony/components/ring_double_siepic.py
--rw-r--r--   0        0        0     1782 2023-05-05 22:23:15.407309 gdsfactory-6.91.0/gdsfactory/simulation/simphony/components/ring_single.py
--rw-r--r--   0        0        0     1416 2023-05-05 22:23:15.407309 gdsfactory-6.91.0/gdsfactory/simulation/simphony/components/ring_single_siepic.py
--rw-r--r--   0        0        0     1099 2023-05-05 22:23:15.407309 gdsfactory-6.91.0/gdsfactory/simulation/simphony/components/straight.py
--rw-r--r--   0        0        0      800 2023-05-05 22:23:15.407309 gdsfactory-6.91.0/gdsfactory/simulation/simphony/get_transmission.py
--rw-r--r--   0        0        0     2516 2023-05-05 22:23:15.407309 gdsfactory-6.91.0/gdsfactory/simulation/simphony/model_from_gdsfactory.py
--rw-r--r--   0        0        0     3841 2023-05-05 22:23:15.407309 gdsfactory-6.91.0/gdsfactory/simulation/simphony/model_from_sparameters.py
--rw-r--r--   0        0        0     2438 2023-05-05 22:23:15.407309 gdsfactory-6.91.0/gdsfactory/simulation/simphony/plot_circuit.py
--rw-r--r--   0        0        0     1798 2023-05-05 22:23:15.407309 gdsfactory-6.91.0/gdsfactory/simulation/simphony/plot_circuit_montecarlo.py
--rw-r--r--   0        0        0     2773 2023-05-05 22:23:15.407309 gdsfactory-6.91.0/gdsfactory/simulation/simphony/plot_model.py
--rw-r--r--   0        0        0     1261 2023-05-05 22:23:15.407309 gdsfactory-6.91.0/gdsfactory/simulation/simphony/tests/test_circuit.py
--rw-r--r--   0        0        0       90 2023-05-05 22:23:15.407309 gdsfactory-6.91.0/gdsfactory/simulation/simphony/tests/test_circuit/test_circuit_transmission.yml
--rw-r--r--   0        0        0     1109 2023-05-05 22:23:15.407309 gdsfactory-6.91.0/gdsfactory/simulation/simphony/tests/test_components.py
--rw-r--r--   0        0        0       66 2023-05-05 22:23:15.407309 gdsfactory-6.91.0/gdsfactory/simulation/simphony/tests/test_components/test_circuits_mzi_.yml
--rw-r--r--   0        0        0       69 2023-05-05 22:23:15.407309 gdsfactory-6.91.0/gdsfactory/simulation/simphony/tests/test_components/test_circuits_ring_double_.yml
--rw-r--r--   0        0        0       69 2023-05-05 22:23:15.407309 gdsfactory-6.91.0/gdsfactory/simulation/simphony/tests/test_components/test_circuits_ring_single_.yml
--rw-r--r--   0        0        0       92 2023-05-05 22:23:15.407309 gdsfactory-6.91.0/gdsfactory/simulation/simphony/tests/test_components/test_elements_bend_circular_.yml
--rw-r--r--   0        0        0       92 2023-05-05 22:23:15.407309 gdsfactory-6.91.0/gdsfactory/simulation/simphony/tests/test_components/test_elements_bend_euler_.yml
--rw-r--r--   0        0        0      412 2023-05-05 22:23:15.407309 gdsfactory-6.91.0/gdsfactory/simulation/simphony/tests/test_components/test_elements_coupler_.yml
--rw-r--r--   0        0        0      412 2023-05-05 22:23:15.407309 gdsfactory-6.91.0/gdsfactory/simulation/simphony/tests/test_components/test_elements_coupler_ring_.yml
--rw-r--r--   0        0        0      114 2023-05-05 22:23:15.407309 gdsfactory-6.91.0/gdsfactory/simulation/simphony/tests/test_components/test_elements_gc1550te_.yml
--rw-r--r--   0        0        0      256 2023-05-05 22:23:15.407309 gdsfactory-6.91.0/gdsfactory/simulation/simphony/tests/test_components/test_elements_mmi1x2_.yml
--rw-r--r--   0        0        0      460 2023-05-05 22:23:15.407309 gdsfactory-6.91.0/gdsfactory/simulation/simphony/tests/test_components/test_elements_mmi2x2_.yml
--rw-r--r--   0        0        0      104 2023-05-05 22:23:15.411309 gdsfactory-6.91.0/gdsfactory/simulation/simphony/tests/test_components/test_elements_straight_.yml
--rw-r--r--   0        0        0      166 2023-05-05 22:23:15.411309 gdsfactory-6.91.0/gdsfactory/simulation/simphony/types.py
--rw-r--r--   0        0        0      471 2023-05-05 22:23:15.411309 gdsfactory-6.91.0/gdsfactory/simulation/sipann/__init__.py
--rw-r--r--   0        0        0     1376 2023-05-05 22:23:15.411309 gdsfactory-6.91.0/gdsfactory/simulation/sipann/bend_circular.py
--rw-r--r--   0        0        0     1465 2023-05-05 22:23:15.411309 gdsfactory-6.91.0/gdsfactory/simulation/sipann/bend_euler.py
--rw-r--r--   0        0        0     2508 2023-05-05 22:23:15.411309 gdsfactory-6.91.0/gdsfactory/simulation/sipann/coupler.py
--rw-r--r--   0        0        0     1892 2023-05-05 22:23:15.411309 gdsfactory-6.91.0/gdsfactory/simulation/sipann/coupler_ring.py
--rw-r--r--   0        0        0      736 2023-05-05 22:23:15.411309 gdsfactory-6.91.0/gdsfactory/simulation/sipann/straight.py
--rw-r--r--   0        0        0      100 2023-05-05 22:23:15.411309 gdsfactory-6.91.0/gdsfactory/simulation/thermal/__init__.py
--rw-r--r--   0        0        0     7781 2023-05-05 22:23:15.411309 gdsfactory-6.91.0/gdsfactory/simulation/thermal/heater.py
--rw-r--r--   0        0        0     1744 2023-05-05 22:23:15.411309 gdsfactory-6.91.0/gdsfactory/snap.py
--rw-r--r--   0        0        0     4245 2023-05-05 22:23:15.411309 gdsfactory-6.91.0/gdsfactory/symbols.py
--rw-r--r--   0        0        0      524 2023-05-05 22:23:15.411309 gdsfactory-6.91.0/gdsfactory/technology/__init__.py
--rw-r--r--   0        0        0     7065 2023-05-05 22:23:15.411309 gdsfactory-6.91.0/gdsfactory/technology/klayout_tech.py
--rw-r--r--   0        0        0     1078 2023-05-05 22:23:15.411309 gdsfactory-6.91.0/gdsfactory/technology/layer_map.py
--rw-r--r--   0        0        0    14989 2023-05-05 22:23:15.411309 gdsfactory-6.91.0/gdsfactory/technology/layer_stack.py
--rw-r--r--   0        0        0    42052 2023-05-05 22:23:15.411309 gdsfactory-6.91.0/gdsfactory/technology/layer_views.py
--rw-r--r--   0        0        0     1984 2023-05-05 22:23:15.411309 gdsfactory-6.91.0/gdsfactory/technology/simulation_settings.py
--rw-r--r--   0        0        0     1635 2023-05-05 22:23:15.411309 gdsfactory-6.91.0/gdsfactory/types.py
--rw-r--r--   0        0        0    10000 2023-05-05 22:23:15.411309 gdsfactory-6.91.0/gdsfactory/typings.py
--rw-r--r--   0        0        0        0 2023-05-05 22:23:15.411309 gdsfactory-6.91.0/gdsfactory/utils/__init__.py
--rw-r--r--   0        0        0     1304 2023-05-05 22:23:15.411309 gdsfactory-6.91.0/gdsfactory/utils/async_utils.py
--rw-r--r--   0        0        0      376 2023-05-05 22:23:15.411309 gdsfactory-6.91.0/gdsfactory/utils/color_utils.py
--rw-r--r--   0        0        0      558 2023-05-05 22:23:15.411309 gdsfactory-6.91.0/gdsfactory/utils/file_utils.py
--rw-r--r--   0        0        0      185 2023-05-05 22:23:15.411309 gdsfactory-6.91.0/gdsfactory/utils/function_utils.py
--rw-r--r--   0        0        0      676 2023-05-05 22:23:15.411309 gdsfactory-6.91.0/gdsfactory/utils/xml_utils.py
--rw-r--r--   0        0        0     1429 2023-05-05 22:23:15.411309 gdsfactory-6.91.0/gdsfactory/utils/yaml_utils.py
--rw-r--r--   0        0        0     4825 2023-05-05 22:23:15.411309 gdsfactory-6.91.0/gdsfactory/watch.py
--rw-r--r--   0        0        0        0 2023-05-05 22:23:15.411309 gdsfactory-6.91.0/gdsfactory/widgets/__init__.py
--rw-r--r--   0        0        0     7921 2023-05-05 22:23:15.411309 gdsfactory-6.91.0/gdsfactory/widgets/layout_viewer.py
--rw-r--r--   0        0        0     7454 2023-05-05 22:23:15.411309 gdsfactory-6.91.0/gdsfactory/write_cells.py
--rw-r--r--   0        0        0     5467 2023-05-05 22:23:15.411309 gdsfactory-6.91.0/pyproject.toml
--rw-r--r--   0        0        0    18547 1970-01-01 00:00:00.000000 gdsfactory-6.91.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-05-09 00:30:20.304903 gdsfactory-6.92.0/LICENSE
+-rw-r--r--   0        0        0    14281 2023-05-09 00:30:20.304903 gdsfactory-6.92.0/README.md
+-rw-r--r--   0        0        0     3415 2023-05-09 00:30:20.312903 gdsfactory-6.92.0/gdsfactory/__init__.py
+-rw-r--r--   0        0        0     2096 2023-05-09 00:30:20.312903 gdsfactory-6.92.0/gdsfactory/add_keepout.py
+-rw-r--r--   0        0        0    12629 2023-05-09 00:30:20.312903 gdsfactory-6.92.0/gdsfactory/add_labels.py
+-rw-r--r--   0        0        0     3711 2023-05-09 00:30:20.312903 gdsfactory-6.92.0/gdsfactory/add_loopback.py
+-rw-r--r--   0        0        0     5054 2023-05-09 00:30:20.312903 gdsfactory-6.92.0/gdsfactory/add_padding.py
+-rw-r--r--   0        0        0    15465 2023-05-09 00:30:20.312903 gdsfactory-6.92.0/gdsfactory/add_pins.py
+-rw-r--r--   0        0        0    14700 2023-05-09 00:30:20.312903 gdsfactory-6.92.0/gdsfactory/add_ports.py
+-rw-r--r--   0        0        0     2884 2023-05-09 00:30:20.312903 gdsfactory-6.92.0/gdsfactory/add_tapers.py
+-rw-r--r--   0        0        0     2257 2023-05-09 00:30:20.312903 gdsfactory-6.92.0/gdsfactory/add_tapers_cross_section.py
+-rw-r--r--   0        0        0     1831 2023-05-09 00:30:20.312903 gdsfactory-6.92.0/gdsfactory/add_termination.py
+-rw-r--r--   0        0        0     1676 2023-05-09 00:30:20.312903 gdsfactory-6.92.0/gdsfactory/asserts.py
+-rw-r--r--   0        0        0    11843 2023-05-09 00:30:20.312903 gdsfactory-6.92.0/gdsfactory/cell.py
+-rw-r--r--   0        0        0    15946 2023-05-09 00:30:20.312903 gdsfactory-6.92.0/gdsfactory/circuitviz.py
+-rw-r--r--   0        0        0     5325 2023-05-09 00:30:20.312903 gdsfactory-6.92.0/gdsfactory/cli.py
+-rw-r--r--   0        0        0    99181 2023-05-09 00:30:20.312903 gdsfactory-6.92.0/gdsfactory/component.py
+-rw-r--r--   0        0        0    23360 2023-05-09 00:30:20.312903 gdsfactory-6.92.0/gdsfactory/component_layout.py
+-rw-r--r--   0        0        0    29699 2023-05-09 00:30:20.312903 gdsfactory-6.92.0/gdsfactory/component_reference.py
+-rw-r--r--   0        0        0     1205 2023-05-09 00:30:20.312903 gdsfactory-6.92.0/gdsfactory/components/C.py
+-rw-r--r--   0        0        0     1144 2023-05-09 00:30:20.312903 gdsfactory-6.92.0/gdsfactory/components/L.py
+-rw-r--r--   0        0        0    20964 2023-05-09 00:30:20.312903 gdsfactory-6.92.0/gdsfactory/components/__init__.py
+-rw-r--r--   0        0        0     2621 2023-05-09 00:30:20.312903 gdsfactory-6.92.0/gdsfactory/components/add_fiducials.py
+-rw-r--r--   0        0        0    14087 2023-05-09 00:30:20.312903 gdsfactory-6.92.0/gdsfactory/components/add_grating_couplers.py
+-rw-r--r--   0        0        0     2014 2023-05-09 00:30:20.312903 gdsfactory-6.92.0/gdsfactory/components/add_trenches.py
+-rw-r--r--   0        0        0     3207 2023-05-09 00:30:20.312903 gdsfactory-6.92.0/gdsfactory/components/align.py
+-rw-r--r--   0        0        0     2622 2023-05-09 00:30:20.312903 gdsfactory-6.92.0/gdsfactory/components/array_component.py
+-rw-r--r--   0        0        0     4705 2023-05-09 00:30:20.312903 gdsfactory-6.92.0/gdsfactory/components/array_with_fanout.py
+-rw-r--r--   0        0        0     4322 2023-05-09 00:30:20.312903 gdsfactory-6.92.0/gdsfactory/components/array_with_via.py
+-rw-r--r--   0        0        0     4042 2023-05-09 00:30:20.312903 gdsfactory-6.92.0/gdsfactory/components/awg.py
+-rw-r--r--   0        0        0     1269 2023-05-09 00:30:20.312903 gdsfactory-6.92.0/gdsfactory/components/bbox.py
+-rw-r--r--   0        0        0     2851 2023-05-09 00:30:20.312903 gdsfactory-6.92.0/gdsfactory/components/bend_circular.py
+-rw-r--r--   0        0        0     2649 2023-05-09 00:30:20.312903 gdsfactory-6.92.0/gdsfactory/components/bend_circular_heater.py
+-rw-r--r--   0        0        0     7882 2023-05-09 00:30:20.312903 gdsfactory-6.92.0/gdsfactory/components/bend_euler.py
+-rw-r--r--   0        0        0     2682 2023-05-09 00:30:20.312903 gdsfactory-6.92.0/gdsfactory/components/bend_port.py
+-rw-r--r--   0        0        0     3664 2023-05-09 00:30:20.312903 gdsfactory-6.92.0/gdsfactory/components/bend_s.py
+-rw-r--r--   0        0        0     5373 2023-05-09 00:30:20.312903 gdsfactory-6.92.0/gdsfactory/components/bezier.py
+-rw-r--r--   0        0        0     1605 2023-05-09 00:30:20.312903 gdsfactory-6.92.0/gdsfactory/components/cavity.py
+-rw-r--r--   0        0        0     5766 2023-05-09 00:30:20.312903 gdsfactory-6.92.0/gdsfactory/components/cdc.py
+-rw-r--r--   0        0        0     2929 2023-05-09 00:30:20.312903 gdsfactory-6.92.0/gdsfactory/components/cdsem_all.py
+-rw-r--r--   0        0        0     1788 2023-05-09 00:30:20.312903 gdsfactory-6.92.0/gdsfactory/components/cdsem_bend180.py
+-rw-r--r--   0        0        0     1631 2023-05-09 00:30:20.312903 gdsfactory-6.92.0/gdsfactory/components/cdsem_coupler.py
+-rw-r--r--   0        0        0     1412 2023-05-09 00:30:20.312903 gdsfactory-6.92.0/gdsfactory/components/cdsem_straight.py
+-rw-r--r--   0        0        0     1565 2023-05-09 00:30:20.316903 gdsfactory-6.92.0/gdsfactory/components/cdsem_straight_density.py
+-rw-r--r--   0        0        0      793 2023-05-09 00:30:20.316903 gdsfactory-6.92.0/gdsfactory/components/circle.py
+-rw-r--r--   0        0        0     5722 2023-05-09 00:30:20.316903 gdsfactory-6.92.0/gdsfactory/components/coh_rx_dual_pol.py
+-rw-r--r--   0        0        0     8922 2023-05-09 00:30:20.316903 gdsfactory-6.92.0/gdsfactory/components/coh_rx_single_pol.py
+-rw-r--r--   0        0        0     5043 2023-05-09 00:30:20.316903 gdsfactory-6.92.0/gdsfactory/components/coh_tx_dual_pol.py
+-rw-r--r--   0        0        0     6118 2023-05-09 00:30:20.316903 gdsfactory-6.92.0/gdsfactory/components/coh_tx_single_pol.py
+-rw-r--r--   0        0        0     2548 2023-05-09 00:30:20.316903 gdsfactory-6.92.0/gdsfactory/components/compass.py
+-rw-r--r--   0        0        0     9856 2023-05-09 00:30:20.316903 gdsfactory-6.92.0/gdsfactory/components/component_lattice.py
+-rw-r--r--   0        0        0     7174 2023-05-09 00:30:20.316903 gdsfactory-6.92.0/gdsfactory/components/component_sequence.py
+-rw-r--r--   0        0        0      812 2023-05-09 00:30:20.316903 gdsfactory-6.92.0/gdsfactory/components/copy_layers.py
+-rw-r--r--   0        0        0     3460 2023-05-09 00:30:20.316903 gdsfactory-6.92.0/gdsfactory/components/coupler.py
+-rw-r--r--   0        0        0     2113 2023-05-09 00:30:20.316903 gdsfactory-6.92.0/gdsfactory/components/coupler90.py
+-rw-r--r--   0        0        0     1802 2023-05-09 00:30:20.316903 gdsfactory-6.92.0/gdsfactory/components/coupler90bend.py
+-rw-r--r--   0        0        0     4666 2023-05-09 00:30:20.316903 gdsfactory-6.92.0/gdsfactory/components/coupler_adiabatic.py
+-rw-r--r--   0        0        0     1909 2023-05-09 00:30:20.316903 gdsfactory-6.92.0/gdsfactory/components/coupler_asymmetric.py
+-rw-r--r--   0        0        0     3970 2023-05-09 00:30:20.316903 gdsfactory-6.92.0/gdsfactory/components/coupler_full.py
+-rw-r--r--   0        0        0     3414 2023-05-09 00:30:20.316903 gdsfactory-6.92.0/gdsfactory/components/coupler_ring.py
+-rw-r--r--   0        0        0     1060 2023-05-09 00:30:20.316903 gdsfactory-6.92.0/gdsfactory/components/coupler_straight.py
+-rw-r--r--   0        0        0     1164 2023-05-09 00:30:20.316903 gdsfactory-6.92.0/gdsfactory/components/coupler_straight_asymmetric.py
+-rw-r--r--   0        0        0     2192 2023-05-09 00:30:20.316903 gdsfactory-6.92.0/gdsfactory/components/coupler_symmetric.py
+-rw-r--r--   0        0        0     1848 2023-05-09 00:30:20.316903 gdsfactory-6.92.0/gdsfactory/components/cross.py
+-rw-r--r--   0        0        0    12873 2023-05-09 00:30:20.316903 gdsfactory-6.92.0/gdsfactory/components/crossing_waveguide.py
+-rw-r--r--   0        0        0      500 2023-05-09 00:30:20.316903 gdsfactory-6.92.0/gdsfactory/components/csv_data/grating_coupler_1etch_h220_e70.csv
+-rw-r--r--   0        0        0     1014 2023-05-09 00:30:20.316903 gdsfactory-6.92.0/gdsfactory/components/csv_data/grating_coupler_2etch_h220_e70_e220.csv
+-rw-r--r--   0        0        0    19749 2023-05-09 00:30:20.316903 gdsfactory-6.92.0/gdsfactory/components/csv_data/taper_strip_0p5_10_100.csv
+-rw-r--r--   0        0        0    19751 2023-05-09 00:30:20.316903 gdsfactory-6.92.0/gdsfactory/components/csv_data/taper_strip_0p5_10_150.csv
+-rw-r--r--   0        0        0    19749 2023-05-09 00:30:20.316903 gdsfactory-6.92.0/gdsfactory/components/csv_data/taper_strip_0p5_10_200.csv
+-rw-r--r--   0        0        0    19751 2023-05-09 00:30:20.316903 gdsfactory-6.92.0/gdsfactory/components/csv_data/taper_strip_0p5_11_200.csv
+-rw-r--r--   0        0        0    19775 2023-05-09 00:30:20.316903 gdsfactory-6.92.0/gdsfactory/components/csv_data/taper_strip_0p5_12_200.csv
+-rw-r--r--   0        0        0     3143 2023-05-09 00:30:20.316903 gdsfactory-6.92.0/gdsfactory/components/csv_data/taper_strip_0p5_3_36.csv
+-rw-r--r--   0        0        0     5272 2023-05-09 00:30:20.316903 gdsfactory-6.92.0/gdsfactory/components/cutback_2x2.py
+-rw-r--r--   0        0        0     6450 2023-05-09 00:30:20.316903 gdsfactory-6.92.0/gdsfactory/components/cutback_bend.py
+-rw-r--r--   0        0        0     3765 2023-05-09 00:30:20.316903 gdsfactory-6.92.0/gdsfactory/components/cutback_component.py
+-rw-r--r--   0        0        0     2721 2023-05-09 00:30:20.316903 gdsfactory-6.92.0/gdsfactory/components/cutback_splitter.py
+-rw-r--r--   0        0        0     2971 2023-05-09 00:30:20.316903 gdsfactory-6.92.0/gdsfactory/components/dbr.py
+-rw-r--r--   0        0        0     4288 2023-05-09 00:30:20.316903 gdsfactory-6.92.0/gdsfactory/components/dbr_tapered.py
+-rw-r--r--   0        0        0     2486 2023-05-09 00:30:20.316903 gdsfactory-6.92.0/gdsfactory/components/delay_snake.py
+-rw-r--r--   0        0        0     3177 2023-05-09 00:30:20.316903 gdsfactory-6.92.0/gdsfactory/components/delay_snake2.py
+-rw-r--r--   0        0        0     3237 2023-05-09 00:30:20.316903 gdsfactory-6.92.0/gdsfactory/components/delay_snake3.py
+-rw-r--r--   0        0        0     4319 2023-05-09 00:30:20.316903 gdsfactory-6.92.0/gdsfactory/components/delay_snake_sbend.py
+-rw-r--r--   0        0        0     1226 2023-05-09 00:30:20.316903 gdsfactory-6.92.0/gdsfactory/components/dicing_lane.py
+-rw-r--r--   0        0        0     3471 2023-05-09 00:30:20.316903 gdsfactory-6.92.0/gdsfactory/components/die.py
+-rw-r--r--   0        0        0     2975 2023-05-09 00:30:20.316903 gdsfactory-6.92.0/gdsfactory/components/die_bbox.py
+-rw-r--r--   0        0        0     2863 2023-05-09 00:30:20.316903 gdsfactory-6.92.0/gdsfactory/components/die_bbox_frame.py
+-rw-r--r--   0        0        0     8015 2023-05-09 00:30:20.316903 gdsfactory-6.92.0/gdsfactory/components/disk.py
+-rw-r--r--   0        0        0     4112 2023-05-09 00:30:20.316903 gdsfactory-6.92.0/gdsfactory/components/edge_coupler_array.py
+-rw-r--r--   0        0        0     1214 2023-05-09 00:30:20.316903 gdsfactory-6.92.0/gdsfactory/components/ellipse.py
+-rw-r--r--   0        0        0     1800 2023-05-09 00:30:20.316903 gdsfactory-6.92.0/gdsfactory/components/extend_ports_list.py
+-rw-r--r--   0        0        0     7944 2023-05-09 00:30:20.316903 gdsfactory-6.92.0/gdsfactory/components/extension.py
+-rw-r--r--   0        0        0      981 2023-05-09 00:30:20.316903 gdsfactory-6.92.0/gdsfactory/components/fiber.py
+-rw-r--r--   0        0        0     1432 2023-05-09 00:30:20.316903 gdsfactory-6.92.0/gdsfactory/components/fiber_array.py
+-rw-r--r--   0        0        0      722 2023-05-09 00:30:20.316903 gdsfactory-6.92.0/gdsfactory/components/fiducial_squares.py
+-rw-r--r--   0        0        0     3290 2023-05-09 00:30:20.316903 gdsfactory-6.92.0/gdsfactory/components/ge_detector_straight_si_contacts.py
+-rw-r--r--   0        0        0     1063 2023-05-09 00:30:20.316903 gdsfactory-6.92.0/gdsfactory/components/grating_coupler_array.py
+-rw-r--r--   0        0        0     4682 2023-05-09 00:30:20.316903 gdsfactory-6.92.0/gdsfactory/components/grating_coupler_dual_pol.py
+-rw-r--r--   0        0        0     7110 2023-05-09 00:30:20.316903 gdsfactory-6.92.0/gdsfactory/components/grating_coupler_elliptical.py
+-rw-r--r--   0        0        0     7221 2023-05-09 00:30:20.316903 gdsfactory-6.92.0/gdsfactory/components/grating_coupler_elliptical_arbitrary.py
+-rw-r--r--   0        0        0     4960 2023-05-09 00:30:20.316903 gdsfactory-6.92.0/gdsfactory/components/grating_coupler_elliptical_lumerical.py
+-rw-r--r--   0        0        0     4592 2023-05-09 00:30:20.316903 gdsfactory-6.92.0/gdsfactory/components/grating_coupler_elliptical_trenches.py
+-rw-r--r--   0        0        0     1773 2023-05-09 00:30:20.316903 gdsfactory-6.92.0/gdsfactory/components/grating_coupler_functions.py
+-rw-r--r--   0        0        0     9058 2023-05-09 00:30:20.316903 gdsfactory-6.92.0/gdsfactory/components/grating_coupler_loss.py
+-rw-r--r--   0        0        0     1786 2023-05-09 00:30:20.316903 gdsfactory-6.92.0/gdsfactory/components/grating_coupler_loss_fiber_single.py
+-rw-r--r--   0        0        0     4142 2023-05-09 00:30:20.316903 gdsfactory-6.92.0/gdsfactory/components/grating_coupler_rectangular.py
+-rw-r--r--   0        0        0     4685 2023-05-09 00:30:20.316903 gdsfactory-6.92.0/gdsfactory/components/grating_coupler_rectangular_arbitrary.py
+-rw-r--r--   0        0        0     3887 2023-05-09 00:30:20.316903 gdsfactory-6.92.0/gdsfactory/components/grating_coupler_rectangular_arbitrary_slab.py
+-rw-r--r--   0        0        0     1578 2023-05-09 00:30:20.316903 gdsfactory-6.92.0/gdsfactory/components/grating_coupler_tree.py
+-rw-r--r--   0        0        0     8773 2023-05-09 00:30:20.316903 gdsfactory-6.92.0/gdsfactory/components/greek_cross.py
+-rw-r--r--   0        0        0     1019 2023-05-09 00:30:20.316903 gdsfactory-6.92.0/gdsfactory/components/hline.py
+-rw-r--r--   0        0        0     3687 2023-05-09 00:30:20.316903 gdsfactory-6.92.0/gdsfactory/components/interdigital_capacitor.py
+-rw-r--r--   0        0        0     1825 2023-05-09 00:30:20.316903 gdsfactory-6.92.0/gdsfactory/components/litho_calipers.py
+-rw-r--r--   0        0        0     1244 2023-05-09 00:30:20.316903 gdsfactory-6.92.0/gdsfactory/components/litho_ruler.py
+-rw-r--r--   0        0        0     1304 2023-05-09 00:30:20.316903 gdsfactory-6.92.0/gdsfactory/components/litho_steps.py
+-rw-r--r--   0        0        0      650 2023-05-09 00:30:20.316903 gdsfactory-6.92.0/gdsfactory/components/logo.py
+-rw-r--r--   0        0        0     1679 2023-05-09 00:30:20.316903 gdsfactory-6.92.0/gdsfactory/components/loop_mirror.py
+-rw-r--r--   0        0        0     3873 2023-05-09 00:30:20.316903 gdsfactory-6.92.0/gdsfactory/components/mmi1x2.py
+-rw-r--r--   0        0        0     2814 2023-05-09 00:30:20.316903 gdsfactory-6.92.0/gdsfactory/components/mmi1x2_with_sbend.py
+-rw-r--r--   0        0        0     3858 2023-05-09 00:30:20.316903 gdsfactory-6.92.0/gdsfactory/components/mmi2x2.py
+-rw-r--r--   0        0        0     3299 2023-05-09 00:30:20.316903 gdsfactory-6.92.0/gdsfactory/components/mmi2x2_with_sbend.py
+-rw-r--r--   0        0        0     4947 2023-05-09 00:30:20.316903 gdsfactory-6.92.0/gdsfactory/components/mmi_90degree_hybrid.py
+-rw-r--r--   0        0        0     3265 2023-05-09 00:30:20.316903 gdsfactory-6.92.0/gdsfactory/components/mode_converter.py
+-rw-r--r--   0        0        0     7414 2023-05-09 00:30:20.320903 gdsfactory-6.92.0/gdsfactory/components/mzi.py
+-rw-r--r--   0        0        0     2499 2023-05-09 00:30:20.320903 gdsfactory-6.92.0/gdsfactory/components/mzi_arm.py
+-rw-r--r--   0        0        0     5835 2023-05-09 00:30:20.320903 gdsfactory-6.92.0/gdsfactory/components/mzi_arms.py
+-rw-r--r--   0        0        0    12214 2023-05-09 00:30:20.320903 gdsfactory-6.92.0/gdsfactory/components/mzi_lattice.py
+-rw-r--r--   0        0        0     4025 2023-05-09 00:30:20.320903 gdsfactory-6.92.0/gdsfactory/components/mzi_pads_center.py
+-rw-r--r--   0        0        0     1064 2023-05-09 00:30:20.320903 gdsfactory-6.92.0/gdsfactory/components/mzi_phase_shifter.py
+-rw-r--r--   0        0        0     6342 2023-05-09 00:30:20.320903 gdsfactory-6.92.0/gdsfactory/components/mzit.py
+-rw-r--r--   0        0        0     3502 2023-05-09 00:30:20.320903 gdsfactory-6.92.0/gdsfactory/components/mzit_lattice.py
+-rw-r--r--   0        0        0     6047 2023-05-09 00:30:20.320903 gdsfactory-6.92.0/gdsfactory/components/mzm.py
+-rw-r--r--   0        0        0     3518 2023-05-09 00:30:20.320903 gdsfactory-6.92.0/gdsfactory/components/nxn.py
+-rw-r--r--   0        0        0     1940 2023-05-09 00:30:20.320903 gdsfactory-6.92.0/gdsfactory/components/optimal_90deg.py
+-rw-r--r--   0        0        0     3876 2023-05-09 00:30:20.320903 gdsfactory-6.92.0/gdsfactory/components/optimal_hairpin.py
+-rw-r--r--   0        0        0     6131 2023-05-09 00:30:20.320903 gdsfactory-6.92.0/gdsfactory/components/optimal_step.py
+-rw-r--r--   0        0        0     6327 2023-05-09 00:30:20.320903 gdsfactory-6.92.0/gdsfactory/components/pack_doe.py
+-rw-r--r--   0        0        0     3860 2023-05-09 00:30:20.320903 gdsfactory-6.92.0/gdsfactory/components/pad.py
+-rw-r--r--   0        0        0     1890 2023-05-09 00:30:20.320903 gdsfactory-6.92.0/gdsfactory/components/pad_gsg.py
+-rw-r--r--   0        0        0     1157 2023-05-09 00:30:20.320903 gdsfactory-6.92.0/gdsfactory/components/pads_shorted.py
+-rw-r--r--   0        0        0     3833 2023-05-09 00:30:20.320903 gdsfactory-6.92.0/gdsfactory/components/polarization_splitter_rotator.py
+-rw-r--r--   0        0        0     1147 2023-05-09 00:30:20.320903 gdsfactory-6.92.0/gdsfactory/components/ramp.py
+-rw-r--r--   0        0        0     1508 2023-05-09 00:30:20.320903 gdsfactory-6.92.0/gdsfactory/components/rectangle.py
+-rw-r--r--   0        0        0     2972 2023-05-09 00:30:20.320903 gdsfactory-6.92.0/gdsfactory/components/rectangle_with_slits.py
+-rw-r--r--   0        0        0     1508 2023-05-09 00:30:20.320903 gdsfactory-6.92.0/gdsfactory/components/regular_polygon.py
+-rw-r--r--   0        0        0     3302 2023-05-09 00:30:20.320903 gdsfactory-6.92.0/gdsfactory/components/resistance_meander.py
+-rw-r--r--   0        0        0     2642 2023-05-09 00:30:20.320903 gdsfactory-6.92.0/gdsfactory/components/resistance_sheet.py
+-rw-r--r--   0        0        0     1273 2023-05-09 00:30:20.320903 gdsfactory-6.92.0/gdsfactory/components/ring.py
+-rw-r--r--   0        0        0     4143 2023-05-09 00:30:20.320903 gdsfactory-6.92.0/gdsfactory/components/ring_crow.py
+-rw-r--r--   0        0        0     3272 2023-05-09 00:30:20.320903 gdsfactory-6.92.0/gdsfactory/components/ring_crow_couplers.py
+-rw-r--r--   0        0        0     2267 2023-05-09 00:30:20.320903 gdsfactory-6.92.0/gdsfactory/components/ring_double.py
+-rw-r--r--   0        0        0     3846 2023-05-09 00:30:20.320903 gdsfactory-6.92.0/gdsfactory/components/ring_double_heater.py
+-rw-r--r--   0        0        0     7757 2023-05-09 00:30:20.320903 gdsfactory-6.92.0/gdsfactory/components/ring_double_pn.py
+-rw-r--r--   0        0        0    12137 2023-05-09 00:30:20.320903 gdsfactory-6.92.0/gdsfactory/components/ring_section_based.py
+-rw-r--r--   0        0        0     2719 2023-05-09 00:30:20.320903 gdsfactory-6.92.0/gdsfactory/components/ring_single.py
+-rw-r--r--   0        0        0     1968 2023-05-09 00:30:20.320903 gdsfactory-6.92.0/gdsfactory/components/ring_single_array.py
+-rw-r--r--   0        0        0     6098 2023-05-09 00:30:20.320903 gdsfactory-6.92.0/gdsfactory/components/ring_single_bend_coupler.py
+-rw-r--r--   0        0        0     2714 2023-05-09 00:30:20.320903 gdsfactory-6.92.0/gdsfactory/components/ring_single_dut.py
+-rw-r--r--   0        0        0     4018 2023-05-09 00:30:20.320903 gdsfactory-6.92.0/gdsfactory/components/ring_single_heater.py
+-rw-r--r--   0        0        0     5267 2023-05-09 00:30:20.320903 gdsfactory-6.92.0/gdsfactory/components/ring_single_pn.py
+-rw-r--r--   0        0        0     2282 2023-05-09 00:30:20.320903 gdsfactory-6.92.0/gdsfactory/components/seal_ring.py
+-rw-r--r--   0        0        0     3758 2023-05-09 00:30:20.320903 gdsfactory-6.92.0/gdsfactory/components/snspd.py
+-rw-r--r--   0        0        0     2059 2023-05-09 00:30:20.320903 gdsfactory-6.92.0/gdsfactory/components/spiral_double.py
+-rw-r--r--   0        0        0     5871 2023-05-09 00:30:20.320903 gdsfactory-6.92.0/gdsfactory/components/spiral_external_io.py
+-rw-r--r--   0        0        0    16658 2023-05-09 00:30:20.320903 gdsfactory-6.92.0/gdsfactory/components/spiral_heater.py
+-rw-r--r--   0        0        0     9181 2023-05-09 00:30:20.320903 gdsfactory-6.92.0/gdsfactory/components/spiral_inner_io.py
+-rw-r--r--   0        0        0     1754 2023-05-09 00:30:20.320903 gdsfactory-6.92.0/gdsfactory/components/splitter_chain.py
+-rw-r--r--   0        0        0     5327 2023-05-09 00:30:20.320903 gdsfactory-6.92.0/gdsfactory/components/splitter_tree.py
+-rw-r--r--   0        0        0     2526 2023-05-09 00:30:20.320903 gdsfactory-6.92.0/gdsfactory/components/straight.py
+-rw-r--r--   0        0        0     1033 2023-05-09 00:30:20.320903 gdsfactory-6.92.0/gdsfactory/components/straight_array.py
+-rw-r--r--   0        0        0     7914 2023-05-09 00:30:20.320903 gdsfactory-6.92.0/gdsfactory/components/straight_heater_doped_rib.py
+-rw-r--r--   0        0        0     1922 2023-05-09 00:30:20.320903 gdsfactory-6.92.0/gdsfactory/components/straight_heater_doped_strip.py
+-rw-r--r--   0        0        0     7891 2023-05-09 00:30:20.320903 gdsfactory-6.92.0/gdsfactory/components/straight_heater_meander.py
+-rw-r--r--   0        0        0     8090 2023-05-09 00:30:20.320903 gdsfactory-6.92.0/gdsfactory/components/straight_heater_meander_doped.py
+-rw-r--r--   0        0        0     5686 2023-05-09 00:30:20.320903 gdsfactory-6.92.0/gdsfactory/components/straight_heater_metal.py
+-rw-r--r--   0        0        0     2809 2023-05-09 00:30:20.320903 gdsfactory-6.92.0/gdsfactory/components/straight_pin.py
+-rw-r--r--   0        0        0     3974 2023-05-09 00:30:20.320903 gdsfactory-6.92.0/gdsfactory/components/straight_pin_slot.py
+-rw-r--r--   0        0        0      655 2023-05-09 00:30:20.320903 gdsfactory-6.92.0/gdsfactory/components/straight_rib.py
+-rw-r--r--   0        0        0      820 2023-05-09 00:30:20.320903 gdsfactory-6.92.0/gdsfactory/components/switch_tree.py
+-rw-r--r--   0        0        0     7713 2023-05-09 00:30:20.320903 gdsfactory-6.92.0/gdsfactory/components/taper.py
+-rw-r--r--   0        0        0     3530 2023-05-09 00:30:20.320903 gdsfactory-6.92.0/gdsfactory/components/taper_adiabatic.py
+-rw-r--r--   0        0        0     2457 2023-05-09 00:30:20.320903 gdsfactory-6.92.0/gdsfactory/components/taper_cross_section.py
+-rw-r--r--   0        0        0     2363 2023-05-09 00:30:20.320903 gdsfactory-6.92.0/gdsfactory/components/taper_from_csv.py
+-rw-r--r--   0        0        0     1215 2023-05-09 00:30:20.320903 gdsfactory-6.92.0/gdsfactory/components/taper_parabolic.py
+-rw-r--r--   0        0        0     1635 2023-05-09 00:30:20.320903 gdsfactory-6.92.0/gdsfactory/components/terminator.py
+-rw-r--r--   0        0        0     2913 2023-05-09 00:30:20.320903 gdsfactory-6.92.0/gdsfactory/components/text.py
+-rw-r--r--   0        0        0     3821 2023-05-09 00:30:20.320903 gdsfactory-6.92.0/gdsfactory/components/text_freetype.py
+-rw-r--r--   0        0        0     3156 2023-05-09 00:30:20.320903 gdsfactory-6.92.0/gdsfactory/components/text_rectangular.py
+-rw-r--r--   0        0        0     3943 2023-05-09 00:30:20.320903 gdsfactory-6.92.0/gdsfactory/components/text_rectangular_font.py
+-rw-r--r--   0        0        0     2536 2023-05-09 00:30:20.320903 gdsfactory-6.92.0/gdsfactory/components/triangles.py
+-rw-r--r--   0        0        0      715 2023-05-09 00:30:20.320903 gdsfactory-6.92.0/gdsfactory/components/verniers.py
+-rw-r--r--   0        0        0     2468 2023-05-09 00:30:20.320903 gdsfactory-6.92.0/gdsfactory/components/version_stamp.py
+-rw-r--r--   0        0        0     2436 2023-05-09 00:30:20.320903 gdsfactory-6.92.0/gdsfactory/components/via.py
+-rw-r--r--   0        0        0     3060 2023-05-09 00:30:20.320903 gdsfactory-6.92.0/gdsfactory/components/via_corner.py
+-rw-r--r--   0        0        0     5342 2023-05-09 00:30:20.320903 gdsfactory-6.92.0/gdsfactory/components/via_cutback.py
+-rw-r--r--   0        0        0    15574 2023-05-09 00:30:20.320903 gdsfactory-6.92.0/gdsfactory/components/via_stack.py
+-rw-r--r--   0        0        0     4554 2023-05-09 00:30:20.320903 gdsfactory-6.92.0/gdsfactory/components/via_stack_slot.py
+-rw-r--r--   0        0        0     4944 2023-05-09 00:30:20.320903 gdsfactory-6.92.0/gdsfactory/components/via_stack_with_offset.py
+-rw-r--r--   0        0        0     1088 2023-05-09 00:30:20.320903 gdsfactory-6.92.0/gdsfactory/components/wafer.py
+-rw-r--r--   0        0        0     2542 2023-05-09 00:30:20.320903 gdsfactory-6.92.0/gdsfactory/components/wire.py
+-rw-r--r--   0        0        0      978 2023-05-09 00:30:20.320903 gdsfactory-6.92.0/gdsfactory/components/wire_sbend.py
+-rw-r--r--   0        0        0     7919 2023-05-09 00:30:20.320903 gdsfactory-6.92.0/gdsfactory/config.py
+-rw-r--r--   0        0        0      481 2023-05-09 00:30:20.320903 gdsfactory-6.92.0/gdsfactory/conftest.py
+-rw-r--r--   0        0        0    38409 2023-05-09 00:30:20.320903 gdsfactory-6.92.0/gdsfactory/constants.py
+-rw-r--r--   0        0        0     1476 2023-05-09 00:30:20.320903 gdsfactory-6.92.0/gdsfactory/containers.py
+-rw-r--r--   0        0        0    82607 2023-05-09 00:30:20.324903 gdsfactory-6.92.0/gdsfactory/cross_section.py
+-rw-r--r--   0        0        0     2974 2023-05-09 00:30:20.324903 gdsfactory-6.92.0/gdsfactory/decorators.py
+-rw-r--r--   0        0        0     6884 2023-05-09 00:30:20.324903 gdsfactory-6.92.0/gdsfactory/difftest.py
+-rw-r--r--   0        0        0      988 2023-05-09 00:30:20.324903 gdsfactory-6.92.0/gdsfactory/events.py
+-rw-r--r--   0        0        0      204 2023-05-09 00:30:20.324903 gdsfactory-6.92.0/gdsfactory/export/__init__.py
+-rw-r--r--   0        0        0     3353 2023-05-09 00:30:20.324903 gdsfactory-6.92.0/gdsfactory/export/to_3d.py
+-rw-r--r--   0        0        0     1940 2023-05-09 00:30:20.324903 gdsfactory-6.92.0/gdsfactory/export/to_np.py
+-rw-r--r--   0        0        0     3058 2023-05-09 00:30:20.324903 gdsfactory-6.92.0/gdsfactory/export/to_stl.py
+-rw-r--r--   0        0        0     7438 2023-05-09 00:30:20.324903 gdsfactory-6.92.0/gdsfactory/export/write_gerbers.py
+-rw-r--r--   0        0        0     2968 2023-05-09 00:30:20.324903 gdsfactory-6.92.0/gdsfactory/filestorage.py
+-rw-r--r--   0        0        0    11802 2023-05-09 00:30:20.324903 gdsfactory-6.92.0/gdsfactory/fill.py
+-rw-r--r--   0        0        0     7799 2023-05-09 00:30:20.324903 gdsfactory-6.92.0/gdsfactory/font.py
+-rw-r--r--   0        0        0     8073 2023-05-09 00:30:20.324903 gdsfactory-6.92.0/gdsfactory/functions.py
+-rw-r--r--   0        0        0       20 2023-05-09 00:30:20.324903 gdsfactory-6.92.0/gdsfactory/gdsdiff/.gitattributes
+-rw-r--r--   0        0        0       83 2023-05-09 00:30:20.324903 gdsfactory-6.92.0/gdsfactory/gdsdiff/.gitconfig
+-rw-r--r--   0        0        0       72 2023-05-09 00:30:20.324903 gdsfactory-6.92.0/gdsfactory/gdsdiff/__init__.py
+-rw-r--r--   0        0        0     1069 2023-05-09 00:30:20.324903 gdsfactory-6.92.0/gdsfactory/gdsdiff/gds_diff_git.py
+-rw-r--r--   0        0        0     2935 2023-05-09 00:30:20.324903 gdsfactory-6.92.0/gdsfactory/gdsdiff/gdsdiff.py
+-rw-r--r--   0        0        0      708 2023-05-09 00:30:20.324903 gdsfactory-6.92.0/gdsfactory/gdsdiff/install.py
+-rw-r--r--   0        0        0      271 2023-05-09 00:30:20.324903 gdsfactory-6.92.0/gdsfactory/gdsdiff/sample.py
+-rw-r--r--   0        0        0     1059 2023-05-09 00:30:20.324903 gdsfactory-6.92.0/gdsfactory/gdsdiff/test_xor.py
+-rw-r--r--   0        0        0     1100 2023-05-09 00:30:20.324903 gdsfactory-6.92.0/gdsfactory/generic_tech/README.md
+-rw-r--r--   0        0        0     1722 2023-05-09 00:30:20.324903 gdsfactory-6.92.0/gdsfactory/generic_tech/__init__.py
+-rw-r--r--   0        0        0      169 2023-05-09 00:30:20.324903 gdsfactory-6.92.0/gdsfactory/generic_tech/generic_tech.sh
+-rw-r--r--   0        0        0     8142 2023-05-09 00:30:20.324903 gdsfactory-6.92.0/gdsfactory/generic_tech/get_klayout_pyxs.py
+-rw-r--r--   0        0        0       44 2023-05-09 00:30:20.324903 gdsfactory-6.92.0/gdsfactory/generic_tech/klayout/README.md
+-rw-r--r--   0        0        0      104 2023-05-09 00:30:20.324903 gdsfactory-6.92.0/gdsfactory/generic_tech/klayout/drc/Makefile
+-rw-r--r--   0        0        0        0 2023-05-09 00:30:20.324903 gdsfactory-6.92.0/gdsfactory/generic_tech/klayout/drc/__init__.py
+-rw-r--r--   0        0        0     2842 2023-05-09 00:30:20.324903 gdsfactory-6.92.0/gdsfactory/generic_tech/klayout/drc/errors.py
+-rw-r--r--   0        0        0      579 2023-05-09 00:30:20.324903 gdsfactory-6.92.0/gdsfactory/generic_tech/klayout/drc/generic.drc
+-rw-r--r--   0        0        0     2929 2023-05-09 00:30:20.324903 gdsfactory-6.92.0/gdsfactory/generic_tech/klayout/drc/generic.lydrc
+-rw-r--r--   0        0        0     1014 2023-05-09 00:30:20.324903 gdsfactory-6.92.0/gdsfactory/generic_tech/klayout/drc/write_drc.py
+-rw-r--r--   0        0        0     6193 2023-05-09 00:30:20.324903 gdsfactory-6.92.0/gdsfactory/generic_tech/klayout/grain.xml
+-rw-r--r--   0        0        0    10140 2023-05-09 00:30:20.324903 gdsfactory-6.92.0/gdsfactory/generic_tech/klayout/icon_128x128.png
+-rw-r--r--   0        0        0     4248 2023-05-09 00:30:20.324903 gdsfactory-6.92.0/gdsfactory/generic_tech/klayout/icon_64x64.png
+-rw-r--r--   0        0        0     3980 2023-05-09 00:30:20.324903 gdsfactory-6.92.0/gdsfactory/generic_tech/klayout/lvs/README.md
+-rw-r--r--   0        0        0     2419 2023-05-09 00:30:20.324903 gdsfactory-6.92.0/gdsfactory/generic_tech/klayout/lvs/drc_malformed/README.md
+-rw-r--r--   0        0        0     9696 2023-05-09 00:30:20.324903 gdsfactory-6.92.0/gdsfactory/generic_tech/klayout/lvs/drc_malformed/generic_tech_malformed.drc
+-rw-r--r--   0        0        0    12347 2023-05-09 00:30:20.324903 gdsfactory-6.92.0/gdsfactory/generic_tech/klayout/lvs/drc_malformed/run_drc.py
+-rw-r--r--   0        0        0     7540 2023-05-09 00:30:20.324903 gdsfactory-6.92.0/gdsfactory/generic_tech/klayout/lvs/generic_tech.lvs
+-rw-r--r--   0        0        0     3437 2023-05-09 00:30:20.324903 gdsfactory-6.92.0/gdsfactory/generic_tech/klayout/lvs/rule_decks/custom_classes.lvs
+-rw-r--r--   0        0        0      479 2023-05-09 00:30:20.324903 gdsfactory-6.92.0/gdsfactory/generic_tech/klayout/lvs/rule_decks/devices_connections.lvs
+-rw-r--r--   0        0        0      582 2023-05-09 00:30:20.324903 gdsfactory-6.92.0/gdsfactory/generic_tech/klayout/lvs/rule_decks/general_connections.lvs
+-rw-r--r--   0        0        0      108 2023-05-09 00:30:20.324903 gdsfactory-6.92.0/gdsfactory/generic_tech/klayout/lvs/rule_decks/general_derivations.lvs
+-rw-r--r--   0        0        0      186 2023-05-09 00:30:20.324903 gdsfactory-6.92.0/gdsfactory/generic_tech/klayout/lvs/rule_decks/heater_connections.lvs
+-rw-r--r--   0        0        0      398 2023-05-09 00:30:20.324903 gdsfactory-6.92.0/gdsfactory/generic_tech/klayout/lvs/rule_decks/heater_derivations.lvs
+-rw-r--r--   0        0        0      574 2023-05-09 00:30:20.324903 gdsfactory-6.92.0/gdsfactory/generic_tech/klayout/lvs/rule_decks/heater_extraction.lvs
+-rw-r--r--   0        0        0     6034 2023-05-09 00:30:20.324903 gdsfactory-6.92.0/gdsfactory/generic_tech/klayout/lvs/rule_decks/layers_definitions.lvs
+-rw-r--r--   0        0        0    12077 2023-05-09 00:30:20.324903 gdsfactory-6.92.0/gdsfactory/generic_tech/klayout/lvs/run_lvs.py
+-rw-r--r--   0        0        0      493 2023-05-09 00:30:20.324903 gdsfactory-6.92.0/gdsfactory/generic_tech/klayout/lvs/testing/testcases/README.md
+-rw-r--r--   0        0        0      531 2023-05-09 00:30:20.324903 gdsfactory-6.92.0/gdsfactory/generic_tech/klayout/lvs/testing/testcases/unit/heater_devices/netlist/straight_heater_metal.spice
+-rw-r--r--   0        0        0    10945 2023-05-09 00:30:20.324903 gdsfactory-6.92.0/gdsfactory/generic_tech/klayout/pymacros/import_generic_pcells.lym
+-rw-r--r--   0        0        0      710 2023-05-09 00:30:20.324903 gdsfactory-6.92.0/gdsfactory/generic_tech/klayout/pymacros/set_menus.lym
+-rw-r--r--   0        0        0      538 2023-05-09 00:30:20.324903 gdsfactory-6.92.0/gdsfactory/generic_tech/klayout/pymacros/set_shortcuts.lym
+-rw-r--r--   0        0        0        0 2023-05-09 00:30:20.324903 gdsfactory-6.92.0/gdsfactory/generic_tech/klayout/python/__init__.py
+-rw-r--r--   0        0        0      114 2023-05-09 00:30:20.324903 gdsfactory-6.92.0/gdsfactory/generic_tech/klayout/python/kgdsfactory/__init__.py
+-rw-r--r--   0        0        0     4303 2023-05-09 00:30:20.324903 gdsfactory-6.92.0/gdsfactory/generic_tech/klayout/python/kgdsfactory/shortcuts.py
+-rw-r--r--   0        0        0      269 2023-05-09 00:30:20.324903 gdsfactory-6.92.0/gdsfactory/generic_tech/klayout/tech/Makefile
+-rw-r--r--   0        0        0     1519 2023-05-09 00:30:20.324903 gdsfactory-6.92.0/gdsfactory/generic_tech/klayout/tech/generic.layerstack
+-rw-r--r--   0        0        0    40153 2023-05-09 00:30:20.324903 gdsfactory-6.92.0/gdsfactory/generic_tech/klayout/tech/generic_tech.lyp
+-rw-r--r--   0        0        0     7689 2023-05-09 00:30:20.324903 gdsfactory-6.92.0/gdsfactory/generic_tech/klayout/tech/generic_tech.lyt
+-rw-r--r--   0        0        0     4258 2023-05-09 00:30:20.324903 gdsfactory-6.92.0/gdsfactory/generic_tech/klayout/tech/xsection_generic.pyxs
+-rw-r--r--   0        0        0     4537 2023-05-09 00:30:20.324903 gdsfactory-6.92.0/gdsfactory/generic_tech/klayout/tech/xsection_generic.xs
+-rw-r--r--   0        0        0     4690 2023-05-09 00:30:20.324903 gdsfactory-6.92.0/gdsfactory/generic_tech/klayout/tech/xsection_planarized.pyxs
+-rw-r--r--   0        0        0     5508 2023-05-09 00:30:20.324903 gdsfactory-6.92.0/gdsfactory/generic_tech/klayout/tech/xsection_planarized.xs
+-rw-r--r--   0        0        0     1855 2023-05-09 00:30:20.324903 gdsfactory-6.92.0/gdsfactory/generic_tech/layer_map.py
+-rw-r--r--   0        0        0     6511 2023-05-09 00:30:20.324903 gdsfactory-6.92.0/gdsfactory/generic_tech/layer_stack.py
+-rw-r--r--   0        0        0    10547 2023-05-09 00:30:20.324903 gdsfactory-6.92.0/gdsfactory/generic_tech/layer_views.yaml
+-rw-r--r--   0        0        0      158 2023-05-09 00:30:20.324903 gdsfactory-6.92.0/gdsfactory/generic_tech/simulation_settings.py
+-rw-r--r--   0        0        0     1431 2023-05-09 00:30:20.324903 gdsfactory-6.92.0/gdsfactory/geometry/__init__.py
+-rw-r--r--   0        0        0     4917 2023-05-09 00:30:20.324903 gdsfactory-6.92.0/gdsfactory/geometry/boolean.py
+-rw-r--r--   0        0        0     3814 2023-05-09 00:30:20.324903 gdsfactory-6.92.0/gdsfactory/geometry/boolean_klayout.py
+-rw-r--r--   0        0        0     1904 2023-05-09 00:30:20.324903 gdsfactory-6.92.0/gdsfactory/geometry/boolean_polygons.py
+-rw-r--r--   0        0        0      598 2023-05-09 00:30:20.324903 gdsfactory-6.92.0/gdsfactory/geometry/check_duplicated_cells.py
+-rw-r--r--   0        0        0     2719 2023-05-09 00:30:20.324903 gdsfactory-6.92.0/gdsfactory/geometry/check_exclusion.py
+-rw-r--r--   0        0        0     2829 2023-05-09 00:30:20.324903 gdsfactory-6.92.0/gdsfactory/geometry/check_inclusion.py
+-rw-r--r--   0        0        0     3566 2023-05-09 00:30:20.324903 gdsfactory-6.92.0/gdsfactory/geometry/check_space.py
+-rw-r--r--   0        0        0     1904 2023-05-09 00:30:20.324903 gdsfactory-6.92.0/gdsfactory/geometry/check_width.py
+-rw-r--r--   0        0        0     5005 2023-05-09 00:30:20.324903 gdsfactory-6.92.0/gdsfactory/geometry/fill_klayout.py
+-rw-r--r--   0        0        0     7084 2023-05-09 00:30:20.324903 gdsfactory-6.92.0/gdsfactory/geometry/fill_tiled.py
+-rw-r--r--   0        0        0     1697 2023-05-09 00:30:20.324903 gdsfactory-6.92.0/gdsfactory/geometry/fillet.py
+-rw-r--r--   0        0        0     6664 2023-05-09 00:30:20.324903 gdsfactory-6.92.0/gdsfactory/geometry/functions.py
+-rw-r--r--   0        0        0     2167 2023-05-09 00:30:20.324903 gdsfactory-6.92.0/gdsfactory/geometry/invert.py
+-rw-r--r--   0        0        0     3685 2023-05-09 00:30:20.328903 gdsfactory-6.92.0/gdsfactory/geometry/layer_priority.py
+-rw-r--r--   0        0        0     3046 2023-05-09 00:30:20.328903 gdsfactory-6.92.0/gdsfactory/geometry/manhattanize.py
+-rw-r--r--   0        0        0     4192 2023-05-09 00:30:20.328903 gdsfactory-6.92.0/gdsfactory/geometry/maskprep.py
+-rw-r--r--   0        0        0     4744 2023-05-09 00:30:20.328903 gdsfactory-6.92.0/gdsfactory/geometry/maskprep_flat.py
+-rw-r--r--   0        0        0     3250 2023-05-09 00:30:20.328903 gdsfactory-6.92.0/gdsfactory/geometry/offset.py
+-rw-r--r--   0        0        0     3842 2023-05-09 00:30:20.328903 gdsfactory-6.92.0/gdsfactory/geometry/outline.py
+-rw-r--r--   0        0        0     2510 2023-05-09 00:30:20.328903 gdsfactory-6.92.0/gdsfactory/geometry/trim.py
+-rw-r--r--   0        0        0     2948 2023-05-09 00:30:20.328903 gdsfactory-6.92.0/gdsfactory/geometry/union.py
+-rw-r--r--   0        0        0     9629 2023-05-09 00:30:20.328903 gdsfactory-6.92.0/gdsfactory/geometry/write_drc.py
+-rw-r--r--   0        0        0     1783 2023-05-09 00:30:20.328903 gdsfactory-6.92.0/gdsfactory/geometry/xor_diff.py
+-rw-r--r--   0        0        0     1158 2023-05-09 00:30:20.328903 gdsfactory-6.92.0/gdsfactory/get_factories.py
+-rw-r--r--   0        0        0    23562 2023-05-09 00:30:20.328903 gdsfactory-6.92.0/gdsfactory/get_netlist.py
+-rw-r--r--   0        0        0    14426 2023-05-09 00:30:20.328903 gdsfactory-6.92.0/gdsfactory/get_netlist_flat.py
+-rw-r--r--   0        0        0      682 2023-05-09 00:30:20.328903 gdsfactory-6.92.0/gdsfactory/get_netlist_klayout.py
+-rw-r--r--   0        0        0     9455 2023-05-09 00:30:20.328903 gdsfactory-6.92.0/gdsfactory/grid.py
+-rw-r--r--   0        0        0     4363 2023-05-09 00:30:20.328903 gdsfactory-6.92.0/gdsfactory/install.py
+-rw-r--r--   0        0        0     1340 2023-05-09 00:30:20.328903 gdsfactory-6.92.0/gdsfactory/klive.py
+-rw-r--r--   0        0        0      585 2023-05-09 00:30:20.328903 gdsfactory-6.92.0/gdsfactory/labels/__init__.py
+-rw-r--r--   0        0        0     3563 2023-05-09 00:30:20.328903 gdsfactory-6.92.0/gdsfactory/labels/add_label_yaml.py
+-rw-r--r--   0        0        0     3847 2023-05-09 00:30:20.328903 gdsfactory-6.92.0/gdsfactory/labels/ehva.py
+-rw-r--r--   0        0        0     3810 2023-05-09 00:30:20.328903 gdsfactory-6.92.0/gdsfactory/labels/merge_test_metadata.py
+-rw-r--r--   0        0        0     4668 2023-05-09 00:30:20.328903 gdsfactory-6.92.0/gdsfactory/labels/siepic.py
+-rw-r--r--   0        0        0     4847 2023-05-09 00:30:20.328903 gdsfactory-6.92.0/gdsfactory/labels/write_labels.py
+-rw-r--r--   0        0        0     1149 2023-05-09 00:30:20.328903 gdsfactory-6.92.0/gdsfactory/materials.py
+-rw-r--r--   0        0        0     5247 2023-05-09 00:30:20.328903 gdsfactory-6.92.0/gdsfactory/name.py
+-rw-r--r--   0        0        0    11237 2023-05-09 00:30:20.328903 gdsfactory-6.92.0/gdsfactory/pack.py
+-rw-r--r--   0        0        0    50880 2023-05-09 00:30:20.328903 gdsfactory-6.92.0/gdsfactory/path.py
+-rw-r--r--   0        0        0    25849 2023-05-09 00:30:20.328903 gdsfactory-6.92.0/gdsfactory/pdk.py
+-rw-r--r--   0        0        0     6170 2023-05-09 00:30:20.328903 gdsfactory-6.92.0/gdsfactory/picmodel.py
+-rw-r--r--   0        0        0     5068 2023-05-09 00:30:20.328903 gdsfactory-6.92.0/gdsfactory/pixelate.py
+-rw-r--r--   0        0        0        0 2023-05-09 00:30:20.328903 gdsfactory-6.92.0/gdsfactory/plugins/dagster/__init__.py
+-rw-r--r--   0        0        0      976 2023-05-09 00:30:20.328903 gdsfactory-6.92.0/gdsfactory/plugins/dagster/workflow.py
+-rw-r--r--   0        0        0      566 2023-05-09 00:30:20.328903 gdsfactory-6.92.0/gdsfactory/plugins/database/README.md
+-rw-r--r--   0        0        0     1592 2023-05-09 00:30:20.328903 gdsfactory-6.92.0/gdsfactory/plugins/database/__init__.py
+-rw-r--r--   0        0        0     6216 2023-05-09 00:30:20.328903 gdsfactory-6.92.0/gdsfactory/plugins/database/db_upload.py
+-rw-r--r--   0        0        0    16143 2023-05-09 00:30:20.328903 gdsfactory-6.92.0/gdsfactory/plugins/database/models.py
+-rw-r--r--   0        0        0    32084 2023-05-09 00:30:20.328903 gdsfactory-6.92.0/gdsfactory/port.py
+-rw-r--r--   0        0        0    37609 2023-05-09 00:30:20.328903 gdsfactory-6.92.0/gdsfactory/quickplotter.py
+-rw-r--r--   0        0        0      696 2023-05-09 00:30:20.328903 gdsfactory-6.92.0/gdsfactory/read/__init__.py
+-rw-r--r--   0        0        0     1639 2023-05-09 00:30:20.328903 gdsfactory-6.92.0/gdsfactory/read/from_dphox.py
+-rw-r--r--   0        0        0     1285 2023-05-09 00:30:20.328903 gdsfactory-6.92.0/gdsfactory/read/from_gdspaths.py
+-rw-r--r--   0        0        0     1953 2023-05-09 00:30:20.328903 gdsfactory-6.92.0/gdsfactory/read/from_np.py
+-rw-r--r--   0        0        0     2813 2023-05-09 00:30:20.328903 gdsfactory-6.92.0/gdsfactory/read/from_phidl.py
+-rw-r--r--   0        0        0    38082 2023-05-09 00:30:20.328903 gdsfactory-6.92.0/gdsfactory/read/from_yaml.py
+-rw-r--r--   0        0        0     5897 2023-05-09 00:30:20.328903 gdsfactory-6.92.0/gdsfactory/read/from_yaml_template.py
+-rw-r--r--   0        0        0     5688 2023-05-09 00:30:20.328903 gdsfactory-6.92.0/gdsfactory/read/import_gds.py
+-rw-r--r--   0        0        0     3407 2023-05-09 00:30:20.328903 gdsfactory-6.92.0/gdsfactory/read/labels.py
+-rw-r--r--   0        0        0     3769 2023-05-09 00:30:20.328903 gdsfactory-6.92.0/gdsfactory/routing/__init__.py
+-rw-r--r--   0        0        0     2920 2023-05-09 00:30:20.328903 gdsfactory-6.92.0/gdsfactory/routing/add_electrical_pads_shortest.py
+-rw-r--r--   0        0        0     3015 2023-05-09 00:30:20.328903 gdsfactory-6.92.0/gdsfactory/routing/add_electrical_pads_top.py
+-rw-r--r--   0        0        0     3035 2023-05-09 00:30:20.328903 gdsfactory-6.92.0/gdsfactory/routing/add_electrical_pads_top_dc.py
+-rw-r--r--   0        0        0     8715 2023-05-09 00:30:20.328903 gdsfactory-6.92.0/gdsfactory/routing/add_fiber_array.py
+-rw-r--r--   0        0        0    10624 2023-05-09 00:30:20.328903 gdsfactory-6.92.0/gdsfactory/routing/add_fiber_single.py
+-rw-r--r--   0        0        0     8967 2023-05-09 00:30:20.328903 gdsfactory-6.92.0/gdsfactory/routing/add_pads.py
+-rw-r--r--   0        0        0    38940 2023-05-09 00:30:20.328903 gdsfactory-6.92.0/gdsfactory/routing/all_angle.py
+-rw-r--r--   0        0        0     3916 2023-05-09 00:30:20.328903 gdsfactory-6.92.0/gdsfactory/routing/auto_taper.py
+-rw-r--r--   0        0        0      982 2023-05-09 00:30:20.328903 gdsfactory-6.92.0/gdsfactory/routing/factories.py
+-rw-r--r--   0        0        0     4415 2023-05-09 00:30:20.328903 gdsfactory-6.92.0/gdsfactory/routing/fanout.py
+-rw-r--r--   0        0        0     2800 2023-05-09 00:30:20.328903 gdsfactory-6.92.0/gdsfactory/routing/fanout2x2.py
+-rw-r--r--   0        0        0    24342 2023-05-09 00:30:20.328903 gdsfactory-6.92.0/gdsfactory/routing/get_bundle.py
+-rw-r--r--   0        0        0     8632 2023-05-09 00:30:20.328903 gdsfactory-6.92.0/gdsfactory/routing/get_bundle_corner.py
+-rw-r--r--   0        0        0     6900 2023-05-09 00:30:20.328903 gdsfactory-6.92.0/gdsfactory/routing/get_bundle_from_steps.py
+-rw-r--r--   0        0        0    12949 2023-05-09 00:30:20.328903 gdsfactory-6.92.0/gdsfactory/routing/get_bundle_from_waypoints.py
+-rw-r--r--   0        0        0     5284 2023-05-09 00:30:20.332903 gdsfactory-6.92.0/gdsfactory/routing/get_bundle_path_length_match.py
+-rw-r--r--   0        0        0     1937 2023-05-09 00:30:20.332903 gdsfactory-6.92.0/gdsfactory/routing/get_bundle_sbend.py
+-rw-r--r--   0        0        0    17064 2023-05-09 00:30:20.332903 gdsfactory-6.92.0/gdsfactory/routing/get_bundle_u.py
+-rw-r--r--   0        0        0     1510 2023-05-09 00:30:20.332903 gdsfactory-6.92.0/gdsfactory/routing/get_input_labels.py
+-rw-r--r--   0        0        0     9233 2023-05-09 00:30:20.332903 gdsfactory-6.92.0/gdsfactory/routing/get_route.py
+-rw-r--r--   0        0        0    10824 2023-05-09 00:30:20.332903 gdsfactory-6.92.0/gdsfactory/routing/get_route_astar.py
+-rw-r--r--   0        0        0     6119 2023-05-09 00:30:20.332903 gdsfactory-6.92.0/gdsfactory/routing/get_route_from_steps.py
+-rw-r--r--   0        0        0     2766 2023-05-09 00:30:20.332903 gdsfactory-6.92.0/gdsfactory/routing/get_route_sbend.py
+-rw-r--r--   0        0        0     3311 2023-05-09 00:30:20.332903 gdsfactory-6.92.0/gdsfactory/routing/get_routes_bend180.py
+-rw-r--r--   0        0        0     1854 2023-05-09 00:30:20.332903 gdsfactory-6.92.0/gdsfactory/routing/get_routes_straight.py
+-rw-r--r--   0        0        0    34394 2023-05-09 00:30:20.332903 gdsfactory-6.92.0/gdsfactory/routing/manhattan.py
+-rw-r--r--   0        0        0    10081 2023-05-09 00:30:20.332903 gdsfactory-6.92.0/gdsfactory/routing/path_length_matching.py
+-rw-r--r--   0        0        0    22568 2023-05-09 00:30:20.332903 gdsfactory-6.92.0/gdsfactory/routing/route_fiber_array.py
+-rw-r--r--   0        0        0     8679 2023-05-09 00:30:20.332903 gdsfactory-6.92.0/gdsfactory/routing/route_fiber_single.py
+-rw-r--r--   0        0        0    18132 2023-05-09 00:30:20.332903 gdsfactory-6.92.0/gdsfactory/routing/route_ports_to_side.py
+-rw-r--r--   0        0        0     4361 2023-05-09 00:30:20.332903 gdsfactory-6.92.0/gdsfactory/routing/route_quad.py
+-rw-r--r--   0        0        0    14370 2023-05-09 00:30:20.332903 gdsfactory-6.92.0/gdsfactory/routing/route_sharp.py
+-rw-r--r--   0        0        0    10167 2023-05-09 00:30:20.332903 gdsfactory-6.92.0/gdsfactory/routing/route_south.py
+-rw-r--r--   0        0        0     5072 2023-05-09 00:30:20.332903 gdsfactory-6.92.0/gdsfactory/routing/sort_ports.py
+-rw-r--r--   0        0        0     2477 2023-05-09 00:30:20.332903 gdsfactory-6.92.0/gdsfactory/routing/utils.py
+-rw-r--r--   0        0        0     2889 2023-05-09 00:30:20.332903 gdsfactory-6.92.0/gdsfactory/samples/01_component_pcell.py
+-rw-r--r--   0        0        0      646 2023-05-09 00:30:20.332903 gdsfactory-6.92.0/gdsfactory/samples/01_component_pcell/test_straight_wide.yml
+-rw-r--r--   0        0        0     1101 2023-05-09 00:30:20.332903 gdsfactory-6.92.0/gdsfactory/samples/01_component_pcell_with_pins.py
+-rw-r--r--   0        0        0      664 2023-05-09 00:30:20.332903 gdsfactory-6.92.0/gdsfactory/samples/01_component_pcell_with_pins/test_straight_narrow.yml
+-rw-r--r--   0        0        0      347 2023-05-09 00:30:20.332903 gdsfactory-6.92.0/gdsfactory/samples/02_component_autoname.py
+-rw-r--r--   0        0        0      887 2023-05-09 00:30:20.332903 gdsfactory-6.92.0/gdsfactory/samples/03_move.py
+-rw-r--r--   0        0        0      881 2023-05-09 00:30:20.332903 gdsfactory-6.92.0/gdsfactory/samples/04_connect.py
+-rw-r--r--   0        0        0      710 2023-05-09 00:30:20.332903 gdsfactory-6.92.0/gdsfactory/samples/05_remove_layers.py
+-rw-r--r--   0        0        0      931 2023-05-09 00:30:20.332903 gdsfactory-6.92.0/gdsfactory/samples/06_remapping_layers.py
+-rw-r--r--   0        0        0     1082 2023-05-09 00:30:20.332903 gdsfactory-6.92.0/gdsfactory/samples/07_flattening_device.py
+-rw-r--r--   0        0        0      475 2023-05-09 00:30:20.332903 gdsfactory-6.92.0/gdsfactory/samples/08_group.py
+-rw-r--r--   0        0        0     1631 2023-05-09 00:30:20.332903 gdsfactory-6.92.0/gdsfactory/samples/11_component_layout.py
+-rw-r--r--   0        0        0     2245 2023-05-09 00:30:20.332903 gdsfactory-6.92.0/gdsfactory/samples/12_component_refs.py
+-rw-r--r--   0        0        0      955 2023-05-09 00:30:20.332903 gdsfactory-6.92.0/gdsfactory/samples/13_component_netlist.py
+-rw-r--r--   0        0        0     2592 2023-05-09 00:30:20.332903 gdsfactory-6.92.0/gdsfactory/samples/14_component_connectivity.py
+-rw-r--r--   0        0        0     1636 2023-05-09 00:30:20.332903 gdsfactory-6.92.0/gdsfactory/samples/15_component_sequence1.py
+-rw-r--r--   0        0        0     1680 2023-05-09 00:30:20.332903 gdsfactory-6.92.0/gdsfactory/samples/16_component_sequence2.py
+-rw-r--r--   0        0        0      965 2023-05-09 00:30:20.332903 gdsfactory-6.92.0/gdsfactory/samples/17_ports.py
+-rw-r--r--   0        0        0      489 2023-05-09 00:30:20.332903 gdsfactory-6.92.0/gdsfactory/samples/18_port_markers.py
+-rw-r--r--   0        0        0      361 2023-05-09 00:30:20.332903 gdsfactory-6.92.0/gdsfactory/samples/19_references.py
+-rw-r--r--   0        0        0      533 2023-05-09 00:30:20.332903 gdsfactory-6.92.0/gdsfactory/samples/20_components.py
+-rw-r--r--   0        0        0      507 2023-05-09 00:30:20.332903 gdsfactory-6.92.0/gdsfactory/samples/21_add_fiber_array.py
+-rw-r--r--   0        0        0      493 2023-05-09 00:30:20.332903 gdsfactory-6.92.0/gdsfactory/samples/22_add_fiber_single.py
+-rw-r--r--   0        0        0      569 2023-05-09 00:30:20.332903 gdsfactory-6.92.0/gdsfactory/samples/22_add_pads.py
+-rw-r--r--   0        0        0      848 2023-05-09 00:30:20.332903 gdsfactory-6.92.0/gdsfactory/samples/23_reticle.py
+-rw-r--r--   0        0        0     1588 2023-05-09 00:30:20.332903 gdsfactory-6.92.0/gdsfactory/samples/23_reticle_passives.py
+-rw-r--r--   0        0        0      457 2023-05-09 00:30:20.332903 gdsfactory-6.92.0/gdsfactory/samples/24_doe.py
+-rw-r--r--   0        0        0      687 2023-05-09 00:30:20.332903 gdsfactory-6.92.0/gdsfactory/samples/24_doe_2.py
+-rw-r--r--   0        0        0      692 2023-05-09 00:30:20.332903 gdsfactory-6.92.0/gdsfactory/samples/24_doe_3.py
+-rw-r--r--   0        0        0      306 2023-05-09 00:30:20.332903 gdsfactory-6.92.0/gdsfactory/samples/25_slot_cross_section.py
+-rw-r--r--   0        0        0     1363 2023-05-09 00:30:20.332903 gdsfactory-6.92.0/gdsfactory/samples/30_lidar.py
+-rw-r--r--   0        0        0     1412 2023-05-09 00:30:20.332903 gdsfactory-6.92.0/gdsfactory/samples/30_lidar_pcell.py
+-rw-r--r--   0        0        0     1943 2023-05-09 00:30:20.332903 gdsfactory-6.92.0/gdsfactory/samples/30_lidar_with_pads.py
+-rw-r--r--   0        0        0        0 2023-05-09 00:30:20.332903 gdsfactory-6.92.0/gdsfactory/samples/__init__.py
+-rw-r--r--   0        0        0     1307 2023-05-09 00:30:20.332903 gdsfactory-6.92.0/gdsfactory/samples/all_angle_routing.py
+-rw-r--r--   0        0        0      558 2023-05-09 00:30:20.332903 gdsfactory-6.92.0/gdsfactory/samples/all_angle_routing/aar_basic_01.pic.yml
+-rw-r--r--   0        0        0     6062 2023-05-09 00:30:20.332903 gdsfactory-6.92.0/gdsfactory/samples/all_angle_routing/aar_bundles.pic.yml
+-rw-r--r--   0        0        0      444 2023-05-09 00:30:20.332903 gdsfactory-6.92.0/gdsfactory/samples/all_angle_routing/aar_error_intermediate_180.pic.yml
+-rw-r--r--   0        0        0      463 2023-05-09 00:30:20.332903 gdsfactory-6.92.0/gdsfactory/samples/all_angle_routing/aar_error_overconstrained.pic.yml
+-rw-r--r--   0        0        0     1552 2023-05-09 00:30:20.332903 gdsfactory-6.92.0/gdsfactory/samples/all_angle_routing/aar_gone_wrong.pic.yml
+-rw-r--r--   0        0        0     1315 2023-05-09 00:30:20.332903 gdsfactory-6.92.0/gdsfactory/samples/all_angle_routing/aar_implicit_final_angle.pic.yml
+-rw-r--r--   0        0        0      602 2023-05-09 00:30:20.332903 gdsfactory-6.92.0/gdsfactory/samples/all_angle_routing/aar_slalom.pic.yml
+-rw-r--r--   0        0        0     3317 2023-05-09 00:30:20.332903 gdsfactory-6.92.0/gdsfactory/samples/all_angle_routing/aar_start_end_customizations.pic.yml
+-rw-r--r--   0        0        0     1484 2023-05-09 00:30:20.332903 gdsfactory-6.92.0/gdsfactory/samples/all_angle_routing/aar_step_definitions.pic.yml
+-rw-r--r--   0        0        0     3045 2023-05-09 00:30:20.332903 gdsfactory-6.92.0/gdsfactory/samples/all_angle_routing/aar_tricky_connections.pic.yml
+-rw-r--r--   0        0        0     3782 2023-05-09 00:30:20.332903 gdsfactory-6.92.0/gdsfactory/samples/all_angle_routing/all_angle_routes.pic.yml
+-rw-r--r--   0        0        0     1988 2023-05-09 00:30:20.332903 gdsfactory-6.92.0/gdsfactory/samples/big_device.py
+-rw-r--r--   0        0        0       19 2023-05-09 00:30:20.332903 gdsfactory-6.92.0/gdsfactory/samples/demo/Makefile
+-rw-r--r--   0        0        0        0 2023-05-09 00:30:20.332903 gdsfactory-6.92.0/gdsfactory/samples/demo/__init__.py
+-rw-r--r--   0        0        0     1129 2023-05-09 00:30:20.332903 gdsfactory-6.92.0/gdsfactory/samples/demo/benchmark/fill_demo.py
+-rw-r--r--   0        0        0      343 2023-05-09 00:30:20.332903 gdsfactory-6.92.0/gdsfactory/samples/demo/benchmark/snap_demo_phidl.py
+-rw-r--r--   0        0        0      637 2023-05-09 00:30:20.332903 gdsfactory-6.92.0/gdsfactory/samples/demo/circuits/mask.pic.yml
+-rw-r--r--   0        0        0      622 2023-05-09 00:30:20.332903 gdsfactory-6.92.0/gdsfactory/samples/demo/circuits/mzi_lattice_filter.pic.yml
+-rw-r--r--   0        0        0      569 2023-05-09 00:30:20.332903 gdsfactory-6.92.0/gdsfactory/samples/demo/circuits/mzi_ubcpdk.pic.yml
+-rw-r--r--   0        0        0      453 2023-05-09 00:30:20.332903 gdsfactory-6.92.0/gdsfactory/samples/demo/circuits/pads.pic.yml
+-rw-r--r--   0        0        0      287 2023-05-09 00:30:20.332903 gdsfactory-6.92.0/gdsfactory/samples/demo/circuits/rectangles.pic.yml
+-rw-r--r--   0        0        0     2260 2023-05-09 00:30:20.332903 gdsfactory-6.92.0/gdsfactory/samples/demo/drc_errors.py
+-rw-r--r--   0        0        0     1014 2023-05-09 00:30:20.332903 gdsfactory-6.92.0/gdsfactory/samples/demo/drc_write.py
+-rw-r--r--   0        0        0     4530 2023-05-09 00:30:20.332903 gdsfactory-6.92.0/gdsfactory/samples/demo/layers.py
+-rw-r--r--   0        0        0      158 2023-05-09 00:30:20.332903 gdsfactory-6.92.0/gdsfactory/samples/demo/layers_sky130.py
+-rw-r--r--   0        0        0      364 2023-05-09 00:30:20.332903 gdsfactory-6.92.0/gdsfactory/samples/demo/layers_xsection.py
+-rw-r--r--   0        0        0      708 2023-05-09 00:30:20.332903 gdsfactory-6.92.0/gdsfactory/samples/demo/lvs.py
+-rw-r--r--   0        0        0      574 2023-05-09 00:30:20.332903 gdsfactory-6.92.0/gdsfactory/samples/demo/pcell.py
+-rw-r--r--   0        0        0     4174 2023-05-09 00:30:20.332903 gdsfactory-6.92.0/gdsfactory/samples/netlists/mzi.yml
+-rw-r--r--   0        0        0     5840 2023-05-09 00:30:20.332903 gdsfactory-6.92.0/gdsfactory/samples/netlists/mzi_full.yml
+-rw-r--r--   0        0        0        0 2023-05-09 00:30:20.332903 gdsfactory-6.92.0/gdsfactory/samples/pdk/__init__.py
+-rw-r--r--   0        0        0     4235 2023-05-09 00:30:20.332903 gdsfactory-6.92.0/gdsfactory/samples/pdk/fab_c.py
+-rw-r--r--   0        0        0      475 2023-05-09 00:30:20.332903 gdsfactory-6.92.0/gdsfactory/samples/pdk/fab_d/__init__.py
+-rw-r--r--   0        0        0     1880 2023-05-09 00:30:20.332903 gdsfactory-6.92.0/gdsfactory/samples/pdk/fab_d/phase_shifters.py
+-rw-r--r--   0        0        0     1715 2023-05-09 00:30:20.332903 gdsfactory-6.92.0/gdsfactory/samples/pdk/test_fab_c.py
+-rw-r--r--   0        0        0       50 2023-05-09 00:30:20.332903 gdsfactory-6.92.0/gdsfactory/samples/pdk/test_fab_c/test_ports_bend_euler_c_.csv
+-rw-r--r--   0        0        0       93 2023-05-09 00:30:20.332903 gdsfactory-6.92.0/gdsfactory/samples/pdk/test_fab_c/test_ports_gc_nitride_c_.csv
+-rw-r--r--   0        0        0       85 2023-05-09 00:30:20.332903 gdsfactory-6.92.0/gdsfactory/samples/pdk/test_fab_c/test_ports_mmi1x2_nitride_c_.csv
+-rw-r--r--   0        0        0      139 2023-05-09 00:30:20.332903 gdsfactory-6.92.0/gdsfactory/samples/pdk/test_fab_c/test_ports_mmi1x2_nitride_o_.csv
+-rw-r--r--   0        0        0       90 2023-05-09 00:30:20.332903 gdsfactory-6.92.0/gdsfactory/samples/pdk/test_fab_c/test_ports_mzi_nitride_c_.csv
+-rw-r--r--   0        0        0      126 2023-05-09 00:30:20.332903 gdsfactory-6.92.0/gdsfactory/samples/pdk/test_fab_c/test_ports_mzi_nitride_o_.csv
+-rw-r--r--   0        0        0       48 2023-05-09 00:30:20.332903 gdsfactory-6.92.0/gdsfactory/samples/pdk/test_fab_c/test_ports_straight_c_.csv
+-rw-r--r--   0        0        0     1023 2023-05-09 00:30:20.332903 gdsfactory-6.92.0/gdsfactory/samples/pdk/test_fab_c/test_settings_bend_euler_c_.yml
+-rw-r--r--   0        0        0     2100 2023-05-09 00:30:20.332903 gdsfactory-6.92.0/gdsfactory/samples/pdk/test_fab_c/test_settings_bend_euler_nc_.yml
+-rw-r--r--   0        0        0     1839 2023-05-09 00:30:20.332903 gdsfactory-6.92.0/gdsfactory/samples/pdk/test_fab_c/test_settings_gc_nc_.yml
+-rw-r--r--   0        0        0     1267 2023-05-09 00:30:20.332903 gdsfactory-6.92.0/gdsfactory/samples/pdk/test_fab_c/test_settings_gc_nitride_c_.yml
+-rw-r--r--   0        0        0     1592 2023-05-09 00:30:20.332903 gdsfactory-6.92.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mmi1x2_nc_.yml
+-rw-r--r--   0        0        0     1061 2023-05-09 00:30:20.336903 gdsfactory-6.92.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mmi1x2_nitride_c_.yml
+-rw-r--r--   0        0        0     1054 2023-05-09 00:30:20.336903 gdsfactory-6.92.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mmi1x2_nitride_o_.yml
+-rw-r--r--   0        0        0     1577 2023-05-09 00:30:20.336903 gdsfactory-6.92.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mmi1x2_no_.yml
+-rw-r--r--   0        0        0     4313 2023-05-09 00:30:20.336903 gdsfactory-6.92.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mzi_nc_.yml
+-rw-r--r--   0        0        0     3625 2023-05-09 00:30:20.336903 gdsfactory-6.92.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mzi_nitride_c_.yml
+-rw-r--r--   0        0        0     3603 2023-05-09 00:30:20.336903 gdsfactory-6.92.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mzi_nitride_o_.yml
+-rw-r--r--   0        0        0     4271 2023-05-09 00:30:20.336903 gdsfactory-6.92.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mzi_no_.yml
+-rw-r--r--   0        0        0      840 2023-05-09 00:30:20.336903 gdsfactory-6.92.0/gdsfactory/samples/pdk/test_fab_c/test_settings_straight_c_.yml
+-rw-r--r--   0        0        0     2171 2023-05-09 00:30:20.336903 gdsfactory-6.92.0/gdsfactory/samples/pdk/test_fab_c/test_settings_straight_nc_.yml
+-rw-r--r--   0        0        0      316 2023-05-09 00:30:20.336903 gdsfactory-6.92.0/gdsfactory/schematic.py
+-rw-r--r--   0        0        0    17692 2023-05-09 00:30:20.336903 gdsfactory-6.92.0/gdsfactory/schematic_editor.py
+-rw-r--r--   0        0        0     4194 2023-05-09 00:30:20.336903 gdsfactory-6.92.0/gdsfactory/serialization.py
+-rw-r--r--   0        0        0     1612 2023-05-09 00:30:20.336903 gdsfactory-6.92.0/gdsfactory/show.py
+-rw-r--r--   0        0        0      724 2023-05-09 00:30:20.336903 gdsfactory-6.92.0/gdsfactory/simulation/__init__.py
+-rw-r--r--   0        0        0     4369 2023-05-09 00:30:20.336903 gdsfactory-6.92.0/gdsfactory/simulation/add_simulation_markers.py
+-rw-r--r--   0        0        0     2476 2023-05-09 00:30:20.336903 gdsfactory-6.92.0/gdsfactory/simulation/convert_sparameters.py
+-rw-r--r--   0        0        0      547 2023-05-09 00:30:20.336903 gdsfactory-6.92.0/gdsfactory/simulation/devsim/__init__.py
+-rw-r--r--   0        0        0     2559 2023-05-09 00:30:20.336903 gdsfactory-6.92.0/gdsfactory/simulation/devsim/doping.py
+-rw-r--r--   0        0        0    11977 2023-05-09 00:30:20.336903 gdsfactory-6.92.0/gdsfactory/simulation/devsim/get_simulation.py
+-rw-r--r--   0        0        0    23601 2023-05-09 00:30:20.336903 gdsfactory-6.92.0/gdsfactory/simulation/devsim/get_simulation_xsection.py
+-rw-r--r--   0        0        0    19708 2023-05-09 00:30:20.336903 gdsfactory-6.92.0/gdsfactory/simulation/devsim/get_solver.py
+-rw-r--r--   0        0        0     1632 2023-05-09 00:30:20.336903 gdsfactory-6.92.0/gdsfactory/simulation/devsim/test_devsim.py
+-rw-r--r--   0        0        0      189 2023-05-09 00:30:20.336903 gdsfactory-6.92.0/gdsfactory/simulation/disable_print.py
+-rw-r--r--   0        0        0       79 2023-05-09 00:30:20.336903 gdsfactory-6.92.0/gdsfactory/simulation/eme/__init__.py
+-rw-r--r--   0        0        0    14784 2023-05-09 00:30:20.336903 gdsfactory-6.92.0/gdsfactory/simulation/eme/meow_eme.py
+-rw-r--r--   0        0        0     1771 2023-05-09 00:30:20.336903 gdsfactory-6.92.0/gdsfactory/simulation/eme/test_meow_simulation.py
+-rw-r--r--   0        0        0        0 2023-05-09 00:30:20.336903 gdsfactory-6.92.0/gdsfactory/simulation/fem/__init__.py
+-rw-r--r--   0        0        0     8968 2023-05-09 00:30:20.336903 gdsfactory-6.92.0/gdsfactory/simulation/fem/mode_solver.py
+-rw-r--r--   0        0        0     2205 2023-05-09 00:30:20.336903 gdsfactory-6.92.0/gdsfactory/simulation/fem/test_mode_solver.py
+-rw-r--r--   0        0        0     3351 2023-05-09 00:30:20.336903 gdsfactory-6.92.0/gdsfactory/simulation/get_effective_indices.py
+-rw-r--r--   0        0        0     3109 2023-05-09 00:30:20.336903 gdsfactory-6.92.0/gdsfactory/simulation/get_modes_path.py
+-rw-r--r--   0        0        0     3888 2023-05-09 00:30:20.336903 gdsfactory-6.92.0/gdsfactory/simulation/get_sparameters_path.py
+-rw-r--r--   0        0        0     1863 2023-05-09 00:30:20.336903 gdsfactory-6.92.0/gdsfactory/simulation/gmeep/__init__.py
+-rw-r--r--   0        0        0     3194 2023-05-09 00:30:20.336903 gdsfactory-6.92.0/gdsfactory/simulation/gmeep/get_material.py
+-rw-r--r--   0        0        0     6137 2023-05-09 00:30:20.336903 gdsfactory-6.92.0/gdsfactory/simulation/gmeep/get_meep_geometry.py
+-rw-r--r--   0        0        0     6054 2023-05-09 00:30:20.336903 gdsfactory-6.92.0/gdsfactory/simulation/gmeep/get_port_eigenmode.py
+-rw-r--r--   0        0        0    11014 2023-05-09 00:30:20.336903 gdsfactory-6.92.0/gdsfactory/simulation/gmeep/get_simulation.py
+-rw-r--r--   0        0        0    15701 2023-05-09 00:30:20.336903 gdsfactory-6.92.0/gdsfactory/simulation/gmeep/get_simulation_grating_farfield.py
+-rw-r--r--   0        0        0    17944 2023-05-09 00:30:20.336903 gdsfactory-6.92.0/gdsfactory/simulation/gmeep/get_simulation_grating_fiber.py
+-rw-r--r--   0        0        0    12302 2023-05-09 00:30:20.336903 gdsfactory-6.92.0/gdsfactory/simulation/gmeep/meep_adjoint_optimization.py
+-rw-r--r--   0        0        0    11914 2023-05-09 00:30:20.336903 gdsfactory-6.92.0/gdsfactory/simulation/gmeep/test_eigenmode.py
+-rw-r--r--   0        0        0      832 2023-05-09 00:30:20.336903 gdsfactory-6.92.0/gdsfactory/simulation/gmeep/test_materials.py
+-rw-r--r--   0        0        0    10128 2023-05-09 00:30:20.336903 gdsfactory-6.92.0/gdsfactory/simulation/gmeep/test_sparameterNxN/test_sparameterNxN_crossing.csv
+-rw-r--r--   0        0        0    10128 2023-05-09 00:30:20.336903 gdsfactory-6.92.0/gdsfactory/simulation/gmeep/test_sparameterNxN/test_sparameterNxN_straight.csv
+-rw-r--r--   0        0        0     6642 2023-05-09 00:30:20.336903 gdsfactory-6.92.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep.py
+-rw-r--r--   0        0        0    10128 2023-05-09 00:30:20.336903 gdsfactory-6.92.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameterNxN_crossing.csv
+-rw-r--r--   0        0        0    10128 2023-05-09 00:30:20.336903 gdsfactory-6.92.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameterNxN_straight.csv
+-rw-r--r--   0        0        0    10093 2023-05-09 00:30:20.336903 gdsfactory-6.92.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameterNxN_symmetries_straight.csv
+-rw-r--r--   0        0        0    10085 2023-05-09 00:30:20.336903 gdsfactory-6.92.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameter_straight_mpi.csv
+-rw-r--r--   0        0        0    10085 2023-05-09 00:30:20.336903 gdsfactory-6.92.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameter_straight_mpi_pool.csv
+-rw-r--r--   0        0        0    34701 2023-05-09 00:30:20.336903 gdsfactory-6.92.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameters_crossing_symmetric.csv
+-rw-r--r--   0        0        0    10123 2023-05-09 00:30:20.336903 gdsfactory-6.92.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameters_straight.csv
+-rw-r--r--   0        0        0     9966 2023-05-09 00:30:20.336903 gdsfactory-6.92.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameters_straight_batch.csv
+-rw-r--r--   0        0        0     9966 2023-05-09 00:30:20.336903 gdsfactory-6.92.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameters_straight_mpi.csv
+-rw-r--r--   0        0        0    10085 2023-05-09 00:30:20.336903 gdsfactory-6.92.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameters_straight_mpi_pool.csv
+-rw-r--r--   0        0        0    10129 2023-05-09 00:30:20.336903 gdsfactory-6.92.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameters_straight_symmetric.csv
+-rw-r--r--   0        0        0    13951 2023-05-09 00:30:20.336903 gdsfactory-6.92.0/gdsfactory/simulation/gmeep/write_sparameters_grating.py
+-rw-r--r--   0        0        0    21273 2023-05-09 00:30:20.336903 gdsfactory-6.92.0/gdsfactory/simulation/gmeep/write_sparameters_meep.py
+-rw-r--r--   0        0        0     8135 2023-05-09 00:30:20.336903 gdsfactory-6.92.0/gdsfactory/simulation/gmeep/write_sparameters_meep_batch.py
+-rw-r--r--   0        0        0     9561 2023-05-09 00:30:20.336903 gdsfactory-6.92.0/gdsfactory/simulation/gmeep/write_sparameters_meep_mpi.py
+-rw-r--r--   0        0        0     1246 2023-05-09 00:30:20.336903 gdsfactory-6.92.0/gdsfactory/simulation/gmsh/__init__.py
+-rw-r--r--   0        0        0     6653 2023-05-09 00:30:20.336903 gdsfactory-6.92.0/gdsfactory/simulation/gmsh/break_geometry.py
+-rw-r--r--   0        0        0    11250 2023-05-09 00:30:20.340903 gdsfactory-6.92.0/gdsfactory/simulation/gmsh/mesh.py
+-rw-r--r--   0        0        0    11808 2023-05-09 00:30:20.340903 gdsfactory-6.92.0/gdsfactory/simulation/gmsh/meshtracker.py
+-rw-r--r--   0        0        0     7752 2023-05-09 00:30:20.340903 gdsfactory-6.92.0/gdsfactory/simulation/gmsh/parse_component.py
+-rw-r--r--   0        0        0     3644 2023-05-09 00:30:20.340903 gdsfactory-6.92.0/gdsfactory/simulation/gmsh/parse_gds.py
+-rw-r--r--   0        0        0     3605 2023-05-09 00:30:20.340903 gdsfactory-6.92.0/gdsfactory/simulation/gmsh/parse_layerstack.py
+-rw-r--r--   0        0        0     2990 2023-05-09 00:30:20.340903 gdsfactory-6.92.0/gdsfactory/simulation/gmsh/refine.py
+-rw-r--r--   0        0        0    10851 2023-05-09 00:30:20.340903 gdsfactory-6.92.0/gdsfactory/simulation/gmsh/scratch/mesh3D.py
+-rw-r--r--   0        0        0     2489 2023-05-09 00:30:20.340903 gdsfactory-6.92.0/gdsfactory/simulation/gmsh/tests/test_meshing.py
+-rw-r--r--   0        0        0    14168 2023-05-09 00:30:20.340903 gdsfactory-6.92.0/gdsfactory/simulation/gmsh/uz_xsection_mesh.py
+-rw-r--r--   0        0        0     7441 2023-05-09 00:30:20.340903 gdsfactory-6.92.0/gdsfactory/simulation/gmsh/xy_xsection_mesh.py
+-rw-r--r--   0        0        0    16326 2023-05-09 00:30:20.340903 gdsfactory-6.92.0/gdsfactory/simulation/gmsh/xyz_mesh.py
+-rw-r--r--   0        0        0     1524 2023-05-09 00:30:20.340903 gdsfactory-6.92.0/gdsfactory/simulation/gtidy3d/__init__.py
+-rw-r--r--   0        0        0     4368 2023-05-09 00:30:20.340903 gdsfactory-6.92.0/gdsfactory/simulation/gtidy3d/get_results.py
+-rw-r--r--   0        0        0    20009 2023-05-09 00:30:20.340903 gdsfactory-6.92.0/gdsfactory/simulation/gtidy3d/get_simulation.py
+-rw-r--r--   0        0        0    21061 2023-05-09 00:30:20.340903 gdsfactory-6.92.0/gdsfactory/simulation/gtidy3d/get_simulation_grating_coupler.py
+-rw-r--r--   0        0        0     2821 2023-05-09 00:30:20.340903 gdsfactory-6.92.0/gdsfactory/simulation/gtidy3d/materials.py
+-rw-r--r--   0        0        0    39677 2023-05-09 00:30:20.340903 gdsfactory-6.92.0/gdsfactory/simulation/gtidy3d/modes.py
+-rw-r--r--   0        0        0     8941 2023-05-09 00:30:20.340903 gdsfactory-6.92.0/gdsfactory/simulation/gtidy3d/sim_run.yaml
+-rw-r--r--   0        0        0     8114 2023-05-09 00:30:20.340903 gdsfactory-6.92.0/gdsfactory/simulation/gtidy3d/tests/sim_ref.yaml
+-rw-r--r--   0        0        0     8114 2023-05-09 00:30:20.340903 gdsfactory-6.92.0/gdsfactory/simulation/gtidy3d/tests/sim_run.yaml
+-rw-r--r--   0        0        0     1597 2023-05-09 00:30:20.340903 gdsfactory-6.92.0/gdsfactory/simulation/gtidy3d/tests/test_modes.py
+-rw-r--r--   0        0        0      262 2023-05-09 00:30:20.340903 gdsfactory-6.92.0/gdsfactory/simulation/gtidy3d/tests/test_modes/test_sweep_width.csv
+-rw-r--r--   0        0        0      879 2023-05-09 00:30:20.340903 gdsfactory-6.92.0/gdsfactory/simulation/gtidy3d/tests/test_results.py
+-rw-r--r--   0        0        0     1505 2023-05-09 00:30:20.340903 gdsfactory-6.92.0/gdsfactory/simulation/gtidy3d/tests/test_simulation.py
+-rw-r--r--   0        0        0     1270 2023-05-09 00:30:20.340903 gdsfactory-6.92.0/gdsfactory/simulation/gtidy3d/tests/test_write_sparameters.py
+-rw-r--r--   0        0        0     9297 2023-05-09 00:30:20.340903 gdsfactory-6.92.0/gdsfactory/simulation/gtidy3d/tests/test_write_sparameters/test_sparameters_straight.csv
+-rw-r--r--   0        0        0     1732 2023-05-09 00:30:20.340903 gdsfactory-6.92.0/gdsfactory/simulation/gtidy3d/tests/test_write_sparameters_grating_coupler.py
+-rw-r--r--   0        0        0     1224 2023-05-09 00:30:20.340903 gdsfactory-6.92.0/gdsfactory/simulation/gtidy3d/utils.py
+-rw-r--r--   0        0        0    10515 2023-05-09 00:30:20.340903 gdsfactory-6.92.0/gdsfactory/simulation/gtidy3d/write_sparameters.py
+-rw-r--r--   0        0        0     7695 2023-05-09 00:30:20.340903 gdsfactory-6.92.0/gdsfactory/simulation/gtidy3d/write_sparameters_grating_coupler.py
+-rw-r--r--   0        0        0      588 2023-05-09 00:30:20.340903 gdsfactory-6.92.0/gdsfactory/simulation/lumerical/__init__.py
+-rw-r--r--   0        0        0    16011 2023-05-09 00:30:20.340903 gdsfactory-6.92.0/gdsfactory/simulation/lumerical/interconnect.py
+-rw-r--r--   0        0        0     4286 2023-05-09 00:30:20.340903 gdsfactory-6.92.0/gdsfactory/simulation/lumerical/read.py
+-rw-r--r--   0        0        0     3569 2023-05-09 00:30:20.340903 gdsfactory-6.92.0/gdsfactory/simulation/lumerical/settings.py
+-rw-r--r--   0        0        0     2348 2023-05-09 00:30:20.340903 gdsfactory-6.92.0/gdsfactory/simulation/lumerical/test_read_sparameters.py
+-rw-r--r--   0        0        0    19865 2023-05-09 00:30:20.340903 gdsfactory-6.92.0/gdsfactory/simulation/lumerical/write_sparameters_lumerical.py
+-rw-r--r--   0        0        0     1504 2023-05-09 00:30:20.340903 gdsfactory-6.92.0/gdsfactory/simulation/lumerical/write_sparameters_lumerical_components.py
+-rw-r--r--   0        0        0      932 2023-05-09 00:30:20.340903 gdsfactory-6.92.0/gdsfactory/simulation/modes/__init__.py
+-rw-r--r--   0        0        0     1574 2023-05-09 00:30:20.340903 gdsfactory-6.92.0/gdsfactory/simulation/modes/coupler.py
+-rw-r--r--   0        0        0     4132 2023-05-09 00:30:20.340903 gdsfactory-6.92.0/gdsfactory/simulation/modes/find_coupling_vs_gap.py
+-rw-r--r--   0        0        0     2534 2023-05-09 00:30:20.340903 gdsfactory-6.92.0/gdsfactory/simulation/modes/find_mode_dispersion.py
+-rw-r--r--   0        0        0     8846 2023-05-09 00:30:20.340903 gdsfactory-6.92.0/gdsfactory/simulation/modes/find_modes.py
+-rwxr-xr-x   0        0        0     7032 2023-05-09 00:30:20.340903 gdsfactory-6.92.0/gdsfactory/simulation/modes/find_modes_cross_section.py
+-rw-r--r--   0        0        0     4448 2023-05-09 00:30:20.340903 gdsfactory-6.92.0/gdsfactory/simulation/modes/find_neff_ng_dw_dh.py
+-rw-r--r--   0        0        0     2706 2023-05-09 00:30:20.340903 gdsfactory-6.92.0/gdsfactory/simulation/modes/find_neff_vs_width.py
+-rw-r--r--   0        0        0     6956 2023-05-09 00:30:20.340903 gdsfactory-6.92.0/gdsfactory/simulation/modes/get_mode_solver_coupler.py
+-rwxr-xr-x   0        0        0     4462 2023-05-09 00:30:20.340903 gdsfactory-6.92.0/gdsfactory/simulation/modes/get_mode_solver_cross_section.py
+-rw-r--r--   0        0        0     5257 2023-05-09 00:30:20.340903 gdsfactory-6.92.0/gdsfactory/simulation/modes/get_mode_solver_rib.py
+-rw-r--r--   0        0        0     1110 2023-05-09 00:30:20.340903 gdsfactory-6.92.0/gdsfactory/simulation/modes/modes/neff_vs_width_nitride.csv
+-rw-r--r--   0        0        0     1102 2023-05-09 00:30:20.340903 gdsfactory-6.92.0/gdsfactory/simulation/modes/modes/neff_vs_width_rib.csv
+-rw-r--r--   0        0        0     1110 2023-05-09 00:30:20.340903 gdsfactory-6.92.0/gdsfactory/simulation/modes/modes/neff_vs_width_strip.csv
+-rw-r--r--   0        0        0     7979 2023-05-09 00:30:20.340903 gdsfactory-6.92.0/gdsfactory/simulation/modes/neff_convergence_test.py
+-rw-r--r--   0        0        0      267 2023-05-09 00:30:20.340903 gdsfactory-6.92.0/gdsfactory/simulation/modes/neff_vs_width.csv
+-rw-r--r--   0        0        0     2469 2023-05-09 00:30:20.340903 gdsfactory-6.92.0/gdsfactory/simulation/modes/overlap.py
+-rw-r--r--   0        0        0      418 2023-05-09 00:30:20.340903 gdsfactory-6.92.0/gdsfactory/simulation/modes/tests/test_dw_dh.py
+-rw-r--r--   0        0        0       83 2023-05-09 00:30:20.340903 gdsfactory-6.92.0/gdsfactory/simulation/modes/tests/test_dw_dh/test_dw_dh.csv
+-rw-r--r--   0        0        0      548 2023-05-09 00:30:20.340903 gdsfactory-6.92.0/gdsfactory/simulation/modes/tests/test_dw_dh/test_dw_dh_dispersion.csv
+-rw-r--r--   0        0        0     1131 2023-05-09 00:30:20.340903 gdsfactory-6.92.0/gdsfactory/simulation/modes/tests/test_find_modes.py
+-rw-r--r--   0        0        0      647 2023-05-09 00:30:20.340903 gdsfactory-6.92.0/gdsfactory/simulation/modes/tests/test_find_modes_dispersion.py
+-rw-r--r--   0        0        0      354 2023-05-09 00:30:20.340903 gdsfactory-6.92.0/gdsfactory/simulation/modes/tests/test_neff_vs_width.py
+-rw-r--r--   0        0        0      113 2023-05-09 00:30:20.340903 gdsfactory-6.92.0/gdsfactory/simulation/modes/tests/test_neff_vs_width/test_neff_vs_width.csv
+-rw-r--r--   0        0        0    15452 2023-05-09 00:30:20.340903 gdsfactory-6.92.0/gdsfactory/simulation/modes/types.py
+-rw-r--r--   0        0        0     1145 2023-05-09 00:30:20.340903 gdsfactory-6.92.0/gdsfactory/simulation/modes/waveguide.py
+-rw-r--r--   0        0        0     2013 2023-05-09 00:30:20.340903 gdsfactory-6.92.0/gdsfactory/simulation/photonic_circuit_models/__init__.py
+-rw-r--r--   0        0        0      597 2023-05-09 00:30:20.340903 gdsfactory-6.92.0/gdsfactory/simulation/photonic_circuit_models/coupler.py
+-rw-r--r--   0        0        0      377 2023-05-09 00:30:20.340903 gdsfactory-6.92.0/gdsfactory/simulation/photonic_circuit_models/fsr.py
+-rw-r--r--   0        0        0      418 2023-05-09 00:30:20.340903 gdsfactory-6.92.0/gdsfactory/simulation/photonic_circuit_models/heater.py
+-rw-r--r--   0        0        0     3063 2023-05-09 00:30:20.340903 gdsfactory-6.92.0/gdsfactory/simulation/photonic_circuit_models/mzi.py
+-rw-r--r--   0        0        0     2616 2023-05-09 00:30:20.340903 gdsfactory-6.92.0/gdsfactory/simulation/photonic_circuit_models/ring.py
+-rw-r--r--   0        0        0     7332 2023-05-09 00:30:20.340903 gdsfactory-6.92.0/gdsfactory/simulation/plot.py
+-rw-r--r--   0        0        0     2480 2023-05-09 00:30:20.340903 gdsfactory-6.92.0/gdsfactory/simulation/plot_csv.py
+-rw-r--r--   0        0        0      703 2023-05-09 00:30:20.340903 gdsfactory-6.92.0/gdsfactory/simulation/port_symmetries.py
+-rw-r--r--   0        0        0     4637 2023-05-09 00:30:20.340903 gdsfactory-6.92.0/gdsfactory/simulation/process/diffusion.py
+-rw-r--r--   0        0        0     5317 2023-05-09 00:30:20.340903 gdsfactory-6.92.0/gdsfactory/simulation/process/implant_tables.py
+-rw-r--r--   0        0        0     6784 2023-05-09 00:30:20.344903 gdsfactory-6.92.0/gdsfactory/simulation/process/pysrim.py
+-rw-r--r--   0        0        0     2182 2023-05-09 00:30:20.344903 gdsfactory-6.92.0/gdsfactory/simulation/process/silicon.py
+-rw-r--r--   0        0        0     1861 2023-05-09 00:30:20.344903 gdsfactory-6.92.0/gdsfactory/simulation/process/skew/antimony_si_skew.csv
+-rw-r--r--   0        0        0     1050 2023-05-09 00:30:20.344903 gdsfactory-6.92.0/gdsfactory/simulation/process/skew/arsenic_si_skew.csv
+-rw-r--r--   0        0        0     1468 2023-05-09 00:30:20.344903 gdsfactory-6.92.0/gdsfactory/simulation/process/skew/boron_si_skew.csv
+-rw-r--r--   0        0        0     1118 2023-05-09 00:30:20.344903 gdsfactory-6.92.0/gdsfactory/simulation/process/skew/phosphorus_si_skew.csv
+-rw-r--r--   0        0        0      191 2023-05-09 00:30:20.344903 gdsfactory-6.92.0/gdsfactory/simulation/sax/__init__.py
+-rw-r--r--   0        0        0    14792 2023-05-09 00:30:20.344903 gdsfactory-6.92.0/gdsfactory/simulation/sax/build_model.py
+-rw-r--r--   0        0        0     7449 2023-05-09 00:30:20.344903 gdsfactory-6.92.0/gdsfactory/simulation/sax/femwell_waveguide_model.py
+-rw-r--r--   0        0        0     1571 2023-05-09 00:30:20.344903 gdsfactory-6.92.0/gdsfactory/simulation/sax/interpolators.py
+-rw-r--r--   0        0        0     6755 2023-05-09 00:30:20.344903 gdsfactory-6.92.0/gdsfactory/simulation/sax/meep_FDTD_model.py
+-rw-r--r--   0        0        0     4528 2023-05-09 00:30:20.344903 gdsfactory-6.92.0/gdsfactory/simulation/sax/meow_eme_model.py
+-rw-r--r--   0        0        0     5613 2023-05-09 00:30:20.344903 gdsfactory-6.92.0/gdsfactory/simulation/sax/mlp.py
+-rw-r--r--   0        0        0     7358 2023-05-09 00:30:20.344903 gdsfactory-6.92.0/gdsfactory/simulation/sax/models.py
+-rw-r--r--   0        0        0    13884 2023-05-09 00:30:20.344903 gdsfactory-6.92.0/gdsfactory/simulation/sax/parameter.py
+-rwxr-xr-x   0        0        0     2205 2023-05-09 00:30:20.344903 gdsfactory-6.92.0/gdsfactory/simulation/sax/plot_model.py
+-rw-r--r--   0        0        0     6805 2023-05-09 00:30:20.344903 gdsfactory-6.92.0/gdsfactory/simulation/sax/read.py
+-rw-r--r--   0        0        0     1350 2023-05-09 00:30:20.344903 gdsfactory-6.92.0/gdsfactory/simulation/sax/tests/test_mzi.py
+-rw-r--r--   0        0        0     2220 2023-05-09 00:30:20.344903 gdsfactory-6.92.0/gdsfactory/simulation/sax/tests/test_mzi_lattice.py
+-rw-r--r--   0        0        0     1397 2023-05-09 00:30:20.344903 gdsfactory-6.92.0/gdsfactory/simulation/sax/tests/test_parameters.py
+-rw-r--r--   0        0        0     1357 2023-05-09 00:30:20.344903 gdsfactory-6.92.0/gdsfactory/simulation/simphony/__init__.py
+-rw-r--r--   0        0        0     1573 2023-05-09 00:30:20.344903 gdsfactory-6.92.0/gdsfactory/simulation/simphony/add_gc.py
+-rw-r--r--   0        0        0     3383 2023-05-09 00:30:20.344903 gdsfactory-6.92.0/gdsfactory/simulation/simphony/circuit.py
+-rw-r--r--   0        0        0      891 2023-05-09 00:30:20.344903 gdsfactory-6.92.0/gdsfactory/simulation/simphony/components/__init__.py
+-rw-r--r--   0        0        0     1295 2023-05-09 00:30:20.344903 gdsfactory-6.92.0/gdsfactory/simulation/simphony/components/bend_circular.py
+-rw-r--r--   0        0        0     1388 2023-05-09 00:30:20.344903 gdsfactory-6.92.0/gdsfactory/simulation/simphony/components/bend_euler.py
+-rw-r--r--   0        0        0     2560 2023-05-09 00:30:20.344903 gdsfactory-6.92.0/gdsfactory/simulation/simphony/components/coupler.py
+-rw-r--r--   0        0        0     1046 2023-05-09 00:30:20.344903 gdsfactory-6.92.0/gdsfactory/simulation/simphony/components/coupler_fdtd.py
+-rw-r--r--   0        0        0     1848 2023-05-09 00:30:20.344903 gdsfactory-6.92.0/gdsfactory/simulation/simphony/components/coupler_ring.py
+-rw-r--r--   0        0        0     1329 2023-05-09 00:30:20.344903 gdsfactory-6.92.0/gdsfactory/simulation/simphony/components/coupler_ring_fdtd.py
+-rw-r--r--   0        0        0      589 2023-05-09 00:30:20.344903 gdsfactory-6.92.0/gdsfactory/simulation/simphony/components/coupler_ring_siepic.py
+-rw-r--r--   0        0        0      913 2023-05-09 00:30:20.344903 gdsfactory-6.92.0/gdsfactory/simulation/simphony/components/gc.py
+-rw-r--r--   0        0        0     2032 2023-05-09 00:30:20.344903 gdsfactory-6.92.0/gdsfactory/simulation/simphony/components/mmi1x2.py
+-rw-r--r--   0        0        0     1910 2023-05-09 00:30:20.344903 gdsfactory-6.92.0/gdsfactory/simulation/simphony/components/mmi2x2.py
+-rw-r--r--   0        0        0     2618 2023-05-09 00:30:20.344903 gdsfactory-6.92.0/gdsfactory/simulation/simphony/components/mzi.py
+-rw-r--r--   0        0        0     1759 2023-05-09 00:30:20.344903 gdsfactory-6.92.0/gdsfactory/simulation/simphony/components/mzi_siepic.py
+-rw-r--r--   0        0        0      487 2023-05-09 00:30:20.344903 gdsfactory-6.92.0/gdsfactory/simulation/simphony/components/mzi_thermal.py
+-rw-r--r--   0        0        0     2597 2023-05-09 00:30:20.344903 gdsfactory-6.92.0/gdsfactory/simulation/simphony/components/ring_double.py
+-rw-r--r--   0        0        0     1665 2023-05-09 00:30:20.344903 gdsfactory-6.92.0/gdsfactory/simulation/simphony/components/ring_double_siepic.py
+-rw-r--r--   0        0        0     1782 2023-05-09 00:30:20.344903 gdsfactory-6.92.0/gdsfactory/simulation/simphony/components/ring_single.py
+-rw-r--r--   0        0        0     1416 2023-05-09 00:30:20.344903 gdsfactory-6.92.0/gdsfactory/simulation/simphony/components/ring_single_siepic.py
+-rw-r--r--   0        0        0     1099 2023-05-09 00:30:20.344903 gdsfactory-6.92.0/gdsfactory/simulation/simphony/components/straight.py
+-rw-r--r--   0        0        0      800 2023-05-09 00:30:20.344903 gdsfactory-6.92.0/gdsfactory/simulation/simphony/get_transmission.py
+-rw-r--r--   0        0        0     2516 2023-05-09 00:30:20.344903 gdsfactory-6.92.0/gdsfactory/simulation/simphony/model_from_gdsfactory.py
+-rw-r--r--   0        0        0     3841 2023-05-09 00:30:20.344903 gdsfactory-6.92.0/gdsfactory/simulation/simphony/model_from_sparameters.py
+-rw-r--r--   0        0        0     2438 2023-05-09 00:30:20.344903 gdsfactory-6.92.0/gdsfactory/simulation/simphony/plot_circuit.py
+-rw-r--r--   0        0        0     1798 2023-05-09 00:30:20.344903 gdsfactory-6.92.0/gdsfactory/simulation/simphony/plot_circuit_montecarlo.py
+-rw-r--r--   0        0        0     2773 2023-05-09 00:30:20.344903 gdsfactory-6.92.0/gdsfactory/simulation/simphony/plot_model.py
+-rw-r--r--   0        0        0     1261 2023-05-09 00:30:20.344903 gdsfactory-6.92.0/gdsfactory/simulation/simphony/tests/test_circuit.py
+-rw-r--r--   0        0        0       90 2023-05-09 00:30:20.344903 gdsfactory-6.92.0/gdsfactory/simulation/simphony/tests/test_circuit/test_circuit_transmission.yml
+-rw-r--r--   0        0        0     1109 2023-05-09 00:30:20.344903 gdsfactory-6.92.0/gdsfactory/simulation/simphony/tests/test_components.py
+-rw-r--r--   0        0        0       66 2023-05-09 00:30:20.344903 gdsfactory-6.92.0/gdsfactory/simulation/simphony/tests/test_components/test_circuits_mzi_.yml
+-rw-r--r--   0        0        0       69 2023-05-09 00:30:20.344903 gdsfactory-6.92.0/gdsfactory/simulation/simphony/tests/test_components/test_circuits_ring_double_.yml
+-rw-r--r--   0        0        0       69 2023-05-09 00:30:20.344903 gdsfactory-6.92.0/gdsfactory/simulation/simphony/tests/test_components/test_circuits_ring_single_.yml
+-rw-r--r--   0        0        0       92 2023-05-09 00:30:20.344903 gdsfactory-6.92.0/gdsfactory/simulation/simphony/tests/test_components/test_elements_bend_circular_.yml
+-rw-r--r--   0        0        0       92 2023-05-09 00:30:20.344903 gdsfactory-6.92.0/gdsfactory/simulation/simphony/tests/test_components/test_elements_bend_euler_.yml
+-rw-r--r--   0        0        0      412 2023-05-09 00:30:20.344903 gdsfactory-6.92.0/gdsfactory/simulation/simphony/tests/test_components/test_elements_coupler_.yml
+-rw-r--r--   0        0        0      412 2023-05-09 00:30:20.344903 gdsfactory-6.92.0/gdsfactory/simulation/simphony/tests/test_components/test_elements_coupler_ring_.yml
+-rw-r--r--   0        0        0      114 2023-05-09 00:30:20.344903 gdsfactory-6.92.0/gdsfactory/simulation/simphony/tests/test_components/test_elements_gc1550te_.yml
+-rw-r--r--   0        0        0      256 2023-05-09 00:30:20.344903 gdsfactory-6.92.0/gdsfactory/simulation/simphony/tests/test_components/test_elements_mmi1x2_.yml
+-rw-r--r--   0        0        0      460 2023-05-09 00:30:20.344903 gdsfactory-6.92.0/gdsfactory/simulation/simphony/tests/test_components/test_elements_mmi2x2_.yml
+-rw-r--r--   0        0        0      104 2023-05-09 00:30:20.344903 gdsfactory-6.92.0/gdsfactory/simulation/simphony/tests/test_components/test_elements_straight_.yml
+-rw-r--r--   0        0        0      166 2023-05-09 00:30:20.344903 gdsfactory-6.92.0/gdsfactory/simulation/simphony/types.py
+-rw-r--r--   0        0        0      471 2023-05-09 00:30:20.344903 gdsfactory-6.92.0/gdsfactory/simulation/sipann/__init__.py
+-rw-r--r--   0        0        0     1376 2023-05-09 00:30:20.344903 gdsfactory-6.92.0/gdsfactory/simulation/sipann/bend_circular.py
+-rw-r--r--   0        0        0     1465 2023-05-09 00:30:20.344903 gdsfactory-6.92.0/gdsfactory/simulation/sipann/bend_euler.py
+-rw-r--r--   0        0        0     2508 2023-05-09 00:30:20.344903 gdsfactory-6.92.0/gdsfactory/simulation/sipann/coupler.py
+-rw-r--r--   0        0        0     1892 2023-05-09 00:30:20.344903 gdsfactory-6.92.0/gdsfactory/simulation/sipann/coupler_ring.py
+-rw-r--r--   0        0        0      736 2023-05-09 00:30:20.344903 gdsfactory-6.92.0/gdsfactory/simulation/sipann/straight.py
+-rw-r--r--   0        0        0      100 2023-05-09 00:30:20.344903 gdsfactory-6.92.0/gdsfactory/simulation/thermal/__init__.py
+-rw-r--r--   0        0        0     7781 2023-05-09 00:30:20.344903 gdsfactory-6.92.0/gdsfactory/simulation/thermal/heater.py
+-rw-r--r--   0        0        0     1744 2023-05-09 00:30:20.344903 gdsfactory-6.92.0/gdsfactory/snap.py
+-rw-r--r--   0        0        0     4245 2023-05-09 00:30:20.344903 gdsfactory-6.92.0/gdsfactory/symbols.py
+-rw-r--r--   0        0        0      524 2023-05-09 00:30:20.344903 gdsfactory-6.92.0/gdsfactory/technology/__init__.py
+-rw-r--r--   0        0        0     7065 2023-05-09 00:30:20.344903 gdsfactory-6.92.0/gdsfactory/technology/klayout_tech.py
+-rw-r--r--   0        0        0     1078 2023-05-09 00:30:20.344903 gdsfactory-6.92.0/gdsfactory/technology/layer_map.py
+-rw-r--r--   0        0        0    14989 2023-05-09 00:30:20.344903 gdsfactory-6.92.0/gdsfactory/technology/layer_stack.py
+-rw-r--r--   0        0        0    42052 2023-05-09 00:30:20.344903 gdsfactory-6.92.0/gdsfactory/technology/layer_views.py
+-rw-r--r--   0        0        0     1984 2023-05-09 00:30:20.344903 gdsfactory-6.92.0/gdsfactory/technology/simulation_settings.py
+-rw-r--r--   0        0        0     1635 2023-05-09 00:30:20.344903 gdsfactory-6.92.0/gdsfactory/types.py
+-rw-r--r--   0        0        0    10000 2023-05-09 00:30:20.344903 gdsfactory-6.92.0/gdsfactory/typings.py
+-rw-r--r--   0        0        0        0 2023-05-09 00:30:20.344903 gdsfactory-6.92.0/gdsfactory/utils/__init__.py
+-rw-r--r--   0        0        0     1304 2023-05-09 00:30:20.344903 gdsfactory-6.92.0/gdsfactory/utils/async_utils.py
+-rw-r--r--   0        0        0      376 2023-05-09 00:30:20.344903 gdsfactory-6.92.0/gdsfactory/utils/color_utils.py
+-rw-r--r--   0        0        0      558 2023-05-09 00:30:20.344903 gdsfactory-6.92.0/gdsfactory/utils/file_utils.py
+-rw-r--r--   0        0        0      185 2023-05-09 00:30:20.344903 gdsfactory-6.92.0/gdsfactory/utils/function_utils.py
+-rw-r--r--   0        0        0      676 2023-05-09 00:30:20.344903 gdsfactory-6.92.0/gdsfactory/utils/xml_utils.py
+-rw-r--r--   0        0        0     1429 2023-05-09 00:30:20.344903 gdsfactory-6.92.0/gdsfactory/utils/yaml_utils.py
+-rw-r--r--   0        0        0     4825 2023-05-09 00:30:20.344903 gdsfactory-6.92.0/gdsfactory/watch.py
+-rw-r--r--   0        0        0        0 2023-05-09 00:30:20.344903 gdsfactory-6.92.0/gdsfactory/widgets/__init__.py
+-rw-r--r--   0        0        0     7921 2023-05-09 00:30:20.344903 gdsfactory-6.92.0/gdsfactory/widgets/layout_viewer.py
+-rw-r--r--   0        0        0     7464 2023-05-09 00:30:20.344903 gdsfactory-6.92.0/gdsfactory/write_cells.py
+-rw-r--r--   0        0        0     5467 2023-05-09 00:30:20.344903 gdsfactory-6.92.0/pyproject.toml
+-rw-r--r--   0        0        0    18552 1970-01-01 00:00:00.000000 gdsfactory-6.92.0/PKG-INFO
```

### Comparing `gdsfactory-6.91.0/LICENSE` & `gdsfactory-6.92.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/README.md` & `gdsfactory-6.92.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# gdsfactory 6.91.0
+# gdsfactory 6.92.0
 
 [![docs](https://github.com/gdsfactory/gdsfactory/actions/workflows/pages.yml/badge.svg)](https://gdsfactory.github.io/gdsfactory/)
 [![PyPI](https://img.shields.io/pypi/v/gdsfactory)](https://pypi.org/project/gdsfactory/)
 [![Conda Version](https://img.shields.io/conda/vn/conda-forge/gdsfactory.svg)](https://anaconda.org/conda-forge/gdsfactory)
 [![Dockerhub](https://img.shields.io/docker/pulls/joamatab/gdsfactory)](https://hub.docker.com/r/joamatab/gdsfactory)
 [![PyPI Python](https://img.shields.io/pypi/pyversions/gdsfactory.svg)](https://pypi.python.org/pypi/gdsfactory)
 [![issues](https://img.shields.io/github/issues/gdsfactory/gdsfactory)](https://github.com/gdsfactory/gdsfactory/issues)
@@ -223,14 +223,13 @@
 
 ---
 
 "I use gdsfactory for all of my photonic tape-outs. The Python interface makes it easy to version control individual photonic components as well as entire layouts, while integrating seamlessly with KLayout and most standard photonic simulation tools, both open-source and commercial.
 
 <div style="text-align: right; margin-right: 10%;">Thomas Dorch - <strong>Freedom Photonics</strong></div>
 
-<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
-<!-- prettier-ignore-start -->
-<!-- markdownlint-disable -->
-<!-- markdownlint-restore -->
-<!-- prettier-ignore-end -->
 
-<!-- ALL-CONTRIBUTORS-LIST:END -->
+## Contributors
+
+Thanks to all the contributors that make this awesome project possible!
+
+[![Meet our contributors!](https://contrib.rocks/image?repo=gdsfactory/gdsfactory)](https://github.com/gdsfactory/gdsfactory/graphs/contributors)
```

### Comparing `gdsfactory-6.91.0/gdsfactory/__init__.py` & `gdsfactory-6.92.0/gdsfactory/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -142,8 +142,8 @@
     "snap",
     "typings",
     "technology",
     "write_cells",
     "xsection",
     "PATH",
 )
-__version__ = "6.91.0"
+__version__ = "6.92.0"
```

### Comparing `gdsfactory-6.91.0/gdsfactory/add_keepout.py` & `gdsfactory-6.92.0/gdsfactory/add_keepout.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/add_labels.py` & `gdsfactory-6.92.0/gdsfactory/add_labels.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/add_loopback.py` & `gdsfactory-6.92.0/gdsfactory/add_loopback.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/add_padding.py` & `gdsfactory-6.92.0/gdsfactory/add_padding.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/add_pins.py` & `gdsfactory-6.92.0/gdsfactory/add_pins.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/add_ports.py` & `gdsfactory-6.92.0/gdsfactory/add_ports.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/add_tapers.py` & `gdsfactory-6.92.0/gdsfactory/add_tapers.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/add_tapers_cross_section.py` & `gdsfactory-6.92.0/gdsfactory/add_tapers_cross_section.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/add_termination.py` & `gdsfactory-6.92.0/gdsfactory/add_termination.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/asserts.py` & `gdsfactory-6.92.0/gdsfactory/asserts.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/cell.py` & `gdsfactory-6.92.0/gdsfactory/cell.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/circuitviz.py` & `gdsfactory-6.92.0/gdsfactory/circuitviz.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/cli.py` & `gdsfactory-6.92.0/gdsfactory/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from gdsfactory.write_cells import write_cells as write_cells_to_separate_gds
 
 try:
     import rich_click as click
 except ImportError:
     import click
 
-VERSION = "6.91.0"
+VERSION = "6.92.0"
 LAYER_LABEL = LAYER.LABEL
 
 
 def print_version(ctx: Context, param: Option, value: bool) -> None:
     """Prints the version."""
     if not value or ctx.resilient_parsing:
         return
```

### Comparing `gdsfactory-6.91.0/gdsfactory/component.py` & `gdsfactory-6.92.0/gdsfactory/component.py`

 * *Files 0% similar despite different names*

```diff
@@ -2963,3227 +2963,3237 @@
 0000b920: 7769 6467 6574 290a 0a20 2020 2064 6566  widget)..    def
 0000b930: 2070 6c6f 745f 6b6c 6179 6f75 7428 0a20   plot_klayout(. 
 0000b940: 2020 2020 2020 2073 656c 662c 0a20 2020         self,.   
 0000b950: 2020 2020 2073 686f 775f 706f 7274 733a       show_ports:
 0000b960: 2062 6f6f 6c20 3d20 5472 7565 2c0a 2020   bool = True,.  
 0000b970: 2020 2020 2020 706f 7274 5f6d 6172 6b65        port_marke
 0000b980: 725f 6c61 7965 723a 204c 6179 6572 203d  r_layer: Layer =
-0000b990: 2028 312c 2031 3029 2c0a 2020 2020 2920   (1, 10),.    ) 
-0000b9a0: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
-0000b9b0: 2022 2222 5265 7475 726e 7320 6b6c 6179   """Returns klay
-0000b9c0: 6f75 7420 696d 6167 652e 0a0a 2020 2020  out image...    
-0000b9d0: 2020 2020 4966 2069 7420 6661 696c 7320      If it fails 
-0000b9e0: 746f 2069 6d70 6f72 7420 6b6c 6179 6f75  to import klayou
-0000b9f0: 7420 6465 6661 756c 7473 2074 6f20 6d61  t defaults to ma
-0000ba00: 7470 6c6f 746c 6962 2e0a 0a20 2020 2020  tplotlib...     
-0000ba10: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
-0000ba20: 2020 2020 2073 686f 775f 706f 7274 733a       show_ports:
-0000ba30: 2073 686f 7773 2063 6f6d 706f 6e65 6e74   shows component
-0000ba40: 2077 6974 6820 706f 7274 206d 6172 6b65   with port marke
-0000ba50: 7273 2061 6e64 206c 6162 656c 732e 0a20  rs and labels.. 
-0000ba60: 2020 2020 2020 2020 2020 2070 6f72 745f             port_
-0000ba70: 6d61 726b 6572 5f6c 6179 6572 3a20 666f  marker_layer: fo
-0000ba80: 7220 7468 6520 706f 7274 732e 0a20 2020  r the ports..   
-0000ba90: 2020 2020 2022 2222 0a0a 2020 2020 2020       """..      
-0000baa0: 2020 636f 6d70 6f6e 656e 7420 3d20 280a    component = (.
-0000bab0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000bac0: 2e61 6464 5f70 696e 735f 7472 6961 6e67  .add_pins_triang
-0000bad0: 6c65 2870 6f72 745f 6d61 726b 6572 5f6c  le(port_marker_l
-0000bae0: 6179 6572 3d70 6f72 745f 6d61 726b 6572  ayer=port_marker
-0000baf0: 5f6c 6179 6572 290a 2020 2020 2020 2020  _layer).        
-0000bb00: 2020 2020 6966 2073 686f 775f 706f 7274      if show_port
-0000bb10: 730a 2020 2020 2020 2020 2020 2020 656c  s.            el
-0000bb20: 7365 2073 656c 660a 2020 2020 2020 2020  se self.        
-0000bb30: 290a 0a20 2020 2020 2020 2074 7279 3a0a  )..        try:.
-0000bb40: 2020 2020 2020 2020 2020 2020 696d 706f              impo
-0000bb50: 7274 206b 6c61 796f 7574 2e64 6220 6173  rt klayout.db as
-0000bb60: 2064 6220 2023 206e 6f71 613a 2046 3430   db  # noqa: F40
-0000bb70: 310a 2020 2020 2020 2020 2020 2020 696d  1.            im
-0000bb80: 706f 7274 206b 6c61 796f 7574 2e6c 6179  port klayout.lay
-0000bb90: 2061 7320 6c61 790a 2020 2020 2020 2020   as lay.        
-0000bba0: 2020 2020 6672 6f6d 2067 6473 6661 6374      from gdsfact
-0000bbb0: 6f72 792e 7064 6b20 696d 706f 7274 2067  ory.pdk import g
-0000bbc0: 6574 5f6c 6179 6572 5f76 6965 7773 0a20  et_layer_views. 
-0000bbd0: 2020 2020 2020 2020 2020 2066 726f 6d20             from 
-0000bbe0: 4950 7974 686f 6e2e 6469 7370 6c61 7920  IPython.display 
-0000bbf0: 696d 706f 7274 2064 6973 706c 6179 0a20  import display. 
-0000bc00: 2020 2020 2020 2020 2020 2066 726f 6d20             from 
-0000bc10: 6970 7977 6964 6765 7473 2069 6d70 6f72  ipywidgets impor
-0000bc20: 7420 496d 6167 650a 0a20 2020 2020 2020  t Image..       
-0000bc30: 2020 2020 2067 6473 7061 7468 203d 2063       gdspath = c
-0000bc40: 6f6d 706f 6e65 6e74 2e77 7269 7465 5f67  omponent.write_g
-0000bc50: 6473 286c 6f67 6769 6e67 3d46 616c 7365  ds(logging=False
-0000bc60: 290a 2020 2020 2020 2020 2020 2020 6c79  ).            ly
-0000bc70: 705f 7061 7468 203d 2067 6473 7061 7468  p_path = gdspath
-0000bc80: 2e77 6974 685f 7375 6666 6978 2822 2e6c  .with_suffix(".l
-0000bc90: 7970 2229 0a0a 2020 2020 2020 2020 2020  yp")..          
-0000bca0: 2020 6c61 7965 725f 7669 6577 7320 3d20    layer_views = 
-0000bcb0: 6765 745f 6c61 7965 725f 7669 6577 7328  get_layer_views(
-0000bcc0: 290a 2020 2020 2020 2020 2020 2020 6c61  ).            la
-0000bcd0: 7965 725f 7669 6577 732e 746f 5f6c 7970  yer_views.to_lyp
-0000bce0: 2866 696c 6570 6174 683d 6c79 705f 7061  (filepath=lyp_pa
-0000bcf0: 7468 290a 0a20 2020 2020 2020 2020 2020  th)..           
-0000bd00: 206c 6179 6f75 745f 7669 6577 203d 206c   layout_view = l
-0000bd10: 6179 2e4c 6179 6f75 7456 6965 7728 290a  ay.LayoutView().
-0000bd20: 2020 2020 2020 2020 2020 2020 6c61 796f              layo
-0000bd30: 7574 5f76 6965 772e 6c6f 6164 5f6c 6179  ut_view.load_lay
-0000bd40: 6f75 7428 7374 7228 6764 7370 6174 682e  out(str(gdspath.
-0000bd50: 6162 736f 6c75 7465 2829 2929 0a20 2020  absolute())).   
-0000bd60: 2020 2020 2020 2020 206c 6179 6f75 745f           layout_
-0000bd70: 7669 6577 2e6d 6178 5f68 6965 7228 290a  view.max_hier().
-0000bd80: 2020 2020 2020 2020 2020 2020 6c61 796f              layo
-0000bd90: 7574 5f76 6965 772e 6c6f 6164 5f6c 6179  ut_view.load_lay
-0000bda0: 6572 5f70 726f 7073 2873 7472 286c 7970  er_props(str(lyp
-0000bdb0: 5f70 6174 6829 290a 0a20 2020 2020 2020  _path))..       
-0000bdc0: 2020 2020 2070 6978 656c 5f62 7566 6665       pixel_buffe
-0000bdd0: 7220 3d20 6c61 796f 7574 5f76 6965 772e  r = layout_view.
-0000bde0: 6765 745f 7069 7865 6c73 5f77 6974 685f  get_pixels_with_
-0000bdf0: 6f70 7469 6f6e 7328 3830 302c 2036 3030  options(800, 600
-0000be00: 290a 2020 2020 2020 2020 2020 2020 706e  ).            pn
-0000be10: 675f 6461 7461 203d 2070 6978 656c 5f62  g_data = pixel_b
-0000be20: 7566 6665 722e 746f 5f70 6e67 5f64 6174  uffer.to_png_dat
-0000be30: 6128 290a 2020 2020 2020 2020 2020 2020  a().            
-0000be40: 696d 6167 6520 3d20 496d 6167 6528 7661  image = Image(va
-0000be50: 6c75 653d 706e 675f 6461 7461 2c20 666f  lue=png_data, fo
-0000be60: 726d 6174 3d22 706e 6722 290a 2020 2020  rmat="png").    
-0000be70: 2020 2020 2020 2020 6469 7370 6c61 7928          display(
-0000be80: 696d 6167 6529 0a0a 2020 2020 2020 2020  image)..        
-0000be90: 6578 6365 7074 2049 6d70 6f72 7445 7272  except ImportErr
-0000bea0: 6f72 3a0a 2020 2020 2020 2020 2020 2020  or:.            
-0000beb0: 7072 696e 7428 0a20 2020 2020 2020 2020  print(.         
-0000bec0: 2020 2020 2020 2022 596f 7520 6361 6e20         "You can 
-0000bed0: 696e 7374 616c 6c20 6070 6970 2069 6e73  install `pip ins
-0000bee0: 7461 6c6c 2067 6473 6661 6374 6f72 795b  tall gdsfactory[
-0000bef0: 6675 6c6c 5d60 2066 6f72 2062 6574 7465  full]` for bette
-0000bf00: 7220 7669 7375 616c 697a 6174 696f 6e22  r visualization"
-0000bf10: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
-0000bf20: 2020 2020 2020 2020 2020 2063 6f6d 706f             compo
-0000bf30: 6e65 6e74 2e70 6c6f 7428 706c 6f74 7465  nent.plot(plotte
-0000bf40: 723d 226d 6174 706c 6f74 6c69 6222 290a  r="matplotlib").
-0000bf50: 0a20 2020 2064 6566 2070 6c6f 745f 6a75  .    def plot_ju
-0000bf60: 7079 7465 7228 7365 6c66 293a 0a20 2020  pyter(self):.   
-0000bf70: 2020 2020 2022 2222 5368 6f77 7320 6375       """Shows cu
-0000bf80: 7272 656e 7420 6764 7320 696e 206b 6c61  rrent gds in kla
-0000bf90: 796f 7574 2e20 5573 6573 204b 7765 6220  yout. Uses Kweb 
-0000bfa0: 6966 2073 6572 7665 7220 7275 6e6e 696e  if server runnin
-0000bfb0: 672e 0a0a 2020 2020 2020 2020 6966 206e  g...        if n
-0000bfc0: 6f74 2074 7269 6573 2075 7369 6e67 204b  ot tries using K
-0000bfd0: 6c61 796f 7574 2077 6964 6765 7420 616e  layout widget an
-0000bfe0: 6420 6669 6e61 6c6c 7920 6465 6661 756c  d finally defaul
-0000bff0: 7473 2074 6f20 6d61 7470 6c6f 746c 6962  ts to matplotlib
-0000c000: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
-0000c010: 2020 2020 2020 7472 793a 0a20 2020 2020        try:.     
-0000c020: 2020 2020 2020 2069 6d70 6f72 7420 6f73         import os
-0000c030: 0a20 2020 2020 2020 2020 2020 2066 726f  .            fro
-0000c040: 6d20 6764 7366 6163 746f 7279 2e63 6f6e  m gdsfactory.con
-0000c050: 6669 6720 696d 706f 7274 2050 4154 480a  fig import PATH.
-0000c060: 2020 2020 2020 2020 2020 2020 6672 6f6d              from
-0000c070: 2067 6473 6661 6374 6f72 792e 7064 6b20   gdsfactory.pdk 
-0000c080: 696d 706f 7274 2067 6574 5f6c 6179 6572  import get_layer
-0000c090: 5f76 6965 7773 0a20 2020 2020 2020 2020  _views.         
-0000c0a0: 2020 2066 726f 6d20 4950 7974 686f 6e2e     from IPython.
-0000c0b0: 6469 7370 6c61 7920 696d 706f 7274 2049  display import I
-0000c0c0: 4672 616d 650a 2020 2020 2020 2020 2020  Frame.          
-0000c0d0: 2020 696d 706f 7274 206b 7765 622e 7365    import kweb.se
-0000c0e0: 7276 6572 5f6a 7570 7974 6572 2061 7320  rver_jupyter as 
-0000c0f0: 6b6a 0a20 2020 2020 2020 2020 2020 2066  kj.            f
-0000c100: 726f 6d20 6874 6d6c 2069 6d70 6f72 7420  rom html import 
-0000c110: 6573 6361 7065 0a0a 2020 2020 2020 2020  escape..        
-0000c120: 2020 2020 6764 7370 6174 6820 3d20 7365      gdspath = se
-0000c130: 6c66 2e77 7269 7465 5f67 6473 2867 6473  lf.write_gds(gds
-0000c140: 6469 723d 5041 5448 2e67 6473 6c69 6220  dir=PATH.gdslib 
-0000c150: 2f20 2265 7874 7261 222c 206c 6f67 6769  / "extra", loggi
-0000c160: 6e67 3d46 616c 7365 290a 0a20 2020 2020  ng=False)..     
-0000c170: 2020 2020 2020 2064 6972 7061 7468 203d         dirpath =
-0000c180: 2047 4453 4449 525f 5445 4d50 0a20 2020   GDSDIR_TEMP.   
-0000c190: 2020 2020 2020 2020 2064 6972 7061 7468           dirpath
-0000c1a0: 2e6d 6b64 6972 2865 7869 7374 5f6f 6b3d  .mkdir(exist_ok=
-0000c1b0: 5472 7565 2c20 7061 7265 6e74 733d 5472  True, parents=Tr
-0000c1c0: 7565 290a 2020 2020 2020 2020 2020 2020  ue).            
-0000c1d0: 6c79 705f 7061 7468 203d 2064 6972 7061  lyp_path = dirpa
-0000c1e0: 7468 202f 2022 6c61 7965 7273 2e6c 7970  th / "layers.lyp
-0000c1f0: 220a 0a20 2020 2020 2020 2020 2020 206c  "..            l
-0000c200: 6179 6572 5f70 726f 7073 203d 2067 6574  ayer_props = get
-0000c210: 5f6c 6179 6572 5f76 6965 7773 2829 0a20  _layer_views(). 
-0000c220: 2020 2020 2020 2020 2020 206c 6179 6572             layer
-0000c230: 5f70 726f 7073 2e74 6f5f 6c79 7028 6669  _props.to_lyp(fi
-0000c240: 6c65 7061 7468 3d6c 7970 5f70 6174 6829  lepath=lyp_path)
-0000c250: 0a0a 2020 2020 2020 2020 2020 2020 7372  ..            sr
-0000c260: 6320 3d20 6622 6874 7470 3a2f 2f31 3237  c = f"http://127
-0000c270: 2e30 2e30 2e31 3a7b 6b6a 2e70 6f72 747d  .0.0.1:{kj.port}
-0000c280: 2f67 6473 3f67 6473 5f66 696c 653d 7b65  /gds?gds_file={e
-0000c290: 7363 6170 6528 7374 7228 6764 7370 6174  scape(str(gdspat
-0000c2a0: 6829 297d 266c 6179 6572 5f70 726f 7073  h))}&layer_props
-0000c2b0: 3d7b 6573 6361 7065 2873 7472 286c 7970  ={escape(str(lyp
-0000c2c0: 5f70 6174 6829 297d 220a 2020 2020 2020  _path))}".      
-0000c2d0: 2020 2020 2020 6c6f 6767 6572 2e64 6562        logger.deb
-0000c2e0: 7567 2873 7263 290a 0a20 2020 2020 2020  ug(src)..       
-0000c2f0: 2020 2020 2069 6620 6b6a 2e6a 7570 7974       if kj.jupyt
-0000c300: 6572 5f73 6572 7665 7220 616e 6420 6e6f  er_server and no
-0000c310: 7420 6f73 2e65 6e76 6972 6f6e 2e67 6574  t os.environ.get
-0000c320: 2822 444f 4353 222c 2046 616c 7365 293a  ("DOCS", False):
-0000c330: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000c340: 2072 6574 7572 6e20 4946 7261 6d65 280a   return IFrame(.
-0000c350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c360: 2020 2020 7372 633d 7372 632c 0a20 2020      src=src,.   
-0000c370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c380: 2077 6964 7468 3d31 3430 302c 0a20 2020   width=1400,.   
-0000c390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c3a0: 2068 6569 6768 743d 3630 302c 0a20 2020   height=600,.   
-0000c3b0: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
-0000c3c0: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-0000c3d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000c3e0: 2072 6574 7572 6e20 7365 6c66 2e70 6c6f   return self.plo
-0000c3f0: 745f 6b6c 6179 6f75 7428 290a 2020 2020  t_klayout().    
-0000c400: 2020 2020 6578 6365 7074 2049 6d70 6f72      except Impor
-0000c410: 7445 7272 6f72 3a0a 2020 2020 2020 2020  tError:.        
-0000c420: 2020 2020 7072 696e 7428 0a20 2020 2020      print(.     
-0000c430: 2020 2020 2020 2020 2020 2022 596f 7520             "You 
-0000c440: 6361 6e20 696e 7374 616c 6c20 6070 6970  can install `pip
-0000c450: 2069 6e73 7461 6c6c 2067 6473 6661 6374   install gdsfact
-0000c460: 6f72 795b 6675 6c6c 5d60 2066 6f72 2062  ory[full]` for b
-0000c470: 6574 7465 7220 7669 7375 616c 697a 6174  etter visualizat
-0000c480: 696f 6e22 0a20 2020 2020 2020 2020 2020  ion".           
-0000c490: 2029 0a20 2020 2020 2020 2020 2020 2072   ).            r
-0000c4a0: 6574 7572 6e20 7365 6c66 2e70 6c6f 745f  eturn self.plot_
-0000c4b0: 6b6c 6179 6f75 7428 290a 0a20 2020 2064  klayout()..    d
-0000c4c0: 6566 2070 6c6f 745f 6d61 7470 6c6f 746c  ef plot_matplotl
-0000c4d0: 6962 2873 656c 662c 202a 2a6b 7761 7267  ib(self, **kwarg
-0000c4e0: 7329 202d 3e20 4e6f 6e65 3a0a 2020 2020  s) -> None:.    
-0000c4f0: 2020 2020 2222 2250 6c6f 7420 636f 6d70      """Plot comp
-0000c500: 6f6e 656e 7420 7573 696e 6720 6d61 7470  onent using matp
-0000c510: 6c6f 746c 6962 2e0a 0a20 2020 2020 2020  lotlib...       
-0000c520: 204b 6579 776f 7264 2041 7267 733a 0a20   Keyword Args:. 
-0000c530: 2020 2020 2020 2020 2020 2073 686f 775f             show_
-0000c540: 706f 7274 733a 2053 6574 7320 7768 6574  ports: Sets whet
-0000c550: 6865 7220 706f 7274 7320 6172 6520 6472  her ports are dr
-0000c560: 6177 6e2e 0a20 2020 2020 2020 2020 2020  awn..           
-0000c570: 2073 686f 775f 7375 6270 6f72 7473 3a20   show_subports: 
-0000c580: 5365 7473 2077 6865 7468 6572 2073 7562  Sets whether sub
-0000c590: 706f 7274 7320 2870 6f72 7473 2074 6861  ports (ports tha
-0000c5a0: 7420 6265 6c6f 6e67 2074 6f20 7265 6665  t belong to refe
-0000c5b0: 7265 6e63 6573 2920 6172 6520 6472 6177  rences) are draw
-0000c5c0: 6e2e 0a20 2020 2020 2020 2020 2020 206c  n..            l
-0000c5d0: 6162 656c 5f61 6c69 6173 6573 3a20 5365  abel_aliases: Se
-0000c5e0: 7473 2077 6865 7468 6572 2061 6c69 6173  ts whether alias
-0000c5f0: 6573 2061 7265 206c 6162 656c 6564 2077  es are labeled w
-0000c600: 6974 6820 6120 7465 7874 206e 616d 652e  ith a text name.
-0000c610: 0a20 2020 2020 2020 2020 2020 206e 6577  .            new
-0000c620: 5f77 696e 646f 773a 2049 6620 5472 7565  _window: If True
-0000c630: 2c20 6561 6368 2063 616c 6c20 746f 2071  , each call to q
-0000c640: 7569 636b 706c 6f74 2829 2077 696c 6c20  uickplot() will 
-0000c650: 6765 6e65 7261 7465 2061 2073 6570 6172  generate a separ
-0000c660: 6174 6520 7769 6e64 6f77 2e0a 2020 2020  ate window..    
-0000c670: 2020 2020 2020 2020 626c 6f63 6b69 6e67          blocking
-0000c680: 3a20 4966 2054 7275 652c 2063 616c 6c69  : If True, calli
-0000c690: 6e67 2071 7569 636b 706c 6f74 2829 2077  ng quickplot() w
-0000c6a0: 696c 6c20 7061 7573 6520 6578 6563 7574  ill pause execut
-0000c6b0: 696f 6e20 6f66 2028 2262 6c6f 636b 2229  ion of ("block")
-0000c6c0: 2074 6865 0a20 2020 2020 2020 2020 2020   the.           
-0000c6d0: 2020 2020 2072 656d 6169 6e64 6572 206f       remainder o
-0000c6e0: 6620 7468 6520 7079 7468 6f6e 2063 6f64  f the python cod
-0000c6f0: 6520 756e 7469 6c20 7468 6520 7175 6963  e until the quic
-0000c700: 6b70 6c6f 7428 2920 7769 6e64 6f77 2069  kplot() window i
-0000c710: 7320 636c 6f73 6564 2e0a 2020 2020 2020  s closed..      
-0000c720: 2020 2020 2020 2020 2020 4966 2046 616c            If Fal
-0000c730: 7365 2c20 7468 6520 7769 6e64 6f77 2077  se, the window w
-0000c740: 696c 6c20 6265 206f 7065 6e65 6420 616e  ill be opened an
-0000c750: 6420 636f 6465 2077 696c 6c20 636f 6e74  d code will cont
-0000c760: 696e 7565 2074 6f20 7275 6e2e 0a20 2020  inue to run..   
-0000c770: 2020 2020 2020 2020 207a 6f6f 6d5f 6661           zoom_fa
-0000c780: 6374 6f72 3a20 5365 7473 2074 6865 2073  ctor: Sets the s
-0000c790: 6361 6c69 6e67 2066 6163 746f 7220 7768  caling factor wh
-0000c7a0: 656e 207a 6f6f 6d69 6e67 2074 6865 2071  en zooming the q
-0000c7b0: 7569 636b 706c 6f74 2077 696e 646f 7720  uickplot window 
-0000c7c0: 7769 7468 2074 6865 0a20 2020 2020 2020  with the.       
-0000c7d0: 2020 2020 2020 2020 206d 6f75 7365 7768           mousewh
-0000c7e0: 6565 6c2f 7472 6163 6b70 6164 2e0a 2020  eel/trackpad..  
-0000c7f0: 2020 2020 2020 2020 2020 696e 7465 7261            intera
-0000c800: 6374 6976 655f 7a6f 6f6d 3a20 456e 6162  ctive_zoom: Enab
-0000c810: 6c65 7320 7573 696e 6720 6d6f 7573 6577  les using mousew
-0000c820: 6865 656c 2f74 7261 636b 7061 6420 746f  heel/trackpad to
-0000c830: 207a 6f6f 6d2e 0a20 2020 2020 2020 2020   zoom..         
-0000c840: 2020 2066 6f6e 7473 697a 653a 2066 6f72     fontsize: for
-0000c850: 206c 6162 656c 732e 0a20 2020 2020 2020   labels..       
-0000c860: 2020 2020 206c 6179 6572 735f 6578 636c       layers_excl
-0000c870: 7564 6564 3a20 6c69 7374 206f 6620 6c61  uded: list of la
-0000c880: 7965 7273 2074 6f20 6578 636c 7564 652e  yers to exclude.
-0000c890: 0a20 2020 2020 2020 2020 2020 206c 6179  .            lay
-0000c8a0: 6572 5f76 6965 7773 3a20 6c61 7965 725f  er_views: layer_
-0000c8b0: 7669 6577 7320 636f 6c6f 7273 206c 6f61  views colors loa
-0000c8c0: 6465 6420 6672 6f6d 204b 6c61 796f 7574  ded from Klayout
-0000c8d0: 2e0a 2020 2020 2020 2020 2020 2020 6d69  ..            mi
-0000c8e0: 6e5f 6173 7065 6374 3a20 6d69 6e69 6d75  n_aspect: minimu
-0000c8f0: 6d20 6173 7065 6374 2072 6174 696f 2e0a  m aspect ratio..
-0000c900: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-0000c910: 2020 2020 6672 6f6d 2067 6473 6661 6374      from gdsfact
-0000c920: 6f72 792e 7175 6963 6b70 6c6f 7474 6572  ory.quickplotter
-0000c930: 2069 6d70 6f72 7420 7175 6963 6b70 6c6f   import quickplo
-0000c940: 740a 0a20 2020 2020 2020 2071 7569 636b  t..        quick
-0000c950: 706c 6f74 2873 656c 662c 202a 2a6b 7761  plot(self, **kwa
-0000c960: 7267 7329 0a0a 2020 2020 6465 6620 706c  rgs)..    def pl
-0000c970: 6f74 2873 656c 662c 2070 6c6f 7474 6572  ot(self, plotter
-0000c980: 3a20 4f70 7469 6f6e 616c 5b50 6c6f 7474  : Optional[Plott
-0000c990: 6572 5d20 3d20 4e6f 6e65 2c20 2a2a 6b77  er] = None, **kw
-0000c9a0: 6172 6773 2920 2d3e 204e 6f6e 653a 0a20  args) -> None:. 
-0000c9b0: 2020 2020 2020 2022 2222 5265 7475 726e         """Return
-0000c9c0: 7320 636f 6d70 6f6e 656e 7420 706c 6f74  s component plot
-0000c9d0: 2075 7369 6e67 206b 6c61 796f 7574 2c20   using klayout, 
-0000c9e0: 6d61 7470 6c6f 746c 6962 2c20 686f 6c6f  matplotlib, holo
-0000c9f0: 7669 6577 7320 6f72 2071 742e 0a0a 2020  views or qt...  
-0000ca00: 2020 2020 2020 5765 2072 6563 6f6d 6d65        We recomme
-0000ca10: 6e64 2075 7369 6e67 206b 6c61 796f 7574  nd using klayout
-0000ca20: 2e0a 0a20 2020 2020 2020 2041 7267 733a  ...        Args:
-0000ca30: 0a20 2020 2020 2020 2020 2020 2070 6c6f  .            plo
-0000ca40: 7474 6572 3a20 706c 6f74 2062 6163 6b65  tter: plot backe
-0000ca50: 6e64 2028 2768 6f6c 6f76 6965 7773 272c  nd ('holoviews',
-0000ca60: 2027 6d61 7470 6c6f 746c 6962 272c 2027   'matplotlib', '
-0000ca70: 7174 272c 2027 6b6c 6179 6f75 7427 292e  qt', 'klayout').
-0000ca80: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-0000ca90: 2020 2020 2070 6c6f 7474 6572 203d 2070       plotter = p
-0000caa0: 6c6f 7474 6572 206f 7220 434f 4e46 2e67  lotter or CONF.g
-0000cab0: 6574 2822 706c 6f74 7465 7222 2c20 226d  et("plotter", "m
-0000cac0: 6174 706c 6f74 6c69 6222 290a 0a20 2020  atplotlib")..   
-0000cad0: 2020 2020 2069 6620 706c 6f74 7465 7220       if plotter 
-0000cae0: 3d3d 2022 6b6c 6179 6f75 7422 3a0a 2020  == "klayout":.  
-0000caf0: 2020 2020 2020 2020 2020 7365 6c66 2e70            self.p
-0000cb00: 6c6f 745f 6b6c 6179 6f75 7428 290a 2020  lot_klayout().  
-0000cb10: 2020 2020 2020 2020 2020 7265 7475 726e            return
-0000cb20: 0a0a 2020 2020 2020 2020 656c 6966 2070  ..        elif p
-0000cb30: 6c6f 7474 6572 203d 3d20 226d 6174 706c  lotter == "matpl
-0000cb40: 6f74 6c69 6222 3a0a 2020 2020 2020 2020  otlib":.        
-0000cb50: 2020 2020 6672 6f6d 2067 6473 6661 6374      from gdsfact
-0000cb60: 6f72 792e 7175 6963 6b70 6c6f 7474 6572  ory.quickplotter
-0000cb70: 2069 6d70 6f72 7420 7175 6963 6b70 6c6f   import quickplo
-0000cb80: 740a 0a20 2020 2020 2020 2020 2020 2071  t..            q
-0000cb90: 7569 636b 706c 6f74 2873 656c 662c 202a  uickplot(self, *
-0000cba0: 2a6b 7761 7267 7329 0a20 2020 2020 2020  *kwargs).       
-0000cbb0: 2020 2020 2072 6574 7572 6e0a 0a20 2020       return..   
-0000cbc0: 2020 2020 2065 6c69 6620 706c 6f74 7465       elif plotte
-0000cbd0: 7220 3d3d 2022 686f 6c6f 7669 6577 7322  r == "holoviews"
-0000cbe0: 3a0a 2020 2020 2020 2020 2020 2020 7472  :.            tr
-0000cbf0: 793a 0a20 2020 2020 2020 2020 2020 2020  y:.             
-0000cc00: 2020 2069 6d70 6f72 7420 686f 6c6f 7669     import holovi
-0000cc10: 6577 7320 6173 2068 760a 0a20 2020 2020  ews as hv..     
-0000cc20: 2020 2020 2020 2020 2020 2068 762e 6578             hv.ex
-0000cc30: 7465 6e73 696f 6e28 2262 6f6b 6568 2229  tension("bokeh")
-0000cc40: 0a20 2020 2020 2020 2020 2020 2065 7863  .            exc
-0000cc50: 6570 7420 496d 706f 7274 4572 726f 7220  ept ImportError 
-0000cc60: 6173 2065 3a0a 2020 2020 2020 2020 2020  as e:.          
-0000cc70: 2020 2020 2020 7072 696e 7428 2279 6f75        print("you
-0000cc80: 206e 6565 6420 746f 2060 7069 7020 696e   need to `pip in
-0000cc90: 7374 616c 6c20 686f 6c6f 7669 6577 7360  stall holoviews`
-0000cca0: 2229 0a20 2020 2020 2020 2020 2020 2020  ").             
-0000ccb0: 2020 2072 6169 7365 2065 0a20 2020 2020     raise e.     
-0000ccc0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-0000ccd0: 6c66 2e70 6c6f 745f 686f 6c6f 7669 6577  lf.plot_holoview
-0000cce0: 7328 2a2a 6b77 6172 6773 290a 0a20 2020  s(**kwargs)..   
-0000ccf0: 2020 2020 2065 6c69 6620 706c 6f74 7465       elif plotte
-0000cd00: 7220 3d3d 2022 7174 223a 0a20 2020 2020  r == "qt":.     
-0000cd10: 2020 2020 2020 2066 726f 6d20 6764 7366         from gdsf
-0000cd20: 6163 746f 7279 2e71 7569 636b 706c 6f74  actory.quickplot
-0000cd30: 7465 7220 696d 706f 7274 2071 7569 636b  ter import quick
-0000cd40: 706c 6f74 320a 0a20 2020 2020 2020 2020  plot2..         
-0000cd50: 2020 2071 7569 636b 706c 6f74 3228 7365     quickplot2(se
-0000cd60: 6c66 290a 2020 2020 2020 2020 2020 2020  lf).            
-0000cd70: 7265 7475 726e 0a20 2020 2020 2020 2065  return.        e
-0000cd80: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-0000cd90: 2072 6169 7365 2056 616c 7565 4572 726f   raise ValueErro
-0000cda0: 7228 6622 7b70 6c6f 7474 6572 2172 7d20  r(f"{plotter!r} 
-0000cdb0: 6e6f 7420 696e 207b 506c 6f74 7465 727d  not in {Plotter}
-0000cdc0: 2229 0a0a 2020 2020 6465 6620 706c 6f74  ")..    def plot
-0000cdd0: 5f68 6f6c 6f76 6965 7773 280a 2020 2020  _holoviews(.    
-0000cde0: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
-0000cdf0: 2020 6c61 7965 7273 5f65 7863 6c75 6465    layers_exclude
-0000ce00: 643a 204f 7074 696f 6e61 6c5b 4c61 7965  d: Optional[Laye
-0000ce10: 7273 5d20 3d20 4e6f 6e65 2c0a 2020 2020  rs] = None,.    
-0000ce20: 2020 2020 6c61 7965 725f 7669 6577 733a      layer_views:
-0000ce30: 204f 7074 696f 6e61 6c5b 4c61 7965 7256   Optional[LayerV
-0000ce40: 6965 7773 5d20 3d20 4e6f 6e65 2c0a 2020  iews] = None,.  
-0000ce50: 2020 2020 2020 6d69 6e5f 6173 7065 6374        min_aspect
-0000ce60: 3a20 666c 6f61 7420 3d20 302e 3235 2c0a  : float = 0.25,.
-0000ce70: 2020 2020 2020 2020 7061 6464 696e 673a          padding:
-0000ce80: 2066 6c6f 6174 203d 2030 2e35 2c0a 2020   float = 0.5,.  
-0000ce90: 2020 293a 0a20 2020 2020 2020 2022 2222    ):.        """
-0000cea0: 506c 6f74 2063 6f6d 706f 6e65 6e74 2069  Plot component i
-0000ceb0: 6e20 686f 6c6f 7669 6577 732e 0a0a 2020  n holoviews...  
-0000cec0: 2020 2020 2020 4172 6773 3a0a 2020 2020        Args:.    
-0000ced0: 2020 2020 2020 2020 6c61 7965 7273 5f65          layers_e
-0000cee0: 7863 6c75 6465 643a 206c 6973 7420 6f66  xcluded: list of
-0000cef0: 206c 6179 6572 7320 746f 2065 7863 6c75   layers to exclu
-0000cf00: 6465 2e0a 2020 2020 2020 2020 2020 2020  de..            
-0000cf10: 6c61 7965 725f 7669 6577 733a 206c 6179  layer_views: lay
-0000cf20: 6572 5f76 6965 7773 2063 6f6c 6f72 7320  er_views colors 
-0000cf30: 6c6f 6164 6564 2066 726f 6d20 4b6c 6179  loaded from Klay
-0000cf40: 6f75 742e 0a20 2020 2020 2020 2020 2020  out..           
-0000cf50: 206d 696e 5f61 7370 6563 743a 206d 696e   min_aspect: min
-0000cf60: 696d 756d 2061 7370 6563 7420 7261 7469  imum aspect rati
-0000cf70: 6f2e 0a20 2020 2020 2020 2020 2020 2070  o..            p
-0000cf80: 6164 6469 6e67 3a20 6172 6f75 6e64 2062  adding: around b
-0000cf90: 6f75 6e64 696e 6720 626f 782e 0a0a 2020  ounding box...  
-0000cfa0: 2020 2020 2020 5265 7475 726e 733a 0a20        Returns:. 
-0000cfb0: 2020 2020 2020 2020 2020 2048 6f6c 6f76             Holov
-0000cfc0: 6965 7773 204f 7665 726c 6179 2074 6f20  iews Overlay to 
-0000cfd0: 6469 7370 6c61 7920 616c 6c20 706f 6c79  display all poly
-0000cfe0: 676f 6e73 2e0a 2020 2020 2020 2020 2222  gons..        ""
-0000cff0: 220a 2020 2020 2020 2020 6672 6f6d 2067  ".        from g
-0000d000: 6473 6661 6374 6f72 792e 6164 645f 7069  dsfactory.add_pi
-0000d010: 6e73 2069 6d70 6f72 7420 6765 745f 7069  ns import get_pi
-0000d020: 6e5f 7472 6961 6e67 6c65 5f70 6f6c 7967  n_triangle_polyg
-0000d030: 6f6e 5f74 6970 0a20 2020 2020 2020 2066  on_tip.        f
-0000d040: 726f 6d20 6764 7366 6163 746f 7279 2e67  rom gdsfactory.g
-0000d050: 656e 6572 6963 5f74 6563 6820 696d 706f  eneric_tech impo
-0000d060: 7274 204c 4159 4552 5f56 4945 5753 0a0a  rt LAYER_VIEWS..
-0000d070: 2020 2020 2020 2020 6966 206c 6179 6572          if layer
-0000d080: 5f76 6965 7773 2069 7320 4e6f 6e65 3a0a  _views is None:.
-0000d090: 2020 2020 2020 2020 2020 2020 6c61 7965              laye
-0000d0a0: 725f 7669 6577 7320 3d20 4c41 5945 525f  r_views = LAYER_
-0000d0b0: 5649 4557 530a 0a20 2020 2020 2020 2074  VIEWS..        t
-0000d0c0: 7279 3a0a 2020 2020 2020 2020 2020 2020  ry:.            
-0000d0d0: 696d 706f 7274 2068 6f6c 6f76 6965 7773  import holoviews
-0000d0e0: 2061 7320 6876 0a0a 2020 2020 2020 2020   as hv..        
-0000d0f0: 2020 2020 6876 2e65 7874 656e 7369 6f6e      hv.extension
-0000d100: 2822 626f 6b65 6822 290a 2020 2020 2020  ("bokeh").      
-0000d110: 2020 6578 6365 7074 2049 6d70 6f72 7445    except ImportE
-0000d120: 7272 6f72 2061 7320 653a 0a20 2020 2020  rror as e:.     
-0000d130: 2020 2020 2020 2070 7269 6e74 2822 796f         print("yo
-0000d140: 7520 6e65 6564 2074 6f20 6070 6970 2069  u need to `pip i
-0000d150: 6e73 7461 6c6c 2068 6f6c 6f76 6965 7773  nstall holoviews
-0000d160: 6022 290a 2020 2020 2020 2020 2020 2020  `").            
-0000d170: 7261 6973 6520 650a 0a20 2020 2020 2020  raise e..       
-0000d180: 2073 656c 662e 5f62 625f 7661 6c69 6420   self._bb_valid 
-0000d190: 3d20 4661 6c73 6520 2023 2072 6563 6f6d  = False  # recom
-0000d1a0: 7075 7465 2074 6865 2062 6f75 6e64 696e  pute the boundin
-0000d1b0: 6720 626f 780a 2020 2020 2020 2020 6220  g box.        b 
-0000d1c0: 3d20 7365 6c66 2e62 626f 7820 2b20 2828  = self.bbox + ((
-0000d1d0: 2d70 6164 6469 6e67 2c20 2d70 6164 6469  -padding, -paddi
-0000d1e0: 6e67 292c 2028 7061 6464 696e 672c 2070  ng), (padding, p
-0000d1f0: 6164 6469 6e67 2929 0a20 2020 2020 2020  adding)).       
-0000d200: 2062 203d 206e 702e 6172 7261 7928 622e   b = np.array(b.
-0000d210: 666c 6174 290a 2020 2020 2020 2020 6365  flat).        ce
-0000d220: 6e74 6572 203d 206e 702e 6172 7261 7928  nter = np.array(
-0000d230: 286e 702e 7375 6d28 625b 3a3a 325d 2920  (np.sum(b[::2]) 
-0000d240: 2f20 322c 206e 702e 7375 6d28 625b 313a  / 2, np.sum(b[1:
-0000d250: 3a32 5d29 202f 2032 2929 0a20 2020 2020  :2]) / 2)).     
-0000d260: 2020 2073 697a 6520 3d20 6e70 2e61 7272     size = np.arr
-0000d270: 6179 2828 6e70 2e61 6273 2862 5b32 5d20  ay((np.abs(b[2] 
-0000d280: 2d20 625b 305d 292c 206e 702e 6162 7328  - b[0]), np.abs(
-0000d290: 625b 335d 202d 2062 5b31 5d29 2929 0a20  b[3] - b[1]))). 
-0000d2a0: 2020 2020 2020 2064 7820 3d20 6e70 2e61         dx = np.a
-0000d2b0: 7272 6179 280a 2020 2020 2020 2020 2020  rray(.          
-0000d2c0: 2020 280a 2020 2020 2020 2020 2020 2020    (.            
-0000d2d0: 2020 2020 6e70 2e6d 6178 696d 756d 286d      np.maximum(m
-0000d2e0: 696e 5f61 7370 6563 7420 2a20 7369 7a65  in_aspect * size
-0000d2f0: 5b31 5d2c 2073 697a 655b 305d 2920 2f20  [1], size[0]) / 
-0000d300: 322c 0a20 2020 2020 2020 2020 2020 2020  2,.             
-0000d310: 2020 206e 702e 6d61 7869 6d75 6d28 7369     np.maximum(si
-0000d320: 7a65 5b31 5d2c 206d 696e 5f61 7370 6563  ze[1], min_aspec
-0000d330: 7420 2a20 7369 7a65 5b30 5d29 202f 2032  t * size[0]) / 2
-0000d340: 2c0a 2020 2020 2020 2020 2020 2020 290a  ,.            ).
-0000d350: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-0000d360: 2020 6220 3d20 6e70 2e68 7374 6163 6b28    b = np.hstack(
-0000d370: 2863 656e 7465 7220 2d20 6478 2c20 6365  (center - dx, ce
-0000d380: 6e74 6572 202b 2064 7829 290a 0a20 2020  nter + dx))..   
-0000d390: 2020 2020 2070 6c6f 7473 5f74 6f5f 6f76       plots_to_ov
-0000d3a0: 6572 6c61 7920 3d20 5b5d 0a20 2020 2020  erlay = [].     
-0000d3b0: 2020 206c 6179 6572 735f 6578 636c 7564     layers_exclud
-0000d3c0: 6564 203d 205b 5d20 6966 206c 6179 6572  ed = [] if layer
-0000d3d0: 735f 6578 636c 7564 6564 2069 7320 4e6f  s_excluded is No
-0000d3e0: 6e65 2065 6c73 6520 6c61 7965 7273 5f65  ne else layers_e
-0000d3f0: 7863 6c75 6465 640a 0a20 2020 2020 2020  xcluded..       
-0000d400: 2066 6f72 206c 6179 6572 2c20 706f 6c79   for layer, poly
-0000d410: 676f 6e20 696e 2073 656c 662e 6765 745f  gon in self.get_
-0000d420: 706f 6c79 676f 6e73 2862 795f 7370 6563  polygons(by_spec
-0000d430: 3d54 7275 6529 2e69 7465 6d73 2829 3a0a  =True).items():.
-0000d440: 2020 2020 2020 2020 2020 2020 6966 206c              if l
-0000d450: 6179 6572 2069 6e20 6c61 7965 7273 5f65  ayer in layers_e
-0000d460: 7863 6c75 6465 643a 0a20 2020 2020 2020  xcluded:.       
-0000d470: 2020 2020 2020 2020 2063 6f6e 7469 6e75           continu
-0000d480: 650a 0a20 2020 2020 2020 2020 2020 2074  e..            t
-0000d490: 7279 3a0a 2020 2020 2020 2020 2020 2020  ry:.            
-0000d4a0: 2020 2020 6c61 7965 725f 7669 6577 203d      layer_view =
-0000d4b0: 206c 6179 6572 5f76 6965 7773 2e67 6574   layer_views.get
-0000d4c0: 5f66 726f 6d5f 7475 706c 6528 6c61 7965  _from_tuple(laye
-0000d4d0: 7229 0a20 2020 2020 2020 2020 2020 2065  r).            e
-0000d4e0: 7863 6570 7420 5661 6c75 6545 7272 6f72  xcept ValueError
-0000d4f0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000d500: 2020 6c61 7965 7273 203d 206c 6973 7428    layers = list(
-0000d510: 6c61 7965 725f 7669 6577 732e 6765 745f  layer_views.get_
-0000d520: 6c61 7965 725f 7669 6577 7328 292e 6b65  layer_views().ke
-0000d530: 7973 2829 290a 2020 2020 2020 2020 2020  ys()).          
-0000d540: 2020 2020 2020 7761 726e 696e 6773 2e77        warnings.w
-0000d550: 6172 6e28 6622 7b6c 6179 6572 2172 7d20  arn(f"{layer!r} 
-0000d560: 6e6f 7420 6465 6669 6e65 6420 696e 207b  not defined in {
-0000d570: 6c61 7965 7273 7d22 290a 2020 2020 2020  layers}").      
-0000d580: 2020 2020 2020 2020 2020 6c61 7965 725f            layer_
-0000d590: 7669 6577 203d 204c 6179 6572 5669 6577  view = LayerView
-0000d5a0: 286c 6179 6572 3d6c 6179 6572 290a 2020  (layer=layer).  
-0000d5b0: 2020 2020 2020 2020 2020 2320 544f 444f            # TODO
-0000d5c0: 3a20 4d61 7463 6820 7570 206f 7074 696f  : Match up optio
-0000d5d0: 6e73 2077 6974 6820 4c61 7965 7256 6965  ns with LayerVie
-0000d5e0: 7773 0a20 2020 2020 2020 2020 2020 2070  ws.            p
-0000d5f0: 6c6f 7473 5f74 6f5f 6f76 6572 6c61 792e  lots_to_overlay.
-0000d600: 6170 7065 6e64 280a 2020 2020 2020 2020  append(.        
-0000d610: 2020 2020 2020 2020 6876 2e50 6f6c 7967          hv.Polyg
-0000d620: 6f6e 7328 706f 6c79 676f 6e2c 206c 6162  ons(polygon, lab
-0000d630: 656c 3d73 7472 286c 6179 6572 5f76 6965  el=str(layer_vie
-0000d640: 772e 6e61 6d65 2929 2e6f 7074 7328 0a20  w.name)).opts(. 
-0000d650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d660: 2020 2064 6174 615f 6173 7065 6374 3d31     data_aspect=1
-0000d670: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0000d680: 2020 2020 2020 6672 616d 655f 7769 6474        frame_widt
-0000d690: 683d 3530 302c 0a20 2020 2020 2020 2020  h=500,.         
-0000d6a0: 2020 2020 2020 2020 2020 2079 6c69 6d3d             ylim=
-0000d6b0: 2862 5b31 5d2c 2062 5b33 5d29 2c0a 2020  (b[1], b[3]),.  
-0000d6c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d6d0: 2020 786c 696d 3d28 625b 305d 2c20 625b    xlim=(b[0], b[
-0000d6e0: 325d 292c 0a20 2020 2020 2020 2020 2020  2]),.           
-0000d6f0: 2020 2020 2020 2020 2066 696c 6c5f 636f           fill_co
-0000d700: 6c6f 723d 6c61 7965 725f 7669 6577 2e66  lor=layer_view.f
-0000d710: 696c 6c5f 636f 6c6f 722e 6173 5f72 6762  ill_color.as_rgb
-0000d720: 2829 206f 7220 2222 2c0a 2020 2020 2020  () or "",.      
-0000d730: 2020 2020 2020 2020 2020 2020 2020 6c69                li
-0000d740: 6e65 5f63 6f6c 6f72 3d6c 6179 6572 5f76  ne_color=layer_v
-0000d750: 6965 772e 6672 616d 655f 636f 6c6f 722e  iew.frame_color.
-0000d760: 6173 5f72 6762 2829 206f 7220 2222 2c0a  as_rgb() or "",.
-0000d770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d780: 2020 2020 6669 6c6c 5f61 6c70 6861 3d6c      fill_alpha=l
-0000d790: 6179 6572 5f76 6965 772e 6765 745f 616c  ayer_view.get_al
-0000d7a0: 7068 6128 2920 6f72 2022 222c 0a20 2020  pha() or "",.   
-0000d7b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d7c0: 206c 696e 655f 616c 7068 613d 6c61 7965   line_alpha=laye
-0000d7d0: 725f 7669 6577 2e67 6574 5f61 6c70 6861  r_view.get_alpha
-0000d7e0: 2829 206f 7220 2222 2c0a 2020 2020 2020  () or "",.      
-0000d7f0: 2020 2020 2020 2020 2020 2020 2020 746f                to
-0000d800: 6f6c 733d 5b22 686f 7665 7222 5d2c 0a20  ols=["hover"],. 
-0000d810: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-0000d820: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
-0000d830: 2020 2020 2020 2066 6f72 206e 616d 652c         for name,
-0000d840: 2070 6f72 7420 696e 2073 656c 662e 706f   port in self.po
-0000d850: 7274 732e 6974 656d 7328 293a 0a20 2020  rts.items():.   
-0000d860: 2020 2020 2020 2020 206e 616d 6520 3d20           name = 
-0000d870: 7374 7228 6e61 6d65 290a 2020 2020 2020  str(name).      
-0000d880: 2020 2020 2020 706f 6c79 676f 6e2c 2070        polygon, p
-0000d890: 7469 7020 3d20 6765 745f 7069 6e5f 7472  tip = get_pin_tr
-0000d8a0: 6961 6e67 6c65 5f70 6f6c 7967 6f6e 5f74  iangle_polygon_t
-0000d8b0: 6970 2870 6f72 743d 706f 7274 290a 0a20  ip(port=port).. 
-0000d8c0: 2020 2020 2020 2020 2020 2070 6c6f 7473             plots
-0000d8d0: 5f74 6f5f 6f76 6572 6c61 792e 6170 7065  _to_overlay.appe
-0000d8e0: 6e64 280a 2020 2020 2020 2020 2020 2020  nd(.            
-0000d8f0: 2020 2020 6876 2e50 6f6c 7967 6f6e 7328      hv.Polygons(
-0000d900: 706f 6c79 676f 6e2c 206c 6162 656c 3d6e  polygon, label=n
-0000d910: 616d 6529 2e6f 7074 7328 0a20 2020 2020  ame).opts(.     
-0000d920: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-0000d930: 6174 615f 6173 7065 6374 3d31 2c0a 2020  ata_aspect=1,.  
-0000d940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d950: 2020 6672 616d 655f 7769 6474 683d 3530    frame_width=50
-0000d960: 302c 0a20 2020 2020 2020 2020 2020 2020  0,.             
-0000d970: 2020 2020 2020 2066 696c 6c5f 616c 7068         fill_alph
-0000d980: 613d 302c 0a20 2020 2020 2020 2020 2020  a=0,.           
-0000d990: 2020 2020 2020 2020 2079 6c69 6d3d 2862           ylim=(b
-0000d9a0: 5b31 5d2c 2062 5b33 5d29 2c0a 2020 2020  [1], b[3]),.    
-0000d9b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d9c0: 786c 696d 3d28 625b 305d 2c20 625b 325d  xlim=(b[0], b[2]
-0000d9d0: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
-0000d9e0: 2020 2020 2020 2063 6f6c 6f72 3d22 7265         color="re
-0000d9f0: 6422 2c0a 2020 2020 2020 2020 2020 2020  d",.            
-0000da00: 2020 2020 2020 2020 6c69 6e65 5f61 6c70          line_alp
-0000da10: 6861 3d6c 6179 6572 5f76 6965 772e 6765  ha=layer_view.ge
-0000da20: 745f 616c 7068 6128 2920 6f72 2022 222c  t_alpha() or "",
-0000da30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000da40: 2020 2020 2074 6f6f 6c73 3d5b 2268 6f76       tools=["hov
-0000da50: 6572 225d 2c0a 2020 2020 2020 2020 2020  er"],.          
-0000da60: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-0000da70: 2020 2020 2020 2020 2a20 6876 2e54 6578          * hv.Tex
-0000da80: 7428 7074 6970 5b30 5d2c 2070 7469 705b  t(ptip[0], ptip[
-0000da90: 315d 2c20 6e61 6d65 290a 2020 2020 2020  1], name).      
-0000daa0: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
-0000dab0: 2072 6574 7572 6e20 6876 2e4f 7665 726c   return hv.Overl
-0000dac0: 6179 2870 6c6f 7473 5f74 6f5f 6f76 6572  ay(plots_to_over
-0000dad0: 6c61 7929 2e6f 7074 7328 0a20 2020 2020  lay).opts(.     
-0000dae0: 2020 2020 2020 2073 686f 775f 6c65 6765         show_lege
-0000daf0: 6e64 3d54 7275 652c 2073 6861 7265 645f  nd=True, shared_
-0000db00: 6178 6573 3d46 616c 7365 2c20 796c 696d  axes=False, ylim
-0000db10: 3d28 625b 315d 2c20 625b 335d 292c 2078  =(b[1], b[3]), x
-0000db20: 6c69 6d3d 2862 5b30 5d2c 2062 5b32 5d29  lim=(b[0], b[2])
-0000db30: 0a20 2020 2020 2020 2029 0a0a 2020 2020  .        )..    
-0000db40: 6465 6620 7368 6f77 280a 2020 2020 2020  def show(.      
-0000db50: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
-0000db60: 7368 6f77 5f70 6f72 7473 3a20 626f 6f6c  show_ports: bool
-0000db70: 203d 2046 616c 7365 2c0a 2020 2020 2020   = False,.      
-0000db80: 2020 7368 6f77 5f73 7562 706f 7274 733a    show_subports:
-0000db90: 2062 6f6f 6c20 3d20 4661 6c73 652c 0a20   bool = False,. 
-0000dba0: 2020 2020 2020 2070 6f72 745f 6d61 726b         port_mark
-0000dbb0: 6572 5f6c 6179 6572 3a20 4c61 7965 7220  er_layer: Layer 
-0000dbc0: 3d20 2831 2c20 3130 292c 0a20 2020 2020  = (1, 10),.     
-0000dbd0: 2020 202a 2a6b 7761 7267 732c 0a20 2020     **kwargs,.   
-0000dbe0: 2029 202d 3e20 4e6f 6e65 3a0a 2020 2020   ) -> None:.    
-0000dbf0: 2020 2020 2222 2253 686f 7720 636f 6d70      """Show comp
-0000dc00: 6f6e 656e 7420 696e 204b 4c61 796f 7574  onent in KLayout
-0000dc10: 2e0a 0a20 2020 2020 2020 2072 6574 7572  ...        retur
-0000dc20: 6e73 2061 2063 6f70 7920 6f66 2074 6865  ns a copy of the
-0000dc30: 2043 6f6d 706f 6e65 6e74 2c20 736f 2074   Component, so t
-0000dc40: 6865 206f 7269 6769 6e61 6c20 636f 6d70  he original comp
-0000dc50: 6f6e 656e 7420 7265 6d61 696e 7320 696e  onent remains in
-0000dc60: 7461 6374 2e0a 2020 2020 2020 2020 7769  tact..        wi
-0000dc70: 7468 2070 696e 7320 6d61 726b 6572 7320  th pins markers 
-0000dc80: 6f6e 2065 6163 6820 706f 7274 2073 686f  on each port sho
-0000dc90: 775f 706f 7274 7320 3d20 5472 7565 2c20  w_ports = True, 
-0000dca0: 616e 6420 6f70 7469 6f6e 616c 6c79 2061  and optionally a
-0000dcb0: 6c73 6f0a 2020 2020 2020 2020 7468 6520  lso.        the 
-0000dcc0: 706f 7274 7320 6672 6f6d 2074 6865 2072  ports from the r
-0000dcd0: 6566 6572 656e 6365 7320 2873 686f 775f  eferences (show_
-0000dce0: 7375 6270 6f72 7473 3d54 7275 6529 0a0a  subports=True)..
-0000dcf0: 2020 2020 2020 2020 4172 6773 3a0a 2020          Args:.  
-0000dd00: 2020 2020 2020 2020 2020 7368 6f77 5f70            show_p
-0000dd10: 6f72 7473 3a20 7368 6f77 7320 636f 6d70  orts: shows comp
-0000dd20: 6f6e 656e 7420 7769 7468 2070 6f72 7420  onent with port 
-0000dd30: 6d61 726b 6572 7320 616e 6420 6c61 6265  markers and labe
-0000dd40: 6c73 2e0a 2020 2020 2020 2020 2020 2020  ls..            
-0000dd50: 7368 6f77 5f73 7562 706f 7274 733a 2061  show_subports: a
-0000dd60: 6464 2070 6f72 7473 206d 6172 6b65 7273  dd ports markers
-0000dd70: 2061 6e64 206c 6162 656c 7320 746f 2072   and labels to r
-0000dd80: 6566 6572 656e 6365 732e 0a20 2020 2020  eferences..     
-0000dd90: 2020 2020 2020 2070 6f72 745f 6d61 726b         port_mark
-0000dda0: 6572 5f6c 6179 6572 3a20 666f 7220 7468  er_layer: for th
-0000ddb0: 6520 706f 7274 732e 0a0a 2020 2020 2020  e ports...      
-0000ddc0: 2020 4b65 7977 6f72 6420 4172 6773 3a0a    Keyword Args:.
-0000ddd0: 2020 2020 2020 2020 2020 2020 6764 7370              gdsp
-0000dde0: 6174 683a 2047 4453 2066 696c 6520 7061  ath: GDS file pa
-0000ddf0: 7468 2074 6f20 7772 6974 6520 746f 2e0a  th to write to..
-0000de00: 2020 2020 2020 2020 2020 2020 6764 7364              gdsd
-0000de10: 6972 3a20 6469 7265 6374 6f72 7920 666f  ir: directory fo
-0000de20: 7220 7468 6520 4744 5320 6669 6c65 2e20  r the GDS file. 
-0000de30: 4465 6661 756c 7473 2074 6f20 2f74 6d70  Defaults to /tmp
-0000de40: 2f2e 0a20 2020 2020 2020 2020 2020 2075  /..            u
-0000de50: 6e69 743a 2075 6e69 7420 7369 7a65 2066  nit: unit size f
-0000de60: 6f72 206f 626a 6563 7473 2069 6e20 6c69  or objects in li
-0000de70: 6272 6172 792e 2031 756d 2062 7920 6465  brary. 1um by de
-0000de80: 6661 756c 742e 0a20 2020 2020 2020 2020  fault..         
-0000de90: 2020 2070 7265 6369 7369 6f6e 3a20 666f     precision: fo
-0000dea0: 7220 6f62 6a65 6374 2064 696d 656e 7369  r object dimensi
-0000deb0: 6f6e 7320 696e 2074 6865 206c 6962 7261  ons in the libra
-0000dec0: 7279 2028 6d29 2e20 316e 6d20 6279 2064  ry (m). 1nm by d
-0000ded0: 6566 6175 6c74 2e0a 2020 2020 2020 2020  efault..        
-0000dee0: 2020 2020 7469 6d65 7374 616d 703a 2044      timestamp: D
-0000def0: 6566 6175 6c74 7320 746f 2032 3031 392d  efaults to 2019-
-0000df00: 3130 2d32 352e 2049 6620 4e6f 6e65 2075  10-25. If None u
-0000df10: 7365 7320 6375 7272 656e 7420 7469 6d65  ses current time
-0000df20: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
-0000df30: 2020 2020 2020 6672 6f6d 2067 6473 6661        from gdsfa
-0000df40: 6374 6f72 792e 6164 645f 7069 6e73 2069  ctory.add_pins i
-0000df50: 6d70 6f72 7420 6164 645f 7069 6e73 5f74  mport add_pins_t
-0000df60: 7269 616e 676c 650a 2020 2020 2020 2020  riangle.        
-0000df70: 6672 6f6d 2067 6473 6661 6374 6f72 792e  from gdsfactory.
-0000df80: 7368 6f77 2069 6d70 6f72 7420 7368 6f77  show import show
-0000df90: 0a0a 2020 2020 2020 2020 636f 6d70 6f6e  ..        compon
-0000dfa0: 656e 7420 3d20 280a 2020 2020 2020 2020  ent = (.        
-0000dfb0: 2020 2020 7365 6c66 2e61 6464 5f70 696e      self.add_pin
-0000dfc0: 735f 7472 6961 6e67 6c65 2870 6f72 745f  s_triangle(port_
-0000dfd0: 6d61 726b 6572 5f6c 6179 6572 3d70 6f72  marker_layer=por
-0000dfe0: 745f 6d61 726b 6572 5f6c 6179 6572 290a  t_marker_layer).
-0000dff0: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-0000e000: 686f 775f 706f 7274 730a 2020 2020 2020  how_ports.      
-0000e010: 2020 2020 2020 656c 7365 2073 656c 660a        else self.
-0000e020: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
-0000e030: 2020 2069 6620 7368 6f77 5f73 7562 706f     if show_subpo
-0000e040: 7274 733a 0a20 2020 2020 2020 2020 2020  rts:.           
-0000e050: 2063 6f6d 706f 6e65 6e74 203d 2073 656c   component = sel
-0000e060: 662e 636f 7079 2829 0a20 2020 2020 2020  f.copy().       
-0000e070: 2020 2020 2063 6f6d 706f 6e65 6e74 2e6e       component.n
-0000e080: 616d 6520 3d20 7365 6c66 2e6e 616d 650a  ame = self.name.
-0000e090: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-0000e0a0: 7265 6665 7265 6e63 6520 696e 2063 6f6d  reference in com
-0000e0b0: 706f 6e65 6e74 2e72 6566 6572 656e 6365  ponent.reference
-0000e0c0: 733a 0a20 2020 2020 2020 2020 2020 2020  s:.             
-0000e0d0: 2020 2069 6620 6973 696e 7374 616e 6365     if isinstance
-0000e0e0: 2863 6f6d 706f 6e65 6e74 2c20 436f 6d70  (component, Comp
-0000e0f0: 6f6e 656e 7452 6566 6572 656e 6365 293a  onentReference):
-0000e100: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000e110: 2020 2020 2061 6464 5f70 696e 735f 7472       add_pins_tr
-0000e120: 6961 6e67 6c65 280a 2020 2020 2020 2020  iangle(.        
-0000e130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e140: 636f 6d70 6f6e 656e 743d 636f 6d70 6f6e  component=compon
-0000e150: 656e 742c 0a20 2020 2020 2020 2020 2020  ent,.           
-0000e160: 2020 2020 2020 2020 2020 2020 2072 6566               ref
-0000e170: 6572 656e 6365 3d72 6566 6572 656e 6365  erence=reference
-0000e180: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-0000e190: 2020 2020 2020 2020 2020 6c61 7965 723d            layer=
-0000e1a0: 706f 7274 5f6d 6172 6b65 725f 6c61 7965  port_marker_laye
-0000e1b0: 722c 0a20 2020 2020 2020 2020 2020 2020  r,.             
-0000e1c0: 2020 2020 2020 2029 0a0a 2020 2020 2020         )..      
-0000e1d0: 2020 7368 6f77 2863 6f6d 706f 6e65 6e74    show(component
-0000e1e0: 2c20 2a2a 6b77 6172 6773 290a 0a20 2020  , **kwargs)..   
-0000e1f0: 2064 6566 205f 7772 6974 655f 6c69 6272   def _write_libr
-0000e200: 6172 7928 0a20 2020 2020 2020 2073 656c  ary(.        sel
-0000e210: 662c 0a20 2020 2020 2020 2067 6473 7061  f,.        gdspa
-0000e220: 7468 3a20 4f70 7469 6f6e 616c 5b50 6174  th: Optional[Pat
-0000e230: 6854 7970 655d 203d 204e 6f6e 652c 0a20  hType] = None,. 
-0000e240: 2020 2020 2020 2067 6473 6469 723a 204f         gdsdir: O
-0000e250: 7074 696f 6e61 6c5b 5061 7468 5479 7065  ptional[PathType
-0000e260: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2020  ] = None,.      
-0000e270: 2020 7469 6d65 7374 616d 703a 204f 7074    timestamp: Opt
-0000e280: 696f 6e61 6c5b 6461 7465 7469 6d65 2e64  ional[datetime.d
-0000e290: 6174 6574 696d 655d 203d 205f 7469 6d65  atetime] = _time
-0000e2a0: 7374 616d 7032 3031 392c 0a20 2020 2020  stamp2019,.     
-0000e2b0: 2020 206c 6f67 6769 6e67 3a20 626f 6f6c     logging: bool
-0000e2c0: 203d 2054 7275 652c 0a20 2020 2020 2020   = True,.       
-0000e2d0: 2077 6974 685f 6f61 7369 733a 2062 6f6f   with_oasis: boo
-0000e2e0: 6c20 3d20 4661 6c73 652c 0a20 2020 2020  l = False,.     
-0000e2f0: 2020 202a 2a6b 7761 7267 732c 0a20 2020     **kwargs,.   
-0000e300: 2029 202d 3e20 5061 7468 3a0a 2020 2020   ) -> Path:.    
-0000e310: 2020 2020 2222 2257 7269 7465 2063 6f6d      """Write com
-0000e320: 706f 6e65 6e74 2074 6f20 4744 5320 6f72  ponent to GDS or
-0000e330: 204f 4153 4953 2061 6e64 2072 6574 7572   OASIS and retur
-0000e340: 6e73 2067 6473 7061 7468 2e0a 0a20 2020  ns gdspath...   
-0000e350: 2020 2020 2041 7267 733a 0a20 2020 2020       Args:.     
-0000e360: 2020 2020 2020 2067 6473 7061 7468 3a20         gdspath: 
-0000e370: 4744 5320 6669 6c65 2070 6174 6820 746f  GDS file path to
-0000e380: 2077 7269 7465 2074 6f2e 0a20 2020 2020   write to..     
-0000e390: 2020 2020 2020 2067 6473 6469 723a 2064         gdsdir: d
-0000e3a0: 6972 6563 746f 7279 2066 6f72 2074 6865  irectory for the
-0000e3b0: 2047 4453 2066 696c 652e 2044 6566 6175   GDS file. Defau
-0000e3c0: 6c74 7320 746f 202f 746d 702f 7261 6e64  lts to /tmp/rand
-0000e3d0: 6f6d 4669 6c65 2f67 6473 6661 6374 6f72  omFile/gdsfactor
-0000e3e0: 792e 0a20 2020 2020 2020 2020 2020 2074  y..            t
-0000e3f0: 696d 6573 7461 6d70 3a20 4465 6661 756c  imestamp: Defaul
-0000e400: 7473 2074 6f20 3230 3139 2d31 302d 3235  ts to 2019-10-25
-0000e410: 2066 6f72 2063 6f6e 7369 7374 656e 7420   for consistent 
-0000e420: 6861 7368 2e0a 2020 2020 2020 2020 2020  hash..          
-0000e430: 2020 2020 2020 4966 204e 6f6e 6520 7573        If None us
-0000e440: 6573 2063 7572 7265 6e74 2074 696d 652e  es current time.
-0000e450: 0a20 2020 2020 2020 2020 2020 206c 6f67  .            log
-0000e460: 6769 6e67 3a20 6469 7361 626c 6520 4744  ging: disable GD
-0000e470: 5320 7061 7468 206c 6f67 6769 6e67 2c20  S path logging, 
-0000e480: 666f 7220 6578 616d 706c 6520 666f 7220  for example for 
-0000e490: 7368 6f77 696e 6720 6974 2069 6e20 4b4c  showing it in KL
-0000e4a0: 6179 6f75 742e 0a20 2020 2020 2020 2020  ayout..         
-0000e4b0: 2020 2077 6974 685f 6f61 7369 733a 2049     with_oasis: I
-0000e4c0: 6620 5472 7565 2c20 6669 6c65 2077 696c  f True, file wil
-0000e4d0: 6c20 6265 2077 7269 7474 656e 2074 6f20  l be written to 
-0000e4e0: 4f41 5349 532e 204f 7468 6572 7769 7365  OASIS. Otherwise
-0000e4f0: 2c20 6669 6c65 2077 696c 6c20 6265 2077  , file will be w
-0000e500: 7269 7474 656e 2074 6f20 4744 532e 0a0a  ritten to GDS...
-0000e510: 2020 2020 2020 2020 4b65 7977 6f72 6420          Keyword 
-0000e520: 4172 6773 3a0a 2020 2020 2020 2020 2020  Args:.          
-0000e530: 2020 4b65 7977 6f72 6420 6172 6775 6d65    Keyword argume
-0000e540: 6e74 7320 7769 6c6c 206f 7665 7272 6964  nts will overrid
-0000e550: 6520 7468 6520 6163 7469 7665 2050 444b  e the active PDK
-0000e560: 2773 2064 6566 6175 6c74 2047 6473 5772  's default GdsWr
-0000e570: 6974 6553 6574 7469 6e67 7320 616e 6420  iteSettings and 
-0000e580: 4f61 7369 7357 7269 7465 5365 7474 696e  OasisWriteSettin
-0000e590: 6773 2e0a 0a20 2020 2020 2020 2020 2020  gs...           
-0000e5a0: 2047 6473 2073 6574 7469 6e67 733a 0a20   Gds settings:. 
-0000e5b0: 2020 2020 2020 2020 2020 2020 2020 2075                 u
-0000e5c0: 6e69 743a 2075 6e69 7420 7369 7a65 2066  nit: unit size f
-0000e5d0: 6f72 206f 626a 6563 7473 2069 6e20 6c69  or objects in li
-0000e5e0: 6272 6172 792e 2031 756d 2062 7920 6465  brary. 1um by de
-0000e5f0: 6661 756c 742e 0a20 2020 2020 2020 2020  fault..         
-0000e600: 2020 2020 2020 2070 7265 6369 7369 6f6e         precision
-0000e610: 3a20 666f 7220 6469 6d65 6e73 696f 6e73  : for dimensions
-0000e620: 2069 6e20 7468 6520 6c69 6272 6172 7920   in the library 
-0000e630: 286d 292e 2031 6e6d 2062 7920 6465 6661  (m). 1nm by defa
-0000e640: 756c 742e 0a20 2020 2020 2020 2020 2020  ult..           
-0000e650: 2020 2020 206f 6e5f 6475 706c 6963 6174       on_duplicat
-0000e660: 655f 6365 6c6c 3a20 7370 6563 6966 7920  e_cell: specify 
-0000e670: 686f 7720 746f 2072 6573 6f6c 7665 2064  how to resolve d
-0000e680: 7570 6c69 6361 7465 2d6e 616d 6564 2063  uplicate-named c
-0000e690: 656c 6c73 2e20 4368 6f6f 7365 206f 6e65  ells. Choose one
-0000e6a0: 206f 6620 7468 6520 666f 6c6c 6f77 696e   of the followin
-0000e6b0: 673a 0a20 2020 2020 2020 2020 2020 2020  g:.             
-0000e6c0: 2020 2020 2020 2022 7761 726e 2220 2864         "warn" (d
-0000e6d0: 6566 6175 6c74 293a 206f 7665 7277 7269  efault): overwri
-0000e6e0: 7465 2061 6c6c 2064 7570 6c69 6361 7465  te all duplicate
-0000e6f0: 2063 656c 6c73 2077 6974 6820 6f6e 6520   cells with one 
-0000e700: 6f66 2074 6865 2064 7570 6c69 6361 7465  of the duplicate
-0000e710: 7320 2861 7262 6974 7261 7269 6c79 292e  s (arbitrarily).
-0000e720: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000e730: 2020 2020 2022 6572 726f 7222 3a20 7468       "error": th
-0000e740: 726f 7720 6120 5661 6c75 6545 7272 6f72  row a ValueError
-0000e750: 2077 6865 6e20 6174 7465 6d70 7469 6e67   when attempting
-0000e760: 2074 6f20 7772 6974 6520 6120 6764 7320   to write a gds 
-0000e770: 7769 7468 2064 7570 6c69 6361 7465 2063  with duplicate c
-0000e780: 656c 6c73 2e0a 2020 2020 2020 2020 2020  ells..          
-0000e790: 2020 2020 2020 2020 2020 226f 7665 7277            "overw
-0000e7a0: 7269 7465 223a 206f 7665 7277 7269 7465  rite": overwrite
-0000e7b0: 2061 6c6c 2064 7570 6c69 6361 7465 2063   all duplicate c
-0000e7c0: 656c 6c73 2077 6974 6820 6f6e 6520 6f66  ells with one of
-0000e7d0: 2074 6865 2064 7570 6c69 6361 7465 732c   the duplicates,
-0000e7e0: 2077 6974 686f 7574 2077 6172 6e69 6e67   without warning
-0000e7f0: 2e0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000e800: 2020 2020 2020 4e6f 6e65 3a20 646f 206e        None: do n
-0000e810: 6f74 2074 7279 2074 6f20 7265 736f 6c76  ot try to resolv
-0000e820: 6520 2861 7420 796f 7572 206f 776e 2072  e (at your own r
-0000e830: 6973 6b21 290a 2020 2020 2020 2020 2020  isk!).          
-0000e840: 2020 2020 2020 666c 6174 7465 6e5f 696e        flatten_in
-0000e850: 7661 6c69 645f 7265 6673 3a20 666c 6174  valid_refs: flat
-0000e860: 7465 6e73 2063 6f6d 706f 6e65 6e74 2072  tens component r
-0000e870: 6566 6572 656e 6365 7320 7768 6963 6820  eferences which 
-0000e880: 6861 7665 2069 6e76 616c 6964 2074 7261  have invalid tra
-0000e890: 6e73 666f 726d 6174 696f 6e73 2e0a 2020  nsformations..  
-0000e8a0: 2020 2020 2020 2020 2020 2020 2020 6d61                ma
-0000e8b0: 785f 706f 696e 7473 3a20 4d61 7869 6d61  x_points: Maxima
-0000e8c0: 6c20 6e75 6d62 6572 206f 6620 7665 7274  l number of vert
-0000e8d0: 6963 6573 2070 6572 2070 6f6c 7967 6f6e  ices per polygon
-0000e8e0: 2e20 506f 6c79 676f 6e73 2077 6974 6820  . Polygons with 
-0000e8f0: 6d6f 7265 2076 6572 7469 6365 7320 7468  more vertices th
-0000e900: 6174 2074 6869 7320 6172 6520 6175 746f  at this are auto
-0000e910: 6d61 7469 6361 6c6c 7920 6672 6163 7475  matically fractu
-0000e920: 7265 642e 0a0a 2020 2020 2020 2020 2020  red...          
-0000e930: 2020 4f61 7369 7320 7365 7474 696e 6773    Oasis settings
-0000e940: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000e950: 2020 636f 6d70 7265 7373 696f 6e5f 6c65    compression_le
-0000e960: 7665 6c3a 204c 6576 656c 206f 6620 636f  vel: Level of co
-0000e970: 6d70 7265 7373 696f 6e20 666f 7220 6365  mpression for ce
-0000e980: 6c6c 7320 2862 6574 7765 656e 2030 2061  lls (between 0 a
-0000e990: 6e64 2039 292e 0a20 2020 2020 2020 2020  nd 9)..         
-0000e9a0: 2020 2020 2020 2020 2020 2053 6574 7469             Setti
-0000e9b0: 6e67 2074 6f20 3020 7769 6c6c 2064 6973  ng to 0 will dis
-0000e9c0: 6162 6c65 2063 656c 6c20 636f 6d70 7265  able cell compre
-0000e9d0: 7373 696f 6e2c 2031 2067 6976 6573 2074  ssion, 1 gives t
-0000e9e0: 6865 2062 6573 7420 7370 6565 6420 616e  he best speed an
-0000e9f0: 6420 392c 2074 6865 2062 6573 7420 636f  d 9, the best co
-0000ea00: 6d70 7265 7373 696f 6e2e 0a20 2020 2020  mpression..     
-0000ea10: 2020 2020 2020 2020 2020 2064 6574 6563             detec
-0000ea20: 745f 7265 6374 616e 676c 6573 3a20 5374  t_rectangles: St
-0000ea30: 6f72 6520 7265 6374 616e 676c 6573 2069  ore rectangles i
-0000ea40: 6e20 636f 6d70 7265 7373 6564 2066 6f72  n compressed for
-0000ea50: 6d61 742e 0a20 2020 2020 2020 2020 2020  mat..           
-0000ea60: 2020 2020 2064 6574 6563 745f 7472 6170       detect_trap
-0000ea70: 657a 6f69 6473 3a20 5374 6f72 6520 7472  ezoids: Store tr
-0000ea80: 6170 657a 6f69 6473 2069 6e20 636f 6d70  apezoids in comp
-0000ea90: 7265 7373 6564 2066 6f72 6d61 742e 0a20  ressed format.. 
-0000eaa0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-0000eab0: 6972 636c 655f 746f 6c65 7261 6e63 653a  ircle_tolerance:
-0000eac0: 2054 6f6c 6572 616e 6365 2066 6f72 2064   Tolerance for d
-0000ead0: 6574 6563 7469 6e67 2063 6972 636c 6573  etecting circles
-0000eae0: 2e20 4966 206c 6573 7320 6f72 2065 7175  . If less or equ
-0000eaf0: 616c 2074 6f20 302c 206e 6f20 6465 7465  al to 0, no dete
-0000eb00: 6374 696f 6e20 6973 2070 6572 666f 726d  ction is perform
-0000eb10: 6564 2e20 4369 7263 6c65 7320 6172 6520  ed. Circles are 
-0000eb20: 7374 6f72 6564 2069 6e20 636f 6d70 7265  stored in compre
-0000eb30: 7373 6564 2066 6f72 6d61 742e 0a20 2020  ssed format..   
-0000eb40: 2020 2020 2020 2020 2020 2020 2076 616c               val
-0000eb50: 6964 6174 696f 6e20 2822 6372 6333 3222  idation ("crc32"
-0000eb60: 2c20 2263 6865 636b 7375 6d33 3222 2c20  , "checksum32", 
-0000eb70: 4e6f 6e65 293a 2074 7970 6520 6f66 2076  None): type of v
-0000eb80: 616c 6964 6174 696f 6e20 746f 2069 6e63  alidation to inc
-0000eb90: 6c75 6465 2069 6e20 7468 6520 7361 7665  lude in the save
-0000eba0: 6420 6669 6c65 2e0a 2020 2020 2020 2020  d file..        
-0000ebb0: 2020 2020 2020 2020 7374 616e 6461 7264          standard
-0000ebc0: 5f70 726f 7065 7274 6965 733a 2053 746f  _properties: Sto
-0000ebd0: 7265 2073 7461 6e64 6172 6420 4f41 5349  re standard OASI
-0000ebe0: 5320 7072 6f70 6572 7469 6573 2069 6e20  S properties in 
-0000ebf0: 7468 6520 6669 6c65 2e0a 0a20 2020 2020  the file...     
-0000ec00: 2020 2022 2222 0a0a 2020 2020 2020 2020     """..        
-0000ec10: 6672 6f6d 2067 6473 6661 6374 6f72 792e  from gdsfactory.
-0000ec20: 7064 6b20 696d 706f 7274 2067 6574 5f61  pdk import get_a
-0000ec30: 6374 6976 655f 7064 6b0a 0a20 2020 2020  ctive_pdk..     
-0000ec40: 2020 2069 6620 6764 7370 6174 6820 616e     if gdspath an
-0000ec50: 6420 6764 7364 6972 3a0a 2020 2020 2020  d gdsdir:.      
-0000ec60: 2020 2020 2020 7761 726e 696e 6773 2e77        warnings.w
-0000ec70: 6172 6e28 0a20 2020 2020 2020 2020 2020  arn(.           
-0000ec80: 2020 2020 2022 6764 7370 6174 6820 616e       "gdspath an
-0000ec90: 6420 6764 7364 6972 2068 6176 6520 626f  d gdsdir have bo
-0000eca0: 7468 2062 6565 6e20 7370 6563 6966 6965  th been specifie
-0000ecb0: 642e 2067 6473 7061 7468 2077 696c 6c20  d. gdspath will 
-0000ecc0: 7461 6b65 2070 7265 6365 6465 6e63 6520  take precedence 
-0000ecd0: 616e 6420 6764 7364 6972 2077 696c 6c20  and gdsdir will 
-0000ece0: 6265 2069 676e 6f72 6564 2e22 0a20 2020  be ignored.".   
-0000ecf0: 2020 2020 2020 2020 2029 0a0a 2020 2020           )..    
-0000ed00: 2020 2020 6465 6661 756c 745f 7365 7474      default_sett
-0000ed10: 696e 6773 203d 2067 6574 5f61 6374 6976  ings = get_activ
-0000ed20: 655f 7064 6b28 292e 6764 735f 7772 6974  e_pdk().gds_writ
-0000ed30: 655f 7365 7474 696e 6773 0a20 2020 2020  e_settings.     
-0000ed40: 2020 2064 6566 6175 6c74 5f6f 6173 6973     default_oasis
-0000ed50: 5f73 6574 7469 6e67 7320 3d20 6765 745f  _settings = get_
-0000ed60: 6163 7469 7665 5f70 646b 2829 2e6f 6173  active_pdk().oas
-0000ed70: 6973 5f73 6574 7469 6e67 730a 0a20 2020  is_settings..   
-0000ed80: 2020 2020 2065 7870 6c69 6369 745f 6764       explicit_gd
-0000ed90: 735f 7365 7474 696e 6773 203d 207b 0a20  s_settings = {. 
-0000eda0: 2020 2020 2020 2020 2020 206b 3a20 760a             k: v.
-0000edb0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-0000edc0: 6b2c 2076 2069 6e20 6b77 6172 6773 2e69  k, v in kwargs.i
-0000edd0: 7465 6d73 2829 0a20 2020 2020 2020 2020  tems().         
-0000ede0: 2020 2069 6620 7620 6973 206e 6f74 204e     if v is not N
-0000edf0: 6f6e 6520 616e 6420 6b20 696e 2064 6566  one and k in def
-0000ee00: 6175 6c74 5f73 6574 7469 6e67 732e 6469  ault_settings.di
-0000ee10: 6374 2829 0a20 2020 2020 2020 207d 0a20  ct().        }. 
+0000b990: 2028 312c 2031 3029 2c0a 2020 2020 2020   (1, 10),.      
+0000b9a0: 2020 7368 6f77 5f6c 6162 656c 733a 2062    show_labels: b
+0000b9b0: 6f6f 6c20 3d20 4661 6c73 652c 0a20 2020  ool = False,.   
+0000b9c0: 2029 202d 3e20 4e6f 6e65 3a0a 2020 2020   ) -> None:.    
+0000b9d0: 2020 2020 2222 2252 6574 7572 6e73 206b      """Returns k
+0000b9e0: 6c61 796f 7574 2069 6d61 6765 2e0a 0a20  layout image... 
+0000b9f0: 2020 2020 2020 2049 6620 6974 2066 6169         If it fai
+0000ba00: 6c73 2074 6f20 696d 706f 7274 206b 6c61  ls to import kla
+0000ba10: 796f 7574 2064 6566 6175 6c74 7320 746f  yout defaults to
+0000ba20: 206d 6174 706c 6f74 6c69 622e 0a0a 2020   matplotlib...  
+0000ba30: 2020 2020 2020 4172 6773 3a0a 2020 2020        Args:.    
+0000ba40: 2020 2020 2020 2020 7368 6f77 5f70 6f72          show_por
+0000ba50: 7473 3a20 7368 6f77 7320 636f 6d70 6f6e  ts: shows compon
+0000ba60: 656e 7420 7769 7468 2070 6f72 7420 6d61  ent with port ma
+0000ba70: 726b 6572 7320 616e 6420 6c61 6265 6c73  rkers and labels
+0000ba80: 2e0a 2020 2020 2020 2020 2020 2020 706f  ..            po
+0000ba90: 7274 5f6d 6172 6b65 725f 6c61 7965 723a  rt_marker_layer:
+0000baa0: 2066 6f72 2074 6865 2070 6f72 7473 2e0a   for the ports..
+0000bab0: 2020 2020 2020 2020 2020 2020 7368 6f77              show
+0000bac0: 5f6c 6162 656c 733a 2073 686f 7773 206c  _labels: shows l
+0000bad0: 6162 656c 732e 0a20 2020 2020 2020 2022  abels..        "
+0000bae0: 2222 0a0a 2020 2020 2020 2020 636f 6d70  ""..        comp
+0000baf0: 6f6e 656e 7420 3d20 280a 2020 2020 2020  onent = (.      
+0000bb00: 2020 2020 2020 7365 6c66 2e61 6464 5f70        self.add_p
+0000bb10: 696e 735f 7472 6961 6e67 6c65 2870 6f72  ins_triangle(por
+0000bb20: 745f 6d61 726b 6572 5f6c 6179 6572 3d70  t_marker_layer=p
+0000bb30: 6f72 745f 6d61 726b 6572 5f6c 6179 6572  ort_marker_layer
+0000bb40: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
+0000bb50: 2073 686f 775f 706f 7274 730a 2020 2020   show_ports.    
+0000bb60: 2020 2020 2020 2020 656c 7365 2073 656c          else sel
+0000bb70: 660a 2020 2020 2020 2020 290a 0a20 2020  f.        )..   
+0000bb80: 2020 2020 2074 7279 3a0a 2020 2020 2020       try:.      
+0000bb90: 2020 2020 2020 696d 706f 7274 206b 6c61        import kla
+0000bba0: 796f 7574 2e64 6220 6173 2064 6220 2023  yout.db as db  #
+0000bbb0: 206e 6f71 613a 2046 3430 310a 2020 2020   noqa: F401.    
+0000bbc0: 2020 2020 2020 2020 696d 706f 7274 206b          import k
+0000bbd0: 6c61 796f 7574 2e6c 6179 2061 7320 6c61  layout.lay as la
+0000bbe0: 790a 2020 2020 2020 2020 2020 2020 6672  y.            fr
+0000bbf0: 6f6d 2067 6473 6661 6374 6f72 792e 7064  om gdsfactory.pd
+0000bc00: 6b20 696d 706f 7274 2067 6574 5f6c 6179  k import get_lay
+0000bc10: 6572 5f76 6965 7773 0a20 2020 2020 2020  er_views.       
+0000bc20: 2020 2020 2066 726f 6d20 4950 7974 686f       from IPytho
+0000bc30: 6e2e 6469 7370 6c61 7920 696d 706f 7274  n.display import
+0000bc40: 2064 6973 706c 6179 0a20 2020 2020 2020   display.       
+0000bc50: 2020 2020 2066 726f 6d20 6970 7977 6964       from ipywid
+0000bc60: 6765 7473 2069 6d70 6f72 7420 496d 6167  gets import Imag
+0000bc70: 650a 0a20 2020 2020 2020 2020 2020 2067  e..            g
+0000bc80: 6473 7061 7468 203d 2063 6f6d 706f 6e65  dspath = compone
+0000bc90: 6e74 2e77 7269 7465 5f67 6473 286c 6f67  nt.write_gds(log
+0000bca0: 6769 6e67 3d46 616c 7365 290a 2020 2020  ging=False).    
+0000bcb0: 2020 2020 2020 2020 6c79 705f 7061 7468          lyp_path
+0000bcc0: 203d 2067 6473 7061 7468 2e77 6974 685f   = gdspath.with_
+0000bcd0: 7375 6666 6978 2822 2e6c 7970 2229 0a0a  suffix(".lyp")..
+0000bce0: 2020 2020 2020 2020 2020 2020 6c61 7965              laye
+0000bcf0: 725f 7669 6577 7320 3d20 6765 745f 6c61  r_views = get_la
+0000bd00: 7965 725f 7669 6577 7328 290a 2020 2020  yer_views().    
+0000bd10: 2020 2020 2020 2020 6c61 7965 725f 7669          layer_vi
+0000bd20: 6577 732e 746f 5f6c 7970 2866 696c 6570  ews.to_lyp(filep
+0000bd30: 6174 683d 6c79 705f 7061 7468 290a 0a20  ath=lyp_path).. 
+0000bd40: 2020 2020 2020 2020 2020 206c 6179 6f75             layou
+0000bd50: 745f 7669 6577 203d 206c 6179 2e4c 6179  t_view = lay.Lay
+0000bd60: 6f75 7456 6965 7728 290a 2020 2020 2020  outView().      
+0000bd70: 2020 2020 2020 6c61 796f 7574 5f76 6965        layout_vie
+0000bd80: 772e 6c6f 6164 5f6c 6179 6f75 7428 7374  w.load_layout(st
+0000bd90: 7228 6764 7370 6174 682e 6162 736f 6c75  r(gdspath.absolu
+0000bda0: 7465 2829 2929 0a20 2020 2020 2020 2020  te())).         
+0000bdb0: 2020 206c 6179 6f75 745f 7669 6577 2e6d     layout_view.m
+0000bdc0: 6178 5f68 6965 7228 290a 2020 2020 2020  ax_hier().      
+0000bdd0: 2020 2020 2020 6c61 796f 7574 5f76 6965        layout_vie
+0000bde0: 772e 6c6f 6164 5f6c 6179 6572 5f70 726f  w.load_layer_pro
+0000bdf0: 7073 2873 7472 286c 7970 5f70 6174 6829  ps(str(lyp_path)
+0000be00: 290a 0a20 2020 2020 2020 2020 2020 206c  )..            l
+0000be10: 6179 6f75 745f 7669 6577 2e73 6574 5f63  ayout_view.set_c
+0000be20: 6f6e 6669 6728 2274 6578 742d 7669 7369  onfig("text-visi
+0000be30: 626c 6522 2c20 2274 7275 6522 2069 6620  ble", "true" if 
+0000be40: 7368 6f77 5f6c 6162 656c 7320 656c 7365  show_labels else
+0000be50: 2022 6661 6c73 6522 290a 0a20 2020 2020   "false")..     
+0000be60: 2020 2020 2020 2070 6978 656c 5f62 7566         pixel_buf
+0000be70: 6665 7220 3d20 6c61 796f 7574 5f76 6965  fer = layout_vie
+0000be80: 772e 6765 745f 7069 7865 6c73 5f77 6974  w.get_pixels_wit
+0000be90: 685f 6f70 7469 6f6e 7328 3830 302c 2036  h_options(800, 6
+0000bea0: 3030 290a 2020 2020 2020 2020 2020 2020  00).            
+0000beb0: 706e 675f 6461 7461 203d 2070 6978 656c  png_data = pixel
+0000bec0: 5f62 7566 6665 722e 746f 5f70 6e67 5f64  _buffer.to_png_d
+0000bed0: 6174 6128 290a 2020 2020 2020 2020 2020  ata().          
+0000bee0: 2020 696d 6167 6520 3d20 496d 6167 6528    image = Image(
+0000bef0: 7661 6c75 653d 706e 675f 6461 7461 2c20  value=png_data, 
+0000bf00: 666f 726d 6174 3d22 706e 6722 290a 2020  format="png").  
+0000bf10: 2020 2020 2020 2020 2020 6469 7370 6c61            displa
+0000bf20: 7928 696d 6167 6529 0a0a 2020 2020 2020  y(image)..      
+0000bf30: 2020 6578 6365 7074 2049 6d70 6f72 7445    except ImportE
+0000bf40: 7272 6f72 3a0a 2020 2020 2020 2020 2020  rror:.          
+0000bf50: 2020 7072 696e 7428 0a20 2020 2020 2020    print(.       
+0000bf60: 2020 2020 2020 2020 2022 596f 7520 6361           "You ca
+0000bf70: 6e20 696e 7374 616c 6c20 6070 6970 2069  n install `pip i
+0000bf80: 6e73 7461 6c6c 2067 6473 6661 6374 6f72  nstall gdsfactor
+0000bf90: 795b 6675 6c6c 5d60 2066 6f72 2062 6574  y[full]` for bet
+0000bfa0: 7465 7220 7669 7375 616c 697a 6174 696f  ter visualizatio
+0000bfb0: 6e22 0a20 2020 2020 2020 2020 2020 2029  n".            )
+0000bfc0: 0a20 2020 2020 2020 2020 2020 2063 6f6d  .            com
+0000bfd0: 706f 6e65 6e74 2e70 6c6f 7428 706c 6f74  ponent.plot(plot
+0000bfe0: 7465 723d 226d 6174 706c 6f74 6c69 6222  ter="matplotlib"
+0000bff0: 290a 0a20 2020 2064 6566 2070 6c6f 745f  )..    def plot_
+0000c000: 6a75 7079 7465 7228 7365 6c66 293a 0a20  jupyter(self):. 
+0000c010: 2020 2020 2020 2022 2222 5368 6f77 7320         """Shows 
+0000c020: 6375 7272 656e 7420 6764 7320 696e 206b  current gds in k
+0000c030: 6c61 796f 7574 2e20 5573 6573 204b 7765  layout. Uses Kwe
+0000c040: 6220 6966 2073 6572 7665 7220 7275 6e6e  b if server runn
+0000c050: 696e 672e 0a0a 2020 2020 2020 2020 6966  ing...        if
+0000c060: 206e 6f74 2074 7269 6573 2075 7369 6e67   not tries using
+0000c070: 204b 6c61 796f 7574 2077 6964 6765 7420   Klayout widget 
+0000c080: 616e 6420 6669 6e61 6c6c 7920 6465 6661  and finally defa
+0000c090: 756c 7473 2074 6f20 6d61 7470 6c6f 746c  ults to matplotl
+0000c0a0: 6962 2e0a 2020 2020 2020 2020 2222 220a  ib..        """.
+0000c0b0: 2020 2020 2020 2020 7472 793a 0a20 2020          try:.   
+0000c0c0: 2020 2020 2020 2020 2069 6d70 6f72 7420           import 
+0000c0d0: 6f73 0a20 2020 2020 2020 2020 2020 2066  os.            f
+0000c0e0: 726f 6d20 6764 7366 6163 746f 7279 2e63  rom gdsfactory.c
+0000c0f0: 6f6e 6669 6720 696d 706f 7274 2050 4154  onfig import PAT
+0000c100: 480a 2020 2020 2020 2020 2020 2020 6672  H.            fr
+0000c110: 6f6d 2067 6473 6661 6374 6f72 792e 7064  om gdsfactory.pd
+0000c120: 6b20 696d 706f 7274 2067 6574 5f6c 6179  k import get_lay
+0000c130: 6572 5f76 6965 7773 0a20 2020 2020 2020  er_views.       
+0000c140: 2020 2020 2066 726f 6d20 4950 7974 686f       from IPytho
+0000c150: 6e2e 6469 7370 6c61 7920 696d 706f 7274  n.display import
+0000c160: 2049 4672 616d 650a 2020 2020 2020 2020   IFrame.        
+0000c170: 2020 2020 696d 706f 7274 206b 7765 622e      import kweb.
+0000c180: 7365 7276 6572 5f6a 7570 7974 6572 2061  server_jupyter a
+0000c190: 7320 6b6a 0a20 2020 2020 2020 2020 2020  s kj.           
+0000c1a0: 2066 726f 6d20 6874 6d6c 2069 6d70 6f72   from html impor
+0000c1b0: 7420 6573 6361 7065 0a0a 2020 2020 2020  t escape..      
+0000c1c0: 2020 2020 2020 6764 7370 6174 6820 3d20        gdspath = 
+0000c1d0: 7365 6c66 2e77 7269 7465 5f67 6473 2867  self.write_gds(g
+0000c1e0: 6473 6469 723d 5041 5448 2e67 6473 6c69  dsdir=PATH.gdsli
+0000c1f0: 6220 2f20 2265 7874 7261 222c 206c 6f67  b / "extra", log
+0000c200: 6769 6e67 3d46 616c 7365 290a 0a20 2020  ging=False)..   
+0000c210: 2020 2020 2020 2020 2064 6972 7061 7468           dirpath
+0000c220: 203d 2047 4453 4449 525f 5445 4d50 0a20   = GDSDIR_TEMP. 
+0000c230: 2020 2020 2020 2020 2020 2064 6972 7061             dirpa
+0000c240: 7468 2e6d 6b64 6972 2865 7869 7374 5f6f  th.mkdir(exist_o
+0000c250: 6b3d 5472 7565 2c20 7061 7265 6e74 733d  k=True, parents=
+0000c260: 5472 7565 290a 2020 2020 2020 2020 2020  True).          
+0000c270: 2020 6c79 705f 7061 7468 203d 2064 6972    lyp_path = dir
+0000c280: 7061 7468 202f 2022 6c61 7965 7273 2e6c  path / "layers.l
+0000c290: 7970 220a 0a20 2020 2020 2020 2020 2020  yp"..           
+0000c2a0: 206c 6179 6572 5f70 726f 7073 203d 2067   layer_props = g
+0000c2b0: 6574 5f6c 6179 6572 5f76 6965 7773 2829  et_layer_views()
+0000c2c0: 0a20 2020 2020 2020 2020 2020 206c 6179  .            lay
+0000c2d0: 6572 5f70 726f 7073 2e74 6f5f 6c79 7028  er_props.to_lyp(
+0000c2e0: 6669 6c65 7061 7468 3d6c 7970 5f70 6174  filepath=lyp_pat
+0000c2f0: 6829 0a0a 2020 2020 2020 2020 2020 2020  h)..            
+0000c300: 7372 6320 3d20 6622 6874 7470 3a2f 2f31  src = f"http://1
+0000c310: 3237 2e30 2e30 2e31 3a7b 6b6a 2e70 6f72  27.0.0.1:{kj.por
+0000c320: 747d 2f67 6473 3f67 6473 5f66 696c 653d  t}/gds?gds_file=
+0000c330: 7b65 7363 6170 6528 7374 7228 6764 7370  {escape(str(gdsp
+0000c340: 6174 6829 297d 266c 6179 6572 5f70 726f  ath))}&layer_pro
+0000c350: 7073 3d7b 6573 6361 7065 2873 7472 286c  ps={escape(str(l
+0000c360: 7970 5f70 6174 6829 297d 220a 2020 2020  yp_path))}".    
+0000c370: 2020 2020 2020 2020 6c6f 6767 6572 2e64          logger.d
+0000c380: 6562 7567 2873 7263 290a 0a20 2020 2020  ebug(src)..     
+0000c390: 2020 2020 2020 2069 6620 6b6a 2e6a 7570         if kj.jup
+0000c3a0: 7974 6572 5f73 6572 7665 7220 616e 6420  yter_server and 
+0000c3b0: 6e6f 7420 6f73 2e65 6e76 6972 6f6e 2e67  not os.environ.g
+0000c3c0: 6574 2822 444f 4353 222c 2046 616c 7365  et("DOCS", False
+0000c3d0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+0000c3e0: 2020 2072 6574 7572 6e20 4946 7261 6d65     return IFrame
+0000c3f0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+0000c400: 2020 2020 2020 7372 633d 7372 632c 0a20        src=src,. 
+0000c410: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c420: 2020 2077 6964 7468 3d31 3430 302c 0a20     width=1400,. 
+0000c430: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c440: 2020 2068 6569 6768 743d 3630 302c 0a20     height=600,. 
+0000c450: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+0000c460: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
+0000c470: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+0000c480: 2020 2072 6574 7572 6e20 7365 6c66 2e70     return self.p
+0000c490: 6c6f 745f 6b6c 6179 6f75 7428 290a 2020  lot_klayout().  
+0000c4a0: 2020 2020 2020 6578 6365 7074 2049 6d70        except Imp
+0000c4b0: 6f72 7445 7272 6f72 3a0a 2020 2020 2020  ortError:.      
+0000c4c0: 2020 2020 2020 7072 696e 7428 0a20 2020        print(.   
+0000c4d0: 2020 2020 2020 2020 2020 2020 2022 596f               "Yo
+0000c4e0: 7520 6361 6e20 696e 7374 616c 6c20 6070  u can install `p
+0000c4f0: 6970 2069 6e73 7461 6c6c 2067 6473 6661  ip install gdsfa
+0000c500: 6374 6f72 795b 6675 6c6c 5d60 2066 6f72  ctory[full]` for
+0000c510: 2062 6574 7465 7220 7669 7375 616c 697a   better visualiz
+0000c520: 6174 696f 6e22 0a20 2020 2020 2020 2020  ation".         
+0000c530: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
+0000c540: 2072 6574 7572 6e20 7365 6c66 2e70 6c6f   return self.plo
+0000c550: 745f 6b6c 6179 6f75 7428 290a 0a20 2020  t_klayout()..   
+0000c560: 2064 6566 2070 6c6f 745f 6d61 7470 6c6f   def plot_matplo
+0000c570: 746c 6962 2873 656c 662c 202a 2a6b 7761  tlib(self, **kwa
+0000c580: 7267 7329 202d 3e20 4e6f 6e65 3a0a 2020  rgs) -> None:.  
+0000c590: 2020 2020 2020 2222 2250 6c6f 7420 636f        """Plot co
+0000c5a0: 6d70 6f6e 656e 7420 7573 696e 6720 6d61  mponent using ma
+0000c5b0: 7470 6c6f 746c 6962 2e0a 0a20 2020 2020  tplotlib...     
+0000c5c0: 2020 204b 6579 776f 7264 2041 7267 733a     Keyword Args:
+0000c5d0: 0a20 2020 2020 2020 2020 2020 2073 686f  .            sho
+0000c5e0: 775f 706f 7274 733a 2053 6574 7320 7768  w_ports: Sets wh
+0000c5f0: 6574 6865 7220 706f 7274 7320 6172 6520  ether ports are 
+0000c600: 6472 6177 6e2e 0a20 2020 2020 2020 2020  drawn..         
+0000c610: 2020 2073 686f 775f 7375 6270 6f72 7473     show_subports
+0000c620: 3a20 5365 7473 2077 6865 7468 6572 2073  : Sets whether s
+0000c630: 7562 706f 7274 7320 2870 6f72 7473 2074  ubports (ports t
+0000c640: 6861 7420 6265 6c6f 6e67 2074 6f20 7265  hat belong to re
+0000c650: 6665 7265 6e63 6573 2920 6172 6520 6472  ferences) are dr
+0000c660: 6177 6e2e 0a20 2020 2020 2020 2020 2020  awn..           
+0000c670: 206c 6162 656c 5f61 6c69 6173 6573 3a20   label_aliases: 
+0000c680: 5365 7473 2077 6865 7468 6572 2061 6c69  Sets whether ali
+0000c690: 6173 6573 2061 7265 206c 6162 656c 6564  ases are labeled
+0000c6a0: 2077 6974 6820 6120 7465 7874 206e 616d   with a text nam
+0000c6b0: 652e 0a20 2020 2020 2020 2020 2020 206e  e..            n
+0000c6c0: 6577 5f77 696e 646f 773a 2049 6620 5472  ew_window: If Tr
+0000c6d0: 7565 2c20 6561 6368 2063 616c 6c20 746f  ue, each call to
+0000c6e0: 2071 7569 636b 706c 6f74 2829 2077 696c   quickplot() wil
+0000c6f0: 6c20 6765 6e65 7261 7465 2061 2073 6570  l generate a sep
+0000c700: 6172 6174 6520 7769 6e64 6f77 2e0a 2020  arate window..  
+0000c710: 2020 2020 2020 2020 2020 626c 6f63 6b69            blocki
+0000c720: 6e67 3a20 4966 2054 7275 652c 2063 616c  ng: If True, cal
+0000c730: 6c69 6e67 2071 7569 636b 706c 6f74 2829  ling quickplot()
+0000c740: 2077 696c 6c20 7061 7573 6520 6578 6563   will pause exec
+0000c750: 7574 696f 6e20 6f66 2028 2262 6c6f 636b  ution of ("block
+0000c760: 2229 2074 6865 0a20 2020 2020 2020 2020  ") the.         
+0000c770: 2020 2020 2020 2072 656d 6169 6e64 6572         remainder
+0000c780: 206f 6620 7468 6520 7079 7468 6f6e 2063   of the python c
+0000c790: 6f64 6520 756e 7469 6c20 7468 6520 7175  ode until the qu
+0000c7a0: 6963 6b70 6c6f 7428 2920 7769 6e64 6f77  ickplot() window
+0000c7b0: 2069 7320 636c 6f73 6564 2e0a 2020 2020   is closed..    
+0000c7c0: 2020 2020 2020 2020 2020 2020 4966 2046              If F
+0000c7d0: 616c 7365 2c20 7468 6520 7769 6e64 6f77  alse, the window
+0000c7e0: 2077 696c 6c20 6265 206f 7065 6e65 6420   will be opened 
+0000c7f0: 616e 6420 636f 6465 2077 696c 6c20 636f  and code will co
+0000c800: 6e74 696e 7565 2074 6f20 7275 6e2e 0a20  ntinue to run.. 
+0000c810: 2020 2020 2020 2020 2020 207a 6f6f 6d5f             zoom_
+0000c820: 6661 6374 6f72 3a20 5365 7473 2074 6865  factor: Sets the
+0000c830: 2073 6361 6c69 6e67 2066 6163 746f 7220   scaling factor 
+0000c840: 7768 656e 207a 6f6f 6d69 6e67 2074 6865  when zooming the
+0000c850: 2071 7569 636b 706c 6f74 2077 696e 646f   quickplot windo
+0000c860: 7720 7769 7468 2074 6865 0a20 2020 2020  w with the.     
+0000c870: 2020 2020 2020 2020 2020 206d 6f75 7365             mouse
+0000c880: 7768 6565 6c2f 7472 6163 6b70 6164 2e0a  wheel/trackpad..
+0000c890: 2020 2020 2020 2020 2020 2020 696e 7465              inte
+0000c8a0: 7261 6374 6976 655f 7a6f 6f6d 3a20 456e  ractive_zoom: En
+0000c8b0: 6162 6c65 7320 7573 696e 6720 6d6f 7573  ables using mous
+0000c8c0: 6577 6865 656c 2f74 7261 636b 7061 6420  ewheel/trackpad 
+0000c8d0: 746f 207a 6f6f 6d2e 0a20 2020 2020 2020  to zoom..       
+0000c8e0: 2020 2020 2066 6f6e 7473 697a 653a 2066       fontsize: f
+0000c8f0: 6f72 206c 6162 656c 732e 0a20 2020 2020  or labels..     
+0000c900: 2020 2020 2020 206c 6179 6572 735f 6578         layers_ex
+0000c910: 636c 7564 6564 3a20 6c69 7374 206f 6620  cluded: list of 
+0000c920: 6c61 7965 7273 2074 6f20 6578 636c 7564  layers to exclud
+0000c930: 652e 0a20 2020 2020 2020 2020 2020 206c  e..            l
+0000c940: 6179 6572 5f76 6965 7773 3a20 6c61 7965  ayer_views: laye
+0000c950: 725f 7669 6577 7320 636f 6c6f 7273 206c  r_views colors l
+0000c960: 6f61 6465 6420 6672 6f6d 204b 6c61 796f  oaded from Klayo
+0000c970: 7574 2e0a 2020 2020 2020 2020 2020 2020  ut..            
+0000c980: 6d69 6e5f 6173 7065 6374 3a20 6d69 6e69  min_aspect: mini
+0000c990: 6d75 6d20 6173 7065 6374 2072 6174 696f  mum aspect ratio
+0000c9a0: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
+0000c9b0: 2020 2020 2020 6672 6f6d 2067 6473 6661        from gdsfa
+0000c9c0: 6374 6f72 792e 7175 6963 6b70 6c6f 7474  ctory.quickplott
+0000c9d0: 6572 2069 6d70 6f72 7420 7175 6963 6b70  er import quickp
+0000c9e0: 6c6f 740a 0a20 2020 2020 2020 2071 7569  lot..        qui
+0000c9f0: 636b 706c 6f74 2873 656c 662c 202a 2a6b  ckplot(self, **k
+0000ca00: 7761 7267 7329 0a0a 2020 2020 6465 6620  wargs)..    def 
+0000ca10: 706c 6f74 2873 656c 662c 2070 6c6f 7474  plot(self, plott
+0000ca20: 6572 3a20 4f70 7469 6f6e 616c 5b50 6c6f  er: Optional[Plo
+0000ca30: 7474 6572 5d20 3d20 4e6f 6e65 2c20 2a2a  tter] = None, **
+0000ca40: 6b77 6172 6773 2920 2d3e 204e 6f6e 653a  kwargs) -> None:
+0000ca50: 0a20 2020 2020 2020 2022 2222 5265 7475  .        """Retu
+0000ca60: 726e 7320 636f 6d70 6f6e 656e 7420 706c  rns component pl
+0000ca70: 6f74 2075 7369 6e67 206b 6c61 796f 7574  ot using klayout
+0000ca80: 2c20 6d61 7470 6c6f 746c 6962 2c20 686f  , matplotlib, ho
+0000ca90: 6c6f 7669 6577 7320 6f72 2071 742e 0a0a  loviews or qt...
+0000caa0: 2020 2020 2020 2020 5765 2072 6563 6f6d          We recom
+0000cab0: 6d65 6e64 2075 7369 6e67 206b 6c61 796f  mend using klayo
+0000cac0: 7574 2e0a 0a20 2020 2020 2020 2041 7267  ut...        Arg
+0000cad0: 733a 0a20 2020 2020 2020 2020 2020 2070  s:.            p
+0000cae0: 6c6f 7474 6572 3a20 706c 6f74 2062 6163  lotter: plot bac
+0000caf0: 6b65 6e64 2028 2768 6f6c 6f76 6965 7773  kend ('holoviews
+0000cb00: 272c 2027 6d61 7470 6c6f 746c 6962 272c  ', 'matplotlib',
+0000cb10: 2027 7174 272c 2027 6b6c 6179 6f75 7427   'qt', 'klayout'
+0000cb20: 292e 0a20 2020 2020 2020 2022 2222 0a20  )..        """. 
+0000cb30: 2020 2020 2020 2070 6c6f 7474 6572 203d         plotter =
+0000cb40: 2070 6c6f 7474 6572 206f 7220 434f 4e46   plotter or CONF
+0000cb50: 2e67 6574 2822 706c 6f74 7465 7222 2c20  .get("plotter", 
+0000cb60: 226d 6174 706c 6f74 6c69 6222 290a 0a20  "matplotlib").. 
+0000cb70: 2020 2020 2020 2069 6620 706c 6f74 7465         if plotte
+0000cb80: 7220 3d3d 2022 6b6c 6179 6f75 7422 3a0a  r == "klayout":.
+0000cb90: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000cba0: 2e70 6c6f 745f 6b6c 6179 6f75 7428 290a  .plot_klayout().
+0000cbb0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+0000cbc0: 726e 0a0a 2020 2020 2020 2020 656c 6966  rn..        elif
+0000cbd0: 2070 6c6f 7474 6572 203d 3d20 226d 6174   plotter == "mat
+0000cbe0: 706c 6f74 6c69 6222 3a0a 2020 2020 2020  plotlib":.      
+0000cbf0: 2020 2020 2020 6672 6f6d 2067 6473 6661        from gdsfa
+0000cc00: 6374 6f72 792e 7175 6963 6b70 6c6f 7474  ctory.quickplott
+0000cc10: 6572 2069 6d70 6f72 7420 7175 6963 6b70  er import quickp
+0000cc20: 6c6f 740a 0a20 2020 2020 2020 2020 2020  lot..           
+0000cc30: 2071 7569 636b 706c 6f74 2873 656c 662c   quickplot(self,
+0000cc40: 202a 2a6b 7761 7267 7329 0a20 2020 2020   **kwargs).     
+0000cc50: 2020 2020 2020 2072 6574 7572 6e0a 0a20         return.. 
+0000cc60: 2020 2020 2020 2065 6c69 6620 706c 6f74         elif plot
+0000cc70: 7465 7220 3d3d 2022 686f 6c6f 7669 6577  ter == "holoview
+0000cc80: 7322 3a0a 2020 2020 2020 2020 2020 2020  s":.            
+0000cc90: 7472 793a 0a20 2020 2020 2020 2020 2020  try:.           
+0000cca0: 2020 2020 2069 6d70 6f72 7420 686f 6c6f       import holo
+0000ccb0: 7669 6577 7320 6173 2068 760a 0a20 2020  views as hv..   
+0000ccc0: 2020 2020 2020 2020 2020 2020 2068 762e               hv.
+0000ccd0: 6578 7465 6e73 696f 6e28 2262 6f6b 6568  extension("bokeh
+0000cce0: 2229 0a20 2020 2020 2020 2020 2020 2065  ").            e
+0000ccf0: 7863 6570 7420 496d 706f 7274 4572 726f  xcept ImportErro
+0000cd00: 7220 6173 2065 3a0a 2020 2020 2020 2020  r as e:.        
+0000cd10: 2020 2020 2020 2020 7072 696e 7428 2279          print("y
+0000cd20: 6f75 206e 6565 6420 746f 2060 7069 7020  ou need to `pip 
+0000cd30: 696e 7374 616c 6c20 686f 6c6f 7669 6577  install holoview
+0000cd40: 7360 2229 0a20 2020 2020 2020 2020 2020  s`").           
+0000cd50: 2020 2020 2072 6169 7365 2065 0a20 2020       raise e.   
+0000cd60: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+0000cd70: 7365 6c66 2e70 6c6f 745f 686f 6c6f 7669  self.plot_holovi
+0000cd80: 6577 7328 2a2a 6b77 6172 6773 290a 0a20  ews(**kwargs).. 
+0000cd90: 2020 2020 2020 2065 6c69 6620 706c 6f74         elif plot
+0000cda0: 7465 7220 3d3d 2022 7174 223a 0a20 2020  ter == "qt":.   
+0000cdb0: 2020 2020 2020 2020 2066 726f 6d20 6764           from gd
+0000cdc0: 7366 6163 746f 7279 2e71 7569 636b 706c  sfactory.quickpl
+0000cdd0: 6f74 7465 7220 696d 706f 7274 2071 7569  otter import qui
+0000cde0: 636b 706c 6f74 320a 0a20 2020 2020 2020  ckplot2..       
+0000cdf0: 2020 2020 2071 7569 636b 706c 6f74 3228       quickplot2(
+0000ce00: 7365 6c66 290a 2020 2020 2020 2020 2020  self).          
+0000ce10: 2020 7265 7475 726e 0a20 2020 2020 2020    return.       
+0000ce20: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+0000ce30: 2020 2072 6169 7365 2056 616c 7565 4572     raise ValueEr
+0000ce40: 726f 7228 6622 7b70 6c6f 7474 6572 2172  ror(f"{plotter!r
+0000ce50: 7d20 6e6f 7420 696e 207b 506c 6f74 7465  } not in {Plotte
+0000ce60: 727d 2229 0a0a 2020 2020 6465 6620 706c  r}")..    def pl
+0000ce70: 6f74 5f68 6f6c 6f76 6965 7773 280a 2020  ot_holoviews(.  
+0000ce80: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
+0000ce90: 2020 2020 6c61 7965 7273 5f65 7863 6c75      layers_exclu
+0000cea0: 6465 643a 204f 7074 696f 6e61 6c5b 4c61  ded: Optional[La
+0000ceb0: 7965 7273 5d20 3d20 4e6f 6e65 2c0a 2020  yers] = None,.  
+0000cec0: 2020 2020 2020 6c61 7965 725f 7669 6577        layer_view
+0000ced0: 733a 204f 7074 696f 6e61 6c5b 4c61 7965  s: Optional[Laye
+0000cee0: 7256 6965 7773 5d20 3d20 4e6f 6e65 2c0a  rViews] = None,.
+0000cef0: 2020 2020 2020 2020 6d69 6e5f 6173 7065          min_aspe
+0000cf00: 6374 3a20 666c 6f61 7420 3d20 302e 3235  ct: float = 0.25
+0000cf10: 2c0a 2020 2020 2020 2020 7061 6464 696e  ,.        paddin
+0000cf20: 673a 2066 6c6f 6174 203d 2030 2e35 2c0a  g: float = 0.5,.
+0000cf30: 2020 2020 293a 0a20 2020 2020 2020 2022      ):.        "
+0000cf40: 2222 506c 6f74 2063 6f6d 706f 6e65 6e74  ""Plot component
+0000cf50: 2069 6e20 686f 6c6f 7669 6577 732e 0a0a   in holoviews...
+0000cf60: 2020 2020 2020 2020 4172 6773 3a0a 2020          Args:.  
+0000cf70: 2020 2020 2020 2020 2020 6c61 7965 7273            layers
+0000cf80: 5f65 7863 6c75 6465 643a 206c 6973 7420  _excluded: list 
+0000cf90: 6f66 206c 6179 6572 7320 746f 2065 7863  of layers to exc
+0000cfa0: 6c75 6465 2e0a 2020 2020 2020 2020 2020  lude..          
+0000cfb0: 2020 6c61 7965 725f 7669 6577 733a 206c    layer_views: l
+0000cfc0: 6179 6572 5f76 6965 7773 2063 6f6c 6f72  ayer_views color
+0000cfd0: 7320 6c6f 6164 6564 2066 726f 6d20 4b6c  s loaded from Kl
+0000cfe0: 6179 6f75 742e 0a20 2020 2020 2020 2020  ayout..         
+0000cff0: 2020 206d 696e 5f61 7370 6563 743a 206d     min_aspect: m
+0000d000: 696e 696d 756d 2061 7370 6563 7420 7261  inimum aspect ra
+0000d010: 7469 6f2e 0a20 2020 2020 2020 2020 2020  tio..           
+0000d020: 2070 6164 6469 6e67 3a20 6172 6f75 6e64   padding: around
+0000d030: 2062 6f75 6e64 696e 6720 626f 782e 0a0a   bounding box...
+0000d040: 2020 2020 2020 2020 5265 7475 726e 733a          Returns:
+0000d050: 0a20 2020 2020 2020 2020 2020 2048 6f6c  .            Hol
+0000d060: 6f76 6965 7773 204f 7665 726c 6179 2074  oviews Overlay t
+0000d070: 6f20 6469 7370 6c61 7920 616c 6c20 706f  o display all po
+0000d080: 6c79 676f 6e73 2e0a 2020 2020 2020 2020  lygons..        
+0000d090: 2222 220a 2020 2020 2020 2020 6672 6f6d  """.        from
+0000d0a0: 2067 6473 6661 6374 6f72 792e 6164 645f   gdsfactory.add_
+0000d0b0: 7069 6e73 2069 6d70 6f72 7420 6765 745f  pins import get_
+0000d0c0: 7069 6e5f 7472 6961 6e67 6c65 5f70 6f6c  pin_triangle_pol
+0000d0d0: 7967 6f6e 5f74 6970 0a20 2020 2020 2020  ygon_tip.       
+0000d0e0: 2066 726f 6d20 6764 7366 6163 746f 7279   from gdsfactory
+0000d0f0: 2e67 656e 6572 6963 5f74 6563 6820 696d  .generic_tech im
+0000d100: 706f 7274 204c 4159 4552 5f56 4945 5753  port LAYER_VIEWS
+0000d110: 0a0a 2020 2020 2020 2020 6966 206c 6179  ..        if lay
+0000d120: 6572 5f76 6965 7773 2069 7320 4e6f 6e65  er_views is None
+0000d130: 3a0a 2020 2020 2020 2020 2020 2020 6c61  :.            la
+0000d140: 7965 725f 7669 6577 7320 3d20 4c41 5945  yer_views = LAYE
+0000d150: 525f 5649 4557 530a 0a20 2020 2020 2020  R_VIEWS..       
+0000d160: 2074 7279 3a0a 2020 2020 2020 2020 2020   try:.          
+0000d170: 2020 696d 706f 7274 2068 6f6c 6f76 6965    import holovie
+0000d180: 7773 2061 7320 6876 0a0a 2020 2020 2020  ws as hv..      
+0000d190: 2020 2020 2020 6876 2e65 7874 656e 7369        hv.extensi
+0000d1a0: 6f6e 2822 626f 6b65 6822 290a 2020 2020  on("bokeh").    
+0000d1b0: 2020 2020 6578 6365 7074 2049 6d70 6f72      except Impor
+0000d1c0: 7445 7272 6f72 2061 7320 653a 0a20 2020  tError as e:.   
+0000d1d0: 2020 2020 2020 2020 2070 7269 6e74 2822           print("
+0000d1e0: 796f 7520 6e65 6564 2074 6f20 6070 6970  you need to `pip
+0000d1f0: 2069 6e73 7461 6c6c 2068 6f6c 6f76 6965   install holovie
+0000d200: 7773 6022 290a 2020 2020 2020 2020 2020  ws`").          
+0000d210: 2020 7261 6973 6520 650a 0a20 2020 2020    raise e..     
+0000d220: 2020 2073 656c 662e 5f62 625f 7661 6c69     self._bb_vali
+0000d230: 6420 3d20 4661 6c73 6520 2023 2072 6563  d = False  # rec
+0000d240: 6f6d 7075 7465 2074 6865 2062 6f75 6e64  ompute the bound
+0000d250: 696e 6720 626f 780a 2020 2020 2020 2020  ing box.        
+0000d260: 6220 3d20 7365 6c66 2e62 626f 7820 2b20  b = self.bbox + 
+0000d270: 2828 2d70 6164 6469 6e67 2c20 2d70 6164  ((-padding, -pad
+0000d280: 6469 6e67 292c 2028 7061 6464 696e 672c  ding), (padding,
+0000d290: 2070 6164 6469 6e67 2929 0a20 2020 2020   padding)).     
+0000d2a0: 2020 2062 203d 206e 702e 6172 7261 7928     b = np.array(
+0000d2b0: 622e 666c 6174 290a 2020 2020 2020 2020  b.flat).        
+0000d2c0: 6365 6e74 6572 203d 206e 702e 6172 7261  center = np.arra
+0000d2d0: 7928 286e 702e 7375 6d28 625b 3a3a 325d  y((np.sum(b[::2]
+0000d2e0: 2920 2f20 322c 206e 702e 7375 6d28 625b  ) / 2, np.sum(b[
+0000d2f0: 313a 3a32 5d29 202f 2032 2929 0a20 2020  1::2]) / 2)).   
+0000d300: 2020 2020 2073 697a 6520 3d20 6e70 2e61       size = np.a
+0000d310: 7272 6179 2828 6e70 2e61 6273 2862 5b32  rray((np.abs(b[2
+0000d320: 5d20 2d20 625b 305d 292c 206e 702e 6162  ] - b[0]), np.ab
+0000d330: 7328 625b 335d 202d 2062 5b31 5d29 2929  s(b[3] - b[1])))
+0000d340: 0a20 2020 2020 2020 2064 7820 3d20 6e70  .        dx = np
+0000d350: 2e61 7272 6179 280a 2020 2020 2020 2020  .array(.        
+0000d360: 2020 2020 280a 2020 2020 2020 2020 2020      (.          
+0000d370: 2020 2020 2020 6e70 2e6d 6178 696d 756d        np.maximum
+0000d380: 286d 696e 5f61 7370 6563 7420 2a20 7369  (min_aspect * si
+0000d390: 7a65 5b31 5d2c 2073 697a 655b 305d 2920  ze[1], size[0]) 
+0000d3a0: 2f20 322c 0a20 2020 2020 2020 2020 2020  / 2,.           
+0000d3b0: 2020 2020 206e 702e 6d61 7869 6d75 6d28       np.maximum(
+0000d3c0: 7369 7a65 5b31 5d2c 206d 696e 5f61 7370  size[1], min_asp
+0000d3d0: 6563 7420 2a20 7369 7a65 5b30 5d29 202f  ect * size[0]) /
+0000d3e0: 2032 2c0a 2020 2020 2020 2020 2020 2020   2,.            
+0000d3f0: 290a 2020 2020 2020 2020 290a 2020 2020  ).        ).    
+0000d400: 2020 2020 6220 3d20 6e70 2e68 7374 6163      b = np.hstac
+0000d410: 6b28 2863 656e 7465 7220 2d20 6478 2c20  k((center - dx, 
+0000d420: 6365 6e74 6572 202b 2064 7829 290a 0a20  center + dx)).. 
+0000d430: 2020 2020 2020 2070 6c6f 7473 5f74 6f5f         plots_to_
+0000d440: 6f76 6572 6c61 7920 3d20 5b5d 0a20 2020  overlay = [].   
+0000d450: 2020 2020 206c 6179 6572 735f 6578 636c       layers_excl
+0000d460: 7564 6564 203d 205b 5d20 6966 206c 6179  uded = [] if lay
+0000d470: 6572 735f 6578 636c 7564 6564 2069 7320  ers_excluded is 
+0000d480: 4e6f 6e65 2065 6c73 6520 6c61 7965 7273  None else layers
+0000d490: 5f65 7863 6c75 6465 640a 0a20 2020 2020  _excluded..     
+0000d4a0: 2020 2066 6f72 206c 6179 6572 2c20 706f     for layer, po
+0000d4b0: 6c79 676f 6e20 696e 2073 656c 662e 6765  lygon in self.ge
+0000d4c0: 745f 706f 6c79 676f 6e73 2862 795f 7370  t_polygons(by_sp
+0000d4d0: 6563 3d54 7275 6529 2e69 7465 6d73 2829  ec=True).items()
+0000d4e0: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
+0000d4f0: 206c 6179 6572 2069 6e20 6c61 7965 7273   layer in layers
+0000d500: 5f65 7863 6c75 6465 643a 0a20 2020 2020  _excluded:.     
+0000d510: 2020 2020 2020 2020 2020 2063 6f6e 7469             conti
+0000d520: 6e75 650a 0a20 2020 2020 2020 2020 2020  nue..           
+0000d530: 2074 7279 3a0a 2020 2020 2020 2020 2020   try:.          
+0000d540: 2020 2020 2020 6c61 7965 725f 7669 6577        layer_view
+0000d550: 203d 206c 6179 6572 5f76 6965 7773 2e67   = layer_views.g
+0000d560: 6574 5f66 726f 6d5f 7475 706c 6528 6c61  et_from_tuple(la
+0000d570: 7965 7229 0a20 2020 2020 2020 2020 2020  yer).           
+0000d580: 2065 7863 6570 7420 5661 6c75 6545 7272   except ValueErr
+0000d590: 6f72 3a0a 2020 2020 2020 2020 2020 2020  or:.            
+0000d5a0: 2020 2020 6c61 7965 7273 203d 206c 6973      layers = lis
+0000d5b0: 7428 6c61 7965 725f 7669 6577 732e 6765  t(layer_views.ge
+0000d5c0: 745f 6c61 7965 725f 7669 6577 7328 292e  t_layer_views().
+0000d5d0: 6b65 7973 2829 290a 2020 2020 2020 2020  keys()).        
+0000d5e0: 2020 2020 2020 2020 7761 726e 696e 6773          warnings
+0000d5f0: 2e77 6172 6e28 6622 7b6c 6179 6572 2172  .warn(f"{layer!r
+0000d600: 7d20 6e6f 7420 6465 6669 6e65 6420 696e  } not defined in
+0000d610: 207b 6c61 7965 7273 7d22 290a 2020 2020   {layers}").    
+0000d620: 2020 2020 2020 2020 2020 2020 6c61 7965              laye
+0000d630: 725f 7669 6577 203d 204c 6179 6572 5669  r_view = LayerVi
+0000d640: 6577 286c 6179 6572 3d6c 6179 6572 290a  ew(layer=layer).
+0000d650: 2020 2020 2020 2020 2020 2020 2320 544f              # TO
+0000d660: 444f 3a20 4d61 7463 6820 7570 206f 7074  DO: Match up opt
+0000d670: 696f 6e73 2077 6974 6820 4c61 7965 7256  ions with LayerV
+0000d680: 6965 7773 0a20 2020 2020 2020 2020 2020  iews.           
+0000d690: 2070 6c6f 7473 5f74 6f5f 6f76 6572 6c61   plots_to_overla
+0000d6a0: 792e 6170 7065 6e64 280a 2020 2020 2020  y.append(.      
+0000d6b0: 2020 2020 2020 2020 2020 6876 2e50 6f6c            hv.Pol
+0000d6c0: 7967 6f6e 7328 706f 6c79 676f 6e2c 206c  ygons(polygon, l
+0000d6d0: 6162 656c 3d73 7472 286c 6179 6572 5f76  abel=str(layer_v
+0000d6e0: 6965 772e 6e61 6d65 2929 2e6f 7074 7328  iew.name)).opts(
+0000d6f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000d700: 2020 2020 2064 6174 615f 6173 7065 6374       data_aspect
+0000d710: 3d31 2c0a 2020 2020 2020 2020 2020 2020  =1,.            
+0000d720: 2020 2020 2020 2020 6672 616d 655f 7769          frame_wi
+0000d730: 6474 683d 3530 302c 0a20 2020 2020 2020  dth=500,.       
+0000d740: 2020 2020 2020 2020 2020 2020 2079 6c69               yli
+0000d750: 6d3d 2862 5b31 5d2c 2062 5b33 5d29 2c0a  m=(b[1], b[3]),.
+0000d760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d770: 2020 2020 786c 696d 3d28 625b 305d 2c20      xlim=(b[0], 
+0000d780: 625b 325d 292c 0a20 2020 2020 2020 2020  b[2]),.         
+0000d790: 2020 2020 2020 2020 2020 2066 696c 6c5f             fill_
+0000d7a0: 636f 6c6f 723d 6c61 7965 725f 7669 6577  color=layer_view
+0000d7b0: 2e66 696c 6c5f 636f 6c6f 722e 6173 5f72  .fill_color.as_r
+0000d7c0: 6762 2829 206f 7220 2222 2c0a 2020 2020  gb() or "",.    
+0000d7d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d7e0: 6c69 6e65 5f63 6f6c 6f72 3d6c 6179 6572  line_color=layer
+0000d7f0: 5f76 6965 772e 6672 616d 655f 636f 6c6f  _view.frame_colo
+0000d800: 722e 6173 5f72 6762 2829 206f 7220 2222  r.as_rgb() or ""
+0000d810: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000d820: 2020 2020 2020 6669 6c6c 5f61 6c70 6861        fill_alpha
+0000d830: 3d6c 6179 6572 5f76 6965 772e 6765 745f  =layer_view.get_
+0000d840: 616c 7068 6128 2920 6f72 2022 222c 0a20  alpha() or "",. 
+0000d850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d860: 2020 206c 696e 655f 616c 7068 613d 6c61     line_alpha=la
+0000d870: 7965 725f 7669 6577 2e67 6574 5f61 6c70  yer_view.get_alp
+0000d880: 6861 2829 206f 7220 2222 2c0a 2020 2020  ha() or "",.    
+0000d890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d8a0: 746f 6f6c 733d 5b22 686f 7665 7222 5d2c  tools=["hover"],
+0000d8b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000d8c0: 2029 0a20 2020 2020 2020 2020 2020 2029   ).            )
+0000d8d0: 0a20 2020 2020 2020 2066 6f72 206e 616d  .        for nam
+0000d8e0: 652c 2070 6f72 7420 696e 2073 656c 662e  e, port in self.
+0000d8f0: 706f 7274 732e 6974 656d 7328 293a 0a20  ports.items():. 
+0000d900: 2020 2020 2020 2020 2020 206e 616d 6520             name 
+0000d910: 3d20 7374 7228 6e61 6d65 290a 2020 2020  = str(name).    
+0000d920: 2020 2020 2020 2020 706f 6c79 676f 6e2c          polygon,
+0000d930: 2070 7469 7020 3d20 6765 745f 7069 6e5f   ptip = get_pin_
+0000d940: 7472 6961 6e67 6c65 5f70 6f6c 7967 6f6e  triangle_polygon
+0000d950: 5f74 6970 2870 6f72 743d 706f 7274 290a  _tip(port=port).
+0000d960: 0a20 2020 2020 2020 2020 2020 2070 6c6f  .            plo
+0000d970: 7473 5f74 6f5f 6f76 6572 6c61 792e 6170  ts_to_overlay.ap
+0000d980: 7065 6e64 280a 2020 2020 2020 2020 2020  pend(.          
+0000d990: 2020 2020 2020 6876 2e50 6f6c 7967 6f6e        hv.Polygon
+0000d9a0: 7328 706f 6c79 676f 6e2c 206c 6162 656c  s(polygon, label
+0000d9b0: 3d6e 616d 6529 2e6f 7074 7328 0a20 2020  =name).opts(.   
+0000d9c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d9d0: 2064 6174 615f 6173 7065 6374 3d31 2c0a   data_aspect=1,.
+0000d9e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d9f0: 2020 2020 6672 616d 655f 7769 6474 683d      frame_width=
+0000da00: 3530 302c 0a20 2020 2020 2020 2020 2020  500,.           
+0000da10: 2020 2020 2020 2020 2066 696c 6c5f 616c           fill_al
+0000da20: 7068 613d 302c 0a20 2020 2020 2020 2020  pha=0,.         
+0000da30: 2020 2020 2020 2020 2020 2079 6c69 6d3d             ylim=
+0000da40: 2862 5b31 5d2c 2062 5b33 5d29 2c0a 2020  (b[1], b[3]),.  
+0000da50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000da60: 2020 786c 696d 3d28 625b 305d 2c20 625b    xlim=(b[0], b[
+0000da70: 325d 292c 0a20 2020 2020 2020 2020 2020  2]),.           
+0000da80: 2020 2020 2020 2020 2063 6f6c 6f72 3d22           color="
+0000da90: 7265 6422 2c0a 2020 2020 2020 2020 2020  red",.          
+0000daa0: 2020 2020 2020 2020 2020 6c69 6e65 5f61            line_a
+0000dab0: 6c70 6861 3d6c 6179 6572 5f76 6965 772e  lpha=layer_view.
+0000dac0: 6765 745f 616c 7068 6128 2920 6f72 2022  get_alpha() or "
+0000dad0: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+0000dae0: 2020 2020 2020 2074 6f6f 6c73 3d5b 2268         tools=["h
+0000daf0: 6f76 6572 225d 2c0a 2020 2020 2020 2020  over"],.        
+0000db00: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+0000db10: 2020 2020 2020 2020 2020 2a20 6876 2e54            * hv.T
+0000db20: 6578 7428 7074 6970 5b30 5d2c 2070 7469  ext(ptip[0], pti
+0000db30: 705b 315d 2c20 6e61 6d65 290a 2020 2020  p[1], name).    
+0000db40: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
+0000db50: 2020 2072 6574 7572 6e20 6876 2e4f 7665     return hv.Ove
+0000db60: 726c 6179 2870 6c6f 7473 5f74 6f5f 6f76  rlay(plots_to_ov
+0000db70: 6572 6c61 7929 2e6f 7074 7328 0a20 2020  erlay).opts(.   
+0000db80: 2020 2020 2020 2020 2073 686f 775f 6c65           show_le
+0000db90: 6765 6e64 3d54 7275 652c 2073 6861 7265  gend=True, share
+0000dba0: 645f 6178 6573 3d46 616c 7365 2c20 796c  d_axes=False, yl
+0000dbb0: 696d 3d28 625b 315d 2c20 625b 335d 292c  im=(b[1], b[3]),
+0000dbc0: 2078 6c69 6d3d 2862 5b30 5d2c 2062 5b32   xlim=(b[0], b[2
+0000dbd0: 5d29 0a20 2020 2020 2020 2029 0a0a 2020  ]).        )..  
+0000dbe0: 2020 6465 6620 7368 6f77 280a 2020 2020    def show(.    
+0000dbf0: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
+0000dc00: 2020 7368 6f77 5f70 6f72 7473 3a20 626f    show_ports: bo
+0000dc10: 6f6c 203d 2046 616c 7365 2c0a 2020 2020  ol = False,.    
+0000dc20: 2020 2020 7368 6f77 5f73 7562 706f 7274      show_subport
+0000dc30: 733a 2062 6f6f 6c20 3d20 4661 6c73 652c  s: bool = False,
+0000dc40: 0a20 2020 2020 2020 2070 6f72 745f 6d61  .        port_ma
+0000dc50: 726b 6572 5f6c 6179 6572 3a20 4c61 7965  rker_layer: Laye
+0000dc60: 7220 3d20 2831 2c20 3130 292c 0a20 2020  r = (1, 10),.   
+0000dc70: 2020 2020 202a 2a6b 7761 7267 732c 0a20       **kwargs,. 
+0000dc80: 2020 2029 202d 3e20 4e6f 6e65 3a0a 2020     ) -> None:.  
+0000dc90: 2020 2020 2020 2222 2253 686f 7720 636f        """Show co
+0000dca0: 6d70 6f6e 656e 7420 696e 204b 4c61 796f  mponent in KLayo
+0000dcb0: 7574 2e0a 0a20 2020 2020 2020 2072 6574  ut...        ret
+0000dcc0: 7572 6e73 2061 2063 6f70 7920 6f66 2074  urns a copy of t
+0000dcd0: 6865 2043 6f6d 706f 6e65 6e74 2c20 736f  he Component, so
+0000dce0: 2074 6865 206f 7269 6769 6e61 6c20 636f   the original co
+0000dcf0: 6d70 6f6e 656e 7420 7265 6d61 696e 7320  mponent remains 
+0000dd00: 696e 7461 6374 2e0a 2020 2020 2020 2020  intact..        
+0000dd10: 7769 7468 2070 696e 7320 6d61 726b 6572  with pins marker
+0000dd20: 7320 6f6e 2065 6163 6820 706f 7274 2073  s on each port s
+0000dd30: 686f 775f 706f 7274 7320 3d20 5472 7565  how_ports = True
+0000dd40: 2c20 616e 6420 6f70 7469 6f6e 616c 6c79  , and optionally
+0000dd50: 2061 6c73 6f0a 2020 2020 2020 2020 7468   also.        th
+0000dd60: 6520 706f 7274 7320 6672 6f6d 2074 6865  e ports from the
+0000dd70: 2072 6566 6572 656e 6365 7320 2873 686f   references (sho
+0000dd80: 775f 7375 6270 6f72 7473 3d54 7275 6529  w_subports=True)
+0000dd90: 0a0a 2020 2020 2020 2020 4172 6773 3a0a  ..        Args:.
+0000dda0: 2020 2020 2020 2020 2020 2020 7368 6f77              show
+0000ddb0: 5f70 6f72 7473 3a20 7368 6f77 7320 636f  _ports: shows co
+0000ddc0: 6d70 6f6e 656e 7420 7769 7468 2070 6f72  mponent with por
+0000ddd0: 7420 6d61 726b 6572 7320 616e 6420 6c61  t markers and la
+0000dde0: 6265 6c73 2e0a 2020 2020 2020 2020 2020  bels..          
+0000ddf0: 2020 7368 6f77 5f73 7562 706f 7274 733a    show_subports:
+0000de00: 2061 6464 2070 6f72 7473 206d 6172 6b65   add ports marke
+0000de10: 7273 2061 6e64 206c 6162 656c 7320 746f  rs and labels to
+0000de20: 2072 6566 6572 656e 6365 732e 0a20 2020   references..   
+0000de30: 2020 2020 2020 2020 2070 6f72 745f 6d61           port_ma
+0000de40: 726b 6572 5f6c 6179 6572 3a20 666f 7220  rker_layer: for 
+0000de50: 7468 6520 706f 7274 732e 0a0a 2020 2020  the ports...    
+0000de60: 2020 2020 4b65 7977 6f72 6420 4172 6773      Keyword Args
+0000de70: 3a0a 2020 2020 2020 2020 2020 2020 6764  :.            gd
+0000de80: 7370 6174 683a 2047 4453 2066 696c 6520  spath: GDS file 
+0000de90: 7061 7468 2074 6f20 7772 6974 6520 746f  path to write to
+0000dea0: 2e0a 2020 2020 2020 2020 2020 2020 6764  ..            gd
+0000deb0: 7364 6972 3a20 6469 7265 6374 6f72 7920  sdir: directory 
+0000dec0: 666f 7220 7468 6520 4744 5320 6669 6c65  for the GDS file
+0000ded0: 2e20 4465 6661 756c 7473 2074 6f20 2f74  . Defaults to /t
+0000dee0: 6d70 2f2e 0a20 2020 2020 2020 2020 2020  mp/..           
+0000def0: 2075 6e69 743a 2075 6e69 7420 7369 7a65   unit: unit size
+0000df00: 2066 6f72 206f 626a 6563 7473 2069 6e20   for objects in 
+0000df10: 6c69 6272 6172 792e 2031 756d 2062 7920  library. 1um by 
+0000df20: 6465 6661 756c 742e 0a20 2020 2020 2020  default..       
+0000df30: 2020 2020 2070 7265 6369 7369 6f6e 3a20       precision: 
+0000df40: 666f 7220 6f62 6a65 6374 2064 696d 656e  for object dimen
+0000df50: 7369 6f6e 7320 696e 2074 6865 206c 6962  sions in the lib
+0000df60: 7261 7279 2028 6d29 2e20 316e 6d20 6279  rary (m). 1nm by
+0000df70: 2064 6566 6175 6c74 2e0a 2020 2020 2020   default..      
+0000df80: 2020 2020 2020 7469 6d65 7374 616d 703a        timestamp:
+0000df90: 2044 6566 6175 6c74 7320 746f 2032 3031   Defaults to 201
+0000dfa0: 392d 3130 2d32 352e 2049 6620 4e6f 6e65  9-10-25. If None
+0000dfb0: 2075 7365 7320 6375 7272 656e 7420 7469   uses current ti
+0000dfc0: 6d65 2e0a 2020 2020 2020 2020 2222 220a  me..        """.
+0000dfd0: 2020 2020 2020 2020 6672 6f6d 2067 6473          from gds
+0000dfe0: 6661 6374 6f72 792e 6164 645f 7069 6e73  factory.add_pins
+0000dff0: 2069 6d70 6f72 7420 6164 645f 7069 6e73   import add_pins
+0000e000: 5f74 7269 616e 676c 650a 2020 2020 2020  _triangle.      
+0000e010: 2020 6672 6f6d 2067 6473 6661 6374 6f72    from gdsfactor
+0000e020: 792e 7368 6f77 2069 6d70 6f72 7420 7368  y.show import sh
+0000e030: 6f77 0a0a 2020 2020 2020 2020 636f 6d70  ow..        comp
+0000e040: 6f6e 656e 7420 3d20 280a 2020 2020 2020  onent = (.      
+0000e050: 2020 2020 2020 7365 6c66 2e61 6464 5f70        self.add_p
+0000e060: 696e 735f 7472 6961 6e67 6c65 2870 6f72  ins_triangle(por
+0000e070: 745f 6d61 726b 6572 5f6c 6179 6572 3d70  t_marker_layer=p
+0000e080: 6f72 745f 6d61 726b 6572 5f6c 6179 6572  ort_marker_layer
+0000e090: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
+0000e0a0: 2073 686f 775f 706f 7274 730a 2020 2020   show_ports.    
+0000e0b0: 2020 2020 2020 2020 656c 7365 2073 656c          else sel
+0000e0c0: 660a 2020 2020 2020 2020 290a 0a20 2020  f.        )..   
+0000e0d0: 2020 2020 2069 6620 7368 6f77 5f73 7562       if show_sub
+0000e0e0: 706f 7274 733a 0a20 2020 2020 2020 2020  ports:.         
+0000e0f0: 2020 2063 6f6d 706f 6e65 6e74 203d 2073     component = s
+0000e100: 656c 662e 636f 7079 2829 0a20 2020 2020  elf.copy().     
+0000e110: 2020 2020 2020 2063 6f6d 706f 6e65 6e74         component
+0000e120: 2e6e 616d 6520 3d20 7365 6c66 2e6e 616d  .name = self.nam
+0000e130: 650a 2020 2020 2020 2020 2020 2020 666f  e.            fo
+0000e140: 7220 7265 6665 7265 6e63 6520 696e 2063  r reference in c
+0000e150: 6f6d 706f 6e65 6e74 2e72 6566 6572 656e  omponent.referen
+0000e160: 6365 733a 0a20 2020 2020 2020 2020 2020  ces:.           
+0000e170: 2020 2020 2069 6620 6973 696e 7374 616e       if isinstan
+0000e180: 6365 2863 6f6d 706f 6e65 6e74 2c20 436f  ce(component, Co
+0000e190: 6d70 6f6e 656e 7452 6566 6572 656e 6365  mponentReference
+0000e1a0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+0000e1b0: 2020 2020 2020 2061 6464 5f70 696e 735f         add_pins_
+0000e1c0: 7472 6961 6e67 6c65 280a 2020 2020 2020  triangle(.      
+0000e1d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e1e0: 2020 636f 6d70 6f6e 656e 743d 636f 6d70    component=comp
+0000e1f0: 6f6e 656e 742c 0a20 2020 2020 2020 2020  onent,.         
+0000e200: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+0000e210: 6566 6572 656e 6365 3d72 6566 6572 656e  eference=referen
+0000e220: 6365 2c0a 2020 2020 2020 2020 2020 2020  ce,.            
+0000e230: 2020 2020 2020 2020 2020 2020 6c61 7965              laye
+0000e240: 723d 706f 7274 5f6d 6172 6b65 725f 6c61  r=port_marker_la
+0000e250: 7965 722c 0a20 2020 2020 2020 2020 2020  yer,.           
+0000e260: 2020 2020 2020 2020 2029 0a0a 2020 2020           )..    
+0000e270: 2020 2020 7368 6f77 2863 6f6d 706f 6e65      show(compone
+0000e280: 6e74 2c20 2a2a 6b77 6172 6773 290a 0a20  nt, **kwargs).. 
+0000e290: 2020 2064 6566 205f 7772 6974 655f 6c69     def _write_li
+0000e2a0: 6272 6172 7928 0a20 2020 2020 2020 2073  brary(.        s
+0000e2b0: 656c 662c 0a20 2020 2020 2020 2067 6473  elf,.        gds
+0000e2c0: 7061 7468 3a20 4f70 7469 6f6e 616c 5b50  path: Optional[P
+0000e2d0: 6174 6854 7970 655d 203d 204e 6f6e 652c  athType] = None,
+0000e2e0: 0a20 2020 2020 2020 2067 6473 6469 723a  .        gdsdir:
+0000e2f0: 204f 7074 696f 6e61 6c5b 5061 7468 5479   Optional[PathTy
+0000e300: 7065 5d20 3d20 4e6f 6e65 2c0a 2020 2020  pe] = None,.    
+0000e310: 2020 2020 7469 6d65 7374 616d 703a 204f      timestamp: O
+0000e320: 7074 696f 6e61 6c5b 6461 7465 7469 6d65  ptional[datetime
+0000e330: 2e64 6174 6574 696d 655d 203d 205f 7469  .datetime] = _ti
+0000e340: 6d65 7374 616d 7032 3031 392c 0a20 2020  mestamp2019,.   
+0000e350: 2020 2020 206c 6f67 6769 6e67 3a20 626f       logging: bo
+0000e360: 6f6c 203d 2054 7275 652c 0a20 2020 2020  ol = True,.     
+0000e370: 2020 2077 6974 685f 6f61 7369 733a 2062     with_oasis: b
+0000e380: 6f6f 6c20 3d20 4661 6c73 652c 0a20 2020  ool = False,.   
+0000e390: 2020 2020 202a 2a6b 7761 7267 732c 0a20       **kwargs,. 
+0000e3a0: 2020 2029 202d 3e20 5061 7468 3a0a 2020     ) -> Path:.  
+0000e3b0: 2020 2020 2020 2222 2257 7269 7465 2063        """Write c
+0000e3c0: 6f6d 706f 6e65 6e74 2074 6f20 4744 5320  omponent to GDS 
+0000e3d0: 6f72 204f 4153 4953 2061 6e64 2072 6574  or OASIS and ret
+0000e3e0: 7572 6e73 2067 6473 7061 7468 2e0a 0a20  urns gdspath... 
+0000e3f0: 2020 2020 2020 2041 7267 733a 0a20 2020         Args:.   
+0000e400: 2020 2020 2020 2020 2067 6473 7061 7468           gdspath
+0000e410: 3a20 4744 5320 6669 6c65 2070 6174 6820  : GDS file path 
+0000e420: 746f 2077 7269 7465 2074 6f2e 0a20 2020  to write to..   
+0000e430: 2020 2020 2020 2020 2067 6473 6469 723a           gdsdir:
+0000e440: 2064 6972 6563 746f 7279 2066 6f72 2074   directory for t
+0000e450: 6865 2047 4453 2066 696c 652e 2044 6566  he GDS file. Def
+0000e460: 6175 6c74 7320 746f 202f 746d 702f 7261  aults to /tmp/ra
+0000e470: 6e64 6f6d 4669 6c65 2f67 6473 6661 6374  ndomFile/gdsfact
+0000e480: 6f72 792e 0a20 2020 2020 2020 2020 2020  ory..           
+0000e490: 2074 696d 6573 7461 6d70 3a20 4465 6661   timestamp: Defa
+0000e4a0: 756c 7473 2074 6f20 3230 3139 2d31 302d  ults to 2019-10-
+0000e4b0: 3235 2066 6f72 2063 6f6e 7369 7374 656e  25 for consisten
+0000e4c0: 7420 6861 7368 2e0a 2020 2020 2020 2020  t hash..        
+0000e4d0: 2020 2020 2020 2020 4966 204e 6f6e 6520          If None 
+0000e4e0: 7573 6573 2063 7572 7265 6e74 2074 696d  uses current tim
+0000e4f0: 652e 0a20 2020 2020 2020 2020 2020 206c  e..            l
+0000e500: 6f67 6769 6e67 3a20 6469 7361 626c 6520  ogging: disable 
+0000e510: 4744 5320 7061 7468 206c 6f67 6769 6e67  GDS path logging
+0000e520: 2c20 666f 7220 6578 616d 706c 6520 666f  , for example fo
+0000e530: 7220 7368 6f77 696e 6720 6974 2069 6e20  r showing it in 
+0000e540: 4b4c 6179 6f75 742e 0a20 2020 2020 2020  KLayout..       
+0000e550: 2020 2020 2077 6974 685f 6f61 7369 733a       with_oasis:
+0000e560: 2049 6620 5472 7565 2c20 6669 6c65 2077   If True, file w
+0000e570: 696c 6c20 6265 2077 7269 7474 656e 2074  ill be written t
+0000e580: 6f20 4f41 5349 532e 204f 7468 6572 7769  o OASIS. Otherwi
+0000e590: 7365 2c20 6669 6c65 2077 696c 6c20 6265  se, file will be
+0000e5a0: 2077 7269 7474 656e 2074 6f20 4744 532e   written to GDS.
+0000e5b0: 0a0a 2020 2020 2020 2020 4b65 7977 6f72  ..        Keywor
+0000e5c0: 6420 4172 6773 3a0a 2020 2020 2020 2020  d Args:.        
+0000e5d0: 2020 2020 4b65 7977 6f72 6420 6172 6775      Keyword argu
+0000e5e0: 6d65 6e74 7320 7769 6c6c 206f 7665 7272  ments will overr
+0000e5f0: 6964 6520 7468 6520 6163 7469 7665 2050  ide the active P
+0000e600: 444b 2773 2064 6566 6175 6c74 2047 6473  DK's default Gds
+0000e610: 5772 6974 6553 6574 7469 6e67 7320 616e  WriteSettings an
+0000e620: 6420 4f61 7369 7357 7269 7465 5365 7474  d OasisWriteSett
+0000e630: 696e 6773 2e0a 0a20 2020 2020 2020 2020  ings...         
+0000e640: 2020 2047 6473 2073 6574 7469 6e67 733a     Gds settings:
+0000e650: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000e660: 2075 6e69 743a 2075 6e69 7420 7369 7a65   unit: unit size
+0000e670: 2066 6f72 206f 626a 6563 7473 2069 6e20   for objects in 
+0000e680: 6c69 6272 6172 792e 2031 756d 2062 7920  library. 1um by 
+0000e690: 6465 6661 756c 742e 0a20 2020 2020 2020  default..       
+0000e6a0: 2020 2020 2020 2020 2070 7265 6369 7369           precisi
+0000e6b0: 6f6e 3a20 666f 7220 6469 6d65 6e73 696f  on: for dimensio
+0000e6c0: 6e73 2069 6e20 7468 6520 6c69 6272 6172  ns in the librar
+0000e6d0: 7920 286d 292e 2031 6e6d 2062 7920 6465  y (m). 1nm by de
+0000e6e0: 6661 756c 742e 0a20 2020 2020 2020 2020  fault..         
+0000e6f0: 2020 2020 2020 206f 6e5f 6475 706c 6963         on_duplic
+0000e700: 6174 655f 6365 6c6c 3a20 7370 6563 6966  ate_cell: specif
+0000e710: 7920 686f 7720 746f 2072 6573 6f6c 7665  y how to resolve
+0000e720: 2064 7570 6c69 6361 7465 2d6e 616d 6564   duplicate-named
+0000e730: 2063 656c 6c73 2e20 4368 6f6f 7365 206f   cells. Choose o
+0000e740: 6e65 206f 6620 7468 6520 666f 6c6c 6f77  ne of the follow
+0000e750: 696e 673a 0a20 2020 2020 2020 2020 2020  ing:.           
+0000e760: 2020 2020 2020 2020 2022 7761 726e 2220           "warn" 
+0000e770: 2864 6566 6175 6c74 293a 206f 7665 7277  (default): overw
+0000e780: 7269 7465 2061 6c6c 2064 7570 6c69 6361  rite all duplica
+0000e790: 7465 2063 656c 6c73 2077 6974 6820 6f6e  te cells with on
+0000e7a0: 6520 6f66 2074 6865 2064 7570 6c69 6361  e of the duplica
+0000e7b0: 7465 7320 2861 7262 6974 7261 7269 6c79  tes (arbitrarily
+0000e7c0: 292e 0a20 2020 2020 2020 2020 2020 2020  )..             
+0000e7d0: 2020 2020 2020 2022 6572 726f 7222 3a20         "error": 
+0000e7e0: 7468 726f 7720 6120 5661 6c75 6545 7272  throw a ValueErr
+0000e7f0: 6f72 2077 6865 6e20 6174 7465 6d70 7469  or when attempti
+0000e800: 6e67 2074 6f20 7772 6974 6520 6120 6764  ng to write a gd
+0000e810: 7320 7769 7468 2064 7570 6c69 6361 7465  s with duplicate
+0000e820: 2063 656c 6c73 2e0a 2020 2020 2020 2020   cells..        
+0000e830: 2020 2020 2020 2020 2020 2020 226f 7665              "ove
+0000e840: 7277 7269 7465 223a 206f 7665 7277 7269  rwrite": overwri
+0000e850: 7465 2061 6c6c 2064 7570 6c69 6361 7465  te all duplicate
+0000e860: 2063 656c 6c73 2077 6974 6820 6f6e 6520   cells with one 
+0000e870: 6f66 2074 6865 2064 7570 6c69 6361 7465  of the duplicate
+0000e880: 732c 2077 6974 686f 7574 2077 6172 6e69  s, without warni
+0000e890: 6e67 2e0a 2020 2020 2020 2020 2020 2020  ng..            
+0000e8a0: 2020 2020 2020 2020 4e6f 6e65 3a20 646f          None: do
+0000e8b0: 206e 6f74 2074 7279 2074 6f20 7265 736f   not try to reso
+0000e8c0: 6c76 6520 2861 7420 796f 7572 206f 776e  lve (at your own
+0000e8d0: 2072 6973 6b21 290a 2020 2020 2020 2020   risk!).        
+0000e8e0: 2020 2020 2020 2020 666c 6174 7465 6e5f          flatten_
+0000e8f0: 696e 7661 6c69 645f 7265 6673 3a20 666c  invalid_refs: fl
+0000e900: 6174 7465 6e73 2063 6f6d 706f 6e65 6e74  attens component
+0000e910: 2072 6566 6572 656e 6365 7320 7768 6963   references whic
+0000e920: 6820 6861 7665 2069 6e76 616c 6964 2074  h have invalid t
+0000e930: 7261 6e73 666f 726d 6174 696f 6e73 2e0a  ransformations..
+0000e940: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e950: 6d61 785f 706f 696e 7473 3a20 4d61 7869  max_points: Maxi
+0000e960: 6d61 6c20 6e75 6d62 6572 206f 6620 7665  mal number of ve
+0000e970: 7274 6963 6573 2070 6572 2070 6f6c 7967  rtices per polyg
+0000e980: 6f6e 2e20 506f 6c79 676f 6e73 2077 6974  on. Polygons wit
+0000e990: 6820 6d6f 7265 2076 6572 7469 6365 7320  h more vertices 
+0000e9a0: 7468 6174 2074 6869 7320 6172 6520 6175  that this are au
+0000e9b0: 746f 6d61 7469 6361 6c6c 7920 6672 6163  tomatically frac
+0000e9c0: 7475 7265 642e 0a0a 2020 2020 2020 2020  tured...        
+0000e9d0: 2020 2020 4f61 7369 7320 7365 7474 696e      Oasis settin
+0000e9e0: 6773 3a0a 2020 2020 2020 2020 2020 2020  gs:.            
+0000e9f0: 2020 2020 636f 6d70 7265 7373 696f 6e5f      compression_
+0000ea00: 6c65 7665 6c3a 204c 6576 656c 206f 6620  level: Level of 
+0000ea10: 636f 6d70 7265 7373 696f 6e20 666f 7220  compression for 
+0000ea20: 6365 6c6c 7320 2862 6574 7765 656e 2030  cells (between 0
+0000ea30: 2061 6e64 2039 292e 0a20 2020 2020 2020   and 9)..       
+0000ea40: 2020 2020 2020 2020 2020 2020 2053 6574               Set
+0000ea50: 7469 6e67 2074 6f20 3020 7769 6c6c 2064  ting to 0 will d
+0000ea60: 6973 6162 6c65 2063 656c 6c20 636f 6d70  isable cell comp
+0000ea70: 7265 7373 696f 6e2c 2031 2067 6976 6573  ression, 1 gives
+0000ea80: 2074 6865 2062 6573 7420 7370 6565 6420   the best speed 
+0000ea90: 616e 6420 392c 2074 6865 2062 6573 7420  and 9, the best 
+0000eaa0: 636f 6d70 7265 7373 696f 6e2e 0a20 2020  compression..   
+0000eab0: 2020 2020 2020 2020 2020 2020 2064 6574               det
+0000eac0: 6563 745f 7265 6374 616e 676c 6573 3a20  ect_rectangles: 
+0000ead0: 5374 6f72 6520 7265 6374 616e 676c 6573  Store rectangles
+0000eae0: 2069 6e20 636f 6d70 7265 7373 6564 2066   in compressed f
+0000eaf0: 6f72 6d61 742e 0a20 2020 2020 2020 2020  ormat..         
+0000eb00: 2020 2020 2020 2064 6574 6563 745f 7472         detect_tr
+0000eb10: 6170 657a 6f69 6473 3a20 5374 6f72 6520  apezoids: Store 
+0000eb20: 7472 6170 657a 6f69 6473 2069 6e20 636f  trapezoids in co
+0000eb30: 6d70 7265 7373 6564 2066 6f72 6d61 742e  mpressed format.
+0000eb40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000eb50: 2063 6972 636c 655f 746f 6c65 7261 6e63   circle_toleranc
+0000eb60: 653a 2054 6f6c 6572 616e 6365 2066 6f72  e: Tolerance for
+0000eb70: 2064 6574 6563 7469 6e67 2063 6972 636c   detecting circl
+0000eb80: 6573 2e20 4966 206c 6573 7320 6f72 2065  es. If less or e
+0000eb90: 7175 616c 2074 6f20 302c 206e 6f20 6465  qual to 0, no de
+0000eba0: 7465 6374 696f 6e20 6973 2070 6572 666f  tection is perfo
+0000ebb0: 726d 6564 2e20 4369 7263 6c65 7320 6172  rmed. Circles ar
+0000ebc0: 6520 7374 6f72 6564 2069 6e20 636f 6d70  e stored in comp
+0000ebd0: 7265 7373 6564 2066 6f72 6d61 742e 0a20  ressed format.. 
+0000ebe0: 2020 2020 2020 2020 2020 2020 2020 2076                 v
+0000ebf0: 616c 6964 6174 696f 6e20 2822 6372 6333  alidation ("crc3
+0000ec00: 3222 2c20 2263 6865 636b 7375 6d33 3222  2", "checksum32"
+0000ec10: 2c20 4e6f 6e65 293a 2074 7970 6520 6f66  , None): type of
+0000ec20: 2076 616c 6964 6174 696f 6e20 746f 2069   validation to i
+0000ec30: 6e63 6c75 6465 2069 6e20 7468 6520 7361  nclude in the sa
+0000ec40: 7665 6420 6669 6c65 2e0a 2020 2020 2020  ved file..      
+0000ec50: 2020 2020 2020 2020 2020 7374 616e 6461            standa
+0000ec60: 7264 5f70 726f 7065 7274 6965 733a 2053  rd_properties: S
+0000ec70: 746f 7265 2073 7461 6e64 6172 6420 4f41  tore standard OA
+0000ec80: 5349 5320 7072 6f70 6572 7469 6573 2069  SIS properties i
+0000ec90: 6e20 7468 6520 6669 6c65 2e0a 0a20 2020  n the file...   
+0000eca0: 2020 2020 2022 2222 0a0a 2020 2020 2020       """..      
+0000ecb0: 2020 6672 6f6d 2067 6473 6661 6374 6f72    from gdsfactor
+0000ecc0: 792e 7064 6b20 696d 706f 7274 2067 6574  y.pdk import get
+0000ecd0: 5f61 6374 6976 655f 7064 6b0a 0a20 2020  _active_pdk..   
+0000ece0: 2020 2020 2069 6620 6764 7370 6174 6820       if gdspath 
+0000ecf0: 616e 6420 6764 7364 6972 3a0a 2020 2020  and gdsdir:.    
+0000ed00: 2020 2020 2020 2020 7761 726e 696e 6773          warnings
+0000ed10: 2e77 6172 6e28 0a20 2020 2020 2020 2020  .warn(.         
+0000ed20: 2020 2020 2020 2022 6764 7370 6174 6820         "gdspath 
+0000ed30: 616e 6420 6764 7364 6972 2068 6176 6520  and gdsdir have 
+0000ed40: 626f 7468 2062 6565 6e20 7370 6563 6966  both been specif
+0000ed50: 6965 642e 2067 6473 7061 7468 2077 696c  ied. gdspath wil
+0000ed60: 6c20 7461 6b65 2070 7265 6365 6465 6e63  l take precedenc
+0000ed70: 6520 616e 6420 6764 7364 6972 2077 696c  e and gdsdir wil
+0000ed80: 6c20 6265 2069 676e 6f72 6564 2e22 0a20  l be ignored.". 
+0000ed90: 2020 2020 2020 2020 2020 2029 0a0a 2020             )..  
+0000eda0: 2020 2020 2020 6465 6661 756c 745f 7365        default_se
+0000edb0: 7474 696e 6773 203d 2067 6574 5f61 6374  ttings = get_act
+0000edc0: 6976 655f 7064 6b28 292e 6764 735f 7772  ive_pdk().gds_wr
+0000edd0: 6974 655f 7365 7474 696e 6773 0a20 2020  ite_settings.   
+0000ede0: 2020 2020 2064 6566 6175 6c74 5f6f 6173       default_oas
+0000edf0: 6973 5f73 6574 7469 6e67 7320 3d20 6765  is_settings = ge
+0000ee00: 745f 6163 7469 7665 5f70 646b 2829 2e6f  t_active_pdk().o
+0000ee10: 6173 6973 5f73 6574 7469 6e67 730a 0a20  asis_settings.. 
 0000ee20: 2020 2020 2020 2065 7870 6c69 6369 745f         explicit_
-0000ee30: 6f61 735f 7365 7474 696e 6773 203d 207b  oas_settings = {
+0000ee30: 6764 735f 7365 7474 696e 6773 203d 207b  gds_settings = {
 0000ee40: 0a20 2020 2020 2020 2020 2020 206b 3a20  .            k: 
 0000ee50: 760a 2020 2020 2020 2020 2020 2020 666f  v.            fo
 0000ee60: 7220 6b2c 2076 2069 6e20 6b77 6172 6773  r k, v in kwargs
 0000ee70: 2e69 7465 6d73 2829 0a20 2020 2020 2020  .items().       
 0000ee80: 2020 2020 2069 6620 7620 6973 206e 6f74       if v is not
 0000ee90: 204e 6f6e 6520 616e 6420 6b20 696e 2064   None and k in d
-0000eea0: 6566 6175 6c74 5f6f 6173 6973 5f73 6574  efault_oasis_set
-0000eeb0: 7469 6e67 732e 6469 6374 2829 0a20 2020  tings.dict().   
-0000eec0: 2020 2020 207d 0a20 2020 2020 2020 2023       }.        #
-0000eed0: 2075 7064 6174 6520 7468 6520 7772 6974   update the writ
-0000eee0: 6520 7365 7474 696e 6773 2077 6974 6820  e settings with 
-0000eef0: 616e 7920 7365 7474 696e 6773 2065 7870  any settings exp
-0000ef00: 6c69 6369 746c 7920 7061 7373 6564 0a20  licitly passed. 
-0000ef10: 2020 2020 2020 2077 7269 7465 5f73 6574         write_set
-0000ef20: 7469 6e67 7320 3d20 6465 6661 756c 745f  tings = default_
-0000ef30: 7365 7474 696e 6773 2e63 6f70 7928 7570  settings.copy(up
-0000ef40: 6461 7465 3d65 7870 6c69 6369 745f 6764  date=explicit_gd
-0000ef50: 735f 7365 7474 696e 6773 290a 2020 2020  s_settings).    
-0000ef60: 2020 2020 6f61 7369 735f 7365 7474 696e      oasis_settin
-0000ef70: 6773 203d 2064 6566 6175 6c74 5f6f 6173  gs = default_oas
-0000ef80: 6973 5f73 6574 7469 6e67 732e 636f 7079  is_settings.copy
-0000ef90: 2875 7064 6174 653d 6578 706c 6963 6974  (update=explicit
-0000efa0: 5f6f 6173 5f73 6574 7469 6e67 7329 0a0a  _oas_settings)..
-0000efb0: 2020 2020 2020 2020 5f63 6865 636b 5f75          _check_u
-0000efc0: 6e63 6163 6865 645f 636f 6d70 6f6e 656e  ncached_componen
-0000efd0: 7473 280a 2020 2020 2020 2020 2020 2020  ts(.            
-0000efe0: 636f 6d70 6f6e 656e 743d 7365 6c66 2c20  component=self, 
-0000eff0: 6d6f 6465 3d77 7269 7465 5f73 6574 7469  mode=write_setti
-0000f000: 6e67 732e 6f6e 5f75 6e63 6163 6865 645f  ngs.on_uncached_
-0000f010: 636f 6d70 6f6e 656e 740a 2020 2020 2020  component.      
-0000f020: 2020 290a 0a20 2020 2020 2020 2069 6620    )..        if 
-0000f030: 7772 6974 655f 7365 7474 696e 6773 2e66  write_settings.f
-0000f040: 6c61 7474 656e 5f69 6e76 616c 6964 5f72  latten_invalid_r
-0000f050: 6566 733a 0a20 2020 2020 2020 2020 2020  efs:.           
-0000f060: 2074 6f70 5f63 656c 6c20 3d20 666c 6174   top_cell = flat
-0000f070: 7465 6e5f 696e 7661 6c69 645f 7265 6673  ten_invalid_refs
-0000f080: 5f72 6563 7572 7369 7665 2873 656c 6629  _recursive(self)
-0000f090: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
-0000f0a0: 2020 2020 2020 2020 2020 2074 6f70 5f63             top_c
-0000f0b0: 656c 6c20 3d20 7365 6c66 0a0a 2020 2020  ell = self..    
-0000f0c0: 2020 2020 6764 7364 6972 203d 2067 6473      gdsdir = gds
-0000f0d0: 6469 7220 6f72 2047 4453 4449 525f 5445  dir or GDSDIR_TE
-0000f0e0: 4d50 0a20 2020 2020 2020 2067 6473 6469  MP.        gdsdi
-0000f0f0: 7220 3d20 7061 7468 6c69 622e 5061 7468  r = pathlib.Path
-0000f100: 2867 6473 6469 7229 0a20 2020 2020 2020  (gdsdir).       
-0000f110: 2069 6620 7769 7468 5f6f 6173 6973 3a0a   if with_oasis:.
-0000f120: 2020 2020 2020 2020 2020 2020 6764 7370              gdsp
-0000f130: 6174 6820 3d20 6764 7370 6174 6820 6f72  ath = gdspath or
-0000f140: 2067 6473 6469 7220 2f20 6622 7b74 6f70   gdsdir / f"{top
-0000f150: 5f63 656c 6c2e 6e61 6d65 7d2e 6f61 7322  _cell.name}.oas"
-0000f160: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
-0000f170: 2020 2020 2020 2020 2020 2067 6473 7061             gdspa
-0000f180: 7468 203d 2067 6473 7061 7468 206f 7220  th = gdspath or 
-0000f190: 6764 7364 6972 202f 2066 227b 746f 705f  gdsdir / f"{top_
-0000f1a0: 6365 6c6c 2e6e 616d 657d 2e67 6473 220a  cell.name}.gds".
-0000f1b0: 2020 2020 2020 2020 6764 7370 6174 6820          gdspath 
-0000f1c0: 3d20 7061 7468 6c69 622e 5061 7468 2867  = pathlib.Path(g
-0000f1d0: 6473 7061 7468 290a 2020 2020 2020 2020  dspath).        
-0000f1e0: 6764 7364 6972 203d 2067 6473 7061 7468  gdsdir = gdspath
-0000f1f0: 2e70 6172 656e 740a 2020 2020 2020 2020  .parent.        
-0000f200: 6764 7364 6972 2e6d 6b64 6972 2865 7869  gdsdir.mkdir(exi
-0000f210: 7374 5f6f 6b3d 5472 7565 2c20 7061 7265  st_ok=True, pare
-0000f220: 6e74 733d 5472 7565 290a 0a20 2020 2020  nts=True)..     
-0000f230: 2020 2063 656c 6c73 203d 2074 6f70 5f63     cells = top_c
-0000f240: 656c 6c2e 6765 745f 6465 7065 6e64 656e  ell.get_dependen
-0000f250: 6369 6573 2872 6563 7572 7369 7665 3d54  cies(recursive=T
-0000f260: 7275 6529 0a20 2020 2020 2020 2063 656c  rue).        cel
-0000f270: 6c5f 6e61 6d65 7320 3d20 5b63 656c 6c2e  l_names = [cell.
-0000f280: 6e61 6d65 2066 6f72 2063 656c 6c20 696e  name for cell in
-0000f290: 206c 6973 7428 6365 6c6c 7329 5d0a 2020   list(cells)].  
-0000f2a0: 2020 2020 2020 6365 6c6c 5f6e 616d 6573        cell_names
-0000f2b0: 5f75 6e69 7175 6520 3d20 7365 7428 6365  _unique = set(ce
-0000f2c0: 6c6c 5f6e 616d 6573 290a 0a20 2020 2020  ll_names)..     
-0000f2d0: 2020 2069 6620 6c65 6e28 6365 6c6c 5f6e     if len(cell_n
-0000f2e0: 616d 6573 2920 213d 206c 656e 2873 6574  ames) != len(set
-0000f2f0: 2863 656c 6c5f 6e61 6d65 7329 293a 0a20  (cell_names)):. 
-0000f300: 2020 2020 2020 2020 2020 2066 6f72 2063             for c
-0000f310: 656c 6c5f 6e61 6d65 2069 6e20 6365 6c6c  ell_name in cell
-0000f320: 5f6e 616d 6573 5f75 6e69 7175 653a 0a20  _names_unique:. 
-0000f330: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-0000f340: 656c 6c5f 6e61 6d65 732e 7265 6d6f 7665  ell_names.remove
-0000f350: 2863 656c 6c5f 6e61 6d65 290a 0a20 2020  (cell_name)..   
-0000f360: 2020 2020 2020 2020 2069 6620 7772 6974           if writ
-0000f370: 655f 7365 7474 696e 6773 2e6f 6e5f 6475  e_settings.on_du
-0000f380: 706c 6963 6174 655f 6365 6c6c 203d 3d20  plicate_cell == 
-0000f390: 2265 7272 6f72 223a 0a20 2020 2020 2020  "error":.       
-0000f3a0: 2020 2020 2020 2020 2072 6169 7365 2056           raise V
-0000f3b0: 616c 7565 4572 726f 7228 0a20 2020 2020  alueError(.     
-0000f3c0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
-0000f3d0: 2244 7570 6c69 6361 7465 6420 6365 6c6c  "Duplicated cell
-0000f3e0: 206e 616d 6573 2069 6e20 7b74 6f70 5f63   names in {top_c
-0000f3f0: 656c 6c2e 6e61 6d65 2172 7d3a 207b 6365  ell.name!r}: {ce
-0000f400: 6c6c 5f6e 616d 6573 2172 7d22 0a20 2020  ll_names!r}".   
-0000f410: 2020 2020 2020 2020 2020 2020 2029 0a20               ). 
-0000f420: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
-0000f430: 7772 6974 655f 7365 7474 696e 6773 2e6f  write_settings.o
-0000f440: 6e5f 6475 706c 6963 6174 655f 6365 6c6c  n_duplicate_cell
-0000f450: 2069 6e20 7b22 7761 726e 222c 2022 6f76   in {"warn", "ov
-0000f460: 6572 7772 6974 6522 7d3a 0a20 2020 2020  erwrite"}:.     
-0000f470: 2020 2020 2020 2020 2020 2069 6620 7772             if wr
-0000f480: 6974 655f 7365 7474 696e 6773 2e6f 6e5f  ite_settings.on_
-0000f490: 6475 706c 6963 6174 655f 6365 6c6c 203d  duplicate_cell =
-0000f4a0: 3d20 2277 6172 6e22 3a0a 2020 2020 2020  = "warn":.      
-0000f4b0: 2020 2020 2020 2020 2020 2020 2020 7761                wa
-0000f4c0: 726e 696e 6773 2e77 6172 6e28 0a20 2020  rnings.warn(.   
-0000f4d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f4e0: 2020 2020 2066 2244 7570 6c69 6361 7465       f"Duplicate
-0000f4f0: 6420 6365 6c6c 206e 616d 6573 2069 6e20  d cell names in 
-0000f500: 7b74 6f70 5f63 656c 6c2e 6e61 6d65 2172  {top_cell.name!r
-0000f510: 7d3a 2020 7b63 656c 6c5f 6e61 6d65 737d  }:  {cell_names}
-0000f520: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-0000f530: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-0000f540: 2020 2020 2020 2020 2063 656c 6c73 5f64           cells_d
-0000f550: 6963 7420 3d20 7b63 656c 6c2e 6e61 6d65  ict = {cell.name
-0000f560: 3a20 6365 6c6c 2e5f 6365 6c6c 2066 6f72  : cell._cell for
-0000f570: 2063 656c 6c20 696e 2063 656c 6c73 7d0a   cell in cells}.
-0000f580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f590: 6365 6c6c 7320 3d20 6365 6c6c 735f 6469  cells = cells_di
-0000f5a0: 6374 2e76 616c 7565 7328 290a 2020 2020  ct.values().    
-0000f5b0: 2020 2020 2020 2020 656c 6966 2077 7269          elif wri
-0000f5c0: 7465 5f73 6574 7469 6e67 732e 6f6e 5f64  te_settings.on_d
-0000f5d0: 7570 6c69 6361 7465 5f63 656c 6c20 6973  uplicate_cell is
-0000f5e0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-0000f5f0: 2020 2020 2020 2020 2020 2072 6169 7365             raise
-0000f600: 2056 616c 7565 4572 726f 7228 0a20 2020   ValueError(.   
-0000f610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f620: 2066 226f 6e5f 6475 706c 6963 6174 655f   f"on_duplicate_
-0000f630: 6365 6c6c 3a20 7b77 7269 7465 5f73 6574  cell: {write_set
-0000f640: 7469 6e67 732e 6f6e 5f64 7570 6c69 6361  tings.on_duplica
-0000f650: 7465 5f63 656c 6c21 727d 206e 6f74 2069  te_cell!r} not i
-0000f660: 6e20 284e 6f6e 652c 2077 6172 6e2c 2065  n (None, warn, e
-0000f670: 7272 6f72 2c20 6f76 6572 7772 6974 6529  rror, overwrite)
-0000f680: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-0000f690: 2020 290a 0a20 2020 2020 2020 2061 6c6c    )..        all
-0000f6a0: 5f63 656c 6c73 203d 205b 746f 705f 6365  _cells = [top_ce
-0000f6b0: 6c6c 2e5f 6365 6c6c 5d20 2b20 736f 7274  ll._cell] + sort
-0000f6c0: 6564 2863 656c 6c73 2c20 6b65 793d 6c61  ed(cells, key=la
-0000f6d0: 6d62 6461 2063 633a 2063 632e 6e61 6d65  mbda cc: cc.name
-0000f6e0: 290a 0a20 2020 2020 2020 206e 6f5f 6e61  )..        no_na
-0000f6f0: 6d65 5f63 656c 6c73 203d 205b 0a20 2020  me_cells = [.   
-0000f700: 2020 2020 2020 2020 2063 656c 6c2e 6e61           cell.na
-0000f710: 6d65 2066 6f72 2063 656c 6c20 696e 2061  me for cell in a
-0000f720: 6c6c 5f63 656c 6c73 2069 6620 6365 6c6c  ll_cells if cell
-0000f730: 2e6e 616d 652e 7374 6172 7473 7769 7468  .name.startswith
-0000f740: 2822 556e 6e61 6d65 6422 290a 2020 2020  ("Unnamed").    
-0000f750: 2020 2020 5d0a 0a20 2020 2020 2020 2069      ]..        i
-0000f760: 6620 6e6f 5f6e 616d 655f 6365 6c6c 733a  f no_name_cells:
-0000f770: 0a20 2020 2020 2020 2020 2020 2077 6172  .            war
-0000f780: 6e69 6e67 732e 7761 726e 280a 2020 2020  nings.warn(.    
-0000f790: 2020 2020 2020 2020 2020 2020 6622 436f              f"Co
-0000f7a0: 6d70 6f6e 656e 7420 7b74 6f70 5f63 656c  mponent {top_cel
-0000f7b0: 6c2e 6e61 6d65 2172 7d20 636f 6e74 6169  l.name!r} contai
-0000f7c0: 6e73 207b 6c65 6e28 6e6f 5f6e 616d 655f  ns {len(no_name_
-0000f7d0: 6365 6c6c 7329 7d20 556e 6e61 6d65 6420  cells)} Unnamed 
-0000f7e0: 6365 6c6c 7322 0a20 2020 2020 2020 2020  cells".         
-0000f7f0: 2020 2029 0a0a 2020 2020 2020 2020 2320     )..        # 
-0000f800: 666f 7220 6365 6c6c 2069 6e20 616c 6c5f  for cell in all_
-0000f810: 6365 6c6c 733a 0a20 2020 2020 2020 2023  cells:.        #
-0000f820: 2020 2020 2070 7269 6e74 2863 656c 6c2e       print(cell.
-0000f830: 6e61 6d65 2c20 7479 7065 2863 656c 6c29  name, type(cell)
-0000f840: 290a 0a20 2020 2020 2020 206c 6962 203d  )..        lib =
-0000f850: 2067 6473 746b 2e4c 6962 7261 7279 280a   gdstk.Library(.
-0000f860: 2020 2020 2020 2020 2020 2020 756e 6974              unit
-0000f870: 3d77 7269 7465 5f73 6574 7469 6e67 732e  =write_settings.
-0000f880: 756e 6974 2c20 7072 6563 6973 696f 6e3d  unit, precision=
-0000f890: 7772 6974 655f 7365 7474 696e 6773 2e70  write_settings.p
-0000f8a0: 7265 6369 7369 6f6e 0a20 2020 2020 2020  recision.       
-0000f8b0: 2029 0a20 2020 2020 2020 206c 6962 2e61   ).        lib.a
-0000f8c0: 6464 2874 6f70 5f63 656c 6c2e 5f63 656c  dd(top_cell._cel
-0000f8d0: 6c29 0a20 2020 2020 2020 206c 6962 2e61  l).        lib.a
-0000f8e0: 6464 282a 746f 705f 6365 6c6c 2e5f 6365  dd(*top_cell._ce
-0000f8f0: 6c6c 2e64 6570 656e 6465 6e63 6965 7328  ll.dependencies(
-0000f900: 5472 7565 2929 0a0a 2020 2020 2020 2020  True))..        
-0000f910: 6966 2077 6974 685f 6f61 7369 733a 0a20  if with_oasis:. 
-0000f920: 2020 2020 2020 2020 2020 206c 6962 2e77             lib.w
-0000f930: 7269 7465 5f6f 6173 2867 6473 7061 7468  rite_oas(gdspath
-0000f940: 2c20 2a2a 6f61 7369 735f 7365 7474 696e  , **oasis_settin
-0000f950: 6773 2e64 6963 7428 2929 0a20 2020 2020  gs.dict()).     
-0000f960: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-0000f970: 2020 2020 206c 6962 2e77 7269 7465 5f67       lib.write_g
-0000f980: 6473 280a 2020 2020 2020 2020 2020 2020  ds(.            
-0000f990: 2020 2020 6764 7370 6174 682c 2074 696d      gdspath, tim
-0000f9a0: 6573 7461 6d70 3d74 696d 6573 7461 6d70  estamp=timestamp
-0000f9b0: 2c20 6d61 785f 706f 696e 7473 3d77 7269  , max_points=wri
-0000f9c0: 7465 5f73 6574 7469 6e67 732e 6d61 785f  te_settings.max_
-0000f9d0: 706f 696e 7473 0a20 2020 2020 2020 2020  points.         
-0000f9e0: 2020 2029 0a20 2020 2020 2020 2069 6620     ).        if 
-0000f9f0: 6c6f 6767 696e 673a 0a20 2020 2020 2020  logging:.       
-0000fa00: 2020 2020 206c 6f67 6765 722e 696e 666f       logger.info
-0000fa10: 2866 2257 726f 7465 2074 6f20 7b73 7472  (f"Wrote to {str
-0000fa20: 2867 6473 7061 7468 2921 727d 2229 0a20  (gdspath)!r}"). 
-0000fa30: 2020 2020 2020 2072 6574 7572 6e20 6764         return gd
-0000fa40: 7370 6174 680a 0a20 2020 2064 6566 2077  spath..    def w
-0000fa50: 7269 7465 5f67 6473 280a 2020 2020 2020  rite_gds(.      
-0000fa60: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
-0000fa70: 6764 7370 6174 683a 204f 7074 696f 6e61  gdspath: Optiona
-0000fa80: 6c5b 5061 7468 5479 7065 5d20 3d20 4e6f  l[PathType] = No
-0000fa90: 6e65 2c0a 2020 2020 2020 2020 6764 7364  ne,.        gdsd
-0000faa0: 6972 3a20 4f70 7469 6f6e 616c 5b50 6174  ir: Optional[Pat
-0000fab0: 6854 7970 655d 203d 204e 6f6e 652c 0a20  hType] = None,. 
-0000fac0: 2020 2020 2020 202a 2a6b 7761 7267 732c         **kwargs,
-0000fad0: 0a20 2020 2029 202d 3e20 5061 7468 3a0a  .    ) -> Path:.
-0000fae0: 2020 2020 2020 2020 2222 2257 7269 7465          """Write
-0000faf0: 2063 6f6d 706f 6e65 6e74 2074 6f20 4744   component to GD
-0000fb00: 5320 616e 6420 7265 7475 726e 7320 6764  S and returns gd
-0000fb10: 7370 6174 682e 0a0a 2020 2020 2020 2020  spath...        
-0000fb20: 4172 6773 3a0a 2020 2020 2020 2020 2020  Args:.          
-0000fb30: 2020 6764 7370 6174 683a 2047 4453 2066    gdspath: GDS f
-0000fb40: 696c 6520 7061 7468 2074 6f20 7772 6974  ile path to writ
-0000fb50: 6520 746f 2e0a 2020 2020 2020 2020 2020  e to..          
-0000fb60: 2020 6764 7364 6972 3a20 6469 7265 6374    gdsdir: direct
-0000fb70: 6f72 7920 666f 7220 7468 6520 4744 5320  ory for the GDS 
-0000fb80: 6669 6c65 2e20 4465 6661 756c 7473 2074  file. Defaults t
-0000fb90: 6f20 2f74 6d70 2f72 616e 646f 6d46 696c  o /tmp/randomFil
-0000fba0: 652f 6764 7366 6163 746f 7279 2e0a 0a20  e/gdsfactory... 
-0000fbb0: 2020 2020 2020 204b 6579 776f 7264 2041         Keyword A
-0000fbc0: 7267 733a 0a20 2020 2020 2020 2020 2020  rgs:.           
-0000fbd0: 2075 6e69 743a 2075 6e69 7420 7369 7a65   unit: unit size
-0000fbe0: 2066 6f72 206f 626a 6563 7473 2069 6e20   for objects in 
-0000fbf0: 6c69 6272 6172 792e 2031 756d 2062 7920  library. 1um by 
-0000fc00: 6465 6661 756c 742e 0a20 2020 2020 2020  default..       
-0000fc10: 2020 2020 2070 7265 6369 7369 6f6e 3a20       precision: 
-0000fc20: 666f 7220 6469 6d65 6e73 696f 6e73 2069  for dimensions i
-0000fc30: 6e20 7468 6520 6c69 6272 6172 7920 286d  n the library (m
-0000fc40: 292e 2031 6e6d 2062 7920 6465 6661 756c  ). 1nm by defaul
-0000fc50: 742e 0a20 2020 2020 2020 2020 2020 206c  t..            l
-0000fc60: 6f67 6769 6e67 3a20 6469 7361 626c 6520  ogging: disable 
-0000fc70: 4744 5320 7061 7468 206c 6f67 6769 6e67  GDS path logging
-0000fc80: 2c20 666f 7220 6578 616d 706c 6520 666f  , for example fo
-0000fc90: 7220 7368 6f77 696e 6720 6974 2069 6e20  r showing it in 
-0000fca0: 4b4c 6179 6f75 742e 0a20 2020 2020 2020  KLayout..       
-0000fcb0: 2020 2020 206f 6e5f 6475 706c 6963 6174       on_duplicat
-0000fcc0: 655f 6365 6c6c 3a20 7370 6563 6966 7920  e_cell: specify 
-0000fcd0: 686f 7720 746f 2072 6573 6f6c 7665 2064  how to resolve d
-0000fce0: 7570 6c69 6361 7465 2d6e 616d 6564 2063  uplicate-named c
-0000fcf0: 656c 6c73 2e20 4368 6f6f 7365 206f 6e65  ells. Choose one
-0000fd00: 206f 6620 7468 6520 666f 6c6c 6f77 696e   of the followin
-0000fd10: 673a 0a20 2020 2020 2020 2020 2020 2020  g:.             
-0000fd20: 2020 2022 7761 726e 2220 2864 6566 6175     "warn" (defau
-0000fd30: 6c74 293a 206f 7665 7277 7269 7465 2061  lt): overwrite a
-0000fd40: 6c6c 2064 7570 6c69 6361 7465 2063 656c  ll duplicate cel
-0000fd50: 6c73 2077 6974 6820 6f6e 6520 6f66 2074  ls with one of t
-0000fd60: 6865 2064 7570 6c69 6361 7465 7320 2861  he duplicates (a
-0000fd70: 7262 6974 7261 7269 6c79 292e 0a20 2020  rbitrarily)..   
-0000fd80: 2020 2020 2020 2020 2020 2020 2022 6572               "er
-0000fd90: 726f 7222 3a20 7468 726f 7720 6120 5661  ror": throw a Va
-0000fda0: 6c75 6545 7272 6f72 2077 6865 6e20 6174  lueError when at
-0000fdb0: 7465 6d70 7469 6e67 2074 6f20 7772 6974  tempting to writ
-0000fdc0: 6520 6120 6764 7320 7769 7468 2064 7570  e a gds with dup
-0000fdd0: 6c69 6361 7465 2063 656c 6c73 2e0a 2020  licate cells..  
-0000fde0: 2020 2020 2020 2020 2020 2020 2020 226f                "o
-0000fdf0: 7665 7277 7269 7465 223a 206f 7665 7277  verwrite": overw
-0000fe00: 7269 7465 2061 6c6c 2064 7570 6c69 6361  rite all duplica
-0000fe10: 7465 2063 656c 6c73 2077 6974 6820 6f6e  te cells with on
-0000fe20: 6520 6f66 2074 6865 2064 7570 6c69 6361  e of the duplica
-0000fe30: 7465 732c 2077 6974 686f 7574 2077 6172  tes, without war
-0000fe40: 6e69 6e67 2e0a 2020 2020 2020 2020 2020  ning..          
-0000fe50: 2020 6f6e 5f75 6e63 6163 6865 645f 636f    on_uncached_co
-0000fe60: 6d70 6f6e 656e 743a 204c 6974 6572 616c  mponent: Literal
-0000fe70: 5b22 7761 726e 222c 2022 6572 726f 7222  ["warn", "error"
-0000fe80: 5d20 3d20 2277 6172 6e22 0a20 2020 2020  ] = "warn".     
-0000fe90: 2020 2020 2020 2066 6c61 7474 656e 5f69         flatten_i
-0000fea0: 6e76 616c 6964 5f72 6566 733a 2066 6c61  nvalid_refs: fla
-0000feb0: 7474 656e 7320 636f 6d70 6f6e 656e 7420  ttens component 
-0000fec0: 7265 6665 7265 6e63 6573 2077 6869 6368  references which
-0000fed0: 2068 6176 6520 696e 7661 6c69 6420 7472   have invalid tr
-0000fee0: 616e 7366 6f72 6d61 7469 6f6e 732e 0a20  ansformations.. 
-0000fef0: 2020 2020 2020 2020 2020 206d 6178 5f70             max_p
-0000ff00: 6f69 6e74 733a 204d 6178 696d 616c 206e  oints: Maximal n
-0000ff10: 756d 6265 7220 6f66 2076 6572 7469 6365  umber of vertice
-0000ff20: 7320 7065 7220 706f 6c79 676f 6e2e 0a20  s per polygon.. 
-0000ff30: 2020 2020 2020 2020 2020 2020 2020 2050                 P
-0000ff40: 6f6c 7967 6f6e 7320 7769 7468 206d 6f72  olygons with mor
-0000ff50: 6520 7665 7274 6963 6573 2074 6861 7420  e vertices that 
-0000ff60: 7468 6973 2061 7265 2061 7574 6f6d 6174  this are automat
-0000ff70: 6963 616c 6c79 2066 7261 6374 7572 6564  ically fractured
-0000ff80: 2e0a 2020 2020 2020 2020 2222 220a 0a20  ..        """.. 
-0000ff90: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-0000ffa0: 6c66 2e5f 7772 6974 655f 6c69 6272 6172  lf._write_librar
-0000ffb0: 7928 0a20 2020 2020 2020 2020 2020 2067  y(.            g
-0000ffc0: 6473 7061 7468 3d67 6473 7061 7468 2c20  dspath=gdspath, 
-0000ffd0: 6764 7364 6972 3d67 6473 6469 722c 2077  gdsdir=gdsdir, w
-0000ffe0: 6974 685f 6f61 7369 733d 4661 6c73 652c  ith_oasis=False,
-0000fff0: 202a 2a6b 7761 7267 730a 2020 2020 2020   **kwargs.      
-00010000: 2020 290a 0a20 2020 2064 6566 2077 7269    )..    def wri
-00010010: 7465 5f6f 6173 280a 2020 2020 2020 2020  te_oas(.        
-00010020: 7365 6c66 2c0a 2020 2020 2020 2020 6764  self,.        gd
-00010030: 7370 6174 683a 204f 7074 696f 6e61 6c5b  spath: Optional[
-00010040: 5061 7468 5479 7065 5d20 3d20 4e6f 6e65  PathType] = None
-00010050: 2c0a 2020 2020 2020 2020 6764 7364 6972  ,.        gdsdir
-00010060: 3a20 4f70 7469 6f6e 616c 5b50 6174 6854  : Optional[PathT
-00010070: 7970 655d 203d 204e 6f6e 652c 0a20 2020  ype] = None,.   
-00010080: 2020 2020 202a 2a6b 7761 7267 732c 0a20       **kwargs,. 
-00010090: 2020 2029 202d 3e20 5061 7468 3a0a 2020     ) -> Path:.  
-000100a0: 2020 2020 2020 2222 2257 7269 7465 2063        """Write c
-000100b0: 6f6d 706f 6e65 6e74 2074 6f20 4744 5320  omponent to GDS 
-000100c0: 616e 6420 7265 7475 726e 7320 6764 7370  and returns gdsp
-000100d0: 6174 682e 0a0a 2020 2020 2020 2020 4172  ath...        Ar
-000100e0: 6773 3a0a 2020 2020 2020 2020 2020 2020  gs:.            
-000100f0: 6764 7370 6174 683a 2047 4453 2066 696c  gdspath: GDS fil
-00010100: 6520 7061 7468 2074 6f20 7772 6974 6520  e path to write 
-00010110: 746f 2e0a 2020 2020 2020 2020 2020 2020  to..            
-00010120: 6764 7364 6972 3a20 6469 7265 6374 6f72  gdsdir: director
-00010130: 7920 666f 7220 7468 6520 4744 5320 6669  y for the GDS fi
-00010140: 6c65 2e20 4465 6661 756c 7473 2074 6f20  le. Defaults to 
-00010150: 2f74 6d70 2f72 616e 646f 6d46 696c 652f  /tmp/randomFile/
-00010160: 6764 7366 6163 746f 7279 2e0a 0a20 2020  gdsfactory...   
-00010170: 2020 2020 204b 6579 776f 7264 2041 7267       Keyword Arg
-00010180: 733a 0a20 2020 2020 2020 2020 2020 2075  s:.            u
-00010190: 6e69 743a 2075 6e69 7420 7369 7a65 2066  nit: unit size f
-000101a0: 6f72 206f 626a 6563 7473 2069 6e20 6c69  or objects in li
-000101b0: 6272 6172 792e 2031 756d 2062 7920 6465  brary. 1um by de
-000101c0: 6661 756c 742e 0a20 2020 2020 2020 2020  fault..         
-000101d0: 2020 2070 7265 6369 7369 6f6e 3a20 666f     precision: fo
-000101e0: 7220 6469 6d65 6e73 696f 6e73 2069 6e20  r dimensions in 
-000101f0: 7468 6520 6c69 6272 6172 7920 286d 292e  the library (m).
-00010200: 2031 6e6d 2062 7920 6465 6661 756c 742e   1nm by default.
-00010210: 0a20 2020 2020 2020 2020 2020 206c 6f67  .            log
-00010220: 6769 6e67 3a20 6469 7361 626c 6520 4744  ging: disable GD
-00010230: 5320 7061 7468 206c 6f67 6769 6e67 2c20  S path logging, 
-00010240: 666f 7220 6578 616d 706c 6520 666f 7220  for example for 
-00010250: 7368 6f77 696e 6720 6974 2069 6e20 4b4c  showing it in KL
-00010260: 6179 6f75 742e 0a20 2020 2020 2020 2020  ayout..         
-00010270: 2020 206f 6e5f 6475 706c 6963 6174 655f     on_duplicate_
-00010280: 6365 6c6c 3a20 7370 6563 6966 7920 686f  cell: specify ho
-00010290: 7720 746f 2072 6573 6f6c 7665 2064 7570  w to resolve dup
-000102a0: 6c69 6361 7465 2d6e 616d 6564 2063 656c  licate-named cel
-000102b0: 6c73 2e20 4368 6f6f 7365 206f 6e65 206f  ls. Choose one o
-000102c0: 6620 7468 6520 666f 6c6c 6f77 696e 673a  f the following:
-000102d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000102e0: 2022 7761 726e 2220 2864 6566 6175 6c74   "warn" (default
-000102f0: 293a 206f 7665 7277 7269 7465 2061 6c6c  ): overwrite all
-00010300: 2064 7570 6c69 6361 7465 2063 656c 6c73   duplicate cells
-00010310: 2077 6974 6820 6f6e 6520 6f66 2074 6865   with one of the
-00010320: 2064 7570 6c69 6361 7465 7320 2861 7262   duplicates (arb
-00010330: 6974 7261 7269 6c79 292e 0a20 2020 2020  itrarily)..     
-00010340: 2020 2020 2020 2020 2020 2022 6572 726f             "erro
-00010350: 7222 3a20 7468 726f 7720 6120 5661 6c75  r": throw a Valu
-00010360: 6545 7272 6f72 2077 6865 6e20 6174 7465  eError when atte
-00010370: 6d70 7469 6e67 2074 6f20 7772 6974 6520  mpting to write 
-00010380: 6120 6764 7320 7769 7468 2064 7570 6c69  a gds with dupli
-00010390: 6361 7465 2063 656c 6c73 2e0a 2020 2020  cate cells..    
-000103a0: 2020 2020 2020 2020 2020 2020 226f 7665              "ove
-000103b0: 7277 7269 7465 223a 206f 7665 7277 7269  rwrite": overwri
-000103c0: 7465 2061 6c6c 2064 7570 6c69 6361 7465  te all duplicate
-000103d0: 2063 656c 6c73 2077 6974 6820 6f6e 6520   cells with one 
-000103e0: 6f66 2074 6865 2064 7570 6c69 6361 7465  of the duplicate
-000103f0: 732c 2077 6974 686f 7574 2077 6172 6e69  s, without warni
-00010400: 6e67 2e0a 2020 2020 2020 2020 2020 2020  ng..            
-00010410: 2020 2020 4e6f 6e65 3a20 646f 206e 6f74      None: do not
-00010420: 2074 7279 2074 6f20 7265 736f 6c76 6520   try to resolve 
-00010430: 2861 7420 796f 7572 206f 776e 2072 6973  (at your own ris
-00010440: 6b21 290a 2020 2020 2020 2020 2020 2020  k!).            
-00010450: 6f6e 5f75 6e63 6163 6865 645f 636f 6d70  on_uncached_comp
-00010460: 6f6e 656e 743a 204c 6974 6572 616c 5b22  onent: Literal["
-00010470: 7761 726e 222c 2022 6572 726f 7222 5d20  warn", "error"] 
-00010480: 3d20 2277 6172 6e22 0a20 2020 2020 2020  = "warn".       
-00010490: 2020 2020 2066 6c61 7474 656e 5f69 6e76       flatten_inv
-000104a0: 616c 6964 5f72 6566 733a 2066 6c61 7474  alid_refs: flatt
-000104b0: 656e 7320 636f 6d70 6f6e 656e 7420 7265  ens component re
-000104c0: 6665 7265 6e63 6573 2077 6869 6368 2068  ferences which h
-000104d0: 6176 6520 696e 7661 6c69 6420 7472 616e  ave invalid tran
-000104e0: 7366 6f72 6d61 7469 6f6e 732e 0a20 2020  sformations..   
-000104f0: 2020 2020 2020 2020 2063 6f6d 7072 6573           compres
-00010500: 7369 6f6e 5f6c 6576 656c 3a20 4c65 7665  sion_level: Leve
-00010510: 6c20 6f66 2063 6f6d 7072 6573 7369 6f6e  l of compression
-00010520: 2066 6f72 2063 656c 6c73 2028 6265 7477   for cells (betw
-00010530: 6565 6e20 3020 616e 6420 3929 2e0a 2020  een 0 and 9)..  
-00010540: 2020 2020 2020 2020 2020 2020 2020 5365                Se
-00010550: 7474 696e 6720 746f 2030 2077 696c 6c20  tting to 0 will 
-00010560: 6469 7361 626c 6520 6365 6c6c 2063 6f6d  disable cell com
-00010570: 7072 6573 7369 6f6e 2c20 3120 6769 7665  pression, 1 give
-00010580: 7320 7468 6520 6265 7374 2073 7065 6564  s the best speed
-00010590: 2061 6e64 2039 2c20 7468 6520 6265 7374   and 9, the best
-000105a0: 2063 6f6d 7072 6573 7369 6f6e 2e0a 2020   compression..  
-000105b0: 2020 2020 2020 2020 2020 6465 7465 6374            detect
-000105c0: 5f72 6563 7461 6e67 6c65 733a 2053 746f  _rectangles: Sto
-000105d0: 7265 2072 6563 7461 6e67 6c65 7320 696e  re rectangles in
-000105e0: 2063 6f6d 7072 6573 7365 6420 666f 726d   compressed form
-000105f0: 6174 2e0a 2020 2020 2020 2020 2020 2020  at..            
-00010600: 6465 7465 6374 5f74 7261 7065 7a6f 6964  detect_trapezoid
-00010610: 733a 2053 746f 7265 2074 7261 7065 7a6f  s: Store trapezo
-00010620: 6964 7320 696e 2063 6f6d 7072 6573 7365  ids in compresse
-00010630: 6420 666f 726d 6174 2e0a 2020 2020 2020  d format..      
-00010640: 2020 2020 2020 6369 7263 6c65 5f74 6f6c        circle_tol
-00010650: 6572 616e 6365 3a20 546f 6c65 7261 6e63  erance: Toleranc
-00010660: 6520 666f 7220 6465 7465 6374 696e 6720  e for detecting 
-00010670: 6369 7263 6c65 732e 2049 6620 6c65 7373  circles. If less
-00010680: 206f 7220 6571 7561 6c20 746f 2030 2c20   or equal to 0, 
-00010690: 6e6f 2064 6574 6563 7469 6f6e 2069 7320  no detection is 
-000106a0: 7065 7266 6f72 6d65 642e 0a20 2020 2020  performed..     
-000106b0: 2020 2020 2020 2020 2020 2043 6972 636c             Circl
-000106c0: 6573 2061 7265 2073 746f 7265 6420 696e  es are stored in
-000106d0: 2063 6f6d 7072 6573 7365 6420 666f 726d   compressed form
-000106e0: 6174 2e0a 2020 2020 2020 2020 2020 2020  at..            
-000106f0: 7661 6c69 6461 7469 6f6e 2028 2263 7263  validation ("crc
-00010700: 3332 222c 2022 6368 6563 6b73 756d 3332  32", "checksum32
-00010710: 222c 204e 6f6e 6529 20e2 8093 2074 7970  ", None) ... typ
-00010720: 6520 6f66 2076 616c 6964 6174 696f 6e20  e of validation 
-00010730: 746f 2069 6e63 6c75 6465 2069 6e20 7468  to include in th
-00010740: 6520 7361 7665 6420 6669 6c65 2e0a 2020  e saved file..  
-00010750: 2020 2020 2020 2020 2020 7374 616e 6461            standa
-00010760: 7264 5f70 726f 7065 7274 6965 733a 2053  rd_properties: S
-00010770: 746f 7265 2073 7461 6e64 6172 6420 4f41  tore standard OA
-00010780: 5349 5320 7072 6f70 6572 7469 6573 2069  SIS properties i
-00010790: 6e20 7468 6520 6669 6c65 2e0a 2020 2020  n the file..    
-000107a0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-000107b0: 7265 7475 726e 2073 656c 662e 5f77 7269  return self._wri
-000107c0: 7465 5f6c 6962 7261 7279 280a 2020 2020  te_library(.    
-000107d0: 2020 2020 2020 2020 6764 7370 6174 683d          gdspath=
-000107e0: 6764 7370 6174 682c 0a20 2020 2020 2020  gdspath,.       
-000107f0: 2020 2020 2067 6473 6469 723d 6764 7364       gdsdir=gdsd
-00010800: 6972 2c0a 2020 2020 2020 2020 2020 2020  ir,.            
-00010810: 7769 7468 5f6f 6173 6973 3d54 7275 652c  with_oasis=True,
-00010820: 0a20 2020 2020 2020 2020 2020 202a 2a6b  .            **k
-00010830: 7761 7267 732c 0a20 2020 2020 2020 2029  wargs,.        )
-00010840: 0a0a 2020 2020 6465 6620 7772 6974 655f  ..    def write_
-00010850: 6764 735f 7769 7468 5f6d 6574 6164 6174  gds_with_metadat
-00010860: 6128 7365 6c66 2c20 2a61 7267 732c 202a  a(self, *args, *
-00010870: 2a6b 7761 7267 7329 202d 3e20 5061 7468  *kwargs) -> Path
-00010880: 3a0a 2020 2020 2020 2020 2222 2257 7269  :.        """Wri
-00010890: 7465 2063 6f6d 706f 6e65 6e74 2069 6e20  te component in 
-000108a0: 4744 5320 616e 6420 6d65 7461 6461 7461  GDS and metadata
-000108b0: 2028 636f 6d70 6f6e 656e 7420 7365 7474   (component sett
-000108c0: 696e 6773 2920 696e 2059 414d 4c2e 2222  ings) in YAML.""
-000108d0: 220a 2020 2020 2020 2020 6764 7370 6174  ".        gdspat
-000108e0: 6820 3d20 7365 6c66 2e77 7269 7465 5f67  h = self.write_g
-000108f0: 6473 282a 6172 6773 2c20 2a2a 6b77 6172  ds(*args, **kwar
-00010900: 6773 290a 2020 2020 2020 2020 6d65 7461  gs).        meta
-00010910: 6461 7461 203d 2067 6473 7061 7468 2e77  data = gdspath.w
-00010920: 6974 685f 7375 6666 6978 2822 2e79 6d6c  ith_suffix(".yml
-00010930: 2229 0a20 2020 2020 2020 206d 6574 6164  ").        metad
-00010940: 6174 612e 7772 6974 655f 7465 7874 2873  ata.write_text(s
-00010950: 656c 662e 746f 5f79 616d 6c28 7769 7468  elf.to_yaml(with
-00010960: 5f63 656c 6c73 3d54 7275 652c 2077 6974  _cells=True, wit
-00010970: 685f 706f 7274 733d 5472 7565 2929 0a20  h_ports=True)). 
-00010980: 2020 2020 2020 206c 6f67 6765 722e 696e         logger.in
-00010990: 666f 2866 2257 7269 7465 2059 414d 4c20  fo(f"Write YAML 
-000109a0: 6d65 7461 6461 7461 2074 6f20 7b73 7472  metadata to {str
-000109b0: 286d 6574 6164 6174 6129 2172 7d22 290a  (metadata)!r}").
-000109c0: 2020 2020 2020 2020 7265 7475 726e 2067          return g
-000109d0: 6473 7061 7468 0a0a 2020 2020 6465 6620  dspath..    def 
-000109e0: 746f 5f64 6963 7428 0a20 2020 2020 2020  to_dict(.       
-000109f0: 2073 656c 662c 0a20 2020 2020 2020 2069   self,.        i
-00010a00: 676e 6f72 655f 636f 6d70 6f6e 656e 7473  gnore_components
-00010a10: 5f70 7265 6669 783a 204f 7074 696f 6e61  _prefix: Optiona
-00010a20: 6c5b 4c69 7374 5b73 7472 5d5d 203d 204e  l[List[str]] = N
-00010a30: 6f6e 652c 0a20 2020 2020 2020 2069 676e  one,.        ign
-00010a40: 6f72 655f 6675 6e63 7469 6f6e 735f 7072  ore_functions_pr
-00010a50: 6566 6978 3a20 4f70 7469 6f6e 616c 5b4c  efix: Optional[L
-00010a60: 6973 745b 7374 725d 5d20 3d20 4e6f 6e65  ist[str]] = None
-00010a70: 2c0a 2020 2020 2020 2020 7769 7468 5f63  ,.        with_c
-00010a80: 656c 6c73 3a20 626f 6f6c 203d 2046 616c  ells: bool = Fal
-00010a90: 7365 2c0a 2020 2020 2020 2020 7769 7468  se,.        with
-00010aa0: 5f70 6f72 7473 3a20 626f 6f6c 203d 2054  _ports: bool = T
-00010ab0: 7275 652c 0a20 2020 2029 202d 3e20 4469  rue,.    ) -> Di
-00010ac0: 6374 5b73 7472 2c20 416e 795d 3a0a 2020  ct[str, Any]:.  
-00010ad0: 2020 2020 2020 2222 2252 6574 7572 6e73        """Returns
-00010ae0: 2044 6963 7420 7265 7072 6573 656e 7461   Dict representa
-00010af0: 7469 6f6e 206f 6620 6120 636f 6d70 6f6e  tion of a compon
-00010b00: 656e 742e 0a0a 2020 2020 2020 2020 4172  ent...        Ar
-00010b10: 6773 3a0a 2020 2020 2020 2020 2020 2020  gs:.            
-00010b20: 6967 6e6f 7265 5f63 6f6d 706f 6e65 6e74  ignore_component
-00010b30: 735f 7072 6566 6978 3a20 666f 7220 636f  s_prefix: for co
-00010b40: 6d70 6f6e 656e 7473 2074 6f20 6967 6e6f  mponents to igno
-00010b50: 7265 2077 6865 6e20 6578 706f 7274 696e  re when exportin
-00010b60: 672e 0a20 2020 2020 2020 2020 2020 2069  g..            i
-00010b70: 676e 6f72 655f 6675 6e63 7469 6f6e 735f  gnore_functions_
-00010b80: 7072 6566 6978 3a20 666f 7220 6675 6e63  prefix: for func
-00010b90: 7469 6f6e 7320 746f 2069 676e 6f72 6520  tions to ignore 
-00010ba0: 7768 656e 2065 7870 6f72 7469 6e67 2e0a  when exporting..
-00010bb0: 2020 2020 2020 2020 2020 2020 7769 7468              with
-00010bc0: 5f63 656c 6c73 3a20 7772 6974 6520 6365  _cells: write ce
-00010bd0: 6c6c 7320 7265 6375 7273 6976 656c 792e  lls recursively.
-00010be0: 0a20 2020 2020 2020 2020 2020 2077 6974  .            wit
-00010bf0: 685f 706f 7274 733a 2077 7269 7465 2070  h_ports: write p
-00010c00: 6f72 7420 696e 666f 726d 6174 696f 6e20  ort information 
-00010c10: 6469 6374 2e0a 2020 2020 2020 2020 2222  dict..        ""
-00010c20: 220a 2020 2020 2020 2020 6420 3d20 7b7d  ".        d = {}
-00010c30: 0a20 2020 2020 2020 2069 6620 7769 7468  .        if with
-00010c40: 5f70 6f72 7473 3a0a 2020 2020 2020 2020  _ports:.        
-00010c50: 2020 2020 706f 7274 7320 3d20 7b70 6f72      ports = {por
-00010c60: 742e 6e61 6d65 3a20 706f 7274 2e74 6f5f  t.name: port.to_
-00010c70: 6469 6374 2829 2066 6f72 2070 6f72 7420  dict() for port 
-00010c80: 696e 2073 656c 662e 6765 745f 706f 7274  in self.get_port
-00010c90: 735f 6c69 7374 2829 7d0a 2020 2020 2020  s_list()}.      
-00010ca0: 2020 2020 2020 645b 2270 6f72 7473 225d        d["ports"]
-00010cb0: 203d 2070 6f72 7473 0a0a 2020 2020 2020   = ports..      
-00010cc0: 2020 6966 2077 6974 685f 6365 6c6c 733a    if with_cells:
-00010cd0: 0a20 2020 2020 2020 2020 2020 2063 656c  .            cel
-00010ce0: 6c73 203d 2072 6563 7572 7365 5f73 7472  ls = recurse_str
-00010cf0: 7563 7475 7265 7328 0a20 2020 2020 2020  uctures(.       
-00010d00: 2020 2020 2020 2020 2073 656c 662c 0a20           self,. 
-00010d10: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00010d20: 676e 6f72 655f 6675 6e63 7469 6f6e 735f  gnore_functions_
-00010d30: 7072 6566 6978 3d69 676e 6f72 655f 6675  prefix=ignore_fu
-00010d40: 6e63 7469 6f6e 735f 7072 6566 6978 2c0a  nctions_prefix,.
-00010d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010d60: 6967 6e6f 7265 5f63 6f6d 706f 6e65 6e74  ignore_component
-00010d70: 735f 7072 6566 6978 3d69 676e 6f72 655f  s_prefix=ignore_
-00010d80: 636f 6d70 6f6e 656e 7473 5f70 7265 6669  components_prefi
-00010d90: 782c 0a20 2020 2020 2020 2020 2020 2029  x,.            )
-00010da0: 0a20 2020 2020 2020 2020 2020 2064 5b22  .            d["
-00010db0: 6365 6c6c 7322 5d20 3d20 636c 6561 6e5f  cells"] = clean_
-00010dc0: 6469 6374 2863 656c 6c73 290a 0a20 2020  dict(cells)..   
-00010dd0: 2020 2020 2064 5b22 6e61 6d65 225d 203d       d["name"] =
-00010de0: 2073 656c 662e 6e61 6d65 0a20 2020 2020   self.name.     
-00010df0: 2020 2064 5b22 7365 7474 696e 6773 225d     d["settings"]
-00010e00: 203d 2063 6c65 616e 5f64 6963 7428 6469   = clean_dict(di
-00010e10: 6374 2873 656c 662e 7365 7474 696e 6773  ct(self.settings
-00010e20: 2929 0a20 2020 2020 2020 2072 6574 7572  )).        retur
-00010e30: 6e20 640a 0a20 2020 2064 6566 2074 6f5f  n d..    def to_
-00010e40: 7961 6d6c 2873 656c 662c 202a 2a6b 7761  yaml(self, **kwa
-00010e50: 7267 7329 202d 3e20 7374 723a 0a20 2020  rgs) -> str:.   
-00010e60: 2020 2020 2022 2222 5772 6974 6520 4469       """Write Di
-00010e70: 6374 2072 6570 7265 7365 6e74 6174 696f  ct representatio
-00010e80: 6e20 6f66 2061 2063 6f6d 706f 6e65 6e74  n of a component
-00010e90: 2069 6e20 5941 4d4c 2066 6f72 6d61 742e   in YAML format.
-00010ea0: 0a0a 2020 2020 2020 2020 4172 6773 3a0a  ..        Args:.
-00010eb0: 2020 2020 2020 2020 2020 2020 6967 6e6f              igno
-00010ec0: 7265 5f63 6f6d 706f 6e65 6e74 735f 7072  re_components_pr
-00010ed0: 6566 6978 3a20 666f 7220 636f 6d70 6f6e  efix: for compon
-00010ee0: 656e 7473 2074 6f20 6967 6e6f 7265 2077  ents to ignore w
-00010ef0: 6865 6e20 6578 706f 7274 696e 672e 0a20  hen exporting.. 
-00010f00: 2020 2020 2020 2020 2020 2069 676e 6f72             ignor
-00010f10: 655f 6675 6e63 7469 6f6e 735f 7072 6566  e_functions_pref
-00010f20: 6978 3a20 666f 7220 6675 6e63 7469 6f6e  ix: for function
-00010f30: 7320 746f 2069 676e 6f72 6520 7768 656e  s to ignore when
-00010f40: 2065 7870 6f72 7469 6e67 2e0a 2020 2020   exporting..    
-00010f50: 2020 2020 2020 2020 7769 7468 5f63 656c          with_cel
-00010f60: 6c73 3a20 7772 6974 6520 6365 6c6c 7320  ls: write cells 
-00010f70: 7265 6375 7273 6976 656c 792e 0a20 2020  recursively..   
-00010f80: 2020 2020 2020 2020 2077 6974 685f 706f           with_po
-00010f90: 7274 733a 2077 7269 7465 2070 6f72 7420  rts: write port 
-00010fa0: 696e 666f 726d 6174 696f 6e2e 0a20 2020  information..   
-00010fb0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00010fc0: 2072 6574 7572 6e20 4f6d 6567 6143 6f6e   return OmegaCon
-00010fd0: 662e 746f 5f79 616d 6c28 636c 6561 6e5f  f.to_yaml(clean_
-00010fe0: 6469 6374 2873 656c 662e 746f 5f64 6963  dict(self.to_dic
-00010ff0: 7428 2a2a 6b77 6172 6773 2929 290a 0a20  t(**kwargs))).. 
-00011000: 2020 2064 6566 2074 6f5f 6469 6374 5f70     def to_dict_p
-00011010: 6f6c 7967 6f6e 7328 7365 6c66 2920 2d3e  olygons(self) ->
-00011020: 2044 6963 745b 7374 722c 2041 6e79 5d3a   Dict[str, Any]:
-00011030: 0a20 2020 2020 2020 2022 2222 5265 7475  .        """Retu
-00011040: 726e 7320 6120 6469 6374 2072 6570 7265  rns a dict repre
-00011050: 7365 6e74 6174 696f 6e20 6f66 2074 6865  sentation of the
-00011060: 2066 6c61 7474 656e 6564 2063 6f6d 706f   flattened compo
-00011070: 6e65 6e74 2e22 2222 0a20 2020 2020 2020  nent.""".       
-00011080: 2064 203d 207b 7d0a 2020 2020 2020 2020   d = {}.        
-00011090: 706f 6c79 676f 6e73 203d 207b 7d0a 2020  polygons = {}.  
-000110a0: 2020 2020 2020 6c61 7965 725f 746f 5f70        layer_to_p
-000110b0: 6f6c 7967 6f6e 7320 3d20 7365 6c66 2e67  olygons = self.g
-000110c0: 6574 5f70 6f6c 7967 6f6e 7328 6279 5f73  et_polygons(by_s
-000110d0: 7065 633d 5472 7565 290a 0a20 2020 2020  pec=True)..     
-000110e0: 2020 2066 6f72 206c 6179 6572 2c20 706f     for layer, po
-000110f0: 6c79 676f 6e73 5f6c 6179 6572 2069 6e20  lygons_layer in 
-00011100: 6c61 7965 725f 746f 5f70 6f6c 7967 6f6e  layer_to_polygon
-00011110: 732e 6974 656d 7328 293a 0a20 2020 2020  s.items():.     
-00011120: 2020 2020 2020 206c 6179 6572 5f6e 616d         layer_nam
-00011130: 6520 3d20 6622 7b6c 6179 6572 5b30 5d7d  e = f"{layer[0]}
-00011140: 5f7b 6c61 7965 725b 315d 7d22 0a20 2020  _{layer[1]}".   
-00011150: 2020 2020 2020 2020 2066 6f72 2070 6f6c           for pol
-00011160: 7967 6f6e 2069 6e20 706f 6c79 676f 6e73  ygon in polygons
-00011170: 5f6c 6179 6572 3a0a 2020 2020 2020 2020  _layer:.        
-00011180: 2020 2020 2020 2020 706f 6c79 676f 6e73          polygons
-00011190: 5b6c 6179 6572 5f6e 616d 655d 203d 205b  [layer_name] = [
-000111a0: 7475 706c 6528 736e 6170 5f74 6f5f 6772  tuple(snap_to_gr
-000111b0: 6964 2876 2929 2066 6f72 2076 2069 6e20  id(v)) for v in 
-000111c0: 706f 6c79 676f 6e5d 0a0a 2020 2020 2020  polygon]..      
-000111d0: 2020 706f 7274 7320 3d20 7b70 6f72 742e    ports = {port.
-000111e0: 6e61 6d65 3a20 706f 7274 2e73 6574 7469  name: port.setti
-000111f0: 6e67 7320 666f 7220 706f 7274 2069 6e20  ngs for port in 
-00011200: 7365 6c66 2e67 6574 5f70 6f72 7473 5f6c  self.get_ports_l
-00011210: 6973 7428 297d 0a20 2020 2020 2020 2063  ist()}.        c
-00011220: 6c65 616e 5f64 6963 7428 706f 7274 7329  lean_dict(ports)
-00011230: 0a20 2020 2020 2020 2063 6c65 616e 5f64  .        clean_d
-00011240: 6963 7428 706f 6c79 676f 6e73 290a 2020  ict(polygons).  
-00011250: 2020 2020 2020 642e 696e 666f 203d 2073        d.info = s
-00011260: 656c 662e 696e 666f 0a20 2020 2020 2020  elf.info.       
-00011270: 2064 2e70 6f6c 7967 6f6e 7320 3d20 706f   d.polygons = po
-00011280: 6c79 676f 6e73 0a20 2020 2020 2020 2064  lygons.        d
-00011290: 2e70 6f72 7473 203d 2070 6f72 7473 0a20  .ports = ports. 
-000112a0: 2020 2020 2020 2072 6574 7572 6e20 640a         return d.
-000112b0: 0a20 2020 2064 6566 2061 7574 6f5f 7265  .    def auto_re
-000112c0: 6e61 6d65 5f70 6f72 7473 2873 656c 662c  name_ports(self,
-000112d0: 202a 2a6b 7761 7267 7329 202d 3e20 4e6f   **kwargs) -> No
-000112e0: 6e65 3a0a 2020 2020 2020 2020 2222 2252  ne:.        """R
-000112f0: 656e 616d 6520 706f 7274 7320 6279 206f  ename ports by o
-00011300: 7269 656e 7461 7469 6f6e 204e 5345 5720  rientation NSEW 
-00011310: 286e 6f72 7468 2c20 736f 7574 682c 2065  (north, south, e
-00011320: 6173 742c 2077 6573 7429 2e0a 0a20 2020  ast, west)...   
-00011330: 2020 2020 204b 6579 776f 7264 2041 7267       Keyword Arg
-00011340: 733a 0a20 2020 2020 2020 2020 2020 2066  s:.            f
-00011350: 756e 6374 696f 6e3a 2074 6f20 7265 6e61  unction: to rena
-00011360: 6d65 2070 6f72 7473 2e0a 2020 2020 2020  me ports..      
-00011370: 2020 2020 2020 7365 6c65 6374 5f70 6f72        select_por
-00011380: 7473 5f6f 7074 6963 616c 3a20 746f 2073  ts_optical: to s
-00011390: 656c 6563 7420 6f70 7469 6361 6c20 706f  elect optical po
-000113a0: 7274 732e 0a20 2020 2020 2020 2020 2020  rts..           
-000113b0: 2073 656c 6563 745f 706f 7274 735f 656c   select_ports_el
-000113c0: 6563 7472 6963 616c 3a20 746f 2073 656c  ectrical: to sel
-000113d0: 6563 7420 656c 6563 7472 6963 616c 2070  ect electrical p
-000113e0: 6f72 7473 2e0a 2020 2020 2020 2020 2020  orts..          
-000113f0: 2020 7072 6566 6978 5f6f 7074 6963 616c    prefix_optical
-00011400: 3a20 7072 6566 6978 2e0a 2020 2020 2020  : prefix..      
-00011410: 2020 2020 2020 7072 6566 6978 5f65 6c65        prefix_ele
-00011420: 6374 7269 6361 6c3a 2070 7265 6669 782e  ctrical: prefix.
-00011430: 0a0a 2020 2020 2020 2020 2e2e 2063 6f64  ..        .. cod
-00011440: 653a 3a0a 0a20 2020 2020 2020 2020 2020  e::..           
-00011450: 2020 2020 2020 2033 2020 340a 2020 2020         3  4.    
-00011460: 2020 2020 2020 2020 2020 2020 205f 7c5f               _|_
-00011470: 5f7c 5f0a 2020 2020 2020 2020 2020 2020  _|_.            
-00011480: 2032 202d 7c20 2020 2020 207c 2d20 350a   2 -|      |- 5.
-00011490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000114a0: 7c20 2020 2020 207c 0a20 2020 2020 2020  |      |.       
-000114b0: 2020 2020 2020 3120 2d7c 5f5f 5f5f 5f5f        1 -|______
-000114c0: 7c2d 2036 0a20 2020 2020 2020 2020 2020  |- 6.           
-000114d0: 2020 2020 2020 207c 2020 7c0a 2020 2020         |  |.    
-000114e0: 2020 2020 2020 2020 2020 2020 2020 3820                8 
-000114f0: 2037 0a20 2020 2020 2020 2022 2222 0a20   7.        """. 
-00011500: 2020 2020 2020 2073 656c 662e 6973 5f75         self.is_u
-00011510: 6e6c 6f63 6b65 6428 290a 2020 2020 2020  nlocked().      
-00011520: 2020 6175 746f 5f72 656e 616d 655f 706f    auto_rename_po
-00011530: 7274 7328 7365 6c66 2c20 2a2a 6b77 6172  rts(self, **kwar
-00011540: 6773 290a 0a20 2020 2064 6566 2061 7574  gs)..    def aut
-00011550: 6f5f 7265 6e61 6d65 5f70 6f72 7473 5f63  o_rename_ports_c
-00011560: 6f75 6e74 6572 5f63 6c6f 636b 7769 7365  ounter_clockwise
-00011570: 2873 656c 662c 202a 2a6b 7761 7267 7329  (self, **kwargs)
-00011580: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
-00011590: 2020 7365 6c66 2e69 735f 756e 6c6f 636b    self.is_unlock
-000115a0: 6564 2829 0a20 2020 2020 2020 2061 7574  ed().        aut
-000115b0: 6f5f 7265 6e61 6d65 5f70 6f72 7473 5f63  o_rename_ports_c
-000115c0: 6f75 6e74 6572 5f63 6c6f 636b 7769 7365  ounter_clockwise
-000115d0: 2873 656c 662c 202a 2a6b 7761 7267 7329  (self, **kwargs)
-000115e0: 0a0a 2020 2020 6465 6620 6175 746f 5f72  ..    def auto_r
-000115f0: 656e 616d 655f 706f 7274 735f 6c61 7965  ename_ports_laye
-00011600: 725f 6f72 6965 6e74 6174 696f 6e28 7365  r_orientation(se
-00011610: 6c66 2c20 2a2a 6b77 6172 6773 2920 2d3e  lf, **kwargs) ->
-00011620: 204e 6f6e 653a 0a20 2020 2020 2020 2073   None:.        s
-00011630: 656c 662e 6973 5f75 6e6c 6f63 6b65 6428  elf.is_unlocked(
-00011640: 290a 2020 2020 2020 2020 6175 746f 5f72  ).        auto_r
-00011650: 656e 616d 655f 706f 7274 735f 6c61 7965  ename_ports_laye
-00011660: 725f 6f72 6965 6e74 6174 696f 6e28 7365  r_orientation(se
-00011670: 6c66 2c20 2a2a 6b77 6172 6773 290a 0a20  lf, **kwargs).. 
-00011680: 2020 2064 6566 2061 7574 6f5f 7265 6e61     def auto_rena
-00011690: 6d65 5f70 6f72 7473 5f6f 7269 656e 7461  me_ports_orienta
-000116a0: 7469 6f6e 2873 656c 662c 202a 2a6b 7761  tion(self, **kwa
-000116b0: 7267 7329 202d 3e20 4e6f 6e65 3a0a 2020  rgs) -> None:.  
-000116c0: 2020 2020 2020 2222 2252 656e 616d 6520        """Rename 
-000116d0: 706f 7274 7320 6279 206f 7269 656e 7461  ports by orienta
-000116e0: 7469 6f6e 204e 5345 5720 286e 6f72 7468  tion NSEW (north
-000116f0: 2c20 736f 7574 682c 2065 6173 742c 2077  , south, east, w
-00011700: 6573 7429 2e0a 0a20 2020 2020 2020 204b  est)...        K
-00011710: 6579 776f 7264 2041 7267 733a 0a20 2020  eyword Args:.   
-00011720: 2020 2020 2020 2020 2066 756e 6374 696f           functio
-00011730: 6e3a 2074 6f20 7265 6e61 6d65 2070 6f72  n: to rename por
-00011740: 7473 2e0a 2020 2020 2020 2020 2020 2020  ts..            
-00011750: 7365 6c65 6374 5f70 6f72 7473 5f6f 7074  select_ports_opt
-00011760: 6963 616c 3a20 746f 2073 656c 6563 7420  ical: to select 
-00011770: 706f 7274 732e 0a20 2020 2020 2020 2020  ports..         
-00011780: 2020 2073 656c 6563 745f 706f 7274 735f     select_ports_
-00011790: 656c 6563 7472 6963 616c 3a0a 2020 2020  electrical:.    
-000117a0: 2020 2020 2020 2020 7072 6566 6978 5f6f          prefix_o
-000117b0: 7074 6963 616c 3a0a 2020 2020 2020 2020  ptical:.        
-000117c0: 2020 2020 7072 6566 6978 5f65 6c65 6374      prefix_elect
-000117d0: 7269 6361 6c3a 0a0a 2020 2020 2020 2020  rical:..        
-000117e0: 2e2e 2063 6f64 653a 3a0a 0a20 2020 2020  .. code::..     
-000117f0: 2020 2020 2020 2020 2020 2020 4e30 2020              N0  
-00011800: 4e31 0a20 2020 2020 2020 2020 2020 2020  N1.             
-00011810: 2020 2020 7c5f 5f5f 7c5f 0a20 2020 2020      |___|_.     
-00011820: 2020 2020 2020 2057 3120 2d7c 2020 2020         W1 -|    
-00011830: 2020 7c2d 2045 310a 2020 2020 2020 2020    |- E1.        
-00011840: 2020 2020 2020 2020 7c20 2020 2020 207c          |      |
-00011850: 0a20 2020 2020 2020 2020 2020 2057 3020  .            W0 
-00011860: 2d7c 5f5f 5f5f 5f5f 7c2d 2045 300a 2020  -|______|- E0.  
-00011870: 2020 2020 2020 2020 2020 2020 2020 207c                 |
-00011880: 2020 207c 0a20 2020 2020 2020 2020 2020     |.           
-00011890: 2020 2020 2053 3020 2020 5331 0a20 2020       S0   S1.   
-000118a0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-000118b0: 2073 656c 662e 6973 5f75 6e6c 6f63 6b65   self.is_unlocke
-000118c0: 6428 290a 2020 2020 2020 2020 6175 746f  d().        auto
-000118d0: 5f72 656e 616d 655f 706f 7274 735f 6f72  _rename_ports_or
-000118e0: 6965 6e74 6174 696f 6e28 7365 6c66 2c20  ientation(self, 
-000118f0: 2a2a 6b77 6172 6773 290a 0a20 2020 2064  **kwargs)..    d
-00011900: 6566 206d 6f76 6528 0a20 2020 2020 2020  ef move(.       
-00011910: 2073 656c 662c 0a20 2020 2020 2020 206f   self,.        o
-00011920: 7269 6769 6e3a 2046 6c6f 6174 3220 3d20  rigin: Float2 = 
-00011930: 2830 2c20 3029 2c0a 2020 2020 2020 2020  (0, 0),.        
-00011940: 6465 7374 696e 6174 696f 6e3a 204f 7074  destination: Opt
-00011950: 696f 6e61 6c5b 466c 6f61 7432 5d20 3d20  ional[Float2] = 
-00011960: 4e6f 6e65 2c0a 2020 2020 2020 2020 6178  None,.        ax
-00011970: 6973 3a20 4f70 7469 6f6e 616c 5b41 7869  is: Optional[Axi
-00011980: 735d 203d 204e 6f6e 652c 0a20 2020 2029  s] = None,.    )
-00011990: 202d 3e20 436f 6d70 6f6e 656e 743a 0a20   -> Component:. 
-000119a0: 2020 2020 2020 2022 2222 5265 7475 726e         """Return
-000119b0: 7320 6e65 7720 436f 6d70 6f6e 656e 7420  s new Component 
-000119c0: 7769 7468 2061 206d 6f76 6564 2072 6566  with a moved ref
-000119d0: 6572 656e 6365 2074 6f20 7468 6520 6f72  erence to the or
-000119e0: 6967 696e 616c 2e0a 0a20 2020 2020 2020  iginal...       
-000119f0: 2063 6f6d 706f 6e65 6e74 2e0a 0a20 2020   component...   
-00011a00: 2020 2020 2041 7267 733a 0a20 2020 2020       Args:.     
-00011a10: 2020 2020 2020 206f 7269 6769 6e3a 206f         origin: o
-00011a20: 6620 636f 6d70 6f6e 656e 742e 0a20 2020  f component..   
-00011a30: 2020 2020 2020 2020 2064 6573 7469 6e61           destina
-00011a40: 7469 6f6e 3a20 782c 2079 2e0a 2020 2020  tion: x, y..    
-00011a50: 2020 2020 2020 2020 6178 6973 3a20 7820          axis: x 
-00011a60: 6f72 2079 2e0a 2020 2020 2020 2020 2222  or y..        ""
-00011a70: 220a 2020 2020 2020 2020 7261 6973 6520  ".        raise 
-00011a80: 5661 6c75 6545 7272 6f72 286d 6f76 655f  ValueError(move_
-00011a90: 6572 726f 725f 6d65 7373 6167 6529 0a0a  error_message)..
-00011aa0: 2020 2020 6465 6620 6d69 7272 6f72 2873      def mirror(s
-00011ab0: 656c 662c 2070 313a 2046 6c6f 6174 3220  elf, p1: Float2 
-00011ac0: 3d20 2830 2c20 3129 2c20 7032 3a20 466c  = (0, 1), p2: Fl
-00011ad0: 6f61 7432 203d 2028 302c 2030 292c 202a  oat2 = (0, 0), *
-00011ae0: 2a6b 7761 7267 7329 202d 3e20 436f 6d70  *kwargs) -> Comp
-00011af0: 6f6e 656e 743a 0a20 2020 2020 2020 2022  onent:.        "
-00011b00: 2222 5265 7475 726e 7320 6e65 7720 436f  ""Returns new Co
-00011b10: 6d70 6f6e 656e 7420 7769 7468 2061 206d  mponent with a m
-00011b20: 6972 726f 7265 6420 7265 6665 7265 6e63  irrored referenc
-00011b30: 652e 0a0a 2020 2020 2020 2020 4172 6773  e...        Args
-00011b40: 3a0a 2020 2020 2020 2020 2020 2020 7031  :.            p1
-00011b50: 3a20 6669 7273 7420 706f 696e 7420 746f  : first point to
-00011b60: 2064 6566 696e 6520 6d69 7272 6f72 2061   define mirror a
-00011b70: 7869 732e 0a20 2020 2020 2020 2020 2020  xis..           
-00011b80: 2070 323a 2073 6563 6f6e 6420 706f 696e   p2: second poin
-00011b90: 7420 746f 2064 6566 696e 6520 6d69 7272  t to define mirr
-00011ba0: 6f72 2061 7869 732e 0a20 2020 2020 2020  or axis..       
-00011bb0: 2022 2222 0a20 2020 2020 2020 2066 726f   """.        fro
-00011bc0: 6d20 6764 7366 6163 746f 7279 2e66 756e  m gdsfactory.fun
-00011bd0: 6374 696f 6e73 2069 6d70 6f72 7420 6d69  ctions import mi
-00011be0: 7272 6f72 0a0a 2020 2020 2020 2020 7265  rror..        re
-00011bf0: 7475 726e 206d 6972 726f 7228 636f 6d70  turn mirror(comp
-00011c00: 6f6e 656e 743d 7365 6c66 2c20 7031 3d70  onent=self, p1=p
-00011c10: 312c 2070 323d 7032 2c20 2a2a 6b77 6172  1, p2=p2, **kwar
-00011c20: 6773 290a 0a20 2020 2064 6566 2072 6f74  gs)..    def rot
-00011c30: 6174 6528 7365 6c66 2c20 616e 676c 653a  ate(self, angle:
-00011c40: 2066 6c6f 6174 203d 2039 302c 202a 2a6b   float = 90, **k
-00011c50: 7761 7267 7329 202d 3e20 436f 6d70 6f6e  wargs) -> Compon
-00011c60: 656e 743a 0a20 2020 2020 2020 2022 2222  ent:.        """
-00011c70: 5265 7475 726e 7320 6e65 7720 636f 6d70  Returns new comp
-00011c80: 6f6e 656e 7420 7769 7468 2061 2072 6f74  onent with a rot
-00011c90: 6174 6564 2072 6566 6572 656e 6365 2074  ated reference t
-00011ca0: 6f20 7468 6520 6f72 6967 696e 616c 2e0a  o the original..
-00011cb0: 0a20 2020 2020 2020 2041 7267 733a 0a20  .        Args:. 
-00011cc0: 2020 2020 2020 2020 2020 2061 6e67 6c65             angle
-00011cd0: 3a20 696e 2064 6567 7265 6573 2e0a 2020  : in degrees..  
-00011ce0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-00011cf0: 2020 6672 6f6d 2067 6473 6661 6374 6f72    from gdsfactor
-00011d00: 792e 6675 6e63 7469 6f6e 7320 696d 706f  y.functions impo
-00011d10: 7274 2072 6f74 6174 650a 0a20 2020 2020  rt rotate..     
-00011d20: 2020 2072 6574 7572 6e20 726f 7461 7465     return rotate
-00011d30: 2863 6f6d 706f 6e65 6e74 3d73 656c 662c  (component=self,
-00011d40: 2061 6e67 6c65 3d61 6e67 6c65 2c20 2a2a   angle=angle, **
-00011d50: 6b77 6172 6773 290a 0a20 2020 2064 6566  kwargs)..    def
-00011d60: 2061 6464 5f70 6164 6469 6e67 2873 656c   add_padding(sel
-00011d70: 662c 202a 2a6b 7761 7267 7329 202d 3e20  f, **kwargs) -> 
-00011d80: 436f 6d70 6f6e 656e 743a 0a20 2020 2020  Component:.     
-00011d90: 2020 2022 2222 5265 7475 726e 7320 7361     """Returns sa
-00011da0: 6d65 2063 6f6d 706f 6e65 6e74 2077 6974  me component wit
-00011db0: 6820 7061 6464 696e 672e 0a0a 2020 2020  h padding...    
-00011dc0: 2020 2020 4b65 7977 6f72 6420 4172 6773      Keyword Args
-00011dd0: 3a0a 2020 2020 2020 2020 2020 2020 636f  :.            co
-00011de0: 6d70 6f6e 656e 743a 2066 6f72 2070 6164  mponent: for pad
-00011df0: 6469 6e67 2e0a 2020 2020 2020 2020 2020  ding..          
-00011e00: 2020 6c61 7965 7273 3a20 6c69 7374 206f    layers: list o
-00011e10: 6620 6c61 7965 7273 2e0a 2020 2020 2020  f layers..      
-00011e20: 2020 2020 2020 7375 6666 6978 2066 6f72        suffix for
-00011e30: 206e 616d 652e 0a20 2020 2020 2020 2020   name..         
-00011e40: 2020 2064 6566 6175 6c74 3a20 6465 6661     default: defa
-00011e50: 756c 7420 7061 6464 696e 6720 2835 3075  ult padding (50u
-00011e60: 6d29 2e0a 2020 2020 2020 2020 2020 2020  m)..            
-00011e70: 746f 703a 206e 6f72 7468 2070 6164 6469  top: north paddi
-00011e80: 6e67 2e0a 2020 2020 2020 2020 2020 2020  ng..            
-00011e90: 626f 7474 6f6d 3a20 736f 7574 6820 7061  bottom: south pa
-00011ea0: 6464 696e 672e 0a20 2020 2020 2020 2020  dding..         
-00011eb0: 2020 2072 6967 6874 3a20 6561 7374 2070     right: east p
-00011ec0: 6164 6469 6e67 2e0a 2020 2020 2020 2020  adding..        
-00011ed0: 2020 2020 6c65 6674 3a20 7765 7374 2070      left: west p
-00011ee0: 6164 6469 6e67 2e0a 2020 2020 2020 2020  adding..        
-00011ef0: 2222 220a 2020 2020 2020 2020 6672 6f6d  """.        from
-00011f00: 2067 6473 6661 6374 6f72 792e 6164 645f   gdsfactory.add_
-00011f10: 7061 6464 696e 6720 696d 706f 7274 2061  padding import a
-00011f20: 6464 5f70 6164 6469 6e67 0a0a 2020 2020  dd_padding..    
-00011f30: 2020 2020 7265 7475 726e 2061 6464 5f70      return add_p
-00011f40: 6164 6469 6e67 2863 6f6d 706f 6e65 6e74  adding(component
-00011f50: 3d73 656c 662c 202a 2a6b 7761 7267 7329  =self, **kwargs)
-00011f60: 0a0a 2020 2020 6465 6620 6162 736f 7262  ..    def absorb
-00011f70: 2873 656c 662c 2072 6566 6572 656e 6365  (self, reference
-00011f80: 2920 2d3e 2043 6f6d 706f 6e65 6e74 3a0a  ) -> Component:.
-00011f90: 2020 2020 2020 2020 2222 2241 6273 6f72          """Absor
-00011fa0: 6273 2070 6f6c 7967 6f6e 7320 6672 6f6d  bs polygons from
-00011fb0: 2043 6f6d 706f 6e65 6e74 5265 6665 7265   ComponentRefere
-00011fc0: 6e63 6520 696e 746f 2043 6f6d 706f 6e65  nce into Compone
-00011fd0: 6e74 2e0a 0a20 2020 2020 2020 2044 6573  nt...        Des
-00011fe0: 7472 6f79 7320 7468 6520 7265 6665 7265  troys the refere
-00011ff0: 6e63 6520 696e 2074 6865 2070 726f 6365  nce in the proce
-00012000: 7373 2062 7574 206b 6565 7069 6e67 2074  ss but keeping t
-00012010: 6865 2070 6f6c 7967 6f6e 2067 656f 6d65  he polygon geome
-00012020: 7472 792e 0a0a 2020 2020 2020 2020 4172  try...        Ar
-00012030: 6773 3a0a 2020 2020 2020 2020 2020 2020  gs:.            
-00012040: 7265 6665 7265 6e63 653a 2043 6f6d 706f  reference: Compo
-00012050: 6e65 6e74 5265 6665 7265 6e63 6520 746f  nentReference to
-00012060: 2062 6520 6162 736f 7262 6564 2069 6e74   be absorbed int
-00012070: 6f20 7468 6520 436f 6d70 6f6e 656e 742e  o the Component.
-00012080: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00012090: 2020 2020 2069 6620 7265 6665 7265 6e63       if referenc
-000120a0: 6520 6e6f 7420 696e 2073 656c 662e 7265  e not in self.re
-000120b0: 6665 7265 6e63 6573 3a0a 2020 2020 2020  ferences:.      
-000120c0: 2020 2020 2020 7261 6973 6520 5661 6c75        raise Valu
-000120d0: 6545 7272 6f72 280a 2020 2020 2020 2020  eError(.        
-000120e0: 2020 2020 2020 2020 2254 6865 2072 6566          "The ref
-000120f0: 6572 656e 6365 2079 6f75 2061 736b 6564  erence you asked
-00012100: 2074 6f20 6162 736f 7262 2064 6f65 7320   to absorb does 
-00012110: 6e6f 7420 6578 6973 7420 696e 2074 6869  not exist in thi
-00012120: 7320 436f 6d70 6f6e 656e 742e 220a 2020  s Component.".  
-00012130: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-00012140: 2020 2020 7265 665f 706f 6c79 676f 6e73      ref_polygons
-00012150: 203d 2072 6566 6572 656e 6365 2e67 6574   = reference.get
-00012160: 5f70 6f6c 7967 6f6e 7328 0a20 2020 2020  _polygons(.     
-00012170: 2020 2020 2020 2062 795f 7370 6563 3d46         by_spec=F
-00012180: 616c 7365 2c20 696e 636c 7564 655f 7061  alse, include_pa
-00012190: 7468 733d 4661 6c73 652c 2061 735f 6172  ths=False, as_ar
-000121a0: 7261 793d 4661 6c73 650a 2020 2020 2020  ray=False.      
-000121b0: 2020 290a 2020 2020 2020 2020 7365 6c66    ).        self
-000121c0: 2e5f 6164 645f 706f 6c79 676f 6e73 282a  ._add_polygons(*
-000121d0: 7265 665f 706f 6c79 676f 6e73 290a 0a20  ref_polygons).. 
-000121e0: 2020 2020 2020 2073 656c 662e 6164 6428         self.add(
-000121f0: 7265 6665 7265 6e63 652e 6765 745f 6c61  reference.get_la
-00012200: 6265 6c73 2829 290a 2020 2020 2020 2020  bels()).        
-00012210: 7365 6c66 2e61 6464 2872 6566 6572 656e  self.add(referen
-00012220: 6365 2e67 6574 5f70 6174 6873 2829 290a  ce.get_paths()).
-00012230: 2020 2020 2020 2020 7365 6c66 2e72 656d          self.rem
-00012240: 6f76 6528 7265 6665 7265 6e63 6529 0a20  ove(reference). 
-00012250: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-00012260: 6c66 0a0a 2020 2020 6465 6620 7265 6d6f  lf..    def remo
-00012270: 7665 2873 656c 662c 2069 7465 6d73 293a  ve(self, items):
-00012280: 0a20 2020 2020 2020 2022 2222 5265 6d6f  .        """Remo
-00012290: 7665 7320 6974 656d 7320 6672 6f6d 2061  ves items from a
-000122a0: 2043 6f6d 706f 6e65 6e74 2c20 7768 6963   Component, whic
-000122b0: 6820 6361 6e20 696e 636c 7564 6520 506f  h can include Po
-000122c0: 7274 732c 2050 6f6c 7967 6f6e 5365 7473  rts, PolygonSets
-000122d0: 205c 0a20 2020 2020 2020 2043 656c 6c52   \.        CellR
-000122e0: 6566 6572 656e 6365 732c 2043 6f6d 706f  eferences, Compo
-000122f0: 6e65 6e74 5265 6665 7265 6e63 6573 2061  nentReferences a
-00012300: 6e64 204c 6162 656c 732e 0a0a 2020 2020  nd Labels...    
-00012310: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
-00012320: 2020 2020 2020 6974 656d 733a 206c 6973        items: lis
-00012330: 7420 6f66 2049 7465 6d73 2074 6f20 6265  t of Items to be
-00012340: 2072 656d 6f76 6564 2066 726f 6d20 7468   removed from th
-00012350: 6520 436f 6d70 6f6e 656e 742e 0a20 2020  e Component..   
-00012360: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00012370: 2069 6620 6e6f 7420 6861 7361 7474 7228   if not hasattr(
-00012380: 6974 656d 732c 2022 5f5f 6974 6572 5f5f  items, "__iter__
-00012390: 2229 3a0a 2020 2020 2020 2020 2020 2020  "):.            
-000123a0: 6974 656d 7320 3d20 5b69 7465 6d73 5d0a  items = [items].
-000123b0: 2020 2020 2020 2020 666f 7220 6974 656d          for item
-000123c0: 2069 6e20 6974 656d 733a 0a20 2020 2020   in items:.     
-000123d0: 2020 2020 2020 2069 6620 6973 696e 7374         if isinst
-000123e0: 616e 6365 2869 7465 6d2c 2050 6f72 7429  ance(item, Port)
-000123f0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00012400: 2020 7365 6c66 2e70 6f72 7473 203d 207b    self.ports = {
-00012410: 6b3a 2076 2066 6f72 206b 2c20 7620 696e  k: v for k, v in
-00012420: 2073 656c 662e 706f 7274 732e 6974 656d   self.ports.item
-00012430: 7328 2920 6966 2076 2021 3d20 6974 656d  s() if v != item
-00012440: 7d0a 2020 2020 2020 2020 2020 2020 656c  }.            el
-00012450: 6966 2069 7369 6e73 7461 6e63 6528 6974  if isinstance(it
-00012460: 656d 2c20 6764 7374 6b2e 5265 6665 7265  em, gdstk.Refere
-00012470: 6e63 6529 3a0a 2020 2020 2020 2020 2020  nce):.          
-00012480: 2020 2020 2020 7365 6c66 2e5f 6365 6c6c        self._cell
-00012490: 2e72 656d 6f76 6528 6974 656d 290a 2020  .remove(item).  
-000124a0: 2020 2020 2020 2020 2020 2020 2020 6974                it
-000124b0: 656d 2e6f 776e 6572 203d 204e 6f6e 650a  em.owner = None.
-000124c0: 2020 2020 2020 2020 2020 2020 656c 6966              elif
-000124d0: 2069 7369 6e73 7461 6e63 6528 6974 656d   isinstance(item
-000124e0: 2c20 436f 6d70 6f6e 656e 7452 6566 6572  , ComponentRefer
-000124f0: 656e 6365 293a 0a20 2020 2020 2020 2020  ence):.         
-00012500: 2020 2020 2020 2073 656c 662e 7265 6665         self.refe
-00012510: 7265 6e63 6573 2e72 656d 6f76 6528 6974  rences.remove(it
-00012520: 656d 290a 2020 2020 2020 2020 2020 2020  em).            
-00012530: 2020 2020 7365 6c66 2e5f 6365 6c6c 2e72      self._cell.r
-00012540: 656d 6f76 6528 6974 656d 2e5f 7265 6665  emove(item._refe
-00012550: 7265 6e63 6529 0a20 2020 2020 2020 2020  rence).         
-00012560: 2020 2020 2020 2069 7465 6d2e 6f77 6e65         item.owne
-00012570: 7220 3d20 4e6f 6e65 0a20 2020 2020 2020  r = None.       
-00012580: 2020 2020 2020 2020 2073 656c 662e 5f6e           self._n
-00012590: 616d 6564 5f72 6566 6572 656e 6365 732e  amed_references.
-000125a0: 706f 7028 6974 656d 2e6e 616d 6529 0a20  pop(item.name). 
-000125b0: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-000125c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000125d0: 2073 656c 662e 5f63 656c 6c2e 7265 6d6f   self._cell.remo
-000125e0: 7665 2869 7465 6d29 0a0a 2020 2020 2020  ve(item)..      
-000125f0: 2020 7365 6c66 2e5f 6262 5f76 616c 6964    self._bb_valid
-00012600: 203d 2046 616c 7365 0a20 2020 2020 2020   = False.       
-00012610: 2072 6574 7572 6e20 7365 6c66 0a0a 2020   return self..  
-00012620: 2020 6465 6620 6861 7368 5f67 656f 6d65    def hash_geome
-00012630: 7472 7928 7365 6c66 2c20 7072 6563 6973  try(self, precis
-00012640: 696f 6e3a 2066 6c6f 6174 203d 2031 652d  ion: float = 1e-
-00012650: 3429 202d 3e20 7374 723a 0a20 2020 2020  4) -> str:.     
-00012660: 2020 2022 2222 5265 7475 726e 7320 616e     """Returns an
-00012670: 2053 4841 3120 6861 7368 206f 6620 7468   SHA1 hash of th
-00012680: 6520 6765 6f6d 6574 7279 2069 6e20 7468  e geometry in th
-00012690: 6520 436f 6d70 6f6e 656e 742e 0a0a 2020  e Component...  
-000126a0: 2020 2020 2020 466f 7220 6561 6368 206c        For each l
-000126b0: 6179 6572 2c20 6561 6368 2070 6f6c 7967  ayer, each polyg
-000126c0: 6f6e 2069 7320 696e 6469 7669 6475 616c  on is individual
-000126d0: 6c79 2068 6173 6865 6420 616e 6420 7468  ly hashed and th
-000126e0: 656e 2074 6865 2070 6f6c 7967 6f6e 2068  en the polygon h
-000126f0: 6173 6865 730a 2020 2020 2020 2020 6172  ashes.        ar
-00012700: 6520 736f 7274 6564 2c20 746f 2065 6e73  e sorted, to ens
-00012710: 7572 6520 7468 6520 6861 7368 2073 7461  ure the hash sta
-00012720: 7973 2063 6f6e 7374 616e 7420 7265 6761  ys constant rega
-00012730: 7264 6c65 7373 206f 6620 7468 6520 6f72  rdless of the or
-00012740: 6465 7269 6e67 0a20 2020 2020 2020 2074  dering.        t
-00012750: 6865 2070 6f6c 7967 6f6e 732e 2020 5369  he polygons.  Si
-00012760: 6d69 6c61 726c 792c 2074 6865 206c 6179  milarly, the lay
-00012770: 6572 7320 6172 6520 736f 7274 6564 2062  ers are sorted b
-00012780: 7920 286c 6179 6572 2c20 6461 7461 7479  y (layer, dataty
-00012790: 7065 292e 0a0a 2020 2020 2020 2020 4172  pe)...        Ar
-000127a0: 6773 3a0a 2020 2020 2020 2020 2020 2020  gs:.            
-000127b0: 7072 6563 6973 696f 6e3a 2052 6f75 6e64  precision: Round
-000127c0: 696e 6720 7072 6563 6973 696f 6e20 666f  ing precision fo
-000127d0: 7220 7468 6520 7468 6520 6f62 6a65 6374  r the the object
-000127e0: 7320 696e 2074 6865 2043 6f6d 706f 6e65  s in the Compone
-000127f0: 6e74 2e0a 2020 2020 2020 2020 2020 2020  nt..            
-00012800: 2020 2020 466f 7220 696e 7374 616e 6365      For instance
-00012810: 2c20 6120 7072 6563 6973 696f 6e20 6f66  , a precision of
-00012820: 2031 652d 3220 7769 6c6c 2072 6f75 6e64   1e-2 will round
-00012830: 2061 2070 6f69 6e74 2061 740a 2020 2020   a point at.    
-00012840: 2020 2020 2020 2020 2020 2020 2830 2e31              (0.1
-00012850: 3234 2c20 312e 3734 3829 2074 6f20 2830  24, 1.748) to (0
-00012860: 2e31 322c 2031 2e37 3529 2e0a 0a20 2020  .12, 1.75)...   
-00012870: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00012880: 2070 6f6c 7967 6f6e 735f 6279 5f73 7065   polygons_by_spe
-00012890: 6320 3d20 7365 6c66 2e67 6574 5f70 6f6c  c = self.get_pol
-000128a0: 7967 6f6e 7328 6279 5f73 7065 633d 5472  ygons(by_spec=Tr
-000128b0: 7565 2c20 6173 5f61 7272 6179 3d46 616c  ue, as_array=Fal
-000128c0: 7365 290a 2020 2020 2020 2020 6c61 7965  se).        laye
-000128d0: 7273 203d 206e 702e 6172 7261 7928 6c69  rs = np.array(li
-000128e0: 7374 2870 6f6c 7967 6f6e 735f 6279 5f73  st(polygons_by_s
-000128f0: 7065 632e 6b65 7973 2829 2929 0a20 2020  pec.keys())).   
-00012900: 2020 2020 2073 6f72 7465 645f 6c61 7965       sorted_laye
-00012910: 7273 203d 206c 6179 6572 735b 6e70 2e6c  rs = layers[np.l
-00012920: 6578 736f 7274 2828 6c61 7965 7273 5b3a  exsort((layers[:
-00012930: 2c20 305d 2c20 6c61 7965 7273 5b3a 2c20  , 0], layers[:, 
-00012940: 315d 2929 5d0a 0a20 2020 2020 2020 2066  1]))]..        f
-00012950: 696e 616c 5f68 6173 6820 3d20 6861 7368  inal_hash = hash
-00012960: 6c69 622e 7368 6131 2829 0a20 2020 2020  lib.sha1().     
-00012970: 2020 2066 6f72 206c 6179 6572 2069 6e20     for layer in 
-00012980: 736f 7274 6564 5f6c 6179 6572 733a 0a20  sorted_layers:. 
-00012990: 2020 2020 2020 2020 2020 206c 6179 6572             layer
-000129a0: 5f68 6173 6820 3d20 6861 7368 6c69 622e  _hash = hashlib.
-000129b0: 7368 6131 286c 6179 6572 2e61 7374 7970  sha1(layer.astyp
-000129c0: 6528 6e70 2e69 6e74 3634 2929 2e64 6967  e(np.int64)).dig
-000129d0: 6573 7428 290a 2020 2020 2020 2020 2020  est().          
-000129e0: 2020 706f 6c79 676f 6e73 203d 2070 6f6c    polygons = pol
-000129f0: 7967 6f6e 735f 6279 5f73 7065 635b 7475  ygons_by_spec[tu
-00012a00: 706c 6528 6c61 7965 7229 5d0a 2020 2020  ple(layer)].    
-00012a10: 2020 2020 2020 2020 706f 6c79 676f 6e73          polygons
-00012a20: 203d 205b 5f72 6e64 2870 2e70 6f69 6e74   = [_rnd(p.point
-00012a30: 732c 2070 7265 6369 7369 6f6e 2920 666f  s, precision) fo
-00012a40: 7220 7020 696e 2070 6f6c 7967 6f6e 735d  r p in polygons]
-00012a50: 0a20 2020 2020 2020 2020 2020 2070 6f6c  .            pol
-00012a60: 7967 6f6e 5f68 6173 6865 7320 3d20 6e70  ygon_hashes = np
-00012a70: 2e73 6f72 7428 5b68 6173 686c 6962 2e73  .sort([hashlib.s
-00012a80: 6861 3128 7029 2e64 6967 6573 7428 2920  ha1(p).digest() 
-00012a90: 666f 7220 7020 696e 2070 6f6c 7967 6f6e  for p in polygon
-00012aa0: 735d 290a 2020 2020 2020 2020 2020 2020  s]).            
-00012ab0: 6669 6e61 6c5f 6861 7368 2e75 7064 6174  final_hash.updat
-00012ac0: 6528 6c61 7965 725f 6861 7368 290a 2020  e(layer_hash).  
-00012ad0: 2020 2020 2020 2020 2020 666f 7220 7068            for ph
-00012ae0: 2069 6e20 706f 6c79 676f 6e5f 6861 7368   in polygon_hash
-00012af0: 6573 3a0a 2020 2020 2020 2020 2020 2020  es:.            
-00012b00: 2020 2020 6669 6e61 6c5f 6861 7368 2e75      final_hash.u
-00012b10: 7064 6174 6528 7068 290a 0a20 2020 2020  pdate(ph)..     
-00012b20: 2020 2072 6574 7572 6e20 6669 6e61 6c5f     return final_
-00012b30: 6861 7368 2e68 6578 6469 6765 7374 2829  hash.hexdigest()
-00012b40: 0a0a 2020 2020 6465 6620 6765 745f 6c61  ..    def get_la
-00012b50: 6265 6c73 280a 2020 2020 2020 2020 7365  bels(.        se
-00012b60: 6c66 2c20 6170 706c 795f 7265 7065 7469  lf, apply_repeti
-00012b70: 7469 6f6e 733d 5472 7565 2c20 6465 7074  tions=True, dept
-00012b80: 683a 204f 7074 696f 6e61 6c5b 696e 745d  h: Optional[int]
-00012b90: 203d 204e 6f6e 652c 206c 6179 6572 3d4e   = None, layer=N
-00012ba0: 6f6e 650a 2020 2020 2920 2d3e 204c 6973  one.    ) -> Lis
-00012bb0: 745b 4c61 6265 6c5d 3a0a 2020 2020 2020  t[Label]:.      
-00012bc0: 2020 2222 2252 6574 7572 6e20 6c61 6265    """Return labe
-00012bd0: 6c73 2e0a 0a20 2020 2020 2020 2041 7267  ls...        Arg
-00012be0: 733a 0a20 2020 2020 2020 2020 2020 2061  s:.            a
-00012bf0: 7070 6c79 5f72 6570 6574 6974 696f 6e73  pply_repetitions
-00012c00: 3a2e 0a20 2020 2020 2020 2020 2020 2064  :..            d
-00012c10: 6570 7468 3a20 4e6f 6e65 2072 6574 7572  epth: None retur
-00012c20: 6e73 2061 6c6c 206c 6162 656c 7320 616e  ns all labels an
-00012c30: 6420 3020 746f 7020 6c65 7665 6c2e 0a20  d 0 top level.. 
-00012c40: 2020 2020 2020 2020 2020 206c 6179 6572             layer
-00012c50: 3a20 6c61 7965 7273 7065 632e 0a20 2020  : layerspec..   
-00012c60: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00012c70: 2066 726f 6d20 6764 7366 6163 746f 7279   from gdsfactory
-00012c80: 2e70 646b 2069 6d70 6f72 7420 6765 745f  .pdk import get_
-00012c90: 6c61 7965 720a 0a20 2020 2020 2020 2069  layer..        i
-00012ca0: 6620 6c61 7965 723a 0a20 2020 2020 2020  f layer:.       
-00012cb0: 2020 2020 206c 6179 6572 2c20 7465 7874       layer, text
-00012cc0: 7479 7065 203d 2067 6574 5f6c 6179 6572  type = get_layer
-00012cd0: 286c 6179 6572 290a 2020 2020 2020 2020  (layer).        
-00012ce0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-00012cf0: 2020 7465 7874 7479 7065 203d 204e 6f6e    texttype = Non
-00012d00: 650a 2020 2020 2020 2020 7265 7475 726e  e.        return
-00012d10: 2073 656c 662e 5f63 656c 6c2e 6765 745f   self._cell.get_
-00012d20: 6c61 6265 6c73 280a 2020 2020 2020 2020  labels(.        
-00012d30: 2020 2020 6170 706c 795f 7265 7065 7469      apply_repeti
-00012d40: 7469 6f6e 733d 6170 706c 795f 7265 7065  tions=apply_repe
-00012d50: 7469 7469 6f6e 732c 0a20 2020 2020 2020  titions,.       
-00012d60: 2020 2020 2064 6570 7468 3d64 6570 7468       depth=depth
-00012d70: 2c0a 2020 2020 2020 2020 2020 2020 6c61  ,.            la
-00012d80: 7965 723d 6c61 7965 722c 0a20 2020 2020  yer=layer,.     
-00012d90: 2020 2020 2020 2074 6578 7474 7970 653d         texttype=
-00012da0: 7465 7874 7479 7065 2c0a 2020 2020 2020  texttype,.      
-00012db0: 2020 290a 0a20 2020 2064 6566 2072 656d    )..    def rem
-00012dc0: 6f76 655f 6c61 6265 6c73 2873 656c 6629  ove_labels(self)
-00012dd0: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
-00012de0: 2020 2222 2252 656d 6f76 6520 6c61 6265    """Remove labe
-00012df0: 6c73 2e22 2222 0a20 2020 2020 2020 2073  ls.""".        s
-00012e00: 656c 662e 5f63 656c 6c2e 7265 6d6f 7665  elf._cell.remove
-00012e10: 282a 7365 6c66 2e6c 6162 656c 7329 0a0a  (*self.labels)..
-00012e20: 2020 2020 2320 4465 7072 6563 6174 6564      # Deprecated
-00012e30: 0a20 2020 2064 6566 2067 6574 5f69 6e66  .    def get_inf
-00012e40: 6f28 7365 6c66 293a 0a20 2020 2020 2020  o(self):.       
-00012e50: 2022 2222 4761 7468 6572 7320 7468 6520   """Gathers the 
-00012e60: 2e69 6e66 6f20 6469 6374 696f 6e61 7269  .info dictionari
-00012e70: 6573 2066 726f 6d20 6576 6572 7920 7375  es from every su
-00012e80: 622d 436f 6d70 6f6e 656e 7420 616e 6420  b-Component and 
-00012e90: 7265 7475 726e 7320 7468 656d 2069 6e20  returns them in 
-00012ea0: 6120 6c69 7374 2e0a 0a20 2020 2020 2020  a list...       
-00012eb0: 2041 7267 733a 0a20 2020 2020 2020 2020   Args:.         
-00012ec0: 2020 2064 6570 7468 3a20 696e 7420 6f72     depth: int or
-00012ed0: 204e 6f6e 650a 2020 2020 2020 2020 2020   None.          
-00012ee0: 2020 2020 2020 4966 206e 6f74 204e 6f6e        If not Non
-00012ef0: 652c 2064 6566 696e 6573 2066 726f 6d20  e, defines from 
-00012f00: 686f 7720 6d61 6e79 2072 6566 6572 656e  how many referen
-00012f10: 6365 206c 6576 656c 7320 746f 0a20 2020  ce levels to.   
-00012f20: 2020 2020 2020 2020 2020 2020 2072 6574               ret
-00012f30: 7269 6576 6520 506f 7274 7320 6672 6f6d  rieve Ports from
-00012f40: 2e0a 0a20 2020 2020 2020 2052 6574 7572  ...        Retur
-00012f50: 6e73 3a0a 2020 2020 2020 2020 2020 2020  ns:.            
-00012f60: 6c69 7374 206f 6620 6469 6374 696f 6e61  list of dictiona
-00012f70: 7269 6573 0a20 2020 2020 2020 2020 2020  ries.           
-00012f80: 2020 2020 204c 6973 7420 6f66 2074 6865       List of the
-00012f90: 2022 2e69 6e66 6f22 2070 726f 7065 7274   ".info" propert
-00012fa0: 7920 6469 6374 696f 6e61 7269 6573 2066  y dictionaries f
-00012fb0: 726f 6d20 616c 6c20 7375 622d 436f 6d70  rom all sub-Comp
-00012fc0: 6f6e 656e 7473 0a20 2020 2020 2020 2022  onents.        "
-00012fd0: 2222 0a20 2020 2020 2020 2044 5f6c 6973  "".        D_lis
-00012fe0: 7420 3d20 7365 6c66 2e67 6574 5f64 6570  t = self.get_dep
-00012ff0: 656e 6465 6e63 6965 7328 7265 6375 7273  endencies(recurs
-00013000: 6976 653d 5472 7565 290a 2020 2020 2020  ive=True).      
-00013010: 2020 7265 7475 726e 205b 442e 696e 666f    return [D.info
-00013020: 2e63 6f70 7928 2920 666f 7220 4420 696e  .copy() for D in
-00013030: 2044 5f6c 6973 745d 0a0a 2020 2020 6465   D_list]..    de
-00013040: 6620 7265 6d61 705f 6c61 7965 7273 280a  f remap_layers(.
-00013050: 2020 2020 2020 2020 7365 6c66 2c20 6c61          self, la
-00013060: 7965 726d 6170 2c20 696e 636c 7564 655f  yermap, include_
-00013070: 6c61 6265 6c73 3a20 626f 6f6c 203d 2054  labels: bool = T
-00013080: 7275 652c 2069 6e63 6c75 6465 5f70 6174  rue, include_pat
-00013090: 6873 3a20 626f 6f6c 203d 2054 7275 650a  hs: bool = True.
-000130a0: 2020 2020 2920 2d3e 2043 6f6d 706f 6e65      ) -> Compone
-000130b0: 6e74 3a0a 2020 2020 2020 2020 2222 2252  nt:.        """R
-000130c0: 6574 7572 6e73 2061 2063 6f70 7920 6f66  eturns a copy of
-000130d0: 2074 6865 2063 6f6d 706f 6e65 6e74 2077   the component w
-000130e0: 6974 6820 7265 6d61 7070 6564 206c 6179  ith remapped lay
-000130f0: 6572 732e 0a0a 2020 2020 2020 2020 4172  ers...        Ar
-00013100: 6773 3a0a 2020 2020 2020 2020 2020 2020  gs:.            
-00013110: 6c61 7965 726d 6170 3a20 4469 6374 696f  layermap: Dictio
-00013120: 6e61 7279 206f 6620 7661 6c75 6573 2069  nary of values i
-00013130: 6e20 666f 726d 6174 207b 6c61 7965 725f  n format {layer_
-00013140: 6672 6f6d 203a 206c 6179 6572 5f74 6f7d  from : layer_to}
-00013150: 2e0a 2020 2020 2020 2020 2020 2020 696e  ..            in
-00013160: 636c 7564 655f 6c61 6265 6c73 3a20 5365  clude_labels: Se
-00013170: 6c65 6374 7320 7768 6574 6865 7220 746f  lects whether to
-00013180: 206d 6f76 6520 4c61 6265 6c73 2061 6c6f   move Labels alo
-00013190: 6e67 2077 6974 6820 706f 6c79 676f 6e73  ng with polygons
-000131a0: 2e0a 2020 2020 2020 2020 2020 2020 696e  ..            in
-000131b0: 636c 7564 655f 7061 7468 733a 2053 656c  clude_paths: Sel
-000131c0: 6563 7473 2077 6865 7468 6572 2074 6f20  ects whether to 
-000131d0: 6d6f 7665 2050 6174 6873 2061 6c6f 6e67  move Paths along
-000131e0: 2077 6974 6820 706f 6c79 676f 6e73 2e0a   with polygons..
-000131f0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00013200: 2020 2020 636f 6d70 6f6e 656e 7420 3d20      component = 
-00013210: 7365 6c66 2e63 6f70 7928 290a 2020 2020  self.copy().    
-00013220: 2020 2020 6c61 7965 726d 6170 203d 207b      layermap = {
-00013230: 5f70 6172 7365 5f6c 6179 6572 286b 293a  _parse_layer(k):
-00013240: 205f 7061 7273 655f 6c61 7965 7228 7629   _parse_layer(v)
-00013250: 2066 6f72 206b 2c20 7620 696e 206c 6179   for k, v in lay
-00013260: 6572 6d61 702e 6974 656d 7328 297d 0a0a  ermap.items()}..
-00013270: 2020 2020 2020 2020 616c 6c5f 4420 3d20          all_D = 
-00013280: 6c69 7374 2863 6f6d 706f 6e65 6e74 2e67  list(component.g
-00013290: 6574 5f64 6570 656e 6465 6e63 6965 7328  et_dependencies(
-000132a0: 5472 7565 2929 0a20 2020 2020 2020 2061  True)).        a
-000132b0: 6c6c 5f44 2e61 7070 656e 6428 636f 6d70  ll_D.append(comp
-000132c0: 6f6e 656e 7429 0a20 2020 2020 2020 2066  onent).        f
-000132d0: 6f72 2044 2069 6e20 616c 6c5f 443a 0a20  or D in all_D:. 
-000132e0: 2020 2020 2020 2020 2020 2066 6f72 2070             for p
-000132f0: 2069 6e20 442e 706f 6c79 676f 6e73 3a0a   in D.polygons:.
-00013300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013310: 6c61 7965 7220 3d20 2870 2e6c 6179 6572  layer = (p.layer
-00013320: 2c20 702e 6461 7461 7479 7065 290a 2020  , p.datatype).  
-00013330: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00013340: 206c 6179 6572 2069 6e20 6c61 7965 726d   layer in layerm
-00013350: 6170 3a0a 2020 2020 2020 2020 2020 2020  ap:.            
-00013360: 2020 2020 2020 2020 6e65 775f 6c61 7965          new_laye
-00013370: 7220 3d20 6c61 7965 726d 6170 5b6c 6179  r = layermap[lay
-00013380: 6572 5d0a 2020 2020 2020 2020 2020 2020  er].            
-00013390: 2020 2020 2020 2020 702e 6c61 7965 7220          p.layer 
-000133a0: 3d20 6e65 775f 6c61 7965 725b 305d 0a20  = new_layer[0]. 
-000133b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000133c0: 2020 2070 2e64 6174 6174 7970 6520 3d20     p.datatype = 
-000133d0: 6e65 775f 6c61 7965 725b 315d 0a20 2020  new_layer[1].   
-000133e0: 2020 2020 2020 2020 2069 6620 696e 636c           if incl
-000133f0: 7564 655f 6c61 6265 6c73 3a0a 2020 2020  ude_labels:.    
-00013400: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-00013410: 6c61 6265 6c20 696e 2044 2e6c 6162 656c  label in D.label
-00013420: 733a 0a20 2020 2020 2020 2020 2020 2020  s:.             
-00013430: 2020 2020 2020 206f 7269 6769 6e61 6c5f         original_
-00013440: 6c61 7965 7220 3d20 286c 6162 656c 2e6c  layer = (label.l
-00013450: 6179 6572 2c20 6c61 6265 6c2e 7465 7874  ayer, label.text
-00013460: 7479 7065 290a 2020 2020 2020 2020 2020  type).          
-00013470: 2020 2020 2020 2020 2020 6f72 6967 696e            origin
-00013480: 616c 5f6c 6179 6572 203d 205f 7061 7273  al_layer = _pars
-00013490: 655f 6c61 7965 7228 6f72 6967 696e 616c  e_layer(original
-000134a0: 5f6c 6179 6572 290a 2020 2020 2020 2020  _layer).        
-000134b0: 2020 2020 2020 2020 2020 2020 6966 206f              if o
-000134c0: 7269 6769 6e61 6c5f 6c61 7965 7220 696e  riginal_layer in
-000134d0: 206c 6179 6572 6d61 703a 0a20 2020 2020   layermap:.     
-000134e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000134f0: 2020 206e 6577 5f6c 6179 6572 203d 206c     new_layer = l
-00013500: 6179 6572 6d61 705b 6f72 6967 696e 616c  ayermap[original
-00013510: 5f6c 6179 6572 5d0a 2020 2020 2020 2020  _layer].        
-00013520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013530: 6c61 6265 6c2e 6c61 7965 7220 3d20 6e65  label.layer = ne
-00013540: 775f 6c61 7965 725b 305d 0a20 2020 2020  w_layer[0].     
-00013550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013560: 2020 206c 6162 656c 2e74 6578 7474 7970     label.texttyp
-00013570: 6520 3d20 6e65 775f 6c61 7965 725b 315d  e = new_layer[1]
-00013580: 0a0a 2020 2020 2020 2020 2020 2020 6966  ..            if
-00013590: 2069 6e63 6c75 6465 5f70 6174 6873 3a0a   include_paths:.
-000135a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000135b0: 666f 7220 7061 7468 2069 6e20 442e 7061  for path in D.pa
-000135c0: 7468 733a 0a20 2020 2020 2020 2020 2020  ths:.           
-000135d0: 2020 2020 2020 2020 206e 6577 5f6c 6179           new_lay
-000135e0: 6572 7320 3d20 6c69 7374 2870 6174 682e  ers = list(path.
-000135f0: 6c61 7965 7273 290a 2020 2020 2020 2020  layers).        
-00013600: 2020 2020 2020 2020 2020 2020 6e65 775f              new_
-00013610: 6461 7461 7479 7065 7320 3d20 6c69 7374  datatypes = list
-00013620: 2870 6174 682e 6461 7461 7479 7065 7329  (path.datatypes)
-00013630: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00013640: 2020 2020 2066 6f72 206c 6179 6572 5f6e       for layer_n
-00013650: 756d 6265 7220 696e 2072 616e 6765 286c  umber in range(l
-00013660: 656e 286e 6577 5f6c 6179 6572 7329 293a  en(new_layers)):
-00013670: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00013680: 2020 2020 2020 2020 206f 7269 6769 6e61           origina
-00013690: 6c5f 6c61 7965 7220 3d20 5f70 6172 7365  l_layer = _parse
-000136a0: 5f6c 6179 6572 280a 2020 2020 2020 2020  _layer(.        
-000136b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000136c0: 2020 2020 286e 6577 5f6c 6179 6572 735b      (new_layers[
-000136d0: 6c61 7965 725f 6e75 6d62 6572 5d2c 206e  layer_number], n
-000136e0: 6577 5f64 6174 6174 7970 6573 5b6c 6179  ew_datatypes[lay
-000136f0: 6572 5f6e 756d 6265 725d 290a 2020 2020  er_number]).    
-00013700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013710: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
-00013720: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00013730: 206f 7269 6769 6e61 6c5f 6c61 7965 7220   original_layer 
-00013740: 696e 206c 6179 6572 6d61 703a 0a20 2020  in layermap:.   
+0000eea0: 6566 6175 6c74 5f73 6574 7469 6e67 732e  efault_settings.
+0000eeb0: 6469 6374 2829 0a20 2020 2020 2020 207d  dict().        }
+0000eec0: 0a20 2020 2020 2020 2065 7870 6c69 6369  .        explici
+0000eed0: 745f 6f61 735f 7365 7474 696e 6773 203d  t_oas_settings =
+0000eee0: 207b 0a20 2020 2020 2020 2020 2020 206b   {.            k
+0000eef0: 3a20 760a 2020 2020 2020 2020 2020 2020  : v.            
+0000ef00: 666f 7220 6b2c 2076 2069 6e20 6b77 6172  for k, v in kwar
+0000ef10: 6773 2e69 7465 6d73 2829 0a20 2020 2020  gs.items().     
+0000ef20: 2020 2020 2020 2069 6620 7620 6973 206e         if v is n
+0000ef30: 6f74 204e 6f6e 6520 616e 6420 6b20 696e  ot None and k in
+0000ef40: 2064 6566 6175 6c74 5f6f 6173 6973 5f73   default_oasis_s
+0000ef50: 6574 7469 6e67 732e 6469 6374 2829 0a20  ettings.dict(). 
+0000ef60: 2020 2020 2020 207d 0a20 2020 2020 2020         }.       
+0000ef70: 2023 2075 7064 6174 6520 7468 6520 7772   # update the wr
+0000ef80: 6974 6520 7365 7474 696e 6773 2077 6974  ite settings wit
+0000ef90: 6820 616e 7920 7365 7474 696e 6773 2065  h any settings e
+0000efa0: 7870 6c69 6369 746c 7920 7061 7373 6564  xplicitly passed
+0000efb0: 0a20 2020 2020 2020 2077 7269 7465 5f73  .        write_s
+0000efc0: 6574 7469 6e67 7320 3d20 6465 6661 756c  ettings = defaul
+0000efd0: 745f 7365 7474 696e 6773 2e63 6f70 7928  t_settings.copy(
+0000efe0: 7570 6461 7465 3d65 7870 6c69 6369 745f  update=explicit_
+0000eff0: 6764 735f 7365 7474 696e 6773 290a 2020  gds_settings).  
+0000f000: 2020 2020 2020 6f61 7369 735f 7365 7474        oasis_sett
+0000f010: 696e 6773 203d 2064 6566 6175 6c74 5f6f  ings = default_o
+0000f020: 6173 6973 5f73 6574 7469 6e67 732e 636f  asis_settings.co
+0000f030: 7079 2875 7064 6174 653d 6578 706c 6963  py(update=explic
+0000f040: 6974 5f6f 6173 5f73 6574 7469 6e67 7329  it_oas_settings)
+0000f050: 0a0a 2020 2020 2020 2020 5f63 6865 636b  ..        _check
+0000f060: 5f75 6e63 6163 6865 645f 636f 6d70 6f6e  _uncached_compon
+0000f070: 656e 7473 280a 2020 2020 2020 2020 2020  ents(.          
+0000f080: 2020 636f 6d70 6f6e 656e 743d 7365 6c66    component=self
+0000f090: 2c20 6d6f 6465 3d77 7269 7465 5f73 6574  , mode=write_set
+0000f0a0: 7469 6e67 732e 6f6e 5f75 6e63 6163 6865  tings.on_uncache
+0000f0b0: 645f 636f 6d70 6f6e 656e 740a 2020 2020  d_component.    
+0000f0c0: 2020 2020 290a 0a20 2020 2020 2020 2069      )..        i
+0000f0d0: 6620 7772 6974 655f 7365 7474 696e 6773  f write_settings
+0000f0e0: 2e66 6c61 7474 656e 5f69 6e76 616c 6964  .flatten_invalid
+0000f0f0: 5f72 6566 733a 0a20 2020 2020 2020 2020  _refs:.         
+0000f100: 2020 2074 6f70 5f63 656c 6c20 3d20 666c     top_cell = fl
+0000f110: 6174 7465 6e5f 696e 7661 6c69 645f 7265  atten_invalid_re
+0000f120: 6673 5f72 6563 7572 7369 7665 2873 656c  fs_recursive(sel
+0000f130: 6629 0a20 2020 2020 2020 2065 6c73 653a  f).        else:
+0000f140: 0a20 2020 2020 2020 2020 2020 2074 6f70  .            top
+0000f150: 5f63 656c 6c20 3d20 7365 6c66 0a0a 2020  _cell = self..  
+0000f160: 2020 2020 2020 6764 7364 6972 203d 2067        gdsdir = g
+0000f170: 6473 6469 7220 6f72 2047 4453 4449 525f  dsdir or GDSDIR_
+0000f180: 5445 4d50 0a20 2020 2020 2020 2067 6473  TEMP.        gds
+0000f190: 6469 7220 3d20 7061 7468 6c69 622e 5061  dir = pathlib.Pa
+0000f1a0: 7468 2867 6473 6469 7229 0a20 2020 2020  th(gdsdir).     
+0000f1b0: 2020 2069 6620 7769 7468 5f6f 6173 6973     if with_oasis
+0000f1c0: 3a0a 2020 2020 2020 2020 2020 2020 6764  :.            gd
+0000f1d0: 7370 6174 6820 3d20 6764 7370 6174 6820  spath = gdspath 
+0000f1e0: 6f72 2067 6473 6469 7220 2f20 6622 7b74  or gdsdir / f"{t
+0000f1f0: 6f70 5f63 656c 6c2e 6e61 6d65 7d2e 6f61  op_cell.name}.oa
+0000f200: 7322 0a20 2020 2020 2020 2065 6c73 653a  s".        else:
+0000f210: 0a20 2020 2020 2020 2020 2020 2067 6473  .            gds
+0000f220: 7061 7468 203d 2067 6473 7061 7468 206f  path = gdspath o
+0000f230: 7220 6764 7364 6972 202f 2066 227b 746f  r gdsdir / f"{to
+0000f240: 705f 6365 6c6c 2e6e 616d 657d 2e67 6473  p_cell.name}.gds
+0000f250: 220a 2020 2020 2020 2020 6764 7370 6174  ".        gdspat
+0000f260: 6820 3d20 7061 7468 6c69 622e 5061 7468  h = pathlib.Path
+0000f270: 2867 6473 7061 7468 290a 2020 2020 2020  (gdspath).      
+0000f280: 2020 6764 7364 6972 203d 2067 6473 7061    gdsdir = gdspa
+0000f290: 7468 2e70 6172 656e 740a 2020 2020 2020  th.parent.      
+0000f2a0: 2020 6764 7364 6972 2e6d 6b64 6972 2865    gdsdir.mkdir(e
+0000f2b0: 7869 7374 5f6f 6b3d 5472 7565 2c20 7061  xist_ok=True, pa
+0000f2c0: 7265 6e74 733d 5472 7565 290a 0a20 2020  rents=True)..   
+0000f2d0: 2020 2020 2063 656c 6c73 203d 2074 6f70       cells = top
+0000f2e0: 5f63 656c 6c2e 6765 745f 6465 7065 6e64  _cell.get_depend
+0000f2f0: 656e 6369 6573 2872 6563 7572 7369 7665  encies(recursive
+0000f300: 3d54 7275 6529 0a20 2020 2020 2020 2063  =True).        c
+0000f310: 656c 6c5f 6e61 6d65 7320 3d20 5b63 656c  ell_names = [cel
+0000f320: 6c2e 6e61 6d65 2066 6f72 2063 656c 6c20  l.name for cell 
+0000f330: 696e 206c 6973 7428 6365 6c6c 7329 5d0a  in list(cells)].
+0000f340: 2020 2020 2020 2020 6365 6c6c 5f6e 616d          cell_nam
+0000f350: 6573 5f75 6e69 7175 6520 3d20 7365 7428  es_unique = set(
+0000f360: 6365 6c6c 5f6e 616d 6573 290a 0a20 2020  cell_names)..   
+0000f370: 2020 2020 2069 6620 6c65 6e28 6365 6c6c       if len(cell
+0000f380: 5f6e 616d 6573 2920 213d 206c 656e 2873  _names) != len(s
+0000f390: 6574 2863 656c 6c5f 6e61 6d65 7329 293a  et(cell_names)):
+0000f3a0: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
+0000f3b0: 2063 656c 6c5f 6e61 6d65 2069 6e20 6365   cell_name in ce
+0000f3c0: 6c6c 5f6e 616d 6573 5f75 6e69 7175 653a  ll_names_unique:
+0000f3d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000f3e0: 2063 656c 6c5f 6e61 6d65 732e 7265 6d6f   cell_names.remo
+0000f3f0: 7665 2863 656c 6c5f 6e61 6d65 290a 0a20  ve(cell_name).. 
+0000f400: 2020 2020 2020 2020 2020 2069 6620 7772             if wr
+0000f410: 6974 655f 7365 7474 696e 6773 2e6f 6e5f  ite_settings.on_
+0000f420: 6475 706c 6963 6174 655f 6365 6c6c 203d  duplicate_cell =
+0000f430: 3d20 2265 7272 6f72 223a 0a20 2020 2020  = "error":.     
+0000f440: 2020 2020 2020 2020 2020 2072 6169 7365             raise
+0000f450: 2056 616c 7565 4572 726f 7228 0a20 2020   ValueError(.   
+0000f460: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f470: 2066 2244 7570 6c69 6361 7465 6420 6365   f"Duplicated ce
+0000f480: 6c6c 206e 616d 6573 2069 6e20 7b74 6f70  ll names in {top
+0000f490: 5f63 656c 6c2e 6e61 6d65 2172 7d3a 207b  _cell.name!r}: {
+0000f4a0: 6365 6c6c 5f6e 616d 6573 2172 7d22 0a20  cell_names!r}". 
+0000f4b0: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+0000f4c0: 0a20 2020 2020 2020 2020 2020 2065 6c69  .            eli
+0000f4d0: 6620 7772 6974 655f 7365 7474 696e 6773  f write_settings
+0000f4e0: 2e6f 6e5f 6475 706c 6963 6174 655f 6365  .on_duplicate_ce
+0000f4f0: 6c6c 2069 6e20 7b22 7761 726e 222c 2022  ll in {"warn", "
+0000f500: 6f76 6572 7772 6974 6522 7d3a 0a20 2020  overwrite"}:.   
+0000f510: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+0000f520: 7772 6974 655f 7365 7474 696e 6773 2e6f  write_settings.o
+0000f530: 6e5f 6475 706c 6963 6174 655f 6365 6c6c  n_duplicate_cell
+0000f540: 203d 3d20 2277 6172 6e22 3a0a 2020 2020   == "warn":.    
+0000f550: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f560: 7761 726e 696e 6773 2e77 6172 6e28 0a20  warnings.warn(. 
+0000f570: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f580: 2020 2020 2020 2066 2244 7570 6c69 6361         f"Duplica
+0000f590: 7465 6420 6365 6c6c 206e 616d 6573 2069  ted cell names i
+0000f5a0: 6e20 7b74 6f70 5f63 656c 6c2e 6e61 6d65  n {top_cell.name
+0000f5b0: 2172 7d3a 2020 7b63 656c 6c5f 6e61 6d65  !r}:  {cell_name
+0000f5c0: 737d 222c 0a20 2020 2020 2020 2020 2020  s}",.           
+0000f5d0: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+0000f5e0: 2020 2020 2020 2020 2020 2063 656c 6c73             cells
+0000f5f0: 5f64 6963 7420 3d20 7b63 656c 6c2e 6e61  _dict = {cell.na
+0000f600: 6d65 3a20 6365 6c6c 2e5f 6365 6c6c 2066  me: cell._cell f
+0000f610: 6f72 2063 656c 6c20 696e 2063 656c 6c73  or cell in cells
+0000f620: 7d0a 2020 2020 2020 2020 2020 2020 2020  }.              
+0000f630: 2020 6365 6c6c 7320 3d20 6365 6c6c 735f    cells = cells_
+0000f640: 6469 6374 2e76 616c 7565 7328 290a 2020  dict.values().  
+0000f650: 2020 2020 2020 2020 2020 656c 6966 2077            elif w
+0000f660: 7269 7465 5f73 6574 7469 6e67 732e 6f6e  rite_settings.on
+0000f670: 5f64 7570 6c69 6361 7465 5f63 656c 6c20  _duplicate_cell 
+0000f680: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+0000f690: 2020 2020 2020 2020 2020 2020 2072 6169               rai
+0000f6a0: 7365 2056 616c 7565 4572 726f 7228 0a20  se ValueError(. 
+0000f6b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f6c0: 2020 2066 226f 6e5f 6475 706c 6963 6174     f"on_duplicat
+0000f6d0: 655f 6365 6c6c 3a20 7b77 7269 7465 5f73  e_cell: {write_s
+0000f6e0: 6574 7469 6e67 732e 6f6e 5f64 7570 6c69  ettings.on_dupli
+0000f6f0: 6361 7465 5f63 656c 6c21 727d 206e 6f74  cate_cell!r} not
+0000f700: 2069 6e20 284e 6f6e 652c 2077 6172 6e2c   in (None, warn,
+0000f710: 2065 7272 6f72 2c20 6f76 6572 7772 6974   error, overwrit
+0000f720: 6529 220a 2020 2020 2020 2020 2020 2020  e)".            
+0000f730: 2020 2020 290a 0a20 2020 2020 2020 2061      )..        a
+0000f740: 6c6c 5f63 656c 6c73 203d 205b 746f 705f  ll_cells = [top_
+0000f750: 6365 6c6c 2e5f 6365 6c6c 5d20 2b20 736f  cell._cell] + so
+0000f760: 7274 6564 2863 656c 6c73 2c20 6b65 793d  rted(cells, key=
+0000f770: 6c61 6d62 6461 2063 633a 2063 632e 6e61  lambda cc: cc.na
+0000f780: 6d65 290a 0a20 2020 2020 2020 206e 6f5f  me)..        no_
+0000f790: 6e61 6d65 5f63 656c 6c73 203d 205b 0a20  name_cells = [. 
+0000f7a0: 2020 2020 2020 2020 2020 2063 656c 6c2e             cell.
+0000f7b0: 6e61 6d65 2066 6f72 2063 656c 6c20 696e  name for cell in
+0000f7c0: 2061 6c6c 5f63 656c 6c73 2069 6620 6365   all_cells if ce
+0000f7d0: 6c6c 2e6e 616d 652e 7374 6172 7473 7769  ll.name.startswi
+0000f7e0: 7468 2822 556e 6e61 6d65 6422 290a 2020  th("Unnamed").  
+0000f7f0: 2020 2020 2020 5d0a 0a20 2020 2020 2020        ]..       
+0000f800: 2069 6620 6e6f 5f6e 616d 655f 6365 6c6c   if no_name_cell
+0000f810: 733a 0a20 2020 2020 2020 2020 2020 2077  s:.            w
+0000f820: 6172 6e69 6e67 732e 7761 726e 280a 2020  arnings.warn(.  
+0000f830: 2020 2020 2020 2020 2020 2020 2020 6622                f"
+0000f840: 436f 6d70 6f6e 656e 7420 7b74 6f70 5f63  Component {top_c
+0000f850: 656c 6c2e 6e61 6d65 2172 7d20 636f 6e74  ell.name!r} cont
+0000f860: 6169 6e73 207b 6c65 6e28 6e6f 5f6e 616d  ains {len(no_nam
+0000f870: 655f 6365 6c6c 7329 7d20 556e 6e61 6d65  e_cells)} Unname
+0000f880: 6420 6365 6c6c 7322 0a20 2020 2020 2020  d cells".       
+0000f890: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
+0000f8a0: 2320 666f 7220 6365 6c6c 2069 6e20 616c  # for cell in al
+0000f8b0: 6c5f 6365 6c6c 733a 0a20 2020 2020 2020  l_cells:.       
+0000f8c0: 2023 2020 2020 2070 7269 6e74 2863 656c   #     print(cel
+0000f8d0: 6c2e 6e61 6d65 2c20 7479 7065 2863 656c  l.name, type(cel
+0000f8e0: 6c29 290a 0a20 2020 2020 2020 206c 6962  l))..        lib
+0000f8f0: 203d 2067 6473 746b 2e4c 6962 7261 7279   = gdstk.Library
+0000f900: 280a 2020 2020 2020 2020 2020 2020 756e  (.            un
+0000f910: 6974 3d77 7269 7465 5f73 6574 7469 6e67  it=write_setting
+0000f920: 732e 756e 6974 2c20 7072 6563 6973 696f  s.unit, precisio
+0000f930: 6e3d 7772 6974 655f 7365 7474 696e 6773  n=write_settings
+0000f940: 2e70 7265 6369 7369 6f6e 0a20 2020 2020  .precision.     
+0000f950: 2020 2029 0a20 2020 2020 2020 206c 6962     ).        lib
+0000f960: 2e61 6464 2874 6f70 5f63 656c 6c2e 5f63  .add(top_cell._c
+0000f970: 656c 6c29 0a20 2020 2020 2020 206c 6962  ell).        lib
+0000f980: 2e61 6464 282a 746f 705f 6365 6c6c 2e5f  .add(*top_cell._
+0000f990: 6365 6c6c 2e64 6570 656e 6465 6e63 6965  cell.dependencie
+0000f9a0: 7328 5472 7565 2929 0a0a 2020 2020 2020  s(True))..      
+0000f9b0: 2020 6966 2077 6974 685f 6f61 7369 733a    if with_oasis:
+0000f9c0: 0a20 2020 2020 2020 2020 2020 206c 6962  .            lib
+0000f9d0: 2e77 7269 7465 5f6f 6173 2867 6473 7061  .write_oas(gdspa
+0000f9e0: 7468 2c20 2a2a 6f61 7369 735f 7365 7474  th, **oasis_sett
+0000f9f0: 696e 6773 2e64 6963 7428 2929 0a20 2020  ings.dict()).   
+0000fa00: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+0000fa10: 2020 2020 2020 206c 6962 2e77 7269 7465         lib.write
+0000fa20: 5f67 6473 280a 2020 2020 2020 2020 2020  _gds(.          
+0000fa30: 2020 2020 2020 6764 7370 6174 682c 2074        gdspath, t
+0000fa40: 696d 6573 7461 6d70 3d74 696d 6573 7461  imestamp=timesta
+0000fa50: 6d70 2c20 6d61 785f 706f 696e 7473 3d77  mp, max_points=w
+0000fa60: 7269 7465 5f73 6574 7469 6e67 732e 6d61  rite_settings.ma
+0000fa70: 785f 706f 696e 7473 0a20 2020 2020 2020  x_points.       
+0000fa80: 2020 2020 2029 0a20 2020 2020 2020 2069       ).        i
+0000fa90: 6620 6c6f 6767 696e 673a 0a20 2020 2020  f logging:.     
+0000faa0: 2020 2020 2020 206c 6f67 6765 722e 696e         logger.in
+0000fab0: 666f 2866 2257 726f 7465 2074 6f20 7b73  fo(f"Wrote to {s
+0000fac0: 7472 2867 6473 7061 7468 2921 727d 2229  tr(gdspath)!r}")
+0000fad0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0000fae0: 6764 7370 6174 680a 0a20 2020 2064 6566  gdspath..    def
+0000faf0: 2077 7269 7465 5f67 6473 280a 2020 2020   write_gds(.    
+0000fb00: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
+0000fb10: 2020 6764 7370 6174 683a 204f 7074 696f    gdspath: Optio
+0000fb20: 6e61 6c5b 5061 7468 5479 7065 5d20 3d20  nal[PathType] = 
+0000fb30: 4e6f 6e65 2c0a 2020 2020 2020 2020 6764  None,.        gd
+0000fb40: 7364 6972 3a20 4f70 7469 6f6e 616c 5b50  sdir: Optional[P
+0000fb50: 6174 6854 7970 655d 203d 204e 6f6e 652c  athType] = None,
+0000fb60: 0a20 2020 2020 2020 202a 2a6b 7761 7267  .        **kwarg
+0000fb70: 732c 0a20 2020 2029 202d 3e20 5061 7468  s,.    ) -> Path
+0000fb80: 3a0a 2020 2020 2020 2020 2222 2257 7269  :.        """Wri
+0000fb90: 7465 2063 6f6d 706f 6e65 6e74 2074 6f20  te component to 
+0000fba0: 4744 5320 616e 6420 7265 7475 726e 7320  GDS and returns 
+0000fbb0: 6764 7370 6174 682e 0a0a 2020 2020 2020  gdspath...      
+0000fbc0: 2020 4172 6773 3a0a 2020 2020 2020 2020    Args:.        
+0000fbd0: 2020 2020 6764 7370 6174 683a 2047 4453      gdspath: GDS
+0000fbe0: 2066 696c 6520 7061 7468 2074 6f20 7772   file path to wr
+0000fbf0: 6974 6520 746f 2e0a 2020 2020 2020 2020  ite to..        
+0000fc00: 2020 2020 6764 7364 6972 3a20 6469 7265      gdsdir: dire
+0000fc10: 6374 6f72 7920 666f 7220 7468 6520 4744  ctory for the GD
+0000fc20: 5320 6669 6c65 2e20 4465 6661 756c 7473  S file. Defaults
+0000fc30: 2074 6f20 2f74 6d70 2f72 616e 646f 6d46   to /tmp/randomF
+0000fc40: 696c 652f 6764 7366 6163 746f 7279 2e0a  ile/gdsfactory..
+0000fc50: 0a20 2020 2020 2020 204b 6579 776f 7264  .        Keyword
+0000fc60: 2041 7267 733a 0a20 2020 2020 2020 2020   Args:.         
+0000fc70: 2020 2075 6e69 743a 2075 6e69 7420 7369     unit: unit si
+0000fc80: 7a65 2066 6f72 206f 626a 6563 7473 2069  ze for objects i
+0000fc90: 6e20 6c69 6272 6172 792e 2031 756d 2062  n library. 1um b
+0000fca0: 7920 6465 6661 756c 742e 0a20 2020 2020  y default..     
+0000fcb0: 2020 2020 2020 2070 7265 6369 7369 6f6e         precision
+0000fcc0: 3a20 666f 7220 6469 6d65 6e73 696f 6e73  : for dimensions
+0000fcd0: 2069 6e20 7468 6520 6c69 6272 6172 7920   in the library 
+0000fce0: 286d 292e 2031 6e6d 2062 7920 6465 6661  (m). 1nm by defa
+0000fcf0: 756c 742e 0a20 2020 2020 2020 2020 2020  ult..           
+0000fd00: 206c 6f67 6769 6e67 3a20 6469 7361 626c   logging: disabl
+0000fd10: 6520 4744 5320 7061 7468 206c 6f67 6769  e GDS path loggi
+0000fd20: 6e67 2c20 666f 7220 6578 616d 706c 6520  ng, for example 
+0000fd30: 666f 7220 7368 6f77 696e 6720 6974 2069  for showing it i
+0000fd40: 6e20 4b4c 6179 6f75 742e 0a20 2020 2020  n KLayout..     
+0000fd50: 2020 2020 2020 206f 6e5f 6475 706c 6963         on_duplic
+0000fd60: 6174 655f 6365 6c6c 3a20 7370 6563 6966  ate_cell: specif
+0000fd70: 7920 686f 7720 746f 2072 6573 6f6c 7665  y how to resolve
+0000fd80: 2064 7570 6c69 6361 7465 2d6e 616d 6564   duplicate-named
+0000fd90: 2063 656c 6c73 2e20 4368 6f6f 7365 206f   cells. Choose o
+0000fda0: 6e65 206f 6620 7468 6520 666f 6c6c 6f77  ne of the follow
+0000fdb0: 696e 673a 0a20 2020 2020 2020 2020 2020  ing:.           
+0000fdc0: 2020 2020 2022 7761 726e 2220 2864 6566       "warn" (def
+0000fdd0: 6175 6c74 293a 206f 7665 7277 7269 7465  ault): overwrite
+0000fde0: 2061 6c6c 2064 7570 6c69 6361 7465 2063   all duplicate c
+0000fdf0: 656c 6c73 2077 6974 6820 6f6e 6520 6f66  ells with one of
+0000fe00: 2074 6865 2064 7570 6c69 6361 7465 7320   the duplicates 
+0000fe10: 2861 7262 6974 7261 7269 6c79 292e 0a20  (arbitrarily).. 
+0000fe20: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+0000fe30: 6572 726f 7222 3a20 7468 726f 7720 6120  error": throw a 
+0000fe40: 5661 6c75 6545 7272 6f72 2077 6865 6e20  ValueError when 
+0000fe50: 6174 7465 6d70 7469 6e67 2074 6f20 7772  attempting to wr
+0000fe60: 6974 6520 6120 6764 7320 7769 7468 2064  ite a gds with d
+0000fe70: 7570 6c69 6361 7465 2063 656c 6c73 2e0a  uplicate cells..
+0000fe80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fe90: 226f 7665 7277 7269 7465 223a 206f 7665  "overwrite": ove
+0000fea0: 7277 7269 7465 2061 6c6c 2064 7570 6c69  rwrite all dupli
+0000feb0: 6361 7465 2063 656c 6c73 2077 6974 6820  cate cells with 
+0000fec0: 6f6e 6520 6f66 2074 6865 2064 7570 6c69  one of the dupli
+0000fed0: 6361 7465 732c 2077 6974 686f 7574 2077  cates, without w
+0000fee0: 6172 6e69 6e67 2e0a 2020 2020 2020 2020  arning..        
+0000fef0: 2020 2020 6f6e 5f75 6e63 6163 6865 645f      on_uncached_
+0000ff00: 636f 6d70 6f6e 656e 743a 204c 6974 6572  component: Liter
+0000ff10: 616c 5b22 7761 726e 222c 2022 6572 726f  al["warn", "erro
+0000ff20: 7222 5d20 3d20 2277 6172 6e22 0a20 2020  r"] = "warn".   
+0000ff30: 2020 2020 2020 2020 2066 6c61 7474 656e           flatten
+0000ff40: 5f69 6e76 616c 6964 5f72 6566 733a 2066  _invalid_refs: f
+0000ff50: 6c61 7474 656e 7320 636f 6d70 6f6e 656e  lattens componen
+0000ff60: 7420 7265 6665 7265 6e63 6573 2077 6869  t references whi
+0000ff70: 6368 2068 6176 6520 696e 7661 6c69 6420  ch have invalid 
+0000ff80: 7472 616e 7366 6f72 6d61 7469 6f6e 732e  transformations.
+0000ff90: 0a20 2020 2020 2020 2020 2020 206d 6178  .            max
+0000ffa0: 5f70 6f69 6e74 733a 204d 6178 696d 616c  _points: Maximal
+0000ffb0: 206e 756d 6265 7220 6f66 2076 6572 7469   number of verti
+0000ffc0: 6365 7320 7065 7220 706f 6c79 676f 6e2e  ces per polygon.
+0000ffd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000ffe0: 2050 6f6c 7967 6f6e 7320 7769 7468 206d   Polygons with m
+0000fff0: 6f72 6520 7665 7274 6963 6573 2074 6861  ore vertices tha
+00010000: 7420 7468 6973 2061 7265 2061 7574 6f6d  t this are autom
+00010010: 6174 6963 616c 6c79 2066 7261 6374 7572  atically fractur
+00010020: 6564 2e0a 2020 2020 2020 2020 2222 220a  ed..        """.
+00010030: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00010040: 7365 6c66 2e5f 7772 6974 655f 6c69 6272  self._write_libr
+00010050: 6172 7928 0a20 2020 2020 2020 2020 2020  ary(.           
+00010060: 2067 6473 7061 7468 3d67 6473 7061 7468   gdspath=gdspath
+00010070: 2c20 6764 7364 6972 3d67 6473 6469 722c  , gdsdir=gdsdir,
+00010080: 2077 6974 685f 6f61 7369 733d 4661 6c73   with_oasis=Fals
+00010090: 652c 202a 2a6b 7761 7267 730a 2020 2020  e, **kwargs.    
+000100a0: 2020 2020 290a 0a20 2020 2064 6566 2077      )..    def w
+000100b0: 7269 7465 5f6f 6173 280a 2020 2020 2020  rite_oas(.      
+000100c0: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
+000100d0: 6764 7370 6174 683a 204f 7074 696f 6e61  gdspath: Optiona
+000100e0: 6c5b 5061 7468 5479 7065 5d20 3d20 4e6f  l[PathType] = No
+000100f0: 6e65 2c0a 2020 2020 2020 2020 6764 7364  ne,.        gdsd
+00010100: 6972 3a20 4f70 7469 6f6e 616c 5b50 6174  ir: Optional[Pat
+00010110: 6854 7970 655d 203d 204e 6f6e 652c 0a20  hType] = None,. 
+00010120: 2020 2020 2020 202a 2a6b 7761 7267 732c         **kwargs,
+00010130: 0a20 2020 2029 202d 3e20 5061 7468 3a0a  .    ) -> Path:.
+00010140: 2020 2020 2020 2020 2222 2257 7269 7465          """Write
+00010150: 2063 6f6d 706f 6e65 6e74 2074 6f20 4744   component to GD
+00010160: 5320 616e 6420 7265 7475 726e 7320 6764  S and returns gd
+00010170: 7370 6174 682e 0a0a 2020 2020 2020 2020  spath...        
+00010180: 4172 6773 3a0a 2020 2020 2020 2020 2020  Args:.          
+00010190: 2020 6764 7370 6174 683a 2047 4453 2066    gdspath: GDS f
+000101a0: 696c 6520 7061 7468 2074 6f20 7772 6974  ile path to writ
+000101b0: 6520 746f 2e0a 2020 2020 2020 2020 2020  e to..          
+000101c0: 2020 6764 7364 6972 3a20 6469 7265 6374    gdsdir: direct
+000101d0: 6f72 7920 666f 7220 7468 6520 4744 5320  ory for the GDS 
+000101e0: 6669 6c65 2e20 4465 6661 756c 7473 2074  file. Defaults t
+000101f0: 6f20 2f74 6d70 2f72 616e 646f 6d46 696c  o /tmp/randomFil
+00010200: 652f 6764 7366 6163 746f 7279 2e0a 0a20  e/gdsfactory... 
+00010210: 2020 2020 2020 204b 6579 776f 7264 2041         Keyword A
+00010220: 7267 733a 0a20 2020 2020 2020 2020 2020  rgs:.           
+00010230: 2075 6e69 743a 2075 6e69 7420 7369 7a65   unit: unit size
+00010240: 2066 6f72 206f 626a 6563 7473 2069 6e20   for objects in 
+00010250: 6c69 6272 6172 792e 2031 756d 2062 7920  library. 1um by 
+00010260: 6465 6661 756c 742e 0a20 2020 2020 2020  default..       
+00010270: 2020 2020 2070 7265 6369 7369 6f6e 3a20       precision: 
+00010280: 666f 7220 6469 6d65 6e73 696f 6e73 2069  for dimensions i
+00010290: 6e20 7468 6520 6c69 6272 6172 7920 286d  n the library (m
+000102a0: 292e 2031 6e6d 2062 7920 6465 6661 756c  ). 1nm by defaul
+000102b0: 742e 0a20 2020 2020 2020 2020 2020 206c  t..            l
+000102c0: 6f67 6769 6e67 3a20 6469 7361 626c 6520  ogging: disable 
+000102d0: 4744 5320 7061 7468 206c 6f67 6769 6e67  GDS path logging
+000102e0: 2c20 666f 7220 6578 616d 706c 6520 666f  , for example fo
+000102f0: 7220 7368 6f77 696e 6720 6974 2069 6e20  r showing it in 
+00010300: 4b4c 6179 6f75 742e 0a20 2020 2020 2020  KLayout..       
+00010310: 2020 2020 206f 6e5f 6475 706c 6963 6174       on_duplicat
+00010320: 655f 6365 6c6c 3a20 7370 6563 6966 7920  e_cell: specify 
+00010330: 686f 7720 746f 2072 6573 6f6c 7665 2064  how to resolve d
+00010340: 7570 6c69 6361 7465 2d6e 616d 6564 2063  uplicate-named c
+00010350: 656c 6c73 2e20 4368 6f6f 7365 206f 6e65  ells. Choose one
+00010360: 206f 6620 7468 6520 666f 6c6c 6f77 696e   of the followin
+00010370: 673a 0a20 2020 2020 2020 2020 2020 2020  g:.             
+00010380: 2020 2022 7761 726e 2220 2864 6566 6175     "warn" (defau
+00010390: 6c74 293a 206f 7665 7277 7269 7465 2061  lt): overwrite a
+000103a0: 6c6c 2064 7570 6c69 6361 7465 2063 656c  ll duplicate cel
+000103b0: 6c73 2077 6974 6820 6f6e 6520 6f66 2074  ls with one of t
+000103c0: 6865 2064 7570 6c69 6361 7465 7320 2861  he duplicates (a
+000103d0: 7262 6974 7261 7269 6c79 292e 0a20 2020  rbitrarily)..   
+000103e0: 2020 2020 2020 2020 2020 2020 2022 6572               "er
+000103f0: 726f 7222 3a20 7468 726f 7720 6120 5661  ror": throw a Va
+00010400: 6c75 6545 7272 6f72 2077 6865 6e20 6174  lueError when at
+00010410: 7465 6d70 7469 6e67 2074 6f20 7772 6974  tempting to writ
+00010420: 6520 6120 6764 7320 7769 7468 2064 7570  e a gds with dup
+00010430: 6c69 6361 7465 2063 656c 6c73 2e0a 2020  licate cells..  
+00010440: 2020 2020 2020 2020 2020 2020 2020 226f                "o
+00010450: 7665 7277 7269 7465 223a 206f 7665 7277  verwrite": overw
+00010460: 7269 7465 2061 6c6c 2064 7570 6c69 6361  rite all duplica
+00010470: 7465 2063 656c 6c73 2077 6974 6820 6f6e  te cells with on
+00010480: 6520 6f66 2074 6865 2064 7570 6c69 6361  e of the duplica
+00010490: 7465 732c 2077 6974 686f 7574 2077 6172  tes, without war
+000104a0: 6e69 6e67 2e0a 2020 2020 2020 2020 2020  ning..          
+000104b0: 2020 2020 2020 4e6f 6e65 3a20 646f 206e        None: do n
+000104c0: 6f74 2074 7279 2074 6f20 7265 736f 6c76  ot try to resolv
+000104d0: 6520 2861 7420 796f 7572 206f 776e 2072  e (at your own r
+000104e0: 6973 6b21 290a 2020 2020 2020 2020 2020  isk!).          
+000104f0: 2020 6f6e 5f75 6e63 6163 6865 645f 636f    on_uncached_co
+00010500: 6d70 6f6e 656e 743a 204c 6974 6572 616c  mponent: Literal
+00010510: 5b22 7761 726e 222c 2022 6572 726f 7222  ["warn", "error"
+00010520: 5d20 3d20 2277 6172 6e22 0a20 2020 2020  ] = "warn".     
+00010530: 2020 2020 2020 2066 6c61 7474 656e 5f69         flatten_i
+00010540: 6e76 616c 6964 5f72 6566 733a 2066 6c61  nvalid_refs: fla
+00010550: 7474 656e 7320 636f 6d70 6f6e 656e 7420  ttens component 
+00010560: 7265 6665 7265 6e63 6573 2077 6869 6368  references which
+00010570: 2068 6176 6520 696e 7661 6c69 6420 7472   have invalid tr
+00010580: 616e 7366 6f72 6d61 7469 6f6e 732e 0a20  ansformations.. 
+00010590: 2020 2020 2020 2020 2020 2063 6f6d 7072             compr
+000105a0: 6573 7369 6f6e 5f6c 6576 656c 3a20 4c65  ession_level: Le
+000105b0: 7665 6c20 6f66 2063 6f6d 7072 6573 7369  vel of compressi
+000105c0: 6f6e 2066 6f72 2063 656c 6c73 2028 6265  on for cells (be
+000105d0: 7477 6565 6e20 3020 616e 6420 3929 2e0a  tween 0 and 9)..
+000105e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000105f0: 5365 7474 696e 6720 746f 2030 2077 696c  Setting to 0 wil
+00010600: 6c20 6469 7361 626c 6520 6365 6c6c 2063  l disable cell c
+00010610: 6f6d 7072 6573 7369 6f6e 2c20 3120 6769  ompression, 1 gi
+00010620: 7665 7320 7468 6520 6265 7374 2073 7065  ves the best spe
+00010630: 6564 2061 6e64 2039 2c20 7468 6520 6265  ed and 9, the be
+00010640: 7374 2063 6f6d 7072 6573 7369 6f6e 2e0a  st compression..
+00010650: 2020 2020 2020 2020 2020 2020 6465 7465              dete
+00010660: 6374 5f72 6563 7461 6e67 6c65 733a 2053  ct_rectangles: S
+00010670: 746f 7265 2072 6563 7461 6e67 6c65 7320  tore rectangles 
+00010680: 696e 2063 6f6d 7072 6573 7365 6420 666f  in compressed fo
+00010690: 726d 6174 2e0a 2020 2020 2020 2020 2020  rmat..          
+000106a0: 2020 6465 7465 6374 5f74 7261 7065 7a6f    detect_trapezo
+000106b0: 6964 733a 2053 746f 7265 2074 7261 7065  ids: Store trape
+000106c0: 7a6f 6964 7320 696e 2063 6f6d 7072 6573  zoids in compres
+000106d0: 7365 6420 666f 726d 6174 2e0a 2020 2020  sed format..    
+000106e0: 2020 2020 2020 2020 6369 7263 6c65 5f74          circle_t
+000106f0: 6f6c 6572 616e 6365 3a20 546f 6c65 7261  olerance: Tolera
+00010700: 6e63 6520 666f 7220 6465 7465 6374 696e  nce for detectin
+00010710: 6720 6369 7263 6c65 732e 2049 6620 6c65  g circles. If le
+00010720: 7373 206f 7220 6571 7561 6c20 746f 2030  ss or equal to 0
+00010730: 2c20 6e6f 2064 6574 6563 7469 6f6e 2069  , no detection i
+00010740: 7320 7065 7266 6f72 6d65 642e 0a20 2020  s performed..   
+00010750: 2020 2020 2020 2020 2020 2020 2043 6972               Cir
+00010760: 636c 6573 2061 7265 2073 746f 7265 6420  cles are stored 
+00010770: 696e 2063 6f6d 7072 6573 7365 6420 666f  in compressed fo
+00010780: 726d 6174 2e0a 2020 2020 2020 2020 2020  rmat..          
+00010790: 2020 7661 6c69 6461 7469 6f6e 2028 2263    validation ("c
+000107a0: 7263 3332 222c 2022 6368 6563 6b73 756d  rc32", "checksum
+000107b0: 3332 222c 204e 6f6e 6529 20e2 8093 2074  32", None) ... t
+000107c0: 7970 6520 6f66 2076 616c 6964 6174 696f  ype of validatio
+000107d0: 6e20 746f 2069 6e63 6c75 6465 2069 6e20  n to include in 
+000107e0: 7468 6520 7361 7665 6420 6669 6c65 2e0a  the saved file..
+000107f0: 2020 2020 2020 2020 2020 2020 7374 616e              stan
+00010800: 6461 7264 5f70 726f 7065 7274 6965 733a  dard_properties:
+00010810: 2053 746f 7265 2073 7461 6e64 6172 6420   Store standard 
+00010820: 4f41 5349 5320 7072 6f70 6572 7469 6573  OASIS properties
+00010830: 2069 6e20 7468 6520 6669 6c65 2e0a 2020   in the file..  
+00010840: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00010850: 2020 7265 7475 726e 2073 656c 662e 5f77    return self._w
+00010860: 7269 7465 5f6c 6962 7261 7279 280a 2020  rite_library(.  
+00010870: 2020 2020 2020 2020 2020 6764 7370 6174            gdspat
+00010880: 683d 6764 7370 6174 682c 0a20 2020 2020  h=gdspath,.     
+00010890: 2020 2020 2020 2067 6473 6469 723d 6764         gdsdir=gd
+000108a0: 7364 6972 2c0a 2020 2020 2020 2020 2020  sdir,.          
+000108b0: 2020 7769 7468 5f6f 6173 6973 3d54 7275    with_oasis=Tru
+000108c0: 652c 0a20 2020 2020 2020 2020 2020 202a  e,.            *
+000108d0: 2a6b 7761 7267 732c 0a20 2020 2020 2020  *kwargs,.       
+000108e0: 2029 0a0a 2020 2020 6465 6620 7772 6974   )..    def writ
+000108f0: 655f 6764 735f 7769 7468 5f6d 6574 6164  e_gds_with_metad
+00010900: 6174 6128 7365 6c66 2c20 2a61 7267 732c  ata(self, *args,
+00010910: 202a 2a6b 7761 7267 7329 202d 3e20 5061   **kwargs) -> Pa
+00010920: 7468 3a0a 2020 2020 2020 2020 2222 2257  th:.        """W
+00010930: 7269 7465 2063 6f6d 706f 6e65 6e74 2069  rite component i
+00010940: 6e20 4744 5320 616e 6420 6d65 7461 6461  n GDS and metada
+00010950: 7461 2028 636f 6d70 6f6e 656e 7420 7365  ta (component se
+00010960: 7474 696e 6773 2920 696e 2059 414d 4c2e  ttings) in YAML.
+00010970: 2222 220a 2020 2020 2020 2020 6764 7370  """.        gdsp
+00010980: 6174 6820 3d20 7365 6c66 2e77 7269 7465  ath = self.write
+00010990: 5f67 6473 282a 6172 6773 2c20 2a2a 6b77  _gds(*args, **kw
+000109a0: 6172 6773 290a 2020 2020 2020 2020 6d65  args).        me
+000109b0: 7461 6461 7461 203d 2067 6473 7061 7468  tadata = gdspath
+000109c0: 2e77 6974 685f 7375 6666 6978 2822 2e79  .with_suffix(".y
+000109d0: 6d6c 2229 0a20 2020 2020 2020 206d 6574  ml").        met
+000109e0: 6164 6174 612e 7772 6974 655f 7465 7874  adata.write_text
+000109f0: 2873 656c 662e 746f 5f79 616d 6c28 7769  (self.to_yaml(wi
+00010a00: 7468 5f63 656c 6c73 3d54 7275 652c 2077  th_cells=True, w
+00010a10: 6974 685f 706f 7274 733d 5472 7565 2929  ith_ports=True))
+00010a20: 0a20 2020 2020 2020 206c 6f67 6765 722e  .        logger.
+00010a30: 696e 666f 2866 2257 7269 7465 2059 414d  info(f"Write YAM
+00010a40: 4c20 6d65 7461 6461 7461 2074 6f20 7b73  L metadata to {s
+00010a50: 7472 286d 6574 6164 6174 6129 2172 7d22  tr(metadata)!r}"
+00010a60: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+00010a70: 2067 6473 7061 7468 0a0a 2020 2020 6465   gdspath..    de
+00010a80: 6620 746f 5f64 6963 7428 0a20 2020 2020  f to_dict(.     
+00010a90: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
+00010aa0: 2069 676e 6f72 655f 636f 6d70 6f6e 656e   ignore_componen
+00010ab0: 7473 5f70 7265 6669 783a 204f 7074 696f  ts_prefix: Optio
+00010ac0: 6e61 6c5b 4c69 7374 5b73 7472 5d5d 203d  nal[List[str]] =
+00010ad0: 204e 6f6e 652c 0a20 2020 2020 2020 2069   None,.        i
+00010ae0: 676e 6f72 655f 6675 6e63 7469 6f6e 735f  gnore_functions_
+00010af0: 7072 6566 6978 3a20 4f70 7469 6f6e 616c  prefix: Optional
+00010b00: 5b4c 6973 745b 7374 725d 5d20 3d20 4e6f  [List[str]] = No
+00010b10: 6e65 2c0a 2020 2020 2020 2020 7769 7468  ne,.        with
+00010b20: 5f63 656c 6c73 3a20 626f 6f6c 203d 2046  _cells: bool = F
+00010b30: 616c 7365 2c0a 2020 2020 2020 2020 7769  alse,.        wi
+00010b40: 7468 5f70 6f72 7473 3a20 626f 6f6c 203d  th_ports: bool =
+00010b50: 2054 7275 652c 0a20 2020 2029 202d 3e20   True,.    ) -> 
+00010b60: 4469 6374 5b73 7472 2c20 416e 795d 3a0a  Dict[str, Any]:.
+00010b70: 2020 2020 2020 2020 2222 2252 6574 7572          """Retur
+00010b80: 6e73 2044 6963 7420 7265 7072 6573 656e  ns Dict represen
+00010b90: 7461 7469 6f6e 206f 6620 6120 636f 6d70  tation of a comp
+00010ba0: 6f6e 656e 742e 0a0a 2020 2020 2020 2020  onent...        
+00010bb0: 4172 6773 3a0a 2020 2020 2020 2020 2020  Args:.          
+00010bc0: 2020 6967 6e6f 7265 5f63 6f6d 706f 6e65    ignore_compone
+00010bd0: 6e74 735f 7072 6566 6978 3a20 666f 7220  nts_prefix: for 
+00010be0: 636f 6d70 6f6e 656e 7473 2074 6f20 6967  components to ig
+00010bf0: 6e6f 7265 2077 6865 6e20 6578 706f 7274  nore when export
+00010c00: 696e 672e 0a20 2020 2020 2020 2020 2020  ing..           
+00010c10: 2069 676e 6f72 655f 6675 6e63 7469 6f6e   ignore_function
+00010c20: 735f 7072 6566 6978 3a20 666f 7220 6675  s_prefix: for fu
+00010c30: 6e63 7469 6f6e 7320 746f 2069 676e 6f72  nctions to ignor
+00010c40: 6520 7768 656e 2065 7870 6f72 7469 6e67  e when exporting
+00010c50: 2e0a 2020 2020 2020 2020 2020 2020 7769  ..            wi
+00010c60: 7468 5f63 656c 6c73 3a20 7772 6974 6520  th_cells: write 
+00010c70: 6365 6c6c 7320 7265 6375 7273 6976 656c  cells recursivel
+00010c80: 792e 0a20 2020 2020 2020 2020 2020 2077  y..            w
+00010c90: 6974 685f 706f 7274 733a 2077 7269 7465  ith_ports: write
+00010ca0: 2070 6f72 7420 696e 666f 726d 6174 696f   port informatio
+00010cb0: 6e20 6469 6374 2e0a 2020 2020 2020 2020  n dict..        
+00010cc0: 2222 220a 2020 2020 2020 2020 6420 3d20  """.        d = 
+00010cd0: 7b7d 0a20 2020 2020 2020 2069 6620 7769  {}.        if wi
+00010ce0: 7468 5f70 6f72 7473 3a0a 2020 2020 2020  th_ports:.      
+00010cf0: 2020 2020 2020 706f 7274 7320 3d20 7b70        ports = {p
+00010d00: 6f72 742e 6e61 6d65 3a20 706f 7274 2e74  ort.name: port.t
+00010d10: 6f5f 6469 6374 2829 2066 6f72 2070 6f72  o_dict() for por
+00010d20: 7420 696e 2073 656c 662e 6765 745f 706f  t in self.get_po
+00010d30: 7274 735f 6c69 7374 2829 7d0a 2020 2020  rts_list()}.    
+00010d40: 2020 2020 2020 2020 645b 2270 6f72 7473          d["ports
+00010d50: 225d 203d 2070 6f72 7473 0a0a 2020 2020  "] = ports..    
+00010d60: 2020 2020 6966 2077 6974 685f 6365 6c6c      if with_cell
+00010d70: 733a 0a20 2020 2020 2020 2020 2020 2063  s:.            c
+00010d80: 656c 6c73 203d 2072 6563 7572 7365 5f73  ells = recurse_s
+00010d90: 7472 7563 7475 7265 7328 0a20 2020 2020  tructures(.     
+00010da0: 2020 2020 2020 2020 2020 2073 656c 662c             self,
+00010db0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010dc0: 2069 676e 6f72 655f 6675 6e63 7469 6f6e   ignore_function
+00010dd0: 735f 7072 6566 6978 3d69 676e 6f72 655f  s_prefix=ignore_
+00010de0: 6675 6e63 7469 6f6e 735f 7072 6566 6978  functions_prefix
+00010df0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00010e00: 2020 6967 6e6f 7265 5f63 6f6d 706f 6e65    ignore_compone
+00010e10: 6e74 735f 7072 6566 6978 3d69 676e 6f72  nts_prefix=ignor
+00010e20: 655f 636f 6d70 6f6e 656e 7473 5f70 7265  e_components_pre
+00010e30: 6669 782c 0a20 2020 2020 2020 2020 2020  fix,.           
+00010e40: 2029 0a20 2020 2020 2020 2020 2020 2064   ).            d
+00010e50: 5b22 6365 6c6c 7322 5d20 3d20 636c 6561  ["cells"] = clea
+00010e60: 6e5f 6469 6374 2863 656c 6c73 290a 0a20  n_dict(cells).. 
+00010e70: 2020 2020 2020 2064 5b22 6e61 6d65 225d         d["name"]
+00010e80: 203d 2073 656c 662e 6e61 6d65 0a20 2020   = self.name.   
+00010e90: 2020 2020 2064 5b22 7365 7474 696e 6773       d["settings
+00010ea0: 225d 203d 2063 6c65 616e 5f64 6963 7428  "] = clean_dict(
+00010eb0: 6469 6374 2873 656c 662e 7365 7474 696e  dict(self.settin
+00010ec0: 6773 2929 0a20 2020 2020 2020 2072 6574  gs)).        ret
+00010ed0: 7572 6e20 640a 0a20 2020 2064 6566 2074  urn d..    def t
+00010ee0: 6f5f 7961 6d6c 2873 656c 662c 202a 2a6b  o_yaml(self, **k
+00010ef0: 7761 7267 7329 202d 3e20 7374 723a 0a20  wargs) -> str:. 
+00010f00: 2020 2020 2020 2022 2222 5772 6974 6520         """Write 
+00010f10: 4469 6374 2072 6570 7265 7365 6e74 6174  Dict representat
+00010f20: 696f 6e20 6f66 2061 2063 6f6d 706f 6e65  ion of a compone
+00010f30: 6e74 2069 6e20 5941 4d4c 2066 6f72 6d61  nt in YAML forma
+00010f40: 742e 0a0a 2020 2020 2020 2020 4172 6773  t...        Args
+00010f50: 3a0a 2020 2020 2020 2020 2020 2020 6967  :.            ig
+00010f60: 6e6f 7265 5f63 6f6d 706f 6e65 6e74 735f  nore_components_
+00010f70: 7072 6566 6978 3a20 666f 7220 636f 6d70  prefix: for comp
+00010f80: 6f6e 656e 7473 2074 6f20 6967 6e6f 7265  onents to ignore
+00010f90: 2077 6865 6e20 6578 706f 7274 696e 672e   when exporting.
+00010fa0: 0a20 2020 2020 2020 2020 2020 2069 676e  .            ign
+00010fb0: 6f72 655f 6675 6e63 7469 6f6e 735f 7072  ore_functions_pr
+00010fc0: 6566 6978 3a20 666f 7220 6675 6e63 7469  efix: for functi
+00010fd0: 6f6e 7320 746f 2069 676e 6f72 6520 7768  ons to ignore wh
+00010fe0: 656e 2065 7870 6f72 7469 6e67 2e0a 2020  en exporting..  
+00010ff0: 2020 2020 2020 2020 2020 7769 7468 5f63            with_c
+00011000: 656c 6c73 3a20 7772 6974 6520 6365 6c6c  ells: write cell
+00011010: 7320 7265 6375 7273 6976 656c 792e 0a20  s recursively.. 
+00011020: 2020 2020 2020 2020 2020 2077 6974 685f             with_
+00011030: 706f 7274 733a 2077 7269 7465 2070 6f72  ports: write por
+00011040: 7420 696e 666f 726d 6174 696f 6e2e 0a20  t information.. 
+00011050: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00011060: 2020 2072 6574 7572 6e20 4f6d 6567 6143     return OmegaC
+00011070: 6f6e 662e 746f 5f79 616d 6c28 636c 6561  onf.to_yaml(clea
+00011080: 6e5f 6469 6374 2873 656c 662e 746f 5f64  n_dict(self.to_d
+00011090: 6963 7428 2a2a 6b77 6172 6773 2929 290a  ict(**kwargs))).
+000110a0: 0a20 2020 2064 6566 2074 6f5f 6469 6374  .    def to_dict
+000110b0: 5f70 6f6c 7967 6f6e 7328 7365 6c66 2920  _polygons(self) 
+000110c0: 2d3e 2044 6963 745b 7374 722c 2041 6e79  -> Dict[str, Any
+000110d0: 5d3a 0a20 2020 2020 2020 2022 2222 5265  ]:.        """Re
+000110e0: 7475 726e 7320 6120 6469 6374 2072 6570  turns a dict rep
+000110f0: 7265 7365 6e74 6174 696f 6e20 6f66 2074  resentation of t
+00011100: 6865 2066 6c61 7474 656e 6564 2063 6f6d  he flattened com
+00011110: 706f 6e65 6e74 2e22 2222 0a20 2020 2020  ponent.""".     
+00011120: 2020 2064 203d 207b 7d0a 2020 2020 2020     d = {}.      
+00011130: 2020 706f 6c79 676f 6e73 203d 207b 7d0a    polygons = {}.
+00011140: 2020 2020 2020 2020 6c61 7965 725f 746f          layer_to
+00011150: 5f70 6f6c 7967 6f6e 7320 3d20 7365 6c66  _polygons = self
+00011160: 2e67 6574 5f70 6f6c 7967 6f6e 7328 6279  .get_polygons(by
+00011170: 5f73 7065 633d 5472 7565 290a 0a20 2020  _spec=True)..   
+00011180: 2020 2020 2066 6f72 206c 6179 6572 2c20       for layer, 
+00011190: 706f 6c79 676f 6e73 5f6c 6179 6572 2069  polygons_layer i
+000111a0: 6e20 6c61 7965 725f 746f 5f70 6f6c 7967  n layer_to_polyg
+000111b0: 6f6e 732e 6974 656d 7328 293a 0a20 2020  ons.items():.   
+000111c0: 2020 2020 2020 2020 206c 6179 6572 5f6e           layer_n
+000111d0: 616d 6520 3d20 6622 7b6c 6179 6572 5b30  ame = f"{layer[0
+000111e0: 5d7d 5f7b 6c61 7965 725b 315d 7d22 0a20  ]}_{layer[1]}". 
+000111f0: 2020 2020 2020 2020 2020 2066 6f72 2070             for p
+00011200: 6f6c 7967 6f6e 2069 6e20 706f 6c79 676f  olygon in polygo
+00011210: 6e73 5f6c 6179 6572 3a0a 2020 2020 2020  ns_layer:.      
+00011220: 2020 2020 2020 2020 2020 706f 6c79 676f            polygo
+00011230: 6e73 5b6c 6179 6572 5f6e 616d 655d 203d  ns[layer_name] =
+00011240: 205b 7475 706c 6528 736e 6170 5f74 6f5f   [tuple(snap_to_
+00011250: 6772 6964 2876 2929 2066 6f72 2076 2069  grid(v)) for v i
+00011260: 6e20 706f 6c79 676f 6e5d 0a0a 2020 2020  n polygon]..    
+00011270: 2020 2020 706f 7274 7320 3d20 7b70 6f72      ports = {por
+00011280: 742e 6e61 6d65 3a20 706f 7274 2e73 6574  t.name: port.set
+00011290: 7469 6e67 7320 666f 7220 706f 7274 2069  tings for port i
+000112a0: 6e20 7365 6c66 2e67 6574 5f70 6f72 7473  n self.get_ports
+000112b0: 5f6c 6973 7428 297d 0a20 2020 2020 2020  _list()}.       
+000112c0: 2063 6c65 616e 5f64 6963 7428 706f 7274   clean_dict(port
+000112d0: 7329 0a20 2020 2020 2020 2063 6c65 616e  s).        clean
+000112e0: 5f64 6963 7428 706f 6c79 676f 6e73 290a  _dict(polygons).
+000112f0: 2020 2020 2020 2020 642e 696e 666f 203d          d.info =
+00011300: 2073 656c 662e 696e 666f 0a20 2020 2020   self.info.     
+00011310: 2020 2064 2e70 6f6c 7967 6f6e 7320 3d20     d.polygons = 
+00011320: 706f 6c79 676f 6e73 0a20 2020 2020 2020  polygons.       
+00011330: 2064 2e70 6f72 7473 203d 2070 6f72 7473   d.ports = ports
+00011340: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00011350: 640a 0a20 2020 2064 6566 2061 7574 6f5f  d..    def auto_
+00011360: 7265 6e61 6d65 5f70 6f72 7473 2873 656c  rename_ports(sel
+00011370: 662c 202a 2a6b 7761 7267 7329 202d 3e20  f, **kwargs) -> 
+00011380: 4e6f 6e65 3a0a 2020 2020 2020 2020 2222  None:.        ""
+00011390: 2252 656e 616d 6520 706f 7274 7320 6279  "Rename ports by
+000113a0: 206f 7269 656e 7461 7469 6f6e 204e 5345   orientation NSE
+000113b0: 5720 286e 6f72 7468 2c20 736f 7574 682c  W (north, south,
+000113c0: 2065 6173 742c 2077 6573 7429 2e0a 0a20   east, west)... 
+000113d0: 2020 2020 2020 204b 6579 776f 7264 2041         Keyword A
+000113e0: 7267 733a 0a20 2020 2020 2020 2020 2020  rgs:.           
+000113f0: 2066 756e 6374 696f 6e3a 2074 6f20 7265   function: to re
+00011400: 6e61 6d65 2070 6f72 7473 2e0a 2020 2020  name ports..    
+00011410: 2020 2020 2020 2020 7365 6c65 6374 5f70          select_p
+00011420: 6f72 7473 5f6f 7074 6963 616c 3a20 746f  orts_optical: to
+00011430: 2073 656c 6563 7420 6f70 7469 6361 6c20   select optical 
+00011440: 706f 7274 732e 0a20 2020 2020 2020 2020  ports..         
+00011450: 2020 2073 656c 6563 745f 706f 7274 735f     select_ports_
+00011460: 656c 6563 7472 6963 616c 3a20 746f 2073  electrical: to s
+00011470: 656c 6563 7420 656c 6563 7472 6963 616c  elect electrical
+00011480: 2070 6f72 7473 2e0a 2020 2020 2020 2020   ports..        
+00011490: 2020 2020 7072 6566 6978 5f6f 7074 6963      prefix_optic
+000114a0: 616c 3a20 7072 6566 6978 2e0a 2020 2020  al: prefix..    
+000114b0: 2020 2020 2020 2020 7072 6566 6978 5f65          prefix_e
+000114c0: 6c65 6374 7269 6361 6c3a 2070 7265 6669  lectrical: prefi
+000114d0: 782e 0a0a 2020 2020 2020 2020 2e2e 2063  x...        .. c
+000114e0: 6f64 653a 3a0a 0a20 2020 2020 2020 2020  ode::..         
+000114f0: 2020 2020 2020 2020 2033 2020 340a 2020           3  4.  
+00011500: 2020 2020 2020 2020 2020 2020 2020 205f                 _
+00011510: 7c5f 5f7c 5f0a 2020 2020 2020 2020 2020  |__|_.          
+00011520: 2020 2032 202d 7c20 2020 2020 207c 2d20     2 -|      |- 
+00011530: 350a 2020 2020 2020 2020 2020 2020 2020  5.              
+00011540: 2020 7c20 2020 2020 207c 0a20 2020 2020    |      |.     
+00011550: 2020 2020 2020 2020 3120 2d7c 5f5f 5f5f          1 -|____
+00011560: 5f5f 7c2d 2036 0a20 2020 2020 2020 2020  __|- 6.         
+00011570: 2020 2020 2020 2020 207c 2020 7c0a 2020           |  |.  
+00011580: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011590: 3820 2037 0a20 2020 2020 2020 2022 2222  8  7.        """
+000115a0: 0a20 2020 2020 2020 2073 656c 662e 6973  .        self.is
+000115b0: 5f75 6e6c 6f63 6b65 6428 290a 2020 2020  _unlocked().    
+000115c0: 2020 2020 6175 746f 5f72 656e 616d 655f      auto_rename_
+000115d0: 706f 7274 7328 7365 6c66 2c20 2a2a 6b77  ports(self, **kw
+000115e0: 6172 6773 290a 0a20 2020 2064 6566 2061  args)..    def a
+000115f0: 7574 6f5f 7265 6e61 6d65 5f70 6f72 7473  uto_rename_ports
+00011600: 5f63 6f75 6e74 6572 5f63 6c6f 636b 7769  _counter_clockwi
+00011610: 7365 2873 656c 662c 202a 2a6b 7761 7267  se(self, **kwarg
+00011620: 7329 202d 3e20 4e6f 6e65 3a0a 2020 2020  s) -> None:.    
+00011630: 2020 2020 7365 6c66 2e69 735f 756e 6c6f      self.is_unlo
+00011640: 636b 6564 2829 0a20 2020 2020 2020 2061  cked().        a
+00011650: 7574 6f5f 7265 6e61 6d65 5f70 6f72 7473  uto_rename_ports
+00011660: 5f63 6f75 6e74 6572 5f63 6c6f 636b 7769  _counter_clockwi
+00011670: 7365 2873 656c 662c 202a 2a6b 7761 7267  se(self, **kwarg
+00011680: 7329 0a0a 2020 2020 6465 6620 6175 746f  s)..    def auto
+00011690: 5f72 656e 616d 655f 706f 7274 735f 6c61  _rename_ports_la
+000116a0: 7965 725f 6f72 6965 6e74 6174 696f 6e28  yer_orientation(
+000116b0: 7365 6c66 2c20 2a2a 6b77 6172 6773 2920  self, **kwargs) 
+000116c0: 2d3e 204e 6f6e 653a 0a20 2020 2020 2020  -> None:.       
+000116d0: 2073 656c 662e 6973 5f75 6e6c 6f63 6b65   self.is_unlocke
+000116e0: 6428 290a 2020 2020 2020 2020 6175 746f  d().        auto
+000116f0: 5f72 656e 616d 655f 706f 7274 735f 6c61  _rename_ports_la
+00011700: 7965 725f 6f72 6965 6e74 6174 696f 6e28  yer_orientation(
+00011710: 7365 6c66 2c20 2a2a 6b77 6172 6773 290a  self, **kwargs).
+00011720: 0a20 2020 2064 6566 2061 7574 6f5f 7265  .    def auto_re
+00011730: 6e61 6d65 5f70 6f72 7473 5f6f 7269 656e  name_ports_orien
+00011740: 7461 7469 6f6e 2873 656c 662c 202a 2a6b  tation(self, **k
+00011750: 7761 7267 7329 202d 3e20 4e6f 6e65 3a0a  wargs) -> None:.
+00011760: 2020 2020 2020 2020 2222 2252 656e 616d          """Renam
+00011770: 6520 706f 7274 7320 6279 206f 7269 656e  e ports by orien
+00011780: 7461 7469 6f6e 204e 5345 5720 286e 6f72  tation NSEW (nor
+00011790: 7468 2c20 736f 7574 682c 2065 6173 742c  th, south, east,
+000117a0: 2077 6573 7429 2e0a 0a20 2020 2020 2020   west)...       
+000117b0: 204b 6579 776f 7264 2041 7267 733a 0a20   Keyword Args:. 
+000117c0: 2020 2020 2020 2020 2020 2066 756e 6374             funct
+000117d0: 696f 6e3a 2074 6f20 7265 6e61 6d65 2070  ion: to rename p
+000117e0: 6f72 7473 2e0a 2020 2020 2020 2020 2020  orts..          
+000117f0: 2020 7365 6c65 6374 5f70 6f72 7473 5f6f    select_ports_o
+00011800: 7074 6963 616c 3a20 746f 2073 656c 6563  ptical: to selec
+00011810: 7420 706f 7274 732e 0a20 2020 2020 2020  t ports..       
+00011820: 2020 2020 2073 656c 6563 745f 706f 7274       select_port
+00011830: 735f 656c 6563 7472 6963 616c 3a0a 2020  s_electrical:.  
+00011840: 2020 2020 2020 2020 2020 7072 6566 6978            prefix
+00011850: 5f6f 7074 6963 616c 3a0a 2020 2020 2020  _optical:.      
+00011860: 2020 2020 2020 7072 6566 6978 5f65 6c65        prefix_ele
+00011870: 6374 7269 6361 6c3a 0a0a 2020 2020 2020  ctrical:..      
+00011880: 2020 2e2e 2063 6f64 653a 3a0a 0a20 2020    .. code::..   
+00011890: 2020 2020 2020 2020 2020 2020 2020 4e30                N0
+000118a0: 2020 4e31 0a20 2020 2020 2020 2020 2020    N1.           
+000118b0: 2020 2020 2020 7c5f 5f5f 7c5f 0a20 2020        |___|_.   
+000118c0: 2020 2020 2020 2020 2057 3120 2d7c 2020           W1 -|  
+000118d0: 2020 2020 7c2d 2045 310a 2020 2020 2020      |- E1.      
+000118e0: 2020 2020 2020 2020 2020 7c20 2020 2020            |     
+000118f0: 207c 0a20 2020 2020 2020 2020 2020 2057   |.            W
+00011900: 3020 2d7c 5f5f 5f5f 5f5f 7c2d 2045 300a  0 -|______|- E0.
+00011910: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011920: 207c 2020 207c 0a20 2020 2020 2020 2020   |   |.         
+00011930: 2020 2020 2020 2053 3020 2020 5331 0a20         S0   S1. 
+00011940: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00011950: 2020 2073 656c 662e 6973 5f75 6e6c 6f63     self.is_unloc
+00011960: 6b65 6428 290a 2020 2020 2020 2020 6175  ked().        au
+00011970: 746f 5f72 656e 616d 655f 706f 7274 735f  to_rename_ports_
+00011980: 6f72 6965 6e74 6174 696f 6e28 7365 6c66  orientation(self
+00011990: 2c20 2a2a 6b77 6172 6773 290a 0a20 2020  , **kwargs)..   
+000119a0: 2064 6566 206d 6f76 6528 0a20 2020 2020   def move(.     
+000119b0: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
+000119c0: 206f 7269 6769 6e3a 2046 6c6f 6174 3220   origin: Float2 
+000119d0: 3d20 2830 2c20 3029 2c0a 2020 2020 2020  = (0, 0),.      
+000119e0: 2020 6465 7374 696e 6174 696f 6e3a 204f    destination: O
+000119f0: 7074 696f 6e61 6c5b 466c 6f61 7432 5d20  ptional[Float2] 
+00011a00: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
+00011a10: 6178 6973 3a20 4f70 7469 6f6e 616c 5b41  axis: Optional[A
+00011a20: 7869 735d 203d 204e 6f6e 652c 0a20 2020  xis] = None,.   
+00011a30: 2029 202d 3e20 436f 6d70 6f6e 656e 743a   ) -> Component:
+00011a40: 0a20 2020 2020 2020 2022 2222 5265 7475  .        """Retu
+00011a50: 726e 7320 6e65 7720 436f 6d70 6f6e 656e  rns new Componen
+00011a60: 7420 7769 7468 2061 206d 6f76 6564 2072  t with a moved r
+00011a70: 6566 6572 656e 6365 2074 6f20 7468 6520  eference to the 
+00011a80: 6f72 6967 696e 616c 2e0a 0a20 2020 2020  original...     
+00011a90: 2020 2063 6f6d 706f 6e65 6e74 2e0a 0a20     component... 
+00011aa0: 2020 2020 2020 2041 7267 733a 0a20 2020         Args:.   
+00011ab0: 2020 2020 2020 2020 206f 7269 6769 6e3a           origin:
+00011ac0: 206f 6620 636f 6d70 6f6e 656e 742e 0a20   of component.. 
+00011ad0: 2020 2020 2020 2020 2020 2064 6573 7469             desti
+00011ae0: 6e61 7469 6f6e 3a20 782c 2079 2e0a 2020  nation: x, y..  
+00011af0: 2020 2020 2020 2020 2020 6178 6973 3a20            axis: 
+00011b00: 7820 6f72 2079 2e0a 2020 2020 2020 2020  x or y..        
+00011b10: 2222 220a 2020 2020 2020 2020 7261 6973  """.        rais
+00011b20: 6520 5661 6c75 6545 7272 6f72 286d 6f76  e ValueError(mov
+00011b30: 655f 6572 726f 725f 6d65 7373 6167 6529  e_error_message)
+00011b40: 0a0a 2020 2020 6465 6620 6d69 7272 6f72  ..    def mirror
+00011b50: 2873 656c 662c 2070 313a 2046 6c6f 6174  (self, p1: Float
+00011b60: 3220 3d20 2830 2c20 3129 2c20 7032 3a20  2 = (0, 1), p2: 
+00011b70: 466c 6f61 7432 203d 2028 302c 2030 292c  Float2 = (0, 0),
+00011b80: 202a 2a6b 7761 7267 7329 202d 3e20 436f   **kwargs) -> Co
+00011b90: 6d70 6f6e 656e 743a 0a20 2020 2020 2020  mponent:.       
+00011ba0: 2022 2222 5265 7475 726e 7320 6e65 7720   """Returns new 
+00011bb0: 436f 6d70 6f6e 656e 7420 7769 7468 2061  Component with a
+00011bc0: 206d 6972 726f 7265 6420 7265 6665 7265   mirrored refere
+00011bd0: 6e63 652e 0a0a 2020 2020 2020 2020 4172  nce...        Ar
+00011be0: 6773 3a0a 2020 2020 2020 2020 2020 2020  gs:.            
+00011bf0: 7031 3a20 6669 7273 7420 706f 696e 7420  p1: first point 
+00011c00: 746f 2064 6566 696e 6520 6d69 7272 6f72  to define mirror
+00011c10: 2061 7869 732e 0a20 2020 2020 2020 2020   axis..         
+00011c20: 2020 2070 323a 2073 6563 6f6e 6420 706f     p2: second po
+00011c30: 696e 7420 746f 2064 6566 696e 6520 6d69  int to define mi
+00011c40: 7272 6f72 2061 7869 732e 0a20 2020 2020  rror axis..     
+00011c50: 2020 2022 2222 0a20 2020 2020 2020 2066     """.        f
+00011c60: 726f 6d20 6764 7366 6163 746f 7279 2e66  rom gdsfactory.f
+00011c70: 756e 6374 696f 6e73 2069 6d70 6f72 7420  unctions import 
+00011c80: 6d69 7272 6f72 0a0a 2020 2020 2020 2020  mirror..        
+00011c90: 7265 7475 726e 206d 6972 726f 7228 636f  return mirror(co
+00011ca0: 6d70 6f6e 656e 743d 7365 6c66 2c20 7031  mponent=self, p1
+00011cb0: 3d70 312c 2070 323d 7032 2c20 2a2a 6b77  =p1, p2=p2, **kw
+00011cc0: 6172 6773 290a 0a20 2020 2064 6566 2072  args)..    def r
+00011cd0: 6f74 6174 6528 7365 6c66 2c20 616e 676c  otate(self, angl
+00011ce0: 653a 2066 6c6f 6174 203d 2039 302c 202a  e: float = 90, *
+00011cf0: 2a6b 7761 7267 7329 202d 3e20 436f 6d70  *kwargs) -> Comp
+00011d00: 6f6e 656e 743a 0a20 2020 2020 2020 2022  onent:.        "
+00011d10: 2222 5265 7475 726e 7320 6e65 7720 636f  ""Returns new co
+00011d20: 6d70 6f6e 656e 7420 7769 7468 2061 2072  mponent with a r
+00011d30: 6f74 6174 6564 2072 6566 6572 656e 6365  otated reference
+00011d40: 2074 6f20 7468 6520 6f72 6967 696e 616c   to the original
+00011d50: 2e0a 0a20 2020 2020 2020 2041 7267 733a  ...        Args:
+00011d60: 0a20 2020 2020 2020 2020 2020 2061 6e67  .            ang
+00011d70: 6c65 3a20 696e 2064 6567 7265 6573 2e0a  le: in degrees..
+00011d80: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00011d90: 2020 2020 6672 6f6d 2067 6473 6661 6374      from gdsfact
+00011da0: 6f72 792e 6675 6e63 7469 6f6e 7320 696d  ory.functions im
+00011db0: 706f 7274 2072 6f74 6174 650a 0a20 2020  port rotate..   
+00011dc0: 2020 2020 2072 6574 7572 6e20 726f 7461       return rota
+00011dd0: 7465 2863 6f6d 706f 6e65 6e74 3d73 656c  te(component=sel
+00011de0: 662c 2061 6e67 6c65 3d61 6e67 6c65 2c20  f, angle=angle, 
+00011df0: 2a2a 6b77 6172 6773 290a 0a20 2020 2064  **kwargs)..    d
+00011e00: 6566 2061 6464 5f70 6164 6469 6e67 2873  ef add_padding(s
+00011e10: 656c 662c 202a 2a6b 7761 7267 7329 202d  elf, **kwargs) -
+00011e20: 3e20 436f 6d70 6f6e 656e 743a 0a20 2020  > Component:.   
+00011e30: 2020 2020 2022 2222 5265 7475 726e 7320       """Returns 
+00011e40: 7361 6d65 2063 6f6d 706f 6e65 6e74 2077  same component w
+00011e50: 6974 6820 7061 6464 696e 672e 0a0a 2020  ith padding...  
+00011e60: 2020 2020 2020 4b65 7977 6f72 6420 4172        Keyword Ar
+00011e70: 6773 3a0a 2020 2020 2020 2020 2020 2020  gs:.            
+00011e80: 636f 6d70 6f6e 656e 743a 2066 6f72 2070  component: for p
+00011e90: 6164 6469 6e67 2e0a 2020 2020 2020 2020  adding..        
+00011ea0: 2020 2020 6c61 7965 7273 3a20 6c69 7374      layers: list
+00011eb0: 206f 6620 6c61 7965 7273 2e0a 2020 2020   of layers..    
+00011ec0: 2020 2020 2020 2020 7375 6666 6978 2066          suffix f
+00011ed0: 6f72 206e 616d 652e 0a20 2020 2020 2020  or name..       
+00011ee0: 2020 2020 2064 6566 6175 6c74 3a20 6465       default: de
+00011ef0: 6661 756c 7420 7061 6464 696e 6720 2835  fault padding (5
+00011f00: 3075 6d29 2e0a 2020 2020 2020 2020 2020  0um)..          
+00011f10: 2020 746f 703a 206e 6f72 7468 2070 6164    top: north pad
+00011f20: 6469 6e67 2e0a 2020 2020 2020 2020 2020  ding..          
+00011f30: 2020 626f 7474 6f6d 3a20 736f 7574 6820    bottom: south 
+00011f40: 7061 6464 696e 672e 0a20 2020 2020 2020  padding..       
+00011f50: 2020 2020 2072 6967 6874 3a20 6561 7374       right: east
+00011f60: 2070 6164 6469 6e67 2e0a 2020 2020 2020   padding..      
+00011f70: 2020 2020 2020 6c65 6674 3a20 7765 7374        left: west
+00011f80: 2070 6164 6469 6e67 2e0a 2020 2020 2020   padding..      
+00011f90: 2020 2222 220a 2020 2020 2020 2020 6672    """.        fr
+00011fa0: 6f6d 2067 6473 6661 6374 6f72 792e 6164  om gdsfactory.ad
+00011fb0: 645f 7061 6464 696e 6720 696d 706f 7274  d_padding import
+00011fc0: 2061 6464 5f70 6164 6469 6e67 0a0a 2020   add_padding..  
+00011fd0: 2020 2020 2020 7265 7475 726e 2061 6464        return add
+00011fe0: 5f70 6164 6469 6e67 2863 6f6d 706f 6e65  _padding(compone
+00011ff0: 6e74 3d73 656c 662c 202a 2a6b 7761 7267  nt=self, **kwarg
+00012000: 7329 0a0a 2020 2020 6465 6620 6162 736f  s)..    def abso
+00012010: 7262 2873 656c 662c 2072 6566 6572 656e  rb(self, referen
+00012020: 6365 2920 2d3e 2043 6f6d 706f 6e65 6e74  ce) -> Component
+00012030: 3a0a 2020 2020 2020 2020 2222 2241 6273  :.        """Abs
+00012040: 6f72 6273 2070 6f6c 7967 6f6e 7320 6672  orbs polygons fr
+00012050: 6f6d 2043 6f6d 706f 6e65 6e74 5265 6665  om ComponentRefe
+00012060: 7265 6e63 6520 696e 746f 2043 6f6d 706f  rence into Compo
+00012070: 6e65 6e74 2e0a 0a20 2020 2020 2020 2044  nent...        D
+00012080: 6573 7472 6f79 7320 7468 6520 7265 6665  estroys the refe
+00012090: 7265 6e63 6520 696e 2074 6865 2070 726f  rence in the pro
+000120a0: 6365 7373 2062 7574 206b 6565 7069 6e67  cess but keeping
+000120b0: 2074 6865 2070 6f6c 7967 6f6e 2067 656f   the polygon geo
+000120c0: 6d65 7472 792e 0a0a 2020 2020 2020 2020  metry...        
+000120d0: 4172 6773 3a0a 2020 2020 2020 2020 2020  Args:.          
+000120e0: 2020 7265 6665 7265 6e63 653a 2043 6f6d    reference: Com
+000120f0: 706f 6e65 6e74 5265 6665 7265 6e63 6520  ponentReference 
+00012100: 746f 2062 6520 6162 736f 7262 6564 2069  to be absorbed i
+00012110: 6e74 6f20 7468 6520 436f 6d70 6f6e 656e  nto the Componen
+00012120: 742e 0a20 2020 2020 2020 2022 2222 0a20  t..        """. 
+00012130: 2020 2020 2020 2069 6620 7265 6665 7265         if refere
+00012140: 6e63 6520 6e6f 7420 696e 2073 656c 662e  nce not in self.
+00012150: 7265 6665 7265 6e63 6573 3a0a 2020 2020  references:.    
+00012160: 2020 2020 2020 2020 7261 6973 6520 5661          raise Va
+00012170: 6c75 6545 7272 6f72 280a 2020 2020 2020  lueError(.      
+00012180: 2020 2020 2020 2020 2020 2254 6865 2072            "The r
+00012190: 6566 6572 656e 6365 2079 6f75 2061 736b  eference you ask
+000121a0: 6564 2074 6f20 6162 736f 7262 2064 6f65  ed to absorb doe
+000121b0: 7320 6e6f 7420 6578 6973 7420 696e 2074  s not exist in t
+000121c0: 6869 7320 436f 6d70 6f6e 656e 742e 220a  his Component.".
+000121d0: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+000121e0: 2020 2020 2020 7265 665f 706f 6c79 676f        ref_polygo
+000121f0: 6e73 203d 2072 6566 6572 656e 6365 2e67  ns = reference.g
+00012200: 6574 5f70 6f6c 7967 6f6e 7328 0a20 2020  et_polygons(.   
+00012210: 2020 2020 2020 2020 2062 795f 7370 6563           by_spec
+00012220: 3d46 616c 7365 2c20 696e 636c 7564 655f  =False, include_
+00012230: 7061 7468 733d 4661 6c73 652c 2061 735f  paths=False, as_
+00012240: 6172 7261 793d 4661 6c73 650a 2020 2020  array=False.    
+00012250: 2020 2020 290a 2020 2020 2020 2020 7365      ).        se
+00012260: 6c66 2e5f 6164 645f 706f 6c79 676f 6e73  lf._add_polygons
+00012270: 282a 7265 665f 706f 6c79 676f 6e73 290a  (*ref_polygons).
+00012280: 0a20 2020 2020 2020 2073 656c 662e 6164  .        self.ad
+00012290: 6428 7265 6665 7265 6e63 652e 6765 745f  d(reference.get_
+000122a0: 6c61 6265 6c73 2829 290a 2020 2020 2020  labels()).      
+000122b0: 2020 7365 6c66 2e61 6464 2872 6566 6572    self.add(refer
+000122c0: 656e 6365 2e67 6574 5f70 6174 6873 2829  ence.get_paths()
+000122d0: 290a 2020 2020 2020 2020 7365 6c66 2e72  ).        self.r
+000122e0: 656d 6f76 6528 7265 6665 7265 6e63 6529  emove(reference)
+000122f0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00012300: 7365 6c66 0a0a 2020 2020 6465 6620 7265  self..    def re
+00012310: 6d6f 7665 2873 656c 662c 2069 7465 6d73  move(self, items
+00012320: 293a 0a20 2020 2020 2020 2022 2222 5265  ):.        """Re
+00012330: 6d6f 7665 7320 6974 656d 7320 6672 6f6d  moves items from
+00012340: 2061 2043 6f6d 706f 6e65 6e74 2c20 7768   a Component, wh
+00012350: 6963 6820 6361 6e20 696e 636c 7564 6520  ich can include 
+00012360: 506f 7274 732c 2050 6f6c 7967 6f6e 5365  Ports, PolygonSe
+00012370: 7473 205c 0a20 2020 2020 2020 2043 656c  ts \.        Cel
+00012380: 6c52 6566 6572 656e 6365 732c 2043 6f6d  lReferences, Com
+00012390: 706f 6e65 6e74 5265 6665 7265 6e63 6573  ponentReferences
+000123a0: 2061 6e64 204c 6162 656c 732e 0a0a 2020   and Labels...  
+000123b0: 2020 2020 2020 4172 6773 3a0a 2020 2020        Args:.    
+000123c0: 2020 2020 2020 2020 6974 656d 733a 206c          items: l
+000123d0: 6973 7420 6f66 2049 7465 6d73 2074 6f20  ist of Items to 
+000123e0: 6265 2072 656d 6f76 6564 2066 726f 6d20  be removed from 
+000123f0: 7468 6520 436f 6d70 6f6e 656e 742e 0a20  the Component.. 
+00012400: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00012410: 2020 2069 6620 6e6f 7420 6861 7361 7474     if not hasatt
+00012420: 7228 6974 656d 732c 2022 5f5f 6974 6572  r(items, "__iter
+00012430: 5f5f 2229 3a0a 2020 2020 2020 2020 2020  __"):.          
+00012440: 2020 6974 656d 7320 3d20 5b69 7465 6d73    items = [items
+00012450: 5d0a 2020 2020 2020 2020 666f 7220 6974  ].        for it
+00012460: 656d 2069 6e20 6974 656d 733a 0a20 2020  em in items:.   
+00012470: 2020 2020 2020 2020 2069 6620 6973 696e           if isin
+00012480: 7374 616e 6365 2869 7465 6d2c 2050 6f72  stance(item, Por
+00012490: 7429 3a0a 2020 2020 2020 2020 2020 2020  t):.            
+000124a0: 2020 2020 7365 6c66 2e70 6f72 7473 203d      self.ports =
+000124b0: 207b 6b3a 2076 2066 6f72 206b 2c20 7620   {k: v for k, v 
+000124c0: 696e 2073 656c 662e 706f 7274 732e 6974  in self.ports.it
+000124d0: 656d 7328 2920 6966 2076 2021 3d20 6974  ems() if v != it
+000124e0: 656d 7d0a 2020 2020 2020 2020 2020 2020  em}.            
+000124f0: 656c 6966 2069 7369 6e73 7461 6e63 6528  elif isinstance(
+00012500: 6974 656d 2c20 6764 7374 6b2e 5265 6665  item, gdstk.Refe
+00012510: 7265 6e63 6529 3a0a 2020 2020 2020 2020  rence):.        
+00012520: 2020 2020 2020 2020 7365 6c66 2e5f 6365          self._ce
+00012530: 6c6c 2e72 656d 6f76 6528 6974 656d 290a  ll.remove(item).
+00012540: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012550: 6974 656d 2e6f 776e 6572 203d 204e 6f6e  item.owner = Non
+00012560: 650a 2020 2020 2020 2020 2020 2020 656c  e.            el
+00012570: 6966 2069 7369 6e73 7461 6e63 6528 6974  if isinstance(it
+00012580: 656d 2c20 436f 6d70 6f6e 656e 7452 6566  em, ComponentRef
+00012590: 6572 656e 6365 293a 0a20 2020 2020 2020  erence):.       
+000125a0: 2020 2020 2020 2020 2073 656c 662e 7265           self.re
+000125b0: 6665 7265 6e63 6573 2e72 656d 6f76 6528  ferences.remove(
+000125c0: 6974 656d 290a 2020 2020 2020 2020 2020  item).          
+000125d0: 2020 2020 2020 7365 6c66 2e5f 6365 6c6c        self._cell
+000125e0: 2e72 656d 6f76 6528 6974 656d 2e5f 7265  .remove(item._re
+000125f0: 6665 7265 6e63 6529 0a20 2020 2020 2020  ference).       
+00012600: 2020 2020 2020 2020 2069 7465 6d2e 6f77           item.ow
+00012610: 6e65 7220 3d20 4e6f 6e65 0a20 2020 2020  ner = None.     
+00012620: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00012630: 5f6e 616d 6564 5f72 6566 6572 656e 6365  _named_reference
+00012640: 732e 706f 7028 6974 656d 2e6e 616d 6529  s.pop(item.name)
+00012650: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
+00012660: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+00012670: 2020 2073 656c 662e 5f63 656c 6c2e 7265     self._cell.re
+00012680: 6d6f 7665 2869 7465 6d29 0a0a 2020 2020  move(item)..    
+00012690: 2020 2020 7365 6c66 2e5f 6262 5f76 616c      self._bb_val
+000126a0: 6964 203d 2046 616c 7365 0a20 2020 2020  id = False.     
+000126b0: 2020 2072 6574 7572 6e20 7365 6c66 0a0a     return self..
+000126c0: 2020 2020 6465 6620 6861 7368 5f67 656f      def hash_geo
+000126d0: 6d65 7472 7928 7365 6c66 2c20 7072 6563  metry(self, prec
+000126e0: 6973 696f 6e3a 2066 6c6f 6174 203d 2031  ision: float = 1
+000126f0: 652d 3429 202d 3e20 7374 723a 0a20 2020  e-4) -> str:.   
+00012700: 2020 2020 2022 2222 5265 7475 726e 7320       """Returns 
+00012710: 616e 2053 4841 3120 6861 7368 206f 6620  an SHA1 hash of 
+00012720: 7468 6520 6765 6f6d 6574 7279 2069 6e20  the geometry in 
+00012730: 7468 6520 436f 6d70 6f6e 656e 742e 0a0a  the Component...
+00012740: 2020 2020 2020 2020 466f 7220 6561 6368          For each
+00012750: 206c 6179 6572 2c20 6561 6368 2070 6f6c   layer, each pol
+00012760: 7967 6f6e 2069 7320 696e 6469 7669 6475  ygon is individu
+00012770: 616c 6c79 2068 6173 6865 6420 616e 6420  ally hashed and 
+00012780: 7468 656e 2074 6865 2070 6f6c 7967 6f6e  then the polygon
+00012790: 2068 6173 6865 730a 2020 2020 2020 2020   hashes.        
+000127a0: 6172 6520 736f 7274 6564 2c20 746f 2065  are sorted, to e
+000127b0: 6e73 7572 6520 7468 6520 6861 7368 2073  nsure the hash s
+000127c0: 7461 7973 2063 6f6e 7374 616e 7420 7265  tays constant re
+000127d0: 6761 7264 6c65 7373 206f 6620 7468 6520  gardless of the 
+000127e0: 6f72 6465 7269 6e67 0a20 2020 2020 2020  ordering.       
+000127f0: 2074 6865 2070 6f6c 7967 6f6e 732e 2020   the polygons.  
+00012800: 5369 6d69 6c61 726c 792c 2074 6865 206c  Similarly, the l
+00012810: 6179 6572 7320 6172 6520 736f 7274 6564  ayers are sorted
+00012820: 2062 7920 286c 6179 6572 2c20 6461 7461   by (layer, data
+00012830: 7479 7065 292e 0a0a 2020 2020 2020 2020  type)...        
+00012840: 4172 6773 3a0a 2020 2020 2020 2020 2020  Args:.          
+00012850: 2020 7072 6563 6973 696f 6e3a 2052 6f75    precision: Rou
+00012860: 6e64 696e 6720 7072 6563 6973 696f 6e20  nding precision 
+00012870: 666f 7220 7468 6520 7468 6520 6f62 6a65  for the the obje
+00012880: 6374 7320 696e 2074 6865 2043 6f6d 706f  cts in the Compo
+00012890: 6e65 6e74 2e0a 2020 2020 2020 2020 2020  nent..          
+000128a0: 2020 2020 2020 466f 7220 696e 7374 616e        For instan
+000128b0: 6365 2c20 6120 7072 6563 6973 696f 6e20  ce, a precision 
+000128c0: 6f66 2031 652d 3220 7769 6c6c 2072 6f75  of 1e-2 will rou
+000128d0: 6e64 2061 2070 6f69 6e74 2061 740a 2020  nd a point at.  
+000128e0: 2020 2020 2020 2020 2020 2020 2020 2830                (0
+000128f0: 2e31 3234 2c20 312e 3734 3829 2074 6f20  .124, 1.748) to 
+00012900: 2830 2e31 322c 2031 2e37 3529 2e0a 0a20  (0.12, 1.75)... 
+00012910: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00012920: 2020 2070 6f6c 7967 6f6e 735f 6279 5f73     polygons_by_s
+00012930: 7065 6320 3d20 7365 6c66 2e67 6574 5f70  pec = self.get_p
+00012940: 6f6c 7967 6f6e 7328 6279 5f73 7065 633d  olygons(by_spec=
+00012950: 5472 7565 2c20 6173 5f61 7272 6179 3d46  True, as_array=F
+00012960: 616c 7365 290a 2020 2020 2020 2020 6c61  alse).        la
+00012970: 7965 7273 203d 206e 702e 6172 7261 7928  yers = np.array(
+00012980: 6c69 7374 2870 6f6c 7967 6f6e 735f 6279  list(polygons_by
+00012990: 5f73 7065 632e 6b65 7973 2829 2929 0a20  _spec.keys())). 
+000129a0: 2020 2020 2020 2073 6f72 7465 645f 6c61         sorted_la
+000129b0: 7965 7273 203d 206c 6179 6572 735b 6e70  yers = layers[np
+000129c0: 2e6c 6578 736f 7274 2828 6c61 7965 7273  .lexsort((layers
+000129d0: 5b3a 2c20 305d 2c20 6c61 7965 7273 5b3a  [:, 0], layers[:
+000129e0: 2c20 315d 2929 5d0a 0a20 2020 2020 2020  , 1]))]..       
+000129f0: 2066 696e 616c 5f68 6173 6820 3d20 6861   final_hash = ha
+00012a00: 7368 6c69 622e 7368 6131 2829 0a20 2020  shlib.sha1().   
+00012a10: 2020 2020 2066 6f72 206c 6179 6572 2069       for layer i
+00012a20: 6e20 736f 7274 6564 5f6c 6179 6572 733a  n sorted_layers:
+00012a30: 0a20 2020 2020 2020 2020 2020 206c 6179  .            lay
+00012a40: 6572 5f68 6173 6820 3d20 6861 7368 6c69  er_hash = hashli
+00012a50: 622e 7368 6131 286c 6179 6572 2e61 7374  b.sha1(layer.ast
+00012a60: 7970 6528 6e70 2e69 6e74 3634 2929 2e64  ype(np.int64)).d
+00012a70: 6967 6573 7428 290a 2020 2020 2020 2020  igest().        
+00012a80: 2020 2020 706f 6c79 676f 6e73 203d 2070      polygons = p
+00012a90: 6f6c 7967 6f6e 735f 6279 5f73 7065 635b  olygons_by_spec[
+00012aa0: 7475 706c 6528 6c61 7965 7229 5d0a 2020  tuple(layer)].  
+00012ab0: 2020 2020 2020 2020 2020 706f 6c79 676f            polygo
+00012ac0: 6e73 203d 205b 5f72 6e64 2870 2e70 6f69  ns = [_rnd(p.poi
+00012ad0: 6e74 732c 2070 7265 6369 7369 6f6e 2920  nts, precision) 
+00012ae0: 666f 7220 7020 696e 2070 6f6c 7967 6f6e  for p in polygon
+00012af0: 735d 0a20 2020 2020 2020 2020 2020 2070  s].            p
+00012b00: 6f6c 7967 6f6e 5f68 6173 6865 7320 3d20  olygon_hashes = 
+00012b10: 6e70 2e73 6f72 7428 5b68 6173 686c 6962  np.sort([hashlib
+00012b20: 2e73 6861 3128 7029 2e64 6967 6573 7428  .sha1(p).digest(
+00012b30: 2920 666f 7220 7020 696e 2070 6f6c 7967  ) for p in polyg
+00012b40: 6f6e 735d 290a 2020 2020 2020 2020 2020  ons]).          
+00012b50: 2020 6669 6e61 6c5f 6861 7368 2e75 7064    final_hash.upd
+00012b60: 6174 6528 6c61 7965 725f 6861 7368 290a  ate(layer_hash).
+00012b70: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+00012b80: 7068 2069 6e20 706f 6c79 676f 6e5f 6861  ph in polygon_ha
+00012b90: 7368 6573 3a0a 2020 2020 2020 2020 2020  shes:.          
+00012ba0: 2020 2020 2020 6669 6e61 6c5f 6861 7368        final_hash
+00012bb0: 2e75 7064 6174 6528 7068 290a 0a20 2020  .update(ph)..   
+00012bc0: 2020 2020 2072 6574 7572 6e20 6669 6e61       return fina
+00012bd0: 6c5f 6861 7368 2e68 6578 6469 6765 7374  l_hash.hexdigest
+00012be0: 2829 0a0a 2020 2020 6465 6620 6765 745f  ()..    def get_
+00012bf0: 6c61 6265 6c73 280a 2020 2020 2020 2020  labels(.        
+00012c00: 7365 6c66 2c20 6170 706c 795f 7265 7065  self, apply_repe
+00012c10: 7469 7469 6f6e 733d 5472 7565 2c20 6465  titions=True, de
+00012c20: 7074 683a 204f 7074 696f 6e61 6c5b 696e  pth: Optional[in
+00012c30: 745d 203d 204e 6f6e 652c 206c 6179 6572  t] = None, layer
+00012c40: 3d4e 6f6e 650a 2020 2020 2920 2d3e 204c  =None.    ) -> L
+00012c50: 6973 745b 4c61 6265 6c5d 3a0a 2020 2020  ist[Label]:.    
+00012c60: 2020 2020 2222 2252 6574 7572 6e20 6c61      """Return la
+00012c70: 6265 6c73 2e0a 0a20 2020 2020 2020 2041  bels...        A
+00012c80: 7267 733a 0a20 2020 2020 2020 2020 2020  rgs:.           
+00012c90: 2061 7070 6c79 5f72 6570 6574 6974 696f   apply_repetitio
+00012ca0: 6e73 3a2e 0a20 2020 2020 2020 2020 2020  ns:..           
+00012cb0: 2064 6570 7468 3a20 4e6f 6e65 2072 6574   depth: None ret
+00012cc0: 7572 6e73 2061 6c6c 206c 6162 656c 7320  urns all labels 
+00012cd0: 616e 6420 3020 746f 7020 6c65 7665 6c2e  and 0 top level.
+00012ce0: 0a20 2020 2020 2020 2020 2020 206c 6179  .            lay
+00012cf0: 6572 3a20 6c61 7965 7273 7065 632e 0a20  er: layerspec.. 
+00012d00: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00012d10: 2020 2066 726f 6d20 6764 7366 6163 746f     from gdsfacto
+00012d20: 7279 2e70 646b 2069 6d70 6f72 7420 6765  ry.pdk import ge
+00012d30: 745f 6c61 7965 720a 0a20 2020 2020 2020  t_layer..       
+00012d40: 2069 6620 6c61 7965 723a 0a20 2020 2020   if layer:.     
+00012d50: 2020 2020 2020 206c 6179 6572 2c20 7465         layer, te
+00012d60: 7874 7479 7065 203d 2067 6574 5f6c 6179  xttype = get_lay
+00012d70: 6572 286c 6179 6572 290a 2020 2020 2020  er(layer).      
+00012d80: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+00012d90: 2020 2020 7465 7874 7479 7065 203d 204e      texttype = N
+00012da0: 6f6e 650a 2020 2020 2020 2020 7265 7475  one.        retu
+00012db0: 726e 2073 656c 662e 5f63 656c 6c2e 6765  rn self._cell.ge
+00012dc0: 745f 6c61 6265 6c73 280a 2020 2020 2020  t_labels(.      
+00012dd0: 2020 2020 2020 6170 706c 795f 7265 7065        apply_repe
+00012de0: 7469 7469 6f6e 733d 6170 706c 795f 7265  titions=apply_re
+00012df0: 7065 7469 7469 6f6e 732c 0a20 2020 2020  petitions,.     
+00012e00: 2020 2020 2020 2064 6570 7468 3d64 6570         depth=dep
+00012e10: 7468 2c0a 2020 2020 2020 2020 2020 2020  th,.            
+00012e20: 6c61 7965 723d 6c61 7965 722c 0a20 2020  layer=layer,.   
+00012e30: 2020 2020 2020 2020 2074 6578 7474 7970           texttyp
+00012e40: 653d 7465 7874 7479 7065 2c0a 2020 2020  e=texttype,.    
+00012e50: 2020 2020 290a 0a20 2020 2064 6566 2072      )..    def r
+00012e60: 656d 6f76 655f 6c61 6265 6c73 2873 656c  emove_labels(sel
+00012e70: 6629 202d 3e20 4e6f 6e65 3a0a 2020 2020  f) -> None:.    
+00012e80: 2020 2020 2222 2252 656d 6f76 6520 6c61      """Remove la
+00012e90: 6265 6c73 2e22 2222 0a20 2020 2020 2020  bels.""".       
+00012ea0: 2073 656c 662e 5f63 656c 6c2e 7265 6d6f   self._cell.remo
+00012eb0: 7665 282a 7365 6c66 2e6c 6162 656c 7329  ve(*self.labels)
+00012ec0: 0a0a 2020 2020 2320 4465 7072 6563 6174  ..    # Deprecat
+00012ed0: 6564 0a20 2020 2064 6566 2067 6574 5f69  ed.    def get_i
+00012ee0: 6e66 6f28 7365 6c66 293a 0a20 2020 2020  nfo(self):.     
+00012ef0: 2020 2022 2222 4761 7468 6572 7320 7468     """Gathers th
+00012f00: 6520 2e69 6e66 6f20 6469 6374 696f 6e61  e .info dictiona
+00012f10: 7269 6573 2066 726f 6d20 6576 6572 7920  ries from every 
+00012f20: 7375 622d 436f 6d70 6f6e 656e 7420 616e  sub-Component an
+00012f30: 6420 7265 7475 726e 7320 7468 656d 2069  d returns them i
+00012f40: 6e20 6120 6c69 7374 2e0a 0a20 2020 2020  n a list...     
+00012f50: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
+00012f60: 2020 2020 2064 6570 7468 3a20 696e 7420       depth: int 
+00012f70: 6f72 204e 6f6e 650a 2020 2020 2020 2020  or None.        
+00012f80: 2020 2020 2020 2020 4966 206e 6f74 204e          If not N
+00012f90: 6f6e 652c 2064 6566 696e 6573 2066 726f  one, defines fro
+00012fa0: 6d20 686f 7720 6d61 6e79 2072 6566 6572  m how many refer
+00012fb0: 656e 6365 206c 6576 656c 7320 746f 0a20  ence levels to. 
+00012fc0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00012fd0: 6574 7269 6576 6520 506f 7274 7320 6672  etrieve Ports fr
+00012fe0: 6f6d 2e0a 0a20 2020 2020 2020 2052 6574  om...        Ret
+00012ff0: 7572 6e73 3a0a 2020 2020 2020 2020 2020  urns:.          
+00013000: 2020 6c69 7374 206f 6620 6469 6374 696f    list of dictio
+00013010: 6e61 7269 6573 0a20 2020 2020 2020 2020  naries.         
+00013020: 2020 2020 2020 204c 6973 7420 6f66 2074         List of t
+00013030: 6865 2022 2e69 6e66 6f22 2070 726f 7065  he ".info" prope
+00013040: 7274 7920 6469 6374 696f 6e61 7269 6573  rty dictionaries
+00013050: 2066 726f 6d20 616c 6c20 7375 622d 436f   from all sub-Co
+00013060: 6d70 6f6e 656e 7473 0a20 2020 2020 2020  mponents.       
+00013070: 2022 2222 0a20 2020 2020 2020 2044 5f6c   """.        D_l
+00013080: 6973 7420 3d20 7365 6c66 2e67 6574 5f64  ist = self.get_d
+00013090: 6570 656e 6465 6e63 6965 7328 7265 6375  ependencies(recu
+000130a0: 7273 6976 653d 5472 7565 290a 2020 2020  rsive=True).    
+000130b0: 2020 2020 7265 7475 726e 205b 442e 696e      return [D.in
+000130c0: 666f 2e63 6f70 7928 2920 666f 7220 4420  fo.copy() for D 
+000130d0: 696e 2044 5f6c 6973 745d 0a0a 2020 2020  in D_list]..    
+000130e0: 6465 6620 7265 6d61 705f 6c61 7965 7273  def remap_layers
+000130f0: 280a 2020 2020 2020 2020 7365 6c66 2c20  (.        self, 
+00013100: 6c61 7965 726d 6170 2c20 696e 636c 7564  layermap, includ
+00013110: 655f 6c61 6265 6c73 3a20 626f 6f6c 203d  e_labels: bool =
+00013120: 2054 7275 652c 2069 6e63 6c75 6465 5f70   True, include_p
+00013130: 6174 6873 3a20 626f 6f6c 203d 2054 7275  aths: bool = Tru
+00013140: 650a 2020 2020 2920 2d3e 2043 6f6d 706f  e.    ) -> Compo
+00013150: 6e65 6e74 3a0a 2020 2020 2020 2020 2222  nent:.        ""
+00013160: 2252 6574 7572 6e73 2061 2063 6f70 7920  "Returns a copy 
+00013170: 6f66 2074 6865 2063 6f6d 706f 6e65 6e74  of the component
+00013180: 2077 6974 6820 7265 6d61 7070 6564 206c   with remapped l
+00013190: 6179 6572 732e 0a0a 2020 2020 2020 2020  ayers...        
+000131a0: 4172 6773 3a0a 2020 2020 2020 2020 2020  Args:.          
+000131b0: 2020 6c61 7965 726d 6170 3a20 4469 6374    layermap: Dict
+000131c0: 696f 6e61 7279 206f 6620 7661 6c75 6573  ionary of values
+000131d0: 2069 6e20 666f 726d 6174 207b 6c61 7965   in format {laye
+000131e0: 725f 6672 6f6d 203a 206c 6179 6572 5f74  r_from : layer_t
+000131f0: 6f7d 2e0a 2020 2020 2020 2020 2020 2020  o}..            
+00013200: 696e 636c 7564 655f 6c61 6265 6c73 3a20  include_labels: 
+00013210: 5365 6c65 6374 7320 7768 6574 6865 7220  Selects whether 
+00013220: 746f 206d 6f76 6520 4c61 6265 6c73 2061  to move Labels a
+00013230: 6c6f 6e67 2077 6974 6820 706f 6c79 676f  long with polygo
+00013240: 6e73 2e0a 2020 2020 2020 2020 2020 2020  ns..            
+00013250: 696e 636c 7564 655f 7061 7468 733a 2053  include_paths: S
+00013260: 656c 6563 7473 2077 6865 7468 6572 2074  elects whether t
+00013270: 6f20 6d6f 7665 2050 6174 6873 2061 6c6f  o move Paths alo
+00013280: 6e67 2077 6974 6820 706f 6c79 676f 6e73  ng with polygons
+00013290: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
+000132a0: 2020 2020 2020 636f 6d70 6f6e 656e 7420        component 
+000132b0: 3d20 7365 6c66 2e63 6f70 7928 290a 2020  = self.copy().  
+000132c0: 2020 2020 2020 6c61 7965 726d 6170 203d        layermap =
+000132d0: 207b 5f70 6172 7365 5f6c 6179 6572 286b   {_parse_layer(k
+000132e0: 293a 205f 7061 7273 655f 6c61 7965 7228  ): _parse_layer(
+000132f0: 7629 2066 6f72 206b 2c20 7620 696e 206c  v) for k, v in l
+00013300: 6179 6572 6d61 702e 6974 656d 7328 297d  ayermap.items()}
+00013310: 0a0a 2020 2020 2020 2020 616c 6c5f 4420  ..        all_D 
+00013320: 3d20 6c69 7374 2863 6f6d 706f 6e65 6e74  = list(component
+00013330: 2e67 6574 5f64 6570 656e 6465 6e63 6965  .get_dependencie
+00013340: 7328 5472 7565 2929 0a20 2020 2020 2020  s(True)).       
+00013350: 2061 6c6c 5f44 2e61 7070 656e 6428 636f   all_D.append(co
+00013360: 6d70 6f6e 656e 7429 0a20 2020 2020 2020  mponent).       
+00013370: 2066 6f72 2044 2069 6e20 616c 6c5f 443a   for D in all_D:
+00013380: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
+00013390: 2070 2069 6e20 442e 706f 6c79 676f 6e73   p in D.polygons
+000133a0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000133b0: 2020 6c61 7965 7220 3d20 2870 2e6c 6179    layer = (p.lay
+000133c0: 6572 2c20 702e 6461 7461 7479 7065 290a  er, p.datatype).
+000133d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000133e0: 6966 206c 6179 6572 2069 6e20 6c61 7965  if layer in laye
+000133f0: 726d 6170 3a0a 2020 2020 2020 2020 2020  rmap:.          
+00013400: 2020 2020 2020 2020 2020 6e65 775f 6c61            new_la
+00013410: 7965 7220 3d20 6c61 7965 726d 6170 5b6c  yer = layermap[l
+00013420: 6179 6572 5d0a 2020 2020 2020 2020 2020  ayer].          
+00013430: 2020 2020 2020 2020 2020 702e 6c61 7965            p.laye
+00013440: 7220 3d20 6e65 775f 6c61 7965 725b 305d  r = new_layer[0]
+00013450: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00013460: 2020 2020 2070 2e64 6174 6174 7970 6520       p.datatype 
+00013470: 3d20 6e65 775f 6c61 7965 725b 315d 0a20  = new_layer[1]. 
+00013480: 2020 2020 2020 2020 2020 2069 6620 696e             if in
+00013490: 636c 7564 655f 6c61 6265 6c73 3a0a 2020  clude_labels:.  
+000134a0: 2020 2020 2020 2020 2020 2020 2020 666f                fo
+000134b0: 7220 6c61 6265 6c20 696e 2044 2e6c 6162  r label in D.lab
+000134c0: 656c 733a 0a20 2020 2020 2020 2020 2020  els:.           
+000134d0: 2020 2020 2020 2020 206f 7269 6769 6e61           origina
+000134e0: 6c5f 6c61 7965 7220 3d20 286c 6162 656c  l_layer = (label
+000134f0: 2e6c 6179 6572 2c20 6c61 6265 6c2e 7465  .layer, label.te
+00013500: 7874 7479 7065 290a 2020 2020 2020 2020  xttype).        
+00013510: 2020 2020 2020 2020 2020 2020 6f72 6967              orig
+00013520: 696e 616c 5f6c 6179 6572 203d 205f 7061  inal_layer = _pa
+00013530: 7273 655f 6c61 7965 7228 6f72 6967 696e  rse_layer(origin
+00013540: 616c 5f6c 6179 6572 290a 2020 2020 2020  al_layer).      
+00013550: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00013560: 206f 7269 6769 6e61 6c5f 6c61 7965 7220   original_layer 
+00013570: 696e 206c 6179 6572 6d61 703a 0a20 2020  in layermap:.   
+00013580: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013590: 2020 2020 206e 6577 5f6c 6179 6572 203d       new_layer =
+000135a0: 206c 6179 6572 6d61 705b 6f72 6967 696e   layermap[origin
+000135b0: 616c 5f6c 6179 6572 5d0a 2020 2020 2020  al_layer].      
+000135c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000135d0: 2020 6c61 6265 6c2e 6c61 7965 7220 3d20    label.layer = 
+000135e0: 6e65 775f 6c61 7965 725b 305d 0a20 2020  new_layer[0].   
+000135f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013600: 2020 2020 206c 6162 656c 2e74 6578 7474       label.textt
+00013610: 7970 6520 3d20 6e65 775f 6c61 7965 725b  ype = new_layer[
+00013620: 315d 0a0a 2020 2020 2020 2020 2020 2020  1]..            
+00013630: 6966 2069 6e63 6c75 6465 5f70 6174 6873  if include_paths
+00013640: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00013650: 2020 666f 7220 7061 7468 2069 6e20 442e    for path in D.
+00013660: 7061 7468 733a 0a20 2020 2020 2020 2020  paths:.         
+00013670: 2020 2020 2020 2020 2020 206e 6577 5f6c             new_l
+00013680: 6179 6572 7320 3d20 6c69 7374 2870 6174  ayers = list(pat
+00013690: 682e 6c61 7965 7273 290a 2020 2020 2020  h.layers).      
+000136a0: 2020 2020 2020 2020 2020 2020 2020 6e65                ne
+000136b0: 775f 6461 7461 7479 7065 7320 3d20 6c69  w_datatypes = li
+000136c0: 7374 2870 6174 682e 6461 7461 7479 7065  st(path.datatype
+000136d0: 7329 0a20 2020 2020 2020 2020 2020 2020  s).             
+000136e0: 2020 2020 2020 2066 6f72 206c 6179 6572         for layer
+000136f0: 5f6e 756d 6265 7220 696e 2072 616e 6765  _number in range
+00013700: 286c 656e 286e 6577 5f6c 6179 6572 7329  (len(new_layers)
+00013710: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+00013720: 2020 2020 2020 2020 2020 206f 7269 6769             origi
+00013730: 6e61 6c5f 6c61 7965 7220 3d20 5f70 6172  nal_layer = _par
+00013740: 7365 5f6c 6179 6572 280a 2020 2020 2020  se_layer(.      
 00013750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013760: 2020 2020 2020 2020 206e 6577 5f6c 6179           new_lay
-00013770: 6572 203d 206c 6179 6572 6d61 705b 6f72  er = layermap[or
-00013780: 6967 696e 616c 5f6c 6179 6572 5d0a 2020  iginal_layer].  
-00013790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000137a0: 2020 2020 2020 2020 2020 6e65 775f 6c61            new_la
-000137b0: 7965 7273 5b6c 6179 6572 5f6e 756d 6265  yers[layer_numbe
-000137c0: 725d 203d 206e 6577 5f6c 6179 6572 5b30  r] = new_layer[0
-000137d0: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
-000137e0: 2020 2020 2020 2020 2020 2020 2020 6e65                ne
-000137f0: 775f 6461 7461 7479 7065 735b 6c61 7965  w_datatypes[laye
-00013800: 725f 6e75 6d62 6572 5d20 3d20 6e65 775f  r_number] = new_
-00013810: 6c61 7965 725b 315d 0a20 2020 2020 2020  layer[1].       
-00013820: 2020 2020 2020 2020 2020 2020 2070 6174               pat
-00013830: 682e 7365 745f 6c61 7965 7273 282a 6e65  h.set_layers(*ne
-00013840: 775f 6c61 7965 7273 290a 2020 2020 2020  w_layers).      
-00013850: 2020 2020 2020 2020 2020 2020 2020 7061                pa
-00013860: 7468 2e73 6574 5f64 6174 6174 7970 6573  th.set_datatypes
-00013870: 282a 6e65 775f 6461 7461 7479 7065 7329  (*new_datatypes)
-00013880: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00013890: 636f 6d70 6f6e 656e 740a 0a20 2020 2064  component..    d
-000138a0: 6566 2074 6f5f 3364 280a 2020 2020 2020  ef to_3d(.      
-000138b0: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
-000138c0: 6c61 7965 725f 7669 6577 733a 204f 7074  layer_views: Opt
-000138d0: 696f 6e61 6c5b 4c61 7965 7256 6965 7773  ional[LayerViews
-000138e0: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2020  ] = None,.      
-000138f0: 2020 6c61 7965 725f 7374 6163 6b3a 204f    layer_stack: O
-00013900: 7074 696f 6e61 6c5b 4c61 7965 7253 7461  ptional[LayerSta
-00013910: 636b 5d20 3d20 4e6f 6e65 2c0a 2020 2020  ck] = None,.    
-00013920: 2020 2020 6578 636c 7564 655f 6c61 7965      exclude_laye
-00013930: 7273 3a20 4f70 7469 6f6e 616c 5b54 7570  rs: Optional[Tup
-00013940: 6c65 5b4c 6179 6572 2c20 2e2e 2e5d 5d20  le[Layer, ...]] 
-00013950: 3d20 4e6f 6e65 2c0a 2020 2020 293a 0a20  = None,.    ):. 
-00013960: 2020 2020 2020 2022 2222 5265 7475 726e         """Return
-00013970: 2043 6f6d 706f 6e65 6e74 2033 4420 7472   Component 3D tr
-00013980: 696d 6573 6820 5363 656e 652e 0a0a 2020  imesh Scene...  
-00013990: 2020 2020 2020 4172 6773 3a0a 2020 2020        Args:.    
-000139a0: 2020 2020 2020 2020 636f 6d70 6f6e 656e          componen
-000139b0: 743a 2074 6f20 6578 7472 7564 6520 696e  t: to extrude in
-000139c0: 2033 442e 0a20 2020 2020 2020 2020 2020   3D..           
-000139d0: 206c 6179 6572 5f76 6965 7773 3a20 6c61   layer_views: la
-000139e0: 7965 7220 636f 6c6f 7273 2066 726f 6d20  yer colors from 
-000139f0: 4b6c 6179 6f75 7420 4c61 7965 7220 5072  Klayout Layer Pr
-00013a00: 6f70 6572 7469 6573 2066 696c 652e 0a20  operties file.. 
-00013a10: 2020 2020 2020 2020 2020 2020 2020 2044                 D
-00013a20: 6566 6175 6c74 7320 746f 2061 6374 6976  efaults to activ
-00013a30: 6520 5044 4b2e 6c61 7965 725f 7669 6577  e PDK.layer_view
-00013a40: 732e 0a20 2020 2020 2020 2020 2020 206c  s..            l
-00013a50: 6179 6572 5f73 7461 636b 3a20 636f 6e74  ayer_stack: cont
-00013a60: 6169 6e73 2074 6869 636b 6e65 7373 2061  ains thickness a
-00013a70: 6e64 207a 6d69 6e20 666f 7220 6561 6368  nd zmin for each
-00013a80: 206c 6179 6572 2e0a 2020 2020 2020 2020   layer..        
-00013a90: 2020 2020 2020 2020 4465 6661 756c 7473          Defaults
-00013aa0: 2074 6f20 6163 7469 7665 2050 444b 2e6c   to active PDK.l
-00013ab0: 6179 6572 5f73 7461 636b 2e0a 2020 2020  ayer_stack..    
-00013ac0: 2020 2020 2020 2020 6578 636c 7564 655f          exclude_
-00013ad0: 6c61 7965 7273 3a20 6c61 7965 7273 2074  layers: layers t
-00013ae0: 6f20 6578 636c 7564 652e 0a0a 2020 2020  o exclude...    
-00013af0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00013b00: 6672 6f6d 2067 6473 6661 6374 6f72 792e  from gdsfactory.
-00013b10: 6578 706f 7274 2e74 6f5f 3364 2069 6d70  export.to_3d imp
-00013b20: 6f72 7420 746f 5f33 640a 0a20 2020 2020  ort to_3d..     
-00013b30: 2020 2072 6574 7572 6e20 746f 5f33 6428     return to_3d(
-00013b40: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00013b50: 662c 0a20 2020 2020 2020 2020 2020 206c  f,.            l
-00013b60: 6179 6572 5f76 6965 7773 3d6c 6179 6572  ayer_views=layer
-00013b70: 5f76 6965 7773 2c0a 2020 2020 2020 2020  _views,.        
-00013b80: 2020 2020 6c61 7965 725f 7374 6163 6b3d      layer_stack=
-00013b90: 6c61 7965 725f 7374 6163 6b2c 0a20 2020  layer_stack,.   
-00013ba0: 2020 2020 2020 2020 2065 7863 6c75 6465           exclude
-00013bb0: 5f6c 6179 6572 733d 6578 636c 7564 655f  _layers=exclude_
-00013bc0: 6c61 7965 7273 2c0a 2020 2020 2020 2020  layers,.        
-00013bd0: 290a 0a20 2020 2064 6566 2074 6f5f 6e70  )..    def to_np
-00013be0: 280a 2020 2020 2020 2020 7365 6c66 2c0a  (.        self,.
-00013bf0: 2020 2020 2020 2020 6e6d 5f70 6572 5f70          nm_per_p
-00013c00: 6978 656c 3a20 696e 7420 3d20 3230 2c0a  ixel: int = 20,.
-00013c10: 2020 2020 2020 2020 6c61 7965 7273 3a20          layers: 
-00013c20: 4c61 7965 7273 203d 2028 2831 2c20 3029  Layers = ((1, 0)
-00013c30: 2c29 2c0a 2020 2020 2020 2020 7661 6c75  ,),.        valu
-00013c40: 6573 3a20 4f70 7469 6f6e 616c 5b54 7570  es: Optional[Tup
-00013c50: 6c65 5b66 6c6f 6174 2c20 2e2e 2e5d 5d20  le[float, ...]] 
-00013c60: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
-00013c70: 7061 645f 7769 6474 683a 2069 6e74 203d  pad_width: int =
-00013c80: 2031 2c0a 2020 2020 2920 2d3e 206e 702e   1,.    ) -> np.
-00013c90: 6e64 6172 7261 793a 0a20 2020 2020 2020  ndarray:.       
-00013ca0: 2022 2222 5265 7475 726e 7320 6120 7069   """Returns a pi
-00013cb0: 7865 6c61 7465 6420 6e75 6d70 7920 6172  xelated numpy ar
-00013cc0: 7261 7920 6672 6f6d 2043 6f6d 706f 6e65  ray from Compone
-00013cd0: 6e74 2070 6f6c 7967 6f6e 732e 0a0a 2020  nt polygons...  
-00013ce0: 2020 2020 2020 4172 6773 3a0a 2020 2020        Args:.    
-00013cf0: 2020 2020 2020 2020 636f 6d70 6f6e 656e          componen
-00013d00: 743a 2043 6f6d 706f 6e65 6e74 2e0a 2020  t: Component..  
-00013d10: 2020 2020 2020 2020 2020 6e6d 5f70 6572            nm_per
-00013d20: 5f70 6978 656c 3a20 796f 7520 6361 6e20  _pixel: you can 
-00013d30: 676f 2066 726f 6d20 3230 2028 636f 6172  go from 20 (coar
-00013d40: 7365 2920 746f 2034 2028 6669 6e65 292e  se) to 4 (fine).
-00013d50: 0a20 2020 2020 2020 2020 2020 206c 6179  .            lay
-00013d60: 6572 733a 2074 6f20 636f 6e76 6572 742e  ers: to convert.
-00013d70: 204f 7264 6572 206d 6174 7465 7273 2028   Order matters (
-00013d80: 6c61 7474 6572 206f 7665 7277 7269 7465  latter overwrite
-00013d90: 2066 6f72 6d65 7229 2e0a 2020 2020 2020   former)..      
-00013da0: 2020 2020 2020 7661 6c75 6573 3a20 6173        values: as
-00013db0: 736f 6369 6174 6564 2074 6f20 6561 6368  sociated to each
-00013dc0: 206c 6179 6572 2028 6465 6661 756c 7473   layer (defaults
-00013dd0: 2074 6f20 3129 2e0a 2020 2020 2020 2020   to 1)..        
-00013de0: 2020 2020 7061 645f 7769 6474 683a 2070      pad_width: p
-00013df0: 6164 6469 6e67 2070 6978 656c 7320 6172  adding pixels ar
-00013e00: 6f75 6e64 2074 6865 2069 6d61 6765 2e0a  ound the image..
-00013e10: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00013e20: 2020 2020 2066 726f 6d20 6764 7366 6163       from gdsfac
-00013e30: 746f 7279 2e65 7870 6f72 742e 746f 5f6e  tory.export.to_n
-00013e40: 7020 696d 706f 7274 2074 6f5f 6e70 0a0a  p import to_np..
-00013e50: 2020 2020 2020 2020 7265 7475 726e 2074          return t
-00013e60: 6f5f 6e70 280a 2020 2020 2020 2020 2020  o_np(.          
-00013e70: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
-00013e80: 2020 2020 6e6d 5f70 6572 5f70 6978 656c      nm_per_pixel
-00013e90: 3d6e 6d5f 7065 725f 7069 7865 6c2c 0a20  =nm_per_pixel,. 
-00013ea0: 2020 2020 2020 2020 2020 206c 6179 6572             layer
-00013eb0: 733d 6c61 7965 7273 2c0a 2020 2020 2020  s=layers,.      
-00013ec0: 2020 2020 2020 7661 6c75 6573 3d76 616c        values=val
-00013ed0: 7565 732c 0a20 2020 2020 2020 2020 2020  ues,.           
-00013ee0: 2070 6164 5f77 6964 7468 3d70 6164 5f77   pad_width=pad_w
-00013ef0: 6964 7468 2c0a 2020 2020 2020 2020 290a  idth,.        ).
-00013f00: 0a20 2020 2064 6566 2077 7269 7465 5f73  .    def write_s
-00013f10: 746c 280a 2020 2020 2020 2020 7365 6c66  tl(.        self
-00013f20: 2c0a 2020 2020 2020 2020 6669 6c65 7061  ,.        filepa
-00013f30: 7468 3a20 7374 722c 0a20 2020 2020 2020  th: str,.       
-00013f40: 206c 6179 6572 5f73 7461 636b 3a20 4f70   layer_stack: Op
-00013f50: 7469 6f6e 616c 5b4c 6179 6572 5374 6163  tional[LayerStac
-00013f60: 6b5d 203d 204e 6f6e 652c 0a20 2020 2020  k] = None,.     
-00013f70: 2020 2065 7863 6c75 6465 5f6c 6179 6572     exclude_layer
-00013f80: 733a 204f 7074 696f 6e61 6c5b 5475 706c  s: Optional[Tupl
-00013f90: 655b 4c61 7965 722c 202e 2e2e 5d5d 203d  e[Layer, ...]] =
-00013fa0: 204e 6f6e 652c 0a20 2020 2029 202d 3e20   None,.    ) -> 
-00013fb0: 6e70 2e6e 6461 7272 6179 3a0a 2020 2020  np.ndarray:.    
-00013fc0: 2020 2020 2222 2257 7269 7465 2061 2043      """Write a C
-00013fd0: 6f6d 706f 6e65 6e74 2074 6f20 5354 4c20  omponent to STL 
-00013fe0: 666f 7220 3344 2070 7269 6e74 696e 672e  for 3D printing.
-00013ff0: 0a0a 2020 2020 2020 2020 4172 6773 3a0a  ..        Args:.
-00014000: 2020 2020 2020 2020 2020 2020 6669 6c65              file
-00014010: 7061 7468 3a20 746f 2077 7269 7465 2053  path: to write S
-00014020: 544c 2074 6f2e 0a20 2020 2020 2020 2020  TL to..         
-00014030: 2020 206c 6179 6572 5f73 7461 636b 3a20     layer_stack: 
-00014040: 636f 6e74 6169 6e73 2074 6869 636b 6e65  contains thickne
-00014050: 7373 2061 6e64 207a 6d69 6e20 666f 7220  ss and zmin for 
-00014060: 6561 6368 206c 6179 6572 2e0a 2020 2020  each layer..    
-00014070: 2020 2020 2020 2020 6578 636c 7564 655f          exclude_
-00014080: 6c61 7965 7273 3a20 6c61 7965 7273 2074  layers: layers t
-00014090: 6f20 6578 636c 7564 652e 0a20 2020 2020  o exclude..     
-000140a0: 2020 2020 2020 2075 7365 5f6c 6179 6572         use_layer
-000140b0: 5f6e 616d 653a 2049 6620 5472 7565 2c20  _name: If True, 
-000140c0: 7573 6573 204c 6179 6572 4c65 7665 6c20  uses LayerLevel 
-000140d0: 6e61 6d65 7320 696e 206f 7574 7075 7420  names in output 
-000140e0: 6669 6c65 6e61 6d65 7320 7261 7468 6572  filenames rather
-000140f0: 2074 6861 6e20 6764 735f 6c61 7965 7220   than gds_layer 
-00014100: 616e 6420 6764 735f 6461 7461 7479 7065  and gds_datatype
-00014110: 2e0a 2020 2020 2020 2020 2020 2020 6875  ..            hu
-00014120: 6c6c 5f69 6e76 616c 6964 5f70 6f6c 7967  ll_invalid_polyg
-00014130: 6f6e 733a 2049 6620 5472 7565 2c20 7265  ons: If True, re
-00014140: 706c 6163 6573 2069 6e76 616c 6964 2070  places invalid p
-00014150: 6f6c 7967 6f6e 7320 2864 6574 6572 6d69  olygons (determi
-00014160: 6e65 6420 6279 2073 6861 7065 6c79 2e50  ned by shapely.P
-00014170: 6f6c 7967 6f6e 2e69 735f 7661 6c69 6429  olygon.is_valid)
-00014180: 2077 6974 6820 6974 7320 636f 6e76 6578   with its convex
-00014190: 2068 756c 6c2e 0a20 2020 2020 2020 2020   hull..         
-000141a0: 2020 2073 6361 6c65 3a20 4f70 7469 6f6e     scale: Option
-000141b0: 616c 2066 6163 746f 7220 6279 2077 6869  al factor by whi
-000141c0: 6368 2074 6f20 7363 616c 6520 6d65 7368  ch to scale mesh
-000141d0: 6573 2062 6566 6f72 6520 7772 6974 696e  es before writin
-000141e0: 672e 0a0a 2020 2020 2020 2020 2222 220a  g...        """.
-000141f0: 2020 2020 2020 2020 6672 6f6d 2067 6473          from gds
-00014200: 6661 6374 6f72 792e 6578 706f 7274 2e74  factory.export.t
-00014210: 6f5f 7374 6c20 696d 706f 7274 2074 6f5f  o_stl import to_
-00014220: 7374 6c0a 0a20 2020 2020 2020 2072 6574  stl..        ret
-00014230: 7572 6e20 746f 5f73 746c 280a 2020 2020  urn to_stl(.    
-00014240: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
-00014250: 2020 2020 2020 2020 2020 6669 6c65 7061            filepa
-00014260: 7468 3d66 696c 6570 6174 682c 0a20 2020  th=filepath,.   
-00014270: 2020 2020 2020 2020 206c 6179 6572 5f73           layer_s
-00014280: 7461 636b 3d6c 6179 6572 5f73 7461 636b  tack=layer_stack
-00014290: 2c0a 2020 2020 2020 2020 2020 2020 6578  ,.            ex
-000142a0: 636c 7564 655f 6c61 7965 7273 3d65 7863  clude_layers=exc
-000142b0: 6c75 6465 5f6c 6179 6572 732c 0a20 2020  lude_layers,.   
-000142c0: 2020 2020 2029 0a0a 2020 2020 6465 6620       )..    def 
-000142d0: 746f 5f67 6d73 6828 0a20 2020 2020 2020  to_gmsh(.       
-000142e0: 2073 656c 662c 0a20 2020 2020 2020 2074   self,.        t
-000142f0: 7970 652c 0a20 2020 2020 2020 207a 3d4e  ype,.        z=N
-00014300: 6f6e 652c 0a20 2020 2020 2020 2078 7365  one,.        xse
-00014310: 6374 696f 6e5f 626f 756e 6473 3d4e 6f6e  ction_bounds=Non
-00014320: 652c 0a20 2020 2020 2020 206c 6179 6572  e,.        layer
-00014330: 5f73 7461 636b 3d4e 6f6e 652c 0a20 2020  _stack=None,.   
-00014340: 2020 2020 2077 6166 6572 5f70 6164 6469       wafer_paddi
-00014350: 6e67 3d30 2e30 2c0a 2020 2020 2020 2020  ng=0.0,.        
-00014360: 7761 6665 725f 6c61 7965 723d 4c41 5945  wafer_layer=LAYE
-00014370: 522e 5741 4645 522c 0a20 2020 2020 2020  R.WAFER,.       
-00014380: 202a 6172 6773 2c0a 2020 2020 2020 2020   *args,.        
-00014390: 2a2a 6b77 6172 6773 2c0a 2020 2020 293a  **kwargs,.    ):
-000143a0: 0a20 2020 2020 2020 2022 2222 5265 7475  .        """Retu
-000143b0: 726e 7320 6120 676d 7368 206d 7368 206f  rns a gmsh msh o
-000143c0: 6620 7468 6520 636f 6d70 6f6e 656e 7420  f the component 
-000143d0: 666f 7220 6669 6e69 7465 2065 6c65 6d65  for finite eleme
-000143e0: 6e74 2073 696d 756c 6174 696f 6e2e 0a0a  nt simulation...
-000143f0: 2020 2020 2020 2020 4172 6775 6d65 6e74          Argument
-00014400: 733a 0a20 2020 2020 2020 2020 2020 2074  s:.            t
-00014410: 7970 653a 206f 6e65 206f 6620 2278 7922  ype: one of "xy"
-00014420: 2c20 2275 7a22 2c20 6f72 2022 3344 222e  , "uz", or "3D".
-00014430: 2044 6574 6572 6d69 6e65 7320 7468 6520   Determines the 
-00014440: 7479 7065 206f 6620 6d65 7368 2074 6f20  type of mesh to 
-00014450: 7265 7475 726e 2e0a 2020 2020 2020 2020  return..        
-00014460: 2020 2020 7a3a 2075 7365 6420 746f 2064      z: used to d
-00014470: 6566 696e 6520 7a2d 736c 6963 6520 666f  efine z-slice fo
-00014480: 7220 7879 206d 6573 6869 6e67 0a20 2020  r xy meshing.   
-00014490: 2020 2020 2020 2020 2078 7365 6374 696f           xsectio
-000144a0: 6e5f 626f 756e 6473 3a20 7573 6564 2074  n_bounds: used t
-000144b0: 6f20 6465 6669 6e65 2069 6e2d 706c 616e  o define in-plan
-000144c0: 6520 6c69 6e65 2066 6f72 2075 7a20 6d65  e line for uz me
-000144d0: 7368 696e 670a 2020 2020 2020 2020 2020  shing.          
-000144e0: 2020 7761 6665 725f 7061 6464 696e 673a    wafer_padding:
-000144f0: 2070 6164 6469 6e67 2062 6579 6f6e 6420   padding beyond 
-00014500: 6262 6f78 2074 6f20 6164 6420 746f 2057  bbox to add to W
-00014510: 4146 4552 206c 6179 6572 732e 0a0a 2020  AFER layers...  
-00014520: 2020 2020 2020 4b65 7977 6f72 6420 4172        Keyword Ar
-00014530: 6773 3a0a 2020 2020 2020 2020 2020 2020  gs:.            
-00014540: 4172 6775 6d65 6e74 7320 666f 7220 7468  Arguments for th
-00014550: 6520 7461 7267 6574 206d 6573 6869 6e67  e target meshing
-00014560: 2066 756e 6374 696f 6e20 696e 2067 6473   function in gds
-00014570: 6661 6374 6f72 792e 7369 6d75 6c61 7469  factory.simulati
-00014580: 6f6e 2e67 6d73 680a 2020 2020 2020 2020  on.gmsh.        
-00014590: 2222 220a 2020 2020 2020 2020 2320 4164  """.        # Ad
-000145a0: 6420 5741 4645 5220 6c61 7965 723a 0a20  d WAFER layer:. 
-000145b0: 2020 2020 2020 2070 6164 6465 645f 636f         padded_co
-000145c0: 6d70 6f6e 656e 7420 3d20 436f 6d70 6f6e  mponent = Compon
-000145d0: 656e 7428 290a 2020 2020 2020 2020 7061  ent().        pa
-000145e0: 6464 6564 5f63 6f6d 706f 6e65 6e74 203c  dded_component <
-000145f0: 3c20 7365 6c66 0a20 2020 2020 2020 2028  < self.        (
-00014600: 786d 696e 2c20 796d 696e 292c 2028 786d  xmin, ymin), (xm
-00014610: 6178 2c20 796d 6178 2920 3d20 7365 6c66  ax, ymax) = self
-00014620: 2e62 626f 780a 2020 2020 2020 2020 706f  .bbox.        po
-00014630: 696e 7473 203d 205b 0a20 2020 2020 2020  ints = [.       
-00014640: 2020 2020 205b 786d 696e 202d 2077 6166       [xmin - waf
-00014650: 6572 5f70 6164 6469 6e67 2c20 796d 696e  er_padding, ymin
-00014660: 202d 2077 6166 6572 5f70 6164 6469 6e67   - wafer_padding
-00014670: 5d2c 0a20 2020 2020 2020 2020 2020 205b  ],.            [
-00014680: 786d 6178 202b 2077 6166 6572 5f70 6164  xmax + wafer_pad
-00014690: 6469 6e67 2c20 796d 696e 202d 2077 6166  ding, ymin - waf
-000146a0: 6572 5f70 6164 6469 6e67 5d2c 0a20 2020  er_padding],.   
-000146b0: 2020 2020 2020 2020 205b 786d 6178 202b           [xmax +
-000146c0: 2077 6166 6572 5f70 6164 6469 6e67 2c20   wafer_padding, 
-000146d0: 796d 6178 202b 2077 6166 6572 5f70 6164  ymax + wafer_pad
-000146e0: 6469 6e67 5d2c 0a20 2020 2020 2020 2020  ding],.         
-000146f0: 2020 205b 786d 696e 202d 2077 6166 6572     [xmin - wafer
-00014700: 5f70 6164 6469 6e67 2c20 796d 6178 202b  _padding, ymax +
-00014710: 2077 6166 6572 5f70 6164 6469 6e67 5d2c   wafer_padding],
-00014720: 0a20 2020 2020 2020 205d 0a20 2020 2020  .        ].     
-00014730: 2020 2070 6164 6465 645f 636f 6d70 6f6e     padded_compon
-00014740: 656e 742e 6164 645f 706f 6c79 676f 6e28  ent.add_polygon(
-00014750: 706f 696e 7473 2c20 6c61 7965 723d 7761  points, layer=wa
-00014760: 6665 725f 6c61 7965 7229 0a0a 2020 2020  fer_layer)..    
-00014770: 2020 2020 6966 206c 6179 6572 5f73 7461      if layer_sta
-00014780: 636b 2069 7320 4e6f 6e65 3a0a 2020 2020  ck is None:.    
-00014790: 2020 2020 2020 2020 7261 6973 6520 5661          raise Va
-000147a0: 6c75 6545 7272 6f72 280a 2020 2020 2020  lueError(.      
-000147b0: 2020 2020 2020 2020 2020 2741 204c 6179            'A Lay
-000147c0: 6572 5374 6163 6b20 6d75 7374 2062 6520  erStack must be 
-000147d0: 7072 6f76 6964 6564 2074 6872 6f75 6768  provided through
-000147e0: 2061 7267 756d 656e 7420 226c 6179 6572   argument "layer
-000147f0: 5f73 7461 636b 222e 270a 2020 2020 2020  _stack".'.      
-00014800: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-00014810: 6966 2074 7970 6520 3d3d 2022 7879 223a  if type == "xy":
-00014820: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00014830: 7a20 6973 204e 6f6e 653a 0a20 2020 2020  z is None:.     
-00014840: 2020 2020 2020 2020 2020 2072 6169 7365             raise
-00014850: 2056 616c 7565 4572 726f 7228 0a20 2020   ValueError(.   
-00014860: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014870: 2027 466f 7220 7879 2d6d 6573 6869 6e67   'For xy-meshing
-00014880: 2c20 6120 7a2d 7661 6c75 6520 6d75 7374  , a z-value must
-00014890: 2062 6520 7072 6f76 6964 6564 2076 6961   be provided via
-000148a0: 2074 6865 2066 6c6f 6174 2061 7267 756d   the float argum
-000148b0: 656e 7420 227a 222e 270a 2020 2020 2020  ent "z".'.      
-000148c0: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-000148d0: 2020 2020 2020 2020 6672 6f6d 2067 6473          from gds
-000148e0: 6661 6374 6f72 792e 7369 6d75 6c61 7469  factory.simulati
-000148f0: 6f6e 2e67 6d73 682e 7879 5f78 7365 6374  on.gmsh.xy_xsect
-00014900: 696f 6e5f 6d65 7368 2069 6d70 6f72 7420  ion_mesh import 
-00014910: 7879 5f78 7365 6374 696f 6e5f 6d65 7368  xy_xsection_mesh
-00014920: 0a0a 2020 2020 2020 2020 2020 2020 7265  ..            re
-00014930: 7475 726e 2078 795f 7873 6563 7469 6f6e  turn xy_xsection
-00014940: 5f6d 6573 6828 7061 6464 6564 5f63 6f6d  _mesh(padded_com
-00014950: 706f 6e65 6e74 2c20 7a2c 206c 6179 6572  ponent, z, layer
-00014960: 5f73 7461 636b 2c20 2a2a 6b77 6172 6773  _stack, **kwargs
-00014970: 290a 2020 2020 2020 2020 656c 6966 2074  ).        elif t
-00014980: 7970 6520 3d3d 2022 757a 223a 0a20 2020  ype == "uz":.   
-00014990: 2020 2020 2020 2020 2069 6620 7873 6563           if xsec
-000149a0: 7469 6f6e 5f62 6f75 6e64 7320 6973 204e  tion_bounds is N
-000149b0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-000149c0: 2020 2020 2072 6169 7365 2056 616c 7565       raise Value
-000149d0: 4572 726f 7228 0a20 2020 2020 2020 2020  Error(.         
-000149e0: 2020 2020 2020 2020 2020 2022 466f 7220             "For 
-000149f0: 757a 2d6d 6573 6869 6e67 2c20 796f 7520  uz-meshing, you 
-00014a00: 6d75 7374 2070 726f 7669 6465 2061 206c  must provide a l
-00014a10: 696e 6520 696e 2074 6865 2078 792d 706c  ine in the xy-pl
-00014a20: 616e 6520 220a 2020 2020 2020 2020 2020  ane ".          
-00014a30: 2020 2020 2020 2020 2020 2276 6961 2074            "via t
-00014a40: 6865 2054 7570 6c65 2061 7267 756d 656e  he Tuple argumen
-00014a50: 7420 5b5b 7831 2c79 315d 2c20 5b78 322c  t [[x1,y1], [x2,
-00014a60: 7932 5d5d 2078 7365 6374 696f 6e5f 626f  y2]] xsection_bo
-00014a70: 756e 6473 2e22 0a20 2020 2020 2020 2020  unds.".         
-00014a80: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-00014a90: 2020 2020 2066 726f 6d20 6764 7366 6163       from gdsfac
-00014aa0: 746f 7279 2e73 696d 756c 6174 696f 6e2e  tory.simulation.
-00014ab0: 676d 7368 2e75 7a5f 7873 6563 7469 6f6e  gmsh.uz_xsection
-00014ac0: 5f6d 6573 6820 696d 706f 7274 2075 7a5f  _mesh import uz_
-00014ad0: 7873 6563 7469 6f6e 5f6d 6573 680a 0a20  xsection_mesh.. 
-00014ae0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00014af0: 6e20 757a 5f78 7365 6374 696f 6e5f 6d65  n uz_xsection_me
-00014b00: 7368 280a 2020 2020 2020 2020 2020 2020  sh(.            
-00014b10: 2020 2020 7061 6464 6564 5f63 6f6d 706f      padded_compo
-00014b20: 6e65 6e74 2c20 7873 6563 7469 6f6e 5f62  nent, xsection_b
-00014b30: 6f75 6e64 732c 206c 6179 6572 5f73 7461  ounds, layer_sta
-00014b40: 636b 2c20 2a2a 6b77 6172 6773 0a20 2020  ck, **kwargs.   
-00014b50: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
-00014b60: 2020 2065 6c69 6620 7479 7065 203d 3d20     elif type == 
-00014b70: 2233 4422 3a0a 2020 2020 2020 2020 2020  "3D":.          
-00014b80: 2020 6672 6f6d 2067 6473 6661 6374 6f72    from gdsfactor
-00014b90: 792e 7369 6d75 6c61 7469 6f6e 2e67 6d73  y.simulation.gms
-00014ba0: 682e 7879 7a5f 6d65 7368 2069 6d70 6f72  h.xyz_mesh impor
-00014bb0: 7420 7879 7a5f 6d65 7368 0a0a 2020 2020  t xyz_mesh..    
-00014bc0: 2020 2020 2020 2020 7265 7475 726e 2078          return x
-00014bd0: 797a 5f6d 6573 6828 7061 6464 6564 5f63  yz_mesh(padded_c
-00014be0: 6f6d 706f 6e65 6e74 2c20 6c61 7965 725f  omponent, layer_
-00014bf0: 7374 6163 6b2c 202a 2a6b 7761 7267 7329  stack, **kwargs)
-00014c00: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
-00014c10: 2020 2020 2020 2020 2020 2072 6169 7365             raise
-00014c20: 2056 616c 7565 4572 726f 7228 0a20 2020   ValueError(.   
-00014c30: 2020 2020 2020 2020 2020 2020 2027 5265               'Re
-00014c40: 7175 6972 6564 2061 7267 756d 656e 7420  quired argument 
-00014c50: 2274 7970 6522 206d 7573 7420 6265 206f  "type" must be o
-00014c60: 6e65 206f 6620 2278 7922 2c20 2275 7a22  ne of "xy", "uz"
-00014c70: 2c20 6f72 2022 3344 222e 270a 2020 2020  , or "3D".'.    
-00014c80: 2020 2020 2020 2020 290a 0a20 2020 2064          )..    d
-00014c90: 6566 206f 6666 7365 7428 0a20 2020 2020  ef offset(.     
-00014ca0: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
-00014cb0: 2064 6973 7461 6e63 653a 2066 6c6f 6174   distance: float
-00014cc0: 203d 2030 2e31 2c0a 2020 2020 2020 2020   = 0.1,.        
-00014cd0: 706f 6c79 676f 6e73 3d4e 6f6e 652c 0a20  polygons=None,. 
-00014ce0: 2020 2020 2020 2075 7365 5f75 6e69 6f6e         use_union
-00014cf0: 3a20 626f 6f6c 203d 2054 7275 652c 0a20  : bool = True,. 
-00014d00: 2020 2020 2020 2070 7265 6369 7369 6f6e         precision
-00014d10: 3a20 666c 6f61 7420 3d20 3165 2d34 2c0a  : float = 1e-4,.
-00014d20: 2020 2020 2020 2020 6a6f 696e 3a20 7374          join: st
-00014d30: 7220 3d20 226d 6974 6572 222c 0a20 2020  r = "miter",.   
-00014d40: 2020 2020 2074 6f6c 6572 616e 6365 3a20       tolerance: 
-00014d50: 696e 7420 3d20 322c 0a20 2020 2020 2020  int = 2,.       
-00014d60: 206c 6179 6572 3a20 4c61 7965 7253 7065   layer: LayerSpe
-00014d70: 6320 3d20 2257 4722 2c0a 2020 2020 2920  c = "WG",.    ) 
-00014d80: 2d3e 2043 6f6d 706f 6e65 6e74 3a0a 2020  -> Component:.  
-00014d90: 2020 2020 2020 2222 2252 6574 7572 6e73        """Returns
-00014da0: 206e 6577 2043 6f6d 706f 6e65 6e74 2077   new Component w
-00014db0: 6974 6820 706f 6c79 676f 6e73 2065 726f  ith polygons ero
-00014dc0: 6465 6420 6f72 2064 696c 6174 6564 2062  ded or dilated b
-00014dd0: 7920 616e 206f 6666 7365 742e 0a0a 2020  y an offset...  
-00014de0: 2020 2020 2020 4172 6773 3a0a 2020 2020        Args:.    
-00014df0: 2020 2020 2020 2020 6469 7374 616e 6365          distance
-00014e00: 3a20 4469 7374 616e 6365 2074 6f20 6f66  : Distance to of
-00014e10: 6673 6574 2070 6f6c 7967 6f6e 732e 2050  fset polygons. P
-00014e20: 6f73 6974 6976 6520 7661 6c75 6573 2065  ositive values e
-00014e30: 7870 616e 642c 206e 6567 6174 6976 6520  xpand, negative 
-00014e40: 7368 7269 6e6b 2e0a 2020 2020 2020 2020  shrink..        
-00014e50: 2020 2020 7072 6563 6973 696f 6e3a 2044      precision: D
-00014e60: 6573 6972 6564 2070 7265 6369 7369 6f6e  esired precision
-00014e70: 2066 6f72 2072 6f75 6e64 696e 6720 7665   for rounding ve
-00014e80: 7274 6578 2063 6f6f 7264 696e 6174 6573  rtex coordinates
-00014e90: 2e0a 2020 2020 2020 2020 2020 2020 6a6f  ..            jo
-00014ea0: 696e 3a20 7b27 6d69 7465 7227 2c20 2762  in: {'miter', 'b
-00014eb0: 6576 656c 272c 2027 726f 756e 6427 7d20  evel', 'round'} 
-00014ec0: 5479 7065 206f 6620 6a6f 696e 2075 7365  Type of join use
-00014ed0: 6420 746f 2063 7265 6174 6520 706f 6c79  d to create poly
-00014ee0: 676f 6e20 6f66 6673 6574 0a20 2020 2020  gon offset.     
-00014ef0: 2020 2020 2020 2074 6f6c 6572 616e 6365         tolerance
-00014f00: 3a20 466f 7220 6d69 7465 7220 6a6f 696e  : For miter join
-00014f10: 7473 2c20 7468 6973 206e 756d 6265 7220  ts, this number 
-00014f20: 6d75 7374 2062 6520 6174 206c 6561 7374  must be at least
-00014f30: 2032 2072 6570 7265 7365 6e74 7320 7468   2 represents th
-00014f40: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
-00014f50: 6d61 7869 6d61 6c20 6469 7374 616e 6365  maximal distance
-00014f60: 2069 6e20 6d75 6c74 6970 6c65 7320 6f66   in multiples of
-00014f70: 206f 6666 7365 7420 6265 7477 6565 6e20   offset between 
-00014f80: 6e65 7720 7665 7274 6963 6573 2061 6e64  new vertices and
-00014f90: 2074 6865 6972 0a20 2020 2020 2020 2020   their.         
-00014fa0: 2020 2020 206f 7269 6769 6e61 6c20 706f       original po
-00014fb0: 7369 7469 6f6e 2062 6566 6f72 6520 6265  sition before be
-00014fc0: 7665 6c69 6e67 2074 6f20 6176 6f69 6420  veling to avoid 
-00014fd0: 7370 696b 6573 2061 7420 6163 7574 6520  spikes at acute 
-00014fe0: 6a6f 696e 7473 2e20 466f 720a 2020 2020  joints. For.    
-00014ff0: 2020 2020 2020 2020 2020 726f 756e 6420            round 
-00015000: 6a6f 696e 7473 2c20 6974 2069 6e64 6963  joints, it indic
-00015010: 6174 6573 2074 6865 2063 7572 7661 7475  ates the curvatu
-00015020: 7265 2072 6573 6f6c 7574 696f 6e20 696e  re resolution in
-00015030: 206e 756d 6265 7220 6f66 0a20 2020 2020   number of.     
-00015040: 2020 2020 2020 2020 2070 6f69 6e74 7320           points 
-00015050: 7065 7220 6675 6c6c 2063 6972 636c 652e  per full circle.
-00015060: 0a20 2020 2020 2020 2020 2020 206c 6179  .            lay
-00015070: 6572 3a20 5370 6563 6966 6963 206c 6179  er: Specific lay
-00015080: 6572 2066 6f72 206e 6577 2070 6f6c 7967  er for new polyg
-00015090: 6f6e 732e 0a0a 2020 2020 2020 2020 2222  ons...        ""
-000150a0: 220a 2020 2020 2020 2020 696d 706f 7274  ".        import
-000150b0: 2067 6473 6661 6374 6f72 7920 6173 2067   gdsfactory as g
-000150c0: 660a 0a20 2020 2020 2020 2067 6473 5f6c  f..        gds_l
-000150d0: 6179 6572 2c20 6764 735f 6461 7461 7479  ayer, gds_dataty
-000150e0: 7065 203d 2067 662e 6765 745f 6c61 7965  pe = gf.get_laye
-000150f0: 7228 6c61 7965 7229 0a20 2020 2020 2020  r(layer).       
-00015100: 2070 203d 2067 6473 746b 2e6f 6666 7365   p = gdstk.offse
-00015110: 7428 0a20 2020 2020 2020 2020 2020 2070  t(.            p
-00015120: 6f6c 7967 6f6e 7320 6f72 2073 656c 662e  olygons or self.
-00015130: 6765 745f 706f 6c79 676f 6e73 2829 2c0a  get_polygons(),.
-00015140: 2020 2020 2020 2020 2020 2020 6469 7374              dist
-00015150: 616e 6365 3d64 6973 7461 6e63 652c 0a20  ance=distance,. 
-00015160: 2020 2020 2020 2020 2020 206a 6f69 6e3d             join=
-00015170: 6a6f 696e 2c0a 2020 2020 2020 2020 2020  join,.          
-00015180: 2020 746f 6c65 7261 6e63 653d 746f 6c65    tolerance=tole
-00015190: 7261 6e63 652c 0a20 2020 2020 2020 2020  rance,.         
-000151a0: 2020 2070 7265 6369 7369 6f6e 3d70 7265     precision=pre
-000151b0: 6369 7369 6f6e 2c0a 2020 2020 2020 2020  cision,.        
-000151c0: 2020 2020 7573 655f 756e 696f 6e3d 7573      use_union=us
-000151d0: 655f 756e 696f 6e2c 0a20 2020 2020 2020  e_union,.       
-000151e0: 2020 2020 206c 6179 6572 3d67 6473 5f6c       layer=gds_l
-000151f0: 6179 6572 2c0a 2020 2020 2020 2020 2020  ayer,.          
-00015200: 2020 6461 7461 7479 7065 3d67 6473 5f64    datatype=gds_d
-00015210: 6174 6174 7970 652c 0a20 2020 2020 2020  atatype,.       
-00015220: 2029 0a0a 2020 2020 2020 2020 636f 6d70   )..        comp
-00015230: 6f6e 656e 7420 3d20 6766 2e43 6f6d 706f  onent = gf.Compo
-00015240: 6e65 6e74 2829 0a20 2020 2020 2020 2063  nent().        c
-00015250: 6f6d 706f 6e65 6e74 2e61 6464 5f70 6f6c  omponent.add_pol
-00015260: 7967 6f6e 2870 2c20 6c61 7965 723d 6c61  ygon(p, layer=la
-00015270: 7965 7229 0a20 2020 2020 2020 2072 6574  yer).        ret
-00015280: 7572 6e20 636f 6d70 6f6e 656e 740a 0a0a  urn component...
-00015290: 6465 6620 636f 7079 280a 2020 2020 443a  def copy(.    D:
-000152a0: 2043 6f6d 706f 6e65 6e74 2c0a 2020 2020   Component,.    
-000152b0: 7265 6665 7265 6e63 6573 3d4e 6f6e 652c  references=None,
-000152c0: 0a20 2020 2070 6f72 7473 3d4e 6f6e 652c  .    ports=None,
-000152d0: 0a20 2020 2070 6f6c 7967 6f6e 733d 4e6f  .    polygons=No
-000152e0: 6e65 2c0a 2020 2020 7061 7468 733d 4e6f  ne,.    paths=No
-000152f0: 6e65 2c0a 2020 2020 6e61 6d65 3d4e 6f6e  ne,.    name=Non
-00015300: 652c 0a20 2020 206c 6162 656c 733d 4e6f  e,.    labels=No
-00015310: 6e65 2c0a 2920 2d3e 2043 6f6d 706f 6e65  ne,.) -> Compone
-00015320: 6e74 3a0a 2020 2020 2222 2252 6574 7572  nt:.    """Retur
-00015330: 6e73 2061 2043 6f6d 706f 6e65 6e74 2063  ns a Component c
-00015340: 6f70 792e 0a0a 2020 2020 4172 6773 3a0a  opy...    Args:.
-00015350: 2020 2020 2020 2020 443a 2063 6f6d 706f          D: compo
-00015360: 6e65 6e74 2074 6f20 636f 7079 2e0a 2020  nent to copy..  
-00015370: 2020 2222 220a 2020 2020 445f 636f 7079    """.    D_copy
-00015380: 203d 2043 6f6d 706f 6e65 6e74 2829 0a20   = Component(). 
-00015390: 2020 2044 5f63 6f70 792e 696e 666f 203d     D_copy.info =
-000153a0: 2044 2e69 6e66 6f0a 2020 2020 2320 445f   D.info.    # D_
-000153b0: 636f 7079 2e5f 6365 6c6c 203d 2044 2e5f  copy._cell = D._
-000153c0: 6365 6c6c 2e63 6f70 7928 6e61 6d65 3d44  cell.copy(name=D
-000153d0: 5f63 6f70 792e 6e61 6d65 290a 0a20 2020  _copy.name)..   
-000153e0: 2066 6f72 2072 6566 2069 6e20 7265 6665   for ref in refe
-000153f0: 7265 6e63 6573 2069 6620 7265 6665 7265  rences if refere
-00015400: 6e63 6573 2069 7320 6e6f 7420 4e6f 6e65  nces is not None
-00015410: 2065 6c73 6520 442e 7265 6665 7265 6e63   else D.referenc
-00015420: 6573 3a0a 2020 2020 2020 2020 445f 636f  es:.        D_co
-00015430: 7079 2e61 6464 2863 6f70 795f 7265 6665  py.add(copy_refe
-00015440: 7265 6e63 6528 7265 6629 290a 2020 2020  rence(ref)).    
-00015450: 666f 7220 706f 7274 2069 6e20 2870 6f72  for port in (por
-00015460: 7473 2069 6620 706f 7274 7320 6973 206e  ts if ports is n
-00015470: 6f74 204e 6f6e 6520 656c 7365 2044 2e70  ot None else D.p
-00015480: 6f72 7473 292e 7661 6c75 6573 2829 3a0a  orts).values():.
-00015490: 2020 2020 2020 2020 445f 636f 7079 2e61          D_copy.a
-000154a0: 6464 5f70 6f72 7428 706f 7274 3d70 6f72  dd_port(port=por
-000154b0: 7429 0a20 2020 2066 6f72 2070 6f6c 7920  t).    for poly 
-000154c0: 696e 2070 6f6c 7967 6f6e 7320 6966 2070  in polygons if p
-000154d0: 6f6c 7967 6f6e 7320 6973 206e 6f74 204e  olygons is not N
-000154e0: 6f6e 6520 656c 7365 2044 2e70 6f6c 7967  one else D.polyg
-000154f0: 6f6e 733a 0a20 2020 2020 2020 2044 5f63  ons:.        D_c
-00015500: 6f70 792e 6164 645f 706f 6c79 676f 6e28  opy.add_polygon(
-00015510: 706f 6c79 290a 2020 2020 666f 7220 7061  poly).    for pa
-00015520: 7468 2069 6e20 7061 7468 7320 6966 2070  th in paths if p
-00015530: 6174 6873 2069 7320 6e6f 7420 4e6f 6e65  aths is not None
-00015540: 2065 6c73 6520 442e 7061 7468 733a 0a20   else D.paths:. 
-00015550: 2020 2020 2020 2044 5f63 6f70 792e 6164         D_copy.ad
-00015560: 6428 7061 7468 290a 2020 2020 666f 7220  d(path).    for 
-00015570: 6c61 6265 6c20 696e 206c 6162 656c 7320  label in labels 
-00015580: 6966 206c 6162 656c 7320 6973 206e 6f74  if labels is not
-00015590: 204e 6f6e 6520 656c 7365 2044 2e6c 6162   None else D.lab
-000155a0: 656c 733a 0a20 2020 2020 2020 2044 5f63  els:.        D_c
-000155b0: 6f70 792e 6164 645f 6c61 6265 6c28 0a20  opy.add_label(. 
-000155c0: 2020 2020 2020 2020 2020 2074 6578 743d             text=
-000155d0: 6c61 6265 6c2e 7465 7874 2c0a 2020 2020  label.text,.    
-000155e0: 2020 2020 2020 2020 706f 7369 7469 6f6e          position
-000155f0: 3d6c 6162 656c 2e6f 7269 6769 6e2c 0a20  =label.origin,. 
-00015600: 2020 2020 2020 2020 2020 206c 6179 6572             layer
-00015610: 3d28 6c61 6265 6c2e 6c61 7965 722c 206c  =(label.layer, l
-00015620: 6162 656c 2e74 6578 7474 7970 6529 2c0a  abel.texttype),.
-00015630: 2020 2020 2020 2020 290a 0a20 2020 2069          )..    i
-00015640: 6620 6e61 6d65 2069 7320 6e6f 7420 4e6f  f name is not No
-00015650: 6e65 3a0a 2020 2020 2020 2020 445f 636f  ne:.        D_co
-00015660: 7079 2e6e 616d 6520 3d20 6e61 6d65 0a0a  py.name = name..
-00015670: 2020 2020 7265 7475 726e 2044 5f63 6f70      return D_cop
-00015680: 790a 0a0a 6465 6620 636f 7079 5f72 6566  y...def copy_ref
-00015690: 6572 656e 6365 280a 2020 2020 7265 662c  erence(.    ref,
-000156a0: 0a20 2020 2070 6172 656e 743d 4e6f 6e65  .    parent=None
-000156b0: 2c0a 2020 2020 636f 6c75 6d6e 733d 4e6f  ,.    columns=No
-000156c0: 6e65 2c0a 2020 2020 726f 7773 3d4e 6f6e  ne,.    rows=Non
-000156d0: 652c 0a20 2020 2073 7061 6369 6e67 3d4e  e,.    spacing=N
-000156e0: 6f6e 652c 0a20 2020 206f 7269 6769 6e3d  one,.    origin=
-000156f0: 4e6f 6e65 2c0a 2020 2020 726f 7461 7469  None,.    rotati
-00015700: 6f6e 3d4e 6f6e 652c 0a20 2020 206d 6167  on=None,.    mag
-00015710: 6e69 6669 6361 7469 6f6e 3d4e 6f6e 652c  nification=None,
-00015720: 0a20 2020 2078 5f72 6566 6c65 6374 696f  .    x_reflectio
-00015730: 6e3d 4e6f 6e65 2c0a 2020 2020 6e61 6d65  n=None,.    name
-00015740: 3d4e 6f6e 652c 0a20 2020 2076 313d 4e6f  =None,.    v1=No
-00015750: 6e65 2c0a 2020 2020 7632 3d4e 6f6e 652c  ne,.    v2=None,
-00015760: 0a29 202d 3e20 436f 6d70 6f6e 656e 7452  .) -> ComponentR
-00015770: 6566 6572 656e 6365 3a0a 2020 2020 7265  eference:.    re
-00015780: 7475 726e 2043 6f6d 706f 6e65 6e74 5265  turn ComponentRe
-00015790: 6665 7265 6e63 6528 0a20 2020 2020 2020  ference(.       
-000157a0: 2063 6f6d 706f 6e65 6e74 3d70 6172 656e   component=paren
-000157b0: 7420 6f72 2072 6566 2e70 6172 656e 742c  t or ref.parent,
-000157c0: 0a20 2020 2020 2020 2063 6f6c 756d 6e73  .        columns
-000157d0: 3d63 6f6c 756d 6e73 206f 7220 7265 662e  =columns or ref.
-000157e0: 636f 6c75 6d6e 732c 0a20 2020 2020 2020  columns,.       
-000157f0: 2072 6f77 733d 726f 7773 206f 7220 7265   rows=rows or re
-00015800: 662e 726f 7773 2c0a 2020 2020 2020 2020  f.rows,.        
-00015810: 7370 6163 696e 673d 7370 6163 696e 6720  spacing=spacing 
-00015820: 6f72 2072 6566 2e73 7061 6369 6e67 2c0a  or ref.spacing,.
-00015830: 2020 2020 2020 2020 6f72 6967 696e 3d6f          origin=o
-00015840: 7269 6769 6e20 6f72 2072 6566 2e6f 7269  rigin or ref.ori
-00015850: 6769 6e2c 0a20 2020 2020 2020 2072 6f74  gin,.        rot
-00015860: 6174 696f 6e3d 726f 7461 7469 6f6e 206f  ation=rotation o
-00015870: 7220 7265 662e 726f 7461 7469 6f6e 2c0a  r ref.rotation,.
-00015880: 2020 2020 2020 2020 6d61 676e 6966 6963          magnific
-00015890: 6174 696f 6e3d 6d61 676e 6966 6963 6174  ation=magnificat
-000158a0: 696f 6e20 6f72 2072 6566 2e6d 6167 6e69  ion or ref.magni
-000158b0: 6669 6361 7469 6f6e 2c0a 2020 2020 2020  fication,.      
-000158c0: 2020 785f 7265 666c 6563 7469 6f6e 3d78    x_reflection=x
-000158d0: 5f72 6566 6c65 6374 696f 6e20 6f72 2072  _reflection or r
-000158e0: 6566 2e78 5f72 6566 6c65 6374 696f 6e2c  ef.x_reflection,
-000158f0: 0a20 2020 2020 2020 206e 616d 653d 6e61  .        name=na
-00015900: 6d65 206f 7220 7265 662e 6e61 6d65 2c0a  me or ref.name,.
-00015910: 2020 2020 2020 2020 7631 3d76 3120 6f72          v1=v1 or
-00015920: 2072 6566 2e76 312c 0a20 2020 2020 2020   ref.v1,.       
-00015930: 2076 323d 7632 206f 7220 7265 662e 7632   v2=v2 or ref.v2
-00015940: 2c0a 2020 2020 290a 0a0a 6465 6620 7465  ,.    )...def te
-00015950: 7374 5f67 6574 5f6c 6179 6572 7328 2920  st_get_layers() 
-00015960: 2d3e 2043 6f6d 706f 6e65 6e74 3a0a 2020  -> Component:.  
-00015970: 2020 696d 706f 7274 2067 6473 6661 6374    import gdsfact
-00015980: 6f72 7920 6173 2067 660a 0a20 2020 2063  ory as gf..    c
-00015990: 3120 3d20 6766 2e63 6f6d 706f 6e65 6e74  1 = gf.component
-000159a0: 732e 7374 7261 6967 6874 280a 2020 2020  s.straight(.    
-000159b0: 2020 2020 6c65 6e67 7468 3d31 302c 0a20      length=10,. 
-000159c0: 2020 2020 2020 2077 6964 7468 3d30 2e35         width=0.5
-000159d0: 2c0a 2020 2020 2020 2020 6c61 7965 723d  ,.        layer=
-000159e0: 2832 2c20 3029 2c0a 2020 2020 2020 2020  (2, 0),.        
-000159f0: 6262 6f78 5f6c 6179 6572 733d 5b28 3131  bbox_layers=[(11
-00015a00: 312c 2030 295d 2c0a 2020 2020 2020 2020  1, 0)],.        
-00015a10: 6262 6f78 5f6f 6666 7365 7473 3d5b 335d  bbox_offsets=[3]
-00015a20: 2c0a 2020 2020 2020 2020 7769 7468 5f62  ,.        with_b
-00015a30: 626f 783d 5472 7565 2c0a 2020 2020 2020  box=True,.      
-00015a40: 2020 636c 6164 6469 6e67 5f6c 6179 6572    cladding_layer
-00015a50: 733d 4e6f 6e65 2c0a 2020 2020 2020 2020  s=None,.        
-00015a60: 6164 645f 7069 6e73 3d4e 6f6e 652c 0a20  add_pins=None,. 
-00015a70: 2020 2020 2020 2061 6464 5f62 626f 783d         add_bbox=
-00015a80: 4e6f 6e65 2c0a 2020 2020 290a 2020 2020  None,.    ).    
-00015a90: 6173 7365 7274 2063 312e 6765 745f 6c61  assert c1.get_la
-00015aa0: 7965 7273 2829 203d 3d20 7b28 322c 2030  yers() == {(2, 0
-00015ab0: 292c 2028 3131 312c 2030 297d 2c20 6331  ), (111, 0)}, c1
-00015ac0: 2e67 6574 5f6c 6179 6572 7328 290a 2020  .get_layers().  
-00015ad0: 2020 2320 7265 7475 726e 2063 310a 2020    # return c1.  
-00015ae0: 2020 6332 203d 2063 312e 7265 6d6f 7665    c2 = c1.remove
-00015af0: 5f6c 6179 6572 7328 5b28 3131 312c 2030  _layers([(111, 0
-00015b00: 295d 290a 2020 2020 6173 7365 7274 2063  )]).    assert c
-00015b10: 322e 6765 745f 6c61 7965 7273 2829 203d  2.get_layers() =
-00015b20: 3d20 7b28 322c 2030 297d 2c20 6332 2e67  = {(2, 0)}, c2.g
-00015b30: 6574 5f6c 6179 6572 7328 290a 2020 2020  et_layers().    
-00015b40: 7265 7475 726e 2063 320a 0a0a 6465 6620  return c2...def 
-00015b50: 5f66 696c 7465 725f 706f 6c79 7328 706f  _filter_polys(po
-00015b60: 6c79 676f 6e73 2c20 6c61 7965 7273 5f65  lygons, layers_e
-00015b70: 7863 6c29 3a0a 2020 2020 7265 7475 726e  xcl):.    return
-00015b80: 205b 0a20 2020 2020 2020 2070 6f6c 7967   [.        polyg
-00015b90: 6f6e 0a20 2020 2020 2020 2066 6f72 2070  on.        for p
-00015ba0: 6f6c 7967 6f6e 2c20 6c61 7965 722c 2064  olygon, layer, d
-00015bb0: 6174 6174 7970 6520 696e 207a 6970 280a  atatype in zip(.
-00015bc0: 2020 2020 2020 2020 2020 2020 706f 6c79              poly
-00015bd0: 676f 6e73 2e70 6f6c 7967 6f6e 732c 2070  gons.polygons, p
-00015be0: 6f6c 7967 6f6e 732e 6c61 7965 7273 2c20  olygons.layers, 
-00015bf0: 706f 6c79 676f 6e73 2e64 6174 6174 7970  polygons.datatyp
-00015c00: 6573 0a20 2020 2020 2020 2029 0a20 2020  es.        ).   
-00015c10: 2020 2020 2069 6620 286c 6179 6572 2c20       if (layer, 
-00015c20: 6461 7461 7479 7065 2920 6e6f 7420 696e  datatype) not in
-00015c30: 206c 6179 6572 735f 6578 636c 0a20 2020   layers_excl.   
-00015c40: 205d 0a0a 0a64 6566 2072 6563 7572 7365   ]...def recurse
-00015c50: 5f73 7472 7563 7475 7265 7328 0a20 2020  _structures(.   
-00015c60: 2063 6f6d 706f 6e65 6e74 3a20 436f 6d70   component: Comp
-00015c70: 6f6e 656e 742c 0a20 2020 2069 676e 6f72  onent,.    ignor
-00015c80: 655f 636f 6d70 6f6e 656e 7473 5f70 7265  e_components_pre
-00015c90: 6669 783a 204f 7074 696f 6e61 6c5b 4c69  fix: Optional[Li
-00015ca0: 7374 5b73 7472 5d5d 203d 204e 6f6e 652c  st[str]] = None,
-00015cb0: 0a20 2020 2069 676e 6f72 655f 6675 6e63  .    ignore_func
-00015cc0: 7469 6f6e 735f 7072 6566 6978 3a20 4f70  tions_prefix: Op
-00015cd0: 7469 6f6e 616c 5b4c 6973 745b 7374 725d  tional[List[str]
-00015ce0: 5d20 3d20 4e6f 6e65 2c0a 2920 2d3e 2044  ] = None,.) -> D
-00015cf0: 6963 745b 7374 722c 2041 6e79 5d3a 0a20  ict[str, Any]:. 
-00015d00: 2020 2022 2222 5265 6375 7273 6520 636f     """Recurse co
-00015d10: 6d70 6f6e 656e 7420 616e 6420 636f 6d70  mponent and comp
-00015d20: 6f6e 656e 7473 2072 6566 6572 656e 6365  onents reference
-00015d30: 7320 7265 6375 7273 6976 656c 792e 0a0a  s recursively...
-00015d40: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
-00015d50: 2020 636f 6d70 6f6e 656e 743a 2063 6f6d    component: com
-00015d60: 706f 6e65 6e74 2074 6f20 7265 6375 7273  ponent to recurs
-00015d70: 652e 0a20 2020 2020 2020 2069 676e 6f72  e..        ignor
-00015d80: 655f 636f 6d70 6f6e 656e 7473 5f70 7265  e_components_pre
-00015d90: 6669 783a 206c 6973 7420 6f66 2070 7265  fix: list of pre
-00015da0: 6669 7820 746f 2069 676e 6f72 652e 0a20  fix to ignore.. 
-00015db0: 2020 2020 2020 2069 676e 6f72 655f 6675         ignore_fu
-00015dc0: 6e63 7469 6f6e 735f 7072 6566 6978 3a20  nctions_prefix: 
-00015dd0: 6c69 7374 206f 6620 7072 6566 6978 2074  list of prefix t
-00015de0: 6f20 6967 6e6f 7265 2e0a 2020 2020 2222  o ignore..    ""
-00015df0: 220a 2020 2020 6967 6e6f 7265 5f66 756e  ".    ignore_fun
-00015e00: 6374 696f 6e73 5f70 7265 6669 7820 3d20  ctions_prefix = 
-00015e10: 6967 6e6f 7265 5f66 756e 6374 696f 6e73  ignore_functions
-00015e20: 5f70 7265 6669 7820 6f72 205b 5d0a 2020  _prefix or [].  
-00015e30: 2020 6967 6e6f 7265 5f63 6f6d 706f 6e65    ignore_compone
-00015e40: 6e74 735f 7072 6566 6978 203d 2069 676e  nts_prefix = ign
-00015e50: 6f72 655f 636f 6d70 6f6e 656e 7473 5f70  ore_components_p
-00015e60: 7265 6669 7820 6f72 205b 5d0a 0a20 2020  refix or []..   
-00015e70: 2069 6620 280a 2020 2020 2020 2020 6861   if (.        ha
-00015e80: 7361 7474 7228 636f 6d70 6f6e 656e 742c  sattr(component,
-00015e90: 2022 6675 6e63 7469 6f6e 5f6e 616d 6522   "function_name"
-00015ea0: 290a 2020 2020 2020 2020 616e 6420 636f  ).        and co
-00015eb0: 6d70 6f6e 656e 742e 6675 6e63 7469 6f6e  mponent.function
-00015ec0: 5f6e 616d 6520 696e 2069 676e 6f72 655f  _name in ignore_
-00015ed0: 6675 6e63 7469 6f6e 735f 7072 6566 6978  functions_prefix
-00015ee0: 0a20 2020 2029 3a0a 2020 2020 2020 2020  .    ):.        
-00015ef0: 7265 7475 726e 207b 7d0a 0a20 2020 2069  return {}..    i
-00015f00: 6620 6861 7361 7474 7228 636f 6d70 6f6e  f hasattr(compon
-00015f10: 656e 742c 2022 6e61 6d65 2229 2061 6e64  ent, "name") and
-00015f20: 2061 6e79 280a 2020 2020 2020 2020 636f   any(.        co
-00015f30: 6d70 6f6e 656e 742e 6e61 6d65 2e73 7461  mponent.name.sta
-00015f40: 7274 7377 6974 6828 6929 2066 6f72 2069  rtswith(i) for i
-00015f50: 2069 6e20 6967 6e6f 7265 5f63 6f6d 706f   in ignore_compo
-00015f60: 6e65 6e74 735f 7072 6566 6978 0a20 2020  nents_prefix.   
-00015f70: 2029 3a0a 2020 2020 2020 2020 7265 7475   ):.        retu
-00015f80: 726e 207b 7d0a 0a20 2020 206f 7574 7075  rn {}..    outpu
-00015f90: 7420 3d20 7b63 6f6d 706f 6e65 6e74 2e6e  t = {component.n
-00015fa0: 616d 653a 2064 6963 7428 636f 6d70 6f6e  ame: dict(compon
-00015fb0: 656e 742e 7365 7474 696e 6773 297d 0a20  ent.settings)}. 
-00015fc0: 2020 2066 6f72 2072 6566 6572 656e 6365     for reference
-00015fd0: 2069 6e20 636f 6d70 6f6e 656e 742e 7265   in component.re
-00015fe0: 6665 7265 6e63 6573 3a0a 2020 2020 2020  ferences:.      
-00015ff0: 2020 6966 2028 0a20 2020 2020 2020 2020    if (.         
-00016000: 2020 2069 7369 6e73 7461 6e63 6528 7265     isinstance(re
-00016010: 6665 7265 6e63 652c 2043 6f6d 706f 6e65  ference, Compone
-00016020: 6e74 5265 6665 7265 6e63 6529 0a20 2020  ntReference).   
-00016030: 2020 2020 2020 2020 2061 6e64 2072 6566           and ref
-00016040: 6572 656e 6365 2e72 6566 5f63 656c 6c2e  erence.ref_cell.
-00016050: 6e61 6d65 206e 6f74 2069 6e20 6f75 7470  name not in outp
-00016060: 7574 0a20 2020 2020 2020 2029 3a0a 2020  ut.        ):.  
-00016070: 2020 2020 2020 2020 2020 6f75 7470 7574            output
-00016080: 2e75 7064 6174 6528 7265 6375 7273 655f  .update(recurse_
-00016090: 7374 7275 6374 7572 6573 2872 6566 6572  structures(refer
-000160a0: 656e 6365 2e72 6566 5f63 656c 6c29 290a  ence.ref_cell)).
-000160b0: 0a20 2020 2072 6574 7572 6e20 6f75 7470  .    return outp
-000160c0: 7574 0a0a 0a64 6566 2066 6c61 7474 656e  ut...def flatten
-000160d0: 5f69 6e76 616c 6964 5f72 6566 735f 7265  _invalid_refs_re
-000160e0: 6375 7273 6976 6528 0a20 2020 2063 6f6d  cursive(.    com
-000160f0: 706f 6e65 6e74 3a20 436f 6d70 6f6e 656e  ponent: Componen
-00016100: 742c 0a20 2020 2067 7269 645f 7369 7a65  t,.    grid_size
-00016110: 3a20 4f70 7469 6f6e 616c 5b66 6c6f 6174  : Optional[float
-00016120: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 7570  ] = None,.    up
-00016130: 6461 7465 645f 636f 6d70 6f6e 656e 7473  dated_components
-00016140: 3d4e 6f6e 652c 0a20 2020 2074 7261 7665  =None,.    trave
-00016150: 7273 6564 5f63 6f6d 706f 6e65 6e74 733d  rsed_components=
-00016160: 4e6f 6e65 2c0a 293a 0a20 2020 2022 2222  None,.):.    """
-00016170: 5265 6375 7273 6976 656c 7920 666c 6174  Recursively flat
-00016180: 7465 6e73 2063 6f6d 706f 6e65 6e74 2072  tens component r
-00016190: 6566 6572 656e 6365 7320 7768 6963 6820  eferences which 
-000161a0: 6861 7665 2069 6e76 616c 6964 2074 7261  have invalid tra
-000161b0: 6e73 666f 726d 6174 696f 6e73 2028 692e  nsformations (i.
-000161c0: 652e 206e 6f6e 2d39 3020 6465 6720 726f  e. non-90 deg ro
-000161d0: 7461 7469 6f6e 7320 6f72 2073 7562 2d67  tations or sub-g
-000161e0: 7269 6420 7472 616e 736c 6174 696f 6e73  rid translations
-000161f0: 2920 616e 6420 7265 7475 726e 7320 6120  ) and returns a 
-00016200: 636f 7079 2069 6620 616e 7920 7375 6263  copy if any subc
-00016210: 656c 6c73 2068 6176 6520 6265 656e 206d  ells have been m
-00016220: 6f64 6966 6965 642e 0a0a 2020 2020 5741  odified...    WA
-00016230: 524e 494e 473a 2074 6869 7320 6675 6e63  RNING: this func
-00016240: 7469 6f6e 2077 696c 6c20 7072 6f64 7563  tion will produc
-00016250: 6520 7361 6d65 2d6e 616d 6520 636f 7069  e same-name copi
-00016260: 6573 206f 6620 6365 6c6c 732e 2049 7420  es of cells. It 
-00016270: 6973 2073 7472 6963 746c 7920 6d65 616e  is strictly mean
-00016280: 7420 746f 2062 6520 7573 6564 206f 6e20  t to be used on 
-00016290: 7772 6974 6520 6f66 2074 6865 2047 4453  write of the GDS
-000162a0: 2066 696c 6520 616e 640a 2020 2020 7368   file and.    sh
-000162b0: 6f75 6c64 206e 6f74 2062 6520 6d69 7865  ould not be mixe
-000162c0: 6420 7769 7468 206f 7468 6572 2063 656c  d with other cel
-000162d0: 6c73 2c20 6f72 2079 6f75 2077 696c 6c20  ls, or you will 
-000162e0: 6c69 6b65 6c79 2065 7870 6572 6965 6e63  likely experienc
-000162f0: 6520 6973 7375 6573 2077 6974 6820 6475  e issues with du
-00016300: 706c 6963 6174 6520 6365 6c6c 730a 0a20  plicate cells.. 
-00016310: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
-00016320: 2063 6f6d 706f 6e65 6e74 3a20 7468 6520   component: the 
-00016330: 636f 6d70 6f6e 656e 7420 746f 2066 6978  component to fix
-00016340: 2028 696e 2070 6c61 6365 292e 0a20 2020   (in place)..   
-00016350: 2020 2020 2067 7269 645f 7369 7a65 3a20       grid_size: 
-00016360: 7468 6520 4744 5320 6772 6964 2073 697a  the GDS grid siz
-00016370: 652c 2069 6e20 756d 2c20 6465 6661 756c  e, in um, defaul
-00016380: 7473 2074 6f20 6163 7469 7665 2050 444b  ts to active PDK
-00016390: 2e67 6574 5f67 7269 645f 7369 7a65 2829  .get_grid_size()
-000163a0: 0a20 2020 2020 2020 2020 2020 2061 6e79  .            any
-000163b0: 2074 7261 6e73 6c61 7469 6f6e 7320 7769   translations wi
-000163c0: 7468 2068 6967 6865 7220 7265 736f 6c75  th higher resolu
-000163d0: 7469 6f6e 2074 6861 6e20 7468 6973 2061  tion than this a
-000163e0: 7265 2063 6f6e 7369 6465 7265 6420 696e  re considered in
-000163f0: 7661 6c69 642e 0a20 2020 2020 2020 2075  valid..        u
-00016400: 7064 6174 6564 5f63 6f6d 706f 6e65 6e74  pdated_component
-00016410: 733a 2074 6865 2072 756e 6e69 6e67 2064  s: the running d
-00016420: 6963 7469 6f6e 6172 7920 6f66 2063 6f6d  ictionary of com
-00016430: 706f 6e65 6e74 7320 7768 6963 6820 6861  ponents which ha
-00016440: 7665 2062 6565 6e20 6d6f 6469 6669 6564  ve been modified
-00016450: 2062 7920 7468 6973 2074 7261 6e73 666f   by this transfo
-00016460: 726d 6174 696f 6e2e 2053 686f 756c 6420  rmation. Should 
-00016470: 616c 7761 7973 2062 6520 4e6f 6e65 2c20  always be None, 
-00016480: 6578 6365 7074 2066 6f72 2072 6563 7572  except for recur
-00016490: 7369 7665 2069 6e76 6f63 6174 696f 6e73  sive invocations
-000164a0: 2e0a 2020 2020 2020 2020 7472 6176 6572  ..        traver
-000164b0: 7365 645f 636f 6d70 6f6e 656e 7473 3a20  sed_components: 
-000164c0: 7468 6520 7365 7420 6f66 2063 6f6d 706f  the set of compo
-000164d0: 6e65 6e74 206e 616d 6573 2077 6869 6368  nent names which
-000164e0: 2068 6176 6520 6265 656e 2074 7261 7665   have been trave
-000164f0: 7273 6564 2e20 5368 6f75 6c64 2061 6c77  rsed. Should alw
-00016500: 6179 7320 6265 204e 6f6e 652c 2065 7863  ays be None, exc
-00016510: 6570 7420 666f 7220 7265 6375 7273 6976  ept for recursiv
-00016520: 6520 696e 766f 6361 7469 6f6e 732e 0a20  e invocations.. 
-00016530: 2020 2022 2222 0a20 2020 2066 726f 6d20     """.    from 
-00016540: 6764 7366 6163 746f 7279 2e64 6563 6f72  gdsfactory.decor
-00016550: 6174 6f72 7320 696d 706f 7274 2069 735f  ators import is_
-00016560: 696e 7661 6c69 645f 7265 660a 0a20 2020  invalid_ref..   
-00016570: 2069 6e76 616c 6964 5f72 6566 7320 3d20   invalid_refs = 
-00016580: 5b5d 0a20 2020 2072 6566 7320 3d20 636f  [].    refs = co
-00016590: 6d70 6f6e 656e 742e 7265 6665 7265 6e63  mponent.referenc
-000165a0: 6573 0a20 2020 2073 7562 6365 6c6c 5f6d  es.    subcell_m
-000165b0: 6f64 6966 6965 6420 3d20 4661 6c73 650a  odified = False.
-000165c0: 2020 2020 6966 2075 7064 6174 6564 5f63      if updated_c
-000165d0: 6f6d 706f 6e65 6e74 7320 6973 204e 6f6e  omponents is Non
-000165e0: 653a 0a20 2020 2020 2020 2075 7064 6174  e:.        updat
-000165f0: 6564 5f63 6f6d 706f 6e65 6e74 7320 3d20  ed_components = 
-00016600: 7b7d 0a20 2020 2069 6620 7472 6176 6572  {}.    if traver
-00016610: 7365 645f 636f 6d70 6f6e 656e 7473 2069  sed_components i
-00016620: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
-00016630: 7472 6176 6572 7365 645f 636f 6d70 6f6e  traversed_compon
-00016640: 656e 7473 203d 2073 6574 2829 0a20 2020  ents = set().   
-00016650: 2066 6f72 2072 6566 2069 6e20 7265 6673   for ref in refs
-00016660: 3a0a 2020 2020 2020 2020 2320 6d61 726b  :.        # mark
-00016670: 2061 6e79 2069 6e76 616c 6964 2072 6566   any invalid ref
-00016680: 7320 666f 7220 666c 6174 7465 6e69 6e67  s for flattening
-00016690: 0a20 2020 2020 2020 2023 206f 7468 6572  .        # other
-000166a0: 7769 7365 2c20 6368 6563 6b20 6966 2074  wise, check if t
-000166b0: 6865 7265 2061 7265 2061 6e79 206d 6f64  here are any mod
-000166c0: 6966 6965 6420 6365 6c6c 7320 6265 6e65  ified cells bene
-000166d0: 6174 6820 2877 6520 6e65 6564 206e 6f74  ath (we need not
-000166e0: 2064 6f20 7468 6973 2069 6620 7468 6520   do this if the 
-000166f0: 7265 6620 7769 6c6c 2062 6520 666c 6174  ref will be flat
-00016700: 7465 6e65 6420 616e 7977 6179 7329 0a20  tened anyways). 
-00016710: 2020 2020 2020 2069 6620 6973 5f69 6e76         if is_inv
-00016720: 616c 6964 5f72 6566 2872 6566 2c20 6772  alid_ref(ref, gr
-00016730: 6964 5f73 697a 6529 3a0a 2020 2020 2020  id_size):.      
-00016740: 2020 2020 2020 696e 7661 6c69 645f 7265        invalid_re
-00016750: 6673 2e61 7070 656e 6428 7265 662e 6e61  fs.append(ref.na
-00016760: 6d65 290a 2020 2020 2020 2020 656c 7365  me).        else
-00016770: 3a0a 2020 2020 2020 2020 2020 2020 2320  :.            # 
-00016780: 6f74 6865 7277 6973 652c 2072 6563 7572  otherwise, recur
-00016790: 7369 7665 6c79 2066 6c61 7474 656e 2072  sively flatten r
-000167a0: 6566 7320 6966 2074 6865 2073 7562 6365  efs if the subce
-000167b0: 6c6c 2068 6173 206e 6f74 2061 6c72 6561  ll has not alrea
-000167c0: 6479 2062 6565 6e20 7472 6176 6572 7365  dy been traverse
-000167d0: 640a 2020 2020 2020 2020 2020 2020 6966  d.            if
-000167e0: 2072 6566 2e70 6172 656e 742e 6e61 6d65   ref.parent.name
-000167f0: 206e 6f74 2069 6e20 7472 6176 6572 7365   not in traverse
-00016800: 645f 636f 6d70 6f6e 656e 7473 3a0a 2020  d_components:.  
-00016810: 2020 2020 2020 2020 2020 2020 2020 666c                fl
-00016820: 6174 7465 6e5f 696e 7661 6c69 645f 7265  atten_invalid_re
-00016830: 6673 5f72 6563 7572 7369 7665 280a 2020  fs_recursive(.  
-00016840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016850: 2020 7265 662e 7061 7265 6e74 2c0a 2020    ref.parent,.  
-00016860: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00016870: 2020 6772 6964 5f73 697a 653d 6772 6964    grid_size=grid
-00016880: 5f73 697a 652c 0a20 2020 2020 2020 2020  _size,.         
-00016890: 2020 2020 2020 2020 2020 2075 7064 6174             updat
-000168a0: 6564 5f63 6f6d 706f 6e65 6e74 733d 7570  ed_components=up
-000168b0: 6461 7465 645f 636f 6d70 6f6e 656e 7473  dated_components
-000168c0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000168d0: 2020 2020 2020 7472 6176 6572 7365 645f        traversed_
-000168e0: 636f 6d70 6f6e 656e 7473 3d74 7261 7665  components=trave
-000168f0: 7273 6564 5f63 6f6d 706f 6e65 6e74 732c  rsed_components,
-00016900: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00016910: 2029 0a20 2020 2020 2020 2020 2020 2023   ).            #
-00016920: 206e 6f77 2c20 6966 2074 6865 2072 6566   now, if the ref
-00016930: 2773 2063 656c 6c20 6265 656e 206d 6f64  's cell been mod
-00016940: 6966 6965 642c 206d 6172 6b20 6974 2061  ified, mark it a
-00016950: 7320 7375 6368 0a20 2020 2020 2020 2020  s such.         
-00016960: 2020 2069 6620 7265 662e 7061 7265 6e74     if ref.parent
-00016970: 2e6e 616d 6520 696e 2075 7064 6174 6564  .name in updated
-00016980: 5f63 6f6d 706f 6e65 6e74 733a 0a20 2020  _components:.   
-00016990: 2020 2020 2020 2020 2020 2020 2073 7562               sub
-000169a0: 6365 6c6c 5f6d 6f64 6966 6965 6420 3d20  cell_modified = 
-000169b0: 5472 7565 0a20 2020 2069 6620 696e 7661  True.    if inva
-000169c0: 6c69 645f 7265 6673 206f 7220 7375 6263  lid_refs or subc
-000169d0: 656c 6c5f 6d6f 6469 6669 6564 3a0a 2020  ell_modified:.  
-000169e0: 2020 2020 2020 6e65 775f 636f 6d70 6f6e        new_compon
-000169f0: 656e 7420 3d20 636f 6d70 6f6e 656e 742e  ent = component.
-00016a00: 636f 7079 2829 0a20 2020 2020 2020 206e  copy().        n
-00016a10: 6577 5f63 6f6d 706f 6e65 6e74 2e6e 616d  ew_component.nam
-00016a20: 6520 3d20 636f 6d70 6f6e 656e 742e 6e61  e = component.na
-00016a30: 6d65 0a20 2020 2020 2020 2023 206d 616b  me.        # mak
-00016a40: 6520 7375 7265 2061 6c6c 206d 6f64 6966  e sure all modif
-00016a50: 6965 6420 6365 6c6c 7320 6861 7665 2074  ied cells have t
-00016a60: 6865 6972 2072 6566 6572 656e 6365 7320  heir references 
-00016a70: 7570 6461 7465 640a 2020 2020 2020 2020  updated.        
-00016a80: 6e65 775f 7265 6673 203d 206e 6577 5f63  new_refs = new_c
-00016a90: 6f6d 706f 6e65 6e74 2e72 6566 6572 656e  omponent.referen
-00016aa0: 6365 732e 636f 7079 2829 0a20 2020 2020  ces.copy().     
-00016ab0: 2020 2066 6f72 2072 6566 2069 6e20 6e65     for ref in ne
-00016ac0: 775f 7265 6673 3a0a 2020 2020 2020 2020  w_refs:.        
-00016ad0: 2020 2020 6966 2072 6566 2e6e 616d 6520      if ref.name 
-00016ae0: 696e 2069 6e76 616c 6964 5f72 6566 733a  in invalid_refs:
-00016af0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00016b00: 206e 6577 5f63 6f6d 706f 6e65 6e74 2e66   new_component.f
-00016b10: 6c61 7474 656e 5f72 6566 6572 656e 6365  latten_reference
-00016b20: 2872 6566 290a 2020 2020 2020 2020 2020  (ref).          
-00016b30: 2020 656c 6966 2028 0a20 2020 2020 2020    elif (.       
-00016b40: 2020 2020 2020 2020 2072 6566 2e70 6172           ref.par
-00016b50: 656e 742e 6e61 6d65 2069 6e20 7570 6461  ent.name in upda
-00016b60: 7465 645f 636f 6d70 6f6e 656e 7473 0a20  ted_components. 
-00016b70: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-00016b80: 6e64 2072 6566 2e70 6172 656e 7420 6973  nd ref.parent is
-00016b90: 206e 6f74 2075 7064 6174 6564 5f63 6f6d   not updated_com
-00016ba0: 706f 6e65 6e74 735b 7265 662e 7061 7265  ponents[ref.pare
-00016bb0: 6e74 2e6e 616d 655d 0a20 2020 2020 2020  nt.name].       
-00016bc0: 2020 2020 2029 3a0a 2020 2020 2020 2020       ):.        
-00016bd0: 2020 2020 2020 2020 7265 662e 7061 7265          ref.pare
-00016be0: 6e74 203d 2075 7064 6174 6564 5f63 6f6d  nt = updated_com
-00016bf0: 706f 6e65 6e74 735b 7265 662e 7061 7265  ponents[ref.pare
-00016c00: 6e74 2e6e 616d 655d 0a20 2020 2020 2020  nt.name].       
-00016c10: 2063 6f6d 706f 6e65 6e74 203d 206e 6577   component = new
-00016c20: 5f63 6f6d 706f 6e65 6e74 0a20 2020 2020  _component.     
-00016c30: 2020 2075 7064 6174 6564 5f63 6f6d 706f     updated_compo
-00016c40: 6e65 6e74 735b 636f 6d70 6f6e 656e 742e  nents[component.
-00016c50: 6e61 6d65 5d20 3d20 6e65 775f 636f 6d70  name] = new_comp
-00016c60: 6f6e 656e 740a 2020 2020 7472 6176 6572  onent.    traver
-00016c70: 7365 645f 636f 6d70 6f6e 656e 7473 2e61  sed_components.a
-00016c80: 6464 2863 6f6d 706f 6e65 6e74 2e6e 616d  dd(component.nam
-00016c90: 6529 0a20 2020 2072 6574 7572 6e20 636f  e).    return co
-00016ca0: 6d70 6f6e 656e 740a 0a0a 6465 6620 5f63  mponent...def _c
-00016cb0: 6865 636b 5f75 6e63 6163 6865 645f 636f  heck_uncached_co
-00016cc0: 6d70 6f6e 656e 7473 2863 6f6d 706f 6e65  mponents(compone
-00016cd0: 6e74 2c20 6d6f 6465 293a 0a20 2020 2076  nt, mode):.    v
-00016ce0: 616c 6964 5f6d 6f64 6573 203d 205b 2277  alid_modes = ["w
-00016cf0: 6172 6e22 2c20 2265 7272 6f72 222c 2022  arn", "error", "
-00016d00: 6967 6e6f 7265 225d 0a0a 2020 2020 6966  ignore"]..    if
-00016d10: 206d 6f64 6520 3d3d 2022 6967 6e6f 7265   mode == "ignore
-00016d20: 223a 0a20 2020 2020 2020 2072 6574 7572  ":.        retur
-00016d30: 6e0a 2020 2020 656c 6966 206d 6f64 6520  n.    elif mode 
-00016d40: 6e6f 7420 696e 2076 616c 6964 5f6d 6f64  not in valid_mod
-00016d50: 6573 3a0a 2020 2020 2020 2020 7261 6973  es:.        rais
-00016d60: 6520 5661 6c75 6545 7272 6f72 280a 2020  e ValueError(.  
-00016d70: 2020 2020 2020 2020 2020 6622 7b6d 6f64            f"{mod
-00016d80: 657d 2069 7320 6e6f 7420 6120 7661 6c69  e} is not a vali
-00016d90: 6420 7661 6c75 6520 666f 7220 6f6e 5f75  d value for on_u
-00016da0: 6e63 6163 6865 645f 636f 6d70 6f6e 656e  ncached_componen
-00016db0: 742e 2054 7279 206f 6e65 206f 6620 7468  t. Try one of th
-00016dc0: 6573 653a 207b 7661 6c69 645f 6d6f 6465  ese: {valid_mode
-00016dd0: 737d 2e22 0a20 2020 2020 2020 2029 0a0a  s}.".        )..
-00016de0: 2020 2020 666f 7220 7375 625f 636f 6d70      for sub_comp
-00016df0: 6f6e 656e 7420 696e 2063 6f6d 706f 6e65  onent in compone
-00016e00: 6e74 2e67 6574 5f64 6570 656e 6465 6e63  nt.get_dependenc
-00016e10: 6965 7328 7265 6375 7273 6976 653d 5472  ies(recursive=Tr
-00016e20: 7565 293a 0a20 2020 2020 2020 2069 6620  ue):.        if 
-00016e30: 6e6f 7420 7375 625f 636f 6d70 6f6e 656e  not sub_componen
-00016e40: 742e 5f6c 6f63 6b65 643a 0a20 2020 2020  t._locked:.     
-00016e50: 2020 2020 2020 206d 6573 7361 6765 203d         message =
-00016e60: 2028 0a20 2020 2020 2020 2020 2020 2020   (.             
-00016e70: 2020 2066 2243 6f6d 706f 6e65 6e74 207b     f"Component {
-00016e80: 7375 625f 636f 6d70 6f6e 656e 742e 6e61  sub_component.na
-00016e90: 6d65 2172 7d20 7761 7320 4e4f 5420 7072  me!r} was NOT pr
-00016ea0: 6f70 6572 6c79 206c 6f63 6b65 642e 2022  operly locked. "
-00016eb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00016ec0: 2022 596f 7520 6e65 6564 2074 6f20 7772   "You need to wr
-00016ed0: 6974 6520 6974 2069 6e74 6f20 6120 6675  ite it into a fu
-00016ee0: 6e63 7469 6f6e 2074 6861 7420 6861 7320  nction that has 
-00016ef0: 7468 6520 4063 656c 6c20 6465 636f 7261  the @cell decora
-00016f00: 746f 722e 220a 2020 2020 2020 2020 2020  tor.".          
-00016f10: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
-00016f20: 6966 206d 6f64 6520 3d3d 2022 7761 726e  if mode == "warn
-00016f30: 223a 0a20 2020 2020 2020 2020 2020 2020  ":.             
-00016f40: 2020 2077 6172 6e69 6e67 732e 7761 726e     warnings.warn
-00016f50: 286d 6573 7361 6765 2c20 556e 6361 6368  (message, Uncach
-00016f60: 6564 436f 6d70 6f6e 656e 7457 6172 6e69  edComponentWarni
-00016f70: 6e67 290a 0a20 2020 2020 2020 2020 2020  ng)..           
-00016f80: 2065 6c69 6620 6d6f 6465 203d 3d20 2265   elif mode == "e
-00016f90: 7272 6f72 223a 0a20 2020 2020 2020 2020  rror":.         
-00016fa0: 2020 2020 2020 2072 6169 7365 2055 6e63         raise Unc
-00016fb0: 6163 6865 6443 6f6d 706f 6e65 6e74 4572  achedComponentEr
-00016fc0: 726f 7228 6d65 7373 6167 6529 0a0a 0a64  ror(message)...d
-00016fd0: 6566 2074 6573 745f 7361 6d65 5f75 6964  ef test_same_uid
-00016fe0: 2829 202d 3e20 4e6f 6e65 3a0a 2020 2020  () -> None:.    
-00016ff0: 696d 706f 7274 2067 6473 6661 6374 6f72  import gdsfactor
-00017000: 7920 6173 2067 660a 0a20 2020 2063 203d  y as gf..    c =
-00017010: 2043 6f6d 706f 6e65 6e74 2829 0a20 2020   Component().   
-00017020: 2063 203c 3c20 6766 2e63 6f6d 706f 6e65   c << gf.compone
-00017030: 6e74 732e 7265 6374 616e 676c 6528 290a  nts.rectangle().
-00017040: 2020 2020 6320 3c3c 2067 662e 636f 6d70      c << gf.comp
-00017050: 6f6e 656e 7473 2e72 6563 7461 6e67 6c65  onents.rectangle
-00017060: 2829 0a0a 2020 2020 7231 203d 2063 2e72  ()..    r1 = c.r
-00017070: 6566 6572 656e 6365 735b 305d 2e70 6172  eferences[0].par
-00017080: 656e 740a 2020 2020 7232 203d 2063 2e72  ent.    r2 = c.r
-00017090: 6566 6572 656e 6365 735b 315d 2e70 6172  eferences[1].par
-000170a0: 656e 740a 0a20 2020 2061 7373 6572 7420  ent..    assert 
-000170b0: 7231 2e75 6964 203d 3d20 7232 2e75 6964  r1.uid == r2.uid
-000170c0: 2c20 6622 7b72 312e 7569 647d 206d 7573  , f"{r1.uid} mus
-000170d0: 7420 6571 7561 6c20 7b72 322e 7569 647d  t equal {r2.uid}
-000170e0: 220a 0a0a 6465 6620 7465 7374 5f6e 6574  "...def test_net
-000170f0: 6c69 7374 5f73 696d 706c 6528 2920 2d3e  list_simple() ->
-00017100: 204e 6f6e 653a 0a20 2020 2069 6d70 6f72   None:.    impor
-00017110: 7420 6764 7366 6163 746f 7279 2061 7320  t gdsfactory as 
-00017120: 6766 0a0a 2020 2020 6320 3d20 6766 2e43  gf..    c = gf.C
-00017130: 6f6d 706f 6e65 6e74 2829 0a20 2020 2063  omponent().    c
-00017140: 3120 3d20 6320 3c3c 2067 662e 636f 6d70  1 = c << gf.comp
-00017150: 6f6e 656e 7473 2e73 7472 6169 6768 7428  onents.straight(
-00017160: 6c65 6e67 7468 3d31 2c20 7769 6474 683d  length=1, width=
-00017170: 3229 0a20 2020 2063 3220 3d20 6320 3c3c  2).    c2 = c <<
-00017180: 2067 662e 636f 6d70 6f6e 656e 7473 2e73   gf.components.s
-00017190: 7472 6169 6768 7428 6c65 6e67 7468 3d32  traight(length=2
-000171a0: 2c20 7769 6474 683d 3229 0a20 2020 2063  , width=2).    c
-000171b0: 322e 636f 6e6e 6563 7428 706f 7274 3d22  2.connect(port="
-000171c0: 6f31 222c 2064 6573 7469 6e61 7469 6f6e  o1", destination
-000171d0: 3d63 312e 706f 7274 735b 226f 3222 5d29  =c1.ports["o2"])
-000171e0: 0a20 2020 2063 2e61 6464 5f70 6f72 7428  .    c.add_port(
-000171f0: 226f 3122 2c20 706f 7274 3d63 312e 706f  "o1", port=c1.po
-00017200: 7274 735b 226f 3122 5d29 0a20 2020 2063  rts["o1"]).    c
-00017210: 2e61 6464 5f70 6f72 7428 226f 3222 2c20  .add_port("o2", 
-00017220: 706f 7274 3d63 322e 706f 7274 735b 226f  port=c2.ports["o
-00017230: 3222 5d29 0a20 2020 206e 6574 6c69 7374  2"]).    netlist
-00017240: 203d 2063 2e67 6574 5f6e 6574 6c69 7374   = c.get_netlist
-00017250: 2829 0a20 2020 2023 2070 7269 6e74 286e  ().    # print(n
-00017260: 6574 6c69 7374 2e70 7265 7474 7928 2929  etlist.pretty())
-00017270: 0a20 2020 2061 7373 6572 7420 6c65 6e28  .    assert len(
-00017280: 6e65 746c 6973 745b 2269 6e73 7461 6e63  netlist["instanc
-00017290: 6573 225d 2920 3d3d 2032 0a0a 0a64 6566  es"]) == 2...def
-000172a0: 2074 6573 745f 6e65 746c 6973 745f 7369   test_netlist_si
-000172b0: 6d70 6c65 5f77 6964 7468 5f6d 6973 6d61  mple_width_misma
-000172c0: 7463 685f 7468 726f 7773 5f65 7272 6f72  tch_throws_error
-000172d0: 2829 202d 3e20 4e6f 6e65 3a0a 2020 2020  () -> None:.    
-000172e0: 696d 706f 7274 2070 7974 6573 740a 0a20  import pytest.. 
-000172f0: 2020 2069 6d70 6f72 7420 6764 7366 6163     import gdsfac
-00017300: 746f 7279 2061 7320 6766 0a0a 2020 2020  tory as gf..    
-00017310: 6320 3d20 6766 2e43 6f6d 706f 6e65 6e74  c = gf.Component
-00017320: 2829 0a20 2020 2063 3120 3d20 6320 3c3c  ().    c1 = c <<
-00017330: 2067 662e 636f 6d70 6f6e 656e 7473 2e73   gf.components.s
-00017340: 7472 6169 6768 7428 6c65 6e67 7468 3d31  traight(length=1
-00017350: 2c20 7769 6474 683d 3129 0a20 2020 2063  , width=1).    c
-00017360: 3220 3d20 6320 3c3c 2067 662e 636f 6d70  2 = c << gf.comp
-00017370: 6f6e 656e 7473 2e73 7472 6169 6768 7428  onents.straight(
-00017380: 6c65 6e67 7468 3d32 2c20 7769 6474 683d  length=2, width=
-00017390: 3229 0a20 2020 2063 322e 636f 6e6e 6563  2).    c2.connec
-000173a0: 7428 706f 7274 3d22 6f31 222c 2064 6573  t(port="o1", des
-000173b0: 7469 6e61 7469 6f6e 3d63 312e 706f 7274  tination=c1.port
-000173c0: 735b 226f 3222 5d29 0a20 2020 2063 2e61  s["o2"]).    c.a
-000173d0: 6464 5f70 6f72 7428 226f 3122 2c20 706f  dd_port("o1", po
-000173e0: 7274 3d63 312e 706f 7274 735b 226f 3122  rt=c1.ports["o1"
-000173f0: 5d29 0a20 2020 2063 2e61 6464 5f70 6f72  ]).    c.add_por
-00017400: 7428 226f 3222 2c20 706f 7274 3d63 322e  t("o2", port=c2.
-00017410: 706f 7274 735b 226f 3222 5d29 0a20 2020  ports["o2"]).   
-00017420: 2077 6974 6820 7079 7465 7374 2e72 6169   with pytest.rai
-00017430: 7365 7328 5661 6c75 6545 7272 6f72 293a  ses(ValueError):
-00017440: 0a20 2020 2020 2020 2063 2e67 6574 5f6e  .        c.get_n
-00017450: 6574 6c69 7374 2829 0a0a 0a64 6566 2074  etlist()...def t
-00017460: 6573 745f 6e65 746c 6973 745f 636f 6d70  est_netlist_comp
-00017470: 6c65 7828 2920 2d3e 204e 6f6e 653a 0a20  lex() -> None:. 
-00017480: 2020 2069 6d70 6f72 7420 6764 7366 6163     import gdsfac
-00017490: 746f 7279 2061 7320 6766 0a0a 2020 2020  tory as gf..    
-000174a0: 6320 3d20 6766 2e63 6f6d 706f 6e65 6e74  c = gf.component
-000174b0: 732e 6d7a 695f 6172 6d73 2829 0a20 2020  s.mzi_arms().   
-000174c0: 206e 6574 6c69 7374 203d 2063 2e67 6574   netlist = c.get
-000174d0: 5f6e 6574 6c69 7374 2829 0a20 2020 2023  _netlist().    #
-000174e0: 2070 7269 6e74 286e 6574 6c69 7374 2e70   print(netlist.p
-000174f0: 7265 7474 7928 2929 0a20 2020 2061 7373  retty()).    ass
-00017500: 6572 7420 6c65 6e28 6e65 746c 6973 745b  ert len(netlist[
-00017510: 2269 6e73 7461 6e63 6573 225d 2920 3d3d  "instances"]) ==
-00017520: 2034 2c20 6c65 6e28 6e65 746c 6973 745b   4, len(netlist[
-00017530: 2269 6e73 7461 6e63 6573 225d 290a 0a0a  "instances"])...
-00017540: 6465 6620 7465 7374 5f65 7874 7261 6374  def test_extract
-00017550: 2829 202d 3e20 436f 6d70 6f6e 656e 743a  () -> Component:
-00017560: 0a20 2020 2069 6d70 6f72 7420 6764 7366  .    import gdsf
-00017570: 6163 746f 7279 2061 7320 6766 0a0a 2020  actory as gf..  
-00017580: 2020 6320 3d20 6766 2e63 6f6d 706f 6e65    c = gf.compone
-00017590: 6e74 732e 7374 7261 6967 6874 280a 2020  nts.straight(.  
-000175a0: 2020 2020 2020 6c65 6e67 7468 3d31 302c        length=10,
-000175b0: 0a20 2020 2020 2020 2077 6964 7468 3d30  .        width=0
-000175c0: 2e35 2c0a 2020 2020 2020 2020 6262 6f78  .5,.        bbox
-000175d0: 5f6c 6179 6572 733d 5b67 662e 4c41 5945  _layers=[gf.LAYE
-000175e0: 522e 5747 434c 4144 5d2c 0a20 2020 2020  R.WGCLAD],.     
-000175f0: 2020 2062 626f 785f 6f66 6673 6574 733d     bbox_offsets=
-00017600: 5b33 5d2c 0a20 2020 2020 2020 2077 6974  [3],.        wit
-00017610: 685f 6262 6f78 3d54 7275 652c 0a20 2020  h_bbox=True,.   
-00017620: 2020 2020 2063 6c61 6464 696e 675f 6c61       cladding_la
-00017630: 7965 7273 3d4e 6f6e 652c 0a20 2020 2020  yers=None,.     
-00017640: 2020 2061 6464 5f70 696e 733d 4e6f 6e65     add_pins=None
-00017650: 2c0a 2020 2020 2020 2020 6164 645f 6262  ,.        add_bb
-00017660: 6f78 3d4e 6f6e 652c 0a20 2020 2029 0a20  ox=None,.    ). 
-00017670: 2020 2063 3220 3d20 632e 6578 7472 6163     c2 = c.extrac
-00017680: 7428 6c61 7965 7273 3d5b 6766 2e4c 4159  t(layers=[gf.LAY
-00017690: 4552 2e57 4743 4c41 445d 290a 0a20 2020  ER.WGCLAD])..   
-000176a0: 2061 7373 6572 7420 6c65 6e28 632e 706f   assert len(c.po
-000176b0: 6c79 676f 6e73 2920 3d3d 2032 2c20 6c65  lygons) == 2, le
-000176c0: 6e28 632e 706f 6c79 676f 6e73 290a 2020  n(c.polygons).  
-000176d0: 2020 6173 7365 7274 206c 656e 2863 322e    assert len(c2.
-000176e0: 706f 6c79 676f 6e73 2920 3d3d 2031 2c20  polygons) == 1, 
-000176f0: 6c65 6e28 6332 2e70 6f6c 7967 6f6e 7329  len(c2.polygons)
-00017700: 0a20 2020 2061 7373 6572 7420 6766 2e4c  .    assert gf.L
-00017710: 4159 4552 2e57 4743 4c41 4420 696e 2063  AYER.WGCLAD in c
-00017720: 322e 6c61 7965 7273 0a20 2020 2072 6574  2.layers.    ret
-00017730: 7572 6e20 6332 0a0a 0a64 6566 2068 6173  urn c2...def has
-00017740: 685f 6669 6c65 2866 696c 6570 6174 6829  h_file(filepath)
-00017750: 3a0a 2020 2020 6d64 3520 3d20 6861 7368  :.    md5 = hash
-00017760: 6c69 622e 6d64 3528 290a 2020 2020 6d64  lib.md5().    md
-00017770: 352e 7570 6461 7465 2866 696c 6570 6174  5.update(filepat
-00017780: 682e 7265 6164 5f62 7974 6573 2829 290a  h.read_bytes()).
-00017790: 2020 2020 7265 7475 726e 206d 6435 2e68      return md5.h
-000177a0: 6578 6469 6765 7374 2829 0a0a 0a64 6566  exdigest()...def
-000177b0: 2074 6573 745f 6262 6f78 5f72 6566 6572   test_bbox_refer
-000177c0: 656e 6365 2829 202d 3e20 436f 6d70 6f6e  ence() -> Compon
-000177d0: 656e 743a 0a20 2020 2069 6d70 6f72 7420  ent:.    import 
-000177e0: 6764 7366 6163 746f 7279 2061 7320 6766  gdsfactory as gf
-000177f0: 0a0a 2020 2020 6320 3d20 6766 2e43 6f6d  ..    c = gf.Com
-00017800: 706f 6e65 6e74 2822 636f 6d70 6f6e 656e  ponent("componen
-00017810: 745f 7769 7468 5f6f 6666 6772 6964 5f70  t_with_offgrid_p
-00017820: 6f6c 7967 6f6e 7322 290a 2020 2020 6331  olygons").    c1
-00017830: 203d 2063 203c 3c20 6766 2e63 6f6d 706f   = c << gf.compo
-00017840: 6e65 6e74 732e 7265 6374 616e 676c 6528  nents.rectangle(
-00017850: 7369 7a65 3d28 312e 3565 2d33 2c20 312e  size=(1.5e-3, 1.
-00017860: 3565 2d33 292c 2070 6f72 745f 7479 7065  5e-3), port_type
-00017870: 3d4e 6f6e 6529 0a20 2020 2063 3220 3d20  =None).    c2 = 
-00017880: 6320 3c3c 2067 662e 636f 6d70 6f6e 656e  c << gf.componen
-00017890: 7473 2e72 6563 7461 6e67 6c65 2873 697a  ts.rectangle(siz
-000178a0: 653d 2831 2e35 652d 332c 2031 2e35 652d  e=(1.5e-3, 1.5e-
-000178b0: 3329 2c20 706f 7274 5f74 7970 653d 4e6f  3), port_type=No
-000178c0: 6e65 290a 2020 2020 6332 2e78 6d69 6e20  ne).    c2.xmin 
-000178d0: 3d20 6331 2e78 6d61 780a 0a20 2020 2061  = c1.xmax..    a
-000178e0: 7373 6572 7420 6332 2e78 7369 7a65 203d  ssert c2.xsize =
-000178f0: 3d20 3265 2d33 0a20 2020 2072 6574 7572  = 2e-3.    retur
-00017900: 6e20 6332 0a0a 0a64 6566 2074 6573 745f  n c2...def test_
-00017910: 6262 6f78 5f63 6f6d 706f 6e65 6e74 2829  bbox_component()
-00017920: 202d 3e20 4e6f 6e65 3a0a 2020 2020 696d   -> None:.    im
-00017930: 706f 7274 2067 6473 6661 6374 6f72 7920  port gdsfactory 
-00017940: 6173 2067 660a 0a20 2020 2063 203d 2067  as gf..    c = g
-00017950: 662e 636f 6d70 6f6e 656e 7473 2e72 6563  f.components.rec
-00017960: 7461 6e67 6c65 2873 697a 653d 2831 2e35  tangle(size=(1.5
-00017970: 652d 332c 2031 2e35 652d 3329 2c20 706f  e-3, 1.5e-3), po
-00017980: 7274 5f74 7970 653d 4e6f 6e65 290a 2020  rt_type=None).  
-00017990: 2020 6173 7365 7274 2063 2e78 7369 7a65    assert c.xsize
-000179a0: 203d 3d20 3265 2d33 0a0a 0a64 6566 2074   == 2e-3...def t
-000179b0: 6573 745f 7265 6d61 705f 6c61 7965 7273  est_remap_layers
+00013760: 2020 2020 2020 286e 6577 5f6c 6179 6572        (new_layer
+00013770: 735b 6c61 7965 725f 6e75 6d62 6572 5d2c  s[layer_number],
+00013780: 206e 6577 5f64 6174 6174 7970 6573 5b6c   new_datatypes[l
+00013790: 6179 6572 5f6e 756d 6265 725d 290a 2020  ayer_number]).  
+000137a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000137b0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+000137c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000137d0: 6966 206f 7269 6769 6e61 6c5f 6c61 7965  if original_laye
+000137e0: 7220 696e 206c 6179 6572 6d61 703a 0a20  r in layermap:. 
+000137f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013800: 2020 2020 2020 2020 2020 206e 6577 5f6c             new_l
+00013810: 6179 6572 203d 206c 6179 6572 6d61 705b  ayer = layermap[
+00013820: 6f72 6967 696e 616c 5f6c 6179 6572 5d0a  original_layer].
+00013830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013840: 2020 2020 2020 2020 2020 2020 6e65 775f              new_
+00013850: 6c61 7965 7273 5b6c 6179 6572 5f6e 756d  layers[layer_num
+00013860: 6265 725d 203d 206e 6577 5f6c 6179 6572  ber] = new_layer
+00013870: 5b30 5d0a 2020 2020 2020 2020 2020 2020  [0].            
+00013880: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013890: 6e65 775f 6461 7461 7479 7065 735b 6c61  new_datatypes[la
+000138a0: 7965 725f 6e75 6d62 6572 5d20 3d20 6e65  yer_number] = ne
+000138b0: 775f 6c61 7965 725b 315d 0a20 2020 2020  w_layer[1].     
+000138c0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+000138d0: 6174 682e 7365 745f 6c61 7965 7273 282a  ath.set_layers(*
+000138e0: 6e65 775f 6c61 7965 7273 290a 2020 2020  new_layers).    
+000138f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013900: 7061 7468 2e73 6574 5f64 6174 6174 7970  path.set_datatyp
+00013910: 6573 282a 6e65 775f 6461 7461 7479 7065  es(*new_datatype
+00013920: 7329 0a20 2020 2020 2020 2072 6574 7572  s).        retur
+00013930: 6e20 636f 6d70 6f6e 656e 740a 0a20 2020  n component..   
+00013940: 2064 6566 2074 6f5f 3364 280a 2020 2020   def to_3d(.    
+00013950: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
+00013960: 2020 6c61 7965 725f 7669 6577 733a 204f    layer_views: O
+00013970: 7074 696f 6e61 6c5b 4c61 7965 7256 6965  ptional[LayerVie
+00013980: 7773 5d20 3d20 4e6f 6e65 2c0a 2020 2020  ws] = None,.    
+00013990: 2020 2020 6c61 7965 725f 7374 6163 6b3a      layer_stack:
+000139a0: 204f 7074 696f 6e61 6c5b 4c61 7965 7253   Optional[LayerS
+000139b0: 7461 636b 5d20 3d20 4e6f 6e65 2c0a 2020  tack] = None,.  
+000139c0: 2020 2020 2020 6578 636c 7564 655f 6c61        exclude_la
+000139d0: 7965 7273 3a20 4f70 7469 6f6e 616c 5b54  yers: Optional[T
+000139e0: 7570 6c65 5b4c 6179 6572 2c20 2e2e 2e5d  uple[Layer, ...]
+000139f0: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 293a  ] = None,.    ):
+00013a00: 0a20 2020 2020 2020 2022 2222 5265 7475  .        """Retu
+00013a10: 726e 2043 6f6d 706f 6e65 6e74 2033 4420  rn Component 3D 
+00013a20: 7472 696d 6573 6820 5363 656e 652e 0a0a  trimesh Scene...
+00013a30: 2020 2020 2020 2020 4172 6773 3a0a 2020          Args:.  
+00013a40: 2020 2020 2020 2020 2020 636f 6d70 6f6e            compon
+00013a50: 656e 743a 2074 6f20 6578 7472 7564 6520  ent: to extrude 
+00013a60: 696e 2033 442e 0a20 2020 2020 2020 2020  in 3D..         
+00013a70: 2020 206c 6179 6572 5f76 6965 7773 3a20     layer_views: 
+00013a80: 6c61 7965 7220 636f 6c6f 7273 2066 726f  layer colors fro
+00013a90: 6d20 4b6c 6179 6f75 7420 4c61 7965 7220  m Klayout Layer 
+00013aa0: 5072 6f70 6572 7469 6573 2066 696c 652e  Properties file.
+00013ab0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00013ac0: 2044 6566 6175 6c74 7320 746f 2061 6374   Defaults to act
+00013ad0: 6976 6520 5044 4b2e 6c61 7965 725f 7669  ive PDK.layer_vi
+00013ae0: 6577 732e 0a20 2020 2020 2020 2020 2020  ews..           
+00013af0: 206c 6179 6572 5f73 7461 636b 3a20 636f   layer_stack: co
+00013b00: 6e74 6169 6e73 2074 6869 636b 6e65 7373  ntains thickness
+00013b10: 2061 6e64 207a 6d69 6e20 666f 7220 6561   and zmin for ea
+00013b20: 6368 206c 6179 6572 2e0a 2020 2020 2020  ch layer..      
+00013b30: 2020 2020 2020 2020 2020 4465 6661 756c            Defaul
+00013b40: 7473 2074 6f20 6163 7469 7665 2050 444b  ts to active PDK
+00013b50: 2e6c 6179 6572 5f73 7461 636b 2e0a 2020  .layer_stack..  
+00013b60: 2020 2020 2020 2020 2020 6578 636c 7564            exclud
+00013b70: 655f 6c61 7965 7273 3a20 6c61 7965 7273  e_layers: layers
+00013b80: 2074 6f20 6578 636c 7564 652e 0a0a 2020   to exclude...  
+00013b90: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00013ba0: 2020 6672 6f6d 2067 6473 6661 6374 6f72    from gdsfactor
+00013bb0: 792e 6578 706f 7274 2e74 6f5f 3364 2069  y.export.to_3d i
+00013bc0: 6d70 6f72 7420 746f 5f33 640a 0a20 2020  mport to_3d..   
+00013bd0: 2020 2020 2072 6574 7572 6e20 746f 5f33       return to_3
+00013be0: 6428 0a20 2020 2020 2020 2020 2020 2073  d(.            s
+00013bf0: 656c 662c 0a20 2020 2020 2020 2020 2020  elf,.           
+00013c00: 206c 6179 6572 5f76 6965 7773 3d6c 6179   layer_views=lay
+00013c10: 6572 5f76 6965 7773 2c0a 2020 2020 2020  er_views,.      
+00013c20: 2020 2020 2020 6c61 7965 725f 7374 6163        layer_stac
+00013c30: 6b3d 6c61 7965 725f 7374 6163 6b2c 0a20  k=layer_stack,. 
+00013c40: 2020 2020 2020 2020 2020 2065 7863 6c75             exclu
+00013c50: 6465 5f6c 6179 6572 733d 6578 636c 7564  de_layers=exclud
+00013c60: 655f 6c61 7965 7273 2c0a 2020 2020 2020  e_layers,.      
+00013c70: 2020 290a 0a20 2020 2064 6566 2074 6f5f    )..    def to_
+00013c80: 6e70 280a 2020 2020 2020 2020 7365 6c66  np(.        self
+00013c90: 2c0a 2020 2020 2020 2020 6e6d 5f70 6572  ,.        nm_per
+00013ca0: 5f70 6978 656c 3a20 696e 7420 3d20 3230  _pixel: int = 20
+00013cb0: 2c0a 2020 2020 2020 2020 6c61 7965 7273  ,.        layers
+00013cc0: 3a20 4c61 7965 7273 203d 2028 2831 2c20  : Layers = ((1, 
+00013cd0: 3029 2c29 2c0a 2020 2020 2020 2020 7661  0),),.        va
+00013ce0: 6c75 6573 3a20 4f70 7469 6f6e 616c 5b54  lues: Optional[T
+00013cf0: 7570 6c65 5b66 6c6f 6174 2c20 2e2e 2e5d  uple[float, ...]
+00013d00: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2020  ] = None,.      
+00013d10: 2020 7061 645f 7769 6474 683a 2069 6e74    pad_width: int
+00013d20: 203d 2031 2c0a 2020 2020 2920 2d3e 206e   = 1,.    ) -> n
+00013d30: 702e 6e64 6172 7261 793a 0a20 2020 2020  p.ndarray:.     
+00013d40: 2020 2022 2222 5265 7475 726e 7320 6120     """Returns a 
+00013d50: 7069 7865 6c61 7465 6420 6e75 6d70 7920  pixelated numpy 
+00013d60: 6172 7261 7920 6672 6f6d 2043 6f6d 706f  array from Compo
+00013d70: 6e65 6e74 2070 6f6c 7967 6f6e 732e 0a0a  nent polygons...
+00013d80: 2020 2020 2020 2020 4172 6773 3a0a 2020          Args:.  
+00013d90: 2020 2020 2020 2020 2020 636f 6d70 6f6e            compon
+00013da0: 656e 743a 2043 6f6d 706f 6e65 6e74 2e0a  ent: Component..
+00013db0: 2020 2020 2020 2020 2020 2020 6e6d 5f70              nm_p
+00013dc0: 6572 5f70 6978 656c 3a20 796f 7520 6361  er_pixel: you ca
+00013dd0: 6e20 676f 2066 726f 6d20 3230 2028 636f  n go from 20 (co
+00013de0: 6172 7365 2920 746f 2034 2028 6669 6e65  arse) to 4 (fine
+00013df0: 292e 0a20 2020 2020 2020 2020 2020 206c  )..            l
+00013e00: 6179 6572 733a 2074 6f20 636f 6e76 6572  ayers: to conver
+00013e10: 742e 204f 7264 6572 206d 6174 7465 7273  t. Order matters
+00013e20: 2028 6c61 7474 6572 206f 7665 7277 7269   (latter overwri
+00013e30: 7465 2066 6f72 6d65 7229 2e0a 2020 2020  te former)..    
+00013e40: 2020 2020 2020 2020 7661 6c75 6573 3a20          values: 
+00013e50: 6173 736f 6369 6174 6564 2074 6f20 6561  associated to ea
+00013e60: 6368 206c 6179 6572 2028 6465 6661 756c  ch layer (defaul
+00013e70: 7473 2074 6f20 3129 2e0a 2020 2020 2020  ts to 1)..      
+00013e80: 2020 2020 2020 7061 645f 7769 6474 683a        pad_width:
+00013e90: 2070 6164 6469 6e67 2070 6978 656c 7320   padding pixels 
+00013ea0: 6172 6f75 6e64 2074 6865 2069 6d61 6765  around the image
+00013eb0: 2e0a 0a20 2020 2020 2020 2022 2222 0a20  ...        """. 
+00013ec0: 2020 2020 2020 2066 726f 6d20 6764 7366         from gdsf
+00013ed0: 6163 746f 7279 2e65 7870 6f72 742e 746f  actory.export.to
+00013ee0: 5f6e 7020 696d 706f 7274 2074 6f5f 6e70  _np import to_np
+00013ef0: 0a0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+00013f00: 2074 6f5f 6e70 280a 2020 2020 2020 2020   to_np(.        
+00013f10: 2020 2020 7365 6c66 2c0a 2020 2020 2020      self,.      
+00013f20: 2020 2020 2020 6e6d 5f70 6572 5f70 6978        nm_per_pix
+00013f30: 656c 3d6e 6d5f 7065 725f 7069 7865 6c2c  el=nm_per_pixel,
+00013f40: 0a20 2020 2020 2020 2020 2020 206c 6179  .            lay
+00013f50: 6572 733d 6c61 7965 7273 2c0a 2020 2020  ers=layers,.    
+00013f60: 2020 2020 2020 2020 7661 6c75 6573 3d76          values=v
+00013f70: 616c 7565 732c 0a20 2020 2020 2020 2020  alues,.         
+00013f80: 2020 2070 6164 5f77 6964 7468 3d70 6164     pad_width=pad
+00013f90: 5f77 6964 7468 2c0a 2020 2020 2020 2020  _width,.        
+00013fa0: 290a 0a20 2020 2064 6566 2077 7269 7465  )..    def write
+00013fb0: 5f73 746c 280a 2020 2020 2020 2020 7365  _stl(.        se
+00013fc0: 6c66 2c0a 2020 2020 2020 2020 6669 6c65  lf,.        file
+00013fd0: 7061 7468 3a20 7374 722c 0a20 2020 2020  path: str,.     
+00013fe0: 2020 206c 6179 6572 5f73 7461 636b 3a20     layer_stack: 
+00013ff0: 4f70 7469 6f6e 616c 5b4c 6179 6572 5374  Optional[LayerSt
+00014000: 6163 6b5d 203d 204e 6f6e 652c 0a20 2020  ack] = None,.   
+00014010: 2020 2020 2065 7863 6c75 6465 5f6c 6179       exclude_lay
+00014020: 6572 733a 204f 7074 696f 6e61 6c5b 5475  ers: Optional[Tu
+00014030: 706c 655b 4c61 7965 722c 202e 2e2e 5d5d  ple[Layer, ...]]
+00014040: 203d 204e 6f6e 652c 0a20 2020 2029 202d   = None,.    ) -
+00014050: 3e20 6e70 2e6e 6461 7272 6179 3a0a 2020  > np.ndarray:.  
+00014060: 2020 2020 2020 2222 2257 7269 7465 2061        """Write a
+00014070: 2043 6f6d 706f 6e65 6e74 2074 6f20 5354   Component to ST
+00014080: 4c20 666f 7220 3344 2070 7269 6e74 696e  L for 3D printin
+00014090: 672e 0a0a 2020 2020 2020 2020 4172 6773  g...        Args
+000140a0: 3a0a 2020 2020 2020 2020 2020 2020 6669  :.            fi
+000140b0: 6c65 7061 7468 3a20 746f 2077 7269 7465  lepath: to write
+000140c0: 2053 544c 2074 6f2e 0a20 2020 2020 2020   STL to..       
+000140d0: 2020 2020 206c 6179 6572 5f73 7461 636b       layer_stack
+000140e0: 3a20 636f 6e74 6169 6e73 2074 6869 636b  : contains thick
+000140f0: 6e65 7373 2061 6e64 207a 6d69 6e20 666f  ness and zmin fo
+00014100: 7220 6561 6368 206c 6179 6572 2e0a 2020  r each layer..  
+00014110: 2020 2020 2020 2020 2020 6578 636c 7564            exclud
+00014120: 655f 6c61 7965 7273 3a20 6c61 7965 7273  e_layers: layers
+00014130: 2074 6f20 6578 636c 7564 652e 0a20 2020   to exclude..   
+00014140: 2020 2020 2020 2020 2075 7365 5f6c 6179           use_lay
+00014150: 6572 5f6e 616d 653a 2049 6620 5472 7565  er_name: If True
+00014160: 2c20 7573 6573 204c 6179 6572 4c65 7665  , uses LayerLeve
+00014170: 6c20 6e61 6d65 7320 696e 206f 7574 7075  l names in outpu
+00014180: 7420 6669 6c65 6e61 6d65 7320 7261 7468  t filenames rath
+00014190: 6572 2074 6861 6e20 6764 735f 6c61 7965  er than gds_laye
+000141a0: 7220 616e 6420 6764 735f 6461 7461 7479  r and gds_dataty
+000141b0: 7065 2e0a 2020 2020 2020 2020 2020 2020  pe..            
+000141c0: 6875 6c6c 5f69 6e76 616c 6964 5f70 6f6c  hull_invalid_pol
+000141d0: 7967 6f6e 733a 2049 6620 5472 7565 2c20  ygons: If True, 
+000141e0: 7265 706c 6163 6573 2069 6e76 616c 6964  replaces invalid
+000141f0: 2070 6f6c 7967 6f6e 7320 2864 6574 6572   polygons (deter
+00014200: 6d69 6e65 6420 6279 2073 6861 7065 6c79  mined by shapely
+00014210: 2e50 6f6c 7967 6f6e 2e69 735f 7661 6c69  .Polygon.is_vali
+00014220: 6429 2077 6974 6820 6974 7320 636f 6e76  d) with its conv
+00014230: 6578 2068 756c 6c2e 0a20 2020 2020 2020  ex hull..       
+00014240: 2020 2020 2073 6361 6c65 3a20 4f70 7469       scale: Opti
+00014250: 6f6e 616c 2066 6163 746f 7220 6279 2077  onal factor by w
+00014260: 6869 6368 2074 6f20 7363 616c 6520 6d65  hich to scale me
+00014270: 7368 6573 2062 6566 6f72 6520 7772 6974  shes before writ
+00014280: 696e 672e 0a0a 2020 2020 2020 2020 2222  ing...        ""
+00014290: 220a 2020 2020 2020 2020 6672 6f6d 2067  ".        from g
+000142a0: 6473 6661 6374 6f72 792e 6578 706f 7274  dsfactory.export
+000142b0: 2e74 6f5f 7374 6c20 696d 706f 7274 2074  .to_stl import t
+000142c0: 6f5f 7374 6c0a 0a20 2020 2020 2020 2072  o_stl..        r
+000142d0: 6574 7572 6e20 746f 5f73 746c 280a 2020  eturn to_stl(.  
+000142e0: 2020 2020 2020 2020 2020 7365 6c66 2c0a            self,.
+000142f0: 2020 2020 2020 2020 2020 2020 6669 6c65              file
+00014300: 7061 7468 3d66 696c 6570 6174 682c 0a20  path=filepath,. 
+00014310: 2020 2020 2020 2020 2020 206c 6179 6572             layer
+00014320: 5f73 7461 636b 3d6c 6179 6572 5f73 7461  _stack=layer_sta
+00014330: 636b 2c0a 2020 2020 2020 2020 2020 2020  ck,.            
+00014340: 6578 636c 7564 655f 6c61 7965 7273 3d65  exclude_layers=e
+00014350: 7863 6c75 6465 5f6c 6179 6572 732c 0a20  xclude_layers,. 
+00014360: 2020 2020 2020 2029 0a0a 2020 2020 6465         )..    de
+00014370: 6620 746f 5f67 6d73 6828 0a20 2020 2020  f to_gmsh(.     
+00014380: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
+00014390: 2074 7970 652c 0a20 2020 2020 2020 207a   type,.        z
+000143a0: 3d4e 6f6e 652c 0a20 2020 2020 2020 2078  =None,.        x
+000143b0: 7365 6374 696f 6e5f 626f 756e 6473 3d4e  section_bounds=N
+000143c0: 6f6e 652c 0a20 2020 2020 2020 206c 6179  one,.        lay
+000143d0: 6572 5f73 7461 636b 3d4e 6f6e 652c 0a20  er_stack=None,. 
+000143e0: 2020 2020 2020 2077 6166 6572 5f70 6164         wafer_pad
+000143f0: 6469 6e67 3d30 2e30 2c0a 2020 2020 2020  ding=0.0,.      
+00014400: 2020 7761 6665 725f 6c61 7965 723d 4c41    wafer_layer=LA
+00014410: 5945 522e 5741 4645 522c 0a20 2020 2020  YER.WAFER,.     
+00014420: 2020 202a 6172 6773 2c0a 2020 2020 2020     *args,.      
+00014430: 2020 2a2a 6b77 6172 6773 2c0a 2020 2020    **kwargs,.    
+00014440: 293a 0a20 2020 2020 2020 2022 2222 5265  ):.        """Re
+00014450: 7475 726e 7320 6120 676d 7368 206d 7368  turns a gmsh msh
+00014460: 206f 6620 7468 6520 636f 6d70 6f6e 656e   of the componen
+00014470: 7420 666f 7220 6669 6e69 7465 2065 6c65  t for finite ele
+00014480: 6d65 6e74 2073 696d 756c 6174 696f 6e2e  ment simulation.
+00014490: 0a0a 2020 2020 2020 2020 4172 6775 6d65  ..        Argume
+000144a0: 6e74 733a 0a20 2020 2020 2020 2020 2020  nts:.           
+000144b0: 2074 7970 653a 206f 6e65 206f 6620 2278   type: one of "x
+000144c0: 7922 2c20 2275 7a22 2c20 6f72 2022 3344  y", "uz", or "3D
+000144d0: 222e 2044 6574 6572 6d69 6e65 7320 7468  ". Determines th
+000144e0: 6520 7479 7065 206f 6620 6d65 7368 2074  e type of mesh t
+000144f0: 6f20 7265 7475 726e 2e0a 2020 2020 2020  o return..      
+00014500: 2020 2020 2020 7a3a 2075 7365 6420 746f        z: used to
+00014510: 2064 6566 696e 6520 7a2d 736c 6963 6520   define z-slice 
+00014520: 666f 7220 7879 206d 6573 6869 6e67 0a20  for xy meshing. 
+00014530: 2020 2020 2020 2020 2020 2078 7365 6374             xsect
+00014540: 696f 6e5f 626f 756e 6473 3a20 7573 6564  ion_bounds: used
+00014550: 2074 6f20 6465 6669 6e65 2069 6e2d 706c   to define in-pl
+00014560: 616e 6520 6c69 6e65 2066 6f72 2075 7a20  ane line for uz 
+00014570: 6d65 7368 696e 670a 2020 2020 2020 2020  meshing.        
+00014580: 2020 2020 7761 6665 725f 7061 6464 696e      wafer_paddin
+00014590: 673a 2070 6164 6469 6e67 2062 6579 6f6e  g: padding beyon
+000145a0: 6420 6262 6f78 2074 6f20 6164 6420 746f  d bbox to add to
+000145b0: 2057 4146 4552 206c 6179 6572 732e 0a0a   WAFER layers...
+000145c0: 2020 2020 2020 2020 4b65 7977 6f72 6420          Keyword 
+000145d0: 4172 6773 3a0a 2020 2020 2020 2020 2020  Args:.          
+000145e0: 2020 4172 6775 6d65 6e74 7320 666f 7220    Arguments for 
+000145f0: 7468 6520 7461 7267 6574 206d 6573 6869  the target meshi
+00014600: 6e67 2066 756e 6374 696f 6e20 696e 2067  ng function in g
+00014610: 6473 6661 6374 6f72 792e 7369 6d75 6c61  dsfactory.simula
+00014620: 7469 6f6e 2e67 6d73 680a 2020 2020 2020  tion.gmsh.      
+00014630: 2020 2222 220a 2020 2020 2020 2020 2320    """.        # 
+00014640: 4164 6420 5741 4645 5220 6c61 7965 723a  Add WAFER layer:
+00014650: 0a20 2020 2020 2020 2070 6164 6465 645f  .        padded_
+00014660: 636f 6d70 6f6e 656e 7420 3d20 436f 6d70  component = Comp
+00014670: 6f6e 656e 7428 290a 2020 2020 2020 2020  onent().        
+00014680: 7061 6464 6564 5f63 6f6d 706f 6e65 6e74  padded_component
+00014690: 203c 3c20 7365 6c66 0a20 2020 2020 2020   << self.       
+000146a0: 2028 786d 696e 2c20 796d 696e 292c 2028   (xmin, ymin), (
+000146b0: 786d 6178 2c20 796d 6178 2920 3d20 7365  xmax, ymax) = se
+000146c0: 6c66 2e62 626f 780a 2020 2020 2020 2020  lf.bbox.        
+000146d0: 706f 696e 7473 203d 205b 0a20 2020 2020  points = [.     
+000146e0: 2020 2020 2020 205b 786d 696e 202d 2077         [xmin - w
+000146f0: 6166 6572 5f70 6164 6469 6e67 2c20 796d  afer_padding, ym
+00014700: 696e 202d 2077 6166 6572 5f70 6164 6469  in - wafer_paddi
+00014710: 6e67 5d2c 0a20 2020 2020 2020 2020 2020  ng],.           
+00014720: 205b 786d 6178 202b 2077 6166 6572 5f70   [xmax + wafer_p
+00014730: 6164 6469 6e67 2c20 796d 696e 202d 2077  adding, ymin - w
+00014740: 6166 6572 5f70 6164 6469 6e67 5d2c 0a20  afer_padding],. 
+00014750: 2020 2020 2020 2020 2020 205b 786d 6178             [xmax
+00014760: 202b 2077 6166 6572 5f70 6164 6469 6e67   + wafer_padding
+00014770: 2c20 796d 6178 202b 2077 6166 6572 5f70  , ymax + wafer_p
+00014780: 6164 6469 6e67 5d2c 0a20 2020 2020 2020  adding],.       
+00014790: 2020 2020 205b 786d 696e 202d 2077 6166       [xmin - waf
+000147a0: 6572 5f70 6164 6469 6e67 2c20 796d 6178  er_padding, ymax
+000147b0: 202b 2077 6166 6572 5f70 6164 6469 6e67   + wafer_padding
+000147c0: 5d2c 0a20 2020 2020 2020 205d 0a20 2020  ],.        ].   
+000147d0: 2020 2020 2070 6164 6465 645f 636f 6d70       padded_comp
+000147e0: 6f6e 656e 742e 6164 645f 706f 6c79 676f  onent.add_polygo
+000147f0: 6e28 706f 696e 7473 2c20 6c61 7965 723d  n(points, layer=
+00014800: 7761 6665 725f 6c61 7965 7229 0a0a 2020  wafer_layer)..  
+00014810: 2020 2020 2020 6966 206c 6179 6572 5f73        if layer_s
+00014820: 7461 636b 2069 7320 4e6f 6e65 3a0a 2020  tack is None:.  
+00014830: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+00014840: 5661 6c75 6545 7272 6f72 280a 2020 2020  ValueError(.    
+00014850: 2020 2020 2020 2020 2020 2020 2741 204c              'A L
+00014860: 6179 6572 5374 6163 6b20 6d75 7374 2062  ayerStack must b
+00014870: 6520 7072 6f76 6964 6564 2074 6872 6f75  e provided throu
+00014880: 6768 2061 7267 756d 656e 7420 226c 6179  gh argument "lay
+00014890: 6572 5f73 7461 636b 222e 270a 2020 2020  er_stack".'.    
+000148a0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
+000148b0: 2020 6966 2074 7970 6520 3d3d 2022 7879    if type == "xy
+000148c0: 223a 0a20 2020 2020 2020 2020 2020 2069  ":.            i
+000148d0: 6620 7a20 6973 204e 6f6e 653a 0a20 2020  f z is None:.   
+000148e0: 2020 2020 2020 2020 2020 2020 2072 6169               rai
+000148f0: 7365 2056 616c 7565 4572 726f 7228 0a20  se ValueError(. 
+00014900: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014910: 2020 2027 466f 7220 7879 2d6d 6573 6869     'For xy-meshi
+00014920: 6e67 2c20 6120 7a2d 7661 6c75 6520 6d75  ng, a z-value mu
+00014930: 7374 2062 6520 7072 6f76 6964 6564 2076  st be provided v
+00014940: 6961 2074 6865 2066 6c6f 6174 2061 7267  ia the float arg
+00014950: 756d 656e 7420 227a 222e 270a 2020 2020  ument "z".'.    
+00014960: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+00014970: 2020 2020 2020 2020 2020 6672 6f6d 2067            from g
+00014980: 6473 6661 6374 6f72 792e 7369 6d75 6c61  dsfactory.simula
+00014990: 7469 6f6e 2e67 6d73 682e 7879 5f78 7365  tion.gmsh.xy_xse
+000149a0: 6374 696f 6e5f 6d65 7368 2069 6d70 6f72  ction_mesh impor
+000149b0: 7420 7879 5f78 7365 6374 696f 6e5f 6d65  t xy_xsection_me
+000149c0: 7368 0a0a 2020 2020 2020 2020 2020 2020  sh..            
+000149d0: 7265 7475 726e 2078 795f 7873 6563 7469  return xy_xsecti
+000149e0: 6f6e 5f6d 6573 6828 7061 6464 6564 5f63  on_mesh(padded_c
+000149f0: 6f6d 706f 6e65 6e74 2c20 7a2c 206c 6179  omponent, z, lay
+00014a00: 6572 5f73 7461 636b 2c20 2a2a 6b77 6172  er_stack, **kwar
+00014a10: 6773 290a 2020 2020 2020 2020 656c 6966  gs).        elif
+00014a20: 2074 7970 6520 3d3d 2022 757a 223a 0a20   type == "uz":. 
+00014a30: 2020 2020 2020 2020 2020 2069 6620 7873             if xs
+00014a40: 6563 7469 6f6e 5f62 6f75 6e64 7320 6973  ection_bounds is
+00014a50: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00014a60: 2020 2020 2020 2072 6169 7365 2056 616c         raise Val
+00014a70: 7565 4572 726f 7228 0a20 2020 2020 2020  ueError(.       
+00014a80: 2020 2020 2020 2020 2020 2020 2022 466f               "Fo
+00014a90: 7220 757a 2d6d 6573 6869 6e67 2c20 796f  r uz-meshing, yo
+00014aa0: 7520 6d75 7374 2070 726f 7669 6465 2061  u must provide a
+00014ab0: 206c 696e 6520 696e 2074 6865 2078 792d   line in the xy-
+00014ac0: 706c 616e 6520 220a 2020 2020 2020 2020  plane ".        
+00014ad0: 2020 2020 2020 2020 2020 2020 2276 6961              "via
+00014ae0: 2074 6865 2054 7570 6c65 2061 7267 756d   the Tuple argum
+00014af0: 656e 7420 5b5b 7831 2c79 315d 2c20 5b78  ent [[x1,y1], [x
+00014b00: 322c 7932 5d5d 2078 7365 6374 696f 6e5f  2,y2]] xsection_
+00014b10: 626f 756e 6473 2e22 0a20 2020 2020 2020  bounds.".       
+00014b20: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
+00014b30: 2020 2020 2020 2066 726f 6d20 6764 7366         from gdsf
+00014b40: 6163 746f 7279 2e73 696d 756c 6174 696f  actory.simulatio
+00014b50: 6e2e 676d 7368 2e75 7a5f 7873 6563 7469  n.gmsh.uz_xsecti
+00014b60: 6f6e 5f6d 6573 6820 696d 706f 7274 2075  on_mesh import u
+00014b70: 7a5f 7873 6563 7469 6f6e 5f6d 6573 680a  z_xsection_mesh.
+00014b80: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00014b90: 7572 6e20 757a 5f78 7365 6374 696f 6e5f  urn uz_xsection_
+00014ba0: 6d65 7368 280a 2020 2020 2020 2020 2020  mesh(.          
+00014bb0: 2020 2020 2020 7061 6464 6564 5f63 6f6d        padded_com
+00014bc0: 706f 6e65 6e74 2c20 7873 6563 7469 6f6e  ponent, xsection
+00014bd0: 5f62 6f75 6e64 732c 206c 6179 6572 5f73  _bounds, layer_s
+00014be0: 7461 636b 2c20 2a2a 6b77 6172 6773 0a20  tack, **kwargs. 
+00014bf0: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+00014c00: 2020 2020 2065 6c69 6620 7479 7065 203d       elif type =
+00014c10: 3d20 2233 4422 3a0a 2020 2020 2020 2020  = "3D":.        
+00014c20: 2020 2020 6672 6f6d 2067 6473 6661 6374      from gdsfact
+00014c30: 6f72 792e 7369 6d75 6c61 7469 6f6e 2e67  ory.simulation.g
+00014c40: 6d73 682e 7879 7a5f 6d65 7368 2069 6d70  msh.xyz_mesh imp
+00014c50: 6f72 7420 7879 7a5f 6d65 7368 0a0a 2020  ort xyz_mesh..  
+00014c60: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00014c70: 2078 797a 5f6d 6573 6828 7061 6464 6564   xyz_mesh(padded
+00014c80: 5f63 6f6d 706f 6e65 6e74 2c20 6c61 7965  _component, laye
+00014c90: 725f 7374 6163 6b2c 202a 2a6b 7761 7267  r_stack, **kwarg
+00014ca0: 7329 0a20 2020 2020 2020 2065 6c73 653a  s).        else:
+00014cb0: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
+00014cc0: 7365 2056 616c 7565 4572 726f 7228 0a20  se ValueError(. 
+00014cd0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+00014ce0: 5265 7175 6972 6564 2061 7267 756d 656e  Required argumen
+00014cf0: 7420 2274 7970 6522 206d 7573 7420 6265  t "type" must be
+00014d00: 206f 6e65 206f 6620 2278 7922 2c20 2275   one of "xy", "u
+00014d10: 7a22 2c20 6f72 2022 3344 222e 270a 2020  z", or "3D".'.  
+00014d20: 2020 2020 2020 2020 2020 290a 0a20 2020            )..   
+00014d30: 2064 6566 206f 6666 7365 7428 0a20 2020   def offset(.   
+00014d40: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
+00014d50: 2020 2064 6973 7461 6e63 653a 2066 6c6f     distance: flo
+00014d60: 6174 203d 2030 2e31 2c0a 2020 2020 2020  at = 0.1,.      
+00014d70: 2020 706f 6c79 676f 6e73 3d4e 6f6e 652c    polygons=None,
+00014d80: 0a20 2020 2020 2020 2075 7365 5f75 6e69  .        use_uni
+00014d90: 6f6e 3a20 626f 6f6c 203d 2054 7275 652c  on: bool = True,
+00014da0: 0a20 2020 2020 2020 2070 7265 6369 7369  .        precisi
+00014db0: 6f6e 3a20 666c 6f61 7420 3d20 3165 2d34  on: float = 1e-4
+00014dc0: 2c0a 2020 2020 2020 2020 6a6f 696e 3a20  ,.        join: 
+00014dd0: 7374 7220 3d20 226d 6974 6572 222c 0a20  str = "miter",. 
+00014de0: 2020 2020 2020 2074 6f6c 6572 616e 6365         tolerance
+00014df0: 3a20 696e 7420 3d20 322c 0a20 2020 2020  : int = 2,.     
+00014e00: 2020 206c 6179 6572 3a20 4c61 7965 7253     layer: LayerS
+00014e10: 7065 6320 3d20 2257 4722 2c0a 2020 2020  pec = "WG",.    
+00014e20: 2920 2d3e 2043 6f6d 706f 6e65 6e74 3a0a  ) -> Component:.
+00014e30: 2020 2020 2020 2020 2222 2252 6574 7572          """Retur
+00014e40: 6e73 206e 6577 2043 6f6d 706f 6e65 6e74  ns new Component
+00014e50: 2077 6974 6820 706f 6c79 676f 6e73 2065   with polygons e
+00014e60: 726f 6465 6420 6f72 2064 696c 6174 6564  roded or dilated
+00014e70: 2062 7920 616e 206f 6666 7365 742e 0a0a   by an offset...
+00014e80: 2020 2020 2020 2020 4172 6773 3a0a 2020          Args:.  
+00014e90: 2020 2020 2020 2020 2020 6469 7374 616e            distan
+00014ea0: 6365 3a20 4469 7374 616e 6365 2074 6f20  ce: Distance to 
+00014eb0: 6f66 6673 6574 2070 6f6c 7967 6f6e 732e  offset polygons.
+00014ec0: 2050 6f73 6974 6976 6520 7661 6c75 6573   Positive values
+00014ed0: 2065 7870 616e 642c 206e 6567 6174 6976   expand, negativ
+00014ee0: 6520 7368 7269 6e6b 2e0a 2020 2020 2020  e shrink..      
+00014ef0: 2020 2020 2020 7072 6563 6973 696f 6e3a        precision:
+00014f00: 2044 6573 6972 6564 2070 7265 6369 7369   Desired precisi
+00014f10: 6f6e 2066 6f72 2072 6f75 6e64 696e 6720  on for rounding 
+00014f20: 7665 7274 6578 2063 6f6f 7264 696e 6174  vertex coordinat
+00014f30: 6573 2e0a 2020 2020 2020 2020 2020 2020  es..            
+00014f40: 6a6f 696e 3a20 7b27 6d69 7465 7227 2c20  join: {'miter', 
+00014f50: 2762 6576 656c 272c 2027 726f 756e 6427  'bevel', 'round'
+00014f60: 7d20 5479 7065 206f 6620 6a6f 696e 2075  } Type of join u
+00014f70: 7365 6420 746f 2063 7265 6174 6520 706f  sed to create po
+00014f80: 6c79 676f 6e20 6f66 6673 6574 0a20 2020  lygon offset.   
+00014f90: 2020 2020 2020 2020 2074 6f6c 6572 616e           toleran
+00014fa0: 6365 3a20 466f 7220 6d69 7465 7220 6a6f  ce: For miter jo
+00014fb0: 696e 7473 2c20 7468 6973 206e 756d 6265  ints, this numbe
+00014fc0: 7220 6d75 7374 2062 6520 6174 206c 6561  r must be at lea
+00014fd0: 7374 2032 2072 6570 7265 7365 6e74 7320  st 2 represents 
+00014fe0: 7468 650a 2020 2020 2020 2020 2020 2020  the.            
+00014ff0: 2020 6d61 7869 6d61 6c20 6469 7374 616e    maximal distan
+00015000: 6365 2069 6e20 6d75 6c74 6970 6c65 7320  ce in multiples 
+00015010: 6f66 206f 6666 7365 7420 6265 7477 6565  of offset betwee
+00015020: 6e20 6e65 7720 7665 7274 6963 6573 2061  n new vertices a
+00015030: 6e64 2074 6865 6972 0a20 2020 2020 2020  nd their.       
+00015040: 2020 2020 2020 206f 7269 6769 6e61 6c20         original 
+00015050: 706f 7369 7469 6f6e 2062 6566 6f72 6520  position before 
+00015060: 6265 7665 6c69 6e67 2074 6f20 6176 6f69  beveling to avoi
+00015070: 6420 7370 696b 6573 2061 7420 6163 7574  d spikes at acut
+00015080: 6520 6a6f 696e 7473 2e20 466f 720a 2020  e joints. For.  
+00015090: 2020 2020 2020 2020 2020 2020 726f 756e              roun
+000150a0: 6420 6a6f 696e 7473 2c20 6974 2069 6e64  d joints, it ind
+000150b0: 6963 6174 6573 2074 6865 2063 7572 7661  icates the curva
+000150c0: 7475 7265 2072 6573 6f6c 7574 696f 6e20  ture resolution 
+000150d0: 696e 206e 756d 6265 7220 6f66 0a20 2020  in number of.   
+000150e0: 2020 2020 2020 2020 2020 2070 6f69 6e74             point
+000150f0: 7320 7065 7220 6675 6c6c 2063 6972 636c  s per full circl
+00015100: 652e 0a20 2020 2020 2020 2020 2020 206c  e..            l
+00015110: 6179 6572 3a20 5370 6563 6966 6963 206c  ayer: Specific l
+00015120: 6179 6572 2066 6f72 206e 6577 2070 6f6c  ayer for new pol
+00015130: 7967 6f6e 732e 0a0a 2020 2020 2020 2020  ygons...        
+00015140: 2222 220a 2020 2020 2020 2020 696d 706f  """.        impo
+00015150: 7274 2067 6473 6661 6374 6f72 7920 6173  rt gdsfactory as
+00015160: 2067 660a 0a20 2020 2020 2020 2067 6473   gf..        gds
+00015170: 5f6c 6179 6572 2c20 6764 735f 6461 7461  _layer, gds_data
+00015180: 7479 7065 203d 2067 662e 6765 745f 6c61  type = gf.get_la
+00015190: 7965 7228 6c61 7965 7229 0a20 2020 2020  yer(layer).     
+000151a0: 2020 2070 203d 2067 6473 746b 2e6f 6666     p = gdstk.off
+000151b0: 7365 7428 0a20 2020 2020 2020 2020 2020  set(.           
+000151c0: 2070 6f6c 7967 6f6e 7320 6f72 2073 656c   polygons or sel
+000151d0: 662e 6765 745f 706f 6c79 676f 6e73 2829  f.get_polygons()
+000151e0: 2c0a 2020 2020 2020 2020 2020 2020 6469  ,.            di
+000151f0: 7374 616e 6365 3d64 6973 7461 6e63 652c  stance=distance,
+00015200: 0a20 2020 2020 2020 2020 2020 206a 6f69  .            joi
+00015210: 6e3d 6a6f 696e 2c0a 2020 2020 2020 2020  n=join,.        
+00015220: 2020 2020 746f 6c65 7261 6e63 653d 746f      tolerance=to
+00015230: 6c65 7261 6e63 652c 0a20 2020 2020 2020  lerance,.       
+00015240: 2020 2020 2070 7265 6369 7369 6f6e 3d70       precision=p
+00015250: 7265 6369 7369 6f6e 2c0a 2020 2020 2020  recision,.      
+00015260: 2020 2020 2020 7573 655f 756e 696f 6e3d        use_union=
+00015270: 7573 655f 756e 696f 6e2c 0a20 2020 2020  use_union,.     
+00015280: 2020 2020 2020 206c 6179 6572 3d67 6473         layer=gds
+00015290: 5f6c 6179 6572 2c0a 2020 2020 2020 2020  _layer,.        
+000152a0: 2020 2020 6461 7461 7479 7065 3d67 6473      datatype=gds
+000152b0: 5f64 6174 6174 7970 652c 0a20 2020 2020  _datatype,.     
+000152c0: 2020 2029 0a0a 2020 2020 2020 2020 636f     )..        co
+000152d0: 6d70 6f6e 656e 7420 3d20 6766 2e43 6f6d  mponent = gf.Com
+000152e0: 706f 6e65 6e74 2829 0a20 2020 2020 2020  ponent().       
+000152f0: 2063 6f6d 706f 6e65 6e74 2e61 6464 5f70   component.add_p
+00015300: 6f6c 7967 6f6e 2870 2c20 6c61 7965 723d  olygon(p, layer=
+00015310: 6c61 7965 7229 0a20 2020 2020 2020 2072  layer).        r
+00015320: 6574 7572 6e20 636f 6d70 6f6e 656e 740a  eturn component.
+00015330: 0a0a 6465 6620 636f 7079 280a 2020 2020  ..def copy(.    
+00015340: 443a 2043 6f6d 706f 6e65 6e74 2c0a 2020  D: Component,.  
+00015350: 2020 7265 6665 7265 6e63 6573 3d4e 6f6e    references=Non
+00015360: 652c 0a20 2020 2070 6f72 7473 3d4e 6f6e  e,.    ports=Non
+00015370: 652c 0a20 2020 2070 6f6c 7967 6f6e 733d  e,.    polygons=
+00015380: 4e6f 6e65 2c0a 2020 2020 7061 7468 733d  None,.    paths=
+00015390: 4e6f 6e65 2c0a 2020 2020 6e61 6d65 3d4e  None,.    name=N
+000153a0: 6f6e 652c 0a20 2020 206c 6162 656c 733d  one,.    labels=
+000153b0: 4e6f 6e65 2c0a 2920 2d3e 2043 6f6d 706f  None,.) -> Compo
+000153c0: 6e65 6e74 3a0a 2020 2020 2222 2252 6574  nent:.    """Ret
+000153d0: 7572 6e73 2061 2043 6f6d 706f 6e65 6e74  urns a Component
+000153e0: 2063 6f70 792e 0a0a 2020 2020 4172 6773   copy...    Args
+000153f0: 3a0a 2020 2020 2020 2020 443a 2063 6f6d  :.        D: com
+00015400: 706f 6e65 6e74 2074 6f20 636f 7079 2e0a  ponent to copy..
+00015410: 2020 2020 2222 220a 2020 2020 445f 636f      """.    D_co
+00015420: 7079 203d 2043 6f6d 706f 6e65 6e74 2829  py = Component()
+00015430: 0a20 2020 2044 5f63 6f70 792e 696e 666f  .    D_copy.info
+00015440: 203d 2044 2e69 6e66 6f0a 2020 2020 2320   = D.info.    # 
+00015450: 445f 636f 7079 2e5f 6365 6c6c 203d 2044  D_copy._cell = D
+00015460: 2e5f 6365 6c6c 2e63 6f70 7928 6e61 6d65  ._cell.copy(name
+00015470: 3d44 5f63 6f70 792e 6e61 6d65 290a 0a20  =D_copy.name).. 
+00015480: 2020 2066 6f72 2072 6566 2069 6e20 7265     for ref in re
+00015490: 6665 7265 6e63 6573 2069 6620 7265 6665  ferences if refe
+000154a0: 7265 6e63 6573 2069 7320 6e6f 7420 4e6f  rences is not No
+000154b0: 6e65 2065 6c73 6520 442e 7265 6665 7265  ne else D.refere
+000154c0: 6e63 6573 3a0a 2020 2020 2020 2020 445f  nces:.        D_
+000154d0: 636f 7079 2e61 6464 2863 6f70 795f 7265  copy.add(copy_re
+000154e0: 6665 7265 6e63 6528 7265 6629 290a 2020  ference(ref)).  
+000154f0: 2020 666f 7220 706f 7274 2069 6e20 2870    for port in (p
+00015500: 6f72 7473 2069 6620 706f 7274 7320 6973  orts if ports is
+00015510: 206e 6f74 204e 6f6e 6520 656c 7365 2044   not None else D
+00015520: 2e70 6f72 7473 292e 7661 6c75 6573 2829  .ports).values()
+00015530: 3a0a 2020 2020 2020 2020 445f 636f 7079  :.        D_copy
+00015540: 2e61 6464 5f70 6f72 7428 706f 7274 3d70  .add_port(port=p
+00015550: 6f72 7429 0a20 2020 2066 6f72 2070 6f6c  ort).    for pol
+00015560: 7920 696e 2070 6f6c 7967 6f6e 7320 6966  y in polygons if
+00015570: 2070 6f6c 7967 6f6e 7320 6973 206e 6f74   polygons is not
+00015580: 204e 6f6e 6520 656c 7365 2044 2e70 6f6c   None else D.pol
+00015590: 7967 6f6e 733a 0a20 2020 2020 2020 2044  ygons:.        D
+000155a0: 5f63 6f70 792e 6164 645f 706f 6c79 676f  _copy.add_polygo
+000155b0: 6e28 706f 6c79 290a 2020 2020 666f 7220  n(poly).    for 
+000155c0: 7061 7468 2069 6e20 7061 7468 7320 6966  path in paths if
+000155d0: 2070 6174 6873 2069 7320 6e6f 7420 4e6f   paths is not No
+000155e0: 6e65 2065 6c73 6520 442e 7061 7468 733a  ne else D.paths:
+000155f0: 0a20 2020 2020 2020 2044 5f63 6f70 792e  .        D_copy.
+00015600: 6164 6428 7061 7468 290a 2020 2020 666f  add(path).    fo
+00015610: 7220 6c61 6265 6c20 696e 206c 6162 656c  r label in label
+00015620: 7320 6966 206c 6162 656c 7320 6973 206e  s if labels is n
+00015630: 6f74 204e 6f6e 6520 656c 7365 2044 2e6c  ot None else D.l
+00015640: 6162 656c 733a 0a20 2020 2020 2020 2044  abels:.        D
+00015650: 5f63 6f70 792e 6164 645f 6c61 6265 6c28  _copy.add_label(
+00015660: 0a20 2020 2020 2020 2020 2020 2074 6578  .            tex
+00015670: 743d 6c61 6265 6c2e 7465 7874 2c0a 2020  t=label.text,.  
+00015680: 2020 2020 2020 2020 2020 706f 7369 7469            positi
+00015690: 6f6e 3d6c 6162 656c 2e6f 7269 6769 6e2c  on=label.origin,
+000156a0: 0a20 2020 2020 2020 2020 2020 206c 6179  .            lay
+000156b0: 6572 3d28 6c61 6265 6c2e 6c61 7965 722c  er=(label.layer,
+000156c0: 206c 6162 656c 2e74 6578 7474 7970 6529   label.texttype)
+000156d0: 2c0a 2020 2020 2020 2020 290a 0a20 2020  ,.        )..   
+000156e0: 2069 6620 6e61 6d65 2069 7320 6e6f 7420   if name is not 
+000156f0: 4e6f 6e65 3a0a 2020 2020 2020 2020 445f  None:.        D_
+00015700: 636f 7079 2e6e 616d 6520 3d20 6e61 6d65  copy.name = name
+00015710: 0a0a 2020 2020 7265 7475 726e 2044 5f63  ..    return D_c
+00015720: 6f70 790a 0a0a 6465 6620 636f 7079 5f72  opy...def copy_r
+00015730: 6566 6572 656e 6365 280a 2020 2020 7265  eference(.    re
+00015740: 662c 0a20 2020 2070 6172 656e 743d 4e6f  f,.    parent=No
+00015750: 6e65 2c0a 2020 2020 636f 6c75 6d6e 733d  ne,.    columns=
+00015760: 4e6f 6e65 2c0a 2020 2020 726f 7773 3d4e  None,.    rows=N
+00015770: 6f6e 652c 0a20 2020 2073 7061 6369 6e67  one,.    spacing
+00015780: 3d4e 6f6e 652c 0a20 2020 206f 7269 6769  =None,.    origi
+00015790: 6e3d 4e6f 6e65 2c0a 2020 2020 726f 7461  n=None,.    rota
+000157a0: 7469 6f6e 3d4e 6f6e 652c 0a20 2020 206d  tion=None,.    m
+000157b0: 6167 6e69 6669 6361 7469 6f6e 3d4e 6f6e  agnification=Non
+000157c0: 652c 0a20 2020 2078 5f72 6566 6c65 6374  e,.    x_reflect
+000157d0: 696f 6e3d 4e6f 6e65 2c0a 2020 2020 6e61  ion=None,.    na
+000157e0: 6d65 3d4e 6f6e 652c 0a20 2020 2076 313d  me=None,.    v1=
+000157f0: 4e6f 6e65 2c0a 2020 2020 7632 3d4e 6f6e  None,.    v2=Non
+00015800: 652c 0a29 202d 3e20 436f 6d70 6f6e 656e  e,.) -> Componen
+00015810: 7452 6566 6572 656e 6365 3a0a 2020 2020  tReference:.    
+00015820: 7265 7475 726e 2043 6f6d 706f 6e65 6e74  return Component
+00015830: 5265 6665 7265 6e63 6528 0a20 2020 2020  Reference(.     
+00015840: 2020 2063 6f6d 706f 6e65 6e74 3d70 6172     component=par
+00015850: 656e 7420 6f72 2072 6566 2e70 6172 656e  ent or ref.paren
+00015860: 742c 0a20 2020 2020 2020 2063 6f6c 756d  t,.        colum
+00015870: 6e73 3d63 6f6c 756d 6e73 206f 7220 7265  ns=columns or re
+00015880: 662e 636f 6c75 6d6e 732c 0a20 2020 2020  f.columns,.     
+00015890: 2020 2072 6f77 733d 726f 7773 206f 7220     rows=rows or 
+000158a0: 7265 662e 726f 7773 2c0a 2020 2020 2020  ref.rows,.      
+000158b0: 2020 7370 6163 696e 673d 7370 6163 696e    spacing=spacin
+000158c0: 6720 6f72 2072 6566 2e73 7061 6369 6e67  g or ref.spacing
+000158d0: 2c0a 2020 2020 2020 2020 6f72 6967 696e  ,.        origin
+000158e0: 3d6f 7269 6769 6e20 6f72 2072 6566 2e6f  =origin or ref.o
+000158f0: 7269 6769 6e2c 0a20 2020 2020 2020 2072  rigin,.        r
+00015900: 6f74 6174 696f 6e3d 726f 7461 7469 6f6e  otation=rotation
+00015910: 206f 7220 7265 662e 726f 7461 7469 6f6e   or ref.rotation
+00015920: 2c0a 2020 2020 2020 2020 6d61 676e 6966  ,.        magnif
+00015930: 6963 6174 696f 6e3d 6d61 676e 6966 6963  ication=magnific
+00015940: 6174 696f 6e20 6f72 2072 6566 2e6d 6167  ation or ref.mag
+00015950: 6e69 6669 6361 7469 6f6e 2c0a 2020 2020  nification,.    
+00015960: 2020 2020 785f 7265 666c 6563 7469 6f6e      x_reflection
+00015970: 3d78 5f72 6566 6c65 6374 696f 6e20 6f72  =x_reflection or
+00015980: 2072 6566 2e78 5f72 6566 6c65 6374 696f   ref.x_reflectio
+00015990: 6e2c 0a20 2020 2020 2020 206e 616d 653d  n,.        name=
+000159a0: 6e61 6d65 206f 7220 7265 662e 6e61 6d65  name or ref.name
+000159b0: 2c0a 2020 2020 2020 2020 7631 3d76 3120  ,.        v1=v1 
+000159c0: 6f72 2072 6566 2e76 312c 0a20 2020 2020  or ref.v1,.     
+000159d0: 2020 2076 323d 7632 206f 7220 7265 662e     v2=v2 or ref.
+000159e0: 7632 2c0a 2020 2020 290a 0a0a 6465 6620  v2,.    )...def 
+000159f0: 7465 7374 5f67 6574 5f6c 6179 6572 7328  test_get_layers(
+00015a00: 2920 2d3e 2043 6f6d 706f 6e65 6e74 3a0a  ) -> Component:.
+00015a10: 2020 2020 696d 706f 7274 2067 6473 6661      import gdsfa
+00015a20: 6374 6f72 7920 6173 2067 660a 0a20 2020  ctory as gf..   
+00015a30: 2063 3120 3d20 6766 2e63 6f6d 706f 6e65   c1 = gf.compone
+00015a40: 6e74 732e 7374 7261 6967 6874 280a 2020  nts.straight(.  
+00015a50: 2020 2020 2020 6c65 6e67 7468 3d31 302c        length=10,
+00015a60: 0a20 2020 2020 2020 2077 6964 7468 3d30  .        width=0
+00015a70: 2e35 2c0a 2020 2020 2020 2020 6c61 7965  .5,.        laye
+00015a80: 723d 2832 2c20 3029 2c0a 2020 2020 2020  r=(2, 0),.      
+00015a90: 2020 6262 6f78 5f6c 6179 6572 733d 5b28    bbox_layers=[(
+00015aa0: 3131 312c 2030 295d 2c0a 2020 2020 2020  111, 0)],.      
+00015ab0: 2020 6262 6f78 5f6f 6666 7365 7473 3d5b    bbox_offsets=[
+00015ac0: 335d 2c0a 2020 2020 2020 2020 7769 7468  3],.        with
+00015ad0: 5f62 626f 783d 5472 7565 2c0a 2020 2020  _bbox=True,.    
+00015ae0: 2020 2020 636c 6164 6469 6e67 5f6c 6179      cladding_lay
+00015af0: 6572 733d 4e6f 6e65 2c0a 2020 2020 2020  ers=None,.      
+00015b00: 2020 6164 645f 7069 6e73 3d4e 6f6e 652c    add_pins=None,
+00015b10: 0a20 2020 2020 2020 2061 6464 5f62 626f  .        add_bbo
+00015b20: 783d 4e6f 6e65 2c0a 2020 2020 290a 2020  x=None,.    ).  
+00015b30: 2020 6173 7365 7274 2063 312e 6765 745f    assert c1.get_
+00015b40: 6c61 7965 7273 2829 203d 3d20 7b28 322c  layers() == {(2,
+00015b50: 2030 292c 2028 3131 312c 2030 297d 2c20   0), (111, 0)}, 
+00015b60: 6331 2e67 6574 5f6c 6179 6572 7328 290a  c1.get_layers().
+00015b70: 2020 2020 2320 7265 7475 726e 2063 310a      # return c1.
+00015b80: 2020 2020 6332 203d 2063 312e 7265 6d6f      c2 = c1.remo
+00015b90: 7665 5f6c 6179 6572 7328 5b28 3131 312c  ve_layers([(111,
+00015ba0: 2030 295d 290a 2020 2020 6173 7365 7274   0)]).    assert
+00015bb0: 2063 322e 6765 745f 6c61 7965 7273 2829   c2.get_layers()
+00015bc0: 203d 3d20 7b28 322c 2030 297d 2c20 6332   == {(2, 0)}, c2
+00015bd0: 2e67 6574 5f6c 6179 6572 7328 290a 2020  .get_layers().  
+00015be0: 2020 7265 7475 726e 2063 320a 0a0a 6465    return c2...de
+00015bf0: 6620 5f66 696c 7465 725f 706f 6c79 7328  f _filter_polys(
+00015c00: 706f 6c79 676f 6e73 2c20 6c61 7965 7273  polygons, layers
+00015c10: 5f65 7863 6c29 3a0a 2020 2020 7265 7475  _excl):.    retu
+00015c20: 726e 205b 0a20 2020 2020 2020 2070 6f6c  rn [.        pol
+00015c30: 7967 6f6e 0a20 2020 2020 2020 2066 6f72  ygon.        for
+00015c40: 2070 6f6c 7967 6f6e 2c20 6c61 7965 722c   polygon, layer,
+00015c50: 2064 6174 6174 7970 6520 696e 207a 6970   datatype in zip
+00015c60: 280a 2020 2020 2020 2020 2020 2020 706f  (.            po
+00015c70: 6c79 676f 6e73 2e70 6f6c 7967 6f6e 732c  lygons.polygons,
+00015c80: 2070 6f6c 7967 6f6e 732e 6c61 7965 7273   polygons.layers
+00015c90: 2c20 706f 6c79 676f 6e73 2e64 6174 6174  , polygons.datat
+00015ca0: 7970 6573 0a20 2020 2020 2020 2029 0a20  ypes.        ). 
+00015cb0: 2020 2020 2020 2069 6620 286c 6179 6572         if (layer
+00015cc0: 2c20 6461 7461 7479 7065 2920 6e6f 7420  , datatype) not 
+00015cd0: 696e 206c 6179 6572 735f 6578 636c 0a20  in layers_excl. 
+00015ce0: 2020 205d 0a0a 0a64 6566 2072 6563 7572     ]...def recur
+00015cf0: 7365 5f73 7472 7563 7475 7265 7328 0a20  se_structures(. 
+00015d00: 2020 2063 6f6d 706f 6e65 6e74 3a20 436f     component: Co
+00015d10: 6d70 6f6e 656e 742c 0a20 2020 2069 676e  mponent,.    ign
+00015d20: 6f72 655f 636f 6d70 6f6e 656e 7473 5f70  ore_components_p
+00015d30: 7265 6669 783a 204f 7074 696f 6e61 6c5b  refix: Optional[
+00015d40: 4c69 7374 5b73 7472 5d5d 203d 204e 6f6e  List[str]] = Non
+00015d50: 652c 0a20 2020 2069 676e 6f72 655f 6675  e,.    ignore_fu
+00015d60: 6e63 7469 6f6e 735f 7072 6566 6978 3a20  nctions_prefix: 
+00015d70: 4f70 7469 6f6e 616c 5b4c 6973 745b 7374  Optional[List[st
+00015d80: 725d 5d20 3d20 4e6f 6e65 2c0a 2920 2d3e  r]] = None,.) ->
+00015d90: 2044 6963 745b 7374 722c 2041 6e79 5d3a   Dict[str, Any]:
+00015da0: 0a20 2020 2022 2222 5265 6375 7273 6520  .    """Recurse 
+00015db0: 636f 6d70 6f6e 656e 7420 616e 6420 636f  component and co
+00015dc0: 6d70 6f6e 656e 7473 2072 6566 6572 656e  mponents referen
+00015dd0: 6365 7320 7265 6375 7273 6976 656c 792e  ces recursively.
+00015de0: 0a0a 2020 2020 4172 6773 3a0a 2020 2020  ..    Args:.    
+00015df0: 2020 2020 636f 6d70 6f6e 656e 743a 2063      component: c
+00015e00: 6f6d 706f 6e65 6e74 2074 6f20 7265 6375  omponent to recu
+00015e10: 7273 652e 0a20 2020 2020 2020 2069 676e  rse..        ign
+00015e20: 6f72 655f 636f 6d70 6f6e 656e 7473 5f70  ore_components_p
+00015e30: 7265 6669 783a 206c 6973 7420 6f66 2070  refix: list of p
+00015e40: 7265 6669 7820 746f 2069 676e 6f72 652e  refix to ignore.
+00015e50: 0a20 2020 2020 2020 2069 676e 6f72 655f  .        ignore_
+00015e60: 6675 6e63 7469 6f6e 735f 7072 6566 6978  functions_prefix
+00015e70: 3a20 6c69 7374 206f 6620 7072 6566 6978  : list of prefix
+00015e80: 2074 6f20 6967 6e6f 7265 2e0a 2020 2020   to ignore..    
+00015e90: 2222 220a 2020 2020 6967 6e6f 7265 5f66  """.    ignore_f
+00015ea0: 756e 6374 696f 6e73 5f70 7265 6669 7820  unctions_prefix 
+00015eb0: 3d20 6967 6e6f 7265 5f66 756e 6374 696f  = ignore_functio
+00015ec0: 6e73 5f70 7265 6669 7820 6f72 205b 5d0a  ns_prefix or [].
+00015ed0: 2020 2020 6967 6e6f 7265 5f63 6f6d 706f      ignore_compo
+00015ee0: 6e65 6e74 735f 7072 6566 6978 203d 2069  nents_prefix = i
+00015ef0: 676e 6f72 655f 636f 6d70 6f6e 656e 7473  gnore_components
+00015f00: 5f70 7265 6669 7820 6f72 205b 5d0a 0a20  _prefix or [].. 
+00015f10: 2020 2069 6620 280a 2020 2020 2020 2020     if (.        
+00015f20: 6861 7361 7474 7228 636f 6d70 6f6e 656e  hasattr(componen
+00015f30: 742c 2022 6675 6e63 7469 6f6e 5f6e 616d  t, "function_nam
+00015f40: 6522 290a 2020 2020 2020 2020 616e 6420  e").        and 
+00015f50: 636f 6d70 6f6e 656e 742e 6675 6e63 7469  component.functi
+00015f60: 6f6e 5f6e 616d 6520 696e 2069 676e 6f72  on_name in ignor
+00015f70: 655f 6675 6e63 7469 6f6e 735f 7072 6566  e_functions_pref
+00015f80: 6978 0a20 2020 2029 3a0a 2020 2020 2020  ix.    ):.      
+00015f90: 2020 7265 7475 726e 207b 7d0a 0a20 2020    return {}..   
+00015fa0: 2069 6620 6861 7361 7474 7228 636f 6d70   if hasattr(comp
+00015fb0: 6f6e 656e 742c 2022 6e61 6d65 2229 2061  onent, "name") a
+00015fc0: 6e64 2061 6e79 280a 2020 2020 2020 2020  nd any(.        
+00015fd0: 636f 6d70 6f6e 656e 742e 6e61 6d65 2e73  component.name.s
+00015fe0: 7461 7274 7377 6974 6828 6929 2066 6f72  tartswith(i) for
+00015ff0: 2069 2069 6e20 6967 6e6f 7265 5f63 6f6d   i in ignore_com
+00016000: 706f 6e65 6e74 735f 7072 6566 6978 0a20  ponents_prefix. 
+00016010: 2020 2029 3a0a 2020 2020 2020 2020 7265     ):.        re
+00016020: 7475 726e 207b 7d0a 0a20 2020 206f 7574  turn {}..    out
+00016030: 7075 7420 3d20 7b63 6f6d 706f 6e65 6e74  put = {component
+00016040: 2e6e 616d 653a 2064 6963 7428 636f 6d70  .name: dict(comp
+00016050: 6f6e 656e 742e 7365 7474 696e 6773 297d  onent.settings)}
+00016060: 0a20 2020 2066 6f72 2072 6566 6572 656e  .    for referen
+00016070: 6365 2069 6e20 636f 6d70 6f6e 656e 742e  ce in component.
+00016080: 7265 6665 7265 6e63 6573 3a0a 2020 2020  references:.    
+00016090: 2020 2020 6966 2028 0a20 2020 2020 2020      if (.       
+000160a0: 2020 2020 2069 7369 6e73 7461 6e63 6528       isinstance(
+000160b0: 7265 6665 7265 6e63 652c 2043 6f6d 706f  reference, Compo
+000160c0: 6e65 6e74 5265 6665 7265 6e63 6529 0a20  nentReference). 
+000160d0: 2020 2020 2020 2020 2020 2061 6e64 2072             and r
+000160e0: 6566 6572 656e 6365 2e72 6566 5f63 656c  eference.ref_cel
+000160f0: 6c2e 6e61 6d65 206e 6f74 2069 6e20 6f75  l.name not in ou
+00016100: 7470 7574 0a20 2020 2020 2020 2029 3a0a  tput.        ):.
+00016110: 2020 2020 2020 2020 2020 2020 6f75 7470              outp
+00016120: 7574 2e75 7064 6174 6528 7265 6375 7273  ut.update(recurs
+00016130: 655f 7374 7275 6374 7572 6573 2872 6566  e_structures(ref
+00016140: 6572 656e 6365 2e72 6566 5f63 656c 6c29  erence.ref_cell)
+00016150: 290a 0a20 2020 2072 6574 7572 6e20 6f75  )..    return ou
+00016160: 7470 7574 0a0a 0a64 6566 2066 6c61 7474  tput...def flatt
+00016170: 656e 5f69 6e76 616c 6964 5f72 6566 735f  en_invalid_refs_
+00016180: 7265 6375 7273 6976 6528 0a20 2020 2063  recursive(.    c
+00016190: 6f6d 706f 6e65 6e74 3a20 436f 6d70 6f6e  omponent: Compon
+000161a0: 656e 742c 0a20 2020 2067 7269 645f 7369  ent,.    grid_si
+000161b0: 7a65 3a20 4f70 7469 6f6e 616c 5b66 6c6f  ze: Optional[flo
+000161c0: 6174 5d20 3d20 4e6f 6e65 2c0a 2020 2020  at] = None,.    
+000161d0: 7570 6461 7465 645f 636f 6d70 6f6e 656e  updated_componen
+000161e0: 7473 3d4e 6f6e 652c 0a20 2020 2074 7261  ts=None,.    tra
+000161f0: 7665 7273 6564 5f63 6f6d 706f 6e65 6e74  versed_component
+00016200: 733d 4e6f 6e65 2c0a 293a 0a20 2020 2022  s=None,.):.    "
+00016210: 2222 5265 6375 7273 6976 656c 7920 666c  ""Recursively fl
+00016220: 6174 7465 6e73 2063 6f6d 706f 6e65 6e74  attens component
+00016230: 2072 6566 6572 656e 6365 7320 7768 6963   references whic
+00016240: 6820 6861 7665 2069 6e76 616c 6964 2074  h have invalid t
+00016250: 7261 6e73 666f 726d 6174 696f 6e73 2028  ransformations (
+00016260: 692e 652e 206e 6f6e 2d39 3020 6465 6720  i.e. non-90 deg 
+00016270: 726f 7461 7469 6f6e 7320 6f72 2073 7562  rotations or sub
+00016280: 2d67 7269 6420 7472 616e 736c 6174 696f  -grid translatio
+00016290: 6e73 2920 616e 6420 7265 7475 726e 7320  ns) and returns 
+000162a0: 6120 636f 7079 2069 6620 616e 7920 7375  a copy if any su
+000162b0: 6263 656c 6c73 2068 6176 6520 6265 656e  bcells have been
+000162c0: 206d 6f64 6966 6965 642e 0a0a 2020 2020   modified...    
+000162d0: 5741 524e 494e 473a 2074 6869 7320 6675  WARNING: this fu
+000162e0: 6e63 7469 6f6e 2077 696c 6c20 7072 6f64  nction will prod
+000162f0: 7563 6520 7361 6d65 2d6e 616d 6520 636f  uce same-name co
+00016300: 7069 6573 206f 6620 6365 6c6c 732e 2049  pies of cells. I
+00016310: 7420 6973 2073 7472 6963 746c 7920 6d65  t is strictly me
+00016320: 616e 7420 746f 2062 6520 7573 6564 206f  ant to be used o
+00016330: 6e20 7772 6974 6520 6f66 2074 6865 2047  n write of the G
+00016340: 4453 2066 696c 6520 616e 640a 2020 2020  DS file and.    
+00016350: 7368 6f75 6c64 206e 6f74 2062 6520 6d69  should not be mi
+00016360: 7865 6420 7769 7468 206f 7468 6572 2063  xed with other c
+00016370: 656c 6c73 2c20 6f72 2079 6f75 2077 696c  ells, or you wil
+00016380: 6c20 6c69 6b65 6c79 2065 7870 6572 6965  l likely experie
+00016390: 6e63 6520 6973 7375 6573 2077 6974 6820  nce issues with 
+000163a0: 6475 706c 6963 6174 6520 6365 6c6c 730a  duplicate cells.
+000163b0: 0a20 2020 2041 7267 733a 0a20 2020 2020  .    Args:.     
+000163c0: 2020 2063 6f6d 706f 6e65 6e74 3a20 7468     component: th
+000163d0: 6520 636f 6d70 6f6e 656e 7420 746f 2066  e component to f
+000163e0: 6978 2028 696e 2070 6c61 6365 292e 0a20  ix (in place).. 
+000163f0: 2020 2020 2020 2067 7269 645f 7369 7a65         grid_size
+00016400: 3a20 7468 6520 4744 5320 6772 6964 2073  : the GDS grid s
+00016410: 697a 652c 2069 6e20 756d 2c20 6465 6661  ize, in um, defa
+00016420: 756c 7473 2074 6f20 6163 7469 7665 2050  ults to active P
+00016430: 444b 2e67 6574 5f67 7269 645f 7369 7a65  DK.get_grid_size
+00016440: 2829 0a20 2020 2020 2020 2020 2020 2061  ().            a
+00016450: 6e79 2074 7261 6e73 6c61 7469 6f6e 7320  ny translations 
+00016460: 7769 7468 2068 6967 6865 7220 7265 736f  with higher reso
+00016470: 6c75 7469 6f6e 2074 6861 6e20 7468 6973  lution than this
+00016480: 2061 7265 2063 6f6e 7369 6465 7265 6420   are considered 
+00016490: 696e 7661 6c69 642e 0a20 2020 2020 2020  invalid..       
+000164a0: 2075 7064 6174 6564 5f63 6f6d 706f 6e65   updated_compone
+000164b0: 6e74 733a 2074 6865 2072 756e 6e69 6e67  nts: the running
+000164c0: 2064 6963 7469 6f6e 6172 7920 6f66 2063   dictionary of c
+000164d0: 6f6d 706f 6e65 6e74 7320 7768 6963 6820  omponents which 
+000164e0: 6861 7665 2062 6565 6e20 6d6f 6469 6669  have been modifi
+000164f0: 6564 2062 7920 7468 6973 2074 7261 6e73  ed by this trans
+00016500: 666f 726d 6174 696f 6e2e 2053 686f 756c  formation. Shoul
+00016510: 6420 616c 7761 7973 2062 6520 4e6f 6e65  d always be None
+00016520: 2c20 6578 6365 7074 2066 6f72 2072 6563  , except for rec
+00016530: 7572 7369 7665 2069 6e76 6f63 6174 696f  ursive invocatio
+00016540: 6e73 2e0a 2020 2020 2020 2020 7472 6176  ns..        trav
+00016550: 6572 7365 645f 636f 6d70 6f6e 656e 7473  ersed_components
+00016560: 3a20 7468 6520 7365 7420 6f66 2063 6f6d  : the set of com
+00016570: 706f 6e65 6e74 206e 616d 6573 2077 6869  ponent names whi
+00016580: 6368 2068 6176 6520 6265 656e 2074 7261  ch have been tra
+00016590: 7665 7273 6564 2e20 5368 6f75 6c64 2061  versed. Should a
+000165a0: 6c77 6179 7320 6265 204e 6f6e 652c 2065  lways be None, e
+000165b0: 7863 6570 7420 666f 7220 7265 6375 7273  xcept for recurs
+000165c0: 6976 6520 696e 766f 6361 7469 6f6e 732e  ive invocations.
+000165d0: 0a20 2020 2022 2222 0a20 2020 2066 726f  .    """.    fro
+000165e0: 6d20 6764 7366 6163 746f 7279 2e64 6563  m gdsfactory.dec
+000165f0: 6f72 6174 6f72 7320 696d 706f 7274 2069  orators import i
+00016600: 735f 696e 7661 6c69 645f 7265 660a 0a20  s_invalid_ref.. 
+00016610: 2020 2069 6e76 616c 6964 5f72 6566 7320     invalid_refs 
+00016620: 3d20 5b5d 0a20 2020 2072 6566 7320 3d20  = [].    refs = 
+00016630: 636f 6d70 6f6e 656e 742e 7265 6665 7265  component.refere
+00016640: 6e63 6573 0a20 2020 2073 7562 6365 6c6c  nces.    subcell
+00016650: 5f6d 6f64 6966 6965 6420 3d20 4661 6c73  _modified = Fals
+00016660: 650a 2020 2020 6966 2075 7064 6174 6564  e.    if updated
+00016670: 5f63 6f6d 706f 6e65 6e74 7320 6973 204e  _components is N
+00016680: 6f6e 653a 0a20 2020 2020 2020 2075 7064  one:.        upd
+00016690: 6174 6564 5f63 6f6d 706f 6e65 6e74 7320  ated_components 
+000166a0: 3d20 7b7d 0a20 2020 2069 6620 7472 6176  = {}.    if trav
+000166b0: 6572 7365 645f 636f 6d70 6f6e 656e 7473  ersed_components
+000166c0: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
+000166d0: 2020 7472 6176 6572 7365 645f 636f 6d70    traversed_comp
+000166e0: 6f6e 656e 7473 203d 2073 6574 2829 0a20  onents = set(). 
+000166f0: 2020 2066 6f72 2072 6566 2069 6e20 7265     for ref in re
+00016700: 6673 3a0a 2020 2020 2020 2020 2320 6d61  fs:.        # ma
+00016710: 726b 2061 6e79 2069 6e76 616c 6964 2072  rk any invalid r
+00016720: 6566 7320 666f 7220 666c 6174 7465 6e69  efs for flatteni
+00016730: 6e67 0a20 2020 2020 2020 2023 206f 7468  ng.        # oth
+00016740: 6572 7769 7365 2c20 6368 6563 6b20 6966  erwise, check if
+00016750: 2074 6865 7265 2061 7265 2061 6e79 206d   there are any m
+00016760: 6f64 6966 6965 6420 6365 6c6c 7320 6265  odified cells be
+00016770: 6e65 6174 6820 2877 6520 6e65 6564 206e  neath (we need n
+00016780: 6f74 2064 6f20 7468 6973 2069 6620 7468  ot do this if th
+00016790: 6520 7265 6620 7769 6c6c 2062 6520 666c  e ref will be fl
+000167a0: 6174 7465 6e65 6420 616e 7977 6179 7329  attened anyways)
+000167b0: 0a20 2020 2020 2020 2069 6620 6973 5f69  .        if is_i
+000167c0: 6e76 616c 6964 5f72 6566 2872 6566 2c20  nvalid_ref(ref, 
+000167d0: 6772 6964 5f73 697a 6529 3a0a 2020 2020  grid_size):.    
+000167e0: 2020 2020 2020 2020 696e 7661 6c69 645f          invalid_
+000167f0: 7265 6673 2e61 7070 656e 6428 7265 662e  refs.append(ref.
+00016800: 6e61 6d65 290a 2020 2020 2020 2020 656c  name).        el
+00016810: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+00016820: 2320 6f74 6865 7277 6973 652c 2072 6563  # otherwise, rec
+00016830: 7572 7369 7665 6c79 2066 6c61 7474 656e  ursively flatten
+00016840: 2072 6566 7320 6966 2074 6865 2073 7562   refs if the sub
+00016850: 6365 6c6c 2068 6173 206e 6f74 2061 6c72  cell has not alr
+00016860: 6561 6479 2062 6565 6e20 7472 6176 6572  eady been traver
+00016870: 7365 640a 2020 2020 2020 2020 2020 2020  sed.            
+00016880: 6966 2072 6566 2e70 6172 656e 742e 6e61  if ref.parent.na
+00016890: 6d65 206e 6f74 2069 6e20 7472 6176 6572  me not in traver
+000168a0: 7365 645f 636f 6d70 6f6e 656e 7473 3a0a  sed_components:.
+000168b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000168c0: 666c 6174 7465 6e5f 696e 7661 6c69 645f  flatten_invalid_
+000168d0: 7265 6673 5f72 6563 7572 7369 7665 280a  refs_recursive(.
+000168e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000168f0: 2020 2020 7265 662e 7061 7265 6e74 2c0a      ref.parent,.
+00016900: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016910: 2020 2020 6772 6964 5f73 697a 653d 6772      grid_size=gr
+00016920: 6964 5f73 697a 652c 0a20 2020 2020 2020  id_size,.       
+00016930: 2020 2020 2020 2020 2020 2020 2075 7064               upd
+00016940: 6174 6564 5f63 6f6d 706f 6e65 6e74 733d  ated_components=
+00016950: 7570 6461 7465 645f 636f 6d70 6f6e 656e  updated_componen
+00016960: 7473 2c0a 2020 2020 2020 2020 2020 2020  ts,.            
+00016970: 2020 2020 2020 2020 7472 6176 6572 7365          traverse
+00016980: 645f 636f 6d70 6f6e 656e 7473 3d74 7261  d_components=tra
+00016990: 7665 7273 6564 5f63 6f6d 706f 6e65 6e74  versed_component
+000169a0: 732c 0a20 2020 2020 2020 2020 2020 2020  s,.             
+000169b0: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
+000169c0: 2023 206e 6f77 2c20 6966 2074 6865 2072   # now, if the r
+000169d0: 6566 2773 2063 656c 6c20 6265 656e 206d  ef's cell been m
+000169e0: 6f64 6966 6965 642c 206d 6172 6b20 6974  odified, mark it
+000169f0: 2061 7320 7375 6368 0a20 2020 2020 2020   as such.       
+00016a00: 2020 2020 2069 6620 7265 662e 7061 7265       if ref.pare
+00016a10: 6e74 2e6e 616d 6520 696e 2075 7064 6174  nt.name in updat
+00016a20: 6564 5f63 6f6d 706f 6e65 6e74 733a 0a20  ed_components:. 
+00016a30: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00016a40: 7562 6365 6c6c 5f6d 6f64 6966 6965 6420  ubcell_modified 
+00016a50: 3d20 5472 7565 0a20 2020 2069 6620 696e  = True.    if in
+00016a60: 7661 6c69 645f 7265 6673 206f 7220 7375  valid_refs or su
+00016a70: 6263 656c 6c5f 6d6f 6469 6669 6564 3a0a  bcell_modified:.
+00016a80: 2020 2020 2020 2020 6e65 775f 636f 6d70          new_comp
+00016a90: 6f6e 656e 7420 3d20 636f 6d70 6f6e 656e  onent = componen
+00016aa0: 742e 636f 7079 2829 0a20 2020 2020 2020  t.copy().       
+00016ab0: 206e 6577 5f63 6f6d 706f 6e65 6e74 2e6e   new_component.n
+00016ac0: 616d 6520 3d20 636f 6d70 6f6e 656e 742e  ame = component.
+00016ad0: 6e61 6d65 0a20 2020 2020 2020 2023 206d  name.        # m
+00016ae0: 616b 6520 7375 7265 2061 6c6c 206d 6f64  ake sure all mod
+00016af0: 6966 6965 6420 6365 6c6c 7320 6861 7665  ified cells have
+00016b00: 2074 6865 6972 2072 6566 6572 656e 6365   their reference
+00016b10: 7320 7570 6461 7465 640a 2020 2020 2020  s updated.      
+00016b20: 2020 6e65 775f 7265 6673 203d 206e 6577    new_refs = new
+00016b30: 5f63 6f6d 706f 6e65 6e74 2e72 6566 6572  _component.refer
+00016b40: 656e 6365 732e 636f 7079 2829 0a20 2020  ences.copy().   
+00016b50: 2020 2020 2066 6f72 2072 6566 2069 6e20       for ref in 
+00016b60: 6e65 775f 7265 6673 3a0a 2020 2020 2020  new_refs:.      
+00016b70: 2020 2020 2020 6966 2072 6566 2e6e 616d        if ref.nam
+00016b80: 6520 696e 2069 6e76 616c 6964 5f72 6566  e in invalid_ref
+00016b90: 733a 0a20 2020 2020 2020 2020 2020 2020  s:.             
+00016ba0: 2020 206e 6577 5f63 6f6d 706f 6e65 6e74     new_component
+00016bb0: 2e66 6c61 7474 656e 5f72 6566 6572 656e  .flatten_referen
+00016bc0: 6365 2872 6566 290a 2020 2020 2020 2020  ce(ref).        
+00016bd0: 2020 2020 656c 6966 2028 0a20 2020 2020      elif (.     
+00016be0: 2020 2020 2020 2020 2020 2072 6566 2e70             ref.p
+00016bf0: 6172 656e 742e 6e61 6d65 2069 6e20 7570  arent.name in up
+00016c00: 6461 7465 645f 636f 6d70 6f6e 656e 7473  dated_components
+00016c10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00016c20: 2061 6e64 2072 6566 2e70 6172 656e 7420   and ref.parent 
+00016c30: 6973 206e 6f74 2075 7064 6174 6564 5f63  is not updated_c
+00016c40: 6f6d 706f 6e65 6e74 735b 7265 662e 7061  omponents[ref.pa
+00016c50: 7265 6e74 2e6e 616d 655d 0a20 2020 2020  rent.name].     
+00016c60: 2020 2020 2020 2029 3a0a 2020 2020 2020         ):.      
+00016c70: 2020 2020 2020 2020 2020 7265 662e 7061            ref.pa
+00016c80: 7265 6e74 203d 2075 7064 6174 6564 5f63  rent = updated_c
+00016c90: 6f6d 706f 6e65 6e74 735b 7265 662e 7061  omponents[ref.pa
+00016ca0: 7265 6e74 2e6e 616d 655d 0a20 2020 2020  rent.name].     
+00016cb0: 2020 2063 6f6d 706f 6e65 6e74 203d 206e     component = n
+00016cc0: 6577 5f63 6f6d 706f 6e65 6e74 0a20 2020  ew_component.   
+00016cd0: 2020 2020 2075 7064 6174 6564 5f63 6f6d       updated_com
+00016ce0: 706f 6e65 6e74 735b 636f 6d70 6f6e 656e  ponents[componen
+00016cf0: 742e 6e61 6d65 5d20 3d20 6e65 775f 636f  t.name] = new_co
+00016d00: 6d70 6f6e 656e 740a 2020 2020 7472 6176  mponent.    trav
+00016d10: 6572 7365 645f 636f 6d70 6f6e 656e 7473  ersed_components
+00016d20: 2e61 6464 2863 6f6d 706f 6e65 6e74 2e6e  .add(component.n
+00016d30: 616d 6529 0a20 2020 2072 6574 7572 6e20  ame).    return 
+00016d40: 636f 6d70 6f6e 656e 740a 0a0a 6465 6620  component...def 
+00016d50: 5f63 6865 636b 5f75 6e63 6163 6865 645f  _check_uncached_
+00016d60: 636f 6d70 6f6e 656e 7473 2863 6f6d 706f  components(compo
+00016d70: 6e65 6e74 2c20 6d6f 6465 293a 0a20 2020  nent, mode):.   
+00016d80: 2076 616c 6964 5f6d 6f64 6573 203d 205b   valid_modes = [
+00016d90: 2277 6172 6e22 2c20 2265 7272 6f72 222c  "warn", "error",
+00016da0: 2022 6967 6e6f 7265 225d 0a0a 2020 2020   "ignore"]..    
+00016db0: 6966 206d 6f64 6520 3d3d 2022 6967 6e6f  if mode == "igno
+00016dc0: 7265 223a 0a20 2020 2020 2020 2072 6574  re":.        ret
+00016dd0: 7572 6e0a 2020 2020 656c 6966 206d 6f64  urn.    elif mod
+00016de0: 6520 6e6f 7420 696e 2076 616c 6964 5f6d  e not in valid_m
+00016df0: 6f64 6573 3a0a 2020 2020 2020 2020 7261  odes:.        ra
+00016e00: 6973 6520 5661 6c75 6545 7272 6f72 280a  ise ValueError(.
+00016e10: 2020 2020 2020 2020 2020 2020 6622 7b6d              f"{m
+00016e20: 6f64 657d 2069 7320 6e6f 7420 6120 7661  ode} is not a va
+00016e30: 6c69 6420 7661 6c75 6520 666f 7220 6f6e  lid value for on
+00016e40: 5f75 6e63 6163 6865 645f 636f 6d70 6f6e  _uncached_compon
+00016e50: 656e 742e 2054 7279 206f 6e65 206f 6620  ent. Try one of 
+00016e60: 7468 6573 653a 207b 7661 6c69 645f 6d6f  these: {valid_mo
+00016e70: 6465 737d 2e22 0a20 2020 2020 2020 2029  des}.".        )
+00016e80: 0a0a 2020 2020 666f 7220 7375 625f 636f  ..    for sub_co
+00016e90: 6d70 6f6e 656e 7420 696e 2063 6f6d 706f  mponent in compo
+00016ea0: 6e65 6e74 2e67 6574 5f64 6570 656e 6465  nent.get_depende
+00016eb0: 6e63 6965 7328 7265 6375 7273 6976 653d  ncies(recursive=
+00016ec0: 5472 7565 293a 0a20 2020 2020 2020 2069  True):.        i
+00016ed0: 6620 6e6f 7420 7375 625f 636f 6d70 6f6e  f not sub_compon
+00016ee0: 656e 742e 5f6c 6f63 6b65 643a 0a20 2020  ent._locked:.   
+00016ef0: 2020 2020 2020 2020 206d 6573 7361 6765           message
+00016f00: 203d 2028 0a20 2020 2020 2020 2020 2020   = (.           
+00016f10: 2020 2020 2066 2243 6f6d 706f 6e65 6e74       f"Component
+00016f20: 207b 7375 625f 636f 6d70 6f6e 656e 742e   {sub_component.
+00016f30: 6e61 6d65 2172 7d20 7761 7320 4e4f 5420  name!r} was NOT 
+00016f40: 7072 6f70 6572 6c79 206c 6f63 6b65 642e  properly locked.
+00016f50: 2022 0a20 2020 2020 2020 2020 2020 2020   ".             
+00016f60: 2020 2022 596f 7520 6e65 6564 2074 6f20     "You need to 
+00016f70: 7772 6974 6520 6974 2069 6e74 6f20 6120  write it into a 
+00016f80: 6675 6e63 7469 6f6e 2074 6861 7420 6861  function that ha
+00016f90: 7320 7468 6520 4063 656c 6c20 6465 636f  s the @cell deco
+00016fa0: 7261 746f 722e 220a 2020 2020 2020 2020  rator.".        
+00016fb0: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
+00016fc0: 2020 6966 206d 6f64 6520 3d3d 2022 7761    if mode == "wa
+00016fd0: 726e 223a 0a20 2020 2020 2020 2020 2020  rn":.           
+00016fe0: 2020 2020 2077 6172 6e69 6e67 732e 7761       warnings.wa
+00016ff0: 726e 286d 6573 7361 6765 2c20 556e 6361  rn(message, Unca
+00017000: 6368 6564 436f 6d70 6f6e 656e 7457 6172  chedComponentWar
+00017010: 6e69 6e67 290a 0a20 2020 2020 2020 2020  ning)..         
+00017020: 2020 2065 6c69 6620 6d6f 6465 203d 3d20     elif mode == 
+00017030: 2265 7272 6f72 223a 0a20 2020 2020 2020  "error":.       
+00017040: 2020 2020 2020 2020 2072 6169 7365 2055           raise U
+00017050: 6e63 6163 6865 6443 6f6d 706f 6e65 6e74  ncachedComponent
+00017060: 4572 726f 7228 6d65 7373 6167 6529 0a0a  Error(message)..
+00017070: 0a64 6566 2074 6573 745f 7361 6d65 5f75  .def test_same_u
+00017080: 6964 2829 202d 3e20 4e6f 6e65 3a0a 2020  id() -> None:.  
+00017090: 2020 696d 706f 7274 2067 6473 6661 6374    import gdsfact
+000170a0: 6f72 7920 6173 2067 660a 0a20 2020 2063  ory as gf..    c
+000170b0: 203d 2043 6f6d 706f 6e65 6e74 2829 0a20   = Component(). 
+000170c0: 2020 2063 203c 3c20 6766 2e63 6f6d 706f     c << gf.compo
+000170d0: 6e65 6e74 732e 7265 6374 616e 676c 6528  nents.rectangle(
+000170e0: 290a 2020 2020 6320 3c3c 2067 662e 636f  ).    c << gf.co
+000170f0: 6d70 6f6e 656e 7473 2e72 6563 7461 6e67  mponents.rectang
+00017100: 6c65 2829 0a0a 2020 2020 7231 203d 2063  le()..    r1 = c
+00017110: 2e72 6566 6572 656e 6365 735b 305d 2e70  .references[0].p
+00017120: 6172 656e 740a 2020 2020 7232 203d 2063  arent.    r2 = c
+00017130: 2e72 6566 6572 656e 6365 735b 315d 2e70  .references[1].p
+00017140: 6172 656e 740a 0a20 2020 2061 7373 6572  arent..    asser
+00017150: 7420 7231 2e75 6964 203d 3d20 7232 2e75  t r1.uid == r2.u
+00017160: 6964 2c20 6622 7b72 312e 7569 647d 206d  id, f"{r1.uid} m
+00017170: 7573 7420 6571 7561 6c20 7b72 322e 7569  ust equal {r2.ui
+00017180: 647d 220a 0a0a 6465 6620 7465 7374 5f6e  d}"...def test_n
+00017190: 6574 6c69 7374 5f73 696d 706c 6528 2920  etlist_simple() 
+000171a0: 2d3e 204e 6f6e 653a 0a20 2020 2069 6d70  -> None:.    imp
+000171b0: 6f72 7420 6764 7366 6163 746f 7279 2061  ort gdsfactory a
+000171c0: 7320 6766 0a0a 2020 2020 6320 3d20 6766  s gf..    c = gf
+000171d0: 2e43 6f6d 706f 6e65 6e74 2829 0a20 2020  .Component().   
+000171e0: 2063 3120 3d20 6320 3c3c 2067 662e 636f   c1 = c << gf.co
+000171f0: 6d70 6f6e 656e 7473 2e73 7472 6169 6768  mponents.straigh
+00017200: 7428 6c65 6e67 7468 3d31 2c20 7769 6474  t(length=1, widt
+00017210: 683d 3229 0a20 2020 2063 3220 3d20 6320  h=2).    c2 = c 
+00017220: 3c3c 2067 662e 636f 6d70 6f6e 656e 7473  << gf.components
+00017230: 2e73 7472 6169 6768 7428 6c65 6e67 7468  .straight(length
+00017240: 3d32 2c20 7769 6474 683d 3229 0a20 2020  =2, width=2).   
+00017250: 2063 322e 636f 6e6e 6563 7428 706f 7274   c2.connect(port
+00017260: 3d22 6f31 222c 2064 6573 7469 6e61 7469  ="o1", destinati
+00017270: 6f6e 3d63 312e 706f 7274 735b 226f 3222  on=c1.ports["o2"
+00017280: 5d29 0a20 2020 2063 2e61 6464 5f70 6f72  ]).    c.add_por
+00017290: 7428 226f 3122 2c20 706f 7274 3d63 312e  t("o1", port=c1.
+000172a0: 706f 7274 735b 226f 3122 5d29 0a20 2020  ports["o1"]).   
+000172b0: 2063 2e61 6464 5f70 6f72 7428 226f 3222   c.add_port("o2"
+000172c0: 2c20 706f 7274 3d63 322e 706f 7274 735b  , port=c2.ports[
+000172d0: 226f 3222 5d29 0a20 2020 206e 6574 6c69  "o2"]).    netli
+000172e0: 7374 203d 2063 2e67 6574 5f6e 6574 6c69  st = c.get_netli
+000172f0: 7374 2829 0a20 2020 2023 2070 7269 6e74  st().    # print
+00017300: 286e 6574 6c69 7374 2e70 7265 7474 7928  (netlist.pretty(
+00017310: 2929 0a20 2020 2061 7373 6572 7420 6c65  )).    assert le
+00017320: 6e28 6e65 746c 6973 745b 2269 6e73 7461  n(netlist["insta
+00017330: 6e63 6573 225d 2920 3d3d 2032 0a0a 0a64  nces"]) == 2...d
+00017340: 6566 2074 6573 745f 6e65 746c 6973 745f  ef test_netlist_
+00017350: 7369 6d70 6c65 5f77 6964 7468 5f6d 6973  simple_width_mis
+00017360: 6d61 7463 685f 7468 726f 7773 5f65 7272  match_throws_err
+00017370: 6f72 2829 202d 3e20 4e6f 6e65 3a0a 2020  or() -> None:.  
+00017380: 2020 696d 706f 7274 2070 7974 6573 740a    import pytest.
+00017390: 0a20 2020 2069 6d70 6f72 7420 6764 7366  .    import gdsf
+000173a0: 6163 746f 7279 2061 7320 6766 0a0a 2020  actory as gf..  
+000173b0: 2020 6320 3d20 6766 2e43 6f6d 706f 6e65    c = gf.Compone
+000173c0: 6e74 2829 0a20 2020 2063 3120 3d20 6320  nt().    c1 = c 
+000173d0: 3c3c 2067 662e 636f 6d70 6f6e 656e 7473  << gf.components
+000173e0: 2e73 7472 6169 6768 7428 6c65 6e67 7468  .straight(length
+000173f0: 3d31 2c20 7769 6474 683d 3129 0a20 2020  =1, width=1).   
+00017400: 2063 3220 3d20 6320 3c3c 2067 662e 636f   c2 = c << gf.co
+00017410: 6d70 6f6e 656e 7473 2e73 7472 6169 6768  mponents.straigh
+00017420: 7428 6c65 6e67 7468 3d32 2c20 7769 6474  t(length=2, widt
+00017430: 683d 3229 0a20 2020 2063 322e 636f 6e6e  h=2).    c2.conn
+00017440: 6563 7428 706f 7274 3d22 6f31 222c 2064  ect(port="o1", d
+00017450: 6573 7469 6e61 7469 6f6e 3d63 312e 706f  estination=c1.po
+00017460: 7274 735b 226f 3222 5d29 0a20 2020 2063  rts["o2"]).    c
+00017470: 2e61 6464 5f70 6f72 7428 226f 3122 2c20  .add_port("o1", 
+00017480: 706f 7274 3d63 312e 706f 7274 735b 226f  port=c1.ports["o
+00017490: 3122 5d29 0a20 2020 2063 2e61 6464 5f70  1"]).    c.add_p
+000174a0: 6f72 7428 226f 3222 2c20 706f 7274 3d63  ort("o2", port=c
+000174b0: 322e 706f 7274 735b 226f 3222 5d29 0a20  2.ports["o2"]). 
+000174c0: 2020 2077 6974 6820 7079 7465 7374 2e72     with pytest.r
+000174d0: 6169 7365 7328 5661 6c75 6545 7272 6f72  aises(ValueError
+000174e0: 293a 0a20 2020 2020 2020 2063 2e67 6574  ):.        c.get
+000174f0: 5f6e 6574 6c69 7374 2829 0a0a 0a64 6566  _netlist()...def
+00017500: 2074 6573 745f 6e65 746c 6973 745f 636f   test_netlist_co
+00017510: 6d70 6c65 7828 2920 2d3e 204e 6f6e 653a  mplex() -> None:
+00017520: 0a20 2020 2069 6d70 6f72 7420 6764 7366  .    import gdsf
+00017530: 6163 746f 7279 2061 7320 6766 0a0a 2020  actory as gf..  
+00017540: 2020 6320 3d20 6766 2e63 6f6d 706f 6e65    c = gf.compone
+00017550: 6e74 732e 6d7a 695f 6172 6d73 2829 0a20  nts.mzi_arms(). 
+00017560: 2020 206e 6574 6c69 7374 203d 2063 2e67     netlist = c.g
+00017570: 6574 5f6e 6574 6c69 7374 2829 0a20 2020  et_netlist().   
+00017580: 2023 2070 7269 6e74 286e 6574 6c69 7374   # print(netlist
+00017590: 2e70 7265 7474 7928 2929 0a20 2020 2061  .pretty()).    a
+000175a0: 7373 6572 7420 6c65 6e28 6e65 746c 6973  ssert len(netlis
+000175b0: 745b 2269 6e73 7461 6e63 6573 225d 2920  t["instances"]) 
+000175c0: 3d3d 2034 2c20 6c65 6e28 6e65 746c 6973  == 4, len(netlis
+000175d0: 745b 2269 6e73 7461 6e63 6573 225d 290a  t["instances"]).
+000175e0: 0a0a 6465 6620 7465 7374 5f65 7874 7261  ..def test_extra
+000175f0: 6374 2829 202d 3e20 436f 6d70 6f6e 656e  ct() -> Componen
+00017600: 743a 0a20 2020 2069 6d70 6f72 7420 6764  t:.    import gd
+00017610: 7366 6163 746f 7279 2061 7320 6766 0a0a  sfactory as gf..
+00017620: 2020 2020 6320 3d20 6766 2e63 6f6d 706f      c = gf.compo
+00017630: 6e65 6e74 732e 7374 7261 6967 6874 280a  nents.straight(.
+00017640: 2020 2020 2020 2020 6c65 6e67 7468 3d31          length=1
+00017650: 302c 0a20 2020 2020 2020 2077 6964 7468  0,.        width
+00017660: 3d30 2e35 2c0a 2020 2020 2020 2020 6262  =0.5,.        bb
+00017670: 6f78 5f6c 6179 6572 733d 5b67 662e 4c41  ox_layers=[gf.LA
+00017680: 5945 522e 5747 434c 4144 5d2c 0a20 2020  YER.WGCLAD],.   
+00017690: 2020 2020 2062 626f 785f 6f66 6673 6574       bbox_offset
+000176a0: 733d 5b33 5d2c 0a20 2020 2020 2020 2077  s=[3],.        w
+000176b0: 6974 685f 6262 6f78 3d54 7275 652c 0a20  ith_bbox=True,. 
+000176c0: 2020 2020 2020 2063 6c61 6464 696e 675f         cladding_
+000176d0: 6c61 7965 7273 3d4e 6f6e 652c 0a20 2020  layers=None,.   
+000176e0: 2020 2020 2061 6464 5f70 696e 733d 4e6f       add_pins=No
+000176f0: 6e65 2c0a 2020 2020 2020 2020 6164 645f  ne,.        add_
+00017700: 6262 6f78 3d4e 6f6e 652c 0a20 2020 2029  bbox=None,.    )
+00017710: 0a20 2020 2063 3220 3d20 632e 6578 7472  .    c2 = c.extr
+00017720: 6163 7428 6c61 7965 7273 3d5b 6766 2e4c  act(layers=[gf.L
+00017730: 4159 4552 2e57 4743 4c41 445d 290a 0a20  AYER.WGCLAD]).. 
+00017740: 2020 2061 7373 6572 7420 6c65 6e28 632e     assert len(c.
+00017750: 706f 6c79 676f 6e73 2920 3d3d 2032 2c20  polygons) == 2, 
+00017760: 6c65 6e28 632e 706f 6c79 676f 6e73 290a  len(c.polygons).
+00017770: 2020 2020 6173 7365 7274 206c 656e 2863      assert len(c
+00017780: 322e 706f 6c79 676f 6e73 2920 3d3d 2031  2.polygons) == 1
+00017790: 2c20 6c65 6e28 6332 2e70 6f6c 7967 6f6e  , len(c2.polygon
+000177a0: 7329 0a20 2020 2061 7373 6572 7420 6766  s).    assert gf
+000177b0: 2e4c 4159 4552 2e57 4743 4c41 4420 696e  .LAYER.WGCLAD in
+000177c0: 2063 322e 6c61 7965 7273 0a20 2020 2072   c2.layers.    r
+000177d0: 6574 7572 6e20 6332 0a0a 0a64 6566 2068  eturn c2...def h
+000177e0: 6173 685f 6669 6c65 2866 696c 6570 6174  ash_file(filepat
+000177f0: 6829 3a0a 2020 2020 6d64 3520 3d20 6861  h):.    md5 = ha
+00017800: 7368 6c69 622e 6d64 3528 290a 2020 2020  shlib.md5().    
+00017810: 6d64 352e 7570 6461 7465 2866 696c 6570  md5.update(filep
+00017820: 6174 682e 7265 6164 5f62 7974 6573 2829  ath.read_bytes()
+00017830: 290a 2020 2020 7265 7475 726e 206d 6435  ).    return md5
+00017840: 2e68 6578 6469 6765 7374 2829 0a0a 0a64  .hexdigest()...d
+00017850: 6566 2074 6573 745f 6262 6f78 5f72 6566  ef test_bbox_ref
+00017860: 6572 656e 6365 2829 202d 3e20 436f 6d70  erence() -> Comp
+00017870: 6f6e 656e 743a 0a20 2020 2069 6d70 6f72  onent:.    impor
+00017880: 7420 6764 7366 6163 746f 7279 2061 7320  t gdsfactory as 
+00017890: 6766 0a0a 2020 2020 6320 3d20 6766 2e43  gf..    c = gf.C
+000178a0: 6f6d 706f 6e65 6e74 2822 636f 6d70 6f6e  omponent("compon
+000178b0: 656e 745f 7769 7468 5f6f 6666 6772 6964  ent_with_offgrid
+000178c0: 5f70 6f6c 7967 6f6e 7322 290a 2020 2020  _polygons").    
+000178d0: 6331 203d 2063 203c 3c20 6766 2e63 6f6d  c1 = c << gf.com
+000178e0: 706f 6e65 6e74 732e 7265 6374 616e 676c  ponents.rectangl
+000178f0: 6528 7369 7a65 3d28 312e 3565 2d33 2c20  e(size=(1.5e-3, 
+00017900: 312e 3565 2d33 292c 2070 6f72 745f 7479  1.5e-3), port_ty
+00017910: 7065 3d4e 6f6e 6529 0a20 2020 2063 3220  pe=None).    c2 
+00017920: 3d20 6320 3c3c 2067 662e 636f 6d70 6f6e  = c << gf.compon
+00017930: 656e 7473 2e72 6563 7461 6e67 6c65 2873  ents.rectangle(s
+00017940: 697a 653d 2831 2e35 652d 332c 2031 2e35  ize=(1.5e-3, 1.5
+00017950: 652d 3329 2c20 706f 7274 5f74 7970 653d  e-3), port_type=
+00017960: 4e6f 6e65 290a 2020 2020 6332 2e78 6d69  None).    c2.xmi
+00017970: 6e20 3d20 6331 2e78 6d61 780a 0a20 2020  n = c1.xmax..   
+00017980: 2061 7373 6572 7420 6332 2e78 7369 7a65   assert c2.xsize
+00017990: 203d 3d20 3265 2d33 0a20 2020 2072 6574   == 2e-3.    ret
+000179a0: 7572 6e20 6332 0a0a 0a64 6566 2074 6573  urn c2...def tes
+000179b0: 745f 6262 6f78 5f63 6f6d 706f 6e65 6e74  t_bbox_component
 000179c0: 2829 202d 3e20 4e6f 6e65 3a0a 2020 2020  () -> None:.    
 000179d0: 696d 706f 7274 2067 6473 6661 6374 6f72  import gdsfactor
 000179e0: 7920 6173 2067 660a 0a20 2020 2063 203d  y as gf..    c =
-000179f0: 2067 662e 636f 6d70 6f6e 656e 7473 2e73   gf.components.s
-00017a00: 7472 6169 6768 7428 6c61 7965 723d 2832  traight(layer=(2
-00017a10: 2c20 3029 290a 2020 2020 7265 6d61 7020  , 0)).    remap 
-00017a20: 3d20 632e 7265 6d61 705f 6c61 7965 7273  = c.remap_layers
-00017a30: 286c 6179 6572 6d61 703d 7b28 322c 2030  (layermap={(2, 0
-00017a40: 293a 2067 662e 4c41 5945 522e 5747 4e7d  ): gf.LAYER.WGN}
-00017a50: 290a 2020 2020 6861 7368 5f67 656f 6d65  ).    hash_geome
-00017a60: 7472 7920 3d20 2238 3366 6263 3661 3832  try = "83fbc6a82
-00017a70: 3839 3530 3565 6165 6433 6132 6533 6162  89505eaed3a2e3ab
-00017a80: 3237 3963 6330 3366 3565 3464 3030 6322  279cc03f5e4d00c"
-00017a90: 0a0a 2020 2020 6173 7365 7274 2028 0a20  ..    assert (. 
-00017aa0: 2020 2020 2020 2072 656d 6170 2e68 6173         remap.has
-00017ab0: 685f 6765 6f6d 6574 7279 2829 203d 3d20  h_geometry() == 
-00017ac0: 6861 7368 5f67 656f 6d65 7472 790a 2020  hash_geometry.  
-00017ad0: 2020 292c 2066 2268 6173 685f 6765 6f6d    ), f"hash_geom
-00017ae0: 6574 7279 203d 207b 7265 6d61 702e 6861  etry = {remap.ha
-00017af0: 7368 5f67 656f 6d65 7472 7928 2921 727d  sh_geometry()!r}
-00017b00: 220a 0a0a 6465 6620 7465 7374 5f72 656d  "...def test_rem
-00017b10: 6f76 655f 6c61 6265 6c73 2829 202d 3e20  ove_labels() -> 
-00017b20: 4e6f 6e65 3a0a 2020 2020 696d 706f 7274  None:.    import
-00017b30: 2067 6473 6661 6374 6f72 7920 6173 2067   gdsfactory as g
-00017b40: 660a 0a20 2020 2063 203d 2067 662e 632e  f..    c = gf.c.
-00017b50: 7374 7261 6967 6874 2829 0a20 2020 2063  straight().    c
-00017b60: 2e72 656d 6f76 655f 6c61 6265 6c73 2829  .remove_labels()
-00017b70: 0a0a 2020 2020 6173 7365 7274 206c 656e  ..    assert len
-00017b80: 2863 2e6c 6162 656c 7329 203d 3d20 300a  (c.labels) == 0.
-00017b90: 0a0a 6465 6620 7465 7374 5f69 6d70 6f72  ..def test_impor
-00017ba0: 745f 6764 735f 7365 7474 696e 6773 2829  t_gds_settings()
-00017bb0: 3a0a 2020 2020 696d 706f 7274 2067 6473  :.    import gds
-00017bc0: 6661 6374 6f72 7920 6173 2067 660a 0a20  factory as gf.. 
-00017bd0: 2020 2063 203d 2067 662e 636f 6d70 6f6e     c = gf.compon
-00017be0: 656e 7473 2e6d 7a69 2829 0a20 2020 2067  ents.mzi().    g
-00017bf0: 6473 7061 7468 203d 2063 2e77 7269 7465  dspath = c.write
-00017c00: 5f67 6473 5f77 6974 685f 6d65 7461 6461  _gds_with_metada
-00017c10: 7461 2829 0a20 2020 2063 3220 3d20 6766  ta().    c2 = gf
-00017c20: 2e69 6d70 6f72 745f 6764 7328 6764 7370  .import_gds(gdsp
-00017c30: 6174 682c 206e 616d 653d 226d 7a69 5f73  ath, name="mzi_s
-00017c40: 616d 706c 6522 2c20 7265 6164 5f6d 6574  ample", read_met
-00017c50: 6164 6174 613d 5472 7565 290a 2020 2020  adata=True).    
-00017c60: 6333 203d 2067 662e 726f 7574 696e 672e  c3 = gf.routing.
-00017c70: 6164 645f 6669 6265 725f 7369 6e67 6c65  add_fiber_single
-00017c80: 2863 3229 0a20 2020 2061 7373 6572 7420  (c2).    assert 
-00017c90: 6333 0a0a 0a64 6566 2074 6573 745f 666c  c3...def test_fl
-00017ca0: 6174 7465 6e5f 696e 7661 6c69 645f 7265  atten_invalid_re
-00017cb0: 6673 5f72 6563 7572 7369 7665 2829 3a0a  fs_recursive():.
-00017cc0: 2020 2020 696d 706f 7274 2067 6473 6661      import gdsfa
-00017cd0: 6374 6f72 7920 6173 2067 660a 2020 2020  ctory as gf.    
-00017ce0: 6672 6f6d 2067 6473 6661 6374 6f72 792e  from gdsfactory.
-00017cf0: 6469 6666 7465 7374 2069 6d70 6f72 7420  difftest import 
-00017d00: 7275 6e5f 786f 720a 2020 2020 6672 6f6d  run_xor.    from
-00017d10: 2067 6473 6661 6374 6f72 792e 726f 7574   gdsfactory.rout
-00017d20: 696e 672e 616c 6c5f 616e 676c 6520 696d  ing.all_angle im
-00017d30: 706f 7274 2067 6574 5f62 756e 646c 655f  port get_bundle_
-00017d40: 616c 6c5f 616e 676c 650a 0a20 2020 2040  all_angle..    @
-00017d50: 6766 2e63 656c 6c0a 2020 2020 6465 6620  gf.cell.    def 
-00017d60: 666c 6174 2829 3a0a 2020 2020 2020 2020  flat():.        
-00017d70: 6320 3d20 6766 2e43 6f6d 706f 6e65 6e74  c = gf.Component
-00017d80: 2829 0a20 2020 2020 2020 206d 6d69 3120  ().        mmi1 
-00017d90: 3d20 2863 203c 3c20 6766 2e63 6f6d 706f  = (c << gf.compo
-00017da0: 6e65 6e74 732e 6d6d 6931 7832 2829 292e  nents.mmi1x2()).
-00017db0: 6d6f 7665 2828 302c 202d 312e 3030 3035  move((0, -1.0005
-00017dc0: 2929 0a20 2020 2020 2020 206d 6d69 3220  )).        mmi2 
-00017dd0: 3d20 2863 203c 3c20 6766 2e63 6f6d 706f  = (c << gf.compo
-00017de0: 6e65 6e74 732e 6d6d 6931 7832 2829 292e  nents.mmi1x2()).
-00017df0: 726f 7461 7465 2838 3029 0a20 2020 2020  rotate(80).     
-00017e00: 2020 206d 6d69 322e 6d6f 7665 2828 3430     mmi2.move((40
-00017e10: 2c20 3230 2929 0a20 2020 2020 2020 2062  , 20)).        b
-00017e20: 756e 646c 6520 3d20 6765 745f 6275 6e64  undle = get_bund
-00017e30: 6c65 5f61 6c6c 5f61 6e67 6c65 285b 6d6d  le_all_angle([mm
-00017e40: 6931 2e70 6f72 7473 5b22 6f32 225d 5d2c  i1.ports["o2"]],
-00017e50: 205b 6d6d 6932 2e70 6f72 7473 5b22 6f31   [mmi2.ports["o1
-00017e60: 225d 5d29 0a20 2020 2020 2020 2066 6f72  "]]).        for
-00017e70: 2072 6f75 7465 2069 6e20 6275 6e64 6c65   route in bundle
-00017e80: 3a0a 2020 2020 2020 2020 2020 2020 632e  :.            c.
-00017e90: 6164 6428 726f 7574 652e 7265 6665 7265  add(route.refere
-00017ea0: 6e63 6573 290a 2020 2020 2020 2020 7265  nces).        re
-00017eb0: 7475 726e 2063 0a0a 2020 2020 4067 662e  turn c..    @gf.
-00017ec0: 6365 6c6c 0a20 2020 2064 6566 2068 6965  cell.    def hie
-00017ed0: 7261 7263 6879 2829 3a0a 2020 2020 2020  rarchy():.      
-00017ee0: 2020 6320 3d20 6766 2e43 6f6d 706f 6e65    c = gf.Compone
-00017ef0: 6e74 2829 0a20 2020 2020 2020 2028 6320  nt().        (c 
-00017f00: 3c3c 2066 6c61 7428 2929 2e72 6f74 6174  << flat()).rotat
-00017f10: 6528 3333 290a 2020 2020 2020 2020 2863  e(33).        (c
-00017f20: 203c 3c20 666c 6174 2829 292e 726f 7461   << flat()).rota
-00017f30: 7465 2833 3329 2e6d 6f76 6528 2830 2c20  te(33).move((0, 
-00017f40: 3130 3029 290a 2020 2020 2020 2020 2863  100)).        (c
-00017f50: 203c 3c20 666c 6174 2829 292e 6d6f 7665   << flat()).move
-00017f60: 2828 3130 302c 2030 2929 0a20 2020 2020  ((100, 0)).     
-00017f70: 2020 2072 6574 7572 6e20 630a 0a20 2020     return c..   
-00017f80: 2063 5f6f 7269 6720 3d20 6869 6572 6172   c_orig = hierar
-00017f90: 6368 7928 290a 2020 2020 635f 6e65 7720  chy().    c_new 
-00017fa0: 3d20 666c 6174 7465 6e5f 696e 7661 6c69  = flatten_invali
-00017fb0: 645f 7265 6673 5f72 6563 7572 7369 7665  d_refs_recursive
-00017fc0: 2863 5f6f 7269 6729 0a20 2020 2061 7373  (c_orig).    ass
-00017fd0: 6572 7420 635f 6e65 7720 6973 206e 6f74  ert c_new is not
-00017fe0: 2063 5f6f 7269 670a 2020 2020 696e 7661   c_orig.    inva
-00017ff0: 6c69 645f 7265 6673 5f66 696c 656e 616d  lid_refs_filenam
-00018000: 6520 3d20 2269 6e76 616c 6964 5f72 6566  e = "invalid_ref
-00018010: 732e 6764 7322 0a20 2020 2069 6e76 616c  s.gds".    inval
-00018020: 6964 5f72 6566 735f 6669 7865 645f 6669  id_refs_fixed_fi
-00018030: 6c65 6e61 6d65 203d 2022 696e 7661 6c69  lename = "invali
-00018040: 645f 7265 6673 5f66 6978 6564 2e67 6473  d_refs_fixed.gds
-00018050: 220a 2020 2020 2320 6764 7320 6669 6c65  ".    # gds file
-00018060: 7320 7368 6f75 6c64 2073 7469 6c6c 2062  s should still b
-00018070: 6520 7361 6d65 2074 6f20 316e 6d20 746f  e same to 1nm to
-00018080: 6c65 7261 6e63 650a 2020 2020 635f 6f72  lerance.    c_or
-00018090: 6967 2e77 7269 7465 5f67 6473 2869 6e76  ig.write_gds(inv
-000180a0: 616c 6964 5f72 6566 735f 6669 6c65 6e61  alid_refs_filena
-000180b0: 6d65 290a 2020 2020 635f 6e65 772e 7772  me).    c_new.wr
-000180c0: 6974 655f 6764 7328 696e 7661 6c69 645f  ite_gds(invalid_
-000180d0: 7265 6673 5f66 6978 6564 5f66 696c 656e  refs_fixed_filen
-000180e0: 616d 6529 0a20 2020 2072 756e 5f78 6f72  ame).    run_xor
-000180f0: 2869 6e76 616c 6964 5f72 6566 735f 6669  (invalid_refs_fi
-00018100: 6c65 6e61 6d65 2c20 696e 7661 6c69 645f  lename, invalid_
-00018110: 7265 6673 5f66 6978 6564 5f66 696c 656e  refs_fixed_filen
-00018120: 616d 6529 0a0a 0a69 6620 5f5f 6e61 6d65  ame)...if __name
-00018130: 5f5f 203d 3d20 225f 5f6d 6169 6e5f 5f22  __ == "__main__"
-00018140: 3a0a 2020 2020 696d 706f 7274 2067 6473  :.    import gds
-00018150: 6661 6374 6f72 7920 6173 2067 660a 0a20  factory as gf.. 
-00018160: 2020 2023 2063 3220 3d20 6766 2e43 6f6d     # c2 = gf.Com
-00018170: 706f 6e65 6e74 2829 0a20 2020 2063 203d  ponent().    c =
-00018180: 2067 662e 636f 6d70 6f6e 656e 7473 2e6d   gf.components.m
-00018190: 7a69 2829 0a20 2020 2070 7269 6e74 2863  zi().    print(c
-000181a0: 2e67 6574 5f6c 6179 6572 5f6e 616d 6573  .get_layer_names
-000181b0: 2829 290a 2020 2020 2320 7220 3d20 632e  ()).    # r = c.
-000181c0: 7265 6628 290a 2020 2020 2320 6332 2e63  ref().    # c2.c
-000181d0: 6f70 795f 6368 696c 645f 696e 666f 2863  opy_child_info(c
-000181e0: 2e6e 616d 6564 5f72 6566 6572 656e 6365  .named_reference
-000181f0: 735b 2273 7874 225d 290a 2020 2020 2320  s["sxt"]).    # 
-00018200: 7465 7374 5f72 656d 6170 5f6c 6179 6572  test_remap_layer
-00018210: 7328 290a 2020 2020 2320 6320 3d20 7465  s().    # c = te
-00018220: 7374 5f67 6574 5f6c 6179 6572 7328 290a  st_get_layers().
-00018230: 2020 2020 2320 632e 706c 6f74 5f71 7428      # c.plot_qt(
-00018240: 290a 2020 2020 2320 632e 706c 6f74 6828  ).    # c.ploth(
-00018250: 290a 2020 2020 2320 6320 3d20 7465 7374  ).    # c = test
-00018260: 5f65 7874 7261 6374 2829 0a20 2020 2023  _extract().    #
-00018270: 2067 6473 7061 7468 203d 2063 2e77 7269   gdspath = c.wri
-00018280: 7465 5f67 6473 2829 0a20 2020 2023 2067  te_gds().    # g
-00018290: 662e 7368 6f77 2867 6473 7061 7468 290a  f.show(gdspath).
-000182a0: 2020 2020 2320 632e 7368 6f77 2873 686f      # c.show(sho
-000182b0: 775f 706f 7274 733d 5472 7565 290a 2020  w_ports=True).  
-000182c0: 2020 632e 7368 6f77 2829 0a                c.show().
+000179f0: 2067 662e 636f 6d70 6f6e 656e 7473 2e72   gf.components.r
+00017a00: 6563 7461 6e67 6c65 2873 697a 653d 2831  ectangle(size=(1
+00017a10: 2e35 652d 332c 2031 2e35 652d 3329 2c20  .5e-3, 1.5e-3), 
+00017a20: 706f 7274 5f74 7970 653d 4e6f 6e65 290a  port_type=None).
+00017a30: 2020 2020 6173 7365 7274 2063 2e78 7369      assert c.xsi
+00017a40: 7a65 203d 3d20 3265 2d33 0a0a 0a64 6566  ze == 2e-3...def
+00017a50: 2074 6573 745f 7265 6d61 705f 6c61 7965   test_remap_laye
+00017a60: 7273 2829 202d 3e20 4e6f 6e65 3a0a 2020  rs() -> None:.  
+00017a70: 2020 696d 706f 7274 2067 6473 6661 6374    import gdsfact
+00017a80: 6f72 7920 6173 2067 660a 0a20 2020 2063  ory as gf..    c
+00017a90: 203d 2067 662e 636f 6d70 6f6e 656e 7473   = gf.components
+00017aa0: 2e73 7472 6169 6768 7428 6c61 7965 723d  .straight(layer=
+00017ab0: 2832 2c20 3029 290a 2020 2020 7265 6d61  (2, 0)).    rema
+00017ac0: 7020 3d20 632e 7265 6d61 705f 6c61 7965  p = c.remap_laye
+00017ad0: 7273 286c 6179 6572 6d61 703d 7b28 322c  rs(layermap={(2,
+00017ae0: 2030 293a 2067 662e 4c41 5945 522e 5747   0): gf.LAYER.WG
+00017af0: 4e7d 290a 2020 2020 6861 7368 5f67 656f  N}).    hash_geo
+00017b00: 6d65 7472 7920 3d20 2238 3366 6263 3661  metry = "83fbc6a
+00017b10: 3832 3839 3530 3565 6165 6433 6132 6533  8289505eaed3a2e3
+00017b20: 6162 3237 3963 6330 3366 3565 3464 3030  ab279cc03f5e4d00
+00017b30: 6322 0a0a 2020 2020 6173 7365 7274 2028  c"..    assert (
+00017b40: 0a20 2020 2020 2020 2072 656d 6170 2e68  .        remap.h
+00017b50: 6173 685f 6765 6f6d 6574 7279 2829 203d  ash_geometry() =
+00017b60: 3d20 6861 7368 5f67 656f 6d65 7472 790a  = hash_geometry.
+00017b70: 2020 2020 292c 2066 2268 6173 685f 6765      ), f"hash_ge
+00017b80: 6f6d 6574 7279 203d 207b 7265 6d61 702e  ometry = {remap.
+00017b90: 6861 7368 5f67 656f 6d65 7472 7928 2921  hash_geometry()!
+00017ba0: 727d 220a 0a0a 6465 6620 7465 7374 5f72  r}"...def test_r
+00017bb0: 656d 6f76 655f 6c61 6265 6c73 2829 202d  emove_labels() -
+00017bc0: 3e20 4e6f 6e65 3a0a 2020 2020 696d 706f  > None:.    impo
+00017bd0: 7274 2067 6473 6661 6374 6f72 7920 6173  rt gdsfactory as
+00017be0: 2067 660a 0a20 2020 2063 203d 2067 662e   gf..    c = gf.
+00017bf0: 632e 7374 7261 6967 6874 2829 0a20 2020  c.straight().   
+00017c00: 2063 2e72 656d 6f76 655f 6c61 6265 6c73   c.remove_labels
+00017c10: 2829 0a0a 2020 2020 6173 7365 7274 206c  ()..    assert l
+00017c20: 656e 2863 2e6c 6162 656c 7329 203d 3d20  en(c.labels) == 
+00017c30: 300a 0a0a 6465 6620 7465 7374 5f69 6d70  0...def test_imp
+00017c40: 6f72 745f 6764 735f 7365 7474 696e 6773  ort_gds_settings
+00017c50: 2829 3a0a 2020 2020 696d 706f 7274 2067  ():.    import g
+00017c60: 6473 6661 6374 6f72 7920 6173 2067 660a  dsfactory as gf.
+00017c70: 0a20 2020 2063 203d 2067 662e 636f 6d70  .    c = gf.comp
+00017c80: 6f6e 656e 7473 2e6d 7a69 2829 0a20 2020  onents.mzi().   
+00017c90: 2067 6473 7061 7468 203d 2063 2e77 7269   gdspath = c.wri
+00017ca0: 7465 5f67 6473 5f77 6974 685f 6d65 7461  te_gds_with_meta
+00017cb0: 6461 7461 2829 0a20 2020 2063 3220 3d20  data().    c2 = 
+00017cc0: 6766 2e69 6d70 6f72 745f 6764 7328 6764  gf.import_gds(gd
+00017cd0: 7370 6174 682c 206e 616d 653d 226d 7a69  spath, name="mzi
+00017ce0: 5f73 616d 706c 6522 2c20 7265 6164 5f6d  _sample", read_m
+00017cf0: 6574 6164 6174 613d 5472 7565 290a 2020  etadata=True).  
+00017d00: 2020 6333 203d 2067 662e 726f 7574 696e    c3 = gf.routin
+00017d10: 672e 6164 645f 6669 6265 725f 7369 6e67  g.add_fiber_sing
+00017d20: 6c65 2863 3229 0a20 2020 2061 7373 6572  le(c2).    asser
+00017d30: 7420 6333 0a0a 0a64 6566 2074 6573 745f  t c3...def test_
+00017d40: 666c 6174 7465 6e5f 696e 7661 6c69 645f  flatten_invalid_
+00017d50: 7265 6673 5f72 6563 7572 7369 7665 2829  refs_recursive()
+00017d60: 3a0a 2020 2020 696d 706f 7274 2067 6473  :.    import gds
+00017d70: 6661 6374 6f72 7920 6173 2067 660a 2020  factory as gf.  
+00017d80: 2020 6672 6f6d 2067 6473 6661 6374 6f72    from gdsfactor
+00017d90: 792e 6469 6666 7465 7374 2069 6d70 6f72  y.difftest impor
+00017da0: 7420 7275 6e5f 786f 720a 2020 2020 6672  t run_xor.    fr
+00017db0: 6f6d 2067 6473 6661 6374 6f72 792e 726f  om gdsfactory.ro
+00017dc0: 7574 696e 672e 616c 6c5f 616e 676c 6520  uting.all_angle 
+00017dd0: 696d 706f 7274 2067 6574 5f62 756e 646c  import get_bundl
+00017de0: 655f 616c 6c5f 616e 676c 650a 0a20 2020  e_all_angle..   
+00017df0: 2040 6766 2e63 656c 6c0a 2020 2020 6465   @gf.cell.    de
+00017e00: 6620 666c 6174 2829 3a0a 2020 2020 2020  f flat():.      
+00017e10: 2020 6320 3d20 6766 2e43 6f6d 706f 6e65    c = gf.Compone
+00017e20: 6e74 2829 0a20 2020 2020 2020 206d 6d69  nt().        mmi
+00017e30: 3120 3d20 2863 203c 3c20 6766 2e63 6f6d  1 = (c << gf.com
+00017e40: 706f 6e65 6e74 732e 6d6d 6931 7832 2829  ponents.mmi1x2()
+00017e50: 292e 6d6f 7665 2828 302c 202d 312e 3030  ).move((0, -1.00
+00017e60: 3035 2929 0a20 2020 2020 2020 206d 6d69  05)).        mmi
+00017e70: 3220 3d20 2863 203c 3c20 6766 2e63 6f6d  2 = (c << gf.com
+00017e80: 706f 6e65 6e74 732e 6d6d 6931 7832 2829  ponents.mmi1x2()
+00017e90: 292e 726f 7461 7465 2838 3029 0a20 2020  ).rotate(80).   
+00017ea0: 2020 2020 206d 6d69 322e 6d6f 7665 2828       mmi2.move((
+00017eb0: 3430 2c20 3230 2929 0a20 2020 2020 2020  40, 20)).       
+00017ec0: 2062 756e 646c 6520 3d20 6765 745f 6275   bundle = get_bu
+00017ed0: 6e64 6c65 5f61 6c6c 5f61 6e67 6c65 285b  ndle_all_angle([
+00017ee0: 6d6d 6931 2e70 6f72 7473 5b22 6f32 225d  mmi1.ports["o2"]
+00017ef0: 5d2c 205b 6d6d 6932 2e70 6f72 7473 5b22  ], [mmi2.ports["
+00017f00: 6f31 225d 5d29 0a20 2020 2020 2020 2066  o1"]]).        f
+00017f10: 6f72 2072 6f75 7465 2069 6e20 6275 6e64  or route in bund
+00017f20: 6c65 3a0a 2020 2020 2020 2020 2020 2020  le:.            
+00017f30: 632e 6164 6428 726f 7574 652e 7265 6665  c.add(route.refe
+00017f40: 7265 6e63 6573 290a 2020 2020 2020 2020  rences).        
+00017f50: 7265 7475 726e 2063 0a0a 2020 2020 4067  return c..    @g
+00017f60: 662e 6365 6c6c 0a20 2020 2064 6566 2068  f.cell.    def h
+00017f70: 6965 7261 7263 6879 2829 3a0a 2020 2020  ierarchy():.    
+00017f80: 2020 2020 6320 3d20 6766 2e43 6f6d 706f      c = gf.Compo
+00017f90: 6e65 6e74 2829 0a20 2020 2020 2020 2028  nent().        (
+00017fa0: 6320 3c3c 2066 6c61 7428 2929 2e72 6f74  c << flat()).rot
+00017fb0: 6174 6528 3333 290a 2020 2020 2020 2020  ate(33).        
+00017fc0: 2863 203c 3c20 666c 6174 2829 292e 726f  (c << flat()).ro
+00017fd0: 7461 7465 2833 3329 2e6d 6f76 6528 2830  tate(33).move((0
+00017fe0: 2c20 3130 3029 290a 2020 2020 2020 2020  , 100)).        
+00017ff0: 2863 203c 3c20 666c 6174 2829 292e 6d6f  (c << flat()).mo
+00018000: 7665 2828 3130 302c 2030 2929 0a20 2020  ve((100, 0)).   
+00018010: 2020 2020 2072 6574 7572 6e20 630a 0a20       return c.. 
+00018020: 2020 2063 5f6f 7269 6720 3d20 6869 6572     c_orig = hier
+00018030: 6172 6368 7928 290a 2020 2020 635f 6e65  archy().    c_ne
+00018040: 7720 3d20 666c 6174 7465 6e5f 696e 7661  w = flatten_inva
+00018050: 6c69 645f 7265 6673 5f72 6563 7572 7369  lid_refs_recursi
+00018060: 7665 2863 5f6f 7269 6729 0a20 2020 2061  ve(c_orig).    a
+00018070: 7373 6572 7420 635f 6e65 7720 6973 206e  ssert c_new is n
+00018080: 6f74 2063 5f6f 7269 670a 2020 2020 696e  ot c_orig.    in
+00018090: 7661 6c69 645f 7265 6673 5f66 696c 656e  valid_refs_filen
+000180a0: 616d 6520 3d20 2269 6e76 616c 6964 5f72  ame = "invalid_r
+000180b0: 6566 732e 6764 7322 0a20 2020 2069 6e76  efs.gds".    inv
+000180c0: 616c 6964 5f72 6566 735f 6669 7865 645f  alid_refs_fixed_
+000180d0: 6669 6c65 6e61 6d65 203d 2022 696e 7661  filename = "inva
+000180e0: 6c69 645f 7265 6673 5f66 6978 6564 2e67  lid_refs_fixed.g
+000180f0: 6473 220a 2020 2020 2320 6764 7320 6669  ds".    # gds fi
+00018100: 6c65 7320 7368 6f75 6c64 2073 7469 6c6c  les should still
+00018110: 2062 6520 7361 6d65 2074 6f20 316e 6d20   be same to 1nm 
+00018120: 746f 6c65 7261 6e63 650a 2020 2020 635f  tolerance.    c_
+00018130: 6f72 6967 2e77 7269 7465 5f67 6473 2869  orig.write_gds(i
+00018140: 6e76 616c 6964 5f72 6566 735f 6669 6c65  nvalid_refs_file
+00018150: 6e61 6d65 290a 2020 2020 635f 6e65 772e  name).    c_new.
+00018160: 7772 6974 655f 6764 7328 696e 7661 6c69  write_gds(invali
+00018170: 645f 7265 6673 5f66 6978 6564 5f66 696c  d_refs_fixed_fil
+00018180: 656e 616d 6529 0a20 2020 2072 756e 5f78  ename).    run_x
+00018190: 6f72 2869 6e76 616c 6964 5f72 6566 735f  or(invalid_refs_
+000181a0: 6669 6c65 6e61 6d65 2c20 696e 7661 6c69  filename, invali
+000181b0: 645f 7265 6673 5f66 6978 6564 5f66 696c  d_refs_fixed_fil
+000181c0: 656e 616d 6529 0a0a 0a69 6620 5f5f 6e61  ename)...if __na
+000181d0: 6d65 5f5f 203d 3d20 225f 5f6d 6169 6e5f  me__ == "__main_
+000181e0: 5f22 3a0a 2020 2020 696d 706f 7274 2067  _":.    import g
+000181f0: 6473 6661 6374 6f72 7920 6173 2067 660a  dsfactory as gf.
+00018200: 0a20 2020 2023 2063 3220 3d20 6766 2e43  .    # c2 = gf.C
+00018210: 6f6d 706f 6e65 6e74 2829 0a20 2020 2063  omponent().    c
+00018220: 203d 2067 662e 636f 6d70 6f6e 656e 7473   = gf.components
+00018230: 2e6d 7a69 2829 0a20 2020 2070 7269 6e74  .mzi().    print
+00018240: 2863 2e67 6574 5f6c 6179 6572 5f6e 616d  (c.get_layer_nam
+00018250: 6573 2829 290a 2020 2020 2320 7220 3d20  es()).    # r = 
+00018260: 632e 7265 6628 290a 2020 2020 2320 6332  c.ref().    # c2
+00018270: 2e63 6f70 795f 6368 696c 645f 696e 666f  .copy_child_info
+00018280: 2863 2e6e 616d 6564 5f72 6566 6572 656e  (c.named_referen
+00018290: 6365 735b 2273 7874 225d 290a 2020 2020  ces["sxt"]).    
+000182a0: 2320 7465 7374 5f72 656d 6170 5f6c 6179  # test_remap_lay
+000182b0: 6572 7328 290a 2020 2020 2320 6320 3d20  ers().    # c = 
+000182c0: 7465 7374 5f67 6574 5f6c 6179 6572 7328  test_get_layers(
+000182d0: 290a 2020 2020 2320 632e 706c 6f74 5f71  ).    # c.plot_q
+000182e0: 7428 290a 2020 2020 2320 632e 706c 6f74  t().    # c.plot
+000182f0: 6828 290a 2020 2020 2320 6320 3d20 7465  h().    # c = te
+00018300: 7374 5f65 7874 7261 6374 2829 0a20 2020  st_extract().   
+00018310: 2023 2067 6473 7061 7468 203d 2063 2e77   # gdspath = c.w
+00018320: 7269 7465 5f67 6473 2829 0a20 2020 2023  rite_gds().    #
+00018330: 2067 662e 7368 6f77 2867 6473 7061 7468   gf.show(gdspath
+00018340: 290a 2020 2020 2320 632e 7368 6f77 2873  ).    # c.show(s
+00018350: 686f 775f 706f 7274 733d 5472 7565 290a  how_ports=True).
+00018360: 2020 2020 632e 7368 6f77 2829 0a             c.show().
```

### Comparing `gdsfactory-6.91.0/gdsfactory/component_layout.py` & `gdsfactory-6.92.0/gdsfactory/component_layout.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/component_reference.py` & `gdsfactory-6.92.0/gdsfactory/component_reference.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/C.py` & `gdsfactory-6.92.0/gdsfactory/components/C.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/L.py` & `gdsfactory-6.92.0/gdsfactory/components/L.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/__init__.py` & `gdsfactory-6.92.0/gdsfactory/components/__init__.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/add_fiducials.py` & `gdsfactory-6.92.0/gdsfactory/components/add_fiducials.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/add_grating_couplers.py` & `gdsfactory-6.92.0/gdsfactory/components/add_grating_couplers.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/add_trenches.py` & `gdsfactory-6.92.0/gdsfactory/components/add_trenches.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/align.py` & `gdsfactory-6.92.0/gdsfactory/components/align.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/array_component.py` & `gdsfactory-6.92.0/gdsfactory/components/array_component.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/array_with_fanout.py` & `gdsfactory-6.92.0/gdsfactory/components/array_with_fanout.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/array_with_via.py` & `gdsfactory-6.92.0/gdsfactory/components/array_with_via.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/awg.py` & `gdsfactory-6.92.0/gdsfactory/components/awg.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/bbox.py` & `gdsfactory-6.92.0/gdsfactory/components/bbox.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/bend_circular.py` & `gdsfactory-6.92.0/gdsfactory/components/bend_circular.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/bend_circular_heater.py` & `gdsfactory-6.92.0/gdsfactory/components/bend_circular_heater.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/bend_euler.py` & `gdsfactory-6.92.0/gdsfactory/components/bend_euler.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/bend_port.py` & `gdsfactory-6.92.0/gdsfactory/components/bend_port.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/bend_s.py` & `gdsfactory-6.92.0/gdsfactory/components/bend_s.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/bezier.py` & `gdsfactory-6.92.0/gdsfactory/components/bezier.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/cavity.py` & `gdsfactory-6.92.0/gdsfactory/components/cavity.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/cdc.py` & `gdsfactory-6.92.0/gdsfactory/components/cdc.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/cdsem_all.py` & `gdsfactory-6.92.0/gdsfactory/components/cdsem_all.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/cdsem_bend180.py` & `gdsfactory-6.92.0/gdsfactory/components/cdsem_bend180.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/cdsem_coupler.py` & `gdsfactory-6.92.0/gdsfactory/components/cdsem_coupler.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/cdsem_straight.py` & `gdsfactory-6.92.0/gdsfactory/components/cdsem_straight.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/cdsem_straight_density.py` & `gdsfactory-6.92.0/gdsfactory/components/cdsem_straight_density.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/circle.py` & `gdsfactory-6.92.0/gdsfactory/components/circle.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/coh_rx_dual_pol.py` & `gdsfactory-6.92.0/gdsfactory/components/coh_rx_dual_pol.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/coh_rx_single_pol.py` & `gdsfactory-6.92.0/gdsfactory/components/coh_rx_single_pol.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/coh_tx_dual_pol.py` & `gdsfactory-6.92.0/gdsfactory/components/coh_tx_dual_pol.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/coh_tx_single_pol.py` & `gdsfactory-6.92.0/gdsfactory/components/coh_tx_single_pol.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/compass.py` & `gdsfactory-6.92.0/gdsfactory/components/compass.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/component_lattice.py` & `gdsfactory-6.92.0/gdsfactory/components/component_lattice.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/component_sequence.py` & `gdsfactory-6.92.0/gdsfactory/components/component_sequence.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/copy_layers.py` & `gdsfactory-6.92.0/gdsfactory/components/copy_layers.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/coupler.py` & `gdsfactory-6.92.0/gdsfactory/components/coupler.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/coupler90.py` & `gdsfactory-6.92.0/gdsfactory/components/coupler90.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/coupler90bend.py` & `gdsfactory-6.92.0/gdsfactory/components/coupler90bend.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/coupler_adiabatic.py` & `gdsfactory-6.92.0/gdsfactory/components/coupler_adiabatic.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/coupler_asymmetric.py` & `gdsfactory-6.92.0/gdsfactory/components/coupler_asymmetric.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/coupler_full.py` & `gdsfactory-6.92.0/gdsfactory/components/coupler_full.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/coupler_ring.py` & `gdsfactory-6.92.0/gdsfactory/components/coupler_ring.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/coupler_straight.py` & `gdsfactory-6.92.0/gdsfactory/components/coupler_straight.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/coupler_straight_asymmetric.py` & `gdsfactory-6.92.0/gdsfactory/components/coupler_straight_asymmetric.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/coupler_symmetric.py` & `gdsfactory-6.92.0/gdsfactory/components/coupler_symmetric.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/cross.py` & `gdsfactory-6.92.0/gdsfactory/components/cross.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/crossing_waveguide.py` & `gdsfactory-6.92.0/gdsfactory/components/crossing_waveguide.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/csv_data/grating_coupler_2etch_h220_e70_e220.csv` & `gdsfactory-6.92.0/gdsfactory/components/csv_data/grating_coupler_2etch_h220_e70_e220.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/csv_data/taper_strip_0p5_10_100.csv` & `gdsfactory-6.92.0/gdsfactory/components/csv_data/taper_strip_0p5_10_100.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/csv_data/taper_strip_0p5_10_150.csv` & `gdsfactory-6.92.0/gdsfactory/components/csv_data/taper_strip_0p5_10_150.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/csv_data/taper_strip_0p5_10_200.csv` & `gdsfactory-6.92.0/gdsfactory/components/csv_data/taper_strip_0p5_10_200.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/csv_data/taper_strip_0p5_11_200.csv` & `gdsfactory-6.92.0/gdsfactory/components/csv_data/taper_strip_0p5_11_200.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/csv_data/taper_strip_0p5_12_200.csv` & `gdsfactory-6.92.0/gdsfactory/components/csv_data/taper_strip_0p5_12_200.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/csv_data/taper_strip_0p5_3_36.csv` & `gdsfactory-6.92.0/gdsfactory/components/csv_data/taper_strip_0p5_3_36.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/cutback_2x2.py` & `gdsfactory-6.92.0/gdsfactory/components/cutback_2x2.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/cutback_bend.py` & `gdsfactory-6.92.0/gdsfactory/components/cutback_bend.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/cutback_component.py` & `gdsfactory-6.92.0/gdsfactory/components/cutback_component.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/cutback_splitter.py` & `gdsfactory-6.92.0/gdsfactory/components/cutback_splitter.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/dbr.py` & `gdsfactory-6.92.0/gdsfactory/components/dbr.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/dbr_tapered.py` & `gdsfactory-6.92.0/gdsfactory/components/dbr_tapered.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/delay_snake.py` & `gdsfactory-6.92.0/gdsfactory/components/delay_snake.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/delay_snake2.py` & `gdsfactory-6.92.0/gdsfactory/components/delay_snake2.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/delay_snake3.py` & `gdsfactory-6.92.0/gdsfactory/components/delay_snake3.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/delay_snake_sbend.py` & `gdsfactory-6.92.0/gdsfactory/components/delay_snake_sbend.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/dicing_lane.py` & `gdsfactory-6.92.0/gdsfactory/components/dicing_lane.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/die.py` & `gdsfactory-6.92.0/gdsfactory/components/die.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/die_bbox.py` & `gdsfactory-6.92.0/gdsfactory/components/die_bbox.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/die_bbox_frame.py` & `gdsfactory-6.92.0/gdsfactory/components/die_bbox_frame.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/disk.py` & `gdsfactory-6.92.0/gdsfactory/components/disk.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/edge_coupler_array.py` & `gdsfactory-6.92.0/gdsfactory/components/edge_coupler_array.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/ellipse.py` & `gdsfactory-6.92.0/gdsfactory/components/ellipse.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/extend_ports_list.py` & `gdsfactory-6.92.0/gdsfactory/components/extend_ports_list.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/extension.py` & `gdsfactory-6.92.0/gdsfactory/components/extension.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/fiber.py` & `gdsfactory-6.92.0/gdsfactory/components/fiber.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/fiber_array.py` & `gdsfactory-6.92.0/gdsfactory/components/fiber_array.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/fiducial_squares.py` & `gdsfactory-6.92.0/gdsfactory/components/fiducial_squares.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/ge_detector_straight_si_contacts.py` & `gdsfactory-6.92.0/gdsfactory/components/ge_detector_straight_si_contacts.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/grating_coupler_array.py` & `gdsfactory-6.92.0/gdsfactory/components/grating_coupler_array.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/grating_coupler_dual_pol.py` & `gdsfactory-6.92.0/gdsfactory/components/grating_coupler_dual_pol.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/grating_coupler_elliptical.py` & `gdsfactory-6.92.0/gdsfactory/components/grating_coupler_elliptical.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/grating_coupler_elliptical_arbitrary.py` & `gdsfactory-6.92.0/gdsfactory/components/grating_coupler_elliptical_arbitrary.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/grating_coupler_elliptical_lumerical.py` & `gdsfactory-6.92.0/gdsfactory/components/grating_coupler_elliptical_lumerical.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/grating_coupler_elliptical_trenches.py` & `gdsfactory-6.92.0/gdsfactory/components/grating_coupler_elliptical_trenches.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/grating_coupler_functions.py` & `gdsfactory-6.92.0/gdsfactory/components/grating_coupler_functions.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/grating_coupler_loss.py` & `gdsfactory-6.92.0/gdsfactory/components/grating_coupler_loss.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/grating_coupler_loss_fiber_single.py` & `gdsfactory-6.92.0/gdsfactory/components/grating_coupler_loss_fiber_single.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/grating_coupler_rectangular.py` & `gdsfactory-6.92.0/gdsfactory/components/grating_coupler_rectangular.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/grating_coupler_rectangular_arbitrary.py` & `gdsfactory-6.92.0/gdsfactory/components/grating_coupler_rectangular_arbitrary.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/grating_coupler_rectangular_arbitrary_slab.py` & `gdsfactory-6.92.0/gdsfactory/components/grating_coupler_rectangular_arbitrary_slab.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/grating_coupler_tree.py` & `gdsfactory-6.92.0/gdsfactory/components/grating_coupler_tree.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/greek_cross.py` & `gdsfactory-6.92.0/gdsfactory/components/greek_cross.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/hline.py` & `gdsfactory-6.92.0/gdsfactory/components/hline.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/interdigital_capacitor.py` & `gdsfactory-6.92.0/gdsfactory/components/interdigital_capacitor.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/litho_calipers.py` & `gdsfactory-6.92.0/gdsfactory/components/litho_calipers.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/litho_ruler.py` & `gdsfactory-6.92.0/gdsfactory/components/litho_ruler.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/litho_steps.py` & `gdsfactory-6.92.0/gdsfactory/components/litho_steps.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/logo.py` & `gdsfactory-6.92.0/gdsfactory/components/logo.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/loop_mirror.py` & `gdsfactory-6.92.0/gdsfactory/components/loop_mirror.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/mmi1x2.py` & `gdsfactory-6.92.0/gdsfactory/components/mmi1x2.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/mmi1x2_with_sbend.py` & `gdsfactory-6.92.0/gdsfactory/components/mmi1x2_with_sbend.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/mmi2x2.py` & `gdsfactory-6.92.0/gdsfactory/components/mmi2x2.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/mmi2x2_with_sbend.py` & `gdsfactory-6.92.0/gdsfactory/components/mmi2x2_with_sbend.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/mmi_90degree_hybrid.py` & `gdsfactory-6.92.0/gdsfactory/components/mmi_90degree_hybrid.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/mode_converter.py` & `gdsfactory-6.92.0/gdsfactory/components/mode_converter.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/mzi.py` & `gdsfactory-6.92.0/gdsfactory/components/mzi.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/mzi_arm.py` & `gdsfactory-6.92.0/gdsfactory/components/mzi_arm.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/mzi_arms.py` & `gdsfactory-6.92.0/gdsfactory/components/mzi_arms.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/mzi_lattice.py` & `gdsfactory-6.92.0/gdsfactory/components/mzi_lattice.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/mzi_pads_center.py` & `gdsfactory-6.92.0/gdsfactory/components/mzi_pads_center.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/mzi_phase_shifter.py` & `gdsfactory-6.92.0/gdsfactory/components/mzi_phase_shifter.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/mzit.py` & `gdsfactory-6.92.0/gdsfactory/components/mzit.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/mzit_lattice.py` & `gdsfactory-6.92.0/gdsfactory/components/mzit_lattice.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/mzm.py` & `gdsfactory-6.92.0/gdsfactory/components/mzm.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/nxn.py` & `gdsfactory-6.92.0/gdsfactory/components/nxn.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/optimal_90deg.py` & `gdsfactory-6.92.0/gdsfactory/components/optimal_90deg.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/optimal_hairpin.py` & `gdsfactory-6.92.0/gdsfactory/components/optimal_hairpin.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/optimal_step.py` & `gdsfactory-6.92.0/gdsfactory/components/optimal_step.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/pack_doe.py` & `gdsfactory-6.92.0/gdsfactory/components/pack_doe.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/pad.py` & `gdsfactory-6.92.0/gdsfactory/components/pad.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/pad_gsg.py` & `gdsfactory-6.92.0/gdsfactory/components/pad_gsg.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/pads_shorted.py` & `gdsfactory-6.92.0/gdsfactory/components/pads_shorted.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/polarization_splitter_rotator.py` & `gdsfactory-6.92.0/gdsfactory/components/polarization_splitter_rotator.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/ramp.py` & `gdsfactory-6.92.0/gdsfactory/components/ramp.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/rectangle.py` & `gdsfactory-6.92.0/gdsfactory/components/rectangle.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/rectangle_with_slits.py` & `gdsfactory-6.92.0/gdsfactory/components/rectangle_with_slits.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/regular_polygon.py` & `gdsfactory-6.92.0/gdsfactory/components/regular_polygon.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/resistance_meander.py` & `gdsfactory-6.92.0/gdsfactory/components/resistance_meander.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/resistance_sheet.py` & `gdsfactory-6.92.0/gdsfactory/components/resistance_sheet.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/ring.py` & `gdsfactory-6.92.0/gdsfactory/components/ring.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/ring_crow.py` & `gdsfactory-6.92.0/gdsfactory/components/ring_crow.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/ring_crow_couplers.py` & `gdsfactory-6.92.0/gdsfactory/components/ring_crow_couplers.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/ring_double.py` & `gdsfactory-6.92.0/gdsfactory/components/ring_double.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/ring_double_heater.py` & `gdsfactory-6.92.0/gdsfactory/components/ring_double_heater.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/ring_double_pn.py` & `gdsfactory-6.92.0/gdsfactory/components/ring_double_pn.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/ring_section_based.py` & `gdsfactory-6.92.0/gdsfactory/components/ring_section_based.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/ring_single.py` & `gdsfactory-6.92.0/gdsfactory/components/ring_single.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/ring_single_array.py` & `gdsfactory-6.92.0/gdsfactory/components/ring_single_array.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/ring_single_bend_coupler.py` & `gdsfactory-6.92.0/gdsfactory/components/ring_single_bend_coupler.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/ring_single_dut.py` & `gdsfactory-6.92.0/gdsfactory/components/ring_single_dut.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/ring_single_heater.py` & `gdsfactory-6.92.0/gdsfactory/components/ring_single_heater.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/ring_single_pn.py` & `gdsfactory-6.92.0/gdsfactory/components/ring_single_pn.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/seal_ring.py` & `gdsfactory-6.92.0/gdsfactory/components/seal_ring.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/snspd.py` & `gdsfactory-6.92.0/gdsfactory/components/snspd.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/spiral_double.py` & `gdsfactory-6.92.0/gdsfactory/components/spiral_double.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/spiral_external_io.py` & `gdsfactory-6.92.0/gdsfactory/components/spiral_external_io.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/spiral_heater.py` & `gdsfactory-6.92.0/gdsfactory/components/spiral_heater.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/spiral_inner_io.py` & `gdsfactory-6.92.0/gdsfactory/components/spiral_inner_io.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/splitter_chain.py` & `gdsfactory-6.92.0/gdsfactory/components/splitter_chain.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/splitter_tree.py` & `gdsfactory-6.92.0/gdsfactory/components/splitter_tree.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/straight.py` & `gdsfactory-6.92.0/gdsfactory/components/straight.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/straight_array.py` & `gdsfactory-6.92.0/gdsfactory/components/straight_array.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/straight_heater_doped_rib.py` & `gdsfactory-6.92.0/gdsfactory/components/straight_heater_doped_rib.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/straight_heater_doped_strip.py` & `gdsfactory-6.92.0/gdsfactory/components/straight_heater_doped_strip.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/straight_heater_meander.py` & `gdsfactory-6.92.0/gdsfactory/components/straight_heater_meander.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/straight_heater_meander_doped.py` & `gdsfactory-6.92.0/gdsfactory/components/straight_heater_meander_doped.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/straight_heater_metal.py` & `gdsfactory-6.92.0/gdsfactory/components/straight_heater_metal.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/straight_pin.py` & `gdsfactory-6.92.0/gdsfactory/components/straight_pin.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/straight_pin_slot.py` & `gdsfactory-6.92.0/gdsfactory/components/straight_pin_slot.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/straight_rib.py` & `gdsfactory-6.92.0/gdsfactory/components/straight_rib.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/switch_tree.py` & `gdsfactory-6.92.0/gdsfactory/components/switch_tree.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/taper.py` & `gdsfactory-6.92.0/gdsfactory/components/taper.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/taper_adiabatic.py` & `gdsfactory-6.92.0/gdsfactory/components/taper_adiabatic.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/taper_cross_section.py` & `gdsfactory-6.92.0/gdsfactory/components/taper_cross_section.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/taper_from_csv.py` & `gdsfactory-6.92.0/gdsfactory/components/taper_from_csv.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/taper_parabolic.py` & `gdsfactory-6.92.0/gdsfactory/components/taper_parabolic.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/terminator.py` & `gdsfactory-6.92.0/gdsfactory/components/terminator.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/text.py` & `gdsfactory-6.92.0/gdsfactory/components/text.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/text_freetype.py` & `gdsfactory-6.92.0/gdsfactory/components/text_freetype.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/text_rectangular.py` & `gdsfactory-6.92.0/gdsfactory/components/text_rectangular.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/text_rectangular_font.py` & `gdsfactory-6.92.0/gdsfactory/components/text_rectangular_font.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/triangles.py` & `gdsfactory-6.92.0/gdsfactory/components/triangles.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/verniers.py` & `gdsfactory-6.92.0/gdsfactory/components/verniers.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/version_stamp.py` & `gdsfactory-6.92.0/gdsfactory/components/version_stamp.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/via.py` & `gdsfactory-6.92.0/gdsfactory/components/via.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/via_corner.py` & `gdsfactory-6.92.0/gdsfactory/components/via_corner.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/via_cutback.py` & `gdsfactory-6.92.0/gdsfactory/components/via_cutback.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/via_stack.py` & `gdsfactory-6.92.0/gdsfactory/components/via_stack.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/via_stack_slot.py` & `gdsfactory-6.92.0/gdsfactory/components/via_stack_slot.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/via_stack_with_offset.py` & `gdsfactory-6.92.0/gdsfactory/components/via_stack_with_offset.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/wafer.py` & `gdsfactory-6.92.0/gdsfactory/components/wafer.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/wire.py` & `gdsfactory-6.92.0/gdsfactory/components/wire.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/components/wire_sbend.py` & `gdsfactory-6.92.0/gdsfactory/components/wire_sbend.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/config.py` & `gdsfactory-6.92.0/gdsfactory/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 from loguru import logger
 import omegaconf
 from omegaconf import OmegaConf
 
 from rich.console import Console
 from rich.table import Table
 
-__version__ = "6.91.0"
+__version__ = "6.92.0"
 PathType = Union[str, pathlib.Path]
 
 home = pathlib.Path.home()
 cwd = pathlib.Path.cwd()
 module_path = pathlib.Path(__file__).parent.absolute()
 repo_path = module_path.parent
 home_path = pathlib.Path.home() / ".gdsfactory"
```

### Comparing `gdsfactory-6.91.0/gdsfactory/constants.py` & `gdsfactory-6.92.0/gdsfactory/constants.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/containers.py` & `gdsfactory-6.92.0/gdsfactory/containers.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/cross_section.py` & `gdsfactory-6.92.0/gdsfactory/cross_section.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/decorators.py` & `gdsfactory-6.92.0/gdsfactory/decorators.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/difftest.py` & `gdsfactory-6.92.0/gdsfactory/difftest.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/events.py` & `gdsfactory-6.92.0/gdsfactory/events.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/export/to_3d.py` & `gdsfactory-6.92.0/gdsfactory/export/to_3d.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/export/to_np.py` & `gdsfactory-6.92.0/gdsfactory/export/to_np.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/export/to_stl.py` & `gdsfactory-6.92.0/gdsfactory/export/to_stl.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/export/write_gerbers.py` & `gdsfactory-6.92.0/gdsfactory/export/write_gerbers.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/filestorage.py` & `gdsfactory-6.92.0/gdsfactory/filestorage.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/fill.py` & `gdsfactory-6.92.0/gdsfactory/fill.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/font.py` & `gdsfactory-6.92.0/gdsfactory/font.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/functions.py` & `gdsfactory-6.92.0/gdsfactory/functions.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/gdsdiff/gds_diff_git.py` & `gdsfactory-6.92.0/gdsfactory/gdsdiff/gds_diff_git.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/gdsdiff/gdsdiff.py` & `gdsfactory-6.92.0/gdsfactory/gdsdiff/gdsdiff.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/gdsdiff/install.py` & `gdsfactory-6.92.0/gdsfactory/gdsdiff/install.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/gdsdiff/test_xor.py` & `gdsfactory-6.92.0/gdsfactory/gdsdiff/test_xor.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/generic_tech/README.md` & `gdsfactory-6.92.0/gdsfactory/generic_tech/README.md`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/generic_tech/__init__.py` & `gdsfactory-6.92.0/gdsfactory/generic_tech/__init__.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/generic_tech/get_klayout_pyxs.py` & `gdsfactory-6.92.0/gdsfactory/generic_tech/get_klayout_pyxs.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/generic_tech/klayout/drc/errors.py` & `gdsfactory-6.92.0/gdsfactory/generic_tech/klayout/drc/errors.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/generic_tech/klayout/drc/generic.drc` & `gdsfactory-6.92.0/gdsfactory/generic_tech/klayout/drc/generic.drc`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/generic_tech/klayout/drc/generic.lydrc` & `gdsfactory-6.92.0/gdsfactory/generic_tech/klayout/drc/generic.lydrc`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/generic_tech/klayout/drc/write_drc.py` & `gdsfactory-6.92.0/gdsfactory/generic_tech/klayout/drc/write_drc.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/generic_tech/klayout/grain.xml` & `gdsfactory-6.92.0/gdsfactory/generic_tech/klayout/grain.xml`

 * *Files 0% similar despite different names*

#### Comparing `gdsfactory-6.91.0/gdsfactory/generic_tech/klayout/grain.xml` & `gdsfactory-6.92.0/gdsfactory/generic_tech/klayout/grain.xml`

```diff
@@ -1,13 +1,13 @@
 <?xml version="1.0" encoding="utf-8"?>
 <salt-grain>
   <name>gdsfactory</name>
   <token/>
   <hidden>false</hidden>
-  <version>6.91.0</version>
+  <version>6.92.0</version>
   <api-version/>
   <title>gdsfactory</title>
   <doc>EDA tool to layout integrated circuits</doc>
   <doc-url>https://gdsfactory.github.io/gdsfactory/</doc-url>
   <url>https://github.com/gdsfactory/gdsfactory</url>
   <license>MIT</license>
   <author>Joaquin Matres</author>
```

### Comparing `gdsfactory-6.91.0/gdsfactory/generic_tech/klayout/icon_128x128.png` & `gdsfactory-6.92.0/gdsfactory/generic_tech/klayout/icon_128x128.png`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/generic_tech/klayout/icon_64x64.png` & `gdsfactory-6.92.0/gdsfactory/generic_tech/klayout/icon_64x64.png`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/generic_tech/klayout/pymacros/import_generic_pcells.lym` & `gdsfactory-6.92.0/gdsfactory/generic_tech/klayout/pymacros/import_generic_pcells.lym`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/generic_tech/klayout/pymacros/set_menus.lym` & `gdsfactory-6.92.0/gdsfactory/generic_tech/klayout/pymacros/set_menus.lym`

 * *Files 0% similar despite different names*

#### Comparing `gdsfactory-6.91.0/gdsfactory/generic_tech/klayout/pymacros/set_menus.lym` & `gdsfactory-6.92.0/gdsfactory/generic_tech/klayout/pymacros/set_menus.lym`

```diff
@@ -12,15 +12,15 @@
   <show-in-menu>false</show-in-menu>
   <group-name/>
   <menu-path>gdsfactory.begin</menu-path>
   <interpreter>python</interpreter>
   <dsl-interpreter-name/>
   <text>import pya
 
-__version__ = &quot;6.91.0&quot;
+__version__ = &quot;6.92.0&quot;
 
 
 def set_menu():
     menu = pya.Application.instance().main_window().menu()
 
     s0 = &quot;gdsfactory&quot;
     if not (menu.is_menu(s0)):
```

### Comparing `gdsfactory-6.91.0/gdsfactory/generic_tech/klayout/pymacros/set_shortcuts.lym` & `gdsfactory-6.92.0/gdsfactory/generic_tech/klayout/pymacros/set_shortcuts.lym`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/generic_tech/klayout/python/kgdsfactory/shortcuts.py` & `gdsfactory-6.92.0/gdsfactory/generic_tech/klayout/python/kgdsfactory/shortcuts.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/generic_tech/klayout/tech/generic.layerstack` & `gdsfactory-6.92.0/gdsfactory/generic_tech/klayout/tech/generic.layerstack`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/generic_tech/klayout/tech/generic_tech.lyp` & `gdsfactory-6.92.0/gdsfactory/generic_tech/klayout/tech/generic_tech.lyp`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/generic_tech/klayout/tech/generic_tech.lyt` & `gdsfactory-6.92.0/gdsfactory/generic_tech/klayout/tech/generic_tech.lyt`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/generic_tech/klayout/tech/xsection_generic.pyxs` & `gdsfactory-6.92.0/gdsfactory/generic_tech/klayout/tech/xsection_generic.pyxs`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/generic_tech/klayout/tech/xsection_generic.xs` & `gdsfactory-6.92.0/gdsfactory/generic_tech/klayout/tech/xsection_generic.xs`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/generic_tech/klayout/tech/xsection_planarized.pyxs` & `gdsfactory-6.92.0/gdsfactory/generic_tech/klayout/tech/xsection_planarized.pyxs`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/generic_tech/klayout/tech/xsection_planarized.xs` & `gdsfactory-6.92.0/gdsfactory/generic_tech/klayout/tech/xsection_planarized.xs`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/generic_tech/layer_map.py` & `gdsfactory-6.92.0/gdsfactory/generic_tech/layer_map.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/generic_tech/layer_stack.py` & `gdsfactory-6.92.0/gdsfactory/generic_tech/layer_stack.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/generic_tech/layer_views.yaml` & `gdsfactory-6.92.0/gdsfactory/generic_tech/layer_views.yaml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/geometry/__init__.py` & `gdsfactory-6.92.0/gdsfactory/geometry/__init__.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/geometry/boolean.py` & `gdsfactory-6.92.0/gdsfactory/geometry/boolean.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/geometry/boolean_klayout.py` & `gdsfactory-6.92.0/gdsfactory/geometry/boolean_klayout.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/geometry/boolean_polygons.py` & `gdsfactory-6.92.0/gdsfactory/geometry/boolean_polygons.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/geometry/check_duplicated_cells.py` & `gdsfactory-6.92.0/gdsfactory/geometry/check_duplicated_cells.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/geometry/check_exclusion.py` & `gdsfactory-6.92.0/gdsfactory/geometry/check_exclusion.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/geometry/check_inclusion.py` & `gdsfactory-6.92.0/gdsfactory/geometry/check_inclusion.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/geometry/check_space.py` & `gdsfactory-6.92.0/gdsfactory/geometry/check_space.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/geometry/check_width.py` & `gdsfactory-6.92.0/gdsfactory/geometry/check_width.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/geometry/fill_klayout.py` & `gdsfactory-6.92.0/gdsfactory/geometry/fill_klayout.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/geometry/fill_tiled.py` & `gdsfactory-6.92.0/gdsfactory/geometry/fill_tiled.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/geometry/fillet.py` & `gdsfactory-6.92.0/gdsfactory/geometry/fillet.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/geometry/functions.py` & `gdsfactory-6.92.0/gdsfactory/geometry/functions.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/geometry/invert.py` & `gdsfactory-6.92.0/gdsfactory/geometry/invert.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/geometry/layer_priority.py` & `gdsfactory-6.92.0/gdsfactory/geometry/layer_priority.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/geometry/manhattanize.py` & `gdsfactory-6.92.0/gdsfactory/geometry/manhattanize.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/geometry/maskprep.py` & `gdsfactory-6.92.0/gdsfactory/geometry/maskprep.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/geometry/maskprep_flat.py` & `gdsfactory-6.92.0/gdsfactory/geometry/maskprep_flat.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/geometry/offset.py` & `gdsfactory-6.92.0/gdsfactory/geometry/offset.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/geometry/outline.py` & `gdsfactory-6.92.0/gdsfactory/geometry/outline.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/geometry/trim.py` & `gdsfactory-6.92.0/gdsfactory/geometry/trim.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/geometry/union.py` & `gdsfactory-6.92.0/gdsfactory/geometry/union.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/geometry/write_drc.py` & `gdsfactory-6.92.0/gdsfactory/geometry/write_drc.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/geometry/xor_diff.py` & `gdsfactory-6.92.0/gdsfactory/geometry/xor_diff.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/get_factories.py` & `gdsfactory-6.92.0/gdsfactory/get_factories.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/get_netlist.py` & `gdsfactory-6.92.0/gdsfactory/get_netlist.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/get_netlist_flat.py` & `gdsfactory-6.92.0/gdsfactory/get_netlist_flat.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/get_netlist_klayout.py` & `gdsfactory-6.92.0/gdsfactory/get_netlist_klayout.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/grid.py` & `gdsfactory-6.92.0/gdsfactory/grid.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/install.py` & `gdsfactory-6.92.0/gdsfactory/install.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/klive.py` & `gdsfactory-6.92.0/gdsfactory/klive.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/labels/__init__.py` & `gdsfactory-6.92.0/gdsfactory/labels/__init__.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/labels/add_label_yaml.py` & `gdsfactory-6.92.0/gdsfactory/labels/add_label_yaml.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/labels/ehva.py` & `gdsfactory-6.92.0/gdsfactory/labels/ehva.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/labels/merge_test_metadata.py` & `gdsfactory-6.92.0/gdsfactory/labels/merge_test_metadata.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/labels/siepic.py` & `gdsfactory-6.92.0/gdsfactory/labels/siepic.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/labels/write_labels.py` & `gdsfactory-6.92.0/gdsfactory/labels/write_labels.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/materials.py` & `gdsfactory-6.92.0/gdsfactory/materials.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/name.py` & `gdsfactory-6.92.0/gdsfactory/name.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/pack.py` & `gdsfactory-6.92.0/gdsfactory/pack.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/path.py` & `gdsfactory-6.92.0/gdsfactory/path.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/pdk.py` & `gdsfactory-6.92.0/gdsfactory/pdk.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/picmodel.py` & `gdsfactory-6.92.0/gdsfactory/picmodel.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/pixelate.py` & `gdsfactory-6.92.0/gdsfactory/pixelate.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/plugins/dagster/workflow.py` & `gdsfactory-6.92.0/gdsfactory/plugins/dagster/workflow.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/plugins/database/README.md` & `gdsfactory-6.92.0/gdsfactory/plugins/database/README.md`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/plugins/database/__init__.py` & `gdsfactory-6.92.0/gdsfactory/plugins/database/__init__.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/plugins/database/db_upload.py` & `gdsfactory-6.92.0/gdsfactory/plugins/database/db_upload.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/plugins/database/models.py` & `gdsfactory-6.92.0/gdsfactory/plugins/database/models.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/port.py` & `gdsfactory-6.92.0/gdsfactory/port.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/quickplotter.py` & `gdsfactory-6.92.0/gdsfactory/quickplotter.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/read/__init__.py` & `gdsfactory-6.92.0/gdsfactory/read/__init__.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/read/from_dphox.py` & `gdsfactory-6.92.0/gdsfactory/read/from_dphox.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/read/from_gdspaths.py` & `gdsfactory-6.92.0/gdsfactory/read/from_gdspaths.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/read/from_np.py` & `gdsfactory-6.92.0/gdsfactory/read/from_np.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/read/from_phidl.py` & `gdsfactory-6.92.0/gdsfactory/read/from_phidl.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/read/from_yaml.py` & `gdsfactory-6.92.0/gdsfactory/read/from_yaml.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/read/from_yaml_template.py` & `gdsfactory-6.92.0/gdsfactory/read/from_yaml_template.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/read/import_gds.py` & `gdsfactory-6.92.0/gdsfactory/read/import_gds.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/read/labels.py` & `gdsfactory-6.92.0/gdsfactory/read/labels.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/routing/__init__.py` & `gdsfactory-6.92.0/gdsfactory/routing/__init__.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/routing/add_electrical_pads_shortest.py` & `gdsfactory-6.92.0/gdsfactory/routing/add_electrical_pads_shortest.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/routing/add_electrical_pads_top.py` & `gdsfactory-6.92.0/gdsfactory/routing/add_electrical_pads_top.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/routing/add_electrical_pads_top_dc.py` & `gdsfactory-6.92.0/gdsfactory/routing/add_electrical_pads_top_dc.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/routing/add_fiber_array.py` & `gdsfactory-6.92.0/gdsfactory/routing/add_fiber_array.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/routing/add_fiber_single.py` & `gdsfactory-6.92.0/gdsfactory/routing/add_fiber_single.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/routing/add_pads.py` & `gdsfactory-6.92.0/gdsfactory/routing/add_pads.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/routing/all_angle.py` & `gdsfactory-6.92.0/gdsfactory/routing/all_angle.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/routing/auto_taper.py` & `gdsfactory-6.92.0/gdsfactory/routing/auto_taper.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/routing/factories.py` & `gdsfactory-6.92.0/gdsfactory/routing/factories.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/routing/fanout.py` & `gdsfactory-6.92.0/gdsfactory/routing/fanout.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/routing/fanout2x2.py` & `gdsfactory-6.92.0/gdsfactory/routing/fanout2x2.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/routing/get_bundle.py` & `gdsfactory-6.92.0/gdsfactory/routing/get_bundle.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/routing/get_bundle_corner.py` & `gdsfactory-6.92.0/gdsfactory/routing/get_bundle_corner.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/routing/get_bundle_from_steps.py` & `gdsfactory-6.92.0/gdsfactory/routing/get_bundle_from_steps.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/routing/get_bundle_from_waypoints.py` & `gdsfactory-6.92.0/gdsfactory/routing/get_bundle_from_waypoints.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/routing/get_bundle_path_length_match.py` & `gdsfactory-6.92.0/gdsfactory/routing/get_bundle_path_length_match.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/routing/get_bundle_sbend.py` & `gdsfactory-6.92.0/gdsfactory/routing/get_bundle_sbend.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/routing/get_bundle_u.py` & `gdsfactory-6.92.0/gdsfactory/routing/get_bundle_u.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/routing/get_input_labels.py` & `gdsfactory-6.92.0/gdsfactory/routing/get_input_labels.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/routing/get_route.py` & `gdsfactory-6.92.0/gdsfactory/routing/get_route.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/routing/get_route_astar.py` & `gdsfactory-6.92.0/gdsfactory/routing/get_route_astar.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/routing/get_route_from_steps.py` & `gdsfactory-6.92.0/gdsfactory/routing/get_route_from_steps.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/routing/get_route_sbend.py` & `gdsfactory-6.92.0/gdsfactory/routing/get_route_sbend.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/routing/get_routes_bend180.py` & `gdsfactory-6.92.0/gdsfactory/routing/get_routes_bend180.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/routing/get_routes_straight.py` & `gdsfactory-6.92.0/gdsfactory/routing/get_routes_straight.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/routing/manhattan.py` & `gdsfactory-6.92.0/gdsfactory/routing/manhattan.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/routing/path_length_matching.py` & `gdsfactory-6.92.0/gdsfactory/routing/path_length_matching.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/routing/route_fiber_array.py` & `gdsfactory-6.92.0/gdsfactory/routing/route_fiber_array.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/routing/route_fiber_single.py` & `gdsfactory-6.92.0/gdsfactory/routing/route_fiber_single.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/routing/route_ports_to_side.py` & `gdsfactory-6.92.0/gdsfactory/routing/route_ports_to_side.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/routing/route_quad.py` & `gdsfactory-6.92.0/gdsfactory/routing/route_quad.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/routing/route_sharp.py` & `gdsfactory-6.92.0/gdsfactory/routing/route_sharp.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/routing/route_south.py` & `gdsfactory-6.92.0/gdsfactory/routing/route_south.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/routing/sort_ports.py` & `gdsfactory-6.92.0/gdsfactory/routing/sort_ports.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/routing/utils.py` & `gdsfactory-6.92.0/gdsfactory/routing/utils.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/samples/01_component_pcell.py` & `gdsfactory-6.92.0/gdsfactory/samples/01_component_pcell.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/samples/01_component_pcell/test_straight_wide.yml` & `gdsfactory-6.92.0/gdsfactory/samples/01_component_pcell/test_straight_wide.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/samples/01_component_pcell_with_pins.py` & `gdsfactory-6.92.0/gdsfactory/samples/01_component_pcell_with_pins.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/samples/01_component_pcell_with_pins/test_straight_narrow.yml` & `gdsfactory-6.92.0/gdsfactory/samples/01_component_pcell_with_pins/test_straight_narrow.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/samples/03_move.py` & `gdsfactory-6.92.0/gdsfactory/samples/03_move.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/samples/04_connect.py` & `gdsfactory-6.92.0/gdsfactory/samples/04_connect.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/samples/05_remove_layers.py` & `gdsfactory-6.92.0/gdsfactory/samples/05_remove_layers.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/samples/06_remapping_layers.py` & `gdsfactory-6.92.0/gdsfactory/samples/06_remapping_layers.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/samples/07_flattening_device.py` & `gdsfactory-6.92.0/gdsfactory/samples/07_flattening_device.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/samples/11_component_layout.py` & `gdsfactory-6.92.0/gdsfactory/samples/11_component_layout.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/samples/12_component_refs.py` & `gdsfactory-6.92.0/gdsfactory/samples/12_component_refs.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/samples/13_component_netlist.py` & `gdsfactory-6.92.0/gdsfactory/samples/13_component_netlist.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/samples/14_component_connectivity.py` & `gdsfactory-6.92.0/gdsfactory/samples/14_component_connectivity.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/samples/15_component_sequence1.py` & `gdsfactory-6.92.0/gdsfactory/samples/15_component_sequence1.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/samples/16_component_sequence2.py` & `gdsfactory-6.92.0/gdsfactory/samples/16_component_sequence2.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/samples/17_ports.py` & `gdsfactory-6.92.0/gdsfactory/samples/17_ports.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/samples/20_components.py` & `gdsfactory-6.92.0/gdsfactory/samples/20_components.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/samples/22_add_pads.py` & `gdsfactory-6.92.0/gdsfactory/samples/22_add_pads.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/samples/23_reticle.py` & `gdsfactory-6.92.0/gdsfactory/samples/23_reticle.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/samples/23_reticle_passives.py` & `gdsfactory-6.92.0/gdsfactory/samples/23_reticle_passives.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/samples/24_doe_2.py` & `gdsfactory-6.92.0/gdsfactory/samples/24_doe_2.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/samples/24_doe_3.py` & `gdsfactory-6.92.0/gdsfactory/samples/24_doe_3.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/samples/30_lidar.py` & `gdsfactory-6.92.0/gdsfactory/samples/30_lidar.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/samples/30_lidar_pcell.py` & `gdsfactory-6.92.0/gdsfactory/samples/30_lidar_pcell.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/samples/30_lidar_with_pads.py` & `gdsfactory-6.92.0/gdsfactory/samples/30_lidar_with_pads.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/samples/all_angle_routing.py` & `gdsfactory-6.92.0/gdsfactory/samples/all_angle_routing.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/samples/all_angle_routing/aar_basic_01.pic.yml` & `gdsfactory-6.92.0/gdsfactory/samples/all_angle_routing/aar_basic_01.pic.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/samples/all_angle_routing/aar_bundles.pic.yml` & `gdsfactory-6.92.0/gdsfactory/samples/all_angle_routing/aar_bundles.pic.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/samples/all_angle_routing/aar_gone_wrong.pic.yml` & `gdsfactory-6.92.0/gdsfactory/samples/all_angle_routing/aar_gone_wrong.pic.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/samples/all_angle_routing/aar_implicit_final_angle.pic.yml` & `gdsfactory-6.92.0/gdsfactory/samples/all_angle_routing/aar_implicit_final_angle.pic.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/samples/all_angle_routing/aar_slalom.pic.yml` & `gdsfactory-6.92.0/gdsfactory/samples/all_angle_routing/aar_slalom.pic.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/samples/all_angle_routing/aar_start_end_customizations.pic.yml` & `gdsfactory-6.92.0/gdsfactory/samples/all_angle_routing/aar_start_end_customizations.pic.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/samples/all_angle_routing/aar_step_definitions.pic.yml` & `gdsfactory-6.92.0/gdsfactory/samples/all_angle_routing/aar_step_definitions.pic.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/samples/all_angle_routing/aar_tricky_connections.pic.yml` & `gdsfactory-6.92.0/gdsfactory/samples/all_angle_routing/aar_tricky_connections.pic.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/samples/all_angle_routing/all_angle_routes.pic.yml` & `gdsfactory-6.92.0/gdsfactory/samples/all_angle_routing/all_angle_routes.pic.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/samples/big_device.py` & `gdsfactory-6.92.0/gdsfactory/samples/big_device.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/samples/demo/benchmark/fill_demo.py` & `gdsfactory-6.92.0/gdsfactory/samples/demo/benchmark/fill_demo.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/samples/demo/circuits/mask.pic.yml` & `gdsfactory-6.92.0/gdsfactory/samples/demo/circuits/mask.pic.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/samples/demo/circuits/mzi_lattice_filter.pic.yml` & `gdsfactory-6.92.0/gdsfactory/samples/demo/circuits/mzi_lattice_filter.pic.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/samples/demo/circuits/mzi_ubcpdk.pic.yml` & `gdsfactory-6.92.0/gdsfactory/samples/demo/circuits/mzi_ubcpdk.pic.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/samples/demo/drc_errors.py` & `gdsfactory-6.92.0/gdsfactory/samples/demo/drc_errors.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/samples/demo/drc_write.py` & `gdsfactory-6.92.0/gdsfactory/samples/demo/drc_write.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/samples/demo/layers.py` & `gdsfactory-6.92.0/gdsfactory/samples/demo/layers.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/samples/demo/lvs.py` & `gdsfactory-6.92.0/gdsfactory/samples/demo/lvs.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/samples/demo/pcell.py` & `gdsfactory-6.92.0/gdsfactory/samples/demo/pcell.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/samples/netlists/mzi.yml` & `gdsfactory-6.92.0/gdsfactory/samples/netlists/mzi.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/samples/netlists/mzi_full.yml` & `gdsfactory-6.92.0/gdsfactory/samples/netlists/mzi_full.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/samples/pdk/fab_c.py` & `gdsfactory-6.92.0/gdsfactory/samples/pdk/fab_c.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/samples/pdk/fab_d/phase_shifters.py` & `gdsfactory-6.92.0/gdsfactory/samples/pdk/fab_d/phase_shifters.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/samples/pdk/test_fab_c.py` & `gdsfactory-6.92.0/gdsfactory/samples/pdk/test_fab_c.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/samples/pdk/test_fab_c/test_settings_bend_euler_c_.yml` & `gdsfactory-6.92.0/gdsfactory/samples/pdk/test_fab_c/test_settings_bend_euler_c_.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/samples/pdk/test_fab_c/test_settings_bend_euler_nc_.yml` & `gdsfactory-6.92.0/gdsfactory/samples/pdk/test_fab_c/test_settings_bend_euler_nc_.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/samples/pdk/test_fab_c/test_settings_gc_nc_.yml` & `gdsfactory-6.92.0/gdsfactory/samples/pdk/test_fab_c/test_settings_gc_nc_.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/samples/pdk/test_fab_c/test_settings_gc_nitride_c_.yml` & `gdsfactory-6.92.0/gdsfactory/samples/pdk/test_fab_c/test_settings_gc_nitride_c_.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mmi1x2_nc_.yml` & `gdsfactory-6.92.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mmi1x2_nc_.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mmi1x2_nitride_c_.yml` & `gdsfactory-6.92.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mmi1x2_nitride_c_.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mmi1x2_nitride_o_.yml` & `gdsfactory-6.92.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mmi1x2_nitride_o_.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mmi1x2_no_.yml` & `gdsfactory-6.92.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mmi1x2_no_.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mzi_nc_.yml` & `gdsfactory-6.92.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mzi_nc_.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mzi_nitride_c_.yml` & `gdsfactory-6.92.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mzi_nitride_c_.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mzi_nitride_o_.yml` & `gdsfactory-6.92.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mzi_nitride_o_.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mzi_no_.yml` & `gdsfactory-6.92.0/gdsfactory/samples/pdk/test_fab_c/test_settings_mzi_no_.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/samples/pdk/test_fab_c/test_settings_straight_c_.yml` & `gdsfactory-6.92.0/gdsfactory/samples/pdk/test_fab_c/test_settings_straight_c_.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/samples/pdk/test_fab_c/test_settings_straight_nc_.yml` & `gdsfactory-6.92.0/gdsfactory/samples/pdk/test_fab_c/test_settings_straight_nc_.yml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/schematic_editor.py` & `gdsfactory-6.92.0/gdsfactory/schematic_editor.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/serialization.py` & `gdsfactory-6.92.0/gdsfactory/serialization.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/show.py` & `gdsfactory-6.92.0/gdsfactory/show.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/__init__.py` & `gdsfactory-6.92.0/gdsfactory/simulation/__init__.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/add_simulation_markers.py` & `gdsfactory-6.92.0/gdsfactory/simulation/add_simulation_markers.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/convert_sparameters.py` & `gdsfactory-6.92.0/gdsfactory/simulation/convert_sparameters.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/devsim/__init__.py` & `gdsfactory-6.92.0/gdsfactory/simulation/devsim/__init__.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/devsim/doping.py` & `gdsfactory-6.92.0/gdsfactory/simulation/devsim/doping.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/devsim/get_simulation.py` & `gdsfactory-6.92.0/gdsfactory/simulation/devsim/get_simulation.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/devsim/get_simulation_xsection.py` & `gdsfactory-6.92.0/gdsfactory/simulation/devsim/get_simulation_xsection.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/devsim/get_solver.py` & `gdsfactory-6.92.0/gdsfactory/simulation/devsim/get_solver.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/devsim/test_devsim.py` & `gdsfactory-6.92.0/gdsfactory/simulation/devsim/test_devsim.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/eme/meow_eme.py` & `gdsfactory-6.92.0/gdsfactory/simulation/eme/meow_eme.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/eme/test_meow_simulation.py` & `gdsfactory-6.92.0/gdsfactory/simulation/eme/test_meow_simulation.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/fem/mode_solver.py` & `gdsfactory-6.92.0/gdsfactory/simulation/fem/mode_solver.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/fem/test_mode_solver.py` & `gdsfactory-6.92.0/gdsfactory/simulation/fem/test_mode_solver.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/get_effective_indices.py` & `gdsfactory-6.92.0/gdsfactory/simulation/get_effective_indices.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/get_modes_path.py` & `gdsfactory-6.92.0/gdsfactory/simulation/get_modes_path.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/get_sparameters_path.py` & `gdsfactory-6.92.0/gdsfactory/simulation/get_sparameters_path.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/gmeep/__init__.py` & `gdsfactory-6.92.0/gdsfactory/simulation/gmeep/__init__.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/gmeep/get_material.py` & `gdsfactory-6.92.0/gdsfactory/simulation/gmeep/get_material.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/gmeep/get_meep_geometry.py` & `gdsfactory-6.92.0/gdsfactory/simulation/gmeep/get_meep_geometry.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/gmeep/get_port_eigenmode.py` & `gdsfactory-6.92.0/gdsfactory/simulation/gmeep/get_port_eigenmode.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/gmeep/get_simulation.py` & `gdsfactory-6.92.0/gdsfactory/simulation/gmeep/get_simulation.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/gmeep/get_simulation_grating_farfield.py` & `gdsfactory-6.92.0/gdsfactory/simulation/gmeep/get_simulation_grating_farfield.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/gmeep/get_simulation_grating_fiber.py` & `gdsfactory-6.92.0/gdsfactory/simulation/gmeep/get_simulation_grating_fiber.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/gmeep/meep_adjoint_optimization.py` & `gdsfactory-6.92.0/gdsfactory/simulation/gmeep/meep_adjoint_optimization.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/gmeep/test_eigenmode.py` & `gdsfactory-6.92.0/gdsfactory/simulation/gmeep/test_eigenmode.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/gmeep/test_materials.py` & `gdsfactory-6.92.0/gdsfactory/simulation/gmeep/test_materials.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/gmeep/test_sparameterNxN/test_sparameterNxN_crossing.csv` & `gdsfactory-6.92.0/gdsfactory/simulation/gmeep/test_sparameterNxN/test_sparameterNxN_crossing.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/gmeep/test_sparameterNxN/test_sparameterNxN_straight.csv` & `gdsfactory-6.92.0/gdsfactory/simulation/gmeep/test_sparameterNxN/test_sparameterNxN_straight.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep.py` & `gdsfactory-6.92.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameterNxN_crossing.csv` & `gdsfactory-6.92.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameterNxN_crossing.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameterNxN_straight.csv` & `gdsfactory-6.92.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameterNxN_straight.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameterNxN_symmetries_straight.csv` & `gdsfactory-6.92.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameterNxN_symmetries_straight.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameter_straight_mpi.csv` & `gdsfactory-6.92.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameter_straight_mpi.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameter_straight_mpi_pool.csv` & `gdsfactory-6.92.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameter_straight_mpi_pool.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameters_crossing_symmetric.csv` & `gdsfactory-6.92.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameters_crossing_symmetric.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameters_straight.csv` & `gdsfactory-6.92.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameters_straight.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameters_straight_batch.csv` & `gdsfactory-6.92.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameters_straight_batch.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameters_straight_mpi.csv` & `gdsfactory-6.92.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameters_straight_mpi.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameters_straight_mpi_pool.csv` & `gdsfactory-6.92.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameters_straight_mpi_pool.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameters_straight_symmetric.csv` & `gdsfactory-6.92.0/gdsfactory/simulation/gmeep/test_write_sparameters_meep/test_sparameters_straight_symmetric.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/gmeep/write_sparameters_grating.py` & `gdsfactory-6.92.0/gdsfactory/simulation/gmeep/write_sparameters_grating.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/gmeep/write_sparameters_meep.py` & `gdsfactory-6.92.0/gdsfactory/simulation/gmeep/write_sparameters_meep.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/gmeep/write_sparameters_meep_batch.py` & `gdsfactory-6.92.0/gdsfactory/simulation/gmeep/write_sparameters_meep_batch.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/gmeep/write_sparameters_meep_mpi.py` & `gdsfactory-6.92.0/gdsfactory/simulation/gmeep/write_sparameters_meep_mpi.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/gmsh/__init__.py` & `gdsfactory-6.92.0/gdsfactory/simulation/gmsh/__init__.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/gmsh/break_geometry.py` & `gdsfactory-6.92.0/gdsfactory/simulation/gmsh/break_geometry.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/gmsh/mesh.py` & `gdsfactory-6.92.0/gdsfactory/simulation/gmsh/mesh.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/gmsh/meshtracker.py` & `gdsfactory-6.92.0/gdsfactory/simulation/gmsh/meshtracker.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/gmsh/parse_component.py` & `gdsfactory-6.92.0/gdsfactory/simulation/gmsh/parse_component.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/gmsh/parse_gds.py` & `gdsfactory-6.92.0/gdsfactory/simulation/gmsh/parse_gds.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/gmsh/parse_layerstack.py` & `gdsfactory-6.92.0/gdsfactory/simulation/gmsh/parse_layerstack.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/gmsh/refine.py` & `gdsfactory-6.92.0/gdsfactory/simulation/gmsh/refine.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/gmsh/scratch/mesh3D.py` & `gdsfactory-6.92.0/gdsfactory/simulation/gmsh/scratch/mesh3D.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/gmsh/tests/test_meshing.py` & `gdsfactory-6.92.0/gdsfactory/simulation/gmsh/tests/test_meshing.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/gmsh/uz_xsection_mesh.py` & `gdsfactory-6.92.0/gdsfactory/simulation/gmsh/uz_xsection_mesh.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/gmsh/xy_xsection_mesh.py` & `gdsfactory-6.92.0/gdsfactory/simulation/gmsh/xy_xsection_mesh.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/gmsh/xyz_mesh.py` & `gdsfactory-6.92.0/gdsfactory/simulation/gmsh/xyz_mesh.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/gtidy3d/__init__.py` & `gdsfactory-6.92.0/gdsfactory/simulation/gtidy3d/__init__.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/gtidy3d/get_results.py` & `gdsfactory-6.92.0/gdsfactory/simulation/gtidy3d/get_results.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/gtidy3d/get_simulation.py` & `gdsfactory-6.92.0/gdsfactory/simulation/gtidy3d/get_simulation.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/gtidy3d/get_simulation_grating_coupler.py` & `gdsfactory-6.92.0/gdsfactory/simulation/gtidy3d/get_simulation_grating_coupler.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/gtidy3d/materials.py` & `gdsfactory-6.92.0/gdsfactory/simulation/gtidy3d/materials.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/gtidy3d/modes.py` & `gdsfactory-6.92.0/gdsfactory/simulation/gtidy3d/modes.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/gtidy3d/sim_run.yaml` & `gdsfactory-6.92.0/gdsfactory/simulation/gtidy3d/sim_run.yaml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/gtidy3d/tests/sim_ref.yaml` & `gdsfactory-6.92.0/gdsfactory/simulation/gtidy3d/tests/sim_ref.yaml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/gtidy3d/tests/sim_run.yaml` & `gdsfactory-6.92.0/gdsfactory/simulation/gtidy3d/tests/sim_run.yaml`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/gtidy3d/tests/test_modes.py` & `gdsfactory-6.92.0/gdsfactory/simulation/gtidy3d/tests/test_modes.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/gtidy3d/tests/test_results.py` & `gdsfactory-6.92.0/gdsfactory/simulation/gtidy3d/tests/test_results.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/gtidy3d/tests/test_simulation.py` & `gdsfactory-6.92.0/gdsfactory/simulation/gtidy3d/tests/test_simulation.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/gtidy3d/tests/test_write_sparameters.py` & `gdsfactory-6.92.0/gdsfactory/simulation/gtidy3d/tests/test_write_sparameters.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/gtidy3d/tests/test_write_sparameters/test_sparameters_straight.csv` & `gdsfactory-6.92.0/gdsfactory/simulation/gtidy3d/tests/test_write_sparameters/test_sparameters_straight.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/gtidy3d/tests/test_write_sparameters_grating_coupler.py` & `gdsfactory-6.92.0/gdsfactory/simulation/gtidy3d/tests/test_write_sparameters_grating_coupler.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/gtidy3d/utils.py` & `gdsfactory-6.92.0/gdsfactory/simulation/gtidy3d/utils.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/gtidy3d/write_sparameters.py` & `gdsfactory-6.92.0/gdsfactory/simulation/gtidy3d/write_sparameters.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/gtidy3d/write_sparameters_grating_coupler.py` & `gdsfactory-6.92.0/gdsfactory/simulation/gtidy3d/write_sparameters_grating_coupler.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/lumerical/__init__.py` & `gdsfactory-6.92.0/gdsfactory/simulation/lumerical/__init__.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/lumerical/interconnect.py` & `gdsfactory-6.92.0/gdsfactory/simulation/lumerical/interconnect.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/lumerical/read.py` & `gdsfactory-6.92.0/gdsfactory/simulation/lumerical/read.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/lumerical/settings.py` & `gdsfactory-6.92.0/gdsfactory/simulation/lumerical/settings.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/lumerical/test_read_sparameters.py` & `gdsfactory-6.92.0/gdsfactory/simulation/lumerical/test_read_sparameters.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/lumerical/write_sparameters_lumerical.py` & `gdsfactory-6.92.0/gdsfactory/simulation/lumerical/write_sparameters_lumerical.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/lumerical/write_sparameters_lumerical_components.py` & `gdsfactory-6.92.0/gdsfactory/simulation/lumerical/write_sparameters_lumerical_components.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/modes/__init__.py` & `gdsfactory-6.92.0/gdsfactory/simulation/modes/__init__.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/modes/coupler.py` & `gdsfactory-6.92.0/gdsfactory/simulation/modes/coupler.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/modes/find_coupling_vs_gap.py` & `gdsfactory-6.92.0/gdsfactory/simulation/modes/find_coupling_vs_gap.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/modes/find_mode_dispersion.py` & `gdsfactory-6.92.0/gdsfactory/simulation/modes/find_mode_dispersion.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/modes/find_modes.py` & `gdsfactory-6.92.0/gdsfactory/simulation/modes/find_modes.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/modes/find_modes_cross_section.py` & `gdsfactory-6.92.0/gdsfactory/simulation/modes/find_modes_cross_section.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/modes/find_neff_ng_dw_dh.py` & `gdsfactory-6.92.0/gdsfactory/simulation/modes/find_neff_ng_dw_dh.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/modes/find_neff_vs_width.py` & `gdsfactory-6.92.0/gdsfactory/simulation/modes/find_neff_vs_width.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/modes/get_mode_solver_coupler.py` & `gdsfactory-6.92.0/gdsfactory/simulation/modes/get_mode_solver_coupler.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/modes/get_mode_solver_cross_section.py` & `gdsfactory-6.92.0/gdsfactory/simulation/modes/get_mode_solver_cross_section.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/modes/get_mode_solver_rib.py` & `gdsfactory-6.92.0/gdsfactory/simulation/modes/get_mode_solver_rib.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/modes/modes/neff_vs_width_nitride.csv` & `gdsfactory-6.92.0/gdsfactory/simulation/modes/modes/neff_vs_width_nitride.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/modes/modes/neff_vs_width_rib.csv` & `gdsfactory-6.92.0/gdsfactory/simulation/modes/modes/neff_vs_width_rib.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/modes/modes/neff_vs_width_strip.csv` & `gdsfactory-6.92.0/gdsfactory/simulation/modes/modes/neff_vs_width_strip.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/modes/neff_convergence_test.py` & `gdsfactory-6.92.0/gdsfactory/simulation/modes/neff_convergence_test.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/modes/overlap.py` & `gdsfactory-6.92.0/gdsfactory/simulation/modes/overlap.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/modes/tests/test_dw_dh/test_dw_dh_dispersion.csv` & `gdsfactory-6.92.0/gdsfactory/simulation/modes/tests/test_dw_dh/test_dw_dh_dispersion.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/modes/tests/test_find_modes.py` & `gdsfactory-6.92.0/gdsfactory/simulation/modes/tests/test_find_modes.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/modes/tests/test_find_modes_dispersion.py` & `gdsfactory-6.92.0/gdsfactory/simulation/modes/tests/test_find_modes_dispersion.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/modes/types.py` & `gdsfactory-6.92.0/gdsfactory/simulation/modes/types.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/modes/waveguide.py` & `gdsfactory-6.92.0/gdsfactory/simulation/modes/waveguide.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/photonic_circuit_models/__init__.py` & `gdsfactory-6.92.0/gdsfactory/simulation/photonic_circuit_models/__init__.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/photonic_circuit_models/coupler.py` & `gdsfactory-6.92.0/gdsfactory/simulation/photonic_circuit_models/coupler.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/photonic_circuit_models/mzi.py` & `gdsfactory-6.92.0/gdsfactory/simulation/photonic_circuit_models/mzi.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/photonic_circuit_models/ring.py` & `gdsfactory-6.92.0/gdsfactory/simulation/photonic_circuit_models/ring.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/plot.py` & `gdsfactory-6.92.0/gdsfactory/simulation/plot.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/plot_csv.py` & `gdsfactory-6.92.0/gdsfactory/simulation/plot_csv.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/port_symmetries.py` & `gdsfactory-6.92.0/gdsfactory/simulation/port_symmetries.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/process/diffusion.py` & `gdsfactory-6.92.0/gdsfactory/simulation/process/diffusion.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/process/implant_tables.py` & `gdsfactory-6.92.0/gdsfactory/simulation/process/implant_tables.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/process/pysrim.py` & `gdsfactory-6.92.0/gdsfactory/simulation/process/pysrim.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/process/silicon.py` & `gdsfactory-6.92.0/gdsfactory/simulation/process/silicon.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/process/skew/antimony_si_skew.csv` & `gdsfactory-6.92.0/gdsfactory/simulation/process/skew/antimony_si_skew.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/process/skew/arsenic_si_skew.csv` & `gdsfactory-6.92.0/gdsfactory/simulation/process/skew/arsenic_si_skew.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/process/skew/boron_si_skew.csv` & `gdsfactory-6.92.0/gdsfactory/simulation/process/skew/boron_si_skew.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/process/skew/phosphorus_si_skew.csv` & `gdsfactory-6.92.0/gdsfactory/simulation/process/skew/phosphorus_si_skew.csv`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/sax/build_model.py` & `gdsfactory-6.92.0/gdsfactory/simulation/sax/build_model.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/sax/femwell_waveguide_model.py` & `gdsfactory-6.92.0/gdsfactory/simulation/sax/femwell_waveguide_model.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/sax/interpolators.py` & `gdsfactory-6.92.0/gdsfactory/simulation/sax/interpolators.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/sax/meep_FDTD_model.py` & `gdsfactory-6.92.0/gdsfactory/simulation/sax/meep_FDTD_model.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/sax/meow_eme_model.py` & `gdsfactory-6.92.0/gdsfactory/simulation/sax/meow_eme_model.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/sax/mlp.py` & `gdsfactory-6.92.0/gdsfactory/simulation/sax/mlp.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/sax/models.py` & `gdsfactory-6.92.0/gdsfactory/simulation/sax/models.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/sax/parameter.py` & `gdsfactory-6.92.0/gdsfactory/simulation/sax/parameter.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/sax/plot_model.py` & `gdsfactory-6.92.0/gdsfactory/simulation/sax/plot_model.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/sax/read.py` & `gdsfactory-6.92.0/gdsfactory/simulation/sax/read.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/sax/tests/test_mzi.py` & `gdsfactory-6.92.0/gdsfactory/simulation/sax/tests/test_mzi.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/sax/tests/test_mzi_lattice.py` & `gdsfactory-6.92.0/gdsfactory/simulation/sax/tests/test_mzi_lattice.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/sax/tests/test_parameters.py` & `gdsfactory-6.92.0/gdsfactory/simulation/sax/tests/test_parameters.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/simphony/__init__.py` & `gdsfactory-6.92.0/gdsfactory/simulation/simphony/__init__.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/simphony/add_gc.py` & `gdsfactory-6.92.0/gdsfactory/simulation/simphony/add_gc.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/simphony/circuit.py` & `gdsfactory-6.92.0/gdsfactory/simulation/simphony/circuit.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/simphony/components/__init__.py` & `gdsfactory-6.92.0/gdsfactory/simulation/simphony/components/__init__.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/simphony/components/bend_circular.py` & `gdsfactory-6.92.0/gdsfactory/simulation/simphony/components/bend_circular.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/simphony/components/bend_euler.py` & `gdsfactory-6.92.0/gdsfactory/simulation/simphony/components/bend_euler.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/simphony/components/coupler.py` & `gdsfactory-6.92.0/gdsfactory/simulation/simphony/components/coupler.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/simphony/components/coupler_fdtd.py` & `gdsfactory-6.92.0/gdsfactory/simulation/simphony/components/coupler_fdtd.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/simphony/components/coupler_ring.py` & `gdsfactory-6.92.0/gdsfactory/simulation/simphony/components/coupler_ring.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/simphony/components/coupler_ring_fdtd.py` & `gdsfactory-6.92.0/gdsfactory/simulation/simphony/components/coupler_ring_fdtd.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/simphony/components/coupler_ring_siepic.py` & `gdsfactory-6.92.0/gdsfactory/simulation/simphony/components/coupler_ring_siepic.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/simphony/components/gc.py` & `gdsfactory-6.92.0/gdsfactory/simulation/simphony/components/gc.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/simphony/components/mmi1x2.py` & `gdsfactory-6.92.0/gdsfactory/simulation/simphony/components/mmi1x2.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/simphony/components/mmi2x2.py` & `gdsfactory-6.92.0/gdsfactory/simulation/simphony/components/mmi2x2.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/simphony/components/mzi.py` & `gdsfactory-6.92.0/gdsfactory/simulation/simphony/components/mzi.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/simphony/components/mzi_siepic.py` & `gdsfactory-6.92.0/gdsfactory/simulation/simphony/components/mzi_siepic.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/simphony/components/ring_double.py` & `gdsfactory-6.92.0/gdsfactory/simulation/simphony/components/ring_double.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/simphony/components/ring_double_siepic.py` & `gdsfactory-6.92.0/gdsfactory/simulation/simphony/components/ring_double_siepic.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/simphony/components/ring_single.py` & `gdsfactory-6.92.0/gdsfactory/simulation/simphony/components/ring_single.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/simphony/components/ring_single_siepic.py` & `gdsfactory-6.92.0/gdsfactory/simulation/simphony/components/ring_single_siepic.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/simphony/components/straight.py` & `gdsfactory-6.92.0/gdsfactory/simulation/simphony/components/straight.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/simphony/get_transmission.py` & `gdsfactory-6.92.0/gdsfactory/simulation/simphony/get_transmission.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/simphony/model_from_gdsfactory.py` & `gdsfactory-6.92.0/gdsfactory/simulation/simphony/model_from_gdsfactory.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/simphony/model_from_sparameters.py` & `gdsfactory-6.92.0/gdsfactory/simulation/simphony/model_from_sparameters.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/simphony/plot_circuit.py` & `gdsfactory-6.92.0/gdsfactory/simulation/simphony/plot_circuit.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/simphony/plot_circuit_montecarlo.py` & `gdsfactory-6.92.0/gdsfactory/simulation/simphony/plot_circuit_montecarlo.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/simphony/plot_model.py` & `gdsfactory-6.92.0/gdsfactory/simulation/simphony/plot_model.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/simphony/tests/test_circuit.py` & `gdsfactory-6.92.0/gdsfactory/simulation/simphony/tests/test_circuit.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/simphony/tests/test_components.py` & `gdsfactory-6.92.0/gdsfactory/simulation/simphony/tests/test_components.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/sipann/bend_circular.py` & `gdsfactory-6.92.0/gdsfactory/simulation/sipann/bend_circular.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/sipann/bend_euler.py` & `gdsfactory-6.92.0/gdsfactory/simulation/sipann/bend_euler.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/sipann/coupler.py` & `gdsfactory-6.92.0/gdsfactory/simulation/sipann/coupler.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/sipann/coupler_ring.py` & `gdsfactory-6.92.0/gdsfactory/simulation/sipann/coupler_ring.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/sipann/straight.py` & `gdsfactory-6.92.0/gdsfactory/simulation/sipann/straight.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/simulation/thermal/heater.py` & `gdsfactory-6.92.0/gdsfactory/simulation/thermal/heater.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/snap.py` & `gdsfactory-6.92.0/gdsfactory/snap.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/symbols.py` & `gdsfactory-6.92.0/gdsfactory/symbols.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/technology/__init__.py` & `gdsfactory-6.92.0/gdsfactory/technology/__init__.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/technology/klayout_tech.py` & `gdsfactory-6.92.0/gdsfactory/technology/klayout_tech.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/technology/layer_map.py` & `gdsfactory-6.92.0/gdsfactory/technology/layer_map.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/technology/layer_stack.py` & `gdsfactory-6.92.0/gdsfactory/technology/layer_stack.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/technology/layer_views.py` & `gdsfactory-6.92.0/gdsfactory/technology/layer_views.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/technology/simulation_settings.py` & `gdsfactory-6.92.0/gdsfactory/technology/simulation_settings.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/types.py` & `gdsfactory-6.92.0/gdsfactory/types.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/typings.py` & `gdsfactory-6.92.0/gdsfactory/typings.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/utils/async_utils.py` & `gdsfactory-6.92.0/gdsfactory/utils/async_utils.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/utils/file_utils.py` & `gdsfactory-6.92.0/gdsfactory/utils/file_utils.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/utils/xml_utils.py` & `gdsfactory-6.92.0/gdsfactory/utils/xml_utils.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/utils/yaml_utils.py` & `gdsfactory-6.92.0/gdsfactory/utils/yaml_utils.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/watch.py` & `gdsfactory-6.92.0/gdsfactory/watch.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/widgets/layout_viewer.py` & `gdsfactory-6.92.0/gdsfactory/widgets/layout_viewer.py`

 * *Files identical despite different names*

### Comparing `gdsfactory-6.91.0/gdsfactory/write_cells.py` & `gdsfactory-6.92.0/gdsfactory/write_cells.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,25 +79,25 @@
     Args:
         dirpath: fixed cell directory path.
         module: Optional plot directive to plot imported component.
 
     """
     dirpath = pathlib.Path(dirpath)
     if not dirpath.exists():
-        raise ValueError(f"{dirpath.absolute()!r} does not exist.")
+        raise ValueError(f"{str(dirpath.absolute())!r} does not exist.")
 
     gdspaths = list(dirpath.glob("*.gds")) + list(dirpath.glob("*.GDS"))
 
     if not gdspaths:
         raise ValueError(f"No GDS files found at {dirpath.absolute()!r}.")
 
     logger.info(f"Writing {len(gdspaths)} cells from {dirpath.absolute()!r}")
 
     script = [script_prefix]
-    script += [f"gdsdir = {dirpath.absolute()!r}\n"]
+    script += [f"gdsdir = {str(dirpath.absolute())!r}\n"]
     script += [
         "import_gds = partial(gf.import_gds, gdsdir=gdsdir, decorator=add_ports)\n"
     ]
 
     cells = [get_script(gdspath, module=module) for gdspath in gdspaths]
     script += sorted(cells)
     return "\n".join(script)
```

### Comparing `gdsfactory-6.91.0/pyproject.toml` & `gdsfactory-6.92.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
   "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Operating System :: OS Independent",
 ]
-version = "6.91.0"
+version = "6.92.0"
 authors = [
 {name = "gdsfactory community", email = "contact@gdsfactory.com"},
 ]
 keywords = ["eda", "photonics", "python"]
 license = {file = "LICENSE"}
 dependencies = [
   "click",
```

### Comparing `gdsfactory-6.91.0/PKG-INFO` & `gdsfactory-6.92.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gdsfactory
-Version: 6.91.0
+Version: 6.92.0
 Summary: python library to generate GDS layouts
 Keywords: eda,photonics,python
 Author-email: gdsfactory community <contact@gdsfactory.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -110,15 +110,15 @@
 Provides-Extra: full
 Provides-Extra: gmsh
 Provides-Extra: meow
 Provides-Extra: ray
 Provides-Extra: sax
 Provides-Extra: tidy3d
 
-# gdsfactory 6.91.0
+# gdsfactory 6.92.0
 
 [![docs](https://github.com/gdsfactory/gdsfactory/actions/workflows/pages.yml/badge.svg)](https://gdsfactory.github.io/gdsfactory/)
 [![PyPI](https://img.shields.io/pypi/v/gdsfactory)](https://pypi.org/project/gdsfactory/)
 [![Conda Version](https://img.shields.io/conda/vn/conda-forge/gdsfactory.svg)](https://anaconda.org/conda-forge/gdsfactory)
 [![Dockerhub](https://img.shields.io/docker/pulls/joamatab/gdsfactory)](https://hub.docker.com/r/joamatab/gdsfactory)
 [![PyPI Python](https://img.shields.io/pypi/pyversions/gdsfactory.svg)](https://pypi.python.org/pypi/gdsfactory)
 [![issues](https://img.shields.io/github/issues/gdsfactory/gdsfactory)](https://github.com/gdsfactory/gdsfactory/issues)
@@ -339,15 +339,14 @@
 
 ---
 
 "I use gdsfactory for all of my photonic tape-outs. The Python interface makes it easy to version control individual photonic components as well as entire layouts, while integrating seamlessly with KLayout and most standard photonic simulation tools, both open-source and commercial.
 
 <div style="text-align: right; margin-right: 10%;">Thomas Dorch - <strong>Freedom Photonics</strong></div>
 
-<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
-<!-- prettier-ignore-start -->
-<!-- markdownlint-disable -->
-<!-- markdownlint-restore -->
-<!-- prettier-ignore-end -->
 
-<!-- ALL-CONTRIBUTORS-LIST:END -->
+## Contributors
+
+Thanks to all the contributors that make this awesome project possible!
+
+[![Meet our contributors!](https://contrib.rocks/image?repo=gdsfactory/gdsfactory)](https://github.com/gdsfactory/gdsfactory/graphs/contributors)
```

